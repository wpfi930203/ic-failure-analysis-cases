---
title: "139_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_1fe45aa375ae8fb7757d3d6e4990a4a57295230462135641
file_size: 509628
---

## The likelihood of multiple bit-ﬂips due to neutron strikes and its implications on circuit designs 

Nanditha P. Rao and Madhav P. Desai Indian Institute of Technology Bombay, Mumbai-76, India Email: nanditha.rao@iiitb.ac.in, madhav@ee.iitb.ac.in

Abstract —A soft error is typically modeled as a probabilistic single bit-ﬂip model. In such models, an important issue to consider is the likelihood of multiple errors. The fact that a particle strike causes multiple ﬂips is noted in the literature. We use post-layout circuit simulations to characterize the impact of a single event transient (SET) on logic circuits and quantify the likelihood of multiple ﬂips. We ﬁnd that the impact of an SET needs to be viewed across two clock cycles and a good fraction of errors had multiple register ﬂips. A key observation is that, amongst the erroneous outcomes, the probability of multiple ﬂips for ‘gate-strike’ cases was substantial and went up to  $\bf{50\%}$  , where as those for ‘register-strike’ cases was only  $\mathbf{\nabla}_{\mathbf{\nabla}}$  . This implies that, even if we were to eliminate the ﬂips due to register strikes using robust ﬂip-ﬂop designs, a large fraction of the remaining ﬂips (due to gate strikes) is likely to be multiple ﬂips. Further, when a strike affected two nearby transistors, we saw an increase of a factor of 2x in multiple ﬂip probability. It is also likely that two SETs merge to produce a wider SET, thus increasing its probability of getting captured. This implies that, existing fault tolerant latch designs may need to be revisited to handle such scenarios.

Index Terms —soft error, multiple bit ﬂips, gate-strikes, logic circuits

## I. I NTRODUCTION 

S OFT errors are known to have a signiﬁcant impact on circuit reliability. When high energy particles strike a semiconductor substrate, they generate charge and in turn a glitch or a transient current in a circuit, known as the single event transient (SET). The SET can occur on a register or on a logic gate and can propagate to be eventually captured in a register, resulting in an error known as a single event upset (SEU) or soft error. Several observations in the literature reveal that a signiﬁcant amount of neutron ﬂux is found even at sea level [1], [2]. The average low energy neutron ﬂux (around 10MeV) at sea level is reported to be nearly 100000 neutrons/sq.cm per year [1]. They report that thousands of upsets happen every year at the ground level, which are mainly recorded by computer systems having error detection and correction logs. For instance, the average error rate in memories observed in several computers were reported to be nearly 1.5e-12 upsets/bit-hr and most of the upsets were due to atmospheric neutrons [2]. Most early studies focused on SEUs only in memories. SEUs in logic circuits were not considered because such circuits exhibit inherent masking phenomena. However, as technology scales, the impact of masking phenomena tends to reduce [3], [4], [5], [6] and it is important to study SEUs in logic circuits.

At the architectural level, soft errors are modeled by a probabilistic single bit-ﬂip fault model [7], [8], [9], [10]. This model has been challenged in [11], [12], [13], which report the probability of multiple bit ﬂips in logic circuits. However, the state-of-art fault model continues to be a single bit-ﬂip, single cycle model for soft error in logic circuits. Reliability estimates (such as mean time to failure/MTTF) and reliability enhancement techniques (such as error correction codes etc) are also based on the assumption that a single bit ﬂip occurs due to a particle strike. However, in reality, if multiple errors occur, these MTTF estimates are likely to be optimistic and the error correction methods are likely to be insufﬁcient. Most of the existing techniques that estimate soft error rate (SER) use approximate modeling techniques to arrive at these conclusions which reduces the accuracy of their results [14], [15], [16]. Therefore it is essential that our estimation technique be as accurate as possible, in order to increase the conﬁdence in the conclusions on the multiple bit ﬂip probability in logic circuits. So, we perform a detailed characterization of the impact of an SET using post-layout circuit (SPICE) simulations and Monte Carlo sampling scheme in order to get accurate bit-ﬂip statistics.

We performed a basic characterization to this extent in our earlier work on the  ISCAS’85  and  ITC ’99 benchmark circuits in 180nm and 65nm technologies [17]. We evaluated the bitﬂip statistics by comparing the SET-induced circuit simulation with a fault-free register-transfer-level (RTL) reference simulation. We found that the impact of an SET in a circuit can be understood as a two-cycle phenomenon, that is, the SEU outcomes need to be observed across two clock cycles (the two clock cycles following the cycle in which the SET is injected) in order to accurately capture the phenomenon. This led us to the fact that there are several possible SEU outcomes. We came up with a systematic notation for these outcomes and estimated the relative probabilities of all SEU outcomes.

We enhance our previous work [17] by performing experiments which are described in the rest of this section. We evaluate the conditional probability of multiple ﬂips given that an erroneous outcome occurs. In other words, given that an SET results in an error, what is the probability that the error is a multiple error? We ﬁnd that, overall, up to   $8\%$  of the erroneous outcomes result in multiple bit-ﬂips. The probability of multiple errors also increases as technology is scaled (based on   $180\mathrm{nm}$   and 65nm data). We show that the increase in multiple ﬂip probability as the technology scales is due to a potential reduction in electrical masking, conﬁrming

the observations made in [3].

