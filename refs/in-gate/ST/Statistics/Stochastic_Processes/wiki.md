The following text has been accessed from https://en.wikipedia.org/wiki/Stochastic_process at Fri Aug 9 02:51:49 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Stochastic process ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
A computer-simulated realization of a Wiener or Brownian_motion process on the
surface of a sphere. The Wiener process is widely considered the most studied
and central stochastic process in probability theory.[1][2][3]
In probability_theory and related fields, a stochastic or random process is a
mathematical_object usually defined as a family of random_variables.
Historically, the random variables were associated with or indexed by a set of
numbers, usually viewed as points in time, giving the interpretation of a
stochastic process representing numerical values of some system randomly
changing over time, such as the growth of a bacterial population, an electrical
current fluctuating due to thermal_noise, or the movement of a gas molecule.[1]
[4][5][6] Stochastic processes are widely used as mathematical_models of
systems and phenomena that appear to vary in a random manner. They have
applications in many disciplines including sciences such as biology,[7]
chemistry,[8] ecology,[9] neuroscience,[10] and physics[11] as well as
technology and engineering fields such as image_processing, signal_processing,
[12] information_theory,[13] computer_science,[14] cryptography[15] and
telecommunications.[16] Furthermore, seemingly random changes in financial
markets have motivated the extensive use of stochastic processes in finance.
[17][18][19]
Applications and the study of phenomena have in turn inspired the proposal of
new stochastic processes. Examples of such stochastic processes include the
Wiener_process or Brownian motion process,[a] used by Louis_Bachelier to study
price changes on the Paris_Bourse,[22] and the Poisson_process, used by A._K.
Erlang to study the number of phone calls occurring in a certain period of
time.[23] These two stochastic processes are considered the most important and
central in the theory of stochastic processes,[1][4][24] and were discovered
repeatedly and independently, both before and after Bachelier and Erlang, in
different settings and countries.[22][25]
The term random function is also used to refer to a stochastic or random
process,[26][27] because a stochastic process can also be interpreted as a
random element in a function_space.[28][29] The terms stochastic process and
random process are used interchangeably, often with no specific mathematical
space for the set that indexes the random variables.[28][30] But often these
two terms are used when the random variables are indexed by the integers or an
interval of the real_line.[5][30] If the random variables are indexed by the
Cartesian_plane or some higher-dimensional Euclidean_space, then the collection
of random variables is usually called a random_field instead.[5][31] The values
of a stochastic process are not always numbers and can be vectors or other
mathematical objects.[5][29]
Based on their mathematical properties, stochastic processes can be divided
into various categories, which include random_walks,[32] martingales,[33]
Markov_processes,[34] LÃ©vy_processes,[35] Gaussian_processes,[36] random
fields,[37] renewal_processes, and branching_processes.[38] The study of
stochastic processes uses mathematical knowledge and techniques from
probability, calculus, linear_algebra, set_theory, and topology[39][40][41] as
well as branches of mathematical_analysis such as real_analysis, measure
theory, Fourier_analysis, and functional_analysis.[42][43][44] The theory of
stochastic processes is considered to be an important contribution to
mathematics[45] and it continues to be an active topic of research for both
theoretical reasons and applications.[46][47][48]
⁰
***** Contents *****
    * 1_Introduction
          o 1.1_Classifications
          o 1.2_Etymology
          o 1.3_Terminology
          o 1.4_Notation
    * 2_Examples
          o 2.1_Bernoulli_process
          o 2.2_Random_walk
          o 2.3_Wiener_process
          o 2.4_Poisson_process
    * 3_Definitions
          o 3.1_Stochastic_process
          o 3.2_Index_set
          o 3.3_State_space
          o 3.4_Sample_function
          o 3.5_Increment
          o 3.6_Further_definitions
                # 3.6.1_Law
                # 3.6.2_Finite-dimensional_probability_distributions
                # 3.6.3_Stationarity
                # 3.6.4_Filtration
                # 3.6.5_Modification
                # 3.6.6_Indistinguishable
                # 3.6.7_Separability
                # 3.6.8_Independence
                # 3.6.9_Uncorrelatedness
                # 3.6.10_Independence_implies_uncorrelatedness
                # 3.6.11_Orthogonality
                # 3.6.12_Skorokhod_space
                # 3.6.13_Regularity
    * 4_Further_examples
          o 4.1_Markov_processes_and_chains
          o 4.2_Martingale
          o 4.3_LÃ©vy_process
          o 4.4_Random_field
          o 4.5_Point_process
    * 5_History
          o 5.1_Early_probability_theory
          o 5.2_Statistical_mechanics
          o 5.3_Measure_theory_and_probability_theory
          o 5.4_Birth_of_modern_probability_theory
          o 5.5_Stochastic_processes_after_World_War_II
          o 5.6_Discoveries_of_specific_stochastic_processes
                # 5.6.1_Bernoulli_process
                # 5.6.2_Random_walks
                # 5.6.3_Wiener_process
                # 5.6.4_Poisson_process
                # 5.6.5_Markov_processes
                # 5.6.6_LÃ©vy_processes
    * 6_Mathematical_construction
          o 6.1_Construction_issues
          o 6.2_Resolving_construction_issues
    * 7_See_also
    * 8_Notes
    * 9_References
    * 10_Further_reading
          o 10.1_Articles
          o 10.2_Books
    * 11_External_links
***** Introduction[edit] *****
A stochastic or random process can be defined as a collection of random
variables that is indexed by some mathematical set, meaning that each random
variable of the stochastic process is uniquely associated with an element in
the set.[4][5] The set used to index the random variables is called the index
set. Historically, the index set was some subset of the real_line, such as the
natural_numbers, giving the index set the interpretation of time.[1] Each
random variable in the collection takes values from the same mathematical_space
known as the state space. This state space can be, for example, the integers,
the real line or     n   {\displaystyle n}  [n]-dimensional Euclidean space.[1]
[5] An increment is the amount that a stochastic process changes between two
index values, often interpreted as two points in time.[49][50] A stochastic
process can have many outcomes, due to its randomness, and a single outcome of
a stochastic process is called, among other names, a sample function or
realization.[29][51]
A single computer-simulated sample function or realization, among other terms,
of a three-dimensional Wiener or Brownian motion process for time 0 â¤ t â¤
2. The index set of this stochastic process is the non-negative numbers, while
its state space is three-dimensional Euclidean space.
**** Classifications[edit] ****
A stochastic process can be classified in different ways, for example, by its
state space, its index set, or the dependence among the random variables. One
common way of classification is by the cardinality of the index set and the
state space.[52][53][54]
When interpreted as time, if the index set of a stochastic process has a finite
or countable number of elements, such as a finite set of numbers, the set of
integers, or the natural numbers, then the stochastic process is said to be in
discrete_time.[55][56] If the index set is some interval of the real line, then
time is said to be continuous. The two types of stochastic processes are
respectively referred to as discrete-time and continuous-time_stochastic
processes.[49][57][58] Discrete-time stochastic processes are considered easier
to study because continuous-time processes require more advanced mathematical
techniques and knowledge, particularly due to the index set being uncountable.
[59][60] If the index set is the integers, or some subset of them, then the
stochastic process can also be called a random sequence.[56]
If the state space is the integers or natural numbers, then the stochastic
process is called a discrete or integer-valued stochastic process. If the state
space is the real line, then the stochastic process is referred to as a real-
valued stochastic process or a process with continuous state space. If the
state space is     n   {\displaystyle n}  [n]-dimensional Euclidean space, then
the stochastic process is called a     n   {\displaystyle n}  [n]-dimensional
vector process or     n   {\displaystyle n}  [n]-vector process.[52][53]
**** Etymology[edit] ****
The word stochastic in English was originally used as an adjective with the
definition "pertaining to conjecturing", and stemming from a Greek word meaning
"to aim at a mark, guess", and the Oxford_English_Dictionary gives the year
1662 as its earliest occurrence.[61] In his work on probability Ars
Conjectandi, originally published in Latin in 1713, Jakob_Bernoulli used the
phrase "Ars Conjectandi sive Stochastice", which has been translated to "the
art of conjecturing or stochastics".[62] This phrase was used, with reference
to Bernoulli, by Ladislaus_Bortkiewicz[63] who in 1917 wrote in German the word
stochastik with a sense meaning random. The term stochastic process first
appeared in English in a 1934 paper by Joseph_Doob.[61] For the term and a
specific mathematical definition, Doob cited another 1934 paper, where the term
stochastischer ProzeÃ was used in German by Aleksandr_Khinchin,[64][65] though
the German term had been used earlier, for example, by Andrei Kolmogorov in
1931.[66]
Early occurrences of the word random in English with its current meaning, which
relates to chance or luck, date back to the 16th century, while earlier
recorded usages started in the 14th century as a noun meaning "impetuosity,
great speed, force, or violence (in riding, running, striking, etc.)". The word
itself comes from a Middle French word meaning "speed, haste", and it is
probably derived from a French verb meaning "to run" or "to gallop". The first
written appearance of the term random process pre-dates stochastic process,
which the Oxford English Dictionary also gives as a synonym, and was used in an
article by Francis_Edgeworth published in 1888.[67]
**** Terminology[edit] ****
The definition of a stochastic process varies,[68] but a stochastic process is
traditionally defined as a collection of random variables indexed by some set.
[69][70] The terms random process and stochastic process are considered
synonyms and are used interchangeably, without the index set being precisely
specified.[28][30][31][71][72][73] Both "collection",[29][71] or "family" are
used[4][74] while instead of "index set", sometimes the terms "parameter set"
[29] or "parameter space"[31] are used.
The term random function is also used to refer to a stochastic or random
process,[5][75][76] though sometimes it is only used when the stochastic
process takes real values.[29][74] This term is also used when the index sets
are mathematical spaces other than the real line,[5][77] while the terms
stochastic process and random process are usually used when the index set
interpreted as time,[5][77][78] and other terms are used such as random field
when the index set is     n   {\displaystyle n}  [n]-dimensional Euclidean
space      R  n     {\displaystyle R^{n}}  [R^{n}] or a manifold.[5][29][31]
**** Notation[edit] ****
A stochastic process can be denoted, among other ways, by     { X ( t )  }  t
&#x2208; T     {\displaystyle \{X(t)\}_{t\in T}}  [{\displaystyle \{X(t)\}_
{t\in T}}],[57]     {  X  t    }  t &#x2208; T     {\displaystyle \{X_{t}\}_
{t\in T}}  [{\displaystyle \{X_{t}\}_{t\in T}}],[70]     {  X  t   }
{\displaystyle \{X_{t}\}}  [{\displaystyle \{X_{t}\}}][79]     { X ( t ) }
{\displaystyle \{X(t)\}}  [{\displaystyle \{X(t)\}}] or simply as     X
{\displaystyle X}  [X] or     X ( t )   {\displaystyle X(t)}  [X(t)], although
X ( t )   {\displaystyle X(t)}  [X(t)] is regarded as an abuse_of_notation.[80]
For example,     X ( t )   {\displaystyle X(t)}  [X(t)] or      X  t
{\displaystyle X_{t}}  [X_{t}] are used to refer to the random variable with
the index     t   {\displaystyle t}  [t], and not the entire stochastic
process.[79] If the index set is     T = [ 0 , &#x221E; )   {\displaystyle T=
[0,\infty )}  [{\displaystyle T=[0,\infty )}], then one can write, for example,
(  X  t   , t &#x2265; 0 )   {\displaystyle (X_{t},t\geq 0)}  [{\displaystyle
(X_{t},t\geq 0)}] to denote the stochastic process.[30]
***** Examples[edit] *****
**** Bernoulli process[edit] ****
Main article: Bernoulli_process
One of the simplest stochastic processes is the Bernoulli_process,[6][81] which
is a sequence of independent_and_identically_distributed (iid) random
variables, where each random variable takes either the value one or zero, say
one with probability     p   {\displaystyle p}  [p] and zero with probability
1 &#x2212; p   {\displaystyle 1-p}  [1-p]. This process can be linked to
repeatedly flipping a coin, where the probability of obtaining a head is     p
{\displaystyle p}  [p] and its value is one, while the value of a tail is zero.
[6][82] In other words, a Bernoulli process is a sequence of iid Bernoulli
random variables,[83] where each coin flip is an example of a Bernoulli_trial.
[84]
**** Random walk[edit] ****
Main article: Random_walk
Random_walks are stochastic processes that are usually defined as sums of iid
random variables or random vectors in Euclidean space, so they are processes
that change in discrete time.[85][86][87][88][89] But some also use the term to
refer to processes that change in continuous time,[90] particularly the Wiener
process used in finance, which has led to some confusion, resulting in its
criticism.[91] There are other various types of random walks, defined so their
state spaces can be other mathematical objects, such as lattices and groups,
and in general they are highly studied and have many applications in different
disciplines.[90][92]
A classic example of a random walk is known as the simple random walk, which is
a stochastic process in discrete time with the integers as the state space, and
is based on a Bernoulli process, where each Bernoulli variable takes either the
value positive one or negative one. In other words, the simple random walk
takes place on the integers, and its value increases by one with probability,
say,     p   {\displaystyle p}  [p], or decreases by one with probability     1
&#x2212; p   {\displaystyle 1-p}  [1-p], so index set of this random walk is
the natural numbers, while its state space is the integers. If the     p = 0.5
{\displaystyle p=0.5}  [p=0.5], this random walk is called a symmetric random
walk.[93][94]
**** Wiener process[edit] ****
Main article: Wiener_process
The Wiener process is a stochastic process with stationary and independent
increments that are normally_distributed based on the size of the increments.
[2][95] The Wiener process is named after Norbert_Wiener, who proved its
mathematical existence, but the process is also called the Brownian motion
process or just Brownian motion due to its historical connection as a model for
Brownian_movement in liquids.[96][97][97][98]
Realizations of Wiener processes (or Brownian motion processes) with drift
(blue) and without drift (red).
Playing a central role in the theory of probability, the Wiener process is
often considered the most important and studied stochastic process, with
connections to other stochastic processes.[1][2][3][99][100][101][102] Its
index set and state space are the non-negative numbers and real numbers,
respectively, so it has both continuous index set and states space.[103] But
the process can be defined more generally so its state space can be     n
{\displaystyle n}  [n]-dimensional Euclidean space.[92][100][104] If the mean
of any increment is zero, then the resulting Wiener or Brownian motion process
is said to have zero drift. If the mean of the increment for any two points in
time is equal to the time difference multiplied by some constant     &#x03BC;
{\displaystyle \mu }  [\mu ], which is a real number, then the resulting
stochastic process is said to have drift     &#x03BC;   {\displaystyle \mu }
[\mu ].[105][106][107]
Almost_surely, a sample path of a Wiener process is continuous everywhere but
nowhere_differentiable. It can be considered as a continuous version of the
simple random walk.[50][106] The process arises as the mathematical limit of
other stochastic processes such as certain random walks rescaled,[108][109]
which is the subject of Donsker's_theorem or invariance principle, also known
as the functional central limit theorem.[110][111][112]
The Wiener process is a member of some important families of stochastic
processes, including Markov processes, LÃ©vy processes and Gaussian processes.
[2][50] The process also has many applications and is the main stochastic
process used in stochastic calculus.[113][114] It plays a central role in
quantitative finance,[115][116] where it is used, for example, in the
BlackâScholesâMerton model.[117] The process is also used in different
fields, including the majority of natural sciences as well as some branches of
social sciences, as a mathematical model for various random phenomena.[3][118]
[119]
**** Poisson process[edit] ****
Main article: Poisson_process
The Poisson process is a stochastic process that has different forms and
definitions.[120][121] It can be defined as a counting process, which is a
stochastic process that represents the random number of points or events up to
some time. The number of points of the process that are located in the interval
from zero to some given time is a Poisson random variable that depends on that
time and some parameter. This process has the natural numbers as its state
space and the non-negative numbers as its index set. This process is also
called the Poisson counting process, since it can be interpreted as an example
of a counting process.[120]
If a Poisson process is defined with a single positive constant, then the
process is called a homogeneous Poisson process.[120][122] The homogeneous
Poisson process is a member of important classes of stochastic processes such
as Markov processes and LÃ©vy processes.[50]
The homogeneous Poisson process can be defined and generalized in different
ways. It can be defined such that its index set is the real line, and this
stochastic process is also called the stationary Poisson process.[123][124] If
the parameter constant of the Poisson process is replaced with some non-
negative integrable function of     t   {\displaystyle t}  [t], the resulting
process is called an inhomogeneous or nonhomogeneous Poisson process, where the
average density of points of the process is no longer constant.[125] Serving as
a fundamental process in queueing theory, the Poisson process is an important
process for mathematical models, where it finds applications for models of
events randomly occurring in certain time windows.[126][127]
Defined on the real line, the Poisson process can be interpreted as a
stochastic process,[50][128] among other random objects.[129][130] But then it
can be defined on the     n   {\displaystyle n}  [n]-dimensional Euclidean
space or other mathematical spaces,[131] where it is often interpreted as a
random set or a random counting measure, instead of a stochastic process.[129]
[130] In this setting, the Poisson process, also called the Poisson point
process, is one of the most important objects in probability theory, both for
applications and theoretical reasons.[23][132] But it has been remarked that
the Poisson process does not receive as much attention as it should, partly due
to it often being considered just on the real line, and not on other
mathematical spaces.[132][133]
***** Definitions[edit] *****
**** Stochastic process[edit] ****
A stochastic process is defined as a collection of random variables defined on
a common probability_space     ( &#x03A9; ,   F   , P )   {\displaystyle
(\Omega ,{\mathcal {F}},P)}  [(\Omega ,{\mathcal {F}},P)], where     &#x03A9;
{\displaystyle \Omega }  [\Omega ] is a sample_space,       F
{\displaystyle {\mathcal {F}}}  [{\mathcal {F}}] is a     &#x03C3;
{\displaystyle \sigma }  [\sigma ]-algebra, and     P   {\displaystyle P}  [P]
is a probability_measure; and the random variables, indexed by some set     T
{\displaystyle T}  [T], all take values in the same mathematical space     S
{\displaystyle S}  [S], which must be measurable with respect to some
&#x03C3;   {\displaystyle \sigma }  [\sigma ]-algebra     &#x03A3;
{\displaystyle \Sigma }  [\Sigma ].[29]
In other words, for a given probability space     ( &#x03A9; ,   F   , P )
{\displaystyle (\Omega ,{\mathcal {F}},P)}  [(\Omega ,{\mathcal {F}},P)] and a
measurable space     ( S , &#x03A3; )   {\displaystyle (S,\Sigma )}  [(S,\Sigma
)], a stochastic process is a collection of     S   {\displaystyle S}  [S]-
valued random variables, which can be written as:[81]
        { X ( t ) : t &#x2208; T } .   {\displaystyle \{X(t):t\in T\}.}  [
                       {\displaystyle \{X(t):t\in T\}.}]
