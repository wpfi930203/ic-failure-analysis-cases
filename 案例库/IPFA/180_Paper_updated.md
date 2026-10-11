---
title: "180_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_ed405f8c3b1cbc00b998a97be9ac9b997295230462135641
file_size: 549334
---

## EBSD Method for Measuring Wafer Off-cut Angle  

Fern Lan NG 1 , Jiang  WU 2  1 Singapore Institute of Manufacturing Technology (SIMTech), Agency for Science, Technology and Research (A\*STAR), 5 CleanTech  Loop #01-01, CleanTech Two Block B, Singapore  2 NanoAnalysis, Oxford Instruments (Singapore), 31 Kaki Bukit Road 3 #05-19, Singapore  Phone : (+65)63376848, Email :  wu.jiang@Oxinst.com

Abstract —Crystal orientation and off-cut angle are critical  parameters in semiconductor wafer manufacturing, impacting  epitaxial layer quality and device performance. This paper  presents a novel method utilizing Electron Backscatter  Diffraction (EBSD) to measure the orientation and off-cut angle  of semiconductor wafers, providing a simpler, faster, and more  efficient alternative to X-ray Diffraction (XRD). The EBSD  method involves calibrating the SEM stage, collecting EBSD  data, and analyzing the data based on pole figures. Three  commercial (001) oriented GaAs wafers with different nominal  off-cut angles of   $6^{\circ}$  ,  $14^{\circ}$  , and   $\mathtt{15^{\circ}}$   respectively were studied using  this method.  The measured results by EBSD are   $\mathbf{5.97^{\circ}}$  ,   $14.01^{\circ}$  and   $\mathbf{15.06^{\circ}},$  , demonstrating close agreement between EBSD  measurements and nominal values. Results indicate an average  angular precision of   $\mathbf{0.04^{\circ}}$   and excellent repeatability.  Compared to XRD, EBSD offers advantages in sample  alignment, data acquisition speed, and data processing  simplicity, making it a valuable complement to traditional XRD  techniques in semiconductor manufacturing quality assurance.

Keywords—Orientation, Off-cut angle, EBSD, SEM, Wafer

## I.    I NSTRUCTION 

Crystal orientation and off-cut angle are important  specifications for all types of semiconductor wafers, such as  Sapphire, Si, SiC, GaAs, GaN, AlN, AlGaN, etc.[1-4]. During  semiconductor manufacturing, the wafer surface may exhibit  a small tilt, known as the off-cut or miscut. The off-cut angle  refers to the orientation deviation between the wafer surface  and the ideal crystallographic planes (see Fig. 1) due to wafer  growth, cutting, polishing and other post-processing  techniques [1]. This slight angular deviational influences the  atomic arrangement on the wafer surface and subsequently  impacts epitaxial layer quality and electronic properties [2-4].  In many semiconductor fabrication processes, optimizing the  off-cut angle can reduce dislocation densities and enhance  chemical uniformity, essential for high-efficiency solar cells  and high-performance devices [2-4]. Therefore, measuring the  off-cut angle is crucial for ensuring the quality of wafers and  epitaxial layers in semiconductor manufacturing.

X-ray diffraction (XRD) is the standard technique for offcut angle measurement, providing a precise and nondestructive assessment [5]. Halliwell et al. developed this  method utilizing a high-resolution XRD to determine the  orientation and off-cut angle of semiconductor wafers,  achieving a precision of   $0.01^{\circ}$   [1]. In their study, the off-cut  angle was denoted as the angle α (see Fig. 1a), representing a  small tilt of the wafer surface with respect to the nearest lowindex crystallographic plane in Physics. The process of  determining the cut-off angle through a multiple-axis  diffractometer involves setting the orientations of the sample  holder, mounting the wafer, performing scans to find the  optimal peak position, as well as analyzing the data to  extrapolate the off-cut angle values. To simplify intricate  operations, Johannes et al. improved this method by

