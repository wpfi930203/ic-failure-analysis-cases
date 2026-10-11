---
title: "☆Milton Ohring, Lucian Kasprzak-Reliability and Failure of Electronic Materials and Devices, Second Edition-Academic Press (2014).pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_b4d2e23a12e26fec4a6d177d2860d5b07295230462135641
file_size: 74067355
---

Without Chapter 4 on the mathematics of reliability it is doubtful that the book title could include the word reliability. Historically, reliability has been inextricably intertwined with statistics and probability theory. Even today a large segment of the reliability literature bears a strong hereditary relationship to these mathematical and philosophical antecedents. Nevertheless, “The failure of devices occurs due to natural laws of change, not to the ﬁnger of fate landing at random on one of group of devices and commanding fail“ (R.G. Stewart, IEEE Transactions on Reliability, R-15,No. 3, 95 (1966)). In a less charitable vein, R.A. Evans has pointed out that probability and statistical inference help us “quantify our ignorance” of failure mechanisms. Uncovering truth should be the objective instead. That is why the primary focus of the book and most of its contents deal with the physics of failure as refracted through the lenses of physical and materials science. With this understanding, our treatment of reliability mathematics is largely limited to the elementary statistical handling of failure data and the simple implications that ﬂow from such analyses. Nevertheless, reliability mathematics permeates the book since failure data are normally presented in these terms.


The midsection of the book spanning Chapters 5 through 10 is devoted to a treatment of the speciﬁc ways materials and devices degrade and fail both on the chip and packaging levels. Failure mechanisms discussed and modeled include those due to mass and electron transport, environmental and corrosion degradation, mechanical stress, and optical as well as nuclear radiation damage. Most failures occurring within interconnections, dielectrics and insulation, contacts, semiconductor junctions, solders, and packaging materials can be sorted into one of these categories. Grouping according to operative failure mechanism, rather than speciﬁc device,material, or circuit element, underscores the fundamental generic approach taken.


Important practical concerns regarding characterizing electronic materials and devices in the laboratory, in order to expose defects and elucidate failure mechanisms, is the subject of Chapter 11. Finally, the last chapter speculates about the future through a discussion of device-shrinkage trends and limits and their reliability implications.


Due to continual and rapid advances in semiconductor technology, the shelf life of any particular product is very short, thus raising the question of


xx Preface to the First Edition


how to convey information that may be quickly outdated. Because concepts are more powerful than facts, I have tried to stress fundamentals and a physical approach that may have applicability to new generations of devices.


Within this approach the dilemma arose whether to emphasize breadth or depth of subject matter. Breadth is a sensible direction for an audience having varied academic backgrounds desirous of a comprehensive but qualitative treatment; on the other hand, depth is necessary to enable practitioners to confront speciﬁc challenges within the evolving electronics industries. As a compromise I have attempted to present a balanced treatment incorporating both attributes and sincerely hope neither audience will be disappointed by the outcome. Nevertheless, space limitations often preclude development of a given subject from its most elementary foundations.


I assume readers of this book are familiar with introductory aspects of electronic materials and possess a cultural knowledge of such subjects as modern physics, thermodynamics, mass transport, solid mechanics, and statistics. If not, the tutorial treatment of subject matter hopefully will ease your understanding of these subjects. Questions and problems have been included at the end of each chapter in an attempt to create a true textbook.


If this book contributes to popularizing this neglected subject and facilitates the assimilation of willing as well as unconvinced converts into the ﬁeld of reliability, it will have succeeded in its purpose.


M. Ohring


Preface to the First Edition xxi


ACKNOWLEDGMENTS


The idea for this book germinated in the classroom of Bell Laboratories,both at AT&T and Lucent Technologies, where I taught and organized several courses on reliability and failure of electronics over the past decade.


Distilling the essence of the vast scattered information on this subject, ﬁrst for course purposes and then into the text and ﬁgures that have emerged between these covers, would not have been possible without the resources of Bell Labs and the generous assistance of some very special people. Of these, two of my dear friends, Lucian (Lou) Kasprzak and Frank Nash, must be acknowledged ﬁrst. Lou, an early observer of transistor hot-electron effects at IBM, is a member of the board of directors of the IEEE International Reliability Physics Symposia, while Frank, an expert in laser reliability at Bell Labs, wrote the incisive book, Estimating Device Reliability:Assessment of Credibility, Kluwer Academic publishers, (1993). Both stimulated my thinking on the direction of the book and helped me to acquire the research literature that was indispensable to its writing.


Importantly, they dispelled some of my naïveté about reliability and helped me to fashion a credible philosophy of the subject, something acquired only after lengthy grappling with the issues.


Students enrolled in courses for which books are simultaneously being written often leave their imprint on them. This is true of several of the students in the Stevens Institute–Bell Laboratories on-premises graduate program. Therefore, I want to thank both Gary Steiner and Jeff Murdock for critiquing various versions of the text. Gary additionally reviewed the exercises and enhanced the quality of several ﬁgures; Jeff assured me that the text was “Murdock-proof.” Other students who tangibly contributed to the book are Ken Jola, Jim Bitetto, Ron Ernst, and Jim Reinhart.


Ephraim Suhir, Walter Brown, Matt Marcus, Alan English, King Tai,Sho Nakahara, George Chu, Reggie Farrow, Clyde Bethea, and Dave Barr,all of Bell Laboratories and Bob Rosenberg of IBM deserve thanks for their encouragement, helpful discussions, and publications. Despite their efforts I am solely responsible for any residual errors and holes in my understanding of the subject.


I am also grateful to the ever-helpful Nick Ciampa of Bell Laboratories for his technical assistance during the preparation of this book and generosity over the years. For help at important times I wish to acknowledge


xxiii


# Acknowledgments


Pat Downes and Krisda Siangchaew. Lastly, thanks are owed to Zvi Ruder for supporting this project at Academic Press and to Linda Hamilton and Julie Champagne for successfully guiding it through the process of publication.


My dear wife, Ahrona, has once again survived the birth of a book in the family, this time during a joyous period when our three grandchildren,Jake, Max, and Geffen, were born. She and they were unfailing sources of inspiration.


xxiv Acknowledgments


CHAPTER 1


An Overview of Electronic Devices and Their Reliability


1.1 ELECTRONIC PRODUCTS


1.1.1 Historical Perspective


Never in human existence have scientiﬁc and technological advances transformed our lives more profoundly, and in so short a time, as during what may be broadly termed the Age of Electricity and Electronics.1 From the telegraph in 1837 (which was in a sense digital, although clearly electromechanical) to the telephone and teletype, television and the personal computer, the cell phone and the digital camera, and the World Wide Web(WWW), the progress has been truly breathtaking. All these technologies have been focused on communicating information at ever increasing speeds. In contrast to the millennia-long metal ages of antiquity, this age is only little more than a century old. Instead of showing signs of abatement,there is every evidence that its pace of progress is accelerating. In both a practical and theoretical sense, a case can be made for dating the origin of this age to the eighth decade of the nineteenth century [1]. The legacy of tinkering with voltaic cells, electromagnets, and heating elements culminated in the inventions of the telephone in 1876 by Alexander Graham Bell, and the incandescent light bulb 3 years later by Thomas Alva Edison.


Despite the fact that James Clerk Maxwell published his monumental work Treatise on Electricity and Magnetism in 1873, the inventors probably did not know of its existence. With little in the way of “science” to guide them, innovation came from wonderfully creative and persistent individuals who incrementally improved devices to the point of useful and reliable function. This was the case with the telephone and incandescent lamp,perhaps the two products that had the greatest inﬂuence in launching the widespread use of electricity. After darkness was illuminated and


1 Electricity means those advances capitalizing on electromagnetics and electromechanics, e.g., generators and motors. In contrast, Electronics relates to the broad range of devices, e.g., vacuum tubes and transistors, which function by controlling the ﬂow of electrical charges in a vacuum, gas, solid,


liquid, or plasma.


Reliability and Failure of Electronic Materials and Devices


ISBN 978-0-12-088574-9


http://dx.doi.org/10.1016/B978-0-12-088574-9.00001-X


© 2015 Elsevier Inc.


All rights reserved. 1


# 1 . An Overview of Electronic Devices and Their Reliability


## 1.1 Electronic Products


### 1.1.1 Historical Perspective


communication over distance demonstrated, the pressing need for electric generators and systems to distribute electricity was apparent. Once this infrastructure was in place, other inventions and products capitalizing on electromagnetic-mechanical phenomena quickly followed. Today, texting from a cell phone has replaced the telegraph for the ultimate person-toperson real-time digital conversation. Literally, the telegraph of 1837 has become texting in 2007. Both use letters to interact with someone on the other end (of the wire, so to speak). The rate is about the same, possibly a letter or so a second, when you consider composition for texting, which is real time versus predeﬁned on a form for the telegraph. Both the telegraph


(1837) and texting (2007) have roughly the same data entry rate of about two letters a second.


Irrespective of the particular invention, however, materials played a critical role. At ﬁrst, conducting metals and insulating nonmetals were the only materials required. Although a reasonable number of metals and insulators were potentially available, few were produced in quantity or had the requisite properties. The incandescent lamp is a case in point [2,3]. In the 40 years prior to 1879, some 20 inventors tried assorted ﬁlaments (e.g.,carbon, platinum, iridium) in various atmospheres (e.g., vacuum, air, nitrogen, hydrocarbon). Frustrating trials with carbon spirals and ﬁlaments composed of carbonized ﬁber, tar, lampblack, paper, ﬁsh line, cotton, and assorted woods paved the way to Edison’s crowning achievement. His patent revealed that the ﬁlament that worked was carbonized cardboard bent in the shape of a horseshoe. Despite the fact that an industry based on incandescent lamps grew rapidly, the ﬁlaments were brittle and hard to handle. The glass envelopes darkened rapidly with time, and the bulbs were short lived. Salvation occurred around 1910 when the Coolidge process [4]for making ﬁne tungsten ﬁlament wire was developed. Well beyond a century after the original Edison patent, ﬁlaments continue to be improved and lamp life extended and today we are increasingly using light emitting diodes (LEDs) as the next generation of efﬁcient illumination.


With the ability to generate electromagnetic waves around the turn of the century, the era of vacuum electronics was born. The invention of vacuum tubes enabled electric waves to be generated, transmitted, detected,and ampliﬁed, making wireless communication possible. In particular, the three-electrode vacuum tube invented by Lee de Forest in 1906 became the foundation of electronics for the ﬁrst half of the twentieth century [5].


Throughout the second half of the twentieth century, electronics has been transformed both by the transistor, which was invented in 1947, and


integrated circuits (ICs), which appeared a decade later. The juxtaposition of these milestone devices in Figure 1.1 demonstrates how far we have come in so short a time.


A pattern can be discerned in the development of not only electrical devices and equipment, but also all types of products. First, the genius of invention envisions a practical use for a particular physical phenomenon.


The design and analysis of the components and devices are then executed,and ﬁnally, the materials and manufacturing processes are selected. Usage invariably exposes defects in design and manufacturing, causing failure or the wearing out of the product. Subsequent iterations of design or materials processing improve the reliability or probability of operating the product for a given time period under speciﬁed conditions without failure. In a sense, new reliability issues replace old ones, but incremental progress is


Figure 1.1 Edison’s horseshoe ﬁlament lamp sketched by patent draftsman Samuel D.


Mott serves as the backdrop to the vacuum tube, discrete transistor, and integrated circuit. Courtesy of FSI International, Inc.


An Overview of Electronic Devices and Their Reliability 3


made. Ultimately, new technologies replace obsolete ones, and the above sequence of events repeats once again.


Well into the Age of Electricity and Electronics, we still use vastly improved versions of some of those early inventions. As you change your next light bulb, however, you will realize that reliability concerns are still an issue. But solid-state electronic products also fail in service, and often with far greater consequences than a burned-out light bulb. While other books are concerned with the theory of phenomena and the practice of designing useful electrical and electronic products based on them, this book focuses on the largely unheralded activities that insure they possess adequate reliability during use.


1.1.2 Solid-State Devices


The scientiﬁc ﬂowering of solid-state device electronics has been due to the synergism between the quantum theory of matter and classical electromagnetic theory. As a result, our scientiﬁc understanding of the behavior of electronic, magnetic, and optical materials has dramatically increased. In ways that continue undiminished to the present day, exploitation of these solid-state devices, particularly semiconductors, has revolutionized virtually every activity of mankind, e.g., manufacturing, communications, the practice of medicine, transportation, and entertainment [6].


Before focusing on electronics, it is worth noting parallel developments in the ﬁeld of photonics. The latter has been deﬁned as “the technology for generating, amplifying, detecting, guiding, modulating, or modifying by nonlinear effects, optical radiation, and applying it from energy generation to communication and information processing” [7]. Building on the theoretical base laid by Maxwell, Planck, and Einstein, optoelectronics (or electro-optics) applications include lasers, ﬁber optics, integrated optics,acousto-optics, nonlinear optics, and optical data storage. Destined to merit an historic age of its own, photonics is projected to dominate applications,as fundamental physical limits to electronic function are reached for example compact disks (CDs) and digital video disks (DVDs).


As already noted, two major revolutions in electronics occurred during the time from the late 1940s to the 1970s. In the ﬁrst, transistors replaced vacuum tubes. These new solid-state devices, which consumed tens of milliwatts and operated at a few volts, eliminated the need for several watts of ﬁlament heater power and hundreds of volts on the tube anode. The second advance, the invention of the IC in 1958, ushered in multidevice chips to replace discrete solid-state diodes and transistors and electronic


### 1.1.2 Solid-State Devices


circuits. Early solid-state devices were not appreciably more reliable than their vacuum tube predecessors, but power and weight savings were impressive. While discrete devices were advantageously deployed in a wide variety of traditional electronics applications, information processing required far greater densities of transistors. This need was satisﬁed by ICs. Is it possible that the productivity gains fueling our gross domestic product are really the ﬂowering of ICs and computers on the WWW?


1.1.3 Integrated Circuits


1.1.3.1 Applications


Starting in the early 1960s, the IC market was based primarily on bipolar transistors. Since the mid-1970s, however, ICs composed of metal-oxidesilicon (MOS) ﬁeld effect transistors prevailed because they possessed the advantages of device miniaturization, high yield, and low power dissipation.


(Both bipolar and MOS transistors will be discussed in Chapter 2.) Then in successive waves, IC generations based on MOS transistors arose, ﬂowered,and were superseded by small-scale integration, medium-scale integration,large-scale integration, very-large-scale integration, ultra-large-scale integration (ULSI), and extreme large-scale integration. The latter, consisting of more than 1010 devices per chip, provides an entire system on a chip. In the early 1970s, sales of ICs reached $1 109; today, digital MOS ICs domi-nate a market worth 1012 dollars a year; likewise, the broader market for electronic equipment exceeds a 1014 dollars.


ICs are pervasive in computers, consumer goods, and communications,where the total demand for each is roughly the same. Worldwide IC revenues are currently about 30% in these three sectors, with an additional 9% accounted for by industry and 2% by the military [7]. The role of the computer industry and defense electronics as driving forces for IC production has been well documented. Less appreciated is the generally equal and at times even more powerful stimulus provided by consumer electronics in fostering the IC revolution.


Consumer products are those purchased by the individual or a family unit. Cell phones, digital cameras, iPods, wireless everything, webcams,Global Positioning System devices, high-deﬁnition televisions (HD TVs),home theater systems, DVD recorders, wristwatches, computers, LCDs,cordless phones, smoke detectors, and automobiles are examples that contain ICs. The automobile is an interesting case in point. There are presently more than 25 microprocessor IC chips in every car, subject to a very hostile environment, to control engine ignition timing, gas–air mixtures, idle speed,


An Overview of Electronic Devices and Their Reliability 5


### 1.1.3 Integrated Circuits


#### 1.1.3.1 Applications


and emissions, as well as chassis suspension, antiskid brakes, and four-wheel steering. Furthermore, recent trends have made vehicles intelligent through special application-speciﬁc ICs that provide computerized navigation and guidance assistance on highways, self parking, and electronic map displays.


In the near future, cars will be remotely controlled by satellite from home to your destination. Advances in one sector of applications ripple through others. Thus, video phones and conferencing, multimedia computers, threedimensional movies, and digital HD TV have permeated the consumer marketplace.


The Bell Labs News issue of February 7, 1997, marking the 50-year anniversary of the invention of the transistor, roughly estimated that“there are some 200 million billion transistors in the world todaydabout 40 million for every woman, man, and child.” In the United States alone,more than 200 ICs are used per household. The transistor count is rapidly swelling as the standard of living rises in China and India. With some 5 109 humans on earth, there is much room for continued expansion ofIC consumption in Third World countries. What is remarkable is how inexpensive the fruits of this technology have become. In the 1950s, the cost of a transistor dropped from $45 to $2. Today’s transistors cost less than a hundred-thousandth of a cent each!


1.1.3.2 Trends


Meeting the needs of burgeoning markets for digital electronic products has necessitated a corresponding growth in the number of transistors and complexity of the ICs that house them. To gain a perspective of IC chip progress made in the 37 years from their inception to 1994, the time span analyzed, consider the following measures of advance [8]:


1. Minimum feature size (F) has decreased by a factor of 50.


2. Die area (D2) has increased by a factor of approximately 170.


3. Packing efﬁciency (PE), deﬁned as the number of transistors per minimum feature area, has multiplied by over 100.


The composite number of transistors per chip N is the product of these three terms, or N¼ F2D2 PE. Substitution indicates a staggeringincrease by a factor of close to 5 107, a number that is manifest in Moore’slaw. In the mid-1970s, Gordon Moore, a founder of Intel, observed an annual doubling of the transistors per IC chip, which held true for about 15 years until about 1990, and a reduction in the rate of increase to 1.5 per year since then. By the end of the twentieth century, a staggering one billion devices per chip was realized, and by 2020, the count will be close to


#### 1.1.3.2 Trends


a trillion. Moore probably overstated the initial progress made, which is,nevertheless, extraordinarily impressive. In view of the fact that the price of chips has not changed appreciably, while their reliability has considerably improved over this time, these phenomenal advances are unprecedented in technological history.


Both microprocessor and memory chips are the indispensable drivers of computer technology. Microprocessor ICs perform the numerous logic functions in circuits, while memory chips essentially store the information generated. Trends showing rapidly increasing transistor numbers in IC chips are presented in Figure 1.2(a) for processor and memory chips. Kurzweil has expanded Moore’s law as seen in Figure 1.2(b), where progress is plotted as a cost of calculation for the entire twentieth century. When coupled with


1.00E+02


1.00E+03


1.00E+04


1.00E+05


1.00E+06


Transistors, Bits


1.00E+07


1.00E+08


1.00E+09


1.00E+10


1.00E+11


1960


1970


1980


1990


2000


2010


Year


Memory Size Trend


(a)


|||||Intel |
|---|---|---|---|---|

|||||■AMD|

|||||AMD |

|||||IBM |

|||||●Memory Size|

|||Processor |and Memory |and Memory |

Figure 1.2 (a) Plot of the time-dependent increase in number of transistors on microprocessor and memory integrated circuit chips. (b) Kurzweil expansion of Moore’s lawdFifth Paradigm, see Moore’s Law in Wikipedia on the Internet.


An Overview of Electronic Devices and Their Reliability 7


the far slower growth in chip size over the years (Figure 1.3), one can begin to appreciate the huge growth in device density and the magnitude of feature (linewidth, Figure 1.4(a)) shrinkage required to make it possible.


Increasing the transistor count improves microprocessor performance as gauged by the number of instructions executed per second. Measured in frequency of operation, Figure 1.4(b) reveals a hundredfold increase in performance every 10 years. However, the key driving parameter, as mentioned above and as shown in Figure 1.4(a), is actually the reduction in linewidth used to fabricate the ICs. We will discuss this parameter in greater detail in Chapter 3, when we deal with processing yield and defects. Also of importance is the increase in hard drive storage capacity achieved in the past quarter century, as shown in Figure 1.4(c), which has improved by ﬁve orders of magnitude. Relying on the same lithography technology, magnetic read/write heads have taken advantage of the reduction in linewidth to create ever smaller heads that ﬂy ever closer to the magnetic disk surface.


It is instructive to quantitatively sketch the time evolution of high-tech consumer electronics in terms of product size. In the past few decades, for


Figure 1.2 (b)dCont'd.


example, the overall volume of mobile communications and personal computers has been reduced by an order of magnitude or more, as shown in Figure 1.5(a) and 1.5(b); corresponding weight savings have also been realized. The latest digital cell phones are less than 100 g, the smallest laptop computers are just about 2 pounds, and digital cameras, at about 4 ounces, have gone from 1 to 10 Mega-pixels in less than a decade(Figure 1.5(c)). It has been estimated that if a digital cell phone contained vacuum tubes instead of transistors, it would be larger than the Washington Monument! This volume reduction is possible because of the increasing power of ICs.


The source of these advances has been our ability to shrink the dimensions of critical device features. As a dramatic example of this, consider the width of aluminum interconnections in the high-device-density IC chips shown in Figure 1.6. The indicated dimensions have shrunk over the years from several microns to 0.35 mm presently. By 2010, conductor linewidths of 0.07 mm are projected. More will be said about shrinkage of


1


Size (sq mm)


10


100


1000


|Chip Size |Chip Size |||||||
|---|---|---|---|---|---|---|---|

|Logic Memory |Logic Memory |||||||

|Logic Memory |Logic Memory |Trend |Trend |||||

1965 1970 1975 1980 1985 1990 1995 2000 2005 2010 Year


Figure 1.3 Plot of the time-dependent increase in chip area of microprocessor and memory circuit chips.


An Overview of Electronic Devices and Their Reliability 9


other device features throughout the book, and trends will be summarized in Chapter 12.


Each increase in packing density introduces a variety of new quality and reliability issues associated with speciﬁc devices, and more importantly, with the rapidly increasing number of contacts, interconnections, and solder joints. Reduced dimensions have made circuits increasingly sensitive to more subtle defects, which had not previously threatened chip reliability.


Confounding physical intuition, IC chip reliability as measured by the number of circuit failures, has, in fact, dramatically increased over the last two decades. As revealed by Figure 1.7, the number of failures in FITs(1 failure in 109 h of service¼ 1 FIT) has been reduced by a factor of 10 in


10 100


Linewidth (nm)


10000


|Linewidth ||||
|---|---|---|---|

|Linewidth ||||

Frequency (MHz)100


1970 1980 1990 2000 2010


Year Chip Speed (MHz)


Frequency


(b)


Figure 1.4 (a) Plot of the time-dependent decrease in lithography linewidth in nanometers. (b) Plot of the time-dependent increase in microprocessor chip speed measured in megahertz. (c) Plot of the increase in hard drive storage capacity.


this same period of time. Shown are the long-term failure rates as well as those that occur shortly after use commences, i.e., infant mortality(see Section 1.3.8). These remarkable reliability trends will probably continue in response to both customer needs and stiff competition, which have aggressively forced manufacturing to reduce the number of defects.


1.1.4 Yield of Electronic Products


Before we can derive the beneﬁts of electronic products, they must ﬁrst be manufactured in satisfactory numbers. Ideally, one might naively hope that after carefully processing a wafer containing a large number of ICs, all would function properly when tested. In reality, however, the number of good, or functional, circuits may range from close to zero for a new technology to almost 100% for a mature technology where the “bugs” have been worked out. The very important term yield refers to the fraction of successful products that survive ﬁnal screening and meet speciﬁcations relative to the total number that started out to be processed or manufactured. Yield is essentially the bottom-line concern of manufacturing technology. In general, yields are never 100% because of some combination


100000


1000000


1985


1995


2005


HD Capacity (GB)


(c)


Figure 1.4dCont'd.


An Overview of Electronic Devices and Their Reliability 11


### 1.1.4 Yield of Electronic Products


Weight (grams)1000


Energy


Limited Energy Systems


toi-V Microsystems


System Size, L+W+H (Inches)00UP


Credit Card


o


Wristwatch


N


Finger Ring


5-7 Years I


Palmtop


台台古台


Notebook


Desktop口


Uira-Low Power


||Cell |Phone Weight |Phone Weight |
|---|---|---|---|

|||Weight ||

1 10


Millions


1996


1998


2002


2004


2006


Consumer Camera Pixels


Pixels


Time


Figure 1.5 (a) Plot of the time-dependent decrease in portable/cell phone weight in grams. (b) Reduction in the dimensions of personal computing systems with time. (From Ref. [9].) (c) Plot of the time-dependent increase in pixels for consumer digital cameras.


of problems associated with circuit design, processing, and random defects.


The ﬁrst may simply be due to errors in circuit design, while the others usually result from lack of process control and contamination. Speciﬁc examples of each will be deferred until Chapter 3.


An excellent way to appreciate the broader factors that inﬂuence yield is through study of Figure 1.8. The ﬁrst important conclusion that can be


Figure 1.6 Shrinkage in the aluminum interconnection linewidth in high device+-1μ


/2μ


-0.07μ


density IC chips. Courtesy of P. Chaudhari, IBM Corp.


4000


0-


00


800


8000口600 F400


0


一300


H


200


60


80


40


30


40 30


20


11111111111111111111111


727680848892962000 YEAR


11110 80


OO


M


300


400


600


Figure 1.7 Long- and early-term failure-rate goals at Intel. The units for long-term failures are FITs, while those for short-term failures are DPMs. (DPM¼ defects permillion). From Ref. [10].


An Overview of Electronic Devices and Their Reliability 13


Line Widths峰


drawn is that yield drops as the chip area increases. Second, for chips of a given area, the highest yields occur for those that have the fewest defects.


Here we note that every new generation of memory and logic chips invariably means an increase in device area. In DRAM memory chips, for example, increasing the capacity to 64 megabit (64 Mb) implies a die size of roughly 2.6 cm2. This means that many fewer defects per unit area can be tolerated if the same yield level is to be achieved in successive generations of product. Simultaneously, the defect that signiﬁes outright die rejection if present, the so-called killer defect, becomes smaller and smaller in size because device features have shrunk in size. What aggravates the problem considerably is that process complexity increases as the device count rises.


One-megabit DRAMs require over 300 process steps, whereas more than 500 steps are necessary for 64-Mb DRAM production. The chance of incorporating defects is thus proportionately raised.


What do defects and yield have to do with reliability? Although yield and reliability have quite different meanings, there is a link between them.


As we have just seen, yield depends on minimizing the presence of defects.


Reliability, an issue that concerns the performance of “yielded” products in service, also depends on defects. The fact that yielded products have passed the last screen does not mean they do not contain potential or latent defects.


Too small to be troublesome initially, the latter may prove fatal under subsequent use involving a stressing regimen that enlarges their size or


Figure 1.8 Yield and defect trends in memory and logic chips as a function of device area. From Intel/Future Horizons as reproduced in Ref. [11].


inﬂuence. Their mutual association with defects implies the logic of connection between yield and reliability.


The subject of yield is addressed again in Chapter 3, where defects, their sources, and how they are statistically modeled are extensively treated. In addition, both theoretical and experimental associations between yield and reliability are discussed.


1.2 RELIABILITY, OTHER “.ILITIES,” AND DEFINITIONS


1.2.1 Reliability


Earlier we deﬁned reliability as the probability of operating a product for a given time period under speciﬁed conditions without failure. Clearly, reliability reﬂects the physical performance of products over time and is taken as a measure of their future dependability and trustworthiness. Each of the above words in italics is signiﬁcant and deserves further commentary.


Under probability, we include the sampling of products for testing, the statistical analysis of failure test results, and the use of distribution functions to describe populations that fail. Even though it is not feasible to predict the lifetime of an individual electronic component, an average lifetime can be estimated based on treating large populations of components probabilistically.


Interestingly, projections of future behavior can often be made without speciﬁc reference to the underlying physical mechanism of degradation.


The time dependence of reliability is implied by the deﬁnition, and therefore the time variable appears in all of the failure distribution functions that will be subsequently deﬁned. Acceptable times for reliable operation are often quoted in decades for communications equipment; for guided missiles, however, only minutes are of interest. The time dependence of degradation of some measurable quantity such as voltage, current, strength,or light emission is often the cardinal concern, and examples of how such changes are modeled are presented throughout the book.


Speciﬁcation of the product testing or operating conditions is essential in predicting reliability. For example, elevating the temperature is the universal way to accelerate failure. It therefore makes a big difference whether the test temperature is 25 C, 25 C, or 125 C. Similarly, other speci-ﬁcations might be the level of voltage, humidity, etc., during testing or use.


Lastly, the question of what is meant by failure must be addressed. Does it mean actual fracture or breakage of a component? Or does it mean some degree of performance degradation? If so, by how much? Does it mean that a speciﬁcation is not being met, and if so, whose speciﬁcation? Despite these


An Overview of Electronic Devices and Their Reliability 15


## 1.2 Reliability, Other ``…ilities,'' and Definitions


### 1.2.1 Reliability


uncertainties it is generally accepted that product failure occurs when the required function is not being performed. A key quantitative measure of reliability is the failure rate. This is the rate at which a device or component can be expected to fail under known use conditions. More will be said about failure rates in Chapter 4, but clearly such information is important to both manufacturers and purchasers of electronic products. With it, engineers can often predict the reliability that can be expected from systems during operation. Failure rates in semiconductor devices are generally determined by device design, the number of in-line process control inspections used,their levels of rejection, and the extent of postprocess screening. Very often,the performance of an IC depends critically on the material’s properties achieved during a particular process step. This requires statistical process control of the process to carefully chosen limits that will guarantee the material’s properties, such that the device performs properly. Therefore,extensive characterization of how the material’s properties depend on process variables is required. An example of this sensitivity is found in the preparation of an extremely thin (angstroms thick) indium tin oxide (ITO) layer used to control the barrier height to carrier injection on a surface or interface used for electrical contact. The barrier height at the surface of the ITO is critically dependent on the details of the preparation process of the ITO.


1.2.2 A Brief History of Reliability


Now that various aspects of reliability have been deﬁned, it is instructive to brieﬂy trace their history with regard to the electronics industry. In few applications are the implications of unreliability of electronic (as well as mechanical) equipment as critical as they are for military operations. While World War I reﬂected the importance of chemistry, World War II and all subsequent wars clearly capitalized on advances in electronics to control the machinery of war-fare. However, early military electronics were far from reliable [12,13]. For example, it was found that 50% of all stored airborne electronics became unserviceable prior to use. The Air Force reported a 20-h maximum period of failure-free operation on bomber electronics. Similarly,the Army was plagued by high truck and power-plant mortalities, while the Navy did not have a dependable torpedo until 1943. Horror stories persisted(and still do) about the large fraction of military electronics that failed to operate successfully when required. Until the early 1950s, the problem of unreliability was met by increasing spare-parts inventories. However, this created the new problem of logistics and the big business associated with the growth of military logistics commands. With this as a background, the US


### 1.2.2 A Brief History of Reliability


Defense Department and electronics industry jointly established an Advisory Group on Reliability of Electronic Equipment in 1952 to seek ways of meliorating the problem. The realization that massive duplication was too expensive drove the military to quantify reliability goals. A several order of magnitude enhancement in product reliability was required to reduce the logistics monster and increase the operational time of equipment. The next 20 years witnessed the introduction of solid-state electronics and much research on all aspects of the subject of reliability. A cumulative reference list of published books dealing with microelectronics and reliability in the years up to 1970 can be found in the journal of the same name [14].


1.2.3 Military Handbook 217


In this section, we shall see how reliability issues have been addressed in a quantitative way by the Defense Department. To meet reliability standards for electronic components and system hardware being developed for the US defense agencies, contractors were obliged, until June 1994, to conform to guidelines in the Military Handbook 217 (MIL-HDBK-217) entitled“Reliability Prediction of Electronic Equipment” [15]. In it there is information on how to predict failure rates of speciﬁc devices and components including discrete semiconductor devices, ICs, vacuum tubes, lasers,resistors, capacitors, switches, rotating devices, connectors, lamps, and so on. Failure rate formulas are given for each product in terms of the involved variables, or factors, that inﬂuence reliability, e.g., temperature, voltage,environment, number of connector pins, and year of manufacture, so that lifetimes may be predicted.


Updated periodically, it has achieved the status of a bible in the ﬁeld; other nations and many individual companies have differing, but essentially similar,guidelines. However, the practice of using MIL-HDBK-217 and other handbooks has been the subject of intense debate over the years. Supporters claim that it enables feasibility evaluation, comparisons of competing designs,and identiﬁcation of potential reliability problems. Detractors, and they are probably in the majority and certainly more vociferous, maintain that MIL-HDBK-217 reliability predictions do not compare well with ﬁeld experience and generally serve to stiﬂe good engineering judgment. Encyclopedic in its coverage of practical reliability concerns, examples of its use coupled with a discussion of its validity will be deferred to Chapter 4.


MIL-HDBK-217 is no longer a conformance document but rather a guidance document for contractors to use as they see ﬁt. However, contractors still have to prove they meet reliability requirements. Hence, great attention is still paid


An Overview of Electronic Devices and Their Reliability 17


### 1.2.3 Military Handbook 217


to the methods and techniques taught in MIL-HDBK-217, which is still available.


1.2.4 Long-term Nonoperating Reliability


We can all appreciate that electrical products might suffer reliability problems as a result of service. But what are we to make of products that are stored in a nonoperating condition for long periods of time, and then fail when turned on. Equipment that is not in direct use is either in a state of dormancy or storage. Dormancy is deﬁned as the state in which equipment is connected and in an operational mode but not operating.


According to this deﬁnition, dormancy rates for domestic appliances,professional and industrial equipment, and transportation vehicles may be well over 90%. On the other hand, equipment that is totally inactivated is said to be in storage; such products may have to be unpacked, set up, and connected to power supplies to become operational. The consequences of nonfunctioning electrical equipment can be severe in the case of warning systems that fail to protect against ﬁre, nuclear radiation, burglary, etc.


when called into service unexpectedly. Military success on the battleﬁeld can hang in the balance because of such failure to function.


The above are all examples of nonoperating reliability, the subject of an entire book by Pecht and Pecht [16]. These authors contend that what are usually understood to be relatively benign dormant and storage environments for electronics may, in fact, be quite stressful. Frequent handling,relocating and transport of equipment, and kitting (packing products in kits), as well as unkitting are sources of impact loading, vibration, and generally harmful stresses. An entirely quiescent environment, involving no handling at all, has even proven deleterious to some products. The materials within the latter are often not in chemical or mechanical equilibrium after processing, and residual stresses may be present. Like a compressed spring that naturally tends to uncoil, the material approaches equilibrium through atomic diffusion or mechanical relaxation processes. Battery corrosion due to current leakage is a prime example of this kind of degradation. Less common examples include failure of presoldered components and open circuiting of ICs, both while being stored on the shelf prior to ﬁnal assembly into electronic products. The former is due to the lack of solderability, presumably because of oxidation, during aging on the shelf. In the latter case, the vexing phenomenon of stress voiding results in slitlike crack formation in the aluminum grains of interconnections, causing ICs to fail.


This effect, attributed to internal stress relief, is aggravated when current is


### 1.2.4 Long-term Nonoperating Reliability


passed through the chip. Stress voiding will be discussed more fully in Chapter 5.


With few exceptions, the environments electronic products are exposed to in operational, dormant, and storage modes are not very different. The primary difference is accelerated damage due to the inﬂuence of applied electric ﬁelds, the currents that ﬂow, and the temperature rise produced.


Several authors have proposed a correlation between the operating and nonoperating reliabilities of electronics. A multiplicative factor “K”deﬁning the ratio of these respective failure rates has been suggested. Values of K ranging anywhere from 10 to 100 have been reported. Such numbers appear to be little more than guesswork and have limited value. A more intelligent approach would be to extrapolate accelerated test results to conditions prevailing during dormancy and storage.


1.2.5 Availability, Maintainability, and Survivability


Important terms related to reliability but having different meanings are availability, maintainability, and survivability. The ﬁrst two refer to cases where there is the possibility of repairing a failed component. Availability is a measure of the degree to which repaired components will operate when called upon to perform. Maintainability refers to the maintenance process associated with retaining or restoring a component or system to a speciﬁed operating condition. In situations where repair of failures is not an option (e.g., in a missile), an appropriate measure of reliability is survivability. Here, performance under stated conditions for a speciﬁed time period without failure is required. Normally these concepts are applied to the reliability of systems.


1.3 FAILURE PHYSICS


1.3.1 Failure Modes and Mechanisms, Reliable


and Failed States


We now turn our attention to the subject of actual physical failure (or failure physics) of electronic devices and components, a concern that will occupy much of the book. At the outset, there is a distinction between failure mode and failure mechanism that should be appreciated, although both terms have been used interchangeably in the literature. A failure mode is the recognizable electrical symptom by which failure is observed. Thus, a short or open circuit, an electrically open device input, and increased current are all modes of electrical failure. Each mode could, in principle, be caused by one or more different failure mechanisms, however. The latter are the speciﬁc


An Overview of Electronic Devices and Their Reliability 19


### 1.2.5 Availability, Maintainability, and Survivability


## 1.3 Failure Physics


### 1.3.1 Failure Modes and Mechanisms, Reliable and Failed States


microscopic physical, chemical, metallurgical, environmental phenomena or processes that cause device degradation or malfunction. For example, open circuiting of an interconnect could occur because of corrosion or because of too much current ﬂow. High-electric-ﬁeld dielectric breakdown in insulators is another example of a failure mechanism.


Components function reliably as long as each of their response parameters, i.e., resistance, voltage, current gain, and capacitance, has values that remain within speciﬁed design limits. Each of the response parameters in turn depends on other variables, e.g., temperature, humidity, and semiconductor doping level, that deﬁne a multidimensional space consisting of reliable states and failed states. Failure consists of a transition from reliable to failed states [17]. Irrespective of the speciﬁc mechanism, failure virtually always begins through a time-dependent movement of atoms, ions, or electronic charge from benign sites in the device or component to harmful sites. If these atoms or electrons accumulate in sufﬁcient numbers at harmful sites, damage ensues. The challenge is to understand the nature of the driving forces that compel matter or charge to move and to predict how long it will take to create a critical amount of damage. In a nutshell, this is what the modeling of failure mechanisms ideally attempts to do. A substantial portion of the latter part of the book is devoted to developing this thought process in assorted applications. Interestingly, there are relatively few categories of driving forces that are operative. Important examples include concentration gradients to spur atomic diffusion or foster chemical reactions, electric ﬁelds to propel charge, and applied or residual stress to promote bulk plastic-deformation effects. And, as we shall see, elevated temperatures invariably hasten each of these processes. In fact, the single most universally inﬂuential variable that accelerates damage and reduces reliability is temperature. Other variables such as humidity, stress, and radiation also accelerate damage in certain devices.


Additionally, the time to a given failure is related to processing and latent defects. If the harmful site already has a minor defect, then the failure happens more quickly because less damage is necessary to cause a failure to occur. Failure rate predictions can be ﬂawed by such occurrences if they are unknown, for example, because test units were not examined before stress or when a root cause is not determined for each failure occurrence.


1.3.2 Conditions for Change


Much can be learned about the way materials degrade and fail by studying chemical reactions. As a result of reaction, the original functional materials


### 1.3.2 Conditions for Change


are replaced by new, unintended ones that impair function. Thermodynamics teaches that reactions naturally proceed when energy is reduced.


Thus, in the transition from reliable to failed behavior, the energies of reliable states exceed those of the failed states; furthermore, the process must proceed at an appreciable rate. Similarly, in chemical systems, two conditions are necessary in order for a reaction to readily proceed at constant temperature and pressure:


1. First, there is a thermodynamic requirement that the energy of the system be minimized. For this purpose, the Gibbs free energy (G) is universally employed as a measure of the chemical energy associated with atoms or molecules. In order for a reaction to occur among chemical species, the change in free energy (DG) must be minimized. Therefore,DG¼Gf –Gi must be negative (DG< 0), where Gf is the free energyof the ﬁnal (e.g., failed) states or products and Gi the free energy of the initial (e.g., reliable) states or reactants. When DG attains the most negative value possible, all of the substances present are in a state of thermodynamic equilibrium. For chemical reactions, thermodynamic data are often tabulated as DG, or in terms of its constituent factors, DH (the enthalpy change) and DS (the entropy change). These contributions are related by


DG ¼ DH  TDS:


(1.1)


Example 1.1


Consider the problem of selecting a contact material for a device made of the hightemperature superconductor YBa2Cu3O7. In addition to the usual attributes of low contact resistance, adhesion, matching of thermal expansion, etc., the contact must be chemically stable. Silver and aluminum are potential contact candidates. Which metal contact is likely to be more stable?


Answer We ﬁrst make the assumption that DG z DH in Eqn (1.1) when TDS is small.


This is generally true in the present case. Therefore, the criterion for possible chemical reaction is that DH< 0. The reactions between Ag or Al and common oxides of YBCO superconductors are given below. Using published enthalpies at 298 K for the involved chemical species, the following DH298 values are calculated for potential reactions between the contact metals and assorted superconductor oxides. In doing so, we recall from elementary thermochemistry that the net enthalpy change is the sum of the enthalpies of the products minus the sum of enthalpies for the reactants, i.e., DH298 (reaction)¼S DH298(products) S DH298 (reactants).


An Overview of Electronic Devices and Their Reliability 21


R e a c t i o n  E n t h a l p y


C u


2


O


ð


4 0


k c a l


=


m o l


Þ


þ


A g


¼


7


:


3


D


2 9 8


¼ þ


3 2


Y


4 5 0


8


B a O


1 3 3


53


A l


A l C u


1 6


4 0 0


23


13


22ReliabilityandFailureofElectronicMaterialsandDevices


22


|Reaction|||||||Enthalpy|Enthalpy|
|---|---|---|---|---|---|---|---|---|

|Cu2O (-40 kcal/mol)|+|2Ag 2(0)|=|Ag2O (-7.3 kcal/mol)|+|2Cu 2(0)|Δ|H298 =+32.7 kcal|

|þ 3 8 0 k c a l |þ 1 0 6 k c a l |0 9 k c a l ||þ 5 0 k c a l |0 : 3 k c a l |2AgY 2(-23.87 kcal/mol)|Δ|H298 = +380 kcal|

|H 9 8 ¼ |H 2 9 8 ¼ |H 2 9 8 ||H 2 9 8 ¼ |+|AgBa (-20.05 kcal/mol)|Δ|H298 =+106 kcal|

||5|5|5|5|5|5|||

Reliability and Failure of


ELECTRONIC MATERIALS ANDDEVICES


Second Edition


MILTON OHRING


Department of Materials Science and Engineering Stevens Institute of Technology


Hoboken, New Jersey


With


LUCIAN KASPRZAK


IBM Retired Bear, Delaware


AMSTERDAM • BOSTON • HEIDELBERG • LONDON


NEW YORK • OXFORD • PARIS • SAN DIEGO


SAN FRANCISCO • SINGAPORE • SYDNEY • TOKYOAP


ELSEVIER


Academic Press is an imprint of Elsevier


# Reliability and Failure of Electronic Materials and Devices


32 Jamestown Road, London NW1 7BY, UK


525 B Street, Suite 1800, San Diego, CA 92101-4495, USA


225 Wyman Street, Waltham, MA 02451, USA


The Boulevard, Langford Lane, Kidlington, Oxford OX5 1GB, UK


Copyright © 2015, 1998 Elsevier Inc. All rights reserved.


No part of this publication may be reproduced or transmitted in any form or by any means, electronic or mechanical, including photocopying, recording, or any information storage and retrieval system,without permission in writing from the publisher. Details on how to seek permission, further


information about the Publisher’s permissions policies and our arrangements with organizations such as the Copyright Clearance Center and the Copyright Licensing Agency, can be found at our


website: www.elsevier.com/permissions.


This book and the individual contributions contained in it are protected under copyright by the


Publisher (other than as may be noted herein).


Notices


Knowledge and best practice in this ﬁeld are constantly changing. As new research and experience broaden our understanding, changes in research methods, professional practices, or medical treatment may become necessary.


Practitioners and researchers must always rely on their own experience and knowledge in evaluating and using any information, methods, compounds, or experiments described herein. In using such


information or methods they should be mindful of their own safety and the safety of others, including parties for whom they have a professional responsibility.


To the fullest extent of the law, neither the Publisher nor the authors, contributors, or editors,


assume any liability for any injury and/or damage to persons or property as a matter of products liability, negligence or otherwise, or from any use or operation of any methods, products,


instructions, or ideas contained in the material herein.


ISBN: 978-0-12-088574-9


Library of Congress Cataloging-in-Publication Data


Ohring, Milton, 1936-


Reliability and failure of electronic materials and devices / Milton Ohring, Lucian Kasprzak. –Second edition.


pages cm


Includes index.


ISBN 978-0-12-088574-9 (hardback)


1. Electronic apparatus and appliances–Reliability. 2. System failures (Engineering) I. Kasprzak,Lucian. II. Title.


TK7870.23.O37 2014


621.381–dc21


2014031265


British Library Cataloguing in Publication Data


A catalogue record for this book is available from the British Library


For information on all Academic Press publications


visit our web site at http://store.elsevier.com/


Working together


to grow libraries in


ELSEVIERBook Aiddeveloping countries


www.elsevier.com●www.bookaid.org


# Copyright


DEDICATION


He whose works exceed his wisdom, his wisdom will endure.


Ethics of the Fathers


In honor of my father, Max,


. a very reliable dad.


- Milton Ohring


# Dedication


PREFACE TO THE SECOND EDITION


The ﬁrst edition is a classic in form, content, and execution. The form of each chapter takes the reader on a trip through a basic phenomena and its application to failure in electronics (from simple physics to the complicated math often involved). The content of the book covers all the relevant disciplines necessary to do a thorough job of discovery of the true cause of failure. The execution includes relevant examples from the macroscopic to the microscopic to the atomic, where necessary. The book is truly a masterpieceddue in large part to Milt’s knowledge and experience in physics, chemistry, electronics, materials, and most of all his unique ability to frame difﬁcult problems in the appropriate mathematics.


As such then, only changes were made where necessary, to keep the book current and useful to the reader (a researcher struggling to determine the true cause of failure so that it can be remedied and never happen again).


By the way that is what has made this industry so successfuldfailure analysis to true root cause.


L. Kasprzak


xvii


# Preface to the Second Edition


PREFACE TO THE FIRST EDITION


Reliability is an important attribute of all engineering endeavors that conjures up notions of dependability, trustworthiness, and conﬁdence. It spells out a prescription for competitiveness in manufacturing, because the lack of reliability means service failures that often result in inconvenience,personal injury, and ﬁnancial loss. More pointedly, our survival in a hightech future increasingly hinges on products based on microelectronics and optoelectronics where reliability and related manufacturing concerns of defects, quality, and yield are of critical interest. Despite their unquestioned importance, these subjects are largely ignored in engineering curricula.


Industry compensates for this educational neglect through on-the-job training. In the process, scientists and engineers of all backgrounds are recast into reliability “specialists” with many different attitudes toward reliability problems, and varied skills in solving them. The reliability practitioner must additionally be a detective, a statistician, and a judge capable of distinguishing between often-conﬂicting data and strongly held opinions. This book attempts to systematically weave together those strands that compose the fabric of the training and practice of reliability engineers.


The multifaceted issues surrounding the reliability and failure of electronic materials and devices lie at the conﬂuence of a large number of disciplinary streams that include materials science, physics, electrical engineering, chemistry, and mechanical engineering, as well as probability and statistics. I have tried to integrate the derivative subject matter of these disciplines in a coherent order and in the right proportions to usefully serve the following audiences:


• advanced undergraduate and ﬁrst year graduate engineering and science students who are being introduced to the ﬁeld,


• reliability professionals and technicians who may ﬁnd it a useful reference and guide to the literature on the subject, and


• technical personnel undergoing a career change.


While the emphasis of the book is on silicon microelectronics technology, reliability issues in compound semiconductor and electro-optical devices, optical ﬁbers, and associated components are also addressed. The book starts with an introductory chapter that brieﬂy deﬁnes the subject of semiconductor reliability, its concerns, and historical evolution. Chapter 2 introduces electronic materials and devices, the way they are processed,


xix


# Preface to the First Edition


how they are expected to behave, and the way they sometimes malfunction. The important subjects of intrinsic and manufacturing defects,contamination, and product yield are the focus of Chapter 3.


|Cu2O + 2 = AlCu2 + 1/ 2Al2O3 (-40 kcal/mol) (-16.1 kcal/mol) 1 ⑨ 3( -400 kcal/mol)|Cu2O + 2 = AlCu2 + 1/ 2Al2O3 (-40 kcal/mol) (-16.1 kcal/mol) 1 ⑨ 3( -400 kcal/mol)|Cu2O + 2 = AlCu2 + 1/ 2Al2O3 (-40 kcal/mol) (-16.1 kcal/mol) 1 ⑨ 3( -400 kcal/mol)|Cu2O + 2 = AlCu2 + 1/ 2Al2O3 (-40 kcal/mol) (-16.1 kcal/mol) 1 ⑨ 3( -400 kcal/mol)|Cu2O + 2 = AlCu2 + 1/ 2Al2O3 (-40 kcal/mol) (-16.1 kcal/mol) 1 ⑨ 3( -400 kcal/mol)|Cu2O + 2 = AlCu2 + 1/ 2Al2O3 (-40 kcal/mol) (-16.1 kcal/mol) 1 ⑨ 3( -400 kcal/mol)|Cu2O + 2 = AlCu2 + 1/ 2Al2O3 (-40 kcal/mol) (-16.1 kcal/mol) 1 ⑨ 3( -400 kcal/mol)|Δ|H298=-109 kcal|

|k c a l = m o l Þ |+|A l 2 O 3 |k c a l = m o l Þ |ð 0 Þ |ð 0 Þ |2Y 2(0)|Δ H298 = +50 kcal||

|2 A g Y |k c a l = m o l Þ |13 |4 0 0 |B a |B a ||||

|2 ð 2 3 : 8 7 |A g B a ||=|þ |þ |+ Ba (0)||△H298=-0.3 kcal|

|||þ 1 |3 ð |2 Y 2 ð 0 Þ |2 Y 2 ð 0 Þ |m o l Þ |||

The positive enthalpy values for Ag mean that this metal is less reactive than Al and therefore likely to be a more stable contact.


2. The second requirement is a practical one that involves kinetics. Once the reaction is thermodynamically possible, it must proceed at an appreciable rate. Otherwise, there will be little actual chemical change and degradation. The rate at which chemical reactions occur is proportional to the Maxwell–Boltzmann factor (also known as the Boltzmann or Arrhenius factor) according to


Rate ¼ A expDGRT;A ¼ constant


(1.2)


where DG* is the activation free energy (in the usual units of J/mol or cal/mol), T is the absolute temperature, and R is the gas constant(¼8.314 J/mol-K or 1.987 cal/mol-K). Because of its ubiquitous presencewhenever degradation is thermally accelerated, Eqn (1.2) is easily one of the most important equations in this book and one worth remembering.


Note that DG* does not equal DG, and in fact has a very different interpretation, as shown in Figure 1.9(a). The energy barrier that atoms or molecules must surmount to squeeze by neighbors, or push them apart,so that reaction can occur is essentially DG*; its magnitude hinges on the particular path between initial (unstable) and ﬁnal (stable) states. If a catalyst is present, DG* may be effectively reduced. In contrast, DG is the ﬁxed energy difference between the ﬁnal and initial states, irrespective of path.


1.3.3 Atom Movements and Driving Forces


The language of diffusion in solids is similar to that used in chemistry when describing chemical reactions. We speak of atoms surmounting energy barriers established along the reaction coordinate. In the periodic lattice of Figure 1.9(b), a model is presented for diffusing atoms positioned between neighboring planes within a crystalline matrix. For atoms to move from one site to another, two conditions must be fulﬁlled; a site must ﬁrst be available for atoms to move into (e.g., a vacancy) and second,the atom must possess sufﬁcient energy to push atoms aside in executing the required jump. Thus, rates of diffusion and chemical reactions are mathematically expressed by the same Boltzmann-type formula (Eqn (1.2)).


An Overview of Electronic Devices and Their Reliability 23


### 1.3.3 Atom Movements and Driving Forces


Speciﬁcally, the diffusion constant D, in units of square centimeters per second, can be written as


D ¼ D0 expEDD=D0 exp -RT(RT)';


(1.3)


where D0 is a constant. For simplicity throughout the remainder of the book we will generally replace DG* by the relevant activation energy barrier, in this case ED. Both D0 and ED are dependent on the nature of the diffusant and matrix and the speciﬁc path taken by the atoms. Values of D as a function of T for atomic diffusion in metals, semiconductors, and oxides are given in various sources [18].


Now we consider the transport of atoms in systems where generalized driving forces exist. If a driving force or bias did not exist in the case of diffusion, atoms would migrate with equal probability in opposite directions and there would be no net displacement. When driving forces (orﬁelds) exist over atomic dimensions a, the periodic array of lattice energy barriers assumes a tilt, or bias, as shown in Figure 1.9(c). Now, atoms in site+a→


Figure 1.9 Potential energy of atoms in a periodic lattice: (a) in the absence of a force,


(b) model of a diffusing atom jumping between neighboring plane sites into a vacancy, (c) in the presence of a force (ﬁeld). The energy barrier for reaction is DG*. From Ref. [18].


FREE ENERGY


山


DISTANCE


AN"Hvacancy(c)FREEOAPPLIED FIELD


△G*NotngO00OO


△G


O O


2 have a lower energy by an amount DG than those in site 1, a distance a away. In addition, the energy barrier to atomic motion from 1 to 2 is lower than that from 2 to 1. In fact, the slope of G with distance, or the free energy gradient, is caused by and is physically equal to the applied driving force (F). This force effectively acts over distance a/2, so that F¼ 2DGawith units of force per mole (or force/atom). Since atoms vibrate in place with with frequency v(≈ 1013 s-1) awaiting a successful jump, the rate at whichfrequency n (z 1013 s1) awaiting a successful jump, the rate at which atoms move to the right is given by


r12 ¼ n exp ðDG  DGÞRT(s-1),(DG*-DG)]ðs1Þ;


(1.4a)


while in the latter case,


r21 ¼ n exp ðDG þ DGÞRT(△G*+△G)(s-ðs1Þ:


(1.4b)


The net rate, or difference of individual rates, is the quantity of signiﬁcance, and it is given by


rnet ¼ r12  r21 ¼ n expfnet = 112 -121 = v exp DGRT△G*2 sinhRT2 sinhDGRT: (1.5)


It is instructive to consider the case where DG*>DG. If additionally,DG is small compared to RT, sinh DG/RT z DG/RT. After substituting DG¼ Fa/2 and noting that the atomic velocity v¼ a rnet, Eqn (1.5)becomes v ¼ DFRT;


(1.6)


where where D is associated with a2v exp [-DG*/RT] (or a2v exp [-ED/RT].D is associated with a2n exp [DG*/RT] (or a2n exp [ED/RT].This important formula is known as the Nernst–Einstein equation and is valid in describing both chemical and physical changes induced through diffusional motion of atoms. It is to the dynamics of microscopic chemical systems what Newton’s law relating force to acceleration is to macroscopic mechanical systems. Later we will model degradation phenomena like electromigration, mechanical creep, and compound growth using this equation. When the driving force is large, however, the higher powers of sinh DG/RT cannot be neglected. Atomic velocities or rates of reaction may then vary as the hyperbolic sine or some power b of the driving force,i.e., Fb. Alternatively, it is common to absorb DG, or the driving forces,


An Overview of Electronic Devices and Their Reliability 25


into DG*, so that in effect a reduced activation energy is operative. As a result, hybrid expressions of the general form


v ¼ KFb exp ðDG  aFÞRT


(1.7)


(K¼ constant) are sometimes used in modeling high ﬁeld damage orphenomena (e.g., dielectric breakdown, high electric-ﬁeld conduction in insulators). The mean time to failure (MTTF) is usually assumed to be proportional to the reciprocal of the degradation reaction velocity, i.e.,MTTF z v1.


It is common to have more than one operative driving force acting in concert with temperature to speed reactions. Note that temperature is not a true driving force, even though terms like “temperature stressing”are frequently used; true driving forces like temperature gradients establish a system bias. Electric ﬁelds, electric currents, mechanical stress, and humidity gradients are examples of forces that have served to hasten failure of components and devices. Empirical formulas combining products of forces and modiﬁed Boltzmann factors (e.g., .Fbii Fbjj .;.exp½ðDG  aFi  bFj.Þ=RT ) might, for example, be used to accountfor dielectric breakdown at a given electric ﬁeld (Fi) and humidity level (Fj).


Whether small or large driving forces are operative is dependent on the physical process in question. Small energy changes, corresponding to bond shifting, or breaking and reforming in a single material, are involved in diffusion, grain growth, and dislocation motion. This contrasts with chemical reactions, for example, where high-energy primary bonds break in reactants and reform in products.


1.3.4 Failure Times and the Acceleration Factor


At the outset, it is important to distinguish among the various times that are associated with failure. Imagine a number (n) of identical units that fail in service after successively longer times t1, t2, t3, t4, t5, . tn. The MTTF is simply deﬁned as


MTTF ¼


t1 þ t2 þ t3 þ t4 þ t5 þ.þ tnn:


(1.8)This time, however, differs from the median time to failure (t50), which is deﬁned to occur when 50% have failed; thus half of the failures happen


### 1.3.4 Failure Times and the Acceleration Factor


prior to t50 and the remaining half after t50. Lastly, there is the mean time between failures, or MTBF, deﬁned as


MTBF ¼ ðt2 (t2-t1)+(t3-t2)+...+(tn-tn-1) t1Þ þ ðt3  t2Þ þ.þ ðtn  tn1Þn¼ (tn-t1)/nðtn  t1Þ=n (1.9)


In this book, we shall usually use MTTF to describe or model physical failure times. On the other hand, t50 will mostly arise in the statistical or mathematical analysis of failure distributions.


In the reliability literature, there is a widely used term known as the acceleration factor (AF), which is based on explicit formulas for failure rate,failure time, or the Nernst–Einstein equation in its various versions and modiﬁcations. AF is deﬁned as the ratio of a degradation rate at an elevated temperature T2 relative to that at a lower base temperature T1, or conversely, as the ratio of times to failure at T1 and T2. Through application of Eqn (1.2), the AF is easily calculated in the temperature range between T1 and T2:


AF ¼ MTTFðT1Þexp[△G*/RT1]MTTFðT2Þ ¼exp[△G*/RT2]exp½DG=RT1exp½DG=RT2 ¼ exp[()(-/)]DGR1T1 1T2:(1.10)


Thus, if the failure time is known at T2, assuming one knows DG*,then it can also be calculated at T1. Additionally, these Arrhenius expressions can be used to determine the activation energy if AF is known experimentally.


When one driving force having magnitudes F1 and F2 is operative at the two temperatures, we may tacitly assume that degradation reaction rates proceed with the velocity given by Eqn (1.6). With such an assumption, the AF is given by


AF ¼ MTTFðT1ÞMTTFðT2Þ ¼ðT1=F1ÞexpEDRT1RT1ðT2=F2ÞexpRT2EDRT2 ¼ T1F2T2F1exp[(-2)]EDR1T1 1T2:


(1.11)


We shall return to AFs in Section 4.5.5.


A ﬁnal note about temperature is necessary in the context of rates. In Figure 1.9(b), as temperature increases, the atoms vibrate at higher frequency and move farther apart. This dual effect causes two sources of


An Overview of Electronic Devices and Their Reliability 27


reaction rate increase. First, the higher frequency of vibrational energy (kT)means the atoms bump into the spaces between the atoms more frequently with higher energy. Second, the spaces between the atoms are larger on average because the center-to-center spacing increases as temperature rises.


Thus, temperature accelerates the rate at which the bad effect will take place. In a sense, temperature has a twofold effect as described above. First,there is more energy driving the reaction (diffusion) rate, and second, the reaction (diffusion) rate can take place more easily because the center-tocenter dilation results in larger spaces for the atoms to move through.


1.3.5 Load-Strength Interference


An instructive way to close this section on reliability physics is to consider the concept of load-strength interference [19]. Every product has a collection of individual strengths (Si) or stress levels of resistance to corresponding loads (Li) applied in service. Note that in the context of this discussion, the loads are more correctly, applied stresses. Thus, a ceramic has an ultimate tensile strength beyond which it fractures, a critical electricﬁeld level that causes breakdown, a speciﬁc resistance to thermal-shock loading, and so on. As long as the mechanical and electrical service loads challenge, but do not exceed, the respective strengths, the ceramic is safe. But, should any one of its strengths be exceeded by the corresponding load, the ceramic undergoes catastrophic failure by that particular mechanism.


These ideas are illustrated in Figure 1.10(a), where the particular set of load and strength variables have discrete values. In this case, the strength exceeds the load, and there is no failure. It is more realistic to assume that the strength of materials is statistically distributed, as shown in Figure 1.10(b) and indicated on the vertical axis. For example, a given ceramic has a probability of failing over a wide distribution of tensile strength levels, while in metals that distribution is extremely narrow.


Similarly, the applied loads are often not constant but distributed over a range of values. Since the magnitude of the statistically lowest strength level is signiﬁcantly higher than the largest applied load by a large margin, failure is again impossible. With time, however, the strength of materials may wane due to degradation (e.g., thermal softening due to creep, corrosion),but the applied stress distribution still remains unchanged. Conditions for marginal behavior followed by failure may then arise because service load levels overlap or interfere with the strengths of the weaker members. This subject will be addressed again in Section 12.5.2.


### 1.3.5 Load-Strength Interference


1.3.6 Semiconductor Device Degradation and Failure


The mechanisms for semiconductor failure can be grouped into three main categories [20]:


1. Chip level or intrinsic failures


2. Packaging or extrinsic failures


3. Electrical stress induced (in-circuit) failures


Intrinsic failure mechanisms originate from the silicon chip or die and the processing performed in the front end2 of manufacturing line (FEOLfront end of line). Potential defects and sources for failure exist in each material used and in every process step that alters composition and device features. Defect sources can reside in the silicon wafer substrate itself; in the dielectrics like SiO2 and other insulating ﬁlms (silicon nitride, phosphorous,and boron-containing oxide glasses); in the metallizations and passivation used in the back-end processing, which include aluminum-base alloy or 0


TIME


Figure 1.10 (a) Discrete set of load and strength values. There is no failure because the strength exceeds the load. (b) Both strengths and loads are statistically distributed.


With time at constant load, decreasing strength causes increasing overlap, or interference, and eventual failure.


2 Front end means silicon wafer processing before metallization, i.e. silicon, dielectric and contact holes. Back end means wafer processing starting with ﬁrst metallization and continuing with


passivation of as many metal levels of metallization, as are needed for wiring to the chip terminals,which are wire bonded to a lead frame or ﬂip chip mounted to a package surface.


An Overview of Electronic Devices and Their Reliability 29


可可


initial


marginal


STRENGTH


STRENGTHdistribution margin


failure


LOAD


load


distribution strength


state


### 1.3.6 Semiconductor Device Degradation and Failure


copper ﬁlm interconnections between devices and components; and in the semiconductor contacts composed of assorted metal alloys and compounds(Al, Al–Si, various metal silicides, Ti–W, TiN, etc.). Design errors plus the combination of lithography (patterning, tolerances, registration, and overlay) and processing defects, the ubiquitous presence of contamination, and the intrinsic limitations of material properties and thickness all sow the seeds for eventual chip-level failures. Temperature, voltage, current, stressing during use, combined with environmental inﬂuences such as humidity and radiation, then accelerate the transition from reliable to failed states. Masstransport-induced failure mechanisms on the chip include interdiffusion that results in unwanted compounds, precipitates or void formation at contacts, electromigration or a current-induced migration of atoms in interconnections, and corrosion at unprotected contacts. Examples of deleterious charge transport effects include Naþ contamination, dielectric breakdown, penetration of SiO2 by so-called hot electrons that originate in the underlying silicon, and “soft errors” in logic or memory caused by ionizing radiation. Chapters 5, 6, 7, and 10 address such failures in greater detail.


Extrinsic failures are identiﬁed with the interconnections formed in the back-end (BEOL-back end of line) processing and packaging of chips.


Potential failures now arise in the steps associated with ensuring that IC contact pads are electrically connected to external power sources and signal processing circuits. Problems arise in attaching dies to metal frames and wires to contact pads, encapsulating chips into packages, and soldering them to printed circuit boards. Speciﬁc failure mechanisms include die fracture,open bond joints, moisture-induced swelling and cracking of plastic packages, corrosion, contamination by impurities, formation of intermetallic compounds and voids at bonds, and fatigue, as well as creep of solder connections. In addition to mass-transport driving forces, thermal mismatch stresses between components play an important role in effecting solder degradation and failure. Chapters 8 and 9 are devoted to addressing failure in packages and interconnections, and particularly the role played by mechanical stresses.


Electrical stress induced failures are event dependent and largely caused by overstressing and excessive static charge generated during handling in service. Electrostatic discharge (ESD) and electrical overstress (EOS) are the operative mechanisms that often destroy sensitive electronic components.


In addition to mishandling, damage is frequently caused by poor initial design of circuits or equipment. The subject of ESD is treated in Chapter 6.


1.3.7 Failure Frequency


Now that an overview of failure in ICs and associated packages has been presented, we may well ask how frequently failure occurs. This is a complex question that depends not only on the more-or-less objective classiﬁcation of device or circuit type, level of technology, and manufacturer, but also on the subjective assessment of what constitutes failure and the often problematical way it is reported. In this regard, we consider both the frequency of failure modes and failure mechanisms. Both display wide quantitative variations, and that is why only a qualitative discussion of them is merited.


The basic failure modes have been classiﬁed as short circuits, open circuits, degraded performance, and functional [21]. By functional failures we mean situations where the output signal is different from the one expected. Thus, diodes and transistors, for example, often fail through short circuiting, as do ceramic, foil, and dry tantalum capacitors. Optoelectronic devices, piezoelectric crystals, and resistors, on the other hand, frequently open circuit. Coils, ICs, and relays are examples that largely exhibit functional failures. Virtually all devices and components suffer more or less performance degradation prior to activation of the particular failure mode.


Many pie charts, histograms, and tables dealing with the frequency of failure mechanism occurrence permeate the literature. They will not be reproduced here because of their very transitory value and narrow utility. In some, intrinsic failures associated with metallizations and dielectrics dominate, while in others, extrinsic failures associated with packaging defects and solder joints are in the majority. Electrical stress induced damage always seems to be well represented.


In addition, it has also been found that the responsibility for failure can be allocated between the manufacturer and the user. ESD and EOS failures caused by mishandling and those due to environmental factors (humidity)are examples of user responsibility. For some of the reasons noted above,the proportionate share of fault between manufacturer and user varies widely. However, a summary [21] of such data shows roughly equal fault.


The literature of reliability physics generally devotes coverage of failure mechanisms in proportion to their frequency of occurrence or their perceived importance; this is also reﬂected in the attention given to them in this book. While failure frequencies of the past and present are no indication of future performance, theymay provide some perspective of what to expect.


In this sense, Chapter 1 through 11 are prerequisite to Chapter 12, which attempts to peer into the reliability implications of future technology trends.


An Overview of Electronic Devices and Their Reliability 31


### 1.3.7 Failure Frequency


1.3.8 The Bathtub Curve and Failure


This overview ends with an introduction to the most widely recognizable graphic representation of reliabilitydthe bathtub curvedfollowed by some thoughts on failure. Originally designed to display the rate at which humans die with age, the bathtub curve has been adopted to describe the life of assorted products. It is reproduced in Figure 1.11 and represents the failure rate as a function of time. Although a more rigorous deﬁnition of failure rate will be given in Chapter 4, the number of failures per unit time will sufﬁce here. Components and devices usually live through one or more stages of this curve. During early life the failure rate is high, since the weak products containing gross or macroscopic manufacturing defects do not survive. This short-time portion of the curve is therefore known as the early failure, or more commonly as the infant mortality, region. Eliminating this region of the curve is effected by the widely employed practice of screening out obviously defective components, as well as weak ones with a high potential for failure. In such screening processes, products must survive the ordeal of burn-in (e.g., stressing at high temperature, application of EOS,temperature cycling) prior to shipment.


In contrast to the declining failure rate of infant mortality, the next region is characterized by a roughly constant failure rate. Since random failures occur that are not intrinsic to devices but rather to external circumstances (e.g., lightning, ﬂoods) during the indicated time span, this region normally corresponds to the working life of the components. Lastly,


Figure 1.11 Bathtub curve.


### 1.3.8 The Bathtub Curve and Failure


the failure rate increases in the last stages of life due to wear out. More subtle, microscopic defects grow over time, curtailing life in these latter stages. The reader will well appreciate that many mechanical components and biological systems seem to track similar life histories.


Approaches to achieving high reliability differ signiﬁcantly in the infant mortality and wear-out stages. In the former, the sources, or root causes, of defects must be exposed, followed by action to eliminate them. If defects cannot be eliminated at the source, then screening by burn-in is conducted.


Wear-out failure is combated by developing robust technologies with improved circuit and device designs that employ damage-resistant materials.


Nowadays, IC chips rarely wear out; rather, new technology usually forces them into retirement. In Section 4.5.9, the bathtub curve will be revisited to capitalize on the statistical functions introduced there.


Perhaps the three most important words raised about failure are when,how, and why; in one form or other, the remainder of the book is largely devoted to addressing them. The connections between these terms are neatly depicted in the triangular representation of Figure 1.12 [22]. At the triangle’s


Figure 1.12 Depiction of connections between the when, why, and how of failures.


Solid lines denote a connection, and dashed lines indicate the absence of a connection. From Ref. [22].


An Overview of Electronic Devices and Their Reliability 33


base we essentially have the divisions of the bathtub curve we have just considered. Corresponding failures can be gradual, the way soles on shoes wear, or sudden and catastrophic, such as when light-bulb ﬁlaments burn out. Failures can be random, say due to ESD, or preordained, where some internal mechanism causes the product to fail deterministically at a set rate from the moment of birth. Preordained failures are thus time dependent.


These descriptors may be directly related, as indicated by the solid lines,or show the absence of a connection in the case of a dashed line. Thus,wear-out failures may be gradual or sudden, but not random. Infant mortality failures display all characteristics, and this makes it difﬁcult to deal with them.


The individual chapters of the book will also deal with two more questions, namely, what happened and where did it happen. The answers are equally important and sort of corollaries to the how and why. Both sets of answers taken together deﬁne the root cause of material failure. These additional questions characterize the speciﬁc mechanism of degradation of a particular material, which ultimately caused the observed failure at some speciﬁc location in the IC, package, or printed circuit board (PCB). Our endeavor is to elucidate the known mechanisms and the kinetics of their behavior with an eye toward eliminating their occurrence in future product designs and processes.


1.4 SUMMARY AND PERSPECTIVE


As its title suggests, this chapter has provided a brief overview of the reliability of electronic materials and devices. These important concerns are intimately tied to the performance of present electronic products as well as to the creation of improved successors. Repeated cycles of manufacture,ﬁeld use, failure, and product redesign have characterized the Age of Electricity and Electronics since its inception, and will probably be coterminous with its demise, if that ever occurs. Issues of defects, product yield,reliability, and degradation are important considerations in these cycles. In this chapter, a broad footprint of these and related topics treated in the book has been broadly sketched.


Appreciation of the causal connections between the types of electronic products and the way they fail requires an understanding of the nature of the materials they are composed of. Recommended texts on materials science and engineering [18,23–25] will assist the reader to acquire this background. Next, the behavior of speciﬁc devices (Chapter 2) and how


## 1.4 Summary and Perspective


they were processed with particular reference made to sources of defects and contamination (Chapter 3) serve to establish the nature of the product prior to service. Product yield measures the effectiveness of eliminating defects during processing. While readers may be knowledgeable about aspects of electronic materials and the devices, processing and the issues surrounding defects and yield are likely to be less familiar.


Now the stage is set for Chapter 4, which is devoted to a quantitative treatment of reliability. Provided that sufﬁcient failure data are available from ﬁeld experience or testing, there are several statistical approaches for dealing with them. The purpose is to obtain failure rates, the MTTF, and to predict future failure behavior. No book on reliability would be complete without treating these concepts. But, by the same token, no book on reliability would be balanced if it did not present some of the current criticisms and controversies surrounding long-held beliefs on failure and the lifetime predictions that stem from them.


Much of the remainder of the book is concerned with failure physics on the chip as well as packaging levels. Here, well-established methods of scientiﬁc investigation are employed to uncover the mechanisms of failure and how they depend on the involved driving forces. Obtaining expressions for failure or degradation times in terms of the operative stresses is a particular objective of these failure modeling studies. Irrespective of the speciﬁc mechanism, failure virtually always begins through a timedependent movement of atoms, electrons, or charge from benign sites in the device or component to harmful sites, or failed states. If these atoms or electrons accumulate in sufﬁcient number at harmful sites, damage results.


As noted earlier, the challenge is to understand the nature of the driving forces that compel matter or charge to move and to predict how long it will take to create a critical amount of damage.


EXERCISES


1. “On October 21, 1879, Thomas Edison’s famous (tungsten ﬁlament)lamp attained an incredible life of 40 h. The entire electrical industry has as its foundation this single invention . the incandescent lamp.”J.W. Guyon, GEC (1979).


a. Support the validity of the second sentence.


b. How many different materials can you identify in a common light


bulb that pose reliability problems?


An Overview of Electronic Devices and Their Reliability 35


## Exercises


2. Provide examples of products combining


a. electrical and mechanical technologies.


b. electrical and electronic technologies.


c. electronic and optical technologies.


3. The law of personal computing systems scaling suggests that the logarithm of the sum of the length (L) plus width (W) plus height (H) varies


linearly with time. If L þ W þ H is halved every 6 years, sketch thevariation for the following computers: desktop, notebook, palmtop,


credit card, wristwatch, and ﬁnger ring. When can ﬁnger ring computers be expected?


4. The number of transistors used per person in theUnited States has grown


from about 5 to 4 107 during the years 1955–1997. Sketch this growthin usage on a graph using appropriate axes. If the trend continues, estimate the number of transistors each person will be using in 2010.


5. The growth in the number of devices per chip (N) appears to obey a


law of the form dN/dt z kN (k¼ constant), i.e., growth proportionalto how many devices are instantaneously present. Chemical reactions


and radioactive decay also suggest similar trends. Discuss physical reasons for the exponential rise or exponential decay.


6. Write an equation that approximates the decrease in size of mobile


phones. In what year can we expect to see the Dick Tracy comics


become reality by incorporating telephones into wristwatches? Assume


that the watch dimensions are 3.5 2 1 cm.


7. The implications of unreliability in the medical profession are at least as


severe as they are in aerospace technology. Comment on possible differences and similarities in the reliability issues faced by each.


8. By considering Figures 1.2 and 1.3, calculate the density (number per


unit area) of devices as a function of time. Is the rate of growth in


device density higher in microprocessor or memory chips?


9. Comment on the thermodynamic stability of silicon, aluminum, and


silicon dioxide that are often either in contact with or located within


a few nanometers of each other on IC chips.


10. Contrast the shape of the bathtub curve for human death rates with age


in 1900 with that at the end of the twentieth century. What are the


reasons for the difference?


11. The energy barrier that must be surmounted to convert “reliable”


states to “failed” states located a distance a apart is Erf. Furthermore,the energies of the reliable and failed states are Er and Ef,


respectively.


a. Represent these states and the energy that separates them graphically.


b. Write an expression for the rate of production of failed states as a function of temperature.


c. Suppose that a driving force acts to produce failed states. Write an expression for the net rate of failed-state production. Represent the action of the driving force graphically.


12. For a particular failure mechanism, two expressions for the MTTF have


been suggested, namely,


MTTF ¼ AFn expRTMTTF=AF" expERTand MTTFand MTTF


¼ B exp= B expE  aFRTE-αF;where F is the


driving force. If A, B, E, n, and a are positive constants independent of


temperature and force,


a. Write expressions for the AF in each case when the temperature is raised from T1 to T2 at constant F.


b. Write expressions for the AF in each case when the force is increased from F1 to F2 at constant T.


c. Which of the two formulas for MTTF gives a higher value of AF for temperature acceleration?


d. Which formula gives a higher value of AF for ﬁeld acceleration?


13. It has been claimed that an AF of two governs chemical reaction rates when the temperature is raised by 10 C. What activation energy when the temperature is raised by 10 °C. What activation energy isis


required for this to happen at room temperature?


14. Contrast the applicability of Newton’s laws and the Nernst–Einstein


equation to the motion of atoms in solids.


15. Suppose the strength (S) of a material has a Gaussian-like spread about


mean value S0 such that the distribution of S values is given by


expexp -10ðSS0Þ2S2010(S-S0)2. The applied load (L), or stress distribution, is similarly given by exp8ðLL0Þ2Where Lo is the mean load. FailureL208(L-L0)2, where L0 is the mean load. Failure


will occur when the strength and load overlap such that a common


value of 0.04 is reached in each distribution.


a. What are the values of L and S that would cause failure?


b. Calculate the ratio L0/S0 at failure.


An Overview of Electronic Devices and Their Reliability 37


16. Initially, the extent of strength–load overlap in a material occurs at a


distribution value of 0.001. During service the applied load remains


constant, but the mean strength of the material declines exponentially


as S0ðtÞ ¼ S0 exp½kt, where k is a constant. If the load and strengthdistributions are described by Gaussians as in Exercise 1–15, and failure


occurs when the value for each is 0.04, calculate the failure time in


terms of L0, S0, and k.


REFERENCES


[1] J.A. Fleming, Fifty Years of ElectricitydThe Memories of an Electrical Engineer, The


Wireless Press, London, 1921.


[2] R. Friedel, P. Israel, B.S. Fein, Edison’s Electric Light, Rutgers University Press, New


Brunswick, 1986.


[3] M. Josephson, Edison, McGraw Hill, New York, 1959.


[4] C.L. Briant, B.P. Bewlay, MRS Bull. XX (8) (1995) 67.


[5] S. Okamura (Ed.), History of Vacuum Tubes, IOS Press, Amsterdam, 1994.


[6] A.J. DeMaria, IEEE Circuit. Devic. 7 (3) (1991) 36.


[7] E.A. Sack, Proc. IEEE 82 (1994) 465.


[8] J.D. Meindl, Proc. IEEE 83 (1995) 619.


[9] S. Malhi, P. Chatterjee, Circuit. Devic. 10 (3) (1994) 13.


[10] D.L. Crook, in: 28th Annual Proceedings of the IEEE Reliability Physics Symposium,


1990, p. 2.


[11] M. Penn, Microelectr. J. 23 (1992) 255.


[12] R.M. Alexander, Tutorial Notes, IEEE International Reliability Physics Symposium


4.1, 1984.


[13] J. Vaccaro, Proc. IEEE 61 (1974) 169.


[14] G.W.A. Dummer, Microelectronics and Reliability 9 (1970) 359.


[15] Military Handbook (MIL-HDBK-217F) Reliability Prediction of Electronic Equipment, Department of Defense, 1991.


[16] M. Pecht, J. Pecht, Long-term Non-operating Reliability of Electronic Products,


CRC Press, Boca Raton, 1995.


[17] A.V. Ferris-Prabhu, Tutorial Notes, IEEE International Reliability Physics Symposium


3.1, 1984.


[18] M. Ohring, Engineering Materials Science, Academic Press, San Diego, 1995.


[19] P.D.T. O’Connor, Practical Reliability Engineering, second ed., Wiley, Chichester,


1985.


[20] E.A. Amerasekera, D.S. Campbell, Failure Mechanisms in Semiconductor Devices,


Wiley, Chichester, 1987.


[21] F. Jensen, Electronic Component Reliability, Fundamentals, Modeling, Evaluation and


Assurance, Wiley, Chichester, 1995.


[22] F.R. Nash, W.B. Joyce, R.L. Hartman, E.I. Gordon, R.W. Dixon, AT&T Tech. J.


64 (3) (1985) 671.


[23] C. Newey, G. Weaver, Materials in Action SeriesdMaterials Principles and Practice,


Butterworths, London, 1990.


[24] M.F. Ashby, D.R.H. Jones, Engineering Materials 1dAn Introduction to Their


Properties and Applications, Pergamon Press, Oxford, 1980.


[25] C.R.M. Grovenor, Microelectronic Materials, Adam Hilger, Bristol, 1989.


## References


CHAPTER 2


Electronic Devices: How They Operate and Are Fabricated


2.1 INTRODUCTION


Books on reliability ideally focus on issues related to component and device failure within the context of how they are intended to function. Because it is often not necessary to know about the latter to address the former, these two bodies of knowledge and expertise often remain separate concerns.


This is especially so because most failures involve materials other than the semiconductors, e.g., metallizations, insulation, and packaging materials.


Nevertheless, it is fair to say that malfunction, failure, and reliability can be more intelligently confronted through some knowledge of device behavior and fabrication methods employed. For example, awareness of device current–voltage characteristics is certainly helpful in diagnosing failure modes in some instances. Similarly, an appreciation of the processing steps involved in device manufacture may suggest ways to avoid future failures.


In this spirit, the chapter is primarily devoted to elevating the consciousness and sensitivity of readers to electronic devices and their uses, characteristics,and instabilities. Many aspects of the degradation and reliability of speciﬁc devices will be introduced here in a qualitative way. We shall return to these same issues in later chapters, where degradation and the physics of failure will be analytically modeled at a deeper level.


A broad tutorial survey of electronic materials initiates the chapter,which then goes on to treat the operation of diodes, transistors, and optical devices. For the most part, the silicon and compound semiconductor devices introduced are those that have been used most broadly in practice.


Instead of mathematical rigor in describing device behavior, equations will be used sparingly and introduced without derivation. Qualitative and intuitive meanings will be emphasized. In doing so it is hoped that the language and terminology used to describe devices will make references to them more understandable later in the book as well as in the reliability literature. Following this, several of the processing steps involved in device manufacture are introduced. Defects and processing problems, the probable


http://dx.doi.org/10.1016/B978-0-12-088574-9.00002-1


All rights reserved. 39


# 2 . Electronic Devices: How They Operate and Are Fabricated


## 2.1 Introduction


sources of a number of reliability concerns, are discussed in the next chapter.


Electrical engineers will probably choose to skip much of this chapter because of its admittedly shallow coverage; however, the latter part dealing with processing may cover new ground. Conversely, the nomenclature and qualitative descriptions of electronic materials and devices may prove instructive to those trained in other disciplines. In either case, several excellent books have been written on the physics of solid state electronic devices [1–5] and on processing technology [6–10] that all readers can beneﬁt from.


2.2 ELECTRONIC MATERIALS


2.2.1 Introduction


At the outset it is important to realize that a very large number of materials have been employed at one time or another in experimental and commercial electronic devices and equipment. They form the sum and substance of active devices and passive components, the packages that enclose them, the substrates and boards on which they are mounted, and the solder and wires that join and connect them. All commercial electronic materials and devices have typically survived a rigorous selection ordeal whose hurdles include:


1. meeting stringent electrical speciﬁcations and requirements,


2. developing reproducible processing and achieving high yields in manufacturing,


3. extensive testing to assure reliable operation.


We are concerned with the properties of these surviving materials and devices and their fates during subsequent use. The survivors, however, are typically but a fraction of the total number of potential candidates that were initially considered. One only has to recall Edison’s experimentation with lamp ﬁlament materials to appreciate what is involved.


A list of the materials employed in commercial electronic devices is entered in Tables 2.1 and 2.2. Although incomplete, the list includes most of the materials addressed in this book. These materials can be conveniently classiﬁed into three categories, namely, conductors, semiconductors, and insulators. Each category is distinguished both by the magnitude of the electrical resistivity as indicated in Figure 2.1 and by the sign of the temperature coefﬁcient of resistivity. By conductors we mean metals with resistivities ranging from 106 to perhaps 104 U-cm. Semiconductor


## 2.2 Electronic Materials


### 2.2.1 Introduction


T a b l e  2.


P h y s i c a l  p r o p e r t i e s  o f  e l e c t r o n i c  m a t e r i a l s


Continued


M e t a l s


M e l t i n g  p o i n t


(


C)


E l e c t r i c a l  r e s i s t i v i t y


U


-c m)


T e m p. c o e f f. r e s i s t i v i t y


e FabricatedElectronic Devices: How They Operate and Ar


a


)


C


D e n s i t y


(g/c m


C o p p e r  1 0 8 3


S i l v e r  9 6 2


G o l d  1 0 6 3


A l u m i n u m  6 6 0


T u n g s t e n  3 4 1 5


P l a t i n u m  1 7 7 2


P a l l a d i u m  1 5 5 2


N i c k e l  1 4 5 5


C h r o m i u m  1 8 7 5


I n v a r (3 6 N i-6 4 F e) 1 4 2 5  8


A l l o y  4 2 (4 3 N i-


5 8 F e)


1 4 2 5  6


K o v a r  1 4 5 0  5


6 3 S n-3 7  P b  1 8 3  1


9 5  P b-5 S n  3 1 0  1


C u-W (2 0%C u) 1 0 8 3


C o S i


5 5 0


T i S i


(C 4 9) 6 5 0


(C 5 4) 8 7 0


W S i


6 5 0


P t S i  3 0 0


C e r a m i c s/g l a s s e s


41


E l


r u


S i l i c o n  d i o x i d e  1 9 8 0


>


A l u m i n u m  o x i d e  2 3 2 3


S i l i c o n  n i t r i d e  2 1 7 3


Metals


(°C)


(Q-cm)


(°C-1)


(g/cm3)


d


|Copper|1083|1083|C o n t i n u e |C o n t i n u e |0.0039|0.0039|
|---|---|---|---|---|---|---|

|8 . 9 3 1 9 . 3 2 . 7 1 9 . 3 2 1 . 5 1 2 . 0 8 . 9 7 . 2 |8 . 0 |8 . 0 |D e n s i t y |D e n s i t y |0.0041|0.0041|

|1 0 . 5 |1 0 . 5 |8 . 1 8 . 3 8 . 4 2 1 1 |8 . 1 8 . 3 8 . 4 2 1 1 |( g / c m 3 ) 2 . 2 3 . 9 3 . 2 |( g / c m 3 ) 2 . 2 3 . 9 3 . 2 |0.0034|

|Aluminum|Aluminum|660|660|2.7x10-6|2.7x10-6|0.0039|

|Tungsten|Tungsten|3415|3415|5.5x10-6|5.5x10-6|0.0045|

|Platinum|Platinum|1772|1772|10.6X10-6|10.6X10-6|0.0039|

|Palladium|Palladium|1552|1552|c o n d c t i v i t y |c o n d c t i v i t y |0.0038|

|Nickel|Nickel|1455|1455|6.8 X 10-6|6.8 X 10-6|0.0069|

|Chromium|Chromium|1875|1875|13x10-6|13x10-6|0.003|

|Invar (36Ni-64Fe)|Invar (36Ni-64Fe)|1425|1425|80X10-6|80X10-6|0.0014|

|Alloy 42 (43Ni- 58Fe)|Alloy 42 (43Ni- 58Fe)|1425|1425|( W / m - K ) |( W / m - K ) |0.0014|

|Kovar|Kovar|1450|1450|T h e m a l 7 3 7 3 0 |T h e m a l 7 3 7 3 0 ||

|0 . 0 0 4 1 |0 . 0 0 4 1 |0 . 0 0 1 4 |0 . 0 0 1 4 |15x10-6|15x10-6||

|0 . 0 0 3 9 0 . 0 0 3 9 0 . 0 0 4 5 0 . 0 0 3 9 0 . 0 0 3 8 0 . 0 0 6 9 0 . 0 0 3 |0 . 0 0 3 9 0 . 0 0 3 9 0 . 0 0 4 5 0 . 0 0 3 9 0 . 0 0 3 8 0 . 0 0 6 9 0 . 0 0 3 |0 . 0 0 1 4 |0 . 0 0 1 4 |19x10-6|19x10-6||

|0 . 0 0 3 4 |0 . 0 0 3 4 |1083|1083|2.5x10-6|2.5x10-6||

|CoSi2|CoSi2|550a|550a|15x10-6|15x10-6||

|TiSi2 (C49)|TiSi2 (C49)|650a|650a|D i e l e c t r i c |D i e l e c t r i c ||

|TiSi2 (C54)|TiSi2 (C54)|870a|870a|c o n s t a n t 9 . 9 7 . 0 |c o n s t a n t 9 . 9 7 . 0 ||

|WSi2|WSi2|650a|650a|3 . 8 |3 . 8 ||

|PtSi|PtSi|300a|300a|35x10-6|35x10-6||

|Melting point Electrical resistivity Dielectric Thermal  conductivity Density Ceramics/glasses (°C) (Q- cm) constant (W/m-K) (g/cm3)|Melting point Electrical resistivity Dielectric Thermal  conductivity Density Ceramics/glasses (°C) (Q- cm) constant (W/m-K) (g/cm3)|Melting point Electrical resistivity Dielectric Thermal  conductivity Density Ceramics/glasses (°C) (Q- cm) constant (W/m-K) (g/cm3)|Melting point Electrical resistivity Dielectric Thermal  conductivity Density Ceramics/glasses (°C) (Q- cm) constant (W/m-K) (g/cm3)|Melting point Electrical resistivity Dielectric Thermal  conductivity Density Ceramics/glasses (°C) (Q- cm) constant (W/m-K) (g/cm3)|Melting point Electrical resistivity Dielectric Thermal  conductivity Density Ceramics/glasses (°C) (Q- cm) constant (W/m-K) (g/cm3)|Melting point Electrical resistivity Dielectric Thermal  conductivity Density Ceramics/glasses (°C) (Q- cm) constant (W/m-K) (g/cm3)|

|Silicon dioxide Aluminum oxide Silicon nitride|1980|>10 x 1015 >10 x 1014 >10 x 1014|1 0 1 4 |7||2.2|

|Silicon dioxide Aluminum oxide Silicon nitride|2323|>10 x 1015 >10 x 1014 >10 x 1014|1 0 1 4 |37||3.9|

|Silicon dioxide Aluminum oxide Silicon nitride|2173|>10 x 1015 >10 x 1014 >10 x 1014|7.0||30|3.2|

Table 2.1


ElectronicDevices:HowTheyOperateandAreFabricated41 Melting point


Electrical resistivity


Temp. coeff. resistivity (x)


Density


C o n t'd


E


l


e


c


t


r


i


Note: Additional properties are listed in Tables 8-2.


aProcessing temperature.


e s i s t i v i t y


of Electronic Materials anReliability and Failured Devices


S i l i c o n  c a r b i d e  3 1 1 0


1 4


3.


A l u m i n u m  n i t r i d e


1 1


B e r y l l i u m  o x i d e  2 5 7 0


2.


9


B o r o n  n i t r i d e


1.


B o r o s i l i c a t e  g l a s s  1 0 7 5


P l a s t i c s


E p o x y-K e v l a r  2 0 0


P o l y i m i d e  2 0 0


E p o x y  F R-4  1 7 5


P o l y i m i d e  3 0 0


1 5


5


T e


ﬂ


o n  4 0 0


Dielectric


Thermal conductivityDensity


Ceramics/


|Silicon carbide|3110|>10 x 1014|42|270|3.2|
|---|---|---|---|---|---|

|Aluminum nitride||>10x1011|8.8|140-230|3.3|

|c o n d u c t i v i t y |2570|>10x1014|6.8|240|2.9|

|Boron nitride||>10 x 1010|6.5|600|1.9|

|Borosilicate glass|1075|>10 x 1010|4.1|5||

|( W / m - K ) 1 4 0 e 2 3 0 ||||||

|T h e r m a l |0 . 2 |0 . 1 6 0 . 1 2 S |3.6|0.2||

|2 7 0 2 4 0 6 0 0 |50 . 3 5 0 . 2 0 . 2 |0 . 1 |4.0|0.35||

|Epoxy FR-4|175a|>10 x 1014|4.7|0.2|1.9|

|Polyimide|300-400a|>10 x1015|3.0-3.5|0.2|1.5|

|Teflon|400a|>10 x 1014|2.2|0.1|2.2|

|Silicone (high-purity)|150a|>10 x 1014|2.7-3.0|0.16||

|c o n s t a n t |3 . 0 e 3 . 5 |2 . 7 e 3 . 0 2 . 6 5 |2.65|0.12S||

|D i e l e c t r i c 4 2 8 . 8 6 . 8 6 . 5 |4 . 1 3 . 6 4 . 0 4 . 7 |2 . 2 ||||

constant


(W/m-K)


S i l i c o n e (h i g h-p u r i t y) 1 5 0


P a r y l e n e  N (v a p o r


d e p o s i t e d)


N o t e: A d d i t i o n a l  p r o p e r t i e s  a r e  l i s t e d  i n  T a b l e s  8


–


P r o c e s s i n g  t e m p e r a t u r e.


D a t a  c o l l e c t e d  f r o m  v a r i o u s  s o u r c e s.


42ReliabilityandFailureofElectronicMaterialsandDevices


42


resistivities depend very strongly on doping level and span a typical range from from 10-3 to 106 Q-cm. However, extremely heavily doped Si has metallic103 to 106 U-cm. However, extremely heavily doped Si has metallic resistivities, while semi-insulating GaAs has a resistivity of w108 U-cm.


Insulator resistivities are the highest of all and can reach values in excess of 1015 U-cm. In electronic applications, insulators are represented by oxides, e.g., SiO2 in IC chips, Al2O3 substrates on which devices are mounted, and polymers, e.g., IC encapsulants and printed circuit boards.


Physically, metals can be distinguished from all other classes of materials


because they become poorer conductors as the temperature is raised,


I refers to indirect band gap.


D refers to direct band gap.


From Refs [1, 11].


1018 1016 1014 1012 1010108 106 104 102110-2 10-4 10-6 10-8●GLASS


GERMANIUM (Ge) SILVER SILICON(Si)


●ALUMINUM NITRIDE


COPPER


DIAMOND


(PURE)


●EPOXY,POLYMIDEGALLIUM PHOSPHIDE (GaP) PLATINUM FUSED


INDIUM PHOSPHIDE(InP)


QUARTZ


11111


10-18 10-16 10-1410-1210-10 10-8 10-6 10-4 10-211102'104106 '108


CONDUCTIVITY σ (Ω-cm)-1


INSULATOR+SEMICONDUCTOR-CONDUCTOR


●TiSi2


GALLIUM ARSENIDE(GaAs)ALUMINUM


Figure 2.1 Electrical resistivities of electronic materials.


Electronic Devices: How They Operate and Are Fabricated 43


|Table 2.2 Properties of Lattice |Table 2.2 Properties of Lattice |elemental and Melting |elemental and Melting |compound Energy |semiconductors Electron |
|---|---|---|---|---|---|

|Material |parameter (nm) |point (K) |gap (eV at 25 C)|mobility (cm2/V-s) |mobility (cm2/V-s |

|Diamond |0.3560 |w4300 |5.4 |1800 |1400 |

|Si |0.5431 |1685 |1.12 I |1450 |450 |

|Ge |0.5657 |1231 |0.68 I |3600 |1900 |

|ZnS |0.5409 |3200 |3.54 D |120 |5 |

|ZnSe |0.5669 |1790 |2.58 D |530 |28 |

|CdS |0.5832 |1750 |2.42 D |340 |50 |

|AlAs |0.5661 |1870 |2.16 I |1200 |420 |

|GaP |0.5451 |1750 |2.26 I |110 |75 |

|GaAs |0.5653 |1510 |1.43 D |8500 |400 |

|InP |0.5869 |1338 |1.27 D |4600 |150 |

|InAs |0.6068 |1215 |0.36 D |30,000 |460 |

implying a positive temperature coefﬁcient of resistivity. Conversely,semiconductors and insulators become better conductors as they become hotter. Even here there are rare exceptions to the rule over small temperature excursions.


2.2.2 Semiconductors


2.2.2.1 Structure


Semiconductors and the devices based on them are a primary focus of the book. Some, but certainly by no means all, of the reasons for device failure and reliability problems can be attributed to malfunction of semiconductors.


The special attributes of semiconductors derive from both their physical and electronic structures. In Figure 2.2 the crystal structures of both Si and GaAs,the two most important semiconductors used in electronics, are depicted.


Silicon has a diamond-cubic structure that is derived from the face-centered cubic lattice but with a two-atom motif per lattice point; this means that there are eight atoms per unit cell. On the other hand, in GaAs the Ga and As atoms alternate as shown within the basic diamond cubic lattice.


In cubic structures there are three important crystallographic planes and directions. The (100) planes are the cube faces and the [100] directions are the cube edges. Planes passing through diagonally opposite cube edges have(110) indices, while (111) planes pass through three diagonally opposite cube corners. The [110] directions are those between the cube center to the midpoint of each of the 12 cube edges; similarly, [111] directions radiate from the cube center to each of the eight cube vertices. Almost every semiconductor electronic device requires either bulk or thin ﬁlm semiconductor single crystals of high crystallographic perfection, except amorphous thin ﬁlm transistors, used in LCDs (liquid crystal displays).


Critical to many of the structural and electronic properties of elemental Si is the tetrahedral atomic grouping, in which each atom is surrounded by four identical atoms. The bonds between atoms, represented by lines, are covalent in nature, reﬂecting the fact that a pair of outer electrons, one from each of the neighboring atoms, comprises the bond. Covalent bonds are typically strong and resistant to deformation. This accounts for silicon’s appreciable hardness, relatively high Young’s modulus, lack of ductility, and high melting point. Although covalent bonds are mechanically strong, the bonding, or valence, electrons within them can be easily detached at relatively low temperatures to become more energetic conduction electrons.


Holes, with an effective positive charge, are then left behind in the broken valence bonds.


Both holes and conduction electrons can readily move under the in-ﬂuence of electric ﬁelds. The semiconductor property known as mobility


(m) is deﬁned as the ratio of the carrier velocity to the applied electric ﬁeld and has units of (cm2/V-s). Mobility values for carriers in semiconductors are listed in Table 2.2. Undesirable reductions in carrier mobility occur in the presence of impurities and lattice defects. The combination of carrier concentrations and velocities inﬂuences and limits all electrical conduction phenomena.


Figure 2.2 (a) Diamond cubic crystal structure of silicon. (b) Model of the zinc blende crystal structure of GaAs. Both Ga and As populate face-centered cubic lattices that interpenetrate one another.


Electronic Devices: How They Operate and Are Fabricated 45


2.2.2.2 Bonds and Bands


2.2.2.2.1 Bonds


Several representations of electronic structure have evolved over the years as aids in interpreting the behavior of semiconductor materials and devices.


The simplest of these, depicted in Figure 2.3, is a physical-bonding model where the tetrahedra are ﬂattened to two dimensions, and each bond between atoms now represents a couple of shared valence electrons.


Introduction of n-type dopants (P, As, and Sb) and p-type dopants (B, In,and Al) into the Si lattice creates extra donor electrons and extra acceptor holes, respectively. Through doping, the number of electron and hole charge carriers can be dramatically enlarged in a controllable way. In this model, conduction electrons hop around in the open spaces between bonds; holes, on the other hand, are conﬁned to, and migrate through, the


Figure 2.3 (a) Representation of a two dimensional silicon lattice containing donor(Pþ5) atoms. (b) Two-dimensional silicon lattice containing acceptor (Bþ3) atoms. Each bond consists of two valence electrons. Direction of carrier motion in electric ﬁeld E is shown.


bond network. An applied electric ﬁeld causes these charge carriers to move in opposite directions. Keep in mind the semiconductor does not possess an excess of charge, but rather is effectively neutral and macroscopically uncharged.


2.2.2.2.2 Bands


The electronic structure of undoped as well as doped semiconductors is popularly represented in terms of the energy band diagrams of Figure 2.4.


When isolated atoms of Si are brought together to form the solid,individual electron energy levels collectively broaden to create bands containing an astounding 1022 or so distinct levels (one for each electron)per cubic centimeter. They are packed so tightly that the energy difference between the highest and lowest levels is only a few electron volts. Thus all of the electrons comprising valence bonds form the valence band, and all of the conduction electrons enter the conduction band. The energies of electron levels within states are noted on the ordinate, while the horizontal axis can be loosely identiﬁed with some macroscopic lattice distance having much larger than atomic dimensions. A key feature of this diagram is the energy gap(Eg) that separates valence and conduction bands. In Si, Eg¼ 1.12 eV, whilein GaAs, Eg¼ 1.43 eV at 300 K. Electron energy levels and states withinthe energy gap are forbidden in pure, structurally perfect Si. Any perturbation (e.g., dopant atom, impurity located either on lattice or interstitial


Figure 2.4 Electron energy band diagrams for semiconductors, metals, and insulators,


(a) n-type semiconductor. (b) p-type semiconductor. Largely ﬁlled valence band lies below EV and largely empty conduction band-lies above EC. The Fermi level lies closer to EC in the n-type semiconductor and closer to EV in the p-type semiconductor. (c)Band diagram of a metal. The uppermost occupied electron state in the distribution corresponds to the Fermi level, above which there are always accessible empty electron states. There is no energy gap in metals. (d) Band diagram for insulators.


Electron energy gaps range from 5 to 10 eV.


Electronic Devices: How They Operate and Are Fabricated 47


sites, vacancy or dislocation defects, precipitates) that disturbs this ideal order is reﬂected in the creation of new quantum states with characteristic energy levels. Such states usually fall somewhere in the gap.


On this basis it is easy to see that ﬁlled n-type dopant donor states(Figure 2.4(a)) lie close to the bottom of the conduction band, to which they readily donate electrons. Similarly, empty p-type dopant acceptor states (Figure 2.4(b)) lie just above the top of the valence band, where they accept electrons, leaving holes behind in the process. In essence, this is how electrical conduction occurs in semiconductors. An energy level of interest that reﬂects the probability of carrier population of states is known as the Fermi (EF) level. It is deﬁned to be the energy level whose probability of occupation is 0.5. In n- and p-type semiconductors, EF lies closer to either the conduction (EC) or valence (EV) band edges, respectively, but usually within the gap.


Band diagrams are helpful in distinguishing the behavior of semiconductors from those of metals and insulators. In metals (Figure 2.4(c)) the Fermi level caps the electron distribution. Below it all levels are occupied by electrons, and above it they are unoccupied. It takes very little energy to access these closely spaced empty levels if the electrons are stimulated electrically, thermally, and optically; this accounts for the excellent electrical and thermal conductivity as well as high reﬂectivity of metals. Band diagrams for insulators (Figure 2.4(d)) resemble those for semiconductors,except for the larger electron energy gaps ranging from 5 to 10 eV.


2.2.2.2.3 Energy–Momentum Representation


Another widely used representation of semiconductor bands is shown in Figure 2.5(a) and b. Here the energy (E) of electron states is plotted as a function of the magnitude and direction of the electron momentum, or equivalently, versus wave vector (k). The resultant parabola-like E vs k curve is important because it provides a useful way to distinguish between Si and Ge on the one hand, and GaAs and similar compound semiconductors on the other [1]. While the former are known as indirect bandgap semiconductors, the latter are direct band-gap semiconductors. Only direct-gap semiconductors are useful in optical devices like light-emitting diodes (LED) or lasers. Photons of the band-gap energy are emitted when electrons descend from the bottom of the conduction band to recombine with holes at the top of the valence band. The transition between the two involved states must conserve electron momentum.


Similarly, when a photon whose energy is equal to or greater than the gap


2.2.4 Insulators


We have already noted that in the scheme of conductors, metals and insulators are at opposite extremes, with semiconductors occupying a broad middle ground. When the latter are very pure or lightly doped, they have high resistivities, and their dielectric character is emphasized. Interestingly,similarities between semiconductors and insulators exist. Energy gaps exist in both, and the response of conductivity to doping and temperature is similar. Insulators are used to isolate conducting regions at different electric potentials so that no current ﬂows between them. They also serve vital dielectric functions that enable circuits to store charge in capacitors that behave as memory elements. High dielectric constant ferroelectric ceramics such as BaTiO3 are important in this regard for potential inclusion in memory chips. Dielectric property change upon cyclic electrical stressing is a concern, however.


The insulating materials we are primarily concerned with are oxides (e.g.,SiO2, Al2O3) and polymers. Invariably these insulators have amorphous structures. Interestingly, solid insulators are not the only ones of interest in electrical equipment. Transformer oil is an example, and its breakdown is an important consideration in the reliability of very high voltage equipment. On the IC chip level, thin ﬁlms and coatings of silicon dioxide, silicon nitride,and silica-based glasses are used in assorted insulating, dielectric, processing,and device passivation roles. These ﬁlm materials are deposited at relatively low temperatures by both physical and chemical vapor deposition techniques. The most important insulator in this book is SiO2 because it plays critical roles in two important diverse electronic technologies, for quite different reasons. Not only does SiO2 serve as the thin ﬁlm gate insulator inﬁeld effect transistors, but in ﬁber form it is the medium through which light propagates in optical communications systems. In these applications it has been the focus of dielectric as well as mechanical breakdown investigations that will be respectively discussed in Chapters 6 and 10.


Since insulators have very few electron and hole carriers, conduction by these carriers is limited, a fact due to the large value of Eg. Thin oxide and glass ﬁlms are actually quite a bit more conductive than bulk insulators. For one thing, due to a lack of crystal perfection, there are fuzzy electrondistribution tails at both the top of the valence band and the bottom of the conduction band. These extend into the normally state-free gap and overlap to create a broad continuum of electron states. Secondly, the metal electrode contacts, due to the metal workfunction1, inﬂuence the nature of electron injection into the insulator. Lastly, because dimensions are small,modest applied voltages all too often lead to large electric ﬁelds that, in turn,may foster nonlinear conduction behavior, charge trapping, and sometimes breakdown. Later, in Chapter 6, other conduction mechanisms will be introduced. Questions of how electrons interact with matrix atoms and other electrons in the insulator to generate damage will be addressed then.


2.3 DIODES


2.3.1 The p–n Junction


The fundamental building block of most semiconductor devices is the p–n junction, i.e., p and n doped regions joined at a junction. Diodes contain one such junction, transistors two, and there are devices that have three or


1Energy necessary to free an electron from the Fermi Level in the metal to vacuum.


Electronic Devices: How They Operate and Are Fabricated 55


## 2.3 Diodes


more junctions. Understanding the operations of rectiﬁcation, ampliﬁcation, and switching implies some knowledge of junction behavior.


Immediately after p and n doped regions come into contact or are shorted together, holes and electrons rapidly traverse the junction and, as shown in Figure 2.8(a), three things happen.


1. Carrier equilibrium results in equalization of the respective Fermi levels.


2. A built-in electric contact potential (V0) or ﬁeld (E) is established that discourages any further charge transport.


3. In effect, a space charge or depletion region (a kind of dielectric, carrierfree zone) develops.


The extent of the space charge region varies inversely with doping level.


When the latter is high, the material is highly conductive and cannot


Figure 2.8 Energy band representation of a semiconductor p–n junction under different conditions of bias. (a) Zero bias voltagedThe Fermi levels are equilibrated on both sides of the junction, creating an internal electric ﬁeld. (b) Reverse biasdThe Fermi levels are displaced as carriers are depleted from the junction region. A small reverse current ﬂows. (c) Forward biasdLarge forward current ﬂows as carriers recombine at the junction.


support high electric ﬁelds. Just the opposite is true at low doping levels.


Thus, devices that function at low voltages are generally more highly doped than those exposed to high voltage levels.


Importantly for device behavior, the internal barrier to charge ﬂow can be manipulated by applying an external bias voltage. When the diode is reverse biased by connecting n to the positive supply voltage (V) and p to the negative supply voltage (Figure 2.8(b)), all of the p-type Si electron levels, including the Fermi level, rigidly rise relative to the n-type Si levels by an amount qV. Electrons and holes are drawn away from the junction in the respective n and p regions. We speak of a depletion region free of carriers. This has the effect of widening the space charge region as well as raising the magnitude of the potential barrier and electric ﬁeld across the junction. As a result, only a very small reverse current (iR) ﬂows. Alternatively, when the diode is forward biased by connecting n to the negative supply voltage and p to the positive supply voltage (Figure 2.8(c)), electron levels in the two semiconductors now rigidly shift in the other direction relative to each other. Electrons and holes now readily ﬂow across the junction where the carriers recombine. This has the effect of reducing the space charge region as well as lowering the magnitude of the potential barrier and electric ﬁeld across the junction. Importantly, electron–hole recombination means a large forward current (i). The p–n junction thus enables currents of vastly differing magnitude to ﬂow by simply changing the bias voltage polarity. This is the behavior desired of rectiﬁers. In contrast, ohmic characteristics are linear and display the same current magnitudes, but of opposite sign, when the voltage polarity reverses.


The ideal junction characteristics, depicted in Figure 2.9, are succinctly governed by an equation that describes the current–voltage variation as.


i ¼ iRexpqVkT 1;


(2.4)


where q is the electronic charge, and kT has the usual meaning. Although DC operation has been described, junctions in devices generally function under ac transient conditions. This causes voltages, currents, and internalﬁelds to be time dependent.


2.3.2 Contacts


When metal contacts are applied to the p and n semiconductor regions,low-resistance ohmic behavior is normally desired. The band diagram for


Electronic Devices: How They Operate and Are Fabricated 57


an idealized ohmic contact is shown in Figure 2.10(a). In practice, however,ohmic contacts are prepared by heavily doping the underlying semiconductor in order to minimize its resistivity. This considerably narrows the region of band bending, promoting bidirectional tunneling of charge across the metal–semiconductor interface (Figure 2.10(b)), and resultant linear i–V behavior.


In addition, metal–semiconductor contacts can also display nonlinear or rectifying characteristics, resulting in unexpected changes in circuit behavior. Schottky-barrier or metal–semiconductor diodes are based on the rectifying properties of certain metal contacts to semiconductors. If a band diagram is drawn for a metal with a work function larger than that of the n-type semiconductor it contacts; the resultant structure of Figure 2.11 behaves very much like the p–n junction diode of Figure 2.8 upon biasing.


There is, of course, no band bending in the metal. A barrier potential of height FB now governs the asymmetric transport of charge across the junction. Despite the fact that the i–V characteristics appear identical,Schottky-barrier and p–n diodes differ in one signiﬁcant way. Under forward bias, majority electrons injected over the barrier are hotter than normal electrons in the metal. Their excess energy is very rapidly quenched,and such thermalized electrons cannot ﬂow back into the semiconductor upon reverse bias because they face a large energy barrier in that direction.


The short recovery time of 1011 s makes Schottky diodes capable of very fast switching in microwave circuits.


Figure 2.9 Ideal and nonideal i–V junction characteristics.


EV


Figure 2.10 (a) Band diagram representation for an idealized ohmic contact between a metal and semiconductor. (b) Band diagram for an ohmic contact illustrating tunneling. FM and FS are respective work functions.


baW


，


qTs


号


EC


Ef


Figure 2.11 Band diagram for idealized Schottky-barrier contact between a metal and semiconductor.


Electronic Devices: How They Operate and Are Fabricated 59


)e(


Evacuum


q中s


qPM


Ec


↑baw


日


Ec Et


Applications normally require either ohmic or Schottky behavior;interestingly, certain compound-semiconductor ﬁeld-effect transistors contain both ohmic and Schottky contacts (Section 2.7.4). Irrespective of whether they are ohmic or rectifying, solid-state reactions between Al contacts and silicon as well as assorted metals (e.g., Au, Ti) and GaAs have been troublesome sources of degradation and failure in devices. These reliability problems are exacerbated when high current densities ﬂow through contacts.


2.3.3 Deviations from Ideal Junction Behavior


There are a number ways that actual junction behavior differs from the ideal.


2.3.3.1 Characteristics


Rather than by Eqn (2.4), diode i–V characteristics are more nearly


described by i ¼ iRexpqVnkT 1, where n, the ideality factor, varies between 1 and 2. In addition, the contact potential due to work function differences between the involved semiconductors makes the i–V forward characteristics appear to be more squarish. Thus, very little forward currentﬂows until a critical voltage somewhat below Eg is applied, after which the current rises very steeply.


Several effects serve to weaken rectifying behavior, resulting in the deviations from good i–V characteristics displayed in Figure 2.9. Ohmic losses in diodes are manifested by passage of less current at high forward bias levels. Carrier generation outside of the junction region means higher reverse currents. These effects cause the diode to be more resistive and display linear i–V behavior as a limiting case. In poorly made diodes the reverse current may sometimes have a surface component that leaks around the junction. Charged contaminants and semiconductor surface states foster electrical leakage paths. The proportions of bulk and surface currents depend on the electrical character of the junction at the point where the bulk meets the surface. Passivating Si diodes with SiO2 layers minimizes such leakage. In good diodes the reverse current remains very small and then sharply increases at the point of breakdown, a subject discussed in the next section. Such characteristics are “hard,” distinguishing them from the“softer” i–V behavior exhibited by junctions possessing weak spots where localized breakdowns cause excessive leakage current.


Finally, there are the characteristics of the open diode that passes no current irrespective of voltage, and the shorted diode through which large currents ﬂow because the device has a low resistive value and is not rectifying.


2.3.3.2 Breakdown


Diode breakdown is much less alarming than it sounds and does not necessarily mean damage. When the applied reverse voltage is increased beyond certain limits (Figure 2.9) diodes undergo breakdown. Depending on doping level, electric ﬁelds in the junction ranging from 200 to 1000 kV/cm can develop in Si. Under such conditions minority carriers that produce the usual reverse or leakage current are accelerated to kinetic energies high enough for them to ionize matrix atoms upon collisional impact. In the case of a single incident electron, two electrons (the original one and the impacted valence electron) will now reside in the conduction band after collision. Each can impact-ionize lattice atoms repeatedly, and with sufﬁcient electron multiplication, avalanche breakdown may occur. The reverse current rises to a value limited only by the external resistance of the circuit. In this state it may operate satisfactorily as a reverse-biased diode.


However, if the reverse current is excessive, the junction can overheat,causing the diode to burn out. Zener diodes capitalize on operation in the breakdown state and are used as voltage references in rectiﬁer and control circuits.


2.3.3.3 Punch-throughs


Although the term sounds as ominous as breakdown, punch-through is not necessarily threatening to continued diode function. Punch-through occurs when lightly doped regions are also physically thin. Upon reverse biasing,the depletion region widens and may extend directly to the ohmic contact,thus shorting out the diode or transistor. Provided that the current ﬂow is limited by the circuit resistance and no overheating occurs, the diode will recover its former properties when the reverse voltage is reduced. As we shall see later, punch-through also occurs in transistors.


2.4 BIPOLAR TRANSISTORS


2.4.1 Transistors in General


Transistors are the most important solid-state devices. Because they are also the most numerous, device reliability and failure issues tend to be


Electronic Devices: How They Operate and Are Fabricated 61


## 2.4 Bipolar Transistors


overwhelmingly focused on them. Since transistors contain two p–n junctions, have three contacts or terminals, are complex geometrically, and frequently require the action of perpendicular electrical ﬁelds, their behavior is more difﬁcult to understand than that of diodes. To complicate matters further there are two fundamentally different types; in the bipolar junction transistor (BJT) current is ampliﬁed, while in the ﬁeld effect transistor (FET) a voltage controls a current. The former relies on the participation of both types of carriers, hence the descriptor “bipolar.” In contrast, only one carrier plays a prominent role in FETs. Transistors perform the basic electrical functions of ampliﬁcation and switching in both discrete and IC conﬁgurations involving low as well as large power applications.


With regard to function it is helpful to distinguish between linear and on–off digital logic circuits. Linear circuits typically operate with low input voltage levels of perhaps w1 mV or so (e.g., audio equipment) and outputs having small deviations about a quiescent operating DC level. Digital circuits are constrained to operate at ﬁxed voltage levels (e.g., 0 or 5 V) and are impervious to noise levels that would present difﬁculty in linear circuitry. The latter are much less tolerant of variations in electrical component characteristics than is the case for digital circuits. With change in operating temperature, linear circuits may drift in and out of speciﬁcations, whereas digital circuits will either function properly or abruptly fail.


Both BJTs and FETs are used in linear and digital circuits; computer logic and memory circuits are primarily composed of FETs, however, and these therefore dominate the transistor market.


2.4.2 Bipolar Junction Transistors


2.4.2.1 Operation


It is common to start discussions of BJTs with the p–n–p type shown in Figure 2.12 because the direction of majority carrier (hole) motion coincides with that of the current ﬂow. There is also an n–p–n version of this device that is easier to fabricate. Because the electron mobility in Si(me¼ 1450 cm2/V-s) is some three times higher than for holes, these fastern–p–n devices are preferred in most applications. By reversing the doping type, bias voltages, and current direction, the treatment applies to n–p–n devices as well. These three-terminal devices contain two junctions separating three semiconducting regions, i.e., the emitter, base, and collector. In the case under discussion these are doped p, n, and p, respectively, and are wired together in a common base conﬁguration. When unbiased, the Fermi


levels line up across the band diagram representation of the device(Figure 2.12(a)).


During transistor operation the p–n junction on the left is forward biased, while the one on the right is reverse biased. The bands bend and move up or down as shown (Figure 2.12(b)). First the heavily doped emitter injects majority (hole) carriers into the lightly doped base region.


There the holes become minority carriers and would normally recombine with majority electrons. However, because the base is lightly doped and made very thin (e.g., 1 mm thick), holes diffuse right through it before they have a chance to recombine. Those holes that traverse the base–collector interface are now efﬁciently swept to the collector contact; equivalently,holes ﬂoat uphill on the band diagram, which is their way of reducing energy.


In well-designed transistors the collector current, iC, is only slightly smaller than the emitter current, iE; for example, iB is typically 1% of iE or iC. Therefore, the common base current gain, deﬁned as a¼ iC/iE, isslightly less than unity. It is not difﬁcult to calculate the AC power gain in the circuit shown in Figure 2.12(c). Due to the exponential character of Eqn (2.4), a small change in emitter–base voltage (DVEB) will cause a large change (DiE) in emitter current. The power supplied to the forward-biased emitter junction, whose resistance is RE, is RE(DiE)2. Likewise, the power delivered to the load resistor RL is RL(DiC)2, where DiC is the change in


Figure 2.12 (a) Band diagram representation of a p–n–p bipolar junction transistor in the common base conﬁguration. Under zero bias, the Fermi levels line up across both junctions. (b) Band diagram representation of transistor under forward bias. (c) Transistor with bias voltages VF and VR applied.


Electronic Devices: How They Operate and Are Fabricated 63


collector current. Because DiE and DiC are approximately equal, the power gain (G) is simply.


G ¼ RLðDiCÞ2REðDiEÞ2zRLRE:


(2.5)


Typically, for RE¼ 25 U and RL¼ 10 kU, a value of G equal to 400 can be anticipated.


Transistor action essentially occurs because the emitter–base voltage in one part of the device controls the collector current elsewhere in the device. In this way small changes in the current at one terminal enable the current through the other two terminals to be controlled. Similar transistor action occurs in other wiring conﬁgurations, e.g., common emitter. Speciﬁc doping levels and base dimensions are required for optimal transistor performance.


2.4.2.2 Planar Bipolar Transistor


Discrete, or single bipolar, transistors of the type just discussed were the ﬁrst to reach the market. Later the concept of integrating many bipolar transistors on a single wafer meant a new processing philosophy. Rather than stacking bulk semiconductor regions “side to side” as in Figure 2.12, a “top to bottom” thin ﬁlm technology was adopted. By sequentially doping through the wafer thickness, the n–p–n (or p–n–p) junction depths, and the base thickness in particular, can be very well controlled. The problem is how to make contact to the emitter, base, and collector regions. Obviously,contacts can only be made on the top surface of the wafer. Novel methods have been developed to direct the current ﬂow, as shown in Figure 2.13.


Electrons injected from the emitter cross the narrow base region vertically down into a highly conducting, heavily doped buried layer that serves as a horizontal extension of the collector. They ﬂow laterally through the buried layer and then veer up to the collector contact at the top surface.


energy is absorbed, momentum conservation governs the electron ascent between the corresponding valence and conduction band states. In direct band-gap materials like GaAs and InP these electron descents and ascents are vertical, conserving momentum; but in Si and other indirect semiconductors the transitions are “slanted” and involve momentum changes that effectively excite lattice vibrations which heat the solid. These wasteful processes dramatically reduce the probability that photons will either be emitted or absorbed during respective electron–hole recombination or generation.


2.2.2.3 Compound Semiconductors


The important III–V compound semiconductors are derived from atomic combinations arising from columns III A (e.g., Al, Ga, In) and V A (e.g., N,P, As) of the periodic table. Other II–VI compound semiconductors are composed of elements from columns II B (Zn, Cd, Hg) and VI A (S, Se,Te). A summary of the electrical properties of elemental and compound semiconductors is reproduced in Table 2.2, where lattice parameters,


Figure 2.5 Energy (E) versus wave vector (k) representation of band structure. (a)direct band-gap semiconductor. (b) indirect band-gap semiconductor.


Electronic Devices: How They Operate and Are Fabricated 49


energy gaps, and mobilities are indicated for the more widely used materials. Ternary (3 atom) and quaternary (4 atom) semiconductors are also widely used in electro-optical applications. For example, AlGaAs ternaries are derived from AlAs and GaAs mixtures. Similarly, InGaAs and GaInAsP devices used in optical communications can be understood as combinations of binary compounds, e.g., GaAs and InAs, and GaAs and InP. In many instances the resultant ternary energy gap and lattice parameter values are simply weighted averages derived from the constituent binaries. Thus by alloying GaAs and GaP, families of light-emitting diodes with compositions GaAs1  xPx become available, provided that the ternary semiconductoralloys are still direct-gap materials. For x¼ 0.4, interpolation yields anenergy gap of 1.9 eV, which from Eqn (2.1) below corresponds to the red portion of the spectrum.


When ﬁlms of AlxGa1  x As deposited on GaAs substrates, or InGaAs deposited on InP, are involved, it is essential that the ﬁlm be epitaxial. This means that ﬁlm and substrate must be “lattice matched” or have as nearly identical lattice parameters as possible. Otherwise, defects that severely limit device function will tend to be present at the ﬁlm–substrate interface.


Typically, mismatches in lattice parameter of no more than 0.1% can be tolerated.


2.2.2.4 Electrical and Optical Function


Semiconductors have several unique properties that enable them to exhibit unusual electrical and optical effects. Like metallic conductors they possess sufﬁcient numbers of high-mobility charge carriers to pass large currents. Unlike conductors, but like insulators, they are capable of supporting large electric ﬁelds; this happens at p–n junctions under reverse bias where charge carriers are depleted. Remarkably, in semiconductor devices either attribute can be emphasized in applications requiring rectiﬁcation (diode) and ampliﬁcation (transistor) of current, or storage of charge (metal oxide semiconductor capacitor). The application of the requisite bias voltages to the device serves to control the magnitude of current ﬂow.


Optical activity is possible in semiconductors because they possess an important pair of electron levels which span the energy gap. Many states of very nearly the same energy are either full or empty at levels near the bottom of the conduction band and the top of the valence band; thus electron transitions can readily occur. The wavelength (l) associated with the band-gap energy is derived from the well known Planck equation,


E¼ hc/l (i.e., Eg¼ hc/l), where h is Planck’s constant and c is the speed oflight. A useful formula connecting Eg and l is.


lðmicronsÞ ¼ 1:24EgðeVÞ:


(2.1)


Three basic types of electro-optical phenomena can be simply understood by referring to Figure 2.6. Depicted are the valence and conduction bands of the involved semiconductor or active electro-optical medium, and the radiative transitions that occur between energy levels in them. Either photons or electronic signals can trigger mutual electro-optical responses at p–n junctions.


1. Stimulated absorption of incident photons (Figure 2.6(a)) excites electrons from the valence to the conduction band, generating mobile carriers or an electric signal. After photon detection (e.g., by a photodiode) electron circuitry is activated to amplify the signal, or deliver external power(e.g., a solar cell).


2. The reverse process of photon emission occurs during deexcitation of electrons from the conduction-to-valence band (Figure 2.6(b)). In light-emitting diodes (LED), for example, the emission is triggered by an electric current that passes through the junction causing electron–hole recombination and a corresponding spontaneous emission of monochromatic light. The light can now be viewed directly in a


Figure 2.6 Basic electron transitions between valence and conduction bands in semiconductors shown within the context of junction devices. (a) Stimulated absorption. (b) Spontaneous emission. (c) Stimulated emission.


Electronic Devices: How They Operate and Are Fabricated 51


display, or made to pass through lenses of an optical system, or enter an optical ﬁber.


3. The last case (Figure 2.6(c)) combines features of the previous two.


Through absorption of light (pumping), electrons ascend from the valence band to an excited state, causing a normally unnatural, inverted population of electron levels. Incident photons that impinge on such excited atoms may now induce stimulated emission of photons from them. These photons have the same energy and phase as those that excited them in the ﬁrst place. If instead of allowing the light to exit the medium it is made to reﬂect back and forth in phase, while impinging on other atoms in excited states, the light intensity is ampli-ﬁed. This is the basis of laser action.


Just how the electro-optical effects are capitalized upon in actual devices is addressed later in the chapter.


2.2.3 Conductors


Conductors are used in circuits to speed the transmission of electronic signals from where they are generated to where they are processed, e.g.,detected, ampliﬁed, stored, or displayed, without distortion or any loss of information. In solid-state circuits this means that conductors must ﬁrst make low-resistance contact to various n and p doped regions, and gate electrodes of devices, and then be connected to other active devices and passive components via a network of interconnections. The latter are found in great profusion on the IC chip itself as well as at the (packaging) interface between the chip and the outside world. Degradation of both contacts and interconnections may alter the ﬁdelity of the intended signal by changing its amplitude, time constant, sign, and shape; frequently, open circuiting is theﬁnal manifestation of conductor degradation.


Properties required of conductors include high electrical conductivity(to minimize both Joule heating and RC time constants), chemical stability(absence of corrosion), ability to be easily processed into required shapes with desired dimensions, compatibility with other device processing and fabrication steps, and lastly, resistance to loss of dimensional and physical integrity due to stress or the passage of large current densities (electromigration). Because the conductivity requirement is often the critical one,conductors are usually limited to metals. These materials have face-centered and body-centered cubic crystal structures for the most part. Unlike semiconductors, in all practical applications metals are polycrystalline.


Relevant properties of metals are given in Table 2.1.


Of the 80 or so metallic elements only a few (e.g., Al, Cu, Au, Ag) have seen extensive use in commercial electronic devices and systems. On IC chips, interconnections are basically limited to Al, Cu and Al alloy (Al–Cu,Al–Cu–Si) metallizations at any given level, and to W/TiN via combinations to connect levels. But, when contacts to semiconductors and external connectors are considered, a much richer assortment of metals, alloys(Ti–W, PdSi, Sn–Pb solder), and intermetallic compounds (TiSi2) is utilized. Metal contacts and interconnections at several levels within ICs are schematically indicated in Figure 2.7 together with typical sites and types of degradation.


Metals are good conductors of electricity because they contain huge numbers of free or conduction electrons; i.e., Cu has 1 and Al has 3 per atom, so we are dealing with w1022 per cm3. Their band structures are complex, but importantly, metals possess either overlapping valence and conduction bands or an unﬁlled conduction band. Further, the absence of energy gaps means that electrons never face any appreciable barrier in accessing the numerous, closely spaced, empty higher energy states under the stimulus of an applied electric ﬁeld or incident photon. Two simple relationships govern the resistivity, r, of metals:


rTotal ¼ rT þ ri þ rd


(2.2)


and


r ¼ r0ð1þ aDT Þ:


(2.3)


Figure 2.7 A schematic of the variety of metal contacts and interconnections (shown in cross-hatch) in integrated circuits together with typical degradation phenomena and sites of occurrence.


Electronic Devices: How They Operate and Are Fabricated 53


The ﬁrst is a statement of Matthiessen’s rule (Eqn (2.2)), which reﬂects the fact that the total resistivity of a metal has three contributions:


1. a thermal one, rT, which increases linearly with temperature in the vicinity of 25 C. Since rT generally dominates the other two contributions in this temperature range, Eqn (2.3) describes the observed resistivity (r) of metals for all practical purposes. In this formula r0 is the resistivity at 25 C, a is the temperature coefﬁcient of resistivity, and DT is the difference in operating temperature relative to 25 C.


2. ri, the resistivity due to atomic impurities (dissolved or in compound form).


3. rd, the resistivity due to defects.


Alloying always increases the resistivity of the base metal. But compared to orders of magnitude change in semiconductor resistivity with minute doping levels, metals suffer relatively little conductivity loss with much larger alloying additions. Lattice defects such as vacancies, dislocations, and grain boundaries raise the resistivity of metals, but only slightly. When impurity or defect concentrations are small, their effect on the total resistivity can be measured only at cryogenic temperatures, where the thermal contribution (rT) is very small by comparison, i.e., frozen out.


During arcing or Joule heating the conductivity of metals may degrade due to oxidation or interdiffusion reactions that cause extensive compositional change. Interconnections suffering electromigration damage invariably show an increase in resistance.


Logic functions can also be carried out more efﬁciently by ﬁeld effect transistors, and it is to these devices that we now turn our attention.


2.5 FIELD EFFECT TRANSISTORS


2.5.1 Introduction


Like BJTs, ﬁeld effect transistors (FETs) are three terminal devices; unlike them, a gate voltage rather than a current controls the current at the other two terminals. Field effect transistors are easily the most widely used of all solid-state devices. They currently dominate computer logic as well as memory integrated circuit chips and are projected to widen this dominance.


At the outset, two distinct types of ﬁeld effect transistor must be distinguished. The ﬁrst and most important is the MOS type, where the metal(M) gate electrode is separated from the semiconductor (S) by a thin


Figure 2.13 Schematic of the planar n–p–n bipolar transistor structure utilizing oxide isolation. The current path from emitter to base to collector is indicated. From Ref. [7].


Electronic Devices: How They Operate and Are Fabricated 65


## 2.5 Field Effect Transistors


### 2.5.1 Introduction


insulator ﬁlm (i.e., SiO2). Voltage applied to the gate controls the currentﬂow between underlying semiconductor regions (source and drain) by either creating or eliminating a conducting channel. Junction ﬁeld effect transistors (JFET) are the second type, and they function by applying a gate voltage to vary the depletion width of a reverse-biased p–n junction.


2.5.2 The MOS Capacitor


Knowing how the MOS capacitor structure responds to applied voltage is prerequisite to understanding MOS ﬁeld effect transistor (MOSFET)behavior. This capacitor structure, which is the essential building block of silicon MOSFETs as well as charge-coupled devices, actually consists of two capacitors in series. The ﬁrst has a ﬁxed value of capacitance determined by the thin SiO2 ﬁlm sandwiched between planar metal (or other conductor,e.g., polysilicon or silicide) and semiconductor surface. Underlying this is the capacitance associated with Si, which varies depending on the extent of charge depletion in the semiconductor. Now consider the “ideal” MOS structure for p-type Si, shown in Figure 2.14(a). With no gate voltage or bias applied, Fermi level equilibration leaves all bands horizontal, or ﬂat; this condition arises when the work functions of the metal and semiconductor are the same, and there is no oxide charge (which we assumed for this illustration). When a negative gate voltage (–VG) is applied to the metal, the energy of all of its conduction electrons is raised uniformly by an amount qV relative to Si. Holes are attracted to the Si/SiO2 interface, making Si there appear to be even more p-type than originally. This causes band bending at the interface (Figure 2.14(b)), which graphically describes a state known as accumulation. The high interfacial hole density effectively serves to make the Si a positively conducting capacitor plate. For high VG values, the MOS capacitance (Co), which depends inversely on SiO2 thickness, is large and solely due to the oxide.


As the polarity of VG is reversed, the overall capacitance decreases. The reason is that holes are repelled from the Si/SiO2 interface. In this depletion regime Si acts like a dielectric with a capacitance governed by the width of the depletion region (Figure 2.14(c)). The two series capacitors have a lower overall capacitance than that of either the semiconductor or oxide alone. Now the bands bend the other way; the slope of the oxide conduction band edge or electric ﬁeld reverses sign, and near the interface the semiconductor acquires an n-like character. At still higher positive voltages,electrons are drawn to the interfacial region, where the semiconductor is locally inverted to n-type. Extreme band bending is characteristic of large


### 2.5.2 The MOS Capacitor


values of VG. An inversion regime (Figure 2.14(d)) is created where the overall capacitance reaches a minimum. Effective charge distributions (Q)on the metal and in the semiconductor are depicted below each of the MOS bias states.


Ideal capacitance–voltage (C–V) characteristics derived from biasing the MOS structure are displayed in Figure 2.15; an entirely complementary behavior is exhibited by n-type Si but with opposite gate voltage polarities.


The MOS capacitor not only plays an active role in device function, but has


Figure 2.14 (a) Ideal metal-oxide-p-type semiconductor (MOS) capacitor structure.


Without applied gate voltage there is no oxide ﬁeld, and a ﬂat-band condition prevails.


(b) Negative gate-voltagedaccumulation of holes results in band bending at the interface. (c) Positive gate-voltagedexpulsion of holes causes Si to act like a dielectric with a capacitance governed by the width of the depletion region. (d) Large positive gate voltagedinversion regime is created and Si interface is effectively n-type.


Electronic Devices: How They Operate and Are Fabricated 67


proven valuable in assessing bulk ionic contamination (e.g., Naþ) and interfacial electronic charge (Qi) introduced during gate-oxide processing.


When such charge exists it can produce large voltage shifts (i.e., V¼Qi/Co) in the C–V characteristics (Figure 2.15). Charging of gate oxides during plasma processing or exposure to ionizing radiation produces similar voltage shifts. Charge drift and recovery in electric ﬁelds cause operational instabilities in devices.


2.5.3 MOS Field Effect Transistor


The n-type MOS (NMOS) ﬁeld effect transistor is shown in Figure 2.16(a),where it is evident that n-doped source and drain regions ﬂank a central MOS capacitor section composed of p-type silicon. Beneath the oxide there are essentially two p–n junctions connected back to back. When no gate voltage is applied, only a small reverse leakage current ﬂows between the source and drain. Recalling the previous section, we note that application of a sufﬁciently large þVG causes inversion of the MOS structure.So-called “strong inversion” essentially occurs at a threshold gate-voltage level VT given by:


VT ¼ DFMS Qi=Co þQd=Co þ 2fF:


(2.6)


Figure 2.15 Ideal capacitance–voltage (C–V) characteristics based on the biasing conditions in Figure 2.18. Flat-band voltage (VFB) shifts from uncharged capacitor(dotted) due to oxide charge are shown. More positive charge (less negative charge)produces negative voltage shifts, and more negative charge (less positive charge)produces positive voltage shifts.


### 2.5.3 MOS Field Effect Transistor


At this voltage a thin surface inversion layer or conducting n-channel forms joining the two heavily doped nþ regions, and the transistor is turned


on. This equation basically expresses that bands must ﬁrst be ﬂat, and the


effective voltage contributions to VT by the ﬁrst two terms ensure this. The work function difference between the gate electrode and semiconductor is


DFMS, while the second term was introduced above, to reﬂect bulk and interface charge Qi. Next, the p-type Si must be depleted of hole charge,dV8


Figure 2.16 Behavior of n-MOS ﬁeld effect transistor. (a) Cross-sectional view showing operation in the linear region. (b) Operation at the edge of saturation (pinch-off). (c)Operation beyond saturation.


Electronic Devices: How They Operate and Are Fabricated 69


(a)Vs= 0VG>VT9


VD small


9石↓


OXIDE


SOURCE(n+)


(n+)


CHANNEL


SUBSTRATE (p-Si)DEPLETION REGION d V8


(b)vs=0VG>VT9


。


VD= VD (Sat)


SOURCE


DRAIN


PINCH-OFF


POINT


SUBSTRATE (p-Si)DEPLETION REGION dV8


VG>VT9


Vs=0


VD>VD (Sat)


SUBSTRATE (p-Si)DEPLETION REGION


nDRAIN


Qd (term 3), and ﬁnally, strong inversion (term 4) must occur. The quantity fF is essentially the difference in magnitude between the midgap (intrinsic)level and the actual Fermi energy, EF. Both Qd and 2fF as well as EF depend on doping level.


As written, this formula refers to n-channel devices, but it also applies to p-channel devices as well if the signs of the last two terms on the right are changed from þ to –. It should be noted that large contributions to VT aremade by both Qi and oxide capacitance, Co. Advantage is taken of this by controllably adjusting VT through ion implantation in order to effectively change Qi, and by growing thick oxides to electrically isolate devices. By the same token, even slight time-dependent electron charging of the oxide in service increasesQi and hence altersVT. In fact, the same factors that cause shifts in C–V characteristics induce threshold voltage shifts. These cause reliability problems because MOSFET action may be unintentionally triggered.


Once the underlying Si is inverted, the electron current ﬂow from the source to drain through the surface n-channel can be controlled by varying the drain voltage (VD). The remaining portions of Figure 2.16 reveal what happens with successively higher drain voltages. If VD is small, electron ﬂow yields a drain current, iD¼VD/R, where R is the channel resistance. Thislinear region is indicated on the iD–VD characteristics of Figure 2.17(a). As VD increases, it eventually reaches a point where the inversion layer width at the drain shrinks to zero, the pinch-off state. Beyond pinch-off, iD essentially saturates, but the channel width is effectively reduced. Electron injection into the drain depletion region is now similar to that of carrier injection from an emitter–base junction into the base–collector depletion region of a bipolar transistor. In addition to these n- and p-channel“enhancement mode” MOSFETS, there are “depletion mode” MOSFETS. These are fabricated containing the channel in the conducting state,and are thus switched on even when VG¼ 0; during operation the con-ducting channel must be turned off by applying the proper polarity voltage.


In both n- and p-type MOSFETs degraded by hot-carrier induced oxide damage, the iD–VD characteristics deviate from the prestressed state as shown in Figure 2.17(b) and c. In essence, drain currents decline in n-MOSFETs and rise in p-MOSFETs. Hot-carrier effects are addressed again in Section 6.4.


2.5.4 CMOS Devices


The combination of MOSFETs, one n-type and the other p-type, is known as a complementary MOS or CMOS device (Figure 2.18). By


### 2.5.4 CMOS Devices


connecting gates in common as the input and drains in common as the output as shown, this device operates as an inverter in digital circuits. Weﬁrst recall that VT is positive in the n-channel transistor and negative in the p-channel transistor. When the input voltage (Vin) is “high,” the n-channel device is in the “on” state and the p-channel device is in the “off” state.


Therefore, the channel resistance of the p-device is much higher than that of the n-device. This causes voltage V to drop mostly across the p-channel,and the output voltage (Vout) is “low.” If the input voltage is now “low,”the n-device is off and most of Vout stems from V which represents the“high” state. Therefore, in either state a transistor is off, and there is no DC 0-2-3-4-5-6


VD


Volts


Figure 2.17 Current-voltage (iD–VD) characteristics of the MOSFET. (a) Ideal behavior.


(b) Forward and reverse n-MOSFET iD–VD characteristics after hot-carrier oxide damage. (c) Forward and reverse p-MOSFET iD–VD characteristics after hot-carrier oxide damage. From Ref. [13].


Electronic Devices: How They Operate and Are Fabricated 71


可


VG=5V


+4


Pre-stressxPost


Pinch-off


Stress


1.0


VD(Sat.)


+3V u


Bd


VG=3V


0.5


VG=+1V


VG = 2V


012


(c)- - Forward


-1.0Reverse


VG = 5V


Pre-stress


-0.8


19=t^


V-0.6 a


1=EA


04


VG=2V


-0.2


3456


0.1


+2


VG=4V


path to ground other than leakage current. No drain current ﬂows except during the very short switching period. The fact that little power is drawn is a primary reason why CMOS dominates the market for low-power logic and memory ICs where switching is the principal function.


2.5.5 MOSFET Instabilities and Malfunction


2.5.5.1 Oxide Charge


The critical gate oxide is quite hospitable to both ionic and electronic charge. In addition to mobile alkali ion contaminants, there is both bulk oxide positive and negative trapped charge, as well as interfacial charge trapped at the Si–SiO2 interface/boundary, and ﬁxed charge some 3 nm away. Area densities for the latter two are 1010 to 1011/cm2. Sources of the charge are thought to be structural defects related to bond breaking and metallic impurity contamination in the oxidation process. During device operation, energetic, or hot, electrons in the channel may also get scattered into the oxide. Time-dependent dielectric breakdown and shifts in VT are two important reliability consequences of such oxide charge buildup. This subject will be addressed more fully in Chapter 6.


Figure 2.18 Top: Circuit connection of transistors in a complementary MOS (CMOS)device. The indicated inverter function requires common gates as the input and common drains as the output. Bottom: CMOS structure.


### 2.5.5 MOSFET Instabilities and Malfunction


2.5.5.2 Short Channel Effects


A concern in VLSI and ULSI circuits is the existence of anomalous MOS transistors with shorter source–drain spacing than minimum design rules specify. The creation of a completely depleted area under the gate will then occur at lower gate voltages, and VT will be effectively reduced. Electricﬁelds are also higher in the drain region, making such transistors much more susceptible to hot electron effects.


2.5.5.3 Parasitic Bipolar Transistors: Latchup


Despite efforts to conﬁne MOS transistor action to a designated region of the substrate, sometimes unintended parasitic bipolar transistor behavior intrudes into the same or a neighboring location. So long as no p–n junction is forward biased, the bipolar transistor is inoperative. But for high enough substrate–source voltages, a large emitter current is injected,resulting in large device currents.


A more serious parasitic phenomenon known as latchup occurs in CMOS devices. Here the closely spaced sources and drains of n and p channel MOSFETs give rise to two parasitic bipolar transistors, one n–p–n and one p–n–p, as shown in Figure 2.19. These transistors are cross connected so that the base–collector junctions are common. Under bias, the p–n–p collector delivers current to the n–p–n base, and the n–p–n collector


Figure 2.19 Latchup arising in CMOS devices due the creation of closely spaced and coupled n–p–n and p–n–p parasitic bipolar transistors.


Electronic Devices: How They Operate and Are Fabricated 73


delivers power to the p–n–p base. If the gains of these transistors are high,both are driven into saturation, and the power supply voltages become connected through a low resistance path. In essence, a device known as a thyristor, which contains p–n–p–n doped regions, is effectively created.


Carriers generated in unwanted regions by leakage currents, substrate current, or even photon irradiation can trigger latchup. When this happens,short-circuit currents rapidly overheat the IC chip, destroying it. Better design of transistor isolation is effective in combating latchup.


2.5.6 Bipolar versus CMOS


Now that the two major transistor technologies have been introduced, it is pedagogically worthwhile to compare the characteristics and attributes of each type of device [14].


1. Size. Using the same lithography tools, the footprint of bipolar transistors is typically 20–40% larger than the corresponding MOS transistor.


A key advantage of CMOS technology is the smaller device area, which translates to a higher packing density.


2. Power consumption. As indicated above, standby power consumption of CMOS transistors is much less than that for bipolar transistors. This advantage, plus high packing densities makes CMOS the obvious choice for ULSI and ELSI applications.


3. Complexity of fabrication process. CMOS devices, with typically 20% fewer processing steps required, are easier to fabricate than bipolar transistors.


Part of the simplicity and smaller size of MOS devices stems from the less stringent isolation required. To isolate or insulate devices from one another on the same chip, more complex and deeper dielectric structures (trenches) are required for bipolar than for MOS devices.


4. Current carrying capacity. An important advantage of the bipolar transistor is its decidedly superior gain because of its high transconductance.


Deﬁned as the derivative of the output current to input voltage, the transconductance (Gm) of a transistor is a measure of its quality as an amplifying device. In bipolar transistors, Gm¼ qic/(kT), where q is theelectronic charge, ic is the collector current, and kT has the usual meaning. For MOS transistors Gm¼ (2mm iDS Cox Z/L)1/2, where m is theelectron mobility, iDS is the drain–source current, Cox is the gate–oxide capacitance, and L and Z are the channel length and width, respectively.


Substitution of typical values reveals that to match the bipolar transconductance, the dimensions of MOS transistors must be a few orders of magnitude larger.


### 2.5.6 Bipolar versus CMOS


5. Sensitivity and speed. The exponential dependence of the current on the base–emitter voltage gives the bipolar transistor superior signal detection capabilities relative to MOS devices. Bipolar devices are also faster than MOS transistors and exhibit higher frequency response and gain. This makes them well suited for high performance analog applications.


6. Market share. Currently, NMOS and CMOS technologies account for about 80% and bipolar 15% of the IC market share. Compound semiconductors and BiCMOS make up the remainder.


For ﬂexible circuit design, BICMOS technology combines the high density of CMOS with the speed of bipolar transistors. This technology has been used in the Intel Pentium microprocessor, a chip containing 3.3 million transistors. In general, BICMOS circuits employ CMOS transistors to perform the logic functions and bipolar transistors to drive the output loads.


2.5.7 Junction Field Effect Transistor


Like the MOSFET, the JFET, depicted in Figure 2.20(a), also consists of a gate–source–drain combination. Rather than an oxide/semiconductor structure, the active region beneath the gate consists of three vertically stacked semiconductor layers. In operation the upper and lower gates (the top and bottom heavily doped p-layers) are connected together, while the lightly doped n-channel in between has the drain voltage (VD) applied across it. Both p–n junctions are slightly reverse biased initially, so that depletion layers extend into the channel. As þVD is applied, a channelcurrent (iD) ﬂows whose magnitude is simply given by Ohm’s law, or VD divided by the channel resistance. At larger values of VD, the voltage drop(i.e., bias) that progressively rises from source to drain increases both iD and the depletion width in concert. Finally, the two depletion regions merge at the drain, and the channel pinches. At that point the current saturates just as it does in MOSFETs and the iD–VD characteristics resemble those displayed in Figure 2.17(a).


Similar devices known as MESFETs are widely used in high-frequency circuits. Fabricated in III–V compound semiconductors, they are discussed in Section 2.7.3.


2.6 MEMORIES


2.6.1 Types of Memories


Together with logic chips, memory chips are critical for computer circuit applications. Memories are circuits that enable the storage of digital


Electronic Devices: How They Operate and Are Fabricated 75


### 2.5.7 Junction Field Effect Transistor


## 2.6 Memories


### 2.6.1 Types of Memories


information, or data, in terms of bits (binary digits). They now account for close to 40% of the integrated circuit market and can stand alone on a single IC chip or be embedded within a larger IC. A road map through the broad variety of memories used, and the categories they belong to, is shown in Figure 2.21. Memories that lose their data when the supply voltage is removed are said to be volatile, while those that retain data under such conditions are nonvolatile. Another subdivision reveals that there are three kinds of memorydserial memory, random access memory (RAM), and read only memory (ROM). Volatile memories include serial, static(SRAM), and dynamic (DRAM) types. Three-quarters of the total memory


Figure 2.20 (a) View of a junction ﬁeld-effect transistor with a detail of the central channel region. (b) Schematic of the MESFET. Current ﬂow through the channel is controlled by the gate voltage, which varies the depletion layer width. From Ref. [1],Copyright by Bell Telephone Laboratories, Inc.


market, including both volatile and nonvolatile, is dominated by DRAMs.


In serial memories, data enters and leaves in the same sequence, so the “ﬁrst in” is the “ﬁrst out.” Charge coupled devices (CCD) described later are used in such memories for video applications.


Random access memories, which come in SRAM and DRAM varieties,are arranged in a matrix array and require both read–write data and address inputs and data outputs. Data can either be written or read directly in a random way, unlike memory locations on magnetic tape, which must be lined up with the read–write head. Storage of data occurs within memory cells. In SRAMs these cells contain inverter circuits, and combinations of them are known as ﬂip-ﬂops, which are capable of assuming two states.


While SRAMs are the fastest of all MOS memories, this is accomplished at the expense of requiring four to six transistors per cell. In contrast, DRAM cells contain an integrated transistor–capacitor unit, enabling greater packing densities at lower cost. The operation of a DRAM will be described in the next section. Since charge is stored in a capacitor within DRAM cells, gradual leakage necessitates refreshing approximately every 2–16 ms. In contrast, static RAMs ensure that voltage levels are maintained as long as the power supply is on.


Read only memories are, in fact, random access memories that are permanently written during the fabrication process. Therefore, the information is lasting (nonvolatile) and can be read but not altered. There are also several kinds of ROMs that can be programmed by the user.


Figure 2.21 Overview of the different types of semiconductor memories. From Ref. [15].


Electronic Devices: How They Operate and Are Fabricated 77


memories


volatile memories


nonvolatile memories


sequentialSRAMDRAMROMPROMEPROMEEPROMNVRAMBRAM


seq. memory


-shift register


-CCD


programmable ROM


static memoryerasable programmable ROM dynamic RAM


electrically erasablebattery-RAM


-pseudo static-virtual static-video-RAM


nonvolatile RAM programmable ROM


read only memory


1. PROMs are ROMs that can only be programmed once. They usually consist of bipolar transistors, and the act of programming causes fuse links to be electrically blown, permanently ﬁxing the memory circuit.


2. EPROMs are similar to PROMs but are erasable by exposure to ultraviolet (UV) radiation. Their operation will be discussed in the next section.


3. EEPROMs are PROMs that are electrically erasable and can be reprogrammed repeatedly.


2.6.2 Memories Are Made of This!


In this section the structure and operation of typical serial, RAM, and ROM memory devices will be brieﬂy described.


1. Charge Coupled Device (CCD). The CCD of Figure 2.22 consists of closely spaced MOS capacitors arrayed on a continuous SiO2 layer that covers the underlying p-type semiconductor. If sufﬁciently large


Figure 2.22 Schematic of a charge-coupled device. Charge originally stored on center capacitor is transferred to neighboring cell by increasing bias voltage. From Ref. [1],Copyright by Bell Telephone Laboratories, Inc.


positive voltage pulses are applied to all of the electrodes, each capacitor will be depleted. In order to transfer charge to one of the cells, a higher bias is applied there to create greater depletion. In effect, a potential well develops there that captures injected electrons. By pulsing the neighboring cell to the right more positively, electrons can be made to transfer between cells. This lively transfer of charge can proceed in both directions. CCDs have found use in imaging devices that ultimately produce electrical video signals.


2. DRAM. The drive to minimize the number of devices per memory cell has led to the widespread use of the NMOS transistor/capacitor combination. A cell cross-section and the way it is wired into the circuit are shown in Figure 2.23. In 256 Mb DRAMs the cell size is <0.7 mm2,while in 1 Gb DRAMs, areas less than 0.3 mm2 are involved. But, for 4 Gb DRAMs the cell size is only <0.1 mm2! Shrinkage of DRAM cells mean that thicknesses of gate and capacitor oxide dielectrics must scale accordingly [16]. The drain of the MOSFET serves as the conductive path between the inversion layers under the capacitor and the transfer gates. Electrodes of the storage capacitor are the drain/conducting polysilicon ﬁll and the substrate ground; they sandwich the SiO2 dielectric in between. High packing density requirements have motivated clever approaches to simultaneously reduce chip surface area while increasing charge storage capacity. By fabricating deep trench capacitors, the capacitance is markedly increased. Trench technology poses processing challenges in ﬁlling deep holes without the formation of defective cells.


Further, as the size of the storage capacitor has continued to decrease,the need has arisen for dielectric materials with higher dielectric constant(Hi k), so that more charge can be stored in a smaller space. Materials such as hafnium silicate, oxidized nitride (ON), oxidized nitride/oxide(ONO), tantalum oxide (Ta2O5), barium strontium titanate (BaxSr1–xTiO3), HfO2, TaO, and TiO2 have begun to replace SiO2, because of their higher dielectric constant. We shall return to the issue of defects in these important devices in Section 3.2.5. Important main modes of failure include gate shorts, and the loss of stored charge due to leakage or recombination.


Provision must also be made to isolate (insulate) the transistor from other nearby circuit elements and devices. The operating principle of the planar bipolar transistor is the same as that for the discrete bipolar transistor. High operational speeds and current capacities have earmarked these devices for digital logic as well as linear input/output circuits. State of the art bipolar transistors are using germanium in the base region of a device called, SiGebased HBT (heterojunction bipolar transistor) [12].


The most complex digital system can be constructed from circuits that perform relatively few operations such as AND, OR, and INVERT.


Individual circuits that perform these functions are known as logic gates.


Over the years different logic gate circuits containing collections of bipolar transistors have been designed and incorporated into a wide variety of digital electronics. We just have time to mention some of the popular ones,namely emitter-coupled logic (ECL), transistor–transistor logic (T2L), and integrated-injection logic (I2L). The reader is referred to electrical engineering texts for descriptions of their operation and relative merits.


3. EPROM. These read only devices are basically MOS transistors that contain an additional polysilicon gate layer embedded within the oxide beneath the gate electrode. Because the embedded gate is unconnected it is electrically ﬂoating. Through application of a high source–drain voltage pulse, an avalanche of electrons is initiated near the


Electronic Devices: How They Operate and Are Fabricated 79


pinched-off region. Some electrons acquire enough energy this way to enter the oxide and charge the ﬂoating gate. It is for this reason that these MOSFETs are known as ﬂoating avalanche, or FAMOS, devices.


In packaging these devices a window is installed over the chip to enable


Figure 2.23 Cross-section of a DRAM cell and its method of interconnection in the circuit. To write, the bit line is driven to a high or low logic level with the cell transistor on. Then the transistor is shut off leaving the capacitor charged high or low. (Charge leakage requires refreshing.) To read, the bit line is left ﬂoating as the transistor is turned on; the small change in bit-line potential is sensed and ampliﬁed to a full logic level. From Ref. [16].


Bit line


Word line


Storage node


Cell


transistor


Storage capacitor


Cell plate


Buried strap


Borderless contact


Passing word line


p-wellTrench Shallow-n


trench


isolation


polysilicon fill


collar


UV light to shine through and erase the memory. By locating theﬂoating gate only a few nanometers from the silicon substrate, tunneling currents can charge the ﬂoating gate and also erase information; this is done in EEPROM devices.


2.6.3 Reliability Problems in Memories


Memory reliability problems can be divided into three categories [17],namely (1) processing or fabrication related, (2) operation related, and (3)environment related. Most concerns are common to SRAMs and DRAMs and to a lesser extent to EPROMs.


Processing difﬁculties include control of the conductor line width and semiconductor doping levels, defects due to contamination, stress, and processinduced radiation. Yields are adversely impacted, and poor performance and degradation often show up in the infant mortality population. Adding redundant columns or rows of devices that can be programmed to substitute for failing memory cells is one of the strategies adopted to combat failed devices.


Operational reliability problems stem from the nonuniform scaling of device features to achieve high packing densities. Reduction in transistor gate lengths without corresponding changes in operating voltages has resulted in higher drain electric ﬁelds. These promote time-dependent changes in dielectric properties and threshold voltage shifts.


Environmental damage is largely related to packaging issues. On the chip level, nuclear radiation in the form of gamma rays and alpha particles,which may originate in the packaging materials (e.g., Pb–Sn solder),impinge on memory cells and ionize atoms, causing local soft errors.


Chapter 7 addresses such reliability issues.


2.7 GAAS DEVICES


2.7.1 Why Compound Semiconductor Devices?


Hailed as the electronic materials of the future, advances in silicon technology have perpetually consigned compound semiconductors to a secondplace status. Nevertheless, there are electronic functions that are performed inefﬁciently or not at all by Si devices; this is the reason for our interest in III–V materials, speciﬁcally GaAs, InP, and ternary and quaternary alloys based on these materials. A comparison with Si indicates several important reasons for their use in devices.


1. The speed (frequency) of devices made from compound semiconductors exceeds that for Si devices simply because electron mobilities are


Electronic Devices: How They Operate and Are Fabricated 81


## 2.7 GaAs Devices


higher. For example, Table 2.2 reveals that me (GaAs) is some six times that for me(Si). This shortens electron transit times and enhances highfrequency operation. Very high speed microwave devices and integrated circuits require these attributes of GaAs devices.


2. The larger band gap in GaAs relative to Si means that it can withstand higher working temperatures, an attractive property in small geometry power devices used in microwave applications. Low power devices that operate at room temperature have correspondingly low thermal generation of carriers and leakage currents, hence low noise.


3. Direct band-gap transitions in compound semiconductors make optical emission and absorption processes more efﬁcient than in Si (Section


2.2.2.4). This has enabled the production of efﬁcient lasers, light emitting diodes, and photodetectors.


4. Optical devices can often be made to operate at speciﬁc wavelengths within a broad spectral domain. In Si, only the wavelength corresponding to the band-gap energy is easily accessible. By alloying compound semiconductors, ternary and quaternary alloys emerge with energy gaps controllably tuned to a desired operating wavelength. Optical communications technology capitalizes on this to create highperformance light sources and detectors that operate at wavelengths where minimum optical losses occur.


5. A desirable attribute of GaAs is its ability to be produced in semiinsulating form with resistivities of w108 U-cm. Such insulating single crystals make excellent substrates for GaAs microwave devices and integrated circuits.


Advantages seldom come without drawbacks. In GaAs we are dealing with a brittle, expensive material that is not easy to process and fabricate into devices. On the other hand, Si is mechanically robust and cheap, and signiﬁcantly easier to process than GaAs. Silicon can also be protected and passivated by an easily grown, high-quality SiO2 ﬁlm, something that cannot be done in GaAs.


The subsequent discussion reﬂects the division of compound semiconductor devices according to microwave and opto-electronic applications. General tutorial reviews of the operation, reliability, and failure of compound semiconductor devices can be found in references [18–20].


2.7.2 Microwave Applications


Microwave frequencies range between 109 Hz (1 GHz) to 1000 GHz with respective wavelengths of 30 to 0.03 cm. Within this spectral domain are a


number of communication systems applications that are important in both the military and civilian sectors. Military applications include ground and airborne radar, electronic warfare including guided weapons, and satellite communications; civilian applications include microwave radar (for police,small boats, intruder alarms, and door openers), direct broadcast satellites(12 GHz), and mobile (1–3 GHz band) as well as cellular (w1 GHz)communications. To make these systems function, devices that generate,detect, and amplify microwave signals are required. Since the limit for silicon devices is w1.5 GHz, GaAs devices are preferred above this frequency. Microwave circuits are sometimes difﬁcult to design because conductors such as stray solder act like antennas at these frequencies.


2.7.3 The GaAs MESFET


By replacing the upper p–n junction of a JFET (Figure 2.20(a)) by a reverse-biased Schottky barrier, the MESFET emerges. The ﬁrst part of the acronym for this device, which is deposited on a semi-insulating GaAs substrate, stands for (Schottky) metal (contact) epitaxial (compound)semiconductor. In the MESFET, schematically depicted in Figure 2.20(b),source–gate–drain electrodes combine to control current ﬂow through a lightly n-doped single crystal (epitaxial) ﬁlm of GaAs that serves as the channel. Sandwiching the channel are the metal contacts above and the semi-insulating GaAs substrate below. Device behavior and characteristics parallel those of the Si JFET. But GaAs MESFETS differ from their lowerfrequency Si cousins because the channels are thinner (w0.1 mm) and gate lengths shorter (<1 mm). For channels of length Lc, the device cutoff frequency is given by vs/(2 p Lc), where vs is the electron saturation velocity(w2 107 cm/s in GaAs). Thus for a 1 mm channel length, w35 GHZoperation is possible.


In addition to the low-power, small-signal MESFETs used in receiver front ends and digital integrated circuits, there are power MESFET devices that operate at higher voltages. These devices contain an interdigitated, or comb-like, array of contacts that encompasses a larger area with a deep active channel. The contrast in geometries and operating conditions is re-ﬂected in different failure mechanisms for low-signal relative to high-power devices.


In contrast to the Schottky gate contact, source and drain contacts in these transistors must be ohmic (e.g., Au–Ge). Accelerated hightemperature testing of these devices has revealed failures due to the degradation of the metal employed in these contacts. “Gate sinking,” a


Electronic Devices: How They Operate and Are Fabricated 83


common failure mechanism involving metal interdiffusion into the GaAs, is discussed further in Chapter 5. Decrease in drain current at zero gate bias,reduction in pinch-off voltage, and degradation of channel properties (e.g.,increase in drain to source resistance) are some of the reliability problems associated with GaAs transistors. Improvements in gate metallizations over the past two decades have extended device lifetimes from thousands of hours employing Al to millions of hours with TiPtAu.


2.7.4 High Electron Mobility Transistor


These quantum devices operate much like MOSFETs and exhibit gains and speeds that are among the highest for any transistors [21,22]. A commonﬁgure of merit for FETs is the transconductance, and it can be increased by reducing the channel resistance through heavy doping. But this strategy degrades electron mobility because of carrier scattering by the ionized impurities. In high electron mobility transistosr (HEMTs), the dual desiderata of high carrier concentrations and mobilities are simultaneously achieved. This is basically accomplished at the interface between n-doped AlGaAs and undoped GaAs, as indicated in Figure 2.24(a). Electrons in the conduction band of the doped AlGaAs (larger energy band gap) spill over into the GaAs (smaller energy band gap), where they are now trapped in a quantum-mechanical well that is free of ionized donor scatterers. As a result of band bending at the junction, the electrons in the well are essentially conﬁned to a thin sheet. For this reason we speak of a two-dimensional electron gas (2-DEG). An electric ﬁeld applied normal to the page will result in enhanced carrier transport in the well channel. The effect of this so-called modulation doping is magniﬁed at low temperatures because thermal scattering by vibrating lattice atoms is minimized. Incorporated within the structure of the GaAs-base HEMT shown in Figure 2.24(b) is such a quantum well. Today, HEMTs also known as MODFETs have been fabricated with gate-lengths of approximately 0.25 mm in InP-base semiconductors. These devices demonstrably outperform GaAs MESFETs with respect to gain and low noise. Short gate-length GaAs and InGaAs MODFETs have frequency responses above 100 GHz with switching delays of w5 ps [19].


Sinking of Schottky gates and degradation of ohmic source and drain contacts are major failure mechanisms in both MESFETs and HEMTs.


Electromigration, surface oxidation of GaAs, burnout, diffusion of dopants from channels, and intermetallic phase formation in Al–Au metallizations


[18] are additional degradation mechanisms.


2.7.5 GaAs Integrated Circuits


Many of the same reasons for the integration of discreet Si devices have driven the development of both analog and digital memory and logic GaAs ICs. Except for microwave applications, these products have lagged behind their Si counterparts. In addition, there have been imperatives to fabricate monolithic microwave (and millimeter wave) integrated circuits, or MMICs.


But microwave circuits are not simply large collections of FETs; in fact, some MMICs do not contain FETs at all! In some MMICs the number of passive circuit elements (resistors, inductors, diodes, transmission lines, interdigitated


Figure 2.24 (a) Band diagram of an n-type AlxGa1–xAs–GaAs heterojunction structure.


Free electrons originating in the AlxGa1–xAs spill over into the quantum well on the GaAs side, creating a highly mobile two-dimensional electron gas or carrier density. An electric ﬁeld is applied normal to the paper. (b) Cross-section of a HEMT structure with dimensions to scale. The gate metal is TiPtAu, while the source and drain contacts are AuGeNi. From Ref. [23].


Electronic Devices: How They Operate and Are Fabricated 85


----------EF 2 DEG


GATEn+AIGaASAIGaASGaAS


SOURCEGATEDRAIN


→|.34μm艹


0.82μm←+1.1μm+


二500 A GaAs,7x1018cm-3 400AAI.26Ga.74As,2X1018cm-3-20AAl 26Ga 74As (undoped spacer)2 DEG


0.8μm GaAs (undoped)


二AlAs/GaAs Superlattice


七_1000A GaAs (undoped)


SEMI-INSULATING SUBSTRATETOTAL GATE WIDTH: 150 μm


METALDONOR LAYERSPACER


and overlay capacitors) may outnumber the FETs by a factor of 10 to 1 [24].


Recently, an extensive evaluation of MMICs composed of 0.5 mm GaAs MESFETs (with Au/Pd/Ti metallizations) tested at temperatures of 200–225 C revealed that the main failure mechanisms were diffusion related, e.g., gate sinking and ohmic contact degradation. Activation energies for failures ranged between 1.5 and 2.2 eV for the most part [25].


2.8 ELECTRO-OPTICAL DEVICES


2.8.1 Introduction


Our main concern with compound semiconductors in this book is related to the failure and reliability of electro-optical devices. The three basic phenomena capitalized upon in these devices-absorption, spontaneous emission, and stimulated emissiondwere already introduced in Section


2.2.2.4 and Figure 2.6. Since so much is at stake in ensuring the reliability of optical communication systems, much of our concern here is with the individual active semiconductor devices employed. Today, long-distance under sea (submarine) systems employ infrared wavelengths of 1.3 and


1.55 mm, where ﬁber transmission losses are minimal. This means that the lasers and LEDs that launch light at one end of the ﬁber and the photodiodes that detect it at the other end must operate at the same wavelength.


To tune devices this way, semiconductors must be tailored to have the necessary energy gaps as well as a good lattice match to the substrate.


Guiding the design of the band gap is Eqn (2.1). For example, by alloying Ga, As, In, and P, ternary In0.47 Ga0.53 As and quaternary InGaAsP devices lattice-matched to InP can be fabricated to serve the needs of light sources and detectors in optical communication systems.


2.8.2 Solar Cells


A good example of devices capitalizing on absorption processes are solar cells, in which solar energy is absorbed and directly converted into electricity. These devices have a p–n junction close enough to the surface so that incident photons can easily penetrate to it. Once the junction is illuminated, carriers that were immobile in the space charge region of the prior unilluminated, or dark, junction, now move. Electrons lose energy by occupying lower conduction band levels in the n-type material; similarly,holes lose energy by ﬂoating upward to ﬁll valence band levels in p-type material. Some of these carriers will promptly recombine. However,enough of them separate further to produce the equivalent of positive and


## 2.8 Electro-Optical Devices


negative battery electrodes, or a photovoltaic effect. The illuminated junction then acts like a photon-activated electrical pump, generating a current in the diode that can power an external circuit.


Reliability of terrestrial solar cells is adversely affected by environmentally generated surface deposits that reduce incident light and enhance corrosion of contact metals. Amorphous, hydrogenated silicon (a-Si:H),extensively employed in thin-ﬁlm transistors for LCDs, has also been used to fabricate solar cells. In such cells, low operating temperatures and exposure to high light intensities degrade the conversion efﬁciency in ways that are not entirely understood.


2.8.3 PIN and Avalanche Photodiodes


Both of these diodes are normally employed as photon (absorption) detectors in optical systems and operate under reverse bias. Compound semiconductor PIN diodes are available in planar and mesa conﬁgurations


[26], which are schematically depicted in Figures 2.25(a) and 2.25(b). These devices rely on InP and InGaAs ﬁlm layers to enable 1.3–1.5 mm wavelength operation in high reliability, long haul, and high bit-rate optical


Figure 2.25 (a) Cross-section of a III–V PIN photodiode in a mesa conﬁguration. (b)Cross-section of a planar III–V PIN photodiode structure.


Electronic Devices: How They Operate and Are Fabricated 87


communication systems. The main objectives in designing PINs are to reduce capacitance to achieve high bandwidth, eliminate noise, and minimize reverse-bias dark current, which limits receiver sensitivity. Easyto-fabricate mesa structures enable the ﬁrst objective to be met, but such devices exhibit dark current instabilities. Planar PIN structures have a passivation layer that protects the junction, and a p-doped InP cap that minimizes leakage current. As a result, planar PINs are inherently more reliable than mesa devices.


Avalanche photodiodes (APD) are similar to planar III–V semiconductor PINs but operate at much higher voltages to obtain multiplication of the photogenerated carriers. Light is absorbed in the InGaAs layer,and holes are swept to an InP junction where the avalanche multiplication of carriers initiates. The separation of absorption and multiplication regions reduces the junction leakage current. Reliability problems arise from high electric ﬁelds, which induce surface charge motion [27]. Other failure mechanisms that lead to increased dark currents stem from contact metal penetration of the junction region and localized breakdown of the junction edge. Although lifetimes of APDs are shorter than for PIN devices, the high failure activation energies of 1 eV result in reliable operation under normal conditions.


2.8.4 Light Emitting Diodes


When these diodes are forward biased, they spontaneously emit light as conduction-band electrons recombine with valence-band holes. This phenomenon of injection electroluminescence has been exploited in LEDs to produce the familiar colored numbers and letters in displays. LEDs are also a viable alternative to lasers in some short to medium distance optical communications systems, where their lower light output is not a disadvantage. Such an application is illustrated in Figure 2.26, where the LED,composed of InGaAsP lattice-matched to the InP substrate, launches


1.3 mm infrared light down the optical ﬁber.


Degradation in these devices stems from both the semiconductor materials and the contact metals [28,29]. Typical p-side metallizations employed are Au–Zn or Au/Pt/Ti. Devices using the latter trimetal contacts generally exhibit less loss in light output during aging at temperatures of 120–200 C. For the Au–Zn LEDs the activation energy for failure has been determined to be in the range 0.75–0.85 eV. At high light power,degradation is primarily caused by dark spot and dark line defect formation,a mode that also afﬂicts lasers. Precipitation of host atoms and the familiar


migration (sinking) of contact metal into the semiconductor have been identiﬁed as degradation mechanisms. Nevertheless, edge-emitting diodes(ELED) are considered to be highly reliable devices, especially at low power levels, levels, where lifetimes of ~ 107 h at 25 C have been projected.where lifetimes of w 107 h at 25 C have been projected.


Organic light-emitting diodes (OLED), composed of a two layer(conductive and emissive) structure of organic semiconductors, emit visible light in response to an applied voltage. The color of the light depends on the choice of organic semiconductors. Typical applications include small displays and general lighting. When used in displays there is no need for aﬂuorescent backlight, needed in active matrix LCD displays. The build up of layers in the structure are the anode (often Al), conductive layer, emissive layer and cathode. In Figure 2.27 electrons ﬂow from the cathode to the anode. Holes have a higher mobility in organic semiconductors and hence some holes, from the conductive layer, diffuse into the emissive layer.


Recombination of electrons with holes in the emissive layer, near the boundary to the conductive layer, produces light. The cathode, on top of the emissive layer, is typically ITO (indium tin oxide), which is transparent


EMITTED


RADIATIONS


+EMISSIVE LAYER


CONDUCTIVE LAYER


CATHODE(-)


\SiN


Figure 2.26 Schematic of a surface-emitting InGaAsP light-emitting diode latticematched to an InP substrate. The 1.3 mm infrared light emitted enters an optical ﬁber.


→ANODE (+)


Figure 2.27 OLED structure.


Electronic Devices: How They Operate and Are Fabricated 89


EPOXY


CONTACTS


InP


n


InGaAsP


p→


-InP


and allows the emitted light to escape. The OLED emits under forward bias. In the reverse direction no light is emitted. The emission of light at low voltage is an advantage because it requires low power and leads to long battery life. Arial light intensity, although lower than LEDs, is bright and greater than LCDs. OLEDs are typically used in small (eventually) ﬂexible displays for mobile phones and portable MP3 players, car radios and in high resolution head-mount displays, which are used much less frequently than 24/7 computer displays.


Emission in the blue was plagued by limited life until a phosphorescent organic semiconductor was substituted. Lifetimes of 20,000 h (well beyond tungsten ﬁlaments) can now be achieved. The organic semiconductors used are also degraded by moisture, hence the need for hermetic seals to insure a long lived display. An example from Sony is shown in Figure 2.28.


2.8.5 Semiconductor Lasers


Due to the many critical laser applications there has been far more published information on the reliability of lasers than of other opto-electronic devices. While light is emitted from LED junctions in all directions, intense,directed beams exit lasers. In order for spontaneous emission of photons and laser action to occur, however, it is ﬁrst necessary to have a population inversion of carriers. This is accomplished in a semiconductor diode structure where both p and n regions are so heavily doped that the Fermi levels lie inside the valence and conduction bands, respectively. Under conditions of high forward bias, large electron and hole concentrations exist


Figure 2.28 Sony’s ﬂexible OLED display.


within respective bands that now overlap in the vicinity of the junction.


A carrier population inversion is created, and stimulated emission occurs.


Parallel facets are cleaved and polished, forming the Fabry–Perot cavity in which the photons multiply, while the other faces are roughened to discourage lasing in these directions.


Emitted laser light has a wavelength corresponding to the band-gap energy (Eqn (2.1)) and exhibits the so-called L–i (L¼ optical power,i¼ current) output characteristics schematically indicated in Figure 2.29.Up to a critical threshold current density (jth), the light output is very low,but beyond jth it rises rapidly. Higher operating temperatures raise jth and lead to lower light outputs. Laser diodes displaying the kinked and nonlinear characteristics shown in Figure 2.29 are considered to be faulty[30]. Peaked kinks are often, but not always, indicative of internal defects and damage, while internal reﬂections frequently, but not always, cause the second type of kink characteristics. Kinks are also associated with higherorder modes of laser emission and changes in jth.


The simplest of all laser structures, the homojunction conﬁguration,contains the same semiconductor material, e.g., GaAs, on both sides of the junction. Good only as a pedagogical tool, such lasers require enormous threshold current densities (w50 kA/cm2 at 300 K and w5 kA/cm2 at 77 K) to initiate lasing. The severe reliability problems implied by Joule heating thus rule out continuous homojunction laser operation at room temperature. Furthermore, carriers can wander from the active region and recombine, resulting in a broadened emission. Output light stems from a considerably narrower active region in double-heterojunction lasers. First, the


Figure 2.29 Assorted laser light output current characteristics depicted schematically. From Ref. [30].


Electronic Devices: How They Operate and Are Fabricated 91


carriers are conﬁned by the two heterojunction GaAs and AlxGa1–x As barriers. Second, light is conﬁned to the active region by virtue of the higher index of refraction of GaAs relative to AlGaAs. Both effects lower the lasing threshold an order of magnitude, while narrow stripe contacts(20 mm wide) reduce jth further, to the point where reliable continuous operation can occur at room temperature. The evolution of these GaAsbased lasers, designed to operate in the range 0.8–0.9 mm, is depicted in Figure 2.30.


Popular laser geometries for optical communication systems are shown in Figure 2.31 and employ InGaAsP semiconductor materials [30]. Known as BH or buried-heterojunction lasers, the light generated in the buried active regions is strongly guided in these devices. Other features include low threshold currents and high quantum efﬁciencies. Instead of using only the reﬂective facets for controlling light output, an extended diffraction grating is incorporated in so-called distributed feedback (DFB) lasers for this


Figure 2.30 Evolution of GaAs-based lasers, designed to operate in the range


0.8–0.9 mm. From Ref. [1], Copyright by Bell Telephone Laboratories, Inc.


purpose. In this way a single laser wavelength from the multipeaked laser output can be selected and ampliﬁed.


A number of failure modes commonly observed in lasers include damage to facets, dark line and dark spot defect formation, aging effects,electrostatic discharge, and current-conﬁnement problems. The latter are manifested as a drop in laser efﬁciency because current leaks or is shunted away from the active region. Poor design, processing, and power surges are often the cause of current conﬁnement problems, to which some lasers structures are more prone than others. Interestingly, InGaAsP lasers have a higher immunity to laser degradation effects than AlGaAs/GaAs-type lasers.


Figure 2.31 Popular laser geometries for optical communication systems. Top: Etched mesa buried heterostructure (EMBH). Middle: Channeled substrate buried heterostructure (CSBH). Bottom: Double channel planar buried heterostructure distributedfeedback. From Ref. [30].


Electronic Devices: How They Operate and Are Fabricated 93


Detailed mechanisms for the failure of lasers and other electro-optical devices and components will be presented in Chapter 10.


2.9 PROCESSINGdTHE CHIP LEVEL


2.9.1 Introduction


It is much easier to draw schematics of devices and IC circuit diagrams on paper or with the aid of computers than to realize them in physical terms.


The production of devices requires different electrical materials to be shaped or patterned and creatively merged to form the active devices and passive components that must then be interconnected, insulated, and ﬁnally packaged. These issues and demands are at the core of a very broad interdisciplinary manufacturing technology that designs, fabricates, and packages solid-state devices and circuits.


Much of the glamour associated with semiconductor manufacturing occurs on the Si chip level, and that is what we shall address here. To appreciate what is involved, consider the state-of-the-art CMOS technology employed in the fabrication of advanced microprocessor chips. At the base of the stunning image of Figure 2.32, beneath the skeleton of the exposed interconnects, contacts, and ﬁrst aluminum wire level, are the CMOS transistors. These MOSFETs have effective channel lengths of


0.25 mm and gate-oxide thicknesses of 7.7 nm [31].


Issues related to the processing and fabrication of both Si and compound semiconductor devices have been very widely treated in the literature and


Figure 2.32 Scanning electron microscope image of the local interconnect and ﬁrstlevel aluminum wires in an SRAM cell. From Ref. [31].


## 2.9 Processing-The Chip Level


form the subject of many excellent books [6–10]. In this section some of the more important individual process steps in the fabrication of silicon IC chips are brieﬂy introduced. The intent is to convey a sense of the physical and chemical principles involved, and how potential defects may be introduced into the product. Processes discussed are number-keyed to the schematic of the MOSFET shown in Figure 2.33. In the following chapter speciﬁc processing defects will be addressed in greater detail.


2.9.2 Silicon Crystal Growth [1]


When defects or reliability problems surface in any manufactured product,our ﬁrst reaction is to suspect the quality of the starting materials. Wafers are the starting materials, but they are sliced from large single crystals. Therefore, growing crystals is the ﬁrst, and in many ways a critical step, in ensuring product quality. Bulk single crystals of silicon are grown by melting a Si charge in a SiO2 crucible, inserting a small cooled single-crystal seed into it, and pulling out the large solidiﬁed crystal. This is the Czochralski technique for growing “CZ” crystals. Successive solidiﬁcation occurs amid complex heat and mass transfer processes between and among the growing single crystal, molten Si, and surrounding inert gas ambient.


Even more complex is the simultaneous convective ﬂuid motion that disperses melt dopants and impurities. This ﬂuid ﬂow is dependent on melt temperature and relative speed of rotation between crystal and melt as the former is being pulled.


Simultaneously, compositional change occurs in both the melt and the crystal. To see why, look at almost any binary Si-dopant (P, B, As) or impurity phase diagram. Note that the liquidus and solidus phase


Figure 2.33 Schematic of the MOSFET indicating key processing steps.


Electronic Devices: How They Operate and Are Fabricated 95


boundary lines drop for small solute additions. Equilibrium at the crystal–melt growth interface implies that the solid is always purer than the liquid.


Since the effect is cumulative during directional solidiﬁcation, axial gradients in composition are predicted [32]. Grown crystals not only exhibit varying concentration proﬁles of intentionally added dopants, but contain unwanted elements like oxygen. But it is the transition metal impurities that are viewed with particular alarm; they cause the most severe problems, and great efforts are made to eliminate them or neutralize their inﬂuence. In addition, defect swirl patterns are not infrequently observed on planes sliced perpendicular to the crystal axis. Furthermore, surface striations that are several microns wide and alternately dopant rich and dopant poor sometimes decorate the length of bulk Si and compound semiconductor single crystals. Both features apparently stem from temperature ﬂuctuations at the growth interface and complex convective ﬂow patterns that cause a periodic partitioning of solute. From the standpoint of the MOSFET, variations in dopant level across the plane of a wafer must be minimized to ensure uniform device processing and chip performance.


Following growth, the crystals are shaped round by grinding and then sawed and polished to produce wafers. Presently, many integrated circuit production lines still process 15–20 cm diameter Si wafers, but large 30 cm diameter wafers have become the world standard with a projection of 45 cm in the future.


2.9.3 Epitaxy [2]


This important term refers to the ordered crystallographic registry of a single crystal ﬁlm deposit on an underlying crystalline substrate template. Ifﬁlm and substrate are the same (Si on Si) we speak of homoepitaxy. In electro-optical devices they are different (InGaAsP on InP), and heteroepitaxy is the appropriate term. The yield of early thin-ﬁlm bipolar transistors fabricated within homoepitaxially deposited Si was dramatically improved relative to those produced within the original, or uncoated, Si wafers. Chemical vapor deposition (CVD) or some variant of it is used to deposit epitaxial semiconductor ﬁlms on wafer substrates. The process typically entails reaction of a chlorinated silane, e.g., SiCl4, and H2 at temperatures of w1100 C and a pressure of w1 atm. Epitaxial processing in CMOS technology helps assure device isolation and minimizes junction leakage currents.


Epitaxial deposition for bipolar devices often involves ion implanted or diffused areas (for isolation (p-type) and subcollectors (n type)) in the wafer prior to the epitaxial deposition. These buried layers can cause auto-doping control problems.


Critical to insuring single crystal formation is a combination of a lowﬁlm nucleation rate and a high ﬁlm growth rate. If many nuclei form on the substrate, a worthless polycrystalline ﬁlm deposits. A low gas supersaturation and deposition rate will create few nuclei. On the other hand, high substrate temperatures enhance diffusion rates and facilitate atomic incorporation into lattice sites. This promotes the early lateral extension of the single crystal ﬁlm, and growth perfection as it thickens. Epitaxial Si ﬁlms are purer and frequently more defect-free than the substrate wafer; furthermore, they can be doped independently of it. Nevertheless, they do contain the assorted point, line, and surface defects noted later in Figure 3.15 that occasionally cause device malfunction.


2.9.4 Ion Implantation [3]


For high-performance devices with shallow junction depths, ion implantation, rather than diffusion, is the preferred method of doping. Unlike diffusion, where the surface dopant concentration is higher than in the crystal interior, the reverse is true in ion implantation. The subsurface wafer penetration of dopant ions is due to energies of w50–200 keV acquired when they are accelerated in the high electric ﬁeld of the implanter. Possessing energies thousands of times larger than the binding energy of lattice atoms, the dopant ions wreak havoc as they are embedded into Si. At ﬁrst a lightning-like ion current excites the atomic electrons and ionizes atoms,absorbing energy in the process. When the dopants lose enough energy,they slow sufﬁciently and then begin to violently collide with Si nuclei,knocking many off their lattice sites. Each dopant ion executes a different odyssey and comes to rest at a different distance from the wafer surface.


Spatially, dopant concentrations are statistically distributed as a Gaussian function both normal to the surface and transverse to it. The depth of the peak and spread of the Gaussian depends on the dopant and the nature of the matrix it passes through, e.g., Si, SiO2, SiN, photoresist. Ion beam damage to the silicon matrix creates disordered and even amorphous regions. These must be repaired by rapid thermal annealing at w900 C,where atoms can diffuse sufﬁciently to restore lattice crystallinity and full electrical activity to the dopants.


Electronic Devices: How They Operate and Are Fabricated 97


In modern IC chips some 15 to 20 or more ion implantation steps are carried out to dope large volumes (tubs), small regions (sources and drains),and to adjust the threshold voltage of ﬁeld effect transistors. This latter operation, which controllably alters the interface charge (Qi in Eqn (2.6)) at the Si–SiO2 boundary, is quite critical and requires precise ion doses and spatial distributions. Tailoring dopant proﬁles by ion implantation has additionally enabled minimization of hot-electron damage and latchup effects, as well as gettering of heavy metal (Fe) contaminants. In the latter two cases, high-energy implants are required to drive dopants deep beneath the surface layer of devices.


Ion implanters are one of the most complex pieces of microelectronics processing equipment; they are also potential and actual sources of contamination and defects. Ideally, a chemically pure, monoenergetic beam is desired.


In a practical sense onemay imagine defects arising from variations in ion beam energy, depth, lateral spatial distribution and ion dose, as well as from the presence of chemical contaminants. Examples are given in Chapter 3.


All of the processes to this point have been concerned with the underlying Si. Above the Si surface are assorted grown and deposited dielectric and conducting ﬁlms that we now consider.


2.9.5 Grown Gate, Field, and Isolation Oxide [4]


Today’s ULSI technology is due in large part to the excellent properties of thermally grown gate, ﬁeld and isolation oxides. This critical SiO2 ﬁlm,used for gate oxide, the smallest fabricated dimension in MOS devices, has been the focus of much study and reliability testing. Currently, gate oxide is less than 10 nm thick, it is made by controllably oxidizing silicon wafers in dry O2. The simple reaction, SiþO2/ SiO2, at temperatures between900 and 1100 C, produces a dense amorphous ﬁlm. Thick oxide growth has traditionally been modeled by linear kinetics at short time (i.e., do z t)and by parabolic kinetics at long time, i.e., do z t1/2, where do is the oxide thickness and t is the time. These formulas may not hold for the ultra thin gate oxides now grown.


Growth in the presence of N2O is a recent advance that has improved the quality of gate oxides. Nitrided oxides are apparently more resistant to(charge) trap generation and to plasma-induced charging, give rise to smaller electric-ﬁeld-induced leakage currents, and are generally longer lived than conventional oxides [33,34]. Oxide charging during operation,and the associated reliability problems of breakdown and hot electron degradation are topics discussed in Chapter 6.


2.9.6 Polysilicon and Metal Gates [5,35,36]


The gate oxide is contacted by a polysilicon electrode. Long ago, polysilicon replaced the much more unreliable aluminum electrodes that caused early dielectric breakdown in underlying oxides. Polysilicon ﬁlms are deposited in low-pressure CVD reactors through the reduction of silane by hydrogen. Below w590 C amorphous ﬁlms form, while above w610 C polycrystalline ﬁlms deposit. This narrow temperature range deﬁnes a useful processing window. At higher temperatures, gas phase reactions result in rough, loosely adhering deposits and silane depletion that causes poor ﬁlm uniformity. Impracticably low deposition rates occur at lower temperatures.


More recently, polysilicon has started to be replaced by metal gates such as TiN, WN and TaN which are compatible with the new hi-k dielectrics


[35]. Because the threshold voltage depends on choice of metal (work function again), different metals are needed for the n-channel and p-channel devices used in CMOS structure [36].


2.9.7 Deposited and Etched Dielectric Films [6,7,16]


Since all devices and interconnections support voltages and carry current while sitting on a conducting Si wafer, strategically placed dielectrics are needed to isolate them electrically. Aside from the critical (grown) gate oxide, an assortment of other insulator ﬁlms are deposited. They include SiO2, silicon nitride, and phospho- and boro-silicate glasses produced by CVD methods, often with the assistance of a plasma discharge. The dielectric ﬁlms must then be etched to expose windows to semiconductor contacts or to conﬁne subsequently deposited metal ﬁlms and vias (see next section). After microelectronic chips are fabricated they are usually encapsulated by a silicon nitride ﬁlm, an effective barrier that prevents moisture and alkali ion (Naþ) penetration. All of the above dielectrics are amorphous in structure and of the order of 1 mm thick. Typical reactions with precursor gases (on the left) and product ﬁlms (on the right) include:


for SiO2,


Si (OC2H5)4 (TEOS)/ SiO2 + byproducts


at 700 C


for silicon nitride,


8NH3 + 3Si2Cl2H2


/ 2Si3N4 + 6HCl + 12H2


at w 750 C SiH4 + NH3 / SiNH + 3H2 at 300 C for phosphosilicate glass, SiH4 + 4PH3 + 6O2


/ SiO2  2P2O5 + 8H2


at 450 C


Electronic Devices: How They Operate and Are Fabricated 99


In general, dielectric ﬁlm deposition steps are carried out at successively lower temperatures so as not to alter the prior processed and doped materials.


The composition, structure, and properties of such CVD ﬁlms vary widely with deposition conditions. Silicon nitride is an example. At very high temperatures dense, crystalline Si3N4 forms, but at lower temperatures considerable hydrogen is incorporated, particularly during plasma assisted deposition. Differences in dielectric strength, internal stress, and resistance to permeation of water and ionic impurities occur, but generally not to the point of compromising reliability. High phosphorous or arsenic glass compositions also corrode aluminum lines when moisture is present. More signiﬁcant are the problems associated with surface coverage by dielectricﬁlms and maintaining a planar terrain for subsequent metal depositions.


Incomplete ﬁlling of deep trenches and regions between metal lines can lead to structural voids and occasional short circuiting.


Maintaining a ﬂat planar topography is extremely important if subsequent lithography patterning errors and defects in deposited structures are to be avoided. The relatively new technique of chemical-mechanical polishing (CMP) has enabled the production of planar interfaces between successive metal and intermetal dielectric levels.


2.9.8 Metallization [8–10,14]


There is a need to contact and interconnect all of the doped semiconductor electrodes, i.e., source, drain, and gate, to other components and devices on the chip. Assorted metal and alloy conductors are employed for contact structures including Al and Al–Si, PtSi, Ti–W, Pd2Si, TiSi2. Interconnections, on the other hand, have historically been composed of Al thin-ﬁlm alloys with dilute Cu or Cu–Si additions. Copper has begun to replace Al, because it has higher conductivity and therefore less IR drop,point to point. In high-density ICs, efﬁcient packing of devices on the chip real estate requires placing interconnect stripes at successive metal levels [37]commonly denoted by M1, M2, M3, etc., as shown in Figure 2.34. High performance chips have from eight to 10 levels of metallization with metal studs ﬁlling vias between layers to maintain a planar surface. The highest level is composed of bus-bars that carry current to the chip contact pads.


Vias in the form of studs or plugs are like staircases that connect neighboringﬂoors, or levels, of interconnects. Tungsten plugs or vias are often deposited by CVD methods to vertically link adjacent interconnect levels. As shown in Figure 2.33, these vias are surrounded by TiN barrier ﬁlms that prevent mobile ions from reaching sensitive junctions and reactive gases from


etching exposed oxides. The above metals possess the best collective basket of desirable properties, including (1) high electrical conductivity; (2) low contact resistance to Si; (3) little tendency to chemically react with or interdiffuse in Si; (4) resistance to corrosion and environmental degradation;


(5) electromigration resistance; (6) ease of deposition; (7) compatibility with other materials and steps in the fabrication process.


The physical vapor deposition (PVD) techniques of evaporation and sputtering are the means employed to deposit metal ﬁlms. Sequential atomby-atom deposition results in ﬁlm nucleation and subsequent growth.


Unlike epitaxial deposition, both methods yield polycrystalline ﬁlms typically having submicron grain sizes, due in part to substrates that are often amorphous (e.g., SiO2).


Evaporation is the simpler of these metallization methods and involves heating of the source metal until it evaporates at appreciable rates. The process is carried out in high vacuum while wafer substrates, carefully positioned relative to the evaporation source, are rotated to yield uniform metal coverage. In sputtering, the metal or alloy to be deposited is fashioned into a cathode plate electrode and generally placed parallel to the wafers(anode) within a chamber containing inert sputtering gas. At low pressures less thanw5 mTorr, and potential differences of a few kilovolts DC, a glow discharge is sustained between electrodes. Within the discharge, energetic


Figure 2.34 Scanning electron microscope image of cross-section with six levels of metallization. From Ref. [38].


Electronic Devices: How They Operate and Are Fabricated 101


positive gas ions bombard the target, dislodging atoms that then deposit on the wafers as a ﬁlm. In magnetron sputtering, magnets placed behind the cathode conﬁne electrons to hop around the target and create a richer plasma that increases ﬁlm deposition rates.


The two metallization processes compete in many applications, and not only in semiconductor technology, but other industries as well. Issues that must be considered in selecting the best one for a particular application include (1) adhesion to the substrate; (2) ﬁlm stress; (3) stoichiometry of alloys ﬁlms; (4) uniform coverage of the topography; and (5) electrical damage to substrate oxides. Sputtering is preferred in most semiconductor applications because stoichiometry of alloys is maintained and step coverage is usually superior. However, evaporated Al ﬁlms appear to be more resistant to electromigration damage.


Many reliability problems are associated with contact and interconnection metallizations. They include changes in contact resistance due to interdiffusion reactions between Al and Si, electromigration-induced degradation of contacts and interconnections, and general corrosion damage. Contacts between Si and Al, two indispensible elements in microelectronics, are particularly troublesome. This results from mutual atomic interdiffusion (Section 5.4.2) and is remedied through alloying(e.g., Al–1%Si) or the use of diffusion barriers (e.g., metal silicides, TiW).


These must be imposed between the silicon and Al interconnections to prevent reaction. Other problems stem from stress. When surrounded on all sides by oxide, as interconnects are in the various metallization levels,tensile stresses develop in the metal. The reason, as we shall see in the next chapter, is due to the larger thermal expansion coefﬁcient of Al relative to SiO2. These thermal stresses are sometimes sufﬁciently large to generate voids that open interconnects.


Since 2000 dual damascene copper metallization [39] has been introduced notably by IBM (Figure 2.35). In this process copper is plated into trenches formed in the low k dielectric passivation separating metal layers.


After inlaying the copper in the preformed trenches the excess copper is removed using chemical mechanical planarization (CMP). The higher conductivity of the copper is a necessity as the line widths become narrower and the number of metal levels increases.


2.9.9 Plasma Etching


Plasma processes are widely employed in the fabrication of semiconductor devices. Examples include plasma-enhanced CVD, photoresist


removal, and the etching of polysilicon, dielectric, and metal thin ﬁlms.


Within the plasma a very reactive environment consisting of high energy electrons, ions, and precursor gas free radicals is created by applied voltages of a few kV. This combination of energetic reactants speeds up otherwise sluggish vapor deposition or material removal (etching)reactions, and effectively makes them proceed at lower temperatures. In our MOSFET, the need to etch contacts and vias in SiO2 is met by radio-frequency (RF) plasmas employing process gases containing ﬂuorine, carbon, and oxygen. Minimum dimensions, high aspect ratio features, and selectivity of the etch are necessary attributes of the etching process. The last attribute requires that neighboring polysilicon, metal, or silicides be immune to etching attack.


Damage to materials during plasma etching includes the buildup of charge and dielectric wearout due to bond breaking and charge trapping.


2.9.10 Lithography


Perhaps the most critical process in microelectronics is lithography, a technology that embodies a collection of critical steps. Lithography involves the use of exposure tools, masks, photoresist materials, and etching processes to enable such blanket area processing steps as ﬁlm deposition, etching,diffusion, and ion implantation to effectively occur only in preselected areas of a wafer surface. While there are obvious parallels to photography, instead of producing ﬂat images on paper, a three-dimensional relief topography is


Copper layer 6


Copper layer 5


Copper layer 4


Copper layer 3 Copper


B


layer 2 Copper


李


layer 1


Local tungsten interconnection


Figure 2.35 Multilevel (six levels) copper metallization. From Ref. [39].


Electronic Devices: How They Operate and Are Fabricated 103


created in materials like Si, SiO2, silicon nitride, aluminum, and photoresist.


After a mask (reticle) is generated with the desired geometric features,lithographic patterning involves spinning a photoresist ﬁlm on the wafer surface. As the name implies, photoresists are sensitive to photons and when developed are resistant to chemical attack by liquid or gaseous etchants.


Some are also sensitive to electrons and X-rays. In general, they consist of specially compounded polymers and display two broad types of behavior.


When exposed to light, the cross-linked polymer chains of positive resists undergo scission, or cutting, rendering them more soluble in a developer,while unexposed areas resist chemical attack. Under the same stimulus,negative resists molecules polymerize, while unexposed regions are soluble and dissolve in the developer.


If, for example, it is desired to dope silicon, a blanket ﬁlm of SiO2 isﬁrst deposited and then covered with a photoresist layer. After exposure and development, the unprotected SiO2 ﬁlm is removed by etching, and the photoresist is stripped away. This leaves the bare Si surface geometrically patterned by the remaining SiO2 ﬁlm mask. Now the exposed Si regions may be ion implanted. Similar steps must be repeated at many different depths, or levels, on the wafer as actual integrated circuits unfold. Alignment, tolerance and overlay of successive levels, e.g., contact metal over a contact hole, is absolutely critical so that correct registry is maintained simultaneously over millions of device features on large wafers. The magnitude of the problem can be appreciated when it is understood that 10 to 20 lithography levels are required in advanced IC chips.


Another method of using photoresist coupled with an underlay ﬁlm is known as the lift off process, primarily used for metallization. A dual layer of underlay and photoresist is patterned and the underlay is overetched,causing the photoresist to overhang the underlay. After metal deposition the undesired metal pattern on top of the photoresist is lifted off by dissolving the underlay ﬁlm.


Poor product yields have often been associated with lithography defects.


These arise predominantly from mask pattern defects that are discussed in Section 3.4.2.4. Metallization patterns deﬁned after etching may then, for example, contain either missing or added metal, which results in open or shorted conductors, respectively. Mask defects can be more readily tolerated by the expedient of employing 5 or 10 reduction stepper tools thatproject the patterns onto photoresists. The 1 systems do not offer thisopportunity and therefore require more defect-free masks.


2.10 MICROELECTROMECHANICAL SYSTEMS


2.10.1 Microelectromechanical Systems [40–42]


With the advent of very sophisticated and very precise techniques of semiconductor fabrication it became possible to construct miniature electromechanical systems of silicon or polymers and connect them, at the same time, to ICs for both control and sensing their mechanical movement or response to external stimuli. The birth of Microelectromechanical Systems provided the ability to construct tiny systems of millimeter size, micron size or even nanometer sizes, bridging to Nanotechnology, another emergingﬁeld. The applications for these tiny machines are almost ubiquitous and yet very little known. Injet (piezoelectric) print heads, optical data communication switches, projector displays, accelerometers in airbags, air pressure sensors for automobile tires, ﬁngerprint sensors, gyroscopes, all contain microelectromechanical systems (MEMS) of one kind or another speciﬁcally designed for the unique application employed. Figure 2.36 shows the tiny mirrors used in digital light processing chips known as DMD. These chips are used in high deﬁnition TV as well as the projectors used in meeting rooms all around the globe. The failure of these systems is quite dependent on their application, however hermiticity of the package, fatigue, wear, delamination and environmental induced failure has been observed.


1. What are some differences between materials used for electrically and mechanically functional applications?


2. Metals are the best conductors of electricity and heat, reﬂect light most efﬁciently, and are the most malleable of materials. Explain these attributes of metals in terms of their electronic and atomic structure.


3. Copper wiring in a telephone switching station was exposed to a ﬁre.


After the ﬁre the electrical resistivity of the wiring was measured. Some wiring was observed to have a lower resistivity, while other wiring exhibited an increase in resistivity.


a. Describe a scenario that would result in a resistivity decrease.


b. Describe a scenario that would result in a resistivity increase.


4. A good dielectric is a good insulator, but a good insulator is not necessarily a good dielectric. Explain why.


5. a. Rectiﬁers conduct large currents in one direction. Metals in contact also conduct large currents, but in both directions. Why can’t rectiﬁers be fabricated using metals?


Electronic Devices: How They Operate and Are Fabricated 105


## 2.10 Microelectromechanical Systems


b. An electric ﬁeld is built in at a semiconductor p–n junction. Insulators can support applied electric ﬁelds. Why can’t useful rectiﬁers


be fabricated using insulators?


c. What properties make semiconductors indispensable for junction


devices.


6. Electronic materials that will probably play important roles in the future are GaN for light sources, YBa2Cu3O7 for interconnections,and titanates for capacitors. Approximately where on the scale of conductivities in Figure 2.1 do these materials belong?


7. The p-type regions of two discrete diodes are connected in common.


Why does the resultant n–p–n structure not behave like a transistor?


Figure 2.36 Digital light processing technology. Courtesy: TI Texas Instruments.


8. Distinguish between (a) bonds and bands, (b) thermal and impurity


scattering, (c) spontaneous and stimulated emission, (d) Fermi energy


and energy gap, (e) direct and indirect band-gap semiconductors, (f)


electronic and opto-electronic devices, (g) metal–semiconductor and


p–n junction diodes, (h) ohmic and Schottky contacts, (i) MESFETs


and HEMTs, (j) bipolar and MOS transistors.


9. High local electric ﬁelds promote avalanche breakdown effects in both


semiconductors and dielectrics. Such breakdown is usually harmless in


semiconductors but can be destructive in dielectrics. Why? Electronavalanche effects do not occur in metals. Why?


10. High-power semiconductor diodes are usually fabricated containing a


heat sink. To understand why, sketch the effect of high operating temperatures on diode current–voltage characteristics.


11. When ohmic and Schottky contacts suffer electrical degradation, some


alteration of the metal–semiconductor band diagram is expected. Indicate possible band-diagram changes in the vicinity of a contact and


explain why they occur.


12. Boeing aerospace conducted reliability studies on some 25 million


semiconductor devices and found that bipolar power devices failed


signiﬁcantly less often than NMOS and CMOS integrated circuits.


What are possible reasons for this observation?


13. In a real, or nonideal, MOS capacitor structure, the work functions of


the metal and semiconductor differ. Sketch the band structures of an


unbiased metal–SiO2–p-type Si capacitor if fM > fSi.


a. Illustrate depletion, accumulation and inversion for this structure.


b. Sketch the band structures for depletion, accumulation, and inversion in an ideal metal–SiO2–n-type Si capacitor structure.


14. One strategy to minimize the probability of latchup in CMOS devices


is to fabricate them within a silicon ﬁlm grown epitaxially on an insulator (SOI). Illustrate how SOI structures suppress latchup.


The implications of charged dislocations on current ﬂow are depicted in Figure 3.6(b). Tortuous current paths result in increased carrier scattering and reduced mobility. Anisotropy develops such that carrier mobility and conductivity normal to dislocation lines are both reduced relative to their behavior parallel to them. Dislocations have also long been identiﬁed as charge recombination centers that degrade the minority carrier diffusion length and lifetime. Table 3.3 indicates the extent to which dislocations degrade the efﬁciency of silicon ribbon solar cells. Perhaps more signiﬁcant than the effect of dislocations on carrier motion is their ability to interact with assorted local impurities and point defects. When metallic impurities segregate at dislocations, problems due to excessive leakage currents and shorting of junctions arise. We have already noted such interactions in the practice of gettering metallic impurities by intentionally introducing dislocations.


Table 3.3 Correlation between dislocation density and solar cell characteristics Dislocation


density density (cm-2)(cm2)


Minority carrier diffusion length (mm)


|Region |||
|---|---|---|

|At twins bulk |||

|2108w106 |12 |9.5 |

|3x 108~106|19 |10.0 |

|None observed |135 |14.3 |

|None observed |156 |14.9 |

efﬁciency %


After Ref. [11].


Dislocations present in the thin base region of epitaxial bipolar transistors are particularly troublesome defects. Such dislocation “pipes” in effect are conducting paths between the emitter and collector that electrically short the base. Pipeline defects have also been observed [12] in CMOS devices, e.g., EEPROMs, where they serve to short sources to drain regions(Figure 3.7). Dopant implant damage coupled with compressive stress from the surrounding oxide appears to be the source of this yield-limiting defect.


3.2.3.2 Stacking Faults


So far we have focused on bond-breaking defects that include dislocations,surfaces, or vacancies. On the other hand, stacking faults correspond to errors in perfect stacking sequences and do not generally involve breaking nearest neighbor bonds. Therefore, charge distributions around stacking fault defect states are only mildly perturbed from those of a perfect lattice. If we consider the (111) close-packed plane in face-centered cubic structures,atoms appear to be arrayed as racked billiard balls on a pool table. Let us call this the A plane. As new atoms or balls are stacked above this layer they generate a parallel (111) plane designated as B, displaced slightly from thisﬁrst layer depending upon which depressions or interstices they nest in.


A third stacked row of atoms now has a choice of lying directly above the A layer or occupying a set of interstices that lie above neither the A nor the B layer; such a new layer is the C plane. In perfect FCC structures, atomic


Figure 3.7 Scanning electron microscope image of source–drain pipeline defect in aﬁeld-effect transistor. From Ref. [12].


Defects, Contaminants, and Yield 125


layers are ordered in sequential . ABCABCABC . fashion. But if the planar ordering is disrupted slightly and the sequence is. ABCBABCABC. (by adding an extra B row) or is . ABCACABC . (by withdrawing a B row), then stacking faults are created.


Due to the presence of two atoms in the primitive unit cell of silicon,the sequence of {111} planes is now .AA0BB0CC0AA0BB0CC0., etc.


Intrinsic stacking faults (ISF), extrinsic stacking faults (ESF), and twin stacking faults (TSF) may be viewed as simple variations from this ideal stacking sequence. For example, in the ISF a pair of atomic planes (such as AA0) is removed from the ideal stacking sequence, while the ESF is formed by inserting a pair of AA0 planes between the BB0 and CC0 layers and the TSF is produced by imposing reﬂection symmetry through a plane midway between the A and A0 layers, i.e., . BB0CC0AA0C0CB0B. .


Stacking faults are formed during oxidation. This process requires accumulation of oxygen at the wafer surface, diffusion through the growing oxide, and reaction at the Si interface, where, as noted earlier, an excess of Si interstitials and a deﬁciency of vacancies develop. Oxidation-induced stacking fault (OSF) defects nucleate at wafer surface damage sites, contamination, and oxide precipitates. They grow by absorbing Si interstitials or emitting vacancies, and their length increases with oxidation time and temperature. Small chlorine additions to the oxidizing ambience markedly decrease their density. Leakage currents in metal oxide–semiconductor devices are enhanced by many orders of magnitude in the presence of OSFs,especially if the associated dislocations are decorated by metallic precipitates


[13]. The cross-section of an epitaxially grown Si layer (Figure 3.8(a)) shows a stacking fault defect possessing a stripelike character. Nucleating at impurities or oxides, stacking faults in Si fan out and often appear as triangles or squares when they intercept the wafer surface normally. OSFs have resulted in high reverse leakage currents at p–n junctions in charge-coupled devices, as the correlation of Figure 3.8(b) reveals.


3.2.4 Grain Boundaries


These surface or area defects are the interfaces that separate individual single crystal grains from one another. In the hierarchy of defects, GBs are the most structurally complex because they encompass dislocations, point defects, and displaced atoms, all in a complex admixture. There are several effects that GBs display in semiconductors. Aside from extending light absorption to slightly lower energies in some materials (e.g., CdS), GBs are always unambiguously deleterious to device behavior. Their structural


complexity means that the electrical behavior will likewise be complex.


The simplest, or tilt, GBs are merely vertical arrays of edge dislocations.


Thus a model similar to that proposed earlier for dislocations holds for GBs,as suggested by Figure 3.9. In this model [15] for n-type material a planar,


1um


10-5


(A)rent curerse rev10-410一7


10-11


020406080100120 number of stacking faults


Figure 3.8 (a) Stacking fault (parallel stripes) and dislocations in the epitaxial tub of a high-speed silicon transistor. The entire area is covered by a dielectric layer. Crosssection transmission electron micrograph. (Courtesy of S. Nakahara, Lucent Technologies, Bell Laboratories Innovations.) (b) Reverse leakage currents in charge-coupled devices as a function of the number of OSFs. (From Ref. [14].)


Defects, Contaminants, and Yield 127


uniform array of trapped majority carriers (electrons) at the boundary creates positively charged depletion layers in the grains on either side. As the Fermi levels in the grains and boundary equilibrate, a Schottky barrier is established. Experiments involving transport properties in bicrystal and polycrystalline semiconductors have shown that GB defects raise the bulk resistivity, reduce carrier mobility, and enhance carrier recombination rates.


These are reasons why the optical performance of polycrystalline lightemitting diodes and solar cells is decidedly inferior to that of similar crystalline devices.


GBs are the preferred location for chemical reactions (e.g., etching,corrosion) as well as the solid-state mass transport effects discussed in Chapter 5 (e.g., diffusion, electromigration). Because boundaries are relatively open structurally, atoms attached to them tend to be energetic. This enables atoms and vacancies to migrate far more rapidly along GBs than through the bulk lattice. Furthermore, GBs are often stronger than the bulk at low temperatures, and they help resist mechanical deformation under stress. But at elevated temperatures, they are weaker than the bulk, and when the material breaks, the fracture often propagates along a GB path.


The dividing line is approximately half the melting temperature (TM, in degrees K); above TM atomic motion and reactions are favored at GBs,weakening their integrity.


Figure 3.9 Band diagram model of a charged GB of width d. Charge is transferred


from the grains to ﬁll GB trapping states, establishing a Schottky barrier of height FB.


The Fermi levels in the grains and GB are EFG and EFB, respectively. From Ref. [15].


Great efforts are made to eliminate any hint of GBs in semiconductor materials. An exception is Si solar cells, where polycrystalline cells are often suitable for the application, and are cheaper to produce, and of course the polysilicon gates of MOSFET devices.


3.2.5 Dislocation Defects in DRAMsdA Case Study


The main technology driver in microelectronics is considered to be DRAMs because their fabrication demands the cutting edge in ﬁne-line lithography and employs the largest wafer diameters. For these reasons DRAM technology is the conduit for innovations in materials, processes,and equipment into IC technology. The periodic architecture of memory cell arrays facilitates detection and localization of defective memory cells in fully automated electrical tests. Thus DRAMs provide ideal devices for studying the inﬂuence of defects on manufacturing yield.


A schematic of a 4-Mb DRAM cell is reproduced in Figure 3.10(a).


Dislocations with distinctive shapes were detected near the capacitor trench using the transmission electron microscope. These defects, shown in Figure 3.10(b), occurred in a region that received a high dose of implanted boron when doping the transistor source and drain [16]. As suggested by Figure 3.10(a), stresses generated during processing were large enough to initiate plastic slip on (111) planes of Si. The role of stress is addressed again in Section 3.3.2.


Recalling that DRAMs must be refreshed periodically to compensate for capacitor charge leakage, we may ask whether dislocations shorten the charge retention time or the refresh delay time. If so, a direct connection between these defects and DRAM performance can be demonstrated. With this motivation, tests that correlated the refresh delay time (or time between refresh cycles) and number of dislocations detected were performed, and typical results are plotted in Figure 3.11. Good cells are represented by the steep, or intrinsic, portion of the data, which extrapolates to a greater than 200 ms charge retention time [17]. The inescapable conclusion is that cells with a retention time of less than this fail by dislocation leakage currents.


3.3 PROCESSING DEFECTS


3.3.1 Scope


In this section we revisit IC manufacturing with an emphasis on defects that arise during chip-level processing. Schnable [18] has conveniently summarized processing defects, the ways they are manifested, and some of their


Defects, Contaminants, and Yield 129


## 3.3 Processing Defects


consequences in the concise compilation of Table 3.4. Defects of a crystallographic as well as structural, electronic, chemical, and morphological nature are included. High on the list of defects in virtually every processing step is contamination, a topic that is comprehensively treated in Section 3.4. We note that other defects have common origins such as stress and the lack of geometric coverage of IC features during ﬁlm deposition and etching.


Dislocation loop


Trench


Slip plane


GatePOLY


1μm


Figure 3.10 (a) Schematic of DRAM cell. Two device cells with trench capacitors,transfer device pedestal outline, and (111) glide plane containing a dislocation are shown. (b) Plan-view transmission electron micrograph of 4-Mb DRAM cell with dislocations having distinctive shapes generated next to the trench capacitor (dark) and transfer device drain. (From Ref. [16].)


Therefore, these are topics that will be treated in some detail. Lastly,lithography defects deserve separate consideration and will be discussed again in connection with yield. Later, in Chapter 8, there is a similar compilation of defects arising from packaging processes.


3.3.2 Stress and Defects


Stress in IC chips is not viewed as a defect per se, because it is an intrinsic consequence of processing dissimilar materials in contact. Nevertheless, stress has an important inﬂuence in generating or exacerbating many Table 3.4 defects such as hillocks, stacking faults, slip, internal stress, microcracking, and corrosion. In process steps involving ﬁlm growth (oxidation) or ﬁlm deposition (chemical vapor deposition (CVD), metallization), internal stresses develop in the bilayer ﬁlm–substrate structure.


Internal stresses arise in various manufacturing operations. When a homogeneous metal strip is reduced slightly by rolling, the surface ﬁbers are extended more than the interior bulk. The latter resists the ﬁber extension and places the surface in compression, while the interior is stressed in tension. This residual stress distribution is locked into the metal but can be


Figure 3.11 Cumulative number of bits in a 4-Mb DRAM that fail a refresh test as a function of refresh delay time. From Ref. [17].


Defects, Contaminants, and Yield 131


T a b l e  3.


4


D e f e c t s  a s s o c i a t e d  w i t h  m i c r o e l e c t r o n i c s  m a n u f a c t u r i n g  p r o c e s s e s  a t  t h e  c h i p  l e v e l


1. E p i t a x y  d e f e c t s:


c o n t a m i n a t i o n; e x c e s s i v e  l a t e r a l  a u t o d o p i n g; e x c e s s i v e  v e r t i c a l  a u t o d o p i n g;


ﬁ


l m  t o o  t h i c k  o r  t o o  t h i n;


h a z e; h e a v y  m e t a l  c o n t a m i n a t i o n; h i l l o c k s; i n a d e q u a t e  r e s i s t i v i t y  u n i f o r m i t y; i n a d e q u a t e  t h i c k n e s s  u n i f o r m i t y; l o w  m i n o r i t y


c a r r i e r  l i f e t i m e; p o o r  c r y s t a l l o g r a p h i c  q u a l i t y; p a t t e r n  s h i f t; r e s i s t i v i t y  t o o  h i g h; r o u g h n e s s; s c r a t c h e s; s t a c k i n g  f a u l t s


2. O x i d a t i o n  d e f e c t s:


a l k a l i  i o n  c o n t a m i n a t i o n; d o p a n t  p e n e t r a t i o n  t h r o u g h  o x i d e  m a s k; e x c e s s i v e  d o p a n t  p i l e u p;


x e d


o x i d e  c h a r g e  i n c o r r e c t; h e a v y  m e t a l  c o n t a m i n a t i o n; i n a d e q u a t e  r a d i a t i o n  h a r d n e s s; i n t e r f a c e  s t a t e  d e n s i t y  t o o  h i g h; l o c a l i z e d


o x i d e  t h i n n i n g; O S F s; o x i d e  t o o  t h i c k  o r  t o o  t h i n; o x i d e-t r a p p e d  c h a r g e  t o o  h i g h; p a r t i c u l a t e  c o n t a m i n a t i o n; s l i p  i n


s u b s t r a t e; s l o w  t r a p p i n g  i n s t a b i l i t y; t h i c k n e s s  n o n u n i f o r m; w h i t e  r i n g (K o o l  e f f e c t)


3. P h o t o r e s i s t  p a t t e r n i n g  d e f e c t s:


a l k a l i  i o n  c o n t a m i n a t i o n; b r i d g i n g; i n a d e q u a t e  p l a n a r i z a t i o n; i n a d e q u a t e  r e s i s t  a d h e s i o n;


i n a d e q u a t e  r e s i s t  e t c h  r e s i s t a n c e; i n a d e q u a t e  r e s o l u t i o n; i n a d e q u a t e  s t e p  c o v e r a g e; i n c o r r e c t  e d g e  c o n t o u r; i n c o r r e c t


l i n e w i d t h; i n t r u s i o n s; m i s a l i g n m e n t; m i s s i n g  i m a g e s; m o u s e  b i t e s; n e c k d o w n s; n o t c h i n g; o p a q u e  s p o t s; o v e r e x p o s u r e;


p a r t i c u l a t e  c o n t a m i n a t i o n; p a t t e r n  d i s c o n t i n u i t i e s; p a t t e r n  d i s t o r t i o n; p i n h o l e s; p o o r  r e s i s t  e t c h  r e s i s t a n c e; p o o r  r e s i s t


t h i c k n e s s  u n i f o r m i t y; p r o t r u s i o n s; r e s i s t  t o o  t h i c k  o r  t o o  t h i n; r o u g h  e d g e s; r o u n d i n g; s c r a t c h e s; s c u m m i n g; s p a c i n g


v i o l a t i o n s; u n d e r e x p o s u r e


4. D i f f u s i o n:


a l k a l i  c o n t a m i n a t i o n; b a n d g a p  n a r r o w i n g; b o r o n  p e n e t r a t i o n  t h r o u g h  o x i d e; c r y s t a l l o g r a p h i c  d a m a g e; d i f f u s i o n


p i p e s; d i s l o c a t i o n s; d o p a n t  p r e c i p i t a t i o n; e m i t t e r  p u s h; h e a v y  m e t a l  c o n t a m i n a t i o n; i n a d e q u a t e  u n i f o r m i t y; l a t e r a l l y


e n h a n c e d  d i f f u s i o n; l i q u i d-p h a s e  p e n e t r a t i o n  o f  o x i d e  m a s k; p o p c o r n  n o i s e; s h e e t  r e s i s t i v i t y  t o o  h i g h; s h e e t  r e s i s t i v i t y  t o o


l o w; s l i p; j u n c t i o n s  t o o  d e e p  o r  t o o  s h a l l o w


132ReliabilityandFailureofElectronicMaterialsandDevices


5. I o n  i m p l a n t a t i o n:


c h a r g e  b u i l d u p; c o n t a m i n a n t s  i n  i m p l a n t  b e a m; i n a d e q u a t e  d o s e  u n i f o r m i t y; i n c o r r e c t  d e p t h; i n c o r r e c t


d o p a n t  s p e c i e s; i n c o r r e c t  d o s e; i n c o r r e c t  i m p l a n t  a n g l e; m e t a l l i c  c o n t a m i n a t i o n; n e u t r a l  s p e c i e s  i n  i m p l a n t  b e a m;


o v e r h e a t i n g; p a r t i c u l a t e  c o n t a m i n a t i o n; p e n e t r a t i o n  i n t o  u n d e r l y i n g  d e v i c e; s e m i c o n d u c t o r  l a t t i c e  d a m a g e


6. T h e r m a l  t r e a t m e n t:


a l k a l i  i o n  c o n t a m i n a t i o n; c a r b o n  c o n t a m i n a t i o n; h e a v y  m e t a l  c o n t a m i n a t i o n; i n c o r r e c t  a m b i e n t;


i n c o r r e c t  c o o l i n g  o r  h e a t i n g  r a t e; i n c o r r e c t  t e m p e r a t u r e; i n c o r r e c t  t i m e; p a r t i c u l a t e  c o n t a m i n a t i o n; s l i p; t h e r m a l  p i t t i n g


7. C l e a n i n g:


a l k a l i  i o n  c o n t a m i n a t i o n; e x c e s s i v e  e t c h i n g; h e a v y  m e t a l  c o n t a m i n a t i o n; i n c o m p l e t e  c o n t a m i n a n t  r e m o v a l;


p a r t i c u l a t e  c o n t a m i n a t i o n; p i t t i n g; r a d i a t i o n  d a m a g e; s c r a t c h e s; s i l i c o n  c r y s t a l l o g r a p h i c  d a m a g e


8. W e t  c h e m i c a l  e t c h i n g:


a l k a l i  i o n  c o n t a m i n a t i o n; c o r r o s i v e  r e s i d u e; f r e c k l e s (u n e t c h e d  p r e c i p i t a t e s); h e a v y  m e t a l


c o n t a m i n a t i o n; i n s o l u b l e  r e s i d u e; l o c a l  c e l l  e t c h i n g; l o s s  o f  r e s i s t  a d h e s i o n; n o n u n i f o r m  e t c h i n g; o v e r e t c h i n g; p a r t i c u l a t e


c o n t a m i n a t i o n; p h o t o m a s k  e r o s i o n; p h o t o v o l t a g e  e f f e c t s; p i t t i n g; p o o r  e t c h  r a t i o; p o o r  w e t t i n g; s t a i n i n g; u n d e r c u t t i n g;


u n d e r e t c h i n g; w r o n g  e t c h  r a t e


9. P l a s m a  e t c h i n g:


c h a r g e  b u i l d u p; c o r r o s i v e  r e s i d u e s; e x c e s s i v e  e t c h i n g  o f  s u b s t r a t e; e x c e s s i v e  l o a d i n g  e f f e c t s; e x c e s s i v e  r e s i s t


e r o s i o n; e x c e s s i v e  v a r i a t i o n  i n  i n d u c t i o n  t i m e; f r e c k l e s (u n e t c h e d  p r e c i p i t a t e s); g r a s s; h y d r o g e n  d o n o r  e f f e c t s  i n  S i;


i n a d e q u a t e  e t c h  r a t i o s; i n c o r r e c t  e d g e  a n g l e; i n s u f


c i e n t  a m o u n t  o f  e t c h i n g; i o n i c  c o n t a m i n a t i o n; l o w  s e l e c t i v i t y; m e t a l l i c


c o n t a m i n a t i o n; n o n u n i f o r m  e t c h i n g; o v e r e t c h i n g; p o o r  e t c h i n g  u n i f o r m i t y; r a d i a t i o n  d a m a g e; r a d i a t i o n  d a m a g e  t o  S i O


;


r e s i d u e  i n  e t c h e d  o p e n i n g s; r e s i d u e  o n  s i d e w a l l s; s i l i c o n  c r y s t a l  d a m a g e; s t r i n g e r s; u n d e r c u t t i n g; u n d e r e t c h i n g


1 0. C V D:


d e v i t r i


c a t i o n; e t c h  r a t e  t o o  h i g h; e x c e s s i v e  c o m p r e s s i v e  s t r e s s; e x c e s s i v e  h y d r o g e n  c o n t e n t; e x c e s s i v e  t e n s i l e  s t r e s s;


e x c e s s i v e l y  h y d r o s c o p i c; i n s u f


c i e n t  c o n f o r m a l i t y; l o c a l i z e d  e t c h  r a t e  a t  s t e p  t o o  h i g h; n o n u n i f o r m  t h i c k n e s s; n o t


s t o i c h i o m e t r i c; t o o  t h i c k  o r  t o o  t h i n; w r o n g  c o m p o s i t i o n


1 1. M e t a l l i z a t i o n:


b l a c k  g o l d; c o n t a i n s  v o i d s; d u c t i l i t y  t o o  l o w; e x c e s s i v e  n a t i v e  o x i d e  i n  c o n t a c t s; e x c e s s i v e  o x i d e  c o n t e n t  i n


m e t a l; e x c e s s i v e  o x y g e n  i n  i n i t i a l l y  d e p o s i t e d  r e g i o n; e x c e s s i v e  r o u g h n e s s; h i g h  s h e e t  r e s i s t i v i t y; h i l l o c k s; i n-p r o c e s s  r a d i a t i o n


d a m a g e; l o w  r e s i s t i v i t y  r a t i o; m i c r o c r a c k s; p o o r  a d h e s i o n; p o o r  s t e p  c o v e r a g e; p o o r  t h i c k n e s s  u n i f o r m i t y; s u s c e p t i b l e  t o


c o r r o s i o n; s u s c e p t i b l e  t o  e l e c t r o m i g r a t i o n; t o o  t h i c k  o r  t h i n; w r o n g  a l l o y  c o m p o s i t i o n


F r o m  R e f. [1 8].


Defects,Contaminants,andYield133


released like a jack-in-the-box. Simply machining a thin surface layer from the rolled metal surface will upset the mechanical equilibrium and cause the remaining material to bow. Residual stresses also arise in castings, heattreated glass, and machined and ground materials.


A more pertinent example of residual stress occurs in silicon wafers whose backsides are thinned by grinding prior to dicing [19]. Thinner wafers facilitate dicing, dissipate heat better, and make for thinner packages.


Unfortunately, grinding induces stresses that cause wafers to warp and more easily break during the dicing process. Furthermore, warped dies are more difﬁcult to electrically contact and mount in the package. All in all, yield can suffer appreciably due to warped wafers. This underscores the importance of understanding and controlling stress.


3.3.2.1 Internal Stress


We all know that stresses and strains will develop throughout a body when forces are applied to it. Under elastic loading conditions, the stresses and strains disappear upon unloading. But materials that are plastically deformed or heated may sometimes contain residual stresses even when the plastic load or heat is removed. Furthermore, what are we to make of processed wafers that are internally stressed, even though no mechanical forces were ever applied to them? Such situations arise all too frequently in thin ﬁlms attached to substrates, and in these cases internal or residual stresses are said to exist. Internal stresses have important implications in inﬂuencing product yield as well as subsequent reliability. There are two main sources of internal stress, and each will be discussed in turn.


3.3.2.2 Extrinsic Residual Stress


These stresses, commonly called thermal stresses, originate from the thermal expansion or contraction of materials when they are mechanically constrained.


To seehow thermal stress candevelop in ahomogeneous body, consider a rodof length Lo clamped at both ends. If its temperature is raised fromTo toT, the rod would tend to expand in lengthby an amount equal toa (T To)Lo,wherea isthe coefﬁcient of thermal expansion deﬁned bya¼DL/Lo(T To) (K1). Butthe rod is constrained and is, therefore, effectively shortened in compression.


The compressive strain is simply e¼DLo/Lo¼a(T To) Lo/Lo or a(T To). By Hooke’s law a stress s develops that is given by Ee, where E isthe modulus of elasticity. Therefore, combining terms (neglecting signs) yields


s ¼ EaðT  ToÞ:


(3.5)


Processing of IC chips generally involves bi- and multilayers of different materials, and a number of failure and reliability problems discussed in this book can be attributed to internal or residual stresses in such structures.


Even the outwardly homogeneous ground silicon wafer discussed above is an effective bilayer consisting of a thin stressed surface layer and the contiguous bulk with a stress of opposite sign. Internal stresses invariably develop in ﬁlm/substrate combinations because of thermal mismatch between the ﬁlm and substrate at the ﬁlm formation and use temperatures. To see why, we assume that the ﬁlm is stress free at the elevated deposition temperature T, and that af> as. As the ﬁlm cools to room temperature To,it contracts more than the substrate, as shown in Figure 3.12(a). Regardless of the resultant stress distribution that prevails, the structure must be in mechanical equilibrium. This requires that both the net force (F)and bending moment (M) vanish on every ﬁlm/substrate free body crosssection. Thus


F ¼ZsdA ¼ 0


(3.6)


M ¼ZsydA ¼ 0;


(3.7)


Figure 3.12 (a) Development of residual tensile stress in a ﬁlm when af> as. (b)Development of residual compressive stress in a ﬁlm when af< as. (From Ref. [20].)Defects, Contaminants, and Yield 135


where A is the sectional area and y is the moment arm. Compatibility demands that both the ﬁlm and the substrate have the same length. A compromise is struck, and the ﬁlm stretches while the substrate contracts by an equal amount to keep the overall length identical in each.


However, the combination is still not in mechanical equilibrium because there is still an unbalanced end moment. To compensate, the ﬁlm/substrate pair elastically bends as shown if not restrained from moving.


Thus, ﬁlms containing internal tensile stresses bend the substrate concave upward. In an entirely analogous fashion, compressive stresses develop inﬁlms that tend to thermally contract less than the substrate. Internal compressive ﬁlm stresses, therefore, now bow the substrate convex downward (Figure 3.12(b)). These results are perfectly general regardless of the speciﬁc mechanisms that cause ﬁlms to stretch or shrink relative to substrates. Sometimes, the tensile stresses are sufﬁciently large to cause ﬁlm fracture. Similarly, excessively high compressive stresses can cause ﬁlm wrinkling and local loss of adhesion to the substrate. Examples of both effects are shown in Figure 3.13.


The magnitude of the thermal stress developed in the ﬁlm is given by [20]


s ¼


1 nf½af  as ðT  ToÞ;


15. Distinguish between the functions of (a) microprocessor and memory


chips, (b) DRAMs and SRAMs, (c) charge-coupled devices and


DRAMs, (d) gate capacitor and trench capacitor.


16. When zero bias is applied in the HEMT structure, the conduction


band edge in the GaAs lies below the Fermi level, implying a large


density of the 2-D electron gas.


a. What do you expect to happen when the gate is biased negatively?


b. Draw band diagrams for both zero and negative bias.


Electronic Devices: How They Operate and Are Fabricated 107


17. When compared to silicon device technology, compoundsemiconductor laser production involves may fewer steps and generally


more art. If this is so, what are the reliability implications of such


products?


18. Some polymers degrade upon exposure to radiation due to bond


breaking. Covalent bond energies for some important atomic pairings


are:


Bond pair Energy (kJ/mol) Bond pair Energy (kJ/mol)


CeC


340


CeH


420


620


CeCl


330


What portion of the electromagnetic spectrum would be expected to cause radiation-damage effects in each bond type?


19. Damage to opto-electronic devices and materials often stems from


recombination of electron–hole pairs without photon emission (nonradiative recombination) and from self-absorption of the involved radiation. Explain how each phenomenon could cause degradation.


[1] S.M. Sze, Semiconductor Devicesdphysics and Technology, Wiley, New York, 1985.


[2] B.G. Streetman, Solid State Electronic Devices, fourth ed., Prentice Hall, Engelwood


Cliffs, NJ, 1995.


[3] J.M. Mayer, S.S. Lau, Electronic Materials Sciencedfor Integrated Circuits in Si and


GaAs, Macmillan, New York, 1990.


[4] A. Bar-Lev, Semiconductors and Electronic Devices, third ed., Prentice Hall, Engelwood Cliffs, NJ, 1993.


[5] T.M. Fredericksen, Intuitive IC Electronics, second ed., McGraw Hill, New York,


1989.


[6] S.M. Sze (Ed.), VLSI Technology, second ed., McGraw Hill, New York, 1988.


[7] S. Middleman, A.K. Hochberg, Process Engineering Analysis in Semiconductor Device


Fabrication, McGraw Hill, New York, 1993.


[8] W.S. Ruska, Microelectronic Processing, McGraw Hill, New York, 1987.


[9] G.E. Anner, Planar Processing Primer, Van Nostrand Reinhold, New York, 1990.


[10] R.C. Jaeger, Introduction to Microelectronic Fabrication, vol. V, Addison-Wesley,


Menlo Park, CA, 1988.


[11] B.R. Pamplin, in: R.C. Weast (Ed.), Handbook of Chemistry and Physics, CRC Press,


Boca Raton, FL, 1980.


[12] B. Myerson, IBM J. Res. Develop. 44 (3) (2000) 391.


[13] A. Schwerin, W. Hansch, W. Weber, IEEE Trans. on Electron Devices, ED-34 (1987)


2493.


[14] A.A. Iranmanesh, B. Bastani, IEEE Circuits Devices 8 (3) (1992) 14.


[15] H.J.M. Veendrick, MOS ICs-from Basics to ASICs, VCH Publishers, Weinheim,


1992.


[16] E. Adler, et al., IBM J. Res. Devel. 39 (1/2) (1995) 167.


[17] H.E. Mass, G. Groeseneken, H. Labon, J. Witters, Microelectronics J. 20 (1989) 9.


[18] W.T. Anderson, Tutorial Notes, IEEE International Reliability Physics Symposium,


7.1, 1992.


[19] W.J. Roesch, Tutorial Notes, IEEE International Reliability Physics Symposium, 1.1,


1988.


[20] A. Christou, Tutorial Notes, IEEE International Reliability Physics Symposium, 3.1,


1986.


[21] H. Morkoc, IEEE Circuits and Devices 7 (1991) 15.


[22] F. Magistrali, C. Tedesco, E. Zanoni, C. Canali, in: A. Christou (Ed.), Reliability of


Gallium Arsenide MMICs, Wiley, Chichester, 1992.


[23] W.T. Anderson, K.A. Christianson, C. Moglestue, Quality and Reliability Eng. Int. 9


(1993) 367.


[24] K. Wilson, GEC J. Res. 4 (1986) 126.


[25] A. Bensoussan, P. Coval, W.J. Roesch, T. Rubalcava. In: 32nd Annual Proceedings of


the IEEE Reliability Physics Symposium, 1994, p. 434.


[26] C.P. Skrimshire, J.R. Farr, D.F. Sloan, M.J. Robertson, P.A. Putland, J.C.D. Stokoe,


R.R. Sutherland, IEE Proc. Pt J 137 (1) (1990) 74.


[27] S.P. Sim, in: A. Christou, B.A. Unger (Eds.), Semiconductor Device Reliability,


Kluwer, Amsterdam, 1990.


[28] M. Fukuda, IEEE J. Lightwave Technol. 6 (1988) 1488.


[29] M. Fukuda, Reliability and Degradation of Semiconductor Lasers and LEDs, Artech,


Boston, 1991.


[30] J. Spencer, R. Koelbl, Tutorial Notes, IEEE International Reliability Physics Symposium, 1.1, 1989.


[31] R.W. Mann, L.A. Clevinger, P.D. Agnello, F.R. White, IBM J. Res. Develop. 39


(1995) 403.


[32] W. Zulehner, in: G. Harbeke, M.J. Schulz (Eds.), Semiconductor Silicon, P.2, Springer


Verlag, Berlin, 1989.


[33] A.B. Joshi, R. Mann, L. Chung, M. Bhat, H.T. Cho, B.W. Min, D.L. Kwong. In: 33rd


Annual Proceedings of the IEEE Reliability Physics Symposium, 1995, p. 156.


[34] C. Felsch, E. Rosenbaum. In: 33rd Annual Proceedings of the IEEE Reliability Physics


Symposium, 1995, p. 142.


[35] O. Joubert, A. Legouil, R. Ramos, M. Helot, O. Luere, E. Richard, G. Cunge,


T. Chevolleau, E. Pargon, L. Vallier, T. Morel, S. Barnola, T. Lill, J. Holland,


A. Patterson, AVS 22 (2006).


[36] Y.-C. Yeo, Q. Lu, P. Ranade, H. Takeuchi, K.J. Yang, I. Polischchuk, T.-J. King,


C. Hu, S.C. Song, H.F. Luan, D.-M. Kwong, IEEE Electron Device Lett. 22 (5)


(2001) 227.


[37] J.G. Ryan, R.M. Geffken, N.R. Poulin, J.R. Paraszczak, IBM J. Res. Develop. 39


(1995) 371.


[38] Intel Tech. J. 6 (2), 2002, p.10.


[39] T.N. Theis, IBM J. Res. Develop. 44 (3) (2000) 379.


[40] D. Sparks, S. Massoud-Ansari, N. Najaﬁ, Reliability, testing and characterization of


MEMS/MOEMS III, in: D. Tanner, R. Ramesham (Eds.), Proceeding SPIE 5343


(2004) 70.


[41] A. Margomenos, D. Peroulis, K.J. Herrick, and L.P.B. Katehi. European Microwave


Conference, 2001, p. 1.


[42] W.R. Ashurst, C. Carraro, R. Maboudian, IEEE Trans. Device Mater. Reliability 3 (4)


(2003) 173.


Electronic Devices: How They Operate and Are Fabricated 109


CHAPTER 3


Defects, Contaminants, and Yield


3.1 SCOPE


There are defects and defects, and there are killer defects!! From the relatively innocuous to those that immediately disqualify an integrated circuit (IC)chip, this chapter is largely concerned with the nature of defects, their generation during processing, strategies used to minimize their inﬂuence,and how they adversely inﬂuence product yield. In Chapter 2 we described how a failure could be hastened by a damaged area. We will now negotiate the mirky waters between an IC that fails at ﬁnal test and one that passes but is doomed to early failure. The harmful effects of crystallographic, structural, compositional, or stoichiometric defects strongly depend on the nature of the material they inhabit. For example, metals are usually far more tolerant of point defects, dislocations, and grain boundaries (GB) than are semiconductors. Semiconductors must be free of dislocations and GBs,whereas metallizations contain these in relatively large densities with little ill effect. And, since the matrices of most ceramics and dielectrics used in microelectronics are already amorphous or ﬁne grained, these same crystallographic defects usually affect properties only marginally, if at all.


At the next level there are defects that represent gross deviations in the structural and chemical integrity of the material over macroscopic dimensions. They include voids, precipitates, missing or misformed structural features because of lithographic errors, deformed or even cracked structures due to stress, and particulate contaminants. Such defects may or may not cause devices or ICs to immediately fail inspection, and might or might not be a source of reliability problems.


Killer defects, however, immediately cause rejection of the product. It does not take a very large defect to become a killer defect if it is strategically located,such as at a semiconductor junction or on a lithography mask. The most troubling aspect is that as circuit features continue to get ever smaller, killer defect sizes shrink in concert. As a rough guide, the “1/3 rule” [1] suggests that the killer defect size scales as one-third the minimum feature size.


The general problem of defects can be put into perspective by considering DRAM chips, the primary driver of microelectronics technology. On the


http://dx.doi.org/10.1016/B978-0-12-088574-9.00003-3


All rights reserved. 111


# 3 . Defects, Contaminants, and Yield


## 3.1 Scope


basis of the 1/3 rule, the killer defect size is estimated to be w0.06 mm for 256-Mb DRAMs (2000), w0.05 mm for 1-Gb DRAMs (2003), and only w0.03 mm for 4-Gb DRAMs (2007). About 700 distinct processing steps are now required to produce advanced DRAM chips. Among these are over 25 lithographic steps, which must be carried out in a manner such that production yields of chips passing ﬁnal inspection are high. At every step in the process there are obstacles, or shall we say opportunities, that have the potential to cause defective products.


Concern over processing defects is perhaps the chief technical preoccupation of manufacturing industries. Survival in the marketplace often hinges on identifying defects and developing and implementing strategies to eliminate them. Defects are intrinsic to processing, and a process devoid of defects does not yet exist.


In what must be regarded as one of the more important chapters in the book, aspects of IC manufacturing are explored again with particular emphasis placed onprocessingdefects and their consequences.Defects not only inﬂuence production costs directly but also reliability concernsmore indirectly; those that go undetected in qualiﬁed products at ﬁnal test are like seeds that can sprout under certain circumstances to yield a bitter reliability harvest.


This chapter starts by introducing crystallographic defects and their role in Si and GaAs. Subsequent topics continue the treatment of chip-level processing introduced at the end of Chapter 2, paying particular attention to cataloging processing defects. Speciﬁc examples are incorporated explaining the role of stress and highlighting the deleterious role of ubiquitous contaminants. Lastly,the integrated statistical effect of defects on process and product yield ismodeled.


While it is impossible to carry out manufacturing processes without incorporating defects, the latter are for the most part removed by inspection and ﬁnal test, or by screening. And those that pass into the released (sold)product are often “cosmetic” and more benign in service than the impression sometimes conveyed by this chapter. With this caveat we start with a discussion of defects in crystalline solids and semiconductors.


3.2 DEFECTS IN CRYSTALLINE SOLIDS AND


SEMICONDUCTORS


3.2.1 General Considerations


All crystalline materials contain intrinsic (lattice) defects such as vacancies,dislocations, and GBs. These defects are deﬁned with examples in Table 3.1.


For the uninitiated it appears tempting to attribute failures and reliability


## 3.2 Defects in Crystalline Solids and Semiconductors


### 3.2.1 General Considerations


I m p e r f e c t i o n s  i n  c o n d e n s e d  m a t t e r


C l a s s i


c a t i o n  D e


n i t i o n  E x a m p l e s


V i b r a t i n g  a t o m  T e m p o r a r y, s m a l l  d i s p l a c e m e n t  f r o m  i d e a l  p o s i t i o n  Z e r o  p o i n t, t h e r m a l


E l e c t r o n i c  c h a r g e  C h a r g e  c a r r i e r  e x c i t e d  f r o m  g r o u n d-s t a t e  b o n d i n g


c o n


g u r a t i o n


E l e c t r o n (


), h o l e (


), e x c i t o n


C h e m i c a l  i m p u r i t y  F o r e i g n  a t o m  o f  d i f f e r i n g  s i z e, v a l e n c e, e l e c t r o n e g a t i v i t y,


a n d/o r  s t r u c t u r e  r e l a t i v e  t o  h o s t  a t o m s/s t r u c t u r e


S u b s t i t u t i o n a l, i n t e r s t i t i a l


P o i n t  l a t t i c e  d e f e c t  M i s s i n g  h o s t  a t o m, e x t r a  h o s t  a t o m, a t o m  o c c u p y i n g  w r o n g


l a t t i c e  s i t e


L a t t i c e  v a c a n c y, s e l f-i n t e r s t i t i a l,


a n t i s i t e  d e f e c t (c o m p o u n d s)


N o n b r i d g i n g  b o n d (N o n c r y s t a l l i n e  m a t e r i a l s)


O n e-d i m e n s i o n a l  d e f e c t  R o w  o f  a t o m s  a t  t h e  e d g e  o f  e x t r a  h a l f-p l a n e  o f  a t o m s  D i s l o c a t i o n (e d g e  a n d  s c r e w)


T w o-d i m e n s i o n a l  d e f e c t  B o u n d a r y  s e p a r a t i n g  a n  e r r o r  i n  s t a c k i n g  s e q u e n c e  o f  a t o m i c


p l a n e s, b o u n d a r y  b e t w e e n  t w o  c r y s t a l s  o f  d i f f e r e n t  r e l a t i v e


o r i e n t a t i o n


S t a c k i n g  f a u l t, G B


T h r e e-d i m e n s i o n a l


d e f e c t


M a c r o s c o p i c  r e g i o n  o f  d i f f e r e n t  d e n s i t y, c h e m i c a l  c o n t e n t,


c o o r d i n a t i o n, e t c.


, f r o m  h o s t


V o i d, f r e e  v o l u m e  f o r  g l a s s e s,


d i s o r d e r, d e f e c t  c l u s t e r,


p r e c i p i t a t e


F r o m  R e f. [2].


Defects,Contaminants,andYield113


problems in electronic materials to the role of such defects, and at one level such an assumption has validity. In practice, however, the evidence leading from microscopic defects to macroscopic failures is usually very tenuous, and few of the latter can unambiguously be attributed to the former. Complicating matters further are the processing defects, introduced during various steps of the manufacturing sequence. These are grosser in scale than lattice defects and strongly inﬂuence yield and malfunction of devices. Returning to lattice defects, the rationale for studying them is to intelligently assess their potential and actual roles as root causes of failures, even though it may be difﬁcult to draw causal relationships.


3.2.2 Point Defects


The vacancy or absence of an atom at a lattice site is the most basic defect.


Vacancies occur in all classes of solids. Not surprisingly, because the movement of atoms from one location to another (diffusion) requires vacancies, and because diffusion is easier at higher temperature, we ﬁnd that the fraction or concentration of vacant lattice sites (Cv) is given by the familiar temperature-dependent Boltzmann expression


Cv ¼ exp EfkT 0


(3.1)


where Ef is the energy required to form a vacancy, i.e., remove an atom from the bulk and place it on the surface. This equation, predicted from thermodynamic considerations, has been experimentally veriﬁed in all classes of solids. As temperature increases so does the atomic vibrational frequency, atom spacing, and concentration of vacancies. One of the most damaging effects vacancies exhibit is the formation of voids, usually at an interface between differing materials. Such damage is generally attributed to the condensation of very large numbers of vacancies.


The chief difference between point defects in metals and semiconductors is that the latter are generally electrically active. Charge activity arises from the four severed dangling covalent bonds surrounding the vacancy in the diamond cubic lattice of Figure 3.1. In contrast, the very mobile free electrons rapidly smooth any charge singularities associated with vacancies in metals.


An initially uncharged vacancy V o in a Si lattice can act as an acceptor by acquiring an electron so that it becomes V . Similarly, it can acquire a positive charge by combining with a hole and become V þ. One can also envision neutral vacancies acquiring more than a single net charge, so that


V 2, V 3, V 2þ, V 3þ, etc., species can exist. Concentrations of such vacancies depend on carrier concentrations because vacancy–charge interactions can be viewed from the standpoint of chemical equilibrium,e.g., [V ]/(n[V o])¼K. Here we note that n and p are electron and holeconcentrations, and that K is the equilibrium constant.


There are other defects associated with impurity atoms (Au, Fei, Mo,Ni) or impurity–impurity pairs (Fei–B) that are electrically active in Si. The subscript i denotes an atom occupying an interstitial site. Similar impurity atom defects have been identiﬁed in GaAs (e.g., Fe, Cu) and InP (e.g., Zn).


Just as with traditional dopants, these defects have energy levels within the forbidden gap and can act as donors or acceptors. A difference is the much deeper (ionization) energies in the gap relative to standard dopants. To study such low defect concentrations (i.e., 1010–1014/cm3) use has been made of deep-level transient spectroscopy (DLTS). This technique relies on excitation of charge emission from defects located within the capacitance region of a p–n junction and detection of the resulting current decay to equilibrium [3]. Signiﬁcantly, DLTS has been installed in the manufacturing environment to monitor trace contamination during deposition of epitaxial ﬁlms.


Other semiconductor defects include vacancy–interstitial pairs or Frenkel defects and antisite defects, which occur in II–VI and III–V compounds. These are characterized, for example, by a Ga atom on an As site within the As sublattice, and similarly misplaced As atoms on the Ga sublattice.


Figure 3.1 Schematic of diamond cubic lattice and broken bonds around a vacancy (V).


Defects, Contaminants, and Yield 115


3.2.2.1 Effect on Diffusion


Point defects play a role in elevated temperature doping, sintering of metal–semiconductor contacts, postannealing of ion implants, and epitaxial deposition. All involve diffusion of atoms, and such processes are complicated in semiconductors. During doping, for example, concentrationdependent diffusion effects arise that can be attributed to pair interactions between charged as well as uncharged vacancies and dopants or impurities.


To illustrate the complexity involved, an expression for the extrinsic(impurity) diffusion coefﬁcient (Dex) is [4]


Dex ¼ Doi þDþip=niþDin=niþD2i ðn=niÞ2 þD3i ðn=niÞ3: (3.2)Thus Dex depends on the doping concentration levels that yield n or p,as well as the carrier concentration (ni) in dopant-free or intrinsic Si. In order of appearance in Eqn (3.2), the various Di terms represent the intrinsic diffusivity of impurity interaction with neutral point defects, a singlycharged donor point defect, a singly-charged acceptor point defect, a doubly-charged acceptor point defect, and a triply-charged acceptor point defect. Since n and p directly reﬂect the doping concentration (C), this complex expression suggests that Dex depends nonlinearly on C such that DexwCa, with a¼ 1,2,3. Therefore, doping proﬁles are far morecomplex than those identiﬁed with a linear diffusion theory, where D is independent of concentration (see Section 5.2).


Examples of anomalous dopant diffusion effects and proﬁles are shown in Figure 3.2(a) and (b). It is evident that the concentration proﬁles of arsenic,boron, and phosphorous deviate from the well-known complementary error function solution that characterizes linear diffusion (Eqn (5.3)) from a constant surface source. The case of the heavily doped phosphorus proﬁle in a diffused emitter (Figure 3.2(b)) is particularly interesting.Near the surface, phosphorus atoms associate with vacancies. But dissociation of this (PV) complex via the reaction (PV)/ Pþ þ V þ e releases vacancies in the proﬁle tail. Theenhanced diffusion induces the observed kink in the proﬁle that causes the socalled emitter-push effect in n–p–n narrow-base, diffused-bipolar transistors.


Typically, the boron-diffused base just under the emitter isw0.2 mm deeper than outside the emitter region (Figure 3.3(a)) because vacancies enhance boron diffusion as well.


Dopant diffusion proﬁles are also altered at junctions or near surfaces and interfaces particularly when oxygen is present. Consider a junction near the surface of a Si wafer patterned by a silicon nitride mask to expose windows for oxidation. For dopants like B, P, and As, diffusion is enhanced,


and the junction moves deeper into the wafer under the window than under the nitride, which is an effective barrier to oxygen penetration(Figure 3.3(b)). Under the same conditions, however, the diffusion of Sb is retarded (Figure 3.3(c)), resulting in a shallower junction. In another effect,shown in Figure 3.3(d), lateral diffusion of dopant enhances the junction depth (xj) under nitride ﬁlms during oxidation. The smaller w is, the larger is xj. An explanation of these effects assumes that Si (self) interstitials are injected into Si during oxidation in order to simultaneously accommodate the volume expansion stemming from oxide formation and reduce the interfacial stress that is generated. Semiconductor point defects include interstitials, and like vacancies, they may occur in nonequilibrium concentrations. Dopants (B and P) that prefer to use interstitials to facilitate


Figure 3.2 (a) Normalized diffusion proﬁles for arsenic and boron in silicon. The error function (erfc) solution is compared with actual proﬁles corresponding to concentration-dependent D values. Note that Cs is the surface concentration and y/yj is related to x/xj where xj is the junction depth. (b) Phosphorous diffusion proﬁles in silicon. Deviation from the erfc proﬁle (a) occurs at successively higher surface concentrations (b, c, d), where ultimately kinks develop. (From Ref. [5].)


Defects, Contaminants, and Yield 117


mass transport show oxidation-enhanced diffusion, while the opposite is true for Sb, which diffuses via a vacancy mechanism.


Calling these enhancements and retardations of dopant concentration processing defects is perhaps too strong an attribution. Even though they alter the intended device behavior, their effects can be designed around in most cases.


3.2.2.2 Oxygen in Crystalline Silicon


It was the fate of silicon, aluminum, and oxygen, the most abundant elements on earth, to be brought together in the minutest of amounts to make ICs possible. While these elements play unambiguously beneﬁcial roles in semiconductor, conductor, and insulator functions, the presence of oxygen within silicon is like a “two-edged sword” [6] as far as device behavior is concerned. Oxygen enters Czochralski process (CZ)-grown crystals because the melt continually erodes and dissolves the SiO2 crucible


Figure 3.2dCont'd.


wall during crystal pulling. A snapshot of the way defects enter the pulled crystal is schematically conveyed in Figure 3.4. Point defects present in solid solution at the highest temperatures promote the nucleation and growth of dislocation defects and oxide precipitates as the crystal cools.


Within crystalline Si, oxygen reveals its many-faceted behavior depending on temperature. When dissolved, oxygen occupies an interstitial site and is electrically inactive. Upon heating silicon to various temperature ranges,the changes that occur are summarized in Table 3.2. When oxygeninduced defects are retained in wafers at room temperature, they can be a source of considerable concern.


3.2.2.3 Gettering


Treatments that remove process-induced contaminants from the active regions of the Si wafer, where devices are being fabricated, are known as gettering [2]. Metal contaminants are the particular targets of gettering processes because they, in combination with precipitates at dislocations and stacking faults, cause excessive leakage currents and low junction breakdown voltages. There are two types of gettering.


Figure 3.3 Collection of anomalous diffusion effects and proﬁles, where xj (i) and xj (f)are the initial and ﬁnal junction positions, respectively. (a) Emitter-push effect. (b)Dopant diffusion enhancement under the window relative to the nitride. (c) Dopant diffusion retardation under the window relative to the nitride. (d) Lateral diffusion enhancement.


Defects, Contaminants, and Yield 119


Figure 3.4 Defect interactions and precipitation reactions in CZ-grown silicon single crystals as a function of temperature.


Table 3.2 Oxygen effects in CZ-grown silicon


Temperature


range


State of oxygen


400e500 C Electrically active, oxygen-related donors formed due to small oxygen complexes


600e700 C First visible evidence of oxygen precipitation, rodlike coesite(SiO2) structures and 2-nm amorphous precipitates identiﬁed 800e1000 C Platelike amorphous structures in the size range 10e500 nm 1000 C


Platelike precipitates accompanied by punched-out prismatic dislocation loops and ESF with associated precipitate


colonies


1200 C


Large polyhedral precipitates identiﬁed as being amorphous,plus large stacking faults


From Ref. [2], p. 223.


3.2.2.3.1 Extrinsic (or External)


In this case gettering is achieved by deliberately introducing trapping sites in the backside of the Si wafer. Through surface damage produced by mechanical abrasion, ion implantation, or laser beam heating and cooling,dislocations are generated. At high temperatures (w1000 C) these defects attract harmful metals such as Cu, Fe, Ni, and Cr, which diffuse to them from the active device regions. The kinetics of gettering depends on the rates of impurity release from the associated state, as well as diffusion to and capture by the getter site.


3.2.2.3.2 Intrinsic (or internal)


Intrinsic gettering is employed to remove both harmful oxygen and metallic elements through heat treatment alone. First, wafers should ideally contain an oxygen concentration of about 8.5 1017 cm3. After an elevated temper-ature solution heat treatment the wafers are cooled, and oxygen precipitates from solid solution in the form of SiO2 particles. These plastically compress the lattice, locally generating dislocations and stacking faults that tie up impurities in the manner described above for extrinsic gettering. In bipolar and complementary metal oxide–semiconductor (CMOS) technologies, which require higher process temperatures and a larger number of processing steps compared to conventional NMOS technology, attention must be paid to the problem of wafer warpage during thermal treatments [7].


The trick in either case is to locate the precipitates far from the devices.


This can be accomplished in a three-step, high–low–high temperature annealing sequence [8]. First the wafer surface is deoxidized at w1100 C.


Outdiffusion and evaporation of oxygen reduces its level to the solubility limit, creating a so-called denuded zone. Annealing times are chosen to extend the denuded zone beyond the position of the deepest p–n junctions to be fabricated. Next, the wafer temperature is reduced to w700 C, which forces oxygen to be expelled from supersaturated Si to nucleate precipitates.


Times ranging froma fewhours to a fewdays are required to do this optimally.


Lastly, a high-temperature anneal in the range 1000–1200 C is required for precipitate growth, dislocation formation, and diffusion of atoms to traps.


Often this complex gettering treatment is performed in conjunction with extrinsic gettering.


3.2.3 Dislocations


These well-known defects extend along a line of atoms in a crystalline matrix. Dislocations exist in all classes of solids but are most easily visualized


Defects, Contaminants, and Yield 121


in cubic lattices. There are two fundamental types of dislocationsdthe edge and screw. Forming an edge dislocation by inserting an extra row of atoms into the diamond cubic lattice of silicon leaves a line of dangling bonds in its wake as shown in Figure 3.5(a). These bonds are generally viewed as acceptors that capture electrons to lower their overall energy. But now a hole can be trapped, and in the recombination that occurs, the captured electron is annihilated. The original high electron energy state is restored,and the process can repeat. This is the reason that dislocations are viewed as carrier generation–recombination centers. Cores of such dislocations are thus negatively charged and surrounded by a cylinder of positive space charge. This would confer inverted p-type behavior near the dislocation in an otherwise n-type matrix.


Dislocations in compound semiconductor lattices, depicted in Figure 3.5(b), are more complex than in Si because two atoms (A and B) are now involved. There are now different core charges depending on whether A or B surfaces are exposed. Dangling A bonds, for example, might produce a positive core charge. Dislocations in compound semiconductors have been known to reduce the lifetime of laser diodes, affect the threshold voltage of ﬁeld-effect transistors, and reduce electron–hole recombination processes that lead to radiation of light.


Figure 3.5 (a) Edge dislocation in the diamond lattice. (b) Dislocations in AB compound semiconductor lattice. (From Ref. [9].)


3.2.3.1 Electrical Effects of Dislocations


To better understand the electrical effects associated with dislocations, let us estimate the effective size of the dislocation depletion radius (rD) due to n-type doping to a level (ND). FollowingZolper andBarnett [10], Poisson’s equation in cylindrical coordinates, used to describe the electrical potential (V) that exists around the dislocation pipe of Figure 3.6(a) at any radius r, has the form


V2V ¼ r dr dr1rddrrdVdr¼ r-P-eNDεεo¼ eNDεεo


ID


dislocation center


inverted region


-1


V=0


dV


n=n


dr


d-y !6u


Winding


path囚旧


①


①一①①


Dislocation space-charge


u-high


pipes


p- low②①Q7


current


in-|om


-=0


r=0rc (5A)


(3.3)


Figure 3.6 (a) Charged dislocation pipe in cylindrical coordinates. (From Ref. [10].) (b)Current ﬂow around charged dislocations in semiconductors. The electron mobility is m and the resistivity is r. (From Ref. [9].)


Defects, Contaminants, and Yield 123


Here r is the charge density, e is the electronic charge, and 3and 3o are the dielectric constant and permittivity of free space, respectively. As boundary conditions, it is assumed that V (rD)¼ 0, and dV(rD)/dr¼ 0.Upon double integration and substitution of these boundary conditions,


V ðrÞ ¼ eND(2-mn)-(2-mr)}εεoEEOV()=={r2D2 ln rDr22 ln r(3.4)


Finally, at the dislocation core radius (rc), typically 0.5 nm, a potential Vi exists that causes inversion. Assuming Vi at rc (i.e., V(rc)¼Vi) we can thensolve for rD at any doping level by trial and error methods. Calculation shows that if Vi¼ 1 V, and ND¼ 2 1017 cm3, then rD¼ 44 shows that if Vj=1V, and ND=2x1017cm-3, then rD=44nm.nm.Physically, the dislocation core traps electrons and in the process is surrounded by a positively charged space charge region.


(3.8)


where nf is the Poisson ratio of the ﬁlm. Stresses of lower magnitude and opposite sign develop in the substrate. It should be noted that across aﬁlm/substrate couple the strains are continuous, but there is no such restriction on the stresses. Because the elastic moduli of ﬁlm and substrate differ, there is a stress discontinuity at the interface. Since two or more materials bonded to each other are involved in many applications, Eqn(3.8) is an important formula that is frequently quoted in the reliability literature. The right-hand side of this equation appears as a factor in virtually every thermal stress formula developed in connection with packaging and thermal cycling of IC chips during processing and use(see Chapter 8).


3.3.2.3 Intrinsic Residual Stress


In addition to thermally induced stresses, there are intrinsic sources of stress that are operative at any given temperature. In ﬁlms these stresses stem from growth processes, i.e., during epitaxy and structural evolution. Tensile stresses usually arise in metal and silicide ﬁlms from densiﬁcation


phenomena arising from coalescence of nuclei, recrystallization, and grain growth. In each case the ﬁlm shrinks relative to the substrate. On the other hand, hydration and ion implantation lead to compressive stress because they expand the ﬁlm relative to the substrate.


200PM10KU09336R


a(b)


Figure 3.13 Stresses in thin ﬁlms that lead to fracture. (a) Image of tensile cracks in a chromium ﬁlm electrodeposited on a nickel substrate that was subsequently pulled in tension. (b) Optical micrograph of crazes in a tungsten thin ﬁlm sputtered on a silicon substrate. Isotropic, compressive residual stresses with magnitudes of w1–3 GPa led to wormlike, wavy, and straight crack traces. Width of straight cracks is w60 mm.


(Courtesy of I.C. Noyan, IBM Corp.)


Defects, Contaminants, and Yield 137


There are complex reasons for the development of intrinsic residual strains, but in epitaxial ﬁlms they include differences in lattice constant or lattice misﬁt between ﬁlm and substrate. In producing high-quality epitaxialﬁlms of compound semiconductors it is critical that the lattice constants of the ﬁlm (af) and substrate (as) be as closely matched as possible. Lattice mismatch or misﬁt ( f ) is deﬁned as


f ¼ as  afaf;


(3.9)


which is the negative of the elastic strain, eE, required to make the ﬁlm register perfectly or epitaxially with the substrate. What happens during epitaxy is schematically indicated in Figure 3.14. When f is zero there is perfect homoepitaxy and no strain or stress. For small values of f, straining of interfacial ﬁlm–substrate atomic bonds is not sufﬁcient to nucleate dislocations, and the interface is defect free. However, for larger misﬁts the only way to reduce accumulated bond strain energy is to generate undesirable misﬁt dislocations at the interface. For devices not to display degraded electrical behavior, misﬁt values less than 0.001 are preferred.


Otherwise, misﬁt strain energy will accumulate internally as the ﬁlm grows until microstructural rearrangements in the form of dislocations


Figure 3.14 Schematic illustration of lattice matched, strained, and relaxed heteroepitaxial structures.


or stacking faults relieve this energy build up. These undesirable defects form at ﬁlm thicknesses of approximately b/(2f ), where b is the dislocation Burgers vector. This means that defects will typically appear afterw200 nm of ﬁlm growth if f¼ 0.001.A collection of defects that have been observed in epitaxial ﬁlms is displayed schematically in Figure 3.15. All, except for the oval defects,probably need no additional comment. The troublesome oval defects are faceted growth hillocks that nucleate at the ﬁlm–substrate interface, and they nest in the epitaxial layer. With a polycrystalline core bounded by four{111} stacking fault planes, they are present in densities as high as 1000/cm2 with sizes exceeding 1 mm. Their presence in GaAs ﬁlms has been attributed to surface contamination.


3.3.2.4 Manifestations of Internal Stress


3.3.2.4.1 Stress Magnitude


The magnitudes of the sum of the thermal and intrinsic internal or residual stresses in ﬁlms commonly employed in silicon technology are entered in Table 3.5. These data are representative, and it should be realized that stress values are subject to considerable scatter depending on how the ﬁlms were deposited. In dielectric ﬁlms, both positive and negative stresses less than 1 GPa in magnitude can be expected. Silicides,on the other hand, are stressed in tension to a level of several gigapascals.


Figure 3.15 Collection of crystallographic matrix defects in epitaxial ﬁlms displayed schematically. 1, Threading edge dislocations; 2, interfacial misﬁt dislocations; 3,threading screw dislocations; 4, growth spiral; 5, stacking fault in ﬁlm; 6, stacking fault in substrate; 7, oval defect; 8, hillock; 9, precipitate or void.


Defects, Contaminants, and Yield 139


Table 3.5 Residual stress values in ﬁlms encountered in Si devices Film Process


|SiO2 |Thermal |900-1200°C|-0.2 to -0.3|
|---|---|---|---|

|SiO2 |CVD 400 °C|40 nm/min |þ0.13 |

|SiO2 |SiH4 þ O2 |400 nm/min |þ0.38 |

|SiO2 |CVD |450°C|þ0.15 |

||TEOS |725 °C|þ0.02 |

|SiO2 |TEOS |685 °C|þ0.38 |

||TEOS þ25% B,P ||-0.02|

|SiO2 |Sputtered ||-0.15|

|Si3N4 |CVD |450-900°C|þ0.7 to þ1.2 |

|Si3N4 |Plasma |400°C|-0.7|

|||700°C|þ0.6 |

|Si3N4 |Plasma 13.56 MHz |150°C|-0.3|

|||300 °C|þ0.02 |

|Si3N4 |Plasma 50 kHz |350 °C|-1.1|

|Poly Si |LPCVD |560-670°C|-0.1 to -0.3|

|TiSi2 |PECVD |As-deposited |þ0.4 |

|||Annealed |þ1.2 |

|TiSi2 |Sputtered ||þ2.3 |

|CoSi2 |Sputtered ||þ1.3 |

|TaSi2 |Sputtered |800 °C anneal|þ3.0 |

|TaSi2 |Sputtered ||þ1.2 |

|W |Sputtered |200e400 W power |+2 to -2|

|W |Sputtered |5e15 mTorr Ar pressure |-3 to +3|

|Al |||þ0.5 to wþ1 |

Conditions


Stress (GPa)


B,P; PECVD; TEOS, tetraethyl orthosilicate.


Data are mostly from Ref. [21], R60.


Example 3.1


What is the thermal stress in thermally grown SiO2 ﬁlms on Si when the difference between growth and ambient temperatures is T To¼ between growth and ambient temperatures is T- To=900K?900K?Answer The extrinsic stress is given by s ¼ ESiO2=ð1 nSiO2Þ ½aSiO2 aSiÞ ðT  Answer The extrinsic stress is given by a = Esio2/(1 - vsio2) [asio2 - asi)] (T - To).ToÞ.Taking the values ESiO2¼ 83 GPa; nSiO2¼ 0:167;aSiO2¼ 0:5 106 K1, Taking the values Esio2 = 83 GPa,vsio2 = 0.167,asio2 =0.5 x10-6 K-1, andandaSi¼ 4 106 K1, the stress is calculated to be s¼0.31 GPa. Comparison with asi=4x 10-6K-1, the stress is calculated to be σ=-0.31 GPa. Comparison with TableTable3.5 shows that virtually all the stress is accounted for by differential thermal expansion


which places SiO2 into compression.


It should be noted that the tabulated stress levels are rather high. In fact, they typically range between 103 and 102 E, and this means that levels comparable to the yield range between 10-3 and 10-2 E,and this means that levels comparable to the yield stressstress


for these materials are reached. Therefore, instances of stress-induced plastic ﬂow and


damage in device structures should not come as a surprise.


3.3.2.4.2 Trench Dislocations


Among the suggested sources for DRAM trench dislocations are mechanical deformation and microcrack formation caused by particulate impact during processing, high implanted dopant levels, and silicide precipitates. In studying device isolation trenches, which have certain similarities to DRAM trenches,Hu [21] has proposed the following three sources for stress.


1. Compressive stress in thermal oxides grown on nonplanar surfaces such as trench corners. Thermal oxide linings are preferred vis-à-vis other dielectric ﬁlms because they have the lowest interface charge state and trap densities.


2. The mismatch in thermal expansion coefﬁcients between the trench dielectric (SiO2) and substrate Si.


3. Intrinsic stress in CVD deposited polysilicon and SiO2.


3.3.2.4.3 Hillock and Whisker Formation


In multilayer integrated devices as well as passive electronic components,the metal ﬁlm conductors employed sometimes develop troublesome surface protuberances known as “hillocks” and “whiskers.” The two probably originate from similar growth and relaxation mechanisms under the action of compressive stresses. They arise both during processing and stressing in service, and therefore adversely affect yield as well as reliability. Hillocks are much shorter, and may be viewed as stunted and more rounded whisker growths. Sometimes observed in thin ﬁlm aluminum interconnects and on contact pads, they are detrimental because their penetration of passivatingﬁlms can lead to electrical short circuits.


Whiskers are ﬁlamentary growths of pure metals, solid solution alloys, and compounds that have a high degree of crystalline perfection and uniformity.


Most whiskers are typically w1 mm thick, straight, parallel-sided single crystals with low index directions. Between straight segments, whiskers can bend sharply. Whiskers are threatening because they can grow to many times the ﬁlm thickness (Figure 3.16(a)) and short relatively remote conductors(Figure 3.16(b)). In addition to vapor deposition processes that leave deposits in compression, electrodeposited tin, cadmium, and indium surfaces commonly exhibit whiskers. Therefore, bright Sn deposits on brass should be avoided, and Ni-rather than Cd-plated screw fasteners are preferred. A rule of thumb by Hitch [22] suggests that whiskers generally form at temperatures of


0.5 TM, where TM is the melting point of the metal.


Hillocks and whiskers have been observed to sprout during electromigration, a subject treated at length in Chapter 5. The SiO2 used to


Defects, Contaminants, and Yield 141


passivate interconnections serves to conformally constrain the powered conductors. Compressive stresses induced in the metal by electrotransport can be relieved through extrusion of hillocks or whiskers that sometimes crack and pierce the conﬁning, insulating dielectric overlayer [20]. Interestingly, compression reduction or creation of tensile stresses through current reversal during electromigration or thermal cycling sometimes causes the hillocks to shrink in size.


3.3.2.4.4 Wafer Bow


The convex or concave bowing of ﬁlm–substrate combinations as a result of internal stress has already been noted in Section 3.3.2. Bowing may result


Figure 3.16 (a) Scanning electron microscope image of whiskers in thin tin ﬁlms.


(Courtesy of P.H. Sun.) (b) Tin whisker shorting calacitors. (Courtesy DfR Solutions.)142 Reliability and Failure of Electronic Materials and Devices


in lithography mask registration, tolerance, and overlay errors because processed feature sizes at the wafer center differ from those at the wafer circumference. However, the use of vacuum chucks tends to eliminate wafer warpage problems. The celebrated Stoney formula (16), relates theﬁlm stress to the bow radius of curvature R and the thicknesses d of bothﬁlm (f) and substrate (s) as


sf ¼


Esd2s


6R1 nsdf:


(3.10)


Over the years a host of experimental techniques, including optical interference, X-ray diffraction, and beam deﬂection, have been employed to measure the stress in ﬁlms and coatings [20]. A recent nondestructive method employs a laser beam that is scanned across the ﬁlm/Si wafer combination. The radius of curvature, which may be hundreds to thousands of meters long, is determined by a (light) position-sensitive detector.


In this way, for example, the simple radially symmetric dishlike bowing can be easily distinguished from the potato-chip-like twisting distortion sometimes seen. We are usually only interested in ﬁlm stress because the relatively massive substrate is only stressed to low levels.


3.3.3 Step Coverage


3.3.3.1 Metallization Coverage


The terrain of ICs consists of an array of stepped regions due to the many stripes, trenches, and openings in dielectrics. These must be coated with a uniform thickness of metal for reliable interconnect and contact performance. But as Figure 3.17 suggests, uniform coverage of a step is sometimes difﬁcult to achieve [23]. For the case shown, wafers rotating in a planetary holder are metallized with aluminum evaporated from an electron beam source. A computer simulation of the deposited ﬁlm, based on line-of-sight impingement and shadowing effects, reveals thinning near the oxide edge and secondary crack formation. The actual metallization topography compares well with prediction. It is not difﬁcult to imagine that such a conductor might pass electrical test and inspection; however, a reliability problem looms if local heating at the constriction and metal transport due to electromigration are excessive.


Both the extent of thinning and crack depth are a function of the wafer surface orientation. In the case of a rectangular trench with steep walls such that the surface normal of the trench bottom is collinear with the Al source, metal will uniformly cover the bottom and thinly coat the


Defects, Contaminants, and Yield 143


side walls. However, for deep trenches and large wafer tilts, asymmetric and discontinuous metal side wall coverage may occur with open circuiting a potential danger. One way to minimize or even eliminate metallization cracking is to raise the temperature of the substrate. This fosters increased surface diffusion of metal and ﬁlling of crevices, which leads to better overall coverage.


Sputtering employing large area cathodes generally results in metallizations with improved step coverage [24]. The reasons are a combination of effects involving ion bombardment–induced defect production and enhanced diffusion, plus resputtering and redeposition of metal atoms on the surface.


Figure 3.17 Scanning electron micrograph and computer simulation of aluminum ﬁlm coverage of a 1-mm step. Thinning and secondary crack formation are evident. From Ref. [23].


3.3.3.2 Dielectric Film Coverage


Lack of conformal coverage is not only limited to metals but also occurs in the deposition of dielectric ﬁlms. Consider how the multilayer interconnect structure typical of Figure 2.32 is fabricated. At a given level, metal stripes are patterned on a ﬂat SiO2 substrate, and after etching, a gap is left with metal on either side. The gap and metal are now ﬁlled and covered with a plasmaenhanced CVD oxide grown from silane and nitrous oxide as shown in Figure 3.18. Filling is incomplete, however, because less oxide deposits on the vertical side walls than on horizontal surfaces. There is a considerable amount of cusping, giving it a “bread loaf” proﬁle (Figure 3.18(a)). As deposition continues, the oxide pinches, trapping a void, or “keyhole,”between the metal lines. This void might be opened during chemical–mechanical polishing (CMP) planarization (Figure 3.18(b)). If so, there is danger of creating a short when the void is ﬁlled during subsequent metal deposition (Figure 3.18(c)). Problems of dielectric ﬁlm coverage and gapﬁlling have occurred in several generations of DRAM chip fabrication and have become increasingly challenging as linewidths continue to shrink.


CMP and planarization of surfaces containing metals (vias) and dielectrics is critical in the realization of multilevel metallization structures on chips with device feature sizes less than 0.25 mm. Defects associated with the polishing process, e.g., differential polishing rates, embedded abrasives, residual surface particles, damage to oxide glasses, etc., are illustrated in Figure 3.19. The prohibitively small allowable (killer) defect sizes (less than 0.08 mm) and low defect densities (w0.15/cm2) that are projected mean that their elimination during processing, and their detection during electrical test and inspection, will present signiﬁcant challenges.


3.4 CONTAMINATION


3.4.1 Introduction


High on the list of defects in virtually every processing step entered in Table 3.4 is contamination. By this we usually mean foreign atoms, molecules, and particles that are chemically and physically different from the desired materials they inhabit. Contaminants can be gaseous, liquid, or solid in nature and can contaminate gaseous, liquid, and solid matrices. For example, gaseous matrices are contaminated by other gases, liquid droplets,and solid aerosol particles. Liquid matrices are contaminated by dissolved gas bubbles, droplets, and solid colloid particles, and solid matrices by


Defects, Contaminants, and Yield 145


## 3.4 Contamination


PECVD OXIDE


Petrus 0000943KV X40:0k  750mm


After oxide planarization


Al/Cu metal lines


(c)After metal deposition


Large metal-filled void


Figure 3.18 Mechanism for the development of intralevel shorts. (a) Scanning electron micrograph of peaked void trapped within the CVD dielectric that is deposited between neighboring metal lines. (b) Void peak is removed during oxide planarization by CMP. (c) Subsequent deposition of metal raises the danger of creating a short between metallization levels. (From Ref. [25].)


adsorbed gaseous and liquid surface ﬁlms as well as particulates. Furthermore, contaminants can be ionic or nonionic, organic, or inorganic.


Defects are manifested primarily in the form of particulate contaminants.


For example, particulates have been estimated to be responsible for 75% or more of the loss in yield of volume-manufactured VLSI chips [27]. In view of this, it is not surprising that billions(109) of dollars are spent annually by microelectronic chip manufacturers to combat contamination problems


[28]. A signiﬁcant proportion of current articles and advertising in trade magazines like Solid State Technology and Semiconductor International is devoted to contamination and defect detection or elimination issues. This reﬂects the magnitude and compelling nature of the problem. The sources of contamination in processing, the nature of particulate contaminants, and the steps and strategies adopted to eliminate or minimize their inﬂuence are all addressed in this section.


Contamination of electronic products stems from essentially four sources: people, clean rooms, equipment, and processes. The impact of these on chip yield will be our primary focus of attention. Exposure to the environment also contaminates electrical products and sometimes leads to reliability problems. Environmental contamination used to adversely affect chip yields, but its impact has declined over the years through the widespread use of clean rooms. Nevertheless, package processing, which is not always done in clean rooms, is more susceptible to atmospheric contamination. Gone are the days when workers contaminated wafers with the W-filled microscratchPlug coringResidual W stringers Recessed plugDishing


Figure 3.19 Scanning electron microscope images of critical metal and dielectric defects induced by CMP. Defect sites on the wafer are noted. From Ref. [26]. Courtesy of KLA-Tencor.


Defects, Contaminants, and Yield 147


CMP Defects


W Puddle


RipoutEmpty microscratchResidual slurrySurface particle


Ti/TiN


BPSG or PSG


cosmetics they wore, the dandruff they shed, or the salt they transported on their shoes during snowy mornings. Over the years the contaminant size has roughly reﬂected the ﬁnest features being processed. But the smaller the particle size, the more numerous and diverse are their sources. Concurrently, circuit shrinkage has signiﬁcantly reduced the size of contaminant particles that can be tolerated.


In the past, the distribution of contaminant sources was roughly evenly divided. Recent trends, however, show that people and clean rooms are less important contributors to contamination problems than equipment and processes. This has happened because of the improvement in clean room technology and the covering of operators in almost space suit like garb,before entry to the clean room. Nowadays, contamination sources are quite subtle. Examples include airborne molecules, process gases (containing O2,N2, H2O, etc., at w0.1–10 ppm levels), liquids (e.g., etching and cleaning solutions, even deionized water), as well as process chambers, tools, robots,and hardware (e.g., desorbed matter, wear particles). For example, in a variety of VLSI process tools involving vacuum hardware, baseline particle levels are constant to a ﬁrst approximation [29]. However, this is punctuated by short bursts where particle counts may rise severalfold above background as a result of opening or closing load locks or transferring wafers. No tool, chemical, or rinsing solution is above suspicion. With this realization we now consider some examples of process-generated contaminants and their roles in fostering damage and yield loss. In contrast,environmental sources of contamination, e.g., corrodents, and their effect on long-term reliability will be treated in Chapter 7.


3.4.2 Process-Induced Contamination


Many processes have proven to be culprits in generating contaminants ranging in size from the atomic to the particulate level. We shall also broaden our deﬁnition to include charging of surfaces as a type of“contamination,” in order to present the damage introduced during plasma etching.


It is instructive to view process contamination as a kind of “food chain,”illustrated in Figure 3.20, that ﬁrst involves generation and transport of particles, and then deposition on the wafer. Implementing control measures to eradicate either their generation or their transport means that particles will not deposit.


Several processes known to generate contamination are brieﬂy treated in turn.


### 3.4.2 Process-Induced Contamination


3.4.2.1 Chemical Vapor Deposition


It is believed that perhaps as much as 25% of all particle-induced yield loss is derived from low-pressure CVD (LPCVD) processing [31]. Among theﬁlms produced by LPCVD are silicon nitride, polysilicon, and SiO2 from tetraethyl orthosilicate. Thin-ﬁlm deposits naturally build up on the tubes of these hot-wall reactors during deposition. Film stress, along with the turbulence of loading wafers, causes shedding of these particulate deposits onto the wafer. Rubbing of quartzware in furnaces and oxidation andﬂaking of heaters are additional contamination sources.


Aside from impurities in the precursor gases, CVD processes can also generate particulates from the gas-phase environment. The basic gas-to-solidﬁlm reaction is designed to occur at wafer substrates. However, when the supersaturation of reactants is too high, nucleation of the solid productmay occur homogeneously in the gas phase. In the form of “snow,” the vapor-borne particulates settle on the substrate and are incorporated into the growingﬁlm. Generation of dislocations and stacking faults, regions of poor adhesion,and roughened ﬁlm topographies are some of the adverse effects produced.


3.4.2.2 Ion Implantation


Even the perceived “clean” process of ion implantation is not above contaminating wafers with particularly damaging elements such as Fe, Ni,


Figure 3.20 Contamination food chain. From Ref. [30].


Defects, Contaminants, and Yield 149


Cr, and Mo. Because of them undesirable MOS threshold voltage drift,defects, junction depth shifts, and reduced carrier lifetimes result [32].


Speciﬁc problems arise from the following sources:


1. Ion-beam-sputtered atoms from photoresist masks, accelerator apertures, vacuum hardware, wafer ﬁxtures, etc., are incorporated in the beam and implant.


2. Chemically different ion species may have the same mass (m) to charge


(q) ratio. The selection of a particular ion for implantation is done with magnets and depends on m/q. If, for example, 11B19F2þ dopant and


98Mo2þ ion contaminants are simultaneously present, both B and Mo would be implanted into the wafer because m/q¼ 49 for both species.


3. Due to charge exchange processes in the beam, ions can either acquire or lose charge; this results in deeper or shallower implant depths, respectively, because the energy of an ion in the beam depends on its valence.


4. Cross-contamination is common when implanters are called on to provide high ﬂuences or ﬂuxes for several different dopants. Thus, faster diffusing boron and phosphorous dopants that contaminate arsenic and antimony implants displace junction depths. For example, a


0.01% contaminant level can cause a junction depth shift of 5%.


3.4.2.3 Plasma Processing


During various ﬁlm deposition and etching processes, devices are often directly exposed to an radio frequency(rf) plasma discharge ambience of reactive ions, which are further accelerated by the wafer self-bias voltage.


Enhanced and guided by the metallization or polysilicon patterns that act as“antennas,” the result of these ion collisions is charging of the surface.


Particularly large antenna surface areas may ultimately cause sufﬁcient charge injection to degrade dielectric properties.


Damage to materials during plasma etching has been classiﬁed into two broad categories [33,34]:


1. Particle current-ﬂow-induced damage. The buildup of charge produced by the plasma and the current driven by electric and magnetic ﬁelds are sources of this damage. Current ﬂow through the dielectric produces wear-out damage due to bond breaking and charge trapping.


2. Plasma exposure damage. This category of damage is a side effect of particle or photon impingement on the surface. Residue layers, impurity permeation of the surface, and ﬁlm adhesion damage due to photons or chemical attack are all examples of damage due to plasma exposure.


Particularly sensitive to plasma damage are gate oxides that have been shown to charge up, exhibit altered C–V curves (Section 2.5.2), and suffer earlier breakdowns as a result. Fortunately, plasma damage effects often occur during overetching and not during the main etching [35]. The subject of plasma damage to gate oxides is treated again in Section 6.3.8.


3.4.2.4 Lithography


Just one glance at the defective mask in Figure 3.21 reveals how patterned features on an IC chip can be severely damaged through incorporation of the indicated imperfections. Particulate contamination in the lithographic process is a chief contributor to such mask defects [36]. Lithography defects of differing severity have been classiﬁed and include killers, unreliable,hard, soft, and repairable [37]. Examples of these lethal defects are conductor opens and shorts through insulators between neighboring conductors. Unreliable defects do not cause immediate failures but may


Figure 3.21 Types of defects commonly encountered in resist processing. 1,Contamination; 2, opaque spot; 3, large hole; 4, pinhole; 5, excess material; 6, lack of adhesion; 7, mouse nips (intrusion); 8, scratch. From Ref. [36].


Defects, Contaminants, and Yield 151


lead to long-term reliability problems. Pinholes and mouse bites that remove a small fraction of a patterned line are examples. Other unreliable defects include image density variations, leftover chemicals or photoresist,and out-of-focus images. Hard defects are composed of excess or missing mask metal ﬁlm, e.g., chromium, while soft defects consist of particulate contaminants, clean room residues, and transparent material. Dust and watermarks that can be removed through cleaning the mask plate are examples of soft defect sources.


Lithography masks usually consist of patterned chromium ﬁlms on glass plates, and these materials as well as photoresists are among potential sources of defects [38]. For example, the glass may contain bubbles, scratches, pits,and surface microcracks. Pits prevent Cr adhesion, resulting in pinholes,while scratches cause nonuniform etching at pattern edges. The chromeﬁlm defects include pinholes and voids, particulate inclusions, and invisible chemical anomalies. Chromium oxides, nitrides, and carbides are examples of the latter, and collectively they cause erratic local etching and undesired patterns.


Photoresists and the assorted chemical solutions used in lithography are also sources of contamination. They undergo extensive ﬁltration to minimize the presence of particle and metal (e.g., Na, K) contamination.


3.4.2.5 Metal Contamination


Since the early days of Si device technology metallic contaminants have limited yield and have been a reliability risk as well. In this regard,Kolbesen [16] has estimated that the iron present in a pinhead, if spread uniformly across the entire annual production of the world’s leading wafer manufacturer, would contaminate the wafers with a lethal dose of 1013 Fe atoms per cm3. The gate oxide is particularly vulnerable to Fe,which lowers the dielectric breakdown voltage. In reducing the oxide thickness from 20 nm to 10 nm, corresponding to a translation from 1 to


0.5 mm linewidth technology, the Fe concentration had to be lowered from 1013 Fe atoms per cm3 to 1011 Fe atoms per cm3, or a factor of 100


[39]. The sources of metal contamination in production lines have been traced to virtually all tools, including furnaces and epitaxial reactors, ion implanters, plasma and reactive ion etching equipment, wet cleaning and etching chemicals, and wafer handlers and equipment. A combination of harmful properties listed below causes metals to play a detrimental role in devices.


1. Transition metals such as Cu, Ni, Fe, and Cr are fast diffusers in Si.


All have diffusivities exceeding 106 cm2/s at temperatures of 1000 C. In particular, Cu, which is currently used in metallizations,has a D value exceeding 106 cm2/s even at 500 C, and an activation energy of less than 1 eV. This compares with D values ofw1013 cm2/s at 1000 C, and activation energies of 3–4 eV for the common silicon dopants, i.e., B, P, and As.


2. Metals have low solubility in Si (in the part per million and below range) with a steep temperature dependence. Trace impurities may dissolve in wafers at elevated processing temperatures but be supersaturated when cooled to room temperature. Their rejection from solution leads to precipitation of silicides, e.g., FeSi2 and NiSi2, at lattice defect nucleation sites.


3. Many transition metals are effective minority carrier recombination and generation centers because they form levels within the Si band gap.


In addition, these metals react with acceptor impurities.


4. Metal precipitates serve as nuclei for the generation of extended defects such as dislocations and OSFs in the Si substrate and gate oxide.


5. Metal decoration of existing defects makes them far more conducting.


Dislocations and stacking faults so affected have caused excessive leakage currents in p–n junctions and retention time failures in DRAMs.


A chronic metal contaminant of interest in microelectronics is sodium.


In the ionic form it inhabits the various oxides and glasses of the IC chip.


Sodium is now largely eliminated from gate oxides, where it causes threshold voltage instabilities in MOSFET operation at surface densities above 1 1010/cm2. Presently, Na concentrations ranging from 1017 to1019 atoms/cm3 are found above the metallization levels, and are primarily introduced via photoresists [40].


3.4.3 Introduction to Particle Science


To develop strategies for reducing particulate contamination levels in microelectronics, it is important to understand the nature of particles, the way they are transported, and their mechanisms of adhesion to surfaces and wafers in particular [41]. The most important attribute of a particle is its size,because properties such as particle velocity, adhesion force, and ability to scatter light depend on it. There are vast differences in the behavior of large-scale objects compared to the submicron-sized particles that are our present concern. For example, the latter will adhere quite strongly to the


Defects, Contaminants, and Yield 153


ceiling of a chamber, but a 1-mm particle will immediately drop because gravitational forces far exceed the very weak adhesion forces. In microelectronic processing, drag, gravitational, and diffusional forces spread contamination by driving particles to wafer surfaces where various forces of adhesion (e.g., van der Waals (vdW), electrostatic, capillary) cause them to stick. Overcoming the inﬂuence of particle adhesion forces is a way to combat contamination. For these reasons, each of the forces will be brieﬂy discussed in turn.


3.4.3.1 Drag


As particles move through a ﬂuid (gas or liquid) they are opposed by frictional drag forces. For a small spherical particle of diameter d, moving slowly with velocity v, the drag force is given by Stokes’ law, or


Fd ¼ 3phd v=Cc:


(3.11)


Here h is the coefﬁcient of viscosity, and Cc is the Cunningham slip correction factor. For air at 1 atm and 20 C, Cc¼ 1 þ 0.16/d, with d givenin micrometer units. Thus, for particles smaller than 0.5 mm, Cc becomes signiﬁcant. Equation (3.11) is well satisﬁed when the Reynolds number for gas ﬂow, deﬁned by d vrf/h (rff¼ ﬂuid density), is less than 1; this is generallya good assumption for microelectronic processing.


3.4.3.2 Gravity


Of all the forces that act on aerosol particles, gravity is especially important because it acts all the time. The gravitational force is given by


Fg ¼ pd36rp  rfg;


(3.12)


where rp is the particle density and g is the gravitational constant. By equating Fd and Fg, the terminal velocity with which particles fall by gravity is given by


v ¼ d2rp  rfCcg18h:


(3.13)


Gravity always enhances the rate of particle impingement on the surface of a wafer. The deposition ﬂux, which is the product of the particle concentration and velocity, will be small if v is small. Importantly, particle impingement rates fall off as the square of the particle size.


3.4.3.3 Diffusion


The constant buffeting and bombardment by ﬂuid molecules causes small particles to execute Brownian diffusive motion. Such random motion becomes important when the particle is less than 1 mm in size. Diffusion distances are given by the familiar formula, x2¼ 4Dt, (see Eqn (5.6)), whereD is the diffusion coefﬁcient and t is the time. Theory shows that D is given by D¼Cc kT/(3phd), where kT has the usual meaning. Clearly, smallerparticles are expected to travel further. We are often concerned with the rate of particle impingement on wafers as a result of diffusion through the surrounding gas phase. Because small particles readily adhere to surfaces,their concentration (C) is lower there than in the bulk gas. This gradient(dC/dx) establishes a diffusive ﬂux ( J ) of particles toward the surface given by D dC/dx. Assuming that the wafer is immersed in an ambience where the particle concentration is Co, the rate of particle impingement (number per unit area per unit time) due to diffusion is given by


J ¼ CoDpt1=2


(3.14)


a result that can be obtained from Eqn (5.4) by differentiating. The number of particles N(t) that accumulate in time is simply the integral of this, or NðtÞ ¼ CoZ


Dpz1=2dz ¼ 2CoDtp1=2; (3.15)


where Co is the particle concentration far from the surface. A comparison of the particle densities that settle on a surface by diffusion relative to gravity is shown in Figure 3.22. Gravitational settling dominates for large particle diameters, whereas diffusional impingement controls when the particle size is small. It is important to note that Brownian motion distances are the same order of magnitude as the thin boundary layer thickness of gas ﬂowing by surfaces. Thus diffusion enables particles to penetrate this stagnant layer,reach the surface, and collect there. The expected particle ﬂux is also indicated in Figure 3.22. Due to the low concentration of large particles, there is a decline in impingement ﬂux at these particle sizes.


3.4.3.4 Electrostatic Forces


Initially uncharged particles often acquire charge through interaction with ionic species and gas molecules that become charged by ionizing radiation.


Defects, Contaminants, and Yield 155


The probability (Pe) that n electronic charges (both positive and negative)are associated with particles is governed by their size (d ) according to a Maxwell-Boltzmann-type expression


P ¼ constðdkT Þ1=2expn2q2dkT:


(3.16)


Thus, very small particles will be uncharged. For particles larger than


0.1 mm, the average n increases with d as n¼ 2.37 (dmm)1/2 [42].Charged particles will interact with one another according to Coulomb’s law.


3.4.3.5 Particle Adhesion


Particles adhere to surfaces through vdW, electrostatic, and capillary forces as well as chemical (hydrophobic/hydrophilic) interactions. Soluble contaminants are effectively removed by chemical solutions that have little inﬂuence on insoluble particles. In what follows, we focus on the latter particles and the nature of the physical forces that bind them to and remove them from surfaces. For the case of spherical particles of diameter d, a


Figure 3.22 Number of particles collected per square centimeter of horizontal surface by diffusion (solid line) and gravity (dashed line), as a function of particle size.


Particle density¼ 1 g/cm3, particle concentration¼ 1/cm3, temperature¼ 20 C. FromRef. [41].


distance z away from a planar surface (Figure 3.23(a)), the vdW adhesion force is given by


FadðvdW Þ ¼ AHd12z2;


(3.17)


where AH is known as the Hamaker constant. The latter depends on the particle and surface compositions, their hardnesses, and the shape and topography of the interacting surfaces. For 1-mm glass microspheres on bare Si in air, AH¼ 14.5 1013 erg, while on SiO2, AH¼ 8.5 1013 erg. Thistranslates into vdW forces of z 1 mdyn; surface pressures of z 108 dyn/cm2 generated are large enough to deform both particle and surface.


Electrostatic forces of adhesion between particles and surfaces(Figure 3.22(b)) have Coulombic and contact potential (CP) components.


The former is given by


FadðCÞ ¼ q24pεεo½d þ 2z2 ;


(3.18)


and the latter by


FadðCPÞ ¼pεodV2cp2z;


(3.19)


where 3is the dielectric constant of the intervening medium and 3o is the permittivity of free space. Vcp is the CP between the particle and surface, a quantity that typically ranges between 0 and 0.5 V. The charge transfer equilibrates the Fermi energies between the two bodies, establishing a capacitor-like double layer at the interface. Generally for small particles,adhesion forces due to CP exceed those due to electrostatic attraction.


For a 1-mm particle, with z¼ 4 108 cm and Vcp¼ 0.5 V, Fad


Figure 3.23 Types of adhesion forces between particles and surfaces. (a) vdW; (b)electrostatic; (c) capillary.


Defects, Contaminants, and Yield 157


(cp) z 1 mdyn. This force is roughly comparable to that for vdW interactions.


In humid environments adhesion between particles and the surface is promoted by the intervening water ﬁlm that develops between them because of capillary attraction (Figure 3.23(c)). A capillary force (Fc) of amount


Fc ¼ 2pdg


(3.20)can be expected, where g is the surface tension of water (72 dyn/cm). For a 1-mm particle, Fc¼ 4.5 102 dyn, a force that is larger than othersconsidered above.


3.4.3.6 Cleaning


Particle removal from wafer surfaces means establishing external forces that exceed the forces of adhesion. These external forces can be divided into three categories [42]: vibratory or mechanical action, hydrodynamic or aerodynamic drag, and wet or dry chemical action. Speciﬁc wafer cleaning techniques include scrubbing, high-pressure gas or liquid jets, wet chemical methods, and ultrasonic, ultraviolet, or ozone cleans.


3.4.3.6.1 Scrubbing


In this mechanical technique a brush rotates across the surface, removing inorganic particles and organic ﬁlms. Like a car hydroplaning on a wet highway, the hydrophilic (water-attracting) brush bristles are separated from the wafer surface by the thin layer of scrubbing solution. Scrubbing effectively removes large particles (>1 mm) from hydrophobic (water repelling) wafer surfaces. But scrubbing is unsuitable for submicron particle removal, especially from patterned wafers, and may even cause damage.


3.4.3.6.2 Pressurized Fluid Jets


This method of cleaning will remove small particles from patterned wafers.


As the ﬂuid moves past particles with velocity v, it drags them with a force given by Eqn (3.11). Higher velocities and viscosity coefﬁcients are more effective in cleaning. As a consequence, the drag force is considerably higher with ﬂuid than with gas jets. Troublesome static charge buildup on wafers and the possibility of mechanical damage are disadvantages.


3.4.3.6.3 Ultrasonics


High-intensity ultrasound waves at frequencies above 20 kHz are employed in this technique. They produce mechanical pressure ﬂuctuations that result


in the formation of cavitation bubbles. During the pressure cycle, the bubbles alternately expand and collapse. At the collapsing bubble interface, sufﬁcient energy is released locally at particles to overcome the force of adhesion and loosen them. While small particles are efﬁciently removed, it is difﬁcult to control cavitation without causing possible wafer damage.


3.4.3.6.4 Wet Chemical Cleaning


This widely used wafer decontamination method effectively removes metal ions and soluble impurities, but is not good for particle removal. Because assorted acids and bases are used, rinsing and drying steps are required.


In addition, particulate contamination is often present in chemical solutions.


3.4.3.6.5 Ultraviolet or Ozone


Dry processing and contactless removal of organic contamination are advantages of this cleaning technique. However, this method is not proven for particle removal.


3.4.4 Combating Contamination


3.4.4.1 Particle Detection


The ﬁrst step in developing a plan for contamination control is to be able to conﬁdently detect and analyze particle size and chemistry of samples. For this purpose instruments have been developed to measure particles in gases and liquids as well as on solid surfaces (wafers). Instrument capabilities include sensitivity (e.g., how small a particle can be detected), selectivity(e.g., ability to not mistakenly respond to something other than what is sought), rate of sampling and dynamic range, or the ratio of the highest to lowest level (e.g., particle size, concentration). Needless to say, high sensitivity, selectivity, rate of sampling, and dynamic range are essential.


In general, optical scattering techniques are employed for particle size and distribution measurements. Larger particles and those of higher refractive index than the surrounding media tend to scatter more light than smaller and lower refractive index particles (however, this is not always true). Rayleigh (dipole) scattering dominates when the particles are much smaller than the wavelength of light used, and yields a signal proportional to the square of the particle volume. Geometrical optics prevails when the particles are much larger than the wavelength, and scattering then occurs by reﬂection and refraction. Between these size range extremes there is Mie scattering. Particle sizes of less than 100 nm can be detected by available instruments, which typically employ computerized image analysis or


Defects, Contaminants, and Yield 159


holography techniques. This equipment and questions of what to sample for, where to sample, how many samples to take, how to interpret a count of zero, and how to analyze data are discussed by Cooper [28].


3.4.4.2 Clean Rooms


The use of clean rooms has traditionally been the chief strategy in combating contamination and particle-induced defects. Monitoring particulate contamination and controlling processing variables, through feedback and feedforward of defect information, help establish high yields for process steps carried out in the clean room. Air whose temperature and humidity is tightly controlled enters clean rooms through efﬁcient particulate air ﬁlters and then is made to ﬂow as laminarly as possible. This minimizes the sideways dispersion of contaminants generated in the room.


The class of a clean room is determined by how many particles of a given size are contained in a volume of its air. For example, a class 100 clean room contains 100 (or 3500) particles 0.5 mm or larger in size, per cubic foot (or cubic meter) of air volume. People in ofﬁces work in a class 100,000 clean room. Wafers in an ofﬁce room would have 1000 times more particles impacting them than those placed in a class 100 clean room. Particle size distribution curves for various classes of clean rooms are depicted in Figure 3.24(a). Because the number of particles increases the smaller they are, more stringent clean room requirements are demanded as minimum IC features shrink. In general, class 10 clean rooms are sufﬁcient for IC processing (oxidation, implantation), but lithographic steps require a more particle-free environment, e.g., a class 1 clean room. Evidence of the need for space-suit-type protection can be seen in the garb worn at Intel(Figure 3.24(b)). As the need develops, the measures taken will be even more elaborate. As an aside it is also important to note that according to Intel the class 1 clean room is 10,000 times cleaner than the cleanest operating room [43]. We also note that the water used in IC fabrication is the cleanest on the planet, because even the tiniest microbe will cause a massive defect in an IC.


3.4.4.3 Integrated Processing


A considerable advancement beyond clean rooms is integrated processing


[44]. In this new manufacturing approach, sequences of two or more chemical or physical IC processing steps are carried out while wafers are maintained in the clean or controlled ambience of cluster tools. For processes carried out at low temperatures, e.g., plasma etching, evaporation,


sputtering, and LPCVD, integrated processing is structured around a vacuum system. At the center of the cluster tool is a central wafer handler capable of delivering the wafer to any one of a number of surrounding chambers or process modules (Figure 3.25). In addition, vacuum load locks permit exchange of wafers between any of the cluster tool modules and


Figure 3.24 (a) Particle size distribution curves for various classes of clean rooms.


(From Ref. [5].) (b) Spacesuit-like garb worn in clean room. (Courtesy of Intel.)


Defects, Contaminants, and Yield 161


(a)10,000


CLASS 1,000 MID-1970's


1,000


CLASS 100 MID-1980's


a CLASS 10 EARLY 1990's


CLASS 1 MID-1990's


0.2


(b)working in a cleanroom Suit made of ultra clean material


includes Helmet air filter


Battery pack for air filter system


Will also wear


2 pairs of gloves


nyion & latex


glasses


2 pieces of foot gear


Belt


disposible shoe covers &outer booties


& safety hairnet


unit


PARTICLE SIZE (um)


PARTICLES/CU SIZE) FT (STATED


external clean rooms where lithography is practiced. Similarly, other controlled minienvironments, e.g., with vacuum, oxygen-free, inert, or controlled gas ambience, enable cleaning, CVD deposition of dielectricﬁlms, reactive ion etching, rapid thermal annealing, and oxidation to be carried out. The greatly enhanced cleanliness results in lower contamination levels of particulates and reactive impurities. In effect, processing in cluster tools occurs in a class 0.1 clean room.


3.5 YIELD


3.5.1 Deﬁnitions and Scope


Yield is generally deﬁned as the ratio of the number of good products produced to the total number of units started in any manufacturing operation [45]. The denominator of this ratio is the sum of the good products and those that had the potential of being good but for some reason were rejected. It should be clear that yield affects the cost of semiconductor products and our ability to predict their price in advance. Yield and cost are the crucial issues that determine the economic success or failure of semiconductor processing and manufacturing industries. The expected inverse


Figure 3.25 Schematic of an integrated vacuum processing or cluster tool. From Ref. [44].


## 3.5 Yield


correlation between yield and processing defects is depicted in Figure 3.26.


Despite wide swings in the monthly tracking of product yield, the trend is inexorably upward as learning occurs. It has been suggested that there are links between defects and reliability as well. Thus logic would dictate that yield and reliability are related despite the fact that the latter presumably refers solely to the performance of good, or yielded, products.


Product yields are generally less than 100% for the following reasons;


1. Circuit design problems. This may simply be due to errors in circuit design. The celebrated discovery in 1994 of omitted circuits within the 3 million transistor Pentium microprocessor chip is an example.


Although the manufacturing yield of this chip was certainly satisfactory initially, the subsequent recall and substitution had the same economic impact as drastically reduced yield. Other problems arise from alteration of circuit parameters beyond acceptable limits due to processing difﬁculties, which are then not accommodated in the design. New device behavior or circuit characteristics, unforeseen by the designer, sometimes surface to the detriment of yield. Some circuits are relatively tolerant to variations in circuit parameters, while others are very sensitive. In such cases an interactive effort between the designer (who identiﬁes sensitive parameters) and process engineer (who optimizes the value and range of these parameters) is required for redesign and tuning of one or more process steps. Circuit design problems are well beyond the scope of this book and will not be discussed further.


7 100


90


吕


80 70 YIELD (percent)40吕召


Y6LD


台古吕吕古


DEFECT DENSITY


10吕


DEFECT DENSITY PER LEVEL/sq.cm.


1986


1987


DATE


Figure 3.26 Defect density and yield variations produced when monitoring the impact of yield enhancement actions in a 1.25-mm process. From Ref. [46].


Defects, Contaminants, and Yield 163


2. Processing defects. Processing is frequently accompanied by inadvertent changes in the dimensions and composition of device features and components that adversely affect yield. Examples of such processing defects and their implications were discussed at length throughout this chapter.


3. Random point defects. Even though processing parameters are well within design speciﬁcations, the yield may still be below 100%. The reason is usually attributed to point defects or particles of macroscopic dimensions that settle on the water or obstruct the proper execution of a given processing step. Dust particles on a lithography mask is an example of the latter. These and other random defects can be killers.


Often, however, a less-than-killer defect survives screening and becomes the nucleus for eventual failure in service.


For any series of IC manufacturing steps, the overall, or cumulative, yield(Y) is the product of the wafer process yield (Yw), the wafer test yield (Yt), and the module test yield (Ym), such that


Y ¼ ðYwÞ  ðYtÞ  ðYmÞ:


(3.21)


Rejects occur at each stage where yield is evaluated, i.e., during individual processing steps including epitaxy, oxidation, metallization, metal removal, electrical testing of scribed and diced fabricated chips, and ﬁnal testing of packaged and assembled modules. Therefore, Yw, Yt, and Ym are each similarly deﬁned by the above generic yield deﬁnition. Because of the many hurdles that must be surmounted during these rigorous evaluation procedures it is remarkable that the quality and reliability of semiconductor electronics is excellent. However, there is always room for improvement,and this section is dedicated to that end.


3.5.2 Statistical Basis for Yield


A functional deﬁnition of yield is the probability of producing chips having no fatal defects that would cause immediate rejection. Yield prediction,therefore, requires calculating the probability of ﬁnding a particular state(a chip with no defects) out of all possible states (chips with zero, one, two,or more defects) when the events or defects are statistically distributed over all states according to some distribution function [47].


It is instructive to start by introducing the statistics of the binomial distribution, which can be physically described by the tossing of coins that have two outcomesdheads or tails. This subject is discussed in virtually every text on statistics and probability. If the probability of getting a head in


one trial toss is p and the probability of getting a tail is q, then it is evident that p þ q¼ 1 (in an unbiased coin p ¼ q ¼ 12). The same holds for N tosses,where the probability of obtaining at least one head or at least one tail is unity, or (p þ q)N¼ 1. Expansion yields


ðpþ qÞN ¼X


k¼1


N !


k!ðN  kÞ! p*(1-p)N-k,k!(N-k)!pkð1 pÞNk;


(3.22)


an equation known as the binomial distribution. Extending the result to N coins each ﬂipped once or one coin ﬂipped N times, the probability (P) that n heads will be obtained in N tosses is


Pðn;N ; pÞ ¼ N !n!ðN  nÞ! n!(N-n)!pnð1 pÞNnp"(1 -p)N-n.:


(3.23)


In a simple example, consider three coins that are tossed once. What is the probability of getting exactly two heads? There are eight possible outcomes (hhh), (hht), (hth), (htt), (ttt), (tth), (tht), and (thh), and of these,three have two heads. Thus the probability we seek is 38. This answer also results from direct substitution of N¼ 3, n¼ 2, p ¼ 12, in which caseP ¼ 3!=ð2!1!Þ  ð12Þ2ð12Þ1 ¼ 38P = 3!/(2!1!)x(2)2(2)1=/3.With no loss in generality let us consider Eqn (3.23) under conditions where N is large, i.e., N>> 1, N>> n, and p is small; but the product Np¼ a is of moderate size. Next, the following quotient of factorials andpolynomials is expanded,


ðN  nÞ! ¼ NðN  1ÞðN  2Þ.ðN  ½n (N-n)!=N(N-1)(N-2)...(N-[n-1])1Þ


¼ Nn1 1N1 2N/1n 1N=N*(1-A)(1-A)-(1-[])zNn:


ð1 pÞNn ¼ expfðN  nÞlnð1 (1-p)N-"=exp{(N-n)ln(1-p)}pÞg


¼ =exp{-(N-m)(p+2+2z+.)}exp ðN  nÞpþ 12p2 þ 13p3 þ.


¼ expNp1þ 11,2pþ 13p2 þ.=exp{-Np(1+12p+1/p+.-)}


¼ = exp[ - Np] or exp[ - a].exp½ Np or exp½  a:


Defects, Contaminants, and Yield 165


Upon substitution in Eqn (3.23),


Pn;N ; p¼ nn!exp½  :


(3.24)


This result is the Poisson approximation to the binomial distribution.


What does all of this have to do with yield? Suppose now that a number of events (defects) occur randomly in adjacent, nonoverlapping domains,and that these events are independent of events in other areas. The probability of a chip containing n defects is then given by Eqn (3.24). Thus the probability of a chip containing zero defects, a quantity previously deﬁned as the yield, is given by


Pð0;NpÞ ¼ Pð0;aÞ ¼ Y ¼ exp½  a:


(3.25)


Furthermore, suppose the domain is the chip of area A, and a is the average number of events or fatal defects per chip. If the defect density or number of defects per unit area is D, then a¼DA, and


Y ¼ exp½ DA:


(3.26)


This important equation expresses theprobability of a chiphavingnodefects provided that the defect density is constant. The strong exponential decrease in yield with increase in A and D should be appreciated. As a consequence of enlarging the die area from 1 to 1.5 cm2 the yield will drop by a factor equal to exp [ (1.51.0)D], assuming the same D; for example, the respective factorsare 0.78 and 0.61 when D¼ 0.5 and 1 defect/cm2. Imperatives to lower Dwhen increasing the wafer size are thus evident. The fundamental relationship expressed in Eqn (3.26) is the basis for yield modeling, a subject treated next.


3.5.3 Yield Modeling


Instead of being constant, assume now that the defect density varies according to the function f(D). Then the probability that a chip will have n defects is given by the Poisson equation, i.e.,


Pðn;DAÞ ¼Z


f ðDÞðDAÞnn!exp½DAdD:


(3.27)


When n¼ 0 the yield is calculated as Y ¼Z


f ðDÞexp½DAdD:


(3.28)


This integral, proposed by Murphy [48], plays an important role in yield modeling. Depending on the form of the function f(D), different yields are obtained when evaluating the integral. Among the many defect density functions suggested over the years, the following have been found useful:


1. Constant D. In the case where D is a constant (i.e., Do), we require that f(D)¼ 0 everywhere except for D¼Do. Mathematically, f(D)¼d(DDo), and f behaves like a delta function (d). Substitution intoEqn (3.28) and integration yields our expected formula


Y ¼ exp½ DoA:


(3.29)


2. Triangular. This approximation to a Gaussian distribution has the form f(D)¼D/Do2 for DoD 0, and f(D)¼ 1/Do (2D/Do) for2DoDDo. When D 2Do, f(D)¼ 0. Substitution into Eqn(3.28) and integration yields Y ¼ ð1 exp½ DoAÞ2ðDoAÞ2


(3.30)


3. Exponential. In this case f(D)¼ 1/Do exp [D/Do], and substitutioninto Eqn (3.28) yields Y ¼ ð1þDoAÞ1


(3.31)


after integration.


Graphic representations of these as well as Gaussian and gamma distribution functions of D are shown in Figure 3.27. The shape of these functions depends on the value of s, the standard deviation normalized with respect to Do. In the case of the gamma function, when s ¼ 1 wehave the simple exponential function. Plots of normalized yield behaviors for the three-parameter gamma distribution as a function of the defect density–area product are displayed in Figure 3.28. For values of s different from zero, yields are always greater than that given by Eqn (3.29).


The reader should not be lulled into thinking that just because mathematical equations for yield exist, f(D) can actually be predicted. In fact,quite the opposite is true. Presently, there is no way to determine f(D)directly. Instead, it is inferred from actual production yields by curve ﬁtting.


Once obtained, f(D) can be said not to be wrong if calculated yields derived from it match the production experience. Nevertheless, there is no reason to assume that f(D) derived for product A will apply to product B, or even to product A in another time frame and environment.


Defects, Contaminants, and Yield 167


3.5.4 Comparison with Experience


Yields generally improve over time as learning occurs. For new products the initial yield may be close to zero. But, by establishing yield targets,monitoring actual performance, prioritizing yield detractors, implementing action, and then iterating improvement cycles of successively shorter duration, yields rise slowly at ﬁrst and then more rapidly, until product yields level off at w90% or more. Simultaneously, defect densities are observed to fall in concert.


Figure 3.27 Graphic representations of distribution functions of D and corresponding expressions for yields. From Ref. [49].


Among other ﬁndings concerning yield are the following:


1. Yield generally declines in dies located at the outer periphery of wafers,as shown in Figure 3.29.


2. As the number of process steps for a given product increases, yield, not surprisingly, is expected to drop. A graphic illustration of how severe the manufacturing yield drop is when the total number of process steps reaches several hundred is depicted in Figure 3.30.


3. Yield projection using Eqn (3.29) is pessimistic because defects preferentially congregate at certain locations on the wafer or cluster, rather than distribute randomly. This tends to leave unexpected defect-free areas that raise yield.


Figure 3.28 Plots of three-parameter-yield model. A¼ chip area, D0¼mean defectdensity, and l¼ variance of D distribution. (Note: l¼ s2). From Ref. [49].


Defects, Contaminants, and Yield 169


3.5.5 Yield and ReliabilitydWhat Is the Link?


There is a quantitative link between yield and reliability that we now explore. A clear distinction was drawn between these separate subjects in Chapter 1. Yield issues fall within the province of the manufacturer;Radial Distance


Figure 3.29 Relative chip yield versus radial distance from center of silicon wafer. From Ref. [45].


No.steps n =


200 300


古


500


Cumulative yield (%)台


400 100


10 97


99


Process step yield (PSY) (%)


Figure 3.30 Cumulative manufacturing yield dependence on the process step yield.


Total manufacturing yield decreases rapidly with yield for each process step as the number of process steps gets large. From Ref. [44].


0731人


reliability, on the other hand, is of primary concern to the user and is measured from the time the product is put in service. Nevertheless, it is known that low-yielding product lots usually have lower reliability, as evidenced by higher failure rates during burn-in. The defects, which are the cause of yield loss, can also cause failure during burn in or early in product life(latent reliability defects), because these defects are so close to total failure that they can only survive for a short time, e.g. a 95% notch in a metal line fails due to electromigration during the ﬁrst few minutes of service. Correlations between yield and reliability have been recognized in practice [50,51] and developed theoretically [51,52]. In the latter regard a quantitative correlation between “reliability defects” and yield defects developed by Huston and Clarke [53] is instructive, and will be sketched here. While we all have a feeling for yield defects, reliability defects are those that do not cause immediate rejection or failure, but change their characteristics under use conditions. These latent defects cause either “near opens” or “near shorts,” and since they are neither completely electrically open nor shorted during the time of manufacture, they are difﬁcult to detect, monitor, or control. Photolithography defects in the aluminum interconnects of Figure 3.31 are examples of near opens. Similarly, defects in gate oxides and passivating insulators are near shorts. Other examples of


Figure 3.31 Photolithography defects in two parallel aluminum interconnects. From Ref. [53].


Defects, Contaminants, and Yield 171


either near-open or near-short defects may exist at contacts, steps, vias, or in polysilicon and between metallization layers.


In the yield modeling literature the concept of critical area (AY) arises as a mathematical quantity that describes the probability that a defect will result in yield loss, e.g., due to a complete open or short. Therefore, we may write


Y ¼ Yo exp½DAY ;


(3.32)


where Yo is the yield for nonrandom defects. In an analogous manner it is possible to deﬁne a reliability critical area (AR), so that the reliability function (R) would be


R ¼ Ro exp½DAR;


(3.33)where Ro is a constant. If the two critical areas are simply related by AR/AY¼K (a constant), and Yo and Ro¼ 1, then


R ¼ YK :


(3.34)


An experimental test was made of this relation by visually counting both kinds of defects in a collection of processed wafers. In Figure 3.32(a) the number of reliability defects is plotted versus yield defects, while the log–log plot of Figure 3.32(b) yields a value of K¼ 0.30.To determine AR, it is necessary to ﬁrst calculate AY. By deﬁnition, the average critical area is given by


AY ¼Z


PYðxÞDðxÞdx;


(3.35)


where, PY(x) is the probability that a defect of size x will cause a yield defect, and D(x) is the defect density function. A similar expression holds for reliability defects. Now consider a pattern of parallel metal stripes (w wide with a space s between them) as shown in Figure 3.33.


A yield defect, or complete open, occurs if the particle of dimension x falls on the pattern and completely covers a metal line. On the other hand, a reliability defect, or near open, occurs if the particle reduces the cross-sectional area of the stripe below some arbitrary value. In the case where reliability defects are assumed, when the cross-sectional


81.9%


Figure 3.32 (a) Number of reliability defects as a function of yield defects. Each point represents the number of observed defects for a single wafer. (b) Log–log plot of reliability yield versus yield. The slope yields a value of K¼ 0.30. (From Ref. [53].)


Figure 3.33 A defect modeled across a metal pattern. The effect of small, medium,and large defects is shown. From Ref. [53].


Defects, Contaminants, and Yield 173


(a)30


哿台 Defects


古 Number of Reliability07


.*


Number of Yield Defects


(b)100% 90.5% 81.9% 74.1%67.0%60.7%100%


人


!


g


」


p


86.1%


90.5%


95.1%


Yield


102030405060


area is reduced below w/4, it is not too hard to show [53,54] the following results:


Particle size (x)


PR(x)


PY(x)


0 x 3w/4


0 3w/4 xw (xw/2)/(w þ s) 0 w xw þ s


2w=ðw þ sÞ


(xw)/(w þ s)w þ s x 2w þ s ½w þ 12ðs xÞðw þ sÞ (xw)/(w þ s)2w þ s x 0 1


Next, a form for D(x) must be selected, and it is usually taken as D(x)w 1/x3, the experimentally observed form. Lastly, the integrals are evaluated through piecewise integration in the different size ranges. In this way both PY(x) and PR(x) can be evaluated and K determined.


3.5.6 Conclusion


A graphic way to conclude the chapter is to consider the representation depicted in Figure 3.34 connecting yield and reliability through a common concern, namely, defects. Until now, our chief interest has been with factors that characterize and inﬂuence yield. Starting with the next chapter,interest shifts to the right side of this diagram as we consider those factors that relate to reliability.


1. Values of the energy to form a vacancy (Ef) of about 1 eV have been measured in the noble metals Cu, Ag, and Au. In Si, Ef z 2.3 eV.


a. What is the equilibrium concentration of vacancies at 1000 K and


at 300 K?


Figure 3.34 A representation of the way yield and reliability concerns are interconnected through defects.


b. What is the vacancy concentration in Si at room temperature?c. Comment onwhether such concentrations pose reliability problems.


2. Oxygen concentrations are generally greater near the seed end of grown crystals than near the bottom. Why? What implication does this have for wafer yield?


3. Approximately what temperature is required to getter iron and copper atoms located 100 mm from extrinsically introduced dislocations if the treatment time is limited to 1 hour? The respective diffusion coefﬁcients are D(Fe)¼ 103 exp [(0.68 eV/kT)] cm2/s and D(Cu)¼4.7 103 exp [(0.43 eV/kT)] cm2/s.


4. The diffusion coefﬁcient of oxygen in Si is given by D¼ 0.17 exp[2.54 eV/kT] cm2/s. Suppose the O concentration in Si is initially7 1017/cm3. How long should deoxidation be carried out at 1100 Cto create a denuded zone containing an O concentration of 7 1016/cm3a distance 2 mm beneath the wafer surface? Assume that diffusion with an error-function-type solution governs deoxidation (see Chapter 5).


5. Differences in atomic radii (R) between silicon (RSi) and dopant atoms(RD) give rise to misﬁt stresses. In this case a measure of the misﬁt (f)has been suggested to be f¼ 1 (RD/RSi)3. Values for RD and solubil-ities (S) at 1200 C for antimony and boron are RSb¼ 0.136 nmand S(Sb)¼ 5.8 1019 cm3 and RB¼ 0.098 nm and S(B)¼5 1020 cm3, respectively. For silicon, RSi¼ 0.117 nm, and theatomic density is 5 1022 cm3.a. Compare this expression for f with that of f in Eqn (3.9).


b. Estimate the residual stresses in Si containing maximum dissolved


levels of antimony and boron.


6. An electric ﬁeld acts normal to the GB of an n-type silicon bicrystal.


Sketch the resulting band structure.


7. A ﬁlm/substrate couple is residually stressed. Sketch the stress and strain variation across the interface. Speciﬁcally, are the stresses and strains continuous or discontinuous in going from ﬁlm to substrate?


8. In the furnace processing of silicon wafers that are being cooled from elevated temperatures, radiation occurs more readily from the wafer periphery than from the center. As a result, a difference of 190 C has been measured between these sites when the wafer is at 1100 C.


a. What is the sign of the residual stresses expected at the edge relative


to the center of the wafer?


b. Estimate the magnitude of the thermal stress. Will dislocations form


if the critical yield strength of Si is 2 106 g/cm2?


Defects, Contaminants, and Yield 175


9. A critical thin ﬁlm in an electronic device is prepared by a process in


which two different thermal mechanisms compete. The ﬁrst mechanism has a high activation energy and yields few product defects, while


the second mechanism proceeds with low activation energy but generates many defects. Is it more desirable to operate the process at


high or low temperatures? Why?


10. In a wafer fabrication facility that produces ﬂash memory chips for


portable computers, silicon nitride is deposited at high temperatures


under low pressure, and chlorine as well as ammonia gas is liberated.


Silicone rubber O-ring gaskets used in the door of the vacuum furnace


reach a temperature of 218 C.


a. Comment on potential yield problems arising from the use of these gaskets.


b. What properties of gaskets would you recommend for this application?


11. Inmaking ﬂat-panel display screens for laptop computers it is determined


that defects measuring 0.5 mm in size can be tolerated if their density does


not exceed 0.0005 per cm2. A studymade in the semiconductor industry


revealed that a density of 5 defects per m2was achievable, for a defect size


of 0.1 mm. The environment in the semiconductor study contained


10,000 particles measuring 0.1 mm, per cu ft. What class clean room


would you recommend for themanufacture of ﬂat-panel display screens?


12. A clean room contains a concentration of 100, 0.5-mm particles in a


cubic foot of air


a. What is the class of the clean room?


b. Wafers are placed on a horizontal surface in this clean room. How long will it take before the surface (number) concentration of particles reaches 0.01/cm2?


c. Suppose the same wafers are stored vertically. How long will it take for the same surface concentration of particles to be reached? Make reasonable assumptions for particle properties.


13. Suppose we wish to calculate the number of chips on a wafer


a. For a 20-cm-diameter wafer with square chips that measure 8 mm on a side how many chips are there on the wafer?


b. For the same wafer containing rectangular chips that measure


10.67 mm 6 mm how many chips are there?


c. A formula to calculate the number (N) of wafers on a chip is given by N¼p(RA1/2)2 A1, where R is the effective wafer radiusand A is the chip area. Repeat parts a and b.


d. Another formula that distinguishes between chips with the same area but different aspect ratio (a) is N ¼ ðpR2=aE2Þexp½aE=R;where E is the chip edge length. (The chip area is aE2.) Recalculate N for parts a and b using this formula.


e. To see what accounts for the difference in these answers consult A.V. Ferris-Prabhu, IEEE Circuits and Devices, (January 1989),p. 37.


14. It is desired to double the area of a chip while keeping the processing


yield constant. By what factor must the defect density be changed to


accomplish this in the case of a. constant, b. triangular, and c. exponential defect distributions?


15. Consider the half-Gaussian defect density distribution given


byf ðDÞ ¼ ð2Do=pÞexp½1=pðD=DoÞ2. Through the use of Eqn(3.28) show that the yield is given by Y ¼ exp½pðDoAÞ2=4


f1 erf ðp1=2DoA=2Þg


16. In the chapter it was stated that


a. yield generally declines in dies located at the outer periphery of wafers, and


b. defects preferentially congregate or cluster at certain locations on the wafer rather than distribute randomly.


Provide possible explanations for these observations.


17. An IC process produces three defects per chip. Which of the yield


modelsdconstant, triangular, or exponentialdis the most optimistic


about yield?


18. Determine the number of fatal defects on a wafer containing laser chips


if the yield of good chips is 80%. There are 2000 chips measuring


0.1 mm 0.25 mm per wafer. Assume that the defects are randomlydistributed.


19. The defect trend in DRAMs is as follows:


Defects Number/cm2 Generation of DRAM


6


16 Kb


256 Kb


0.6


1 Mb


16 Mb


If the trend continues, what defect density will be tolerated in the 1-Gb DRAMs? Estimate the number of defects on a 20-cm-diameter wafer containing 1-Gb DRAMs if the chip dimensions measure 1.5 cm 1.5 cm.


Defects, Contaminants, and Yield 177


20. A multichip module consists of six chips. These are listed with their


yields in early production runs as well as later in mature products


Chip type


|Microprocessor |1 |55 |90 |
|---|---|---|---|

|ASIC |2 |50 |85 |

|Memory |3 |60 |99 |

Number Early yield Later yield


What are the overall early and long-term yields for these modules?


[1] S.D. Wolter, M.B. Ferrara, K.A. Welch, Solid State Technol. (October 1995) 85.


[2] L.C. Kimerling, J.R. Patel, in: N. Einspruch (Ed.), VLSI Science, Microstructure


Science, vol. 12, Academic Press, Boston, 1985.


[3] G.L. Miller, D.V. Lang, L.C. Kimerling, Ann. Rev. Mater. Sci. (1977).


[4] J.C.C. Tsai, in: S.M. Sze (Ed.), VLSI Technology, McGraw Hill, New York, 1988.


[5] S.M. Sze, Semiconductor Devices, Physics and Technology, J. Wiley and Sons, New


York, 1985. Copyright by Bell Telephone Laboratories, Inc.


[6] H. Tsuya, Semiconduct. Semimet., 42, Academic Press, 1994, 619.


[7] B.O. Kolbesen, H.P. Strunk, in: N. Einspruch (Ed.), VLSI Science, Microstructure


[8] J.W. Mayer, S.S. Lau, Electronic Materials Science: For Integrated Circuits in Si and


[9] H.F. Matare, Defect Electronics in Semiconductors, Wiley-Interscience, New York,


1971.


[10] J.C. Zolper, A.M. Barnett, IEEE Trans. Elec. Dev. 37 (1990) 478.


[11] S. Mahajan, Progr. Mater. Sci. 33 (1) (1989).


[12] S.-H. Soh, J. Lari, S. Hunt, T. Davies, M. Kuo, U. Kim, M. Cheung, E. Lucero, 33rd


Annual Proceedings of the IEEE Reliability Physics Symposium, p. 244, 1995.


[13] G.J. Declerck, in: R.A. Levy (Ed.), Microelectronic Materials and Processing, Kluwer


Academic Publ., Dordrecht, 1989.


[14] P. Schley, G. Kissinger, R. Barth, K.-E. Ehwald, Solid State Phenomena, 1993,


pp. 32–33, 353.


[15] C.H. Seager, Ann. Rev. Mater. Sci. 15 (1985) 271.


[16] P.M. Fahey, S.R. Mader, S.R. Stifﬂer, R.L. Mohler, J.D. Mis, J.A. Slinkman, IBM J.


Res. Develop. 36 (1992) 158.


[17] B.O. Kolbesen, in: S. Coffa, J.M. Poate (Eds.), Crucial Issues in Semiconductor


Materials and Processing Technologies, Kluwer, 1992.


[18] G.L. Schnable, in: A.H. Landsberg (Ed.), Microelectronics Manufacturing Diagnostics


Handbook, Van Nostrand Reinhold, New York, 1993.


[19] I. Blech, D. Dang, Solid State. Tech. 37 (8) (1994) 74.


[20] M. Ohring, The Materials Science of Thin Films, Academic Press, Boston, 1992.


[21] S.M. Hu, J. Appl. Phys. 70 (R53) (1991).


[22] T.T. Hitch, Circuit World 16 (2) (1990).


[23] I.A. Blech, D.B. Fraser, S.E. Hasko, J. Vac. Sci. Tech. 15 (1978) 13.


[24] W.D. Westwood, in: R. Levy (Ed.), Microelectronic Materials and Processes, Kluwer,


Dordrecht, 1989.


[25] D.R. Cote, S.V. Nguyen, W.J. Cote, S.L. Pennington, A.K. Stamper, D.V. Podlesnik,


IBM J. Res. Develop. 39 (1995) 437.


[26] Semiconductor International, November 1997, p. 55.


[27] T. Hattori, Solid State Tech. 33 (1990) 7. S-1.


[28] D.W. Cooper, in: A.H. Landsberg (Ed.), Microelectronics Manufacturing Diagnostics


[29] P. Borden, IEEE Trans. Semiconduc. Manuf. 3 (4) (1990) 189.


[30] T. Francis, Semiconductor International, October 1993, p. 62.


[31] P. Burggraaf, Semiconduc. Int. 18 (5) (1995) 69.


[32] F.A. Stevie, R.G. Wilson, D.S. Simons, M.I. Current, P.C. Zalm, J. Vac. Sci. Technol.


B 12 (4) (1994) 2263.


[33] S.J. Fonash, C.R. Viswanathan, Y.D. Chan, Solid State Tech. 37 (7) (1994) 99.


[34] H. Shin, C. Hu, IEEE Trans. Semiconduc. Manuf. 6 (1993) 96.


[35] Y. Uraoka, K. Eriguchi, T. Tamaki, K. Tsuji, IEEE Trans. Semiconduc. Manuf. 7


(1994) 293.


[36] L. F. Thompson and M. J. Bowden, in Introduction to microlithography, ed. L. F.


Thompson, C. G.Wilson, andM. J. Bowden, American Chemical Society,Washington,


DC (1983)


[37] S.N. Gupta, A.K. Bagchi, N.N. Kundu, Microelectron. J. 16 (1) (1985) 22.


[38] S. Wolf, R.N. Tauber, Silicon Processing for the VLSI Era, Lattice Press, Sunset Beach,


CA, 1986.


[39] W.B. Henley, L. Jastrebski, N.F. Haddad, 31st Annual Proceedings of the IEEE


Reliability Physics Symposium, p. 22, 1993.


[40] J. Chinn, Y.S. Ho, M. Chang, T. Turner, 32nd Annual Proceedings of the IEEE


Reliability Physics Symposium, p. 249, 1994.


[41] D. Leith, in: R.P. Donovan, M. Dekkar (Eds.), Particle Control for Semiconductor


Manufacturing, 1990. New York.


[42] V.B. Menon, in: R.P. Donovan, M. Dekkar (Eds.), Particle Control for Semiconductor Manufacturing, 1990. New York.


[43] See: Inside the Intel manufacturing process, what is a clean room?, Intel Web Site.


[44] G.W. Rublof, D.T. Bordonaro, IBM J. Res. Develop. 36 (1992) 233.


[45] P.J. Bonk, M.R. Gupta, R.A. Hamilton, A.V. Satya, in: A.W. Landzberg (Ed.),


Microelectronics Manufacturing Diagnostics Handbook, Van Nostrand Reinhold,


New York, 1993.


[46] J.M. Pimbley, M. Ghezzo, H.G. Parks, D.M. Brown (Eds.), VLSI Electronics


Microstructure Science, vol. 19, Academic Press, 1989.


[47] A.V. Ferris Prabhu, Introduction to Semiconductor Device Modeling, Artech House,


Boston, 1992.


[48] B.T. Murphy, Proc. IEEE 52 (1964) 1537.


[49] D. Koehler, W.E. Beadle, in: W.E. Beadle, J.C.C. Tsai, R.D. Plummer (Eds.), Quick


Reference Manual for Silicon Integrated Circuit Technology, Published by John Wiley


and Sons, 1985. Copyright Bell Laboratories.


[50] J.G. Prendergast, Proc. 31st Annual Proceedings of the IEEE Reliability Physics


Symposium, p. 87, 1993.


[51] F. Kuper, J. van der Pol, E. Ooms, T. Johnson, R. Wijburg, W. Koster, D. Johnston,


34th Annual IEEE International Reliability Physics Symposium, p. 17, 1996.


[52] C.G. Shirley, A Defect Model of Reliability, Tutorial Notes, IEEE International


Reliability Physics Symposium, p. 3.1, 1995.


[53] H.H. Huston, C.P. Clarke, 30th Annual Proceedings of the IEEE Reliability Physics


Symposium, p. 268, 1992.


[54] C.H. Stapper, IBM J. Res. Develop. 27 (1983) 549.


Defects, Contaminants, and Yield 179


CHAPTER 4


The Mathematics of Failure and Reliability


4.1 INTRODUCTION


This chapter focuses on the mathematical methods employed in analyzing product quality and failure data. These data are obtained through measurement, testing, and service experience with the objective of obtaining the most probable values of parameters that characterize quality control,failure rates, and projected lifetimes of components and devices. As we shall see, statistical analysis is part of all quality and yield assessments associated with the processing and manufacture of devices. In particular, the use of reliability mathematics and analysis in predicting the fate of products during service is a recurring theme of this book.


We may well ask what are the sources for the data we analyze. Assorted information on the quality of a product or component is invariably gathered during stages of its manufacture through testing and screening. Then ﬁnally,prior to shipment, products undergo ﬁnal inspection and qualiﬁcation. The purpose is to weed out obvious rejects as well as weak products that would probably fail early during service. Testing to uncover these rejects may, at a minimum, involve nondestructive inspection and measurement of electrical characteristics. For more robust products, the weeding process requires that they survive the ordeal of exposure to conditions harsher than those they will experience in actual use. Burn-in is such an example. Here a simple pass–fail(or go–no go) decision is made as a result of response to stressing at elevated temperatures, voltages, currents, etc. Information gathered from such screening ultimately relates to either process or product yield, and is used in the yield models presented previously. Because of its pass–fail nature, the data are essentially time independent and are normally handled by simpleGaussian or normal distribution function statistics. Burn-in tests, however, do have a time dependence that is usually recorded.


In order to predict the reliability or fate of products during service,more extensive time-dependent destructive testing will now be required to allow values of failure rates to be determined. These are extracted from


http://dx.doi.org/10.1016/B978-0-12-088574-9.00004-5


All rights reserved. 181


# 4 . The Mathematics of Failure and Reliability


## 4.1 Introduction


other mathematical functions, e.g., exponential, lognormal, and Weibull distributions that are used to ﬁt failure data. Failure times, which depend on the testing conditions, e.g., temperature, voltage, etc., will vary from sample to sample and lot to lot. When the product is inexpensive(e.g., a light bulb) and there are many, one has the luxury of testing numerous samples to failure, and good statistical information will generally emerge. However, if the product is costly (e.g., a laser) an extensive failure testing program may not be feasible. Normally, reliability testing consumes a considerable portion of the vendor’s research and development budget. When one considers the pharmaceutical industry, it is apparent that extensive reliability testing is not limited only to electronic products.


In addition to vendor-initiated product evaluation, there is the customer service experience to contend with. Depending on the nature of the product, ﬁeld failure data may be more problematic, statistically, because the data are less abundant and subject to an often uncontrolled operating or testing environment. Nevertheless, this information is extremely valuable because it provides a powerful incentive to the vendor to conduct a failure analysis study that may uncover an overlooked product defect. By merging all of this vendor/customer-generated reliability information, intelligent predictions of product lifetimes are possible.


It must be emphasized, however, that the puzzling causes and attributes of physical degradation and failure mechanisms are generally not illuminated through statistical analysis of lifetime data. Neither are any clues revealed with regard to minimizing or eliminating failure. Rather,statistical analysis of the kind addressed in this chapter in a sense quantiﬁes and institutionalizes our ignorance of the causes of failure. As pointed out by Pecht and Nash [1], reliability assessment based on root-cause analysis of failure mechanisms, damage sites, and dependence on operating stress has proven to be effective in the prevention, detection, and correction of failures associated with the design, manufacture, and operation of products.


Traditional reliability prediction methods based on statistical analysis and curve ﬁtting of failure data have also addressed these same issues of design,manufacture, and operation of products, but not as effectively. Nevertheless, virtually all failure test data reported in the literature are analyzed by the mathematics of statistics and associated probability theory. As we shall see, however, there is controversy involved in doing this and there are questions related to the credibility of the conclusions.


This chapter’s discussion of statistics and probability, failure distributions,reliability estimates, and conﬁdence of predictions is treated more extensively in Refs [2–5]. They are recommended for their lucid presentations.


4.2 STATISTICS AND DEFINITIONS


4.2.1 Normal Distribution Function


A useful skill for an engineer concerned with product reliability is to be able to convert a mass (mess?) of failure data into a form amenable to analysis without having a FIT (an acronym of “failure unit”). As an example,consider a company that makes electrical fuses for trucks that are rated at 10 A. Fuses fail by melting when current-induced Joule heat cannot be effectively removed. Because fuses protect other circuitry from electrical overload failure, it is vital that they function within the rated value, say between 9 and 11 A. Circuit damage or less-than optimum performance may be the outcome of operating outside these current extremes. Fuses are produced in lots of tens of thousands, and it is not practical to test them all and reject those that fail. To determine if fuses operate within speciﬁcations without excessive variability, a random sample from the population of 10,000 fuses is chosen and tested by increasing the current until they fail or open the circuit. The failure currents measured for such a population of 100 fuses are entered in Table 4.1. It is clear that although values cluster at about 10 A, there is a spread that warrants further statistical analysis [2].


To proceed, it is convenient to ﬁrst create a failure frequency distribution, as indicated in Table 4.2. For this purpose the range represented by minimum and maximum current values is arbitrarily subdivided into a number of cells (11 in this example) and the number of fuses destroyed in each current interval is noted. The results are best represented in the form


Table 4.1 Fuse test currents


|9.60 |9.76 |9.46 |10.42 |9.34 |10.20 |10.06 |10.36 |9.16 |9.54 |
|---|---|---|---|---|---|---|---|---|---|

|10.22 |10.41 |10.19 |9.61 |10.20 |9.76 |10.32 |10.04 |9.88 |10.02 |

|9.46 |9.72 |9.28 |10.02 |9.88 |10.11 |9.72 |10.24 |10.24 |10.85 |

|9.58 |9.76 |9.51 |9.68 |9.82 |8.86 |10.04 |9.88 |10.09 |10.06 |

|9.76 |9.22 |10.01 |10.44 |9.74 |9.88 |9.92 |9.56 |10.08 |10.08 |

|10.12 |9.69 |10.24 |10.23 |10.89 |10.22 |9.92 |10.21 |9.60 |10.19 |

|9.76 |10.32 |10.04 |9.88 |10.02 |9.62 |9.76 |9.46 |10.42 |9.34 |

|10.20 |10.06 |10.36 |9.16 |9.54 |9.76 |9.20 |10.00 |10.44 |10.48 |

|9.88 |9.92 |9.56 |10.08 |10.09 |9.58 |9.76 |9.51 |9.68 |9.82 |

|8.84 |10.04 |9.88 |10.11 |10.06 |9.46 |9.72 |9.28 |10.02 |9.89 |

The Mathematics of Failure and Reliability 183


## 4.2 Statistics and Definitions


of a histogram, shown in Figure 4.1, where the ordinate is the number (or percent) of failures. Since the histogram is approximately symmetric about 10 10 A with only a ±5% spread, the distribution of failures is deemedA with only a 5% spread, the distribution of failures is deemedacceptable. It is common to plot failure data in another way. The number of failures that occur at less than or equal to a given value is noted, then a cumulative distribution function (CDF) can be deﬁned. Such cumulative distribution numbers for the indicated fuse current values are also listed in Table 4.2 and plotted in Figure 4.2.


The continuous normal, or Gaussian, distribution function is ideally suited to mathematically treat these data. This widely used, two-parameter function was used previously in connection with yield (see Figure 3.26).


Discovered in 1733 by De Moivre as the limiting form of the binomial distribution for discrete random variables, the normal distribution deals with the statistics of random events, numbers, and phenomena. Underlying the validity of this function is the central limit theorem, which states that when the sample size is very large, the distribution of means approximates a normal distribution. Thus a superposition of the independent random variables, each of which contributes a small amount to the total, always tends toward normality. As the number of contributing factors increases,the approximation becomes more exact. This condition certainly obtains in IC manufacturing with tens of photomask steps and hundreds of individual process steps, each of which can introduce defects.


Table 4.2 Frequency and cumulative distributions of fuse test currents Frequency distribution


ive distributions of fuse test currents Frequency distribution


|Cell |Current limits |Number in cell |Upper current |Cumulative number |
|---|---|---|---|---|

|1 |8.70e8.90 |2 |8.90 |2 |

|2 |8.90e9.10 |0 |9.10 |2 |

|3 |9.10e9.30 |7 |9.30 |9 |

|4 |9.30e9.50 |6 |9.50 |15 |

|5 |9.50e9.70 |15 |9.70 |30 |

|6 |9.70e9.90 |22 |9.90 |52 |

|7 |9.90e10.10 |22 |10.10 |74 |

|8 |10.10e10.30 |14 |10.30 |88 |

|9 |10.30e10.50 |10 |10.50 |98 |

|10 |10.50e10.70 |0 |10.70 |98 |

|11 |10.70e10.90 |2 |10.90 |100 |

Cumulative distribution


8.899.29.49.69.810 10.2 10.410.6 10.8


CURRENT (A)


Figure 4.1 Frequency-distribution function for fuse failure data plotted in the form of a histogram representing the number of failed fuses in discrete current intervals.


CUMULATIVE PERCENTAGE20


0+


11


凹


Figure 4.2 Cumulative distribution function plot for fuse-failure currents.


The Mathematics of Failure and Reliability 185


台


NUMBER PER CELL古


The probability distribution function (PDF) that deﬁnes the normal distribution is f(x) has the familiar mathematical form


fx ¼ 1sð2pÞ1=2exp exp ðx (x-u)mÞ22s2;


(4.1)


where the quantities s and m are deﬁned in the bell-shaped curve of unit area (Figure 4.3(a)). For a distribution of values it is evident that m is the mean value and s is a measure of their spread about the mean known as the standard deviation. From statistics we know that m is the sum of the individual xi values divided by the number of data points (n), i.e., m ¼ Sxi/n,where where the sum is over i. Similarly, σ is defined as {Σ(u - xj)2/(n - 1)}1/2.the sum is over i. Similarly, s is deﬁned as {S(m  xi)2/(n  1)}1/2.Using these deﬁnitions, m and s for the fuse current data can be readily evaluated.


It It is customary to express x in standard units, ≥=(x - u)/σ, because theis customary to express x in standard units, z ¼ (x  m)/s, because the simpler mathematical form, based symmetrically about the origin,


fz ¼ 1ð2pÞ1=2exp(2)z22;


(4.2)


results. This equation suggests that z is normally distributed with m ¼ 0 ands ¼ 1.


4.2.2 Statistical Process Control, Cpk, and “Six Sigma”


The application of statistics to IC fabrication can be for either discrete variables, such as defects, or continuous variables, such as threshold voltage of MOSFETs. A state-of-the-art IC fabrication process has approximately 25 mask levels and about 600 individual process steps. Each process step and masking level can introduce defects, all of which can potentially impact the yield and reliability of an IC. Defects at any process step will impact yield and reliability. For example, slight variations in oxide thickness, stored oxide charge, semiconductor doping in the channel, or even channel length will inﬂuence the threshold voltage of the 100 million CMOS FETs in a chip, as well as, the hundreds of chips in a wafer. Variations within a chip and from chip to chip will be manifest in ﬁnal test yield at the wafer level as we will discuss next. So the question is how to handle the control of the process and the defects introduced by processing. First we need to understand and appreciate some of the features of Eqn (4.1), which is widely employed in industry to monitor the extent of process and production


quality control. Sigma (s) is a measure of the spread of a measured process variable, say Vt (threshold voltage), a parameter used to infer yield. Vt has limits beyond which a chip or entire wafer will be scrapped (yield ¼ 0). Sofor critical parameters, such as Vt, oxide charge, oxide thickness, etc., these limits deﬁne an acceptable range of the parameter in question. Ideally, we would like the parameter mean centered between the upper limit and the


3.4 ppm


74


μ-6o μ-5o μ-4o μ-3o μ-2o μ-1o μ μ-10 μ-20 μ-30 μ-40 μ-50 μ-6ox→


Figure 4.3 (a) Plot of the normal probability distribution function f(x) ¼ 1/s(2p)1/2exp [(x  m)2/2s2] versus x. (b) Six Sigma quality statistics depicted in terms exp -[(x - μ)2/2σ2] versus x. (b) Six Sigma quality statistics depicted in terms ofofpositive and negative process shifts about the nominal target mean. The numbers of rejects that arise are shaded in at the extremes of the displaced distributions. From Ref. [6].


The Mathematics of Failure and Reliability 187


PROBABILITY


DENSITY f(x)


u-20 μ-ouu+oμ+20


f (x)


1.5o1.5o


lower limit that we will accept. We say the parameter mean should lie half way between the upper control limit (UCL) and the lower control limit(LCL) (see Figure 4.4). Then, if s is small, we expect the entire distribution(normal) for a single process step or mask level to lie within the UCL and the LCL for that parameter. Well, for a normal distribution w68.26% lies between between +σ and -σ, and ~95% lies between +2σ and -2o. Approxi-þs and s, and w95% lies between þ2s and 2s. Approxi-mately 99.7% lies between þ3s and 3s. If now the spread from mately 99.7% lies between +3o and -3o. If now the spread from +30þ3sto to -3o is small compared to the spread between UCL and LCL, then we3s is small compared to the spread between UCL and LCL, then wehave high certainty that the parameter is controlled well enough for our purposes. But wait again, we have hundreds of chips in a wafer and hundreds of millions of FETs on each chip. So if we only control to þ3s and 3s -3o we will possibly make scrap 0.3% of the time either on a chip or waferwe will possibly make scrap 0.3% of the time either on a chip or waferbasis, which on a chip basis implies we may never make a good chip. It became very important therefore to control parameters to much tighter levels in order to guarantee some yield. What we described is statistical process control (SPC), a method to ascertain that a process step is controlled well enough to yield greater than zero.


A more sophisticated method measures terms Cp and Cpk to determine the capability of a process. Cp ¼ (UCL  LCL)/6s and Cpk ¼ Cp(1 where k is the ratio of the mean drift to (UCL - LCL)/2. Cp measures the capability of a process. Cp = (UCL - LCL)/6σ and Cpk = Cp(1 - k),k),where k is the ratio of the mean drift to (UCL  LCL)/2. Cp measuresshort-term capability (see Figure 4.5) and Cpk measures long-term process capability (see Figure 4.6). The interested reader is referred to an excellent


Figure 4.4 Statistical process control chart.


p Control Chart


45%


40%大UCL=36.16% De fective15%10%


5%


0%LC=278


20032/1/2/2/2003


2/3/20032/4/2003-2/5/20032/6/20032/7/20032/8/20032/9/2003


20032/10/Subgroup Number


2/11/20032/12/20032/13/20032/14/20032/15/2003


丰


20%-Avg=19.47 25%+月 30%1


35%十


book by E.E. Lewis [7]. These parameters measure how much of the process window (UCL  LCL) is used by the process and how well process window (UCL - LCL) is used by the process and how well thetheprocess is centered. Values of Cp and Cpk of 1 are marginal, whereas 2 or 3 are much better because less of the process window is covered by the spread of the parameter in question.


The next step in SPC is called “Six Sigma.” For example, “Six Sigma in everything we do.” [6] was a Motorola Corporation rallying call to increase competitiveness by enhancing the quality of products. Whereas


Short-term capability


Time 1


Time 2


Time 3


Time N


Long-term capability


Nonconformance


to standard


LSL


USLLSL


USL LSL


USL


Cp<1


Cp=1


Cp >1


Figure 4.5 Capability index Cp for normal distribution from Ref. [7].


LSLNOMINALUSL


Figure 4.6 Long term process capability from Ref. [7].


The Mathematics of Failure and Reliability 189


68.26% of the area under the normal distribution or product distribution curve falls within 1s (s to þs), 99.7% within 3s, and 99.9999998%falls within 6s (6s to þ6s). Manufacturing processes, however,experience shifts in the mean as great as 1.5s in practice becauseequipment, operators, and environmental conditions are never constant.


Six Sigma quality is therefore deﬁned as the number of rejects that occur when such shifts happen (Figure 4.3(b)). This, in effect, means tolerating no more than 3.4 defective parts per million produced. It amounts to w4.5s of allowable variability. A strict Six Sigma would result in two defective parts in 1 109. IC chips in the near future will contain 1 109FETs and most likely require the strict Six Sigma control of defects. An example of long-term capability is shown in Figure 4.7. Of course,achieving Six Sigma quality is easier said than done, but it remains a vital challenge for industry. Those inclined can calculate what seven sigma implies!


4.2.3 Accuracy and Precision


We have just seen that failure testing is subject to a Gaussian spread; the same is true of all property measurements and manufacturing-quality control monitoring. With respect to measurements the most often asked questions are, how accurate are they, and with what precision are they made The distinction between these two terms can be immediately grasped by viewing Figure 4.8. High shooting accuracy is achieved in both Figure 4.8(a) and (b) because the target hits are centered around the bull’s-eye. Thus the mean value m is the same in both cases and not far from the distribution center. But the precision of the shooter is better in a than in b because all the bullet holes cluster and have a small dispersion,or spread. High precision is thus characterized by a small s; equivalently,we speak of a small random uncertainty. Poor accuracy is attained in Figures 4.8(c) and (d) because all holes are far off the bull’s-eye; here we speak of a large systematic uncertainty. Again, shooter precision is better in c because all the bullet holes cluster more tightly. The case in d is worst of all because neither accuracy nor precision is achieved; i.e., both s and m are large.


Is it more desirable to have high accuracy or high precision? Good shooting instructors know that it is better ﬁrst to work on attaining smaller clusters or groupings. Thus the path to becoming a sharpshooter is to be precise ﬁrst. Accuracy can then be gained by adjusting or calibrating the movable sights.


Figure 4.7 Long term process capability from Ref. [7].


The Mathematics of Failure and Reliability 191


Rolled - throughput yield (%)20


110100100010,000100,000 1,000,000 Complexity


110100100010,000100,0001,000,000 Complexity


● Six sigma


o Five sigma


■Four sigma


□Three sigma


Note: Long-term capability based on an equivalent, one-sided 1.50 mean shift


30 40 50召 d 80 100


90 30 40 50 60 70 80 1000


4.2.4 Failure Rates


The fuse current data treated above were essentially time independent.


Reliability, however, implies time dependence of failure, with time reckoned from the instant the product is put into service. To include time (t) weﬁrst deﬁne the PDF to be f(t). Therefore, the CDF, deﬁned by F(t), is given by the integral


Ft ¼ Z


f ðyÞdy;


(4.3)


where the lower time limit is taken to be N instead of 0 for mathematicalpurposes, and y is a dummy variable of integration. For a given population,F(t) is the fraction that fails up to time t, and it is related to the PDF by


Figure 4.8 Four target-shooting characteristics depicted schematically in both


graphical and statistical terms. (a) Good precision–good accuracy; small s and small


shift (X1) from target center (X0). (b) Poor precision–good accuracy; large s and small X1.


(c) Good precision–poor accuracy; small s and large X1. (d) Poor precision–poor accuracy; large s and large X1. From Ref. [8].


f(t) ¼ dF(t)/dt. A reliability, or survival, function, R(t), can then be deﬁnedto indicate the surviving fraction, i.e.,RðtÞ R(t)=1-F(t).¼ 1 FðtÞ:


(4.4)


The failure rate (also known as the hazard rate), l(t), is deﬁned as the number of products (e.g., devices) that failed between t and t þ Dt, per timeincrement Dt, as a fraction of those that survived to time t. This complex deﬁnition of the failure rate is written as


lt_F(t+△t)-F(t) ¼ Δt(1 - F(t))Fðt þ DtÞ  FðtÞDtð1 FðtÞÞ ¼ 1-F(t)f ðtÞ1 FðtÞ ¼f ðtÞRðtÞ


(4.5)


by employing F(t) and its derivative. From this it is easy to show that l(t) λ(t)=-dlnR(t)/dt.¼ dlnR(t)/dt.A good way to appreciate how failure rates are calculated is through a couple of practical examples.


Example 4.1


Suppose that a population of 525,477 solid-state devices is burned in at elevated temperature, and the number of failed devices are weeded out as a function of time is recorded in the following table. Determine the failure rates, l(t), at the indicated times.


Answer


Results of the calculations are tabulated.


Time(h)


Number failed, f(t)


Cumulative


failures, F(t) l(t) (hL1)


|1 |6253 |6253 |0.0119 |525,477 x 1|1.19 x 107|
|---|---|---|---|---|---|

|2 |1034 |7287 |0.00199 |519,224 x 2|9.96 x105|

|3 |617 |7904 |0.00119 |518,190 x 3|3.97 x105|

|4 |419 |8323 |0.000810 |517,573 x 4|2.02 x105|

|5 |502 |8825 |0.000971 |517,154 x 5|1.94 x 105|

|6 |401 |9226 |0.000777 |516,652 x 6|1.29 x 105|

|7 |297 |9523 |0.000577 |516,252 x 7|8.22 X 104|

|8 |214 |9737 |0.000415 |515,954 x 8|5.18 X 104|

|9 |206 |9943 |0.000400 |515,740 x 9|4.44 X 104|

|10 |193 |10,136 |0.000375 |515,534 x 10|3.74 x104|

Number of device hours


FITs


Sample calculation at 5 5h using  EEqn  (4.5): λ(t) =502/525,477 x (1 - 8323/525,477)-1l(t) ¼ 502/525,477  (1  8323/525,477)1¼ 0.0009710/h.


Because the failure rates are very low, a new numerically larger unit, the FIT, has


been deﬁned and is widely used in the microelectronics industry. The FIT is not an acronym, but a contraction of “failure unit”; it equals the number of failures in 109 device-hours. For example, 1 FIT is one failure in 109 device-hours, one failure in 107 The Mathematics of Failure and Reliability 193


devices after 100 h of operation, or one failure in 106 devices after 1000 h, etc.


Employing this deﬁnition, failure rates in terms of FITs were generated, and the values are displayed in the last column of the above table. After 5 h, for example, l(t) ¼ (502/517,154  5)  109 ¼ 1.94  105 517,154 x 5) x 109 = 1.94 x 105 FITs.FITs.


4.3 ALL ABOUT EXPONENTIAL, LOGNORMAL,


AND WEIBULL DISTRIBUTIONS


4.3.1 Exponential Distribution Function


4.3.1.1 Mathematics


We have already introduced the normal distribution function, whose PDF was given by Eqn (4.1). It was used to assess product properties or quality,and no time dependence was attached to the variable of interest. There are three additional PDFs, the exponential, lognormal, and Weibull, that can also be used like the normal distribution function in evaluating quality control. But in this book they have a more vital role; they are called upon to analyze and characterize failure and reliability data in material systems with the objective of predicting future behavior. Therefore, time, not a property relating to quality, is now the variable of interest. Of these functions the most simple mathematically is the exponential distribution.


The exponential PDF is deﬁned by


f f(t) =λoexp(-λot),ðtÞ ¼ lo expð lotÞ;


(4.6)where lo is a constant. Through simple integration (Eqn (4.2)) the CDF is evaluated to be


F(t)=fλ。exp(-λop)dy=1-exp(-λot).lo expð loyÞdy ¼ 1 exp lot: (4.7)


Finally, the failure rate is given by


lt ¼ 1-F(t)f ðtÞ1 FðtÞ ¼[1-(1-exp-λot)]lo doexp(-hot)expð lotÞ½1ð1 exp lotÞ ¼ lo; (4.8)and, importantly, is seen to be constant. Therefore, the mean time to failure(MTTF) is the reciprocal, or 1/lo. Plots of the functions f(t), F(t), and l(t)are depicted in Figure 4.9 as a function of time (in 1/lo units).


## 4.3 All About Exponential, Lognormal, and Weibull Distributions


Example 4.2


Suppose the population of devices is described by the life distribution F(t) ¼ 1  Suppose the population of devices is described by the life distribution F(t) =1- exp (-0.0001t).exp(0.0001t).1. What is the probability that a new device will fail after 1000 h? After 5000 h?Between these times?


2. What is the failure rate at 1000 h? After 5000 h?


1. By substitution, F(t) ¼ 1  exp [0.0001(1000)] ¼ 0.095. Similarly, at 5000 h,F(t) ¼ 0.39. The probability of device failure between 1000 and 5000 h  Answer 1. By substitution,F(t)=1-exp[-0.0001(1000)]=0.095.Similarly,at5000h, F(t) = 0.39. The probability of device failure between 1000 and 5000 h is F(5000) -F(1000) =0.39-0.095 =0.30. 2. f(t) = dF(t)/dt = 0.0001 exp(-0.0001). The failure rate is λ(t) =f(t)/ [1 -F(t)] = 0.0001 exp (-0.0001t)/exp (-0.000t) = 0.0001. For this distribution the failure rate is seen to be time-independent.isF(5000)  F(1000) ¼ 0.39  0.095 ¼ 0.30.2. f(t) ¼ dF(t)/dt ¼ 0.0001 exp(0.0001). The failure rate is l(t) ¼ f(t)/[1  F(t)] ¼ 0.0001 exp (0.0001t)/exp (0.000t) ¼ 0.0001. For thisdistribution the failure rate is seen to be time-independent.


4.3.1.2 Constant Failure Rate Modeling


Due to ease in dealing with a constant failure rate, the exponential distribution function has proven popular as the traditional basis for reliability(a)


PROBABILITY DENSITY f(t)


DISTRIBUTION FUNCTION F(t)


1.0-


f(t) = λoexp [-λot]


F(t) = 1 - exp [-λot]


TIME t no2/no3/no


1/no2/no3/no


(c)HAZARD FUNCTION λ(t)3λ0


2λ0


入o


TIME t


ol


01/No2/no3/Noλ(t)=λo


01


Figure 4.9 Plots of exponential distribution functions. (a) f(t) versus time. (b) F(t) versus time. (c) l(t) versus time. Time is measured in units of 1/lo.


The Mathematics of Failure and Reliability 195


modeling. For the reasons enumerated below, some of which are historical in nature, it is not difﬁcult to see why the constant failure rate model has been so widely used [1].


1. The ﬁrst generalized reliability models of the 1950s were based on electron vacuum tubes, and these exhibited constant failure rates.


2. Failure data acquired several decades ago were “tainted by equipment accidents, repair blunders, inadequate failure reporting, reporting of mixed age equipment, defective records of equipment operating times, mixed operational environmental conditions .” [9]. The net effect was to produce what appeared to be a random constant failure rate.


3. Early generations of electronic devices contained many intrinsically high failure rate mechanisms. This was reﬂected in different infant mortality and wear-out failure rates in subpopulations, and contributed to the appearance of a constant failure rate for products in service.


4. Even in the absence of signiﬁcant intrinsic failure mechanisms, early fragile devices responded to random environmental overstressing by failing at a roughly constant rate.


5. It often happens that equipment repeatedly overhauled or repaired contains a variety of components in a variable state of wear. Even though each of the components probably obeys time-dependent failure distributions,e.g., lognormal or Weibull, the admixture of varying projected lifetimes may conspire to yield a roughly time-independent rate of failure.


6. The simple addition of a decreasing infant mortality rate and an increasing wear-out failure rate results in a roughly constant failure over a limited time span.


Given these reasons it is not difﬁcult to see why the U.S. Department of Defense and its associated agencies (e.g., Rome Air Development Center,Navy) and assorted military electronics contractors (e.g., RCA, Boeing Aircraft Company) adopted the exponential model as a basis for reliability prediction and assessment. In the Military Handbook (MIL-HDBK-217),cited in Chapter 1, failure rates for devices and components are generally given in the form


lp ¼ lbpTpQpE. ¼ lbPpi;


(4.9)


where lp is the part failure rate and lb is the base failure rate usually expressed by a model relating the inﬂuence of electrical and temperature stresses on the part. The individual p factors take into account the roles of temperature (T), quality (Q), and environment (E) as well as other


variables that may inﬂuence failure rates (e.g., voltage-stress factor, forwardcurrent factor).


A page fromMIL-HDBK-217 is reproduced in Figure 4.10, enabling us to calculate failure rates for low-frequency, siliconFETs.The temperature factor is easily recognized to be the thermally activated Maxwell–Boltzmann factor,


MIL-HDBK-217F


6.4 TRANSISTORS, LOW FREQUENCY, SI FET


SPECIFICATION


DESCRIPTION


MIL-S-19500


N-Channel and P-Channel Si FET(Frequency ≤400 MHz)λp=λbπTπAπQπE Failures/106 Hours


Base Failure Rate -λb


|Application (Pr,Rated Output Power)|πA|
|---|---|

|Linear Amp lification (Pr<2W) Smell Signal Switching|1.5 .70|

|Power FETs (Non-linear, Pr≥2W)||

|2≤Pr<5W|2.0|

|5 ≤ Pr<50W|4.0|

|50 ≤ Pp< 250W|8.0|

|Pr ≥ 250W|10|

|Transistor Type|入b|
|---|---|

|MOSFET|.012 .0045|

|JFET|.012 .0045|

Application Factor - πA


Temperature Factor - πT


|Tj(°C)|"T|TJ (°C)|"T|
|---|---|---|---|

|25|1.0|105|3.9|

|30|1.1|110|4.2|

|35|1.2|115|4.5|

|40|1.4|120|4.8|

|45|1.5|125|5.1|

|50|1.6|130|5.4|

|55|1.8|135|5.7|

|60|2.0|140|6.0|

|65|2.1|145|6.4|

|70|2.3|150|6.7|

|75|2.5|155|7.1|

|80|2.7|160|7.5|

|85|3.0|165|7.9|

|90|3.2|170|8.3|

|95|3.4||8.7|

|100|3.7|175||

|πT =exp (-1925 (TJ+273 298)) Tj=Junction Temperature (°C)|πT =exp (-1925 (TJ+273 298)) Tj=Junction Temperature (°C)|πT =exp (-1925 (TJ+273 298)) Tj=Junction Temperature (°C)|πT =exp (-1925 (TJ+273 298)) Tj=Junction Temperature (°C)|

Environment Factor-πE


|Environment|TE|TE|
|---|---|---|

|GB||1.0|

|GF||6.0|

|GM||9.0|

|Ns||9.0|

|NU|19||

|AIC|13||

|AIF|29||

|AuC|20||

|AUF|43||

|ARW|24||

|SF||.50|

|MF|14||

|ML|32||

|CL|320||

Quality Factor-TTQ


|Quality|πQ|
|---|---|

|JANTXV JANTX JAN Lower Plastic|.70|

|JANTXV JANTX JAN Lower Plastic|1.0|

|JANTXV JANTX JAN Lower Plastic|2.4|

|JANTXV JANTX JAN Lower Plastic|5.5|

|JANTXV JANTX JAN Lower Plastic|8.0|

Figure 4.10 Failure rate for low-frequency ﬁeld-effect transistors. Pages 6–8 reproduced from MIL-HDBK-217F.


The Mathematics of Failure and Reliability 197


while the quality factor applies to the speciﬁc device model and the type of package. Environmental factors vary widely between the extremes of “ground benign” conditions (GB ¼ 1) and a cannon launch (CL ¼ 450). In addition,there is a fourth application factor pA that depends on the power level. For example, in the case of a plastic encapsulated small signal switching MOSFET operating at 30 C, and used in space ﬂight (SF), a failure rate of lp ¼ 0.012  1.1  8.0  0.50  0.70 ¼ 0.037 per 106 h, or 37 FITs ispredicted. Be forewarned that the Handbook’s precision greatly exceeds its accuracy by several orders of magnitude!


4.3.1.3 Is Constant Failure Rate Modeling a Paradigm in Transition?


This question has been discussed by McLinn [10], who suggested that it is time to create a new and better paradigm to replace the “defunct” exponential distribution that has served electronics for the past 45 years. Based on a 1991 critical review [1] of proposed reliability models for advanced microelectronic devices of high gate count (e.g., VLSI, VHSIC), it was recommended that the assumption of a constant failure rate be considered invalid. This was particularly true for device failures caused by electromigration and dielectric breakdown phenomena. In addition, years of experience has shown that failure-rate predictions using existing MIL-HDBK-217 speciﬁcations can differ by several orders of magnitude for the same device depending on the manufacturer. Far from exhibiting a constant failure rate, it is well known that infant-mortality failures of semiconductor products display a decreasing failure rate with time. In addition, recent generations of semiconductor products are signiﬁcantly more reliable than their predecessors and exhibit low failure rates.


To address these facts, MIL-HDBK-217 has incorporated additional terms such as the learning factor pL, which attempts to weigh the effect of the number of years (Y) the product has been in production. One such explicit form is pL ¼ 0.01 exp (5.35  0.35Y). Inclusion of this time factoreffectively results in a decreasing rather than constant hazard rate. Alternative constant failure-rate-reliability prediction procedures by various companies (e.g., AT&T, Bellcore, British Telecom, France Telecom,Nippon Telegraph, Telephone) have been developed. Finally, total abandonment of MIL-HDBK-217 speciﬁcations by some US device manufacturers as well as by Japan and other Paciﬁc Rim nations in favor of physical investigations of the root causes of failure has become increasingly popular. Primarily because it is well known that, on two different process lines in the same company, the same product with the same process may


exhibit quite different process variability, which may change the root cause of failure, the failure rate, and its model. Therefore the origin of the product can sometimes inﬂuence its behavior.


In conclusion, two broad viewpoints of addressing reliability,MIL-HDBK-217 versus the physics of failure, are compared item by item in Table 4.3 to expose relative advantages and shortcomings.


4.3.2 Lognormal Distribution


Shortcomings in the exponential distribution function have prompted the use of alternative distribution functions to model reliability data. One of the most popular of these is the lognormal distribution function. Mathematically, the lognormal is not a separate distribution, because by taking natural logarithms of all data points, the transformed data can be analyzed as a normal distribution. The lognormal PDF is given by


f ðtÞ ¼ 1tsð2pÞ1=2exp½ðlnðtÞ  lnðmÞ22s2(4.10)


while the lognormal CDF has the form


Ft ¼ Fs1 lntm:


(4.11)


Here Fz ¼ 121þ Erf ðz=21=2Þ or 122 Erfcðz=21=2Þ, since Erfc(z/21/2) ¼ 1  Erf(z/21/2).Substitution in Eqn (4.8) shows that the hazard function is given by lðtÞ ¼ 21=2 exp 12s2 lnðt=mÞ2p1=2tsErfchlntm.sð1=2Þ1=2i:


(4.12)


In these expressions the error function (Erf) and complementary error function (Erfc) are related to the integral of the Gaussian function and appear in connection with solutions to diffusion problems (see Eqn (5.4)).


Both range from 0 to 1, while their arguments assume any values. Comparison with Eqn (4.1) reveals that the lognormal distribution is derived from the normal distribution by substituting ln t for x. Just as there are two parameters that deﬁne the normal distribution, two parameters also deﬁne the lognormal distribution. The ﬁrst is m, which has the physical signiﬁcance of representing the median time, or time when 50% of the


The Mathematics of Failure and Reliability 199


Table 4.3 Comparison of reliability prediction methodologies Issue


MIL-HDBK-217


T


,


j


A  T


P r e s s u r e  d i f f e r e n t i a l,


a t m o s p h e r e


P r e s s u r e


V


v o l t a g e,


e l e c t r i c


e l d,


A


a r e a,


Q


s s


i n t e r f a c i a l


x e d  c h a r g e,


t e m p e r a t u r e,


c u r r e n t  d e n s i t y,


h u m i d i t y.


f t e r  R e f. [2 4].


226ReliabilityandFailureofElectronicMaterialsandDevices


stresses. Based on the Nernst–Einstein approach to reactions and processes introduced in Section 1.3.3, it is not difﬁcult to incorporate such effects into an expression for predicted times to failure. The stresses may exponentially affect lifetime, serve to reduce the effective activation energy for failure, be a multiplicative factor, or appear as some combination of these in


Figure 4.23 (a) Simulated device failure data at different temperatures plotted as lognormal distributions. (b) Lifetimes (MTTF) corresponding to 50% cumulative failures plotted as log MTTF versus 1/T (K).


The Mathematics of Failure and Reliability 227


(a) 0.999


|||||||D|||||||
|---|---|---|---|---|---|---|---|---|---|---|---|---|

|||||(①)|||||||||

0.998


0.995


0.99


0.98


0.97


0.96


0.94


0.90


0.84


0.80


0.75


0.70


0.60


0.50


0.40


0.30


0.25


0.20


0.16


0.10


0.08


0.06


0.04


0.02


0.01


0.005


0.002


0.001


Time (h)


expressions for MTTF. A form of the Eyring model for the inﬂuence of an additional stress in addition to temperature is thus


MTTF ¼ ATa expERTexp1RBþ CT; (4.45)


where a, A, B, and C are constants. Often the inﬂuence of the exponential factor swamps that of the Ta term, so that it is sometimes omitted, in which case we are back to Eqn (4.43). Reliability practitioners have often invoked assorted variants of this phenomenological equation in the literature. One example of the form


MTTF ¼ AVb expERT


(4.46)is used for situations where voltage (V) acceleration is operative. To use this formula, three constants, A, b, and E, must be known or estimated.


4.5.8 Is Arrhenius Erroneous?


Among the issues involving reliability prediction, the exact role of temperature in accelerating failure is one of the most controversial. Traditionally thought to be the prime variable inﬂuencing the failure of microelectronics through thermal activation of damage mechanisms,Hakim [27] raises the question, “Is Arrhenius erroneous?” This critic


Figure 4.23 dContinued 228 Reliability and Failure of Electronic Materials and Devices


contends that lowering the operating temperature of equipment will not necessarily improve system reliability. If true, the size of cooling systems in electronic equipment could be reduced, with with no loss of reliability an added bonus. In general, temperature AFs in MIL-HDBK-217 may work well for individual devices and components. But a large proportion of electronic systems failures today are not caused by parts failures but by other events within the system such as electromagnetic interference, timing problems, electrostatic discharge, and mishandling [28]. This again raises questions as to the utility of MIL-HDBK-217.


Pecht et al. [29] have addressed the role of temperature, with an emphasis on those integrated circuit failure mechanisms operative in the range 55 to 125 C. They suggest that most mechanisms have notquantitatively distinguished the roles of steady-state temperature, temperature transients, rate of temperature rise or drop, and temperature gradients.


This assessment is probably correct simply because the admixture of these effects with those of the simultaneously operative nonthermal stresses, all within the complex geometry and environment of devices, makes failure modeling practically intractable. A consequence of this is the wide


Figure 4.24 Arrhenius plots of mean dielectric breakdown times (t50) for 15 nm thick SiO2 ﬁlms. Data points are derived from lognormal failure distributions obtained at the indicated electric ﬁelds. Note that in Figure 6.13 the activation energy for breakdown is


essentially independent of electric ﬁeld. From Ref. [26].


The Mathematics of Failure and Reliability 229


variability of activation energies reported in Table 4.4. Questions related to whether failures at elevated temperatures are the same as those at use temperatures, and whether mechanisms and activation energies change,have already been raised; they will be addressed again in Section 4.6.3.


Blanks [30] in a similar vein has questioned the validity of the Arrhenius relation when nonconstant failure rates prevail. He suggests that the temperature-dependent rate of equipment failure is less than that predicted by the Arrhenius AF when the hazard rate decreases with time. This implies that failure lifetimes would be underestimated in the case of common lognormal failure distributions. Conversely, when the hazard rate increases with time, the Arrhenius AF would overestimate equipment failure rates.


The Arrhenius truth of increased atom movements and reaction rates with rising temperature is not being challenged in these collective criticisms.


Our ignorance lies in how to unambiguously isolate and characterize individual damage mechanisms when an admixture or distribution of activation energies may exist. Nevertheless, blaming steady-state temperatures for failures and blindly invoking Arrhenius AFs probably shifts emphasis away from design and manufacturing deﬁciencies in many cases.


4.5.9 The Bathtub Curve Revisited


In Section 1.3.8 the famous bathtub curve, so named for its shape, was introduced as a way to plot failure rates over product life cycles. The early failure, or “infant mortality,” regime has, for understandable reasons, been the subject of considerable scrutiny for many years. During short times the weak or marginally functional members of the population fail according to a decreasing failure rate. In a model developed at AT&T [31] based on life testing under simulated ﬁeld conditions, the bathtub curve is plotted as the hazard function, or failure rate (in FITs) versus time, as shown in Figure 4.25(a). Early failures are modeled by a Weibull hazard function of the form l(t) ¼ l(0)t(1b), where 1  b < 1, and l(0) is basically the initialfailure rate. On the log l – log t plot the resulting declining failure rate line is deﬁned by an w20 FIT data point after a period of 104 h, a time somewhat longer than 1 year.


The temperature dependence of infant failures is important because of thermal burn-in screening. Assorted bipolar, MOS, and electro-optical device families have surprisingly exhibited a common low activation energy ranging from 0.25 to 0.4 eV despite the fact that many different failure mechanisms are involved [33]. Following elevated temperature stressing,hazard rates at service temperatures can be estimated by calculating the


appropriate AF and substituting it into Eqn (4.40). Failures on the left-hand edge of the bathtub curve reﬂect workmanship defects that include faulty design, omitted inspections, and mishandling. Particulates and contamination during the processing of IC chips are also leading causes of early failures.


Beyond the infant mortality regime is the long, roughly ﬂat portion known as the intrinsic failure period. Failures occur randomly in this region,and the failure rate is approximately constant. Mathematically, the constant hazard rate of the exponential distribution is admirably suited to model such random failures. Most of the useful life of a component is spent here,so that much reliability testing is conducted to determine values of l in this region.


Figure 4.25 (a) Bathtub curve plotted as the hazard function or rate (in FITs) versus log time. The failure rates are typical but do not correspond to any particular device. (b)Roller coaster l(t), which starts high initially, falls to a local minimum (a valley), and then rises up and over a hump ﬁnally to merge with ﬂatter portions. From Ref. [32].


What is more revealing is the ratio of the two-system failure rates, i.e.,ls (c)/ls(h), which is plotted in Figure 4.21. Cold sparing is predicted to have a considerable advantage over hot sparing, particularly at earlier times.


In In the example given above, λs (c)/λs (h) = 7 x 10-2 after 10 years. Despitethe example given above, ls (c)/ls (h) ¼ 7  102 after 10 years. Despitethese predictions, it may be physically difﬁcult to realize the beneﬁts of cold sparing in practice. For example, the regenerator could fail not because of wear out, which is what has been tacitly assumed all along. Rather, material creep may slowly misalign each laser with respect to its ﬁber and allow less light to enter it. Since this creep mechanism occurs whether or not the laser is turned on, the system is essentially hot spared.


TIME t/MEDIAN LIFE tm


Figure 4.20 Plot of the cold spared failure rate, ls(c) versus time. From Ref. [12].


1011


10u


14.5-4


109


3.5


3.25


08h


1.25


nu. .3入可Lu


2.75 2 106L 0


v2.5


/21.5/10.5


2.251.751.25


Failure Rate λc (FITs) x Median Life tm (hours)105/m.dLh.山I umd1111


10-410-310-210-1100101102


0.75σ=0.25


1.50


σ=0.25


0σ=6


4.4.3 How MIL-HDBK-217 Treats System Reliability


Physics of failure


Relative cost of analysis


Low. Many computer programs available.


Implementation costs less than 1% of hardware cost.


Very high. Cost to


implement complex system may exceed that of


hardware.


Device coverage


Covers 19 major electronic device categories.


Addresses microcircuits only.


No models for other


Device defect modeling


Assumes ﬁeld failures are caused by random defects accelerated by operating stresses.


Failure mechanisms generally neglect impact of


manufacturing defects.


Device design modeling


Assumes design is perfect(based on qualiﬁcation


testing). Assumes all failures are caused by manufacturing defects.


Assumes ﬁeld failures are caused by poor device designs. Ignores handling and manufacturing defects.


Model


development


Models based on a statistical analysis of actual ﬁeld


failures (statistical models).


Develops models based on principles of physics,


chemistry, mechanics and materials (deterministic models).


DoD/Industry


Used successfully on thousands of military development efforts over past 30 years.


No complete system analysis ever documented.


Coordination All updates undergo DoD,tri-service and industry coordination


Developed models have never been coordinated.


Input data required


Minimal. Readily available to the system designer in terms of part type, stress,characteristics


Extremely extensive.


Information difﬁcult to


obtain without testing.


Variations in material


property can cause wide swings in model predictions.


Output data Predicts relative frequency of device failures in a


population. Failure rates can be summed and scaled to yield system behavior.


Alternate designs can be compared.


Predicts the time of


occurrence of speciﬁc failure mode in a speciﬁc device.


Reliability is based on


weakest part. Comparisons only on weakest links.


distribution will fail, i.e., m ¼ ln t50. Second, there is the shape parameter s,which strongly inﬂuences the shape of f(t) and F(t), as shown in Figure 4.11(a) and (b). Note that s is not the standard deviation of a population of lifetimes as in the normal distribution. Also shown in Figure 4.11(c) is the variation in lognormal failure rates as a function of s.


Later, in Section 4.3.5, it is shown how to extract s values from reliability plots. Large values of s (s > 2) reﬂect initially high failure rates that decrease with time. When a semiconductor product is in early manufacture,and quality control is still a problem, typical values of s are as high as 3 or 4.


Such values are indicative of processing and failures that are out of control.


Later, when manufacturing has advanced along the learning curve and the product is a candidate for high-reliability applications, s z 1 or less [12].


When s is close to 1, the failure rate is roughly constant, but it increases for values of less than w0.5. Thus the lognormal distribution can represent the early failure, steady state, or wear-out time regimes in the life of devices. As an example, failure times of GaAs–AlGaAs lasers aged at 70 C are plotted in lognormal fashion in Figure 4.12.


A useful and widely employed way to display the hazard rate for lognormal distributions, known as the Goldthwaite plot, is shown in Figure 4.13 [14]. Based on Eqn (4.12), this representation plots the failure


Table 4.3 Comparison of reliability prediction methodologiesdCont'd Issue


Arrhenius model


Used to empirically model temperature versus


reliability.


Used to obtain temperature acceleration of corrosion,electromigration, solder creep, etc.


Appropriate application


System design. Parts count can be applied with very limited information.


Component design.


Device screening


Recognizes that device screening reduces latent defects and ﬁeld failures.


Screening has no impact on component design. Assumes defect-free components.


Operating temperature


Direct impact on the


frequency of failure but not as large as critics claim.


Promoters claim microcircuit device reliability is


independent of temperature below 150 C.


Temperature cycling


Accounted for in the environmental factor.


Models focus on


temperature cycling as primary cause of failure.


The Mathematics of Failure and Reliability 201


rate (in units of FITs  t50) versus the normalized time t0 (a ratio of t/t50) rate (in units of FITs Xt50) versus the normalized time t'(a ratio of t/t50) forfordifferent values of s. It is apparent that an increase in s has the effect of moving the failure-rate peak to shorter times; that is why small s values are desired. Superimposed on the ﬁgure are plots of the locus of constant failure rate (lo) at a given time to. Thus the ordinate l t50 is taken as lo t50, so that l t50 t50 =(λo to)/(to/t5o). This equation plots as a straight line with a slope of -1¼ (lo to)/(to/t50). This equation plots as a straight line with a slope of 1in the log–log plot of Figure 4.13. The interested reader should determine what sample size and data could be used to measure t50 ¼ 108 h and a life of40 years. Often projections are far more precise than we can measure. Are they then accurate? What conﬁdence is there in their use?


As an application [16] of this ﬁgure, consider a failure distribution with s ¼ 2. The failure rate is low initially, but it rises with time. Whent/t50 z 3  103, the failure rate is 10 FITs, and t is equal to 40 years. t/t50 ≈ 3 x10-3, the failure rate is 10 FITs, and t is equal to 40 years. ForForthis this to happen t50 must be equal to 1.2 x 108 h; if t50 is less than this value,to happen t50 must be equal to 1.2  108 h; if t50 is less than this value,the failure rate will increase to more than 10 FITs in 40 years.


Figure 4.11 Plots of lognormal distribution functions. (a) f(t) versus time. (b) F(t) versus


time. (c) l(t) versus time. Time is measured in units of t50. Variations in lognormal distributions are shown as a function of s.


(a)PROBABILITY DENSITY f (t)


(b)1.0DISTRIBUTION FUNCTION F(t)


0.10.5


1.0=0


0.1=0


t502t503t500


t502t503t50


(c) 4r


十TIME 0t502t503t50 HAZARD FUNCTION λ(t)


4.3.3 Weibull Distribution


Like the lognormal, the Weibull is a two-parameter distribution. By adjusting a time scale parameter a and a shape parameter b, a variety of functional behaviors can be generated to ﬁt a wide range of experimental data. For example, the Weibull distribution applies to both decreasing failure rates, typical of early failures, and increasing failure rates that describe long-time wear out. The forms of the probability and CDFs are explicitly given by


ft ¼


btb1 exph ðt=aÞbiabb;a are constants > 0(4.13)


Ft ¼ 1 exph ðt=aÞbi:


(4.14)


Figure 4.12 Lognormal distribution of failure times for early vintage GaAs–AlGaAs lasers aged at 70 C. From Ref. [13].


The Mathematics of Failure and Reliability 203


These functions are plotted in Figure 4.14(a) and (b), together with the Weibull failure rate, (Figure 4.14(c)) which has the functional form


lt ¼ btb1ab_BrB-1:


(4.15)


There are a few cases of the Weibull distribution that are worth noting.


If, for example, b ¼ 1, we have the case of the exponential distribution.Explicit forms for the important reliability functions are then f(t) ¼ 1/aexp exp [-(t/ax)], F(t) = 1 - exp [-(t/α)], and λ(t) = 1/x.[(t/a)], F(t) ¼ 1  exp [(t/a)], and l(t) ¼ 1/a.When b ¼ 2, the Rayleigh distribution, a special case of the Weibulldistribution, emerges. The functions that characterize this distribution are given given byf(t) =(2t/a) exp [-(t/α)], F(t) =1-exp [-(t/a)2], and λ(t)=2t/a2.by f(t)¼ (2t/a) exp [(t/a)], F(t)¼ 1 exp [(t/a)2], and l(t)¼ 2t/a2.Rayleigh distributions are not normally used to describe the reliability of electronic products; however, this distribution function appears in an application to corrosion failure in Section 7.4.4. Signiﬁcantly, the hazard rate increases linearly with time.


Figure 4.13 Normalized plot of hazard rates for lognormal distributions having different values of s. After Ref. [15].


10-1010-810-6


1014nrn!I1000 AT17i 10 YEAR FIT 410-41111Yringrm21014σ=5.0σ=6.010


MEDIAN LIFE X FAILURE RATE IN FIT100k


106


o=2.75


σ=2.5/σ=2.25o=2.0/o=1.5o=1.0σ=0.5


, .d.dmithmil/σ=1.75g=1.25o=0.75=0.25104


|104|||1411 山,|uul|Al|山uul|川|
|---|---|---|---|---|---|---|---|

||10-10|10-8|10-6 10-4|10-2||100|102|

||||t'=TIME/MEDIAN LIFE|||||

o=3.0


o=3.25


高


108


o=3.5


75.01.25I


.5


.251010


o=4.0


102


o=4.5


1012


10-2100102


Time-dependent corrosion failures of bonding pads are plotted in Weibull form in Figure 4.15.


4.3.4 Lognormal versus Weibull


A comparative examination of Figures 4.11 and 4.14 reveals that the PDF,CDF, and failure rates of both of these important functions can be made to approximate one another by adjusting the respective parameters. If this is the case, then what are the distinctions among these distributions? Does it make a difference on which function is chosen to describe failure data?Which failure phenomena are best plotted in lognormal form? and Which are better described by a Weibull distribution? And ﬁnally, do these functions have any physical signiﬁcance? This last question, which underlies the previous three, is addressed separately in Section 4.5.


Which distribution to use for a given set of data is an important question in reliability modeling. Both lognormal and Weibull distributions outwardly appear to ﬁt most sets of data equally, as illustrated in Figure 4.16 0a203α


Figure 4.14 Plots of Weibull distribution functions. (a) f(t) versus time. (b) F(t) versus


time. (c) l(t) versus time. Time is measured in units of a. Variations in Weibull distributions are shown as a function of b.


The Mathematics of Failure and Reliability 205


β


(b) DISTRIBUTION FUNCTION F (t)


0.5-


TIME t4=β


2α3x0α


2α3α


(c)HAZARD FUNCTION λ(t)


3/α


β=4


2/Q


1/α


0.5 06TIME t 0


TIMEt


1.0卜


for the case of light bulb wear-out failures [3]. Closer examination, however, reveals that the Weibull distribution provides a better ﬁt to short time failures, while the lognormal plot is better at predicting longer lifetimes.


However, in this application long-time projections rather than infantmortality failures are usually of interest; thus a lognormal characterization of bulb life is preferred.


Lognormal distributions tend to apply when gradual degradation occurs over time because of diffusion effects, corrosion processes, and chemical reactions. Early p–n–p mesa transistors, bipolar and MOS transistors, lightemitting diodes (LEDs), and lasers are examples of devices whose failures have been modeled by lognormal statistics [18]. On the other hand,Weibull distributions appear to be applicable in cases where the weak link,or the ﬁrst of many ﬂaws, propagates to failure. Dielectric breakdown,capacitor failures, and fracture in ceramics are typically described by Weibull distributions.


Plotting failure data that ﬁt lognormal and Weibull distributions are facilitated with the use of special lognormal or Weibull graph paper because of the desired linear plots result. When predictions must be projected beyond the range of recorded failure data, the choice of the distribution function becomes important. A more advanced knowledge of statistics,


Figure 4.15 Weibull plot of bonding-pad corrosion failures. Increasing failure rate is indicated by the value of b ¼ 1.59. From Ref. [17].


probability theory, and failure physics may be required to make intelligent life projections in such cases.


If the data in Figure 4.16 were available for only a small population, say 10 test units, then the shape of the plot would be much in question and projections would be very problematic. This could be the case for a very expensive device made only in small quantities. Under such circumstances it would be very difﬁcult to determine an actual ﬁt to either lognormal or Weibull distributions. Further, if the device was required to exhibit high reliability and not be replaced, then the ﬁrst occurrence of failure would be paramount and its prevention essential to success of the program. In such cases analysis of each failure would be necessary, to determine root cause,before risk and probability of failure could be projected.


4.3.5 Plotting Probability Functions as Straight Lines


Virtually every reliability study concludes with some sort of linear plot of the number of failures versus time from which reliability parameters are derived. Just what constitutes the failed population, or a quantity equivalent to or proportional to it, depends on the particular failure phenomenon in question. The rate of current increase is such a measure for laser failures in Figure 4.12. Since a good linear ﬁt of failure time data is required, the question arises of how to make nonlinear reliability functions plot as straight


Figure 4.16 Light-bulb failure times plotted in terms of lognormal (a) and Weibull (b)distribution functions. From Ref. [13].


The Mathematics of Failure and Reliability 207


(a)e0.998 g


0.9898


0.98贸


0.95


S8:8


0.9


0.8、


0.7


0.4


0.3-Failure probability、


Failure probability0.02


I


0.01I


0.05. .0.02-0.01


0.003


0.005=


0.002亿


200 300 400500 700 9002000200Time (h)


300 400500 7009002000


T*7


0.001-x


0.05g


0.15


0.32


2(b)0.999


lines. Equivalently, How are Weibull and lognormal plot axes created, so that lines emerge while plotting failure-statistics data versus time? Reliability analysis is then essentially reduced to selecting the right plotting paper or computer program that generates it.


The problem of linearizing the Weibull function is easy because no complex functions are involved. Starting with Eqn (4.14) we note that taking successive logs of both sides yields


ln1 FðtÞ ¼ ðt=aÞb


(4.16)


lnf ln ½1 FðtÞg ¼ b ln ðtÞ  b lna:


(4.17)


The simple algebraic equation of a straight line is y ¼ mx þ b, where y is the ordinate, x is the abscissa, m is equal to the slope, and b represents the intercept on the ordinate axis. In comparison with Eqn (4.17), y ¼ ln {ln[1  (t)]}, x ¼ ln (t), m ¼ b, and b ¼ b ln a. Thus Weibull paper isgenerated by plotting ln {ln [1  F(t)]} or log {log [1  F(t)]} usuallyexpressed as cumulative percentage, versus either ln (t) or log (t), respectively. If the CDF or F(t) data that ranges from slightly above zero to slightly below 1.0 obeys Weibull statistics as a function of time, then a straight line will be obtained when plotted on this paper. It is not a difﬁcult matter to extract b and a values using standard algebraic methods.


In the case of the lognormal function, Eqn (4.11) suggests that a straight line results if ln (t) is plotted versus F1F(t); i.e., ln (t) ¼ m þ sF1F(t).From this plot a slope of s and an intercept equal to m are obtained. The slope can also be estimated from the literal deﬁnition


s ¼ ln t2  ln t1F1Fðt2Þ  F1Fðt1Þ :


(4.18)


This last expression simpliﬁes if points on the graph corresponding to F ¼ 50%, t50% and F ¼ 15.9%, t15.9% are selected. Letting F1 F(t2) ¼ F(0),and therefore F(t2) ¼ 0.5; similarly F1F(t1) ¼ 1.00 whenF(t1) ¼ F(1) ¼ 0.159. (Note Erf (z) ¼ Erf (z).) Substituting thesevalues yields the simple result s ¼ ln [t0.5/t0.159]. For example, in the case ofFigure 4.12, s ¼ 1.1.When failure data are abundant and there are many F values to plot,little difﬁculty in generating straight lines is experienced. However, what if there are few failures, so that obtaining a good estimate of statistical


parameters is problematical? Under these circumstances F can be obtained by ranking the exact failure times. For example, if the sample size is n, then 1/n is an estimate of F(t) for the ﬁrst ordered failure time, 2/n for the second failure time, etc. Thus, for the ith failure, F(ti) ¼ i/n. There is, however, arecommended way to estimate a statistically more accurate CDF or F value for the population [2], and that is by using Eqn (4.19); i.e.,


Fti ¼ i i-0.30:3nþ 0:4:


(4.19)To see how to use this formula, consider the following illustrative problem:


Example 4.3


A collection of 60 laser diodes were tested, and 7 failures occurred after 1000 h. The lifetimes obtained are tabulated below.


Rank number (i)


Lifetime (h)


F(ti) [ (i L 0.3)/(60 D 0.4)


|1 |181 |0.012 |(1.2%) |
|---|---|---|---|

|2 |299 |0.028 |(2.8%) |

|3 |389 |0.045 |(4.5%) |

|4 |430 |0.061 |(6.1%) |

|5 |535 |0.078 |(7.8%) |

|6 |610 |0.094 |(9.4%) |

|7 |805 |0.111 |(11.1%) |

1. Plot the results in both Weibull and lognormal fashion.


2. What is the MTTF for each?


3. For the lognormal plot, what is the value of s?


4. For the Weibull plot, what is a?


1. First, F(ti) is calculated for n ¼ 60 and i ¼ 1, 2, 3,., 7 and entered in the table.The F values are plotted versus log time on Weibull and lognormal paper as shown in Figure 4.17(a) and (b).


2. At a value of F ¼ 0.5, MTTF ¼ 2170 h (Weibull) and 3600 h (lognormal).3. It was shown above that s ¼ ln [t0.5/t0.159]. Substituting, s ¼ ln [3600/980] ¼ 1.30.4. From Eqn (4.16) we note that when t ¼ a, ln [1  F(t)] ¼ 1. Thus, 4. From Eqn (4.16) we note that when t = α, ln [1 - F(t)] = -1. Thus, 11 -F(t)=0.368, and F(t) =0.632. At this value, which is noted on the ordinateF(t) ¼ 0.368, and F(t) ¼ 0.632. At this value, which is noted on the ordinateaxis, a ¼ t ¼ 2990 h.


The Mathematics of Failure and Reliability 209


This example clearly shows the differences and difﬁculty in projecting failure rates with limited data, the normal situation for a working reliability engineer. Using the models as plotted we would project 99%failure at 7500 h for the Weibull and 75,000 h for the lognormal, quite a


0.0110


Figure 4.17 Laser diode failure times from Example 4.3 (a) plotted on Weibull probability paper and (b) plotted on Lognormal probability paper.


(a)0.98


0.85


0.632


0.55


0.45


0.35


0.17


0.12


0.05


0.03


|||||||10||||||||||||
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

difference! And maybe more important, for a mission critical application,which demanded very high reliability, the Weibull would predict a much shorter time to ﬁrst failure than the lognormal. The decision would be very difﬁcult and possibly require redundancy to ensure the execution of the mission.


Figure 4.17 dContinued


The Mathematics of Failure and Reliability 211


(b)0.999


0.001 10


4.3.6 Freak Behavior


Although it inspires conﬁdence to have failure data plot linearly on one of the probability papers, quite often this is not the case [19]. In Figure 4.18 such an S-shaped example of lognormal data is shown for CMOS integrated circuits,suggesting that two distinct failure mechanisms are operative. The observed plotwas decomposed into amain distribution operative at long times aswell as a“sport,” or freak, population that exhibits untimely failures at short times. Each component behavior in this plot is linear, and a superposition of the two weighted according to the individual relative proportions yields the observed bimodal failure behavior. While the sport population had a median time to failure ofw1.7 h, the value for the main distribution wasw180 h.


Freak failures are addressed again later in the chapter.


4.4 SYSTEM RELIABILITY


4.4.1 Introduction


Thus far we have dealt only with the reliability and statistical analysis of the failure of an individual device (e.g., transistor), component (capacitor), or constituent region within these (insulation). However, in practice, we


Figure 4.18 Lognormal lifetime data for CMOS ICs tested at 200 C consist of a main and a freak distribution. Roughly 75% of failures belong to the main distribution, which


has a median life of 180 h and s ¼ 1.20. The remaining 25% constitute the freakdistribution, with a median life of 1.7 h and s ¼ 0.78. Data from AT&T Bell Laboratories.


## 4.4 System Reliability


always use multidevice and multicomponent structures that are connected together and interact in complex ways within a system. How do we deal with reliability of the system as a whole? There is a large literature on the subject of system reliability [2,4,20]. We shall deal only with several relatively simple systems that build on our prior statistical experience with individual products. As has been the custom in this chapter, mathematical rigor will be sacriﬁced in an attempt to convey meanings and signiﬁcance.


Two rules are needed to calculate the reliability of the simplest types of systems [2]:


1. The multiplication rule states that the probability that several independent events will all occur is the product of the individual event probabilities.


2. The complement rule states that the probability that an event will not occur is one minus the probability of the event occurring.


Let us now consider the system shown in Figure 4.19(a) composed of n independent elements connected in series, or in a chain, such that system failure occurs when any one of the elements fails. If Ri(t) is the reliability or


Figure 4.19 (a) System composed of n independent elements with failure rate li connected in series. Note: n > i  1. (b) A parallel, or redundant, system of n com-ponents each with reliability Ri.


The Mathematics of Failure and Reliability 213


survival function of a given element, the overall system reliability, Rs(t), is given by the multiplication rule, or


RsðtÞ ¼ R1ðtÞ  R2ðtÞ  R3ðtÞ .RnðtÞ:


(4.20)In terms of the CDF formulation (Eqn (4.4)), the system unreliability is given by the complement rule, or


FsðtÞ ¼ 1Y


i¼1


ð1 FiðtÞÞ:


(4.21)


Since the hazard function l ¼ d[ln R(t)]/dt, the system failure rate, ls,is the sum of the individual failure rates,


ls ¼ l1 þ l2 þ l3 þ.þ ln:


(4.22)


This means that the reliability of a series system is always worse than that of the weakest component.


In contrast, the parallel, or redundant, system of n components(Figure 4.19(b)) continues to operate until the last unit fails. The corresponding functional relationships for Rs(t) and Fs(t) in a parallel system are


RsðtÞ ¼ 1Y


i¼11 RiðtÞ


(4.23)


FsðtÞ ¼ F1ðtÞ  F2ðtÞ  F3ðtÞ .FnðtÞ:


(4.24)


It can be shown [2] that if a single component with a CDF of F is replaced by n components, the ratio of the system to component failure rates is lowered by a factor equal to


li


ls¼


1þ F þ F2 þ F3 þ.Fn1nFn1:


(4.25)


The simple formulas given above illustrate that the reliability of individual units govern the life of the system in a bottom-up approach. In general, for a system of n elements whose individual reliabilities are known but whose interconnection conﬁgurations are unknown, the lower and upper bounds for system reliability are given by the series and parallel models, respectively.


Example 4.4


Consider a 50-pin module such that the probability of failure upon inserting it into a mating connector is 1.8  103% per pin. What is the probability of failure of themodule?


In this problem the module is the system (s), and the pins (p) are the elements. If we assume that a single pin failure causes the module to fail, then by Eqn (4.21), Fs ¼ 1 (1 Fp)n, where n is the number of pins per module. Substituting, Fp ¼ 1.8  105and n ¼ 50 yields Fs ¼ 1  (1  1.8  105)50 ¼ 0.00090.Therefore, the failure probability is predicted to be 0.09%, or 9 module failures in 10,000 insertions.


4.4.2 Redundancy in a Two-Laser System


Transoceanic cables for optical communications systems typically contain a hundred or so repeaters stretched across the ocean ﬂoor. Their function is to boost, or regenerate, the laser light signal, which attenuates with distance of transmission. Because of the enormous expense of submarine cable repair, redundant lasers are used in repeater systems to achieve the high reliability that is so critical in this application.


Redundancy, or the presence of spares that can be pressed into service should they be needed, is a common strategy used to achieve low system failure rates. In this section we consider the reliability of a regenerator that contains two lasers, one sparing the other, where each is assumed to fail according to lognormal statistics. Joyce and Anthony [12] considered two different models for the two-laser regenerator, and they are treated in turn.


4.4.2.1 Cold-Spared Assembly


In the so-called “cold-spared” assembly the second laser is called into service and begins to degrade after the ﬁrst laser fails. The duration of system survival depends on the ﬁrst component lasting until turn-on of the second, and the probability that the second will operate to time t. A plot of the cold spared failure rate, ls(c), is shown in Figure 4.20, and clearly resembles the Goldthwaite plot (Figure 4.13).


As an example, let us assume the lasers have a median lifetime of 100 years and s ¼ 1. After 10 years of system life, the abscissa of Figure 4.20is 1/10, in which case ls(c) (FITs)  t50 ¼ 3  105. Therefore,


The Mathematics of Failure and Reliability 215


ls 2s (c) = 3 x 105/8.76 x 105 = 0.34 FITs. With the passage of time the(c) ¼ 3  105/8.76  105 ¼ 0.34 FITs. With the passage of time theadvantages of redundancy diminish.


4.4.2.2 Hot-Spared (Parallel) Assembly


This assembly consists of lasers conﬁgured in parallel. Thus, lasers degrade concurrently, and the assembly fails if and only if both independent components fail. For this simpler case, the appropriate lognormal distribution and hazard functions of Eqns (4.11) and (4.12) apply. The hotspared failure rate (Eqn (4.25)) is simply ls (h) ¼ (2F/1 þ F) li; whenplotted, it is similar in appearance to that for ls (c).


Among the electrical products whose reliability MIL-HDBK-217 attempts to predict are microelectronic circuits including monolithic bipolar and MOS digital as well as linear gate logic arrays, microprocessors, MOS memories, GaAs MMICs, and assorted hybrid microcircuits. In these as well as other integrated circuits we are speaking of systems composed of thousands and even millions of identical transistor or gate units. The basic difference in the failure rate formulas for these systems, compared to individual devices (see Section 4.3.1.2), is that account is made of both the chip and package complexity. As a typical example, the predicted failure rate for an MOS gate array circuit can be calculated using the formula (p. 5–3 of MIL-HDBK-217)


lp ¼C1pT þ C2pEpQpL failures106h:


(4.26)Among the terms in this equation is the learning factor pL, discussed in Section 4.3.1.3. The constant C1 depends on the number of gates, which in turn is approximated by the number of transistors divided by 4. As expected, actual C1 values rise with gate count. Values of C2 reﬂect the complexity and type of package and are given by an expression of the type,


Figure 4.21 Plot of the ratio of the cold-spared to hot-spared failure rates, i.e., ls(c)/ls(h) versus time. From Ref. [12].


The Mathematics of Failure and Reliability 217


3=275E25


<J=6


-2.25-2 10-11.75 10211T1.5


1.25 10318332


10-4


0.5o =0.25


105


Failureλh Rate


10-6


10-410-310-210-1100101102 TIME t/MEDIAN LIFE tm


/Failure Rate λc


C2 ¼ k1ðNpÞk2. Np is the number of pins present, while k1 and k2are constants that depend on type of package employed, i.e., hermetic, dual in-line, ﬂatpack, cans, etc.


The shortcomings associated with MIL-HDBK-217 failure-rate modeling raised earlier persist when we are dealing with systems. Simply because of the added system complexity, one suspects that life predictions will be even more problematic than for individual devices.


4.5 ON THE PHYSICAL SIGNIFICANCE OF FAILURE


DISTRIBUTION FUNCTIONS


4.5.1 Introduction


A question raised earlier inquired whether the widely used failure distributions possess any physical signiﬁcance. If they do, is their mathematical form predictable? Thus far they appear to be a useful guide to plotting failure time data and predicting, through projection, what lies ahead.


However, they do not seem to have any link to the microscopic mechanisms that cause failure or to be rooted in physical terms. In the following sections an attempt is made to provide a physical rationale for the form of failure distribution functions. The effects of acceleration factors (AFs), the role of temperature, and how they are incorporated into the reliability functions are topics treated in the last of these sections.


4.5.2 The Weakest Link


Phenomena like the fracture of silica optical ﬁbers (Section 10.4) and dielectric breakdown of insulators (Section 6.3) are thought to originate at a fatal ﬂaw that grows with time. In the same way that a weak link threatens the integrity of a chain, so too defects of critical size will cause failure in electronic components. A simple derivation of the weakest link theory assumes that for the involved component of size L to survive under some condition of stressing, each of its differential elements dL must survive. In the case of the mechanical fracture of an optical ﬁber, L would be the length of ﬁber subjected to loading. If F is the probability of length L breaking, then 1  F is the probability of survival. Similarly, the survivalprobability of an inﬁnitesimal link is (1  dF) where dF is the probabilitythat length dL breaks. Thus we may equate the survival probability of length L to that of all of its constituent links, or


1 F ¼ ð1 dFÞL=dL:


(4.27)


## 4.5 On the Physical Significance of Failure Distribution Functions


Note the multiplicative nature of the survival probability, where the exponent is simply the number of differential links. By taking logs, this equation is simply recast into the form


F ¼ 1 expF = 1-expLdLIn (1-dF)}.ln1 dF:


(4.28)When  dF is small, expansion of In (1 - dF) yields -dF, and therefore,dF is small, expansion of ln (1  dF) yields dF, and therefore,F F=1 - exp {(L/dL(-dF)}, or.¼ 1  exp {(L/dL(dF)}, or.


F ¼ 1 expLdFF=1-expdL JdL:


(4.29)


We expect that dF/dL will physically depend on the applied stress s.


The dependence of F on L can be modeled in various ways, but it is common to assume a power law relationship, i.e., dF/dL ¼ 1/Lo (s/so)m,where Lo and m are constants. This leads to the expression F ¼ 1 exp{-t()"}F=1-exp LLossoLo Tm;


(4.30)


which has the Weibull form of Eqn (4.14) when s replaces time as the variable of interest. This equation is widely used in the reliability analysis of the strength of optical ﬁbers and ceramic materials.


In the case of dielectric breakdown the operative stress is the electricﬁeld E, and electrode areas (A) rather than lengths are relevant. Therefore,the failure probability for dielectrics as a function of E is predicted to have the form


F ¼ 1 expF=1-exp{(f)"}AAoEEon;


(4.31)


where n is a constant. Again it has the Weibull form in situations where E rather than time is the variable with a statistical spread. This equation will be referred again in Chapter 6.


4.5.3 The Weibull Distribution: Is There a Weak Link to the


Avrami Equation?


There is an interesting, and apparently unreported, connection between Weibull distributions and the Avrami equation of metallurgical literature fame. To see why, let us consider an initially defect-free matrix of volume Vo within a component that will eventually fail. With time, the


The Mathematics of Failure and Reliability 219


seeds of damage, e.g., precipitates, voids, charged traps, continuously germinate throughout the matrix with a constant nucleation rate _N (in units of number of nuclei/cm3  s). If a nucleus of damage (or defect)grows as a sphere from time t ¼ 0, then its volume is given byV ¼ 4pr3/3. Assuming that the sphere of radius r expands with constantgrowth velocity G, then at time t, r ¼ Gt; therefore, the volume isV ¼ 4p(Gt)3/3. Physically, damage nucleates at different times; if theevent occurs at time s, then the defect volume V 0 is given by V 0 ¼ 4pG3(t  s)3/3. The number of such damage defects formed perunit volume of undamaged matrix in time ds is _Nds. If the damage entities do not overlap, the total damaged volume V* is the sum of the defect volumes and is given by


V  ¼ SV 0 ¼ 4p3Z


VoG3 _Nðt  sÞds ¼ pVoG3 _Nt43: (4.32)The fractional volume that is damaged is F ¼ V*/Vo, or


F ¼ p3G3 _Nt4:


(4.33)


This equation applies only to short times or small F values. Later, however,the defective regions impinge on one another in much the same way that circular water wavelets do when raindrop nuclei randomly strike a pond and spread outward. Therefore, F stops increasing according to Eqn (4.33) and decreases with time as impingement of damaged regions occurs. Eventually, F levels off. Equation (4.34) accounts for both short- and long-time behavior:


FðtÞ ¼ 1 exphp3G3 _Nt4i:


(4.34)


At short times a Taylor expansion yields Eqn (4.33), while at long times F approaches 1.


Thiswell-known relationship is the celebratedAvrami equation. It has been used for well over a half century to describe the fractional amount of solid-state diffusional transformation of a matrix from which new phases nucleate and grow. A readable derivation and simple application of this equation is given in Ref. [21]. The most general form of the Avrami equation, valid for arbitrary defect geometries and failure processes, is commonly written as


FðtÞ ¼ 1 exp½ KðTÞtn;


(4.35)


and plotted in Figure 4.22. Here K(T) is a thermally activated, temperaturedependent constant (K(T) ¼ Ko exp [E/kT]), and n is a constant typicallyvarying between 1 and 4. In this form, constant K(T) has absorbed both timeand temperature-dependent nucleation and growth terms. One suspects that rapid damage growth follows a long period during which defects incubate;alternatively, failure nuclei can form readily, but subsequent growth of damage is sluggish. These behavioral extremes model nucleation- and growthcontrolled damage regimes, respectively. The critical question of what value of F is necessary for failure depends on the particular damage mechanism.


There are two publications on issues related to reliability that make use of an Avrami-like equation. The ﬁrst deals with void nucleation and growth damage during electromigration, an important reliability problem treated at length in Chapter 5. Resulting increases in resistance (R) with time were ﬁtted to an equation of the form exp [K(T)tn] [22]. A secondapplication, interestingly, involves modeling the time-dependent learning curve and yield improvement in processing integrated circuits. The theory developed involved an Avrami-like formula [23].


Comparison with Eqn (4.14) shows that F in Eqn (4.35) has exactly the same form as the Weibull CDF F; thus n ¼ b, and K(T) ¼ (1/a)b. Assuggested by Eqn (4.17), a plot of ln{ln[1  F(t)]} versus ln t yields a linewith a slope of n. There are other noteworthy similarities. For example, n,like b, is usually a small number, while K(T) like a, assumes a wide range of values.


Figure 4.22 Plot of Avrami equation as F(t) versus log t at different temperatures(T1 > T2 > T3).


The Mathematics of Failure and Reliability 221


4.5.4 Physics of the Lognormal Distribution


The lognormal distribution is characterized by a failure rate l(t) that has a single maximum, with l equal to zero at both zero and inﬁnite time. This is distinct from the Weibull distribution, which simply shows a monotonic increase with time. Electronic components have wear-out hazard functions that do not rise monotonically, and this partially accounts for the utility of the lognormal distribution. Physical models of failure generally invoke the central limit theorem (Section 4.2.1) to explain that speciﬁc energy levels Ei are nominally the same in all components and are distributed in a Gaussian fashion. Since degradation is directly related to the occupancy of such levels according to the Maxwell–Boltzmann factor, exp [Ei/kT], the logarithmyields Ei/kT, which is normally distributed; hence the lognormal distribution. Service environments of electronic products are relatively benign and vary little among populations. Since the spread in product life is primarily a function of manufacturing variability, it is possible to predict lifetimes on the basis of reliability testing.


In a speciﬁc application, Jordan [18] has discussed the aging degradation of GaP red LEDs in terms of diffusion and accumulation of point defects in the p–n junction region. Explicit expressions for the reduction of the electroluminescent efﬁciency were derived and had the form of the lognormal function.


There is an interesting inequivalence between the lognormal description of electronic components and the increasing hazard function for human lifetimes [3,12]. For living species, internal aging processes apparently generate species-speciﬁc biological clocks with increasing hazard functions as t / N. Furthermore, the presence of redundancy at many levels complicates the form of the hazard function. For example, loss of a kidney does not cause death in humans. In addition, random external variables,e.g., bacteria, viruses, accidents, addiction to cigarettes, alcohol, or drugs,become increasingly life-threatening as the recuperative powers of the body wear out. In contrast to electronic devices, the longevity of humans cannot be predicted with any accuracy through a physical examination.


4.5.5 Acceleration Factor


In recent years electronic devices and components have become very reliable, so that failure rates are now quite low when tested under ambient conditions. However, in order to make more meaningful lifetime projections, many failures, or data points, are required. This can be achieved experimentally through accelerated testing. Since many aging mechanisms


are governed by the Maxwell–Boltzmann factor, raising the temperature of the product under test is usually the most effective way to hasten failure.


The AF, an important term in the subject of reliability, was previously deﬁned as the ratio of the degradation or failure time at the use temperature T1 relative to that at an elevated, accelerated-test temperature T2. In using AF concepts it is assumed that the mechanism of damage does not change in the process. This caveat is an important one. After all, when a hen incubates eggs at room temperature, chicks will hatch; but if the process is accelerated in boiling water, hard boiled eggs result! True acceleration simply means speeding up the action without distorting it in any way. Essentially reproducing Eqn (1.10), the AF is given by.


AF ¼ Rate ðT2ÞRate ðT1Þ ¼MTTF ðT1ÞMTTF ðT2Þ ¼ exp[(-)],ER1T1 1T2; (4.36)


where the simple symbol E replaces the previously used DG* in all subsequent Arrhenius-type formulas. The activation energy (E) is normally positive, so that when T2 > T1, AF > 0. More complex expressions for AF arise when driving forces differ at T1 and T2, as noted in Eqn (1.11). For example,


AF ¼ expR(EE)ER1T1 1T2+c(2-n)},þ CV2  V1; (4.37)with C a constant, is commonly used to describe accelerated testing and burn-in under the combined inﬂuence of temperature and applied voltage V.


More generally, the question arises as to how to incorporate AF values obtained from accelerated testing under some set of stress-test conditions (s),into reliability functions that are valid under use conditions (u). In the sense used, stresses include temperature, voltage, current, and humidity, taken singly or in combination. True, or linear, acceleration factors apply when every test failure time and distribution function is multiplied by the same constant value to obtain projected results during use. Therefore,tf(u) ¼ AF  tf(s), and the PDF transforms tt(u) = AF x tf(s), and the PDF transforms asas


fuðtÞ fu(t)=(1/AF) xf(t/AF).¼ ð1=AFÞ  fsðt=AFÞ:


(4.38)


Similarly, formulas for the cumulative distribution and hazard functions transform as


FuðtÞ Fu(t) = (1/AF) x {AF x F(t/AF)} = Fe(t/AF)¼ ð1=AFÞ  fAF Fsðt=AFÞg ¼ Fsðt=AFÞ (4.39)


The Mathematics of Failure and Reliability 223


luðtÞ ¼ ð1=AFÞ x λs(t/AF), lsðt=AFÞ;


(4.40)


respectively. Substitution shows that there is no simple relation between the hazard function at use relative to test conditions for the lognormal case, but explicit formulas for the other two distributions are


Exponential lu ¼ ð1=AFÞ  Exponentialλu= (1/AF)xλs,ls;


(4.41)


Weibull luðtÞ ¼ ð1=AFÞb B xλs(t) lsðtÞ


(4.42)


Example 4.5


Tantalum capacitors were tested at elevated temperature, and the failure times were Weibull distributed with scale parameter a ¼ 2.5  105 h and a shape parameter b ¼ 0.5. Weibull distributed with scale parameter =2.5 x105 h and a shape parameter β= 0.5.IfIfthe AF is estimated to be 1  104, what is the probability that the capacitors will the AF is estimated to be 1 x 104, what is the probability that the capacitors will lastlast1 year?


The failure probability is given by FðtÞ ¼ 1 exphThe failure probability is given by F(t) =1- exp(AFxx)tAFabi. In 1 year there are 8760 h.


Therefore, F8760 ¼ 1 exp 1x104x2.5x105Therefore, F(8760) =1-exp{-[ 876011042:51051=2)]"}¼ 0:00187(. Thus the survivalprobability is equal to 1  F(8760) or probability is equal to 1 - F(8760) or 0.998.0.998.


4.5.6 The Arrhenius Model


Rooted in the very nature of atoms and molecules is their thermally activated response to increasing temperature expressed by the Maxwell–Boltzmann or Arrhenius factor (Eqn (1.2)). Because of the intimate linkage of reaction rates, failure times, and AFs, it is natural to incorporate the Arrhenius factor into the probability functions and their derived parameters. However, this involves more than a simple


substitution of exp长(六一/方)ER1T1 1T2for AF; while AF applies to only twotemperatures, the Arrhenius factor is more generally applicable to a range of temperatures.


The activation energy for degradation and damage processes at the atomic level critically affects the macroscopic MTTF through the formula


MTTF ¼ A expERT;


(4.43)


where A is a constant. A list of activation energies for common failure mechanisms in silicon devices is included in Table 4.4.


To illustrate how temperature inﬂuences failure times, consider the data of Figure 4.23(a), which are plotted in lognormal fashion. In obtaining the activation energy that characterizes these data, lifetimes are picked off the abscissa axis at the ordinate value corresponding to 50% cumulative failures.


These times (t50) are deﬁned as MTTF and are plotted in the Arrhenius manner, i.e., log MTTF versus 1/T(K), as shown in Figure 4.23(b). From the equation of the resulting straight line,


log MTTF ¼ log Aþ E=ð2:303RTÞ


(4.44)


the slope represents E/(2.303 R). Calculation yields a value of E ¼ 1.03 eV. Note that in this case the same activation energy wouldbe obtained when selecting times corresponding to other percentage cumulative failures (e.g., 10%), because the lines are parallel. When this is true it means that the same failure mechanism is probably operative at different temperatures and times.


The same procedure can be followed for Weibull data consisting of a set of parallel failure-distribution lines as a function of time, when plotted at different temperatures. As noted earlier in Eqn (4.17), the slopes yield the value for b; by then reading off times to reach a given Fusually F ¼ 12and plotting them versus 1/T in the Arrhenius manner, the activationenergy can be extracted.


Complications arise when cumulative failure distributions at different temperatures are not parallel to one another. This is what has occurred in Figure 4.24 where thin-ﬁlm dielectric breakdown data are plotted.


Outwardly, it appears that the activation energy is dependent on electricﬁeld. An admixture of failure mechanisms may be involved to account for the nonparallel failure distributions. In such cases, variations of Eyring-type relationships, which are considered next, may be more appropriate than the simple Arrhenius expression.


4.5.7 The Eyring Model


While the Arrhenius model is based solely on temperature stressing, the socalled “Eyring model” [25] takes into account the action of multiple


The Mathematics of Failure and Reliability 225


T a b l e  4.


T i m e-d e p e n d e n t  f a i l u r e  m e c h a n i s m s  i n  s i l i c o n  d e v i c e s


D e v i c e  a s s o c i a t i o n  F a i l u r e  m e c h a n i s m  R e l e v a n t  v a r i a b l e s


A c c e l e r a t i n g


f a c t o r s  A c t i v a t i o n  e n e r g y (e V)


S i O


a n d  S i-S i O


S u r f a c e  c h a r g e  M o b i l e  i o n s  V,


0 5


D i e l e c t r i c  b r e a k d o w n


T  E


0.


C h a r g e  i n j e c t i o n


3 (S l o w  t r a p p i n g)


M e t a l l i z a t i o n  E l e c t r o m i g r a t i o n


, g r a d i e n t s  o f


a n d


, g r a i n  s i z e


J


C o r r o s i o n (c h e m i c a l,


g a l v a n i c, e l e c t r o l y t i c)


C o n t a m i n a t i o n,


w


6 (f o r  e l e c t r o l y s i s


m a y  h a v e  t h r e s h o l d s)


C o n t a c t  d e g r a d a t i o n


, m e t a l s, i m p u r i t i e s


B o n d s  a n d  o t h e r


m e c h a n i c a l  i n t e r f a c e s


I n t e r m e t a l l i c  g r o w t h


, i m p u r i t i e s, b o n d


s t r e n g t h


I n  A l


A u


0 5  e V


F a t i g u e  B o n d  s t r e n g t h,


t e m p e r a t u r e  c y c l i n g


e x t r e m e s


M e t a l  p e n e t r a t i o n


h e r m e t i c i t y


A l u m i n u m  p e n e t r a t i o n


i n t o  S i  s e a l  l e a k s


The limits that bound this range of values on the high and low ends are known as conﬁdence limits. To be meaningful, reliability projections should be accompanied by a statement of the conﬁdence level. Statistical inference will not inform us of the fate of a particular specimen, but it could, for example, state that 97% of the components in a population will have an MTTF of 1500 h. When the population is very large, then its standard deviation will also serve for the specimen itself. There are standard mathematical techniques for evaluating conﬁdence limits, but a discussion of them would take us too far aﬁeld. For this information the reader is referred to the indicated Refs [3,4,39].


More relevant is what happens when very few failures are available for analysis. Does it mean that traditional reliability modeling is precluded?


The Mathematics of Failure and Reliability 233


Surprisingly, all is not lost! An approach is available to estimate an upper bound for the probability of failure and even to attach a level of conﬁdence to it. Following Nash [3,37], let us consider a subpopulation of N devices where n failures are seen in time t ¼ ta. The probability of such an outcomeis given by the binomial formula (Eqn (3.23)), now written in the form


Pðn; taÞ ¼ N !n!ðN  nÞ!FðtaÞn½1 FðtaÞNn:


(4.47)


In this equation F(ta) is the failure function or probability of failure in the time interval t ¼ 0 to t ¼ ta. In the extreme case where there are nofailures, n ¼ 0. Since F(t) ¼ 1  R(t) by Eqn (4.4),Pð0; taÞ ¼ RNðtaÞ;


(4.48)whereR is the reliability or survival function.Because,P(0, ta)þP(n> 1, ta)¼ 1by deﬁnition, it follows that the probability of 1 or more failures is given by Pðn  1; taÞ ¼ 1 RNðtaÞ:


(4.49)


The problem now reduces to selecting an appropriate functional form of R(ta). As we shall see, R(ta) will contain an undetermined parameter related to a characteristic lifetime. Since no failures were observed, a conservative bound on this characteristic lifetime will require that the chance of this occurrence be small. If, for example, P(n > 1, ta) ¼ 0.95 or 95%, then alower limit on the characteristic lifetime is such that the actual observation of zero failures is very unlikely, i.e., only 5%. A conﬁdence level C(0), for the case of no failure, is deﬁned to be


Cð0Þ ¼ Pðn  1; taÞ:


(4.50)


This value of C(0) is a known quantity that we impose in the analysis.


In what follows, expressions for the failure rate will be developed for two different failure models. In the case that failures are described by a Weibull function,


RðtÞ ¼ exph ðt=sÞbi;


(4.51)


the characteristic lifetime, s, is used in place of a (see Eqn (4.14)). When no failures occur in testing N components for a time ta, then


Cð0Þ ¼ 1 exphNðta=sÞbi:


(4.52)


Suppose we wish to calculate the hazard rate at a speciﬁc time, say 1 h.


Then by Eqn (4.15),


l1 λ1=BT-B.¼ bsb:


(4.53)


It is usually desired to include temperature effects, so that inclusion of the AF (Eqn (4.42)), coupled with elimination of s between the last two equations, yields the following expression for the failure rate at use temperature Tu.


l1ðTuÞ ¼ b ln½1=ð1 Cð0ÞÞNðAFtaÞbβln[1/(1-C(0))]:


(4.54)


Example 4.6


Suppose that ICs are used in a critical application at 40 C. The manufacturer selects Suppose that ICs are used in a critical application at 40 C. The manufacturer selects aa sample population of 1000 chips, ages them at 150 C for 2 years (ta ¼ 1.75  104 h) sample population of 1000 chips, ages them at 150 °C for 2 years (ta = 1.75 x 104 h) andandno failures are observed. Typical data for other similar products suggest that the activation energy for failure is 0.4 eV and b ¼ 0.25. What upper bound value for the failure rate, l1(40 (40 °C), can be predicted with a confidence of 90% (C = 0.9)?C), can be predicted with a conﬁdence of 90% (C ¼ 0.9)?


First the AF is evaluated from Eqn (4.36): AF ¼ exp8.62x10-5h0:48:621050.4(33-423)]1313 1423i¼ 47:2. Aftersubstituting in Eqn (4.54), l1ðTuÞ ¼ 103x(47.2x1.75x104)0.25=1.91 x10-5 /h or 19,094 FITs0:25 ln 1ð10:9Þ103ð47:21:75104Þ0:25 ¼ 1:91 105=h or 19,094 FITs Compared to the decreasing hazard rate of the Weibull model, the use of the exponential distribution is easily derived. Under conditions where no failures are observed during testing, l(t) ¼ l1(Tu) ¼ const, and it is easily shown that.


l 2 = (N.AF·ta)-1 x In[1/(1 -C(0))].¼ ðN$AF$taÞ1  ln11 Cð0Þ:


(4.55)


Using the same data above in Example 4.6, the assumption of an exponential distribution would result in l ¼ 2.7 FITs, quite a difference.


4.6.3 Risky Reliability Modeling


Making reliability estimates is often fraught with pitfalls, as the following example illustrates [40]. In a hypothetical but realistic scenario, suppose that GaAs high-electron mobility transistors (HEMTs) are needed for a state-ofthe-art communications satellite that costs $100,000,000. The desired life is 25 years, and failure of even a single transistor will degrade the performance of the satellite. Engineers at the company contracted to design, manufacture, test, and specify the reliability of the HEMTs conduct a testing


The Mathematics of Failure and Reliability 235


program involving accelerated aging of the devices under bias. Ten transistors were tested at each of four aging temperatures, 225, 234, 240, and 260 C, and the MTTF were found to be 980, 380, 190 and 33 h,respectively, as depicted in the plot of Figure 4.26. Signiﬁcantly, there were no infant-mortality failures. Longer time tests at lower temperatures were planned, but an answer was needed as soon as possible, and it was based on these four data points.


Employing the familiar relation MTTF z exp [E/(RT)] (Eqn (4.43)),an Arrhenius plot (Figure 4.27) of the failure times versus 1/T(K) yields an activation energy (E) for failure of 2.2 eV. Projecting the 225 C data to the use temperature results in MTTFð298 KÞ ¼ MTTFð498 KÞexp h2:28:621051498 1298ior 1.18  1015 MTTF(498 K); this is equivalent toan AF of over 1015. It means that the predicted life at 25 C is 1.2  1018 h 1:3 1014years, or equivalently, more than 5  1012 desired lifetimes.Based on this calculation the overjoyed engineers enthusiastically endorsedthe reliability of these transistors. But, can this predicted life, which is some 30,000 times the age of the earth, be believed? After all, Evans [42]has commented that “Acceleration factors of 10 are not unreasonable.


Factors much larger than that tend to be ﬁgments of the imagination and


Figure 4.26 Failure of high-electron mobility transistor transistors as a function of time. Data reported by Ref. [41].


of lots of correct, but irrelevant, arithmetic.” If so, is there a more reasonable approach to this problem?


One difﬁculty with the analysis is the assumption that elevatedtemperature data can be simply extrapolated to the use temperature.


Making an w200 C extrapolation is risky for semiconductor devices and requires caution; accelerated aging should preferably be done closer to the use temperatures, if possible. What if a change in failure mechanism having a smaller activation energy occurred at these lower temperatures? To check such a possibility, it would have been a good idea to estimate the activation energy (E) that would be required to give a 25 year (2.19  105 h) life. Under the above assumptions,E ¼ 8:62105ð1=2981=498Þ ln2:191050:98103¼ 0:34 eV. The decrease in activation energyfrom 2.2 to 0.34 eV is perhaps fortuitous, but signiﬁcant because the latter value is characteristic for infant mortality failures of many semiconductor products, as indicated in Section 4.5.9. In fact, as Figures 4.26 and 4.27 reveal, longer-time testing of these HEMTs at three lower temperatures indicated failures with an activation energy of 0.60 eV.


Figure 4.27 Arrhenius plot of the failure times versus 1/T (K). High temperature data yield an activation energy for failure of 2.2 eV. Low temperature data yield an activation energy for failure of 0.60 eV.


The Mathematics of Failure and Reliability 237


It is instructive to view graphically what happens to the hazard rate when two failure populations, a largemain and small freak, are exhibited, as shown in Figure 4.28. At elevated temperatures both failure behaviors merge into what appears to be a main (bimodal) distribution. However, at lower temperatures these distributions diverge according to their respective activation energies.


Now the freak population poses a particular threat at low temperatures.


A similar methodology for early-life reliability prediction in integrated circuits was advanced in a recent publication [44]. It was suggested that early failures are not intrinsic, but rather premature or infant failures.


Therefore, the common practice of extrapolating intrinsic life-test distributions to estimate early-life reliability is incorrect and often leads to unduly optimistic predictions. This all underscores the necessity for screening weak products, some of which may have the potential to cause freak failures.


4.6.4 Freak Failures


The subject of freak failures is perhaps the most difﬁcult topic addressed in reliability. Valuable insights into this problem have been provided byNash [3].


Assuring reliability against freak phenomena is open-ended and unstructured because statistically insigniﬁcant numbers of freak failures occur. In order to design strategies against freak failures it is instructive toﬁrst distinguish between the normal and freak products of manufacture. The reliability of normal products has the following characteristics:


Figure 4.28 Schematic depiction of failure rate distribution consisting of large main and small freak populations. At low temperatures the two populations diverge, with freak failures occurring at short times. After Ref. [43].


1. Failure mechanisms are few in number, e.g., dielectric breakdown,electromigration, etc.


2. Thesemechanisms are distributed among the entire populationof products.


3. Failures are independent of lot number or time of manufacture.


4. The normal or statistical variability of manufacturing processes gives rise to the defects that cause normal failures.


5. Normal failure mechanisms are characterized by well-known activation energies and AFs. Product lifetimes are therefore statistically predictable.


6. Importantly, normal products do not fail prematurely. Screening prior to shipment generally weeds out the weak products that would have failed by the normal failure mechanisms.


Abnormal or freak failures, on the other hand, differ from normal failures in all respects. Speciﬁcally, they have the following characteristics:


1. There are many causes and mechanisms of freak failures. Each one is different and occurs with low frequency. Thus freak failures cannot be statistically modeled. If they could, they would cease to be freak and become normal failures.


2. Freak failures are found only in small subsets of the overall population of products.


3. Such failures are dependent on lot as well as time of manufacture.


4. Failure times are often very short and frequently unrelated to operating times. Freak failures are not wear-out failures!


5. In contrast to normal failures, there are very few studies of freak failures in the literature.


Two observations of failures summarize the distinction between normal and abnormal products. Normal products do not fail under anticipated use conditions; ﬁeld failures are of the freak variety.


4.6.5 Minimizing Freak Failures


Is there any hope for a workable strategy to deal with abnormal products?Before answering the question it is helpful to better understand what are thought to be the sources of freak failures. These include:


1. Random one-of-a-kind accidents (e.g., electrostatic discharge or electrical overstress due to mishandling).


2. Manufacturing processes that are poorly controlled (e.g., particulate contamination) or prone to yield low-quality results.


3. Changes in the quality or properties of raw materials used (e.g., due to new suppliers).


The Mathematics of Failure and Reliability 239


Based on the last two considerations, the remedies required to minimize the possibility of freak failures are those that continuously improve product quality. Speciﬁc measures to improve products for high-reliability applications include:


1. Additional and stricter testing to identify and eliminate products that exhibit signs of being in the least atypical. Tighter pass-fail limits, aging at higher temperatures and bias voltages, and more stages of inspection represent some of the new quality hurdles that should be instituted.


2. Laboratory analysis of each and every service failure to establish fundamental causes of failure. Such information should result in corrective redesign and manufacturing changes aimed at improving the product.


3. Implementation of more robust designs with higher safety margins.


4. Rejection of products that have been reworked.


5. Institution of traceability to pinpoint faulty processes and identify suspected lots.


6. Stricter supplier monitoring.


The remainder of this book is primarily concerned with normal failures because virtually the entire reliability physics literature is concerned with them. Unfortunately, this same literature offers little insight into the uncharted territory of freak failures; we therefore travel the more comfortable and well illuminated paths of normal behavior.


4.7 A SKEPTICAL AND IRREVERENT SUMMARY


Now that rather elaborate statistical methods have been presented to analyze degradation and failure data, we may ask how correct and reliable the conclusions are. Skepticism about statistics being able to justify any particular point of view is not solely limited to the social sciences; examples were given in the chapter questioning the validity of the predictions made. I am not the only one to raise such doubts, but rather have humbly followed more eloquent analysts and critics of reliability methodology and its philosophical underpinnings. One such critic is R.A.


Evans, an editorial writer for the IEEE Transactions on Reliability, whose column appears in each issue. In these often memorable editorials, many issues related to reliability, statistics, and improving product quality are addressed in a witty and perceptive manner. Several excerpts from this column will give the reader a sense of his concerns and provide a perspective on this chapter.


## 4.7 A Skeptical and Irreverent Summary


STATISTICS AND IGNORANCE


We spend too much time in our reliability courses on probability and statistical inference . that show us how to quantify our ignorance. We do not spend enough time on removing that ignorance . the engineering, physics and chemistry of why things fail and why things don’t fail.


from Vol. 39, p. 257, Aug. 1990


SUPERSTITION, WITCHCRAFT, PREDICTION


The title is a parallel to Disraeli’s phrase, “Lies, Damned Lies, and Statistics”. . A main use of engineering reliability prediction is for the marketplace. That is, a customer wants to know the reliability of a product, before buying the product.


The vagaries of such numbers (predictions for the marketplace) leads to the infamous numbers games.


from Vol. 37, p. 257, Aug. 1988


STATISTICS VERSUS PHYSICS


Statistics describes only populations, not individuals. In particular, the hazard rate(failure rate) of a population does not say anything at all about the behavior of an individual. . An individual part is likely to degrade with time, and thus get worse as time goes by; it can do that and still be a member of a constanthazard-rate population. . Reliability-statistics is not physics; don’t ever confuse them. . The quality and reliability disciplines use statistics as a last resort. If we were smarter about the world, we wouldn’t have to.


from Vol. 38, p. 273, Aug. 1989


WHERE DO I BEGIN?


. you are placed in charge of creating a cost-effective reliability program . tell me what I should do? . Most corrective action will be a combination of management and engineering changes. Some will require scientiﬁc advances. A very few will require mathematical advances. Very rarely will mathematical statistics be a bottleneck, although some statistical principles are always important. . Don’t get a bunch of experts to come and lecture everyone on reliability statistics.


from Vol. 38, p. 513, Dec. 1989


RELIABILITY PREDICTION AND MIL-HDBK-217


One should use MIL-HDBK-217, not because it is so great, but in spite of its weaknesses. When it is used like any other engineering tool, it can be a great help.


If it is confused with holy writ, then there is no end of trouble. The search for certainty often ends up in the acceptance of superstition.


from Vol. 37, p. 257, Aug 1988


The Mathematics of Failure and Reliability 241


## Statistics and Ignorance


## Superstition, Witchcraft, Prediction


## Statistics versus Physics


## Where Do I Begin?


## Reliability Prediction and MIL-HDBK-217


4.8 EPILOGUEdFINAL COMMENT


Catastrophic failure, device degradation, and AFs are some of the most important and the most difﬁcult aspects of working as a reliability engineer.


The AF for a given test depends on test parameters, samples, and stress conditions. If we ﬁrst take a thermally activated mechanism, we will necessarily assume a Maxwell–Boltzmann thermal activation for the rate of degradation. But the degradation may not always be outright catastrophic failure. The degradation may be a % change in some parameter, say threshold voltage or resistance, such that the circuit is slower than it needs to be. A case in point, which is counter intuitive comes up with hot electron induced threshold voltage shift of MOSFETs. The threshold voltage shift is less at higher temperature because it slowly anneals above room temperature. This gives the appearance that it is inverse with temperature. This comes about because the observation is a competition of two separate effects. First, the hot electrons are generated in the channel and some of them surmount the barrier at the oxide interface and are trapped in the gate oxide at the drain end of the channel. Second, the electrons trapped in the gate oxide anneal out as they are released from the traps in the gate oxide. The annealing effect is thermally activated and causes less observed shift at higher temperatures. The complexity of this effect is further complicated by the generation of hot electrons which also increases with applied drain voltage and shorter channel length, both of which increase the electric ﬁeld, which is the driving force producing the hot electrons. In order to determine an AF, one must ﬁrst determine how much threshold voltage shift will constitute failure. This shift is usually called an end of life shift. The trick is to put this end of life shift in the context of the mean and standard deviation of the expected values of the threshold voltage values expected in a chip and a wafer. Notice we are talking about the tail of the onset of failure, which although not early life failure, is somewhat like early life failure. Chip failure will be determined by the MOSFET device which is the closest to the end of life value. Six sigma will bear quite heavily on our decision as to whether a process is well controlled or not,both from a yield and a reliability standpoint. In very sophisticated designs one may even have to consider the duty cycle of the device to come to aﬁnal decision. Such considerations often lead to design groundrules for dimensions and guidelines for maximum currents and voltages in devices.


Violation of these rules will result in premature failure. However the rules are design, process and technology dependent, which is another way of


## 4.8 Epilogue-Final Comment


saying they are dependent upon the company making the chip, and even possibly the organization within the company.


4.1 Calculate the mean and standard deviation for the fuse data listed in


Table 4.1. What percentage of the measurements fall within the interval between m  s and m þ s? How does this percentage comparewith the predicted area under a normal distribution curve?


4.2 During the cyclic stress or fatigue testing of a large number of solder


joints, the following failures were recorded in the indicated intervals.


Calculate the failure rates per cycle and plot the results as a function of the number of cycles in order to obtain a “bathtub” curve.


4.3 A failure mechanism that follows the exponential distribution function


will not beneﬁt from burn-in. Why?


4.4 “Grandfather’s clock . stood ninety years on the ﬂoor . but it


stopped short, never to go again when the old man died (at exactly


90).” Even more reliable was “The Deacon’s Masterpiece,” the


wonderful one-horse shay that lasted “one hundred years and a


day.” Each of these fabled marvels of American craftsmanship had a


reliability of unity until failure, at which time it became zero. Assuming


Weibull statistics can be applied in these cases, calculate the characteristic lifetimes (a) and shape parameters (b) in each case.


Number of cycles


Percentage of failed joints


during given interval of testing


0e50


1.21


50e100


100e150


0.13


150e200


0.62


200e250


0.36


250e300


300e350


4.51


350e400


6.73


400e450


3.24


450e500


13.2


500e600


4.65


600e700


8.58


700e800


2.24


The Mathematics of Failure and Reliability 243


4.5 The extreme value distribution (due to Gummel) has a probability


density function given by f(t) ¼ (1/b) exp [(t  s)/b] exp (exp[(t  s)/b]), where b and s are constants. What are the mathematicalforms of F(t) and l(t)?


4.6 Demonstrate the explicit relationship connecting F(t) and l(t), namely,


FðtÞ ¼ 1 exp"Z t0lðtÞdt#:


4.7 A LED has a MTTF of 250,000 h.


a. Based on the exponential distribution, predict the probability of failure within a year.


b. At what time would half of the devices fail?


c. Suppose failures are modeled with a lognormal distribution function with a standard deviation s ¼ 1.5. What is the probability ofLED failure in one year?


4.8 Fifteen 75-W light bulbs were tested for 1000 h, and the failure times


in hours were 890; 808; 501; 760; 490; 658; 832; 743; 993; 812; 378;


576; 899; 910; 959.


a. What is the MTTF?


b. Assuming constant failure-rate modeling. What is the reliability after 400 and after 800 h?


4.9 The failure fraction of a laser transmitter is 3% over a period of


25 years. Express the hazard rate in FITs.


4.10 Certain device failures obey lognormal statistics with s ¼ 4.5.a. What is the maximum value of the normalized failure rate and at what normalized time does it occur?


b. How long does it take to reach a maximum failure rate of 10 FITs?


4.11 a. Provided that lognormal behavior is obeyed, what minimum median lifetime (t50) is required for devices to function 40 years and suffer only 100 FITs if s ¼ 1.0?


b. What maximum standard deviation should be targeted if no more than 10 FITs can be tolerated in devices with a median lifetime of 1  108 h?


4.12 A reliability engineer using the MIL-HDBK-217 calculates a failure


rate of 225 FITs for a particular device using exponential distribution


function statistics.


a. What is the CDF for 20 years of operation?


b. As a result of accelerated testing it was found that wear-out phenomena were governed by Weibull failure functions. The Weibull parameters were a ¼ 5  106 h, b ¼ 3. What is thepredicted CDF after 20 years?


4.13 A bathtub curve consists of three linear regions as a function of


time (t), namely,


1. an infant mortality failure rate that decreases as l(t) ¼ C1  C2t;2. a zero random failure rate;


3. a wear-out region that varies as C3(t  to).a. Sketch the bathtub curve.


b. Calculate f(t) and F(t) values in each of the three regions.


4.14 The Rayleigh distribution is deﬁned by a single parameter k, and the


hazard rate increases linearly with time such that l ¼ kt. From thisinformation calculate f(t) and F(t) for Rayleigh distributions. What


is the connection between the Rayleigh and Weibull distribution


functions?


The Mathematics of Failure and Reliability 231


Finally, there is the wear-out failure regime. Here components degrade at an accelerated pace, so the failure rate increases in this region. This is the regime where lognormal and Weibull statistics enjoy a dominant role.


A manufacturing goal for high-reliability components is to extend the life of components prior to the onset of wear out. Remarkable strides have been made in this direction. It should be noted that while experimental failure data for some devices and components may reﬂect the entire shape of the bathtub curve, this is not true of the mathematical distribution functions. These distributions ﬁt only one or, at most, two regions of the curve reasonably well.


What has been said thus far about the bathtub curve is the traditional wisdom. For more than a decade this view has been disputed in criticism to the effect that “the bathtub does not hold water any more” [34] and “the roller coaster curve is in” [32]. Very low infant mortality failure rates of devices nowadays is the basis for the former observation, while the latter characterization is due to the sometimes-observed short time hump in the hazard rate. Thus l(t), which starts high initially, falls to a local minimum (a valley) and then rises up and over a hump to ﬁnally merge with ﬂatter portions of the curve, as suggested in Figure 4.25(b). As far back as 1968,Peck [35] attributed the humps to what he called “freak” failures and suggested that they could be eliminated by stress screening such as burn-in.


Later, Peck [36] discerned a considerable lengthening of the infant mortality region for integrated circuits to times approaching 100,000 h. After that, the hazard rate apparently meets the main failure distribution. At this stage it becomes an academic question; devices do not actually fail but become obsolete due to design changes and introduction of new technology.


Note l(t) for a system on a chip with 108 transistors is possibly an admixture of a few of the mechanisms in Table 4.4, all competing or behaving to give a low or high reliability, respectively. Rarely do all chips fail due to one and only one failure mechanism. If they do then it is quite possibly wear out, and the root cause of failure may not have been determined or removed from the design and fabrication process.


4.6 PREDICTION CONFIDENCE AND ASSESSING RISK


4.6.1 Introduction


Thus far we have been been blessed with a generous amount of failure data to enable us to readily perform statistical analyses of the kind discussed in this Chapter Indeed, much of the electronics reliability physics literature is


## 4.6 Prediction Confidence and Assessing Risk


devoted to accelerated testing that generates such data in abundance. In practice, however, there are many important situations where there are very few, if any, failures. Military systems, nuclear reactors, airport trafﬁc control systems, undersea communication links, and surgical electronic equipment spring tomind as examples where catastrophemay result from a single failure.


In such cases, how are statistical predictions of failure made, and how conﬁdent canwe be of reliability estimates?What dowedowhen zero failures are seen in laboratory failure-testing experiments? Questions involving statistically insigniﬁcant numbers of failures, and the risks involved in drawing conclusions from them, are addressed in this section [37].


Measurement error associated with the statistical counting of % failure is fairly straight forward and essentially a discrete parameter. For example, 1 fail in 10, 10%. An analogue parameter such as temperature or threshold voltage has an error associated with the technique of measurement and the accuracy and precision of the device used for themeasurement. The interested reader is referred to Yardley Beers [38], “Theory of Error” for a thorough and complete discussion of experimental error. A careful analysis of the data generated by any experiment must be a prerequisite to what follows below.


4.6.2 Conﬁdence Limits


The degree of conﬁdence we have in the estimates of m, s, a, b, l, or any other statistical quantity mentioned in this chapter is dependent on the number of samples tested and quantity of data, as well as on the measurement error of the statistic under consideration. Since the average value for a speciﬁc sample will differ from the true value of the population, the latter should be quoted to lie within a range in which we have conﬁdence.


4.15 A missile guidance system contains 100 transistors each of which is


99.9% reliable. The failure of any transistor will cause the guidance


system to fail. How reliable is the guidance system? Suppose there


are 1000 transistors. What is the system reliability?


4.16 For a particular telephone IC circuit pack, Weibull infant mortality


failure rates are characterized by l(t) ¼ 34,100 t0.728 FITs.a. If the failure rate at the end of a year is 25 FITs, calculate the percentage of devices failing during the ﬁrst 6 months.


b. Suppose the circuit pack contained 250 such components. How many would fail after 6 months?


4.17 A communications system consists of a transmitter, a receiver, and an


encoder such that the failure of any of these components will cause


failure of the system. If the individual reliabilities are 0.93, 0.99,


and 0.95, respectively, what is the system reliability?


a. If the exponential distribution governs failure in each of the components, what is the system failure rate?


4.18 Consider a control system that contains subsystems having the


following reliability characteristics.


Central processing unit


Weibull b ¼ 1.05, a ¼ 100 h


I/O card


Exponential 1/lo ¼ 750 h


Actuator


Lognormal m ¼ 6.4, s ¼ 1.5


The Mathematics of Failure and Reliability 245


It is necessary for all subsystems to function for the system to operate.


What is the reliability of the system at 300 h? From Ref. [45]


4.19 Sketch what happens to the bathtub curve if


a. component dimensions shrink further.


b. devices are powered under successively higher current–voltage stressing.


4.20 Consider the bathtub curve for humans. Specify examples of the


causes of death that are operative in each of the three time domains.


4.21 A 16-position connector is subjected to ﬁve different degradation


mechanisms. The reliability for each mechanism is Ri(i ¼ 15).a. Write an expression for the overall reliability R of the connector.


b. If the Ri are all equal to Ro, what is value of R?


c. What contact reliability is required to produce a connector reliability of 0.9999?


4.22 In a population of photodiodes, 20% display freak (f) failures at a


MTTF of 12,000 h, while the main (m) population has an MTTF


of 28,000 h.


a. Sketch the probability density function, f(t), for this population if they are normal distributions.


b. Suppose s(f) > 2s(m). What is the ratio of the peak values of f(t),i.e., ff(t)/fm(t)?


4.23 In GaAs transistors were tested at 180, 196, and 210 C, and the times


to failure in hours were:


180 C: 250, 420, 1000, 1300, 1300, 1300, 1300, 1500, 1500, 1600


196 C: 190, 200, 330, 330, 400, 400, 420, 600, 800


210 C: 105, 110, 120, 130, 210, 230, 290, 300, 320, 400


a. What are the MTTF at each temperature if the data follow lognormal statistics?


b. What is the activation energy for failure?


c. What is the mean life at 110 C?


4.24 While testing a 10,000 FIT device, 23 failures were observed within


the ﬁrst hour of burn-in. What was the total number of devices in the


burn-in lot?


4.25 The overall reaction rate that leads to failure of a component is the


result of two mechanisms having different activation energies, E1


and E2. In failure mode A these mechanisms occur in series (sequentially), while for failure mode B they add in parallel. Sketch the overall reaction rate versus temperature in the form of an Arrhenius plot


for both failure modes. What are the reliability implications of the thermal dependencies of these two failure modes with respect to predicting low-temperature failure?


[1] M.G. Pecht, F.R. Nash, Proc. IEEE 82 (1994) 992.


[2] P.A. Tobias, D.C. Trindade, Applied Reliability, Van Nostrand Reinhold, New York,


[3] F.R. Nash, Estimating Device Reliability: Assessment of Credibility, Kluwer


Academic, Boston, 1993.


[4] P.D.T. O’Connor, Practical Reliability Engineering, second ed., Wiley, Chichester,


[5] R.A. Evans, Tutorial notes, in: Annual Reliability and Maintainability Symposium,


1994.


[6] P.E. Fieler, Tutorial notes, in: IEEE International Reliability Physics Symposium, 2.1,


1990.


[7] E.E. Lewis, Introduction to Reliability Engineering, second ed., Addison Wesley


Publishing, 1996.


[8] J.A. Carr, Electron. Technol. J.


[9] K.L. Wong, Qual. Reliab. Eng. Int. 7 (1991) 489.


[10] J.A. McLinn, Qual. Reliab. Eng. Int. 6 (1990) 237.


[11] S.F. Morris, J.F. Reilly. Proc. Ann. Reliability and Maintainability Symposium, 1993,


p. 503.


[12] W.B. Joyce, P.J. Anthony, IEEE Trans. Reliab. 37 (1988) 299.


[13] F.R. Nash, Estimating Device Reliability: Assessment of Credibility, Kluwer


[14] L.R. Goldthwaite, in: Proc. 7th National Symposium on Reliability and Quality


Control in Electronics, 1961, p. 208.


[15] L.R. Goldthwaite, Proceedings of the Seventh National Symposium on Reliability and


Quality Control in Electronics, 1961, p. 208.


[16] W.J. Bertram, in: S.M. Sze (Ed.), VLSI Technology, second. ed., McGraw Hill, New


York, 1988.


[17] K.D. Hong, S.S. Lee, J.Y. Kim, S. Daniel, C.K. Yoon, 33rd Annual Proceedings of the


IEEE Reliability Physics Symposium, 1995, p. 85.


[18] A.S. Jordan, Microelectron. Reliab. 18 (1978) 267.


[19] D.S. Peck, in: 9th Annual Proceedings of the IEEE Reliability Physics Symposium,


1971, p. 69.


[20] R. Ramakumar, Engineering ReliabilitydFundamentals and Applications, Prentice


Hall, Englewood Cliffs, NJ, 1993.


[21] K.N. Tu, J.W. Mayer, L.C. Feldman, Electronic Thin Film Science for Electrical


Engineers and Materials Scientists, Macmillan, New York, 1992.


[22] K.P. Rodbell, M.V. Rodriguez, P.J. Ficalora, J. Appl. Phys. 61 (1987) 2844.


[23] W. Hillberg, Microelectron. Reliab. 20 (1980) 337.


[24] W.J. Bertram, in: S.M. Sze (Ed.), VLSI Technology, second ed., McGraw Hill, New


[25] H. Eyring, S.H. Lin, S.M. Lin, Basic Chemical Kinetics, J. Wiley, New York, 1980.


[26] J.S. Suehle, P. Chaparala, C. Messick, W.M. Miller, K.C. Boyko, 32nd Annual Proceedings of the IEEE Reliability Physics Symposium, 1994, p. 120.


[27] E.B. Hakim, Solid State Tech. 33 (8) (1990) 57.


The Mathematics of Failure and Reliability 247


[28] P.D.T. O’Connor, Solid State Tech. 33 (8) (1990) 59.


[29] M. Pecht, P. Lall, E.B. Hakim, Qual. Reliab. Eng. Int. 8 (1992) 165.


[30] H.S. Blanks, Qual. Reliab. Eng. Int. 6 (1990) 259.


[31] D.J. Klinger, Y. Nakada, M.A. Menendez, AT&T Reliability Manual, Van Nostrand


Reinhold, 1990.


[32] K.L. Wong, Qual. Reliab. Eng. Int. 5 (1989) 29.


[33] D.S. Peck, in: 16th Annual Proceedings of the IEEE Reliability Physics Symposium,


1978, p. 1. F.S. Beltramo. Proceedings of the Annual Reliability and Maintainability


Symposium, vol. 327, 1988.


[34] K.L. Wong, Qual. Reliab. Eng. Int. 4 (1988) 279.


[35] D.S. Peck, in: 6th Annual Proceedings of the IEEE Reliability Physics Symposium,


1968.


[36] D.S. Peck, Trans. Electron. Devices 26 (1979) 38.


[37] F.R. Nash, in: Materials Research Society Symposium Proceedings, vol. 184, 3, 1990.


[38] Yardley Beers, Introduction to the Theory of Error, Addison Wesley Publishing, 1957.


[39] G.W.A. Dummer, N.B. Grifﬁn, Electronics ReliabilitydCalculation and Design,


Pergamon Press, Oxford, 1966.


[40] F.R. Nash, Seminar at Stevens Institute, September 27, 1995.


[41] A. Christou, in: A. Christou (Ed.), Reliability of Gallium Arsenide MMICs, Wiley,


[42] R.A. Evans, IEEE Trans. Reliab. 40 (1991) 497.


[43] F.R. Nash, Lucent Technologies, Bell Laboratories Innovations.


[44] S.S. Menon, K.F. Poole, Microelectron. Reliab. 35 (1147) (1995).


[45] T.D. Thomas, P.B. Lawler, in: Electronic Materials Handbook, vol. 1 Packaging, ASM


International, Materials Park, Ohio, 1989, p. 899.


CHAPTER 5


Mass Transport-Induced Failure


5.1 INTRODUCTION


The preceding chapters have introduced the devices, processing defects,and yields of electronic products that will now see service. Chapter 4 prepared us to expect product failures and provided mathematical tools that enable future performance to be predicted. From now until the end of Chapter 10, we shall be primarily concerned with the detailed microscopic mechanisms that cause these products to degrade in use. We have already noted (Section 1.3.1) that virtually all failures in electronic materials and devices are the result of the physical movement of atoms or charge carriers from benign locations associated with normal behavior to other sites where they contribute to creating or enlarging defects that lead to component malfunction. Because solids are often not in thermodynamic equilibrium,atoms feel compelled to move or react. Thus, silicon and aluminum should theoretically revert to SiO2 and Al2O3 in air at room temperature, while dopants at junctions should intermix in response to thermodynamic imperatives. But fortunately, for the most part, these and other scenarios for change and reaction in chemically unstable materials, interfaces, and structures do not occur. The low operating temperatures involved essentially reduce reaction rates to negligible levels. Nevertheless, there are other material combinations and forces present that do pose threats to reliability because the chemical and physical changes they induce are on a scale comparable to device or component feature dimensions.


In this chapter we primarily deal with phenomena attributable to atomic diffusional motion on the chip level. This should be distinguished from other transport effects treated elsewhere, i.e., electron (Chapter 6), ionic(Chapter 7), and stress-induced ﬂow of solder (Chapter 9). Effects of atomic diffusion include compound formation, precipitation reactions, void formation, alloying, contact and interconnect reactions, and general degradation of the metallization. Related examples involve environmentally induced ion migration during corrosion and the permeation of water through plastic packages.


http://dx.doi.org/10.1016/B978-0-12-088574-9.00005-7


All rights reserved. 249


It is a primary objective of this chapter to predict the time dependence of the visible manifestations of failure based on the mass transport models that describe them. Metals are the major culprits associated with mass transport-induced reliability problems at both chip and packaging levels.


Degradation and failure phenomena due to interdiffusion, compound formation, electromigration (EM), and contact reactions are some of the effects modeled in this chapter.


5.2 DIFFUSION AND ATOM MOVEMENTS IN SOLIDS


5.2.1 Mathematics of Diffusion


Diffusion is deﬁned as the migration of atoms (or molecules) in a matrix under the inﬂuence of a concentration-gradient driving force. Through sequential motion of countless numbers of atoms, each jumping from site to site, an observable macroscopic change in atomic concentration, C, results.


In most cases the diffusing and matrix atoms differ, but they may be the same, as during EM in Al conductors. Fick’s law, the phenomenological equation that deﬁnes diffusion, is written as


Jm ¼ DdC=dx:


(5.1)


Concentration gradients (dC/dx) in the positive x direction cause transport of a mass ﬂux of atoms (Jm) in the negative x direction, signifying that the vectors deﬁning these terms are oppositely directed; hence the negative sign. Flux units mirror those of concentration. For C in atoms/cm3 or g/cm3, the corresponding units of Jm are atoms/cm2-s or g/cm2-s.


Irrespective of concentration units, values of D, the diffusion coefﬁcient or diffusivity, are always expressed in units of (distance)2/time, i.e., cm2/s. The diffusion coefﬁcient, a measure of the extent of mass transport, depends on a number of factors, including the nature of the diffusing atoms and matrix,the speciﬁc transport path (i.e., lattice, grain boundary (GB), dislocation,surface, interstitial, etc.), temperature, and the concentration of the diffusing species. Temperature, the most important factor inﬂuencing D, was already noted in Eqns (5.1)–(5.3), while dopant concentration effects in semiconductors were sketched in Section 3.2.2.1.


During nonsteady-state diffusion, more atoms enter a region of the matrix than leave, and therefore, their concentration builds in time(dC/dt> 0). This is normally the case in a homogeneous matrix. But there are situations where more atoms leave a region than enter it. In time, this loss of matter (dC/dt< 0) leads to mass depletion or even voids that can


adversely affect reliability. Such effects may occur at interfaces between different phases, or when the matrix is heterogeneous and contains numerous GBs and structural defects. In either case, nonsteady-state diffusion can be accounted for by equating the negative divergence of the mass ﬂux (i.e., –V Jm) to dC/dt. When proper account is taken the mass flux (i.e., -V x Jm) to dC/dt. When proper account is taken ofofinstantaneous mass conservation at each value of x, the equation governing diffusion in one dimension is


vCðx; tÞvt¼ Dv2Cx; tvx2


(5.2)


if D is constant.


There is a simple solution to this equation when diffusion occurs in a semi-inﬁnite matrix, and atoms are supplied at the x¼ 0 boundary from aninexhaustible or continuous surface source of concentration Cs. Further, it is assumed that the initial concentration in the matrix is Co, or constant throughout, and remains Co at inﬁnite distance. These initial and boundary conditions may be written as C(x, t¼ 0)¼Co, C(x¼ 0, t)¼Cs(Cs¼ constant), and C(x ¼N, t)¼Co. Employing standard boundary-value methods for solving partial differential equations, the solution to Eqn (5.2) is


½Cðx; tÞ  Co=½Cs  Co ¼ Erfchx=ð4DtÞ1=2i[C(x,t)- Co]/[Cx- Co] = Erfc[x/(4Dt)1/2].: (5.3)Known as the complementary error function, Erfc [x/(4Dt)1/2] is mathematically deﬁned as


Erfc½x=ð4DtÞ1=2 ¼ 1 2Erfc[x/(4Dt)1/2]=1-p1=2Z exp-22dz.


x 2ðDtÞ1=2


exp z2dz: (5.4)


An even simpler solution to Eqn (5.2) results if a ﬁnite or instantaneous rather than continuous surface concentration S (in units of atoms/cm2) is involved. The Gaussian solution has the form


Cðx; tÞ ¼ SðpDtÞ1=2exp x24Dt


(5.5)


For example, if dopant atoms diffuse into a Si wafer, the amount left on the surface decreases with time; i.e., at x¼ 0, C(0, t)¼ S/(pDt)1/2.Graphic solutions for continuous and ﬁnite-source concentration proﬁles


Mass Transport-Induced Failure 251


are shown in Figure 5.1. Like trigonometric functions, values for the complementary error function and Gaussian are tabulated as a function of the argument [x/(4Dt)1/2] in mathematical references and texts on statistics. These same functions are used in the probability and reliability mathematics of Chapter 4.


When back-of-the-envelope estimates for the extent of diffusional penetration are sought, the equation


x2 ¼ 4Dt;


(5.6)based on the practical implications of Eqns (5.4) and (5.5), serves rather well.


5.2.2 Diffusion Coefﬁcients and Microstructure


Together with Eqn (5.6), the other important thing to remember about diffusion is that the diffusivity is thermally activated (Eqns (5.1)–(5.3)). In the expression for diffusivity, both Do and ED are dependent on the nature of the diffusant and matrix, and the speciﬁc path taken by the atoms (see section 5.2.1). Thus for diffusion through grains of a polycrystalline matrix, atoms can either exchange places with matrix atoms (vacancies), hop within the conﬁnes of a dislocation core, migrate along GBs, or skip along the surface. Short-circuit atom transport via the latter three paths requires successively less energy expenditure than for


Figure 5.1 Sequence of concentration proﬁles at different diffusion times. (a)Continuous (constant) source at surface yields complementary error function solutions.


(b) Instantaneous (ﬁnite) source at surface yields Gaussian solutions. As the time quadruples from t1 to t2 (t2¼ 4t1), the diffusional penetration distance doubles from x1to x2.


CsCs-COC(x,t)-Co=Erfc (x/√4Dt)Concentration, C


t3>t2>t1


t1t2t3


t2


X1 X2


Distance, x


Co


Concentration,C合」


VπDt C(x,t) =S exp - (x2/4Dt)


motion through the bulk. The reason is due to a correspondingly less conﬁning atomic environment that presents fewer physical obstacles to diffusion. These ideas have been quantitatively conﬁrmed in facecentered cubic metals. The following expressions typically describe the diffusivity of atoms along the indicated paths [1]. To obtain these values it is assumed that both the GB width and dislocation radius are


0.5 nm in size.


Lattice or bulk diffusion DL ¼ 0:5 exp 17:0TM=T cm2=s (5.7a)


Dislocation Dd ¼ 0:7 exp 12:5TM=T cm2=s (5.7b)


Grain boundary DGB ¼ 0:3 exp 8:9TM=T cm2=s (5.7c)


Surface Ds ¼ 0:014 exp 6:5TM=T cm2=s (5.7d)Note should be taken of the different activation energies for each diffusion mechanism. Thus bulk, dislocation, GB, and surface diffusion mechanisms have activation energies that vary as 17.0 RTM, 12.5 RTM,


8.9 RTM, and 6.54 RTM, respectively, where TM is the melting point and R is the gas constant.


The regimes of dominant diffusion mechanisms are outlined in Figure 5.2 as a function of grain size (l) and dislocation density (rd)for different temperatures. This diffusion map is the outcome of allowing the various transport processes to freely compete, where the lines represent the conditions for equal mass ﬂuxes from neighboring regime mechanisms. Although strictly intended for self-diffusion, we shall assume that the map applies to impurity diffusion as well. In the thin-ﬁlm regime (shown dotted) at low temperatures, GB diffusion dominates, and therefore GB diffusion coefﬁcients must be used for the purposes of calculation. Even if driving forces other than concentration gradients are operative, microscopic atomic migration occurs along these same paths.


Effective diffusivity values vary as a function of grain size, necessitating some sort of averaging of the individual contributions from lattice and GB mechanisms. An effective diffusivity, Deff¼DL þ fDGB has beensuggested, where f is the fraction of atoms in short-circuit paths.


A measure of f is the ratio of the GB thickness to grain diameter. In general, grain size variations will correspondingly cause differing diffusivities.


Mass Transport-Induced Failure 253


5.3 BINARY DIFFUSION AND COMPOUND FORMATION


5.3.1 Interdiffusion and the Phase Diagram


Many reliability problems stem from interdiffusion effects at the interface between two dissimilar materials e.g., solder joint, semiconductor contact.


To better understand the nature of reaction, let us consider a couple consisting of two elements A and B, in contact at a planar interface. What will happen if the couple is now heated to temperature To, where diffusion of atoms normally occurs? The answer depends on the nature of A and B, their grain structures, and the magnitude of the involved diffusivities. A good-ﬁrst step is to look at the phase diagram for A and B.


Among the possible reactions are those shown in Figure 5.3, where solid solution (Figure 5.3(a)) and eutectic (Figure 5.3(b)) behaviors are depicted.


Below each of these, typical interdiffusion proﬁles are depicted(Figure 5.3(c) and (d)) at To and time t. These representations emphasize the connection between phase-concentration distributions and phase diagram-imposed solubility limits. For complete solid solution systems


Figure 5.2 Regimes of dominant diffusion mechanism in FCC metals as a function of grain size ([) and dislocation density (pd) at different temperatures. From Ref. [2].


(e.g., Ge–Si), phases can theoretically assume any binary composition. But in eutectic systems (e.g., Pb–Sn), interdiffusion occurs only up to the solubility limit, resulting in the formation of a range of terminal solid solutions.


Concentration proﬁles in real systems are generally not error-functionlike or symmetric across the couple interface, because the diffusivity usually depends on composition and hence position. The rather involved graphic Boltzmann–Matano analysis can yield values for the overall diffusivity,D(C), in such couples, provided that the diffusional proﬁles are known [3].


For many solid solutions (e.g., Cu–Ni, In–Pb) the ﬁrst of the two Darken equations (the second is Eqn (5.11)) yields the (chemical) diffusivity in the couple, namely,


DðCÞ ¼ CADðBÞ þ CBDðAÞ


(5.8)


This equation suggests that a kind of weighted average of individual diffusivities D(A) and D(B) determines the magnitude of D(C). In turn, the resulting nonlinear diffusion equation


Figure 5.3 Schematic solid solution (a) and eutectic (b) phase diagrams for A and B


components. Interdiffusion proﬁles at temperature To (dotted) corresponding to solid solution (c) and eutectic (d) phase diagrams.


Mass Transport-Induced Failure 255


vCðx; tÞvt¼ vvxDðCÞ vCðx; tÞvx;


yields complex diffusion proﬁles.


5.3.2 Compound Formation


Many interdiffusion-related reliability problems are due to compound formation effects at solder–metal interfaces or semiconductor contacts.


These applications will be addressed in later sections, e.g., 8.3.3.3 and 5.4,but the underlying roles of phase diagrams, transport mechanisms, and kinetics are considered here. Compound-forming systems generally have more complex phase diagrams than those we have been considering. An idealized version is shown in Figure 5.4, where the resulting concentration proﬁle across a couple composed of components A and B is also indicated.


The growth kinetics of the (AB) compound phase is of particular interest.


Atoms from both a and b phases must be transported to the interface for the compound to thicken. Conservation of mass requires that the two shaded areas on the a-phase side be equal, and similarly on the b-phase side.


Figure 5.4 Depiction of intermediate compound (g) formation arising from reaction between components A and B. The reaction temperature is dotted in on phase


diagram.


Analysis [1] shows that reaction at the a/g interface results in compound growth kinetics given by


Xa ¼DaðCA  CaÞ2ðCa  CgÞCgt1=2:


(5.9)


A similar expression holds for the b/g interface, and therefore the ﬁnal compound layer thickness, the sum of both, is expected to grow parabolically in time i.e.,


Xg ¼ constexpECRTt1=2:


(5.10)


Parabolic, thermally activated growth with activation energy EC should come as no surprise when Eqn (5.10) is compared with Eqn (5.6), which expresses the fundamental connection among variables for diffusional processes.


Examples of parabolic growth occur during the elevated-temperature diffusion-controlled oxidation of many metals (e.g., Al, Cu) and the formation of intermetallic compounds and metal silicides. When the oxides are adherent to the base metal, parabolic growth dominates, but this is not so when the oxide is porous and ﬂakes off. In such a case oxygen (or the metal)does not have to diffuse through the oxide; it can directly access the metal surface from the gas phase and form oxide through direct chemical reaction.


Such reaction-controlled oxidation frequently occurs only for short times in continuous or protective oxides (e.g., SiO2) but persists indeﬁnitely in nonprotective (porous) oxides (e.g., MgO). Reaction-controlled growth is characterized by linear, rather than parabolic, kinetics. Other time dependencies have also been observed during oxidation.


5.3.3 The Kirkendall Effect


In this section we address the implications of a binary alloy system whose individual components have different diffusivities. Let us consider a diffusion couple composed of equal volumes of A and B bonded across a planar interface that contains a row of minute, inert markers as shown in Figure 5.5(a). For simplicity, the A–B solid solution system of Figure 5.3(a)is assumed. Suppose A-vacancy exchanges are less prevalent than those between B atoms and vacancies. Therefore, in a given time less A is transported to the right (Figure 5.5(b)) than B to the left (Figure 5.5(c)). If the couple suffers no volume change, then the marker has effectively shifted


Mass Transport-Induced Failure 257


to the right (Figure 5.5(d) and (e)). This effect is known as the Kirkendall effect, and it dispelled early notions that both atoms in an alloy interdiffused at the same rate. The second Darken equation predicts that the effective velocity (v) of the marker-plane motion is


v ¼ ðDA DBÞ dCAdx;


(5.11)


where the concentration gradient is evaluated at the interface [3].


Figure 5.5 (a) Illustration of Kirkendall effect in a diffusion couple composed of A and B components bonded across a planar interface containing a row of small, inert markers. (b) Diffusion of A atoms to the right. (c) Diffusion of B atoms to the left. (d)Final position of marker, which effectively shifts to the right (e) if the couple suffers no volume change.


Not only is there an effective interfacial migration, but the possibility also exists that voids may form. To see why, we note that the difference between the large ﬂux of B atoms and the smaller counterﬂux of A atoms must be equal to the ﬂux of vacancies. The basic diffusion equation (Eqn (5.2)), derived by setting the negative divergence of the mass ﬂux equal to the time rate of change of concentration, also applies to vacancies. Therefore, there will tend to be a vacancy buildup on the B side balanced by a corresponding depletion on the A side. When a critical vacancy supersaturation develops, there is always the possibility that they may condense into voids. The big question, of course, is what level of vacancy supersaturation is critical. This depends on generally unknown vacancy trapping and emission probabilities, void/matrix interfacial properties, and local driving forces. There is scarcely a more alarming occurrence for reliability prospects than void or incipient crack formation, but this is just what happens in the Al–Au contact system considered next.


5.3.4 The Purple Plague


This colorful term refers to the purple AuAl2 intermetallic phase formed when Al and Au reacts. The compound was known for at least 70 years before it surfaced as a reliability concern in wire bonds to transistors and hybrid ICs some 45 years ago. Various bonding conﬁgurations are susceptible to purple-plague formation and the damage associated with it. These include Au wires or wedges bonded to thin-ﬁlm pads of Al on Si, Al wires attached to an Au-plated ﬁlm on Si or a contact post, and Au wire/Au balls bonded under heat and pressure (thermal compression) to Al ﬁlms. At elevated temperatures and long times the AuAl2 compound forms in the reaction zone, and the bond fails as a result of annular microcrack formation.


The Al–Au phase diagram reveals the existence of ﬁve intermetallic compounds. Each of the bond types above can be modeled by a planar diffusion couple between the involved elements. But depending on the relative initial metal thicknesses (d), different ﬁnal phase mixtures result if equilibrium is attained. For example, when dAl> dAu, then the formation of AuAl2 and excess Al is predicted. Similarly, in an excess of Au, the AlAu4 compound will eventually form. In these as well as other Al–Au combinations, some AuAl2 will also form. What is so alarming about its presence is the Kirkendall porosity that accompanies it (Figure 5.6). Since voids form on the Au side of the interface, Au apparently migrates more


Mass Transport-Induced Failure 259


rapidly than Al; a fact conﬁrmed independently in the diffusion literature.


Figure 5.16 (a) Experiment demonstrating stress effects during electromigration in short conductors. (b) Scanning electron micrographs of gold stripe powered at 106 A/cm2. Cathode end at left is depleted of gold, while anode end at right contains hillock growths. From Ref. [20].


Mass Transport-Induced Failure 279


that counters the primary EM ﬂux. Under these conditions, the two masstransport driving forces balance, or


ZqE ¼ Udsdx:


(5.27)


Substituting, ds/dx z sc/Lc and Ec¼ rje(c), where critical values are denoted by c, the result that emerges is


LcjeðcÞ ¼ UscZqr:


(5.28)


Signiﬁcantly, the shorter the stripe length, the larger the current density required to sustain electrotransport. This effect must be accounted for during lifetime testing because otherwise-unduly pessimistic life predictions may result for short stripes.


Later, in Section 5.7, the role of stress in voiding phenomena, a reliability problem of current concern, will be explored.


5.5.5 Structural Models for EM Damage


5.5.5.1 Electromigration in Grain Boundaries


Thus far we have tacitly assumed that powered interconnects have a homogeneous structure. But we know that the grain structure of thin ﬁlms can vary widely depending on deposition conditions and that structure has a profound effect on EM damage. Powered single-crystal Al stripes, for example, have been shown to exhibit virtually “inﬁnite” life. The primary reason for this is that diffusion and drift of atoms in GBs far exceeds transport through the bulk of the grains. In fact, the activation energy for the former is only about half that of the latter (compare Eqn 5.7(a) and (c)).


At low temperatures, in particular, it is an excellent assumption to view the stripe as an interconnected GB network and neglect mass transport everywhere except within the network channels. Thus, ﬁne-grained ﬁlms have many channels, or paths, for atomic migration, while coarse-grainedﬁlms have many fewer such avenues for transport.


5.5.5.2 Structural Barriers


Interfaces between adjoining regions of an interconnect where properties differ may be regarded as structural barriers. The difference can be very large or barely perceptible; it can take the form of variations in grain orientation, grain size, or differences in chemical composition, such as at a contact between the metallization and semiconductor. In addition,


differences in atomic diffusivity, effective valence and vacancy generation,and trapping characteristics can serve as barriers capable of creating local mass-ﬂux divergences. Furthermore, the situation is not static. With EM-induced heating, boundaries may move, grains may recrystallize,and subtle structural and chemical evolution may occur in the conductor.


To appreciate structural barriers, consider what happens when a ﬁnegrained stripe segment abuts one of larger grain size. For one direction of current ﬂow, atoms that migrate readily through numerous GBs suddenly come upon a region with a dearth of GB paths that lead away. Such a barrier results in a pileup of matter. Similarly, void formation can be expected in regions where more atoms leave than enter. It is not difﬁcult to model what might be expected at the barrier interface (x¼ 0) betweenstripe region 1, extending from x¼ –N to x¼ 0, and adjoining region 2,ranging from x¼ 0 to x¼N [21]. Suppose differing vacancy GB diffu-sivities, effective valences, current densities, resistivities, vacancy lifetimes(s1,s2), temperatures, etc., distinguish each region. Under isothermal conditions, and neglecting stress or other effects that inﬂuence vacancy motion.


vCi


vt¼ 02 (DZ*qpje0C Gio-GDi0x2v2Civx2DZqrjeRTivCvxþ Cio  Cisi; (5.29)where i¼ 1, 2, C is the vacancy concentration, and Co is the equilibriumvacancy concentration. The ﬁrst two terms on the right express the diffusional and ﬁeld-driven mass contributions; only the last term is unfamiliar and represents the vacancy generation (or annihilation) rate. Steady-state conditions typically prevail within minutes, so vCi=vt can be safely dropped. Imposing the conditions of a continuous concentration (C1¼C2)and ﬂux vC1/vx¼ vC2/vx at x¼ 0 enables C to be calculated at the inter-face. The results of a sample calculation for the vacancy supersaturation S(S ¼ (C –Co)/Co) versus distance are shown in Figure 5.17 for the casewhere grain sizes (d1, d2) differ across the interface.


Although a vacancy supersaturation (or subsaturation) may be predicted, the crucial question is whether it is sufﬁcient to cause nucleation of voids (or growths). This is a very complicated issue that depends on the chemical and physical nature of the heterogeneous void nucleation site.


Unfortunately, it is not known with any certainty what level of vacancy supersaturation is required to generate damage. The problem of void nucleation and its time dependence during EM has been addressed [22]employing concepts of classical or capillarity theory. A signiﬁcant feature


Mass Transport-Induced Failure 281


of the analysis is the prediction of a void incubation time that has, in effect,been observed [23].


With increasingly shrinking interconnect stripe widths, broad-area or blanket metallizations leave greater numbers of GB “triple points” and grains lined up in a bamboo-like structure after patterning. The conﬂuence of three GBs at a triple point is schematically depicted in Figure 5.18(a), and shown in a portion of the Al interconnect reproduced in Figure 5.18(b).


Divergences in mass transport can occur, assuming that migrating atoms are solely conﬁned to GB channels. It is apparent that when fewer atoms leave the triple point than enter it, a mass accumulation is favored. But, when more atoms leave the triple point than enter it, voids form. Less EM damage is anticipated when fewer GBs are oriented parallel to the axis of current ﬂow. Thus we may expect conductor life to sequentially increase as grains change from a bimodal size distribution to small, large, near-bamboo and hyperbamboo, structures.


Figure 5.17 Calculated vacancy supersaturation at the interface between regions with a grain-size discontinuity. This condition is mathematically approximated by a difference in number of GB transport paths within the two regions. Note: x is the vacancy sink distance ðx ¼ ð2DsÞ1=2Þ, je¼ 1 106 A/cm2 and T¼ 400 K. From Ref. [21].


Figure 5.18 (a) Schematic of grain-boundary triple point conﬁguration. When the electron current polarity is reversed, the electromigration damage in the form of mass accumulation and voids at triple points also reverses. (From Ref. [21]). (b) Actual triple point grain conﬁgurations in an aluminum interconnect (800 nm wide, 400 nm thick)imaged by focused ion beam (FIB) microscopy. Courtesy of D. Barr, Lucent Technologies,Bell Laboratories Innovations.


Mass Transport-Induced Failure 283


δ


Jell


II


θI


III OII


丁


2d


JeIII


VOID


5.5.5.3 GB Grooving


As another example of a structural barrier that may generate void damage we consider the phenomenon of GB grooving [24]. In Figure 5.19(a) the crosssection of a ﬁlm at a junction between two grains is shown. Although such a structure may be stable for all practical purposes, it is, nevertheless, not in


'y(x,t)


x


YsYs


Vb


W


FILM


→+0∞


SUBSTRATE


(b)Js


JS


X=0


X


子


JGB


Je


thermodynamic equilibrium. The reason is that the surface (gs) and GB (gb)


Figure 5.19 (a) Initial ﬁlm proﬁle is shown dotted. Asymmetric grain-boundary grooving as a result of electromigration. (From Ref. [24].) (b) Schematic of electromigration-induced vacancy ﬂux at grain-boundary triple point. The electromigration-induced surface ion ﬂux (JS) compensates for the vacancy ﬂux(JV¼ –JGB) to preserve the dihedral angle. (From Ref. [21].)


interfacial tensions are not mechanically balanced in the vertical direction. But,through thermal GB grooving processes as a result of mass transport, equilibrium between the involved tensions is achieved such that 2 gs sin q¼ gb. If aunidirectional surface ﬂux of atoms now ﬂows past the junction as a result of EM, mechanical equilibrium at the groove is upset. As atoms preferentially accumulate on one side of the boundary, an asymmetry inﬁlm height develops and the dihedral angle sharpens. In order to reestablish equilibrium the groove widens and deepens. In the next instant of time the equilibrium is upset again,and so on. This perpetual drive to equilibrium punctuated by intermediate moments of instability ultimately causes the groove to reach the substrate where a void or open circuit is produced. Such amechanism occurs at any level of vacancy supersaturation, in contrast to the damage model presented in Section 5.5.5.2. Analytical expressions for the kinetics of grooving and surface topography of the grains have been published.


Finally, we may consider grooving to cause damage at a GB triple point by an EM-induced vacancy ﬂux, as shown in Figure 5.19(b). This case has been modeled [21], and the length (y) of the GB hole produced as a function of time (t) is given by


yðtÞ ¼ MðBtÞ3=4ﬃﬃﬃ2pG74 ;


(5.30)


where M¼CbdDbZ*qE/2nsDsUgs, B ¼Db gs nsU2/kT, and G is thegamma function. In these expressions b refers to the GB, s to the surface;vs is the effective surface ion concentration, and U is the atomic volume.


Times calculated to produce damage are of the order of tens of hours for reasonable choices of the involved constants.


5.6 EM IN PRACTICE


5.6.1 Manifestations of EM Damage


All powered metals in ICs are potentially susceptible to EM effects. Interconnects, contacts, and vias are the three locations that are particularly prone to damage. Much of Section 5.5 was devoted to degradation and failure in interconnections; this discussion is by no means over and will continue. We start by discussing EM-damage manifestations in contacts and vias.


5.6.1.1 EM at Contacts


Large mass divergences are expected at powered contacts because any metal that leaves the semiconductor interface cannot be replenished. The subject


Mass Transport-Induced Failure 285


of diffusional degradation at contacts in both Si and GaAs devices was treated earlier. However, in the presence of simultaneous EM, the damage accelerates. Ondrusek et al. [25] have studied the wear-out of both Al–Si and TiSi2–Si contacts and found the latter to be considerably less susceptible to EM degradation. For the case of Al–Si contacts, previously introduced in Section 5.4.2 in connection with junction spiking, the following was observed:


1. Current-induced migration of Si through Al–1%Si metallization results in contact failure having activation energy of 0.9 eV.


2. Either accumulations or depletions of Si in the contact window occur depending on the direction of current ﬂow. Electron ﬂow into the contact causes a Si buildup at the contact; when the polarity of current ﬂow is reversed, Si is driven into the Al–1%Si metallization. These effects are shown respectively in Figure 5.20.


3. Large reverse-bias p – n junction leakage currents occur during Si depletion and the contact resistance increases when Si accumulates.


4. The mean time for contact failure depends on current density as MTTFz jne ; n is found to range from 5 to 11 as the current increases.


In contrast, the failure activation energy was 1.1 eV for the Si accumulation mode of failure in TiSi2–Si contacts. However, for the depletion mode of failure the activation energy was 1.5 eV. Similar beneﬁcial life extensions occur with the use of TaSi2 contacts to Si [26]. Activation energies for EM failures ranged from 1.1 to 1.4eV, suggesting damage and open circuiting in the matrix rather than GBs of the Al. Transition to a high-resistance, nonohmic state is a manifestation of failure.


EM damage is not limited solely to silicon devices but occurs in compound semiconductors as well. High-power, broad-band MMICs are


Figure 5.20 Accumulation- and depletion-mode contact failures caused by silicon electromigration are dependent on direction of electron ﬂow. Depletion-mode failures occur by aluminum spiking. From Ref. [25].


susceptible under conditions of accelerated testing. Failure analysis of these devices reveals that EM of the AuCr ohmic contact metallization occurs in the manner schematically depicted in Figure 5.11(c).


5.6.1.2 EM at Vias


It has already been noted (Section 2.9.8) that IC architecture makes extensive use of successive interconnect levels and vias that enable current to ﬂow between levels. Typical structures employ Al–Cu vias sandwiched between Al–Cu interconnects, but for higher reliability, tungsten plug vias are employed. In addition, thin diffusion-barrier ﬁlms of TiN are frequently used to line vias. While the Al metallization tends to migrate, or “walk” off the via, W exhibits negligible diffusion or transport. Therefore, like contacts, via–interconnect interfaces are sites of potentially large mass divergences where Al depletion due to EM cannot be replaced. By carrying the shunted current when the Al has migrated, the TiN layer plays an important role in forestalling failure.


Degradation at vias is not only dependent on the composition and grain structure of the metals employed and the uniformity of ﬁlm coverage, but also on the direction of current ﬂow. Several models for EM damage at vias are shown in Figure 5.21 illustrating the numerous opportunities for mass divergence at contact interfaces within the complex via–conductor geometry [27,28]. Simple electrotransport of Al leaves voids at the bottom(Figure 5.21(a)) and top (Figure 5.21(b)) plug interfaces when electronsﬂow into or away from them. In addition, thinned metal conductors in the via sidewalls (Figure 5.21(c)) and corners induce current crowding and excessive joule-heating effects that lead to accelerated degradation. For these reasons it should not be surprising that failure is signiﬁcantly more frequent in via structures than in interconnect stripes as the comparison in Figure 5.22 reveals.


5.6.2 EM in Interconnects: Current and Temperature


Dependence


Irrespective of the kind of damage produced, the analysis of more than a quarter century of EM reliability testing of interconnections has distilled the following general relationship between mean time to failure (MTTF) and operating current density and temperature, namely


MTTF1 ¼ Bjne expEekT:


(5.31)


Mass Transport-Induced Failure 287


This equation, where B is a constant and Ee is the activation energy for EM, is attributed to Black [30], who found that n¼ 2. In this or otherversions, the equation plays a useful role in designing metallizations.


An argument that supports the n¼ 2 current density–dependence suggests that MTTF1 suggests that MTTF-1is proportional to the product of the number of voids in a stripe and the rate at which voids grow. Each of these factors M1


Figure 5.21 Electromigration damage at vias between metallization levels M1 and M2.


(a) Void formation in metallization at bottom of via plug. (From Ref. [27].) (b) Void formation in metallization at top of via plug. (From Ref. [27].) (c) Thinned metallizations at via bottom and sidewalls. (From Ref. [28].)


95


Via at


9010 mA / μm2


75


Fails50


(%)


25


10 mA / um2


aStripe at e 000000


Figure 5.22 Comparison of via and interconnect stripe failure rates. From Ref. [29].


Al accumulation(b)


TiW


e-)M2


Al-Cu


wAl depletion


void


eAI-Cu


M1


eM2二voids


depends on je, so that a j2e dependence is predicted. An additional theoretical justiﬁcation for this formula, based on stress effects, will be derived later, in Section 5.7.3.2. Finally, a recent experimental study in which temperature was measured over a 1-mm diameter spot size supports the Black equation for low values of current density [31]. However, at high current densities larger values of n reﬂect synergistic effects beyond simple isothermal transport, e.g., due to thermal gradients, current crowding, stripe narrowing, etc. The data of Figure 5.23 display these trends and indicate that values as high as n z 10 occur when je approaches 1 107 A/cm2.The thermally activated nature of EM damage is underscored by Eqn(5.31). It is important to realize, however, that Ee and n values extracted from lifetime testing, resistance monitoring, or other indirect measurements typically reﬂect a complex admixture of mass transport and damage processes: void nucleation, migration and coalescence, GB diffusion, surface diffusion, stress-assisted diffusion, thermomigration, grooving, extrusion,and so on. Increasing current densities enhance these processes in a


Figure 5.23 Electromigration lifetime of aluminum metallizations as a function of current density. Criterion for life is a 10% change in resistivity. Below, a current density of 2 106 A/cm2, n¼ 2. Larger values of n are attained as je approaches 1 107A/cm2. From Ref. [31].


Mass Transport-Induced Failure 289


nonlinear fashion. It is little wonder, then, that hot spots develop to further accelerate failure.


A range of activation energy values typically measured in assorted metalﬁlms used in electronics technology are entered in Table 5.1. Corresponding composition and grain size ranges employed are also listed. For more detailed information on the more than 60 studies from which the representative composite values of Ee were selected, the reader should consult the indicated reference. The overwhelming bulk of the data pertains to Al and Al alloy metallizations, where the following observations apply:


1. The activation energy for bulk diffusion in pure Al is 1.4 eV. For ﬁlms with large grain size there are few avenues for defect diffusion paths,and thus Ee is found to be 1–1.2 eV. However, measured Ee values in the neighborhood of 0.4–0.6 eV for the usual ﬁne-grained ﬁlms are indicative of GB mass transport-induced damage. Observed grain size-dependent activation energies are the apparent consequence of weighting admixtures of low bulk and high GB diffusivity contributions.


2. Additions of Cu to Al raise Ee by a few tenths of 1 eV and extend MTTF lifetimes of Al accordingly. This important ﬁnding is the basis for the use of Al alloy metallizations containing approximately


0.3–5 wt% Cu. The effect of Cu is not completely understood, but


Table 5.1 Electromigration in metal ﬁlms Metal


Grain size (mm) )Failure criteria Ee (eV)


|Pure Al |0.1e2 |DR/R, open |0.35 to |2e4 |
|---|---|---|---|---|

|||circuit |w0.6 ||

||6e8 ||1.0e1.2 ||

|Ale0.3 to |1e6 |DR/R, open |0.5e0.8 |2 |

|5 wt% Cu ||circuit |||

|Ale0.3 to |0.3e7.6 |DR/R, open |0.31e0.8 |1.7e5.4 |

|3 wt% Si ||circuit |||

||||0.25-0.86||

|AleCueSi |0.25e0.6 |DR/R, open |0.25e0.86 |0.25e0.86 |

|||circuit ||1.7 |

|Au |0.2e0.5 |DR/R, open circuit, tracer, |0.7e0.9 |3.3e4 |

|Ag Cu |||1.1e1.4a |0.3e0.95 1.1 |

¼ added by authors.Primarily adapted from Ref. [32].


the Al2Cu precipitates and dissolved Cu appear to interact with Al atoms in GBs and impede their motion. (In commercial Al–Cu precipitation hardening alloys these same Al2Cu precipitates strengthen the Al matrix.) It is also common to add 1 wt% Si as well to prevent Al–Si interdiffusion at semiconductor contacts.


3. The activation energy values are in general agreement with the diffusivity systematics presented in Eqn (5.7). Thus Ee scales directly with higher melting point and larger grain size.


5.6.3 Effect of Conductor Geometry and Grain Structure


on EM


The dependence of conductor length and width on EM life has been a subject of continuing interest. Assuming constant width, longer stripes simply have more potential failure sites (e.g., triple points) than shorter conductors, and therefore, they are observed to exhibit reduced lifetimes.


But, when stripes are unusually short, stress-induced mass backﬂow effects(Sect. 5.5.4) surface to counter EM damage.


From the earlier discussion of structural barriers (Section 5.5.5.2) the desirability of having equiaxed grains is evident. Even better than equiaxed grains are interconnects with no GBs, i.e., a single-crystal Al ﬁlm.


Since it is impractical to deposit such a ﬁlm, the best alternative is an interconnect with a bamboo grain structure that effectively behaves like a series stack of single crystals. The GBs are then oriented normal to the current ﬂow. In such a case the only path available for mass transport is through the bulk grains, an unlikely avenue at low temperature. From a geometric standpoint, shrinking line dimensions make bamboo structures more probable. Interestingly, the effect of decreasing ﬁlm linewidths on EM failure time reveals an unexpected beneﬁcial twist, as revealed in Figure 5.24. Film life decreases as the linewidth is reduced from 4 to 2 mm, in accord with intuitive expectations that the narrower the stripe,the easier it is for damage to span across it. However, an encouraging increase in life occurs below 2 mm because of the bamboo grain development [33].


formationLwy


dAI


L


flow


Figure 5.15 Schematic model of damage in an interconnect subject to electromigration. Hillocks and voids develop in response to temperature gradients superimposed on the directed electron current ﬂow.


temperature attained is a useful prelude to estimating the current passed prior to failing. Such an analysis [17,18] is applicable to the behavior of fuses that cause an open circuit by melting.


Let us ﬁrst consider current i (A) passing through a wire of length L and cross-sectional area A whose electrical resistivity is r (U-cm) and thermal conductivity is k (W/cm-K). Assuming no heat loss occurs by radiation or convection, the nonsteady-state heat ﬂow equation describing the temperature (T) at any position (x) may be written as


dcvT


vt¼ kv2Tvx2þ i2rA2;


(5.22)


with d and c the wire density and heat capacity, respectively. (Note that k/dc is the thermal diffusivity, which has units of cm2/s.) In addition to the two familiar terms in Eqn (5.22), the rate of heat generation must be considered. In a short length of resistor wire dx, this amounts to i2 r dx/A.


Thermal and electrical conductivities (s, where s¼ 1/r) of metals aretheoretically connected by the well-known Weidemann–Franz law,expressed by s¼ k/LT, where L is the Lorenz number, a constant equalto to 2.44x10-8 W-Q/K2. In the steady state, dT/dt=0, and therefore2.44 108 W-U/K2. In the steady state, dT/dt¼ 0, and thereforeEqn (5.22) now assumes the far simpler form of the harmonic oscillator equation,


dT 2


dx2þ B2T ¼ 0;


(5.23)


where B2¼ i2L/(A2k2).The physical problem we now address is a conductor whose ends are maintained at ambient temperature To. Wirebonds that connect silicon chips to metal lead frames approximate this geometry. By solving Eqn(5.23), it is not difﬁcult to show that the maximum temperature (Tmax)reached, which occurs at the midspan (L/2), is given by


Tmax


To¼


1 cos BL2¼


cosiL1=2L2Ak :


(5.24)


Wire failure occurs when Tmax reaches the melting point TM, in which case the critical current density jcrit (i/A) is given by


jcrit ¼2kL1=2Lcos1ToTMjenit =(2c/L1/2L)cos-1(To/TM).:


(5.25)


Mass Transport-Induced Failure 277


Substituting the following values for Al, k¼ 240 W/m-K, L¼ 10–2 m,TM¼ 933 K, and To¼ 298 K, yields jcrit¼ 3.83 108 A/m2 or3.83 104A/cm2. As noted earlier, thin-ﬁlm stripes are able to sustainpassage of considerably larger current densities because the substrate serves as a massive heat sink for the conductor.


More involved nonsteady-state heat ﬂow analyses that include radial heat loss from powered wires have also been published [19]. Such calculations of transient temperature behavior have proven useful in designing operating conditions for wire bonding processes that avoid excessive heat damage due to passage of high currents.


What are the implications of temperature gradients on EM in thin-ﬁlm stripe metallizations? Assuming that the above calculation applies, we may expect a sine-like temperature distribution, i.e., To at the ends, Tmax at the center. Therefore, atoms originating at the negative end of the stripe migrate not only in the direction of electron ﬂow, but also into a hotter region of the stripe. They accelerate because of the strong thermal activation of the ion mobility and in moving ever faster leave mass-depleted regions behind. At the anode end the reverse happens. Now the atoms are driven from a hot region, where they move rapidly, to the cooler end,where they decelerate. Atoms pile up, and mass tends to accumulate there.


These expectations are borne out by the overall negative sign of second term in Eqn (5.21). If at the cathode end dT/dx is negative, the temperature derivative of the quantity in parentheses is also negative; i.e., Z* < 0,and the rise in D with temperature swamps any countertrend in the other terms. Therefore, ðvC=vtÞ < 0, and mass depletions are anticipated. Theheated stripe is like a highway that goes from one lane to two lanes and then back to one lane. Cars that initially travel slowly pick up speed in the two-lane portion only to slow down again. In concert, the intercar spacing is small initially, then widens (as gaps or voids develop), and ﬁnally decreases as cars enter a jam once again (where hillocks form). Some of these features are illustrated in the model of void and hillock damage depicted in Figure 5.15.


5.5.4 Role of Stress


Metal thin ﬁlms are invariably deposited in a state of stress. Therefore, we may well ask what role stress plays in EM. Just as an electric ﬁeld causes atomic drift, so too a gradient of stress (s) acts as a generalized force to induce atomic motion. Thus, atoms preferentially migrate from compressively (smore negative) stressed regions and accumulate at locations stressed


in tension (s more positive), while vacancies diffuse the other way. The resulting stress gradient causes a backﬂow of matter, and, as we shall see, this effect has signiﬁcance in short conductors. Thermodynamics argues that the free energy per atom in a stress ﬁeld, or chemical potential (m) of an atom,depends on the stress and is equal to m¼ –sU, where U is the atomicvolume (cm3/atom). Furthermore, the force per atom in a stress ﬁeld is the negative gradient of the chemical potential, or


F ¼ Udsdx:


(5.26)


Blech [20] demonstrated the role of stress in a clever experiment involving electrotransport in short Au lines deposited on longer more resistive molybdenum ﬁlm conductors. Current through the latter shunted to the Au as shown in Figure 5.16, causing atoms to electromigrate from the cathode to anode side and pile up there. The displaced cathode edge enabled a direct measurement of the atomic drift velocity. A surprising result was the cessation of edge migration when stripes were shorter than a critical length Lc. The effect arises from a stress-induced backﬂow of atoms


While AuAl2 alone has an acceptable electrical conductivity and is mechanically strong, Kirkendall voids degrade both of these bond properties. The rate at which AuAl2 thickens is given by x2AuAl2=t ¼1:23 exp½1:2 eV=ðkTÞðcm2=sÞ and follows parabolic kinetics [1].


5.4 REACTIONS AT METAL–SEMICONDUCTOR CONTACTS


5.4.1 Introduction to Contacts


Achieving the requisite ohmic or Schottky electrical behavior of contacts poses challenges in processing ﬁrst, which are then followed by the reliability concerns of property change in service. Metal–semiconductor interdiffusion effects at contacts are primarily responsible for reliability problems manifested as short circuits at junctions, increases in contact resistance, and Schottky barrier height variations. These effects are aggravated in devices that pass large currents and heat appreciably. In silicon devices prior to about 1980, aluminum was the contact metal of choice.


However, as device dimensions shrank, the Al–Si interdiffusion damage described in the next section led to the adoption of alternative metal–silicide contacts.


Figure 5.6 Extensive AuAl2 growth and Kirkendall porosity at the interface between a thermosonically formed gold ball bonded to an aluminum pad. From Ref. [4].


New contact metallurgies for Si are less susceptible to reliability problems than metal contacts to GaAs and compound semiconductor devices.


Among the reasons for this are [5]:


1. GaAs decomposes into Ga and As2 gas at 580C.


2. The Schottky barrier height (FB) is typically w0.8 eV for most metals.


An implication of this is intrinsically high contact resistance. (In contrast,FB for Si is w0.6 eV.)


3. It is difﬁcult to dope n-GaAs to levels higher than 5 1018/cm2.4. Annealing up to 850 C is required to electrically activate dopants following ion implantation. Therefore, special precautions must be taken to avoid decomposition or melting.


5. Because two elements comprise compound semiconductors, there are more possibilities for reaction with contact metals.


5.4.2 Al–Si Contacts


The problems considered in this section arise during processing rather than service. Nevertheless, they are instructive and when extrapolated to low temperatures and long times may have reliability implications. We ﬁrst consider the simple Al–Si contact, which until the VLSI regime was the common method for making electrical connection to Si devices. To form the contact, Al is deposited on the Si, which is covered by a native,discontinuous thin ﬁlm of oxide, as shown in Figure 5.7(a) and (b). The contact structure essentially consists of a diffusion couple of the two elements.


Reference to the accompanying Al–Si phase diagram (Figure 5.8) reveals that the solubility of Si in Al increases as the temperature is raised, reaching w1 wt% at 500 C. At this common processing temperature, Si readily diffuses in Al in order to satisfy its solubility requirements (Figure 5.7(c)); the loss of Si leaves pits behind in the semiconductor. Meanwhile, Al countermigrates into the Si. However, very small amounts of Al dissolve in Si. Excess Al ﬁlls the Si-depleted regions and precipitates in the form of conductingﬁlaments that can “spike,” or short, shallow junctions (Figure 5.7(d)).


Damage at Al–Si contacts shown in Figure 5.9 takes the form of surface pits, which can be made visible by etching off the aluminum. The Si-pit size(dSi) has been shown [6] to grow in a thermally activated way with parabolic kinetics; i.e., dSiz expð EkTÞt1=2. Furthermore, as the contact area (AC)increases, the pit size was observed to decrease according to dSi z AC0.4. In order to explain this effect we note that increasing the contact area enlarges


Mass Transport-Induced Failure 261


the Si to Al ratio. But the volume of Al that can be saturated at any diffusion temperature remains ﬁxed. More locations and avenues for interdiffusion means less reaction at each site, and hence a smaller dSi.


Example 5.1


Consider the contact structure of Figure 5.7(c) consisting of a pure Al ﬁlm of indicated geometry over Si. Calculate the depth (y) of Si depletion in the wafer during a processing


Figure 5.7 Schematic sequence of interdiffusion effects at an Al–Si contact, leading to junction spiking. (a) Native oxide in contact window. (b) Deposition of aluminum. (c)Silicon diffusion into aluminum upon sintering treatment at 450 C. See Example 5.1.


(d) Counter diffusion of aluminum into silicon shorts junction.


heat heat treatment of 1 h at 450 C, where the solubility (S) of Si in Al is 0.5 wt%. The respectivetreatment of 1 h at 450 C, where the solubility (S) of Si in Al is 0.5 wt%. The respective densities for Si and Al are rSi¼ 2.33 and rA1¼ 2.7.Answer The amount of Si needed to saturate the metal contact structure depends on the Al volume as well as the solubility of Si in Al. Conservation of mass requires that the amount of Si lost beneath the contact window must equal that which enters the metal. For(polycrystalline) Ale(single crystal)Si couples, the diffusivity of Si in Al is given by D¼ 25 104 exp [e0.79 eV/(kT)] cm2/s [5]. By Eqn (5.6), the total diffusion length D = 25 x 10-4 exp [-0.79 eV/(kT)] cm2/s [5]. By Eqn (5.6), the total diffusion length (L)(L)along both sides of the contact at 450 C is calculated to be L¼ 4 {(25 along both sides of the contact at 450C is calculated to be L=4x {(25 x10104 -4 exp [-0.79 eV/8.62x10-5 x723])x3600}1/2=1.07x10-2 cm (107 μm). Therefore,exp [e0.79 eV/8.62 105 723]) 3600}1/2¼ 1.07 102 cm (107 mm). Therefore,LwdrAlS¼wCyrSi. Solving, y ¼ LdrAlSðCrSiÞ ; substituting rAl¼ 2.7, rSi¼ 2.33, and assuming w¼ 2 mm, d¼ 1 mm, and C¼ 5 mm, y is calculated to be 0.123 mm.


WEIGHT PERCENT SILICON


1020


7000.5丁


↓


577°


1500


(AI)


1.59


-1430°


(1.65)


1400


1300


0.16 (0.17)


3001


1200


(AI)+Si


1100


630


C °TEMPERATURE,0


0.51.01.5


610


590


700


660°


5705


5779


1(11.7)


01020304050 60708090100 AI


ATOMIC PERCENT SILICONSi


11.3


Si-→


A1-%'si15


12.1(12.5)


577.2°


At-%Si


900


2961.52.0一30405060708090


Figure 5.8 Equilibrium phase diagram of the Al–Si system.


Mass Transport-Induced Failure 263


This example shows that direct Al–Si contact cannot be tolerated under any circumstances, because the reaction dimensions are uncomfortably large compared to device junction depths. The use of Al metallizations saturated with greater than 1 wt% Si eliminates the driving force for these interdiffusion effects. But when this alloy cools, Si precipitates as its solubility declines, leaving nodules behind on the semiconductor surface. These nodular islands are p-type Si (Al) doped and generally raise the contact resistance. Similar but generally more severe interdiffusion effects result from reaction between Al and polycrystalline Si (polysilicon) ﬁlms. Diffusion and reaction lengths are expected to be larger for polysilicon.


5.4.3 Metal Silicide Contacts to Silicon


To protect submicron-deep junctions against the intrusion of the Al metallization, diffusion barriers composed of metal silicides, or Ti–W alloys are commonly interposed to limit interdiffusion between Al and Si. Silicides are metals with resistivities of w15–50 mU-cm, which is considerably higher than the value for Al (2.8 mU-cm). They are formed by reacting refractory metal ﬁlms deposited on Si wafers. Rather than the pitted Al–Si interface, the resulting silicide layers yield very stable planar and uniformly thick contacts. Silicides that have seen use in microelectronics applications


Figure 5.9 Alloy penetration pits formed by interdiffusion of aluminum and silicon.


Contact reaction occurred during sintering at 400 C for 1 hour. From C.M. Bailey, D.H.


Hensler, AT&T Bell Laboratories.


are listed in Table 2.1 together with some of their properties. These contacts are relatively immune to degradation in normal service. Problems do,however, arise at elevated temperatures during EM and such effects in TiSi2 and TaSi2 contacts will be discussed in Section 5.6.1.1.


Silicides not only provide necessary electrical contact functions, but also serve as diffusion barriers. Occasionally, Al and the silicide chemically combine so that the fundamental problem of curbing Al reactivity remains.


As an example of the potential degradation of metal silicides consider the case of PtSi [7]. This intermetallic has been used in microelectronics because it makes nearly ideal ohmic and Schottky barrier contacts. However, the reaction between Al interconnects and PtSi at a Si contact yields the PtAl2 intermetallic compound and attendant electrical instabilities in the operation of Schottky diodes. Compound formation was reported to obey reaction kinetics given by


fPtAl2 ¼ 1 expð½KðTÞtn:


(5.12)


Here fPtAl2 is the fractional amount of PtSi transformed to PtAl2, and K(T) is a temperature-dependent constant proportional to the ubiquitous Boltzmann factor z exp[–E/kT]. The constant n had a value close to 3,and activation energy E was equal to 2.2 eV. As a gage of the reaction,f reached a value of 0.5 at 340 C after 1000 h.


This study is interesting for a couple of reasons. First, Eqn (5.12) is the Avrami equation (see Eqns 4.35), which describes the kinetics of phase transformations that occur by nucleation and growth processes. Secondly,such kinetics have the form of the Weibull distribution function.


5.4.4 Contacts to GaAs Devices


5.4.4.1 Scope


Just as in Si devices, the seeds of GaAs contact reliability problems are often planted during processing. A good example is reproduced in the transmission electron microscopic cross-sectional image of a high-electronmobility transistor contact structure (Figure 5.10). Due to a 1–2 nm thick oxide barrier between the metallization and underlying AlGaAs, metal alloying occurred nonuniformly. In reducing contact quality, conducting projections that threatened to short to the GaAs layer, formed.


The resemblance to the “spiking” of shallow junctions in Si, discussed in Section 5.4.2, is evident.


Service failures in GaAs devices can occur at surfaces and interfaces, in the substrate or active layers, at Schottky and ohmic contacts, and by EM


Mass Transport-Induced Failure 265


and corrosion damage of the metallization. Damage manifestations of several of these are schematically shown in Figure 5.11 indicating mass transport effects between and around the contact metals. Lifetimes of all GaAs devices (e.g., MESFETs, MODFETs, LEDs) depend strongly on the AIGaAsGaAs


1 cm=650A Figure 5.10 TEM micrograph of Ni/Au-Ge/Ag/Au alloyed ohmic contact (420 C, 20 Figure 5.10 TEM micrograph of Ni/Au-Ge/Ag/Au alloyed ohmic contact (420°C, 20 s)s)on a GaAs/AlGaAs HEMT structure. From Ref. [8]. Courtesy F. Ren, Lucent Technologies,Bell Laboratories Innovations.


(a)SOURCEGATE


Wn-epiC


Si- GaAs


Figure 5.11 Views of damage to metal contacts in GaAs transistors. (a) Localization of damage in a MESFET at A. surface region between gate and source (and drain)metallization, B. source and drain ohmic contacts, C. Schottky gate contact and underlying channel, and D. gate metallization. (From Ref. [9].) (b) Damage due to a highpower pulse applied to the gate. A. interdiffusion of Au through Cr to active channel,B. thermal runaway, C. metal–GaAs interdiffusion. (From Ref. [9].) (c) Interelectrode short-circuit bridge. A. material depletion, B. initiation of migration, C. drain (AuGeNi),D. edge of gate recess, E. gate (Al), F. traces of material migration, G. droplets due to material accumulation. (From Ref. [10].)


GaAsMETAL


stability of the metals employed in ohmic, Schottky, and heat-sinking contacts [9–12]. The three main contact-degradation effects include:


1. Long-term interdiffusion within metal sandwich structures;


2. Electric ﬁeld-induced metal migration between closely spaced neighboring electrodes; and


3. Metal migration through narrow conductors carrying large current densities (EM).


Figure 5.11 Cont'd.


Mass Transport-Induced Failure 267


S


G


5.4.4.2 Schottky Contacts


These contacts must adhere well to GaAs, have a high conductivity (low sheet resistance), be amenable to lithographic processing, and be stable with respect to interdiffusion, corrosion, and EM. Only a few metals possess this complement of properties, with Al and Ti being the most commonly employed. In the case of Al, two speciﬁc failure mechanisms have been identiﬁed, namely Al/GaAs interdiffusion and EM. Accompanying the degradation at the Al/GaAs interface is an undesirable increase in electron barrier height, typically from 0.7 to 0.9 eV. While Al/GaAs contacts are thermally stable, the same is not true for Ti, which readily oxidizes. This makes wire bonding difﬁcult, a problem solved by an Au overlayer.


However, the Au/Ti/GaAs contact structure is unstable at temperatures as low as 200 C. The solution here as in Si technology is to interpose diffusion barriers that minimize, but do not totally eliminate, reactions between Au and Ti. Metals such as Pt, W, Pt/Cr, and Pd have been used for this purpose.


Diffusion of Au into GaAs after penetrating through metal-barrier layers is a primary failure mechanism in Au-based gate metallizations. When this happens, the metal/semiconductor interface advances into the channel,narrowing its effective thickness. In addition, diffused metal alters the net donor concentration in the channel and modiﬁes device behavior.


Typical activation energies for degradation of Al contacts range from 0.8 to


1.0 eV. Reﬂecting greater stability, the corresponding activation energies for Au-based contacts are larger, and values of 1.5–1.8 eV have been reported.


5.4.4.3 Ohmic Contacts


Parasitic contact resistance at source and drain ohmic contacts inﬂuences a number of FET device parameters (transconductance, saturation current,etc.). The most widely used metallization for ohmic contacts to GaAs is derived from an Au–Ge eutectic alloy covered by a Ni layer to improve wettability. The resulting AuGeNi possesses low contact resistance required for high-frequency and high-power applications. Increases in contact resistance have been attributed to four effects:


1. Outdiffusion of Ga and As from GaAs and subsequent reaction with the contact metal. A nonstoichiometric defect-rich region is then left behind under the contact.


2. Indiffusion of Ga.


3. The doping density in the semiconductor is reduced by indiffusion of Au and Ni.


4. Formation of NiAsGe, AuGa, and Ni2GeAs compound phases. This reduces the effective contact area.


Among the interesting manifestations of damage in unpassivated GaAs MESFETs are As2O3 polyp growths over ohmic contacts containing Au


[13]. A model for their growth suggests that As is liberated as a by-product of GaAs dissociation by Au, a reaction that results in the formation of an AuGa alloy. Room temperature Kirkendall-like interdiffusion between Ga and Au facilitates the simultaneous migration of As to the contact surface,where it oxidizes. Passivation protection against moisture minimizes the occurrence of such damage.


5.4.4.4 Gate Sinking


Diffusion of gate metals into the underlying GaAs effectively reduces the thickness of the active layer, an effect known as “gate sinking.” The change in device pinch-off voltage (Vp), a degradation mode suffered by GaAs MESFETS, is a consequence of gate sinking [14]. A diffusion model to explain this effect is based on the metal migration that occurs. For onedimensional diffusion of the Schottky contact metal into GaAs we have for constant surface concentration, Cs (Eqn (5.3)),


Cðx; tÞ ¼ CsErfc"xð4DtÞ1=2#:


(5.13)


Assuming that the metal front is at depth Xd with a concentration of w104, then Xd¼ 2.75 2 (Dt)1/2. Theory shows that the pinch-offvoltage in an active layer of thickness W, reduced in time t by Xd, is given by


VpðtÞ ¼ qNðW  XdÞ22εþ Vo;


(5.14)


where N is the effective layer doping level, q is the electronic charge, ε is the effective dielectric constant, and Vo is the built-in voltage. Relative to the initial pinch-off voltage, Vpð0Þ ¼ qNW 22εþ Vo, the change is given by DVp ¼ qNXdWε;


(5.15)


where it is assumed that Vo is constant and Xd/(2W)< 1.


Therefore, it is predicted that the pinch-off voltage drifts parabolically with time according to


Mass Transport-Induced Failure 269


D½Vpðt;TÞ ¼ 5:5qNWεðDotÞ1=2 exp Ed2kT(5.16)


by combining previous equations and decomposing the temperaturedependent diffusivity into constants Do and Ed. Comparison of Eqn(5.16) with the measured behavior of MESFETs is made in Figure 5.12(a) and lends support to the proposed diffusion model.


5.4.4.5 Failure in MODFETs


Mechanisms for MODFET failure have been summarized by Anderson


[11] and include those mentioned earlier. Contact degradation and gate interdiffusion are the most common. Thus gate sinking from Schottky contacts, in addition to effectively thinning the AlGaAs layer, alters Schottky barrier heights. Interdiffusion of ohmic contact metal into GaAs apparently causes electron trapping, establishing a barrier to current ﬂow.


Deconﬁnement of the two-dimensional electron gas (Section 2.7.4),together with reduction of carrier mobility and saturation velocity, are other suggested consequences of the diffusion of either contact metal,dopants, or semiconductor constituents. The parabolic kinetics of change in barrier height and source resistance shown in Figure 5.12(b) and (c) lend further credence to diffusion-based degradation mechanisms. These effects are not solely limited to GaAs-based HEMTs. A recent study on 0.1 mm gate length InP HEMTs [15] revealed a transconductance decrease as a result of gate sinking. The kinetics of degradation were parabolic with time,and deﬁned by an activation energy of 1.26 eV.


5.5 EM PHYSICS AND DAMAGE MODELS


5.5.1 Introduction


Electromigration, a phenomenon not unlike electrolysis, is characterized by the migration of metal atoms in a conductor through which large direct-current densities (je) pass. It occurs in pure metals as well as in alloys and has been suggested as a mechanism for failure of tungstenﬁlaments in light bulbs. Lamp ﬁlament failures will be addressed at the end of the chapter. EM was ﬁrst identiﬁed as a reliability problem in IC metallizations more than 30 years ago. Interest in EM has persisted to the present day, where it still remains a troublesome reliability issue, as re-ﬂected by the many publications and conference sessions devoted to it each year.


Of the order of hundreds to several thousand meters of narrow, thin-ﬁlm interconnections of Al less than 1 mm in width are now present on typical IC chips to connect devices to one another and to contact pads. For a 700 million-transistor microprocessor chip, average interconnect lengths


Figure 5.12 Diffusion-induced changes in electrical characteristics of GaAs devices. In all cases, data plotted versus square root of time reveals parabolic kinetics. (a) Pinch-off voltage (Vp) drift for MESFETs aged at 205 and 225 C. (From Ref. [14].) (b) Decrease voltage (Vp) drift for MESFETs aged at 205 and 225°C.(From Ref.[14].)(b) Decrease inin barrier heights (FB) of AlGaAs/GaAs HEMTs aged at 225, 250, and 275 C. (c) Increase barrier heights (TB) of AlGaAs/GaAs HEMTs aged at 225, 250, and 275°C.(c) Increase inin parasitic source resistance (Rs) of AlGaAs/GaAs HEMTs aged at 225, 250 and 275 parasitic source resistance (Rs) of AlGaAs/GaAs HEMTs aged at 225, 250 and 275C.C.


(From Ref. [9].)


Mass Transport-Induced Failure 271


(a)0.500


0.400


225C


£0.300


Xd (A)


0.200


50


205C


0.100


0.000


0 01,0002,0003,0004,0005,000 VTIME (hrs)1/2


(b)0-30


T=225°C


-60


(人 u」)


8中


▽


-120


T=275°℃


GATE AI/Ti E=1.3eV


-150


-180


0102030405060 VTIME (hrs)1/2


-90


T=250°C


150


ofw30 mm are suggested, but in actuality a distribution of both shorter and longer lines is present. Critical interconnections such as clock, control, and data lines between the processor and cache may run the entire length of a chip and be 1–2 cm long. Optimum operation of devices frequently requires high signal currents. Because conductor cross-sectional areas are now quite a bit less than one square micron, current densities can reach high levels even at modest applied voltages. In fact, Al interconnects are designed to carry about 105 A/cm2 and can sustain up to w107 A/cm2 without immediately opening. This is a very large current density and would cause an isolated bulk Al conductor to rapidly melt, as we shall see in the calculation of Section 5.5.3. However, catastrophic failure does not occur immediately in thin-ﬁlm IC interconnections because they are effectively bonded to a massive heat sink that efﬁciently conducts away the joule heat that is generated.


Passage of high current densities through interconnects causes timedependent mass-transport effects that are manifest as surface morphological changes. Resulting conductor degradation includes mass pileups in hillocks and whiskers, void formation and thinning, localized heating, and cracking of passivating dielectrics; examples of the effects of EM are shown in Figure 5.13. In bootstrap fashion these damage processes accelerate to the point where open circuiting terminates conductor life. There is thus a basis for a corollary of one of Murphy’s laws: “A million-dollar computer will protect a 25-cent fuse by blowing ﬁrst.”


Figure 5.12 Cont'd.


As the feature size of dimensions has shrunk the need for a higher conductivity metal has resulted in the choice of copper as a replacement for Al–Cu. Copper has unique requirements, namely it must be encased in a diffusion barrier on all sides to keep it from diffusing into SiO2 and the Si devices, as well as prevent corrosion and EM extrusions. The use of lower dielectric constant (k) interlayer dielectrics (ILD), which are softer than SiO2, has further complicated the occurrence of stress and voiding due to these material properties. As we discussed in Chapter 2, the dual damascene process is used to ﬁll prelined trenches with copper, and the excess copper is removed using chemical mechanical polishing (CMP). We will present the


Figure 5.13 Scanning electron microscope images of electromigration damage in aluminum interconnects. (a) Hillock extruded through a hole in overlying glass layer causing a short. (b) Void formation across the stripe. From Ref. [16]. For other examples of electromigration damage, see Figure 5.26.


Mass Transport-Induced Failure 273


details for copper electromigration (EM) and stress voiding (SV) in Section


5.8, after discussing Al–Cu, which is still used in all manufacturing facilities which are not practicing state-of-the-art technology. A key point is that as technology evolves it takes a very long time for older technology to be replaced in existing facilities. In particular, new technology is usually placed in new facilities and the old facilities are used to continue making older products, until the cost of manufacture will no longer sustain the selling price. This is called end of life for a product made in a given older technology and is the death knell for availability of that product. Often ﬁrms that depend on that product are given the option of a one time ﬁnal buy to help them transition to a replacement.


5.5.2 Physical Description of EM


5.5.2.1 Atomic Model


At a fundamental level, EM involves the interaction between current carriers and migrating atoms. The nature of the interaction is not entirely understood, but it is generally accepted that in an electron conductor,electrons (of charge q) streaming toward the anode can impart sufﬁcient momentum to atomic ion cores upon impact to propel them into neighboring vacant sites. Depicted in Figure 5.14 is the sequence of events. The electric ﬁeld, which exerts an electrostatic pull on positively charged ion cores toward the cathode, is simply insufﬁcient to withstand the oppositely(anode) directed “electron-wind” force at high current densities. Therefore,


Figure 5.14 Atomic model of electromigration. The electron wind at large current densities imparts sufﬁcient momentum to ion cores to propel them into neighboring vacancies.


there is a net force (F) that biases the normally random motion of an atom precariously perched in a saddle-point conﬁguration between two ﬂanking half-vacancies. This force, given by


F ¼ ZqE ¼ Zqrje;


(5.17)


is sufﬁcient to push the ion over the energy barrier, so that it preferentially migrates toward the anode. In this equation the electric ﬁeld E is related to the current density through the resistivity r, i.e.,E¼ rje, and Z* is theeffective ion valence. Experiment reveals Z* to be negative in sign and has a magnitude far in excess of typical chemical valences. There is wide scatter in reported magnitudes of Z* in different metals. For Al a typical value is 10, while values several times larger have been reportedin Au and Sn.


5.5.2.2 Macroscopic Equations of EM


Even though there are no concentration gradients present in pure metals,diffusional atomic movement by EM does in fact occur. How is this possible, and how is the apparent paradox resolved? Earlier, in Section


1.3.3, notions of atom transport were enlarged to include the effect of generalized forces such as electric ﬁelds, and the very important Nernst–Einstein equation (Eqn 1.6) was derived. We start here with an operating deﬁnition of the ﬁeld-induced mass ﬂux that results in a diffusional drift of migrating atoms with velocity v, namely.


J ¼ Cv;


(5.18)where C is the atomic concentration (atoms/cm3). The total mass-ﬂux J (atoms/cm2-s) through the conductor due to both atomic diffusion(Eqn (5.1)) and drift (Eqns. (5.18) and (5.16)) is


J ¼ DdCdxþ CDFRT;


(5.19)


where F is the generalized force and RT has the usual meaning. For our particular application, F¼Z*q E (Eqn (5.17)), and if the concentration-gradient term is neglected,J ¼ CDZqrjeRT:


(5.20)EM is thus characterized at a fundamental level by the material constants Z*, D, and r.


Mass Transport-Induced Failure 275


The passage to nonsteady-state mass transport is made via the equation of continuity; i.e., vCvt ¼ V$J . Film damage effects are caused by of continuity; i.e., a=-V.J. Film damage effects are caused by aanonvanishing divergence of J given by vCvt ¼vJvx 0x=-a-vJvTdTdx, orvC vt¼  0xlvvxCDZqrjeRT厂OTl vvTCDZqrjeRTvT了vx0 fCDZ*qpjel d fCDZ*qpjel oT: (5.21)


Thus when dC/dt< 0, mass depletion occurs and voids form. On the other hand, mass accumulates in growths and hillocks when dC/dt> 0.


However, when dC/dt¼ 0 there is no change in atomic density, and nodamage occurs. If alloys are involved, the appropriate diffusion term D v2Cvx2, normally absent in the case of a pure conductor, would beincluded.Many of the time-dependent failure models that we will consider later are based either on portions of Eqn (5.21) or on modiﬁcations of it. The ﬁrst term on the right-hand side arises from local structural and property gradients at constant temperature. Temperature gradients and thermally dependent properties that exist along powered ﬁlm stripes contribute to the second term on the right. The resultant damage is schematically depicted in Figure 5.15.


5.5.3 Temperature Distribution in Powered Conductors


Before addressing material transport during EM it is instructive to consider the separate issue of heat transfer in powered metal wires. Calculation of the


DirectionVoid


of electronformation


Hillock


From the standpoint of processing, the ﬁlm lifetime seems to be affected by method of ﬁlm deposition; evaporated ﬁlms are apparently longer lived than sputtered ﬁlms, a fact perhaps attributable to a more random crystallographic texture in the case of the latter. Multiple GB orientations thus appear to encourage electrotransport damage effects. A suggested formula that neatly summarizes the dependence of mean lifetime on grain size (S),


Mass Transport-Induced Failure 291


the standard deviation statistical spread in grain size (sgs), and the preferred crystallographic orientation is


BS


s2gs$logI111I2002:


(5.32)


Here the I’s are the corresponding X-ray intensities for planes of indicated indices and B is a proportionality constant. Clearly, more nearly equiaxed large grains that have a strong [111] orientation (texture) in theﬁlm plane are desirable.


A signiﬁcant experimental advance in characterizing the role of ﬁlm texture on EM has recently emerged. By capturing the backscattered electron-diffraction pattern from patterned interconnects with the use of a scanning electron microscope, the crystallographic orientation, or microtexture, of each individual grain has been mapped (see Section 11.3.2.1).


Intriguing ﬁndings using this so-called electron backscatter diffraction technique include the disappearance of certain off [111] texture grains as well as grain rotation as a result of EM [34].


Figure 5.24 Mean time to failure as a function of interconnect linewidth for evaporated (E-gun) and sputtered (ln–S) Al ﬁlms. From Ref. [33].


5.6.4 EM Lifetime Distributions


EM failure times are invariably modeled as lognormal distributions. Examples of EM failure data plotted in lognormal form are shown in Figure 5.25. There are two physical reasons that explain why this particular statistical function is applicable to EM failures. The ﬁrst has to do with profusion of damage mechanisms exhibited. As a result of the suggestion in Section 4.5.4 we may assume that EM exhibits a corresponding number of randomly distributed activation energies. But since failure times are directly proportional to the Maxwell–Boltzmann factor, exp [–Ee/kT], the logarithm yields Ee/kT, which is normally distributed. Hence the overall use of the lognormal distribution.


A second explanation justifying the applicability of the lognormal distribution is based on the temperature dispersion of conductors during life testing [36]. Due to the different thermal resistance values, individual stripe temperatures are normally distributed. Given the Black equation’s exponential dependence on temperature, a lognormal distribution of failure times would be expected.


Another approach to the statistics of interconnect reliability adopts the view that a metal stripe is a chain ofN independent links such that F(t) is the cumulative distribution function (CDF) of a single link [37]. The scaled CDF of the chain, FN(t), is then the strength distribution of the “weakest link,” or


FNt ¼ 1 ½1 FðtÞN :


(5.33)


Simple substitution of the Weibull form of F(t) reveals that FN(t) is also a Weibull distribution. Nevertheless, attempts to ﬁt large failure populations to such a self-reproducing Weibull function have proven unsuccessful [38].


But if F(t) is lognormal, FN(t) is not lognormal. The conclusion is that lognormal distributions can approximate true failure times only in a ﬁnite percentile interval. Furthermore, what characterizes the length of the weak link is not clear. Is it, for example, the grain size or perhaps the threshold length, Lc?


5.6.5 EM Testing


Irrespective of degradation mechanism, it is always a desideratum to accelerate testing in order to rapidly screen production lots prone to failure.


In the case of EM several test methods have gained popularity. Each has individual advantages and drawbacks, but in common fast response (minutes


Mass Transport-Induced Failure 293

