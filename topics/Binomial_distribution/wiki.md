The following text has been accessed from https://en.wikipedia.org/wiki/Binomial_distribution at Thu Aug 8 22:52:16 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Binomial distribution ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Binomial model" redirects here. For the binomial model in options pricing, see
Binomial_options_pricing_model.
See also: Negative_binomial_distribution
                                Binomial distribution
Probability mass function
[Probability_mass_function_for_the_binomial_distribution]
Cumulative distribution function
[Cumulative_distribution_function_for_the_binomial_distribution]
Notation       B ( n , p )   {\displaystyle B(n,p)}  [B(n,p)]
               n &#x2208; { 0 , 1 , 2 , &#x2026; }   {\displaystyle n\in \
            {0,1,2,\ldots \}}  [{\displaystyle n\in \{0,1,2,\ldots \}}] – number of
Parameters  trials
               p &#x2208; [ 0 , 1 ]   {\displaystyle p\in [0,1]}  [{\displaystyle
            p\in [0,1]}] – success probability for each trial
Support        k &#x2208; { 0 , 1 , &#x2026; , n }   {\displaystyle k\in \{0,1,\ldots
            ,n\}}  [{\displaystyle k\in \{0,1,\ldots ,n\}}] – number of successes
                  (   n k   )     p  k   ( 1 &#x2212; p  )  n &#x2212; k
pmf         {\displaystyle {\binom {n}{k}}p^{k}(1-p)^{n-k}}  [{\displaystyle {\binom
            {n}{k}}p^{k}(1-p)^{n-k}}]
CDF             I  1 &#x2212; p   ( n &#x2212; k , 1 + k )   {\displaystyle I_{1-p}
            (n-k,1+k)}  [{\displaystyle I_{1-p}(n-k,1+k)}]
Mean           n p   {\displaystyle np}  [np]
               &#x230A; n p &#x230B;   {\displaystyle \lfloor np\rfloor }  [\lfloor
Median      np\rfloor ] or     &#x2308; n p &#x2309;   {\displaystyle \lceil np\rceil
            }  [\lceil np\rceil ]
               &#x230A; ( n + 1 ) p &#x230B;   {\displaystyle \lfloor (n+1)p\rfloor }
Mode        [\lfloor (n+1)p\rfloor ] or     &#x2308; ( n + 1 ) p &#x2309; &#x2212; 1
            {\displaystyle \lceil (n+1)p\rceil -1}  [{\displaystyle \lceil
            (n+1)p\rceil -1}]
Variance       n p ( 1 &#x2212; p )   {\displaystyle np(1-p)}  [np(1-p)]
Skewness          1 &#x2212; 2 p   n p ( 1 &#x2212; p )      {\displaystyle {\frac
            {1-2p}{\sqrt {np(1-p)}}}}  [{\frac {1-2p}{\sqrt {np(1-p)}}}]
Ex.               1 &#x2212; 6 p ( 1 &#x2212; p )   n p ( 1 &#x2212; p )
kurtosis    {\displaystyle {\frac {1-6p(1-p)}{np(1-p)}}}  [{\frac {1-6p(1-p)}{np(1-
            p)}}]
                 1 2    log  2   &#x2061;  (  2 &#x03C0; e n p ( 1 &#x2212; p )  )  +
            O  (   1 n   )    {\displaystyle {\frac {1}{2}}\log _{2}\left(2\pi enp(1-
Entropy     p)\right)+O\left({\frac {1}{n}}\right)}  [{\displaystyle {\frac {1}
            {2}}\log _{2}\left(2\pi enp(1-p)\right)+O\left({\frac {1}{n}}\right)}]
            in shannons. For nats, use the natural log in the log.
MGF            ( 1 &#x2212; p + p  e  t    )  n     {\displaystyle (1-p+pe^{t})^{n}}
            [{\displaystyle (1-p+pe^{t})^{n}}]
CF             ( 1 &#x2212; p + p  e  i t    )  n     {\displaystyle (1-p+pe^{it})^
            {n}}  [{\displaystyle (1-p+pe^{it})^{n}}]
PGF            G ( z ) = [ ( 1 &#x2212; p ) + p z  ]  n     {\displaystyle G(z)=[(1-
            p)+pz]^{n}}  [{\displaystyle G(z)=[(1-p)+pz]^{n}}]
Fisher          g  n   ( p ) =   n  p ( 1 &#x2212; p )      {\displaystyle g_{n}(p)=
information {\frac {n}{p(1-p)}}}  [g_{n}(p)={\frac {n}{p(1-p)}}]
            (for fixed     n   {\displaystyle n}  [n])
Binomial distribution for     p = 0.5   {\displaystyle p=0.5}  [p=0.5]
with n and k as in Pascal's_triangle

The probability that a ball in a Galton_box with 8 layers (n = 8) ends up in
the central bin (k = 4) is     70  /  256   {\displaystyle 70/256}  [70/256].
In probability_theory and statistics, the binomial distribution with parameters
n and p is the discrete_probability_distribution of the number of successes in
a sequence of n independent experiments, each asking a yesâno_question, and
each with its own boolean-valued outcome: success/yes/true/one (with
probability p) or failure/no/false/zero (with probability q = 1 â p). A
single success/failure experiment is also called a Bernoulli_trial or Bernoulli
experiment and a sequence of outcomes is called a Bernoulli_process; for a
single trial, i.e., n = 1, the binomial distribution is a Bernoulli
distribution. The binomial distribution is the basis for the popular binomial
test of statistical_significance.
The binomial distribution is frequently used to model the number of successes
in a sample of size n drawn with_replacement from a population of size N. If
the sampling is carried out without replacement, the draws are not independent
and so the resulting distribution is a hypergeometric_distribution, not a
binomial one. However, for N much larger than n, the binomial distribution
remains a good approximation, and is widely used.
⁰
***** Contents *****
    * 1_Specification
          o 1.1_Probability_mass_function
          o 1.2_Cumulative_distribution_function
    * 2_Example
    * 3_Expectation
    * 4_Variance
    * 5_Mode
    * 6_Median
    * 7_Covariance_between_two_binomials
    * 8_Related_distributions
          o 8.1_Sums_of_binomials
          o 8.2_Ratio_of_two_binomial_distributions
          o 8.3_Conditional_binomials
          o 8.4_Bernoulli_distribution
          o 8.5_Poisson_binomial_distribution
          o 8.6_Normal_approximation
          o 8.7_Poisson_approximation
          o 8.8_Limiting_distributions
          o 8.9_Beta_distribution
    * 9_Confidence_intervals
          o 9.1_Wald_method
          o 9.2_AgrestiâCoull_method
          o 9.3_Arcsine_method
          o 9.4_Wilson_(score)_method
          o 9.5_Comparison
    * 10_Generating_binomial_random_variates
    * 11_Tail_bounds
    * 12_History
    * 13_See_also
    * 14_References
    * 15_Further_reading
    * 16_External_links
***** Specification[edit] *****
**** Probability mass function[edit] ****
In general, if the random variable X follows the binomial distribution with
parameters n â â and p â [0,1], we write X ~ B(n, p). The probability of
getting exactly k successes in n trials is given by the probability_mass
function:
         f ( k , n , p ) = Pr ( k ; n , p ) = Pr ( X = k ) =    (   n k   )
      p  k   ( 1 &#x2212; p  )  n &#x2212; k     {\displaystyle f(k,n,p)=\Pr
      (k;n,p)=\Pr(X=k)={\binom {n}{k}}p^{k}(1-p)^{n-k}}  [{\displaystyle f
      (k,n,p)=\Pr(k;n,p)=\Pr(X=k)={\binom {n}{k}}p^{k}(1-p)^{n-k}}]
for k = 0, 1, 2, ..., n, where
            (   n k   )    =    n !   k ! ( n &#x2212; k ) !
      {\displaystyle {\binom {n}{k}}={\frac {n!}{k!(n-k)!}}}  [{\displaystyle
      {\binom {n}{k}}={\frac {n!}{k!(n-k)!}}}]
is the binomial_coefficient, hence the name of the distribution. The formula
can be understood as follows. k successes occur with probability pk and n â k
failures occur with probability (1 â p)n â k. However, the k successes can
occur anywhere among the n trials, and there are        (   n k   )
{\displaystyle {\binom {n}{k}}}  [{\binom {n}{k}}] different ways of
distributing k successes in a sequence of n trials.
In creating reference tables for binomial distribution probability, usually the
table is filled in up to n/2 values. This is because for k > n/2, the
probability can be calculated by its complement as
         f ( k , n , p ) = f ( n &#x2212; k , n , 1 &#x2212; p ) .
      {\displaystyle f(k,n,p)=f(n-k,n,1-p).}  [f(k,n,p)=f(n-k,n,1-p).]
Looking at the expression f(k, n, p) as a function of k, there is a k value
that maximizes it. This k value can be found by calculating
            f ( k + 1 , n , p )   f ( k , n , p )    =    ( n &#x2212; k ) p
      ( k + 1 ) ( 1 &#x2212; p )      {\displaystyle {\frac {f(k+1,n,p)}{f
      (k,n,p)}}={\frac {(n-k)p}{(k+1)(1-p)}}}  [{\frac {f(k+1,n,p)}{f(k,n,p)}}=
      {\frac {(n-k)p}{(k+1)(1-p)}}]
and comparing it to 1. There is always an integer M that satisfies
         ( n + 1 ) p &#x2212; 1 &#x2264; M < ( n + 1 ) p .   {\displaystyle
      (n+1)p-1\leq M<(n+1)p.}  [(n+1)p-1\leq M<(n+1)p.]
