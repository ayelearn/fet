The following text has been accessed from https://en.wikipedia.org/wiki/Probability_distribution#Continuous_probability_distribution at Thu Aug 8 23:42:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Probability distribution ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about probability distributions. For generalized functions in
mathematical analysis, see Distribution_(mathematics). For continuous variation
in biology, see Genetic_variability. For other uses, see Distribution.
 This article has multiple issues. Please help improve_it or discuss these issues on the talk_page. (Learn
 how_and_when_to_remove_these_template_messages)
  This article includes a list_of_references, but its sources remain unclear because it has insufficient
  inline_citations. Please help to improve this article by introducing more precise citations. (July 2011)
  (Learn_how_and_when_to_remove_this_template_message)
  This article needs additional citations for verification. Please help improve_this_article by adding_citations_to_reliable
  sources. Unsourced material may be challenged and removed.
  Find sources: "Probability_distribution" â news Â· newspapers Â· books Â· scholar Â· JSTOR (July 2011)(Learn_how_and
  when_to_remove_this_template_message)
 (Learn_how_and_when_to_remove_this_template_message)
In probability_theory and statistics, a probability distribution is a
mathematical function that provides the probabilities of occurrence of
different possible outcomes in an experiment. In more technical terms, the
probability distribution is a description of a random phenomenon in terms of
the probabilities of events. For instance, if the random_variable X is used to
denote the outcome of a coin toss ("the experiment"), then the probability
distribution of X would take the value 0.5 for X = heads, and 0.5 for X = tails
(assuming the coin is fair). Examples of random phenomena can include the
results of an experiment or survey.
A probability distribution is specified in terms of an underlying sample_space,
which is the set of all possible outcomes of the random phenomenon being
observed. The sample space may be the set of real_numbers or a set of vectors,
or it may be a list of non-numerical values; for example, the sample space of a
coin flip would be {heads, tails} .
Probability distributions are generally divided into two classes. A discrete
probability distribution (applicable to the scenarios where the set of possible
outcomes is discrete, such as a coin toss or a roll of dice) can be encoded by
a discrete list of the probabilities of the outcomes, known as a probability
mass_function. On the other hand, a continuous probability distribution
(applicable to the scenarios where the set of possible outcomes can take on
values in a continuous range (e.g. real numbers), such as the temperature on a
given day) is typically described by probability_density_functions (with the
probability of any individual outcome actually being 0). The normal
distribution is a commonly encountered continuous probability distribution.
More complex experiments, such as those involving stochastic_processes defined
in continuous_time, may demand the use of more general probability_measures.
A probability distribution whose sample space is one-dimensional (for example
real numbers, list of labels, ordered labels or binary) is called univariate,
while a distribution whose sample space is a vector_space of dimension 2 or
more is called multivariate. A univariate distribution gives the probabilities
of a single random_variable taking on various alternative values; a
multivariate distribution (a joint_probability_distribution) gives the
probabilities of a random_vector â a list of two or more random variables â
taking on various combinations of values. Important and commonly encountered
univariate probability distributions include the binomial_distribution, the
hypergeometric_distribution, and the normal_distribution. The multivariate
normal_distribution is a commonly encountered multivariate distribution.
⁰
***** Contents *****
    * 1_Introduction
    * 2_Terminology
          o 2.1_Basic_terms
    * 3_Cumulative_distribution_function
    * 4_Discrete_probability_distribution
          o 4.1_Measure_theoretic_formulation
          o 4.2_Cumulative_distribution_function
          o 4.3_Delta-function_representation
          o 4.4_Indicator-function_representation
    * 5_Continuous_probability_distribution
    * 6_Some_properties
    * 7_Kolmogorov_definition
    * 8_Random_number_generation
    * 9_Applications
    * 10_Common_probability_distributions
          o 10.1_Related_to_real-valued_quantities_that_grow_linearly_(e.g.
            errors,_offsets)
          o 10.2_Related_to_positive_real-valued_quantities_that_grow
            exponentially_(e.g._prices,_incomes,_populations)
          o 10.3_Related_to_real-valued_quantities_that_are_assumed_to_be
            uniformly_distributed_over_a_(possibly_unknown)_region
          o 10.4_Related_to_Bernoulli_trials_(yes/no_events,_with_a_given
            probability)
          o 10.5_Related_to_categorical_outcomes_(events_with_K_possible
            outcomes,_with_a_given_probability_for_each_outcome)
          o 10.6_Related_to_events_in_a_Poisson_process_(events_that_occur
            independently_with_a_given_rate)
          o 10.7_Related_to_the_absolute_values_of_vectors_with_normally
            distributed_components
          o 10.8_Related_to_normally_distributed_quantities_operated_with_sum
            of_squares_(for_hypothesis_testing)
          o 10.9_Useful_as_conjugate_prior_distributions_in_Bayesian_inference
    * 11_See_also
    * 12_References
          o 12.1_Citations
          o 12.2_Sources
    * 13_External_links
