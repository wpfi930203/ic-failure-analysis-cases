---
title: "298_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_a35afc7ce8049bc5076dec1e04aea3f67295230462135641
file_size: 4277070
---

## Enhancement of localization capability of lock-in thermography for power  semiconductor devices by searching high-emissivity films   

Norimichi Chinone, Toru Matsumoto, and Kazushige Koshikawa

System Division, Hamamatsu Photonics K. K., 812, Joko-cho, Higashi-ku, Hamamatsu City, 431-3196 Japan, Phone  +81-03-435-1560, Fax +81-03-435-0121.  \*Email:  norimcihi.chinone@sys.hpk.co.jp

## Abstract 

We will demonstrate the capability of lock-in thermography (LIT) for fault localization in a packaged power semiconductor device  by using high-emissivity film. Different types of films were investigated to explore suitable type of film for LIT. Pasting the  selected film on the heatsink of a packaged device increased the signal-to-noise ratio of LIT analysis, which enhanced the  nondestructive localization ability of LIT.

## Introduction 

Lock-in thermography (LIT) images the hot spot whose joule  heating synchronizes to external voltage modulation [1].  Because of this modulation feature, LIT improves the hot spot  detectability and has much higher spatial resolution compared  to static thermography [1]. In addition, heat conducts almost all  material, which enables non-destructive analysis. These  features makes LIT suitable technique for early stage in fault  localization of semiconductor devices. However, the result of  LIT strongly depends on sample surface emissivity [1], which  makes measurement of low emissivity sample such as power  devices covered with metal challenging. Black paint and black  film are known as countermeasure for eliminating the surface  condition dependency. Adhesive films can be suitable material  for that purpose since they are easy to paste on samples, they  are uniform, and they are easy to remove from sample.

In this study, we chose several types of adhesive films and  investigated how effective to LIT they are. In addition, we  demonstrate a case study of measuring package insulated gate  bipolar transistor (IGBT) using LIT with the most effective  film.

## Investigation of films  

## Experimental method  

We investigated three types of films with different base  material; polyester (PE), polyimide (PI), acetate (A). We  prepared an IGBT chip with artificial short fault between gate  and emitter. We measured thermal emission from the  Au-coated backside (collector electrode) with a piece of film  pasted as illustrated in Fig. 1(a). The camera used for this  measurement is Indium-Antimony (InSb) camera, which is  sensitive to infrared ray (IR) of   $3.7\ \upmu\mathrm{m}{-5.2\ \upmu\mathrm{m}}$   range. Lock-in  frequency is   $10\,\mathrm{Hz}$  . Amplitude of applied voltage is 1.5 V. The  position of field of view (FOV) is illustrated in Fig. 1(a) by box  with dashed line and its size is 9.6 mm by 7.6 mm.

Emissivity of films when they pasted on metal electrode was  measured as follows; pieces of films were pasted on the  electrode of the IGBT chip mounded on a heater. As a black  body, carbon nanotube array (CNT) grown on silicon substrate  [2] was also mounted on the heater. We measured intensity of  IR image and calculated the ratio of intensity of film surface  and CNT array surface.

## Experimental results and discussions  

Figure 1(b) shows radiated IR image. The bright color (white)  indicates low intensity IR radiation. Figure 1(c) shows the LIT  amplitude image with film whose base material is polyester.  Although we could not observe any hot spot without film (not  shown), we can see clear hot spot in the LIT image at the  position indicated by white arrow in Fig. 1(c). In other  experiment, we confirmed that we cannot see nothing without  tape.

![IR camera  FOW  IGBT chip  Fiim  Gate  Emitter  a  2mm  IGBT  chip  (b) IR image  mm  (c) LITamplitude  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0a5935b9-0e3b-4606-8ec8-8c4909cf12c2/0a5935b9-0e3b-4606-8ec8-8c4909cf12c2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=f89946a5c6fd3a4ba5133828dba1102115f3da3e)
Fig. 1 Experimental setup and typical result (a) Simplified  experimental setup (b) IR radiation image (c) Typical LIT result

