The following text has been accessed from https://en.wikipedia.org/wiki/Multinomial_distribution at Fri Aug 9 02:54:33 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Multinomial distribution ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
                                  Multinomial
              n > 0   {\displaystyle n>0}  [n>0] number of trials (integer)
Parameters     p  1   , &#x2026; ,  p  k     {\displaystyle p_{1},\ldots ,p_
           {k}}  [p_{1},\ldots ,p_{k}] event probabilities (    &#x03A3;  p  i
           = 1   {\displaystyle \Sigma p_{i}=1}  [\Sigma p_{i}=1])
               x  i   &#x2208; { 0 , &#x2026; , n } ,     i &#x2208; { 1 ,
           &#x2026; , k }   {\displaystyle x_{i}\in \{0,\dots ,n\},\,\,\,\,i\in
Support    \{1,\dots ,k\}}  [{\displaystyle x_{i}\in \{0,\dots
           ,n\},\,\,\,\,i\in \{1,\dots ,k\}}]
              &#x03A3;  x  i   = n    {\displaystyle \Sigma x_{i}=n\!}  [
           {\displaystyle \Sigma x_{i}=n\!}]
                 n !    x  1   ! &#x22EF;  x  k   !     p  1    x  1
pmf        &#x22EF;  p  k    x  k       {\displaystyle {\frac {n!}{x_{1}!\cdots
           x_{k}!}}p_{1}^{x_{1}}\cdots p_{k}^{x_{k}}}  [\frac{n!}{x_1!\cdots
           x_k!} p_1^{x_1} \cdots p_k^{x_k}]
              E &#x2061; (  X  i   ) = n  p  i     {\displaystyle \operatorname
Mean       {E} (X_{i})=np_{i}}  [{\displaystyle \operatorname {E} (X_{i})=np_
           {i}}]
              Var &#x2061; (  X  i   ) = n  p  i   ( 1 &#x2212;  p  i   )
           {\displaystyle \operatorname {Var} (X_{i})=np_{i}(1-p_{i})}  [
           {\displaystyle \operatorname {Var} (X_{i})=np_{i}(1-p_{i})}]
