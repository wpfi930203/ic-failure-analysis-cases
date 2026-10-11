---
title: "148_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_686bb26ce6a8124dd6dc091ff5f020b87295230462135641
file_size: 868925
---

## Backside Preparation by Milling Approach of Module  Device for Failure Analysis  

Kevin Emmanuel Fulla Jr. 1 , Mark Anthony Acedillo 2    Febus Reidj Cruz 3 , Flordeliza Valiente 4   Maxim Integrated – Failure Analysis Department, Gateway Business Park, General Trias Cavite, Philippines  School of Electrical, Electronics, and Computer Engineering, Mapua University, Manila, Philippines  Phone:  $+63$   (2) 902-2000 local 2396;   Email:  1 KevinEmmanuel.Fulla@maximintegrated.com,  2 Mark.Acedillo@maximintegrated.com,   3 reidjcruz@gmail.com,  4 FLVALIENTE@mapua.edu.ph

Abstract —  The traditional chemical decapsulation of module devices  led to new failure analysis (FA) issues. Conventional backside sample  preparation or decapsulation for module devices is prone to damage  and time consuming. As a result, chemical and other mechanical  backside preparation techniques have very small success rates to  maintain the electrical behaviour of module devices. This study  proposes a backside decapsulation technique with better result that  takes a lesser cycle time and preserves the physical profile and electrical  behaviour of the device.

Keywords  —  Backside Preparation/Decapsulation, Bench Test,  Fault Isolation, Milling, X-prep, Module Devices

## I.    I NTRODUCTION 

Fault isolation has a major role in failure analysis. It helps in  the localization of the damage/defect in the failing device. [1]  Devices are subjected for decapsulation to expose the die surface  prior to fault isolation. Backside fault isolation is a common  method for die level failure analysis wherein the active circuitry  in the substrate layer can be easily inspected; thus, localization is  easier in comparison to front side fault isolation. [2]

Module devices were developed for industrial power supplies.  These devices have components built inside like. They have  components built inside like (i.e. transformer, inductor, capacitor,  etc.) molded within the plastic package along with the device’s  die. Components built in the module are highly sensitive and  prone to damage when performing chemical decapsulation.  Additionally, chemical decapsulation may also damage metal  traces on the substrate which should be connected to the device on  the other components. [2] Front side decapsulation using  chemicals like Nitric acid and Sulfuric acid is only suitable if a  device already has a suspected defect and preserves the electrical  behaviour of the device for fault isolation was not a concern. In a  recent study, backside polishing is one of the more common  backside sample preparation techniques used in failure analysis.  Part of the substrate thinned down until the target area is exposed.  [3]

The main objective of this study is to develop a new backside  decapsulation or preparation process for module devices.  Specifically, the paper aims (1) to achieve better decapsulation  results that will expose the backside of the die without physical  damage while preserving the electrical behaviour of the device;  (2) to determine which specific tool/s and settings should be used  for faster milling; (3) to have an experimentation or  characterization using the milling approach for better results and  reduced cycle time; (5) to increase the success rate of finding the  root cause of failure and reduce the chemical usage.

This paper will only focus on one module device characterized  with four different tool path patterns and three different drill bit  diameters. Specific opening/location will be milled out as outlined  using X-prep tool. Lastly, the author will use the device’s  evaluation kit for electrical verification.

## II.   R EVIEW OF RELATED LITERATURE   

Based on the paper entitled “Novel Sample Preparation  Techniques in Exposing Die Backside on Molded Packages”, the  researcher used the traditional backside decapsulation techniques  which were chemical etching, laser ablation, and mechanical  lapping to peel off the copper die pad. This paper presented two  novel samples of deprocessing approach to expose the die  backside in a molded package. The researcher focused on the  mechanical approach when there is a need for material analysis  and chemical approach when the units are for electrical  characterization and fault localization. [2]

