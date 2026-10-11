---
title: "239_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_2b1687072784c92f36d0ca0cc0cf061c7295230462135641
file_size: 1340162
---

## Enhancing the SRAM Failure Analysis Process  

Raymond G. Mendaros  Global Failure Analysis (GFA)  Analog Devices General Trias (ADGT)   Gateway Business Park, Brgy. Javalera, Gen. Trias, Cavite, Philippines 4107  Phone: +63 2 867703, Email:   raymond.mendaros@analog.com

Abstract-   The advent of the 65nm silicon fabrication  technology node and smaller geometries; particularly for static  random-access memory (SRAM) array, posed several Failure  Analysis (FA) challenges such as the fault isolation capability  limitations, physical FA (PFA) approach identification intricacy,  defect node localization complexity and defect to fail mode  correlation difficulty. To address these challenges, device defect  modeling (DDM) process through software simulations and  building of defect databases were introduced. Through the aid of  the DDM process, defect sites were reduced to a single transistor  or node from the SRAM array.  Defect models were derived from  the simulation process that guided analysts in identifying the  suitable PFA approach.  DDM process was effective in the failure  mechanism to failure mode simulations. The DDM process was  likewise instrumental in building defect databases for SRAM  layout designs. These databases contained relevant information  such as circuit simulation results, fabrication material stacking,  suggested fault isolation techniques and potential defect locations  that served as references for analysts.

Keywords  – Defect Modeling, Static Random Access Memory,  fault isolation, 65nm technology node, SRAM defect database

## I. I NTRODUCTION 

Driven by the industry’s requirement of reducing chip  size, semiconductor companies implemented in their products  the 65nm silicon die fabrication process and smaller geometries  [1]. This die fabrication process node, due to the reduced  component size, posed several FA challenges. In this technical  literature, the focus of the study is on the failure analysis  process improvement for 65nm embedded 6T SRAM devices  wherein the learning can be fanned out to smaller fabrication  technology geometries. The FA challenges for leading  technologies are as follows:

## 1.    FA tools and techniques’ fault isolation limitations   

Advanced photon emission microscopy (PEM), optical  beam induced resistance change (OBIRCH) and thermal  camera’s failure analysis fault isolation tools do not anymore  have enough resolutions to pinpoint the exact anomalous  SRAM memory transistor for 65nm and smaller technologies.  As an example, the PEM photo in  Figure 1  was captured on a  huge    $0.18\mathrm{um}$     technology   node.   There   were   two  metal–oxide–semiconductor field-effect (MOSFET) transistors  in the emitting site but because of the tool’s limited optical and  camera magnification capability, even at this huge technology  node, the exact emitting transistor could not be identified. This  capability limitation is magnified when dealing with smaller

geometries such as the 65nm technology node.  The limitation  encountered on the PEM system is a common shortcoming for  the OBIRCH and thermal systems.

![Pin 15(DATA)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/50d256f6-ee76-4611-a842-78c2adf318bd/50d256f6-ee76-4611-a842-78c2adf318bd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=04454d8d0eae56eaa2b023209eac6c55d863bca1)
Figure 1. PEM detected photon emissions from two NMOS transistors  however, the machine resolution could not resolve which transistor was  emitting. This is a 0.18um technology process.

## 2.   Identification of the suitable physical failure analysis (PFA)  technique or methodology  

The PFA technique or approach to be used may vary  depending on the defect type. For instance, an electrostatic  discharge (ESD) damage such as “pinholes”, due to its  miniscule physical attribute, is preferred to be chemically  deprocessed. Deprocessing will enable the inspection of the  whole layer (top down inspection), thus, has higher chances of  locating submicron defects as compared to the progressive  cross section approach. A via or plug formation defect, on the  other hand, is preferred to be cross-sectioned using a Focus ion  beam (FIB) equipment to have a good view of the defect site  (cross sectional view).

## 3.   Defect node localization is another FA challenge   

SRAM cell has six transistors in its circuit. Since DDM  process simulates a possible defect site through replicating the  failing electrical output response, the suspected defect site can  be narrowed down to a node or transistor.

## 4.    Physical defect to failure mode correlation   

Not all visual anomalies seen during physical failure  analysis (PFA) will necessary result to a failure. A suspected  physical defect observed in the chip can be electrically  simulated using the DDM process to determine its consistency  with the device’s failure mode.