Variance      Cov &#x2061; (  X  i   ,  X  j   ) = &#x2212; n  p  i    p  j
           &#xA0; &#xA0; ( i &#x2260; j )   {\displaystyle \operatorname {Cov}
           (X_{i},X_{j})=-np_{i}p_{j}~~(i\neq j)}  [{\displaystyle
           \operatorname {Cov} (X_{i},X_{j})=-np_{i}p_{j}~~(i\neq j)}]
              &#x2212; log &#x2061; ( n ! ) &#x2212; n  &#x2211;  i = 1   k
           p  i   log &#x2061; (  p  i   ) +  &#x2211;  i = 1   k    &#x2211;
           x  i   = 0   n      (   n  x  i     )     p  i    x  i     ( 1
           &#x2212;  p  i    )  n &#x2212;  x  i     log &#x2061; (  x  i   ! )
Entropy    {\displaystyle -\log(n!)-n\sum _{i=1}^{k}p_{i}\log(p_{i})+\sum _
           {i=1}^{k}\sum _{x_{i}=0}^{n}{\binom {n}{x_{i}}}p_{i}^{x_{i}}(1-p_
           {i})^{n-x_{i}}\log(x_{i}!)}  [{\displaystyle -\log(n!)-n\sum _{i=1}^
           {k}p_{i}\log(p_{i})+\sum _{i=1}^{k}\sum _{x_{i}=0}^{n}{\binom {n}{x_
           {i}}}p_{i}^{x_{i}}(1-p_{i})^{n-x_{i}}\log(x_{i}!)}]
                (    &#x2211;  i = 1   k    p  i    e   t  i        )    n
MGF        {\displaystyle {\biggl (}\sum _{i=1}^{k}p_{i}e^{t_{i}}{\biggr )}^
           {n}}  [\biggl( \sum_{i=1}^k p_i e^{t_i} \biggr)^n]
                (   &#x2211;  j = 1   k    p  j    e  i  t  j      )   n
CF         {\displaystyle \left(\sum _{j=1}^{k}p_{j}e^{it_{j}}\right)^{n}}
           [ \left(\sum_{j=1}^k p_je^{it_j}\right)^n] where      i  2   =
           &#x2212; 1   {\displaystyle i^{2}=-1}  [i^{2}=-1]
                (    &#x2211;  i = 1   k    p  i    z  i      )    n
           &#xA0;for&#xA0;  (  z  1   , &#x2026; ,  z  k   ) &#x2208;   C   k
PGF        {\displaystyle {\biggl (}\sum _{i=1}^{k}p_{i}z_{i}{\biggr )}^{n}
           {\text{ for }}(z_{1},\ldots ,z_{k})\in \mathbb {C} ^{k}}  [\biggl
           ( \sum_{i=1}^k p_i z_i \biggr)^n\text{ for }
           (z_1,\ldots,z_k)\in\mathbb{C}^k]
In probability_theory, the multinomial distribution is a generalization of the
binomial_distribution. For example, it models the probability of counts of each
side for rolling a k-sided die n times. For n independent trials each of which
leads to a success for exactly one of k categories, with each category having a
given fixed success probability, the multinomial distribution gives the
probability of any particular combination of numbers of successes for the
various categories.
When k is 2 and n is 1, the multinomial distribution is the Bernoulli
distribution. When k is 2 and n is bigger than 1, it is the binomial
distribution. When k is bigger than 2 and n is 1, it is the categorical
distribution.
The Bernoulli_distribution models the outcome of a single Bernoulli_trial. In
other words, it models whether flipping a (possibly biased) coin one time will
result in either a success (obtaining a head) or failure (obtaining a tail).
The binomial_distribution generalizes this to the number of heads from
performing n independent flips (Bernoulli trials) of the same coin. The
multinomial distribution models the outcome of n experiments, where the outcome
of each trial has a categorical_distribution, such as rolling a k-sided die n
times.
Let k be a fixed finite number. Mathematically, we have k possible mutually
exclusive outcomes, with corresponding probabilities p1, ..., pk, and n
independent trials. Since the k outcomes are mutually exclusive and one must
occur we have pi â¥ 0 for i = 1, ..., k and      &#x2211;  i = 1   k    p  i
= 1   {\displaystyle \sum _{i=1}^{k}p_{i}=1}  [\sum_{i=1}^k p_i = 1]. Then if
the random variables Xi indicate the number of times outcome number i is
observed over the n trials, the vector X = (X1, ..., Xk) follows a multinomial
distribution with parameters n and p, where p = (p1, ..., pk). While the trials
are independent, their outcomes X are dependent because they must be summed to
n.
In some fields such as natural_language_processing, categorical and multinomial
distributions are synonymous and it is common to speak of a multinomial
distribution when a categorical_distribution is actually meant. This stems from
the fact that it is sometimes convenient to express the outcome of a
categorical distribution as a "1-of-K" vector (a vector with one element
containing a 1 and all other elements containing a 0) rather than as an integer
in the range     1 &#x2026; K   {\displaystyle 1\dots K}  [1 \dots K]; in this
form, a categorical distribution is equivalent to a multinomial distribution
over a single trial.
⁰
***** Contents *****
    * 1_Specification
          o 1.1_Probability_mass_function
    * 2_Visualization
          o 2.1_As_slices_of_generalized_Pascal's_triangle
          o 2.2_As_polynomial_coefficients
    * 3_Properties
          o 3.1_Matrix_notation
    * 4_Example
    * 5_Sampling_from_a_multinomial_distribution
    * 6_To_simulate_from_a_multinomial_distribution
    * 7_Related_distributions
    * 8_References
          o 8.1_Citations
          o 8.2_Sources
***** Specification[edit] *****
**** Probability mass function[edit] ****
Suppose one does an experiment of extracting n balls of k different colors from
a bag, replacing the extracted ball after each draw. Balls from the same color
are equivalent. Denote the variable which is the number of extracted balls of
color i (i = 1, ..., k) as Xi, and denote as pi the probability that a given
extraction will be in color i. The probability_mass_function of this
multinomial distribution is:
             f (  x  1   , &#x2026; ,  x  k   ; n ,  p  1   , &#x2026; ,  p  k
      )      = Pr (  X  1   =  x  1    &#xA0;and&#xA0;  &#x2026;
      &#xA0;and&#xA0;   X  k   =  x  k   )         =   {         n !    x  1
      ! &#x22EF;  x  k   !     p  1    x  1     &#x00D7; &#x22EF; &#x00D7;  p
      k    x  k       ,     when&#xA0;   &#x2211;  i = 1   k    x  i   = n
      0    otherwise,              {\displaystyle {\begin{aligned}f(x_
      {1},\ldots ,x_{k};n,p_{1},\ldots ,p_{k})&{}=\Pr(X_{1}=x_{1}{\text{ and
      }}\dots {\text{ and }}X_{k}=x_{k})\\&{}={\begin{cases}{\displaystyle {n!
      \over x_{1}!\cdots x_{k}!}p_{1}^{x_{1}}\times \cdots \times p_{k}^{x_
      {k}}},\quad &{\text{when }}\sum _{i=1}^{k}x_{i}=n\\\\0&{\text
      {otherwise,}}\end{cases}}\end{aligned}}}  [{\displaystyle {\begin
      {aligned}f(x_{1},\ldots ,x_{k};n,p_{1},\ldots ,p_{k})&{}=\Pr(X_{1}=x_{1}
      {\text{ and }}\dots {\text{ and }}X_{k}=x_{k})\\&{}={\begin{cases}
      {\displaystyle {n! \over x_{1}!\cdots x_{k}!}p_{1}^{x_{1}}\times \cdots
      \times p_{k}^{x_{k}}},\quad &{\text{when }}\sum _{i=1}^{k}x_{i}=n\\\\0&
      {\text{otherwise,}}\end{cases}}\end{aligned}}}]
for non-negative integers x1, ..., xk.
The probability mass function can be expressed using the gamma_function as:
         f (  x  1   , &#x2026; ,  x  k   ;  p  1   , &#x2026; ,  p  k   ) =
      &#x0393; (  &#x2211;  i    x  i   + 1 )    &#x220F;  i   &#x0393; (  x  i
      + 1 )     &#x220F;  i = 1   k    p  i    x  i     .   {\displaystyle f(x_
      {1},\dots ,x_{k};p_{1},\ldots ,p_{k})={\frac {\Gamma (\sum _{i}x_{i}+1)}
      {\prod _{i}\Gamma (x_{i}+1)}}\prod _{i=1}^{k}p_{i}^{x_{i}}.}  [f
      (x_1,\dots, x_{k}; p_1,\ldots, p_k) = \frac{\Gamma(\sum_i x_i + 1)}
      {\prod_i \Gamma(x_i+1)} \prod_{i=1}^k p_i^{x_i}.]
This form shows its resemblance to the Dirichlet_distribution which is its
conjugate_prior.
***** Visualization[edit] *****
**** As slices of generalized Pascal's triangle[edit] ****
Just like one can interpret the binomial_distribution as (normalized) one-
dimensional (1D) slices of Pascal's_triangle, so too can one interpret the
multinomial distribution as 2D (triangular) slices of Pascal's_pyramid, or 3D/
4D/+ (pyramid-shaped) slices of higher-dimensional analogs of Pascal's
triangle. This reveals an interpretation of the range of the distribution:
discretized equilaterial "pyramids" in arbitrary dimensionâi.e. a simplex
with a grid.
**** As polynomial coefficients[edit] ****
Similarly, just like one can interpret the binomial_distribution as the
polynomial coefficients of     ( p  x  1   + ( 1 &#x2212; p )  x  2    )  n
{\displaystyle (px_{1}+(1-p)x_{2})^{n}}  [(p x_1 + (1-p) x_2)^n] when expanded,
one can interpret the multinomial distribution as the coefficients of     (  p
1    x  1   +  p  2    x  2   +  p  3    x  3   + &#x22EF; +  p  k    x  k    )
n     {\displaystyle (p_{1}x_{1}+p_{2}x_{2}+p_{3}x_{3}+\cdots +p_{k}x_{k})^{n}}
[{\displaystyle (p_{1}x_{1}+p_{2}x_{2}+p_{3}x_{3}+\cdots +p_{k}x_{k})^{n}}]
when expanded. (Note that just like the binomial distribution, the coefficients
must sum to 1.) This is the origin of the name "multinomial distribution".
***** Properties[edit] *****
The expected number of times the outcome i was observed over n trials is
         E &#x2061; (  X  i   ) = n  p  i   .    {\displaystyle \operatorname
      {E} (X_{i})=np_{i}.\,}  [\operatorname{E}(X_i) = n p_i.\,]
The covariance_matrix is as follows. Each diagonal entry is the variance of a
binomially distributed random variable, and is therefore
         Var &#x2061; (  X  i   ) = n  p  i   ( 1 &#x2212;  p  i   ) .
      {\displaystyle \operatorname {Var} (X_{i})=np_{i}(1-p_{i}).\,}  [
      {\displaystyle \operatorname {Var} (X_{i})=np_{i}(1-p_{i}).\,}]
The off-diagonal entries are the covariances:
         Cov &#x2061; (  X  i   ,  X  j   ) = &#x2212; n  p  i    p  j
      {\displaystyle \operatorname {Cov} (X_{i},X_{j})=-np_{i}p_{j}\,}  [
      {\displaystyle \operatorname {Cov} (X_{i},X_{j})=-np_{i}p_{j}\,}]
for i, j distinct.
All covariances are negative because for fixed n, an increase in one component
of a multinomial vector requires a decrease in another component.
When these expressions are combined into a matrix with i, j element     cov
&#x2061; (  X  i   ,  X  j   ) ,   {\displaystyle \operatorname {cov} (X_{i},X_
{j}),}  [{\displaystyle \operatorname {cov} (X_{i},X_{j}),}] the result is a k
× k positive-semidefinite covariance_matrix of rank k − 1. In the special case
where k = n and where the pi are all equal, the covariance matrix is the
centering_matrix.
The entries of the corresponding correlation_matrix are
         &#x03C1; (  X  i   ,  X  i   ) = 1.   {\displaystyle \rho (X_{i},X_
      {i})=1.}  [\rho(X_i,X_i) = 1.]
         &#x03C1; (  X  i   ,  X  j   ) =    Cov &#x2061; (  X  i   ,  X  j   )
      Var &#x2061; (  X  i   ) Var &#x2061; (  X  j   )    =    &#x2212;  p  i
      p  j      p  i   ( 1 &#x2212;  p  i   )  p  j   ( 1 &#x2212;  p  j   )
      = &#x2212;      p  i    p  j     ( 1 &#x2212;  p  i   ) ( 1 &#x2212;  p
      j   )     .   {\displaystyle \rho (X_{i},X_{j})={\frac {\operatorname
      {Cov} (X_{i},X_{j})}{\sqrt {\operatorname {Var} (X_{i})\operatorname
      {Var} (X_{j})}}}={\frac {-p_{i}p_{j}}{\sqrt {p_{i}(1-p_{i})p_{j}(1-p_
      {j})}}}=-{\sqrt {\frac {p_{i}p_{j}}{(1-p_{i})(1-p_{j})}}}.}  [
      {\displaystyle \rho (X_{i},X_{j})={\frac {\operatorname {Cov} (X_{i},X_
      {j})}{\sqrt {\operatorname {Var} (X_{i})\operatorname {Var} (X_{j})}}}=
      {\frac {-p_{i}p_{j}}{\sqrt {p_{i}(1-p_{i})p_{j}(1-p_{j})}}}=-{\sqrt
      {\frac {p_{i}p_{j}}{(1-p_{i})(1-p_{j})}}}.}]
Note that the sample size drops out of this expression.
Each of the k components separately has a binomial distribution with parameters
n and pi, for the appropriate value of the subscript i.
The support of the multinomial distribution is the set
         { (  n  1   , &#x2026; ,  n  k   ) &#x2208;   N   k   &#x2223;  n  1
      + &#x22EF; +  n  k   = n } .    {\displaystyle \{(n_{1},\dots ,n_{k})\in
      \mathbb {N} ^{k}\mid n_{1}+\cdots +n_{k}=n\}.\,}  [{\displaystyle \{(n_
      {1},\dots ,n_{k})\in \mathbb {N} ^{k}\mid n_{1}+\cdots +n_{k}=n\}.\,}]
Its number of elements is
            (    n + k &#x2212; 1   k &#x2212; 1    )    .   {\displaystyle
      {n+k-1 \choose k-1}.}  [{n+k-1 \choose k-1}.]
**** Matrix notation[edit] ****
In matrix notation,
         E &#x2061; (  X  ) = n  p  ,    {\displaystyle \operatorname {E}
      (\mathbf {X} )=n\mathbf {p} ,\,}  [{\displaystyle \operatorname {E}
      (\mathbf {X} )=n\mathbf {p} ,\,}]