f(k, n, p) is monotone increasing for k < M and monotone decreasing for k > M,
with the exception of the case where (n + 1)p is an integer. In this case,
there are two values for which f is maximal: (n + 1)p and (n + 1)p â 1. M is
the most probable outcome (that is, the most likely, although this can still be
unlikely overall) of the Bernoulli trials and is called the mode.
**** Cumulative distribution function[edit] ****
The cumulative_distribution_function can be expressed as:
         F ( k ; n , p ) = Pr ( X &#x2264; k ) =  &#x2211;  i = 0   &#x230A; k
      &#x230B;      (   n i   )     p  i   ( 1 &#x2212; p  )  n &#x2212; i
      {\displaystyle F(k;n,p)=\Pr(X\leq k)=\sum _{i=0}^{\lfloor k\rfloor }{n
      \choose i}p^{i}(1-p)^{n-i}}  [F(k;n,p)=\Pr(X\leq k)=\sum _{i=0}^{\lfloor
      k\rfloor }{n \choose i}p^{i}(1-p)^{n-i}]
where     &#x230A; k &#x230B;    {\displaystyle \lfloor k\rfloor \,}  [
{\displaystyle \lfloor k\rfloor \,}] is the "floor" under k, i.e. the greatest
integer less than or equal to k.
It can also be represented in terms of the regularized_incomplete_beta
function, as follows:[1]
             F ( k ; n , p )    = Pr ( X &#x2264; k )       =  I  1 &#x2212; p
      ( n &#x2212; k , k + 1 )       = ( n &#x2212; k )    (   n k   )
      &#x222B;  0   1 &#x2212; p    t  n &#x2212; k &#x2212; 1   ( 1 &#x2212; t
      )  k    d t .       {\displaystyle {\begin{aligned}F(k;n,p)&=\Pr(X\leq
      k)\\&=I_{1-p}(n-k,k+1)\\&=(n-k){n \choose k}\int _{0}^{1-p}t^{n-k-1}(1-
      t)^{k}\,dt.\end{aligned}}}  [{\begin{aligned}F(k;n,p)&=\Pr(X\leq k)\\&=I_
      {1-p}(n-k,k+1)\\&=(n-k){n \choose k}\int _{0}^{1-p}t^{n-k-1}(1-t)^
      {k}\,dt.\end{aligned}}]
Some closed-form bounds for the cumulative distribution function are given
below.
***** Example[edit] *****
Suppose a biased_coin comes up heads with probability 0.3 when tossed. What is
the probability of achieving 0, 1,..., 6 heads after six tosses?
         Pr ( 0  &#xA0;heads  ) = f ( 0 ) = Pr ( X = 0 ) =    (   6 0   )
      0.3  0   ( 1 &#x2212; 0.3  )  6 &#x2212; 0   = 0.117649   {\displaystyle
      \Pr(0{\text{ heads}})=f(0)=\Pr(X=0)={6 \choose 0}0.3^{0}(1-0.3)^{6-
      0}=0.117649}  [{\displaystyle \Pr(0{\text{ heads}})=f(0)=\Pr(X=0)={6
      \choose 0}0.3^{0}(1-0.3)^{6-0}=0.117649}]
         Pr ( 1  &#xA0;heads  ) = f ( 1 ) = Pr ( X = 1 ) =    (   6 1   )
      0.3  1   ( 1 &#x2212; 0.3  )  6 &#x2212; 1   = 0.302526   {\displaystyle
      \Pr(1{\text{ heads}})=f(1)=\Pr(X=1)={6 \choose 1}0.3^{1}(1-0.3)^{6-
      1}=0.302526}  [{\displaystyle \Pr(1{\text{ heads}})=f(1)=\Pr(X=1)={6
      \choose 1}0.3^{1}(1-0.3)^{6-1}=0.302526}]
         Pr ( 2  &#xA0;heads  ) = f ( 2 ) = Pr ( X = 2 ) =    (   6 2   )
      0.3  2   ( 1 &#x2212; 0.3  )  6 &#x2212; 2   = 0.324135   {\displaystyle
      \Pr(2{\text{ heads}})=f(2)=\Pr(X=2)={6 \choose 2}0.3^{2}(1-0.3)^{6-
      2}=0.324135}  [{\displaystyle \Pr(2{\text{ heads}})=f(2)=\Pr(X=2)={6
      \choose 2}0.3^{2}(1-0.3)^{6-2}=0.324135}]
         Pr ( 3  &#xA0;heads  ) = f ( 3 ) = Pr ( X = 3 ) =    (   6 3   )
      0.3  3   ( 1 &#x2212; 0.3  )  6 &#x2212; 3   = 0.18522   {\displaystyle
      \Pr(3{\text{ heads}})=f(3)=\Pr(X=3)={6 \choose 3}0.3^{3}(1-0.3)^{6-
      3}=0.18522}  [{\displaystyle \Pr(3{\text{ heads}})=f(3)=\Pr(X=3)={6
      \choose 3}0.3^{3}(1-0.3)^{6-3}=0.18522}]
         Pr ( 4  &#xA0;heads  ) = f ( 4 ) = Pr ( X = 4 ) =    (   6 4   )
      0.3  4   ( 1 &#x2212; 0.3  )  6 &#x2212; 4   = 0.059535   {\displaystyle
      \Pr(4{\text{ heads}})=f(4)=\Pr(X=4)={6 \choose 4}0.3^{4}(1-0.3)^{6-
      4}=0.059535}  [{\displaystyle \Pr(4{\text{ heads}})=f(4)=\Pr(X=4)={6
      \choose 4}0.3^{4}(1-0.3)^{6-4}=0.059535}]
         Pr ( 5  &#xA0;heads  ) = f ( 5 ) = Pr ( X = 5 ) =    (   6 5   )
      0.3  5   ( 1 &#x2212; 0.3  )  6 &#x2212; 5   = 0.010206   {\displaystyle
      \Pr(5{\text{ heads}})=f(5)=\Pr(X=5)={6 \choose 5}0.3^{5}(1-0.3)^{6-
      5}=0.010206}  [{\displaystyle \Pr(5{\text{ heads}})=f(5)=\Pr(X=5)={6
      \choose 5}0.3^{5}(1-0.3)^{6-5}=0.010206}]
         Pr ( 6  &#xA0;heads  ) = f ( 6 ) = Pr ( X = 6 ) =    (   6 6   )
      0.3  6   ( 1 &#x2212; 0.3  )  6 &#x2212; 6   = 0.000729   {\displaystyle
      \Pr(6{\text{ heads}})=f(6)=\Pr(X=6)={6 \choose 6}0.3^{6}(1-0.3)^{6-
      6}=0.000729}  [{\displaystyle \Pr(6{\text{ heads}})=f(6)=\Pr(X=6)={6
      \choose 6}0.3^{6}(1-0.3)^{6-6}=0.000729}][2]
***** Expectation[edit] *****
If X ~ B(n, p), that is, X is a binomially distributed random variable, n being
the total number of experiments and p the probability of each experiment
yielding a successful result, then the expected_value of X is:[3]
         E &#x2061; [ X ] = n p .   {\displaystyle \operatorname {E} [X]=np.}
      [{\displaystyle \operatorname {E} [X]=np.}]
For example, if n = 100, and p = 1/4, then the average number of successful
results will be 25.
Proof: We calculate the mean, Î¼, directly calculated from its definition
         &#x03BC; =  &#x2211;  i = 0   n    x  i    p  i   ,   {\displaystyle
      \mu =\sum _{i=0}^{n}x_{i}p_{i},}  [{\displaystyle \mu =\sum _{i=0}^{n}x_
      {i}p_{i},}]
and the binomial_theorem:
             &#x03BC;    =  &#x2211;  k = 0   n   k    (   n k   )     p  k
      ( 1 &#x2212; p  )  n &#x2212; k         = n p  &#x2211;  k = 0   n   k
      ( n &#x2212; 1 ) !   ( n &#x2212; k ) ! k !     p  k &#x2212; 1   ( 1
      &#x2212; p  )  ( n &#x2212; 1 ) &#x2212; ( k &#x2212; 1 )         = n p
      &#x2211;  k = 1   n      ( n &#x2212; 1 ) !   ( ( n &#x2212; 1 ) &#x2212;
      ( k &#x2212; 1 ) ) ! ( k &#x2212; 1 ) !     p  k &#x2212; 1   ( 1
      &#x2212; p  )  ( n &#x2212; 1 ) &#x2212; ( k &#x2212; 1 )         = n p
      &#x2211;  k = 1   n      (    n &#x2212; 1   k &#x2212; 1    )     p  k
      &#x2212; 1   ( 1 &#x2212; p  )  ( n &#x2212; 1 ) &#x2212; ( k &#x2212; 1
      )         = n p  &#x2211;  &#x2113; = 0   n &#x2212; 1      (    n
      &#x2212; 1  &#x2113;   )     p  &#x2113;   ( 1 &#x2212; p  )  ( n
      &#x2212; 1 ) &#x2212; &#x2113;       with&#xA0;  &#x2113; := k &#x2212; 1
      = n p  &#x2211;  &#x2113; = 0   m      (   m &#x2113;   )     p  &#x2113;
      ( 1 &#x2212; p  )  m &#x2212; &#x2113;       with&#xA0;  m := n &#x2212;
      1       = n p ( p + ( 1 &#x2212; p )  )  m         = n p
      {\displaystyle {\begin{aligned}\mu &=\sum _{k=0}^{n}k{\binom {n}{k}}p^{k}
      (1-p)^{n-k}\\&=np\sum _{k=0}^{n}k{\frac {(n-1)!}{(n-k)!k!}}p^{k-1}(1-p)^{
      (n-1)-(k-1)}\\&=np\sum _{k=1}^{n}{\frac {(n-1)!}{((n-1)-(k-1))!(k-1)!}}p^
      {k-1}(1-p)^{(n-1)-(k-1)}\\&=np\sum _{k=1}^{n}{\binom {n-1}{k-1}}p^{k-1}
      (1-p)^{(n-1)-(k-1)}\\&=np\sum _{\ell =0}^{n-1}{\binom {n-1}{\ell }}p^
      {\ell }(1-p)^{(n-1)-\ell }&&{\text{with }}\ell :=k-1\\&=np\sum _{\ell
      =0}^{m}{\binom {m}{\ell }}p^{\ell }(1-p)^{m-\ell }&&{\text{with }}m:=n-
      1\\&=np(p+(1-p))^{m}\\&=np\end{aligned}}}  [{\displaystyle {\begin
      {aligned}\mu &=\sum _{k=0}^{n}k{\binom {n}{k}}p^{k}(1-p)^{n-k}\\&=np\sum
      _{k=0}^{n}k{\frac {(n-1)!}{(n-k)!k!}}p^{k-1}(1-p)^{(n-1)-(k-1)}\\&=np\sum
      _{k=1}^{n}{\frac {(n-1)!}{((n-1)-(k-1))!(k-1)!}}p^{k-1}(1-p)^{(n-1)-(k-
      1)}\\&=np\sum _{k=1}^{n}{\binom {n-1}{k-1}}p^{k-1}(1-p)^{(n-1)-(k-
      1)}\\&=np\sum _{\ell =0}^{n-1}{\binom {n-1}{\ell }}p^{\ell }(1-p)^{(n-1)-
      \ell }&&{\text{with }}\ell :=k-1\\&=np\sum _{\ell =0}^{m}{\binom {m}{\ell
      }}p^{\ell }(1-p)^{m-\ell }&&{\text{with }}m:=n-1\\&=np(p+(1-p))^
      {m}\\&=np\end{aligned}}}]
It is also possible to deduce the mean from the equation     X =  X  1   +
&#x22EF; +  X  n     {\displaystyle X=X_{1}+\cdots +X_{n}}  [{\displaystyle
X=X_{1}+\cdots +X_{n}}] whereby all      X  i     {\displaystyle X_{i}}  [X_
{i}] are Bernoulli_distributed random variables with     E [  X  i   ] = p
{\displaystyle E[X_{i}]=p}  [E[X_{i}]=p] (     X  i   = 1   {\displaystyle X_
{i}=1}  [{\displaystyle X_{i}=1}] if the ith experiment succeeds and      X  i
= 0   {\displaystyle X_{i}=0}  [{\displaystyle X_{i}=0}] otherwise). We get:
E [ X ] = E [  X  1   + &#x22EF; +  X  n   ] = E [  X  1   ] + &#x22EF; + E
[  X  n   ] =     p + &#x22EF; + p  &#x23DF;    n  &#xA0;times    = n p
{\displaystyle E[X]=E[X_{1}+\cdots +X_{n}]=E[X_{1}]+\cdots +E[X_
{n}]=\underbrace {p+\cdots +p} _{n{\text{ times}}}=np}  [{\displaystyle E[X]=E
[X_{1}+\cdots +X_{n}]=E[X_{1}]+\cdots +E[X_{n}]=\underbrace {p+\cdots +p} _{n
{\text{ times}}}=np}]
***** Variance[edit] *****
The variance is:
         Var &#x2061; ( X ) = n p ( 1 &#x2212; p ) .   {\displaystyle
      \operatorname {Var} (X)=np(1-p).}  [{\displaystyle \operatorname {Var}
      (X)=np(1-p).}]
Proof: Let     X =  X  1   + &#x22EF; +  X  n     {\displaystyle X=X_{1}+\cdots
+X_{n}}  [{\displaystyle X=X_{1}+\cdots +X_{n}}] where all      X  i
{\displaystyle X_{i}}  [X_{i}] are independently Bernoulli distributed random
variables. Since     Var &#x2061; (  X  i   ) = p ( 1 &#x2212; p )
{\displaystyle \operatorname {Var} (X_{i})=p(1-p)}  [{\displaystyle
\operatorname {Var} (X_{i})=p(1-p)}], we get:
         Var &#x2061; ( X ) = Var &#x2061; (  X  1   + &#x22EF; +  X  n   ) =
      Var &#x2061; (  X  1   ) + &#x22EF; + Var &#x2061; (  X  n   ) = n Var
      &#x2061; (  X  1   ) = n p ( 1 &#x2212; p ) .   {\displaystyle
      \operatorname {Var} (X)=\operatorname {Var} (X_{1}+\cdots +X_
      {n})=\operatorname {Var} (X_{1})+\cdots +\operatorname {Var} (X_
      {n})=n\operatorname {Var} (X_{1})=np(1-p).}  [{\displaystyle
      \operatorname {Var} (X)=\operatorname {Var} (X_{1}+\cdots +X_
      {n})=\operatorname {Var} (X_{1})+\cdots +\operatorname {Var} (X_
      {n})=n\operatorname {Var} (X_{1})=np(1-p).}]
***** Mode[edit] *****
Usually the mode of a binomial B(n,âp) distribution is equal to     &#x230A;
( n + 1 ) p &#x230B;   {\displaystyle \lfloor (n+1)p\rfloor }  [\lfloor
(n+1)p\rfloor ], where     &#x230A; &#x22C5; &#x230B;   {\displaystyle \lfloor
\cdot \rfloor }  [\lfloor \cdot \rfloor ] is the floor_function. However, when
(n + 1)p is an integer and p is neither 0 nor 1, then the distribution has two
modes: (n + 1)p and (n + 1)p â 1. When p is equal to 0 or 1, the mode will be
0 and n correspondingly. These cases can be summarized as follows:
          mode  =   {    &#x230A; ( n + 1 )  p &#x230B;    if&#xA0;  ( n + 1 )
      p  &#xA0;is 0 or a noninteger  ,     ( n + 1 )  p &#xA0;  &#xA0;and&#xA0;
      &#xA0; ( n + 1 )  p &#x2212; 1    if&#xA0;  ( n + 1 ) p &#x2208; { 1 ,
      &#x2026; , n } ,     n    if&#xA0;  ( n + 1 ) p = n + 1.
      {\displaystyle {\text{mode}}={\begin{cases}\lfloor (n+1)\,p\rfloor &
      {\text{if }}(n+1)p{\text{ is 0 or a noninteger}},\\(n+1)\,p\ {\text{ and
      }}\ (n+1)\,p-1&{\text{if }}(n+1)p\in \{1,\dots ,n\},\\n&{\text{if }}
      (n+1)p=n+1.\end{cases}}}  [{\text{mode}}={\begin{cases}\lfloor
      (n+1)\,p\rfloor &{\text{if }}(n+1)p{\text{ is 0 or a noninteger}},\\
      (n+1)\,p\ {\text{ and }}\ (n+1)\,p-1&{\text{if }}(n+1)p\in \{1,\dots
      ,n\},\\n&{\text{if }}(n+1)p=n+1.\end{cases}}]
Proof: Let
         f ( k ) =    (   n k   )     p  k    q  n &#x2212; k   .
      {\displaystyle f(k)={\binom {n}{k}}p^{k}q^{n-k}.}  [{\displaystyle f(k)=
      {\binom {n}{k}}p^{k}q^{n-k}.}]
For     p = 0   {\displaystyle p=0}  [p=0] only     f ( 0 )   {\displaystyle f
(0)}  [f(0)] has a nonzero value with     f ( 0 ) = 1   {\displaystyle f(0)=1}
[f(0)=1]. For     p = 1   {\displaystyle p=1}  [p=1] we find     f ( n ) = 1
{\displaystyle f(n)=1}  [f(n)=1] and     f ( k ) = 0   {\displaystyle f(k)=0}
[f(k)=0] for     k &#x2260; n   {\displaystyle k\neq n}  [k\neq n]. This proves
that the mode is 0 for     p = 0   {\displaystyle p=0}  [p=0] and     n
{\displaystyle n}  [n] for     p = 1   {\displaystyle p=1}  [p=1].
Let     0 < p < 1   {\displaystyle 0<p<1}  [0<p<1]. We find
            f ( k + 1 )   f ( k )    =    ( n &#x2212; k ) p   ( k + 1 ) ( 1
      &#x2212; p )      {\displaystyle {\frac {f(k+1)}{f(k)}}={\frac {(n-k)p}{
      (k+1)(1-p)}}}  [{\frac {f(k+1)}{f(k)}}={\frac {(n-k)p}{(k+1)(1-p)}}].
From this follows
             k > ( n + 1 ) p &#x2212; 1 &#x21D2; f ( k + 1 ) < f ( k )     k =
      ( n + 1 ) p &#x2212; 1 &#x21D2; f ( k + 1 ) = f ( k )     k < ( n + 1 ) p
      &#x2212; 1 &#x21D2; f ( k + 1 ) > f ( k )       {\displaystyle {\begin
      {aligned}k>(n+1)p-1\Rightarrow f(k+1)<f(k)\\k=(n+1)p-1\Rightarrow f
      (k+1)=f(k)\\k<(n+1)p-1\Rightarrow f(k+1)>f(k)\end{aligned}}}  [
      {\displaystyle {\begin{aligned}k>(n+1)p-1\Rightarrow f(k+1)<f(k)\\k=
      (n+1)p-1\Rightarrow f(k+1)=f(k)\\k<(n+1)p-1\Rightarrow f(k+1)>f(k)\end
      {aligned}}}]
So when     ( n + 1 ) p &#x2212; 1   {\displaystyle (n+1)p-1}  [(n+1)p-1] is an
integer, then     ( n + 1 ) p &#x2212; 1   {\displaystyle (n+1)p-1}  [(n+1)p-1]
and     ( n + 1 ) p   {\displaystyle (n+1)p}  [(n+1)p] is a mode. In the case
that     ( n + 1 ) p &#x2212; 1 &#x2209;  Z    {\displaystyle (n+1)p-1\notin
\mathbb {Z} }  [(n+1)p-1\notin \mathbb {Z} ], then only     &#x230A; ( n + 1 )
p &#x2212; 1 &#x230B; + 1 = &#x230A; ( n + 1 ) p &#x230B;   {\displaystyle
\lfloor (n+1)p-1\rfloor +1=\lfloor (n+1)p\rfloor }  [\lfloor (n+1)p-1\rfloor
+1=\lfloor (n+1)p\rfloor ] is a mode.[4]
***** Median[edit] *****
In general, there is no single formula to find the median for a binomial
distribution, and it may even be non-unique. However several special results
have been established:
    * If np is an integer, then the mean, median, and mode coincide and equal
      np.[5][6]
    * Any median m must lie within the interval ânpâ â¤ m â¤ ânpâ.[7]
    * A median m cannot lie too far away from the mean: |m â np| â¤ min
      {âln 2, max{p, 1 â p}â}.[8]
    * The median is unique and equal to m = round(np) when |m â np| â¤ min
      {p, 1 â p} (except for the case when p = 1/2 and n is odd).[7]
    * When p = 1/2 and n is odd, any number m in the interval 1/2
      (n â 1) â¤ m â¤ 1/2(n + 1) is a median of the binomial distribution.
      If p = 1/2 and n is even, then m = n/2 is the unique median.
***** Covariance between two binomials[edit] *****
If two binomially distributed random variables X and Y are observed together,
estimating their covariance can be useful. The covariance is
         Cov &#x2061; ( X , Y ) = E &#x2061; ( X Y ) &#x2212;  &#x03BC;  X
      &#x03BC;  Y   .   {\displaystyle \operatorname {Cov} (X,Y)=\operatorname
      {E} (XY)-\mu _{X}\mu _{Y}.}  [\operatorname {Cov} (X,Y)=\operatorname {E}
      (XY)-\mu _{X}\mu _{Y}.]
