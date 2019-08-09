The following text has been accessed from https://en.wikipedia.org/wiki/Wishart_distribution at Fri Aug 9 02:54:44 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Wishart distribution ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
                                    Wishart
Notation   X ~ Wp(V, n)
Parameters n > p â 1 degrees_of_freedom (real)
           V > 0 scale_matrix (p Ã p pos._def)
Support    X(p Ã p) positive_definite_matrix
               f   X    (  x  ) =     |   x    |   ( n &#x2212; p &#x2212; 1 )
           /  2    e  &#x2212; tr &#x2061; (   V   &#x2212; 1    x  )  /  2
           2    n p  2     |    V     |   n  /  2    &#x0393;  p   (   n 2   )
           {\displaystyle f_{\mathbf {X} }(\mathbf {x} )={\frac {|\mathbf {x}
           |^{(n-p-1)/2}e^{-\operatorname {tr} (\mathbf {V} ^{-1}\mathbf {x} )/
PDF        2}}{2^{\frac {np}{2}}|{\mathbf {V} }|^{n/2}\Gamma _{p}({\frac {n}
           {2}})}}}  [{\displaystyle f_{\mathbf {X} }(\mathbf {x} )={\frac
           {|\mathbf {x} |^{(n-p-1)/2}e^{-\operatorname {tr} (\mathbf {V} ^{-
           1}\mathbf {x} )/2}}{2^{\frac {np}{2}}|{\mathbf {V} }|^{n/2}\Gamma _
           {p}({\frac {n}{2}})}}}]
               * Îp is the multivariate_gamma_function
               * tr is the trace function
              E &#x2061; [ X ] = n   V     {\displaystyle \operatorname {E}
Mean       [X]=n{\mathbf {V} }}  [{\displaystyle \operatorname {E} [X]=n
           {\mathbf {V} }}]
Mode       (n â p â 1)V for n â¥ p + 1
              Var &#x2061; (   X   i j   ) = n  (   v  i j   2   +  v  i i    v
Variance   j j    )    {\displaystyle \operatorname {Var} (\mathbf {X} _
           {ij})=n\left(v_{ij}^{2}+v_{ii}v_{jj}\right)}  [\operatorname{Var}
           (\mathbf{X}_{ij}) = n \left (v_{ij}^2+v_{ii}v_{jj} \right )]
Entropy    see_below
              &#x0398; &#x21A6;   |    I   &#x2212; 2 i    &#x0398;     V    |
           &#x2212;   n 2       {\displaystyle \Theta \mapsto \left|{\mathbf
CF         {I} }-2i\,{\mathbf {\Theta } }{\mathbf {V} }\right|^{-{\frac {n}
           {2}}}}  [\Theta \mapsto \left|{\mathbf I} - 2i\,{\mathbf\Theta}
           {\mathbf V}\right|^{-\frac{n}{2}}]
In statistics, the Wishart distribution is a generalization to multiple
dimensions of the gamma_distribution. It is named in honor of John_Wishart, who
first formulated the distribution in 1928.[1]
It is a family of probability_distributions defined over symmetric,
nonnegative-definite matrix-valued random_variables (ârandom matricesâ).
These distributions are of great importance in the estimation_of_covariance
matrices in multivariate_statistics. In Bayesian_statistics, the Wishart
distribution is the conjugate_prior of the inverse covariance-matrix of a
multivariate-normal_random-vector.[2]
⁰
***** Contents *****
    * 1_Definition
    * 2_Occurrence
    * 3_Probability_density_function
    * 4_Use_in_Bayesian_statistics
          o 4.1_Choice_of_parameters
    * 5_Properties
          o 5.1_Log-expectation
          o 5.2_Log-variance
          o 5.3_Entropy
          o 5.4_Cross-entropy
          o 5.5_KL-divergence
          o 5.6_Characteristic_function
    * 6_Theorem
          o 6.1_Corollary_1
          o 6.2_Corollary_2
    * 7_Estimator_of_the_multivariate_normal_distribution
    * 8_Bartlett_decomposition
    * 9_Marginal_distribution_of_matrix_elements
    * 10_The_range_of_the_shape_parameter
    * 11_Relationships_to_other_distributions
    * 12_See_also
    * 13_References
    * 14_External_links
***** Definition[edit] *****
Suppose G is a p Ã n matrix, each column of which is independently drawn from
a p-variate_normal_distribution with zero mean:
          G  ( i )   = (  g  i   1   , &#x2026; ,  g  i   p    )  T   &#x223C;
      N  p   ( 0 , V ) .   {\displaystyle G_{(i)}=(g_{i}^{1},\dots ,g_{i}^{p})^
      {T}\sim N_{p}(0,V).}  [{\displaystyle G_{(i)}=(g_{i}^{1},\dots ,g_{i}^
      {p})^{T}\sim N_{p}(0,V).}]
Then the Wishart distribution is the probability_distribution of the p Ã p
random matrix [3]
         S = G  G  T   =  &#x2211;  i = 1   n    G  ( i )    G  ( i )   T
      {\displaystyle S=GG^{T}=\sum _{i=1}^{n}G_{(i)}G_{(i)}^{T}}  [
      {\displaystyle S=GG^{T}=\sum _{i=1}^{n}G_{(i)}G_{(i)}^{T}}]
known as the scatter_matrix. One indicates that S has that probability
distribution by writing
         S &#x223C;  W  p   ( V , n ) .   {\displaystyle S\sim W_{p}(V,n).}
      [S\sim W_p(V,n).]
The positive integer n is the number of degrees_of_freedom. Sometimes this is
written W(V, p, n). For n â¥ p the matrix S is invertible with probability 1
if V is invertible.
If p = V = 1 then this distribution is a chi-squared_distribution with n
degrees of freedom.
***** Occurrence[edit] *****
The Wishart distribution arises as the distribution of the sample covariance
matrix for a sample from a multivariate_normal_distribution. It occurs
frequently in likelihood-ratio_tests in multivariate statistical analysis. It
also arises in the spectral theory of random_matrices[citation_needed] and in
multidimensional Bayesian analysis.[4] It is also encountered in wireless
communications, while analyzing the performance of Rayleigh_fading MIMO
wireless channels .[5]
***** Probability density function[edit] *****
The Wishart distribution can be characterized by its probability_density
function as follows:
Let X be a p Ã p symmetric matrix of random variables that is positive
definite. Let V be a (fixed) symmetric positive definite matrix of size p Ã p.
Then, if n â¥ p, X has a Wishart distribution with n degrees of freedom if it
has the probability_density_function
          f   X    (  x  ) =   1   2  n p  /  2     |   V   |   n  /  2
      &#x0393;  p    (   n 2   )        |  x  |    ( n &#x2212; p &#x2212; 1 )
      /  2    e  &#x2212; ( 1  /  2 ) tr &#x2061; (    V    &#x2212; 1    x  )
      {\displaystyle f_{\mathbf {X} }(\mathbf {x} )={\frac {1}{2^{np/2}\left|
      {\mathbf {V} }\right|^{n/2}\Gamma _{p}\left({\frac {n}{2}}\right)}}
      {\left|\mathbf {x} \right|}^{(n-p-1)/2}e^{-(1/2)\operatorname {tr} (
      {\mathbf {V} }^{-1}\mathbf {x} )}}  [{\displaystyle f_{\mathbf {X} }
      (\mathbf {x} )={\frac {1}{2^{np/2}\left|{\mathbf {V} }\right|^{n/2}\Gamma
      _{p}\left({\frac {n}{2}}\right)}}{\left|\mathbf {x} \right|}^{(n-p-1)/
      2}e^{-(1/2)\operatorname {tr} ({\mathbf {V} }^{-1}\mathbf {x} )}}]
where      |   x   |    {\displaystyle \left|{\mathbf {x} }\right|}  [
{\displaystyle \left|{\mathbf {x} }\right|}] is the determinant of      x
{\displaystyle \mathbf {x} }  [\mathbf {x} ] and Îp is the multivariate_gamma
function defined as
          &#x0393;  p    (   n 2   )  =  &#x03C0;  p ( p &#x2212; 1 )  /  4
      &#x220F;  j = 1   p   &#x0393;  (    n 2   &#x2212;    j &#x2212; 1  2
      )  .   {\displaystyle \Gamma _{p}\left({\frac {n}{2}}\right)=\pi ^{p(p-
      1)/4}\prod _{j=1}^{p}\Gamma \left({\frac {n}{2}}-{\frac {j-1}
      {2}}\right).}  [{\displaystyle \Gamma _{p}\left({\frac {n}{2}}\right)=\pi
      ^{p(p-1)/4}\prod _{j=1}^{p}\Gamma \left({\frac {n}{2}}-{\frac {j-1}
      {2}}\right).}]
