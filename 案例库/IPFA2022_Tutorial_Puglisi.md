---
title: "IPFA2022_Tutorial_Puglisi.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_c394976927f5e0886a4b97ca1b4f0d477295230462135641
file_size: 7955022
---

## Defects in electronics: 

## from reliability physics to new applications 

Prof. Francesco Maria Puglisi University of Modena and Reggio Emilia

## Defects and Reliability 

Reliability: “The probability that an item will perform a required function under stated  conditions for a stated period of time”.

##   No reliability  $=$   No business 

Wide range of reliability issues in electron devices

Mechanical stress     Elevated temperature and/or electrical stress     Radiation exposure

Significant impact on both FEOL and MOL/BEOL   Reliability of interconnects   Leakage currents in dielectrics  eventually leading to  dielectric breakdown   Electrical features  of the device (e.g.,  $\mathsf{V}_{\top}$   shift, SS increase,   $\mathsf{I}_{\mathsf{o f f}}$   increase,   $\mathsf{I}_{\mathsf{o n}}$   reduction, …)   Major role  in the working principles of some  emerging devices  (e.g., resistive memories)

## Defects in Electronics 

Caused by defects in the atomic structure of the device, that can  capture/emit charge and lead to device performance degradation.

Four main device performance degradation mechanisms:    Bias temperature instability (BTI)

Occurs when bias is applied at the gate of a device   Causes defects located within the oxide to capture  charge either from the channel or the gate   Trapped charges change the threshold voltage and  possibly impact on the mobility in the channel   Accelerated by both gate bias and temperature and  is at least partially recoverable

![T=150°℃  -2.0V  40  1.4nmPNO   -1.8V  -1.6V  -1.4V  -1.2V  -1.0V  30  -0.8V  u]   -0.6V  20  10  10   10-2   10-1   10C   10-   10   10   102   10  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/024053ec-6343-4102-9229-254c85458afc/024053ec-6343-4102-9229-254c85458afc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=0921a668657ed6a35886a5beb62d29228a208040)
T. Grasser et al., IEEE T-ED, vol. 58, no. 11, 2011

## Defects in Electronics 

##   Hot Carrier (HC) degradation 

At high V  , channel carriers are accelerated towards the drain DS     Carriers with high kinetic energy, hot carriers, can cause damage close  to the interface     They can either get trapped or break Si-H bonds and create interface  states (dangling bonds)     Interface states can then charge and thus affect the channel similar to

border (i.e., bulk) defects

![(100) Si  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1f5b0eae-3e90-4548-aaae-40d3df142cec/1f5b0eae-3e90-4548-aaae-40d3df142cec.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=b35fed8a4e55042c1da68bd43f24663d2d354ee1)
## Defects in Electronics 

##   Random telegraph noise (RTN) 

Caused by defects randomly capturing and  emitting charge     Results in step-like noise in the channel and/or  gate current. Many defects together give  “flicker” 1/f noise     Causes various issues in integrated circuits,  e.g. failure in SRAM and jitter in ring oscillators     The effect increases with device scaling     Its randomness can be actually a resource in  some applications (e.g., TRNG, cryptography)

![Two-levelRTN  2  Time(ms)   X10  1025  L2→L1  Transition   Double   2  Gaussian  O15   Fitting  UL=-0.0024  L1-→12   U=31.9886  OTOS  Transition  15  sample#n（a.u)   Current(a:u)  Multi-levelRTN  28  1000   2000   3000   4000   5000   6000   7000   8000   9000   10000  Time（ms）  Quadruple Gaussian Fitting  H0.0432  9.8840  30.1977  80.06  39.9720  OO   2  102  20   30   0  sample#n(A)   Current (a.u.)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3ee362e2-0c5b-404c-9d3f-11b5a5ae2927/3ee362e2-0c5b-404c-9d3f-11b5a5ae2927.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=0d75fb98847ab917233201d7e51ec7fc78d24049)
F. M. Puglisi et al., IEEE IPFA, 2017

## Defects in Electronics 

Stress Induced Leakage Current (SILC) and Time-Dependent Dielectric Breakdown (TDDB)

Caused by pre-existing and stress-generated  defects that can aid tunneling of charge across the  dielectric     Increased leakage w.r.t. pure direct/FN tunneling  and higher power consumption     Electrical stress may create new defects, worsening  the scenario (SILC)     Eventually can cause the soft (SBD) and then hard  (HBD) failure of the dielectric (TDDB)     Fundamentals of Charge Trapping Physics   Non-radiative Multi-Phonon Trap-Assisted Tunneling   Multi-state defects (metastable states and multiple charge states)     Connection with Reliability Phenomena     Random Telegraph Noise   Complexity and Electrostatic Interactions   Defects Motion (and further complexity)     Defects Generation   Thermochemical model   Other TDDB models   Precursors and multi-scale simulations     Applications   Defects and True Random Number Generation     Common Misconceptions

![1SILC   2SBD  3HBD  hard  breakdown  wear-out   soft  (SILC)   breakdown  initiall  Stress Time  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a8808229-4bf4-462f-b82d-b51097ef887f/a8808229-4bf4-462f-b82d-b51097ef887f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=bd94a0018f1976473609c1c4984d04cbf2ca08ed)
## Non-radiative Multi-Phonon TAT 

capture

(a)initial

Trap Assisted Tunneling ina   P →t expon.distribution  𝑒𝑥𝑝𝑜𝑛. 𝑑𝑖𝑠𝑡𝑟𝑖𝑏𝑢𝑡𝑖𝑜𝑛   Coupling of charge  carriers to dielectric   𝐸 Eph = hwo  𝑝ℎ  = ℏ𝜔 0 phonons (assumed of a  of a   𝜏 𝑐 −1   =  (𝜏 't c.nm  𝑐,𝑚 ) −1 single frequency   $\omega_{0}$  )  𝑚   Sum up contributions for  all possible number of  is for  OF   𝜏 𝑒 −1   =  (𝜏 (Ten)-1  𝑒,𝑛 ) −1  (c)final   emission  nhoo  phonons involved  m ,  n  𝑛

mhoo

Involves tunneling  probability  probability  L

Capture probability

peaks at

Rhys factor)

![ (WKB) and   and   𝜏 Tc,.m  𝑐,𝑚 −1  = 𝑁𝐸 = N(Em)·f(Em)·Ca(m)·Pt  𝑚  ∙𝑓𝐸 𝑚  ∙𝐶𝑎(𝑚) ∙𝑃 𝑡  (a)initial   (b)defect  on   Te, =N(En)·(1-f(En))·Em(n)· Pt  𝜏 −1  = 𝑁𝐸  ∙(1 −𝑓𝐸  ) ∙𝐸𝑚(𝑛) ∙𝑃 𝑒,𝑛  𝑛  𝑛  𝑡 capture  （c）final  note that Em (Er,V,m)  𝑛𝑜𝑡𝑒𝑡ℎ𝑎𝑡 Eact(capt)  EREL=ShOO   (Huang- ang-V is the local potential at  V is the local potential at  mhoo   Temissiont   act(em)  the defect site the defect site   nhoof  7=O  Dq-1  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/00fd9f6a-4604-4d00-8348-ce9cadb88731/00fd9f6a-4604-4d00-8348-ce9cadb88731.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=8cb943838547987369dc3a13d507471fbf9d70a0)
Emission peaks at

## Non-radiative Multi-Phonon TAT 

##   Trap Assisted Tunneling 

Fermi’s golden rule:   Transition probability L between    two charge states the sum of the    transition probabilities between    different resonant   vibrational eigenfunctions,    proportional to their overlap     Coupling of charge  carriers to dielectric    $\begin{array}{c}{E_{p h}=\hslash\omega_{0}}\\ {\tau_{c}^{-1}=\displaystyle\sum_{m}(\tau_{c,m})^{-1}}\\ {\tau_{e}^{-1}=\displaystyle\sum_{n}(\tau_{e,n})^{-1}}\end{array}$    phonons (assumed of a    single frequency   $\omega_{0}$  )     Sum up contributions for    all possible number of    phonons involved  m ,  n     Involves tunneling  probability   $P_{t}$   (WKB) and   𝜏 𝑐,𝑚 −1  = 𝑁𝐸 𝑚  ∙𝑓𝐸 𝑚  ∙𝐶𝑎(𝑚) ∙𝑃 𝑡   multiphonon transition   𝜏 𝑒,𝑛 −1  = 𝑁𝐸 𝑛  ∙(1 −𝑓𝐸 𝑛  ) ∙𝐸𝑚(𝑛) ∙𝑃   probability  L  𝑛𝑜𝑡𝑒𝑡ℎ𝑎𝑡  $E_{m}\left(E_{T},V,m\right)$      Capture probability    peaks at   $m=\mathsf{S}$   (Huang  Rhys factor)  𝐶𝑎𝑚= 𝑐 0 (𝜎) ∙𝐿(𝑚, 𝜔 0 , 𝑇, 𝑆)     Emission peaks at   $\eta=0 $  𝐸𝑚𝑛= 𝑐 0 (𝜎) ∙𝐿(𝑛, 𝜔 0 , 𝑇, 𝑆) ∙𝑒

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/accc14c0-322c-459a-b4e1-81dec8d6552b/accc14c0-322c-459a-b4e1-81dec8d6552b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=93f42e8893bbf306b72b7246ce82deb67ee6e85f)
𝑡

![(a)initial  (b)defect  capture  （c）final  Eact（capt-.  EREL=ShOO  mhoo   temissiont   act(em)  nhoot  Bq-1  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/08882c8f-7b2a-4f81-b08d-5d5cfd55723f/08882c8f-7b2a-4f81-b08d-5d5cfd55723f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=addc510ecbebd9cd4158c90108b4dfd60efa19f5)
𝑝ℎ 𝑘𝑇

## Non-radiative Multi-Phonon TAT 

## Key defect properties 

Relaxation energy (sets the T dependence of TAT)     Thermal ionization energy  $ E_{R E L}=S\hbar\omega_{0}$      Capture cross-section     Depend on specific charge transition

![10-  T=6.2K  10-2   T=50K  T=200K  10  T=300K  10   T=400K  10-5  10-6  10   SiOxIL/5nm HfO2  SiO x  IL/5nm HfO 2 10  solid:wHKtraps  10  dashed:w/oHKtraps  10  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d9ea6630-197e-4994-8680-ee3747b2595b/d9ea6630-197e-4994-8680-ee3747b2595b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=7c7f971216fb2c0d55b2ed5f36e9a53090177033)
## Key material properties 

||HfO2|
|---|---|
|Electron affinity|2.4eV|
|Bandgap|5.8eV|
|Relative permittivity|21|
|Electroneffectivemass|0.18m0|
|Hole effective mass|0.2m0|
|Phonon effective energy (hwo)|0.07eV|


|Material|oz[cm²]|Erlev]|EREL[eV]|
|---|---|---|---|
|HfO2|1-1 0-14|1.4-2.4|1.19|


|||Ab-initio calculations (from the literature)|||||
|---|---|---|---|---|---|---|
|||||||2+|
|HfO2|ErIev|0.56[39]|0.76[39]|2.33[39]|2.32[39]||
|HfO2|EREL[eV]|0.43[39]|0.48[39]|0.80[39]|1.0139]||


