---
title: "129_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_3f0710e670ed8031178fe7cca88ad8327295230462135641
file_size: 653235
---

## TEM-EDX Line Scan to Investigate   $\mathbf{O}_{2}$   Diffusion across Physical Vapor Deposited  Al-Cu Layer   

Wan Tatt Wai\* a , Ong Jia Sheng a , Loh Yeong Jia b  & Low Lynn Yien c

a  Unit Process, Infineon Technologies Kulim, 09000 Malaysia.  b  Process Integration, Infineon Technologies Kulim, 09000 Malaysia  c Product Engineering, Infineon Technologies Kulim, 09000 Malaysia  Phone: +604 4278079 Fax: +604 4278442 \*Email: tattwai.wan@infineon.com

## Abstract 

$\mathrm{O}_{2}$   diffusion through Aluminium-Copper (Al-Cu) layer deposited by physical vapor deposition (PVD) process can be investigated  using TEM (Transmission Electron Microscope) coupled with EDX (Energy Dispersive X-ray) line scan. During PVD process, the  wafer is hot after Al-Cu deposition thus a cooling step is required before the wafer is unloaded (vacuum release). Higher amount of   $\mathrm{O}_{2}$   diffusion was observed for sample with 30s cooling time compared to the one with longer cooling time which is 60s. This  indicated that higher wafer temperature induce higher   $\mathrm{O}_{2}$   diffusion rate in Al-Cu when exposed to air. No  $\mathrm{O}_{2}$   diffusion within  tungsten (W) layer was observed. Al-Cu exposure time to air before it is coated with photoresist is also studied. Wafer with 60s  cooling time and 16 hours exposure time in air has  $\mathrm{O}_{2}$   diffusion level is higher than the wafer with same cooling time but with 8  hours exposure time. The TEM-EDX line scan profile indicated that at room temperature, the   $\mathrm{O}_{2}$   continue to diffuse through Al-Cu  layer at lower rate until its surface is coated with photoresist.  The  $\mathrm{O}_{2}$   diffusion as analyzed by TEM-EDX method is a function of  temperature and time. The higher the temperature, the faster the  $\mathrm{O}_{2}$   diffusion while the longer the exposure time to air, the more the  diffusion of   $\mathrm{O}_{2}$   into Al-Cu.

## Introduction 

Back end of line (BEOL) interconnects metallization for  FET (Field Effect Transistor) technology comprise of  Chemical Vapor Deposition (CVD) process for W deposition  (on barrier layer), followed by PVD process for Al-Cu  deposition (on W). CVD is a deposition method used to  produce high quality thin film such as mono-crystalline,  epitaxial, oxide or metal. Volatile chemical is used as precursor.  PVD is characterized by a process in which the material goes  from condensed phase to vapor phase and then back to thin film  phase, by means of sputtering and evaporation mechanisms. It  is mostly used for metals deposition. After that, there is  lithography patterning step (with photoresist coating) followed  by wet chemical etching for Al-Cu and then W (Fig. 1). The  metal layer stacks are shown in Fig. 2.

![Barrierlayer  Barrier layer  W deposited by  W deposited by   Al-Cu deposited  Al-Cu deposited  CVD CVD   byPVD  by PVD Photoresist  Photoresist   Wet chemicaletching  Wet chemical etching   Photoresist coating  Photoresist coating  removal  removal  ofAl-Cu&W  of Al-Cu & W  onAl-Cu  on Al-Cu ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9b0a1b68-7b0b-4381-96a8-63c866f8d962/9b0a1b68-7b0b-4381-96a8-63c866f8d962.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=ae2b62e6a1224d2421bedd80fa1e1640d346a198)
Fig. 1 Process route of BEOL interconnect metallization for FET.

![Wetetch  Wet etch Resist  Resist  PR AlCu W  Barrier  Banr  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6f2333c8-467f-435f-b1d4-4eed4338cd5c/6f2333c8-467f-435f-b1d4-4eed4338cd5c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=e03136a225b7c7d426b9d452248514362a6fee4a)
Fig. 2 Metal stacks diagram illustrating the metallization steps  followed by photoresist coating & wet chemical etch.