We measured the intensity at the center of hot spot. Table 1  summarizes the intensity of LIT amplitude image acquired with  various films. The intensity depends on tape, which indicates  that each films has different effectiveness for LIT. The film PE  was most effective for LIT in our measurement. To see the  correlation between emissivity and LIT amplitude, we plotted  the intensity of LIT as a function of emissivity as shown in Fig.  2.

Table 1   Obtained maximum intensity of LIT amplitude image and  emissivity of the sample surface with films being pated.

|Tape #|Thickness (mm)|Emissivity|Intensity (arb. unit)|
|---|---|---|---|
|PI|0.035|0.35|5633|
|PE|0.055|0.71|10833|
|A|0.058|0.50|8033|


![10000  TapeA  1000   an   PE  100  1O  0.1   100  Frequency (Hz)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/628a2ce9-47bc-4946-9912-e932d163e327/628a2ce9-47bc-4946-9912-e932d163e327.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=712af5f2dad3960167d8a41a22e51840e6a03217)
Fig. 3 Frequency dependence of LIT amplitude with different films.

## Experimental method  

![12000  10000  Ca!un  8000  6000  4000  2000  0.1   0.２   0.3   0.4   0.5   0.6   0.8  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4752bc25-e445-4a8a-a1c4-22d08d229cc7/4752bc25-e445-4a8a-a1c4-22d08d229cc7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=9fc27a427e55715c43624c5c936b1d1ee11095ae)
Fig. 2 LIT amplitude for different types of films.

Figure 2 shows LIT amplitude is proportional to emissivity of  the sample surface with film, which means that the emissivity  strongly dominates effectiveness of film for LIT. From the  table 1 and Fig. 2, film PE is the most effective for LIT and the  film A is the second. However, another measurement also  shows that emissivity is not the only parameter which  determines the effectiveness of film for LIT. We measured  peak intensity of LIT amplitude image with various lock-in  frequency while the amplitude of the applied power is kept  constant. Figure 3 shows frequency dependence of LIT  amplitude for films A and PE. Plots of both films has  monotonically decreasing feature. This is because temperature  modulation caused by periodical heating (thermal wave) with  higher frequency propagates shorter distance. Carefully  investigating the Fig. 3, we can notice that film PE has steeper  slope compared to film A. In the frequency lower than   $10\:\mathrm{Hz}$  ,  film PE is better than film A, however, in frequency higher than   $10~\mathrm{Hz}$  , film A is better. This result suggests that the thermal  impedance of film affects the effectiveness of film for LIT.  Therefore, for selecting proper film, one should consider which  frequency range is suitable for their samples.

## Application of the film to package IGBT device  

Next, we applied the film PE for package IGBT measurement  using LIT. We measured this IGBT sample from heatsink side,  which is typically not suitable for LIT due to low emissivity.  We made a short failure in gate by applying 90 V between gate  and emitter (Rating gate-emitter voltage is 50 V). After over  voltage application, the resistance between gate and emitter  was  $20\;\Omega$  .

![RCI  9.6mm  x7.6 mm  15.4mm  Heat sink (Collector)   1.5 mm  IGBT chip  Wire   3.0 mm  Resin  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cece7412-4a58-4c61-8724-08344e240362/cece7412-4a58-4c61-8724-08344e240362.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=a839edd07ee777e636c247b5b9a1c4ce229852ac)
Fig. 4   Package sample overview (a) Photograph of the IGBT  sample. The marked rectangular area is the region of interest.  (b) Schematic cross-sectional view of the sample.

