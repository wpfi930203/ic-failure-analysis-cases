---
title: "228_Paper_updated.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_d4caffcdca21995324737c4e72f30cfc7295230462135641
file_size: 2380085
---

##  Improved Defect Detection of Advanced  Semiconductor Packaging in Acoustic Imaging  

Zi-Ying Oh 1 , Shao-Qian Chong 2 , Arya Sukumaran Nair 3 , Bernice Zee 1  1 Device Analysis, Advanced Micro Devices, 508 Chai Chee Lane, Singapore 469032  2 Nanyang Technological University, School of Electrical & Electronic Engineering, 50 Nanyang Ave, Singapore 639798  3 PVA TePla Analytical Systems GmbH, Deutschordenstrasse 38, 73463 Westhausen, Germany  Phone : (65)67969888, Email :  zi-ying.oh@amd.com

Abstract —Subtle defect in advanced packages has become  invisible in conventional acoustic time-domain imaging.  Acoustic Z-Gate collects image and A-scan waveform  information in one file, enabling signal post-processing. This  paper presents a case study using fast Mexican hat wavelet  filtering of Z-Gate file to detect subtle defect. The same filtering  technique is also demonstrated to isolate defect depth in a  stacked X3D package. Early results using signal-based machine  learning, from a small training Z-Gate dataset, to automate  defect detection in X3D package are also presented.

Keywords—acoustic, defect detection, machine learning,  SAM, semiconductor package, wavelet filtering, Z-Gate

## I.    I NTRODUCTION 

Scanning acoustic microscopy (SAM) is a frequently used  failure analysis (FA) tool for visualizing defects in  semiconductor packages without destructive physical failure  analysis (PFA). In the past, to obtain highly resolved acoustic  images for defect detection, one could rely on hardware such  as high-speed analogue-to-digital converter (ADC) for nanoseconds gating, transducers of the right focal length and  frequency as well as active z-axis positioning of the transducer  to achieve optimal results [1]. However, as semiconductor  packages become more complex with the introduction of new  builds of material and architectures like 3D stacking, the  impact of wave attenuation due to absorption, reflection and  scattering of the acoustic wave when it encounters different  material interfaces become harder to overcome [2]. The loss  of acoustic intensity inevitably leads to poor signal to noise  ratio (SNR) of the resultant acoustic image, causing subtle  defects to go undetected. In addition, interconnect sizes are  shrinking rapidly, thus pushing current leading edge acoustic  microscopes to their theoretical resolution limits.

Various works described the use of signal and image  processing algorithms to help overcome this challenge. In the  paper by Brand et al. [3], the author investigated three  different approaches such as Signal Analysis and Parametric  Imaging (SA-PI), Signal Analysis and Defect Evaluation (SADE), and Image Processing and Resolution Enhancement (IPRE) to improve image resolution and contrast to better detect  defects. Particularly, part of the SA-DE processing steps  included wavelet analysis employing a Gaussian mother  wavelet of the fourth order for deriving wavelet coefficients  versus scaling factors and time [3]. Results obtained showed  that significant differences could be observed in the  distributions of the wavelet coefficients between intact and  defective flip chip interconnects. However, this was only  demonstrated on standard flip chip packages and the effects of  signal convolution from multiple reflections within a stacked  die package were not addressed in this paper. A recent paper  by Gupta et al. [4] described the use of 4D block-matching

(BM4D) filter to denoise acoustic volumetric signals and  reduce the noises in acoustic images from SAM. The BM4D  filter utilized the transform domain filtering technique with  hard thresholding and Wiener filtering stages. Again, the  author demonstrated on a sample with relatively large  features. Furthermore, since the filter was applied to a 2D time  domain image, if the image itself was generated from acoustic  signals that had data from more than one interface, the features  from a secondary interface may get enhanced as well, causing  the actual defect to get obscured. Ultimately, a methodology  that has the capability to reconstruct and denoise images from  different interfaces in a stack die would be crucial to expose  subtle defects.

