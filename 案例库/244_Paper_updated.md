---
title: "244_Paper_updated.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_f7a57e07a92423d4e78f323cf93af8a07295230462135641
file_size: 1391949
---

## Second Harmonic Laser Voltage Imaging on  FinFET Devices  

Kai Hui  $\mathrm{Ng^{l}}$  , Yi Xuan Seah 1 , Gopinath Ranganathan 1  1 Device Analysis, AMD Singapore  Email : kaihui.ng@amd.com

Abstract— Second harmonic Laser Voltage Imaging (LVI) is  a laser-based fault isolation technique that maps the duty cycle  degradation of the targeted circuitry. This paper presents  successful case studies that captures anomalies in scan chain  using second harmonic LVI on sub-10nm FinFET devices.

Keywords— duty cycle, harmonics, Laser Voltage Imaging  (LVI), Laser Voltage Probing (LVP)

## I.    I NTRODUCTION 

Laser Voltage Imaging (LVI) is a commonly used fault  isolation technique to detect abnormal transitions in scan  chains by mapping the changes in the active transistors at a  target frequency. The fundamental principle of LVI is based  on the electro-optic modulation of the reflected laser triggered  by the changes in the electrical field and free carrier density of  the affected transistors [1].

A harmonic is a sinusoidal signal with a frequency that is  an integer multiple of the fundamental frequency (f). At  $50\%$    duty cycle (Fig. 1), no even harmonics should exist (Fig. 2)  [2].

![Pulse Width, Ton  Duty Cycle  Input  g×100%  Signal  5096  Period, T  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/868a7df2-3169-4500-a31c-609bd07b0073/868a7df2-3169-4500-a31c-609bd07b0073.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=fb0580a922b9ed7eb3d3f81119c07fdf970532ae)
Fig.   $1.\,50\%$   Duty Cycle in Time Domain.

$$a_{0}={\frac{1}{\pi}}{\int_{0}}^{2\pi}f(x)\,d x$$݀ݔ
1

ଶగ

(2)

ܽ

=

න

݂(ݔ) cos(݊ݔ)

݀ݔ

(3)

ߨ

ଶగ ܾ

=  1

න

݂(ݔ) sin(݊ݔ)

݀ݔ

(4)

ߨ

When n is an odd number,   $b_{n}$   determines the amplitude of the  function   $f(x)$     while   $a_{n}$   remains as zero.  $f(x)$    decreases by  1/n as the odd-numbered values of n increases. When n is an  even number, both   $a_{n}$   and   $b_{n}$   are zero, hence no even  harmonics is present at a   $50\%$   duty cycle [3].

If a physical anomaly is present in the device, the signal  propagating through the scan chain path will be flawed. The  duty cycle of the degraded output signal will no longer be at   $50\%$   (Fig. 3), therefore even harmonics will exist (Fig. 4). The  activity of the defective transistor(s) in the scan chain path will  be mapped through LVI at second harmonic frequency (2f).

![Pulse Width, Ton  Input  Degraded  Signal  Duty Cycle  Period, T  ×100%  Degraded  259/6  Output   0001000100010001  Signal  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cb7e37d0-a40e-467e-a452-92f89873936c/cb7e37d0-a40e-467e-a452-92f89873936c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=929ef80c2495903ebb2a693dada131bc6c5e112f)
Fig. 3. Non-  $50\%$   Duty Cycle in Time Domain .

![31  Frequency  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0feaf953-9919-48af-8f68-2e0d30780192/0feaf953-9919-48af-8f68-2e0d30780192.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=f2c2dccd2c4e4f2ccf268a0919e482f772244517)
Fig. 2.  $50\%$   Duty Cycle in Frequency Domain.

This can be further explained using the following Fourier  series function (Eq. 1).

$$f(x)={\frac{a_{0}}{2}}+\sum_{n=1}^{\infty}a_{n}\cos(n x)+\sum_{n=1}^{\infty}b_{n}\sin(n x)$$
(1)

