The following text has been accessed from https://en.wikipedia.org/wiki/Random_variable at Thu Aug 8 22:51:45 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Random variable ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (February 2012)(Learn_how_and
 when_to_remove_this_template_message)
Part of a series on statistics
Probability_theory
[Nuvola_apps_atlantik.png]
    * Probability_axioms
    * Probability_space
    * Sample_space
    * Elementary_event
    * Event
    * Random variable
    * Probability_measure
    * Complementary_event
    * Joint_probability
    * Marginal_probability
    * Conditional_probability
    * Independence
    * Conditional_independence
    * Law_of_total_probability
    * Law_of_large_numbers
    * Bayes'_theorem
    * Boole's_inequality
    * Venn_diagram
    * Tree_diagram
    * v
    * t
    * e
In probability_and_statistics, a random variable, random quantity, aleatory
variable, or stochastic variable is described informally as a variable_whose
values_depend on outcomes of a random phenomenon.[1] The formal mathematical
treatment of random variables is a topic in probability_theory. In that
context, a random variable is understood as a measurable_function defined on a
probability_space whose outcomes are typically real numbers.[2]
This graph shows how random variable is a function from all possible outcomes
to numerical quantities and also how it is used for defining probability mass
functions.
A random variable's possible values might represent the possible outcomes of a
yet-to-be-performed experiment, or the possible outcomes of a past experiment
whose already-existing value is uncertain (for example, because of imprecise
measurements or quantum_uncertainty). They may also conceptually represent
either the results of an "objectively" random process (such as rolling a die)
or the "subjective" randomness that results from incomplete knowledge of a
quantity. The meaning of the probabilities assigned to the potential values of
a random variable is not part of probability theory itself but is instead
related to philosophical arguments over the interpretation_of_probability. The
mathematics works the same regardless of the particular interpretation in use.
As a function, a random variable is required to be measurable, which allows for
probabilities to be assigned to sets of its potential values. It is common that
the outcomes depend on some physical variables that are not predictable. For
example, when tossing a fair coin, the final outcome of heads or tails depends
on the uncertain physical conditions. Which outcome will be observed is not
certain. The coin could get caught in a crack in the floor, but such a
possibility is excluded from consideration.
The domain of a random variable is a sample space, which is interpreted as the
set of possible outcomes of a random phenomenon. For example, in the case of a
coin toss, only two possible outcomes are considered, namely heads or tails.
A random variable has a probability_distribution, which specifies the
probability of its values. Random variables can be discrete, that is, taking
any of a specified finite or countable_list of values, endowed with a
probability_mass_function characteristic of the random variable's probability
distribution; or continuous, taking any numerical value in an interval or
collection of intervals, via a probability_density_function that is
characteristic of the random variable's probability distribution; or a mixture
of both types.
Two random variables with the same probability distribution can still differ in
terms of their associations with, or independence from, other random variables.
The realizations of a random variable, that is, the results of randomly
choosing values according to the variable's probability distribution function,
are called random_variates.
⁰
***** Contents *****
    * 1_Definition
          o 1.1_Standard_case
          o 1.2_Extensions
    * 2_Distribution_functions
    * 3_Examples
          o 3.1_Discrete_random_variable
                # 3.1.1_Coin_toss
                # 3.1.2_Dice_roll
          o 3.2_Continuous_random_variable
          o 3.3_Mixed_type
    * 4_Measure-theoretic_definition
          o 4.1_Real-valued_random_variables
    * 5_Moments
    * 6_Functions_of_random_variables
          o 6.1_Example_1
          o 6.2_Example_2
          o 6.3_Example_3
          o 6.4_Example_4
    * 7_Equivalence_of_random_variables
          o 7.1_Equality_in_distribution
          o 7.2_Almost_sure_equality
          o 7.3_Equality
    * 8_Convergence
    * 9_Notes
    * 10_See_also
    * 11_References
          o 11.1_Literature
    * 12_External_links
***** Definition[edit] *****
A random variable is a measurable_function     X &#x003A; &#x03A9; &#x2192; E
{\displaystyle X\colon \Omega \to E}  [{\displaystyle X\colon \Omega \to E}]
from a set of possible outcomes     &#x03A9;   {\displaystyle \Omega }  [\Omega
] to a measurable_space     E   {\displaystyle E}  [E]. The technical axiomatic
definition requires     &#x03A9;   {\displaystyle \Omega }  [\Omega ] to be a
sample space of a probability_triple (see the measure-theoretic_definition).
The probability that     X   {\displaystyle X}  [X] takes on a value in a
measurable set     S &#x2286; E   {\displaystyle S\subseteq E}  [{\displaystyle
S\subseteq E}] is written as
         P &#x2061; ( X &#x2208; S ) = P &#x2061; ( { &#x03C9; &#x2208;
      &#x03A9; &#x2223; X ( &#x03C9; ) &#x2208; S } )   {\displaystyle
      \operatorname {P} (X\in S)=\operatorname {P} (\{\omega \in \Omega \mid X
      (\omega )\in S\})}  [{\displaystyle \operatorname {P} (X\in
      S)=\operatorname {P} (\{\omega \in \Omega \mid X(\omega )\in S\})}],
where     P   {\displaystyle \operatorname {P} }  [\operatorname {P} ] is the
probability_measure on     ( &#x03A9; ,   F   )   {\displaystyle (\Omega ,
{\mathcal {F}})}  [(\Omega, \mathcal{F})].
**** Standard case[edit] ****
In many cases,     X   {\displaystyle X}  [X] is real-valued, i.e.     E =  R
{\displaystyle E=\mathbb {R} }  [E = \mathbb{R}]. In some contexts, the term
random_element (see extensions) is used to denote a random variable not of this
form.
When the image (or range) of     X   {\displaystyle X}  [X] is countable, the
random variable is called a discrete random variable[3]:399 and its
distribution can be described by a probability_mass_function that assigns a
probability to each value in the image of     X   {\displaystyle X}  [X]. If
the image is uncountably infinite then     X   {\displaystyle X}  [X] is called
a continuous random variable. In the special case that it is absolutely
continuous, its distribution can be described by a probability_density
function, which assigns probabilities to intervals; in particular, each
individual point must necessarily have probability zero for an absolutely
continuous random variable. Not all continuous random variables are absolutely
continuous,[4] for example a mixture_distribution. Such random variables cannot
be described by a probability density or a probability mass function.
Any random variable can be described by its cumulative_distribution_function,
which describes the probability that the random variable will be less than or
equal to a certain value.
**** Extensions[edit] ****
The term "random variable" in statistics is traditionally limited to the real-
valued case (    E =  R    {\displaystyle E=\mathbb {R} }  [E=\mathbb {R} ]).
In this case, the structure of the real numbers makes it possible to define
quantities such as the expected_value and variance of a random variable, its
cumulative_distribution_function, and the moments of its distribution.
However, the definition above is valid for any measurable_space     E
{\displaystyle E}  [E] of values. Thus one can consider random elements of
other sets     E   {\displaystyle E}  [E], such as random boolean_values,
categorical_values, complex_numbers, vectors, matrices, sequences, trees, sets,
shapes, manifolds, and functions. One may then specifically refer to a random
variable of type     E   {\displaystyle E}  [E], or an    E   {\displaystyle E}
[E]-valued random variable.
This more general concept of a random_element is particularly useful in
disciplines such as graph_theory, machine_learning, natural_language
processing, and other fields in discrete_mathematics and computer_science,
where one is often interested in modeling the random variation of non-numerical
data_structures. In some cases, it is nonetheless convenient to represent each
element of     E   {\displaystyle E}  [E] using one or more real numbers. In
this case, a random element may optionally be represented as a vector_of_real-
valued_random_variables (all defined on the same underlying probability space
&#x03A9;   {\displaystyle \Omega }  [\Omega ], which allows the different
random variables to covary). For example:
    * A random word may be represented as a random integer that serves as an
      index into the vocabulary of possible words. Alternatively, it can be
      represented as a random indicator vector whose length equals the size of
      the vocabulary, where the only values of positive probability are     ( 1
      &#xA0; 0 &#xA0; 0 &#xA0; 0 &#xA0; &#x22EF; )   {\displaystyle (1\ 0\ 0\
      0\ \cdots )}  [{\displaystyle (1\ 0\ 0\ 0\ \cdots )}],     ( 0 &#xA0; 1
      &#xA0; 0 &#xA0; 0 &#xA0; &#x22EF; )   {\displaystyle (0\ 1\ 0\ 0\ \cdots
      )}  [{\displaystyle (0\ 1\ 0\ 0\ \cdots )}],     ( 0 &#xA0; 0 &#xA0; 1
      &#xA0; 0 &#xA0; &#x22EF; )   {\displaystyle (0\ 0\ 1\ 0\ \cdots )}  [
      {\displaystyle (0\ 0\ 1\ 0\ \cdots )}] and the position of the 1
      indicates the word.
    * A random sentence of given length     N   {\displaystyle N}  [N] may be
      represented as a vector of     N   {\displaystyle N}  [N] random words.
    * A random_graph on     N   {\displaystyle N}  [N] given vertices may be
      represented as a     N &#x00D7; N   {\displaystyle N\times N}  [N\times
      N] matrix of random variables, whose values specify the adjacency_matrix
      of the random graph.
    * A random_function     F   {\displaystyle F}  [F] may be represented as a
      collection of random variables     F ( x )   {\displaystyle F(x)}  [F
      (x)], giving the function's values at the various points     x
      {\displaystyle x}  [x] in the function's domain. The     F ( x )
      {\displaystyle F(x)}  [F(x)] are ordinary real-valued random variables
      provided that the function is real-valued. For example, a stochastic
      process is a random function of time, a random_vector is a random
      function of some index set such as     1 , 2 , &#x2026; , n
      {\displaystyle 1,2,\ldots ,n}  [{\displaystyle 1,2,\ldots ,n}], and
      random_field is a random function on any set (typically time, space, or a
      discrete set).
