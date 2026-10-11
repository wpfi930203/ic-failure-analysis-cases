---
title: "David Su_TEM_FIB_Tutorial_for_Printing_Part_1.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_301ba96415e2a84c74e03c2d36ec8e537295230462135641
file_size: 21455434
---

## IPFA 2019 Tutorial: Transmission Electron Microscopy and  Focused Ion Beams 

David Su

## Acknowledgment 

•  Yu Zhu – TSMC   •  Jong-Shing Bow – IST   •  Ozan Ugurlu – Thermo Fisher   •  David Tien – Thermo Fisher

## Outline 

•  TEM: Imaging and Diffraction   •  TEM: Elemental and Chemical Analysis   •  STEM: Imaging and Analysis   •  TEM, STEM: Spherical aberration (Cs) correction   •  TEM: Sample preparation   •  FIB: Circuit Editing   •  Concluding Remarks

## Microscopes 

SEM

STEM

## TEM/STEM  

![OM mscop  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/78005e8c-8346-47d1-8604-8bd50f7485c2/78005e8c-8346-47d1-8604-8bd50f7485c2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=a6ef7dc5c28d03d0e2ceaad614f33531e28ccae2)
![SEM  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5428db4d-ffc2-466f-9d43-5893910bbdcf/5428db4d-ffc2-466f-9d43-5893910bbdcf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=926c207cf766ccb85decc954000b227f2259421a)
𝛿  \~ a few nm

![TEM  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/15820ac4-292f-4f14-86ae-ea274e2bc506/15820ac4-292f-4f14-86ae-ea274e2bc506.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=23cc8fcd4f07c02bfbac7accb98a4fb91f2fb7bc)
𝜆  \~ 500nm 𝛿  \~ 300nm

𝜆  \~ a few pm (10 -3   nm) 𝛿  \~ 0.1nm, due to lens aberrations

• The smallest distance that can be resolved  $\begin{array}{r}{\delta=\frac{0.61\,\lambda}{\mathrm{NA}}}\end{array}$

• λ is the wavelength, NA is the numerical aperture

## TEM in the Semiconductor Industry 

•  Development: –  In-Depth Materials Analysis –  Process Characterization –  Metrology   •  Production: –  Initial Fab Ramp-Up –  Metrology –  Process Monitoring   •  Failure Analysis

## Failure Analysis 

![Failed  Device Failed   Device  End of Line test End of Line test  Device level  Device level EDA Volume  EDA Volume  > 2 cells  > 2 cells Diagnostics (SW) Diagnostics (Sw)  ≤ 1 cell  ≤ 1 cell Electrical Failure  Electrical Failure  Analysis (EFA) Analysis (EFA)  sub-  Subcei  cell Physical Failure  Physical Failure  Analysis (PFA)  Analysis (PFA) Root Cause Root Cause  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8b898323-172c-480d-96a9-8fced1109c53/8b898323-172c-480d-96a9-8fced1109c53.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=3f252f61a4747e04fd6a16f1bb00f331d38cebdf)
Delayering/Deprocessing

SEM

FIB

TEM

…

## Typical TEM/STEM Techniques 

![Energy Loss (eV)  EDS, EELS EDS,EELS  Image  Image  (Point, line scan, or mapping)  (Point, line scan, or mapping) (BF, DF, HRTEM,  (BF,DF,HRTEM.  Tomography Tomography  HAADF, HRSTEM,)  HAADF, HRSTEM,)  Diffraction (SADP,  Diffraction (SADP,  Nano-diff, CBED)  Nano-diff, CBED) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1e5a4c88-42b8-4035-b640-5807172387fa/1e5a4c88-42b8-4035-b640-5807172387fa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=7ccfe6a92969a9bf6f7fe47d894f54ec3af7bbc4)
## Beam-specimen interactions 

## §  Beam-specimen interactions 

