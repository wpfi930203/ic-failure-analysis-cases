---
title: "SzuHuat & Venkat.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_e0c2178eb044465b433ae72307b768b77295230462135641
file_size: 14858762
---

IPFA 2019


Advanced Fault Isolation Technologies: Design  House and Foundry Perspectives


Szu Huat


GLOBALFOUNDRIES, Singapore


Venkat Ravikumar


Advanced Micro Devices, Singapore


Singapore University of Technology and Design


Foundry Vs Design House


||Foundry |Design House |
|---|---|---|

|Types of |Yield, customer returns |Yield, customer returns, post silicon validation, reliability, test verification |

|Failures |Yield, customer returns |Yield, customer returns, post silicon validation, reliability, test verification |

|Fail Samples |Wafer with many dies, some packaged units |Many one of a kind failures |

|Fail Samples |Wafer with many dies, some packaged units |(early |

|Fail Samples |Wafer with many dies, some packaged units |samples/reliability/returns) |

|Information Availability |Limited, subject to customer and confidentiality |More easily available |

|Resource and Infrastructure availability |Many products/customers with limited resources |More easily available |

FA 101 – Simple FA Process Flow


[Source: Vallet DP, IEEE Design & Test of Computers, 1997.]


Failure  Verification


Fault


Localization


Deprocessing


Defect Localization  and


Characterization


Inspection and  Physical


narrows the  search area  for defects


electrical  verification  of the


failure


mode


sequentially  delayers,


employing


both


mechanical  and chemical  means.


a secondary


localization step  to further pinpoint  the exact fail


location or


characterize the  defect


delayers or Xsection to


inspect the


defect, to


determine the  failure root


cause


Global


Local


Advanced Fault Isolation Technologies


• Dynamic Fault Isolation (Vs Static Fault Isolation)


• Change in mindset (    measurement of FA success)


• Enhanced workflow


• Advanced techniques and derivatives


• Cross-functional domain approaches (design, test, AI…)


Role of Fault Isolation in Product Value Chain


Root cause/


Improvement fixes


B1


nt4


Test


Product


Physical failure


engineering


Fault Isolationanalysis (PFA)TNA sigl


Accelerating Product Yield Ramp


|IMPROVED 1st Silicon Ramp FASTER TIME TO PRODUCTION Yield Production ramp Accelerated  ramp|EFFECTIVE YIELD MONITORING Improved Profitability Respins|
|---|---|

|IMPROVED 1st Silicon Ramp FASTER TIME TO PRODUCTION Yield Production ramp Accelerated  ramp|Tapeout|

|6 |6 |

Attributes of Advanced Fault Isolation  Technologies


• Yield-Oriented


– Strive for 100% yield impactful FA success – More than a technique; workflow is important


• Effective and Efficient


– Harness strengths and understand limitations of different techniques


• Innovative


– Beyond mainstream approaches (bitmapping, scan diagnosis etc) Develop alternatives


– Overcome product information inadequacy (foundry environment) – Cross-functional domain collaborations (software, hardware, AI)


Purpose


• Review advanced failure isolation methods


• Demonstrate using case examples


• Discuss emerging and cross-functional domain approaches


Outline


• Introduction


– FA process flow


– Importance of FA (Fault Isolation) to yield engineering


– Overview of current fault isolation methods (software, hardware, static, dynamic,


global, local)


• Equipment Setup and Workflows


– Software-based techniques setup workflow and challenges – Motivation for dynamic fault isolation approaches


– Introduction to Test Fundamentals


• Typical test flow, terminologies, common debug tools


– Hardware-based techniques setup workflow and challenges


• Hard-dock, soft-dock


• Wafer, package


• Challenges: cooling, optical resolution, vibration etc.


1.5 HR


• Global Dynamic Fault Isolation techniques: Concepts/ Principles and


Applications


– Emission-based (PEM, Thermal)


– Laser-based (SDL, LADA, TRLADA, FM/LVI, 2nd harmonic, phase mapping, 2pLADA,


EeLADA)


• Local Dynamic Fault Isolation techniques: Concepts/ principles and


– Laser Voltage Probing (LVP)


• Other Emerging Techniques


2 HR


Overview


Fault  Isolation


Software  approach


Hardware  approach


Bitmapping (eMemories)


农N


Scan Diagnosis (Digital Logic)


Static


Tester-based


(Dynamic)


SB


SFC


[Source: Mentor, a Siemens Business, -layout-aware-diagnosis-]


Global Local


Digital Logic Failures


namepath


T p 0


0.


• Software-based


List of PFA candidates


1 1 69 hdrmsfqbxss2fr /lym_i4/lym_i/lym_glm_i/i_lym_glm_clus4293.8 4693 1 2.1 100 hdrmsfqbxss2fr /lym_i1/lym_i/lym_glm_i/i_lym_glm_clus1435.1  1 3 63 hdrmsfqbxss2fr /lym_i3/lym_i/lym_glm_i/i_lym_glm_clus3028.4 4287


4349


1 0 1 1 0 0  0  1 0 1 1


1 0 1 0 0 0 1 0 0 1 0 1 1


Expected Responses (test pattern) coord1x_人3


Test outcome 1 1.6 100 hdrmsfqbxss2fr


365.95 3193


1 1.4 100 hdrmsfqbxss2fr


3091.4 4647


fail


Tester


Scan-out


Suspect


FF1


Clock reaching


@6ns


FF2 1


0


Combinational Logic


Ob6u W3


LogicCombinational


1


1 1 81 hdrmsfqbxss2fr /lym_i2/lym_i/lym_glm_i/i_lym_glm_clus2430.7  1 1.2 100 hdrmsfqbxss2fr /lym_i5/lym_i/lym_glm_i/i_lym_glm_clus365.69  1 1.2 100 hdrmsfqbxss2fr /lym_i4/lym_i/lym_glm_i/i_lym_glm_clus3954.3  1 1.4 99 hdrmsfqbxss2fr


2801.6 3875


4517


3283


4376


1 3.1 100 hdrmsfqbxss2fr /lym_i1/lym_i/lym_glm_i/i_lym_glm_clus1632 4304


Combinational Logic1


Scan test/ logic suspects (chain pass)


Scan chain suspects (chain fail) Suspect 2


Problem Statement


1888


|35um|35um|35um|
|---|---|---|

177um


• Long suspected beyond physical FA inspection confidence


Layout-aware Scan Diagnosis


Net trace from


diagnosed callouts


Potential suspect area for  inspection


红


--


"


U


DCH


WC伍佰


2m EP ID UE


n


LIKImmT


Driver


NetA


THDTNIMNM AEIF


Suspect area


NC


C


NetB


00 100


LUULED BLDE BNLLUULOLEJLJIBUILL


E I


工1


红重


XX


DriverNetB


[Source: Geir E, Mentor, a Siemens Business]


807712


519681487


Volume Diagnosis


56


1 20


tackingNets S


170489352040758420407667


19682776


NetID NetID


19682786


Nets Stacking


‘fingerprinting’ : Pareto


d


141


1 20 56


103 141


140


120


100


Die countscount80


60


40


20


● Enables prioritization of dies for physical failure analysis•


17049127


20494243-904098


20494182


1597240820494160


‘fingerprinting’: Pareto


15972416


2040758317048976


20494246-


20494149-20494164


1597239420407601


904104


Enables prioritization of dies for physical failure analysis


。


103 d


Case Example


35um


P


Heatmap


NV 6.2mmX30.0R GE(M)


10mm


Count: 30


30.00


Layout


PFA


Root-Cause Deconvolution Analysis


• Challenge: inherent ambiguity of scan diagnosis results


• multiple suspects callouts for a real defect


• Solution: RCD reduces diagnosis noise by statistically evaluating the