PVA TePla introduced Z-Gate data collection to capture  A-Scan signal of every pixel from a particular gated time to  obtain a 3D file of the region of interest (ROI) [5]. Such data  type enables signal post-processing, which Wolf et al. suggest  in their papers that the application of synthetic aperture  focusing technique (SAFT) in combination with information  compression and filtering techniques could be used for better  defect detection in stack die packages [6, 7]. They discuss the  use of SAFT for imaging structures at various depths of the  package and the use of fast Mexican hat wavelet filtering for  information compression and improvement of SNR so that the  probability of defect detection improves.

Nair et al. presented how Z-Gate file can also be utilized  in signal-based machine learning to train models for  classifying C4 bumps into defect and intact classes in flipchips [5]. Signal-based machine learning will be a more robust  option, than image-based one, to build models for automating  defect detection in advanced semiconductor packaging due to  the abundance of signals available for training from just one  sample.

In this work, the authors explore post-scan signalprocessing of Z-Gate files, via fast Mexican hat wavelet  filtering (in the wavelet software) to reconstruct acoustic  images for isolating defect depth and detecting subtle defects  in complex X3D stacked package. Early results using signalbased machine learning (in AI signal analyzer) of Z-Gate  dataset to automate defect detection in X3D stacked package  are also presented.

## II.   S AMPLE  D ESCRIPTION 

X3D (Extended 3D Technology) stacked package consists  of structural silicon (Si) and X3D die, of   $20\upmu\mathrm{m}$   and   $7\upmu\mathrm{m}$   Si  thickness respectively, stacked on a CPU complex die (CCD)  with copper-pillar (CuP) bumps interconnect, as depicted in  Fig. 1. This increases challenge in determining defect depth  non-destructively as demonstrated in Fig. 2, where changing  acoustic time-domain gating does not bring about significant

changes to the appearance of delamination and CuP bumps  under the structure Si region.  Defect has also become acoustic  invisible in the case of Fig. 3 where no anomaly can be  observed from the acoustic image at the thermal hotspot site  of an X3D part failing power supply short.

![Structural  Si   X3D   Structural  Si  CCD   CCDD  CCDmetals  CuPbump  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bff3646b-1b7f-479c-b691-127549b6ba1b/bff3646b-1b7f-479c-b691-127549b6ba1b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=32796f29bb64566f032d3835994f4d7dd37943a9)
Fig. 1. Cross-section schematic of X3D stacked package.

![175-189ns   175-179ns   180-184ns  cturalSi   X3D  a   CC  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e6dc09b3-a2b8-4dd2-909d-14a9d8200ad2/e6dc09b3-a2b8-4dd2-909d-14a9d8200ad2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=5ee1688ba968e46659e0f2537b28ed8cf8743ee1)
Fig. 2. Acoustic images showing delamination at Structural Si region with  (a) wide 14ns gating and (b) & (c) with consecutive fine 5ns gating.

![Measured:393.70m  Ca  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f80a6f7b-6ce7-4556-b0bf-b10b81ed6391/f80a6f7b-6ce7-4556-b0bf-b10b81ed6391.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=35b909c0781641691f70e5a8a63829f5fce0dfb6)
Fig. 3. (a) Thermal camera image showing hotspot on a X3D part failing  power supply short and (b) the corresponding acoustic image observing no  anomaly.

## III.   M ETHODOLOGY 

Measurements were collected on a PVA TePla  SAM300HD2 scanning acoustic microscope, fitted with  7giga-samplings per second (GSPS) ADC and 200MHz 8 mm  transducer, to obtain Z-Gate files of the X3D samples.  Resulting file size captured from Z-Gate can be up to eight  times smaller than that captured from conventional volume  scan (also known as Z-Scan in PVA TePla’s SAM machines),  reducing time taken for signal post-processing and signalbased machine learning, enabling the subsequent applications  documented in this paper.

process A-scan signals at every pixel in the Z-Gate file  through Mexican hat wavelet filter. Z-Gate file size and the  number of voices input will affect the time taken for this  calculation.