To address these FA challenges, DDM process and  defect database generations were implemented in FA process.

## II.   EXPERIMENTS  

The study was focused on one embedded 6T SRAM  layout design. The memory failures were confined to “stuck to  low” and “stuck to high” memory failures. Timing and voltage  sensitive failures were not included due to the absence of the  exact transistor models for the LTSpice simulation software.  The memory failure types that were covered were single bit,  dual (twin) bit, full row and full column failures.

DDM simulated defect models were documented in the  database. An LTSpice student version (version 1.0.0.1) was  used in all the circuit simulations. The exact transistor models  of the 65nm memory device were not available due to  proprietary reasons. The inputs of the process are the gathered  electrical failure characteristic or behavior of the sample being  analyzed. These are the memory type (e.g. “single bit”) and  output response (e.g. “stuck to low”). The outputs are the  simulated failure memory type and output response that  corresponds to the introduced defect model (e.g. “added  resistance”) in the simulation circuit. The introduced defect  model, location of the defect in the circuit and the plots of the  simulated electrical failure characteristic or behavior are  documented in the database. The process flow is shown in  Figure 2.

![Inputs:   Staft   Process  1.Faling SRAMdevice  requiring simulation  2.Unervereddeuiring   Openha  simulation  Run thesimulationcircuit with the   Debug the simulation  stimulus   circuit  Is the circuit's  expected  output  simulated?  Modeladefectbased on the  SRAM's failing signatureor  uncovered PFAdefect  Add themodeled defect in the   Re-do the defect the  simulation circuit   modeling process  Run the simulation circuit with the  stimulus  Is the output  anticahe  rejectunit?   Output  1.Failure signatureandor  Record simulationmodel and   physical defect has  resultsin the database   been simulated  2.Updated database  End  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ab373d38-c318-4a5f-b5c3-542fc56d0447/ab373d38-c318-4a5f-b5c3-542fc56d0447.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=b500bd2b962044645fdbc5de05eb09f362f6b883)
Figure 2. Conceptual framework process flow.

This section was divided into 5 subsections. The first  section was the creation of an SRAM Device Defect Modeling  (DDM) simulation circuits using LTSpice (version 1.0.0.1)  software.  Figure 3  is a representative single SRAM 6T cell  created in the LTSpice schematics software. For the actual

DDM simulation circuit, several SRAM cells were created in  the software. The memory failures that were considered were  confined to “stuck to low” and “stuck to high” memory failures.  The memory failure types that were covered were: single bit,  dual (twin) bit, full row and full column failures.

![￥Cc2  Wordline  Output-Bitlne  PULSE(0 3 10n 1n 1n 1u 2u)  Gnd  tran03u 0.100n  include BSIM3v31.txt  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/87afa4a9-8708-4b39-b2fd-32ebcf556424/87afa4a9-8708-4b39-b2fd-32ebcf556424.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=21a02ab9044f3222a99dd8cfa6379d60d97ab1e6)
Figure 3. LTSpice representative circuit of a single SRAM cell

The second section was the creation of a process flow for  the defect simulations using the DDM circuit. The inputs of the  process were the fail memory types (e.g. single bit, dual bit,  etc.) and output response (e.g. “stuck to low”). The output of the  process were the simulated electrical failure responses. The  modeled defects were recorded in a database.

The third section was the building of defect databases for  specific SRAM layout designs. The contents of the databases  are as follows:

The  memory failure type  column contained the four  common memory array failures types: Single bit, Dual bit, Row  and Column failures. The  Input signal   column contained the  input pattern going to the memory array.   The  failure output  response  column listed the SRAM failing response. These were  either “stuck low” or “stuck high” output failure condition.  Commonly for embedded SRAMs, SPI communication  protocol is used. Thus, the output response was either logic  “low” or “high” only. The  simulated defect  column represented  the modeled defect that replicated the electrical failure mode or  characteristic.

The   lay-out location of the simulated defect  column, on  the other hand, indicated the location of the modeled defect in  the layout. The next column,  cross sectional illustration of the  fab process stacking of the simulated defect , illustrated the Fab  process material stacking of the defect site. The  FA techniques  to be considered  column listed the fault isolation and PFA  techniques to be utilized based on the modeled defect and  location. Finally, the  Images/ Output plots  column documents  the simulated electrical output response.