We then evaluate this probability separately for strikes on logic gates and strikes on registers to understand their individual contributions. One of the key observations from our analysis is that, amongst the erroneous outcomes, the probability of multiple bit-ﬂips for ‘gate-strike’ cases was substantial and went up to   $50\%$  , that is, these errors are caused due to the propagation of the SET from the logic gate to the ﬂip-ﬂop. On the other hand, out of the erroneous outcomes, the likelihood of multiple ﬂips for ‘register-strike’ cases was just about  $2\%$  . This implies that, if we were to do hardened ﬂip-ﬂop designs to eliminate the ﬂips due to register strikes, then in such designs, out of the remaining ﬂips which will be due to ‘gate strikes’, a large fraction will be multiple ﬂips.

We study the impact of the width of the SET on the multiple ﬂip probabilities. We ﬁnally study the factor by which multiple ﬂips increase if a strike affects two nearby transistors in a circuit instead of one. We saw a substantial increase, a factor of 2x on an average, in the multiple ﬂip probability, when two transistors were affected. We show that it is likely that two SETs from nearest logic gates can merge and produce an SET of larger width at the input of a ﬂip-ﬂop, further increasing its chance of getting captured. So, existing error tolerant latch designs may need to be revisited to handle such scenarios.

We organize the rest of the paper as follows. In Section II, we provide a brief recap/introduction to the two-cycle phenomenon and describe the possible SEU outcomes in a logic circuit. We describe the experimental setup in Section III. We present our simulation results on  ISCAS’85, ISCAS’89 and  ITC ’99 benchmarks in Section IV. We discuss the role of electrical masking in Section V. We present the role of SET width and the impact of two SETs on multiple ﬂip probability in Sections VI and VII respectively. In Section VIII, we conclude the paper.

## II. TWO-CYCLE PHENOMENON AND THE POSSIBLE SEUOUTCOMES

In a logic circuit, a high-energy particle can strike a logic gate or a register, resulting in an SET. We call this the ‘gatestrike’ and ‘register-strike’ respectively. We model the SET as a current injection at the drain of a transistor in a particular clock cycle ‘k’. This SET can eventually propagate and get captured in a register or a ﬂip-ﬂop in the same clock cycle ‘k’ or in the subsequent clock cycle   ${\mathrm{�lder'}}$  , depending on the time instant at which the SET occurs in clock cycle ‘k’. These two possibilities can be explained as follows. If the SET ﬂips a register content early in the clock cycle ‘k’, it will have enough time to propagate and ﬂip some register in clock cycle  ${\bf\Psi}^{*}\mathrm{k}{\bf+}\mathrm{l}\,^{\prime}$  ’, as illustrated in Figure 1. However, if the SET ﬂips a register later in the clock cycle   $\mathbf{\epsilon}_{\mathrm{K}},$  , the error will not have enough time to propagate and ﬂip some other register in the subsequent clock cycle   ${\mathrm{�lder'}}$  , as illustrated in Figure 2. Thus, the impact of an SET, in reality, needs to be viewed across two clock cycles to accurately capture the phenomenon. We call this the ‘two-cycle phenomenon’, which is also explained in a detailed manner in our earlier work [17]. This time dependence of the strike is currently missing in the single bit ﬂip, single cycle fault model.

![Glitch injection  cycle  CLOCK  k-1   K+卫  SET  REGISTERSTRIKE  RegAflips   Flippropagatesiin  incycle(k)   time   REGA  OUTPUT  RegBflipsright   RegBflipis  aftertheclock   recorded at(k+1))   REGB  edge   OUTPUT  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cb77d19d-fad1-4651-a90a-59e4cad2a1f4/cb77d19d-fad1-4651-a90a-59e4cad2a1f4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=048c38ea27473bac4634e2d7ea9aa3f595ab32c1)
Figure 1. A ﬂip occurs in both clock cycles due to the SET occurring early in the clock cycle

![Glitch injection  cycle  CLOCK  k-1   K+工  SET  REGISTERSTRIKE  RegAflips   Flipcannot  incycle(k)   propagateintime   REGA  OUTPUT  RegBdoesnot  REGB  OUTPUT  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/362c02f5-b0ac-4769-8ecd-e31cc27fae7f/362c02f5-b0ac-4769-8ecd-e31cc27fae7f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=442e33f53506837688b2ec7d99aedd144507dec8)
Figure 2. A ﬂip does not propagate in time to the next cycle due to the SET occurring late in the clock cycle

We now classify the ﬂips and come up with a systematic notation for the possible SEU outcomes across two clock cycles. This is shown in Figure 3. In the ﬁgure, ‘N’ stands for no-ﬂip, ‘F’ stands for ﬂip and   $\mathrm{^\mathrm{F_{m}}}^{\prime}$   stands for multiple ﬂips. So, the illustrations in Figure 1 and 2 can be classiﬁed as ‘FF’ and ‘FN’ type of outcomes respectively as per this terminology. Thus, the occurrence of second ﬂip depends on the time instant at which the SET occurred in the ﬁrst clock cycle. Flips in the subsequent clock cycles can be understood completely based on logical propagation of the ﬂip in the second cycle which occurs on the clock edge.