The density above is not the joint density of all the      p  2
{\displaystyle p^{2}}  [p^{2}] elements of the random matrix X (such      p  2
{\displaystyle p^{2}}  [p^{2}]-dimensional density does not exists because of
the symmetry constrains      X  i j   =  X  j i     {\displaystyle X_{ij}=X_
{ji}}  [{\displaystyle X_{ij}=X_{ji}}]), it is rather the joint density of
p ( p + 1 )  /  2   {\displaystyle p(p+1)/2}  [p(p+1)/2] elements      X  i j
{\displaystyle X_{ij}}  [X_{ij}] for     i &#x2264; j   {\displaystyle i\leq j}
[i\leq j] ([1], page 38). Also, the density formula above applies only to
positive definite matrices      x  ;   {\displaystyle \mathbf {x} ;}  [
{\displaystyle \mathbf {x} ;}] for other matrices the density is equal to zero.
The joint-eigenvalue density for the eigenvalues      &#x03BB;  1   , &#x2026;
&#x03BB;  p   &#x2265; 0   {\displaystyle \lambda _{1},\dots \lambda _{p}\geq
0}  [{\displaystyle \lambda _{1},\dots \lambda _{p}\geq 0}] of a random matrix
X  &#x223C;  W  p   (  I  , n )   {\displaystyle \mathbf {X} \sim W_{p}(\mathbf
{I} ,n)}  [{\displaystyle \mathbf {X} \sim W_{p}(\mathbf {I} ,n)}] is [6], [7]
          c  n , p    e  &#x2212;   1 2    &#x2211;  i    &#x03BB;  i
      &#x220F;  &#x03BB;  i   ( n &#x2212; p &#x2212; 1 )  /  2    &#x220F;  i
      < j    |   &#x03BB;  i   &#x2212;  &#x03BB;  j    |    {\displaystyle c_
      {n,p}e^{-{\frac {1}{2}}\sum _{i}\lambda _{i}}\prod \lambda _{i}^{(n-p-1)/
      2}\prod _{i<j}|\lambda _{i}-\lambda _{j}|}  [{\displaystyle c_{n,p}e^{-
      {\frac {1}{2}}\sum _{i}\lambda _{i}}\prod \lambda _{i}^{(n-p-1)/2}\prod _
      {i<j}|\lambda _{i}-\lambda _{j}|}]
where      c  n , p     {\displaystyle c_{n,p}}  [{\displaystyle c_{n,p}}]is a
constant.
In fact the above definition can be extended to any real n > p â 1. If n â¤
p â 1, then the Wishart no longer has a density—instead it represents a
singular distribution that takes values in a lower-dimension subspace of the
space of p Ã p matrices.[8]
***** Use in Bayesian statistics[edit] *****
In Bayesian_statistics, in the context of the multivariate_normal_distribution,
the Wishart distribution is the conjugate prior to the precision matrix Î© =
Î£â1, where Î£ is the covariance matrix.[9]:135
**** Choice of parameters[edit] ****
The least informative, proper Wishart prior is obtained by setting n = p.
[citation_needed]
The prior mean of Wp(V, n) is nV, suggesting that a reasonable choice for V
would be nâ1Î£0, where Î£0 is some prior guess for the covariance matrix.
***** Properties[edit] *****
**** Log-expectation[edit] ****
The following formula plays a role in variational_Bayes derivations for Bayes
networks involving the Wishart distribution: [9]:693
         E &#x2061; [  ln &#x2061;  |  X  |   ] =  &#x03C8;  p    (   n 2   )
      + p  ln &#x2061; ( 2 ) + ln &#x2061;  |   V   |    {\displaystyle
      \operatorname {E} [\,\ln \left|\mathbf {X} \right|\,]=\psi _{p}\left(
      {\frac {n}{2}}\right)+p\,\ln(2)+\ln |\mathbf {V} |}  [{\displaystyle
      \operatorname {E} [\,\ln \left|\mathbf {X} \right|\,]=\psi _{p}\left(
      {\frac {n}{2}}\right)+p\,\ln(2)+\ln |\mathbf {V} |}]