***** Distribution functions[edit] *****
If a random variable     X &#x003A; &#x03A9; &#x2192;  R    {\displaystyle
X\colon \Omega \to \mathbb {R} }  [X\colon \Omega \to \mathbb {R} ] defined on
the probability space     ( &#x03A9; ,   F   , P )   {\displaystyle (\Omega ,
{\mathcal {F}},\operatorname {P} )}  [{\displaystyle (\Omega ,{\mathcal
{F}},\operatorname {P} )}] is given, we can ask questions like "How likely is
it that the value of     X   {\displaystyle X}  [X] is equal to 2?". This is
the same as the probability of the event     { &#x03C9; : X ( &#x03C9; ) = 2 }
{\displaystyle \{\omega :X(\omega )=2\}\,\!}  [\{\omega :X(\omega )=2\}\,\!]
which is often written as     P ( X = 2 )     {\displaystyle P(X=2)\,\!}  [P
(X=2)\,\!] or      p  X   ( 2 )   {\displaystyle p_{X}(2)}  [p_{X}(2)] for
short.
Recording all these probabilities of output ranges of a real-valued random
variable     X   {\displaystyle X}  [X] yields the probability_distribution of
X   {\displaystyle X}  [X]. The probability distribution "forgets" about the
particular probability space used to define     X   {\displaystyle X}  [X] and
only records the probabilities of various values of     X   {\displaystyle X}
[X]. Such a probability distribution can always be captured by its cumulative
distribution_function
          F  X   ( x ) = P &#x2061; ( X &#x2264; x )   {\displaystyle F_{X}
      (x)=\operatorname {P} (X\leq x)}  [F_{X}(x)=\operatorname {P} (X\leq x)]
and sometimes also using a probability_density_function,      p  X
{\displaystyle p_{X}}  [p_{X}]. In measure-theoretic terms, we use the random
variable     X   {\displaystyle X}  [X] to "push-forward" the measure     P
{\displaystyle P}  [P] on     &#x03A9;   {\displaystyle \Omega }  [\Omega ] to
a measure      p  X     {\displaystyle p_{X}}  [p_{X}] on      R
{\displaystyle \mathbb {R} }  [\mathbb {R} ]. The underlying probability space
&#x03A9;   {\displaystyle \Omega }  [\Omega ] is a technical device used to
guarantee the existence of random variables, sometimes to construct them, and
to define notions such as correlation_and_dependence or independence based on a
joint_distribution of two or more random variables on the same probability
space. In practice, one often disposes of the space     &#x03A9;
{\displaystyle \Omega }  [\Omega ] altogether and just puts a measure on      R
{\displaystyle \mathbb {R} }  [\mathbb {R} ] that assigns measure 1 to the
whole real line, i.e., one works with probability distributions instead of
random variables. See the article on quantile_functions for fuller development.
***** Examples[edit] *****
**** Discrete random variable[edit] ****
In an experiment a person may be chosen at random, and one random variable may
be the person's height. Mathematically, the random variable is interpreted as a
function which maps the person to the person's height. Associated with the
random variable is a probability distribution that allows the computation of
the probability that the height is in any subset of possible values, such as
the probability that the height is between 180 and 190 cm, or the probability
that the height is either less than 150 or more than 200 cm.
Another random variable may be the person's number of children; this is a
discrete random variable with non-negative integer values. It allows the
computation of probabilities for individual integer values â the probability
mass function (PMF) â or for sets of values, including infinite sets. For
example, the event of interest may be "an even number of children". For both
finite and infinite event sets, their probabilities can be found by adding up
the PMFs of the elements; that is, the probability of an even number of
children is the infinite sum     PMF &#x2061; ( 0 ) + PMF &#x2061; ( 2 ) + PMF
&#x2061; ( 4 ) + &#x22EF;   {\displaystyle \operatorname {PMF}
(0)+\operatorname {PMF} (2)+\operatorname {PMF} (4)+\cdots }  [{\displaystyle
\operatorname {PMF} (0)+\operatorname {PMF} (2)+\operatorname {PMF} (4)+\cdots
}].
In examples such as these, the sample_space is often suppressed, since it is
mathematically hard to describe, and the possible values of the random
variables are then treated as a sample space. But when two random variables are
measured on the same sample space of outcomes, such as the height and number of
children being computed on the same random persons, it is easier to track their
relationship if it is acknowledged that both height and number of children come
from the same random person, for example so that questions of whether such
random variables are correlated or not can be posed.
If     {  a  n   } , {  b  n   }   {\textstyle \{a_{n}\},\{b_{n}\}}  [
{\textstyle \{a_{n}\},\{b_{n}\}}] are countable sets of real numbers,      b  n
> 0   {\textstyle b_{n}>0}  [{\textstyle b_{n}>0}] and      &#x2211;  n    b  n
= 1   {\displaystyle \sum _{n}b_{n}=1}  [{\displaystyle \sum _{n}b_{n}=1}],
then     F =  &#x2211;  n    b  n    &#x03B4;   a  n       {\displaystyle
F=\sum _{n}b_{n}\delta _{a_{n}}}  [{\displaystyle F=\sum _{n}b_{n}\delta _{a_
{n}}}] is a discrete distribution function. Here      &#x03B4;  t   ( x ) = 0
{\displaystyle \delta _{t}(x)=0}  [{\displaystyle \delta _{t}(x)=0}] for     x
< t   {\displaystyle x<t}  [{\displaystyle x<t}],      &#x03B4;  t   ( x ) = 1
{\displaystyle \delta _{t}(x)=1}  [{\displaystyle \delta _{t}(x)=1}] for     x
&#x2265; t   {\displaystyle x\geq t}  [{\displaystyle x\geq t}]. Taking for
instance an enumeration of all rational numbers as     {  a  n   }
{\displaystyle \{a_{n}\}}  [\{a_{n}\}], one gets a discrete distribution
function that is not a step function or piecewise constant.[3]

*** Coin toss[edit] ***
The possible outcomes for one coin toss can be described by the sample space
&#x03A9; = {  heads  ,  tails  }   {\displaystyle \Omega =\{{\text{heads}},
{\text{tails}}\}}  [\Omega =\{{\text{heads}},{\text{tails}}\}]. We can
introduce a real-valued random variable     Y   {\displaystyle Y}  [Y] that
models a $1 payoff for a successful bet on heads as follows:
         Y ( &#x03C9; ) =   {    1 ,    if&#xA0;  &#x03C9; =  heads  ,     0 ,
      if&#xA0;  &#x03C9; =  tails  .         {\displaystyle Y(\omega )={\begin
      {cases}1,&{\text{if }}\omega ={\text{heads}},\\[6pt]0,&{\text{if }}\omega
      ={\text{tails}}.\end{cases}}}  [{\displaystyle Y(\omega )={\begin
      {cases}1,&{\text{if }}\omega ={\text{heads}},\\[6pt]0,&{\text{if }}\omega
      ={\text{tails}}.\end{cases}}}]
