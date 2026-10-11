---
title: "IPFA2022_Kuball_Tutorial_V1.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_ed041e1392b8e0c743584ee8ad651d8d7295230462135641
file_size: 6469478
---

## Advanced thermal characterization of GaN devices, from  micro to nanoscale, and new heat sinking solutions 

## Professor Martin Kuball\* 

Royal Academy of Engineering Chair in Emerging Technologies Center for Device Thermography and Reliability, University of Bristol, UK

![Keep Out  Keep Out  Video Zone Video Zone  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b01710a5-5a7b-4d92-ba57-7111c77b695f/b01710a5-5a7b-4d92-ba57-7111c77b695f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=cd704fa8aef65775280aab5c03d27829b3214f38)
## Outline 

Background – Why thermal analysis is needed     Limitations of thermal (and electrical) simulations     Thermal analysis of semiconductor devices – Raman thermography, HQTI,   Thermal AFM      Thermal conductivity measurement of materials including of semiconductor   epi and substrate, die attach, packaging – TTR, FTDR     Probing electric field distribution in devices - EFISHG     Application examples     Discussions and Questions

Keep Out  Video Zone

## Todays’ challenges …  more compact, higher power &  higher efficiency 

Power consumption is a challenge for computing (AI, big data) and  communication technologies.  New hardware is needed.

![Junctiontemperature  256°C225C   175°C  1E48  1E47  1E+6  1E+S  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/67b373f3-b64e-45e0-89ed-08d7050c5fb9/67b373f3-b64e-45e0-89ed-08d7050c5fb9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=26907aee6693232a89f00d559d6c2a537290769b)
Computing

https://www.sciencealert.com/computers-will-require

more-energy-than-the-world-generates-by-2040

Keeping electronics cool is key to meeting these challenges…

![Keep Out  Keep Out  Video Zone Video Zone  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/18d2af8a-d2f3-46d3-b525-1fcfc60ed1ed/18d2af8a-d2f3-46d3-b525-1fcfc60ed1ed.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=6a62e36972c0965953ebfafec544453a37aab14f)
## Examples of “hot spots” in devices 

![Different transistor  Different transistor  materials:  materials: 110  110   GaN-on-di GaN-on-di   GaN-on-di (no metal) GaN-on-di (no metal)   GaAs GaAs  100 100   GaAs (no metal) GaAs (no metal)   Si Si  C] [Oo1   90  90   Si (no metal) Si (no metal)  o Temperature [  80  80  Dielectric  Line  gate  profilel  70 NO   Epitaxy heat  Substrate   1mm  80  60  source gate  drain ee  50  50  heat  heat -1  0  1  2  3  4  5  6  7  8 Position [microns]  Position  [microns] ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7af3d7d8-f78b-4db6-a7a5-f059f53e943c/7af3d7d8-f78b-4db6-a7a5-f059f53e943c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=bd173200be5c4e45df49ae4e4ad10a122717ea65)
Hot spots are often very local -

submicron size

![Temperature  Temperature  Heat flow  Heat flow source nos    Pdiss=1.28W/mm  P diss =1.28W/mm  Drain GaAs saeo    gate]  gate  dielectric  dielectric T.[°C]  T. [°C]  Heat flux [x109 W/m2]  Heat flux [×10 9   W/m 2 ] 45  45  100  100 0  11.6  1.6 Pdiss=2.86W/mm  P diss =2.86W/mm Silicon T.[°C]  T. [°C]  Heat flux [x109 w/m2]  Heat flux [×10 9   W/m 2 ] 45  45  100  100  0  13  13 GaN-on-di !p-uo-ne   Pdiss=11.2W/mm  P diss =11.2W/mm Keep Out  Keep Out  T.[°C]  T. [°C]  Heat flux [x109 W/m2]  Heat flux [×10 9   W/m 2 ]  Video Zone  Video Zone 45 45   100  100  0  13  13 4 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6420845c-30ad-4908-97c2-1515c560d1b4/6420845c-30ad-4908-97c2-1515c560d1b4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=b7c0465714b44067441063e4f258dd7830b036b6)
## Device temperature – What needs to be considered ? 

![Local heat source Local heat source  Jouleheat  FP  Passivation  AlGaN  GaN   Heat flow 0.5um  TBReff  siC  Die attach  Die attach  Package baseplate  Package baseplate ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5a40d1fb-b394-4894-8907-228dc7461e25/5a40d1fb-b394-4894-8907-228dc7461e25.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=c5b89ab4a3066ed87a85f3556d5c3bcbad484872)
## Thermal conductivity 

•  Device epilayer   •  Substrate epilayer   •  Die attach   •  Package baseplate

Thermal boundary  resistance  between  different materials

![Keep Out  Keep Out  Video Zone  Video Zone ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/975b95ce-dc38-4d4c-9dc8-49b0e85d167c/975b95ce-dc38-4d4c-9dc8-49b0e85d167c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=40724a3a5939d9371f67980efd4f9ebe39cd0103)
## How  ‘was’  temperature determined ? 

![Infra-Red (IR) Thermography  Infra-Red (IR) Thermography ()    5000K   Planck's law  Planck’s law 62,0\*C  60.0  4000K  55,0  3000K  50.0  0.5   25  Wavelength (um)  From wiki  From wiki  45.0  40.0  35,0  30.0  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9a30aea3-0a05-4d22-90d7-c05929b5bfab/9a30aea3-0a05-4d22-90d7-c05929b5bfab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=99d759eaf8a1ed97216716c8a97fc65b2ff1adf8)
Keep Out  Video Zone

Measures intensity of IR light emitted from, e.g., semiconductor device

## What spatial resolution is achievable with IR? 

![The Rayleigh Criterion  Airy Disk 1   Airy Disk2  Figure 4  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9af9218c-d0de-4c5d-89e1-8aeaf08b81b4/9af9218c-d0de-4c5d-89e1-8aeaf08b81b4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=bc7e84ed6fcd107bfe951993863db59b76fe3b65)
https://www.zeiss.com/microscopy/int/solutions/reference/ basic-microscopy/numerical-aperture-and-resolution.html

![IR thermography  IR thermography 入 range  λ range 1200K  Wieh law  1000K  BOO  Wavelength (um)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/759544ba-8050-4f24-a835-746d0072baee/759544ba-8050-4f24-a835-746d0072baee.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=a6372d74790ab3828acc28679e68cda62e2f6c33)
Resolution =  0.6ȉ𝜆𝜆 𝑁𝑁𝑁𝑁

where NA is the  numerical aperture of  the objective lens

Realistically one can achieve a  spatial resolution of maybe 3 µm  which  is not enough for much of todays’ technology.

![Keep Out  Keep Out  Video Zone  Video Zone ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a117baae-ac68-4e45-911a-4de6e0a66af7/a117baae-ac68-4e45-911a-4de6e0a66af7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=0563063a81afc1744515d2eda265cd1dc38537d3)
## Alternatives – Why not use simulation alone? 

There are plenty of thermal  simulation tools available!

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/655ec66c-943f-4dce-9729-87a61db91b9f/655ec66c-943f-4dce-9729-87a61db91b9f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=397542fa39fbbe27a09e8b44e4ffb459499bc3fd)
https://www.ansys.com/products/electronics/ansys-icepak

Accurate  inputs  are  needed  for semiconductor device thermal simulations. But,  there  are  uncertainties  in  many parameters: interfaces, microstructure, size effects, all need to be considered.

Example: Thermal Boundary Resistance (TBR), e.g.,  ZnO/GaN interface.  Different models give different values…

![2000  ZnO/HQ/ZnO  (PRB 93,115310)  (WMW)   ≤=1  E(AGF)   =1.  1000  (isotropic)  800  600  400  AGF  DMM  200  ZnO/GaN  100  100   600  Temperature (K)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/54760833-145d-4f5c-8aae-ce9004e2e5dd/54760833-145d-4f5c-8aae-ce9004e2e5dd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=4a52e2cd4bf6ed4ad3d8e3c02464826b958c8045)
J.T. Gaskins et al., Nano  Lett., vol. 18, pp. 7469 – 7477, November 2018.

![Keep Out  Keep Out  Video Zone  Video Zone ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6a86729c-7f0e-4cb3-8150-90dee1887b3f/6a86729c-7f0e-4cb3-8150-90dee1887b3f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=2aa6e55edba5471f41ebfef53bbdbe6c17546e32)
## Raman Thermography  temperature measurement 

