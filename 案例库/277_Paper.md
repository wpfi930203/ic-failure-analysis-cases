---
title: "277_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_2bcc3c6bce606fb20e202d86b2f6f63c7295230462135641
file_size: 809927
---

## Three-dimensional Structure Recognition of Circuit Patterns on Semiconductor Devices  Using Multiple SEM Images Detected in Different Electron Scattering Angles  

Kenji Yasui 1\* , Mayuka Osaki 1 , Atsushi Miyamoto 1 , and Hitoshi Namai 2

1 Hitachi, Ltd., Totsuka-ku, Yokohama City, Kanagawa, Japan.  2 Hitachi High-Technologies Corporation, Ichige, Hitachinaka City, Ibaraki, Japan  \*Phone: +81-80-2098-2429 \*Fax: +81-45-443-9427 \*E-mail: kenji.yasui.rp@hitachi.com

## Abstract   

We propose a method for recognizing the three-dimensional structure of circuit patterns to achieve automatic pattern  width measurement of semiconductor devices using scanning electron microscope (SEM). Pattern measurement requires pattern recognition technique to identify the measurement position from an SEM image. However, pattern  width and brightness values on an image fluctuate according to patterning conditions, type of material, etc., so distinguishing between line and space through image matching based on brightness information is difficult. In view of this  problem, we investigated a line and space discrimination method that focuses on fundamentally different three-dimensional structures (concavity and convexity) and considering that this difference between concavity and convexity  appears as a difference in the scattering angles of secondary electrons, we captured two images corresponding to these  two scattering angles. In this way, we were able to design image feature that portray the difference between line and  space from these two images and perform high-speed and easy capture of concavity and convexity information. In  experiments, the proposed method achieved a  $100\%$   accuracy rate in automatic critical-dimension measurements.  Keywords – CD-SEM, Pattern recognition, Line and space discrimination

## 1.    Background  

With the ongoing expansion of the information society, the  demand for faster and smaller semiconductor devices is  increasing and the circuit pattern is shrinking [1], high  density and highly integrated. Here, to achieve early launch  of semiconductor production lines and stable production  processes, high-precision inspection and measurement  technologies for the circuit pattern dimensions are essential.  The Critical Dimension Scanning Electron Microscope  (CD-SEM)   is   a   widespread   production   process  management   tool. The   CD-SEM   obtains   electron  microscope images of evaluation points and makes CD  measurements of patterns on the sub-nanometer order [2][3].  One-dimensional measurements of line width and hole  diameter are typical CD targets.

Recent trends in device manufacturing control and  performance improvement of CD-SEM is shown in Figure  1. As the circuit patterns is highly integrated, the number of  semiconductor manufacturing processes increase. So, the  number of required evaluation points also increase  dramatically to monitor CD distribution in wafers. The  increase in the number of evaluation points in recent years

has generated a strong need for increasing the success rate  of automatic measurement in CD-SEM to prevent  increasing engineering time such as making and modifying  measuremernt recipes. Automatic measurements require  pattern   recognition   technique   for   identifying   the  measurement position from an SEM image. The  identification   of   the   measurement   position   has  conventionally been based on image matching [4]. The  image matching is broadly divided into so-called image  grayscale-based techniques and feature-based techniques.  Techniques robust to pattern shape deformation in the  imaging target and brightness contrast variation in the  image have also been proposed. In semiconductor device  patterns, line width and brightness values on an image can  fluctuate according to production process conditions, type  of pattern material, etc. Consequently, in a layout having an  alternate arrangement of non-unique lines and spaces, line  and space discrimination by simple image matching based  only on grayscale or the feature on the image is difficult. An  example of an SEM image of a line and space pattern is  shown in Figure 2. Here, the brightness values and  dimensions of these lines and spaces are similar making line  and space discrimination difficult.