Since we are interested in evaluating the accuracy of the single bit-ﬂip model, we focus on the likelihood of multiple register ﬂips. The ones caused directly as a result of the SET are denoted by   $\mathrm{"N F_{m}}^{\bullet}$  ’,   $\mathrm{^\mathrm{{*}}F_{m}F^{\circ}}$   and   $\mathbf{\thereforeF}_{\mathrm{m}}\mathbf{N}^{\prime}$  . The multiple ﬂip caused due to the propagation of the previous ﬂip is denoted by   $\mathrm{^\circF_{m}}^{\circ}$  ’, which will be anyway captured by modeling the ﬁrst ﬂip using the traditional single bit-ﬂip model. So, the multiple

![Particlestrike  Strike on a gate   Strike on aregister  \*k-+1"  77   MF   FM   FF   77   MF   F7   FF  MF   FN   FF   MF   FN   FF.  FF   FF  Multiple  fiips  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/935a841f-fdfd-4be2-af3e-719b200b43f0/935a841f-fdfd-4be2-af3e-719b200b43f0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=3b66089fbf11d547e76257af29ab8b8d25a74a2c)
Figure 3. A systematic notation for the possible error (SEU) outcomes caused due to an SET in a logic circuit

ﬂips in this case are not a direct result of the SET and we do not consider this in our experiments.

## III. S IMULATION SETUP 

The energy of secondary ions is typically known to range from 1 to 10MeV [18], [19]. The SET is represented as a current that is injected at the drain of a transistor [20], [21], which is positive-going for PMOS and negative for NMOS by convention. We use the double exponential glitch model, which has a fast rise time (attributed to the drift process) and a slow decay/fall time (attributed to the diffusion process of charge collection). Further, the magnitude of current for an NMOS is reported to be nearly three times that of PMOS in [3]. A ﬁxed glitch is used in our experiments. We use the scaling trends presented in [22] to arrive at the glitch height and width for the technology we simulate. Scaling trends presented in [23] indicate a glitch height of nearly 2mA at 180nm and nearly 1mA for 65nm for an NMOS transistor at 5MeV. Glitch width for these technologies is nearly 130ps at 5MeV [23]. Although the height and width of the SET depends on several factors such as the particle energy, width of the logic gate etc, these magnitudes are a reasonable assumption for a preliminary analysis. We also assume that the probability of an SET affecting a drain of a transistor is proportional to its area, which means that, larger the area of the drain, higher is the chance of it getting affected.

Each circuit that we perform our experiment on, is described as a Verilog or VHDL netlist (RTL). The circuit is implemented to layout using synthesis and placement-route (PNR) tools. The post-layout Verilog and circuit netlist are then extracted. We simulate the post-layout Verilog netlist with a representative test-bench using the  ModelSim  simulator and store the input/output values of all the ﬂip-ﬂops (registers). These are called as the reference values. From the post-layout circuit netlist, we generate ‘sample circuit simulation decks’ by picking a random clock cycle (k) for simulation, selecting a random drain (d) to inject the SET and selecting a random time instant (t) in the clock cycle to inject the SET.

The sample circuit is simulated for three clock cycles as shown in Figure 2 and the register outputs are recorded at two clock instants:   $\mathbf{\epsilon}_{\mathbf{k}},$   and   ${\bf\Psi}^{\bullet}\mathrm{k}{\bf+}\mathrm{l}\,^{\bullet}$  . We use the Ngspice or Hspice circuit simulators to perform our simulations. In the (k-1) th   clock cycle, the input registers of the circuit netlist are initialized with the corresponding input values obtained from the RTL reference values for that clock cycle. In the  $\mathbf{k}^{\mathrm{th}}$    clock cycle, we inject the SET at a random point in time (t) in the clock cycle. Inputs to the circuit change at the falling edge of the clock cycle k, so that there is sufﬁcient setup time. We note the register outputs at the rising edges of clock cycles    $k$  and    $k+1$  . The register values from the SET injected circuit simulation are compared with the corresponding reference values from the fault-free RTL simulation. Differences between the sampled values in the circuit simulation and the reference values are recorded as bit-ﬂips in the respective clock cycles.

We generate several sample simulation decks with different    $(d,k,t)$   values. The average number of sample circuit simulations run for each circuit was about 4000. We ran these simulations in parallel using GNU Parallel on a high performance computing cluster in Centre for Development of Advanced Computing (CDAC) Pune, India, which utilizes multiple cores. The time taken to run these many simulations for each circuit was on an average about 1 to 2 hours.

We extract the bit-ﬂip information from each simulation and then classify these ﬂips into one of the SEU outcomes described in Figure 3. We continue to generate the circuit samples until the standard error (  $.\frac{S t a n d a r d\;d e v i a t i o n}{\sqrt{N}\quad-})$  ) is reduced to less than   $10\%$   of the value of the estimate. The probabilities obtained from this Monte Carlo sampling experiment fall within the   $95\%$   conﬁdence interval. The experimental setup is brieﬂy described in Algorithm 1. This entire process is automated using a set of python and perl scripts.

## IV. R ESULTS 

We perform our experiments on  ISCAS’85  (c432 etc) , ISCAS’89  (s344 etc) and  ITC’99  (b01 etc) benchmark circuits in   $180\mathrm{nm}$   and 65nm technologies. Flip-ﬂops (registers) are added to the inputs and outputs of the combinational circuits of the  ISCAS’85  benchmarks. Clock frequency for each circuit is set to the maximum operable frequency of the post-layout netlist, which is determined by post-layout timing analysis. It typically ranged from 100MHz to 500MHz. We calculate the probability of a ‘gate-strike’ and ‘register-strike’ depending on whether the SET was injected on a gate or a register. Further, we classify the bit-ﬂips into one of the SEU outcomes described in Figure 3.

## A. Probability that an error occurs 

We evaluated the probabilities of all the SEU outcomes under the condition that the SET occurs at a register (‘register strike’) and the SET occurs at a gate (‘gate strike’) separately in [17]. In both ‘register strike’ and ‘gate strike’ cases, we ﬁnd that,    $P_{N N}$  , that is, probability of no-ﬂips is dominant, that is, the SET causes no ﬂips. The probability    $1-P_{N N}$  indicates the probability that a ﬂip or an error occurred. This is plotted in Figure 4. The ﬂip probability for register-strike

Algorithm 1  Experimental setup to perform the circuit level characterization of the impact of an SET

## Input:  Verilog/VHDL description of circuit 

Perform Synthesis of the Verilog/VHDL description   •    Perform placement and route of the resulting Synthesis   • output    Extract the post-layout Verilog and SPICE netlists   •    Simulate the post-layout Verilog netlist using ModelSim   • for 10000 clock cycles    Store the input and output values of all ﬂip-ﬂops at every   • clock cycle    for  (Number of simulations)   • {    Create a sample simulation netlist from the post-layout   • SPICE netlist: { –  Pick a random drain    $d$   of a transistor at which the SET will be injected –  Pick a random clock cycle    $k$   from the reference trace for simulation –  Pick the inputs to the sample netlist from the chosen clock cycle  $k$  –  Inject the SET at a random time instant  t  in the selected clock cycle }   •  Simulate the sample SPICE netlist with parameters    $d,k,t$  for 3 clock cycles    Store the output values of all ﬂip-ﬂops at the 2nd and 3rd   • clock edges    Compare the outputs from SPICE netlist with that of the   • Verilog netlist    Note any discrepancy in the output as a bit-ﬂip   •    Evaluate the conditional probability of multiple ﬂips   • given at least one error occurred    Simulations are run to reach a   $95\%$   conﬁdence interval   • }  Calculate the statistics of all SEU outcomes

Output:

cases is substantially greater (nearly 10x greater) than that for the gate-strike cases. This indicates that, when an SET occurs on a register, it is more likely to cause an error, than one at a gate. Protecting the ﬂip-ﬂops or having robust ﬂip-ﬂop designs can help reduce this ﬂip probability. Further, the ﬂip probabilities are higher in the 65nm technology, which means that, as technology scales, the likelihood of an error increases.

## B. Probability of multiple register ﬂips given an erroneous outcome 

In our previous work [17], we reported the multiple ﬂip probability    $P(N F_{m}|N F)$  . However, we ﬁnd that the following estimate is more interesting. Given that an error or a ﬂip occurred due to an SET, that is, one of these cases occurred $N F^{*}$  ,  $F^{*}N$   or    $F F^{*} $  (where    $F^{*} $  means one or more ﬂips), what is the likelihood that the ﬁrst error event caused by the SET affects multiple registers? There are two possibilities:

![0.35  .15  0.05  Testcircuits  180nm(gatestrike)   ←65nm（gatestrike)  180nm(flip-flopstrike)  ←65nm（flip-flopstrike)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e4d92a21-0598-42e1-9a84-a1a22de48f05/e4d92a21-0598-42e1-9a84-a1a22de48f05.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=d58e143654a9f627e9181155d9018d0953e8eb83)
Figure 4.  Probability of at least one bit-ﬂip for ‘gate-strike’ and ‘registerstrike’ scenarios