In the case n = 1 (the case of Bernoulli_trials) XY is non-zero only when both
X and Y are one, and Î¼X and Î¼Y are equal to the two probabilities. Defining
pB as the probability of both happening at the same time, this gives
         Cov &#x2061; ( X , Y ) =  p  B   &#x2212;  p  X    p  Y   ,
      {\displaystyle \operatorname {Cov} (X,Y)=p_{B}-p_{X}p_{Y},}
      [\operatorname {Cov} (X,Y)=p_{B}-p_{X}p_{Y},]
and for n independent pairwise trials
         Cov &#x2061; ( X , Y  )  n   = n (  p  B   &#x2212;  p  X    p  Y   )
      .   {\displaystyle \operatorname {Cov} (X,Y)_{n}=n(p_{B}-p_{X}p_{Y}).}
      [\operatorname {Cov} (X,Y)_{n}=n(p_{B}-p_{X}p_{Y}).]
If X and Y are the same variable, this reduces to the variance formula given
above.
***** Related distributions[edit] *****
**** Sums of binomials[edit] ****
If X ~ B(n, p) and Y ~ B(m, p) are independent binomial variables with the same
probability p, then X + Y is again a binomial variable; its distribution is
Z=X+Y ~ B(n+m, p):
             P &#x2061; ( Z = k )    =  &#x2211;  i = 0   k    [     (   n i
      )     p  i   ( 1 &#x2212; p  )  n &#x2212; i    ]   [     (   m  k
      &#x2212; i    )     p  k &#x2212; i   ( 1 &#x2212; p  )  m &#x2212; k + i
      ]        =    (    n + m  k   )     p  k   ( 1 &#x2212; p  )  n + m
      &#x2212; k         {\displaystyle {\begin{aligned}\operatorname {P}
      (Z=k)&=\sum _{i=0}^{k}\left[{\binom {n}{i}}p^{i}(1-p)^{n-i}\right]\left[
      {\binom {m}{k-i}}p^{k-i}(1-p)^{m-k+i}\right]\\&={\binom {n+m}{k}}p^{k}(1-
      p)^{n+m-k}\end{aligned}}}  [{\begin{aligned}\operatorname {P} (Z=k)&=\sum
      _{i=0}^{k}\left[{\binom {n}{i}}p^{i}(1-p)^{n-i}\right]\left[{\binom {m}
      {k-i}}p^{k-i}(1-p)^{m-k+i}\right]\\&={\binom {n+m}{k}}p^{k}(1-p)^{n+m-
      k}\end{aligned}}]