If the coin is a fair_coin, Y has a probability_mass_function      f  Y
{\displaystyle f_{Y}}  [f_{Y}] given by:
          f  Y   ( y ) =   {       1 2    ,    if&#xA0;  y = 1 ,        1 2
      ,    if&#xA0;  y = 0 ,         {\displaystyle f_{Y}(y)={\begin{cases}
      {\tfrac {1}{2}},&{\text{if }}y=1,\\[6pt]{\tfrac {1}{2}},&{\text{if
      }}y=0,\end{cases}}}  [{\displaystyle f_{Y}(y)={\begin{cases}{\tfrac {1}
      {2}},&{\text{if }}y=1,\\[6pt]{\tfrac {1}{2}},&{\text{if }}y=0,\end
      {cases}}}]
*** Dice roll[edit] ***
If the sample space is the set of possible numbers rolled on two dice, and the
random variable of interest is the sum S of the numbers on the two dice, then S
is a discrete random variable whose distribution is described by the
probability_mass_function plotted as the height of picture columns here.
A random variable can also be used to describe the process of rolling dice and
the possible outcomes. The most obvious representation for the two-dice case is
to take the set of pairs of numbers n1 and n2 from {1, 2, 3, 4, 5, 6}
(representing the numbers on the two dice) as the sample space. The total
number rolled (the sum of the numbers in each pair) is then a random variable X
given by the function that maps the pair to the sum:
         X ( (  n  1   ,  n  2   ) ) =  n  1   +  n  2     {\displaystyle X((n_
      {1},n_{2}))=n_{1}+n_{2}}  [X((n_{1},n_{2}))=n_{1}+n_{2}]
and (if the dice are fair) has a probability mass function ÆX given by:
          f  X   ( S ) =    min ( S &#x2212; 1 , 13 &#x2212; S )  36   ,
      &#xA0;for&#xA0;  S &#x2208; { 2 , 3 , 4 , 5 , 6 , 7 , 8 , 9 , 10 , 11 ,
      12 }   {\displaystyle f_{X}(S)={\frac {\min(S-1,13-S)}{36}},{\text{ for
      }}S\in \{2,3,4,5,6,7,8,9,10,11,12\}}  [{\displaystyle f_{X}(S)={\frac
      {\min(S-1,13-S)}{36}},{\text{ for }}S\in \{2,3,4,5,6,7,8,9,10,11,12\}}]
**** Continuous random variable[edit] ****
Formally, a continuous random variable is a random variable whose cumulative
distribution_function is continuous everywhere.[5] There are no "gaps", which
would correspond to numbers which have a finite probability of occurring.
Instead, continuous random variables almost_never take an exact prescribed
value c (formally,     &#x2200; c &#x2208;  R  :  Pr ( X = c ) = 0
{\textstyle \forall c\in \mathbb {R} :\;\Pr(X=c)=0}  [{\textstyle \forall c\in
\mathbb {R} :\;\Pr(X=c)=0}]) but there is a positive probability that its value
will lie in particular intervals which can be arbitrarily_small. Continuous
random variables usually admit probability_density_functions (PDF), which
characterize their CDF and probability_measures; such distributions are also
called absolutely_continuous; but some continuous distributions are singular,
or mixes of an absolutely continuous part and a singular part.
An example of a continuous random variable would be one based on a spinner that
can choose a horizontal direction. Then the values taken by the random variable
are directions. We could represent these directions by North, West, East,
South, Southeast, etc. However, it is commonly more convenient to map the
sample space to a random variable which takes values which are real numbers.
This can be done, for example, by mapping a direction to a bearing in degrees
clockwise from North. The random variable then takes values which are real
numbers from the interval [0, 360), with all parts of the range being "equally
likely". In this case, X = the angle spun. Any real number has probability zero
of being selected, but a positive probability can be assigned to any range of
values. For example, the probability of choosing a number in [0, 180] is
&#x200b;1⁄2. Instead of speaking of a probability mass function, we say that
the probability density of X is 1/360. The probability of a subset of [0, 360)
can be calculated by multiplying the measure of the set by 1/360. In general,
the probability of a set for a given continuous random variable can be
calculated by integrating the density over the given set.
Given any interval     I = [ a , b ] = { x &#x2208;  R  : a &#x2264; x &#x2264;
b }   {\textstyle I=[a,b]=\{x\in \mathbb {R} :a\leq x\leq b\}}  [{\textstyle I=
[a,b]=\{x\in \mathbb {R} :a\leq x\leq b\}}][nb_1], a random variable      X  I
&#x223C; U &#x2061; ( I ) = U &#x2061; [ a , b ]   {\displaystyle X_{I}\sim
\operatorname {U} (I)=\operatorname {U} [a,b]}  [{\displaystyle X_{I}\sim
\operatorname {U} (I)=\operatorname {U} [a,b]}] called a "continuous_uniform
random variable" (CURV) is defined to take any value in the interval with equal
likelihood.[nb_2] The probability of      X  I     {\displaystyle X_{I}}  [X_
{I}] falling in any subinterval     [ c , d ] &#x2286; [ a , b ]
{\displaystyle [c,d]\subseteq [a,b]}  [{\displaystyle [c,d]\subseteq [a,b]}][nb
1] is proportional to the length of the subinterval, specifically
   c &#x2265; a &#xA0; &#x2227; &#xA0; d &#x2264; b  &#x27F9;  Pr  (   X  I
