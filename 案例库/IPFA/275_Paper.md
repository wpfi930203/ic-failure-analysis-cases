---
title: "275_Paper.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_b9a119c1b9e140bf40d2edb2132f1f397295230462135641
file_size: 3770850
---

EN_PAPER

# CPB fcCSP BGA Package Reliability assessment via the study of Bump Cross Section Morphology after Product Realiability stress testing


CPB fcCSP BGA Package Reliability assessment via the study of Bump Cross Section Morphology after Product Realiability stress testing


## Authors


-                                                


## Abstract


In this paper we study and assess fine-pitch CPB fcCSP BGA package reliability via the study of bump cross section morphology after product reliability stress testing. The IMC formation and progression in copper pillar bump was studied in Mass Production destined SoC Controller to predict the health and life time left for the CPB. In particular we are interested in the reliability of fine-pitch oblong copper pillar bumps arranged in Omni-directional patterns. During product reliability testing, CPB cross-section analysis (Via P-FIB) was performed on CPB bumps strategically located in different sections of the fcCSP BGA package after each reliability test read point. JEDEC standard suite of package related tests were performed. IMC formation and progression under the effect of abovementioned environmental stresses as well as different assembly line variations and materials, including molding compound and substrate, were taken into account. We also compare IMC formation from two different bumping technologies. By assessing the various IMC, void and crack formations, we propose that the product reliability engineer should consider verifying health of product physically in addition to ATE final test. This paper also provides feedback to package technology development from product reliability point of view.


# Introduction


Introduction


In current semiconductor packaging, narrow pitch electrical interconnection and its reliability have become a significant challenge due to the need for high packaging density  [1] .


The traditional lead-free solder bump technology has been difficult to meet the needs for the density and current capacity.


Copper pillar bump interconnect technology, has become commonly used since its introduction in mass production in 2005  [2] [3]  due to its good electrical properties, and electromigration resistance. However, due to process limitation, current copper pillar bump needs to have solder cap, resulting in diffusion reaction between copper and solder forming intermetallic compounds (IMC) or Kirkendall voids inside the joint  [4] . Furthermore, the entire solder joint may be transformed into intermetallic compounds during assembly or operation. This will have a great influence on mechanical, electrical and thermal properties of the whole structure  [5] .


There are a lot of studies about quality and reliability of copper pillar bump technology  [6] [7] [8] . It was found that void formation and cracking at Cu/Cu3Sn and Cu6Sn5/solder interfaces became the dominant failure modes of the bump joint and the Sn solder was usually depleted before the joint failed, which means the joint was only composed of Cu6Sn5 and Cu3Sn phases as a Cu/Cu3Sn/Cu6Sn5/Cu3Sn/Cu structure  [9] . Therefore, there is a need to investigate ways to improve the properties of Cu-Sn IMC. One way to address this could be to add a third element to Cu-Sn based IMCs. Out of different metallic elements studied, Ni is suggested to be a good candidate for addition into solders  [10] .


In this paper, we expand the study of copper pillar bump to real SoC product stressed under product reliability testing. We incorporate novel cross-section analysis techniques to evaluate IMCs formation in the copper pillar bump. We will intensively discuss the effect of Ni layer in the copper pillar bump. This will provide feedback to package technology development, as well as further recommendation for product reliability engineer.


# Experiment


Experiment


# A. Samples


A. Samples


The fcCSP BGA product, a SoC controller chip with metal lid, was selected as test vehicle  [1] [2] . The chip was manufactured using 28nm logic process technology node from a leading foundry. The stack up (Metal  &  ELK) follows the foundry standard process and incorporates a PI layer on top of the passivation layer. The bump dimensions prior to reflow are 55µ, 45µ Height  &  width respectively. The UBM dimensions are 75µ, 45µ. The copper bump has an oblong shape and are arranged in Omni-directional patterns. There is a Nickel layer between the copper pillar and the solder cap in order to prevent Cu diffusion into solder. Figure  1(a)  shows the illustration of the bump's cross-section after chip attach reflow process step and figure 1(b) shows the SoC controller bump pattern layout.


