---
title: "111_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_c9aaf52be55691d11a2609d8bd2dd01a7295230462135641
file_size: 3279117
---

## High resolution CT cross section observation using  Vertical Oblique CT method  

Naoki Seimiya 1 , Naohiro Wakabayashi 2  , Shoji Adachi 3 , Atsushi Tamura  4  ,   Shuhei Takizawa 5 , Yusuke   $\mathrm{Oka^{6}}$  ,   1,2,3,4,5,6 U.H.System corporation, 505-1, Shimotsuruma, Yamato-city, Kanagawa pref, Japan  Phone : (+81)-46-272-0111, Email : n.seimiya@uhsystem.co.jp

Abstract — With the advent of three-dimensional stacking in  semiconductor packages, the role of X-ray CT in nondestructive failure analysis has become increasingly critical.  Additionally, as the internal structures of packages, such as  bumps and VIAs, become finer, the demand for higher  resolution in X-ray CT continues to grow. However,  conventional X-ray CT systems require the sample to be rotated  perpendicularly to the X-ray optical axis. This necessitates  maintaining a certain distance between the sample and the Xray source, which precludes high magnification imaging. To  address this issue, Oblique CT technology was developed in the  early 2000s and has since become prevalent in the  semiconductor industry. Oblique CT allows for significantly  higher CT imaging magnification compared to conventional CT,  enabling CT scans with submicron resolution even for large  packages. However, Oblique CT has the disadvantage of not  being able to obtain accurate vertical slice images. In our efforts  to   overcome   this   limitation   as   an   X-ray   equipment  manufacturer, we have devised a new imaging technique called  Vertical Oblique CT. In this paper, we will first clarify the  differences between conventional CT and Oblique CT, and then  introduce the new imaging technique called Vertical Oblique  CT.

Keywords— horizontal slice image, vertical slice image,  conventional CT, Normal Oblique CT, Vertical Oblique CT

## I.    INTRODUCTION  

In the failure analysis of three-dimensional semiconductor  packages, which have advanced with chip stacking  technology, non-destructive observation using X-ray CT has  become essential. Additionally, recent semiconductor  packages tend to increase in size due to the advancement of  miniaturization and the introduction of chip-let technology.  For such samples, conventional CT systems, which rotate the  sample between the X-ray tube and detector, face challenges  in achieving sufficient resolution due to the inability to  increase imaging magnification. This is where Oblique CT  has garnered attention in recent years. Oblique CT, developed  by U.H. System in 2002, has evolved dramatically over the  past 20 years and is now capable of capturing CT images at  the nanometer scale even for large packages.

## II.   M AGNIFICATION AND  R ESOLUTION OF  C ONVENTIONAL  CT  AND  O BLIQUE  CT  

The magnification of X-rays can be determined by the  formula FDD/FOD. FDD stands for Focus Detector  Distance, and FOD stands for Focus Object Distance. In  other words, to increase magnification, the FOD needs to be  shortened. Fig. 1 shows an example of FDD and FOD when  CT imaging a bump inside a semiconductor package  approximately 25mm in size using a conventional CT.  When the observation area is the bump indicated in red, the

geometric magnification is   $500/25=20\mathrm{x}$  . Since it is  necessary to rotate the sample   $360^{\circ}$   relative to the X-ray  optical axis, the rotation center must be kept away from the  X-ray source by the radius of rotation, making it impossible  to shorten the FOD. Therefore, the magnification cannot be  increased. This means that as the package size increases, the  limitation on magnification becomes more significant.  While increasing the FDD is another method to increase  magnification, the X-ray tubes typically used for highresolution imaging focus the X-ray beam down to the  nanometer level. When the FDD is increased, there is a  problem of insufficient X-ray power. Hence, in this  example, the FDD is fixed at   $500\mathrm{mm}$  .

![x-ray  Tube  FOD  25mm  FDD  500mm  X-ray detector  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/83ddc39b-f8ee-44ba-ad9a-a9886707680a/83ddc39b-f8ee-44ba-ad9a-a9886707680a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=f21411b487e2bef73c97d03d5aff6f3590ace766)
Fig. 1.   Example of FDD and FOD in conventional CT

