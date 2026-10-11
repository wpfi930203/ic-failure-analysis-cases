---
title: "tut-3.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_b4219cb4ff0b36195b98515284535b0e7295230462135641
file_size: 19548426
---

Tutorial:

## High-Resolution Non-Destructive  

Defect Localization

![FraunhoferIMWS  Team Non-Destructive  Defect Localization  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fd0c79e9-cb71-40c5-b882-640768f5fc35/fd0c79e9-cb71-40c5-b882-640768f5fc35.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=9ca02a57669f36bf4620980c6fff30e80bc61003)
## Dr. Sebastian Brand 

Dept. Electronic Materials and Components Fraunhofer IMWS , Germany

www.imws.fraunhofer.de/ndl

## Outline 

Background and Motivation

##   Acoustic Microscopy 

The acoustic Transducer, its Selection and Focusing    Physical Fundamentals and Contrast Mechanism   Machine Learning based Signal Analysis for Defect Identification   Case Studies (SAM  $^+$   GHz-SAM)

##   Lock-In Thermography 

Physical Fundamentals and Contrast Mechanism     Temperature Measurements     The LIT Technique and Application Approaches in 2D- and 3D-LIT     Case Studies     Machine Learning based Signal Analysis for Defect Identification

## Background & Motivation for NDL 

Technology Development:  Material interaction and behavior   Failure Analysis:  Defect localization without part alteration   $\Rightarrow$  root cause analysis   Quality Assessment:  high coverage  high reliability and premium quality

![89C51SND1-EL  SAMPLES  0140A00657F  1o0nm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e5ea6663-6cce-4fdf-9783-32f3acc5a689/e5ea6663-6cce-4fdf-9783-32f3acc5a689.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=6b3888bc41d903eea158ce899649e1509d357b69)
Challenge:  increasing integration density  reduction in feature dimension  high  resolution and sensitivity requirements

##   Microscopic Techniques with high Sensitivity 

![Physical  Physical  Defect  Defect  Characterization  Characterization Localization  Localization Electrical  Electrical  Active Methods  Active Methods  Passive Methods  Passive Methods Characterization  Characterization  High-Resolution  High-Resolution  techniques requiring  techniquesrequiring  preparation  preparation   SEM  SEM   Electrical  Electrical  measurements  measurements   Optical (PEM,EMI)  Optical (PEM, EMI)    Ultrasonics UItrasonics     TEN  TEM   Curve tracing  Curve tracing   Magnetic (MCI)  Magnetic (MCI)    X-Ray  X-Ray    SIMS  SIMS   ,Memory Bitmap'  „Memory Bitmap“   Thermal (LIT)  Thermal (LIT)    Light  Light     …   Logic diagnostics  Logic diagnostics  Microscopy  Microscopy Contrast Mechanisms according to Nature of Defect Contrast Mechanisms according to Nature of Defect  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/313c13a1-00dd-4eab-9be9-ba0d665c22f3/313c13a1-00dd-4eab-9be9-ba0d665c22f3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=f65c994e7684f5285baf8898544fada1b84513e9)
Background & Motivation for NDL

## Defect Localization by 

— Scanning Acoustic Microscopy —

(SAM)

## What can Acoustic Microscopy do? 

It allows to „look“ inside a sample without destructive preparation…

![40un  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/58f05d7d-a4a6-46d5-92ec-922c46b0b559/58f05d7d-a4a6-46d5-92ec-922c46b0b559.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=4adcc9cc231422a2ecd4ebd8b574d3d992dc297d)
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e374464f-6f10-493d-88ef-d606795869b0/e374464f-6f10-493d-88ef-d606795869b0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=6c5ea2acc0fb6da083fe75f5bcd898d7852fe046)
6

## Fundamentals of Acoustic Inspection 

“Acoustic Inspection submits mechanical waves (in elastic regime) into a specimen where they  interact with its structure and records the echoes that are emitted to the receiver”

Elastic/Acoustic Wave: Pressure wave, caused by alternating variation of density and pressure

|Infrasonic|Audible sound|Ultrasonic|Hypersonic|
|---|---|---|---|


Propagates in solids, fluids and gases      Does  not  propagate in vacuum !!     In fluids and gases only longitudinal (compressional) waves     In solids also shear wave modes

## Fundamentals of Acoustic Inspection 

![C  CG  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ed9e4968-4013-457f-9571-2a6028e43e4c/ed9e4968-4013-457f-9571-2a6028e43e4c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=f6ac38698cc96964ea4495c2e13bc690fce3e5a4)
## Specific Abilities of Acoustic Waves: 

penetrate  opaque materials    non-destructivity     reflected  on boundaries    detection/ analysis of   hidden structures     time-resolved    spatial resolution (3D)     Can be  focused    high resolution     scattered  on particles    material   characterization

## Example for Application in µ-Electronics: 

![Underfill  Misshapen  delam  bumps  Shorts between  bumps  Substrate  Delam  Voids in the underfill  Bump fracture/fatigue  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/14247fee-28df-4042-9baf-86f9e14dba62/14247fee-28df-4042-9baf-86f9e14dba62.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=ed27827da101b9de83fd50a4a89f9c08b145f026)
## Working Principle of SAM 

![Pulser- /  Pulser- / Receiver + Digitize  Receiver + Digitizer Signal Generator  Signal Generator z   Transducer Transducer   x · Transmits & receives acoustic signals    Transmits & receives acoustic signals   Pulser/ Receiver Unit Pulser/ Receiver Unit   y · Generates pulse    Generates pulse · Amplifies received signal    Amplifies received signal   A/D-Converter A/D-Converter  · Digitizes signal    Digitizes signal   3-Axis Scanner 3-Axis Scanner   water container  water container · Scans transducer    Scans transducer  Transducer  Transducer 3-Axis Scanner  3-Axis Scanner 10 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7e46bb1e-2c34-4204-adfa-ffc2ca1674dc/7e46bb1e-2c34-4204-adfa-ffc2ca1674dc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=068d3c518e88d7379b3eac01df14cd340a475364)
## Working Principle of SAM 

power amp

Method: Method:

Focused acoustic probe is scanned across the sample @each scan position acoustic signal emitted into

![sample    Received echoes analyzed for imaging by Dr.Sebastian Brand,  FraunhoferIMws,  Halle, Germany  Cu-metallization  Cu-metallization  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dbcbb32f-979e-461c-8618-828f618be9ef/dbcbb32f-979e-461c-8618-828f618be9ef.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=49d761593de4a5d06a3b874a0eb130eff91d653e)
![Interface ,1""  Interface „1“ Interface ,2"  Interface „2“ Interface ,3"  Interface „3“ 6.8   6.9   ?1   7.2   73   7.5  t[us]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/48a70a99-c0bf-4282-9df4-b6ab22225203/48a70a99-c0bf-4282-9df4-b6ab22225203.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=0d6092b607c28397d9cac46126ac56152fbe57da)
received acoustic signal

11

## Application Example 

Imaging of small-scale defects  in a bonded wafer pair

![200  2mm-200gm  2009  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/928086bd-2446-44ff-88ef-2c86906cf540/928086bd-2446-44ff-88ef-2c86906cf540.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=2198507855b729a28d0813231f8f79934cba5b1e)
12

## The focused acoustic Probe 

Acoustic Transducer used for generation of an ultrasonic wave (and for reception)

![Ccccc<<<:  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ddb4b697-c5d8-4b3b-bfca-10866d723c85/ddb4b697-c5d8-4b3b-bfca-10866d723c85.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=dfa9824e7f9d1e40d9c481cd904a045d8f3393b6)
## Ultrasonic Transducer 

## Excitation of acoustic Wave: Piezo Effect 

Acoustic Wave:  alternating variation of pressure and density   Excited:  through expansion or displacement of a body   Equipment:  voice coils, whistles    up to kHz range only

Piezo-Materials (ceramics, crystals, polymers used in SAM)

## Piezo Effect: 

![Force Force  el.Voltage el.Voltage  Force Force  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d3341c83-b76c-4bd6-a52b-a3b21513f6a7/d3341c83-b76c-4bd6-a52b-a3b21513f6a7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=15e8ed0cb38d3ce09d9beb84d5f4ee4a56a56e56)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2ab27a1f-400a-4ea4-b2a9-05daedc9f3a0/2ab27a1f-400a-4ea4-b2a9-05daedc9f3a0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=c537f79b8d0fbb563a86ec05505452f576fe26a7)
Force  leads to  displacement  of  charge  carriers,  $\Rightarrow$  separation  resulting in  el. voltage  on surfaces   Reversible :  Voltage  results in  displacement   density variation    $\Rightarrow$  pressure variation

picture sources: https://de.wikipedia.org/wiki/Piezoelektrizitaet ; https://en.wikipedia.org/wiki/Piezoelectricity

## The Acoustic Transducer 

Has specific parameters    is core element of acoustic inspection tool Consists of a piezo actor, backing and delay line

Specific Parameters:

Geometry (single element, array)   Power (size, thickness of the piezo element)   Frequency (wavelength   resolution)   Bandwidth (transfer function)   Aperture (flat, curved, array, with lens)

