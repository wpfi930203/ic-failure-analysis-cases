---
title: "IPFA2022_tutorial_Introduction_to_scan_diagnosis_Jayant.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_9764365f74c659de6df6b0c2c481050b7295230462135641
file_size: 4965554
---

## An introduction to scan diagnosis 

Jayant D’Souza

Siemens EDA

SIEMENS

## Objective 

Scan testing is the defacto standard of testing digital devices  during manufacturing. Scan diagnosis, leverages the DFT  structures such as scan and ATPG patterns to localize defects on  failing die. This tutorial will give an overview of scan testing and  different scan diagnosis techniques that are available today. It will  also show how volume scan diagnosis can be leveraged to  perform yield analysis over the product lifecycle.

## Outline 

Overview of chip design flow   Principles of DFT and test   Principles of scan and ATPG test   Scan diagnosis   Volume scan diagnosis applications   Conclusion

## Chip Design Flow 

Typical chip design flow comprises several steps from  requirements gathering to product specification, and finally   product architecture definition

Design development begins at RTL and passes through several  stages before fabrication

## Chip Design Flow 

![Functional Coding  Functional Coding  Place Gates  Place Gates RTL  RTL  (Some DFT)  (Some DFT) Level  Level Clock Tree  Clock Tree  Verification Verification   Synthesis  Synthesis Physical  Physical Design  Design  Signal Routing  Signal Routing Logic Synthesis Logic Synthesis   (Layout)  (Layout) Gate  Gate  Verification  Verification Level  Level  DFT Insertion/  DFT Insertion/ Pattern Generation  Pattern Generation 70  No Verification Verification   Timing  Timing  Meet Timing?  Meet Timing? Closure  Closure Loop  Loop  Yes Yes  5 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c9c184bb-e090-414f-84cd-de44dfd39f62/c9c184bb-e090-414f-84cd-de44dfd39f62.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=ea7b6769d42e10a366f107016d6a30e01a6f8152)
## Chip Design Flow From Layout 

![Fabrication Fabrication  DFM  DFM Manufacturing  Manufacturing Test  Test PD  PD  Physical  Physical  Post-  Post-  Verification  Verification  Post Silicon Post Silicon  Processing  Processing  (LVS/DRC) (LVS/DRC)  Good Unit? Good Unit?  7O  No Tapeout Tapeout   Yes Yes  Diagnosis/ Diagnosis/  Ship  Ship Failure Analysis  Failure Analysis ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/30bbe57b-bf4f-461c-a1f9-7701576edcd7/30bbe57b-bf4f-461c-a1f9-7701576edcd7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=5ae2c247e1ec0a2ba67f806d4923fdb97dc741e6)
## Why do we test? 

Ensure outgoing quality   Does every unit shipped function completely and reliably?     Cost to replace parts grows exponentially throughout design cycle     Cost of bad part in critical device is immeasurable (for e.g. a pacemaker or  airplane)

![\$1000  \$1000 \$100  \$100 \$10  \$10 串！  \$1 Analysis  Analysis  Design  Design  7  Test  Test  Field  Field ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/92133526-e338-43b3-bc23-a95314d62d24/92133526-e338-43b3-bc23-a95314d62d24.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=a8755bab043899e94fb4ec6ac697728b13bcbf18)
## Why do we test? 

Valuable information gained from testing that can be leveraged  for:

Yield improvement   Reliability (e.g. defect clustering)

## Manufacturing test 

Wafer probe testing   Cost effective to test most products   \$(Package +  Burn In  + Final test insertion) > \$(Wafer probe)     Package level test   Usually only for tiny die on mature process + Cheap package → Blind  Assembly

## Why not functional patterns? 

Designers generate many patterns (i.e. testbenches) that  exercise functional modes

Intended to verify functionality by exercising functional modes of  operation(i.e. does the design perform the correct functionality)

Not designed to target all defect types

Requires in-depth knowledge of the design

Prohibitive time and effort required to achieve good test  coverage

## Why not functional patterns? 

Functional verification patterns are not efficient in terms of test    data volume and test time     Does not necessarily verify that part was manufactured    correctly     Typical stuck-at coverage of functional patterns <= 70%     Limited  Controllability  and  Observability   Primary inputs for Control   Primary outputs for Observe

In this section, we covered ...    a high-level introduction to chip design   different manufacturing test techniques   The efficacy of using functional test patterns

## Principles of DFT and test 

## What is DFT? 

DFT = Design-for-Test

Comprises strategies to structurally test design with the  goal of:

Improving product quality by detecting defects   Making it easier to generate vectors   Reducing vector generation time   Reducing cost of device

## Benefits of using structured DFT 

Repeatable from one design to another Does not require deep knowledge of the design

Automated by tools algorithmically Can easily measure quality of test (For e.g. test  coverage) Efficient test data volume and test time

## Benefits of using structured DFT 

Increases productivity:

Quicker time-to-market Shorter design cycle time Reduced cost of test Improves product quality: Reduced Defective Parts Per Million (DPPM)

## Product yield as a function of defect  coverage 

![Defect Level  Defect Level 959  95% 1-○  1.0 Y=0.1  Y = 0.1 0.8  0.8 Y = 0.25  Y = 0.25 0.6  0.6 Y=0.5  Y = 0.5 ○.4  0.4 Y = 0.75  Y = 0.75 0.２  0.2 Y=0.9  Y = 0.9 0 20  20  40  60  80  80  10:0  100 Defect Coverage (%)  Defect Coverage (%) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/609627aa-94d2-4884-91a8-fb09f430b079/609627aa-94d2-4884-91a8-fb09f430b079.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=6477dbb4ffdcf8bf559fa62b62c8d44837c5b22b)
$$D L=1-Y^{(1-d)}$$
where\*:    ${\pmb d}=$   defect coverage   DL  (Defect Level)  $=$   Shipped parts that are bad in   Defective Parts per Million (DPM)   Y  (Yield) = number of defect-free parts   d  (Defect coverage) = # of defects detected / total # of defects