After wavelet calculation completes, the desired gate  parameters, such as gate position and width, can be entered  into the popped-up window, as shown in Fig. 5, for image  reconstruction. Gate parameters here are in samplings,  different from the nanoseconds gating in time-domain  imaging (TDI). Gate starts at 1sampling after filtering.  Depending on ADC speed in the setup, gate size (in  samplings) can be obtained by multiplying the time-domain  gate width with ADC sampling rate, which is set at 7GSPS in  this paper. Hence for a 5ns gate in TDI, 35samplings gate size  should be used for image reconstruction in the wavelet  software.

In the wavelet software (user interface shown in Fig. 4), ZGate file is first loaded, then the number of voices which  determines the level of filtering by specifying number of times  A-scan signal passes through the Mexican hat filter is entered,  and lastly, a wavelet threshold (input between 0.1 to 0.5) to  eliminate low intensity signals. Calculation will then begin, to

![wData  Number of Voices2   Wavelet Threshold0.1  Load Data   Load Data Offline  Calculate Wavelet  veletAppliedImag  ofFliah  Apply Gate  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a010b303-74c2-4386-b59a-24738239e2be/a010b303-74c2-4386-b59a-24738239e2be.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=018ef5745bf55e62313b70b7f3a74098d393fdb8)
Fig. 4. User interface of wavelet software for loading Z-Gate file, entering  number of voices and wavelet threshold.

![AInput  Entergatestart:  EnterGatesize  105  EnterSliding size:  35  OR   Cancel  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/75e4114a-45d4-4642-a94e-96072e7daaa7/75e4114a-45d4-4642-a94e-96072e7daaa7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=df5a3ffb302dcda9e38f131ff7b9578a20784c97)
Fig. 5. Gate selection pop-up window in wavelet software.

Signal-based machine learning is based on the principle  that every feature and defect possesses a unique A-scan  waveform as demonstrated in Fig. 6 example where  delamination waveforms (1 & 2), bump waveforms (3 & 4)  and in-between bump region waveforms (5 & 6) are identical  amongst each feature but differ significantly from others.

![DelaminationA-scan  BumpA-scan  5  In-betweenbu  mpregionA-scan  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9ec8cf07-92cf-47be-a6e1-391bf0f94fc8/9ec8cf07-92cf-47be-a6e1-391bf0f94fc8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=f617c5a070509b51b66b6df02c83d8ca81b71037)
Fig. 6. Acoustic micrograph features with their unique A-scan waveforms.

In the AI analyzer tool, Z-Gate file is first loaded, and  gating is applied to the A-scan waveform to generate an  image for labelling as shown in Fig. 7. Every feature and  defect should be assigned a unique class listed in Fig. 8, and  manually drawn out at the corresponding feature/area. In the  backend software will extract A-Scans from corresponding  ROI. Defect classes are created with augmentation to make  up for limited dataset, as defective features are usually less  abundant than intact features. When this completes, a mask  of the classes and their respective regions (as shown in Fig.  8) will be created and saved for training.

![AAl SignalAnah  BatchLabelTrai  Imagefor  ApplyGate   labelling  Label  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4322f962-3107-4797-99b4-cfeb17c8d706/4322f962-3107-4797-99b4-cfeb17c8d706.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=77fba56584e7f3270c8f6011f97ae4d3a9df6f97)
Fig. 7. Load file and image generation in AI signal analyzer.

![CSAMima   MaskforTraining  Classesfor  labelling  ODefect  ODefectTypell  ODefect Type IlI  OMarginalDefe  Olntact  OStructure  OBackground  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/19280cb1-183f-4d71-9383-1bf500f08200/19280cb1-183f-4d71-9383-1bf500f08200.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=f5c9b4dfc0e464f3113cf09edb941fd6788c4790)
Fig. 8. Classes labelling and mask generation in AI signal analyzer.