integrating a laser-based optical alignment tool into XRD to  aid the system setup [2].

While XRD is a reliable and accurate tool for the off-cut  angle measurement, it has some limitations. Firstly, complex  equipment alignments and calibration procedures can  introduce operational errors and increase measurement  uncertainty [1-2]. Secondly, the time-consuming nature of  data acquisition, which requires repeated scans at four  positions, can prolong the overall measurement process [1-2].  Thirdly, the millimetre-scale X-ray beam is unsuitable for  analyzing nano-scale semiconductor dies and devices.  Therefore, the semiconductor industry is continually seeking  advancements to address these limitations of XRD [4]. This  paper presents a novel method for measuring the orientation  and off-cut angle of semiconductor wafers using electron  backscatter diffraction (EBSD). This method provides simpler  operation, faster data acquisition, and easier data processing  than the XRD method.

## II.   EBSD   M ETHOD 

EBSD is an orientation analysis technique based on  scanning electron microscopy (SEM) with nanoscale spatial  resolution. It determines the local crystal orientations by  detecting and analyzing the electron diffraction patterns  produced when a focused electron beam interacts with the  crystal lattice of a sample [6]. EBSD offers a viable alternative  to XRD for measuring the off-cut angle.

![MD   The (001) planenormal  XRDoff-cutangle  Wafersurface  α:Off-cutangle  GaAs(001)plane  ND  (001)Crystallineplane  CO   Offcutangle  DS   wafersurface  Structure  Crystal System:Cubic-High  Laue Group:   11（m-3m)  Space Group:  216 (F-43m)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f14ac049-2fc7-44e5-a082-644159b472a8/f14ac049-2fc7-44e5-a082-644159b472a8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=37a728266ce0d3e27125e5eb4fbd437d7bf66ac5)
Fig. 1.   (a) Section through the (100) GaAs wafer showing the definition  of the off-cut angle based on the XRD method. Here the off-cut angle is a  small tilt of the wafer surface with respect to the nearest low-index  crystallographic plane, highlighted as α. (b) Illustration of the off-cut angle  inside a GaAs unit cell. Note that this off-cut angle represents the angle  between the real sample surface ( Orange plane perpendicular to ND ) and  the ideal (001) crystal plane (Light blue plane perpendicular to the c-axis).

A.   Displaying orientation and off-cut angle through Pole  Figure

A   pole   figure   is   a   two-dimensional   graphical  representation of orientation, showing the orientation of a  specific crystal plane normal (a pole) with respect to the  sample reference frame [7-8]. Imagine a grain positioned at  the center of a reference sphere and obtain the intersections  with the sphere of the vectors normal to all crystallographic  equivalent planes (hkl) (see Fig. 2a). Here, the reference  sphere is derived from the sample reference frame (or sample  coordinate) with three axes, namely the reference direction  (RD), the transverse direction (TD) and the normal direction  (ND). The plane formed by RD and TD corresponds to the  sample surface, while ND is perpendicular to this sample  surface. Next, draw a line joining the south pole with the  intersection point of the normal vector and the sphere. Project  these intersection points onto the equatorial (TD-RD) plane to  obtain new intersections. The latter intersection points, called  poles, indicate the positions of the (hkl) planes relative to the  sample axes. This procedure is sketched in Fig. 2, showing a  transformation from the   $\{100\}$   planes of a cubic crystal to the  corresponding pole figure.

The pole figure that describes the angular relationships  between crystal planes as the poles can effectively visualize  the off-cut angle. Fig. 2b demonstrates the measurement of the  off-cut angle of a (100) oriented GaAs wafer within a   $\{100\}$    pole figure.  The left image in Fig. 2b illustrates the concept  of the off-cut angle of this GaAs wafer based on the XRD  method, marked as α. Correspondingly,  the α angle is  converted into the distance from a selected pole to the ND (the  centre point of the circle in the pole figure). The selected pole  is the nearest one to the ND among the equivalent (hkl) planes.