![35000  Pinch-off  30000   Increase ofP,T   P  P2  (n'e) suno   25000   P3  20000   GaNE2high  15000  GaNA1(LO)  10000  5000  550   600   650   700   750  Raman shift(cm-1)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e5e12bf0-0262-4255-b241-71c97da3313d/e5e12bf0-0262-4255-b241-71c97da3313d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=6f3ba3be6f85bfa88ea1119c9bc7bf19bbc4d016)
Temperature measurement with  submicron spatial and 10ns time resolution  possible (e.g. 532 nm laser is used to  generate this spectrum)

![Phonons =  Phonons =  vibration of  vibration of  atoms in crystal  atoms in crystal  lattice lattice      off  on  Temperature  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/aa7b22fb-4ba3-4526-aded-6b80af3ca3d4/aa7b22fb-4ba3-4526-aded-6b80af3ca3d4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=7a35bc02e63d1725385ac4f7475ebc0bf4705c74)
M. Kuball, Surf. Interface Anal.  3 1, 987  (2001); M. Kuball and J.W. Pomeroy, IEEE  Trans. Dev Mat. Rel.  16 , 684 (2016).

Keep Out  Video Zone

## How is the measurement done ? 

![140  Source   Gate   Drain  120  100  <0Q)  89  60   400ns  40   200ns  20  200ns  83  Position (um)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/02b7d3cc-feb4-4219-95cd-193f35eaf2a9/02b7d3cc-feb4-4219-95cd-193f35eaf2a9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=16e20e1129cf9a49735a35f7d65af6a5bc940fd9)
Serial point-by-point measurement

![Dhjectivo   Raman  Iems   scattering  SFP   Laser light  Gat4  S心ur心e   Passivation   crain  Earnier  GaN channel  Su bstrate  Oblectlve   Raman  Icns   scaterna  Laser llght  +: Nanoparticle  SFP  Gate  Sa4nce   Pabsivation   crain  Barrier  GaN channel  Substrate  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/16b9f22c-3847-47ae-84e3-c9503c64c7a9/16b9f22c-3847-47ae-84e3-c9503c64c7a9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=a3b46ddf7a1e77584ec932721a255ee8949ca980)
Keep Out  Video Zone

## How is the measurement done ? 

![Light  140  Source   Gate   Drain  0.5NA  Objective  120  Drain  AGar  100  -8umD.o  <0Q)   sic  80  Heatspreader  80   4000  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8c33f760-f6ca-48a8-8b1d-b3ed4dd17a05/8c33f760-f6ca-48a8-8b1d-b3ed4dd17a05.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=b1e7a0e0ff3f8d7c54e599d9f4a7197f704e7622)
40

200

![2001S  GaNarea  SiC Area  20  Heatsin  ObjeNive   Keep Out  Keep Out  Serial point-by-point measurement  Video Zone  Video Zone Light  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1b7a4a6e-ab6c-4476-8613-6c7f7e737493/1b7a4a6e-ab6c-4476-8613-6c7f7e737493.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=f076e3d238cd4025f2bb21ddb25183b408ba231c)
## Spatial resolution in Raman thermography 

Resolution  is determined by 3D point spread function at the laser focus:

![Lateral  Lateral Axial  Axial ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e55782ab-4735-490c-8460-5258f132f160/e55782ab-4735-490c-8460-5258f132f160.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=35da3c1524003c0ba3029e1a81bb0fa4d61847ff)
http://zeiss-campus.magnet.fsu.edu/referencelibrary/  pdfs/ZeissConfocalPrinciples.pdf

$$\begin{array}{r l}{F W H M_{i I I,l a t e r a I}\,{=}\,0.51\,\frac{\uplambda_{\mathrm{exc}}}{N A}}\\ {F W H M_{i I I,a x i a I}\,\approx\frac{1.67\cdot n\cdot\uplambda_{\mathrm{exc}}}{N A^{2}}}\end{array}$$
Typical values at 532nm are: •  FWHM _lateral  = 0.5 µm •  FWHM _axial  = 5-8 µm

nm-scale resolution can be  achieved by increasing NA…

Keep Out  Video Zone

## Comparison Raman vs IR thermography 

![160 1 60   gate   Raman Raman.  C] Oo1    IR IFR  o Temperature [ 120 120   source source   drain  drain   3D sim 3D sim.  . 88  80 -10  -10  -5  0  5  10 10  13 13  Position  Position [um]  [ µ m ] ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bb93f106-f1dc-45c9-ade8-888207720b52/bb93f106-f1dc-45c9-ade8-888207720b52.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=ca4b4ce69a965ede8d64ef41e1984565fae54f7e)
IR averages laterally over a few µm as well  as vertically through the semiconductor  layers (in most cases).

M. Kuball et al., CSICS 2007

Keep Out  Video Zone

## Also often used – Thermoreflectance (TR) 

Measure temperature induced reflectivity change, though  we find this technique not that accurate / reliable for

complex structures.

A. Ziabari et. al,  Nature Comm. Vol. 9 , no:  255  ( 2018 )

