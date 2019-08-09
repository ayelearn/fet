The following text has been accessed from https://en.wikipedia.org/wiki/Information_theory at Fri Aug 9 03:44:40 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Information theory ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with Information_science.
Information theory
[Binaryerasurechannel.png]
    * Entropy
    * Differential_entropy
    * Conditional_entropy
    * Joint_entropy
    * Mutual_information
    * Conditional_mutual_information
    * Relative_entropy
    * Entropy_rate
    * Asymptotic_equipartition_property
    * Rateâdistortion_theory
    * Shannon's_source_coding_theorem
    * Channel_capacity
    * Noisy-channel_coding_theorem
    * ShannonâHartley_theorem
    * v
    * t
    * e
Information theory studies the quantification, storage, and communication of
information. It was originally proposed by Claude_Shannon in 1948 to find
fundamental limits on signal_processing and communication operations such as
data_compression, in a landmark paper titled "A_Mathematical_Theory_of
Communication". Applications of fundamental topics of information theory
include lossless_data_compression (e.g. ZIP_files), lossy_data_compression
(e.g. MP3s and JPEGs), and channel_coding (e.g. for DSL). Its impact has been
crucial to the success of the Voyager missions to deep space, the invention of
the compact_disc, the feasibility of mobile_phones, the development of the
Internet, the study of linguistics and of human perception, the understanding
of black_holes, and numerous other fields.
A key measure in information theory is "entropy". Entropy quantifies the amount
of uncertainty involved in the value of a random_variable or the outcome of a
random_process. For example, identifying the outcome of a fair coin_flip (with
two equally likely outcomes) provides less information (lower entropy) than
specifying the outcome from a roll of a die (with six equally likely outcomes).
Some other important measures in information theory are mutual_information,
channel_capacity, error_exponents, and relative_entropy.
The field is at the intersection of mathematics, statistics, computer_science,
physics, neurobiology, information_engineering, and electrical_engineering. The
theory has also found applications in other areas, including statistical
inference, natural_language_processing, cryptography, neurobiology,[1] human
vision,[2] the evolution[3] and function[4] of molecular codes
(bioinformatics), model_selection in statistics,[5] thermal_physics,[6] quantum
computing, linguistics, plagiarism_detection,[7] pattern_recognition, and
anomaly_detection.[8] Important sub-fields of information theory include source
coding, channel_coding, algorithmic_complexity_theory, algorithmic_information
theory, information-theoretic_security, Grey_system_theory and measures of
information.
⁰
***** Contents *****
    * 1_Overview
    * 2_Historical_background
    * 3_Quantities_of_information
          o 3.1_Entropy_of_an_information_source
          o 3.2_Joint_entropy
          o 3.3_Conditional_entropy_(equivocation)
          o 3.4_Mutual_information_(transinformation)
          o 3.5_KullbackâLeibler_divergence_(information_gain)
          o 3.6_Other_quantities
    * 4_Coding_theory
          o 4.1_Source_theory
                # 4.1.1_Rate
          o 4.2_Channel_capacity
                # 4.2.1_Capacity_of_particular_channel_models
    * 5_Applications_to_other_fields
          o 5.1_Intelligence_uses_and_secrecy_applications
          o 5.2_Pseudorandom_number_generation
          o 5.3_Seismic_exploration
          o 5.4_Semiotics
          o 5.5_Miscellaneous_applications
    * 6_See_also
          o 6.1_Applications
          o 6.2_History
          o 6.3_Theory
          o 6.4_Concepts
    * 7_References
          o 7.1_The_classic_work
          o 7.2_Other_journal_articles
          o 7.3_Textbooks_on_information_theory
          o 7.4_Other_books
          o 7.5_MOOC_on_information_theory
    * 8_External_links
***** Overview[edit] *****
Information theory studies the transmission, processing, extraction, and
utilization of information. Abstractly, information can be thought of as the
resolution of uncertainty. In the case of communication of information over a
noisy channel, this abstract concept was made concrete in 1948 by Claude
Shannon in his paper "A_Mathematical_Theory_of_Communication", in which
"information" is thought of as a set of possible messages, where the goal is to
send these messages over a noisy channel, and then to have the receiver
reconstruct the message with low probability of error, in spite of the channel
noise. Shannon's main result, the noisy-channel_coding_theorem showed that, in
the limit of many channel uses, the rate of information that is asymptotically
achievable is equal to the channel_capacity, a quantity dependent merely on the
statistics of the channel over which the messages are sent.[1]
Information theory is closely associated with a collection of pure and applied
disciplines that have been investigated and reduced to engineering practice
under a variety of rubrics throughout the world over the past half century or
more: adaptive_systems, anticipatory_systems, artificial_intelligence, complex
systems, complexity_science, cybernetics, informatics, machine_learning, along
with systems_sciences of many descriptions. Information theory is a broad and
deep mathematical theory, with equally broad and deep applications, amongst
which is the vital field of coding_theory.
Coding theory is concerned with finding explicit methods, called codes, for
increasing the efficiency and reducing the error rate of data communication
over noisy channels to near the channel_capacity. These codes can be roughly
subdivided into data_compression (source coding) and error-correction (channel
coding) techniques. In the latter case, it took many years to find the methods
Shannon's work proved were possible.
A third class of information theory codes are cryptographic algorithms (both
codes and ciphers). Concepts, methods and results from coding theory and
information theory are widely used in cryptography and cryptanalysis. See the
article ban_(unit) for a historical application.
Information theory is also used in information_retrieval, intelligence
gathering, gambling, statistics, and even in musical_composition.
***** Historical background[edit] *****
Main article: History_of_information_theory
The landmark event that established the discipline of information theory and
brought it to immediate worldwide attention was the publication of Claude_E.
Shannon's classic paper "A_Mathematical_Theory_of_Communication" in the Bell
System_Technical_Journal in July and October 1948.
Prior to this paper, limited information-theoretic ideas had been developed at
Bell_Labs, all implicitly assuming events of equal probability. Harry_Nyquist's
1924 paper, Certain Factors Affecting Telegraph Speed, contains a theoretical
section quantifying "intelligence" and the "line speed" at which it can be
transmitted by a communication system, giving the relation W = K log m
(recalling Boltzmann's_constant), where W is the speed of transmission of
intelligence, m is the number of different voltage levels to choose from at
each time step, and K is a constant. Ralph_Hartley's 1928 paper, Transmission
of Information, uses the word information as a measurable quantity, reflecting
the receiver's ability to distinguish one sequence_of_symbols from any other,
thus quantifying information as H = log Sn = n log S, where S was the number of
possible symbols, and n the number of symbols in a transmission. The unit of
information was therefore the decimal_digit, which has since sometimes been
called the hartley in his honor as a unit or scale or measure of information.
Alan_Turing in 1940 used similar ideas as part of the statistical analysis of
the breaking of the German second world war Enigma ciphers.
Much of the mathematics behind information theory with events of different
probabilities were developed for the field of thermodynamics by Ludwig
Boltzmann and J._Willard_Gibbs. Connections between information-theoretic
entropy and thermodynamic entropy, including the important contributions by
Rolf_Landauer in the 1960s, are explored in Entropy_in_thermodynamics_and
information_theory.
In Shannon's revolutionary and groundbreaking paper, the work for which had
been substantially completed at Bell Labs by the end of 1944, Shannon for the
first time introduced the qualitative and quantitative model of communication
as a statistical process underlying information theory, opening with the
assertion that
      "The fundamental problem of communication is that of reproducing at one
      point, either exactly or approximately, a message selected at another
      point."
With it came the ideas of
    * the information_entropy and redundancy of a source, and its relevance
      through the source_coding_theorem;
    * the mutual_information, and the channel_capacity of a noisy channel,
      including the promise of perfect loss-free communication given by the
      noisy-channel_coding_theorem;
    * the practical result of the ShannonâHartley_law for the channel
      capacity of a Gaussian_channel; as well as
    * the bitâa new way of seeing the most fundamental unit of information.
***** Quantities of information[edit] *****
Main article: Quantities_of_information
Information theory is based on probability_theory and statistics. Information
theory often concerns itself with measures of information of the distributions
associated with random variables. Important quantities of information are
entropy, a measure of information in a single random_variable, and mutual
information, a measure of information in common between two random variables.
The former quantity is a property of the probability distribution of a random
variable and gives a limit on the rate at which data generated by independent
samples with the given distribution can be reliably compressed. The latter is a
property of the joint distribution of two random variables, and is the maximum
rate of reliable communication across a noisy channel in the limit of long
block lengths, when the channel statistics are determined by the joint
distribution.
The choice of logarithmic base in the following formulae determines the unit of
information_entropy that is used. A common unit of information is the bit,
based on the binary_logarithm. Other units include the nat, which is based on
the natural_logarithm, and the decimal_digit, which is based on the common
logarithm.
In what follows, an expression of the form p log p is considered by convention
to be equal to zero whenever p = 0. This is justified because      lim  p
&#x2192; 0 +   p log &#x2061; p = 0   {\displaystyle \lim _{p\rightarrow
0+}p\log p=0}  [\lim _{p\rightarrow 0+}p\log p=0] for any logarithmic base.
**** Entropy of an information source[edit] ****
Based on the probability_mass_function of each source symbol to be
communicated, the Shannon entropy H, in units of bits (per symbol), is given by
         H = &#x2212;  &#x2211;  i    p  i    log  2   &#x2061; (  p  i   )
      {\displaystyle H=-\sum _{i}p_{i}\log _{2}(p_{i})}  [{\displaystyle H=-
      \sum _{i}p_{i}\log _{2}(p_{i})}]
