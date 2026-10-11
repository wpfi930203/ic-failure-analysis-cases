---
title: "tut-8.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_7ef5e13b31d59b6a395a4d0c492979777295230462135641
file_size: 8234898
---

## characterization, reliability   characterization, reliability GaN devices, technology, and Gaudenzio Meneghesso challenges and future prospects 

Enrico Zanoni, Matteo Buffolo, Carlo De Santi, Matteo Meneghini andGaudenzioMeneghesso Department of Information Engineering, University of Padova

## Outline 

Outline

A few words on Gallium Nitride • Scaling in rf GaN HEMTs control of short channel effects vs trapping  Deep level effects - double pulse is not all · Scaling in rf GaN HEMTs control of short channel effects vs trapping  modeling the effects of traps  reliability effects due to C doping  P-gate normally off issues : introduction Reliability of RF GaN HEMTs

• A few words  on Gallium Nitride

• Deep level effects – double pulse is not all

• modeling the effects of traps

• reliability effects due to C doping

• P-gate normally off issues : introduction

• Reliability of RF GaN HEMTs

2

## Properties of Gallium Nitride 

Properties of Gallium Nitride

3

Si

GaAs

1.42

Material

(eV)

1.12

G

E

12.9

ε

r

9400

11.7

(cm

1440

/Vs)

µ

2

0.3

E

crit

|Material                     Si      GaAs      4H-SiC|GaN |β-Ga2O3            Diamond          AIN|||
|---|---|---|---|---|
|Eq(ev)|1.1２     1.42           3.23|③.4|4.9                        5.5                 ６.2||
||１１.７      12.9           9.66|8.9|¥10                         5.7                 8.5||
|μ (cm2/Vs)|144０|94００           950|140０|250                      4500               450|
|Ecrit (MV/cm)|0.③|0.4             ２.５|③.③|8×                        10＊                15*|
|Vs (x107 cm/s)||0.9                I|2.4|１—１                         2.③                 1-4|
|Kth (W/cmK)|1.③       0.55            ③.7                     2.0                     0.1-0.3                     2③                2.85||||


GaN  1400

(MV/cm)

cm/s)

(x10

1

7

s

1.3

(W/cmK)

k

th

0.55 semiconductor with

•

the largest energy gap

•

the largest critical field

the highest saturation velocity

•

v

Values from

https://doi.org/10.1007/978-3-030-20208-8_2

3.4  8.9  3.3  2.4  2.5 thelargest energy gap the largest critical field the highest saturation velocity

4

> ideal candidate for power semiconductor devices (high temperature/high voltage)

0.4

0.9

to higher

a

and

along

Figure:

![characteristics Electronegativity  anionic  spontaneous polarization , GQ   As a consequence,  I(Ga)face    has electronegativity [0001]   GQ   have (-)  the (0001) axis  On top of this polarization! [1120]   [1100]  Nitrogen  GO  gallium.  cationic GQ   atoms B (N)face  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/38b80711-ad5e-405d-9856-743c637ff860/38b80711-ad5e-405d-9856-743c637ff860.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=76e27747c33548b0609b2874601292acad0498d8)
)

## compared  (+)  ''   

-2

GaN (C m

-0.029

Material

''

-0.034

''

Image: https://sciencenotes.org/wp-content/uploads/2019/09/ElectronegativityTrend2.png

Piezoelectric

) -2

Nitrogen  nas  higher electronegativity,  compared  tC gallium.

-0.032

|Material|GaN (C m-2)|InN (C m-2)|AIN (C m-2)|
|---|---|---|---|
|Psp|-0.029|-0.032|-0.081|
|Psp|-0.034|-0.042|-0.090|


|||||||
|---|---|---|---|---|---|
|2.04|2.55|3.04|3.44|3.98||
|        A                1.61      |        S                1.90      |2.19|2.58|3.16||
|        31                ea                1.81      |        32                Ge                2.01      |        33                AS                2.18      |        34                se                2.55      |        35                Er                2.96      ||
|        249                178      |        50                sn                1.963      |        ST                2.05      |        52                21      |        53                2.66      ||


InN (C m

-0.042

Asa  conseguence,  Ga  and atoms  have  anionic (+)  and cationic  characteristics spontaneous polarization Psp along the (0001) axis

On top of this →   Piezoelectric polarization!

## Band diagram and charge distribution in an AlGaN/GaN HEMT Dashed: realistic profile 

Both the

GaN and the AlGaN layers are typically

Conduction band  $10^{15}\,\mathsf{c m}^{3})$

, to minimize electron scattering at

When a potential Vg is applied to the gate, the charge in the 2DEG can be modulated:

impurities.

left undoped

$$n_{s}(V_{G})=\frac{[Q_{\pi}(A l G a N)-Q_{\pi}(G a N)]t+\epsilon\left[V_{G}-\left(\phi_{b}-\frac{\Delta E_{C}}{q}\right)\right]}{q(t+d)}$$
weak n-type conductivity

Undoped GaN has a

epitaxy (always higher than 10

)

-3

cm

15

the 2DEG can be modulated:

−

When a potential

−

=

'

![AlGaN   GaN   Substrate  qNDD   +Qπ(AlGaN)  Qπ(GaN)  -Qπ(GaN)   YS  —Qscr  -Qπ(AlGaN)  ECz1  ams  EGaN  EGCN  [qNbD -Qn(AlGaN)]  EAIGaN  EAIGaN  Solid: approximated profile  6 Conduction band  Dashed: realistic profile  qVAIGaN  AE  EC  qVGaN.  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/38cab751-6b18-4d90-84d4-99a77f2dd918/38cab751-6b18-4d90-84d4-99a77f2dd918.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=eed8ecd636e616b87e9fd01b136ce1383571dcd2)
conversion applications

Current development of lateral GaN HEMTs for RF and powei conversionapplications

1. Power GaN HEMTs for switching applications

7

## The  

Silicon

![GaN power devices are typically grown on a silicon substrate (6’’-8’’) large lattice mismatch results in high  threading dislocation densities Typical structure of AlGaN/GaN power HEMTs  Field plate  Drain  Source  Gate   Passivation  AIGaN/GaN HEMT  Silicon  MAS5.0kV2.7mmx15.0k   3.00um  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6dd16c93-b24c-4152-bb9f-d9f5c77c4bef/6dd16c93-b24c-4152-bb9f-d9f5c77c4bef.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=397043562cf2707d8fd1a6450731d3eff0193321)
CrosssectionSEMimageof0.5/mNRF1field platedAIGaN/GaNHEMTtechnology(Nitronex)

https://iopscience.iop.org/article/10.1149/2.0251602jss/pdf

Image: htps://www.richardsonrfpd.com/docs/rfpd/Nitronex Substrates for GaN RF Devices App%20Notes.pdf https://iopscience.iop.org/article/10.1149/2.0251602jss/pdf https://drupal.limec-int.com/sites/default/files/inline-images/GaN-on-200mm%20Si%20wtafer.ig

Image:

GaN power devices are typically grown on a silicon substrate (6"-8')→ The large lattice mismatch results in high threading dislocation densities

![GaN Buffer Layer  AIGaN Transition Layer  soonm  8 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f575771f-389e-4247-9264-106a80855c22/f575771f-389e-4247-9264-106a80855c22.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=5ce1fe3c563881883a54fa282f46963ae7243255)
## Ron vs BDV for power devices resistive  

The off-state voltage is supported by the gate-drain access region devices, the

The on-resistance then depends on the breakdown voltage:

Ron = Rchannel + Rdrain
Decreasing the gate

![supported by the gate-drain access region    /   Wg quns   Ecrit  Decreasing the gate  length from 1 μm to  The on-resistance then depends on the breakdown voltage:     10  . -LG=0.25μm, Ecrit=1 MV/cm   4 0.25 μm can lead to a   10 '  Lg=1μm, Ecrit=1 MV/cm  substantial reduction  1 - LG=0.25μm,Ecrit=3.3 MV/cm  in the resistive losses   = 1 , 3  Breakdown voltage (V)   Ueda, Properties and Advantages of Gallium Nitride (in Power GaN Devices) 10 ()%\*"  %110  =1 MV/cm  =3.3 MV/cm =1 MV/cm      9 crit  crit =0.25 m, E  crit =0.25 m, E  2 #\$%""&'  10-2  101  =1 m, E  10２   103  10  104  Breakdown voltage (V)  G  G  G ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a8476d29-5a96-46fb-90f7-0d174bf29b92/a8476d29-5a96-46fb-90f7-0d174bf29b92.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=664b98fe112a6cd116873ce3329519a6dee915e9)
length

0.25 µm can lead to a

substantial reduction

The off-state voltage is

from 1 µm to

See also:

in the resistive losses

![LGD  AIGaN  Rchannel   Rdrain  GaN  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b2643df3-ce74-4e48-a32c-75d96bf9fdec/b2643df3-ce74-4e48-a32c-75d96bf9fdec.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=602d8e4ba8d7ccf991ce17656c4d489b9da17ff5)
For high breakdown voltage devices, the resistive contribution of the gatedrain access region becomes relevant

See also: Ueda, Properties and Advantages of Gallium Nitride (in Power GaN Devices)  =

!"

1

10

0

10

-1

10

1

10 -2

10

S +

n p

![Lateral GaN device  Vertical GaN device Oxide  GaN-on-Si epi   GaN and substrate  high speed, highest mobility, already on the market on silicon substrate high breakdown voltage, high current capability, several concepts  Vertical GaN device  - Surface passivation   n  Oxide  + +  n pn  （b)   Alo.2Gao.8N  AIGaN barrier  S  Edge   Metal  region   GaN  uid-GaN channel  n-Nrift reg:on  Alo.17Ga0.83N  Buffer layer(s)  GaN-on-Si epi  http://dx.doi.org/10.3390/ma11101968 Alo.35Ga0.65N  AIN   n+ GaN an d substrate  AIN nucleation layer  Silicon   -100nm  Si-substrate  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cb835009-543d-4092-9732-9fc4c8030ad7/cb835009-543d-4092-9732-9fc4c8030ad7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=198ac67edcc789bf5b137ed9a6898ffa3358da0d)
Lateral GaN device

Surface passivation

S

G

AlGaN barrier -----------------------------------------

1

(

uid-GaN channel

(

Buffer layer(s)

AlN nucleation layer

Si-substrate

Two main device architectures:

## Lateral vs Vertical GaN transistors  drift region 

Lateral:

•

Vertical:

•

proposed

Two main device architectures:

· Lateral: high speed, highest mobility, already on the market on silicon substrate · Vertical: high breakdown voltage, high current capability, several concepts proposed

D

## Options for Enhancement mode operation 

Options for Enhancement mode operation

p-GaN gate

![Drain   cascode configuration  Drain  650#   650-1200V  GaN HEMT  max 7nv  max20.v  16U  Silicon MOSFET  8  Oun  Co  TGate   Gate  11 p-GaN gate   cascode configuration  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9b87bfd5-dfd2-497f-8e15-251d1f2599c8/9b87bfd5-dfd2-497f-8e15-251d1f2599c8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=44b305011e2050f78603f73e4a383f0a069bd2df)
## Design of p-GaN gate 

![The use of a p-GaN gate lifts the conduction band diagram at the AlGaN/GaN  p-GaN  Afterintroductionofa  interface, resulting in normally-off operation AIGaN   AlGaN  p-GaN cap layer  AE   GaN  中B   GaN  Metal   AEF   Metal  metal   AiGaN   GaN   metal   p-GaN   AlGaN   GaN  Normally-onoperation   Normally-offoperation  (AlGaN/GaNheterostructures)   (p-GaN/AlGaN/GaNheterostructures)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ed35f877-a005-46fc-8259-2eae79852ae2/ed35f877-a005-46fc-8259-2eae79852ae2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=1f66e16cbe953f3e84f0f266c657f5e87a49bb09)
Design of p-GaN gate

Figure:

12

Figure: http://dx.doi.org/10.1016/i.mssp.2017.09.027

## Design of p-GaN  gate 

![Simulated conduction band diagrams of a p-GaN/AlGaN/GaN heterostructure, for two different values   50  E。XAIGaN=0.12   EctAGaN=15nm   C  -EF   EE   AO  )    )    are needed (see (c))  uuu)   ③0   normally-on  20  dAIGaN=25nm   Al26Ga74N   10  Ga   GaN   GaN   normally-off  25   5075100125150   25   5075100125150   8.0   0.1   0.2   0.3  depth (nm)   depth (nm)   Al molar fraction, x  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ac111b49-2771-46aa-8ef2-79de3b22d2c2/ac111b49-2771-46aa-8ef2-79de3b22d2c2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=82e93d5d8988762eadc04ecf93b7fe6fa38cbce7)
Design of p-GaN gate

•

•

For normally-off,

Figure:

13

## Driving a transistor with p-GaN gate: gate resistors 

Rg controls switching speed  Separate Rg for turn-on and turn-off

## Turn-on resistor 

• R

G

controls switching speed

for turn-on and turn-off

• Separate R

G

Turn-on resistor

• Controls turn-on slew rate

• Too small

· Controls turn-on slew rate   · Too small → high dV/dt, drain current ringing

## Turn-off resistor 

· RGoFr Smaller than RGon, to obtain strong pull down  , to obtain strong pull    undershoot  · Too small RgorF may create Vgs under oaepoerorrf teDriver（OFF）

Turn-off resistor

• R

smaller than R

GOFF

down

GON

• Too small R

GOFF

may create V

and ringing

GS

CGD

For driver with single output

![RGON  RGOFF  LowVfSchotikyiDiode  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5f0b19f3-1733-4a29-8997-ddd8a061a84d/5f0b19f3-1733-4a29-8997-ddd8a061a84d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=43af8a6aa7dbcf99b5bc3afa534fc7d4823cf5a8)
![RGONI  POUT  RGOFF  NOUT  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a003dd2-d59f-4a7f-ad49-309952545c28/7a003dd2-d59f-4a7f-ad49-309952545c28.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=896824096b408b7c8b77a92052e351d81331b097)
![VDRN  RGLON   14 RGOFE  DCLANP  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e8cf1870-dafb-4133-9700-72455806cb54/e8cf1870-dafb-4133-9700-72455806cb54.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=ac8458a86f5df994bf840711eb2b4572623b8574)
For driverwithseparatepullup/down outputs

Preferred Approach

## Driving a GlT: turn-on 

GS  (V p

![RG2   , steady electric current flows through D  can be selected to produce a relatively   ApplicationNote_CoolGaN_600V_emode_HEMTs_Driving_CoolGaN_high_electron_mobility_transistors_with_EiceDRIVER_1EDI_CompactGate Diver IC Output Voltage  Driving  VGS.SS   Signal  ON (PulI-Up)   RG1ml   CSU   https://industrial.panasonic.com/content/data/SC/ds/ds8/c2/APN_PGA26E07BA_EN.pdf IG,SS   V   VGSF  PWM-   Ree   IG.PK=  Wpvs   ApplicationNotes-v02_00-EN.pdf?fileId=5546d46262b31d2e016368e4d7a90708  vgs  8<  RG1   Exponential Decay, t=RGCsu  OFF (Pull-Down)   ; −  IG.SS  VP-VGS.SS  RG2   [A]Vneg1  OA   O  7 89 7   Vcc Csu    89  neg1   ((Csu+Cg)   GSF  :7 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/01f4f569-e8aa-432a-b694-22a1cbbe6c80/01f4f569-e8aa-432a-b694-22a1cbbe6c80.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=d6bb0e82d7297517dc7a186c59e1b6cab233269d)
Turn-on:

‐

scale current stable mA

Source:

https://doi.org/10.1002/9781119594406.ch3

Driving a GIT: turn-on

$\left(D_{P}\right)$   = −   $\mathsf{V}_{\mathsf{G S,S S}} $  https://doi.org/10.1002/9781119594406.ch3 https://www.infineon.com/dgdl/Infineon-   $\mathsf{D}_{\mathsf{p}}$   $\mathsf{R}_{\mathbb{G}2}$    "&56  GS,SS

Turn-off: negative bias is applied to the gate thanks to the Rgs/Csu network

when parasitic diode (

) reaches the V https://industrial.panasonic.com/content/data/SC/ds/ds8/c2/APN PGA26E07BA EN.pdf   https://doi.org/10.1002/9781119594406.ch3   https://www.infineon.c com/dgdl/lntineon   ApplicationNote CoolGaN 60oV emode HEMTs Driving CoolGaN high electron mobility transistors with EiceDRIVER 1EDI Compact  ApplicatiogNotes-v02 00-EN.pdf?fleld=5546d46262b31d2e016368e4d7a90708

3

2

## Origin of Electron Traps 

D

Origin of Electron Traps

pseudo-trapping effects may •

p-GaN gate in a Schottky

-----------------------------------------

junction e-mode HEMT

p-GaN gate in a Schottky iunction e-modeHEMT Surface passivation p-type buffer in case of strong C doping

within electrically insulated layers:

buffer or channel and backbarrier

C doping

also occur due to charge storage

at the back interface between

•

or nucleation layer

![within buffer due to Fe or C compensation, residual C after MOCVD growth, defects  at device surface  Surface passivation  within AlGaN and its  AIGaN barrier   interfaces  uid-GaN channel  uid-GaN channel  AlN nucleation layer  or C compensation, residual  within buffer due to Fe  Buffer layer(s)  Si-substrate  C after MOCVD growth, defects  Buffer layer(s)  AIN nucleation layer   Si substrate for power  Si-substrate   16  devices, SiC (rarely  sapphire) for RF ones  different mismatch  different defectivity  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4fe313e8-7c8a-4972-9d94-2ac55f7053c1/4fe313e8-7c8a-4972-9d94-2ac55f7053c1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=162309360bfbceb5d22040a739689721d104f960)
at the back interface between buffer or channel and backbarrier or nucleationlayer

G

S p-type buffer in case of strong

## Trapping effects in GaN HEMTs: Current Collapse 

![VPP  Trapping effects in GaN HEMTs: Current Collapse  Measured by pulsing from =0,   Measured by pulsing from  G_QB  vdd  recoverable decrease in  (50V)   G_QB  trapping conditions (V  drain current induced by trapping R  rest conditions (V =0)  =50) Current Collaps  DUT  1us  e D_QB V Current collapse  VSS   Current collapse  C-8  0.2  0.15  0.15  IDEAL  Siump   0.05  0.05  -0.02   0.02  0.040.06  0.080.1   -0.054-2   10  12  TIME(S)   TIME(S)   ×10  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9f007f6c-ea7e-452d-b4f4-76521be3e4ea/9f007f6c-ea7e-452d-b4f4-76521be3e4ea.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=937d5eba511c3fdf35376e0e6afefd606be1def7)
DD (50 V) V

1 µs

99 µs

ON

ON

ON

OFF

V GS (-8

OFF

Slump

V)

OFF

![transient before reaching steady-state value  0.8  The same happens if ID-VD curves are   Ton/ToFF = 1 μs/999 μs - VG = 0V - LGD = 10μm  Current  collapse  0.6  uuuu   measured from several QBPs 0.4  Measured by pulsing from  rest conditions (Vg_QB=0,  0.2   Mreasured by pulsing from   trapping conditions (Vg_QB=-8,  Vd_QB=50)  0O  10   12  VDS(V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4a00060f-50af-48c3-80dd-5860995631c6/4a00060f-50af-48c3-80dd-5860995631c6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=7d45f95942f081293006224fe4d63cf4bed6617d)
phase

Current collapse → recoverable decrease in drain current induced by trapping When a HEMT is switched on after a trapping phase → current shows an exponential transient before reaching steady-state value The same happens if ID-VD curves are measured from several QBPs

IDEAL

## Improved setup for CC evaluation 

![Low-Voltage   High-Voltage  Modules   Power Amplifier  PA   Double-Pulse  Drain   (this work)  Pulser   conventional  gate-lag  Scope  Rsense  TV  DS  diff. probe  IRsense  PA   DUT   DS  Gate  Pulser  optional  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/86be7855-2b83-4325-8ab0-d91038bef4ee/86be7855-2b83-4325-8ab0-d91038bef4ee.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=90450851df8802098ef1698a98c19da04196879f)
## GaN-HEMT, Parasitics: Current Collapse 

GaN-HEMT, Parasitics: Current Collapse

![0.6   Traps in the access  Traps under the gate   0.8  regions  Traps in the access  0.5  regions  0.6  0.4  0.3   ()  0.4  (Vg,qiVd,q)   sa  (0v;0v)  Where are  0.2   (-6V;0V)   (ov;0v)  (-6V;10V)   the traps   0.2   (-8V;0V)  (-6V;20V)   (-8V;10V)  0.1   (-6V;30V)   located?   (-8V;20V)  (-8V;30V)  (-6V;40V)  (-8V;40V)  (-6V;50V)   0.0   (-8V;50V)  0.0  81012  Where are  the traps located?  1015202530  VDS(V)  VDS(V)  AlGaN   AlGaN  GaN   GaN  AVTH   ARON   AVTH   ARON  ) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bcf9dfad-ee28-409e-93d3-43b95b0d3ea9/bcf9dfad-ee28-409e-93d3-43b95b0d3ea9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=c023fe8f992049100f33e4b18b3985f45c2d84b0)
(V

D,Q

;V

G,Q

## Origin of Dynamic-Ron 

![0.4   Trapping in off-state may induce a non-monotonic variation of on-resistance ToN/ToFF = 20μs/2ms -VG= 0V   35  Tamb  一口-30°C  0-50°℃  Setup for pulsed   75°℃  0.3   V-100°C  characterization   150°C  125°C  ()   0.2  SCOPE   (0v:0v)   0  -20V:0V)  20V:50V）  20V:100V)  0.1   20  ：200V   15  20V；300V)  20V;400V)  -20V：500V)  -20V；600V)  1OD  0.0  W   [20.020.0,100200300400500,00)  (2020（20（202020（20  VDS(V)  (VGSQ,VDSQ)(V,V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4e8575c3-a7e8-4194-8b9f-171e9b705b02/4e8575c3-a7e8-4194-8b9f-171e9b705b02.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=a32654c1e0941c13550cde51efaa3a8aea6819f4)
Origin of Dynamic-Ron

Setup for pulsed

characterization

Meneghini et al.,

20 Trapping in off-state may induce a non-monotonic variation of on-resistance

## N  decrease in  <200 V, C )  DSon 

C-doped GaN

1: ionization of buffer

)