![min.  0.0  550   600   650   700   750   800  Wavelength (nm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/901cc11f-d1d9-448d-8f3c-8b8f813d3e0d/901cc11f-d1d9-448d-8f3c-8b8f813d3e0d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=ec45c3a4143d3db39572d32da58939acf6955569)
Comparison of TR vs Raman on industry processed GaN wafers:

![180  160  140  120  100  40  20-  10  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3a0db502-0236-4959-86b1-2cc7256c5b17/3a0db502-0236-4959-86b1-2cc7256c5b17.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=ca01c65d71d7354483e24c5863a3e052de2dfb40)
![140  120  100  60  14  14  Raman Thermoreflectance  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c1472211-8925-4ca0-964e-f6f2062302c4/c1472211-8925-4ca0-964e-f6f2062302c4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=dc6f73d126ef93e6d5f39c47ae3050bbca581f74)
![Keep Out  Keep Out  Video Zone  Video Zone ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fbf52457-420c-4a7b-97d4-58077e5d9735/fbf52457-420c-4a7b-97d4-58077e5d9735.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=48f72b2422f858f672576b520494be0a700fc0a8)
## Applications of Raman thermography 

![250 8x250um 200 150 uua  4x250μm Powerdensity[W/mm] 100 35-40 口30-35 □25-30 口20-25 uun  口15-20 口10-15 口5-10 26 50  80  100  150  250  500 Fingerwidth(μm) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a7b45be2-12f8-4849-b13e-3b3ff993d1d4/a7b45be2-12f8-4849-b13e-3b3ff993d1d4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=a787509be541b836672183dbecd345f9f847f96e)
![Thermal  HEMT thermal  Substrate Material   conductivity  resistance [°C mm/W]  @25°C [W/mK]  Sapphire   3   Schottky  ImmplantMesa  GaN Capo  Silicon   130   lsolabion  SiC   ４２０   AIGaN Barrier  Polycrystalline   2DEG  1200'   10   -GaH Channel  diamond  AIGaN Buffer  M Kuball et al, IEEE Trans. Dev. Mat Rel. 16, 667 (2016) M Kuball et al, IEEE Trans. Dev. Mat Rel. 16, 667 (2016)   Nucleation Layers  T. Boles, AIP Conference  T. Boles, AIP Conference  Jouleheat   Proceedings1934,020001  Proceedings 1934, 020001   High Resistivity  (2018)  (2018)  Silicon Substrate  S  AIGaN  GaN   Keep Out  Keep Out  0.sum   Video Zone  Video Zone TBRefr  siC  15  15 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/40ee057c-1e98-4ad6-9b77-b14a5d01bdf8/40ee057c-1e98-4ad6-9b77-b14a5d01bdf8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=53d3f004e260bdbe65d66886e44b49af6db14242)
M. Kuball, et al. Appl. Phys. Lett.  82 , 124 (2003)

## Applications of Raman thermography 

![180   × GaN 160  140   ♦  SiC 0Q   120  Thermal Boundary  Thermal Boundary  100   Resistance  Resistance 8O  4O  20  GaN   Sic  0.1   10   100   1000  Depth (μm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/113d8d55-59f4-43f0-a7b8-03bb3a2ec4cf/113d8d55-59f4-43f0-a7b8-03bb3a2ec4cf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=062ff4b5738c950ba26d6465f3c52823475dd0ad)
M. Kuball et al,, IEEE Electron Dev Llett.  23 , 7 (2002).

![6 GaN  CS-6  CS-6 5  Extra channel temperature rise  URI-4  URI-4  CS-3  CS-3  TBR x10-8(m2K/W)    30%  30% 4  sitc  CS-4  URI-3a URI-3a   CS-2   200 nm  3  CS-5  CS-5  URI-2,  URI-2  20% URI-3b  URI-3b 2 cS- 1  CS-1  1  URl-1   URI-1  accuracy  Measurement   Measurement  accuracy  10%%  10%  500 nm   sic  59/0  5%   100 100   150  150  200  200  250  250 Interface temperature (°C)  Interface temperature ( o C)  Keep Out  Keep Out  Related to microstructure  Related to microstructure  Video Zone  Video Zone ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2a2a62b6-56a0-4873-a64f-4be67d651cbd/2a2a62b6-56a0-4873-a64f-4be67d651cbd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=ae82a11196b662ade917644eaad0ac0463c4cd4e)
A. Manoi et al, Electron Dev. Lett. 31, 1395 (2010)

## Time-resolved Raman thermography 

![Pulsed  Pulsed   ON  OFF  OFF laser   514  Taser   Experiment  source  source  Simulation  120  100  80  Best  Best IR time  IR time  6O  resolution  resolution Time (μs)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e387ef3e-6988-479d-b32c-a3caa186b6ca/e387ef3e-6988-479d-b32c-a3caa186b6ca.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=6729d7a674e6eb9ad6394f9ee528152088d534b0)
The technique allows probing temperature as function of time (best resolution we  demonstrated was 5ns but this could be improved even further).

![Keep Out  Keep Out  Video Zone  Video Zone ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e5f73384-a4b6-4d49-bf5d-b09d2f462e1a/e5f73384-a4b6-4d49-bf5d-b09d2f462e1a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=0075f535fbc8ddf76440827a0de0a9eb39834690)
M Kuball et al, IEEE Trans. Dev. Mat Rel. 16, 667 (2016); M. Kuball et al., IEEE Electron Dev Lett 28, 86 (2007).

## Time-resolved Raman thermography 

![GaN-on-sapphire  GaN-on-sapphire 120 120  C] o Oo1   6.1   Heat diffusion  Heat diffusion Temperature [ 100 100  88  80  yo.+x   GaN-on-SiC  GaN-on-SiC 60 -100  -100  0  100  100  200  200 Time [ns] Time [ns]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/07087fc2-0746-44f6-af26-afb28a513aa2/07087fc2-0746-44f6-af26-afb28a513aa2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=9277c204a136f08d397d31aef41f31e2fb8120f0)
G. J. Riedel  et al .,  IEEE Electron Dev Lett  29 , 416 (2008)

![S  D  S 4O  40 D  S m  wm ooL  µ C) ③0  30  100  o Temperature rise ( 20 20     G  25μm  25 µm Temperature  Temperature   Splits  splits 10 10   Implications for  Implications for  Identical  ldentical   linearity of devices  linearity of devices increase  increase 0 10 W/mm 10 W/mm  0.0  0.0  0.5  0.5  1.0  1.0  1.5  1.5  2.0  2.0  2.5  2.5 3.0  3.0 Time (μs)  Time ( µ s)  Keep Out  Keep Out  Video Zone  Video Zone A. Manoi et al., Solid-State Electronics, 57, 14 (2011)  A. Manoi et al., Solid-State Electronics,  57 , 14 (2011) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c7ae971f-773f-479a-a3fa-ab485989676c/c7ae971f-773f-479a-a3fa-ab485989676c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=10f49d597f97b0335bfbb6bfb2a6ec915ccde2bd)
## Raman thermography – DC vs RF operation 

![a)  090 60015705   loadline  DC  100VDS  5.9W/mm  454050   30V  DS  2.5W/mm  Lateralpostion[um]  350  DC,175°C  RF,175°C  300   DC,150°C  RF,150°C  DC,125C  250   口RF，125°℃  200  150  100  10   12  Pss[W]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/39c9b436-5e30-4055-a8d1-fb148e694c8e/39c9b436-5e30-4055-a8d1-fb148e694c8e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=14ea29e27226b0b5a49bbc283c7c6c5599be4d48)
![AlGaN  GaN  30V  OS  100V  ODS   20nm  30VDs   60VDs100VDs  S  Lateralpostion[μm]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/97d5531d-78d0-43f9-97bf-39044c3d1f68/97d5531d-78d0-43f9-97bf-39044c3d1f68.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=84c9bcd4ffb69fd828e61f32aedab83f2bcd30f2)
M Kuball et al, IEEE Trans. Dev. Mat Rel. 16, 667 (2016).

Keep Out  Video Zone

## Strain correction in Raman measurements 

![570   E,(high)   Calibration  569  EZ   A(LO)  568  coefficients   coefficients  567  566  ve  surement  565  E2△w   A(LO)△W  564  (ON-pinch   6ff)   (ON-pinchoff)  563  GaN/SiC  562  Analysis  GaN/Sapphire  561  GaN/Si(111)  560   freestandingGaN   E2△T   A(LO) △T  559  100   200   300   400   500   600   700  Temperature   Stresscorrection  Compare  35000  Pinch-off  30000   lncrease   P   Options:  P2   1)E2△T=A(LO)△T,useE△Tvalue;  25000   P3  PA   2)E2△T=A(LO)△T,use A(LO)△T value;  PS  20000   GaNE2high   3)E2△T≠A(LO)△T,perform 2peakanalysis  toseparatestressandtemperature.  15000  GaNA1(LO)  10000  M Kuball et al, IEEE Trans. Dev. Mat Rel. 16, 667 (2016) MKuballetal,IEEETrans.Dev.MatRe  5000  550   600   650   700   750  Ramanshift(cm-1)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6ca4ca00-c481-42b1-88e4-e566ad26866d/6ca4ca00-c481-42b1-88e4-e566ad26866d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=c94a057eefa77d0b8877f67f1191a2d8a5b7ae1c)
Temperature dependence of  phonon modes:

$$\Delta\omega=\omega_{0}-\frac{A}{\exp\left[\frac{B\hbar\omega_{0}}{k_{B}T}\right]-1}$$
In addition, phonon energy is  also affected by strain:

$$\Delta\upomega\approx\up a\,\left(\upvarepsilon_{\boldsymbol{x}\boldsymbol{x}}+\upvarepsilon_{\boldsymbol{y}\boldsymbol{y}}\right)+\upmathsf{b}\;\upvarepsilon_{\boldsymbol{z}\boldsymbol{z}}$$
Keep Out  Video Zone

## Raman example Ga 2 O 3  power & GaN RF switch 

![Heatflux  x104(w/cm²)  Sat  Devices  Devices   0.8   9.5  Measurement  SiO2   processed   Simulation   △T(°C)  processed   0_D   A.V  VD   at NICT  at NICT  Gate   2.4   23  -Ga2O3channel (0.3 μm)  Si+-implanted   2.S   nos   19   "SLCFET"  “SLCFET” ■Meas. 1.87 W/mm  UID Ga2O: buffer (0.9 μm)    Meas. 1.00 W/mm   Superlattice   devices  devices  1S  Fe-doped semi-insulating   ... 3-D Sim. surface  β-Ga,0s (010) substrate   1.87 W/mm   - 3-D Sim. channel   13   processed  processed  Buffer  S   at Northrup  at Northrup  150   VDs=1V  Grumman  Grumman :1.46W/mm   120  Simulated channel temperature  100   GRT measurement   100  1.00 W/mm   GRT simulation  Raman measurement   C.Middletonetal,IEEEElectron  C. Middleton et al, IEEE Electron  80  Rr, Ram.an simylatio/mm)   Dev Lett. 40, 1374 - 1377 (2019) Dev Lett.40, 1374 - 1377 (2019)   0.51 W/mm  6O  +  ：   ：:  0.14 W/mm  4O-10   2O   30   40  20-   Keep Out  Keep Out  Lateral position [μm]  J. W. Pomeroy, et al., IEEE Electron Dev. Lett. 40, 189 - 192 (2019).  J. W. Pomeroy, et al., IEEE Electron Dev. Lett.  40 , 189 – 192 (2019).  C1   Video Zone  Video Zone Power Density (W/mm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/47317097-9b59-44a4-b336-fbf5098a5f13/47317097-9b59-44a4-b336-fbf5098a5f13.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=52bdb4a6f6bb2ec5c39edc2ff5ae4d9e87963425)
## GaN RF devices - different manufacturers 

