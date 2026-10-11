---
title: "CMOS-VLSI-design.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_9c494ac7201adddbd2c2721f643f4ca97295230462135641
file_size: 14503637
---

FOURTH EDITION


CMOnVLSI DESIGN A CIRCUITS AND


SYSTEMS PERSPECTIVE


NEIL H.E.WESTEDAVID MONEY HARRIS


Fourth Edition


CMOS VLSI Design


A Circuits and Systems Perspective


This page intentionally left blank


Neil H. E. Weste


Macquarie University and The University of Adelaide


David Money Harris


Harvey Mudd College


Addison-Wesley


Boston   Columbus   Indianapolis   New York   San Francisco   Upper Saddle River


Amsterdam   Cape Town   Dubai   London   Madrid   Milan  Munich  Paris  Montreal  Toronto  Delhi  Mexico City  Sao Paulo  Sydney  Hong Kong  Seoul  Singapore  Taipei  Tokyo


Editor in Chief:  Michael Hirsch


Acquisitions Editor:  Matt Goldstein


Editorial Assistant:  Chelsea Bell


Managing Editor:  Jeffrey Holcomb


Senior Production Project Manager:  Marilyn Lloyd


Media Producer:  Katelyn Boller


Director of Marketing:  Margaret Waples


Marketing Coordinator:  Kathryn Ferranti


Senior Manufacturing Buyer:  Carol Melville


Senior Media Buyer:  Ginny Michaud


Text Designer:  Susan Raymond


Art Director, Cover:  Linda Knowles


Cover Designer:  Joyce Cosentino Wells/J Wells Design


Cover Image:  Cover photograph courtesy of Nick Knupffer—Intel Corporation.


Copyright © 2009 Intel Corporation. All rights reserved.


Full Service Vendor:  Gillian Hall/The Aardvark Group Publishing Service


Copyeditor:  Kathleen Cantwell, C4 Technologies


Proofreader:  Holly McLean-Aldis


Indexer:  Jack Lewis


Printer/Binder:  Edwards Brothers


Cover Printer:  Lehigh-Phoenix Color/Hagerstown


Credits and acknowledgments borrowed from other sources and reproduced with permission in this textbook appear on appropriate page within text or on page 838.


The interior of this book was set in Adobe Caslon and Trade Gothic.


Copyright © 2011, 2005, 1993, 1985 Pearson Education, Inc., publishing as Addison-Wesley. All rights reserved. Manufactured in the United States of America. This publication is protected by Copyright, and permission should be obtained from the publisher prior to any prohibited reproduction, storage in a retrieval system, or transmission in any form or by any means, electronic, mechanical, photocopying, recording, or likewise. To obtain permission(s) to use material from this work,please submit a written request to Pearson Education, Inc., Permissions Department, 501 Boylston Street, Suite 900, Boston, Massachusetts 02116.


Many of the designations by manufacturers and sellers to distinguish their products are claimed as trademarks. Where those designations appear in this book, and the publisher was aware of a trademark claim, the designations have been printed in initial caps or all caps.


Cataloging-in-Publication Data is


on ﬁle with the Library of Congress.


10  9  8  7  6  5  4  3  2  1—EB—14 13 12 11 10 ISBN 10: 0-321-54774-8


ISBN 13: 978-0-321-54774-3


is an imprint of


To Avril, Melissa, Tamara, Nicky, Jocelyn,Makayla, Emily, Danika, Dan and Simon


N. W.


To Jennifer, Samuel, and Abraham


D. M. H.


vii


Preface   xxv


Chapter 1  Introduction


|1.1 |A Brief History  . . . . . . . . . . . . . . . . . . . . . . . . . |A Brief History  . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . 1 |
|---|---|---|---|

|1.2 |Preview . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |Preview . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . 6 |

|1.3 |MOS Transistors . . . . . . . . . . . . . . . . . . . . . . . . |MOS Transistors . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . 6 |

||CMOS Logic . . . . . . . . . . . . . . . . . . . . . . . . . . . |CMOS Logic . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . 9 |

|1.4 |1.4.1 The Inverter    9 |||

||1.4.2 The NAND |Gate    9 ||

||1.4.3 CMOS Logic |Gates    9 ||

||1.4.4 The NOR Gate |11 ||

||1.4.5 Compound |Gates    11 ||

||1.4.6 Pass Transistors |and Transmission Gates |12 |

||1.4.7 Tristates    14 |||

||1.4.8 Multiplexers |15 ||

||1.4.9 Sequential |Circuits    16 ||

|1.5 |CMOS Fabrication and |Layout . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . 19 |

||1.5.1 Inverter |Cross-Section    19 ||

||1.5.2 Fabrication |Process    20 ||

||1.5.3 Layout Design |Rules    24 ||

||1.5.4 Gate Layouts |27 ||

||1.5.5 Stick Diagrams |28 ||

|1.6 |Design Partitioning  . . . |. . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . 29 |

||1.6.1 Design |Abstractions   30 ||

||1.6.2 Structured |Design    31 ||

||1.6.3 Behavioral, Structural, |and Physical |Domains    31 |

|1.7 |Example: A Simple |MIPS Microprocessor  . . . . |. . . . . . . . . . . . . . . . . . . . . . . 33 |

||1.7.1 MIPS Architecture |33 ||

||1.7.2 Multicycle |MIPS Microarchitecture    34 ||

|1.8 |Logic Design . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . 38 |

||1.8.1 Top-Level Interfaces |38 ||

||1.8.2 Block Diagrams |38 ||

||1.8.3 Hierarchy    40 |||

||1.8.4 Hardware Description |Languages    40 ||

|1.9 |Circuit Design  . . . . . . . |. . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . 42 |

Contents


viii


1.10 Physical Design . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 45


1.10.1 Floorplanning    45


1.10.2 Standard Cells    48


1.10.3 Pitch Matching    50


1.10.4 Slice Plans    50


1.10.5 Arrays   51


1.10.6 Area Estimation   51


1.11 Design Veriﬁcation  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 53


1.12 Fabrication, Packaging, and Testing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 54


Summary and a Look Ahead    55


Exercises    57


Chapter 2  MOS Transistor Theory


2.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 61


2.2 Long-Channel I-V Characteristics  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 64


2.3 C-V Characteristics  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 68


2.3.1 Simple MOS Capacitance Models    68


2.3.2 Detailed MOS Gate Capacitance Model    70


2.3.3 Detailed MOS Diffusion Capacitance Model    72


2.4 Nonideal I-V Effects  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 74


2.4.1 Mobility Degradation and Velocity Saturation    75 75


2.4.2 Channel Length Modulation   78


2.4.3 Threshold Voltage Effects    79


2.4.4 Leakage    80


2.4.5 Temperature Dependence    85


2.4.6 Geometry Dependence    86


2.4.7 Summary    86


2.5 DC Transfer Characteristics  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 87


2.5.1 Static CMOS Inverter DC Characteristics    88


2.5.2 Beta Ratio Effects    90


2.5.3 Noise Margin    91


2.5.4 Pass Transistor DC Characteristics    92


2.6 Pitfalls and Fallacies  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 93 Summary 94


Exercises    95


Chapter 3  CMOS Processing Technology


3.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 99


3.2 CMOS Technologies  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 100


3.2.1 Wafer Formation    100


3.2.2 Photolithography    101


Contents ix


||3.2.3 Well and Channel |Formation |103 ||
|---|---|---|---|---|

||3.2.4 Silicon Dioxide |(SiO2)    105 |||

||3.2.5 Isolation |106 |||

||3.2.6 Gate Oxide |107 |||

||3.2.7 Gate and |Source/Drain Formations |108 ||

||3.2.8 Contacts and |Metallization    110 |||

||3.2.9 Passivation |112 |||

||3.2.10 Metrology |112 |||

|3.3 |Layout Design Rules |. . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . |. . . . . . . . . . 113 |

||3.3.1 Design Rule |Background    113 |||

||3.3.2 Scribe Line and |Other Structures |116 ||

||3.3.3 MOSIS |Scalable CMOS Design |Rules    117 ||

||3.3.4 Micron Design |Rules    118 |||

|3.4 |CMOS Process Enhancements |. . . . . . . |. . . . . . . . . . . . . . . . . . . |. . . . . . . . . . 119 |

||3.4.1 Transistors |119 |||

||3.4.2 Interconnect |122 |||

||3.4.3 Circuit Elements |124 |||

||3.4.4 Beyond Conventional |CMOS |129 ||

|3.5 |Technology-Related |CAD Issues . . . . . . |. . . . . . . . . . . . . . . . . . . |. . . . . . . . . . 130 |

||3.5.1 Design Rule |Checking (DRC) |131 ||

||3.5.2 Circuit Extraction |132 |||

|3.6 |Manufacturing |Issues  . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . |. . . . . . . . . . 133 |

||3.6.1 Antenna |Rules    133 |||

||3.6.2 Layer |Density Rules    134 |||

||3.6.3 Resolution Enhancement |Rules |134 ||

||3.6.4 Metal |Slotting Rules   135 |||

||3.6.5 Yield |Enhancement Guidelines |135 ||

|3.7 |Pitfalls and Fallacies |. . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . |. . . . . . . . . . 136 |

3.8 Historical Perspective . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 137 Summary  139


Exercises  139


Chapter 4  Delay


4.1 Introduction   . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 141


4.1.1 Deﬁnitions    141


4.1.2 Timing Optimization    142


4.2 Transient Response  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 143


4.3 RC Delay Model  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 146


4.3.1 Effective Resistance    146


4.3.2 Gate and Diffusion Capacitance    147


4.3.3 Equivalent RC Circuits    147


4.3.4 Transient Response    148


4.3.5 Elmore Delay    150


||4.3.6 Layout Dependence |of Capacitance    153 ||
|---|---|---|---|

||4.3.7 Determining |Effective Resistance    154 ||

|4.4 |Linear Delay |Model  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . 155 |

||4.4.1 Logical |Effort    156 ||

||4.4.2 Parasitic |Delay    156 ||

||4.4.3 Delay in a |Logic Gate    158 ||

||4.4.4 Drive |159 ||

||4.4.5 Extracting |Logical Effort from Datasheets   159 ||

||4.4.6 Limitations |to the Linear Delay Model   160 ||

|4.5 |Logical Effort of Paths |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . 163 |

||4.5.1 Delay in Multistage |Logic Networks    163 ||

||4.5.2 Choosing |the Best Number of Stages    166 ||

||4.5.3 Example |168 ||

||4.5.4 Summary |and Observations    169 ||

||4.5.5 Limitations |of Logical Effort    171 ||

||4.5.6 Iterative |Solutions for Sizing    171 ||

|4.6 |Timing Analysis Delay |Models . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . 173 |

||4.6.1 Slope-Based |Linear Model   173 ||

||4.6.2 Nonlinear |Delay Model    174 ||

||4.6.3 Current |Source Model    174 ||

|4.7 |Pitfalls and |Fallacies  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . 174 |

x


4.8 Historical Perspective . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 175 Summary  176


Exercises  176


Chapter 5  Power


5.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 181


||5.1.1 |Deﬁnitions    182 |181|
|---|---|---|---|

||5.1.2 |Examples    182 ||

||5.1.3 |Sources of Power Dissipation    184 ||

|5.2 |Dynamic |Power  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . 185 |

||5.2.1 Activity |Factor    186 ||

||5.2.2 Capacitance |188 ||

||5.2.3 |Voltage    190 ||

||5.2.4 Frequency |192 ||

||5.2.5 |Short-Circuit Current    193 ||

||5.2.6 Resonant |Circuits    193 ||

|5.3 |Static Power |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . 194 |

||5.3.1 Static |Power Sources    194 ||

||5.3.2 Power |Gating    197 ||

||5.3.3 |Multiple Threshold Voltages and Oxide Thicknesses |199 |

Contents xi


5.3.4 Variable Threshold Voltages    199


5.3.5 Input Vector Control   200


5.4 Energy-Delay Optimization . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 200


5.4.1 Minimum Energy    200


5.4.2 Minimum Energy-Delay Product    203


5.4.3 Minimum Energy Under a Delay Constraint    203


5.5 Low Power Architectures  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 204


5.5.1 Microarchitecture    204


5.5.2 Parallelism and Pipelining    204


5.5.3 Power Management Modes    205


5.6 Pitfalls and Fallacies . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 206


5.7 Historical Perspective . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 207


Summary  209


Exercises   209


Chapter 6  Interconnect


|6.1 |Introduction  . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . 211 |
|---|---|---|---|

||6.1.1 Wire Geometry |211 ||

||6.1.2 Example: |Intel Metal Stacks    212 ||

|6.2 |Interconnect |Modeling  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . 213 |

||6.2.1 Resistance |214 ||

||6.2.2 |Capacitance    215 ||

||6.2.3 Inductance |218 ||

||6.2.4 Skin Effect |219 ||

||6.2.5 |Temperature Dependence    220 ||

|6.3 |Interconnect |Impact . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . 220 |

||6.3.1 Delay |220 ||

||6.3.2 Energy |222 ||

||6.3.3 Crosstalk |222 ||

||6.3.4 Inductive |Effects    224 ||

||6.3.5 An Aside |on Effective Resistance and Elmore Delay   227 ||

|6.4 |Interconnect Engineering |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . 229 |

||6.4.1 Width, |Spacing, and Layer    229 ||

||6.4.2 Repeaters |230 ||

||6.4.3 Crosstalk |Control    232 ||

||6.4.4 Low-Swing |Signaling    234 ||

||6.4.5 |Regenerators    236 ||

|6.5 |Logical Effort with |Wires  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . 236 |

6.6 Pitfalls and Fallacies . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 237 Summary   238


Exercises  238


xii


Chapter 7  Robustness


|7.1 |Introduction . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . |. . . . 241 |
|---|---|---|---|---|

|7.2 |Variability . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . |. . . . 241 |

||7.2.1 Supply |Voltage    242 |||

||7.2.2 Temperature |242 |||

||7.2.3 Process |Variation    243 |||

||7.2.4 Design Corners |244 |||

|7.3 |Reliability . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . |. . . . 246 |

||7.3.1 Reliability |Terminology    246 |||

||7.3.2 Oxide Wearout |247 |||

||7.3.3 Interconnect |Wearout    249 |||

||7.3.4 Soft Errors |251 |||

||7.3.5 Overvoltage |Failure    252 |||

||7.3.6 Latchup |253 |||

|7.4 |Scaling . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . |. . . . 254 |

||7.4.1 Transistor Scaling |255 |||

||7.4.2 Interconnect |Scaling    257 |||

||7.4.3 International |Technology Roadmap for Semiconductors |258 ||

||7.4.4 Impacts on |Design    259 |||

|7.5 |Statistical Analysis |of Variability . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . |. . . . 263 |

||7.5.1 Properties of |Random Variables    263 |||

||7.5.2 Variation Sources |266 |||

||7.5.3 Variation Impacts |269 |||

|7.6 |Variation-Tolerant |Design . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . |. . . . 274 |

||7.6.1 Adaptive Control |275 |||

||7.6.2 Fault Tolerance |275 |||

|7.7 |Pitfalls and Fallacies |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . |. . . . 277 |

7.8 Historical Perspective . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 278 Summary  284


Exercises 284


Chapter 8  Circuit Simulation


8.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 287


8.2 A SPICE Tutorial  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 288


8.2.1 Sources and Passive Components    288


8.2.2 Transistor DC Analysis    292


8.2.3 Inverter Transient Analysis    292


8.2.4 Subcircuits and Measurement    294


8.2.5 Optimization    296


8.2.6 Other HSPICE Commands    298


Contents xiii


|8.3 |Device Models  . |. . . . . . . . . . . . . . . . . . . . |. . . . |. . . . . . . . . . . . . . . . . . . . . . . . 298 |
|---|---|---|---|---|

||8.3.1 Level 1 |Models    299 |||

||8.3.2 Level 2 |and 3 Models    300 |||

||8.3.3 BSIM Models |300 |||

||8.3.4 Diffusion |Capacitance Models |300 ||

||8.3.5 Design Corners |302 |||

|8.4 |Device |Characterization  . . . . . . . . . . . . . |. . . |. . . . . . . . . . . . . . . . . . . . . . . . . 303 |

||8.4.1 I-V Characteristics |303 |||

||8.4.2 Threshold |Voltage    306 |||

||8.4.3 Gate Capacitance |308 |||

||8.4.4 Parasitic |Capacitance    308 |||

||8.4.5 Effective |Resistance    310 |||

||8.4.6 |Comparison of Processes    311 |||

||8.4.7 Process and |Environmental |Sensitivity |313 |

|8.5 |Circuit |Characterization  . . . . . . . . . . . . . |. . . . |. . . . . . . . . . . . . . . . . . . . . . . . 313 |

||8.5.1 Path Simulations |313 |||

||8.5.2 DC Transfer |Characteristics    315 |||

||8.5.3 Logical |Effort    315 |||

||8.5.4 Power and |Energy    318 |||

||8.5.5 |Simulating Mismatches    319 |||

||8.5.6 Monte |Carlo Simulation    319 |||

|8.6 |Interconnect Simulation |. . . . . . . . . . . . . |. . . . |. . . . . . . . . . . . . . . . . . . . . . . . 319 |

8.7 Pitfalls and Fallacies . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 322 Summary  324


Exercises 324


Chapter 9  Combinational Circuit Design


9.1 Introduction  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 327


9.2 Circuit Families . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 328


9.2.1 Static CMOS    329


9.2.2 Ratioed Circuits    334


9.2.3 Cascode Voltage Switch Logic    339


9.2.4 Dynamic Circuits    339


9.2.5 Pass-Transistor Circuits    349


9.3 Circuit Pitfalls  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 354


9.3.1 Threshold Drops   355


9.3.2 Ratio Failures    355


9.3.3 Leakage    356


9.3.4 Charge Sharing    356


9.3.5 Power Supply Noise    356


9.3.6 Hot Spots    357


xiv


9.3.7 Minority Carrier Injection    357


9.3.8 Back-Gate Coupling    358


9.3.9 Diffusion Input Noise Sensitivity    358


9.3.10 Process Sensitivity    358


9.3.11 Example: Domino Noise Budgets    359


9.4 More Circuit Families . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 360


9.5 Silicon-On-Insulator Circuit Design  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 360


9.5.1 Floating Body Voltage    361


9.5.2 SOI Advantages    362


9.5.3 SOI Disadvantages    362


9.5.4 Implications for Circuit Styles    363


9.5.5 Summary    364


9.6 Subthreshold Circuit Design  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 364... . . . . .


9.6.1 Sizing    365


9.6.2 Gate Selection    365


9.7 Pitfalls and Fallacies  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 366


9.8 Historical Perspective . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 367


Summary   369


Exercises   370


Chapter 10  Sequential Circuit Design


10.1 Introduction  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 375


10.2 Sequencing Static Circuits . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 376


10.2.1 Sequencing Methods    376


10.2.2 Max-Delay Constraints    379


10.2.3 Min-Delay Constraints    383


10.2.4 Time Borrowing    386


10.2.5 Clock Skew    389


10.3 Circuit Design of Latches and Flip-Flops . . . . . . . . . . . . . . . . . . . . . . . . . . . 391


10.3.1 Conventional CMOS Latches    392


10.3.2 Conventional CMOS Flip-Flops    393


10.3.3 Pulsed Latches    395


10.3.4 Resettable Latches and Flip-Flops    396


10.3.5 Enabled Latches and Flip-Flops    397


10.3.6 Incorporating Logic into Latches    398


10.3.7 Klass Semidynamic Flip-Flop (SDFF)    399


10.3.8 Differential Flip-Flops    399


10.3.9 Dual Edge-Triggered Flip-Flops    400


10.3.10 Radiation-Hardened Flip-Flops    401


10.3.11 True Single-Phase-Clock (TSPC) Latches and Flip-Flops    402


10.4 Static Sequencing Element Methodology . . . . . . . . . . . . . . . . . . . . . . . . . . . 402


10.4.1 Choice of Elements    403


10.4.2 Characterizing Sequencing Element Delays    405


WEB


ENHANCED


Contents xv


TABLE 1.4  NOR gate truth table


|A |B |Y |
|---|---|---|

|0 |0 |1 |

|0 |1 |0 |

|1 |0 |0 |

|1 |1 |0 |

↓


FIGURE 1.16  2-input NOR  gate schematic (a) and symbol


(b) Y = A + B


FIGURE 1.17  3-input NOR  gate schematic Y = A + B + C


A B


Y


(a)


9 9


(b)


C


Chapter 1      Introduction


12


This AOI22 gate can be used as a 2-input inverting multiplexer by connecting C = A as a select signal. Then, Y = B if C is 0, while Y = D if C is 1. Section 1.4.8 shows a way to improve this multiplexer design.


Example 1.2


Sketch a static CMOS gate computing Y = (A + B + C) · D.


SOLUTION: Figure 1.19 shows such an OR-AND-INVERT-3-1 (OAI31) gate. The nMOS pull-down network pulls the output low if D is 1 and either A or B or C are 1,so D is in series with the parallel combination of A, B, and C. The pMOS pull-up net-


马


work is the conduction complement, so D must be in parallel with the series combination of A, B, and C.


1.4.6 Pass Transistors and Transmission Gates


The strength of a signal is measured by how closely it approximates an ideal voltage source.


In general, the stronger a signal, the more current it can source or sink. The power supplies, or rails, (VDD and GND) are the source of the strongest 1s and 0s.


An nMOS transistor is an almost perfect switch when passing a 0 and thus we say it passes a strong 0. However, the nMOS transistor is imperfect at passing a 1. The high voltage level is somewhat less than VDD, as will be explained in Section 2.5.4. We say it passes a degraded or weak 1. A pMOS transistor again has the opposite behavior, passing strong 1s but degraded 0s. The transistor symbols and behaviors are summarized in Figure


1.20 with g, s, and d indicating gate, source, and drain.


When an nMOS or pMOS is used alone as an imperfect switch, we sometimes call it a pass transistor. By combining an nMOS and a pMOS transistor in parallel (Figure


1.21(a)), we obtain a switch that turns on when a 1 is applied to g (Figure 1.21(b)) in which 0s and 1s are both passed in an acceptable fashion (Figure 1.21(c)). We term this a transmission gate or pass gate. In a circuit where only a 0 or a 1 has to be passed, the appropriate transistor (n or p) can be deleted, reverting to a single nMOS or pMOS device.


FIGURE 1.18  CMOS compound gate for function Y = (A · B) + (C · D)


C D


A


B C


D


B


A C


B D


(c)


(e)


(d)


(f)


C D B D


C-d


FIGURE 1.19


CMOS compound gate  for function


Y = (A + B + C) · D


BY


C D D


C B A


1.4      CMOS Logic 13


|||g g = 0 ||Input |Output g = 1 |
|---|---|---|---|---|---|

|nMOS |s |d s |d ||0 strong 0 |

|||g = 1 |||g = 1 |

|||s |d |1 |degraded 1 |

||(a)|(a) (b) ||(c) ||

|||g g = 0 ||Input |Output g = 0 |

|pMOS ||s d s |d ||0 degraded 0 |

|||g = 1 |||g = 0 |

|||s |d |1 |strong 1 |

|(d)|(d)|(d) (e) ||(f) ||

|FIGURE 1.20  Pass transistor strong and |FIGURE 1.20  Pass transistor strong and |FIGURE 1.20  Pass transistor strong and |degraded |outputs ||

Note that both the control input and its complement are required by the transmission gate. This is called double rail logic. Some circuit symbols for the transmission gate are shown in Figure 1.21(d).1 None are easier to draw than the simple schematic, so we will use the schematic version to represent a transmission gate in this book.


In all of our examples so far, the inputs drive the gate terminals of nMOS transistors in the pull-down network and pMOS transistors in the complementary pull-up network,as was shown in Figure 1.14. Thus, the nMOS transistors only need to pass 0s and the pMOS only pass 1s, so the output is always strongly driven and the levels are never degraded. This is called a fully restored logic gate and simpliﬁes circuit design considerably.


In contrast to other forms of logic, where the pull-up and pull-down switch networks have to be ratioed in some manner, static CMOS gates operate correctly independently of the physical sizes of the transistors. Moreover, there is never a path through ‘ON’ transistors from the 1 to the 0 supplies for any combination of inputs (in contrast to single-channel MOS, GaAs technologies, or bipolar). As we will ﬁnd in subsequent chapters, this is the basis for the low static power dissipation in CMOS.


10.4.3 State Retention Registers    408


10.4.4 Level-Converter Flip-Flops   408


10.4.5 Design Margin and Adaptive Sequential Elements    409


10.4.6 Two-Phase Timing Types   411


10.5 Sequencing Dynamic Circuits  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 411. .. . .


10.6 Synchronizers  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 411. . . . . . . . . . .. ..


10.6.1 Metastability   412


10.6.2 A Simple Synchronizer   415


10.6.3 Communicating Between Asynchronous Clock Domains   416


10.6.4 Common Synchronizer Mistakes   417


10.6.5 Arbiters   419


10.6.6 Degrees of Synchrony   419


10.7 Wave Pipelining . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 420


10.8 Pitfalls and Fallacies  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 422


10.9 Case Study: Pentium 4 and Itanium 2 Sequencing Methodologies  . . . . . 423


Summary  423


Exercises  425


Chapter 11  Datapath Subsystems


11.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 429


11.2 Addition/Subtraction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 429


11.2.1 Single-Bit Addition    430


11.2.2 Carry-Propagate Addition    434


11.2.3 Subtraction    458


11.2.4 Multiple-Input Addition    458


11.2.5 Flagged Preﬁx Adders    459


11.3 One/Zero Detectors  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 461


11.4 Comparators . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 462


11.4.1 Magnitude Comparator    462


11.4.2 Equality Comparator    462


11.4.3 K = A + B Comparator    463


11.5 Counters . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 463


11.5.1 Binary Counters    464


11.5.2 Fast Binary Counters    465


11.5.3 Ring and Johnson Counters    466


11.5.4 Linear-Feedback Shift Registers    466


11.6 Boolean Logical Operations . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 468


11.7 Coding  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 468


11.7.1 Parity    468


11.7.2 Error-Correcting Codes    468


11.7.3 Gray Codes    470


11.7.4 XOR/XNOR Circuit Forms    471


xvi


11.8 Shifters . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 472


11.8.1 Funnel Shifter    473


11.8.2 Barrel Shifter    475


11.8.3 Alternative Shift Functions    476


11.9 Multiplication  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 476


11.9.1 Unsigned Array Multiplication    478


11.9.2 Two’s Complement Array Multiplication    479


11.9.3 Booth Encoding    480


11.9.4 Column Addition    485


11.9.5 Final Addition    489


11.9.6 Fused Multiply-Add    490


11.9.7 Serial Multiplication    490


11.9.8 Summary    490


11.10 Parallel-Preﬁx Computations . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 491


11.11 Pitfalls and Fallacies  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 493 Summary 494


Exercises 494


|Chapter |12  Array |Subsystems ||
|---|---|---|---|

|12.1 |Introduction . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . 497 |

|12.2 |SRAM . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . 498 |

|12.2.1 |SRAM |Cells    499 ||

|12.2.2 |Row |Circuitry    506 ||

|12.2.3 |Column |Circuitry    510 ||

|12.2.4 |Multi-Ported |SRAM and Register Files    514 ||

|12.2.5 |Large |SRAMs    515 ||

|12.2.6 |Low-Power |SRAMs    517 ||

|12.2.7 |Area, |Delay, and Power of RAMs and Register Files |520 |

|12.3 |DRAM . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . 522 |

|12.3.1 |Subarray |Architectures    523 ||

|12.3.2 |Column Circuitry |525 ||

|12.3.3 |Embedded |DRAM    526 ||

|12.4 |Read-Only Memory |. . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . 527 |

|12.4.1 |Programmable |ROMs    529 ||

|12.4.2 |NAND |ROMs    530 ||

|12.4.3 |Flash    531 |||

|12.5 Serial |Access |Memories . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . 533 |

|12.5.1 |Shift |Registers    533 ||

|12.5.2 |Queues (FIFO, |LIFO)    533 ||

|12.6 |Content-Addressable |Memory  . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . 535 |

|12.7 |Programmable Logic |Arrays . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . 537 |

Contents xvii


12.8 Robust Memory Design . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 541


12.8.1 Redundancy    541


12.8.2 Error Correcting Codes (ECC)    543


12.8.3 Radiation Hardening    543


12.9 Historical Perspective . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 544 Summary  545


Exercises   546


|Chapter 13  Special-Purpose Subsystems |Chapter 13  Special-Purpose Subsystems |Chapter 13  Special-Purpose Subsystems |Chapter 13  Special-Purpose Subsystems |Chapter 13  Special-Purpose Subsystems |
|---|---|---|---|---|

|13.1 |Introduction . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . 549 |

|13.2 |Packaging and Cooling . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . 549 |

||13.2.1 Package Options |549 |549 ||

||13.2.2 Chip-to-Package |Connections |551 ||

||13.2.3 Package Parasitics |552 |||

||13.2.4 Heat Dissipation |552 |||

||13.2.5 Temperature Sensors |553 |||

|13.3 |Power Distribution . . . . . . . . |. . . . . . |. . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . 555 |

||13.3.1 On-Chip Power |Distribution |Network    556 ||

||13.3.2 IR Drops    557 ||||

||13.3.3 L di/dt Noise    558 ||||

||13.3.4 On-Chip Bypass |Capacitance |559 ||

||13.3.5 Power Network |Modeling |560 ||

||13.3.6 Power Supply |Filtering    564 |||

||13.3.7 Charge Pumps    564 ||||

||13.3.8 Substrate Noise   565 ||||

||13.3.9 Energy Scavenging |565 |||

|13.4 |Clocks . . . . . . . . . . . . . . . . . . |. . . . . . |. . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . 566 |

||13.4.1 Deﬁnitions    566 ||||

||13.4.2 Clock System |Architecture |568 ||

||13.4.3 Global Clock |Generation |569 ||

||13.4.4 Global Clock |Distribution |571 ||

||13.4.5 Local Clock Gaters |575 |||

||13.4.6 Clock Skew Budgets |577 |||

||13.4.7 Adaptive Deskewing |579 |||

|13.5 |PLLs and DLLs  . . . . . . . . . . |. . . . . . |. . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . 580 |

||13.5.1 PLLs    580 ||||

||13.5.2 DLLs   587 ||||

||13.5.3 Pitfalls   589 ||||

|13.6 |I/0 . . . . . . . . . . . . . . . . . . . . . |. . . . . . |. . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . 590 |

||13.6.1 Basic I/O Pad |Circuits    591 |||

||13.6.2 Electrostatic Discharge |Protection |593 ||

||13.6.3 Example: MOSIS I/O |Pads |594 ||

||13.6.4 Mixed-Voltage I/O |596 |||

xviii


13.7 High-Speed Links . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 597


13.7.1 High-Speed I/O Channels    597


13.7.2 Channel Noise and Interference   600


13.7.3 High-Speed Transmitters and Receivers   601


13.7.4 Synchronous Data Transmission   606


13.7.5 Clock Recovery in Source-Synchronous Systems   606


13.7.6 Clock Recovery in Mesochronous Systems   608


13.7.7 Clock Recovery in Pleisochronous Systems   610


13.8 Random Circuits . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 610.... .


13.8.1 True Random Number Generators    610


13.8.2 Chip Identiﬁcation   611


13.9 Pitfalls and Fallacies  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 612 Summary  613


Exercises   614


|Chapter 14  Design Methodology and Tools |Chapter 14  Design Methodology and Tools |Chapter 14  Design Methodology and Tools |Chapter 14  Design Methodology and Tools |
|---|---|---|---|

|14.1 |Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . |. . . 615 |

|14.2 |Structured Design Strategies . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . |. . . 617 |

||14.2.1 A Software Radio—A System Example    618 |||

||14.2.2 Hierarchy   620 |||

||14.2.3 Regularity   623 |||

||14.2.4 Modularity   625 |||

||14.2.5 Locality   626 |||

||14.2.6 Summary   627 |||

|14.3 |Design Methods  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . |. . . 627 |

||14.3.1 Microprocessor/DSP    627 |||

||14.3.2 Programmable Logic    628 |||

||14.3.3 Gate Array and Sea of Gates Design    631 |||

||14.3.4 Cell-Based Design    632 |||

||14.3.5 Full Custom Design    634 |||

||14.3.6 Platform-Based Design—System on a Chip    635 |||

||14.3.7 Summary   636 |||

|14.4 |Design Flows  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . |. . . 636 |

||14.4.1 Behavioral Synthesis Design Flow (ASIC Design |Flow)    637 ||

||14.4.2 Automated Layout Generation    641 |||

||14.4.3 Mixed-Signal or Custom-Design Flow    645 |||

|14.5 |Design Economics . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . |. . . 646 |

||14.5.1 Non-Recurring Engineering Costs (NREs)    647 |||

||14.5.2 Recurring Costs    649 |||

||14.5.3 Fixed Costs    650 |||

||14.5.4 Schedule    651 |||

||14.5.5 Personpower    653 |||

||14.5.6 Project Management    653 |||

||14.5.7 Design Reuse    654 |||

Contents xix


14.6 Data Sheets and Documentation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 655


14.6.1 The Summary    655


14.6.2 Pinout    655


14.6.3 Description of Operation    655


14.6.4 DC Speciﬁcations    655


14.6.5 AC Speciﬁcations    656


14.6.6 Package Diagram    656


14.6.7 Principles of Operation Manual    656


14.6.8 User Manual    656


14.7 CMOS Physical Design Styles  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 656


14.8 Pitfalls and Fallacies  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 657.. . . .


Exercises   657


|Chapter 15  Testing, Debugging, and Veriﬁcation |Chapter 15  Testing, Debugging, and Veriﬁcation |Chapter 15  Testing, Debugging, and Veriﬁcation |
|---|---|---|

|15.1 |Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . 659 |

||15.1.1 Logic Veriﬁcation    660 ||

||15.1.2 Debugging    662 ||

||15.1.3 Manufacturing Tests    664 ||

|15.2 |Testers, Test Fixtures, and Test Programs  . . . . . . |. . . . . . . . . . . . . . . . . . . . 666 |

||15.2.1 Testers and Test Fixtures    666 ||

||15.2.2 Test Programs    668 ||

||15.2.3 Handlers    669 ||

|15.3 |Logic Veriﬁcation Principles . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . 670 |

||15.3.1 Test Vectors    670 ||

||15.3.2 Testbenches and Harnesses    671 ||

||15.3.3 Regression Testing    671 ||

||15.3.4 Version Control    672 ||

||15.3.5 Bug Tracking    673 ||

|15.4 |Silicon Debug Principles  . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . 673 |

|15.5 |Manufacturing Test Principles . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . 676 |

||15.5.1 Fault Models    677 ||

||15.5.2 Observability    679 ||

||15.5.3 Controllability    679 ||

||15.5.4 Repeatability    679 ||

||15.5.5 Survivability    679 ||

||15.5.6 Fault Coverage    680 ||

||15.5.7 Automatic Test Pattern Generation (ATPG) |680 |

||15.5.8 Delay Fault Testing    680 ||

|15.6 |Design for Testability  . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . . . . . . . . . . . . . 681 |

||15.6.1 Ad Hoc Testing    681 ||

||15.6.2 Scan Design    682 ||

||15.6.3 Built-In Self-Test (BIST)    684 ||

||15.6.4 IDDQ Testing    687 ||

||15.6.5 Design for Manufacturability    687 ||

xx


15.7 Boundary Scan  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 688... ..


15.8 Testing in a University Environment . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 689


15.9 Pitfalls and Fallacies  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 690 Summary  697


Exercises   697


|Appendix A  Hardware Description Languages |Appendix A  Hardware Description Languages |Appendix A  Hardware Description Languages |
|---|---|---|

|A.1 |Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . A.1.1 Modules    700 |. . . . . . . . 699 |

||A.1.2 Simulation and Synthesis    701 ||

|A.2 |Combinational Logic . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . 702 |

||A.2.1 Bitwise Operators    702 ||

||A.2.2 Comments and White Space    703 ||

||A.2.3 Reduction Operators    703 ||

||A.2.4 Conditional Assignment   704 ||

||A.2.5 Internal Variables   706 ||

||A.2.6 Precedence and Other Operators   708 ||

||A.2.7 Numbers   708 ||

||A.2.8 Zs and Xs   709 ||

||A.2.9 Bit Swizzling   711 ||

||A.2.10 Delays   712 ||

|A.3 |Structural Modeling  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . 713 |

|A.4 |Sequential Logic . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . 717 |

||A.4.1 Registers    717 ||

||A.4.2 Resettable Registers    718 ||

||A.4.3 Enabled Registers    719 ||

||A.4.4 Multiple Registers    720 ||

||A.4.5 Latches    721 ||

||A.4.6 Counters    722 ||

||A.4.7 Shift Registers    724 ||

|A.5 |Combinational Logic with Always / Process Statements  . . . . . . |. . . . . . . . 724 |

||A.5.1 Case Statements    726 ||

||A.5.2 If Statements    729 ||

||A.5.3 SystemVerilog Casez    731 ||

||A.5.4 Blocking and Nonblocking Assignments    731 ||

|A.6 |Finite State Machines  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . 735 |

||A.6.1 FSM Example    735 ||

||A.6.2 State Enumeration    736 ||

||A.6.3 FSM with Inputs    738 ||

|A.7 |Type Idiosyncracies . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . |. . . . . . . . 740 |

Contents xxi


A.8 Parameterized Modules  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 742 A.9 Memory . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 745 A.9.1 RAM    745


A.9.2 Multiported Register Files    747


A.9.3 ROM    748


A.10 Testbenches . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 749 A.11 SystemVerilog Netlists  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 754 A.12 Example: MIPS Processor  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 755 A.12.1 Testbench    756


A.12.2 SystemVerilog    757


A.12.3 VHDL    766


Exercises   776


References   785


Index   817


Credits   838


xxiii


In the two-and-a-half decades since the ﬁrst edition of this book was published, CMOS technology has claimed the preeminent position in modern electrical system design. It has enabled the widespread use of wireless communication, the Internet, and personal computers. No other human invention has seen such rapid growth for such a sustained period.


The transistor counts and clock frequencies of state-of-the-art chips have grown by orders of magnitude.


||1st Edition |2nd Edition |3rd Edition |4th Edition |
|---|---|---|---|---|

|Year |1985 |1993 |2004 |2010 |

|Transistor Counts |105–106 |106–107 |108–109 |109–1010 |

|Clock Frequencies |107 |108 |109 |109 |

|Worldwide Market |$25B |$60B |$170B |$250B |

This edition has been heavily revised to reﬂect the rapid changes in integrated circuit design over the past six years. While the basic principles are largely the same, power consumption and variability have become primary factors for chip design. The book has been reorganized to emphasize the key factors: delay, power, interconnect, and robustness.


Other chapters have been reordered to reﬂect the order in which we teach the material.


How to Use This Book


This book intentionally covers more breadth and depth than any course would cover in a


semester. It is accessible for a ﬁrst undergraduate course in VLSI, yet detailed enough for


advanced graduate courses and is useful as a reference to the practicing engineer. You are


encouraged to pick and choose topics according to your interest. Chapter 1 previews the


entire ﬁeld, while subsequent chapters elaborate on speciﬁc topics. Sections are marked


with the “Optional” icon (shown here in the margin) if they are not needed to understandOPTIONAL subsequent sections. You may skip them on a ﬁrst reading and return when they are relevant to you.


We have endeavored to include ﬁgures whenever possible (“a picture is worth a thousand words”) to trigger your thinking. As you encounter examples throughout the text, we


urge you to think about them before reading the solutions. We have also provided extensive references for those who need to delve deeper into topics introduced in this text. We


Preface


xxiv


have emphasized the best practices that are used in industry and warned of pitfalls and fallacies. Our judgments about the merits of circuits may become incorrect as technology and applications change, but we believe it is the responsibility of a writer to attempt to call out the most relevant information.


Supplements


Numerous supplements are available on the Companion Web site for the book,www.cmosvlsi.com. Supplements to help students with the course include:


A lab manual with laboratory exercises involving the design of an 8-bit micropro-A lab manual with laboratory exercises involving the design of an 8-bit microprocessor covered in Chapter 1.


A collection of links to VLSI resources including open-source CAD tools and pro-A collection of links to VLSI resources including open-source CAD tools and process parameters.


A student solutions manual that includes answers to odd-numbered problems.


Certain sections of the book moved online to shorten the page count. These sec-Certain sections of the book moved online to shorten the page count. These sections are indicated by the “Web Enhanced” icon (shown here in the margin).


Supplements to help instructors with the course include:


A sample syllabus.A sample syllabus.


© Lecture slides for an introductory VLSI course.Lecture slides for an introductory VLSI course.


●An instructor’s manual with solutions.


These materials have been prepared exclusively for professors using the book in a course. Please send email to computing@aw.com for information on how to access them.


Acknowledgments


We are indebted to many people for their reviews, suggestions, and technical discussions.


These people include: Bharadwaj “Birdy” Amrutur, Mark Anders, Adnan Aziz, Jacob Baker, Kaustav Banerjee, Steve Bibyk, David Blaauw, Erik Brunvand, Neil Burgess,Wayne Burleson, Robert Drost, Jo Ebergen, Sarah Harris, Jacob Herbold, Ron Ho, David Hopkins, Mark Horowitz, Steven Hsu, Tanay Karnik, Omid Kaveh, Matthew Keeter,Ben Keller, Ali Keshavarzi, Brucek Khailany, Jaeha Kim, Volkan Kursun, Simon Knowles,Ram Krishnamurthy, Austin Lee, Ana Sonia Leon, Shih-Lien Lu, Sanu Mathew, Aleksandar Milenkovic, Sam Naffziger, Braden Phillips, Stefan Rusu, Justin Schauer, James Stine, Jason Stinson, Aaron Stratton, Ivan Sutherland, Jim Tschanz, Alice Wang, GuYeon Wei, and Peiyi Zhao. We apologize in advance to anyone we overlooked.


MOSIS and IBM kindly provided permission to use nanometer SPICE models for many examples. Nathaniel Pinckney spent a summer revising the laboratory exercises and updating simulations. Jaeha Kim contributed new sections on phase-locked loops and high-speed I/O for Chapter 13. David would like to thank Bharadwaj Amrutur of the Indian Institute of Science and Braden Phillips of the University of Adelaide for hosting him during two productive summers of writing.


Contents xxv


Addison-Wesley has done an admirable job with the grueling editorial and production process. We would particularly like to thank our editor, Matt Goldstein, and our compositor, Gillian Hall.


Sally Harris has been editing family books since David was an infant on her lap. She read the page proofs with amazing attention to detail and unearthed hundreds of errors. This book would not have existed without the support of our families. David would particularly like to thank his wife Jennifer and sons Abraham and Samuel for enduring two summers of absence while writing, and to our extended family for their tremendous assistance.


We have become painfully aware of the ease with which mistakes creep into a book.


Scores of 3rd edition readers have reported bugs that are now corrected. Despite our best efforts at validation, we are conﬁdent that we have introduced a similar number of new errors. Please check the errata sheet at www.cmosvlsi.com/errata.pdf to see if the bug has already been reported. Send your reports to bugs@cmosvlsi.com.


January 2010


1


Introduction


1.1 A Brief History


In 1958, Jack Kilby built the ﬁrst integrated circuit ﬂip-ﬂop with two transistors at Texas Instruments. In 2008, Intel’s Itanium microprocessor contained more than 2 billion transistors and a 16 Gb Flash memory contained more than 4 billion transistors. This corresponds to a compound annual growth rate of 53% over 50 years. No other technology in history has sustained such a high growth rate lasting for so long.


This incredible growth has come from steady miniaturization of transistors and improvements in manufacturing processes. Most other ﬁelds of engineering involve tradeoffs between performance, power, and price. However, as transistors become smaller, they also become faster, dissipate less power, and are cheaper to manufacture. This synergy has not only revolutionized electronics, but also society at large.


The processing performance once dedicated to secret government supercomputers is now available in disposable cellular telephones. The memory once needed for an entire company’s accounting system is now carried by a teenager in her iPod. Improvements in integrated circuits have enabled space exploration, made automobiles safer and more fuelefﬁcient, revolutionized the nature of warfare, brought much of mankind’s knowledge to our Web browsers, and made the world a ﬂatter place.


Figure 1.1 shows annual sales in the worldwide semiconductor market. Integrated circuits became a $100 billion/year business in 1994. In 2007, the industry manufactured approximately 6 quintillion (6 × 1018) transistors, or nearly a billion for every human being on the planet. Thousands of engineers have made their fortunes in the ﬁeld. New fortunes lie ahead for those with innovative ideas and the talent to bring those ideas to reality.


During the ﬁrst half of the twentieth century, electronic circuits used large, expensive,power-hungry, and unreliable vacuum tubes. In 1947, John Bardeen and Walter Brattain built the ﬁrst functioning point contact transistor at Bell Laboratories, shown in Figure


1.2(a) [Riordan97]. It was nearly classiﬁed as a military secret, but Bell Labs publicly introduced the device the following year.


We have called it the Transistor, T-R-A-N-S-I-S-T-O-R, because it is a resistor or  semiconductor device which can amplify electrical signals as they are transferred


through it from input to output terminals. It is, if you will, the electrical equivalent  of a vacuum tube ampliﬁer. But there the similarity ceases. It has no vacuum, no   ﬁlament, no glass tube. It is composed entirely of cold, solid substances.


2


Ten years later, Jack Kilby at Texas Instruments realized the potential for miniaturization if multiple transistors could be built on one piece of silicon. Figure 1.2(b) shows hisﬁrst prototype of an integrated circuit, constructed from a germanium slice and gold wires. The invention of the transistor earned the Nobel Prize in Physics in 1956 for Bardeen, Brattain, and their supervisor William Shockley. Kilby received the Nobel Prize in Physics in 2000 for the invention of the integrated circuit.


Transistors can be viewed as electrically controlled switches with a control terminal and two other terminals that are connected or disconnected depending on the voltage or current applied to the control. Soon after inventing the point contact transistor, Bell Labs developed the bipolar junction transistor. Bipolar transistors were more reliable, less noisy,and more power-efﬁcient. Early integrated circuits primarily used bipolar transistors.


Bipolar transistors require a small current into the control (base) terminal to switch much larger currents between the other two (emitter and collector) terminals. The quiescent power dissipated by these base currents, drawn even when the circuit is not switching,


FIGURE 1.1  Size of worldwide semiconductor market (Courtesy of Semiconductor Industry Association.)


FIGURE 1.2  (a) First transistor (Property of AT&T Archives. Reprinted with permission of AT&T.) and (b) ﬁrst integrated circuit (Courtesy of Texas Instruments.)


0 50


ingsGlobal Semiconductor Bill


100


(Billions of US$)150


200


1982 1984 1986 1988 1990 1992 1994 1996 1998 2000 2002 Year


2004 2006 2008


250


)b(


)a(


1.1      A Brief History 3


limits the maximum number of transistors that can be integrated onto a single die. By the 1960s, Metal Oxide Semiconductor Field Effect Transistors (MOSFETs) began to enter production. MOSFETs offer the compelling advantage that they draw almost zero control current while idle. They come in two ﬂavors: nMOS and pMOS, using n-type and p-type silicon, respectively. The original idea of ﬁeld effect transistors dated back to the German scientist Julius Lilienﬁeld in 1925 [US patent 1,745,175] and a structure closely resembling the MOSFET was proposed in 1935 by Oskar Heil [British patent 439,457], but materials problems foiled early attempts to make functioning devices.


In 1963, Frank Wanlass at Fairchild described the ﬁrst logic gates using MOSFETs[Wanlass63]. Fairchild’s gates used both nMOS and pMOS transistors, earning the name Complementary Metal Oxide Semiconductor, or CMOS. The circuits used discrete transistors but consumed only nanowatts of power, six orders of magnitude less than their bipolar counterparts. With the development of the silicon planar process, MOS integrated circuits became attractive for their low cost because each transistor occupied less area and the fabrication process was simpler [Vadasz69]. Early commercial processes used only pMOS transistors and suffered from poor performance, yield, and reliability. Processes using nMOS transistors became common in the 1970s [Mead80]. Intel pioneered nMOS technology with its 1101 256-bit static random access memory and 4004 4-bit microprocessor, as shown in Figure 1.3. While the nMOS process was less expensive than CMOS,nMOS logic gates still consumed power while idle. Power consumption became a major issue in the 1980s as hundreds of thousands of transistors were integrated onto a single die. CMOS processes were widely adopted and have essentially replaced nMOS and bipolar processes for nearly all digital logic applications.


In 1965, Gordon Moore observed that plotting the number of transistors that can be most economically manufactured on a chip gives a straight line on a semilogarithmic scale[Moore65]. At the time, he found transistor count doubling every 18 months. This observation has been called Moore’s Law and has become a self-fulﬁlling prophecy. Figure 1.4 shows that the number of transistors in Intel microprocessors has doubled every 26 months since the invention of the 4004. Moore’s Law is driven primarily by scaling down the size of transistors and, to a minor extent, by building larger chips. The level of integration of chips has been classiﬁed as small-scale, medium-scale, large-scale, and very largescale. Small-scale integration (SSI) circuits, such as the 7404 inverter, have fewer than 10


FIGURE 1.3  (a) Intel 1101 SRAM (© IEEE 1969 [Vadasz69]) and (b) 4004 microprocessor (Reprinted with  permission of Intel Corporation.)


4004


4


gates, with roughly half a dozen transistors per gate. Medium-scale integration (MSI) circuits, such as the 74161 counter, have up to 1000 gates. Large-scale integration (LSI)circuits, such as simple 8-bit microprocessors, have up to 10,000 gates. It soon became apparent that new names would have to be created every ﬁve years if this naming trend continued and thus the term very large-scale integration (VLSI) is used to describe most integrated circuits from the 1980s onward. A corollary of Moore’s law is Dennard’s Scaling Law [Dennard74]: as transistors shrink, they become faster, consume less power, and are cheaper to manufacture. Figure 1.5 shows that Intel microprocessor clock frequencies have doubled roughly every 34 months.This frequency scaling hit the power wall around 2004,and clock frequencies have leveled off around 3 GHz. Computer performance, measured in time to run an application, has advanced even more than raw clock speed. Presently, the performance is driven by the number of cores on a chip rather than by the clock. Even though an individual CMOS transistor uses very little energy each time it switches, the enormous number of transistors switching at very high rates of speed have made power consumption a major design consideration again. Moreover, as transistors have become so small, they cease to turn completely OFF. Small amounts of current leaking through each transistor now lead to signiﬁcant power consumption when multiplied by millions or billions of transistors on a chip.


The feature size of a CMOS manufacturing process refers to the minimum dimension of a transistor that can be reliably built. The 4004 had a feature size of 10 m in 1971. The Core 2 Duo had a feature size of 45 nm in 2008. Manufacturers introduce a new process generation (also called a technology node) every 2–3 years with a 30% smaller feature size to pack twice as many transistors in the same area. Figure 1.6 shows the progression of process generations. Feature sizes down to 0.25 m are generally speciﬁed in microns (10–6 m), while smaller feature sizes are expressed in nanometers (10–9 m). Effects that were relatively minor in micron processes, such as transistor leakage, variations in characteristics of adjacent transistors, and wire resistance, are of great signiﬁcance in nanometer processes.


Moore’s Law has become a self-fulﬁlling prophecy because each company must keep up with its competitors. Obviously, this scaling cannot go on forever because transistors cannot be smaller than atoms. Dennard scaling has already begun to slow. By the 45 nm


FIGURE 1.4 Transistors in Intel microprocessors [Intel10]


Year


8008


8080


8086


80286


Intel386


Intel486


Pentium


Pentium Pro


Pentium II


Pentium III Pentium 4


1,000 10,000 100,000 Transistors1,000,000 10,000,000 100,000,000


1,000,000,000


1970


1975


1980


1985


1990


1995


2000


2005


Pentium M


Core 2 Duo


Core 2 Quad


1.1      A Brief History 5


FIGURE 1.5 Clock frequencies of Intel microprocessors


|10 |10 μm |10 μm |10 μm |10 μm |10 μm |10 μm |10 μm |10 μm |10 μm |10 μm |10 μm |
|---|---|---|---|---|---|---|---|---|---|---|---|

||6 μm |6 μm |6 μm |6 μm |6 μm |6 μm |6 μm |6 μm |6 μm |6 μm |6 μm |

||3 μm |●1.5 μm||||||||||

|1 ||1.5 μm |1 μm |0.8 μm ||||||||

|0.1 ||||0.6 μm |0.35 |μm 0.25 180 |μm nm 130 |nm ||||

|0||||||||90 nm |65 |nm 45 nm ||

|||||||||||32 |nm 22 nm |

FIGURE 1.6 Process generations. Future predictions from [SIA2007].


10


Clock Speed (MHz)100


1,000


10,000


月


Pentium Pro/II/III Pentium 4


2010


Pentium M Core 2 Duo


0


2015


Feature Size (um)


0.01


T


6


generation, designers are having to make trade-offs between improving power and improving delay. Although the cost of printing each transistor goes down, the one-time design costs are increasing exponentially, relegating state-of-the-art processes to chips that will sell in huge quantities or that have cutting-edge performance requirements. However,many predictions of fundamental limits to scaling have already proven wrong. Creative engineers and material scientists have billions of dollars to gain by getting ahead of their competitors. In the early 1990s, experts agreed that scaling would continue for at least a decade but that beyond that point the future was murky. In 2009, we still believe that Moore’s Law will continue for at least another decade. The future is yours to invent.


1.2 Preview


As the number of transistors on a chip has grown exponentially, designers have come to rely on increasing levels of automation to seek corresponding productivity gains. Many designers spend much of their effort specifying functions with hardware description languages and seldom look at actual transistors. Nevertheless, chip design is not software engineering. Addressing the harder problems requires a fundamental understanding of circuit and physical design. Therefore, this book focuses on building an understanding of integrated circuits from the bottom up.


In this chapter, we will take a simpliﬁed view of CMOS transistors as switches. With this model we will develop CMOS logic gates and latches. CMOS transistors are massproduced on silicon wafers using lithographic steps much like a printing press process. We will explore how to lay out transistors by specifying rectangles indicating where dopants should be diffused, polysilicon should be grown, metal wires should be deposited, and contacts should be etched to connect all the layers. By the middle of this chapter, you will understand all the principles required to design and lay out your own simple CMOS chip.


The chapter concludes with an extended example demonstrating the design of a simple 8-bit MIPS microprocessor chip. The processor raises many of the design issues that will be developed in more depth throughout the book. The best way to learn VLSI design is by doing it. A set of laboratory exercises are available at www.cmosvlsi.com to guide you through the design of your own microprocessor chip.


1.3 MOS Transistors


Silicon (Si), a semiconductor, forms the basic starting material for most integrated circuits[Tsividis99]. Pure silicon consists of a three-dimensional lattice of atoms. Silicon is a Group IV element, so it forms covalent bonds with four adjacent atoms, as shown in Figure 1.7(a). The lattice is shown in the plane for ease of drawing, but it actually forms a cubic crystal. As all of its valence electrons are involved in chemical bonds, pure silicon is a poor conductor. The conductivity can be raised by introducing small amounts of impurities, called dopants, into the silicon lattice. A dopant from Group V of the periodic table,such as arsenic, has ﬁve valence electrons. It replaces a silicon atom in the lattice and still bonds to four neighbors, so the ﬁfth valence electron is loosely bound to the arsenic atom,as shown in Figure 1.7(b). Thermal vibration of the lattice at room temperature is enough to set the electron free to move, leaving a positively charged As+ ion and a free electron.


The free electron can carry current so the conductivity is higher. We call this an n-type


1.3      MOS Transistors 7


semiconductor because the free carriers are negatively charged electrons. Similarly, a


Group III dopant, such as boron, has three valence electrons, as shown in Figure 1.7(c).


The dopant atom can borrow an electron from a neighboring silicon atom, which in turn


becomes short by one electron. That atom in turn can borrow an electron, and so forth, so


the missing electron, or hole, can propagate about the lattice. The hole acts as a positive


carrier so we call this a p-type semiconductor.


A junction between p-type and n-type silicon is called a diode, as shown in Figure 1.8.


 and n-type silicon is called a diode, as shown in Figure 1.8.


|p-type |n-type |
|---|---|

When the voltage on the p-type semiconductor, called the anode, is raised above the ntype cathode, the diode is forward biased and current ﬂows. When the anode voltage is less


than or equal to the cathode voltage, the diode is reverse biased and very little current ﬂows.


A Metal-Oxide-Semiconductor (MOS) structure is created by superimposing several


layers of conducting and insulating materials to form a sandwich-like structure. These-D structures are manufactured using a series of chemical processing steps involving oxidation


of the silicon, selective introduction of dopants, and deposition and etching of metal wires


and contacts. Transistors are built on nearly ﬂawless single crystals of silicon, which are


available as thin ﬂat circular wafers of 15–30 cm in diameter. CMOS technology provides


two types of transistors (also called devices): an n-type transistor (nMOS) and a p-type


transistor (pMOS). Transistor operation is controlled by electric ﬁelds so the devices are


also called Metal Oxide Semiconductor Field Effect Transistors (MOSFETs) or simply


FETs. Cross-sections and symbols of these transistors are shown in Figure 1.9. The n+


and p+ regions indicate heavily doped n- or p-type silicon.


FIGURE 1.7  Silicon lattice and dopant atoms


FIGURE 1.9  nMOS transistor (a) and pMOS transistor (b)


Si Si


Si


-


Si 一Si


As Si


-Si Si


B Si


一


一一-


一一


-一一 Si Si


+


一-一


n+


p Gate


Source


Drain


bulk Si


SiO2


n Gate


吉


Polysilicon


p+


FIGURE 1.8


p-n junction diode  structure and symbol


Anode Cathode


8


Each transistor consists of a stack of the conducting gate, an insulating layer of silicon dioxide (SiO2, better known as glass), and the silicon wafer, also called the substrate, body,or bulk. Gates of early transistors were built from metal, so the stack was called metaloxide-semiconductor, or MOS. Since the 1970s, the gate has been formed from polycrystalline silicon (polysilicon), but the name stuck. (Interestingly, metal gates reemerged in 2007 to solve materials problems in advanced manufacturing processes.) An nMOS transistor is built with a p-type body and has regions of n-type semiconductor adjacent to the gate called the source and drain. They are physically equivalent and for now we will regard them as interchangeable. The body is typically grounded. A pMOS transistor is just the opposite, consisting of p-type source and drain regions with an n-type body. In a CMOS technology with both ﬂavors of transistors, the substrate is either n-type or p-type. The other ﬂavor of transistor must be built in a special well in which dopant atoms have been added to form the body of the opposite type.


The gate is a control input: It affects the ﬂow of electrical current between the source and drain. Consider an nMOS transistor. The body is generally grounded so the p–n junctions of the source and drain to body are reverse-biased. If the gate is also grounded, no current ﬂows through the reverse-biased junctions. Hence, we say the transistor is OFF. If the gate voltage is raised, it creates an electric ﬁeld that starts to attract free electrons to the underside of the Si–SiO2 interface. If the voltage is raised enough, the electrons outnumber the holes and a thin region under the gate called the channel is inverted to act as an n-type semiconductor. Hence, a conducting path of electron carriers is formed from source to drain and current can ﬂow. We say the transistor is ON.


For a pMOS transistor, the situation is again reversed. The body is held at a positive voltage. When the gate is also at a positive voltage, the source and drain junctions are reverse-biased and no current ﬂows, so the transistor is OFF. When the gate voltage is lowered, positive charges are attracted to the underside of the Si–SiO2 interface. A sufﬁciently low gate voltage inverts the channel and a conducting path of positive carriers is formed from source to drain, so the transistor is ON. Notice that the symbol for the pMOS transistor has a bubble on the gate, indicating that the transistor behavior is the opposite of the nMOS. The positive voltage is usually called VDD or POWER and represents a logic 1 value in digital circuits. In popular logic families of the 1970s and 1980s, VDD was set to 5 volts.


Smaller, more recent transistors are unable to withstand such high voltages and have used supplies of 3.3 V, 2.5 V, 1.8 V, 1.5 V, 1.2 V, 1.0 V, and so forth. The low voltage is called GROUND (GND) or VSS and represents a logic 0. It is normally 0 volts.


||g = 0 ||g = 1 |
|---|---|---|---|

||d d ||d |

|nMOS |g |OFF |ON |

||。 50||D|

||s s ||s |

|pMOS |g |ON |OFF |

||0|||

|FIGURE |1.10  Transistor symbols and switch-level s s |models |s |

In summary, the gate of an MOS transistor controls the ﬂow of current between the source and drain. Simplifying this to the extreme allows the MOS transistors to be viewed as simple ON/OFF switches. When the gate of an nMOS transistor is 1, the transistor is ON and there is a conducting path from source to drain. When the gate is low, the nMOS transistor is OFF and almost zero current ﬂows from source to drain. A pMOS transistor is just the opposite, being ON when the gate is low and OFF when the gate is high. This switch model is illustrated in Figure 1.10, where g, s,and d indicate gate, source, and drain. This model will be our most common one when discussing circuit behavior.


1.4      CMOS Logic 9


1.4 CMOS Logic


1.4.1 The Inverter


Figure 1.11 shows the schematic and symbol for a CMOS inverter or NOT gate using one nMOS transistor and one pMOS transistor. The bar at the top indicates VDD and the triangle at the bottom indicates GND. When the input A is 0, the nMOS transistor is OFF and the pMOS transistor is ON. Thus, the output Y is pulled up to 1 because it is connected to VDD but not to GND. Conversely, when A is 1, the nMOS is ON, the pMOS is OFF, and Y is pulled down to ‘0.’ This is summarized in Table 1.1.


1.4.2 The NAND Gate


Figure 1.12(a) shows a 2-input CMOS NAND gate. It consists of two series nMOS transistors between Y and GND and two parallel pMOS transistors between Y and VDD. If either input A or B is 0, at least one of the nMOS transistors will be OFF, breaking the path from Y to GND. But at least one of the pMOS transistors will be ON, creating a path from Y to VDD. Hence, the output Y will be 1. If both inputs are 1, both of the nMOS transistors will be ON and both of the pMOS transistors will be OFF. Hence, the output will be 0. The truth table is given in Table 1.2 and the symbol is shown in Figure 1.12(b).


Note that by DeMorgan’s Law, the inversion bubble may be placed on either side of the


gate. In the ﬁgures in this book, two lines intersecting at a T-junction are connected. Two lines crossing are connected if and only if a dot is shown.


k-input NAND gates are constructed using k series nMOS transistors and k parallel pMOS transistors. For example, a 3-input NAND gate is shown in Figure 1.13. When any of the inputs are 0, the output is pulled high through the parallel pMOS transistors. When all of the inputs are 1, the output is pulled low through the series nMOS transistors.


1.4.3 CMOS Logic Gates


The inverter and NAND gates are examples of static CMOS logic gates, also called complementary CMOS gates. In general, a static CMOS gate has an nMOS pull-down network to connect the output to 0 (GND) and pMOS pull-up network to connect the output to 1(VDD), as shown in Figure 1.14. The networks are arranged such that one is ON and the other OFF for any input pattern.


TABLE 1.1  Inverter truth table


|A |Y |
|---|---|

|0 |1 |

|1 |0 |

TABLE 1.2  NAND gate truth table


|A |B |Pull-Down Network |Pull-Up Network |Y |
|---|---|---|---|---|

|0 |0 |OFF |ON |1 |

|0 |1 |OFF |ON |1 |

|1 |0 |OFF |ON |1 |

|1 |1 |ON |OFF |0 |

。


FIGURE 1.11


Inverter schematic


(a) and symbol


(b) Y = A


FIGURE 1.12 2-input NAND  gate schematic (a) and symbol


(b) Y = A · B


FIGURE 1.13  3-input NAND  gate schematic Y = A · B · C


VDD


GND


The pull-up and pull-down networks in the inverter each consist of a single transistor. The NAND gate uses a series pull-down network and a parallel pullup network. More elaborate networks are used for more complex gates. Two or more transistors in series are ON only if all of the series transistors are ON.


Two or more transistors in parallel are ON if any of the parallel transistors are ON. This is illustrated in Figure 1.15 for nMOS and pMOS transistor pairs.


By using combinations of these constructions, CMOS combinational gates can be constructed. Although such static CMOS gates are most widely used,Chapter 9 explores alternate ways of building gates with transistors.


In general, when we join a pull-up network to a pull-down network to form a logic gate as shown in Figure 1.14, they both will attempt to exert a logic level at the output. The possible levels at the output are shown in Table 1.3.


From this table it can be seen that the output of a CMOS logic gate can be in four states. The 1 and 0 levels have been encountered with the inverter and NAND gates, where either the pull-up or pull-down is OFF and the other structure is ON. When both pull-up and pull-down are OFF, the highimpedance or ﬂoating Z output state results. This is of importance in multiplexers, memory elements, and tristate bus drivers. The crowbarred (or contention) X level exists when both pull-up and pull-down are simultaneously turned ON. Contention between  the two networks results in an indeterminate output level and dissipates static power. It is usually an unwanted condition.


FIGURE 1.15  Connection and behavior of series and parallel transistors


a


b 00，


b


亨


OFF


g1 g2


宁0o or0


00


1亨


1言


ON


g1


g20


0文0


1鲁


F


daL


g2


0 罗


了9


1 00 1


o0o8


FIGURE 1.14  General logic gate using  pull-up and pull-down networks


Output


Inputs


pMOS pull-up network


nMOS pull-down network


1.4      CMOS Logic 11


1.4.4 The NOR Gate


A 2-input NOR gate is shown in Figure 1.16. The nMOS transistors are in parallel to pull the output low when either input is high. The pMOS transistors are in series to pull the output high when both inputs are low, as indicated in Table 1.4. The output is never crowbarred or left ﬂoating.


Example 1.1


Sketch a 3-input CMOS NOR gate.


SOLUTION: Figure 1.17 shows such a gate. If any input is high, the output is pulled low through the parallel nMOS transistors. If all inputs are low, the output is pulled high through the series pMOS transistors.


1.4.5 Compound Gates


A compound gate performing a more complex logic function in a single stage of logic is formed by using a combination of series and parallel switch structures. For example, the derivation of the circuit for the function Y = (A · B) + (C · D) is shown in Figure 1.18.


This function is sometimes called AND-OR-INVERT-22, or AOI22 because it performs the NOR of a pair of 2-input ANDs. For the nMOS pull-down network, take the uninverted expression ((A · B) + (C · D)) indicating when the output should be pulled to‘0.’ The AND expressions (A · B) and (C · D) may be implemented by series connections of switches, as shown in Figure 1.18(a). Now ORing the result requires the parallel connection of these two structures, which is shown in Figure 1.18(b). For the pMOS pull-up network, we must compute the complementary expression using switches that turn on with inverted polarity. By DeMorgan’s Law, this is equivalent to interchanging AND and OR operations. Hence, transistors that appear in series in the pull-down network must appear in parallel in the pull-up network. Transistors that appear in parallel in the pulldown network must appear in series in the pull-up network. This principle is called conduction complements and has already been used in the design of the NAND and NOR gates. In the pull-up network, the parallel combination of A and B is placed in series with the parallel combination of C and D. This progression is evident in Figure 1.18(c) and Figure 1.18(d). Putting the networks together yields the full schematic (Figure 1.18(e)).


The symbol is shown in Figure 1.18(f ).


TABLE 1.3  Output states of CMOS logic gates


||pull-up OFF |pull-up ON |
|---|---|---|

|pull-down OFF |Z |1 |

|pull-down ON |0 |crowbarred (X) |

his is the basis for the low static power dissipation in CMOS.


|||Input |Output |
|---|---|---|---|

||g = 0, gb = 1 ||g = 1, gb = 0 |

||a b ||0 strong 0 |

||g = 1, gb = 0 |g |= 1, gb = 0 |

||a b ||1 strong 1 |

|(a) |(b) |(c) ||

1We call the left and right terminals a and b because each is technically the source of one of the transistors and the drain of the other.


FIGURE 1.21  Transmission gate


g


gb


a 京b


a 8b


14


A consequence of the design of static CMOS gates is that they must be inverting.


The nMOS pull-down network turns ON when inputs are 1, leading to 0 at the output.


We might be tempted to turn the transistors upside down to build a noninverting gate. For example, Figure 1.22 shows a noninverting buffer. Unfortunately, now both the nMOS and pMOS transistors produce degraded outputs, so the technique should be avoided.


Instead, we can build noninverting functions from multiple stages of inverting gates. Figure 1.23 shows several ways to build a 4-input AND gate from two levels of inverting static CMOS gates. Each design has different speed, size, and power trade-offs.


Similarly, the compound gate of Figure 1.18 could be built with two AND gates, an OR gate, and an inverter. The AND and OR gates in turn could be constructed from NAND/NOR gates and inverters, as shown in Figure 1.24, using a total of 20 transistors,as compared to eight in Figure 1.18. Good CMOS logic designers exploit the efﬁciencies of compound gates rather than using large numbers of AND/OR gates.


FIGURE 1.22


Bad noninverting buffer


BAD


FIGURE 1.23  Various implementations  of a CMOS 4-input AND gate


FIGURE 1.24  Inefﬁcient discrete gate implementation of AOI22  with transistor counts indicated


2>0


AND


OR


B C D


FIGURE 1.25


Tristate buffer  symbol


EN


1.4.7 Tristates


Figure 1.25 shows symbols for a tristate buffer. When the enable input EN is 1, the output Y equals the input A, just as in an ordinary buffer. When the enable is 0, Y is left ﬂoating (a‘Z’ value). This is summarized in Table 1.5. Sometimes both true and complementary enable signals EN and EN are drawn explicitly, while sometimes only EN is shown.


了


The transmission gate in Figure 1.26 has the same truth table as a tristate buffer. It only requires two transistors but it is a nonrestoring circuit. If the input is noisy or otherwise degraded, the output will receive the same noise. We will see in Section 4.4.2 that the delay of a series of nonrestoring gates increases rapidly with the number of gates.


TABLE 1.5  Truth table for tristate


|EN / EN |A |Y |
|---|---|---|

|0 / 1 |0 |Z |

|0 / 1 |1 |Z |

|1 / 0 |0 |0 |

|1 / 0 |1 |1 |

FIGURE 1.26


Transmission gate


1.4      CMOS Logic 15


Figure 1.27(a) shows a tristate inverter. The output is actively driven from VDD or GND, so it is a restoring logic gate. Unlike any of the gates considered so far, the tristate inverter does not obey the conduction complements rule because it allows the output to ﬂoat under certain input combinations. When EN is 0 (Figure 1.27(b)), both enable transistors are OFF, leaving the output ﬂoating. When EN is 1


文


个


子


(Figure 1.27(c)), both enable transistors are ON. They are


conceptually removed from the circuit, leaving a simple


inverter. Figure 1.27(d) shows symbols for the tristate


inverter. The complementary enable signal can be generated


internally or can be routed to the cell explicitly. A tristate


buffer can be built as an ordinary inverter followed by a


tristate inverter.


Tristates were once commonly used to allow multiple units to drive a common bus, as long as exactly one unit is enabled at a time. If multiple units drive the bus, contention occurs and power is wasted. If no units drive the bus, it can ﬂoat to an invalid logic level that causes the receivers to waste power. Moreover, it can be difﬁcult to switch enable signals at exactly the same time when they are distributed across a large chip. Delay between different enables switching can cause contention. Given these problems, multiplexers are now preferred over tristate busses.


1.4.8 Multiplexers


Multiplexers are key components in CMOS memory elements and data manipulation structures. A multiplexer chooses the output from among several inputs based on a select signal. A 2-input, or 2:1 multiplexer, chooses input D0 when the select is 0 and input D1 when the select is 1. The truth table is given in Table 1.6; the logic function is Y = S · D0 + S · D1.


Two transmission gates can be tied together to form a compact 2-input multiplexer, as shown in Figure 1.28(a). The select and its complement enable exactly one of the two transmission gates at any given time. The complementary select S is often not drawn in the symbol, as shown in Figure 1.28(b).


Again, the transmission gates produce a nonrestoring multiplexer. We could build a restoring, inverting multiplexer out of gates in several ways. One is the compound gate of Figure 1.18(e), connected as shown in Figure 1.29(a). Another is to gang together two tristate inverters, as shown in Figure 1.29(b). Notice that the schematics of these two approaches are nearly identical, save that the pull-up network has been slightly simpliﬁed and permuted in Figure 1.29(b). This is possible because the select and its complement are mutually exclusive. The tristate approach is slightly more compact and faster because it


TABLE 1.6  Multiplexer truth table


|S / S |D1 |D 0 |Y ||
|---|---|---|---|---|

|0 / 1 |X |0 |0 ||

|0 / 1 |X |1 |1 ||

|1 / 0 |0 |X |0 ||

|1 / 0 |1 |X |1 ||

FIGURE 1.27  Tristate Inverter


EN EN


EN = 0 Y = 'Z'


EN = 1 Y = A


FIGURE 1.28  Transmission  gate multiplexer


S


D0七


D1-口


0 1


D0 D1


S。


16


requires less internal wire. Again, if the complementary select is generated within the cell,it is omitted from the symbol (Figure 1.29(c)).


Larger multiplexers can be built from multiple 2-input multiplexers or by directly ganging together several tristates. The latter approach requires decoded enable signals for each tristate; the enables should switch simultaneously to prevent contention. 4-input(4:1) multiplexers using each of these approaches are shown in Figure 1.30. In practice,both inverting and noninverting multiplexers are simply called multiplexers or muxes.


1.4.9 Sequential Circuits


So far, we have considered combinational circuits, whose outputs depend only on the current inputs. Sequential circuits have memory: their outputs depend on both current and previous inputs. Using the combinational circuits developed so far, we can now build sequential circuits such as latches and ﬂip-ﬂops. These elements receive a clock, CLK, and a data input, D, and produce an output, Q. A D latch is transparent when CLK = 1, meaning that Q follows D. It becomes opaque when CLK = 0, meaning Q retains its previous value and ignores changes in D. An edge-triggered ﬂip-ﬂop copies D to Q on the rising edge of CLK and remembers its old value at other times.


FIGURE 1.29  Inverting multiplexer


FIGURE 1.30  4:1 multiplexer


S D0


D1


↓子


0Y


S0


)-Y


S1


D2 D3


D0


D2


运远云


D3


S1S0 S1S0 S1S0 S1S0


1.4      CMOS Logic 17


1.4.9.1 Latches A D latch built from a 2-input multiplexer and two inverters is shown in


Figure 1.31(a). The multiplexer can be built from a pair of transmission gates, shown in


Figure 1.31(b), because the inverters are restoring. This latch also produces a complementary output, Q. When CLK = 1, the latch is transparent and D ﬂows through to Q (Figure


1.31(c)). When CLK falls to 0, the latch becomes opaque. A feedback path around the


inverter pair is established (Figure 1.31(d)) to hold the current state of Q indeﬁnitely.


The D latch is also known as a level-sensitive latch because the state of the output is


dependent on the level of the clock signal, as shown in Figure 1.31(e). The latch shown is


a positive-level-sensitive latch, represented by the symbol in Figure 1.31(f ). By inverting


the control connections to the multiplexer, the latch becomes negative-level-sensitive.


1.4.9.2 Flip-Flops By combining two level-sensitive latches, one negative-sensitive and


one positive-sensitive, we construct the edge-triggered ﬂip-ﬂop shown in Figure 1.32(a–


b). The ﬁrst latch stage is called the master and the second is called the slave.


While CLK is low, the master negative-level-sensitive latch output (QM ) follows the


D input while the slave positive-level-sensitive latch holds the previous value (Figure


1.32(c)). When the clock transitions from 0 to 1, the master latch becomes opaque and


holds the D value at the time of the clock transition. The slave latch becomes transparent,


passing the stored master value (QM ) to the output of the slave latch (Q). The D input is


blocked from affecting the output because the master is disconnected from the D input


(Figure 1.32(d)). When the clock transitions from 1 to 0, the slave latch holds its value


and the master starts sampling the input again.


While we have shown a transmission gate multiplexer as the input stage, good design


practice would buffer the input and output with inverters, as shown in Figure 1.32(e), to


FIGURE 1.31  CMOS positive-level-sensitive D latch


1 0


9


CLK


Q


d


-古


Q Q


(b)口


CLK = 1 D -0-


CLK = 0 D


LatchQ


18


preserve what we call “modularity.” Modularity is explained further in Section 1.6.2 and robust latches and registers are discussed further in Section 10.3.


In summary, this ﬂip-ﬂop copies D to Q on the rising edge of the clock, as shown in Figure 1.32(f ). Thus, this device is called a positive-edge triggered ﬂip-ﬂop (also called a D ﬂip-ﬂop, D register, or master–slave ﬂip-ﬂop). Figure 1.32(g) shows the circuit symbol for the ﬂip-ﬂop. By reversing the latch polarities, a negative-edge triggered ﬂip-ﬂop may be


FIGURE 1.32  CMOS positive-edge-triggered D ﬂip-ﬂop


CLK = 1 D


CLK = 0


QM


(g)


D 0d


LatchQMLatch CLK


CLKro<


3


口 CLK


1.5      CMOS Fabrication and Layout 19


constructed. A collection of D ﬂip-ﬂops sharing a common clock input is called a register.


A register is often drawn as a ﬂip-ﬂop with multi-bit D and Q busses.


In Section 10.2.5 we will see that ﬂip-ﬂops may experience hold-time failures if the system has too much clock skew, i.e., if one ﬂip-ﬂop triggers early and another triggers late because of variations in clock arrival times. In industrial designs, a great deal of effort is devoted to timing simulations to catch hold-time problems. When design time is more important (e.g., in class projects), hold-time problems can be avoided altogether by distributing a two-phase nonoverlapping clock. Figure 1.33 shows the ﬂip-ﬂop clocked with two nonoverlapping phases. As long as the phases never overlap, at least one latch will be opaque at any given time and hold-time problems cannot occur.


1.5 CMOS Fabrication and Layout


Now that we can design logic gates and registers from transistors, let us consider how the transistors are built. Designers need to understand the physical implementation of circuits because it has a major impact on performance, power, and cost.


Transistors are fabricated on thin silicon wafers that serve as both a mechanical support and an electrical common point called the substrate. We can examine the physical layout of transistors from two perspectives. One is the top view, obtained by looking down on a wafer. The other is the cross-section, obtained by slicing the wafer through the middle of a transistor and looking at it edgewise. We begin by looking at the cross-section of a complete CMOS inverter. We then look at the top view of the same inverter and deﬁne a set of masks used to manufacture the different parts of the inverter. The size of the transistors and wires is set by the mask dimensions and is limited by the resolution of the manufacturing process. Continual advancements in this resolution have fueled the exponential growth of the semiconductor industry.


1.5.1 Inverter Cross-Section


Figure 1.34 shows a cross-section and corresponding schematic of an inverter. (See the inside front cover for a color cross-section.) In this diagram, the inverter is built on a p-type substrate. The pMOS transistor requires an n-type body region, so an n-well is diffused into the substrate in its vicinity. As described in Section 1.3, the nMOS transistor


FIGURE 1.33 CMOS ﬂip-ﬂop with two-phase nonoverlapping clocks


φ2


φ1


20


has heavily doped n-type source and drain regions and a polysilicon gate over a thin layer of silicon dioxide (SiO2, also called gate oxide). n+ and p+ diffusion regions indicate heavily doped n-type and p-type silicon. The pMOS transistor is a similar structure with p-type source and drain regions. The polysilicon gates of the two transistors are tied together somewhere off the page and form the input A. The source of the nMOS transistor is connected to a metal ground line and the source of the pMOS transistor is connected to a metal VDD line. The drains of the two transistors are connected with metal to form the output Y. A thick layer of SiO2 called ﬁeld oxide prevents metal from shorting to other layers except where contacts are explicitly etched.


A junction between metal and a lightly doped semiconductor forms a Schottky diode that only carries current in one direction. When the semiconductor is doped more heavily, it forms a good ohmic contact with metal that provides low resistance for bidirectional currentﬂow. The substrate must be tied to a low potential to avoid forward-biasing the p-n junction between the p-type substrate and the n+ nMOS source or drain. Likewise, the n-well must be tied to a high potential. This is done by adding heavily doped substrate and well contacts,or taps, to connect GND and VDD to the substrate and n-well, respectively.


1.5.2  Fabrication Process


For all their complexity, chips are amazingly inexpensive because all the transistors and wires can be printed in much the same way as books. The fabrication sequence consists of a series of steps in which layers of the chip are deﬁned through a process called photolithography.


Because a whole wafer full of chips is processed in each step, the cost of the chip is proportional to the chip area, rather than the number of transistors. As manufacturing advances allow engineers to build smaller transistors and thus ﬁt more in the same area, each transistor gets cheaper. Smaller transistors are also faster because electrons don’t have to travel as far to get from the source to the drain, and they consume less energy because fewer electrons are needed to charge up the gates! This explains the remarkable trend for computers and electronics to become cheaper and more capable with each generation.


The inverter could be deﬁned by a hypothetical set of six masks: n-well, polysilicon,n+ diffusion, p+ diffusion, contacts, and metal (for fabrication reasons discussed in Chapter 3, the actual mask set tends to be more elaborate). Masks specify where the components will be manufactured on the chip. Figure 1.35(a) shows a top view of the six masks.


(See also the inside front cover for a color picture.) The cross-section of the inverter from Figure 1.34 was taken along the dashed line. Take some time to convince yourself how the top view and cross-section relate; this is critical to understanding chip layout.


FIGURE 1.34   Inverter cross-section with well and substrate contacts. Color version on inside front cover.


p-substrate


n-well


Substrate Tap


Well Tap


□n+ diffusion□p+ diffusion ATTYpolysilicon metal1


nMOS Transistor


pMOS Transistor


LTGate


GateV17


1.5      CMOS Fabrication and Layout 21


Consider a simple fabrication process to illustrate the concept. The process begins with the creation of an n-well on a bare p-type silicon wafer. Figure 1.36 shows cross-sections of the wafer after each processing step involved in forming the n-well; Figure 1.36(a) illustrates the bare substrate before processing. Forming the n-well requires adding enough Group V dopants into the silicon substrate to change the substrate from p-type to n-type in the region of the well. To deﬁne what regions receive n-wells, we grow a protective layer of


FIGURE 1.35   Inverter mask set. Color version on inside front cover.


1I□


□


CHFAAFRFFRG-CHAG


Metal


Contact


n+ Diffusion


p+ Diffusion n-well


22


oxide over the entire wafer, then remove it where we want the wells. We then add the ntype dopants; the dopants are blocked by the oxide, but enter the substrate and form the wells where there is no oxide. The next paragraph describes these steps in detail.


The wafer is ﬁrst oxidized in a high-temperature (typically 900–1200 °C) furnace that causes Si and O2 to react and become SiO2 on the wafer surface (Figure 1.36(b)). The oxide must be patterned to deﬁne the n-well. An organic photoresist2 that softens where


FIGURE 1.36  Cross-sections while manufacturing the n-well


we n-well


Photoresist


(h)


2Engineers have experimented with many organic polymers for photoresists. In 1958, Brumford and Walker reported that Jello™ could be used for masking. They did extensive testing, observing that “various Jellos™ were evaluated with lemon giving the best result.”


1.5      CMOS Fabrication and Layout 23


exposed to light is spun onto the wafer (Figure 1.36(c)). The photoresist is exposed through the n-well mask (Figure 1.35(b)) that allows light to pass through only where the well should be. The softened photoresist is removed to expose the oxide (Figure 1.36(d)).


The oxide is etched with hydroﬂuoric acid (HF) where it is not protected by the photoresist (Figure 1.36(e)), then the remaining photoresist is stripped away using a mixture of acids called piranha etch (Figure 1.36(f )). The well is formed where the substrate is not covered with oxide. Two ways to add dopants are diffusion and ion implantation. In the diffusion process, the wafer is placed in a furnace with a gas containing the dopants. When heated, dopant atoms diffuse into the substrate. Notice how the well is wider than the hole in the oxide on account of lateral diffusion (Figure 1.36(g)). With ion implantation, dopant ions are accelerated through an electric ﬁeld and blasted into the substrate. In either method, the oxide layer prevents dopant atoms from entering the substrate where no well is intended. Finally, the remaining oxide is stripped with HF to leave the bare wafer with wells in the appropriate places.


The transistor gates are formed next. These consist of polycrystalline silicon, generally called polysilicon, over a thin layer of oxide. The thin oxide is grown in a furnace. Then the wafer is placed in a reactor with silane gas (SiH4) and heated again to grow the polysilicon layer through a process called chemical vapor deposition. The polysilicon is heavily doped to form a reasonably good conductor. The resulting cross-section is shown in Figure 1.37(a).


As before, the wafer is patterned with photoresist and the polysilicon mask (Figure


1.35(c)), leaving the polysilicon gates atop the thin gate oxide (Figure 1.37(b)).


The n+ regions are introduced for the transistor active area and the well contact. As with the well, a protective layer of oxide is formed (Figure 1.37(c)) and patterned with the n-diffusion mask (Figure 1.35(d)) to expose the areas where the dopants are needed (Figure 1.37(d)). Although the n+ regions in Figure 1.37(e) are typically formed with ion implantation, they were historically diffused and thus still are often called n-diffusion.


Notice that the polysilicon gate over the nMOS transistor blocks the diffusion so the source and drain are separated by a channel under the gate. This is called a self-aligned process because the source and drain of the transistor are automatically formed adjacent to the gate without the need to precisely align the masks. Finally, the protective oxide is stripped(Figure 1.37(f )).


The process is repeated for the p-diffusion mask (Figure 1.35(e)) to give the structure of Figure 1.38(a). Oxide is used for masking in the same way, and thus is not shown. Theﬁeld oxide is grown to insulate the wafer from metal and patterned with the contact mask(Figure 1.35(f )) to leave contact cuts where metal should attach to diffusion or polysilicon(Figure 1.38(b)). Finally, aluminum is sputtered over the entire wafer, ﬁlling the contact cuts as well. Sputtering involves blasting aluminum into a vapor that evenly coats the wafer. The metal is patterned with the metal mask (Figure 1.35(g)) and plasma etched to remove metal everywhere except where wires should remain (Figure 1.38(c)). This completes the simple fabrication process.


Modern fabrication sequences are more elaborate because they must create complex doping proﬁles around the channel of the transistor and print features that are smaller than the wavelength of the light being used in lithography. However, masks for these elaborations can be automatically generated from the simple set of masks we have just examined. Modern processes also have 5–10+ layers of metal, so the metal and contact steps must be repeated for each layer. Chip manufacturing has become a commodity, and many different foundries will build designs from a basic set of masks.


24


1.5.3 Layout Design Rules


Layout design rules describe how small features can be and how closely they can be reliably packed in a particular manufacturing process. Industrial design rules are usually speciﬁed in microns. This makes migrating from one process to a more advanced process or a different foundry’s process difﬁcult because not all rules scale in the same way.


Universities sometimes simplify design by using scalable design rules that are conservative enough to apply to many manufacturing processes. Mead and Conway [Mead80]popularized scalable design rules based on a single parameter, , that characterizes the resolution of the process.  is generally half of the minimum drawn transistor channel length.


This length is the distance between the source and drain of a transistor and is set by the minimum width of a polysilicon wire. For example, a 180 nm process has a minimum polysilicon width (and hence transistor length) of 0.18 m and uses design rules with


FIGURE 1.37  Cross-sections while manufacturing polysilicon and n-diffusion


n-well n-well


N


p-substrate n+


Thin gate oxide


Thin gate oxide Polysilicon


w n-well


1.5      CMOS Fabrication and Layout 25


= 0.09 m.3 Lambda-based rules are necessarily conservative because they round up dimensions  to an integer multiple of . However, they make scaling layout trivial; the same layout can be moved to a new process simply by specifying a new value of . This chapter will present design rules in terms of . The potential density advantage of micron rules is sacriﬁced for simplicity and easy scalability of lambda rules. Designers often describe a process by its feature size. Feature size refers to minimum transistor length, so  is half the feature size.


Unfortunately, below 180 nm, design rules have become so complex and processspeciﬁc that scalable design rules are difﬁcult to apply. However, the intuition gained from a simple set of scalable rules is still a valuable foundation for understanding the more complex rules. Chapter 3 will examine some of these process-speciﬁc rules in more detail.


The MOSIS service [Piña02] is a low-cost prototyping service that collects designs from academic, commercial, and government customers and aggregates them onto one mask set to share overhead costs and generate production volumes sufﬁcient to interest fabrication companies. MOSIS has developed a set of scalable lambda-based design rules that covers a wide range of manufacturing processes. The rules describe the minimum width to avoid breaks in a line, minimum spacing to avoid shorts between lines, and minimum overlap to ensure that two layers completely overlap.


A conservative but easy-to-use set of design rules for layouts with two metal layers in an n-well process is as follows:


Metal and diffusion have minimum width and spacing of 4 .


Contacts are 2lx2land must be surrounded by 1l on the layers above andContacts are 2 × 2  and must be surrounded by 1  on the layers above and


below.


●Polysilicon uses a width of 2 .


FIGURE 1.38  Cross-sections while manufacturing p-diffusion, contacts, and metal


Thick field oxide


3Some 180 nm lambda-based rules actually set  = 0.10 m, then shrink the gate by 20 nm while generating masks. This keeps 180 nm gate lengths but makes all other features slightly larger.


26


Polysilicon overlaps diffusion by 2 l where a transistor is desired and has a spacingPolysilicon overlaps diffusion by 2  where a transistor is desired and has a spacing  of 1  away where no transistor is desired.


Polysilicon and contacts have a spacing of 3 & from other polysilicon or contacts.Polysilicon and contacts have a spacing of 3  from other polysilicon or contacts.  N-well surrounds pMOS transistors by 6 2 and avoids nMOS transistors by 6 2.N-well surrounds pMOS transistors by 6  and avoids nMOS transistors by 6 .


Figure 1.39 shows the basic MOSIS design rules for a process with two metal layers.


Section 3.3 elaborates on these rules and compares them with industrial design rules.


In a three-level metal process, the width of the third layer is typically 6  and the spacing 4 . In general, processes with more layers often provide thicker and wider toplevel metal that has a lower resistance.


Transistor dimensions are often speciﬁed by their Width/Length (W/L) ratio. For example, the nMOS transistor in Figure 1.39 formed where polysilicon crosses n-diffusion has a W/L of 4/2. In a 0.6 m process, this corresponds to an actual width of 1.2 m and a length of 0.6 m. Such a minimum-width contacted transistor is often called a unit transistor.4 pMOS transistors are often wider than nMOS transistors because holes move more slowly than electrons so the transistor has to be wider to deliver the same current. Figure


1.40(a) shows a unit inverter layout with a unit nMOS transistor and a double-sized pMOS transistor. Figure 1.40(b) shows a schematic for the inverter annotated with Width/Length for each transistor. In digital systems, transistors are typically chosen to have the minimum possible length because short-channel transistors are faster, smaller, and consume less power. Figure 1.40(c) shows a shorthand we will often use, specifying multiples of unit width and assuming minimum length.


FIGURE 1.39  Simpliﬁed -based design rules


Metal1


Metal2


Diffusion Polysilicon


Metal1-Diffusion Contact


Metal1-


Polysilicon Contact


Metal1-Metal2 Vias


4 4


1 1 2乙 7


**


周叁


--花2☑


11111n


2 4


width


spacing


4Such small transistors in modern processes often behave slightly differently than their wider counterparts.


Moreover, the transistor will not operate if either contact is damaged. Industrial designers often use a transistor wide enough for two contacts (9 ) as the unit transistor to avoid these problems.


1.5      CMOS Fabrication and Layout 27


1.5.4 Gate Layouts


A good deal of ingenuity can be exercised and a vast amount of


time wasted exploring layout topologies to minimize the size of


a gate or other cell such as an adder or memory element. For


many applications, a straightforward layout is good enough and


can be automatically generated or rapidly built by hand. This


section presents a simple layout style based on a “line of diffusion” rule that is commonly used for standard cells in automated


layout systems. This style consists of four horizontal strips:


metal ground at the bottom of the cell, n-diffusion, p-diffusion,


and metal power at the top. The power and ground lines are


often called supply rails. Polysilicon lines run vertically to form


transistor gates. Metal wires within the cell connect the transistors appropriately.


Figure 1.41(a) shows such a layout for an inverter. The


input A can be connected from the top, bottom, or left in


polysilicon. The output Y is available at the right side of the


cell in metal. Recall that the p-substrate and n-well must be tied to ground and power,respectively. Figure 1.41(b) shows the same inverter with well and substrate taps placed under the power and ground rails, respectively. Figure 1.42 shows a 3-input NAND gate.


Notice how the nMOS transistors are connected in series while the pMOS transistors are connected in parallel. Power and ground extend 2  on each side so if two gates were abutted the contents would be separated by 4 , satisfying design rules. The height of the cell is 36 , or 40  if the 4  space between the cell and another wire above it is counted. All these examples use transistors of width 4 . Choice of transistor width is addressed further in Chapters 4–5 and cell layout styles are discussed in Section 14.7.


These cells were designed such that the gate connections are made from the top or bottom in polysilicon. In contemporary standard cells, polysilicon is generally not used as a routing layer so the cell must allow metal2 to metal1 and metal1 to polysilicon contacts


FIGURE 1.41  Inverter cell layout


GND VDD


FIGURE 1.40  Inverter with dimensions labeled


8/2 4/2


2 1


FIGURE 1.42  3-input NAND standard  cell gate layouts


40 λ


32 λ


4 λ


GND1111


28


to each gate. While this increases the size of the cell, it allows free access to all terminals on metal routing layers.


1.5.5 Stick Diagrams


Because layout is time-consuming, designers need fast ways to plan cells and estimate area before committing to a full layout. Stick diagrams are easy to draw because they do not need to be drawn to scale. Figure 1.43 and the inside front cover show stick diagrams for an inverter and a 3-input NAND gate. While this book uses stipple patterns, layout designers use dry-erase markers or colored pencils.


With practice, it is easy to estimate the area of a layout from the corresponding stick diagram even though the diagram is not to scale. Although schematics focus on transistors, layout area is usually determined by the metal wires.


Transistors are merely widgets that ﬁt under the wires. We


区


deﬁne a routing track as enough space to place a wire and the required spacing to the next wire. If our wires have a width of 4  and a spacing of 4  to the next wire, the track pitch is 8 , as shown in Figure 1.44(a). This pitch also leaves room for a transistor to be placed between the wires (Figure


1.44(b)). Therefore, it is reasonable to estimate the height and width of a cell by counting the number of metal tracks and multiplying by 8 . A slight complication is the required spacing of 12  between nMOS and pMOS transistors set by the well, as shown in Figure 1.45(a). This space can be occupied by an additional track of wire, shown in Figure


1.45(b). Therefore, an extra track must be allocated between nMOS and pMOS transistors regardless of whether wire is actually used in that track. Figure 1.46 shows how to count tracks to estimate the size of a 3-input NAND. There are four vertical wire tracks, multiplied by 8  per track to give a cell width of 32 . There are ﬁve horizontal tracks, giving a cell height of 40 . Even though the horizontal tracks are not drawn to scale, they are still easy to count. Figure 1.42


FIGURE 1.43  Stick diagrams of inverter and 3-input NAND gate. Color version on inside front cover.


GND r277777


111Metal1


pdiff


ndiff


FIGURE 1.44  Pitch of routing tracks


FIGURE 1.45  Spacing between nMOS and pMOS transistors


4λ


1.6      Design Partitioning 29


shows that the actual NAND gate layout matches the dimensions predicted by the stick diagram. If transistors are wider than 4 , the extra width must be factored into the area estimate. Of course, these estimates are oversimpliﬁcations of the complete design rules and a trial layout should be performed for truly critical cells.


Example 1.3


Sketch a stick diagram for a CMOS gate computing Y = (A + B + C) · D (see Figure 1.18) and estimate the cell width and height.


SOLUTION: Figure 1.47 shows a stick diagram.


Counting horizontal and vertical pitches gives an estimated cell size of 40 by 48 .


1.6 Design Partitioning


By this point, you know that MOS transistors behave as voltage-controlled switches. You know how to build logic gates out of transistors. And you know how transistors are fabricated and how to draw a layout that speciﬁes how transistors should be placed and connected together. You know enough to start building your own simple chips.


The greatest challenge in modern VLSI design is not in designing the individual transistors but rather in managing system complexity. Modern System-On-Chip (SOC)designs combine memories, processors, high-speed I/O interfaces, and dedicated application-speciﬁc logic on a single chip. They use hundreds of millions or billions of transistors and cost tens of millions of dollars (or more) to design. The implementation


FIGURE 1.47  CMOS compound gate for function Y = (A + B + C) · D


5 tracks = 40


6 tracks = 48


FIGURE 1.46  3-input NAND gate area estimation


40


32


30


must be divided among large teams of engineers and each engineer must be highly productive. If the implementation is too rigidly partitioned, each block can be optimized without regard to its neighbors, leading to poor system results. Conversely, if every task is interdependent with every other task, design will progress too slowly. Design managers face the challenge of choosing a suitable trade-off between these extremes. There is no substitute for practical experience in making these choices, and talented engineers who have experience with multiple designs are very important to the success of a large project.


Design proceeds through multiple levels of abstraction, hiding details until they become necessary. The practice of structured design, which is also used in large software projects,uses the principles of hierarchy, regularity, modularity, and locality to manage the complexity.


1.6.1 Design Abstractions


Digital VLSI design is often partitioned into ﬁve levels of abstractions: architecture design,microarchitecture design, logic design, circuit design, and physical design. Architecture describes the functions of the system. For example, the x86 microprocessor architecture speciﬁes the instruction set, register set, and memory model. Microarchitecture describes how the architecture is partitioned into registers and functional units. The 80386, 80486,Pentium, Pentium II, Pentium III, Pentium 4, Core, Core 2, Atom, Cyrix MII, AMD Athlon, and Phenom are all microarchitectures offering different performance / transistor count / power trade-offs for the x86 architecture. Logic describes how functional units are constructed. For example, various logic designs for a 32-bit adder in the x86 integer unit include ripple carry, carry lookahead, and carry select. Circuit design describes how transistors are used to implement the logic. For example, a carry lookahead adder can use static CMOS circuits, domino circuits, or pass transistors. The circuits can be tailored to emphasize high performance or low power. Physical design describes the layout of the chip. Analog and RF VLSI design involves the same steps but with different layers of abstraction.


These elements are inherently interdependent and all inﬂuence each of the design objectives. For example, choices of microarchitecture and logic are strongly dependent on the number of transistors that can be placed on the chip, which depends on the physical design and process technology. Similarly, innovative circuit design that reduces a cache access from two cycles to one can inﬂuence which microarchitecture is most desirable. The choice of clock frequency depends on a complex interplay of microarchitecture and logic,circuit design, and physical design. Deeper pipelines allow higher frequencies but consume more power and lead to greater performance penalties when operations early in the pipeline are dependent on those late in the pipeline. Many functions have various logic and circuit designs trading speed for area, power, and design effort. Custom physical design allows more compact, faster circuits and lower manufacturing costs, but involves an enormous labor cost. Automatic layout with CAD systems reduces the labor and achieves faster times to market.


To deal with these interdependencies, microarchitecture, logic, circuit, and physical design must occur, at least in part, in parallel. Microarchitects depend on circuit and physical design studies to understand the cost of proposed microarchitectural features. Engineers are sometimes categorized as “short and fat” or “tall and skinny” (nothing personal,we assure you!). Tall, skinny engineers understand something about a broad range of topics. Short, fat engineers understand a large amount about a narrow ﬁeld. Digital VLSI design favors the tall, skinny engineer who can evaluate how choices in one part of the system impact other parts of the system.


1.6      Design Partitioning 31


1.6.2 Structured Design


Hierarchy is a critical tool for managing complex designs. A large system can be partitioned hierarchically into multiple cores. Each core is built from various units. Each unit in turn is composed of multiple functional blocks.5 These blocks in turn are built from cells,which ultimately are constructed from transistors. The system can be more easily understood at the top level by viewing components as black boxes with well-deﬁned interfaces and functions rather than looking at each individual transistor. Logic, circuit, and physical views of the design should share the same hierarchy for ease of veriﬁcation. A design hierarchy can be viewed as a tree structure with the overall chip as the root and the primitive cells as leafs.


Regularity aids the management of design complexity by designing the minimum number of different blocks. Once a block is designed and veriﬁed, it can be reused in many places. Modularity requires that the blocks have well-deﬁned interfaces to avoid unanticipated interactions. Locality involves keeping information where it is used, physically and temporally. Structured design is discussed further in Section 14.2.


1.6.3 Behavioral, Structural, and Physical Domains


An alternative way of viewing design partitioning is shown with the Y-chart shown in Figure 1.48 [Gajski83, Kang03]. The radial lines on the Y-chart represent three distinct design domains: behavioral, structural, and physical. These domains can be used to describe the design of almost any artifact and thus form a general taxonomy for describing


FIGURE 1.48  Y Diagram (Reproduced from [Kang03] with permission of The McGraw-Hill  Companies.)


Structural


Behavioral


Geometrical/Physical


Processor


Register ALU


Leaf Cell


Transistor


Mask


Cell


Module


Chip


Boolean


●Finite


Algorithm


Placement


Equation


Description


State Machine


Floorplan


Domain


5Some designers refer to both units and functional blocks as modules.


the design process. Within each domain there are a number of levels of design abstraction that start at a very high level and descend eventually to the individual elements that need to be aggregated to yield the top level function (i.e., transistors in the case of chip design).


The behavioral domain describes what a particular system does. For instance, at the highest level we might specify a telephone touch-tone generator. This behavior can be successively reﬁned to more precisely describe what needs to be done in order to build the tone generator (i.e., the frequencies desired, output levels, distortion allowed, etc.).


At each abstraction level, a corresponding structural description can be developed.


The structural domain describes the interconnection of modules necessary to achieve a particular behavior. For instance, at the highest level, the touch-tone generator might consist of a keypad, a tone generator chip, an audio ampliﬁer, a battery, and a speaker. Eventually at lower levels of abstraction, the individual gate and then transistor connections required to build the tone generator are described.


For each level of abstraction, the physical domain description explains how to physically construct that level of abstraction. At high levels, this might consist of an engineering drawing showing how to put together the keypad, tone generator chip, battery, and speaker in the associated housing. At the top chip level, this might consist of a ﬂoorplan,and at lower levels, the actual geometry of individual transistors.


The design process can be viewed as making transformations from one domain to another while maintaining the equivalency of the domains. Behavioral descriptions are transformed to structural descriptions, which in turn are transformed to physical descriptions. These transformations can be manual or automatic. In either case, it is normal design practice to verify the transformation of one domain to the other. This ensures that the design intent is carried across the domain boundaries. Hierarchically specifying each domain at successively detailed levels of abstraction allows us to design very large systems. The reason for strictly describing the domains and levels of abstraction is to deﬁne a precise design process in which the ﬁnal function of the system can be traced all the way back to the initial behavioral description. In an ideal ﬂow, there should be no opportunity to produce an incorrect design. If anomalies arise, the design process is corrected so that those anomalies will not reoccur in the future. A designer should acquire a rigid discipline with respect to the design process, and be aware of each transformation and how and why it is failproof. Normally, these steps are fully automated in a modern design process, but it is important to be aware of the basis for these steps in order to debug them if they go astray.


The Y diagram can be used to illustrate each domain and the transformations between domains at varying levels of design abstraction. As the design process winds its way from the outer to inner rings, it proceeds from higher to lower levels of abstraction and hierarchy.


Most of the remainder of this chapter is a case study in the design of a simple microprocessor to illustrate the various aspects of VLSI design applied to a nontrivial system.


We begin by describing the architecture and microarchitecture of the processor. We then consider logic design and discuss hardware description languages. The processor is built with static CMOS circuits, which we examined in Section 1.4; transistor-level design and netlist formats are discussed. We continue exploring the physical design of the processor including ﬂoorplanning and area estimation. Design veriﬁcation is critically important and happens at each level of the hierarchy for each element of the design. Finally, the layout is converted into masks so the chip can be manufactured, packaged, and tested.


1.7      Example: A Simple MIPS Microprocessor 33


1.7 Example: A Simple MIPS Microprocessor


We consider an 8-bit subset of the MIPS microprocessor architecture [Patterson04,Harris07] because it is widely studied and is relatively simple, yet still large enough to illustrate hierarchical design. This section describes the architecture and the multicycle microarchitecture we will be implementing. If you are not familiar with computer architecture, you can regard the MIPS processor as a black box and skip to Section 1.8.


A set of laboratory exercises is available at www.cmosvlsi.com in which you can learn VLSI design by building the microprocessor yourself using a free open-source CAD tool called Electric or with commercial design tools from Cadence and Synopsys.


1.7.1 MIPS Architecture


The MIPS32 architecture is a simple 32-bit RISC architecture with relatively few idiosyncrasies. Our subset of the architecture uses 32-bit instruction encodings but only eight 8-bit general-purpose registers named $0–$7. We also use an 8-bit program counter(PC). Register $0 is hardwired to contain the number 0. The instructions are ADD, SUB,AND, OR, SLT, ADDI, BEQ, J, LB, and SB.


The function and encoding of each instruction is given in Table 1.7. Each instruction is encoded using one of three templates: R, I, and J. R-type instructions (register-based)are used for arithmetic and specify two source registers and a destination register. I-type instructions are used when a 16-bit constant (also known as an immediate) and two registers must be speciﬁed. J-type instructions ( jumps) dedicate most of the instruction word to a 26-bit jump destination. The format of each encoding is deﬁned in Figure 1.49. The six most signiﬁcant bits of all formats are the operation code (op). R-type instructions all share op = 000000 and use six more funct bits to differentiate the functions.


TABLE 1.7  MIPS instruction set (subset supported)


|Instruction |Function |Encoding |op |funct |
|---|---|---|---|---|

|add $1, $2, $3 |addition: $1 <- $2 + $3 |R |000000 |100000 |

|sub $1, $2, $3 |subtraction: $1 <- $2 – $3 |R |000000 |100010 |

|and $1, $2, $3 |bitwise and: $1 <- $2 and $3 |R |000000 |100100 |

|or $1, $2, $3 |bitwise or: $1 <- $2 or $3 |R |000000 |100101 |

|slt $1, $2, $3 |set less than: $1 <- 1 if $2 < $3 $1 <- 0 otherwise |R |000000 |101010 |

|addi $1, $2, imm |add immediate: $1 <- $2 + imm |I |001000 |n/a |

|beq $1, $2, imm |branch if equal: PC <- PC + imm × 4a |I |000100 |n/a |

|j destination |jump: PC <- destinationa |J |000010 |n/a |

|lb $1, imm($2) |load byte: $1 <- mem[$2 + imm] |I |100000 |n/a |

|sb $1, imm($2) |store byte: mem[$2 + imm] <- $1 |I |101000 |n/a |

a.Technically, MIPS addresses specify bytes. Instructions require a 4-byte word and must begin at addresses that are a multiple of four. To most effectively use instruction bits in the full 32-bit MIPS architecture, branch and jump constants are


speciﬁed in words and must be multiplied by four (shifted left 2 bits) to be converted to byte addresses.


34


We can write programs for the MIPS processor in assembly language, where each line of the program contains one instruction such as ADD or BEQ. However, the MIPS hardware ultimately must read the program as a series of 32-bit numbers called machine language. An assembler automates the tedious process of translating from assembly language to machine language using the encodings deﬁned in Table 1.7 and Figure 1.49. Writing nontrivial programs in assembly language is also tedious, so programmers usually work in a high-level language such as C or Java. A compiler translates a program from high-level language source code into the appropriate machine language object code.


Example 1.4


Figure 1.50 shows a simple C program that computes the nth Fibonacci number fn deﬁned recursively for n > 0 as fn = fn–1 + fn–2, f–1 = –1, f0 = 1. Translate the program into MIPS assembly language and machine language.


SOLUTION: Figure 1.51 gives a commented assembly language program. Figure 1.52 translates the assembly language to machine language.


1.7.2 Multicycle MIPS Microarchitecture


We will implement the multicycle MIPS microarchitecture given in Chapter 5 of[Patterson04] and Chapter 7 of [Harris07] modiﬁed to process 8-bit data. The microarchitecture is illustrated in Figure 1.53. Light lines indicate individual signals while heavy


FIGURE 1.49  Instruction encoding formats


int fib(void)


{


int n = 8;            /* compute nth Fibonacci number */


int f1 = 1, f2 = -1;  /* last two Fibonacci numbers */


while (n != 0) {      /* count down to n = 0 */


f1 = f1 + f2;


f2 = f1 - f2;


n = n - 1;


}


return f1;


FIGURE 1.50  C Code for Fibonacci program


Format Example


Encoding


R


I


J


||0 |ra |rb |rd |0 |funct |
|---|---|---|---|---|---|---|

|6 |5 |5 |5 |16 |16 |16 |

||op |ra |rb |imm |imm |imm |

|6 26 |6 26 |6 26 |6 26 |6 26 |6 26 ||

||op |dest |dest |dest |dest |dest |

5


add $rd, $ra, $rb


beq $ra, $rb, imm


j dest


1.7      Example: A Simple MIPS Microprocessor 35


# fib.asm


# Register usage: $3: n $4: f1 $5: f2


|# |return value written to |address 255 ||
|---|---|---|---|

|fib: |addi $3, $0, 8      # |initialize n=8 ||

||addi $4, $0, 1      # initialize |f1 = 1 ||

||addi $5, $0, -1     # initialize |f2 = -1 ||

|loop: |beq $3, $0, end     # |Done with loop if n = 0 ||

||add $4, $4, $5      # |f1 = f1 + f2 ||

||sub $5, $4, $5      # |f2 = f1 - f2 ||

||addi $3, $3, -1     # n |= n - 1 ||

||j loop              # |repeat until done ||

|end: |sb $4, 255($0)      # |store result in address |255 |

FIGURE 1.51  Assembly language code for Fibonacci program


Hexadecimal Encoding


|Instruction |Binary |Encoding|Encoding ||
|---|---|---|---|---|

|addi $3, $0, 8 |001000 |00000 |00011 |000000000000100 |

|addi $4, $0, 1 |001000 |00000 |00100 |000000000000000 |

|addi $5, $0, -1 |001000 |00000 |00101 |111111111111111 |

|beq  $3, $0, end |000100 |00011 |00000 |000000000000010 |

|add  $4, $4, $5 |000000 |00100 |00101 00100 |00000 10000 |

|sub  $5, $4, $5 |000000 |00100 |00101 00101 |00000 10001 |

|addi $3, $3, -1 |001000 |00011 |00011 |111111111111111 |

|j loop |000010 ||000000000000000000000000001 ||

|sb   $4, 255($0) |101000 |00000 |00100 |000000001111111 |

0 20030008  1 20040001  1 2005ffff  0 10600004  0 00852020  0 00852822  1 2063ffff  1 08000003  1 a00400ff


FIGURE 1.52  Machine language code for Fibonacci program


FIGURE 1.53  Multicycle MIPS microarchitecture. Adapted from [Patterson04] and [Harris07] with permission from Elsevier.


Imm


RD


Instr / Datam MemorydD


9A1


A3


WD3


RD2 RD1


WE3


A2


e


em9CLK


RegisteraD


Filea


PC 0 1


er


PCNext


内Instr25:21 20:16


7:0 5:0


SrcB


20:16


ALU


15:11


<<2


ALUResult


SrcA


白ALUOut


31:26


Branch


MemWrite


ALUSrcA RegWrite


Op


Funct


Control Unit


Zero


K之


ALUControl2:0


WD


√WE


RM


Adr


Data


aCLK


CLK白A


00 01


10 11


W


M


ALUSrcB1:0


IRWrite3:0 IorD


↓PCWrite


PCEn


PCSrc1:0


00 01 10


ImmX4


36


lines indicate busses. The control logic and signals are highlighted in blue while the datapath is shown in black. Control signals generally drive multiplexer select signals and register enables to tell the datapath how to execute an instruction.


Instruction execution generally ﬂows from left to right. The program counter (PC)speciﬁes the address of the instruction. The instruction is loaded 1 byte at a time over four cycles from an off-chip memory into the 32-bit instruction register (IR). The Op ﬁeld (bits 31:26 of the instruction) is sent to the controller, which sequences the datapath through the correct operations to execute the instruction. For example, in an ADD instruction, the two source registers are read from the register ﬁle into temporary registers A and B. On the next cycle, the aludec unit commands the Arithmetic/Logic Unit (ALU) to add the inputs. The result is captured in the ALUOut register. On the third cycle, the result is written back to the appropriate destination register in the register ﬁle.


The controller contains a ﬁnite state machine (FSM) that generates multiplexer select signals and register enables to sequence the datapath. A state transition diagram for the FSM is shown in Figure 1.54. As discussed, the ﬁrst four states fetch the instruction from


FIGURE 1.54  Multicycle MIPS control FSM (Adapted from [Patterson04] and [Harris07] with permission from Elsevier.)


Instruction decode/


register fetch


R-type completion


7


11


Reset


ALUSrcA = 0


IorD = 0


IRWrite0


ALUSrcB = 01 ALUOp = 00


PCWrite


PCSrc = 00


IRWrite1


IRWrite2


IRWrite3


ALUSrcA = 0 ALUSrcB = 11 ALUOp = 00


ALUSrcA = 1 ALUSrcB = 10 ALUOp = 00


ALUSrcA = 1 ALUSrcB = 00 ALUOp = 10


Instruction fetch


Memory address


computation


(Op = 'LB') or (Op = 'SB') 9


↑


(Op = R-type)


Execution


ALUSrcA = 1 ALUSrcB = 00 ALUOp = 01 Branch = 1 PCSrc = 01


PCWrite PCSrc = 10


'LB')(Op =


(Op = 'SB')


Branch completion


Jump


= 'J')(Opcompletion


Memory access


IorD = 1


MemWrite IorD = 1


RegDst = 1


RegWrite


MemtoReg = 0


Write-back step


RegDst = 0


MemtoReg = 1


1.7      Example: A Simple MIPS Microprocessor 37


memory. The FSM then is dispatched based on Op to execute the particular instruction.


The FSM states for ADDI are missing and left as an exercise for the reader.


Observe that the FSM produces a 2-bit ALUOp output. The ALU decoder unit in the controller uses combinational logic to compute a 3-bit ALUControl signal from the ALUOp and Funct ﬁelds, as speciﬁed in Table 1.8. ALUControl drives multiplexers in the ALU to select the appropriate computation.


|ALUOp |Funct |ALUControl |Meaning ||
|---|---|---|---|---|

|00 |x |010 |ADD ||

|01 |x |110 |SUB ||

|10 |100000 |010 |ADD ||

|10 |100010 |110 |SUB ||

|10 |100100 |000 |AND ||

|10 |100101 |001 |OR ||

|10 |101010 |111 |SLT ||

|11 |x |x |undeﬁned ||

Example 1.5


Referring to Figures 1.53 and 1.54, explain how the MIPS processor fetches and executes the SUB instruction.


SOLUTION: The ﬁrst step is to fetch the 32-bit instruction. This takes four cycles because the instruction must come over an 8-bit memory interface. On each cycle, we want to fetch a byte from the address in memory speciﬁed by the program counter, then increment the program counter by one to point to the next byte.


The fetch is performed by states 0–3 of the FSM in Figure 1.54. Let us start with state 0. The program counter (PC) contains the address of the ﬁrst byte of the instruction. The controller must select IorD = 0 so that the multiplexer sends this address to the memory. MemRead must also be asserted so the memory reads the byte onto the MemData bus. Finally, IRWrite0 should be asserted to enable writing memdata into the least signiﬁcant byte of the instruction register (IR).


Meanwhile, we need to increment the program counter. We can do this with the ALU by specifying PC as one input, 1 as the other input, and ADD as the operation. To select PC as the ﬁrst input, ALUSrcA = 0. To select 1 as the other input, ALUSrcB = 01.


To perform an addition, ALUOp = 00, according to Table 1.8. To write this result back into the program counter at the end of the cycle, PCSrc = 00 and PCEn = 1 (done by setting PCWrite = 1).


All of these control signals are indicated in state 0 of Figure 1.54. The other register enables are assumed to be 0 if not explicitly asserted and the other multiplexer selects are don’t cares. The next three states are identical except that they write bytes 1,2, and 3 of the IR, respectively.


The next step is to read the source registers, done in state 4. The two source registers are speciﬁed in bits 25:21 and 20:16 of the IR. The register ﬁle reads these registers and puts the values into the A and B registers. No control signals are necessary for SUB(although state 4 performs a branch address computation in case the instruction is BEQ). TABLE 1.8  ALUControl determination


38


The next step is to perform the subtraction. Based on the Op ﬁeld (IR bits 31:26),the FSM jumps to state 9 because SUB is an R-type instruction. The two source registers are selected as input to the ALU by setting ALUSrcA = 1 and ALUSrcB = 00.


Choosing ALUOp = 10 directs the ALU Control decoder to select the ALUControl signal as 110, subtraction. Other R-type instructions are executed identically except that the decoder receives a different Funct code (IR bits 5:0) and thus generates a different ALUControl signal. The result is placed in the ALUOut register.


Finally, the result must be written back to the register ﬁle in state 10. The data comes from the ALUOut register so MemtoReg = 0. The destination register is speci-ﬁed in bits 15:11 of the instruction so RegDst = 1. RegWrite must be asserted to perform the write. Then, the control FSM returns to state 0 to fetch the next instruction.


1.8 Logic Design


We begin the logic design by deﬁning the top-level chip interface and block diagram. We then hierarchically decompose the units until we reach leaf cells. We specify the logic with a Hardware Description Language (HDL), which provides a higher level of abstraction than schematics or layout. This code is often called the Register Transfer Level (RTL)description.


1.8.1 Top-Level Interfaces


The top-level inputs and outputs are listed in Table 1.9. This example uses a two-phase clocking system to avoid hold-time problems. Reset initializes the PC to 0 and the control FSM to the start state.


|Inputs |Outputs |
|---|---|

|ph1 |MemWrite |

|ph2 |Adr[7:0] |

|reset |WriteData[7:0] |

|MemData[7:0] ||

The remainder of the signals are used for an 8-bit memory interface (assuming the memory is located off chip). The processor sends an 8-bit address Adr and optionally asserts MemWrite. On a read cycle, the memory returns a value on the MemData lines while on a write cycle, the memory accepts input from WriteData. In many systems, MemData and WriteData can be combined onto a single bidirectional bus, but for this example we preserve the interface of Figure 1.53. Figure 1.55 shows a simple computer system built from the MIPS processor, external memory, reset switch, and clock generator.


1.8.2  Block Diagrams


The chip is partitioned into two top-level units: the controller and datapath, as shown in the block diagram in Figure 1.56. The controller comprises the control FSM, the ALU decoder, and the two gates used to compute PCEn. The ALU decoder consists of combinaTABLE 1.9  Top-level inputs and outputs


1.8      Logic Design 39


tional logic to determine ALUControl. The 8-bit datapath contains the remainder of the6chip. It can be viewed as a collection of wordslices or bitslices. A wordslice is a column containing an 8-bit ﬂip-ﬂop, adder, multiplexer, or other element. For example, Figure 1.57


shows a wordslice for an 8-bit 2:1 multiplexer. It contains eight individual 2:1 multiplexers, along with a zipper containing a buffer and inverter to drive the true and complementary select signals to all eight multiplexers.6 Factoring these drivers out into the zipper


一 saves space as compared to putting inverters in each multiplexer. Alternatively, the9 datapath can be viewed as eight rows of bitslices. Each bitslice has one bit of each component, along with the horizontal wires connecting the bits together.


The chip partitioning is inﬂuenced by the intended physical design. The datapath


contains most of the transistors and is very regular in structure. We can achieve high density with moderate design effort by handcrafting each wordslice or bitslice and tiling the


FIGURE 1.55  MIPS computer system


FIGURE 1.56  Top-level MIPS block diagram


→reset


ph1


ph2


crystal oscillator


MIPS


processor


Adr WriteData MemData


external memory


8 8 8


2-phase clock


generator


datapath controller


如加*加→*


op[5:0]zero


alusrcaalusrcb[1:0]pcen


pcsource[1:0]memtoregregdstiordregwriteirwrite[3:0]


funct[5:0]


alucontrol[2:0]


reset


memdata[7:0]


Jaddz


writedata[7:0]adr[7:0]


memwrite


aludec


aluop[1:0]


6In this example, the zipper is shown at the top of the wordslice. In wider datapaths, the zipper is sometimes placed in the middle of the wordslice so that it drives shorter wires. The name comes from the way the layout resembles a plaid sweatshirt with a zipper down the middle.


FIGURE 1.57  8-bit 2:1  multiplexer wordslice


D1[7]


山s 01sL--sel


D0[7]


D1[6]D0[6]


D1[0]D0[0]


Y[7]


Y[6]


Y[0]


circuits together. Building datapaths using wordslices is usually easier because certain structures, such as the zero detection circuit in the ALU, are not identical in each bitslice.


However, thinking about bitslices is a valuable way to plan the wiring across the datapath.


The controller has much less structure. It is tedious to translate an FSM into gates by hand, and in a new design, the controller is the most likely portion to have bugs and lastminute changes. Therefore, we will specify the controller more abstractly with a hardware description language and automatically generate it using synthesis and place & route tools or a programmable logic array (PLA).


1.8.3 Hierarchy


The best way to design complex systems is to decompose them into simpler pieces. Figure


1.58 shows part of the design hierarchy for the MIPS processor. The controller contains the controller_pla and aludec, which in turn is built from a library of standard cells such as NANDs, NORs, and inverters. The datapath is composed of 8-bit wordslices, each of which also is typically built from standard cells such as adders, register ﬁle bits, multiplexers, and ﬂip-ﬂops. Some of these cells are reused in multiple places.


The design hierarchy does not necessarily have to be identical in the logic, circuit, and physical designs. For example, in the logic view, a memory may be best treated as a black box, while in the circuit implementation, it may have a decoder, cell array, column multiplexers, and so forth. Different hierarchies complicate veriﬁcation, however, because they must be ﬂattened until the point that they agree. As a matter of practice, it is best to make logic, circuit, and physical design hierarchies agree as far as possible.


1.8.4 Hardware Description Languages


Designers need rapid feedback on whether a logic design is reasonable. Translating block diagrams and FSM state transition diagrams into circuit schematics is time-consuming and prone to error; before going through this entire process it is wise to know if the toplevel design has major bugs that will require complete redesign. HDLs provide a way to specify the design at a higher level of abstraction to raise designer productivity. They were originally intended for documentation and simulation, but are now used to synthesize gates directly from the HDL.


FIGURE 1.58  MIPS design hierarchy


mips


controller


datapath


alu


fulladder


nand2


nor2


inv


controller_pla


and2_8


adder_8


or2_8


regramarray


\


000


0 0 0


mux4_8


flop_8


a2o1


mux4


invbuf


and2 or2


flop


zerodetect


1.8      Logic Design 41


The two most popular HDLs are Verilog and VHDL. Verilog was developed by Advanced Integrated Design Systems (later renamed Gateway Design Automation) in 1984 and became a de facto industry open standard by 1991. In 2005, the SystemVerilog extensions were standardized, and some of these features are used in this book. VHDL,which stands for VHSIC Hardware Description Language, where VHSIC in turn was a Department of Defense project on Very High Speed Integrated Circuits, was developed by committee under government sponsorship. As one might expect from their pedigrees,Verilog is less verbose and closer in syntax to C, while VHDL supports some abstractions useful for large team projects. Many Silicon Valley companies use Verilog while defense and telecommunications companies often use VHDL. Neither language offers a decisive advantage over the other so the industry is saddled with supporting both. Appendix A offers side-by-side tutorials on Verilog and VHDL. Examples in this book are given in Verilog for the sake of brevity.


When coding in an HDL, it is important to remember that you are specifying hardware that operates in parallel rather than software that executes in sequence. There are two general coding styles. Structural HDL speciﬁes how a cell is composed of other cells or primitive gates and transistors. Behavioral HDL speciﬁes what a cell does.


A logic simulator simulates HDL code; it can report whether results match expectations, and can display waveforms to help debug discrepancies. A logic synthesis tool is similar to a compiler for hardware: it maps HDL code onto a library of gates called standard cells to minimize area while meeting some timing constraints. Only a subset of HDL constructs are synthesizable; this subset is emphasized in the appendix. For example, ﬁle I/O commands used in testbenches are obviously not synthesizable. Logic synthesis generally produces circuits that are neither as dense nor as fast as those handcrafted by a skilled designer. Nevertheless, integrated circuit processes are now so advanced that synthesized circuits are good enough for the great majority of application-speciﬁc integrated circuits(ASICs) built today. Layout may be automatically generated using place & route tools.


Verilog and VHDL models for the MIPS processor are listed in Appendix A.12. In Verilog, each cell is called a module. The inputs and outputs are declared much as in a C program and bit widths are given for busses. Internal signals must also be declared in a way analogous to local variables. The processor is described hierarchically using structural Verilog at the upper levels and behavioral Verilog for the leaf cells. For example, the controller module shows how a ﬁnite state machine is speciﬁed in behavioral Verilog and the aludec module shows how complex combinational logic is speciﬁed. The datapath is speciﬁed structurally in terms of wordslices, which are in turn described behaviorally.


For the sake of illustration, the 8-bit adder wordslice could be described structurally as a ripple carry adder composed of eight cascaded full adders.


The full adder could be expressed structurally as a sum and a


carry subcircuit. In turn, the sum and carry subcircuits could


be expressed behaviorally. The full adder block is shown in


Figure 1.59 while the carry subcircuit is explored further in


Section 1.9.


wire [6:0] carry;


FIGURE 1.59  Full adder


+c s


cout


carry


|module adder(input logic |[7:0] |a, b, |
|---|---|---|

|input  logic ||c, |

|output logic |[7:0] |s, |

|output logic ||cout); |

sum


s


a b c


42


fulladder fa0(a[0], b[0], c,        s[0], carry[0]);


fulladder fa1(a[1], b[1], carry[0], s[1], carry[1]);


fulladder fa2(a[2], b[2], carry[1], s[2], carry[2]);


...


fulladder fa7(a[7], b[7], carry[6], s[7], cout);


endmodule


module fulladder(input logic a, b, c,


output logic s, cout);


sum s1(a, b, c, s);


carry c1(a, b, c, cout);


module carry(input logic a, b, c,


output logic cout);


assign cout = (a&b) | (a&c) | (b&c); endmodule


1.9 Circuit Design


Circuit design is concerned with arranging transistors to perform a particular logic function. Given a circuit design, we can estimate the delay and power. The circuit can be represented as a schematic, or in textual form as a netlist. Common transistor level netlist formats include Verilog and SPICE. Verilog netlists are used for functional veriﬁcation,while SPICE netlists have more detail necessary for delay and power simulations.


Because a transistor gate is a good insulator, it can be modeled as a capacitor, C.


When the transistor is ON, some current I ﬂows between source and drain. Both the current and capacitance are proportional to the transistor width.


古


The delay of a logic gate is determined by the current that it can deliver and the capacitance that it is driving, as shown in Figure 1.60 for one inverter driving another inverter. The capacitance is charged or discharged according to the constitutive equation


If an average current I is applied, the time t to switch between 0 and VDD is


Hence, the delay increases with the load capacitance and decreases with the drive current.


To make these calculations, we will have to delve below the switch-level model of a transistor. Chapter 2 develops more detailed models of transistors accounting for the current and capacitance. One of the goals of circuit design is to choose transistor widths to meet delay requirements. Methods for doing so are discussed in Chapter 4.


I CdVdt


丁


=


tCIVDD=


FIGURE 1.60   Circuit delay  and power: (a) inverter pair,


(b) transistor-level model


showing capacitance and


current during switching, (c) static leakage current during  quiescent operation


X


I C


Istatic


1.9      Circuit Design 43


Energy is required to charge and discharge the load capacitance. This is called dynamic power because it is consumed when the circuit is actively switching. The dynamic power consumed when a capacitor is charged and discharged at a frequency f is


Even when the gate is not switching, it draws some static power. Because an OFF transistor is leaky, a small amount of current Istatic ﬂows between power and ground, resulting in a static power dissipation of


Chapter 5 examines power in more detail.


A particular logic function can be implemented in many ways.


Should the function be built with ANDs, ORs, NANDs, or NORs?


What should be the fan-in and fan-out of each gate? How wide should


the transistors be on each gate? Each of these choices inﬂuences the


capacitance and current and hence the speed and power of the circuit, as


well as the area and cost.


As mentioned earlier, in many design methodologies, logic synthesis tools automatically make these choices, searching through the standard cells for the best implementation. For many applications, synthesis


is good enough. When a system has critical requirements of high speed


or low power or will be manufactured in large enough volume to justify


the extra engineering, custom circuit design becomes important for critical portions of the chip.


Circuit designers often draw schematics at the transistor and/or gate


level. For example, Figure 1.61 shows two alternative circuit designs for


the carry circuit in a full adder. The gate-level design in Figure 1.61(a)


requires 26 transistors and four stages of gate delays (recall that ANDs


and ORs are built from NANDs and NORs followed by inverters). The


transistor-level design in Figure 1.61(b) requires only 12 transistors and


two stages of gate delays, illustrating the beneﬁts of optimizing circuit


designs to take advantage of CMOS technology.


These schematics are then netlisted for simulation and veriﬁcation.


One common netlist format is structural Verilog HDL. The gate-level design can be netlisted as follows:


logic x, y, z;


and g1(x, a, b);


and g2(y, a, c);


and g3(z, b, c);


or  g4(cout, x, y, z);


P


CV fDD


dynamic =


I VDD


static


FIGURE 1.61  Carry subcircuit


a b a c b c


y


z


g3


g4


c c


b a a b


cn


n1


n2


n3


n4 n5


n6 p6


p5 p4


p3


p2


p1


i1 i3


i2 i4


44


This is a technology-independent structural description, because generic gates have been used and the actual gate implementations have not been speciﬁed. The transistorlevel netlist follows:


output tri   cout);


tri   i1, i2, i3, i4, cn;


supply0 gnd;


supply1 vdd;


tranif1 n1(i1, gnd, a);


tranif1 n2(i1, gnd, b);


tranif1 n3(cn, i1, c);


tranif1 n4(i2, gnd, b);


tranif1 n5(cn, i2, a);


tranif0 p1(i3, vdd, a);


tranif0 p2(i3, vdd, b);


tranif0 p3(cn, i3, c);


tranif0 p4(i4, vdd, b);


tranif0 p5(cn, i4, a);


tranif1 n6(cout, gnd, cn);


tranif0 p6(cout, vdd, cn);


Transistors are expressed as


Transistor-type name(drain, source, gate);


tranif1 corresponds to nMOS transistors that turn ON when the gate is 1 while tranif0 corresponds to pMOS transistors that turn ON when the gate is 0. Appendix A.11 covers Verilog netlists in more detail.


With the description generated so far, we still do not have the information required to determine the speed or power consumption of the gate. We need to specify the size of the transistors and the stray capacitance. Because Verilog was designed as a switch-level and gate-level language, it is poorly suited to structural descriptions at this level of detail.


Hence, we turn to another common structural language used by the circuit simulator SPICE. The speciﬁcation of the transistor-level carry subcircuit at the circuit level might be represented as follows:


.SUBCKT CARRY A B C COUT VDD GND


MN1 I1 A GND GND NMOS W=2U L=0.6U AD=1.8P AS=3P


MN2 I1 B GND GND NMOS W=2U L=0.6U AD=1.8P AS=3P


MN3 CN C I1 GND NMOS W=2U L=0.6U AD=3P AS=3P


MN4 I2 B GND GND NMOS W=2U L=0.6U AD=0.9P AS=3P


MN5 CN A I2 GND NMOS W=2U L=0.6U AD=3P AS=0.9P


MP1 I3 A VDD VDD PMOS W=4U L=0.6U AD=3.6P AS=6P


MP2 I3 B VDD VDD PMOS W=4U L=0.6U AD=3.6P AS=6P


MP3 CN C I3 VDD PMOS W=4U L=0.6U AD=6P AS=6P


1.10      Physical Design 45


MP4 I4 B VDD VDD PMOS W=4U L=0.6U AD=1.8P AS=6P  MP5 CN A I4 VDD PMOS W=4U L=0.6U AD=6P AS=1.8P  MN6 COUT CN GND GND NMOS W=4U L=0.6U AD=6P AS=6P  MP6 COUT CN VDD VDD PMOS W=8U L=0.6U AD=12P AS=12P  CI1 I1 GND 6FF


CI3 I3 GND 9FF


CA A GND 12FF


CB B GND 12FF


CC C GND 6FF


CCN CN GND 12FF


CCOUT COUT GND 6FF


.ENDS


Transistors are speciﬁed by lines beginning with an M as follows:


Mname  drain   gate   source   body   type   W=width  L=length


AD=drain area   AS=source area


Although MOS switches have been masquerading as three terminal devices (gate,source, and drain) until this point, they are in fact four terminal devices with the substrate or well forming the body terminal. The body connection was not listed in Verilog but is required for SPICE. The type speciﬁes whether the transistor is a p-device or n-device.


The width, length, and area parameters specify physical dimensions of the actual transistors. Units include U (micro, 10–6), P (pico, 10–12), and F (femto, 10–15). Capacitors are speciﬁed by lines beginning with C as follows:


Cname   node1   node2   value


In this description, the MOS model in SPICE calculates the parasitic capacitances inherent in the MOS transistor using the device dimensions speciﬁed. The extra capacitance statements in the above description designate additional routing capacitance not inherent to the device structure. This depends on the physical design of the gate. Long wires also contribute resistance, which increases delay. At the circuit level of structural speciﬁcation,all connections are given that are necessary to fully characterize the carry gate in terms of speed, power, and connectivity. Chapter 8 describes SPICE models in more detail.


1.10 Physical Design


1.10.1 Floorplanning


Physical design begins with a ﬂoorplan. The ﬂoorplan estimates the area of major units in the chip and deﬁnes their relative placements. The ﬂoorplan is essential to determine whether a proposed design will ﬁt in the chip area budgeted and to estimate wiring lengths and wiring congestion. An initial ﬂoorplan should be prepared as soon as the logic is loosely deﬁned. As usual, this process involves feedback. The ﬂoorplan will often suggest changes to the logic (and microarchitecture), which in turn changes the ﬂoorplan. For example, suppose microarchitects assume that a cache requires a 2-cycle access latency. If the ﬂoorplan shows that the data cache can be placed adjacent to the execution units in the


46


datapath, the cache access time might reduce to a single cycle. This could allow the microarchitects to reduce the cache capacity while providing the same performance. Once the cache shrinks, the ﬂoorplan must be reconsidered to take advantage of the newly available space near the datapath. As a complex design begins to stabilize, the ﬂoorplan is often hierarchically subdivided to describe the functional blocks within the units.


The challenge of ﬂoorplanning is estimating the size of each unit without proceeding through a detailed design of the chip (which would depend on the ﬂoorplan and wire lengths). This section assumes that good estimates have been made and describes what aﬂoorplan looks like. The next sections describe each of the types of components that might be in a ﬂoorplan and suggests ways to estimate the component sizes.


Figure 1.62 shows the chip ﬂoorplan for the MIPS processor including the pad frame.


The top-level blocks are the controller and datapath. A wiring channel is located between the two blocks to provide room to route control signals to the datapath. The datapath is further partitioned into wordslices. The pad frame includes 40 I/O pads, which are wired to the pins on the chip package. There are 29 pads used for signals; the remainder are VDD and GND. The ﬂoorplan is drawn to scale and annotated with dimensions. The chip is designed in a 0.6 m process on a 1.5 × 1.5 mm die so the die is 5000  on a side. Each pad is 750 ×


FIGURE 1.62  MIPS ﬂoorplan


2550 λ


O I/10 pads


wiring channel: 25 tracks = 200λ


pads10 I/O


3500 λ


5000 λ


10 I/O pads 10 I/O pads


8 bitslices + 1 zipper row + 3 decoder rows = 12 rows x 110 λ / row = 1320 λ height


width determined from slice plan


height determined from


PLA size width matches  datapath


(4.8 Mλ2)


control


2550λ x 380λ(1.0 Mλ2)


5000λ


3500 h1900 λ


2550λ x 1320λ


(3.4 Mλ2)


1.10      Physical Design 47


350 , so the maximum possible core area inside the pad frame is 3500 × 3500 = 12.25 M 2. Due to the wiring channel, the actual core area of 4.8 M 2 is larger than the sum of the block areas. This design is said to be pad-limited because the I/O pads set the chip area.


Most commercial chips are core-limited because the chip area is set by the logic excluding the pads. In general, blocks in a ﬂoorplan should be rectangular because it is difﬁcult for a designer to stuff logic into an odd-shaped region (although some CAD tools do so just ﬁne).


Figure 1.63 shows the actual chip layout. Notice the 40 I/O pads around the periphery. Just inside the pad frame are metal2 VDD and GND rings, marked with + and –.


HMC


|||王 neon HARVEY MUDD COLLEGE NWLHWNI37D INOXN3人.08 OVALOO IVZ, DC|
|---|---|---|

onleHMC


OWH


FIGURE 1.63  MIPS layout


48


On-chip structures can be categorized as random logic, datapaths, arrays, analog, and input/output (I/O). Random logic, like the aludecoder, has little structure. Datapaths operate on multi-bit data words and perform roughly the same function on each bit so they consist of multiple N-bit wordslices. Arrays, like RAMs, ROMs, and PLAs, consist of identical cells repeated in two dimensions. Productivity is highest if layout can be reused or automatically generated. Datapaths and arrays are good VLSI building blocks because a single carefully crafted cell is reused in one or two dimensions. Automatic layout generators exist for memory arrays and random logic but are not as mature for datapaths. Therefore, many design methodologies ignore the potential structure of datapaths and instead lay them out with random logic tools except when performance or area are vital. Analog circuits still require careful design and simulation but tend to involve only small amounts of layout because they have relatively few transistors. I/O cells are also highly tuned to each fabrication process and are often supplied by the process vendor.


Random logic and datapaths are typically built from standard cells such as inverters,NAND gates, and ﬂip-ﬂops. Standard cells increase productivity because each cell only needs to be drawn and veriﬁed once. Often, a standard cell library is purchased from a third party vendor.


Another important decision during ﬂoorplanning is to choose the metal orientation.


The MIPS ﬂoorplan uses horizontal metal1 wires, vertical metal2 wires, and horizontal metal3 wires. Alternating directions between each layer makes it easy to cross wires on different layers.


1.10.2 Standard Cells


A simple standard cell library is shown on the inside front cover. Power and ground run horizontally in metal1. These supply rails are 8  wide (to carry more current) and are separated by 90  center-to-center. The nMOS transistors are placed in the bottom 40  of the cell and the pMOS transistors are placed in the top 50 . Thus, cells can be connected by abutment with the supply rails and n-well matching up. Substrate and well contacts are placed under the supply rails. Inputs and outputs are provided in metal2, which runs vertically. Each cell is a multiple of 8  in width so that it offers an integer number of metal2 tracks. Within the cell, poly is run vertically to form gates and diffusion and metal1 are run horizontally, though metal1 can also be run vertically to save space when it does not interfere with other connections.


Cells are tiled in rows. Each row is separated vertically by at least 110  from the base of the previous row. In a 2-level metal process, horizontal metal1 wires are placed in routing channels between the rows. The number of wires that must be routed sets the height of the routing channels. Layout is often generated with automatic place & route tools. Figure


1.64 shows the controller layout generated by such a tool. Note that in this and subsequent layouts, the n-well around the pMOS transistors will usually not be shown.


When more layers of metal are available, routing takes place over the cells and routing channels may become unnecessary. For example, in a 3-level metal process, metal3 is run horizontally on a 10  pitch. Thus, 11 horizontal tracks can run over each cell. If this is sufﬁcient to accommodate all of the horizontal wires, the routing channels can be eliminated.


Automatic synthesis and place & route tools have become good enough to map entire designs onto standard cells. Figure 1.65 shows the entire 8-bit MIPS processor synthesized from the VHDL model given in Appendix A.12 onto a cell library in a 130 nm process with


1.10      Physical Design 49


seven metal layers. Compared to Figure 1.63, the synthesized design shows little discernible structure except that 26 rows of standard cells can be identiﬁed beneath the wires. The area is approximately 4 M 2. Synthesized designs tend to be somewhat slower than a good custom design, but they also take an order of magnitude less design effort.


FIGURE 1.64  MIPS controller layout (synthesized)


FIGURE 1.65  Synthesized MIPS processor


a 1


(


p


!


o


u


)


n


|


l


'


-88


"


50


1.10.3 Pitch Matching


|A |A |A |A |B |
|---|---|---|---|---|

|A |A |A |A |B |

|C C |C C |C C |C C |D |

The area of the controller in Figure 1.64 is dominated by the routing channels. When the logic is more regular, layout density can be improved by including the wires in cells that“snap together.” Snap-together cells require more design and layout effort but lead to smaller area and shorter (i.e., faster) wires. The key issue in designing snap-together cells is pitch-matching. Cells that connect must have the same size along the connecting edge.


Figure 1.66 shows several pitch-matched cells. Reducing the size of cell D does not help the layout area. On the other hand, increasing the size of cell D also affects the area of B and/or C.


Figure 1.67 shows the MIPS datapath in more detail. The eight horizontal bitslices are clearly visible. The zipper at the top of the layout includes three rows for the decoder that is pitch-matched to the register ﬁle in the datapath. Vertical metal2 wires are used for control, including clocks, multiplexer selects, and register enables. Horizontal metal3 wires run over the tops of cells to carry data along a bitslice.


The width of the transistors in the cells and the number of wires that must run over the datapath determines the minimum height of the datapath cells. 60–100  are typical heights for relatively simple datapaths. The width of the cell depends on the cell contents.


1.10.4 Slice Plans


Figure 1.68 shows a slice plan of the datapath. The diagram illustrates the ordering of wordslices and the allocation of wiring tracks within each bitslice. Dots indicate that a bus passes over a cell and is also used in that cell. Each cell is annotated with its type and width (in number of tracks). For example, the program counter (pc) is an output of the PC ﬂop and is also used as an input to the srcA and address multiplexers. The slice plan


Vddgnd


||Zipper|Zipper|Zipper|
|---|---|---|---|

|||Bitslice 7||

|||Bitslice 0||

|||flop mux adder|flop mux adder|

Register File Decoder


vdd gnd


wordslice


FIGURE 1.67  MIPS datapath layout  1


FIGURE 1.66  Pitch-matching


of snap-together cells


1.10      Physical Design 51


makes it easy to calculate wire lengths and evaluate wiring congestion before laying out the datapath. In this case, it is evident that the greatest congestion takes place over the registerﬁle, where seven wiring tracks are required.


The slice plan is also critical for estimating area of datapaths. Each wordslice is annotated with its width, measured in tracks. This information can be obtained by looking at the cell library layouts. By adding up the widths of each element in the slice plan, we see that the datapath is 319 tracks wide, or 2552  wide. There are eight bitslices in the 8-bit datapath.


In addition, there is one more row for the zipper and three more for the three register ﬁle address decoders, giving a total of 12 rows. At a pitch of 110 / row, the datapath is 1320  tall. The address decoders only occupy a small fraction of their rows, leaving wasted empty space. In a denser design, the controller could share some of the unused area.


1.10.5 Arrays


Figure 1.69 shows a programmable logic array (PLA) used for the control FSM next state and output logic. A PLA can compute any function expressed in sum of products form.


The structure on the left is called the AND plane and the structure on the right is the OR plane. PLAs are discussed further in Section 12.7.


This PLA layout uses 2 vertical tracks for each input and 3 for each output plus about 6 for overhead. It uses 1.5 horizontal tracks for each product or minterm, plus about 14 for overhead. Hence, the size of a PLA is easy to calculate. The total PLA area is 500 × 350, plus another 336  × 220  for the four external ﬂip-ﬂops needed in the control FSM.


The height of the controller is dictated by the height of the PLA plus a few wiring tracks to route inputs and outputs. In comparison, the synthesized controller from Figure 1.64 has a size of 1500 × 400  because the wiring tracks waste so much space.


1.10.6 Area Estimation


A good ﬂoorplan depends on reasonable area estimates, which may be difﬁcult to make before logic is ﬁnalized. An experienced designer may be able to estimate block area by


FIGURE 1.68  Datapath slice plan


register file


'm


Re


ramslices


a d


IR3...0Mw


srcB srcA


m


u X


aluoutPC


6 17


17


13 6 9


9 9 9 9 13


13


mux2flopen(wiring)flopen


(wiring)flopen(wiring)flopen


(wiring)flopmux2regram0regramregramregramregramregramwe.6a1we.6e.p0mux4doymux2flopmux3opfl


zerodetectinvmux2and2or2fulladdermux4 4 4 16


9 9 9


op[6:0]


funct[6:0]


register adrs


|memdata |ata||||||||||||||||||||srcA ||||||||
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

|writedata |ata||||||||||||||||||srcB |3|||||||||

|adr ||||||||||im|ned|immediate |||||||aluout |out|||||||||

|||||||||||im|ned|immediate |||||||aluout |out|||||||||

||||||||||||||||||rd2|||out|||||||||

rd2


52


OR PLANE


AND PLANE


t


*te


comparison to the area of a comparable block drawn in the past. In the absence of data for such comparison, Table 1.10 lists some typical numbers. Be certain to account for large wiring channels at a pitch of 8  / track. Larger transistors clearly occupy a greater area, so this may be factored into the area estimates as a function of W and L (width and length).


For memories, don’t forget about the decoders and other periphery circuits, which often take as much area as the memory bits themselves. Your mileage may vary, but datapaths and arrays typically achieve higher densities than standard cells.


Given enough time, it is nearly always possible to shave a few lambda here or there from a design. However, such efforts are seldom a good investment unless an element is repeated so often that it accounts for a major fraction of the chip area or if ﬂoorplan errors have led to too little space for a block and the block must be shrunk before the chip can be completed. It is wise to make conservative area estimates in ﬂoorplans, especially if there is risk that more functionality may be added to a block.


非非非非非非非非非非非非


INPUTS


OUTPUTS


FIGURE 1.69  PLA for control FSM


TABLE 1.10  Typical layout densities


|Element |Area |
|---|---|

|random logic (2-level metal process) |1000 – 1500 2 / transistor |

|datapath |250 – 750 2 / transistor or 6 WL + 360 2 / transistor |

|SRAM |1000 2 / bit |

|DRAM (in a DRAM process) |100 2 / bit |

|ROM |100 2 / bit |

1.11      Design Verification 53


Some cell library vendors specify typical routed standard cell layout densities in kgates / mm2.7 Commonly, a gate is deﬁned as a 3-input static CMOS NAND or NOR with six transistors. A 65 nm process ( 0.03 m) with eight metal layers may achieve a density of 160–500 kgates / mm2 for random logic. This corresponds to about 370–1160 2 / transistor. Processes with many metal layers obtain high density because routing channels are not needed.


1.11 Design Veriﬁcation


Integrated circuits are complicated enough that if anything can go wrong, it probably will.


Design veriﬁcation is essential to catching the errors before manufacturing and commonly accounts for half or more of the effort devoted to a chip.


As design representations become more detailed, veriﬁcation time increases. It is not practical to simulate an entire chip in a circuit-level simulator such as SPICE for a large number of cycles to prove that the layout is correct. Instead, the design is usually tested for functionality at the architectural level with a model in  a language such


as C and at the logic level by simulating the HDL description. Then,


the circuits are checked to ensure that they are a faithful representation


of the logic and the layout is checked to ensure it is a faithful representation of the circuits, as shown in Figure 1.70. Circuits and layout must


meet timing and power speciﬁcations as well.


A testbench is used to verify that the logic is correct. The testbench


instantiates the logic under test. It reads a ﬁle of inputs and expected


outputs called test vectors, applies them to the module under test, and


logs mismatches. Appendix A.12 provides an example of a testbench for


verifying the MIPS processor logic.


A number of techniques are available for circuit veriﬁcation. If the


logic is synthesized onto a cell library, the postsynthesis gate-level


netlist can be expressed in an HDL again and simulated using the same


test vectors. Alternatively, a transistor-level netlist can be simulated


against the test vector, although this can result in tricky race conditions


for sequential circuits. Powerful formal veriﬁcation tools are also available to check that a circuit performs the same Boolean function as the


associated logic. Exotic circuits should be simulated thoroughly to


ensure that they perform the intended logic function and have adequate


noise margins; circuit pitfalls are discussed throughout this book.


Layout vs. Schematic tools (LVS) check that transistors in a layout


are connected in the same way as in the circuit schematic. Design rule


checkers (DRC) verify that the layout satisﬁes design rules. Electrical rule


checkers (ERC) scan for other potential problems such as noise or premature wearout; such problems will also be discussed later in the book.


FIGURE 1.70  Design and veriﬁcation sequence


Specification


Architecture


Design


Logic


Circuit


Physical


Function


Function Timing Power


71 kgate = 1000 gates.


54


1.12 Fabrication, Packaging, and Testing


Once a chip design is complete, it is taped out for manufacturing. Tapeout gets its name from the old practice of writing a speciﬁcation of masks to magnetic tape; today, the mask descriptions are usually sent to the manufacturer electronically. Two common formats for mask descriptions are the Caltech Interchange Format (CIF) [Mead80] (mainly used in academia) and the Calma GDS II Stream Format (GDS) [Calma84] (used in industry). Masks are made by etching a pattern of chrome on glass with an electron beam. A set of masks for a nanometer process can be very expensive. For example, masks for a large chip in a 180 nm process may cost on the order of a quarter of a million dollars. In a 65 nm process, the mask set costs about $3 million. The MOSIS service in the United States and its EUROPRACTICE and VDEC counterparts in Europe and Japan make a single set of masks covering multiple small designs from academia and industry to amortize the cost across many customers. With a university discount, the cost for a run of 40 small chips on a multi-project wafer can run about $10,000 in a 130 nm process down to $2000 in a


0.6 m process. MOSIS offers certain grants to cover fabrication of class project chips.


Integrated circuit fabrication plants (fabs) now cost billions of dollars and become obsolete in a few years. Some large companies still own their own fabs, but an increasing number of fabless semiconductor companies contract out manufacturing to foundries such as TSMC, UMC,  and IBM.


Multiple chips are manufactured simultaneously on a single silicon wafer, typically 150-300 mm (6"-12") in diameter. Fabrication requires many deposition, masking,etch-150–300 mm (6–12) in diameter. Fabrication requires many deposition, masking, etching, and implant steps. Most fabrication plants are optimized for wafer throughput rather than latency, leading to turnaround times of up to 10 weeks. Figure 1.71 shows an engineer in a clean room holding a completed 300 mm wafer. Clean rooms are ﬁltered to eliminate most dust and other particles that could damage a partially processed wafer. The engineer is wearing a “bunny suit” to avoid contaminating the clean room. Figure 1.72 is a


HAAVEY SUDD COLLEOE


HATHAHIEL PINCIHEY U


CHD DLLE US


14-144也trad -0.1mm


FIGURE 1.71  Engineer holding processed


12-inch wafer (Photograph courtesy of the Intel  Corporation.)


FIGURE 1.72  MIPS processor photomicrograph (only part of pad frame shown)


Summary and a Look Ahead 55


photomicrograph (a photograph taken under a microscope) of the 8-bit MIPS processor.


Processed wafers are sliced into dice (chips) and packaged. Figure 1.73 shows the 1.5 ×


1.5 mm chip in a 40-pin dual-inline package (DIP). This wire-bonded package uses thin gold wires to connect the pads on the die to the lead frame in the center cavity of the package.


These wires are visible on the pads in Figure 1.72. More advanced packages offer different trade-offs between cost, pin count, pin bandwidth, power handling, and reliability, as will be discussed in Section 13.2. Flip-chip technology places small solder balls directly onto the die, eliminating the bond wire inductance and allowing contacts over the entire chip area rather than just at the periphery.


Even tiny defects in a wafer or dust particles can cause a chip to fail. Chips are tested before being sold. Testers capable of handling high-speed chips cost millions of dollars, so many chips use built-in self-test features to reduce the tester time required. Chapter 15 is devoted to design veriﬁcation and testing.


Summary and a Look Ahead


“If the automobile had followed the same development cycle as the computer, a RollsRoyce would today cost $100, get one million miles to the gallon, and explode once a  year . . .”


—Robert X. Cringely


CMOS technology, driven by Moore’s Law, has come to dominate the semiconductor industry. This chapter examined the principles of designing a simple CMOS integrated circuit. MOS transistors can be viewed as electrically controlled switches. Static CMOS gates are built from pull-down networks of nMOS transistors and pull-up networks of pMOS transistors. Transistors and wires are fabricated on silicon wafers using a series of deposition, lithography, and etch steps. These steps are deﬁned by a set of masks drawn as a chip layout. Design rules specify minimum width and spacing between elements in the layout. The chip design process can be divided into architecture, logic, circuit, and physical design. The performance, area, and power of the chip are inﬂuenced by interrelated decisions made at each level. Design veriﬁcation plays an important role in constructing such complex systems; the reliability requirements for hardware are much greater than those typically imposed on software.


Primary design objectives include reliability, performance, power, and cost. Any chip should, with high probability, operate reliably for its intended lifetime. For example, the chip must be designed so that it does not overheat or break down from excessive voltage.


Performance is inﬂuenced by many factors including clock speed and parallelism. CMOS transistors dissipate power every time they switch, so the dynamic power consumption is related to the number and size of transistors and the rate at which they switch. At feature


FIGURE 1.73  Chip in a 40-pin dual-inline package


56


sizes below 180 nm, transistors also leak a signiﬁcant amount of current even when they should be OFF. Thus, chips now draw static power even when they are idle. One of the central challenges of VLSI design is making good trade-offs between performance and power for a particular application. The cost of a chip includes nonrecurring engineering(NRE) expenses for the design and masks, along with per-chip manufacturing costs related to the size of the chip. In processes with smaller feature sizes, the per-unit cost goes down because more transistors can be packed into a given area, but the NRE increases. The latest manufacturing processes are only cost-effective for chips that will sell in huge volumes. Nevertheless, plenty of interesting markets exist for chips in mature,inexpensive manufacturing processes.


To quantify how a chip meets these objectives, we must develop and analyze more complete models. The remainder of this book will expand on the material introduced in this chapter. Of course, transistors are not simply switches. Chapter 2 examines the current and capacitance of transistors, which are essential for estimating delay and power. A more detailed description of CMOS processing technology and layout rules is presented in Chapter 3. The next four chapters address the fundamental concerns of circuit designers. The models from Chapter 2 are too detailed to apply by hand to large systems, yet not detailed enough to fully capture the complexity of modern transistors. Chapter 4 develops simpliﬁed models to estimate the delay of circuits. If modern chips were designed to squeeze out the ultimate possible performance without regard to power, they would burn up. Thus, it is essential to estimate and trade off the power consumption against performance. Moreover, low power consumption is crucial to mobile battery-operated systems.


Power is considered in Chapter 5. Wires are as important as transistors in their contribution to overall performance and power, and are discussed in Chapter 6. Chapter 7 addresses design of robust circuits with a high yield and low failure rate.


Simulation is discussed in Chapter 8 and is used to obtain more accurate performance and power predictions as well as to verify the correctness of circuits and logic. Chapter 9 considers combinational circuit design. A whole kit of circuit families are available with different trade-offs in speed, power, complexity, and robustness. Chapter 10 continues with sequential circuit design, including clocking and latching techniques.


The next three chapters delve into CMOS subsystems. Chapter 11 catalogs designs for a host of datapath subsystems including adders, shifters, multipliers, and counters.


Chapter 12 similarly describes memory subsystems including SRAMs, DRAMs, CAMs,ROMs, and PLAs. Chapter 13 addresses special-purpose subsystems including power distribution, clocking, and I/O.


The ﬁnal chapters address practicalities of CMOS system design. Chapter 14 focuses on a range of current design methods, identifying the issues peculiar to CMOS. Testing,design-for-test, and debugging techniques are discussed in Chapter 15. Hardware description languages (HDLs) are used in the design of nearly all digital integrated circuits today. Appendix A provides side-by-side tutorials for Verilog and VHDL, the two dominant HDLs.


A number of sections are marked with an “optional” icon. These sections describe particular subjects in greater detail. You may skip over these sections on a ﬁrst reading and return to them when they are of practical relevance. To keep the length of this book under control, some optional topics have been published on the Internet rather than in print.


These sections can be found at www.cmosvlsi.com and are labeled with a “Web Enhanced” icon. A companion text, Digital VLSI Chip Design with Cadence and Synopsys CAD Tools [Brunvand09], covers practical details of using the leading industrial CAD tools to build chips.


Exercises 57


Exercises


1.1 Extrapolating the data from Figure 1.4, predict the transistor count of a microprocessor in 2016.


1.2 Search the Web for transistor counts of Intel’s more recent microprocessors. Make a  graph of transistor count vs. year of introduction from the Pentium Processor in


1993 to the present on a semilogarithmic scale. How many months pass between


doubling of transistor counts?


1.3 As the cost of a transistor drops from a microbuck ($10-6) toward a nanobuck, what  opportunities can you imagine to change the world with integrated circuits?


1.4 Read a biography or history about a major event in the development of integrated  circuits. For example, see Crystal Fire by Lillian Hoddesonor, Microchip by Jeffrey  Zygmont, or The Pentium Chronicles by Robert Colwell. Pick a team or individual  that made a major contribution to the ﬁeld. In your opinion, what were the characteristics that led to success? What traits of the team management would you seek to  emulate or avoid in your own professional life?


1.5 Sketch a transistor-level schematic for a CMOS 4-input NOR gate.


1.6 Sketch a transistor-level schematic for a compound CMOS logic gate for each of  the following functions:


a) Y = ABC + D


b) Y = (AB + C) · D


c) Y = AB + C · (A + B)


1.7 Use a combination of CMOS gates (represented by their symbols) to generate the  following functions from A, B, and C.


a) Y = A (buffer)


b) Y = AB + AB (XOR)


c) Y = A B+ AB (XNOR)


d) Y = AB + BC + AC (majority)


1.8 Sketch a transistor-level schematic of a CMOS 3-input XOR gate. You may assume  you have both true and complementary versions of the inputs available.


1.9 Sketch transistor-level schematics for the following logic functions. You may assume  you have both true and complementary versions of the inputs available.


a) A 2:4 decoder deﬁned by


Y0 = A0 · A1


Y1 = A0 · A1


Y2 = A0 · A1


Y3 = A0 · A1


b) A 3:2 priority encoder deﬁned by


Y0 = A0 · (A1 + A2)


58


1.10 Sketch a stick diagram for a CMOS 4-input NOR gate from Exercise 1.5.


1.11 Estimate the area of your 4-input NOR gate from Exercise 1.10.


1.12 Using a CAD tool of your choice, layout a 4-input NOR gate. How does its size


compare to the prediction from Exercise 1.11?


1.13 Figure 1.74 shows a stick diagram of a 2-input NAND gate. Sketch a side view


(cross-section) of the gate from X to X .


1.14 Figure 1.75 gives a stick diagram for a level-sensitive latch. Estimate the area of the  latch.


1.15 Draw a transistor-level schematic for the latch of Figure 1.75. How does the schematic differ from Figure 1.31(b)?


1.16 Consider the design of a CMOS compound OR-AND-INVERT (OAI21) gate


computing F = (A + B) · C.


a) sketch a transistor-level schematic


b) sketch a stick diagram


c) estimate the area from the stick diagram


d) layout your gate with a CAD tool using unit-sized transistors


e) compare the layout size to the estimated area


FIGURE 1.74  2-input NAND gate stick diagram


X'


FIGURE 1.75  Level-sensitive latch stick diagram


Exercises 59


1.17 Consider the design of a CMOS compound OR-OR-AND-INVERT (OAI22)


gate computing F = (A + B) · (C + D).


1.18 A 3-input majority gate returns a true output if at least two of the inputs are true. A  minority gate is its complement. Design a 3-input CMOS minority gate using a


single stage of logic.


1.19 Design a 3-input minority gate using CMOS NANDs, NORs, and inverters. How  many transistors are required? How does this compare to a design from Exercise


1.18(a)?


1.20 A carry lookahead adder computes G = G3 + P3(G2 + P2(G1 + P1G0)). Consider


designing a compound gate to compute G.


1.21 www.cmosvlsi.com has a series of four labs in which you can learn VLSI design  by completing the multicycle MIPS processor described in this chapter. The labs use  the open-source Electric CAD tool or commercial tools from Cadence and Synopsys. They cover the following:


a) leaf cells: schematic entry, layout, icons, simulation, DRC, ERC, LVS;


hierarchical design


b) datapath design: wordslices, ALU assembly, datapath routing


c) control design: random logic or PLAs


d) chip assembly, pad frame, global routing, full-chip veriﬁcation, tapeout


61


MOS Transistor Theory


2.1  Introduction


In Chapter 1, the Metal-Oxide-Semiconductor (MOS) transistor was introduced in terms


of its operation as an ideal switch. As we saw in Section 1.9, the performance and power ofH[


a chip depend on the current and capacitance of the transistors and wires. In this chapter,


we will examine the characteristics of MOS transistors in more detail; Chapter 6 addresses-EGwires.


Figure 2.1 shows some of the symbols that are commonly used for MOS transistors.


The three-terminal symbols in Figure 2.1(a) are used in the great majority of schematics.


If the body (substrate or well) connection needs to be shown, the four-terminal symbols in


Figure 2.1(b) will be used. Figure 2.1(c) shows an example of other symbols that may be


encountered in the literature.


The MOS transistor is a majority-carrier device in which the current in a conducting


channel between the source and drain is controlled by a voltage applied to the gate. In an


nMOS transistor, the majority carriers are electrons; in a pMOS transistor, the majority


carriers are holes. The behavior of MOS transistors can be understood by ﬁrst examining


an isolated MOS structure with a gate and body but no source or drain. Figure 2.2 shows


a simple MOS structure. The top layer of the structure is a good conductor called the gate.


Early transistors used metal gates. Transistor gates soon changed to use polysilicon, i.e.,


silicon formed from many small crystals, although metal gates are making a resurgence at


65 nm and beyond, as will be seen in Section 3.4.1.3. The middle layer is a very thin insulating ﬁlm of SiO2 called the gate oxide. The bottom layer is the doped silicon body. The


ﬁgure shows a p-type body in which the carriers are holes. The body is grounded and a


voltage is applied to the gate. The gate oxide is a good insulator so almost zero current


ﬂows from the gate to the body.1


In Figure 2.2(a) , a negative voltage is applied to the gate, so there is negative charge


on the gate. The mobile positively charged holes are attracted to the region beneath the


gate. This is called the accumulation mode. In Figure 2.2(b), a small positive voltage is


applied to the gate, resulting in some positive charge on the gate. The holes in the body are


repelled from the region directly beneath the gate, resulting in a depletion region forming


below the gate. In Figure 2.2(c), a higher positive potential exceeding a critical threshold


voltage Vt is applied, attracting more positive charge to the gate. The holes are repelled further and some free electrons in the body are attracted to the region beneath the gate. This


conductive layer of electrons in the p-type body is called the inversion layer. The threshold


1Gate oxides are now only a handful of atomic layers thick and carriers sometimes tunnel through the oxide,


creating a current through the gate. This effect is explored in Section 2.4.4.2.


FIGURE 2.1


MOS transistor symbols


Chapter 2      MOS Transistor Theory


62


voltage depends on the number of dopants in the body and the thickness tox of the oxide. It is usually positive, as shown in this example, but can be engineered to be negative.


Figure 2.3 shows an nMOS transistor. The transistor consists of the MOS stack between two n-type regions called the source and drain. In Figure 2.3(a), the gate-to-source voltage Vgs is less than the threshold voltage. The source and drain have free electrons. The body has free holes but no free electrons. Suppose the source is grounded. The junctions between the body and the source or drain are zero-biased or reverse-biased, so little or no current ﬂows. We say the transistor is OFF, and this mode of operation is called cutoff. It is often convenient to approximate the current through an OFF transistor as zero, especially in comparison to the current through an ON transistor. Remember, however, that small amounts of current leaking through OFF transistors can become signiﬁcant, especially when multiplied by millions or billions of transistors on a chip. In Figure 2.3(b), the gate voltage is greater than the threshold voltage. Now an inversion region of electrons (majority carriers)called the channel connects the source and drain, creating a conductive path and turning the transistor ON. The number of carriers and the conductivity increases with the gate voltage.


The potential difference between drain and source is Vds = Vgs  Vgd . If Vds = 0 (i.e., Vgs = Vgd),there is no electric ﬁeld tending to push current from drain to source.


When a small positive potential Vds is applied to the drain (Figure 2.3(c)), current Idsﬂows through the channel from drain to source.2 This mode of operation is termed linear,


FIGURE 2.2  MOS structure demonstrating (a) accumulation, (b) depletion, and


(c) inversion


2The terminology of source and drain might initially seem backward. Recall that the current in an nMOS transistor is carried by moving electrons with a negative charge. Therefore, positive current from drain to source corresponds to electrons ﬂowing from their source to their drain.


Polysilicon Gate


p-type Body


+–


Vg < 0


0 < Vg < Vt


Vg > Vt


Depletion Region


Inversion Region


Silicon Dioxide Insulator


2.1      Introduction 63


resistive, triode, nonsaturated, or unsaturated; the current increases with both the drain voltage and gate voltage. If Vds becomes sufﬁciently large that Vgd < Vt , the channel is no longer inverted near the drain and becomes pinched off (Figure 2.3(d)). However, conduction is still brought about by the drift of electrons under the inﬂuence of the positive drain voltage. As electrons reach the end of the channel, they are injected into the depletion region near the drain and accelerated toward the drain. Above this drain voltage the current Ids is controlled only by the gate voltage and ceases to be inﬂuenced by the drain. This mode is called saturation.


FIGURE 2.3  nMOS transistor demonstrating cutoff, linear, and saturation regions of operation


Vgs = 0


Vgd


Vgs > Vt


田n+


Vgd = Vgs


eee9


Vgs > Vgd > Vt


Vgd < Vt


田


Vds = 0


④


0 < Vds < Vgs – Vt


Vds > Vgs – Vt


p-type body p-type body


田田日+田田


田田田田④


b g


b个


b↓


Cutoff:


No Channel Ids = 0


Linear:


Channel Formed


Ids Increases with Vds


eeee


Saturation:


Channel Pinched Off Ids Independent of Vds


Ids Ids


64


In summary, the nMOS transistor has three modes of operation. If Vgs < Vt , the transistor is cutoff (OFF). If Vgs > Vt , the transistor turns ON. If Vds is small, the transistor acts as a linear resistor in which the current ﬂow is proportional to Vds. If Vgs > Vt and Vds is large, the transistor acts as a current source in which the current ﬂow becomes independent of Vds .


The pMOS transistor in Figure 2.4 operates in just the opposite fashion.


The n-type body is tied to a high potential so the junctions with the p-type source and drain are normally reverse-biased. When the gate is also at a high potential, no current ﬂows between drain and source. When the gate voltage is lowered by a threshold Vt , holes are attracted to form a p-type channel immediately beneath the gate, allowing current to ﬂow between drain and source.


The threshold voltages of the two types of transistors are not necessarily equal, so we use the terms Vtn and Vtp to distinguish the nMOS and pMOS thresholds.


Although MOS transistors are symmetrical, by convention we say that majority carriers ﬂow from their source to their drain. Because electrons are negatively charged, the source of an nMOS transistor is the more negative of the two terminals. Holes are positively charged so the source of a pMOS transistor is the more positive of the two terminals. In static CMOS gates, the source is the terminal closer to the supply rail and the drain is the terminal closer to the output.


We begin in Section 2.2 by deriving an ideal model relating current and voltage (I-V)for a transistor. The delay of MOS circuits is determined by the time required for this current to charge or discharge the capacitance of the circuits. Section 2.3 investigates transisr


tor capacitances. The gate of an MOS transistor is inherently a good capacitor with a thin dielectric; indeed, its capacitance is responsible for attracting carriers to the channel and thus for the operation of the device. The p–n junctions from source or drain to the body contribute additional parasitic capacitance. The capacitance of wires interconnecting the transistors is also important and will be explored in Section 6.2.2.


This idealized I-V model provides a general qualitative understanding of transistor behavior but is of limited quantitative value. On the one hand, it neglects too many effects that are important in transistors with short channel lengths L. Therefore, the model is not sufﬁcient to calculate current accurately. Circuit simulators based on SPICE [Nagel75]use models such as BSIM that capture transistor behavior quite thoroughly but require entire books to fully describe [Cheng99]. Chapter 8 discusses simulation with SPICE.


The most important effects seen in these simulations that impact digital circuit designers are examined in Section 2.4. On the other hand, the idealized I-V model is still too complicated to use in back-of-the-envelope calculations tuning the performance of large circuits. Therefore, we will develop even simpler models for performance estimation in Chapter 4.


Section 2.5 wraps up this chapter by applying the I-V models to understand the DC transfer characteristics of CMOS gates and pass transistors.


2.2 Long-Channel I-V Characteristics


As stated previously, MOS transistors have three regions of operation:


Cutoff or subthreshold regionCutoff or subthreshold region


Linear regionLinear region


Saturation regionSaturation region


FIGURE 2.4  pMOS transistor


立


n-type Body立


Gate


Body (usually VDD)


2.2      Long-Channel I-V Characteristics 65


Let us derive a model [Shockley52, Cobbold70, Sah64] relating the current and voltage (I-V) for an nMOS transistor in each of these regions. The model assumes that the channel length is long enough that the lateral electric ﬁeld (the ﬁeld between source and drain) is relatively low, which is no longer the case in nanometer devices. This model is variously known as the long-channel, ideal, ﬁrst-order, or Shockley model. Subsequent sections will reﬁne the model to reﬂect high ﬁelds, leakage, and other nonidealities.


The long-channel model assumes that the current through an OFF transistor is 0.


When a transistor turns ON (Vgs > Vt), the gate attracts carriers (electrons) to form a channel. The electrons drift from source to drain at a rate proportional to the


electric ﬁeld between these regions. Thus, we can compute currents if we


know the amount of charge in the channel and the rate at which it moves.


We know that the charge on each plate of a capacitor is Q = CV. Thus, the


charge in the channel Qchannel is


(2.1)


where Cg is the capacitance of the gate to the channel and Vgc Vt is the amount of voltage attracting charge to the channel beyond the minimum


required to invert from p to n. The gate voltage is referenced to the channel, which is not grounded. If the source is at Vs and the drain is at Vd , the


average is Vc = (Vs + Vd)/2 = Vs + Vds /2. Therefore, the mean difference


between the gate and channel potentials Vgc is Vg – Vc = Vgs – Vds /2, as


shown in Figure 2.5.


We can model the gate as a parallel plate capacitor with capacitance proportional to area over thickness. If the gate has length L and width W and the oxide thickness is tox, as shown in Figure 2.6, the capacitance is


(2.2)


where 0 is the permittivity of free space, 8.85 × 10–14 F/cm, and the permittivity of SiO2 is kox = 3.9 times as great. Often, the ox/tox term is called Cox, the capacitance per unit area of the gate oxide.


FIGURE 2.6  Transistor dimensions


C V Vg gc t


channel


= ( )


C kWLt


WL t


C WL


g =


= =


ox


L


tox


SiO2 Gate Oxide


(insulator, ox = 3.9 0)


polysilicon


gate


FIGURE 2.5  Average gate to channel voltage


–


Vgs


Vds


Average gate to channel potential:Vgc = (Vgs + Vgd)/2 = Vgs – Vds/2


Vs


Vd


Cg


Vg


66


Some nanometer processes use a different gate dielectric with a higher dielectric constant. In these processes, we call tox the equivalent oxide thickness (EOT), the thickness of a layer of SiO2 that has the same Cox. In this case, tox is thinner than the actual dielectric.


Each carrier in the channel is accelerated to an average velocity, v, proportional to the lateral electric ﬁeld, i.e., the ﬁeld between source and drain. The constant of proportionality  is called the mobility.


(2.3)


A typical value of  for electrons in an nMOS transistor with low electric ﬁelds is 500–700 cm2/V· s. However, most transistors today operate at far higher ﬁelds where the mobility is severely curtailed (see Section 2.4.1).


The electric ﬁeld E is the voltage difference between drain and source Vds divided by the channel length


(2.4)


The time required for carriers to cross the channel is the channel length divided by the carrier velocity: L/v. Therefore, the current between source and drain is the total amount of charge in the channel divided by the time required to cross


(2.5)


where


(2.6)


The term Vgs – Vt arises so often that it is convenient to abbreviate it as VGT .


EQ  (2.5) describes the linear region of operation, for Vgs > Vt , but Vds relatively small. It is called linear or resistive because when Vds << VGT , Ids increases almost linearly with Vds,just like an ideal resistor. The geometry and technology-dependent parameters are sometimes merged into a single factor . Do not confuse this use of  with the same symbol used for the ratio of collector-to-base current in a bipolar transistor. Some texts [Gray01]lump the technology-dependent parameters alone into a constant called “k prime.”3


(2.7)


If Vds > Vdsat VGT, the channel is no longer inverted in the vicinity of the drain; we say it is pinched off. Beyond this point, called the drain saturation voltage, increasing the drain voltage has no further effect on current. Substituting Vds = Vdsat at this point of maximum current into EQ (2.5), we ﬁnd an expression for the saturation current that is independent of Vds.


(2.8)


3Other sources (e.g., MOSIS) deﬁne


; check the deﬁnition before using quoted data.


v E=


EVLds=


IQL v


CWLV V V


V


ds


gs


GT


= (


)Vds


CWLV


V V


;


k


Cox


=2BV22


2.2      Long-Channel I-V Characteristics 67


This expression is valid for Vgs > Vt and Vds > Vdsat . Thus, long-channel MOS transistors are said to exhibit square-law behavior in saturation.


Two key ﬁgures of merit for a transistor are Ion and Ioff. Ion (also called Idsat) is the ON current, Ids, when Vgs = Vds = VDD. Ioff is the OFF current when Vgs = 0 and Vds = VDD.


According to the long-channel model, Ioff = 0 and


(2.9)


EQ (2.10) summarizes the current in the three regions:


(2.10)


Example 2.1


Consider an nMOS transistor in a 65 nm process with a minimum drawn channel length of 50 nm ( = 25 nm). Let W/L = 4/2  (i.e., 0.1/0.05 m). In this process, the gate oxide thickness is 10.5 Å. Estimate the high-ﬁeld mobility of electrons to be 80 cm2/V· s at 70 ºC. The threshold voltage is 0.3 V. Plot Ids vs. Vds for Vgs = 0, 0.2, 0.4,


0.6, 0.8, and 1.0 V using the long-channel model.


SOLUTION: We ﬁrst calculate .


(2.11)


Figure 2.7(a) shows the I-V characteristics for the transistor. According to the ﬁrst-order model, the current is zero for gate voltages below Vt. For higher gate voltages, current increases linearly with Vds for small Vds . As Vds reaches the saturation point Vdsat = VGT,current rolls off and eventually becomes independent of Vds when the transistor is saturated. We will later see that the Shockley model overestimates current at high voltage because it does not account for mobility degradation and velocity saturation caused by the high electric ﬁelds.


pMOS transistors behave in the same way, but with the signs of all voltages and currents reversed. The I-V characteristics are in the third quadrant, as shown in Figure 2.7(b).


To keep notation simple in this text, we will disregard the signs and just remember that the current ﬂows from source to drain in a pMOS transistor. The mobility of holes in silicon is typically lower than that of electrons. This means that pMOS transistors provide less current than nMOS transistors of comparable size and hence are slower. The symbols n and p are used to distinguish mobility of electrons and of holes in nMOS and pMOS transistors, respectively. The mobility ratio n / p is typically 2–3; we will generally use 2 for examples in this book. The pMOS transistor has the same geometry as the nMOS in Figure 2.7(a), but with p = 40 cm2/V· s and Vtp = – 0.3 V. Similarly, n, p, k n, and k p are sometimes used to distinguish nMOS and pMOS I-V characteristics.


DD


on


= ( )2


<


Cutoff Linear


dsat


ds > dsat Saturation


× ×


×


CWLox


F cm


cm V s


80


3 9 8 85 10


10 5 10


. .


.


262


cm


A V


W L


68


2.3 C-V Characteristics


Each terminal of an MOS transistor has capacitance to the other terminals. In general,these capacitances are nonlinear and voltage dependent (C-V); however, they can be approximated as simple capacitors when their behavior is averaged across the switching voltages of a logic gate. This section ﬁrst presents simple models of each capacitance suitable for estimating delay and power consumption of transistors. It then explores more detailed models used for circuit simulation. The more detailed models may be skipped on a ﬁrst reading.


2.3.1 Simple MOS Capacitance Models


The gate of an MOS transistor is a good capacitor. Indeed, its capacitance is necessary to attract charge to invert the channel, so high gate capacitance is required to obtain high Ids.


As seen in Section 2.2, the gate capacitor can be viewed as a parallel plate capacitor with the gate on top and channel on bottom with the thin oxide dielectric between. Therefore,the capacitance is


(2.12)


The bottom plate of the capacitor is the channel, which is not one of the transistor’s terminals. When the transistor is on, the channel extends from the source (and reaches the drain if the transistor is unsaturated, or stops short in saturation). Thus, we often approximate the gate capacitance as terminating at the source and call the capacitance Cgs.


Most transistors used in logic are of minimum manufacturable length because this results in greatest speed and lowest dynamic power consumption.4 Thus, taking this miniFIGURE 2.7  I-V characteristics of ideal 4/2  (a) nMOS and (b) pMOS transistors


4Some designs use slightly longer than minimum transistors that have higher thresholds because of the short-channel effect (see Sections 2.4.3.3 and 5.3.3). This avoids the cost of an extra mask step for highVt transistors. The change in channel length is small (~5–10%), so the change in gate capacitance is minor.


(b)Vds


Ids(μA)


100 150


0.2


0.4


0.6


0.8


−0.2


−0.4


−0.6


−0.8


−1


−50


−100


−150+0


Vgs = 1.0


Vgs = −0.4 Vgs = −0.6 Vgs = −0.8


Vgs = −1.0


Vgs = 0.8


Vgs = 0.6 Vgs = 0.4


C C WLg = ox


2.3      C-V Characteristics 69


mum L as a constant for a particular process, we can deﬁne


(2.13)


(2.14)


Notice that if we develop a more advanced manufacturing process in which both the channel length and oxide thickness are reduced by the same factor, Cpermicron remains unchanged. This relationship is handy for quick calculations but not exact; Cpermicron has fallen from about 2 fF/ m in old processes to about 1 fF/ m at the 90 and 65 nm nodes. Table 8.5 lists gate capacitance for a variety of processes.


In addition to the gate, the source and drain also have capacitances. These capacitances are not fundamental to operation of the devices, but do impact circuit performance and hence are called parasitic capacitors. The source and drain capacitances arise from the p–n junctions between the source or drain diffusion and the body and hence are also called diffusion5 capacitance Csb and Cdb . A depletion region with no free carriers forms along the junction. The depletion region acts as an insulator between the conducting p- and n-type regions, creating capacitance across the junction. The capacitance of these junctions depends on the area and perimeter of the source and drain diffusion, the depth of the diffusion, the doping levels, and the voltage. As diffusion has both high capacitance and high resistance, it is generally made as small as possible in the layout. Three types of diffusion regions are frequently seen, illustrated by the two series transistors in Figure 2.8. In Figure


5Device engineers more properly call this depletion capacitance, but the term diffusion capacitance is widely used by circuit designers.


FIGURE 2.8  Diffusion region geometries


C C


g = ×permicron


C LtL


permicron ox


ox ox


3λ


6λ


5λ


Drain2


Gate2


Source2


Drain1


Gate1


Source1


Isolated Diffusion


Shared Diffusion


Merged Diffusion


70


2.8(a), each source and drain has its own isolated region of contacted diffusion. In Figure


2.8(b), the drain of the bottom transistor and source of the top transistor form a shared contacted diffusion region. In Figure 2.8(c), the source and drain are merged into an uncontacted region. The average capacitance of each of these types of regions can be calculated or measured from simulation as a transistor switches between VDD and GND.


Table 8.5 also lists the capacitance for each scenario for a variety of processes.


For the purposes of hand estimation, you can observe that the diffusion capacitance Csb and Cdb of contacted source and drain regions is comparable to the gate capacitance(e.g., 1–2 fF/ m of gate width). The diffusion capacitance of the uncontacted source or drain is somewhat less because the area is smaller but the difference is usually unimportant for hand calculations. These values of Cg = Csb = Cdb  1fF/ m will be used in examples throughout the text, but you should obtain the appropriate data for your process using methods to be discussed in Section 8.4.


2.3.2  Detailed MOS Gate Capacitance Model


OPTIONAL


The MOS gate sits above the channel and may partially overlap the source and drain diffusion areas. Therefore, the gate capacitance has two components: the intrinsic capacitance Cgc (over the channel) and the overlap capacitances Cgol (to the source and drain). The intrinsic capacitance was approximated as a simple parallel plate in EQ (2.12)with capacitance C0 = WLCox. However, the bottom plate of the capacitor depends on the mode of operation of the transistor. The intrinsic capacitance has three components representing the different terminals connected to the bottom plate: Cgb (gate-to-body), Cgs(gate-to-source), and Cgd (gate-to-drain). Figure 2.9(a) plots capacitance vs. Vgs in the cutoff region and for small Vds, while 2.9(b) plots capacitance vs. Vds in the linear and saturation regions [Dally98].


1. Cutoff. When the transistor is OFF (Vgs < Vt), the channel is not inverted and charge  on the gate is matched with opposite charge from the body. This is called Cgb, the


gate-to-body capacitance. For negative Vgs, the transistor is in accumulation and Cgb =C0. As Vgs increases but remains below a threshold, a depletion region forms at the


surface. This effectively moves the bottom plate downward from the oxide, reducing  the capacitance, as shown in Figure 2.9(a).


2. Linear. When Vgs > Vt, the channel inverts and again serves as a good conductive bottom plate. However, the channel is connected to the source and drain, rather than the  body, so Cgb drops to 0. At low values of Vds, the channel charge is roughly shared


between source and drain, so Cgs = Cgd = C0/2. As Vds increases, the region near the  drain becomes less inverted, so a greater fraction of the capacitance is attributed to the  source and a smaller fraction to the drain, as shown in Figure 2.9(b).


3. Saturation. At Vds > Vdsat,  the transistor saturates and the channel pinches off. At this  point, all the intrinsic capacitance is to the source, as shown in Figure 2.9(b). Because  of pinchoff, the capacitance in saturation reduces to Cgs = 2/3 C0 for an ideal transistor [Gray01].


The behavior in these three regions can be approximated as shown in Table 2.1.


FIGURE 2.9  Intrinsic gate capacitance Cgc = Cgs + Cgd + Cgb as a  function of (a) Vgs and (b) Vds


7Vgs


0 Vt


C0


C0 2


Cgb


Cgs,Cgd Cgc


Cgs


Cgc


Vds Vdsat 3


2C0


Cgd


2.3      C-V Characteristics 71


The gate overlaps the source and drain in a real device and also has fringing ﬁelds terminating on the source and drain. This leads to additional overlap capacitances, as shown in Figure 2.10. These capacitances are proportional to


the width of the transistor. Typical values are Cgsol = Cgdol = 0.2 – 0.4 fF/ m.


They should be added to the intrinsic gate capacitance to ﬁnd the total.


(2.15)


It is convenient to view the gate capacitance as a single-terminal capacitor attached to the gate (with the other side not switching). Because the source and drain actually form second terminals, the effective gate capacitance varies with the switching activity of the source and drain. Figure 2.11 shows the effective gate capacitance in a 0.35 m process for seven different combinations of source and drain behavior [Bailey98].


More accurate modeling of the gate capacitance may be achieved by using a chargebased model [Cheng99]. For the purpose of delay calculation of digital circuits, we usually approximate Cg = Cgs + Cgd + Cgb C0 + 2CgolW or use an effective capacitance extracted


TABLE 2.1  Approximation for intrinsic MOS gate capacitance


|Parameter |Cutoff |Linear |Saturation |
|---|---|---|---|

|Cgb |C0 |0 |0 |

|Cgs |0 |C0/2 |2/3 C0 |

|Cgd |0 |C0/2 |0 |

|Cg = Cgs + Cgd + Cgb |C0 |C0 |2/3 C0 |

FIGURE 2.11  Data-dependent gate capacitance


C W


gsol


gdol


overlap


==


Case 1


Case 2


Case 3


Case 4


Case 5


Case 6


Case 7


1 IL1


Cg/C0


1.3


1.1


1.0


.80


.42


.31.13


Case 1 Case 2 Case 3 Case 4


Case 5 Case 6 Case 7


FIGURE 2.10  Overlap capacitance


Cgdol


Cgsol


72


from simulation [Nose00b]. It is important to remember that this model signiﬁcantly overestimates the capacitance of transistors operating just below threshold.


2.3.3  Detailed MOS Diffusion Capacitance Model


As mentioned in Section 2.3.1, the p–n junction between the source diffusion and the body contributes parasitic capacitance across the depletion region. The capacitance depends on both the area AS and sidewall perimeter PS of the source diffusion region. The geometry is illustrated in Figure 2.12. The area is AS = WD. The perimeter is PS = 2W +2D. Of this perimeter, W abuts the channel and the remaining W + 2D does not.


The total source parasitic capacitance is


(2.16)


where Cjbs (the capacitance of the junction between the body and the bottom of the source) has units of capacitance/area and Cjbssw (the capacitance of the junction between the body and the side walls of the source) has units of capacitance/length.


Because the depletion region thickness depends on the bias conditions, these parasitics are nonlinear. The area junction capacitance term is [Gray01]


(2.17)


CJ is the junction capacitance at zero bias and is highly process-dependent. MJ is the junction grading coefﬁcient, typically in the range of 0.5 to 0.33 depending on the abruptness of the diffusion junction.   is the built-in potential that depends on doping levels.


(2.18)


vT is the thermal voltage from thermodynamics, not to be confused with the threshold voltage Vt . It has a value equal to kT/q (26 mV at room temperature), where k = 1.380 ×10–23 J/K is Boltzmann’s constant, T is absolute temperature (300 K at room temperature),and  q = 1.602 × 10–19 C is the charge of an electron. NA and ND are the doping levels of the body and source diffusion region. ni is the intrinsic carrier concentration in undoped silicon and has a value of 1.45 × 1010 cm–3 at 300 K.


The sidewall capacitance term is of a similar form but uses different coefﬁcients.


(2.19)


In processes below about 0.35 m that employ shallow trench isolation surrounding transistors with an SiO2 insulator (see Section 3.2.6), the sidewall capacitance along the nonconductive trench tends to be minimal, while the sidewall facing the channel is more signiﬁcant. In some SPICE models, the capacitance of this sidewall abutting the gate and channel is speciﬁed with another set of parameters:


(2.20)


C AS C


PS C


sb


jbs


jbssw


= × + ×


M J


= +1400


= vN N n


A D


i


ln


JSW


sw,SW


M JSW


= +1


jbsswg


sb SWG


M JSWG


FIGURE 2.12  Diffusion region geometry


W Source


2.3      C-V Characteristics 73


Section 8.3.4 discusses SPICE perimeter capacitance models further.


The drain diffusion has a similar parasitic capacitance dependent on AD, PD, and Vdb. Equivalent relationships hold for pMOS transistors, but doping levels differ. As the capacitances are voltage-dependent, the most useful information to digital designers is the value averaged across a switching transition. This is the Csb or Cdb value that was presented in Section 2.3.1.


Example 2.2


Calculate the diffusion parasitic Cdb of the drain of a unit-sized contacted nMOS transistor in a 65 nm process when the drain is at 0 V and again at VDD = 1.0 V. Assume the substrate is grounded. The diffusion region conforms to the design rules from Figure


2.8 with = 25 nm. The transistor characteristics are CJ = 1.2 fF/ m2, MJ = 0.33,CJSW = 0.1 fF/ m, CJSWG = 0.36 fF/ m, MJSW = MJSWG = 0.10, and 0 = 0.7 V at room temperature.


SOLUTION: From Figure 2.8, we ﬁnd a unit-size diffusion contact is 4 × 5 , or 0.1 ×


0.125 m. The area is 0.0125 m2 and perimeter is 0.35 m plus 0.1 m along the channel. At zero bias, Cjbd = 1.2 fF/ m2, Cjbdsw = 0.1 fF/ m, and Cjbdswg = 0.36 fF/m. Hence, the total capacitance is


(2.21)


At a drain voltage of VDD, the capacitance reduces to


(2.22)


For the purpose of manual performance estimation, this nonlinear capacitance is too


much effort. An effective capacitance averaged over the switching range is quite satisfactory for digital applications. In this example, the effective drain capacitance would


be approximated as the average of the two extremes, 0.081 fF.


Diffusion regions were historically used for short wires called runners in processes


with only one or two metal levels. Diffusion capacitance and resistance are large


enough that such practice is now discouraged; diffusion regions should be kept asXsmall as possible on nodes that switch.


In summary, an MOS transistor can be viewed as a four-terminal device with


capacitances between each terminal pair, as shown in Figure 2.13. The gate capacitance includes an intrinsic component (to the body, source and drain, or source alone,


depending on operating regime) and overlap terms with the source and drain. The


source and drain have parasitic diffusion capacitance to the body.


Cdb 0


0 0125


1 2


0 35


mfF m


mfF


( ) = (


( )


fF


+ ( )


0 36


0 086


Cdb 1


11 00 7


.+


0 33


(1+


10 7


0 076


0 10


FIGURE 2.13  Capacitance of an  MOS transistor


。Drain


Body


Cgs 9Cgd


古Cdb


Csb


灭Cgb


74


2.4 Nonideal I-V Effects


The long-channel I-V model of EQ (2.10) neglects many effects that are important to devices with channel lengths below 1 micron. This section summarizes the effects of greatest signiﬁcance to designers, then models each one in more depth.


Figure 2.14 compares the simulated I-V characteristics of a 1-micron wide nMOS transistor in a 65 nm process to the ideal characteristics computed in Section 2.2. The saturation current increases less than quadratically with increasing Vgs . This is caused by two effects: velocity saturation and mobility degradation. At high lateral ﬁeld strengths(Vds /L), carrier velocity ceases to increase linearly with ﬁeld strength. This is called velocity saturation and results in lower Ids than expected at high Vds . At high vertical ﬁeld strengths(Vgs /tox), the carriers scatter off the oxide interface more often, slowing their progess.


This mobility degradation effect also leads to less current than expected at high Vgs . The saturation current of the nonideal transistor increases somewhat with Vds . This is caused by channel length modulation, in which higher Vds increases the size of the depletion region around the drain and thus effectively shortens the channel.


The threshold voltage indicates the gate voltage necessary to invert the channel and is primarily determined by the oxide thickness and channel doping levels. However, otherﬁelds in the transistor have some effect on the channel, effectively modifying the threshold voltage. Increasing the potential between the source and body raises the threshold through the body effect. Increasing the drain voltage lowers the threshold through drain-induced barrier lowering. Increasing the channel length raises the threshold through the short channel effect.


Several sources of leakage result in current ﬂow in nominally OFF transistors. When Vgs < Vt , the current drops off exponentially rather than abruptly becoming zero. This is called subthreshold conduction. The current into the gate Ig is ideally 0.  However, as the


FIGURE 2.14  Simulated and ideal I-V characteristics


400 600 800 1000 1200


Ids( A)


车


Vgs = 0.6


Vgs = 0.4 Vgs = 1.0↓


州/


Channel length modulation:


Saturation current increases


with Vds一


Ion = 747 mA @


Vgs = Vds = VDD


Simulated


Ideal (based on example in Section 2.2)


Velocity saturation and mobility degradation:Saturation current increases less than


quadratically with Vgs


Velocity saturation and mobility degradation:Ion lower than ideal model predicts


2.4      Nonideal I-V Effects 75


thickness of gate oxides reduces to only a small number of atomic layers, electrons tunnel through the gate, causing some gate leakage current. The source and drain diffusions are typically reverse-biased diodes and also experience junction leakage into the substrate or well.


Both mobility and threshold voltage decrease with rising temperature. The mobility effect tends to dominate for strongly ON transistors, resulting in lower Ids at high temperature. The threshold effect is most important for OFF transistors, resulting in higher leakage current at high temperature. In summary, MOS characteristics degrade with temperature.


It is useful to have a qualitative understanding of nonideal effects to predict their impact on circuit behavior and to be able to anticipate how devices will change in future process generations. However, the effects lead to complicated I-V characteristics that are hard to directly apply in hand calculations. Instead, the effects are built into good transistor models and simulated with SPICE or similar software.


2.4.1 Mobility Degradation and Velocity Saturation


Recall from EQ (2.3) that carrier drift velocity, and hence current, is proportional to the lateral electric ﬁeld Elat = Vds /L between source and drain. The constant of proportionality is called the carrier mobility, . The long-channel model assumed that carrier mobility is independent of the applied ﬁelds. This is a good approximation for low ﬁelds, but breaks down when strong lateral or vertical ﬁelds are applied.


As an analogy, imagine that you have been working all night in the VLSI lab and decide to run down and across the courtyard to the coffee cart.6 The number of hours you have been up is analogous to the lateral electric ﬁeld. The longer you have been up, the faster you want to reach coffee: Your speed equals your fatigue times your mobility. There is a strong wind blowing in the courtyard, analogous to the vertical electric ﬁeld. This wind buffets you against the wall, slowing your progress. In the same way, a high voltage at the gate of the transistor attracts the carriers to the edge of the channel, causing collisions with the oxide interface that slow the carriers. This is called mobility degradation. Moreover, freshman physics is just letting out of the lecture hall. Occasionally, you bounce off a confused freshman, fall down, and have to get up and start running again. This is analogous to carriers scattering off the silicon lattice (technically called collisions with optical phonons). The faster you try to go, the more often you collide. Beyond a certain level of fatigue, you reach a maximum average speed. In the same way, carriers approach a maximum velocity vsat when high ﬁelds are applied. This phenomenon is called velocity saturation.7


Mobility degradation can be modeled by replacing  with a smaller eff that is a function of Vgs. A universal model [Chen96, Chen97] that matches experimental data from multiple processes reasonably well is


(2.23)


6This practice has been observed empirically, but is not recommended. Productivity decreases with fatigue.


Beyond a certain point of exhaustion, the net work accomplished per hour becomes negative because so many mistakes are made.


7Do not confuse the saturation region of transistor operation (where Vds > Vgs – Vt) with velocity saturation(where Elat = Vds /L approaches Ec). In this text, the word “saturation” alone refers to the operating region while “velocity saturation” refers to the limiting of carrier velocity at high ﬁeld.


eff


V nm


++


540V.s


0 54nm


1 85


·


V t


185


1 5 0 338nm


76


Example 2.3


Compute the effective mobilities for nMOS and pMOS transistors when they are fully ON. Use the physical parameters from Example 2.1.


SOLUTION: Use Vgs = 1.0 for ON transistors, remembering that we are treating voltages as positive in a pMOS transistor. Substituting Vt = 0.3 V and tox = 1.05 nm into EQ(2.23) gives:


eff-n(Vgs = 1.0) = 96 cm2/V, eff-p(Vgs = 1.0) = 36 cm2/V


Figure 2.15 shows measured data for carrier velocity as a function of the electric ﬁeld,E, between the drain and source. At low ﬁelds, the velocity increases linearly with theﬁeld. The slope is the mobility, eff. At ﬁelds above a critical level, Ec , the velocity levels out at vsat, which is approximately 107 cm/s for electrons and 8 × 106 cm/s for holes[Muller03]. As shown in the ﬁgure, the velocity can be approximated reasonably well with the following expression [Toh88, Takeuchi94]:


(2.24)


where, by continuity, the critical electric ﬁeld is


(2.25)


The critical voltage Vc is the drain-source voltage at which the critical effective ﬁeld is reached: Vc = Ec L.


Example 2.4


Find the critical voltage for fully ON nMOS and pMOS transistors using the effective mobilities from Example 2.3.


SOLUTION: Using EQ (2.25)


The nMOS transistor is velocity saturated in normal operation because Vc-n is comparable to VDD. The pMOS transistor has lower mobility and thus is not as badly velocity saturated.


Using a derivation similar to that of Section 2.2 with the new carrier velocity expression in EQ (2.24) gives modiﬁed equations for linear and saturation currents [Sodini84].


v


E


E E


c


= +


sat


v c =2 sat eff


c n


c p


=( )×( ) =


2 10 96


5 10


1 04


2 8 1


cm s


cm V


2 22


)×( ) =


FIGURE 2.15  Carrier velocity vs. electric ﬁeld at 300 K, adapted  from [Jacoboni77]. Velocity


saturates at high ﬁelds.


103 106


107


104


105


E (V/cm)


v (cm/s)


Electrons


Holes


Measured


Curve Fit vsat-n vsat-p


μpμn


2.4      Nonideal I-V Effects 77


(2.26)


Note that eff is a decreasing function of Vgs because of mobility degradation. Observe that the current in the linear regime is the same as in EQ (2.5) except that the mobility term is reduced by a factor related to Vds. At sufﬁciently high lateral ﬁelds, the current saturates at some value dependent on the maximum carrier velocity. Equating the two parts of EQ(2.26) at Vds = Vdsat lets us solve for the saturation voltage


(2.27)


Noting that EQ (2.27) is in the same form as a parallel resistor equation, we see that Vdsat is less than the smaller of VGT and Vc . Finally, substituting EQ (2.27) into EQ (2.26) gives a simpliﬁed expression for saturation current accounting for velocity saturations:


(2.28)


If VGT << Vc , velocity saturation effects are negligible and EQ (2.28) reduces to the squarelaw model. This is also called the long-channel regime. But if VGT >> Vc , EQ (2.28)approaches the velocity-saturated limit


(2.29)


Observe that the drain current is quadratically dependent on voltage in the longchannel regime and linearly dependent when fully velocity saturated. For moderate supply voltages, transistors operate in a region where the velocity neither increases linearly withﬁeld, nor is completely saturated. The -power law model given in EQ (2.30) provides a simple approximation to capture this behavior [Sakurai90].  is called the velocity saturation index and is determined by curve ﬁtting measured I-V data. Transistors with long channels or low VDD display quadratic I-V characteristics in saturation and are modeled with = 2. As transistors become more velocity saturated, increasing Vgs has less effect on current and  decreases, reaching 1 for transistors that are completely velocity saturated.


For simplicity, the model uses a straight line in the linear region. Overall, the model is based on three parameters that can be determined empirically from a curve ﬁt of I-V characteristics: , Pc , and Pv.


(2.30)


(2.31)


V V V


ds c


) <


dsat Linea


r


Saturation


dsat sat


C W V


V v


>


GT c GT


WC v


GT GT


dsat ox sat


WC v V


IVV


<<


Cutoff


Linear


dsat Saturation


V Vds >


P V


0c


v GT


78


Figure 2.16 compares the -power law model against simulated results, using = 1.3. The ﬁt is poor at low Vds , but the current at Vds = VDD matches simulation fairly well across the full range of Vgs.


The low-ﬁeld mobility of holes is much lower than that of electrons, so pMOS transistors experience less velocity saturation than nMOS for a given VDD. This shows up as a larger value of for pMOS than for nMOS transistors.


These models become too complicated to give much insight for hand calculations. A simpler approach is to observe, in velocitysaturated transistors, Ids grows linearly rather than quadratically with Vgs when the transistor is strongly ON. Figure 2.17 plots Ids vs. Vgs(holding Vds = Vgs). This is equivalent to plotting Ion vs. VDD. For Vgs signiﬁcantly above Vt, Ids ﬁts a straight line quite well. Thus, we can approximate the ON current as


(2.32)


where Vt* is the x-intercept.


2.4.2 Channel Length Modulation


Ideally, Ids is independent of Vds for a transistor in saturation, making the transistor a perfect current source. As discussed in Section 2.3.3, the p–n junction between the drain and body forms a depletion region with a width Ld that increases with Vdb , as shown in Figure 2.18. The depletion region effectively shortens the channel length to


(2.33)


To avoid introducing the body voltage into our calculations,assume the source voltage is close to the body voltage so Vdb Vds.


Hence, increasing Vds decreases the effective channel length. Shorter channel length results in higher current; thus, Ids increases with Vds in saturation, as shown in Figure 2.18. This can be crudely modeled by multiplying EQ (2.10) by a factor of (1 + Vds / VA), where VA is called the Early voltage [Gray01]. In the saturation region, we ﬁnd


(2.34)


As channel length gets shorter, the effect of the channel length modulation becomes relatively more important. Hence, VA is propor-


09e


tional to channel length. This channel length modulation model is a gross oversimpliﬁcation of nonlinear behavior and is more useful for conceptual understanding than for accurate device modeling.


Channel length modulation is very important to analog designers because it reduces the gain of ampliﬁers. It is generally unimportant for qualitatively understanding the behavior of digital circuits.


I k V Vds gs t= ( )*


L Ld


ds A


FIGURE 2.16  Comparison of -power law model with  simulated transistor behavior


0.6 0.8


0 200 400 600 800


厂Vds


Simulated-power law


800


600


400


Ids (μA)


Vgs = Vds


V*t


0 0.2 0.4 0.6 0.8 1.0


FIGURE 2.17 Ids vs. Vgs in saturation, showing good linear ﬁt at high Vgs


晶n+


p-type body田田⑤b


Vdb


L Leff


Ld


Depletion


region


FIGURE 2.18  Depletion region shortens effective  channel length


2.4      Nonideal I-V Effects 79


2.4.3 Threshold Voltage Effects


So far, we have treated the threshold voltage as a constant. However, Vt increases with the source voltage, decreases with the body voltage, decreases with the drain voltage, and increases with channel length [Roy03]. This section models each of these effects.


2.4.3.1 Body Effect Until now, we have considered a transistor to be a three-terminal device with gate, source, and drain. However, the body is an implicit fourth terminal.


When a voltage Vsb is applied between the source and body, it increases the amount of charge required to invert the channel, hence, it increases the threshold voltage. The threshold voltage can be modeled as


(2.35)


where Vt 0 is the threshold voltage when the source is at the body potential, s is the surface potential at threshold (see a device physics text such as [Tsividis99] for further discussion of surface potential), and  is the body effect coefﬁcient, typically in the range 0.4 to 1 V1/2.


In turn, these depend on the doping level in the channel, NA. The body effect further degrades the performance of pass transistors trying to pass the weak value (e.g., nMOS transistors passing a ‘1’), as we will examine in Section 2.5.4. Section 5.3.4 will describe how a body bias can intentionally be applied to alter the threshold voltage, permitting trade-offs between performance and subthreshold leakage current.


(2.36)


(2.37)


For small voltages applied to the source or body, EQ (2.35) can be linearized to


(2.38)


(2.39)


Example 2.5


Consider the nMOS transistor in a 65 nm process with a nominal threshold voltage of


0.3 V and a doping level of 8 × 1017 cm–3. The body is tied to ground with a substrate contact. How much does the threshold change at room temperature if the source is at


0.6 V instead of 0?


SOLUTION: At room temperature, the thermal voltage vT = kT/q = 26 mV and ni = 1.45× 1010 cm–3. The threshold increases by 0.04 V.


= + +(


A i


vNn


= 2 ln


si


si ox


q


V V k Vt t sb= +0


N n


= γ=


q si


(2.40)


2.4.3.2 Drain-Induced Barrier Lowering The drain voltage Vds creates an electric ﬁeld that affects the threshold voltage. This drain-induced barrier lowering (DIBL) effect is especially pronounced in short-channel transistors. It can be modeled as


(2.41)


where  is the DIBL coefﬁcient, typically on the order of 0.1 (often expressed as 100 mV/V).


Drain-induced barrier lowering causes Ids to increase with Vds in saturation, in much the same way as channel length modulation does. This effect can be lumped into a smaller Early voltage VA used in EQ (2.34). Again, this is a bane for analog design but insigniﬁcant for most digital circuits. More signiﬁcantly, DIBL increases subthreshold leakage at high Vds, as we will discuss in Section 2.4.4.


2.4.3.3 Short Channel Effect The threshold voltage typically increases with channel length. This phenomenon is especially pronounced for small L where the source and drain depletion regions extend into a signiﬁcant portion of the channel, and hence is called the short channel effect8 or Vt rolloff [Tsividis99, Cheng99]. In some processes, a reverse short channel effect causes Vt  to decrease with length.


There is also a narrow channel effect in which Vt varies with channel width; this effect tends to be less signiﬁcant because the minimum width is greater than the minimum length.


0O2.4.4 Leakage


Even when transistors are nominally OFF, they leak small amounts of current. Leakage mechanisms include subthreshold conduction between source and drain, gate leakage from the gate to body, and junction leakage from source to body and drain to body, as illustrated in Figure 2.19 [Roy03, Narendra06]. Subthreshold conduction is caused by thermal emission of carriers over the potential barrier set by the threshold. Gate leakage is a quantum-mechanical effect caused by tunneling through the extremely thin gate dielectric. Junction leakage is caused by current through the p-n junction between the source/drain diffusions and the body.


8The term short-channel effect is overused in the CMOS literature. Sometimes, it refers to any behavior outside the long-channel models. Other times, it refers to a range of behaviors including DIBL that are most signiﬁcant for very short channel lengths [Muller03]. In this text, we restrict the term to describe the sensitivity of threshold voltage to channel length.


s = ( ) ××


2 0 026


8 10 1 45 10


0 93


cm cm


r==


5 10 3 9 8 85 10


2 1 6 10


11 7 8


19


×× ×


) ×


85 10


8 10


0 16


0 3


0 6


) ×(


) =


= + +


Vt


) = 0 34. V


= 0


FIGURE 2.19


Leakage current paths


tn+Gate


Body Isub


Ijunct Igate


2.4      Nonideal I-V Effects 81


In processes with feature sizes above 180 nm, leakage was typically insigniﬁcant except in very low power applications. In 90 and 65 nm processes, threshold voltage has reduced to the point that subthreshold leakage reaches levels of 1s to 10s of nA per transistor, which is signiﬁcant when multiplied by millions or billions of transistors on a chip.


In 45 nm processes, oxide thickness reduces to the point that gate leakage becomes comparable to subthreshold leakage unless high-k gate dielectrics are employed. Overall, leakage has become an important design consideration in nanometer processes.


2.4.4.1 Subthreshold Leakage The long-channel transistor I-V model assumes current only ﬂows from source to drain when Vgs > Vt. In real transistors, current does not abruptly cut off below threshold, but rather drops off exponentially, as seen in Figure 2.20. When the gate voltage is high, the transistor is strongly ON. When the gate falls below Vt , the exponential decline in current appears as a straight line on the logarithmic scale. This regime of Vgs < Vt is called weak inversion. The subthreshold leakage current increases signiﬁcantly with Vds because of drain-induced barrier lowering (see Section 2.4.3.2). There is a lower limit on Ids set by drain junction leakage that is exacerbated by the negative gate voltage (see Section 2.4.4.3).


Subthreshold leakage current is described by EQ (2.42). Ids0 is the current at threshold and is dependent on process and device geometry. It is typically extracted from simulation but can also be calculated from EQ (2.43); the e1.8 term was found empirically[Sheu87]. n is a process-dependent term affected by the depletion region characteristics and is typically in the range of 1.3–1.7 for CMOS processes. The ﬁnal term indicates that leakage is 0 if Vds = 0, but increases to its full value when Vds is a few multiples of the thermal voltage vT (e.g., when Vds > 50 mV). More signiﬁcantly, drain-induced barrier lowering effectively reduces the threshold voltage, as indicated by the Vds term. This can increase leakage by an order of magnitude for Vds = VDD as compared to small Vds. The body effect also modulates Vt when Vsb  0.


(2.42)


Idss(A/μm)


100p 10n


1u 100u 10m


1p


10p


1n 100n


承、


10u 1m


−0.6 −0.4 −0.2 0.0 0.2 0.4 0.6 0.8 1.0Vt Vds = 0.1 Vds = 1.0


Ioff = 27 nA/μm


Subthreshold Slope S = 100 mV/decade Saturation


Region


Subthreshold


2.0 nA/μm


DIBL


GIDL


FIGURE 2.20  I-V characteristics of a 65 nm nMOS transistor  at 70 °℃ on a log scaleat 70 C on a log scale


I Ids ds


Vgs Vt


Vds k Vsb


nv


Vds v


82


(2.43)


Subthreshold conduction is used to advantage in very low-power circuits, as will be explored in Section 9.6. It afﬂicts dynamic circuits and DRAMs, which depend on the storage of charge on a capacitor. Conduction through an OFF transistor discharges the capacitor unless it is periodically refreshed or a trickle of current is available to counter the leakage. Leakage also contributes to power dissipation in idle circuits. Subthreshold leakage increases exponentially as Vt decreases or as temperature rises, so it is a major problem for chips using low supply and threshold voltages and for chips operating at high temperature.


As shown in Figure 2.20, subthreshold current ﬁts a straight line on a semilog plot.


The inverse of the slope of this line is called the subthreshold slope, S


(2.44)


The subthreshold slope indicates how much the gate voltage must drop to decrease the leakage current by an order of magnitude. A typical value is 100 mV/decade at room temperature. EQ (2.42) can be rewritten using the subthreshold slope as


(2.45)


where Ioff is the subthreshold current at Vgs = 0 and Vds = VDD.


Example 2.6


What is the minimum threshold voltage for which the leakage current through an OFF transistor (Vgs = 0) is 103 times less than that of a transistor that is barely ON(Vgs = Vt) at room temperature if n = 1.5? One of the advantages of silicon-oninsulator (SOI) processes is that they have smaller n (see Section 9.5). What threshold is required for SOI if n = 1.3?


SOLUTION: vT = 26 mV at room temperature. Assume Vds >> vT so leakage is signiﬁcant. We solve


(2.46)


In the CMOS process, leakage rolls off by a factor of 10 for every 90 mV Vgs falls below threshold. This is often quoted as a subthreshold slope of S = 90 mV/decade.


In the SOI process, the subthreshold slope S is 78 mV/decade, so a threshold of only 234 mV is required.


2.4.4.2 Gate Leakage  According to quantum mechanics, the electron cloud surrounding an atom has a probabilistic spatial distribution. For gate oxides thinner than 15–20 Å,I


2 1 8= e .


Sd


dV


=( )=logln10110


I Ids


Vgs Vds Vdd k Vsb S


Vds vT


off


I V


ds gs


Vt nvT


( ) = ==


10 27


0mV


2.4      Nonideal I-V Effects 83


there is a nonzero probability that an electron in the gate will ﬁnd itself on the wrong side of the oxide, where it will get whisked away through the channel. This effect of carriers crossing a thin barrier is called tunneling, and results in leakage current through the gate.


Two physical mechanisms for gate tunneling are called Fowler-Nordheim (FN) tunneling and direct tunneling. FN tunneling is most important at high voltage and moderate oxide thickness and is used to program EEPROM memories (see Section 12.4). Direct tunneling is most important at lower voltage with thin oxides and is the dominant leakage component.


The direct gate tunneling current can be estimated as [Chandrakasan01]


(2.47)


where A and B are technology constants.


Transistors need high Cox to deliver good ON current, driving the decrease in oxide thickness. Tunneling current drops exponentially with the oxide thickness and has only recently become signiﬁcant. Figure 2.21 plots gate leakage current density (current/area)JG against voltage for various oxide thicknesses. Gate leakage increases by a factor of 2.7 or more per angstrom reduction in thickness [Rohrer05]. Large tunneling currents impact not only dynamic nodes but also quiescent power consumption and thus limits equivalent oxide thicknesses tox to at least 10.5 Å to keep gate leakage below 100 A/cm2.


To keep these dimensions in perspective, recall that each atomic layer of SiO2 is about 3Å, so such gate oxides are a handful of atomic layers thick. Section 3.4.1.3 describes innovations in gate insulators with higher dielectric constants that offer good Cox while reducing tunneling.


Tunneling current can be an order of magnitude higher for nMOS than pMOS transistors with SiO2 gate dielectrics because the electrons tunnel from the conduction band while the holes tunnel from the valence band and see a higher barrier [Hamzaoglu02].


Different dielectrics may have different tunneling properties.


WAVY2_B_toxtDDtVDDB


0 0.3 0.6 0.9 1.2 1.5 1.8


10–9 10–6 10–3 cm2)JG(A/100 103 106 109


tox 6 Å 8 Å 10 Å 12 Å


15 Å 19 Å


VDDtrend


FIGURE 2.21  Gate leakage current from [Song01]


84


2.4.4.3 Junction Leakage The p–n junctions between diffusion and the substrate or well form diodes, as shown in Figure 2.22. The well-to-substrate junction is another diode.


The substrate and well are tied to GND or VDD to ensure these diodes do not become forward biased in normal operation. However, reverse-biased diodes still conduct a small amount of current ID. 9


(2.48)


where IS depends on doping levels and on the area and perimeter of the diffusion region and VD is the diode voltage (e.g., –Vsb or –Vdb). When a junction is reverse biased by signiﬁcantly more than the thermal voltage, the leakage is just –IS, generally in the 0.1–0.01 fA/ m2 range, which is negligible compared to other leakage mechanisms.


More signiﬁcantly, heavily doped drains are subject to band-to-band tunneling(BTBT) and gate-induced drain leakage (GIDL).


BTBT occurs across the junction between the source or drain and the body when the junction is reverse-biased. It is a function of the reverse bias and the doping levels. High halo doping used to increase Vt to alleviate subthreshold leakage instead causes BTBT to grow. The leakage is exacerbated by trap-assisted tunneling (TAT) when defects in the silicon lattice called traps reduce the distance that a carrier must tunnel. Most of the leakage occurs along the sidewall closest to the channel where the doping is highest. It can be modeled as


(2.49)


where Xj is the junction depth of the diffusion, Eg is the bandgap voltage, and A and B are technology constants [Mukhopadhyay05]. The electric ﬁeld along the junction at a reverse bias of VDD is


(2.50)


GIDL occurs where the gate partially overlaps the drain. This effect is most pronounced when the drain is at a high voltage and the gate is at a low voltage. GIDL current is proportional to gate-drain overlap area and hence to transistor width. It is a strong function of the electric ﬁeld and hence increases rapidly with the drain-to-gate voltage. How9Beware that ID and IS stand for the diode current and diode reverse-biased saturation currents, respectively. The D and S are not related to drain or source.


I ID S


V vT


= e


FIGURE 2.22  Substrate to diffusion diodes in CMOS circuits


WX A


BTBT


j


dd


Eg Ej


0 5


1 5


N N N


vN N n


halo sd halo


sd


halo sd


) +


2.4      Nonideal I-V Effects 85


ever, it is normally insigniﬁcant at |Vgd| VDD [Mukhopadhyay05], only coming into play when the gate is driven outside the rails in an attempt to cut off subthreshold leakage.


2.4.5 Temperature Dependence


Transistor characteristics are inﬂuenced by temperature [Cobbold66, Vadasz66,Tsividis99, Gutierrez01]. Carrier mobility decreases with temperature. An approximate relation is


(2.51)


where T is the absolute temperature, Tr is room temperature, and k  is a ﬁtting parameter with a typical value of about 1.5. vsat also decreases with temperature, dropping by about 20% from 300 to 400 K.


The magnitude of the threshold voltage decreases nearly linearly with temperature and may be approximated by


(2.52)


where kvt is typically about 1–2 mV/K.


Ion at high VDD decreases with temperature. Subthreshold leakage increases exponentially with temperature. BTBT increases slowly with temperature, and gate leakage is almost independent of temperature.


The combined temperature effects are shown in Figure 2.23. At high Vgs, the current has a negative temperature coefﬁcient; i.e., it decreases with temperature. At low Vgs, the current has a positive temperature coefﬁcient. Thus, OFF current increases with temperature.


ON current Idsat normally decreases with temperature, as shown in Figure 2.24, so circuit performance is worst at high temperature. However, for systems operating at low VDD(typically < 0.7 – 1.1 V), Idsat increases with temperature [Kumar06].


TTTrrk


( ) = ( )


V T V T k T Tt t r vt r( ) ( ) ( )=


Increasing Temperature


Ids


FIGURE 2.23  I–V characteristics of nMOS transistor in  saturation at various temperatures


Ion(μA)


720


740 760 780 800


0 20 40 60 80 100 120 Temperature (C)


FIGURE 2.24  Idsat vs. temperature


86


Conversely, circuit performance can be improved by cooling. Most systems use natural convection or fans in conjunction with heat sinks, but water cooling, thin-ﬁlm refrigerators, or even liquid nitrogen can increase performance if the expense is justiﬁed. There are many advantages of operating at low temperature [Keyes70, Sun87]. Subthreshold leakage is exponentially dependent on temperature, so lower threshold voltages can be used.


Velocity saturation occurs at higher ﬁelds, providing more current. As mobility is also higher, these ﬁelds are reached at a lower power supply, saving power. Depletion regions become wider, resulting in less junction capacitance.


Two popular lab tools for determining temperature dependence in circuits are a can of freeze spray and a heat gun. The former can be used to momentarily “freeze” a chip to see whether performance alters and the other, of course, can be used to heat up a chip. Often,these tests are done to quickly determine whether a chip is prone to temperature effects. Be careful—sometimes the sudden temperature change can fracture chips or their packages.


2.4.6 Geometry Dependence


The layout designer draws transistors with width and length Wdrawn and Ldrawn. The actual gate dimensions may differ by some factors XW and XL. For example, the manufacturer may create masks with narrower polysilicon or may overetch the polysilicon to provide shorter channels (negative XL) without changing the overall design rules or metal pitch. Moreover, the source and drain tend to diffuse laterally under the gate by LD, producing a shorter effective channel length that the carriers must traverse between source and drain. Similarly, WD accounts for other effects that shrink the transistor width. Putting these factors together, we can compute effective transistor lengths and widths that should be used in place of L and W in the current and capacitance equations given elsewhere in the book. The factors of two come from lateral diffusion on both sides of the channel.


(2.53)


Therefore, a transistor drawn twice as long may have an effective length that is more than twice as great. Similarly, two transistors differing in drawn widths by a factor of two may differ in saturation current by more than a factor of two. Threshold voltages also vary with transistor dimensions because of the short and narrow channel effects.


Combining threshold changes, effective channel lengths, channel length modulation,and velocity saturation effects, Idsat does not scale exactly as 1/L. In general, when currents must be precisely matched (e.g., in sense ampliﬁers or A/D converters), it is best to use the same width and length for each device. Current ratios can be produced by tying several identical transistors in parallel.


In processes below 0.25 m, the effective length of the transistor also depends signiﬁcantly on the orientation of the transistor. Moreover, the amount of nearby polysilicon also affects etch rates during manufacturing and thus channel length. Transistors that must match well should have the same orientation. Dummy polysilicon wires can be placed nearby to improve etch uniformity.


2.4.7 Summary


Although the physics of nanometer-scale devices is complicated, the impact of nonideal I-V behavior is fairly easy to understand from the designer’s viewpoint.


W W


eff drawn eff drawn


= += +


2 2


2.5      DC Transfer Characteristics 87


Threshold drops  Pass transistors suffer a threshold drop when passing the wrong value:


nMOS transistors only pull up to VDD – Vtn, while pMOS transistors only pull down to


|Vtp|. The magnitude of the threshold drop is increased by the body effect. Therefore, pass


transistors do not operate very well in nanometer processes where the threshold voltage is


a signiﬁcant fraction of the supply voltage. Fully complementary transmission gates should


be used where both 0s and 1s must be passed well.


Leakage current  Ideally, static CMOS gates draw zero current and dissipate zero power


when idle. Real gates draw some leakage current. The most important source at this time


is subthreshold leakage between source and drain of a transistor that should be cut off. The


subthreshold current of an OFF transistor decreases by an order of magnitude for every


60–100 mV that Vgs is below Vt . Threshold voltages have been decreasing, so subthreshold


leakage has been increasing dramatically. Some processes offer multiple choices of Vt : lowVt devices are used for high performance in critical circuits, while high-Vt devices are used


for low leakage elsewhere.


The transistor gate is a good insulator. However, signiﬁcant tunneling current ﬂows


through very thin gates. This has limited the scaling of gate oxide and led to new high-k


gate dielectrics.


Leakage current causes CMOS gates to consume power when idle. It also limits the


amount of time that data is retained in dynamic logic, latches, and memory cells. In


nanometer processes, dynamic logic and latches require some sort of feedback to prevent


data loss from leakage. Leakage increases at high temperature.


VDD Velocity saturation and mobility degradation result in less current than expected at


high voltage. This means that there is no point in trying to use a high VDD to achieve fast


transistors, so VDD has been decreasing with process generation to reduce power consumption. Moreover, the very short channels and thin gate oxides would be damaged by high


VDD.


Delay  Transistors in series drop part of the voltage across each transistor and thus experience smaller ﬁelds and less velocity saturation than single transistors. Therefore, series


transistors tend to be a bit faster than a simple model would predict. For example, two


nMOS transistors in series deliver more than half the current of a single nMOS transistor


of the same width. This effect is more pronounced for nMOS transistors than pMOS


transistors because nMOS transistors have higher mobility to begin with and thus are


more velocity saturated.


Matching  If two transistors should behave identically, both should have the same dimensions and orientation and be interdigitated if possible.


2.5 DC Transfer Characteristics


Digital circuits are merely analog circuits used over a special portion of their range. The DC transfer characteristics of a circuit relate the output voltage to the input voltage,assuming the input changes slowly enough that capacitances have plenty of time to charge or discharge. Speciﬁc ranges of input and output voltages are deﬁned as valid 0 and 1 logic levels. This section explores the DC transfer characteristics of CMOS gates and pass transistors.


88


2.5.1 Static CMOS Inverter DC Characteristics


Let us derive the DC transfer function (Vout vs. Vin) for the static CMOS inverter shown in Figure 2.25. We begin with Table 2.2, which outlines various regions of operation for the n- and p-transistors. In this table, Vtn is the threshold voltage of the n-channel device,and Vtp is the threshold voltage of the p-channel device. Note that Vtp is negative. The


equations are given both in terms of Vgs /Vds and Vin /Vout. As the source of the nMOS transistor is grounded, Vgsn = Vin and Vdsn = Vout. As the source of the pMOS transistor is tied to VDD, Vgsp = Vin – VDD and Vdsp = Vout – VDD.


The objective is to ﬁnd the variation in output voltage (Vout) as a function of the input voltage (Vin). This may be done graphically, analytically (see Exercise 2.16), or through simulation [Carr72]. Given Vin, we must ﬁnd Vout subject to the constraint that Idsn =|Idsp|. For simplicity, we assume Vtp = –Vtn and that the pMOS transistor is 2–3 times as wide as the nMOS transistor so n = p. We relax this assumption in Section 2.5.2.


We commence with the graphical representation of the simple algebraic equations described by EQ (2.10) for the two transistors shown in Figure 2.26(a). The plot shows Idsn and Idsp in terms of Vdsn and Vdsp for various values of Vgsn and Vgsp. Figure 2.26(b)shows the same plot of Idsn and |Idsp| now in terms of Vout for various values of Vin. The possible operating points of the inverter, marked with dots, are the values of Vout where Idsn = |Idsp| for a given value of Vin. These operating points are plotted on Vout vs. Vin axes in Figure 2.26(c) to show the inverter DC transfer characteristics. The supply current IDD= Idsn = |Idsp| is also plotted against Vin in Figure 2.26(d) showing that both transistors are momentarily ON as Vin passes through voltages between GND and VDD,  resulting in a pulse of current drawn from the power supply.


The operation of the CMOS inverter can be divided into ﬁve regions indicated on Figure 2.26(c). The state of each transistor in each region is shown in Table 2.3. In region A, the nMOS transistor is OFF so the pMOS transistor pulls the output to VDD. In region B, the nMOS transistor starts to turn ON, pulling the output down. In region C, both transistors are in saturation. Notice that ideal transistors are only in region C for Vin = VDD/2 and that the slope of the transfer curve in this example is –  in this region, corresponding to inﬁnite gain. Real transistors have ﬁnite output resistances on account of channel length modulation, described in Section 2.4.2, and thus have ﬁnite slopes over a broader region C. In region D, the pMOS transistor is partially ON and in region E, it is completely


TABLE 2.2  Relationships between voltages for the three regions of operation of a CMOS inverter


||Cutoff |Linear |Saturated |
|---|---|---|---|

|nMOS |Vgsn < Vtn |Vgsn > Vtn |Vgsn > Vtn |

|nMOS |Vin < Vtn |Vin > Vtn |Vin > Vtn |

|nMOS ||Vdsn < Vgsn – Vtn |Vdsn > Vgsn – Vtn |

|nMOS ||Vout < Vin – Vtn |Vout > Vin – Vtn |

|pMOS |Vgsp > Vtp |Vgsp < Vtp |Vgsp < Vtp |

|pMOS |Vin > Vtp + VDD |Vin < Vtp + VDD |Vin < Vtp + VDD |

|pMOS ||Vdsp > Vgsp – Vtp |Vdsp < Vgsp – Vtp |

|pMOS ||Vout > Vin – Vtp |Vout < Vin – Vtp |

5Idsn


Idsp


Vout


Vin


FIGURE 2.25


A CMOS inverter


2.5      DC Transfer Characteristics 89


OFF, leaving the nMOS transistor to pull the output down to GND. Also notice that the inverter’s current consumption is ideally zero, neglecting leakage, when the input is within a threshold voltage of the VDD or GND rails. This feature is important for low-power operation.


Figure 2.27 shows simulation results of an inverter from a 65 nm process. The


pMOS transistor is twice as wide as the nMOS transistor to achieve approximately


equal betas. Simulation matches the simple models reasonably well, although the transition is not quite as steep because transistors are not ideal current sources in saturation.


The crossover point where Vinv = Vin = Vout is called the input threshold. Because


both mobility and the magnitude of the threshold voltage decrease with temperature


for nMOS and pMOS transistors, the input threshold of the gate is only weakly


sensitive to temperature.


TABLE 2.3  Summary of CMOS inverter operation


|Region |Condition |p-device |n-device |Output |
|---|---|---|---|---|

|A |0 Vin < Vtn |linear |cutoff |Vout = VDD |

|B |Vtn Vin < VDD/2 |linear |saturated |Vout > VDD /2 |

|C |Vin = VDD/2 |saturated |saturated |Vout drops sharply |

|D |VDD /2 < Vin VDD – |Vtp| |saturated |linear |Vout < VDD/2 |

|E |Vin > VDD – |Vtp| |cutoff |linear |Vout = 0 |

Vgsn5


Vgsn4 Vgsn3 Vgsn2 Vgsn1


Vgsp5 Vgsp4 Vgsp3 Vgsp2 V。gsp1


–VDD


Vdsn


–Vdsp


–Idsp


Idsn


Vin5


Vin4 Vin3 Vin2 Vin1


Vin0


Vin1 Vin2 Vin3 Vin4


Idsn, |I    |dsp


IDD


Vtn


VDD–|Vtp|


VDD/2


FIGURE 2.26  Graphical derivation of CMOS inverter DC characteristic


0.0


0.0 0.2 0.4 0.6 0.8 1.0 Vin


FIGURE 2.27  Simulated CMOS  inverter DC characteristic


90


2.5.2 Beta Ratio Effects


We have seen that for p = n, the inverter threshold voltage Vinv is VDD/2. This may be desirable because it maximizes noise margins (see Section 2.5.3) and allows a capacitive load to charge and discharge in equal times by providing equal current source and sink capabilities (see Section 4.2). Inverters with different beta ratios r = p / n are called skewed inverters [Sutherland99]. If r > 1, the inverter is HI-skewed. If r < 1,the inverter is LO-skewed. If r = 1, the inverter has normal skew or is unskewed.


A HI-skew inverter has a stronger pMOS transistor. Therefore, if the input is VDD /2, we would expect the output will be greater than VDD /2. In other words, the input threshold must be higher than for an unskewed inverter. Similarly, a LO-skew inverter has a weaker pMOS transistor and thus a lower switching threshold.


Figure 2.28 explores the impact of skewing the beta ratio on the DC transfer characteristics. As the beta ratio is changed, the switching threshold moves. However, the output voltage transition remains sharp. Gates are usually skewed by adjusting the widths of transistors while maintaining minimum length for speed.


The inverter threshold can also be computed analytically. If the longchannel models of EQ (2.10) for saturated transistors are valid:


(2.54)


By setting the currents to be equal and opposite, we can solve for Vinv as a function of r :


(2.55)


In the limit that the transistors are fully velocity saturated, EQ (2.29) shows


(2.56)


Redeﬁning r = Wpvsat-p / Wnvsat-n, we can again ﬁnd the inverter threshold


(2.57)


In either case, if Vtn = –Vtp and r = 1, Vinv = VDD /2 as expected. However, velocity saturated inverters are more sensitive to skewing because their DC transfer characteristics are not as sharp.


DC transfer characteristics of other static CMOS gates can be understood by collapsing the gates into an equivalent inverter. Series transistors can be viewed as a single transistor of greater length. If only one of several parallel transistors is ON, the other I


dn


tn


dp


tp


β(


V Vr


+ ++


I W C v


=ox sat inv ox sat inv


tpV )


V Vrr


0.5 1 2


p n


= 10


= 0.1


FIGURE 2.28  Transfer characteristics of  skewed inverters


2.5      DC Transfer Characteristics 91


transistors can be ignored. If several parallel transistors are ON, the collection can be viewed as a single transistor of greater width.


2.5.3 Noise Margin


Noise margin is closely related to the DC voltage characteristics [Wakerly00]. This parameter allows you to determine the allowable noise voltage on the input of a gate so that the output will not be corrupted. The speciﬁcation most commonly used to describe noise margin (or noise immunity) uses two parameters: the LOW noise margin, NML, and the HIGH noise margin, NMH. With reference to Figure 2.29, NML is deﬁned as the difference in maximum LOW input voltage recognized by the receiving gate and the maximum LOW output voltage produced by the driving gate.


(2.58)


The value of NMH is the difference between the minimum HIGH output voltage of the driving gate and the minimum HIGH input voltage recognized by the receiving gate.


Thus,


(2.59)


VIH = minimum HIGH input voltage


VIL = maximum LOW input voltage


VOH= minimum HIGH output voltage


VOL = maximum LOW output voltage


Inputs between VIL and VIH are said to be in the indeterminate region or forbidden zone and do not represent legal digital logic levels. Therefore, it is generally desirable to have VIH as close as possible to VIL and for this value to be midway in the “logic swing,” VOL to VOH. This implies that the transfer characteristic should switch abruptly; that is, there should be high gain in the transition region. For the purpose of calculating noise margins,the transfer characteristic of the inverter and the deﬁnition of voltage levels VIL, VOL, VIH,and VOH are shown in Figure 2.30. Logic levels are deﬁned at the unity gain point where NM V VL IL OL=


NM V


H


OH


IH


Indeterminate


NML


NMH


Input Characteristics


Output Characteristics


VOH


VOL GND


VIH VIL


Logical High Input Range


Logical Low Input Range


Logical HighLogical High Output Range


Logical LowLogical Low Output Range


FIGURE 2.29  Noise margin deﬁnitions


92


the slope is –1. This gives a conservative bound on the worst case static noise margin [Hill68, Lohstroh83, Shepard99]. For the inverter shown, the NML is 0.46 VDD while the NMH is 0.13 VDD.


Note that the output is slightly degraded when the input is at its worst legal value; this is called noise feedthrough or propagated noise.


The exercises at the end of the chapter examine graphical and analytical approaches of ﬁnding the logic levels and noise margins.


If either NML or NMH for a gate are too small, the gate may be disturbed by noise that occurs on the inputs. An unskewed gate has equal noise margins, which maximizes immunity to arbitrary noise sources. If a gate sees more noise in the high or low input state, the gate can be skewed to improve that noise margin at the expense of the other. Note that if |Vtp| = Vtn , then NMH and NML increase as threshold voltages are increased.


Quite often, noise margins are compromised to improve speed.


Circuit examples in Chapter 9 will illustrate this trade-off. Noise sources tend to scale with the supply voltage, so noise margins are best given as a fraction of the supply voltage. A noise margin of 0.4 V is quite comfortable in a 1.8 V process, but marginal in a 5 V process.


DC analysis gives us the static noise margins specifying the level of noise that a gate may see for an indeﬁnite duration. Larger noise pulses may be acceptable if they are brief; these are described by dynamic noise margins speciﬁed by a maximum amplitude as a function of the duration [Lohstroh79, Somasekhar00]. Unfortunately,there is no simple amplitude-duration product that conveniently speciﬁes dynamic noise margins.


2.5.4 Pass Transistor DC Characteristics


Recall from Section 1.4.6 that nMOS transistors pass ‘0’s well but 1s poorly. We are now ready to better deﬁne “poorly.” Figure 2.31(a)shows an nMOS transistor with the gate and drain tied to VDD.


Imagine that the source is initially at Vs = 0. Vgs > Vtn, so the transistor is ON and current ﬂows. If the voltage on the source rises to Vs =VDD – Vtn, Vgs falls to Vtn and the transistor cuts itself OFF. Therefore, nMOS transistors attempting to pass a 1 never pull the source above VDD – Vtn.10 This loss is sometimes called a threshold drop.


Moreover, when the source of the nMOS transistor rises, Vsb becomes nonzero. As described in Section 2.4.3.1, this nonzero source to body potential introduces the body effect that increases the threshold voltage. Using the data from the example in that section, a pass transistor driven with VDD = 1 V would produce an output of only 0.65 V, potentially violating the noise margins of the next stage.


Similarly, pMOS transistors pass 1s well but 0s poorly. If the pMOS source drops below |Vtp|, the transistor cuts off. Hence,pMOS transistors only pull down to within a threshold above GND,as shown in Figure 2.31(b).


10Technically, the output can rise higher very slowly by means of subthreshold leakage.


VOL


VIL VIH


Unity Gain Points


Slope = −1


VDD – VDD


|Vtp|


βp/βn > 1


FIGURE 2.30  CMOS inverter noise margins


VDD VDD


Vs = VDD – Vtn


VDD – Vtn


VDD – Vtn VDD – Vtn


UVDD – Vtn VDD – 2Vtn(a)U


立GND


Vs = |Vtp|


FIGURE 2.31  Pass transistor  threshold drops


2.6      Pitfalls and Fallacies 93


As the source can rise to within a threshold voltage of the gate, the output of several transistors in series is no more degraded than that of a single transistor (Figure 2.31(c)).


However, if a degraded output drives the gate of another transistor, the second transistor can produce an even further degraded output (Figure 2.31(d)).


If we attempt to use a transistor as a switch, the threshold drop degrades the output voltage. In old processes where the power supply voltage was high and Vt was a small fraction of VDD, the drop was tolerable. In modern processes where Vt is closer to 1/3 of VDD,the threshold drop can produce an invalid or marginal logic level at the output. To solve this problem, CMOS switches are generally built using transmission gates.


Recall from Section 1.4.6 that a transmission gate consists of an nMOS transistor and a pMOS transistor in parallel with gates controlled by complementary signals. When the transmission gate is ON, at least one of the two transistors is ON for any output voltage and hence, the transmission gate passes both 0s and 1s well. The transmission gate is a fundamental and ubiquitous component in MOS logic. It ﬁnds use as a multiplexing element, a logic structure, a latch element, and an analog switch. The transmission gate acts as a voltage-controlled switch connecting the input and the output.


2.6 Pitfalls and Fallacies


This section lists a number of pitfalls and fallacies that can deceive the novice (or experienced) designer.


2.1 Consider an nMOS transistor in a 0.6 m process with W/L = 4/2  (i.e., 1.2/0.6  m). In this process, the gate oxide thickness is 100 Å and the mobility of electrons  is 350 cm2/V· s. The threshold voltage is 0.7 V. Plot Ids vs. Vds for Vgs = 0, 1, 2, 3, 4, and 5 V.


2.2 Show that the current through two transistors in series is equal to the current through  a single transistor of twice the length if the transistors are well described by the Shockley model. Speciﬁcally, show that IDS1 =


IDS2 in Figure 2.32 when the transistors are


in their linear region: VDS < VDD – Vt , VDD


> Vt (this is also true in saturation). Hint:


Express the currents of the series transistors in terms of V1 and solve for V1.


2.3 In Exercise 2.2, the body effect was


ignored. If the body effect is considered,


will IDS2 be equal to, greater than, or less


than IDS1? Explain.


VDS


IDS1


IDS2


V1


W/2L


W/L


FIGURE 2.32  Current in series transistors


96


2.4 A 90 nm long transistor has a gate oxide thickness of 16 Å. What is its gate capacitance per micron of width?


2.5 Calculate the diffusion parasitic Cdb of the drain of a unit-sized contacted nMOS  transistor in a 0.6 m process when the drain is at 0 and at VDD = 5 V. Assume the  substrate is grounded. The transistor characteristics are CJ = 0.42 fF/ m2, MJ =


0.44, CJSW = 0.33 fF/ m, MJSW = 0.12, and 0 = 0.98 V at room temperature.


2.6 Prove EQ (2.27).


2.7 Consider the nMOS transistor in a 0.6 m process with gate oxide thickness of 100 Å. The doping level is NA = 2 × 1017 cm–3 and the nominal threshold voltage is 0.7  V. The body is tied to ground with a substrate contact. How much does the threshold change at room temperature if the source is at 4 V instead of 0?


2.8 Does the body effect of a process limit the number of transistors that can be placed  in series in a CMOS gate at low frequencies?


2.9 Sometimes the substrate is connected to a voltage called the substrate bias to alter  the threshold of the nMOS transistors. If the threshold of an nMOS transistor is to  be raised, should a positive or negative substrate bias be used?


2.10 An nMOS transistor has a threshold voltage of 0.4 V and a supply voltage of VDD =


1.2 V. A circuit designer is evaluating a proposal to reduce Vt by 100 mV to obtain  faster transistors.


a) By what factor would the saturation current increase (at Vgs = Vds = VDD) if the


transistor were ideal?


b) By what factor would the subthreshold leakage current increase at room temperature at Vgs = 0? Assume n = 1.4.


c) By what factor would the subthreshold leakage current increase at 120 °C?


Assume the threshold voltage is independent of temperature.


2.11 Find the subthreshold leakage current of an inverter at room temperature if the


input A = 0. Let n = 2 p = 1 mA/V2, n = 1.0, and |Vt| = 0.4 V. Assume the body  effect and DIBL coefﬁcients are =


= 0.


2.12 Repeat Exercise 2.11 for a NAND gate built from unit transistors with inputs A = B = 0. Show that the subthreshold leakage current through the series transistors is half  that of the inverter if n = 1.


2.13 Repeat Exercises 2.11 and 2.12 when = 0.04 and VDD = 1.8 V, as in the case of a  more realistic transistor.  has a secondary effect, so assume that it is 0. Did the


leakage currents go up or down in each case? Is the leakage through the series transistors more than half, exactly half, or less than half of that through the inverter?


2.14 Peter Pitfall is offering to license to you his patented noninverting buffer circuit


shown in Figure 2.33. Graphically derive the transfer characteristics for this buffer. Assume n = p =  and Vtn = |Vtp| = Vt .  Why is it a bad circuit idea?


FIGURE 2.33


Noninverting buffer


Exercises 97


2.15 A novel inverter has the transfer characteristics shown in Figure 2.34. What  are the values of VIL, VIH, VOL, and VOH that give best noise margins? What are  these high and low noise margins?


2.16 Section 2.5.1 graphically determined the transfer characteristics of a static


CMOS inverter. Derive analytic expressions for Vout as a function of Vin for  regions B and D of the transfer function. Let |Vtp| = Vtn and p = n.


2.17 Using the results from Exercise 2.16, calculate the noise margin for a CMOS  inverter operating at 1.0 V with Vtn = |Vtp| = 0.35 V, p = n.


2.18 Repeat Exercise 2.16 if the thresholds and betas of the two transistors are not  necessarily equal. Also solve for the value of Vin for region C where both transistors are saturated.


2.19 Using the results from Exercise 2.18, calculate the noise margin for a CMOS  inverter operating at 1.0 V with Vtn = |Vtp| = 0.35 V, p = 0.5 n.


2.20 Give an expression for the output voltage for the pass transistor networks


shown in Figure 2.35. Neglect the body effect.


2.21 Suppose VDD = 1.2 V and Vt = 0.4 V. Determine Vout in Figure 2.36 for the    following. Neglect the body effect.


a) Vin = 0 V


b) Vin = 0.6 V


c) Vin = 0.9 V


d) Vin = 1.2 V.


(d)(b)


FIGURE 2.35  Pass transistor networks


0.3


0.9


1.2


FIGURE 2.34


Transfer characteristics


FIGURE 2.36


Single pass transistor


99


CMOS Processing Technology


3.1 Introduction


Chapter 1 summarized the steps in a basic CMOS process. These steps are expanded upon in this chapter. Where possible, the processing details are related to the way CMOS circuits and systems are designed. Modern CMOS processing is complex, and while coverage of every nuance is not within the scope of this book, we focus on the fundamental concepts that impact design.


A fair question from a designer would be “Why do I care how transistors are made?”In many cases, if designers understand the physical process, they will comprehend the reason for the underlying design rules and in turn use this knowledge to create a better design. Understanding the manufacturing steps is also important when debugging some difﬁcult chip failures and improving yield.


Fabrication plants, or fabs, are enormously expensive to develop and operate. In the early days of the semiconductor industry, a few bright physicists and engineers could bring up a fabrication facility in an industrial building at a modest cost and most companies did their own manufacturing. Now, a fab processing 300 mm wafers in a 45 nm process costs about $3 billion. The research and development underlying the technology costs another$2.4 billion. Only a handful of companies in the world have the sales volumes to justify such a large investment. Even these companies are forming consortia to share the costs of technology development with their market rivals. Some companies, such as TSMC,UMC, Chartered, and IBM operate on a foundry model, selling space on their fab line to fabless semiconductor ﬁrms. Figure 3.1 shows workers and machinery in the cavernous clean room at IBM’s East Fishkill 300 mm fab.


Recall that silicon in its pure or intrinsic state is a semiconductor, having bulk electrical resistance somewhere between that of a conductor and an insulator. The conductivity of silicon can be raised by several orders of magnitude by introducing impurity atoms into the silicon crystal lattice. These dopants can supply either free electrons or holes. Group III impurity elements such as boron that use up electrons are referred to as acceptors because they accept some of the electrons already in the silicon, leaving holes. Similarly,Group V donor elements such as arsenic and phosphorous provide electrons. Silicon that contains a majority of donors is known as n-type, while silicon that contains a majority of acceptors is known as p-type. When n-type and p-type materials are brought together, the region where the silicon changes from n-type to p-type is called a junction. By arranging junctions in certain physical structures and combining them with wires and insulators, various semiconductor devices can be constructed. Over the years, silicon semiconductor processing has evolved sophisticated techniques for building these junctions and other insulating and conducting structures.


Chapter 3      CMOS Processing Technology


The chapter begins with the steps of a generic process characteristic of commercial 65 nm manufacturing. It also surveys a variety of process enhancements that beneﬁt certain applications. The chapter examines layout design rules in more detail and discusses layout CAD issues such as design rule checking.


3.2 CMOS Technologies


CMOS processing steps can be broadly divided into two parts. Transistors are formed in the Front-End-of-Line (FEOL) phase, while wires are built in the Back-End-of-Line(BEOL) phase. This section examines the steps used through both phases of the manufacturing process.


3.2.1  Wafer Formation


The basic raw material used in CMOS fabs is a wafer or disk of silicon, roughly 75 mm to 300 mm (12––a dinner plate!) in diameter and less than 1 mm thick. Wafers are cut from boules, cylindrical ingots of single-crystal silicon, that have been pulled from a crucible of pure molten silicon. This is known as the Czochralski method and is currently the most common method for producing single-crystal material. Controlled amounts of impurities are added to the melt to provide the crystal with the required electrical properties. A seed crystal is dipped into the melt to initiate crystal growth. The silicon ingot takes on the same crystal orientation as the seed. A graphite radiator heated by radio-frequency induction surrounds the quartz crucible and maintains the temperature a few degrees above the melting point of silicon (1425 °C). The atmosphere is typically helium or argon to prevent the silicon from oxidizing.


The seed is gradually withdrawn vertically from the melt while simultaneously being rotated, as shown in Figure 3.2. The molten silicon attaches itself to the seed and recrystallizes as it is withdrawn. The seed withdrawal and rotation rates determine the diameter of the ingot. Growth rates vary from 30 to 180 mm/hour.


FIGURE 3.1  IBM, East Fishkill, NY fab (Courtesy of International  Business Machines Corporation. Unauthorized use not permitted.)


Si Boule


Molten Si


Crucible Heating


Coil 4


Pulling Member 14 Seed


Holder


Surface


FIGURE 3.2  Czochralski


system for growing Si boules


(Adapted from [Schulmann98].)


3.2      CMOS Technologies 101


3.2.2  Photolithography


Recall that regions of dopants, polysilicon, metal, and contacts are deﬁned using masks.


For instance, in places covered by the mask, ion implantation might not occur or the dielectric or metal layer might be left intact. In areas where the mask is absent, the implantation can occur, or dielectric or metal could be etched away. The patterning is achieved by a process called photolithography, from the Greek photo (light), lithos (stone),and graphe (picture), which literally means “carving pictures in stone using light.” The primary method for deﬁning areas of interest (i.e., where we want material to be present or absent) on a wafer is by the use of photoresists. The wafer is coated with the photoresist and subjected to selective illumination through the photomask. After the initial patterning of photoresist, other barrier layers such as polycrystalline silicon, silicon dioxide, or silicon nitride can be used as physical masks on the chip. This distinction will become more apparent as this chapter progresses.


A photomask is constructed with chromium (chrome) covered quartz glass. A UV light source is used to expose the photoresist. Figure 3.3 illustrates the lithography process.


The photomask has chrome where light should be blocked. The UV light ﬂoods the mask from the backside and passes through the clear sections of the mask to expose the organic photoresist (PR) that has been coated on the wafer. A developer solvent is then used to dissolve the soluble unexposed photoresist, leaving islands of insoluble exposed photoresist.


This is termed a negative photoresist. A positive resist is initially insoluble, and when exposed to UV becomes soluble. Positive resists provide for higher resolution than negative resists, but are less sensitive to light. As feature sizes become smaller, the photoresist layers have to be made thinner. In turn, this makes them less robust and more subject to failure which can impact the overall yield of a process and the cost to produce the chip.


The photomask is commonly called a reticle and is usually smaller than the wafer, e.g.,2 cm on a side. A stepper moves the reticle to successive locations to completely expose the wafer. Projection printing is normally used, in which lenses between the reticle and wafer focus the pattern on the wafer surface. Older techniques include contact printing, where the mask and wafer are in contact, and proximity printing, where the mask and wafer are close but not touching. The reticle can be the same size as the area to be patterned (1×) or larger. For instance, 2.5× and 5× steppers with optical reduction have been used in the industry.


Quartz Glass


Chrome Pattern Photomask


Wafer Gaps in


chrome allow UV through.


Photoresist is exposed where UV illuminates it.


UV light floods backside of mask.


Unexposed photoresist is


eventually removed by an appropriate solvent leaving the islands of


exposed


photoresist.


FIGURE 3.3  Photomasking with a negative resist (lens system between mask and wafer  omitted to improve clarity and avoid diffracting the reader )


102


The wavelength of the light source inﬂuences the minimum feature size that can be printed. Deﬁne the minimum pitch (width + spacing) of a process to be 2b. The resolution of a lens depends on the wavelength  of the light and the numerical aperture NA of the lens:


(3.1)


The numerical aperture is


(3.2)


where n is the refractive index of the medium (1 for air, 1.33 for water, and up to 1.5 for oil), and  is the angle of acceptance of the lens. Increasing  requires larger optics.


Lenses used in the 1970s had a numerical aperture of 0.2. Intel uses a numerical aperture of 0.92 for their 45 nm process [Mistry07]. Nikon and ASML broke the 1.0 barrier by introducing immersion lithography that takes advantage of water’s higher refractive index[Geppert04], and in 2008, NA = 1.35 had been reached. All of these advances have come at the expense of multimillion dollar optics systems. k1 depends on the coherence of the light, antireﬂective coatings, photoresist parameters, and resolution enhancement techniques. Presently, 0.8 is considered easy, while 0.5 is very hard.


The depth of focus is


(3.3)


where k2 ranges from 0.5 to 1. Advanced lithography systems with short wavelengths and large numerical apertures have a very shallow depth of focus, requiring that the surface of the wafer be maintained extremely ﬂat.


In the 1980s, mercury lamps with 436 nm or 365 nm wavelengths were used. At the


0.25 m process generation, excimer lasers with 248 nm (deep ultraviolet) were adopted and have been used down to the 180 nm node. Currently, 193 nm argon-ﬂuoride lasers are used for the critical layers down to the 45 nm node and beyond. The critical layers are those that deﬁne the device behavior. An example would be the gate (polysilicon), source/drain(diffusion), ﬁrst metal, and contact masks. With such a laser, a numerical aperture of 1.35,and k1 = 0.5, the best achievable pitch is 2b = 72 nm, corresponding to a polysilicon halfpitch of 36 nm. It is amazing that we can print features so much smaller than the wavelength of the light, but even so, lithography is becoming a serious problem at the 45 nm node and below.


Efforts to develop 157 nm deep UV lithography systems were unsuccessful and have been abandoned by the industry. In the future, 13.5 nm extreme ultraviolet (EUV) light sources may be used, but presently, these sources require prohibitively expensive reﬂective optics and vacuum processing and are not strong enough for production purposes. Some predict that EUV will be ready by 2011 or 2012, while others are skeptical [Mack08].


Wavelengths comparable to or greater than the feature size cause distortion in the patterns exposed on the photoresist. Resolution enhancement techniques (RETs) precompensate for this distortion so the desired patterns are obtained [Schellenberg03]. These techniques involve modifying the amplitude, phase, or direction of the incoming light. The 2


b k=


NA


NA = nsin


DOF


=k22


3.2      CMOS Technologies 103


ends of a line in a layout receive less light than the center, causing nonuniform exposure. Optical proximity correction (OPC) makes small changes to the patterns on the masks to compensate for these local distortions. Figure 3.4 shows an example of printing with and without optical proximity correction. OPC predistorts the corners to reduce undesired rounding. Phase shift masks (PSM)takes advantage of the diffraction grating effect of parallel lines on a mask,varying the thickness of the mask to change the phase such that light from adjacent lines are out of phase and cancel where no light is desired. Off-axis illumination can also improve contrast for certain types of dense, repetitive patterns. Double-patterning is a sequence of two precisely aligned exposure steps with different masks for the same photoresist layer [Mack08]. OPC became necessary at the 180 nm node and all of these techniques are in heavy use by the 45 nm node.


Each successive UV stepper is more expensive and the throughput of the stepper may decrease. This is just another contributory issue to the spiraling cost of chip manufacturing. The cost of masks is also skyrocketing, forcing chip designers to amortize design and mask expenses across the largest volume possible. This theme will be reinforced in Section 14.3.


3.2.3  Well and Channel Formation


The following are main CMOS technologies:


n-well process


p-well process


twin-well process


triple-well process


Silicon-on-insulator processes are also available through some manufacturers (see Section


3.4.1.2).


Chapter 1 outlined an n-well process. Historically, p-well processes preceded n-well processes. In a p-well process, the nMOS transistors are built in a p-well and the pMOS transistor is placed in the n-type substrate. p-well processes were used to optimize the pMOS transistor performance. Improved techniques allowed good pMOS transistors to be fabricated in an n-well and excellent nMOS transistors to be fabricated in the p-type substrate of an n-well process. In the n-well process, each group of pMOS transistors in an n-well shares the same body node but is isolated from the bodies of pMOS transistors in different wells. However, all the nMOS transistors on the chip share the same body, which is the substrate. Noise injected into the substrate by digital circuits can disturb sensitive analog or memory circuits. Twin-well processes accompanied the emergence of n-well processes. A twin-well process allows the optimization of each transistor type. A third well can be added to create a triple-well process. The triple-well process has emerged to provide good isolation between analog and digital blocks in mixed-signal chips; it is also used to isolate high-density dynamic memory from logic. Most fabrication lines provide a baseline twin-well process that can be upgraded to a triple-well process with the addition of a single mask level.


Wells and other features require regions of doped silicon. Varying proportions of donor and acceptor dopants can be achieved using epitaxy, deposition, or implantation.


Mask overlaid  with micrograph


FIGURE 3.4  Subwavelength features


printed with and without OPC. Predistortion  of corners in OPC reduces undesired


rounding. (Adapted from [Schellenberg98] with permission of SPIE.)


Epitaxy involves growing a single-crystal ﬁlm on the silicon surface (which is already a single crystal) by subjecting the silicon wafer surface to an elevated temperature and a source of dopant material.


Epitaxy can be used to produce a layer of silicon with fewer defects than the native wafer surface and also can help prevent latchup (see Section 7.3.6). Foundries may provide a choice of epi (with epitaxial layer) or non-epi wafers. Microprocessor designers usually prefer to use epi wafers for uniformity of device performance.


Deposition involves placing dopant material onto the silicon surface and then driving it into the bulk using a thermal diffusion step. This can be used to build deep junctions. A step called chemical vapor deposition (CVD) can be used for the deposition. As its name suggests, CVD occurs when heated gases react in the vicinity of the wafer and produce a product that is deposited on the silicon surface. CVD is also used to lay down thin ﬁlms of material later in the CMOS process.


Ion implantation involves bombarding the silicon substrate with highly energized donor or acceptor atoms. When these atoms impinge on the silicon surface, they travel below the surface of the silicon, forming regions with varying doping concentrations. At elevated temperature (>800 °C) diffusion occurs between silicon regions having different densities of impurities, with impurities tending to diffuse from areas of high concentration to areas of low concentration. Therefore, it is important to keep the remaining process steps at as low a temperature as possible once the doped areas have been put into place.


However, a high-temperature annealing step is often performed after ion implantation to redistribute dopants more uniformly. Ion implantation is the standard well and source/drain implant method used today. The placement of ions is a random process, so doping levels cannot be perfectly controlled, especially in tiny structures with relatively small numbers of dopant atoms. Statistical dopant ﬂuctuations lead to variations in the threshold voltage that will be discussed in Section 7.5.2.2.


Blindly trusting one’s models


Models should be viewed as only approximations to reality, not reality itself, and used within  their limitations. In particular, simple models like the Shockley or RC models aren’t even close  to accurate fits for the I-V characteristics of a modern transistor. They are valuable for the  insight they give on trends (i.e., making a transistor wider increases its gate capacitance and  decreases its ON resistance), not for the absolute values they predict. Cutting-edge projects  often target processes that are still under development, so these models should only be


viewed as speculative. Finally, processes may not be fully characterized over all operating regimes; for example, don’t assume that your models are accurate in the subthreshold region  unless your vendor tells you so. Having said this, modern SPICE models do an extremely good  job of predicting performance well into the GHz range for well-characterized processes and  models when using proper design practices (such as accounting for temperature, voltage, and  process variation).


Using excessively complicated models for manual calculations


Because models cannot be perfectly accurate, there is little value in using excessively complicated models, particularly for hand calculations. Simpler models give more insight on key


trade-offs and more rapid feedback during design. Moreover, RC models calibrated against


simulated data for a fabrication process can estimate delay just as accurately as elaborate


models based on a large number of physical parameters but not calibrated to the process.


Assuming a transistor with twice the drawn length has exactly half the current


To first order, current is proportional to W/L. In modern transistors, the effective transistor  length is usually shorter than the drawn length, so doubling the drawn length reduces current  by more than a factor of two. Moreover, the threshold voltage tends to increase for longer


transistors, resulting in less current. Therefore, it is a poor strategy to try to ratio currents by  ratioing transistor lengths.


94


Assuming two transistors in series deliver exactly half the current of a single transistor


To first order, this would be true. However, each series transistor sees a smaller electric field  across the channel and hence are each less velocity saturated. Therefore, two series transistors  in a nanometer process will deliver more than half the current of a single transistor. This is  more pronounced for nMOS than pMOS transistors because of the higher mobility and the


higher degree of velocity saturation of electrons than holes at a given field. Hence, NAND gates  perform better than first order estimates might predict.


Ignoring leakage


In contemporary processes, subthreshold and gate leakage can be quite significant. Leakage is  exacerbated by high temperature and by random process variations. Undriven nodes will not  retain their state for long; they will leak to some new voltage. Leakage power can account for  a large fraction of total power, especially in battery-operated devices that are idle most of the  time.


Using nMOS pass transistors


nMOS pass transistors only pull up to VDD – Vt. This voltage may fall below VIH of a receiver, especially as VDD decreases. For example, one author worked with a scan latch containing an  nMOS pass transistor that operated correctly in a 250 nm process at 2.5 V. When the latch was


ported to a 180 nm process at 1.8 V, the scan chain stopped working. The problem was traced


to the pass transistor and the scan chain was made operational in the lab by raising VDD to 2  V. A better solution is to use transmission gates in place of pass transistors.


Summary


In summary, we have seen that MOS transistors are four-terminal devices with a gate,source, drain, and body. In normal operation, the body is tied to GND or VDD so the transistor can be modeled as a three-terminal device. The transistor behaves as a voltagecontrolled switch. An nMOS switch is OFF (no path from source to drain) when the gate voltage is below some threshold Vt . The switch turns ON, forming a channel connecting source to drain, when the gate voltage rises above Vt . This chapter has developed more elaborate models to predict the amount of current that ﬂows when the transistor is ON.


The transistor operates in three modes depending on the terminal voltages:


Vgs < Vt


Ids  0


Vgs > Vt, Vds < Vdsat Linear


Ids increases with Vds (like a resistor)


Vgs > Vt, Vds > Vdsat Saturation


Ids constant (like a current source)


In a long-channel transistor, the saturation current depends on . pMOS transistors are similar to nMOS transistors, but have the signs reversed and deliver about half the current because of lower mobility.


In a real transistor, the I-V characteristics are more complicated. Modern transistors are extraordinarily small and thus experience enormous electric ﬁelds even at low voltage. The high ﬁelds cause velocity saturation and mobility degradation that lead to less current than you might otherwise expect. This can be modeled as a saturation current dependent on  ,where the velocity saturation index  is less than 2. Moreover, the saturation current does increase slightly with Vds because of channel length modulation. Although simple hand calculations are no longer accurate, the general shape does not change very much and the transfer characteristics can still be derived using graphical or simulation methods.


VGT2


VGT


Exercises 95


Even when the gate voltage is low, the transistor is not completely OFF. Subthreshold current through the channel drops off exponentially for Vgs < Vt , but is nonnegligible for transistors with low thresholds. Junction leakage currents ﬂow through the reverse-biased p–n junctions. Tunneling current ﬂows through the insulating gate when the oxide becomes thin enough.


We can derive the DC transfer characteristics and noise margins of logic gates using either analytical expressions or a graphical load line analysis or simulation. Static CMOS gates have excellent noise margins.


Unlike ideal switches, MOS transistors pass some voltage levels better than others.


An nMOS transistor passes 0s well, but only pulls up to VDD – Vtn when passing 1s. The pMOS passes 1s well, but only pulls down to |Vtp| when passing 0s. This threshold drop is exacerbated by the body effect, which increases the threshold voltage when the source is at a different potential than the body.


There are too many parameters in a modern BSIM model for a designer to deal with intuitively. Instead, CMOS transistors are usually characterized by the following basic ﬁgures of merit:


Target supply voltage


Lgate / Lpoly Effective channel length (< feature size) tox


Effective oxide thickness (a.k.a. EOT)


Idsat


Ids @ Vgs = Vds = VDD


Ioff


Ids @ Vgs = 0, Vds = VDD


Ig


Gate leakage @ Vgs = VDD


[Muller03] and [Tsividis99] offer comprehensive treatments of device physics at a more advanced level. [Gray01] describes MOSFET models in more detail from the analog designer’s point of view.


The ﬁrst step in most CMOS processes is to deﬁne the well regions. In a triple-well process, a deep n-well is ﬁrst driven into the p-type substrate, usually using high-energy Mega electron volt levels (MeV) ion implantation as opposed to a thermally diffused operation. This avoids the thermal cycling (i.e., the wafers do not have to be raised significantly in temperature), which improves throughput and reliability. A 2–3 MeV implantation can yield a 2.5–3.5 m deep n-well. Such a well has a peak dopant concentration just under the surface and for this reason is called a retrograde well. This can enhance device performance by providing improved latchup characteristics and reduced susceptibility to vertical punch-through (see Section 7.3.5). A thick (3.5–5.5 m) resist has to be used to block the high energy implantation where no well should be formed. Thick resists and deep implants necessarily lead to fairly coarse feature dimensions for wells, compared to the minimum feature size. Shallower n-well and p-well regions are then implanted. After the wells have been formed, the doping levels can be adjusted (using a threshold implant) to set the desired threshold voltages for both nMOS and pMOS transistors. With multiple threshold implant masks, multiple Vt  options can be provided on the same chip. For a given gate and substrate material, the threshold voltage depends on the doping level in the substrate (NA), the oxide thickness (tox), and the surface state charge (Qfc). The implant can affect both NA and Qfc and hence Vt . Figure 3.5 shows a typical triple-well structure.


As discussed, the nMOS transistor is situated in the p-well located in the deep n-well.


Other nMOS transistors could be built in different p-wells so that they do not share the same body node. Transistors in a p-well in a triple-well process will have different characteristics than transistors in the substrate because of the different doping levels. The pMOS


3.2      CMOS Technologies 105


transistors are located in the shallow (normal) n-well. The ﬁgure shows the cross-section of an inverter.


Wells are deﬁned by separate masks. In the case of a twin-well process, only one mask need be deﬁned because the other well by deﬁnition is its complement. Triple-well processes have to deﬁne at least two masks, one for the deep well and the other for either n-well or p-well.


Transistors near the edge of a retrograde well (e.g., within about 1 m) may have different threshold voltages than those far from the edge because ions scatter off the photoresist mask into the edge of the well, as shown in Figure 3.6 [Hook03]. This is called the well-edge proximity effect.


3.2.4 Silicon Dioxide (SiO2)


Many of the structures and manufacturing techniques used to make silicon integrated circuits rely on the properties of SiO2. Therefore, reliable manufacture of SiO2 is extremely important. In fact, unlike competing materials, silicon has dominated the industry because it has an easily processable oxide (i.e., it can be grown and etched). Various thicknesses of SiO2 may be required, depending on the particular process. Thin oxides are required for transistor gates; thicker oxides might be required for higher voltage devices, while even thicker oxide layers might be required to ensure that transistors are not formed unintentionally in the silicon beneath polysilicon wires (see the next section).


p+n-well


p-well


Deep n-well


FIGURE 3.5  Well structure in triple-well process


Substrate


Well


Resist


Scattering


Well Implant


FIGURE 3.6  Well-edge proximity effect, in which dopants scattering  off photoresist increase the doping level near the edge of a well


(© IEEE 2003.)


106


Oxidation of silicon is achieved by heating silicon wafers in an oxidizing atmosphere.


The following are some common approaches:


Wet oxidation––when the oxidizing atmosphere contains water vapor. The temperature is usually between 900 °C and 1000 °C. This is also called pyrogenic oxidation  when a 2:1 mixture of hydrogen and oxygen is used. Wet oxidation is a rapid


process.


Dry oxidation––when the oxidizing atmosphere is pure oxygen. Temperatures are  in the region of 1200 °C to achieve an acceptable growth rate. Dry oxidation forms  a better quality oxide than wet oxidation. It is used to form thin, highly controlled  gate oxides, while wet oxidation may be used to form thick ﬁeld oxides.


Atomic layer deposition (ALD)––when a thin chemical layer (material A )  is attached  to a surface and then a chemical (material B) is introduced to produce a thin layer  of the required layer (i.e., SiO2––this can also be used for other various dielectrics  and metals). The process is then repeated and the required layer is built up layer by  layer. [George96, Klaus98].


The oxidation process normally consumes part of the silicon wafer (deposition and ALD do not). Since SiO2 has approximately twice the volume of silicon, the SiO2 layer grows almost equally in both vertical directions. Thus, after processing, the SiO2 projects above and below the original unoxidized silicon surface.


3.2.5  Isolation


Individual devices in a CMOS process need to be isolated from one another so that they do not have unexpected interactions. In particular, channels should only be inverted beneath transistor gates over the active area; wires running elsewhere shouldn’t create parasitic MOS channels. Moreover, the source/drain diffusions of unrelated transistors should not interfere with each other.


The process ﬂow in Section 1.5 was historically used to provide this isolation. The transistor gate consists of a thin gate oxide layer. Elsewhere, a thicker layer of ﬁeld oxide separates polysilicon and metal wires from the substrate. The MOS sandwich formed by the wire, thick oxide, and substrate behaves as an unwanted parasitic transistor. However,the thick oxide effectively sets a threshold voltage greater than VDD that prevents the transistor from turning ON during normal operation. Actually, these ﬁeld devices can be used for I/O protection and are discussed in Section 13.6.2. The source and drain of the transistors form reverse-biased p–n junctions with the substrate or well, isolating them from their neighbors.


The thick oxide used to be formed by a process called Local Oxidation of Silicon(LOCOS). A problem with LOCOS-based processes is the transition between thick and thin oxide, which extended some distance laterally to form a so-called bird’s beak. The lateral distance is proportional to the oxide thickness, which limits the packing density of transistors.


Starting around the 0.35 m node, shallow trench isolation (STI) was introduced to avoid the problems with LOCOS. STI forms insulating trenches of SiO2 surrounding the transistors (everywhere except the active area). The trench width is independent of its depth, so transistors can be packed as closely as the lithography permits. The trenches isolate the wires from the substrate, preventing unwanted channel formation. They also reduce the sidewall capacitance and junction leakage current of the source and drain.


3.2      CMOS Technologies 107


STI starts with a pad oxide and a silicon nitride layer, which act as the masking layers,as shown in Figure 3.7. Openings in the pad oxide are then used to etch into the well or substrate region (this process can also be used for source/drain diffusion). A liner oxide is then grown to cover the exposed silicon (Figure 3.7(b)). The trenches are ﬁlled with SiO2 or other ﬁllers using CVD that does not consume the underlying silicon (Figure 3.7(c)).


The pad oxide and nitride are removed and a Chemical Mechanical Polishing (CMP) step is used to planarize the structure (Figure 3.7(d)). CMP, as its name suggests, combines a mechanical grinding action in which the rotating wafer is contacted by a stationary polishing head while an abrasive mixture is applied. The mixture also reacts chemically with the surface to aid in the polishing action. CMP is used to achieve ﬂat surfaces, which are of central importance in modern processes with many layers.


From the designer’s perspective, the presence of a deep n-well and/or trench isolation makes it easier to isolate noise-sensitive (analog or memory) portions of a chip from digital sections. Trench isolation also permits nMOS and pMOS transistors to be placed closer together because the isolation provides a higher source/drain breakdown voltage––the voltage at which a source or drain diode starts to conduct in the reverse-biased condition. The breakdown voltage must exceed the supply voltage (so junctions do not break down during normal operation) and is determined by the junction dimensions and doping levels of the junction formed. Deeper trenches increase the breakdown voltage.


3.2.6  Gate Oxide


The next step in the process is to form the gate oxide for the transistors. As mentioned,this is most commonly in the form of silicon dioxide (SiO2).


In the case of STI-deﬁned source/drain regions, the gate oxide is grown on top of the planarized structure that occurs at the stage shown in Figure 3.7(d). This is shown in


Silicon Nitride


Well or Active


Substrate or Buried Oxide


(a) Trench Etch


(b) Liner Oxidation


(c) Fill Trench with Dielectric


(d) CMP for Planarization


Pad Oxide


Trench


Substrate p-well


Trench Oxide


FIGURE 3.7  Shallow trench isolation


108


Figure 3.8. The oxide structure is called the gate stack. This term arises because current processes seldom use a pure SiO2 gate oxide, but prefer to produce a stack that consists of a few atomic layers, each 3–4 Å thick, of SiO2 for reliability, overlaid with a few layers of an oxynitrided oxide(one with nitrogen added). The presence of the nitrogen increases the dielectric constant, which decreases the effective oxide thickness (EOT); this means that for a given oxide thickness, it performs like a thinner oxide. Being able to use a thicker oxide improves the robustness of the process. This concept is revisited in Section 3.4.1.3.


Many processes in the 180 nm generation and beyond provide at least two oxide thicknesses, as will be discussed in Section 3.4.1.1 (thin for logic transistors and thick for I/O transistors that must withstand higher voltages). At the 65 nm node, the effective thickness of the thin gate oxide is only 10.5–15 Å.


3.2.7  Gate and Source/Drain Formations


When silicon is deposited on SiO2 or other surfaces without crystal orientation, it forms polycrystalline silicon, commonly called polysilicon or simply poly. An annealing process is used to control the size of the single crystal domains and to improve the quality of the polysilicon. Undoped polysilicon has high resistivity. The resistance can be reduced by implanting it with dopants and/or combining it with a refractory metal. The polysilicon gate serves as a mask to allow precise alignment of the source and drain on either side of the gate. This process is called a self-aligned polysilicon gate process. Aluminum could not be used because it would melt during formation of the source and drain.


As a historical note, early metal-gate processes ﬁrst diffused source and drain regions,and then formed a metal gate. If the gate was misaligned, it could fail to cover the entire channel and lead to a transistor that never turned ON. To prevent this, the metal gate had to overhang the source and drain by more than the alignment tolerance of the process.


This created large parasitic gate-to-source and gate-to-drain overlap capacitances that degraded switching speeds.


The steps to deﬁne the gate, source, and drain in a self-aligned polysilicon gate are as follows:


Grow gate oxide wherever transistors are required (area = source + drain + gate)––elsewhere there will be thick oxide or trench isolation (Figure 3.9(a))


Deposit polysilicon on chip (Figure 3.9(b))


Pattern polysilicon (both gates and interconnect) (Figure 3.9(c))


Etch exposed gate oxide—i.e., the area of gate oxide where transistors are required  that was not covered by polysilicon; at this stage, the chip has windows down to  the well or substrate wherever a source/drain diffusion is required (Figure 3.9(d)) Implant pMOS and nMOS source/drain regions (Figure 3.9(e))


The source/drain implant density is relatively low, typically in the range 1018–1020 cm–3 of impurity atoms. Such a lightly doped drain (LDD) structure reduces the electricﬁeld at the drain junction (the junction with the highest voltage), which improves the immunity of the device to hot electron damage (see Section 7.3.6) and suppresses shortchannel effects. The LDD implants are shallow and lightly doped, so they exhibit low


Gate Oxide


FIGURE 3.8  Gate oxide formation


3.2      CMOS Technologies 109


capacitance but high resistance. This reduces device performance somewhat because of the resistance in series with the transistor. Consequently, deeper, more heavily doped source/drain implants are needed in conjunction with the LDD implants to provide devices that combine hot electron suppression with low source/drain resistance. A silicon nitride(Si3N4) spacer along the edge of the gate serves as a mask to deﬁne the deeper diffusion regions, as shown in Figure 3.10(a). For in-depth coverage of various LDD structures, see[Ziegler02].


As mentioned, the polysilicon gate and source/drain diffusion have high resistance due to the resistivity of silicon and their extremely small dimensions. Modern processes form a surface layer of a refractory metal on the silicon to reduce the resistance. A refractory metal is one with a high melting point that will not be damaged during subsequent processing. Tantalum, nickel, molybdenum, titanium, or cobalt are commonly used. The metal is deposited on the silicon (speciﬁcally on the gate polysilicon and/or source/drain regions). A layer of silicide is formed when the two substances react at elevated temperatures. In a polycide process, only the gate polysilicon is silicided. In a silicide process (usually implemented as a self-aligned silicidization––from whence comes the synonymous


Poly Gate


Shallow n-Source/Drain


p-well p-well


Implantation


FIGURE 3.9  Gate and shallow source/drain deﬁnition


110


term salicide) both gate polysilicon and source/drain regions are silicided. This process lowers the resistance of the polysilicon interconnect and the source and drain diffusion. Figure 3.10(b) shows the resultant structure with gate and source/drain regions silicided. In addition, SiO2 or an alternative dielectric has been used to cover all areas prior to the next processing steps. The ﬁgure shows a resulting structure with some vertical topology typical of older processes. The rapid transitions in surface height can lead to breaks in subsequent layers that fail to conform, or can entail a plethora of design rules that relate to metal edges. To avoid these problems, a CMP step is used to planarize the dielectric, leaving a ﬂat surface for metallization as shown in Figure 3.10(c).


Nanometer processes involve another implantation step called halo doping that increases the doping of the substrate or well near the ends of the channels. The halo doping alleviates DIBL, short channel effects, and punchthrough but increases GIDL and BTBT leakage at the junction between the diffusion and channel [Roy03].


3.2.8  Contacts and Metallization


Contact cuts are made to source, drain, and gate according to the contact mask. These are holes etched in the dielectric after the source/drain step discussed in the previous section.


Older processes commonly use aluminum (Al) for wires, although newer ones offer copper(Cu) for lower resistance. Tungsten (W) can be used as a plug to ﬁll the contact holes (to alleviate problems of aluminum not conforming to small contacts). In some processes, the tungsten can also be used as a local interconnect layer.


Metallization is the process of building wires to connect the devices. As mentioned previously, conventional metallization uses aluminum. Aluminum can be deposited either


SiN Spacer


Deep Source/Drain Diffusion


Polished Dielectric


Dielectric Silicide


LDD


FIGURE 3.10  Transistor with LDD and deep diffusion, salicide, and planarized dielectric


3.2      CMOS Technologies 111


by evaporation or sputtering. Evaporation is performed by passing


a high electrical current through a thick aluminum wire in a vacuum chamber. Some of the aluminum atoms are vaporized and


deposited on the wafer. An improved form of evaporation that


suffers less from contamination focuses an electron beam at a


container of aluminum to evaporate the metal. Sputtering is


achieved by generating a gas plasma by ionizing an inert gas


using an RF or DC electric ﬁeld. The ions are focused on an aluminum target and the plasma dislodges metal atoms, which are


then deposited on the wafer.


Wet or dry etching can be used to remove unwanted metal.


Piranha solution is a 3:1 to 5:1 mix of sulfuric acid and hydrogen


peroxide that is used to clean wafers of organic and metal contaminants or photoresist after metal patterning. Plasma etching


is a dry etch process with ﬂuorine or chlorine gas used for metallization steps. The plasma charges the etch gas ions, which are


attracted to the appropriately charged silicon surface. Very sharp etch proﬁles can be achieved using plasma etching. The result of the contact and metallization patterning steps is shown in Figure 3.11.


Subsequent intermetal vias and metallization are then applied. Some processes offer uniform metal dimensions for levels 2 to n–1, where n is the top level of metal. The top level is normally a thicker layer for use in power distribution and as such has relaxed width and spacing constraints. Other processes use successively thicker and wider metal for the upper layers, as will be explored in Section 6.1.2.


Polysilicon over diffusion normally forms a transistor gate, so a short metal1 wire is necessary to connect a diffusion output node to a polysilicon input. Some processes add tungsten (W) layer above polysilicon and below metal1; this layer is called local interconnect and can be drawn on a ﬁner pitch than metal1. Local interconnect offers denser cell layouts, especially in static RAMs. Figure 3.12 shows a scanning electron micrograph of a partially completed SRAM array. The oxide has been removed to show the diffusion,polysilicon, local interconnect, and metal1. Local interconnect is used to connect the nMOS and pMOS transistors without rising up to metal1. SRAM cells are discussed further in Section 12.2.


metal1 V


Contact Stud


Polysilicon Wordline


Local interconnect between n and p diffusion


n-diffusion


Unit Cell


FIGURE 3.12  Partially completed 6-transistor SRAM array using local interconnect (Courtesy of International Business Machines Corporation. Unauthorized use not  permitted.)


p-well metal1


G


FIGURE 3.11  Aluminum metallization


112


Contemporary logic processes use copper interconnects and low-k dielectrics to reduce wire resistance and capacitance. These enhancements are discussed in Section


3.4.2.


Figure 3.13 shows a cross-section of an IBM microprocessor showing the 11 layers of metal in a 90 nm process. The bottom level is tungsten local interconnect. The next ﬁve layers are on a 1× width and thickness (0.12 m width and spacing). Metal 6–8 are on a 2×width, spacing, and thickness and metal 9–10 are 4×. These ten layers use copper wires with low-k dielectrics. The top level is aluminum and is primarily used for I/O pads. The local interconnect and metal1 are used in both directions, while the upper layers are used in alternating preferred directions. A pair of vias between metal 9 and 10 are visible. The interfaces between dielectric levels after each step of CMP are also visible.


Figure 3.14 shows a micrograph in which the oxide between metal layers has been stripped away to reveal the complex three-dimensional structure of chip wiring.


3.2.9  Passivation


The ﬁnal processing step is to add a protective glass layer called passivation or overglass that prevents the ingress of contaminants. Openings in the passivation layer, called overglass cuts, allow connection to I/O pads and test probe points if needed. After passivation,further steps can be performed such as bumping, which allows the chip to be directly connected to a circuit board using plated solder bumps in the pad openings.


3.2.10  Metrology


Metrology is the science of measuring. Everything that is built in a semiconductor process has to be measured to give feedback to the manufacturing process. This ranges from simple optical measurements of line widths to advanced techniques to measure thin ﬁlms and defects such as voids in copper interconnect. A natural requirement exists for in situ


FIGURE 3.13  Cross-section showing 11 levels of


metallization (Courtesy of International Business Machines  Corporation. Unauthorized use not permitted.)


FIGURE 3.14  Micrograph of metallization in  six-layer copper process (Courtesy of International Business Machines Corporation.


Unauthorized use not permitted.)


3.3      Layout Design Rules 113


real-time measurements so that the manufacturing process can be controlled in a direct feedback manner.


Optical microscopes are used to observe large structures and defects, but are no longer adequate for structures smaller than the wavelength of visible light (~0.5 m).


Scanning electron microscopy (SEM) is used to observe very small features. An SEM raster scans a structure under observation and observes secondary electron emission to produce an image of the surface of the structure. Energy Dispersive Spectroscopy (EDX)bombards a circuit with electrons causing x-ray emission. This can be used for imaging as well. A Transmission Electron Microscope (TEM), which observes the results of passing electrons through a sample (rather than bouncing them off the sample), is sometimes also used to measure structures.


3.3 Layout Design Rules


Layout rules, also referred to as design rules, were introduced in Chapter 1 and can be considered a prescription for preparing the photomasks that are used in the fabrication of integrated circuits. The rules are deﬁned in terms of feature sizes (widths), separations, and overlaps. The main objective of the layout rules is to build reliably functional circuits in as small an area as possible. In general, design rules represent a compromise between performance and yield. The more conservative the rules are, the more likely it is that the circuit will function. However, the more aggressive the rules are, the greater the opportunity for improvements in circuit performance and size.


Design rules specify to the designer certain geometric constraints on the layout artwork so that the patterns on the processed wafer will preserve the topology and geometry of the designs. It is important to note that design rules do not represent some hard boundary between correct and incorrect fabrication. Rather, they represent a tolerance that ensures high probability of correct fabrication and subsequent operation. For example, you may ﬁnd that a layout that violates design rules can still function correctly and vice versa.


Nevertheless, any signiﬁcant or frequent departure (design rule waiver) from design rules will seriously prejudice the success of a design.


Chapter 1 described a version of design rules based on the MOSIS CMOS scalable rules. The MOSIS rules are expressed in terms of . These rules allow some degree of scaling between processes, as in principle, you only need to reduce the value of  and the designs will be valid in the next process down in size. Unfortunately, history has shown that processes rarely shrink uniformly. Thus, industry usually uses the actual micron design rules for layouts. At this time, custom layout is usually constrained to a number of often-used standard cells or memories, where the effort expended is amortized over many instances. Only for extremely high-volume chips is the cost savings of a smaller fullcustom layout worth the labor cost of that layout.


3.3.1  Design Rule Background


We begin by examining the reasons for the most important design rules.


3.3.1.1 Well Rules  The n-well is usually a deeper implant (especially a deep n-well) than the transistor source/drain implants, and therefore, it is necessary to provide sufﬁcient clearance between the n-well edges and the adjacent n+ diffusions. The clearance between the well edge and an enclosed diffusion is determined by the transition of the ﬁeld oxide


114


across the well boundary. Processes that use STI may permit zero inside clearance. In older LOCOS processes, problems such as the bird’s beak effect usually force substantial clearances. Being able to place nMOS and pMOS transistors closer together can signiﬁcantly reduce the size of SRAM cells.


Because the n-well sheet resistance can be several k  per square, it is necessary to ground the well thoroughly by providing a sufﬁcient number of well taps. This will prevent excessive voltage drops due to well currents. Guidelines on well and substrate taps are given in Section 7.3.6. Where wells are connected to different potentials (say in analog circuits), the spacing rules may differ from equipotential wells (all wells at the same voltage––the normal case in digital logic).


Mask Summary: The masks encountered for well speciﬁcation may include n-well,p-well, and deep n-well. These are used to specify where the various wells are to be placed.


Often only one well is speciﬁed in a twin-well process (i.e., n-well) and by default the p-well is in areas where the n-well isn’t (i.e., p-well equals the logical NOT of the n-well).


3.3.1.2 Transistor Rules  CMOS transistors are generally deﬁned by at least four physical masks. These are active (also called diffusion, diff, thinox, OD, or RX), n-select (also called n-implant, nimp, or nplus), p-select (also called p-implant, pimp, or pplus) and polysilicon(also called poly, polyg, PO, or PC). The active mask deﬁnes all areas where either n- or ptype diffusion is to be placed or where the gates of transistors are to be placed. The gates of transistors are deﬁned by the logical AND of the polysilicon mask and the active mask, i.e.,where polysilicon crosses diffusion. The select layers deﬁne what type of diffusion is required. n-select surrounds active regions where n-type diffusion is required. p-select surrounds areas where p-type diffusion is required. n-diffusion areas inside p-well regions deﬁne nMOS transistors (or n-diffusion wires). n-diffusion areas inside n-well regions deﬁne n-well contacts. Likewise, p-diffusion areas inside n-wells deﬁne pMOS transistors(or p-diffusion wires). p-diffusion areas inside p-wells deﬁne substrate contacts (or p-well contacts). Frequently, design systems will deﬁne only n-diffusion (ndiff ) and p-diffusion(pdiff ) to reduce the complexity of the process. The appropriate selects are generated automatically. That is, ndiff will be converted automatically into active with an overlapping rectangle or polygon of n-select.


It is essential for the poly to cross active completely; otherwise the transistor that has been created will be shorted by a diffusion path between source and drain. Hence, poly is required to extend beyond the edges of the active area. This is often termed the gate extension. Active must extend beyond the poly gate so that diffused source and drain regions exist to carry charge into and out of the channel. Poly and active regions that should not form a transistor must be kept separated; this results in a spacing rule from active to polysilicon.


Figure 3.15(a) shows the mask construction for the ﬁnal structures that appear in Figure 3.15(b).


Mask Summary: The basic masks (in addition to well masks) used to deﬁne transistors,diffusion interconnect (possibly resistors), and gate interconnect are active, n-select, p-select,and polysilicon. These may be called different names in some processes. Sometimes n-diffusion (ndiff ) and p-diffusion (pdiff ) masks are used in place of active to alleviate designer confusion.


3.3.1.3 Contact Rules  There are several generally available contacts:


Metal to p-active (p-diffusion)


Metal to n-active (n-diffusion)


3.3      Layout Design Rules 115


Metal to polysilicon


Metal to well or substrate


Depending on the process, other contacts such as buried polysilicon-active contacts may be allowed for local interconnect.


Because the substrate is divided into well regions, each isolated well must be tied to the appropriate supply voltage; i.e., the n-well must be tied to VDD and the substrate or p-well must be tied to GND with well or substrate contacts. As mentioned in Section 1.5.1, metal makes a poor connection to the lightly doped substrate or well. Hence, a heavily doped active region is placed beneath the contact, as shown at the source of the nMOS transistor in Figure 3.16.


Whenever possible, use more than one contact at each connection. This signiﬁcantly improves yield in many processes because the connection is still made even if


one of the contacts is malformed.


Mask Summary: The only mask involved with contacts to active or poly


is the contact mask, commonly called CONT or CA. Contacts are normally of


uniform size to allow for consistent etching of very small features.


3.3.1.4 Metal Rules Metal spacing may vary with the width of the metal line


(so called fat-metal rules). That is, above some metal wire width, the minimum spacing may be increased. This is due to etch characteristics of small versus large metal wires. There may also be maximum metal width rules. That is,


single metal wires cannot be greater than a certain width. If wider wires are


desired, they are constructed by paralleling a number of smaller wires and


n-select


p-select


Active


Poly


p-diffusion


p-transistor Well Contact


n-transistor


Substrate Contact


Gate Extension


FIGURE 3.15  CMOS n-well process transistor and well/substrate contact construction


n+Substrate Contact


FIGURE 3.16  Substrate contact


116


adding checkerboard links to tie the wires together. Additionally, there may be spacing rules that are applied to long, closely spaced parallel metal lines.


Older nonplanarized processes required greater width and spacing on upper-level metal wires (e.g., metal3) to prevent breaks or shorts between adjoining wires caused by the vertical topology of the underlying layers. This is no longer a consideration for modern planarized processes. Nevertheless, width and spacing are still greater for thicker metal layers.


Mask Summary: Metal rules may be complicated by varying spacing dependent on width: As the width increases, the spacing increases. Metal overlap over contact might be zero or nonzero. Guidelines will also exist for electromigration, as discussed in Section


7.3.3.1.


3.3.1.5 Via Rules Processes may vary in whether they allow stacked vias to be placed over polysilicon and diffusion regions. Some processes allow vias to be placed within these areas, but do not allow the vias to straddle the boundary of polysilicon or diffusion. This results from the sudden vertical topology variations that occur at sublayer boundaries.


Modern planarized processes permit stacked vias, which reduces the area required to pass from a lower-level metal to a high-level metal.


Mask Summary: Vias are normally of uniform size within a layer. They may increase in size toward the top of a metal stack. For instance, large vias required on power busses are constructed from an array of uniformly sized vias.


3.3.1.6 Other Rules The passivation or overglass layer is a protective layer of SiO2 (glass)that covers the ﬁnal chip. Appropriately sized openings are required at pads and any internal test points.


Some additional rules that might be present in some processes are as follows:


Extension of polysilicon or metal beyond a contact or via


Differing gate poly extensions depending on the device length


Maximum width of a feature


Minimum area of a feature (small pieces of photoresist can peel off and ﬂoat away) Minimum notch sizes (small notches are rarely beneﬁcial and can interfere with  resolution enhancement techniques)


3.3.1.7 Summary Whereas earlier processes tended to be process driven and frequently had long and involved design rules, processes have become increasingly “designer friendly”or, more speciﬁcally, computer friendly (most of the mask geometries for designs are algorithmically produced). Companies sometimes create “generic” rules that span a number of different CMOS foundries that they might use. Some processes have design guidelines that feature structures to be avoided to ensure good yields. Traditionally, engineers followed yield-improvement cycles to determine the causes of defective chips and modify the layout to avoid the most common systematic failures. Time to market and product life cycles are now so short that yield improvement is only done for the highest volume parts.


It is often better to reimplement a successful product in a new, smaller technology rather than to worry about improving the yield on the older, larger process.


3.3.2  Scribe Line and Other Structures


The scribe line surrounds the completed chip where it is cut with a diamond saw. The construction of the scribe line varies from manufacturer to manufacturer. It is designed to


3.3      Layout Design Rules 117


prevent the ingress of contaminants from the side of the chip (as opposed to the top of the chip, which is protected by the overglass).


Several other structures are included on a mask including the alignment mark, critical dimension structures, vernier structures, and process check structures [Hess94]. The mask alignment mark is usually placed by the foundry to align one mask to the next. Critical dimension test structures can be measured after processing to check proper etching of narrow polysilicon or metal lines. Vernier structures are used to judge the alignment between layers. A vernier is a set of closely spaced parallel lines on two layers. Misalignment between the two layers can be judged by the alignment of the two verniers. Test structures such as chains of contacts and vias, test transistors, and ring oscillators are used to evaluate contact resistance and transistor parameters. Often these structures can be placed along the scribe line so they do not consume useful wafer area.


3.3.3  MOSIS Scalable CMOS Design Rules


Class project designs often use the -based scalable CMOS design rules from MOSIS because they are simple and freely available. MOSIS once offered a wide variety of processes, from 2 m to 180 nm, compatible with the scalable CMOS rules. Indeed, MOSIS also supports three variants of these rules: SCMOS, SUBM, and DEEP, which are progressively more conservative to support feature sizes down to 180 nm. Chips designed in the conservative DEEP rules could be fabricated on any of the MOSIS processes.


As time has passed, the older processes became obsolete and the newer processes have too many nuances to be compatible with scalable design rules. The MOSIS processes most commonly used today are the ON Semiconductor (formerly AMI) 0.5 m process and the IBM 130, 90, 65, and 45 nm processes.


The 0.5 m process is popular for university class projects because MOSIS Educational Program offers generous grants to cover fabrication costs for 1.5 mm × 1.5 mm“TinyChips.” The best design rules for this process are the scalable SUBM rules1 using= 0.3 m. Thus, a TinyChip is 5000 × 5000 . Polysilicon is drawn at 2 = 0.6 m,then biased by MOSIS by 0.1 m prior to mask generation to give a true 0.5 m gate length. When simulating circuits, be sure to use the biased channel lengths to  model the transistor behavior accurately. In SPICE, the XL parameter is added to the speciﬁed transistor length to ﬁnd the actual length. Thus, a SPICE deck could specify a drawn channel length of L = 0.6 m for each transistor and include XL = 0.1 m in the model ﬁle to indicate a biased length of 0.5 m. There is a tutorial at www.cmosvlsi.com on designing in this process with the Electric CAD tool suite. [Brunvand09] explains how to design in this process with the Cadence and Synopsys tool suites; this ﬂow has a steeper learning curve but better mirrors industry practices.


Credible research chips need more advanced processes to reﬂect contemporary design challenges. The IBM processes are presently discounted for universities, and MOSIS offers certain research grants as well. The best way to design in these processes is with the Cadence and Synopsys tools using IBM’s proprietary micron-based design rules. The design ﬂow is presently poorly documented by MOSIS and ranges from difﬁcult at the 130 nm node to worse at deeper nodes. Unfortunately, this presently limits access to these processes to highly sophisticated research groups.


1Technically, MOSIS has two sets of contact rules [MOSIS09]. The standard rules require polysilicon and active to overlap contacts by 1.5 . Half-lambda rules reduce productivity because they force the designer off a  grid. The “alternate contact rules” are preferable because they require overlap by 1 , at the expense of more conservative spacing rules; these alternate rules are used in the examples in this text.


118


Section 1.5.3 introduced the SCMOS design rules. More extensive rules are illustrated and summarized on the inside back cover. Layouts consist of a set of rectangles on various layers such as polysilicon or metal. Width is the minimum width of a rectangle on a particular layer. Spacing is the minimum spacing between two rectangles on the same or different layers. Overlap speciﬁes how much a rectangle must surround another on another layer. Dimensions are all speciﬁed in  except for overglass cuts that do not scale well because they must contact large bond wires or probe tips. Select layers are often generated automatically and thus are not shown in the layout. If the active layer satisﬁes design rules,the select will too.


Contacts and vias must be exactly 2 × 2 . Larger connections are made from arrays of small vias to prevent current crowding at the periphery. The spacing rules of polysilicon or diffusion to arrays of multiple contacts is slightly larger than that to a single contact.


Section 1.5.5 estimated the pitch of lower-level metal to be 8 : 4  for the width and 4  for spacing. Technically, the minimum width and spacing are 3 , but the minimum metal contact size is 2 × 2  plus 1  surround on each side, for a width of 4 . Thus, the pitch for contacted metal lines can be reduced to 7 . Moreover, if the lines are drawn at 3  and the contacts are staggered so two adjacent lines never have adjacent contacts, the pitch reduces to 6.5 . Nevertheless, using a pitch of 8  for planning purposes is good practice and leaves a bit of “wiggle room” to solve difﬁcult layout problems.


3.3.4  Micron Design Rules


Table 3.1 lists a set of micron design rules for a hypothetical 65 nm process representing an amalgamation of several real processes. Rule numbers reference the diagram on the inside back cover. Observe that the rules differ slightly but not immensely from lambdabased rules with = 0.035 m. A complete set of micron design rules in this generationﬁlls hundreds of pages. Note that upper level metal rules are highly variable depending on the metal thickness; thicker wires require greater widths and spacings and bigger vias.


TABLE 3.1  Micron design rules for 65 nm process Layer


Rule


65 nm Rule


( m)


Width


0.5


Spacing to well at different potential


0.7


Spacing to well at same potential


(diffusion)


2.1


0.10


2.2


Spacing to active


0.12


2.3


Source/drain surround by well


0.15


2.4


Substrate/well contact surround by well


2.5


Spacing to active of opposite type


0.25


3.1


0.065


3.2


Spacing to poly over ﬁeld oxide


3.2a


Spacing to poly over active


3.3


Gate extension beyond active


3.4


Active extension beyond poly


3.5


Spacing of poly to active


0.07


3.4      CMOS Process Enhancements 119


3.4 CMOS Process Enhancements


3.4.1  Transistors


3.4.1.1 Multiple Threshold Voltages and Oxide Thicknesses  Some processes offer multiple threshold voltages and/or oxide thicknesses. Low-threshold transistors deliver more ON current, but also have greater subthreshold leakage. Providing two or more thresholds permits the designer to use low-Vt devices on critical paths and higher-Vt devices elsewhere to limit leakage power. Multiple masks and implantation steps are used to set the various thresholds. Alternatively, transistors with slightly longer channels can be used; these transistors naturally have higher thresholds because of the short channel effect (see Section


2.4.3.3) [Rohrer05].


Thin gate oxides also permit more ON current. However, they break down when exposed to the high voltages needed in I/O circuits. Oxides thinner than about 15 Å also


Layer


Select


4.1


Spacing from substrate/well contact to gate


4.2


Overlap of active


4.3


Overlap of substrate/well contact


4.4


Spacing to select


0.20


Contact(to poly or active)


5.1, 6.1


Width (exact)


0.08


5.2b, 6.2b Overlap by poly or active


5.3, 6.3


Spacing to contact


5.4


Spacing to gate


7.1


0.09


7.2


Spacing to well metal1


7.3, 8.3


Overlap of contact or via


7.4


Spacing to metal for lines wider than 0.5 m


0.30


Via1–Via6 8.1, 14.1, … Width (exact)


8.2, 14.2, … Spacing to via on same layer


Metal2–Metal7


9.1, …


9.2, …


Spacing to same layer metal


9.3, …


Overlap of via


9.4, …


Via7–8


Spacing


Metal8–9


0.40


Spacing to metal for lines wider than 1.0 m


0.50


TABLE 3.1  Micron design rules for 65 nm process (continued)


120


contribute to large gate leakage currents. Many processes offer a second,thicker oxide for the I/O transistors (see Section 13.6). For example, 3.3 V I/O circuits commonly use 0.35 m channel lengths and 7 nm gate oxides.


When gate leakage is a problem and high-k dielectrics are unavailable, an intermediate oxide thickness may also be provided to reduce leakage. Again,multiple masks are used to deﬁne the different oxides.


3.4.1.2 Silicon on Insulator A variant of CMOS that has been available for many years is Silicon on Insulator (SOI). As the name suggests, this is a process where the transistors are fabricated on an insulator. SOI stands in contrast to conventional bulk processes in which the transistors are fabricated on a conductive substrate. Two main insulators are used: SiO2 and sapphire. One major advantage of an insulating substrate is the elimination of the capacitance between the source/drain regions and body, leading to higher-speed devices. Another major advantage is lower subthreshold leakage due to steeper subthreshold slope resulting from a smaller n in EQ (2.44). The drawbacks are time-dependent threshold variations caused by the ﬂoating body.


Figure 3.17 shows two common types of SOI. Figure 3.17(a) illustrates a sapphire substrate. In this technology (for example, Peregrine Semiconductor’s UltraCMOS), a thin layer of silicon is formed on the sapphire surface. The thin layer of silicon is selectively doped to deﬁne different threshold transistors. Gate oxide is grown on top of this and then polysilicon gates are deﬁned. Following this, the nMOS and pMOS transistors are formed by implantation. Figure 3.17(b) shows a silicon-based SOI process. Here, a silicon substrate is used and a buried oxide (BOX) is grown on top of the silicon substrate. A thin silicon layer is then grown on top of the buried oxide and this is selectively implanted to form nMOS and pMOS transistor regions. Gate, source, and drain regions are then deﬁned in a similar fashion to a bulk process. Sapphire is optically and RF transparent. As such, it can be of use in optoelectronic areas when merged with III-V based light emitters.


SOI devices and circuits are discussed further in Section 9.5.


3.4.1.3 High-k Gate Dielectrics MOS transistors need high gate capacitance to attract charge to the channel. This leads to very thin SiO2 gate dielectrics (e.g., 10.5–12 Å,merely four atomic layers, in a 65 nm process). Gate leakage increases unacceptably below these thicknesses, which brings an end to classical scaling [Bai04]. Simple SiO2 has a dielectric constant of k = 3.9. As shown in EQ (2.2), gates could use thicker dielectrics and hence leak less if a material with a higher dielectric constant were available.


A ﬁrst step in this direction was the introduction of nitrogen to form oxynitride gate dielectrics, called SiON, around the 130 nm generation, providing k of about 4.1–4.2.


High-k dielectrics entered commercial manufacturing in 2007, ﬁrst with a hafnium-based material in Intel’s 45 nm process [Auth08]. Hafnium oxide (HfO2) has k = 20.


A depletion region forms at the interface of polysilicon and the gate dielectric. This effectively increases tox, which is undesirable for performance. Moreover, polysilicon gates can be incompatible with high-k dielectrics because of effects such as threshold voltage pinning and phonon scattering, which make it difﬁcult to obtain low thresholds and reduce the mobility. The Intel 45 nm process returned to metal gates to solve these problems and also to reduce gate resistance, as shown in Figure 3.18 [Mistry07]. Thus, the term MOS is


Sapphire


Buried Silicon Oxide (BOX)n-transistor


p-transistor


FIGURE 3.17  SOI types


3.4      CMOS Process Enhancements 121


technically accurate again! nMOS and pMOS transistors use different types of


metal with different work functions (energy required to free an electron from a


solid) to set the threshold voltages. A second lower-resistance metal layer plays a


role similar to a silicide.


One of the challenges with metal gates is that they melt if exposed to the


high temperature source/drain formation steps. But if the gate were formed after


the source and drain, the self-alignment advantage would be lost. Intel sidesteps


this conundrum by ﬁrst building the transistor with a high-k dielectric and a


standard polysilicon gate. After the transistor is complete and the interlayer


dielectric is formed, the wafer is polished to expose the polysilicon gates and


etched to remove the undesired poly. A thin metal gate is deposited in the trench.


Different metals with different workfunctions are required for the nMOS and


pMOS transistors. Finally, the trench is ﬁlled with a thicker layer of Al for low gate resistance, and the wafer is planarized again.


3.4.1.4 Higher Mobility Increasing the mobility ( ) of the semiconductor improves drive current and transistor speed. One way to improve the mobility is to introduce mechanical strain in the channel. This is called strained silicon.


Figure 3.19 shows strained nMOS and pMOS transistors in the Intel 65 nm process that achieve 40% and 100% higher mobility than unstrained transistors, respectively[Tyagi05, Thompson02, Thompson04]. The nMOS channel is under tensile stress created by an insulating ﬁlm of silicon nitride (SiN) capping the gate. The pMOS channel is under compressive stress produced by etching a recess into the source and drain, then ﬁlling the slot with an epitaxial layer of silicon germanium (SiGe). Germanium is another group IV semiconductor with a larger atomic radius than silicon. When a small fraction of the silicon atoms are replaced by germanium, the lattice retains its shape but undergoes mechanical strain because of the larger atoms. Using separate strain mechanisms for the nMOS and pMOS transistors improves mobility of both electrons and holes. An alternative approach is to implant germanium atoms in the channel, introducing tensile stress that only improves electron mobility. STI also introduces stress that affects mobility, so the diffusion layout can impact performance [Topaloglu07].


High-Stress Film


Silicide


Channel


source


drain


Strain


SiGe


FIGURE 3.19  Strained silicon transistor micrographs: (a) nMOS, (b) pMOS (© IEEE 2005.)


FIGURE 3.18  High-k gate stack TEM (© IEEE 2007.)


122


SiGe is also used in high-performance bipolar transistors, especially for radiofrequency (RF) applications. SiGe bipolar devices can be combined with conventional CMOS on the same substrate, which is valuable for low-cost system-on-chip applications that require both digital and RF circuits [Hashimoto02, Harame01a, Harame01b].


3.4.1.5 Plastic Transistors MOS transistors can be fabricated with organic chemicals. These transistors show promise in active matrix displays, ﬂexible electronic paper, and radio-frequency ID tags because the devices can be manufactured from an inexpensive chemical solution[Huitema03, Myny09]. Figure 3.20 shows the structure of a plastic pMOS transistor. The transistor is built “upside down” with the gold gates and interconnect patterned ﬁrst on the substrate. Then an organic insulator or silicon nitride is laid down, followed by the gold source and drain connections. Finally, the organic semiconductor (pentacene) is laid down. The mobility of the carriers in the plastic pMOS transistor is about


0.15 cm2/V · s. This is three orders of magnitude lower than that of a comparable silicon device, but is good enough for special applications. Typical lengths and widths are 5 m and 400 m, respectively.


3.4.1.6 High-Voltage Transistors High-voltage MOSFETs can also be integrated onto conventional CMOS processes for switching and high-power applications. Gate oxide thickness and channel length have to be larger than usual to prevent breakdown. Specialized process steps are necessary to achieve very high breakdown voltages.


3.4.2  Interconnect


Interconnect has advanced rapidly. While two or three metal layers were once the norm,CMP has enabled inexpensive processes to include seven or more layers. Copper metal and low-k dielectrics are almost universal to reduce the resistance and capacitance of these wires.


3.4.2.1 Copper Damascene Process While aluminum was long the interconnect metal of choice, copper has largely superseded it in nanometer processes. This is primarily due to the higher conductivity of copper compared to aluminum. Some challenges of adopting copper include the following [Merchant01]:


Copper atoms diffuse into the silicon and dielectrics, destroying transistors.


The processing required to etch copper wires is tricky.


Copper oxide forms readily and interferes with good contacts.


Care has to be taken not to introduce copper into the environment as a pollutant.


Barrier layers have to be used to prevent the copper from entering the silicon surface.


A new metallization procedure called the damascene process was invented to form this barrier. The process gets its name from the medieval metallurgists of Damascus who craftedﬁne inlaid swords. In a conventional subtractive aluminum-based metallization step, as we have seen, aluminum is layered on the silicon surface (where vias also have been etched)and then a mask and resist are used to deﬁne which areas of metal are to be retained. The unneeded metal is etched away. A dielectric (SiO2 or other) is then placed over the aluminum conductors and the process can be repeated.


Substrate (glass/plastic)


Semiconductor (Pentacene)


Insulator (Polymer Si/Nx)


Gold Terminals Gate Source


FIGURE 3.20  Plastic transistors


3.4      CMOS Process Enhancements 123


A typical copper damascene process is shown in Figure 3.21, which is an adaptation of a dual damascene process ﬂow from Novellus. Figure 3.21(a) shows a barrier layer over the prior metallization layer. This stops the copper from diffusing into the dielectric and silicon. The via dielectric is then laid down (Figure 3.21(b)). A further barrier layer can then be patterned, and the line dielectric is layered on top of the structure, as shown in Figure 3.21(c). An anti-reﬂective layer (which helps in the photolithographic process) is added to the top of the sandwich. The two dielectrics are then etched away where the lines and vias are required. A barrier layer such as 10 nm thick Ta or TaN ﬁlm is then deposited to prevent the copper from diffusing into the dielectrics [Peng02]. As can be seen, a thin layer of the barrier remains at the bottom of the via so the barrier must be conductive. A copper seed layer is then coated over the barrier layer (Figure 3.21(g )). The resulting structure is electroplated full of copper, and ﬁnally the structure is ground ﬂat with CMP,as shown in Figure 3.21(h).


3.4.2.2 Low-k Dielectrics SiO2 has a dielectric constant of k = 3.9–4.2. Low-k dielectrics between wires are attractive because they decrease the wire capacitance [Brown03]. This reduces wire delay, noise, and power consumption. Adding ﬂuorine to the silicon dioxide creates ﬂuorosilicate glass (FSG or SiOF) with a dielectric constant of 3.6, widely used in 130 nm processes. Adding carbon to the oxide can reduce the dielectric constant to about


2.8–3; such SiCOH (also called carbon-doped oxide, CDO) is commonly used at the 90 and 65 nm generation. Alternatively, porous polymer-based dielectrics can deliver even lower dielectric constants. For example, SiLK, from Dow Chemical, has k = 2.6 and may scale to k = 1.6–2.2 by increasing the porosity. IBM has demonstrated air (or vacuum)


(a) Diffusion Barrier Etch Stop


(b) Via Dielectric


(c ) Line Dielectric


(d) Anti-Reflective Layer


(e) Dielectric Etch


(f) Ta Barrier


(g) Cu Seed


(h) Cu Fill (electroplate)and CMP


FIGURE 3.21  Copper dual damascene interconnect processing steps


124


gaps, which have k = 1 where the dielectric has been eliminated entirely, as shown in Figure 3.22. Developing low-k dielectrics that can withstand the high temperatures during processing and the forces applied during CMP is a major challenge.


3.4.3  Circuit Elements


While CMOS transistors provide for almost complete digital functionality,the use of CMOS technology as the mixed signal and RF process of choice has driven the addition of special process options to enhance the performance of circuit elements required for these purposes.


3.4.3.1 Capacitors In a conventional CMOS process, a capacitor can be constructed using the gate and source/drain of an MOS transistor, a diffusion area(to ground or VDD), or a parallel metal plate capacitor (using stacked metal layers). The MOS capacitor has good capacitance per area but is relatively nonlinear if operated over large voltage ranges. The diffusion capacitor cannot be used for a ﬂoating capacitor (where neither terminal is connected to ground). The metal parallel plate capacitor has low capacitance per area. Normally, the aim in using a ﬂoating capacitor is to have the highest ratio of desired capacitance value to stray capacitance (to ground normally). The bottom metal plate contributes stray capacitance to ground.


Analog circuits frequently require capacitors in the range of 1 to 10 pF. The ﬁrst method for doing this was to add a second polysilicon layer so that a poly-insulator-poly(PIP) capacitor could be constructed. A thin oxide was placed between the two polysilicon layers to achieve capacitance of approximately 1 fF/ m2.


The most common capacitor used in CMOS processes today is a fringe capacitor,which consists of interdigitated ﬁngers of metal, as shown in Figure 3.23. Multiple layers can be stacked to increase the capacitance per area.


3.4.3.2 Resistors In unaugmented processes, resistors can be built from any layer, with the ﬁnal resistance depending on the resistivity of the layer. Building large resistances in a small area requires layers with high resistivity, particularly polysilicon, diffusion, and n-wells. Diffusion has a large parasitic capacitance to ground, making it unsuitable for high-frequency applications. Polysilicon gates are usually silicided to have low resistivity.


The ﬁx for this is to allow for undoped high-resistivity polysilicon. This is speciﬁed with a silicide block mask where high-value poly resistors are required. The resistivity can be tuned to around 300–1000 /square, depending on doping levels. Another material used for precision resistors is nichrome, although this requires a special processing step.


A typical resistor layout is shown in Figure 3.24. This geometry is sometimes called a meander structure. A number of unit resistors have been used so that a variety of matched resistor values can be constructed. For instance, if 20 k , and 15 k  resistors were required, a unit value of 5 k  could be used. Then three resistors (as shown) would construct a 15 k  resistor. The two resistors at the ends are called dummy resistors or ﬁngers.


They perform no circuit function, but replicate the proximity effects (such as etch and implant) that the interior resistors see during processing. This helps ensure that all resistors are matched.


The various resistor options have temperature and voltage coefﬁcients. Foundry design manuals normally include these values.


FIGURE 3.22  Micrograph showing air gap  insulation between copper wires (Courtesy  of International Business Machines Corporation. Unauthorized use not permitted.)


FIGURE 3.23


Fringe capacitor


3.4      CMOS Process Enhancements 125


3.4.3.3 Inductors The desire to integrate inductors on chips has increased radically with


the upsurge in interest in RF circuits. The most common monolithic inductor is the spiral


inductor, which is a spiral of upper-level metal. A typical inductor is shown in Figure


3.25(a). As the process is planar, an underpass connection has to be made to complete the


inductor. A typical equivalent model is shown in Figure 3.25(b). In addition to the


required inductance L, there are several parasitic components. Rs is the


series resistance of the metal (and contacts) used to form the inductor.


Cp is the parallel capacitance to ground due to the area of the metal


wires forming the inductor. Cs is the shunt capacitance of the underpass. Finally, Rp is an element that models the loss incurred in the resistive substrate.


Usually, when considering an inductor, the parameters of interest


to a designer are its inductance, the Q of the inductor, and the selfresonant frequency. High Qs are sought to create low phase-noise oscillators, narrow ﬁlters, and low-loss circuits in general. Q values for typical planar inductors on a bulk process range from 5 to 10.


The number of turns n required to achieve some inductance L if


the wire pitch, in turns per meter, is P = 1/2(W + S), is [Lee98]


(3.4)


where 0 = 1.2 × 10–6 H/m is the permeability of free space. Figure 3.25 has n = 1.75 turns. Higher-quality inductors can also be manufactured using bond wires between I/O pads. The inductance of a wire of length l and radius r is approximately


(3.5)


or about 1 nH/mm for standard 1 mil (25 m) bond wires.


Dummy Finger


FIGURE 3.24  Resistor layout


LP


l r


20 75


Rs


Cs


Rp


FIGURE 3.25  Typical spiral inductor and  equivalent circuit [Rotella02]


126


Reduction in Q occurs because of the resistive loss in the conductors used to build the inductor (Rs), and the eddy current loss in the resistive silicon substrate (Rp). In an effort to increase Q, designers have resorted to removing the substrate below the inductor using MEMS techniques [Yoon02]. The easiest way to improve the Q of monolithic inductors is to increase the thickness of the top-level metal. The Q can also be improved by using a patterned ground shield in polysilicon under the inductor to decrease substrate losses.


3.4.3.4 Transmission Lines A transmission line can be used on a chip to provide a known impedance wire. Two basic kinds of transmission lines are commonly used: microstrips and coplanar waveguides.


A microstrip transmission line, as shown in Figure 3.26(a), is composed of a wire of width w and thickness t placed over a ground plane and separated by a dielectric of height h and dielectric constant k. In the chip case, the wire might be the top level of metallization and the ground plane the next metal layer down.


A coplanar waveguide does not require a sublayer ground plane and is shown in Figure 3.26(b). It consists of a wire of width w spaced s on each side from coplanar ground wires. The reader is referred to [Wadell91] for detailed design equations.


3.4.3.5 Bipolar Transistors  Bipolar transistors were mentioned previously in our discussion of SiGe process options. Both npn and pnp bipolar transistors can be added to a CMOS process, which is then called a BiCMOS process. These processes tend to be used for specialized analog or high-voltage circuits. In a regular n-well process, a parasitic vertical pnp transistor is present that can be used for circuits such as bandgap voltage references. This transistor is shown in Figure 3.27 with the p-substrate collector, the n-well base, and the p-diffusion emitter. Both process cross-section and layout are shown. This transistor, in conjunction with a parasitic npn, is the cause of latchup (see Section 7.3.6).


3.4.3.6 Embedded DRAM Dynamic RAM (DRAM) uses a single transistor and a capacitor to store a bit of information. It is about ﬁve times denser than static RAM (SRAM)conventionally used on CMOS logic chips, so it can reduce the size of a chip containing large amounts of memory. DRAM was conventionally manufactured on specialized processes that produced low-performance logic transistors. DRAM requires specialized structures to build capacitors in a small area. One common structure is a trench, which is etched


w


h


FIGURE 3.26  Microstrip and coplanar waveguide


3.4      CMOS Process Enhancements 127


down into the substrate. Some recent processes have introduced compact capacitor structures for building embedded DRAM alongside high-performance logic. Section 12.3 discusses DRAM in more depth.


3.4.3.7 Non-Volatile Memory Non-volatile memory (NVM) retains its state when the power is removed from the circuit. The simplest NVM is a mask-programmed ROM cell(see Section 12.4). This type of NVM is not reprogrammable or programmable after the device is manufactured. A one-time programmable (OTP) memory can be implemented using a fuse constructed of a thin piece of metal through which is passed a current that vaporizes the metal by exceeding the current density in the wire. The ﬁrst reprogrammable memories used a stacked polysilicon gate structure and were programmed by applying a high voltage to the device in a manner that caused Fowler-Nordheim tunneling to store a charge on a ﬂoating gate. The whole memory could be erased by exposing it to UV light that knocked the charge off the gate. These memories evolved to electrically erasable memories, which are today represented by Flash memory.


A typical Flash memory transistor is shown in Figure 3.28 [She02]. The source and drain structures can vary considerably to allow for high-voltage operation, but the dualgate structure is fairly common. The gate structure is a stacked conﬁguration commencing with a thin tunnel oxide or nitride. A ﬂoating polysilicon gate sits on top of this oxide and a conventional gate oxide is placed on top of the ﬂoating gate. Finally, a polysilicon control gate is placed on top of the gate oxide. The operation of the cell is also shown in Figure


p+ substrate Contact


p+ diode


n+ well Contact


Collector


Base


Emitter


Cross-Section


Representative Layout


p+ diffusion


FIGURE 3.27  Vertical pnp bipolar transistor


Control Gate Floating Gate


Tunnel Oxide


n-well p-well


0 V


1.2 V


Normal Operation


Floating


20 V


Program


Deprogram


FIGURE 3.28  Flash memory construction and operation


128


3.28. In normal operation, the ﬂoating gate determines whether or not the transistor is conducting. To program the cell, the source is left ﬂoating and the control gate is raised to approximately 20 V (using an on-chip voltage multiplier). This causes electrons to tunnel into the ﬂoating gate, and thus program it. To deprogram a cell, the drain and source are left ﬂoating and the substrate (or well) is connected to 20 V. The electrons stored on theﬂoating gate tunnel away, leaving the gate in an unprogrammed state.


3.4.3.8 Fuses and Antifuses During manufacturing, fuses can be blown with a high current or zapped by a laser. In the latter case, an area is normally left in the passivation oxide to allow the laser direct access to the metal link that is to be cut. Figure 3.29 shows the layout of a metal fuse.


Laser-blown fuses are large and the blow process can damage adjacent devices. Electronic fuses are structures whose characteristics can be nondestructively altered by applying a high current. For example, IBM eFUSEs are narrow polysilicon wires silicided with cobalt. The resistance is initially about 200 . If a programming current of 10–15 mA is applied for 200 s, the cobalt will migrate to the anode, as shown in Figure 3.30. This raises the resistance by an order of magnitude. Simple sense circuits are used to detect the state of the eFUSE. IBM uses fuses for chip serial numbers, thermal sensor calibration, and to reconﬁgure defective components [Rohrer05, Rizzolo07].


An antifuse is a similar device that initially has a high resistivity but can become low resistance when a programming voltage is applied. This device requires special processing and is used in programmable logic devices (see Section 12.7).


3.4.3.9 Microelectromechanical Systems (MEMS) Semiconductor processes and especially CMOS processes have been used to construct tiny mechanical systems monolithically. A typical device is the well-known air-bag sensor,which is a small accelerometer consisting of an air bridge capacitor that can detect sudden changes in acceleration when co-integrated with some conditioning electronics. MEMS micromirrors on torsional hinges are used in inexpensive, high-resolution digital light projectors. Structures such as cantilevers,mechanical resonators, and even micromotors have been built. A full discussion of MEMS is beyond the scope of this book, but further material can be found in texts such as [Maluf04].


3.4.3.10 Integrated Photonics Although silicon is opaque at visible wavelengths, it is transparent in the infrared range used in optical ﬁbers. Semiconductor photonic components are rapidly evolving. Components compatible with a conventional CMOS process include waveguides, modulators, and photodetectors [Salib04, Young10]. A key missing component is an optical source, such as a laser. However, just as VDD is generated off-chip from a DC power supply, light can be generated off-chip and brought onto the chip through an optical ﬁber. Figure 3.31 shows a holographic lens used to couple an optical ﬁber to an on-chip waveguide [Huang06]. Integrated photonics shows particular promise for optical transceivers to replace copper wires in high-speed networks.


Fuse


Metal Track


FIGURE 3.29


A typical metal fuse


Intact


Blown


FIGURE 3.30  eFUSE (© IEEE 2005.)


FIGURE 3.31  Optical waveguide and holographic lens integrated with a 130 nm CMOS  process (© IEEE 2006.)


3.4      CMOS Process Enhancements 129


3.4.3.11 Three-Dimensional Integrated Circuits 3D ICs contain multiple layers of


devices. Stacking transistors in layers can reduce wire lengths, improving speed and power.


It also can permit heterogeneous technologies to be combined in one package; for example, logic, memory, and analog/RF chips can be stacked into one package.


IBM has described a process in which 200 mm wafers are ground down to a remarkable 20 m thickness after fabrication [Topol06]. They are aligned to 1 m tolerance, and


then one is bonded on top of another using oxide-fusion or copper bonding. Tall skinny


through-silicon vias (TSVs) between the wafers are etched and metallized;


the aspect ratio of the vias and the thickness of the wafers sets the density


of contacts between wafers. Densities of 104 TSVs/mm2 or more can presently be achieved. Some of the challenges in 3D integration include wafer


bowing, testing layers before they are bonded, and managing cooling and


power delivery. Figure 3.32 shows two wafers bonded together. The bottom


wafer has four levels of metal and the top wafer has two levels. The 8- m


wide landing pad on the top metal layer of the bottom wafer provides tolerances for misalignment with the 3D vias protruding from beneath the top


wafer.


3D ICs are starting to move from research into production [Emma08].


An initial application is to stack multiple memory chips to provide a higher


capacity in a standard form factor.


3.4.4  Beyond Conventional CMOS


A major problem with scaling bulk transistors is the subthreshold leakage from drain to source caused by the inability of the gate to turn off the channel completely. This can be improved by a gate structure where the gate is placed on two, three, or four sides of the channel to gain better control over the charge in the channel. A promising structure solves the problem by forming a vertical channel and constructing the gate in a pincer-like arrangement around three sides. These devices have been given the generic name “ﬁnfets”because the source/drain regions form ﬁns on the silicon surface [Hisamoto98]. Figure


3.33(a) shows a 3D view of a ﬁnfet, while Figure 3.33(b) shows the cross-section and Figure 3.33(c) shows the top view. The gate wraps around three sides of the vertical


BOX


Gate Top View


FIGURE 3.33  Finfet structure


FIGURE 3.32  Scanning electron micrograph  of 3-dimensional integration of two wafers


(Reprinted from [Koester08]. Courtesy of


International Business Machines Corporation. Unauthorized use not permitted.)


130


source/drain ﬁns. The width of the device is deﬁned by the height of the ﬁn, so wide devices are constructed by paralleling ﬁns. Figure 3.34 shows a micrograph of a prototype ﬁnfet that Intel calls a trigate transistor [Kavalleros06].


Compounds from groups III and V of the periodic table, such as GaAs, offer electron mobilities up to 30 times higher than silicon. Such III-V materials have been research topics for decades. GaAs was once used for very high frequency applications, but has largely been replaced by advanced CMOS processes. However, III-V materials might be integrated into CMOS some day in the future.


Nanotechnology is presently a hot research area seeking alternative structures to replace CMOS when conventional scaling ﬁnally runs out of steam. Little obvious progress in radical new device structures has been made since the previous edition of the book, but conventional sub-100 nm CMOS transistors are now being called nanotechnology! Alternative technologies have a large hurdle to overcome competing with the hundreds of billions of dollars that have been invested in advancing CMOS over four decades.


Carbon nanotubes are one nanotechnology that have been used to demonstrate transistor behavior and build inverters [Liu01]. Nanotubes are cylinders with a diameter of a few nanometers. They are of interest because the nanotube is smaller than the predicted endpoint for CMOS gate lengths, and because the nanotubes offer high mobility. A theoretical nanotube transistor is shown in Figure 3.35 [Wong03]. Presently, the speeds are quite slow and the manufacturing techniques are limited, but they may be of interest in the future [Raychowdhury07, Patil09].


3.5 Technology-Related CAD Issues


The mask database is the interface between the semiconductor manufacturer and the chip designer. Two basic checks have to be completed to ensure that this description can be turned into a working chip. First, the speciﬁed geometric design rules must be obeyed.


Second, the interrelationship of the masks must, upon passing through the manufacturing


FIGURE 3.35  Carbon nanotube transistor (© IEEE 2003.)


FIGURE 3.34  Trigate transistor (Reprinted with permission of Intel  Corporation.)


3.5      Technology-Related CAD Issues 131


process, produce the correct interconnected set of circuit elements. To check these two requirements, two basic CAD tools are required: a Design Rule Check (DRC) program and a mask circuit extraction program. The most common approach to implementing these tools is a set of subprograms that perform general geometry operations. A particular set of DRC rules or extraction rules for a given CMOS process (or any semiconductor process)deﬁnes the operations that must be performed on each mask and the inter-mask checks that must be completed. Accompanied by a written description, these run sets are usually the deﬁning speciﬁcation for a process.


In this section, we will examine a hypothetical DRC and extraction system to illustrate the nature of these run sets.


3.5.1  Design Rule Checking (DRC)


Although we can design the physical layout in a certain set of mask layers, the actual masks used in fabrication can be derived from the original speciﬁcation. Similarly, when we want a program to determine what we have designed by examining the interrelationship of the various mask layers, it may be necessary to determine various logical combinations between masks.


To examine these concepts, let us posit the existence of the following functions(loosely based on the Cadence DRACULA DRC program), which we will apply to a geometric database (i.e., rectangles, polygons, and paths):


AND  layer1 layer2 -> layer3


ANDs layer1 and layer2 together to produce layer3


(i.e., the intersection of the two input mask descriptions)


OR layer1 layer2 -> layer3


ORs layer1 and layer2 together to produce layer3(i.e., the union of the two input mask descriptions)


NOT layer1 layer2 -> layer3


Subtracts layer2 from layer1 to produce layer3


(i.e., the difference of the two input mask descriptions)


WIDTH layer > dimension -> layer3


Checks that all geometry on layer is larger than dimension  Any geometry that is not is placed in layer3


SPACE layer > dimension -> layer3


Checks that all geometry on layer is spaced further than dimension Any geometry that is not is placed in layer3


The following layers will be assumed as input:


nwell


active


poly


poly-contact active-contact metal


132


Typically, useful sublayers are generated initially. First, the four kinds of active area are isolated. The rule set to accomplish this is as follows:


NOT  all nwell -> substrate


AND  nwell active -> nwell-active NOT  active nwell -> pwell-active AND  nwell-active p-select -> pdiff AND  nwell-active n-select -> vddn AND  pwell-active n-select -> ndiff AND  pwell-active p-select -> gndp


In the above speciﬁcation, a number of new layers have been designated. For instance,the ﬁrst rule states that wherever nwell is absent, a layer called substrate exists. The second rule states that all active areas within the nwell are nwell-active. A combination of nwellactive and p-select or n-select yields pdiff (p diffusion) or vddn (well tap).


To ﬁnd the transistors, the following rule set is used:


AND poly ndiff -> ngates AND poly pdiff -> pgates


The ﬁrst rule states that the combination of poly and ndiff yields the ngates region—all of the n-transistor gates.


Typical design rule checks (DRC) might include the following:


WIDTH metal  < 0.13 -> metal-width-error SPACE metal  < 0.13 -> metal-space-error


For instance, the ﬁrst rule determines if any metal is narrower than 0.13 m and places the errors in the metal-width-error layer. This layer might be interactively displayed to highlight the errors.


3.5.2  Circuit Extraction


Now imagine that we want to determine the electrical connectivity of a mask database.


The following commands are required:


CONNECT layer1 layer2


Electrically connect layer1 and layer2.


MOS name drain-layer gate-layer source-layer substrate-layer


Deﬁne an MOS transistor in terms of the component terminal layers. (This is, admittedly, a little bit of magic.)


The connections between layers can be speciﬁed as follows:


CONNECT active-contact pdiff CONNECT active-contact ndiff CONNECT active-contact vddn CONNECT active-contact gndp CONNECT active-contact metal CONNECT gndp substrate


CONNECT vddn nwell


CONNECT poly-contact poly CONNECT poly-contact metal


The connections between the diffusions and metal are speciﬁed by the ﬁrst seven statements. The last two statements specify how metal is connected to poly.


3.6      Manufacturing Issues 133


Finally, the active devices are speciﬁed in terms of the layers that we have derived:


MOS nmos ndiff ngates ndiff substrate MOS pmos pdiff pgates pdiff nwell


An output statement might then be used to output the extracted transistors in some netlist format (i.e., SPICE format). The extracted netlist is often used to compare the layout against the intended schematic.


It is important to realize that the above run set is manually generated. The data you extract from such a program is only as good as the input. For instance, if parasitic routing capacitances are required, then each layer interaction must be coded. If parasitic resistance is important in determining circuit performance, it also must be speciﬁcally included in the extraction run set.


3.6 Manufacturing Issues


As processes have evolved, various rules and guidelines have emerged that reﬂect the complexity of the processing. These rules are often called Design for Manufacturability (DFM).


3.6.1  Antenna Rules


When a metal wire contacted to a transistor gate is plasma-etched, it can charge up to a voltage sufﬁcient to zap the thin gate oxides. This is called plasma-induced gate-oxide damage, or simply the antenna effect. It can increase the gate leakage, change the threshold voltage, and reduce the life expectancy of a transistor. Longer wires accumulate more charge and are more likely to damage the gates.


During the high-temperature plasma etch process, the diodes formed by source and drain diffusions can conduct signiﬁcant amounts of current. These diodes bleed off charge from wires before gate oxide is damaged.


Antenna rules specify the maximum area of metal that can be connected to a gate without a source or drain to act as a discharge element. Larger gates can withstand more charge buildup. The design rules normally deﬁne the maximum ratio of metal area to gate area such that charge on the metal will not damage the gate. The ratios can vary from 100:1 to 5000:1 depending on the thickness of the gate oxide (and hence breakdown voltage) of the transistor in question. Higher ratios apply to thicker gate oxide transistors(i.e., 3.3 V I/O transistors).


Figure 3.36 shows an antenna rule violation and two ways to ﬁx it. In Figure 3.36(a),a long metal1 line is connected to a transistor gate. It has no connection to diffusion until metal2 is formed, so the gate may be damaged during the metal1 plasma etch. In Figure


3.36(b), the metal1 line is interrupted with a jumper to metal2. This reduces the amount of charge that could zap the gate during the metal1 etch and solves the problem. In Figure


3.36(c), an antenna diode is added, providing a discharge path during the etch. The diode is reverse-biased during normal operation and thus does not disturb circuit function(except for the area and capacitance that it contributes). Note that the problem could also have been solved by making the gate wider.


134


For circuits requiring good matching, such as analog and memory cells, transistor gates should connect directly to diffusion with a short segment of metal1 to avoid gate damage that could introduce mismatches.


3.6.2  Layer Density Rules


Another set of rules that pertain to advanced processes are layer density rules, which specify a minimum and maximum density of a particular layer within a speciﬁed area. Etch rates have some sensitivity to the amount of material that must be removed. For example,if polysilicon density were too high or too low, transistor gates might end up over- or under-etched, resulting in channel-length variations. Similarly, the CMP process may cause dishing (excessive removal) of copper when the density is not uniform.


To prevent these issues, a metal layer might be required to have 30% minimum and 70% maximum density within a 100 m by 100 m area. For digital circuits, these density levels are normally reached with routine routing unless empty spaces exist. Analog and RF circuits, on the other hand, are almost by deﬁnition sparse. Thus, diffusion, polysilicon,and metal layers may have to be added manually or by a ﬁll program after design has been completed. The ﬁll can be grounded or left ﬂoating. Floating ﬁll contributes lower total capacitance but more coupling capacitance to nearby wires. Grounded ﬁll requires routing the ground net to the ﬁll structures. Clever ﬁll patterns such as staggered rectangles, plussign patterns, or diamonds result in lower and more predictable capacitance than do simple geometrical grids [Kahng08]. Designers must be aware of the ﬁll so that it does not introduce unexpected parasitic capacitance to nearby wires.


3.6.3  Resolution Enhancement Rules


Some resolution enhancement techniques impose further design rules. For example, polysilicon typically uses the narrowest lines and thus needs the most enhancement. This can be simplest if polysilicon gates are only drawn in a single orientation (horizontal or vertical).


Using a single orientation also reduces systematic process variability. Avoid small jogs and notches (those less than the minimum layer width), because such notches can interfere with proper OPC analysis.


metal2


Long metal1 connected to gate can cause damage.


Add metal2 jumper to fix problem.


Add diode to fix problem.


metal1


metal2 metal1


diffusion


FIGURE 3.36  Antenna rule violation and ﬁxes


3.6      Manufacturing Issues 135


The design community is presently debating a move toward restrictive design rules to facilitate RET and reduce manufacturing variability by limiting designers to a smaller set of uniform layout features. These rules might come at the expense of greater area. For example, Intel introduced restrictive design rules for polysilicon in the 45 nm process to control variation and facilitate 193 nm double-patterning lithography [Webb08]. Under these rules, polysilicon is limited to one pitch and direction in layout. This also simpliﬁed contact and metal1 rules: the contact pitch is the same as the gate pitch, and metal1 parallel to the gates also has the same pitch. Wide poly pads for contacts and orthogonal polysilicon routing were eliminated by introducing a trench contact suitable for local interconnect. Intel found that the restrictive rules did not impact standard cell density and that excellent yield is achieved.


3.6.4  Metal Slotting Rules


Some processes have special rules requiring that wide (e.g. > 10–40 m) metal wires have slots. Slots are long slits, on the order of 3 m wide, in the wire running parallel to the direction of current ﬂow, as shown in Figure 3.37. They provide stress relief, help keep the wire in place, and reduce the risk of electromigration failure (see Section 7.3.3.1). Design rules vary widely between manufacturers.


3.6.5  Yield Enhancement Guidelines


To improve yield, some processes recommend increasing certain widths and spacings where they do not impact area or performance. For example, increasing the polysilicon gate extension slightly reduces the risk of transistor failures from poly/diffusion mask misalignment.


Increasing space between metal lines where possible reduces the risk of shorts and also reduces wire capacitance. Other good practices to improve yield include the following:


Space out wires to reduce risk of short circuits and reduce capacitance.


Use non-minimum-width wires to reduce risk of open circuits and to reduce


resistance.


Use at least two vias for every connection to avoid open circuits if one via is


malformed, and to reduce electromigration wearout.


Surround contacts and vias by landing pads with more than the minimum overlap  to reduce resistance variation and open circuits caused by misaligned contacts.


Use wider-than-minimum transistors; minimum-width transistors are subject to  greater variability and tend not to perform as well.


Avoid non-rectangular shapes such as 45-degree angles and circles. For specialized  circuits such as RAMs that strongly beneﬁt from 45-degree angles, verify masks  after optical proximity correction analysis.


Place dummy transistors or cells at the edge of arrays and sensitive circuits to


improve uniformity and matching.


If it looks nice, it will work better.


3.37 Pitfalls and Fallacies


50 m


FIGURE 3.37  Slots in  wide metal power bus


136


3.7 Pitfalls and Fallacies


Targeting a bleeding-edge process


There is a fine balance when you are deciding whether or not to move to a new process for a  new design. On the one hand, you are tempted by increased density and speed. On the other  hand, support for the new process can initially be expensive (becoming familiar with process  rules, CAD tool scripts, porting analog and RF designs, locating logic libraries, etc.). In addition, CMOS foundries frequently tune their processes in the first few months of production, and       often yield improvement steps can reflect back to design rule changes that impact designs late  in their tapeout schedule. For this reason, it is frequently prudent not to jump immediately  into a new process when it becomes available. On the other hand, if you are limited in speed  or some other attribute that is solved by the new process, then you don’t have much choice  but to bite the bullet.


Using lambda design rules on commercial designs


Lambda rules have been used in this text for ease of explanation and consistency. They are  usable for class designs. However, they are not very useful for production designs for deep submicron processes. Of particular concern are the metal width and spacing rules, which are too  conservative for most production processes.


Failing to account for the parasitic effects of metal fill


With area density rules, particularly in metal, most design flows include an automatic fill step  to achieve the correct metal density. Particularly in analog and RF circuits, it is important to  either exclude the automatic fill operation from that area or check circuit performance after  the fill by completing a full parasitic extract and rerunning the verification simulation scripts.


Failing to include process calibration test structures


In the discussion on scribe line structures, it was mentioned that test structures are frequently  inserted here by the silicon manufacturer. Documentation is often unavailable, so it is prudent  for designers (particularly in academic designs, which receive less support from a foundry) to  include their own test structures such as transistors or ring oscillators. This allows designers  to calibrate the silicon against simulation models.


Waiving design rules


Sometimes it is tempting to ignore a design rule when you are certain it does not apply. For  example, consider two wires separated by only 2 . This violates a design rule because the


wires might short together during manufacturing. If the wires are actually connected elsewhere, one might ignore the rule because further shorting is harmless. However, it is possible  that the “antifeature” between the wires would produce a narrow strip of photoresist that


could break off and float around during manufacturing, damaging some other structure. Moreover, even if the rule violation is safe, keeping track of all the legitimate exceptions is too much  work, especially on a large design. It is better to simply fix the design rule error.


Placing cute logos on a chip


Designers have a tradition of hiding their initials on the chip or embedding cute logos in an unused corner of the die. Some automatic wafer inspection tools find that the logos look more  like a spec of dust than a legitimate chip structure and mark all of the chips as defective! Some  companies now ban the inclusion of layout that is not essential to the operation of the device. Others require placing the logo in the corner of the chip and covering it with a special


pseudolayer called LOGO to tell RET and wafer inspection tools to ignore the logo.


Logos on the image sensor for  the Spirit Mars rover


(Reprinted from Molecular


Expressions Silicon Zoo,


micro.magnet.fsu.edu/creatures, with permission of Michael Davidson.)


3.8      Historical Perspective 137


3.8 Historical Perspective


In the ﬁrst days of integrated circuits, layout editors and design rule checkers were humans with knives and magnifying lenses. [Volk01] tells a captivating story of design at Intel in the early 1970s. Mask designers drew layout with sharp colored pencils on very large sheets of Mylar graph paper, as shown in Figure 3.38(a). Engineers and technicians then scrutinized the drawings to see if all of the design rules were satisﬁed and if the connections matched the schematic. Most chips at the time were probably manufactured with minor design rule errors, but correct wiring was essential. For example, two engineers each checked all 20,000 transistors on the 8086 in 1977 by hand. Both found 19 of the same 20 errors, giving conﬁdence that the design was correct.


3.2 If the gate oxide thickness in a SiO2-based structure is 2 nm, what would be the


thickness of an HfO2-based dielectric providing the same capacitance?


3.3 Explain the difference between a polycide and a salicide CMOS process. Which


would be likely to have higher performance and why?


3.4 Draw the layout for a pMOS transistor in an n-well process that has active, p-select, n-select, polysilicon, contact, and metal1 masks. Include the well contact to VDD.


3.5 What is the lowest resistance metal for interconnect? Why isn’t it used?


3.6 Calculate the minimum contacted pitch as shown in Figure 3.39 for metal1 in terms  of  using the SUBM rules. Is there a wiring strategy that can reduce this pitch?


Contacted Pitch


FIGURE 3.39  Contacted metal pitch


140


3.7 Using the SUBM rules, calculate the minimum uncontacted and contacted transistor pitch, as shown in Figure 3.40.


3.8 Using Figure 3.41 and the SUBM design rules, calculate the minimum n to p pitch  and the minimum inverter height with and without the poly contact to the gate (in). If  an SOI process has 2 spacing between n and p diffusion, to what are the two pitches  reduced?


3.9 Design a metal6 fuse ROM cell in a process where the minimum metal width is 0.5  m and the maximum current density is 2 mA/ m. A fuse current of less than 10  mA is desired.


Uncontacted Transistor Pitch


Contacted Transistor Pitch


FIGURE 3.40  Uncontacted and  contacted transistor pitch


Minimum n-transistor Width


Minimum


p-transistor Width


out


in


FIGURE 3.41  Minimum inverter height


141


Delay


4.1 Introduction


In Chapter 1 we learned how to make chips that work. Now we move on to making chips that work well. The two most common metrics for a good chip are speed and power, discussed in this chapter and Chapter 5, respectively. Delay and power are inﬂuenced as much by the wires as by the transistors, so Chapter 6 delves into interconnect analysis and design. A chip is of no value if it cannot reliably accomplish its function, so Chapter 7 examines how we achieve robustness in designs.


The most obvious way to characterize a circuit is through simulation, and that will be the topic of Chapter 8. Unfortunately, simulations only inform us how a particular circuit behaves, not how to change the circuit to make it better. There are far too many degrees of freedom in chip design to explore each promising path through simulation (although some may try). Moreover, if we don’t know approximately what the result of the simulation should be, we are unlikely to catch the inevitable bugs in our simulation model. Mediocre engineers rely entirely on computer tools, but outstanding engineers develop their physical intuition to rapidly predict the behavior of circuits. In this chapter and the next two, we are primarily concerned with the development of simple models that will assist us in understanding system performance.


4.1.1  Deﬁnitions


We begin with a few deﬁnitions illustrated in Figure 4.1:


Propagation delay time, tpd = maximum time from the


input crossing 50% to the output crossing 50%


Contamination delay time, tcd = minimum time from the  input crossing 50% to the output crossing 50%


Rise time, tr = time for a waveform to rise from 20% to  80% of its steady-state value


Fall time, tf = time for a waveform to fall from 80% to  20% of its steady-state value


Edge rate, trf = (tr + tf )/2


Intuitively, we know that when an input changes, the output will retain its old value for at least the contamination delay and take on its new value in at most the propagation delay. We sometimes


tpdf


tf


tr


t t


tpdr


FIGURE 4.1  Propagation delay and rise/fall times


Chapter 4      Delay


142


differentiate between the delays for the output rising, tpdr /tcdr , and the output falling,tpdf /tcdf . Rise/fall times are also sometimes called slopes or edge rates. Propagation and contamination delay times are also called max-time and min-time, respectively. The gate that charges or discharges a node is called the driver and the gates and wire being driven are called the load. Propagation delay is usually the most relevant value of interest, and is often simply called delay.


A timing analyzer computes the arrival times, i.e., the latest time at which each node in a block of logic will switch. The nodes are classiﬁed as inputs, outputs, and internal nodes. The user must specify the arrival time of inputs and the time data is required at the outputs. The arrival time ai at internal node i depends on the propagation delay of the gate driving i and the arrival times of the inputs to the gate:


(4.1)


The timing analyzer computes the arrival times at each node and checks that the outputs arrive by their required time. The slack is the difference between the required and arrival times. Positive slack means that the circuit meets timing. Negative slack means that the circuit is not fast enough. Figure 4.2 shows nodes annotated with arrival times. If the outputs are all required at 200 ps, the circuit has 60 ps of slack.


A practical timing analyzer extends this arrival time model to account for a number of effects. Arrival times and propagation delays are deﬁned separately for rising and falling transitions. The delay of a gate may be different from different inputs. Earliest arrival times can also be computed based on contamination delays. Considering all of these factors gives a window over which the gate may switch and allows the timing analyzer to verify that setup and hold times are satisﬁed at each register.


4.1.2  Timing Optimization


In most designs there will be many logic paths that do not require any conscious effort when it comes to speed. These paths are already fast enough for the timing goals of the system. However, there will be a number of critical paths that limit the operating speed of the system and require attention to timing details. The critical paths can be affected at four main levels:


The architectural/microarchitectural level


The logic level


The circuit level


The layout level


j fanin i


pdi


} +


max


I0a0 = 20


a7 = 60


a8 = 80


a9 = 110O9


O12


a10 = 90


a11 = 60


a12 = 140


a1 = 30 a2 = 50 a3 = 20 a4 = 20 a5 = 20 a6 = 20


I1 I2 I3 I4 I5 I6


FIGURE 4.2  Arrival time example


4.2      Transient Response 143


The most leverage is achieved with a good microarchitecture. This requires a broad knowledge of both the algorithms that implement the function and the technology being targeted, such as how many gate delays ﬁt in a clock cycle, how quickly addition occurs,how fast memories are accessed, and how long signals take to propagate along a wire.


Trade-offs at the microarchitectural level include the number of pipeline stages, the number of execution units (parallelism), and the size of memories.


The next level of timing optimization comes at the logic level. Trade-offs include types of functional blocks (e.g., ripple carry vs. lookahead adders), the number of stages of gates in the clock cycle, and the fan-in and fan-out of the gates. The transformation from function to gates and registers can be done by experience, by experimentation, or, most often, by logic synthesis. Remember, however, that no amount of skillful logic design can overcome a poor microarchitecture.


Once the logic has been selected, the delay can be tuned at the circuit level by choosing transistor sizes or using other styles of CMOS logic. Finally, delay is dependent on the layout. The ﬂoorplan (either manually or automatically generated) is of great importance because it determines the wire lengths that can dominate delay. Good cell layouts can also reduce parasitic capacitance.


Many RTL designers never venture below the microarchitectural level. A common design practice is to write RTL code, synthesize it (allowing the synthesizer to do the timing optimizations at the logic, circuit, and placement levels) and check if the results are fast enough. If they are not, the designer recodes the RTL with more parallelism or pipelining, or changes the algorithm and repeats until the timing constraints are satisﬁed. Timing analyzers are used to check timing closure, i.e., whether the circuit meets all of the timing constraints.


Without an understanding of the lower levels of abstraction where the synthesizer is working,a designer may have a difﬁcult time achieving timing closure on a challenging system.


This chapter focuses on the logic and circuit optimizations of selecting the number of stages of logic, the types of gates, and the transistor sizes. We begin by examining the transient response of an inverter. Using the device models from Chapter 2, we can write differential equations for voltage as a function of time to calculate delay. Unfortunately,these equations are too complicated to give much insight, yet too simple to give accurate results. This chapter focuses on developing simpler models that offer the designer more intuition. The RC delay model approximates a switching transistor with an effective resistance and provides a way to estimate delay using arithmetic rather than differential equations. The method of Logical Effort simpliﬁes the model even further and is a powerful way to evaluate delay in circuits. The chapter ends with a discussion of other delay models used for timing analysis.


4.2 Transient Response


The most fundamental way to compute delay is to develop a physical model of the circuit of interest, write a differential equation describing the output voltage as a function of input voltage and time, and solve the equation. The solution of the differential equation is called the transient response, and the delay is the time when the output reaches VDD /2.


The differential equation is based on charging or discharging of the capacitances in the circuit. The circuit takes time to switch because the capacitance cannot change its voltage instantaneously. If capacitance C is charged with a current I, the voltage on the capacitor varies as:


(4.2)


I CdVdt=


144


Every real circuit has some capacitance. In an integrated circuit, it typically consists of the gate capacitance of the load along with the diffusion capacitance of the driver’s own transistors, as discussed in Section 2.3. As will be explored further in Section 6.2.2, wires that connect transistors together often contribute the majority of the capacitance. The transistor current depends on the input (gate)and output (source/drain) voltages. To illustrate these points, consider computing the step response of an inverter.


Figure 4.3(a) shows an inverter X1 driving another inverter X2 at the end of a wire. Suppose a voltage step from 0 to VDD is applied to node A and we wish to compute the propagation delay, tpdf , through X1, i.e., the delay from the input step until node B crosses VDD/2.


These capacitances are annotated on Figure 4.3(b). There are diffusion capacitances between the drain and body of each transistor and between the source and body of each transistor: Cdb and Csb . The gate capacitance Cgs of the transistors in X2 are part of the load. The wire capacitance is also part of the load. The gate capacitance of the transistors in X1 and the diffusion capacitance of the transistors in X2 do not matter because they do not connect to node B. The source-to-body capacitors Csbn1 and Csbp1 have both terminals tied to constant voltages and thus do not contribute to the switching capacitance. It is also irrelevant whether the second terminal of each capacitor connects to ground or power because both are constant supplies, so for the sake of simplicity, we can draw all of the capacitors as if they are connected to ground. Figure 4.3(c) shows the equivalent circuit diagram in which all the capacitances are lumped into a single Cout.


Before the voltage step is applied, A = 0. N1 is OFF, P1 is ON, and B = VDD.


After the step, A = 1. N1 turns ON and P1 turns OFF and B drops toward 0.


The rate of change of the voltage VB at node B depends on the output capacitance and on the current through N1:


(4.3)


Suppose the transistors obey the long-channel models. The current depends on whether N1 is in the linear or saturation regime. The gate is at VDD, the source is at 0, and the drain is at VB. Thus, Vgs = VDD and Vds = VB. Initially, Vds = VDD > Vgs – Vt , so N1 is in saturation. As VB falls below VDD – Vt , N 1 enters the linear regime. Substituting EQ (2.10) and rearranging, we ﬁnd the differential equation governing VB.


(4.4)


During saturation, the current is constant and VB drops linearly until it reaches VDD Vt . Thereafter, the differential equation becomes nonlinear. The response can be computed numerically. The rising output response is computed in an analogous fashion and is symmetric with the falling response if p = n.


CdVdt


dsn


dV dt


VV


2V


X1 P1 N1


X1 P1


P1 N1


X1 N1


N2 P2 X2


wire


Csbn1 Cdbn1 Cdbp1 Csbp1


Cwire


Cgsp2


Cgsn2


Cout = Cdbn1 + Cdbp1 +Cwire +


Cgsn2 + Cgsp2


FIGURE 4.3  Capacitances for inverter  delay calculations


4.2      Transient Response 145


Example 4.1


Plot the response of the inverter to a step input and determine the


propagation delay. Assume that the nMOS transistor width is


1 m and the output capacitance is 20 fF. Use the following longchannel model parameter values for a 65-nm process: L = 50 nm,


VDD = 1.0 V, Vt = 0.3 V, tox = 10.5 Å, = 80 cm2/V · s.


SOLUTION: The response is plotted in Figure 4.4. The input, A, rises


at 10 ps. The solid blue line indicates the step response predicted by


the long-channel model. The output, B, initially follows a straight


line, as the saturated nMOS transistor behaves as a constant current


source. B eventually curves as it approaches 0 and the nMOS transistor enters the linear regime. The propagation delay is 12.5 ps.


The solid black line indicates the step response predicted by


SPICE. The propagation delay is 15.8 ps, which is longer because


the mobility used in the long-channel model didn’t fully account for


velocity saturation and mobility degradation effects. SPICE shows


that B also initially rises momentarily before falling. This effect is called bootstrapping and will be discussed in Section 4.4.6.6. The dashed black line shows an RC model that approximates the nMOS transistor as a 1 k  resistor when it is ON. The propagation delay predicted by the RC model matches SPICE fairly well, although the fall time is overestimated. RC models will be explored further in Section 4.3.


In a real circuit, the input comes from another gate with a nonzero rise/fall time. This input can be approximated as a ramp with the same rise/fall time. Again, let us consider a rising ramp and a falling output and examine how the nonzero rise time affects the propagation delay.


Assuming Vtn + |Vtp| < VDD, the ramp response includes three phases, as shown in Table 4.1. When A starts to rise, N1 remains OFF and B remains at VDD. When A reaches Vtn , N1 turns ON. It ﬁghts P1 and starts to gradually pull B down toward an intermediate value predicted by the DC circuit response examined in Section 2.5. When A gets close enough to VDD, P1 turns OFF and B falls to 0 unopposed. Thus, we can write the differential equations for VB in each phase:


(4.5)


TABLE 4.1  Phases of inverter ramp response


Phase


VA


N1


P1


VB


0 < VA < Vtn


OFF ON


Vtn < VA < VDD  |Vtp|


Intermediate


VDD  |Vtp| < VA < VDD


ON OFF


Falling toward 0


Phase 1


Phase 2


V V dV


dt


dsp


B (RC Model)


(V)


20p


40p


60p


80p


t(s)


FIGURE 4.4


Inverter step response


146


The currents could be estimated using the long-channel model again, but working out the full model is tedious and offers little insight. The key observation is that the propagation delay increases because N1 is not fully ON right away and because it must ﬁght P1 in Phase


2. Section 4.4.6.1 develops a model for how propagation delay increases with rise time.


More complex gates such as NANDs or NORs have transistors in series. Each series transistor sees a smaller Vds and delivers less current. The current through the transistors can be found by solving the simultaneous nonlinear differential equations, which again is best done numerically. If the transistors have the same dimensions and the load is the same, the delay will increase with the number of series transistors.


This section has shown how to develop a physical model for a circuit, write the differential equation for the model, and solve the equation to compute delay. The physical modeling shows that the delay increases with the output capacitance and decreases with the driver current. The differential equations used the long-channel model for transistor current, which is inaccurate in modern processes. The equations are also too nonlinear to solve in closed form, so they have to be solved numerically and give little insight about delay. Circuit simulators automate this process using more accurate delay equations and give good predictions of delay, but offer even less insight. The rest of this chapter is devoted to developing simpler delay models that offer more insight and tolerable accuracy.


4.3 RC Delay Model


RC delay models approximate the nonlinear transistor I-V and C-V characteristics with an average resistance and capacitance over the switching range of the gate. This approximation works remarkably well for delay estimation despite its obvious limitations in predicting detailed analog behavior.


4.3.1  Effective Resistance


The RC delay model treats a transistor as a switch in series with a resistor. The effective resistance is the ratio of Vds to Ids averaged across the switching interval of interest.


A unit nMOS transistor is deﬁned to have effective resistance R. The size of the unit transistor is arbitrary but conventionally refers to a transistor with minimum length and minimum contacted diffusion width (i.e., 4/2 ). Alternatively, it may refer to the width of the nMOS transistor in a minimum-sized inverter in a standard cell library. An nMOS transistor of k times unit width has resistance R/k because it delivers k times as much current. A unit pMOS transistor has greater resistance, generally in the range of 2R–3R,because of its lower mobility. Throughout this book we will use 2R for examples to keep arithmetic simple. R is typically on the order of 10 k  for a unit transistor. Sections 4.3.7 and 8.4.5 examine how to determine the effective resistance for transistors in a particular process.


According to the long-channel model, current decreases linearly with channel length and hence resistance is proportional to L. Moreover, the resistance of two transistors in series is the sum of the resistances of each transistor (see Exercise 2.2). However, if a transistor is fully velocity-saturated, current and resistance become independent of channel length. Real transistors operate somewhere between these two extremes. This also means that the resistance of transistors in series is somewhat lower than the sum of the resistances, because series transistors see smaller Vds and are less velocity-saturated. The effect is more pronounced for nMOS transistors than pMOS because of the higher mobility and


4.3      RC Delay Model 147


greater degree of velocity saturation. The simplest approach is to neglect velocitysaturation for hand calculations, but recognize that series transistors will be somewhat faster than predicted.


4.3.2  Gate and Diffusion Capacitance


Each transistor also has gate and diffusion capacitance. We deﬁne C to be the gate capacitance of a unit transistor of either ﬂavor. A transistor of k times unit width has capacitance kC. Diffusion capacitance depends on the size of the source/drain region. Using the approximations from Section 2.3.1, we assume the contacted source or drain of a unit transistor to also have capacitance of about C. Wider transistors have proportionally greater diffusion capacitance. Increasing channel length increases gate capacitance proportionally but does not affect diffusion capacitance.


Although capacitances have a nonlinear voltage dependence, we use a single average value. As discussed in Section 2.3.1, we roughly estimate C for a minimum length transistor to be 1 fF/ m of width. In a 65 nm process with a unit transistor being 0.1 m wide, C is thus about 0.1 fF.


4.3.3  Equivalent RC Circuits


Figure 4.5 shows equivalent RC circuit models for nMOS and pMOS transistors of width k with contacted diffusion on both source and drain. The pMOS transistor has approximately twice the resistance of the nMOS transistor because holes have lower mobility than electrons. The pMOS capacitors are shown with VDD as their second terminal because the n-well is usually tied high. However, the behavior of the capacitor from a delay perspective is independent of the second terminal voltage so long as it is constant. Hence, we sometimes draw the second terminal as ground for convenience.


The equivalent circuits for logic gates are assembled from the individual transistors. Figure 4.6 shows the equivalent circuit for a fanout-of-1 inverter with negligible wire capacitance. The unit inverters of Figure 4.6(a) are composed from an nMOS transistor of unit size and a pMOS transistor of twice unit


s d


kC


kC kC


R/k


2R/k


FIGURE 4.5


Equivalent circuits for transistors


2C 2C


C 2C


6C


Nonswitching capacitances:irrelevant


capacitances


FIGURE 4.6  Equivalent circuit for an inverter


148


width to achieve equal rise and fall resistance. Figure 4.6(b) gives an equivalent circuit, showing the ﬁrst inverter driving the second inverter’s gate. If the input A rises, the nMOS transistor will be ON and the pMOS OFF. Figure 4.6(c)illustrates this case with the switches removed. The capacitors shorted between two constant supplies are also removed because they are not charged or discharged. The total capacitance on the output Y is 6C.


Example 4.2


Sketch a 3-input NAND gate with transistor widths chosen to achieve effective rise and fall resistance equal to that of a unit inverter (R). Annotate the gate with its gate and diffusion capacitances. Assume all diffusion nodes are contacted. Then sketch equivalent circuits for the falling output transition and for the worst-case rising output transition.


SOLUTION: Figure 4.7(a) shows such a gate. The three nMOS transistors are in series so the resistance is three times that of a single transistor. Therefore,each must be three times unit width to compensate. In other words, each transistor has resistance R/3 and the series combination has resistance R.


The two pMOS transistors are in parallel. In the worst case (with one of the inputs low), only one of the pMOS transistors is ON. Therefore, each must be twice unit width to have resistance R.


Technicians working at a light table then cut each level of layout onto sheets of rubylith to make the masks, as shown in Figure 3.38(b). Rubylith is a two-layered material with a base of heavy transparent Mylar and a thin ﬁlm of red cellophane-like material. The red ﬁlm was then peeled away where transistors or wires should be formed. The designer and technician spent days inspecting the rubylith for peeling errors and unintended cuts.


The sheets had to be handled with great care to avoid rubbing off pieces. Corrections were performed with a surgical scalpel and metal ruler to add new wires, or with red tape to remove objects. The ﬁnal result was checked with a 7 times magnifying glass. Finally, the rubylith sheets were sent to a mask vendor to be optically reduced to form the masks.


Despite all this care, the initial version of Intel’s ﬁrst product, the 3101 64-bit RAM, was actually a 63-bit RAM because of an error peeling the rubylith. Designers today still gripe at their tools, but the industry has come a long way.


Advances in semiconductor devices are usually presented at the International Electron Devices Meeting (IEDM). Table 3.2 summarizes key characteristics from Intel and IBM.


FIGURE 3.38  Hand-drawn layout: (a) standard cell, (b) cutting patterns onto rubylith (Reprinted from [Volk01] with permission of Intel Corporation.)


138


Process development has become so expensive that IBM has formed the Common Platform alliance with partners including Chartered Semiconductor, Samsung, Inﬁneon, and STMicro, to share the R&D costs. IBM offers both SOI and bulk processes; Table 3.2 focuses on their SOI devices that have better Idsat / Ioff ratios. All of the processes in this table are considered high-performance processes that focus on a high Idsat. Many manufacturers also offer low-power processes with higher threshold voltages and thicker oxides to reduce leakage, especially in battery-powered communications devices.


The transistor characteristics are listed for low-Vt transistors. Since the 130 nm generation, nearly all processes have offered a regular-Vt transistor offering an order of magnitude lower Ioff at the expense of a 15% reduction in Idsat. Some low-power processes provide a high-Vt transistor to reduce leakage by another order of magnitude. Most manufacturers use a separate implant mask to specify the threshold voltage, but Intel reduces manufacturing cost by using a slightly (~10%) longer channel length instead, which increases Vt on account of the short-channel effect [Rusu07].


Reported subthreshold slopes range from 85–100 mV/decade. DIBL coefﬁcients range from 100–130 mV/V and tend to get larger with technology scaling.


TABLE 3.2  CMOS process characteristics


Manufacturer


Intel


IBM


Feature Size f


nm


250 180 130 90


65


45


130 90


Reference


[Bohr96]


[Yang98] [Tyagi00] [Thompson02] [Bai04]


[Mistry07] [Natarajan08] [Sleight01] [Khare02] [Lee05]


[Narasimha06]


1.8 1.5 1.3 1.2


1.2 1


Lgate


180 140 70 50


35


60


4.1 3


1.5 1.2


2.3 1.85 1.05 1.15


Idsat-n


A/ m 700 940 1170 1449 1460 1360 1550 915 1000 1137 1140


Idsat-p


A/ m 320 420 600 725


880 1070 1210 520 480 700 800


nA/ m 1


100 400


100 100 100


100 200 200 200


no no no yes


yes yes yes


no no yes yes


High-k Gates


no no no no


no


yes yes


no no no


Gate Pitch


640 480 336 260


220 160 112.5 325 245


190


Metal1 Pitch


640 500 350 220


210 150 112.5 350 245


Metal Layers


Material


Al


Al Cu Cu


Cu Cu Cu


Cu Cu Cu Cu


Low-k Dielectric


none FSG FSG CDO CDO CDO CDO SiLK SiLK CDO Porous


3.9 3.55 3.6 2.9


2.9


2.75 2.4


SRAM Cell Size m2


10.26 5.59 2.09 1


0.57 0.346 0.171 1.8 0.99 0.65 0.37


Summary 139


CMOS process options and directions can greatly inﬂuence design decisions. Frequently,the combination of performance and cost possibilities in a new process can provide new product opportunities that were not available previously. Similarly, venerable processes can offer good opportunities with the right product.


One issue that has to be kept in mind is the ever-increasing cost of having a CMOS design fabricated in a leading-edge process. Mask cost for critical layers is in the vicinity of$100K per mask. A full mask set for a 65 nm process can exceed $1M in cost, and the price has been roughly doubling at each technology node. This in turn is reﬂected in the types of design and approaches to design that are employed for CMOS chips of the future.


For instance, making a design programmable so that it can have a longer product life is a good ﬁrst start. Chapter 14 covers these approaches in depth.


For more advanced reading on silicon processing, consult textbooks such as [Wolf00].


3.1 A 248 nm UV step and scan machine costs $10M and can produce 80 300 mm


diameter, 90 nm node wafers per hour. A 193 nm UV step and scan machine costs $40M and can process 20 300 mm diameter, 50 nm node wafers per hour. If the


machines have a depreciation period of four years, what is the difference in the cost  per chip for a chip that occupies 50 square mm at 90 nm resolution if the stepper is  used 10 times per process run for the critical layers?


Figure 4.7(b) shows the capacitances. Each input presents ﬁve units of gate capacitance to whatever circuit drives that input. Notice that the capacitors on source diffusions attached to the rails have both terminals shorted together so they are irrelevant to circuit operation. Figure 4.7(c)redraws the gate with these capacitances deleted and the remaining capacitances lumped to ground.


Figure 4.7(d) shows the equivalent circuit for the falling output transition. The output pulls down through the three series nMOS transistors.


Figure 4.7(e) shows the equivalent circuit for the rising output transition. In the worst case, the upper two inputs are 1 and the bottom one falls to 0.


The output pulls up through a single pMOS transistor. The upper two nMOS transistors are still on, so the diffusion capacitance between the series nMOS transistors must also be discharged.


4.3.4  Transient Response


Now, consider applying the RC model to estimate the step response of theﬁrst-order system shown in Figure 4.8. This system is a good model of an inverter sized for equal rise and fall delays. The system has a transfer function


(4.6)


and a step response


(4.7)


H s


sRC


( ) =+11


V t VDDtout e( ) = /


9C 3C 3C


3 3 3 2


5C


5C 2


3 3 3


3C 3C 3C


3C


2C


3 3 2


R/3


R/3 R/3


3C 3C 9C


Falling


Rising


FIGURE 4.7  Equivalent circuits  for a 3-input NAND gate


C Vout


FIGURE 4.8


First-order RC system


4.3      RC Delay Model 149


where = RC. The propagation delay is the time at which Vout reaches VDD /2, as shown in Figure 4.9.


tpd = RC ln 2


(4.8)


The factor of ln 2 = 0.69 is cumbersome. The effective resistance R is an empirical parameter anyway, so it is preferable to incorporate the factor of ln 2 to deﬁne a new effective resistance R = R ln 2. Now the propagation delay is simply R C. For the sake of convenience, we usually drop the prime symbols and just write


tpd = RC


(4.9)


where the effective resistance R is chosen to give the correct delay.


Figure 4.10 shows a second-order system. R1 and R2 might model the two series nMOS transistors in a NAND gate or an inverter driving a long wire with non-negligible resistance. The transfer function is


(4.10)


The function has two real poles and the step response is


(4.11)


with


(4.12)


EQ (4.12) is so complicated that it defeats the purpose of simplifying a CMOS circuit into an equivalent RC network. However, it can be further approximated as a ﬁrstorder system with a single time constant:


s R C R R C


s R C R C


( ) =+


1 1


1 1 2 2


V t VDD


e e


( ) =


/


4 1 1


,


* *


±


R C R R C


R C


RRRCCC* *;2121


Vout VDD


ln 2


FIGURE 4.9  First-order step response


R1


C1 R2


C2


FIGURE 4.10  Second-order  RC system


150


(4.13)


This approximation works best when one time constant is signiﬁcantly bigger than the other [Horowitz84]. For example, if R1 = R2 = R and C1 = C2 = C, then 1 = 2.6 RC,2 = 0.4 RC, = 3 RC and the second-order response and its ﬁrst-order approximation are shown in Figure 4.11. The error in estimated propagation delay from the ﬁrst-order approximation is less than 7%. Even in the worst case, where the two time constants are equal, the error is less than 15%. The single time constant is a bad description of the behavior of intermediate nodes. For example, the response at n1 cannot be described well by a single time constant. However, CMOS designers are primarily interested in the delay to the output of a gate, where the approximation works well. In the next section, we will see how to ﬁnd a simple single time constant approximation for general RC tree circuits using the Elmore delay model.


Second-order Response


First-order Approximation


FIGURE 4.11  Comparison of second-order response to ﬁrst-order  approximation


4.3.5  Elmore Delay


In general, most circuits of interest can be represented as an RC tree, i.e., an RC circuit with no loops. The root of the tree is the voltage source and the leaves are the capacitors at the ends of the branches. The Elmore delay model [Elmore48] estimates the delay from a source switching to one of the leaf nodes changing as the sum over each node i of the capacitance Ci on the node, multiplied by the effective resistance Ris on the shared path from the source to the node and the leaf. Application of Elmore delay is best illustrated through examples.


(4.14)


Example 4.3


Compute the Elmore delay for Vout in the 2nd order RC system from Figure 4.10.


SOLUTION: The circuit has a source and two nodes. At node n1, the capacitance is C1 and the resistance to the source is R1. At node Vout, the capacitance is C2 and the resistance to the source is (R1 + R2). Hence, the Elmore delay is tpd = R1C1 + (R1 + R2)C2, just as the single time constant predicted in EQ (4.13). Note that the effective resistances should account for the factor of ln 2.


pd


is i


4.3      RC Delay Model 151


Example 4.4


Estimate tpd for a unit inverter driving m identical unit inverters.


SOLUTION: Figure 4.12 shows an equivalent circuit for the falling transition. Each load inverter presents 3C units of gate capacitance, for a total of 3mC. The output node also sees a capacitance of 3C from the drain diffusions of the driving inverter. This capacitance is called parasitic because it is an undesired side-effect of the need to make the drain large enough to contact. The parasitic capacitance is independent of the load that the inverter is driving. Hence, the total capacitance is (3 + 3m)C. The resistance is R, so the Elmore delay is tpd = (3 + 3m)RC. The equivalent circuit for the rising transition gives the same results.


Example 4.5


Repeat Example 4.4 if the driver is w times unit size.


SOLUTION: Figure 4.13 shows the equivalent circuit. The driver transistors are w times as wide, so the effective resistance decreases by a factor of w . The diffusion capacitance increases by a factor of w. The Elmore delay is tpd = ((3w + 3m)C)(R/w) = (3 + 3m/w)RC.


Deﬁne the fanout of the gate, h, to be the ratio of the load capacitance to the input capacitance. (Diffusion capacitance is not counted in the fanout.) The load capacitance is 3mC. The input capacitance is 3wC. Thus, the inverter has a fanout of h = m/w and the delay can be written as (3 + 3h)RC.


Example 4.6


If a unit transistor has R = 10 k  and C = 0.1 fF in a 65 nm process, compute the delay,in picoseconds, of the inverter in Figure 4.14 with a fanout of h = 4.


SOLUTION: The RC product in the 65 nm process is (10 k )(0.1 fF) = 1 ps. For h = 4,the delay is (3 + 3h)(1 ps) = 15 ps. This is called the fanout-of-4 (FO4) inverter delay and is representative of gate delays in a typical circuit. Remember that a picosecond is a trillionth of a second. The inverter can switch about 66 billion times per second. This stunning speed partially explains the fantastic capabilities of integrated circuits.


It is often helpful to express delay in a process-independent form so that circuits can be compared based on topology rather than speed of the manufacturing process. Moreover, with a process-independent measure for delay, knowledge of circuit speeds gained while working in one process can be carried over to a new process. Observe that the delay of an ideal fanout-of-1 inverter with no parasitic capacitance is = 3RC 1 [Sutherland99].


We denote the normalized delay d relative to this inverter delay:


(4.15)


1Do not confuse this deﬁnition of = 3RC, the delay of a parasitic-free fanout-of-1 inverter, with Mead and Conway’s deﬁnition [Mead80] = RC, the delay of an nMOS transistor driving its own gate, or with the use of  as an arbitrary time constant. For the remainder of this text, = 3RC.


tpd


3mC


Diffusion/Parasitic Cap


Load


Cap


R/w


3wC Diffusion Cap


Load Cap


FIGURE 4.12  Equivalent  circuit for inverter


FIGURE 4.13  Equivalent  circuit for wider inverter


FIGURE 4.14  Fanout-of-4 (FO4) inverter


152


Hence, the delay of a fanout-of-h inverter can be written in normalized form as d = h + 1,assuming that diffusion capacitance approximately equals gate capacitance. An FO4 inverter has a delay of 5 . If diffusion capacitance were slightly higher or lower, the FO4 delay would change by only a small amount. Thus, circuit delay measured in FO4 delays is nearly constant from one process to another.2


Example 4.7


Estimate tpdf and tpdr for the 3-input NAND gate from Example 4.2 if the output is loaded with h identical NAND gates.


SOLUTION: Each NAND gate load presents 5 units of capacitance on a given input. Figure 4.15(a) shows the equivalent circuit including the load for the falling transition. Node n1 has capacitance 3C and resistance of R/3 to ground. Node n2 has capacitance 3C and resistance (R/3 + R/3) to ground. Node Y has capacitance (9 + 5h)C and resistance (R/3 + R/3 +R/3) to ground. The Elmore delay for the falling output is the sum of these RC products, tpdf = (3C)(R/3) + (3C)(R/3 + R/3) + ((9 + 5h)C)(R/3


+ R/3 + R/3) = (12 + 5h)RC.


Figure 4.15(b) shows the equivalent circuit for the falling transition. In the worst case, the two inner inputs are 1 and the outer input falls. Y is pulled up to VDD through a single pMOS transistor. The ON nMOS transistors contribute parasitic capacitance that slows the transiton. Node Y has capacitance (9 + 5h)C and resistance R to the VDD supply. Node n2 has capacitance 3C. The relevant resistance is only R, not(R + R/3), because the output is being charged only through R. This is what is meant by the resistance on the shared path from the source (VDD) to the node (n2) and the leaf(Y ). Similarly, node n1 has capacitance 3C and resistance R. Hence, the Elmore delay for the rising output is tpdr = (15 + 5h)RC. The R/3 resistances do not contribute to this delay. Indeed, they shield the diffusion capacitances, which don’t have to charge all the way up before Y rises. Hence, the Elmore delay is conservative and the actual delay is somewhat faster.


Although the gate has equal resistance pulling up and down, the delays are not quite equal because of the capacitances on the internal nodes.


Example 4.8


Estimate the contamination delays tcdf and tcdr for the 3-input NAND gate from Example 4.2 if the output is loaded with h identical NAND gates.


SOLUTION: The contamination delay is the fastest that the gate might switch. For the falling transition, the best case is that the bottom two nMOS transistors are already ON when the top one turns ON. In such a case, the diffusion capacitances on n1 and n2 have already been discharged and do not contribute to the delay. Figure 4.16(a) shows the equivalent circuit and the delay is tcdf = (9 + 5h)RC.


2This assumes that the circuit is dominated by gate delay. The RC delay of long wires does not track well with the gate delay, as will be explored in Chapter 6.


R/3 R/3 R/3


(9 + 5h)C


3C 3C


n1 n2


FIGURE 4.15  Equivalent circuits  for loaded gate


FIGURE 4.16  Equivalent circuits  for contamination delay


4.3      RC Delay Model 153


For the rising transition, the best case is that all three pMOS transistors turn on simultaneously. The nMOS transistors turn OFF, so n1 and n2 are not connected to the output and do not contribute to delay. The parallel transistors deliver three times as much current, as shown in Figure 4.16(b), so the delay is tcdr = (3 + (5/3)h)RC.


In all of the Examples, the delay consists of two components. The parasitic delay is the time for a gate to drive its own internal diffusion capacitance. Boosting the width of the transistors decreases the resistance but increases the capacitance so the parasitic delay is ideally independent of the gate size.3 The effort delay depends on the ratio h of external load capacitance to input capacitance and thus changes with transistor widths. It also depends on the complexity of the gate. The capacitance ratio is called the fanout or electrical effort and the term indicating gate complexity is called the logical effort. For example, an inverter has a delay of d = h + 1, so the parasitic delay is 1 and the logical effort is also 1. The NAND3 has a worst case delay of d = (5/3)h + 5. Thus, it has a parasitic delay of 5 and a logical effort of 5/3. These delay components will be explored further in Section 4.4.


4.3.6  Layout Dependence of Capacitance


In a good layout, diffusion nodes are shared wherever possible to reduce the diffusion capacitance. Moreover, the uncontacted diffusion nodes between series transistors are usually smaller than those that must be contacted. Such uncontacted nodes have less capacitance (see Sections 2.3.3 and


8.4.4), although we will neglect the difference for hand calculations. A conservative method of estimating capacitances


before layout is to assume uncontacted diffusion between series


transistors and contacted diffusion on all other nodes. However, a more accurate estimate can be made once the layout is


known.


Example 4.9


Figure 4.17(a) shows a layout of the 3-input NAND gate.


A single drain diffusion region is shared between two of the pMOS transistors. Estimate the actual diffusion capacitance from the layout.


SOLUTION: Figure 4.17(b) redraws the schematic with these capacitances lumped to ground. The output node has the following diffusion capacitances: 3C from the nMOS transistor drain, 2C from the isolated pMOS transistor drain,and 2C from a pair of pMOS drains that share a contact.


Thus, the actual diffusion capacitance on the output is 7C,rather than 9C predicted in Figure 4.15.


3Gates with wider transistors may use layout tricks so the diffusion capacitance increases less than linearly with width, slightly decreasing the parasitic delay of large gates as discussed in Section 4.3.6.


Shared


Contacted Diffusion


Merged


Uncontacted Diffusion


Isolated Contacted Diffusion


7C 3C 3C


(b)VDD


FIGURE 4.17  3-input NAND annotated with diffusion  capacitances extracted from the layout


154


The diffusion capacitance can also be decreased by folding wide transistors.


Figure 4.18(a) shows a conventional layout of a 24/12  inverter. Because a unit (4) transistor has diffusion capacitance C, the inverter has a total diffusion capacitance of 9C. The folded layout in Figure 4.18(b) constructs each transistor from two parallel devices of half the width. Observe that the diffusion area has shrunk by a factor of two, reducing the diffusion capacitance to 4.5C. In general, folded layouts offer lower parasitic delay than unfolded layouts. The folded layout may also ﬁt better in a standard cell of limited height, and the shorter polysilicon lines have lower resistance. For these reasons, wide transistors are folded whenever possible. In some nanometer processes (generally 45 nm and below), transistor gates are restricted to a limited choice of pitches to improve manufacturability and reduce variability. For example, the spacing between polysilicon for gates may always be the contacted transistor pitch, even if no contact is required. Moreover,using a single standard transistor width may reduce variability.


4.3.7  Determining Effective Resistance


The effective resistance can be determined through simulation or analysis. Section 8.4.5 explains the simulation technique, which is most accurate. This section, however, offers an analysis that provides more insight into the relationship of resistance to other parameters.


Recall that the effective resistance is the average value of Vds / Ids of a transistor during a switching event. As mentioned in Section 4.3.4, the resistance is scaled by a factor of ln 2 so that propagation delay can be written as an RC product. For the step response of a rising input, we are interested in the time for the output to discharge from VDD to VDD / 2 through an nMOS transistor. If the transistor is sufﬁciently velocity-saturated that Vdsat < VDD / 2, then the transistor will remain in the saturation region throughout this transition and the current is roughly constant at Idsat. In such a case, the effective resistance is


(4.16)


Channel length modulation and DIBL cause the current to decrease somewhat with Vds in a real transistor, slightly increasing the effective resistance.


More importantly, the input has a nonzero rise time and we are interested in the time from when the input rises through VDD / 2 until the output falls through VDD / 2. Assume that the input and output slopes are equal and that the output starts to fall when the input passes through VDD / 2. Then, the output will reach VDD / 2 when the input reaches VDD, as shown in Figure 4.19.


Deﬁne the transistor current to be IL at the start of the transition (when Vgs = VDD / 2, Vds = VDD) and IH at the end of the transition (when Vgs = VDD, Vds = VDD / 2), as shown in Figure 4.20. Then,the transistor can be approximated during the switching event as a current source Ieff that is the average of these two extremes [Na02]:


(4.17)


IdV


V I


step


3 2 4


I IH L


=+2


Vin Vout


VDD VDD/2  0


FIGURE 4.18  Layout styles:


(a) conventional, (b) folded


FIGURE 4.19  Propagation delay  with input and output approximated  as ramps


Vin = 1.0


Vin = 0.5


200 400 600 800


IL


FIGURE 4.20  Approximate switching trajectory


4.4      Linear Delay Model 155


The time for the output to discharge to VDD / 2 is thus:


(4.18)


Equating this to tpd = RC gives


(4.19)


4.4 Linear Delay Model


The RC delay model showed that delay is a linear function of the fanout of a gate. Based on this observation, designers further simplify delay analysis by characterizing a gate by the slope and y-intercept of this function. In general, the normalized delay of a gate can be expressed in units of  as


d = f + p


(4.20)


p is the parasitic delay inherent to the gate when no load is attached. f is the effort delay or stage effort that depends on the complexity and fanout of the gate:


f = gh


(4.21)


The complexity is represented by the logical effort, g [Sutherland99]. An inverter is deﬁned to have a logical effort of 1. More complex gates have greater logical efforts, indicating that they take longer to drive a given fanout. For example, the logical effort of the 3-input NAND gate from the previous example is 5/3. A gate driving h identical copies of itself is said to have a fanout or electrical effort of h. If the load does not contain identical copies of the gate, the electrical effort can be computed as


(4.22)


where Cout is the capacitance of the external load being driven and Cin is the


input capacitance of the gate.4


Figure 4.21 plots normalized delay vs. electrical effort for an idealized


inverter and 3-input NAND gate. The y-intercepts indicate the parasitic delay,


i.e., the delay when the gate drives no load. The slope of the lines is the logical


effort. The inverter has a slope of 1 by deﬁnition. The NAND has a slope of 5/3.


The remainder of this section explores how to estimate the logical effort


and parasitic delay and how to use the linear delay model.


4Some board-level designers say a device has a fanout of h when it drives h other devices, even if the other devices have different capacitances. This deﬁnition would not be useful for calculating delay and is best avoided in VLSI design. The term electrical effort avoids this potential confusion and emphasizes the parallels with logical effort.


CV


=2


RVI


I I


= =+2


hCC= outin


Electrical Effort:h = Cout/Cin


Inverter


3-input NAND


g = 1


p = 1


d = h + 1 g = 5/3


p = 3


d = (5/3)h + 3


Effort Delay: f


Parasitic Delay: p 0 1 2 3 4 5


0 1 2 3 4 5 6 7 8


FIGURE 4.21


Normalized delay vs. fanout


156


4.4.1  Logical Effort


Logical effort of a gate is deﬁned as the ratio of the input capacitance of the gate to the input capacitance of an inverter that can deliver the same output current. Equivalently, logical effort indicates how much worse a gate is at producing output current as compared to an inverter, given that each input of the gate may only present as much input capacitance as the inverter.


Logical effort can be measured in simulation from delay vs. fanout plots as the ratio of the slope of the delay of the gate to the slope of the delay of an inverter, as will be discussed in Section 8.5.3. Alternatively, it can be estimated by sketching gates. Figure 4.22 shows inverter, 3-input NAND, and 3-input NOR gates with transistor widths chosen to achieve unit resistance, assuming pMOS transistors have twice the resistance of nMOS transistors.5 The inverter presents three units of input capacitance. The NAND presentsﬁve units of capacitance on each input, so the logical effort is 5/3. Similarly, the NOR presents seven units of capacitance, so the logical effort is 7/3. This matches our expectation that NANDs are better than NORs because NORs have slow pMOS transistors in series.


Table 4.2 lists the logical effort of common gates. The effort tends to increase with the number of inputs. NAND gates are better than NOR gates because the series transistors are nMOS rather than pMOS. Exclusive-OR gates are particularly costly and have different logical efforts for different inputs. An interesting case is that multiplexers built from ganged tristates, as shown in Figure 1.29(b), have a logical effort of 2 independent of the number of inputs. This might at ﬁrst seem to imply that very large multiplexers are just as fast as small ones. However, the parasitic delay does increase with multiplexer size;hence, it is generally fastest to construct large multiplexers out of trees of 4-input multiplexers [Sutherland99].


4.4.2  Parasitic Delay


The parasitic delay of a gate is the delay of the gate when it drives zero load. It can be estimated with RC delay models. A crude method good for hand calculations is to count only diffusion capacitance on the output node. For example, consider the gates in Figure 4.22,assuming each transistor on the output node has its own drain diffusion contact. Transistor widths were chosen to give a resistance of R in each gate. The inverter has three units of diffusion capacitance on the output, so the parasitic delay is 3RC = . In other words,


5This assumption is made throughout the book. Exercises 4.19–4.20 explore the effects of different relative resistances (see also [Sutherland99]). The overall conclusions do not change very much, so the simple model is good enough for most hand estimates. A simulator or static timing analyzer should be used when more accurate results are required.


TABLE 4.2  Logical effort of common gates Gate Type


Number of Inputs


inverter


NAND


4/3


5/3


6/3


(n + 2)/3


NOR


7/3


9/3


(2n + 1)/3


tristate, multiplexer


XOR, XNOR


4, 4


6, 12, 6 8, 16, 16, 8


FIGURE 4.22  Logic gates  sized for unit resistance


(c)A


3 3


Cin = 3 g = 3/3


Cin = 5 g = 5/3


Cin = 7 g = 7/3


4.4      Linear Delay Model 157


the normalized parasitic delay is 1. In general, we will call the normalized parasitic delay pinv . pinv is the ratio of diffusion capacitance to gate capacitance in a particular process. It is usually close to 1 and will be considered to be 1 in many examples for simplicity. The 3-input NAND and NOR each have 9 units of diffusion capacitance on the output, so the parasitic delay is three times as great (3pinv, or simply 3). Table 4.3 estimates the parasitic delay of common gates. Increasing transistor sizes reduces resistance but increases capacitance correspondingly, so parasitic delay is, on ﬁrst order, independent of gate size. However, wider transistors can be folded and often see less than linear increases in internal wiring parasitic capacitance, so in practice, larger gates tend to have slightly lower parasitic delay.


This method of estimating parasitic delay is obviously crude. More reﬁned estimates use the Elmore delay counting internal parasitics, as in Example 4.7, or extract the delays from simulation. The parasitic delay also depends on the ratio of diffusion capacitance to gate capacitance. For example, in a silicon-on-insulator process in which diffusion capacitance is much less, the parasitic delays will be lower. While knowing the parasitic delay is important for accurately estimating gate delay, we will see in Section 4.5 that the best transistor sizes for a particular circuit are only weakly dependent on parasitic delay. Hence,crude estimates tend to be sufﬁcient to reach a good circuit design.


Nevertheless, it is important to realize that parasitic delay grows more than linearly with the number of inputs in a real NAND or NOR circuit. For example, Figure 4.23 shows a model of an n-input NAND gate in which the upper inputs were all 1 and the bottom input rises. The gate must discharge the diffusion capacitances of all of the internal nodes as well as the output. The Elmore delay is


(4.23)


TABLE 4.3  Parasitic delay of common gates Gate Type


2n


R nC


iR


nnC


n RC


i n


( )( )


5 2


n n n n


R/n R/n R/n


R/n


nC


3nC


FIGURE 4.23 n-input NAND gate parasitic delay


158


This delay grows quadratically with the number of series transistors n, indicating that beyond a certain point it is faster to split a large gate into a cascade of two smaller gates.


We will see in Section 4.4.6.5 that the coefﬁcient of the n2 term tends to be even larger in real circuits than in this simple model because of gate-source capacitance. In practice, it is rarely advisable to construct a gate with more than four or possibly ﬁve series transistors.


When building large fan-in gates, trees of NAND gates are better than NOR gates because the NANDs have lower logical effort.


4.4.3  Delay in a Logic Gate


Consider two examples of applying the linear delay model to logic gates.


Example 4.10


Use the linear delay model to estimate the delay of the fanout-of-4 (FO4) inverter from Example 4.6. Assume the inverter is constructed in a 65 nm process with = 3 ps.


SOLUTION: The logical effort of the inverter is g = 1, by deﬁnition. The electrical effort is 4 because the load is four gates of equal size. The parasitic delay of an inverter is pinv  1. The total delay is d = gh + p = 1 × 4 + 1 = 5 in normalized terms, or tpd = 15 ps in absolute terms.


Often path delays are expressed in terms of FO4 inverter delays. While not all designers are familiar with the  notation, most experienced designers do know the delay of a fanout-of-4 inverter in the process in which they are working. can be estimated as 0.2 FO4 inverter delays. Even if the ratio of diffusion capacitance to gate capacitance changes so pinv = 0.8 or 1.2 rather than 1, the FO4 inverter delay only varies from 4.8 to 5.2. Hence, the delay of a gate-dominated logic block expressed in terms of FO4 inverters remains relatively constant from one process to another even if the diffusion capacitance does not.


As a rough rule of thumb, the FO4 delay for a process (in picoseconds) is 1/3 to 1/2 of the drawn channel length (in nanometers). For example, a 65 nm process with a 50 nm channel length may have an FO4 delay of 16–25 ps. Delay is highly sensitive to process,voltage, and temperature variations, as will be examined in Section 7.2. The FO4 delay is usually quoted assuming typical process parameters and worst-case environment (low power supply voltage and high temperature).


Example 4.11


A ring oscillator is constructed from an odd number of inverters, as shown in Figure


4.24. Estimate the frequency of an N-stage ring oscillator.


SOLUTION: The logical effort of the inverter is g = 1, by deﬁnition. The electrical effort of each inverter is also 1 because it drives a single identical load. The parasitic delay is also 1. The delay of each stage is d = gh + p = 1 × 1 + 1 = 2. An N-stage ring oscillator


FIGURE 4.24  Ring oscillator


4.4      Linear Delay Model 159


has a period of 2N stage delays because a value must propagate twice around the ring to regain the original polarity. Therefore, the period is T = 2 × 2N. The frequency is the reciprocal of the period, 1/4N.


A 31-stage ring oscillator in a 65 nm process has a frequency of 1/(4 × 31 × 3 ps) =


2.7 GHz.


Note that ring oscillators are often used as process monitors to judge if a particular chip is faster or slower than nominally expected. One of the inverters should be replaced with a NAND gate to turn the ring off when not in use. The output can be routed to an external pad, possibly through a test multiplexer. The oscillation frequency should be low enough (e.g., 100 MHz) that the path to the outside world does not attenuate the signal too badly.


4.4.4  Drive


A good standard cell library contains multiple sizes of each common gate. The sizes are typically labeled with their drive. For example, a unit inverter may be called inv_1x. An inverter of eight times unit size is called inv_8x. A 2-input NAND that delivers the same current as the inverter is called nand2_1x.


It is often more intuitive to characterize gates by their drive, x, rather than their input capacitance. If we redeﬁne a unit inverter to have one unit of input capacitance, then the drive of an arbitrary gate is


(4.24)


Delay can be expressed in terms of drive as


(4.25)


4.4.5  Extracting Logical Effort from Datasheets


When using a standard cell library, you can often extract logical effort of gates directly from the datasheets. For example, Figure 4.25 shows the INV and NAND2 datasheets from the Artisan Components library for the TSMC 180 nm process. The gates in the library come in various drive strengths. INVX1 is the unit inverter; INVX2 has twice the drive. INVXL has the same area as the unit inverter but uses smaller transistors to reduce power consumption on noncritical paths. The X12–X20 inverters are built from three stages of smaller inverters to give high drive strength and low input capacitance at the expense of greater parasitic delay.


From the datasheet, we see the unit inverter has an input capacitance of 3.6 fF. The rising and falling delays are speciﬁed separately. We will develop a notation for different delays in Section 9.2.1.5, but will use the average delay for now. The average intrinsic or parasitic delay is (25.3 + 14.6)/2 = 20.0 ps. The slope of the delay vs. load capacitance curve is the average of the rising and falling Kload values. An inverter driving a fanout of h will thus have a delay of


(4.26)


xCg= in


dCxp= +out


pd =


20 0


3 6


4 53 2 37 2


).


psfFgategates


ns pF


ps


( .


. )


20 0 12 4h


160


Figure 4.25  Artisan Components cell library datasheets. Reprinted with permission.


The slope of the delay vs. fanout curve indicates = 12.4 ps and the y-intercept indicates pinv = 20.0 ps, or (20.0/12.4) = 1.61 in normalized terms. This is larger than the delay of 1 estimated earlier, probably because it includes capacitance of internal wires.


By a similar calculation, we ﬁnd the X1 2-input NAND gate has an average delay from the inner (A) input of


(4.27)


Thus, the parasitic delay is (25.4/12.4) = 2.05 and the logical effort is (15.5/12.4) = 1.25.


The logical effort is slighly better than the theoretical 4/3 value, for reasons to be explored in Section 4.4.6.3. The parasitic delay from the outer (B) input is slightly higher, as expected.


The parasitic delay and logical effort of the X2 and X4 gates are similar, conﬁrming our model that logical effort should be independent of gate size for gates of reasonable sizes.


4.4.6 Limitations to the Linear Delay Model


The linear delay model works remarkably well even in advanced technologies; for example,Figure 8.30 shows subpicosecond agreement in a 65 nm process assuming that input and output slopes are matched. Nevertheless, it also has limitations that should be understood when more accuracy is needed.


31 3 19 5 2


4 2


psfFgategates4 53 2 842


25 4 15 5


4.4      Linear Delay Model 161


4.4.6.1 Input and Output Slope  The largest source of error in the linear delay model is the input slope effect. Figure 4.26(a) shows a


fanout-of-4 inverter driven by ramps with different slopes. Recall that


the ON current increases with the gate voltage for an nMOS transistor. We say the transistor is OFF for Vgs < Vt , fully ON for Vgs = VDD,


and partially ON for intermediate gate voltages. As the rise time of


the input increases, the delay also increases because the active transistor is not turned fully ON at once. Figure 4.26(b) plots average


inverter propagation delay vs. input rise time. Notice that the delay vs.


rise time data ﬁts a straight line quite well [Hedenstierna87].


Accounting for slopes is important for accurate timing analysis


(see Section 4.6), but is generally more complex than is worthwhile


for hand calculations. Fortunately, we will see in Section 4.5 that circuits are fastest when each gate has the same effort delay and when


that delay is roughly 4 . Because slopes are related to edge rate, fast


circuits tend to have relatively consistent slopes. If a cell library is


characterized with these slopes, it will tend to be used in the regime


in which it most accurately models delay.


4.4.6.2 Input Arrival Times  Another source of error in the linear delay


model is the assumption that one input of a multiple-input gate


switches while the others are completely stable. When two inputs to a


series stack turn ON simultaneously, the delay will be slightly longer


than predicted because both transistors are only partially ON during


the initial part of the transition. When two inputs to a parallel stack


turn ON simultaneously, the delay will be shorter than predicted


because both transistors deliver current to the output. The delays are


also slightly different depending on which input arrives ﬁrst, as will be


explored in Section 8.5.3.


4.4.6.3 Velocity Saturation  The estimated logical efforts assume


that N transistors in series must be N times as wide to give equal current. However, as discussed in Section 4.3.1, series transistors see less


velocity saturation and hence have lower resistance than we estimated


[Sakurai91].


To make a better estimate, observe that N transistors in series are equivalent to one transistor with N times the channel length. Substituting L and NL into EQ (2.28) shows that the ratio of Idsat for two series transistors to that of a single transistor is


(4.28)


In the limit that the transistors are not at all velocity saturated (Vc >> VDD Vt ), the current ratio reduces to 1/N as predicted. In the limit that the transistors are completely velocity saturated, the current is independent of the number of series transistors.


Example 4.12


Determine the relative saturation current of 2- and 3-transistor nMOS and pMOS stacks in a 65 nm process. VDD = 1.0 V and Vt = 0.3 V. Use Vc = Ec L = 1.04 V for nMOS devices and 2.22 V for pMOS devices.


V NV


dsat series


=(


4x


(b)0


t (ps)


tr = 10 ps


tr = 30 ps


tr = 50 ps


20 16 12 8 4 0


FIGURE 4.26  SPICE simulation of slope effect on  CMOS inverter delay


162


SOLUTION: Applying EQ (4.28) gives a ratio of 0.63 for 2 nMOS transistors, 0.46 for 3 nMOS transistors, 0.57 for 2 pMOS transistors, and 0.40 for 3 pMOS transistors. The pMOS are closer to the ideal result of 0.5 and 0.33 because they experience less velocity saturation.


The transistors are scaled to deliver the same current as an inverter. Three series nMOS transistors must be 1/0.46 = 2.18 times as wide, rather than three times as wide.


Three series pMOS transistors must be 2.5 times as wide. Figure 4.27 modiﬁes Figure


4.22 to reﬂect velocity saturation. The logical efforts of the NAND and NOR are lower than originally predicted, and agree with the results obtained by curve-ﬁtting SPICE simulations in Section 8.5.3.


4.4.6.4 Voltage Dependence  Designers often need to predict how delay will vary if the supply or threshold voltage is changed. Recalling that delay is proportional to CVDD / I and using the -power law model of EQ (2.30) for Idsat , we can estimate the scaling of the RC time constant and of gate delay as


(4.29)


where k reﬂects process parameters.


Alternatively, using the straight line saturation current model from EQ (2.32) for velocity-saturated transistors, we obtain an even simpler estimate:


(4.30)


This model predicts that the supply voltage can be reduced without changing the delay of a velocity-saturated transistor so long as the threshold is reduced in proportion.


When VDD < Vt , delay instead depends on the subthreshold current of EQ (2.45):


(4.31)


4.4.6.5 Gate-Source Capacitance The examples in Section 4.3 assumed that gate capacitance terminates on a ﬁxed supply rail. As discussed in Section 2.3.2, the bottom terminal of the gate oxide capacitor is the channel, which is primarily connected to the source when the transistor is ON. This means that as the source of a transistor changes value, charge is required to change the voltage on Cgs, adding to the delay for series stacks.


4.4.6.6 Bootstrapping  Transistors also have some capacitance from gate to drain. This capacitance couples the input and output in an effect known as bootstrapping, which can be understood by examining Figure 4.28(a). Our models so far have only considered Cin(Cgs). This ﬁgure also considers Cgd, the gate to drain capacitance. In the case that the input is rising (the output starts high), the effective input capacitance is Cgs + Cgd. When the output starts to fall, the voltage across Cgd changes, requiring the input to supply additional current to charge Cgd. In other words, the impact of Cgd on gate capacitance is effectively doubled.


kCV


kC V V


t DD


*


= kCV I


DD V S


2.18


Cin = 4.18 g = 1.40


Cin = 6


g = 2


FIGURE 4.27  Logical effort  estimates accounting for


velocity saturation


4.5      Logical Effort of Paths 163


To illustrate the effect of the bootstrap capacitance on a circuit, Figure


4.28(b) shows two inverter pairs. The top pair has an extra bit of capacitance between the input and output of the second inverter. The bottom pair has the same amount of extra capacitance from input to ground. When x falls, nodes a and c begin to rise (Figure 4.28(c)). At ﬁrst, both nodes see approximately the same capacitance, consisting of the two transistors and the extra 3 fF. As node a rises, it initially bumps up b or “lifts b by its own bootstraps.” Eventually the nMOS transistors turn ON, pulling down b and d. As b falls, it tugs on a through the capacitor, leading to the slow ﬁnal transition visible on node a. Also observe that b falls later than d because of the extra charge that must be supplied to discharge the bootstrap capacitor. In summary, the extra capacitance has a greater effect when connected between input and output as compared to when it is connected between input and ground.


Because Cgd is fairly small, bootstrapping is only a mild annoyance in digital circuits. However, if the inverter is biased in its linear region near VDD /2, the Cgd is multiplied by the large gain of the inverter. This is known as the Miller effect and is of major importance in analog circuits.


4.5 Logical Effort of Paths


Designers often need to choose the fastest circuit topology and gate sizes for a particular logic function and to estimate the delay of the design. As has been stated, simulation or timing analysis are poor tools for this task because they only determine how fast a particular implementation will operate, not whether the implementation can be modiﬁed for better results and if so, what to change. Inexperienced designers often end up in the “simulate and tweak”loop involving minor changes and many fruitless simulations. The method of Logical Effort [Sutherland99] provides a simple method “on the back of an envelope” to choose the best topology and number of stages of logic for a function. Based on the linear delay model, it allows the designer to quickly estimate the best number of stages for a path, the minimum possible delay for the given topology, and the gate sizes that achieve this delay. The techniques of Logical Effort will be revisited throughout this text to understand the delay of many types of circuits.


4.5.1  Delay in Multistage Logic Networks


Figure 4.29 shows the logical and electrical efforts of each stage in a multistage path as a function of the sizes of each stage. The path of interest (the only path in this case) is marked with the dashed blue line. Observe that logical effort is independent of size, while electrical effort depends on sizes. This section develops some metrics for the path as a whole that are independent of sizing decisions.


16/2 32/2


3 fF


FIGURE 4.28  The effect of bootstrapping  on inverter delay and waveform shape


FIGURE 4.29  Multistage logic network


g1 = 1


h1 = x/10


g2 = 5/3 h2 = y/x


g3 = 4/3 h3 = z/y


g4 = 1


h4 = 20/z


164


The path logical effort G can be expressed as the products of the logical efforts of each stage along the path.


(4.32)


The path electrical effort H can be given as the ratio of the output capacitance the path must drive divided by the input capacitance presented by the path. This is more convenient than deﬁning path electrical effort as the product of stage electrical efforts because we do not know the individual stage electrical efforts until gate sizes are selected.


(4.33)


The path effort F is the product of the stage efforts of each stage. Recall that the stage effort of a single stage is  f = gh. Can we by analogy state F = GH for a path?


(4.34)


In paths that branch,


. This is illustrated in Figure 4.30, a circuit with a twoway branch. Consider a path from the primary input to one of the outputs. The path logical effort is G = 1 × 1 = 1. The path electrical effort is H = 90/5 = 18. Thus, GH = 18. But F = f1 f2 = g1 h1 g2h2 = 1 × 6 × 1 × 6 = 36. In other words, F = 2GH in this path on account of the two-way branch.


We must introduce a new kind of effort to account for branching between stages of a path. This branching effort b is the ratio of the total capacitance seen by a stage to the capacitance on the path; in Figure 4.30 it is (15 + 15)/15 = 2.


(4.35)


The path branching effort B is the product of the branching efforts between stages.


(4.36)


Now we can deﬁne the path effort F as the product of the logical, electrical, and branching efforts of the path. Note that the product of the electrical efforts of the stages is actually BH, not just H.


F = GBH


(4.37)


We can now compute the delay of a multistage network. The path delay D is the sum of the delays of each stage. It can also be written as the sum of the path effort delay DF and path parasitic delay P :


(4.38)


The product of the stage efforts is F, independent of gate sizes. The path effort delay is the sum of the stage efforts. The sum of a set of numbers whose product is constant is G


gi


= out(path)


in(path)


f


g h


i i


F GH


onpath offpath


onpath


bi


d D P


15 15


FIGURE 4.30  Circuit with  two-way branch


4.5      Logical Effort of Paths 165


minimized by choosing all the numbers to be equal. In other words, the path delay is minimized when each stage bears the same effort. If a path has N stages and each bears the same effort, that effort must be


(4.39)


Thus, the minimum possible delay of an N-stage path with path effort F and path parasitic delay P is


(4.40)


This is a key result of Logical Effort. It shows that the minimum delay of the path can be estimated knowing only the number of stages, path effort, and parasitic delays without the need to assign transistor sizes. This is superior to simulation, in which delay depends on sizes and you never achieve certainty that the sizes selected are those that offer minimum delay.


It is also straightforward to select gate sizes to achieve this least delay. Combining EQs (4.21) and (4.22) gives us the capacitance transformation formula to ﬁnd the best input capacitance for a gate given the output capacitance it drives.


(4.41)


Starting with the load at the end of the path, work backward applying the capacitance transformation to determine the size of each stage. Check the arithmetic by verifying that the size of the initial stage matches the speciﬁcation.


Example 4.13


Estimate the minimum delay of the path from A to B in Figure 4.31 and choose transistor sizes to achieve this delay. The initial NAND2 gate may present a load of 8  of transistor width on the input and the output load is equivalent to 45  of transistor width.


SOLUTION: The path logical effort is G = (4/3) × (5/3) × (5/3) = 100/


27. The path electrical effort is H = 45/8. The path branching effort is B = 3 × 2 = 6. The path effort is F = GBH = 125. As there are three stages, the best stage effort is


. The path parasitic delay is P = 2 + 3 + 2 = 7. Hence, the minimum path delay is D = 3 × 5 + 7 = 22 in units of , or 4.4 FO4 inverter delays. The gate sizes are computed with the capacitance transformation from EQ (4.41) working backward along the path: y = 45 × (5/3)/5 = 15.


x = (15 + 15) × (5/3)/5 = 10. We verify that the initial 2-input NAND gate has the speciﬁed size of (10 + 10 + 10) × (4/3)/5 = 8.


The transistor sizes in Figure 4.32 are chosen to give the desired amount of input capacitance while achieving equal rise and fall delays. For example, a 2-input NOR gate should have a 4:1 P/N ratio. If the total input capacitance is 15, the pMOS width must be 12 and the nMOS width must be 3 to achieve that ratio.


We can also check that our delay was achieved. The NAND2 gate delay is d1 = g1h1 + p1 = (4/3) × (10 + 10 + 10)/8 + 2 = 7. The NAND3ˆ


/f g h Fi iN= = 1


D NF


1/


ˆ


f̂ =


125 5


x x x


FIGURE 4.31  Example path


P: 4 N: 4


P: 4 N: 6


P: 12


N: 3


FIGURE 4.32  Example path annotated with  transistor sizes


166


gate delay is d2 = g2h2 + p2 = (5/3) × (15 + 15)/10 + 3 = 8. The NOR2 gate delay is d3 =g3h3 + p3 = (5/3) × 45/15 + 2 = 7. Hence, the path delay is 22, as predicted.


Recall that delay is expressed in units of . In a 65 nm process with = 3 ps, the delay is 66 ps. Alternatively, a fanout-of-4 inverter delay is 5 , so the path delay is 4.4 FO4s.


Many inexperienced designers know that wider transistors offer more current and thus try to make circuits faster by using bigger gates. Increasing the size of any of the gates except the ﬁrst one only makes the circuit slower. For example, increasing the size of the NAND3 makes the NAND3 faster but makes the NAND2 slower, resulting in a net speed loss. Increasing the size of the initial NAND2 gate does speed up the circuit under consideration. However, it presents a larger load on the path that computes input A, making that path slower. Hence, it is crucial to have a speciﬁcation of not only the load the path must drive but also the maximum input capacitance the path may present.


4.5.2  Choosing the Best Number of Stages


Given a speciﬁc circuit topology, we now know how to estimate delay and choose gate sizes. However, there are many different topologies that implement a particular logic function. Logical Effort tells us that NANDs are better than NORs and that gates with few inputs are better than gates with many. In this section, we will also use Logical Effort to predict the best number of stages to use.


Logic designers sometimes estimate delay by counting the number of stages of logic, assuming each stage has a constant “gate delay.” This is potentially misleading because it implies that the fastest circuits are those that use the fewest stages of logic.


Of course, the gate delay actually depends on the electrical effort, so sometimes using fewer stages results in more delay. The following example illustrates this point.


Example 4.14


A control unit generates a signal from a unit-sized inverter. The signal must drive unit-sized loads in each bitslice of a 64-bit datapath. The designer can add inverters to buffer the signal to drive the large load. Assuming polarity of the signal does not matter, what is the best number of inverters to add and what delay can be achieved?


SOLUTION: Figure 4.33 shows the cases of adding 0, 1, 2, or 3 inverters. The path electrical effort is H = 64. The path logical effort is G = 1, independent of the number of inverters. Thus, the path effort is F = 64. The inverter sizes are chosen to achieve equal stage effort. The total delay is


The 3-stage design is fastest and far superior to a single stage. If an even number of inversions were required, the two- or four-stage designs are promising. The four-stage design is slightly faster, but the two-stage design requires signiﬁcantly less area and power.


In general, you can always add inverters to the end of a path without changing its function (save possibly for polarity). Let us compute how many should be added for least delay. The logic block shown in Figure 4.34 has n1 stages and a path effort of F. Consider adding N – n1 inverters to the end to bring the path to N stages. The extra inverters do not change the path logical effort but do add


D N


2.8


23


Initial Drivers


Datapath Loads


N:f:D:


1 64 65


2 8 18


3 4 15


15.3


Fastest


FIGURE 4.33  Comparison of different  number of stages of buffers


N – n1 Extra Inverters


Logic Block n1 Stages Path Effort F


FIGURE 4.34  Logic block with additional inverters


4.5      Logical Effort of Paths 167


parasitic delay. The delay of the new path is


(4.42)


Differentiating with respect to N and setting to 0 allows us to solve for the best number of stages, which we will call . The result can be expressed more compactly by deﬁning


to be the best stage effort.


(4.43)


EQ (4.43) has no closed form solution. Neglecting parasitics (i.e., assuming pinv = 0),we ﬁnd the classic result that the stage effort = 2.71828 (e) [Mead80]. In practice, the parasitic delays mean each inverter is somewhat more costly to add. As a result, it is better to use fewer stages, or equivalently a higher stage effort than e. Solving numerically, when pinv = 1, we ﬁnd = 3.59.


A path achieves least delay by using


stages. It is important to understand not only the best stage effort and number of stages but also the sensitivity to using a different number of stages. Figure 4.35 plots the delay increase using a particular number of stages against the total number of stages, for pinv = 1. The x-axis plots the ratio of the actual number of stages to the ideal number. The y-axis plots the ratio of the actual delay to the best achievable. The curve is ﬂat around the optimum. The delay is within 15% of the best achievable if the number of stages is within 2/3 to 3/2 times the theoretical best number (i.e.,  is in the range of 2.4 to 6).


Using a stage effort of 4 is a convenient choice and simpliﬁes mentally choosing the best number of stages. This effort gives delays within 2% of minimum for pinv in the range of 0.7 to 2.5. This further explains why a fanout-of-4 inverter has a “representative” logic gate delay.


p N n p


+ (


N̂


= F N1/ ˆ


ˆ logN F=


1.4


1.6


2.0


1.15


1.26


1.51


(ρ = 6)


(ρ = 2.4)


N/N


FIGURE 4.35  Sensitivity of delay to number of stages


168


4.5.3  Example


Consider a larger example to illustrate the application of Logical Effort. Our esteemed colleague Ben Bitdiddle is designing a decoder for a register ﬁle in the Motoroil 68W86,an embedded processor for automotive applications. The decoder has the following speci-ﬁcations:


16-word register ﬁle


32-bit words


Each register bit presents a load of three unit-sized transistors on the word line (two unit-sized access transistors plus some wire capacitance)


True and complementary versions of the address bits A[3:0] are available


Each address input can drive 10 unit-sized transistors


As we will see further in Section 12.2.2, a 2N-word decoder consists of 2N N-input AND gates. Therefore, the problem is reduced to designing a suitable 4-input AND gate.


Let us help Ben determine how many stages to use, how large each gate should be, and how fast the decoder can operate.


The output load on a word line is 32 bits with three units of capacitance each, or 96 units. Therefore, the path electrical effort is H = 96/10 = 9.6. Each address is used to compute half of the 16 word lines; its complement is used for the other half. Therefore, a B =8-way branch is required somewhere in the path. Now we are faced with a chicken-andegg dilemma. We need to know the path logical effort to calculate the path effort and best number of stages. However, without knowing the best number of stages, we cannot sketch a path and determine the logical effort for that path. There are two ways to resolve the dilemma. One is to sketch a path with a random number of stages, determine the path logical effort, and then use that to compute the path effort and the actual number of stages. The path can be redesigned with this number of stages, reﬁning the path logical effort. If the logical effort changes signiﬁcantly, the process can be repeated. Alternatively,we know that the logic of a decoder is rather simple, so we can ignore the logical effort(assume G = 1). Then we can proceed with our design, remembering that the best number of stages is likely slightly higher than predicted because we neglected logical effort.


Taking the second approach, we estimate the path effort is F = GBH = (1)(8)(9.6) =


76.8. Targeting a best stage effort of = 4, we ﬁnd the best number of stages is N = log4


76.8 = 3.1. Let us select a 3-stage design, recalling that a 4-stage design might be a good choice too when logical effort is considered. Figure 4.36 shows a possible 3-stage design(INV-NAND4-INV).


The path has a logical effort of G = 1 × (6/3) × 1 = 2, so the actual path effort is F =(2)(8)(9.6) = 154. The stage effort is


. This is in the reasonable range of


2.4 to 6, so we expect our design to be acceptable. Applying the capacitance transformation, we ﬁnd gate sizes z = 96 × 1/5.36 = 18 and y = 18 × 2 /5.36 = 6.7. The delay is 3 ×


5.36 + 1 + 4 + 1 =  22.1.


Logical Effort also allows us to rapidly compare alternative designs using a spreadsheet rather than a schematic editor and a large number of simulations. Table 4.4 compares a number of alternative designs. We ﬁnd a 4-stage design is somewhat faster, as we suspected. The 4-stage NAND2-INV-NAND2-INV design not only has the theoretical best number of stages, but also uses simpler 2-input gates to reduce the logical effort and parasitic delay to obtain a 12% speedup over the original design. However, the 3-stage design has a smaller total gate area and dissipates less power.


f =


5 36


1 3


4.5      Logical Effort of Paths 169


4.5.4  Summary and Observations


Logical Effort provides an easy way to compare and select circuit topologies, choose the best number of stages for a path, and estimate path delay. The notation takes some time to become natural, but this author has poured through all the letters in the English and Greek alphabets without ﬁnding better notation. It may help to remember d for “delay,” p for “parasitic,” b for “branching,” f for “effort,” g for “logical effort” (or perhaps gain), and h as the next letter after “f ” and “g.” The notation is summarized in Table 4.5 for both stages and paths.


The method of Logical Effort is applied with the following steps:


1. Compute the path effort:  F = GBH


2. Estimate the best number of stages:


3. Sketch a path using:  stages


4. Estimate the minimum delay:


5. Determine the best stage effort:


6. Starting at the end, work backward to ﬁnd sizes:


= ( ) =


CL


Ip


In Ic


FIGURE 5.4


CMOS inverter


0 0.2 0.4 0.6 0.8 1


0.5 1


(mA)


Linear ShortCircuit Current


Pp = Ip(VDD  Vout)


Pn = InVout


Ic = Ip  In


Pc = IcVout


(mW)


0.2 0.4 0.6 t(ns)


0.8 1


(fJ)


0 75 150


Vout = lcdt1C


EC = Pc dt


Evdd = Pvdd dt


Pvdd = IpVDD


FIGURE 5.5  Inverter switching voltage, current, power, and energy


Chapter 5      Power


184


one would expect charging a capacitor through a linear resistor. When Vin rises, the pMOS starts to turn OFF. However, there is a small blip of current while the partially ON pMOS ﬁghts against the nMOS. This is called short-circuit current. The inverter draws power from VDD as Vout rises. Half of the power is dissipated in the pMOS transistor and the other half is delivered to the capacitor. VDD supplies a total of 150 fJ of energy, of which half is stored on the capacitor. The inverter is sized for equal rise/fall times so the falling transition is symmetric. The energy on the capacitor is dumped to GND. The short-circuit current consumes an almost imperceptibly small 2.7 fJ of additional energy from VDD during this transition.


Suppose that the gate switches at some average frequency fsw. Over some interval T,the load will be charged and discharged Tfsw times. Then, according to EQ (5.3), the average power dissipation is


(5.9)


This is called the dynamic power because it arises from the switching of the load. Because most gates do not switch every clock cycle, it is often more convenient to express switching frequency fsw as an activity factor  times the clock frequency f. Now, the dynamic power dissipation may be rewritten as


(5.10)


The activity factor is the probability that the circuit node transitions from 0 to 1, because that is the only time the circuit consumes power. A clock has an activity factor of = 1 because it rises and falls every cycle. Most data has a maximum activity factor of 0.5 because it transitions only once each cycle. Truly random data has an activity factor of 0.25 because it transitions every other cycle. Static CMOS logic has been empirically determined to have activity factors closer to 0.1 because some gates maintain one output state more often than another and because real data inputs to some portions of a system often remain constant from one cycle to the next.


5.1.3  Sources of Power Dissipation


Power dissipation in CMOS circuits comes from two components:


Dynamic dissipation due to


○ charging and discharging load capacitances as gates switch


○  “short-circuit” current while both pMOS and nMOS stacks are partially ON  Static dissipation due to


○ subthreshold leakage through OFF transistors


○ gate leakage through gate dielectric


○ junction leakage from source/drain diffusions


○ contention current in ratioed circuits (see Section 9.2.2)


Putting this together gives the total power of a circuit


(5.11)


E T


Tf CV T


CV f


switching


sw


dynamic switching short circuit


5.2      Dynamic Power 185


(5.12)


(5.13)


Power can also be considered in active, standby, and sleep modes. Active power is the power consumed while the chip is doing useful work. It is usually dominated by Pswitching.


Standby power is the power consumed while the chip is idle. If clocks are stopped and ratioed circuits are disabled, the standby power is set by leakage. In sleep mode, the supplies to unneeded circuits are turned off to eliminate leakage. This drastically reduces the sleep power required, but the chip requires time and energy to wake up so sleeping is only viable if the chip will idle for long enough.


[Gonzalez96] found that roughly one-third of microprocessor power is spent on the clock, another third on memories, and the remaining third on logic and wires. In nanometer technologies, nearly one-third of the power is leakage. High-speed I/O contributes a growing component too. For example, Figure 5.6 shows the active power consumption of Sun’s 8-core 84 W Niagra2 processor [Nawathe08]. The cores and other components collectively account for clock, logic, and wires.


The next sections investigate how to estimate and minimize each of these components of power. Many tools are available to assist with power estimation; these are discussed further in Sections 8.5.4 and 14.4.1.6.


5.2 Dynamic Power


Dynamic power consists mostly of the switching power, given in EQ (5.10). The supply voltage VDD and frequency f are readily known by the designer. To estimate this power, one can consider each node of the circuit. The capacitance of the node is the sum of the gate,diffusion, and wire capacitances on the node. The activity factor can be estimated using techniques described in Section 5.2.1 or measured from logic simulations. The effective capacitance of the node is its true capacitance multiplied by the activity factor. The switching power depends on the sum of the effective capacitances of all the nodes.


Activity factors can be heavily dependent on the particular task being executed. For example, a processor in a cell phone will use more power while running video games than while displaying a calendar. CAD tools do a ﬁne job of power estimation when given a realistic workload. Low power design involves considering and reducing each of the terms in switching power.


As VDD is a quadratic term, it is good to select the minimum VDD that can support the required frequency of operation. Likewise, we choose the lowest frequency of operation that achieves the desired end performance. The activity factor is mainly reduced by putting unused blocks to sleep. Finally, the circuit may be optimized to reduce the overall load capacitance of each section.


Example 5.1


A digital system-on-chip in a 1 V 65 nm process (with 50 nm drawn channel lengths and  = 25 nm) has 1 billion transistors, of which 50 million are in logic gates and the remainder in memory arrays. The average logic transistor width is 12  and the average memory transistor width is 4 . The memory arrays are divided into banks and only the


static sub gate junct contention


= + + +( )


total dynamic static


Cores 32%


Memory 20%


I/O 13%


Leakage 21%


Other


14%


FIGURE 5.6  Power in Niagra2


186


necessary bank is activated so the memory activity factor is 0.02. The static CMOS logic gates have an average activity factor of 0.1. Assume each transistor contributes 1 fF/ m of gate capacitance and 0.8 fF/ m of diffusion capacitance. Neglect wire capacitance for now (though it could account for a large fraction of total power). Estimate the switching power when operating at 1 GHz.


SOLUTION: There are (50  106 logic transistors)(12 )(0.025 m/ )((1 + 0.8) fF/ m) =27 nF of logic transistors and (950  106 memory transistors)(4 )(0.025 m/ )((1 +


0.8) fF/ m) = 171 nF of memory transistors. The switching power consumption is[(0.1)(27  10–9) + (0.02)(171  10–9)](1.0 V)2(109 Hz) = 6.1 W.


Dynamic power also includes a short-circuit power component caused by power rushing from VDD to GND when both the pullup and pulldown networks are partially ON while a transistor switches. This is normally less than 10% of the whole, so it can be conservatively estimated by adding 10% to the switching power.


Switching power is consumed by delivering energy to charge a load capacitance, then dumping this energy to GND. Intuitively, one might expect that power could be saved by shufﬂing the energy around to where it is needed rather than just dumping it. Resonant circuits, and adiabatic charge-recovering circuits [Maksimovic00, Sathe07] seek to achieve such a goal. Unfortunately, all of these techniques add complexity that detracts from the potential energy savings, and none have found more than niche applications.


5.2.1  Activity Factor


The activity factor is a powerful and easy-to-use lever for reducing power. If a circuit can be turned off entirely, the activity factor and dynamic power go to zero. Blocks are typically turned off by stopping the clock; this is called clock gating. When a block is on, the activity factor is 1 for clocks and substantially lower for nodes in logic circuits. The activity factor of a logic gate can be estimated by calculating the switching probability. Glitches can increase the activity factor.


5.2.1.1 Clock Gating  Clock gating ANDs a clock signal with an enable to turn off the clock to idle blocks. It is highly effective because the clock has such a high activity factor,and because gating the clock to the input registers of a block prevents the registers from switching and thus stops all the activity in the downstream combinational logic.


Clock gating can be employed on any enabled register. Section 10.3.5 discusses enabled register design. Sometimes the logic to compute the enable signal is easy; for example, a ﬂoating-point unit can be turned off when no ﬂoating-point instructions are being issued. Often, however, clock gating signals are some of the most critical paths of the chip.


The clock enable must be stable while the clock is active (i.e., 1 for systems using positive edge-triggered ﬂip-ﬂops). Figure 5.7 shows how an enable latch can be used to ensure the enable does not change before the clock falls.


When a large block of logic is turned off, the clock can be gated early in the clock distribution network, turning off not only the registers but also a portion of the global network. The clock network has an activity factor of 1 and a high capacitance, so this saves signiﬁcant power.


clk


Enable Logic


Enable Latch


Clock


Gater


Registers


FIGURE 5.7  Clock gating


5.2      Dynamic Power 187


5.2.1.2 Switching Probability  Recall that the activity factor of a node is the probability


that it switches from 0 to 1. This probability depends on the logic function. By analyzing


the probability that each node is 1, we can estimate the activity factors. Although designers don’t manually estimate activity factors very often, the exercise is worth doing here to


gain some intuition about switching activity.


Deﬁne Pi to be the probability that node i is 1. Pi = 1 – Pi is the probability that node


i is 0. i , the activity factor of node i, is the probability that the node is 0 on one cycle and


1 on the next. If the probability is uncorrelated from cycle to cycle,


(5.14)


Completely random data has P = 0.5 and thus = 0.25. Structured data may have different probabilities. For example, the upper bits of a 64-bit unsigned integer representing a physical quantity such as the intensity of a sound or the amount of money in your bank account are 0 most of the time. The activity factor is lower than 0.25 for such data.


Table 5.1 lists the output probabilities of various gates as a function of their input probabilities, assuming the inputs are uncorrelated. According to EQ (5.14), the activity factor of the output is PYPY.


Example 5.2


Figure 5.8 shows a 4-input AND gate built using a tree (a) and a chain (b) of gates.


Determine the activity factors at each node in the circuit assuming the input probabilities PA = PB = PC = PD = 0.5.


SOLUTION: Figure 5.9 labels the signal probabilities and the activity factors at each node based on Table 5.1 and EQ (5.14). The chain has a lower activity factor at the intermediate nodes.


TABLE 5.1  Switching probabilities


PY


AND2


PAPB


AND3


PAPBPC


OR2


1 – PAPB


NAND2


NOR2


XOR2


PAPB + PAPB


i iP P


P =   =


n4


n5


n6


n7


Z


P =  =


FIGURE 5.8  4-input AND circuits


188


When paths contain reconvergent fanouts, signals become correlated and conditional probabilities become required. Power analysis tools are the most convenient way to handle large complex circuits.


Preliminary power estimation requires guessing an activity factor before RTL code is written and workloads are known. = 0.1 is a reasonable choice in the absence of better data.


5.2.1.3 Glitches  The switching probabilities computed in the previous section are only valid if the gates have zero propagation delay. In reality, gates sometimes make spurious transitions called glitches when inputs do not arrive simultaneously. For example, in Figure 5.8(b), suppose ABCD changes from 1101 to 0111. Node n4 was 1 and falls to 0.


However, nodes n5, n6, n7, and Z may glitch before n4 changes, as shown in Figure 5.10.


The glitches cause extra power dissipation. Chains of gates are particularly prone to this problem. Glitching can raise the activity factor of a gate above 1 and can account for the majority of power in certain circuits such as ripple carry adders and array multipliers (see Chapter 11). Glitching power can be accurately assessed through simulations accounting for timing.


5.2.2  Capacitance


Switching capacitance comes from the wires and transistors in a circuit. Wire capacitance is minimized through good ﬂoorplanning and placement (the locality aspect of structured design). Units that exchange a large amount of data should be placed close to each other to reduce wire lengths.


Device-switching capacitance is reduced by choosing fewer stages of logic and smaller transistors. Minimum-sized gates can be used on non-critical paths. Although Logical Effort ﬁnds that the best stage effort is about 4, using a larger stage effort increases delay only slightly and greatly reduces transistor sizes. Therefore, gates that are large or have a high activity factor and thus dominate the power can be downsized with only a small performance impact. For example, buffers driving I/O pads or long wires may use a stage effort of 8–12 to reduce the buffer size. Similarly, registers should use small clocked transistors because their activity factor is an order of magnitude greater than transistors in combinational logic. In Chapter 6, we will see that wire capacitance dominates many circuits. The most energy-efﬁcient way to drive long wires is with inverters or buffers rather than with more complex gates that have higher logical efforts [Stan99].


Figure 5.11 shows an example of transistor sizing in a 64-bit Kogge-Stone adder (see Section 11.2.2.8) [Markovic 04]. In Figure 5.11(a), the gates are sized to achieve minimum possible delay. The high spikes in the middle correspond to large gates driving the long wires. In Figure 5.11(b), the circuit is reoptimized for 10% greater delay. The energy is reduced by 55%. In general, large energy savings can be made by relaxing a circuit a small amount from the minimum delay point.


Unfortunately, there are no closed-form methods to determine gate sizes that minimize energy under a delay constraint, even for circuits as simple as an inverter chain


P = 3/4 α = 3/16 P = 3/4


α = 3/16


P = 1/16


α = 15/256


P = 3/4


α = 3/16 P = 1/4α = 3/16P = 7/8α = 7/64 P = 1/8α = 7/64


P = 15/16


α = 15/256 P = 1/16α = 15/256


FIGURE 5.9  Signal probabilities and activity factors


n3 n4


n7 D


Glitches


FIGURE 5.10


Glitching in a chain of gates


FIGURE 5.11 Adder gate sizing  under a delay constraint


(Adapted from [Markovic 04].


© IEEE 2004.)


5.2      Dynamic Power 189


[Ma94]. However, it is straightforward to solve the problem numerically, as will be formulated in the next section.


5.2.2.1 Gate Sizing Under a Delay Constraint  In Chapter 4, Logical Effort showed us how to minimize delay. In many cases, we are willing to increase delay to save energy. We can extend the iterative technique from Section 4.5.6 to size a circuit for minimum switching energy under a delay constraint.


First, consider a model to compute the energy of a circuit. If a unit inverter has gate capacitance 3C, then a gate with logical effort g, parasitic delay p, and drive x has gx times as much gate capacitance and px times as much diffusion capacitance. The switching energy of each gate depends on its activity factor, the diffusion capacitance of the gate, the wire capacitance Cwire, and the gate capacitance of all the stages it drives. The energy of the entire circuit is the sum of the energies of each gate.


(5.15)


If wire capacitance is expressed in multiples of the capacitance of a unit inverter as c = Cwire /3C and we normalize energy for the capacitance and voltage of the process,EQ (5.15) becomes the sum of the effective capacitances of the nodes.


(5.16)


Now, we seek to minimize E such that the worst-case arrival time is less than some delay D. The problem is still a posynomial and has a unique solution that can be found quickly by a good optimizer.


Example 5.3


Generate an energy-delay trade-off curve for the circuit from Figure 4.37 as delay varies from the minimum possible (Dmin = 23.44 ) to 50 . Assume that the input probabilities are 0.5.


SOLUTION: Figure 5.12 shows the activity factors of each node. Hence, the energy of this circuit is


(5.17)


Energy


fanout


+ +


Cp x


g x


j j


i nodes


c p x


nodes


x di i


= + +( ) + +( ) + +( )+


1 4


3 2


3 16


3 4


7 1024


87 1024


10 3


) + +( )


x x


x2


x3


x4


x5


p1 = 1/2 α1 = 1/4


p1 = 3/4


α1 = 3/16


p4 = 3/32


c4 = 10


c5 = 12


α4 = 87/1024


p3 = 1/4α3 = 3/16


p5 = 29/32


α5 = 87/1024


FIGURE 5.12  Activity factors


Figure 5.13 shows the energy-delay trade-off curve obtained by repeatedly solving for minimum energy under a delay constraint. The curve is steep near Dmin, indicating that a large amount of energy can be saved for a small increase in delay. The delay cannot be reduced below Dmin for any amount of energy unless the size of the input inverter is increased (which would increase the delay of the previous circuit).


5.2.3  Voltage


Voltage has a quadratic effect on dynamic power. Therefore, choosing a lower power supply signiﬁcantly reduces power consumption. As many transistors are operating in a velocity-saturated regime, the lower power supply may not reduce performance as much as long-channel models predict. The chip may be divided into multiple voltage domains,where each domain is optimized for the needs of certain circuits. For example, a systemon-chip might use a high supply voltage for memories to ensure cell stability, a medium voltage for a processor, and a low voltage for I/O peripherals running at lower speeds. In Section 5.3.2, we will examine how voltage domains can be turned off entirely to save leakage power during sleep mode.


Voltage also can be adjusted based on operating mode; for example, a laptop processor may operate at high voltage and high speed when plugged into an AC adapter, but at lower voltage and speed when on battery power. If the frequency and voltage scale down in proportion, a cubic reduction in power is achieved. For example, the laptop processor may scale back to 2/3 frequency and voltage to save 70% in power when unplugged.


5.2.3.1 Voltage Domains  Some of the challenges in using voltage domains include converting voltage levels for signals that cross domains, selecting which circuits belong in which domain, and routing power supplies to multiple domains.


Figure 5.14 shows direct connection of inverters in two domains using high and low supplies, VDDH and VDDL, respectively. A gate in the VDDH domain can directly drive a gate in the VDDL domain. However, the gate in the VDDL domain will switch faster than it would if driven by another VDDL gate. The timing analyzer must consider this when computing the contamination delay, lest a hold time be violated. Unfortunately, the gate in the VDDL domain cannot directly drive a gate in the VDDH domain. When n2 is at VDDL,the pMOS transistor in the VDDH domain has Vgs = VDDH – VDDL. If this exceeds Vt, the pMOS will turn ON and burn contention current. Even if the difference is less than Vt ,the pMOS will suffer substantially increased leakage. This problem may be alleviated by using a high-Vt pMOS device in the receiver if the voltage difference between domains is small enough [Tawﬁk09].


FIGURE 4.37  Example path


4.6      Timing Analysis Delay Models 173


The stage efforts, f, are equal for each gate in paths with no ﬁxed capacitive loads, but may change after a load.


To minimize delay, upsize gates on nodes with large ﬁxed capacitances to reduce  the effort borne by the gate, while only slightly increasing the effort borne by the  predecessor.


A standard cell library offers a discrete set of sizes. Gate drives must be rounded to the nearest available size. For example, the circuit might use inv_1x, nand2_2x, nor2_2x,nor3_3x, and inv_6x. The delay increases to 23.83, less than a 2% penalty. In general,libraries with a granularity of  between successive drives are nearly as good as those with continuous sizes, so long as large inverters are available to drive big loads. Even using a granularity of 2 between drives (1x, 2x, 4x, 8x) is sufﬁcient to obtain good results.


Although this section used a linear delay model to build on the insights of Logical Effort, it is also possible to use more elaborate models taking into account sensitivity to edge rate, VDD, and Vt [Patil07]; the extra complexity is not a problem for a numerical solver and the model allows for optimizing supply and threshold voltages as well as sizes.


Timing models are discussed further in Section 4.6.


4.6 Timing Analysis Delay Models


To handle a chip with millions of gates, the delay model for a timing analyzer must be easy enough to compute that timing analysis is fast, yet accurate enough to give conﬁdence. This section reviews several delay models for timing analysis that are much faster than SPICE simulations, yet more accurate than the simple linear delay model. Timing (and area, power,and noise) models for each gate in a standard cell library are stored in a .lib ﬁle. These models are part of the Liberty standard documented at www.opensourceliberty.org. Logical effort parameters for standard cells can be obtained by ﬁtting a straight line to the timing models, assuming equal delays and rise/fall times for the previous stage.


4.6.1  Slope-Based Linear Model


A simple approach is to extend the linear delay model by adding a term reﬂecting the input slope. Assuming the slope of the input is proportional to the delay of the previous stage, the delays for rising and falling outputs can be expressed as:


delay_rise =intrinsic_rise + rise_resistance × capacitance +slope_rise × delay_previous


delay_fall =intrinsic_fall + fall_resistance × capacitance +slope_fall × delay_previous


TABLE 4.6  Path design for minimum delays


Stage (i )


xi


fi


cin


di


ai


1: INV


4.85


5.85


2: NAND2


1.62


2.16


6.85


12.70


3: NOR2


2.70


4: NOR3


3.37


7.86


7.85


20.55


5: INV


6.35


1.89


2.89


23.44


174


Linear delay models are not accurate enough to handle the wide range of slopes and loads found in synthesized circuits, so they have largely been superseded by nonlinear delay models.


4.6.2  Nonlinear Delay Model


A nonlinear delay model looks up the delay from a table based on the load capacitance and the input slope. Separate tables are used to lookup rising and falling delays and output slopes. Table 4.7 shows an example of a nonlinear delay model for the falling delay of an inverter. The timing analyzer uses interpolation when a speciﬁc load capacitance or slope is not in the table.


Nonlinear delay models are widely used at the time of this writing. However, they do not contain enough information to characterize the delay of a gate driving a complex RC interconnect network with the accuracy desired by some users. They also lack the accuracy to fully characterize noise events. A different model must be created for each voltage and temperature at which the chip might be characterized.


4.6.3  Current Source Model


The limitations of nonlinear delay models have motivated the development of current source models. A current source model theoretically should express the output DC current as a nonlinear function of the input and output voltages of the cell. A timing analyzer numerically integrates the output current to ﬁnd the voltage as a function of time into an arbitrary RC network and to solve for the propagation delay.


The Liberty Composite Current Source Model (CCSM) instead stores output current as a function of time for a given input slew rate and output capacitance. The competing Effective Current Source Model (ECSM) stores output voltage as a function of time. The two representations are equivalent, and can be synthesized into a true current source model [Chopra06].


4.7 Pitfalls and Fallacies


Defining gate delay for an unloaded gate


When marketing a process, it is common to report gate delay based on an inverter in a ring  oscillator (2 ), or even the RC time constant of a transistor charging its own gate capacitance (1/3 ). Remember that the delay of a real gate on the critical path should be closer to 5–6 .


TABLE 4.7  Nonlinear Delay Model for inverter tpdf (ps)


Rise Time (ps)


Cout (fF)


11.5


13.3


17.0


21.2


25.3


18.4


20.2


24.1


30.9


38.5


32.0


33.8


37.6


43.4


58.5


59.2


60.9


65.7


72.3


87.8


4.8      Historical Perspective 175


When in doubt, ask how “gate delay” is defined or ask for the FO4 inverter delay.


Trying to increase speed by increasing the size of transistors in a path


Most designers know that increasing the size of a transistor decreases its resistance and thus  makes it faster at driving a constant load. Novice designers sometimes forget that increasing  the size increases input capacitance and makes the previous stage slower, especially when  that previous stage belongs to somebody else’s timing budget. The authors have seen this lead  to lack of convergence in full-chip timing analysis on a large microprocessor because individual engineers boost the size of their own gates until their path meets timing. Only after the  weekly full-chip timing roll-up do they discover that their inputs now arrive later because of  the greater load on the previous stage. The solution is to include in the specification of each  block not only the arrival time but also the resistance of the driver in the previous block.


Trying to increase speed by using as few stages of logic as possible


Logic designers often count “gate delays” in a path. This is a convenient simplification when  used properly. In the hands of an inexperienced engineer who believes each gate contributes  a gate delay, it suggests that the delay of a path is minimized by using as few stages of logic as  possible, which is clearly untrue.


4.8 Historical Perspective


Figure 1.5 illustrated the exponential increase in microprocessor frequencies over nearly four decades. While much of the improvement comes from the natural improvements in gate delay with feature size, a signiﬁcant portion is due to better microarchitecture and circuit design with fewer gate delays per cycle. From a circuit perspective, the cycle time is best expressed in FO4 inverter delays.


Figure 4.38 illustrates the historical trends in microprocessor cycle time based on chips reported at the International Solid-State Circuits Conference. Early processors operated at close to 100 FO4 delays per cycle. The Alpha line of microprocessors from Digital Equipment Corporation shocked the staid world of circuit design in the early 1990s by proving that cycle times below 20 FO4 delays were possible. This kicked off a race for higher clock frequencies. By the late 1990s, Intel and AMD marketed processors primarily on frequency. The Pentium II and III reached about 20–24 FO4 delays/cycle.


The Pentium 4 drove cycle times down to about 10 FO4 at the expense of a very long


0 10 20 30 40 50 60 70 80


1994 1996 1998 2000 2002 2004 2006 2008


x86


PA-RISC


Power/PowerPC Sparc


Alpha


FIGURE 4.38  Microprocessor cylcle time trends. Data has some uncertainty based on estimating FO4  delay as a function of feature size.


176


pipeline and enormous power consumption. Microarchitects predicted that performance would be maximized at a cycle time of only 8 FO4 delays/cycle [Hrishikesh02].


The short cycle times came at the expense of vast numbers (20–30) of pipeline stages and enormous power consumption (nearly 100 W). As will be seen in the next chapter,power became as important as performance speciﬁcations. The number of gates per cycle rebounded to a more power-efﬁcient point. [Srinivasan02] observed that 19–24 FO4 delays per cycle provides a better trade-off between performance and power.


Application-speciﬁc integrated circuits have generally operated at much lower frequencies (e.g., 200–400 MHz in nanometer processes) so that they can be designed more easily. Typical ASIC cycle times are 40–100 FO4 delays per cycle [Mai05, Chinnery02],although performance-critical designs sometimes are as fast as 25 FO4s.


The VLSI designer’s challenge is to engineer a system that meets speed requirements while consuming little power or area, operating reliably, and taking little time to design.


Circuit simulation is an important tool for calculating delay and will be discussed in depth in Chapter 5, but it takes too long to simulate every possible design; is prone to garbagein, garbage-out mistakes; and doesn’t give insight into why a circuit has a particular delay or how the circuit should be changed to improve delay. The designer must also have simple models to quickly estimate performance by hand and explain why some circuits are better than others.


Although transistors are complicated devices with nonlinear current-voltage and capacitance-voltage relationships, for the purpose of delay estimation in digital circuits,they can be approximated quite well as having constant capacitance and an effective resistance R when ON. Logic gates are thus modeled as RC networks. The Elmore delay model estimates the delay of the network as the sum of each capacitance times the resistance through which it must be charged or discharged. Therefore, the gate delay consists of a parasitic delay (accounting for the gate driving its own internal parasitic capacitance)plus an effort delay (accounting for the gate driving an external load). The effort delay depends on the electrical effort (the ratio of load capacitance to input capacitance, also called fanout) and the logical effort (which characterizes the current driving capability of the gate relative to an inverter with equal input capacitance). Even in advanced fabrication processes, the delay vs. electrical effort curve ﬁts a straight line very well. The method of Logical Effort builds on this linear delay model to help us quickly estimate the delay of entire paths based on the effort and parasitic delay of the path. We will use Logical Effort in subsequent chapters to explain what makes circuits fast.


4.1 Sketch a 2-input NOR gate with transistor widths chosen to achieve effective rise  and fall resistances equal to a unit inverter. Compute the rising and falling propagation delays of the NOR gate driving h identical NOR gates using the Elmore delay  model. Assume that every source or drain has fully contacted diffusion when making  your estimate of capacitance.


4.2 Sketch a stick diagram for the 2-input NOR. Repeat Exercise 4.1 with better capacitance estimates. In particular, if a diffusion node is shared between two parallel


Exercises 177


transistors, only budget its capacitance once. If a diffusion node is between two


series transistors and requires no contacts, only budget half the capacitance because  of the smaller diffusion area.


4.3 Find the rising and falling propagation delays of an unloaded AND-OR-INVERT  gate using the Elmore delay model. Estimate the diffusion capacitance based on a  stick diagram of the layout.


4.4 Find the worst-case Elmore parasitic delay of an n-input NOR gate.


4.5 Sketch a delay vs. electrical effort graph like that of Figure 4.21 for a 2-input NOR  gate using the logical effort and parasitic delay estimated in Section 4.4.2. How does  the slope of your graph compare to that of a 2-input NAND? How does the  y-intercept compare?


4.6 Let a 4x inverter have transistors four times as wide as those of a unit inverter. If a  unit inverter has three units of input capacitance and parasitic delay of pinv, what is  the input capacitance of a 4x inverter? What is the logical effort? What is the parasitic delay?


4.7 A 3-stage logic path is designed so that the effort borne by each stage is 12, 6, and 9  delay units, respectively. Can this design be improved? Why? What is the best number of stages for this path? What changes do you recommend to the existing design?


4.8 Suppose a unit inverter with three units of input capacitance has unit drive.


a) What is the drive of a 4x inverter?


b) What is the drive of a 2-input NAND gate with three units of input capacitance?


4.9 Sketch a 4-input NAND gate with transistor widths chosen to achieve equal rise


and fall resistance as a unit inverter. Show why the logical effort is 6/3.


4.10 Consider the two designs of a 2-input AND gate shown in Figure 4.39. Give an


intuitive argument about which will be faster. Back up your argument with a calculation of the path effort, delay, and input capacitances x and y to achieve this delay.


4.11 Consider four designs of a 6-input AND gate shown in Figure 4.40. Develop an


expression for the delay of each path if the path electrical effort is H. What design is  fastest for H = 1? For H = 5? For H = 20? Explain your conclusions intuitively.


FIGURE 4.39  2-input AND gate


FIGURE 4.40  6-input AND gate


178


4.12 Repeat the decoder design example from Section 4.5.3 for a 32-word register ﬁle


with 64-bit registers. Determine the fastest decoder design and estimate the delay of  the decoder and the transistor widths to achieve this delay.


4.13 Design a circuit at the gate level to compute the following function:


if (a == b) y = a;else y = 0;


Let a, b, and y be 16-bit busses. Assume the input and output capacitances are each  10 units. Your goal is to make the circuit as fast as possible. Estimate the delay in


FO4 inverter delays using Logical Effort if the best gate sizes were used. What sizes  do you need to use to achieve this delay?


4.14 Plot the average delay from input A of an FO3 NAND2 gate from the datasheet in  Figure 4.25. Why is the delay larger for the XL drive strength than for the other


drive strengths?


4.15 Figure 4.41 shows a datasheet for a 2-input NOR gate in the Artisan Components  standard cell library for the TSMC 180 nm process. Find the average parasitic delay  and logical effort of the X1 NOR gate A input. Use the value of  from Section 4.4.5.


FIGURE 4.41  2-input NOR datasheet (Courtesy of Artisan  Components.)


Exercises 179


4.16 Find the parasitic delay and logical effort of the X2 and X4 NOR gate A input using  Figure 4.41. By what percentage do they differ from that of the X1 gate? What does  this imply about our model that parasitic delay and logical effort depend only on


gate type and not on transistor sizes?


4.17 What are the parasitic delay and logical effort of the X1 NOR gate B input in Figure 4.41? How and why do they differ from the A input?


4.18 Parasitic delay estimates in Section 4.4.2 are made assuming contacted diffusion on  each transistor on the output node and ignoring internal diffusion. Would parasitic  delay increase or decrease if you took into account that some parallel transistors on  the output node share a single diffusion contact? If you counted internal diffusion  capacitance between series transistors? If you counted wire capacitance within the  cell?


4.19 Consider a process in which pMOS transistors have three times the effective resistance as nMOS transistors. A unit inverter with equal rising and falling delays in


this process is shown in Figure 4.42. Calculate the logical efforts of a 2-input


NAND gate and a 2-input NOR gate if they are designed with equal rising and falling delays.


4.20 Generalize Exercise 4.19 if the pMOS transistors have  times the effective resistance of nMOS transistors. Find a general expression for the logical efforts of a kinput NAND gate and a k-input NOR gate. As increases, comment on the relative  desirability of NANDs vs. NORs.


4.21 Some designers deﬁne a “gate delay” to be a fanout-of-3 2-input NAND gate rather  than a fanout-of-4 inverter. Using Logical Effort, estimate the delay of a fanout-of3 2-input NAND gate. Express your result both in  and in FO4 inverter delays,


assuming pinv = 1.


4.22 Repeat Exercise 4.21 in a process with a lower ratio of diffusion to gate capacitance  in which pinv = 0.75. By what percentage does this change the NAND gate delay, as  measured in FO4 inverter delays? What if pinv = 1.25?


4.23 The 64-bit Naffziger adder [Naffziger96] has a delay of 930 ps in a fast 0.5- m


Hewlett-Packard process with an FO4 inverter delay of about 140 ps. Estimate its  delay in a 65 nm process with an FO4 inverter delay of 20 ps.


4.24 An output pad contains a chain of successively larger inverters to drive the (relatively) enormous off-chip capacitance. If the ﬁrst inverter in the chain has an input  capacitance of 20 fF and the off-chip load is 10 pF, how many inverters should be  used to drive the load with least delay? Estimate this delay, expressed in FO4


inverter delays.


TABLE 4.4  Spreadsheet comparing decoder designs Design


Stages N


NAND4-INV


29.8


NAND2-NOR2


20/9


30.1


INV-NAND4-INV


22.1


NAND4-INV-INV-INV


21.1


NAND2-NOR2-INV-INV


20.5


NAND2-INV-NAND2-INV


16/9


19.7


INV-NAND2-INV-NAND2-INV


20.4


NAND2-INV-NAND2-INV-INV-INV


21.6


A[3] A[3] A[2] A[2] A[1] A[1] A[0] A[0]


word[0]


word[15]


96 Units of Wordline Capacitance


10 10


FIGURE 4.36  3-stage decoder design


ˆ logN F= 4


ˆ / ˆ1


/ ˆ f F N= 1


170


CAD tools are very fast and accurate at evaluating complex delay models, so Logical Effort should not be used as a replacement for such tools. Rather, its value arises from“quick and dirty” hand calculations and from the insights it lends to circuit design. Some of the key insights include:


The idea of a numeric “logical effort” that characterizes the complexity of a logic  gate or path allows you to compare alternative circuit topologies and show that


some topologies are better than others.


NAND structures are faster than NOR structures in static CMOS circuits.


Paths are fastest when the effort delays of each stage are about the same and when  these delays are close to four.


Path delay is insensitive to modest deviations from the optimum. Stage efforts of


2.4–6 give designs within 15% of minimum delay. There is no need to make calculations to more than 1–2 signiﬁcant ﬁgures, so many estimations can be made in  your head. There is no need to choose transistor sizes exactly according to theory  and there is little beneﬁt in tweaking transistor sizes if the design is reasonable.


Using stage efforts somewhat greater than 4 reduces area and power consumption  at a slight cost in speed. Using efforts greater than 6–8 comes at a signiﬁcant cost  in speed.


Using fewer stages for “less gate delays” does not make a circuit faster. Making


gates larger also does not make a circuit faster; it only increases the area and power  consumption.


The delay of a well-designed path is about log4 F fanout-of-4 (FO4) inverter


delays. Each quadrupling of the load adds about one FO4 inverter delay to the


path. Control signals fanning out to a 64-bit datapath therefore incur an ampliﬁcation delay of about three FO4 inverters.


TABLE 4.5  Summary of Logical Effort notation Term


Stage Expression


Path Expression


number of stages


logical effort


g (see Table 4.2)


electrical effort


branching effort


effort


effort delay


parasitic delay


p (see Table 4.3)


delay


pi


d D Pi F


4.5      Logical Effort of Paths 171


The logical effort of each input of a gate increases through no fault of its own as


the number of inputs grows. Considering both logical effort and parasitic delay, we


ﬁnd a practical limit of about four series transistors in logic gates and about four


inputs to multiplexers. Beyond this fan-in, it is faster to split gates into multiple


stages of skinnier gates.


Inverters or 2-input NAND gates with low logical efforts are best for driving


nodes with a large branching effort. Use small gates after the branches to minimize


load on the driving gate.


When a path forks and one leg is more critical than the others, buffer the noncritical legs to reduce the branching effort on the critical path.


4.5.5  Limitations of Logical Effort


Logical Effort is based on the linear delay model and the simple premise that making the effort delays of each stage equal minimizes path delay. This simplicity is the method’s greatest strength, but also results in a number of limitations:


Logical Effort does not account for interconnect. The effects of nonnegligible wire  capacitance and RC delay will be revisited in Chapter 6. Logical Effort is most


applicable to high-speed circuits with regular layouts where routing delay does not  dominate. Such structures include adders, multipliers, memories, and other datapaths and arrays.


Logical Effort explains how to design a critical path for maximum speed, but not  how to design an entire circuit for minimum area or power given a ﬁxed speed constraint. This problem is addressed in Section 5.2.2.1.


Paths with nonuniform branching or reconvergent fanout are difﬁcult to analyze  by hand.


The linear delay model fails to capture the effect of input slope. Fortunately, edge  rates tend to be about equal in well-designed circuits with equal effort delay per  stage.


4.5.6  Iterative Solutions for Sizing


To address the limitations in the previous section, we can write the delay equations for each gate in the system and minimize the latest arrival time. No closed-form solutions exist, but the equations are easy to solve iteratively on a computer and the formulation still gives some insight for the designer. This section examines sizing for minimum delay, while Section 5.2.2.1 examines sizing for minimum energy subject to a delay constraint.


The ith gate is characterized by its logical effort, gi , parasitic delay, pi , and drive,xi .Formally, our goal is to ﬁnd a nonnegative vector of drives x that minimizes the arrival time of the latest output. This can be done using a commercial optimizer such as MOSEK or, for smaller problems, Microsoft Excel’s solver. The arrival time equations are classiﬁed as convex, which has the pleasant property of having a single optimum; there is no risk ofﬁnding a wrong answer. Moreover, they are of a special class of functions called posynomials, which allows an especially efﬁcient technique called geometric programming to be applied [Fishburn85].


172


Example 4.15


The circuit in Figure 4.37 has nonuniform branching, reconvergent fanout, and a wire load in the middle of the path, all of which stymie back-of-the-envelope application of Logical Effort. The wire load is given in the same units as the gate capacitances (i.e.,multiples of the capacitance of a unit inverter). Assume the inputs arrive at time 0.


Write an expression for the arrival time of the output as a function of the gate drives.


Determine the sizes to achieve minimum delay.


SOLUTION: The delay equations for each gate are obtained using EQ (4.25). Note that x indicates drive, not size. According to EQ (4.24), the input capacitance of a gate with logical effort g and drive x is Cin = gx.


(4.44)


Write the arrival times using the deﬁnitions from EQ (4.1).


(4.45)


Use a solver to choose the drives to minimize the latest arrival time. Table 4.6 summarizes the results. The minimum delay is 23.44.


The example leads to several interesting observations:


In paths that branch, each fork should contribute equal delay. If one fork were


faster than the other, it could be downsized to reduce the capacitance it presents to  the stage before the branch.


7 3


4 3


5 4


= + +=


+ + 0


a a d a a d a


a a d a a d d


2 3


= { }+= + =


max ,


+ { }+ +max ,d d d d


x5 c4 = 10


4.25 The clock buffer in Figure 4.43 can present a maximum input capacitance of 100 fF. Both true and complementary outputs must drive loads of 300 fF. Compute the


input capacitance of each inverter to minimize the worst-case delay from input to  either output. What is this delay, in ? Assume the inverter parasitic delay is 1.


4.26 The clock buffer from Exercise 4.25 is an example of a 1–2 fork. In general, if a 1–2  fork has a maximum input capacitance of C1 and each of the two legs drives a load of  C2, what should the capacitance of each inverter be and how fast will the circuit


operate? Express your answer in terms of pinv.


gclk


FIGURE 4.43  Clock buffer


FIGURE 4.42


Unit inverter


181


Power


5.1 Introduction


On Earth, apart from nuclear sources, all energy is or has been stockpiled from the sun. In essence, Earth is a huge battery that has been charged up over billions of years via the energy of sunlight in the form of plant growth, which in turn has been turned to carbon and then to oil, gas, coal or other carbon-based fuels. Additionally, in these times, we can harvest energy directly from the sun (solar power), or indirectly from the wind, tides, precipitation (hydro) or geothermal. Energy undergoes transformations. Sunlight to plant growth. Plants to carbon. Carbon to heat. Heat to electricity. Electricity to chemical (battery charging). Chemical to electricity (battery discharging). Electricity to audio (playing an MP3). In the last conversion, some energy is transformed into sound that dissipates into the universe. The rest is turned to heat as the tunes are decoded and played. It is also lost to the universe (perhaps warming our hands slightly on a cold night). So pervasive are energy transformations in everyday life, we are often not at all aware of them. Most times they occur quietly and unnoticed.


Today, we are interested in power from a number of points of view. In portable applications, products normally run off batteries. While battery technology has improved markedly over the years, it remains that a battery of a certain weight and size has a certain energy capacity. For example, a pair of rechargeable AA batteries has an energy capacity of about 7 W-hr, and a good lithium-ion laptop battery has an energy density of about 80 W-hr/lb.


Inevitably, the battery runs down and needs recharging or replacement. Product designers are interested in extending the lifetime of the battery while simultaneously adding features and reducing size, so creating low-power IC designs is key. In applications that are permanently connected to a power cord, the ever-present need to reduce dependence on fossil fuels and reduce greenhouse emissions leads us to look for low power solutions to all problems involving electronics. High-performance chips are limited to about 150 W before liquid cooling or other costly heat sinks become necessary. In 2006, data centers and servers in the United States consumed 61 billion kWh of electricity [EPA07]. This represents the output of 15 power plants, costs about $4.5 billion, and amounts to 1.5% of total U.S.


energy consumption—more than that consumed by all the television sets in the country.


While chip functionality was once limited by area, it is now often constrained by power.


High-performance design and energy-efﬁcient design have become synonymous.


In this chapter, we will examine the fundamental theory behind the various sources of power dissipation in a CMOS chip. Next, we will look at methods of estimating and minimizing these sources. Then, some architectural ideas for achieving low power are discussed.


182


While we concentrate mainly on the methods available as an IC designer to reduce power, it should be remembered that it is the application and architectural level where the major impact on power dissipation can be made. Quite simply stated, the less time you have a circuit turned on, the less power it will dissipate. It is a simple maxim, but drives all of the work on extremely low power circuits. To state this again, you must optimize power in a top-down manner, from the problem deﬁnition downward. Do not optimize from the bottom up, i.e., the circuit level; you will be doomed to fail.


5.1.1  Deﬁnitions


We have thrown some terms about already including power and energy. It is informative to go back to basics and examine what we mean by these terms and why we are even interested in them.


The instantaneous power P (t) consumed or supplied by a circuit element is the product of the current through the element and the voltage across the element


(5.1)


The energy consumed or supplied over some time interval T is the integral of the instantaneous power


(5.2)


The average power over this interval is


(5.3)


Power is expressed in units of Watts (W). Energy in circuits is usually expressed in Joules ( J), where 1 W = 1 J/s. Energy in batteries is often given in W-hr, where 1 W-hr =(1 J/s)(3600 s/hr)(1 hr) = 3600 J.


5.1.2  Examples


Figure 5.1 shows a resistor. The voltage and current are related by Ohm’s Law, V = IR, so the instantaneous power dissipated in the resistor is


(5.4)


This power is converted from electricity to heat.


Figure 5.2 shows a voltage source VDD. It supplies power proportional to its current


(5.5)


Figure 5.3 shows a capacitor. When the capacitor is charged from 0 to VC, it stores energy EC


(5.6)


The capacitor releases this energy when it discharges back to 0.


P t I t V t( ) = ( ) ( )


E P t dt


T TP t dt


avg


= = ( )1


P tV tRI t RRRR( ) = ( )= ( )22


t I t V


I t V t dt CdVdtV t dt C V t dV C


VC


= ( ) ( ) = ( ) = ( ) =


2 VC2


VR


+−


IR


FIGURE 5.1


Resistor


+VC−


IC = C  dV/dt


FIGURE 5.3


Capacitor


FIGURE 5.2


Voltage source


5.1      Introduction 183


Figure 5.4 shows a CMOS inverter driving a load capacitance. When the input switches from 1 to 0, the pMOS transistor turns ON and charges the load to VDD.


According to EQ (5.6), the energy stored in the capacitor is


(5.7)


The energy delivered from the power supply is


(5.8)


Observe that only half of the energy from the power supply is stored in the capacitor. The other half is dissipated (converted to heat) in the pMOS transistor because the transistor has a voltage across it at the same time a current ﬂows through it. The power dissipated depends only on the load capacitance, not on the size of the transistor or the speed at which the gate switches. Figure 5.5 shows the energy and power of the supply and capacitor as the gate switches.


When the input switches from 0 back to 1, the pMOS transistor turns OFF and the nMOS transistor turns ON, discharging the capacitor. The energy stored in the capacitor is dissipated in the nMOS transistor. No energy is drawn from the power supply during this transition. The same analysis applies for any static CMOS gate driving a capacitive load.


Figure 5.5 shows the waveforms as the inverter drives a 150 fF capacitor at 1 GHz.


When Vin begins to fall, the pMOS transistor starts to turn ON. It is initially saturated,and the current Ip ramps up and eventually levels out at Idsat as Vin falls. Eventually, Vout rises to the point that the pMOS shifts to the linear regime. Ip tapers off exponentially, as E


C V


L DD


= 12


I t V dt CdVdtV dt CV


dV CV


The standard method to handle voltage domain crossings is a level converter, shown in Figure 5.15. When A = 0, N1 is OFF and N2 is ON. N2 pulls Y down to 0, which turns on P1, pulling X up to VDDH and ensuring that P2 turns OFF. When A = 1, N1 is ON and N2 is OFF. N1 pulls X down to 0, which turns on P2, pulling Y up to VDDH. In either case, the level converter behaves as a buffer and properly drives Y between 0 and VDDH without risk of transistors remaining partially ON. Unfortunately, the level converter costs delay (about 2 FO4) and power at each domain crossing. [Kulkarni04] and [Ishihara04]survey a variety of other level converters. The cost can be partially alleviated by building the converter into a register and only crossing voltage domains on clock cycle boundaries.


Such level-converter ﬂops are described in Section 10.4.4.


The easiest way to use voltage domains is to associate each domain with a large area of the ﬂoorplan. Thus, each domain receives its own power grid. Note that level converters


0 1 2 3 4 5 6 7 8 9


0 10 20 30 40 50 D E


Dmin


FIGURE 5.13


Energy-delay trade-off curve


VDDH VDDL


VDDL VDDH


FIGURE 5.14


Voltage domain crossing


VDDL


VDDH


N2 P2


FIGURE 5.15  Level converter


5.2      Dynamic Power 191


require two power supplies, so they should be placed near the periphery of the domain where necessary for domain crossings.


An alterative approach is called clustered voltage scaling (CVS) [Usami95], in which two supply voltages can be used in a single block. Figure 5.16 shows an example of clustered voltage scaling. Gates early in the path use VDDH. Noncritical gates later in the path use VDDL. Voltages are assigned such that a path never crosses from a VDDL gate to a VDDH gate within a block of combinational logic, so level converters are only required at the registers. CVS requires that two power supplies be distributed across the entire block. This can be done by using two power rails. A cell library can have high- and low-voltage versions of each cell, differentiated only by the rail to which the pMOS transistors are connected, so that the ﬂavor of gate can be interchanged. Note that many processes require a large spacing between n-wells at different potentials, which limits the proximity of the VDDH and VDDL gates.


LC


VDDL Cluster


VDDH Cluster


FIGURE 5.16  Clustered voltage scaling


5.2.3.2 Dynamic Voltage Scaling (DVS)  Many systems have timevarying performance requirements. For example, a video decoder requires


more computation for rapidly moving scenes than for static scenes. A


workstation requires more performance when running SPICE than when


running Solitaire. Such systems can save large amounts of energy by


reducing the clock frequency to the minimum sufﬁcient to complete the


task on schedule, then reducing the supply voltage to the minimum necessary to operate at that frequency. This is called dynamic voltage scaling


(DVS) or dynamic voltage/frequency scaling (DVFS) [Burd00]. Figure


5.17 shows a block diagram for a basic DVS system. The DVS controller


takes information from the system about the workload and/or the die


temperature. It determines the supply voltage and clock frequency sufﬁcient to complete the workload on schedule or to maximize performance without overheating. A switching voltage regulator efﬁciently steps down Vin from a high value to the necessary VDD. The core logic contains a phase-locked loop or other clock synthesizer to generate the speciﬁed clock frequency.


The DVS controller determines the operating frequency, then chooses the lowest supply voltage suitable for that frequency. One method of choosing voltage is with a precharacterized table of voltage vs. frequency. This is inherently conservative because the voltage


Switching Voltage Regulator  VDD


Core Logic


DVS Controller


Freq Control Voltage Control


Workload


Temperature


FIGURE 5.17  DVS system


192


should be high enough to sufﬁce for even worst-case parts (see Chapter 7 about variability). The quad-core Itanium processor contains a fuse-programmable table that can be tailored to each chip during production [Stackhouse09]. Another method is to use a replica circuit such as a ring oscillator that tracks the performance of the system, as discussed in Section 7.5.3.4.


Consider how the energy for a system varies with the workload. Deﬁne the rate to be the fraction of maximum performance required to complete the workload in a speciﬁed amount of time.


Figure 5.18 plots energy against rate. If the rate is less than 1, the clock frequency can be adjusted down accordingly, or the system can run at full frequency until the work is done, then stop the clock and go to sleep; this may be simpler than building a continuously adjustable clock. Without DVS, the energy varies linearly with the rate. With ideal DVS, the voltage could also be reduced at lower rates. Assuming a linear relationship between voltage and frequency, the energy is proportional to the rate cubed, giving much greater savings at lower rates. Operating at half the maximum rate costs only one-eighth of the energy.


Such scaling assumes a continuously adjustable supply voltage, which is more expensive than a supply with discrete levels.


Characterizing a circuit across a continuous range of voltages and frequencies is also difﬁcult. If the supply voltage is limited to three levels, e.g., 1.0, 0.75, and 0.5 V, and the frequencies limited to three settings as well,much of the beneﬁt of DVS still can be achieved. Better yet, a system can dither between these voltages to save even more energy [Gutnik97]. For example, if a rate of 0.6 is required, the system could operate at a rate of 0.75 for 40% of the computation, then switch to a rate of 0.5 for the remaining 60%. Hence, by dithering between three levels,the system can achieve almost as low energy as by using an arbitrary supply voltage.


Indeed, dithering between only two supply voltages selected for full and half-rate operation is sufﬁcient to get more than 80% of the beneﬁt of DVS [Aisaka02].


Section 5.3.2 discusses power gating to turn off power to a block during sleep mode.


The same mechanism can be used to select from one of several supply voltages for each block during active mode. This allows local voltage dithering so that each block can operate at a preferred voltage.


DVS normally operates over a range from the maximum VDD down to about half that value. It can be extended further into the subthreshold regime [Zhai05a, Calhoun06a];this is sometimes called ultra-dynamic voltage scaling (UDVS). It can be challenging to build a replica circuit that tracks the worst case delay on the chip across a very wide range of voltages. DVS is now widely used in systems ranging from consumer electronics to high-performance microprocessors [Keating07, Stackhouse09].


Subthreshold and gate leakage are strongly sensitive to the supply voltage, so DVS also is effective at reducing leakage during periods of low activity.


Operating at varied VDD voltages implies an adjustable voltage regulator that reduces the voltage from a higher supply. Be careful to use a switching type regulator; otherwise,the power will just be dissipated in the regulator.


5.2.4  Frequency


Dynamic power is directly proportional to frequency, so a chip obviously should not run faster than necessary. As mentioned earlier, reducing the frequency also allows downsizing


Rate


Fixed Supply


Arbitrary Supply


Three Levels,Undithered


Three Levels,


Dithered


FIGURE 5.18  Energy reduction from DVS


5.2      Dynamic Power 193


transistors or using a lower supply voltage, which has an even greater impact on power.


The performance can be recouped through parallelism (see Section 5.5.2), especially if area is not as important as power.


Even if multiple voltage supplies are not available, a chip may still use multiple frequency domains so that certain portions can run more slowly than others. For example, a microprocessor bus interface usually runs much slower than the core. Low frequency domains can also save energy by using smaller transistors.


Frequency domain crossings are easiest if the frequencies are related by integer multiples and the clocks are synchronized between domains. Section 10.6 discusses synchronization further.


5.2.5  Short-Circuit Current


Short-circuit power dissipation occurs as both pullup and pulldown networks are partially ON while the input switches, as was illustrated in Figure 5.5. It increases as the input edge rates become slower because both networks are ON for more time [Veendrick84]. However, it decreases as load capacitance increases because with large loads the output only switches a small amount during the input transition, leading to a small Vds across the transistor that is causing the short-circuit current. Unless the input edge rate is much slower than the output edge rate, short-circuit current is a small fraction (< 10%) of current to the load and can be ignored in hand calculations. It is good to use relatively crisp edge rates at the inputs to gates with wide transistors to minimize their short-circuit current. This is achieved by keeping the stage effort of the previous stage reasonable, e.g., 4 or less. In general, gates with balanced input and output edge rates have low short-circuit power.


Short-circuit power is strongly sensitive to the ratio v = Vt / VDD. In the limit that v > 0.5, short-circuit current is eliminated entirely because the pullup and pulldown networks are never simultaneously ON. For v = 0.3 or 0.2, short-circuit power is typically about 2% or 10% of switching power, respectively, assuming clean edges [Nose00a]. In nanometer processes, Vt can scarcely fall below 0.3 V without excessive leakage, and VDD is on the order of 1 V, so short-circuit current has become almost negligible.


5.2.6  Resonant Circuits


Resonant circuits seek to reduce switching power consumption by letting energy slosh back and forth between storage elements such as capacitors and inductors rather than dumping the energy to ground. The technique is best suited to applications such as clocks that operate at a constant frequency.


Figure 5.19 shows a model of a resonant clock network [Chan05]. Cclock is the


capacitance of the clock network. In an ordinary clock circuit, it is driven between


VDD and GND by a strong clock buffer. The resonant clock network adds the


inductor L1 and the capacitor C2, which is approximately 10Cclock. Rclock and Rind


represent losses in the clock wires and in the inductor that lower the quality of the


resonator. In the resonant clock circuit, energy moves back and forth between L1


and Cclock, causing a sinusoidal oscillation at the resonant frequency f. The driver


pumps in just enough energy to compensate for the resistive losses. C2 must be large


enough to store excess energy and not interfere with the resonance of the clock


capacitance.


(5.18)


L C


1 clock


Cclock Rclock L1


Rind


FIGURE 5.19


Resonant clock network


194


In a mechanical analogy, inductors represent springs and capacitors represent mass.


The clock itself has high capacitance and little inductance, representing a rigid mass suspended on a set of springs corresponding to the inductor L1. The mass oscillates up and down. The clock driver gives the mass a kick to get it started and compensate for damping in the springs, but little energy is required because the springs do most of the work storing energy on the way down and delivering it back to the mass on the way up.


IBM has demonstrated a resonant global clock distribution system for the Cell processor [Chan09]. At an operating frequency of 4–5 GHz, the system could reduce chip power by 10%. Some of the drawbacks of resonant clocking include the limited range of operating frequencies, the sinusoidal clock output, and the difﬁculty of building a highquality inductor in a CMOS process.


5.3 Static Power


Static power is consumed even when a chip is not switching. CMOS has replaced nMOS processes because contention current inherent to nMOS logic limited the number of transistors that could be integrated on one chip. Static CMOS gates have no contention current. Prior to the 90 nm node, leakage power was of concern primarily during sleep mode because it was negligible compared to dynamic power. In nanometer processes with low threshold voltages and thin gate oxides, leakage can account for as much as a third of total active power. Section 2.4.4 introduced leakage current mechanisms. This section brieﬂy reviews each source of static power. It then discusses power gating, which is a key technique to reduce power in sleep mode. Because subthreshold leakage is usually the dominant source of static power, other techniques for leakage reduction are explored, including multiple threshold voltages, variable threshold voltages, and stack forcing.


5.3.1  Static Power Sources


As given in EQ (5.12), static power arises from subthreshold, gate, and junction leakage currents and contention current. Entire books have been written about leakage[Narendra06], but this section summarizes the key effects.


5.3.1.1 Subthreshold Leakage  Subthreshold leakage current ﬂows when a transistor is supposed to be OFF. It is given by EQ (2.45). For Vds exceeding a few multiples of the thermal voltage (e.g., Vds > 50 mV), it can be simpliﬁed to


(5.19)


where Ioff is the subthreshold current at Vgs = 0 and Vds = VDD, and S is the subthreshold slope given by EQ (2.44) (about 100 mV/decade). Ioff is a key process parameter deﬁning the leakage of a single OFF transistor. It ranges from about 100 nA/ m for typical low-Vt devices to below 1 nA/ m for high-Vt devices.  is the DIBL coefﬁcient, typically around 100 mV/V for a 65 nm transistor, and trending upward because the drain exerts an increasing inﬂuence on the channel as the geometry shrinks. If Vds is small, Isub may decrease by roughly an order of magnitude from Ioff. k  is the body effect coefﬁcient, which describes how the body effect modulates the threshold voltage. Raising the source voltage or applying a negative body voltage can further decrease leakage.


k V


sub off


5.3      Static Power 195


Ioff is usually speciﬁed at 25 °C and increases exponentially with temperature because Vt decreases with temperature and S is directly proportional to temperature. Ioff typically increases by one to two orders of magnitude at 125 °C, so limiting die temperature is essential to controlling leakage.


The leakage through two or more series transistors is dramatically reduced on account of the stack effect [Ye98, Narendra01]. Figure 5.20 shows two series OFF transistors with gates at 0 volts. The drain of N2 is at VDD, so the stack will leak. However, the middle node voltage Vx settles to a point that each transistor has the same current. If Vx is small,N1 will see a much smaller DIBL effect and will leak less. As Vx rises, Vgs for N2 becomes negative, reducing its leakage. Hence, we would expect that the series transistors leak less.


This can be demonstrated mathematically by solving for Vx and Isub, assuming that Vx > 50 mV.


(5.20)


(5.21)


(5.22)


Using the typical values above and VDD = 1.0 V, we ﬁnd that the stack effect


reduces subthreshold leakage by a factor of about 10. Stacks with three or more


OFF transistors have even lower leakage.


Subthreshold leakage cannot be reduced without consideration of other forms


of leakage [Mukhopadhyay05]. Raising the halo doping level to raise Vt by controlling DIBL and short-channel effects causes BTBT to increase. Applying a reverse


body bias to increase Vt also causes BTBT to increase. Applying a negative gate


voltage to turn the transistor OFF more strongly causes GIDL to increase. Figure


5.21 shows how subthreshold leakage dominates in a 50 nm process at low Vt , but


how the other sources take over at higher Vt [Agarwal07].


Silicon on Insulator (SOI) circuits are attractive for low-leakage designs because they have a sharper subthreshold current rolloff (smaller n in EQ (2.42)). SOI circuit design will be discussed further in Section 9.5.


5.3.1.2 Gate Leakage  Gate leakage occurs when carriers tunnel through a thin gate dielectric when a voltage is applied across the gate (e.g., when the gate is ON). A process usually speciﬁes IG in nA/ m for a minimum-length gate or in A/mm2 of transistor gate.


Gate leakage is an extremely strong function of the dielectric thickness. It is normally limited to acceptable levels in the process by selection of the dielectric thickness. pMOS gate leakage is an order of magnitude smaller in ordinary SiO2 gates and can often be ignored,but it can be signiﬁcant for other gate dielectrics.


Gate leakage also depends on the voltage across the gate. For example, Figure 5.22 shows two series transistors. If N1 is ON and N2 is OFF, N1 has Vgs = VDD and experiences full gate leakage. On the other hand, if N1 is OFF and N2 is on, N2 has Vgs = Vt and I


sub oﬀ


−


η


− γ


=+ +1 2


k k


1 1 2


V S


0 0


Vx VDD


N2


FIGURE 5.20


Series OFF transistors  demonstrating the stack  effect


FIGURE 5.21


Leakage as a function of Vt(© IEEE 2007.)


Vx = 0 VDD


Vx = VDD Vt N1


FIGURE 5.22


Gate leakage in series stack


196


experiences negligible gate leakage [Lee03, Mukhopadhyay03]. In both cases, the OFF transistor has no gate leakage. Thus, gate leakage can be alleviated by stacking transistors such that the OFF transistor is closer to the rail.


Table 5.2 summarizes the combined effects of gate and subthreshold leakage on the 3-input NAND gate shown in Figure 5.23 using data from [Lee03] for a process with 15Å oxides and 60 nm channel length. The gate leakage through an ON nMOS transistor is


6.3 nA. pMOS gate leakage is negligible. The subthreshold leakage through an nMOS transistor with Vds = VDD is 5.63 nA and the subthreshold leakage through a pMOS transistor with |Vds| = VDD is 9.3 nA.


The NAND3 beneﬁts from the stack effect to reduce subthreshold leakage. In the 000 case, all three nMOS transistors are OFF and the triple stack effect cuts leakage by a factor of 10. Both intermediate nodes drift up to somewhere around 100–200 mV set by the stack effect. In the 001 and 100 cases, two nMOS transistors are OFF and the double stack effect cuts leakage by a factor of 5. In the 110 case, the nMOS stack experiences full subthreshold leakage because only one transistor is OFF and it sees Vds = VDD. In the 011 and 101 cases, the single OFF nMOS transistor sees Vds = VDD – Vt , so the leakage is partially reduced. In the 111 case, all three parallel pMOS transistors leak.


The NAND3 also sees pattern-dependent gate leakage. In the 000 case, all three nMOS transistors are off, so no gate current ﬂows. In the 001 and 011 cases, the ON transistors see Vgs = Vt and thus have little leakage. In the 010 case, gate leakage through N2 charges Vx and Vz up to an intermediate voltage until the increase in source/drain voltage reduces the gate current. This raises the source voltage of N3, effectively eliminating its subthreshold leakage. In the 101 case, N 1 sees full gate leakage, while N 3 has little because Vz is at a high voltage. In the 110 case, N1 and N2 both see gate leakage, and in the 111 case, all three nMOS transistors leak.


5.3.1.3 Junction Leakage  Junction leakage occurs when a source or drain diffusion region is at a different potential from the substrate. Although the ordinary leakage of reverse-biased diodes is usually negligible, BTBT and GIDL can result in leakage currents that approach subthreshold leakage levels in high-Vt transistors. BTBT is maximum when a strong reverse bias is applied between the drain and body (e.g., Vdb = VDD for an nMOS transistor). GIDL is maximum when the transistor is OFF and a strong bias is applied to the drain (e.g., Vgd = –VDD for an nMOS transistor). Junction leakage is often


TABLE 5.2  Gate and subthreshold leakage in NAND3 (nA)Input State (ABC) Isub Igate Itotal


Vx


Vz


0 0.4


stack effect


001


0 0.7


VDD – Vt


010


0 1.3 1.3


intermediate


011


3.8


0 10.1


0.7 6.3 7.0


101


3.8 6.3 10.1


5.6 12.6 18.2


111


28 18.9 46.9


N1 N2


N3


FIGURE 5.23  NAND gate  demonstrating pattern


dependence of gate and  subthreshold leakage


5.3      Static Power 197


minor in comparison to the other leakages, but can be expressed in nA/ m of transistor width when it needs to be considered.


5.3.1.4 Contention Current  Static CMOS circuits have no contention current. However,certain alternative circuits inherently draw current even while quiescent. For example,pseudo-nMOS gates discussed in Section 9.2.2 experience contention between the nMOS pulldowns and the always-on pMOS pullups when the output is 0. Current-mode logic and many analog circuits also draw static current. Such circuits should be turned OFF in sleep mode by disabling the pullups or current source.


5.3.1.5 Static Power Estimation  Static current estimation is a matter of estimating the total width of transistors that are leaking, multiplying by the leakage current per width,and multiplying by the fraction of transistors that are in their leaky state (usually onehalf ). Add the contention current if applicable. The static power is the supply voltage times the static current.


Example 5.4


Consider the system-on-chip from Example 5.1. Subthreshold leakage for OFF devices is 100 nA/ m for low-threshold devices and 10 nA/ m for high-threshold devices. Gate leakage is 5 nA/ m. Junction leakage is negligible. Memories use lowleakage devices everywhere. Logic uses low-leakage devices in all but 5% of the paths that are most critical for performance. Estimate the static power consumption.


SOLUTION: There are (50  106 logic transistors)(0.05)(12 )(0.025 m/ ) = 0.75  106 m of low-threshold devices and [(50  106 logic transistors)(0.95)(12 ) + (950  106 memory transistors)(4 )](0.025 m/ ) = 109.25  106 m of high-threshold devices.


Neglecting the beneﬁts of series stacks, half the transistors are OFF and contribute subthreshold leakage. Half the transistors are ON and contribute gate leakage. Isub =[(0.75  106 m)(100 nA/ m) + (109.25  106 m)(10 nA/ m)]/2 = 584 mA. Igate =((0.75 + 109.25)  106 m)(5 nA/ m)/2 = 275 mA. Pstatic = (584 mA + 275 mA)(1 V)= 859 mW. This is 15% of the switching power and is enough to  deplete the battery of a hand-held device rapidly.


5.3.2  Power Gating


The easiest way to reduce static current during sleep mode is to turn off the power supply to the sleeping blocks. This technique is called power gating and is shown in Figure 5.24. The logic block receives its power from a virtual VDD rail,VDDV. When the block is active, the header switch transistors are ON, connecting VDDV to VDD. When the block goes to sleep, the header switch turns OFF,allowing VDDV to ﬂoat and gradually sink toward 0. As this occurs, the outputs of the block may take on voltage levels in the forbidden zone. The output isolation gates force the outputs to a valid level during sleep so that they do not cause problems in downstream logic.


Power gating introduces a number of design issues. The header switch requires careful sizing. It should add minimal delay to the circuit during active operation, and should have low leakage during sleep. The transition between active and sleep modes takes some time and energy, so power gating is only effective when a block is turned off long enough. When a block is gated, the


VDDV


Sleep


PowerGated Block


Output Isolation Header Switch


Transistors


FIGURE 5.24  Power gating


198


state must either be saved or reset upon power-up. Section 10.4.3 discusses state retention registers that use a second power supply to maintain the state. Alternatively, the important registers can be saved to memory so the entire block can be power-gated. The registers must then be reloaded from memory when power is restored. [Keating07] addresses at length how to use power gating in a standard CAD ﬂow. If power switches are fast enough, they can be used to save leakage power during active mode by powering down clock-gated blocks [Tschanz03, Min06]. If saving or losing the state costs too much overhead, turning the power supply down to the minimum level necessary to retain state(about 300 mV) using DVS is sufﬁcient to eliminate gate leakage and reduce subthreshold leakage energy by more than an order of magnitude [Calhoun04].


Power gating was originally proposed as Multiple Threshold CMOS (MTCMOS)[Mutoh95] because it used low-Vt transistors for logic and high-Vt header and footer switches. However, the name is somewhat confusing because a system may use multiple threshold voltages without power gating. Moreover, it is unnecessary to switch both VDD and GND.


5.3.2.1 Power Gate Design  Power gating can be done externally with a disable input to a voltage regulator or internally with high-Vt header or footer switches. External power gating completely eliminates leakage during sleep, but it takes a long time and signiﬁcant energy because the power network may have 100s of nF of decoupling capacitance to discharge.


On-chip power gating can use pMOS header switch transistors or nMOS footer switch transistors. nMOS transistors deliver more current per unit width so they can be smaller. On the other hand, if both internal and external power gating are used, it is more consistent for both methods to cut off VDD. pMOS power gating also is simpler when multiple power supplies are employed. As a practical matter, ensuring that GND is always constant reduces confusion among designers and CAD tools; this alone is enough for many projects to choose pMOS power gating.


Theoretically, it is possible to use ﬁne-grained power gating applied to individual logic gates, but placing a switch in every cell has enormous area overhead. Practical designs use coarse-grained power gating where the switch is shared across an entire block. The switch has an effective resistance that inevitably causes some voltage droop on VDDV and increases the delay of the block. The switch is commonly sized to keep this delay to 5–10%. One way to achieve this is to calculate or simulate how much voltage droop can occur on VDDV while maintaining acceptable delay. Then the average current of the block is determined through power analysis. The switch width is chosen so that the voltage droop is small enough when the average current ﬂows through the switch. If the block is large enough that switching events are spread over time and has enough capacitance on VDDV to smooth out ripples, this average current method [Mutoh99] is satisfactory. Wider switches reduce the droop but have more leakage when OFF and take more energy. For example, 45 nm Core processors use 1.5 meters of low-leakage pMOS power gate transistor per core to turn off the idle cores [Kumar09].


Example 5.5


A cache in a 65 nm process consumes an average power of 2 W. Estimate how wide should the pMOS header switch be if delay should not increase by more than 5%?


SOLUTION: The 65 nm process operates at 1 V, so the average current is 2 W / 1 V = 2 A.


The pMOS transistor has an ON resistance of R = 2 k · m. A 5% delay increase


5.3      Static Power 199


corresponds to a droop on VDDV of about 5% (check this using EQ (4.29). Thus, Rswitch= 0.05  × 1 V / 2 A = 25 m . So the transistor width must be k · m/25 m = 8 × 104


m. The ON resistance at low Vds is lower than R. Circuit simulation shows that a width of 3.7 × 104 m sufﬁces to keep droop to 5%.


The power switch is generally made of many transistors in parallel. The length and width of the transistors should be selected to maximize the Ion / Ioff ratio; this is highly process-dependent and generally requires SPICE simulations sweeping L and W. A reverse body bias may be applied to the power switch transistors during sleep mode to improve their Ion / Ioff ratio (see Section 5.3.4). Alternatively, the switch can be overdriven positively or negatively to turn it ON or OFF more effectively so long as the gate oxide is not overstressed [Min06].


When the power switch is turned ON, the sudden inrush of current can cause IR and L di/dt drop noise (see Section 13.3) and electromigration of the power bus (see Section


7.3.3.1). To alleviate these problems, the switch can be turned on gradually by controlling how many parallel transistors are ON.


5.3.3  Multiple Threshold Voltages and Oxide Thicknesses


Selective application of multiple threshold voltages can maintain performance on critical paths with low-Vt transistors while reducing leakage on other paths with high-Vt transistors.


A multiple-threshold cell library should contain cells that are physically identical save for their thresholds, facilitating easy swapping of thresholds. Good design practice starts with high-Vt devices everywhere and selectively introduces low-Vt  devices where necessary.


Using multiple thresholds requires additional implant masks that add to the cost of a CMOS process. Alternatively, designers can increase the channel length, which tends to raise the threshold voltage via the short channel effect. For example, in Intel’s 65 nm process, drawing transistors 10% longer reduces Ion by 10% but reduces Ioff by a factor of 3[Rusu07]. The dual-core Xeon processor uses longer transistors almost exclusively in the caches and in 54% of the core gates.


Most nanometer processes offer a thin oxide for logic transistors and a much thicker oxide for I/O transistors that can withstand higher voltages. The oxide thickness is controlled by another mask step. Gate leakage is negligible in the thick oxide devices, but their performance is inadequate for high speed logic applications. Some processes offer another intermediate oxide thickness to reduce gate leakage.


[Anis03] provides an extensive survey of the applications of multiple thresholds.


5.3.4  Variable Threshold Voltages


Recall from EQ (2.38) that Vsb modulates the threshold voltage through the body effect.


Another method to achieve high Ion in active mode and low Ioff in sleep mode is to dynamically adjust the threshold voltage of the transistor by applying a body bias. This technique is sometimes called variable threshold CMOS (VTCMOS).


For example, low-Vt devices can be used and a reverse body bias (RBB) can be applied during sleep mode to reduce leakage [Kuroda96]. Alternatively, higher-Vt devices can be used, and then a forward body bias (FBB) can be applied during active mode to increase performance [Narendra03]. Body bias can be applied to the power gating transistors to turn them off more effectively during sleep.


Too much reverse body bias (e.g., < –1.2 V)  leads to greater junction leakage through BTBT [Keshavarzi01], while too much forward body bias (> 0.4 V) leads to substantial current through the body to source diodes. According to EQ (2.39), the body effect weakens as tox becomes thinner, so body biasing offers diminishing returns at 90 nm and below[von Arnim05].


Applying a body bias requires additional power supply rails to distribute the substrate and well voltages. For example, an RBB scheme for a 1.0 V n-well process could bias the p-type substrate at VBBn = – 0.4 V and the n-well at VBBp =  1.4 V. Figure 5.25 shows a schematic and cross-section of an inverter using body bias. In an n-well process, all nMOS transistors share the same p substrate and must use the same VBBn. In a triple-well process,groups of transistors can use different p-wells isolated from the substrate and thus can use different body biases. The well and substrate carry little current, so the bias voltages are relatively easy to generate using a charge pump (see Section 13.3.8).


GND VBBp


VBBn


VDD VBBp


FIGURE 5.25  Body bias


5.3.5  Input Vector Control


As was illustrated in Table 5.2, the stack effect and input ordering cause subthreshold and gate leakage to vary by up to two orders of magnitude between best and worst cases.


Therefore, the leakage of a block of logic depends on gate inputs, which in turn depend on the inputs to the block of logic. The idea of input vector control is to apply the input pattern that minimizes block leakage when the block is placed in sleep mode [Narendra06,Abdollahi04]. The vector can be applied via set/reset inputs on the registers or via a scan chain. It is hard to control all the gates in a block of logic using only the block inputs, but the best input vectors may save 25–50% of leakage as compared to random vectors. Applying the input vector causes some switching activity, so a block may need to remain in sleep for thousands of cycles to recoup the energy spent entering the sleep state.


5.4 Energy-Delay Optimization


At this point, a natural question is: what is the best choice of VDD and Vt ? The answer, of course, depends on the objective. Minimum power by itself is not an interesting objective because it is achieved as the delay for a computation approaches inﬁnity and nothing is accomplished. The time for a computation must be factored into the analysis. Better metrics include minimizing the energy, minimizing the energy-delay product, and minimizing energy under a delay constraint.


5.4.1  Minimum Energy


According to EQ (5.3), the product of the power of an operation and the time for the operation to complete is the energy consumed. Hence, the power-delay product (PDP) is simply the


5.4      Energy-Delay Optimization 201


energy. The minimum energy point is the least energy that an operation could consume if delay were unimportant. It occurs in subthreshold operation where VDD < Vt . The minimum energy point typically consumes an order of magnitude less energy than the conventional operating point, but runs at least three orders of magnitude more slowly [Wang06].


John von Neumann ﬁrst asserted (without justiﬁcation) that the “thermodynamic minimum of energy per elementary act of information” was kT ln2 [von Neumann66].


[Meindl00] proved this result for CMOS by considering the minimum allowable voltage at which an inverter could operate. To achieve nonzero noise margins, an inverter must have a slope steeper than –1 at the switching point, Vinv. For an ideal inverter with n = 1 in the subthreshold characteristics, this occurs at a minimum operating voltage of


(5.23)


The energy stored on the gate capacitance of a single MOSFET is E = QVDD/2,where Q is the charge. The minimum possible charge is one electron, q. Substituting Vmin for VDD gives Emin = kT ln 2 = 2.9 × 10–21 J. In contrast, a unit inverter in a 0.5 m 5 V process draws about 1.5 × 10–13 J from the supply when switching, and the same inverter in a 65 nm 1 V process draws 3 × 10–16 J.


Inverters have been demonstrated operating with power supplies under 100 mV, but these do not actually minimize energy in a real CMOS process. Although they have extremely low switching energy, they run so slowly that the leakage energy dominates. The true minimum energy point is at a higher voltage that balances switching and leakage energy.


In subthreshold operation, the current drops exponentially as VDD – Vt decreases and thus the delay increases exponentially. The switching energy improves quadratically with VDD. Leakage current improves slowly with VDD because of DIBL, but the leakage energy increases exponentially because the slower gate leaks for a longer time. To achieve minimum energy operation, all transistors should be minimum width. This reduces both switching capacitance and leakage. Gate and junction leakage and short-circuit power are negligible in subthreshold operation, so the total energy is the sum of the switching and leakage energy, which is minimized near the point they crossover, as shown in Figure 5.26. V


vT


min ln= =2 2 36 mV@ 300 K


VDD(V)


10 6


1.5


Analytical Solution


10 5 10 4 10 3 10 2 10 1 100


ET


EL


EDYN


TD


ILEAK


0 10 6


FIGURE 5.26  Minimum energy point (Reprinted from [Calhoun05]. ©2005 IEEE.)


202


To compute the energy, assume that a circuit has N gates on the critical path, a total effective capacitance Ceff, and a total effective width Weff of leaking transistor. The delay of a gate operating subthreshold with a load Cg is given by EQ (4.31). The cycle time is thus


(5.24)


The energy consumed in one cycle is


(5.25)


It is possible to differentiate EQ (5.25) with respect to VDD to ﬁnd the minimum energy point [Calhoun05], but the results are rather messy.


A more intuitive approach is to look at the minimum energy point graphically. Figure


5.27(a) plots the energy and delay contours as a function of VDD and Vt for a ring oscillator in a 180 nm process designed to reﬂect the behavior of a microprocessor pipeline[Wang02]. As VDD increases or Vt decreases, the operating frequency increases exponentially assuming the circuit is operating at or near threshold. At VDD = Vt , the circuit operates at about 10 MHz. The energy contours are normalized to the minimum energy point.


This point, marked with a cross, occurs at VDD = 0.13 V and Vt = 0.37 V. The energy is about 10 times lower than at a typical operating point, but the delay is three to four orders of magnitude greater.


The shape of the curve is only a weak function of process parameters, so it remains valid for nanometer processes. However, the result does depend strongly on the relative switching and leakage energies. Figure 5.27(b) plots the results when the activity factor drops to 0.1, reducing Ceff. Switching energy is less important, so the circuit can run at a higher supply voltage. The threshold then increases to cut leakage. The total energy is D


NkC V


g DD


I V D W NkC


VD


switching eff


leak sub


D V


V C W NkC


total switching leak


eff eff


= + =


1.05


1.25


1.75


0.35


0.45


0.55


0.1 0.20.3 0.4 0.5 0.6


0.1


1.75 2


V DD = V t


FIGURE 5.27  Contours of energy and delay for ring oscillators with (a)  = 1, (b)  = 0.1 (Adapted from [Wang02]. © IEEE 2002.)


5.4      Energy-Delay Optimization 203


greatly reduced. The result also depends on temperature: at high temperature, circuits leak more so a higher threshold voltage should be used. Process variation also pushes the best operating point toward higher voltage and energy.


5.4.2  Minimum Energy-Delay Product


The energy-delay product (EDP) is a popular metric that balances the importance of energy and delay [Gonzalez97, Stan99, Nose00c]. Neglecting leakage, we can elegantly solve for the supply voltage that minimizes EDP. Considering leakage, the best supply voltage is slightly higher.


First, consider the EDP when leakage is negligible. The energy to charge a load capacitance Ceff is given by EQ (5.7). The delay, using an -power law model, is given by EQ (4.29). Thus, the EDP is


(5.26)


Differentiating with respect to VDD and setting the result to 0 gives the voltage at which the EDP is minimized


(5.27)


Recall that  is between 1 (completely velocity saturated) and 2 (no velocity saturation). For a typical value


of , we come to the interesting conclusion that


VDD-opt  2Vt , which is substantially lower than most


systems presently run.


EQ (5.26) suggests that the EDP improves as Vt


approaches 0, which is obviously not true because leakage power would dominate. When a leakage term is


incorporated into EQ (5.27), the results become too


messy to reprint here. Figure 5.28 shows contours of


EDP and delay as a function of VDD and Vt . EDP is


normalized to the best achievable. For typical process


parameters, the best Vt is about 100–150 mV and the


EDP is about four times better than at a typical operating point of VDD = 1.0 V and Vt = 0.3 V. At the optimum, leakage energy is about half of dynamic energy.


The dashed lines indicate contours of equal speed, normalized to the speed at the best EDP point. To operate at higher speed requires increasing the EDP. Section 7.5.3.2 will revisit this analysis considering process variation and show that the minimum EDP point occurs at a higher voltage and threshold when variations are accounted for.


5.4.3  Minimum Energy Under a Delay Constraint


In practice, designers generally face the problem of achieving minimum energy under a delay constraint. Equivalently, the power consumption of the system is limited by battery or cooling considerations and the designer seeks to achieve minimum delay under an


EDP


kC V


opt


2.7


1.8


FIGURE 5.28  Contours of energy-delay product (Adapted from [Gonzalez97]. © IEEE 1997.)


204


energy constraint. Figure 5.27(a) showed contours of delay and energy. The best supply voltage and threshold for operation at a given delay is where the delay and energy contours are tangent.


For a given supply voltage and threshold voltage, the designer can make logic and sizing choices that affect delay and energy. Figure 5.13 showed an example of an energydelay trade-off curve. Such curves can be generated using a logic synthesizer or sizing tool constrained to various delays. The curve becomes steep near the point of minimum delay,so energy-efﬁcient designs should aim to operate at a longer delay.


Energy under a delay constraint is also minimized when leakage is about half of dynamic power [Markovic 04]. However, the curve is fairly ﬂat around this point, so many designs operate at lower leakage to facilitate power saving during sleep mode.


5.5 Low Power Architectures


VLSI design used to be constrained by the number of transistors that could ﬁt on a chip.


Extracting maximum speed from each transistor maximized overall performance. Now that billions of nanometer-scale transistors ﬁt on a chip, many designs have become power constrained and the most energy-efﬁcient design is the highest performer. This is one of the factors that has driven the industry’s abrupt shift to multicore processors.


5.5.1  Microarchitecture


Energy-efﬁcient architectures take advantage of the structured design principles of modularity and locality [Horowitz04, Naffziger0b]. [Pollack99] observed that processor performance grows with the square root of the number of transistors. Building complex,sprawling processors to extract the last bit of instruction-level parallelism from a problem is a highly inefﬁcient use of energy. Microarchitectures are moving toward larger numbers of simpler cores seeking to handle task and data-level parallelism. Smaller cores also have shorter wires and faster memory access.


Memories have a much lower power density than logic because their activity factors are miniscule and their regularity simpliﬁes leakage control. If a task can be accelerated using either a faster processor or a larger memory, the memory is often preferable. Memories now comprise more than half the area of many chips.


Special-purpose functional units can offer an order of magnitude better energy efﬁciency than general-purpose processors. Accelerators for compute-intensive applications such as graphics, networking, and cryptography ofﬂoad these tasks from the processor.


Such heterogeneous architectures, combining regular cores, specialized accelerators, and large amounts of memory, are of growing importance.


Commercial software has historically lagged at least a decade behind hardware advances such as virtual memory, memory protection, 32- and 64-bit datapaths, and robust power-management. Presently, programmers have trouble taking advantage of many cores. Time will tell whether programming practices and tools catch up or whether microarchitectures will have to yield to the needs of programmers.


5.5.2  Parallelism and Pipelining


In the past, parallelism and pipelining have been effective ways to reduce power consumption, as shown in Figure 5.29 [Chandrakasan92].


5.5      Low Power Architectures 205


Replacing a single functional unit with N parallel units allows each to operate at 1/N the frequency. A multiplexer selects between the results. The voltage can be scaled down accordingly, offering quadratic savings in energy at the expense of doubling the area. Replacing a single functional unit with an N-stage pipelined unit also reduces the amount of logic in a clock cycle at the expense of more registers. Again, the voltage can be scaled down. The two techniques can be combined for even better energy efﬁciency.


When leakage is unimportant, parallelism offers a slight edge because the multiplexer has less overhead than the pipeline registers.


Also, perfectly balancing logic across pipeline stages can be difﬁcult.


Now that leakage is a substantial fraction of total power, pipelining becomes preferable because the parallel hardware has N times as much leakage [Markovic 04].


Now that VDD is closer to the best energy-delay point, the potential supply reduction and energy savings are diminishing. Nevertheless, parallelism and pipelining remain primary tools to extract performance from the vast transistor budgets now available.


5.5.3  Power Management Modes


As your parents taught you to turn off the lights when you leave a room, chip designers have now learned they must turn off portions of the chip when they are not active by applying clock and power gating. Many chips now employ a variety of power management modes giving a trade-off between power savings and wake-up time.


For example, the Intel Atom processor [Gerosa09] operates at a peak frequency of 2 GHz at 1 V, consuming 2 W. The power management modes are shown in Figure 5.30.


In the low frequency mode, the clock drops as slow as 600 MHz while the power supply


f/2


FIGURE 5.29  Functional units: (a) normal,


(b) parallel, (c) pipelined


Partial Flush OFF


Flushed


OFF OFF OFF


OFF OFF


C0 HFM


C0 LFM


Core Voltage


Core Clock


PLL


L1 Caches


L2 Caches


Wake-Up Time


C1/C2


C4


C6


< 1 s < 30 s < 100 s


FIGURE 5.30  Atom power management modes (© 2009 IEEE.)


206


reduces to 0.75 V. In sleep mode C1, the core clock is turned off and the level 1 cache isﬂushed and power-gated to reduce leakage, but the processor can return to active state in 1 microsecond. In sleep mode C4, the PLL is also turned OFF. In sleep mode C6, the core and caches are all power-gated to reduce power to less than 80 mW, but wake-up time rises to 100 microseconds. For a typical workload, the processor can spend 80–90% of its time in C6 sleep mode, reducing average power to 220 mW.


The worst-case power that a chip may consume can be a factor of two or more greater than the normal power. Code triggering maximal power consumption is sometimes called a thermal virus [Naffziger06] because it seeks to burn out the chip. To avoid having to design for this worst case, chips can employ adaptive features, throttling back activity if the issue rate or die temperature becomes too high. Section 13.2.5 discusses temperature sensors further.


Power management results in substantially lower power consumption during idle mode than active mode. The transition between idle and active may require multiple cycles to avoid sudden current spikes that excite power supply resonances and cause excessive supply noise.


5.6 Pitfalls and Fallacies


Oversizing gates


Designers seeking timing closure tend to crank up the size of gates. Doubling the size of all the  gates on a gate-dominated path does not improve delay, but doubles the power consumption.


Designing for speed without regard to power


Nanometer processes have reached a point where it is no longer possible to design a large chip  for speed without regard to power: the chip will be impossible to cool. Designs must be power  efficient. Systems tuned exclusively for speed tend to use large gates and speculative logic that  consumes a great deal of power. If a core or processing element can be simplified to offer 80% of the performance at 50% of the power, then two cores in parallel can offer 160% of the


throughput at the same power.


Reporting power at a given frequency instead of energy per operation


Sometimes a module is described by its power at an arbitrary frequency (e.g., 10 mW @ 1 GHz). This is equivalent to reporting energy because E = P/f (e.g., 10 pJ). Reporting energy is arguably  cleaner because it is a single number.


Reporting Power-Delay Product when Energy-Delay Product is meant


Extending the previous point, sometimes a system is described by its PDP at a given frequency, where the frequency is slower than the reciprocal of the delay. This metric is really a variation  of the EDP, because the power at a low enough frequency is equivalent to energy. Reporting the  EDP is definitely cleaner because it doesn’t involve an arbitrary choice of frequency.


Failing to account for leakage


Many designers are accustomed to focusing on dynamic power. Leakage in all its forms has become extremely important in nanometer processes. Ignoring it not only underestimates power  consumption but also can cause functional failures in sensitive circuits.


5.7      Historical Perspective 207


5.7 Historical Perspective


The history of electronics has been a relentless quest to reduce power so that more capabilities can be provided in a smaller volume.


The Colossus, brought online in 1944, was one of the world’s ﬁrst fully electronic computers. The secret machine was built from 2400 vacuum tubes and consumed 15 kW as it worked day and night decrypting secret German communications. The machine was destroyed after the war, but a functional replica shown in Figure 5.31 was rebuilt in 2007.


Vacuum tube machines ﬁlled entire rooms and failed frequently. Imagine the problem of keeping 2400 light bulbs burning simultaneously. By the 1960s, vacuum tubes were surpassed by solid-state transistors that were far smaller and consumed milliwatts rather than watts. Gordon Moore soon issued his famous prophecy about the exponential growth in the number of transistors per chip.


MOSFETs entered the scene commercially around 1970. For more than a decade,nMOS technology predominated because it could pack transistors more densely (and hence cheaply) than CMOS. nMOS circuits used depletion load (negative-Vt ) nMOS pullups as resistive loads, so each gate with an output of 0 dissipated contention power. For example, Figure 5.32 shows an nMOS 2-input NOR gate.


CMOS circuits made their debut in watch circuits (pioneered by none other than the Swiss, of course!), where their key ability to draw almost zero power while not switching was critical [Vittoz72]. This use succeeded despite very low circuit densities and low circuit speed of the CMOS technologies of the day. It was not until the mid 1980s that the ever-increasing power dissipation of mainstream circuits such as microprocessors forced a move from nMOS to CMOS technology, again despite density arguments.


FIGURE 5.31  Reconstructed Colossus Mark 2 (Photograph by Tony Sale. Reprinted with permission.)


Depletion-Mode


nMOS Load


FIGURE 5.32


nMOS NOR gate


208


As engineers became capable of integrating millions (and now billions) of CMOS transistors onto a single chip, power consumption became a concern for CMOS as well. In the 1990s, designers facing the power wall abandoned the longcherished 5 V standard and began scaling power supplies to reduce dynamic power. Eventually, this forced threshold voltages to decrease until subthreshold leakage has become an issue. As gate dielectrics have scaled down to a few atoms in thickness, quantum mechanical effects have made gate leakage problematic as well. With supplies at 1 V, there is limited room for further power scaling: we are stuck between a rock and a hot place.


On February 5, 2001, Intel Vice President Patrick Gelsinger gave a keynote speech at the International Solid State Circuits Conference[Gelsinger01]. He showed that microprocessor power consumption has been increasing exponentially (see Figure 5.33) and was forecast to grow even faster in the coming decade.


He predicted that “business as usual will not work in the future,” and that if scaling continued at this pace, by 2005, high-speed processors would have the power density of a nuclear reactor, by 2010, a rocket nozzle, and by 2015, the surface of the sun! Obviously,business did not proceed as usual and power consumption has leveled out at under 150 W for high-performance processors and much lower for battery-powered systems.


Clock gating was the ﬁrst widely applied technique for power reduction because it is relatively straightforward. Power gating was initially applied to low-power batteryoperated systems to increase the standby lifetime, but is now required for leakage control even in high-performance microprocessors [Rusu10]. Voltage domains are also widely used. Initially, separate supplies were provided for the core and I/O to provide compatibility with legacy I/O standards. The next step was to separate the supplies for the memories from the core logic. Memories arrays often use a constant relatively high supply voltage (as high as the process allows) for reliability. Logic dissipates the bulk of the dynamic power,so it operates at a lower, possibly variable voltage. Sometimes phase-locked loops or sensitive analog circuitry use yet another ﬁltered domain. Dynamic voltage scaling is commonly used to support a range of power/performance trade-offs [Clark01]. For example, laptop processors commonly run at a higher voltage when the system is plugged into wall power.


Body bias has been used for leakage control in applications such as the Intel XScale microprocessor [Clark02], the Transmeta Efﬁceon microprocessor, and a Toshiba MPEG4 video codec [Takahashi98]. Clustered voltage scaling was also used in the video codec. Both of these techniques introduce overhead routing the bias or voltage lines through a block and controlling noise on these lines. They have not achieved the widespread popularity of other techniques, and the effectiveness of body bias becomes limited below 130 nm because the body effect coefﬁcient decreases along with oxide thickness.


The move to CMOS technology was really the last major movement in mass-market semiconductor technologies. To date, no one has come up with better devices. The hundreds of billions of dollars that have been invested in optimizing CMOS make it a formidable technology to surpass. Rather than looking for a replacement, our best hope is to continue learning to use energy as efﬁciently as we can.


8085


286


386


486


P6


Hot Plate Nuclear Reactor Rocket Nozzle


Sun’s Surface


Pentium® proc


100 1000 10000


1990 Year


FIGURE 5.33  Microprocessor power density trends as predicted in 2001 (Reprinted with permission of Intel Corporation.)


Summary 209


The power consumption of a circuit has both dynamic and static components. The dynamic power comes from charging and discharging the load capacitances and depends on the frequency, voltage, capacitance, and activity factor. The static power comes from leakage and from circuits that have an intentional path from VDD to GND. CMOS circuits have historically consumed relatively low power because complementary CMOS gates dissipate almost zero static power when operated at high Vt . However, leakage is increasing as feature size decreases, making static power consumption as great a concern as dynamic power. The best way to control power is to turn off a circuit when it is not in use.


The most important techniques are clock gating, which turns off the clock when a unit is idle, and power gating, which turns off the power supply when a unit is in sleep mode.


5.1 You are synthesizing a chip composed of random logic with an average activity factor of 0.1. You are using a standard cell process with an average switching capacitance of 450 pF/mm2. Estimate the dynamic power consumption of your chip if it  has an area of 70 mm2 and runs at 450 MHz at VDD = 0.9 V.


5.2 You are considering lowering VDD to try to save power in a static CMOS gate. You  will also scale Vt  proportionally to maintain performance. Will dynamic power consumption go up or down? Will static power consumption go up or down?


5.3 The stack effect causes the current through two series OFF transistors to be an order  of magnitude less than Ioff when DIBL is signiﬁcant. Show that the current is Ioff/2 when DIBL is insigniﬁcant (e.g.,  = 0). Assume = 0, n = 1.


5.4 Determine the activity factor for the signal shown in Figure 5.34. The clock rate is 1  GHz.


FIGURE 5.34  Signal for Exercise 5.4


0 1 2 3 4 5 6 7 8 9 10


t (ns)


5.5 Consider the buffer design problem from Example 4.14. If the delay constraint is 20 , how many stages will give the lowest energy, and how should the stages be sized?


5.6 Repeat Exercise 5.5 if the load is 500 rather than 64 and the delay constraint is 30 .


5.7 Derive the switching probabilities in Table 5.1.


5.8 Design an 8-input OR gate with a delay of under 4 FO4 inverters. Each input may  present at most 1 unit of capacitance. The load capacitance is 16 units. If the input  probabilities are 0.5, compute the switching probability at each node and size the


circuit for minimum switching energy.


5.9 Construct a table similar to Table 5.2 for a 2-input NOR gate.


SOLUTION: The sheet resistance is


(6.4)


The total resistance is


(6.5)


The resistivity of polysilicon, diffusion, and wells is signiﬁcantly inﬂuenced by the doping levels. Polysilicon and diffusion typically have sheet resistances under 10 /square when silicided and up to several hundred /square when unsilicided. Wells have lower doping and thus even higher sheet resistance. These numbers are highly processdependent. Large resistors are often made from wells or


unsilicided polysilicon.


Contacts and vias also have a resistance, which is


dependent on the contacted materials and size of the contact. Typical values are 2–20 . Multiple contacts should


be used to form low-resistance connections, as shown in


Figure 6.8. When current turns at a right angle or reverses,


a square array of contacts is generally required, while fewer


contacts can be used when the ﬂow is in the same direction.


6.2.2 Capacitance


An isolated wire over the substrate can be modeled as a conductor over a ground plane. The wire capacitance has two major components: the parallel plate capacitance of the bottom of the wire to ground and the fringing capacitance arising from fringing ﬁelds along the edge of a conductor with ﬁnite thickness. In addition, a wire adjacent to a second wire on the same layer can exhibit capacitance to that neighbor. These effects are illustrated in Figure 6.9. The classic parallel plate capacitance formula is


(6.6)


Note that oxides are often doped with phosphorous to trap ions before they damage transistors; this oxide has ox k 0, with k = 4.1 as compared to 3.9 for an ideal oxide or lower for low-k dielectrics.


The fringing capacitance is more complicated to compute and requires a numerical ﬁeld solver for exact results. A number of authors have proposed approximations to this calculation [Barke88, Ruehli73, Yuan82]. One intuitively R =


2 2 10 0 22 10


m m


R = ( )


1000 0 125


Chwl= ox


FIGURE 6.8  Multiple vias for low-resistance connections


t h


w s


FIGURE 6.9 Effect of fringing ﬁelds on capacitance


Chapter 6      Interconnect


216


appealing approximation treats a lone conductor above a ground plane as a rectangular middle section with two hemispherical end caps, as shown in Figure 6.10[Yuan82]. The total capacitance is assumed to be the sum of a parallel plate capacitor of width w – t/2 and a cylindrical capacitor of radius t/2. This results in an expression for the capacitance that is accurate within 10% for aspect ratios less than 2 and t h.


(6.7)


An empirical formula that is computationally efﬁcient and relatively accurate is[Meijs84, Barke88]


(6.8)


which is good to 6% for aspect ratios less than 3.3.


These formulae do not account for neighbors on the same layer or higher layers. Capacitance interactions between layers can become quite complex in modern multilayer CMOS processes. A conservative upper bound on capacitance can be obtained assuming parallel neighbors on the same layer at minimum spacing and that the layers above and below the conductor of interest are solid ground planes. Similarly, a lower bound can be obtained assuming there are no other conductors in the system except the substrate. The upper bound can be used for propagation delay and power estimation while the lower bound can be used for contamination delay calculations before layout information is available.


A cross-section of the model used for capacitance upper bound calculations is shown in Figure 6.11. The total capacitance of the conductor of interest is the sum of its capacitance to the layer above, the layer below, and the two adjacent conductors. If the layers above and below are not switching,2 they can be modeled as ground planes and this component of capacitance is called Cgnd. Wires do have some capacitance to further neighbors, but this capacitance is generally negligible because most electric ﬁelds terminate on the nearest conductors. The dielectrics used between adjacent wires have the lowest possible dielectric constant khoriz to minimize capacitance. The dielectric between layers must provide greater mechanical stability and may have a larger kvert. EQ (6.9) gives a simple and physically intuitive estimate of wire capacitance [Bohr95]. The constant Cfringe term accounts for fringing capacitance and gives a better ﬁt for w and s up to several times minimum [Ho01].


(6.9)


2Or at least consist of a large number of orthogonal conductors that on average cancel each other’s switching activities.


wt


h t


lwh


w h


0 77 1 06


1 06


0 25


l kwhkts


total top bot adj


vert


horiz


+Cfringe


Parallel Plate Half Cylinders


FIGURE 6.10 Yuan & Trick  capacitance model including  fringing ﬁelds


6.2      Interconnect Modeling 217


The capacitances can be computed by generating a lookup table of


data with a ﬁeld solver such as FastCap [Nabors92] or HSPICE. The


table may contain data for different widths and spacings for each metal


layer, assuming the layers above and below are occupied or unoccupied.


The table should list both Cadj and Cgnd, because coupling to adjacent


lines is of great importance. Figure 6.12 shows representative data for a


metal2 wire in a 180 nm process with wire and oxide thicknesses of 0.7


m. The width and spacing are given in multiples of the 0.32 m minimum. For an isolated wire above the substrate, the capacitance is


strongly inﬂuenced by spacing between conductors. For a wire sandwiched between metal1 and metal3 planes, the capacitance is higher


and is more sensitive to the width (determining parallel plate capacitance) but less sensitive to spacing once the spacing is signiﬁcantly greater than the wire thickness. In either case, the y-intercept is greater than zero so doubling the width of a wire results in less than double the total capacitance. The data ﬁts EQ (6.9) with Cfringe =


0.05 fF/ m. Tight-pitch metal lines have a capacitance of roughly 0.2 fF/ m.


In practice, the layers above and below the conductor of interest are neither solid planes nor totally empty. One can extract capacitance more accurately by interpolating between these two extremes based on the density of metal on each level. [Chern92] gives formulae for this interpolation accurate to within 10%. However, if the wiring above and below is fairly dense (e.g., a bus on minimum pitch), it is well-approximated as a plane.


Dense wire ﬁll is added to many chips for mechanical stability and etch uniformity, making this approximation even more appropriate.


500


1000 1500 2000 w (nm)


Isolated


M1, M3 planes


s = 320 s = 480 s = 640 s =


350


300


FIGURE 6.12  Capacitance of metal2 line as a function of width and spacing


Layer n


Ctop


Layer n + 1


Layer n − 1


h2


h1


CbotCadj w


FIGURE 6.11  Multilayer capacitance model


218


6.2.3 Inductance


Most design tools consider only interconnect resistance and capacitance. Inductance is dif-ﬁcult to extract and model, so engineers prefer to design in such a way that inductive effects are negligible. Nevertheless, inductance needs to be considered in high-speed designs for wide wires such as clocks and power busses.


Although we generally discuss current ﬂowing from a gate output to charge or discharge a load capacitance, current really ﬂows in loops. The return path for a current loop is usually the power or ground network; at the frequencies of interest, the power supply is an “AC ground” because the bypass capacitance forms a low-impedance path between VDD and GND. Currents ﬂowing around a loop generate a magnetic ﬁeld proportional to the area of the loop and the amount of current. Changing the current requires supplying energy to change the magnetic ﬁeld. This means that changing currents induce a voltage proportional to the rate of change. The constant of proportionality is called the inductance, L.3


(6.10)


Inductance and capacitance also set the speed of light in a medium. Even if the resistance of a wire is zero leading to zero RC delay, the speed of light ﬂight-time along a wire of length with inductance and capacitance per unit length of L and C is


(6.11)


If the current return paths are the same as the conductors on which electric ﬁeld lines terminate, the signal velocity v is


(6.12)


where 0 is the magnetic permeability of free space (4  ×  10–7 H/m) and c is the speed of light in free space (3 × 108 m/s). In other words, signals travel about half the speed of light. Using low-k (< 3.9) dielectrics raises this velocity. However, many signals have electric ﬁelds terminating on nearby neighbors, but currents returning in more distant power supply lines. This raises the inductance and reduces the signal velocity.


Changing magnetic ﬁelds in turn produce currents in other loops. Hence, signals on one wire can inductively couple onto another; this is called inductive crosstalk.


The inductance of a conductor of length l and width w located a height h above a ground plane is approximately


(6.13)


assuming w < h and thickness is negligible. Typical on-chip inductance values are in the range of 0.15–1.5 pH/ m depending on the proximity of the power or ground lines.


(Wires near their return path have smaller current loops and lower inductance.)


3L is used to indicate both inductance and transistor channel length. The meaning should be clear from context.


V LdIdt=


t l LCpd =


= = =1 1


3 9


L l


h w


6.2      Interconnect Modeling 219


Extracting inductance in general is a three-dimensional problem and is extremely time-consuming for complex geometries. Inductance depends on the entire loop and therefore cannot be simply decomposed into sections as with capacitance. It is therefore impractical to extract the inductance from a chip layout. Instead, usually inductance is extracted using tools such as FastHenry [Kamon94] for simple test structures intended to capture the worst cases on the chip. This extraction is only possible when the power supply network is highly regular. Power planes are ideal but require a large amount of metal resources. Dense power grids are usually the preferred alternative. Gaps in the power grid force current to ﬂow around the gap, increasing the loop area and greatly increasing inductance. Moreover, large loops couple magnetic ﬁelds through other loops formed by conductors at a distance. Therefore, mutual inductive coupling can occur over a long distance,especially when the return path is far from the conductor.


6.2.4 Skin Effect


Current ﬂows along the path of lowest impedance Z = R + j L. At high frequency, ,impedance becomes dominated by inductance. The inductance is minimized if the currentﬂows only near the surface of the conductor closest to the return path(s). This skin effect can reduce the effective cross-sectional area of thick conductors and raise the effective resistance at high frequency. The skin depth for a conductor is


(6.14)


where  is the magnetic permeability of the dielectric (normally the same as in free space,4 × 10–7 H/m). The frequency of importance is the highest frequency with signiﬁcant power in the Fourier transform of the signal. This is not the chip operating frequency, but rather is associated with the faster edges. A sine wave with the same 20–80% rise/fall time as the signal has a period of 8.65trf . Therefore, the frequency associated with the edge can be approximated as


(6.15)


where trf  is the average 20–80% rise/fall time.


In a chip with a good power grid, good current return paths are usually available on all sides. Thus, it is a reasonable approximation to assume the current ﬂows in a shell of thickness  along the four sides of the conductor, as shown in Figure 6.13. If min(w, t) >2 , part of the conductor carries no current and the resistance increases.


Example 6.2


Determine the skin depth for a copper wire in a chip with 20 ps edge rates.


SOLUTION: According to EQ (6.15), the maximum frequency of interest is


(6.16)


=28 65. trf


×=


8 65 20


3 6 10


5 8


rad/s GHz


FIGURE 6.13  Current ﬂow  in shell determined by skin  depth


220


According to EQ (6.14), the skin depth is thus


(6.17)


This exceeds half the thickness of typical metal layers, so the skin effect is rarely a factor in CMOS circuits.


6.2.5 Temperature Dependence


Interconnect capacitance is independent of temperature, but the resistance varies strongly.


The temperature coefﬁcients of copper and aluminum are about 0.4%/°C over the normal operating range of circuits; that is, a 100 °C increase in temperature leads to 40% higher resistance. At liquid nitrogen temperature (77 K), the resistivity of copper drops to 0.22


· cm, an order-of-magnitude improvement. This suggests great advantages for RCdominated paths in cooled systems.


6.3 Interconnect Impact


Using the lumped models, this section examines the delay, energy, and noise impact of wires.


6.3.1 Delay


Interconnect increases circuit delay for two reasons. First, the wire capacitance adds loading to each gate. Second, long wires have signiﬁcant resistance that contributes distributed RC delay or ﬂight time. It is straightforward to add wire capacitance to the Elmore delay calculations of Section 4.3.5, so in this section we focus on the RC delay.


The Elmore delay of a single-segment L-model is RC. As the number of segments of the L-model increases, the Elmore delay decreases toward RC/2. The Elmore delay of a


- or T-model is RC/2 no matter how many segments are used. Thus, a single-segment-model is a good approximation for hand calculations.


Example 6.3


A 10x unit-sized inverter drives a 2x inverter at the end of the 1 mm wire from Example 6.1. Suppose that wire capacitance is 0.2 fF/ m and that unit-sized nMOS transistor has R = 10 k  and C = 0.1 fF. Estimate the propagation delay using the Elmore delay model; neglect diffusion capacitance.


SOLUTION: The driver has a resistance of 1 k .The receiver has a 2-unit nMOS transistor and a 4-unit pMOS transistor, for a capacitance of 0.6 fF. The wire capacitance is 200 fF.


Figure 6.14 shows an equivalent circuit for the system using a single-segment-model. The Elmore delay is tpd = (1000 )(100 fF) + (1000 + 800 )(100 fF +


0.6 fF) = 281 ps. The capacitance of the long wire dominates the delay; the capacitance of the 2x inverter is negligible in comparison.


)=


2 2 2 10 3 6 10


4 10


rad/s


H/m


0 99. m


6.3      Interconnect Impact 221


Because both wire resistance and wire capacitance increase with length,wire delay grows quadratically with length. Using thicker and wider wires,lower-resistance metals such as copper, and lower-dielectric constant insulators helps, but long wires nevertheless often have unacceptable delay. Section


6.4.2 describes how repeaters can be used to break a long wire into multiple segments such that the overall delay becomes a linear function of length.


Example 6.4


Find the RC ﬂight time per mm2 for a wire using the parameters from Example 6.3.


Express the result in FO4/mm2, if the FO4 inverter delay is 15 ps. What is the ﬂight time to cross a 10 mm die?


SOLUTION: R = 800 /mm. C = 0.2 pF/mm. The ﬂight time is RC/2 = 80 ps/mm2, or


5.3 FO4/mm2. The ﬂight time across a 10 mm die is thus 530 FO4, which is dozens of clock cycles.


Polysilicon and diffusion wires (sometimes called runners) have high resistance, even if silicided. Diffusion also has very high capacitance. Do not use diffusion for routing. Use polysilicon sparingly, usually in latches and ﬂip-ﬂops (i.e., do not use for other than intracell routing).


Recall that the Elmore delay model only considers the resistance on the path from the driver to a leaf. Capacitances on other branches are lumped as if they were at the branch point. This gives a conservative result because they are really partially shielded by their resistances.


Example 6.5


Figure 6.15 models a gate driving wires to two destinations. The gate is represented as a voltage source with effective resistance R1. The two receivers are located at nodes 3 and 4. The wire to node 3 is long enough that it is represented with a pair of-segments, while the wire to node 4 is represented with a single segment. Find the Elmore delay from input x to each receiver.


SOLUTION: The Elmore delays are


(6.18)


R C R R C R R R C R C


R C R


= + +( ) + + +( ) += + C C


R R C


( ) + +( )


800 Ω


100 f F 100 f F


Driver


Wire


0.6 f F


1000 Ω


FIGURE 6.14  Equivalent circuit for example


FIGURE 6.15  Interconnect modeling with RC tree


Node 4


Node 3


Long Wire Medium Wire


R4


R2


C1 C2


C3


R3


222


6.3.2 Energy


The switching energy of a wire is set by its capacitance. Long wires have signiﬁcant capacitance and thus require substantial amounts of energy to switch.


Example 6.6


Estimate the energy per unit length to send a bit of information (one rising and one falling transition) in a CMOS process.


SOLUTION: E = (0.2 pF/mm) (1.0 V)2 = 0.2 pJ/bit/mm. Sometimes energy in a communication link is expressed as power per gigabit per second: 0.2 mW/Gbps.


Example 6.7


Consider a microprocessor on a 20 mm × 20 mm die running at 3 GHz in the 65 nm process. A layer of metal is routed on a 250 nm pitch. Half of the available wire tracks are used. The wires have an average activity factor of 0.1. Determine the power consumed by the layer of metal.


SOLUTION: There are (20 mm) / (250 nm) = 80,000 tracks of metal across the die, of which 40,000 are occupied. The wire capacitance is (0.2 pF/mm)(20 mm)(40,000 tracks) = 160 nF. The power is (0.1)(160 nF)(1.0 V)2(3 GHz) = 48 W. This is clearly a problem, especially considering that the chip has more than one layer of metal. The activity factor needs to be much lower to keep power under control.


210


5.10 Design a header switch for a power gating circuit in a 65 nm process. Suppose the  pMOS transistor has an ON resistance of about 2.5 k · m. The block being gated  has an ON current of 100 mA. How wide must the header transistor be to cause less  than a 2% increase in delay?


211


Interconnect


6.1 Introduction


The wires linking transistors together are called interconnect and play a major role in the performance of modern systems. In the early days of VLSI, transistors were relatively slow.


Wires were wide and thick and thus had low resistance. Under those circumstances, wires could be treated as ideal equipotential nodes with lumped capacitance. In modern VLSI processes, transistors switch much faster. Meanwhile, wires have become narrower, driving up their resistance to the point, that in many signal paths, the wire RC delay exceeds gate delay. Moreover, the wires are packed very closely together and thus a large fraction of their capacitance is to their neighbors. When one wire switches, it tends to affect its neighbor through capacitive coupling; this effect is called crosstalk. Wires also account for a large portion of the switching energy of a chip. On-chip interconnect inductance had been negligible but is now becoming a factor for systems with fast edge rates and closely packed busses. Considering all of these factors, circuit design is now as much about engineering the wires as the transistors that sit underneath.


The remainder of this section deﬁnes the dimensions used to describe interconnect and gives a practical example of wire stacks in nanometer processes. Section 6.2 explores how to model the resistance, capacitance, and inductance of wires. Section 6.3 examines the impact of wires on delay, energy, and noise. Section 6.4 considers the tools at a designer’s disposal for improving performance and controlling noise. Section 6.5 extends the method of Logical Effort to give insights about designing paths with interconnect.


6.1.1  Wire Geometry


Figure 6.1 shows a pair of adjacent wires. The wires have width w, length l,


thickness t, and spacing of s from their neighbors and have a dielectric of


height h between them and the conducting layer below. The sum of width and


spacing is called the wire pitch. The thickness to width ratio t/w is called the


aspect ratio.


Early CMOS processes had a single metal layer and until the early 1990s


only two or three layers were available, but with advances in chemicalmechanical polishing it became far more practical to manufacture many metal


layers. As discussed in Section 3.4.2, aluminum (Al) wires used in older processes gave way to copper (Cu) around the 180 or 130 nm node to reduce resistance. Soon after, manufacturers began replacing the SiO2 insulator between wires with a succession of materials with lower dielectric constants (low-k) to reduce capacitance. A 65 nm process typically


FIGURE 6.1  Interconnect geometry


212


has 8–10 metal layers and the layer count has been increasing at a rate of about one layer every process generation or two.


6.1.2 Example: Intel Metal Stacks


Figure 6.2 shows cross-sections of the metal stacks in the Intel 90 and 45 nm processes,shown to scale [Thompson02, Moon08]. The 90 nm process has six metal layers, while the 45 nm process shows the bottom eight metal layers. The transistors are tiny gizmos beneath the vast labyrinth of wire. Metal1 is on the tightest pitch, roughly that of a contacted transistor, to provide dense routing within cells. The upper levels are progressively thicker and on a greater pitch to offer lower-resistance interconnections over progressively longer distances. The wires have a maximum aspect ratio of about 1.8.


M1 M2 M3


M3 M1


M6


M5


M4


M2 M4 M5 M6 M7 M8


1 m


FIGURE 6.2 SEM image of wire cross-sections in Intel’s (a) 90 nm and (b) 45 nm processes ((a) From [Thompson02] © 2002  IEEE. (b) From [Moon08] with permission of Intel Corporation.)


The top-level metal is usually used for power and clock distribution because it has the lowest resistance. Intel’s 45 nm process introduced an unusual extra-thick ninth Cu metal layer used to distribute power to different power-gated domains across the die (see Section 5.3.2). Figure 6.3 shows a full cross-section including this MT9 layer, a Cu bump for connecting to the power or ground network in the package (see Section 13.2.2), and a VA9 via between MT9 and the bump. The lower levels of metal and transistors are scarcely visible beneath these fat top layers. Table 6.1 lists the thickness and minimum pitch for each metal layer.


FIGURE 6.3  SEM image of complete cross-section of  Intel’s 45 nm process including M9 and I/O bump


(From [Moon08] with permission of Intel Corporation.)


6.2      Interconnect Modeling 213


6.2 Interconnect Modeling


A pipe makes a good mechanical analogy for a wire, as shown in Figure 6.4 [Ho07]. The resistance relates to the wire’s cross-sectional area. A narrow pipe impedes the ﬂow of current. The capacitance relates to a trough underneath the leaky pipe that must ﬁll up before current passes out the end of the pipe. And the inductance relates to a paddle wheel along the wire with inertia that opposes changes in the rate of ﬂow. Each of these elements is discussed further in this section.


A wire is a distributed circuit with a resistance and capacitance per unit length. Its behavior can be approximated with a number of lumped elements. Three standard approximations are the L-model, -model, and T-model, so-named because of their shapes. Figure 6.5 shows how a distributed RC circuit is equivalent to N distributed RC segments of proportionally smaller resistance and capacitance, and how these segments can be modeled with lumped elements. As the number of segments approaches inﬁnity, the lumped approximation will converge with the true distributed circuit. The L-model is a poor choice because a large number of segments are required for accurate results. The -model is much better; three segments are sufﬁcient to give results accurate to 3% [Sakurai83]. The T-model is comparable to the -model, but produces a circuit with one more node that is slower to solve by hand or with a circuit simulator. Therefore, it is common practice to model long wires with a 3–5 segment -model for simulation. If inductance is considered, it is placed in series with each resistor. The remainder of this section considers how to compute the resistance, capacitance, and inductance.


TABLE 6.1  Intel 45 nm metal stack Layer


t (nm)


w (nm)


s (nm)


pitch (nm)


M9


7 m


17.5 m


13 m


30.5 m


M8


410


810


M7


504


280


560


324


180


360


252


240


M3


M2


M1


Pipe: Resistance


Trough: Capacitance


Water Wheel: Inductance


FIGURE 6.4  Pipe analogy for wire


C/2 C/2


L-model


-model


T-model N Segments


R/2 R/2


C/N C/N


C/N


R/N R/N


FIGURE 6.5  Lumped approximation to distributed RC circuit


214


6.2.1 Resistance


The resistance of a uniform slab of conducting material can be expressed as


(6.1)


where  is the resistivity.1 This expression can be rewritten as


(6.2)


where R = /t is the sheet resistance and has units of /square. Note that a square is a dimensionless quantity corresponding to a slab of equal length and width. This is convenient because resistivity and thickness are characteristics of the process outside the control of the circuit designer and can be abstracted away into the single sheet resistance parameter.


To obtain the resistance of a conductor on a layer, multiply the sheet resistance by the ratio of length to width of the conductor. For example,the resistances of the two shapes in Figure 6.6 are equal because the length-to-width ratio is the same even though the sizes are different.


Nonrectangular shapes can be decomposed into simpler regions for which the resistance is calculated [Horowitz83].


Table 6.2 shows bulk electrical resistivities of pure metals at room temperature [Bakoglu90]. The resistivity of thin metal ﬁlms used in wires tends to be higher because of scattering off the surfaces and grain boundaries, e.g., 2.2–2.6  · cm for Cu and 3.6–4.0  · cm for Al [Kapur02].


As shown in Figure 6.7, copper must be surrounded by a lower-conductivity diffusion barrier that effectively reduces the wire cross-sectional area and hence raises the resistance.


Moreover, the polishing step can cause dishing that thins the metal. Even a 10 nm barrier is quite signiﬁcant when the wire width is only tens of nanometers. If the average barrier thickness is tbarrier and the height is reduced by tdish, the resistance becomes


(6.3)


1  is used to indicate both resistivity and best stage effort. The meaning should be clear from context.


TABLE 6.2  Bulk resistivity of pure metals at 22 °C Metal


Resistivity (mW · cm)


Silver (Ag)


Copper (Cu)


1.7


Gold (Au)


Aluminum (Al)


Tungsten (W)


5.3


Molybdenum (Mo)


Titanium (Ti)


43.0


Rtlw=R Rlw=


l w t


) (


dish barrier


barrier


1 Block


R = R (l /w)


4 Blocks


R = R (2l /2w)= R (l /w)


w w


FIGURE 6.6


Two conductors with equal resistance


tbarrier


tdish


Cu


FIGURE 6.7  Copper barrier  layer and dishing


6.2      Interconnect Modeling 215


Example 6.1


Compute the sheet resistance of a 0.22 m thick Cu wire in a 65 nm process. Find the total resistance if the wire is 0.125 m wide and 1 mm long. Ignore the barrier layer and dishing.


6.3.3 Crosstalk


As reviewed in Figure 6.16, wires have capacitance to their adjacent neighbors as well as to ground. When wire A switches, it tends to bring its neighbor B along with it on account of capacitive coupling, also called crosstalk. If B is supposed to switch simultaneously, this may increase or decrease the switching delay. If B is not supposed to switch, crosstalk causes noise on B. We will see that the impact of crosstalk depends on the ratio of Cadj to the total capacitance. Note that the load capacitance is included in the total, so for short wires and large loads, the load capacitance dominates and crosstalk is unimportant. Conversely, crosstalk is very important for long wires.


6.3.3.1 Crosstalk Delay Effects  If both a wire and its neighbor are switching, the direction of the switching affects the amount of charge that must be delivered and the delay of the switching. Table 6.3 summarizes this effect. The charge delivered to the coupling capacitor is Q = Cadj V, where V is the change in voltage between A and B. If A switches but B does not, V = VDD. The total capacitance effectively seen by A is just the capacitance to ground and to B. If both A and B switch in the same direction, V = 0. Hence, no charge is required and Cadj is effectively absent for delay purposes. If A and B switch in the opposite direction, V = 2VDD. Twice as much charge is required. Equivalently, the capacitor can be treated as being effectively twice as large switching through VDD. This is analogous to the Miller effect discussed in Section 4.4.6.6. The Miller Coupling Factor (MCF)describes how the capacitance to adjacent wires is multiplied to ﬁnd the effective capacitance. Some designers use MCF = 1.5 as a statistical compromise when estimating propagation delays before layout information is available.


Cgnd


CgndCadj


FIGURE 6.16  Capacitances  to adjacent neighbor and to  ground


6.3      Interconnect Impact 223


A conservative design methodology assumes neighbors are switching when computing propagation and contamination delays (MCF = 2 and 0, respectively). This leads to a wide variation in the delay of wires. A more aggressive methodology tracks the time window during which each signal can switch. Thus, switching neighbors must be accounted for only if the potential switching windows overlap. Similarly, the direction of switching can be considered. For example, dynamic gates described in Section 9.2.4 precharge high and then fall low during evaluation. Thus, a dynamic bus will never see opposite switching during evaluation.


Example 6.8


Each wire in a pair of 1 mm lines has capacitance of 0.08 fF/ m to ground and 0.12 fF/


m to its neighbor. Each line is driven by an inverter with a 1 k  effective resistance.


Estimate the contamination and propagation delays of the path. Neglect parasitic capacitance of the inverter and resistance of the wires.


SOLUTION: We ﬁnd Cgnd = (0.08 fF/ m)(1000 m) = 80 fF and Cadj = 120 fF. The delay is RCeff. The contamination delay is the minimum possible delay, which occurs when both wires switch in the same direction. In that case, Ceff = Cgnd and the delay is tcd =(1 k )(0.08 pF) = 80 ps. The propagation delay is the maximum possible delay, which occurs when both wires switch in opposite directions. In this case, Ceff = Cgnd + 2Cadj and the delay is tpd = (1 k )(0.32 pF) = 320 ps. This is a factor of four difference between best and worst case.


6.3.3.2 Crosstalk Noise Effects  Suppose wire A switches while B is


supposed to remain constant. This introduces noise as B partially


switches. We call A the aggressor or perpetrator and B the victim. If the


victim is ﬂoating, we can model the circuit as a capacitive voltage


divider to compute the victim noise, as shown in Figure 6.17.


Vaggressor is normally VDD.


(6.19)


If the victim is actively driven, the driver will supply current to oppose and reduce the victim noise. We model the drivers as resistors,as shown in Figure 6.18. The peak noise becomes dependent on the time constant ratio k of the aggressor to the victim [Ho01]:


(6.20)


TABLE 6.3  Dependence of effective capacitance on switching direction


DV


Ceff(A)


MCF


Constant


VDD Cgnd + Cadj 1


Switching same direction as A


Switching opposite to A


2VDD Cgnd + 2Cadj 2


victim


adj


gnd adj


aggressor


=+


kV


=+ +11


Cadj


Cgnd-v


Aggressor


Victim


ΔVaggressor


ΔVvictim


Raggressor


Rvictim


Cgnd-a


FIGURE 6.17 Coupling to ﬂoating victim


FIGURE 6.18  Coupling to driven victim


224


(6.21)


Figure 6.19 shows simulations of coupling when the aggressor is driven with a unit inverter; the victim is undriven or driven with an inverter of half, equal, or twice the size of the aggressor; and Cadj = Cgnd. Observe that when the victim is ﬂoating, the noise remains indeﬁnitely. When the victim is driven, the driver restores the victim. Larger (faster) drivers oppose the coupling sooner and result in noise that is a smaller percentage of the supply voltage. Note that during the noise event the victim transistor is in its linear region while the aggressor is in saturation. For equal-sized drivers, this means Raggressor is two to four times Rvictim, with greater ratios arising from more velocity saturation [Ho01]. In general, EQ (6.20) is conservative, especially when wire resistance is included [Vittal99].


It is often used to ﬂag nets where coupling can be a problem; then simulations can be performed to calculate the exact coupling noise. Coupling noise is of greatest importance on weakly driven nodes where k < 1.


We have only considered the case of a single neighbor switching. When both neighbors switch, the noise will be twice as great. We have also modeled the layers above and below as AC ground planes, but wires on these layers are likely to be switching. For a long line, you can expect about as many lines switching up and switching down, giving no net contribution to delay or noise. However, a short line running over a 64-bit bus in which all 64 bits are simultaneously switching from 0 to 1 will be strongly inﬂuenced by this switching.


6.3.4 Inductive Effects


Inductance has always been important for integrated circuit packages where the physical dimensions are large, as will be discussed in Section 13.2.3. On-chip inductance is important for wires where the speed-of-light ﬂight time is longer than either the rise times of the circuits or the RC delay of the wire. Because speed-of-light ﬂight time increases link


aggressor gnd adj


victim gnd adj


v +


Victim (Undriven): 50%


Victim (Half-Size Driver): 16%


Victim (Equal-Size Driver): 8%


Victim (Double-Size Driver): 4%


80 120 160 200 240 280 320 360


FIGURE 6.19  Waveforms of coupling noise


6.3      Interconnect Impact 225


early according to EQ (6.11) and RC delay increases quadratically with length, we can estimate the set of wire lengths for which inductance is relevant [Ismail99].


(6.22)


Example 6.9


Consider a metal2 signal line with a sheet resistance of 0.10 /  and a width of 0.125 m. The capacitance is 0.2 fF/ m and inductance is 0.5 pH/ m. Compute the velocity of signals on the line and plot the range of lengths over which inductance matters as a function of the rise time.


SOLUTION: The velocity is


(6.23)


Note that this is 100 mm/ns or 1 mm/10 ps. The resistance is (0.1 / )(1 /0.125 m)= 0.8 / m. Figure 6.20 plots the length of wires for which inductance is relevant against rise times. Above the horizontal line, wires greater than 125 m are limited by RC delay rather than LC delay. To the right of the diagonal line, rise times are greater than the LC delay. Only in the region between these lines is inductance relevant to delay calculations. This region has very fast edge rates, so inductance is not very important to the delay of highly resistive signal lines.


As the example illustrated, inductance will only be important to


the delay of low-resistance signals such as wide clock lines. Inductive crosstalk is also important for wide busses far away from their


current return paths. In power distribution networks, inductance


means that if one portion of the chip requires a rapidly increasing


amount of current, that charge must be delivered from nearby


decoupling capacitors or supply pins; portions of the chip further


away are unaware of the changing current needs until a speed-oflight ﬂight time has elapsed and hence will not supply current


immediately. Adding inductance to the power grid simulation generally reveals greater supply noise than would otherwise be predicted. Power networks will be discussed further in Section 13.3.


In wide, thick, upper-level metal lines, resistance and RC delay


may be small. This pushes the horizontal line in Figure 6.20


upward, increasing the range of edge rates for which inductance


matters. This is especially common for clock signals. Inductance


tends to increase the propagation delay and sharpen the edge rate.


To see the effects of inductance, consider a 5 mm-long clock line


above a ground plane driving a 2 pF clock load. If its width is 4.8 m


and thickness is 1.7 m, it has resistance of 4 /mm, capacitance of


0.4 pF/mm, and inductance of 0.12 nH/mm. Figure 6.21 presents models of the clock line as a 5-stage -model without (a) and with (b) inductance. Figure 6.21(c) shows the


lRLC


< <


= =(


)(


)= =


0 2


pH/ m fF/ m


m/s


100 ps


10 ps


1 ps


0.1 ps


Wire Length


10 m


100 m


1mm  10mm


Inductance


Matters


RC Delay


Dominates


Rise Time


Rise Time and


RC Dominate


FIGURE 6.20  Wire lengths and edge rates for which  inductance impacts delay


226


response of each model to an ideal voltage source with 80 ps rise time. The model including inductance shows a greater delay until the clock begins to rise because of the speed-oflight ﬂight time. It also overshoots. However, the rising edge is sharper and the rise time is shorter. In some circumstances when the driver impedance is matched to the characteristic impedance of the wire, the sharper rising edge can actually result in a shorter propagation delay measured at the 50% point.


To reduce the inductance and the impact of skin effect when no ground plane is available, it is good practice to split wide wires into thinner sections interdigitated with power and ground lines to serve as return paths. For example, Figure 6.22 shows how a 16 mwide clock line can be split into four 4 m lines to reduce the inductance.


0.2 pF


0.4 pF


4 Ω


2 pF 2 pF RC


RLC


RC


0.12 nH


FIGURE 6.21 Wide clock line modeled with and without inductance


16 m


4 m


FIGURE 6.22  Wide clock line interdigitated with power  and ground lines to reduce inductance


6.3      Interconnect Impact 227


A bus made of closely spaced wires far above


a ground plane is particularly susceptible to


crosstalk. Figure 6.23 shows the worst case


crosstalk scenario. The victim line is in the center. The two adjacent neighbors rise, capacitively


coupling the victim upward. The other bus wires


fall. Each one creates a loop of current ﬂowing


counterclockwise through the wire and back


along the ground plane. These loops induce a


magnetic ﬁeld, which in turn induces a current


ﬂowing in the other direction in the victim line.


This is called mutual inductive coupling and also


makes the victim rise. The noise from each


aggressor sums on to the victim in much the same way that multiple primary turns in a transformer couple onto a single secondary turn. Computing the inductive crosstalk requires extracting a mutual inductance matrix for the bus and simulating the system. As this is not yet practical for large chips, designers instead either follow design rules that keep the inductive effects small or ignore inductance and hope for the best. The design rules may be of the form that one power or ground wire must be inserted between every N signal lines on each layer. N is called the signal:return (SR) ratio [Morton99]. The returns give an alternative path for current to ﬂow, reducing the mutual inductance. The inductive effects on noise and delay are generally small for N = 8 and negligible for N = 4 when normal wiring pitches are used [Linderman04]. N = 2 means each signal is shielded on one side, also eliminating half the capacitive crosstalk. However, low SR ratios are expensive in terms of metal resources.


In summary, on-chip inductance is difﬁcult to extract. Mutual inductive coupling may occur over a long range, so inductive coupling is difﬁcult to simulate even if accurate values are extracted. Instead, design rules are usually constructed so that inductive effects may be neglected for most structures. The easiest way to do this is to provide a regular power grid in which power and ground are systematically allocated track to keep the SR ratio low.


Inductance should be incorporated into simulations of the power and clock networks and into the noise and delay calculations for busses with large SR ratios in high-speed designs.


6.3.5 An Aside on Effective Resistance and Elmore Delay


Recall from Section 4.3.4 that a factor of ln 2 was lumped into the effective resistance of a transistor so that the Elmore delay model predicts propagation delay, yet we have not accounted for the factor in wire resistance. This section examines the discrepancy.


According to the Elmore delay model, a gate with effective resistance R and capacitance C has a propagation delay of RC. A wire with distributed resistance R and capacitance C treated as a single -segment has propagation delay RC/2. Reviewing the properties of RC circuits, we recall that the lumped RC circuit in Figure 6.24(a) has a unit step response of


(6.24)


The propagation delay of this circuit is obtained by solving for tpd when Vout(tpd) = 1/2:


(6.25)


t R'C


out e( ) = 1


pd = =ln .2 0 69


Current Loops


Magnetic Field


Mutual Inductive Coupling


FIGURE 6.23  Inductive and capacitive crosstalk in a bus


228


The distributed RC circuit in Figure 6.24(b) has no closed form time domain response. Because the capacitance is distributed along the circuit rather than all being at the end, you would expect the capacitance to be charged on average through about half the resistance and that the propagation delay should thus be about half as great. A numerical analysis ﬁnds that the propagation delay is 0.38R C.


To reconcile the Elmore model with the true results for a logic gate, recall that logic gates have complex nonlinear I-V characteristics and are approximated as having an effective resistance. If we characterize that effective resistance as R = R ln 2, the propagation delay really becomes the product of the effective resistance and the capacitance: tpd = RC.


For distributed circuits, observe that


Therefore, the Elmore delay model describes distributed delay well if we use an effective wire resistance scaled by ln 2 from that computed with EQ (6.2). This is somewhat inconvenient. The effective resistance is further complicated by the effect of nonzero rise time on propagation delay. Figure 6.25 shows that the propagation delay depends on the rise time of the input and approaches RC for lumped systems and RC/2 for distributed systems when the input is a slow ramp. This suggests that when the input is slow, the effective resistance for delay calculations in a distributed RC circuit is equal to the true resistance.


Finally, we note that for many analyses such as repeater insertion calculations in Section


6.4.2, the results are only weakly sensitive to wire resistance, so using the true wire resistance does not introduce great error.


In summary, it is a reasonable practice to estimate the ﬂight time along a wire as RC/2 where R is the true resistance of the wire. When more accurate results are needed, it is important to use good transistor models and appropriate input slopes in simulation.


The Elmore delay can be viewed in terms of the ﬁrst moment of the impulse response of the circuit. CAD tools can obtain greater accuracy by approximating delay based on higher moments using a technique called moment matching. Asymptotic Waveform Evaluation (AWE) uses moment matching to estimate interconnect delay with better accuracy than the Elmore delay model and faster run times than a full circuit simulation [Celik02].


0 38


ln =


R C R C


FIGURE 6.24  Lumped and distributed RC circuit response


R'C


Vin(t)


Vout(t)


Lumped Distributed


6.4      Interconnect Engineering 229


6.4 Interconnect Engineering


As gate delays continue to improve while long wire delays remain constant or even get slower, wire engineering has become a major part of integrated circuit design. It is necessary to develop a ﬂoorplan early in the design cycle, identify the long wires, and plan for them. While ﬂoorplanning in such a way that critical communicating units are close to one another has the greatest impact on performance, it is inevitable that long wires will still exist. Aspect ratios in old processes were below 1, but are close to 2 in nanometer processes to help the resistance of such narrow lines. This comes at the expense of substantially increased coupling capacitance. The designer has a number of techniques to engineer wires for delay and coupling noise. The width, spacing, and layer usage are all under the designer’s control. Shielding can be used to further reduce coupling on critical nets.


Repeaters inserted along long wires reduce the delay from a quadratic to a linear function of length. Wire capacitance and resistance complicate the use of Logical Effort in selecting gate sizes.


6.4.1 Width, Spacing, and Layer


The designer selects the wire width, spacing, and layer usage to trade off delay, bandwidth,energy, and noise. By default, minimum pitch wires are preferred for noncritical interconFIGURE 6.25  Effect of rise time on lumped and distributed RC circuit delays


0.5 1 0


trise RC


tpd RC


V(t) Input


Distributed Lumped


0.38


230


nections for best density and bandwidth. When the load is dominated by wire capacitance,the best way to reduce delay is to increase spacing, reducing the capacitance to nearby neighbors. This also reduces energy and coupling noise. When the delay is dominated by the gate capacitance and wire resistance, widening the wire reduces resistance and delay.


However, it increases the capacitance of the top and bottom plates. Widening wires also increases the fraction of capacitance of the top and bottom plates, which somewhat reduces coupling noise from adjacent wires. However, wider wires consume more energy. The wire thickness depends on the choice of metal layer. The lower layers are thin and optimized for a tight routing pitch. Middle layers are often slightly thicker for lower resistance and better current-handling capability. Upper layers may be even thicker to provide a low-resistance power grid and fast global interconnect. Wiring tracks are a precious resource and are often allocated in the ﬂoorplan; the wise designer maintains a reserve of wiring tracks for unanticipated changes late in the design process.


The power grid is usually distributed over multiple layers. Most of the currenthandling capability is provided in the upper two layers with lowest resistance. However,the grid must extend down to metal1 or metal2 to provide easy connection to cells.


6.4.2 Repeaters


Both resistance and capacitance increase with wire length l, so the RC delay of a wire increases with l 2 , as shown in Figure 6.26(a). The delay may be reduced by splitting the wire into N segments and inserting an inverter or buffer called a repeater to actively drive the wire [Glasser85], as shown in Figure 6.26(b). The new wire involves N segments with RC ﬂight time of (l/N )2 , for a total delay of l 2/N. If the number of segments is proportional to the length, the overall delay increases only linearly with l.


Using inverters as repeaters gives best performance. Each repeater adds some delay. If the distance is too great between repeaters, the delay will be dominated by the long wires. If the distance is too small, the delay will be dominated by the large number of inverters. As usual, the best distance between repeaters is a compromise between these extremes. Suppose a unit inverter has resistance R, gate capacitance C,4 and diffusion capacitance Cpinv. A wire has resistance Rw and capacitance Cw per unit length. Consider inserting repeaters of W times unit size.


4Note that C now refers to the capacitance of an entire inverter, not a single transistor, so = RC.


Wire Length: l


Receiver


l /N


Segment


Repeater


N Segments


FIGURE 6.26  Wire with and without repeaters


W CWpinv


RwlN


Cw


Cw 2


CW


FIGURE 6.27  Equivalent circuit for  segment of repeated wire


6.4      Interconnect Engineering 231


Figure 6.27 shows a model of one segment. The Elmore delay of the repeated wire is


(6.26)


Differentiating EQ (6.26) with respect to N and W shows that the best length of wire between repeaters is (see Exercise 6.5)


(6.27)


Recall from Example 4.10 that the delay of an FO4 inverter is 5RC. Assuming pinv  0.5 using folded transistors, EQ (6.27) simpliﬁes to


(6.28)


The delay per unit length of a properly repeated wire is


(6.29)


To achieve this delay, the inverters should use an nMOS transistor width of


(6.30)


The energy per unit length to send a bit depends on the wire and repeater capacitances


(6.31)


In other words, repeaters sized for minimum delay add 87% to the energy of an unrepeated wire.


Example 6.10


Compute the delay per mm of a repeated wire in a 65 nm process. Assume the wire is on a middle routing layer and has 2x width, spacing, and height, so its resistance is 200/mm and capacitance is 0.2 pF/mm. The FO4 inverter delay is 15 ps. Also ﬁnd the repeater spacing and driver size to achieve this delay and the energy per bit.


SOLUTION: Using EQ (6.29), the delay is


(6.32)


This delay is achieved using a spacing of 0.45 mm between repeaters and an nMOS driver width of 18 m (180x unit size). The energy per bit is 0.4 pJ/mm.


NRWClNCW


RlNC lNCW


+ +( ) +


l N


p R Cw w


R Cw w


= 0 77.FO4


RCR C


= + +( )( )2 2 1


1 67


FO4


RC R C


lC NWC


pV


= + +( ) = ++1 112


1 87


t pd = ( )(


1 67 15 200


41


ps /mm pF/mm ps/mm


232


As one might expect, the curve of delay vs. distance and driver size is relatively ﬂat near the minimum. Thus, substantial energy can be saved for a small increase in delay. At the minimum EDP point, the segments become 1.7x longer and the drivers are only 0.6x as large. The delay increases by 14% but the repeaters only add 30% to the energy of the unrepeated line [Ho01]. For the parameters in Example 6.10, the minimum EDP can be found numerically at a spacing of about 0.8 mm and a driver width of 11 m (110x unit size), achieving an energy of 0.26 pJ/mm at a delay of 47 ps/mm. These longer segments are more susceptible to noise.


Unfortunately, inverting repeaters complicate design because you must either ensure an even number of repeaters on each wire or adapt the receiving logic to accept an inverted input. Some designers use inverter pairs (buffers) rather than single inverters to avoid the polarity problem. The pairs contribute more delay. However, the ﬁrst inverter size W1 may be smaller, presenting less load on the wire driving it. The second inverter may be larger,driving the next wire more strongly. You can show that the best size of the second inverter is W2 = kW1, where k = 2.25 if pinv = 0.5. The distance between repeaters increases to (see Exercise 6.6)


(6.33)


The delay per unit length becomes


(6.34)


using transistor widths of


(6.35)


and the energy per bit per unit length is


(6.36)


This typically means that wires driven with noninverting repeaters are only about 8%slower per unit length than those using inverting repeaters. Only about two-thirds as many repeaters are required, simplifying ﬂoorplanning. Total repeater area and power increases slightly.


The overall delay is a weak function of the distance between repeaters, so it is reasonable to increase this distance to reduce the difﬁculty of ﬁnding places in the ﬂoorplan for repeaters while only slightly increasing delay. Repeaters impose directionality on a wire.


Bidirectional busses and distributed tristate busses cannot use simple repeaters and hence are slower; this favors point-to-point unidirectional communications.


6.4.3 Crosstalk Control


Recall from EQ (6.20) that the capacitive crosstalk is proportional to the ratio of coupling capacitance to total capacitance. For modern wires with an aspect ratio (t/w) of 2 or l


RC kkp R C


1 22


= 1 81. FO4


WW k


W W k


E l


C Vw DD


6.4      Interconnect Engineering 233


greater, the coupling capacitance can account for 2/3 to 3/4 of the total capacitance and crosstalk can create large amounts of noise and huge data-dependent delay variations.


There are several approaches to controlling this crosstalk:


Increase spacing to adjacent lines


Shield wires


Ensure neighbors switch at different times


Crosstalk cancellation


The easiest approach to ﬁx a minor crosstalk problem is to increase the spacing. If the crosstalk is severe, the spacing may have to be increased by more than one full track. In such a case, it is more efﬁcient to shield critical signals with power or ground wires on one or both sides to eliminate coupling. For example, clock wires are usually shielded so that switching neighbors do not affect the delay of the clock wire and introduce clock jitter.


Sensitive analog wires passing near digital signals should also be shielded.


An alternative to shielding is to interleave busses that are guaranteed to switch at different times. For example, if bus A switches on the rising edge of the clock and bus B switches on the falling edge of the clock, by interleaving the bits of the two busses you can guarantee that both neighbors are constant during a switching event. This avoids the delay impact of coupling; however, you must still ensure that coupling noise does not exceed noise budgets. Figure 6.28 shows wires shielded (a) on one side, (b) on both sides, and (c)interleaved. Critical signals such as clocks or analog voltages can be shielded above and below as well.


Alternatively, wires can be arranged to cancel the effects of crosstalk. Three such methods include staggered repeaters, charge compensation, and twisted differential signaling[Ho03b]. Each technique seeks to cause equal amounts of positive and negative crosstalk on the victim, effectively producing zero net crosstalk.


Figure 6.29(a) shows two wires with staggered repeaters. Each segment of the victim sees half of a rising aggressor segment and half of a falling aggressor segment. Although the cancellation is not perfect because of delays along the segments, staggering is a very effective approach. Figure 6.29(b) shows charge compensation in which an inverter and transistor are added between the aggressor and victim. The transistor is connected to behave as a capacitor. When the aggressor rises and couples the victim upward, the inverter falls and couples the victim downward. By choosing an appropriately sized compensation transistor, most of the noise can be canceled at the expense of the extra circuitry.


Figure 6.29(c) shows twisted differential signaling in which each signal is routed differentially. The signals are swapped or twisted such that the victim and its complement each see equal coupling from the aggressor and its complement. This approach is expensive in wiring resources, but it effectively eliminates crosstalk. It is widely used in memory designs that are naturally differential, as explored in Section 12.2.3.3.


vdd a0


a1


gnd


a2


vdd


b0 a1


a2 b2


vdd a0 a1 gnd a2 a3 vdd(a)


a0


b1


FIGURE 6.28  Wire shielding topologies


234


6.4.4 Low-Swing Signaling


Driving long wires is slow because of the RC delay, and expensive in power because of the large capacitance to switch. Low-swing signaling improves performance by sensing when a wire has swung through some small Vswing rather than waiting for a full swing. If the driver is turned off after the output has swung sufﬁciently, the power can be reduced as well. However, the improvements come at the expense of more complicated driver and receiver circuits. Low-swing signaling may also require a twisted differential pair of wires to eliminate common-mode noise that could corrupt the small signal.


The power consumption for low-swing signaling depends on both the driver voltage Vdrive and the actual voltage swing Vswing. Each time the wire is charged and discharged, it consumes Q = CVswing. If the effective switching frequency of the wire is f, the average current is


In addition to working at the standard process corners, chips must function in a very high temperature, high voltage burn-in corner (e.g., 125 to 140 °C externally, corresponding to an even higher internal temperature, and 1.3–1.7× nominal VDD [Vollertsen99])during test. While it does not have to run at full speed, it must operate correctly so that all nodes can toggle. The burn-in corner has very high leakage and can dictate the size of keepers and weak feedback on domino gates and static latches.


Processes with multiple threshold voltages and/or multiple oxide thicknesses can see each ﬂavor of transistor independently varying as fast, typical, or slow. This can easily lead to more corners than anyone would care to simulate and raises challenges about identifying what corners must be checked for different types of circuits.


7.3 Reliability


Designing reliable CMOS chips involves understanding and addressing the potential failure modes [Segura04]. This section addresses reliability problems (hard errors) that cause integrated circuits to fail permanently, including the following:


Oxide wearout


Interconnect wearout


Overvoltage failure


Latchup


This section also considers transient failures (soft errors) triggered by radiation that cause the system to crash or lose data. Circuit pitfalls and common design errors are discussed in Section 9.3.


7.3.1 Reliability Terminology


A failure is a deviation from compliance with the system speciﬁcation for a given period of time. Failures are caused by faults, which are deﬁned as failures of subsystems. Faults have many causes, ranging from design bugs to manufacturing defects to wearout to external disturbances to intentional abuse of a product. Not all faults lead to errors; some are masked. For example, a bug in the multiprocessor interface logic does not cause an error in a single-processor system. A defective via may go unnoticed if it is in parallel with a good one. Studying the underlying faults gives insight into predicting and improving the failure rate of the overall system.


7.3      Reliability 247


A number of acronyms are commonly used in describing reliability [Tobias95].


MTBF is the mean time between failures: (number of devices × hours of operation) / number of failures. FIT is the failures in time, the number of failures that would occur every thousand hours per million devices, or equivalently, 109 × (failure rate/hour). 1000 FIT is one failure in 106 hours = 114 years. This is good for a single chip. However, if a system contains 100 chips each rated at 1000 FIT and a customer purchases 10 systems, the failure rate is 100 × 1000 × 10 = 106 FIT, or one failure every 1000 hours (42 days). Reliability targets of less than 100 FIT are desirable.


Most systems exhibit the bathtub curve shown in Figure 7.6. Soon after birth, systems with weak or marginal components tend to fail. This period is called infant mortality. Reliable systems then enter their useful operating life, in which the failure rate is low. Finally, the failure rate increases at the end of life as the system wears


out. It is important to age systems past infant mortality


before shipping the products. Aging is accelerated by


stressing the part through burn-in at higher than normal


voltage and temperature, as discussed in Section 7.2.4.


Engineers typically desire product lifetimes exceeding 10 years, but it is clearly impossible to test a product


for 10 years before selling it. Fortunately, most wearout


mechanisms have been observed to display an exponential relationship with voltage or temperature. Thus,


systems are subjected to accelerated life testing during


burn-in conditions to simulate the aging process and


evaluate the time to wearout. The results are extrapolated to normal operating conditions to judge the actual


useful operating life. For example, Figure 7.7 shows the


measured lifetime of gate oxides in an IBM 32 nm process at elevated voltages [Arnaud08]. The extrapolated


results show a lifetime exceeding 10 years at 10% above


the nominal 0.9 V VDD.


Life testing is time-consuming and comes right at


the end of the project when pressures to get to market


are greatest. Part of any high-volume chip design will


necessarily include designing a reliability assessment


program that consists of burn-in boards deliberately


stressing a number of chips over an extended period.


Designers have tried to develop reliability simulators to


predict lifetime [Hu92, Hsu92], but physical testing


remains important. For high-volume parts, the source of


failures is tracked and common points of failure can be


redesigned and rolled into manufacturing.


7.3.2 Oxide Wearout


As gate oxides are subjected to stress, they gradually wear out, causing the threshold voltage to shift and the gate leakage to increase. Eventually, the circuit fails because transistors become too slow, mismatches become too large, or leakage currents become too great.


Processes generally specify a maximum operating voltage to ensure oxide wearout effects


Time


Infant


Mortality


Useful


Operating Life


Wearout


FIGURE 7.6  Reliability bathtub curve


FIGURE 7.7 Accelerated life testing of gate oxides in IBM 32 nm  process (© IEEE 2008.)


Chapter 7      Robustness


248


are limited during the lifetime of a chip. The primary mechanisms for oxide wearout include the following:


Hot carriers


Negative bias temperature instability (NBTI)


Time-dependent dielectric breakdown (TDDB)


7.3.2.1 Hot Carriers   As transistors switch, high-energy (“hot”) carriers are occasionally injected into the gate oxide and become trapped there. Electrons have higher mobility and account for most of the hot carriers. The damaged oxide changes the  I-V characteristics of the device, reducing current in nMOS transistors and increasing current in pMOS transistors. Damage is maximized when the substrate current Isub is large, which typically occurs when nMOS transistors see a large Vds while ON. Therefore, the problem is worst for inverters and NOR gates with fast rising inputs and heavily loaded outputs [Sakurai86],and for high power supply voltages.


Hot carriers cause circuit wearout as nMOS transistors become too slow. They can also cause failures of sense ampliﬁers and other matched circuits if matched components degrade differently [Huh98]. Hot electron degradation can be analyzed with simulators[Hu92, Hsu91, Quader94]. The wear is limited by setting maximum values on input rise time and stage electrical effort [Leblebici96]. These maximum values depend on the process and operating voltage.


7.3.2.2 Negative Bias Temperature Instability    When an electric ﬁeld is applied across a gate oxide, dangling bonds called traps develop at the Si-SiO2 interface. The threshold voltage increases as more traps form, reducing the drive current until the circuit fails[Doyle91, Reddy02]. The process is most pronounced for pMOS transistors with a strong negative bias (i.e., a gate voltage of 0 and source voltage of VDD) at elevated temperature. It has become the most important oxide wearout mechanism for many nanometer processes.


When a ﬁeld Eox = VDD/tox is applied for time t, the threshold voltage shift can be modeled as [Paul07]:


(7.1)


The high stress during burn-in can lock in most of the threshold voltage shift expected from NBTI; this is good because it allows testing with full NBTI degradation.


During design, a chip should be simulated under the worst-case NBTI shift expected over its lifetime.


7.3.2.3 Time-Dependent Dielectric Breakdown   As an electric ﬁeld is applied across the gate oxide, the gate current gradually increases. This phenomenon is called time-dependent dielectric breakdown (TDDB) and the elevated gate current is called stress-induced leakage current (SILC). The exact physical mechanisms are not fully understood, but TDDB likely results from a combination of charge injection, bulk trap state generation, and trap-assisted conduction [Hicks08]. After sufﬁcient stress, it can result in catastrophic dielectric breakdown that short-circuits the gate.


The failure rate is exponentially dependent on the temperature and oxide thickness[Monsieur01]; for a 10-year life at 125 °C, the ﬁeld across the gate Eox = VDD/tox should be kept below about 0.7 V/nm [Moazzami90]. Nanometer processes operate close to this limit. The problem is greatest when voltage overshoots occur; this can be caused by noisy V k tt


0 0 25.


7.3      Reliability 249


power supplies or reﬂections at I/O pads. Reliability is improved by lowering the power supply voltage, minimizing power supply noise, and using thicker oxides on the I/O pads.


7.3.3 Interconnect Wearout


High currents ﬂowing through wires eventually can damage the wires. For wires carrying unidirectional (DC) currents, electromigration is the main failure mode. For wires carrying bidirectional (AC) currents, self-heating is the primary concern.


7.3.3.1 Electromigration   High current densities lead to an “electron wind”


that causes metal atoms to migrate over time. Such electromigration causes


wearout of metal interconnect through the formation of voids [Hu95]. Figure


7.8 shows a scanning electron micrograph of electromigration failure of a via


between M2 and M3 layers [Christiansen06]. Remarkable videos taken under a


scanning electron microscope show void formation and migration and wire failure [Meier99]. The problem is especially severe for aluminum wires; it is commonly alleviated with an Al-Cu or Al-Si alloy and is much less important for


pure copper wires because of the different grain transport properties. The electromigration properties also depend on the grain structure of the metal ﬁlm.


Electromigration depends on the current density J = I/wt. It is more


likely to occur for wires carrying a DC current where the electron wind blows


in a constant direction than for those with bidirectional currents [Liew90].


Electromigration current limits are usually expressed as a maximum Jdc. The


mean time to failure (MTTF) also is highly sensitive to operating temperature as given by Black’s Equation [Black69]:


(7.2)


Ea is the activation energy that can be experimentally determined by stress testing at high temperatures and n is typically 2. The electromigration DC current limits vary with materials, processing, and desired MTTF and should be obtained from the fabrication vendor.


In the absence of better information, a maximum Jdc of 1–2 mA/ m2 is a conservative limit for aluminum wires at 110 °C [Rzepka98]. Copper is less susceptible to electromigration and may endure current densities of 10 mA/ m2 or better [Young00]. Current density may be more limited in contact cuts.


Considering the dynamic switching power, we can estimate the maximum switching capacitance that a wire can drive. The current is Idc = P/V = CVf. Thus, for a wire limited to Idc–max, the switching capacitance should be less than


(7.3)


7.3.3.2 Self-Heating   While bidirectional wires are less prone to electromigration, their current density is still limited by self-heating. High currents dissipate power in the wire.


Because the surrounding oxide or low-k dielectric is a thermal insulator, the wire temperature can become signiﬁcantly greater than the underlying substrate. Hot wires exhibit greater resistance and delay. Electromigration is also highly sensitive to temperature, so self-heating may cause temperature-induced electromigration problems in the bidirectional wires. Brief


MTTFe


E kT


dc


V f


FIGURE 7.8  Electromigration failure of  M2-M3 via (© IEEE 2006.)


pulses of high peak currents may even melt the interconnect. Self-heating is dependent on the root-mean-square (RMS) current density. This can be measured with a circuit simulator or calculated as


(7.4)


A conservative rule to control reliability problems with self-heating is to keep Jrms < 15 mA/ m2 for bidirectional aluminum wires on a silicon substrate[Rzepka98]. The maximum capacitance of the wire can be estimated based on the RMS current. If a signal has symmetric rising and falling edges, we only need to consider half of a period. Figure 7.9(a) shows a signal with a 20–80% rise time tr and an average period T = 1/ f. The switching current i(t) can be approximated as a triangular pulse of duration t = tr / (0.8–0.2), as shown in Figure


7.9(b). Then, the RMS current is


(7.5)


and, to avoid excessive self-heating, the wire and load capacitance should be less than


(7.6)


Example 7.1


A clock signal is routed on the top metal layer using a wire that is 1 m wide and has a self-heating limit of 10 mA. The wire has a capacitance of 0.4 fF/ m and the load capacitance is 85 fF. The clock switches at 3 GHz and has a 20 ps rise time. How far can the wire run between repeaters without overheating?


SOLUTION: A clock has an activity factor of 1. According to EQ (7.6), the maximum capacitance of the line is


(7.7)


Thus, the maximum wire length is (685 – 85 fF) / (0.4 fF/ m) = 1500 m.


I t dt T


rms


( )2


i t dt


1 0 5


2 0 5


0 0 5


1 26


.1 26


C =


( ) ××


1 26 1


1 3 10 20 10


685


9 12


Hz s


T/2


0 VDD


0.8 VDD


0.2 VDD


i(t)


2CVDD/Δt


Δt = tr/0.6


FIGURE 7.9  Switching waveforms  for RMS current estimation


7.3      Reliability 251


In summary, electromigration from high DC current densities is primarily a problem in power and ground lines. Self-heating limits the RMS current density in bidirectional signal lines. However, do not overlook the signiﬁcant unidirectional currents that ﬂow through the wires contacting nMOS and pMOS transistors. For example, Figure 7.10 shows which lines in an inverter are limited by DC and RMS currents. Both problems can be addressed by widening the lines or reducing the transistor sizes (and hence the current).


7.3.4 Soft Errors


In the 1970s, as dynamic RAMs (DRAMs) replaced core memories, DRAM vendors were puzzled to ﬁnd DRAM bits occasionally ﬂipping value spontaneously. At


ﬁrst, the errors were attributed to “system noise,” “voltage marginality,” “sense


ampliﬁers,” or “pattern sensitivity,” but the errors were found to be random. When


the corrupted bit was rewritten with a new value, it was no more likely than any


other bit to experience another error. In a classic paper [May79], Intel identiﬁed the


source of these soft errors as alpha particle collisions that generate electron-hole


pairs in the silicon as the particles lose energy. The excess carriers can be collected


into the diffusion terminals of transistors. If the charge collected is comparable to


the charge on the node, the voltage can be disturbed.


Soft errors are random nonrecurring errors triggered by


radiation striking a chip. Alpha particles, emitted by the decay


of trace uranium and thorium impurities in packaging materials, was once the dominant source of soft errors, but they have


been greatly reduced by using highly puriﬁed materials. Today,


high-energy (> 1 MeV ) neutrons from cosmic radiation


account for most soft errors in many systems [Baumann01,


Baumann05]. When a neutron strikes a silicon atom, it can


induce ﬁssion, shattering the atom into charged fragments that


continue traveling through the substrate. These ions leave a trail


of electron-hole pairs behind as they travel through the lattice.


Figure 7.11 shows the effect of an ion striking a reverse-biased


p-n junction [Baumann05]. The ion leaves a cylindrical trail of


electrons and holes in its wake, with a radius of less than a


micron. Within tens of picoseconds, the electric ﬁeld at the


junction collects the carriers into a funnel-shaped depletion region. Over the subsequent nanoseconds, electrons diffuse into the depletion region. Depending on the type of ion, its energy, its trajectory, and the geometry of the p-n junction, up to several hundred femtocoulombs of charge may be collected onto the junction.


The spike of current is called a single-event transient (SET). If the collected charge exceeds a critical amount, Qcrit, it may ﬂip the state of the node, causing a fault called a single-event upset (SEU). Failures caused by such faults are called soft errors. Qcrit depends on the capacitance and voltage of the node, and on any feedback devices that may ﬁght against the disturbance. This is a serious challenge because both capacitance and voltage have been decreasing as transistors shrink, reducing Qcrit. Fortunately, the amount of charge collected on a smaller junction also decreases, but the net trend has been toward higher soft error rates.


The holes generated by the particle strike ﬂow to a nearby substrate contact where they are collected. The current ﬂowing through the resistive substrate raises the potential of the substrate. This can turn on a parasitic bipolar transistor (see Section 7.3.6) between


Jdc


Jrms


FIGURE 7.10  Current density limits in an inverter


FIGURE 7.11  Generation and collection of carriers after a  radiation strike (© IEEE 2005.)


the source and drain of a nearby nMOS transistor, disturbing that transistor too[Osada04]. Such multinode disturbances can be controlled by using plenty of substrate and well contacts.


At sea level, SRAM generally experiences a soft error rate (SER) of 100–2000 FIT/Mb[Hazucha00, Normand96]. The neutron ﬂux from cosmic rays increases by two orders of magnitude at aircraft ﬂight altitudes [Ziegler96] and can cause up to 106 FIT/Mb at these levels. Depending on the process and layout, roughly 1% of the soft errors affect multiple nodes [Hazucha04].


Soft errors affect memories, registers, and combinational logic. Memories use error detecting and correcting codes to tolerate soft errors, so these errors rarely turn into failures in a well-designed system. Such codes will be discussed further in Sections 11.7.2 and


12.8.2. Soft errors in registers are becoming much more common as their charge storage diminishes. Radiation-hardening schemes for registers and memory are discussed in Sections 10.3.10 and 12.8.3.


In combinational logic, the collected charge causes a momentary glitch on the output of a gate. This glitch can propagate through downstream logic until it reaches a register.


The fault does not necessarily cause a failure. The masking mechanisms include the following: Logical masking : the SEU may not trigger a sensitized path through the logic. For  example, if both inputs to a NAND gate are 0, a SEU on one input does not affect  the output.


Temporal masking : The SEU may not reach a register at the time it is sampling.


Electrical masking : The SEU may be attenuated if it is faster than the bandwidth of  the gate.


In older technologies, larger gates had more charge, so they were less likely to experience upsets. Even if they did see an upset, it was likely to be attenuated by electrical masking. However, soft errors in combinational logic are a growing problem at 65 nm and below because the gates have less capacitance and higher speed [Mitra05, Rao07]. Section


7.6.2 discusses the use of redundancy to mitigate logic errors.


7.3.5 Overvoltage Failure


Tiny transistors can be easily damaged by relatively low voltages. Overvoltage may be triggered by excessive power supply transients or by electrostatic discharge (ESD) from static electricity entering the I/O pads, which can cause very large voltage and current transients(see Section 13.6.2).


Overvoltage at the gate node accelerates the oxide wearout. In extreme cases, it can cause breakdown and arcing across the thin dielectric, destroying the device. The DC oxide breakdown voltage scales with oxide thickness and absolute temperature and can be modeled as [Monsieur01]


(7.8)


with typical values of a = 1.5 V/nm, b = 533 V · K, and V0 close to 0. Breakdown occurs around 3 V under worst case (hot) conditions in a 65 nm process.


Higher-than-normal voltages applied between source and drain lead to punchthrough when the source/drain depletion regions touch [Tsividis99]. This can lead to abnormally high current ﬂow and ultimately self-destructive overheating.


at


TV


bd ox= + + 0


7.3      Reliability 253


Both problems lead to a maximum safe voltage that can be applied to transistors. Even when catastrophic failure is avoided, high voltage accelerates the wearout mechanisms. Thus,processes specify a Vmax for long-term reliable operation. For nanometer processes, this voltage is often much less than the I/O standard voltage, requiring a second type of transistor with thicker oxides and longer channels to endure the higher I/O voltages.


7.3.6 Latchup


Early adoption of CMOS processes was slowed by a curious tendency of CMOS chips to develop low-resistance paths between VDD and GND, causing catastrophic meltdown.


The phenomenon, called latchup, occurs when parasitic bipolar transistors formed by the substrate, well, and diffusion turn ON. With process advances and proper layout procedures, latchup problems can be easily avoided.


The cause of the latchup effect [Estreich82, Troutman86] can be understood by examining the process cross-section of a CMOS inverter, as shown in Figure 7.12(a), over which is laid an equivalent circuit. In addition to the expected nMOS and pMOS transistors, the schematic depicts a circuit composed of an npn-transistor, a pnp-transistor, and two resistors connected between the power and ground rails (Figure 7.12(b)). The npntransistor is formed between the grounded n-diffusion source of the nMOS transistor, the p-type substrate, and the n-well. The resistors are due to the resistance through the substrate or well to the nearest substrate and well taps. The cross-coupled transistors form a bistable silicon-controlled rectiﬁer (SCR). Ordinarily, both parasitic bipolar transistors are OFF. Latchup can be triggered when transient currents ﬂow through the substrate during normal chip power-up or when external voltages outside the normal operating range are applied. If substantial current ﬂows in the substrate, Vsub will rise, turning ON the npntransistor. This pulls current through the well resistor, bringing down Vwell and turning ON the pnp-transistor. The pnp-transistor current in turn raises Vsub, initiating a positive feedback loop with a large current ﬂowing between VDD and GND that persists until the power supply is turned off or the power wires melt.


Fortunately, latchup prevention is easily accomplished by minimizing Rsub and Rwell.


Some processes use a thin epitaxial layer of lightly doped silicon on top of a heavily doped


FIGURE 7.12  Origin and model of CMOS latchup


Rsub


Rwell


Vsub


Vwell


Vsub Rsub


254


substrate that offers a low substrate resistance. Most importantly, the designer should place substrate and well taps close to each transistor.


A conservative guideline is to place a tap adjacent to every source connected to VDD or GND. If this is not practical, you can obtain more detailed information from the process vendor (they will normally specify a maximum distance for diffusion to substrate/well tap)or try the following guidelines:


Every well should have at least one tap.


All substrate and well taps should connect directly to the


appropriate supply in metal.


A tap should be placed for every 5–10 transistors, or more  often in sparse areas.


nMOS transistors should be clustered together near GND  and pMOS transistors should be clustered together near VDD,avoiding convoluted structures that intertwine nMOS and  pMOS transistors in checkerboard patterns.


I/O pads are especially susceptible to latchup because external voltages can ring below GND or above VDD, forward biasing the junction between the drain and substrate or well and injecting current into the substrate. In such cases, guard rings should be used to collect the current, as shown in Figure 7.13. Guard rings are simply substrate or well taps tied to the proper supply that completely surround the transistor of concern. For example, the n+ diffusion in Figure 7.13(b) can inject electrons into the substrate if it falls a diode drop below 0 volts. The p+ guard ring tied to ground provides a lowresistance path to collect these electrons before they interfere with the operation of other circuits outside the guard ring. All diffusion structures in any circuit connected to the external world must be guard ringed; i.e., n+ diffusion by p+ connected to GND or p+ diffusion by n+ connected to VDD. For the ultra-paranoid, double guard rings may be employed; i.e., n+ ringed by p+ to GND, then n+ to VDD or p+ ringed by n+ to VDD, then p+ to GND.


SOI processes avoid latchup entirely because they have no parasitic bipolar structures.


Also, processes with VDD < 1.4–2 V are immune to latchup because the two parasitic transistors will never have a large enough voltage to sustain positive feedback [ Johnston96].


Therefore, latchup has receded to a minor concern in nanometer processes.


7.4 Scaling


The only constant in VLSI design is constant change. Figure 1.6 showed the unrelenting march of technology, in which feature size has reduced by 30% every two to three years.


As transistors become smaller, they switch faster, dissipate less power, and are cheaper to manufacture! Since 1995, as the technical challenges have become greater, the pace of innovation has actually accelerated because of ferocious competition across the industry.


Such scaling is unprecedented in the history of technology. However, scaling also exacerp+n-well


p+ Guard Ring


n+ Guard Ring


FIGURE 7.13  Guard rings


7.4      Scaling 255


bates reliability issues, increases complexity, and introduces new problems. Designers need to be able to predict the effect of this feature size scaling on chip performance to plan future products, ensure existing products will scale gracefully to future processes for cost reduction, and anticipate looming design challenges. This section examines how transistors and interconnect scale, and the implications of scaling for design. The Semiconductor Industry Association prepares and maintains an International Technology Roadmap for Semiconductors predicting future scaling. Section 7.8 gives a case study of how scaling has inﬂuenced Intel microprocessors over more than three decades.


(6.37)


Hence, the dynamic dissipation is


(6.38)


In contrast, a rail-to-rail driver uses Vdrive = Vswing = VDD and thus consumes power proportional to VDD2. Vswing must be less than or equal to Vdrive. By making Vswing less than Vdrive, we speed up the wire because we do not need to wait for a full swing. By making both voltages signiﬁcantly less than VDD, we can reduce the power by an order of magnitude.


Ti t


f CV


drive


swing


f CV V


dynamic avg drive


swing drive


FIGURE 6.29  Crosstalk control schemes


Coupled Noise


Cancels


Aggressor(a)


6.4      Interconnect Engineering 235


Low-swing signaling involves numerous challenges. A low Vdrive must be provided to the chip and distributed to low-swing drivers. The signal should be transmitted on differential pairs of wires that are twisted to cancel coupling from neighbors and equalized to prevent interference from the previous data transmitted. The driver must turn on long enough to produce Vswing at the far end of the line, then turn off to prevent unnecessary power dissipation. This generally leads to a somewhat larger swing at the near end of the line. The receiver must be clocked at the appropriate time to amplify the differential signal. Distributing a self-timed clock from driver to receiver is difﬁcult because the distances are long, so the time to transmit a full-swing clock exceeds the time for the data to complete its small swing.


Figure 6.30 shows a synchronous low-swing signaling technique using the system clock for both driver and receiver [Ho03a]. During the ﬁrst half of the cycle, the driver is OFF (high impedance) and the differential wires are equalized to the same voltage. During the second half of the cycle, the drivers turn ON. At the end of the cycle, the receiver senses the differential voltage and ampliﬁes it to full-swing levels. Figure 6.30(a) shows the overall system architecture. Figure 6.30(b) shows the driver for one of the wires. The gates use ordinary VDD while the drive transistors use Vdrive. Because Vdrive < VDD – Vt ,nMOS transistors are used for both the pullup and pulldown to deliver low effective resistance in their linear regime. A second driver using the complementary input drives the complementary wire. Figure 6.30(c) shows the differential wires with twisting and equalizing. The end of the wire only swings part-way, reducing power consumption. Using medium Vdrive and small Vswing is faster than using a smaller Vdrive and waiting for the wire to swing all the way. Figure 6.30(d) shows the clocked sense ampliﬁer based on the SA-F/F that will be described further in Section 10.3.8. The sense ampliﬁer uses pMOS input transistors because the small-swing inputs are close to GND and below the threshold of nMOS transistors. Note that the clock period must be long enough to transmit an adequate voltage swing. If the clock period increases, the circuit will actually dissipate more power because the voltage swing will increase to a maximum of Vdrive.


(a)a


LowSwing Driver


Sense Amplifier


Twisted, Equalized Differential Wires


a clk


Vdrive


d d


f f


SR Latch


Q y


FIGURE 6.30  Low-swing signaling system


236


6.4.5 Regenerators


Repeaters are placed in series with wires and thus are limited to unidirectional busses. An alternative is to use regenerators (also called boosters) placed in parallel with wires at periodic intervals, as shown in Figure 6.31. When the wire is initially ‘0,’ the regenerator senses a rising transition and accelerates it. Conversely, when the wire is initially ‘1,’ the regenerator accelerates the falling transition. Regenerators trade off up to 20% better delay or energy for reduced noise margins.


Regenerators generally use skewed gates to sense a transition. As discussed in Section


9.2.1.5, a HI-skew gate favors the rising output by using a low switching point, and a LOskew gate does the reverse. Figure 6.32 shows a self-timed regenerator [Dobbalaere95].


When the wire begins to rise, the LO-skewed NAND gate detects the transition midway and turns on the pMOS driver to assist. The normal-skew inverters eventually detect the transition and ﬂip node x, turning off the pMOS driver.


When the wire begins to fall, the HI-skewed NOR gate turns on the nMOS to assist. Other regenerator designs include [Nalamalpu02, Singh08].


6.5 Logical Effort with Wires


Interconnect complicates the application of Logical Effort because the wires have a ﬁxed capacitance. The branching effort at a wire with capacitance Cwire driving a gate load of Cgate is (Cgate + Cwire) / Cgate. This branching effort is not constant; it depends on the size of the gate being driven. The simple rule that circuits are fastest when all stages bear equal effort is no longer true when wire capacitance is introduced. If the wire is very short or very long, approximations are possible, but when the wire and gate loads are comparable, there is no simple method to determine the best stage effort.


Every circuit has some interconnect, but when the interconnect is short(Cwire << Cgate), it can be ignored. Alternatively, you can compute the average ratio of wire capacitance to parasitic diffusion capacitance and add this as extra parasitic capacitance when determining parasitic delay. For connections between nearby gates, this generally leads to a best stage effort  slightly greater than 4.


The path should use fewer stages because each stage contributes wire capacitance. To reduce delay, the gates should be sized larger so that the wire capacitance is a smaller fraction of the whole. However, this comes at the expense of increased energy.


Conversely, when the interconnect is long (Cwire >> Cgate), the gate at the end can be ignored. The path can now be partitioned into two parts. The ﬁrst part drives the wire while the second receives its input from the wire. The ﬁrst part is designed to drive the load capacitance of the wire; the extra load of the receiver is negligible. To save energy, theﬁnal stage driving the wire should have a low logical effort and a high electrical effort; an inverter is preferred [Stan99]. The size of the receiver is chosen by practical considerations: Larger receivers may be faster, but they also cost area and power. If the wire is long enough that the RC ﬂight time exceeds a few gate delays, it should be broken into segments driven by repeaters.


The most difﬁcult problems occur when Cwire Cgate. These medium-length wires introduce branching efforts that are a strong function of the size of the gates they drive.


Writing a delay equation as a function of the gate sizes along the path and the wire capacitance results in an expression that can be differentiated with respect to gate sizes to comLong Wire


Regenerator


FIGURE 6.31


Long Wire


n p


Rising Boost


Falling Boost


FIGURE 6.32  Regenerator


6.6      Pitfalls and Fallacies 237


pute the best sizes. Alternatively, a convex optimizer can be used to minimize delay or generate an energy-delay trade-off curve.


Figure 6.33 shows three stages along a path. By writing the Elmore delay and differentiating with respect to the size of the middle stage, we ﬁnd the interesting result that the delay caused by the capacitance of a stage should equal the delay caused by the resistance of the stage [Morgenshtein09]:


(6.39)


Example 6.11


The path in Figure 6.34 contains a medium-length wire modeled as a lumped capacitance. Write an equation for path delay in terms of x and y. How large should the x and y inverters be for shortest path delay? What is the stage effort of each stage?


C R


) = +( )+


Stage i − 1


Stage i + 1


Stage i


Ri − 1, Ci − 1


Ri + 1, Ci + 1


Ri, Ci


Rwi − 1, Cwi − 1


Rwi, Cwi


xi − 1


xi + 1


FIGURE 6.33  Path with wires


10 fF


50 fF 100 fF


FIGURE 6.34  Path with medium-length wire


SOLUTION: From the Logical Effort delay model, we ﬁnd the path delay is


(6.40)


Differentiating with respect to each size and setting the results to 0 allows us to solve EQ (6.41) for x = 33 fF and y = 57 fF.


(6.41)


The stage efforts are (33/10) = 3.3, (57 + 50)/33 = 3.2, and (100/57) = 1.8. Notice that the ﬁrst two stage efforts are equal as usual, but the third stage effort is lower. As x already drives a large wire capacitance, y may be rather large (and will bear a small stage effort) before the incremental increase in delay of x driving y equals the incremental decreases in delay of y driving the output.


6.6 Pitfalls and Fallacies


Designing a large chip without considering the floorplan


In the mid-1990s, designers became accustomed to synthesizing a chip from HDL and “tossing  the netlist over the wall” to the vendor who would place & route it and manufacture the chip. Many designers were shielded from considering the physical implementation. Now flight


dx yx


yP


= +++ +1050 100


1 10


10 500


1 1000


+= = +


x y


238


times across the chip are a large portion of the cycle time in slow systems and multiple cycles  in faster systems. If the chip is synthesized without a floorplan, some paths with long wires  will be discovered to be too slow after layout. This requires resynthesis with new timing constraints to shorten the wires. When the new layout is completed, the long wires simply show  up in different paths. The solution to this convergence problem is to make a floorplan early  and microarchitect around this floorplan, including budgets for wire flight time between


blocks. Algorithms termed timing directed placement have alleviated this problem, resulting in  place & route tools that converge in one or a few iterations.


Leaving gaps in the power grid


Current always flows in loops. Current flowing along a signal wire must return in the power/ground network. The area of the loop sets the inductance of the signal. A discontinuity in the  power grid can force return current to find a path far from the signal wire, greatly increasing  the inductance, which increases delay and noise. Because signal inductance is usually not


modeled, the delay and noise will not be discovered until after fabrication.


As feature size decreases, transistors get faster but wires do not. Interconnect delays are now very important. The delay is again estimated using the Elmore delay model based on the resistance and capacitance of the wire and its driver and load. The wire delay grows with the square of its length, so long wires are often broken into shorter segments driven by repeaters. Vast numbers of wires are required to connect all the transistors, so processes provide many layers of interconnect packed closely together. The capacitive coupling between these tightly packed wires can be a major source of noise in a system. These challenges are managed by using many metal layers of various thicknesses to provide high bandwidth for short thin wires and lower delay for longer fat wires. The microarchitecture becomes inherently linked to the ﬂoorplan because the design must allocate one or more cycles of pipeline delay for wires that cross the chip.


6.1 Estimate the resistance per mm of a minimum pitch Cu wire for each layer in the  Intel 45 nm process described in Table 6.1. Assume a 10 nm high-resistance barrier  layer and negligible dishing.


6.2 Consider a 5 mm-long, 4 -wide metal2 wire in a 0.6 m process. The sheet resistance is 0.08 /  and the capacitance is 0.2 fF/ m. Construct a 3-segment


-model for the wire.


6.3 A 10x unit-sized inverter drives a 2x inverter at the end of the 5 mm wire from


Exercise 6.2. The gate capacitance is C = 2 fF/ m and the effective resistance is


R = 2.5 k · m for nMOS transistors. Estimate the propagation delay using the  Elmore delay model; neglect diffusion capacitance.


6.4 Find the best width and spacing to minimize the RC delay of a metal2 bus in the  180 nm process described in Figure 6.12 if the pitch cannot exceed 960 nm. Minimum width and spacing are 320 nm. First, assume that neither adjacent bit is


switching. How does your answer change if the adjacent bits may be switching?


Exercises 239


6.5 Derive EQ (6.27)–(6.30). Assume the initial driver and ﬁnal receiver are of the same  size as the repeaters so the total delay is N times the delay of a segment.


6.6 Revisit Exercise 6.5 using a pair of inverters (a noninverting buffer) instead of a single inverter. The ﬁrst inverter in each pair is W1 times unit width. The second is a  factor of k larger than the ﬁrst. Derive EQ (6.33)–(6.36).


6.7 Compute the characteristic velocity (delay per mm) of a repeated metal2 wire in the  180 nm process. A unit nMOS transistor has resistance of 2.5 k  and capacitance of


0.7 fF, and the pMOS has twice the resistance. Use the data from Figure 6.12. Consider both minimum pitch and double-pitch (twice minimum width and spacing) wires. Assume solid metal above and below the wires and that the neighbors are not  switching.


6.8 Prove EQ (6.39).


241


Robustness


7.1 Introduction


A central challenge in building integrated circuits is to get millions or billions of transistors to all function, not just once, but for a quintillion consecutive cycles. Transistors are so small that printing errors below the wavelength of light and variations in the discrete number of dopant atoms have major effects on their performance. Over the course of their operating lives, chips may be subjected to temperatures ranging from freezing to boiling.


Intense electric ﬁelds gradually break down the gates. Unrelenting currents carry away the atoms of the wires like termites slowly devouring a mansion. Cosmic rays zap the bits stored in tiny memory cells.


Despite these daunting challenges, engineers routinely build robust integrated circuits with lifetimes exceeding ten years of continuous operation. Conventional static CMOS circuits are exceptionally well-suited to the task because they have great noise margins, are minimally sensitive to variations in transistor parameters, and will eventually recover even if a noise event occurs. Fairly simple guidelines on the maximum voltages and currents sufﬁce to ensure long operating life. Fault-tolerant and adaptive architectures can correct for errors and adjust the chip to run at its best despite manufacturing variations and changing operating conditions.


Section 7.2 begins by examining the sources of manufacturing and environmental variations and their effects on a chip. Section 7.3 then discusses reliability, including wearout, soft errors, and catastrophic failures. A good design should work well not only in the current manufacturing process, but also when ported to a more advanced process. Section 7.4 addresses scaling laws to predict how future processes will evolve. Section 7.5 revisits variability with a more mathematical treatment. Section 7.6 examines adaptive and faulttolerant design techniques to compensate for variations and transient errors.


7.2 Variability


So far, when considering the various aspects of determining a circuit’s behavior, we have only alluded to the variations that might occur in this behavior given different operating conditions. In general, there are three different sources of variation—two environmental and one manufacturing:


Process variation


Supply voltage


Operating temperature


242


The variation sources are also known as Process, Voltage, and Temperature (PVT). You must aim to design a circuit that will operate reliably operate over all extremes of these three variables. Failure to do so causes circuit problems, poor yield, and customer dissatisfaction.


Variations are usually modeled with uniform or normal (Gaussian)statistical distributions, as shown in Figure 7.1. Uniform distributions are speciﬁed with a half-range a. For good results, accept variations over the entire half-range. For example, a uniform distribution for VDD could be speciﬁed at 1.0 V ±10%. This distribution has a 100 mV halfrange. All parts should work at any voltage in the range. Normal distributions are speciﬁed with a standard deviation . Processing variations are usually modeled with normal distributions. Retaining parts with a 3  distribution will result in 0.26% of parts being rejected. A 2  retention results in 4.56% of parts being rejected, while 1  results in a


31.74% rejection rate. Obviously, rejecting parts outside 1  of nominal would waste a large number of parts. A 3  or 2  limit is conventional and a manufacturer with a commercially viable CMOS process should be able to supply a set of device parameters describing this range. For components such as memory cells that are replicated millions of times,a 0.26% failure rate is far too high. Such circuits must tolerate 5, 6, or even 7  of variation. Remember that if only the variations in one direction (e.g., too slow) matter, the reject rate is halved.


7.2.1 Supply Voltage


Systems are designed to operate at a nominal supply voltage, but this voltage may vary for many reasons including tolerances of the voltage regulator, IR drops along supply rails, and di/dt noise. The system designer may trade-off power supply noise against resources devoted to power supply regulation and distribution; typically the supply is speci-ﬁed at ±10% around nominal at each logic gate. The supply varies across the chip as well as in time. For example, Figure 7.2 shows a voltage map indicating the worst case droop as a function of position on a chip [Bernstein06, Su03].


Speed is roughly proportional to VDD, so to ﬁrst order this leads to±10% delay variations (check for your process and voltage when this is critical). Power supply variations also appear in noise budgets.


7.2.2 Temperature


Section 2.4.5 showed that as temperature increases, drain current decreases. The junction temperature of a transistor is the sum of the ambient temperature and the temperature rise caused by power dissipation in the package. This rise is determined by the power consumption and the package thermal resistance, as discussed in Section 13.2.4.


Table 7.1 lists the ambient temperature ranges for parts speciﬁed to commercial,industrial, and military standards. Parts must function at the bottom end of the ambient range unless they are allowed time to warm up before use. The junction temperature (the temperature at the semiconductor junctions forming the transistors) may signiﬁcantly exceed the maximum ambient temperature. Commonly commercial parts are veriﬁed to operate with junction temperatures up to 125 °C.


3 2 1 0 1 2 3 Accepting parts


within 1  would exclude 31.7%


1 All parts lie within


the half-range


Normal Distribution


Uniform Distribution


x a


FIGURE 7.1


Uniform and normal distributions


FIGURE 7.2  Voltage droop map (Courtesy of          International Business Corporation. Unauthorized  use not permitted.)


7.2      Variability 243


Temperature varies across a die depending on which portions dissipate the most power. The variation is gradual, so all circuits in a given 1 mm diameter see nearly the same temperature. Temperature varies in time on a scale of milliseconds. Figure 7.3 shows a simulated thermal map for the Itanium 2 microprocessor [Harris01b]. The execution core has hot spots exceeding 100 °C, while the caches in the periphery are below 70 °C.


7.2.3 Process Variation


Devices and interconnect have variations in ﬁlm thickness, lateral


dimensions, and doping concentrations [Bernstein99]. These variations


can be classiﬁed as inter-die (e.g., all the transistors on one die might be


shorter than normal because they were etched excessively) and intra-die


(e.g., one transistor might have a different threshold voltage than its


neighbor because of the random number of dopant atoms implanted).


For devices, the most important variations are channel length L and


threshold voltage Vt . Channel length variations are caused by photolithography proximity effects, deviations in the optics, and plasma etch


dependencies. Threshold voltages vary because of different doping concentrations and annealing effects, mobile charge in the gate oxide, and


discrete dopant variations caused by the small number of dopant atoms


in tiny transistors. Threshold voltages gradually change as transistors


wear out; such time-dependent variation will be examined in Section 7.3.


For interconnect, the most important variations are line width and


spacing, metal and dielectric thickness, and contact resistance. Line width and spacing, like channel length, depend on photolithography and etching proximity effects. Thickness may be inﬂuenced by polishing. Contact resistance depends on contact dimensions and the etch and clean steps.


Process variations can be classiﬁed as follows:


Lot-to-lot (L2L)


Wafer-to-wafer (W2W )


Die-to-die (D2D), inter-die, or within-wafer (WIW )


Within-die (WID) or intra-die


Wafers are processed in batches called lots. A lot processed after a furnace has been shut down and cleaned may behave slightly differently than the lot processed earlier. One wafer may be exposed to an ion implanter for a slightly different amount of time than another,causing W2W threshold voltage variation. A die near the edge of the wafer may etch slightly differently than a die in the center, causing D2D channel length variations. For example, Figure 7.4 plots the operating frequency of ring oscillators as a function of their position on the wafer, showing a 20% variation involving both a systematic radial component and a smaller random component. Unless calibrations are made on a per-lot or perwafer basis, L2L and W2W variations are often lumped into the D2D variations. D2D variations ultimately make one chip faster or slower than another. They can be handled by


TABLE 7.1  Ambient temperature ranges Standard


Maximum


Commercial


0 °C


70 °C


Industrial


–40 °C


85 °C


Military


–55 °C


125 °C


FIGURE 7.3  Thermal map of Itanium 2 (© IEEE 2001.)


244


providing enough margin to cover 2 or 3  of variation and by rejecting the small number of chips that fall outside this bound, as discussed in the next section.


WID variations were once small compared to D2D variations and were largely ignored by digital designers but have become quite important in nanometer processes.


Some WID variations are spatially correlated; these are called process tilt. For example, an ion implanter might deliver a greater dose near the center of a wafer than near the periphery, causing threshold voltages to tilt radially across the wafer. In summary, transistors on the same die match better than transistors on different dice and adjacent transistors match better than widely separated ones. WID variations are more challenging to manage because some of the millions or billions of transistors on a chip are likely to stray far from typical parameters. Section 7.5 considers the statistics of WID variation.


7.2.4 Design Corners


From the designer’s point of view, the collective effects of process and environmental variation can be lumped into their effect on transistors: typical (also called nominal ), fast, or slow. In CMOS, there are two types of transistors with somewhat independent characteristics, so the speed of each can be characterized. Moreover, interconnect speed may vary independently of devices. When these processing variations are combined with the environmental variations, we deﬁne design or process corners. The term corner refers to an imaginary box that surrounds the guaranteed performance of the circuits, as shown in Figure


7.5. The box is not square because some characteristics such as oxide thickness track between devices, making it impossible to ﬁnd a slow nMOS transistor with thick oxide and a fast pMOS transistor with thin oxide simultaneously.


FIGURE 7.4  Wafer map of the frequency distribution of a ring oscillator circuit  in 90-nm CMOS technology. From M. Pelgrom, “Nanometer CMOS: An Analog  Design Challenge!” IEEE Distinguished Lecture, Denver 2006. (Figure courtesy  of B. Ljevar (NXP). Reprinted with permission.)


7.2      Variability 245


Table 7.2 lists a number of interesting design corners. The corners are speciﬁed withﬁve letters describing the nMOS, pMOS, interconnect, power supply, and temperature,respectively. The letters are F, T, and S, for fast, typical, and slow. The environmental corners for a 1.8 V commercial process are shown in Table 7.3, illustrating that circuits are fastest at high voltage and low temperature. Circuits are most likely to fail at the corners of the design space, so nonstandard circuits should be simulated at all corners to ensure they operate correctly in all cases. Often, integrated circuits are designed to meet a timing speciﬁcation for typical processing. These parts may be binned; faster parts are rated for higher frequency and sold for more money, while slower parts are rated for lower frequency. In any event, the parts must still work in the slowest SSSSS environment. Other integrated circuits are designed to obtain high yield at a relatively low frequency; these parts are simulated for timing in the slow process corner. The fast corner FFFFF has maximum speed.


Other corners are used to check for races and ratio problems where the relative strengths and speeds of different transistors or interconnect are important. The FFFFS corner is important for noise because the edge rates are fast, causing more coupling; the threshold voltages are low; and the leakage is high [Shepard99].


Often, the corners are abbreviated to fewer letters. For example, two letters generally refer to nMOS and pMOS. Three refer to nMOS, pMOS, and overall environment. Four refer to nMOS, pMOS, voltage, and temperature.


It is important to know the design corner when interpreting delay speciﬁcations. For example, the datasheet shown in Figure 4.25 is speciﬁed at the 25 °C TTTT corner. The SS corner is 27% slower. The cells are derated at 71% per volt and 0.13%/°C, for additional penalties of 13% each in the low voltage and high temperature corners. These factors are multiplicative, giving SSSS delay of 1.62 times nominal.


TABLE 7.2  Design corner checks Corner


Purpose


nMOS pMOS Wire VDD Temp


S Timing speciﬁcations (binned parts)


S Timing speciﬁcations (conservative)


F Race conditions, hold time constraints, pulse collapse, noise


?


S Dynamic power


S Subthreshold leakage noise and power, overall noise analysis


S Races of gates against wires


F Races of wires against gates


F Pseudo-nMOS and ratioed circuits noise margins, memory read/write,race of pMOS against nMOS


F Ratioed circuits, memory read/write, race of nMOS against pMOS


TABLE 7.3  Environmental corners


Corner


Voltage


1.98


nMOS


Fast


Slow


TT


FF


SS


FS


SF


FIGURE 7.5  Design corners


246


[Ho01] and [Chinnery02] ﬁnd the FO4 inverter delay can be estimated from the effective channel length Leff (also called Lgate) as follows:


Leff × (0.36 ps/nm) in TTTT corner


Leff × (0.50 ps/nm) in TTSS corner


Leff × (0.60 ps/nm) in SSSS corner


Note that the effective channel length is aggressively scaled faster than the drawn channel length to improve performance, as shown in Table 3.2. Typically, Leff = 0.5–0.7 Ldrawn.


For example, Intel’s 180 nm process was originally manufactured with Leff = 140 nm and eventually pushed to Leff = 100 nm. This model predicts an FO4 inverter delay of about 50–70 ps in the TTSS corner where design usually takes place. Low-power processes with higher threshold voltages will have longer FO4 delays.


7.4.1 Transistor Scaling


Dennard’s Scaling Law [Dennard74] predicts that the basic operational characteristics of a MOS transistor can be preserved and the performance improved if the critical parameters of a device are scaled by a dimensionless factor S. These parameters include the following: All dimensions (in the x, y, and z directions)


Device voltages


Doping concentration densities


This approach is also called constant ﬁeld scaling because the electric ﬁelds remain the same as both voltage and distance shrink. In contrast, constant voltage scaling


shrinks the devices but not the power supply. Another approach is lateral


scaling, in which only the gate length is scaled. This is commonly called a


gate shrink because it can be done easily to an existing mask database for a


design.


The effects of these types of scaling are illustrated in Table 7.4 (next


page). The industry generally scales process generations with


; this


is also called a 30% shrink. It reduces the cost (area) of a transistor by a factor of two. A 5% gate shrink (S = 1.05) is commonly applied as a process


becomes mature to boost the speed of components in that process.


Figure 7.14 shows how voltage has scaled with feature size. Historically, feature sizes were shrunk from 6 m to 1 m while maintaining a 5 V


supply voltage. This constant voltage scaling offered quadratic delay


improvement as well as cost reduction. It also maintained continuity in I/O


voltage standards. Constant voltage scaling increased the electric ﬁelds in


devices. By the 1 m generation, velocity saturation was severe enough that decreasing feature size no longer improved device current. Device breakdown from the high ﬁeld was another risk. And power consumption became unacceptable. Therefore, Dennard scaling has been the rule since the half-micron node. A 30% shrink with Dennard scaling improves clock frequency by 40% and cuts power consumption per gate by a factor of 2.


Maintaining a constant ﬁeld has the further beneﬁt that many nonlinear factors and wearout mechanisms are essentially unaffected. Unfortunately, voltage scaling has dramatically slowed since the 90 nm generation because of leakage, and this may ultimately limit CMOS scaling.


The FO4 inverter delay will scale as 1/S assuming ideal constant-ﬁeld scaling. As we saw in Section 7.2.4, this delay is commonly 0.5 ps/nm of the effective channel length for typical processing and worst-case environment.


S = 2


Feature Size ( m)


10 VDD


FIGURE 7.14


Voltage scaling with feature size


256


Example 7.2


Nanometer processes have gate capacitance of roughly 1 fF/ m. If the FO4 inverter delay of a process with features size f (in nm) is 0.5 ps × f, estimate the ON resistance of a unit (i.e., 4  wide) nMOS transistor.


SOLUTION: An FO4 inverter has a delay of 5 = 15RC. Therefore,


(7.9)


A unit transistor has width W = 2f and thus capacitance of C = 2f fF/ m. Solving for R,


(7.10)


TABLE 7.4  Inﬂuence of scaling on MOS device characteristics Parameter


Sensitivity


Dennard Scaling


Constant Voltage


Lateral Scaling


Scaling Parameters


Length: L


1/S


Width: W


Gate oxide thickness: tox


Supply voltage: VDD


Threshold voltage: Vtn, Vtp


Substrate doping: NA


Device Characteristics


Current: Ids


Resistance: R


Gate capacitance: C


Gate delay:


1/S2


Clock frequency: f


S2


Switching energy (per gate): E


CV 2DD


1/S3


Switching power dissipation (per gate): P


Ef


Area (per gate): A


Switching power density


P/A


S3


Switching current density


Ids/A


W L t


DD ds


WL tox


= =0 515 30. psnm


16 6


ps nm


m fF


7.4      Scaling 257


Note that this is independent of feature size. The resistance of a unit transistor is roughly independent of feature size, while the gate capacitance decreases with feature size. Alternatively, the capacitance per micron is roughly independent of feature size while the resistance · micron decreases with feature size.


7.4.2 Interconnect Scaling


Wires also tend to be scaled equally in width and thickness to maintain an aspect ratio close to 2.1 Table 7.5 shows the resistance, capacitance, and delay per unit length. Wires


TABLE 7.5  Inﬂuence of scaling on interconnect characteristics Parameter


Sensitivity Scale Factor


Width: w


Spacing: s


Thickness: t


Interlayer oxide height: h


Die size


Dc


Characteristics per Unit Length


Wire resistance per unit length: Rw


Fringing capacitance per unit length: Cwf


Parallel plate capacitance per unit length: Cwp


Total wire capacitance per unit length: Cw


Cwf  + Cwp


Unrepeated RC constant per unit length: twu


RwCw


Repeated wire RC delay per unit length: twr(assuming constant ﬁeld scaling of gates)


Crosstalk noise


Energy per bit per unit length: Ew


CwVDD2


Local/Semiglobal Interconnect Characteristics


Length: l


Unrepeated wire RC delay


l 2twu


Repeated wire delay


ltwr


Energy per bit


l Ew


Global Interconnect Characteristics


S2Dc2


Dc /S2


1Historically, wires had a lower aspect ratio and could be scaled in width but not thickness. This helped control RC delay. However, coupling capacitance becomes worse at higher aspect ratios and thus crosstalk limits wires to an aspect ratio of 2–3 before the noise is hard to manage.


1 / SRCR Cw w


1 / S


D Sc


258


can be classiﬁed as local, semiglobal, and global. Local wires run within functional units and use the bottom layers of metal. Semiglobal (or scaled ) wires run across larger blocks or cores, typically using middle layers of metal. Both local and semiglobal wires scale with feature size. Global wires run across the entire chip using upper levels of metal. For example, global wires might connect cores to a shared cache. Global wires do not scale with feature size; indeed, they may get longer (by a factor of Dc , on the order of 1.1) because die size has been gradually increasing.


Most local wires are short enough that their resistance does not matter. Like gates,their capacitance per unit length is remaining constant, so their delay is improving just like gates. Semiglobal wires long enough to require repeaters are speeding up, but not as fast as gates. This is a relatively minor problem. Global wires, even with optimal repeaters, are getting slower as technology scales. The time to cross a chip in a nanometer process can be multiple cycles, and this delay must be accounted for in the microarchitecture.


Observe that when wire thickness is scaled, the capacitance per unit length remains constant. Hence, a reasonable initial estimate of the capacitance of a minimum-pitch wire is about 0.2 fF/ m, independent of the process. In other words, wire capacitance is roughly 1/5 of gate capacitance per unit length.


7.4.3 International Technology Roadmap for Semiconductors


The incredible pace of scaling requires cooperation among many companies and researchers both to develop compatible process steps and to anticipate and address future challenges before they hold up production. The Semiconductor Industry Association (SIA)develops and updates the International Technology Roadmap for Semiconductors (ITRS)[SIA07] to forge a consensus so that development efforts are not wasted on incompatible technologies and to predict future needs and direct research efforts. Such an effort to predict the future is inevitably prone to error, and the industry has scaled feature sizes and clock frequencies more rapidly than the roadmap predicted in the late 1990s. Nevertheless, the roadmap offers a more coherent vision than one could obtain by simply interpolating straight lines through historical scaling data.


The ITRS forecasts a major new technology generation, also called technology node,approximately every three years. Table 7.6 summarizes some of the predictions, particularly for high-performance microprocessors. However, serious challenges lie ahead, and major breakthroughs will be necessary in many areas to maintain the scaling on the roadmap.


TABLE 7.6  Predictions from the 2007 ITRS Year


2009


2012


2018


2021


Feature size (nm)


8.4


Lgate (nm)


VDD (V)


0.65


Billions of transistors/die


6.2


12.4


24.7


Wiring levels


15


Maximum power (W)


DRAM capacity (Gb)


Flash capacity (Gb)


7.4      Scaling 259


7.4.4 Impacts on Design


One of the limitations of ﬁrst-order scaling is that it gives the wrong impression of being able to scale proportionally to zero dimensions and zero voltage. In reality, a number of factors change signiﬁcantly with scaling. This section attempts to peer into the crystal ball and predict some of the impacts on design for the future. These predictions are notoriously risky because chip designers have had an astonishing history of inventing ingenious solutions to seemingly insurmountable barriers.


7.4.4.1 Improved Performance and Cost  The most positive impact of scaling is that performance and cost are steadily improving. System architects need to understand the scaling of CMOS technologies and predict the capabilities of the process several years into the future, when a chip will be completed. Because transistors are becoming cheaper each year,architects particularly need creative ideas of how to exploit growing numbers of transistors to deliver more or better functions. When transistors were ﬁrst invented, the best predictions of the day suggested that they might eventually approach a ﬁfty-cent manufacturing cost. Figure 7.15 plots the number of transistors and average price per transistor shipped by the semiconductor industry over the past three decades [Moore03]. In 2008, you could buy more than 100,000 transistors for a penny, and the price of a transistor is expected to reach a microcent by 2015 [SIA07].


7.4.4.2 Interconnect  Scaled transistors are steadily improving in delay, but scaled global wires are getting worse. Figure 7.16, taken from the 1997 Semiconductor Industry Association Roadmap [SIA97], forecast the sum of gate and wire bottoming out at the 250 or 180 nm generation and getting worse thereafter. The wire problem motivated a number of papers predicting the demise of conventional wires. However, the plot is misleading in two ways. First, the “gate” delay is shown for a single unloaded transistor (delay = RC ) rather than a realistically loaded gate (e.g., an FO4 inverter delay = 15RC ). Second, the wire delays shown are for ﬁxed lengths, but as technology scales, most local wires connecting gates within a unit also become shorter.


In practice, for short wires, such as those inside a logic gate, the wire RC delay is negligible and will remain so for the foreseeable future. However, the long wires present a considerable challenge. It is no longer possible to send a signal from one side of a large,


FIGURE 7.15  Transistor shipments and average price (© IEEE 2003.)


260


high-performance chip to another in a single cycle. Also, the “reachable radius” that a signal can travel in a cycle is steadily getting smaller, as shown in Figure 7.17. This requires that microarchitects understand the ﬂoorplan and budget multiple pipeline stages for data to travel long distances across the die.


Repeaters help somewhat, but even so, interconnect does not keep up. Moreover,the “repeater farms” must be allocated space in the ﬂoorplan. As scaled gates become faster, the delay of a repeater goes down and hence, you should expect it will be better to use more repeaters. This means a greater number of repeater farms are required.


One technique to alleviate the interconnect problem is to use more layers of interconnect. Table 7.7 shows the number of layers of interconnect increasing with each generation in TSMC processes. The lower layers of interconnect are classically scaled to provide high-density short connections. The higher layers are scaled less aggressively, or possibly even reverse-scaled to be thicker and wider to provide low-resistance, highspeed interconnect, good clock distribution networks, and a stiff power grid. Copper and low-k dielectrics were also introduced to reduce resistance and capacitance.


Blocks of 50–100 Kgates (1 Kgate = 1000 3-input NAND gates or 6000 transistors) will continue to have reasonably short internal wires and acceptably low wire RC delay [Sylvester98]. Therefore, large systems can be partitioned into blocks of roughly this size with repeaters inserted as necessary for communication between blocks.


TABLE 7.7  Scaling of metal layers in TSMC processes Process (nm)


3 (Al)


4 (Al)


5 (Al)


6 (Al, low-k)


7 (Cu, low-k)


8 (Cu, low-k)


9 (Cu, low-k)


10 (Cu, low-k)


FIGURE 7.16  Gate and wire delay scaling (Reprinted from [SIA97] with permission  of the Semiconductor Industry Association.)


Chip Size


Reachable Radius


180 nm


90 nm


FIGURE 7.17


Reachable radius scaling


7.4      Scaling 261


7.4.4.3 Power  In classical constant ﬁeld scaling, dynamic power density remains constant and overall chip power increases only slowly with die size. In practice, microprocessor power density skyrocketed in the 1990s because extensive pipelining increased clock frequencies much faster than classical scaling would predict and because VDD is somewhat higher than constant ﬁeld scaling would demand. High-performance microprocessors bumped against the limit of about 150 W that a low-cost fan and heat sink can dissipate.


This trend has necessarily ended, and now designers aim for the maximum performance under a power envelope rather than for the maximum clock rate.


Static power is a more serious limitation. Subthreshold leakage power increased exponentially as threshold voltages decreased, and has abruptly changed from being negligible to being a substantial fraction of the total. Section 5.4.2 demonstrated that static power should account for approximately one-third of total power to minimize the energy-delay product. Higher leakage has required the adoption of power gating techniques to control power during sleep mode, especially for battery-powered systems. To limit leakage to –100 nA/ m, Vt has remained fairly constant near 300 mV. The VDD /Vt ratio has dropped from about 5 in older processes toward 3, and EQ (5.27) showed that it may go as low as 2 for best EDP. As the ratio decreased, circuits with threshold drops have ceased to be viable.


Performance suffers as the gate overdrive decreases, so VDD scaling has slowed below the 90 nm node. This increases the electric ﬁelds, exacerbating velocity saturation and reliability problems. It also raises dynamic power.


Gate leakage current is also important for oxides of less than 15–20 Å, and essentially precludes scaling oxides below 10 Å. If oxides thickness does not scale with the other dimensions, the ratio of ON to OFF current degrades. High-k metal gates solve the problem by offering a lower effective thickness at a higher physical thickness.


Even if power remains constant, lower supply voltage leads to higher current density.


This in turn causes higher IR drops and di/dt noise in the supply network (see Sections


9.3.5 and 13.3). These factors lead to more pins and metal resources on a chip being required for the power distribution networks.


All considered, scaling is being squeezed from many directions by power limitations.


Some manufacturers are ﬁnding that conventional scaling can offer performance or power beneﬁts, but not both [Muller08]. Intel is aggressively introducing new materials such as high-k metal gates and strained silicon to continue to see both performance and power beneﬁts from scaling at the 45 nm node. Even so, the frenetic pace of Moore’s Law may begin slowing at last.


7.4.4.4 Variability  As transistors shrink, the spread in parameters such as channel length and threshold voltage increases. Variability has moved from being an analog nuisance to becoming a key factor in mainstream digital circuits. Designers are forced to employ wider guard bands to ensure that an acceptable fraction of chips meet speciﬁcations. Later sections of this chapter examine variability and variation-tolerant design techniques in more detail.


7.4.4.5 Productivity  The number of transistors that ﬁt on a chip is increasing faster than designer productivity (gates/week). This leads to design teams of increasing size, difﬁculty recruiting enough experienced engineers when the economy is good, and a trend to outsource to locations such as India where more engineering graduates are available. (Bangalore was once considered a low-cost labor market as well, but salaries have been increasing exponentially because of demand and may approach global parity within the decade.) It has driven a search for design methodologies that maximize productivity, even at the expense of performance and area. Now most chips are designed using synthesis and place


& route; the number of situations where custom circuit design is affordable is diminishing.


In other words, creativity is shifting from the circuit to the systems level for many designs.


On the other hand, performance is still king in the microprocessor world. Design teams in that ﬁeld are approaching the size of automotive and aerospace teams because the development cost is justiﬁed by the size of the market. This drives a need for engineering managers who are skilled in leading such large organizations.


The number of 50–100 Kgate blocks is growing, even in relatively low-end systems.


This demands greater attention to ﬂoorplanning and placement of the blocks.


One of the key tools to solve the productivity gap is design reuse. Intellectual property(IP) blocks can be purchased and used as black boxes within a system-on-chip (SOC) in much the same way chips are purchased for a board-level design. Early problems with validation of IP blocks have been partially overcome, but the market for IP still lacks transparency.


7.4.4.6 Physical Limits  How far will CMOS processes scale? A minimum-sized transistor in a 32 nm process has an effective channel length of less than 100 Si atoms. The gate oxide is only 4 atoms thick. The channel contains approximately 50 dopant atoms. It is clear that scaling cannot continue indeﬁnitely as dimensions reach the atomic scale.


Numerous papers have been written forecasting the end of silicon scaling [Svensson03].


For example, in 1972, the limit was placed at the 0.25 m generation because of tunneling and ﬂuctuations in dopant distributions [Hoeneisen72, Mead80]; at this generation, chips were predicted to operate at 10–30 MHz! In 1999, IBM predicted that scaling would nearly grind to a halt beyond the 100 nm generation in 2004 [Davari99].


In the authors’ experience, seemingly insurmountable barriers have seemed to loom about a decade away. Reasons given for these barriers have included the following:


Subthreshold leakage at low VDD and Vt


Tunneling current through thin oxides


Poor I-V characteristics due to DIBL and other short channel effects


Dynamic power dissipation


Lithography limitations


Exponentially increasing costs of fabrication facilities and mask sets


Electromigration


Interconnect delay


Variability


Dennard scaling is beginning to groan under the weight of its own success. At the 32 nm node and beyond, the performance and power beneﬁts of geometrical scaling are starting to diminish as the engineering costs continue to escalate. Nevertheless, scaling still provides a competitive advantage in a cutthroat industry. Improved structures such as copper wires, low-k dielectrics, strained silicon, high-k metal gates, and 3D integration provide beneﬁts independent of reduced feature size. Novel structures are under intensive research. A large number of extremely talented people are continuously pushing the limits and hundreds of billions of dollars are at stake, so we are reluctant to bet against the future of scaling.


7.5      Statistical Analysis of Variability 263


7.5 Statistical Analysis of Variability


Variability was introduced in Section 7.2. Die-to-die variability is relatively straightforward to handle with process corners deﬁning the range of acceptable variations (e.g., 3 );designing to ensure that all chips within the corners meet speed, power, and functionality requirements; and rejecting the few chips that fall outside the corners. Within-die variability is more complicated because a chip has millions or billions of transistors. Even if the die itself is in the TT corner, some transistors are likely to stray at least 5  from the mean. To achieve acceptable yield, most chips with a few such extreme variations must still be acceptable. Static CMOS gates are so robust that they generally function correctly even when parameters vary enormously. However, their delay and leakage will change, which affects the delay and leakage of the entire chip. Special circuits such as memories, analog circuits, and trickier circuit families may fail entirely under extreme variation.


This section revisits within-die variability from a statistical point of view. It begins with a review of the properties of random variables that are essential for understanding onchip variability. Then, it examines the sources of variability in more detail. Finally, it considers the impact of variation on circuit delay, energy, and functionality.


7.5.1 Properties of Random Variables


The probability distribution function (PDF ) f (x) speciﬁes the probability that the value of a continuous random variable X falls in a particular interval:


(7.11)


The cumulative distribution function (CDF ) F(x) speciﬁes the probability that X is less than some value x:


(7.12)


Thus, the PDF is the slope of the CDF at any given point.


(7.13)


The mean or expected value, written as X or E[X], is the average value of X.


(7.14)


The standard deviation (X) measures the dispersion; i.e., how far X is expected to vary from its mean.


(7.15)


It is often more convenient to deal with the variance, 2(X ), to avoid the square root.


P a X b


f x dx


a b


< = ( )


F x P X x


f u du


= <( ) =


f xddxF x( ) ( )=


X E X


x f x dx


E x X


x X f x dx


= ( ) = ( )2 2


264


When studying variability in circuits, we are usually interested in the variation from the nominal (mean) value. Thus, a random variable X can be written as X = X + Xv, where X is the mean and Xv is a random variable with zero mean describing the variation. Thus,we will focus on such zero-mean random variables.


7.5.1.1 Uniform Random Variables  Figure 7.1(a) shows a uniform random variable with zero mean. A uniform random variable distributed between –a and a has the following PDF, CDF, and variance:


(7.16)


7.5.1.2 Normal Random Variables  Figure 7.1(b) shows a normal random variable. It is convenient to shift the variable to have zero mean, then scale it to have a standard deviation = 1. The result is called a standard normal distribution and has the following PDF, CDF, and variance:


(7.17)


where erf(x) is the error function.2 For example, a threshold voltage with a mean of 0.3 V and a standard deviation of 0.025 V can be expressed as Vt =


0.3 + 0.025 X, where X is a standard normal random variable.


A component may fail if a parameter varies too far. The CDF describes the probability that the parameter is less than an upper bound. It is shown in Figure 7.18 and handy values are given in Table 7.8. For example, a chip may be rejected if its delay is more than 3  above nominal, and this event has a probability of 0.135%.


7.5.1.3 Sums of Random Variables  Chip designers are frequently interested in quantities such as path delay that are the sum of independent random variables. The mean is the sum of the means. If the distributions are normal, the sum is another normal distribution with 2Microsoft Excel and other spreadsheets deﬁne erf, which is more convenient than looking it up in a mathematical handbook. In some versions of Excel, you must ﬁrst select Add-Ins from the Tools menu and check Analysis ToolPak to use the function.


f x


a x a


F x


1 2 0


otherwise


x a x a


Xa


1 2 1


erf


= 1


−3 −2 −1 0 1 2 3


−2


F(x)


10−10


10−8


10−6


10−4


10−2


1 − F(x)


FIGURE 7.18  Cumulative distribution function  for a standard normal random variable


7.5      Statistical Analysis of Variability 265


a variance equal to the sum of the variances:


(7.18)


Even if the distributions are not normal, the Central Limit Theorem states that EQ (7.18)still holds as the number of variables gets large. Therefore, it is often a reasonable approximation to replace uniformly distributed variables with normal variables that have the same variance.


7.5.1.4 Maximum of Random Variables  The cycle time is set by the


longest of many possible critical paths that have nearly equal nominal


delays. Let M be the maximum of N random variables with independent standard normal distributions. M is not normally distributed, but


its expected value and standard deviation can be found numerically as


a function of N, as given in Table 7.9. As N increases, the expected


maximum increases (roughly logarithmically for big N ) and its standard deviation decreases. Figure 7.19 shows how the distribution of


longest paths change with the number of nearly critical paths. As the


number of paths increase, they form a tight wall with an expected


worst-case delay that can be signiﬁcantly longer than nominal


[Bowman02]. [Clark61] extends this tabular approach to handle random variables with correlations and unequal standard deviations.


TABLE 7.8  CDF of standard normal random variables


1 – F(x)


0.8413


1.59 × 10–1