•  The ﬁrst error event occurs at cycle    $k+1$   and consists of multiple registers being in error, that is,    $\begin{array}{r l}{P_{m}}&{{}=}\end{array}$   $P(N F_{m}|a t l e a s t\,o n e\,f l i p)$  , where  $P(a t l e a s t\,o n e\,f l i p)$   is  $1-P(N N)$  . •  The ﬁrst error event occurs at cycle    $k$   and consists of multiple registers being in error, that is,  $P(F_{m}N|a t l e a s t\,o n e\,f l i p)$  . There is another scenario where the multiple ﬂips leads to ﬂip in the next cycle: P ( F m F | atleast one flip ) .

We do not consider the probability  $P(F F_{m}|a t l e a s t\,o n e\,f l i p)$  , because the multiple ﬂips in cycle  $k+1$   are caused due to the propagation of the ﬁrst ﬂip, which will be anyway captured by modeling the ﬁrst ﬂip using the traditional single bit-ﬂip model. So, the multiple ﬂips in this case are not a direct result of the SET.

Amongst the two cases mentioned above, we did not come across the scenario of    $P(F_{m}N|a t l e a s t\,o n e\,f l i p)$   or  $P(F_{m}F|a t l e a s t\,o n e\,f l i p)$   in our experiments, that is, multiple ﬂips in clock cycle ‘k’. Hence, we report the ﬁrst probability:  $P_{m}\,=\,P(N F_{m}|a t l e a s t\,o n e\,f l i p)$  . This is calculated as follows for both the gate-strike and register-strike (denoted by reg-strike in the equation) cases put together:

$$P_{m}=\frac{N o.\;o f\;(N F_{m})_{G a t e-s t r i k e}+N o.\;o f\;(N F_{m})_{r e g-s t r i k e}}{(N o.\;o f\;c a s e s\;w i t h\;a t l e a s t\;o n e\;f l i p)_{g a t e+r e g-s t r i k e}}$$
In other words, we calculate

$$P_{m}=\frac{N o.\;o f\;(N F_{m})_{G a t e-s t r i k e}+N o.\;o f\;(N F_{m})_{r e g-s t r i k e}}{(N o.\;o f\;N F,\;F N\;o r\;F F)_{g a t e+r e g-s t r i k e}}$$
For instance, if we ran 5000 simulations, out of which there were 1000 cases in which at least one error occurred (this can include  NF ,  FN  or    $F F$   across gate and register strikes), out of which, say 100 cases had multiple errors   $(N F_{m})$  , we calculate  $P_{m}$   as 100/1000. This probability is shown in Table

I for the benchmark circuits, across both register and gate strikes.

Table I P ROBABILITY OF MULTIPLE BIT FLIPS GIVEN THAT AT LEAST ONE ERROR OCCURRED ACROSS ALL STRIKES  (‘-’  INDICATES NO MULTIPLE ERROR EVENTS WERE OBSERVED )