Figure 4(a) is a picture of the sample from the heatsink side.  The black area is resin and the white area is heatsink. Figure  4(b) illustrates schematic cross-sectional structure of the  sample. Si IGBT chip is mounted on cupper heatsink with the  thickness of   $1.5~\mathrm{mm}$  . The chip is molded by 3-mm-thick resin.  We measured the rectangular area boxed with dotted line in  Fig. 4(a) with LIT. The applied voltage and the lock-in  frequency were  $0.3\;\mathrm{V}$   and   $10\:\mathrm{Hz}$  , respectively. The integration  time for lock-in measurement was 600 seconds. After this  measurement, we pasted the tape PE on the sample surface,  which was revealed to be most effective for LIT in the previous  section.

In order to correlate the chip position and LIT result, we used  scanning acoustic microscope (SAT). For further confirmation  of LIT result, we partially decaped the heatsink and did  optical-beam   induced   resistance   change   (OBIRCH)  measurement.

Figure 5 shows the LIT images. Figures 5(a)-(c) (upper side in  the figure) are the result without pasting tape. On the other  hand, Figs. 5(d)-(f) (lower side of the figure) are results with  pasting tape.

In the LIT image without film, it is hard to find the hott spot.  In contrast, in the LIT images with film, we can find clear hot  spot. In the amplitude image (Fig. 5(e)), the central area has red  color, which means the amplitude of IR intensity change or  temperature change is large. Fig. 5 clearly shows that the  pasting film enhanced sensitivity of LIT. In addition, some  scars on the heatsink as indicated by arrow in Fig. 5(a) strongly  affect the LIT image without film (Figs. 5(b) and (c)) while the  scars less affect the LIT image with film. This is also benefit of  pasting film.

![Scar on the heatsink   Scar on the heatsink  w/o Tape  w/Tape  1mm  IR image   LIT amplitude image   LIT phase image  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8c641103-9e94-4df6-884e-ba01016149eb/8c641103-9e94-4df6-884e-ba01016149eb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=e2c81ba638b78222b7f81fbb4309dafdd91786c6)
Fig. 5 Comparison of LIT result without and with film. (a), (b), and (c) are IR image, LIT amplitude image, and LIT phase image without pasting  film, respectively. (d), (e), and (f) are IR image, LIT amplitude image, and LIT phase image with pasting film, respectively

We superpositioned the LIT image Fig. 5(e) on SAT image as  shown in Fig. 6. This SAT image was obtained from resin side  and was flipped for matching the orientation of SAT image to  that of LIT image. For make the superpositioned image easy to  see, the color of  pixels with low intensity were changed to  transparent after denoising. In Fig. 6, the orange colored  circular spot is the hot spot. It is clear that the hot spot is inside  the chip area, which shows the high localization capability of  LIT without decapsulation. After this measurement, we  decaped this sample and did OBIRCH measurement. Figure  7(a) shows the picture of partially decapped sample.

![Gatndin  chip  Emitter bonding  9.6.mm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9296aed2-1b7d-4720-92ba-f9fa6bb963d1/9296aed2-1b7d-4720-92ba-f9fa6bb963d1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=bce17baa6a1889e8bab66d1e4e821939f080019d)
Fig. 6 Superpositioned image of LIT and scanning acoustic  microscope.

At first, we tried OBIRCH measurement with biased condition,  however, large current noise, which might be due to unstable  current at the damaged position, prepended OBIRCH  measurement. Therefore, we tried OBIRCH measurement with  non-biased condition. Figure 7 shows the resulting OBIRCH  images. Fig. 7(b) is the laser reflection image of the decaped  sample at the position which gave hot spot in LIT image. We  can see small damaged site as indicated by white arrow. Figure  7(c) is the OBIRCH image at identical area. We can see clear  OBIRCH signal with the white and black pair, which may be  caused by Seebeck effect, at the position pointed by a white  arrow. This observation confirmed that the site which was  suggested by LIT without decapping is identical to damaged  site. This positional agreement in two method is due to merits  of measuring from heatsink side. Between chip and heatsink  surface, the thermal propagation path is simple and thermal  impedance is lower compared to resin side. Figure 8 shows the  thermal diffusion length per unit frequency of cupper and  typical resin materials calculated by following equation:

$$L_{\mathrm{th}}=(\kappa/\pi\rho c)^{1/2},$$
(1)