where pi is the probability of occurrence of the i-th possible value of the
source symbol. This equation gives the entropy in the units of "bits" (per
symbol) because it uses a logarithm of base 2, and this base-2 measure of
entropy has sometimes been called the "shannon" in his honor. Entropy is also
commonly computed using the natural_logarithm (base e, where e is Euler's
number), which produces a measurement of entropy in "nats" per symbol and
sometimes simplifies the analysis by avoiding the need to include extra
constants in the formulas. Other bases are also possible, but less commonly
used. For example, a logarithm of base 28 = 256 will produce a measurement in
bytes per symbol, and a logarithm of base 10 will produce a measurement in
decimal digits (or hartleys) per symbol.
Intuitively, the entropy HX of a discrete random variable X is a measure of the
amount of uncertainty associated with the value of X when only its distribution
is known.
The entropy of a source that emits a sequence of N symbols that are independent
and_identically_distributed (iid) is N â H bits (per message of N symbols).
If the source data symbols are identically distributed but not independent, the
entropy of a message of length N will be less than N â H.
The entropy of a Bernoulli_trial as a function of success probability, often
called the binary_entropy_function, Hb(p). The entropy is maximized at 1 bit
per trial when the two possible outcomes are equally probable, as in an
unbiased coin toss.
If one transmits 1000 bits (0s and 1s), and the value of each of these bits is
known to the receiver (has a specific value with certainty) ahead of
transmission, it is clear that no information is transmitted. If, however, each
bit is independently equally likely to be 0 or 1, 1000 shannons of information
(more often called bits) have been transmitted. Between these two extremes,
information can be quantified as follows. If ð is the set of all messages
{x1, ..., xn} that X could be, and p(x) is the probability of some     x
&#x2208;  X    {\displaystyle x\in \mathbb {X} }  [x\in \mathbb {X} ], then the
entropy, H, of X is defined:[9]
         H ( X ) =   E   X   [ I ( x ) ] = &#x2212;  &#x2211;  x &#x2208;  X
      p ( x ) log &#x2061; p ( x ) .   {\displaystyle H(X)=\mathbb {E} _{X}[I
      (x)]=-\sum _{x\in \mathbb {X} }p(x)\log p(x).}  [H(X)=\mathbb {E} _{X}[I
      (x)]=-\sum _{x\in \mathbb {X} }p(x)\log p(x).]
(Here, I(x) is the self-information, which is the entropy contribution of an
individual message, and ð¼X is the expected_value.) A property of entropy is
that it is maximized when all the messages in the message space are
equiprobable p(x) = 1/n; i.e., most unpredictable, in which case H(X) = log n.
The special case of information entropy for a random variable with two outcomes
is the binary_entropy_function, usually taken to the logarithmic base 2, thus
having the shannon (Sh) as unit:
          H   b    ( p ) = &#x2212; p  log  2   &#x2061; p &#x2212; ( 1
      &#x2212; p )  log  2   &#x2061; ( 1 &#x2212; p ) .   {\displaystyle H_
      {\mathrm {b} }(p)=-p\log _{2}p-(1-p)\log _{2}(1-p).}  [H_{\mathrm {b} }
      (p)=-p\log _{2}p-(1-p)\log _{2}(1-p).]
**** Joint entropy[edit] ****
The joint_entropy of two discrete random variables X and Y is merely the
entropy of their pairing: (X, Y). This implies that if X and Y are independent,
then their joint entropy is the sum of their individual entropies.
For example, if (X, Y) represents the position of a chess piece â X the row
and Y the column, then the joint entropy of the row of the piece and the column
of the piece will be the entropy of the position of the piece.
         H ( X , Y ) =   E   X , Y   [ &#x2212; log &#x2061; p ( x , y ) ] =
      &#x2212;  &#x2211;  x , y   p ( x , y ) log &#x2061; p ( x , y )
      {\displaystyle H(X,Y)=\mathbb {E} _{X,Y}[-\log p(x,y)]=-\sum _{x,y}p
      (x,y)\log p(x,y)\,}  [H(X,Y)=\mathbb {E} _{X,Y}[-\log p(x,y)]=-\sum _
      {x,y}p(x,y)\log p(x,y)\,]
Despite similar notation, joint entropy should not be confused with cross
entropy.
**** Conditional entropy (equivocation)[edit] ****
The conditional_entropy or conditional uncertainty of X given random variable Y
(also called the equivocation of X about Y) is the average conditional entropy
over Y:[10]
         H ( X  |  Y ) =   E   Y   [ H ( X  |  y ) ] = &#x2212;  &#x2211;  y
      &#x2208; Y   p ( y )  &#x2211;  x &#x2208; X   p ( x  |  y ) log &#x2061;
      p ( x  |  y ) = &#x2212;  &#x2211;  x , y   p ( x , y ) log &#x2061; p
      ( x  |  y ) .   {\displaystyle H(X|Y)=\mathbb {E} _{Y}[H(X|y)]=-\sum _
      {y\in Y}p(y)\sum _{x\in X}p(x|y)\log p(x|y)=-\sum _{x,y}p(x,y)\log p
      (x|y).}  [{\displaystyle H(X|Y)=\mathbb {E} _{Y}[H(X|y)]=-\sum _{y\in Y}p
      (y)\sum _{x\in X}p(x|y)\log p(x|y)=-\sum _{x,y}p(x,y)\log p(x|y).}]
Because entropy can be conditioned on a random variable or on that random
variable being a certain value, care should be taken not to confuse these two
definitions of conditional entropy, the former of which is in more common use.
A basic property of this form of conditional entropy is that:
         H ( X  |  Y ) = H ( X , Y ) &#x2212; H ( Y ) .    {\displaystyle H
      (X|Y)=H(X,Y)-H(Y).\,}  [H(X|Y)=H(X,Y)-H(Y).\,]
