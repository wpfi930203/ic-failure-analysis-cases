---
title: "tutorial_note_cher_ming.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_755633fa61fc545dc35b8fb5cfc98ce37295230462135641
file_size: 4355674
---

![coe  FH3O  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e15af004-4139-4ed7-bd8c-4a9e8d7451b4/e15af004-4139-4ed7-bd8c-4a9e8d7451b4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=64497e6fc851721ce6d5cf7bb68823e492cfb5f8)
## Failure mechanisms and root  cause analysis 

## Cher Ming Tan, Ph.D 

Director, Center for Reliability Sciences and Technologies   Professor in Electronic Engineering, College of Engineering   Chair Professor in Mechanical Engineering, Ming Chi University    of Technology, Taiwan   Fellow of Institute of Engineers, Singapore; Fellow of    Singapore Quality Institute   IEEE EDS Distinguished Lecturer,    Editor, Scientific Report, Nature Publishing Group   Editor of IEEE Transaction on Devices and Materials Reliability,    Series Editor of Springer Brief on Reliability   Member of Advisory Panel, Elsevier Publishing Group   Technical committee in IEEE Standards 1413.1 and 1624   Email ID:  cmtan@cgu.edu.tw ; cherming@ieee.org

## Outlines 

• Definition of Failure mode, failure mechanisms and root causes   • FMEA and FMMEA   • Some examples of Failure mechanisms in microelectronics   • Case studies on Failure mechanisms and root causes    identification • LED degradation in outdoor application • PCB burnt in public transport application   • Conclusion

## Definition 

•  Failure Modes are associated with deviant function or  behavior. Examples of failure modes are:

• Ductile fracture.   • Brittle fracture.   • Fatigue fracture.   • Corrosion.   • Erosion.   • Wear   •  Basically, the phenomenon of failure that can be observed or    measured are all belong to failure mode.

## Failure  mechanisms 

•  Failure Mechanisms are  associated with deviant physical  condition or physical state . •  They are the underlying physics  or chemistry of the failure mode.

|FailedPart|FailureMode|Failure Mechanism|
|---|---|---|
|chp|ooen|        Aluminum wiring disconnection (corrosion,                migration,latch-up)                Bonding pad corrosion                Paly Silicon wiring disconnection(melting)                Bondpeeling(formation ofAu-Al and other                intermetallic                compounds)      |
|chp|Shorts|        Oxide film breakdownor pinhole                Electrostaticbreakdown                PN junction degradation                Interlayer insulatorbreakdown orpinhole                -Conductive foreignmatter                Contamination within the process                .Chip cracking                Entry of moisture      |
|chp|        IC functian                faidre                (characteristie                fluctuation and                functionfailure)      |        Hot electron or hot carrier injection to the oxide                Surface inversion                .Crystal defect                Contamination within the process      |
|chp|Malfunction|        ·Softerror                Latch-up                Electromagnetic interferenoe[EMI)      |
|Package|open|        ·Bonding wire disconnection or peeling                Lead dirtiness,stress due to oxidation or absorbed                moisture                +heatstress      |
|Package|        Package                cracking                shorts or leaks      |        De-laminatian between the chip or leadframe and                motdresin                Wire touchingcontact between the wires,chip                andead                frame)                Electrochemicalmigrationbetweenleads      |
|Package|Soldering defect|Surface contamination of oxidation|


•  Identify failure modes are  relatively easy, but to identify  and confirm failure mechanisms  requires good knowledge of the  physics of failure and material  sciences

## Root Causes 

• According to Collins English Dictionary, root cause is the  fundamental reason for the occurrence of a problem.

• In engineering, root cause is the main reason why the failure  mechanism can occur.

• Examples of root causes are

• Conduction wire too thin for the current to be passed    through   • Process contamination that leads to low oxide breakdown    voltage   • Electrode area too small that lead to excessive heating that    cause battery to explode

Identify root causes requires good knowledge of failure  mechanisms and detail product/process knowledge

5

## Failure Mode and Effects  Analysis (FMEA) 

A systematic approach to identify failure modes

## Introduction 

• FMEA is an analytical technique used by engineers to ensure that potential  problems have been considered and addressed.     • It is a summary of the engineer’s thoughts as he or she designs a  component or a system or develops a process.   • It can help to improve the quality and reliability of products and processes.   Thus, maintain a competitive edge of a company.   • It is a living document which changes along the product life cycle   • A team effort of a cross functional team is necessary for FMEA to be  effective

## Introduction (Illustration using Process FMEA) 

• It identifies potential product related process failure modes   • It assesses the potential customer effects of the failures   • It identifies the potential manufacturing or assembly process causes and   identifies process variables on which to focus controls for occurrence   reduction or detection of the failure conditions   • It develops a ranked list of potential failure modes, thus establishing a   priority system for corrective action considerations   • It documents the results of the manufacturing or assembly process

## Potential Failure Modes 

• The way a product could fail to fulfill the design intent or process  requirements

• Caused by deficiencies in product design or production process

• We spend a lot of time and money correcting failure modes that have  already occurred.  It would be more cost-effective to identify and correct  the design and process deficiencies that cause them.  This is what FMEA  is for.

## Failure Mode and Effect Analysis 

• A systematic method of identifying, prioritizing and acting on potential  failure modes before they occur   • A proactive, preventive approach to product failures, rather than an afterthe-fact analysis.  Hence, it relies on product knowledge, engineering  expertise and intuition, rather than mathematical formulas   • Goal:  prevent the customer from experiencing the negative effects of  failure modes

## Failure Mode and Effect Analysis 

• FMEA helps determine:

• How could the product fail?   • What effect would the failure mode have?   • How severe is the effect?   • What could cause the failure mode?   • How likely is it to occur?   • What controls are in place?   • How effective are they?   • What is the overall risk?   • What can be done to reduce the risk?

## Failure Mode and Effect Analysis 

• The Risk Priority Number is used to rank order failure modes in terms of  their relative risk.

• The failure mode with the highest RPN is the most serious and warrants  corrective action first, and so on down the list.

## Background 

• FMEA was developed as a formal methodology in the 1950s at Grumman Aircraft  Corporation, where it was used to analyze the safety of flight control systems for  naval aircrafts.  • From the 1970s through the 1990s, various military and professional society  standards and procedures were written to define and improve the FMEA  methodology (Bowles 2003; Guidelines for Failure Mode and Effects Analysis 2003;  Kara-Zaitri et al. 1992). • In 1971, the Electronic Industries Association (EIA) G-41 committee on reliability  published “Failure Mode and Effects Analysis.” In 1974, the U.S. Department of  Defense published MIL-STD 1629 “Procedures for Performing a Failure Mode,  Effects and Criticality Analysis,” which through several revisions became the basic  approach for analyzing systems.  • In 1985, the International Electrotechnical Commission (IEC) introduced IEC 812  “Analysis Techniques for System Reliability—Procedure for Failure Modes and  Effects Analysis.”

## Background 

• In the late 1980s, the automotive industry adopted the FMEA practice.    • In 1993, the Supplier Quality Requirements Task Force comprised of  representatives from Chrysler, Ford, and GM, introduced FMEA into the  quality manuals through the QS 9000 process.    • In 1994, the Society of Automotive Engineers (SAE) published SAE J-1739  “Potential Failure Modes and Effects Analysis in Design and Potential Failure  Modes and Effects Analysis in Manufacturing and Assembly Processes”  reference manual that provided general guidelines in preparing an FMEA.    • In 1999, Daimler Chrysler, Ford, and GM, as part of the International  Automotive Task Force, agreed to recognize the new international standard  “ISO/TS 16949” that included FMEA and would eventually replace QS 9000 in  2006.

## Background 

• Factors contributing to the spread of FMEA

• rapid advancements in technology are forcing manufacturers to  develop new products more quickly to remain competitive.  With less  time for testing and redesign, they must achieve their reliability target  the first time around   • Foreign and domestic competition has raised customers’ expectations  for quality and reliability   • The trend toward litigation has forced manufacturers to exercise  greater care in the design and manufacture of their products   • Some manufacturers require that their suppliers use FMEA (QS9000)

## Applications 