However, if X and Y do not have the same probability p, then the variance of
the sum will be smaller_than_the_variance_of_a_binomial_variable distributed as
B ( n + m ,    p &#x00AF;    ) .    {\displaystyle B(n+m,{\bar {p}}).\,}  [B
(n+m,{\bar {p}}).\,]
**** Ratio of two binomial distributions[edit] ****
This result was first derived by Katz et al. in 1978.[9]
Let X ~ B(n,p1) and Y ~ B(m,p2) be independent. Let T = (X/n)/(Y/m).
Then log(T) is approximately normally distributed with mean log(p1/p2) and
variance ((1/p1) â 1)/n + ((1/p2) â 1)/m.
**** Conditional binomials[edit] ****
If X ~ B(n, p) and Y | X ~ B(X, q) (the conditional distribution of Y,
given X), then Y is a simple binomial random variable with distribution Y ~ B
(n, pq).
For example, imagine throwing n balls to a basket UX and taking the balls that
hit and throwing them to another basket UY. If p is the probability to hit UX
then X ~ B(n, p) is the number of balls that hit UX. If q is the probability to
hit UY then the number of balls that hit UY is Y ~ B(X, q) and therefore Y ~ B
(n, pq).
[Proof]
Since     X &#x223C; B ( n , p )   {\displaystyle X\sim B(n,p)}  [
{\displaystyle X\sim B(n,p)}] and     Y &#x223C; B ( X , q )   {\displaystyle
Y\sim B(X,q)}  [{\displaystyle Y\sim B(X,q)}], by the law_of_total_probability,
             Pr [ Y = m ]    =  &#x2211;  k = m   n   Pr [ Y = m &#x2223; X = k
      ] Pr [ X = k ]       =  &#x2211;  k = m   n      (   n k   )       (   k
      m   )     p  k    q  m   ( 1 &#x2212; p  )  n &#x2212; k   ( 1 &#x2212; q
      )  k &#x2212; m         {\displaystyle {\begin{aligned}\Pr[Y=m]&=\sum _
      {k=m}^{n}\Pr[Y=m\mid X=k]\Pr[X=k]\\[2pt]&=\sum _{k=m}^{n}{\binom {n}{k}}
      {\binom {k}{m}}p^{k}q^{m}(1-p)^{n-k}(1-q)^{k-m}\end{aligned}}}  [
      {\displaystyle {\begin{aligned}\Pr[Y=m]&=\sum _{k=m}^{n}\Pr[Y=m\mid
      X=k]\Pr[X=k]\\[2pt]&=\sum _{k=m}^{n}{\binom {n}{k}}{\binom {k}{m}}p^{k}q^
      {m}(1-p)^{n-k}(1-q)^{k-m}\end{aligned}}}]
Since         (   n k   )         (   k m   )     =     (   n m   )
(    n &#x2212; m   k &#x2212; m    )     ,   {\displaystyle {\tbinom {n}{k}}
{\tbinom {k}{m}}={\tbinom {n}{m}}{\tbinom {n-m}{k-m}},}  [{\displaystyle
{\tbinom {n}{k}}{\tbinom {k}{m}}={\tbinom {n}{m}}{\tbinom {n-m}{k-m}},}] the
equation above can be expressed as
         Pr [ Y = m ] =  &#x2211;  k = m   n      (   n m   )       (    n
      &#x2212; m   k &#x2212; m    )     p  k    q  m   ( 1 &#x2212; p  )  n
      &#x2212; k   ( 1 &#x2212; q  )  k &#x2212; m     {\displaystyle \Pr
      [Y=m]=\sum _{k=m}^{n}{\binom {n}{m}}{\binom {n-m}{k-m}}p^{k}q^{m}(1-p)^
      {n-k}(1-q)^{k-m}}  [{\displaystyle \Pr[Y=m]=\sum _{k=m}^{n}{\binom {n}
      {m}}{\binom {n-m}{k-m}}p^{k}q^{m}(1-p)^{n-k}(1-q)^{k-m}}]
