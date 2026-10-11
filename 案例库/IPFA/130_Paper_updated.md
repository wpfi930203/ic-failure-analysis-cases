---
title: "130_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_04b91517a0ef68db6e944da883d12c187295230462135641
file_size: 1212340
---

## C-TransNet: Automatic Classification Network for  Nanoscale Wafer SEM Defects   

Yibo Qiao 1 , Yining Chen 2\*  1,2 College of Integrated Circuits, Zhejiang University, Zhejiang, Hangzhou 311200, China  2 Phone : (+86)13003630090, Email :  yining.chen@zju.edu.cn

Abstract —Defect analysis is crucial for semiconductor  manufacturing processes, especially for nanoscale processes.  Automated classification of SEM defects can assist engineers in  identifying root causes more quickly, thereby improving yield.  We presents a comprehensive approach using a combination of  Convolutional Neural Network (CNN) and Transformer  networks for classifying wafer defects in semiconductor  manufacturing processes. By fusing CNN and Transformer  networks, we achieve accurate defect classification with fewer  parameters. Experimental results using a real 12-inch wafer fab  dataset demonstrate a classification accuracy of   $\mathbf{97.25\%}$  , even  when dealing with an unbalanced dataset. Consequently, our  method significantly improves the performance of SEM defect  image classification.

Keywords—semiconductor manufacturing, scanning electron  microscope (SEM), computer vision, defect classification

## I.    I NTRODUCTION 

The manufacturing process of integrated circuits involves  complex procedures like film deposition, ion implantation,  etching, and polishing. As circuit components become smaller,  more layers are added to the design. Hence, each chip  undergoes multiple processing steps. Deviations during this  process can lead to defects on the wafer surface. Accurate  defect identification is crucial for engineers to detect  irregularities and make necessary adjustments for improved  production yield.

![Semiconductor   WaferleveldefectsNanoscaleSEMdefect  manufaturingprocess   OGlobalobservation   OMorphologyobservation  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5a437968-a46d-4d15-a23d-eefd97e5db90/5a437968-a46d-4d15-a23d-eefd97e5db90.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215838%3B1743219438&q-key-time=1743215838%3B1743219438&q-header-list=host&q-url-param-list=&q-signature=e767307251fbd533ffbae0f8187dc1857b02c3af)
Fig. 1.   Wafer level defects and Nanoscale SEM defects in semiconductor  production.

Early semiconductor defect detection relied on traditional  methods such as rule-based methods, statistical methods, and  morphological algorithms [1]. These methods consumed a  large amount of manpower. With the emergence of deep  learning technology, it is possible to automatically learn and  extract features from a large amount of a large amount of  training data with limited human intervention. Deep learning  methods have proven potential in improving efficiency in the  field of defect detection Error! Reference source not  found. [2]. However, in semiconductor manufacturing, defect  detection based on deep learning methods mainly focuses on  the distribution patterns of defects on the entire wafer [3], that  is, wafer level defect detection. This type of defect data is very  different from SEM defect data. As shown in  Error!

Reference source not found. , wafer level defects provide a  global observation view of defect distribution, but they lack  detailed information. Morphology observation based on  scanning electron microscopy (SEM) allows for a detailed  examination of nanoscale defects and provides fine attention  to the specific details of defects, which is crucial for  identifying subtle defects that are essential for root cause  analysis [4]. This detailed analysis is crucial for identifying  defect causes related to the process and implementing  corresponding measures to improve production quality and  consistency [5].

Due to the different characteristics between wafer SEM  defect images and natural images, existing classification  networks for natural images cannot be directly applied to SEM  defect classification. Therefore, there is a research gap in the  microscopic analysis of nanoscale defects in SEM  morphology. Overall, various challenges are faced in wafer  defect analysis, including a large class imbalance in SEM  defects, complex defect types, and a lack of publicly available  large-scale wafer SEM datasets for training. Additionally, due  to the urgency of semiconductor manufacturing, the earlier the  root cause of a defect is identified, the more beneficial it is for  yield improvement, which imposes requirements on the  inference speed of automated defect classification networks.

To tackle these challenges, a more effective and precise  defect feature extraction network is required. It should achieve  satisfactory classification and segmentation accuracy with  limited data and have fewer parameters and lighter weight  operations to prevent overfitting and reduce computational  resource consumption.

The contributions of this paper include:

We focus on the crucial issue of defect morphology  classification in SEM root cause analysis.       We propose a SEM defect classification network that  effectively combines Convolutional Neural Network  (CNN) with Transformer architecture.       To facilitate the study of SEM defect morphology  analysis, we collect and annotate a nanoscale SEM  defect dataset from real semiconductor manufacturing  equipment.        Experimental results demonstrate that our proposed  network outperforms the current state-of-the-art  network, achieving a classification accuracy of   $97.25\%$  .