**** Mutual information (transinformation)[edit] ****
Mutual_information measures the amount of information that can be obtained
about one random variable by observing another. It is important in
communication where it can be used to maximize the amount of information shared
between sent and received signals. The mutual information of X relative to Y is
given by:
         I ( X ; Y ) =   E   X , Y   [ S I ( x , y ) ] =  &#x2211;  x , y   p
      ( x , y ) log &#x2061;    p ( x , y )   p ( x )  p ( y )
      {\displaystyle I(X;Y)=\mathbb {E} _{X,Y}[SI(x,y)]=\sum _{x,y}p(x,y)\log
      {\frac {p(x,y)}{p(x)\,p(y)}}}  [I(X;Y)=\mathbb {E} _{X,Y}[SI(x,y)]=\sum _
      {x,y}p(x,y)\log {\frac {p(x,y)}{p(x)\,p(y)}}]
where SI (Specific mutual Information) is the pointwise_mutual_information.
A basic property of the mutual information is that
         I ( X ; Y ) = H ( X ) &#x2212; H ( X  |  Y ) .    {\displaystyle I
      (X;Y)=H(X)-H(X|Y).\,}  [I(X;Y)=H(X)-H(X|Y).\,]
That is, knowing Y, we can save an average of I(X; Y) bits in encoding X
compared to not knowing Y.
Mutual information is symmetric:
         I ( X ; Y ) = I ( Y ; X ) = H ( X ) + H ( Y ) &#x2212; H ( X , Y ) .
      {\displaystyle I(X;Y)=I(Y;X)=H(X)+H(Y)-H(X,Y).\,}  [I(X;Y)=I(Y;X)=H(X)+H
      (Y)-H(X,Y).\,]
Mutual information can be expressed as the average KullbackâLeibler
divergence (information gain) between the posterior_probability_distribution of
X given the value of Y and the prior_distribution on X:
         I ( X ; Y ) =   E   p ( y )   [  D   K L    ( p ( X  |  Y = y )
      &#x2016; p ( X ) ) ] .   {\displaystyle I(X;Y)=\mathbb {E} _{p(y)}[D_
      {\mathrm {KL} }(p(X|Y=y)\|p(X))].}  [I(X;Y)=\mathbb {E} _{p(y)}[D_
      {\mathrm {KL} }(p(X|Y=y)\|p(X))].]
In other words, this is a measure of how much, on the average, the probability
distribution on X will change if we are given the value of Y. This is often
recalculated as the divergence from the product of the marginal distributions
to the actual joint distribution:
         I ( X ; Y ) =  D   K L    ( p ( X , Y ) &#x2016; p ( X ) p ( Y ) ) .
      {\displaystyle I(X;Y)=D_{\mathrm {KL} }(p(X,Y)\|p(X)p(Y)).}  [I(X;Y)=D_
      {\mathrm {KL} }(p(X,Y)\|p(X)p(Y)).]
Mutual information is closely related to the log-likelihood_ratio_test in the
context of contingency tables and the multinomial_distribution and to Pearson's
Ï2_test: mutual information can be considered a statistic for assessing
independence between a pair of variables, and has a well-specified asymptotic
distribution.
**** KullbackâLeibler divergence (information gain)[edit] ****
The KullbackâLeibler_divergence (or information divergence, information gain,
or relative entropy) is a way of comparing two distributions: a "true"
probability_distribution p(X), and an arbitrary probability distribution q(X).
If we compress data in a manner that assumes q(X) is the distribution
underlying some data, when, in reality, p(X) is the correct distribution, the
KullbackâLeibler divergence is the number of average additional bits per
datum necessary for compression. It is thus defined
          D   K L    ( p ( X ) &#x2016; q ( X ) ) =  &#x2211;  x &#x2208; X
      &#x2212; p ( x ) log &#x2061;  q ( x )   &#x2212;   &#x2211;  x &#x2208;
      X   &#x2212; p ( x ) log &#x2061;  p ( x )  =  &#x2211;  x &#x2208; X   p
      ( x ) log &#x2061;    p ( x )   q ( x )    .   {\displaystyle D_{\mathrm
      {KL} }(p(X)\|q(X))=\sum _{x\in X}-p(x)\log {q(x)}\,-\,\sum _{x\in X}-p
      (x)\log {p(x)}=\sum _{x\in X}p(x)\log {\frac {p(x)}{q(x)}}.}  [D_{\mathrm
      {KL} }(p(X)\|q(X))=\sum _{x\in X}-p(x)\log {q(x)}\,-\,\sum _{x\in X}-p
      (x)\log {p(x)}=\sum _{x\in X}p(x)\log {\frac {p(x)}{q(x)}}.]
Although it is sometimes used as a 'distance metric', KL divergence is not a
true metric since it is not symmetric and does not satisfy the triangle
inequality (making it a semi-quasimetric).
Another interpretation of the KL divergence is the "unnecessary surprise"
introduced by a prior from the truth: suppose a number X is about to be drawn
randomly from a discrete set with probability distribution p(x). If Alice knows
the true distribution p(x), while Bob believes (has a prior) that the
distribution is q(x), then Bob will be more surprised than Alice, on average,
upon seeing the value of X. The KL divergence is the (objective) expected value
of Bob's (subjective) surprisal minus Alice's surprisal, measured in bits if
the log is in base 2. In this way, the extent to which Bob's prior is "wrong"
can be quantified in terms of how "unnecessarily surprised" it is expected to
make him.
**** Other quantities[edit] ****
Other important information theoretic quantities include RÃ©nyi_entropy (a
generalization of entropy), differential_entropy (a generalization of
quantities of information to continuous distributions), and the conditional
mutual_information.
***** Coding theory[edit] *****
Main article: Coding_theory
A picture showing scratches on the readable surface of a CD-R. Music and data
CDs are coded using error correcting codes and thus can still be read even if
they have minor scratches using error_detection_and_correction.
Coding_theory is one of the most important and direct applications of
information theory. It can be subdivided into source_coding theory and channel
coding theory. Using a statistical description for data, information theory
quantifies the number of bits needed to describe the data, which is the
information entropy of the source.
    * Data compression (source coding): There are two formulations for the
      compression problem:
    * lossless_data_compression: the data must be reconstructed exactly;
    * lossy_data_compression: allocates bits needed to reconstruct the data,
      within a specified fidelity level measured by a distortion function. This
      subset of information theory is called rateâdistortion_theory.
    * Error-correcting codes (channel coding): While data compression removes
      as much redundancy as possible, an error correcting code adds just the
      right kind of redundancy (i.e., error_correction) needed to transmit the
      data efficiently and faithfully across a noisy channel.