To gain a deeper understanding of off-cut angles as  expressed in pole figures, we analyse two different examples.  Fig. 2a is a special pole figure where the off-cur angle is 0. In  this case, ND is completely overlapped with the (001) pole at  the centre of the circle, indicating that the wafer surface is a  real (001) plane in the real space. In Fig. 2b, the off-cut angle  is not 0, with a slight shift between the (001) pole and ND.

## B.   Workflow of EBSD method  

According to the XRD method, we designed an EBSD  workflow to measure the off-cut angle, involving three steps.

## 1)   calibrating SEM stage  

The sample stage calibration plays an important role in  minimizing the instrument error. Sample stage calibration is  the first step in this measurement. Unlike the XRD method, a  single crystal silicon with known orientation is used as an  embedded reference to calibrate the system. The (001) single  crystal Si possessing a tiny off-cut angle, such as NIST SRM  Si, is recommended. Moreover, the samples to be tested and  the standard Si must be mounted on the SEM stage together.

The calibration process may involve tilting/rotating the  SEM stage as well as rotating the standard Si. After these  operations, we aim to obtain a pole figure that is the same to  Fig. 2a in which a (100) pole of Si completely overlaps with  the ND. This ensures that the surface of the SEM stage is  calibrated to the geometry like Fig. 2a.

## 2)   Collecting EBSD data  

The off-cut angle is denoted as a misorientation angle  between a selected crystal plane and the wafer surface in terms  of the EBSD method. Achieving a high-resolution EBSD

measurement requires high-precision EBSD hardware and  indexing techniques. The angular precision (sometimes  referred to as the angular resolution) of routine EBSD analyses  is often quoted as between  $0.5^{\circ}$   and   $1^{\circ}$   [9-10]. To improve the  precision of misorientation measurements, an Oxford  Instruments Symmetry EBSD detector possessing a  megapixel pattern resolution was employed. Moreover,   Refined Accuracy [11], a band refinement approach with an  angular resolution of   ${<}0.05^{\circ}$  , was used as the pattern indexing  method. EBSD map covering 100 pixels was performed in  order to acquire enough orientation data. It is also essential to  conduct EBSD mapping at least three times to derive a mean  value of off-cut angles with reduced statistical error.

## 3)   Analyzing the data  

Commercial EBSD software which can process EBSD  orientation maps and generate pole figures is recommended.  Then, the off-cut angle can be measured using the angular  measurement tool embedded in the software module of the  pole figure.

## III.   E XPERIMENTAL 

Three commercial (001) oriented GaAs wafers with the  nominal off-cut angles of  $6^{\circ}$  ,  $14^{\circ}$  , and  $15^{\circ}$   were studied in this  work, named sample A, B and C, respectively. Samples were  polished on one side and cut into   $10\mathrm{mm}\!\times\!10\mathrm{mm}$   pieces  to  meet the geometric configuration of EBSD. GaAs samples  and the standard Si sample were all mounded on the same  SEM holder using carbon tape. EBSD data were collected at  20kV in a Helios NanoLab 600i FIB equipped with an Oxford  Symmetry CMOS-based EBSD detector. The EBSD  parameters used for orientation mapping were as follows: a  pattern resolution of   $622\!\times\!512$   pixels, 8 frames per pixel,  Refine Accuracy for pattern indexing, a mapping size with

![ND  (a)  (001)  (-100)  TD  >RD   RD  (010)  (0-10)   (001)   (010)  (100)  (100)  ND  （D)  TD  (001)  (0-10)  TD  (001)  (0-10)  >RD   RD  (001)  (100)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/152a5be8-4e2d-409c-b6f1-6b2f495c4c3f/152a5be8-4e2d-409c-b6f1-6b2f495c4c3f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=aececbb94c86489a20a999e8ce33e150f4777ffe)
Fig. 2.  Schematic showing the orientation of a cubic crystal and the  corresponding   $\{100\}$   pole figure. (a) Presentation of the case when the  off-cut angle  $=0$  . (b) Illustration of the case for the off-cut angle  $\neq0$  .  It is represented by the distance between the (001) pole and the ND,  highlighted as the red arrow.