The Fourier coefficients,   $a_{0}(\operatorname{Eq.}2)$  ,  $a_{n}$   (Eq. 3) and  $b_{n}$   (Eq. 4)  of the function  $f(x)$    are defined as the following, where n is  the  ${\mathfrak{n}}^{\mathrm{th}}$   harmonic.

![f2f3f4f5f6f7f  Frequency  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2584d29e-3c14-45d9-a753-ee936c613d83/2584d29e-3c14-45d9-a753-ee936c613d83.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=c896c3f0b1c71e4751bfe0dc1ea81ff0e37f1184)
Fig. 4. Non-  $.50\%$   Duty Cycle in Frequency Domain.

In this paper, we analyse the behaviors of fin field-effect  transistor (FinFET) samples through second harmonic LVI at   $50\%$   duty cycle.

## II.   E XPERIMENTAL  S ETUP 

Prior to conducting a LVI analysis, other widely used fault  isolation techniques such as Photon Emission Microscopy  (PEM) (Fig. 5) and Soft Defect Localization (SDL) (Fig. 6)

were performed to further reduce our region of interest to  work on and identify the affected scan chain path.

![PEM at 50X   PEM at SIL Zoom1  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/374fd1c3-d77c-46e3-8373-3e22fef3c1da/374fd1c3-d77c-46e3-8373-3e22fef3c1da.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=4a17b97b9891a13f3111b1f3288cd242f7610fa5)
Fig. 5. Reduced Region of Interest using PEM.

![SDLat50X   SDL at SIL Zoom8  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b4d4db24-164a-4d26-b204-2bc723a312c7/b4d4db24-164a-4d26-b204-2bc723a312c7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=0975bc87b647f9e6cad09ad7f7b088c2aa1ca080)
Fig. 6. Reduced Region of Interest using SDL.

Fault isolation at a higher magnification and resolution can  be achieved by using a higher Numerical Aperture (NA) lens  and a laser-based tool equipped with a shorter laser  wavelength [4]. This theory can be determined using the  following equation (Eq.5).

$$R\,=\,\frac{0.61\lambda}{N A}$$
(5)

where   R is the resolution   $\uplambda$   is the wavelength  NA is the Numerical Aperture

The silicon surface of the die is commonly milled down to   $50{\pm}5\,\upmu\mathrm{m}$   when using a   $1064\mathrm{nm}$   laser-based fault isolation tool  coupled with a Solid Immersion Lens (SIL) to obtain optimal  spatial resolution [5].

To conduct a typical scan chain LVI analysis, an automatic  test equipment (ATE) is used to deliver sequential logic  periodically into the scan cells in an infinite loop and a fault  isolation tool equipped with   $1064\mathrm{nm}$   laser to map the activity  of the transistors at the specific frequency. The setup and flow  of an LVI analysis is illustrated in Fig. 7.