***** Introduction[edit] *****
The probability_mass_function (pmf) p(S) specifies the probability distribution
for the sum S of counts from two dice. For example, the figure shows that p(11)
= 2/36 = 1/18. The pmf allows the computation of probabilities of events such
as P(S > 9) = 1/12 + 1/18 + 1/36 = 1/6, and all other probabilities in the
distribution.
To define probability distributions for the simplest cases, it is necessary to
distinguish between discrete and continuous random_variables. In the discrete
case, it is sufficient to specify a probability_mass_function     p
{\displaystyle p}  [p] assigning a probability to each possible outcome: for
example, when throwing a fair dice, each of the six values 1 to 6 has the
probability 1/6. The probability of an event is then defined to be the sum of
the probabilities of the outcomes that satisfy the event; for example, the
probability of the event "the dice rolls an even value" is
         p ( 2 ) + p ( 4 ) + p ( 6 ) = 1  /  6 + 1  /  6 + 1  /  6 = 1  /  2.
      {\displaystyle p(2)+p(4)+p(6)=1/6+1/6+1/6=1/2.}  [{\displaystyle p(2)+p
      (4)+p(6)=1/6+1/6+1/6=1/2.}]
In contrast, when a random variable takes values from a continuum then
typically, any individual outcome has probability zero and only events that
include infinitely many outcomes, such as intervals, can have positive
probability. For example, the probability that a given object weighs exactly
500 g is zero, because the probability of measuring exactly 500 g tends to zero
as the accuracy of our measuring instruments increases. Nevertheless, in
quality control one might demand that the probability of a "500 g" package
containing between 490 g and 510 g should be no less than 98%, and this demand
is less sensitive to the accuracy of measurement instruments.
Continuous probability distributions can be described in several ways. The
probability_density_function describes the infinitesimal probability of any
given value, and the probability that the outcome lies in a given interval can
be computed by integrating the probability density function over that interval.
On the other hand, the cumulative_distribution_function describes the
probability that the random variable is no larger than a given value; the
probability that the outcome lies in a given interval can be computed by taking
the difference between the values of the cumulative distribution function at
the endpoints of the interval. The cumulative distribution function is the
antiderivative of the probability density function provided that the latter
function exists.
The probability_density_function (pdf) of the normal_distribution, also called
Gaussian or "bell curve", the most important continuous random distribution. As
notated on the figure, the probabilities of intervals of values correspond to
the area under the curve.
***** Terminology[edit] *****
As probability theory is used in quite diverse applications, terminology is not
uniform and sometimes confusing. The following terms are used for non-
cumulative probability distribution functions:
    * Frequency distribution: A frequency_distribution is a table that displays
      the frequency of various outcomes in a sample.
    * Relative frequency distribution: A frequency_distribution where each
      value has been divided (normalized) by a number of outcomes in a sample
      i.e. sample size.
    * Probability distribution: Sometimes used as an alias for Relative
      frequency distribution but most books use it as a limit to which Relative
      frequency distribution tends when sample size tends to population size.
      It's a general term to indicate the way the total probability of 1 is
      distributed over all various possible outcomes (i.e. over entire
      population). It may for instance refer to a table that displays the
      probabilities of various outcomes in a finite population or to the
      probability density of an uncountably infinite population.
    * Cumulative_distribution_function: is a general functional form to
      describe a probability distribution.
    * Probability distribution function: somewhat ambiguous term sometimes
      referring to a functional form of probability distribution table. Could
      be called a "normalized frequency distribution function", where area
      under the graph equals to 1.
    * Probability mass, Probability_mass_function, p.m.f., Discrete probability
      distribution function: for discrete random variables.
    * Categorical_distribution: for discrete random variables with a finite set
      of values.
    * Probability density, Probability_density_function, p.d.f., Continuous
      probability distribution function: most often reserved for continuous
      random variables.