In the next step, the mask is loaded into the training  parameters window shown in Fig. 9. Under “Network  Parameters”, Gated Recurrent Unit (GRU) network was  selected for training the X3D sample in this paper while  varying the number of epochs (at 20, 100 and 500). Training  options, min batch size and training and test splits   $(10\%)$   are  maintained throughout the different epoch trainings.

A sequential model will be generated after training  completion. This model is saved, and loaded into the “Test”  window, shown in Fig. 10, together with the Z-Gate file for  prediction. “Apply Gate” produces a SAM image for results  overlay after prediction.

![ Al Signal Analyzer  Label   BatchLabel   Train   Test  LoadData  Network Parameters  Select Network   GRU  Training Options   adam  MiniBatchSize   64  MaxEpochs   20  Test and Validation Split  ValidationSplit(%)   10  Test Split(%)   10  Train Network  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/103f8dd0-bea5-4e17-ba97-e16f443017ea/103f8dd0-bea5-4e17-ba97-e16f443017ea.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=b749edbfa7a368c36c2563e77081eed0e4f0c72f)
Fig. 9. Training parameters input in AI signal analyzer.

![AI Signal Analyzer  Label   Batch Label   Train   Test  Load Data   ApplyGate  A-Scan  Load Network   Run Testing  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4347eb39-1783-469f-b41f-e02a50eb57df/4347eb39-1783-469f-b41f-e02a50eb57df.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=4a818fedba2729990b8e8c302a8646d7b35b4181)
Fig. 10. Prediction window in AI signal analyzer.

## IV.   R ESULTS AND  D ISCUSSION 

## A.   Defect depth isolation  

Reconstructed acoustic image slices obtained in wavelet  software via fast Mexican hat wavelet filtering is presented in  Fig. 11(d-f) corresponding respectively to their time-domain  fine gating images in Fig. 11(a-c). Delamination patch at the  structural Si region appears brightest in Fig. 11(e) and darkens  in the next slice shown in Fig. 11(f) where CuP bumps are  resolved. It can then be deduced that delamination occurred at  the interface above the CuP bumps and CCD metals,  indicating oxide bond delamination between structural Si and  CCD. This is verified from focused-ion beam (FIB) crosssection at the delamination region depicted in Fig. 12, where  oxide bond delamination is observed between CCD and  structural Si.

![175-179ns   180-184ns   185-189ns  mpsresolved  Defe  tappears  a   Cb   C  106-140samplings   141-175samplings   176-210samplings  No bumps  appears  ce   C  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9d90a90a-b0fd-4a34-ba6b-220fd210a9fa/9d90a90a-b0fd-4a34-ba6b-220fd210a9fa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=5a46606631c4ebaa6e7d2577525541f21eb18408)
Fig. 11. (a-c) Conventional time-domain acoustic images obtained via  consecutive fine 5ns gating and (d-f) their corresponding reconstructed  acoustic image slices after fast Mexican hat wavelet filtering, isolating  delamination in slice (e).

![Structural Si  Oxidebonddelamination  CCD  CCDmetals  CuPbump  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/842a41d2-6371-425c-b71a-117eb2ec7b23/842a41d2-6371-425c-b71a-117eb2ec7b23.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=f0e539191fb1204e5bd3f6182c8510bbb51f311f)
Fig. 12. FIB Cross-section of X3D stacked package at acoustic  delamination site showing oxide delamination.

## B.   Subtle defect detection  

Z-Gate file of the X3D reject failing power supply short is  subjected to post-scan fast Mexican hat wavelet filtering in the  wavelet software, and the reconstructed image slice is  displayed in Fig. 13(b). Black dot anomalies, circled in red,  are revealed at the thermal hotspot location on the  reconstructed image slice. This helps to isolate defect  underneath the X3D die, narrowing down ROI to focus for  subsequent PFA.