Fig. 2 shows the relationship between FDD and FOD  when imaging the same sample using Oblique CT. If the FDD  remains the same at 500mm and the FOD is reduced to 2mm,  the magnification becomes   $500/2=250\mathrm{x}$  . In Oblique CT, the  detector is tilted, and the sample is rotated 360 degrees  horizontally. Since many semiconductor packages are thin and  flat, as in this example, it is often possible to achieve high  magnification.

![x-ray  Tube  FDD500mm  FOD2mm  X-raydetector  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b08ea350-359c-464f-88ee-a759572c27ce/b08ea350-359c-464f-88ee-a759572c27ce.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=f891b8eddf60298ab1a58c9d17177dda034a4258)
Fig. 2.  Example of FDD and FOD in Oblique CT

Next, Table I shows the relationship between FDD, FOD,  magnification, and pixel size. Many failure analysis  engineers desire CT imaging with a pixel size of less than   $1\upmu\mathrm{m}$  , but it is clear that achieving a pixel size of less than

$1\upmu\mathrm{m}$   requires an FOD of 5mm or less. In the case of the  package shown in Fig. 1, conventional CT cannot shorten the  FOD to less than 25mm, thus only achieving a pixel size of  up to  $5\upmu\mathrm{m}$  . In contrast, if Oblique CT can shorten the FOD to  2mm, a size of   $0.4\upmu\mathrm{m}/$  /pixel can be achieved.

TABLE I.     R ELATIONSHIP BETWEEN  FDD,   FOD,  MAGNIFICATION , AND PIXEL SIZE .

|500|500|1|100.00|
|---|---|---|---|
|500|50|10|10.00|
|500|25|20|5.00|
|500|10|50|2.00|
|500|5|100|1.00|
|500|2|250|0.40|
|500|1.7|300|0.33|


The pixel pitch (pixel size at 1x magnification) typically  ranges from about   $50\upmu\mathrm{m}$   to   $200\upmu\mathrm{m}$  , depending on the  specifications of the chosen FPD (Flat Panel Detector). For  ease of calculation, the pixel pitch is assumed to be   $100\upmu\mathrm{m}$    here.

III.

##   E XAMPLES OF  I MAGING WITH  N ORMAL  O BLIQUE  

CT

You may now understand why Oblique CT is effective for  high magnification imaging of semiconductor packages. Here  are some examples of such imaging. Following this, we will  introduce Vertical Oblique CT. To distinguish between  Vertical Oblique CT and regular Oblique CT, we will refer to  the regular Oblique CT as "Normal Oblique CT." All the CT  imaging examples introduced in this paper were captured  using the U.H.System XVA-160αⅡ.

Fig. 3 is a horizontal slice image captured with Normal  Oblique CT of an area where electromigration is occurring  between lead frames. Although the magnification is not very  high at 50x, the package size is large, making it an image that  cannot be captured with conventional CT.

Fig. 3 shows a horizontal slice image captured with  Normal Oblique CT, where electromigration has occurred  between lead frames. Although the magnification is not very  high at 50x, this is an image that cannot be captured with  conventional CT due to the large package size.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6a5dae49-bdfd-4bce-a91c-3405c3ad4938/6a5dae49-bdfd-4bce-a91c-3405c3ad4938.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=f6bf394f349985797fa4a26b503b9fbc35bfa4bc)
Fig. 3.  Horizontal slice image of electromigration captured with Normal  Oblique CT

Fig. 4 is a schematic diagram of a build-up substrate  embedded in an FCBGA package. With the results of TDR  analysis (Time Domain Reflectometry) indicating a  suspected open fault near the V23_Via, Normal Oblique CT  analysis was performed. The package is approximately   $30\,\times$  30mm in size .

![3D  V23Via  2  OuterBGA  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bb892bfe-cba2-4d05-ab23-719aec6ae663/bb892bfe-cba2-4d05-ab23-719aec6ae663.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=37431457d23b720d496820cbf82943cb6b3f0459)
Fig. 4.   Schematic diagram of the build-up substrate

Fig. 5 shows the results of a 150x Normal Oblique CT  scan with the V23_Via centered on the screen. The scan  revealed not only the deformation of the V23_Via but also  the erosion of the adjacent substrate's plating. If destructive  physical cross-sectioning had been performed immediately  without non-destructive X-ray CT observation, the crosssection might have been cut at the location indicated by the  red line. In that case, the substrate's plating erosion visible to  the right of the V23_Via would have been missed. Without  the information about this plating erosion, the direction of  the corrective measures to prevent recurrence could have  been misguided. This case highlighted the crucial importance  of non-destructive defect analysis.