Historically, in many problems from the natural sciences a point     t &#x2208;
T   {\displaystyle t\in T}  [t\in T] had the meaning of time, so     X ( t )
{\displaystyle X(t)}  [X(t)] is a random variable representing a value observed
at time     t   {\displaystyle t}  [t].[134] A stochastic process can also be
written as     { X ( t , &#x03C9; ) : t &#x2208; T }   {\displaystyle \{X
(t,\omega ):t\in T\}}  [{\displaystyle \{X(t,\omega ):t\in T\}}] to reflect
that it is actually a function of two variables,     t &#x2208; T
{\displaystyle t\in T}  [t\in T] and     &#x03C9; &#x2208; &#x03A9;
{\displaystyle \omega \in \Omega }  [{\displaystyle \omega \in \Omega }].[29]
[135]
There are others ways to consider a stochastic process, with the above
definition being considered the traditional one.[69][70] For example, a
stochastic process can be interpreted or defined as a      S  T
{\displaystyle S^{T}}  [{\displaystyle S^{T}}]-valued random variable, where
S  T     {\displaystyle S^{T}}  [{\displaystyle S^{T}}] is the space of all the
possible     S   {\displaystyle S}  [S]-valued functions of     t &#x2208; T
{\displaystyle t\in T}  [t\in T] that map from the set     T   {\displaystyle
T}  [T] into the space     S   {\displaystyle S}  [S].[28][69]
**** Index set[edit] ****
The set     T   {\displaystyle T}  [T] is called the index set[4][52] or
parameter set[29][136] of the stochastic process. Often this set is some subset
of the real_line, such as the natural_numbers or an interval, giving the set
T   {\displaystyle T}  [T] the interpretation of time.[1] In addition to these
sets, the index set     T   {\displaystyle T}  [T] can be other linearly
ordered sets or more general mathematical sets,[1][55] such as the Cartesian
plane      R  2     {\displaystyle R^{2}}  [R^{2}] or     n   {\displaystyle n}
[n]-dimensional Euclidean space, where an element     t &#x2208; T
{\displaystyle t\in T}  [t\in T] can represent a point in space.[49][137] But
in general more results and theorems are possible for stochastic processes when
the index set is ordered.[138]
**** State space[edit] ****
The mathematical_space     S   {\displaystyle S}  [S] of a stochastic process
is called its state space. This mathematical space can be defined using
integers, real_lines,     n   {\displaystyle n}  [n]-dimensional Euclidean
spaces, complex planes, or more abstract mathematical spaces. The state space
is defined using elements that reflect the different values that the stochastic
process can take. [1][5][29][52][57]
**** Sample function[edit] ****
A sample function is a single outcome of a stochastic process, so it is formed
by taking a single possible value of each random variable of the stochastic
process.[29][139] More precisely, if     { X ( t , &#x03C9; ) : t &#x2208; T }
{\displaystyle \{X(t,\omega ):t\in T\}}  [{\displaystyle \{X(t,\omega ):t\in
T\}}] is a stochastic process, then for any point     &#x03C9; &#x2208;
&#x03A9;   {\displaystyle \omega \in \Omega }  [\omega \in \Omega ], the
mapping
   X ( &#x22C5; , &#x03C9; ) : T &#x2192; S ,   {\displaystyle X(\cdot ,\omega
    ):T\rightarrow S,}  [{\displaystyle X(\cdot ,\omega ):T\rightarrow S,}]
is called a sample function, a realization, or, particularly when     T
{\displaystyle T}  [T] is interpreted as time, a sample path of the stochastic
process     { X ( t , &#x03C9; ) : t &#x2208; T }   {\displaystyle \{X(t,\omega
):t\in T\}}  [{\displaystyle \{X(t,\omega ):t\in T\}}].[51] This means that for
a fixed     &#x03C9; &#x2208; &#x03A9;   {\displaystyle \omega \in \Omega }
[\omega \in \Omega ], there exists a sample function that maps the index set
T   {\displaystyle T}  [T] to the state space     S   {\displaystyle S}  [S].
[29] Other names for a sample function of a stochastic process include
trajectory, path function[140] or path.[141]
**** Increment[edit] ****
An increment of a stochastic process is the difference between two random
variables of the same stochastic process. For a stochastic process with an
index set that can be interpreted as time, an increment is how much the
stochastic process changes over a certain time period. For example, if     { X
( t ) : t &#x2208; T }   {\displaystyle \{X(t):t\in T\}}  [{\displaystyle \{X
(t):t\in T\}}] is a stochastic process with state space     S   {\displaystyle
S}  [S] and index set     T = [ 0 , &#x221E; )   {\displaystyle T=[0,\infty )}
[{\displaystyle T=[0,\infty )}], then for any two non-negative numbers      t
1   &#x2208; [ 0 , &#x221E; )   {\displaystyle t_{1}\in [0,\infty )}  [
{\displaystyle t_{1}\in [0,\infty )}] and      t  2   &#x2208; [ 0 , &#x221E; )
{\displaystyle t_{2}\in [0,\infty )}  [{\displaystyle t_{2}\in [0,\infty )}]
such that      t  1   &#x2264;  t  2     {\displaystyle t_{1}\leq t_{2}}  [
{\displaystyle t_{1}\leq t_{2}}], the difference      X   t  2     &#x2212;  X
t  1       {\displaystyle X_{t_{2}}-X_{t_{1}}}  [{\displaystyle X_{t_{2}}-X_{t_
{1}}}] is a     S   {\displaystyle S}  [S]-valued random variable known as an
increment.[49][50] When interested in the increments, often the state space
S   {\displaystyle S}  [S] is the real line or the natural numbers, but it can
be     n   {\displaystyle n}  [n]-dimensional Euclidean space or more abstract
spaces such as Banach_spaces.[50]
**** Further definitions[edit] ****
*** Law[edit] ***
For a stochastic process     X &#x003A; &#x03A9; &#x2192;  S  T
{\displaystyle X\colon \Omega \rightarrow S^{T}}  [{\displaystyle X\colon
\Omega \rightarrow S^{T}}] defined on the probability space     ( &#x03A9; ,
F   , P )   {\displaystyle (\Omega ,{\mathcal {F}},P)}  [(\Omega ,{\mathcal
{F}},P)], the law of stochastic process     X   {\displaystyle X}  [X] is
defined as the image_measure:
    &#x03BC; = P &#x2218;  X  &#x2212; 1   ,   {\displaystyle \mu =P\circ X^{-
                  1},}  [{\displaystyle \mu =P\circ X^{-1},}]
where     P   {\displaystyle P}  [P] is a probability measure, the symbol
&#x2218;   {\displaystyle \circ }  [\circ ] denotes function composition and
X  &#x2212; 1     {\displaystyle X^{-1}}  [{\displaystyle X^{-1}}] is the pre-
image of the measurable function or, equivalently, the      S  T
{\displaystyle S^{T}}  [{\displaystyle S^{T}}]-valued random variable     X
{\displaystyle X}  [X], where      S  T     {\displaystyle S^{T}}  [
{\displaystyle S^{T}}] is the space of all the possible     S   {\displaystyle
S}  [S]-valued functions of     t &#x2208; T   {\displaystyle t\in T}  [t\in
T], so the law of a stochastic process is a probability measure.[28][69][142]
[143]
For a measurable subset     B   {\displaystyle B}  [B] of      S  T
{\displaystyle S^{T}}  [{\displaystyle S^{T}}], the pre-image of     X
{\displaystyle X}  [X] gives
       X  &#x2212; 1   ( B ) = { &#x03C9; &#x2208; &#x03A9; : X ( &#x03C9; )
 &#x2208; B } ,   {\displaystyle X^{-1}(B)=\{\omega \in \Omega :X(\omega )\in
  B\},}  [{\displaystyle X^{-1}(B)=\{\omega \in \Omega :X(\omega )\in B\},}]
so the law of a     X   {\displaystyle X}  [X] can be written as:[29]
   &#x03BC; ( B ) = P ( { &#x03C9; &#x2208; &#x03A9; : X ( &#x03C9; ) &#x2208;
B } ) .   {\displaystyle \mu (B)=P(\{\omega \in \Omega :X(\omega )\in B\}).}  [
      {\displaystyle \mu (B)=P(\{\omega \in \Omega :X(\omega )\in B\}).}]
The law of a stochastic process or a random variable is also called the
probability law, probability distribution, or the distribution.[134][142][144]
[145][146]
*** Finite-dimensional probability distributions[edit] ***
Main article: Finite-dimensional_distribution
For a stochastic process     X   {\displaystyle X}  [X] with law     &#x03BC;
{\displaystyle \mu }  [\mu ], its finite-dimensional distributions are defined
as:
     &#x03BC;   t  1   , &#x2026; ,  t  n     = P &#x2218; ( X (   t  1    ) ,
    &#x2026; , X (   t  n    )  )  &#x2212; 1   ,   {\displaystyle \mu _{t_
{1},\dots ,t_{n}}=P\circ (X({t_{1}}),\dots ,X({t_{n}}))^{-1},}  [{\displaystyle
    \mu _{t_{1},\dots ,t_{n}}=P\circ (X({t_{1}}),\dots ,X({t_{n}}))^{-1},}]
where     n &#x2265; 1   {\displaystyle n\geq 1}  [n\geq 1] is a counting
number and each set      t  i     {\displaystyle t_{i}}  [t_{i}] is a non-empty
finite subset of the index set     T   {\displaystyle T}  [T], so each      t
i   &#x2282; T   {\displaystyle t_{i}\subset T}  [{\displaystyle t_{i}\subset
T}], which means that      t  1   , &#x2026; ,  t  n     {\displaystyle t_
{1},\dots ,t_{n}}  [{\displaystyle t_{1},\dots ,t_{n}}] is any finite
collection of subsets of the index set     T   {\displaystyle T}  [T].[28][147]
For any measurable subset     C   {\displaystyle C}  [C] of the     n
{\displaystyle n}  [n]-fold Cartesian_power      S  n   = S &#x00D7; &#x22EF;
&#x00D7; S   {\displaystyle S^{n}=S\times \dots \times S}  [{\displaystyle S^
{n}=S\times \dots \times S}], the finite-dimensional distributions of a
stochastic process     X   {\displaystyle X}  [X] can be written as:[29]
      &#x03BC;   t  1   , &#x2026; ,  t  n     ( C ) = P   (     {   &#x03C9;
  &#x2208; &#x03A9; :   (    X   t  1     ( &#x03C9; ) , &#x2026; ,  X   t  n
( &#x03C9; )   )   &#x2208; C   }     )   .   {\displaystyle \mu _{t_{1},\dots
   ,t_{n}}(C)=P{\Big (}{\big \{}\omega \in \Omega :{\big (}X_{t_{1}}(\omega
 ),\dots ,X_{t_{n}}(\omega ){\big )}\in C{\big \}}{\Big )}.}  [{\displaystyle
\mu _{t_{1},\dots ,t_{n}}(C)=P{\Big (}{\big \{}\omega \in \Omega :{\big (}X_{t_
   {1}}(\omega ),\dots ,X_{t_{n}}(\omega ){\big )}\in C{\big \}}{\Big )}.}]
The finite-dimensional distributions of a stochastic process satisfy two
mathematical conditions known as consistency conditions.[58]
*** Stationarity[edit] ***
Main article: Stationary_process
Stationarity is a mathematical property that a stochastic process has when all
the random variables of that stochastic process are identically distributed. In
other words, if     X   {\displaystyle X}  [X] is a stationary stochastic
process, then for any     t &#x2208; T   {\displaystyle t\in T}  [t\in T] the
random variable      X  t     {\displaystyle X_{t}}  [X_{t}] has the same
distribution, which means that for any set of     n   {\displaystyle n}  [n]
index set values      t  1   , &#x2026; ,  t  n     {\displaystyle t_{1},\dots
,t_{n}}  [{\displaystyle t_{1},\dots ,t_{n}}], the corresponding     n
{\displaystyle n}  [n] random variables
    X   t  1     , &#x2026;  X   t  n     ,   {\displaystyle X_{t_{1}},\dots X_
            {t_{n}},}  [{\displaystyle X_{t_{1}},\dots X_{t_{n}},}]
all have the same probability_distribution. The index set of a stationary
stochastic process is usually interpreted as time, so it can be the integers or
the real line.[148][149] But the concept of stationarity also exists for point
processes and random fields, where the index set is not interpreted as time.
[148][150][151]
When the index set     T   {\displaystyle T}  [T] can be interpreted as time, a
stochastic process is said to be stationary if its finite-dimensional
distributions are invariant under translations of time. This type of stochastic
process can be used to describe a physical system that is in steady state, but
still experiences random fluctuations.[148] The intuition behind stationarity
is that as time passes the distribution of the stationary stochastic process
remains the same.[152] A sequence of random variables forms a stationary
stochastic process only if the random variables are identically distributed.
[148]
A stochastic process with the above definition of stationarity is sometimes
said to be strictly stationary, but there are other forms of stationarity. One
example is when a discrete-time or continuous-time stochastic process     X
{\displaystyle X}  [X] is said to be stationary in the wide sense, then the
process     X   {\displaystyle X}  [X] has a finite second moment for all     t
&#x2208; T   {\displaystyle t\in T}  [t\in T] and the covariance of the two
random variables      X  t     {\displaystyle X_{t}}  [X_{t}] and      X  t + h
{\displaystyle X_{t+h}}  [{\displaystyle X_{t+h}}] depends only on the number
h   {\displaystyle h}  [h] for all     t &#x2208; T   {\displaystyle t\in T}
[t\in T].[152][153] Khinchin introduced the related concept of stationarity in
the wide sense, which has other names including covariance stationarity or
stationarity in the broad sense.[153][154]
*** Filtration[edit] ***
A filtration is an increasing sequence of sigma-algebras defined in relation to
some probability space and an index set that has some total_order relation,
such in the case of the index set being some subset of the real numbers. More
formally, if a stochastic process has an index set with a total order, then a
filtration     {    F    t    }  t &#x2208; T     {\displaystyle \{{\mathcal
{F}}_{t}\}_{t\in T}}  [{\displaystyle \{{\mathcal {F}}_{t}\}_{t\in T}}], on a
probability space     ( &#x03A9; ,   F   , P )   {\displaystyle (\Omega ,
{\mathcal {F}},P)}  [(\Omega ,{\mathcal {F}},P)] is a family of sigma-algebras
such that        F    s   &#x2286;    F    t   &#x2286;   F     {\displaystyle
{\mathcal {F}}_{s}\subseteq {\mathcal {F}}_{t}\subseteq {\mathcal {F}}}  [
{\displaystyle {\mathcal {F}}_{s}\subseteq {\mathcal {F}}_{t}\subseteq
{\mathcal {F}}}] for all     s &#x2264; t   {\displaystyle s\leq t}  [s\leq t],
where     t , s &#x2208; T   {\displaystyle t,s\in T}  [{\displaystyle t,s\in
T}] and     &#x2264;   {\displaystyle \leq }  [\leq ] denotes the total order
of the index set     T   {\displaystyle T}  [T].[52] With the concept of a
filtration, it is possible to study the amount of information contained in a
stochastic process      X  t     {\displaystyle X_{t}}  [X_{t}] at     t
&#x2208; T   {\displaystyle t\in T}  [t\in T], which can be interpreted as time
t   {\displaystyle t}  [t].[52][155] The intuition behind a filtration        F
t     {\displaystyle {\mathcal {F}}_{t}}  [{\mathcal {F}}_{t}] is that as time
t   {\displaystyle t}  [t] passes, more and more information on      X  t
{\displaystyle X_{t}}  [X_{t}] is known or available, which is captured in
F    t     {\displaystyle {\mathcal {F}}_{t}}  [{\mathcal {F}}_{t}], resulting
in finer and finer partitions of     &#x03A9;   {\displaystyle \Omega }
[\Omega ].[156][157]
*** Modification[edit] ***
A modification of a stochastic process is another stochastic process, which is
closely related to the original stochastic process. More precisely, a
stochastic process     X   {\displaystyle X}  [X] that has the same index set
T   {\displaystyle T}  [T], set space     S   {\displaystyle S}  [S], and
probability space     ( &#x03A9; ,   F   , P )   {\displaystyle (\Omega ,{\cal
{F}},P)}  [{\displaystyle (\Omega ,{\cal {F}},P)}] as another stochastic
process     Y   {\displaystyle Y}  [Y] is said to be a modification of     Y
{\displaystyle Y}  [Y] if for all     t &#x2208; T   {\displaystyle t\in T}
[t\in T] the following
       P (  X  t   =  Y  t   ) = 1 ,   {\displaystyle P(X_{t}=Y_{t})=1,}  [
                      {\displaystyle P(X_{t}=Y_{t})=1,}]