The following terms are somewhat ambiguous as they can refer to non-cumulative
or cumulative distributions, depending on authors' preferences:
    * Probability distribution function: continuous or discrete, non-cumulative
      or cumulative.
    * Probability function: even more ambiguous, can mean any of the above or
      other things.
**** Basic terms[edit] ****
    * Mode: for a discrete random variable, the value with highest probability
      (the location at which the probability mass function has its peak); for a
      continuous random variable, a location at which the probability density
      function has a local peak.
    * Support: the smallest closed set whose complement has probability zero.
    * Head: the range of values where the pmf or pdf is relatively high.
    * Tail: the complement of the head within the support; the large set of
      values where the pmf or pdf is relatively low.
    * Expected_value or mean: the weighted_average of the possible values,
      using their probabilities as their weights; or the continuous analog
      thereof.
    * Median: the value such that the set of values less than the median, and
      the set greater than the median, each have probabilities no greater than
      one-half.
    * Variance: the second moment of the pmf or pdf about the mean; an
      important measure of the dispersion of the distribution.
    * Standard_deviation: the square root of the variance, and hence another
      measure of dispersion.
    * Symmetry: a property of some distributions in which the portion of the
      distribution to the left of a specific value is a mirror image of the
      portion to its right.
    * Skewness: a measure of the extent to which a pmf or pdf "leans" to one
      side of its mean. The third standardized_moment of the distribution.
    * Kurtosis: a measure of the "fatness" of the tails of a pmf or pdf. The
      fourth standardized moment of the distribution.
***** Cumulative distribution function[edit] *****
Because a probability distribution P on the real line is determined by the
probability of a scalar random variable X being in a half-open interval
(ââ, x], the probability distribution is completely characterized by its
cumulative_distribution_function:
         F ( x ) = P &#x2061; [ X &#x2264; x ]   &#xA0;for all&#xA0;  x
      &#x2208;  R  .   {\displaystyle F(x)=\operatorname {P} [X\leq x]\qquad
      {\text{ for all }}x\in \mathbb {R} .}  [{\displaystyle F(x)=\operatorname
      {P} [X\leq x]\qquad {\text{ for all }}x\in \mathbb {R} .}]