![Some guideline values, assuming  Some guideline values, assuming  DPM = 50:  DPM = 50: Y=> 60  Y=> 60       80       90       95 80   90   95  d => 99.99 99.97 99.95 99.90  d => 99.99  99.97  99.95  99.90 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b4811fae-0f0e-4297-81e7-5943d345aa80/b4811fae-0f0e-4297-81e7-5943d345aa80.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=ff7664b13797ebc3f6d729c69783f8d32a4713b3)
## Structured DFT  

##   Scan 

All flops/latches become virtual windows into the design   Accessed via a shift path during test mode   Enabling Technology

## Structured DFT Methods 

Automatic Test Pattern Generation (ATPG)

Built-In-Self-Test (BIST)   Logic BIST   Based on scan architecture   Pattern generation achieved by on-board logic   Results compared on-board   Memory BIST   On-board state machines generate patterns in specific algorithmic steps targeted  at Memory defects

## Defects vs. Faults 

What is a defect?   What is a fault?   What is the difference?

## Defects 

A defect is a physical fact     Devices fail due to manufacturing problems   Contamination   Insufficient doping   Process or mask errors   Metal trace opens/bridges   ...

![TOP-SDB1-  SYSCPUOUT  VCC   -DATA_OUT  SEL_6[0]  20.0kV ×9.99k3.00#m  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/41eb9bf8-7533-4137-ba59-14a4f7962007/41eb9bf8-7533-4137-ba59-14a4f7962007.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=b248022fa2f6fe7c9de0dd4f3c5e78ccf3a82bf7)
Defects can result in   Shorts to power/ground or neighboring nets   Slow transistors   CMOS stuck-on/open   Open/broken nets   ….

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5fad0bed-dacf-47d9-bf43-998713169580/5fad0bed-dacf-47d9-bf43-998713169580.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=a43883a4c96970a698e8418cbc1e8c9e11861fdd)
## Faults 

Faults are a model of the “effect of a defect”     They are abstractions of physical defect behavior     Provide logical description of defect behavior     Provide a unit of measure, e.g. for test coverage and fault coverage

![TOP-SDB1-  SYSCPUOUT  VCC   -DATA_OUT  SEL6[0]  99k3.0m  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/02f38c56-6a69-4388-9c6d-137d1d0aa896/02f38c56-6a69-4388-9c6d-137d1d0aa896.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=ceea9c62642f68fa43118124cbe9d5c164e77e73)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/548f2da9-ad1c-4303-8440-e446dcd22e1c/548f2da9-ad1c-4303-8440-e446dcd22e1c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=c974deddf08baddd5a0256512aee7870cdeef0a8)
Defect

## Fault Models 

Fault models provide a mechanism to emulate defects so test  patterns can be generated to identify the defects   A fault is detected when there is an observed difference  between good behavior and faulty behavior   The most common fault model is a stuck-at fault model

## Traditional logic fault models 

Stuck-at   Models a permanent high or low value at gate terminals

![s-a-0  X  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/95079678-ff3f-44f5-b326-936936d83577/95079678-ff3f-44f5-b326-936936d83577.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=145b3f1de6999db6cec03f5b8ca7b050bf276938)
|13|Good||A s.a.1|
|---|---|---|---|
|||As.a:0||
|||||
|||||
|||||
|||||


## Traditional logic fault models 

##   Transition 

Models gross delay on gate terminals   Terminals are slow to rise or fall

0

1

b

AND(0, b)

AND(1, b)

## Other logic fault models 

Path delay   Models combined delay along a path though the circuit.   Paths are slow to rise or fall     IDDQ   Models high current flow through a gate

## Defect-based testing 

Maps logical tests to physical domain to target specific defects

![上三 - 下-- 15 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c561a1a4-c4f5-493a-9c15-ca8e77ea5d49/c561a1a4-c4f5-493a-9c15-ca8e77ea5d49.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=f4bda804a38d068b44c0e72b753ff9cf6c037076)
## Newer fault models and test methods 

Layout-aware test

Extractions from physical database   Deterministic method

Cell-aware test   Uses parasitics inside standard cell to model defects

![3-0L-83  potential bridgelocation  net1  net2  widemetal  in layerx    signalsinlayerx+1  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3b0d2b53-7f2b-47fe-bea2-706f1e18d5e0/3b0d2b53-7f2b-47fe-bea2-706f1e18d5e0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=cdea904cca921ac167f6ca117cc49880f5cb3476)
![open  defect  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/56339eaa-f5cf-4349-807d-45d6653a0992/56339eaa-f5cf-4349-807d-45d6653a0992.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=67c74d4c02901a48af1f39e1feafeb1f76650a0a)
## Why is a fault model important? 

A fault changes the good (or fault-free) function  g  of a modeled

circuit into a faulty function  f.   We can represent this in a computer.   Makes faults ‘countable’   How many have been detected?   Measure of ‘quality’ of the test

In this section, we covered ...

an introduction to DFT and structured DFT techniques     the impact of DFT on product quality     abstractions and models of circuits and faults     the difference between a fault and a defect     the principles of traditional and some of the newer fault models and test   methods

## Principles of scan and ATPG 

## Scan Flip-flop/Scan cell 

Fundamental test device in scan testing   Replaces D-flip flops   Enables ATPG-based testing for a design

![Replaced by  Replaced by MUX-D Scan Cell MUX-D Scan Cell  Original  Original Flip-Flop  Flip-Flop D  ２_２  N_2  DFF1  DFF 1 D  Q SI  SI  D  scan_out  scan_out SE  SE  MUX1  MUX 1  DFF  DFF  CLK  CLK CLK  CLK ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ed873011-4f41-40e6-a849-17d368307dfb/ed873011-4f41-40e6-a849-17d368307dfb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=c38276017975e7bd45ceaebe75aa46c1c8480717)
## Scan testing 

Scan test is a process/flow that:

Creates control and observation points by replacing flip-flops with scan cells     Connects the scan cells together to create scan chains     Utilizes these scan chains, test patterns (typically ATPG) are generated that:   Set a specific value at a specific node (Control)   Propagate the result so it can be measured (Observe)

![SI SD  SO SE  SE CLK  33 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ff409074-a4d9-4636-9ee5-f01dfd7f15ce/ff409074-a4d9-4636-9ee5-f01dfd7f15ce.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=0d9411fdbe4e77b54390c4950b8fab88d14952f6)
## Automatic Test Pattern Generation (ATPG) 