![Devicemanufacturing  Device manufacturing  Inspection system Inspection system  ·Increase of the number of manufacturing processes per a wafer ncrease of the number of manufacturing processes per a wafer   · Improvement of automatic measurement success ratio is needed  ·Improvement of automatic measurement success ratio is needed ·Increase of the number of evaluation points per a wafer ncrease of the number of evaluation points per a wafer   Wafer  Wafer Imaging  Imaging Process  Process feedback  feedback Pattern recognition  Pattern recognition Upper image  Upper image  (Enhanced L/S discrimination  (Enhanced L/S discrimination) High-density  High-density   0.9 0.9 1.0 1.0 0.9 0.9 1.0 0.9  CD-SEM  CD-SEM integration  integration  1.0 1.0 1.0 1.0 0.9 0.9 0.8 0 1.0 1.0 1.0 0.9 0   New function:  New function :  Wide Wide   1.1 1.1 1.1 1.0 0.9 0.9 0.8 .1 1.1 1.1   Detecting SE separately  Detecting SE separately   Measurement  Measurement 1.2 1.2 1.2 1.1 0.9 1.0 1.0 2 1.2 1.2 1.1 0.9 1.0 1.  1.5 1.4 1.3 1.2 1.2 1.5 1.4 1.3 1.2 1.2    In two different  In two different  Line Width:32 nm  Line Width:32 nm  LineWidth≤10nm  Line Width ≦ 10nm Narrow  Narrow  1.8 1.6 1.2  1.8 1.6 1.2  scattering angles.  scattering angles. CD distribution  CD distribution  Lower image  Lower image (2009) （2009)   (2017-)  (2017-) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2a52a6ea-2511-4487-801e-ffbd906d5e9b/2a52a6ea-2511-4487-801e-ffbd906d5e9b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=1cb6d1365b9f16c0932a71d1a86afdcaa37f24bb)
Figure.1 Trends in device manufacturing control and performance improvement of CD-SEM

Against the above background, we propose a line and  space discrimination method that focuses on differences in  three-dimensional structures (concavity and convexity) that  correspond to fundamental differences between lines and  spaces. There are currently many three-dimensional  measurement techniques using SEM such as stereo and  photometric techniques [5][6][7][8]. These techniques,  however, are computationally intensive while contributing  to a drop in throughput, and they can also hinder automation  by requiring, for example, the setting of appropriate  processing parameters. As such, they have been difficult to  apply in practice. In contrast, we focused on physical  phenomena in which secondary electrons (SE) scattered  from spaces are partially shielded by lines and studied the  use of two SE detectors that capture the difference in  scattering angles. We also designed image features that  characterize this difference in scattered electrons between  lines and spaces from two images. This method makes for  high-speed and easy capture of concavity and convexity  information. We expect it to lead to robust automatic  measurements even for pattern widths and other dimensions  that fluctuate.

![SEM image  SEM image 100 nm 100nm  Iine  Line  Space  Space  Cross section  Cross section  ofline and  of line and  space patterns  space patterns ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/720908d0-9dae-487f-b2a0-096da24ebc4d/720908d0-9dae-487f-b2a0-096da24ebc4d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=5a774050cbf14702edb5acd4fc96eb95fc17f276)
Figure 2. Example of a line and space pattern in an SEM image  (provided by imec)

## 2.    Proposed Method  

## 2.1.    Concept of Line and Space Recognition  

In this section, we explain the concept of our proposed line  and space recognition method. We first describe the principle of SEM imaging using Figure 3. The SEM scans a  converged electron beam (primary electrons) across an imaging area on a wafer in the x, y directions by raster  scanning. The SEM obtains a two-dimensional image by  detecting SE scattered from each irradiated position and  converting the number of detected electrons into pixel  brightness values.

Now, to capture concavity and convexity information, we  focus on the amount of SE scattered from a line and from a  space as shown in Figure 4. Here, we see that all SE  scattered from a line are detected while SE from the space  are partially shielded by lines. The amount of SE detected  in different scattering angle for lines and spaces, while  dependent on line height and other factors, tends to behave  as shown in Figure 5. This suggests that line and space  discrimination, in principle, can be achieved by comparing  the difference in image brightness between the line and  space portions of line and space pattern. However, it is  known that the total SE count varies according to material,