## Simplified TAT Formalism 

##   Simplified TAT approach 

Tunneling and multiphonon transition probabilities can   𝜏 𝑐 −1   = 𝑁∙𝑓∙𝑐 0  ∙𝑒 − 𝜆 𝑑 𝑐  ∙𝑒 − 𝑘𝑇 𝐸 𝑐   be replaced by two  𝜏 −1   = 𝑁∙(1 −𝑓) ∙𝑐   ∙𝑒 − 𝜆 𝑑 𝑒  ∙𝑒 −𝐸   exponentials  𝑒  0     Characteristic tunneling   length calculated via WKB    $\begin{array}{r}{\lambda_{c}=(2\sqrt{\phi_{b}2m^{*}q/\hbar^{2}})^{-1}}\\ {\lambda_{e}=(2\sqrt{E_{T}2m^{*}q/\hbar^{2}})^{-1}}\end{array}$    neglecting the effect of the    field on the barrier     Thermal barriers calculated   considering that emission    (𝐸 𝑅𝐸𝐿  −Δ𝐸) 2  =  𝐸 𝑅𝐸𝐿   occurs from trap ground  𝐸 𝑐  =  𝐸 𝑒  4𝐸 𝑅𝐸𝐿  4   state     ΔE is the difference  𝑥 𝑡   between the charge carrier  Δ𝐸= 𝐸 𝑇  + 𝑞𝑉 𝐺  −𝜙 𝑏  𝑡   energy and the ground state   𝑜𝑥   of the trap

L. Larcher et al., Nanotechnology 2012 (vol. 2)

![𝑒 𝑘𝑇  𝒙 𝒕 qVG  𝒒𝑽 𝑮 𝒕 LoX  𝒐𝒙  𝝓 𝒃 capture  emission   𝒙 𝒕 𝒕 tox  𝒐𝒙 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5e2e41d9-7197-4ff0-acae-8832fe9167ca/5e2e41d9-7197-4ff0-acae-8832fe9167ca.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=109e2cc720fa1302720c423691c3b9875f552846)
## Multiple Sources and Destinations 

##   Multiple sources / destinations 

All processes are possible  in all conditions     Many possible capture / emission processes and related capture / emission times     Most likely process depends on applied conditions     Mathiessen rule applies

$$\begin{array}{r}{\tau_{c}^{-1}=\left(\tau_{c,T E}^{-1}+\tau_{c,B E}^{-1}+\tau_{c,C B}^{-1}+\tau_{c,V B}^{-1}+\tau_{c,D}^{-1}\right)^{-1}}\\ {\tau_{e}^{-1}=\left(\tau_{e,T E}^{-1}+\tau_{e,B E}^{-1}+\tau_{e,C B}^{-1}+\tau_{e,V B}^{-1}+\tau_{e,D}^{-1}\right)^{-1}}\end{array}$$
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1a50e19b-dd6d-47ca-93a7-f3a72c68a9a0/1a50e19b-dd6d-47ca-93a7-f3a72c68a9a0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=5b682a7bc919f9a8f60711cb1ef07f9fbd979caa)
## Metastable States 

##   Possible metastable states  

Changes in configuration without charge transition, regulated by a purely thermal barrier   Identified in   ${\mathsf{S i O}}_{2}$   by ab-initio DFT calculations for  oxygen vacancies, hydrogen bridge and hydroxyl E’ center   Important to describe long-term BTI   Also a possible responsible for RTN

![k12\*   522  62:1   meutral   charged  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f9a053e8-83e1-42ab-aee0-0f7aceb05c57/f9a053e8-83e1-42ab-aee0-0f7aceb05c57.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=9f87cf57a415546d6f5567b5cf15bee254d8ada0)
![(a) Hydrogen bridge   : (b) Hydroxyl E'  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c6108961-4626-4df0-8bec-f97209d4054c/c6108961-4626-4df0-8bec-f97209d4054c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=840cbb358ce41e99816cb4341c54add15f3eb53a)
Adapted from W. Yannick et al., Proc. R. Soc. A., 2016

![Configuration coordinate  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/da01cbd6-2afc-4a49-8e13-d38328cc47fb/da01cbd6-2afc-4a49-8e13-d38328cc47fb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=ec252975341ef7d482cd40cb634cd1f87534e82e)
Adapted from B. Stampfer, (2020) [Dissertation, T. U. Wien]

## Connection with Reliability Phenomena 

One defect kind / many reliability phenomena   BTI (unbalanced transition rates)   Different conditions during stress and relaxation   Different processes favored in different conditions   Source and destination are  not  of special concern

![T>0  Gate   Oxide   Channel  Vb>0  Em  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/062e8803-bfbe-43ea-b599-4e44661f1255/062e8803-bfbe-43ea-b599-4e44661f1255.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=cf8375ec86004df28a5e9214bd40f730f8e52f91)
![T=150°C  -2.0V  40  1.4nmPNO   -1.8V  -1.6V  1.4V  30   1.0V  -0.8V  u   -0.6V  20  10-5   10   10-1   10   1.0-3   10-2  10-1   100   101   102   10  StressTime[s]   RelaxationTime[s]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0341eba1-f72c-4088-adb2-83998238628b/0341eba1-f72c-4088-adb2-83998238628b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=f6475979fdcd78c197911306a96807becca25f1c)
T. Grasser et al., IEEE T-ED, vol. 58, no. 11, 2011

## Connection with Reliability Phenomena 

##   One defect kind / many reliability phenomena 

Leakage (balanced  fast  transition rates)

The source and destination are important     Capture and emission sequence of events must lead to charge transfer from one  electrode to the other     Many mechanisms – some of which involving defects

$$I=\frac{q}{\tau_{c}+\tau_{e}}$$Tc + Te
![  1. Drift/diffusion  1. Drift/diffusion  (2)  （1）     2. Thermionic emission  2. Thermionic emission  S  （11)     3. Direct Tunneling (or Fowler-Nordheim)  3. Direct Tunneling (or Fowler-Nordheim) 8）     4. Electrode-to-band tunneling  4. Electrode-to-band tunneling  【3）  9)     5. Intra-band tunneling  5. Intra-band tunneling  (10)-     6. Band-to-band tunneling  6. Band-to-band tunneling  6)     7. Generation/recombination  7. Generation/recombination    8. Electrode-to-trap capture  8. Electrode-to-trap capture    9. Trap-to-electrode emission  9. Trap-to-electrode emission  a    10. Trap-to-trap tunneling  10. Trap-to-trap tunneling  e.g.,I = 1pA means  𝑒. 𝑔. , 𝐼= 1𝑝𝐴𝑚𝑒𝑎𝑛𝑠   11. Trap-to-band tunneling  11. Trap-to-band tunneling  πc+t。≈ 100ns  𝜏  + 𝜏  ≈100𝑛𝑠 𝑐  𝑒 15  15  Courtesy of Applied Materials  Courtesy of Applied Materials ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4fd5829e-2a0e-4ab1-918d-f42bfa1141e3/4fd5829e-2a0e-4ab1-918d-f42bfa1141e3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=90a58460613e737d480b63779143e1b5713a6c78)
## Connection with Reliability Phenomena 

One defect kind / many reliability phenomena   RTN (balanced slow transition rates)   Metastable states can be involved   Electrostatic interactions between defects involved   Source and destination are  not  of special concern  but…