• Advanced product quality planning   • Problem solving   • Continual improvement   • Product design   • Manufacturing and assembly processes   • Improve reliability of the product

## Applications 

• Design FMEA • help eliminate design-related failures, i.e. Failures due to inadequate  strength, inappropriate material etc.   • Process FMEA • help eliminate failures that result from changes in process variables,  i.e. Out-of-spec conditions such as wrong size, hardness etc.   • Service FMEA • help eliminate product failures due to improper installation, operation,  maintenance and repair.

## Benefits 

• Reduces number of product failures  experienced by customers, hence  improve customer satisfaction • bathtub curve - infant mortality,  useful life and wearout • Infant mortality period - its  failure can be reduced by  process FMEA • Useful life period - its failures  can be reduced by design  FMEA • Wearout period - its failure can  be delayed by service FMEA

![Failure Rate  Process  FMEA   Design FMEA   Design FMEA  Early Life   Useful Life   Wear-out  Product Life Cycle  Failures due to  deficiencies in:   Production   Design   Design  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bac63b63-a4cd-49a8-bce4-d0b3b15cbe44/bac63b63-a4cd-49a8-bce4-d0b3b15cbe44.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=a69852a072fe8117245e53de0ae1b16869ae6b21)
Bathtub Curve

## Benefits 

• Shortens lead time to introduce a new product or start up a process, since  there are fewer problems requiring engineering changes.

• Cost avoidance • fewer engineering changes • less scrap and rework • less time and dollars spent troubleshooting • reduced installation and service costs • reduce product warranty costs • reduce potential for liability suits

## Benefits 

• Cost Effective

• FMEA is a small addition to the design phase workload, with the potential to greatly  impact succeeding phases of the product development cycle   • FMEA simply provides more discipline and structure to the failure analysis activity for  engineers on their designs.

## • Versatile 

• Can be applied to any product in any industry   • Does not require extensive formal training   • Based on logic and intuition, rather than mathematical formulas   • Useful to individuals from all disciplines

## Other Benefits 

• It can improve an organization’s image and competitiveness   • It can shorten the learning curve associated with a new product or process • It allows more efficient allocation of resources because management has  better information about potential problems and appropriate corrective  actions   • It can save time down the road when similar products or processes are  being designed.   • So, FMEA makes good business sense.

## Key Elements of an Effective FMEA 

![How is quality designed into the system?  Concept design   +Customer-driven specificalions  +FMEA  ·Design of experiments [classical or Toguchi]  How is testing maximized?  Development   ·Reliability growth  +FMEA  +DOE  ·What kind of tests are effective?  How can it be tested?  Validation test   +What kind of samples should be obtained?  ·What kind of testing should be done?  ●How long should the testing be?  |s reliability testing oppropriate?lf so, what kind?  ls occelerated testing opplicable?  How can the process be kept in control  and improving?  Process   +FMEA  +Stalistical process control  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6e66ae90-23fa-41e2-94b3-8f72b271d2b8/6e66ae90-23fa-41e2-94b3-8f72b271d2b8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=f244025ac98194a6596796bc0e1550457c33da0d)
## FMEA Team 

• It requires a team approach. • Only a team can provide the range of technical expertise and experience  needed to identify all potential failure modes, accurately assess their  effect, and recommend appropriate action. • The size and composition of the team will depend on the product or  process being analyzed.  It should be cross-functional team that  represents all the areas involved in the design or production of the  product. • Team members should also represent a variety of disciplines- engineers,  technicians, line operators etc.

## Documentation 

• An FMEA is documented on a special form which is saved and updated  throughout the life of the product or process.  It is a  “living document”.

• The FMEA form serves many purposes:

• It helps lead the team through the analysis in a logical sequence   • It captures the design rationale for the product or process so that future teams don’t  have to “reinvent the wheel”   • It acts as a catalyst to stimulate the exchange of ideas among team members.  As a  result, the product or process is subjected to a more rigorous and productive analysis   • It also makes communication easier because team members are working from the  same model.

## Documentation (FMEA revision) 

• Considerable time and resource will have been utilized in the preparation  of an FMEA.  To maximize its use and benefits, design and process  modifications which affect the validity of the analysis must be investigated  and the FMEA updated, as necessary.  The changes should be recorded  for future reference and the revised document re-issued.

• Procedures for updating FMEAs must be considered.  Creating this  discipline ensures continuous re-evaluation of potential failure risk, thus  providing on-going product control.

## Documentation (FMEA revision) 

• FMEA updating may be integrated into existing systems, or the systems may  have to be modified to cater for such changes.  Changes and events which would  prompt a revision to an FMEA (design or process) could include:

• customer complaints and warranty returns    • proprietary part design modification   • specification change    • alternative processes    • process alteration - material/routing/handling    • increased or reduced process capability   • revisions in tooling fixture or assembly aids    • routine process and quality performance changes initial sample rejection    • gauging methods.

## Types of FMEAs 

## • System FMEA 

• Used to analyze systems and  subsystems in the early  concept and design stage.     • It focuses on potential failure  modes between the functions of  the system caused by system  deficiencies   • It includes the interactions  between systems and elements  of the system

• The output of the system FMEA is • a potential list of failure modes  ranked by the RPN • a potential list of system  functions that could detect  potential failure modes • a potential list of design actions  to eliminate failure modes,  safety issues, and reduce the  occurrence

## System FMEA 

• The benefits of the system FMEA are

• helps select the optimum system design alternative   • helps in determining redundancy   • helps in defining the basis for system level diagnostic procedures   • increase the likelihood that potential problems will be considered   • identifies potential system failures and their interction with other    systems or subsystems

## Design FMEA 

• It is used to analyze product before  they are released to manufacturing.

• It focuses on failure modes caused by  design deficiencies

• Output of the design FMEA

• a potential list of failure modes ranked  by the RPN   • a potential list of critical and/or  significant characteristics   • a potential list of design actions to  eliminate failure modes, safety issues,  and reduce the occurrence   • a potential list of parameters for  appropriate testing, inspection, and/or  detection methods   • a potential list of recommended actions  for the critical and significant  characteristics

## • Benefits of the design FMEA 

• establishes a priority for design  improvement actions   • documents the rationale for  changes   • provides information to help  through product design verification  and testing   • helps identify the critical or  significant characteristics   • assists in the evaluation of design  requirements and alternatives   • help identify and eliminate  potential safety concerns   • helps identify product failure early  in the product development phase

## Process FMEA 

• It is used to analyze manufacturing and  assembly processes

• It focuses on failure modes caused by  process or assembly deficiencies

## • Output 

• a potential list of failure modes ranked by  the RPN   • a potential list of critical and/or significant  characteristics   • a potential list of recommended actions to  address the critical and significant  characteristics   • a potential list to eliminate the causes of  failure modes, reduce their occurrence,  and improve defect detection if Cpk cannot be improved

• Benefits of the Process FMEA

• identifies process  deficiencies and offers a  corrective action plan   • identifies the critical and/or  significant characteristics  and helps in developing  control plans   • establishes a priority of  corrective actions   • assists in the analysis of the  manufacturing or assembly  process   • documents the rationale for  changes

## Service FMEA 

• It is used to analyze services  before they reach the customer.

• It focuses on failure modes (tasks,  errors, mistakes) caused by  system or process deficiencies

## • Output 

• a potential list of errors ranked by  RPN   • a potential list of critical or significant  tasks, or processes   • a potential list of bottleneck  processes or tasks   • a potential list to eliminate the errors   • a potential list of monitoring  system/process functions

## • Benefits of the Service FMEA 

• assists in the analysis of job  flow   • assists in the analysis of the  system and/or process   • identifies task deficiencies   • identifies critical or significant  tasks and helps in the  development of control plans   • establishes a priority for  improvement actions   • documents the rationale for  changes

Relationship of system, assembly and

part FMEA