For a given fault from a fault model:

How to find a sequence of input stimuli that can distinguish the  good circuit from a faulty circuit?

Note that fault model determines detection conditions

## ATPG on a single gate 

Find a sequence of input stimuli that distinguish good value  from faulty value

$\mathsf{a}\!\!=\!\!1$  , b=0 will cause a difference at the output of the faulty gate   (1,0) is a test for the stuck-at 1 fault at b

![a y b stuck-at 1 stuck-at 1  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/73a40f1c-c8bd-45b8-9812-927ff0a25002/73a40f1c-c8bd-45b8-9812-927ff0a25002.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=37e0e7779b0e1231e87ef83fb97f3b62a370bdf5)
test

|Good y|Faulty y|
|---|---|
|||
|||
|||
|||


## Test generation 

Test patterns accomplish 2 things:   Fault activation (control)   Fault propagation (observe)

![1  Fault Activation  Fault Activation SC  SC  Test for  Testfor  Stuck-At O  Stuck-At 0 1  1 SC  SC  1 0  0  1  [1] SC  SC  SC SC  0 SC  SC 1 SC  SC  1 1  X  XI  [X] Fault Propagation  Fault Propagation  SC  SC  X  SC SSC  1 SC  SC ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/616bfd1e-b873-4082-9932-856a2a57bfdc/616bfd1e-b873-4082-9932-856a2a57bfdc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=ae4efa212759edb0aba959a6bb5062e6b164834c)
## Test generation 

A  test cube  minimum defined values needed to control and    observe a fault site     All X-states on control side are  random fill     All X-states on observation are  masked  during unload

![1 SC  SC  Test for  Test for  Stuck-At O  Stuck-At 0 X  1 SC  SC  1 Control  Control  0  0  1  [1] Observe  Observe  SC SC   SC  SC Fill  Fill  X SC  SC 1 SC  SC  1 1  X  XI  [X] SC  SC  X  SC  SC 1 SC  SC ③7  37 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a13b96ab-11b0-4974-9a53-9e7c66191372/a13b96ab-11b0-4974-9a53-9e7c66191372.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=cf7f98d2d4f8c31f3acc2f24c169b3728c89dbad)
## Test Generation 

Previous example is a simplification of test generation      ATPG tools are much more complex     Actual ATPG uses numerous heuristics and optimizations for  run time, memory usage, etc.     ATPG generally tries to generate fewest patterns with highest  test coverage

## How ATPG Works 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/754a6296-682a-42a4-9656-1a6215c8aa0b/754a6296-682a-42a4-9656-1a6215c8aa0b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=4d8c64cb69752f73f05db7c6c5fb95c2e381a2a5)
4. Stimuli on ATE

5. Response for  fault-free circuit

1. Target faults 2. Generate test cube:    specified bits: 1-5% 3. Random fill: 99-95%

## Principles of test generation 

![….  …. Good circuit function  Good circuit function   Faulty circuit function  Faulty circuit function  g  f …. …. XOR XOR   XOR  XOR  ….  XOR  XOR CF  OR ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fc31ec79-b9f8-402f-9771-c6b7582c30b5/fc31ec79-b9f8-402f-9771-c6b7582c30b5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=c46eaa8c221ed61c1e81767c5ad0339baac70ea7)
## From the ATE point of view 

![….  …. Good circuit function  Good circuit function   Faulty circuit function  Faulty circuit function  g  f …. …. Expected values Expected values   ≠  Measured values  Measured values  =>  Defective part  Defective part ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4d66f542-8cd9-4fac-bbc7-1694a58254d6/4d66f542-8cd9-4fac-bbc7-1694a58254d6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=e8bec4de5d1bbd6051a7215eb06600ab569e3a6f)
## Basic Scan pattern 

Basic scan test contain the following events: Basic scan test contain the following events:

![1. 1. Load scan chain (many cycles)   Load scan chain (many cycles)  PULSE CAPTURE  PULSE CAPTURE 2. Force primary inputs (PI)  2.  Force primary inputs (PI)  Clk.  CLK. 3. Measure primary outputs (PO)  3.  Measure primary outputs (PO)   Capture cycle  Capture cycle  Capture  Capture Cycle Cycle  4. Pulse capture clock  4. 5. 5. Unload values from scan cells   Pulse capture clock  Unload values from scan cells   Force PI Measure PO  capture clock 一  S  1 Load next pattern  Load next pattern  Load Scan Chain  Load Scan Chain  Pulse …. CLK  CLK B  SIE   SE  SE CILK  PIS  PIs  X X PD  PO ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7484152e-f51b-49a9-91a3-6c9eecfa9a81/7484152e-f51b-49a9-91a3-6c9eecfa9a81.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=cee5fa0b00505877271c84df8b89ee1eaa4de80c)
## Basic Scan Test (Cont.) 

Load values into the scan cells

1.  Force SE to “1” (scan enable)   2.  Force SI (scan chain input pin)   3.  Pulse shift clock   4.  Repeat steps 2 and 3 until all scan cells are loaded   1 st  Shift

![1st Shift 1st Shift  A Y B  SE SE-S  SI CL 01 1  1  SO  K SI  D  Q  D  Q  D  Q 1 SE  SE  1 CLK CLK  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fbd005c8-0029-48a2-b7a7-15651a5c1bfb/fbd005c8-0029-48a2-b7a7-15651a5c1bfb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=416118f24155e20ca7129cb5da09c24fe2e52e13)
## Basic Scan Test (Cont.) 

Load values into the scan cells.

1.  Force SE to “1”   2.  Force SI   3.  Pulse shift clock   4.  Repeat steps 2 and 3 until all scan cells are loaded   1st   2nd

![A Y B 0 11  1  1  SO SI  D  Q  D  Q  D  Q 1  1 SE  SE  1 CLK  CLK ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d51ba8d8-9de5-462c-aad3-725d04fe1296/d51ba8d8-9de5-462c-aad3-725d04fe1296.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=385f84eff4385b44e5a42bd2afc7414b4580f776)
![ist   2ndl  Shift  Shift  Shift  Shift SE SE  S  SI ！  CL K ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2552e67d-c639-4655-a920-9452de22b7a8/2552e67d-c639-4655-a920-9452de22b7a8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=bc651112b4a43ebc33610f9143cbad5f48b33b93)
## Basic Scan Test (Cont.) 