As a comparison, we also selected another SoC controller chip which was manufactured using 16nm logic process technology node from the same foundry but different bumping technology from assembly house. The main difference in terms of copper pillar bump is that there is no nickel layer between copper pillar and solder cap.


# B. Test Condition


B. Test Condition


SoC controller chips from 28nm logic process technology node with different molding compounds and substrates were manufactured, in order to study the effect coming from package materials. Product reliability tests according to JEDEC standard were conducted on the parts. At least one part was pulled after each read point for further analysis. The new SoC controller chip manufactured using 16nm logic technology node and different bump technology without nickel layer between copper pillar and solder cap was also subjected to temperature cycling test and the unit post 750 cycles was selected for the same analysis.


# C. Analysis


C. Analysis


Cross-section analysis was performed after each reliability read point on corner bumps to maximize the impact from reliability stress. Two bumps were selected and each bump was cross-sectioned along the long side and perpendicular to the long side. Figure  2  shows the overview of the sample after lapping off the substrate and the locations for the cross-section analysis, as well as the directions for the cross-section analysis.


For cut #1, the direction is perpendicular to the short side of the oblong shape. Plasma-FIB milling and imaging were used due to its fast milling speed, accuracy, less damage and wide coverage. It is important to have large observed area for quantitative analysis. More discussion about this unique cut techniques and its benefit can be found in reference  [11] . For cut #2, Cross-section Polisher (CP) and SEM imaging were utilized. The copper pillar bumps were then inspected by SEM. The thickness of IMCs were measured. EDX analysis was also performed across all layers in the bump to reveal the composition of IMCs, as shown in Figure  3 .


# Results and discussions


Results and discussions


# A. Results from different cross-section directions of oblong bumps


Figure  4 (a) shows the cross-section along the long side of the copper pillar bump (P-FIB cross-section) and figure  4(b)  shows the cross-section along the short side (CP crosssection). It is clearly shown the different shapes of the crosssections from different cutting locations. The difference is due to the oblong shape of the bump. The bump reflow can be observed to be different from the two directions. IMC formation can be observed. More details will be discussed in the next section. The following observations can be made:


# B. IMC formation as progression of temperature cycling test


1. On the copper pillar bump side, Ni layer was clearly seen. It effectively stopped the diffusion of copper to the solder. Less IMCs were formed compared to the copper trace side.


2. On the copper trace side, more Cu6Sn5 was formed.


A closer look even showed Cu3Sn which indicated more copper diffusion from trace into solder cap.


# E. IMC formation from different bumping technology and process -with or without Nickel layer between the CPB and the solder


E. IMC formation from different bumping technology and process -with or without Nickel layer between the CPB and the solder


As a comparison, Figure  8  shows the cross-section of copper pillar bump from another SoC controller chip manufactured using different bumping technology: (a) before reliability testing; (b) post temperature cycling 750 cycles; and (c) closer look of IMCs in the copper pillar bump. This bumping technology doesn't include the Nickel layer between the copper pillar and the solder cap. It is clear that copper in the pillar diffused into solder cap even before any reliability testing and formed brittle Cu3Sn IMC phase. Post temperature cycling 750 cycles, unlike the previous product, solder was consumed and IMC formation was enough to fully connect copper pillar and copper pad. Kirkendall voids were also observed all over the bump structure. This indicates the change of mechanical and electrical properties of the copper pillar bump structure, as well as reliability concern in the long run.


|4|Supplier G|Supplier I|

|DOE|Molding Compound|Substrate|Ni3Sn (μm)|Cu6Sn5 (μm)|Cu3Sn (μm)|
|---|---|---|---|---|---|

|1|Supplier X Supplier U 0.958|Supplier X Supplier U 0.958|Supplier X Supplier U 0.958|2.436|0.518|