![System FMEA  Failure   Effect   cause  niode  The problem   The ramifications   The cause[s] of  of the problem   the problem  AssemblyFMEA  Failure   Effect   Cause  mode:  The causes of   The effect from the   Newroot causes  the problem   systemFMEAwith   for the ossembly  from the system   perhaps a belter   failure modes  FEA   definition  Part FMEA  Failure   Effect   cause  mode  The causes of   The same effect as   Specific root  the problem from  the assembly   causes for the  fhe assembly   FMEA   assembly failure  FNEA   modes  Note: The failure modes of the system FMEA generate allthe essential information for the  assembly and part FMEA.Although the effect stays the same,the causes in the system  FMEA become the failure modes in the assembly, which in turn generate their own  causes, which ultimotely become the failure modes in the part FMEA.  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d6938786-7c15-43d2-b25c-25b46035e622/d6938786-7c15-43d2-b25c-25b46035e622.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=7ce2d96a5c66d34756114e2b2b8fa4c474aaf9a2)
## Specific questions in the course of  performing a design FMEA 

1.  What does the product do and what are its intended uses?   2.  How does the product perform its function?   3.  What raw materials and components are used to build the product?   4.  How, and under what conditions does the product interface with other   products?   5.  What by-products are created by the product or by the use of the product?   6.  How is the product uses, maintained, repaired, and disposed of at the end of   its useful life?   7.  What are the manufacturing steps in the production of the product?   8.  What energy sources are involved and how?   9.  Who will use or be in the vicinity of the product, and what are the capabilities   and limitations of these individuals?


## A typical example of FMEA form 

## Design FMEA 

System  FMEA Number Subsystem  Page. Component  Design Responsibility  Prepared by. Model Year(s)Wehicle(s)  Key Date FMEA Date (Orig.)  {Rev.] Core Team

|Function|        Potential                Failune                Mode      |        Potential Etect(s)                Ol Failune      |||        Potential Cause[s)                Mechanism(s)                Qf Failure      ||        Current Design                Contro-ts      ||中|        Recommended                Action(s)      |        Responsibility                        Completion                Dae      |Action Results|Action Results|Action Results|Action Results|Action Results|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|Function|        Potential                Failune                Mode      |        Potential Etect(s)                Ol Failune      |||        Potential Cause[s)                Mechanism(s)                Qf Failure      ||        Current Design                Contro-ts      ||中|        Recommended                Action(s)      |        Responsibility                        Completion                Dae      |        Actions.                Taken      ||||.|
||||||||||||||||||
||||||||||||||||||


## Failure Modes and Mechanisms  Effect Analysis (FMMEA)  

Knowing failure modes are not sufficient to prevent recurring  failures and solve the failure issues, understanding of the  failure mechanisms are necessary.

Also, accelerated life testing requires the knowledge of  failure mechanism, instead of failure mode

## Introduction 

• FMMEA enhances the value of failure modes and effects analysis (FMEA)  and failure modes, effects, and criticality analysis (FMECA) by identifying  the “high priority failure mechanisms” to help create an action plan to  mitigate their effects.    • Failure mechanisms are the processes by which specific combinations of  physical, electrical, chemical, and mechanical stresses induce failure. Neither FMEA nor FMECA identify the failure mechanisms and models in  the analysis and reporting process.    • In order to understand and prevent failures, failure mechanisms must be  identified with respect to the predominant stresses (mechanical, thermal,  electrical, chemical, and radiation) that precipitate these failures.    • Understanding the cause and consequences of failure mechanisms aid the  design and development of a product, including accelerated testing, rootcause analysis, and life consumption monitoring.

## Introduction 

• For accelerated testing design, one also needs to know the failure  mechanisms that are likely to be relevant in the operating condition.  • Only with the knowledge of the failure mechanism, one can design  appropriate tests (stress levels, physical architecture, and durations) that  will precipitate the failures by the relevant mechanism without resulting in  spurious failures. • All the root-cause analysis techniques, including cause and effect diagram  and fault tree analysis, require that we know how the conditions during an  incident may have an impact on the failure.  • The hypothesis development and verification processes are also affected  by the failure mechanisms analysis.  • Knowledge of failure mechanisms and the stresses that influence these  mechanisms is an important issue for life consumption monitoring of a  product.

## Introduction 

• To make sure that the appropriate data are collected and utilized for the  remaining life assessment during health monitoring, the prioritized list of  failure mechanisms are essential. • The traditional FMEA and FMECA do not address the key issue of failure  mechanisms to analyse failures in products.  • To overcome this, a FMMEA methodology has been developed.  • The FMMEA process merges the systematic nature of the FMEA template  with the “design for reliability” philosophy and knowledge. In addition to the  information gathered and used for FMEA, FMMEA uses application  conditions and the duration of the intended application with knowledge of  active stresses and potential failure mechanisms.  • The potential failure mechanisms are considered individually and are  assessed using appropriate models for design and qualification of the  product for the intended application.

## Introduction 

• FMMEA is a systematic approach to identify and prioritize failure  mechanisms and models for all potential failures modes.

• High priority failure mechanisms determine the operational stresses and  the environmental and operational parameters that need to be controlled  or accounted for in the design.

• FMMEA is based on understanding the relationships between product  requirements and the physical characteristics of the product (and their  variation in the production process), the interactions of product materials  with loads (stresses at application conditions), and their influence on  product failure susceptibility with respect to the use conditions.

• This involves finding the failure mechanisms and the reliability models to  quantitatively evaluate failure susceptibility.

## FMMEA  methodology 

![FMMEA  Material  Defineitem andidentify  propertiesand  elementsand functions  product  tobe analyzed  geometries  Estimatedlife   Identifypotentialfailure   Monitorlifecycle  cycleloading   modes   environmentand  operatingloading  Identifypotentialfailure  causes  Identifypotentialfailure  mechanisms  Identifyfailuremodels  Maintenance   Prioritizethefailure  records   mechanisms  Choose  monitoring  Documenttheprocess  parametersand  locations  40  40 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2aab612a-b93c-4b11-b455-2c9815a352ad/2aab612a-b93c-4b11-b455-2c9815a352ad.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=c76c995cf2093e334587ab6a6d4e234b50b1b691)
## Identifying Failure Mechanisms 

• Prior knowledge of available failure mechanisms will be useful.   • Attending related conferences such as IRPS, IPFA etc will be an    avenue   • Professional courses on failure mechanisms are available.   • Research Lab on failure physics and reliability will be helpful.

## Case Study of Failure  Mechanism on LED dimming  under outdoor applications 

HB LED  Applicatio n Space

![Other   MobileAppliances  Indicators,small displays  Illumination  amusement,misc.other  HBLED  Market  SignsandDisplays  Signals  UTUITY-VS  THREESYOU  Automotive  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6948fd45-8cfb-448a-8d5a-b13f3f36fece/6948fd45-8cfb-448a-8d5a-b13f3f36fece.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=7eccda1c64dcaae28e80726b0da4ff69bb62eed2)
Many applications of HB LEDs will be exposed to high humidity in outdoor environments  http://www.signindustry.com/ledlighting/articles/2006-04-03-LB-HighBrightnessLEDs.php3

• A total of 15 units of OSRAM’s 3-W Platinum DRAGON white packaged LEDs are placed in a life test  humidity  chamber  (Weiss  Gallenkamp SB11/300/800) with test condition set at different temperatures and RH

## Experimentation 

• During the humidity test, all LEDs are switched off to  prevent  the  trapped  moisture  in  the encapsulation from being evaporated by the heat generated during operation.

• The LEDs are removed from the humidity chamber at  specific  intervals  to  have  their  electrical parameters measured using a multichannel  I – V Keithley 2602A meter and their optical parameters (2 π  forward  flux)  measured  by  an  optical measurement system comprising a 1-m-diameter integrating sphere (Gigahertz-Optik UMBB-1000) and a spectroradiometer (Optronic Laboratories OL770).

## Experimental Results – Three Stages of  Degradation Modes 

![30 30  25 25  LUMENS DEGRADATION (%) N  NO  20 15 10 5 0 24 24   48 A8   72 NN   1２0  120  144  144  396  396  420  420  444  444  588  588 Test time (Hours)  Test time (Hours) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/288c7246-5364-4d75-b6f9-440bc0879b28/288c7246-5364-4d75-b6f9-440bc0879b28.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=0e6b3beea37620b5f819c6bd4a91bdc1ceb83d00)
Percentage luminous flux degradation vs. time for   $95\%$    RH set of LEDs.