## II.   R ELATED  W ORK 

In the past, manual visual methods and traditional  computer vision techniques were used for wafer defect  detection. However, these methods had limitations such as  low detection accuracy and inability to adapt to complex  defect classes. With the emergence of deep learning,

intelligent methods using deep learning models like CNNs,  LSTMs (Long Short-Term Memory), and autoencoders have  been applied to wafer defect detection. These models have  shown promising results in handling complex problems and  large-scale datasets.

Deep learning models have significantly advanced image  classification tasks. Models like AlexNet, VGG, GoogLeNet,  ResNet, and MobileNet have achieved state-of-the-art results.  Chen et al. developed an online wafer bin pattern recognition  system using supervised learning, addressing the issue of  excessive reliance on product dependency patterns and  derivative patterns [6]. Huang et al. proposed an intelligent  defect detection system for products that utilizes Generative  Adversarial Networks (GAN) to tackle the problem of  insufficient surface defect datasets, enabling the detection of  common defects [7]. Yu et al. introduced a hybrid deep  learning model, presenting a Stacked Convolutional Sparse  Denoising Autoencoder (SCSDAE) that combines CNN and  SDAE to achieve robustness and effective feature learning  through layer-wise accumulation [8]. However, existing deep  learning defect detection research primarily relies on CNNbased model construction. Nevertheless, obtaining global  contextual information has become challenging due to the  limited receptive field of CNN. Inspired by the success of the  Transformer model in language tasks, recent studies have  explored the application of Transformer models in computer  vision tasks. For example, the Vision Transformer (ViT)  model utilizes the attention mechanism of Transformers to  process images [9]. Additionally, there are other Transformer  variants in the computer vision field, such as DeiT and CaiT  models [10]. Swin Transformer introduces a novel  architectural design similar to CNN, which effectively handles  images of various scales [11]. However, the overall  computational complexity of Transformers remains high,  making   them   unsuitable   for   industrial   applications.  Integrating and leveraging the strengths of Transformer and  CNN while maintaining lightweight performance remains a  challenging task.

In this study, we propose a lightweight classification  network that combines the classification component of the  network with both CNN and Transformer. This integration  aims to leverage the strengths of both models while addressing  computational complexity.

## III.   M ETHODOLOGY 

## A.    C-TransNet  

CNN is a widely used structure in the field of image  processing, while Transformer is a recently proposed novel  and excellent structure. In order to address the complexity and  diversity of SEM defect morphology during the chip  manufacturing process, our model combines the structures of  CNN and Transformer, constructing our classification system.  As shown in Fig. 2, the network consists of three CNN blocks  and one Transformer block. The network first extract features  through the CNN blocks, and then input the feature maps into  the Transformer block to obtain more refined features. Finally,  the classification results are obtained through global average  pooling and fully connected layers.

![ClassificationMapping:  Hole  Infilm  Local   Particle  Feature   PatternDeform  Extraction:  Scratch  3   FCN  RB   RB  GAP  GlobalFeatureExtraction  RB   RB   RB  CTT   CIMT  RB   RB   RB  Transformer  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9454f1b5-6589-414c-b6c0-fbbed416184d/9454f1b5-6589-414c-b6c0-fbbed416184d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215838%3B1743219438&q-key-time=1743215838%3B1743219438&q-header-list=host&q-url-param-list=&q-signature=619f236cbe4e0287f32f9e84c6a02e9d2d391ec4)
Fig. 2.   Framework of the proposed method.

## B.    Feature Extraction  

CNN excels in local feature extraction, while Transformer  is suitable for global feature extraction. In order to draw more  attention to the defect parts of nanoscale wafer SEM, we need  to explore a suitable combination of CNN and Transformer for  more refined feature extraction. There are two representative  visualization models of Transformer: Vision Transformer and  Swin Transformer. Among them, Swin Transformer has lower  computational complexity and performs better in small  sample classification. It also has structural similarities with  CNN, making it easier to integrate with CNN. Therefore, our  network chooses to combine Swin Transformer with CNN.  The specific structural parameters are shown in 0.

TABLE I.     C-T RANS N ET  S TRUCTURE  P ARAMETER .

|C- TransNet|Feature Extraction|Feature Extraction|Feature Extraction|Feature Extraction|
|---|---|---|---|---|
|C- TransNet|Part1|Part2|Part3|Part4|
|Block- number|2|2|6|2|
|Block- attribute|CNN|CNN|CNN|Transformer|
|Output Size|56 × 56|56 × 56|56 × 56|56 × 56|
|Channel|64|128|256|512|