![A. Manoi et al, IEEE Electron  A. Manoi et al, IEEE Electron  F. Gucmann et al., CSMantech 2019.  F. Gucmann et al., CSMantech 2019.  D  SiN  SiN  G  G  S  Dev. Lett. 31,1395 (2010)  Dev. Lett. 31, 1395 (2010)  Source   Drain  T nax  max  T.E.M.  160   Packaged - 2, 4 fingers, T =25°C, 50°℃   GaN GaN  140   (W =75μm, Gate pitch=30μm)  ●Manufacturer C   T Raman  Raman si   Manufacturer C   TBR TBRe  eff  Sio  SiC (W,=125μm, Gate pitch=30μm)   GaN  120  (W,=45μm, GG=14μm)   Manufacturer D - 4 fingers, T=50°C   2 and 4 finger devices packaged  2 and 4 finger devices packaged  100  and on wafer  and on wafer  sic  8   •  Device layout (Wa, gate pitch)  Device layout   , gate pitch)  6   has the strongest influence  has the strongest influence  GaN  2   •  Some differences due to  Some differences due to    interface  On wafer - 2 fingers, T,=25°℃  uue   Manufacturer A   differences in thermal  differences in thermal   AIN   defects   TBRe  euo   (W,=50μm, Gate pitch=17μm)   interface  ☆←Manufacturer B   resistance between the GaN  resistance between the GaN (W=40μm, Gate pitch=40μm)    Sic  10121416182022   and SiC (TBReff)  and SiC  P   (W/mm)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3bf95e84-d812-43ac-8b40-21aabf0c387f/3bf95e84-d812-43ac-8b40-21aabf0c387f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=6a96174c4486056247b5fa02e7fa1d0e1928bfec)
We have looked at 100s of devices from working with industry, and always find  that a combination of measurement and simulation is the best approach, rather  than relying only on simulation.

Keep Out  Video Zone

## Diamond on N-polar GaN 

|5-10nmMOCVD SiN4|
|---|
|N-polar GaN Channel|
|Alo.38Gao.62N BackBarrier|
|Graded AlGaN|
|Si-doped GaN|
|S.I.GaNBuffer|
|SiC/SapphireSubstrate|


![Cross-section SEM   >moreisotropic   Diamond  Diamond   SisN  GaN HEMT  2DEG  GaNHEMT   1m   1nm  STEM  25  Diamond/10nmSiN/GaN  Diamond/1nmSiN/GaN  )   20  15  10nmSiN4   M. Malakoutian et al, ACS Appl. Mater. Interfaces 13, 60553 (2021) M.Malakoutianet al,ACSAppl.Mater.Interfaces 13,60553 (2021)  <1nm SiN4  Calculated lumpedTBRrange  300   700   16002000   Keep Out  Keep Out  Diamond Thickness (nm)   Video Zone Video Zone  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0d2960dd-6e08-4421-9615-0f11a6f59a99/0d2960dd-6e08-4421-9615-0f11a6f59a99.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=9d1e173cb441c99aea030414dedf89006bd36870)
Ultra-low TBR between  diamond and GaN for  efficient heat extraction

## How to compare simulated and measured data 

## 2-D device simulation 

Carrier concentration and mobility  adjusted to match I thres  and I DS

Computationally efficient 3-D finite element model 2-D Joule heat power distribution, applied to 3-D model  for each  ${\sf V}_{\sf D S}$  , normalised to measured P diss

![Gate  Gate 1 μm  1 μm n-Ga2O3 channel (0.3 μm)  n - -Ga 2 O 3  channel (0.3  μm) UID Ga2O3 buffer (0.9 μm)  UID Ga 2 O 3  buffer (0.9  μm) Vds = 20V0  V   = 20V,  0  0.14 [GW/cm 3 ] 0114 [GW/cm3]  DS Vds = 40V,0  V DS  = 40V,  0  2:3 [GW/cm²]  2.3 [GW/cm 3 ] ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/03dbbd93-6341-454f-a23a-427df1638dd9/03dbbd93-6341-454f-a23a-427df1638dd9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=5c54673c6580a6aef044d43a6b8d9b5282080ead)
Increasing V DS  – Joule  heating more concentrated  near gate

Joule heat  distribution at  each bias voltage

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a10f2162-bfd2-4054-b8ac-a1762fababf2/a10f2162-bfd2-4054-b8ac-a1762fababf2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=f93da8f4e2d4e457fbf75598aa51632a727a86ba)
Thermal  parameters

![Inc. T. dependent  Inc. T. dependent,   T peak  peak anisotropic thermal  anisotropic therma.  conductivity  conductivity  1/2 symmetry  ½ symmetry ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7b548a29-c346-487a-aed1-439bbb202db9/7b548a29-c346-487a-aed1-439bbb202db9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=024a925cd8f2bc4c4c1c5e1eee0396e2543820a1)
Material simulation    parameters are fitted to    agree with the thermal    Raman data.

Keep Out  Video Zone

## What is Raman actually measuring ? 

![SP  AlGaN  Raman probed  Gam   GaN volume  TBReif  Sio  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dc557a86-9871-4c59-84fb-8687504ede78/dc557a86-9871-4c59-84fb-8687504ede78.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=1ffc98420e43a2a0dba5319d26493d3dbfaf1dbe)
For  transparent materials  the  technique measures  a volumetric  average  (note it is also material  sensitive); for  non-transparent  material the  surface temperature  is measured.

Calibrated simulations  then used for device design,  e.g., gate pitch and width  dependence of device  temperature.