This division of coding theory into compression and transmission is justified
by the information transmission theorems, or sourceâchannel separation
theorems that justify the use of bits as the universal currency for information
in many contexts. However, these theorems only hold in the situation where one
transmitting user wishes to communicate to one receiving user. In scenarios
with more than one transmitter (the multiple-access channel), more than one
receiver (the broadcast_channel) or intermediary "helpers" (the relay_channel),
or more general networks, compression followed by transmission may no longer be
optimal. Network_information_theory refers to these multi-agent communication
models.
**** Source theory[edit] ****
Any process that generates successive messages can be considered a source of
information. A memoryless source is one in which each message is an independent
identically_distributed_random_variable, whereas the properties of ergodicity
and stationarity impose less restrictive constraints. All such sources are
stochastic. These terms are well studied in their own right outside information
theory.
*** Rate[edit] ***
Information rate is the average entropy per symbol. For memoryless sources,
this is merely the entropy of each symbol, while, in the case of a stationary
stochastic process, it is
         r =  lim  n &#x2192; &#x221E;   H (  X  n    |   X  n &#x2212; 1   ,
      X  n &#x2212; 2   ,  X  n &#x2212; 3   , &#x2026; ) ;   {\displaystyle
      r=\lim _{n\to \infty }H(X_{n}|X_{n-1},X_{n-2},X_{n-3},\ldots );}  [r=\lim
      _{n\to \infty }H(X_{n}|X_{n-1},X_{n-2},X_{n-3},\ldots );]
that is, the conditional entropy of a symbol given all the previous symbols
generated. For the more general case of a process that is not necessarily
stationary, the average rate is
         r =  lim  n &#x2192; &#x221E;     1 n   H (  X  1   ,  X  2   ,
      &#x2026;  X  n   ) ;   {\displaystyle r=\lim _{n\to \infty }{\frac {1}
      {n}}H(X_{1},X_{2},\dots X_{n});}  [r=\lim _{n\to \infty }{\frac {1}{n}}H
      (X_{1},X_{2},\dots X_{n});]
that is, the limit of the joint entropy per symbol. For stationary sources,
these two expressions give the same result.[11]
It is common in information theory to speak of the "rate" or "entropy" of a
language. This is appropriate, for example, when the source of information is
English prose. The rate of a source of information is related to its redundancy
and how well it can be compressed, the subject of source coding.
**** Channel capacity[edit] ****
Main article: Channel_capacity
Communications over a channelâsuch as an ethernet cableâis the primary
motivation of information theory. As anyone who's ever used a telephone (mobile
or landline) knows, however, such channels often fail to produce exact
reconstruction of a signal; noise, periods of silence, and other forms of
signal corruption often degrade quality.
Consider the communications process over a discrete channel. A simple model of
the process is shown below:
[Channel_model]
Here X represents the space of messages transmitted, and Y the space of
messages received during a unit time over our channel. Let p(y|x) be the
conditional_probability distribution function of Y given X. We will consider p
(y|x) to be an inherent fixed property of our communications channel
(representing the nature of the noise of our channel). Then the joint
distribution of X and Y is completely determined by our channel and by our
choice of f(x), the marginal distribution of messages we choose to send over
the channel. Under these constraints, we would like to maximize the rate of
information, or the signal, we can communicate over the channel. The
appropriate measure for this is the mutual_information, and this maximum mutual
information is called the channel_capacity and is given by:
         C =  max  f   I ( X ; Y ) .    {\displaystyle C=\max _{f}I(X;Y).\!}
      [C=\max _{f}I(X;Y).\!]
This capacity has the following property related to communicating at
information rate R (where R is usually bits per symbol). For any information
rate R < C and coding error Îµ > 0, for large enough N, there exists a code of
length N and rate â¥ R and a decoding algorithm, such that the maximal
probability of block error is â¤ Îµ; that is, it is always possible to
transmit with arbitrarily small block error. In addition, for any rate R > C,
it is impossible to transmit with arbitrarily small block error.
Channel_coding is concerned with finding such nearly optimal codes that can be
used to transmit data over a noisy channel with a small coding error at a rate
near the channel capacity.
*** Capacity of particular channel models[edit] ***
    * A continuous-time analog communications channel subject to Gaussian_noise
      â see ShannonâHartley_theorem.
    * A binary_symmetric_channel (BSC) with crossover probability p is a binary
      input, binary output channel that flips the input bit with probability p.
      The BSC has a capacity of 1 − Hb(p) bits per channel use, where Hb is the
      binary_entropy_function to the base-2 logarithm:
            [Binary_symmetric_channel.svg]
    * A binary_erasure_channel (BEC) with erasure probability p is a binary
      input, ternary output channel. The possible channel outputs are 0, 1, and
      a third symbol 'e' called an erasure. The erasure represents complete
      loss of information about an input bit. The capacity of the BEC is 1 − p
      bits per channel use.
            [Binary_erasure_channel.svg]