existence probability of each defect suspect based on design statistics


• Pre-requisite: Large dataset


2%2%


9%


34%


13%


■OPEN M2■SHORT M1


15%


OPEN M3■OPEN M4


24%


18T Buffer Cell 8TLSSD cell


r


■ SHORT M3


[Source: Yan Pan, ISTFA, 2013]


Cell-Aware Diagnosis


• Challenge: Field returns due to internal cell defects.


• Achieve 0 DPPM for automotive !


1.3


• Solution: cell-aware


• Pre-requisite: cell-aware fault model


#cell_internal_suspects=4, #total_cell_internal_faults=56


suspectscore fail_match pass_mismatch typevalue locationlayout_layer critical_area


|1.1|100|2|0|CELL|0|/cpu_i/uPMI/ix420||
|---|---|---|---|---|---|---|---|

|1.2|100|2|0|CELL BRIDGE||D2/NET7_1-C/1.0||

|1.3|100|2|0|CELL_OPEN||D10/NET7_3-NET7_4/1.0G||

|1.4|95|2|1|CELL TON||D22/M1_1-M1_2/1.0||

|1.5|95|2|1|CELL_TOFF||D28/M4_1-M42/1.0G||

|1.6|95|2|1|OPEN|0|B6 route_2 1.85E+02||

|||||||VIA2 9.59E+00||

|||||||route_3 1.34E+01||

[Source: Mentor, a Siemens Business, -cell-aware-diagnosis-]


Memory Failures Fault Localization


• Electrical log


• Diagnosis: Electrical to  logical address


• Scrambling: Logical to  physical address


Embedded memories


Embedded Memory Built-in Self-Test  Memory BIST Controller


|TMB BAP TMB SIB SIB|TMB BAP TMB SIB SIB|
|---|---|

|TAP||

Memory


Interface


TMB


BIST AccessBAP


SIBSIB


IEEE 1149.1


IEEE 1687


Std TAP


Segment Insertion Bit Port (BAP)


[Source: Mentor, a Siemens Business,


• Applies to both functional and structural test


Stop-on-Nth Error Diagnosis


Signed-off LVDB/TSDB


Top.lvdb/ Top.tsdb


ATE Test


Designers


Top.etManufacturing/


Program


Fail logs


Diagnostic


CDP Top.patternspec


Top.pinmap/ Top.setup


Raw Memory


1. Pattern Conversion Tessent Siliconlnsight2. Program Development(TSI)


(JSON)Memory Fail logs


Test Engineering


Memory Library Files


Bitmap


Test patterns .STIL


(TSI) Process


Top.CDP


Failures


Scrambling info


LEF/ DEF


Diagnostic filesPFA


FA


Classification and Selection of Fail Dies


E


Count


TX=


□□Bit fails classification


Software Approach Not Available


Bitmapping


(eMemories) 9


Scan Diagnosis


(Digital Logic)


Limitation in Static Fault Isolation


Test Cycle 0


Compare Fail


Waveform viewer  Fail event


Dynamic   Photon   Emission


0 000000


ref 文文道区


Overlay image  fail 00000000000


die X的这送凶*xxxHXXXXXXXHX


Power up


Automatic Test Equipment (ATE)


Manipulator


Pin DUT board  (512/1024/2048)


***


Testhead with   pin electronics


Power supply


Chiller


Workstation


Test Pattern


• Vector cell/ vector data


• Waveform indices


|signal Vector Cycle #|DS0|DS1|DS2|DS3|DS4|OE|GPIO _1|GPIO _2|CPI O 3|GPIO _ 3|GPIO_ 4|GPIO _5|GPIO 6|GPIO 7|GP IO_8|Mode _0|Mode _1|Mode  2|edi_ a _ 1|edi _a_ 2|edi  a  3|i  a  4ed|||b3 edi_|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

|signal Vector Cycle #|DS0|DS1|DS2|DS3|DS4|OE|GPIO _1|GPIO _2|CPI O 3|GPIO _ 3|GPIO_ 4|GPIO _5|GPIO 6|GPIO 7|GP IO_8|Mode _0|Mode _1|Mode  2|edi_ a _ 1|edi _a_ 2|edi  a  3||edi _ b_ 1|edi _b_ 2|b3 edi_|

|1|X|X|X|X|。|0|。|0|1|X|X|X|X|X|X|0|X 0|X 0|X|X|X|1|0 1|0 1|0|

|2|X|X|X|X|0|。|0|0||||||||||||||1|0 1|0 1|0|

|3|X|X|X|X|0|0||001||X|X|X|X|X|X|0|x|0|0|X|X|X|I 10|10|10||

|4|X|X|X|X|0|0|0|0||||||||||||||1|0|0|10|

|5|X|X|X|X|0|0|0|0|1|X|X|X|X|X|X|0|X 0|X 0|X|X X||1|0 1|0 1|1|

|6|X|X|X|X|0|0|0|0|1|X|X|X|X|X|X|0|X 0|X 0|X|X X||1|0 1|0 1|1|

|7|X|X|X|X|0|0|0|0|1|X|X|X|X|X|X|0|X 0|X 0|X|X|X|1|0 1|0 1|1|

|8|X|X|X|X T|0|000||||||||||||||||1|0 11|0 11||

|9|X|X|X|X|0|0|0|0|1|X|X|X|X|X|X|0 X|0|0|X|X X|||10 11|10 11||

|10|X|X|X|X|0|0|0|0|1|X|X|X|X|X X|X X|X|X|||||0x|0x|0|X|

|11||||||||||||||||||||||||||

Physical Waveform Table


Waveform


“d1: 1             d2:0”


d1d2


“d3: 0             d4:1”


“r1: H”


TDO


Physical


waveform index


Tester period


Drive Actions


2  3


…


六d4


↓


GPIO_1


Test Pass or Fail Determination


• compare vectors


• expect ‘H’ or ‘L’


|signal Vector Cycle #|S0D|DS1|DS2|DS3|DS4|OE|GP IO 1|GP IO_2|GPIO_3|GP IO_3|GPIO 4|GP IO_5|GPIO_6|GPIO 7|GPIO 8|Mode _0|Mode _1|Mode 2|_a_1edi|edi_a_2|edi_a_3|edi_a_4|_b_1edi|edi_b_2|edi_b_3|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

|801|H|L|H|H|P|口|。|。|0|1|||1|0|一|H|生|1||HH|7|H|7|1|H|

|802|L|H|L|7|d|。|0||10||10|1||0 0|1|0|H|7||HH|7|1|H|7|H|

|803|H|L|H|7|d|0|0||1 1|0|0|0|0|0||1|0H|7|7|H H||H|1|7|H|

|801|7||HH|7|d|0|0|1|1|0|1|1|0|0||0|1H|1|1|1|7|1|H|7|1|

|809|7|1|1|7|d|0|0|1|0|1|1|0|0|1|0|0|H|7|1|7|7|H|H|7|7|

|809|H|H|H|7|d|0|0|0|0|1|0|1|1|1||1|IH|1|1|FH||1|1|1|H|

|80L|7|1|H|7|d|0|0|0|1|1|1|0|1||00|01||H|7 I|H|H|7|HH||7|

|808|7|H|H|7|d|0|0|0|0|0|0|0|1|1|1|IH||H|H|H|7|1|1|1|1|

|806||HH|1|7|d|0|0|1|1|0|1|1|1|0|0|01||H|1 H|7||H|1|1|1|

|810|H|7|1|H|d|0|0|1|0|0|0|1|1|0|0|1|1|0|Tl||H|7|7|7|H|

|81↓|H7||1|1|d|0|0|0|0|0|1T|1|1|1|1|||0T|0T|01|||1|1|1|

Useful Test Debug Tools for EFI


Test programdevelopment


DUT


Validation


↑


|||Tester System |Tester System |Tester System |
|---|---|---|---|---|

|Pin Margin |Error map |Error map |Error map |Patte |

||Shmoo |||Timing Diagram |

rn Debug


Timing Diagram


|X|↑ x x|↑|↑|↑|↑|↑ 李 泰 11 x X x x x 。 0|↑ 李 泰 11 x X x x x 。 0|↑ 李 泰 11 x X x x x 。 0|↑ 李 泰 11 x X x x x 。 0|↑ 李 泰 11 x X x x x 。 0|↑ 李 泰 11 x X x x x 。 0|↑ 李 泰 11 x X x x x 。 0|
|---|---|---|---|---|---|---|---|---|---|---|---|---|

|X|↑ x x|↑|P|||↑ 李 泰 11 x X x x x 。 0|↑ 李 泰 11 x X x x x 。 0|↑ 李 泰 11 x X x x x 。 0|↑ 李 泰 11 x X x x x 。 0|↑ 李 泰 11 x X x x x 。 0|↑ 李 泰 11 x X x x x 。 0|↑ 李 泰 11 x X x x x 。 0|

||||||DAB||支||||||

Test cycles


• Analog output waveform can be analyzed for every test cycles


• Applications:


• 1) test program debug 2) test modification debug 3) fail mode eg. stuck@