|Example|        Pm-                ‘gate and                register                strike"                180nm      |        Pm-                ‘gate and                register                strike'                65mm      |
|---|---|---|
|c432|0.006|0.035|
|c499|0.003|0.016|
|c880||0.001|
|c1355|0.003|0.007|
|c1908|0.003|0.037|
|boi||0.02|
|b03|0.005|0.007|
|b04||0.03|
|b06|0.042|0.05|
|b09|0.005|0.044|
|bio|0.007|0.06|
|bii||0.036|
|b13||0.038|
|s344||0.02|
|s820||0.081|
|s1196||0.014|
|s1238||0.022|
|S1423||0.028|
|        3:8                decoder      |0.006|0.014|
|8-bit LFSR|0.007|0.018|


From Table I, we see that the maximum probability of multiple ﬂips    $P_{m}$   that was observed in the circuits we simulated, across both register and gate strikes was  $8\%$  . This probability is likely to depend on several factors such as the number of ﬂip-ﬂops, presence of balanced paths, logic depth, logic gates, input combinations and so on. Although   $8\%$   seems low, it can still have a signiﬁcant impact on error detection and correction schemes.

C. The contribution of gate strikes and register strikes to multiple register ﬂips

In this section, we analyze our results further to understand the role of gate-strikes and register-strikes independently on the multiple ﬂip probability. In other words, we address the following question. Given that an error occurred due to a strike on a logic gate, what is the probability that it was a multiple ﬂip? This is denoted by    $P_{G M}$  . Similarly, we calculate the multiple ﬂip probability    $P_{R M}$   given that an error was caused due to a register strike. We calculate    $P_{G M}$   and    $P_{R M}$  respectively as follows:

$$P_{G M}=\frac{N u m b e r\;o f\;(N F_{m})_{g a t e-s t r i k e}}{(N u m b e r\;o f\;N F,\;F N\;o r\;F F)_{g a t e-s t r i k e}}$$
(3)

$$P_{R M}=\frac{N u m b e r\;o f\;(N F_{m})_{r e g i s t e r-s t r i k e}}{(N u m b e r\;o f\;N F,\;F N\;o r\;F F)_{r e g i s t e r-s t r i k e}}$$
(4)

In these equations, we should note that, the denominator in both the fractions is the total number of cases which had

erroneous outcomes (ﬂips). For the gate strike scenario, when an SET occurs on a logic gate in clock cycle ‘k’, the register ﬂip is most likely to occur due to the propagation of the SET and hence, the ﬂip is likely to occur in the subsequent clock cycle   ${\mathrm{*}}_{\mathrm{k+1}},$  . Thus, a major contributor of the erroneous outcomes is the ‘NF’ scenario. On the other hand, for the register strike case, an SET is more likely to cause an error in the same clock cycle and hence errors are mainly contributed by the ‘FN’ and ‘FF’ scenarios. So,    $P_{F N}$   and    $P_{F F}$   are dominant for register strike cases and    $P_{N F}$   is dominant for gate strike scenarios. From Table II, we ﬁnd that    $P_{G M}$   is signiﬁcantly greater than    $P_{R M}$   and its value is found to be a maximum of   $50\%$  . This is mainly because of two reasons:

When an SET occurs on a register, •

–  The probability of a ﬂip or an error occurring is high (high probabilities of an    $F F$   or an    $F N$  ) as compared to the SET occurring on a gate (Figure 4). The ﬂip probability for register-strike cases is found to be nearly 10x greater than that for the gate-strike cases. This increases the denominator in equation 4 and results in a small value for    $P_{R M}$  . –  The probability of an    $N F$   scenario is small, as compared to the  $F N$   and    $F F$   scenarios for a register strike. Hence    $N F_{m}$   scenarios are also less leading to a small value in the numerator in equation 4. This again leads to low value of    $P_{R M}$  .

When an SET occurs on a logic gate,   • –  The probability of a ﬂip is low (low probabilities of an  $F F$   or an  $F N$  ) as compared to the SET occurring on a register as already observed in Figure 4. This decreases the denominator in equation 3. –  The major contributor of ﬂips for gate strikes is  $N F$  . Hence  $N F_{m}$   scenarios are also high, as compared to the register strike cases, leading to a large value in the numerator in equation 3. These lead to a high value of    $P_{G M}$  .

To summarize, given that there is an error, the probability of multiple errors in the case of register-strike cases is less: about  $2\%$  , where as they are signiﬁcant in the gate-strike cases and can be up to   $50\%$  . Robust ﬂip-ﬂops can be designed to eliminate the errors due to ‘register strikes’. But they will not be able to eliminate the errors caused due to the propagation of the SETs from the logic gate. Thus, the key message is that, in a circuit design with robust ﬂip-ﬂops, although we can eliminate the ﬂips due to ‘register strike’ cases, out of the remaining ﬂips which are going to be due to ‘gate strikes’, multiple ﬂips will be extremely likely. So, alternate methods such as delay capture ﬂip-ﬂop designs or introducing uneven path delays to registers may be needed to prevent multiple errors due to strikes on logic gates.

## V. S AMPLE WAVEFORMS INDICATING THE REDUCTION OF ELECTRICAL MASKING WITH SCALING 

There are three inherent masking phenomena in logic circuits:

![NAND   NAND  (strike)  Outputs of the gates are plotted  3.7226n  65  nmn  Glitch  4.2746n  1.8000  180   1.8000  0.00  1.8600  Glitch  599.40  543.09m  Glitch has almost died down  here  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/524b0666-cbbe-48f9-8ee6-856b0c872d95/524b0666-cbbe-48f9-8ee6-856b0c872d95.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=48f2ed3e96f1b568f3565cc812660ed060aa52c3)
Figure 5. 180nm vs 65nm- propagation of an SET. The outputs of three gates are shown against the clock.

