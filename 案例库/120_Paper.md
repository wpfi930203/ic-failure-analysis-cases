---
title: "120_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_c81ef928ba599bb838f6be1113c5b0967295230462135641
file_size: 402376
---

## Enhanced Package Fault Isolation Method Using  Time Domain Reflectometry (TDR)   Incorporation  with Mathematics  

Lan Yin Lee, Kok Keng Chua

Device Analysis Engineering Lab, Xilinx Asia Pacific, 5 Changi Business Park Vista, 486040, Singapore.

Phone: +65-6407-3000 Fax: +65-6789-8886 Email:  lanyinl@xilinx.com

Abstract-  Time domain reflectometry (TDR) has gained attention  in electrical verification for electronic components over the years.  TDR works by sending a series of short pulses through a  transmission line under investigation, and measures the  reflections that result from a signal travelling through a  transmission environment. [1,2] It is often being used for short or  open failures defect localization, to isolate whether the short/ open  failure is in the die region or package region. With the  enhancement of process technology and increase of layers in the  package/ silicon die, and due to limitation of reference medium,  the results produced by using TDR can only be used as a rough  guide, i.e. based on the TDR results, we can only narrow the open/  short failure to be in the die or package, we could not tell which  layer of package the short/open is.  This paper demonstrates some  successful cases with the incorporation of mathematics together  with the use of TDR machine. Open failure can be accurately  localized down to specific substrate layer via mathematics  calculation. Physical failure analysis further confirmed the  accuracy of this method by showing the defect at that specific  layer in those cases.

Keywords  –   Time domain reflectometry (TDR), defect localization,  open/ short failure, mathematics calculation.

TDR came to the attention of geologists and other scientists  in late 1930's. There was a significant relationship between  dielectric properties of soil, rock and other materials and their  moisture content. TDR was then developed as the result of  World War II research and was used for defining these  dielectric relationships. [3] Time domain reflectometry (TDR)  has gained attention in electrical verification for electronic  components over the years. TDR works by sending a series of  short pulses through a transmission line under investigation,  and measures the reflections that result from a signal travelling  through a transmission environment. [1,2] In semiconductor  industry, TDR was often used to determine whether a short or  open failure is in the silicon die or package substrate. For  Stacked Silicon Interconnect Technology (SSIT) product, TDR  was also used for short/ open failure localization, whether  failure is in the C4 bump, micro bump, interposer, silicon die or  package substrate. It will be more useful if more reference  points such as golden samples with simulated open in C4 bump  or simulated open in micro bump are used in comparison. As  shown in Figure 1. However, due to limitation of the fabrication  of these reference units, no further fault isolation can be done  simply based on this TDR curve. For the open failure showing

in the substrate, we have no way to know which layer of the  substrate this open failure is located. Layer by layer polishing  and isolation needed to be carried out to find the open failure,  which is time consuming and not   $100\%$   hit rate guaranteed as  we need to choose between cross-sectioning method to check  the substrate copper vias or parallel lapping to check the  substrate trace. With the incorporation of mathematics together  with the use of TDR machine, open failure can be accurately  localized at specific substrate layer. This paper demonstrates  some successful cases with the incorporation of mathematics  together with the use of TDR machine. Physical failure analysis  further carried out to confirm the accuracy of this method by  showing the defect at that TDR isolated failing layer in those  cases.

![5oo.omV  Ref Open  Substrate w/o die  F4 pinAR8  GoodUnil AinAAH  0.003469   50.00ps/div  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/40c64ecb-c3ed-46ce-a54b-632dc545bb62/40c64ecb-c3ed-46ce-a54b-632dc545bb62.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=76e2f5d6b8dd519d7c9a96bba10173ed7adec181)
Fig. 1 Example of TDR curve with reference point (simulate open in C4 bump)

## II. INCORPORATION OF TDR AND MATHEMATICS  

An open failure was reported in a 4cm x 4cm package device.  This type of device was made up of 10 substrate layers. Curve  trace confirmed that this is a valid open failure. (Refer to Figure  2.) As no emission hotspot can be performed for open failure,  only TDR can be used. By performing typical TDR analysis,  we know that this open failure is in the substrate. However, we  do not know which layer of substrate this open failure is  located. (Fig. 3)

![S/N1  RET  SDOU  400U  300u  2D0U  1D0U  F1D0u  -200  -300U  -4D0U  SDOU  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a3023ece-e067-4907-ad47-c3742383f047/a3023ece-e067-4907-ad47-c3742383f047.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=351c3bc100fb65e72fd0e01932387858dc711dc9)
Fig. 2 Valid open failure was reported