Factoring      p  k   =  p  m    p  k &#x2212; m     {\displaystyle p^{k}=p^
{m}p^{k-m}}  [{\displaystyle p^{k}=p^{m}p^{k-m}}] and pulling all the terms
that don't depend on     k   {\displaystyle k}  [k] out of the sum now yields
             Pr [ Y = m ]    =    (   n m   )     p  m    q  m    (   &#x2211;
      k = m   n      (    n &#x2212; m   k &#x2212; m    )     p  k &#x2212; m
      ( 1 &#x2212; p  )  n &#x2212; k   ( 1 &#x2212; q  )  k &#x2212; m    )
      =    (   n m   )    ( p q  )  m    (   &#x2211;  k = m   n      (    n
      &#x2212; m   k &#x2212; m    )      (  p ( 1 &#x2212; q )  )   k &#x2212;
      m   ( 1 &#x2212; p  )  n &#x2212; k    )        {\displaystyle {\begin
      {aligned}\Pr[Y=m]&={\binom {n}{m}}p^{m}q^{m}\left(\sum _{k=m}^{n}{\binom
      {n-m}{k-m}}p^{k-m}(1-p)^{n-k}(1-q)^{k-m}\right)\\[2pt]&={\binom {n}{m}}
      (pq)^{m}\left(\sum _{k=m}^{n}{\binom {n-m}{k-m}}\left(p(1-q)\right)^{k-m}
      (1-p)^{n-k}\right)\end{aligned}}}  [{\displaystyle {\begin{aligned}\Pr
      [Y=m]&={\binom {n}{m}}p^{m}q^{m}\left(\sum _{k=m}^{n}{\binom {n-m}{k-
      m}}p^{k-m}(1-p)^{n-k}(1-q)^{k-m}\right)\\[2pt]&={\binom {n}{m}}(pq)^
      {m}\left(\sum _{k=m}^{n}{\binom {n-m}{k-m}}\left(p(1-q)\right)^{k-m}(1-
      p)^{n-k}\right)\end{aligned}}}]
After substituting     i = k &#x2212; m   {\displaystyle i=k-m}  [
{\displaystyle i=k-m}] in the expression above, we get
         Pr [ Y = m ] =    (   n m   )    ( p q  )  m    (   &#x2211;  i = 0
      n &#x2212; m      (    n &#x2212; m  i   )    ( p &#x2212; p q  )  i
      ( 1 &#x2212; p  )  n &#x2212; m &#x2212; i    )    {\displaystyle \Pr
      [Y=m]={\binom {n}{m}}(pq)^{m}\left(\sum _{i=0}^{n-m}{\binom {n-m}{i}}(p-
      pq)^{i}(1-p)^{n-m-i}\right)}  [{\displaystyle \Pr[Y=m]={\binom {n}{m}}
      (pq)^{m}\left(\sum _{i=0}^{n-m}{\binom {n-m}{i}}(p-pq)^{i}(1-p)^{n-m-
      i}\right)}]
Notice that the sum (in the parentheses) above equals     ( p &#x2212; p q + 1
&#x2212; p  )  n &#x2212; m     {\displaystyle (p-pq+1-p)^{n-m}}  [
{\displaystyle (p-pq+1-p)^{n-m}}] by the binomial_theorem. Substituting this in
finally yields
             Pr [ Y = m ]    =    (   n m   )    ( p q  )  m   ( p &#x2212; p q
      + 1 &#x2212; p  )  n &#x2212; m         =    (   n m   )    ( p q  )  m
      ( 1 &#x2212; p q  )  n &#x2212; m         {\displaystyle {\begin
      {aligned}\Pr[Y=m]&={\binom {n}{m}}(pq)^{m}(p-pq+1-p)^{n-m}\\[4pt]&=
      {\binom {n}{m}}(pq)^{m}(1-pq)^{n-m}\end{aligned}}}  [{\displaystyle
      {\begin{aligned}\Pr[Y=m]&={\binom {n}{m}}(pq)^{m}(p-pq+1-p)^{n-m}\\
      [4pt]&={\binom {n}{m}}(pq)^{m}(1-pq)^{n-m}\end{aligned}}}]
and thus     Y &#x223C; B ( n , p q )   {\displaystyle Y\sim B(n,pq)}  [
{\displaystyle Y\sim B(n,pq)}] as desired.
**** Bernoulli distribution[edit] ****
The Bernoulli_distribution is a special case of the binomial distribution,
where n = 1. Symbolically, X ~ B(1, p) has the same meaning as X ~ Bernoulli
(p). Conversely, any binomial distribution, B(n, p), is the distribution of the
sum of n Bernoulli_trials, Bernoulli(p), each with the same probability p.[10]
**** Poisson binomial distribution[edit] ****
The binomial distribution is a special case of the Poisson_binomial
distribution, or general_binomial_distribution, which is the distribution of a
sum of n independent non-identical Bernoulli_trials B(pi).[11]
**** Normal approximation[edit] ****
Binomial probability_mass_function and normal probability_density_function
approximation for n = 6 and p = 0.5
If n is large enough, then the skew of the distribution is not too great. In
this case a reasonable approximation to B(n, p) is given by the normal
distribution
           N   ( n p ,  n p ( 1 &#x2212; p ) ) ,   {\displaystyle {\mathcal
      {N}}(np,\,np(1-p)),}  [{\displaystyle {\mathcal {N}}(np,\,np(1-p)),}]
and this basic approximation can be improved in a simple way by using a
suitable continuity_correction. The basic approximation generally improves as n
increases (at least 20) and is better when p is not near to 0 or 1.[12] Various
rules_of_thumb may be used to decide whether n is large enough, and p is far
enough from the extremes of zero or one:
    * One rule[12] is that for n > 5 the normal approximation is adequate if
      the absolute value of the skewness is strictly less than 1/3; that is, if
                   |  1 &#x2212; 2 p  |    n p ( 1 &#x2212; p )    =   1  n
            |      1 &#x2212; p  p    &#x2212;    p  1 &#x2212; p       |  <
            1 3   .   {\displaystyle {\frac {|1-2p|}{\sqrt {np(1-p)}}}={\frac
            {1}{\sqrt {n}}}\left|{\sqrt {\frac {1-p}{p}}}-{\sqrt {\frac {p}{1-
            p}}}\,\right|<{\frac {1}{3}}.}  [{\displaystyle {\frac {|1-2p|}
            {\sqrt {np(1-p)}}}={\frac {1}{\sqrt {n}}}\left|{\sqrt {\frac {1-p}
            {p}}}-{\sqrt {\frac {p}{1-p}}}\,\right|<{\frac {1}{3}}.}]
    * A stronger rule states that the normal approximation is appropriate only
      if everything within 3 standard deviations of its mean is within the
      range of possible values; that is, only if
               &#x03BC; &#x00B1; 3 &#x03C3; = n p &#x00B1; 3   n p ( 1 &#x2212;
            p )   &#x2208; ( 0 , n ) .   {\displaystyle \mu \pm 3\sigma =np\pm
            3{\sqrt {np(1-p)}}\in (0,n).}  [{\displaystyle \mu \pm 3\sigma
            =np\pm 3{\sqrt {np(1-p)}}\in (0,n).}]
      This 3-standard-deviation rule is equivalent to the following conditions,
      which also imply the first rule above.
               n > 9  (    1 &#x2212; p  p   )    and   n > 9  (   p  1
            &#x2212; p    )  .   {\displaystyle n>9\left({\frac {1-p}
            {p}}\right)\quad {\text{and}}\quad n>9\left({\frac {p}{1-
            p}}\right).}  [{\displaystyle n>9\left({\frac {1-p}{p}}\right)\quad
            {\text{and}}\quad n>9\left({\frac {p}{1-p}}\right).}]
[Proof]
The rule     n p &#x00B1; 3   n p ( 1 &#x2212; p )   &#x2208; ( 0 , n )
{\displaystyle np\pm 3{\sqrt {np(1-p)}}\in (0,n)}  [{\displaystyle np\pm 3
{\sqrt {np(1-p)}}\in (0,n)}] is totally equivalent to request that
         n p &#x2212; 3   n p ( 1 &#x2212; p )   > 0   and   n p + 3   n p ( 1
      &#x2212; p )   < n .   {\displaystyle np-3{\sqrt {np(1-p)}}>0\quad {\text
      {and}}\quad np+3{\sqrt {np(1-p)}}<n.}  [{\displaystyle np-3{\sqrt {np(1-
      p)}}>0\quad {\text{and}}\quad np+3{\sqrt {np(1-p)}}<n.}]
Moving terms around yields:
         n p > 3   n p ( 1 &#x2212; p )     and   n ( 1 &#x2212; p ) > 3   n p
      ( 1 &#x2212; p )   .   {\displaystyle np>3{\sqrt {np(1-p)}}\quad {\text
      {and}}\quad n(1-p)>3{\sqrt {np(1-p)}}.}  [{\displaystyle np>3{\sqrt {np
      (1-p)}}\quad {\text{and}}\quad n(1-p)>3{\sqrt {np(1-p)}}.}]