![Incident Beam Incident Beam  X-rays  X-rays Backscattered ē Backscattered e  Auger e  Auger ē TEM  TEM Specimen Specimen  Elastically Scattered  Elastically Scattered   Elastically Scattered  Elastically Scattered  Electrons Incoherent Electrons Incoherent   Electrons Incoherent Electrons Incoherent  Elastically Scattered  Elastically Scattered   Elastically Scattered  Elastically Scattered  Electrons (Diffraction)  Electrons (Diffraction)  Electrons (Diffraction)  Electrons (Diffraction) Inelastically Scattered  Inelastically Scatte'red   Inelastically Scattered  Inelastically Scattered  Electrons (EELS) Electrons (EELS)   Electrons (EELS) Electrons (EELS)  Unscattered Electrons  Unscattered Electrons (Zero-Loss) (Zero-Loss)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b81618d3-8893-4dfe-889f-3e1a66f78a3a/b81618d3-8893-4dfe-889f-3e1a66f78a3a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=ac261b18ff35cb25dab9bd45a2e5b84a6d789987)
Inelastic incoherent    scattering (<1 degrees):    EELS   Coherent elastic scattering    (1-10 degrees): Diffraction     Incoherent elastic    scattering (higher degrees):    Mass-thickness\*

## Transmission Electron Microscopy 

## Advantage: 

l  High Spatial Resolution: \~0.1nm   l  Analysis of Crystal Defects: Dislocations, Stacking Faults, Twins  etc.   l  High Spatial Resolution Elemental and Chemical Analysis:  l  Good Elemental Sensitivitiy: 0.1wt% - 1wt%

## Disadvantage 

m  Difficult Sample Preparation: 10nm – 100nm thickness

## Transmission Electron Microscope 

![Electron Gun Electron Gun  Condenser Aperture Condenser Aperture   Condenser Lenses Condenser Lenses  Objective Aperture Objective Aperture   (EDS detector) (EDS detector)  TEM sample holder TEM sample holder   Objective Lenses Objective Lenses  Intermediate Lenses  Intermediate Lenses Projector lenses Projector lenses  Binoculars  (STEM detector) (STEM detector)  Imagerecording system  (EELS detector) (EELS detector)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/47c01fae-01fb-48a5-aaa2-86f6e0adde4d/47c01fae-01fb-48a5-aaa2-86f6e0adde4d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=651971b777a95b8ccf4bbedae63d49da93c84970)
•  TEM schematic:  Gun, lenses,  sample, detectors  (STEM, EDS, EELS)

## Elemental and Chemical Analysis 

## Inelastic scattering 

Incoming electrons ionize theatom(core-shell excitation), loses energy

![Auger  emiss.  SSSs  x-ray  ejected  energyloss  electron  electron  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4ec4f6fd-3920-4b07-8d7e-31106c77dce2/4ec4f6fd-3920-4b07-8d7e-31106c77dce2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=fe144889456777148f7287e508ea01b178cbbe3f)
![Incident e-beam  Backscattered  electrons   X-Rays  Secondary  electrons  Specimen  Elastically   Inelastically  scattered   scattered  electrons   electrons  Direct transmitted  e-beam  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/28dd39c5-a20d-478e-a3c7-1ffa63184a73/28dd39c5-a20d-478e-a3c7-1ffa63184a73.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=6be8fca32a51a5eefa6d7477de9480f6ef8bfb1e)
![Electron gun  Condensor aperture  (EDX  (EDX  detector)  detector) Specimen port  Intermediate aperture  Intermediatelens  Projectorlenses  Binoculars  rescentscreen  (EELS detector) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e0246677-d4cd-45e6-bd3f-1eeb1329bb8d/e0246677-d4cd-45e6-bd3f-1eeb1329bb8d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=c3ef519957240121346c32629e0968928f95542c)
•  Energy-Dispersive X-ray - EDX   •  Electron Energy Loss Spectroscopy - EELS

## Beam-specimen interactions 

## •  Beam-specimen interactions 

![Incident Beam IncidentBeam  X-rays  X-rays Backscattered ē Backscattered e  Auger é  Auger ē TEM  TEM Specimen  Specimen Elastically Scattered  Elastically Scattered   Elastically Scattered  Elastically Scattered  Electrons (Diffraction)  Electrons (Diffraction)  Electrons (Diffraction)  Electrons (Diffraction) Inelastically Scatte'red  Inelastically Scattered   Inelastically Scattered  Ihelastically Scattered  Electrons (EELS) Electrons (EELS)   Electrons (EELS) Electrons (EELS)  Unscattered Electrons Unscattered Electrons  (Zero-Loss) (Zero-Loss)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4282eabe-0572-4d16-8be2-da005506a41f/4282eabe-0572-4d16-8be2-da005506a41f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=6c01a79d30cd94d2631b285f85ff1a18622e19b1)
## X-Ray Production 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f2910592-21cf-400c-9b62-da1860931b19/f2910592-21cf-400c-9b62-da1860931b19.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=3b12c9d87958891bd1c9bdbf56069485f125862b)
X-ray energy is the difference  between 2 energy levels

![Beam  Beam  electron  electron b a K  L  M Beam  Beam  electron  electron  Ioses Ek  loses E K ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/494ad7f1-da5e-4e6e-b5b9-2156da45ed03/494ad7f1-da5e-4e6e-b5b9-2156da45ed03.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=500ff7ac8c004c262c4aeb9582fd6c29eea94034)
## X-Ray Detection 

![oetfee   Dewar Dewar  ORO  Electron  Electron  Trap Trap  SiLi SiLi  Window Window  Crystal Crystal  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/93d060bb-04e9-4832-9563-35c7ada3d57a/93d060bb-04e9-4832-9563-35c7ada3d57a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=9b9cb867075bb26c123b19462226c242d3a21d25)
EDS Detector

## X-Ray Detection 

![Silicon Crystal  1. Incident x-ray produces  a high-energy  a high-energy  photoelectron, when it  photoelectron, w  hits the crystal  hits the crystal 2. High-energy  2. High-energy  photoelectron knocks a  photoelectron kr  VB electron into  VB electron into CB,  leaving an intrins  leaving an intrinsic  hole.  hole. 3. On average 3.8eV to 3.9  3. On average 3.8e  eV are  dissipated per  V 3ra   diccinato  hole created. Particle1  4. It continues until it  losses all of its energy. •  Typical x-ray energy 4.5  keV (Ti k a ) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b83959cd-c805-4b41-9592-939476fc5cff/b83959cd-c805-4b41-9592-939476fc5cff.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=e88f5eee172546510c2a863474030f47d2485389)
## Interaction Volume 

![Incident e - Incident e  TEM Sample TEMSample  Bulk Si Sample Bulk Si Sample   X-Rays  X-Rays 100 nm  100 nm  Or less  or less High Spatial  High Spatial  Resolution  Resolution  in TEM inTEM  K x-rays  K X-rays L X-rays  L X-rays ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/91f5a775-0d58-4136-9c89-5d65da2332a8/91f5a775-0d58-4136-9c89-5d65da2332a8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=880a4d961c8060181a443026ed51c20bd8da29f9)
Scale in Microns

## X-Ray Yield 

w  = fraction of ionization events  producing characteristic x-rays   the rest produce Auger e –

•  w   increases with Z  ${\mathfrak{O}}_{\mathsf{K}}$    typical values are: 0.03 for carbon (12) K-series @ 0.3  keV 0.54 for germanium (32) K-series @  9.9 keV 0.96 for gold (79) K-series @ 67 keV X-ray production is inefficient for low Z lines  (e.g., O, N, C) since mostly Augers produced

•  w   for each shell:   $\mathfrak{O}_{\mathsf{K}},\mathfrak{O}_{\mathsf{L}},\mathfrak{O}_{\mathsf{M}}$  X-ray production is inefficient for L-shell and  M-shell ionizations since    ${\mathfrak{o}}_{\mathfrak{l}}$  and  ${\mathfrak{omega}}_{\mathtt{M}}$   always < 0.5: w L  = 0.36 for Au (79) w M  = 0.002 for Au (79)

![0.7  0.5  K Shell  0③  L Shell  0.1   M Shell  20   40   60   80   10:0  Atomic Number (Z)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a8f9140d-56e2-4558-beb0-ef5e67246ab8/a8f9140d-56e2-4558-beb0-ef5e67246ab8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=c889951d101d361fb56cabc559a2167a19af9251)
## EDS in TEM 

•  Spatial resolution –  2-20 nm (  $\mathbf{\mathfrak{10^{3}}}$    times better than SEM/EPMA)   •  Energy Resolution \~130-140 eV   •  Elemental detectability –  0.1 wt% - 1 wt%, depending on the specimen (\~same as  SEM/EDS)   •  Can use typical TEM specimens (t \~ 50-500 nm) –  EELS requires specimens < 20-30 nm   •  Good for High Z elements –  EELS is better at low Z elements

## EDS Detectors  

![Incidentbeam  Upperobjective  Bewindow   polepiece  SiLLi)  detector   DesiredX-ray  collection angleQ  -Specimen  Collimator  Lower objective  Transmitted  Undesired   electrons   polepiece  x-ray  collection angle  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1936b416-6c49-4662-ae6b-e7efe3b804de/1936b416-6c49-4662-ae6b-e7efe3b804de.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=d18e71de7b57865ee5d600cb3118db1afb10de29)
![-20degrees   Odegrees   +20degrees  beam   Incidentbeam  Det.3,4   Det.1,2   PNSensor SDD  4M）  12  10  0.8  0.6  04  Super-x  02   Cold trap  Si(Li) O.3 sr  30   -2O   -10   10   20   3D  Alpha tilt angle (degrees)   a. 4 Silicon Drift Detectors (SDD)  a. 4 Silicon Drift Detectors (SDD) -20 degrees   Odegrees   +20 degrees   b. > 0.9 srad (Solid Angle)/120   srad  (Solid Angle)/120  mm2detector area  mm2detector area SDD:(Silicon Drift Detectors)  SDD:( S ilicon  D rift  D etectors)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/adbcb94f-ae19-495e-910e-312ec7d2193e/adbcb94f-ae19-495e-910e-312ec7d2193e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=9834efa7b9d89a88510eb111bef7c6674e208425)
a. Single Si(Li) Detectors  b.  $\mathbf{\tilde{\Sigma}}_{\mathbf{0}.3}$   srad  (Solid Angle)/30  mm2detector area

•  Si (Li) detector   •  Si Drift detector   •  Multiple detectors

## Spectrum Imaging 

•  Combining STEM and EDS (Spectrum  Imaging) maging)