Load values into the scan cells.

1.  Force SE to “1”   2.  Force SI   3.  Pulse shift clock   4.  Repeat steps 2 and 3 until all scan cells are loaded


![3rd Shift  3 rd  Shift   1st  1st   2nd  2nd   3rd  3rd Shift  Shift  Shift  Shift  Shift  Shift A Y B  SE  SE S  SI 0151  0 11  SI S   0  HPORT!  D  Q  1  D  Q  1  D  Q  SO  CLK  CLK 0  1  1 SE  SE  1  -LOAD  LOAD CLK  CLK ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1a6ce552-0338-44de-8ad2-745f9ed9ef20/1a6ce552-0338-44de-8ad2-745f9ed9ef20.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=b7ebdb632a3ecb5cb12bce3ae965699ee01b261f)
## Basic Scan Test (Cont.) 

Force primary inputs   Force normal primary inputs   Force SE to “0” (exits shift mode)   Now all internal values can be predicted

||LOAD|
|---|---|
|        Capture                Cycle      |FORCE PI|
|        Capture                Cycle      |MEASURE PO|
|        Capture                Cycle      |PULSE CAPTURE|
||Clk.|


![1 B A 1 1  1 0  1  1 1  1 1  Y  SE A B SI  D  Q  D  Q  D  Q  SO  SO  Force PI 0  1  1 0 SE  SE CLK  CLK ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5d0ce15e-0b87-4f76-9df9-8c366e216f9f/5d0ce15e-0b87-4f76-9df9-8c366e216f9f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=0373c929525cfd24245ccf2d3aa2e6e587d9672d)
## Basic Scan Test (Cont.) 

![LOAD  LOAD Measure primary outputs Measure primary outputs   FORCE PI  FORCE PI Capture  Capture   MEASURE PO  MEASURE PO ·Measure "1" on Y  Measure “ 1 ” on Y  Cycle  Cycle  PULSE CAPTURE  PULSE CAPTURE Clk.  CLK. 1 A 1 1  1 山jL  1  1  1  1  Y  SE B  0  1  1 A B SO SI  D  Q  D  Q  D  Q 0  1  1  Y 0  Measure PO CLK  CLK SE  SE  Force PI SSE  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/534817a7-f1c4-41f2-8ce8-d4d31a3e02a7/534817a7-f1c4-41f2-8ce8-d4d31a3e02a7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=08e1949254435228efd9acbf3ec1c68576dea3b6)
## Basic Scan Test (Cont.) 

Pulse Capture Clock

Loads scan cells with functional inputs

to observe circuit status

![LOAD  LOAD FORCE PI  FORCE PI Capture  Capture   MEASURE PO  MEASURE PO Cycle  Cycle PULSE CAPTURE  PULSE CAPTURE Clk.  CLK. ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9d8dc79b-de06-4575-8499-6832782c5e86/9d8dc79b-de06-4575-8499-6832782c5e86.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=3c115c9cd960caf1dfb921f9f53376873370abb0)
![1 A 1  1  1  1  1  CLK  CLK B  1  0  1  1  1  Y  SE  SE A B SO SI  D  Q  D  Q  D  Q 1  1  1  Y 0  Measure PO DC   Pulse capture SE  SE CLK  CLK  Force PI  CLK Capture Cycle  Capture Cycle ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3d3fa837-e560-4462-9ee8-18fd2427450d/3d3fa837-e560-4462-9ee8-18fd2427450d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=511ec07f700a0c5c716a13bbb2119ae1fb2401bb)
## Basic Scan Test (Cont.) 

Unload the scan chain

As new data is being shifted into the scan chain during load serially, the previous internal circuit state is being  serially shifted out and measured at scan out (SO)

![LOAD/  LOAD/  UNLOAD  UNLOAD A  1st  1st  2nd  2nd  3rd  3rd B  Y  Shift  Shift  Shift  Shift  Shift  Shift SE  SE RRR   LOAD  LOAD S  SI 101 1 0.1   SS  SI  1  D  Q  0  D  Q  1  D  Q  1 1 1  CLK  CLK 1  0  1  SD  SO  UNLOAD  UNLOAD SO SE  SE  1 CLK  CLK Previous internal state  Previous internal state Measure_sco  Measure_sco  of scan cells measured  of scan cells measured at scan out  at scan out ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5a466cff-441a-4be8-af8e-0c79f41ef417/5a466cff-441a-4be8-af8e-0c79f41ef417.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=0d3d35974507b3e7eef1554f89b1b74d595f2f12)
## ATPG and scan patterns 

ATPG is entirely focused on “capture”

ATPG comprises two major parts   Test generation   Simulation     Simulation of the tests generated for fault-free/“good” circuit    values stored in the pattern set   “Fault” simulation to ensure that a targeted fault will cause a difference  in good circuit response.

## Scan test patterns 

ATPG will try and detect all faults using the most compact    pattern set     The faults detected are in design logic outside of the scan chain     ATPG test pattern set for the ATE typically comprises:   Chain tests – to verify integrity of scan chains/cells   Scan tests – to verify integrity of logic and paths between scan chains

## Summary 

In this section, we covered ...

how an ATPG tool works,     How ATPG is a very complex task,     How scan technology can be used by ATPG to structurally test a design

## Scan diagnosis 

## Overview of the product flow 

ATPG test patterns are used during manufacturing test to  screen out bad parts eioutpaaparts

![Good  Good   Ship to  Ship to  Devices  Devices  customer  customer Manufacturing  Manufacturing Pattern  Pattern   Test  Test Generation  Generation  scan  Scan   Statistical  Statistical  FAIL  FAILPASS  Diagnosis  Diagnosis  Analysis Analysis  Test Patterns  Test Patterns      Defect  Defect  Localization  Localization ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5a133b21-4f7e-42ff-ac6c-ec66b4fdaffd/5a133b21-4f7e-42ff-ac6c-ec66b4fdaffd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=b298c339375e77a3c2099043072ea1a80bcf043d)
## What happens to the failing parts? 