![a   IPF   PolePlotfor(001)-Ga As  IPF Coloring II Zo  G  OOE  2  AngularDistance fromZ [deg]  2   Raster:10x10StepSize:0.7um  (100) -Ga As   <110)-Ga As   <111) -Ga As  Measurement Count:100  Entire Dataset  Half width:10.0  Sample Symm.: Triclinic  Use Sample Symmetry: No  Projection Type: Equal Area  Projection Plane: XY  Hemisphere: Upper  <C)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a377261d-2822-481f-82a8-6b73a9e6de2a/a377261d-2822-481f-82a8-6b73a9e6de2a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=220e2f60d5b21f97ecc735bed854da06fb230b12)
Fig. 3. The off-cut angle measurement using EBSD method. (a) EBSD orientation map of a GaAs (100) single crystal; (b) grain orienation  described by the GaAs unit cell;(c) {100},{110}, and {111} pole figures; (d) the (100) pole plot used to measure the off-cut angle.

100 pixels, etc. EBSD data collection followed the proposed  workflow. First, calibrate the SEM stage based on the pole  figure of Si. By appropriately rotating or tilting the SEM stage,  the Si (001) plane normal was overlapped with the Z-axis on  the pole figure. Next, move to GaAs samples for EBSD data  acquisition and analysis. Two software from Oxford  Instruments, AZtecHKL and AztecCrsytal, were used for  EBSD data acquisition and generation of pole figures,  respectively.

## IV.   R ESULTS 

Fig. 3 presents the typical result obtained from sample C  with the nominal off-cut angle of   $15^{\circ}$  . It is a good example to  interpret the experimental results. Fig. 3a is the orientation  map with a single colour, showing a typical characteristic of a  single crystal. According to the orientation map legend, this  wafer possesses an orientation close to the   $\{100\}$   crystal  planes. Fig. 3b exhibits the sample orientation using a cubic  unit. It shows that the c-axis of the unit aligns closely with the  normal direction of the sample surface (Z-axis or ND). Fig. 3c  presents the pole figures of (100), (110), and (111) planes,  generated by AZtecCrystal software based on orientation data.  Our proposed approach recommends identifying the point  closest to the Z-axis (or ND) to measure the sample's off-cut  angle. This pole is highlighted by an red arrow in the   $\{100\}$  pole figure. Pole plots in AZtecCrystal serve as an useful tool  for this application. Pole plots provide the distribution of poles  as a function of the angle away from a chosen direction. Fig.  3d is the (100) pole plot, revealing distances of all (100) poles  from the Z-axis and facilitating a direct readout of the off-cut  angle from the first peak at   $15.06^{\circ}$  .

Table I lists all off-cut angles measured across three  samples. These data reported here are the mean of at least three  mapping datasets per sample. It took us around 1 minute to  collect one EBSD mapping data. The close agreement  between these EBSD measurements and nominal values,  usually verified via XRD, demonstrates the accuracy and

efficiency of the EBSD method. Further examination of the  average KAM (Kernel Average Misorientation) values  derived from EBSD orientation maps reveals an angular  precision of   $0.04^{\circ}$   in this study.

The difference between XRD and EBSD approach can be  summarized when comparing the experimental procedures  and outcomes. Primarily, XRD offers better measurement  accuracy. However, EBSD excels in determining the off-cut  angle at localized positions on a wafer. Its advantages include  simplified sample alignment, quicker data acquisition, and  easier data processing. If the EBSD method would be applied  to wafer-level samples, tilt-free EBSD technology should be  developed. Ultimately, our proposed EBSD method is a  valuable complement to the established XRD technique.