![1. An ATE sends  2. The laser from the  sequential logic  fault isolation tool is  periodically into  the scan cells of   reflected onto the silicon  the device in an   surface which changes  Device  infinite loop.   the electrical field and  free carrier density of  Vector#   Instruction   Scan-in Pin   the affected transistors.  -LOOP  0011  23   00  0011    paddnbg  LOOPEND   [ 1t901  LOST  ATE Test Patterns   3. The fault isolation tool  maps the activity of the  transistors at a specific  frequency.  Laser Voltage Imaging (LVI)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6298b3e8-a5c2-407f-93fe-a7bb330188e7/6298b3e8-a5c2-407f-93fe-a7bb330188e7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=f62e13c7306804a5ce3cab6700689472fa5c4be9)
Fig. 7. ATE + Fault Isolation Setup for LVI Analysis.

With the defined input sequential logic in the scan test  patterns and correct test parameters, second harmonic LVI  data can be obtained by simply switching the target frequency  to scan on the spectrum analyzer of the fault isolation tool.

## III.   R ESULTS  &   D ISCUSSION 

## Case Study 1:  

A typical first harmonic LVI analysis would show an  absence of LVI sites at the targeted and subsequent  downstream scan flop if a physical defect is present. The  absence of LVI sites indicates the start of a faulty transition at  the targeted scan flop that propagates to the downstream scan  flops.

Fig. 8 and Fig. 9 shows an example of a first harmonic LVI  obtained at the fundamental frequency (f) at passing and  failing conditions. The scan flops that are upstream and  downstream of the targeted flop are illustrated in green and  red respectively. The LVI sites around the targeted scan flop  at both conditions were observed to be indistinguishable from  one another.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f03916ba-0fe5-4a86-adcf-619f73be4cc4/f03916ba-0fe5-4a86-adcf-619f73be4cc4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=b79277ae4598ac0305db202d26f1f344d9c4faa8)
Fig. 8. First Harmonic LVI at Passing Condition.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9f39e56a-b9cc-4afd-a999-8ebb3bd7dbef/9f39e56a-b9cc-4afd-a999-8ebb3bd7dbef.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=8607f2b02424342b3499fae389c2b55c6c3b0dc2)
Fig. 9. First Harmonic LVI at Failing Condition.

Unlike first harmonic LVI analysis, second harmonic LVI  analysis would not show any LVI sites at   $50\%$   duty cycle. The  presence of any additional LVI sites indicates the start of a  corrupted signal propagation from the targeted scan flop.

Fig. 10 and Fig. 11 compares the second harmonic LVI  obtained at second harmonic frequency (2f) at passing and  failing conditions. The additional bright spots observed at the  failing test condition was induced by an even harmonic signal  at   $50\%$   duty cycle, therefore suggests that a defect is present  and signal corruption starts from this scan flop illustrated in  blue.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/81e76fa9-ac1a-4bff-ad1c-a261aeb5313b/81e76fa9-ac1a-4bff-ad1c-a261aeb5313b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=df6a1450310b50cff4584fe5b6a997e7d962355e)
Fig. 10. Second Harmonic LVI at the Same Passing Condition.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ddb0edd7-49df-4e0c-8d6f-5a28b05d5c0e/ddb0edd7-49df-4e0c-8d6f-5a28b05d5c0e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=56a00be0f393517c383f2b19d99a6033515ca448)
Fig. 11. Second Harmonic LVI at the Same Failing Condition.

## Case Study 2:  

Fig. 12 and Fig. 13 shows another example of a first  harmonic LVI obtained at the fundamental frequency (f) at  passing and failing conditions. The scan flops that are  upstream and downstream of the targeted flop are illustrated  in green and red respectively. Likewise for this case study,  LVI sites around the targeted scan flop at both conditions were  observed to be indistinguishable from one another.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6856195b-cc6a-4d9b-89ab-44f3de4c48bc/6856195b-cc6a-4d9b-89ab-44f3de4c48bc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=df1f64fbc370ca0e1bf59a77b1a5916ecf52ad1c)
Fig. 12. First Harmonic LVI at Passing Condition.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/030260df-cb64-421f-9e15-fd91674066b4/030260df-cb64-421f-9e15-fd91674066b4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=23e1e08539071c48f6f93e1d38b253c5a829d750)
Fig. 13. First Harmonic LVI at Failing Condition.

Fig. 14 and Fig. 15 compares the second harmonic LVI  obtained at second harmonic frequency (2f) at passing and  failing conditions. Additional bright spots were observed at  the failing test condition which suggests that a defect is present  and signal corruption starts from the scan flop illustrated in  blue.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a90cf4df-c1dc-4f4a-924b-3234366d9c70/a90cf4df-c1dc-4f4a-924b-3234366d9c70.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=961c8623c364bc1b6563bf8c5304a844827af617)
Fig. 14. Second Harmonic LVI at Passing Condition.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b668cc86-5d57-4524-a68c-11e7fc8a8162/b668cc86-5d57-4524-a68c-11e7fc8a8162.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=30417d5ffff0bbe7763e077723437b51cfd51c1d)
Fig. 15. Second Harmonic LVI at Failing Condition.