![14Samples96120144168360384408456480552796844 TA  12 Percentage lumens degradation 10 8 6 4 2 0 Test time (Hrs) Testtime(Hrs)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/67ae007b-f29d-4d17-aca4-e5307f081938/67ae007b-f29d-4d17-aca4-e5307f081938.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=2ac939e25f422447a85d9d20089af67940952e33)
Percentage luminous flux degradation vs time for   $85\%$    RH set of LEDs.

## Stage 1 Degradation  Mode 

• We have shown the following:

• Not chip degradation   • Not phosphor degradation   • Due to moisture in the silicone encapsulation   • Due to light scattering by the moisture particles instead of light absorption

But why the degradation recover?

"Uncover the degradation science of silicone under the  combined temperature and humidity conditions."  IEEE  46   Access  6 (2017): 1302-1311.”

![100.1  100.1 100.0 100.0  99.9  99.9 99.8  99.8 Weight (%)  99.7  99.7 unstressed LED 1  unstressed LED 1  unstressed LED 2  unstressed LED2  99.6  99.6  LED 3 (24 hours)  LED 3 (24 hours)  LED 4 (24 hours)  LED 4 (24 hours)  LED 5 (24 hours)  LED 5 (24 hours)  99.5  99.5 LED 6 (48 hours)  LED 6 (48 hours)  LED 7 (48 hours)  LED 7 (48 hours)  99.4  99.4  LED 8 (48 hours)  LED 8 (48 hours)  99.3  99.3 ③0  30  50  50  70  90  90  110  110  130  130  150  150  1７0  170 Temperature (°C)  Temperature  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1d00f92c-c1cc-4be0-be58-59103962c73c/1d00f92c-c1cc-4be0-be58-59103962c73c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=ebde870aa6c307dd837efab3127dae5ad2534a9e)
Weight changes   $(\%)$   of the LED as a function of  temperature after the LEDs are subjected to   $85\%\mathrm{RH}$   and 85C.  It represents the saturation of  moisture absorption for silicone.

![ANSYS  NODAL SOLUTION  NOV62014  STEP=1  15:53:09  SUB=24  TIME=24  TEMP   (zG)  RSYS=0  SMN =.274E-11  SMX=.85  274E   188889   377778   .566667   755556  094444   283333   472222   661111   8S  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/00eb648b-9fb7-44be-8bdc-b51d35539184/00eb648b-9fb7-44be-8bdc-b51d35539184.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=b9ef4c4810f57586f7b7fe8f6cc1bc01d2df5250)
## Moisture concentration vs. Time 

• The  ratio  of  the  peak average  moisture concentration  in  silicone from 95%RH to 85% RH is 1.12.

• This is comparable to the ratio  of  the  peak  lumen degradation from 95% RH to 85% RH which is 1.25 as determined experimentally.

![0.8  0.2  0.6   Average  Average  0.5   moisture  moisture  concentrati  concentrati S   0.4  on in  on in  0.3   silicone cilian  ezi   Average  Average  0.2   moisture  moisture  concentrati O.1   concentrati  on in Die  Attach Attach  100   200   300   400   500  -0.1  Time(Hrs)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5b7e96cc-344a-48f1-ba41-8219be31798a/5b7e96cc-344a-48f1-ba41-8219be31798a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=7e9a18dcbd2f4e4077a5017d30332d5ac814a510)
Time to Peak Lumen Degradation

|85% RH and 85C|85% RH and 85C|85% RH and 85C|95% RH and 85C|95% RH and 85C|95% RH and 85C|
|---|---|---|---|---|---|
|Time||Time for moisture|Time||peak   Time for moisture|
| Iumen||flux       shift| lumen||flux       shift        from |
|degradation|silicone       td||degradation||silicone       td|
|(Experimental)|attach||(Experimental)||attach|
||(simulation)||||(simulation))|
|120 Hours|105 Hours||72 Hours||78 Hours|


## Permanent Degradation 

## Degradation mechanisms of LEDs at  different RH 

Distribution parameters of the dominant degradation  mechanism at different RH at 85C

|        Lognormal                Distribution                parameters      |95% RH|95% RH|95% RH|85%RH|85%RH|85%RH|70% RH|70% RH|70% RH|
|---|---|---|---|---|---|---|---|---|---|
|        Lognormal                Distribution                parameters      |Degradation %|Degradation %|Degradation %|Degradation %|Degradation %|Degradation %|Degradation %|Degradation %|Degradation %|
|        Lognormal                Distribution                parameters      |50/0| 1 00/| 1 50/。|59/0|1 00/| 1 50/|59/0|1 00/| 1 50/|
|T5o (hours)|99.13| 147.21|186.72|110|185|403.4|232.|389.0|434.4|
|Shape parameter|0.5|0.26|0.34|1.97|2.89|0.43|0.73|0.75|1.33|
|        Incubation       tinm e                (hours)      ||||19|③0|60|||230|
|        Incubation       tinm e                (hours)      ||||19|||||230|


Cher Ming Tan and Preetpal Singh, “Time Evolution Degradation Physics In High Power White  LEDs Under High Temperature-Humidity Conditions”, IEEE TDMR, Vol 14(2), June 2014

Degradation  mechanisms  of LEDs at  different RH

• From the previous findings, we can see that  the shape parameters at each %  degradation are different, indicating that the  degradation mechanisms at each %  degradation are different, i.e. the  degradation physics is evolving with time.  • Also, the shape parameters at a given %  degradation are different at different %RH. •  This implies that no extrapolation is  possible from 95% to 85% to 70% RH. • In other words, the test data at 85%RH and  85 o C cannot be used to estimate the life  time of LEDs under lower humidity condition  as the acceleration is not linear, and Peck  model is not applicable.

Time Evolution    of the    degradation   Using 70%RH    and 85C as    example

•  The degradation process begins from bond pad contamination and Kirkendall void  formation,  galvanic  dissolution, phosphor  dissolution to encapsulant, and die attach delamination.

![Readepositionhef baon A   AuBal   Kirkendall void formation and Corrosion Kirkendall void formation and Corrosion   dissolution dissolution  Phosphor  Phosphor  PartA GaN dice surface  Part B Phosphor coating  Encapsulant  I5kU   35SE1  smooth surface  andbondingring   1SkU   X130100M   1916SEI  15kU   X78828Mm   17/FEB/14   Encapsulation  Encapsulation  Fresh Unit Fresh Unit   Au bonding wire   and die attach  and die attach  delamination  delamination  15kU   100m   2027SEI   due to  due to  53 hygroscopic  hygroscopic  stress  stress ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f93958c8-6a24-4210-b7bb-1c9aeb3e00eb/f93958c8-6a24-4210-b7bb-1c9aeb3e00eb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=7a77a51c012c04cb9563b62dd514d4395be363a3)
## Encapsulation and die attach delamination  

![VoidspresentallovertheLED  Voidscreatedonouterrings  die-dieattachinterfaceand  (darkarea)  littlebitaroundLEDdie  Dieattach  Moldingpart  Littledarkeningdue toless  voidsaroundtheLEDchip  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f11d1db4-73b9-440c-a64a-af557877e971/f11d1db4-73b9-440c-a64a-af557877e971.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=a72b2beac4af39f653e10fc2125775028e852e00)
C-SAM of flipped blue LED (a) before initial degradation (tested for 24 hours) and (b)  after final degradation (tested for 356 hours). Die attach interface with LED chip got  completely blackened after testing for 356 hours whereas area outside LED chip is  not so darkened. The die attach area can be identified easily by a square exactly at  the center of the LED package

Investigate the different degradation processes in the  2 nd   and 3 rd   stages for LEDs tested while turning on

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f2c97285-4567-4e3c-a03b-6a12e1e7054f/f2c97285-4567-4e3c-a03b-6a12e1e7054f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=f050cb1c506e1a297b8f530df607b5dfc5584365)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/db00bd50-7009-43c5-a721-0962c233aaa8/db00bd50-7009-43c5-a721-0962c233aaa8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=cedcab308a801917d6bc9c4393e5ed0f57b0058a)
![Encapsulant   Molding part  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2fb82c0b-fa96-4cbc-b7a0-9587bd39d884/2fb82c0b-fa96-4cbc-b7a0-9587bd39d884.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=11da1f790a3c1fb264e93872845a34ae59f7d5a7)
Micrographs of the degraded unit