![Ba Ba+   +  Mg  BST-MgO thin-film on MgO  BST-MgO thin-film on MgO  Columnar growth with PLD Columnar growth with PLD  Ti  Ba Mg v a.   Sr HAADF HAADF   100 nm  HAADF HAADF   100nm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ef553d89-2bda-46fe-9101-1772a1d20b6b/ef553d89-2bda-46fe-9101-1772a1d20b6b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=99a62c59ba92d5974401a8125faff13f209cd7b9)
## Spectrum Imaging 

35 nm

•  STEM-EDS (Spectrum Imaging)

![Co 20nm  Fe Distribution of Fe, Co and  Distribution of Fe, Co and  Au in nano-particles. Au in nano-particles.  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f1e9cfcf-5570-42c3-ab35-fa67cfc6b40d/f1e9cfcf-5570-42c3-ab35-fa67cfc6b40d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=fbd09121e3e3c23ef1844cb54ea4a9fc81e02608)
\* EELS spectrum imaging will be available mid-2009

## Transmission Electron Microscopy (TEM) TEM and STEM 

![TEM  TEM  Scanning TEM (STEM) Scanning TEM (STEM)  TEM camera  TEM camera HAAD-STEM detector HAAD-STEM detector  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ddadbd7f-38b0-43a5-8d24-56e4dfa03eaf/ddadbd7f-38b0-43a5-8d24-56e4dfa03eaf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=4d85f37b2d531df0e1624c47c1117f1fb2aff4d9)
## Diffraction 