and
         Var &#x2061; (  X  ) = n { diag &#x2061; (  p  ) &#x2212;  p    p    T
      } ,    {\displaystyle \operatorname {Var} (\mathbf {X} )=n\lbrace
      \operatorname {diag} (\mathbf {p} )-\mathbf {p} \mathbf {p} ^{\rm
      {T}}\rbrace ,\,}  [{\displaystyle \operatorname {Var} (\mathbf {X}
      )=n\lbrace \operatorname {diag} (\mathbf {p} )-\mathbf {p} \mathbf {p} ^
      {\rm {T}}\rbrace ,\,}]
with pT = the row vector transpose of the column vector p.
***** Example[edit] *****
Suppose that in a three-way election for a large country, candidate A received
20% of the votes, candidate B received 30% of the votes, and candidate C
received 50% of the votes. If six voters are selected randomly, what is the
probability that there will be exactly one supporter for candidate A, two
supporters for candidate B and three supporters for candidate C in the sample?
Note: Since weâre assuming that the voting population is large, it is
reasonable and permissible to think of the probabilities as unchanging once a
voter is selected for the sample. Technically speaking this is sampling without
replacement, so the correct distribution is the multivariate_hypergeometric
distribution, but the distributions converge as the population grows large.
         Pr ( A = 1 , B = 2 , C = 3 ) =    6 !   1 ! 2 ! 3 !    (  0.2  1   )
      (  0.3  2   ) (  0.5  3   ) = 0.135   {\displaystyle \Pr(A=1,B=2,C=3)=
      {\frac {6!}{1!2!3!}}(0.2^{1})(0.3^{2})(0.5^{3})=0.135}  [ \Pr
      (A=1,B=2,C=3) = \frac{6!}{1! 2! 3!}(0.2^1) (0.3^2) (0.5^3) = 0.135 ]