Fresh unit

After 144 hours of  White HB LED   under 85/85 with  350 mA

“Uncover the Degradation Science of Silicone Under the Combined Temperature and Humidity  Conditions” November 2017, IEEE Access 6:1-1, DOI: 10.1109/ACCESS.2017.2778289

## Investigate the different degradation processes  in the 2 nd   and 3 rd   stages 

![Hydrolysis  45Hrs  105   Condensation  Cracksrecover  Dueto diffusion   Hrs  Thermal Oxidation  020406080100120140160  TestingHours  Thermaloxidation  Thermal Ageing  150Hrs  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/40ef806d-16ab-4cc5-819f-fa2c05be66db/40ef806d-16ab-4cc5-819f-fa2c05be66db.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=3d0a6cd9bae8e61e1b3af9f54297e49754515b13)
![CH CH CH, CH CH CH —————- OH-Si-O-Si-O-Si-O-Si-O-Si-O-Si-OH —————- CH3CHCHCH;CHCH3 Hydrolysis Condensation ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/69566eef-9329-41cb-a32a-46ee237a4be0/69566eef-9329-41cb-a32a-46ee237a4be0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=51f1acb4402f6b38e349af5c706519fd85a2ea73)
“Time evolution of packaged LED lamp  degradation in outdoor applications”,  Optical  Materials ,  Volume 86 , December 2018,  Pages 148-154

"Impact of visible light and humidity on the stability  of high-power light emitting diode packaging  material", Journal of Applied Physics 130,  083101 (2021)  https://doi.org/10.1063/5.0059515

## Density  Functional  Theory Computation 

![150  150 100  100 ΔG KJ/mol 50 E a 0 0  1 -50 -50   Reaction Co-ordinate  Reaction Co-ordinate ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b9e50a77-8d1e-490e-8a55-317e7de885fa/b9e50a77-8d1e-490e-8a55-317e7de885fa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=526e2c15a19584fb75fd99fa7579142b61cc87ec)
Identified  Minimum  Energy Paths  (MEP)  of Hydrolysis(red)  and Condensation  (blue)  of PDMS as represented by the Free Energy Change (ΔG) (yaxis)  and  reaction  coordinates (x-axis)

![100  G  KJ/mol  20  -10  Reaction Co-ordinate  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/afbe46b3-5b2c-42de-8a72-03f2d013c050/afbe46b3-5b2c-42de-8a72-03f2d013c050.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=d7436d7e605df92a21b2f6994d65e593942172d6)
Reaction  intermediates  of hydrolysis  reaction  traced from Transition State Search computation is represented in terms of Free Energy Change (ΔG) and the Reaction Coordinates.

![LO  DG  KJ/mol  -O  Reaction Co-ordinate  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/adc3b62e-b289-438d-ae24-bb028f9ef4ca/adc3b62e-b289-438d-ae24-bb028f9ef4ca.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=6bd8c20c930b926953ac481394e78328cfc8fb6d)
Reaction  intermediates  of Condensation  reaction traced from Transition State Search  computation  is represented in terms of Free Energy Change (ΔG) and the Reaction Co-ordinates.

## Experimental Results and Analysis  

Water content is 1.5x10 -3  mol of H  O/mm 3   of silicone 2

|Current|        Total LED                Temperature                (Ttotai)      |        Time to                discoloration      |        Discolored                area                （Ad)      |        Rate of                reaction                >      |        Activation                Energy*                （Ea)      |
|---|---|---|---|---|---|
|(m A)|(Kelvin)|(hours)|(sq-mm)|        (mm2)/                hour)      |(KJ/mol)|
|350|458|1２７|8.04|0.063|124.3|
|300|433.3|180|6.02|0.033|120|


\* activation energy is computed using Polayni-Eyring Model instead of  Arrhenius model

The experimentally determined Activation energy is 124.3 kJ/mol, and our simulation results agree well with the experimental data.

## Mathematical  Model of  degradation 

The growth of the area of discoloration with  time is given as

$$\begin{array}{c}{{V_{d}(t)=A_{0}+A_{2}e^{A_{1}t}\,;}}\\ {{A_{1}=\frac{\sum_{i=1}^{2}\beta_{i}P_{i}}{k_{1}E_{a}-\frac{k_{B}T}{V}-\,\alpha_{c o n d}\beta_{3}}}}\\ {{A_{2}=V_{0}e^{A_{1}(-t_{0})}}}\end{array}$$
$t_{0} $  is the  incubation time for the formation of discoloration, i.e. it is the time needed to accumulate sufficient hydrolysis byproduct to begin the discoloration and the corresponding discolored  volume  is   $V_{0}$  .  If  the silicone has larger defects that can absorb  light  for  the  initiation  of hydrolysis, then the incubation time will be smaller. In other words,    $A_{2}$  represents the quality of the silicone. The poorer the quality, the larger its value.

Here    $P_{1}$   represents the power density of the blue light and  $P_{2}$   represents the power density of the yellow light. The corresponding  $\beta$   represents the absorption coefficient of the different light by the discolored region respectively, which we assumed to be constant in this work.

The very initial absorption of the lights could be due to the defects in silicone or trapped water molecules in the silicone.

$\alpha_{c o n d} $  is the heat released from condensation reaction per unit volume of the hydrolyzed PDMS and  $\beta_{3}$   represents the fraction of  𝛼𝑐𝑜𝑛𝑑  that will contribute to the subsequent hydrolysis.

## Comparison of our Model with Experiments 

![1O  10  350mA  350mA  300mA  300mA 1O  10 9 9 （zuu  ) 2  W  8  ) Czuu   m  2  8  m 9-0X]  -6 Area of Discoloration (x10  C  7 6  【9-0LX)  -6 Area of discoloration (x10  7 6 5 5 4 4 3 3 2 2 1 1 0 0 0  50  50  100  100  150  150  200  200 0  50  50  100  100  150  150  200  200 Time (hours)  Time (hours)  Time (hours)  Time (hours) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7b777ecb-d797-4310-b168-a173d5168306/7b777ecb-d797-4310-b168-a173d5168306.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=827cb1021a019c5725a2d26f80a31fffac60883c)
The data points represent the experimental data and the  solid lines in the above figures are from our  mathematical model

## Lifetime Prediction based on the Model 

![0.025  3.5  10.02  2.5  0.015  0.01   L-S  0.005  0.5  100   200   300  2001   3:00   9001  Time (hours)  Current (mA)  300mAA350mA   250mA  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cada8020-ff1f-475b-887f-22998f12d213/cada8020-ff1f-475b-887f-22998f12d213.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=9e17471187cff16005ab54edbc981a3918357a25)
$\mathsf{A}_{\mathsf{d}}$   is the area of discoloration    $\mathsf{A}_{2}$   depends on silicone quality and can be found by observing the time    where the discoloration start

## Variation in degradation  mechanisms for different  amount of RH 

## Water content is 1.5x10 -3  mol of H  O/mm 3   of silicone 2 

![Initial (0.0 kJ/mol) Initial (0.0 kJ/mol)   Rl 1 (22.5 kJ/mol)  RI 1 (22.5 kJ/mol)  TS (23.88 kJ/mol) TS (23.88 kJ/mol)   Final (22.27 kJ/mol)  Final (22.27 kJ/mol) CH3  CH 3  CH3  CH 3  CH CH3  3  CH3  CH 3  CH CH3  3  CH3  CH 3 |  |  |  |  |  | (Si-O-) (Si-O-)sH + 2H,O  6 H + 2H 2 O  (Si-O-) (Si-O-) + H,O + H+ + OH-  6  + H 2 O + H +   + OH -  (Si-O-)s-H + Si-(OH)2 + H2O  (Si-O-) 5 -H + Si-(OH) 2  + H 2 O  (Si-O-) (Si-O-)s-H + Si-(OH)2 + H2  5 -H + Si-(OH) 2  + H 2 |  |  |  |  |  | CH3  CH 3  CH3  CH 3  CH3  CH 3  CH3  CH 3  CH3   CH 3  CH3  CH 3 Direction of hydrolysis reaction  Direction of hydrolysis reaction ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4c86336b-5294-4267-b170-ece68906d5d6/4c86336b-5294-4267-b170-ece68906d5d6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=36547ef361e0825fa9248c1fdd173e891ea37b37)
## Water content is 2.2x10 -3  mol of H  O/mm 3   of silicone 2 

