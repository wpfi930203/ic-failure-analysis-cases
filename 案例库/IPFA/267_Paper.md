---
title: "267_Paper.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_eeeacc86c26299c1183618b192f7c9cd7295230462135641
file_size: 4832570
---

## Investigating Reliability Issues in Multi-Layered STT-MRAM with Synthetic Antiferromagnets 

Mario Bendra ∗ , † , Roberto Lacerda de Orio † , Wolfgang Goes ‡ , Siegfried Selberherr † , and Viktor Sverdlov ∗ , † ∗ Christian Doppler Laboratory for Nonvolatile Magnetoresistive Memory and Logic at the †  Institute for Microelectronics, TU Wien, Gußhausstraße 27-29, A-1040 Wien, Austria ‡  Silvaco Europe Ltd., Compass Point, St Ives, Cambridge, PE27 5JL, United Kingdom e-mail: bendra@iue.tuwien.ac.at

Abstract —In exploring the reliability issues of multi-layered STT-MRAM, particularly with synthetic antiferromagnets, our research delves into the complexities of magnetization dynamics. We leverage the spin drift-diffusion model to investigate the intricacies of the back-hopping effect which leads to undesired switching in the device’s layers. This phenomenon is notably magnified as devices become smaller, aiming for higher memory density but at the cost of data integrity. Our focus extends to the nuanced role of interface exchange coupling in multilayered configurations, illustrating its pivotal influence on the magnetic interactions and stability within these advanced spintronic devices. By examining how the non-magnetic layers mediate exchange coupling and impact the magnetic coherence between ferromagnetic layers, we gain crucial insights into the mechanisms driving magnetic stability and domain wall behaviors. This comprehensive approach, encompassing both charge and spin currents, offers a comprehensive view of MRAM dynamics and underscores the importance of fine-tuning exchange coupling for enhanced device performance. This kind of advancements are aimed to significantly elevate the capabilities of memory technologies, paving the way for improved data retention and faster write/read operations. Our findings represent a significant stride in advancing high-capacity and high-efficiency memory solutions.

Index  Terms —reliability  issues,  spintronic  devices,  backhopping, spin-transfer torques, interlayer exchange coupling, micromagnetics, synthetic anti-ferromagnetic

## I. I NTRODUCTION 

Investigating the reliability of multi-layered spin-transfer torque  magnetoresistive  random  access  memory  (STTMRAM)  equipped  with  synthetic  antiferromagnets  is paramount, especially as this technology finds increasing application in sectors such as computing-in-memory systems [1], automotive [2], real-time industrial environments [3], and  high-density  storage  configurations  [4].  Central  to STT-MRAM’s architecture is the magnetic tunnel junction (MTJ), consisting of a CoFeB reference layer (RL) and a free layer (FL), separated by an MgO tunnel barrier (TB) or a non-magnetic spacer (NMS), a design critical for achieving the  miniaturization  necessary  for  high-density  memory advancements [5].

The trend towards smaller cell sizes, however, introduces significant reliability challenges, including the back-hopping phenomenon which compromises memory cell stability [6], [7]. Addressing these issues has led to a concentrated effort on leveraging interlayer exchange coupling (IEC), a mechanism

![NMS  NMS  TB  TB ca  (a) NI  NM  HL  RI  RL  ET  FL  NI  NM J Tieci  iec 1 NMS  NMS  NMS  NMS TB TB  CDD  (b) NI  NM  HL  RI  RL  PI  PL  FL  NI  NM J Tieci  iec 1  J TieC2  iec 2 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f7ad063e-577a-4257-8464-ce961414cb64/f7ad063e-577a-4257-8464-ce961414cb64.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215785%3B1743219385&q-key-time=1743215785%3B1743219385&q-header-list=host&q-url-param-list=&q-signature=a05a69771fd7f3295b921bd5b3d3a97671680775)
Fig. 1. This figure shows the intricate design of a multilayered MRAM cell. Color-coding is utilized for clear differentiation of components: the hard layer (HL) is marked in yellow, the RL in red, the FL in blue, the PL in teal, the TB in orange, and the NMS in green. Non-magnetic (NM) contacts are represented in gray. Interfacial engineering regions are highlighted by white zigzag lines. The interaction strengths between the HL and the RL and between the RL and the PL are denoted by    $J_{i e c_{1}}$   and    $J_{i e c_{2}}$  , respectively.