acceptors (C

N

BTB

![DS carbon at nitrogen site acceptors in the buffer are ionized,  and this induces a significant  increase in dynamic-R  , charge is  redistributed;  increase in vertical  Strain-relief layer  , vertical (drain to  substrate) leakage becomes    field-assisted detrapping may  also lower dynamic-Ron In off-state, at V  DS  leakage; BTB   DS on  For higher V 1: ionization of buffer  acceptors (Cn)  How to explain the non-monotonic behavior?  C-doped GaN  for higher V  3: at high Vps, vertical  leakage dominates  dynamic-R  relevant (  Note: BTB  1)  Positive  2)  3) BWE  charge   P-FEFFECT  2: leaky UiD promotes transfer  ofelectronsto2DEGandflowof  positive charge (reduction in  UID GaN  dynamic Ron)  AlGaN  , vertical  EEETRA   CTIONSONELECTRONDEVICESVOL64NO.7,ULY2017  Strain-relief layer  "LeakyDielectric"Model for theSuppression  leakage dominates of DynamicRon in Carbon-Doped  DS AIGaN/GaNHEMTs  MichaelJ.ren,MemberEEE,SergeKarboyan,IndranilChatterjee,Member,EEE,AlexanderPooth  PeterMoens,AbhishekBanerjee,andMartinKuball,SeniorMember,EEE  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/962d0175-054e-4165-b101-73a1c41f2f0a/962d0175-054e-4165-b101-73a1c41f2f0a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=296d22e0798a455365f3149157816c2836bdbc1f)
UID GaN

dynamic R

AlGaN

)

Meneghini et al.,

http://dx.doi.org/10.1016/j.mssp.2017.10.009

https://doi.org/10.1016/S0040-6090(99)00344-2   $\Rightarrow$   ${\sf V}_{\sf D S}$  21  ,

Positive

charge

on

## Current development of lateral GaN HEMTs for RF and powe conversionapplications 

2. RF GaN HEMTs

2.RFGaNHEMTs

conversion applications

22

\\