Initial (0.0 kJ/mol)  RI 1 (64.86 kJ/mol)  TS (67.77 kJ/mol)

Final (225.6 kJ/mol)

![CH3  CH 3  CH CT3  3  CH CH3  3  CH3  CH 3  CH CH3  3  CH CH3  3 |  |  |  |  |  | (Si-O-)sH + 3H2O  (Si-O-) 6 H + 3H 2 O  (Si-O-)6 + 3H2O  (Si-O-) 6  + 3H 2 O  (Si-O-)s-H + Si-(OH)2 + 2H2O  (Si-O-) 5 -H + Si-(OH) 2  + 2H 2 O  (Si-O-) (Si-O-)s-H + Si-(OH)2 + 2H2O  5 -H + Si-(OH) 2  + 2H 2 O |  |  |  |  |  | CH3  CH 3  CH3  CH 3  CH3  CH 3  CH3  CH 3  CH3  CH 3  CH3  CH 3 Direction of hydrolysis reaction ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b2e743eb-7943-49aa-b1c3-3df782e77424/b2e743eb-7943-49aa-b1c3-3df782e77424.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=1ecedc4de538806b609964360e45a49b7beadb40)
## Water content is 1.5 x10 -3  mol of H  O/mm 3   of silicone 2 

Initial (0.0 kJ/mol) kJ/moi   TS (0.444 kJ/mol) IS (0.444 kJ/mol)

## RI 2 (0.103 kJ/mol) 12 (0.103 kJ/mol)  

## Final (-22.305 kJ/mol) Fihai(-2  

![CH CT:  | 3  CH |  3  CH CH:  | 3  CH |  3  CH CH3  | 3  CH CH3  | 3 (Si-O-) (Si-O-)s-H + Si-(OH)2 + H2O  5 -H + Si-(OH) 2  + H 2 O  (Si-O-) (Si-O-)s-H + Si-(OH)2 + H2O  5 -H + Si-(OH) 2  + H 2 O  (Si-O-) (Si-O-) + H2O + H+ + OH  6  + H 2 O + H +   + OH -  (Si-O-)H + 2H2O  (Si-O-) 6 H + 2H 2 O |  |  |  |  |  | CH3  CH 3  CH3  CH 3  CH3  CH 3  CH3  CH 3  CH3  CH 3  CH3  CH 3 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c79180d2-5f15-4549-a920-d5d35c19a9fd/c79180d2-5f15-4549-a920-d5d35c19a9fd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=5e5483f86d56235d1da226fc8dceafa6d6d74448)
Direction of Condensation reaction

## Water content is 2.2x10 -3  mol of H  O/mm 3   of silicone 2 

Initial (0.0 kJ/mol)

RI 1 (22.75 kJ/mol)

TS (579.64 kJ/mol)

![CH | 3  CH CF  |  3  CH | 3  CH | 3 (Si-O-)s-H + Si-(OH)2 + 2H2O  (Si-O-) 5 -H + Si-(OH) 2  + 2H 2 O  (Si-O-) (Si-O-)s-H + -Si-OH + (CH3+)2 + 2H2O  5 -H + -Si-OH + (CH 3 + ) 2  + 2H 2 O  (Si-O-)sH + 2H2O + H+ + OH  (Si-O-) 6 H + 2H 2 O + H +   + OH - |  |  |  \  | HO-  HO - CH3  CH 3  CH3  CH 3  CH31  CH 3  CH3  CH 3 Direction of Condensation reaction ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6c1df9f9-6929-4ef3-b14d-68f41e880f6c/6c1df9f9-6929-4ef3-b14d-68f41e880f6c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=5a91bc2a4882e42f04deb00b4737d4c5500bce30)
Direc

## Water content is 2.2x10 -3  mol of H  O/mm 3   of silicone 2 

![RI 2 (162.36 kJ/mol) Rl 2 (162.36 kJ/m0l)   Final (-142.87 kJ/mol) Final (-142.87 kJ/mol)  (Si-O-)4-Si=O + -Si-OH + (CH3+)3 + 2H2O (Si-O-)sH + 3H2C  CH3CH3   CH3  Direction of Condensation reaction Direction of Condensation reaction  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/447bb724-a2a3-4ad5-a8c4-93da6f39e27c/447bb724-a2a3-4ad5-a8c4-93da6f39e27c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=15c869714f403357a1e350f3d7343e3473d62885)
## Activation Energies with different amount of  humidity level 

![4.5  4.0-  3.5-  3.0  2.5  2.0  1.5  1.0-  0.5  0.0-  0.5   1.0   1.5   2.5   ③.0  x 10-3 moles of H,0 per mm? of Silicone  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a3fda66b-640a-43ce-94b3-6051a8906fbb/a3fda66b-640a-43ce-94b3-6051a8906fbb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=55bdac05e67f35e5cf2e529c621a6ef83884f4e7)
Hydrolysis

![7.0  6.5  6.0  5.5  5.0  4.5  4.0  3.5  3.0  281  1.5  1.0  0.5  0.0  -0.5  -1.0  00   0.5   1.0   1.５   ２０   2.５   3.0   3.5   ¥4.0   4.5  x 10- moles of HO per mm? of Silicone  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b1ce7535-19df-4f76-b6ab-6d4378e9e8d2/b1ce7535-19df-4f76-b6ab-6d4378e9e8d2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=fd792d1692a29f1e323dd12632f79f5797a7af90)
Condensation

## Effect of increasing humidity in LED degradation rate 

![T2O  H 2 O  E a-cond  a-Cond  E a-Hyd  a-Hyd ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8f172b20-1da0-48de-bff1-2afb7399c05d/8f172b20-1da0-48de-bff1-2afb7399c05d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=545e602eaf54dc4950463cea23bf830cc31b1ab9)
• When   $\mathsf{H}_{2}\mathsf{O}$   content increases drastically, there will be minimal or no dependency on the condensation reaction to provide energy for subsequent hydrolysis in the Silicone.

• Thus,  hydrolysis  will  be  the  dominant degradation reaction in the LED housing due abundance of   $\mathsf{H}_{2}\mathsf{O}$  .

• This abundance of   $\mathsf{H}_{2}\mathsf{O}$   causes lowering of the E a  and simultaneously increasing the rate of the reaction as the combined energy of the LED and test system is high.

## Case Study on the Failure  Mechanism of Printed Circuit  Board burnt and its Root Cause 

## Introduction 

• PCB failures range from circuit malfunctions to propagating  PCB faults.    • PCB failures that may appear similar can originate from many  different root causes. A propagating circuit board fault is usually  considered universally to be a high severity thermal event. • Its initiating mechanism starts when a resistive path forms  between two traces or planes in a PCB that are at a different  electric potential. This resistive path can form due to an external  heat source, insulation breakdown, arcing, or contamination. • The power dissipated at the fault region should be sufficient to  generate enough heat to further damage the PCB and sustain  the thermal event.

## Failure Analysis of PCB 

• The PCB in this case study was used in public  transport. It has multiple layers that consist of  8 layers with 2 mm of total thickness. • These PCB Layer 4 is the electrical ground  plane and layer 5 is the power plane (VIN)  where 12 V is connected to it.  • Its base material is FR4 (flame retardant) and  had superior CAF (conductive anodic  filament)-resistance (anti-migration) properties  and a high glass transition temperature (Tg)  (minimum 170 C) for applications where high  mechanical and chemical resistances to heat  and moisture properties are required. • After their operation for 1.5 months, the  operations of the ethernet device stopped and  the burn-out area at the bottom edge of the  PCB was found, as shown in Figure  1 .

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9031dbff-789b-4395-aada-727dde926754/9031dbff-789b-4395-aada-727dde926754.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=4e9daba94ccbdae38486c1c62819aceceda7805c)
Figure 1.  Visual inspection  (side view) of failed PCBs