&#x2208; [ c , d ]  )  = Pr  (  c &#x2264;  X  I   &#x2264; d  )  =    d
&#x2212; c   b &#x2212; a      {\displaystyle c\geq a\ \wedge \ d\leq b\implies
\Pr \left(X_{I}\in [c,d]\right)=\Pr \left(c\leq X_{I}\leq d\right)={\frac {d-c}
{b-a}}}
[{\displaystyle c\geq a\ \wedge \ d\leq b\implies \Pr \left(X_{I}\in
[c,d]\right)=\Pr \left(c\leq X_{I}\leq d\right)={\frac {d-c}{b-a}}}]
where the denominator comes from the unitarity_axiom of probability. The
probability_density_function of a CURV     X &#x223C; U &#x2061; [ a , b ]
{\displaystyle X\sim \operatorname {U} [a,b]}  [{\displaystyle X\sim
\operatorname {U} [a,b]}] is given by the indicator_function of its interval of
support normalized by the interval's length:
    f  X   ( x ) =   {       1  b &#x2212; a    ,    a &#x2264; x &#x2264; b
0 ,    otherwise  .         {\displaystyle f_{X}(x)={\begin{cases}\displaystyle
{1 \over b-a},&a\leq x\leq b\\0,&{\text{otherwise}}.\end{cases}}}
[{\displaystyle f_{X}(x)={\begin{cases}\displaystyle {1 \over b-a},&a\leq x\leq
b\\0,&{\text{otherwise}}.\end{cases}}}]
Of particular interest is the uniform distribution on the unit_interval     [ 0
, 1 ]   {\displaystyle [0,1]}  [[0,1]]. Samples of any desired probability
distribution     D   {\displaystyle \operatorname {D} }  [{\displaystyle
\operatorname {D} }] can be generated by calculating the quantile_function of
D   {\displaystyle \operatorname {D} }  [{\displaystyle \operatorname {D} }] on
a randomly-generated_number distributed uniformly on the unit interval. This
exploits properties_of_cumulative_distribution_functions, which are a unifying
framework for all random variables.
**** Mixed type[edit] ****
A mixed random variable is a random variable whose cumulative_distribution
function is neither piecewise-constant (a discrete random variable) nor
everywhere-continuous.[5] It can be realized as the sum of a discrete random
variable and a continuous random variable; in which case the CDF will be the
weighted average of the CDFs of the component variables.[5]
An example of a random variable of mixed type would be based on an experiment
where a coin is flipped and the spinner is spun only if the result of the coin
toss is heads. If the result is tails, X = â1; otherwise X = the value of the
spinner as in the preceding example. There is a probability of &#x200b;1⁄2 that
this random variable will have the value â1. Other ranges of values would
have half the probabilities of the last example.
Most generally, every probability distribution on the real line is a mixture of
discrete part, singular part, and an absolutely continuous part; see Lebesgue's
decomposition_theorem_Â§ Refinement. The discrete part is concentrated on a
countable set, but this set may be dense (like the set of all rational
numbers).
***** Measure-theoretic definition[edit] *****
The most formal, axiomatic definition of a random variable involves measure
theory. Continuous random variables are defined in terms of sets of numbers,
along with functions that map such sets to probabilities. Because of various
difficulties (e.g. the BanachâTarski_paradox) that arise if such sets are
insufficiently constrained, it is necessary to introduce what is termed a
sigma-algebra to constrain the possible sets over which probabilities can be
defined. Normally, a particular such sigma-algebra is used, the Borel_Ï-
algebra, which allows for probabilities to be defined over any sets that can be
derived either directly from continuous intervals of numbers or by a finite or
countably_infinite number of unions and/or intersections of such intervals.[2]
The measure-theoretic definition is as follows.
Let     ( &#x03A9; ,   F   , P )   {\displaystyle (\Omega ,{\mathcal {F}},P)}
[(\Omega ,{\mathcal {F}},P)] be a probability_space and     ( E ,   E   )
{\displaystyle (E,{\mathcal {E}})}  [(E,{\mathcal {E}})] a measurable_space.
Then an    ( E ,   E   )   {\displaystyle (E,{\mathcal {E}})}  [(E,{\mathcal
{E}})]-valued random variable is a measurable function     X &#x003A; &#x03A9;
&#x2192; E   {\displaystyle X\colon \Omega \to E}  [X\colon \Omega \to E],
which means that, for every subset     B &#x2208;   E     {\displaystyle B\in
{\mathcal {E}}}  [B\in {\mathcal {E}}], its preimage      X  &#x2212; 1   ( B )
&#x2208;   F     {\displaystyle X^{-1}(B)\in {\mathcal {F}}}  [X^{-1}(B)\in
{\mathcal {F}}] where      X  &#x2212; 1   ( B ) = { &#x03C9; : X ( &#x03C9; )
&#x2208; B }   {\displaystyle X^{-1}(B)=\{\omega :X(\omega )\in B\}}  [X^{-1}
(B)=\{\omega :X(\omega )\in B\}].[6] This definition enables us to measure any
subset     B &#x2208;   E     {\displaystyle B\in {\mathcal {E}}}  [B\in
{\mathcal {E}}] in the target space by looking at its preimage, which by
assumption is measurable.
In more intuitive terms, a member of     &#x03A9;   {\displaystyle \Omega }
[\Omega ] is a possible outcome, a member of       F     {\displaystyle
{\mathcal {F}}}  [{\mathcal {F}}] is a measurable subset of possible outcomes,
the function     P   {\displaystyle P}  [P] gives the probability of each such
measurable subset,     E   {\displaystyle E}  [E] represents the set of values
that the random variable can take (such as the set of real numbers), and a
member of       E     {\displaystyle {\mathcal {E}}}  [{\mathcal {E}}] is a
"well-behaved" (measurable) subset of     E   {\displaystyle E}  [E] (those for
which the probability may be determined). The random variable is then a
function from any outcome to a quantity, such that the outcomes leading to any
useful subset of quantities for the random variable have a well-defined
probability.
When     E   {\displaystyle E}  [E] is a topological_space, then the most
common choice for the Ï-algebra       E     {\displaystyle {\mathcal {E}}}  [
{\mathcal {E}}] is the Borel_Ï-algebra       B   ( E )   {\displaystyle
{\mathcal {B}}(E)}  [{\mathcal {B}}(E)], which is the Ï-algebra generated by
the collection of all open sets in     E   {\displaystyle E}  [E]. In such case
the     ( E ,   E   )   {\displaystyle (E,{\mathcal {E}})}  [(E,{\mathcal
{E}})]-valued random variable is called the    E   {\displaystyle E}  [E]-
valued random variable. Moreover, when space     E   {\displaystyle E}  [E] is
the real line      R    {\displaystyle \mathbb {R} }  [\mathbb {R} ], then such
a real-valued random variable is called simply the random variable.
**** Real-valued random variables[edit] ****
In this case the observation space is the set of real numbers. Recall,
( &#x03A9; ,   F   , P )   {\displaystyle (\Omega ,{\mathcal {F}},P)}  [(\Omega
,{\mathcal {F}},P)] is the probability space. For real observation space, the
function     X &#x003A; &#x03A9; &#x2192;  R    {\displaystyle X\colon \Omega
\rightarrow \mathbb {R} }  [X\colon \Omega \rightarrow \mathbb {R} ] is a real-
valued random variable if
         { &#x03C9; : X ( &#x03C9; ) &#x2264; r } &#x2208;   F    &#x2200; r
      &#x2208;  R  .   {\displaystyle \{\omega :X(\omega )\leq r\}\in {\mathcal
      {F}}\qquad \forall r\in \mathbb {R} .}  [\{\omega :X(\omega )\leq r\}\in
      {\mathcal {F}}\qquad \forall r\in \mathbb {R} .]
This definition is a special case of the above because the set     { ( &#x2212;
&#x221E; , r ] : r &#x2208;  R  }   {\displaystyle \{(-\infty ,r]:r\in \mathbb
{R} \}}  [\{(-\infty ,r]:r\in \mathbb {R} \}] generates the Borel Ï-algebra on
the set of real numbers, and it suffices to check measurability on any
generating set. Here we can prove measurability on this generating set by using
the fact that     { &#x03C9; : X ( &#x03C9; ) &#x2264; r } =  X  &#x2212; 1
( ( &#x2212; &#x221E; , r ] )   {\displaystyle \{\omega :X(\omega )\leq r\}=X^
{-1}((-\infty ,r])}  [\{\omega :X(\omega )\leq r\}=X^{-1}((-\infty ,r])].
***** Moments[edit] *****
The probability distribution of a random variable is often characterised by a
small number of parameters, which also have a practical interpretation. For
example, it is often enough to know what its "average value" is. This is
captured by the mathematical concept of expected_value of a random variable,
denoted     E &#x2061; [ X ]   {\displaystyle \operatorname {E} [X]}
[\operatorname {E} [X]], and also called the first moment. In general,     E
&#x2061; [ f ( X ) ]   {\displaystyle \operatorname {E} [f(X)]}  [
{\displaystyle \operatorname {E} [f(X)]}] is not equal to     f ( E &#x2061;
[ X ] )   {\displaystyle f(\operatorname {E} [X])}  [{\displaystyle f
(\operatorname {E} [X])}]. Once the "average value" is known, one could then
ask how far from this average value the values of     X   {\displaystyle X}
[X] typically are, a question that is answered by the variance and standard
deviation of a random variable.     E &#x2061; [ X ]   {\displaystyle
\operatorname {E} [X]}  [\operatorname {E} [X]] can be viewed intuitively as an
average obtained from an infinite population, the members of which are
particular evaluations of     X   {\displaystyle X}  [X].
Mathematically, this is known as the (generalised) problem_of_moments: for a
given class of random variables     X   {\displaystyle X}  [X], find a
collection     {  f  i   }   {\displaystyle \{f_{i}\}}  [\{f_{i}\}] of
functions such that the expectation values     E &#x2061; [  f  i   ( X ) ]
{\displaystyle \operatorname {E} [f_{i}(X)]}  [{\displaystyle \operatorname {E}
[f_{i}(X)]}] fully characterise the distribution of the random variable     X
{\displaystyle X}  [X].
Moments can only be defined for real-valued functions of random variables (or
complex-valued, etc.). If the random variable is itself real-valued, then
moments of the variable itself can be taken, which are equivalent to moments of
the identity function     f ( X ) = X   {\displaystyle f(X)=X}  [f(X)=X] of the
random variable. However, even for non-real-valued random variables, moments
can be taken of real-valued functions of those variables. For example, for a
categorical random variable X that can take on the nominal values "red", "blue"
or "green", the real-valued function     [ X =  green  ]   {\displaystyle [X=
{\text{green}}]}  [[X={\text{green}}]] can be constructed; this uses the
Iverson_bracket, and has the value 1 if     X   {\displaystyle X}  [X] has the
value "green", 0 otherwise. Then, the expected_value and other moments of this
function can be determined.
***** Functions of random variables[edit] *****
A new random variable Y can be defined by applying a real Borel_measurable
function     g &#x003A;  R  &#x2192;  R    {\displaystyle g\colon \mathbb {R}
\rightarrow \mathbb {R} }  [g\colon \mathbb {R} \rightarrow \mathbb {R} ] to
the outcomes of a real-valued random variable     X   {\displaystyle X}  [X].
That is,     Y = g ( X )   {\displaystyle Y=g(X)}  [Y=g(X)]. The cumulative
distribution_function of     Y   {\displaystyle Y}  [Y] is then
          F  Y   ( y ) = P &#x2061; ( g ( X ) &#x2264; y ) .   {\displaystyle
      F_{Y}(y)=\operatorname {P} (g(X)\leq y).}  [F_{Y}(y)=\operatorname {P} (g
      (X)\leq y).]