holds. Two stochastic processes that are modifications of each other have the
same law[158] and they are said to be stochastically equivalent or equivalent.
[159]
Instead of modification, the term version is also used,[150][160][161][162]
however some authors use the term version when two stochastic processes have
the same finite-dimensional distributions, but they may be defined on different
probability spaces, so two processes that are modifications of each other, are
also versions of each other, in the latter sense, but not the converse.[163]
[142]
If a continuous-time real-valued stochastic process meets certain moment
conditions on its increments, then the Kolmogorov_continuity_theorem says that
there exists a modification of this process that has continuous sample paths
with probability one, so the stochastic process has a continuous modification
or version.[161][162][164] The theorem can also be generalized to random fields
so the index set is     n   {\displaystyle n}  [n]-dimensional Euclidean space
[165] as well as to stochastic processes with metric_spaces as their state
spaces.[166]
*** Indistinguishable[edit] ***
Two stochastic processes     X   {\displaystyle X}  [X] and     Y
{\displaystyle Y}  [Y] defined on the same probability space     ( &#x03A9; ,
F   , P )   {\displaystyle (\Omega ,{\mathcal {F}},P)}  [(\Omega ,{\mathcal
{F}},P)] with the same index set     T   {\displaystyle T}  [T] and set space
S   {\displaystyle S}  [S] are said be indistinguishable if the following
       P (  X  t   =  Y  t    &#xA0;for all&#xA0;  t &#x2208; T ) = 1 ,
{\displaystyle P(X_{t}=Y_{t}{\text{ for all }}t\in T)=1,}  [{\displaystyle P(X_
                    {t}=Y_{t}{\text{ for all }}t\in T)=1,}]
holds.[142][158] If two     X   {\displaystyle X}  [X] and     Y
{\displaystyle Y}  [Y] are modifications of each other and are almost surely
continuous, then     X   {\displaystyle X}  [X] and     Y   {\displaystyle Y}
[Y] are indistinguishable.[167]
*** Separability[edit] ***
Separability is a property of a stochastic process based on its index set in
relation to the probability measure. The property is assumed so that
functionals of stochastic processes or random fields with uncountable index
sets can form random variables. For a stochastic process to be separable, in
addition to other conditions, its index set must be a separable_space,[b] which
means that the index set has a dense countable subset.[150][168]
More precisely, a real-valued continuous-time stochastic process     X
{\displaystyle X}  [X] with a probability space     ( &#x03A9; ,   F   , P )
{\displaystyle (\Omega ,{\cal {F}},P)}  [{\displaystyle (\Omega ,{\cal
{F}},P)}] is separable if its index set     T   {\displaystyle T}  [T] has a
dense countable subset     U &#x2282; T   {\displaystyle U\subset T}  [
{\displaystyle U\subset T}] and there is a set      &#x03A9;  0   &#x2282;
&#x03A9;   {\displaystyle \Omega _{0}\subset \Omega }  [{\displaystyle \Omega _
{0}\subset \Omega }] of probability zero, so     P (  &#x03A9;  0   ) = 0
{\displaystyle P(\Omega _{0})=0}  [{\displaystyle P(\Omega _{0})=0}], such that
for every open set     G &#x2282; T   {\displaystyle G\subset T}  [
{\displaystyle G\subset T}] and every closed set     F &#x2282;  R = ( &#x2212;
&#x221E; , &#x221E; )    {\displaystyle F\subset \textstyle R=(-\infty ,\infty
)}  [{\displaystyle F\subset \textstyle R=(-\infty ,\infty )}], the two events
{  X  t   &#x2208; F  &#xA0;for all&#xA0;  t &#x2208; G &#x2229; U }
{\displaystyle \{X_{t}\in F{\text{ for all }}t\in G\cap U\}}  [{\displaystyle \
{X_{t}\in F{\text{ for all }}t\in G\cap U\}}] and     {  X  t   &#x2208; F
&#xA0;for all&#xA0;  t &#x2208; G }   {\displaystyle \{X_{t}\in F{\text{ for
all }}t\in G\}}  [{\displaystyle \{X_{t}\in F{\text{ for all }}t\in G\}}]
differ from each other at most on a subset of      &#x03A9;  0
{\displaystyle \Omega _{0}}  [\Omega _{0}].[169][170][171] The definition of
separability[c] can also be stated for other index sets and state spaces,[174]
such as in the case of random fields, where the index set as well as the state
space can be     n   {\displaystyle n}  [n]-dimensional Euclidean space.[31]
[150]
The concept of separability of a stochastic process was introduced by Joseph
Doob,[168] where the underlying idea is to make a countable set of points of
the index set determine the properties of the stochastic process.[172] Any
stochastic process with a countable index set already meets the separability
conditions, so discrete-time stochastic processes are always separable.[175] A
theorem by Doob, sometimes known as Doob's separability theorem, says that any
real-valued continuous-time stochastic process has a separable modification.
[168][170][176] Versions of this theorem also exist for more general stochastic
processes with index sets and state spaces other than the real line.[136]
*** Independence[edit] ***
Two stochastic processes     X   {\displaystyle X}  [X] and     Y
{\displaystyle Y}  [Y] defined on the same probability space     ( &#x03A9; ,
F   , P )   {\displaystyle (\Omega ,{\mathcal {F}},P)}  [(\Omega ,{\mathcal
{F}},P)] with the same index set     T   {\displaystyle T}  [T] are said be
independent if for all     n &#x2208;  N    {\displaystyle n\in \mathbb {N} }
[n\in \mathbb {N} ] and for every choice of epochs      t  1   , &#x2026; ,  t
n   &#x2208; T   {\displaystyle t_{1},\ldots ,t_{n}\in T}  [{\displaystyle t_
{1},\ldots ,t_{n}\in T}], the random vectors      (  X (  t  1   ) , &#x2026; ,
X (  t  n   )  )    {\displaystyle \left(X(t_{1}),\ldots ,X(t_{n})\right)}  [
{\displaystyle \left(X(t_{1}),\ldots ,X(t_{n})\right)}] and      (  Y (  t  1
) , &#x2026; , Y (  t  n   )  )    {\displaystyle \left(Y(t_{1}),\ldots ,Y(t_
{n})\right)}  [{\displaystyle \left(Y(t_{1}),\ldots ,Y(t_{n})\right)}] are
independent.[177]:p. 515
*** Uncorrelatedness[edit] ***
Two stochastic processes      {  X  t   }    {\displaystyle \left\{X_
{t}\right\}}  [\left\{X_{t}\right\}] and      {  Y  t   }    {\displaystyle
\left\{Y_{t}\right\}}  [{\displaystyle \left\{Y_{t}\right\}}] are called
uncorrelated if their cross-covariance      K   X   Y    &#x2061; (  t  1   ,
t  2   ) = E &#x2061;  [   (  X (  t  1   ) &#x2212;  &#x03BC;  X   (  t  1   )
)   (  Y (  t  2   ) &#x2212;  &#x03BC;  Y   (  t  2   )  )   ]
{\displaystyle \operatorname {K} _{\mathbf {X} \mathbf {Y} }(t_{1},t_
{2})=\operatorname {E} \left[\left(X(t_{1})-\mu _{X}(t_{1})\right)\left(Y(t_
{2})-\mu _{Y}(t_{2})\right)\right]}  [{\displaystyle \operatorname {K} _
{\mathbf {X} \mathbf {Y} }(t_{1},t_{2})=\operatorname {E} \left[\left(X(t_{1})-
\mu _{X}(t_{1})\right)\left(Y(t_{2})-\mu _{Y}(t_{2})\right)\right]}] is zero
for all times.[178]:p. 142 Formally:
          {  X  t   }  ,  {  Y  t   }   &#xA0;uncorrelated    &#x27FA;    K   X
      Y    &#x2061; (  t  1   ,  t  2   ) = 0  &#x2200;  t  1   ,  t  2
      {\displaystyle \left\{X_{t}\right\},\left\{Y_{t}\right\}{\text
      { uncorrelated}}\quad \iff \quad \operatorname {K} _{\mathbf {X} \mathbf
      {Y} }(t_{1},t_{2})=0\quad \forall t_{1},t_{2}}  [{\displaystyle \left\{X_
      {t}\right\},\left\{Y_{t}\right\}{\text{ uncorrelated}}\quad \iff \quad
      \operatorname {K} _{\mathbf {X} \mathbf {Y} }(t_{1},t_{2})=0\quad \forall
      t_{1},t_{2}}].
*** Independence implies uncorrelatedness[edit] ***
If two stochastic processes     X   {\displaystyle X}  [X] and     Y
{\displaystyle Y}  [Y] are independent, then they are also uncorrelated.[178]:
p. 151
*** Orthogonality[edit] ***
Two stochastic processes      {  X  t   }    {\displaystyle \left\{X_
{t}\right\}}  [\left\{X_{t}\right\}] and      {  Y  t   }    {\displaystyle
\left\{Y_{t}\right\}}  [{\displaystyle \left\{Y_{t}\right\}}] are called
orthogonal if their cross-correlation      R   X   Y    &#x2061; (  t  1   ,  t
2   ) = E &#x2061; [ X (  t  1   )    Y (  t  2   )  &#x00AF;   ]
{\displaystyle \operatorname {R} _{\mathbf {X} \mathbf {Y} }(t_{1},t_
{2})=\operatorname {E} [X(t_{1}){\overline {Y(t_{2})}}]}  [{\displaystyle
\operatorname {R} _{\mathbf {X} \mathbf {Y} }(t_{1},t_{2})=\operatorname {E} [X
(t_{1}){\overline {Y(t_{2})}}]}] is zero for all times.[178]:p. 142 Formally:
          {  X  t   }  ,  {  Y  t   }   &#xA0;orthogonal    &#x27FA;    R   X
      Y    &#x2061; (  t  1   ,  t  2   ) = 0  &#x2200;  t  1   ,  t  2
      {\displaystyle \left\{X_{t}\right\},\left\{Y_{t}\right\}{\text
      { orthogonal}}\quad \iff \quad \operatorname {R} _{\mathbf {X} \mathbf
      {Y} }(t_{1},t_{2})=0\quad \forall t_{1},t_{2}}  [{\displaystyle \left\{X_
      {t}\right\},\left\{Y_{t}\right\}{\text{ orthogonal}}\quad \iff \quad
      \operatorname {R} _{\mathbf {X} \mathbf {Y} }(t_{1},t_{2})=0\quad \forall
      t_{1},t_{2}}].
*** Skorokhod space[edit] ***
Main article: Skorokhod_space
A Skorokhod space, also written as Skorohod space, is a mathematical space of
all the functions that are right-continuous with left limits, defined on some
interval of the real line such as     [ 0 , 1 ]   {\displaystyle [0,1]}  [
[0,1]] or     [ 0 , &#x221E; )   {\displaystyle [0,\infty )}  [[0,\infty )],
and take values on the real line or on some metric space.[179][180][181] Such
functions are known as cÃ dlÃ g or cadlag functions, based on the acronym of
the French expression continue Ã  droite, limite Ã  gauche, due to the
functions being right-continuous with left limits.[179][182] A Skorokhod
function space, introduced by Anatoliy_Skorokhod,[181] is often denoted with
the letter     D   {\displaystyle D}  [D],[179][180][181][182] so the function
space is also referred to as space     D   {\displaystyle D}  [D].[179][183]
[184] The notation of this function space can also include the interval on
which all the cÃ dlÃ g functions are defined, so, for example,     D [ 0 , 1 ]
{\displaystyle D[0,1]}  [{\displaystyle D[0,1]}] denotes the space of cÃ dlÃ g
functions defined on the unit_interval     [ 0 , 1 ]   {\displaystyle [0,1]}  [
[0,1]].[182][184][185]
Skorokhod function spaces are frequently used in the theory of stochastic
processes because it often assumed that the sample functions of continuous-time
stochastic processes belong to a Skorokhod space.[181][183] Such spaces contain
continuous functions, which correspond to sample functions of the Wiener
process. But the space also has functions with discontinuities, which means
that the sample functions of stochastic processes with jumps, such as the
Poisson process (on the real line), are also members of this space.[184][186]
*** Regularity[edit] ***
In the context of mathematical construction of stochastic processes, the term
regularity is used when discussing and assuming certain conditions for a
stochastic process to resolve possible construction issues.[187][188] For
example, to study stochastic processes with uncountable index sets, it is
assumed that the stochastic process adheres to some type of regularity
condition such as the sample functions being continuous.[189][190]
***** Further examples[edit] *****
**** Markov processes and chains[edit] ****
Main article: Markov_process
Markov processes are stochastic processes, traditionally in discrete_or
continuous_time, that have the Markov property, which means the next value of
the Markov process depends on the current value, but it is conditionally
independent of the previous values of the stochastic process. In other words,
the behavior of the process in the future is stochastically independent of its
behavior in the past, given the current state of the process.[191][192]
The Brownian motion process and the Poisson process (in one dimension) are both
examples of Markov processes[193] in continuous time, while random_walks on the
integers and the gambler's_ruin problem are examples of Markov processes in
discrete time.[194][195]
A Markov chain is a type of Markov process that has either discrete state_space
or discrete index set (often representing time), but the precise definition of
a Markov chain varies.[196] For example, it is common to define a Markov chain
as a Markov process in either discrete_or_continuous_time with a countable
state space (thus regardless of the nature of time),[197][198][199][200] but it
has been also common to define a Markov chain as having discrete time in either
countable or continuous state space (thus regardless of the state space).[196]
It has been argued that the first definition of a Markov chain, where it has
discrete time, now tends to be used, despite the second definition having been
used by researchers like Joseph_Doob and Kai_Lai_Chung.[201]
Markov processes form an important class of stochastic processes and have
applications in many areas.[40][202] For example, they are the basis for a
general stochastic simulation method known as Markov_chain_Monte_Carlo, which
is used for simulating random objects with specific probability distributions,
and has found application in Bayesian_statistics.[203][204]
The concept of the Markov property was originally for stochastic processes in
continuous and discrete time, but the property has been adapted for other index
sets such as     n   {\displaystyle n}  [n]-dimensional Euclidean space, which
results in collections of random variables known as Markov random fields.[205]
[206][207]
**** Martingale[edit] ****
Main article: Martingale_(probability_theory)
A martingale is a discrete-time or continuous-time stochastic process with the
property that, at every instant, given the current value and all the past
values of the process, the conditional expectation of every future value is
equal to the current value. In discrete time, if this property holds for the
next value, then it holds for all future values. The exact mathematical
definition of a martingale requires two other conditions coupled with the
mathematical concept of a filtration, which is related to the intuition of
increasing available information as time passes. Martingales are usually
defined to be real-valued,[208][209][155] but they can also be complex-valued
[210] or even more general.[211]
A symmetric random walk and a Wiener process (with zero drift) are both
examples of martingales, respectively, in discrete and continuous time.[208]
[209] For a sequence of independent_and_identically_distributed random
variables      X  1   ,  X  2   ,  X  3   , &#x2026;   {\displaystyle X_{1},X_
{2},X_{3},\dots }  [X_{1},X_{2},X_{3},\dots ] with zero mean, the stochastic
process formed from the successive partial sums      X  1   ,  X  1   +  X  2
,  X  1   +  X  2   +  X  3   , &#x2026;   {\displaystyle X_{1},X_{1}+X_{2},X_
{1}+X_{2}+X_{3},\dots }  [{\displaystyle X_{1},X_{1}+X_{2},X_{1}+X_{2}+X_
{3},\dots }] is a discrete-time martingale.[212] In this aspect, discrete-time
martingales generalize the idea of partial sums of independent random
variables.[213]
Martingales can also be created from stochastic processes by applying some
suitable transformations, which is the case for the homogeneous Poisson process
(on the real line) resulting in a martingale called the compensated Poisson
process.[209] Martingales can also be built from other martingales.[212] For
example, there are martingales based on the martingale the Wiener process,
forming continuous-time martingales.[208][214]
Martingales mathematically formalize the idea of a fair game,[215] and they
were originally developed to show that it is not possible to win a fair game.
[216] But now they are used in many areas of probability, which is one of the
main reasons for studying them.[155][216][217] Many problems in probability
have been solved by finding a martingale in the problem and studying it.[218]
Martingales will converge, given some conditions on their moments, so they are
often used to derive convergence results, due largely to martingale_convergence
theorems.[213][219][220]
Martingales have many applications in statistics, but it has been remarked that
its use and application are not as widespread as it could be in the field of
statistics, particularly statistical inference.[221] They have found
applications in areas in probability theory such as queueing theory and Palm
calculus[222] and other fields such as economics[223] and finance.[18]
**** LÃ©vy process[edit] ****
Main article: LÃ©vy_process
LÃ©vy processes are types of stochastic processes that can be considered as
generalizations of random walks in continuous time.[50][224] These processes
have many applications in fields such as finance, fluid mechanics, physics and
biology.[225][226] The main defining characteristics of these processes are
their stationarity and independence properties, so they were known as processes
with stationary and independent increments. In other words, a stochastic
process     X   {\displaystyle X}  [X] is a LÃ©vy process if for     n
{\displaystyle n}  [n] non-negatives numbers,     0 &#x2264;  t  1   &#x2264;
&#x22EF; &#x2264;  t  n     {\displaystyle 0\leq t_{1}\leq \dots \leq t_{n}}  [
{\displaystyle 0\leq t_{1}\leq \dots \leq t_{n}}], the corresponding     n
&#x2212; 1   {\displaystyle n-1}  [n-1] increments
       X   t  2     &#x2212;  X   t  1     , &#x2026; ,  X   t  n &#x2212; 1
 &#x2212;  X   t  n     ,   {\displaystyle X_{t_{2}}-X_{t_{1}},\dots ,X_{t_{n-
 1}}-X_{t_{n}},}  [{\displaystyle X_{t_{2}}-X_{t_{1}},\dots ,X_{t_{n-1}}-X_{t_
                                    {n}},}]