Case Examples


|Reference |Reference |Reference |
|---|---|---|

|tdi |||

|tdo |tdo ||

|Stuck@0 |Stuck@0 |Stuck@0 |

|tdo |0||

|tdi |0 O|Stuck@1 |

|tdi |0 O|tdo|

|tdo |O-|tdo|

tdo N


tdi


tdo mmn


Reference


abnormal


Shmoo Analysis


VDD Vs Freq


||Test operating point |Test operating point |Test operating point |Test operating point |Test operating point |Test operating point |Test operating point |Test operating point |Test operating point |Test operating point |Test operating point |Test operating point |Test operating point |Test operating point |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

||Passing ||window |window |window |window ||1|||||||

1.2


1.1


1.0


HARD FAIL


V


0.8


0.9


MHz


0.7


No Passing window


0.6-0.5


一


T


50100150200250300350400


||Reference unit |Reference unit |Reference unit |Reference unit |Reference unit |Reference unit |Reference unit |Reference unit |Reference unit |
|---|---|---|---|---|---|---|---|---|---|

|Bad unit ||||Test opera |Test opera |Test opera |Test opera |Test opera |Test opera |

||"|||||||||

||tu|||||||||

||配章 c20  290 90 070 08 20 0 04 000 0 2 1010611 116 11R 12 1 10|配章 c20  290 90 070 08 20 0 04 000 0 2 1010611 116 11R 12 1 10|配章 c20  290 90 070 08 20 0 04 000 0 2 1010611 116 11R 12 1 10|配章 c20  290 90 070 08 20 0 04 000 0 2 1010611 116 11R 12 1 10|配章 c20  290 90 070 08 20 0 04 000 0 2 1010611 116 11R 12 1 10|配章 c20  290 90 070 08 20 0 04 000 0 2 1010611 116 11R 12 1 10|配章 c20  290 90 070 08 20 0 04 000 0 2 1010611 116 11R 12 1 10|配章 c20  290 90 070 08 20 0 04 000 0 2 1010611 116 11R 12 1 10|配章 c20  290 90 070 08 20 0 04 000 0 2 1010611 116 11R 12 1 10|

||红|||||||||

||2T|||||||||

||小|||||||||

||SUI 201 360|||||||||

||60 780 804 te sd e 90|i *.|f 530 shar 80|f 530 shar 80|f 530 shar 80||11103218|11103218|11103218|

00.760.82☑进起


1121181.2413


00 14 300 006 07 0 0p000 12 320 09 090 1


ting point


25C


6' e n sh an as h o10


85Cer,2 028 0aas c00 a ogt 3r00 208d 0s


HVO95


Anatomy of Tester Docking


Locks


Load board  Pogo tower


Probe card  Testhead


Prober Head plate


Types of Testing


Testhead


Loadboard


Package level (Final Test)


Wafer level


socket


Prober  Interface  board


Pogo tower


Probe card


Interface to Scanning Optical Microscope  Prober


ProductionSWAPprober


Laser scanning


Types of Interface for Wafer-level Dynamic EFI


Hard dock


(pogo tower-based)


Soft dock


(cable dock)


Automatic


Test Equipment


Interface board


Prober Interface board


Prober


□Pogo tower


Diagnosis package


package


Diagnosis


Pogo tower 1 /// cables(interposer)


Comparison


||Hard-dock|Soft-dock|
|---|---|---|

|Additional Cost Incurred|Uses production probe stack. No additional cost.|Requires customized probecard or tester interface board.|

|Speed limitation|Similar to production.|Constrained by cable length.|

|Tester Vibration Isolation|Tester vibrations (fan|Tester vibrations decoupled.|

|Tester Vibration Isolation|cooling) not decoupled.|Tester vibrations decoupled.|

|Setup Time|Uses exact probe stack.|Test correlation required|

|Setup Time|Test correlation not|Test correlation required|

|Setup Time|necessary|necessary|

State-of-the-art Wafer-level Systems


Thermo Fisher


SCIENTIFIC


SEMICAPS 5000


MeridianTM WS-DP


5EM1CAPS


HAMAMATSU


iPHEMOS-DD


PHDTON IS OUR BUSINESS


Signal Extractions for Dynamic EFI


Probecard PCB


(Topside)


signal


outout


经


Probehead


plated through-hole on


Probecard PCB (underside)


Loadboard(Topside)


Interface for Package-Level Dynamic FI


Modified lid


025P


YLNO


。0"XOOCHS50OGNO的。


31010-000-05D0.


Conventional lid


OFEN


75010仙


Signal  out


Cooling Challenges for High Current Devices


• Require optical and physical  connection to the sample


• Unable to use heat sinks, fans, etc


|Cooling Solution |Power capacity |Temperature range |Ease of use |Cost |
|---|---|---|---|---|

|Forced Air convection |~10-30W |-40C to >100C |Easy |Cheap |

|Solid state cooling (such as contact diamond) |>100W |-40C to >100C |Subject to warpage/physical barrier |Expensive |

|Water based cooling (spray cooling) |>100W |12C to 40C |Water tight chamber restricts lens |Most expensive |

Solid Immersion Lens (Refractive)


RSIL


Sample0


Z=


RSIL0


Sample


nsilicon


10


Z=0


Challenges: Optical Resolution


boness I


760um


←


r/n→L90mu↑


thickness RSIL


• RSIL thickness has to be big enough for better collection efficiency


Trade-off in Laser Stimulation Throughput


0.000


without SIL


OBIC (A)-0.002


-0.003


-0.004


0200400600


Laser Power (mW)


Voltage =-1V


-0.001


with SIL


• OBIC on Reverse PN Junction


Visible Light Imaging Through SIL  without SIL


with GaP SIL


Table 1: Wavelength of optical CFI technique, required SIL


IR confocal


• Very thin Si Substrate


• Few microns


• Only work on packagedVIS


level EFI


confocal


[Source: Heiko Lohrke, ISTFA, 2016]


material and resolution


|Wavelength [nm]|SIL Material|n of SIL Mat.|Resolution [nm]|Absorption Depth in Si [um]|
|---|---|---|---|---|

|1064|Si|3.5 [4]|152|<300|

|650|GaP|3.3[1]|98|3|

|550|GaP|3.4[1]|81|1.5|

|440|SiC|2.7 [5]|81|0.13|

|330|C|2.5 [6]|66|0.012|

16 nm technology


IR conventional


Wafer-level Dynamic EFI Workflow


