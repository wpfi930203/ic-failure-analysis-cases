---
title: "196_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_67ad6e251978ddd123ba2e22c2b584a27295230462135641
file_size: 1087712
---

## Supervised Learning Approach in Automated Defect  Detection for Failure Analysis in Scanning Acoustic  Microscopy   

Wai Kit Tang 1 , Kim Hui Yap 2 ,  Kejun Wu 2 , Bernice Zee 1     1 Device Analysis, Advanced Micro Devices, 508 Chai Chee Lane, Singapore, Singapore  2 Nanyang Technological University, School of Electrical & Electronic Engineering, 50 Nanyang Ave, Singapore 639798.  Phone : (65)67969888, Email :  tang.waikit@amd.com

Abstract  — Scanning acoustic microscopy (SAM) is a nondestructive imaging technique commonly used in failure  analysis (FA) to detect defects between the semiconductor  package interfacial layers. With the relentless scaling of package  interconnects it is increasingly challenging for the human eye to  spot defects in an acoustic image. The paper aims to study the  viability of using automated defect detection through a  supervised learning approach to identify defects from an  acquired dataset of acoustic images. A typical dataset of acoustic  images generally suffers class imbalances with more images in  the “normal” class category. Our approach tackles the dataset  volume increment through the usage of image patches for  training. Two pre-trained convolution neural networks (CNN)  are used to distinguish the “anomaly” class image patches. The  Area Under the Receiver Operating Characteristics Curve  (AUROC) attained a value of 0.997 with the implementation of  the EfficientNet architecture.

Keywords—Failure analysis, machine learning, defect  detection

## I.    INTRODUCTION  

Failure analysis (FA) is a crucial step in product design,  reliability qualification, and field reject investigation to  undercover the root cause of failures [1]. Recent  advancements in semiconductor packaging technologies have  enabled form factor reduction, interconnect shrinkage, and  densification. This phenomenon poses significant challenges  for FA as the defects are becoming smaller and more difficult  to detect in high input/output (I/O) density advanced  semiconductor packages.

Scanning acoustic microscopy (SAM) is one of the nondestructive methods used to detect defects occurring between  the interfacial layers of a semiconductor package [2]. The  principle of acoustic imaging involves propagating focused  acoustic waves from a transducer through a medium, typically  distilled water, to the specimen under examination. During the  transmission process, a portion of the waves undergo  reflection and are collected by the same transducer. The  scattering of acoustic waves becomes evident in areas with  inhomogeneity, particularly in the presence of defects.  Currently, defect identification in acoustic images relies  heavily on an FA analyst’s ability to spot differences between  a good reference and a reject. However, as defects shrink and  become obscured by dense front-end-of-line (FEOL)  metallization, this introduces subjectivity and the potential for  human error.

To address the challenge, automated defect detection  becomes an effective tool to aid the analysts’ ability to  recognize failure sites. Fig. 1 relates the finding of “anomaly”  sites to the corresponding physical defects.

![a  CD   Die   Delamination  Bump  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e7d51007-e6e7-42dc-ab00-700ed967e6f9/e7d51007-e6e7-42dc-ab00-700ed967e6f9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215884%3B1743219484&q-key-time=1743215884%3B1743219484&q-header-list=host&q-url-param-list=&q-signature=ce9ae45d886a44f13ad8ae3f99d9abbadb733196)
Fig. 1.   (a) An “anomaly” in acoustic imaging corresponding to (b)  Delamination in the back end of line (BEOL).

Creating an acoustic image dataset from production units  for utilization in machine learning training is a formidable  task. The challenge stems from the scarcity of training data for  the “anomaly” class image label. The constructed dataset is  generally imbalanced with overwhelming numbers favoring  the “normal” class image label. The following Fig. 2 depicts  the different class labels assigned to the acoustic images.