Table II P ROBABILITY OF MULTIPLE BIT FLIPS GIVEN THAT AT LEAST ONE ERROR OCCURRED . G ATE STRIKES AND REGISTER STRIKES ARE PRESENTED SEPARATELY . (‘-’  INDICATES NO MULTIPLE ERROR EVENTS WERE OBSERVED )

|Example|        PGM-                'gate,                strike”                180nm      |        PGM-                ‘gate                strike"                65mm      |        PRM-                ‘register                strike”                180nm      |        PRM-                'register                strike"                65nm      |
|---|---|---|---|---|
|c432|0.4|0S||0.002|
|c499|0.11|0.2|||
|c880|||||
|c1355|0.33|0.2|||
|c1908|0.067|0.25||0.008|
|boi||0.035||0.016|
|b03|0.12|0.042||0.004|
|b04||0.172|||
|bo6|0.288|0.35||0.003|
|b09|0.08|0.36||0.003|
|b1o|0.058|0.4|||
|bi1||0.12||0.0012|
|b13||0.34|||
|s344||0.07||0.012|
|s820||0.12|||
|s1196||0.045|||
|s1238||0.08|||
|s1423||0.27||0.003|
|3:8decoder|0.107|0.27|0.001||
|8-bitLFSR|0.073|0.17|||


1) Logical masking, in which, the type of logic gate and its input combinations could mask the propagation of the SET/glitch.   2) Electrical masking, in which the SET can get attenuated as it passes through the logic stages.   3) Latching window masking, in which, the SET can get masked if it does not fall within the setup/hold times of the capturing latch.

As the technology scales, the impact of these masking phenomena reduces and hence the SER in logic circuits tends to

increase [3], [4], [5]. In Figure 5, we show an example of an SET propagating through a section of our 3:8 decoder. In the case of   $180\mathrm{nm}$   circuits, the glitch dies down by the time it propagates through two gates, where as the glitch propagates through the three gates in 65nm. This is because, the gates in 65nm are smaller and faster and hence the glitch does not die down. Thus, in our examples, we can attribute the increase in ﬂip probability with scaling, to the reduction in electrical masking.

## VI. I MPACT OF THE  SET  WIDTH ON MULTIPLE FLIP PROBABILITY 

For a given particle energy, is there a minimum SET width after which we start observing errors and in particular multiple errors? Although it seems obvious that the width of the SET will impact the probability of SEU outcomes, we quantify the extent to which the SET width has an impact on multiple ﬂips. We simulate a subset of benchmark circuits in 65nm technology with varying SET pulse widths- 130ps, 90ps and 50ps. In Tables III and IV, we present the probability of noﬂips   $(P_{N N})$   for register strikes and gate strikes respectively, for varying pulse widths. We note that the probability of “noﬂip” increases with reduction in SET width in both the cases. In other words, the probability of a ﬂip (P(1-NN)) reduces by a maximum of   $10\%$   as the SET width reduces from 130ps to 50ps. In Table V, we present the probability of multiple ﬂips    $P_{m}$   across both register and gate strikes. We see that the probability of multiple ﬂips also reduces as the SET width is reduced. In one of the circuits, the multiple ﬂip probability dropped to zero, thus eliminating all multiple ﬂips. This could be attributed to the fact that, an SET with a smaller pulse width has a lower chance of getting captured in a ﬂip-ﬂop (less chance of overlap within the setup-hold window), thus reducing the probability of a ﬂip and in turn multiple ﬂips.

Table III P ROBABILITY OF NO FLIP  P(NN)  FOR VARYING PULSE WIDTHS ,  FOR ‘ REGISTER STRIKE ’  CASES

|Example|        PNN                130ps      |        PNN                90ps      |        PNN                Sops      |
|---|---|---|---|
|c432|0.75|0.775|0.797|
|bi|0.712|0.78|0.78|
|b03|0.754|0.78|0.799|
|bo6|0.75|0.766|0.8|
|bo9|0.766|0.8|0.819|
|bio|0.77|0.78|0.81|
|S344|0.714|0.762|0.81|
|s820|0.75|0.82|0.83|
|s1423|0.743|0.78|0.8|
|3:8decoder|0.76|0.775|0.797|


RTL simulation and calculate the SEU probabilities. Given an erroneous outcome, we calculate the probability that multiple registers are in error, across both gate and register strikes. This probability  $P_{m}$   is presented in Table VI for a subset of circuits in   $65\mathrm{nm}$   technology. We see that the increase in multiple ﬂip probability is substantial for most of the circuits and is of the factor of   $2\mathbf{X}$   on an average as compared to the scenario where a single SET was injected. Thus, given that a particle strike is quite likely to create two SETs in a layout, especially as technology scales, it is now even more important to take appropriate circuit/layout measures to reduce the probability of multiple ﬂips.

Table IV P ROBABILITY OF NO FLIP  P(NN)  FOR VARYING PULSE WIDTHS ,  FOR ‘ GATE STRIKE ’  CASES

|Example|        PNN                130ps      |        PNN                90ps      |        RNN                Sops      |
|---|---|---|---|
|c432|0.98|0.98|0.98|
|bi|0.973|0.983|0.985|
|bo3|0.975|0.983|0.988|
|bo6|0.977|0.981|0.99|
|b09|0.971|0.99|0.991|
|bio|0.978|0.985|0.993|
|S344|0.978|0.986|0.994|
|s820|0.991|0.993|0.996|
|s1423|0.981|0.994|0.995|
|3:8decoder|0.982|0.991|0.992|