If function     g   {\displaystyle g}  [g] is invertible (i.e.,     h =  g
&#x2212; 1     {\displaystyle h=g^{-1}}  [{\displaystyle h=g^{-1}}] exists,
where     h   {\displaystyle h}  [h] is     g   {\displaystyle g}  [g]'s
inverse_function) and is either increasing_or_decreasing, then the previous
relation can be extended to obtain
          F  Y   ( y ) = P &#x2061; ( g ( X ) &#x2264; y ) =   {    P &#x2061;
      ( X &#x2264; h ( y ) ) =  F  X   ( h ( y ) ) ,    if&#xA0;  h =  g
      &#x2212; 1    &#xA0;increasing  ,        P &#x2061; ( X &#x2265; h ( y )
      ) = 1 &#x2212;  F  X   ( h ( y ) ) ,    if&#xA0;  h =  g  &#x2212; 1
      &#xA0;decreasing  .         {\displaystyle F_{Y}(y)=\operatorname {P} (g
      (X)\leq y)={\begin{cases}\operatorname {P} (X\leq h(y))=F_{X}(h(y)),&
      {\text{if }}h=g^{-1}{\text{ increasing}},\\\\\operatorname {P} (X\geq h
      (y))=1-F_{X}(h(y)),&{\text{if }}h=g^{-1}{\text{ decreasing}}.\end
      {cases}}}  [{\displaystyle F_{Y}(y)=\operatorname {P} (g(X)\leq y)=
      {\begin{cases}\operatorname {P} (X\leq h(y))=F_{X}(h(y)),&{\text{if
      }}h=g^{-1}{\text{ increasing}},\\\\\operatorname {P} (X\geq h(y))=1-F_{X}
      (h(y)),&{\text{if }}h=g^{-1}{\text{ decreasing}}.\end{cases}}}]
With the same hypotheses of invertibility of     g   {\displaystyle g}  [g],
assuming also differentiability, the relation between the probability_density
functions can be found by differentiating both sides of the above expression
with respect to     y   {\displaystyle y}  [y], in order to obtain[5]
          f  Y   ( y ) =  f  X     (   h ( y )   )    |    d h ( y )   d y    |
      .   {\displaystyle f_{Y}(y)=f_{X}{\bigl (}h(y){\bigr )}\left|{\frac {dh
      (y)}{dy}}\right|.}  [{\displaystyle f_{Y}(y)=f_{X}{\bigl (}h(y){\bigr
      )}\left|{\frac {dh(y)}{dy}}\right|.}]
If there is no invertibility of     g   {\displaystyle g}  [g] but each     y
{\displaystyle y}  [y] admits at most a countable number of roots (i.e., a
finite, or countably infinite, number of      x  i     {\displaystyle x_{i}}
[x_{i}] such that     y = g (  x  i   )   {\displaystyle y=g(x_{i})}  [
{\displaystyle y=g(x_{i})}]) then the previous relation between the probability
density_functions can be generalized with
          f  Y   ( y ) =  &#x2211;  i    f  X   (  g  i   &#x2212; 1   ( y ) )
      |    d  g  i   &#x2212; 1   ( y )   d y    |    {\displaystyle f_{Y}
      (y)=\sum _{i}f_{X}(g_{i}^{-1}(y))\left|{\frac {dg_{i}^{-1}(y)}
      {dy}}\right|}  [f_{Y}(y)=\sum _{i}f_{X}(g_{i}^{-1}(y))\left|{\frac {dg_
      {i}^{-1}(y)}{dy}}\right|]
where      x  i   =  g  i   &#x2212; 1   ( y )   {\displaystyle x_{i}=g_{i}^{-
1}(y)}  [{\displaystyle x_{i}=g_{i}^{-1}(y)}], according to the inverse
function_theorem. The formulas for densities do not demand     g
{\displaystyle g}  [g] to be increasing.
In the measure-theoretic, axiomatic_approach to probability, if a random
variable     X   {\displaystyle X}  [X] on     &#x03A9;   {\displaystyle \Omega
}  [\Omega ] and a Borel_measurable_function     g &#x003A;  R  &#x2192;  R
{\displaystyle g\colon \mathbb {R} \rightarrow \mathbb {R} }  [g\colon \mathbb
{R} \rightarrow \mathbb {R} ], then     Y = g ( X )   {\displaystyle Y=g(X)}  [
{\displaystyle Y=g(X)}] is also a random variable on     &#x03A9;
{\displaystyle \Omega }  [\Omega ], since the composition of measurable
functions is_also_measurable. (However, this is not necessarily true if     g
{\displaystyle g}  [g] is Lebesgue_measurable.[citation_needed]) The same
procedure that allowed one to go from a probability space     ( &#x03A9; , P )
{\displaystyle (\Omega ,P)}  [{\displaystyle (\Omega ,P)}] to     (  R  , d  F
X   )   {\displaystyle (\mathbb {R} ,dF_{X})}  [(\mathbb {R} ,dF_{X})] can be
used to obtain the distribution of     Y   {\displaystyle Y}  [Y].
**** Example 1[edit] ****
Let     X   {\displaystyle X}  [X] be a real-valued, continuous_random_variable
and let     Y =  X  2     {\displaystyle Y=X^{2}}  [{\displaystyle Y=X^{2}}].
          F  Y   ( y ) = P &#x2061; (  X  2   &#x2264; y ) .   {\displaystyle
      F_{Y}(y)=\operatorname {P} (X^{2}\leq y).}  [F_{Y}(y)=\operatorname {P}
      (X^{2}\leq y).]
If     y < 0   {\displaystyle y<0}  [{\displaystyle y<0}], then     P (  X  2
&#x2264; y ) = 0   {\displaystyle P(X^{2}\leq y)=0}  [{\displaystyle P(X^
{2}\leq y)=0}], so
          F  Y   ( y ) = 0    if    y < 0.   {\displaystyle F_{Y}(y)=0\qquad
      {\hbox{if}}\quad y<0.}  [F_{Y}(y)=0\qquad {\hbox{if}}\quad y<0.]
If     y &#x2265; 0   {\displaystyle y\geq 0}  [{\displaystyle y\geq 0}], then
         P &#x2061; (  X  2   &#x2264; y ) = P &#x2061; (  |  X  |  &#x2264;
      y   ) = P &#x2061; ( &#x2212;   y   &#x2264; X &#x2264;   y   ) ,
      {\displaystyle \operatorname {P} (X^{2}\leq y)=\operatorname {P} (|X|\leq
      {\sqrt {y}})=\operatorname {P} (-{\sqrt {y}}\leq X\leq {\sqrt {y}}),}
      [\operatorname {P} (X^{2}\leq y)=\operatorname {P} (|X|\leq {\sqrt
      {y}})=\operatorname {P} (-{\sqrt {y}}\leq X\leq {\sqrt {y}}),]
so
          F  Y   ( y ) =  F  X   (   y   ) &#x2212;  F  X   ( &#x2212;   y   )
      if    y &#x2265; 0.   {\displaystyle F_{Y}(y)=F_{X}({\sqrt {y}})-F_{X}(-
      {\sqrt {y}})\qquad {\hbox{if}}\quad y\geq 0.}  [F_{Y}(y)=F_{X}({\sqrt
      {y}})-F_{X}(-{\sqrt {y}})\qquad {\hbox{if}}\quad y\geq 0.]
**** Example 2[edit] ****
Suppose     X   {\displaystyle X}  [X] is a random variable with a cumulative
distribution
          F  X   ( x ) = P ( X &#x2264; x ) =   1  ( 1 +  e  &#x2212; x    )
      &#x03B8;        {\displaystyle F_{X}(x)=P(X\leq x)={\frac {1}{(1+e^{-x})^
      {\theta }}}}  [F_{X}(x)=P(X\leq x)={\frac {1}{(1+e^{-x})^{\theta }}}]
where     &#x03B8; > 0   {\displaystyle \theta >0}  [\theta >0] is a fixed
parameter. Consider the random variable     Y =  l o g  ( 1 +  e  &#x2212; X
) .   {\displaystyle Y=\mathrm {log} (1+e^{-X}).}  [{\displaystyle Y=\mathrm
{log} (1+e^{-X}).}] Then,
          F  Y   ( y ) = P ( Y &#x2264; y ) = P (  l o g  ( 1 +  e  &#x2212; X
      ) &#x2264; y ) = P ( X &#x2265; &#x2212;  l o g  (  e  y   &#x2212; 1 ) )
      .    {\displaystyle F_{Y}(y)=P(Y\leq y)=P(\mathrm {log} (1+e^{-X})\leq
      y)=P(X\geq -\mathrm {log} (e^{y}-1)).\,}  [{\displaystyle F_{Y}(y)=P
      (Y\leq y)=P(\mathrm {log} (1+e^{-X})\leq y)=P(X\geq -\mathrm {log} (e^
      {y}-1)).\,}]