![Ca  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ad3c575b-31f4-47b4-908e-5d24bf191b14/ad3c575b-31f4-47b4-908e-5d24bf191b14.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215884%3B1743219484&q-key-time=1743215884%3B1743219484&q-header-list=host&q-url-param-list=&q-signature=cf87237df0c33b261f81dbd54a62d450d28979b1)
Fig. 2.   (a) An acoustic image labeled as “anomaly” (b) An acoustic image  labeled as “normal”.

In this paper, an acoustic image dataset was created from  SAM images of a product undergoing accelerated stress  testing (AST). Products undergoing AST typically exhibit a  higher probability of failure, with the occurrence of defects  manifesting in the form of delamination at the interfaces, thus  contributing to the “anomaly” class image label. The  following Table I highlights the composition of the acoustic  image dataset collected for this study.

TABLE I.     A COUSTIC  I MAGE  D ATASET

|Dataset|Image Class|Image Class|
|---|---|---|
|Dataset|“Normal”|“Anomaly”|
|Number of images|118|21|


## II.   P ROBLEM  S TATEMENT   

As the dataset is small and unbalanced with more images  in the “normal” class category, the conventional approach  towards supervised learning is not applicable. This is  especially so when convolution neural networks (CNN) work  under the assumption that the dataset is huge and balanced. In  this paper, the approach to increase the dataset volume was  executed by dividing the image into image patches as the input  training data. These image patches were identified  individually to facilitate proper labeling on all patches.  Subsequently, the training data are fed into pre-trained CNN  networks such as ResNet [3] and EfficientNet [4]. The  performance of the models to distinguish both “normal” and  “anomaly” image patches is then verified through the area  under the receiver operating characteristic curve (AUROC).

## III.   P ROCEDURE 

## A.   Dataset Preparation  

The dataset comprises images obtained from SAM on a  product undergoing AST. SAM parameters were maintained  consistently for the scans and all the images were verified by  an analyst for accurate identification of the “anomaly” region.  The decision to select the image patches of   $32\mathrm{~x~}32$   size for  training purposes was to ensure that the analyst had an ample  viewing window to label each image patch as “normal” or  “anomaly” accurately. As illustrated in Fig. 3 comparing the  same “anomaly” patch in   $16\textbf{x}16$   and   $32\textbf{x}32$  , neighboring  information was inadequate for accurate labeling in the   $16~\mathrm{{x}}$    16 patch size.

![ca   C    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9e583cb7-8465-41f7-ae4c-56028ca66e93/9e583cb7-8465-41f7-ae4c-56028ca66e93.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215884%3B1743219484&q-key-time=1743215884%3B1743219484&q-header-list=host&q-url-param-list=&q-signature=34f81c8469a246d6dddfaa59774e49b9add61478)
Fig. 3.   (a)   $16\mathrm{~x~}16$   image patch and (b)  $32\;\mathbf{x}\;32$   image patch.

Before dividing the image into patches, the background  border was removed from the acoustic images. For the  anomaly regions, cropping was performed to generate  $32\;\mathbf{x}\;32$    patches, and subsequent image augmentations were applied to  maintain an 8:2 normal and anomaly image ratio. In addition,  a   $50\%$   overlap of the pixel areas with the neighboring image  patches was implemented to augment the number of image  patches. These steps contributed to approximately 34,000  image patches for training inputs as shown in Table 2. The  dataset preparation flow is described in Fig. 4 and samples of  the “anomaly” class and “normal” class image patches are  illustrated in Fig. 5. The image patches were subjected to  transformations such as resizing to 224 pixels and normalized  with mean [0.485, 0.456, 0.406] and standard [0.229, 0.224,  0.225].

![Divide into  Remove   patchesof  Background   32X32    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dede14fe-3a76-4e00-a4dd-289f27b53195/dede14fe-3a76-4e00-a4dd-289f27b53195.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215884%3B1743219484&q-key-time=1743215884%3B1743219484&q-header-list=host&q-url-param-list=&q-signature=d2e8d070841360a319d94125f9775c029091d995)
Fig. 4.   Dataset preparation overview.