vital for the performance and stability of memory cells, particularly in multi-layer cell configurations and complex MTJ stacks aimed at increasing memory density [8].

IEC’s role in defining the magnetic orientation of ferromagnetic layers, with a focus on the efficiency of metallic spacers, has been extensively studied to adapt MTJ performance across a wide array of applications, potentially replacing traditional memory systems [9]. Advancements in MTJ technology, especially in the CoFeB/MgO system known for its perpendicular magnetic anisotropy, include efforts to enhance interfacial anisotropy through strategies like adding a capping layer or inserting additional  $\mathrm{MgO}$   or non-magnetic spacer layers within the free layer [10], [11]. These innovations have facilitated the downscaling of MTJ dimensions and their commercialization by semiconductor foundries [12].

Our exploration of IEC in multilayered structures reveals its critical influence on magnetic stability in spintronic devices, essential for efficient STT switching. Our investigation aims to optimize interlayer exchange coupling to improve data retention and write/read speeds in memory devices, directly addressing the pressing reliability issues associated with STTMRAM’s miniaturization [6], [7], [8].

We investigate the complexities of multi-layered MRAM cells through a detailed evaluation of spin-transfer torques, which is crucial for the memory’s fundamental operation. Our study introduces a detailed modeling approach which accurately captures the essential physical phenomena governing spin-transfer torques.

Fig. 1 presents two distinct schematic views of multilayered MRAM cells, designated as Stack A and Stack B. Fig. 1(a) illustrates Stack A, portraying a composite MRAM cell comprised of a layered structure with a CoPt HL, a Ru NMS, a CoFeB RL, an MgO TB, and a CoFeB FL. The thicknesses are specified as HL ( 5 . 3 nm ) — NMS Ru ( 0 . 85 nm ) — RL ( 1 . 1 nm ) — TB ( 0 . 9 nm ) — FL ( 1 . 4 nm ), connected to non-magnetic (NM) contacts of ( 50 nm ).

Fig. 1(b) depicts Stack B, showing a more complex MRAM structure which incorporates CoPt in both the hard and reference layers, with Ru and Ta as NMS, a CoFeB spinpolarization layer (PL), an MgO TB, and concluding with a CoFeB FL. This arrangement is described as HL ( 5 . 3 nm ) —  $\mathrm{{NMS}_{\mathrm{{Ru}}}}$   ( 0 . 85 nm ) — RL ( 3 . 2 nm ) —  $\mathrm{NMS_{Ta}}$   ( 0 . 4 nm ) — PL ( 1 . 3 nm ) — TB ( 0 . 9 nm ) — FL ( 1 . 4 nm ), ending with NM contacts ( 50 nm ). The overall diameter for both stacks is 70 nm .

The simulation parameters for the various MRAM setups displayed in Fig. 1 are listed in Table I, with corresponding references [13], [14], [15], [16]. These parameters align with experimental observations noted in NMS research [17], [18], with significant instances of coupling strengths surpassing  $\pm2~\mathrm{mJ/m^{2}}$    documented in [19].

Our study employs the Landau-Lifshitz-Gilbert (LLG) equation to capture the dynamics of normalized magnetization in multi-layered MRAM cells, using the finite element method (FEM) for numerical solutions. The LLG equation, is as follows:

$$\frac{\partial\mathbf{m}}{\partial t}=-\gamma\mathbf{m}\times\mathbf{H_{\mathrm{eff}}}+\alpha\mathbf{m}\times\frac{\partial\mathbf{m}}{\partial t}+\frac{1}{M_{S}}\mathbf{T_{S}}$$
(1)

m  represents the normalized magnetization vector, with    $\gamma$  and    $\alpha$   denoting the gyromagnetic ratio and Gilbert damping constant, respectively. The term    $\mathbf{H}_{\mathrm{eff}}$   denotes the effective field, while    $\mathbf{T_{S}}$   signifies spin-transfer torque contributions.