***** Sampling from a multinomial distribution[edit] *****
First, reorder the parameters      p  1   , &#x2026; ,  p  k     {\displaystyle
p_{1},\ldots ,p_{k}}  [p_{1},\ldots ,p_{k}] such that they are sorted in
descending order (this is only to speed up computation and not strictly
necessary). Now, for each trial, draw an auxiliary variable X from a uniform
(0, 1) distribution. The resulting outcome is the component
         j = min  {   j &#x2032;  &#x2208; { 1 , &#x2026; , k } :  (   &#x2211;
      i = 1    j &#x2032;     p  i    )  &#x2212; X &#x2265; 0  }  .
      {\displaystyle j=\min \left\{j'\in \{1,\dots ,k\}:\left(\sum _{i=1}^
      {j'}p_{i}\right)-X\geq 0\right\}.}  [{\displaystyle j=\min \left\{j'\in \
      {1,\dots ,k\}:\left(\sum _{i=1}^{j'}p_{i}\right)-X\geq 0\right\}.}]
{Xj = 1, Xk = 0 for k â  j } is one observation from the multinomial
distribution with      p  1   , &#x2026; ,  p  k     {\displaystyle p_
{1},\ldots ,p_{k}}  [p_{1},\ldots ,p_{k}] and n = 1. A sum of independent
repetitions of this experiment is an observation from a multinomial
distribution with n equal to the number of such repetitions.
***** To simulate from a multinomial distribution[edit] *****
Various methods may be used to simulate from a multinomial distribution. A very
simple solution is to use a uniform pseudo-random number generator on (0,1).
First, we divide the (0,1) interval in k subintervals equal in length to the
probabilities of the k categories. Then, we generate n independent pseudo-
random numbers to determine in which of the k intervals they occur and count
the number of occurrences in each interval.
  Example
If we have:
Categories                      1    2    3    4    5    6
Probabilities                   0.15 0.20 0.30 0.16 0.12 0.07
Superior limits of subintervals 0.15 0.35 0.65 0.81 0.93 1.00
Then, with a software like Excel, we may use the following recipe:
Cells :   Ai     Bi             Ci                        ... Gi
Formulae :Rand() =If            =If(And                   ... =If
                  ($Ai<0.15;1;0) ($Ai>=0.15;$Ai<0.35);1;0)     ($Ai>=0.93;1;0)
After that, we will use functions such as SumIf to accumulate the observed
results by category and to calculate the estimated covariance matrix for each
simulated sample.
Another way is to use a discrete random number generator. In that case, the
categories must be labeled or relabeled with numeric values.
In the two cases, the result is a multinomial distribution with k categories.
This is equivalent, with a continuous random distribution, to simulate k
independent standardized normal distributions, or a multinormal distribution N
(0,I) having k components identically distributed and statistically
independent.
Since the counts of all categories have to sum to the number of trials, the
counts of the categories are always negatively correlated.[1]
***** Related distributions[edit] *****
    * When k = 2, the multinomial distribution is the binomial_distribution.
    * Categorical_distribution, the distribution of each trial; for k = 2, this
      is the Bernoulli_distribution.
    * The Dirichlet_distribution is the conjugate_prior of the multinomial in
      Bayesian_statistics.
    * Dirichlet-multinomial_distribution.
    * Beta-binomial_model.
    * Negative_multinomial_distribution
    * HardyâWeinberg_principle (it is a trinomial distribution with
      probabilities     (  &#x03B8;  2   , 2 &#x03B8; ( 1 &#x2212; &#x03B8; ) ,
      ( 1 &#x2212; &#x03B8;  )  2   )   {\displaystyle (\theta ^{2},2\theta (1-
      \theta ),(1-\theta )^{2})}  [(\theta ^{2},2\theta (1-\theta ),(1-\theta
      )^{2})])
***** References[edit] *****
**** Citations[edit] ****
   1. ^"1.7_-_The_Multinomial_Distribution_|_STAT_504".
      onlinecourses.science.psu.edu. Retrieved 2016-09-11.
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
**** Sources[edit] ****
    * Evans, Morton; Hastings, Nicholas; Peacock, Brian (2000). Statistical
      Distributions (3rd ed.). New York: Wiley. pp. 134â136. ISBN 0-471-
      37124-6.
Weisstein,_Eric_W. "Multinomial_Distribution". MathWorld. Wolfram_Research.
    * v
    * t
    * e
Probability_distributions
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

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Multinomial_distribution&oldid=908216476"
Categories:
    * Discrete_distributions
    * Multivariate_discrete_distributions
    * Factorial_and_binomial_topics
    * Exponential_family_distributions
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÄeÅ¡tina
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Tagalog
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 28 July 2019, at 07:52 (UTC).
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