Dynamic Fault Isolation


Paeof


Failure Verification


Priofitzation


Few weeks lead-time


• Packaging and lid customization takes time and money


• Not suitable for fast yield ramp in a foundry environment


Few hours


• Cost- and time-efficient approach  Failure


Characterizaton on


Tester-based FI


ATE


Fai，es9nature


(wafer level)


wafer is not destroyed


Striving for 100% FA Success Rate


Supply leakage


Bad Die 1


Dynamic Current


Ref 1 Ref 2 Bad Die1 Bad Die2


VDD Voltage


□


■


■□


Bad Die 2 足山


Test Cycles


Challenge: 100% FA Success Rate = 100% Yield Success


||Yield |
|---|---|

|≠|101 mll|

|Productivity |Performance |

Picking low-hanging fruit to  boost productivity


Find the RIGHT dies that matter to YIELD


|Fail Pass ||
|---|---|

Dies Selection for Analysis


w/ wafer signature


w/out wafer signature


|||0 --01|0 --01||||5171|
|---|---|---|---|---|---|---|---|

|||01|01|117/00RC101 201|117/00RC101 201|的|的|

|"||||--:|--:|↓ ↓|↓ ↓|

|||级1源 4231|级1源 4231|11 11|11 11|1991|1991|

||股:窗|1006 182 1:402: 2 1|1006 182 1:402: 2 1|1|1|0|0|

|NO|901|0|0|1 1 1|1 1 1|I 1|I 1|

||壹|||了 31: IUARB|了 31: IUARB|了 31: IUARB|143 1 了|

|-|10v 1↓||||||1te 1|

|a.|110m|- t :n T||n|XIADQ 11||1.|

|二|0811053 L|001001||H|||10434R 123 11|

||9|3R:OE CUE - I :02|| 9|8 e 39||12B 180 1 10221|

|||1 0:40- 12 ID|110|10 ↓|26 15 -.||e AX|

|9|的|5|5||器||126 1 111a|

|¥ C|验|1118881|1118881||||75 11118|

|||||- 9高 2|- 9高 2|- 9高 2|0EI|

|- -|011-|00|00|19 8|19 8|19 8|限验制!|

||||||1 "|1 "|↓ - -|

|an|9 ■ -|S t|S t|||||

|-|EDEI OH:A|11 O 1|11 O 1||E10B0|E10B0|目|

|a|0:--|2801 10 02 区2|2801 10 02 区2|||||

||mon :|N111D 1PRE X 格|N111D 1PRE X 格||00 10%|00 10%||

|||t|0::--|0::--|00 10%|00 10%||

|5|5|X|t:|t:|-|-|-|

|3|3||12100|12100||||

|Le d|Le d|a|a|-- 148|----|----|----|

2


，


3 5


授


、


• Decision making should be easy


• Should we choose any bad dies?


• How sure are we that the dies


identified are representative of the


yield loss, not outlier?


Failure Characterization: Classification


||||||-5C|-5C|25C|25C|25C|75C|75C|75C|Core  to do EFA|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

||DieX|DieY|fail mode|location|Vmin (0.934V)|Vmax (0.985V)|Vmin (0.9V)|Vmin (0.934V)|Vmax (0.985V)|Vmin (0.9V)|Vmin (0.934V)|Vmax (0.985V)||

|CAT 1|6||8 pure|center|0|0|0|0|0|1|1|1|27|

|CAT 1|8||1pure|edge|0|0|0|1|0|1|1|1|29|

|CAT 1|10||3 pure|center|0|1|0|1|1|1|1|1|18|

|CAT 1|4||7 pure|center|0|1|0|0|1|1|1|1|39|

|CAT 1|2||3 pure|edge|0|0|0|1|1|1|1|1|12|

|CAT 1|3||2|pure|edge|o|0|。|1|1|0|0|1|7|

|CAT 1|9||7 multi|center|0|T|0|o|1|1|1|1|26|

|CAT 1|13||4|multi|edge|0|I|0|0|1|1|1|1|19|

|CAT 1|12||8multi|edge|0|0|0|0|0|0|0|1|7|

|CAT 2|8||3 pure|center|0|0|0|0|0|0|0|0|10,16|

|CAT 2|3|4 pure||center|0|0|0|0|0|0|0|0|19|

|CAT 2|5||5 pure|center|0|0|0|0|0|0|0|0|35|

|CAT 2|8||6 pure|center|0|0|0|0|0|0|0|0|12,19,27,47|

|CAT 2|5||8pure|edge|0|0|0|。|0|0|0|0|20,39|

|CAT 2|8||9 pure|edge|0|0|0|0|0|0|0|0|22,43|

Failure Mode Characterization:


Identify the right test mode for debug


||Prod|Test characterization / Experiments|Test characterization / Experiments|Test characterization / Experiments|Test characterization / Experiments|
|---|---|---|---|---|---|

||sort|Test characterization / Experiments|Test characterization / Experiments|Test characterization / Experiments|Test characterization / Experiments|

||test|Test characterization / Experiments|Test characterization / Experiments|Test characterization / Experiments|Test characterization / Experiments|

|P/F state|PLL|P /F  state|Higher|Forced Reset|Higher|

|P/F state|test @|P /F  state|Vdd|Forced Reset|Vdd +|

|P/F state|1.1V|P /F  state|Vdd|Forced Reset|Forced|

|P/F state|1.1V|P /F  state|Vdd|Forced Reset|Reset|

|Pass|65|Pass|61|65|65|

|Pass|65|Fail|4|0|0|

|Fail|177|Pass|47|35|159|

|Fail|177|Fail|130|142|18|

|Yield Impact (%)|73|%yield recovery|26|20|90|

Failure Characterization:  Identify the ROI


Category 1


Category 2


ROI B  ROI A


I2C data pin  fail at cycle  1108


1mm


I2C data pin  fail at cycle  1136


Category 1  84%


26%


1Category 2


Fundamentals  I▲


Reverse Bias


Forward Bias


1) Intraband:


2) Interband:


Carriers pick upSensitivity Limit kinetic energy in


Vrecombination


E-field and relax by


of injected


emitting photons


excess carriers


Leakage


Band-band


34


[Source: Christian Boit, ISTFA, 2014]


PN Junction


Forward biased


Reverse biased


150


500 50mA,1.07V450


125


400


Intensity (a.u)台a宫


30mA,1.00V 20mA,0.95V


Intensity (a.u)员


10mA,0.90V


25


50-


15mA,7.9V


0+


8001000 1200 14001600


Wavelength (nm)


400500600700800900 0


caust 30mA,8.2V 45mA,8.5V 60mA. 8.9V


40mA,1.03V虽


[Source: WB Len, ISTFA, 2003]  [Source: JCH Phang, IPFA, 2005]


CMOS Inverter


APO


df2h


1V


mid-rail


V(V)


vdsat=


vout


M3:528.338m 8.36904uA


0V


=1,


I (uA)


vth=41 ds=11


M5:31.4286m 531.694pA


WbI '0ZIZIE L81dV


dsot=


:


TO M2:516.241m 516.241mV


CMOS Circuits  Vout (buffer)


∞


●7.82uA


Vout (aoi22) Vout (nand2)No heounspt


7.78uA


Vin (aoi22)B


出


Vout (aoi21)<0


u200.0


NO hotspot


Vout (nor2)


。""


3


211l (buffer)


目


11


291pA


u


4.01uA


35000l (nand2)


3IInA


69InA


8000


l (aoi22)


500 0


0200.0


l (aoi21)


83.0pA


• VIL < Vin < Vin+X


– aoi22 (signal)


100.0


400.0


||l (nor2)|l (nor2)|
|---|---|---|

|Vin (aoi22)<VIL X|Vin (aoi22)<VIL X|Vin (aoi22)<VIL X|