The last two sections (  $4^{\mathrm{th}}$   and   $5^{\mathrm{th}}$  ) revealed the areas in  FA process where the DDM process were utilized and  demonstrated. DDM’s usefulness in addressing the different  failure analysis challenges. At least two case studies each were  discussed to validate these two sections of the methodology.  Evidences of the simplified process were discussed.

## III. R ESULTS AND DISCUSSION   

## 6T SRAM DDM Simulation Circuit Creation   

Creating simulation circuits required knowledge on both  the simulation software and electronic circuit’s functionality. In  this study, there were three simulation circuits that were  created. The first circuit is a single cell to simulate single bit  failures. There were two variations of the circuit; with and  without output inverter. See  figures 5a and 5b  for the LTSpice  circuit and input/output responses.

The second circuit is a two adjacent cell to simulate dual  (double) bit failures. See  Figure 6a and 6b . Two separate  adjacent circuits were created, one lateral and one vertical dual  bit circuits.  Figure 6a and 6b  represent a lateral dual bit  simulator. The third circuit is composed of nine transistors,  3-rows by 3-columns memory array, to simulate row and  column failures. See  Figure 7a . The circuits were validated by  observing their output responses. See  Figure 7b and 7c.  An  SRAM cell without an inverter circuit at its output manifested  an opposite of its input signal.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/64fe88f5-37a0-45df-b75e-eeaa3e69682a/64fe88f5-37a0-45df-b75e-eeaa3e69682a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=d0206651e1dae8f082e942acc1e7e5867603a3f3)
Figure 5a. Single cell simulator without inverter circuit at the output

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/188b90b7-6f19-4f13-8d43-cd896e4af914/188b90b7-6f19-4f13-8d43-cd896e4af914.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=5a978f96c7fbd2382fb75d48199d6cd157406f63)
Figure 5b. Single cell simulator with inverter circuit at the output

![LSED3  ram03u0100m  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d2c64ac3-af7c-4b60-a4ae-e2d96cf68ff2/d2c64ac3-af7c-4b60-a4ae-e2d96cf68ff2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=20832ce30375513020c236048288e167a563af81)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/97255cf3-35dd-496d-8208-5cd0fcc08f13/97255cf3-35dd-496d-8208-5cd0fcc08f13.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=d4ca56687feab634cb420be140395ec6fe849548)
Figure 6b. Input and output plots of the dual bit cell

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8f8cb116-9518-469a-b5f0-0839272bbe70/8f8cb116-9518-469a-b5f0-0839272bbe70.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=20a4c65752341bfa9a1d089ea4b120e7ef0d6b0e)
Figure 7a. A 3-rows by 3 columns array simulation circuit for row and column  failures

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d5791466-d2e4-441b-a590-54c678a8d1ac/d5791466-d2e4-441b-a590-54c678a8d1ac.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=e5f70f32eb637e7db8c22ae8953f5f55caae5cb7)
Figure 7b. Input to the 3-rows by 3 columns array

![  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/93e29e5b-8b02-4394-9f19-52dbf7a3553e/93e29e5b-8b02-4394-9f19-52dbf7a3553e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=f81705088aab4e36f63040ba06dfa8b992880d95)
Figure 7c. Outputs of the 3-rows by 3 columns array

## Defect simulation process using the DDM circuit  

The defect simulation process flow is shown in  Figure 2.   The inputs of the process are the fail memory type (e.g. single  bit) and output response (e.g. “stuck to low”). The outputs of  the process are the simulated failure responses and updated  database.

## Defect Database  

Databases were created with the consideration to the  embedded SRAM lay-out design being utilized by ADI. The  defect database serves as reference and guide for analysts. The  benefits and advantages of the databases are as follows:

## a.   Defect sites’ locations are identified in the layout   

This avoided the tedious circuit analysis, commonly  manual approach, before the DDM process was implemented as  potential defect sites were already identified. Through the  database, once memory fail type and failure output response are  known, analysts already have an idea where to focus the  physical failure analysis and inspection.

## b.   The die fabrication material stackings are illustrated   

The information about material stacking were further  verified through Focus Ion Beam (FIB) cross-sections of actual  memory cells. With this information being available, analysts  can effectively plan their physical failure analysis approach. On  the other hand, without this information, the analyst recourses  to layout review and consultations which can cause significant  delays.