Since     0 < p < 1   {\displaystyle 0<p<1}  [0<p<1], we can apply the square
power and divide by the respective factors     n  p  2     {\displaystyle np^
{2}}  [{\displaystyle np^{2}}] and     n ( 1 &#x2212; p  )  2
{\displaystyle n(1-p)^{2}}  [{\displaystyle n(1-p)^{2}}], to obtain the desired
conditions:
         n > 9  (    1 &#x2212; p  p   )    and   n > 9  (   p  1 &#x2212; p
      )  .   {\displaystyle n>9\left({\frac {1-p}{p}}\right)\quad {\text
      {and}}\quad n>9\left({\frac {p}{1-p}}\right).}  [{\displaystyle n>9\left(
      {\frac {1-p}{p}}\right)\quad {\text{and}}\quad n>9\left({\frac {p}{1-
      p}}\right).}]
Notice that these conditions automatically imply that     n > 9
{\displaystyle n>9}  [{\displaystyle n>9}]. On the other hand, apply again the
square root and divide by 3,
            n  3   >     1 &#x2212; p  p    > 0   and      n  3   >    p  1
      &#x2212; p     > 0.   {\displaystyle {\frac {\sqrt {n}}{3}}>{\sqrt {\frac
      {1-p}{p}}}>0\quad {\text{and}}\quad {\frac {\sqrt {n}}{3}}>{\sqrt {\frac
      {p}{1-p}}}>0.}  [{\displaystyle {\frac {\sqrt {n}}{3}}>{\sqrt {\frac {1-
      p}{p}}}>0\quad {\text{and}}\quad {\frac {\sqrt {n}}{3}}>{\sqrt {\frac {p}
      {1-p}}}>0.}]
Subtracting the second set of inequalities from the first one yields:
            n  3   >     1 &#x2212; p  p    &#x2212;    p  1 &#x2212; p     >
      &#x2212;    n  3   ;   {\displaystyle {\frac {\sqrt {n}}{3}}>{\sqrt
      {\frac {1-p}{p}}}-{\sqrt {\frac {p}{1-p}}}>-{\frac {\sqrt {n}}{3}};}  [
      {\displaystyle {\frac {\sqrt {n}}{3}}>{\sqrt {\frac {1-p}{p}}}-{\sqrt
      {\frac {p}{1-p}}}>-{\frac {\sqrt {n}}{3}};}]
and so, the desired first rule is satisfied,
          |      1 &#x2212; p  p    &#x2212;    p  1 &#x2212; p       |  <    n
      3   .   {\displaystyle \left|{\sqrt {\frac {1-p}{p}}}-{\sqrt {\frac {p}
      {1-p}}}\,\right|<{\frac {\sqrt {n}}{3}}.}  [{\displaystyle \left|{\sqrt
      {\frac {1-p}{p}}}-{\sqrt {\frac {p}{1-p}}}\,\right|<{\frac {\sqrt {n}}
      {3}}.}]
    * Another commonly used rule is that both values     n p   {\displaystyle
      np}  [np] and     n ( 1 &#x2212; p )   {\displaystyle n(1-p)}  [
      {\displaystyle n(1-p)}] must be greater than or equal to 5. However, the
      specific number varies from source to source, and depends on how good an
      approximation one wants. In particular, if one uses 9 instead of 5, the
      rule implies the results stated in the previous paragraphs.
[Proof]
Assume that both values     n p   {\displaystyle np}  [np] and     n ( 1
&#x2212; p )   {\displaystyle n(1-p)}  [{\displaystyle n(1-p)}] are greater
than 9. Since     0 < p < 1   {\displaystyle 0<p<1}  [{\displaystyle 0<p<1}],
we easily have that
         n p &#x2265; 9 > 9 ( 1 &#x2212; p )   and   n ( 1 &#x2212; p )
      &#x2265; 9 > 9 p .   {\displaystyle np\geq 9>9(1-p)\quad {\text
      {and}}\quad n(1-p)\geq 9>9p.}  [{\displaystyle np\geq 9>9(1-p)\quad
      {\text{and}}\quad n(1-p)\geq 9>9p.}]
We only have to divide now by the respective factors     p   {\displaystyle p}
[p] and     1 &#x2212; p   {\displaystyle 1-p}  [1-p], to deduce the
alternative form of the 3-standard-deviation rule:
         n > 9  (    1 &#x2212; p  p   )    and   n > 9  (   p  1 &#x2212; p
      )  .   {\displaystyle n>9\left({\frac {1-p}{p}}\right)\quad {\text
      {and}}\quad n>9\left({\frac {p}{1-p}}\right).}  [{\displaystyle n>9\left(
      {\frac {1-p}{p}}\right)\quad {\text{and}}\quad n>9\left({\frac {p}{1-
      p}}\right).}]
The following is an example of applying a continuity_correction. Suppose one
wishes to calculate Pr(X â¤ 8) for a binomial random variable X. If Y has a
distribution given by the normal approximation, then Pr(X â¤ 8) is
approximated by Pr(Y â¤ 8.5). The addition of 0.5 is the continuity
correction; the uncorrected normal approximation gives considerably less
accurate results.
This approximation, known as de_MoivreâLaplace_theorem, is a huge time-saver
when undertaking calculations by hand (exact calculations with large n are very
onerous); historically, it was the first use of the normal distribution,
introduced in Abraham_de_Moivre's book The_Doctrine_of_Chances in 1738.
Nowadays, it can be seen as a consequence of the central_limit_theorem since B
(n, p) is a sum of n independent, identically distributed Bernoulli_variables
with parameter p. This fact is the basis of a hypothesis_test, a "proportion z-
test", for the value of p using x/n, the sample proportion and estimator of p,
in a common_test_statistic.[13]
For example, suppose one randomly samples n people out of a large population
and ask them whether they agree with a certain statement. The proportion of
people who agree will of course depend on the sample. If groups of n people
were sampled repeatedly and truly randomly, the proportions would follow an
approximate normal distribution with mean equal to the true proportion p of
agreement in the population and with standard deviation     &#x03C3; =     p
( 1 &#x2212; p )  n      {\displaystyle \sigma ={\sqrt {\frac {p(1-p)}{n}}}}  [
{\displaystyle \sigma ={\sqrt {\frac {p(1-p)}{n}}}}]
**** Poisson approximation[edit] ****
The binomial distribution converges towards the Poisson_distribution as the
number of trials goes to infinity while the product np remains fixed or at
least p tends to zero. Therefore, the Poisson distribution with parameter Î» =
np can be used as an approximation to B(n, p) of the binomial distribution if n
is sufficiently large and p is sufficiently small. According to two rules of
thumb, this approximation is good if n â¥ 20 and p â¤ 0.05, or if n â¥ 100
and np â¤ 10.[14]
Concerning the accuracy of Poisson approximation, see Novak,[15] ch. 4, and
references therein.
**** Limiting distributions[edit] ****
    * Poisson_limit_theorem: As n approaches â and p approaches 0 with the
      product np held fixed, the Binomial(n, p) distribution approaches the
      Poisson_distribution with expected_value Î» = np.[14]
    * de_MoivreâLaplace_theorem: As n approaches â while p remains fixed,
      the distribution of
                  X &#x2212; n p   n p ( 1 &#x2212; p )      {\displaystyle
            {\frac {X-np}{\sqrt {np(1-p)}}}}  [{\frac {X-np}{\sqrt {np(1-p)}}}]
      approaches the normal_distribution with expected value 0 and variance 1.
      [citation_needed] This result is sometimes loosely stated by saying that
      the distribution of X is asymptotically_normal with expected value np and
      variance np(1 â p). This result is a specific case of the central_limit
      theorem.
**** Beta distribution[edit] ****
The binomial distribution and beta distribution are different views of the same
model of repeated Bernoulli trials. The binomial distribution is the PMF of k
successes given n independent events each with a probability p of success. The
beta distribution is the PDF for the probability of success p given n
independent events with k observed successes. [16] Mathematically, when
ð¼=ð+1 and ð½=ðâð+1, the beta distribution and the binomial
distribution are related by a factor of n+1:
   B e t a ( p ; &#x03B1; ; &#x03B2; ) = ( n + 1 ) B i n o m ( k ; n ; p )
{\displaystyle Beta(p;\alpha ;\beta )=(n+1)Binom(k;n;p)}
[{\displaystyle Beta(p;\alpha ;\beta )=(n+1)Binom(k;n;p)}]
Beta_distributions also provide a family of prior_probability_distributions for
binomial distributions in Bayesian_inference:[17]
         P ( p ; &#x03B1; , &#x03B2; ) =     p  &#x03B1; &#x2212; 1   ( 1
      &#x2212; p  )  &#x03B2; &#x2212; 1      B  ( &#x03B1; , &#x03B2; )    .
      {\displaystyle P(p;\alpha ,\beta )={\frac {p^{\alpha -1}(1-p)^{\beta -1}}
      {\mathrm {B} (\alpha ,\beta )}}.}  [{\displaystyle P(p;\alpha ,\beta )=
      {\frac {p^{\alpha -1}(1-p)^{\beta -1}}{\mathrm {B} (\alpha ,\beta )}}.}]
***** Confidence intervals[edit] *****
Main article: Binomial_proportion_confidence_interval
Even for quite large values of n, the actual distribution of the mean is
significantly nonnormal.[18] Because of this problem several methods to
estimate confidence intervals have been proposed.
In the equations for confidence intervals below, the variables have the
following meaning:
    * n1 is the number of successes out of n, the total number of trials
    *        p   &#x005E;    =    n  1   n     {\displaystyle {\widehat {p\,}}=
      {\frac {n_{1}}{n}}}  [{\displaystyle {\widehat {p\,}}={\frac {n_{1}}
      {n}}}] is the proportion of successes
    *    z   {\displaystyle z}  [z] is the     1 &#x2212;    1 2    &#x03B1;
      {\displaystyle 1-{\tfrac {1}{2}}\alpha }  [{\displaystyle 1-{\tfrac {1}
      {2}}\alpha }] quantile of a standard_normal_distribution (i.e., probit)
      corresponding to the target error rate     &#x03B1;   {\displaystyle
      \alpha }  [\alpha ]. For example, for a 95% confidence level the error
      &#x03B1;   {\displaystyle \alpha }  [\alpha ] = 0.05, so     1 &#x2212;
      1 2    &#x03B1;   {\displaystyle 1-{\tfrac {1}{2}}\alpha }  [
      {\displaystyle 1-{\tfrac {1}{2}}\alpha }] = 0.975 and     z
      {\displaystyle z}  [z] = 1.96.