are all independent of each other, and the distribution of each increment only
depends on the difference in time.[50]
A LÃ©vy process can be defined such that its state space is some abstract
mathematical space, such as a Banach_space, but the processes are often defined
so that they take values in Euclidean space. The index set is the non-negative
numbers, so     I = [ 0 , &#x221E; )   {\displaystyle I=[0,\infty )}  [
{\displaystyle I=[0,\infty )}], which gives the interpretation of time.
Important stochastic processes such as the Wiener process, the homogeneous
Poisson process (in one dimension), and subordinators are all LÃ©vy processes.
[50][224]
**** Random field[edit] ****
Main article: Random_field
A random field is a collection of random variables indexed by a     n
{\displaystyle n}  [n]-dimensional Euclidean space or some manifold. In
general, a random field can be considered an example of a stochastic or random
process, where the index set is not necessarily a subset of the real line.[31]
But there is a convention that an indexed collection of random variables is
called a random field when the index has two or more dimensions.[5][29][227] If
the specific definition of a stochastic process requires the index set to be a
subset of the real line, then the random field can be considered as a
generalization of stochastic process.[228]
**** Point process[edit] ****
Main article: Point_process
A point process is a collection of points randomly located on some mathematical
space such as the real line,     n   {\displaystyle n}  [n]-dimensional
Euclidean space, or more abstract spaces. Sometimes the term point process is
not preferred, as historically the word process denoted an evolution of some
system in time, so a point process is also called a random point field.[229]
There are different interpretations of a point process, such a random counting
measure or a random set.[230][231] Some authors regard a point process and
stochastic process as two different objects such that a point process is a
random object that arises from or is associated with a stochastic process,[232]
[233] though it has been remarked that the difference between point processes
and stochastic processes is not clear.[233]
Other authors consider a point process as a stochastic process, where the
process is indexed by sets of the underlying space[d] on which it is defined,
such as the real line or     n   {\displaystyle n}  [n]-dimensional Euclidean
space.[236][237] Other stochastic processes such as renewal and counting
processes are studied in the theory of point processes.[238][239]
***** History[edit] *****
**** Early probability theory[edit] ****
Probability theory has its origins in games of chance, which have a long
history, with some games being played thousands of years ago,[240][241] but
very little analysis on them was done in terms of probability.[240][242] The
year 1654 is often considered the birth of probability theory when French
mathematicians Pierre_Fermat and Blaise_Pascal had a written correspondence on
probability, motivated by a gambling problem.[240][243][244] But there was
earlier mathematical work done on the probability of gambling games such as
Liber de Ludo Aleae by Gerolamo_Cardano, written in the 16th century but
posthumously published later in 1663.[240][245]
After Cardano, Jakob_Bernoulli[e] wrote Ars_Conjectandi, which is considered a
significant event in the history of probability theory.[240] Bernoulli's book
was published, also posthumously, in 1713 and inspired many mathematicians to
study probability.[240][247][248] But despite some renown mathematicians
contributing to probability theory, such as Pierre-Simon_Laplace, Abraham_de
Moivre, Carl_Gauss, SimÃ©on_Poisson and Pafnuty_Chebyshev,[249][250] most of
the mathematical community[f] did not consider probability theory to be part of
mathematics until the 20th century.[249][251][252][253]
**** Statistical mechanics[edit] ****
In the physical sciences, scientists developed in the 19th century the
discipline of statistical_mechanics, where physical systems, such as containers
filled with gases, can be regarded or treated mathematically as collections of
many moving particles. Although there were attempts to incorporate randomness
into statistical physics by some scientists, such as Rudolf_Clausius, most of
the work had little or no randomness.[254][255] This changed in 1859 when James
Clerk_Maxwell contributed significantly to the field, more specifically, to the
kinetic theory of gases, by presenting work where he assumed the gas particles
move in random directions at random velocities.[256][257] The kinetic theory of
gases and statistical physics continued to be developed in the second half of
the 19th century, with work done chiefly by Clausius, Ludwig_Boltzmann and
Josiah_Gibbs, which would later have an influence on Albert_Einstein's
mathematical model for Brownian_movement.[258]
**** Measure theory and probability theory[edit] ****
At the International_Congress_of_Mathematicians in Paris in 1900, David_Hilbert
presented a list of mathematical_problems, where his sixth problem asked for a
mathematical treatment of physics and probability involving axioms.[250] Around
the start of the 20th century, mathematicians developed measure theory, a
branch of mathematics for studying integrals of mathematical functions, where
two of the founders were French mathematicians, Henri_Lebesgue and Ãmile
Borel. In 1925 another French mathematician Paul_LÃ©vy published the first
probability book that used ideas from measure theory.[250]
In 1920s fundamental contributions to probability theory were made in the
Soviet Union by mathematicians such as Sergei_Bernstein, Aleksandr_Khinchin,[g]
and Andrei_Kolmogorov.[253] Kolmogorov published in 1929 his first attempt at
presenting a mathematical foundation, based on measure theory, for probability
theory.[259] In the early 1930s Khinchin and Kolmogorov set up probability
seminars, which were attended by researchers such as Eugene_Slutsky and Nikolai
Smirnov,[260] and Khinchin gave the first mathematical definition of a
stochastic process as a set of random variables indexed by the real line.[64]
[261][h]
**** Birth of modern probability theory[edit] ****
In 1933 Andrei Kolmogorov published in German his book on the foundations of
probability theory titled Grundbegriffe der Wahrscheinlichkeitsrechnung,[i]
where Kolmogorov used measure theory to develop an axiomatic framework for
probability theory. The publication of this book is now widely considered to be
the birth of modern probability theory, when the theories of probability and
stochastic processes became parts of mathematics.[250][253]
After the publication of Kolmogorov's book, further fundamental work on
probability theory and stochastic processes was done by Khinchin and Kolmogorov
as well as other mathematicians such as Joseph_Doob, William_Feller, Maurice
FrÃ©chet, Paul_LÃ©vy, Wolfgang_Doeblin, and Harald_CramÃ©r.[250][253] Decades
later CramÃ©r referred to the 1930s as the "heroic period of mathematical
probability theory".[253] World_War_II greatly interrupted the development of
probability theory, causing, for example, the migration of Feller from Sweden
to the United_States_of_America[253] and the death of Doeblin, considered now a
pioneer in stochastic processes.[263]
Mathematician Joseph Doob did early work on the theory of stochastic processes,
making fundamental contributions, particularly in the theory of martingales.
[264][262] His book Stochastic Processes is considered highly influential in
the field of probability theory.[265]
**** Stochastic processes after World War II[edit] ****
After World War II the study of probability theory and stochastic processes
gained more attention from mathematicians, with significant contributions made
in many areas of probability and mathematics as well as the creation of new
areas.[253][266] Starting in the 1940s, Kiyosi_ItÃ´ published papers developing
the field of stochastic_calculus, which involves stochastic integrals and
stochastic differential_equations based on the Wiener or Brownian motion
process.[267]
Also starting in the 1940s, connections were made between stochastic processes,
particularly martingales, and the mathematical field of potential_theory, with
early ideas by Shizuo_Kakutani and then later work by Joseph Doob.[266] Further
work, considered pioneering, was done by Gilbert_Hunt in the 1950s, connecting
Markov processes and potential theory, which had a significant effect on the
theory of LÃ©vy processes and led to more interest in studying Markov processes
with methods developed by ItÃ´.[22][268][269]
In 1953 Doob published his book Stochastic processes, which had a strong
influence on the theory of stochastic processes and stressed the importance of
measure theory in probability.[266] [265] Doob also chiefly developed the
theory of martingales, with later substantial contributions by Paul-AndrÃ©
Meyer. Earlier work had been carried out by Sergei_Bernstein, Paul_LÃ©vy and
Jean_Ville, the latter adopting the term martingale for the stochastic process.
[270][271] Methods from the theory of martingales became popular for solving
various probability problems. Techniques and theory were developed to study
Markov processes and then applied to martingales. Conversely, methods from the
theory of martingales were established to treat Markov processes.[266]
Other fields of probability were developed and used to study stochastic
processes, with one main approach being the theory of large deviations.[266]
The theory has many applications in statistical physics, among other fields,
and has core ideas going back to at least the 1930s. Later in the 1960s and
1970s fundamental work was done by Alexander Wentzell in the Soviet Union and
Monroe_D._Donsker and Srinivasa_Varadhan in the United States of America,[272]
which would later result in Varadhan winning the 2007 Abel Prize.[273] In the
1990s and 2000s the theories of SchrammâLoewner_evolution[274] and rough
paths[142] were introduced and developed to study stochastic processes and
other mathematical objects in probability theory, which respectively resulted
in Fields_Medals being awarded to Wendelin_Werner[275] in 2008 and to Martin
Hairer in 2014.[276]
The theory of stochastic processes still continues to be a focus of research,
with yearly international conferences on the topic of stochastic processes.[46]
[225]
**** Discoveries of specific stochastic processes[edit] ****
Although Khinchin gave mathematical definitions of stochastic processes in the
1930s,[64][261] specific stochastic processes had already been discovered in
different settings, such as the Brownian motion process and the Poisson
process.[22][25] Some families of stochastic processes such as point processes
or renewal processes have long and complex histories, stretching back
centuries.[277]
*** Bernoulli process[edit] ***
The Bernoulli process, which can serve as a mathematical model for flipping a
biased coin, is possibly the first stochastic process to have been studied.[82]
The process is a sequence of independent Bernoulli trials,[83] which are named
after Jackob_Bernoulli who used them to study games of chance, including
probability problems proposed and studied earlier by Christiaan Huygens.[278]
Bernoulli's work, including the Bernoulli process, were published in his book
Ars Conjectandi in 1713.[279]
*** Random walks[edit] ***
In 1905 Karl_Pearson coined the term random walk while posing a problem
describing a random walk on the plane, which was motivated by an application in
biology, but such problems involving random walks had already been studied in
other fields. Certain gambling problems that were studied centuries earlier can
be considered as problems involving random walks.[90][279] For example, the
problem known as the Gambler's ruin is based on a simple random walk,[195][280]
and is an example of a random walk with absorbing barriers.[243][281] Pascal,
Fermat and Huyens all gave numerical solutions to this problem without
detailing their methods,[282] and then more detailed solutions were presented
by Jakob Bernoulli and Abraham_de_Moivre.[283]
For random walks in     n   {\displaystyle n}  [n]-dimensional integer
lattices, George_PÃ³lya published in 1919 and 1921 work, where he studied the
probability of a symmetric random walk returning to a previous position in the
lattice. PÃ³lya showed that a symmetric random walk, which has an equal
probability to advance in any direction in the lattice, will return to a
previous position in the lattice an infinite number of times with probability
one in one and two dimensions, but with probability zero in three or higher
dimensions.[284][285]
*** Wiener process[edit] ***
The Wiener_process or Brownian motion process has its origins in different
fields including statistics, finance and physics.[22] In 1880, Thorvald_Thiele
wrote a paper on the method of least squares, where he used the process to
study the errors of a model in time-series analysis.[286][287][288] The work is
now considered as an early discovery of the statistical method known as Kalman
filtering, but the work was largely overlooked. It is thought that the ideas in
Thiele's paper were too advanced to have been understood by the broader
mathematical and statistical community at the time.[288]
Norbert Wiener gave the first mathematical proof of the existence of the Wiener
process. This mathematical object had appeared previously in the work of
Thorvald_Thiele, Louis_Bachelier, and Albert_Einstein.[22]
The French mathematician Louis_Bachelier used a Wiener process in his 1900
thesis[289][290] in order to model price changes on the Paris_Bourse, a stock
exchange,[291] without knowing the work of Thiele.[22] It has been speculated
that Bachelier drew ideas from the random walk model of Jules_Regnault, but
Bachelier did not cite him,[292] and Bachelier's thesis is now considered
pioneering in the field of financial mathematics.[291][292]
It is commonly thought that Bachelier's work gained little attention and was
forgotten for decades until it was rediscovered in the 1950s by the Leonard
Savage, and then become more popular after Bachelier's thesis was translated
into English in 1964. But the work was never forgotten in the mathematical
community, as Bachelier published a book in 1912 detailing his ideas,[292]
which was cited by mathematicians including Doob, Feller[292] and Kolmogorov.
[22] The book continued to be cited, but then starting in the 1960s the
original thesis by Bachelier began to be cited more than his book when
economists started citing Bachelier's work.[292]
In 1905 Albert_Einstein published a paper where he studied the physical
observation of Brownian motion or movement to explain the seemingly random
movements of particles in liquids by using ideas from the kinetic_theory_of
gases. Einstein derived a differential_equation, known as a diffusion_equation,
for describing the probability of finding a particle in a certain region of
space. Shortly after Einstein's first paper on Brownian movement, Marian
Smoluchowski published work where he cited Einstein, but wrote that he had
independently derived the equivalent results by using a different method.[293]
Einstein's work, as well as experimental results obtained by Jean_Perrin, later
inspired Norbert Wiener in the 1920s[294] to use a type of measure theory,
developed by Percy_Daniell, and Fourier analysis to prove the existence of the
Wiener process as a mathematical object.[22]
*** Poisson process[edit] ***
The Poisson process is named after SimÃ©on_Poisson, due to its definition
involving the Poisson_distribution, but Poisson never studied the process.[23]
[295] There are a number of claims for early uses or discoveries of the Poisson
process.[23][25] At the beginning of the 20th century the Poisson process would
arise independently in different situations.[23][25] In Sweden 1903, Filip
Lundberg published a thesis containing work, now considered fundamental and
pioneering, where he proposed to model insurance claims with a homogeneous
Poisson process.[296][297]
Another discovery occurred in Denmark in 1909 when A.K._Erlang derived the
Poisson distribution when developing a mathematical model for the number of
incoming phone calls in a finite time interval. Erlang was not at the time
aware of Poisson's earlier work and assumed that the number phone calls
arriving in each interval of time were independent to each other. He then found
the limiting case, which is effectively recasting the Poisson distribution as a
limit of the binomial distribution.[23]
In 1910 Ernest_Rutherford and Hans_Geiger published experimental results on
counting alpha particles. Motivated by their work, Harry_Bateman studied the
counting problem and derived Poisson probabilities as a solution to a family of
differential equations, resulting in the independent discovery of the Poisson
process.[23] After this time there were many studies and applications of the
Poisson process, but its early history is complicated, which has been explained
by the various applications of the process in numerous fields by biologists,
ecologists, engineers and various physical scientists.[23]
*** Markov processes[edit] ***
Markov processes and Markov chains are named after Andrey_Markov who studied
Markov chains in the early 20th century.[298] Markov was interested in studying
an extension of independent random sequences.[298] In his first paper on Markov
chains, published in 1906, Markov showed that under certain conditions the
average outcomes of the Markov chain would converge to a fixed vector of
values, so proving a weak_law_of_large_numbers without the independence
assumption,[6][299][300][301] which had been commonly regarded as a requirement
for such mathematical laws to hold.[301] Markov later used Markov chains to
study the distribution of vowels in Eugene_Onegin, written by Alexander
Pushkin, and proved a central_limit_theorem for such chains.[6][299]
In 1912 PoincarÃ© studied Markov chains on finite_groups with an aim to study
card shuffling. Other early uses of Markov chains include a diffusion model,
introduced by Paul and Tatyana_Ehrenfest in 1907, and a branching process,
introduced by Francis_Galton and Henry_William_Watson in 1873, preceding the
work of Markov.[299][300] After the work of Galton and Watson, it was later
revealed that their branching process had been independently discovered and
studied around three decades earlier by IrÃ©nÃ©e-Jules_BienaymÃ©.[302] Starting
in 1928, Maurice_FrÃ©chet became interested in Markov chains, eventually
resulting in him publishing in 1938 a detailed study on Markov chains.[299]
[303]
Andrei_Kolmogorov developed in a 1931 paper a large part of the early theory of
continuous-time Markov processes.[253][259] Kolmogorov was partly inspired by
Louis Bachelier's 1900 work on fluctuations in the stock market as well as
Norbert_Wiener's work on Einstein's model of Brownian movement.[259][304] He
introduced and studied a particular set of Markov processes known as diffusion
processes, where he derived a set of differential equations describing the
processes.[259][305] Independent of Kolmogorov's work, Sydney_Chapman derived
in a 1928 paper an equation, now called the ChapmanâKolmogorov_equation, in a
less mathematically rigorous way than Kolmogorov, while studying Brownian
movement.[306] The differential equations are now called the Kolmogorov
equations[307] or the KolmogorovâChapman equations.[308] Other mathematicians
who contributed significantly to the foundations of Markov processes include
William Feller, starting in the 1930s, and then later Eugene Dynkin, starting
in the 1950s.[253]
*** LÃ©vy processes[edit] ***
LÃ©vy processes such as the Wiener process and the Poisson process (on the real
line) are named after Paul LÃ©vy who started studying them in the 1930s,[225]
but they have connections to infinitely_divisible_distributions going back to
the 1920s.[224] In a 1932 paper Kolmogorov derived a characteristic_function
for random variables associated with LÃ©vy processes. This result was later
derived under more general conditions by LÃ©vy in 1934, and then Khinchin
independently gave an alternative form for this characteristic function in
1937.[253][309] In addition to LÃ©vy, Khinchin and Kolomogrov, early
fundamental contributions to the theory of LÃ©vy processes were made by Bruno
de_Finetti and Kiyosi_ItÃ´.[224]
***** Mathematical construction[edit] *****
In mathematics, constructions of mathematical objects are needed, which is also
the case for stochastic processes, to prove that they exist mathematically.[58]
There are two main approaches for constructing a stochastic process. One
approach involves considering a measurable space of functions, defining a
suitable measurable mapping from a probability space to this measurable space
of functions, and then deriving the corresponding finite-dimensional
distributions.[310]
Another approach involves defining a collection of random variables to have
specific finite-dimensional distributions, and then using Kolmogorov's
existence_theorem[j] to prove a corresponding stochastic process exists.[58]
[310] This theorem, which is an existence theorem for measures on infinite
product spaces,[314] says that if any finite-dimensional distributions satisfy
two conditions, known as consistency conditions, then there exists a stochastic
process with those finite-dimensional distributions.[58]
**** Construction issues[edit] ****
When constructing continuous-time stochastic processes certain mathematical
difficulties arise, due to the uncountable index sets, which do not occur with
discrete-time processes.[59][60] One problem is that is it possible to have
more than one stochastic process with the same finite-dimensional
distributions. For example, both the left-continuous modification and the
right-continuous modification of a Poisson process have the same finite-
dimensional distributions.[315] This means that the distribution of the
stochastic process does not, necessarily, specify uniquely the properties of
the sample functions of the stochastic process.[310][316]
Another problem is that functionals of continuous-time process that rely upon
an uncountable number of points of the index set may not be measurable, so the
probabilities of certain events may not be well-defined.[168] For example, the
supremum of a stochastic process or random field is not necessarily a well-
defined random variable.[31][60] For a continuous-time stochastic process     X
{\displaystyle X}  [X], other characteristics that depend on an uncountable
number of points of the index set     T   {\displaystyle T}  [T] include:[168]
    * a sample function of a stochastic process     X   {\displaystyle X}  [X]
      is a continuous_function of     t &#x2208; T   {\displaystyle t\in T}
      [t\in T];
    * a sample function of a stochastic process     X   {\displaystyle X}  [X]
      is a bounded_function of     t &#x2208; T   {\displaystyle t\in T}  [t\in
      T]; and
    * a sample function of a stochastic process     X   {\displaystyle X}  [X]
      is an increasing_function of     t &#x2208; T   {\displaystyle t\in T}
      [t\in T].
To overcome these two difficulties, different assumptions and approaches are
possible.[70]
**** Resolving construction issues[edit] ****
One approach for avoiding mathematical construction issues of stochastic
processes, proposed by Joseph_Doob, is to assume that the stochastic process is
separable.[317] Separability ensures that infinite-dimensional distributions
determine the properties of sample functions by requiring that sample functions
are essentially determined by their values on a dense countable set of points
in the index set.[318] Furthermore, if a stochastic process is separable, then
functionals of an uncountable number of points of the index set are measurable
and their probabilities can be studied.[168][318]
Another approach is possible, originally developed by Anatoliy_Skorokhod and
Andrei_Kolmogorov,[319] for a continuous-time stochastic process with any
metric space as its state space. For the construction of such a stochastic
process, it is assumed that the sample functions of the stochastic process
belong to some suitable function space, which is usually the Skorokhod space
consisting of all right-continuous functions with left limits. This approach is
now more used than the separability assumption,[70][264] but such a stochastic
process based on this approach will be automatically separable.[320]
Although less used, the separability assumption is considered more general
because every stochastic process has a separable version.[264] It is also used
when it is not possible to construct a stochastic process in a Skorokhod space.
[173] For example, separability is assumed when constructing and studying
random fields, where the collection of random variables is now indexed by sets
other than the real line such as     n   {\displaystyle n}  [n]-dimensional
Euclidean space.[31][321]
***** See also[edit] *****
    * List_of_stochastic_processes_topics
    * Covariance_function
    * Deterministic_system
    * Dynamics_of_Markovian_particles
    * Entropy_rate (for a stochastic process)
    * Ergodic_process
    * GenI_process
    * Gillespie_algorithm
    * Interacting_particle_system
    * Law_(stochastic_processes)
    * Markov_chain
    * Probabilistic_cellular_automaton
    * Random_field
    * Randomness
    * Stationary_process
    * Statistical_model
    * Stochastic_calculus
    * Stochastic_control
    * Stochastic_processes_and_boundary_value_problems
***** Notes[edit] *****
   1. ^ The term Brownian motion can refer to the physical process, also known
      as Brownian movement, and the stochastic process, a mathematical object,
      but to avoid ambiguity this article uses the terms Brownian motion
      process or Wiener process for the latter in a style similar to, for
      example, Gikhman and Skorokhod[20] or Rosenblatt.[21]
   2. ^ The term "separable" appears twice here with two different meanings,
      where the first meaning is from probability and the second from topology
      and analysis. For a stochastic process to be separable (in a
      probabilistic sense), its index set must be a separable space (in a
      topological or analytic sense), in addition to other conditions.[136]
   3. ^ The definition of separability for a continuous-time real-valued
      stochastic process can be stated in other ways.[172][173]
   4. ^ In the context of point processes, the term "state space" can mean the
      space on which the point process is defined such as the real line,[234]
      [235] which corresponds to the index set in stochastic process
      terminology.
   5. ^ Also known as James or Jacques Bernoulli.[246]
   6. ^ It has been remarked that a notable exception was the St Petersburg
      School in Russia, where mathematicians led by Chebyshev studied
      probability theory.[251]
   7. ^ The name Khinchin is also written in (or transliterated into) English
      as Khintchine.[64]
   8. ^ Doob, when citing Khinchin, uses the term 'chance variable', which used
      to be an alternative term for 'random variable'.[262]
   9. ^ Later translated into English and published in 1950 as Foundations of
      the Theory of Probability[250]
  10. ^ The theorem has other names including Kolmogorov's consistency theorem,
      [311] Kolmogorov's extension theorem[312] or the DaniellâKolmogorov
      theorem.[313]