c.   Transistor and SRAM cell’s nodes such as, source, drain,  gate, Vdd, ground, etc., are identified and labelled.

The delays incurred due to the repeated access and viewing  of lay-outs to identify nodes are avoided. Furthermore, this  complements the material stacking information. The defect  locations are mapped in the FA reports from a top down  (layout) and cross-sectional (material stacking) perspective.  Table 1  showed a portion of the database.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b08c22f6-0dd6-4ea2-9479-83889a331efa/b08c22f6-0dd6-4ea2-9479-83889a331efa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=eace905ba73f22bb1d839ffa9037f3e8ad0e10d2)
Table 1. Representative defect database from one of the SRAM designs

## DDM failure mechanism-to-fail mode simulations  

Two representative failure mechanisms were simulated.

## a.   Simulation #1 – A Particle Defect  

A known programming pattern was loaded into the  device, particularly to the embedded SRAM, but the read codes  (checksum values) do not match the written pattern.  Bitmapping analysis was performed to test the memory array  and found a single bit failure with “stuck to high” output  condition. The bitmapping tool was able to identify the cell’s  physical location in the memory array.

Physical FA (PFA) done by ADI’s subcontractor  uncovered a random fabrication defect. A fall-on nitride (N)  particle between the gate and drain terminals of a transistor in  the failing site was identified. See  Figure 8.  The electrical  failing signature of the memory cell was confirmed when a  short on the gate and drain and an open contact on the drain  defect models were introduced into the simulation circuit.  The  anomalous contact is the common drain of the NMOS in one of  the inverters and pass transistor drain of the worldline. See  Figure 9  for the DDM simulation results.

![ESX  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e38d9071-ee45-4e5d-8be2-91b872f3d5c8/e38d9071-ee45-4e5d-8be2-91b872f3d5c8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=c7ab06cd31c58369bb4873f51d23cdb9958dbbc7)
Figure 8. TEM post FIB cross section (left) and EDX (right) results of the  suspect site

![wordline  sS  dd  vdd  WSS  wordline  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a22beaa4-f496-488a-81d7-cb25849d9705/a22beaa4-f496-488a-81d7-cb25849d9705.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=3ff9a5740847581d741cef846c0facc461379d19)
Figure 9. Stuck high output failure was confirmed

## b.   Simulation #2 –Resistive W-Plug Contact Defect  

ADI ATE testing showed that the programmed value of  “0” was showing an erroneous read value of “1”. Bitmapping  analysis showed two adjacent cells were failing. All the fault  isolation analysis techniques that were performed (PVC,  C-AFM and nano-probing) on the failing cells yielded no  anomalies. Physical analysis was still pursued and found  silicide and contact formation defects that were one cell away  from the bitmapper’s identified physical failing location. See  Figure 10  for the cross-sectional view of the defect and its  location in the layout. The defect observed was modeled and  introduced in the simulation circuit. Simulation results showed  that the defect site was consistent with the electrical failing  signature. See  Figure 11  for the simulation results.

differs in the locations where they occur. ESD defects are  expected to be situated near the edges of the transistors’ gate  channel where high electric fields are present while  deprocessing artifacts are observed at the center of the gate  channel [4]. Deprocessing artifacts are represented by  mechanically induced damaged sites in the silicon substrate.  These damaged sites are manifested in the form of silicon pits,  voids, slits and fractures resulting from the tensional or  shearing stresses in the silicon substrate when the polysilicons  separate from the silicon substrate.  Figures 12a and 12b  are  SEM photos of a valid and invalid ESD pinholes.

A DDM simulation of an artifact defect in one of the  SRAM transistors did not yield to the expected failure mode.  DDM process in this case was the more efficient approach  rather than conducting actual evaluations.

![T1,T2:Pull-up transistors  T3,T4:Pull-down transistors  T5,T6:Pass Transistors     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/370baede-db7f-4f9e-a55e-1275a116e252/370baede-db7f-4f9e-a55e-1275a116e252.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=1e2903a3cf2e1a1aa94fa106b8816d914627ebbb)
Figure 10. Focus Ion Beam X-section found silicide and contact formation  defect on the common source of the failing SRAM cells

![Simulation(Open Source-T6)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5074f005-e4c7-4e65-ad87-6d4d8a0e597c/5074f005-e4c7-4e65-ad87-6d4d8a0e597c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=778838d1ee3e91a7718460c3a298bf23b07bcc6a)
Figure 11. The stuck-to-low simulation has been confirmed when source of the  output pass transistor is isolated