![Ca  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/89a64a5a-b1ce-46f6-8ff6-e661bad2c4ee/89a64a5a-b1ce-46f6-8ff6-e661bad2c4ee.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=363b7e177222556e23c316e7e51c16390ce19a79)
Fig. 13. Thermal camera image showing hotspot on a X3D part failing  VDDCR_CPU0 vs VSS short failure and (b) the corresponding  reconstructed acoustic image, via fast Mexican hat wavelet filtering,  revealing anomalies at hotspot site.

Parallel lapping was performed on the X3D reject to thin  down underfill and observed Aluminium pad (AP) stringers in  the optical image in Fig. 14. FIB cross-section in Fig. 15  verified AP stringers creating short path between alternating  power supply and ground APs and observed passivation  cracks at this thermal hotspot location.

![ihger  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cb83e3e9-e300-4384-8f8d-27f67536f545/cb83e3e9-e300-4384-8f8d-27f67536f545.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=476c392bbcf4bfc54a0dca4c1aa1e9b8909cc641)
Fig. 14. Parallel lapping revealed AP stringers at black dot acoustic  anomalies and thermal hotspot location.

![AP stringers   Passivation cracks  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/413abbf5-028c-49c8-bda2-a28c57f5c8ff/413abbf5-028c-49c8-bda2-a28c57f5c8ff.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=9d3195f36177746a3e7ab7d39dbf054da16b0a25)
Fig. 15. FIB cross-section of black dot acoustic anomaly verifying AP  stringers and observed passivation cracks.

C.   Automatic defect detection via signal-based machine  learning

The same Z-Gate file from case study A (Defect depth  isolation) is loaded into the AI signal analyzer toolbox for  signal-based machine learning. “Defect” label (in red) is  assigned to the oxide bond delamination region, while “Defect  Type II” label (in blue) is assigned to the bright anomalies  under X3D region, as depicted in Fig. 16. “Intact” label (in

yellow) is assigned to corresponding good reference areas of  “Defect” and “Defect Type II”, while structure (in white) is  used for peripheral regions with different pattern from  “Intact”.

Prediction results from the three models trained with 20,  100 and 500 epochs are presented in Fig. 17. Among the three,  “Defect” and “Defect Type II” are most accurately predicted  in the 100 Epochs model, along with the lowest false detection  of Defect Type I in the X3D region.

![Labellingonacousticimage  Classesfor  Structural Si region  labelling  ODefect  ODefect TypeIl  O Defect Type Ill  O Marginal Defect  intact   X3D region  OStructure  OBackground  Structural Siregion  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/960d5a14-ce63-44f2-a778-2a28a8653f6d/960d5a14-ce63-44f2-a778-2a28a8653f6d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=a17202b3fb75057ebf02fdace7371f1697d5dd2f)
Fig. 16. Labelling of Defect type I, Defect Type II, Intact and Structure.

![Typelldefect  False  detectionof  Typeldefect  TypeIdefect  Typelldefect  20Epochs   100Epochs   500Epochs  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c7f995a9-5420-4a69-8ead-da9963b05737/c7f995a9-5420-4a69-8ead-da9963b05737.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215760%3B1743219360&q-key-time=1743215760%3B1743219360&q-header-list=host&q-url-param-list=&q-signature=aa19924aae12a04755fed89df375126684935289)
Fig. 17. Prediction results of X3D defects after various Epochs training.

The confusion matrix from 100 epochs model,  documented in Fig. 18, suggests room for improvement in the  “Defect” class (in red) due to 12 wrong predictions as “Intact”  and 1 wrong prediction as “Structure”. “Structure” class also  reported 188 incorrect predictions as “Intact”. There should be  unique labels for both “Intact” classes to represent good area  from “Defect” and “Defect Type II” separately. In addition,  more structure labels should be added to further differentiate  the bumps and in-between bump regions as different classes  to improve model performance.