TABLE I.

MEASURED RESULTS OF THREE SAMPLES

|Sample A|Off-cut angle 5.97°|The nominal value 6°|Average KAM 0.05°|
|---|---|---|---|
|B|14.01°|14°|0.03°|
|C|15.06°|15°|0.02°|


## V.   C ONCLUSION   

The off-cut angle of semiconductor wafers plays a vital  role in determining the quality of epitaxial layers and the  performance of semiconductor devices. In this study, we  proposed an EBSD-based method for accurately measuring  the off-cut angle of (001) GaAs wafers. By following a  carefully designed workflow and utilizing high-precision  EBSD hardware and software, we demonstrated that EBSD  can provide precise measurements of off-cut angles. Our  results show that the off-cut angles measured by EBSD are  very close to the nominal values, indicating the reliability and

accuracy of this method. Compared to XRD, EBSD offers  advantages in terms of sample alignment, data acquisition  speed, and simplicity of data processing, making it a  promising technique for measuring off-cut angles in  semiconductor manufacturing.

## R EFERENCES 

[1]    M. A. G. Halliwell and S. J. Chua, "Determining substrate orientation  using a high-resolution diffractometer," J. Crystal Growth, vol. 192,  pp. 456-461, 1998.    [2]    J. Enslin et al., "Determination of Sapphire Off-Cut and Its Influence  on the Morphology and Local Defect Distribution in Epitaxially  Laterally Overgrown AlN for Optically Pumped UVC Lasers," Phys.  Status Solidi A, vol. 216, no. 6, p. 1900682, 2019.    [3]    M. Reiche, M. Kittler, R. Scholz, A. Hähnel, and T. Arguirov,  "Structure and properties of dislocations in interfaces of bonded silicon  wafers," J. Phys.: Conf. Ser., vol. 281, no. 1, p. 012017, Apr. 2011. doi:  10.1088/1742-6596/281/1/012017.    [4]    K. W. S. Yeung, "The Effect of Offcut Angle on Electrical  Conductivity of Direct Wafer-Bonded n-GaAs/n-GaAs Structures for  Wafer-Bonded Tandem Solar Cells," M.S. thesis, University of  California, Los Angeles, 2012.    [5]    Covalent   Metrology   Services,   "XRD   Offcut   Measurement,"  Whitepaper, 2021.    [6]    R. Borrajo-Pelaez and P. Hedström, “Recent Developments of  Crystallographic Analysis Methods in the Scanning Electron  Microscope for Applications in Metallurgy,” Critical Reviews in Solid  State and Materials Sciences, vol. 43, no. 6. Taylor and Francis Inc.,  pp. 455–474, 02-Nov-2018, doi: 10.1080/10408436.2017.1370576.    [7]    J. K. Mason and C. A. Schuh, "Representations of Texture," in Electron  Backscatter Diffraction in Materials Science, A. Schwartz, M. Kumar,  B. Adams, and D. Field, Eds., Springer, Boston, MA, 2009.    [8]    V. Randle and O. Engler, Introduction to Texture Analysis:  Macrotexture, Microtexture and Orientation Mapping, 1st ed., CRC  Press, 2000, doi: 10.1201/9781482287479.    [9]    F. J. Humphreys, "Grain and subgrain characterisation by electron  backscatter diffraction," J. Mater. Sci., vol. 36, pp. 3833-3854, 2001.    [10]   S. Zaefferer, "A critical review of orientation microscopy in SEM and  TEM," Cryst. Res. Technol., vol. 46, pp. 607-628, 2011.    [11]   K. Thomsen, N. H. Schmidt, A. Bewick, K. Larsen, and J. Goulden,  "Improving the Accuracy of Orientation Measurements using EBSD,"  Microsc. Microanal., vol. 19, no. S2, pp. 724-725, 2013.