![225  [10 fingers 20 fingers 50 fingers  200  Die  175   IGaN  2.L  sic  125   Brazing  andpackage  100   Dieattach  Carrier  75  Test fixture  60   TM  Testfixture  25  10   20   ③0  Pdiss (W)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ac873488-d32e-438d-97fa-d47ca9cdb0ca/ac873488-d32e-438d-97fa-d47ca9cdb0ca.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=47b63eeb9d243d9ab537afcfa0fb4064c82f2ae7)
![400  270  350  Temperature rise   220  250  170  200  150  120  100  50   T=25°CPiss=4W/mm  20   40   60   80100120  Gate pitch (μm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/37ba898a-b13a-43e8-a301-d052ed3d39f7/37ba898a-b13a-43e8-a301-d052ed3d39f7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=4ac42f26f8d9755d0393e71254157b54459def1f)
Keep Out  Video Zone

## What determines device temperature leterminiesdevicetemperature  

![COLD  COLD -500  Thermal conductivity (bulk) Thermal conductivity (bulk)  -1 000  Thermal conductivity (thin layers)  Thermal conductivity (thin layers) -1500   Thermal resistances at interfaces  Thermal  resistances at interfaces Thermal capacitances Thermal capacitances  -2000  -2500  1000   2000   HOTooO  HOT  5000   6000   7000   8001  x （km]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f9f5f50b-9add-43f9-9ede-416c16dd355f/f9f5f50b-9add-43f9-9ede-416c16dd355f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=ca41b305c2884010f259f9a4eafe282ff542352f)
We can measure the temperature of a  component but for enabling design changes we  need to measure these underlying properties

Keep Out  Video Zone

## How to measure thermal conductivity ? 

![Probe beam  Probe beam Pumplaser  Pump laser  1 ns  Pump pulse  Pump pulse  intensity  intensity time Photodetector  Photodetector RXT  𝑹𝑹∝𝑻 Beam splitter  Beam splitter  Reflected  Reflected probe beam  probe beam  time  time Objective  Objective Thermoreflectance  Thermoreflectance  transient  transient "Contactless",  “Contactless”,  Epilayer  Interface  Interface Epilayer  above  above  Substrate Substrate   heat diffusion  heat diffusion  bandgap TTR  bandgap TTR ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/082c5db3-60f6-47d6-bf11-e11bcd9d9f61/082c5db3-60f6-47d6-bf11-e11bcd9d9f61.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=17711dddd5e480aeab42caa5643b5a9210bcccfd)
•  Thermal conductivities   •  Thermal boundary resistances

Pomeroy et al., IEEE Electron Dev. Lett.  35 , 1007  (2014)

![TR  IGaN  GaN (\~700 nm)   \~160w/mk  TypicalTBR\~  AmorphousSi,N   25m²K/GW  Poly.Diamond  (50-100 nm)   1200W/mk  AIGaN  GaN  CrvstalineAIN   TBR  2   15 m²K/GW [2]  Poly.Diamond  0_01  TherMapSolutions  10   10:0   1000  Time (ns)  Device temperature can be  Device temperature can be  estimated using simulation using  estimated using simulation using   Keep Out  Keep Out  TTR data as input parameters  TTR data as input parameters  Video Zone  Video Zone ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2cac0cea-6088-449a-bfba-c6d69b6a4e15/2cac0cea-6088-449a-bfba-c6d69b6a4e15.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=18d04be6a7d2de947db2f3add5c75e8089dc08e2)
Transient Thermoreflectance (TTR)

## GaN-substrate thermal boundary resistance (TBR) 

![AiGaN  1_0  GaN  Dielectric  JTBReff  0_8  Nucleation  :01-:6   Diamond  Lower TBR  Opaque HF diamond  0.2  -0-:0  TranslucentMwdiamond  200   400   6001   800  Time (ns)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4fa227f5-0066-4e3a-bf3f-65e6d8c8d303/4fa227f5-0066-4e3a-bf3f-65e6d8c8d303.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=4047304b2f0327ffd5be642fcfd396ae19264560)
![33.00  33.00 30.80  30.80 28.60  28.60 26.40  26.40 24.20  24.20 TBR (1E-8 m2K/GW)  TBR (1E-8 m 2 K/GW)  22.00  22.00 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3922ac8a-58cb-431e-bb80-df5a41df088a/3922ac8a-58cb-431e-bb80-df5a41df088a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=239d230162a0cec0d6808a9aa5e4fa902104cae0)
Quality control and rapid feedback for optimising GaN-on-diamond wafer  fabrication process (DARPA programm with Element Six Technologies)

Keep Out  Video Zone

## SiC substrate thermal conductivity 

High-purity, semi-insulating, on-axis, 4H-SiC from five vendors  has been analysed using transient thermoreflectance; C-face  (optical polish) and the Si-face (CMP).

|Vendor|        Si Face                Polishing      |        Si Face TC                (W m-1 K-1)      |        C Face                Polishing      |        C Face TC                (W m-1 K-1)      |
|---|---|---|---|---|
||CMP|253±33|Optical|300+42/-43|
||CMP|263+33/-32|Optical|277+49/40|
||CMP|240±30|Optical|343+45/-44|
||CMP|243±33|Optical|196±31|
||CMP|259±51|Optical|384±50|


D. Field et al,, CS MANTECH 2022

![CE   CFace  CFacoFil  SiFaoe  SiFaooFil  -  -1 010   10-0K0  Time (ns)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f221206d-ca5d-4c10-995d-b1bdd869977f/f221206d-ca5d-4c10-995d-b1bdd869977f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=08f6f44097019058d8294656a3a9d26170e6157d)
In-depth know-how how to fit &  analyze the experimental  measurement traces / data

![Keep Out  Keep Out  Video Zone Video Zone  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1597fdbb-fe3e-425d-8c1b-6784cae3b5da/1597fdbb-fe3e-425d-8c1b-6784cae3b5da.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=7d40823b12bd467041f575e366cce276d0bb1fda)
## Integration of GaN with diamond (up 2000 W/mK) 

![SiC has a thermal conductivity of 450 W/mK !!!  SiC has a thermal conductivity of 450 W/mK !!! Temp  Temp  carrier  carrier  Temp  Temp  Temp  Temp   Temp  Temp   carrier  carrier carrier  carrier  carrier  carrier GaN HEMT  GaN HEMT  GaN HEMT  GaN HEMT GaN HEMT GaN HEMT   GaN HEMT GaN HEMT   GaN HEMT GaN HEMT   Seedlayer  Seed layer  Seedlayer  Seed layer Seedlayer  Seed layer Substrate  Substrate  Substrate  Substrate  Diamond Diamond   Diamond  Diamond Direct  Direct  Diamond  Diamond  Source field plate  Deposition  Deposition  Passivation  Drain  AlGaN  NJTT DARPA programmes, 3x increased  NJTT DARPA programmes,  3x increased  power devices, around 2013 (Qorv0,  power devices , around 2013 (Qorvo,   GaN 160 W/mK  Raytheon etc); we use here however  Raytheon etc);  we use here however  crystalline AiN instead of SiN.  crystalline AlN instead of SiN.   SiN 1 W/mK   Keep Out  Keep Out  Video Zone  Video Zone Diamond  heat  >1000 w/mk  30 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6a6abee8-b689-493d-8c75-d1a61a00dc36/6a6abee8-b689-493d-8c75-d1a61a00dc36.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=44105f9fb5ffe32a370177e48cba8ed5a82996ac)
## Thermal resistance at the GaN-AlN-diamond interface 

Diamond growth is seeded with  nanodiamond particles  which have defined  surface charge;  AlN surface is prepared  using plasma treatment. 100µm-thick  adherent diamond films now grown.  S.  Mandal et al., ACS Appl. Mater. Interfaces  11, 40826 (2019).

![220  210   Probe bea  200  PnmpIas  190   Pump pul   Jntensiry  Diamond (< 10 um)  Photcdetector  180   Amorphous AIN (20  mmm  Beam splitter  Reflected        170   Objective   probe beam   Thermoremectance   GaN   Nano/micr  Nano/micr transient  oseeding  oseeding Handle wafe  Epitaye  interfac  Seed-2  ③0   Substrate  eot diffusion  Current state-of-the-art  Seed-1  (Si3N4 interlayer)  Seed-1  20  Hydrogen  Hydrogen  Oxygen  Oxygen   AlNsurface   Seed-3   treated  treated  treated  treated   treatment1   nanoseeds  nanoseeds nanoseeds  nanoseeds  AlN surface   AIN surface  treatment2  treatment2  Amorphous AIN   Crystalline AIN   AlGaN  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b651b361-dc27-4ec3-9d13-472c681b9af8/b651b361-dc27-4ec3-9d13-472c681b9af8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=eed310b7e93c1c37c72a40b65d880b4f071d5505)
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/03a2c1f7-a277-4513-9bc0-6b4f67b1a2dd/03a2c1f7-a277-4513-9bc0-6b4f67b1a2dd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=57eae68e073aa45b69374c51105e41a799946770)
3× better TBR eff  than state of the art, but still room for improvement.

Keep Out  Video Zone

## Thermal resistance GaN-on-Diamond device 

GaN-on-SiC

GaN-on-diamond

The full benefits of diamond can be  exploited for  narrow pitch devices , e.g., 13 µm, enabling a  dramatic  improvement in areal power density,  compared to GaN-on-SiC.

,

Gerrer et al, IEEE Trans. Electron Dev, 68, 1530 (2021)

Keep Out  Video Zone

## Ultra-high power RF GaN-diamond devices 

![9 μm pitch devices - note GaN-on-SiC  9 µm pitch devices – note GaN-on-SiC Drain contact  Drain contact  devices have about a 30-40 µm pitch  devices have about a 30-40 μm pitch  11  11m  µ m Good RF  Good RF  performance  performance 80   A power increase of 2.75x can be  A power increase of 2.75x  can be  GaN on Diamond   achieved compared to GaN-on-SiC.  achieved compared to GaN-on-SiC. CW dynamic loadlines  Gate fingers  Gate fingers  Source contacts  Source contacts  60   <75%   T. Gerrer et al, IEEE Trans.  T. Gerrer et al, IEEE Trans.  Electron Dev., 68, 1530 (2021) Electron Dev.,68, 1530 (2021)  10.0kV 17.6mm x3.50k SE(M)   10.0  - DCIv Vcs=OV  VDs=10V  VDs=20V  VDs=30V  Working Current  20-  Keep Out  Keep Out  Video Zone  Video Zone 10   33  ¥30   50   60  Voltage (V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a56f237-6645-48ee-8f74-393005518e38/7a56f237-6645-48ee-8f74-393005518e38.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=20bbbce3a16c678400a8cbf9b010bced69f112d9)
## Scanning thermal microscopy (SThM) 

Ther  Thermocouple  integ  integrated into  AFM  AFM tip

![ANSYS  2019R1  ACADEMIC  647nm  600  550  500  450  350  300  250  200  150  100  20pm   20μm  Temperature map Temperature map   Surface topography Surface topography  34 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f87111ea-0d13-4406-886c-00233b41ae5e/f87111ea-0d13-4406-886c-00233b41ae5e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=1847ed894269de7c033b8ca03650e06f00fc638b)
Keep Out  Video Zone

## SThM calibration – be careful 

![Large contact  70°C  1.4pm  43°C   0.opm  x:12μm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ff9c14e3-1dc1-4460-a90e-04e0f283f9d7/ff9c14e3-1dc1-4460-a90e-04e0f283f9d7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=f7625a9d3eb9efc1152f6dd4388888afb5bc16af)
## Thermal resistance AFM tip - sample surface dependent on 

Variable tip/sample contact area (sample roughness, surface features)   Possible sample thermal conductivity influence

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7dbcc27f-cc35-4c1b-91c1-63ebea934dcc/7dbcc27f-cc35-4c1b-91c1-63ebea934dcc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=cd26b1bf4895682305a5ec6d80e4915a542dce60)
Needs careful point by point  calibration in the measurement

F. Gucmann et al, Nano Today 39, 101206 (2021)

Keep Out  Video Zone

## Hyperspectral quantum rod thermal imaging (HQTI) 

![入start=440 nm  Wavelength   Increasing T   CdSe/CdS  CdSe/CdS 02   quantum rods  quantum rods  =560 nm  Datacube   ShE  Wavelength  SPfilter   HPfilter   ^stop=720 nm  onochron   650 nm Tunable filter  500nm  Beam splitter  Camera  Wavelength (nm)   Wavelength (nm)  Beam splitter   Quantumrodlayer  FieldPlate  LED   SP filter  450nm   500nm   Source   LGate  Passivation   Drain  AlGaN  GaN  Strainrelief layer  Wavelength  Quantum rods   Silicon substrate  DUT   20m  Fast 2D imaging of devce temperature, no device specific calibration   specific calibration   Keep Out  Keep Out  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c93a5b80-63d6-46f7-af15-1e5ac77651e1/c93a5b80-63d6-46f7-af15-1e5ac77651e1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=ef45f4291bc09fb718416963abf10c3e1db68eaa)
B. Oner et at, ACS Appl. Electron. Mater. 2, 93 (2020); B. Oner et al. IEEE Electron Dev Lett 41, 812-815, (2020)

## HQTI comparison to simulation & IR measurements 

![HTQI  HTQI             FE simulation       IR thermography FE simulation   IR thermography  HQT  AT(C)   △T(C)   △T(OC)   IR  80   Model:Surface  Model: Channel  65   SS   28  S5   S5   60  18.7  F50  5   AS  4  35  20wm   30  25   25   201  G-FP    Channel opening  9.3  10-  15   15  Distance(μm)  20wm   20wm   20mi  source   Drain   Source   Drain   Source   Drain  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/36ad786e-cc72-4c2a-a184-c22a214927f8/36ad786e-cc72-4c2a-a184-c22a214927f8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=36a3a687e48ab428d4f150b35e0e6c5d59cdc4a2)
Fast temperature maps with submicron spatial resolution (0.6 µm)

Video Zone

## Can one push spatial resolution even further ? 

![With HSIL  With HSIL  Standard optics  Standard optics source   Gate   Drain   Source   Gate   Drain  GaN  Sicn=2.6  SIL  air  50μm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/60c3f19d-8c27-4bb6-80a4-892818fca490/60c3f19d-8c27-4bb6-80a4-892818fca490.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=643d9bf209ec90254c62b092050033a0ac2e289f)
J.W. Pomeroy et al., J. Appl. Phys. 118, 144501 (2015).

![10  Lateral:  widefield   0.6  confocal  uum   Axial:  ...widefield  Designed   - confocal  Sm  SiC SILlimit  le>  0.2  0.0  N.A.  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d6a01270-a9f0-444e-9fb7-6f671ea818d6/d6a01270-a9f0-444e-9fb7-6f671ea818d6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=1f3c8094dcd38f852f8c5cf08948d0fa5c091c69)
Lateral and axial spatial resolutions  <100nm are possible for high n  materials  $\mathbf{\sigma}->$   Possible to probe 3-D  temperature distribution without  spatial average effects.

![ction  n9  sample   illumination  (unknown)   (known)  Moirep   ern (raw images)  sample  (SIM image)  Reconstruction  STED   Saturated  Excitation   EffectivePSF  pattern   depletior  SIM or STED  SIM or STED Keep Out  Keep Out  Video Zone  Video Zone ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/15af9095-fd15-4dca-b7d0-585cbc33f843/15af9095-fd15-4dca-b7d0-585cbc33f843.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=27a45120ef62a88b3dab6767239f1c5385c4967c)
Comparison between different devices approaches

|Technique|        Spatial                resolution      |        Time-                resolution      |Accuracy| Speed|
|---|---|---|---|---|
|IF|>3μm|μs to ms|        Limited for small                features      | Full area maps|
|Raman|        0.5-0.7μm                (50-100nm with                SIL)      |ns|High|        Mostly point                measurements      |
|Thermoreflectance|0.5-0.7μm|US|         Sometimes ok                sometimes not      |Full area maps|
|SThM|nm-resolution|s|        Needs careful                calibration      |Full area maps|
|HQTI|        0.5-0.7μm                (50-100nm with                SIL)      |μs to ms|        High - needs                deposition of                 nanoparticles      |Full area maps|
|        Electrical testing                methods      |        None                (temperature                average)      |        Various                 ranges      |        Limited as it                averages of                large areas      |70|


Keep Out  Video Zone

## We can also go even further … 

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b17b9567-75ba-4159-ba6f-86c3a672f0fb/b17b9567-75ba-4159-ba6f-86c3a672f0fb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=bf3f9ffb43ed693ae9d5fd2ad3dba10a33075186)
![Directly measure underlying electric field distribution  Directly measure underlying electric field distribution Second harmonic generation for electric fields  Second harmonic generation for electric fields x（2),x（3)  SourceGate   Drain  Gate   SourceGate   Drain  Vns=15V  iNpas   WaferA  2DEG   Drain   x105   WaferB   Vos=15V  VDs=45V  Doped GaN buffer  60v  Fundamental  VDs=75V  laser,Iw   90v  105  os=105V  EFISHG signal,12w  Position(um)  Position (um)  Y. Cao et al., Nature Electronics  Y. Ca0 et al., Nature Electronics 4, 478 (2021)  4,  478 (2021)  Two RF devices with different epitaxies TwoRF deviceswith different epitaxies  Electric field within semiconductor device  Electric field within semiconductor device Keep Out  Keep Out  𝑋𝑋𝑋𝑋𝑋𝑋  +(3xxxxxEx,Ex,Ex+6xxxzzEx,Ez,Ez)²   Video Zone  Video Zone ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1d9eb4cb-a24a-45cb-adf2-c246bacf2d65/1d9eb4cb-a24a-45cb-adf2-c246bacf2d65.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=92333018d2806f49c179c6208b64171bf3a34d44)
∝2𝜒𝜒