![Scaling requires maintaining high aspect ratio Lg/d In order not to loose current: increase aluminum content tailor polarization (Al)InGaN, AlN,   adopt N-polar architecture Vertical scaling to suppress  Multichannel and castellated  Control short-channel effects high compensation (Fe+C)  (tradeoff with collapse) 'short-channeleffect"  Reductionofparasitic   Gate  ScAlN barrier  Gradual channel  use backbarrier Surface passivation to reduce  resistance/capacitance  current collapse  Source   Linearity Drain  HEMTs         Lateral scaling toreduce   Longer gate-to-drain separation  electron transit time   for improved breakdownvoltage  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ec942ed2-6f10-49ed-aa25-5ea0633d7571/ec942ed2-6f10-49ed-aa25-5ea0633d7571.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=043c8260151ce8aa44ee10937685125512907f1b)
scaling

## AlGaN 

adopt N-polar architecture    $(\mathsf{F e}{+}\mathsf{C})$  23

## Issues with Fe and C compensation in short-channel devices 

1.GaN HEMTscaling   2. GaN buffer compensation with Fe and C   3. Carbon acceptors: hole redistribution effects   4. Carbon acceptors and hot electron degradation

1. GaN HEMT scaling

6. Separating C

Solving dispersion vs short-channel effects trade-off with backbarrier

N

5. AlGaN backbarrier vs Fe-doping   6. Separating Cn acceptors by an AlGaN backbarrier

2. GaN buffer compensation with Fe and C  3. Carbon acceptors: hole redistribution effects   acceptors by an AlGaN backbarrier  24

Conclusions

## Contribution of leakage to charge trapping 

Dependence of current collapse on the quiescent bias point applied to the gate

In off-state conditions → current collapse increases with gate leakage (electrons injected from the gate)

Contribution of leakage to charge trapping

In off-state conditions

20

Current Collapse (%)

18

16

14

12

10

Quiescent bias for

=0 V

V

DS

8

-7

-8

![Dependence of current collapse on the quiescent bias point applied to the gate  current collapse increases with gate leakage   - e 20   - e - e  Current collapse  -  Gate leakage   ()  m  18   e 16  e   Gate leakage (µA/mm) 6  4  2  0 Quiescent bias for   (a)  -3 10   currentcollapsemeasurements:   Current collapse  Trapping voltage on the gate (V) Vps=OV   25  Gate leakage  -4 GB  Trapping voltage on the gate (V)   -5 25  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/68a47339-fc94-4798-84f3-fefc41de5a33/68a47339-fc94-4798-84f3-fefc41de5a33.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=47285af644d1038b0961e33fe75c59a556781eea)
-6

−3

##  cm  s µ 18 

s µ

DSQ

GSQ

![Fe concentration at SiC interface 1 × 10 Concentration constant till 0.6 µm from the   then one decade decay every 0.4 μm  = 0V, 100 1000   = - 3.8V, V (VGsq=0V;VDsq=0V)  m-gate AlGaN/GaN HEMT  (VGsq=-3.8V:VDsq=40V)  AlGaN/GaN interface,   DSQ 800  (Vgs from -2.5V to 0V steps 0.5V)  approaching 2DEG   = 0V, V u   600  Frequency dispersion effects – Fe Doping  Fe-doped buffer GSQ µ s  Dashed line: Stress off-state V 400   Solid line: Quiescent V Measure : 1  200  • •  • µ O  VDS(V)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/67608cac-6af6-444e-a3f2-35805e30c059/67608cac-6af6-444e-a3f2-35805e30c059.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=6e5e2e512a50b38873c53fd7d6b82860051a8368)
## Fe-doped buffer 

Fe concentration at SiC interface 1 x 1018 cm-3  $1\times10^{18}\,{\mathsf{c m}}^{-3}$    Concentration constant till 0.6 μm from the   AlGaN/GaN interface,   then one decade decay every 0.4 um   approaching2DEG

µ

## Solid line: 

Quiescent VgsQ = 0V, VpsQ= 0V, 100μs Measure : 1 μs

$\mathsf{V}_{\mathsf{G S Q}}\!\!=\!\!-3.8\mathsf{V},\,\mathsf{V}_{\mathsf{D S Q}}\!\!=40\mathsf{V},\,100\upmu\mathrm{s}$  26

https://doi.org/10.1109/TED.2021.3081613

,

## =-3.8V,   2 

cm

![m-gate AlGaN/GaN HEMT,   GSF  Activation energy 0.52 eV 300C   s V  ×  10 40°C  Fe-doped buffer µ  Cross-section 5  500C  Drain Current Transient Spectroscopy – Fe doping  60°C  700C   Filling pulse 1  increasing T  =40V  a  µ 0.5   DSF m   V  30°C  40°C  500C  )10L60//a/   32   3   36   60°C  70°C  g/kT (eV-1)  S   3  10   10   10   10   10   10   10  time (s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/18066978-77ad-4479-93e6-a3b7334cc50b/18066978-77ad-4479-93e6-a3b7334cc50b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=65ccfd38401f4fd59d93adf2d007886cc1b50ed7)
![vol. 68, no. 7, pp. 3325–3332, 2021, doi:  Drain Voltage VDs  https://doi.org/10.1109/TED.2021.3081613 Vps,pulse  Drain Current I,  VDs, steady   ID, steady  DCT  Gate Voltage Vgs  D,pulse  VGs, steady  DuT  VGS.pulse  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e9a2d8ad-3be5-4391-91f2-4c9a685bd78a/e9a2d8ad-3be5-4391-91f2-4c9a685bd78a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=65b0340c4011a1dfb38c857449d63716762bca23)
0.5 μm-gate AIGaN/GaN HEMT,   Fe-doped buffer   Filling pulse 1 μus Vgss=-3.8V,   VdsF=40V   Activation energy   0.52 eV   Cross-section 5 x 10-16 cm2   M. Cioni et al., IEEE Trans. Electron Devices   vol. 68, n0.7, pp. 3325-3332, 2021, doi:   https://doi.0rg/10.1109/TED.2021.3081613

,   is

2

-16

## Deep levels related to Fe in the current  

The deep-level E2 with

![M. Meneghini “Role of buffer  doping and pre- existing trap states   collapse and  degradation of  AlGaN/GaN HEMTs,”  IEEE International  Reliability Physics  Symposium 2014  related to a defect whose concentration increases with Fe-doping (can be  +3 eV  – 10 0.0041  sampleA  (') snds ssuoo    ··sample B  0.003   Increasing   sampleC   d   y   V Fe doping   SampleD   +2.5 eV and/or E  4x1017  -14 E2   = 10  2x1017  0.002  1x1017  0.002  Nfe=O   0.001    σ and 0.000   0.000   V 10   1011   101   10   10   10   10   Fe doping  Time (s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/eb0f30ac-ba8e-4edd-b38e-f0751e3716f6/eb0f30ac-ba8e-4edd-b38e-f0751e3716f6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=3853e80c9991d9d4a0fbc89253c239bb1e7ad021)
M. Meneghini et al., "Role of buffer doping and preexisting trap states in the current collapse and degradation of AIGaN/GaN HEMTs," IEEEInternational Reliability Physics Symposium 2014

0.6) eV  ÷

E2 corresponds to a deep-acceptor-levels with Ev+2.5 eV and/or Ev+3 eV - (0.5

C

E

## Fe-related deep-level effects 

A. Chini et al.,

“Experimental and

Numerical Correlation

Iron doping  far from

between Current-Collapse

and Fe-doping...” in

Proc.

![WaferA  higher Iron concentration in proximity of the 2DEG leads to AIGaN   1.9um GaN buffer  1019  Iron doping  3×1018  reaches  1018   2DEG     3×10   Non optimized Iron-doping process SIMSdata  UO   101  simulated  3×10   iron profile  1016  500   1000   1500   1900  depth(nm)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2b983388-c774-4215-a7d9-a89a33d64590/2b983388-c774-4215-a7d9-a89a33d64590.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=7a040a031204c26d4086849762c4d82a5c1415c0)
, 2012.

IEEE International  Reliability Physics

Symposium

Iron doping far from 2DEG

Iron doping reaches 2DEG

![WaferB  AIGaN   1.8μm GaN buffer  1019  3×1018   Iron doping  1018   far from  3×1017   2DEG   SIMSdata  1017   simulated  3×1016   iron profile  1016  detectionTimit  3×1015  500   1000   15001800  depth(nm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4fd25e6f-5f70-41dc-b128-3612517bc6e3/4fd25e6f-5f70-41dc-b128-3612517bc6e3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=9dd199e9df931434c24a433f2985141054113f1a)
![（-n-e)   Iron doping far from 2DEG  WaferB  0.9  WaferA·  paz    Iron doping reaches 2DEG  pulsed from  0.7  Vgs=VTh and Vds=40V  to Vgs=1V and Vds=5V  0.6  10n 0.1μ 1μ 10μ0.1m 1m 10m 0.1 110 100  time (s)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/84c0ec36-cfb9-453d-bd8c-bdc1470a9c95/84c0ec36-cfb9-453d-bd8c-bdc1470a9c95.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=028dc57b7b18e252856b82431bf384361ad5c9fb)
Non optimized Iron-doping process → higher Iron concentration in proximity of the 2DEG leads to higher dynamic current dispersion.

reaches

2DEG

## Fe-related deep-level effects 

![Source   Gate    = 2.0 W/mm. The  largest concentration of trapped carriers is located in the GaN buffer layer under the gate edge   Drain  0.6   toward the drain contact between 150 and 250 nm from the 2-D electron gas (2-DEG) Weconsidertheelectricfield(F)in  correspondencetothepeakinthe  ionizedFe-trapsconcentration  D,steady 1.5    = 40 V and P  appedcnarge  1.2E+17  9.6E+16  7.2E+16  4.8E+16  2.4E+16  O.OE+OO  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4924b9ea-e4ad-4f2a-99ea-caed489ba02e/4924b9ea-e4ad-4f2a-99ea-caed489ba02e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=7ed3f34a54db053aa86e9350ab71c4852777e0e4)
https://doi.org/10.1109/TED.2021.3081613

$\mathsf{V}_{\mathsf{D S,s t e a d v}}=40\;\mathsf{V} $   $\mathsf{P_{D,s t e a d y}}=2.0\;\mathsf{W/m i}$

## Fe-induced deep levels 

![Drain current transients at dissipated power but different V . No effect of electric field on  time constant = No Poole-Frenkel effect  15V  Cardwell et al. [8]   Silvestri et al. [29]   20V  10.0   Sharma et al. [11]   Chini et al. [30]   25W  30V  Horita et al.[12]   thiswork   overlapped  35W  Z.S   Bouslama et al. [28]   3   40V  a  S.O  Ea=0.52eV  2.S   0=5x10-16cm   15V to 40V  15V  peaks aligned  20V  25V  0.0   00//   30V  26   28   30   32   34   36   38   40   42   35V  40v  q/kT (eV-1)   b  1O   103   10   105   1O  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7cec1c67-e5a7-4797-ac8c-6c1c25409405/7cec1c67-e5a7-4797-ac8c-6c1c25409405.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=d662d364570c9ef765c27a812bc162cf03b3b5cb)
highly reproducible (

DS

Fe-related deep-levels

•

## Fe-related deep-levels 

from

fast (1

µ

•

s filling time is sufficient)

not affected by electric field •

https://doi.org/10.1109/TED.2021.3081613

https://doi.0rg/10.1109/TED.2021.3081613

highly reproducible (t(T) can be used for (T) can be used for  Tj evaluation, Chini et al.ESSDERC 2022) fast (1us filling time is sufficient) not affected by electric field

Drain current transients at constant dissipated power but different Vps from 15V to 40V. No effect of electric field on time constant = No Poole-Frenkel effect

τ

## Signature of traps E1 and E2 (database, 80 paper 

![18  Hacke1994  E1 (process):   Auret1998  OWang1998  18   Shmidt1999  Ea=0.82±0.06 eV   △Chung2000  Fang2000  =8.5x10-13 cm2   Amhnar2004  Osaka2005  Hogsen2005  Armstrong2006  E2 (buffer, Fe):   Umana2007  Ea=0.82±0.06 eV  Ea=0.63±0.04 eV 2 E1 (process):    cm 2  E2 (buffer, Fe):    cm  IEa=0.63±0.04 eV   RAinhat2908   Polyakov2010  7Park2010  -14  = 2.3x10-14 cm2   Arehart2010  10   -13  Arehart2011  Kamyczek2012  =8.5x10  = 2.3x10  Verzellesi2003  Okino2004  Fang2005  ,Verzellesi2009  Tapajna2010  Jho20113口  DasGupta2012  Silvestri2012  σ  σ  Caesar2012  Sasikumar2012  Bisi et al, IEEE TED 60, 3166 (2013)  Cardwell2013  Silvestri2013  Maenakgh2esso2013  32  Meneghini2013  Meneghini2014  Bisi et al, IEEE TED 60, 3166 (2013)   Meneghesso2013  Bisi2013  Thiswork  20   ③0   0   58  a/KT  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/38ff7a2c-765f-4dcb-9015-5192393ab2f8/38ff7a2c-765f-4dcb-9015-5192393ab2f8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=7c67f967433b7ddbbcb2814f13f46ccd30fe6708)
Activation  energy

|Reference|        Activation                ene      |Cross section|Cross section|        Trap                Iahel      |Growth technique|Material| Interpretation|||
|---|---|---|---|---|---|---|---|---|---|
|Arehart et al.|0.6|        Different growth                techniques (MBE,                MOCVD, HVPE) →      |MBE|n-type GaN|Point defects around dislocations|||||
|Cho et al.|0.62|        Different growth                techniques (MBE,                MOCVD, HVPE) →      |MOCVD|n-type GaN|Trap related to line defects|||||
|Cho et al.|0.5-0|        Different growth                techniques (MBE,                MOCVD, HVPE) →      ||MOCVD| n-type GaN|Pont detect, possibiy nitrogen antisite||||
|Hacke et al.|0.58|        Different growth                techniques (MBE,                MOCVD, HVPE) →      |HVPE|n-type GaN|        May correspond to the nitrogen energy                level      |||||
|Haase et al.|0.59|        Intrinsic defect of GaN,                or impurity common to                all growth techniques      |MOCVD|n-type GaN|Intrinsic point defect, e.g. N-antisite|||||
|Cho et al.|0.5-0|        Intrinsic defect of GaN,                or impurity common to                all growth techniques      |MOCVD|UID-GaN|Origin unclear, n-antisite |||||
|Chung et al.|0.60|        Intrinsic defect of GaN,                or impurity common to                all growth techniques      |MOCVD|        Undoped and In-                 doped GaN      |        Native defects or related complexes, such                 as antisites, vacancies and interstitials       |||||
|Fang et al.|0.62|        Intrinsic defect of GaN,                or impurity common to                all growth techniques      |MOCVD, MBE, HVPE |n-type GaN|        Tentatively assigned to nitrogen antisite                defect      |||||
|Hierro et al.,|0.62ev|0.62ev|0.62ev|6·10-15 cm2|6·10-15 cm2||MOCVD|UID-GaN|Possibly related to IMg-complexes in n-GaN|
|Pernot et al.,|0.6ev|0.6ev|0.6ev|8·10-16 cm2|8·10-16 cm2||MOCVD|n-type GaN|Possibly related to IMg-complexes in n-GaN|
|Wang et al.|0.578ev|0.578ev|0.578ev|||E２|MBE| n-type GaN|Point or line defect?|
|Hacke et al.|0.62ev|0.62ev|0.62ev|3.5·10-15 -2.4-10-14cm2|E2|MOCVD|         n-tye GaN with light                Mg-doping                n-type GaN      ||Point or line defect?|
| Fang et al.|0.62ev|0.62ev|0.62ev|7.4·10-15cm2|7.4·10-15cm2|B|         n-tye GaN with light                Mg-doping                n-type GaN      |RMBE||
| Fang et al.|0.62ev|0.62ev|0.62ev|7.4·10-15cm2|7.4·10-15cm2|B|         n-tye GaN with light                Mg-doping                n-type GaN      |RMBE|Also found in MOCVD and HVPE GaN layers|
| Sasikumar et al.|0.54ev|0.54ev|0.54ev|1·10-15cm2|1·10-15cm2||MOCVD|         n-polar MIS HEMTs                 with Fe-doped buffer      |        Virtual gate-related defect, nearly identical                to the 0.57 eV trap detected in GaN-polar                HEMTs      |
| Arehart et al.|0.57ev|0.57ev|0.57ev|        6-10-150                Detected also in                1-10-130     samples without Fe-                doping!! Not directly                1.5-10-15                related to the iron level                4-7-10-15                5.4·10-16 -7.2   (Rudzinski et al., phys. stat. sol. (c)                3, No.6, 2231-2236 (2006))      |HEMTs|        Found on devices from different                vendors/universities; trap related to a                common defect source, or characteristic                surface/interface state      ||||
| Silvestri et al.|0.7ev|0.7ev|0.7ev|        6-10-150                Detected also in                1-10-130     samples without Fe-                doping!! Not directly                1.5-10-15                related to the iron level                4-7-10-15                5.4·10-16 -7.2   (Rudzinski et al., phys. stat. sol. (c)                3, No.6, 2231-2236 (2006))      |1-10-130|        Fe-doped AIGaN/GaN                HEMTS      |Iron-related buffer traps|||
|Cardwell et al.|0.57ev|0.57ev|0.57ev|        6-10-150                Detected also in                1-10-130     samples without Fe-                doping!! Not directly                1.5-10-15                related to the iron level                4-7-10-15                5.4·10-16 -7.2   (Rudzinski et al., phys. stat. sol. (c)                3, No.6, 2231-2236 (2006))      |1.5-10-15|        HEMTs with Fe-                 doped buffer      |        Traps located in the buffer, whose                 concentration is influenced by Fe      |||
| Armstrong et al.|0.6ev|0.6ev|0.6ev|        6-10-150                Detected also in                1-10-130     samples without Fe-                doping!! Not directly                1.5-10-15                related to the iron level                4-7-10-15                5.4·10-16 -7.2   (Rudzinski et al., phys. stat. sol. (c)                3, No.6, 2231-2236 (2006))      |4-7-10-15|         n-type GaN with                different C content      |        Trap is not related to excess C                incorporation, may be an intrinsic defect       |||
| Soh et al.|0.59-0.63 ev|0.59-0.63 ev|0.59-0.63 ev|        6-10-150                Detected also in                1-10-130     samples without Fe-                doping!! Not directly                1.5-10-15                related to the iron level                4-7-10-15                5.4·10-16 -7.2   (Rudzinski et al., phys. stat. sol. (c)                3, No.6, 2231-2236 (2006))      |5.4·10-16 -7.2|        UID-GaN and                n-type GaN, varying                 dislocation density      |        Attributed to edge dislocations in GaN;                linear array of defects due to dangling                bonds      |||


Reference

0.6 eV 0.62 eV

4.65∙10

Arehart et al.  Cho et al.

Cho et al.

0.5-0.6 eV

Hacke et al.

0.58 eV

Haase et al.

0.598 eV

2

Cho et al.

0.5-0.6 eV

Chung et al.

0.601 eV

0.62 eV

Fang et al.

0.62 eV

Hierro et al.,

0.6 eV

Pernot et al.,

0.578 eV

Wang et al.

0.62 eV

Hacke et al.

0.62 eV

Fang et al.

Sasikumar et al.

0.54 eV

0.57 eV

Arehart et al.

0.7 eV

0.57 eV

Silvestri et al.

Cardwell et al.

0.6 eV

Armstrong et al.

0.59-0.63 eV

Soh et al.

2

Cross section

cm

-14

2∙10

– 1.71∙10

– 3.1∙10

-

-17

2.3∙10

2

2

cm  cm

-15

-16

-

6∙10

8∙10

-14

-2.4∙10

-15

3.5∙10

2

2

cm

cm

-15

-15

7.4∙10

1∙10

2

cm

-15

6∙10

2

cm

cm

-13

-15

1∙10

1.5∙10

2

cm

-15

4-7∙10

( -15

-7.2∙10

-16

5.4∙10

## Carbon compensation models 

-2.5 eV

C

G. Verzellesi et al. , IEEE El. Dev. Lett. 35, 443 (2014)

G. Verzellesi et al. , IEEE

El. Dev. Lett. 35, 443

(2014)

CN

E

![model A)   C doping modeled according to two alternative compensation mechanisms:  =0.11 eV (donors) and  model B)   (model A)   with energy E GaN:C   GaN:C  0.11 ev  EcGa (don.)   2.5eV  CGa 3.28eV   =N  N CGa \* Eac (acc.)  CN Ecn (acc.)   0.9ev  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d5c76f89-dd62-44db-9a0e-ae140cb4d022/d5c76f89-dd62-44db-9a0e-ae140cb4d022.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=efe6d63cb1dbf3b001651c49f5e02c7628b0884d)
C doping modeled according to two alternative compensation mechanisms:

1) autocompensation by Cv-Cga. states with energies EcGa=0.11 eV (donors) and Ecn=3.28 eV (acceptors) and equal concentration Ncn=NcGa (model A)

2) compensation by a dominant C-related acceptor state Cv with energy E.-2.5 e

Ga

-C

N

1) autocompensation by C

## Hot-electron trapping in C-doped buffer 

![ON-state   J. Joh and J. A. del Alamo, in IEEE  Transactions on Electron Devices, vol.  58, no. 1, pp. 132-140, Jan. 2011,  doi:10.1109/TED.2010.2087339. TP  AlGaN   \~0.74ev  TP2  Hot-electron trapping in C-doped buffer  TP2   EC  二F  GaN  Vps=0 state  0.74 ev  G  AlGaN  GaN  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d93ce2ab-cddf-4a3b-9789-01c6e8580b7f/d93ce2ab-cddf-4a3b-9789-01c6e8580b7f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=269dde35cd40c402f086b017661c0f4d80de552a)
J. Joh and J. A. del Alamo, in IEEE Transactions on Electron Devices, vol. 58, no. 1, pp. 132-140, Jan. 2011, doi:10.1109/TED.2010.2087339.

## Fe vs C simulation results 

Fe-doped

For

• •

![anhemtmsh.grd-off25pul1m_trans_dos.dat   ganhemt_msh.grd-off25pul1m_trans_des.dat  trapped electrons negatively ionized  =25V, off-state  eTrappedcnarge   eTrappedCnarge  9.0E+16   1.0E+17  7.2E+16   8.0E+16  5.4E+16   6.0E+16  3.6E+16   4.0E+16  1.8E+16  0.0E+00    buffer the negative charge corresponds to   one the negative charge corresponds to   2.0E+16  0.0E+00  DS [A]Fe-doped   [B] C-doped  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/20f9d22a-ac1d-4474-a031-9fcbb2c650de/20f9d22a-ac1d-4474-a031-9fcbb2c650de.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=6fc232d14304cea2e0ee524ae01afbde346792b1)
For the

C-doped

acceptors

For Fe-doped buffer the negative charge corresponds to trapped electrons For the C-doped one the negative charge corresponds to negatively ionized acceptors due to emission of holes.

C. De Santi et al., Proc. SPIE Vol. 12001 doi: 10.1117/12.2609666

![1③  50  D.U.T.  [12] Pernot  [5] Cho  [5] Cho  [6] Cho  [7] Cho  [7] Cho  [8] Chung  [8] Chung  45  40  12  10-1F   Iron  8   D.U.T.  Stress @ v   4.4V   =20V  40  ] Recovery @ Vgs = 0 V ,   =0V   [12]Pernot  1.05   -1  q/kT [eV  0.8 eV  1.05_≤  30 -1 ) 6   0.62 ev   V  [5]Cho  [5]Cho  1.00   1.00   q/kT (eV 5-1   [6]Cho  35 [7]Cho  VGs,interp = -2 V  0.90  0.95   0.62 eV  30  Carbon   CP17 VTH ET=0.8eV  CK02 ET=0.6  EA04 DCT ET=0.40eV  EA04 VTH ET= 0.43eV  10.90  0.95  20  112111  ③F   [8] Chung  [7]Cho  [8] Chung   De Santi  Caesar  Meneghini   Tanaka   Tapajna  CF03:E1  CF03:E3  0.85   20   25   ③0   35   45   50  0.80  0.75  Vps,meas = 3 V  Iron  25   Osaka   Huber  D.U.T.  10.80  10.75   q/kT [eV-1]   0.70  tmeas = 3 us   10 20  18  16  14  12  10 -Pre-stress  8  6 0.70  4 美0.65   20  ) 2 T τ  ln( T=RT   0.65   20  S0.60   13 12 11 10 9 ) 8 T 7  ln( 6 5 4 3 2 1  T=50°℃   0.60   Carbon  2  τ  T=75°C   18  0.55   0.55  0.50   1.05 1.00 0.95 0.90 0.85 0.80 0.75 0.70 0.65 0.60 0.55 0.50 0.45 0.40  T=100°C  T=125°C   0.50   16   De Santi  Caesar  Meneghini   0.8 ev  0.45   T=150°C  0.45   Osaka    T = 100°C   T = 125°C   T = 150°C  Tanaka  0.40    = 0 V    Pre-stress    T = 50°C   T = 75°C  1k  10.40   Huber  10u²100u²1m²10m²100m   10   100²10u100μ1m10m100m   T = RT  10   100   Tapajna  CF03:E1  100  12   CF03:E3  Fe compensation + residual C  time (s)   time (s)   CP17VTH ET=0.8eV  DS CK02 ET=0.6  10   = 0 V , V  10  37  X EA04 VTH ET= 0.43eV  EA04DCT ET=0.40eV  1  time (s) D.U.T.  GS  10m 100m Recovery @ V  20   ③0   40  q/kT (eV-1)  1m ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/eeaf6cac-f419-42e8-af66-14c61c16b6ee/eeaf6cac-f419-42e8-af66-14c61c16b6ee.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=6651cb535267948fdb386610c56446ed7848b973)
= 20 V

= - 4.4 V , V

GS

DS

Stress @ V

1.05

1.00

0.95

0.90

NFP

0.85

GS,interp

V

= -2 V

CW01 (CREE )

= 3 V

10µ

DS,00  / I DS,stress I

V

0.80

DS,meas

t

0.75

= 3 us

0.70

meas

0.65

0.60

0.55

0.45

0.50

0.40

10

100m

1

100µ

1m

10m

time (s)

100µ

10µ

100

## Dynamic I, - Vgs measurements 

D

![Stress phase  m AlGaN/GaN HEMT,  analysis in various bias conditions  150°C  Timeelapsed  0.7   Fe-doped + C contaminant SLX4CX02A2ACH4_PCM_2   1E-5S  3E-5S  Wg= 2x50 um   5E-5S  0.6  1E-4S  =0.15um  2.15E-4s  GS  =1um   4,64E-4s  0.5   µ  -0,001s  =2.85um  uun   GD   Standard 0.15   0,00215s  DS,meas  =3v   0,00464s  0.4   0.01S  =3us  meas   0.02154s  [Vgs,meas = [-4.5,0] V   0.04642s  0.3   -0.1S  CD   Stress @ (VTH-1, 20) V   0,21544s  0,46416s  0.2   -1S  -2.15443s  4,64159s  0.1   -10S  21,54434s   measurements  46,41589s  100s  0.0  -4.5 -4.0 -3.5 -3.0 -2.5 -2.0 -1.5 -1.0 -0.5 0.0  Vgs (v)  Thresholdvoltage  On-resistance  evaluationregion  evaluationregion  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/46ab5307-57fc-4361-8ca5-e696096c1e8f/46ab5307-57fc-4361-8ca5-e696096c1e8f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=69f6b163f294fbfe50c12eb43926be335502aae5)
– V

Dynamic I

Standard 0.15 μm AlGaN/GaN HEMT, Fe-doped + C contaminant

analysis in various bias conditions

GS

240

## D  260  = 280 

50

![ Unbiased recovery 10 ms stress (saturation region)  from stretched   ] -07   10 ms stress @ (VTh-1,20) V  exponential fit = =  ∗exp − B  T [K] 300 320  1000 s unbiased recovery   [10] Hierro  [12] Pernot   [8] Chung  [8] Chung  101  40 -1 q/kT [eV  exponential fit  T from stretched  (0,0) Ref. pre-stress    [5] Cho  [5] Cho  [6] Cho  [7] Cho  [7] Cho -9   Temperature   340  SLX4 CX02   0.9      y = A \* exp  A2A_CH4_PCM_14    ssas ou'sa,ysa  50°C  Lg = 0.15 um  100C  75°C   360  Iron  LGs = 1 um   0-8  LGD = 2.85 um  Wg = 2x50 um  380  T [K]  τ  Vgs,meas = -1.5 V   0.7  Vds,meas = 3 V   380   860   340   320  300   280260240  tmeas = 3 uS   30  131   00  6   13 12 11 10 9 8 7 6 5 4 3 2 1 0.6  ) 2 T τ  ln(  111  12-I   Iron   10-5   10-4   10-3   10-210-410-310-210-1  100   101   10２   103   101  10 ms stress – only Fe responds  Time (s)   Time (s)  DS,no stress /I DS I Fe traps responsible for the  1.0  0.9  0.8  0.7  0.6  3  (≥|)u  10  [10] Hierro  initial Vrh jump (t < 10 μs)   2  [12]chernot  10  [5]Cho  Ea = 0.56 ± 0,02 eV  1000 s unbiased recovery  A2A_CH4_PCM_14  = -1.5 V  1  39  132111   [6]Cho  [7]Cho  SLX4_CX02   = 0.15 um   = 2.85 um  = 2x50 um  = 3 V  10  [7]Cho  [8] Chung   = 1 um   = 3 us  [8]Chung  GS,meas   DS,meas   0  X Unbiased recovery 10 ms stress (saturation region)   10 GS  GD  G  meas  Time (s)  ③0   40   50  G L L L W V V t  −1 10  q/kT [eV-1]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c605d0c0-3623-4640-8981-5cd44a68d6e4/c605d0c0-3623-4640-8981-5cd44a68d6e4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=2a779a45d837082cae569fb8c2f7d5a360488a43)
TH

10 ms stress @ (V

-1,20) V

1.0

(0,0) Ref. pre-stress

Temperature

25 °C

0.9

DS,no stress /I DS I

50 °C

75 °C

C

100 °C

0.8

0.7

0.6

−5

10

10

10

−4

−3

Time (s)

Fe traps responsible for the

initial V

jump (t < 10 µs)

TH

E

= 0,56 ± 0,02 eV

a

−2

10

−3

10

−4

10

−2

10

TH

TH

100 s  stress @ (V

-1, 20) V

(0,0) Ref.pre-stress

1.0

0.9

Temperature

25 °C

1.1

a

100 °C

50 °C

DS,no stress /I DS I

0.7

0.8

75 °C

125 °C

0.6

150°C

0.5

0.4

−3

−4

10

−2

10

0

−1

10

10

−5

10

10

10

Time (s)

nd

Focus on 2

recovery transient

DS C traps with E slight I

= 0.9 ± 0.03 eV

40

![0 s stress @ (Vtu-1, 20) V  DCT in saturation :   measured near V  = -1,75 V  1000 s unbiased recovery   Unbiased recovery 100 s stress (saturation region)  ) 30 -1  DCT in saturation :  q/kT (eV  1-1  1-0   Ids measured near VTH  Temperature  —(0,0) Ref.pre-stress  GS,meas  Carbon  20  0.9   @ Vgs,meas = -1,75 V  25°C    De Santi  Caesar  Meneghini  SLX4C   Tanaka   Tapajna 50°C    Osaka   Huber A2A_CH4_PCM_14   0.8  75°C  @ V 100°C   LG = 0.15 μm  I DS  125°C  150°C   20  18  16  14 )  T 12 ln( 10  8 LGs = 1 μm  LGD = 2.85 μm  6  4 10  0.6  0-7  2  τ   Wg = 2x50 μm   20  Vgs,meas = -1.75 V   0.5   Carbon  DS, no stress /I DS I  18  Vds,meas = 3 V  1.1  1.0  0.9  0.8  0.7  0.6  0.5  0.4  3  tmeas = 3 μS   0_4   16  10-3   10-2   10-1   100   101   1O210-410-310-210-1  10  10°101   ¥102   103  Time (s)   A2A_CH4_PCM_14  = -1.75 V  2  Time (s)  recovery of the  10 1000 s unbiased recovery  SLX4_CX02   m  µ m µ m  = 3 V   decrease (slight VTH shift) during stress  12  100 s stress – C contribution  on 2nd recovery transient → recovery of the  µ m   = 2.85    = 2x50   s  = 0.15   µ  1 µ  = 1   GS,meas   DS,meas   = 3   10  19   De Santi  decrease (slight VTH shift) during stress   Caesar  G  GS  GD  G  meas  0  Meneghini  L  L  L  W V V  10 t  Osaka  with Ea = 0.9 ± 0.03 eV   Time (s)  40  Tanaka   000  −1  Huber  10  Tapajna  Unbiased recovery 100 s stress (saturation region)  −2 10  20   39  −3  q/kT (eV-1)  10  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fde5ace9-ff8a-44b1-956e-dbf68633d288/fde5ace9-ff8a-44b1-956e-dbf68633d288.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=18c514488bb3c6e70265139b165eaa4de765078d)
−4

10

−5

10

1

## 100 s stress - On-resistance dynamics linear region   transport 

![Measurement in   Contribution of  in the gate-drain access region 100 s stress @ (Vtu-1, 20) v  +  Recovery of (Vtu-1, 20) V stress   increases due to gate-to-drain access region traps  decreases due to thermal emission of trapped charge   /h —(O,O) Ref.pre-stress  -   contribution). Two transient: e Temperature  10   25°C   1  50°C  DS, no stress /I DS I 1.0  125°C  0.9  0.8 100 s stress – On-resistance dynamics  3  SLX4_CX02  150°C   10 0.9   A2A_CH4_PCM_14  A2A_CH4_PCM_14 0.9  I 'sa.  -1, 20) V stress  m  m = -0.3 V  2  LG = 0.15 μm  SLX4_CX02   m  µ µ  = 3 V  10  LGs = 1 μm   Isa  µ m   = 2.85    = 2x50   s  = 0.15  µ  µ  LGD = 2.85 μm   = 1   GS,meas   DS,meas   = 3   1  Wg = 2x50 μm  10 0.8   G  GS  GD  G  meas  Vgs,meas = -0.3 V   0.8  L  L  L  W V V  t 0  VDs,meas = 3 V  10 10-5   10-4   10-3   10-2   10-1   100   101   102   10-4  −1  10-3  Time (s)  1.0-２  10-1   ¥100   tmeas =3 μs  101   ¥10２   ¥103  TH  10 Time (s)   Time (s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0156c586-88cc-43e5-8306-bf06b1971195/0156c586-88cc-43e5-8306-bf06b1971195.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=3271ad8a506c9459df5af117d32bbba47387b0dd)
100 s  stress @ (V

TH

Temperature

(0,0) Ref.pre-stress

1.0

25 °C

50 °C

-1, 20) V  75 °C

100 °C

125 °C

150°C

DS,no stress

0.9

/I DS I

0.8

10

10

−2

−1

−3

10

−4

10

−5

10

10

Time (s)

@ V

DCT: I

GS

DS

R

DS

I

decreases   increases

1)

I

ON

ON

DS

2)

R

Recovery of (V  10    $\oslash\bigvee_{\tt G S}=\neg0,3\;\vee $  ON  41 −3 R 10 −4 10

−5

10

1

10

0

## On-state stress on C  acceptors 

![n2623_30V_des  1E+13  VDs=30,40,50V  8E+12  drain  6E+12  C. De Santi et al., Proc. SPIE Vol. 12001 doi: 10.1117/12.2609666  4E+12  n262350Vdes   gate  2E+12  Length[um]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b55249aa-dc2a-457a-8092-adc304d3611a/b55249aa-dc2a-457a-8092-adc304d3611a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=5f43942ee4b4a3fd946c22f34399fec23dc21270)
C. De Santi et al., Proc. SPIE Vol. 12001 doi: 1021117/12.2609666

## N 

trapping and detrapping having the same activation energy

![(i) negative charge (ionized C Front-Gating OFF-State Stress(FGOS)  acceptors) is located in the GaN buffer  in the gate-drain region, thus initially  ;   capture and recovery have similar  extremely long time constant (1s- : both involve hole re-emission,  redistribution and capture  (iii) hole emission is accelerated by  electric field due to  Poole-Frenkel ON Temp.(C):Experimental Data[7]   ExperimentalData[7]  affecting mainly R  18  140  120  16  100  80  trapping and detrapping having the same activation energy  s)  effect C-related hole redistribution effects  40   101   102   10   (ii)   3  101   100   10  tstress (s)   10  S  Ocovon  Temp.(C)   Simulations   Simulations  1.6   140  1128  80  49   102   10   100   10   407  tstress(s)   recovery  <S)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ef17c0fe-53a5-426c-b501-97554272d6aa/ef17c0fe-53a5-426c-b501-97554272d6aa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=68f025dfb60e1c07a4f9e37a7453c6be8f0b9dd8)
, V D

Stress/recovery conditions are (V

(i) negative charge (ionized CN acceptors) is located in the GaN buffer in the gate-drain region, thus initially affecting mainly Roni

(ii) capture and recovery have similar extremely long time constant (1s103s): both involve hole re-emission, redistribution and capture

(ili) hole emission is accelerated by electric field due toPoole-Frenkel effect

B

G

![ acceptor sites at the channel/buffer interface with N  SiN Passivation  1. Holes are detrapped from C  AIGaN Barrier  2-DEG   UID:GaN Channe   = 0.9 eV.  C:GaN Buffer  a E SiC Substrate  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/75230ec5-f00d-494d-85ee-d9c4cda73f61/75230ec5-f00d-494d-85ee-d9c4cda73f61.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=b5f8018232d2c1b97b8d5871a1025a771bb0f8bc)
1. Holes are detrapped from C acceptor sites at the channel/buffer interface with  $\mathsf{E_{a}}=0.9$

![ acceptor sites at the channel/buffer interface with  = 0.9 eV. They leave negative ionized   where N  2. Holes move towards gate and  SiN Passivation  buffer/nucleation layer interface .  1. Holes are detrapped from C  AIGaN Barrier   defects N 2-DEG   UID:GaN Channe  they get trapped at C acceptors  C:GaN Buffer  a E SiC Substrate  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a1708293-a8d3-4d0e-a985-dc59f619cae4/a1708293-a8d3-4d0e-a985-dc59f619cae4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=8fa18ad4e734ef441df07c897af68d9e43767f36)
1. Holes are detrapped from Cn acceptor sitesatthechannel/bufferinterfacewith  $\mathsf{E_{a}}=0.9$  E。 = 0.9 eV. They leave negative ionized acceptors

2. Holes move towards gate and buffer/nucleation layer interface where they get trapped at Cn defects.

![ acceptor N sites at the channel/buffer interface with  = 0.9 eV. They leave negative ionized  2. Holes move towards gate and   where buffer/nucleation layer interface SiN Passivation  .   3. In order to return to their original position, holes have to be detrapped from   (so same 0.9 eV  1. Holes are detrapped from C  AIGaN Barrier   defects N 2-DEG   acceptors  they get trapped at C UID:GaN Channe  C:GaN Buffer   at back interface activation energy) a  N E  OOOOOO  C SiC Substrate  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/deddfe72-c320-42d2-86fc-84930e9a5fde/deddfe72-c320-42d2-86fc-84930e9a5fde.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=682667d9d759c928ca10e9842fb28409095e1d6e)
1. Holes are detrapped from Cn acceptor sites at the channel/buffer interface with E。 = 0.9 eV. They leave negative ionized acceptors

2. Holes move towards gate and buffer/nucleationlayer interfacewhere they get trapped at C defects

3. In order to return to their original position, holes have to be detrapped from  ${\mathsf{C}}_{\mathsf{N}}$  Cn at back interface (so same 0.9 eV activationenergy)


## Short channel effects vs trapping 

![High C-doping   Medium C-doping   , vol. 15, no. 11, 2022, doi: 10.35848/1882-  Low C-doping  10  Vsfrom2Vupto20V   Vfrom2Vupto20V  Vosfrom2Vupto20V  step+1v   Step+1V  1step+1V   150mA/mm  150mA/mm   150mA/mm   100m  100m   100m  10m  1om   10m  1  n  100p  100p   100p  10u  10P   10u  DIBL=40mV/V   DIBL=150mV/V  DIBL=122mV/V  1  6   6  VGsM)   VGS(M)   VGS(M)  14  1.2  @VGS=2V   1338883389998888   @VGS=2V   0-0-8-8-3-8:0-0-0-8   @VGS=2V   0-0-0-  12   12  E0.8  夏0.6   08   0.8   Appl. Phys. Express 0.6  0.6  0.4  DC   0.4   -DC   0.4   DC  02   Pulse width=1μs  Roomtemperature  [0:0]  GateLag   0.2   Room temperature  Pulsewidth=1μs-   0:01  GateLag   0.2   /Room temperature--[0:0]  Pulse width=1μs   GateLag  Dutycycle=1%   DrainLag15V   Duty cycle=1%   DrainLag 15V   Dutycycle=1%   DrainLag15V  10   8   10   10  VDS(V)   VDs(V)   VDs(M)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f9a8611c-4e5a-475a-8d1c-211d6e1d4ff5/f9a8611c-4e5a-475a-8d1c-211d6e1d4ff5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=023c04b5f803e35e516e54c0c9987f47cc25f467)
K. Harrouche, F. Medjdoub et al.,

0786/ac9c46.

= 2

## Carbon doping and reliability very long    C-doping  

(a)

(a)

1.2

µ

L

m

G

L

G

= 2

G

200

G

V

= 0.15

On State:

W

-4

1

GS,STR

W

-4

50

DS, meas

Off-state step-stress

![a   Due to the  recovery time  constant （a）   1.2  may induce memory and charge accumulation  Even worse, hot- electron injection  LG = 0.15 μm   Pre   Lg = 0.15 μm   pre  1.0  -Wg = 2 × 50 μm   1.0  -Wg = 2×50 μm  Off State:   On State:  0.8  Vg.str = -7 V   0.8  -Vgs,str = O V  uuuu   (uuu/)   Vds, meas = 8 V  Vds,meas = 8 V   O   VdS,Str:  0.6   0.6  SO   0.4   20V  10V   SO.   O.4   O  10V  30V   20V  40   30V  0.2   0.2    =- 50   40   in 0.0   VDS,STR:   60V   0.0   50.V  DS  GS 一   -2   一一   一一   10V steps, up to 60V (V VGS(V)   VGs(V)   Step-stress : increase V (b)400  (b)400   O   Pre   Vds,str:  pre  10V  O  20V  VdS,STr:   10V  300   30V   300  20  40  (w/sw)   (ww/sw)   30V  50  40  200   60V   200  50V  uuo  100   OffState:   100   On State:  Vgs,Str = -7 V  Vgs,str = O V  Vds, meas = 8 V  8￥  meas  -2   一一  -2   一一  VGS(V)  VGS(V)    10 V 1  :  0 V Off-state step-stress   On-state step-stress  :   10 V  20 V  30 V  40 V  50 V  DS,STR  Pre  DS,STR  0 V ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d6108aae-1ee3-4a93-be3d-90e26fa35b9c/d6108aae-1ee3-4a93-be3d-90e26fa35b9c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=a67384eac6fffb450c566d1cd06887574c1867c1)
(mS/mm) m g

Pre

V

0.6

0.8

0.2

0.4

= 8 V

V

0.6

0 V

0

10 V

-5

= -7 V

V

Off State:

20 V

V

0.0

0.8

G,STR

V

-5

30 V

:

= 0.15

0.2

DS,meas

0.4

50 V

0.0

40 V  = 8 V

DS,STR

0

×

-2

0

0

-4

V

60 V

-3

(V)

GS

V

µ

m  Pre

400

0 V

-2

(b)

10 V  20 V

400

DS,STR

= -7 V

30 V  40 V

V

300

300

1.2

60 V

:

-5

50 V

(mS/mm) m g

(A/mm) DS I

1.0

200

Off State:

(A/mm) DS I

GS,STR

|         SiN Passivation|||
|---|---|---|
|AIGaN Barrier|AIGaN Barrier||
|2-DEG                UID:GaN Channel|||
||||
|C:GaN Buffer|||
|SiC Substrate|||


100

DS, meas

100

-1

1.0

(b)

-4

-5

GS -3

-1

(V)

V

Due to the very long recovery time constant C-doping may induce memory and charge accumulation

V

m

0

30 V  40 V

7V, off-state) or 50V (V on-state). 120 s stress/step followed by 300 s recovery   $\mathsf{V}_{\mathsf{D S}}$   $(\mathsf{V}_{\mathsf{G S}}=-$  without bias   $(\mathsf{V}_{\mathsf{G S}}\mathrm{{=}}\mathsf{0V},$

Even worse, hotelectron injection and trapping in the C-doped GaN buffer may lead to semi-permanent degradation

V

50 V

V

= 0 V

µ

= 8 V

m µ

(V)

50

-1

-2

Pre

= 0 V

GS

= 8 V

×

-1

On State:

GS,STR

DS, meas -3

(V)

On-state step-stress

-2

V

V -3

GS

V

## Carbon and hot-electron effects ON STATE 

stresS at Vgs=-7V, VDs =60V, OFF STATE

DS

![ =60V,  Affer Stress(VG,STR,VD,STR）=（-7,60）V  0.4  02  DS 02   =-0V, V <uun)  0.4   NCEFF(cm-3)  68+16  GS 0.6   4.0e+16  5.0e+16   stress at V 0.8  3.0e+16  x(um)  10  90 x)    (Vgs,str: Vds,str)  concentration Left, off-state (0,0) V  02   Net ionized 0.4  acceptors  0.6   (-7, 60) V  Right, on- 0.8  state a   Depth, y (μm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6abb7745-de8d-42ee-aded-323be78de764/6abb7745-de8d-42ee-aded-323be78de764.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=a152fbccbab2e56c7e7cdff13b79c52ccd1fba8b)
stress at V

Net ionized acceptors concentration Left, off-state Right, onstate

hot-electrons exit from the channel and  get trapped  N at C

=-7V, V

=60V,

![After Stress(VG,STR,VD,STR）=（0,60）V  0.2  0.1  cuun)   0.1  0.2   eDensity (cm^-3)  .0e+19  2.2e+14  03  5.6e+09  02  0.5  x(um)  1O  uuo  (Vgs,str: Vds,str):  (0, 0) V  (0, 60) V  acceptors  0.2   0.4   0.6   0.8  a   Depth, y (μm)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4f5173de-2f4d-42e9-aa6d-60a70ffcd368/4f5173de-2f4d-42e9-aa6d-60a70ffcd368.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=df1afbe1d3fa48db0966f4d778a06daf8de920c3)
stress    $\mathsf{V}_{\mathsf{G S}}\!\!=\!\!-0\mathsf{V},\,\mathsf{V}_{\mathsf{D S}}=\!\!60\mathsf{V},$  VGS   OV,VDS

OFF STATE

GS

##  decrease, but How to separate Cn from channel electrons undoped GaN  short-channel effects worsen 

![Tch.100   Tch.150   to C Tch.250   , vol. 15, no. 11, 2022, doi: 10.35848/1882-  Tch.500  101  Vosfrom2Vupto20V   Vosfrom2Vupto20V   Vnsfrom2V upto20V   Vosfrom2Vupto10V  Step+1V   150mA/mm   150mA/mm   10-1   150mA/mm   10-1   150mA/mm  10-1   aocaNcnainer  10-2   T7100-500Jmm  10-3  10-3   102   82X0   from channel electrons  104  10-6  DIBL=40mV/V   DIBL=60mV/V   DIBL=80mV/V   DIBL=355mV/V  105   cicSubstrate  103  6   6   8   -6  VGS(M)   VGS(V)   VGS(V)   VGS(M)  @VGS=2V   1@VGS=2V   1.2@VGS=2V   1.4-@VGS=2V   09:0-00-0-0-0-2-0   As a thicker (Tch)  1.2  0.8   undoped GaN  0.8   channel is adopted,  10.6   0.8  20.61    Appl. Phys. Express  trapping effectsdue  00.4   10.6  DC   DC   0.4   -DC   0.4   -DC   to Cv decrease, but  Pulsewidth=1us-GateLag  Room temperature-—[0,0]   0.2   Roomtemperature—[0.0]  Pulsewidth=1μs-GateLag   0.2  Pulsewidth=1μs  Room temperature-—-[0:0]  GateLag   0.2   /Room temperature-\*-[0:0]  Pulsewidth=1μs   GateLag   short-channel  Duty cycle=1%   DrainLag15V   Dutycycle=1%   DrainLag15V   Duty cycle=1%   DrainLag15V   Dutycycle=1%   Drain Lag15y effects worsen  0   10   10   10  VDS(M)   VDS(M)   VDS(V)   VDS(M)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7ad8acd6-bb9a-4982-ab49-3d4e8f027f72/7ad8acd6-bb9a-4982-ab49-3d4e8f027f72.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=1fb7fa988a15de038e28a045201879ac6f177625)
How to separate C

K. Harrouche, F. Medjdoub et al.,

0786/ac9c46.

N

## AlGaN backbarrier instead of Fe 

Goal: Compare the Fe doped vs AlGaN backbarrier 150 nm InAl(Ga)N/GaN HEMTs, from the point of view of short channel effects, trapping and on-wafer reliability

→ Fe doping: 0.8 μm Fe-doped (max: 2x1018 cm-3) GaN layer under the undoped GaN channel

→ AlGaN Back-barrier: AlGaN backbarrier instead of Fe doped GaN

: 0.8

\*

µ

AlGaN Back-barrier

Fe doping

![) GaN layer under the undoped GaN channel,  2ndpassivation   2ndpassivation  Gate   ICP CVD Passivation   Gate   ICP CVD Passivation  Source   : AlGaN backbarrier instead of Fe doped GaN  Drain   Source   Drain  Ino.12Alo.8Gao.0sN, Ino.18Alo.82N (6.5 nm)   Ino.12Alo.8Gao.08N, Ino.18Alo.82N (6.5 nm)  AIN Interlayer (1 nm)   AIN Interlayer (1 nm)  nid GaN (150 nm)   2DEG   nid GaN (150 nm)   2DEG  Fe doped GaN (0.8 μm)  AIGaN Back-barrier & nid GaN (1.6 μm)  nid GaN (0.8 um)  -3 AIN Nucleation (100 nm)   cm  AIN Nucleation (100 nm)  SiC substrate   SiC substrate  18 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b493a8db-8024-40c9-aa47-c7266e9dbd15/b493a8db-8024-40c9-aa47-c7266e9dbd15.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=32d94482ffd870d5d7eb22beac464c29230a105c)
\*S. Piotrowicz et al., in 2019 14th EuMIC, Sep. 2019, 41-44

## Backbarrier devices: lower current collapse 

![306  VDs = 2.5 V  256  Vgs,Q = -6 V  20   InAlGaN devices have smaller C.C. compared with InAlN devices. 156  10%  InAIN: Fe  s) V   InAIGaN: Fe  596   µ InAIN b.b  s/100  InAIGaN: b.b  1   15  µ 2O   25   3O  Vds.Q (v)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/30f15cfe-3d8a-42fd-82b3-bbddda980c1a/30f15cfe-3d8a-42fd-82b3-bbddda980c1a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=af81ada27edc24a0b9107d01bb98d84692c62874)
/ Back-barrier devices have smaller C.C. (1 μs/100 μs) V InAlGaN devices have smaller C.C. compared with InAlN devices.

https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10274766

## Dynamic Vth Transient: Fe-doped devices 

Dynamic V

TH

transients @ various temperatures - Recovery phase

V

th

V

= 10 V

= -6 V

-1.7

GS,Fill

DS,Fill

V

-1.8

-1.9

-2.0

(V) TH V

-2.1

-2.2

![-1-→  Vt, transients @ various temperatures - Recovery phase  Vgs,Fill = -6 V   InAiN: Fe    in the buffer. 10   Fe related trap  , 102, 19, 0–4, 2013. -1.8   Vds,Fill = 10 V   InAlGaN: Fe  —30°C  44 -1.9    InAlN: Fe   Silvestri  Cardwell  40°C  42 60°℃   (>s) (⊥ 2)ul   , 102, 7, 2013,  -2.0  80°C  -2.1   40 100°CH  )  K   InAIN: Fe  -2.2   -1 q/kT (eV  Appl. Phys. Lett.  InAIGaN:Fe  -2.4VDs.M=3V   38 -2.4 TFim = 1m s  -2.5   Fe related trap  36  [1,2]  Appl. Phys. Lett.  Silvestri  Cardwell  10-5 10-4 10-3 10-2 10-1 10° 101 102   32   ③4   38   ③8   40   42   44  34 Time (s)   q/kT (eV-1)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/78494c99-511e-47bf-94af-71f5d5a4b0b5/78494c99-511e-47bf-94af-71f5d5a4b0b5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=cefd841d56e7ef92c0e5ec639fc341127eeb33eb)
-2.3

= 3 V

V

DS,M

-2.4

= 1m s

2  [1] M. Silvestri  [2] D. W. Cardwell    10

T

Fill

-2.5

-4

-5

10

-2

10

10

-3

10

10

Time (s)

TH

## 32 ,  et al. 30 

The significant V

10  et al. )  ) (sK  T  ln( 2  2  τ

InAlN: Fe

30°C

40°C

60°C

80°C

100°C

1

10

0

10

-1

## Dynamic Vth Transient: Fe-doped devices 

Dynamic V

![Vth transients @ various temperatures - Recovery phase    is observed for long time constant  20   , 31, 7, 662–664, Jul. 2010.  , 68, 5, 2564–2567, 2021, -1-7   Long time constant trap: Carbon  InAIN: Fe  45  18  -1.8   -30°C  18  -1.9   Long time constant trap: Carbon  40 40°C  60°℃   S14  -2.0  80°C  -2.1   35 100°C   Z12   InAIN: Fe  )  100   InAIGaN:Fe  -2.2   -1 30 -2.3VDs.m =3V Vgs.Fmu =-6V  2.4 Tr= 100 s Vos.Fm= 10 V   InAlGaN: Fe  25  q/kT (eV  IEEE Electron Device Lett. IEEE Trans. Electron Devices Tapajna  N. Zagni  N. Zagni  -2.5    InAlN: Fe   Tapajna  N. Zagni   N. Zagni  10-510-410-310-210-1100101102  20  15   20   25   ③0   35   40   45  Time (s)   q/kT (eV-1)  15 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a6c73511-762f-4e2c-9b31-c1378c9ccab9/a6c73511-762f-4e2c-9b31-c1378c9ccab9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=d7631395d393c1e4ba24249497007d56faeed0bf)
TH

transients @ various temperatures - Recovery phase

th

V

-1.7

-1.8

-1.9

-2.0

-2.1

(V) TH V

-2.2

-2.3

= 3 V

V

V

= -6 V

GS,Fill

DS,M

-2.4

T

= 100 s

V

Fill

DS,Fill

= 10 V

-2.5

10

-2

-3

10

10

-5

-4

10

10

Time (s)

## 100 s filling time (all traps respond): 

10 20  18  16  14  12  10  8  6  4 )  ) (sK  T  ln( 2  2  τ  [1, 2]

[2] N. Zagni

InAlN: Fe

30°C

60°C

40°C

80°C

100°C

2   et al.   10  ,    1   et al.

10

10

0

-1

## Dynamic Vru Transient: backbarrier devices 

![Vth transients @ various temperatures - Recovery phase   20    signature is observed during the recovery test.  , 31, 7, 662–664, Jul. 2010.  , 68, 5, 2564–2567, 2021, -1-，   InAIGaN: b.b   InAIGaN: b.b.  18  -1.8   Tapajna  16   N. Zagni  -1.9   (zMS)  45  N. Zagni  -2.0  12  -2.1   40 VgsFiu=-6V   u   IO7  -2-3  2.2   Vds,Fill = 10 V   35  0   IEEE Electron Device Lett. IEEE Trans. Electron Devices Vds.m = 3 V  -2.4   ) Carbon  TFill = 100 s   -1 30 -2.5   q/kT (eV 10-5   10-410-310-210-1 10°101102   InAlGaN: b.b.  15   20   25   ③5   40   45  25 Time (s)   q/kT (eV-1)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/473431d4-8d72-4e97-969d-190951f888f8/473431d4-8d72-4e97-969d-190951f888f8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=17c5e5b5e131eab258656af0059a02a6d3efd025)
Dynamic V

TH

transients @ various temperatures - Recovery phase

th

V

InAlGaN: b.b

10

-1.7

-1.8

-1.9

-2.0

-2.1

= -6 V

GS,Fill

(V) TH V

V

-2.2

= 10 V

V

DS,Fill

V

-2.3

= 3 V

DS,M

-2.4

= 100 s

T

Fill

-2.5

-5

-4

-2

10

-3

10

-1

18

10

10

10

10

Time (s)

Only C related acceptor

##  Tapajna  N. Zagni   N. Zagni   20 

Carbon  15

[1] M. Tapajna

[2] N. Zagni

20

16 )

14

) (sK

2

,  10   et al. ,  12 T 10 ln( 8  6  4   et al. τ

2

1

[1,2]

10

0

## Separating Cu from 2DEG with backbarrier 

MONOLAYER

0.15 um RF AIGaN/GaN HEMTs SiC substrate (from the same batch)

Separating C

•

•

N

Aim:

•

•

Study dynamic breakdown

|C Doped Mono-layer AIGaN barrier||
|---|---|
|GaN Buffer|GaN Buffer|
|SiC Substrate                   Ca|SiC-Substrate|


## Backbarrier: 

Study DC performance and trapping effects BILAYER Study dynamic breakdown

Monolayer: C-doped AlGaN Bilayer: o Thin undoped AlGaN layer o C-doped AlGaN

0

## Electroluminescence measurements  Mono-layer 

-1  (V)

m  = 9 V  µ  V  = 1   -2 DS  GD no FP V  L -3 Electroluminescence measurements  8  7  6  5  4 10  10  10  10  10  (a.u.) D EL/I    acceptors can act as a

•

•

higher electric field

•

Hypothesis: charged C

hot electrons

![Bi-layer ¥108 Mono-layer 10７ （n-e) 10６ =9√ DS 105 GD  1um no FP 104 一一 Vgs (v) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e9d17072-1b8a-48ab-bc30-78982ea319bf/e9d17072-1b8a-48ab-bc30-78982ea319bf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=6bc7302393d97d6d24e0b5d94d77a67d78ab5c5f)
region, limiting the peak electric field

N

## Breakdown measurements 

Additional confirmation of the lower electric field in the monolayer devices

Breakdown voltage (in OFF-state) is consistently higher in monolayer devices than in bilayer ones

BILAYERDEVICESHAVEAHIGHER ELECTRICFIELD

Breakdown measurements

Additional confirmation of the lower

•

•

electric field in the monolayer devices

Breakdown voltage (in OFF-state) is

than in bilayer ones

BILAYER DEVICES HAVE A HIGHER

ELECTRIC FIELD

![220  GStres-M  2010  Mono-laver  1819   BiHlayer  1610  110   39.2V/Lm  1019  80  44.5V/jm  LGD（lm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4da06725-0e4f-4623-a3aa-ba6a91a97804/4da06725-0e4f-4623-a3aa-ba6a91a97804.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=edbe53ea1c7e3786fc61652993da2ce2b47435b6)
## Mono- and bi-layer backbarrier devices 

Improved DC performance in devices with bilayer backbarrier: in the monolayer backbarrier, C acceptors are closer to the channel → Coulombic scattering and trapping causes higher RoN

## Defects can be identified by DcTS: 

Improved DC performance in devices with

bilayer backbarrier: in the monolayer

The C level, only in monolayer devices A second level, common to both backbarrier structures, already reported in GaN

•

backbarrier, C acceptors are closer to the

Coulombic scattering and  channel

ON trapping causes higher R

Defects can be identified by DCTS:

The C

N

level, only in monolayer devices

A second level, common to both

•

backbarrier structures, already reported

in GaN

![20:0   https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9764531 Mono-layerE1:0.82eV  18.0   Mono-layerE2:0.91eV  Bi-layerE1:0.58 eV  16.0  14.0  12.0  10.0  Crelated trap (E2)  80  [9]Hogsed  8.0   [10lWang  E1Group  11iHonda  1.0  [12]Marso  2.0   [13]Umana-membreno  21   28   28   32   31   38   38  g/kT(eVil)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/731ccf71-764a-4252-af5d-a9430459a0e3/731ccf71-764a-4252-af5d-a9430459a0e3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=86cb1055d114bd5f3bdb9b1615c02aacddcf2eb3)
30

## Step-stress tests 

20

(V)

off-state

off

106%

= 1.5

L

GD

Mono-layer

(%)

104%

Bi-layer

Ref.

ON_unstressed

/ R

102%

ON_stressed

100%

V

GS,Stress

R

= -7 V

60

0

45

30

15

V

(V)

DS_stress

higher electric field in bilayer devices

Step-stress tests

![off  on-state on   = 0 V   Mono-layer  Bi-layer  Ref.  Semi on  10  V DS_stress   separation between channel electrons and C-doped layer 069/6   GS,Stress  108%   120/  Mono-layer LGD = 1.5 μm  V  (-n-e)    Mono-layer  0  Vgs,stress = 0 V  Ref.  Bi-layer.-·-·--  120%   with SFP   110% pessesun    1 06%   100% Ref.   Bi-layer   passesun   Mi-ny-layer  049/   Ref.   (%) ON_unstressed  / R ON_stressed R 1NO1   1 04%    = -2 V  40  -NOL  1 1 0%  020/   semi-on-state GS,Stress  30  passas no  Semi on   1 02   V  (V) 20 000/    Mono-layer  DS_stress   1 00   Bi-layer  1 000  GS,Stress    Ref.  10  V  -2M  GS,Stress  15  ¥30   45   80   10   20  0  ③0   40   10   20   ③0  Vds_stress (V)   Vds_stress (V)   Vds_stress (V)  104%  102%  100% ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/39a69ca9-baeb-4da2-b5f2-f9d835127678/39a69ca9-baeb-4da2-b5f2-f9d835127678.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=28280fce45a0b33392903307bfac91a26eeadbde)
(a.u.)  ON_unstressed

m

with SFP

µ

75

## Trap-related transconductance overshoot  From -7 V to 0 V  From 0 V to -7 V 

600

V

= 15 V

DS

thin

500

(mS/mm) m g

400

300

−1

200

100

From -7 V to 0 V

From 0 V to -7 V

0

−2

−1

−3

−4

(V)

V

![thick SiN   Gate  electrons are suddenly released, leading to a negative   SiN   Going from pinch-off to on-state at high Vps trapped   (V)  trapped  −2 GaNiCap   LM  electrons are suddenly released, leading to a negative  GS J AIGaN barrier   (I 2DEG  (K  threshold voltage shift   = 15 V  −3 V GaN layer (150\~250nm)  DS   >   dID   AID   dID  AINN  Sic   Going from pinch-off to on-state at high V  J  N  9m_overshoot   dVGS   dVT   dVGS  (I  (K 600  Trap-related transconductance overshoot Vds = 15 V    −  600   (m S/mm ) Vds = 15 V  m g  ６00   Vds=15V  ww/st   500  400    thin  (I J (K LM  (ww/Sw)  medium 500  400    From -7 V to 0 V medium   From 0 V to -7 V  −1  (ww/Sw）   400  500   thick  300   threshold voltage shift   =  300   −2  (V)  30O  uu o    200   F_!H&)'\$!!0  200   V GS  uu   200  100   From -7 V to 0 V  From 0 V to -7 V    = 15 V  100   From 0 V to -7 V  From -7 V to 0 V  −3  100   From0Vto  From -7 V to  DS  12  V 600  500  400  300  200 VGs（V)  100  0 −4  Vgs (v)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7976ee55-842f-4a66-85ae-8f2066a8a04b/7976ee55-842f-4a66-85ae-8f2066a8a04b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=4e84d6dc685da4b4cb4870555efcfa1ee62a48ca)
GS

E

(mS/mm) m g

## Hysteresis and transient effects due to traps 

![600  thin  (ww/sw)   450  300  -2.32V  uuo   150  Hysteresis and transient effects due to traps  10\~  VtH:Vgs@IDs= 10 μA/mm  Gate Voltage (V)  demonstrate that there is no g m overshoot going back from on-  Detrapping occurs on the «go»  -2.5  From-7Vto0V  -2.6  Hysteresis measurements  From0Vto-7V  measurement: trapping is -2.7  -2.8  -2.9  -3.0   state to pinch-off -3.1  -3.2  2   6810  Vds(V)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/392170c3-ceda-4e0a-b45b-dfec2577b91c/392170c3-ceda-4e0a-b45b-dfec2577b91c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=33136e9b963a2dec12bd36440b80e89b5b5d0ed6)
Hysteresis measurements demonstrate that there is no gm overshoot going back from onstate to pinch-off

or

Detrapping requires high V trap   ionization or photionization  trapping and short-channel

There is a trade-off between traps are at the GaN/AlN  energetic electrons trapping and short-channel effects

62

effects

![Vns: 10V 10-1 CUUUU 40-3  thick 1 0-5 medium  thim 10-9 一 VGSV) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2fae8511-599d-4c52-b226-428900a1df58/2fae8511-599d-4c52-b226-428900a1df58.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=45ac70bfd5772c38b90dc3704c6a0c9af1183d5b)
)

emission rate (s

-1

6

4

2

0

0

## Correlation with electroluminescence 

![−1   and appears to be correlated with  electroluminescence (EL) intensity. Both features have bell-shape behaviour (=  depend on a «hot-electron» effect e.g. trap impact-ionization or EL photoionization) (Vgs,b, Vds,B)  (-4 V, 7 V)   8,0×105   -BL1.3  (-3 V,7 V)  (-2.5 V, 7 V)    (V)  C  −2 （-n-e)   6,0×105  —(-2 ,7 )   GS (-1 V, 7 V)   V (-0.5 V, 7 V)   4,0×105  -10   (0V,7V)   BL1.3  −3  2,0×105  -15  0.0  (Vgs,s = -7 V, Vds,s = 15 V),  -20   −4 (Vgs,m = -0.5 V, Vds,m = 10 v)  5  5  5  5  0,0  5  -2,0×10  8,0×10  ts = 100 s  6,0×10  4,0×10  2,0×10  BL1.3  −2,0×10 1∈-4   ○,01   10:0  GS  Vgs (v)  EL Intensity (a.u.) Time (s)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/58e38690-e186-4d9c-965f-5891c8d8ca4c/58e38690-e186-4d9c-965f-5891c8d8ca4c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=421ab19a18279659314088653679b9aba30a88b6)
, V

GS,B

DS,B

)

(-4 V, 7 V)

0

(-3 V, 7 V)

(-2.5 V, 7 V)

(-2 V, 7 V)

(-0.5 V, 7 V)

(-1 V, 7 V)

(0 V, 7 V)

−5

−10

= 15 V),

−15

= -7 V, V

DS,S

(V

−20

GS,S

= -0.5 V, V

GS,M

DS,M

= 100 s

(V

S

t

−25

= 10 V)

1E−6

0,01

1E−4

Time (s)

5

(V

Emission rate (1/

Relative Drain Current Change (%)

τ

BL1.3  100  ) is not monotonic with V

1

oarre  femperafure

![WAVEFORM OSCILLOSCOPE  20× GENERATOR AMPLIFIER Ch1  Ch2  Ch1  Ch2 Currentprobe Dependence on barrier properties, voltage and temperature D.U.T 0.8  08 LG=0.1μm  AIGaNwidth 19.7nm(VGsFILL:VDs.FLL)=  AIGaNwidth 19.7nmLG=0.1μm  (VGS.FILL·VDS.ALL)=  AIGaNwidth 19.7nm  (VGS.FILL:VDS.ALL) GSlength=1μm  VDS=3V  （-5.0）V  0.7 VDS=3V  GSlength=1μm  （-5.0)V  0.7VDS=3V  （-5.0)V （-5.5)V  （-5.5）V  26.6% Al in Barrier  （-5.5)V GDlength=3um..  22.6%AlinBarrier （-510)V  90.6 24.6%AIinBarrier GDlength=3μm-  （-5.10)V  （-5.10)V TCapDrainSide=1μm  （-5.15）V  TCapDrainSide=1μm  (-5.15)V  LG=0.1μm  （-5.15）V 0:5-  ≤0.5 2FPDrainSide=Oum  (-5.20)V  2FPDrainSide=0um  （-5.20)V  GSlength=1μm  （-5,20)V .（-5.25）V  0:4  （-5.25）V  0:4  GDlength=3μm-  （-5.25)V (-5.30)V  （-5.30)V  （-5.30)V TCapDrainSide=1μm (-5.45)V  30.3  (-5.46)V  2FPDrainSide=0μm  (5.45)V （-5.45)V  （-5.45）V  （-5.45）V (-5.50)V  64（-5.50)V  (-5.50)V 0.1  0.1 082  0.0  0.0 61E-51E-40.0010.010.1  10 1001000  1E-61E-51E-40.0010.010.1  10： 1001000  1E-61E-51E-40.0010.01 0.1  101001000 time(s)  time(s)  time(s) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b57eff18-6dbe-4559-9bc1-2d5d39ed4d55/b57eff18-6dbe-4559-9bc1-2d5d39ed4d55.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=5375f6a8365655da5bc5f6ed1c3b5c3f152228bf)
## Dependence on barrier properties, voltage and temperature 