imaging conditions, etc. [9], so using only differences in  image brightness runs the risk of making errors in line and  space discrimination.

We therefore studied a system for detecting SE separately  in different scattering angles. Referring again to the amount  of SE detected in different scattering angle in Figure 4, the  amount of SE detected from a space is less than that of a  line since SE scattered at low angles (less than angle α in  the figure) are shielded by a line. By comparing the image  brightness between low-angle range A and high-angle range  B, it is expected to detect the difference of line and space. For this reason, we proposed to divide detection range of  SE scattering angle by boundary angle α. We considered  that the signal ratio between these two images could be used  to achieve stable line and space discrimination independent  of total SE count.

Magnetic lens

![Converged  Converged  Detector  Detector electron beam  electron beam Irradiation position  Irradiation position  Secondary  Secondary   y  Imaging  Imaging of electron beam  of electron beam electrons  electrons z y Wafer  Wafer  x Imaging area  Imaging area x ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3721e19e-635e-4196-a325-d6c19eeaacd1/3721e19e-635e-4196-a325-d6c19eeaacd1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=f755759c98d646270e516a081165ac5844f1a88f)
Figure 3. Schematic diagram of SEM imaging

![Converged  Converged   Converged  Converged  electron beam  electron beam  electron beam  electron beam Detector  Detector  Detector  Detector Secondary  Secondary  Secondary  Secondary  electrons electrons   electrons  electrons Iine  Line  _pattern,  pattern (a) Scattered electrons  (a) Scattered electrons  (b) Scattered electrons  (b) Scattered electrons from a line  from a line  from a space  from a space ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1d0d80e0-4811-4afd-b3a3-5ab4d4a34d0a/1d0d80e0-4811-4afd-b3a3-5ab4d4a34d0a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=4ca3b8f6c106c0b646e2479d3a16f1965e7f3e5a)
Figure 4. Electron scattered model of SEM

![Line Iine   A  B Number of  detected SEs  Space  Space 0  AS  45  α  90  90 SE scattering angle[degrees]  SE scattering angle [degrees] ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2b8d18b0-87ad-471a-9ad5-ec04b3ecdd0f/2b8d18b0-87ad-471a-9ad5-ec04b3ecdd0f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=d851f996c48ddabf3bb74efdbb4fd2dd70e3af78)
Figure 5. SE scattering angle distribution

## 2.2.    Electron Optical System  

We studied a configuration consisting of upper and lower  detectors as one means of generating images discriminating  SE scattering angle in the previous section. A schematic  view of the experimental equipment is shown in Figure 6.  In this configuration, SE greater than scattering angle   $\upalpha$   are  detected by the upper detector, and SE less than scattering  angle   $\upalpha$   are detected by the lower detector. Here, since scattering angle α depends on pattern dimensions, we estimated   $\upalpha$   from typical pattern dimensions. In the following, we denote the images obtained from the upper and lower  detectors as  $P_{U}$   and  $P_{L}$  , respectively.

![Upper  Upper  Converged  Converged   detector  detector electron beam  electron beam  (θ: 1arge)  ( θ : large) Lower  Lower  detector  detector (0: small)  ( θ : small) Secondary  Secondary M agnetic lens  Magnetic lens electrons electrons  θ  Wafer  Wafer Figure 6. Optical detection system with two  Figure 6. Optical detection system with two         elevation-discriminating detectors  elevation-discriminating detectors  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5a50b267-363c-40e9-8530-c7f26aeb8a19/5a50b267-363c-40e9-8530-c7f26aeb8a19.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=dad491d390c5e1ba59bbe22ab0917ff89dac0294)
## 2.3.    Feature Value Design  