***** Discrete probability distribution[edit] *****
See also: Probability_mass_function and Categorical_distribution
The probability mass function of a discrete probability distribution. The
probabilities of the singletons {1}, {3}, and {7} are respectively 0.2, 0.5,
0.3. A set not containing any of these points has probability zero.
The cdf of a discrete probability distribution, ...
... of a continuous probability distribution, ...
... of a distribution which has both a continuous part and a discrete part.
A discrete probability distribution is a probability distribution that can take
on a countable number of values.[1] For the probabilities to add up to 1, they
have to decline to zero fast enough. For example, if     P &#x2061; ( X = n ) =
1  2  n        {\displaystyle \operatorname {P} (X=n)={\tfrac {1}{2^{n}}}}  [
{\displaystyle \operatorname {P} (X=n)={\tfrac {1}{2^{n}}}}] for n = 1, 2, ...,
the sum of probabilities would be 1/2 + 1/4 + 1/8 + ... = 1.
Well-known discrete probability distributions used in statistical modeling
include the Poisson_distribution, the Bernoulli_distribution, the binomial
distribution, the geometric_distribution, and the negative_binomial
distribution. Additionally, the discrete_uniform_distribution is commonly used
in computer programs that make equal-probability random selections between a
number of choices.
When a sample (a set of observations) is drawn from a larger population, the
sample points have an empirical_distribution that is discrete and that provides
information about the population distribution.
**** Measure theoretic formulation[edit] ****
A measurable_function     X &#x003A; A &#x2192; B   {\displaystyle X\colon A\to
B}  [X\colon A\to B] between a probability_space     ( A ,   A   , P )
{\displaystyle (A,{\mathcal {A}},P)}  [(A,{\mathcal {A}},P)] and a measurable
space     ( B ,   B   )   {\displaystyle (B,{\mathcal {B}})}  [(B,{\mathcal
{B}})] is called a discrete random variable provided that its image is a
countable set. In this case measurability of     X   {\displaystyle X}  [X]
means that the pre-images of singleton sets are measurable, i.e.,      X
&#x2212; 1   ( { b } ) &#x2208;   A     {\displaystyle X^{-1}(\{b\})\in
{\mathcal {A}}}  [{\displaystyle X^{-1}(\{b\})\in {\mathcal {A}}}] for all
b &#x2208; B   {\displaystyle b\in B}  [b\in B]. The latter requirement induces
a probability_mass_function      f  X   &#x003A; X ( A ) &#x2192;  R
{\displaystyle f_{X}\colon X(A)\to \mathbb {R} }  [f_{X}\colon X(A)\to \mathbb
{R} ] via      f  X   ( b ) := P (  X  &#x2212; 1   ( { b } ) )
{\displaystyle f_{X}(b):=P(X^{-1}(\{b\}))}  [{\displaystyle f_{X}(b):=P(X^{-1}
(\{b\}))}]. Since the pre-images of disjoint sets are disjoint,
          &#x2211;  b &#x2208; X ( A )    f  X   ( b ) =  &#x2211;  b &#x2208;
      X ( A )   P (  X  &#x2212; 1   ( { b } ) ) = P  (   &#x22C3;  b &#x2208;
      X ( A )    X  &#x2212; 1   ( { b } )  )  = P ( A ) = 1.   {\displaystyle
      \sum _{b\in X(A)}f_{X}(b)=\sum _{b\in X(A)}P(X^{-1}(\{b\}))=P\left
      (\bigcup _{b\in X(A)}X^{-1}(\{b\})\right)=P(A)=1.}  [{\displaystyle \sum
      _{b\in X(A)}f_{X}(b)=\sum _{b\in X(A)}P(X^{-1}(\{b\}))=P\left(\bigcup _
      {b\in X(A)}X^{-1}(\{b\})\right)=P(A)=1.}]
This recovers the definition given above.
**** Cumulative distribution function[edit] ****
Equivalently to the above, a discrete random variable can be defined as a
random variable whose cumulative_distribution_function (cdf) increases only by
jump_discontinuitiesâthat is, its cdf increases only where it "jumps" to a
higher value, and is constant between those jumps. Note however that the points
where the cdf jumps may form a dense set of the real numbers. The points where
jumps occur are precisely the values which the random variable may take.
**** Delta-function representation[edit] ****
Consequently, a discrete probability distribution is often represented as a
generalized probability_density_function involving Dirac_delta_functions, which
substantially unifies the treatment of continuous and discrete distributions.
This is especially useful when dealing with probability distributions involving
both a continuous and a discrete part.
**** Indicator-function representation[edit] ****
For a discrete random variable X, let u0, u1, ... be the values it can take
with non-zero probability. Denote
          &#x03A9;  i   =  X  &#x2212; 1   (  u  i   ) = { &#x03C9; : X
      ( &#x03C9; ) =  u  i   } ,  i = 0 , 1 , 2 , &#x2026;   {\displaystyle
      \Omega _{i}=X^{-1}(u_{i})=\{\omega :X(\omega )=u_{i}\},\,i=0,1,2,\dots }
      [\Omega _{i}=X^{-1}(u_{i})=\{\omega :X(\omega )=u_{i}\},\,i=0,1,2,\dots ]
These are disjoint_sets, and for such sets
         P  (   &#x22C3;  i    &#x03A9;  i    )  =  &#x2211;  i   P (  &#x03A9;
      i   ) =  &#x2211;  i   P ( X =  u  i   ) = 1.   {\displaystyle P\left
      (\bigcup _{i}\Omega _{i}\right)=\sum _{i}P(\Omega _{i})=\sum _{i}P(X=u_
      {i})=1.}  [{\displaystyle P\left(\bigcup _{i}\Omega _{i}\right)=\sum _
      {i}P(\Omega _{i})=\sum _{i}P(X=u_{i})=1.}]