The last expression can be calculated in terms of the cumulative distribution
of     X ,   {\displaystyle X,}  [X,] so
              F  Y   ( y )    = 1 &#x2212;  F  X   ( &#x2212; log &#x2061; (  e
      y   &#x2212; 1 ) )       = 1 &#x2212;   1  ( 1 +  e  log &#x2061; (  e  y
      &#x2212; 1 )    )  &#x03B8;            = 1 &#x2212;   1  ( 1 +  e  y
      &#x2212; 1  )  &#x03B8;            = 1 &#x2212;  e  &#x2212; y &#x03B8;
      .       {\displaystyle {\begin{aligned}F_{Y}(y)&=1-F_{X}(-\log(e^{y}-
      1))\\[5pt]&=1-{\frac {1}{(1+e^{\log(e^{y}-1)})^{\theta }}}\\[5pt]&=1-
      {\frac {1}{(1+e^{y}-1)^{\theta }}}\\[5pt]&=1-e^{-y\theta }.\end
      {aligned}}}  [{\displaystyle {\begin{aligned}F_{Y}(y)&=1-F_{X}(-\log(e^
      {y}-1))\\[5pt]&=1-{\frac {1}{(1+e^{\log(e^{y}-1)})^{\theta }}}\\[5pt]&=1-
      {\frac {1}{(1+e^{y}-1)^{\theta }}}\\[5pt]&=1-e^{-y\theta }.\end
      {aligned}}}]
which is the cumulative_distribution_function (CDF) of an exponential
distribution.
**** Example 3[edit] ****
Suppose     X   {\displaystyle X}  [X] is a random variable with a standard
normal_distribution, whose density is
          f  X   ( x ) =   1  2 &#x03C0;     e  &#x2212;  x  2    /  2   .
      {\displaystyle f_{X}(x)={\frac {1}{\sqrt {2\pi }}}e^{-x^{2}/2}.}  [f_{X}
      (x)={\frac {1}{\sqrt {2\pi }}}e^{-x^{2}/2}.]
Consider the random variable     Y =  X  2   .   {\displaystyle Y=X^{2}.}  [
{\displaystyle Y=X^{2}.}] We can find the density using the above formula for a
change of variables:
          f  Y   ( y ) =  &#x2211;  i    f  X   (  g  i   &#x2212; 1   ( y ) )
      |    d  g  i   &#x2212; 1   ( y )   d y    |  .   {\displaystyle f_{Y}
      (y)=\sum _{i}f_{X}(g_{i}^{-1}(y))\left|{\frac {dg_{i}^{-1}(y)}
      {dy}}\right|.}  [f_{Y}(y)=\sum _{i}f_{X}(g_{i}^{-1}(y))\left|{\frac {dg_
      {i}^{-1}(y)}{dy}}\right|.]
In this case the change is not monotonic, because every value of     Y
{\displaystyle Y}  [Y] has two corresponding values of     X   {\displaystyle
X}  [X] (one positive and negative). However, because of symmetry, both halves
will transform identically, i.e.,
          f  Y   ( y ) = 2  f  X   (  g  &#x2212; 1   ( y ) )  |    d  g
      &#x2212; 1   ( y )   d y    |  .   {\displaystyle f_{Y}(y)=2f_{X}(g^{-1}
      (y))\left|{\frac {dg^{-1}(y)}{dy}}\right|.}  [f_{Y}(y)=2f_{X}(g^{-1}
      (y))\left|{\frac {dg^{-1}(y)}{dy}}\right|.]
The inverse transformation is
         x =  g  &#x2212; 1   ( y ) =   y     {\displaystyle x=g^{-1}(y)={\sqrt
      {y}}}  [x=g^{-1}(y)={\sqrt {y}}]
and its derivative is
            d  g  &#x2212; 1   ( y )   d y    =   1  2   y      .
      {\displaystyle {\frac {dg^{-1}(y)}{dy}}={\frac {1}{2{\sqrt {y}}}}.}  [
      {\frac {dg^{-1}(y)}{dy}}={\frac {1}{2{\sqrt {y}}}}.]
Then,
          f  Y   ( y ) = 2   1  2 &#x03C0;     e  &#x2212; y  /  2     1  2   y
      =   1  2 &#x03C0; y     e  &#x2212; y  /  2   .   {\displaystyle f_{Y}
      (y)=2{\frac {1}{\sqrt {2\pi }}}e^{-y/2}{\frac {1}{2{\sqrt {y}}}}={\frac
      {1}{\sqrt {2\pi y}}}e^{-y/2}.}  [f_{Y}(y)=2{\frac {1}{\sqrt {2\pi }}}e^{-
      y/2}{\frac {1}{2{\sqrt {y}}}}={\frac {1}{\sqrt {2\pi y}}}e^{-y/2}.]
This is a chi-squared_distribution with one degree_of_freedom.
**** Example 4[edit] ****
Suppose     X   {\displaystyle X}  [X] is a random variable with a normal
distribution, whose density is
          f  X   ( x ) =   1  2 &#x03C0;  &#x03C3;  2       e  &#x2212; ( x
      &#x2212; &#x03BC;  )  2    /  ( 2  &#x03C3;  2   )   .   {\displaystyle
      f_{X}(x)={\frac {1}{\sqrt {2\pi \sigma ^{2}}}}e^{-(x-\mu )^{2}/(2\sigma ^
      {2})}.}  [{\displaystyle f_{X}(x)={\frac {1}{\sqrt {2\pi \sigma ^{2}}}}e^
      {-(x-\mu )^{2}/(2\sigma ^{2})}.}]
Consider the random variable     Y =  X  2   .   {\displaystyle Y=X^{2}.}  [
{\displaystyle Y=X^{2}.}] We can find the density using the above formula for a
change of variables:
          f  Y   ( y ) =  &#x2211;  i    f  X   (  g  i   &#x2212; 1   ( y ) )
      |    d  g  i   &#x2212; 1   ( y )   d y    |  .   {\displaystyle f_{Y}
      (y)=\sum _{i}f_{X}(g_{i}^{-1}(y))\left|{\frac {dg_{i}^{-1}(y)}
      {dy}}\right|.}  [f_{Y}(y)=\sum _{i}f_{X}(g_{i}^{-1}(y))\left|{\frac {dg_
      {i}^{-1}(y)}{dy}}\right|.]
In this case the change is not monotonic, because every value of     Y
{\displaystyle Y}  [Y] has two corresponding values of     X   {\displaystyle
X}  [X] (one positive and negative). Differently from the previous example, in
this case however, there is no symmetry and we have to compute the two distinct
terms:
          f  Y   ( y ) =  f  X   (  g  1   &#x2212; 1   ( y ) )  |    d  g  1
      &#x2212; 1   ( y )   d y    |  +  f  X   (  g  2   &#x2212; 1   ( y ) )
      |    d  g  2   &#x2212; 1   ( y )   d y    |  .   {\displaystyle f_{Y}
      (y)=f_{X}(g_{1}^{-1}(y))\left|{\frac {dg_{1}^{-1}(y)}{dy}}\right|+f_{X}
      (g_{2}^{-1}(y))\left|{\frac {dg_{2}^{-1}(y)}{dy}}\right|.}  [
      {\displaystyle f_{Y}(y)=f_{X}(g_{1}^{-1}(y))\left|{\frac {dg_{1}^{-1}(y)}
      {dy}}\right|+f_{X}(g_{2}^{-1}(y))\left|{\frac {dg_{2}^{-1}(y)}
      {dy}}\right|.}]
The inverse transformation is
         x =  g  1 , 2   &#x2212; 1   ( y ) = &#x00B1;   y     {\displaystyle
      x=g_{1,2}^{-1}(y)=\pm {\sqrt {y}}}  [{\displaystyle x=g_{1,2}^{-1}(y)=\pm
      {\sqrt {y}}}]
and its derivative is
            d  g  1 , 2   &#x2212; 1   ( y )   d y    = &#x00B1;   1  2   y
      .   {\displaystyle {\frac {dg_{1,2}^{-1}(y)}{dy}}=\pm {\frac {1}{2{\sqrt
      {y}}}}.}  [{\displaystyle {\frac {dg_{1,2}^{-1}(y)}{dy}}=\pm {\frac {1}{2
      {\sqrt {y}}}}.}]