Diagnosis uses a log of the failing cycles to identify and isolate  defect and defect locations

![TesterFailure  LogFiles  Identify/ranksuspects  thatmatchfailingdata  Suspected defects  Classify defect behavior;   Defect   open,short,delay,and so on  Classification  Defect  Isolatedefecttophysical  Markthe   lsolation  feature(s); vias, segments,  Failing die  layer  Physical Defect  55  55 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c41bfa0f-3a18-428b-9d92-cdbbc9fe3ff0/c41bfa0f-3a18-428b-9d92-cdbbc9fe3ff0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=46b84d5ba01831537774fdcd55a410a07aae9f19)
## Defects 

Static defects – always cause the same failure     Delay defects – defects that affect long paths     Parametric defects      Others …     These defects could occur in back-end layers or in the front-end

## Diagnosis process 

Diagnosis is a simulation-based technique to identify defects  and defect locations     Activation conditions, observation conditions both considered  during the diagnosis process     ATPG fault type is an abstraction of a defect     Diagnosis uses that abstraction to model silicon defect behavior

## Scan Test 

![10011010  01011  1001001  0011101  1100011  Test Patterns Test Patterns  STIL  STIL 1001101  0001101  1101011  ATPG  ATPG Design w/scan  Design w/scan Verilog netlist Verilog netlist  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a825e27d-9f46-41c7-9ad4-1bed7b164dea/a825e27d-9f46-41c7-9ad4-1bed7b164dea.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=290f740d1b941ce2098a1bdb0b14bf2cc02c2c01)
## Scan Test 

![1001001  0011107  1100011  Test Patterns est Patterns    Stimuli  Stimuli   Shift in  Shift in  Capture  Capture  Shift out  Shift out  Response  Response STIL  STIL 00001101   10100110  1 0 1 0 0 1 1 0  -0-1-1-0-0-1-1-1-  0 1 1 0 0 1 1 1 1101011  Logic  Logic X ATPG  ATPG  11101100  1 1 1 0 1 1 0 0  70-1-1-10-1-0-0-  0 1 1  1  0 1 0  0 Defect  Defect  Logic  Logic 0001010  0 0 0 1 0 1 0 1  10-0-0-0-0-000-  0 1 0 0 0 1 1 1 Design w/scan  Design w/scan Verilog netlist  Verilog netlist ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8a94bb1a-7102-45b8-9058-66147a65d64e/8a94bb1a-7102-45b8-9058-66147a65d64e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=e27b23783bc37365a2d8163636f54d7b15e859f4)
## Scan test and diagnosis flow 

![1001001  0011107  1100011  Response  Response Test Patterns Test Patterns  STIL  STIL 1001101   01100111  0 1 1 0 0 1 1 1 0001101  1101011  Logic  Logic X ATPG  ATPG  0 1 1 111010   1  0 1 0  0 suspect  Suspect  Logic  Logic  Failures  Failures 0 1 0 0 0 1 1 1 1000111  Design w/scan  Design w/scan Verilog netlist  Verilog netlist ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ad342c82-3e06-449e-8887-e8bc04a260ae/ad342c82-3e06-449e-8887-e8bc04a260ae.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=9d5de6141340479ad4c0ded766ec99fbdbb57b6c)
## Scan test and diagnosis flow 

![1001001  0011107  1100011  Fail  Fail data  data Test Patterns Test Patterns  STIL  STIL Scan  Scan 1001101  0001101   diagnosis  diagnosis  0 1 1 0 0 1 1 1 10011  1101011  01100111  Logic  Logic 01110100   X ?ATPG  ATPG  Logic   RFailures  01000111   0 1 1  1  0 1 0  0 Logic  Failures  Failures Logic  Design w/scan  Design w/scan  010001  0 1 0 0 0 1 1 1 Verilog netlist  Verilog netlist ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2bfcea5d-86ca-49ba-8ea6-81631f07921f/2bfcea5d-86ca-49ba-8ea6-81631f07921f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=cc203eab759519b1771bfb774d6eba8232ce482d)
## Layout-Aware Scan Diagnosis 

![1001001  0011107  1100011  Fail  Fail  Defect classification Defect classification  data  data  Physical location  Physical location Test Patterns Test Patterns   Logic location  Logic location STIL  STIL 1001101   Scan  Scan 0001101   diagnosis  diagnosis  X23   Jreg_out_bit_to_tdc  1101011   instr_reg_0  X区  01100111  XX  mux21_ni  01110100  ATPG  ATPG  Logic   Failures  01000111    Diagnosis produces physical call-outs  Diagnosis produces physical call-outs     Physical call-outs provide valuable classifications for yield  Physical call-outs provide valuable  classifications for yield  Design w/scan  Design w/scan  analysis  analysis Verilog netlist  Verilog netlist  Layout   Layout LEF/DEF  LEF/DEF  Reduced suspect area accelerates failure analysis (FA)  Reduced suspect area accelerates failure analysis (FA) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/df8756fb-cf82-4f16-8fad-99511c44d462/df8756fb-cf82-4f16-8fad-99511c44d462.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=a2b1c2fff1219a5473de93d383f6737de1a649fa)
## Scan diagnosis flow 

Scan diagnosis comprises:   Chain diagnosis   Logic diagnosis     Chain diagnosis is performed first if chain failures are found     Logic diagnosis performed if all chain tests pass

## Diagnosis process 

•  Extracts circuit of interest based on captured failures

•  Becomes an identified defect region

Applies defect models to circuit of interest and simulates failing  patterns

If defect model simulation matches observed failures it becomes a  suspect

Simulates passing patterns to improve result resolution

•  Uses layout information to determine possibility and location •  Becomes a layout suspect if justified by layout

## Scan diagnosis process 

Diagnosis simulation identifies the areas of interest in the  design based on failing cycles