Table VIPROBABILITY OF MULTIPLE BIT FLIPS GIVEN THAT AT LEAST ONE ERROROCCURRED ACROSS GATE AND REGISTER STRIKES. RESULTS OBTAINEDWITH TWO SETS ARE COMPARED WITH THOSE WITH ONE SET FOR THE65NM IMPLEMENTATIONS

|Example|        Pm-                65nm                withone                SET      |        Pm-                65nm                withtwo                SETs      |        Factor                increase      |
|---|---|---|---|
|C432|0.035|0.04|1.14|
|c880|0.001|0.009||
|c1355|0.007|0.024|3.42|
|boi|0.02|0.024|1-2|
|bo3|0.007|0.021||
|b04|0.03|0.057|1.9|
|bio|0.06|0.0674|1.12|
|611|0.036|0.05|1.38|
|613|0.038|0.072|1.89|
|s344|0.02|0.054|2.2|
|s1196|0.014|0.031|2.21|
|s1238|0.022|0.057|2.59|
|3:8decoder|0.014|0.022|1.57|


Table VPROBABILITY OF MULTIPLE BIT FLIPS GIVEN THAT AT LEAST ONE ERROROCCURRED- FOR VARYING SET WIDTHS.

|Example|Pm-130ps|Pm-90ps|Pm-50ps|
|---|---|---|---|
|c432|3.5%|2.39%|1.8%|
|boi|29%0|1.36%|1.3%|
|b03|0.7%|0.59%|0.3%|
|bo6||3.5%|0.8%|
|b09|4.4%|1.1%|0.35%|
|b1o|6%%|4.1%|2.3%|
|s344|29%0|0.4%|0.05%|
|s820|8.1%|1.9%|0%|
|s1423|2.8%|1.8%|1.01%|
|3:8decoder|1.4%|0.7%|0.6%|


## VII. I MPACT OF TWO  SET S ON MULTIPLE FLIP PROBABILITY 

Typically, a particle strike will affect more than one transistor or in other words, result in more than one SET in a logic circuit especially as technology scales [24], [18]. We quantify the factor by which the multiple ﬂip probability would increase in such a scenario. So, we alter our existing simulation set up and inject two SETs instead of one. The gate/register on which the ﬁrst SET is injected is chosen the same way as earlier (the larger the area of the gate, higher is the probability of it getting chosen). We then inspect the layout of each circuit and inject the second SET on the gate/register which is located the closest to the originally selected gate/register, at the same time. We compare the register outputs from the SET injected SPICE simulation with that of the fault-free

Further, it is also likely that two SETs generated in a circuit can merge and produce an SET whose width is large, increasing its probability of getting captured in a ﬂip-ﬂop. We demonstrate this using a simulation of a 3:8 decoder example shown in Figure 6(a). The highlighted gates U19 and U26 connect to U24 and ﬂip-ﬂop reg7. From the waveforms in Figure 6 (b), we observe that the SETs on U19 and U26 merge to produce a wider SET on U24. This can increase the probability of the ﬂip-ﬂop capturing the SET. So, existing error tolerant latch designs may need to be revisited to handle such scenarios.

## VIII. C ONCLUSION AND DISCUSSION 

We have performed a detailed characterization of the impact of an SET on a logic circuit to quantify the extent to which the single bit-ﬂip model is realistic. We note that the impact of an SET can be completely understood by viewing the outcomes across two clock cycles. Overall, up to  $8\%$   of the erroneous outcomes resulted in multiple bit-ﬂips. Amongst the erroneous outcomes, the probability of multiple bit ﬂips (caused as a direct result of the SET) for gate strike cases was substantial and went up to   $50\%$  , where as those for register strike cases was just about  $2\%$  . This implies that, even if were to eliminate the ﬂips due to register strikes using robust ﬂipﬂop designs, out of the remaining ﬂips which will be due to

![S_GSS  U19  （a  SGS  U26  U24   5_GS  utput_dee[7:0]  HSS5_GS.  HSG5_CS,   S66_GS_A0122  65_GS   reg7  (V) : 1(8)  v(u24:2)  U24  C.C-(V) : 1(≤)  2_0  v[u26z)  U26  ) : 1(≤)  20   v[u-19:z)  U19  -二_0 .  (V) : 1(≤)  vIcIk  05   CK  00  1CS3  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d93be55a-2729-440a-b872-f92df612a016/d93be55a-2729-440a-b872-f92df612a016.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=f2729d0be9c392effdd3c34610c866d8524e36b1)
Figure 6. (a) Schematic of 3:8 decoder which shows U19 and U26 connecting to U24 and reg7 (b) SETs on U26 and U19 merge to produce a wider SET on U24.

gate strikes, a large fraction will be multiple ﬂips. Thus, there is a need to focus on circuit techniques to eliminate these type of errors. Further, we saw a substantial increase, a factor of 2x on an average, in the multiple ﬂip probability, when an SET affected two nearby transistors. We also showed that two SETs from nearby logic gates can merge and produce an SET of larger width at the input of a ﬂip-ﬂop, thus increasing its likelihood of getting captured. So, existing error tolerant latch designs need to be revisited to handle such scenarios. To sum up, multiple SETs are quite likely and will have serious implications on circuit reliability unless efﬁcient circuit/layout level approaches are implemented.

## R EFERENCES 