Then,
          f  Y   ( y ) =   1  2 &#x03C0;  &#x03C3;  2        1  2   y      (  e
      &#x2212; (   y   &#x2212; &#x03BC;  )  2    /  ( 2  &#x03C3;  2   )   +
      e  &#x2212; ( &#x2212;   y   &#x2212; &#x03BC;  )  2    /  ( 2  &#x03C3;
      2   )   ) .   {\displaystyle f_{Y}(y)={\frac {1}{\sqrt {2\pi \sigma ^
      {2}}}}{\frac {1}{2{\sqrt {y}}}}(e^{-({\sqrt {y}}-\mu )^{2}/(2\sigma ^
      {2})}+e^{-(-{\sqrt {y}}-\mu )^{2}/(2\sigma ^{2})}).}  [{\displaystyle f_
      {Y}(y)={\frac {1}{\sqrt {2\pi \sigma ^{2}}}}{\frac {1}{2{\sqrt {y}}}}(e^
      {-({\sqrt {y}}-\mu )^{2}/(2\sigma ^{2})}+e^{-(-{\sqrt {y}}-\mu )^{2}/
      (2\sigma ^{2})}).}]
This is a noncentral_chi-squared_distribution with one degree_of_freedom.
***** Equivalence of random variables[edit] *****
There are several different senses in which random variables can be considered
to be equivalent. Two random variables can be equal, equal almost surely, or
equal in distribution.
In increasing order of strength, the precise definition of these notions of
equivalence is given below.
**** Equality in distribution[edit] ****
If the sample space is a subset of the real line, random variables X and Y are
equal in distribution (denoted     X     =   d     Y   {\displaystyle X
{\stackrel {d}{=}}Y}  [X{\stackrel {d}{=}}Y]) if they have the same
distribution functions:
         P &#x2061; ( X &#x2264; x ) = P &#x2061; ( Y &#x2264; x )    for all
      x .   {\displaystyle \operatorname {P} (X\leq x)=\operatorname {P} (Y\leq
      x)\quad {\hbox{for all}}\quad x.}  [\operatorname {P} (X\leq
      x)=\operatorname {P} (Y\leq x)\quad {\hbox{for all}}\quad x.]
To be equal in distribution, random variables need not be defined on the same
probability space. Two random variables having equal moment_generating
functions have the same distribution. This provides, for example, a useful
method of checking equality of certain functions of independent,_identically
distributed_(IID)_random_variables. However, the moment generating function
exists only for distributions that have a defined Laplace_transform.
**** Almost sure equality[edit] ****
Two random variables X and Y are equal almost_surely (denoted     X      =
a.s.      Y   {\displaystyle X\;{\stackrel {\text{a.s.}}{=}}\;Y}  [
{\displaystyle X\;{\stackrel {\text{a.s.}}{=}}\;Y}]) if, and only if, the
probability that they are different is zero:
         P &#x2061; ( X &#x2260; Y ) = 0.   {\displaystyle \operatorname {P}
      (X\neq Y)=0.}  [\operatorname {P} (X\neq Y)=0.]
For all practical purposes in probability theory, this notion of equivalence is
as strong as actual equality. It is associated to the following distance:
          d  &#x221E;   ( X , Y ) = ess &#x2061;  sup  &#x03C9;    |  X
      ( &#x03C9; ) &#x2212; Y ( &#x03C9; )  |  ,   {\displaystyle d_{\infty }
      (X,Y)=\operatorname {ess} \sup _{\omega }|X(\omega )-Y(\omega )|,}  [
      {\displaystyle d_{\infty }(X,Y)=\operatorname {ess} \sup _{\omega }|X
      (\omega )-Y(\omega )|,}]
where "ess sup" represents the essential_supremum in the sense of measure
theory.
**** Equality[edit] ****
Finally, the two random variables X and Y are equal if they are equal as
functions on their measurable space:
         X ( &#x03C9; ) = Y ( &#x03C9; )    for all&#xA0;   &#x03C9; .
      {\displaystyle X(\omega )=Y(\omega )\qquad {\hbox{for all }}\omega .}  [X
      (\omega )=Y(\omega )\qquad {\hbox{for all }}\omega .]
This notion is typically the least useful in probability theory because in
practice and in theory, the underlying measure_space of the experiment is
rarely explicitly characterized or even characterizable.
***** Convergence[edit] *****
Main article: Convergence_of_random_variables
A significant theme in mathematical statistics consists of obtaining
convergence results for certain sequences of random variables; for instance the
law_of_large_numbers and the central_limit_theorem.
There are various senses in which a sequence      X  n     {\displaystyle X_
{n}}  [X_{n}] of random variables can converge to a random variable     X
{\displaystyle X}  [X]. These are explained in the article on convergence_of
random_variables.
***** Notes[edit] *****
   1. ^ a b The interval I can be closed (of the form     I =  [  a , b  ]
      {\textstyle I=\left[a,b\right]}  [{\textstyle I=\left[a,b\right]}]), open
      (    I =  (  a , b  )    {\displaystyle I=\left(a,b\right)}  [
      {\displaystyle I=\left(a,b\right)}]) or clopen (of the form     I =  (  a
      , b  ]    {\displaystyle I=\left(a,b\right]}  [{\displaystyle I=\left
      (a,b\right]}] or     I =  [  a , b  )    {\textstyle I=\left[a,b\right)}
      [{\textstyle I=\left[a,b\right)}]). The singleton sets     { a }
      {\displaystyle \{a\}}  [\{a\}] and     { b }   {\displaystyle \{b\}}  [\
      {b\}] have measure_zero and so are equivalent from the perspective of the
      Lebesgue_measure     &#x03BC;   {\displaystyle \mu }  [\mu ] and measures
      absolutely_continuous with respect to it.
   2. ^ Formally, given any subsets     S , T &#x2286; I   {\displaystyle
      S,T\subseteq I}  [{\displaystyle S,T\subseteq I}] of equal Lebesgue
      measure, the probabilities that X is contained_in     S   {\displaystyle
      S}  [S] and     T   {\displaystyle T}  [T] are equal:     Pr  (  X
      &#x2208; S  )  = Pr  (  X &#x2208; T  )    {\displaystyle \Pr \left(X\in
      S\right)=\Pr \left(X\in T\right)}  [{\displaystyle \Pr \left(X\in
      S\right)=\Pr \left(X\in T\right)}].
***** See also[edit] *****
    * [icon]Statistics_portal
    * Aleatoricism
    * Algebra_of_random_variables
    * Event_(probability_theory)
    * Multivariate_random_variable
    * Observable_variable
    * Probability_distribution
    * Random_element
    * Random_function
    * Random_measure
    * Random_number_generator produces a random value
    * Random_vector
    * Randomness
    * Stochastic_process
    * Relationships_among_probability_distributions
***** References[edit] *****
   1. ^Blitzstein, Joe; Hwang, Jessica (2014). Introduction to Probability. CRC
      Press. ISBN 9781466575592.
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
   3. ^ a bSteigerwald, Douglas G. "Economics_245A_â_Introduction_to_Measure
      Theory" (PDF). University of California, Santa Barbara. Retrieved April
      26, 2013.
   4. ^ a bYates, Daniel S.; Moore, David S; Starnes, Daren S. (2003). The
      Practice_of_Statistics (2nd ed.). New York: Freeman. ISBN 978-0-7167-
      4773-4. Archived from the_original on 2005-02-09.
   5. ^L. CastaÃ±eda; V. Arunachalam & S. Dharmaraja (2012). Introduction_to
      Probability_and_Stochastic_Processes_with_Applications. Wiley. p. 67.
   6. ^ a b c dBertsekas, Dimitri P. (2002). Introduction_to_Probability.
      Tsitsiklis, John N., Î¤ÏÎ¹ÏÏÎ¹ÎºÎ»Î®Ï, ÎÎ¹Î¬Î½Î½Î·Ï Î. Belmont,
      Mass.: Athena Scientific. ISBN 188652940X. OCLC 51441829.
   7. ^ Fristedt_&_Gray_(1996, page 11)
**** Literature[edit] ****
    * Fristedt, Bert; Gray, Lawrence (1996). A_modern_approach_to_probability
      theory. Boston: BirkhÃ¤user. ISBN 3-7643-3807-5.
Kallenberg,_Olav (1986). Random_Measures (4th ed.). Berlin: Akademie_Verlag.
ISBN 0-12-394960-2. MR 0854102.
Kallenberg, Olav (2001). Foundations_of_Modern_Probability (2nd ed.). Berlin:
Springer_Verlag. ISBN 0-387-95313-2.
Papoulis,_Athanasios (1965). Probability,_Random_Variables,_and_Stochastic
Processes (9th ed.). Tokyo: McGrawâHill. ISBN 0-07-119981-0.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Random_variable", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Zukerman, Moshe (2014), Introduction_to_Queueing_Theory_and_Stochastic
Teletraffic_Models (PDF)
Zukerman, Moshe (2014), Basic_Probability_Topics (PDF)
    * v
    * t
    * e