Interlayer exchange coupling (IEC), crucial for MRAM functionality, is modeled with the boundary term for energy density due to interlayer coupling, expressed as:

$$\mathbf{E}=-J_{1}\cos(\Delta\phi)$$
(2)

$\Delta\phi$   is the angle between the magnetizations of coupled layers and    $J_{1}$   is the coupling strength. The FEM implementation in our framework leverages the MFEM library [20], facilitating the integration of these complex interactions within the simulation environment [21], [22]. This approach ensures a nuanced understanding of the magnetic interactions at play, particularly at the interfaces where the IEC manifests as detailed in [23].

TABLE I S IMULATION  P ARAMETERS .

|LLG parameters|StackA|Stack B|
|---|---|---|
| Saturation magnetization (Ms,|0.73 × 106 A/m|0.85 × 106 A/m|
|HI)|||
|         Saturation magnetization (Ms,                RI)      |1.1 × 106 A/m|0.8 × 106 A/m|
|||1.1 x 106 A/m|
|         Saturation magnetization (Ms,                PI）      |||
|Saturation magnetization (Ms,|1.1 × 106 A/m|1.1 × 106 A/m|
|FI）|1.1 × 106 A/m||
|Exchange constant (Aezc, HL)|1.0 × 10-11 J/m|1.0 × 10-11 J/m|
|Exchange constant (Aezc, RL)|2.0 × 10-11 J/m|        1.0 × 10-11 J/m                2.0 × 10-11 J/m      |
|Exchange constant (Aexc, PL)|||
|Exchange constant (Aexc, FL)|2.0 × 10-11 J/m|2.0 × 10-11 J/m|
|Shape anisotropy (Ku, HL)|7.843 × 105 J/m3|7.843 × 105 J/m3|
|Shape anisotropy (Ku, RL)|8.501 × 105 J/m3|8.318 × 105 J/m3|
|Shape anisotropy (Ku, PL)||9.974 × 105 J/m3|
|Shape anisotropy (Ku, FL)|9.261 × 105 J/m3|9.261 × 105 J/m3|
|Gilbert damping (Q, HL)|0.02|        0.02              |
|Gilbert damping (o, RL)|0.01|0.02|
|Gilbert damping (Q, PL)||0.015|
|Gilbert damping (α, FL)|0.005|0.01|
|IEC (Jiec, Ru)|-1.32 mJ/m2|-1.5 mJ/m2|
|        IEC (Jiec, Ta)                 Resistance parallel (Rp)      ||0.8 mJ/m2|
||1.68 k2|1.68 kΩ2|
|Resistance parallel (RAP)|4.22k2|4.22k|


## III. R ESULTS 

The following sections report the results of switching simulations performed on the structures depicted in Fig. 1. Due to the capability of computing the torque acting in all layers with a unified expression, the presented FE solver is suitable for the simulation of such structures.

Fig. 3 to Fig. 6 depict the magnetization state from P to AP switching in Stack A and Stack B with different coupling strengths. In Fig. 3 and Fig. 4 the left-hand side illustrates the HL, the RL, and the FL. On the right-hand side the FL is clipped to enhance the visualization of the RL. In Fig. 5 and Fig. 6 the left-hand side illustrates the HL, the RL, the PL, and the FL. On the right-hand side the FL is clipped to enhance the visualization of the PL. Color coding is employed to indicate the magnetization states: red signifies magnetization pointing in the positive    $x$  -direction, while blue indicates the negative  $x$  -direction.

## A. Stack A 

The structure depicted in Fig. 1(a) comprises a CoFeB RL which is antiferromagnetic (AFM) coupled to a CoPt HL [14]. Fig.2(a) shows the magnetization switching from P to AP under a bias of  2V . The magnetization set at    $m_{x}=1$   reflects the average orientation of both the RL and the FL, pointing positively along the    $x$  -axis. With a strong AFM coupling of  $\mathrm{\dot{-}1.32\;\dot{m}J/m^{2}}$    [14], our findings deviated from the anticipated back-hopping behavior, stabilizing at an equilibrium magnetization state of    $m_{x}=0$  , or an AP configuration between the RL and the FL. On the other hand, a weaker AFM coupling of

![1 . 0 Cap  (a) 0_5  0 . 5 x 0 0_0  . 0 Magnetization m − -0_5  0 . 5  Jiec=-1.32mJ/m²  J iec  =  − 1 . 32mJ/m ² Jiec=-0.5mJ/m2  J iec  =  − 0 . 5mJ/m ² − 1 . 0 1 . 0 CDJ  (b) 0. 5  0 . 5 0_0  0 . 0 − 0_5  0 . 5  Jiec/Ta = 0.8mJ/m2  J iec/Ta  = 0 . 8mJ/m ² Jiec/Ta = 0.2mJ/m2  J iec/Ta  = 0 . 2mJ/m ² − 1 . 0 0 . 0  0.2  0 . 2  0.4  0 . 4  Q.6  0 . 6  0 . 8  1 . 0  1 1.2  . 2  1.  1 . 4  1 16  . 6 Time ns  Time [ns] ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/00bad7d8-b340-4025-a768-1cfdd01293dd/00bad7d8-b340-4025-a768-1cfdd01293dd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215785%3B1743219385&q-key-time=1743215785%3B1743219385&q-header-list=host&q-url-param-list=&q-signature=18067adede8bff97205c66d638e44e3cad0a91bf)
Fig. 2. Magnetization trajectories for P to AP switching, labeled as (a) Stack A and (b) Stack B.

$-0.5\ \mathrm{mJ/m^{2}}$    resulted in partial back-hopping within the RL, impeded by the emergence of domain walls in both the FL and the RL. This partial reversal is attributed to the insufficiency of the applied bias to completely reverse the magnetization in the RL. Fig.3 captures key phases of the switching process from P to AP under a strong AFM coupling of    $-1.32\mathrm{mJ/m^{2}}$  . The snapshots on the left primarily illustrate the FL, while those on the right are clipped to better depict the underlying RL. Fig.3(a) shows the initial magnetization state with the HL aligned in the negative    $x$  -direction and both the RL and the FL in the positive    $x$  -direction. At approximately  0 . 4ns , Fig.3(b) clearly demonstrates that only the FL is reversing, with the RL remaining stable due to the strong AFM coupling. Around  1ns , Fig.3(c) confirms the successful switch from P to AP, with no back-hopping in the RL. However, in Fig.4, we illustrate the magnetization reversal under a weaker coupling of  $-0.5\;\mathrm{mJ/m^{2}}$  . In Fig.4(a), the RL begins reversing around  0 . 4ns  as shown in Fig.4(b) right-hand side, due to the weaker AFM coupling between the HL and the RL. After approximately  1ns , Fig. 4(c) shows almost complete reversal of the RL’s magnetization.

## B. Stack B 

![(a) CaD  CD  (b) (c) CCD  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b48135ee-d7c3-4433-9f02-f920fac346ae/b48135ee-d7c3-4433-9f02-f920fac346ae.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215785%3B1743219385&q-key-time=1743215785%3B1743219385&q-header-list=host&q-url-param-list=&q-signature=7060417dc3b6a153523a66b1c5dcba27bf50130f)
Fig. 3. Magnetization state from P to AP switching in Stack A with an AFM of    $\mathrm{\tilde{-}1.32~\mathrm{\mum}J/\mathrm{m}^{2}}$    is depicted.

Similar to StackA, the inclusion of a synthetic antiferromagnetic (SAF) layer accompanied by a PL in this structure aims to enhance spin polarization. As depicted in Fig.1(b), the configuration consists of a CoPt RL AFM linked to a CoPt HL via a Ru NMS. Additionally, a CoFeB PL is connected to the RL through FM coupling facilitated by a Ta NMS. The AFM coupling mediated by a Ru NMS showcases a notable coupling of    $-1.5\ \mathrm{mJ/m^{2}}$  , indicating a strong AFM connection. Initially, the FM connection via a Ta NMS was estimated by Devolder  et al.  [15] at    $0.8~\mathrm{mJ/m^{2}}$  , a substantial

![(a) CaD  CD  (b) (c) CC  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/78882429-d70f-4240-9096-52fb0d58ee40/78882429-d70f-4240-9096-52fb0d58ee40.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215785%3B1743219385&q-key-time=1743215785%3B1743219385&q-header-list=host&q-url-param-list=&q-signature=579e2b813c2342a5912c23b6a00321757d165a58)
Fig. 4. Magnetization state from P to AP switching in Stack A with an AFM of    $\mathrm{-0.5\mJ/m^{2}}$    is depicted.

FM coupling. However, subsequent studies by Devolder  et al. [24] and Goff  et al.  [25] revised this strength to  $0.21~\mathrm{mJ/m^{2}}$  , marking it as weaker than initially anticipated.

Fig.2(b) illustrates the transition from P to AP magnetization under a bias of  2V . The initial magnetization, set at    $m_{x}\,=\,1$  , reflects the average magnetization direction of both the PL and the FL, positively oriented along the  x - axis. With the initial stronger FM coupling, the absence of back-hopping suggests that the coupling is robust enough to prevent magnetization reversal in the PL. However, under the later proposed weaker FM coupling strength, the PLs alignment with the RL is compromised, leading to a notable magnetization reversal.

Fig.5 captures crucial stages of the switching process from P to AP under a strong FM coupling of    $0.8\mathrm{mJ/m^{2}}$  . The lefthand side snapshots primarily feature the FL, while the right

![caD  (a) (b) CC  (c) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3060b5ee-2c85-4222-8459-1712448e048b/3060b5ee-2c85-4222-8459-1712448e048b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215785%3B1743219385&q-key-time=1743215785%3B1743219385&q-header-list=host&q-url-param-list=&q-signature=a128d941dff9db27be32bb0fd5e6e84964da2c77)
Fig. 5. Magnetization state from P to AP switching in Stack B with an FM of    $\mathrm{{\bar{0.8}}\ m J/\mathrm{{m}^{2}}}$    is depicted.

![caD  (a) (b) CCD  (c) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4a05f382-79eb-4034-b2c4-2e66a3e820f1/4a05f382-79eb-4034-b2c4-2e66a3e820f1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215785%3B1743219385&q-key-time=1743215785%3B1743219385&q-header-list=host&q-url-param-list=&q-signature=8453ac578fd775e1780c155438151f11c896d422)
Fig. 6. Magnetization state from P to AP switching in Stack B with an FM of    $\mathrm{{\bar{0}}.2\ m J/\mathrm{{m}^{2}}}$    is depicted.

## IV. C ONCLUSION 

We discuss the impact of coupling strengths on magnetization behavior within synthetic antiferromagnetic layer structures under various coupling conditions. We specifically investigate the effects of AFM and FM coupling strengths on magnetization behavior during the switching from P to AP configurations under applied biases. The investigations focus on a structure consisting of a CoFeB RL AFM coupled to a CoPt HL, which is chosen to examine the phenomenon of back-hopping, as previously discussed in related research. These findings highlight that a strong AFM coupling significantly stabilizes the magnetization, preventing back-hopping and achieving a stable AP configuration between the RL and the FL.

Furthermore, the configuration featuring a SAF layer with a PL aims to enhance spin polarization through specific AFM and FM coupling arrangements. Strong AFM links facilitated by a Ru NMS and initial substantial FM coupling via Ta NMS were analyzed. It was observed that robust coupling strengths maintain the intended magnetization orientation, while weaker coupling strengths, as revised in later studies, allow magnetization reversals, affecting the stability of the intended magnetic configurations.

The strength and nature of the magnetic coupling in antiferromagnetic structures play a crucial role in influencing the magnetization dynamics and stability, which is fundamental for optimizing performance in spintronic devices. Valuable insights into the design and functional adjustments necessary for enhancing device reliability and efficiency in practical applications is discussed, underscoring the critical interplay between magnetic coupling and device performance. These observations are pivotal for devising strategies to improve the operational characteristics of spintronic technologies.

## A CKNOWLEDGMENT 

The financial support by the Federal Ministry of Labour and Economy, the National Foundation for Research, Technology and Development, and the Christian Doppler Research Association is gratefully acknowledged.

hand side is trimmed to enhance the visualization of the PL beneath. Fig.5(a) displays the initial magnetization state with the HL aligned in the negative  $x$  -direction and the RL, the PL, and the FL in the positive  $x$  -direction. At approximately  0 . 4ns , Fig.5(b), shows that only the FL is undergoing magnetization reversal, with the PL remaining stable due to the strong FM coupling. Approximately at  1ns , Fig.5(c) confirms the successful transition from P to AP, with no back-hopping observed in the PL. Conversely, in Fig.6, the magnetization reversal process under a weaker FM coupling of    $0.2\ \mathrm{mJ/m^{2}}$  is depicted. The PL beginning to reverse around  0 . 4ns , as demonstrated in Fig.6(b) on the right-hand side, due to the weaker FM coupling between the RL and the PL. By about 1ns , Fig. 6(c) displays the almost complete reversal of the PLs magnetization.

## R EFERENCES 

[1] S. Jung, H. Lee, S. Myung, H. Kim, S. K. Yoon  et al. , “A Crossbar Array of Magnetoresistive Memory Devices for In-Memory Computing,” in Nature , vol. 601, 2022, pp. 211–216.   [2] V. B. Naik, K. Yamane, T. Lee, J. Kwon, R. Chao  et al. , “JEDECQualified Highly Reliable 22nm FD-SOI Embedded MRAM For Low-Power Industrial-Grade, and Extended Performance Towards Automotive-Grade-1 Applications,” in  IEEE International Electron Devices Meeting (IEDM) , 2020, pp. 11.3.1–11.3.4.   [3] S. Ikegawa, K. Nagel, F. B. Mancoff, S. M. Alam, M. Arora  et al. , “HighSpeed (400MB/s) and Low-BER STT-MRAM Technology for Industrial Applications,” in  IEEE International Electron Devices Meeting (IEDM) , 2022, pp. 10.4.1–10.4.4.   [4] J. A. Smith and E. B. Doe, “Advancements in Nonvolatile Memory Technologies: The Role of STT-MRAM,”  Journal of Memory Systems , vol. 15, no. 2, pp. 134–145, 2023.   [5] L. M. Johnson and A. N. Roberts, “Magnetic Tunnel Junctions: The Backbone of STT-MRAM,”  Advanced Materials Technology , vol. 29, no. 4, pp. 560–572, 2022.   [6] H. O. Lee and Y. J. Kim, “Challenges in Miniaturization of STT-MRAM Devices,”  NanoTech Review , vol. 12, no. 1, pp. 88–97, 2024.   [7] C. Abert, H. Sepehri-Amin, F. Bruckner, C. Vogler, M. Hayashi, and D. Suess, “Back-Hopping in Spin-Transfer-Torque Devices: Possible Origin and Countermeasures,”  Phys. Rev. Appl. , vol. 9, 2018.   [8] S. K. Patel and F. H. Wong, “Interlayer Exchange Coupling in Magnetic Tunnel Junctions: Implications for Memory Stability,”  Journal of Spintronics and Magnetic Nanotechnology , vol. 8, no. 3, pp. 201–210, 2023.   [9] M. T. Garcia and D. R. Lopez, “Metallic Spacers in Spintronic Devices: A Review,”  Spintronics Research Letters , vol. 10, no. 2, pp. 154–163, 2024.   [10] H. Sato, M. Yamanouchi, S. Ikeda, S. Fukami, F. Matsukura, and H. Ohno, “MgO/CoFeB/Ta/CoFeB/MgO Recording Structure in Magnetic Tunnel Junctions With Perpendicular Easy Axis,” in  IEEE Transactions on Magnetics (TMAG) , vol. 49, 2013, pp. 4437–4440.   [11] B. Jinnai, J. Igarashi, K. Watanabe, T. Funatsu, H. Sato  et al. , “HighPerformance Shape-Anisotropy Magnetic Tunnel Junctions down to 2.3 nm,” in  IEEE International Electron Devices Meeting (IEDM) , 2020, pp. 24.6.1–24.6.4.   [12] Y. Zhang and X. L. Wang, “Enhancing Interfacial Anisotropy in Magnetic Tunnel Junctions for STT-MRAM Applications,”  Materials Science and Engineering R: Reports , vol. 141, pp. 58–69, 2022.   [13] S. Ikeda, K. Miura, H. Yamamoto, K. Mizunuma, H. D. Gan  et al. , “A Perpendicular-Anisotropy CoFeB–MgO Magnetic Tunnel Junction,” in Nature Materials , vol. 9, 2010, p. 721–724.   [14] S. Bin Hamid, R. Dutta, O. Hassan, and M. Z. Baten, “Implementing Bidirectional Logic with Backhopping in Magnetic Tunnel Junctions,” AIP Advances , vol. 14, no. 2, p. 025224, 02 2024. [Online]. Available: https://doi.org/10.1063/5.0169751   [15] T. Devolder, J.-V. Kim, F. Garcia-Sanchez, J. Swerts, W. Kim, S. Couet, G. Kar, and A. Furnemont, “Time-resolved spin-torque switching in mgo-based perpendicularly magnetized tunnel junctions,” Phys. Rev. B , vol. 93, p. 024420, Jan 2016. [Online]. Available: https://link.aps.org/doi/10.1103/PhysRevB.93.024420   [16] S.  Lepadatu,  “Boris  Computational  Spintronics  Online  Materials Database,”  http://www.boris-spintronics.uk/online-materials-database/, Accessed: 24.03.2024.   [17] B. Khodadadi, J. B. Mohammadi, J. M. Jones, A. Srivastava, C. Mewes, T. Mewes, and C. Kaiser, “Interlayer Exchange Coupling in Asymmetric  Co − Fe / Ru / Co − Fe  Trilayers Investigated with Broadband Temperature-Dependent Ferromagnetic Resonance,”  Phys. Rev. Appl. , vol. 8, p. 014024, Jul 2017.   [18] A. Mouhoub, F. Millo, C. Chappert, J.-V. Kim, J. L´etang, A. Solignac, and T. Devolder, “Exchange Energies in CoFeB/Ru/CoFeB Synthetic Antiferromagnets,”  Phys. Rev. Mater. , vol. 7, p. 044404, Apr 2023.   [19] T. Katayama, S. Yuasa, J. Velev, M. Y. Zhuravlev, S. S. Jaswal, and E. Y. Tsymbal, “Interlayer Exchange Coupling in Fe/MgO/Fe Magnetic Tunnel Junctions,”  Applied Physics Letters , vol. 89, no. 11, p. 112503, 09 2006.   [20] T. Kolev and V. Dobrev, “MFEM: Modular Finite Element Methods Library,” http://mfem.org, Accessed: 24.03.2024.   [21] S. Fiorentini, N. P. Jørstad, J. Ender, R. L. de Orio, S. Selberherr, M. Bendra, W. Goes, and V. Sverdlov, “Finite Element Approach for the Simulation of Modern MRAM Devices,” in  Micromachines , vol. 14, 2023.   [22] ViennaSpinMag, “An Open Access Finite Element-based Application for Calculating the Magnetization Dynamics of Multi-Layered Structures Composed of Ferromagnets, Metal Spacers and Tunnel Barriers.” https: //www.iue.tuwien.ac.at/viennaspinmag/, Accessed: 24.03.2024.   [23] M. Bendra, R. de Orio, S. Selberherr, W. Goes, and V. Sverdlov, “Advanced Modeling and Simulation of Multi-Layered Spin-Transfer Torque Magnetoresistive Random Access Memory with Interface Exchange Coupling,”  Micromachines , 2024, Under Review.   [24] T. Devolder, O. Bultynck, P. Bouquin, V. D. Nguyen, S. Rao, D. Wan, B. Sor´ee, I. P. Radu, G. S. Kar, and S. Couet, “Back hopping in spin transfer torque switching of perpendicularly magnetized tunnel junctions,”  Phys. Rev. B , vol. 102, p. 184406, Nov 2020. [Online]. Available: https://link.aps.org/doi/10.1103/PhysRevB.102.184406   [25] A. Le Goff, K. Garcia, N. Vernier, T. Tahmasebi, S. Cornelissen, T. Min, and T. Devolder, “Effect of ta insertion in reference layers of mtjs with perpendicular anisotropy,”  IEEE Transactions on Magnetics , vol. 50, no. 11, pp. 1–4, 2014.