ESSUW


– nand2 (signal)


000


250.0


500


– No signals in further


stages


Emission Spectroscopy


*Show the difference in setup for a basic PEM and one w/prism


*Show one example of a signal image each


Emission Spectra


Fundamental Spectra


入


15501050800 700600500 nm


||1||Ill:oxide radiation|
|---|---|---|---|

|||I: field| accelerated carriers|

|pn-forward||||

|TY|I: bipolar effects|I: bipolar effects|I: bipolar effects|

104


pn-reverse


103 N(E)*


gate oxide


102


defects


a.u.


101


saturated


n-MOSFET


0.40.8


hv


1.21.62.02.4 eV 2.8*N(E):relative Number of Emission Events


105


[Source: Christian Boit, ISTFA, 2015]


Dynamic PEM Setup


LN2-cooled  Automatic


• Localization performed


while the device is


Eqipment Probe stack DUT


Photon Emission Microscopy


人


PC


InGaAs detector


Grabberscreen FrameMonitor


Stage


activated by an ATE


Modes of Application for Global EFI


Loop entire pattern


Hold state


SEMICA


• Better SNR


• Require to know cycle to hold state


Dynamic PEM on MemoryBIST failures


PEM at 20X


Fail Rate (au)


|M1  Bridge|M2 Bridge|M2 Bridge|M2 Broken|M2 Broken|Active Bridge|Missing CA|shortPC-CA|
|---|---|---|---|---|---|---|---|

|BEOL FEOL|BEOL FEOL|BEOL FEOL|BEOL FEOL|BEOL FEOL|BEOL FEOL|BEOL FEOL|BEOL FEOL|

Abnormal  spot


Defect Pareto


• Not so successful on BEOL defect


• Mx-related defects do not emit photons


Dynamic PEM Derivatives


• Differential and lock-in


• Gated Imaging


[Source: ZL Qian, ISTFA 2010]


[Source: ZL Qian, IPFA 2017]


Challenges with CMOS Scaling


[Source: Andrea Bahgat Shehata, ISTA 2014]


• supply voltage reduces


|Increasing λcutoff|Increasing λcutoff|Increasing λcutoff|Increasing λcutoff||
|---|---|---|---|---|

|Increasing λcutoff|Increasing λcutoff|Increasing λcutoff|Increasing λcutoff||

||||DBX,SP1800,TACQ =60s 十 DBX,SP1900,TACQ =60s|DBX,SP1800,TACQ =60s 十 DBX,SP1900,TACQ =60s|

||||子 =60s|子 =60s|

||||DBX,SP2000,TACQ|DBX,SP2000,TACQ|

Signal


• spontaneous emission is


becoming fainter


• "red-shift" (lower energy) of


(a.u.)


the hot-carrier distribution


MEAN古w


• 32 nm SOI testchip inverter


chain


• Short pass (SP) filter to study


Emission signal mean, E


the SNR


• SP1600: l = 1600 nm


0.50.60.70.80.911.11.2 Power supply voltage, VDD (V)


Quantum Efficiency of Detectors  100Si CCD


InGaAs


Quantum Efficiency (%)20八


400900140019002400


古吕


MCT


80


[Source: SL Tan, IPFA 2006]


Qualitative Spectral Range Comparison of  Black Body and Detectors


Relative


Detector


Black SensitivitySiCompound Typ. IR Detector


Body


103CCD.CCD


Intensity


[Arb102 Units]


T=500K


[Arb]


[Units]


T=400 K


100 10-1


T=300K


10-2


123456789 Wavelength λ [μm]


T=600 KRadiant


Temperature Radiation


Wafer-level Thermal Microscopy


|Automatic Test|Automatic Test||
|---|---|---|

|Equipment|Equipment||

|Probe stack|Probe stack||

|DUT|||

|Stage|Stage||

|△|△|PC|

|Thermal Frame Camera Grabber|Thermal Frame Camera Grabber|Thermal Frame Camera Grabber|

• Dynamic test runs  at MegaHertz


(MHz), >> faster


than camera


response


Thermal


Emission


• Lock-In thermal Microscopy Tool emission not


feasible


• steady-state thermography


Dynamic Thermal Microscopy sensitivity on  Memory BIST


Thermal emmi result at  2X (4 scan frame, 4s/f


acquisition time)


Photon emmi result at 5X