![a  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/88ccddf6-4afc-467e-82f7-21d98dbe081d/88ccddf6-4afc-467e-82f7-21d98dbe081d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215884%3B1743219484&q-key-time=1743215884%3B1743219484&q-header-list=host&q-url-param-list=&q-signature=de3f2b6e381c7f5cd7504944620f2ed43d032d94)
Fig. 5.    (a) “Anomaly” image patches (b) “Normal” image patch.

TABLE II.

A UGMENTED  A COUSTIC  I MAGE  D ATASET

|Image patches|Augmented dataset|Augmented dataset|
|---|---|---|
|Image patches|Training|Testing|
|Number of image patches|33937|17012|


## B.   CNN Architectures  

In the context of a small dataset, pre-trained CNN  networks are viable options for classifying the image patch  classes. In this paper, two pre-trained CNN models, namely  ResNet-18 and EfficientNet-b0, were explored to assess the  feasibility of their application on the acoustic image patch  dataset. ResNet architectures tackle the vanishing gradient  problem through the usage of residual blocks to establish a  direct connection between layers for facilitating gradient flow  [3]. EfficientNet, on the other hand, employs a compound  scaling method that uniformly scales the dimension of the  network to enhance model accuracy and efficiency [4]. Both  models have established good performance in image  recognition tasks in other commonly available datasets. The  following Fig. 6 and Fig. 7 illustrate the flow of the ResNet18 and EfficientNet-b0 Architectures respectively.

![3x3conv,64  3x3 conv, 256, /2  3x3 conv, 64  3x3 conv, 256  3x3 conv,64  3x3 conv, 256  T  3x3 conv,64  3x3 conv, 256   3x3 conv, 64  3x3 conv, 512, /2  3x3 conv,128,/2  3x3 conv, 512  3x3 conv,128  3x3 conv,512  3x3 conv,128  3x3conv,512  3x3 conv,128  Average Pool,FC  Output  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3eceda76-cd35-4c00-9d2a-a49852966cb1/3eceda76-cd35-4c00-9d2a-a49852966cb1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215884%3B1743219484&q-key-time=1743215884%3B1743219484&q-header-list=host&q-url-param-list=&q-signature=9fa3686926dc625a50ece87c88c9804d052b285b)
Fig. 6.   Schematic of the ResNet-18 network on the SAM image patches,  conv refers to convolution block.

![Conv,3x3  MBConv6,5x5  MBConv1,3x3  MBConv6,5x5  MBConv6, 3x3  MBConv6,5x5  MBConv6,3x3  MBConv6, 5x5  MBConv6,5x5  MBConv6,5x5  MBConv6,5x5  MBConv6,5x5  MBConv6, 3x3  MBConv6,5x5  MBConv6,3x3  MBConv6,3x3  MBConv6, 3x3  Average Pool, FC  Output    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d137d475-bf36-4680-a57d-fb8683ff1e5f/d137d475-bf36-4680-a57d-fb8683ff1e5f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215884%3B1743219484&q-key-time=1743215884%3B1743219484&q-header-list=host&q-url-param-list=&q-signature=5032320c11917a64fbd96a5c675b54128a1e745b)
Fig. 7.   Schematic of the EfficientNet-b0 network on the SAM image  patches, MBConv refers to an inverted residual block.

## IV.   R ESULTS  A ND  D ISCUSSION 

## A.   Performance Metrics  

Anomaly detection falls under a binary classification in  which the classes of image patches fall into either the  “normal” or “anomaly” class. Hence, AUROC is a suitable  metric to evaluate the performance of the classifier for binary

classification [5]. A higher value of the AUROC will indicate  a better performance of the classifier in separating the  “normal” class and “anomaly” class image patches.