In the local feature extraction, we use ResNet Block (RB),  a CNN-based model with excellent performance, for feature  extraction. The RB introduces skip connections on top of the  original network architecture, which can address the issues of  gradient explosion and gradient vanishing caused by network  depth. As shown in Fig. 3, there are two types of residual  blocks in the local feature extraction, both of which have  shortcut connections. When the number of input and output  feature maps is the same, an identity mapping, known as the  Identity Block, is used to directly connect the input and output.  However, when the number of channels is not the same  (doubled), the feature channels do not match, making direct  addition impossible. In this case, a convolutional residual  block, known as the Conv Block, is used. This block adds an  additional convolutional layer on the shortcut connection path,  allowing for channel transformation. Once the channel

numbers match, the Identity Block can be used in series for  feature extraction.

![IdentityBlock   ConvBlock:  3x3 Conv   3x3Conv  Batch Norm   Batch Norm  ReLU   ReLU  1x1Conv  3×3 Conv   3x3 Conv  BatchNorm   Batch Norm  ReLU   ReLU  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7aa64886-c863-4dfc-91ad-9da80c299422/7aa64886-c863-4dfc-91ad-9da80c299422.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215838%3B1743219438&q-key-time=1743215838%3B1743219438&q-header-list=host&q-url-param-list=&q-signature=d4e65a02a5010e847a2f4f3dbe84c180898d8f83)
Fig. 3.   An illustration of the RB.

## C.   CTT   

In the last module, a modified Swin transformer module is  included to match the feature mapping format obtained by the  CNN. It is called CTT (CNN to Transformer) module.

As shown in Fig. 4, the CTT first converts the feature maps  from two-dimensional images to one-dimensional vectors to  integrate the structure of the swin-transformer. This  transformation process is completed by the patchmerge  module. Then, global contextual information fusion and  exploration are achieved by two similar subunits. Each  subunit consists of a normalization layer, an attention module  (Window Multi-head Self-Attention or Shift Multi-head SelfAttention), and an MLP layer. The attention module captures  global   contextual   information   through   cross-window  connections, thereby improving the performance of the  network model. The attention module of the first subunit uses  the Window Multi-head Self-Attention (W-MSA) module,  which only performs self-attention calculations within each  window, ignoring information from adjacent blocks, and there  is no possibility of information interaction between windows.  On the other hand, the Shift Window Multi-head SelfAttention (SW-MSA) module of the second subunit achieves  information interaction between adjacent blocks by moving  the window to the bottom right corner at multiples of M/2 (M  represents the window size), introducing cross-window  connectivity and improving the performance of the network  model.

![14×14.256  PatchMerging(7×7). 512   CTT:  Layer Norm   W-MSA   Layer Norm   MILP  Layer Norm   SW-MSA   LayerNorm   MLP  Reshape  7×7.512  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ca05a069-3c84-4d01-9dc1-fce534001234/ca05a069-3c84-4d01-9dc1-fce534001234.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215838%3B1743219438&q-key-time=1743215838%3B1743219438&q-header-list=host&q-url-param-list=&q-signature=fe7bf277c6cef273d5f8e9a6b960fa09097d7f29)
Fig. 4.   An illustration of the CTT module.

## D.   Classification Mapping  

After multiple feature extraction blocks, a 7x7 feature map  is obtained from the original 224x224 defect image. The  classification mapping is performed through normalization  layer, global average pooling layer (to reduce image size and  prevent overfitting), and fully connected layer. The global  average pooling (GAP) layer reduces the size of the image to  a negligible extent, thereby reducing the computational  resources required for model inference. Additionally, the GAP  layer does not have any learnable parameters, avoiding the  problem of overfitting. Finally, the fully connected (FCN)  layer maps the output of the global average pooling layer to  the final classification result, converting the features into  probabilities for each class. The class with the highest  probability is selected as the predicted defect category.

## IV.   E XPERIMENTAL  A NALYSIS 

This experiment uses NVIDIA GeForce RTX4090,  Windows 11 operating system, and the network model is  coded in Python 3.9 using PyTorch as a deep learning  framework.

## A.   Dataset  

The dataset used for training and evaluating the model  consists of 3,840 SEM images of wafer defects collected from  a 12-inch 55nm fabrication facility. These images were  carefully labeled by skilled engineers on a one-by-one basis to  ensure data quality. Fig. 5 illustrates the examples of wafer  maps and their defect categories in the datasets. The images  have a resolution of   $480\mathbf{x}\bar{4}80$   and are categorized into five  defect classes: hole, infilm, particle, pattern deform, and  scratch.  TABLE II.  lists the distribution of defect categories  in the datasets. We developed a multi-label classification  model using this dataset.