Based on the paper entitled “Characterization of Wet Chemical  Etching for Effective Backside Sample Preparation on Devices  with Exposed Pads”, the researchers presented a methodology for  backside sample preparation on devices with exposed pad/flag  using wet chemical etching and compared it with mechanical  backside polishing. They used a non-fuming nitric acid with  $69\%$  -  $70\%$   concentration and any temperature between   $80^{\circ}\mathrm{C}$   to   $150^{\circ}\mathrm{C}$  ,

a backside sample preparation can be achieved in less than 15  minutes. [3]

Based on the paper entitled “Novel Backside Sample  Preparation Processes for Advanced CMOS Integrated Circuits  Failure Analysis”, the researcher developed a backside  preparation technique where “blown capacitor” defect and “block  metal etch” defect were observed during fault localization. In  addition, the researcher used an Anti-Reflection Coating (ARC)  to improve the success rate and sensitivity of backside photoemission microscopy. [4]

In the paper entitled “Simple Die-Level Backside Thinning  Sample Preparation Method for Failure Localization”, the  researcher focused on an alternative way to perform difficult  sample preparation process which is difficult to the failure  localization from backside silicon. Experienced analysts choose to  vary the abrasive materials and resources for more desirable  results. Various improvements and modifications can be made to  different analysis objectives and final thickness requirements. [5]

Based on the paper entitled “Sample Preparation on Backside  Mechanical Decapsulation Methodology for Effective Failure  Analysis on Non-Exposed Die Pad Package”, chemical etching is  not recommended for backside sample preparation. Due to quick  reaction of  $65\%$   Acid Fuming Nitric, the copper leads were almost  etched off even when sealed with 3M High Temperature Tape.  The paper proposed backside mechanical sample preparation  replacing existing chemical etching which ensured the copper  leads are intact for further failure analysis. [7]

## III.   METHODOLOGY  

Figure 1 shows the bond diagram of the module device used in  this study. It indicates the area where the milling should be  focused.

![C  14  34   E13  12  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b5983346-963f-457d-91cd-b83e9eac9530/b5983346-963f-457d-91cd-b83e9eac9530.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=fe4e57f38e9cc8f9abab95ea21a41148b9f6bff7)
Figure 1.   Bond diagram of a module device showing the area to be  milled (red box).

Figure 2 shows the detailed process/steps of how to perform  backside preparation on the exposed pad of a module device.

![Start  Sample and Tool  Preparation  Selecting Milling  Region  Leveling Sample / Z-Origin  Defining Milling  Location  Setting X/Y Feed  Rate and Patterns  SettingParameters  (Material Removal,Tool  Sample  RPM, Number of Passes)   Checking  Start Milling   End  Doesthemilling   yes  achieved the  desired output?  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2afb393f-4814-4d04-ad9c-bcc8689bdc7d/2afb393f-4814-4d04-ad9c-bcc8689bdc7d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=9ecfc52636c5f7e078efa078c07cdb2af2e379d8)
Figure 2.   Process flow of the milling approach.

## 3.1 Sample and Tool Preparation:  

Samples were fixed onto a Borosilicate glass using melted  crystal wax. Crystal wax can be melted using a hot plate with a  temperature of   $130^{\circ}\mathrm{C}$  .

The glass slide with the mounted sample was placed on a  fixture and was secured by tightening the screws on each side of  the fixture. The fixture was then placed on the platform and the  thumb screw was tightened. Al/Cu tipped probe was inserted with  safety cover open and the tool was placed and held in the collet as  shown in Figure 3.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9af1bc8d-cca9-45a4-b917-de7c0b1e58de/9af1bc8d-cca9-45a4-b917-de7c0b1e58de.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=679047186fe06869beb91ead8b9d70cb13f733c7)
Figure 3.   (A) Unit mounted on fixture; (B) Tool selection.

## 3.2 Milling Region Selection:   

Figure 4 shows the different milling modes of the tool. Visible  Region/Object, Non-Visible Region-Centered; Non-Visible  Region – non-centered, and four-sided Trench. In this paper,  Visible Region/Object was used since the target area (exposed  pad) was visible with the machine’s camera and top left and  bottom right can be aligned using the tool’s cross hair.