## Edge termination(ET) in GaN vertical devices 

![Mg ion implantation  Mg ion implantation Anode  Anode   p+ GaN  p+GaN  wd  p-GaN  n GaN drift layer  n GaN drift layer  GaN substrate   n-GaN drift layer  N8+   Anode   N8+  p+GaN  Cathode  n GaN drift layer  GaN substrate  GaN substrate  Cathode  Cathode  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4aee841e-59a3-4aef-8919-cea7e51e276f/4aee841e-59a3-4aef-8919-cea7e51e276f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=2f72bb3343d73bae359f9744738267da4d1f9b16)
•  Edge termination (ET) in vertical power devices  critical to maximize break down voltage.

•  The optimal working of the ET depends on doping, ion implication, angles of bevels etc ie is  critically dependent on process parameters.

Keep Out  Video Zone

## Ion-implanted 2-step mesa ET 

![Excessive implantation dose  Excessive implantation dose  Deficient implantation dose  Deficient implantation dose 1E-5  1E-5  0.12 0.12   -1  BV=800V  -1  BV=800V Current (A)     Anode Anode   BV=800V   Anode Anode   BV=800V  0.08 0.08  p-GaN 3.5x1017  p - GaN  3.5×10 17 1E-6  1E-6  0.04  0.04  p p+GaN  + GaN  Mg 4x1017  Mg 4×10 17  p+GaN  p + GaN 0  0 Current (A)  0.00 0.00  0  1  2  3  4  5 1E-7 ooe..-Voltage (V)  Voltage (V)  Z (µm) (uun)   n-GaN  n - GaN  Z (µm) (uun)   n-GaN  n - GaN 7  1E-8  1E-8  7  1  E Efield (MV/cm)   field (MV/cm)  1  Efield (MV/cm)  E  field (MV/cm) 3.5  3.5  3.5  3.5 5×1013 cm-2  5×10 13   cm -2  1E-9  1E-9  ion implantation dose  ion implantation dose  0  0 2  2 -800  -800  -600  -600  -400  -400  -200  -200  0  0  10  10  20  20  30  4O  40  50  50  0  10 10   20  20  ③0  30  40  40  50  50 Voltage (V)  Voltage (V)  X (μm)  X (µm)  X (μm)  X (µm) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d539404f-d879-4cc1-8847-cb27d23c49fa/d539404f-d879-4cc1-8847-cb27d23c49fa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=3ec1c75c2b8f8d243f8858a6e0aa7d15446edf71)
•  Same breakdown voltage can result from higher or lower ion implantation dose  than desired value. •  Different electric field distributions clearly indicate how the ion implantation dose  deviate from the optimal design.

Keep Out  Video Zone