A common defect for this process route was incomplete W  etch (or W residues) after wet chemical process (Fig. 3).  Mixture of sulfuric and nitric acid is used to etch the Al-Cu.  The end of this process should expose the W surface for  readiness of subsequent hydrogen peroxide attack to further  remove the W and open up the barrier layer. W incomplete etch  could happened if there is material properties change of either  Al-Cu or W. Material properties of W is based on the  performance of CVD process while the properties of AlCu is  based on the performance of PVD process. No wafer’s slot  dependency was found for CVD and Wet etch processes.  Therefore, the root cause of the defect can be traced back to  PVD. Furthermore, the dependency of W incomplete etch  occurrence to the exposure time between PVD and photoresist  coating was also observed. Longer the exposure time, higher  the occurrences. Hence, investigation was initiated on how the  properties of Al-Cu changed during PVD process that affect the  underneath W layer [1] and subsequently impact the etching  efficiency during wet chemical process.

![Al-Cu pad Al-Cupad   Al-Cu pad Al-eu-pad  W residues  W residues ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1fac1a14-17c4-4f8d-89bf-c9815f92dd37/1fac1a14-17c4-4f8d-89bf-c9815f92dd37.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=688f49d71f8633872c9d619500279418f7aa93c3)
Fig. 3 Microscopy view of Al-Cu pad and W residues (due to W  incomplete etch) after wet chemical etching and photoresist removal.

PVD process was done in vacuum mode and after the Al-Cu  deposition, the wafer was let to cool down before it was  transferred to unload port for further vacuum release and  unloading (Fig. 4). If the cooling time is not enough and the  wafer remain hot during vacuum release, high level of   $\mathrm{O}_{2}$   can  be diffused into the Al-Cu layer [2]. This is especially true for  the last processed wafer in a single lot in PVD, which has the  highest occurrences of W incomplete etch. The hypothesis is  the last wafer is not given enough time to be cooled down after  coming out from the cooling chamber, and the vacuum is  already released and wafers is unloaded (exposed to air). This  will cause more  $\mathrm{O}_{2}$   diffusion into Al-Cu of the last wafer which  remain hot.

![GMAfXP  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1ae96cdc-3628-40c3-bdce-ae27f7c9fa93/1ae96cdc-3628-40c3-bdce-ae27f7c9fa93.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=e1010d495b7587b4d5235ade8f98d722af4eab2e)
Fig 4. Typical unloading port for PVD tool. Post processed and  cooling wafers will be transferred to the port (vacuum). Vacuum in  unloading port will be released after entry of the last wafer.

On the other hand, although the wafer is already cooled  down, its exposure time to air (before the Al-Cu is coated with  photoresist) can also induce certain amount  $\mathrm{O}_{2}$   diffusion. For  the first time, TEM-EDX line scan method was used for the  investigation of the level of   $\mathrm{O}_{2}$   diffusion through Al-Cu layer  until the Al-  $\mathrm{.Cu/W}$   interface. It was predicted that the significant  amount of   $\mathrm{O}_{2}$   diffused into the Al-Cu layer and the level   $\mathrm{O}_{2}$  accumulated at Al-Cu/W interface could have made the wet  etching of Al-Cu and W difficult.

## Experimental 

4 wafers were prepared as samples for the experiments.  Sample 1 and 2 were prepared at 30s and 60s cooling time  (after Al-Cu deposition step by PVD) respectively. Both  samples have exposure time before photoresist coating of 8  hours.

Sample 3 and 4 were prepared at 30s and 60s cooling time  respectively, with both the exposure time before photoresist  coating is 16 hours (Table 1). Focus ion beam (FIB) was used  to prepare the lamella for TEM analysis (FEI, TECNAI G2).  EDX line scan was performed from the middle layer of the  Al-Cu across the Al-  $\mathrm{\Delta\nu/W}$   interface into the W layer (Fig. 7).

![Vacuum release & wafer unloaded  Vacuumrelease&waferunloaded  immediately after last wafer enter  immediatelyafterlastwaferenter  unloading port from cooling chamber  unloading port from cooling chamber Post PVD wafer  Post PVD wafer Unloading  Unloading  portdoor  port door Cooling chamber  Cooling chamber Unloading port  Unloading port ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c4baa5d9-89b5-4cde-b003-5e2124a88b3c/c4baa5d9-89b5-4cde-b003-5e2124a88b3c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=e25f6f1a78980de337c332930c0edd3c1479084c)
Fig. 5 Illustration of post PVD wafer transported from cooling  chamber to unloading port. The last wafer that enter unloading port  can still be hot if its cooling time is not enough in cooling chamber.

![Al-Cu deposition  Al-Cu deposition   Photoresist coating  Photoresist coating  byPvD  by PVD  onAI-Cu  on Al-Cu Exposure time  Exposure time ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1713bc1d-1480-4c59-bfea-12278de43413/1713bc1d-1480-4c59-bfea-12278de43413.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=29a3b0a7b7b96717de4543330127e9aca804585a)
Fig. 6 Exposure time is a period of idling time for wafers after  unloaded from PVD tool and before starting of photoresist coating  process.