**** Wald method[edit] ****
                   p   &#x005E;    &#x00B1; z         p   &#x005E;    ( 1
            &#x2212;     p   &#x005E;    )  n    .   {\displaystyle {\widehat
            {p\,}}\pm z{\sqrt {\frac {{\widehat {p\,}}(1-{\widehat {p\,}})}
            {n}}}.}  [{\displaystyle {\widehat {p\,}}\pm z{\sqrt {\frac {
            {\widehat {p\,}}(1-{\widehat {p\,}})}{n}}}.}]
      A continuity_correction of 0.5/n may be added.[clarification_needed]
**** AgrestiâCoull method[edit] ****
[19]
                  p &#x007E;    &#x00B1; z        p &#x007E;    ( 1 &#x2212;
            p &#x007E;    )   n +  z  2       .   {\displaystyle {\tilde
            {p}}\pm z{\sqrt {\frac {{\tilde {p}}(1-{\tilde {p}})}{n+z^{2}}}}.}
            [{\displaystyle {\tilde {p}}\pm z{\sqrt {\frac {{\tilde {p}}(1-
            {\tilde {p}})}{n+z^{2}}}}.}]
      Here the estimate of p is modified to
                  p &#x007E;    =     n  1   +   1 2    z  2     n +  z  2
            {\displaystyle {\tilde {p}}={\frac {n_{1}+{\frac {1}{2}}z^{2}}{n+z^
            {2}}}}  [{\displaystyle {\tilde {p}}={\frac {n_{1}+{\frac {1}{2}}z^
            {2}}{n+z^{2}}}}]
**** Arcsine method[edit] ****
[20]
          sin  2   &#x2061;  (  arcsin &#x2061;  (      p   &#x005E;     )
      &#x00B1;   z  2   n       )  .   {\displaystyle \sin ^{2}\left(\arcsin
      \left({\sqrt {\widehat {p\,}}}\right)\pm {\frac {z}{2{\sqrt
      {n}}}}\right).}  [{\displaystyle \sin ^{2}\left(\arcsin \left({\sqrt
      {\widehat {p\,}}}\right)\pm {\frac {z}{2{\sqrt {n}}}}\right).}]
**** Wilson (score) method[edit] ****
Main article: Binomial_proportion_confidence_interval_Â§ Wilson_score_interval
The notation in the formula below differs from the previous formulas in two
respects:[21]
    * Firstly, zx has a slightly different interpretation in the formula below:
      it has its ordinary meaning of 'the xth quantile of the standard normal
      distribution', rather than being a shorthand for 'the (1 â x)-th
      quantile'.
    * Secondly, this formula does not use a plus-minus to define the two
      bounds. Instead, one may use     z =  z  &#x03B1;  /  2
      {\displaystyle z=z_{\alpha /2}}  [{\displaystyle z=z_{\alpha /2}}] to get
      the lower bound, or use     z =  z  1 &#x2212; &#x03B1;  /  2
      {\displaystyle z=z_{1-\alpha /2}}  [{\displaystyle z=z_{1-\alpha /2}}] to
      get the upper bound. For example: for a 95% confidence level the error
      &#x03B1;   {\displaystyle \alpha }  [\alpha ] = 0.05, so one gets the
      lower bound by using     z =  z  &#x03B1;  /  2   =  z  0.025   =
      &#x2212; 1.96   {\displaystyle z=z_{\alpha /2}=z_{0.025}=-1.96}  [
      {\displaystyle z=z_{\alpha /2}=z_{0.025}=-1.96}], and one gets the upper
      bound by using     z =  z  1 &#x2212; &#x03B1;  /  2   =  z  0.975   =
      1.96   {\displaystyle z=z_{1-\alpha /2}=z_{0.975}=1.96}  [{\displaystyle
      z=z_{1-\alpha /2}=z_{0.975}=1.96}].
                      p   &#x005E;    +    z  2    2 n    + z          p
            &#x005E;    ( 1 &#x2212;     p   &#x005E;    )  n   +    z  2    4
            n  2          1 +    z  2   n        {\displaystyle {\frac {
            {\widehat {p\,}}+{\frac {z^{2}}{2n}}+z{\sqrt {{\frac {{\widehat
            {p\,}}(1-{\widehat {p\,}})}{n}}+{\frac {z^{2}}{4n^{2}}}}}}{1+{\frac
            {z^{2}}{n}}}}}  [{\displaystyle {\frac {{\widehat {p\,}}+{\frac {z^
            {2}}{2n}}+z{\sqrt {{\frac {{\widehat {p\,}}(1-{\widehat {p\,}})}
            {n}}+{\frac {z^{2}}{4n^{2}}}}}}{1+{\frac {z^{2}}{n}}}}}][22]
**** Comparison[edit] ****
The exact (ClopperâPearson) method is the most conservative.[18]
The Wald method, although commonly recommended in textbooks, is the most
biased.[clarification_needed]
***** Generating binomial random variates[edit] *****
Methods for random_number_generation where the marginal_distribution is a
binomial distribution are well-established.[23][24]
One way to generate random samples from a binomial distribution is to use an
inversion algorithm. To do so, one must calculate the probability that Pr(X =
k) for all values k from 0 through n. (These probabilities should sum to a
value close to one, in order to encompass the entire sample space.) Then by
using a pseudorandom_number_generator to generate samples uniformly between 0
and 1, one can transform the calculated samples into discrete numbers by using
the probabilities calculated in the first step.
***** Tail bounds[edit] *****
For k â¤ np, upper_bounds for the lower tail of the distribution function can
be derived. Recall that     F ( k ; n , p ) = Pr ( X &#x2264; k )
{\displaystyle F(k;n,p)=\Pr(X\leq k)}  [F(k;n,p)=\Pr(X\leq k)], the probability
that there are at most k successes.
Hoeffding's_inequality yields the bound
         F ( k ; n , p ) &#x2264; exp &#x2061;  (  &#x2212; 2    ( n p &#x2212;
      k  )  2    n    )  ,    {\displaystyle F(k;n,p)\leq \exp \left(-2{\frac {
      (np-k)^{2}}{n}}\right),\!}  [F(k;n,p)\leq \exp \left(-2{\frac {(np-k)^
      {2}}{n}}\right),\!]
and Chernoff's_inequality can be used to derive the bound
         F ( k ; n , p ) &#x2264; exp &#x2061;  (  &#x2212;   1  2  p       ( n
      p &#x2212; k  )  2    n    )  .    {\displaystyle F(k;n,p)\leq \exp \left
      (-{\frac {1}{2\,p}}{\frac {(np-k)^{2}}{n}}\right).\!}  [F(k;n,p)\leq \exp
      \left(-{\frac {1}{2\,p}}{\frac {(np-k)^{2}}{n}}\right).\!]
Moreover, these bounds are reasonably tight when p = 1/2, since the following
expression holds for all k â¥ 3n/8[25]
         F ( k ; n ,    1 2    ) &#x2264;   14 15   exp &#x2061;  (  &#x2212;
      16 (   n 2   &#x2212; k  )  2    n    )  .    {\displaystyle F(k;n,
      {\tfrac {1}{2}})\leq {\frac {14}{15}}\exp \left(-{\frac {16({\frac {n}
      {2}}-k)^{2}}{n}}\right).\!}  [{\displaystyle F(k;n,{\tfrac {1}{2}})\leq
      {\frac {14}{15}}\exp \left(-{\frac {16({\frac {n}{2}}-k)^{2}}
      {n}}\right).\!}]
However, the bounds do not work well for extreme values of p. In particular, as
p     &#x2192;   {\displaystyle \rightarrow }  [\rightarrow ] 1, value F(k;n,p)
goes to zero (for fixed k, n with k < n) while the upper bound above goes to a
positive constant. In this case a better bound is given by [26]
         F ( k ; n , p ) &#x2264; exp &#x2061;  (  &#x2212; n D  (    k n
      &#x2225; p  )   )     if&#xA0;  0 <   k n   < p   {\displaystyle F
      (k;n,p)\leq \exp \left(-nD\left({\frac {k}{n}}\parallel
      p\right)\right)\quad \quad {\text{if }}0<{\frac {k}{n}}<p}  [
      {\displaystyle F(k;n,p)\leq \exp \left(-nD\left({\frac {k}{n}}\parallel
      p\right)\right)\quad \quad {\text{if }}0<{\frac {k}{n}}<p}]
where D(a || p) is the relative_entropy between an a-coin and a p-coin (i.e.
between the Bernoulli(a) and Bernoulli(p) distribution):
         D ( a &#x2225; p ) = ( a ) log &#x2061;   a p   + ( 1 &#x2212; a ) log
      &#x2061;    1 &#x2212; a   1 &#x2212; p    .    {\displaystyle D
      (a\parallel p)=(a)\log {\frac {a}{p}}+(1-a)\log {\frac {1-a}{1-p}}.\!}  [
      {\displaystyle D(a\parallel p)=(a)\log {\frac {a}{p}}+(1-a)\log {\frac
      {1-a}{1-p}}.\!}]