where  $\kappa,\rho$  , and   $c$   are thermal conductivity, density, and thermal  capacity, respectively.

![(a)  0.5 mn  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/724ac828-dc1f-4185-8bb4-9792ff715b1c/724ac828-dc1f-4185-8bb4-9792ff715b1c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=ec81ea026faf9c6e96c475afd690f565c19338ad)
Fig. 7    OBIRCH results (a) Photograph of decaped sample (b)  LSM pattern image

![C 一 Epoxy  Polyimide  CU ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/641986b7-2435-4672-a919-d2f8c778f9f5/641986b7-2435-4672-a919-d2f8c778f9f5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=ea3c8f1f7b9a09435bf9534fc4530efb43ba6e6b)
Fig. 8 Thermal diffusion length of different materials

This graph shows that thermal wave in cupper propagates over  10 times easier than resins. When the lock-in frequency is 10  Hz, the thermal diffusion length in cupper is about   $1.9\ \mathrm{mm}$  ,  which is larger than thickness of cupper heatsink (1.5 mm).  This calculation agrees the fact we could obtain clear hot spot  from the heatsink side.

In the resin side, there are wires, which may make the thermal  propagation path indirect and may become additional heat  source. Figure 8(a) and (b) show LIT image which was  acquired from heatsink side and resin side, respectively. Figure  9(a) was acquired with lock-in frequency of   $10\:\mathrm{Hz}$   as same as  Fig. 5 (sample is different one). However, 10-Hz was too high  for getting LIT image from resin side, therefore, the Fig. 9(b)  was acquired with lock-in frequency of   $0.4\,\textrm{Hz}$  . From the  heatsink side (Fig. 9(a)), single circular hot spot is observed. In  contrast, from the resin side, the LIT image has  heat area with  distorted shape. Determining hot spot in the chip from the Fig.  9(b) is difficult since these hot spot in Fig. 9(b) originate from  bonding wire inside the resin. Therefore measuring from  heatsink side is much more straightforward than measuring  from resin side. The only disadvantage of measuring heatsink  side is low emissivity, which can be overcome by pasting the  film as shown in this paper. In other words, pasting film on  sample fully enables the benefit of measuring from heatsink  side in package device, which enhance the localization  capability.

![Heatsink(Collector)  IGBTchip  ire  Resin    1 mm  10Hz  Heatsink(Collector)  IGBTchip  Wire  Resin  1 mm  0.4Hz  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a1af58ba-4fb5-4669-b546-39f1655f057d/a1af58ba-4fb5-4669-b546-39f1655f057d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=462b4dfe832c2c6a205b3fc3d2030b94a7b6aeaa)
Fig. 9 LIT images from (a) heatsink side and (b) resin side

## Conclusion 

We investigated films with different base materials and  examined their effectiveness for enhancing LIT sensitivity. It  was revealed that the different type of tape has different  effectiveness for LIT sensitivity and was strongly correlated to  emissivity. In addition, different films have different frequency  characteristics. These results suggests both of emissivity and  thermal impedance of the film are important for LIT.

We applied the high emissivity film PE, which exhibited  highest effectiveness for LIT, for measuring package IGBT  sample with LIT from heatsink side. The film enhanced the LIT  result drastically. The results showed that the LIT with high  emissivity film enhances the localization capability. Pasting  high emissivity film is convenient method for enabling  nondestructive localization of package power device.

## Acknowledgments 

This study is supported by Mr. Yasunori Goto from Toyota  Motor Corporation.

## References 

[1]    O. Breitenstein, M. Langenkanp, F. Altmann, D. Katzer, A. Lindner and  H. Eggers, “Microscopic lock-in thermography investigation of leakage  sites in integrated circuits,” Rev. Sci. Instrum., vol. 71, p. 4155 (2000).    [2]    Kohei Mizuno et al., “A black body absorber from vertically aligned  single-walled carbon nanotubes,” PNAS, vol. 106, p. 6044.