We calculate image features  f i  $\mathrm{i}\,(\mathrm{i}=1,2,3)$   for line (concavity) and space (convexity) discrimination from the two  images  P U ,  P L . The following describes the calculation  method with reference to Figure 6. First, as a preprocessing  step, we divide the image into segments using pattern edges  as boundary lines to obtain regions  $R$   (Figure 7(a)). We calculate feature values for each region  R . A pattern edge on  an SEM image becomes apparent through a so-called edge  effect that can be observed as a white band, and this turns  out to be suitable for extracting these regions [10].

As described in section 2.1, the signal ratio between the  two images differs between a line and a space, so we determine image ratio  $P_{L/U}$   using the following equation.

$$P_{L/U}\,{=}\,P_{L}/P_{U}$$
(1)

Next, using  $P_{L/U},$   we determine feature value  $f_{1}(\mathbf{R})$   in each  region  $R$   using the following equation.

$$f_{1}(R){=}\operatorname*{min}_{x\in R}\bigl(P_{L/U}(x)\bigr)$$
(2)

An example of a signal profile of   $P_{L/U}$   is shown in Figure  7(b). Feature value  $f_{1}$   is large for a line but small for a space,  which enables line and space discrimination.

On the other hand, it must be kept in mind that the brightness value of an SEM image can change due to sample  charging by electron beam irradiation. An example of a signal profile of   $P_{L/U}$   with a large charge effect is shown in  Figure 7(c). It can be seen here that  $P_{L/U}$  has greatly changed  due to the gradient of the SE scattered distribution caused  by charging and that the degree of separation of the feature  value  $f_{1}$   between a line and a space has dropped. In contrast,  experiments have shown that the image sum   $P_{L+U}$   (total SE  count) given by the following equation is hardly affected by  charging.

$$P_{L+U}\!=\!P_{L}\!+\!P_{U}$$
(3)

To therefore improve the stability of line and space discrimination under charging, we add feature values  $f_{2}(R)$   and   $f_{3}(R)$   calculated by the following equations based on    $P_{U+L}$  .

(4)

(5)

$$\begin{array}{l}{f_{2}(R)\!=\!\displaystyle\sum_{x\in R}\left(P_{L+U}(x)\!-\!\operatorname*{min}_{x\in R}\!\left(P_{L+U}(x)\right)\right)}\\ {\qquad\displaystyle\operatorname*{max}_{x\in R^{\prime}}\left(P_{L+U}(x)\right)\!-\!\operatorname*{min}_{x\in R^{\prime}}\!\left(P_{L+U}(x)\right)}\\ {f_{3}(R)\!=\!\displaystyle\operatorname*{max}_{x\in R^{\prime}}x_{\operatorname*{min}}}\\ {x_{\operatorname*{max}}\!=\!\displaystyle\operatorname*{max}_{x\in R^{\prime}}\left(P_{L+U}(x)\right)}\\ {x_{\operatorname*{min}}\!=\!\displaystyle\operatorname*{argmin}_{x\in R^{\prime}}\left(P_{L+U}(x)\right)}\\ {\qquad\qquad\displaystyle x_{\in R^{\prime}}}\end{array}$$
(6)

(7)

Here,    $R$  ’  is the white-band neighboring region.

Examples of signal profiles of  $P_{U+L}$   are shown in Figure 8.  Feature value  $f_{2}$  quantifies signal swelling between white  bands and feature value  $f_{3}$   quantifies the gradient of signal  change in a white band. Within a space near a line sidewall,   $P_{U+L}$   tends to drop due to shielding of scattered electrons.  The values of both  $f_{2}$   and  $f_{3}$   are expected to be larger at a  space than at a line.

The proposed method aims for robust line and space discrimination under variation in pattern shape, material, and  charge effect. Table 1 summarizes assumed target fluctuations, their image profile variation and the tolerance of the  three feature values  $f_{1},f_{2},f_{3}$  . Although line and space discrimination by a single feature value can be difficult, we  expect all pattern fluctuations to be covered by using three  features complementarity. We therefore plan to perform line  and space discrimination using a support vector machine  (SVM) [11] based on these three feature values.