Statistics
    * Outline
    * Index
Descriptive_statistics
                               * Mean
                                     o arithmetic
                Center               o geometric
                                     o harmonic
                               * Median
                               * Mode
                               * Variance
                               * Standard_deviation
Continuous_data Dispersion     * Coefficient_of_variation
                               * Percentile
                               * Range
                               * Interquartile_range
                               * Central_limit_theorem
                               * Moments
                Shape                o Skewness
                                     o Kurtosis
                                     o L-moments
Count_data          * Index_of_dispersion
                    * Grouped_data
Summary tables      * Frequency_distribution
                    * Contingency_table
                    * Pearson_product-moment_correlation
                    * Rank_correlation
Dependence                o Spearman's_rho
                          o Kendall's_tau
                    * Partial_correlation
                    * Scatter_plot
                    * Bar_chart
                    * Biplot
                    * Box_plot
                    * Control_chart
                    * Correlogram
                    * Fan_chart
Graphics            * Forest_plot
                    * Histogram
                    * Pie_chart
                    * QâQ_plot
                    * Run_chart
                    * Scatter_plot
                    * Stem-and-leaf_display
                    * Radar_chart
Data_collection
                           * Population
                           * Statistic
                           * Effect_size
Study_design               * Statistical_power
                           * Optimal_design
                           * Sample_size_determination
                           * Replication
                           * Missing_data
                           * Sampling
                                 o stratified
Survey_methodology               o cluster
                           * Standard_error
                           * Opinion_poll
                           * Questionnaire
                           * Scientific_control
                           * Randomized_experiment
                           * Randomized_controlled_trial
Controlled_experiments     * Random_assignment
                           * Blocking
                           * Interaction
                           * Factorial_experiment
                           * Adaptive_clinical_trial
Adaptive Designs           * Up-and-Down_Designs
                           * Stochastic_approximation
                           * Cross-sectional_study
Observational_Studies      * Cohort_study
                           * Natural_experiment
                           * Quasi-experiment
Statistical_inference
                * Population
                * Statistic
                * Probability_distribution
                * Sampling_distribution
                      o Order_statistic
                * Empirical_distribution
                      o Density_estimation
                * Statistical_model
                      o Model_specification
                      o Lp_space
                * Parameter
                      o location
                      o scale
                      o shape
Statistical     * Parametric_family
theory                o Likelihood (monotone)
                      o Locationâscale_family
                      o Exponential_family
                * Completeness
                * Sufficiency
                * Statistical_functional
                      o Bootstrap
                      o U
                      o V
                * Optimal_decision
                      o loss_function
                * Efficiency
                * Statistical_distance
                      o divergence
                * Asymptotics
                * Robustness
                                    * Estimating_equations
                                          o Maximum_likelihood
                                          o Method_of_moments
                                          o M-estimator
                                          o Minimum_distance
            Point_estimation        * Unbiased_estimators
                                          o Mean-unbiased_minimum-variance
                                                # RaoâBlackwellization
                                                # LehmannâScheffÃ©_theorem
                                          o Median_unbiased
                                    * Plug-in
                                    * Confidence_interval
                                    * Pivot
Frequentist                         * Likelihood_interval
inference   Interval_estimation     * Prediction_interval
                                    * Tolerance_interval
                                    * Resampling
                                          o Bootstrap
                                          o Jackknife
                                    * 1-_&_2-tails
                                    * Power
            Testing_hypotheses            o Uniformly_most_powerful_test
                                    * Permutation_test
                                          o Randomization_test
                                    * Multiple_comparisons
                                    * Likelihood-ratio
            Parametric_tests        * Score/Lagrange_multiplier
                                    * Wald
                * Z-test_(normal)
                * Student's_t-test
                * F-test
                           * Chi-squared
                           * G-test
                           * KolmogorovâSmirnov
                           * AndersonâDarling
                           * Lilliefors
            Goodness       * JarqueâBera
            of_fit         * Normality_(ShapiroâWilk)
                           * Likelihood-ratio_test
Specific                   * Model_selection
tests                            o Cross_validation
                                 o AIC
                                 o BIC
                           * Sign
                                 o Sample_median
                           * Signed_rank_(Wilcoxon)
            Rank                 o HodgesâLehmann_estimator
            statistics     * Rank_sum_(MannâWhitney)
                           * Nonparametric anova
                                 o 1-way_(KruskalâWallis)
                                 o 2-way_(Friedman)
                                 o Ordered_alternative_(JonckheereâTerpstra)
                * Bayesian_probability
                      o prior
Bayesian              o posterior
inference       * Credible_interval
                * Bayes_factor
                * Bayesian_estimator
                      o Maximum_posterior_estimator
    * Correlation
    * Regression_analysis
                       * Pearson_product-moment
Correlation            * Partial_correlation
                       * Confounding_variable
                       * Coefficient_of_determination
                       * Errors_and_residuals
Regression             * Regression_validation
analysis               * Mixed_effects_models
                       * Simultaneous_equations_models
                       * Multivariate_adaptive_regression_splines_(MARS)
                       * Simple_linear_regression
Linear_regression      * Ordinary_least_squares
                       * General_linear_model
                       * Bayesian_regression
                       * Nonlinear_regression
                       * Nonparametric
Non-standard           * Semiparametric
predictors             * Isotonic
                       * Robust
                       * Heteroscedasticity
                       * Homoscedasticity
Generalized_linear     * Exponential_families
model                  * Logistic_(Bernoulli) / Binomial / Poisson_regressions
                       * Analysis_of_variance_(ANOVA,_anova)
Partition_of           * Analysis_of_covariance
variance               * Multivariate_ANOVA
                       * Degrees_of_freedom
Categorical / Multivariate / Time-series / Survival_analysis
                 * Cohen's_kappa
                 * Contingency_table
Categorical      * Graphical_model
                 * Log-linear_model
                 * McNemar's_test
                 * Regression
                 * Manova
                 * Principal_components
                 * Canonical_correlation
                 * Discriminant_analysis
Multivariate     * Cluster_analysis
                 * Classification
                 * Structural_equation_model
                       o Factor_analysis
                 * Multivariate_distributions
                       o Elliptical_distributions
                             # Normal
                                  * Decomposition
                                  * Trend
                                  * Stationarity
             General              * Seasonal_adjustment
                                  * Exponential_smoothing
                                  * Cointegration
                                  * Structural_break
                                  * Granger_causality
                                  * DickeyâFuller
                                  * Johansen
             Specific tests       * Q-statistic_(LjungâBox)
                                  * DurbinâWatson
Time-series                       * BreuschâGodfrey
                                  * Autocorrelation_(ACF)
                                        o partial_(PACF)
                                  * Cross-correlation_(XCF)
             Time_domain          * ARMA_model
                                  * ARIMA_model_(BoxâJenkins)
                                  * Autoregressive_conditional
                                    heteroskedasticity_(ARCH)
                                  * Vector_autoregression_(VAR)
                                  * Spectral_density_estimation
             Frequency_domain     * Fourier_analysis
                                  * Wavelet
                                  * Whittle_likelihood
                                   * KaplanâMeier_estimator_(product_limit)
             Survival_function     * Proportional_hazards_models
Survival                           * Accelerated_failure_time_(AFT)_model
                                   * First_hitting_time
             Hazard_function       * NelsonâAalen_estimator
             Test                  * Log-rank_test
Applications
                           * Bioinformatics
Biostatistics              * Clinical_trials / studies
                           * Epidemiology
                           * Medical_statistics
                           * Chemometrics
                           * Methods_engineering
Engineering_statistics     * Probabilistic_design
                           * Process / quality_control
                           * Reliability
                           * System_identification
                           * Actuarial_science
                           * Census
                           * Crime_statistics
                           * Demography
Social_statistics          * Econometrics
                           * National_accounts
                           * Official_statistics
                           * Population_statistics
                           * Psychometrics
                           * Cartography
                           * Environmental_statistics
Spatial_statistics         * Geographic_information_system
                           * Geostatistics
                           * Kriging
    * [Category]Category
    * [Portal]Portal
    * [Commons page]Commons
    * [WikiProject] WikiProject

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Random_variable&oldid=908123851"
Categories:
    * Statistical_randomness
Hidden categories:
    * Articles_lacking_in-text_citations_from_February_2012
    * All_articles_lacking_in-text_citations
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_October_2018
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
    * AzÉrbaycanca
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Sicilianu
    * Simple_English
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Basa_Sunda
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * à°¤à±à°²à±à°à±
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 27 July 2019, at 16:17 (UTC).
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