Asymptotically, this bound is reasonably tight; see [26] for details. An
equivalent formulation of the bound is
         Pr ( X &#x2265; k ) = F ( n &#x2212; k ; n , 1 &#x2212; p ) &#x2264;
      exp &#x2061;  (  &#x2212; n D  (    k n   &#x2225; p  )   )     if&#xA0;
      p <   k n   < 1.    {\displaystyle \Pr(X\geq k)=F(n-k;n,1-p)\leq \exp
      \left(-nD\left({\frac {k}{n}}\parallel p\right)\right)\quad \quad {\text
      {if }}p<{\frac {k}{n}}<1.\!}  [{\displaystyle \Pr(X\geq k)=F(n-k;n,1-
      p)\leq \exp \left(-nD\left({\frac {k}{n}}\parallel p\right)\right)\quad
      \quad {\text{if }}p<{\frac {k}{n}}<1.\!}]
Both these bounds are derived directly from the Chernoff_bound. It can also be
shown that,
         Pr ( X &#x2265; k ) = F ( n &#x2212; k ; n , 1 &#x2212; p ) &#x2265;
      1  ( n + 1  )  2      exp &#x2061;  (  &#x2212; n D  (    k n   &#x2225;
      p  )   )     if&#xA0;  p <   k n   < 1.    {\displaystyle \Pr(X\geq k)=F
      (n-k;n,1-p)\geq {\frac {1}{(n+1)^{2}}}\exp \left(-nD\left({\frac {k}
      {n}}\parallel p\right)\right)\quad \quad {\text{if }}p<{\frac {k}
      {n}}<1.\!}  [{\displaystyle \Pr(X\geq k)=F(n-k;n,1-p)\geq {\frac {1}{
      (n+1)^{2}}}\exp \left(-nD\left({\frac {k}{n}}\parallel
      p\right)\right)\quad \quad {\text{if }}p<{\frac {k}{n}}<1.\!}]
This is proved using the method of types (see for example chapter 11 of
Elements of Information Theory by Cover and Thomas [27]).
We can also change the     ( n + 1  )  2     {\displaystyle (n+1)^{2}}  [(n+1)^
{2}] in the denominator to       2 n     {\displaystyle {\sqrt {2n}}}  [{\sqrt
{2n}}], by approximating the binomial coefficient with Stirling's formula.[28]
***** History[edit] *****
This distribution was derived by James_Bernoulli. He considered the case where
p = r/(r + s) where p is the probability of success and r and s are positive
integers. Blaise_Pascal had earlier considered the case where p = 1/2.
***** See also[edit] *****
    * [icon]Statistics_portal
    * Logistic_regression
    * Multinomial_distribution
    * Negative_binomial_distribution
    * Beta-binomial_distribution
    * Binomial measure, an example of a multifractal measure.[29]
    * Statistical_mechanics
***** References[edit] *****
   1. ^Wadsworth, G. P. (1960). Introduction_to_Probability_and_Random
      Variables. New York: McGraw-Hill. p. 52.
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
   3. ^ Hamilton Institute. "The_Binomial_Distribution" October 20, 2010.
   4. ^ See Proof_Wiki
   5. ^ See alsoNicolas, AndrÃ© (January 7, 2019). "Finding_mode_in_Binomial
      distribution". Stack_Exchange.
   6. ^Neumann, P. (1966). "Ãber den Median der Binomial- and
      Poissonverteilung". Wissenschaftliche Zeitschrift der Technischen
      UniversitÃ¤t Dresden (in German). 19: 29â33.
   7. ^ Lord, Nick. (July 2010). "Binomial averages when the mean is an
      integer", The_Mathematical_Gazette 94, 331-332.
   8. ^ a bKaas, R.; Buhrman, J.M. (1980). "Mean, Median and Mode in Binomial
      Distributions". Statistica Neerlandica. 34 (1): 13â18. doi:10.1111/
      j.1467-9574.1980.tb00681.x.
   9. ^Hamza, K. (1995). "The smallest uniform upper bound on the distance
      between the mean and the median of the binomial and Poisson
      distributions". Statistics & Probability Letters. 23: 21â25. doi:
      10.1016/0167-7152(94)00090-U.
  10. ^ Katz D. et al.(1978) "Obtaining confidence intervals for the risk ratio
      in cohort studies". Biometrics 34:469â474
  11. ^Taboga, Marco. "Lectures_on_Probability_Theory_and_Mathematical
      Statistics". statlect.com. Retrieved 18 December 2017.
  12. ^ Wang, Y. H. (1993). "On_the_number_of_successes_in_independent_trials"
      (PDF). Statistica Sinica. 3 (2): 295â312. Archived from the_original
      (PDF) on 2016-03-03.
  13. ^ a bBox, Hunter and Hunter (1978). Statistics for experimenters. Wiley.
      p. 130.
  14. ^ NIST/SEMATECH, "7.2.4._Does_the_proportion_of_defectives_meet
      requirements?" e-Handbook of Statistical Methods.
  15. ^ a b NIST/SEMATECH, "6.3.3.1._Counts_Control_Charts", e-Handbook of
      Statistical Methods.
  16. ^ Novak S.Y. (2011) Extreme value methods with applications to finance.
      London: CRC/ Chapman & Hall/Taylor & Francis.
  17. ISBN 9781-43983-5746.
  18. ^ https://www.statlect.com/probability-distributions/beta-distribution
  19. ^MacKay, David (2003). Information Theory, Inference and Learning
      Algorithms. Cambridge University Press; First Edition. ISBN 978-
      0521642989.
  20. ^ a bBrown, Lawrence D.; Cai, T. Tony; DasGupta, Anirban (2001),
      "Interval_Estimation_for_a_Binomial_Proportion", Statistical Science, 16
      (2): 101â133, CiteSeerX 10.1.1.323.7752, doi:10.1214/ss/1009213286,
      retrieved 2015-01-05
  21. ^Agresti, Alan; Coull, Brent A. (May 1998), "Approximate_is_better_than
      'exact'_for_interval_estimation_of_binomial_proportions" (PDF), The
      American Statistician, 52 (2): 119â126, doi:10.2307/2685469,
      JSTOR 2685469, retrieved 2015-01-05
  22. ^ Pires M. A. Confidence_intervals_for_a_binomial_proportion:_comparison
      of_methods_and_software_evaluation.
  23. ^Wilson, Edwin B. (June 1927), "Probable_inference,_the_law_of
      succession,_and_statistical_inference" (PDF), Journal of the American
      Statistical Association, 22 (158): 209â212, doi:10.2307/2276774,
      JSTOR 2276774, archived from the_original (PDF) on 2015-01-13, retrieved
      2015-01-05
  24. ^"Confidence_intervals". Engineering Statistics Handbook. NIST/Sematech.
      2012. Retrieved 2017-07-23.
  25. ^ Devroye, Luc (1986) Non-Uniform Random Variate Generation, New York:
      Springer-Verlag. (See especially Chapter_X,_Discrete_Univariate
      Distributions)
  26. ^Kachitvichyanukul, V.; Schmeiser, B. W. (1988). "Binomial random variate
      generation". Communications of the ACM. 31 (2): 216â222. doi:10.1145/
      42372.42381.
  27. ^ MatouÅ¡ek, J, Vondrak, J: The Probabilistic Method (lecture notes) [1].
  28. ^ a b R. Arratia and L. Gordon: Tutorial on large deviations for the
      binomial distribution, Bulletin of Mathematical Biology 51(1) (1989),
      125â131 [2].
  29. ^ Theorem 11.1.3 inCover, T.; Thomas, J. (2006). Elements_of_Information
      Theory (2nd ed.). Wiley. p. 350. ISBN 9781118585771.
  30. ^"Sharper_Lower_Bounds_for_Binomial/Chernoff_Tails". Stack_Exchange.
      December 7, 2015.
  31. ^ Mandelbrot, B. B., Fisher, A. J., & Calvet, L. E. (1997). A
      multifractal model of asset returns. 3.2 The Binomial Measure is the
      Simplest Example of a Multifractal
***** Further reading[edit] *****
    * Hirsch, Werner Z. (1957). "Binomial_DistributionâSuccess_or_Failure,
      How_Likely_Are_They?". Introduction to Modern Statistics. New York:
      MacMillan. pp. 140â153.
Neter, John; Wasserman, William; Whitmore, G. A. (1988). Applied Statistics
(Third ed.). Boston: Allyn & Bacon. pp. 185â192. ISBN 0-205-10328-6.
***** External links[edit] *****
 Wikimedia Commons has media related to Binomial_distributions.
    * Interactive graphic: Univariate_Distribution_Relationships
    * Binomial_distribution_formula_calculator
    * Difference of two binomial variables: X-Y or |X-Y|
    * Querying_the_binomial_probability_distribution_in_WolframAlpha
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
index.php?title=Binomial_distribution&oldid=906990039"
Categories:
    * Discrete_distributions
    * Factorial_and_binomial_topics
    * Conjugate_prior_distributions
    * Exponential_family_distributions
Hidden categories:
    * CS1_German-language_sources_(de)
    * Pages_using_deprecated_image_syntax
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_May_2012
    * Wikipedia_articles_needing_clarification_from_July_2012
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
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
    * This page was last edited on 19 July 2019, at 17:54 (UTC).
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