***** Applications to other fields[edit] *****
**** Intelligence uses and secrecy applications[edit] ****
Information theoretic concepts apply to cryptography and cryptanalysis.
Turing's information unit, the ban, was used in the Ultra project, breaking the
German Enigma_machine code and hastening the end_of_World_War_II_in_Europe.
Shannon himself defined an important concept now called the unicity_distance.
Based on the redundancy of the plaintext, it attempts to give a minimum amount
of ciphertext necessary to ensure unique decipherability.
Information theory leads us to believe it is much more difficult to keep
secrets than it might first appear. A brute_force_attack can break systems
based on asymmetric_key_algorithms or on most commonly used methods of
symmetric_key_algorithms (sometimes called secret key algorithms), such as
block_ciphers. The security of all such methods currently comes from the
assumption that no known attack can break them in a practical amount of time.
Information_theoretic_security refers to methods such as the one-time_pad that
are not vulnerable to such brute force attacks. In such cases, the positive
conditional mutual_information between the plaintext and ciphertext
(conditioned on the key) can ensure proper transmission, while the
unconditional mutual information between the plaintext and ciphertext remains
zero, resulting in absolutely secure communications. In other words, an
eavesdropper would not be able to improve his or her guess of the plaintext by
gaining knowledge of the ciphertext but not of the key. However, as in any
other cryptographic system, care must be used to correctly apply even
information-theoretically secure methods; the Venona_project was able to crack
the one-time pads of the Soviet Union due to their improper reuse of key
material.
**** Pseudorandom number generation[edit] ****
Pseudorandom_number_generators are widely available in computer language
libraries and application programs. They are, almost universally, unsuited to
cryptographic use as they do not evade the deterministic nature of modern
computer equipment and software. A class of improved random number generators
is termed cryptographically_secure_pseudorandom_number_generators, but even
they require random_seeds external to the software to work as intended. These
can be obtained via extractors, if done carefully. The measure of sufficient
randomness in extractors is min-entropy, a value related to Shannon entropy
through RÃ©nyi_entropy; RÃ©nyi entropy is also used in evaluating randomness in
cryptographic systems. Although related, the distinctions among these measures
mean that a random_variable with high Shannon entropy is not necessarily
satisfactory for use in an extractor and so for cryptography uses.
**** Seismic exploration[edit] ****
One early commercial application of information theory was in the field of
seismic oil exploration. Work in this field made it possible to strip off and
separate the unwanted noise from the desired seismic signal. Information theory
and digital_signal_processing offer a major improvement of resolution and image
clarity over previous analog methods.[12]
**** Semiotics[edit] ****
Semioticians Doede_Nauta and Winfried_NÃ¶th both considered Charles_Sanders
Peirce as having created a theory of information in his works on semiotics.
[13]:171[14]:137 Nauta defined semiotic information theory as the study of "the
internal processes of coding, filtering, and information processing."[13]:91
Concepts from information theory such as redundancy and code control have been
used by semioticians such as Umberto_Eco and Ferruccio_Rossi-Landi to explain
ideology as a form of message transmission whereby a dominant social class
emits its message by using signs that exhibit a high degree of redundancy such
that only one message is decoded among a selection of competing ones.[15]
**** Miscellaneous applications[edit] ****
Information theory also has applications in gambling_and_investing, black
holes, and bioinformatics.
***** See also[edit] *****
    * [icon]Mathematics_portal
    * Algorithmic_probability
    * Algorithmic_information_theory
    * Bayesian_inference
    * Communication_theory
    * Constructor_theory - a generalization of information theory that includes
      quantum information
    * Inductive_probability
    * Info-metrics
    * Minimum_message_length
    * Minimum_description_length
    * List_of_important_publications
    * Philosophy_of_information
**** Applications[edit] ****
    * Active_networking
    * Cryptanalysis
    * Cryptography
    * Cybernetics
    * Entropy_in_thermodynamics_and_information_theory
    * Gambling
    * Intelligence_(information_gathering)
    * Seismic_exploration
**** History[edit] ****
    * Hartley,_R.V.L.
    * History_of_information_theory
    * Shannon,_C.E.
    * Timeline_of_information_theory
    * Yockey,_H.P.
**** Theory[edit] ****
    * Coding_theory
    * Detection_theory
    * Estimation_theory
    * Fisher_information
    * Information_algebra
    * Information_asymmetry
    * Information_field_theory
    * Information_geometry
    * Information_theory_and_measure_theory
    * Kolmogorov_complexity
    * List_of_unsolved_problems_in_information_theory
    * Logic_of_information
    * Network_coding
    * Philosophy_of_information
    * Quantum_information_science
    * Source_coding
**** Concepts[edit] ****
    * Ban_(unit)
    * Channel_capacity
    * Communication_channel
    * Communication_source
    * Conditional_entropy
    * Covert_channel
    * Decoder
    * Differential_entropy
    * Encoder
    * Fungible_information
    * Information_entropy
    * Joint_entropy
    * KullbackâLeibler_divergence
    * Mutual_information
    * Pointwise_mutual_information (PMI)
    * Receiver_(information_theory)
    * Redundancy
    * RÃ©nyi_entropy
    * Self-information
    * Unicity_distance
    * Variety
    * Hamming_distance