![TEOVAPP  001  00#2  BE  00#3  00#4  TN  HO  BE  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3878d0af-6488-4cbb-86f2-dd517f44d93d/3878d0af-6488-4cbb-86f2-dd517f44d93d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=9ad279becda9987ee514b70bdb38dd58267ff6dc)
![Distance=0.7nm-RTN  Empty SlowDefect   Filled Slow DefectOxygenVacancy  0.25   0.5   0.75  Time [s]   X10  bairrier   Distance=1.1nm-No RTN  barrer  u  No Coulomb Interaction   Coulomb Interaction  0.25   0.5   0.75  Un-altered TAT @ Vo defectAltered TAT @ Vo defect  Time [s]   X10  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1e541b34-1d95-4f74-805b-5a4d975d3a25/1e541b34-1d95-4f74-805b-5a4d975d3a25.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=0c1cd545cfc22a3b6706b80dba37b64b45258d0f)
![-10   APP=0.5V  X10  1.85  1.8  0.02   0.03   0.04   0.05  Time(s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/868ed40e-a897-43f3-bdf3-969dc6e31bd5/868ed40e-a897-43f3-bdf3-969dc6e31bd5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=4e90e4d062a6a8db20ca828ac14116710fb1e74c)
S. Vecchi et al., IEEE IRPS, 2022

16

## Random Telegraph Noise 

![MIM Stacks  MIM Stacks  TE OVAPP  TiN/(2nm)HfO,/TiN  TiN/(2nm)HfO 2 /TiN  HfO2  ITiN   ×10-11   VAPP = 0.3 V  10.2   5 Oxygen Vacancies (V+)  5 Oxygen Vacancies (V + ) "fast" traps  “fast” traps  TAT Leakage Current  TAT Leakage Current   →White Noise  White Noise BE-Level2  00°#1   4 Oxygen lons (0%)  4  Oxygen Ions (O 0 )      9.8   Leyel   Level4.  10°#2   "slow" traps  “slow” traps   24 = 16 Possible Configurations  2 4 = 16 Possible Configurations  B  √0°#3   TAT and DT Current  TAT and DT Current   0.076   0.077   0.078   0.079   0.08  M☆0°#4   Modulation  Modulation  RANDOM TELEGRAPH NOISE  RANDOM TELEGRAPH NOISE  Time (s)  Only 4 Configurations can be detected directly from the simulator:  Only 4 Configurations can be detected directly from the simulator: Coo   100  00#1   A-O   B011   C0011   Ｄ０００１   万0   O #2 and 0° #3  O 0   #2  and  O 0   #3 0°#2   NS   predominantly change their  predominantly change their  0：#3   occupancy over Time  occupancy  over  Time  00#4   1   0.10.2 0.3 0.4 0.5   promoting RTN  promoting  RTN  Applied Voltage (V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6d7b5ed1-1b78-4e4c-addc-eb6b80d6b1a5/6d7b5ed1-1b78-4e4c-addc-eb6b80d6b1a5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=7d1c059f2a4302c16f29debab20beb7e3445d4a7)
## Random Telegraph Noise 

•  O 0   #2  and   $_{0^{0}}$    #3  belong to the (yellow) region that is typically accessible by experiments   •  Both  monotonic  (  $\mathbb{O}^{0}$    #3 ) and  non-monotonic  (  $\bullet\circ$    #2 ,  #1 ,  #4 )   $\pmb{\tau_{c}/\pmb{\tau_{e}}}$   trends  are appreciable

$\pmb{\tau_{c}}/\pmb{\tau_{e}}$   slopes  commonly used to:

![Estimate vertical position of defects Estimate vertical position of defects   Classify defects  Classify defects  100   100  𝜕ln  τ 𝑐  re  Slope > 0  Slope > 0   𝑋 XTX  ∝  𝑘𝑇  τ 𝑒  type-l   type-ll  𝑇  𝑞  𝜕𝑉 𝑔   τ 𝑐 𝜕ln 𝑘𝑇  τ  slope  Slope < 0  Slope < 0   X  𝑋  ∝1 −  𝑒 𝑇  𝑞  𝜕𝑉  .1  𝑔  0.7 0.8 0.9 1.01.11.2   0.3 0.4 0.5 0.6 0.7 0.8  [1] C. Chen et al., IEEE EDL, 2016.  [1] C. Chen et al., IEEE EDL, 2016.   [2] T. Nagumo et al., IEEE IEDM, 2010.  [2] T. Nagumo et al., IEEE IEDM, 2010.  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7d6f48d8-d2d3-4b8b-8abf-cb032c7a6125/7d6f48d8-d2d3-4b8b-8abf-cb032c7a6125.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=f5a9869f8868675cb744eb54c8297ae962c3ccba)
![10-5  0.1 0.2 0.3 0.4 0.5  Applied Voltage (V)  -0°#1→10°#3  ■+0°#2-→10°#4  Obs.Zone  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/28102854-287a-4fdf-a63a-e8d09ad718ed/28102854-287a-4fdf-a63a-e8d09ad718ed.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=f1257f67e2d194c20b569e2370d2db8a22f9b897)
## What about Non-Monotonic trends? 

S. Vecchi et al., IEEE IRPS, 2022

## Random Telegraph Noise 

![ZT,REAL   ZT,ESTIMATED   Error  Monotonic trend  (slope < 0)   0.72nm   0.54nm   -25%  Non-Monotonic  slope >0   1.37nm   1.46nm   +6.6 %  trend   slope<0   1.37nm   0.49nm   64%  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/aa72dd4e-f406-4993-b3c7-5eaf01360210/aa72dd4e-f406-4993-b3c7-5eaf01360210.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=92e3864f121ebb50264dc5617dd1966a5c641e9a)
![TE  BB  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2d4f6d68-793a-4163-b2c7-c0ac3e937d36/2d4f6d68-793a-4163-b2c7-c0ac3e937d36.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=437003c3c4d631bda7da14a1bea9c8873ffd0849)
$\pmb{\tau_{c}}/\pmb{\tau_{e}}$   slopes  commonly used to:

Estimate vertical position of defects

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6adbadc5-5e37-43a5-bd34-92f2034fc3cb/6adbadc5-5e37-43a5-bd34-92f2034fc3cb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=0f259f11394aa90149954959ffeff20dd6f63526)
𝜕ln  τ 𝑐 Slope > 0   𝑋  ∝  𝑘𝑇  τ 𝑒 𝑇  𝑞  𝜕𝑉 𝑔

Slope < 0

𝜕ln 𝑘𝑇

𝑐

𝑋

τ

∝1 −

𝑇

τ

𝑒 𝑞

𝜕𝑉

𝑔

![Classify defects  Classify defects  10   O° #2 Capture  ISource Changing  Not a  100   type-l  trap!  1  10  0.1   0.2   0.3   0.4   0.5  AppliedVoltage(V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b7bac66d-b916-47a1-a2b7-280bdd134232/b7bac66d-b916-47a1-a2b7-280bdd134232.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=d755194792cdd0d08c777aea6892228705cf32c6)
[1] C. Chen et al., IEEE EDL, 2016.

S. Vecchi et al., IEEE IRPS, 2022

## RTN and Electrostatic Interactions 

![Potential profile at O° #2   Potential profile at  O 0   #2  Potential profile at O° #3  Potential profile at  O 0   #3 Vapp = 0.3 V  V APP  = 0.3 V  d(#3,#4) = 1.75 nm   Vapp = 0.3 V  V APP  = 0.3 V 0.3   Z coord  Z coord   0.3  of#2  of  #2  Z coord  Z coord  Slight   z  of#3  of  #3 0.2   Interaction   0.2  with  0.1   00.#3.   Neutral (0e)  Neutral (0 e - )  0.1  Slight  Interaction  Charged (1e)  Charged (1 e - ) with O° #2  0.511.5   d(#2,#3) = 1.46 nm   0.5  1  1.5  Z (nm)   Z (nm)  Local Potential at O Local Potential at Oo #2  0   #2  d(#2,#4) = 0.47 nm   Local Potential at O Local Potential at Oo #3  0   #3 0.2  03   Rigid Shift  induced by  0.2   00#1   0   -0111   -0011   -0001   O.1  O.1   0#2   10  00#3  00#4  -0.1   -0.1  0.10.20.30.40.5  0.10.20.30.40.5  Applied Voltage (V)  Applied Voltage (V)  S. Vecchi et al., IEEE IRPS, 2022 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4274d58c-eca2-4fab-b4eb-ab9b68047576/4274d58c-eca2-4fab-b4eb-ab9b68047576.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=c6f111b9bffa1f151f9212a096efb8c6c10236cd)
## RTN and Electrostatic Interactions 

![Potential profile at O #2  Potential profile at O 0   #2  Potential profile at O° #3  Potential profile at O 0   #3 Vapp = 0.3 V  V APP  = 0.3 V  d(#3,#4) = 1.75 nm   Vapp = 0.3 V  V APP  = 0.3 V 0.3   Z coord  Z coord   0.3  Z coord  Z coord  of#2  of  #2 Slight   of#3  of  #3 0.2   Interaction   0.2  With  0.1   0.1  Slight  Interaction.  with O #2  0.5   d(#2,#3) = 1.46 nm   0.5   1Ｓ  Z （nm  Local Potential at  Local Potential at O #2 vs VAPp  O 0   #2  vs  V APP  d(#2,#4) = 0.47 nm   Local Potential at O0 #3 vs VAPp  Local Potential at  O 0   #3  vs V APP 0.2  0.3   Rigid Shift      induced by  0.2   00#1   0111   0   0001   O.1  00#4  0°#2   0  0.1  0：#3   1  00#4  -0.1   -O.1  0.10.2 0.3 0.4 0.5  0.10.20.30.40.5  Applied Voltage (V)  Applied Voltage (V)  S. Vecchi et al., IEEE IRPS, 2022 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f0dde8af-f422-482d-ba13-8ae1ee706dfd/f0dde8af-f422-482d-ba13-8ae1ee706dfd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=88fe85ad517981e4cbb0c186b0cdaa795de11b8a)
## RTN and Electrostatic Interactions 

![YZ Plane @ X(O' #2)   YZ E-field Map: Conf. A   YZ Plane @ X(O #3)   YZ E-field Map: Conf. A   MMW  cmm  (wu) z   uuu   E-field at   100#2  isfilled   4.0  0#3is  sightly  W   MW   perturbed  byO#2  3.0  APP  =0.3V   Y (nm)   VAPP  =0.3V   Y (nm)  YZ Plane @ X(O° #2)   YZ E-field Map: Conf. D   2.0  YZPlane @X(O° #3)   YZ E-field Map: Conf. D  (u）z   E-fieldat  uuu   O#3 is not  1.0  perturbed  byO0#2  (#2 is empty)  YAPp=0.3V   Y (nm)   VAPP = 0.3 V   Y (nm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f67e6e42-9ab8-4d19-ab3c-191e0589966c/f67e6e42-9ab8-4d19-ab3c-191e0589966c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=66c25e106a8b602ea0557526e776daef2ae1c50b)
## RTN and Electrostatic Interactions 

![t,of O° #3 changes with the occupancy of O0 #2  τ c  of  O 0   #3  changes with the occupancy of  O 0   #2 YZ Plane @ X(O #3)   YZ E-field Map: Conf. A      cm  100#2  ○° #2 Full   E-field at   4.0  isfilled  0#3is  slightly  perturbed  by0#2  3.0  0°#2 Empty   Vapp = 0.3 V   Y (nm)  0.076   0.078   0.08   0.082   0.084  ×10\~   Time (s)   2.0  YZ Plane @ X(O° #3)   YZ E-field Map: Conf. D  Capture from Bottom of O'  E-field at  uuu   0°#3 isnot  C   1.0  perturbed  byO0#2  40%Difference   (#2 is empty)  0.076   0.078   0.08   0.082   0.084   VAPP = 0.3 V   Y (nm)  Time (s)  Of course also the occupancy of     #3  impacts on   00#2    #2 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3a260aca-eed1-4c32-a7f8-cf7bbec12f3e/3a260aca-eed1-4c32-a7f8-cf7bbec12f3e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=5d3af18407aa8a8e24664a6934fb43f97450a61a)
…

## RTN and Electrostatic Interactions 

![-11  ×101   =0.3V  APP   a   10   VAPP=0.3V   emptyfull  · Detailed analysis    Detailed analysis  10.2   10.2  10   evel2   Level1口  · RTN decomposition    RTN decomposition  9.8   98   Level3  9.6   Level4  9.2   9.3   9.4   9.5   9.6  MarkovChainofO#2and#3  ×10-11  10.2  Level2  9.8   Level4  Level  AL   CL   9.2   9.③   94   9.5   9_6  9.6   O° #2 T. analysis   Time (s)  ImpactofO°#3on#2  2.5   W   3.5  Proposed method:  40  Neutral O°(0e-)Charged O°(1e-)   Time (s)   8c.1  ventionalmethod:  20  Upto33%modulationof  · No significant complexity at eye inspection  No significant complexity at eye inspection  T.of #2due to#3   Looks like standard multi-level RTN  Looks like standard multi-level RTN -20   -20  · Complexity is hidden    Complexity is hidden  0.2   0.250.30.350.4   0.2 0.25 0.3 0.35 0.4  VAPP(V)   VAPP(V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d85545a8-9404-466f-ac30-b42bef6da4cf/d85545a8-9404-466f-ac30-b42bef6da4cf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=0885c3b28483651889026d4d9766254c678333f5)
## Leakage and Electrostatic Interactions 

Contribution of trapped charge to the  electric field

Can be quite significant    Heavier computation workload

∆𝑰% =

𝑰

𝒘

MIS Stacks Analysis Si/(1nm)SiOx/(2nm)HfO2/TiN

−𝑰

𝒘𝒐

∙𝟏𝟎𝟎

𝑰 𝒘𝒐

![si  Isiox  HfO2  TN  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0fa6658c-8efb-48ce-bb41-89d7dfe5e7ff/0fa6658c-8efb-48ce-bb41-89d7dfe5e7ff.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=539e2b7149a12d5c0ff359bd1da31cc0386f0651)
Statistics: 30 devices

$I=$  Leakage Current  considering ( w ) and  without considering ( w/o ) trapped charge  term

![Low Doping   p-type   High Doping  300  200  (%) IV   100   -SO  -100   -100  n-type  Low Doping   High Doping  400   100  300  200   SO  Z100  IN  Electric Field (MV/cm)   Electric Field (MV/cm)  -Device   Deyice   RefLine  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1741a8ba-a78d-45ff-935b-0c68a1c0cc3f/1741a8ba-a78d-45ff-935b-0c68a1c0cc3f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=0c32ce4fd68ceccff2fdd6a5ada3cc46af91e700)
## RTN and Defects Motion 

Advanced transient MC and kinetic MC 3D simulations combining:

![Stochastic charge trapping (NMP-TAT)  Stochastic charge trapping (NMP-TAT)  EA,D - kD · FEFF(x,y,Z)  RD(x,y,z) = Vo · exp  Defects electrostatic interactions  Defects electrostatic interactions  kB·T(x,y,z)  kMC  SIMULATION  START  Initial configuration    Defects stochastic field-assisted motion  Defects stochastic field-assisted motion Window0   Defects parameters setup   △to=t-to  Initial configuration of traps  CN  ASE  1stdiffusionevent  N/(4nm)HfO2/TiN   b) Band Diagram  EC   Window1  Vapp O   TAT   TRANSIENT SIMULATION  q中B：   FN   dominant   △t,=t2-t  EC   tm = simulation time  PT   1O-15   一O一TAT on  BE   00   --TAT off  Metal   TAT   Timing of n diffusion events  TE   Trap   Metal10-   (to, t1, , tr), and related  00#   88   0.45 0.55 0.65 0.75   defect configurations   nthdiffusionevent  00#2   (Co, ..., Cn)  Insulator   Applied Voltage (V)   Window1  00#3  00#4  TN    SE = Schottky/Thermionic Emission   White noise·   △tn = tm- tn  DT = Direct Tunneling  FN = Fowler-Nordheim Tunneling  TAT = Trap-Assisted Tunneling  Concatenat  CEND  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/01c882cf-9eb8-438a-b7d1-d474bf84cb37/01c882cf-9eb8-438a-b7d1-d474bf84cb37.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=eb54b758a929290ba474f97383f41ae654ce5585)
## RTN and Defects Motion 

“Static” (though complex) RTN w/o defect motion   “Dynamic” RTN with instabilities w/ defect motion

![00#2  10-13   Vapp = 0.6 V   00#1  4-Level RTN  100   200   300   400   500   600   700   800   900   1000  Window10   Window 27  2.56  20   ALO   80   100   120   140   160   180   200  Time (s)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ccf74c5d-a03a-4dfe-ae90-d4607abe4712/ccf74c5d-a03a-4dfe-ae90-d4607abe4712.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=42439617ea53f86fcda665b3864fe341f3dfca3d)
## RTN and Defects Motion 

E-field change with defect motion causes significant RTN instabilities J

![a  ×10-13Window10   ×10-13Window27   Window 10  A  2.6   2.6  △I/IMN = 1.0 %  2.58   △I/IMIN = 0.3 %  2.56   2.56  Mainly  involved  S0   60   186   190   194  V+inTAT  VLoc = 0.385 V  02   ○#2  00#1   00#1  50   60   186   190   194   Potential  Time (s)   Time (s)   Window 27   ?  Mainly   Mainly   0.457  involved   involved  V+inTAT   V+inTAT  0.40-  Mainly  (uuu)   involved  V+ in TAT  1.65nm   0.35  W   Vtoc = 0.420 v  2.65nm  0.30  0.25  Y (nm)   Y (nm)  ○V+○0°#10°#2√0°#3★0°#4  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f12687cf-cd54-426d-b870-b50086d02774/f12687cf-cd54-426d-b870-b50086d02774.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=62f1b2f5287d1407d0b4485bf862f9114e534961)
## RTN and Defects Motion 

This phenomenon has been previously reported in the literature but lacked a solid explanation although  interactions between defects has been suspected for a long time to be deeply involved in the mechanism   Observed in device-level as well as with in-situ C-AFM measurements

![(a)   VcAFM= 5.0V  n++Si   Siox   HfO2   AU  d  <o)   (c)  HfO2   S  SiOx  0.8  0.6  sio  n++si  10nm   5nm  Energy (keV)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8e058920-d452-4c68-9238-0c92536c0851/8e058920-d452-4c68-9238-0c92536c0851.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=63998453864c686f29d1ce3d1a4e0c5043e10a48)
## Not Only Charge Trapping 

##   Many concurrent mechanisms 

Charge trapping   Defects electrostatic interactions   Defects migration (drift and diffusion)   Defects generation / recombination   Interactions of all above mechanisms

All rates of above mechanisms strongly  depend on actual conditions   Complex framework   Need for detailed understanding of all mechanisms

![[wu] z   [wu] 2  T   STI  202  Y   .0  Diffusion  Diffusion  Vodefect   Ointerstitialdefect   OVacantinterstitialsite  YZPnnE@X（O#2)   YZE-field Map:  LA  z  VAPP=0.3V   Ynm)  YZPlune@X（O#2）   YZE-fieldMap:Conf.D  （uu）z  VAPP=0.3V  Y（nm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1b0edccd-1402-49ab-969a-a26d492c4f38/1b0edccd-1402-49ab-969a-a26d492c4f38.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=25019318f31f40f724b28874d1f7732add043589)
L. Vandelli et al, IEEE T-ED, vol. 60, no. 5, 2013. F. M. Puglisi et al., SSE, vol. 125, 2016. S. Vecchi et al., IEEE IRPS, 2022.

## Test vs. Operating Conditions 

In which conditions do we test for reliability?

RTN and Leakage typically in use conditions     BTI and TDDB typically in accelerated conditions   Different models give different predictions at op.  conditions

Are the mechanisms the same in test vs.  operating conditions?

Big open question in reliability community     Important to project reliability margins and targets   Expected  $\mathsf{V}_{\top}$   shift   $@\,85\ ^{\circ}\mathrm{C}$   in 10 yrs   Expected TDDB lifetime  $@$   rated T and  $\mathsf{V}_{\mathsf{D D}}$    Constant stress vs. pulsed stress (in-circuit realistic workload)

![1.0E+19  E-Model  1.0E+17  (E)izModel  1.0E+15  VNModel  1.0E+13  1/E-Model  1.0E+11  1.0E+09  1.0E+07  1.0E+05  1.0E+03  1.0E+01  1.0E-01  1L0   S  ElectricField:E(Mv/cm)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7ecf29d5-f451-4e35-afed-c4b3720f455b/7ecf29d5-f451-4e35-afed-c4b3720f455b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=1ad95b7c74efb286c48b4ad61e3839f2c403fa9c)
J. McPherson, Microelectronics Reliability, vol. 52, Issues 9–10, 2012.

![AVh DCstress(α=1) trendovertime(a<1) ACstress Stress  Recovery (ON)  （OFF) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2c86ad94-baea-43a7-a634-61804f95b319/2c86ad94-baea-43a7-a634-61804f95b319.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=187d7feda10aea67740d456d89544aa959dc3b72)
B. Halak, Microelectronics Reliability, vol. 67, 2016.

## Defects Generation 

Many models exist that attempt at describing the process of  defect generation within dielectrics

Of crucial importance to determine the device lifetime     Both physical and empirical models available     A complex matter that gave rise to decades-long disputes that are still  ongoing     Recent multiscale collaborative approaches bridging atomistic  calculations to comprehensive device physics simulations are shedding  new interesting light

## Thermochemical Model 

Describes the bond breakage rate for molecules that are  strained by the local electric field

$$G=G_{0}e x p\left(-\frac{\Delta H}{k_{B}T}\right)$$
$\mathsf{G}_{0}$   is the bond vibration frequency   $(\sim\!10^{14}\,{\sf H z})$  . It represents the number  of times per second that the strained molecule interacts with the  surrounding lattice

The exponential term represents the Boltzmann probability that, on a  given interaction with the lattice, the bond will receive enough energy to  break   J. McPherson, J Appl Phys 84, p. 1513, 1998

J. McPherson, J Appl Phys 88, p.5351, 2000   J. McPherson, IEEE Trans Elect Dev 50, p. 1771, 2003   McPherson J. J Appl Phys 95, p. 8101, 2004

## Thermochemical Model 

Δ𝐻  is the enthalpy of activation (or activation energy) and represents  the energy required to break the bond

$$G=G_{0}e x p\left(-\frac{E_{A}}{k_{B}T}\right)$$
$$E_{A}=E_{A0}-b E_{O X}$$
![519  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1bebbef6-8737-4ff1-b5a9-f6a2c2ecedc8/1bebbef6-8737-4ff1-b5a9-f6a2c2ecedc8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=c2343955d2e267ef71e812d5d5103182a57b6ac0)
$\textbf{\em E}_{A0} $  is the zero field activation energy  $\begin{array}{r}{b=p_{0}\left(\frac{2+k}{3}\right)}\end{array} $  is the bond polarization factor  $p_{0}$   is the molecular dipole moment   k is the relative dielectric constant

![SeverelyStretchedBond  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/177cf4b6-159b-40bc-a5e3-c14e1761ebec/177cf4b6-159b-40bc-a5e3-c14e1761ebec.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=ad131c0253a47f50e06219b92bcc275894eb9e2b)
## Thermochemical Model 

Time to breakdown is assumed to be inversely proportional to the bond  breakage-rate

$$t_{B D}\propto G^{-1}=G_{0}^{-1}e x p\left(\frac{E_{A}}{k_{B}T}\right)$$
$$t_{B D}=A_{0}e x p\left(\frac{E_{A0}}{k_{B}T}-\gamma E_{o x}\right)$$
$$\gamma=-\left[\frac{\partial\ln(t_{B D})}{\partial E_{o x}}\right]_{T}=\frac{b}{k_{B}T}$$
where γ is the field acceleration parameter

$\sf t_{b d}$   is actually the   $\mathsf{t}_{63\%}$   of a Weibull distribution

![r2  SeverelyStretched Bond  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/475207cb-b4df-4a1b-9e15-b7bc4f77e556/475207cb-b4df-4a1b-9e15-b7bc4f77e556.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=3f863366775b5e779e41f42ccc51614d245be9cc)
## Thermochemical Model 

𝐸

𝐴

𝑡

∝𝐺

−1

−1

𝐵𝐷

= 𝐺

𝑒𝑥𝑝

0

𝑘

𝑇

𝐵

𝐸

𝐴0

𝑡

= 𝐴

𝐵𝐷

𝑒𝑥𝑝

0

−𝛾𝐸

𝑜𝑥

𝑘

𝑇

𝐵

![   1.O  1.0  1000  1000 T = 25°C  T = 25°C  12A SiO,/25A HfSiON  12Å SiO x /25Å HfSiON 0.5  0.5  nMOSFET  nMOSFET TDDB (63%)  TDDB (63%) 0.0 0.0  ((-)u|-)u[  ln(-ln(1-F))  -0.5 -0.5    [s]  Y = 2.86 cm/MV  = 2.86 cm/MV 100  100 63 -1.0 -1.0   t -1.5  -1.5 >3.3V  3.3V -２.0  -2.0 3.4V  3.4V (aD  (a)  △3.5V  3.5V  (b)  (b) -2.5  -2.5  10 0.1  0.1  10  1000 1000   8  9  10 stress time [s]  stress time [s]  Electric Field [MV/cm] Electric Field [Mv/cm]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e0ca978b-d1cc-4bac-8e4c-e1393590ab7c/e0ca978b-d1cc-4bac-8e4c-e1393590ab7c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=1c703ed287b9e6b2be7de695ec0cd4758097fb89)
A. Padovani et al., IEEE EDL, vol. 34, no. 10, 2013.

𝜕ln 𝑡

𝐵𝐷

𝑏

𝛾= −

=

𝜕𝐸

𝑜𝑥

𝑘

𝑇

𝑇

𝐵

## Thermochemical Model 

Assuming   ${\sf t}_{\sf b d}={\sf G}^{\cdot1}$  , TDDB data  measured at different stress voltages  can be used to characterize the  defect generation process

F [eV]

$$t_{B D}\propto G^{-1}=G_{0}^{-1}e x p\left(\frac{E_{A}}{k_{B}T}\right)$$
![H.→  1.7 T = 25°C  T = 25°C E Ea,G = 2.4eV  A,G  = 2.4eV 1.5  1.5  b\~ 11eA  b  11eÅ  Ea = 2.65eV  E   = 2.65eV A b\~ 11eA  b  11eÅ 1.3  1.3 SiO/HfSiON  IL-HfO2 data siON  SiON 1-1  1.1 7  8  9  10  11  12  13  13  14 Electric Field [MV/cm] Electric Field [Mv/cm]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b8248fa7-02d9-4194-b0b7-4856e1e2ffe1/b8248fa7-02d9-4194-b0b7-4856e1e2ffe1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=d4bab79ecb2687425dc3d14d9b1a9a419510e870)
$$E_{A}=E_{A0}-b E_{o x}=k_{B}T l n(t_{B D}G_{0})$$
E

## Breakdown Models 

The thermochemical model is the  most conservative and perhaps the  most physically sound, but is it also  correct?

It’s critical to identify the actual  failure model to correctly project  lifetime and target  reliability/performance tradeoff     Very diverse trends found in the  literature…

![1.0E+19  E- Model  1.0E+17  (E}12 - Model  1.0E+15  VN - Model  1.0E+13  1/E-Model  1.0E+11  1.0E+09  1.0E+07  1.0E+05  1.0E+03  1.0E+01  1.0E-01  5   15  ElectricField:E(MV/cm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f880ff0d-b0e8-408b-a29b-af0ad8ba900c/f880ff0d-b0e8-408b-a29b-af0ad8ba900c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=77c995956d663f789d01f96c20f6a5c1cf996f7b)
## Breakdown Models 

Mainly, 4 models are under discussion

Thermochemical (E)   $\begin{array}{r l}&{T_{\mathrm{BD}}=T_{\mathrm{BD0}}\mathrm{exp}(-\gamma_{V}V)\sim\mathrm{exp}(-\gamma_{E}E)}\\ &{T_{\mathrm{BD}}=T_{\mathrm{BD0}}\mathrm{exp}(G_{V}/V)\sim e x p(G_{E}/E)}\\ &{T_{\mathrm{BD}}=T_{\mathrm{BD0}}\mathrm{exp}(-\eta_{V}\sqrt{V})\sim(-\eta_{E}\sqrt{E})}\\ &{T_{\mathrm{BD}}=Z V^{-m}{\sim}E^{-m}}\end{array}$      AHI (1/E)     Current (√E)     Power-law (E -m )

Empirical models (e.g., Clustering model) are excluded from this discussion

Different experimental results point to different models

High dependence on experimental conditions, process details, quality of materials,  material thickness…     Selecting an appropriate acceleration model is significant for the final projection results at  use conditions.     Subject of intensive debate over many decades (also now!)     However, the E-model is the only physically sound model that can reproduce the  strong temperature dependence of the breakdown process

## Puzzling Trends 

![1.E+15  Linear-E  1.E+14   En-model  -Root-E  1.E+13   .ENn)  1/E  1.E+12  Target  1.E+11   vE-m   ORegular WL tests  LongtermPLtests（\~270days)  1.E+10  1/E-model ormodelssuchas  1.E+09  ID-model with similar trending.  1.E+08   Packagelevel TDDBresult.  1.E+07  e   1.E+06   E-model  1.E+05  Example lifetimetarget at  100kPOHat0.2MV/cm.  1.E+04  1.E+03   Wafer-levelTDDBresults.  1.E+02  E-field(MV/cm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/97f3c2d2-4ae9-4ea3-bedd-138cd71f5011/97f3c2d2-4ae9-4ea3-bedd-138cd71f5011.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=f08e7cc0aca4370c7f96b1681577eddebcf7b890)
M. Gall et al., AIP Conference Proceedings 1601, 79 (2014)

![1.0E+09  J.Kim,J.McPherson  10 yrs at 105C  IEEE-IRPS,478(2006)  1.0E+07  JSR   BDII CoralFSG   PETEOS   SiO2 (9.0nm Gate Ox)  23   12.6   2.9  3.6   k=4.2   3-yearTDDBStudy  1.0E+05  1.0E+03  1.0E+01  1.0E-01  N  E (MV/cm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7d22f170-d277-4f8b-b6a4-e0c7b25c6ccc/7d22f170-d277-4f8b-b6a4-e0c7b25c6ccc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=133336065a77fb1435a8c746d2d19a5843409e17)
Low-k Silica Interconnects (BEOL)

J. Kim, J. McPherson, IEEE IRPS 2006.

## Puzzling Trends 

![Many FEOL, MOL, and BEOL materials  Many FEOL, MOL, and BEOL materials Cu-based Interconnects (BEOL)  Cu-based Interconnects (BEOL) 1.E+08  BEOL Low-k  Experimental Data   1.E+07   Sio2   (SicOH):  O   1.E+06   6mmm   m-20  C   TvEmpdely   K:2.50  1.E+05   -2.55   SiOCN  Mxpd-E)   1.E183   RSAAm   RefSAm  4/6nm  05   1.522.53  3.5  1.E+02  Electricfield[MV/cm]   Ref. [43]  FEOL  1.E+01   55nm  HfO,  cap.  Porous Low-k Interconnects (BEOL)  Porous Low-k Interconnects (BEOL)  1.E+00   Fsio2  4.8 nm  1.E-01  20  Dielectric Voltage (V)    E-model looks like a good candidate but… -model looks like a good candidate but.  Data      Deviations are clearly seen  Deviations are clearly seen E-model  sqrt(E)-model   Must be extended to account for varying EAo and b  Must be extended to account for varying    and b LE-model  1/E-model     Somehow the concept of carrier energy must enter  Somehow the concept of carrier energy must enter  into the picture  into the picture Field (Mv/cm)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f0dffd76-2002-4b76-8e3f-dc8b85ce9c8a/f0dffd76-2002-4b76-8e3f-dc8b85ce9c8a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=1b284fd0c1ec9f3bf317aedb4c733b8a1101ad29)
![Non-constant EAo and b?  Non-constant   and b? 105-  2.15mm   Sios:  30   1onm   Mn  60  85  11SMMo  110  1-40 -  10  200  240  2.80   Car  ME-T  2.0   2.5   3.0  3.54.0   0.00220.0026   10.003   0.00  Gate Voltage (V)   1/T (1/K)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c8194a94-f466-41f0-aa14-ecba5cb1920a/c8194a94-f466-41f0-aa14-ecba5cb1920a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=439254f288e66a19ed98a34ff7a0d31d0f683d0d)
N. Suzumura et al., Microelectronic Engineering, vol. 106, 2013. E. Chery et al., Microelectronic Engineering, vol. 109, 2013. E. Wu, IEEE T-ED, vol. 66, no. 11, 2019.

## Microscopic Multi-scale Modeling 

##   Important to factors to consider for careful TDDB simulation 

Local temperature and thermal  dissipation at defects (NMP-TAT)     Local field and impact of trapped  charge     All possible charge transport  mechanisms     Thermochemical defect generation     Defects recombination

![STAGEI   STAGEII   STAGEIII  10-4   an  custer  10-6  10-8  /um]  10-10  22  10-12  10-14  C  Voltage[v]  22   42   IN2   22  C  Y   文国   YEenr  TIMEA   TIMEB   TIMEC   TIMED  Y(nm]   SFS  xnm]   Ynm]   SFS  xm]   Ynm]   Sr-S  x[m]   1.5  Area: 109 cm\*  1.101   Va  3.3W  01.5  [uu]   [uu]z  2   ((-T)u1-)u)  101.01  +  -0.5  Y[nm]  5/-5x[nm]   Ynm]  5/-5x[nm]   Y[nm]s/sx[nm]   -1.0  0509c  F. M. Puglisi et al., pssa, vol. 213, issue 2, 2016.  F. M. Puglisi et al., pssa, vol. 213, issue 2, 2016.  -1.5    4. 100rc  0759c  F. M. Puglisi et al., IEEE JETCAS, vol. 6, no. 2, 2016.  -2.0   01259c  M. Puglisi et al., IEEE JETCAS, vol. 6, no. 2, 2016.   simulatiofs  L.Vandelli et al, IEEE T-ED, vol. 60, no. 5, 2013.  L. Vandelli et al, IEEE T-ED, vol. 60, no. 5, 2013.  -2.5  1.0-1   101   103   105.  time to BD[s]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/19beb477-106f-4980-94db-43ac9516f144/19beb477-106f-4980-94db-43ac9516f144.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=500af29998140d3521eef56edac50a17112117c8)
##   Lots of insights 

Spatial and temporal correlation of  defects generation (at late stages)   Thermal runaway process   Defects characterization   Still E-model trends…

## Microscopic Multi-scale Modeling 

##   Recent advances from DFT 

In   $\mathsf{a S i O}_{2}$   wide-angle O-Si-O  bonds (precursors) can trap up  to two electrons     Doubly charged precursors lower the local   $\mathsf{E}_{\mathsf{A}0}$   for vacancy generation process     Link between tunneling (therefore current and carrier energy) and thermochemical model     Effectively results in a powerlaw trend!

Opens up possibilities for  similar mechanisms in other material systems

![EX  e-trapping   e-trapping   capture  178°angle  1/πc12   1/℃c23   AEa=mh  emission  1D   2）D-1   3D2  1/ez1   △Een=nlug  Non forming bonds   e"emission   Y  Metal-ion   Oxygen-ion   anode   defect   cathode  (gate)   (Sisubstrate)  1021   1E+21  SiO2   9nm Dataof[108]  1017   Multi-scale  T=25°C   1E+1  atomistic  1013   simulation of  1E+13   Wieh  109   E=0.7eV  1E+09  1OS  101   ●Vogel data[61]   1E+05  3   Kimura data[62]   Lines: Power-law  10-3   -simulations   1E+01   modelwithm=30  Vg=4.2V   -simulations   Blue line:E,=0.6eV  Vg=4.8V   10-7  1E-03  △Vg=5.4V  -5   15   18  ElectricField (MV/cm)  10-1   10Z   1O5   108   Electric Field [Mv/cm]  TDDB[s]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/92067a77-541a-4bd2-b287-9dd70ab93e1e/92067a77-541a-4bd2-b287-9dd70ab93e1e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=5857512a0ed055926a9b3fa2e156200fd959165c)
A. Padovani et al., Journal of Applied Physics 121, 155101 (2017) A.-M. El-Sayed et al., J. Phys.: Condens. Matter 27, 265501 (2015). E. Wu, IEEE T-ED, vol. 66, no. 11, 2019.

## Applications 

Intrinsic multiple levels of randomness in charge trapping   Stochastic  $\uptau_{\complement}$   and   $\uptau_{\mathrm{e}}$   (e.g., randomness in leakage and RTN properties)   Stochastic defect generation (e.g., stochastic jumps in leakage)   Emerging devices promising for applications that leverage upon randomness

![Security   Computing  Neuromorphic computing  Cryptography,  Secretkeygeneration   Stochastic   Stochastic synapse  spiking  neuron  Stochastic computing  Entropy  Source:   Analoguemultiplication  TRNG  Physicalunclonablefunction  WeakPUF   Strong PUF  Bayesian inference  Tine  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bccb78ea-c469-403f-9a09-5128381dc1a0/bccb78ea-c469-403f-9a09-5128381dc1a0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=8e133b1c330971fd0048b15407c0e44051c9fac5)
![Linearfeedbackshift-register(LFSR)  Pseudo-random  number generator  (PRNG)  Random  CMOS-basedTRNG  number  SRAMmetastability  generator   MOSFETnoise  (RNG)  Stochasticmemory-basedTRNG  True-random  numbergenerator  (TRNG)  Transport luctuations→noise  Switchingvoltage/timevariability  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d0271e2b-9257-417e-94ca-08c6c92ce965/d0271e2b-9257-417e-94ca-08c6c92ce965.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=0deeb33bc4d23078d758f72bf7b7fce5d5f17b26)
## Security and Encryption in the IoE 

##   Security and Encryption in the IoE ecosystem 

Data generated at the edge but processed in the cloud   Confidential/classified information travels over 5G/6G networks   Fast, low-power, reliable encryption (OTP generation)

## Stochastic Computing 

Calculate probabilities with random bit streams   Bayesian inference / Stochastic spiking neurons   Need to control the stream bias (output bit probability)

![Gateway  CenterServer  Enter  vlobile  SMs   ENAL   VOICE  OTP   OTP   OTP  Successful Transaction  Processing  Enter  OTP  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bc54c6d7-e1e0-44a3-8fc8-1600a52190b9/bc54c6d7-e1e0-44a3-8fc8-1600a52190b9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=db5043986f2976157d8c43137f1562a537648634)
Software and traditional hardware RNG are PRNG

Software tools are easily attacked / PRNG are deterministic   Need for TRNG (truly stochastic and unbiased – or with bias control)

![0,1,1,0,1,0,1,0 (4/8)  0,0,1,0,1,0,1,0(3/8)  1, 0, 1,1,1,0, 1,1 (6/8)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/48ba2d54-e215-40f4-a3af-e721f90cf617/48ba2d54-e215-40f4-a3af-e721f90cf617.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=0e1663b0c06d58fd191e4cb8cb39f2e251ec6df1)
## True Random Number Generators 

Concept : exploit an entropy source / stochastic process to generate a nonpredictable, random bit sequence

Examples of entropy sources:

Thermal noise     Jitter in digital circuits     Process variations     Domain (F/M) Switching     Phase or structural change     Chaos (e.g., Chua’s oscillator)     Dielectric Breakdown     Diffusion of atomic species     Random Telegraph Noise

![Time-Domain Noise  ldeal  Clock  Real  Clock  Direction  202  (vu) uouno  198  Time (s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ab17a54b-89a4-4750-a57e-fde22d57b5d3/ab17a54b-89a4-4750-a57e-fde22d57b5d3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=20991d40e5ac4ec467d67c4192aa2e67c2b8c6c0)
## Random Telegraph Noise 

Random fluctuations in read current    Between two/many levels (two/multi-level RTN)   Typically low frequency (up to few 100s kHz)     Present in nearly all devices (FETs, RRAMs…)     Related to stochastic charge capture/emission processes  at defects     Relatively strong PSD

![m'el  30  20  1C  Jm  2000   4000.   6000   8000   10000  Time [s]  Knee Point  1HF  Plateau  -160  Corner Freguenc  10   10  Frequency (Hz)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4d37c4ac-48b0-41a7-bb52-b3cdd834ce70/4d37c4ac-48b0-41a7-bb52-b3cdd834ce70.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=31299e091ac15a519a56868b1d39ff91b18f28f9)
F. M. Puglisi et al. -  IEEE T-IM 2016

![T=340K  ea  8000  8.5   mmh  2000   4  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9edbfefe-bb25-4725-becc-941e9495dc35/9edbfefe-bb25-4725-becc-941e9495dc35.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=eaef1f8dc965e43eb9602c56ab6c533d07dc7380)
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3a50b6d4-2c70-4867-ade6-c5c25d1bd1f8/3a50b6d4-2c70-4867-ade6-c5c25d1bd1f8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=fd3811559ac9f4884acd04eb6694ccb654b0b727)
![口口口 eolset  ipleo letgnuo ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/17897388-f528-4e25-bef3-f55e3960d2e9/17897388-f528-4e25-bef3-f55e3960d2e9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=a038fe191807a65cb21cb88da3ab891f1e03aaa2)
T. Figliolia et al. -  IEEE ISCAS 2016  M. Yoshinaga et al. -  IEEE ISCAS 2016

F. M. Puglisi et al. -  IEEE IRPS 2015

## RTN for TRNG: Concept 

Originally put forward in 2006 by exploiting RTN  fluctuations in nanoscale MOSFETs

Statistically hard to see RTN in MOSFETs

Large arrays of FETs needed, with a complex peripheral  circuitry to increase the chance to find robust RTN with  high PSD

Scheme similar to thermal noise-based circuits:

RTN is more powerful than thermal noise   Truly stochastic (tunneling, that is purely quantum)   Lower frequency phenomenon (lower throughput) than  thermal noise

Remarkable 50 μW @ 200 kb/s – 1.2 V

![von Neumann Algorithm:  moiso   no data  01  mo data  Random  mumbers  Decoder  Quallty  Check  Random  mumbers  Transislorarray  5  4.5  0.9  Entropy   Monte Carloπ  Entropy alfter v.Neumann correclion  0.8  3.5  3_0  MonteCarloπ  MonteCarloπafterv.Neumann cor.  0.6   2.5  2×105   4×105   6×105   8x105   106  SamplingFrequency[Hz]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/be4c5bb1-5ae9-4679-bf5f-16335d46e237/be4c5bb1-5ae9-4679-bf5f-16335d46e237.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=5c3f61e32f071aa4f295435116edbbc85baedaec)
## RTN for TRNG: Possibilities 

IoE requirements can be met  with new devices

RRAM exhibit strong RTN,  especially in HRS

Single device entropy source     Can be read successfully with   just 0.1 V or less     Wide variety of possible current   ranges     Compact and low-power circuit   design     Slow fluctuations

![Ti/5 nm ALD TiO2/Au (5 μm × 5 μm )   Ti/10 nm ALD TiO2/Au (5 μm × 5 μm )   Ti/10 nm ALD TiO2/Au (50 μm × 50 μm  0.05V  14.5  14.0   100μm  0.05  10.0  95  9.0  ua   01  3.0  2.8  2.6  D30  0.52   14.5  0.50   14.0  0.48  13.5  0.46  15   20   10  Time(s)   Time(s)  Ti/10 nm ALD TiO/Au (50 μm × 50 μm)   Ti/10 nmALD TiO/Au (50 μmx 50μm)  0.21   0.25V  270   370  284  258   360  252  3:50  264  258  252   0.21   360  200  3510  264  258   3410  360  270  261   350  258   340  252  12   1-5   12   1S  Time (s)   Time (s)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c72a0379-4268-45f1-aea3-eb031d88def8/c72a0379-4268-45f1-aea3-eb031d88def8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=30369e8b6bf9ade2c1081df078ee600737adb95f)
X. Li. et al., Adv. Funct. Mater., 31, 2102172, 2021.

## RTN for TRNG: Current Solutions 

A solution for the low throughput issue is to  recur to hybrid-TRNGs

Seed a fast PRNG by means of a truly  random source

Proposed combination of:   Low-throughput TRNG based on a h-BN RRAM  device   Non-linear Feedback Shift Register

![Low throughput   Highthroughp  Lowthroughputh-BNbasedTRNG   output   output  REAI   NLFSR  S/H   (24 shift registers  VOUT  CLK   CLKHS  1Mbit/s  1MHz  Lowthroughputh-BNbasedTRNG  hBN   High-Pass   Sample&  Comparator   ToggleFF   NLFSR  RRAM   Converter   Filter   Hold  05  10   20   30  Time(s)  Test   p-ValueResult  Frequency Test   0.174   PASSED  Frequency Testwithin a Block   0.965   PASSED  Run Test   0.285   PASSED  Longest Run of Ones in a Block   0.269   PASSED  Binary Matrix Rank Test   0.722   PASSED  DFTTest   0.557   PASSED  Non-Overlapping Template Matching Test  0.880   PASSED  OverlappingTemplateMatchingTest   0.159   PASSED  Maurer's Universal Statistical test   0.165   PASSED  Linear Complexity Test   0.365   PASSED  Serial test   1.000   PASSED  Approximate Entropy Test   0.9997   PASSED  Cumulative Sums (forward/backwards)   >0.208  PASSED  Random Excursions Test   >0.025  PASSED  Random ExcursionsVariant Test   >0.027  PASSED  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a0163cef-aa67-486c-83c4-14b47c27b9f4/a0163cef-aa67-486c-83c4-14b47c27b9f4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=76d2a95b9eab9ebf17396804ea8b18f799eaec64)
Decouple the bandwidth and power  requirements:

Low-power low-bandwidth amplifier is ok   Low-power comparator   High-speed all-digital NLFSR

## RTN for TRNG: Challenges 

RTN shows a number of instabilities

Multi-level   Non-steady over time   Mutant / Anomalous / Temporary     Complex physics of many intertwined  phenomena: hard to control   Mechanisms understanding is critical     Solutions sought after at both device and  circuit level. Critical role of:   I-V converter gain   Baseline current level can change due to defects  generation/recombination and drift   Filter cutoff frequency (bias compensation)   RTN typical dwell times can change due to  electrostatic interactions, drift/diffusion, and  metastability

![×10  a   8  Ointerstitial  diffusion  20   0.02V  Ointerstitialdiffusion  28   10   15   20  Time[s]  X10  0.02V   1.409  Ointerstitial  162°   diffusion  1.408  1.407  1.406  002V  Ointerstitialdiffusion  1.405  10   15   20   25   30  Time[s]  12  "Ointerstitial  diffusion  12   20  Time (s)  Ointerstitial  diffusion  15元   2203   225   30  Time[s]  X1O  N1408  Diffusion   4075   Ointerstitial  diffusion  1407  Diffusion  14065  Ointerstitial  1406   diffusion  OVodefect   OinterstitialdefectOVacantinterstitialsite  14055  315   201   25  Tme[s]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7ac24939-36a0-4e7f-924e-9516d8edb9f8/7ac24939-36a0-4e7f-924e-9516d8edb9f8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=2c36b34a271a51edaca6dddd6d5b60fe2a808b24)
X. Li. et al., Adv. Funct. Mater., 31, 2102172, 2021. F.M. Puglisi et al., SSE 125, 204-213, 2016.

## The Role of Circuit Design 

A solution to handle multi-level RTN has  been recently proposed using RTN in the  drain current of a MOSFET

Detect the edge of the transitions     Use those to generate square pulses that  are then sampled     Circuit scheme that can be also adapted  to other devices

Still requires stable RTN signals that do  not evolve over time or show instabilities

More compact and energy efficient devices  typically show more complex RTN

Device-level design driven by advanced  physical understanding is mandatory

![a e Drain Current  Sub-CircuitOutput （D）  Differentiator  AbsoluteValue  C  Comparator ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f86c4e9a-6f46-4ffa-9e9c-adca88b4adb1/f86c4e9a-6f46-4ffa-9e9c-adca88b4adb1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=dc5c08534bf37da55e9456e148dd08ada6863628)
J. Brown et al., Sci Rep 10, 17210 (2020).

## The Role of Materials 

Recently, it has been  suggested that some  material systems may  show more stable RTN  signals than others in  specific conditions

Complex scenario, in  which all elements of the  stack matter, together  with operating conditions

|        Sample                number      |        Sample                structure      |        Oxide                thickness      |        Device size                [μm ×μm]      |        Deposition                method      |        Typeof                defects      |WRTN|        IMAX/IMIN                mA]      |        Power                nw]      |        OC/OE                msl      |        Quality                assessment      |
|---|---|---|---|---|---|---|---|---|---|---|
|NO.1|Ni/Al2Os/Au||5×5|||||||        Quality                assessment      |
|NO.1|Ni/Al2Os/Au|5nm|5×5|ALD|        Native                Induced      |||||No RTN|
|||||ALD||||||No RTN|
|No.2|Ni/HfO2/Au|5mm|SXS|ALD|Native|||||No RTN|
|||Snm|5×5|ALD|ALD|        Induced                Native      |        AS                O.S      |60000/24000|189000|2990/7460|
|No.3|Au/HfO2/Au||||||0.85/0.66|0.38|850/580|Poor (unstable)|
|No.4|Ti/TiO2/Au|5m|S×S|ALD|        Native                Induced      ||              |||Poor (unstable)|
|NO.S||||ALD|Native||||| No RTN|
|NO.S|Ti/TiO2/Au|10mm|5×5|ALD|Induced|              ||||Poor (unstable)|
|NO.6|Ti/TiO/Au|10 nm|50×50|ALD||||||No RTN|
|NO.6|Ti/TiO/Au|10 nm|50×50|ALD|Native|        0.05                0_1      |56/52|2.70|        63.3/36.1                62.8/48      |Excellent|
||Ti/TiO/Au|10 nm||ALD|Native|0.15|        116/108                195/180      |11.20||Excellent|
||||||Native|||28.13|48.3/22.2|Outstanding|
||||||        Native                Native      |0.2|270/252|52.20|        40/17.6                24.1/23.1      |Excellent (up-trend)|
|No.7|Ti/TiO/Au|12mm|5×5|Sputtering||        0.25              |370/340|88.75||Excellent (up-trend)|
|No.7||12mm|5×5|Sputtering|Native|0.01|                2400/2000      |||No RTN|
||||||        Induced                Induced      |||NN|        230/420                100/260      |Excellent|
|NO.8|Ni/TiO/Au|12nm|S×S|Sputtering|Native|        -0.01                0.02      |        -1900/-2200                11.5/6      |        20.50                0.18      |29.6/27.2|        Excellent                Very good (anomalous)      |


2D materials may play a  very interesting role in  creating stable signals  (e.g., h-BN)

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fa7dc099-bca6-4fff-a048-0ae8410ecb60/fa7dc099-bca6-4fff-a048-0ae8410ecb60.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=b222b20474f918b6789637f2196a535505b8c416)
## The Role of Materials 

Combining DFT  calculations, molecular  dynamics, and multi-scale  physics-based simulations  provided the understanding  of the defect physics in  multilayer 2D h-BN     Clever circuit design based  on the device physics  specifications ensured the  design of a successful  hybrid TRNG achieving 1  Mbit/s truly random bit  stream also for very long  sequences     Currently the chip is under  fabrication… more to come

![17 Mbit sequence 17 Mbit sequence  @ 1 Mbit/s @1 Mbit/s  Firstvacancy   ·P2   口.P3   P4   P5  P6  Secondvacancy  Thirdvacancy  00.20.40.60.811.21.41.61.82  5   6   8  9101112  VacancyFormationEnergy(eV)   z（nm)  54  54 C. Wen et al., Adv. Mater. 2021, 33, 2100185.  CWen etal   Ao  Mater.2021.33.2100185  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/649c923e-91e0-4b4e-91a4-5ff18c84f76b/649c923e-91e0-4b4e-91a4-5ff18c84f76b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=40e7d27c50544c2316b9672250aa2486d7d5cf29)
## Common Misconceptions 

Poole-Frenkel conduction (and some other models)     If it fits it must be it! (especially charge transport and TDDB)     Metastable states used “freely”     Defects do not move (FEOL)     Defects classification with RTN   “Simple” RTN means simple physics and defect scenario     Ignore trapped charge field contribution     Empirical models and derived claims     Test conditions vs. use conditions

## Common Misconceptions 

H. Schroeder, Journal of Applied Physics 117, 215103 (2015)

![[a] -15-  Sehe tky   Frenkel-p oole  2二—   -0.1y.   33  -25-  -38  Reverse  300   1500   300心   1500   3000  E12 (v/m}1/2   E1/2 (v/m}12  [b]-21[  Ohmic.1bduetion   Frenkel-Poole  -2  -0.14\*.  Slope = 1.1  39  Forw ard  -30  1500   3000   4500  Irl ]   E12 rv fm 112  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e527c192-b105-4fe0-b12d-d070a4ad5568/e527c192-b105-4fe0-b12d-d070a4ad5568.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=9f4e0d043f35f69ee70055e32def497672fbe3c8)
If it fits, check for parameters values!

![-8.0-(a) schottky Emission   （b)Poole-Frenkel  Region   -6.4   Emission Region  -8.51  =-9.01   GATE   OXIDE  -9.5-   6.8  -10.0-  0.3   0:4V(1/2)  0.6   7.0   07   0.8  √v(volt1/2)  OFPEecp  Poole-Frenkel Emisxio   Sehottky Emission   KBT  4  265K   2SK  20K  195k   4255K  10   30k  325K  2   340K   340k  810840870900930   810.840870900930  E²(V/em）)2   E2(V/em）  D. Tomer et al., Appl. Phys. Lett. 106, 173510 (2015).  D. Tomer et al., Appl. Phys. Lett. 106, 173510 (2015). 58  56  S. Munjal et al., Sci Rep 7, 12427 (2017).  S. Munjal et al., Sci Rep 7, 12427 (2017).  K. Jung et al., J. Korean Phys. Soc. 59(4), 2778 - 2781 (2011).  K. Jung et al., J. Korean Phys. Soc. 59(4), 2778 - 2781 (2011). ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ac886e5b-b793-4485-b5e1-3c76cf3bf0eb/ac886e5b-b793-4485-b5e1-3c76cf3bf0eb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215813%3B1743219413&q-key-time=1743215813%3B1743219413&q-header-list=host&q-url-param-list=&q-signature=b7f59362a4f3fbb65db573bba342ca092ceac481)
Poole-Frenkel conduction is ALMOST NEVER the dominant conduction mechanism!

## Conclusions 

Importance of a correct theoretical framework for charge trapping     Charge trapping subtends all the main reliability phenomena     Complexity emerges from relatively simple scenarios     Key mechanisms have strong interdependencies     Defects Generation   No consensus but good progresses after several years!   Importance of atomistic modeling and multi-scale simulations     New applications are emerging in which defects are exploited as a resource!   True Random Number Generation   Physical Unclonable Functions   Defects engineering can be a futuristic and exciting way     Misconceptions should be carefully addressed to avoid inconsistencies and confusion