![V23_Via  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e44e3698-dd55-4bd0-8f10-c788bbd3cc27/e44e3698-dd55-4bd0-8f10-c788bbd3cc27.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=00815fcb5382c99ef442f3e11b433f1bdbd8cfe1)
Fig. 5.   Horizontal slice image by 150x Normal Oblique CT

IV.   A DVANTAGES AND  D ISADVANTAGES OF  N ORMAL  O BLIQUE  CT

To further deepen understanding of Oblique CT, let me  introduce experimental results using a TEM grid. Fig. 6  shows an image of a laminated sample containing a Cu  TEM grid observed through 2D X-ray. You can see the  formation of fine mesh structures.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/59292e72-d0c8-47e0-9d95-33a08bec7059/59292e72-d0c8-47e0-9d95-33a08bec7059.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=b3d2a6984a1e3e0b57a386c62bcded8810f66d38)
Fig. 6.   Laminated TEM grid

Fig. 7 shows the sample setup for Normal Oblique CT  imaging of the TEM grid. Since the sample is simply placed  on the table, the setup is extremely simple. In practice, the  sample is fixed with tape to prevent it from moving during  CT imaging.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fb50564c-e649-48ed-a63a-9a8ea4f379bf/fb50564c-e649-48ed-a63a-9a8ea4f379bf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=65f4402f2e703f395f231f8560eb807e4ac48409)
Fig. 7. Sample setup for Normal Oblique CT

Fig. 8 shows a horizontal slice image captured with Normal  Oblique CT at  $300\mathbf{x}$   magnification. The scan time is  approximately 3 minutes, but you can see that the image  resolution is sufficient to measure the width of each Cu bar.  This ease of capturing high-magnification CT images is also  one of the greatest advantages of Normal Oblique CT.

![Voltage100kvCur  0.42um/Pixel  45.77[um]  20.53[um]  60.22[um]  34.74[um]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d5c67707-1fef-46a3-8172-6a17f9e51f6b/d5c67707-1fef-46a3-8172-6a17f9e51f6b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=eb8958ca23548073d23e9c35b21c039d4d5e9b10)
Fig. 8.   Horizontal slice image by 300x Normal Oblique CT

This data was captured at   $300\mathrm{x}$   magnification with a  resolution of   $0.42\upmu\mathrm{m}$   per pixel. Although the pixel  resolution differs slightly from the   $300\mathbf{x}$   resolution shown in  Table I, please understand that this discrepancy is due to the  pixel pitch of the FPD used in the equipment, which was not   $100\upmu\mathrm{m}$  . Fig. 9 shows the relationship between magnification  and pixel resolution for this Normal Oblique CT imaging.

![ocus  1.28mm  FDD600mr  FOD2mm  Magnification=600/2=300x  Pixel pich:127μm/300x= 0.42um/pixel  X-raydetector  Tilt angle of 50 degrees  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f32f53d8-af9a-414b-9da2-0a57d4fe5433/f32f53d8-af9a-414b-9da2-0a57d4fe5433.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=801c4e9b60327cd3775d64c99d6281ee083e2b25)
Fig. 9. Magnification and pixel resolution of TEM grid imaging by Normal  Oblique CT

The vertical distance from the center of the TEM grid,  including the thickness of the laminate and the thickness of  the X-ray target, is   $1.28\mathrm{mm}$  . With the detector's tilt angle at  50 degrees, the FOD is 2mm, and the FDD was set to   $600\mathrm{mm}$  , resulting in a magnification of  $600/2=300\mathrm{x}$  .

You may notice that the XVA-160α II has the X-ray tube  located above the sample table and the detector located  below the sample table. Typically, the heavy X-ray tube  should be placed below the table, but if the X-ray tube is  below, the carbon plate of the table would be between the  sample and the X-ray tube. This would prevent the FOD  from being shortened by the thickness of the carbon plate.  The thickness of the carbon plate is generally around 1mm  to   $1.5\mathrm{mm}$  . By looking at Table I, you can understand how  much the 1mm difference in FOD affects the magnification  and resolution.