![piezo  piezo iens  lens ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2b607186-9dbc-49b4-bf53-1e0e269e2984/2b607186-9dbc-49b4-bf53-1e0e269e2984.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=120c0c9d3d89c2a0c09a7a42eb7676bc833c051e)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7c0591fc-3116-4232-941d-4f2b177d9400/7c0591fc-3116-4232-941d-4f2b177d9400.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=ccf30650a0bdcd2a4ebc80d31a2f208f3f12acb2)
## The Acoustic Transducer 

## Single-Element – focused by acoustic lens 

## Phased Array – el. Focused 

Wavelets are transmitted with mech. delays  in phase   Lens Parameters: ROC, Aperture angle

Wavelets are transmitted with el. delays    phase shifts

![focal plane  focal plane ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/84e1e6f8-e7a6-4b65-95a2-aba58ead85b7/84e1e6f8-e7a6-4b65-95a2-aba58ead85b7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=686a5dcd34250b4f1aa093a4c2eea1e5da2efc5d)
![multiple piezo - elements multiple piezo - elements  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ba7830b3-cc00-491b-a397-c68b417a3164/ba7830b3-cc00-491b-a397-c68b417a3164.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=300f9cf9f113db99d38fdc754eaa327f7b7cfa99)
## Wavelength and Resolution 

resolution  resolution wavelengt  wavelength wave velo  wave velocity frequency  frequency aadiutsref r  aperture radius radius of  curvature curvature

![10 10<  2  Raperture!  R  ：  𝑤  :  aperture ROC  ROC  𝜆  :  𝜐  :  c=1500m/s  c=1500 m/s  half aperture  half aperture    𝑓 :  wavelength [um] wnlubui   c= 3500 m/s c= 6000 m/s  RSC:  R  :  c= 9000 m/s  Focal Plane  Focal Plane  a ROC: 1 10 10  𝜆 W = 0.61  𝑤= 0.61  N.A.  𝑁. 𝐴. 𝜐 𝜆=  𝑓 100  10 0  107  10 1  10Ｚ  10 2  10 10  3  N.A.:  𝑁. 𝐴. =  𝑅 aperture  𝑎𝑝𝑒𝑟𝑡𝑢𝑟𝑒 = sin 𝜑 sin Phalf aperture  frequency [MHz]  frequency [MHz]  ROC  𝑅𝑂𝐶  ℎ𝑎𝑙𝑓 𝑎𝑝𝑒𝑟𝑡𝑢𝑟𝑒 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/feb9b498-9631-43ba-bbcc-2c2a5f9fef43/feb9b498-9631-43ba-bbcc-2c2a5f9fef43.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=6a4a5db19a91283e23c1bc15aa34f3c1b8528388)
Resolution dependent on wave velocity, frequency and numerical aperture of the lens

## Focusing Acoustic Waves 

## Focusing by acoustic Lens 

Focusing defined by  numerical  aperture  (N.A.) of lens     Opening angle  narrows focal spot  increases resolution     Radius of Curvature    places focal  spot (notice spherical aberration)     Refractive index  of lens material

![ROC ROC  ϕ Focal Plane Focal Plane  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4fb444a1-5f71-4ac6-bbbb-a86690dac084/4fb444a1-5f71-4ac6-bbbb-a86690dac084.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=161f3daea8b1303ee5057c82af869e228a59c0e0)
## Tuning the Transducer Aperture 

Animation : sound intensity  $\Rightarrow$  as function  $\Rightarrow$  N.A. and lens contour   Focal spot narrows  in lateral and axial extent, but  stays at equal distance

![ROC ϕ FocalPlane  Focal Plane ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d3a59995-c6af-4568-bc69-1dc79e40fb2c/d3a59995-c6af-4568-bc69-1dc79e40fb2c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=5cbbe320ba64e710f3e34174dac75bd1f1164999)
Adjustment of the Lens Opening Angle

![19 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/068fb794-1a85-44f9-b694-391a7f989f30/068fb794-1a85-44f9-b694-391a7f989f30.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=55dbe5c733306aed0708c9efa9b29c5825493cb1)
## Tuning the Transducer Aperture 

Animation:  sound intensity as function of aperture and lens contour   Focal spot moves  along depth-axis, but remain in  equal shape

![ROC ϕ Focal Plane  Focal Plane ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4a9b2aa7-bf2e-401b-9579-db0ba504e1fa/4a9b2aa7-bf2e-401b-9579-db0ba504e1fa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=8feba387f8b08388a806614e8ef7bcb6a67eef6d)
Adjustment of the Lens ROC

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7e45b487-f261-4a1b-b2d9-3a8862b6e83c/7e45b487-f261-4a1b-b2d9-3a8862b6e83c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=d1da0525e36652bdb8808e4851dc2bb2d767bc16)
## Focusing sound into solid Materials 

Large differences in wave propagation velocities     Large refractive indices  low aberrations     High reflectivity  small signals     Curved wave front  Angular incidence  lateral wave modes

## Focusing in SAM can be difficult 

![water  water  SoundIntensityFields  Sound Intensity Fields Si behind a layer of water  Si behind a layer of water Acoustic Lens  Acoustic Lens Acoustic Lens  Acoustic Lens Si-die  Si-die water  water water  water  Focus of Sound Beam  Focus of Sound Beam 21 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8811ddcb-3026-4c56-b9b7-a93cd4965c8b/8811ddcb-3026-4c56-b9b7-a93cd4965c8b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=23150a2a565db42b77bbd7f1533a0e9638858c37)
![Lens  Lens  Si-die  Si-die tituteor   anicsofMaterials IW  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9f9bf526-e2d2-4e3b-b7e4-924813ef21f8/9f9bf526-e2d2-4e3b-b7e4-924813ef21f8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=fdefac4cef474d9b9c042dd0b56460f773590700)
## Propagation of Acoustic Waves 

Acoustic Transducer used for generation of an ultrasonic wave (and for reception)

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/37cdb832-1721-48c1-9d39-d3d217606a01/37cdb832-1721-48c1-9d39-d3d217606a01.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=a8b650680e29a7307e34b410189892029b98aa54)
## Acoustic Wave Generation 

##   Excitation of a periodic variation of pressure and density 

Equilibrium p=p 0 , ρ=ρ 0

Distortion acts on volume  (Pressure increase)

Distortion is removed

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bebe511e-d741-4625-9e16-dea0fc763297/bebe511e-d741-4625-9e16-dea0fc763297.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=3e618b5ea1f3dd829624955208c16219803346f2)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f682e606-d030-4eea-8826-8108f32958c2/f682e606-d030-4eea-8826-8108f32958c2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=840eb73c9f4c7707773a3bd167b73c0ba5648a53)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3bda6c72-eb21-4303-9e3d-32d2f5b0b43a/3bda6c72-eb21-4303-9e3d-32d2f5b0b43a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=cfb8c52613a6974aec153d19f8e30d9bfa80335b)
p= p 0  + p S ρ= ρ 0  + ρ S

p= p 0  - p S ρ= ρ 0  - ρ S

Mass increase by Pressure and  Density increase in volume - negative pressure outside

Mass streams out of the  volume,  inertia   overpressure outside volume

## Displacement as Result of Force 

Newtons 2. Law :    $\rho\frac{\partial^{2}\xi}{\partial t^{2}}\!=\!\frac{\partial\sigma_{s}}{\partial x}$

Hooke‘s Law

:

$$\sigma_{s}=\mu\frac{\partial\xi}{\partial x}$$
Wave eqn. (1-D) :

$$\rho\frac{\partial^{2}\xi}{\partial t^{2}}=\mu\frac{\partial^{2}\xi}{\partial x^{2}}$$
![Input  Input  Output  Output System System  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2e3c14ae-a6ac-453e-a5f3-6086653bbab3/2e3c14ae-a6ac-453e-a5f3-6086653bbab3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=d8ebb7173c38ef82c1ff1be91920e1ef8ec0fc93)
Harmonic Solution :   $\xi=\xi_{0}e^{j(\omega t\pm k x)}$

![ξ sheared volume sheared volume  x ξ  - Displacement  - Displacement σ        - Shear Force - Shear Force  µ  - Shear Modulus  - Shear Modulus   - Density  - Density ω   - angular Frequency  - angular Frequency t           - Time  - Time X, y, z - spatial coordinates  x, y, z - spatial coordinates ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/830abe9b-eec1-4f79-a81a-1cc610cc2904/830abe9b-eec1-4f79-a81a-1cc610cc2904.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=8594c06c7c7320714355b93375c7185a2f81377e)
## Wave Generation and Propagation 

## Newtons 2 nd   Law:  

States that the force applied to an object is directly proportional to the acceleration  it experiences with respect to its mass.

## Hooke’s Law:  

It states that within an elastic limit, the deformation of a material is directly  proportional to the force applied to it according to  $\mathsf{F}=\mathsf{k x},$  , where F: force, k: elastic  parameter,  x: displacement.

## Wave Equation:  

States that the second derivative of displacement with respect to space and time  equals the product of elasticity and mass density, reflecting the balance between  inertia and elasticity in wave motion.

## Wave Propagation: Harmonic Excitation 

Wave propagation : (Sher mode)

ଶ

𝜌𝜔

ଶ

= 𝜇𝑘

𝜔 ଶ

= 𝜇

𝑘 ଶ

𝜌

Velocity of the Mode :