![H  Logic  Logic  OHEHE  EOHEHO  Ldgic  Logic  Defect   Logic  OHHE  Relevant portion of  Relevant portion of  Full design  Full design  (With  (With passing and failing cycles)  passing  and  failing  cycles)  design for diagnosis  design for diagnosis  of specific fail log  of specific fail log ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/77c64f77-6aa9-4315-b356-1e5218288d2e/77c64f77-6aa9-4315-b356-1e5218288d2e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=4d33583f476e2b65fc2901c503ed8eddc92af36b)
## Chain Diagnosis Internal Process 

![Chain patterns  Chain patterns  Scan patterns  Scan patterns  Flat Model  Flat Model 10011001001   1001101000  1001001100   11011101010   ATPG  ATPG Chain pattern  Chain pattern  failures  failures 10011000000   Step 1:  Step 1:  Step 2:  Step 2: 0001001100   Identify faulty chains  Identify faulty chains  Identify suspected faulty scan cells  Identify suspected faulty scan cells Scan pattern failures  Scan pattern failures 110100100001  011100010  Chain diagnosis Chain diagnosis  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/297a645c-690e-4dff-be90-53f8d0076869/297a645c-690e-4dff-be90-53f8d0076869.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=032659e4d51d798f0526ec231b7afedec1c5854c)
## Identification of faulty chains (and defect type) 

![Shift In  Shift In  (No Capture) (No Capture)   Shift Out  Shift Out 001100110011 001100110011   001100110011 001100110011  Good chain Good chain  Logic  Logic 001100110011 001100110011   X  11 111111111111  11 11 11 11 11 stuck-at 1  stuck-at 1  Logic  Logic  Observed failures  Observed failures √√√√√  001100110011 001100110011   X 00 000110011001  0 1 1 0 0 1 1 0 0 1 Hold-time Hold-time  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c00d352b-0faa-4e86-8b06-ef075dcd4318/c00d352b-0faa-4e86-8b06-ef075dcd4318.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=54c95192f32ace8b79ab818a3628c012b40b15da)
Page 67

## Determining chain defect type 

•  Assume shift-in pattern: 001100110011

| Shift out|Fault type|
|---|---|
|001000100010|Slow Rise|
|011101110111| Slow Fall|
|011001100110|slow|
|101110111011|Fast Rise|
|000100010001|Fast Fall|
|100110011001|Fast (Hold-time)|
|000000000000|Stuck-at-0|
|111111111111|Stuck-at-1|
| Other patterns|Indeterminate|


## Locating defective scan cell in chain 

![Shift In  Shift In  Capture  Capture  Shift Out  Shift Out 001100110011  001100110011  1  0  1  0  1  0  1  1  0  0  0  1  101111010110  1011110 1 011 0 Logic Logic  100010110101 100010110101   1  0  0  0  1  x  1  1  0  1  0  1  111111 111111011010  01 1 010 stuck-at 1  stuck-at 1  Logic 101010110001 101010110001   1  0  1  0  1  0  1  1  0  0  0  1  101001100111  10 1 0011001 1 1 Page 69  Page 69 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e75d9150-7ae0-4091-a5cd-a5d91211afc1/e75d9150-7ae0-4091-a5cd-a5d91211afc1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=27e62b8069e2a3387c1d1547e5437bee9dedf78a)
## Chain diagnosis 

More chain defects in:   Early process ramp   Early product ramp (NPI)     Usually tapers off with process/product maturity     Can be as high as 50% even at mature process/product    lifecycle

## Logic diagnosis 

Locate defects in design logic outside of chains   Assumes chains are working correctly   Diagnosis is performed using logical simulation   Several defect models and heuristics applied   Physical layout information used during the process   Critical for FA usable diagnosis results

## Logic diagnosis process 

![Logic   Defect Simulation Defect Simulation  + Logic   Layout validation Layout validation  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/88c1e44c-12af-42e6-a888-bf0eb62dbcb6/88c1e44c-12af-42e6-a888-bf0eb62dbcb6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=53a18231279674bd4962e2fed1c70c6b1485b0a0)
## Layout-aware diagnosis 

Dramatic suspect reduction

Eliminate false bridge / open suspects   Detailed bridge / open classifications   Analyze net topology for suspect segment   Defect bounding box

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/327f6f1b-4e2b-4d76-9423-119ec2a9722b/327f6f1b-4e2b-4d76-9423-119ec2a9722b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=f72679a3613c23994b709d5bd1eee8cce5e4aa37)
The foundation for effective yield analysis   Physical call-outs provide valuable  classifications for statistical analysis

Reduced suspect area accelerates FA   Report X, Y, and layer   Marker files for effective layout viewing

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e8b75171-311c-4ada-b480-604df9c6238f/e8b75171-311c-4ada-b480-604df9c6238f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=a955b6f9aa93ec6419d07aba6ce9e85c84a84d00)
## Layout-aware diagnosis 

Traditional Logic Diagnosis

## Layout-Aware Diagnosis 

![M3 M2 M1 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fe1e5d21-dcb5-4887-b0eb-368232cb2e21/fe1e5d21-dcb5-4887-b0eb-368232cb2e21.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=f047a73fa7a0cbe2e31ea5725e13a4825f610d9e)
![B3 B2 B4 B5 B1 B7 B1 3broken  B8 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3007bbac-2bf5-4554-b55e-86eec09e5671/3007bbac-2bf5-4554-b55e-86eec09e5671.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=fee197d7cae7a7e3174fc567285ef9d5ae46f53d)
Suspect types: OPEN and DOM   Possible Bridges:  99   Possible Open Segments:  14   Suspect area:  1,192µm2

Y.-J. Chang, et.al., “Experiences with Layout-Aware Diagnosis,” Electronic Device Failure Analysis, May 2010

Suspect types: 1 (OPEN)   Possible Bridges:  0   Possible Open Segments: 1   Suspect area:  130µm2

## Combining layout and simulation… 

Layout-aware diagnosis of Open suspects on the same net.