![ave2   Bragg's angle  Bragg’s angle wave1  incident   reflected  angle   angle  atomic  plane  M=2  atomic  plane  asine  ③1998  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/695ffe25-c3b1-46ed-86dd-119d2874553e/695ffe25-c3b1-46ed-86dd-119d2874553e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=767ff741452a00ae974e227f1755ccdc7d212aca)
D L = BC + BD = 2dsin q  = n l

Assuming: n=1, d = 2.5 Å For TEM at 200:   l  = 0.0251 Å

q 1 =0.29  o   à  Pretty small angle

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c3a48f04-0c98-446f-9de9-1ddc521de56e/c3a48f04-0c98-446f-9de9-1ddc521de56e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=3eb9314836d486d07c9486d1185ef14e4c4c4291)
## F. C. C. Crystal : [1 1 0] 

![z a y x [110] [110]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5878b076-b7da-403d-8f79-16a2f263ca86/5878b076-b7da-403d-8f79-16a2f263ca86.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=60c9aded19fdb7686cd2d979248e20f57020db70)
For cubic crystals, distance between planes:

$${\bf d}_{h k l}={\frac{\bf a}{\bf\Gamma(h^{2}+k^{2}+l^{2})^{1/2}}}$$
a – lattice parameter h, k, l – Miller Indices

## Diffraction: Si [110] 

For cubic crystals

$${\bf d}_{h k l}={\frac{\bf a}{\bf\Gamma(h^{2}+k^{2}+l^{2})^{1/2}}}$$
Si lattice parameter:  a = 0.5439 nm

![54.74  35.:6\*   35259  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2fbc6498-1448-4431-89b9-2fa3ba90ffc8/2fbc6498-1448-4431-89b9-2fa3ba90ffc8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=7e4e930be8e006cc0d8fb5766a8e15d4721198a5)
## d111 = 0.3140nm

![d331 = 0.1248nm  d 331  = 0.1248nm  d220 = 0.1923nm  d 220  = 0.1923nm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3ecc8cdb-6158-4a43-87f9-bda1f3b72f9b/3ecc8cdb-6158-4a43-87f9-bda1f3b72f9b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=80629b462495da0f2fc765625358fe32be714b69)
d200 = 0.2720nm

d

311  = 0.1640nm

## Diffraction 

![Zone Axis  Zone Axis [u v w]  [u v w] ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8b2526a5-c2a2-4217-ad56-e0882dc0a434/8b2526a5-c2a2-4217-ad56-e0882dc0a434.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=89447aeaaea82bb334cd0048038987a842386e9e)
![0.5 1/nm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d589554f-4dda-47b7-abcb-9fdd89a1bbad/d589554f-4dda-47b7-abcb-9fdd89a1bbad.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=0ad86bfbca1813f09855fb66851be1e10091f84e)
Zone axis

![2  3  1 q A B ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/be4f986f-3b20-4f97-aa09-67c0d3070da9/be4f986f-3b20-4f97-aa09-67c0d3070da9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=86c703e12ce18673ea1af9f2b0f918a837d442c0)
Lattice planes that satisfy:  $\mathbf{u}h+\mathbf{v}k+\mathbf{w}l=\mathbf{0}$

For Si [110] zone axis the planes {111}, {002}, {220}, {113}, …  meet that condition

## Electron Diffraction Pattern--Spot to Ring 

![(a)  (a)  （o>  (b)  (c) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d42e3527-19ad-4ab6-af32-090133a9bb3e/d42e3527-19ad-4ab6-af32-090133a9bb3e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=eef93abdbf06e28e6bdb62c98a317f1b4206af2a)
## Diffraction of Polycrystalline Material  

![Courtesy Dr. Jong-Shing Bow esy Dr. Jong-Shing Bow  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7bd87991-7ee1-410e-895b-eb4e0b9c7d8c/7bd87991-7ee1-410e-895b-eb4e0b9c7d8c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=359f51fa690ae892eae17090e91e5039bdc1fab2)
## Diffraction Patterns 

## Single Crystal 

## Polycrystalline Material 

## Amorphous Material 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bfd88d40-ba0f-4e2e-8154-fa79d185868c/bfd88d40-ba0f-4e2e-8154-fa79d185868c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=e7239f2a93b60782b5b3d33ecbff91e1a7e0c88f)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f03b549e-a7d5-482e-b780-d50b84d6c852/f03b549e-a7d5-482e-b780-d50b84d6c852.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=8f52e75c3d2a77fd6a5d86766ea79a10bcc856a4)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6252c10e-5b83-4c76-91fb-7bc3cfaf6b9e/6252c10e-5b83-4c76-91fb-7bc3cfaf6b9e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=eb42f2f6e549c46e392c8f6450cf48266a5db7db)
l  Each spot corresponds to  one set of  ( h k l ) crystal  planes of   ${\mathsf{d}}_{h k l}$   spacing.

l  Each ring corresponds to  one set of  ( h k l ) crystal  planes of  ${\mathsf{d}}_{h k l}$   spacing.

l  There is no defined d  spacing  è  diffuse ring.

## Objective System 