***** References[edit] *****
   1. ^ a b c d e f g h iJoseph L. Doob (1990). Stochastipoic_processes. Wiley.
      p. 46, 47.
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
   3. ^ a b c dL. C. G. Rogers; David Williams (2000). Diffusions,_Markov
      Processes,_and_Martingales:_Volume_1,_Foundations. Cambridge University
      Press. p. 1. ISBN 978-1-107-71749-7.
   4. ^ a b cJ. Michael Steele (2012). Stochastic_Calculus_and_Financial
      Applications. Springer Science & Business Media. p. 29. ISBN 978-1-4684-
      9305-4.
   5. ^ a b c d eEmanuel Parzen (2015). Stochastic_Processes. Courier Dover
      Publications. p. 7, 8. ISBN 978-0-486-79688-8.
   6. ^ a b c d e f g h i j k lIosif Ilyich Gikhman; Anatoly Vladimirovich
      Skorokhod (1969). Introduction_to_the_Theory_of_Random_Processes. Courier
      Corporation. p. 1. ISBN 978-0-486-69387-3.
   7. ^ a b c d eGagniuc, Paul A. (2017). Markov Chains: From Theory to
      Implementation and Experimentation. NJ: John Wiley & Sons. pp. 1â235.
      ISBN 978-1-119-38755-8.
   8. ^Paul C. Bressloff (2014). Stochastic_Processes_in_Cell_Biology.
      Springer. ISBN 978-3-319-08488-6.
   9. ^N.G. Van Kampen (2011). Stochastic_Processes_in_Physics_and_Chemistry.
      Elsevier. ISBN 978-0-08-047536-3.
  10. ^Russell Lande; Steinar Engen; Bernt-Erik SÃ¦ther (2003). Stochastic
      Population_Dynamics_in_Ecology_and_Conservation. Oxford University Press.
      ISBN 978-0-19-852525-7.
  11. ^Carlo Laing; Gabriel J Lord (2010). Stochastic_Methods_in_Neuroscience.
      OUP Oxford. ISBN 978-0-19-923507-0.
  12. ^Wolfgang Paul; JÃ¶rg Baschnagel (2013). Stochastic_Processes:_From
      Physics_to_Finance. Springer Science & Business Media. ISBN 978-3-319-
      00327-6.
  13. ^Edward R. Dougherty (1999). Random_processes_for_image_and_signal
      processing. SPIE Optical Engineering Press. ISBN 978-0-8194-2513-3.
  14. ^Thomas M. Cover; Joy A. Thomas (2012). Elements_of_Information_Theory.
      John Wiley & Sons. p. 71. ISBN 978-1-118-58577-1.
  15. ^Michael Baron (2015). Probability_and_Statistics_for_Computer
      Scientists,_Second_Edition. CRC Press. p. 131. ISBN 978-1-4987-6060-7.
  16. ^Jonathan Katz; Yehuda Lindell (2007). Introduction_to_Modern
      Cryptography:_Principles_and_Protocols. CRC Press. p. 26. ISBN 978-1-
      58488-586-3.
  17. ^FranÃ§ois Baccelli; Bartlomiej Blaszczyszyn (2009). Stochastic_Geometry
      and_Wireless_Networks. Now Publishers Inc. ISBN 978-1-60198-264-3.
  18. ^J. Michael Steele (2001). Stochastic_Calculus_and_Financial
      Applications. Springer Science & Business Media. ISBN 978-0-387-95016-7.
  19. ^ a bMarek Musiela; Marek Rutkowski (2006). Martingale_Methods_in
      Financial_Modelling. Springer Science & Business Media. ISBN 978-3-540-
      26653-2.
  20. ^Steven E. Shreve (2004). Stochastic_Calculus_for_Finance_II:_Continuous-
      Time_Models. Springer Science & Business Media. ISBN 978-0-387-40101-0.
  21. ^Iosif Ilyich Gikhman; Anatoly Vladimirovich Skorokhod (1969).
      Introduction_to_the_Theory_of_Random_Processes. Courier Corporation.
      ISBN 978-0-486-69387-3.
  22. ^Murray Rosenblatt (1962). Random_Processes. Oxford University Press.
  23. ^ a b c d e f g h iJarrow, Robert; Protter, Philip (2004). "A short
      history of stochastic integration and mathematical finance: the early
      years, 1880â1970". A Festschrift for Herman Rubin. Institute of
      Mathematical Statistics Lecture Notes - Monograph Series. pp. 75â80.
      CiteSeerX 10.1.1.114.632. doi:10.1214/lnms/1196285381. ISBN 978-0-940600-
      61-4. ISSN 0749-2170.
  24. ^ a b c d e f g hStirzaker, David (2000). "Advice to Hedgehogs, or,
      Constants Can Vary". The Mathematical Gazette. 84 (500): 197â210. doi:
      10.2307/3621649. ISSN 0025-5572. JSTOR 3621649.
  25. ^Donald L. Snyder; Michael I. Miller (2012). Random_Point_Processes_in
      Time_and_Space. Springer Science & Business Media. p. 32. ISBN 978-1-
      4612-3166-0.
  26. ^ a b c dGuttorp, Peter; Thorarinsdottir, Thordis L. (2012). "What
      Happened to Discrete Chaos, the Quenouille Process, and the Sharp Markov
      Property? Some History of Stochastic Point Processes". International
      Statistical Review. 80 (2): 253â268. doi:10.1111/j.1751-
      5823.2012.00181.x. ISSN 0306-7734.
  27. ^Dmytro Gusak; Alexander Kukush; Alexey Kulik; Yuliya Mishura; Andrey
      Pilipenko (2010). Theory_of_Stochastic_Processes:_With_Applications_to
      Financial_Mathematics_and_Risk_Theory. Springer Science & Business Media.
      p. 21. ISBN 978-0-387-87862-1.
  28. ^Valeriy Skorokhod (2005). Basic_Principles_and_Applications_of
      Probability_Theory. Springer Science & Business Media. p. 42. ISBN 978-3-
      540-26312-8.
  29. ^ a b c d e fOlav Kallenberg (2002). Foundations_of_Modern_Probability.
      Springer Science & Business Media. pp. 24â25. ISBN 978-0-387-95313-7.
  30. ^ a b c d e f g h i j k l m n o pJohn Lamperti (1977). Stochastic
      processes:_a_survey_of_the_mathematical_theory. Springer-Verlag.
      pp. 1â2. ISBN 978-3-540-90275-1.
  31. ^ a b c dLoÃ¯c Chaumont; Marc Yor (2012). Exercises_in_Probability:_A
      Guided_Tour_from_Measure_Theory_to_Random_Processes,_Via_Conditioning.
      Cambridge University Press. p. 175. ISBN 978-1-107-60655-5.
  32. ^ a b c d e f g hRobert J. Adler; Jonathan E. Taylor (2009). Random
      Fields_and_Geometry. Springer Science & Business Media. pp. 7â8.
      ISBN 978-0-387-48116-6.
  33. ^Gregory F. Lawler; Vlada Limic (2010). Random_Walk:_A_Modern
      Introduction. Cambridge University Press. ISBN 978-1-139-48876-1.
  34. ^David Williams (1991). Probability_with_Martingales. Cambridge
      University Press. ISBN 978-0-521-40605-5.
  35. ^L. C. G. Rogers; David Williams (2000). Diffusions,_Markov_Processes,
      and_Martingales:_Volume_1,_Foundations. Cambridge University Press.
      ISBN 978-1-107-71749-7.
  36. ^David Applebaum (2004). LÃ©vy_Processes_and_Stochastic_Calculus.
      Cambridge University Press. ISBN 978-0-521-83263-2.
  37. ^Mikhail Lifshits (2012). Lectures_on_Gaussian_Processes. Springer
      Science & Business Media. ISBN 978-3-642-24939-6.
  38. ^Robert J. Adler (2010). The_Geometry_of_Random_Fields. SIAM. ISBN 978-0-
      89871-693-1.
  39. ^Samuel Karlin; Howard E. Taylor (2012). A_First_Course_in_Stochastic
      Processes. Academic Press. ISBN 978-0-08-057041-9.
  40. ^Bruce Hajek (2015). Random_Processes_for_Engineers. Cambridge University
      Press. ISBN 978-1-316-24124-0.
  41. ^ a bG. Latouche; V. Ramaswami (1999). Introduction_to_Matrix_Analytic
      Methods_in_Stochastic_Modeling. SIAM. ISBN 978-0-89871-425-8.
  42. ^D.J. Daley; David Vere-Jones (2007). An_Introduction_to_the_Theory_of
      Point_Processes:_Volume_II:_General_Theory_and_Structure. Springer
      Science & Business Media. ISBN 978-0-387-21337-8.
  43. ^Patrick Billingsley (2008). Probability_and_Measure. Wiley India Pvt.
      Limited. ISBN 978-81-265-1771-8.
  44. ^Pierre BrÃ©maud (2014). Fourier_Analysis_and_Stochastic_Processes.
      Springer. ISBN 978-3-319-09590-5.
  45. ^Adam Bobrowski (2005). Functional_Analysis_for_Probability_and
      Stochastic_Processes:_An_Introduction. Cambridge University Press.
      ISBN 978-0-521-83166-6.
  46. ^Applebaum, David (2004). "LÃ©vy processes: From probability to finance
      and quantum groups". Notices of the AMS. 51 (11): 1336â1347.
  47. ^ a bJochen Blath; Peter Imkeller; Sylvie RÅlly (2011). Surveys_in
      Stochastic_Processes. European Mathematical Society. ISBN 978-3-03719-
      072-2.
  48. ^Michel Talagrand (2014). Upper_and_Lower_Bounds_for_Stochastic
      Processes:_Modern_Methods_and_Classical_Problems. Springer Science &
      Business Media. pp. 4â. ISBN 978-3-642-54075-2.
  49. ^Paul C. Bressloff (2014). Stochastic_Processes_in_Cell_Biology.
      Springer. pp. viiâix. ISBN 978-3-319-08488-6.
  50. ^ a b c dSamuel Karlin; Howard E. Taylor (2012). A_First_Course_in
      Stochastic_Processes. Academic Press. p. 27. ISBN 978-0-08-057041-9.
  51. ^ a b c d e f g h i jApplebaum, David (2004). "LÃ©vy processes: From
      probability to finance and quantum groups". Notices of the AMS. 51 (11):
      1337.
  52. ^ a bL. C. G. Rogers; David Williams (2000). Diffusions,_Markov
      Processes,_and_Martingales:_Volume_1,_Foundations. Cambridge University
      Press. pp. 121â124. ISBN 978-1-107-71749-7.
  53. ^ a b c d e fIonut Florescu (2014). Probability_and_Stochastic_Processes.
      John Wiley & Sons. pp. 294, 295. ISBN 978-1-118-59320-2.
  54. ^ a bSamuel Karlin; Howard E. Taylor (2012). A_First_Course_in_Stochastic
      Processes. Academic Press. p. 26. ISBN 978-0-08-057041-9.
  55. ^Donald L. Snyder; Michael I. Miller (2012). Random_Point_Processes_in
      Time_and_Space. Springer Science & Business Media. p. 24, 25. ISBN 978-1-
      4612-3166-0.
  56. ^ a bPatrick Billingsley (2008). Probability_and_Measure. Wiley India
      Pvt. Limited. p. 482. ISBN 978-81-265-1771-8.
  57. ^ a bAlexander A. Borovkov (2013). Probability_Theory. Springer Science &
      Business Media. p. 527. ISBN 978-1-4471-5201-9.
  58. ^ a b cPierre BrÃ©maud (2014). Fourier_Analysis_and_Stochastic_Processes.
      Springer. p. 120. ISBN 978-3-319-09590-5.
  59. ^ a b c d eJeffrey S Rosenthal (2006). A_First_Look_at_Rigorous
      Probability_Theory. World Scientific Publishing Co Inc. pp. 177â178.
      ISBN 978-981-310-165-4.
  60. ^ a bPeter E. Kloeden; Eckhard Platen (2013). Numerical_Solution_of
      Stochastic_Differential_Equations. Springer Science & Business Media.
      p. 63. ISBN 978-3-662-12616-5.
  61. ^ a b cDavar Khoshnevisan (2006). Multiparameter_Processes:_An
      Introduction_to_Random_Fields. Springer Science & Business Media.
      pp. 153â155. ISBN 978-0-387-21631-7.
  62. ^ a b"Stochastic". Oxford_English_Dictionary (3rd ed.). Oxford University
      Press. September 2005.
  63.  (Subscription or UK_public_library_membership required.)
  64. ^O. B. SheÄ­nin (2006). Theory_of_probability_and_statistics_as
      exemplified_in_short_dictums. NG Verlag. p. 5. ISBN 978-3-938417-40-9.
  65. ^Oscar Sheynin; Heinrich Strecker (2011). Alexandr_A._Chuprov:_Life,
      Work,_Correspondence. V&R unipress GmbH. p. 136. ISBN 978-3-89971-812-6.
  66. ^ a b c dDoob, Joseph (1934). "Stochastic_Processes_and_Statistics".
      Proceedings of the National Academy of Sciences of the United States of
      America. 20 (6): 376â379. Bibcode:1934PNAS...20..376D. doi:10.1073/
      pnas.20.6.376. PMC 1076423. PMID 16587907.
  67. ^Khintchine, A. (1934). "Korrelationstheorie der stationeren
      stochastischen Prozesse". Mathematische Annalen. 109 (1): 604â615. doi:
      10.1007/BF01449156. ISSN 0025-5831.
  68. ^Kolmogoroff, A. (1931). "Ãber die analytischen Methoden in der
      Wahrscheinlichkeitsrechnung". Mathematische Annalen. 104 (1): 1. doi:
      10.1007/BF01457949. ISSN 0025-5831.
  69. ^"Random". Oxford_English_Dictionary (3rd ed.). Oxford University Press.
      September 2005.
  70.  (Subscription or UK_public_library_membership required.)
  71. ^Bert E. Fristedt; Lawrence F. Gray (2013). A_Modern_Approach_to
      Probability_Theory. Springer Science & Business Media. p. 580. ISBN 978-
      1-4899-2837-5.
  72. ^ a b c dL. C. G. Rogers; David Williams (2000). Diffusions,_Markov
      Processes,_and_Martingales:_Volume_1,_Foundations. Cambridge University
      Press. pp. 121, 122. ISBN 978-1-107-71749-7.
  73. ^ a b c d eSÃ¸ren Asmussen (2003). Applied_Probability_and_Queues.
      Springer Science & Business Media. p. 408. ISBN 978-0-387-00211-8.
  74. ^ a bDavid Stirzaker (2005). Stochastic_Processes_and_Models. Oxford
      University Press. p. 45. ISBN 978-0-19-856814-8.
  75. ^Murray Rosenblatt (1962). Random_Processes. Oxford University Press.
      p. 91.
  76. ^John A. Gubner (2006). Probability_and_Random_Processes_for_Electrical
      and_Computer_Engineers. Cambridge University Press. p. 383. ISBN 978-1-
      139-45717-0.
  77. ^ a bKiyosi ItÅ (2006). Essentials_of_Stochastic_Processes. American
      Mathematical Soc. p. 13. ISBN 978-0-8218-3898-3.
  78. ^M. LoÃ¨ve (1978). Probability_Theory_II. Springer Science & Business
      Media. p. 163. ISBN 978-0-387-90262-3.
  79. ^Pierre BrÃ©maud (2014). Fourier_Analysis_and_Stochastic_Processes.
      Springer. p. 133. ISBN 978-3-319-09590-5.
  80. ^ a bDmytro Gusak; Alexander Kukush; Alexey Kulik; Yuliya Mishura; Andrey
      Pilipenko (2010). Theory_of_Stochastic_Processes:_With_Applications_to
      Financial_Mathematics_and_Risk_Theory. Springer Science & Business Media.
      p. 1. ISBN 978-0-387-87862-1.
  81. ^Richard F. Bass (2011). Stochastic_Processes. Cambridge University
      Press. p. 1. ISBN 978-1-139-50147-7.
  82. ^ a b ,John Lamperti (1977). Stochastic_processes:_a_survey_of_the
      mathematical_theory. Springer-Verlag. p. 3. ISBN 978-3-540-90275-1.
  83. ^Fima C. Klebaner (2005). Introduction_to_Stochastic_Calculus_with
      Applications. Imperial College Press. p. 55. ISBN 978-1-86094-555-7.
  84. ^ a bIonut Florescu (2014). Probability_and_Stochastic_Processes. John
      Wiley & Sons. p. 293. ISBN 978-1-118-59320-2.
  85. ^ a bIonut Florescu (2014). Probability_and_Stochastic_Processes. John
      Wiley & Sons. p. 301. ISBN 978-1-118-59320-2.
  86. ^ a bDimitri P. Bertsekas; John N. Tsitsiklis (2002). Introduction_to
      Probability. Athena Scientific. p. 273. ISBN 978-1-886529-40-3.
  87. ^Oliver C. Ibe (2013). Elements_of_Random_Walk_and_Diffusion_Processes.
      John Wiley & Sons. p. 11. ISBN 978-1-118-61793-9.
  88. ^Achim Klenke (2013). Probability_Theory:_A_Comprehensive_Course.
      Springer. p. 347. ISBN 978-1-4471-5362-7.
  89. ^Gregory F. Lawler; Vlada Limic (2010). Random_Walk:_A_Modern
      Introduction. Cambridge University Press. p. 1. ISBN 978-1-139-48876-1.
  90. ^Olav Kallenberg (2002). Foundations_of_Modern_Probability. Springer
      Science & Business Media. p. 136. ISBN 978-0-387-95313-7.
  91. ^Ionut Florescu (2014). Probability_and_Stochastic_Processes. John Wiley
      & Sons. p. 383. ISBN 978-1-118-59320-2.
  92. ^Rick Durrett (2010). Probability:_Theory_and_Examples. Cambridge
      University Press. p. 277. ISBN 978-1-139-49113-6.
  93. ^ a b cWeiss, George H. (2006). "Random Walks". Encyclopedia of
      Statistical Sciences. p. 1. doi:10.1002/0471667196.ess2180.pub2.
      ISBN 978-0471667193.
  94. ^Aris Spanos (1999). Probability_Theory_and_Statistical_Inference:
      Econometric_Modeling_with_Observational_Data. Cambridge University Press.
      p. 454. ISBN 978-0-521-42408-0.
  95. ^ a bFima C. Klebaner (2005). Introduction_to_Stochastic_Calculus_with
      Applications. Imperial College Press. p. 81. ISBN 978-1-86094-555-7.
  96. ^Allan Gut (2012). Probability:_A_Graduate_Course. Springer Science &
      Business Media. p. 88. ISBN 978-1-4614-4708-5.
  97. ^Geoffrey Grimmett; David Stirzaker (2001). Probability_and_Random
      Processes. OUP Oxford. p. 71. ISBN 978-0-19-857222-0.
  98. ^Fima C. Klebaner (2005). Introduction_to_Stochastic_Calculus_with
      Applications. Imperial College Press. p. 56. ISBN 978-1-86094-555-7.
  99. ^Brush, Stephen G. (1968). "A history of random processes". Archive for
      History of Exact Sciences. 5 (1): 1â2. doi:10.1007/BF00328110.
      ISSN 0003-9519.
 100. ^ a bApplebaum, David (2004). "LÃ©vy processes: From probability to
      finance and quantum groups". Notices of the AMS. 51 (11): 1338.
 101. ^Iosif Ilyich Gikhman; Anatoly Vladimirovich Skorokhod (1969).
      Introduction_to_the_Theory_of_Random_Processes. Courier Corporation.
      p. 21. ISBN 978-0-486-69387-3.
 102. ^Ionut Florescu (2014). Probability_and_Stochastic_Processes. John Wiley
      & Sons. p. 471. ISBN 978-1-118-59320-2.
 103. ^ a bSamuel Karlin; Howard E. Taylor (2012). A_First_Course_in_Stochastic
      Processes. Academic Press. pp. 21, 22. ISBN 978-0-08-057041-9.
 104. ^Ioannis Karatzas; Steven Shreve (1991). Brownian_Motion_and_Stochastic
      Calculus. Springer. p. VIII. ISBN 978-1-4612-0949-2.
 105. ^Daniel_Revuz; Marc Yor (2013). Continuous_Martingales_and_Brownian
      Motion. Springer Science & Business Media. p. IX. ISBN 978-3-662-06400-9.
 106. ^Jeffrey S Rosenthal (2006). A_First_Look_at_Rigorous_Probability_Theory.
      World Scientific Publishing Co Inc. p. 186. ISBN 978-981-310-165-4.
 107. ^Donald L. Snyder; Michael I. Miller (2012). Random_Point_Processes_in
      Time_and_Space. Springer Science & Business Media. p. 33. ISBN 978-1-
      4612-3166-0.
 108. ^J. Michael Steele (2012). Stochastic_Calculus_and_Financial
      Applications. Springer Science & Business Media. p. 118. ISBN 978-1-4684-
      9305-4.
 109. ^ a bPeter MÃ¶rters; Yuval Peres (2010). Brownian_Motion. Cambridge
      University Press. pp. 1, 3. ISBN 978-1-139-48657-6.
 110. ^Ioannis Karatzas; Steven Shreve (1991). Brownian_Motion_and_Stochastic
      Calculus. Springer. p. 78. ISBN 978-1-4612-0949-2.
 111. ^Ioannis Karatzas; Steven Shreve (1991). Brownian_Motion_and_Stochastic
      Calculus. Springer. p. 61. ISBN 978-1-4612-0949-2.
 112. ^Steven E. Shreve (2004). Stochastic_Calculus_for_Finance_II:_Continuous-
      Time_Models. Springer Science & Business Media. p. 93. ISBN 978-0-387-
      40101-0.
 113. ^Olav Kallenberg (2002). Foundations_of_Modern_Probability. Springer
      Science & Business Media. pp. 225, 260. ISBN 978-0-387-95313-7.
 114. ^Ioannis Karatzas; Steven Shreve (1991). Brownian_Motion_and_Stochastic
      Calculus. Springer. p. 70. ISBN 978-1-4612-0949-2.
 115. ^Peter MÃ¶rters; Yuval Peres (2010). Brownian_Motion. Cambridge
      University Press. p. 131. ISBN 978-1-139-48657-6.
 116. ^Fima C. Klebaner (2005). Introduction_to_Stochastic_Calculus_with
      Applications. Imperial College Press. ISBN 978-1-86094-555-7.
 117. ^Ioannis Karatzas; Steven Shreve (1991). Brownian_Motion_and_Stochastic
      Calculus. Springer. ISBN 978-1-4612-0949-2.
 118. ^Applebaum, David (2004). "LÃ©vy processes: From probability to finance
      and quantum groups". Notices of the AMS. 51 (11): 1341.
 119. ^Samuel Karlin; Howard E. Taylor (2012). A_First_Course_in_Stochastic
      Processes. Academic Press. p. 340. ISBN 978-0-08-057041-9.
 120. ^Fima C. Klebaner (2005). Introduction_to_Stochastic_Calculus_with
      Applications. Imperial College Press. p. 124. ISBN 978-1-86094-555-7.
 121. ^Ioannis Karatzas; Steven Shreve (1991). Brownian_Motion_and_Stochastic
      Calculus. Springer. p. 47. ISBN 978-1-4612-0949-2.
 122. ^Ubbo F. Wiersema (2008). Brownian_Motion_Calculus. John Wiley & Sons.
      p. 2. ISBN 978-0-470-02171-2.
 123. ^ a b cHenk C. Tijms (2003). A_First_Course_in_Stochastic_Models. Wiley.
      pp. 1, 2. ISBN 978-0-471-49881-0.
 124. ^D.J. Daley; D. Vere-Jones (2006). An_Introduction_to_the_Theory_of_Point
      Processes:_Volume_I:_Elementary_Theory_and_Methods. Springer Science &
      Business Media. pp. 19â36. ISBN 978-0-387-21564-8.
 125. ^Mark A. Pinsky; Samuel Karlin (2011). An_Introduction_to_Stochastic
      Modeling. Academic Press. p. 241. ISBN 978-0-12-381416-6.
 126. ^J. F. C. Kingman (1992). Poisson_Processes. Clarendon Press. p. 38.
      ISBN 978-0-19-159124-2.
 127. ^D.J. Daley; D. Vere-Jones (2006). An_Introduction_to_the_Theory_of_Point
      Processes:_Volume_I:_Elementary_Theory_and_Methods. Springer Science &
      Business Media. p. 19. ISBN 978-0-387-21564-8.
 128. ^J. F. C. Kingman (1992). Poisson_Processes. Clarendon Press. p. 22.
      ISBN 978-0-19-159124-2.
 129. ^Samuel Karlin; Howard E. Taylor (2012). A_First_Course_in_Stochastic
      Processes. Academic Press. pp. 118, 119. ISBN 978-0-08-057041-9.
 130. ^Leonard Kleinrock (1976). Queueing_Systems:_Theory. Wiley. p. 61.
      ISBN 978-0-471-49110-1.
 131. ^Murray Rosenblatt (1962). Random_Processes. Oxford University Press.
      p. 94.
 132. ^ a bMartin Haenggi (2013). Stochastic_Geometry_for_Wireless_Networks.
      Cambridge University Press. pp. 10, 18. ISBN 978-1-107-01469-5.
 133. ^ a bSung Nok Chiu; Dietrich Stoyan; Wilfrid S. Kendall; Joseph Mecke
      (2013). Stochastic_Geometry_and_Its_Applications. John Wiley & Sons.
      pp. 41, 108. ISBN 978-1-118-65825-3.
 134. ^J. F. C. Kingman (1992). Poisson_Processes. Clarendon Press. p. 11.
      ISBN 978-0-19-159124-2.
 135. ^ a bRoy L. Streit (2010). Poisson_Point_Processes:_Imaging,_Tracking,
      and_Sensing. Springer Science & Business Media. p. 1. ISBN 978-1-4419-
      6923-1.
 136. ^J. F. C. Kingman (1992). Poisson_Processes. Clarendon Press. p. v.
      ISBN 978-0-19-159124-2.
 137. ^ a bAlexander_A._Borovkov (2013). Probability_Theory. Springer Science &
      Business Media. p. 528. ISBN 978-1-4471-5201-9.
 138. ^Georg Lindgren; Holger Rootzen; Maria Sandsten (2013). Stationary
      Stochastic_Processes_for_Scientists_and_Engineers. CRC Press. p. 11.
      ISBN 978-1-4665-8618-5.
 139. ^ a b cValeriy Skorokhod (2005). Basic_Principles_and_Applications_of
      Probability_Theory. Springer Science & Business Media. pp. 93, 94.
      ISBN 978-3-540-26312-8.
 140. ^Donald L. Snyder; Michael I. Miller (2012). Random_Point_Processes_in
      Time_and_Space. Springer Science & Business Media. p. 25. ISBN 978-1-
      4612-3166-0.
 141. ^Valeriy Skorokhod (2005). Basic_Principles_and_Applications_of
      Probability_Theory. Springer Science & Business Media. p. 104. ISBN 978-
      3-540-26312-8.
 142. ^Ionut Florescu (2014). Probability_and_Stochastic_Processes. John Wiley
      & Sons. p. 296. ISBN 978-1-118-59320-2.
 143. ^Patrick Billingsley (2008). Probability_and_Measure. Wiley India Pvt.
      Limited. p. 493. ISBN 978-81-265-1771-8.
 144. ^Bernt Ãksendal (2003). Stochastic_Differential_Equations:_An
      Introduction_with_Applications. Springer Science & Business Media. p. 10.
      ISBN 978-3-540-04758-2.
 145. ^ a b c d ePeter K. Friz; Nicolas B. Victoir (010). Multidimensional
      Stochastic_Processes_as_Rough_Paths:_Theory_and_Applications. Cambridge
      University Press. p. 571. ISBN 978-1-139-48721-4.
 146. ^Sidney I. Resnick (2013). Adventures_in_Stochastic_Processes. Springer
      Science & Business Media. pp. 40â41. ISBN 978-1-4612-0387-2.
 147. ^Ward Whitt (2006). Stochastic-Process_Limits:_An_Introduction_to
      Stochastic-Process_Limits_and_Their_Application_to_Queues. Springer
      Science & Business Media. p. 23. ISBN 978-0-387-21748-2.
 148. ^David Applebaum (2004). LÃ©vy_Processes_and_Stochastic_Calculus.
      Cambridge University Press. p. 4. ISBN 978-0-521-83263-2.
 149. ^Daniel Revuz; Marc Yor (2013). Continuous_Martingales_and_Brownian
      Motion. Springer Science & Business Media. p. 10. ISBN 978-3-662-06400-9.
 150. ^L. C. G. Rogers; David Williams (2000). Diffusions,_Markov_Processes,
      and_Martingales:_Volume_1,_Foundations. Cambridge University Press.
      p. 123. ISBN 978-1-107-71749-7.
 151. ^ a b c dJohn Lamperti (1977). Stochastic_processes:_a_survey_of_the
      mathematical_theory. Springer-Verlag. pp. 6 and 7. ISBN 978-3-540-90275-
      1.
 152. ^Iosif I. Gikhman; Anatoly Vladimirovich Skorokhod (1969). Introduction
      to_the_Theory_of_Random_Processes. Courier Corporation. p. 4. ISBN 978-0-
      486-69387-3.
 153. ^ a b c dRobert J. Adler (2010). The_Geometry_of_Random_Fields. SIAM.
      p. 14, 15. ISBN 978-0-89871-693-1.
 154. ^Sung Nok Chiu; Dietrich Stoyan; Wilfrid S. Kendall; Joseph Mecke (2013).
      Stochastic_Geometry_and_Its_Applications. John Wiley & Sons. p. 112.
      ISBN 978-1-118-65825-3.
 155. ^ a bJoseph L. Doob (1990). Stochastic_processes. Wiley. pp. 94â96.
 156. ^ a bIonut Florescu (2014). Probability_and_Stochastic_Processes. John
      Wiley & Sons. pp. 298, 299. ISBN 978-1-118-59320-2.
 157. ^Iosif Ilyich Gikhman; Anatoly Vladimirovich Skorokhod (1969).
      Introduction_to_the_Theory_of_Random_Processes. Courier Corporation.
      p. 8. ISBN 978-0-486-69387-3.
 158. ^ a b cDavid Williams (1991). Probability_with_Martingales. Cambridge
      University Press. pp. 93, 94. ISBN 978-0-521-40605-5.
 159. ^Fima C. Klebaner (2005). Introduction_to_Stochastic_Calculus_with
      Applications. Imperial College Press. pp. 22â23. ISBN 978-1-86094-555-
      7.
 160. ^Peter MÃ¶rters; Yuval Peres (2010). Brownian_Motion. Cambridge
      University Press. p. 37. ISBN 978-1-139-48657-6.
 161. ^ a bL. C. G. Rogers; David Williams (2000). Diffusions,_Markov
      Processes,_and_Martingales:_Volume_1,_Foundations. Cambridge University
      Press. p. 130. ISBN 978-1-107-71749-7.
 162. ^Alexander A. Borovkov (2013). Probability_Theory. Springer Science &
      Business Media. p. 530. ISBN 978-1-4471-5201-9.
 163. ^Fima C. Klebaner (2005). Introduction_to_Stochastic_Calculus_with
      Applications. Imperial College Press. p. 48. ISBN 978-1-86094-555-7.
 164. ^ a bBernt Ãksendal (2003). Stochastic_Differential_Equations:_An
      Introduction_with_Applications. Springer Science & Business Media. p. 14.
      ISBN 978-3-540-04758-2.
 165. ^ a bIonut Florescu (2014). Probability_and_Stochastic_Processes. John
      Wiley & Sons. p. 472. ISBN 978-1-118-59320-2.
 166. ^Daniel Revuz; Marc Yor (2013). Continuous_Martingales_and_Brownian
      Motion. Springer Science & Business Media. pp. 18â19. ISBN 978-3-662-
      06400-9.
 167. ^David Applebaum (2004). LÃ©vy_Processes_and_Stochastic_Calculus.
      Cambridge University Press. p. 20. ISBN 978-0-521-83263-2.
 168. ^Hiroshi Kunita (1997). Stochastic_Flows_and_Stochastic_Differential
      Equations. Cambridge University Press. p. 31. ISBN 978-0-521-59925-2.
 169. ^Olav Kallenberg (2002). Foundations_of_Modern_Probability. Springer
      Science & Business Media. p. 35. ISBN 978-0-387-95313-7.
 170. ^Monique Jeanblanc; Marc Yor; Marc Chesney (2009). Mathematical_Methods
      for_Financial_Markets. Springer Science & Business Media. p. 11.
      ISBN 978-1-85233-376-8.
 171. ^ a b c d e fKiyosi ItÅ (2006). Essentials_of_Stochastic_Processes.
      American Mathematical Soc. pp. 32â33. ISBN 978-0-8218-3898-3.
 172. ^Iosif Ilyich Gikhman; Anatoly Vladimirovich Skorokhod (1969).
      Introduction_to_the_Theory_of_Random_Processes. Courier Corporation.
      p. 150. ISBN 978-0-486-69387-3.
 173. ^ a bPetar Todorovic (2012). An_Introduction_to_Stochastic_Processes_and
      Their_Applications. Springer Science & Business Media. pp. 19â20.
      ISBN 978-1-4613-9742-7.
 174. ^Ilya Molchanov (2005). Theory_of_Random_Sets. Springer Science &
      Business Media. p. 340. ISBN 978-1-85233-892-3.
 175. ^ a bPatrick Billingsley (2008). Probability_and_Measure. Wiley India
      Pvt. Limited. pp. 526â527. ISBN 978-81-265-1771-8.
 176. ^ a bAlexander A. Borovkov (2013). Probability_Theory. Springer Science &
      Business Media. p. 535. ISBN 978-1-4471-5201-9.
 177. ^Dmytro Gusak; Alexander Kukush; Alexey Kulik; Yuliya Mishura; Andrey
      Pilipenko (2010). Theory_of_Stochastic_Processes:_With_Applications_to
      Financial_Mathematics_and_Risk_Theory. Springer Science & Business Media.
      p. 22. ISBN 978-0-387-87862-1.
 178. ^Joseph L. Doob (1990). Stochastic_processes. Wiley. p. 56.
 179. ^Davar Khoshnevisan (2006). Multiparameter_Processes:_An_Introduction_to
      Random_Fields. Springer Science & Business Media. p. 155. ISBN 978-0-387-
      21631-7.
 180. ^ Lapidoth, Amos, A Foundation in Digital Communication, Cambridge
      University Press, 2009.
 181. ^ a b c Kun Il Park, Fundamentals of Probability and Stochastic Processes
      with Applications to Communications, Springer, 2018, 978-3-319-68074-3
 182. ^ a b c dWard Whitt (2006). Stochastic-Process_Limits:_An_Introduction_to
      Stochastic-Process_Limits_and_Their_Application_to_Queues. Springer
      Science & Business Media. pp. 78â79. ISBN 978-0-387-21748-2.
 183. ^ a bDmytro Gusak; Alexander Kukush; Alexey Kulik; Yuliya Mishura; Andrey
      Pilipenko (2010). Theory_of_Stochastic_Processes:_With_Applications_to
      Financial_Mathematics_and_Risk_Theory. Springer Science & Business Media.
      p. 24. ISBN 978-0-387-87862-1.
 184. ^ a b c dVladimir I. Bogachev (2007). Measure_Theory_(Volume_2). Springer
      Science & Business Media. p. 53. ISBN 978-3-540-34514-5.
 185. ^ a b cFima C. Klebaner (2005). Introduction_to_Stochastic_Calculus_with
      Applications. Imperial College Press. p. 4. ISBN 978-1-86094-555-7.
 186. ^ a bSÃ¸ren Asmussen (2003). Applied_Probability_and_Queues. Springer
      Science & Business Media. p. 420. ISBN 978-0-387-00211-8.
 187. ^ a b cPatrick Billingsley (2013). Convergence_of_Probability_Measures.
      John Wiley & Sons. p. 121. ISBN 978-1-118-62596-5.
 188. ^Richard F. Bass (2011). Stochastic_Processes. Cambridge University
      Press. p. 34. ISBN 978-1-139-50147-7.
 189. ^Nicholas H. Bingham; RÃ¼diger Kiesel (2013). Risk-Neutral_Valuation:
      Pricing_and_Hedging_of_Financial_Derivatives. Springer Science & Business
      Media. p. 154. ISBN 978-1-4471-3856-3.
 190. ^Alexander A. Borovkov (2013). Probability_Theory. Springer Science &
      Business Media. p. 532. ISBN 978-1-4471-5201-9.
 191. ^Davar Khoshnevisan (2006). Multiparameter_Processes:_An_Introduction_to
      Random_Fields. Springer Science & Business Media. pp. 148â165.
      ISBN 978-0-387-21631-7.
 192. ^Petar Todorovic (2012). An_Introduction_to_Stochastic_Processes_and
      Their_Applications. Springer Science & Business Media. p. 22. ISBN 978-1-
      4613-9742-7.
 193. ^Ward Whitt (2006). Stochastic-Process_Limits:_An_Introduction_to
      Stochastic-Process_Limits_and_Their_Application_to_Queues. Springer
      Science & Business Media. p. 79. ISBN 978-0-387-21748-2.
 194. ^Richard Serfozo (2009). Basics_of_Applied_Stochastic_Processes. Springer
      Science & Business Media. p. 2. ISBN 978-3-540-89332-5.
 195. ^Y.A. Rozanov (2012). Markov_Random_Fields. Springer Science & Business
      Media. p. 58. ISBN 978-1-4613-8190-7.
 196. ^Sheldon M. Ross (1996). Stochastic_processes. Wiley. pp. 235, 358.
      ISBN 978-0-471-12062-9.
 197. ^Ionut Florescu (2014). Probability_and_Stochastic_Processes. John Wiley
      & Sons. pp. 373, 374. ISBN 978-1-118-59320-2.
 198. ^ a bSamuel Karlin; Howard E. Taylor (2012). A_First_Course_in_Stochastic
      Processes. Academic Press. p. 49. ISBN 978-0-08-057041-9.
 199. ^ a bSÃ¸ren Asmussen (2003). Applied_Probability_and_Queues. Springer
      Science & Business Media. p. 7. ISBN 978-0-387-00211-8.
 200. ^Emanuel Parzen (2015). Stochastic_Processes. Courier Dover Publications.
      p. 188. ISBN 978-0-486-79688-8.
 201. ^Samuel Karlin; Howard E. Taylor (2012). A_First_Course_in_Stochastic
      Processes. Academic Press. pp. 29, 30. ISBN 978-0-08-057041-9.
 202. ^John Lamperti (1977). Stochastic_processes:_a_survey_of_the_mathematical
      theory. Springer-Verlag. pp. 106â121. ISBN 978-3-540-90275-1.
 203. ^Sheldon M. Ross (1996). Stochastic_processes. Wiley. pp. 174, 231.
      ISBN 978-0-471-12062-9.
 204. ^Sean Meyn; Richard L. Tweedie (2009). Markov_Chains_and_Stochastic
      Stability. Cambridge University Press. p. 19. ISBN 978-0-521-73182-9.
 205. ^Samuel Karlin; Howard E. Taylor (2012). A_First_Course_in_Stochastic
      Processes. Academic Press. p. 47. ISBN 978-0-08-057041-9.
 206. ^Reuven Y. Rubinstein; Dirk P. Kroese (2011). Simulation_and_the_Monte
      Carlo_Method. John Wiley & Sons. p. 225. ISBN 978-1-118-21052-9.
 207. ^Dani Gamerman; Hedibert F. Lopes (2006). Markov_Chain_Monte_Carlo:
      Stochastic_Simulation_for_Bayesian_Inference,_Second_Edition. CRC Press.
      ISBN 978-1-58488-587-0.
 208. ^Y.A. Rozanov (2012). Markov_Random_Fields. Springer Science & Business
      Media. p. 61. ISBN 978-1-4613-8190-7.
 209. ^Donald L. Snyder; Michael I. Miller (2012). Random_Point_Processes_in
      Time_and_Space. Springer Science & Business Media. p. 27. ISBN 978-1-
      4612-3166-0.
 210. ^Pierre Bremaud (2013). Markov_Chains:_Gibbs_Fields,_Monte_Carlo
      Simulation,_and_Queues. Springer Science & Business Media. p. 253.
      ISBN 978-1-4757-3124-8.
 211. ^ a b cFima C. Klebaner (2005). Introduction_to_Stochastic_Calculus_with
      Applications. Imperial College Press. p. 65. ISBN 978-1-86094-555-7.
 212. ^ a b cIoannis Karatzas; Steven Shreve (1991). Brownian_Motion_and
      Stochastic_Calculus. Springer. p. 11. ISBN 978-1-4612-0949-2.
 213. ^Joseph L. Doob (1990). Stochastic_processes. Wiley. pp. 292, 293.
 214. ^Gilles Pisier (2016). Martingales_in_Banach_Spaces. Cambridge University
      Press. ISBN 978-1-316-67946-3.
 215. ^ a bJ. Michael Steele (2012). Stochastic_Calculus_and_Financial
      Applications. Springer Science & Business Media. p. 12, 13. ISBN 978-1-
      4684-9305-4.
 216. ^ a bP. Hall; C. C. Heyde (2014). Martingale_Limit_Theory_and_Its
      Application. Elsevier Science. p. 2. ISBN 978-1-4832-6322-9.
 217. ^J. Michael Steele (2012). Stochastic_Calculus_and_Financial
      Applications. Springer Science & Business Media. p. 115. ISBN 978-1-4684-
      9305-4.
 218. ^Sheldon M. Ross (1996). Stochastic_processes. Wiley. p. 295. ISBN 978-0-
      471-12062-9.
 219. ^ a bJ. Michael Steele (2012). Stochastic_Calculus_and_Financial
      Applications. Springer Science & Business Media. p. 11. ISBN 978-1-4684-
      9305-4.
 220. ^Olav Kallenberg (2002). Foundations_of_Modern_Probability. Springer
      Science & Business Media. p. 96. ISBN 978-0-387-95313-7.
 221. ^J. Michael Steele (2012). Stochastic_Calculus_and_Financial
      Applications. Springer Science & Business Media. p. 371. ISBN 978-1-4684-
      9305-4.
 222. ^J. Michael Steele (2012). Stochastic_Calculus_and_Financial
      Applications. Springer Science & Business Media. p. 22. ISBN 978-1-4684-
      9305-4.
 223. ^Geoffrey Grimmett; David Stirzaker (2001). Probability_and_Random
      Processes. OUP Oxford. p. 336. ISBN 978-0-19-857222-0.
 224. ^Glasserman, Paul; Kou, Steven (2006). "A Conversation with Chris Heyde".
      Statistical Science. 21 (2): 292, 293. arXiv:math/0609294. doi:10.1214/
      088342306000000088. ISSN 0883-4237.
 225. ^Francois Baccelli; Pierre Bremaud (2013). Elements_of_Queueing_Theory:
      Palm_Martingale_Calculus_and_Stochastic_Recurrences. Springer Science &
      Business Media. ISBN 978-3-662-11657-9.
 226. ^P. Hall; C. C. Heyde (2014). Martingale_Limit_Theory_and_Its
      Application. Elsevier Science. p. x. ISBN 978-1-4832-6322-9.
 227. ^ a b c dJean Bertoin (1998). LÃ©vy_Processes. Cambridge University
      Press. p. viii. ISBN 978-0-521-64632-1.
 228. ^ a b cApplebaum, David (2004). "LÃ©vy processes: From probability to
      finance and quantum groups". Notices of the AMS. 51 (11): 1336.
 229. ^David Applebaum (2004). LÃ©vy_Processes_and_Stochastic_Calculus.
      Cambridge University Press. p. 69. ISBN 978-0-521-83263-2.
 230. ^Leonid Koralov; Yakov G. Sinai (2007). Theory_of_Probability_and_Random
      Processes. Springer Science & Business Media. p. 171. ISBN 978-3-540-
      68829-7.
 231. ^David Applebaum (2004). LÃ©vy_Processes_and_Stochastic_Calculus.
      Cambridge University Press. p. 19. ISBN 978-0-521-83263-2.
 232. ^Sung Nok Chiu; Dietrich Stoyan; Wilfrid S. Kendall; Joseph Mecke (2013).
      Stochastic_Geometry_and_Its_Applications. John Wiley & Sons. p. 109.
      ISBN 978-1-118-65825-3.
 233. ^Sung Nok Chiu; Dietrich Stoyan; Wilfrid S. Kendall; Joseph Mecke (2013).
      Stochastic_Geometry_and_Its_Applications. John Wiley & Sons. p. 108.
      ISBN 978-1-118-65825-3.
 234. ^Martin Haenggi (2013). Stochastic_Geometry_for_Wireless_Networks.
      Cambridge University Press. p. 10. ISBN 978-1-107-01469-5.
 235. ^D.J. Daley; D. Vere-Jones (2006). An_Introduction_to_the_Theory_of_Point
      Processes:_Volume_I:_Elementary_Theory_and_Methods. Springer Science &
      Business Media. p. 194. ISBN 978-0-387-21564-8.
 236. ^ a bD.R. Cox; Valerie Isham (1980). Point_Processes. CRC Press. p. 3.
      ISBN 978-0-412-21910-8.
 237. ^J. F. C. Kingman (1992). Poisson_Processes. Clarendon Press. p. 8.
      ISBN 978-0-19-159124-2.
 238. ^Jesper Moller; Rasmus Plenge Waagepetersen (2003). Statistical_Inference
      and_Simulation_for_Spatial_Point_Processes. CRC Press. p. 7. ISBN 978-0-
      203-49693-0.
 239. ^Samuel Karlin; Howard E. Taylor (2012). A_First_Course_in_Stochastic
      Processes. Academic Press. p. 31. ISBN 978-0-08-057041-9.
 240. ^Volker Schmidt (2014). Stochastic_Geometry,_Spatial_Statistics_and
      Random_Fields:_Models_and_Algorithms. Springer. p. 99. ISBN 978-3-319-
      10064-7.
 241. ^D.J. Daley; D. Vere-Jones (2006). An_Introduction_to_the_Theory_of_Point
      Processes:_Volume_I:_Elementary_Theory_and_Methods. Springer Science &
      Business Media. ISBN 978-0-387-21564-8.
 242. ^D.R. Cox; Valerie Isham (1980). Point_Processes. CRC Press. ISBN 978-0-
      412-21910-8.
 243. ^ a b c d e fGagniuc, Paul A. (2017). Markov Chains: From Theory to
      Implementation and Experimentation. US: John Wiley & Sons. pp. 1â2.
      ISBN 978-1-119-38755-8.
 244. ^David, F. N. (1955). "Studies in the History of Probability and
      Statistics I. Dicing and Gaming (A Note on the History of Probability)".
      Biometrika. 42 (1/2): 1â15. doi:10.2307/2333419. ISSN 0006-3444.
      JSTOR 2333419.
 245. ^L. E. Maistrov (2014). Probability_Theory:_A_Historical_Sketch. Elsevier
      Science. p. 1. ISBN 978-1-4832-1863-2.
 246. ^ a bSeneta, E. (2006). "Probability, History of". Encyclopedia of
      Statistical Sciences. p. 1. doi:10.1002/0471667196.ess2065.pub2.
      ISBN 978-0471667193.
 247. ^John Tabak (2014). Probability_and_Statistics:_The_Science_of
      Uncertainty. Infobase Publishing. pp. 24â26. ISBN 978-0-8160-6873-9.
 248. ^Bellhouse, David (2005). "Decoding Cardano's Liber de Ludo Aleae".
      Historia Mathematica. 32 (2): 180â202. doi:10.1016/j.hm.2004.04.001.
      ISSN 0315-0860.
 249. ^Anders Hald (2005). A_History_of_Probability_and_Statistics_and_Their
      Applications_before_1750. John Wiley & Sons. p. 221. ISBN 978-0-471-
      72517-6.
 250. ^L. E. Maistrov (2014). Probability_Theory:_A_Historical_Sketch. Elsevier
      Science. p. 56. ISBN 978-1-4832-1863-2.
 251. ^John Tabak (2014). Probability_and_Statistics:_The_Science_of
      Uncertainty. Infobase Publishing. p. 37. ISBN 978-0-8160-6873-9.
 252. ^ a bChung, Kai Lai (1998). "Probability and Doob". The American
      Mathematical Monthly. 105 (1): 28â35. doi:10.2307/2589523. ISSN 0002-
      9890. JSTOR 2589523.
 253. ^ a b c d e fBingham, N. (2000). "Studies in the history of probability
      and statistics XLVI. Measure into probability: from Lebesgue to
      Kolmogorov". Biometrika. 87 (1): 145â156. doi:10.1093/biomet/87.1.145.
      ISSN 0006-3444.
 254. ^ a bBenzi, Margherita; Benzi, Michele; Seneta, Eugene (2007). "Francesco
      Paolo Cantelli. b. 20 December 1875 d. 21 July 1966". International
      Statistical Review. 75 (2): 128. doi:10.1111/j.1751-5823.2007.00009.x.
      ISSN 0306-7734.
 255. ^Doob, Joseph L. (1996). "The Development of Rigor in Mathematical
      Probability (1900-1950)". The American Mathematical Monthly. 103 (7):
      586â595. doi:10.2307/2974673. ISSN 0002-9890. JSTOR 2974673.
 256. ^ a b c d e f g h i jCramer, Harald (1976). "Half a Century with
      Probability Theory: Some Personal Recollections". The Annals of
      Probability. 4 (4): 509â546. doi:10.1214/aop/1176996025. ISSN 0091-
      1798.
 257. ^Truesdell, C. (1975). "Early kinetic theories of gases". Archive for
      History of Exact Sciences. 15 (1): 22â23. doi:10.1007/BF00327232.
      ISSN 0003-9519.
 258. ^Brush, Stephen G. (1967). "Foundations of statistical mechanics
      1845?1915". Archive for History of Exact Sciences. 4 (3): 150â151. doi:
      10.1007/BF00412958. ISSN 0003-9519.
 259. ^Truesdell, C. (1975). "Early kinetic theories of gases". Archive for
      History of Exact Sciences. 15 (1): 31â32. doi:10.1007/BF00327232.
      ISSN 0003-9519.
 260. ^Brush, S.G. (1958). "The development of the kinetic theory of gases IV.
      Maxwell". Annals of Science. 14 (4): 243â255. doi:10.1080/
      00033795800200147. ISSN 0003-3790.
 261. ^Brush, Stephen G. (1968). "A history of random processes". Archive for
      History of Exact Sciences. 5 (1): 15â16. doi:10.1007/BF00328110.
      ISSN 0003-9519.
 262. ^ a b c dKendall, D. G.; Batchelor, G. K.; Bingham, N. H.; Hayman, W. K.;
      Hyland, J. M. E.; Lorentz, G. G.; Moffatt, H. K.; Parry, W.; Razborov, A.
      A.; Robinson, C. A.; Whittle, P. (1990). "Andrei Nikolaevich Kolmogorov
      (1903â1987)". Bulletin of the London Mathematical Society. 22 (1): 33.
      doi:10.1112/blms/22.1.31. ISSN 0024-6093.
 263. ^Vere-Jones, David (2006). "Khinchin, Aleksandr Yakovlevich".
      Encyclopedia of Statistical Sciences. p. 1. doi:10.1002/
      0471667196.ess6027.pub2. ISBN 978-0471667193.
 264. ^ a bVere-Jones, David (2006). "Khinchin, Aleksandr Yakovlevich".
      Encyclopedia of Statistical Sciences. p. 4. doi:10.1002/
      0471667196.ess6027.pub2. ISBN 978-0471667193.
 265. ^ a bSnell, J. Laurie (2005). "Obituary: Joseph Leonard Doob". Journal of
      Applied Probability. 42 (1): 251. doi:10.1239/jap/1110381384. ISSN 0021-
      9002.
 266. ^Lindvall, Torgny (1991). "W. Doeblin, 1915-1940". The Annals of
      Probability. 19 (3): 929â934. doi:10.1214/aop/1176990329. ISSN 0091-
      1798.
 267. ^ a b cGetoor, Ronald (2009). "J. L. Doob: Foundations of stochastic
      processes and probabilistic potential theory". The Annals of Probability.
      37 (5): 1655. arXiv:0909.4213. doi:10.1214/09-AOP465. ISSN 0091-1798.
 268. ^ a bBingham, N. H. (2005). "Doob: a half-century on". Journal of Applied
      Probability. 42 (1): 257â266. doi:10.1239/jap/1110381385. ISSN 0021-
      9002.
 269. ^ a b c d eMeyer, Paul-AndrÃ© (2009). "Stochastic Processes from 1950 to
      the Present". Electronic Journal for History of Probability and
      Statistics. 5 (1): 1â42.
 270. ^"Kiyosi ItÃ´ receives Kyoto Prize". Notices of the AMS. 45 (8):
      981â982. 1998.
 271. ^Jean Bertoin (1998). LÃ©vy_Processes. Cambridge University Press.
      p. viii and ix. ISBN 978-0-521-64632-1.
 272. ^J. Michael Steele (2012). Stochastic_Calculus_and_Financial
      Applications. Springer Science & Business Media. p. 176. ISBN 978-1-4684-
      9305-4.
 273. ^P. Hall; C. C. Heyde (2014). Martingale_Limit_Theory_and_Its
      Application. Elsevier Science. pp. 1, 2. ISBN 978-1-4832-6322-9.
 274. ^Dynkin, E. B. (1989). "Kolmogorov and the Theory of Markov Processes".
      The Annals of Probability. 17 (3): 822â832. doi:10.1214/aop/1176991248.
      ISSN 0091-1798.
 275. ^Ellis, Richard S. (1995). "An overview of the theory of large deviations
      and applications to statistical mechanics". Scandinavian Actuarial
      Journal. 1995 (1): 98. doi:10.1080/03461238.1995.10413952. ISSN 0346-
      1238.
 276. ^Raussen, Martin; Skau, Christian (2008). "Interview with Srinivasa
      Varadhan". Notices of the AMS. 55 (2): 238â246.
 277. ^Malte Henkel; Dragi Karevski (2012). Conformal_Invariance:_an
      Introduction_to_Loops,_Interfaces_and_Stochastic_Loewner_Evolution.
      Springer Science & Business Media. p. 113. ISBN 978-3-642-27933-1.
 278. ^"2006 Fields Medals Awarded". Notices of the AMS. 53 (9): 1041â1044.
      2015.
 279. ^Quastel, Jeremy (2015). "The Work of the 2014 Fields Medalists". Notices
      of the AMS. 62 (11): 1341â1344.
 280. ^D.J. Daley; D. Vere-Jones (2006). An_Introduction_to_the_Theory_of_Point
      Processes:_Volume_I:_Elementary_Theory_and_Methods. Springer Science &
      Business Media. pp. 1â4. ISBN 978-0-387-21564-8.
 281. ^Anders Hald (2005). A_History_of_Probability_and_Statistics_and_Their
      Applications_before_1750. John Wiley & Sons. p. 226. ISBN 978-0-471-
      72517-6.
 282. ^ a bJoel Louis Lebowitz (1984). Nonequilibrium_phenomena_II:_from
      stochastics_to_hydrodynamics. North-Holland Pub. pp. 8â10. ISBN 978-0-
      444-86806-0.
 283. ^Ionut Florescu (2014). Probability_and_Stochastic_Processes. John Wiley
      & Sons. p. 374. ISBN 978-1-118-59320-2.
 284. ^Oliver C. Ibe (2013). Elements_of_Random_Walk_and_Diffusion_Processes.
      John Wiley & Sons. p. 5. ISBN 978-1-118-61793-9.
 285. ^Anders Hald (2005). A_History_of_Probability_and_Statistics_and_Their
      Applications_before_1750. John Wiley & Sons. p. 63. ISBN 978-0-471-72517-
      6.
 286. ^Anders Hald (2005). A_History_of_Probability_and_Statistics_and_Their
      Applications_before_1750. John Wiley & Sons. p. 202. ISBN 978-0-471-
      72517-6.
 287. ^Ionut Florescu (2014). Probability_and_Stochastic_Processes. John Wiley
      & Sons. p. 385. ISBN 978-1-118-59320-2.
 288. ^Barry D. Hughes (1995). Random_Walks_and_Random_Environments:_Random
      walks. Clarendon Press. p. 111. ISBN 978-0-19-853788-5.
 289. ^Thiele, Thorwald N. (1880). "Om_Anvendelse_af_mindste_Kvadraterbs
      Methode_i_nogle_TilfÃ¦lde,_hvoren_Komplikation_af_visse_Slags_uensartede
      tilfÃ¦ldige_Fejlkilder_giver_Fejleneen_"systematisk"_Karakter". Kongelige
      Danske Videnskabernes Selskabs Skrifter. Series 5 (12): 381â408.
 290. ^Hald, Anders (1981). "T. N. Thiele's Contributions to Statistics".
      International Statistical Review / Revue Internationale de Statistique.
      49 (1): 1â20. doi:10.2307/1403034. ISSN 0306-7734. JSTOR 1403034.
 291. ^ a bLauritzen, Steffen L. (1981). "Time Series Analysis in 1880: A
      Discussion of Contributions Made by T.N. Thiele". International
      Statistical Review / Revue Internationale de Statistique. 49 (3):
      319â320. doi:10.2307/1402616. ISSN 0306-7734. JSTOR 1402616.
 292. ^Bachelier, Luis (1900). "ThÃ©orie_de_la_spÃ©culation" (PDF). Ann._Sci.
      Ãc._Norm._SupÃ©r. Serie 3;17: 21â89.
 293. ^Bachelier, Luis (1900). "The_Theory_of_Speculation". Ann. Sci. Ãc.
      Norm. SupÃ©r. Serie 3;17: 21â89 (Engl. translation by David R. May,
      2011).
 294. ^ a bCourtault, Jean-Michel; Kabanov, Yuri; Bru, Bernard; Crepel, Pierre;
      Lebon, Isabelle; Le Marchand, Arnaud (2000). "Louis Bachelier on the
      Centenary of Theorie de la Speculation". Mathematical Finance. 10 (3):
      339â353. doi:10.1111/1467-9965.00098. ISSN 0960-1627.
 295. ^ a b c d eJovanovic, Franck (2012). "Bachelier: Not the forgotten
      forerunner he has been depicted as. An analysis of the dissemination of
      Louis Bachelier's work in economics". The European Journal of the History
      of Economic Thought. 19 (3): 431â451. doi:10.1080/09672567.2010.540343.
      ISSN 0967-2567.
 296. ^Brush, Stephen G. (1968). "A history of random processes". Archive for
      History of Exact Sciences. 5 (1): 25. doi:10.1007/BF00328110. ISSN 0003-
      9519.
 297. ^Brush, Stephen G. (1968). "A history of random processes". Archive for
      History of Exact Sciences. 5 (1): 1â36. doi:10.1007/BF00328110.
      ISSN 0003-9519.
 298. ^D.J. Daley; D. Vere-Jones (2006). An_Introduction_to_the_Theory_of_Point
      Processes:_Volume_I:_Elementary_Theory_and_Methods. Springer Science &
      Business Media. pp. 8â9. ISBN 978-0-387-21564-8.
 299. ^Embrechts, Paul; Frey, RÃ¼diger; Furrer, HansjÃ¶rg (2001). "Stochastic
      processes in insurance and finance". Stochastic Processes: Theory and
      Methods. Handbook of Statistics. 19. p. 367. doi:10.1016/S0169-7161
      (01)19014-0. ISBN 978-0444500144. ISSN 0169-7161.
 300. ^CramÃ©r, Harald (1969). "Historical review of Filip Lundberg's works on
      risk theory". Scandinavian Actuarial Journal. 1969 (sup3): 6â12. doi:
      10.1080/03461238.1969.10404602. ISSN 0346-1238.
 301. ^ a bGagniuc, Paul A. (2017). Markov Chains: From Theory to
      Implementation and Experimentation. NJ: John Wiley & Sons. pp. 2â8.
      ISBN 978-1-119-38755-8.
 302. ^ a b c dCharles Miller Grinstead; James Laurie Snell (1997).
      Introduction_to_Probability. American Mathematical Soc. pp. 464â466.
      ISBN 978-0-8218-0749-1.
 303. ^ a bPierre Bremaud (2013). Markov_Chains:_Gibbs_Fields,_Monte_Carlo
      Simulation,_and_Queues. Springer Science & Business Media. p. ix.
      ISBN 978-1-4757-3124-8.
 304. ^ a bHayes, Brian (2013). "First links in the Markov chain". American
      Scientist. 101 (2): 92â96. doi:10.1511/2013.101.92.
 305. ^Seneta, E. (1998). "I.J. BienaymÃ© [1796-1878]: Criticality, Inequality,
      and Internationalization". International Statistical Review / Revue
      Internationale de Statistique. 66 (3): 291â292. doi:10.2307/1403518.
      ISSN 0306-7734. JSTOR 1403518.
 306. ^Bru, B.; Hertz, S. (2001). "Maurice FrÃ©chet". Statisticians of the
      Centuries. pp. 331â334. doi:10.1007/978-1-4613-0179-0_71. ISBN 978-0-
      387-95283-3.
 307. ^Marc Barbut; Bernard Locker; Laurent Mazliak (2016). Paul_LÃ©vy_and
      Maurice_FrÃ©chet:_50_Years_of_Correspondence_in_107_Letters. Springer
      London. p. 5. ISBN 978-1-4471-7262-8.
 308. ^Valeriy Skorokhod (2005). Basic_Principles_and_Applications_of
      Probability_Theory. Springer Science & Business Media. p. 146. ISBN 978-
      3-540-26312-8.
 309. ^Bernstein, Jeremy (2005). "Bachelier". American Journal of Physics. 73
      (5): 398â396. Bibcode:2005AmJPh..73..395B. doi:10.1119/1.1848117.
      ISSN 0002-9505.
 310. ^William J. Anderson (2012). Continuous-Time_Markov_Chains:_An
      Applications-Oriented_Approach. Springer Science & Business Media.
      p. vii. ISBN 978-1-4612-3038-0.
 311. ^Kendall, D. G.; Batchelor, G. K.; Bingham, N. H.; Hayman, W. K.; Hyland,
      J. M. E.; Lorentz, G. G.; Moffatt, H. K.; Parry, W.; Razborov, A. A.;
      Robinson, C. A.; Whittle, P. (1990). "Andrei Nikolaevich Kolmogorov
      (1903â1987)". Bulletin of the London Mathematical Society. 22 (1): 57.
      doi:10.1112/blms/22.1.31. ISSN 0024-6093.
 312. ^David Applebaum (2004). LÃ©vy_Processes_and_Stochastic_Calculus.
      Cambridge University Press. p. 67. ISBN 978-0-521-83263-2.
 313. ^ a b cRobert J. Adler (2010). The_Geometry_of_Random_Fields. SIAM.
      p. 13. ISBN 978-0-89871-693-1.
 314. ^Krishna B. Athreya; Soumendra N. Lahiri (2006). Measure_Theory_and
      Probability_Theory. Springer Science & Business Media. ISBN 978-0-387-
      32903-1.
 315. ^Bernt Ãksendal (2003). Stochastic_Differential_Equations:_An
      Introduction_with_Applications. Springer Science & Business Media. p. 11.
      ISBN 978-3-540-04758-2.
 316. ^David Williams (1991). Probability_with_Martingales. Cambridge
      University Press. p. 124. ISBN 978-0-521-40605-5.
 317. ^Rick Durrett (2010). Probability:_Theory_and_Examples. Cambridge
      University Press. p. 410. ISBN 978-1-139-49113-6.
 318. ^Patrick Billingsley (2008). Probability_and_Measure. Wiley India Pvt.
      Limited. pp. 493â494. ISBN 978-81-265-1771-8.
 319. ^Alexander A. Borovkov (2013). Probability_Theory. Springer Science &
      Business Media. pp. 529â530. ISBN 978-1-4471-5201-9.
 320. ^Krishna B. Athreya; Soumendra N. Lahiri (2006). Measure_Theory_and
      Probability_Theory. Springer Science & Business Media. p. 221. ISBN 978-
      0-387-32903-1.
 321. ^ a bRobert J. Adler; Jonathan E. Taylor (2009). Random_Fields_and
      Geometry. Springer Science & Business Media. p. 14. ISBN 978-0-387-48116-
      6.
 322. ^Krishna B. Athreya; Soumendra N. Lahiri (2006). Measure_Theory_and
      Probability_Theory. Springer Science & Business Media. p. 211. ISBN 978-
      0-387-32903-1.
 323. ^Alexander A. Borovkov (2013). Probability_Theory. Springer Science &
      Business Media. p. 536. ISBN 978-1-4471-5201-9.
 324. ^Benjamin Yakir (2013). Extremes_in_Random_Fields:_A_Theory_and_Its
      Applications. John Wiley & Sons. p. 5. ISBN 978-1-118-72062-2.