![R1,R2,R3,R4,R5,R6, R7  R 1  R 2  R 3  R 4  R 5  R 6  R 7 TKTKTKKTK  W  E (a) Image segmentation  (a) Image segmentation R 1  R 2  R 3  R 4  R 5 W  E P PLUT  L/U f(R2)  f 1 ( R 2 )  f(R3)  f 1 ( R 3 ) (b) Signal profile of PuU  (b) Signal profile of  R 1  R 2  R 3  R 4  R 5 W  E P PLU?  L/U f（R2)  f ( R )  f(R3)  f ( R ) 1  2  1  3 (c) Signal profile of P1/U  (c) Signal profile of  with large charge effect  with large charge effect ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/26bf4a14-b179-4454-924a-1381f7bdcdd4/26bf4a14-b179-4454-924a-1381f7bdcdd4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=7b20beeb2e2fd71800e6080a83a7845db07de9fc)
Figure 7. Calculation of feature  $f_{\mathrm{l}}$   using  P L/U

Table 1. Signal profile fluctuations with design variation

||||Line width|Space width|Height, depth|M aterial|Charge effect|
|---|---|---|---|---|---|---|---|
|         Line and space                cross section      ||||| Electron beam|||
|        Signal                profile      |PL+U|||||||
|        Signal                profile      |PIU|||||||
|        All features                Featuref                Featuref                Featuref      ||||||||
|        All features                Featuref                Featuref                Featuref      |Featuref|Featuref||||||
|        All features                Featuref                Featuref                Featuref      |Featuref|Featuref||||||
|        All features                Featuref                Featuref                Featuref      |Featuref|Featuref||||||


![R 21   R  R 222   R 24   R 22s  1  2  3  4  5 W  E 3(R2)  f 3 ( R 2 )  f(R3)  f 3 ( R 3 ) P PL+U  L+U f2(R2)  f 2 ( R 2 )  f(R3)  f 2 ( R 3 ) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/860f744d-1232-4801-a187-852133f0c770/860f744d-1232-4801-a187-852133f0c770.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=33e35559d8f158454f83f045959f49d5a0871495)
Figure 8. Calculation of features  f 2  and  $f_{3}$   using  $P_{L+U}$

## 3.    Experiment  

## 3.1.   Experimental Conditions  

We tested the proposed method using actual images. Specifically, we used a total of 866 sample images taken of  about 4000 lines and spaces in six datasets A to F having  different design rules for evaluation. In addition, in order to  do experiment assuming process variations, datasets A to D  contain with several variations whose design pitch is the  same, but line width vary from original design. There are  five or six groups divided by the similar line width in each  dataset. The fluctuating items shown in Table 1 were included in these six datasets. The images of three typical  samples 1 to 3 are shown in Figure 9. In samples 1 and 2,  the brightness and darkness of lines and spaces are reversed.  In sample 3, moreover, the widths of lines and spaces are  close, which makes line and space discrimination by line  width difficult. Multiple lines and spaces exist in each image, and in the experiment, only successful discrimination  of all lines and spaces are success and a failure otherwise.  We also evaluated conventional grayscale-based template  matching as a comparison experiment with respect to the  proposed method.

![(a) Sample 1  (a) Sample 1  (b) Sample 2  (b) Sample 2  (c) Sample 3  (c) Sample 3 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/43791d38-01a6-416c-80ca-fa0af3e8d973/43791d38-01a6-416c-80ca-fa0af3e8d973.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=5c13b8b47ebf73a151e481e2561ecbeb2c71e920)
Figure 9. Examples of images for evaluation  ((c): provided by imec)

## 3.2   Experimental Results  