![ALLIGD  SelectMode  VisibleRegion/Object  Non-VisibleRegion/Centered  Non-Visible Region/Non-Centered  Four(4)SidedTrench    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/69a10d60-40f0-4fe9-bfde-064498bf5360/69a10d60-40f0-4fe9-bfde-064498bf5360.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=b461b246048bbe72daac0d8d5f603ab45a2628e3)
Figure 4.   Mode Selection.

3.3 Levelling the Sample and Z-Origin:

Figure 5 shows the points of origin for the levelling process and  the z-origin parameters. This is an option that would be used to  correct the uneven mounting of the sample to the glass in the  fixture. The levelling process is automatic and involves touching  probe tip directly on the surface of the sample. The determination  of level is the difference in height between points for each axis (X  and Y). Z-origin is an automatic touch down in the center of the  defined region. It is used to determine where the surface of the  part is located or how far the spindle needs to move in order to  touch the surface of the part. Once established, this Z-Origin  becomes the reference for material removed until the origin has  been redefined by the user, or another tool has been inserted into  the collet.

![ogivsin  Z-Origin  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0e5a31d1-4d4f-4d6f-b683-e4bf51e59564/0e5a31d1-4d4f-4d6f-b683-e4bf51e59564.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=c321df0008b7e390300e3146f30b434ee3fbb9e5)
Figure 5.   (A) Levelling points of origin; (B) Z-origin parameters.

## 3 .4 Defining Milling Location: 

Figure 6 shows the location of the visible region where milling  should be focused. X/Y axis was defined on the top left and  bottom right corners where the spindle should be milled that had  been locked.

![ALLIED  Define  Milling/Pollshing Reg  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e3f63c5b-ce30-41a5-abcf-1ed2ef2ab4c8/e3f63c5b-ce30-41a5-abcf-1ed2ef2ab4c8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=610e9b2346298ade9f977b4a78c958105ed51b87)
Figure 6.   Target location for visible region definition.

## 3.5 Setting X/Y Feed Rate and Patterns  

X/Y feed rate depends on the diameter of the tool.   X/Y Feed rate  $=$  Tool diameter x 3

Figure 7 shows the different tool path patterns on which  direction the spindle should move.

![D  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1eeaee92-cd49-4bb3-bca7-7516dde370d9/1eeaee92-cd49-4bb3-bca7-7516dde370d9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=250d2351a0e6cd79922c169e0e41483803734309)
Figure 7.   Tool path patterns (A) vertical serpentine; (B) horizontal  serpentine; (C) spiral serpentine; (D) combination of a and b.

3.6 Setting Parameters (Material Removal, Tool RPM, Number of  Passes):

Figure 8 shows the final review of the parameters prior to  milling. Material removal was set on the desired amount of the  material to be milled or removed. Tool RPM is the speed of the  tool which is set to 22,000 rpm for copper exposed pads. The  number of passes is set on how many passes/cycles for the probe  tip to mill the location.

![ALLIGD  Setup:   Active:  Material Removal:   19m   Remaining   0.0pm  Number of Pas   Completed:   190.0pm  Amount perPass   19.o0um   RemainingPasses  X/YFeed Rate   omm/s   Above Z-origin Point  Z-Position:   0.opm  Tool RPM:   2000  Cycle Time:   0:00:00  Total Remov.  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/27c505b6-c98a-4edf-b38d-e0696404e323/27c505b6-c98a-4edf-b38d-e0696404e323.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=7dc9e40e544268533052be0d3cb88f34f3f83531)
Figure 8.   Final review of parameters or the start screen prior to milling.

IV.   R ESULTS AND DISCUSSIONS

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c0f23186-a63a-414f-a3c3-b1b24f27869b/c0f23186-a63a-414f-a3c3-b1b24f27869b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=b9e378918552300aa87b66aad59d7651950beb07)
Figure 10. Partial backside IR inspection using Laser Scanning Optical  Microscope.

## 4.2.2 Optical inspection: 

4.1. Milling approach of exposing the backside of the die.

Figure 9 shows the transition of the module device from an  intact unit to an exposed die backside.