![0.7  FVds=3V   a dominant charge-trapping process E1   traps in the semiconductor material are  charged by electrons injected from the gate  metal through defects located in the AlGaN  second trap E2, whose signal is independent  (VgS,FILLVdS,FILL)  on the properties of the barrier, was also  detected. This trap is supposed to originate  from surface defects, is responsible for a  minor (\~0.1 V) threshold voltage shift and  is weakly thermally activated (0.25–0.4 eV) (-5,25) V  (-5,30) V  (MII!On 4A-()  0.6  Dependence on barrier properties, voltage and temperature  (-5,35) V  (-5,40) V  0.5  (-5,45) V  (-5,50) V  0.4  LG=0.1μm   barrier GSlength=1μm  03  GDlength=3μm  •  • TCapDrainSide=1μm  ０.２  U+   2FPDrainSide=Oum   E2  0.1 F26.6% Al in Barrier  19.7nm AlGaN Barrier  0.0   业业业  1E-6 1E-5 1E-4 0.001 0.01   0.1   10   100   1000  time(s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0c111dfe-9375-4f0c-87d1-30bc8f4bbd97/0c111dfe-9375-4f0c-87d1-30bc8f4bbd97.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=456f20e4d8ab676d77b477af7aca7d92d5307884)
a dominant charge-trapping process E1 → traps in the semiconductor material are charged by electrons injected from the gate metal through defects located in the AlGaN barrier

second trap E2, whose signal is independent on the properties of the barrier, was also detected. This trap is supposed to originate from surface defects, is responsible for a minor (\~0.1 V) threshold voltage shift and is weakly thermally activated (0.25-0.4 eV)

## How to investigate trapping transients? 

![1.10    We want the time constant spectrum  1.05   (VGM;VDM)=(0V;7V)-Dark-T=80°C  VGF;VDF)=（-6V;27V)  1.00   VGF;VDF=(-1V;27V)  VGF;VDF）=（-6V;8V)  0.95  0.90    Numerical simulations 0.85    Compact modeling 0.80    Physical modeling 0.75  13   2  log 1o(time) (s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3d3f1342-64cc-4ca6-94b2-55a577126d8a/3d3f1342-64cc-4ca6-94b2-55a577126d8a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=9d7f96d7eb090c11e5bf3513a17d425a35baafdf)
•