![SNRF1 U30  RefOpen   Substrate wfo die U30  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fb771594-f56d-4dbe-aa90-eb8871f230a2/fb771594-f56d-4dbe-aa90-eb8871f230a2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=9bb9025ebf0eb29ddcf0abd57bc0890257293d7b)
Fig. 3 TDR showed open failure in substrate

By collecting this specific package type substrate layer  information (the copper vias height as well as the substrate  traces length in each layer) for the reported failing pin, we can  calculate and isolate the open failure accurately by rationing the  scale in Fig. 3. In the case study above, the failing pin’s total  substrate metal traces and copper vias height was added up to  be 9000um. Next, from the TDR results, it was found that the  distance between “Ref open” (blue line, open at solder ball) to  the open failure (red line) is 3.5 scales (distance A in Fig. 3);  while the full package distance from solder ball (blue line) to  silicon die surface (yellow line) is calculated to be 7 scales  (distance B in Fig. 3). By using mathematics ratio failing  location can be calculated as below:

Full package distance of the failing pin (9000um):  $\mathbf{B}=$  open  failure distance (from solder ball) : A

For this case, the open failure distance was finally calculated  to be at the distance of 4500um from solder ball; which is  located at substrate metal 1, which is nearest to silicon die.

## III. DESTRUCTIVE FAILURE ANALYSIS  

Following the TDR calculation results, destructive failure  analysis was performed to delayer from silicon die as the  defect location is nearer to this site. Optical inspection  confirmed substrate metal 1 trace open. (Fig.4)

![Cu trace open  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/be5b675d-1d08-4dd9-8701-02b58ebe472d/be5b675d-1d08-4dd9-8701-02b58ebe472d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=9fd23d3112dabc2ad45635d4ae5253871e9944fe)
Fig. 4 Substrate metal 1 trace was confirmed open

## IV. CASE STUDY 2  

Here is another example which uses this method to  successfully isolate the failure.  Another open failure was  reported in a  $4.5\mathrm{cm}\,\mathrm{x}\,4.5\mathrm{cm}$   package. This type of package is  having a total of 14 substrate layers. Again, after curve trace  confirmation of this valid open and TDR showing it is open in  the substrate, refer to Fig. 5. However, for this case we do not  have a simulated open on silicon die surface as reference. We  will take the peak of the good unit as the reference point  (indicated by black arrow in Fig. 5).

![RefOpen  BadH39   Si die interface  Si die interface  Ge0d H39  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2b690a0a-eb51-4c65-b4ce-972d3866bca7/2b690a0a-eb51-4c65-b4ce-972d3866bca7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=bb03c3899d73fd42417691b35b60033a8aaf6c96)
Fig. 5 TDR showed open failure in substrate for case study 2

For this case, due to 14 layers stack of substrate, the total  substrate metal traces for the reported failing pin was calculated  to be 30000um. And, full package distance from solder ball to  Si die is calculated to be 20 scales, while the open failure is  located at 16th scales from solder ball. By using mathematics  (Full package distance of the failing pin, 30000 um : 20 scales  $=$

open failure distance from solder ball : 16 scales ), the open  failure distance is calculated to be 24000um away from solder  ball; which was then mapped to be substrate metal 3 in this  package. Following physical failure analysis to perform  parallel lapping from Si die site and reach metal 3, this open  failure was physically confirmed due to broken substrate trace.  (Fig. 6)

![SubstrateM3  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ee63c6aa-bcf5-4940-affb-d5a503803c16/ee63c6aa-bcf5-4940-affb-d5a503803c16.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=9109ae138293058e636a2056cff0d838486e3867)
Fig. 6 Parallel lapping until metal 3 found broken substrate trace

## V. CONCLUSION  

Enhanced package fault isolation method using time domain  reflectometry (TDR) incorporation with mathematics  demonstrated a new effective way for fault isolation. With the  incorporation of this cost-free method into existing TDR  machine, destructive failure analysis cycle time has greatly  reduced. Moreover, this method can guarantee higher  percentage of hit rate.

## ACKNOWLEDGEMENT  

The authors would like to thank their colleagues in Xilinx  Asia Pacific Device Analysis Lab (xap_dal) for their support.

## R EFERENCES 

[1]     “Tektronix TDR Application Note”, Tektronix, 2008, Available:  http://www.tektronix.com/oscilloscopes     [2]    K.K. Ng, C. K. Sin, “Investigation of Time Domain Reflectometry  (TDR) on Power Mosfet Semiconductor Device”, Proc. 20th IPFA,  2013, pp 107-111    [3]    Infrastructure Technology Institute, “History of TDR”, Available:  http://www.iti.northwestern.edu/tdr/operational/history.html