![> Forms Images  Ø  Forms Images •  Bright Field  Bright Field •  Dark Field  Dark Field •  HREM  HREM Sample  Sample Object Plane  Object Plane Ø > Forms Diffraction   Forms Diffraction Objective Lens  Objective Lens Back-Focal  Back-Focal Diffraction Diffraction  Plane  Plane Image Plane  Image Plane  Image  Image ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/07fd5cd2-ba59-4800-b358-aa5ea164bbb8/07fd5cd2-ba59-4800-b358-aa5ea164bbb8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=8b1b27c58bb9907c037d45c949ab95e3201dd1a0)
![Sample  Sample Objective Lens Objective Lens  Object  Object  Back-focal Plane Back-focal Plane  Object  Object   Plane  Plane Piane  Plane  Image Plane  Image Plane  Diffraction Diffraction  Imaging  Intermediate  Intermediate  Lens  Lens Object  Object   Object  Object  Image Plane Image Plane  Plane  Plane  Plane  Plane Projector  Projector  Lens  Lens Screen  Screen ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f00e61e7-f66d-407e-845d-7a8448473371/f00e61e7-f66d-407e-845d-7a8448473371.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=076fc3767846d48d286f7ab75422968822b7ef74)
## Contrast Mechanisms 

Ø  Mass-Thickness Contrast Ø  Diffraction Contrast Ø  Phase Contrast

## Typical TEM Image Contrast 

![Cu (29) Cu (29)  Ta (73)  Ta (73)  Low k  Low K W (74)  W (74)  SiO2  SiO 2 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9e005801-5a9e-4eec-923f-9fea14d8e68f/9e005801-5a9e-4eec-923f-9fea14d8e68f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=31c38d5dcf41d91c5ff05b577730e2243a64cce3)
![SiO2  SiO 2 Si(14) substrate Si(14) substrate  Si(14) substrate Si(14) substrate  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/210d7104-13dd-4615-973c-a5c1fd6bc0b0/210d7104-13dd-4615-973c-a5c1fd6bc0b0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=10e56fe71b642dfbb01c522c475c775c48d5cf88)
## OBJ Apertures and Contrast of TEM Images 

![Bright Field Bright Field  Dark Field Dark Field  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a8f207d1-1043-472f-86c2-3128cfe7b507/a8f207d1-1043-472f-86c2-3128cfe7b507.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=7eaa7a0547333cd02258d1181ecf503430a41150)
High Resolution (Phase Contrast)

## Imaging Mechanisms 

Ø

## Mass-Thickness Contrast 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2b1724ed-2617-42c0-9f05-7bd371168e97/2b1724ed-2617-42c0-9f05-7bd371168e97.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=1b982cc144203e5a1907a5ed816666627ab1c890)
•  Incoherent elastic  SC  scattering of electrons

![Higher  Higher  Lower Thick. .ower Thick   Higher Mass Thickness  • Objective  Objective  Lens  Lens • Objective  Objective  Aperture Aperture  • +  Image Plane Image Plane  Intensity Profile Intensity Profile  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/59ca920e-d37a-427c-9086-84efc37f8f01/59ca920e-d37a-427c-9086-84efc37f8f01.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=65e318c9b6ecb7656615fc5f320b1d02e46c0906)
Probability of elastic  FY  SC  scattering is a function of Z

As the thickness increases  AS  ea  elastic scattering increases

Most important for  noncrystalline (amorphous)  Y  Sa  samples

## Imaging Mechanisms Mass-Thickness Contrast 

Ø

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6f2f3f3d-0f36-4f77-984b-6ea1e20af385/6f2f3f3d-0f36-4f77-984b-6ea1e20af385.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=420e121cdb7791e925fcd714e727d2b02b7966f7)
![0.5pm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d5aa8205-2c46-45f4-a354-9060cc5a8a87/d5aa8205-2c46-45f4-a354-9060cc5a8a87.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=3060b58eade86a529f359fb338249d20d4b1d255)
Graphene (w/o Obj Ap.)

## Imaging Mechanisms 

Ø

## Diffraction Contrast 

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/83002a39-3eab-40ee-8c45-20a5f1769cf1/83002a39-3eab-40ee-8c45-20a5f1769cf1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=659a5a2ea0f8f04ac853c18693671e0668dad101)
![Random  Random  Zone Axis  Zone Axis Objective  Objective  Lens  Lens Objective  Objective  Aperture  Aperture Image Plane  Image Plane Intensity Profile  Intensity Profile ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/87442e57-7263-4686-8433-e2b8587747d6/87442e57-7263-4686-8433-e2b8587747d6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=064329543527c537592fe4113fab7ce74d96466c)
![101/nm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/51bd2ed2-8e30-40e3-b7bc-8ebd39904a16/51bd2ed2-8e30-40e3-b7bc-8ebd39904a16.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=7449f1a3189ed5bf85f13b97468f753159c591bb)
![101/nm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/be07af44-f045-4196-a617-26346b3aa4a0/be07af44-f045-4196-a617-26346b3aa4a0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=aff5527366e37c9e4535da7b66099cba16e91fd3)
Far from Zone Axis (No Diffraction)

Near Zone Axis (Diffraction)

•  Coherent elastic scattering  of electrons   •  Scattering occurs at  special (Bragg) angles   •  Most important for  crystalline samples   •  Useful for Dark Field  Imaging

## Image Contrast: Diffraction Conditions 

![T T ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/86c977dc-833a-4e20-88cc-20e11365e37e/86c977dc-833a-4e20-88cc-20e11365e37e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=11639732ef007eff615f1f4f107e8a5ecc6df6fe)
## Dark Field (DF) Images  

![50nm   50nm   50nm  50nm   50nm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/08d2b9cf-5a53-4fe7-8566-b68284ade8b0/08d2b9cf-5a53-4fe7-8566-b68284ade8b0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=07ab670daa6bb2e482af071dff1505318c9b40e9)
## Understanding TEM Contrast 