< 1)

•

We want the time constant spectrum    $(A_{i},\tau_{i})!$  o Physical modeling o Numerical simulations Compact modeling

Q

\*

D

B

· exp − 1   · exp − B \* :  = R  ;

\* , B

$$I(t)=I(0)\left(1+A\cdot\exp\left(-\frac{t}{\tau_{0}}\right)^{\beta}\right)$$
\* o

o

o

D B • 1  = 1 0

$$A\cdot\exp\left(-\frac{t}{\tau_{0}}\right)\stackrel{\beta}{66}=\sum_{i=1}^{k}A_{i}\cdot\exp\left(-\frac{t}{\tau_{i}}\right)$$
## Methods for time constant extraction 

## 1) Derivative method 

Peak of the derivative Does not correctly reproduce amplitude Is not analytically correct: noise, overlapping transients

1) Derivative method

•

Peak of the derivative

•

Does not correctly reproduce

amplitude

Is not analytically correct:

•

noise, overlapping transients

![1.10  0.12 （VGF；VDF）=(-6V;27V） 1.05  Dark-80°C  0.10  A (VGM:VDM)=（1V:2V） (VGM:VDM)=(0V;7V) 1.00  0.08 cne)  'ds 0.95  0.08 e2me  0016010 0.90  0.01  1 80.85  0.02 10.80  0.00 0.75  -0.02 -6-5-4-3-2-10  512 67 -6-5-4-3-2-10 log1o(time)(s)  log1o（time)(s) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/76de45fc-6a0b-4990-a2f0-e700d13deaf9/76de45fc-6a0b-4990-a2f0-e700d13deaf9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=105a2a5dacacba2cbe3fae995209fd3ea2ecf652)
[Bisi TED 60 10 2013]

## Methods for time constant extraction 

= 0.95

β

0

2) Asymptotic method