where      &#x03C8;  p     {\displaystyle \psi _{p}}  [\psi _{p}] is the
multivariate digamma function (the derivative of the log of the multivariate
gamma_function).
**** Log-variance[edit] ****
The following variance computation could be of help in Bayesian statistics:
         Var &#x2061;  [   ln &#x2061;  |  X  |    ]  =  &#x2211;  i = 1   p
      &#x03C8;  1    (    n + 1 &#x2212; i  2   )    {\displaystyle
      \operatorname {Var} \left[\,\ln \left|\mathbf {X} \right|\,\right]=\sum _
      {i=1}^{p}\psi _{1}\left({\frac {n+1-i}{2}}\right)}  [{\displaystyle
      \operatorname {Var} \left[\,\ln \left|\mathbf {X} \right|\,\right]=\sum _
      {i=1}^{p}\psi _{1}\left({\frac {n+1-i}{2}}\right)}]
where      &#x03C8;  1     {\displaystyle \psi _{1}}  [\psi _{1}] is the
trigamma function. This comes up when computing the Fisher information of the
Wishart random variable.
**** Entropy[edit] ****
The information_entropy of the distribution has the following formula:[9]:693
         H &#x2061;  [    X    ]  = &#x2212; ln &#x2061;  (  B (  V  , n )  )
      &#x2212;    n &#x2212; p &#x2212; 1  2   E &#x2061;  [   ln &#x2061;  |
      X  |    ]  +    n p  2     {\displaystyle \operatorname {H} \left
      [\,\mathbf {X} \,\right]=-\ln \left(B(\mathbf {V} ,n)\right)-{\frac {n-p-
      1}{2}}\operatorname {E} \left[\,\ln \left|\mathbf {X} \right|\,\right]+
      {\frac {np}{2}}}  [{\displaystyle \operatorname {H} \left[\,\mathbf {X}
      \,\right]=-\ln \left(B(\mathbf {V} ,n)\right)-{\frac {n-p-1}
      {2}}\operatorname {E} \left[\,\ln \left|\mathbf {X} \right|\,\right]+
      {\frac {np}{2}}}]
where B(V, n) is the normalizing_constant of the distribution:
         B (  V  , n ) =   1    |  V  |   n  /  2    2  n p  /  2    &#x0393;
      p    (   n 2   )     .   {\displaystyle B(\mathbf {V} ,n)={\frac {1}
      {\left|\mathbf {V} \right|^{n/2}2^{np/2}\Gamma _{p}\left({\frac {n}
      {2}}\right)}}.}  [{\displaystyle B(\mathbf {V} ,n)={\frac {1}
      {\left|\mathbf {V} \right|^{n/2}2^{np/2}\Gamma _{p}\left({\frac {n}
      {2}}\right)}}.}]
This can be expanded as follows:
             H &#x2061;  [    X    ]     =   n 2   ln &#x2061;  |  V  |  +    n
      p  2   ln &#x2061; 2 + ln &#x2061;  &#x0393;  p    (   n 2   )  &#x2212;
      n &#x2212; p &#x2212; 1  2   E &#x2061;  [   ln &#x2061;  |  X  |    ]  +
      n p  2         =   n 2   ln &#x2061;  |  V  |  +    n p  2   ln &#x2061;
      2 + ln &#x2061;  &#x0393;  p    (   n 2   )  &#x2212;    n &#x2212; p
      &#x2212; 1  2    (   &#x03C8;  p    (   n 2   )  + p ln &#x2061; 2 + ln
      &#x2061;  |  V  |   )  +    n p  2         =   n 2   ln &#x2061;  |  V  |
      +    n p  2   ln &#x2061; 2 + ln &#x2061;  &#x0393;  p    (   n 2   )
      &#x2212;    n &#x2212; p &#x2212; 1  2    &#x03C8;  p    (   n 2   )
      &#x2212;    n &#x2212; p &#x2212; 1  2    (  p ln &#x2061; 2 + ln
      &#x2061;  |  V  |   )  +    n p  2         =    p + 1  2   ln &#x2061;  |
      V  |  +   1 2   p ( p + 1 ) ln &#x2061; 2 + ln &#x2061;  &#x0393;  p
      (   n 2   )  &#x2212;    n &#x2212; p &#x2212; 1  2    &#x03C8;  p
      (   n 2   )  +    n p  2         {\displaystyle {\begin
      {aligned}\operatorname {H} \left[\,\mathbf {X} \,\right]&={\frac {n}
      {2}}\ln \left|\mathbf {V} \right|+{\frac {np}{2}}\ln 2+\ln \Gamma _
      {p}\left({\frac {n}{2}}\right)-{\frac {n-p-1}{2}}\operatorname {E} \left
      [\,\ln \left|\mathbf {X} \right|\,\right]+{\frac {np}{2}}\\[8pt]&={\frac
      {n}{2}}\ln \left|\mathbf {V} \right|+{\frac {np}{2}}\ln 2+\ln \Gamma _
      {p}\left({\frac {n}{2}}\right)-{\frac {n-p-1}{2}}\left(\psi _{p}\left(
      {\frac {n}{2}}\right)+p\ln 2+\ln \left|\mathbf {V} \right|\right)+{\frac
      {np}{2}}\\[8pt]&={\frac {n}{2}}\ln \left|\mathbf {V} \right|+{\frac {np}
      {2}}\ln 2+\ln \Gamma _{p}\left({\frac {n}{2}}\right)-{\frac {n-p-1}
      {2}}\psi _{p}\left({\frac {n}{2}}\right)-{\frac {n-p-1}{2}}\left(p\ln
      2+\ln \left|\mathbf {V} \right|\right)+{\frac {np}{2}}\\[8pt]&={\frac
      {p+1}{2}}\ln \left|\mathbf {V} \right|+{\frac {1}{2}}p(p+1)\ln 2+\ln
      \Gamma _{p}\left({\frac {n}{2}}\right)-{\frac {n-p-1}{2}}\psi _{p}\left(
      {\frac {n}{2}}\right)+{\frac {np}{2}}\end{aligned}}}  [{\displaystyle
      {\begin{aligned}\operatorname {H} \left[\,\mathbf {X} \,\right]&={\frac
      {n}{2}}\ln \left|\mathbf {V} \right|+{\frac {np}{2}}\ln 2+\ln \Gamma _
      {p}\left({\frac {n}{2}}\right)-{\frac {n-p-1}{2}}\operatorname {E} \left
      [\,\ln \left|\mathbf {X} \right|\,\right]+{\frac {np}{2}}\\[8pt]&={\frac
      {n}{2}}\ln \left|\mathbf {V} \right|+{\frac {np}{2}}\ln 2+\ln \Gamma _
      {p}\left({\frac {n}{2}}\right)-{\frac {n-p-1}{2}}\left(\psi _{p}\left(
      {\frac {n}{2}}\right)+p\ln 2+\ln \left|\mathbf {V} \right|\right)+{\frac
      {np}{2}}\\[8pt]&={\frac {n}{2}}\ln \left|\mathbf {V} \right|+{\frac {np}
      {2}}\ln 2+\ln \Gamma _{p}\left({\frac {n}{2}}\right)-{\frac {n-p-1}
      {2}}\psi _{p}\left({\frac {n}{2}}\right)-{\frac {n-p-1}{2}}\left(p\ln
      2+\ln \left|\mathbf {V} \right|\right)+{\frac {np}{2}}\\[8pt]&={\frac
      {p+1}{2}}\ln \left|\mathbf {V} \right|+{\frac {1}{2}}p(p+1)\ln 2+\ln
      \Gamma _{p}\left({\frac {n}{2}}\right)-{\frac {n-p-1}{2}}\psi _{p}\left(
      {\frac {n}{2}}\right)+{\frac {np}{2}}\end{aligned}}}]