|        13834                16.7%      |0.0%|        12                0.0%      |0.0%|        99.9%                0.1%      |
|---|---|---|---|---|
|0.0%|        10747                13.0%      |0.0%|0.0%|        100%                0.0%      |
|0.0%|0.0%|        57217                69.2%      |        188                0.2%      |        99.79%                0.3%      |
|0.0%|0.0%|0.0%|        680                0.8%      |        100%                0.0%      |
|        100%                0.0%      |        100%                0.0%%%      |        100.0%                0.0%      |        78.3%                21.7%%      |        99.8%                0.2%      |


## V.   C ONCLUSION AND  F UTURE  W ORK 

Advanced signal post-processing has been demonstrated  to improve defect detection in non-destructive acoustic  imaging. Application of fast Mexican hat wavelet filtering to  acoustic Z-Gate file helped to isolate oxide bond delamination  between structural die and CCD in the X3D stacked package  and revealed subtle defect at thermal hotspot location on a  X3D part failing power supply short, which was otherwise not  visible in conventional time-domain acoustic image. In  addition to abovementioned technical advancements, such  post-scan signal processing of Z-Gate files helps to free up  tool time too.

Early results achieved from a small training Z-Gate dataset  via signal-based machine learning opens possibility of  automatic defect detection on complex packages. A major  takeaway in this early study is the impact of labelling  precision on model performance in prediction accuracy. As  sample complexity increases, a larger set of classes will be  required to allocate each feature and defect with a unique  class. Ability to create customized classes will greatly  improve model training. Future work to train good parts to  predict deviations in failed samples is also in the plans.

## A CKNOWLEDGMENT  

The authors would like to thank PVA TePla for sharing  beta versions of wavelet software and AI signal analyzer for  evaluation, their expert advice to setup and optimize signalbased ML for our applications and our  colleagues from  Device Analysis Laboratory, Advanced Micro Devices  (Singapore) for their support.

$\copyright$   2024 Advanced Micro Devices, Inc. All rights reserved.  AMD, the AMD Arrow logo, and combinations thereof are  trademarks of Advanced Micro Devices, Inc. Other product  names used in this publication are for identification  purposes only and may be trademarks of their respective  companies.

## R EFERENCES 

[1]    Z. Y. Oh, F. J. Foo and B. Zee, "Optimization and Application of  Acoustic Imaging for Defect Detection in Stack Die Packages," 2018  IEEE International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), 2018, pp. 1-5.    [2]    J S. Tismer, S. Brand, S. Klengel, M. Petzold and P. Czurratis,  "Acoustic imaging of bump defects in flip-chip devices using split  spectrum analysis," 2013 IEEE International Ultrasonics Symposium  (IUS), Prague, Czech Republic, 2013, pp. 950-953.    [3]    Brand, S., Czurratis, P., Hoffrogge, P. et al. Extending acoustic  microscopy for comprehensive failure analysis applications. J Mater  Sci: Mater Electron 22, 2011, pp. 1580–1593.    [4]    Gupta, S.K., Pal, R., Ahmad, A. et al. Image denoising in acoustic  microscopy using block-matching and 4D filter. Sci Rep 13, 13212  (2023)    [5]    A. S. Nair, P. Hoffrogge, P. Czurratis, E. Kuehnicke and M. Wolf,  "Automated Defect Classification In Semiconductor Devices Using  Deep Learning Networks," 2022 IEEE International Symposium on the  Physical and Failure Analysis of Integrated Circuits (IPFA), Singapore,  Singapore, 2022, pp. 1-8.    [6]    M. Wolf, A. Sukumaran Nair, P. Hoffrogge, E. Kühnicke, P. Czurratis,  Improved failure analysis in scanning acoustic microscopy via  advanced signal processing techniques, Microelectronics and  Reliability 138 (2022).     [7]    M. Wolf, B. Birki, P. Hoffrogge, P. Czurratis, C. Bakre, M. Pacheco,  D. Goyal, "Near-Field Synthetic Aperture Focusing Technique to  Enhance the Inspection Capability of Multi-Layer HBM Stacks in  Scanning Acoustic Microscopy." Proceedings of the ISTFA 2023,  Phoenix, Arizona, USA,  pp. 448-451.