![ExposedPad  Copper  DieBackside   Die Attach  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/11b8dfc5-a117-43e1-b772-9903c7b19bd6/11b8dfc5-a117-43e1-b772-9903c7b19bd6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=72ffeb0a16e6030ced704e1e001de69ef9859696)
Figure 9.    (A) Backside of the package prior to backside milling; (B)  Copper exposed after removal of exposed pad; (C) Die attach is  exposed; (D) Exposure of the die backside after die attach removal.

4.2. Backside inspection method after exposing the die backside:

After removing the exposed pad and die attach, the backside of  the die was inspected using the following methods:

## 4.2.1 Backside IR Inspection: 

A method used to thoroughly inspect the whole die from the  silicon level up to the top metal lines. Visible defect or damage  such as electrical overstress (EOS) damage can be easily seen  from the backside using IR inspection as shown in Figure 10.

Figure 11 shows the die backside when inspected using low  power microscope. This is the most common method used to  inspect the backside of the die if there is a sign of die crack or  chip-out.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6743334e-3826-4e48-9a0a-de6d8e453a44/6743334e-3826-4e48-9a0a-de6d8e453a44.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=3aa902a0bb945cb004867ae69a69b31c5e94317a)
Figure 11.   Backside inspection using low power optical microscope.

## 4.3 Data Gathering  

This section shows all data gathered during the milling process  and includes the before and after results of electrical verification  of the module device.

As presented in Table 1, four different tool path patterns and  three different drill bit sizes were used and characterized for the  fastest cycle time. Results showed that the 1mm Al/Cu Drill Bit  and the D tool path pattern has the fastest cycle time with the  fastest completion and recorded at only 4.33 minutes.

Table 1.   Summary of results showing the total cycle time using different  drill bit diameters and tool path patterns.

|S/N|Tool Path Patterns|Al/Cu Drill Bit Diameter (mm)|Total Cycle Time (minutes)|
|---|---|---|---|
|1|A|0.5|45.02|
|2|A|0.7|30.42|
|3|A|1|5.23|
|4|B|0.5|26.88|
|5|B|0.7|19.75|
|6|B|1|5.42|
|7|C|0.5|33.02|
|8|C|0.7|26.72|
|9|C|1|6.88|
|10|D|0.5|26.28|
|11|D|0.7|24.55|
|12|D|1|4.33|


Figure 12 shows the interaction plot with the fastest approach  in milling the exposed pad of a module device was conducted  using tool path pattern and tool diameter. This plot provides an  idea on how long it will take to mill and expose the backside of  the die using the right combination of tool path patterns and tool  diameter.

![InteractionPlotforCycleTime  DataMeans  SO  Pattern  40  30  20  TO  a(o.5mm)   b(o.7mm)   c（1mm)  Diameter  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f08e252c-9526-4e8b-bf4f-f3e10495de8b/f08e252c-9526-4e8b-bf4f-f3e10495de8b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=a2cd390a734b34e55733274180d8311cd7bef144)
Figure 12. Interaction plot for cycle time.

Note: Since the Pattern D is the last experiment for the 0.7mm  diameter, the bit has been overused and resulted to consume more  time than diameter   $b(0.7m m)$  ; Pattern (B).

As presented in Table 2, all the units subjected to backside  decapsulation were evaluated on bench. Results showed that  backside decapsulated units have the same electrical readings, in  comparison to an intact unit. After conducting the electrical  verification,   $100\%$   of the units were still found functional. Thus,  the backside decapsulation process did not affect the electrical  behaviour of the device.

Table 2.   Bench test results