![Pattern  Hole   Infilm   Particle   Scratch  deform  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fd4e7ef6-fee8-4852-9ddd-4ac86d5df260/fd4e7ef6-fee8-4852-9ddd-4ac86d5df260.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215838%3B1743219438&q-key-time=1743215838%3B1743219438&q-header-list=host&q-url-param-list=&q-signature=688e18d10c8e8c855822068489458dfe7f372878)
Fig. 5.   Examples of SEM defect categories.

TABLE II.     D ISTRIBUTION OF THE  D EFECT  C ATEGORIES IN OUR  D ATASETS .

|Defect|Numbers|Proportion|
|---|---|---|
|Hole|750|19.5%|
|Infilm|294|7.7%|
|Particle|1500|39.1%|
|Pattern Deform|750|19.5%|
|Scratch|546|14.2%|


## B.   Evaluation Indicators  

The model's performance is evaluated using several  indicators, including Precision, Recall, and Specificity.   Precision measures the accuracy of the model's predictions for  positive cases. It refers to the proportion of true positive cases  among the predicted positive cases. The calculation formula is  shown in (1), where TP represents true positives (correctly  predicted by the model) and FP represents false positives  (incorrectly predicted by the model). Recall measures the  model's ability to identify a certain type of defect. It refers to  the proportion of true positive cases among the actual positive  cases. The calculation formula is shown in (2), where FN  represents false negatives (incorrectly predicted as other types  of defects by the model). Specificity measures the model's  ability to identify other types of defects. It quantifies the  model's discriminative power. It is defined as the proportion  of true negatives among the predicted other types of defects.  The calculation formula is shown in (3), where TN represents  true negatives and FP represents false positives (incorrectly  predicted as a certain type of defect by the model).

$$\mathrm{Precision}={\frac{T P}{T P+F P}}$$
$$\mathrm{Recall}\!=\frac{T P}{T P+F\!N}$$
$$\mathrm{{specific}}={\frac{T N}{T N+F P}}$$
determines the size of the network. The proposed model has a  storage size of approximately 1/10 of VGG and 1/2 of  ResNet34 and Swin-Transformer. Additionally, the proposed  model achieves the highest accuracy with the fewest number  of parameters.

## C.   Classification Results  

TABLE III.  presents the classification results of the model,  with all indicators for each defect category exceeding   $90\%$  .  This indicates that the combination of CNN and Transformer  in our approach effectively extracts distinctive features of  different defects. The classification effectiveness of each  defect class is analyzed using confusion matrices. The  matrices, shown in Fig. 6, represent the accuracy of each  class's classification for all models. The analysis reveals that  the Pattern Deform category achieves   $100\%$   classification  effectiveness across all models, indicating that defects in this  category are highly distinguishable. On the other hand, the  Scratch category proves to be the most challenging to classify,  with all models struggling to accurately differentiate scratches  from other defect categories. In the proposed model, only  $5.98\%$  of scratch defects are misclassified as particles, and another   $3.14\%$   as holes, resulting in a classification accuracy of  $90.87\%$  for this defect category. This performance surpasses the other  models, which achieve the best accuracy of only   $84.48\%$   for  the Scratch category.

We conducted a cross-comparison between our model and  state-of-the-art existing models. The classification results of  the model are compared with VGG, ResNet34, and SwinTransformer models. VGG is a classical model, ResNet34 is  widely used in classification, and Swin-Transformer is a  recent application of Transformer in computer vision. The  comparison includes accuracy, storage size, number of  parameters, and computation. Detailed results of the  comparison are shown in TABLE IV. . In terms of accuracy,  the proposed model achieves a classification accuracy of   $97.25\%$  , which is higher than any other model in the  comparison table. The storage size refers to the memory  occupied by the model file, and the number of parameters

![Confusion Matrix  100  hole   98.98   0.00   1.00   0.00   3.14  80  infilm   0.00   98.91   1.00   0.00   0.00  60  particle   0.00   1.09   98.00   0.00   5.98  40  patterndeform-   0.00   0.00   0.00   100.00   0.00  20  scratch   1.02   0.00   0.00   0.00   90.87  TrueLabels  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1196ffba-af7a-4d2d-9112-be086db0f97e/1196ffba-af7a-4d2d-9112-be086db0f97e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215838%3B1743219438&q-key-time=1743215838%3B1743219438&q-header-list=host&q-url-param-list=&q-signature=067d1defb4f5eec07036ffa3d089b288b24f74e9)
Fig. 6.   Confusion Matrix. (The four plots represent VGG, ResNet34, SwinTransformer and ours in that order)