Next, let's look at the vertical slice image. Fig. 10 shows  the vertical slice image obtained from the same scan.

![59.69[um  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8f03d68a-460a-4c64-8935-200907664d95/8f03d68a-460a-4c64-8935-200907664d95.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=7cfad06c7a59316f094e194015be0db99a67818a)
Fig. 10. Vertical slice image of the TEM grid by Normal Oblique CT

The width of the bar indicated by the red circle is not  significantly different from the measurement in the  horizontal slice image. However, due to the detector's angle,  metal artifacts have appeared, causing the Cu bar to look  different from its actual shape. Unfortunately, it is not  possible to measure the thickness of the bar from this image.  This is the critical drawback of Normal Oblique CT  mentioned at the beginning.

## V.   P ROBLEM  S OLVING WITH  V ERTICAL  O BLIQUE  CT  

We have found that while horizontal slice images obtained  by Normal Oblique CT are very accurate, vertical slice  images are inaccurate. However, to measure the thickness of  the TEM grid bars accurately, precise vertical slice images

are necessary. Therefore, we decided to change our  approach and stand the sample upright on the table for  imaging.

In Vertical Oblique CT, as shown in Fig.11, we cut off the  unnecessary parts of the laminated pack to shorten the FOD.  We understand the importance of maintaining nondestructive analysis in CT imaging, but please consider this  approach as a means to achieve high resolution with  Vertical Oblique CT.

![opper   UHSS  eco grids  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cf7d6aca-6fa2-4648-90e6-4e6e7873148b/cf7d6aca-6fa2-4648-90e6-4e6e7873148b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=ef05b6048a86ef4d87f73963d2841bff17f2345a)
Fig. 11. TEM grid sample with unnecessary laminated parts cut off for  high-magnification Vertical Oblique CT

Fig. 12 shows the sample setup for Vertical Oblique CT  imaging. A plastic clip was used to secure the sample. In  practice, the sample was taped to prevent movement during  imaging.  The XVA-160αⅡ is capable of accommodating  samples with a height of up to 124.7 mm.

![#1020meshcopper  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6f052270-536c-40dd-9f78-86ef80e1ed31/6f052270-536c-40dd-9f78-86ef80e1ed31.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=1cdb7ca45232e6e4ca14c2810f08c53010afb469)
Fig. 12. Sample setup for Vertical Oblique CT

Fig. 13 shows the results of a 90x Vertical Oblique CT scan.  Although the magnification is lower compared to Normal  Oblique CT, it was possible to obtain an accurate horizontal  slice image and measure the thickness of the bar.

![Voltage100kV Current73uA  1.40um/Pix  17.02[um]   58.04[um]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/472dc1e2-f4e1-4382-a4b5-7a1d93094d14/472dc1e2-f4e1-4382-a4b5-7a1d93094d14.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=f2902faaa6cfb60a5120d275bb36d815327b62cb)
Fig. 13. Horizontal slice image by 90x Vertical Oblique CT

Fig. 14 shows the same data with further digital zoom. The  detailed shape of the Cu bar becomes clear, and the  approximately  $3\upmu\mathrm{m}$   step at the bottom of the bar is captured.

![Voltage100kVCurrent73uA  1.40um/Pixel   50um  3.36[um]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/32ea6875-8c8a-4b9b-b893-8b6e097473dd/32ea6875-8c8a-4b9b-b893-8b6e097473dd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=3e79920fde58a949c7ec52580f9e98e05a167b90)
Fig. 15 shows the relationship between magnification and  pixel resolution for this Normal Oblique CT imaging.

![FDD600mm  FOD6.6mm  nagnification=600/6.6=90.9x  Pixelpich:127μm/90.9x=1.4μm/pixel  X-ray detector  Tilt angle of 50 degrees  GeometricmagnificationiscalculatedbyFDD/FOD  FDD(Focus Detector Distance)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5a1e8159-4019-46e6-871a-f630c19ca489/5a1e8159-4019-46e6-871a-f630c19ca489.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=cb260503eb828e9dc85b98f3f366f80e1fae312f)
Fig. 15. Horizontal slice image by 90x Vertical Oblique CT

As you can see in Fig. 11, this time we left about 3mm of  margin when cutting off the unnecessary laminated parts. If

the laminate were cut off more precisely, it would be  possible to achieve higher magnification and resolution with  Vertical Oblique CT imaging. You might be wondering if  conventional CT would be better if the sample can be cut,  and that is a valid point. However, in the case of  conventional CT, to achieve the same resolution, it would be  necessary to cut off both sides of the laminate and make it  into a strip to reduce the rotation radius. The advantage of  Vertical Oblique CT is that if the observation area is close to  the edge, there is no need to cut it at all, and even if cutting  is necessary, it is sufficient to cut only one side as in this  example.

## VI.   E XAMPLES OF  I MAGING WITH  V ERTICAL  O BLIQUE  CT 

Fig. 16 shows an example of a TSV with a diameter of  approximately   $6\upmu\mathrm{m}$   captured using 150x Vertical Oblique  CT. The relationship between the micropump and the TSV  is captured quite clearly.

![30.03[um]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/04e97d8c-53f8-4737-bbdd-10a8057afb52/04e97d8c-53f8-4737-bbdd-10a8057afb52.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=1ad9bc56871993bc76e6c6b76003ab7cb9c0a58d)
Fig. 16. Example of a TSV with a diameter of approximately   $6\upmu\mathrm{m}$   captured  using 150x Vertical Oblique CT

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/92baae3b-4762-4ca1-b79d-dc4a4cb341fa/92baae3b-4762-4ca1-b79d-dc4a4cb341fa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=2cb3c071a4aca6d9246c524599de3f3539dd62db)
Fig. 17. Horizontal slice image by 45x Vertical Oblique CT

The imaged area is shown in Fig. 18. It should be noted that  the portion below the blue line was cut off during imaging.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/64593605-0dc0-4fa0-9437-a516da8390d8/64593605-0dc0-4fa0-9437-a516da8390d8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215824%3B1743219424&q-key-time=1743215824%3B1743219424&q-header-list=host&q-url-param-list=&q-signature=ae15f7ae6b8b031114e8a78abe81260ccd887bd7)
Fig. 18. Sample captured with 45x Vertical Oblique CT