|S/N|Conditions|Supply Current Reading (mA)|VCC (V)|VOUT (V)|
|---|---|---|---|---|
|REF1|Intact Unit|8.569|5.080|3.327|
|REF2|Decapped REF1|8.599|5.065|3.297|
|1|Backside Decapsulated Units|8.763|5.049|3.331|
|2|Backside Decapsulated Units|8.609|5.042|3.333|
|3|Backside Decapsulated Units|8.798|5.065|3.311|
|4|Backside Decapsulated Units|8.832|5.074|3.329|
|5|Backside Decapsulated Units|8.734|5.063|3.311|
|6|Backside Decapsulated Units|8.651|5.079|3.303|
|7|Backside Decapsulated Units|8.721|5.061|3.320|
|8|Backside Decapsulated Units|8.790|5.067|3.306|
|9|Backside Decapsulated Units|8.732|5.063|3.314|
|10|Backside Decapsulated Units|8.624|5.064|3.306|
|11|Backside Decapsulated Units|8.682|5.066|3.309|
|12|Backside Decapsulated Units|8.782|5.062|3.311|
|Datasheet Specifications|Datasheet Specifications|TYP=9.5|MIN=4.75 TYP=5 MAX=5.25|3.3|


## V.   C ONCLUSIONS 

In this work, backside decapsulation or preparation of module  device was done through milling approach. The proposed  backside decapsulation process successfully exposed the die  backside while preserving the electrical behaviour of the device.

The use of larger drill bit diameter (1mm) and a combination of  vertical and horizontal serpentine tool path patterns could result to  a lesser cycle time. It may also increase the success rate of root  cause finding resulting from the next failure analysis step/s, lessen  the cycle time of the analysis, and reduce of chemical usage.

## VI.   R ECOMMENDATIONS 

The author presents these recommendations for the future  researchers to further improve this research: (1) Frontside  decapsulation or preparation using milling approach. (2)  Optimizing the advance option of X-prep tool by using 3D contour  workflow and apply it on other devices. (3) Considering other  mode selection of the X-prep tool especially on device with no  exposed pads using Non-visible Region / Centered or Non-Visible  Region / Non-Centered.

## VII.   A CKNOWLEDGMENT 

The author would like to thank Maxim Integrated Philippines  Failure Analysis Department for the assistance, usage of  equipment and resources to finish this research paper.

## VIII. R EFERENCES 

[1]    Yu, H.-T., Liu, H.-C., Huang, C.-C., & Huang, S.-M. (2018).  Case Study for Backside Sample Preparation in Copper  Based Dummy Package.   2018 IEEE International  Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), Singapore , 1-4.    [2]    Mendaros, R., & Capito, E. (2011). Novel Sample  Preparation Techniques in Exposing Die Backside on  Molded Packages.  18th IEEE International Symposium on  the Physical and Failure Analysis of Integrated Circuits  (IPFA), Incheon , 1-4.    [3]    Sabate, A. C., & Galarce, R. V. (2014). Characterization of  Wet Chemical Etching for Effective Backside Sample  Preparation on Devices with Exposed Pads.  Proceedings of  the 21th International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA), Marina Bay  Sands , 94-97.    [4]    Chew, Y. Y., Siek, K. H., & Yee, W. M. (1999). Novel  Backside Sample Preparation Proceses for Advanced  CMOS Integrated Circuits Failure Analysis.  Proceedings of  the 1999 7th International Symposium on the Physical and  Failure Analysis of Integrated Circuits , 119-122.    [5]    Lee, N. (2017). Simple Die-Level Backside Thinning  Sample Preparation Method for Failure Localization.  2017  IEEE 24th International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA), Chengdu , 1- 4.    [6]    Loh, T. H., Yee, W. M., & Chew, Y. Y. (1999).  Characterization and Application of Highly Sensitive InfraRed Emission Microscopy for Microprocessor Backside  Failure Analysis.  Proceedings of the 1999 7th International  Symposium on the Physical and Failure Analysis of  Integrated Circuits, Singapore , 108-112.    [7]    Ong, P., Ng, K., & Gwee, H. (2018). Sample Preparation on  Backside Mechanical Decapsulation Methodology for  Effective Failure Analysis on Non-Exposed Die Pad  Package.  2018 IEEE International Symposium on the  Physical and Failure Analysis of Integrated Circuits (IPFA),  Singapore , 1-4.    [8]    Wu, H., & Cargo, J. (2004). Backside Failure Analysis and  Case Studies for Cu/Low k Technology.  Proceedings of the  11th International Symposium on the Physical and Failure  Analysis of Integrated Circuits. IPFA 2004, Taiwan , 127- 134.