The two parameters of the AUROC are the true positive  rate (TPR) and false positive rate (FPR). The TPR is denoted  by the following equation:

$$\begin{array}{r}{T P R=\frac{T P}{T P+F N}}\end{array}$$
TP represents the true positive referring to the number of  image patches classified correctly as “anomaly” while FN  represents the false negative which refers to the number of  “normal” image patches classified as “anomaly”. The second  parameter FPR is denoted as follows:

$$\begin{array}{r}{F P R=\frac{F P}{F P+T N}}\end{array}$$
FP represents the false positive referring to the number of  image patches classified wrongly as “anomaly” while TN  represents the true negative which refers to the number of  image patches correctly classified as “normal”. With the TPR  plotted against the FPR, the receiver operating characteristics  curve can be plotted and the AUROC value can be tabulated  from the area under the curve as shown in Fig. 8.

![AUROC  1FPR  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a123a5d0-2e4c-42ad-aad8-68fd04c16bf3/a123a5d0-2e4c-42ad-aad8-68fd04c16bf3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215884%3B1743219484&q-key-time=1743215884%3B1743219484&q-header-list=host&q-url-param-list=&q-signature=5df917f25cb2f21f4dd2f6994615daeb92f8ad38)
Fig. 8.   A typical AUROC curve.

## B.   Experimental Results  

The following Fig. 9 and Fig. 10 displayed the AUROC  scores and the corresponding curves.

![ROC  1D  0.8  04  02  AUROC=0.989  O_O   02   0.4   0.6   0.8   10  FPR  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8c46500f-df78-4a5c-9f5d-abc194f3eae3/8c46500f-df78-4a5c-9f5d-abc194f3eae3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215884%3B1743219484&q-key-time=1743215884%3B1743219484&q-header-list=host&q-url-param-list=&q-signature=38da22f9e7e3f6d1c1d430178fc04be5f50a7d3f)
Fig. 9.   AUROC score of ResNet-18 network.

![ROC  10  0.8  0.6  0.4  0.2  AUR0C=0.997  0_0  0.0   0.2   0.4   0.6   0.8   1.0  FPR  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c4b778b9-3bda-4413-a0f1-27448ea76bbc/c4b778b9-3bda-4413-a0f1-27448ea76bbc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215884%3B1743219484&q-key-time=1743215884%3B1743219484&q-header-list=host&q-url-param-list=&q-signature=adc02b92ee8d6a9b0b45f19f1d2bc1a652108514)
Fig. 10.    AUROC score of EfficientNet-b0 network.

The performance of both networks on the acoustic image  dataset was validated by the high AUROC scores. The score  was largely attributed to the significantly large number of  “normal” class image patches. The EfficientNet-b0 AUROC  score of 0.997 signified that despite a small number of  “anomaly” image patches, most of them were correctly  predicted by the model. The results further established that the  supervised learning approach through image patches was a  viable option for automated defect detection in acoustic  images for failure analysis purposes.

## C.    $50\%$   overlapping of image patches  

Using a  $50\%$   overlap of the image patches, the “anomaly”  test patches can be fed to the model up to 4 times thus the  location of the anomaly was still effectively determined when  the neighboring patches predicted an “anomaly” class label.  This is illustrated in Fig. 11.

![a  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/35fe59cb-3b3c-4e08-a537-bac37d09f552/35fe59cb-3b3c-4e08-a537-bac37d09f552.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215884%3B1743219484&q-key-time=1743215884%3B1743219484&q-header-list=host&q-url-param-list=&q-signature=0e2fe2fc4d7b313c4132fe2d21378e0ed29effd7)
Fig. 11.    (a) Wrongly predicted image patch, (b) Correctly predicted image  patches, (c) Illustration of deteming defect through neighboring predicted  image patches. Blue for wrongly predicted image patches and red for  correctly predicted image patches.