The auto measurement success rate including line and  space pattern recognition for each dataset is shown in Figure  10. In the conventional method, we performed evaluations  using an image of a line width group in each dataset as a  template image. In the proposed method, we performed  evaluations using the leave-one-out cross-validation  method to test performance with respect to untrained data.  While the success rate by the conventional method varied  from   $65\%$   to   $100\%$  , the proposed method was successful in  automatic measurements for all data. Since the evaluation  datasets A to D includes various patterns whose line width  is different assuming process variation, the success rate is  low in the conventional method. In figure 11, the success  rate for each line width is shown. In datasets A to D, each  template image is selected from the line width group 3 in  conventional method, and the larger the group number is,  the wider line width is. The success rate decreases as the  line width variation becomes larger. However, dataset A is  an exception, there are two reasons. The first reason is that  the design pitch of group 2 is different slightly from group  3. The second is that the line width variations of group 1 and  2 for group 3 are very small.

On the other hand, the proposed method is not affected by  process variations. The distribution of feature values {f1, f2,  f3} in each of datasets A to F is shown in Figure 12 (a) to  (f), respectively. These results indicate that line and space  feature values are distributed with a high degree of separation and that stable line and space discrimination can be  achieved even for a certain amount of fluctuation.

We performed SVM learning for each dataset in the experiment of Figure 10 and established discriminating  hyperplanes. However, if it were possible to perform common hyperplane learning independent of datasets, the setup  cost of automatic measurements could be greatly decreased.  To test this possibility, we performed line and space discrimination after merging datasets A to F and achieved a  success rate of   $98.2\%$  . In short, while discrimination failed  for a few samples, we were still able to obtain a high success  rate. The distribution of feature values after this merging is  shown in Figure 13. The samples for which discrimination  failed are located at the boundary between the line and space  feature value distributions. These samples at the boundary  were strongly affected by charging, so to improve performance stability, we need to study imaging techniques that  can mitigate charging and feature values and are robust to  charging effects.

![■ Conventional  Proposed  Conventional  Proposed Measurement success rate (%)  100 100  50 SO  0 A  B  C  D  E  F ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/895b78c6-0b47-4ce2-9d42-bbc775bfc9ad/895b78c6-0b47-4ce2-9d42-bbc775bfc9ad.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=268ed509d0b140a3219789493509edd32cdc2d61)
Figure 10. Results of proposed method in each dataset

![Measurement success rate (%)  Conventional  Conventional  Measurement success rate (%)  ■Conventional  Conventional 100  100  Proposed  Proposed  晨100  100  Proposed  Proposed SD  50  SO  50 0  0 se  1  2 ¥34  3  4  5  1  2  3  3 4  4  5 Line width group number  Line width group number  Line width group number  Line width group number (a)Dataset A  (a) Dataset A  (b) Dataset B  (b) Dataset B Measurement success rate (%)  ■ Conventional  Conventional  Measurement success rate (%)  ■ Conventional  Conventional Proposed  Proposed  Proposed  Proposed 100  100  袁100  100 SSS  SO  50  SO  50 0  0 123456  1  2  3  4  5  6  1  2  3  4  5 Line width group number  Line width group number  Line width group number  Line width group number (c)Dataset C  (c) Dataset C  (d) Dataset D  (d) Dataset D ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fc42c958-1738-40b0-90fb-aad9e9813b22/fc42c958-1738-40b0-90fb-aad9e9813b22.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=204749602ab552149cc676bdf0c2893f78baa06b)
Figure 11. Results of proposed method in each line width

![Iine  Line Space Space   f 1  1 f 3  f 2 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/34643b92-54ac-456b-8420-6b2c55c9fb08/34643b92-54ac-456b-8420-6b2c55c9fb08.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=d4a931fa91ac603d01810f818e709165b8d9d99e)
Figure 13. Feature distribution of all datasets