![SiO2  SiO 2  Cu (29) Cu (29)  Diffraction contrast  Diffraction contrast & Mass absorption  & Mass absorption   Ta (73)  Ta (73) contrast  contrast  Low K  Low K Mass absorption  Mass absorption contrast  contrast Si(14) substrate Si(14) substrate    Both Si substrate and  Both Si substrate and  silicide are dark:  silicide are dark:   00   W (74)  W (74)  SiO2  SiO 2 Mass absorption  Mass absorption  contrast (silicide) and  contrast (silicide) and  Diffraction contrast  Diffraction contrast  (Si sub) dominate. (Si sub) dominate.  Silicide and Si substrate can be  Silicide and Si substrate can be  separated, by "separating" mass  separated, by “separating” mass  absorption contrast and diffraction  absorption contrast and diffraction  contrast (How?) contrast (How?)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2247cadb-9de9-4d39-b29d-d8597997cf7d/2247cadb-9de9-4d39-b29d-d8597997cf7d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=be764fcf327e84333e16783b55d2e1efd53753d6)
## OBJ Apertures and Contrast of TEM Images 

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4ca4da43-65a7-4c9a-9001-831180a636a4/4ca4da43-65a7-4c9a-9001-831180a636a4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=9924764ec948fc1bee4e2d482c7e66d51522ebd1)
High Resolution (Phase Contrast)

## Imaging Mechanism 

![Ø  Phase Contrast Phase Contrast  Direct Beam  Direct Beam Sample  Sample AAA   Diffracted Beam  Diffracted Beam Phase Shift depends on:  Phase Shift depends on:  Thickness Thickness  Objective  Objective Diffraction plane  Diffraction plane Lens  Lens Defocus Defocus  C s ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b1e0eb95-df49-47dd-896a-fee6b288b3d1/b1e0eb95-df49-47dd-896a-fee6b288b3d1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=87db9430c5bf0ef5039e5dffa287100d31b94c09)
## Imaging Mechanisms 

Ø

## Phase Contrast 

•  High Resolution TEM   •  Forms images using  interference of multiple  beams.   •  Difficult to interpret  image directly without  simulation.

22  42

45  45

(uuru)

28  48

Thickness (nm)

51

![Defocus (nm) Defocus (nm)  -60  -60  -50 -50   -40 -40   -③0  -30  -20 -20   -10 -10   0 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b57ea0c0-9b8e-4f2a-b28e-96a890ccd9f0/b57ea0c0-9b8e-4f2a-b28e-96a890ccd9f0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=3f5ae0220c0887c3497e35f268c4f2dc95398432)
54

![57 60 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b06032a7-32df-4aa4-a537-e2b23763b2c1/b06032a7-32df-4aa4-a537-e2b23763b2c1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=2b0230bfe27caccd7eabf372d0fdb2597a8fbbbe)
## HREM Image — Semiconductor 

![Poly si  Poly Si Nitride  Nitride Oxide  Oxide <1 1 0> Si <1 1 0> Si  d d111 = 0.314 nm  111  = 0.314 nm 5 nm ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/650d1af8-ed3b-4017-a158-94c292bdfb10/650d1af8-ed3b-4017-a158-94c292bdfb10.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=98820d1c0256b45920302b2d60443779edac3bb7)
## Scanning TEM (STEM) 

![EDS  EDS  SrTiO3\*  SrTiO  \* 3 JSample  Sample HAADF  HAADF  HAADF - High Angle  F - High Angle   Detector Detector  Annular Dark Field ar Dark Field  B500C  BODDC  ADF – Annular Dark  Annular Dark   25000  ADF  ADF   20000  Detector Detector   15000  10000  BF – Bright Field right Field  SOOC  BF  EBF   2000   2100   2200   2300   2400   2500   2600   2700   2800  EELS EELS  Detector Detector   \*D.O. Klenov & S. Stemmer MST, v24, iss:6 pg: 660  \* D.O. Klenov & S. Stemmer MST, v24, iss:6 pg: 660 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/226656c1-5e65-45a1-b426-de9bc45b3744/226656c1-5e65-45a1-b426-de9bc45b3744.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=e0ae87201ebb16162dfdf4853f1671d7521cde84)
Field

## BF-TEM vs. HAADF-STEM vs. ADF-STEM 

![BF-TEM BF-TEM   HAADF-STEM HAADF-STEM   ADF-STEM ADF-STEM  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/959c72b6-43ef-4327-8856-10c9bf4a9716/959c72b6-43ef-4327-8856-10c9bf4a9716.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=18a8ab050fd223e6a6056f3a0a7586c227bab23c)
•  ADF sensitive to diffraction contrast and thus grain orientation •  Polycrystalline phase:  Speckled with bright contrast from micro-grains •  Amorphous phase:  Homogeneous appearance due to absence of  diffracting grains

## Scanning TEM (STEM) 

•  Advantages: •  Z-Contrast imaging (fast qualitative data) •  Directly interpretable image (No simulation needed) •  Spectrum imaging •  Almost no chromatic aberration (better for imaging thicker samples)   •  Disadvantages •  Extensive alignment •  Sample damage

## Z-Contrast Imaging 

•  STEM (Imaging)