The identified patches would count as 3 true positive  patches and 1 false negative patch. However, in our failure  analysis workflow, where the objective is to assist the human  analysts, having 3 image patches identified as anomalous  aligns collectively aids the analysts in focusing attention on  that specific region. This application aligns with the  overarching goal of utilizing automation in acoustic image  analysis to facilitate and enhance the efficiency of human-led  failure analysis work.

## D.   Limitations   

In terms of dataset preparation, relatively more effort was  required in labeling the dataset for the supervised learning  approach using the different CNN architectures. It involved  careful filtering of the image patches containing the  “anomaly” from the pool of image patches obtained from the  acoustic images. This process was labor-intensive and timeconsuming as the classification of the image patches had to be  verified by the FA analyst. In addition, in the case of unseen  defects, the trained model would not be able to recognize the  defects. Therefore, the dataset used for training the model had  to contain a representative class of all the defects. However, it  was not possible to obtain a dataset to represent all possible  classes of defects through the images.

## V.   F UTURE WORK 

## A.   Unsupervised learning  

Labeling on all image patches was critical for training  under supervised learning, hence the dataset preparation for  unsupervised learning could be more practical for failure  analysis. It aligns better with the industry's need by leveraging  the abundance of “normal” class images for training. In  addition, an unsupervised learning approach potentially  overcomes the case of unseen defects as they are classified not  in the “normal” cluster.

B.

Other Non-Destructive Imaging Techniques

A similar strategy of using image patches for increasing  dataset volume to apply machine learning approaches could  be applied to other imaging techniques such as X-RAY  imaging. Further exploration of the method in other imagebased FA techniques would provide a bridge between failure  analysis challenges and potential automation solutions.

## VI.   C ONCLUSION   

In this paper, we introduced the strategy of using image  patches as training inputs to increase the dataset volume for  supervised learning. Two pre-trained CNN networks were  used on the image patches dataset and attained an AUROC  value of 0.997 through the EfficientNet-b0 architecture. The  identification of the “anomaly” class image patch  subsequently assisted the failure analyst in locating the site for  physical failure analysis.

## A CKNOWLEDGMENT 

The author would like to thank staff from the School of  Electrical & Electronic Engineering, Nanyang Technological  University (NTU) Singapore as well as colleagues from the  Device Analysis Laboratory, Advanced Micro Devices  (Singapore) for their support.

$\copyright$   2024 Advanced Micro Devices, Inc. All rights reserved.  AMD, the AMD Arrow logo, and combinations thereof are

trademarks of Advanced Micro Devices, Inc. Other product  names used in this publication are for identification  purposes only and may be trademarks of their respective  companies.

## R EFERENCES 

[1]    Zulkifli, S. M., Zee, B., Qiu, W., & Gu, A. (2017, July). High-res 3D  X-ray microscopy for non-destructive failure analysis of chip-to-chip  micro-bump interconnects in stacked die packages. In 2017 IEEE 24th  International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA) (pp. 1-5).     [2]    Mehr, M. Y., Bahrami, A., Fischer, H., Gielen, S., Corbeij, R., Van  Driel, W. D., & Zhang, G. Q. (2015, April). An overview of scanning  acoustic microscope, a reliable method for non-destructive failure  analysis of microelectronic components. In 2015 16th International  Conference on Thermal, Mechanical and Multi-Physics Simulation and  Experiments in Microelectronics and Microsystems (pp. 1-4).    [3]    He, K., Zhang, X., Ren, S., & Sun, J. (2016). Deep residual learning  for image recognition. In Proceedings of the IEEE conference on  computer vision and pattern recognition (pp. 770-778).    [4]    Tan, M., & Le, Q. (2019, May). Efficientnet: Rethinking model scaling  for convolutional neural networks. In International conference on  machine learning (pp. 6105-6114).     [5]    Hanley, J. A., & McNeil, B. J. (1982). The meaning and use of the area  under a receiver operating characteristic (ROC) curve. Radiology,  143(1), (pp. 29-36).