$$v={\frac{\omega}{k}}\ \ ={\sqrt{\frac{\mu}{\rho}}}$$
ξ  - Displacement   σ        - Shear Force   µ  - Shear Modulus     - Density   ω   - angular Frequency   t           - Time   x, y, z - spatial coordinates

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e01ba42e-8809-4bbc-87cf-1a89f5c295e0/e01ba42e-8809-4bbc-87cf-1a89f5c295e0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=a10d2e55d01e7ff6166d9e5bdc30c0b899645ecd)
Velocity of the  Shear Mode

## Velocity of the  Compressional Mode 

$$v_{s}={\sqrt{\frac{c_{44}}{\rho}}}$$
$$v_{l}=\sqrt{\frac{c_{11}}{\rho}}$$
Fluids and Gases only support Compressional Modes

Solids also support Transverse and combined Modes

$$\upsilon=\frac{\omega}{k}=2\pi f\frac{\lambda}{2\pi}=2\pi f\frac{\upsilon}{2\pi f}$$
## Sound Wave Generation and Propagation 

![Longitudinal Mode  Longitudinal Mode  Transverse Mode Transverse Mode  Direction displacement:  Direction displacement: Direction of Wave propagation: irection of Wave propagation:  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/022c5232-9b2a-457b-89d7-b8bd99159030/022c5232-9b2a-457b-89d7-b8bd99159030.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=52c452c68087467c26e88bf50d830fcd4410b563)
Rayleigh Wave:  Surface Acoustic Wave with longitudinal and transverse components.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/714adef2-dcb9-40f6-b385-21f1ef8987d4/714adef2-dcb9-40f6-b385-21f1ef8987d4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=299dc6fe1f1f43c94316110ee6e64121dfb4f019)
27

## Wave-Sample Interaction  

The acoustic wave interacts with the samples internal structure and objects

![Acoustic Wave interacting  Acoustic Wave interac  with objects in sample  with objects in sample 28  28 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b1b96a9d-3a2e-445c-b8f8-2e3d603b8355/b1b96a9d-3a2e-445c-b8f8-2e3d603b8355.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=bd11a4a0e6d58998c4243a476073f83af05c0521)
## Behavior on Material Interfaces 

## Z = Acoustic Impedance (mode specific) 

![v 1 NN  v 2 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c5d444df-6673-4f51-b7e4-268e3d6ce93b/c5d444df-6673-4f51-b7e4-268e3d6ce93b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=dfb2dfd794fd9f0462959809ec7479b344e8f35e)
incident wave component

$Z=\rho\cdot v=\sqrt{\rho\,c_{i j}}=\sigma\frac{\partial\xi}{\partial t} $   $v={\sqrt{\frac{c_{i j}}{\rho}}}$

reflected wave component:   $R(\mathbf{90^{\circ}})={\frac{\mathbf{Z}_{2}-\mathbf{Z}_{1}}{\mathbf{Z}_{1}+\mathbf{Z}_{2}}}$

transmitted wave component:

$$T(90^{\circ})={\frac{2Z_{1}}{Z_{1}+Z_{2}}}$$
Mode - converted component (excitation of additional wave modes, depending on  angle of incidence and elastic material properties)

Snellius‘ Law :   $\frac{\sin(\,\vartheta_{1})}{\sin(\,\vartheta_{2})}\!=\!\frac{v_{1}}{v_{2}}$  (geometrical optics)

Acoustic Impedance Values of selected Materials

![Tungsten Tungsten   1 04  104 Alumina  Alumina  21  45 Copper  Copper  N  42 Beryllia  Beryllia  32  32 Siicon  Silicon  20  20 Aluminum Aluminum   17 Glass  Glass  15 Plastic Plastic   2 3,5 3，5  Water  Water  15  1,5 Air  Air 0,004  0,004 0  20  20  41 0  40  60  60  89  80  1 0 0  100  120  120 ③0  30  Unit:  Unit:  [Z] = MRayl =106  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/78725624-fcf6-4f19-83fd-521988f171a9/78725624-fcf6-4f19-83fd-521988f171a9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=828b9218c40a81c40d38dc7730e1a1e73e06603d)
## Mode Conversion 

## Excitation of additional wave modes 

axial reflection

In a focused wave field    Wave fronts a planar in focus   Wave fronts are curved outside focus   Gradual transition of curvature     Angle of incidence   when sample distance    critical angle possible

angular contribution

sample surface

focal plane

Snellius‘ Law :   $\frac{\sin(\,\vartheta_{1})}{\sin(\,\vartheta_{2})}\!=\!\frac{v_{2}}{v_{1}}$  Critical Angle : sin( 𝜗 ௧ ) = ௩ మ sin( 𝜗 ଶ ) ௩ భ

sin( 𝜗 ோ

) =

𝑣

ଵ

𝑣 ோ

When this term becomes real-valued – meaning, that  𝝑 𝟐   is 90°

## Crack Detection using transverse Waves 

Focused transducer stepwise approaching the sample surface     Transmitting/receiving a signal pulse     V(z) material signature frequency dependent     Sensitive for crack inspection

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dc6ae40f-e6e8-4f12-821f-6e7d2a1f64ec/dc6ae40f-e6e8-4f12-821f-6e7d2a1f64ec.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=a993f5e343c04e4807bd2f1d76634d3b40e78436)
![Rayleigh  axialreflection  contribution  sample  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/58023751-6dbf-43f0-90f2-a8d596e86fb7/58023751-6dbf-43f0-90f2-a8d596e86fb7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=993ea5dfddf3741420536b1a71a016afb479065a)
## ML-based Signal Analysis 

![2mm   2mm   2mm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8f3b4481-a6b1-41e8-ada5-75acc505b37e/8f3b4481-a6b1-41e8-ada5-75acc505b37e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=0427cf13cf3faf8e3640fb13b61915ca1e2673a7)
## Challenges : 

Image depends on gate position in signal   Same object can have different intensity/ contrast

Which area is delaminated?

## ML-based Signal Analysis 

![Output  Output  Label  Label gating  gating Input  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c4bbd672-2432-461f-9d23-ddddf61ef4cd/c4bbd672-2432-461f-9d23-ddddf61ef4cd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=0aebe29fba158acd320d2e7938db0609013a9f57)
Operator independent Signal interpretation