(9 scan frame, 60s/f


No abnormal emmi hotspot  observed on same location!!


Exclusive thermal hotspot  observed in SRAM array


[Source: BL Yeoh, IPFA 2018]


Thermal microscopy localization accuracy on  Memory BIST


Overlay


PEM


IR


Thermal: Dynamic vs Static bias


Thermal signal


Artifact


Static bias


Dynamic bias


• Static mode: Artifact signal reduce detectability of weak signal


• Dynamic mode: Eliminate artifact signal, leaving only real signal spot


Thermal Laser Stimulation Techniques


|TLS|Full name|Bias/detection|Device analysis||
|---|---|---|---|---|

|tech-|Full name|Bias/detection|Device analysis||

|nique|Full name|Bias/detection|Device analysis||

|OBIRCH|Optical Beam Induced Resistivity Change|Constant voltage / Current variation|Identifies areas of high local resistance||

|TIVA|Thermally Induced Voltage Alteration|Constant current / Voltage variation|Identifies areas of high||

|TIVA|Thermally Induced Voltage Alteration|Constant current / Voltage variation|local resistance||

|SEI|Seebeck Effect Imaging|Zero current / voltage variation|Zero current / voltage variation|Identifies thermoelectrically active material interfaces|

R=R0[1+a(T-To)].


where:


Ro=P0W.H


a - temperature coefficient of resistivity (TCR),po - resistivity of the material,


standard temperature To.


△V = S12△T = (S1 - S2) △T.


where S1, S2 are thermoelectric


powers of materials which form a junction


L


[Source: Arkadiusz, Dissertation 2010]


• Static applications on hard defects


• Laser Wavelength: 1340 nm (localized heating laser)


Soft Defects


Vdd


Ref


85C


• Presence of passing


window


• 2 possibilities


– Recovers with thermal


stimulus


– Degrades with thermal


Temperature Effect on MOSFET


10-6


• low gate voltages (subthreshold):  Vt


10-9


dependence, drain


L=9μm z/L=9.7


current increase with


(A)ID10-8


VD=0.1V


temperature


VBS=OV


• higher gate voltages


(above threshold):


10-10296K250200150100T=77KEXP


mobility dependence,


o CALCULATED


drain current decrease


T=


61


10-120.2。0.20.40.60.81.0 VG(V)


with temperature


Soft Defect Localization Setup


Probe Stack


wafer


Laser


Scanner


Photodetector


Image  Processor


→


Display


Trigger


+


Pulse


sync "


Soft Defect Localization (SDL)


• 1340nm laser


• Eph < 1.1 eV


P Passing window


• Free carrier absorption


1.5


sion (%)Transmis1


X 1016 cm-3


0.1Si indirect bandgap


0.01一


730


1.01.52.02.5


Wavelength (um)


Tester Shmoo


Laser Scanning


Signal Overlaid Image


625um Si 33


Laser-based Stimulation Techniques


|||P|||
|---|---|---|---|---|

||Passing|windov|||

||Bad Die|Good Die (reference) O|
|---|---|---|

|T= 25C|" ****|Good Die (reference) O|

|Test Set Point|" ****|Good Die (reference) O|

|T=110C|T=110C|T=110C|

• Fmax performance


• SDL Fail-Pass: favourable


Spot 1


Spot 2


Signal: Fail- Pass


qdsp6_L2_16KB_ctl_reg_F


EomG


Photoelectric Effect


• injected carriers locally give rise to


– Photoconductive effect:  (decrease) material  resistance


– Photovoltaic effect:  (increase) current in


separated electric fields


• 1064nm laser


• Eph > 1.1 eV


• e-h pairs generation


Photoelectric Laser Stimulation Techniques


|PLS|Full name|Bias/detection|Device analysis|
|---|---|---|---|

|tech-|Full name|Bias/detection|Device analysis|

|nique|Full name|Bias/detection|Device analysis|

|OBIC|Optical Beam|Constant voltage / Current variation|localizes p-n junctions|

|OBIC|Induced Current|Constant voltage / Current variation|localizes p-n junctions|

|LIVA|Light Induced|Constant current / Voltage variation|Reads out signals sensitive|

|LIVA|Voltage|Constant current / Voltage variation|to logical state|

|LIVA|Alteration|Constant current / Voltage variation|to logical state|

|Dynamic||Constant voltage|Shift of rise/fall times of|

|Dynamic||Constant voltage|FET to study delay|

|Dynamic||Constant voltage|variations|

|OBIRCH, SEI||see table 4.1 for details|treated as parasitic effects by PLS|

LADA   effects


Photocurrent Critical Sources


VSS


DRAIN


VDD


N+/Psub (pWell)


Nwell/Psub  p-substrate


NMOS


PMOS


[Source: Jeremy A. Rowlette, ITC 2003] GNMOS


GPMOS


LADA Vs SDL


• Localized heating of


healthy transistors


p+n+


n+


p+


d+早


induce weak time  shifts (< 2ps)


p-Well


n-Well+


• Insignificant


LADA Effect on PMOS


否


• photocurrent flows from the n-well tap


to the p-substrate


• well resistance reduce


• Body potential drop


• Vt reduce


d+0+


n-Well+2JP


nPd


N


bstrate


LADA Effect on NMOS


• photocurrent flows


from the drain to the


GNMOS


p-well tap


I


• Additional drive


current


古n+


<


a


p


z


云p


Propagation delay changes


Equivalent model


DR/


Case Example: Digital Function Fail


|Vdd|Wave form|
|---|---|

|0.9V|3MHz(pass)|

|0.8V|3MHz & 6MHz Mixed (fail)|

|0.7V|6MHz(fail)|

客2


ROL: 40 34 μm 21.05 μm


Do


GENFSYS{MMG44_5DCLK


INV DoDODO


clock output


24MHzpbuffershold


3MHz


12MHz6MHz


input clock


2divider区


RESETn


(DLY4)


• Laser stimulation induce Vmin increase


• Issue found to be due to hold time violation


1 divider


[Source: : Lee, Sukho, ISTFA 2014]


Case Example: Analog Function Fail


互


ZNO


及


理LNO


LaHe.


3NO


0sec


L00


0.400


cant


Laser off:30MHz"


.*。。t"t OK000200


.YS"Laser on:10MHz


000W


m N**14


PASS: 20MHz


Fail: 30MHz


Figure-16 A typical Shmoo plot of a passing and failing condition, note the additional failing column on the 30MHz Shmoo plot. Each column is 10MHz wide in X.


dvlo


山


canef


1.m


Lod


Loke


2:000


G62


IAG


fo s0


a540


a0.


0400


Laser off: Fail 30MHz Laser on: Pass 30MHz


Soft failures: Case Example


Vdd(V)


Vdd (V)


||Fai |Fai |Fai |Fai |Fai |Fai |Fai |
|---|---|---|---|---|---|---|---|

||Ref|
|---|---|

1.12


1.04


0.96


l


0.88


30445872861003044587286100 Period (ns)


Period (ns)


LADA


Signal image


Shmoo


000吕0


00


5000


000 0 00


0o


0001000


D0


00010


g0


咖


00  0 00 00 u


00 000000-u00


o


000 0000000


0 000


。000


000 00000000000 On 0


00Do0


0 80


00 0


1.16 V


。旨口


"品0点


DO00000


0000 000


0000000


%003000000


Intention:


Solid Fail-Pass


00吕


吕0


50um 0吕


0吕0


Indicates weakest link


Shmoo Response to Laser Stimulus


0%


|||||||||1.09 V|1.09 V|1.09 V|1.09 V|1.09 V|1.09 V|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

09 V|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

|||||1.16 V|1.16 V|1.16 V|
|---|---|---|---|---|---|---|

|||||*|*||||it|*|||
|---|---|---|---|---|---|---|---|---|---|---|---|---|

|||||*|*||||||||

|||||*|*|||||*|||

|||||*|||||||*||

|||||*|||||*|*|*||

|||||||||||*|||

|||||1.02 V|1.02 V|1.02 V|1.02 V|1.02 V|1.02 V|1.02 V|1.02 V|1.02 V|

|||||||*|*|||、|、||

|||||||大|大|||党|党||

||||||||||||*|*|

5%


20%


Combining Scan Diagnosis & LADA


Logic Test


Scan Diag/ Volume Diag  Shmoo Analysis


Test at reduced VDD


1st Shift-out


Cycle


*


二


Scan-in


(0.00.6.00)


Overlaid image


(Scan Diagnosis/ Chip floorplan)


HHHA AhmAh


LDAE F


on


科V Bounding boxes


al


Volume Scan Diagnosis


Dynamic PEM in LADA Signal Vicinity


LADA Signal image


EN4_DG_1


Fail die


Limitations of LADA


• Signal (esp. Pass- Fail) might not indicate a source of


problem


• Multiple signals could be obtained. Unable to determine the  criticality of signals


Digital logic


SRAM


Electrically-Enhanced LADA (EeLADA)


LADA Versus EeLADA


Wafer level scanning optical microscope  Test Pattern


Trigger  Pulse


sync


Laser (pulse)


ri er


lse


failure log


Comparator


log


• LADA applies to  soft failures


• EeLADA applies  to BOTH soft and  hard failures


Requisites for EeLADA


• ability to stimulate ‘healthy’ transistors (flip a cell, SEU)


– pulsed-laser source


• Fail log (fail cycle, pinname, fail state)


Laser: 1064 nm


1E-7


1E-8


1E-9


1E-10


1E-11


1E-12


0.1


0.01


1E-3


Energy  Power


1E-13 1E-11 1E-9 1E--7 1E-5  Pulse Duration (s)


Induced SEU in SRAM: Simulation


[Source: Douin A, IEEE transactions on nuclear science, 2006]


Types of Laser Pulsing


Pulsed Pumping


Amplitude electro-optic modulation (EOM)


Pulsed Pumping: Current Spikes


Duty


Output waveform from  photoreceiver


A


Zoom-in on A


• 10 kHz_0.5 DC input to TTL


• High frequency and large amplitude ringing on the rising edge


• High peak power induced


power


Ave


power=


Peak


Scope input impedance: 50 Ω.


EOM Modulation


• absence of photocurrent overshoots


• delayed response time of 0.2 ms


• DC maintains at 0.5


300 kHz


600 kHz


EOM: Average Power


• > 0.5: possibly due to piezo-resonance effect plays a small part in this variation;


• < 0.5 (> 700 MHz): possibly signal ringing due to electronic pickups from the


high voltage pulser


• Peak power increase due to reduction in DC is studied


Identified for  experiments


100% power output from fibre: 512 mW


Modulation Frequency (kHz)


200 400 600 800 1000 1200


0.3


0.4


0.5


0.6


Pulsed-LADA on SRAM


cw


EOM (400 kHz)


20X objective


Test point: 0.8V


264 mW


75 mW


White: pass-fail


FR (out of 100 loops) on SRAM


• increase in modulation frequency


increases SEU/ LADA FR       lowering of


threshold laser energy for stimulation


less device damage


• 50% FR can be achieved at VDD:1.15 V


• pulsed-LADA less sensitive to boundary


biasing (0.8V boundary)


LADA site


50


300


20  40  60  80  100


0.93V


1.0V


1.15V


EeLADA Application on Memory BIST Failure


Fail pinname


Fail cycle


Fail state


EeLADA signal


Pulse width: 50 ms


Pulse train freq: 10 kHz


Overlay image


EeLADA Application on ATPG Logic Failure


4-level logic sub-circuit


Reference fail log


Fail signature from faults in surrounding  nodes


EeLADA on ATPG Logic Failure: Example


50X


36%


3.6%


Compare matching percentage


(Loc1  with highest matching rate, 36%)


Missing via


Common Terminologies


LP: Laser Probing


LVP: Laser voltage probing


LTP: Laser timing Probe


LTM: Laser timing module


EOP: Electro optical probing


VLP: Visible light probing


SWP: short wavelength probing


LVI: Laser voltage imaging


FM: Frequency mapping


EOFM: Electro optical frequency mapping  SMI: signal mapping imaging


LVX: Laser Voltage probing and imaging


Fundamentals


• Measure changes to absorption of a


transistor


• Local electric fields as well as free


carriers modulate the amount of light


absorbed


– Absorption coefficient (Amplitude


modulation)


– Refractive Index (Phase modulation)


• In addition to free carrier absorption that


occurs at all laser wavelengths, there are


other field effects


– Franz Keldysh


– Kerr


– Electro-refraction


[Source: : Mario Paniccia, Journal of Vacuum Science & Technology B, 1998]


Optical Effects-induced Reflected Laser  Modulation


• When refractive index changes, absorption coefficient also


changes and vice versa. This is known as Kramers-Kronig relation.


This means multiple mechanisms can affect optical parameters.


• Absorption coefficient can be affected by


– Fluctuations to free-carrier density (Free carrier absorption)


– Absorption by tunneling of carriers at high electric fields (Franz  Keldysh)


• Refractive index can be affected directly by electric field [smaller


effects]


• Thermal effects


Δn


Continuous wave LVP => changes to light


intensity


Pulsed laser LVP => changes in phase and  intensity


Phase


Δα


[Source: : Ulrike Kindereit, dissertation, 2008]


Free Carrier Absorption Effect


• Free carriers absorb light across


wavelengths through phonon transfer


• Carriers are modulated by changes to


voltage in terminals of the transistor


• Changes in carrier density causes


changes to absorption


• Where do the carriers change?


1064nm


1320nm


Free carrier density


Photon energy (eV)


Absorption


changes


significantly  depending on  carrier density


[Source: : R. Soref , J. Quantum Electron, 1987]


Carriers Fluctuation


VG


Substrate


Gate


VD


Source


Drai n


Vss


Gate =OFF   Drain = OFF


Max carriers


Most absorption


Min carriers


Least absorption


Drain


*BLUE << RED Carrier density


Gate =OFF   Drain = ON


Gate = ON   Drain = OFF


• The reverse biased diode junction


between drain/source and body as well


as the area under the gate


Franz-Keldysh Effect


• Efficiency of absorption and e-h generation


increases in the presence of electric field.


• E-field assisted tunneling between valence band


and conduction band


• Happens when we use wavelength close to the


bandgap (~1.14eV) of Si (e.g 1064nm


wavelength)


• Not a factor when wavelength is not near bandgap


(e.g.1320nm)


[Source: P. H. Wendland , Phys. Rev, 1965]


Difference Between Pulsed and Continuous  LVP


 Femtosecond pulsed laser  Single measurement per pass  Slower data collection


 More complex


 Higher bandwidth


 Continuous wave laser


 Multiple measurements per


pass


 Faster data collection


 Less complex


 Lower bandwidth


 Allows Laser Voltage Imaging  Pass 1


Pass 2


Pass 1


Sampling  frequency


Continuous wave (CW-LVP)


Pulsed LVP


CW-LVx


Spectrum analyzer  frequency mapping


oscilloscope


laser probing


Frequency Map


10MHz


lens


Laser source


High speed


photo detector


electronics


100ns


Laser probe waveform


[Source: Ng, ISTFA 2010]


Case Examples– Frequency Mapping (FM/LVI)


• FM is great for global fault isolation


• Specifically useful for broken chains (JTAG/Scan)


• Requires a periodic signal to pass through the failing circuitry


Laser  Voltage  Imaging


Scan  Chain


Chain stopped  toggling on this  flop


Either inputs to  flop or internal  nets contain


defect


• Scan Chain Failure


• Clock = 100MHz


• 0101 pattern loaded into Chain


• Data Frequency = 50MHz


• LVI Search for 50MHz


 Gross Scan logic failure


 No emission site


 LVI at clock frequency shows abnormal signals  on callout


 CW-LVP shows similar anomaly


When the transistor suffers  active damage, signals can  appear very anomalous


Limitations of LVI


Not sensitive to phase -> Phase LVI


Unable to show sites on transistors with aperiodic signal -> Laser  Probing


LVI cannot distinguish between  periodic signals


LVI does not work on aperiodic  signals


Phase LVI


• Can differentiate phase offsets between same frequency signals


• Uses Lock-in amplifier instead of Spectrum Analyzer


• Phase information is useful for signal separation


• Limitation: requires periodic signals


Phase LVI: 10MHz, 0.9V


Amplitude


Black = out of  phase


[Source: Ranganathan, ISTFA 2017]


• Phase provides additional information about signal  propagation


• Scan in = 0011 will have 4 phases


• Scan Chain Failure, but LVI unable to detect any


anomaly


• Output pin is not stuck


• Phase LVI identified a phase mismatch from


expectation, identified nearby aggressor


• Physical analysis showed metal short as suspected


– Emission-based (PEM, Thermal, Spectroscopy)


– Laser-based (LVP)


Logic Waveform Mapping: Inverter


C9 OUT


INT


IN  OUT


Inverter


waveforms   are expected


Logic Waveform Mapping: AND


OUT  A


B


unexpected


C3


INB


OUT


INA


expected


States of an inverter


The output of inverter 1 is low to high  The output of inverter 2 is high to low


28 nm  bulk


Schematic


• LVP response of inverter is straightforward


• Input goes high, output goes low


• Signals are 0 or 1,  only 2 states


Combinational logic analysis of NAND


• Truth table only has ‘0’ or ‘1’


• LVP depends on number of Channels ON


• Two PMOS channels in parallel


• One PMOS channel ON = ‘1’


• Both PMOS channels ON = ‘1+’


NAND


Combinational logic analysis of NOR


• Two PMOS channels are in series


• Both PMOS channels are ON = ‘1’


• One PMOS channel is OFF = ‘0’


• Both PMOS channels are OFF  = ‘0-’


NOR


CASE STUDY: 2-input NAND


• Diagnostics says OPEN/DOM CELL


• Output  has flat states and sharp toggles


• Library comparison shows mismatch on cycles 2,3,4,6


• PFA confirms net B short to VDD


Mismatches


Mismatches when B = 0


NAND  Schemat ic


• Laser Voltage probing is the most  deterministic way to check if a


particular transistor is toggling the  way as we expected it to


Useful for Pattern Verification


•  Is the pattern running?


• Is the data propagation correct?


Pattern1


Pattern 2


The 2 patterns are sending  different logic to the node on  this vector


• LVP is useful even when the defect is not in the


• Scan logic failure


• Signal probed on launch cell shows good signal


• Signal reached first 2 capture muxes, but missing on


third


• Missing via observed between mux 2 and 3


LVP results


Schematic view of callouts


SEM Inspection


Layout view of callouts


• Analog failure, output had bad duty cycle


• Probing within the cell showed triangular waveforms


• Input to the cell looked okay


• Nanoprobing on the failing device showed N-P ratio


mismatches


Internal net  INPUT


Final output


Output driver


GOOD UNIT


REJECT UNIT


INPUT


Internal net


• The time resolution of the tool is better than 20ps


• We can also estimate the delay between cells in a  path to compare against design simulations


ΔT(cell2 – cell1) = 190ps ΔT(cell3 – cell2) = 210ps ΔT(cell4 – cell3) = 240ps


Timing measurements


Timing resolution


Path delay, cell delay


design simulations can be  verified with LVP


Clock


Path delay


Cell delay


Cell1


Cell2


Cell3


Cell4


• LVP excellent for hold and setup time violations


• These are fundamental design considerations


• VMIN/VMAX/speed limitations are almost always


due to setup or hold violations


• Setup time: how early the data should reach  before the clock


• Hold time: min time after the clock the data  should hold before the cell can latch the data


Timing violation


Clock  Data


setup time


Hold time


Data


Technology Scaling


• As features become smaller, more transistors fall within the optic probe location


• Causes electro-optic crosstalk


• CAD alignment is a problem as well


• Besides scaling, FINFETs have directional properties


• Polarization of light is important consideration


PLANAR TRANSISTOR FINFETs


New materials and


geometry


Polarization of optic probe


will influence how it interacts  with the device


Need for Resolution


• NA scaled first -> approached refractive index


• Now scaling wavelength -> short wavelength probing


Resolution advancement λ


NA


Gen1 1320nm


2.4


Gen2 1320nm


2.65


Gen3 1320nm


Gen4 1064nm


3.3


Gen5


785nm


2.9


Gen6


577nm


32nm   28nm  20nm   14nm   10nm   7nm    5nm


Gen1   Gen2   Gen3   Gen4   Gen5  Gen6


Spot Size


Abbe’s limit


2x contacted poly pitch


nm


[Source: en.wikichip.org


CAD alignment requires better optical  resolution


• Short wavelength allow much better CAD alignment


0.1um


Shorter Wavelength Probing


• Sample preparation to below 10um residual silicon thickness


• Thermal control, hard to dissipate heat from localized heat emitters


• Laser waveforms show effects of invasiveness


Ultra-thin Sample show bump  profiles


Waveforms using visible probe


Waveforms do not  have sharp


transitions or flat  states as NIR


[Source: Christian Boit, IPFA 2016]  [Source: T.Eiles, ISTFA 2016]


CW-LVP Enhancements


1. High NA solid


immersion lens


2. Wavelength


compatible


optics


1. Different  wavelengths


2. Lower  noise


Polarization


1. High frequency


detector


2. Low Frequency


1. Filters


2. Amplifiers


1. Spectrum


analyzer


2. Lock-in Amplifier


1. Oscilloscope


2. Digitizer


Software 1. Signal interpretation


2. Auto focus, alignment, drift correction


Overview of LVx Technologies


• Laser probing and frequency mapping are power fault isolation techniques


– First silicon debug


– Failure analysis


– Timing violations and speed path analysis


– Pattern verification


• Most deterministic technique


• Frequency mapping is a global technique but limited to periodic signals


• Laser probing works on a single transistor at a time


• Laser probing can work for most tests, even aperiodic signals


• Resolution constraints cause crosstalk and shorter wavelength light can


help


Cross-Functional Approaches


• No one technique that is  formidable


• Gap analysis


– Theoretical limits (Resolution & Sensitivity)


– Capability (defect coverage) – Productivity (FA process)


Failure  Analysis


Design


IT


Time Resolved Laser Assisted Device  Alteration


• Pulsed NIR laser, precisely timed, instead of continuous laser


• Useful for understanding which test cycles in a test are critical


• Can identify when exactly a critical signal passes through a path


• Reduces average laser power, while higher peak power for critical cycles


• Higher spatial resolution than regular LADA


• Single event upsets can be created


Different pulsed laser options


• Pulsed laser is useful for analog and high speed debug


• By limiting the dwell time of photons within Silicon, generated carriers have shorter life


time and reduced invasiveness


Passing band


• Fs Pulsed laser can be used to identify signal


propagation delay in a critical path


[Source: K. Erington, IRPS 2014]


2photon Laser Assisted Device Alteration


• 2 photon LADA also uses pulsed laser. The principle of operation is frequency addition


which is a non-linear effect that can occur when a high intensity of photons are confined to


a tiny spot.


• Fs pulsed laser with photon energy <


bandgap of Silicon [for high transmission


through Si]


• Frequency is doubled at the focus point of


laser


• Resultant photon has higher energy than


bandgap and injects carriers


Technique able to achieve higher resolution


than other techniques


[Source: K Serrels , OPTICS EXPRESS  2013]


LVP Challenge: Optical Resolution


• Optic probe profile (L) = intensity distribution of the probe


• Modulation capacity (M) = amount of modulation achieved in an area


• Change in reflectance   ∝  L * M


• Total change in reflectance = sum of changes caused by individual


modulating devices


Figure 1: Simplified model of the optic probe profile relating


1 Transistor


6-9 Transistor


the probe diameter to the NA and wavelength


Optic Probe profile


Pattern Comparison


• Good match between simulation (CLA) and actual waveform (LP)


• The match can be further improved through automation


Number of bins


net 4  net 2


Picosecond Imaging for Circuit Analysis


• Based on hot carrier emission in the transistor


• created by the transient current pulses present in the transistors during


switching


• Single-photon detector


PICA low jitter allows to separate events close in time and  accurately measure small propagation delays


Separating closely spaced gates  using time-knob


[Source: F. Stellari, ISTFA 2013]


[Source: Bahgat Shehata, ISTFA 2014]


Use of Analog Simulation in Failure Analysis


[Source: Etienne Auvray ,ISTFA 2018]


Anomaly


Automated Multi-level Trace


S/D


1st


2nd


additional  3rd


Artificial Intelligence Offers Opportunities


• Enhanced


Productivity


• Abilities to


provide NEW  INSIGHTS


Opportunities for FA: Machine Learning


1950s 1960s 1970s 1980s 1990s 2000s 2010s


Failure Analysis


Artificial Neural Network


• Productivity


enhancement


Fail dies


Characterization (static current, dynamic current)


Trained System


Fail dies w/ extreme  anomaly


Predict PFA positive


• New opportunities


Fail dies w/ subtle  anomaly


[Source: Zhao lin ,IPFA 2018]


Extreme and Subtle Leakage Current Fail Dies


Dynamic current


Static current


• Decisions on subtle fail dies – 1) Should we ignore? 2) Which to select


Subtle Leakage Example


Dynamic PEM


Facial Recognition


[Ref: Mirza Saquib Us Sarwar, TENCON, 2010 ]


• row-by-row feature extraction -> compare


Comparison Scheme


• Extraction from reference image to create an intensity matrix


• Cross-correlation of test images Ix to intensity matrix


• Generation of similarity score


• Classification of test images


Enhanced EeLADA


• Pixel-by-pixel ‘feature’ extraction


• Multiple fail pins => 3D vector; 1 fail pin => 2D vector


[Source: Man hon Thor, ISTFA 2018]


MBIST Fault Localization


Technical Signal Image


Technical Signal Overlaid Image


Periphery Defect Bitmap Interpretation


Programmed   defect


• Accuracy ~ 1.5 mm


• More precise localization than bitmap


Bitmap Results


Overview Of Content


– Time-resolved LADA


– 2pLADA


– Circuit Simulation for LVP and Emission predictions – ANN for FA success prediction


– Facial Recognition concept for EeLADA


Conclusions


• 100% impactful FA success is important


• Multiple gaps (defect detection, technique limitations, alternative approaches, productivity etc) still exisit


• Innovation


– Improve current technologies


– Look beyond FA (cross-functional domain learnings)


Thank you for your attention