Our series is a Dirichlet series

•

•

Taylor series

•

)

-1

1/2, 2/3, 1)

## 2) Asymptotic method 

10

ν

Asymptotic  Laplace  = 0.7  = 1s  β  vs  τ 0   $\upbeta=1/3,$  4  3  ) 2 g(  1  0 Methods for time constant extraction  ν

(s

•

point integration

Not fully correct

•

It only works for a single exponential

•

![Asymptotic   β=0.95  vs Laplace  =1S  β=O.7  68  100  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b317b892-4d9c-4ed0-a8f2-6d8863267114/b317b892-4d9c-4ed0-a8f2-6d8863267114.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=40790c0ddd7742852c4d7cc76c300e63c36d0d38)
2.0

0.0

## -1    L  -2.0  log(time) 

•

every β value (≠1)

•

•

Analytically correct and complete

= 0.5)

-4.0 -6.0 0%

50%

Can be used for multiple and overlapped    The source transient can be reconstructed by  using the stretched exponential definition  (not the inverse function, independent)  β  Reconstructed from derivative  Reconstructed from   Original ( 100% Transient

Spectral Amplitude (%)

1.0

0.8

β=0.95

0.6

transients

β=0.3

suaa

![60  50  40  30  20  10  0  NO  1.0   （）   Original (β = 0.5)  4  [Modolo, Scientific Reports 2022]  60   Reconstructed from derivative  10 100   - Reconstructed from -1   0.8   f（t)   50  Atot  2 (t3=1ks, β3=0.5)   10  △O  0.6  ●(t=1,β=0.4)  Time (s)  ③0   500/  (t2=1ms, β2=0.8)   0 0.4   10 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8133b456-eeda-4329-8134-ac8bb650c53a/8133b456-eeda-4329-8134-ac8bb650c53a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=f8fa23f0444447db6ef6acd25799a263695b9c95)
0.4  •

•

Ooo

![20  0.2   0.2   =0.5) =0.4) =0.8) 2  -2 10  69  10  3  β β =1ks,   1 =1ms,  0.0   β 0.0  10-6   f(t)  Atot  10-4  =1,   10-2   100   -4  102   104  3  1  2  10 τ τ τ 10-6 10-4 10-2 10°102 10-6 10-4 10-2 10° 102    (  (  ( Time (s)  Time (s)   Time (s)   [Modolo, Scientific Reports 2022]  -6 10 1.0  0.8  0.6  0.4 89  0.2  0.0 f(t) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cf75721e-9a98-4439-ab55-4394af4640c7/cf75721e-9a98-4439-ab55-4394af4640c7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=b42f6f58e963c4397ee651cd4587dad105d50511)
-6.0

-4.0

-2.0

0.0

２.0

log(time)

## New algorithm based on inverse Laplace transform 

![10  f(t) =Z-,A·exp(-  三1  1.0   608   0.8  0.8   New algorithm based on inverse Laplace transform ft)   60   pn!dua   Atot  (t=1ks, β=0.5)   0.6  -0.6  (π=1,β=0.4)  (T2=1ms, β2=0.8)   3Q  0.4  20   0.4  02  0.0   02  G0-6   10-4   10-2   M00   102   104  Time (s)  70 10-6   10-4   10-2   100   102   104  https://doi.0rg/10.1038/s41598-022-05830-7   Time (s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6e8b9f73-2b5c-44ac-ac4e-6a53520c0578/6e8b9f73-2b5c-44ac-ac4e-6a53520c0578.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=53ec2a401f42fb8e069ad181b824c5b6bfd0139d)
## New algorithm based on inverse Laplace transform 

![g(v)=L-{f()}=L-√ex(-())  (   30°C   100  a  ¥8   90°C  100   New algorithm based on inverse Laplace transform  150°C   80  95   AO   （oo)  )osai/a)sa,   145  ( ada   10-2510-21  10-1710-13   10-9  89  α (cm²)  100  80   30C  90C   80  15   150C  71 Fitting   NO  70   2O  10-510410-310-10-1100101102  Recovery Time(s)  10-12 10-10 10-810-6 104 10-2 10°1020.10.2 0.3 0.40.5 0.60.7  t (s)   Ea (eV)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/75d4e93a-edba-42a7-b1fe-fce8967f5eaf/75d4e93a-edba-42a7-b1fe-fce8967f5eaf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=838ea56526ee6a6f92fa45a1d5e34c77f86ed571)
## New algorithm based on inverse Laplace transform 

![1.5  100   1.0  () a  a  Trapsdistribution   AlGaN   GaN   (%) 0s1/(4)s1   0.6  New algorithm based on inverse Laplace transform 92  0.0  AIGaN   GaN  0.4  88   ()     Surface   06   2DEG   Recovery Time;   100  Acceptors   EC   10us   d  80  30C   100ps:  -0.8-   EF   80  1ms  Surface Donors  90C   10ms  E(ev)   ¥4號  100ms  150C  -1S  TCAD   10S  100s  70  72 10-5 10-4 10-3 10-210-1 10° 101 102   -0.6-0.30.0   0.3   0.6  Time (s)   Vertical Direction  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6049e62d-a54e-4fe8-946d-2b2374252ac8/6049e62d-a54e-4fe8-946d-2b2374252ac8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=462e61b79789849349c4a7b45107a4dafc1510fa)
https://doi.org/10.1038/s41598-022-05830-7

## Compact modeling based on trap properties 

![Fmi  Fn   100   30C  Vin   Vout,i   ya + uepy    (%)   000420  Cn=   r  Compact modeling based on trap properties  AVth   150  00  Rni  6O  Vin   Vout,i   ③0  Cn   Cni  10-9   10-7   10-5   10-3   10-1   101   103  73  T (s)  Vtrap(t) = (01 VDG + 02(1 - exp(-03 VDG)))  Rrap   exp  tps://doi.0rg/10.1109/TED.2022.3184622   rap   rtrap  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/617d8a32-0cda-4b37-83e5-d13d794b74e5/617d8a32-0cda-4b37-83e5-d13d794b74e5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=27b5618bef6bfc09482a961bad2cc141f8d8c0c3)
## Compact modeling based on trap properties 

![0.09  GateVoltage   Measured I  0.08   OV   1   AV  0.1V   2?   5   Simulated ID  0.07   0.5V   32   6  0.06  0.05  Drain Voltage  0.04   0.1V  1V  0.03   S  10V  0.02   20v  0.01  0.00  2   6  81012  74 Drain Voltage (V)   Gate Voltage (V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d820b5a5-66ee-4ca1-af8c-2b64da4eb3f2/d820b5a5-66ee-4ca1-af8c-2b64da4eb3f2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=31960d3ab5831005778e4503530e647951521574)
![i∈ [1,n]  (Afi, EA,fi, Oc,fi), (Ari, EA,ri, Oc,ri)  Compact modeling based on trap properties  Fri  F  no  Vin   Cni=   Cni=   Vout,i  Vth,1   Vth,i = Vout,i / vi   Vth,n  AVth   >Vth,i  i=1  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/588c1bd2-ba9d-4d12-be16-0c2274095b62/588c1bd2-ba9d-4d12-be16-0c2274095b62.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=9cb70bc282af78b7ec910e724f315dc636a35144)
https://doi.org/10.1109/TED.2022.3184622

## Compact modeling based on trap properties 

Compact modeling based on trap properties

https://doi.org/10.1109/TED.2022.3184622

![10  GateVoltage  Ss   Drain Voltge  0.30  30°C  0.25   90°C  150°C  0.20  0.15  0.10  0.05  0.00   75 10-510-410-310-210-110°101   10-510-410-310-210-110°101  Filling Time (s)   Recovery Time (s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/03847e35-649f-43c3-a4fe-4f083f7f7b41/03847e35-649f-43c3-a4fe-4f083f7f7b41.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=d52c78dcaeb6730ffc3e18208dd9e548c67a35d6)
![Frequency=1Hz   D=5%   Frequency=10Hz   D=5%  0.20  Experimental  0.15  0.10  D=50%  D=50%  0.05  LL  0.00   D=95%   D=95%  Frequency=100Hz   D=5%   Frequency=1kHz   D=5%  0.20  0.15  0.10  D=50%   D=50%  0.05  0.00   D=95%   76  D=95%  0.0   0.2   0.4   0.6   0.8   1.0   0.0   0.2   0.4   0.6   0.8   1.0  Time (s)   Time (s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c9e7ee95-e5c1-43c4-b4d9-506e02fcf70f/c9e7ee95-e5c1-43c4-b4d9-506e02fcf70f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=064e0cebe347d8a3f808022d1ab1a7d0338d1d70)
https://doi.org/10.1109/TED.2022.3184622

https://doi.0rg/10.1109/TED.2022.3184622

Compact modeling based on trap properties

![103  D=5%  102  101  D=95%  100  10-1  AVTH  0.30  10-2  0.25  10-3   0.20  0.15  10-4  0.10  10-5   0.05  77 1MHz   10 kHz   100 Hz   1H吃   0.00  10-6  10-5   10-410-310-2 10-1 10°101   102   103  ton (s)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dd6cd812-aca9-4d36-806d-807b0769e847/dd6cd812-aca9-4d36-806d-807b0769e847.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=3842e893161580df99d4a652e5af9f171ea9ac5d)
## Trapping related with gate leakage current in N polardevices 

|80 nm PECVD SiNx|
|---|
|5nminsituMOcVDSiN|
|        2.6nm UID Al,Ga1.yN Cap                Y: 22%, 34%, 46%      |
|        10 nm UID GaN Channel                2DEG..      |
|0.7 nm UID AIN Interlayer|
|10 nm UID Alo.38Gao.62N Spacer|
|        20nm Si-Doped (7 x 1018 cm-3)                Graded AlGa1-xN (x: 5% ~38%)      |
|10nm Si-Doped (7 x 1018 cm-3) GaN|
|~145nm UID GaN Spacer|
|1.35 μm Fe-Doped S.1. GaN|
|~20 nm GaN Nucleation layer|
|430 μm Miscut Sapphire Substrate|


![y= 22%, 34%, 46%  T-Gate  G   25%\~75%  >(SL"   Range within 1.5IQR  Median Line  Pad   Pad   Mean  Metal   Metal   Outliers  S   LGF   SiN   DD  Source   Drain  Ohmic   Ohmic  10-5  AlGaN Cap   MBE Regrown  NIBERegrown   n/UID GaN   NN   ③  nUIDGaN   GaN Channel  Al Concentration (%)  2DEG  AIGaNBackbarrier   Isolation   25%\~75%  3096   Range within 1.5IQR  Median Line  Mlean  GaN Buffer   ea dwnis  2596   Outliers  2096  SapphireSubstrate  Trapping Voltage:  1596  (Vgs:Vds)=(-7;15)V  Off time=100μs  1096   On time=1μs  2296   3496   4696  Al Concentration  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8e3ef851-6f7a-4318-b1bf-86ada7ae8ca0/8e3ef851-6f7a-4318-b1bf-86ada7ae8ca0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=082bf6a096e0744351c41298f051a855a9c97c33)
## a 

![306   Same activation energy (E  independently from the Al%   TrappingVoltage:  By modulating the gate current,  charge injected into a single deep  Changing AlGaN composition does not alter energy and behaviour of  (VGs;VDs) = (-7; 15) V  level is modulated 25/  dnis  209  Trapping related with gate leakage current  15  Off time = 100 μs  10% On time = 1 μs   content  the trap 22   eV) 349   469  Al Concentration  12   5.5  VTH = 20 mA/mm  5.0   Alo.46Ga0.54N cap  1.0  VGS.M=3V  Vgs,stress = -5 V   4.5    = 0.5 eV 0.8  Vds,stress   4.0  0.6   from 0 V  3.5  to 20 V,   a 0.4   3.0   E step 5 V  E。 = 0.5 eV  0.2   2.5  22%AI  2.0  0.0  3233343536373839  1E-4   0.01   100  Time (s)   q/kT (eV-1)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e8d04aef-4373-47d5-9947-7662989d1de3/e8d04aef-4373-47d5-9947-7662989d1de3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=e9ea59049f0458447376fb08383f4caaa8e7ea3a)
Same activation energy (Ea =0.5   independently from theAl%   content   By modulating the gate current   charge injected into a single deep   level is modulated   Changing AlGaN composition does   not alter energy and behaviour of   the trap

## Commercial N-polar substrates (Transphorm) 

|5-8nm:in-situ SiN|
|---|
|47.5 nm: GaN Cap|
|2.6nm:TopAlGaNBarrier|
|12 nm:GaN channel              2DEG|
|10nm:AlGaNBackBarrier|
|20nm:Graded AlGaN BackBarrier|
|150 nm:GaN:UID                     N-pol|
|1.5um:GaNInsulatingBuffer|
|100nm:AIN/AlGaNBuffer|
|100-mmSubstrate(SapphireorSiC)|


D

D

![I I 0.8   0.8  T = 150°C Recipe A; Vgs.m = 0 V   T=150°C  0.7   0.7  C  0.6   cuu  0.6   Recipe B; Vgs.m = 0 V  0.5   0.5  Nostress   Nostress  0.4   0.4  0.3   V GS,stress  =-8V   0.3   GS,stress  =-8V  C  C  0.2   from0V   00.2    from 0 V  DS,stress   DS,stress  0.1   0.1  to 50 V, step 5 V   Ito 50 V, step 5 V  0.0   0.0  10   100  VDS(V)   VDS(V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4fa92125-33f8-49aa-bb3e-204a5a1419a0/4fa92125-33f8-49aa-bb3e-204a5a1419a0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=66887d249fe5e3160b45daa135cc0552908e8671)
80

two options for epi:   Recipe A and B   Under stress   I, increases in Recipe B   I, decreases in Recipe A

## I, increase in Recipe B samples : Fe detrapping 

I

increase in Recipe B samples : Fe detrapping

D

![@ Stress (t=100s)   @ Recovery (trecovery=1000s)  1.20  Recipe B  1.15  pez   50°C   Vgs,stress = -8 V  1.10   35°C  80°C  =30V  1.05   —110°℃   DS,stress  140°C  1.00  No Stress, RT  100u   1om   100   100u   1om   100  tstress (S)   二一   （S)  trecovery   12.0-   X Recipe B Device (our data)  Feinliterature:  10.0-  fCho 2001 J. Cryst. Growth  P>   8.02t20aan JAP  Cho2003JAP   Fe  4.0-  Chung 2000 JAP   E  = 0.6 eV  81 2.0  20   25   ③0   35   40   45   50  q/kT [eV-1]  81  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/98fe9d0c-7877-41fb-9206-bb932c97de26/98fe9d0c-7877-41fb-9206-bb932c97de26.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=2047c73234a3978d609b8789f909f83b13337c70)
## Conclusions 

Conclusions

of dispersion effects

• Limits of Fe and C compensation

effects

· Trade-off between control of short-channel effects and reduction • Trade-off between control of short-channel effects and reduction  • TCAD and compact modeling of deep-levels and hot-electron  of dispersioneffects  Limits of Fe and C compensatior · Use of backbarriers, buffer-free structures · Reduction of dispersion effects in N-polar devices · TCAD and compact modeling of deep-levels and hot-electron effects

## Conclusions 

reduction of dispersion effects

Trade-off between control of short-channel effects anc  reductionofdispersioneffects    Limits of Fe and C compensation   · Use of backbarriers, buffer-free structures   · TCAD and compact modeling of deep-levels and hot-electron  effects

Conclusions

•

Limits of Fe and C compensation •

•

•

effects

## FAILURE MECHANISMS OF RF GaN HEMTs 

![Electron trappingin SiN  Adapted from: Meneghesso et al., Int.  Jour. of Microwave and wireless tech.  2010 and from W. Sasangka, “Reliability  of AlGaN/GaN High Electron Mobility  Transistors”, 2018 DOI:  10.13140/RG.2.2.15242.52168 FAILURE MECHANISMS OF RF GaN HEMTs  Delaminationof  Gatemetalinterconnect  Passivation  degradation  Ohmiccontacts  Source   STN   Gaite   Drain   degradation  GaN-cap(2nm)   GaMN  Feedmetalinterconnect  AIGaN(18nm)  AIN/GaN superlattice  degradation  Sid   Gate-edge Hotelectronstrap  degradation generation  Adapted from: Meneghesso e  Jour. of Microwave and wirele  apgeneration duetoelectro-   2010 and from W. Sasangka,  Gate-edge  of AIGaN/GaN High Electron ↑  hermomechanicaldamageof  degradation  Transistors", 2018 D0l:  AIGaN/GaNsystem  10.13140/RG.2.2.15242.5216  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/de0a28ec-14d2-4ee8-b06a-0b66519543b9/de0a28ec-14d2-4ee8-b06a-0b66519543b9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=b0a231a5cb9a136eb6028c19c282c0259fd31de5)
SiC

< 20 W/mm

## m  extreme conditions 

![Sample A (Vss = 0 V. Vps = 30 V. 24h DC stress)  Substantial g decrease after 24h tests 0.35  before  0.30   after   at 0.25  uuuu   0.20  20V  0.15   > 20 W/mm 0.10-   10v  0.05   VDs from 10 V to 20 V  oxidation  Stepof5V  0.00-  -5-4-3-2-1  Vgs (v)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d11ae679-ad5c-4890-9b83-14ae1d957a0a/d11ae679-ad5c-4890-9b83-14ae1d957a0a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=0cc8e9a1f88d7dc27116d28207e295370845cd37)
![No threshold voltage shift  regions of source and   > 20 W/mm  Sample C (Ves = 0 V, VDs = 60 V, 24h DC stress)  0.35   drain  before   = 60 V 0.30    after   Substantial gm    0.25   DS  decrease after 24h tests  et  0.20-    = 0 V, V extreme conditions  O.15-  0.10:   No threshold voltage shift  Vds from 10 V  0.05-   GS  to 20 V   → damage in the access   = 30 Vafter 24h at V  Step of 5V   regions of source and  0.00-  -6-5   -4-3-2-1   drain  Vgs (v)  85 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4cea1f58-0e5f-4965-8bfb-601521205eda/4cea1f58-0e5f-4965-8bfb-601521205eda.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=2dbff9a5b4588ad9a0cc387203bfe9fd05cecda2)
after 24h at V

GS

= 0 V, V

after24h：  $\mathsf{V}_{\mathsf{G S}}=0\;\mathsf{V},\,\mathsf{V}_{\mathsf{D S}}=30 $ after24hat

DS

## Sidewall diffusion of O and Au, subsequent AlGaN oxidation and pitting 

![Oxide at interfaces  Degradation requires high T,  j and electric field = holes generated by impact- ionization play a role Sidewall diffusion of Au, O;  AlGaN oxidation and pitting DRAIN  GATE   DRAIN  Sidewall diffusion of O and Au, subsequent AlGaN GATE   and defects  Defects   pit  50nm  AlGaN degradation increases  in direction of drain  70nm   GATE  MAG:225kxHV:300kV   70nm   GATE  MAG:225kXHV:300KV  IRPS 2020  Degradation requires high T,  j and electric field = holes  Au substituted Ni   Au substituted Ni   ,   generated by impact- et al.  ionization play a role  Sidewall diffusion of Au, O;  AlGaN  AU   AIGaN oxidation and pitting  7o nm   GaN   7onm  MAG:225kX HV:300kV   MAG:225kXHV:300kV  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9a6fb21d-ceea-440f-8d26-dbbeff018a4a/9a6fb21d-ceea-440f-8d26-dbbeff018a4a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=647371c86d8ad43435d8b56c6db9d211cd99a9a8)
oxidation and pitting

## Surface erosion and crystal defects, with O accumulation 

![GATE   Pitting is frequently found slightly beyond gate edges: oxygen diffusion continues on the device surface  Possible nucleation of  the electrochemical reaction at defects,  dislocations SiN  AlGaN  Surface erosion and crystal defects, with O accumulation GaN   Heavy pitting and  crystal defects  20nm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6d757b58-40b1-4f1b-8cd8-5bccf21c604d/6d757b58-40b1-4f1b-8cd8-5bccf21c604d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=76ba19b9ffa73720cedee5f3bc7638a5ed76fbb6)
TEM image of defect at the gate-drain access region and EDX map of oxygen, after 24h DC test at Vgs = 1 V, Vps = 38 V, DC P, = 31 W/mm

DS

at V

GS

= 1 V, V

= 38 V, DC P

D

Pitting is frequently   found slightly beyond   gate edges:   oxygen diffusion   continues   on the device surface

Possible nucleation of the electrochemical reaction at defects, dislocations

Thermal Storage Tests

5

![200°C  275°C  24 300°C  )  hs   = 1.8 eV 325°C  -1 T (eV 6    10  22 10  ×  b SSC  -1５  1.87  A  20 q/k E -20  -25  7  6  5  4  3  2  1  0 10  10  10  10  10  10  10  10  Time to Failure (h) 1000   2000  (b) （a>   Time (h)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0392b386-66e7-475e-b1e3-2feb7a655e72/0392b386-66e7-475e-b1e3-2feb7a655e72.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=b8e810098a8b57c67c9ed39d3548c2beb5b7f298)
(%) DSS I

0 -5

-10 ∆

-15

-20

26

-25

0

$\Delta I_{D S S}=-0.1+1.0~e x p(-(x/9.6e8)^{0.36})$  ;

1000

(a)

Time (h)

2000

275

°

C:

= −Z. \  \. Z ^_\`:−:_/b. c^d;

∆W

XYY

[1-3]

Failure Criteria:

A

: 1.8 eV

degradation.

10% I

DSS

Estimated TTF @ 200°C: > 200 years

![10  106   1.87x106 hs  105   200°C  Q4  10  euu  102  101   Ea = 1.8 eV  10０  20   22   24   26  （D>   q/k,T (eV-1)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a34560e3-3efb-4b28-80cd-48d2c4461202/a34560e3-3efb-4b28-80cd-48d2c4461202.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=e56e4fa9037fc3f1abe1247e0b281b8890d91b8b)
275°C

325°C

300°C

88

Thermal Storage Tests

5

![200°C  275°C  24 300°C  )  hs   = 1.8 eV 325°C  -1 T (eV 6    10  22 10  ×  b SSC  -1５  1.87  A  20 q/k E -20  -25  7  6  5  4  3  2  1  0 10  10  10  10  10  10  10  10  Time to Failure (h) 1000   2000  (b) （a>   Time (h)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2078a467-c187-4494-925d-787906df92a2/2078a467-c187-4494-925d-787906df92a2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=da3b4793fc597be43d675826aaf9b27ef3c49f96)
(%) DSS I

0 -5

-10 ∆

-15

-20

26

-25

0

$\Delta I_{D S S}=-0.1+1.0~e x p(-(x/9.6e8)^{0.36})$  ;

1000

(a)

Time (h)

2000

275

°

C:

= −Z. \  \. Z ^_\`:−:_/b. c^d;

∆W

XYY

[1-3]

Failure Criteria:

A

: 1.8 eV

degradation.

10% I

DSS

Estimated TTF @ 200°C: > 200 years

![10  106   1.87x106 hs  105   200°C  Q4  10  euu  102  101   Ea = 1.8 eV  10０  20   22   24   26  （D>   q/k,T (eV-1)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/192fb665-0d91-4a5d-a55a-442e93e2ea36/192fb665-0d91-4a5d-a55a-442e93e2ea36.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=49c81dcc76c605c38474a806cfa50ed9d2402a70)
275°C

325°C

300°C

89

Thermal Storage Tests

5

![200°C  275°C  24 300°C  )  hs   = 1.8 eV 325°C  -1 T (eV 6    10  22 10  ×  b SSC  -1５  1.87  A  20 q/k E -20  -25  7  6  5  4  3  2  1  0 10  10  10  10  10  10  10  10  Time to Failure (h) 1000   2000  (b) （a>   Time (h)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8102625f-715a-4c19-af80-46ba87a7ec8d/8102625f-715a-4c19-af80-46ba87a7ec8d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=050c7ffd2e4bc501c807e3d4a1dc711e48a34168)
(%) DSS I

0 -5

-10 ∆

-15

-20

26

-25

0

$\Delta I_{D S S}=-0.1+1.0~e x p(-(x/9.6e8)^{0.36})$  ;

1000

(a)

Time (h)

2000

275

°

C:

= −Z. \  \. Z ^_\`:−:_/b. c^d;

∆W

XYY

[1-3]

Failure Criteria:

A

: 1.8 eV

degradation.

10% I

DSS

Estimated TTF @ 200°C: > 200 years

![10  106   1.87x106 hs  105   200°C  Q4  10  euu  102  101   Ea = 1.8 eV  10０  20   22   24   26  （D>   q/k,T (eV-1)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ebe3aac1-1d1e-4095-aea0-b6d3656b079d/ebe3aac1-1d1e-4095-aea0-b6d3656b079d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=81bd6987d1f0890471f77b4232a5fd2041ab02c7)
275°C

325°C

300°C

90

## Thermal  Storage  Tests 

![Integrated Intensities (a.u.)  , and NixAuy and Ni-Pt and Ni-Au alloys;   decrease [1]. IntegratedIntensities(a.u.)  2000   4000  400   800  AUM   Gate  Gate   s Ni/Au/Pt   AUL  Au/Ni/Pt  SiNx  PtN   100  SiNx   SO  Metal/epiinterdiffusion  AIGaN   Alk(x3)   Gal   AIGaN   SAlK(xS)  NK(x4)  sa  Nk{x4)  50nm   200   50nm   Position(nm)  GaN   GaN  After2000hoursstoragetest@325°℃  Position(nm)  Freshdevice  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/eeac781e-09d8-4195-99cd-31f8f128bff8/eeac781e-09d8-4195-99cd-31f8f128bff8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=aa6f180507e0cc6a2c69b7d8ffc5ab48821345e1)
Thermal Storage Tests

Ni/Au/Pt interdiffusion:

Ni/Au/Ptinterdiffusion:

3

Pt, NiPt 3  91   ${\boldsymbol{\mathsf{n}}}_{\mathsf{s}}$

## Thermal Storage Tests 

![Degraded   Interdiffusion of Schottky metal into expitaxial layers created cracks and pits, possibly   due to the thermal expansion coefficient difference of GaN, AlGaN and SiN [1]  Reference  interdiffusionand  gate sinking  vertical crack  50   mm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e6c5fb0c-e315-4a5e-9c64-b5d0a73e7c40/e6c5fb0c-e315-4a5e-9c64-b5d0a73e7c40.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=56bf9488e260d7c6117aa376769b7e265804ca11)
rtical cracks at the gate corner of the device

Thermal Storage Tests

92

High Temperature Operating Life Tests (HTOL)

![-20  4O  SSO  -6O   C leads   hs 210°C  5 225°℃   10 -80   ° × 250°C  Operating at 200 10-1   10°  101  102  103  to MTTF > 1.37  （a>   Time (h)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fbb44a31-ce1e-4d95-8bf0-ee01eec73fe7/fbb44a31-ce1e-4d95-8bf0-ee01eec73fe7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=28aa615e07fbc3dd77d79d4c74c3af50d3c230da)
0

-20

(%) DSS I

-40

-60

∆

210°C

= 1.0 eV

225°C

-80

250°C

a

E

26

24

23

25 -1

10

-1

0

1

2

10

10

10

degradation.

eV

3

10

)

(

T

b

q/k

(a)

Time (h)

Failure Criteria:

![ and Estimated TTF @ 200°C: > 15.6 years: 10６  Different failure mechanism compared with storage tests. Operating at 200°C leads  () s l    rto MTTF > 1.37 × 105 hs  104  102  E。 = 1.0 eV  10０  21   22   23.24   25   28  q/k,T (eV-1)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/06f14389-a461-42e6-b775-1af868556dbb/06f14389-a461-42e6-b775-1af868556dbb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=7ccc9d854f99156112f7ccab2c7b3cd570b0f061)
21 0 10 93 (b)  [1]

20% I

DSS

6  4  2 10  10  10 ) h (   Time to Failure

: 1.0 eV

A

E

=

High Temperature Operating Life Tests (HTOL)  = 30 V, T

![Bright field STEM image of the cross- section of GaN HEMTs after 2000 h at   DS 225°C, and 970 h at Tj = 250°C Pits affecting the  AlGaN at the gate   = 100 mA/mm, V edge towards the  drain side  20nm  DS Oxygen at the Pt/AlGaN  I AIGaN  interface and within the   surface  pits, extending into the  AIGaN layer.   oxygen EDX map  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/badee1c3-a337-4ef0-8f40-d858ff397580/badee1c3-a337-4ef0-8f40-d858ff397580.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=5733ffb5c2c12e14720126a626a0ce7733d92dc8)
Pits affecting the

AlGaN at the gate

edge towards the

drain side

Oxygen at the Pt/AlGaN

interface and within the

pits, extending into the

AlGaN layer.

Pits and cracks at the gate edge on the drain side:

94

12

7

9

6

5

5

5

## 1.5x10  2.4x10  1.1x10 2.0x10 2.0x10 1.3x10  2.6x10 Thermally-Activated mechanisms: Arrhenius-based reliability evaluation 

Failure

criterion

30

25

E

a

20

E

=2.15 eV

a

15

ln (TTF)

=1.94 eV

E

a

10

a

![25   Thermally-Activated mechanisms: Arrhenius-based reliability   Test DC thermal  storage thermal  0.50um DC  storage RF RF  RF thermal E,=2.24 eV   0.50jum storage  20   0.50μum storage  0.25um storage  (LL)   15   E.=2.15 eV   Ea (eV) Technology µ m  µ m  0.25μm RF  0.50um RF  µ m µ m µ m  µ m Ea=1.94 ev  0.5   0.5   0.25um RF  0.5  0.5  0.25   0.25  10  E.=1.92 eV  E.=1.82 eV  E,=1.40 ev  evaluation E。=2.12 eV   2.24   2.15  1.94 1.92 1.40  1.82 18   19   20   21   22   23   24   25  25 g/kT (eV-l)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b7a3de93-4414-404d-91f8-75e158a65569/b7a3de93-4414-404d-91f8-75e158a65569.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=6ffc361b7aa86e4dfe0904d776a9b9e8231efb19)
a

GH50 DC (UNIPD)  GH50 storage (UNIPD)  GH50 storage (UNIPD)  GH25 storage (UNIPD)  GH50 RF (GT)  GH50 DC (GT)  GH25 RF (GT)  24

=1.92 eV

E

=1.82 eV

a

E

a

=1.40 eV

E

5

=2.12 eV

E

IG-10x

0

19

18

21

20

IG-10x

the 1.8 eV – 2.25 eV interval

||||        Failure                criterion      |        TTF                (hours)      |
|---|---|---|---|---|
|Ea (eV)Technology|Ea (eV)Technology|Test|        Failure                criterion      |        TTF                (hours)      |
|2.24|0.5m|DO|IDS-20%|1.5x1012|
||0.5um|thermal|||
|2.15|0.5um|        storage                thermal      |IDS-20%|2.4x107|
|1.94|0.5um|storage|IDS-1 0%|1.1x109|
|1.92|0.5um|RF|-1dB power|2.0x106|
|1.40|0.25 um|RF|-1dB power|2.0x105|
|1.82|0.25μum|        RF                thermal      |IG-10x|1.3x105|
|２.1２|0.25um||IG-10x|2.6x105|
|||storage|||


=2.24 eV

23

)

22

-1

q/kT (eV

Thermal Storage Tests

5

![200°C  275°C  24 300°C  )  hs   = 1.8 eV 325°C  -1 T (eV 6    10  22 10  ×  b SSO  -1５  1.87  A  20 q/k E -20  -25  7  6  5  4  3  2  1  0 10  10  10  10  10  10  10  10  Time to Failure (h) 1000   2000  (b) （a>   Time (h)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7123f489-fac2-466b-bb3a-72f1dc6f31df/7123f489-fac2-466b-bb3a-72f1dc6f31df.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=f2d4562e3b07e8467b9b302b289c715cad69d92c)
(%) DSS I

0

-5

-10

∆

-15

-20

26

-25

0

$\Delta I_{D S S}=-0.1+1.0~e x p(-(x/9.6e8)^{0.36})$  ;

1000

(a)

Time (h)

2000

275

°

C:

= −Z. \  \. Z ^_\`:−:_/b. c^d;

∆W

XYY

[1-3]

Failure Criteria:

A

: 1.8 eV

degradation.

10% I

DSS

Estimated TTF @ 200°C: > 200 years

![10  106   1.87x106 hs  105   200°C  Q4  10  euu  102  101   Ea = 1.8 eV  10０  20   22   24   26  （D>   q/k,T (eV-1)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0dd8c913-8cfa-4d05-8fc6-c1456d57f9c0/0dd8c913-8cfa-4d05-8fc6-c1456d57f9c0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=cff02fd9c6e3043c87fac529434aeb1769ffe64b)
275°C

325°C

300°C

96