***** References[edit] *****
   1. ^ a bF. Rieke; D. Warland; R Ruyter van Steveninck; W Bialek (1997).
      Spikes: Exploring the Neural Code. The MIT press. ISBN 978-0262681087.
   2. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
      .citation q{quotes:"\"""\"""'""'"}.mw-parser-output .citation .cs1-lock-
      free a{background:url("//upload.wikimedia.org/wikipedia/commons/thumb/6/
      65/Lock-green.svg/9px-Lock-green.svg.png")no-repeat;background-position:
      right .1em center}.mw-parser-output .citation .cs1-lock-limited a,.mw-
      parser-output .citation .cs1-lock-registration a{background:url("//
      upload.wikimedia.org/wikipedia/commons/thumb/d/d6/Lock-gray-alt-2.svg/
      9px-Lock-gray-alt-2.svg.png")no-repeat;background-position:right .1em
      center}.mw-parser-output .citation .cs1-lock-subscription a{background:
      url("//upload.wikimedia.org/wikipedia/commons/thumb/a/aa/Lock-red-alt-
      2.svg/9px-Lock-red-alt-2.svg.png")no-repeat;background-position:right
      .1em center}.mw-parser-output .cs1-subscription,.mw-parser-output .cs1-
      registration{color:#555}.mw-parser-output .cs1-subscription span,.mw-
      parser-output .cs1-registration span{border-bottom:1px dotted;cursor:
      help}.mw-parser-output .cs1-ws-icon a{background:url("//
      upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Wikisource-logo.svg/
      12px-Wikisource-logo.svg.png")no-repeat;background-position:right .1em
      center}.mw-parser-output code.cs1-code{color:inherit;background:
      inherit;border:inherit;padding:inherit}.mw-parser-output .cs1-hidden-
      error{display:none;font-size:100%}.mw-parser-output .cs1-visible-error
      {font-size:100%}.mw-parser-output .cs1-maint{display:none;color:
      #33aa33;margin-left:0.3em}.mw-parser-output .cs1-subscription,.mw-parser-
      output .cs1-registration,.mw-parser-output .cs1-format{font-size:95%}.mw-
      parser-output .cs1-kern-left,.mw-parser-output .cs1-kern-wl-left{padding-
      left:0.2em}.mw-parser-output .cs1-kern-right,.mw-parser-output .cs1-kern-
      wl-right{padding-right:0.2em}
   3. ^Delgado-Bonal, Alfonso; MartÃ­n-Torres, Javier (2016-11-03). "Human
      vision_is_determined_based_on_information_theory". Scientific Reports. 6
      (1). Bibcode:2016NatSR...636038D. doi:10.1038/srep36038. ISSN 2045-2322.
      PMC 5093619.
   4. ^cf; Huelsenbeck, J. P.; Ronquist, F.; Nielsen, R.; Bollback, J. P.
      (2001). "Bayesian inference of phylogeny and its impact on evolutionary
      biology". Science. 294 (5550): 2310â2314. Bibcode:2001Sci...294.2310H.
      doi:10.1126/science.1065889.
   5. ^Allikmets, Rando; Wasserman, Wyeth W.; Hutchinson, Amy; Smallwood,
      Philip; Nathans, Jeremy; Rogan, Peter K. (1998). "Thomas_D._Schneider],
      Michael_Dean_(1998)_Organization_of_the_ABCR_gene:_analysis_of_promoter
      and_splice_junction_sequences". Gene. 215 (1): 111â122. doi:10.1016/
      s0378-1119(98)00269-8.
   6. ^ Burnham, K. P. and Anderson D. R. (2002) Model Selection and Multimodel
      Inference: A Practical Information-Theoretic Approach, Second Edition
      (Springer Science, New York)
   7. ISBN 978-0-387-95364-9.
   8. ^Jaynes, E. T. (1957). "Information_Theory_and_Statistical_Mechanics".
      Phys. Rev. 106 (4): 620. Bibcode:1957PhRv..106..620J. doi:10.1103/
      physrev.106.620.
   9. ^Bennett, Charles H.; Li, Ming; Ma, Bin (2003). "Chain_Letters_and
      Evolutionary_Histories". Scientific American. 288 (6): 76â81. Bibcode:
      2003SciAm.288f..76B. doi:10.1038/scientificamerican0603-76.
      PMID 12764940.
  10. ^David R. Anderson (November 1, 2003). "Some_background_on_why_people_in
      the_empirical_sciences_may_want_to_better_understand_the_information-
      theoretic_methods" (PDF). Archived from the_original (pdf) on July 23,
      2011. Retrieved 2010-06-23.
  11. ^Fazlollah M. Reza (1994) [1961]. An_Introduction_to_Information_Theory.
      Dover Publications, Inc., New York. ISBN 0-486-68210-2.
  12. ^Robert B. Ash (1990) [1965]. Information_Theory. Dover Publications,
      Inc. ISBN 0-486-66521-6.
  13. ^Jerry D. Gibson (1998). Digital_Compression_for_Multimedia:_Principles
      and_Standards. Morgan Kaufmann. ISBN 1-55860-369-7.
  14. ^ The_Corporation_and_Innovation, Haggerty, Patrick, Strategic Management
      Journal, Vol. 2, 97-118 (1981)
  15. ^ a bNauta, Doede (1972). The Meaning of Information. The Hague: Mouton.
      ISBN 9789027919960.
  16. ^NÃ¶th, Winfried (January 2012). "Charles_S._Peirce's_theory_of
      information:_a_theory_of_the_growth_of_symbols_and_of_knowledge".
      Cybernetics and Human Knowing. 19 (1â2): 137â161.
  17. ^ NÃ¶th, Winfried (1981). "Semiotics_of_ideology". Semiotica, Issue 148.
**** The classic work[edit] ****
    * Shannon,_C.E. (1948), "A_Mathematical_Theory_of_Communication", Bell
      System Technical Journal, 27, pp. 379â423 & 623â656, July & October,
      1948. PDF.
      Notes_and_other_formats.
    * R.V.L. Hartley, "Transmission_of_Information", Bell System Technical
      Journal, July 1928
    * Andrey_Kolmogorov (1968), "Three_approaches_to_the_quantitative
      definition_of_information" in International Journal of Computer
      Mathematics.
**** Other journal articles[edit] ****
    * J. L. Kelly, Jr., Betbubbles.com, "A New Interpretation of Information
      Rate" Bell System Technical Journal, Vol. 35, July 1956, pp. 917â26.
    * R. Landauer, IEEE.org, "Information is Physical" Proc. Workshop on
      Physics and Computation PhysComp'92 (IEEE Comp. Sci.Press, Los Alamitos,
      1993) pp. 1â4.
    * R. Landauer, IBM.com, "Irreversibility and Heat Generation in the
      Computing Process" IBM J. Res. Dev. Vol. 5, No. 3, 1961
    * Timme, Nicholas; Alford, Wesley; Flecker, Benjamin; Beggs, John M.
      (2012). "Multivariate information measures: an experimentalist's
      perspective". arXiv:1111.6857 [cs.IT].
**** Textbooks on information theory[edit] ****
    * Arndt, C. Information Measures, Information and its Description in
      Science and Engineering (Springer Series: Signals and Communication
      Technology), 2004,
ISBN 978-3-540-40855-0
Ash, RB. Information Theory. New York: Interscience, 1965.
ISBN 0-470-03445-9. New York: Dover 1990.
ISBN 0-486-66521-6
Gallager,_R. Information Theory and Reliable Communication. New York: John
Wiley and Sons, 1968.
ISBN 0-471-29048-3
Goldman, S. Information Theory. New York: Prentice Hall, 1953. New York: Dover
1968
ISBN 0-486-62209-6, 2005
ISBN 0-486-44271-3
Cover,_Thomas; Thomas, Joy A. (2006). Elements of information theory (2nd ed.).
New York: Wiley-Interscience. ISBN 0-471-24195-4.
Csiszar,_I, Korner, J. Information Theory: Coding Theorems for Discrete
Memoryless Systems Akademiai Kiado: 2nd edition, 1997.
ISBN 963-05-7440-3
MacKay,_David_J._C.. Information_Theory,_Inference,_and_Learning_Algorithms
Cambridge: Cambridge University Press, 2003.
ISBN 0-521-64298-1
Mansuripur, M. Introduction to Information Theory. New York: Prentice Hall,
1987.
ISBN 0-13-484668-0
McEliece,_R. The Theory of Information and Coding". Cambridge, 2002.
ISBN 978-0521831857
Pierce, JR. "An introduction to information theory: symbols, signals and
noise". Dover (2nd Edition). 1961 (reprinted by Dover 1980).
Reza,_F. An Introduction to Information Theory. New York: McGraw-Hill 1961. New
York: Dover 1994.
ISBN 0-486-68210-2
Shannon,_Claude; Weaver,_Warren (1949). The_Mathematical_Theory_of
Communication (PDF). Urbana,_Illinois: University_of_Illinois_Press. ISBN 0-
252-72548-4. LCCN 49-11922.
Stone, JV. Chapter 1 of book "Information_Theory:_A_Tutorial_Introduction",
University of Sheffield, England, 2014.
ISBN 978-0956372857.
Yeung, RW. A_First_Course_in_Information_Theory Kluwer Academic/Plenum
Publishers, 2002.
ISBN 0-306-46791-7.
Yeung, RW. Information_Theory_and_Network_Coding Springer 2008, 2002.
ISBN 978-0-387-79233-0
**** Other books[edit] ****
    * Leon Brillouin, Science and Information Theory, Mineola, N.Y.: Dover,
      [1956, 1962] 2004.
ISBN 0-486-43918-6
James_Gleick, The_Information:_A_History,_a_Theory,_a_Flood, New York:
Pantheon, 2011.
ISBN 978-0-375-42372-7
A. I. Khinchin, Mathematical Foundations of Information Theory, New York:
Dover, 1957.
ISBN 0-486-60434-9
H. S. Leff and A. F. Rex, Editors, Maxwell's Demon: Entropy, Information,
Computing, Princeton University Press, Princeton, New Jersey (1990).
ISBN 0-691-08727-X
Robert_K._Logan. What is Information? - Propagating Organization in the
Biosphere, the Symbolosphere, the Technosphere and the Econosphere, Toronto:
DEMO Publishing.
Tom Siegfried, The Bit and the Pendulum, Wiley, 2000.
ISBN 0-471-32174-5
Charles Seife, Decoding_the_Universe, Viking, 2006.
ISBN 0-670-03441-X
Jeremy Campbell, Grammatical_Man, Touchstone/Simon & Schuster, 1982,
ISBN 0-671-44062-4
Henri Theil, Economics and Information Theory, Rand McNally & Company -
Chicago, 1967.
Escolano, Suau, Bonev, Information_Theory_in_Computer_Vision_and_Pattern
Recognition, Springer, 2009.
ISBN 978-1-84882-296-2
Vlatko Vedral, Decoding Reality: The Universe as Quantum Information, Oxford
University Press 2010.
ISBN 0-19-923769-7
**** MOOC on information theory[edit] ****
    * Raymond W. Yeung, "Information_Theory" (The_Chinese_University_of_Hong
      Kong)
***** External links[edit] *****
 Wikiquote has quotations related to: Information_theory
Library_resources about
Information theory
===============================================================================
    * Resources_in_your_library
    * Resources_in_other_libraries
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Information", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Lambert F. L. (1999), "Shuffled_Cards,_Messy_Desks,_and_Disorderly_Dorm_Rooms_-
Examples_of_Entropy_Increase?_Nonsense!", Journal of Chemical Education
IEEE_Information_Theory_Society and ITSOC_Monographs,_Surveys,_and_Reviews
    * v
    * t
    * e
Subfields of and cyberneticians involved in cybernetics
                   * Polycontexturality
                   * Second-order_cybernetics
                   * Catastrophe_theory
                   * Connectionism
                   * Control_theory
                   * Cybernetics_in_the_Soviet_Union
                   * Decision_theory
                   * Engineering_cybernetics
                   * Information theory
                   * Semiotics
                   * Synergetics
Subfields          * Biological_cybernetics
                   * Biosemiotics
                   * Biomedical_cybernetics
                   * Biorobotics
                   * Computational_neuroscience
                   * Homeostasis
                   * Management_cybernetics
                   * Medical_cybernetics
                   * Neurocybernetics
                   * Sociocybernetics
                   * Emergence
                   * Artificial_intelligence
                   * Maleyka_Abbaszadeh
                   * Igor_Aleksander
                   * William_Ross_Ashby
                   * Gregory_Bateson
                   * Anthony_Stafford_Beer
                   * Natalia_Bekhtereva
                   * Claude_Bernard
                   * Ludwig_von_Bertalanffy
                   * Valentin_Braitenberg
                   * Gordon_S._Brown
                   * Walter_Bradford_Cannon
                   * Manfred_Clynes
                   * Heinz_von_Foerster
                   * Charles_FranÃ§ois
                   * Jay_Wright_Forrester
                   * Jacque_Fresco
                   * Buckminster_Fuller
                   * Ranulph_Glanville
                   * Ernst_von_Glasersfeld
                   * Pyotr_Grigorenko
                   * N._Katherine_Hayles
                   * Francis_Heylighen
                   * Erich_von_Holst
                   * Jason_Jixuan_Hu
                   * Cliff_Joslyn
                   * Stuart_Kauffman
                   * Sergei_P._Kurdyumov
Cyberneticists     * Allenna_Leonard
                   * Alexander_Lerner
                   * Niklas_Luhmann
                   * Alexey_Lyapunov
                   * Warren_McCulloch
                   * Humberto_Maturana
                   * Marian_Mazur
                   * Margaret_Mead
                   * Ulla_Mitzdorf
                   * Talcott_Parsons
                   * Gordon_Pask
                   * Walter_Pitts
                   * Qian_Xuesen
                   * Alfred_Radcliffe-Brown
                   * I._A._Richards
                   * Robert_Trappl
                   * Valentin_Turchin
                   * Jakob_von_UexkÃ¼ll
                   * Stuart_Umpleby
                   * Francisco_Varela
                   * Frederic_Vester
                   * Charles_Geoffrey_Vickers
                   * John_N._Warfield
                   * William_Grey_Walter
                   * Kevin_Warwick
                   * Norbert_Wiener
                   * Jennifer_Wilby
                   * Anthony_Wilden
    * v
    * t
    * e
Data_compression methods
                             * Arithmetic
                             * Asymmetric_numeral_systems
                             * Golomb
                             * Huffman
                                   o Adaptive
                                   o Canonical
                                   o Modified
                             * Range
         Entropy_type        * Shannon
                             * ShannonâFano
                             * ShannonâFanoâElias
                             * Tunstall
                             * Unary
                             * Universal
                                   o Exp-Golomb
                                   o Fibonacci
                                   o Gamma
                                   o Levenshtein
                             * Byte_pair_encoding
                             * DEFLATE
                             * Snappy
Lossless                     * LempelâZiv
                                   o LZ77 /_LZ78_(LZ1 /_LZ2)
                                   o LZFSE
                                   o LZJB
                                   o LZMA
         Dictionary_type           o LZO
                                   o LZRW
                                   o LZS
                                   o LZSS
                                   o LZW
                                   o LZWL
                                   o LZX
                                   o LZ4
                                   o Brotli
                                   o Zstandard
                             * BWT
                             * CTW
                             * Delta
         Other types         * DMC
                             * MTF
                             * PAQ
                             * PPM
                             * RLE
                         * Bit_rate
                               o ABR
                               o CBR
                               o VBR
                         * Companding
                         * Convolution
         Concepts        * Dynamic_range
                         * Latency
                         * NyquistâShannon_theorem
                         * Sampling
                         * Sound_quality
                         * Speech_coding
Audio                    * Sub-band_coding
                         * A-law
                         * Î¼-law
                         * ACELP
                         * ADPCM
                         * CELP
                         * DPCM
         Codec parts     * Fourier_transform
                         * LPC
                               o LAR
                               o LSP
                         * MDCT
                         * Psychoacoustic_model
                         * WLPC
                      * Chroma_subsampling
                      * Coding_tree_unit
                      * Color_space
                      * Compression_artifact
         Concepts     * Image_resolution
                      * Macroblock
                      * Pixel
                      * PSNR
                      * Quantization
Image                 * Standard_test_image
                      * Chain_code
                      * DCT
                      * EZW
                      * Fractal
         Methods      * KLT
                      * LP
                      * RLE
                      * SPIHT
                      * Wavelet
                         * Bit_rate
                               o ABR
                               o CBR
                               o VBR
                         * Display_resolution
         Concepts        * Frame
                         * Frame_rate
Video                    * Frame_types
                         * Interlace
                         * Video_characteristics
                         * Video_quality
                         * DCT
         Codec parts     * Deblocking_filter
                         * Lapped_transform
                         * Motion_compensation
             * Entropy
             * Information theory
                   o Timeline
             * Kolmogorov_complexity
Theory       * Lossy
                   o DCT
             * Quantization
             * Rateâdistortion
             * Redundancy
    * [Template] Compression_formats
    * [Template] Compression_software_(codecs)
    * v
    * t
    * e
Areas_of_mathematics
                  * Category_theory
                  * Information theory
Foundations       * Mathematical_logic
                  * Philosophy_of_mathematics
                  * Set_theory
                  * Abstract
Algebra           * Elementary
                  * Linear
                  * Multilinear
                  * Calculus
                  * Real_analysis
Analysis          * Complex_analysis
                  * Differential_equations
                  * Functional_analysis
                  * Combinatorics
Discrete          * Graph_theory
                  * Order_theory
                  * Game_theory
                  * Algebraic
                  * Analytic
Geometry          * Differential
                  * Discrete
                  * Euclidean
                  * Finite
                  * Arithmetic
Number_theory     * Algebraic_number_theory
                  * Analytic_number_theory
                  * Diophantine_geometry
                  * Algebraic
Topology          * Differential
                  * Geometric
                  * Control_theory
                  * Mathematical_economics
                  * Mathematical_finance
Applied           * Mathematical_physics
                  * Mathematical_statistics
                  * Probability
                  * Statistics
                  * Computer_science
                  * Theory_of_computation
Computational     * Numerical_analysis
                  * Optimization
                  * Computer_algebra
                  * History_of_mathematics
Others            * Recreational_mathematics
                  * Mathematics_and_art
                  * Mathematics_education
    * [Category] Category
    * [Portal] Portal
    * [Commons page]Commons
    * [WikiProject]WikiProject
    * v
    * t
    * e
Computer_science
Note: This template roughly follows the 2012 ACM_Computing_Classification
System.
                          * Printed_circuit_board
                          * Peripheral
                          * Integrated_circuit
Hardware                  * Very_Large_Scale_Integration
                          * Systems_on_Chip_(SoCs)
                          * Energy_consumption_(Green_computing)
                          * Electronic_design_automation
                          * Hardware_acceleration
                          * Computer_architecture
Computer systems          * Embedded_system
organization              * Real-time_computing
                          * Dependability
                          * Network_architecture
                          * Network_protocol
Networks                  * Network_components
                          * Network_scheduler
                          * Network_performance_evaluation
                          * Network_service
                          * Interpreter
                          * Middleware
Software organization     * Virtual_machine
                          * Operating_system
                          * Software_quality
                          * Programming_paradigm
                          * Programming_language
                          * Compiler
                          * Domain-specific_language
Software_notations        * Modeling_language
and tools                 * Software_framework
                          * Integrated_development_environment
                          * Software_configuration_management
                          * Software_library
                          * Software_repository
                          * Software_development_process
                          * Requirements_analysis
                          * Software_design
Software_development      * Software_construction
                          * Software_deployment
                          * Software_maintenance
                          * Programming_team
                          * Open-source_model
                          * Model_of_computation
                          * Formal_language
Theory_of_computation     * Automata_theory
                          * Computational_complexity_theory
                          * Logic
                          * Semantics
                          * Algorithm_design
                          * Analysis_of_algorithms
Algorithms                * Algorithmic_efficiency
                          * Randomized_algorithm
                          * Computational_geometry
                          * Discrete_mathematics
                          * Probability
Mathematics               * Statistics
of computing              * Mathematical_software
                          * Information theory
                          * Mathematical_analysis
                          * Numerical_analysis
                          * Database_management_system
                          * Information_storage_systems
                          * Enterprise_information_system
                          * Social_information_systems
                          * Geographic_information_system
                          * Decision_support_system
Information               * Process_control_system
systems                   * Multimedia_information_system
                          * Data_mining
                          * Digital_library
                          * Computing_platform
                          * Digital_marketing
                          * World_Wide_Web
                          * Information_retrieval
                          * Cryptography
                          * Formal_methods
                          * Security_services
Security                  * Intrusion_detection_system
                          * Hardware_security
                          * Network_security
                          * Information_security
                          * Application_security
                          * Interaction_design
Humanâcomputer       * Social_computing
interaction               * Ubiquitous_computing
                          * Visualization
                          * Accessibility
                          * Concurrent_computing
                          * Parallel_computing
Concurrency               * Distributed_computing
                          * Multithreading
                          * Multiprocessing
                          * Natural_language_processing
                          * Knowledge_representation_and_reasoning
                          * Computer_vision
Artificial                * Automated_planning_and_scheduling
intelligence              * Search_methodology
                          * Control_method
                          * Philosophy_of_artificial_intelligence
                          * Distributed_artificial_intelligence
                          * Supervised_learning
                          * Unsupervised_learning
Machine_learning          * Reinforcement_learning
                          * Multi-task_learning
                          * Cross-validation
                          * Animation
                          * Rendering
                          * Image_manipulation
Graphics                  * Graphics_processing_unit
                          * Mixed_reality
                          * Virtual_reality
                          * Image_compression
                          * Solid_modeling
                          * E-commerce
                          * Enterprise_software
                          * Computational_mathematics
                          * Computational_physics
                          * Computational_chemistry
                          * Computational_biology
                          * Computational_social_science
                          * Computational_engineering
Applied                   * Computational_healthcare
computing                 * Digital_art
                          * Electronic_publishing
                          * Cyberwarfare
                          * Electronic_voting
                          * Video_games
                          * Word_processing
                          * Operations_research
                          * Educational_technology
                          * Document_management
    * [Wikipedia book] Book
    * [Category] Category
    * [Portal] Portal
    * [Outline] Outline
    * [WikiProject]WikiProject
    * [Commons page] Commons
Authority_control [Edit_this_at_Wikidata]     * GND: 4026927-9
                                              * NDL: 00575012

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Information_theory&oldid=908002757"
Categories:
    * Information_theory
    * Cybernetics
    * Formal_sciences
    * Information_Age
Hidden categories:
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_NDL_identifiers
***** Navigation menu *****
**** Personal tools ****
    * Not logged in
    * Talk
    * Contributions
    * Create_account
    * Log_in
**** Namespaces ****
    * Article
    * Talk
⁰
**** Variants ****
**** Views ****
    * Read
    * Edit
    * View_history
⁰
**** More ****
**** Search ****
[Unknown INPUT type][Search][Go]
**** Navigation ****
    * Main_page
    * Contents
    * Featured_content
    * Current_events
    * Random_article
    * Donate_to_Wikipedia
    * Wikipedia_store
**** Interaction ****
    * Help
    * About_Wikipedia
    * Community_portal
    * Recent_changes
    * Contact_page
**** Tools ****
    * What_links_here
    * Related_changes
    * Upload_file
    * Special_pages
    * Permanent_link
    * Page_information
    * Wikidata_item
    * Cite_this_page
**** In other projects ****
    * Wikimedia_Commons
    * Wikiquote
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Boarisch
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Hrvatski
    * Ido
    * Bahasa_Indonesia
    * Interlingua
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * à´®à´²à´¯à´¾à´³à´
    * Bahasa_Melayu
    * MirandÃ©s
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * áá¼ááºáá¬áá¬áá¬
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Occitan
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 26 July 2019, at 18:47 (UTC).
    * Text is available under the Creative_Commons_Attribution-ShareAlike
      License; additional terms may apply. By using this site, you agree to the
      Terms_of_Use and Privacy_Policy. WikipediaÂ® is a registered trademark of
      the Wikimedia_Foundation,_Inc., a non-profit organization.
    * Privacy_policy
    * About_Wikipedia
    * Disclaimers
    * Contact_Wikipedia
    * Developers
    * Cookie_statement
    * Mobile_view
    * [Wikimedia_Foundation]
    * [Powered_by_MediaWiki]