Laser Voltage Probing (LVP), a laser-based voltage and  timing failure analysis technique that shares the same  fundamental principle as LVI, is commonly used to  demonstrate the hypothesis observed in the second harmonic  LVI analysis. In this case study, two vectors of the input  sequential logic in the scan test patterns were amended.  Despite the slight deviation from a   $50\%$   duty cycle with the  adjust vectors, this creates a less repetitive waveform to  identify the start of the abnormal transitions of the output  sequential logic in each flop.

Fig. 16 shows the logic transition of the targeted scan flop  and its input logic from the upstream flop with respect to the  clock net. The transitions of the targeted scan flop were  observed to be delayed by three clock cycles compared to the  flop upstream of the targeted flop.

![Ck  Upstream  ScanFlop  Targeted  Scan Flop  (Passing  Condition)  Targeted  ScanFlop  (Failing  Condition)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/77203f2a-25b3-4704-9cd6-6696c5c254f7/77203f2a-25b3-4704-9cd6-6696c5c254f7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215769%3B1743219369&q-key-time=1743215769%3B1743219369&q-header-list=host&q-url-param-list=&q-signature=955f8acc31b31220f4cbca3bcf833ea349ae9aa6)
Fig. 16. LVP at Passing & Failing Conditions.

At a passing condition, LVP at the targeted scan flop  exhibits correct toggling of the output logic, whereas under a  failing condition, LVP at the targeted scan flop shows  incorrect toggling of the output logic. This implies that signal  corruption originates from the targeted scan flop as the output  logic fails to toggle at the correct clock cycle. Thus, this  collection of LVP results corroborates the observations made  from the second harmonic LVI analysis.

## IV.   C ONCLUSIONS 

The paper shows the benefits of fault isolation on FinFET  devices by using second harmonic LVI when a typical first  harmonic LVI configuration is not successful. This technique  provides a higher level of confidence to pursue physical  failure analysis at the scan cell of interest for scan chain  failures.

## A CKNOWLEDGMENT 

The authors would like to thank AMD Singapore for  supporting this work.

## R EFERENCES 

[1]    W. Lua, V. K. Ravikumar and A. Phoa, "Low Frequency Detector for  Enhanced Laser Voltage Probing and Imaging Applications at Slow  Speeds", 2018 IEEE International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA), 2018, pp. 1-7.    [2]    G. Celi, S. Dudit, T. Parrassin, M. Vallet, P. Perdu, A. Reverdy and D.  Lewis, “Laser Voltage Imaging: New Perspective Using Second  Harmonic Detection on Submicron Technology”, 38th International  Symposium for Testing and Failure Analysis (ISTFA), 2012, pp. 176- 182.    [3]    S. Y. Liu, K. Yuan Chao, H. H. Chou and W. Sheng Wu, "The  Application of 2nd Harmonic Laser Voltage Imaging for Timing  Failure,   Re-Thinning   Techniques   for   Effective   Dislocation  Identification", 2022 IEEE International Symposium on the Physical  and Failure Analysis of Integrated Circuits (IPFA), 2022, pp. 1-5.    [4]    G. Ranganathan, V. K. Ravikumar, A. Phoa and C. W. Teo, "Timing  analysis case studies using 1064 nm Continuous Wave laser for Fault  Isolation on scan failures", 2015 IEEE International Symposium on the  Physical and Failure Analysis of Integrated Circuits (IPFA), 2015, pp.  13-16.    [5]    J. Beutler, V. C. Hodges, J. J. Clement, J. Stevens, E. I. Cole Jr., S.  Silverman and R. Chivas, “Visible Light LVP on Bulk Silicon  Devices”, 41st International Symposium for Testing and Failure  Analysis (ISTFA), 2015.