![rel. porosity  rel. porosity DEF BMP INT BMP BCK RND Air Trapped 13  > quatification  quatification 2  classification 11  10  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2e05a513-3e02-4d3f-b1b1-126e333a9c3e/2e05a513-3e02-4d3f-b1b1-126e333a9c3e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=b61ed84e3f8a5f2642d73194267a7f44a4af3bfe)
![ML-based Signal Analysis  ML-based Signal Analysis → Delamination    Delamination DELAM  Intact  Die  Lead  2mm   35  35 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6de31493-bf0d-446b-a23a-24024bd0365c/6de31493-bf0d-446b-a23a-24024bd0365c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=77bcab7412eb86c90326ac9351ec13d5ce1a67db)
![Flip-Chip Analysis by ML Flip-Chip Analysis by ML  DEFBMP  set"A"   INTBMP   setB"   DefBump  BCKRND  AirTrapped   intact bump  nobump  undefined  400um  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6f170387-7aef-464b-a25c-b8d172381296/6f170387-7aef-464b-a25c-b8d172381296.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=9b0dc09c5a9951bb892488b379ff0c665316e295)
## Material Characterization through ML 

![Porosity in Die attach → ,  Porosity in Die attach     <<   pores  pores semiconductormaterial   50nm - 2μm  50nm – 2µm high   rel. porosity  rel. porosity 25  die-attach   米   13  [o/o]   regression slope 1  data set -I :  p  12  data set - Il: △ t  metallization  substrate  TE  neatsink  1O  Brand et al., “Deep Learning assisted quantitative Assessment of the  et al., "Deep Learning assisted quantitative Assessment of the  Porosity in Ag-Sinter joints based on non-destructive acoustic  ity in Ag-Sinter joints based on non-destructive acoustic  inspection.”, ECTC, 2021, pp 877-884. ction.", ECTC, 2021, pp 877-884.   ③7  37 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0f04aee2-85b3-4d90-9632-710f67acdf82/0f04aee2-85b3-4d90-9632-710f67acdf82.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=8682b46d33b7e7e86f22a2927258ffa5e6d400e7)
## Selected Cases of Application 

– SAM –

## Crack Inspection in Si / Al2O！ 3 Wafer

![Interface imaging  Interface imaging AI>O  Al  O 2  3 Si ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2274a63b-18c5-485d-95d8-5d8f4e09bc8d/2274a63b-18c5-485d-95d8-5d8f4e09bc8d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=d3327cee309236433117c870ff5045b0e68a3b5d)
## Crack Inspection in Si / Al 2 O 3  Wafer 

## defocusing required 

excitation of transverse wave modes

![Al2O3  Al 2 O 3 Si  Si ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cbab9125-bfd6-4775-9286-0967aed4e003/cbab9125-bfd6-4775-9286-0967aed4e003.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=e5283db2239b129bb68afa84e96bd9a12d57ff06)
Brand S. et al. (2017). "Defect analysis using scanning acoustic microscopy for bonded microelectronic components with extended  resolution and defect sensitivity." J Microsyst Technol DOI 10.1007/s00542-017-3521-7: 1-7.

## Analysis of Flip-Chip Bumps 

![Conventional SAM  Conventional SAM ooooo  0000o  600000  Split Spectrum Analysis plit Spectrum Analysis  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/06267cd2-2b01-44bb-b897-bd0fb237e8f4/06267cd2-2b01-44bb-b897-bd0fb237e8f4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=5e0b135b666d90315dd3852d048f5a2748eeffb3)
![Thin-layer Delam detection in Transmission mode Gatesetup1  Gate setup 1  Gate setup 2  Gate setup 2 150  150  TT-SAMconfirmS  TT-SAM confirms 100  100 50  50  theproperPE-  the proper PEAmplitude  -50 0  Amplitude  -50 0  SAM setup is #2 Transducer  Image  -100 -150  -150 Time(50ns/division)  Time (50 ns/division)  Time (50 ns/division) Time(50ns/division)   Water  x  x Receiver  TT-SAM PE-SAM  PE-SAM  PE-SAM  PE-SAM ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2edd4019-9ac9-40fe-ac17-85269f4b98d0/2edd4019-9ac9-40fe-ac17-85269f4b98d0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=fd6bf9a9e4fa9a935f0e67e0af491eeda0f66ec5)
Moore, T.M. and Hartfield, C.D. Through-Transmission Acoustic Inspection of Ball Grid Array (BGA) Packages.  ISTFA 1997

## GHz-SAM of Cu-Cu Wire Bond Interfaces GHz-SAM ofCu-CuWireBondinterfaces  

![ 50 μm   Conventional SAM30o  Conventional SAM 300   GHz-SAM  GHz – SAM                    MHz (FL 0.1")  MHz (FL 0.1“)  1 GHz (FL 80 μm)  1 GHz (FL 80 µm) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/389a3268-261c-4aec-93aa-92fe51afe7c0/389a3268-261c-4aec-93aa-92fe51afe7c0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=b173cf370495db907928c93f587d4f4b971c2e08)
Vogg G. et al. (2015). "Scanning acoustic GHz-microscopy versus conventional SAM for advanced assessment of ball bond and  metal interfaces in microelectronic devices." Microelectronics Reliability (55), pp 1554-1558

## GHz-SAM inspection of TSV´s 

![defocus sequence (line)  defocus sequence (line) 10  15  [uwn]z  20  29  -30  -35  -40   hagu  20   40   60   80   100  x[pm]  -10  20  [n]z  -30  -40  20um   1KX10T  -5O  20  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a5ab87b9-e3fd-496a-911a-e54882e8558a/a5ab87b9-e3fd-496a-911a-e54882e8558a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=558cfe58b603376494c3f9f56f826aa5a8d75a69)
Brand S. et al. (2015). "Acoustic GHz-microscopy and its potential applications in 3D-integration technologies." IEEE 65th  Electronic Components and Technology Conference (ECTC), pp 46-53

## µ-crack detection by GHz-SAM 

Small Sub-surface defects    GHz-SAM inspection in V(x,y,z) mode

## optical micrograph 

GHz-SAM micrograph (in focus)  GHz-SAM micrograph (de-focused)

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7fadf2af-ddad-4cea-bd5f-adfb44a6707e/7fadf2af-ddad-4cea-bd5f-adfb44a6707e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=ff032720f597047d9657e47cd2d4d96c70ad05c0)
![40 µm  40 µm 40.pm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9fddd550-edcc-470a-9e7f-f9488948b92e/9fddd550-edcc-470a-9e7f-f9488948b92e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=b673a293a2e7fa356a3c1bfcad1e7813d0d5476f)
Brand S. et al. (2014). "Scanning acoustic gigahertz microscopy for metrology applications in three-dimensional integration technologies."  J. Micro/Nanolith. MEMS MOEMS 13(1): 1-10.

![µ-crack detection by GHz-SAM u-crack detection by GHz-SAM  surface GHz-SAN  surface GHz-SAM  - micrograph  - micrograph SEM  SEM PFIB- cut  PFIB - cut 50 µm defocused GHz-SAM  defocused GHz-SAM  - micrograph  - micrograph 2KX  10um   ND5.0mm   40 µm clear indication for crack  clear indication for crack 5.73Kx2μm   Hgh Current    FIB Mog-4.62   defocused GHz-SAM - micrograp  defocused GHz-SAM - micrograph ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5598d74b-ad41-4d1c-983f-4b516d16a763/5598d74b-ad41-4d1c-983f-4b516d16a763.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=9a29a57b3466a931231afe83ee5a4c86a84c9837)
Defect Localization by

— Lock-In Thermography —

(LIT)

## Preface 

Direct thermal imaging  for detection of local  heating caused by resistive electrical defects

##   Typical  thermally active  defects: 

resistive shorts between metal lines, contacts,  bumps, pins, etc.      oxide breakdowns      locally increased metal or poly Si line    resistance     increased contact resistance

![迎  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/89956294-bde1-4823-868d-98e68a03eb4f/89956294-bde1-4823-868d-98e68a03eb4f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=72453a601c787e8918218c7808282e10214c7b4c)
## Direct Thermal Imaging 

![ThermoHuman  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/532ecd46-b371-4a01-a2af-82d679a14bdd/532ecd46-b371-4a01-a2af-82d679a14bdd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=d0d4b9ee564c62da4dac9f88ef3762d69cb24dbb)
Source: www://hiitscience.com

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5b068789-8d70-4abc-ac08-ea505ea8bb7d/5b068789-8d70-4abc-ac08-ea505ea8bb7d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=f7f60d2f4fa86d5f35c4739b70eca2fb539e7fce)
Imaging using  IR-sensitive  detector   Contactless  temperature measurements by  detection of thermal radiation

49

Source: www://flir-infrarotkameras.de

## Thermal Imaging Scenario 

![atmosphere  detectoroffset  loffset(x, y)  MWV  atmospheric transmissivity  sample   IR-camera  T atmosphere  Ir(adiation)   opfics  sample  atmospheric emissivity  emssivity  & atmosphere  ε (x, y)   IR-detector  obiect  sample   self-radiation ofoptics  loptics(x, V, T)  @ by Dr. Sebastian Brand  © by Dr. Sebastian Brand 50  50 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d49d96a3-08ad-43be-9f6d-7a1ccf3bc102/d49d96a3-08ad-43be-9f6d-7a1ccf3bc102.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=94aab3b26e1a887ce4a29fe0f1837824a6676eeb)
## Infrared Detection 

atmospheric transmission of electromagnetic radiation in IR range (20°C, 100% rel. humidity)

![  3 major windows SWIR, MWIR, LWIR ajor windows SWIR, MWIR, LWIR    detector materials:  ector materials:    SWIR (1 - 2 μm): InGaAs, PbS  SWIR (1 – 2 µm): InGaAs, PbS  (d）0  LIT in FA  LIT in FA   MWIR (3 - 5 μm): InSb, HgCdTe  MWIR   : InSb, HgCdTe   LWIR ( 8 - 14 μm): HgCdTe  LWIR  ( 8 – 14 µm): HgCdTe  short-  short-  mid-  mid-  long range  long range 100  8O  6  20  112  Wavelength(microns)  LIT in FA commonly performed in mid-range  LIT in FA commonly performed in mid-range  5678910   20μm   20  Welleniange  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0122cf8f-6621-4898-a75c-be2fa3060387/0122cf8f-6621-4898-a75c-be2fa3060387.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=8a0e7125aafaddf73a61c301106ef6dd1fee7109)
## Thermal Imaging Scenario 

![atmosphere  detectoroffset  loffset(x, y)  MWV  atmospheric transmissivity  sample   IR-camera  T atmosphere  radiation   optics  I (x, y, T,ε )  sample  atmospheric emissivity  emssivity  & atmosphere  8(x,y)   IR-detector  obiect  self-radiation ofoptics  sample  Loptics(x, y, T)   by Dr. Sebastian Brand  © by Dr. Sebastian Brand 52  52 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fa974ebb-be8a-429c-96f1-3ad645d293a0/fa974ebb-be8a-429c-96f1-3ad645d293a0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=af8341ebd18491359f4c295480ed7da5f5ecc0bd)
## Black Body Radiation 

## Radiation behavior / characteristics described by: 

![Allincident  radiationis  absorbed  Blackbody  Radiator  Sssssssssssssssssss  / Emitted Radiation  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5b857e84-d674-481c-865d-f3ada5b16d95/5b857e84-d674-481c-865d-f3ada5b16d95.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=edaed10221bc2fea94e0b4e3a7a482e2e1f3ede2)
Planck‘s Law   Wien‘s Law   Stefan-Boltzmann‘s-Law

idealized generalization/simplification     absorbs all incident energy     absorption  $=$   emission     no transmission     no reflection     intensity and spectral distribution   depend on T only

## Direct Thermal Imaging - Planck’s Law 

describes the relationship of radiated thermal energy as a function of wavelength  and temperature

![350  350 200°C  200°C 100°C  100°C 300  300  50°C  50°C 20°C  20°C ] 1  -1  0°C  µm  uun  250  250 -2 specific irradiance M  [W m  8  200  200 150 150  100 100  50  50 0 0  5  10  15  15  20  20  25  25  30 入in [um]   in [µm]  54 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1977002a-9f34-4db8-bc70-0f7d8f1a2516/1977002a-9f34-4db8-bc70-0f7d8f1a2516.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=7b3995ba515b4c9db5b00b85b25cd70494fab114)
𝟎

𝟐𝝅𝒉𝒄

𝟏

𝟓

𝒉𝒄 ష𝟏

𝒌𝑻

Every  object irradiates energy  because of its temperature

steep increase and slower decrease of  radiated energy with increased  wavelength (decreasing frequency)

:  wavelength T:  temperature h:  Planck‘s constant :  Boltzmann‘s constant c:  wave velocity of light :  emissivity

## Direct Thermal Imaging - Planck’s Law 

describes the relationship of radiated thermal energy as a function of wavelength  and temperature

𝟎

𝟐𝝅𝒉𝒄

𝟐

𝟏

𝟓

𝒉𝒄 ష𝟏

𝒌𝑻

![ultraviolet   visible   infrared  radiation   radiation   radiation   TEC  SCIENCE.COM  1010  10000K  108   5778K  106   2000K  1000K  1O4  500K  1:02  250K  100K  100.1   0.2   0.3   0.40.50.6   0.8   45   678910   20   30   40 50 6070 8090100  wavelength(um)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/48c9b658-8009-4671-b64f-e78aae904ba5/48c9b658-8009-4671-b64f-e78aae904ba5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=e1555bb7a3b97c090d231c5c43a8d19cc91d6a0d)
image source: https://www.tec-science.com/thermodynamics/temperature/plancks-law-of-blackbody-radiation/

Every  object irradiates energy  because of its temperature     steep increase and slower decrease of  radiated energy with increased  wavelength (decreasing frequency)

:  wavelength T:  temperature h:  Planck‘s constant :  Boltzmann‘s constant c:  wave velocity of light :  emissivity

## Direct Thermal Imaging - Wien’s Law  

describes the relationship of the wavelength at maximum amplitude to the temperature     max    𝟏  𝑻

![350  350 200°C  200°C 100°C  100°C 300  300  50°C  50°C 20°C  20°C ] -1  0°○  0°C  µm  uun  250  250  Wien‘s Law Wien's Law  -2 specific irradiance M  [W m  U  200  200 150 150  100 100  50  50 0 0  5  10  10  15  15  20  20  25  25  30 入in[um]   in [µm] ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f3b35bdc-2ccd-42cc-9d12-35e81445387c/f3b35bdc-2ccd-42cc-9d12-35e81445387c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=4aec66c948dce0b5a3e1f285d8d13cfcd6970a03)
𝒎𝒂𝒙

Wavelength at maximum intensity  decreases with increasing  temperature (frequency increases)

:  wavelength T:  temperature h:  Planck‘s constant :  Boltzmann‘s constant c:  wave velocity of light :  emissivity

## Direct thermal imaging -Stefan Boltzmann’s Law 

describes the relationship of the radiated energy to the temperature  M  T4

![350  350 200°C  200°C 100°C  100°C 300  300  50°C  50°C 20°C  20°C ] -1  0°C  µm  uun  250  250 -2  area corresponds  area corresponds  specific irradiance M  [W m  uu]   to total energy  to total energy 200 200      150 150  100 100  50  50 0 0  5  10  10  15  15  20  20  25  25  30 30  入in[μm]   in [µm] ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b3814699-bac9-4ba9-ab44-d81461561445/b3814699-bac9-4ba9-ab44-d81461561445.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=3a25f539abb4610043f0898dc59e2b65a336f3a7)
𝟒

Total radiated energy increases with a  power of four  with temperature

:  wavelength T:  temperature h:  Planck‘s constant :  Boltzmann‘s constant c:  wave velocity of light :  emissivity

## Direct thermal imaging – Emissivity 

Object of  equal  temperature shows  contrast

Emissivity  “scales” the  actual irradiated  energy

Emissivity  ε depends  on  material, surface quality, T,

Metals : low emissivity  (< 1% to 5 %)

Si :  transparent ,  medium emissivity (\~10%)

Glass, mold compounds : high emissivity

Opaque samples :

(absorption)

ε may change during experiment!  (e.g. thermal

degradation of metal lines)

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cf6b7b46-9b62-454b-9a7f-614ec5c3b189/cf6b7b46-9b62-454b-9a7f-614ec5c3b189.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=a58de477c1df889715e3cfd3d8e4679922d9491a)
ASIC at room temperature

Even  unpowered ICs  show strong IR contrast, which is  pure  emissivity contrast!

## Direct thermal imaging – Emissivity 

## Emissivity Compensation 

Measurement of T requires (!!) calibration of emissivity and  system transfer function for Camera, T-range and Sample

Acquisition of calibration image at defined temperature (e.g.,  T room )

Emissivity correction through normalizing the IR image to  calibration image (e.g., recorded in unpowered state)

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b7c7d7dd-0430-4048-9325-016c3001c472/b7c7d7dd-0430-4048-9325-016c3001c472.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=bcc6f48ab4090477708c39a7a990583348045fa4)
uncorrected (unpowered)

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2f0712ba-37b6-43b3-b5e3-c874fb7e182f/2f0712ba-37b6-43b3-b5e3-c874fb7e182f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=3cd725a082efbc01625798288ab9934945725c58)
![[°C] 120 120  100 100  80  80 60  60 △O  40 20 20  0 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/66490516-0062-465e-ba11-3dd499925fb7/66490516-0062-465e-ba11-3dd499925fb7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=a34f4015345b767343ead2c1c69715e159088f6f)
Temperature in °C