***** Further reading[edit] *****
 This article's further_reading may not follow Wikipedia's content_policies or
 guidelines. Please improve_this_article by removing less relevant or redundant
 publications with the same_point_of_view; or by incorporating the relevant
 publications into the body of the article through appropriate citations. (July
 2018)(Learn_how_and_when_to_remove_this_template_message)
**** Articles[edit] ****
    * Applebaum, David (2004). "LÃ©vy processes: From probability to finance
      and quantum groups". Notices of the AMS. 51 (11): 1336â1347.
Cramer, Harald (1976). "Half a Century with Probability Theory: Some Personal
Recollections". The Annals of Probability. 4 (4): 509â546. doi:10.1214/aop/
1176996025. ISSN 0091-1798.
Guttorp, Peter; Thorarinsdottir, Thordis L. (2012). "What Happened to Discrete
Chaos, the Quenouille Process, and the Sharp Markov Property? Some History of
Stochastic Point Processes". International Statistical Review. 80 (2):
253â268. doi:10.1111/j.1751-5823.2012.00181.x. ISSN 0306-7734.
Jarrow, Robert; Protter, Philip (2004). "A short history of stochastic
integration and mathematical finance: the early years, 1880â1970". A
Festschrift for Herman Rubin. Institute of Mathematical Statistics Lecture
Notes - Monograph Series. pp. 75â91. doi:10.1214/lnms/1196285381. ISBN 978-0-
940600-61-4. ISSN 0749-2170.
Meyer, Paul-AndrÃ© (2009). "Stochastic Processes from 1950 to the Present".
Electronic Journal for History of Probability and Statistics. 5 (1): 1â42.
**** Books[edit] ****
    * Robert J. Adler (2010). The_Geometry_of_Random_Fields. SIAM. ISBN 978-0-
      89871-693-1.