![Sink Faill  Pass  Pass Pass  Pass Sink Fail  Driver  Driver Layout-aware diagnosis rejects the potential Open suspect because  Layout-aware diagnosis rejects the potential Open suspect becal  Pass  Pass the interconnect doesn’t support a single open failure; suspect list  the interconnect doesn't support a single open failure; suspect li  will be different between basic and layout aware diagnosis will be different between basic and layout aware diagnosis  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/187a4e48-001f-49d3-9260-30c5a0bc09aa/187a4e48-001f-49d3-9260-30c5a0bc09aa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=3490d15a323ea59a1f984e5cd17f3e45e0faf008)
## Combining layout and simulation… 

Layout-aware line of sight bridge. yout-avwaieieoisiglitpiiuoe

![A  Sink Fail  Pass  Pass Driver  Driver C  Pass  Pass B  Sink Fail   Driver Driver  In order for a bridge to exist between A  In order for a bridge to exist between A  and B, C must not exist and B would most  and B, C must not exist and B would most  likely need to be closer to A likely need to be closer to A  Pass  Pass ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2c0ba2c7-df79-40a6-a12f-50843c562acf/2c0ba2c7-df79-40a6-a12f-50843c562acf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=54a23d7fccde2e01606a393d2bb870804326e8be)
## Combining layout and simulation… 

![Pass  Pass Pass  Pass Sink Fail  Sink Fail  Driver  Driver Metal3 (X, Y, area)  Metal3 (X, Y, area) Suspect area enclosed  Suspect area enclosed   Metal4 (X, Y, area)  Metal4 (X, Y, area) in red polygon indicating  in red polygon indicating   Via3 - Single  Via3 – Single Pass  Pass  probable defect area  probable defect area  Via3 - Double  Via3 – Double … ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5f35f859-28d7-4891-814a-3960407d2716/5f35f859-28d7-4891-814a-3960407d2716.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=1f4f9b65bb0565530c938499633c7dcf948caf4d)
## Layout Aware – Bridge Resolution 

Layout-aware diagnosis identifies which segments of the nets  can be bridged

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/241b576f-3a15-47dc-a3d2-7d8a8ac29132/241b576f-3a15-47dc-a3d2-7d8a8ac29132.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=58464f3f7983580c7e21e1631a0f85d298c28888)
## OPEN Defect localization using diagnosis 

![Suspect OPEN  segment  Failing  sinks  Suspect OPEN  Suspect OPEN  Passing sinks  segment  segment ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/49403dfe-73b9-42cd-97fd-83abf0aac35a/49403dfe-73b9-42cd-97fd-83abf0aac35a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=e6b054751b5ef728ebc9f3488a2401c6524b21e4)
## Localization of suspects within a cell 

Suspect bounding box  includes complete cell

All locations in the cell are  deemed equivalent

PFA search area  localized to suspects  within cell

![Suspect  Suspect  bounding box  bounding box ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/896fd2a3-65dd-4433-b1b1-39937191286c/896fd2a3-65dd-4433-b1b1-39937191286c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=2817e6b4b49a31bda3e6b9e06ee87148e9dd525b)
In this section we covered…

The basics of scan diagnosis     The basics of chain diagnosis and logic diagnosis     How layout-aware diagnosis can be used to localize defect    areas for FA

## Volume scan diagnosis  applications 

## Using diagnosis results…. 

## Location  

PFA

![2了  Ireg_instr_reg_o.  ELE..  mux21_ni  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/65ad088c-a33e-4ff5-8a50-62693948fb00/65ad088c-a33e-4ff5-8a50-62693948fb00.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=419ecb40707fb3ba044e6bc41d3cd71e220e7efd)
Netlist pathname

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/006e8a7a-e675-46a7-aba8-31ad79b2ebbd/006e8a7a-e675-46a7-aba8-31ad79b2ebbd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=ac3777f3c8653a16dedb1ac71b653a5684c495cb)
Defect Bounding Box

![Location Properties Location Properties   Yield Learning Yield Learning  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9a7a7a29-b04a-4bce-9299-23a99588a844/9a7a7a29-b04a-4bce-9299-23a99588a844.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=17634dc813b2e6f4252f2eccca482c5b62620a60)
Bridge

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/80ac1938-9e4b-4b66-8543-be9cba9df31e/80ac1938-9e4b-4b66-8543-be9cba9df31e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=b57036a278d2b52afcc1ed83cf92f19ff0c56704)
![Driver  Suspectarea  Driver   NetB  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f58b82d8-a721-4b8a-9bc5-c3aa59ae4205/f58b82d8-a721-4b8a-9bc5-c3aa59ae4205.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=bb928266ba31df66b3936ab028e523282f01ced8)
![Open  Open suspectarea  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/25bd64ea-8401-4ae5-9c21-de2a42124502/25bd64ea-8401-4ae5-9c21-de2a42124502.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=f9f25c20869ff3d3f27de40edecd14a00bfaa5a4)
•

Library Cell Name

•

Cell Area

•  Layout Layer   •  Critical Area   •  Type (S2S, C2C)   •  Layout Layer   •  Critical Area   •  Via Macro Name

## Dealing with diagnosis ambiguity 

Diagnosis results have ambiguity (noise)

One or more locations, one or more properties (root cause)

Challenging to use raw diagnosis results to produce an accurate defect  distribution or select best die for FA