TABLE III.

C LASSIFICATION  R ESULTS

|Defect|Precision(%)|Recall(%)|Specificity(%)|
|---|---|---|---|
|Hole|96.1|98.0|99.0|
|Infilm|94.7|94.7|99.6|
|Particle|97.0|98.0|98.1|
|Pattern Deform|100.0|100.0|100.0|
|Scratch|97.1|91.7|99.5|


TABLE IV.   COMPARISON WITH STATE-OF-THE-ART WORKS.

|Method|Accuracy(%)|        Model                Size(MB)      |        FLOPs(                1092      |        Params                （X106）      |
|---|---|---|---|---|
|VGG16|95.29|512.0|123.76|138.36|
|ResNet34|95.69|8１.3|45.25|41.28|
|        Swin-                Transformer      |94.51|105.0|34.97|28.27|
|TransNet)Ours|97.25|54.8|20.50|14.33|


## V.   C ONCLUSION 

We present a novel approach for semiconductor  manufacturing defect classification using a deep learning  model that combines the strengths of CNN and Transformer.  We utilize SEM data collected from real industrial settings to

evaluate the proposed model for nanoscale defects. The  findings indicate that the proposed method improves the  classification performance of SEM defect images. Compared  to other models, it achieves the highest classification accuracy  of   $97.25\%$   with the least computational complexity and  parameter count. This approach has practical applications in  reducing manual workload and enhancing the efficiency of  defect analysis in the industry.

## A CKNOWLEDGMENT 

This research is supported by Zhejiang Provincial  Department of Science and Technology’s 2024 R&D Project  (2024JCZX0031), and SUTD-ZJU IDEA Visiting Professor  Grant SUTD-ZJU (VP) 201906.

## R EFERENCES 

[1]    T. Lechien, E. Dehaerne, “Automated Semiconductor Defect  Inspection in Scanning Electron Microscope Images: a Systematic  Review,” arXiv preprint arXiv:2308.08376 (2023).    [2]    H. Geng, Q. Sun, T. Chen, et al, “Mixed-Type Wafer Failure Pattern  Recognition,”  Proceedings of the 28th Asia and South Pacific Design  Automation Conference. 2023.    [3]    Y. Kim, D. Cho,  J. H. Lee, “Wafer defect pattern classification with  detecting out-of-distribution,” Microelectronics Reliability. Volume  122, 2021.    [4]    E. G. Seebauer, K. W. Noh, “Trends in semiconductor defect  engineering at the nanoscale,” Materials Science and Engineering: R:  Reports 70.3-6 (2010): 151-168.    [5]    D. Malinaric, R. R. Hoffmeister, and C. Sun, “Case study for root cause  analysis   of   yield   problems,”   2000   IEEE/SEMI   Advanced  Semiconductor Manufacturing Conference and Workshop. ASMC  2000 (Cat. No. 00CH37072). IEEE, 2000.    [6]    F. Chen, S.-C. Lin, K. Y.-Y. Doong, K. Young, “Logic product yield  analysis by wafer bin map pattern recognition supervised neural  network,” in: IEEE international symposium on semiconductor  manufacturing, Vol. 1, 2003, pp. 501 – 504    [7]    C.-C. Huang, X.-P. Lin, “Study on machine learning based intelligent  defect detection system, “in: MATEC Web of Conferences, Vol. 201,  EDP Sciences, 2018, p. 01010    [8]    J. Yu, X. Zheng, J. Liu, “Stacked convolutional sparse denoising autoencoder for identification of defect patterns in semiconductor wafer  map, ” Computers in Industry 109 (2019) 121 – 133    [9]    CA. Dosovitskiy, L. Beyer, A. Kolesnikov, D. Weissenborn, X. Zhai,  T. Unterthiner, et al., “An image is worth 16x16 words: Transformers  for image recognition at scale,” arXiv preprint arXiv:2010.11929  (2020).    [10]    X. Li, T. Zhang, Z. Zhang, H. Wei, Y. Qian, “Survey of transformer  research in computer vision,” Computer Engineering and Applications  59 (1) (2023) 1 – 14.    [11]    Z. Liu, Y. Lin, Y. Cao, H. Hu, Y. Wei, Z. Zhang, et al., “Swin  transformer: Hierarchical vision transformer using shifted windows,”   in: Proceedings of the IEEE/CVF international conference on computer  vision, 2021, pp. 10012 – 10022.