## EFISHG measurement 

![Anode   Outer bevel  pGaN   100V  aserdiode   200V  nGaN  00nmCW   Lens   Fundamental   (un'qe)   300V  Mirroi   2laserIu  n+GaN  SEFISHG signa  BulkGaN  substrate  Half-wave   Cathode   ple  Lens   Polarizer plate  Short pass   Ti:Sapphire  dichroic mirror  800nmfs  DUT  Reversebias   Lock-in  band pass   Avalanche   -30   -20   -10   10   20   30  filter   photodetector  Position (μm)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/85666801-88b4-418e-a8de-30ed1372d9f6/85666801-88b4-418e-a8de-30ed1372d9f6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=344a7e61b6b195b6c76a33c0635916506dd1e7c4)
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f25dcc0f-7e61-4e88-9acb-65fbd3febf4a/f25dcc0f-7e61-4e88-9acb-65fbd3febf4a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=d3c25429d7bc35b6c352a1195dae06386c42c993)
EFISHG measurements is most sensitive to in-plane  electric fieldS, but here we mostly probe the vertical  electric field

Y. Cao et al., CS MANTECH 2022

Keep Out  Video Zone

## Effect of ion implantation dose on electric field distribution 

![-1 一一   -1 Anean  Anode  BV=800V  BV=800V  Anode  Anode  P GaNV5=1800V  BV=800V p +  GaN  Mg 4x1017  Mg 4×10 17  p+ GaN  p +  GaN  p -   GaN  3.5×10 17  1x1019   1×10 19   1x1019   1×10 19 0  0 Z (µm) 7  (uun)   n- GaN  n -   GaN  Z (µm)  n- GaN  n -   GaN 7  1  E field (MV/cm)  E z  field (MV/cm)  1  E, field (MV/cm)  E  field (MV/cm) z  (300V)  (300V)  (300V)  (300V) 2  0  1.5  1.5  0  1.5 15  2 0  10  10  20  20  ③0  30  4O  40  50  50  0  10  10  20  20  ③0  30  △O  40  50  50 X (μm)  X (µm) X (μm)  X (µm) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4faaf23b-aee6-4369-8e9b-96100ef344e8/4faaf23b-aee6-4369-8e9b-96100ef344e8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=88e1e3ce173db2fdd8d0c47c1a1702785b30ce34)
![E, along junctions  E z  along junctions Anode   Outer bevel   ()    TII  1.５  1.0  (a)  0.5  0_0  20   ③0   50  Position (μm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d48485b1-083d-42e8-bb20-ac2e990efc26/d48485b1-083d-42e8-bb20-ac2e990efc26.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=49dac87a156d1c0246fbc7685e9067cdfa5fe667)
•  When implantation dose is higher than desired, donor-like damages are fully compensated   •  When implantation dose is lower than desired, the partially thinned p-GaN layer spreads    $E_{z}$    •  In none of those cases there agreement to experiment.

Keep Out  Video Zone

## Effect of ion implantation dose on electric field distribution 

![-1  Anode   Outer bevel  2.0  Anode  Anode  BV=800V  BV=800V  E, along junctions  E z  along junctions  1600  p+ GaN  p +  GaN  p- GaN 1x1017  p -   GaN  1×10 17 1-5  6×1017  6×10 17  1200  0 800  Z (µm) (uun)   n -   GaN  E> field  E z  field   1.0  n-GaN   (mv/cm)  (MV/cm) 7   300V  300V    400  1 0.5  2 1013   1014   1015   1016  0  0_0   Mg ion dose (cm-2)  2 0  10 10   20  20  ③0  30  40 40   50  10   20   ③0   40   50   Y. Cao et al, CS Mantech 2022  Y. Cao et al, CS Mantech 2022 X (μm)  X (µm) Position (μm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/56182584-7d95-45d4-83b1-f0570ab3246f/56182584-7d95-45d4-83b1-f0570ab3246f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=450a0473ed66b914957c1eee97d55a90cc6bfc87)
•  Considering the partial activation of Mg in GaN, the low effective acceptor concentration in  partially thinned p-GaN layer leads to early depletion and field peak around anode •  The simulated   $E_{z}$   distribution clearly indicates a lower ion implantation dose than desired

Keep Out  Video Zone

## Example of an other edge termination 

![Anode   Etchedring   1801  Anode   Etchedring  SiN SiNx   SiNx  SiN 100   x  Anode  x un   20mGaNFull-comensated  20nm p ++   GaN Fully-compensated  （um   450nm p +   GaN 600V   80   600V   600V   (3x1019 cm-3)  (3×10 19  cm -3 )  ET  ET BOOV   800V   120   BOOV  1000V   60   1000V   100   1000V   Edge termination ring Edge termination ring    Partially-compensated  Partially-compensated  p- GaN ET  p- GaN ET ¥80  12 μm n GaN (\~1x1016 cm-3)  12 µm n -   GaN (\~1×10 16  cm -3 ) DILI   O   OIJ  60  1 μm n+ GaN (2x1018 cm-3)  1 µm n +   GaN (2×10 18  cm -3 ) 20  n+ GaN substrate  n+ GaN substrate Cathode  Cathode 10   20   30   50   60   30   4O   50   60   20   30：   40   50  Position (μm)      Em)   B  Y Cao et al, accepted for publicatior  Y Cao et al, accepted for publication    -1  -1  -1     in Appl. Phys. Lett. (2022)  in Appl. Phys. Lett. (2022)   Anode Anode   SiNx  SiNx  Anode node   Sinx  SiNx  Anode   SiNx  SiNx   p+Gan  p+GaN  Et (FC)  ET (FC)  p+GaN   p+GaN  ET (FC)  ET (FC)     p+GaN   p+GaN    ET (FC)    0  0  0              C 40nm 6x1017 cm-3  40nm 6×10 17   cm -3  40nm 5x1017 cm-3  40nm 5×10 17   cm -3             ET (PC)  ET (PC)  ET (PC)  ET (PC)       A 1  n-GaN  n-GaN  Exfield (Mv/cm)  E x  field (MV/cm)  1  n-GaN n-GaN   Exfield (Mv/cm)  E x  field (MV/cm)  1  n-GaN n-GaN   Ex field (Mv/cm)  E x  field (MV/cm) 1.3  1.3  2  3.3 2 0.6  0.6  1 0  0  0 2  2  2 0  20  20  40  60 60   80 0   0  20  20  40  60  60  80  80  0  20  20  40  60  60  80  80 Keep Out  Keep Out  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1a319315-f406-4abe-a6b5-b9f8afd345a3/1a319315-f406-4abe-a6b5-b9f8afd345a3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=c13613a9463f09fb0522c254a3f4ff6b33cd292e)
partialll

compensat

avers

in the

ecge

Optimization / quality control

Video Zone

## Optimization of ET fabrication 

![Black box  Implantation dose  Fabrication  with full set of   Electrical test  Etching thickness  parameters  Optimized device  Bevel mesa angle  Fabrication with   Doping concentration   Electrical test /  reduced set of  field measurement  parameters  Epitaxial growth   Device internal  operation  Keep Out  Keep Out  Video Zone  Video Zone ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d43a316c-72b3-41f0-a9e7-c7a712c8293d/d43a316c-72b3-41f0-a9e7-c7a712c8293d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=eb6f2e8aaf27bc2082e205439c570729541bd898)
## Advanced device packaging & die attach 

![GaN  microwave  transistor  Diamond  heat....  spreader  noie  Microfluidic  coolinB:  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a6510f98-feeb-48b0-9dbf-084fb26305ac/a6510f98-feeb-48b0-9dbf-084fb26305ac.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=20df231fe101100e30638e39d3cbd869f3bf7277)
## Metal – diamond composites  (thermal  

conductivity as high as 800 W/mK

Inlet

Jet impinging to extract  waste heat

d=2mm

![Faqir et al., Journal of Microelectronics and  Faqir et al., Journal of Microelectronics and   Microfluidics  Microfluidics  Electronic Packaging 10, 54 (2013)  Electronic Packaging  10 , 54 (2013). with copper  with  copper  （0,0)   Die   foam and  foam  and  Epoxy   advanced heat  advanced heat  Copper lid   transfer fluid  transfer fluid Copper foam  -0.93kPa  2.60kPa  Outlet  Diamond   d=2mm  insert  10m  Keep Out  Keep Out   Pressure distribution in jet channel   Video Zone Video Zone  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4ce64eb8-ff3a-450b-adb8-23df2af3e94f/4ce64eb8-ff3a-450b-adb8-23df2af3e94f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=ede55d8ea1897f2d312aa2ef9cd658f927860829)
G. Zhang et al, IEEE Trans Comp Packag Manufact Techn 11, 748 (2021) 48

## Package material and die attach thermal properties 

![Thermal boundary  Thermal boundary   Effective thermal  Effectivethermal  resistance  resistance  conductivity  conductivity High-power Die High-power Die   Voids  Voids  K'<K  𝜿𝜿 ′   ≪𝜿𝜿 ldie  𝑹𝑹  Die attach  𝟏𝟏 Die attach  Die attach  𝜿𝜿  𝜿𝜿 ′  120   Heatsink  𝑹𝑹 R2  𝟐𝟐  （0。>  Thermal  Thermal  80  conductivity conductivity  Heatsink  Heatsink 40  Thermal properties often not well  Thermal properties often not well  enough known enoughknown  49  49 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3cc4159f-0a64-4a3b-a731-39a32783bafa/3cc4159f-0a64-4a3b-a731-39a32783bafa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=c495339178488be9a752ce46aadd35fa5f850fd8)
Keep Out  Video Zone

## Frequency domain thermoreflectance 

![(-n-e)   Phase shift  Heat the surface of the  Heat the surface of the  Measure the probe  Measure the probe   Pump laser   sample (\~1mm spot)  sample (\~1mm spot) reflected signal  reflected signal   (Modulationfrequency10Hz-10kHz)  -5 5   Probe laser  DOO,  000000  Phase (deg) (bap)  -20 -20  Monitor the surface  Monitor the surface  temperature change  temperature change -35  -35 000000000  Data  Data -50  -50 101  10 1  ¥102  10 2  103  10 3  104  10 4 Frequency (Hz)  Frequency (Hz) N Poopakdee, et al., ACS Appl. Electron Mat. (2022); Z. Abdhalla et al., CS  MANTECH2022  MANTECH 2022 N Poopakdee, et al., ACS Appl. Electron Mat. (2022); Z. Abdhalla et al., CS   Keep Out  Keep Out  Video Zone  Video Zone Determine the thermal property with  Determine the thermal property with  heat diffusion model heat diffusion model   Sample ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e3cb982b-c8fe-407e-831e-0ba44330c3d6/e3cb982b-c8fe-407e-831e-0ba44330c3d6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=b1db1a071980d81be7d992d8028424e24c2c4083)
## Frequency domain thermoreflectance 

![Diamon  k = 900 ±50 W/m·K  -25  Pump laser   (y-w/m) y pansean   Copder  (Modulation frequency 10Hz-10kHz)  103  (6ek   0.25mm  0.25mm   Silicon  Probe   -30   Diamond Diamond  Nlaser  Sapphire  102  -35  Best fit  Data   ooooo  -40   101  ¥103   104   10：   102   ¥103  Frequency (Hz)   Literature k (W/m·K)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fcef24a4-a2a0-4581-881f-408e4807da53/fcef24a4-a2a0-4581-881f-408e4807da53.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=d3f4fab308670935e4c8ef56339493f333ee9f34)
FDTR can measure a wide range of thermal conductivity materials,  with different thickness including a thin high thermal conductivity  diamond, not possible with standard laser flash

Keep Out  Video Zone

Sample

## Frequency domain thermoreflectance 

![Pump   Probe  Cu-Dia  Aufilm  GaN 2μm  .HEATFLOW   Cladding  2  SiC 75μm  TPD  fmod ≈ 40kHz   Diamond   3mm  TPD   Die attach 20μm   Composite  fmod\~7kHz  Heat sink 1mm   Cladding   TherMapSolutions  TPD  fmod \~ 100Hz  FDTR   LFA   K=527±61W/mK  KC3   G,=21.4±0.9MW/m²K  Sample   (W/m·K)   (MW/m2·K)   (MW/m2·K)   （pmm)   (W/m-K)   G2=5.24±1.34MW/m²K  Cu-Dia-1   801 ± 135   13.3 ± 0.6   5.21 ± 1.74   172 ± 23   860   -Bestfit  Cu-Dia-2   412 ± 53   16.5 ± 0.9   6.04 ± 0.68   97.8 ± 6.2   ５04   Data  Ag-Dia   306 ± 49   54.9 ± 31.5   5.09 ± 1.33   69.9 ± 9.1   28５  -30   G±25%  N Poopakdee, et al., ACS Appl. Electron Mat. (2022) - https://doi.org/10.1021/acsaelm.1c01239  N Poopakdee, et al., ACS Appl. Electron Mat. (2022) - https://doi.org/10.1021/acsaelm.1c01239    & UoB Masters thesis; Z. Abdhalla et al., CS MANTECH 2022; Z. Abdhalla et al. (in   & UoB Masters thesis; Z. Abdhalla et al., CS MANTECH 2022; Z. Abdhalla et al. (in   -35   Keep Out  Keep Out  preparation).  preparation).  G2±25%  -40   Video Zone  Video Zone 102   103   104  Frequency (Hz)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/46859064-a840-4ab8-a9ed-2c2fac99db28/46859064-a840-4ab8-a9ed-2c2fac99db28.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=9845e8d01206984a8e856a74d8c478a7a489d1a8)
## Die attach properties: Probing through the full die 

![ o Supplier 1  x Supplier 2  K2= 7 ±1 W/m·K  (bap)  20  XXV  se   K' = 72 ±5 W/m·K  -35  -50  102   ¥103  Frequency  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c0459010-b06f-4506-9c9c-5a95403cf371/c0459010-b06f-4506-9c9c-5a95403cf371.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=cfc6756ed0f6a3b271a948fc5c5378ac6aeb9458)
Data sheet of die attach: 200 W/mK

![Pump   Probe  GaN2μm  HEATFLOW  Sic75μm  TPD   10kHz  Die attach 20μm  PO   SkHE  Heat sink 1mm  \*Die attach:datasheetK=200W/m·K  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/09b56fa8-e05c-4505-af9a-b6249855d912/09b56fa8-e05c-4505-af9a-b6249855d912.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=e377eade551a09ce09d265310676166d34cd61dd)
![170μm 170pm   185pm  185μm Supplier 1  Supplier 1  Supplier 2  Supplier 2 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/db133553-44b6-4067-8f47-46f3b4b494bb/db133553-44b6-4067-8f47-46f3b4b494bb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=a6d73a3e22b1c3a1c56ed0ff4b2492595f717ed4)
X-ray transmission imaging

![Keep Out  Keep Out  Video Zone  Video Zone ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0020afc3-68de-4e38-87c6-4c6ff65ef2da/0020afc3-68de-4e38-87c6-4c6ff65ef2da.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=99594cff8982fc7d7ef0b108d72cfa9bf1bac219)
## Conclusions 

Measuring temperature with higher resolution  important for todays’ semiconductor technology.

A thermal simulation is only as accurate as its input parameters (and the models used e.g. for  interfaces) –  do not trust simulation blindly .     There are numerous  new techniques emerging that allow temperature measurements with  sub-micron spatial resolution , e.g. Raman thermography, HQTI etc.     Experimental techniques allow validation of thermal models for device optimization.   Thermal materials characterization of high benefit also for package developments.

![  140 Source  Gate  Drain Pdiss=1.28w/mm   DC 120 2  µ s gatej   dielectric   100  Pump laser  o C)  Probe  Temperature rise ( 80  laser    60  400 ns 40  200 ns  copper  20  Keep Out  Keep Out  -200 ns 0  heatdiffusion   Video Zone  Video Zone -8  -6  -4  -2  0  2  4  6  aluminium  Position ( µ m) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0c171ef4-6339-4533-a677-5c29746dde32/0c171ef4-6339-4533-a677-5c29746dde32.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=9b62bfaf60989d1f5d21e97cf4999d8125d0ecd9)
## Thanks to my team & our collaborators 

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d100254b-01db-4684-9536-16f56db9ea52/d100254b-01db-4684-9536-16f56db9ea52.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=6ba8e7ec547e818dda170977beb94b36cc8afb59)
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4f6a6cbb-12ed-4ba5-a4ce-eac8b632c31c/4f6a6cbb-12ed-4ba5-a4ce-eac8b632c31c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=12f7444f4c6ef4137869374e9434a606ea9ec573)
![Keep Out  Keep Out  Video Zone  Video Zone ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cd5ae80d-2454-4cd0-a8ba-6963010d083a/cd5ae80d-2454-4cd0-a8ba-6963010d083a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215807%3B1743219407&q-key-time=1743215807%3B1743219407&q-header-list=host&q-url-param-list=&q-signature=a342cda62df8bf6c7dee97c8d3a0ee3a934c647d)