## Identification of the Failure  Mechanism 

• A V-groove penalization was used here. A pizza cutter/V-cut was employed for the de-penalization. • A similar burn-out as in Figure 1  was  observed on a few originally good   inventory boards after testing them with the  system in the factory.  • The supply current was monitored to avoid  severe damage to the testing PCBs.  • It was found that, after the initial  shortcircuited event, the burn-out expanded  due to the over current protection (OCP)   mechanisms in the power module.

![Pizza cutter  de-penalization  fne  GND  Zoomin  coupon   No Copper Inner Copper  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/916a3c02-f7c1-4e96-9451-668ad12d39d9/916a3c02-f7c1-4e96-9451-668ad12d39d9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=1803da526a7a1486f040f244f216d4fb905b6206)
Figure 2 Cross-section of  the board near the V-cut  scoring area.

## Identification of the Failure  Mechanism 

• Upon careful examination of the PCBs that  were not short-circuited or burned out,  the  presence of many crack lines could be seen  (Figure  3 ).  • These crack lines were found  after the depenalization.  • With these crack lines, moisture from the  environment could  penetrate and diffuse into  the PCB easily.  • In the presence of the applied voltage, the  electric  field could cause the copper ions  from the PCB copper planes to drift across  either as a  dendrite formation or as a CAF  formation.

![Impacted  area  <   GND   Crack  coupon   No Copper   Inner Copper  Inner  No Copper  Copper  a  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8a1e3893-631e-4af1-a1ea-b88bf5e63404/8a1e3893-631e-4af1-a1ea-b88bf5e63404.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=806f3129474c52634493053401938b813a1c2256)
Figure 3.  Cross-section of the  PCB: ( a ) potential crack location;  ( b ) after pizza cutter (V-cut) depanel  process.

## Identification of the Failure  Mechanism 

• The formation of dendrites and CAFs can seriously influence the reliability of electronic  systems.

• Dendritic growth usually occurs when metal ions move  in the electrolyte layer  near the anode and then deposit  near the cathode  and grow in a tree-like or needle-like   formation under the influence of a DC voltage bias and it  is usually formed on the surface of a PCB.

• Heat can be generated from the electrical ionic  conduction current during the migration process or from  the electrical current conducted through the dendrites  when they bridge the conductors.

• Eventually, the dendrites can  develop into substantially  low resistance with significant heat dissipation and can  result in a propagating fault in a PCB.

![Anode   Cathode  20KU   8308   16mm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/70566102-6340-471b-8775-bf21602ef933/70566102-6340-471b-8775-bf21602ef933.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=a4e52471650ef2590c750fbf443b0b7f77476e07)
## Identification of the Failure  Mechanism 

• Conductive Anode Formation (CAF)   • The CAFs are formed as anode metal gradually becomes  ions and begins to migrate under the effects of the bias  voltage.  It is formed within the PCB insulation materials .     • , hence the name conductive anodic filament  Unlike dendrite  formation, the conductive filament growth forms from the  anode to the  cathode .    • Failure symptoms of a CAF range from intermittent resistive  faults under current limit conditions to catastrophic   propagating circuit board faults if the fault current is not  sufficiently limited.    • Basically,  CAF formation follows a two-step process; namely,  the formation of a microcrack that bridges two conductors to  establish the migration path and an electrochemical reaction  with the presence of a DC bias and moisture to drive the  migration along the cracks between the two conductors.    • This was observed in our experiments.