Table 1 Wafer samples preparation for experiments

||30s cooling time|30s cooling time|60s cooling time|60s cooling time|
|---|---|---|---|---|
|#|Exposure time 8 hrs|Exposure time 16 hrs|Exposure time 8 hrs|Exposure time 16 hrs|
|1|+||||
|2|||+||
|3||+|||
|4||||+|


![ Resist  Resist  PR AlCu Area where the TEM-  Area where the TEMW   EDX line scan is done  EDX line scan is done Barrier  Barrier  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a0ef5ccc-a52f-424b-8fcc-fd99b6b761bb/a0ef5ccc-a52f-424b-8fcc-fd99b6b761bb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=55c3d2acee6916aa322782df374164af07a4cf37)
Fig. 7 Illustration of area where TEM-EDX line is performed.

## Results & Discussions 

TEM-EDX line scan profile for wafers which exposure time  are 8 hours (Fig.5) shows significant different between samples  of 30s and 60s cooling time.   $\mathrm{O}_{2}$   diffusion in Al-Cu layer for  sample 1 (30s cooling time) (Fig.5 Top) is strong   $({\sim}5\,\mathrm{\wt{\%}})$  while for sample 2 (60s cooling time) (Fig.5 Bottom) is mild   $(1{\mathrm{-}}2\ \mathrm{wt}\%)$  ) due to lower temperature. This indicated that less

cooling time lead to insufficient reduction of wafer’s  temperature when vacuum is released and thus  $\mathrm{O}_{2}$   is diffused at  higher rate into the Al-Cu layer.

![Al-Cu  Al-Cu  W diffusion in Al-  diffusion in Al- Strong O2  Strong O 2  No O2 diffusion  No O 2  diffusion  through W layer  through W layer Cu (Green line)  Cu (Green line) Image No.: 3Sample No.: 1Tool: TEM  1E816680_05_STEMDX_01  Al-Cu  Al-Cu  W Mild O2  Mild O 2 diffusion in  diffusion in  Al-Cu  Al-Cu  Image No.: 6 Sample No.: 2 Tool: TEM  1E816680_10_STEMDX_01  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/87e3425d-67d0-4727-872b-04cd953ea421/87e3425d-67d0-4727-872b-04cd953ea421.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=3d2626a0d8d5f851fbac35848e4e7c46aa885e71)
Fig. 8 Top: Sample 1 shows strong   $\mathrm{O}_{2}$   diffusion in Al-Cu due to  insufficient reduction of wafer’s temperature Bottom: Sample 2  shows mild diffusion of  $\mathrm{O}_{2}$   in Al-Cu when cooling time is longer.

For the wafer samples with 16 hours exposure time (Fig. 6),   $\mathrm{O}_{2}$   diffusion in Al-Cu layer for sample 3 (30s cooling time)  (Fig.6 Top) is strong while for the sample 4 (60s cooling time)  (Fig.6 Bottom) is moderate   $(3–4\;\mathrm{wt}\%)$  ). This further prove that  longer cooling time reduce   $\mathrm{O}_{2}$   diffusion rate. In addition,   $\mathrm{O}_{2}$  diffusion level is higher for sample 4 (16 hrs exposure time)  when compared to sample 2 (8 hrs exposure time), indicating  long exposure time also lead to slow   $\mathrm{O}_{2}$   diffusion in Al-Cu  although cooling time is sufficient. No  $\mathrm{O}_{2}$   diffusion in W was  observed for all conditions. The   $\mathrm{O}_{2}$   diffusion as analyzed by  TEM-EDX method is a function of temperature and time. The  higher the temperature, the faster the   $\mathrm{O}_{2}$   diffusion while the  longer the exposure time to air, the more the diffusion of   $\mathrm{O}_{2}$  into Al-Cu. The diffusion coefficient in solids at different  temperature is generally found to be well predicted by  Arrhenius equation:

$$D=D_{0}\cdot\exp\left(-{\frac{E_{\mathrm{{A}}}}{R T}}\right)$$
D is the diffusion coefficient,   $\mathbf{D}_{0}$   is the maximal diffusion  coefficient,   $\mathrm{E_{A}}$   ia the activation energy, T is the absolute  temperature and R is the universal gas constant.