Robert J. Adler; Jonathan E. Taylor (2009). Random_Fields_and_Geometry.
Springer Science & Business Media. ISBN 978-0-387-48116-6.
Pierre BrÃ©maud (2013). Markov_Chains:_Gibbs_Fields,_Monte_Carlo_Simulation,
and_Queues. Springer Science & Business Media. ISBN 978-1-4757-3124-8.
Joseph_L._Doob (1990). Stochastic_processes. Wiley.
Anders Hald (2005). A_History_of_Probability_and_Statistics_and_Their
Applications_before_1750. John Wiley & Sons. ISBN 978-0-471-72517-6.
Crispin_Gardiner (2010). Stochastic_Methods. Springer. ISBN 978-3-540-70712-7.
Iosif I. Gikhman; Anatoly Vladimirovich Skorokhod (1996). Introduction_to_the
Theory_of_Random_Processes. Courier Corporation. ISBN 978-0-486-69387-3.
Emanuel_Parzen (2015). Stochastic_Processes. Courier Dover Publications.
ISBN 978-0-486-79688-8.
Murray_Rosenblatt (1962). Random_Processes. Oxford University Press.
***** External links[edit] *****
    *  Media related to Stochastic_processes at Wikimedia Commons
    * v
    * t
    * e
Stochastic processes
                       * Bernoulli_process
                       * Branching_process
                       * Chinese_restaurant_process
                       * GaltonâWatson_process
                       * Independent_and_identically_distributed_random
                         variables