[1] J. Ziegler, “Terrestrial cosmic ray intensities,”  IBM Journal of Research and Development , vol. 42, pp. 117–140, Jan 1998.   [2] E. Normand, “Single event upset at ground level,”  Nuclear Science, IEEE Transactions on , vol. 43, no. 6, pp. 2742–2750, 1996.   [3] R. Ramanarayanan, V. Degalahal, R. Krishnan, J. Kim, V. Narayanan, Y. Xie, M. Irwin, and K. Unlu, “Modeling soft errors at the device and logic levels for combinational circuits,”  Dependable and Secure Computing, IEEE Transactions on , vol. 6, no. 3, pp. 202–216, 2009.   [4] M. Fazeli, S. Ahmadian, S. Miremadi, H. Asadi, and M. Tahoori, “Soft error rate estimation of digital circuits in the presence of multiple event transients (mets),” in  Design, Automation Test in Europe Conference Exhibition (DATE), 2011 , pp. 1–6, 2011.   [5] J. Hayes, I. Polian, and B. Becker, “An analysis framework for transienterror tolerance,” in  VLSI Test Symposium, 2007. 25th IEEE , pp. 249–255, 2007.   [6] P. Shivakumar, M. Kistler, S. Keckler, D. Burger, and L. Alvisi, “Modeling the effect of technology trends on the soft error rate of combinational logic,” in  Dependable Systems and Networks, 2002. DSN 2002. Proceedings. International Conference on , pp. 389–398, 2002.   [7] S. Mukherjee, J. Emer, and S. Reinhardt, “The soft error problem: an architectural perspective,” in  High-Performance Computer Architecture, 2005. HPCA-11. 11th International Symposium on , pp. 243–247, 2005.   [8] N. Wang, J. Quek, T. Rafacz, and S. Patel, “Characterizing the effects of transient faults on a high-performance processor pipeline,” in  Dependable Systems and Networks, 2004 International Conference on , pp. 61– 70, 2004.   [9] N. J. Wang, A. Mahesri, and S. J. Patel, “Examining ace analysis reliability estimates using fault-injection,”  SIGARCH Comput. Archit. News , vol. 35, pp. 460–469, June 2007.   [10] N. Wang and S. Patel, “Restore: Symptom-based soft error detection in microprocessors,”  Dependable and Secure Computing, IEEE Transactions on , vol. 3, pp. 188–201, July 2006.   [11] J. Blome, S. Mahlke, D. Bradley, and K. Flautner, “A microarchitectural analysis of soft error propagation in a production-level embedded microprocessor,” in  In Proceedings of the First Workshop on Architecture Reliability , 2005.   [12] H. Cha, E. Rudnick, J. Patel, R. Iyer, and G. Choi, “A gate-level simulation environment for alpha-particle-induced transient faults,”  Computers, IEEE Transactions on , vol. 45, no. 11, pp. 1248–1256, 1996.   [13] G. Saggese, N. Wang, Z. Kalbarczyk, S. Patel, and R. Iyer, “An experimental study of soft errors in microprocessors,”  Micro, IEEE , vol. 25, no. 6, pp. 30–39, 2005.   [14] H. Asadi and M. Tahoori, “Soft error derating computation in sequential circuits,” in  Computer-Aided Design, 2006. ICCAD ’06. IEEE/ACM International Conference on , pp. 497–501, 2006.   [15] N. Miskov-Zivanov and D. Marculescu, “Circuit reliability analysis using symbolic techniques,”  Computer-Aided Design of Integrated Circuits and Systems, IEEE Transactions on , vol. 25, no. 12, pp. 2638–2649, 2006.   [16] N. Miskov-Zivanov and D. Marculescu, “Mars-c: modeling and reduction of soft errors in combinational circuits,” in  Design Automation Conference, 2006 43rd ACM/IEEE , pp. 767–772, 2006.   [17] N. P. Rao and M. P. Desai, “A detailed characterization of errors in logic circuits due to single-event transients,” in  Digital System Design (DSD), 2015 Euromicro Conference on , pp. 714–721, Aug 2015.   [18] O. Amusan, A. Steinberg, A. Witulski, B. Bhuva, J. Black, M. Baze, and L. Massengill, “Single event upsets in a 130 nm hardened latch design due to charge sharing,” in  Reliability physics symposium, 2007. proceedings. 45th annual. ieee international , pp. 306–311, April 2007.   [19] R. Baumann, “Radiation-induced soft errors in advanced semiconductor technologies,”  Device and Materials Reliability, IEEE Transactions on , vol. 5, pp. 305–316, Sept 2005.   [20] Q. Zhou and K. Mohanram, “Gate sizing to radiation harden combinational logic,”  Computer-Aided Design of Integrated Circuits and Systems, IEEE Transactions on , vol. 25, no. 1, pp. 155–166, 2006.   [21] E. Neto, I. Ribeiro, M. Vieira, G. Wirth, and F. Kastensmidt, “Using bulk built-in current sensors to detect soft errors,”  Micro, IEEE , vol. 26, no. 5, pp. 10–18, 2006.   [22] P. Dodd, M. Shaneyfelt, J. Felix, and J. Schwank, “Production and propagation of single-event transients in high-speed digital logic ics,” Nuclear Science, IEEE Transactions on , vol. 51, pp. 3278–3284, Dec 2004.   [23] P. Dodd, M. Shaneyfelt, J. Felix, and J. Schwank, “Production and propagation of single-event transients in high-speed digital logic ics,” Nuclear Science, IEEE Transactions on , vol. 51, pp. 3278–3284, Dec 2004.   [24] N. Seifert, B. Gill, V. Zia, M. Zhang, and V. Ambrose, “On the scalability of redundancy based ser mitigation schemes,” in  Integrated Circuit Design and Technology, 2007. ICICDT ’07. IEEE International Conference on , pp. 1–9, May 2007.