Fig. 10 indicate the hit rate of W residues defects of  productive lots. It shows that exposure time more of than 8 hrs  lead to higher occurrence of W incomplete etch (  $40\%$   hit rate).  The experimental results at the same time revealed that sample  4 (16 hrs exposure time with 30s cooling time) has the strongest   $\mathrm{O}_{2}$   diffusion in Al-Cu.

![Al-Cu  Al-Cu  W  Strong O2  Strong O 2 diffusion in Al- diffusion in Al-   No O2 diffusion  No O 2  diffusion  Cu (Green line)  Cu (Green line)  through W layer  through W layer ImaNoSamLnTlTM  Al-Cu Al-Cu   W Moderate  Moderate  C  O 2 diffusion in  diffusion in  Al-Cu  Al-Cu Image No.:6Sample No.: 2Tool:TEM  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/afd51a32-3110-408c-8204-b0728bb9f1ea/afd51a32-3110-408c-8204-b0728bb9f1ea.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=ba2f7ece1f16464eab2b32ab74987d8aed48c4f1)
Fig. 9 Top: Sample 3 shows strong   $\mathrm{O}_{2}$   diffusion in Al-Cu due to  insufficient reduction of wafer’s temperature and long exposure time.  Bottom: Sample 4 shows moderate diffusion of   $\mathrm{O}_{2}$   in Al-Cu due to  long exposure time although cooling time is sufficient.

Therefore the mechanisms of W incomplete etch can be  attributed to the reduced etching efficiency of the Al-Cu due to   $\mathrm{O}_{2}$   incorporated into the Al-Cu layer and changed its material  properties. The phase lattice of the Al-Ox layer is not known,  but it could be some structure which prohibited either the  further oxidation of metal layer by nitric acid or subsequent  dissolution of metal oxide layer by sulfuric acid. Insufficient  etching of Al-Cu subsequently lead to incomplete etch of W  due to the remains of Al-Cu on top of W is not able to be  removed by hydrogen peroxide chemistry effectively. While  the cooling time  needed to be optimized to lower down the  wafers’ temperature for avoiding fast  $\mathrm{O}_{2}$   diffusion, reducing the

exposure time play a more important role to avoid W  incomplete etch. This is because even the wafers of post PVD  process is already cooled down,   $\mathrm{O}_{2}$   diffusion still occurred at  lower rate during long exposure time. The TEM-EDX line scan  method has successfully differentiated the   $\mathrm{O}_{2}$   diffusion level  across Al-Cu layer in response to experimental conditions. The  detection might not come easily if using normal surface  scanning and depth profiling methods.

![100.009%  90.005  80.00%  70.00%  60.005  50.009  40.005%  30.009  20.00%  10.005%  0.0056  2≤hr<44≤hr<66≤hr<88≤hr<1010≤hr<12 12≤hr<1414≤hr<1616≤hr<1818≤hr<24  ExposureTime  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/99cae0bd-aa70-44ed-8263-ef93aab1ca21/99cae0bd-aa70-44ed-8263-ef93aab1ca21.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=465b06683bdf273b088e0524321c89187f8d483e)
Fig. 10 Percentage hit rate or occurrences of W residues vs exposure  time between PVD and photoresist coating.

## Conclusion 

The  $\mathrm{O}_{2}$   diffusion in PVD deposited Al-Cu layer was studied  using TEM-EDX line scan and the results show that at 30s  cooling time after deposition, the reduction of wafer  temperature is not insufficient thus causing high amount of   $\mathrm{O}_{2}$  diffusion in Al-Cu. At longer cooling time as 60s, the diffusion  is mild. This indicated that  $\mathrm{O}_{2}$   might diffused at higher rate into  Al-Cu when it temperature is high. However, even when the  cooling time is sufficient, the exposure time of Al-Cu in the air  before photoresist coating is more critical. The studies found  that among the wafers with 60s cooling time, 16 hrs exposure  time encounter more  $\mathrm{O}_{2}$   diffusion compared to 8 hrs exposure  time at room temperature.   $\mathrm{O}_{2}$   diffusion continued at lower rate  when exposed to air even the wafer’s temperature is already  low. Higher hit rate of W incomplete etch was observed for  wafers with exposure time more than 8hrs, indicating that  limiting the exposure time is critical to reduce the defect.

## Acknowledgments 

Many thanks were extended to characterization laboratory  Infineon Technologies Kulim especially Zakaria Nurhanani for  supporting the TEM-EDX analysis.

## References 

[1]    Y. Pauleau  et al. ,  J. Vac. Sci. & Tech. B. Vol. 6 , pp. 817, 1988.  [2]    I. Prigogine  et al., Advances in Chem. Phys. , Vol. 38 pp. 324-325,  1978.