“true temperature" (ε - corrected) unpowered

“absolute temperature" ( ε -corrected) powered

## Absolute High-Temperature – Measurement 

Irradiated energy increases with   T4   Emissivity may vary between   $1\%$   and   $95\%$   across  the sample

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/390c898d-1d19-45ab-b4c3-929b91e1cf94/390c898d-1d19-45ab-b4c3-929b91e1cf94.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=b08aac8718df94b077cd44adabd554a8d8bd1406)
Extreme dynamics  of irradiated energy across  sample between  $\Rightarrow$  cold/hot areas and materials

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1e332b19-3ede-4dee-adc8-08a9d440c731/1e332b19-3ede-4dee-adc8-08a9d440c731.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=6a3104a07ae0ecf64cf354f291a7ff54db21c9d9)
hot-  $\bf\cdot\delta_{i}O_{z}$   areas  detector saturated colder metal areas  $\Rightarrow$  signal in the noise floor

![290  270  250  230  210  190  170  150  130  110  90  50  [w/Mi u! lamod pajepie!!      400000 400000   30      300000 300000  metal  metal glass  glass     200000 200000      100000 100000           0 0  50  50  10:0  100  150  150  200  200  250  250 Tin [°C]  T in [°C] ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/50903464-fae9-45ba-a1d5-4aabee5ed5c2/50903464-fae9-45ba-a1d5-4aabee5ed5c2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=fa1a51d39ea5c710395c6bf9b8bac376b7cfdb15)
## Lock-In Thermography – Fundamentals – 

Resistive defects cause local  temperature increase

In Microelectronics  only µW  dissipated power  corresponds  to  temperature increase in  µK  range

BUT : Sensitivity of IR-camera  >10 mK  !!!  only

Steady state imaging: strong  T  saturation  and  shadowing of small hot spots

Buried defects  (from package interior)  $\Rightarrow$  small ΔT  at  surface

Lock-In amplification  to increase  sensitivity  of  thermal imaging!

![Amp+Topo  Hot spots  NumberofPeriods:1582   U:3V   SOO  240pm  Global Phase   ：300   1:6,SmA  Frequency   ：25Hz   tint:4ms  Nobice:detail Image of a defect in the conductive path area  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5ba44396-9765-48f3-8d64-4b4b0d0e51e5/5ba44396-9765-48f3-8d64-4b4b0d0e51e5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=c1902a341f0cb56a25a4d7f2de539c86018e2eec)
![Hot spot  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8eef3f84-d812-40da-b91d-2b32f8cc5e53/8eef3f84-d812-40da-b91d-2b32f8cc5e53.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=ccf96655a4b7d4a5473bb31bf9e81ff0788e4afb)
## LIT Measurement Techniques 

![  correlation with sine- and  correlation with sine- and  R  capturedthermalsignal  camera   cosine signal shape  cosine signal shape   narrow band analysis of  narrow band analysis of  SMU-powersupply   dynamic signal  dynamic signal thermalsignal  sample  or  DUT"  LL  electricalexcitationsignal    sample  sample periodically excited by el. signal (sine or square)  periodically excited  by el. signal (sine or square)   heat source (defect)  heat source (defect) stimulated  stimulated   IR camera captures sequence of thermal images  IR camera captures  sequence of thermal images   sin/ -cos correlation of thermal signal (@ each pixel);  sin/ -cos  correlation  of thermal signal (   each pixel);  Amplitude (A), Phase (Φ)  Amplitude (A), Phase ( ) measurement repeated and averaged > increase in sensitivity  measurement repeated and  averaged   increase in sensitivity ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d6699d8e-150b-4246-a8d6-dde8bd5f400a/d6699d8e-150b-4246-a8d6-dde8bd5f400a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=4906b3a6e4527a8b0e9b0e2914a0fa0d053e09fa)
## The Lock-In Technique 

Periodic excitation of sample  $\Rightarrow$  thermal response measured     Response has a causal relation to excitation (as it caused it)     Estimation of correlation coefficient (description of similarity of measured and excitation signal)

![measuredsignal=25°  sine  cosine  0.5  [n'e]  -0.5  0.02   0.04   0.06   0.08   0.1   0.12   0.14   0.16   0.18  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/aa905220-a837-4192-aac6-bf88fda32864/aa905220-a837-4192-aac6-bf88fda32864.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=09c2490fb8a65aad41bd1e547f7ef917f2e1919e)
tsi

![Q5  [n'e]  -0.5  measuredsignal=25°  signal modulatedwithsine  signalmodulatedwithcosine  0.02   0.04   0.06   0.08   0.1   0.12   0.14   0.16   0.18  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/688d5f0f-7c2a-446b-a275-761881c63d82/688d5f0f-7c2a-446b-a275-761881c63d82.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=03ee3dcd439e317c0f83c05db725697e38650fb6)
## The Lock-In Technique 

Temporal integration of modulated / correlated signals  weighting by the expected outcome     averaging over all periods     applicable to linear-time-invariant (LTI) systems

![sine-correlation  S 0° 0.5  [ne]  𝑻 -0.5  𝑺 Soo  𝟎°  = න𝒔 Smeas(t) \* sin(wt) dt  𝒎𝒆𝒂𝒔  𝒕∗𝐬𝐢𝐧  𝒕𝒅𝒕 𝟎 0.02   0.04   0.06   0.08   0.1   0.12   0.14   0.16   0.18  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0ea57325-99ff-4449-b869-9e36a8dc73bf/0ea57325-99ff-4449-b869-9e36a8dc73bf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=e6f066e17b9ba31dc832e67234218110838b4b97)
$$\begin{array}{l}{A=\sqrt{{S_{0^{\circ}}}^{2}+{S_{90^{\circ}}}^{2}}}\\ {\hfill}\\ {\varphi=\tan^{-1}\frac{S_{90^{\circ}}}{S_{0^{\circ}}}}\end{array}$$
A:  amplitude of measured signal ϕ:  phase shift of measured signal relative  to excitation

![S  S  cosine-correlation  900  90° 0.5  [ne]  -0.5   𝑻 𝑺 S90。=   = න𝒔 Smeas(t) \* cos(ot) dt  𝒕∗𝒄𝒐𝒔  𝒕𝒅𝒕 𝟗𝟎°  𝒎𝒆𝒂𝒔 一一   𝟎 0.02   0.04   0.06   0.08   0.1   0.12   0.14   0.16   0.18  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/739cee54-1590-4136-88f3-2cbea8da04d1/739cee54-1590-4136-88f3-2cbea8da04d1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=02bb946f9080209c4e56eea01abe28ac2876ee19)
## Lock-In Thermography   – the Principle – 

![Averaging in 2 separate  Averaging in 2 separate Classical Two-Phase LIT  lassical Two-Phase LIT   Heating power  Heating power frame storages !  frame storages ! P image processing: nage processing:  t Individual incoming  Individual incoming  Multiplication by weighting factors  Multiplication by weighting factors  Result  Result frames  frames 1  0° (incl. topography  (incl. topography  sin(t)  sin(t)  t and noise)  and noise)  -  1 sin(t)\*F(t)  1 ) F(t) -90° -cos(t)\*F(t)  2 1 -cos(t)  -cos(t) t -1  △ t=1/fframe  t=1/f frame ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/345636b2-98b6-4d54-9621-a6f70648d2bd/345636b2-98b6-4d54-9621-a6f70648d2bd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=f99d5a55225afefd2694c41ca366602e9b9556a2)
## Lock-In Thermography   – the Principle – 

Primary results :  $0^{\circ}$   image and   $.90^{\circ}$   image (modulated by emissivity contrast)   Converted into amplitude and phase images

![Hot spot  Hot spot 250μm  250 µm  250μm  250 µm Amplitude image  Amplitude image  Phase image  Phase image A =√(s0} +(s-90)  A   S 0 2 S 90 2  Φ = arctan  arctan   S  S -900  90   S 0   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/44ae0c28-ec18-41fb-96be-c17a55fcad5d/44ae0c28-ec18-41fb-96be-c17a55fcad5d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=c63ae1e56c4b737f58a2fbd7290a8ee6825a3d79)
![Hot spot  Hot spot 250μm  250 µm ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f59ad67f-f4df-4756-9d42-4338fb1cd0cc/f59ad67f-f4df-4756-9d42-4338fb1cd0cc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=a4e7ed03cf079e7cdefec2ce35c8504e6bcd8b39)
Topography  $^+$   Amplitude        Localization of hotspots related  to layout

## Resulting Images  

## – an Example – 

![topography topography  single IR image,  single IR image, emissivity dominated emissivity dominated  amplitude image  amplitude image contains emissivity contains emissivity  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d87ecebc-f116-43e5-b2d2-efc0ef3aeb5b/d87ecebc-f116-43e5-b2d2-efc0ef3aeb5b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=5ab0fc22d87d1fd871a7d64b6f76fa8fe11749cc)
![in-phase / 0° in-phase/0°  best spatial resol..  best spatial resol., contains emissivity contains emissivity  phase image phase image  low spatial res.  low spatial res. emissivity-corrected  emissivity-corrected dynamic compression dynamic compression  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1cbb2b2d-7c79-453b-a7e8-d777aa73510e/1cbb2b2d-7c79-453b-a7e8-d777aa73510e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=9a6dd2f2723c64a4485519c7173937534950c866)
![out-of-phase / -90° out-of-phase / -90  low spatial resol.  low spatial resol., emissivity dominated emissivity dominated  0%-90° image  0°/-90° image better spatial res.,  better spatial res., emissivity-corrected emissivity-corrected  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5c6d8ef6-40ec-44d2-bcfe-b066ce2d6b39/5c6d8ef6-40ec-44d2-bcfe-b066ce2d6b39.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=dd1c6e1997a7fdd823cb8f24a1143ff898553b95)
## Steady state imaging vs. LIT 

![Amplitude  400um   Global PhafPeriods:1088   Y:8y4mA  Frequency   :steady   tInt:4ms   LOWN.   IM  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/758f487d-2f01-4d93-8149-0dd5292e2c9d/758f487d-2f01-4d93-8149-0dd5292e2c9d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=27d9cfc1c25b8fa84a4fe840af7e664948a431a7)
Contrast governed by  local emissivity  and  heating related saturation,  weak  heat sources  not visible

![Amplitude 400pm  Global PhafPeriods: 1423  Y:77mA  SS Frequency  ：25Hz  tInt:4ms  IM ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/680e6519-6e23-4972-b219-92d549994446/680e6519-6e23-4972-b219-92d549994446.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=6cd5f4e140f76cfffedc830081eec56760b539ba)
Lock-In Thermography

Weak  heat  sources  become  visible,  improved  spatial resolution

## – the Frequency Benefit – 

![Influence of the Lock-in frequency  Influence of the Lock-in frequency 1Hz 1HZ   25Hz  25Hz   入 = thermal diffusion length  λ =  thermal diffusion length     2 \*     proportional to 1/√fLock-in   proportional to 1/√f Lock-in \* c  \* 2 \*  f    Si: 3 mm @ 3 Hz  → 1 mm @ 30 Hz  Si: 3 mm @ 3 Hz       1 mm @ 30 Hz p  Lock-In  Lock In ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/575aefa6-f9a6-4fdb-a6a8-a5cdeec924a1/575aefa6-f9a6-4fdb-a6a8-a5cdeec924a1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=0cb8015bb17e74dc8ce5b4dfc189192cba3b6b53)
## LIT  

## – the Frequency Benefit – 

![1HＺ  1 Hz  5Hz  5 Hz  7TＺ  7 Hz 9HＺ  9 Hz  11HZ  11 Hz  15 Hz 15Hz  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fe8518d2-7fca-428f-828a-5c896fc610d6/fe8518d2-7fca-428f-828a-5c896fc610d6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=fd991d93d3006ab6cdcb79bba76618b8d4413cce)
With increasing f Lock-In  spreading  reduces  and resolution  increases

## The Lock-In Technique 

![-4.22°   =3.55e-15°  ock-ln   simulated   ock-ln   TRTR  1.5  Lock-ln-periods:1measured△o=20.8°   simulated△o=25  simulatedsignal;   =20  poise  0.5  [n'e]  -0.5  -1.5  0.2   0.4   0.6   0.8   1.2   1.4   1.6   1.8  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a6aa238f-570f-4b22-b237-cea2c4765c0e/a6aa238f-570f-4b22-b237-cea2c4765c0e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=71282c10024f489dcfaf2d4e269432226010cfb5)
![PowerSpectrumbyTRTR  80   SNRTRTR = 22.4dB @ 1 Hz△ΦTRTR= 20.8°  60  40  20  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/978d597d-61d8-4310-a0a0-9c65c651039b/978d597d-61d8-4310-a0a0-9c65c651039b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=b47adac3f9a9922648ed636d4c7dbfc2a0ed629c)
## The Lock-In Technique 

![5  AO  5   20  16   10  20  200   400   600   800   1000   1200  Lock-InPeriodsN  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/60af3770-beaf-4792-8635-ac05ebe50a89/60af3770-beaf-4792-8635-ac05ebe50a89.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=160e41cc4ab28df5002282fc70c4997e344e421b)
Signal-to-Noise (SNR) versus lock-in periods:

## Customization of Excitation Signals 

![0.6  08  Square Sauare   'n'e apndwe    'n'e apndwe  0.6   ○A  ○.  0.2  0.№  50   100   150   200   250   10   20   30   50  t[s]   f[Hz]  0.5   0.2  Multi-Sine Aulti-Sine  'n'e apn!idwe   'n'e apndwe  0.05  -0.5  50   100   150   20:0   250   20   40   60   89   10:0   120   140  tIsT   f[Hz]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/34e3a2bd-c567-4018-8487-e2b22006c18c/34e3a2bd-c567-4018-8487-e2b22006c18c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=495a99294c725514d07b728e76ae8fcd7d79499c)
LIT-imaging at specific Frequencies

Signal shapes  spectral content:   Square : Spectral power decreases with 1/f  fixed relation   $\Rightarrow$  cannot be adjusted   Multi-Sine : defined spectral distribution by  adjusted power density , no  “off”  section in excitation

## Broad Band LIT 

![modulated  IR   thermal signal  camera  Arbitrary Waveform  Generator (AWG)  thermal signal   Acquisition-sample   software on PC  ",DUT"   - all frames acquired  and stored  - on-the fly- averaging  electrical excitation signal  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a9e7f54e-d81e-4c56-a655-8654dbb8365e/a9e7f54e-d81e-4c56-a655-8654dbb8365e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=ee6150b35678dc0cc796b75e188a6cc78e65224b)
## Simultaneous LIT at multiple frequencies (multi-sine) 

Design excitation signal to contain energy at multiple frequencies a(f)   Acquire and store all frames of the period   $\Rightarrow$  offline analysis: FFT (spectral decomposition)

Brand S. et al. (2019). "Advanced 3D localization in Lock-In Thermography based on the analysis of the TRTR (Time-Resolved Thermal  Response) received upon arbitrary waveform stimulation.“  $45^{\mathrm{{th}}}$    ISTFA 2019: 1-8.

## 3D – Packages Defect Localization with LIT 

## Semi-destructive Approach: 

![Hot Spot Hot Spot  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1a38b554-2050-45a7-be1c-ac1280d36672/1a38b554-2050-45a7-be1c-ac1280d36672.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=b471e7e3b15305e6fb2f41bc5fbd6980a88d377e)
![Hot Spot  Hot Spot ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4b591cde-66a2-41a5-9c65-b0a68842ada5/4b591cde-66a2-41a5-9c65-b0a68842ada5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=7450963a3a8247c63c99cadbad702198f23e2436)
![Hot Spot  Hot Spot ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3b92dc5d-6443-4b5d-aeb1-1360f6c0e2aa/3b92dc5d-6443-4b5d-aeb1-1360f6c0e2aa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=48d09e8333a31efcc19025d0b86d38f6a46658ee)
1 st   investigation: Hot spot localized within IC  area

2 nd   Investigation:   Mould removed   → local spot, but which IC    level?   75

3 rd   investigation: disconnected bond wire of upper IC hot spot still present  $\longrightarrow$   defect at lower IC

## 3D – Packages Defect Localization with LIT 

3D localization  of shorts in unfilled TSV structures  by LIT focus series:

Defocus value at sharpest spot  $=$   defect depth

![Surface  25pm  Focus  Defect  positions  position  100  Surface  -100μm   80  -150μm  -200pm   6O  20  20   30   40   S0   60   -250   -200-150-100   -50  Position[px]   DistancetoSurface[um]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/78a77ee2-dacd-4e0e-b50b-e01b4337786f/78a77ee2-dacd-4e0e-b50b-e01b4337786f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=d35bdb473a7ca405493a0fcd8154e449c680b04f)
![Surface   -100μm  -150μm   -200pm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/773a403f-b027-4bf3-97b6-ac0dc491ebc6/773a403f-b027-4bf3-97b6-ac0dc491ebc6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215825%3B1743219425&q-key-time=1743215825%3B1743219425&q-header-list=host&q-url-param-list=&q-signature=65a3cb1ffb8741afce2ca850f71200d6b79e9ba8)
Altmann et.al. ISTFA 2012

## 3D – Packages Defect Localization with LIT PackagesDefect Locallzatlon With Lil  

![Faulty  Faulty  FIB  FIB   formation of  formation of  cut  cut  TSV  TSV  metallisation  metallisation Si - residues  Si - residues Sample 45° tilted and rotated  Sample   tilted and rotated  77 NN  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/96aa42c9-1096-41f6-a781-58f9eb849280/96aa42c9-1096-41f6-a781-58f9eb849280.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=adab724c12b641b571d123949cb422d5b43c3195)
## 3D – Packages Defect Localization with LIT 

“Heat flow takes time”  phase shift depends on defect depth and covering material layers  “Fingerprint” enables 3D defect localization

Previous studies investigated spectral phase shift to correlate with defect depth (e.g. Schmidt et al., 2012; Mat Sci and Eng, 177(15); doi: 10.1016/j.mseb.2012.02.011)

z

n

n

µ

n

n

z

n

2

\*

![100  -fail  mold  mold  80   -upperdie  A x  lowerdie  upper die  upper die   s  60  lower die  lower die  40  B C  x  x multi-layer  multi-layer         20  lead-frame lead-frame  8   10  fiock-in [Hz]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5a02feb5-c846-4f18-bd00-e7e192ed13cf/5a02feb5-c846-4f18-bd00-e7e192ed13cf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=449b62b9a3c3fe7447c6145a5d86ad2b64729f9f)
c

p , n

\*

\*

2 \*

f

Classical LIT  : separate measurement at  each  frequency Multi-Sine  : simultaneous measurement at  all  frequencies

## 3D – LIT  Heat Propagation 

Omni-directional propagation     thermal conductivity and diffusivity define propagation spread in sample     Lateral spreading  resolution reduction     Irradiation at surface (IR-radiation)

![122222222222  Material - IV Material - IV   T 5 Material - III Material - .   1A  T 4 Material - 1  Material - II  3  T 3 T 1 T N  2 Material - 1  Material - I thermal source  thermal source 79 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/64aed09c-54a2-4c0f-80fd-9820279612d6/64aed09c-54a2-4c0f-80fd-9820279612d6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=7d2b8d1a8e31e3480e22d425e1c2006a7217e3e6)
![3D – Packages Defect Localization with LIT 3D - Packages Defect Localization with LIT  time-domainsignal  1Hz 1TＺ     TRTR / Multi-Sine @ 4 frequencie  TRTR / Multi-Sine   4 frequencies 150   17Hz 7Hz IN   t[s]  Phase vs. Frequency  Phase vs. Frequency  13Hz  13Hz 200  180   7TＺ  7Hz 13Hz 13HZ   160  140  120   1Hz 1TＺ  8100  17Hz 7HＺ   80  60  20  10   14   16  80  80  f[Hz]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/18604e98-ccb8-46fd-b453-4d09b4cd184b/18604e98-ccb8-46fd-b453-4d09b4cd184b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=a68cc97d0e95bbbd12e20e3d6e8a736f36ce8df5)
## 3D-LIT: Quantitative Depth Estimation 

Semi-analytical method for propagation tracing   Takes thermal properties into account   Precise quantitative depth estimation of thermal sources   Reduction of thermal spreading related artifacts

![Material - IV Material - IV   -T5  T 5 114  T Material - Ill  Material - III  4 Material - I  Material - II T 3 T 1 T N  2 Material - 1  Material - I thermal source  thermal source ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0b3909f2-8468-40db-8be4-3b9f09e95486/0b3909f2-8468-40db-8be4-3b9f09e95486.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=fb0b251825303c697481b6e10bcc1955a37db2d6)
![3DPIot  410  410   250  250  unn  µm  un  µm 0.2  lateral-x[mm]  0.4  0.6  2  4  0.8  10   34  6   lateral-y[mm]  lateral-x[mm]  mm]  82  Imm]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d4a47679-2351-40a5-b5b0-2a220ab05821/d4a47679-2351-40a5-b5b0-2a220ab05821.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=91e4620649eaeafd0a0dcc8fa6a4274256c56613)
## Selected Cases of Application 

– LIT –

## High Resolution IR imaging 

## Solid immersion lens (SIL) 

Silicon Solid Immersion Lens  (SIL) increases  N.A.  (and thus diffraction-limited  spatial resolution) by a factor of  3.5  ( Si ),  4  ( Ge )

![S  sample  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/920cec62-603b-4366-8033-d78e9d497756/920cec62-603b-4366-8033-d78e9d497756.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=90e204abc23459a294b02ffad2b77165837a90b0)
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7c45f49d-dbe2-478a-b966-bf0d2ce0b473/7c45f49d-dbe2-478a-b966-bf0d2ce0b473.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=4fbe6c5d748cbbd5e854c3fb663601fc69c59b71)
SIL widely used in emission microscopy and laser techniques (mostly from backside)   SIL in LIT: highly sensitive thermal imaging with 1.5 µm spatial resolution

## Handling a semi-spherical silicon SIL 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0c17d018-1dec-463c-84de-014e5661718c/0c17d018-1dec-463c-84de-014e5661718c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=ce94717a0ef2d6879cdbb29508324599003910f8)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ec6bb7a0-79ca-4eb2-a938-ee0382270727/ec6bb7a0-79ca-4eb2-a938-ee0382270727.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=cc4ed381ca7402044743c07a6aa3909c32f45cb5)
SIL attached to prober   accurate positioning on sample   increase in resolution / sensitivity

## SIL-Case: Edge leakage at IC structure 

![Amplitude  100µm 100μm  Number of Periods:71   U:3V  240um   Number of Periods:268   U:3V   zopm  Global Phase   00   I:0.14mA   GlobalPhase   ：00   1:0.13mA  Frequency   ：0.5Hz   tint:1ms   Frequency   0.5Hz   tInt:1ms  Notice:Detail Image of Sample2   Notice:SILI   Sample2  Imaging with 5x Objective >  Imaging with 5x Objective →   SIL in working position  enhanced  SIL in working position   enhanced  hot spot detected  hot spot detected  88  86  allocation to IC structure allocation to IC structure  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2f42442d-db8b-498a-947c-c7b7cdef05b7/2f42442d-db8b-498a-947c-c7b7cdef05b7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=8b9217d123b54c41da823a98c35f5f17ed760375)
## Standard-LIT – IC-Level 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/76a3da24-ee76-4696-af90-3467bef5b8ef/76a3da24-ee76-4696-af90-3467bef5b8ef.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=b8fa3db94eb30411980fa93e3610fd9ddfa169be)
Pressure sensor for highly stable industrial  application     Showed leakage (1mA@10V vs. 1nA) at  piezo bridge     Crystal defects  linear metal inclusions in  highly doped regions

![9onm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7881cde3-033c-4deb-b3ac-61058003450e/7881cde3-033c-4deb-b3ac-61058003450e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=ec53a75ae8292c183fa287814b8b40c5d7d9c640)
![500nm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8112e1e7-4007-4027-a14a-778c53bae665/8112e1e7-4007-4027-a14a-778c53bae665.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=542191abfa577736c13f715a234681a16bf6ec9f)
## Standard-LIT on a packaged Device 

No direct optical access to die or interconnects within a package   But heat propagates through opaque layers to the device surface    Enables  non-destructive through-package  hot spot localization   lower lock-in frequency allows higher SNR, but less lateral resolution due to thermal  spreading  sample related optimization

![3Hz  3Hz  6Hz  6Hz  9Hz  9Hz ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3784bc0b-e1e5-4029-8e75-040ea78dfb84/3784bc0b-e1e5-4029-8e75-040ea78dfb84.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=ffcedcc19bad6f436075d0b0b7a7d4383a55ac04)
![Standard-LIT – Packaged Devices Standard-LiT - Packaged Devices   Organic Material Organic Materia  Conductive layer of  Conductive layer of  corroded metallization  corroded metallization Mag - 68.87 K × 100 nm\*   Frnhofer  CAP-I  CAP-I  CAP-II CAP-Il  FDg1   T-54.0\*  89  89 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/be840b38-1944-41e5-90f3-ee8e653f9b4e/be840b38-1944-41e5-90f3-ee8e653f9b4e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=96266b61da7967a46609cd19be3c437b2cf37a17)
## Standard-LIT – Packaged Devices 

## 1. Case study: short between two pins 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5516fbad-1451-4fc4-8c1b-94472677b9a1/5516fbad-1451-4fc4-8c1b-94472677b9a1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=7ac0c0a0ecb4050bd0ff67f771733c623515f2bd)
Hot spot localization outside of IC  (  $\rightarrow$  correlation with XRAY)

![20pm   T=7.99kV   ture Size = 30.00 μm  FIB EHT =0.00 KV   Stage at R=207.  Mag=500x   WD=8mm   HighCurrent=Off   FIBProbe=200pA  Stage at T=54.0\*  Tit Angle =36.0\*  Detector=SE2   Pixel Size = S85.9 nm   FIBMag=7.12KXDate:13Aug 2007   User Name = KRAUSE  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/31b43a6b-cb8d-4e6f-9647-976364aa057d/31b43a6b-cb8d-4e6f-9647-976364aa057d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=52ae50f2f865cd97bab8f151bd0b28791ebee9f8)
Failure mode visible after decapsulation → touching bond wires

## Standard-LIT – Packaged Devices 

![Hot spot  Hot spot 1.5 mm  1.5 mm  3 mm  3 mm  Au wires  Au wires Flitter/  Flitter/  particle  particle ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d06853a3-7c91-4143-851e-067661e3e7ca/d06853a3-7c91-4143-851e-067661e3e7ca.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=1f242498b4d8009f23684d6242ea0fadb5e93095)
2. Case study: improved spatial resolution by local thinning


## Standard-LIT – Packaged Devices 

## 3. Case study: Plasma-FIB validation at short within package 

![EDX analysis : Al, Ti short path  EDX analysis : Al, Ti short path Thermal signal outside of chip Thermal signal outside of chip   Specimenmilledatfrontside  Specimen milled at front side , chip removed  chip removed 1  2 Thermal signal of short   Al eriodenanzahl:1484   U:3,SV   riodenanzahl:3991   :2V  GlobalePhase:0   1:13,5m   Globale Phase:0   I:9,23mA  Frequenz   ：11,47HztInt:0,8ms   Frequenz   ：23,9Hz  tint:0,8ms  Plasma-FIB cross sectioning  Plasma-FIB cross sectioning  Particle/  Particle/  inclusion  inclusion Ti 4 3 92  Fraun  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6639cd3c-aafc-4262-8e06-2d57230caf0d/6639cd3c-aafc-4262-8e06-2d57230caf0d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=c612578c874d85763e6765d4ae07a04b84302b99)
## Machine Learning enhanced 

– LIT –

## Machine Learning assisted 3D-Localization 

slanted polished stacked 4-die sample

Maps of spectral amplitudes

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/39178ffc-84df-4594-a1d4-be07d6857535/39178ffc-84df-4594-a1d4-be07d6857535.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=9c7b8714ed64ad37e441caf6295afe235e5307ee)
Needle probing at several vertical positions – emulation of increasing hot-spot depths

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e39a1392-5584-42bd-b2f3-a534ff014e15/e39a1392-5584-42bd-b2f3-a534ff014e15.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=1e723392822d39778d3d917385d7cbd33118b548)
Optical image of sample back-side with probe tip

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/77fbd166-2c3a-419e-9bb8-b4807ede5a94/77fbd166-2c3a-419e-9bb8-b4807ede5a94.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=506bd62bd0b47cd466ef7fb7cc0457297d1613b2)
IR - image

## Machine Learning assisted 3D-Localization 

![TRTR - Signals in spectral-domain - Signals in spectral-domain  Classification Classification  Thermogram + Classification Map  Thermogram + Classification Map ！1  D1 CAT-D-1  D2  D2  CAT-D-2  CAT-D-5  CAT-D-6  D5 D5   CAT-VOID  D6  D6 VOID Training Data  Training Data  Classes  Classes ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dec605e7-732e-4b5a-9abe-cb45efe0da20/dec605e7-732e-4b5a-9abe-cb45efe0da20.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=87c5187ca1b090766ce43f2dca6be79b3f71a535)
![D4 D4D1D1 D5 D5D2 D2D6 D6CAT-D-2 CAT-D-5 CAT-D-6  D3 D3CAT-VOID CAT-D-3 CAT-D-4 # 96 96](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7eebc482-d141-49f8-9d33-13ef54cb933c/7eebc482-d141-49f8-9d33-13ef54cb933c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=578776f4822ff5e8c9f397468154e82fecffa5da)
## Quantitative Depth Estimation through ML 

![Classification   Regression  20  1 00  1D Real valued  1 D Complex valued   G  2D mod. Google NET  80   19  [       S    1D Real valued  1 D Complex valued  2D mod. Google NET  10  40  20  raw TRTR   raw TRTR  Data Type   Data Type  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c019be72-2c19-439d-98f6-0f562889fa78/c019be72-2c19-439d-98f6-0f562889fa78.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=c8f94ab7adf27265914d896c68ec62df857e8262)
## Summary & Conclusion 

ND-Techniques highly valuable for Defect localization   ND-at expense of resolution and sensitivity    imaging through   intermediate materials   Increasingly challenged with integration density    Tutorial aimed at proving an insight into LIT and SAM   Existing methods need to be adjusted to novel technologies   AI-signal and Data interpretation   Resolution & Sensitivity enhancement through analytical approaches

Tutorial:

## High-Resolution Non-Destructive  

Defect Localization

![FraunhoferIMWS  Team Non-Destructive  Defect Localization  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d099b896-5a44-4dc4-9407-1fb2246c568a/d099b896-5a44-4dc4-9407-1fb2246c568a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=87f56812cfa8104cfe60fbe5eb4d629119acb77e)
## Dr. Sebastian Brand 

Dept. Electronic Materials and Components Fraunhofer IMWS , Germany

www.imws.fraunhofer.de/ndl