|2|Supplier X Supplier I|Supplier X Supplier I|0.734|3.825|0.518|

|3|Supplier G Supplier U 0.978|Supplier G Supplier U 0.978|Supplier G Supplier U 0.978|2.201|0.724|

|4|Supplier G Supplier I|Supplier G Supplier I|0.832|2.661|0.538|

|D. IMC formation post different reliability tests|D. IMC formation post different reliability tests|D. IMC formation post different reliability tests|D. IMC formation post different reliability tests|D. IMC formation post different reliability tests||

A. Results from different cross-section directions of oblong bumps


# F. Kirkendall Void formation observations throughout this study


F. Kirkendall Void formation observations throughout this study


We noticed that Kirkendall void formation was most frequent to two areas in our structures under DOE. In the Sn-Cu interface between solder cap and Cu trace. And at the side wall of the CPB between wicked Sn and Cu pillar bump.


Figure  9  shows such voiding mechanisms. The voiding between Sn and Cu at the side of the CPB wall shown in figure  9 (a) is considered non-critical. However the voiding between Sn in bump solder area and Cu trace is critical.


# G. Available solder volume in solder cap (thickness) and its relation to long term reliability


G. Available solder volume in solder cap (thickness) and its relation to long term reliability


We collected this data from the large number of Cut2 bumps/samples that we performed and noticed the following trend. Figure  10  shows gradual depletion of Sn in bump area for samples undergoing HTS reliability testing. As we progressed in the reliability stress test we noticed the conversion of Sn to its basic IMC formations; which is a well-documented phenomenon in many of the published literature article on this subjects  [9] . For the Bump structure with Ni barrier that transformation was much slower than a different bump structure without the Ni diffusion barrier shown in Figure  11 . The latter literally running out of Sn in the solder bump area and fully transformed into many of the different IMC including the brittle IMC phase Cu3Sn. We believe the combination of Ni barrier and 8-12µ of solder thickness in bump area is ample enough to sustain 10 Years' worth of reliability for a consumer application end product. The fact that bump structure is oblong (oval) also contributes to larger effective bump area and is a major contribution factor to this enhanced long term reliability. However the secondary product with no Ni Barrier seems to pause a risk for field life given its IMC structure.


# Conclusions


Conclusions


Based on the exhaustive cross-section analysis and thorough discussions, the following conclusions can be made:


1. In this fine pitch copper pillar bumping technology, Ni layer between copper pillar bump and solder cap is highly recommended since it effectively reduced the diffusion of Cu to Sn hence formation of brittle IMC Cu3Sn and Kirkendall void formation. This can also help to sustain both mechanical and electrical properties of copper pillar bump. This is beneficial for real product lifetime.


2. For our particular package structure other packaging materials, namely molding compound and substrate, have negligible effect on IMC formation throughout the entire product lifetime.


3. Temperature is the largest driving force for Cu diffusion and IMC formation. As can be seen from HTS, solder cap was completely consumed after 1000 hours. Future study may be focused on the available solder volume in the solder cap and its relation to long term reliability.


4. We believe that relying on ATE solely is not enough to assess the health of the CPB structures. Such bump cross section observation after reliability stress testing, on the other hand, offers a more comprehensive and conclusive way. We recommend product reliability engineer to consider physical cross-section review of CPB structures as supplemental criterion for product qualification.


|Preconditioning|T0, Post-PC|2|
|---|---|---|

|TC (Cycles)|250/500/750/1000/2000|5|

|HTS (Hours)|168/500/1000|3|

|UHAST (Hours)|96/168|2|

|BHAST (Hours)|96/168|2|

|DOE|Molding Compound|Substrate|
|---|---|---|

|1|Supplier X|Supplier U|

|2|Supplier X|Supplier I|

|3|Supplier G|Supplier U|

## References


-                                                                                                                                                                                                         