It follows that the probability that X takes any value except for u0, u1, ...
is zero, and thus one can write X as
         X ( &#x03C9; ) =  &#x2211;  i    u  i    1   &#x03A9;  i
      ( &#x03C9; )   {\displaystyle X(\omega )=\sum _{i}u_{i}1_{\Omega _{i}}
      (\omega )}  [{\displaystyle X(\omega )=\sum _{i}u_{i}1_{\Omega _{i}}
      (\omega )}]
except on a set of probability zero, where      1  A     {\displaystyle 1_{A}}
[1_{A}] is the indicator_function of A. This may serve as an alternative
definition of discrete random variables.
***** Continuous probability distribution[edit] *****
See also: Probability_density_function
A continuous probability distribution is a probability distribution with a
cumulative distribution function that is absolutely_continuous. Equivalently,
it is a probability distribution on the real_numbers that is absolutely
continuous with respect to Lebesgue_measure. Such distributions can be
represented by their probability_density_functions. If the distribution of X is
continuous, then X is called a continuous random variable. There are many
examples of continuous probability distributions: normal, uniform, chi-squared,
and others.
Formally, if X is a continuous random variable, then it has a probability
density_function Æ(x), and therefore its probability of falling into a given
interval, say [a, b], is given by the integral
         P &#x2061; [ a &#x2264; X &#x2264; b ] =  &#x222B;  a   b   f ( x )  d
      x   {\displaystyle \operatorname {P} [a\leq X\leq b]=\int _{a}^{b}f
      (x)\,dx}  [{\displaystyle \operatorname {P} [a\leq X\leq b]=\int _{a}^
      {b}f(x)\,dx}]
In particular, the probability for X to take any single value a (that is a â¤
X â¤ a) is zero, because an integral with coinciding upper and lower limits is
always equal to zero.
Note on terminology: some authors use the term "continuous distribution" to
denote distributions whose cumulative distribution functions are continuous,
rather than absolutely_continuous. These distributions are the ones
&#x03BC;   {\displaystyle \mu }  [\mu ] such that     &#x03BC; { x }  =  0
{\displaystyle \mu \{x\}\,=\,0}  [\mu \{x\}\,=\,0] for all      x
{\displaystyle \,x}  [\,x]. This definition includes the (absolutely)
continuous distributions defined above, but it also includes singular
distributions, which are neither continuous nor discrete nor a mixture of
those. An example is given by the Cantor_distribution.
***** Some properties[edit] *****
    * The probability distribution of the sum of two independent random
      variables is the convolution of each of their distributions.
    * Probability distributions are not a vector_spaceâthey are not closed
      under linear_combinations, as these do not preserve non-negativity or
      total integral 1âbut they are closed under convex_combination, thus
      forming a convex_subset of the space of functions (or measures).
***** Kolmogorov definition[edit] *****
Main articles: Probability_space and Probability_measure
In the measure-theoretic formalization of probability_theory, a random_variable
is defined as a measurable_function X from a probability_space      ( &#x03A9;
,   F   , P )    {\displaystyle \scriptstyle (\Omega ,{\mathcal
{F}},\operatorname {P} )}  [\scriptstyle (\Omega ,{\mathcal {F}},\operatorname
{P} )] to a measurable_space      (   X   ,   A   )    {\displaystyle
\scriptstyle ({\mathcal {X}},{\mathcal {A}})}  [\scriptstyle ({\mathcal {X}},
{\mathcal {A}})]. A probability distribution of X is the pushforward_measure
X*P  of X , which is a probability_measure on      (   X   ,   A   )
{\displaystyle \scriptstyle ({\mathcal {X}},{\mathcal {A}})}  [\scriptstyle (
{\mathcal {X}},{\mathcal {A}})] satisfying X*P = PXâ1.[2]
***** Random number generation[edit] *****
Main article: Pseudo-random_number_sampling
A frequent problem in statistical simulations (the Monte_Carlo_method) is the
generation of pseudo-random_numbers that are distributed in a given way. Most
algorithms are based on a pseudorandom_number_generator that produces numbers X
that are uniformly distributed in the half-open_interval [0,1). These random
variates X are then transformed via some algorithm to create a new random
variate having the required probability distribution.
***** Applications[edit] *****
The concept of the probability distribution and the random variables which they
describe underlies the mathematical discipline of probability theory, and the
science of statistics. There is spread or variability in almost any value that
can be measured in a population (e.g. height of people, durability of a metal,
sales growth, traffic flow, etc.); almost all measurements are made with some
intrinsic error; in physics many processes are described probabilistically,
from the kinetic_properties_of_gases to the quantum_mechanical description of
fundamental_particles. For these and many other reasons, simple numbers are
often inadequate for describing a quantity, while probability distributions are
often more appropriate.
Several more specific example of an application:
    * The cache_language_models and other statistical_language_models used in
      natural_language_processing to assign probabilities to the occurrence of
      particular words and word sequences do so by means of probability
      distributions.
    * Probabilistic load flow in power-flow_study explains the uncertainties of
      input variables as probability distribution and provide the power flow
      calculation also in term of probability distribution.[3]
***** Common probability distributions[edit] *****
For a more comprehensive list, see List_of_probability_distributions.
The following is a list of some of the most common probability distributions,
grouped by the type of process that they are related to. For a more complete
list, see list_of_probability_distributions, which groups by the nature of the
outcome being considered (discrete, continuous, multivariate, etc.)
All of the univariate distributions below are singly peaked; that is, it is
assumed that the values cluster around a single point. In practice, actually
observed quantities may cluster around multiple values. Such quantities can be
modeled using a mixture_distribution.
**** Related to real-valued quantities that grow linearly (e.g. errors,
offsets)[edit] ****
    * Normal_distribution (Gaussian distribution), for a single such quantity;
      the most commonly used continuous distribution
**** Related to positive real-valued quantities that grow exponentially (e.g.
prices, incomes, populations)[edit] ****
    * Log-normal_distribution, for a single such quantity whose log is normally
      distributed
    * Pareto_distribution, for a single such quantity whose log is
      exponentially distributed; the prototypical power_law distribution
**** Related to real-valued quantities that are assumed to be uniformly
distributed over a (possibly unknown) region[edit] ****
    * Discrete_uniform_distribution, for a finite set of values (e.g. the
      outcome of a fair die)
    * Continuous_uniform_distribution, for continuously distributed values
**** Related to Bernoulli trials (yes/no events, with a given probability)
[edit] ****
    * Basic distributions:
          o Bernoulli_distribution, for the outcome of a single Bernoulli trial
            (e.g. success/failure, yes/no)
          o Binomial_distribution, for the number of "positive occurrences"
            (e.g. successes, yes votes, etc.) given a fixed total number of
            independent occurrences
          o Negative_binomial_distribution, for binomial-type observations but
            where the quantity of interest is the number of failures before a
            given number of successes occurs
          o Geometric_distribution, for binomial-type observations but where
            the quantity of interest is the number of failures before the first
            success; a special case of the negative_binomial_distribution
    * Related to sampling schemes over a finite population:
          o Hypergeometric_distribution, for the number of "positive
            occurrences" (e.g. successes, yes votes, etc.) given a fixed number
            of total occurrences, using sampling_without_replacement
          o Beta-binomial_distribution, for the number of "positive
            occurrences" (e.g. successes, yes votes, etc.) given a fixed number
            of total occurrences, sampling using a PÃ³lya_urn_scheme (in some
            sense, the "opposite" of sampling_without_replacement)
**** Related to categorical outcomes (events with K possible outcomes, with a
given probability for each outcome)[edit] ****
    * Categorical_distribution, for a single categorical outcome (e.g. yes/no/
      maybe in a survey); a generalization of the Bernoulli_distribution
    * Multinomial_distribution, for the number of each type of categorical
      outcome, given a fixed number of total outcomes; a generalization of the
      binomial_distribution
    * Multivariate_hypergeometric_distribution, similar to the multinomial
      distribution, but using sampling_without_replacement; a generalization of
      the hypergeometric_distribution
**** Related to events in a Poisson process (events that occur independently
with a given rate)[edit] ****
    * Poisson_distribution, for the number of occurrences of a Poisson-type
      event in a given period of time
    * Exponential_distribution, for the time before the next Poisson-type event
      occurs
    * Gamma_distribution, for the time before the next k Poisson-type events
      occur
**** Related to the absolute values of vectors with normally distributed
components[edit] ****
    * Rayleigh_distribution, for the distribution of vector magnitudes with
      Gaussian distributed orthogonal components. Rayleigh distributions are
      found in RF signals with Gaussian real and imaginary components.
    * Rice_distribution, a generalization of the Rayleigh distributions for
      where there is a stationary background signal component. Found in Rician
      fading of radio signals due to multipath propagation and in MR images
      with noise corruption on non-zero NMR signals.
**** Related to normally distributed quantities operated with sum of squares
(for hypothesis testing)[edit] ****
    * Chi-squared_distribution, the distribution of a sum of squared standard
      normal variables; useful e.g. for inference regarding the sample_variance
      of normally distributed samples (see chi-squared_test)
    * Student's_t_distribution, the distribution of the ratio of a standard
      normal variable and the square root of a scaled chi_squared variable;
      useful for inference regarding the mean of normally distributed samples
      with unknown variance (see Student's_t-test)
    * F-distribution, the distribution of the ratio of two scaled chi_squared
      variables; useful e.g. for inferences that involve comparing variances or
      involving R-squared (the squared correlation_coefficient)
**** Useful as conjugate prior distributions in Bayesian inference[edit] ****
Main article: Conjugate_prior
    * Beta_distribution, for a single probability (real number between 0 and
      1); conjugate to the Bernoulli_distribution and binomial_distribution
    * Gamma_distribution, for a non-negative scaling parameter; conjugate to
      the rate parameter of a Poisson_distribution or exponential_distribution,
      the precision (inverse variance) of a normal_distribution, etc.
    * Dirichlet_distribution, for a vector of probabilities that must sum to 1;
      conjugate to the categorical_distribution and multinomial_distribution;
      generalization of the beta_distribution
    * Wishart_distribution, for a symmetric non-negative_definite matrix;
      conjugate to the inverse of the covariance_matrix of a multivariate
      normal_distribution; generalization of the gamma_distribution
***** See also[edit] *****
    * [icon]Statistics_portal
    * List_of_probability_distributions
    * Copula_(statistics)
    * Empirical_probability
    * Histogram
    * Joint_probability_distribution
    * Likelihood_function
    * List_of_statistical_topics
    * Kirkwood_approximation
    * Moment-generating_function
    * Quasiprobability_distribution
    * RiemannâStieltjes_integral_application_to_probability_theory
***** References[edit] *****
**** Citations[edit] ****
   1. ^1941-, ÃÄ±nlar, E. (Erhan) (2011). Probability and stochastics. New
      York: Springer. p. 51. ISBN 9780387878591. OCLC 710149819.
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
   3. ^W., Stroock, Daniel (1999). Probability theory : an analytic view (Rev.
      ed.). Cambridge [England]: Cambridge University Press. p. 11. ISBN 978-
      0521663496. OCLC 43953136.
   4. ^Chen, P.; Chen, Z.; Bak-Jensen, B. (April 2008). "Probabilistic_load
      flow:_A_review". 2008 Third International Conference on Electric Utility
      Deregulation and Restructuring and Power Technologies. pp. 1586â1591.
      doi:10.1109/drpt.2008.4523658. ISBN 978-7-900714-13-8.
**** Sources[edit] ****
    * B. S. Everitt: The Cambridge Dictionary of Statistics, Cambridge
      University_Press, Cambridge (3rd edition, 2006).
ISBN 0-521-69027-7
Bishop: Pattern Recognition and Machine Learning, Springer,
ISBN 0-387-31073-8.
den Dekker, A. J.; Sijbers, J. (2014). "Data distributions in magnetic
resonance images: A review". Physica_Medica. 30 (7): 725â741. doi:10.1016/
j.ejmp.2014.05.002. PMID 25059432.
***** External links[edit] *****
 Wikimedia Commons has media related to Probability_distribution.
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Probability_distribution",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Field_Guide_to_Continuous_Probability_Distributions, Gavin E. Crooks.
    * v
    * t
    * e
Probability distributions
List
                                          * Benford
                                          * Bernoulli
                                          * beta-binomial
                                          * binomial
                                          * categorical
Discrete univariate                       * hypergeometric
with finite support                       * Poisson_binomial
                                          * Rademacher
                                          * soliton
                                          * discrete_uniform
                                          * Zipf
                                          * ZipfâMandelbrot
                                          * beta_negative_binomial
                                          * Borel
                                          * ConwayâMaxwellâPoisson
                                          * discrete_phase-type
                                          * Delaporte
                                          * extended_negative_binomial
Discrete univariate                       * GaussâKuzmin
with infinite support                     * geometric
                                          * logarithmic
                                          * negative_binomial
                                          * parabolic_fractal
                                          * Poisson
                                          * Skellam
                                          * YuleâSimon
                                          * zeta
                                          * arcsine
                                          * ARGUS
                                          * BaldingâNichols
                                          * Bates
                                          * beta
                                          * beta_rectangular
                                          * IrwinâHall
Continuous univariate                     * Kumaraswamy
supported on a bounded interval           * logit-normal
                                          * noncentral_beta
                                          * raised_cosine
                                          * reciprocal
                                          * triangular
                                          * U-quadratic
                                          * uniform
                                          * Wigner_semicircle
                                          * Benini
                                          * Benktander_1st_kind
                                          * Benktander_2nd_kind
                                          * beta_prime
                                          * Burr
                                          * chi-squared
                                          * chi
                                          * Dagum
                                          * Davis
                                          * exponential-logarithmic
                                          * Erlang
                                          * exponential
                                          * F
                                          * folded_normal
                                          * FloryâSchulz
                                          * FrÃ©chet
                                          * gamma
                                          * gamma/Gompertz
                                          * generalized_inverse_Gaussian
                                          * Gompertz
                                          * half-logistic
                                          * half-normal
                                          * Hotelling's_T-squared
                                          * hyper-Erlang
                                          * hyperexponential
                                          * hypoexponential
Continuous univariate                     * inverse_chi-squared
supported on a semi-infinite interval           o scaled_inverse_chi-squared
                                          * inverse_Gaussian
                                          * inverse_gamma
                                          * Kolmogorov
                                          * LÃ©vy
                                          * log-Cauchy
                                          * log-Laplace
                                          * log-logistic
                                          * log-normal
                                          * Lomax
                                          * matrix-exponential
                                          * MaxwellâBoltzmann
                                          * MaxwellâJÃ¼ttner
                                          * Mittag-Leffler
                                          * Nakagami
                                          * noncentral_chi-squared
                                          * Pareto
                                          * phase-type
                                          * poly-Weibull
                                          * Rayleigh
                                          * relativistic_BreitâWigner
                                          * Rice
                                          * shifted_Gompertz
                                          * truncated_normal
                                          * type-2_Gumbel
                                          * Weibull
                                                o Discrete_Weibull
                                          * Wilks's_lambda
                                          * Cauchy
                                          * exponential_power
                                          * Fisher's_z
                                          * Gaussian_q
                                          * generalized_normal
                                          * generalized_hyperbolic
                                          * geometric_stable
                                          * Gumbel
                                          * Holtsmark
                                          * hyperbolic_secant
                                          * Johnson's_SU
                                          * Landau
Continuous univariate                     * Laplace
supported on the whole real line          * asymmetric_Laplace
                                          * logistic
                                          * noncentral_t
                                          * normal_(Gaussian)
                                          * normal-inverse_Gaussian
                                          * skew_normal
                                          * slash
                                          * stable
                                          * Student's_t
                                          * type-1_Gumbel
                                          * TracyâWidom
                                          * variance-gamma
                                          * Voigt
                                          * generalized_extreme_value
                                          * generalized_Pareto
                                          * MarchenkoâPastur
Continuous univariate                     * q-exponential
with support whose type varies            * q-Gaussian
                                          * q-Weibull
                                          * shifted_log-logistic
                                          * Tukey_lambda
Mixed continuous-discrete univariate      * rectified_Gaussian
                                            inverse_matrix_gamma
                                            inverse-Wishart
                                            matrix_normal
Multivariate_(joint)                        matrix_t
                                            matrix_gamma
                                            normal-inverse-Wishart
                                            normal-Wishart
                                            Wishart
Directional                                 von_MisesâFisher
                                            Bingham
Degenerate and singular                     Cantor
                                          * Circular
                                          * compound_Poisson
                                          * elliptical
                                          * exponential
                                          * natural_exponential
Families                                  * locationâscale
                                          * maximum_entropy
                                          * mixture
                                          * Pearson
                                          * Tweedie
                                          * wrapped
    * v
    * t
    * e
Theory of probability distributions
    * probability_mass_function (pmf)
    * probability_density_function (pdf)
    * cumulative_distribution_function (cdf)
    * quantile_function
    * raw_moment
    * central_moment
    * mean
    * variance
    * standard_deviation                     [Loglogisticpdf_no-labels.svg]
    * skewness
    * kurtosis
    * L-moment
    * moment-generating_function (mgf)
    * characteristic_function
    * probability-generating_function (pgf)
    * cumulant
    * combinant
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
                * Probability distribution
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
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85038545
                                              * NDL: 00564751

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Probability_distribution&oldid=909787075"
Categories:
    * Probability_distributions
    * Mathematical_and_quantitative_methods_(economics)
Hidden categories:
    * Articles_lacking_in-text_citations_from_July_2011
    * All_articles_lacking_in-text_citations
    * Articles_needing_additional_references_from_July_2011
    * All_articles_needing_additional_references
    * Articles_with_multiple_maintenance_issues
    * Wikipedia_articles_with_LCCN_identifiers
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
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
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * Latina
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * à·à·à¶à·à¶½
    * Simple_English
    * SlovenÅ¡Äina
    * Basa_Sunda
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 16:22 (UTC).
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