## Demonstrate the Other Usefulness of DDM  

## a.   Wet Chemical Deprocessing Induced Artifacts Verifications  [2,3]   

Wet Chemical Deprocessing is one of the techniques in  exposing embedded structures in an integrated circuit (IC).  Layers of the die from the passivation to silicon substrate can be  selectively etched away using this technique. From series of  evaluations conducted, it was discovered that there were silicon  damage sites that were induced during wet chemical  deprocessing. Their physical attributes were identical to the  attributes of electro-static discharge (ESD) defects. It only

![          Figure 12a. Valid ESD defect: SEM  Figure 12a.Valid ESD defect: SEM   Figure 12b. Deprocessing artifact: A  Figure 12b. Deprocessing artifact: A  photo of pinholes underneath the  photo of pinholes underneath the   pit or void at the center of the channel  pit or void at the center of the channel gate oxide layer  gate oxide layer ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7b92bccb-672e-45a0-b863-73af4ecaf596/7b92bccb-672e-45a0-b863-73af4ecaf596.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=df1d3ec3a4d1506499f7fe0ba1287af26f0f1fd6)
## b.   Failure Mechanism Undetermined Investigation   

An electrical failure was confirmed to be SRAM array  related. Fault isolation analysis using C-AFM confirmed a  contrast anomaly on the VDD contact. See  figure 13.  PFA on  the part, inspecting all the layers of the die, did not uncover the  defect. DDM process was used to explain the potential defect  site.  See Figure 14.  From the simulation results, the defect site  was in the metal layers but was missed during the PFA.

![SEMImage  C-AFM+1Vbias ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2de159cd-91c5-4c4e-81e7-bf7ae2b610a7/2de159cd-91c5-4c4e-81e7-bf7ae2b610a7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=f33fa29ba8b59bda3cfe51e2b88bf1aa1ce13d05)
Figure 13. C-AFM showing a VDD contact via anomaly

![S  S1-short#1  S2-short#2  Memory fault model on SN2.Failure is simulated on S1 (short #1).  Short#1  VTo  11.1852  Stucktolowoutput  11.1851m  11.1850  Failure is simulated when VDD is shorted to input bit line (PMOS source-to-drain short).  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7bfa5f56-b2c8-4bdd-a419-506e1d9b8547/7bfa5f56-b2c8-4bdd-a419-506e1d9b8547.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215670%3B1743219270&q-key-time=1743215670%3B1743219270&q-header-list=host&q-url-param-list=&q-signature=306e97728b0231b35b32e43d3a9592a531960c9e)
Figure 14. DDM simulation results.

## IV. C ONCLUSION 

The DDM process was found to be effective in  identifying potential defect sites in the SRAM array. This was  exemplified by the successful simulation cases. The DDM  process was instrumental in generating defect databases. The  information in the database hastened the failure analysis  process; particularly, the fault isolation steps, as analysts had a  clear understanding of the layout and material stacking that  eliminated the tedious and time-consuming reverse circuit  engineering analysis procedure.  Furthermore, the DDM  process and defect database have shown that the prevailing  failure analysis challenges of the 65nm technology node can be  addressed by the process.

## A CKNOWLEDGMENT 

The author wishes to express his gratitude to the ADI  team from Failure analysis, TPG Product Line and Design  groups for their contribution on the analysis of the failures and  inputs to this technical paper.

## R EFERENCES 

[1]       PTI. (2013, June 6). “ IIT Mandi develops next generation IC chips. The  Economics   Times”    Retrieved   from  https://www.iitmandi.ac.in/news/articles/files/indianexpress_economi ctimes.pdf     [2]        R. Mendaros, et al.,  “Discovery of wet chemical deprocessing induced  artifacts – A common problem affecting all MOS and CMOS  Technologies” , ASEMEP 2016, Manila, Philippines.     [3]   R. Mendaros, et al.,     “Identification of Wet Chemical Deprocessing  Induced  Artifacts – A Common Problem Affecting All MOS and  CMOS Technologies”,  ISTFA 2016, Texas, USA    [4]        Analog Devices Incorporated. (2014). “ Reliability Handbook” .  Retrieved from  http://www.analog.com/media/en/technical-documentation/user-guide s/UG-311.pdf