![HAADF HAADF   HAADF HAADF  Titanium Oxide  Titanium Oxide  Nanotubes with  Nanotubes with  Sputtered Pt Sputtered Pt  BF BF  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/450015c7-a048-42f5-849e-15acc873e83e/450015c7-a048-42f5-849e-15acc873e83e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=314ca552914b7545e4a96fe2a2f71f7a444df643)
\* Lee, W.J., Smyrl, W.H. et al. Journal of Electrochemical Society, v 155, n 9, 2008 p B915    (Ozan Ugurlu)

## Comparison of 10nm Technology 

![a) A11 Bionic   (b) Exynos8895   (a) A11 Bionic   (b) Exynos8895  100nm  P-Fins   N-Fins   100 nm P-Fins   N-Fins   50nm   50nm  NOASDCGeHTaW  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/93c98210-c3c2-4814-bf8b-7533d7cc9bab/93c98210-c3c2-4814-bf8b-7533d7cc9bab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=f3dd70b3729bbfbb5e221856a3e380e8d8998072)
•  EDX analysis of leading edge technology

courtesy of MSS Co.

## Elemental and Chemical Analysis 

## Inelastic scattering 

Incoming electrons ionize theatom(core-shell excitation), loses energy

![Auger  ★emiss.  SSss  x-ray  ejected  energyloss  electron  electron  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5eebd1f9-578c-4d23-80ed-dc7166af1bd6/5eebd1f9-578c-4d23-80ed-dc7166af1bd6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=0549129fd00ad8682150afd5a588780a9a3e225b)
![Incident e-beam  Backscattered  electrons   X-Rays  Secondary  electrons  Specimen  Elastically   Inelastically  scattered   scattered  electrons   electrons  Direct transmitted  e-beam  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e802a8d5-c2b3-4381-9fe5-bcaaecac595d/e802a8d5-c2b3-4381-9fe5-bcaaecac595d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=6ec627800721f667046e77dfb0dd88148393b8a8)
![Electron gun  Condensor aperture  (EDX  (EDX  detector)  detector) Specimen port  Intermediate aperture  Intermediatelens  Projectorlenses  Binoculars  rescentscreen  (EELS detector) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/115f9f92-51b6-4715-a50f-74406ac66134/115f9f92-51b6-4715-a50f-74406ac66134.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=3f2c53c97d2ac8181ff91b41fc1235d7d0d0eb51)
•  Energy-Dispersive X-ray - EDX   •  Electron Energy Loss Spectroscopy - EELS

## Beam-specimen interactions 

## •  Beam-specimen interactions 

![Incident Beam IncidentBeam  X-rays  X-rays Backscattered ē Backscattered e  Auger é  Auger ē TEM  TEM Specimen  Specimen Elastically Scattered  Elastically Scattered   Elastically Scattered  Elastically Scattered  Electrons (Diffraction)  Electrons (Diffraction)  Electrons (Diffraction)  Electrons (Diffraction) Inelastically Scatte'red  Inelastically Scattered   Inelastically Scattered  Ihelastically Scattered  Electrons (EELS) Electrons (EELS)   Electrons (EELS) Electrons (EELS)  Unscattered Electrons Unscattered Electrons  (Zero-Loss) (Zero-Loss)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/22a20680-fa96-479a-9498-fe62f40092c3/22a20680-fa96-479a-9498-fe62f40092c3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=d0dcea95c38f9615fd4ce1609bd3043d81a6db9e)
## X-Ray Production 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c923dd2d-6300-41d0-8dbb-98ed183635ba/c923dd2d-6300-41d0-8dbb-98ed183635ba.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=eabac94ae250cf398feb2fe32885b99854533b29)
X-ray energy is the difference  between 2 energy levels

![Beam  Beam  electron  electron b a K  L  M Beam  Beam  electron  electron  Ioses Ek  loses E K ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/26d2696e-2a58-484a-8c26-62cf69b9c579/26d2696e-2a58-484a-8c26-62cf69b9c579.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=42d27e9290655ac37831f9cd70e07fca019965e3)
## X-Ray Detection 

![oetfee   Dewar Dewar  ORO  Electron  Electron  Trap Trap  SiLi SiLi  Window Window  Crystal Crystal  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/63474000-c085-48f6-b447-32d1a77a21eb/63474000-c085-48f6-b447-32d1a77a21eb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=dc8e55cea07985c65131f5fc591b4d40f8a4e6e8)
EDS Detector

## X-Ray Detection 

![Silicon Crystal  1. Incident x-ray produces  a high-energy  a high-energy  photoelectron, when it  photoelectron, w  hits the crystal  hits the crystal 2. High-energy  2. High-energy  photoelectron knocks a  photoelectron kr  VB electron into  VB electron into CB,  leaving an intrins  leaving an intrinsic  hole.  hole. 3. On average 3.8eV to 3.9  3. On average 3.8e  eV are  dissipated per  V 3ra   diccinato  hole created. Particle1  4. It continues until it  losses all of its energy. •  Typical x-ray energy 4.5  keV (Ti k a ) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8ed7760a-4a07-4e04-ab67-138d56af51c2/8ed7760a-4a07-4e04-ab67-138d56af51c2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=2148ed6f38b3b6ac0d3157083bf5fe391c7c52dd)
## Interaction Volume 

![Incident e - Incident e  TEM Sample TEMSample  Bulk Si Sample Bulk Si Sample   X-Rays  X-Rays 100 nm  100 nm  Or less  or less High Spatial  High Spatial  Resolution  Resolution  in TEM inTEM  K x-rays  K X-rays L X-rays  L X-rays ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1150146b-ef93-4f0c-a842-6cbad8127705/1150146b-ef93-4f0c-a842-6cbad8127705.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=8aa69119ab53774b08186fc18937ca07edc8842b)
Scale in Microns

## X-Ray Yield 

w  = fraction of ionization events  producing characteristic x-rays   the rest produce Auger e –

•  w   increases with Z  ${\mathfrak{O}}_{\mathsf{K}}$    typical values are: 0.03 for carbon (12) K-series @ 0.3  keV 0.54 for germanium (32) K-series @  9.9 keV 0.96 for gold (79) K-series @ 67 keV X-ray production is inefficient for low Z lines  (e.g., O, N, C) since mostly Augers produced

•  w   for each shell:   $\mathfrak{O}_{\mathsf{K}},\mathfrak{O}_{\mathsf{L}},\mathfrak{O}_{\mathsf{M}}$  X-ray production is inefficient for L-shell and  M-shell ionizations since    ${\mathfrak{o}}_{\mathfrak{l}}$  and  ${\mathfrak{omega}}_{\mathtt{M}}$   always < 0.5: w L  = 0.36 for Au (79) w M  = 0.002 for Au (79)

![0.7  0.5  K Shell  0③  L Shell  0.1   M Shell  20   40   60   80   10:0  Atomic Number (Z)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c5862dfc-5f5c-4780-b25e-d24739e563ff/c5862dfc-5f5c-4780-b25e-d24739e563ff.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=2c7b101e00a705e00839b6858f472d95adcdd5bd)
## EDS in TEM 

•  Spatial resolution –  2-20 nm (  $\mathbf{\mathfrak{10^{3}}}$    times better than SEM/EPMA)   •  Energy Resolution \~130-140 eV   •  Elemental detectability –  0.1 wt% - 1 wt%, depending on the specimen (\~same as  SEM/EDS)   •  Can use typical TEM specimens (t \~ 50-500 nm) –  EELS requires specimens < 20-30 nm   •  Good for High Z elements –  EELS is better at low Z elements

## EDS Detectors  

![Incidentbeam  Upperobjective  Bewindow   polepiece  SiLi)  detector   DesiredX-ray  collection angleQ  Specimen  Collimator  Lowerobjective  Transmitted  polepiece  Undesired   electrons  X-ray  collection angle  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4abfd425-82bb-42ff-a47d-90ea38482d07/4abfd425-82bb-42ff-a47d-90ea38482d07.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=f46010f36da9f647a440b6784ed8d0c1423281e9)
a. Single Si(Li) Detectors  b.  $\mathbf{\tilde{\Sigma}}_{\mathbf{0}.3}$   srad  (Solid Angle)/30  mm2detector area

