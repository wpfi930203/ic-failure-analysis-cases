---
title: "211_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_a479374f0f6c3d4d9c0152140c8d88947295230462135641
file_size: 1934565
---

## Endpoint Detection Methods in Implementing  AI-assisted Polishing Process  

Hao TAN\*, Jacobus LEO, Shreyas M PARAB, Krishnanunni MENON, Yuzhe ZHAO, Yanlin PAN,  Changqing CHEN and Pik Kee TAN  GLOBALFOUNDRIES Singapore Pte. Ltd., 60 Woodlands Industrial Park D Street 2, Singapore, 738406, Singapore.  \* Phone: +65-66702865   Fax: +65-66700425   Email:  hao.tan@globalfoundries.com

Abstract-   Sample preparation plays a critical role in the failure  analysis process of modern IC chips. The common problem in  sample preparation is over-polishing. To reduce this problem, an  AI-assisted monitoring system can be deployed, which can  evaluate the progress of sample polishing process and suggest the  steps following up. However, to build such an AI system, a  tremendous number of images with proper classification are  needed. To prepare these images, a reliable endpoint detection  method for image analysis is necessary. In this paper, two  endpoint detection methods are studied, and grayscale line profile  analysis is discussed in detail. The current results are very  promising for further development.

## I. I NTRODUCTION 

Modern IC chips’ back end of line (BEOL) structures can be  considered as several film layers stacked on the front end of line  (FEOL) layer built on the silicon substrates. As illustrated in  Fig.1, a typical BEOL stacking has a few metal layers, some of  which are using low-k dielectric material. Generally, failure  analysis (FA) involves removal of a few film layers before the  defect is visible or detectable by physical inspections or  electrical approaches such as nano-probing and passive voltage  contrast imaging techniques (by either electron or ion beam).  Obviously, sample preparation plays a critical role in the quality  of the FA process. The common problem in sample preparation  is over-polishing. If we can build an AI-assisted monitoring  system, the FA engineers just need to put the sample under a  microscope to capture an image of the surface morphology  from the sample being polished, and the AI will evaluate the  image captured and tell what BEOL layers are present on this  image. Moreover, the AI may judge if the polishing target has  been achieved and advise the polishing recipe next, and  consequently, the over-polishing problem can be avoided.

information identified. Obviously, this categorization process  will be very time-consuming and almost impossible if it is done  manually. Therefore, it will be of great importance to develop  endpoint detection methods to map out the image BEOL  information automatically. In this study, we will discuss two  endpoint detection methods with examples.

Keywords  –  Endpoint detection, AI-assisted, Polishing Process .

Fig. 2 shows the flow chart of one way to implement such a  system mentioned above: raw pictures are collected as the  unclassified learning materials, which cannot be directly used  for machine learning. After proper image processing, those raw  pictures will be mapped out with BEOL information and  classified accordingly. Eventually, the AI system can be built  through machine learning and/or deep learning from the  classified pictures [1] – [4].

Generally, machine learning and deep learning require a huge  amount of well-categorized data, in this case, lots of images of  the polished sample surface with proper BEOL film layer

|Si02|Si02|Si02|
|---|---|---|
|Si0z|Si0z|Si0z|
|low-k|4||
|low-k|3||
|low-k|2||
|low-k|low-k|low-k|


![RawPictures  Automatic Processing:  Endpoint Detection  Classified  Pictures  Machine Learning /  Deep Learning  Al-assisted  Polishing Process  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b6ec9471-3a82-4f0b-a548-a02bfcd81528/b6ec9471-3a82-4f0b-a548-a02bfcd81528.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=04421625e347963d47605859304df3eff343ab81)
Fig. 2 Flow chart of implementing an AI-assisted polishing process.

## II.   EXPERIMENTS  

General 40nm IC chips were used for polishing process  studies. The optical microscope images during polishing were  taken by a CCD camera.  A self-developed LabView  application based on the Vision Assistant module of National

Instruments (NI) [5] was used for image processing and  analysis.

## III. RESULTS AND DISCUSSION  

During the polishing process, the sample surface morphology  will evolve as the BEOL film layers are being removed away  gradually. Fig. 3 shows the sample surface pattern before and  after polishing process. It can be seen from this figure that the  surface pattern is getting irregular with several new features  formed after polishing. There are several ripples formed near  the left edge of the figure. The ripple patterns are formed almost  on every polished sample and can be considered as a typical  polished surface feature. Based on our experience, these ripples  stand for different FEOL/BEOL layers and we would like to  extract this layer information from the ripple patterns.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/11f77cfd-ddbc-46df-8fcb-8f137766727a/11f77cfd-ddbc-46df-8fcb-8f137766727a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=a7c225ec758a673e8fa70a1bf6591f119b28cb8e)
Fig. 3 Surface pattern morphology before and after finger polishing process.

Fig. 4 shows the ripple pattern on another polished sample.  We tried the grayscale line profile analysis method over the  picture: set different sampling lines over the region of interest  and check the grayscale intensity profile on each line.  Normalization was applied to the raw data and four profiles  (corresponding to the four lines in Fig. 4) are illustrated in Fig.  5.

It can be seen clearly in Fig. 5 that there is a group of four  small side by side peaks in each profile curve, as indicated by  the dotted boxes in Fig. 5. This group of four peaks stands for  the first four metal layers above contact, namely M1, M2, M3,  and M4.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a9545df3-f686-4cf4-b81c-5651a84791d4/a9545df3-f686-4cf4-b81c-5651a84791d4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=cf6a538f59b41c0acb3584f8179fd2d2fa13ebc9)
Fig. 4 Relationship between ripples and film stacks.