## VII.   SUMMARY 

So far, we have looked at the challenges and solutions for  the three techniques: conventional CT, Normal Oblique CT,  and Vertical Oblique CT. Table II shows the strengths and  weaknesses of each technique as we see them.

TABLE II.     S TRENGTHS AND WEAKNESSES OF THE THREE  CT TECHNIQUES

||Conventional CT||Vertical Oblique CT|Normal Oblique CT|
|---|---|---|---|---|
|Magnification|||||
|Artifact|||||
|        Horizontal slice                image      |||||
|        Verticalslice                Image      |||||


Normal Oblique CT has the advantages of high  magnification and fewer artifacts but has issues with vertical  slice images. Vertical Oblique CT solves the issues with  vertical slice images but has problems with horizontal slice  images. Conventional CT has no issues with either horizontal  or vertical slices but is difficult to increase magnification and  is prone to artifacts.

Non-destructive analysis for successful failure analysis  sometimes requires complete non-destructiveness, but partial  destruction may be permissible in some cases. For example,  CT imaging of a large substrate can only be done with Normal  Oblique CT. However, if the defective area can be identified  and unnecessary parts can be cut off to some extent, Vertical  Oblique CT becomes effective. Furthermore, if the sample can  be reduced to strip-shaped pieces, conventional CT becomes  effective. Understanding the strengths and weaknesses of each  CT technique and using them appropriately according to the  sample condition and purpose is the key to successful nondestructive failure analysis with X-ray CT. If the defective  area can be visualized with X-ray CT, the chances of  successful failure analysis increase significantly.

## ACKNOWLEDGMENT  

Vertical Oblique CT method is an imaging technique created  based on advice from many Japanese users of the 3D X-ray  CT equipment we manufacture and sell. Thank you to all our  users.

## REFERENCES  

Masaki Misawa, Tiseanu Ion, Ryusuke Hirashima, Naohiro Wakabayashi,  and Kazuto Koizumi    National Institute of Advanced Industrial Science and Technology (AIST) and  Uni-Hite system corporation    "Method for Reconstructing Inclined Three-Dimensional X-ray CT  Images"[ 傾斜三次元 X  線 CT  画像の再構成方法 ]    Japanese Unexamined Patent Application Publication No.2003-344316,  December 3, 2003