Discrete_time          * Markov_chain
                       * Moran_process
                       * Random_walk
                             o Loop-erased
                             o Self-avoiding
                             o Biased
                             o Maximal_entropy
                       * Bessel_process
                       * Birthâdeath_process
                       * Brownian_motion
                             o Bridge
                             o Excursion
                             o Fractional
                             o Geometric
                             o Meander
                       * Cauchy_process
                       * Contact_process
                       * Continuous-time_random_walk
                       * Cox_process
                       * Diffusion_process
                       * Empirical_process
                       * Feller_process
                       * FlemingâViot_process
                       * Gamma_process
                       * Geometric_process
                       * Hunt_process
                       * Interacting_particle_systems
Continuous_time        * ItÃ´_diffusion
                       * ItÃ´_process
                       * Jump_diffusion
                       * Jump_process
                       * LÃ©vy_process
                       * Local_time
                       * Markov_additive_process
                       * McKeanâVlasov_process
                       * OrnsteinâUhlenbeck_process
                       * Poisson_process
                             o Compound
                             o Non-homogeneous
                             o Point_process
                       * SchrammâLoewner_evolution
                       * Semimartingale
                       * Sigma-martingale
                       * Stable_process
                       * Superprocess
                       * Telegraph_process
                       * Variance_gamma_process
                       * Wiener_process
                       * Wiener_sausage
                       * Branching_process
                       * GalvesâLÃ¶cherbach_model
                       * Gaussian_process
                       * Hidden_Markov_model_(HMM)
                       * Markov_process
                       * Martingale
                             o Differences
Both                         o Local
                             o Sub-
                             o Super-
                       * Random_dynamical_system
                       * Regenerative_process
                       * Renewal_process
                       * Stochastic_chains_with_memory_of_variable_length
                       * White_noise
                       * Dirichlet_process
                       * Gaussian_random_field
                       * Gibbs_measure
                       * Hopfield_model
                       * Ising_model
                             o Potts_model
                             o Boolean_network
Fields and other       * Markov_random_field
                       * Percolation
                       * PitmanâYor_process
                       * Point_process
                             o Cox
                             o Poisson
                       * Random_field
                       * Random_graph
                       * Autoregressive_conditional_heteroskedasticity_(ARCH)
                         model
                       * Autoregressive_integrated_moving_average_(ARIMA)_model
Time_series_models     * Autoregressive_(AR)_model
                       * Autoregressiveâmoving-average_(ARMA)_model
                       * Generalized_autoregressive_conditional
                         heteroskedasticity_(GARCH)_model
                       * Moving-average_(MA)_model
                       * BlackâDermanâToy
                       * BlackâKarasinski
                       * BlackâScholes
                       * Chen
                       * Constant_elasticity_of_variance_(CEV)
                       * CoxâIngersollâRoss_(CIR)
                       * GarmanâKohlhagen
Financial models       * HeathâJarrowâMorton_(HJM)
                       * Heston
                       * HoâLee
                       * HullâWhite
                       * LIBOR_market
                       * RendlemanâBartter
                       * SABR_volatility
                       * VaÅ¡Ã­Äek
                       * Wilkie
                       * BÃ¼hlmann
Actuarial_models       * CramÃ©râLundberg
                       * Risk_process
                       * SparreâAnderson
                       * Bulk
                       * Fluid
Queueing_models        * Generalized_queueing_network
                       * M/G/1
                       * M/M/1
                       * M/M/c
                       * CÃ dlÃ g_paths
                       * Continuous
                       * Continuous_paths
                       * Ergodic
                       * Exchangeable
                       * Feller-continuous
                       * GaussâMarkov
Properties             * Markov
                       * Mixing
                       * Piecewise_deterministic
                       * Predictable
                       * Progressively_measurable
                       * Self-similar
                       * Stationary
                       * Time-reversible
                       * Central_limit_theorem
                       * Donsker's_theorem
                       * Doob's_martingale_convergence_theorems
                       * Ergodic_theorem
Limit theorems         * FisherâTippettâGnedenko_theorem
                       * Large_deviation_principle
                       * Law_of_large_numbers_(weak/strong)
                       * Law_of_the_iterated_logarithm
                       * Maximal_ergodic_theorem
                       * Sanov's_theorem
                       * BurkholderâDavisâGundy
Inequalities           * Doob's_martingale
                       * KunitaâWatanabe
                       * CameronâMartin_formula
                       * Convergence_of_random_variables
                       * DolÃ©ans-Dade_exponential
                       * Doob_decomposition_theorem
                       * DoobâMeyer_decomposition_theorem
                       * Doob's_optional_stopping_theorem
                       * Dynkin's_formula
                       * FeynmanâKac_formula
                       * Filtration
                       * Girsanov_theorem
                       * Infinitesimal_generator
                       * ItÃ´_integral
                       * ItÃ´'s_lemma
                       * Kolmogorov_continuity_theorem
                       * Kolmogorov_extension_theorem
                       * LÃ©vyâProkhorov_metric
                       * Malliavin_calculus
Tools                  * Martingale_representation_theorem
                       * Optional_stopping_theorem
                       * Prokhorov's_theorem
                       * Quadratic_variation
                       * Reflection_principle
                       * Skorokhod_integral
                       * Skorokhod's_representation_theorem
                       * Skorokhod_space
                       * Snell_envelope
                       * Stochastic_differential_equation
                             o Tanaka
                       * Stopping_time
                       * Stratonovich_integral
                       * Uniform_integrability
                       * Usual_hypotheses
                       * Wiener_space
                             o Classical
                             o Abstract
                       * Actuarial_mathematics
                       * Econometrics
                       * Ergodic_theory
                       * Extreme_value_theory_(EVT)
                       * Large_deviations_theory
                       * Mathematical_finance
                       * Mathematical_statistics
Disciplines            * Probability_theory
                       * Queueing_theory
                       * Renewal_theory
                       * Ruin_theory
                       * Statistics
                       * System_on_Chip design
                       * Stochastic_analysis
                       * Time_series_analysis
                       * Machine_learning
    * List_of_topics
    * Category
    * v
    * t
    * e
Industrial_and_applied_mathematics
                       * Computational_logic
                       * Algorithms
                             o design
Computational                o analysis
                       * Information_theory
                       * Coding_theory
                       * Cryptography
                       * Computer_algebra
                       * Computational_number_theory
Discrete               * Combinatorics
                       * Graph_theory
                       * Discrete_geometry
                                 * Operator_algebra
                                 * Representation_theory
                   Algebraic     * Renormalization_group
                                 * Feynman_integral
Mathematical                     * M-theory
physics                          * Differential_geometry
                                 * Fourier_analysis
                   Analytic      * Harmonic_analysis
                                 * Functional_analysis
                                 * Operator_theory
                       * Approximation_theory
                       * Numerical_analysis
Analysis               * Differential_equations
                       * Dynamical_systems
                       * Control_theory
                       * Variational_calculus
                       * Distributions (random_variables)
Probability_theory     * Stochastic processes / analysis
                       * Path_integral
                       * Stochastic_variational_calculus
                       * Statistics
                       * Operations_research
Decision_sciences      * Optimization
                       * Game_theory
                       * Mathematical_economics
                       * Mathematical_finance
                       * Biology
                       * Chemistry
Other applications     * Psychology
                       * Sociology
                       * "The_Unreasonable_Effectiveness_of_Mathematics_in_the
                         Natural_Sciences"
    * Category
    * Mathematics_portal / outline / topics_list

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Stochastic_process&oldid=909922576"
Categories:
    * Stochastic_processes
    * Stochastic_models
    * Statistical_data_types
Hidden categories:
    * CS1:_long_volume_value
    * Wikipedia_spam_cleanup_from_July_2018
    * Wikipedia_further_reading_cleanup
    * Commons_category_link_is_on_Wikidata
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * à´®à´²à´¯à´¾à´³à´
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 8 August 2019, at 14:11 (UTC).
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