![Line Tine  Line  Line Sp ace  Space f  f Space  Space  1  1 f  f f  2  f  2 3  3 (a) Dataset A  (a) Dataset A  (b) Dataset B  (b) Dataset B Iime  Line  Line  Line f  f Sp ace  Space  1  Sp ace  Space  1 f  f f  2  f  2 3  3 (c) Dataset C  (c) Dataset C  (d) Dataset D  (d) Dataset D Tine  Line  Iime  Line Space Space  f  Space  Space  f 1  1 f  f f  2  f  2 3  3 (e) Dataset E  (e) Dataset E  (f) Dataset F  (f) Dataset F ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7e37f962-3ac8-4081-98a5-6c8b0d0f5e5e/7e37f962-3ac8-4081-98a5-6c8b0d0f5e5e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215685%3B1743219285&q-key-time=1743215685%3B1743219285&q-header-list=host&q-url-param-list=&q-signature=bcc44ac546545f3aa5797d46bb66bfcf276b7735)
Figure 12. Feature distribution of each dataset

## 4.    Conclusion and future work  

In this research, we proposed a line and space discrimination method focusing on three-dimensional structures  (concavity and convexity) with the aim of achieving automatic critical-dimension measurements of semiconductor  patterns using SEM. Focusing on the fact that differences in  concavity and convexity are manifested as differences in the  scattering angle of secondary electrons, we captured two  images for different scattering angles and designed image  feature values that characterizes differences between lines  and spaces from those two images. This method has made  high-speed and easy capturing of concavity and convexity  information possible and has achieved a success rate in automatic critical-dimension measurements of   $100\%$   for each  design rule.

High-precision measurement of pattern shapes is essential  to early launch of semiconductor production lines and stable  production. We expect that automatic critical-dimension  measurements will be achieved by the proposed method to  deal with the dramatic increase in evaluation points in recent  years. Going forward, we plan to perform evaluations for  even more pattern variations and to bring the proposed  method to a practical level of application.

## Acknowledgments  

We extend our appreciation to those concerned at Interuniversity Microelectronics Centre (imec) for providing the  evaluation samples used in this study.

## References  

[1]   International Technology Roadmap for Semiconductors  2.0 Edition, (2015).    [2]   K. Nakahira, A. Miyamoto, and T. Honda: “A fast iterative  technique for restoring scanning electron microscope images”, Nuclear Instruments and Methods in Physics  Research A, Vol.768, pp.89-95, (2014).    [3]   A. Miyamoto and Y. Hojyo: “Generation of large field  SEM image by panorama composition technology for  nano-order measurement”, Measurement Science and  Technology, Vol.27, No.1, pp.025407.1-10, (2016).    [4]   A. Miyamoto and R. Matsuoka: "Automatic Generation of  Imaging Sequence for CD-SEM Using Design Data",  Electronics and Communications in Japan, Vol.99, No.9,  pp.62-71 (2016).    [5]   X. Zhang, et al: “Addressing FinFET metrology challenges in   $1\times$   node using tilt-beam critical dimension  scanning electron microscope”, Proc. of SPIE, Vol.9050,  pp.90500C-1-10, (2014).    [6]   W. Ito, et al: “Novel three dimensional (3D) CD-SEM profile measurements”, Proc. of SPIE, Vol.9050, pp.90500D1-9, (2014).    [7]   A. Miyamoto, D. Chen, and S. Kaneko: “Bootstrapping  de-shadowing and self-calibration for scanning electron  microscope photometric stereo”, Measurement Science  and Technology, Vol.25, pp.105402-1-15, (2014).    [8]   A. Miyamoto, H. Matsuse and G. Koutaki: "Robust surface reconstruction by design-guided SEM photometric  stereo", Measurement Science and Technology, No.28,  No.4, 045405-1-11 (2017)    [9]   L. REIMER: “Scanning Electron Microscopy”,   Springer, (1998).    [10]   A. Miyamoto and H. Honda: “Development of Surface/Embedded Particle Classification Algorithm for  SEM-ADC”, IEICE Trans, Vol.J91-D, No.6, pp.1604- 1612 (2008).    [11]   J.A.K. Suykens, and J. Vanderwalle: “Least Squares Support Vector Machines”, Neural Processing Letters, Vol.9,  pp.293-300, (1999).