**** Cross-entropy[edit] ****
The cross_entropy of two Wishart distributions      p  0     {\displaystyle p_
{0}}  [p_{0}] with parameters      n  0   ,  V  0     {\displaystyle n_{0},V_
{0}}  [n_{0},V_{0}] and      p  1     {\displaystyle p_{1}}  [p_{1}] with
parameters      n  1   ,  V  1     {\displaystyle n_{1},V_{1}}  [n_{1},V_{1}]
is
             H (  p  0   ,  p  1   )    =  E   p  0     &#x2061; [  &#x2212;
      log &#x2061;  p  1    ]       =  E   p  0     &#x2061;  [   &#x2212; log
      &#x2061;      |  X  |   (  n  1   &#x2212; p &#x2212; 1 )  /  2    e
      &#x2212; tr &#x2061; (   V   1   &#x2212; 1    X  )  /  2      2   n  1
      p  /  2     |   V   1   |    n  1    /  2    &#x0393;  p    (     n  1
      2    )      ]        =      n  1   p  2    log &#x2061; 2 +     n  1   2
      log &#x2061;  |   V   1   |  + log &#x2061;  &#x0393;  p   (     n  1   2
      ) &#x2212;      n  1   &#x2212; p &#x2212; 1  2     E   p  0     &#x2061;
      [   log &#x2061;  |  X  |    ]  +    1 2     E   p  0     &#x2061;
      [   tr &#x2061;  (     V   1   &#x2212; 1    X    )    ]        =      n
      1   p  2    log &#x2061; 2 +     n  1   2    log &#x2061;  |   V   1   |
      + log &#x2061;  &#x0393;  p   (     n  1   2    ) &#x2212;      n  1
      &#x2212; p &#x2212; 1  2     (   &#x03C8;  p   (     n  0   2    ) + p
      log &#x2061; 2 + log &#x2061;  |   V   0   |   )  +    1 2    tr &#x2061;
      (     V   1   &#x2212; 1    n  0     V   0     )        = &#x2212;     n
      1   2    log &#x2061;  |     V   1   &#x2212; 1     V   0     |  +     p
      + 1  2    log &#x2061;  |   V   0   |  +     n  0   2    tr &#x2061;
      (     V   1   &#x2212; 1     V   0    )  + log &#x2061;  &#x0393;  p
      (     n  1   2    )  &#x2212;      n  1   &#x2212; p &#x2212; 1  2
      &#x03C8;  p   (     n  0   2    ) +     p ( p + 1 )  2    log &#x2061; 2
      {\displaystyle {\begin{aligned}H(p_{0},p_{1})&=\operatorname {E} _{p_{0}}
      [\,-\log p_{1}\,]\\[8pt]&=\operatorname {E} _{p_{0}}\left[\,-\log {\frac
      {\left|\mathbf {X} \right|^{(n_{1}-p-1)/2}e^{-\operatorname {tr} (\mathbf
      {V} _{1}^{-1}\mathbf {X} )/2}}{2^{n_{1}p/2}\left|\mathbf {V} _{1}\right|^
      {n_{1}/2}\Gamma _{p}\left({\tfrac {n_{1}}{2}}\right)}}\right]\\[8pt]&=
      {\tfrac {n_{1}p}{2}}\log 2+{\tfrac {n_{1}}{2}}\log \left|\mathbf {V} _
      {1}\right|+\log \Gamma _{p}({\tfrac {n_{1}}{2}})-{\tfrac {n_{1}-p-1}
      {2}}\operatorname {E} _{p_{0}}\left[\,\log \left|\mathbf {X}
      \right|\,\right]+{\tfrac {1}{2}}\operatorname {E} _{p_{0}}\left
      [\,\operatorname {tr} \left(\,\mathbf {V} _{1}^{-1}\mathbf {X}
      \,\right)\,\right]\\[8pt]&={\tfrac {n_{1}p}{2}}\log 2+{\tfrac {n_{1}}
      {2}}\log \left|\mathbf {V} _{1}\right|+\log \Gamma _{p}({\tfrac {n_{1}}
      {2}})-{\tfrac {n_{1}-p-1}{2}}\left(\psi _{p}({\tfrac {n_{0}}{2}})+p\log
      2+\log \left|\mathbf {V} _{0}\right|\right)+{\tfrac {1}{2}}\operatorname
      {tr} \left(\,\mathbf {V} _{1}^{-1}n_{0}\mathbf {V} _{0}\,\right)\\
      [8pt]&=-{\tfrac {n_{1}}{2}}\log \left|\,\mathbf {V} _{1}^{-1}\mathbf {V}
      _{0}\,\right|+{\tfrac {p+1}{2}}\log \left|\mathbf {V} _{0}\right|+{\tfrac
      {n_{0}}{2}}\operatorname {tr} \left(\,\mathbf {V} _{1}^{-1}\mathbf {V} _
      {0}\right)+\log \Gamma _{p}\left({\tfrac {n_{1}}{2}}\right)-{\tfrac {n_
      {1}-p-1}{2}}\psi _{p}({\tfrac {n_{0}}{2}})+{\tfrac {p(p+1)}{2}}\log 2\end
      {aligned}}}  [{\displaystyle {\begin{aligned}H(p_{0},p_
      {1})&=\operatorname {E} _{p_{0}}[\,-\log p_{1}\,]\\[8pt]&=\operatorname
      {E} _{p_{0}}\left[\,-\log {\frac {\left|\mathbf {X} \right|^{(n_{1}-p-1)/
      2}e^{-\operatorname {tr} (\mathbf {V} _{1}^{-1}\mathbf {X} )/2}}{2^{n_
      {1}p/2}\left|\mathbf {V} _{1}\right|^{n_{1}/2}\Gamma _{p}\left({\tfrac
      {n_{1}}{2}}\right)}}\right]\\[8pt]&={\tfrac {n_{1}p}{2}}\log 2+{\tfrac
      {n_{1}}{2}}\log \left|\mathbf {V} _{1}\right|+\log \Gamma _{p}({\tfrac
      {n_{1}}{2}})-{\tfrac {n_{1}-p-1}{2}}\operatorname {E} _{p_{0}}\left
      [\,\log \left|\mathbf {X} \right|\,\right]+{\tfrac {1}{2}}\operatorname
      {E} _{p_{0}}\left[\,\operatorname {tr} \left(\,\mathbf {V} _{1}^{-
      1}\mathbf {X} \,\right)\,\right]\\[8pt]&={\tfrac {n_{1}p}{2}}\log 2+
      {\tfrac {n_{1}}{2}}\log \left|\mathbf {V} _{1}\right|+\log \Gamma _{p}(
      {\tfrac {n_{1}}{2}})-{\tfrac {n_{1}-p-1}{2}}\left(\psi _{p}({\tfrac {n_
      {0}}{2}})+p\log 2+\log \left|\mathbf {V} _{0}\right|\right)+{\tfrac {1}
      {2}}\operatorname {tr} \left(\,\mathbf {V} _{1}^{-1}n_{0}\mathbf {V} _
      {0}\,\right)\\[8pt]&=-{\tfrac {n_{1}}{2}}\log \left|\,\mathbf {V} _{1}^{-
      1}\mathbf {V} _{0}\,\right|+{\tfrac {p+1}{2}}\log \left|\mathbf {V} _
      {0}\right|+{\tfrac {n_{0}}{2}}\operatorname {tr} \left(\,\mathbf {V} _
      {1}^{-1}\mathbf {V} _{0}\right)+\log \Gamma _{p}\left({\tfrac {n_{1}}
      {2}}\right)-{\tfrac {n_{1}-p-1}{2}}\psi _{p}({\tfrac {n_{0}}{2}})+{\tfrac
      {p(p+1)}{2}}\log 2\end{aligned}}}]
Note that when      p  0   =  p  1     {\displaystyle p_{0}=p_{1}}  [p_{0}=p_
{1}] we recover the entropy.
**** KL-divergence[edit] ****
The KullbackâLeibler_divergence of      p  1     {\displaystyle p_{1}}  [p_
{1}] from      p  0     {\displaystyle p_{0}}  [p_{0}] is
              D  K L   (  p  0   &#x2016;  p  1   )    = H (  p  0   ,  p  1
      ) &#x2212; H (  p  0   )       = &#x2212;    n  1   2   log &#x2061;  |
      V   1   &#x2212; 1     V   0    |  +    n  0   2   ( tr &#x2061; (   V
      1   &#x2212; 1     V   0   ) &#x2212; p ) + log &#x2061;     &#x0393;  p
      (    n  1   2   )     &#x0393;  p    (    n  0   2   )     +      n  0
      &#x2212;  n  1    2     &#x03C8;  p    (    n  0   2   )
      {\displaystyle {\begin{aligned}D_{KL}(p_{0}\|p_{1})&=H(p_{0},p_{1})-H(p_
      {0})\\[6pt]&=-{\frac {n_{1}}{2}}\log |\mathbf {V} _{1}^{-1}\mathbf {V} _
      {0}|+{\frac {n_{0}}{2}}(\operatorname {tr} (\mathbf {V} _{1}^{-1}\mathbf
      {V} _{0})-p)+\log {\frac {\Gamma _{p}\left({\frac {n_{1}}{2}}\right)}
      {\Gamma _{p}\left({\frac {n_{0}}{2}}\right)}}+{\tfrac {n_{0}-n_{1}}
      {2}}\psi _{p}\left({\frac {n_{0}}{2}}\right)\end{aligned}}}  [
      {\displaystyle {\begin{aligned}D_{KL}(p_{0}\|p_{1})&=H(p_{0},p_{1})-H(p_
      {0})\\[6pt]&=-{\frac {n_{1}}{2}}\log |\mathbf {V} _{1}^{-1}\mathbf {V} _
      {0}|+{\frac {n_{0}}{2}}(\operatorname {tr} (\mathbf {V} _{1}^{-1}\mathbf
      {V} _{0})-p)+\log {\frac {\Gamma _{p}\left({\frac {n_{1}}{2}}\right)}
      {\Gamma _{p}\left({\frac {n_{0}}{2}}\right)}}+{\tfrac {n_{0}-n_{1}}
      {2}}\psi _{p}\left({\frac {n_{0}}{2}}\right)\end{aligned}}}]
**** Characteristic function[edit] ****
The characteristic_function of the Wishart distribution is
         &#x0398; &#x21A6;   |     I   &#x2212; 2 i    &#x0398;      V     |
      &#x2212; n  /  2   .   {\displaystyle \Theta \mapsto \left|\,{\mathbf {I}
      }-2i\,{\mathbf {\Theta } }\,{\mathbf {V} }\,\right|^{-n/2}.}  [
      {\displaystyle \Theta \mapsto \left|\,{\mathbf {I} }-2i\,{\mathbf {\Theta
      } }\,{\mathbf {V} }\,\right|^{-n/2}.}]
In other words,
         &#x0398; &#x21A6; E &#x2061;  [   exp &#x2061;  (   i tr &#x2061;
      (    X    &#x0398;     )    )    ]  =   |     I   &#x2212; 2 i
      &#x0398;      V     |   &#x2212; n  /  2     {\displaystyle \Theta
      \mapsto \operatorname {E} \left[\,\exp \left(\,i\operatorname {tr} \left
      (\,\mathbf {X} {\mathbf {\Theta } }\,\right)\,\right)\,\right]=\left|\,
      {\mathbf {I} }-2i\,{\mathbf {\Theta } }\,{\mathbf {V} }\,\right|^{-n/2}}
      [{\displaystyle \Theta \mapsto \operatorname {E} \left[\,\exp \left
      (\,i\operatorname {tr} \left(\,\mathbf {X} {\mathbf {\Theta }
      }\,\right)\,\right)\,\right]=\left|\,{\mathbf {I} }-2i\,{\mathbf {\Theta
      } }\,{\mathbf {V} }\,\right|^{-n/2}}]
where E[â] denotes expectation. (Here Î and I are matrices the same size as
V(I is the identity_matrix); and i is the square root of â1).[7]
Since the determinant's range contains a closed line through the origin for
matrix dimensions greater than two, the above formula is only correct for small
values of the Fourier variable. (see https://arxiv.org/pdf/1901.09347.pdf)
***** Theorem[edit] *****
If a p Ã p random matrix X has a Wishart distribution with m degrees of
freedom and variance matrix V â write      X  &#x223C;    W    p   (   V   ,
m )   {\displaystyle \mathbf {X} \sim {\mathcal {W}}_{p}({\mathbf {V} },m)}
[\mathbf{X}\sim\mathcal{W}_p({\mathbf V},m)] â and C is a q Ã p matrix of
rank q, then [10]
          C   X     C    T   &#x223C;    W    q    (    C     V      C    T   ,
      m  )  .   {\displaystyle \mathbf {C} \mathbf {X} {\mathbf {C} }^{T}\sim
      {\mathcal {W}}_{q}\left({\mathbf {C} }{\mathbf {V} }{\mathbf {C} }^
      {T},m\right).}  [\mathbf{C}\mathbf{X}{\mathbf C}^T \sim \mathcal
      {W}_q\left({\mathbf C}{\mathbf V}{\mathbf C}^T,m\right).]
**** Corollary 1[edit] ****
If z is a nonzero p Ã 1 constant vector, then:[10]
            z    T    X    z   &#x223C;  &#x03C3;  z   2    &#x03C7;  m   2   .
      {\displaystyle {\mathbf {z} }^{T}\mathbf {X} {\mathbf {z} }\sim \sigma _
      {z}^{2}\chi _{m}^{2}.}  [{\mathbf z}^T\mathbf{X}{\mathbf
      z}\sim\sigma_z^2\chi_m^2.]
In this case,      &#x03C7;  m   2     {\displaystyle \chi _{m}^{2}}
[\chi_m^2] is the chi-squared_distribution and      &#x03C3;  z   2   =    z
T     V     z     {\displaystyle \sigma _{z}^{2}={\mathbf {z} }^{T}{\mathbf {V}
}{\mathbf {z} }}  [\sigma_z^2={\mathbf z}^T{\mathbf V}{\mathbf z}] (note that
&#x03C3;  z   2     {\displaystyle \sigma _{z}^{2}}  [\sigma_z^2] is a
constant; it is positive because V is positive definite).
**** Corollary 2[edit] ****
Consider the case where zT = (0, ..., 0, 1, 0, ..., 0) (that is, the j-th
element is one and all others zero). Then corollary 1 above shows that
          w  j j   &#x223C;  &#x03C3;  j j    &#x03C7;  m   2
      {\displaystyle w_{jj}\sim \sigma _{jj}\chi _{m}^{2}}  [w_{jj}\sim\sigma_
      {jj}\chi^2_m]
gives the marginal distribution of each of the elements on the matrix's
diagonal.
George_Seber points out that the Wishart distribution is not called the
âmultivariate chi-squared distributionâ because the marginal distribution
of the off-diagonal_elements is not chi-squared. Seber prefers to reserve the
term multivariate for the case when all univariate marginals belong to the same
family.[11]
***** Estimator of the multivariate normal distribution[edit] *****
The Wishart distribution is the sampling_distribution of the maximum-likelihood
estimator (MLE) of the covariance_matrix of a multivariate_normal_distribution.
[12] A derivation_of_the_MLE uses the spectral_theorem.
***** Bartlett decomposition[edit] *****
The Bartlett decomposition of a matrix X from a p-variate Wishart distribution
with scale matrix V and n degrees of freedom is the factorization:
          X  =   L     A      A    T      L    T   ,   {\displaystyle \mathbf
      {X} ={\textbf {L}}{\textbf {A}}{\textbf {A}}^{T}{\textbf {L}}^{T},}
      [\mathbf{X} = {\textbf L}{\textbf A}{\textbf A}^T{\textbf L}^T,]
where L is the Cholesky_factor of V, and:
          A  =   (     c  1     0   0   &#x22EF;   0      n  21      c  2     0
      &#x22EF;   0      n  31      n  32      c  3     &#x22EF;   0
      &#x22EE;   &#x22EE;   &#x22EE;   &#x22F1;   &#x22EE;      n  p 1      n
      p 2      n  p 3     &#x22EF;    c  p      )     {\displaystyle \mathbf
      {A} ={\begin{pmatrix}c_{1}&0&0&\cdots &0\\n_{21}&c_{2}&0&\cdots &0\\n_
      {31}&n_{32}&c_{3}&\cdots &0\\\vdots &\vdots &\vdots &\ddots &\vdots \\n_
      {p1}&n_{p2}&n_{p3}&\cdots &c_{p}\end{pmatrix}}}  [\mathbf A = \begin
      {pmatrix}
      c_1 & 0 & 0 & \cdots & 0\\
      n_{21} & c_2 &0 & \cdots& 0 \\
      n_{31} & n_{32} & c_3 & \cdots & 0\\
      \vdots & \vdots & \vdots &\ddots & \vdots \\
      n_{p1} & n_{p2} & n_{p3} &\cdots & c_p
      \end{pmatrix}]
where      c  i   2   &#x223C;  &#x03C7;  n &#x2212; i + 1   2
{\displaystyle c_{i}^{2}\sim \chi _{n-i+1}^{2}}  [c_i^2 \sim \chi^2_{n-i+1}]
and nij ~ N(0, 1) independently.[13] This provides a useful method for
obtaining random samples from a Wishart distribution.[14]
***** Marginal distribution of matrix elements[edit] *****
Let V be a 2 Ã 2 variance matrix characterized by correlation_coefficient â1
< Ï < 1 and L its lower Cholesky factor:
          V  =   (     &#x03C3;  1   2     &#x03C1;  &#x03C3;  1    &#x03C3;  2
      &#x03C1;  &#x03C3;  1    &#x03C3;  2      &#x03C3;  2   2      )   ,   L
      =   (     &#x03C3;  1     0     &#x03C1;  &#x03C3;  2       1 &#x2212;
      &#x03C1;  2      &#x03C3;  2      )     {\displaystyle \mathbf {V} =
      {\begin{pmatrix}\sigma _{1}^{2}&\rho \sigma _{1}\sigma _{2}\\\rho \sigma
      _{1}\sigma _{2}&\sigma _{2}^{2}\end{pmatrix}},\qquad \mathbf {L} ={\begin
      {pmatrix}\sigma _{1}&0\\\rho \sigma _{2}&{\sqrt {1-\rho ^{2}}}\sigma _
      {2}\end{pmatrix}}}  [\mathbf{V} = \begin{pmatrix}
      \sigma_1^2 & \rho \sigma_1 \sigma_2 \\
      \rho \sigma_1 \sigma_2 & \sigma_2^2
      \end{pmatrix},
      \qquad
      \mathbf{L} = \begin{pmatrix}
      \sigma_1 & 0 \\
      \rho \sigma_2 & \sqrt{1-\rho^2} \sigma_2
      \end{pmatrix}]
Multiplying through the Bartlett decomposition above, we find that a random
sample from the 2 Ã 2 Wishart distribution is
          X  =   (     &#x03C3;  1   2    c  1   2      &#x03C3;  1    &#x03C3;
      2    (  &#x03C1;  c  1   2   +   1 &#x2212;  &#x03C1;  2      c  1    n
      21    )       &#x03C3;  1    &#x03C3;  2    (  &#x03C1;  c  1   2   +   1
      &#x2212;  &#x03C1;  2      c  1    n  21    )     &#x03C3;  2   2    (
      (  1 &#x2212;  &#x03C1;  2    )   c  2   2   +   (    1 &#x2212;
      &#x03C1;  2      n  21   + &#x03C1;  c  1    )   2    )     )
      {\displaystyle \mathbf {X} ={\begin{pmatrix}\sigma _{1}^{2}c_{1}^
      {2}&\sigma _{1}\sigma _{2}\left(\rho c_{1}^{2}+{\sqrt {1-\rho ^{2}}}c_
      {1}n_{21}\right)\\\sigma _{1}\sigma _{2}\left(\rho c_{1}^{2}+{\sqrt {1-
      \rho ^{2}}}c_{1}n_{21}\right)&\sigma _{2}^{2}\left(\left(1-\rho ^
      {2}\right)c_{2}^{2}+\left({\sqrt {1-\rho ^{2}}}n_{21}+\rho c_{1}\right)^
      {2}\right)\end{pmatrix}}}  [\mathbf{X} = \begin{pmatrix}
      \sigma_1^2 c_1^2 & \sigma_1 \sigma_2 \left (\rho c_1^2 + \sqrt{1-\rho^2}
      c_1 n_{21} \right ) \\
      \sigma_1 \sigma_2 \left (\rho c_1^2 + \sqrt{1-\rho^2} c_1 n_{21} \right )
      & \sigma_2^2 \left(\left (1-\rho^2 \right ) c_2^2 + \left (\sqrt{1-
      \rho^2} n_{21} + \rho c_1 \right )^2 \right)
      \end{pmatrix}]
The diagonal elements, most evidently in the first element, follow the Ï2
distribution with n degrees of freedom (scaled by Ï2) as expected. The off-
diagonal element is less familiar but can be identified as a normal_variance-
mean_mixture where the mixing density is a Ï2 distribution. The corresponding
marginal probability density for the off-diagonal element is therefore the
variance-gamma_distribution
         f (  x  12   ) =     |  x  12   |     n &#x2212; 1  2     &#x0393;
      (   n 2   )     2  n &#x2212; 1   &#x03C0;  (  1 &#x2212;  &#x03C1;  2
      )    (   &#x03C3;  1    &#x03C3;  2    )   n + 1        &#x22C5;  K    n
      &#x2212; 1  2     (    |  x  12   |    &#x03C3;  1    &#x03C3;  2    (  1
      &#x2212;  &#x03C1;  2    )     )  exp &#x2061;   (    &#x03C1;  x  12
      &#x03C3;  1    &#x03C3;  2   ( 1 &#x2212;  &#x03C1;  2   )    )
      {\displaystyle f(x_{12})={\frac {\left|x_{12}\right|^{\frac {n-1}{2}}}
      {\Gamma \left({\frac {n}{2}}\right){\sqrt {2^{n-1}\pi \left(1-\rho ^
      {2}\right)\left(\sigma _{1}\sigma _{2}\right)^{n+1}}}}}\cdot K_{\frac {n-
      1}{2}}\left({\frac {\left|x_{12}\right|}{\sigma _{1}\sigma _{2}\left(1-
      \rho ^{2}\right)}}\right)\exp {\left({\frac {\rho x_{12}}{\sigma _
      {1}\sigma _{2}(1-\rho ^{2})}}\right)}}  [f(x_{12}) =  \frac{\left | x_
      {12} \right |^{\frac{n-1}{2}}}{\Gamma\left(\frac{n}{2}\right) \sqrt{2^{n-
      1} \pi \left (1-\rho^2 \right ) \left (\sigma_1 \sigma_2 \right )^{n+1}}}
      \cdot K_{\frac{n-1}{2}} \left(\frac{\left |x_{12} \right |}{\sigma_1
      \sigma_2 \left (1-\rho^2 \right )}\right) \exp{\left(\frac{\rho x_{12}}
      {\sigma_1 \sigma_2 (1-\rho^2)}\right)}]
where KÎ½(z) is the modified_Bessel_function_of_the_second_kind.[15] Similar
results may be found for higher dimensions, but the interdependence of the off-
diagonal correlations becomes increasingly complicated. It is also possible to
write down the moment-generating_function even in the noncentral case
(essentially the nth power of Craig (1936)[16] equation 10) although the
probability density becomes an infinite sum of Bessel functions.
***** The range of the shape parameter[edit] *****
It can be shown [17] that the Wishart distribution can be defined if and only
if the shape parameter n belongs to the set
          &#x039B;  p   := { 0 , &#x2026; , p &#x2212; 1 } &#x222A;  (  p
      &#x2212; 1 , &#x221E;  )  .   {\displaystyle \Lambda _{p}:=\{0,\ldots ,p-
      1\}\cup \left(p-1,\infty \right).}  [{\displaystyle \Lambda _{p}:=\
      {0,\ldots ,p-1\}\cup \left(p-1,\infty \right).}]
This set is named after Gindikin, who introduced it[18] in the seventies in the
context of gamma distributions on homogeneous cones. However, for the new
parameters in the discrete spectrum of the Gindikin ensemble, namely,
          &#x039B;  p   &#x2217;   := { 0 , &#x2026; , p &#x2212; 1 } ,
      {\displaystyle \Lambda _{p}^{*}:=\{0,\ldots ,p-1\},}  [{\displaystyle
      \Lambda _{p}^{*}:=\{0,\ldots ,p-1\},}]
the corresponding Wishart distribution has no Lebesgue density.
***** Relationships to other distributions[edit] *****
    * The Wishart distribution is related to the inverse-Wishart_distribution,
      denoted by      W  p   &#x2212; 1     {\displaystyle W_{p}^{-1}}  [W_p^{-
      1}], as follows: If X ~ Wp(V, n) and if we do the change of variables C =
      Xâ1, then      C  &#x223C;  W  p   &#x2212; 1   (   V   &#x2212; 1   ,
      n )   {\displaystyle \mathbf {C} \sim W_{p}^{-1}(\mathbf {V} ^{-1},n)}
      [\mathbf{C}\sim W_p^{-1}(\mathbf{V}^{-1},n)]. This relationship may be
      derived by noting that the absolute value of the Jacobian_determinant of
      this change of variables is |C|p+1, see for example equation (15.15) in.
      [19]
    * In Bayesian_statistics, the Wishart distribution is a conjugate_prior for
      the precision_parameter of the multivariate_normal_distribution, when the
      mean parameter is known.[9]
    * A generalization is the multivariate_gamma_distribution.
    * A different type of generalization is the normal-Wishart_distribution,
      essentially the product of a multivariate_normal_distribution with a
      Wishart distribution.