![() si ni)  200300400500600700800   90010001100  Distance X (pixel)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a59d48f-c415-47b8-be0a-924a816425e8/7a59d48f-c415-47b8-be0a-924a816425e8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=1bb3a36cc6187f8d79385853b5ea730f5b1fdd6b)
Fig. 5 Grayscale line profile traces.

Fig. 6 shows the overlay of the grayscale profile of line 4 in  Fig.s 4 and 5 with the actual sample surface. It is very clear  from Fig. 6 that the peaks stand for their corresponding BEOL  film layers and where the FEOL contact (CA) layer is. With this  information, the BEOL boundaries can be detected in each  sampling line and the BEOL map can be drawn by connecting  the pixel location from those peaks of the same BEOL film  layer. For demonstration purpose, there are only four sampling  lines in Fig. 4. In the real case, more lines can be added to  construct a high-resolution BEOL terrain map.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/022a58db-fe1b-4bd0-93d6-5f76628b7d12/022a58db-fe1b-4bd0-93d6-5f76628b7d12.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=9b0ce330b4b28feaf69d39db45a98a2780c89dd2)
Fig. 6 Grayscale line profile and ripple pattern comparison.

To further test the grayscale line profile method, we applied  this method to other samples and Fig. 7 shows one of those  samples.

It can be seen from Fig. 7 that the ripple feature also exists in  this sample and a few distinctive peaks can be identified from  the profile lines.

![(a)   FEOL    （D>  (b)    FEO  1>x  2m1msm  1100   1150   1200   1250   1300   1350  Distance X (pixel)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fc7ab665-f582-4b86-a9b0-fcc770183459/fc7ab665-f582-4b86-a9b0-fcc770183459.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=5649160985a9a9c9e5e3a6abab42245ae45fa74d)
Fig. 7 Line profile studies on another IC chip. (a) Sample surface and the profile  lines; (b) Grayscale line profile traces.

So far, we have demonstrated that the grayscale line profile  method can successfully extract BEOL information from  images of the polished sample surface with ripple patterns.  What if there is no ripple pattern formed yet? For example,  when the polishing is just started, no material has been removed  and there is no new pattern formed yet. In this case, we can use  the pattern matching method: the initial status of the sample  surface is recorded as the template, during the polishing process,  a series of images will be taken and pattern matching algorithm  will try to identify the template within each image obtained. If  the algorithm failed to identify the template in the image, then

that area can be labeled as a new BEOL region, as its upper  BEOL layer has just been removed.

Fig. 8 shows an example of the pattern matching method. Fig.  8(a) is the template image taken at T0, i.e., before polishing  started (M7 of BEOL stacking), while Fig.s 8(b) to 8(d) were  taken after polishing for 90s, 390s, and 510s, respectively.

![C  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d61b145b-43a9-45a3-a889-96217018559c/d61b145b-43a9-45a3-a889-96217018559c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=21d166210ae81df332b82ee40eafdf0b4606edcd)
Fig. 8 Pattern matching method applied on the corner of a 40nm IC sample. (a)  T0 image for pattern recognition template; (b) After 90s polishing; (c) After  390s polishing; (d) After 510s polishing.

From the images in Fig. 8, we can tell that after 90s polishing,  the morphology is almost the same as T0 in Fig. 8(b), however,  there is a pink colored region appeared in Fig. 8(c) and the  barrier of the M7 is still visible at the bottom right corner. After  510s polishing, the barrier layer at the bottom right corner is  gone and the sample is supposed to have M7 removed at this  region, as shown in Fig. 8(d). We took a picture of the same  region every 90s during polishing and used our own-developed  application to match the template pattern of Fig. 8(a). The  results show that from 510s onward, the template pattern cannot  be matched (detected). Therefore, images before 510s can be  labeled as M7 and images after 510s can be categorized as M6.

The pattern matching method is not efficient when the BEOL  layers getting thinner and more layers overlapped in the optical  images. If the template for recognition is not a well-defined  feature but a few patterns overlapped, it is highly possible that  the algorithm will miss the target. In our current study, the top  layer or top three layers on IC chips have suitable layer  thickness and a nice template can be obtained. With careful  adjustments of the algorithm settings, the detectability can be  improved, but more studies are needed to make this method  applicable to images of any IC chips.

## IV. C ONCLUSION 

Reliable endpoint detection methods are important for  automatic image categorization so as to generate the training  data for machine learning and/or deep learning in a later stage.  Here we successfully demonstrated how to use grayscale line  profile analysis to detect the endpoint of BEOL film layers with

ripple patterns formed on a polished sample surface. Pattern  matching method is another important approach for those  images without ripple patterns. Both methods discussed here  seem to be very promising for future work.

## R EFERENCES 

[1]    Y. LeCun, Y. Bengio, and G. Hinton, “Deep Learning,”  Nature , vol. 521,  pp. 436-444, May 2015.    [2]    J. Schmidhuber, “Deep learning in neural networks: An overview,”  Neural Networks , vol. 61, pp. 85-117, Jan 2015.    [3]    T. Wang, D. Zhao, Y. He, and X. Lu, “Effect of slurry injection position  on material removal in chemical mechanical planarization,”  Int J. Adv.  Man Tech , vol. 67, pp. 2903-2908, Aug 2013.    [4]    Y. Jeng , and P. Huang, “A Material Removal Rate Model Considering  Interfacial Micro-Contact Wear Behavior for Chemical Mechanical  Polishing, ”  J. Electro Soc , vol. 127, pp. 190-197, Jan 2005.    [5]    http://www.ni.com/en-sg/shop/data-acquisition-and-control/add-ons-fordata-acquisition-and-control/what-is-vision-development-module.html