![-20 degrees   0 degrees   +20 degrees  beam   Incidentbeam  Det.3,4   Det.1,2   PNSensor SDD  4M）  12  0.8  06  mfeedth  04  Super-x  0.2   Cold trap  Si(Li) O.3 sr  30   -20   -10   20   39   Alpha tilt angle (degrees)   a. 4 Silicon Drift Detectors (SDD) a. 4 Silicon Drift Detectors (SDD)  -20 degrees   0 degrees   +20 degrees   b. > 0.9 srad (Solid Angle)/120   srad  (Solid Angle)/120  mm2detector area  mm2detector area SDD:(Silicon Drift Detectors)  SDD:( S ilicon  D rift  D etectors)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1e9a2ed3-fd21-4305-ae82-d84a730f9ab3/1e9a2ed3-fd21-4305-ae82-d84a730f9ab3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=251f219b7c9b685eca315b4e1f9e1ca109028f36)
•  Si (Li) detector   •  Si Drift detector   •  Multiple detectors

## Spectrum Imaging 

•  Combining STEM and EDS (Spectrum  Imaging) maging)

![Ba Ba+   +  Mg  BST-MgO thin-film on MgO  BST-MgO thin-film on MgO  Columnar growth with PLD Columnar growth with PLD  Ti  Ba Mg v a.   Sr HAADF HAADF   100 nm  HAADF HAADF   100nm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a8ecbba4-8cbd-4607-a94d-d459316eb2a9/a8ecbba4-8cbd-4607-a94d-d459316eb2a9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=c942a7da58e455f60c941ed381d2d330e7ed1e3c)
## Spectrum Imaging 

35 nm

•  STEM-EDS (Spectrum Imaging)

![Co 20nm  Fe Distribution of Fe, Co and  Distribution of Fe, Co and  Au in nano-particles. Au in nano-particles.  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b5e5ff35-f0c1-4578-b3d1-63645cf28257/b5e5ff35-f0c1-4578-b3d1-63645cf28257.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=0444f7ba73616b50eedab24e197e995098108ea5)
\* EELS spectrum imaging will be available mid-2009

## Comparison of 10nm Technology 

![a) A11 Bionic   (b) Exynos8895   (a) A11 Bionic   (b) Exynos8895  100nm  P-Fins   N-Fins   100 nm P-Fins   N-Fins   50nm   50nm  NOASDCGeHTaW  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/828422bc-3cbe-40b8-9551-8440651869c9/828422bc-3cbe-40b8-9551-8440651869c9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215613%3B1743219213&q-key-time=1743215613%3B1743219213&q-header-list=host&q-url-param-list=&q-signature=b38b19194948b4f75addf7deeb38fc07a53d4f57)
•  EDX analysis of leading edge technology

courtesy of MSS Co.