![suspect   score fail_match pass_mismatch type   value pin_pathname cell_name net_pathname layout_status  100   9   OPEN/DOM   both   ./n_6950  #potential_open_segments=1, #total_segments=1,   #potential_bridge_aggressors=3, #total_neighbors=22  suspect   score fail_match pass_mismatch type   value   location layout_layer critical_area  工-1   100   DOM   aggr   .../n_4643   Metal3   4.85E+06  2  1-2   96   OPEN   both   B1   Metal1   4.82E+04  vial   5.79E+04  Metal2   2.56E+05  via2   9.87E+04  Metal3   4.44E+05  100   OPEN/DOM   both   ./p0207A67923/YMXI2X1  #potential_open_segments=1, #total_segments=1,   #potential _bridge_aggressors=0, #total_neighbors=15  suspect   score faii_match pass_mismatch type   value   location layout_layer critical_area  2-1   100   CELL   both   :. : /p0207A67923  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e0966dc6-fd8c-4fc1-991d-4006b89cf6ef/e0966dc6-fd8c-4fc1-991d-4006b89cf6ef.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=de3a02674d9076cdd735b31b78fa5f53d620eed7)
## Defect pareto and yield analysis 

Yield analysis tries to find the physical properties that are likely  to fail

Comprises the creation of defect paretos

Defect paretos are trended over time

Multiple data sources are used during the process of creating  defect paretos

Data source is dependent on data access

Foundry – access to in depth process information

Fabless – access to design information and little manufacturing data

## Diagnosis-driven yield analysis 

Using diagnosis reports for yield analysis requires some    disambiguation     Statistically analyze all the raw diagnosis reports to determine    the most likely defect type and defect location   Employ machine learning to remove unlikely suspects     Requires “volume” diagnosis   Collecting test data on all failing parts   Running diagnosis on all failed parts

## Using scan diagnosis as a data source 

Statistical analysis of the raw diagnosis data amplifies ambiguity  in the diagnosis report

![450  Injected defects  400   Count of die (diagnosis)  350  300  250  200  150  100  50  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2dec62a5-f9cf-44a9-9d6d-9cd830d783cb/2dec62a5-f9cf-44a9-9d6d-9cd830d783cb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=5c41ca85243b89e7463ba5e6c2508786ae836cb9)
## Machine learning on diagnosis data 

Statistical analysis including ML of diagnosis data  that  combines design information with diagnosis behavior  can  be used to eliminate ambiguity

![450  Injected defects  4100  ■ Count of die (diagnosis)  350   HRCD  300  250  200  150  100  SO  CritArea SHORT   CritArea OPEN   CritArea OPEN   Count ViaMacroCount ViaMacrovia  CritAreaOPEN   Area CELL   CountViaMacro   CritArea OPEN   CritArea SHORT  route_2   route_3   route_2   via2   route_1   via3   route_4   route_3  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d7886450-538c-457a-a550-cd0667de04b7/d7886450-538c-457a-a550-cd0667de04b7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=f035ca2d56a6f50899e09e236b84f78cca292c1e)
## Improved FA localization…. 

Statistical analysis can be useful to select die for FA   Improve resolution of diagnosis result

![RCD-SumofProbability   Total   CRF   Pareto  CritArea SHORT route_2   269.963   0.565  CritArea OPEN route_3   156.503   0.892  CritAreaOPENroute_2   51.534   1.000  DielD   CritAreaSHORTroute_2  1464   18   38   0.997  46   28   0.996  suspectscorefail_match pass_mismatch type   valuepin_pathname cell_name net_pathnarme layout_status  731   38  100   S0   BRIDGE_2WAY   /cpu_i/ix1226/Y buf02 /cpu_i/nx1227 L0CATION_IN_LAYOUT  1387   2   suspect  score fail_match pass_mismatch type   value pin_pathname cell_name net_pathname layout_layer critical_area  969   29   100  30   BRIDGE_2WAY   /cpu_i/ix1222/Y buf02 /cpu_i/nx1223  route_1   8.0L+01  route_2   3.34E+02  1.45E+00  1.12E+02  6.83E+00  XXX—XL1  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1e65eb17-530e-4a43-93d0-3776b70a4a46/1e65eb17-530e-4a43-93d0-3776b70a4a46.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=fcb0235035f0a36c184e85b911b0d154c2cb8195)
## Leveraging diagnosis for yield analysis 

Creating a defect pareto from diagnosis data can move  diagnosis resolution to the next level

![Logic diagnosis  Logic diagnosis  Layout-aware diagnosis  Layout-aware diagnosis  Statistical analysis/ML  Statistical analysis/ML ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/db28502c-f354-4b9a-ae09-99ff56da4829/db28502c-f354-4b9a-ae09-99ff56da4829.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=f8e83095d69a42ad9adbf822dee607fa0116a9f5)
## Defect localization goes further….  

Suspect net and defect bounding box on section of net

![Defect  symptom:1  suspect:1.1  layer:VIA5  category:M6_M5H  critical_area:0.00248  score:100  l：3322.4399  2299.1799  2：  3322.8000  2:2299.5400  Suspect OPEN  Suspect OPEN  segment  segment ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a3b97ed9-b752-45cb-9c7a-e4741ba6159b/a3b97ed9-b752-45cb-9c7a-e4741ba6159b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=fbd916651f5064c1dd954ac06dc7416a23a2a731)
## What does that mean for yield analysis? 

Another data source for correlation   Rich data source that is tied to design

## Volume diagnosis as a tool for analysis  

![Statistical analysis/ML Statistical analysis/ML   Location analysis Location analysis   Property analysis Property analysis  All root causes from diagnosis All root causes from diagnosis  Single Via5  Single Via5 Via Macro Name  Via Macro Name Removed  Removed (noise)  (noise)  RCD  RCD All failing die  All failing die Real  Real . Number of failing die  Number of failing die where defect includes  where defect includes  .    single Via5  single Via5 93  93 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c3daaa4c-db7a-45b0-b900-90d034373ba4/c3daaa4c-db7a-45b0-b900-90d034373ba4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=7ad3401442802fde86d5030ceb8ab2edcea8e3cf)
## Diagnosis suspect heatmap analysis 

Correlation with other data sources  could help distinguish process or  design issues

![Filter by  ayei  Failuretype  50  Total  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a70edfc1-918e-47c3-8338-aa79ef450554/a70edfc1-918e-47c3-8338-aa79ef450554.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=630c8570a751da44a8e8fff662c4cc26dce84cec)
Die level clusters corresponded to wafer  level clusters

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/38217b4b-8307-46b8-bb66-1494a302234b/38217b4b-8307-46b8-bb66-1494a302234b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215808%3B1743219408&q-key-time=1743215808%3B1743219408&q-header-list=host&q-url-param-list=&q-signature=8cc938bf54c190022a5be8d82e980955a1296a8b)
Lacking dummy fill caused  CMP-induced defects

In this section, we covered…   How volume diagnosis can be used to guide FA   How volume scan diagnosis data can be used for:   Yield analysis   Defect paretos from diagnosis can further inform FI/FA

## Conclusion 

Structured DFT techniques like scan and ATPG are heavily used for  manufacturing test     Failing cycle information from the ATE contains a wealth of information     Scan diagnosis converts the failing cycle information into useful  information for FA and yield analysis

Thank you!