![Hole to Line  Cathode  + Anode  Line to Line [正】 1A(ResearcHoleto Hole  Layer to Layer ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/64dd7280-bd3f-445c-8476-e13270a4d838/64dd7280-bd3f-445c-8476-e13270a4d838.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=32c7d58cb79c026774f8f7ca478db61fefe5d8df)
![ViaBarrel  ViaBarel  CAH  Cu  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9b62b58e-a229-4dd5-9505-eac2f34ea7d7/9b62b58e-a229-4dd5-9505-eac2f34ea7d7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=ba4eac07f4f59c1e7b5436d625dcb215925385e6)
## Conductive Anode Filament (CAF) 

• As the conductive particles are close to the cathode as driven by the electric field from the anode to the cathode, partial discharge can occur due to the intensification of the electric field between them.

• In the presence of multiple conductive particles, as in our case, the frequency of the partial discharge can be much higher.

• However, partial discharge does not necessary lead to the breakdown of the dielectric but it will lead to the reduction of its breakdown voltage.

• As  the size and concentration of  the particles increase, the insulating performance of the dielectric is further inhibited.

• With the reduction in the insulating performance, a leakage current can flow through the FR4 and generate heat.

• It is worth noting that if the temperature around the FR4 exceeds more than  $65^{\circ}\mathrm{C}$  , heat dissipation becomes a major issue for the FR4; beyond  this temperature, the failure mechanism changes to a thermal breakdown from an electric breakdown

## Conductive Anode Filament (CAF) 

• After a partial discharge, a short carbonization path is formed that connects  the conductive particles to the nearby electrode. In a sense, the electrode  is now extruded.  • When the  resistance reduces to a certain value that corresponds with an increase in the leakage current,  the Joule heating can drive out the  surrounding moisture and an increase in resistance can be expected, as  was observed in our experiments. • However, this localized  heat enlarges the crack. Hence, external moisture  can now diffuse further and in a greater  amount into the FR4.  • As the conductive particles move closer to the extruded electrode, partial  discharge occurs again. This iteration continues until the effective distance  between  the extruded electrode and the anode becomes so close that the  field between them is  so high, it exceeds the breakdown field of the FR4,  which is already reduced due to the presence of conductive particles and carbonization.

![GND  Edge  Between VIN-GND  Short points  Edge  GND  Copper particle  diffusionintotheFR4  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/31e7f41d-948b-4d8e-bec8-f806ea465e47/31e7f41d-948b-4d8e-bec8-f806ea465e47.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=8f0471b48e14962552123f27645584a5d270d1d6)
Figure 4.  A 3D X-ray of the PCB that shows the cross-section of the PCB. The propagation of the  cracks and the movement of copper from the V IN  layer to the GND layer due to the presence of the water layer and electric field can be seen: ( a ) shows the formation of crack lines before the resistance  between them begins to decrease; ( b , d ) are the plane  of  the  GND  and  V IN  layer, respectively, as extracted from the 3D Xray; ( c ) is the plane in the middle of the GND layer and V IN  layer as extracted from the 3D X-ray where the white arrows represent copper particles; ( e ) side view of the PCB showing the short point in between the V IN  layer and GND layer.

To further analyze and characterize the cracks formed in the PCB, as shown in Figure  4,   the PCB area with the cracks was dissected out and examined under an X-ray  Micro CT  (computed tomography) scanner system (model number CTLab-HX130-2- E).  Volume Histogram

![PD:9104.933μm  W:3314C:3074   Edge  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4f77d185-930d-4d8a-9e11-08b2215416e2/4f77d185-930d-4d8a-9e11-08b2215416e2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=37f0da1c0862a83e4d9cc8313cdd2c7d10cd1e31)
Figure 6.  A total of 78 cracks are  identified and represented by  individual colors.

Volume histogram of the  cracks shown in Figure  6

![25  20  () uanba   15  0  2x105   6x105   1x106   1.4x106  Volume (μm3)  PD:9104.933μm  Edge  W:3314C:3074  Volume (cubic micrometers)  5.1×104   4.6×105   8.7x105   1.28×106   1.69x106  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/73a0eb28-646f-44f4-8ab4-7b521b3a21b8/73a0eb28-646f-44f4-8ab4-7b521b3a21b8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=84ed6e2745ed11a697642f84864f287c80272ae4)
Cracks with the same  volume are  shown  with the same color

## Root Cause Identification 

• It could be  observed that large cracks  occurred at the edge of the PCB and they  progressed toward  the inner parts of the  PCB along with the GND and VIN layers.

• All these cracks were due to excessive  high strain at a high strain rate induced  during the V-cut de-panelization s  measured experimentally with the results  shown in Figure  8 .

![2000  IPC-WP-011  StandardLimit  1500  Location-1  1000  Location-2  Location-3  500  100   1000   10,000   100,000   10,00,000  StrainRate(uStrain/sec)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0621806d-d0b7-4a24-a963-b0efefdfd2b1/0621806d-d0b7-4a24-a963-b0efefdfd2b1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=9dc0f32cd482585373c58ba315f93628abd04eb3)
Figure 8.  Strain gauge measurement  data show that a part of the principal  strain exceeds the  IPC-WP-011 standard  limits during the cutting process.

## Root Cause Identification 

• The large cracks observed were concentrated in a certain area of the PCB instead of  being  distributed uniformly.  • This non-uniform distribution of the crack sizes was believed  to be due to the inhomogeneous  strain distribution along the edge of the PCB during the V-cut de-panelizationas simulated  using a finite element analysis. • There were also large cracks present away from the edge but they were  closed to the largest  cracks, indicating the weakening of the mechanical integrity of the  board after the large cracks occurred.

![Pizza cutter  PCB   de-panel   PCB  Coupon  V-cutline  simulation  0.0045602  0.0018  0.0012  0.0006  0.00018503  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b23cb252-0d8c-4093-88f6-1c5f9dffebe1/b23cb252-0d8c-4093-88f6-1c5f9dffebe1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=c75b0ca98a464673d5186e9b2696dd9b46caece8)
Figure 11.  PCB de-panel  process and mechanical  simulation result.  Locations 1, 2, and 3  show strain  gauge  measurement points.

## Root Cause Confirmation 

• To further confirm the proposed mechanism, 5 samples of the PCB that  had crack  lines due to de-penalization were subjected to 65  ◦ C/95% RH.

• Table 1  summarizes the test  results. The test condition was selected so that  a continuous film of water could be formed  in the PCB.

• The test results showed clearly that these cracks allowed moisture to  diffuse  into the PCB and reduced the impedance between the GND and

二101 11+

|Sample #|        Initial Resistance                between Vin and      |        Measured Resistance                after the Specified                Test Duration (Ω)      |        Test Duration                (Hours)      |
|---|---|---|---|
||Over 108|58.6|160|
||Over 108|30.9 K|I13|
||Over 1o8|316.2||
||Over 108|1.63 K||
||Over 108|46-5|I41|


## Failure Process and the Underlying Mechanism 

![Looping  1.Inthepresenceof   3.Localizedleakage of  Crack   moisture andelectricfield,   2.This will cause the   the currentstartsto  copperionsfromthe   concentration ofthe   flow,whichincreases  GND  copperplaneswilldrift   electricfield and   thetemperatureof  through theglassfiberas   decreasethe   theFR4locallydueto  theinitialstepof   insulationresistance   highresistanceofthe  conductiveanodefilament   oftheFR4   path and theJoule  (CAF)mechanism   heating.  CracksinPCB along  thecopperedge and  Moremoisturewillenterintothe   4.Thelocalized increasein  moisturepenetration  FR4,andcontinuouslysevered  temperaturecreatesnon-from steps1-4.  uniform thermo-mechanicalstressand  Insulationresistance  enlargesthecrackthrough  betweenVInandGND  isreduced   theirpropagate.  5.Asthelocalizedtemperature  6.Whenthecarbidebetween   increasesbeyond 65C,  Lowimpedance   the two copper traces pilesup,   electricalbreakdownbecomes  currentpathsare   acarbonizationconduction   thermalbreakdown,molecular  formedthroughthe   channelisformed,andthe   chainsin theFR4arebroken by  cracks   FR4losesitsinsulation   theflowofelectronswith  capabilityirreversibly,   carbondepositionalongthe  resultingin theburn-out.   path,thusfurtherincreasesthe  leakage current.  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/78a0e9db-d9d7-41be-b432-3039264defcc/78a0e9db-d9d7-41be-b432-3039264defcc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=e2dc3b5b5aa59b18b198e5ce39d92976f2506f54)
## Root Cause Confirmation 

• In the pizza cut de-penalizing, the applied  mechanical stress caused cracks on the   copper keep-out area of the PCB, as shown  in Figure  12.  However, without de-paneling,   there was no crack on the copper keep-out  area .

• It was, therefore, clear that it was the pizza  cutter de-penalization that caused the   cracks in the PCB, which then resulted in  moisture diffusion into the PCB.

• As the cutting area was near the GND plane  and VIN plane, as can be seen in Figure  2 ,  the reported failure mode was observed.

• We found that no damage was observed if a  manual de-penalization was performed.

![PCB NO.1  No.2 Pizza-cut Crack Crack NO.1  （100X）  NO.2  (100X) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3d039128-647a-4ae6-b6c1-6edb71a0b6cc/3d039128-647a-4ae6-b6c1-6edb71a0b6cc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=81552928e777a62417fdf54ed50a3715716c13fc)
Figure 12.  Observation of cracks in a  PCB after de-paneling using an Olympus  BX51 microscope at 50 ×  magnification of: ( b ) location No. 1 and  ( c ) location No. 2, as marked in ( a ),  which is a horizontal  cross-section of a  PCB with a pizza cutter de-panel.

## Corrective Actions and Reliability  Verification 

• With the identification of the root cause, another type of de-penalization was introduced where no crack was produced. Due to confidential considerations, this new way cannot be disclosed.

• To verify the effectiveness of the corrective actions, reliability tests were performed along with the new de-penalization method. The test condition was set at 65  ° C/95% RH so that a continuous water film could be formed if cracks existed. To speed up the test, a voltage of 100 V was applied across the GND and V IN .

![S11  S12  1×102   S13   1×102  S14  S15   1x101   A  1×101   S16  S17  S18   1×10-1  1×100   81-10  1×10-3  1x10-1  1×10-2   1x10-5  1x10-3   1×10-7  1x104   1x10-9  1×10-5   1X10-11  100   200   300   400   500   600   700800   100   200   300   400   500   600  Time(Hours)   Time(Hours)  a   b  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bd874dbd-9dd0-4e9d-9e98-ea1a3d3048f6/bd874dbd-9dd0-4e9d-9e98-ea1a3d3048f6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=258fa509d76ef0b95f77fe1cce859a8f84106ffb)
Figure 14.  Resistance changes over time under the reliability test mentioned above: ( a ) 10 samples  with the new de-penalization; ( b ) 5 samples with pizza cut de-penalization and the resistance fluctuation as reported earlier can be observed. The resistance in the  Y -axis is in GW.

![Step1:Receptionof failed device  Step 2: Detailed Examination and Failure ModeIdentification  Step-3:Failure Mechanism Proposal andIdentification  Step-4:FailureMechanism Confirmation  Step-5: Corrective Action and its EffectivenessVerification  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/721fb1ae-9c7e-4930-9984-ade9a68d4489/721fb1ae-9c7e-4930-9984-ade9a68d4489.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215831%3B1743219431&q-key-time=1743215831%3B1743219431&q-header-list=host&q-url-param-list=&q-signature=cdedb66d5bcbadc6b9b10439ab932e77a65b8774)
Flow chart of failure analysis for root cause

## Summary 

• A detailed failure analysis showed that the failure mechanism was a propagating fault of a CAF formation as moisture was diffused into the PCBs via microcracks introduced due to a V-cut de-penalization. • Although the PCB itself was CAF-resistant, the presence of a microcrack due to de-penalization could render its CAF resistance ineffective.   • With the identified root cause, a modified de-penalization method was developed and no microcracks were observed with this new method, which verified the root cause.  The modified method is proven with reliability test.

Tan, C.-M.; Chen, H.-H.; Wu, J.-P.; Sangwan, V.; Tsai, K.-Y.; Huang, W.-C. Root Cause Analysis  of a Printed Circuit Board (PCB) Failure in a Public Transport Communication System.  Appl.  Sci.  2022 ,  12 , 640. https://doi.org/10.3390/app12020640

## Conclusion 

• Failure is sure to happen.   • Pre-mature failure must be avoided   • The avoidance of pre-mature failure can be made only if root causes can be identified and verified through reliability tests.   • Root causes identification requires the knowledge of failure mechanisms, instead of failure modes.   • Failure mechanisms identification and verification requires extensive material analysis tools, in-depth failure analysis tools, and simulations, together with good knowledge of various failure mechanisms.