***** See also[edit] *****
    * Chi-squared_distribution
    * Complex_Wishart_distribution
    * F-distribution
    * Gamma_distribution
    * Hotelling's_T-squared_distribution
    * Inverse-Wishart_distribution
    * Multivariate_gamma_distribution
    * Student's_t-distribution
    * Wilks'_lambda_distribution
***** References[edit] *****
   1. ^ a bWishart,_J. (1928). "The generalised product moment distribution in
      samples from a normal multivariate population". Biometrika. 20A (1â2):
      32â52. doi:10.1093/biomet/20A.1-2.32. JFM 54.0565.02. JSTOR 2331939.
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
   3. ^Koop, Gary; Korobilis, Dimitris (2010). "Bayesian Multivariate Time
      Series Methods for Empirical Macroeconomics". Foundations and Trends in
      Econometrics. 3 (4): 267â358. doi:10.1561/0800000013.
   4. ^Gupta, A. K.; Nagar, D. K. (2000). Matrix Variate Distributions. Chapman
      & Hall /CRC. ISBN 1584880465.
   5. ^Gelman, Andrew (2003). Bayesian_Data_Analysis (2nd ed.). Boca Raton,
      Fla.: Chapman & Hall. p. 582. ISBN 158488388X. Retrieved 3 June 2015.
   6. ^Zanella, A.; Chiani, M.; Win, M.Z. (April 2009). "On the marginal
      distribution of the eigenvalues of wishart matrices". IEEE Transactions
      on Communications. 57 (4): 1050â1060. doi:10.1109/TCOMM.2009.04.070143.
   7. ^Muirhead, Robb J. (2005). Aspects of Multivariate Statistical Theory
      (2nd ed.). Wiley Interscience. ISBN 0471769851.
   8. ^ a bAnderson,_T._W. (2003). An Introduction to Multivariate Statistical
      Analysis (3rd ed.). Hoboken, N. J.: Wiley_Interscience. p. 259. ISBN 0-
      471-36091-0.
   9. ^Uhlig, H. (1994). "On Singular Wishart and Singular Multivariate Beta
      Distributions". The Annals of Statistics. 22: 395â405. doi:10.1214/aos/
      1176325375.
  10. ^ a b c dBishop, C. M. (2006). Pattern Recognition and Machine Learning.
      Springer.
  11. ^ a bRao, C. R. (1965). Linear Statistical Inference and its
      Applications. Wiley. p. 535.
  12. ^Seber, George A. F. (2004). Multivariate Observations. Wiley. ISBN 978-
      0471691211.
  13. ^Chatfield, C.; Collins, A. J. (1980). Introduction to Multivariate
      Analysis. London: Chapman and Hall. pp. 103â108. ISBN 0-412-16030-7.
  14. ^Anderson,_T._W. (2003). An Introduction to Multivariate Statistical
      Analysis (3rd ed.). Hoboken, N. J.: Wiley_Interscience. p. 257. ISBN 0-
      471-36091-0.
  15. ^Smith, W. B.; Hocking, R. R. (1972). "Algorithm AS 53: Wishart Variate
      Generator". Journal_of_the_Royal_Statistical_Society,_Series_C. 21 (3):
      341â345. JSTOR 2346290.
  16. ^Pearson,_Karl; Jeffery,_G._B.; Elderton,_Ethel_M. (December 1929). "On
      the Distribution of the First Product Moment-Coefficient, in Samples
      Drawn from an Indefinitely Large Normal Population". Biometrika.
      Biometrika Trust. 21: 164â201. doi:10.2307/2332556. JSTOR 2332556.
  17. ^Craig, Cecil C. (1936). "On_the_Frequency_Function_of_xy". Ann. Math.
      Statist. 7: 1â15. doi:10.1214/aoms/1177732541.
  18. ^Peddada and Richards, Shyamal Das; Richards, Donald St. P. (1991).
      "Proof of a Conjecture of M. L. Eaton on the Characteristic Function of
      the Wishart Distribution,". Annals_of_Probability. 19 (2): 868â874.
      doi:10.1214/aop/1176990455.
  19. ^Gindikin, S.G. (1975). "Invariant generalized functions in homogeneous
      domains,". Funct._Anal._Appl. 9 (1): 50â52. doi:10.1007/BF01078179.
  20. ^Dwyer, Paul S. (1967). "Some Applications of Matrix Derivatives in
      Multivariate Analysis". J._Amer._Statist._Assoc. 62 (318): 607â625.
      JSTOR 2283988.
***** External links[edit] *****
    * A_C++_library_for_random_matrix_generator
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
index.php?title=Wishart_distribution&oldid=908604787"
Categories:
    * Continuous_distributions
    * Multivariate_continuous_distributions
    * Covariance_and_correlation
    * Random_matrices
    * Conjugate_prior_distributions
    * Exponential_family_distributions
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_October_2010
    * Articles_with_unsourced_statements_from_June_2014
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
    * CatalÃ 
    * Deutsch
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * Nederlands
    * æ¥æ¬èª
    * SlovenÄina
    * Basa_Sunda
    * Svenska
    * ä¸­æ
Edit_links
    * This page was last edited on 30 July 2019, at 19:47 (UTC).
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
