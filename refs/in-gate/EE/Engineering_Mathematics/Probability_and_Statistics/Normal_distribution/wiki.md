The following text has been accessed from https://en.wikipedia.org/wiki/Normal_distribution at Thu Aug 8 22:52:02 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Normal distribution ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the univariate normal distribution. For normally
distributed vectors, see Multivariate_normal_distribution. For normally
distributed matrices, see Matrix_normal_distribution.
"Bell curve" redirects here. For other uses, see Bell_curve_(disambiguation).
                              Normal Distribution
Probability density function
[Probability_density_function_for_the_normal_distribution]
The red curve is the standard normal distribution
Cumulative distribution function
[Cumulative_distribution_function_for_the_normal_distribution]
                                 N   ( &#x03BC; ,  &#x03C3;  2   )
Notation                    {\displaystyle {\mathcal {N}}(\mu ,\sigma ^{2})}  [
                            {\mathcal {N}}(\mu ,\sigma ^{2})]
                               &#x03BC; &#x2208;  R    {\displaystyle \mu \in
                            \mathbb {R} }  [{\displaystyle \mu \in \mathbb {R}
Parameters                  }] = mean (location)
                                &#x03C3;  2   > 0   {\displaystyle \sigma ^
                            {2}>0}  [\sigma ^{2}>0] = variance (squared scale)
Support                        x &#x2208;  R    {\displaystyle x\in \mathbb {R}
                            }  [{\displaystyle x\in \mathbb {R} }]
                                 1  2 &#x03C0;  &#x03C3;  2       e  &#x2212;
                            ( x &#x2212; &#x03BC;  )  2     2  &#x03C3;  2
PDF                         {\displaystyle {\frac {1}{\sqrt {2\pi \sigma ^
                            {2}}}}e^{-{\frac {(x-\mu )^{2}}{2\sigma ^{2}}}}}  [
                            {\displaystyle {\frac {1}{\sqrt {2\pi \sigma ^
                            {2}}}}e^{-{\frac {(x-\mu )^{2}}{2\sigma ^{2}}}}}]
                                 1 2    [  1 + erf &#x2061;  (    x &#x2212;
                            &#x03BC;   &#x03C3;   2      )   ]
                            {\displaystyle {\frac {1}{2}}\left[1+\operatorname
CDF                         {erf} \left({\frac {x-\mu }{\sigma {\sqrt
                            {2}}}}\right)\right]}  [{\displaystyle {\frac {1}
                            {2}}\left[1+\operatorname {erf} \left({\frac {x-\mu
                            }{\sigma {\sqrt {2}}}}\right)\right]}]
                               &#x03BC; + &#x03C3;   2    erf  &#x2212; 1
                            &#x2061; ( 2 F &#x2212; 1 )   {\displaystyle \mu
Quantile                    +\sigma {\sqrt {2}}\operatorname {erf} ^{-1}(2F-1)}
                            [{\displaystyle \mu +\sigma {\sqrt
                            {2}}\operatorname {erf} ^{-1}(2F-1)}]
Mean                           &#x03BC;   {\displaystyle \mu }  [\mu ]
Median                         &#x03BC;   {\displaystyle \mu }  [\mu ]
Mode                           &#x03BC;   {\displaystyle \mu }  [\mu ]
Variance                        &#x03C3;  2     {\displaystyle \sigma ^{2}}
                            [\sigma ^{2}]
Skewness                       0   {\displaystyle 0}  [{\displaystyle 0}]
Ex._kurtosis                   0   {\displaystyle 0}  [{\displaystyle 0}]
                                 1 2   log &#x2061; ( 2 &#x03C0; e  &#x03C3;  2
Entropy                     )   {\displaystyle {\frac {1}{2}}\log(2\pi e\sigma
                            ^{2})}  [{\displaystyle {\frac {1}{2}}\log(2\pi
                            e\sigma ^{2})}]
                               exp &#x2061; ( &#x03BC; t +  &#x03C3;  2    t  2
MGF                         /  2 )   {\displaystyle \exp(\mu t+\sigma ^{2}t^
                            {2}/2)}  [{\displaystyle \exp(\mu t+\sigma ^{2}t^
                            {2}/2)}]
                               exp &#x2061; ( i &#x03BC; t &#x2212;  &#x03C3;
CF                          2    t  2    /  2 )   {\displaystyle \exp(i\mu t-
                            \sigma ^{2}t^{2}/2)}  [{\displaystyle \exp(i\mu t-
                            \sigma ^{2}t^{2}/2)}]
                                 I   ( &#x03BC; , &#x03C3; ) =   (    1  /
                            &#x03C3;  2     0     0   2  /   &#x03C3;  2      )
                            {\displaystyle {\mathcal {I}}(\mu ,\sigma )={\begin
                            {pmatrix}1/\sigma ^{2}&0\\0&2/\sigma ^{2}\end
                            {pmatrix}}}  [{\displaystyle {\mathcal {I}}(\mu
                            ,\sigma )={\begin{pmatrix}1/\sigma ^{2}&0\\0&2/
Fisher_information          \sigma ^{2}\end{pmatrix}}}]       I   ( &#x03BC; ,
                            &#x03C3;  2   ) =   (    1  /   &#x03C3;  2     0
                            0   1  /  ( 2  &#x03C3;  4   )    )
                            {\displaystyle {\mathcal {I}}(\mu ,\sigma ^{2})=
                            {\begin{pmatrix}1/\sigma ^{2}&0\\0&1/(2\sigma ^
                            {4})\end{pmatrix}}}  [{\displaystyle {\mathcal {I}}
                            (\mu ,\sigma ^{2})={\begin{pmatrix}1/\sigma ^
                            {2}&0\\0&1/(2\sigma ^{4})\end{pmatrix}}}]
                                D  KL   (    N    0   &#x2016;    N    1   ) =
                            1 2   { (  &#x03C3;  0    /   &#x03C3;  1    )  2
                            +    (  &#x03BC;  1   &#x2212;  &#x03BC;  0    )  2
                            &#x03C3;  1   2     &#x2212; 1 + 2 ln &#x2061;
                            &#x03C3;  1    &#x03C3;  0     }   {\displaystyle
                            D_{\text{KL}}({\mathcal {N}}_{0}\|{\mathcal {N}}_
Kullback-Leibler_divergence {1})={1 \over 2}\{(\sigma _{0}/\sigma _{1})^{2}+
                            {\frac {(\mu _{1}-\mu _{0})^{2}}{\sigma _{1}^{2}}}-
                            1+2\ln {\sigma _{1} \over \sigma _{0}}\}}  [
                            {\displaystyle D_{\text{KL}}({\mathcal {N}}_{0}\|
                            {\mathcal {N}}_{1})={1 \over 2}\{(\sigma _{0}/
                            \sigma _{1})^{2}+{\frac {(\mu _{1}-\mu _{0})^{2}}
                            {\sigma _{1}^{2}}}-1+2\ln {\sigma _{1} \over \sigma
                            _{0}}\}}]
In probability_theory, the normal (or Gaussian or Gauss or LaplaceâGauss)
distribution is a very common continuous_probability_distribution. Normal
distributions are important in statistics and are often used in the natural and
social_sciences to represent real-valued random_variables whose distributions
are not known.[1][2] A random_variable with a Gaussian distribution is said to
be normally distributed and is called a normal deviate.
The normal distribution is useful because of the central_limit_theorem. In its
most general form, under some conditions (which include finite variance), it
states that averages of samples of observations of random_variables
independently drawn from independent distributions converge_in_distribution to
the normal, that is, they become normally distributed when the number of
observations is sufficiently large. Physical quantities that are expected to be
the sum of many independent processes (such as measurement_errors) often have
distributions that are nearly normal.[3] Moreover, many results and methods
(such as propagation_of_uncertainty and least_squares parameter fitting) can be
derived analytically in explicit form when the relevant variables are normally
distributed.
The normal distribution is sometimes informally called the bell curve. However,
many other distributions are bell-shaped (such as the Cauchy, Student's_t-, and
logistic distributions).
The probability_density of the normal distribution is
         f ( x &#x2223; &#x03BC; ,  &#x03C3;  2   ) =   1  2 &#x03C0;  &#x03C3;
      2       e  &#x2212;    ( x &#x2212; &#x03BC;  )  2     2  &#x03C3;  2
      {\displaystyle f(x\mid \mu ,\sigma ^{2})={\frac {1}{\sqrt {2\pi \sigma ^
      {2}}}}e^{-{\frac {(x-\mu )^{2}}{2\sigma ^{2}}}}}  [{\displaystyle f(x\mid
      \mu ,\sigma ^{2})={\frac {1}{\sqrt {2\pi \sigma ^{2}}}}e^{-{\frac {(x-\mu
      )^{2}}{2\sigma ^{2}}}}}]
where
    *    &#x03BC;   {\displaystyle \mu }  [\mu ] is the mean or expectation of
      the distribution (and also its median and mode),
    *    &#x03C3;   {\displaystyle \sigma }  [\sigma ] is the standard
      deviation, and
    *     &#x03C3;  2     {\displaystyle \sigma ^{2}}  [\sigma ^{2}] is the
      variance.
⁰
***** Contents *****
    * 1_Definition
          o 1.1_Standard_normal_distribution
          o 1.2_General_normal_distribution
          o 1.3_Notation
          o 1.4_Alternative_parameterizations
    * 2_Properties
          o 2.1_Symmetries_and_derivatives
          o 2.2_Moments
          o 2.3_Fourier_transform_and_characteristic_function
          o 2.4_Moment_and_cumulant_generating_functions
    * 3_Cumulative_distribution_function
          o 3.1_Standard_deviation_and_coverage
          o 3.2_Quantile_function
    * 4_Zero-variance_limit
    * 5_Central_limit_theorem
    * 6_Maximum_entropy
    * 7_Operations_on_normal_deviates
          o 7.1_Infinite_divisibility_and_CramÃ©r's_theorem
          o 7.2_Bernstein's_theorem
    * 8_Other_properties
    * 9_Related_distributions
          o 9.1_Operations_on_a_single_random_variable
          o 9.2_Combination_of_two_independent_random_variables
          o 9.3_Combination_of_two_or_more_independent_random_variables
          o 9.4_Operations_on_the_density_function
          o 9.5_Extensions
    * 10_Normality_tests
    * 11_Estimation_of_parameters
          o 11.1_Sample_mean
          o 11.2_Sample_variance
          o 11.3_Confidence_intervals
    * 12_Bayesian_analysis_of_the_normal_distribution
          o 12.1_Sum_of_two_quadratics
                # 12.1.1_Scalar_form
                # 12.1.2_Vector_form
          o 12.2_Sum_of_differences_from_the_mean
          o 12.3_With_known_variance
          o 12.4_With_known_mean
          o 12.5_With_unknown_mean_and_unknown_variance
    * 13_Occurrence_and_applications
          o 13.1_Exact_normality
          o 13.2_Approximate_normality
          o 13.3_Assumed_normality
          o 13.4_Produced_normality
    * 14_Generating_values_from_normal_distribution
    * 15_Numerical_approximations_for_the_normal_CDF
    * 16_History
          o 16.1_Development
          o 16.2_Naming
    * 17_See_also
    * 18_Notes
    * 19_References
          o 19.1_Citations
          o 19.2_Sources
    * 20_External_links
***** Definition[edit] *****
**** Standard normal distribution[edit] ****
The simplest case of a normal distribution is known as the standard normal
distribution. This is a special case when     &#x03BC; = 0   {\displaystyle \mu
=0}  [\mu =0] and     &#x03C3; = 1   {\displaystyle \sigma =1}  [\sigma =1],
and it is described by this probability_density_function:
         &#x03C6; ( x ) =   1  2 &#x03C0;     e  &#x2212;   1 2    x  2
      {\displaystyle \varphi (x)={\frac {1}{\sqrt {2\pi }}}e^{-{\frac {1}{2}}x^
      {2}}}  [{\displaystyle \varphi (x)={\frac {1}{\sqrt {2\pi }}}e^{-{\frac
      {1}{2}}x^{2}}}]
The factor     1  /    2 &#x03C0;     {\displaystyle 1/{\sqrt {2\pi }}}  [1/
{\sqrt {2\pi }}] in this expression ensures that the total area under the curve
&#x03C6; ( x )   {\displaystyle \varphi (x)}  [\varphi (x)] is equal to one.
[note_1] The factor     1  /  2   {\displaystyle 1/2}  [1/2] in the exponent
ensures that the distribution has unit variance (i.e. the variance is equal to
one), and therefore also unit standard deviation. This function is symmetric
around     x = 0   {\displaystyle x=0}  [x=0], where it attains its maximum
value     1  /    2 &#x03C0;     {\displaystyle 1/{\sqrt {2\pi }}}  [1/{\sqrt
{2\pi }}] and has inflection_points at     x = + 1   {\displaystyle x=+1}  [
{\displaystyle x=+1}] and     x = &#x2212; 1   {\displaystyle x=-1}  [x=-1].
Authors may differ also on which normal distribution should be called the
"standard" one. Gauss defined the standard normal as having variance
&#x03C3;  2   = 1  /  2   {\displaystyle \sigma ^{2}=1/2}  [{\displaystyle
\sigma ^{2}=1/2}], that is
         &#x03C6; ( x ) =    e  &#x2212;  x  2      &#x03C0;
      {\displaystyle \varphi (x)={\frac {e^{-x^{2}}}{\sqrt {\pi }}}}  [
      {\displaystyle \varphi (x)={\frac {e^{-x^{2}}}{\sqrt {\pi }}}}]
Stigler[4] goes even further, defining the standard normal with variance
&#x03C3;  2   = 1  /  ( 2 &#x03C0; )   {\displaystyle \sigma ^{2}=1/(2\pi )}  [
{\displaystyle \sigma ^{2}=1/(2\pi )}] :
         &#x03C6; ( x ) =  e  &#x2212; &#x03C0;  x  2       {\displaystyle
      \varphi (x)=e^{-\pi x^{2}}}  [{\displaystyle \varphi (x)=e^{-\pi x^{2}}}]
**** General normal distribution[edit] ****
Every normal distribution is a version of the standard normal distribution
whose domain has been stretched by a factor     &#x03C3;   {\displaystyle
\sigma }  [\sigma ] (the standard deviation) and then translated by
&#x03BC;   {\displaystyle \mu }  [\mu ] (the mean value):
         f ( x &#x2223; &#x03BC; ,  &#x03C3;  2   ) =   1 &#x03C3;   &#x03C6;
      (    x &#x2212; &#x03BC;  &#x03C3;   )  .   {\displaystyle f(x\mid \mu
      ,\sigma ^{2})={\frac {1}{\sigma }}\varphi \left({\frac {x-\mu }{\sigma
      }}\right).}  [{\displaystyle f(x\mid \mu ,\sigma ^{2})={\frac {1}{\sigma
      }}\varphi \left({\frac {x-\mu }{\sigma }}\right).}]
The probability density must be scaled by     1  /  &#x03C3;   {\displaystyle
1/\sigma }  [1/\sigma ] so that the integral is still 1.
If     Z   {\displaystyle Z}  [Z] is a standard_normal_deviate, then     X =
&#x03C3; Z + &#x03BC;   {\displaystyle X=\sigma Z+\mu }  [{\displaystyle
X=\sigma Z+\mu }] will have a normal distribution with expected value
&#x03BC;   {\displaystyle \mu }  [\mu ] and standard deviation     &#x03C3;
{\displaystyle \sigma }  [\sigma ]. Conversely, if     X   {\displaystyle X}
[X] is a normal deviate with parameters     &#x03BC;   {\displaystyle \mu }
[\mu ] and      &#x03C3;  2     {\displaystyle \sigma ^{2}}  [\sigma ^{2}],
then     Z = ( X &#x2212; &#x03BC; )  /  &#x03C3;   {\displaystyle Z=(X-\mu )/
\sigma }  [{\displaystyle Z=(X-\mu )/\sigma }] will have a standard normal
distribution. This variate is called the standardized form of     X
{\displaystyle X}  [X]
Every normal distribution is the exponential of a quadratic_function:
         f ( x ) =  e  a  x  2   + b x + c     {\displaystyle f(x)=e^{ax^
      {2}+bx+c}}  [{\displaystyle f(x)=e^{ax^{2}+bx+c}}]
where     a < 0   {\displaystyle a<0}  [a<0] and     c =  b  2    /  ( 4 a ) +
ln &#x2061; ( &#x2212; a  /  &#x03C0; )  /  2   {\displaystyle c=b^{2}/(4a)+\ln
(-a/\pi )/2}  [{\displaystyle c=b^{2}/(4a)+\ln(-a/\pi )/2}]. In this form, the
mean value is     &#x03BC; = &#x2212; b  /  ( 2 a )   {\displaystyle \mu =-b/
(2a)}  [{\displaystyle \mu =-b/(2a)}], and the variance is      &#x03C3;  2   =
&#x2212; 1  /  ( 2 a )   {\displaystyle \sigma ^{2}=-1/(2a)}  [{\displaystyle
\sigma ^{2}=-1/(2a)}]. For the standard normal distribution,     a = &#x2212; 1
/  2   {\displaystyle a=-1/2}  [{\displaystyle a=-1/2}],     b = 0
{\displaystyle b=0}  [b=0], and     c = &#x2212; ln &#x2061; ( 2 &#x03C0; )  /
2   {\displaystyle c=-\ln(2\pi )/2}  [{\displaystyle c=-\ln(2\pi )/2}].
**** Notation[edit] ****
The probability density of the standard Gaussian distribution (standard normal
distribution) (with zero mean and unit variance) is often denoted with the
Greek letter     &#x03D5;   {\displaystyle \phi }  [\phi ] (phi).[5] The
alternative form of the Greek letter phi,     &#x03C6;   {\displaystyle \varphi
}  [\varphi ], is also used quite often.
The normal distribution is often referred to as     N ( &#x03BC; ,  &#x03C3;  2
)   {\displaystyle N(\mu ,\sigma ^{2})}  [N(\mu ,\sigma ^{2})] or       N
( &#x03BC; ,  &#x03C3;  2   )   {\displaystyle {\mathcal {N}}(\mu ,\sigma ^
{2})}  [{\mathcal {N}}(\mu ,\sigma ^{2})].[6] Thus when a random variable     X
{\displaystyle X}  [X] is distributed normally with mean     &#x03BC;
{\displaystyle \mu }  [\mu ] and variance      &#x03C3;  2     {\displaystyle
\sigma ^{2}}  [\sigma ^{2}], one may write
         X &#x223C;   N   ( &#x03BC; ,  &#x03C3;  2   ) .   {\displaystyle
      X\sim {\mathcal {N}}(\mu ,\sigma ^{2}).}  [{\displaystyle X\sim {\mathcal
      {N}}(\mu ,\sigma ^{2}).}]
**** Alternative parameterizations[edit] ****
Some authors advocate using the precision     &#x03C4;   {\displaystyle \tau }
[\tau ] as the parameter defining the width of the distribution, instead of the
deviation     &#x03C3;   {\displaystyle \sigma }  [\sigma ] or the variance
&#x03C3;  2     {\displaystyle \sigma ^{2}}  [\sigma ^{2}]. The precision is
normally defined as the reciprocal of the variance,     1  /   &#x03C3;  2
{\displaystyle 1/\sigma ^{2}}  [{\displaystyle 1/\sigma ^{2}}].[7] The formula
for the distribution then becomes
         f ( x ) =    &#x03C4;  2 &#x03C0;      e  &#x2212; &#x03C4; ( x
      &#x2212; &#x03BC;  )  2    /  2   .   {\displaystyle f(x)={\sqrt {\frac
      {\tau }{2\pi }}}e^{-\tau (x-\mu )^{2}/2}.}  [{\displaystyle f(x)={\sqrt
      {\frac {\tau }{2\pi }}}e^{-\tau (x-\mu )^{2}/2}.}]
This choice is claimed to have advantages in numerical computations when
&#x03C3;   {\displaystyle \sigma }  [\sigma ] is very close to zero and
simplify formulas in some contexts, such as in the Bayesian_inference of
variables with multivariate_normal_distribution.
Also the reciprocal of the standard deviation      &#x03C4;  &#x2032;   = 1  /
&#x03C3;   {\displaystyle \tau ^{\prime }=1/\sigma }  [\tau ^{\prime }=1/\sigma
] might be defined as the precision and the expression of the normal
distribution becomes
         f ( x ) =    &#x03C4;  &#x2032;    2 &#x03C0;     e  &#x2212;
      (  &#x03C4;  &#x2032;    )  2   ( x &#x2212; &#x03BC;  )  2    /  2   .
      {\displaystyle f(x)={\frac {\tau ^{\prime }}{\sqrt {2\pi }}}e^{-(\tau ^
      {\prime })^{2}(x-\mu )^{2}/2}.}  [{\displaystyle f(x)={\frac {\tau ^
      {\prime }}{\sqrt {2\pi }}}e^{-(\tau ^{\prime })^{2}(x-\mu )^{2}/2}.}]
According to Stigler, this formulation is advantageous because of a much
simpler and easier-to-remember formula, and simple approximate formulas for the
quantiles of the distribution.
Normal distributions form an exponential_family with natural_parameters
&#x03B8;  1   =   &#x03BC;  &#x03C3;  2        {\displaystyle \textstyle \theta
_{1}={\frac {\mu }{\sigma ^{2}}}}  [{\displaystyle \textstyle \theta _{1}=
{\frac {\mu }{\sigma ^{2}}}}] and       &#x03B8;  2   =    &#x2212; 1   2
&#x03C3;  2         {\displaystyle \textstyle \theta _{2}={\frac {-1}{2\sigma ^
{2}}}}  [{\displaystyle \textstyle \theta _{2}={\frac {-1}{2\sigma ^{2}}}}],
and natural statistics x and x2. The dual, expectation parameters for normal
distribution are Î·1 = Î¼ and Î·2 = Î¼2 + Ï2.
***** Properties[edit] *****
The normal distribution is the only absolutely_continuous distribution whose
cumulants beyond the first two (i.e., other than the mean and variance) are
zero. It is also the continuous distribution with the maximum_entropy for a
specified mean and variance.[8][9] Geary has shown, assuming that the mean and
variance are finite, that the normal distribution is the only distribution
where the mean and variance calculated from a set of independent draws are
independent of each other.[10][11]
The normal distribution is a subclass of the elliptical_distributions. The
normal distribution is symmetric about its mean, and is non-zero over the
entire real line. As such it may not be a suitable model for variables that are
inherently positive or strongly skewed, such as the weight of a person or the
price of a share. Such variables may be better described by other
distributions, such as the log-normal_distribution or the Pareto_distribution.
The value of the normal distribution is practically zero when the value     x
{\displaystyle x}  [x] lies more than a few standard_deviations away from the
mean (e.g., a spread of three standard deviations covers all but 0.27% of the
total distribution). Therefore, it may not be an appropriate model when one
expects a significant fraction of outliersâvalues that lie many standard
deviations away from the meanâand least squares and other statistical
inference methods that are optimal for normally distributed variables often
become highly unreliable when applied to such data. In those cases, a more
heavy-tailed distribution should be assumed and the appropriate robust
statistical_inference methods applied.
The Gaussian distribution belongs to the family of stable_distributions which
are the attractors of sums of independent,_identically_distributed
distributions whether or not the mean or variance is finite. Except for the
Gaussian which is a limiting case, all stable distributions have heavy tails
and infinite variance. It is one of the few distributions that are stable and
that have probability density functions that can be expressed analytically, the
others being the Cauchy_distribution and the LÃ©vy_distribution.
**** Symmetries and derivatives[edit] ****
The normal distribution with density     f ( x )   {\displaystyle f(x)}  [f(x)]
(mean     &#x03BC;   {\displaystyle \mu }  [\mu ] and standard deviation
&#x03C3; > 0   {\displaystyle \sigma >0}  [\sigma >0]) has the following
properties:
    * It is symmetric around the point     x = &#x03BC; ,   {\displaystyle
      x=\mu ,}  [{\displaystyle x=\mu ,}] which is at the same time the mode,
      the median and the mean of the distribution.[12]
    * It is unimodal: its first derivative is positive for     x < &#x03BC; ,
      {\displaystyle x<\mu ,}  [{\displaystyle x<\mu ,}] negative for     x >
      &#x03BC; ,   {\displaystyle x>\mu ,}  [{\displaystyle x>\mu ,}] and zero
      only at     x = &#x03BC; .   {\displaystyle x=\mu .}  [{\displaystyle
      x=\mu .}]
    * The area under the curve and over the     x   {\displaystyle x}  [x]-axis
      is unity (i.e. equal to one).
    * Its density has two inflection_points (where the second derivative of
      f   {\displaystyle f}  [f] is zero and changes sign), located one
      standard deviation away from the mean, namely at     x = &#x03BC;
      &#x2212; &#x03C3;   {\displaystyle x=\mu -\sigma }  [{\displaystyle x=\mu
      -\sigma }] and     x = &#x03BC; + &#x03C3; .   {\displaystyle x=\mu
      +\sigma .}  [{\displaystyle x=\mu +\sigma .}][12]
    * Its density is log-concave.[12]
    * Its density is infinitely differentiable, indeed supersmooth of order 2.
      [13]
Furthermore, the density     &#x03C6;   {\displaystyle \varphi }  [\varphi ] of
the standard normal distribution (i.e.     &#x03BC; = 0   {\displaystyle \mu
=0}  [\mu =0] and     &#x03C3; = 1   {\displaystyle \sigma =1}  [{\displaystyle
\sigma =1}]) also has the following properties:
    * Its first derivative is      &#x03C6;  &#x2032;   ( x ) = &#x2212; x
      &#x03C6; ( x ) .   {\displaystyle \varphi ^{\prime }(x)=-x\varphi (x).}
      [{\displaystyle \varphi ^{\prime }(x)=-x\varphi (x).}]
    * Its second derivative is      &#x03C6;  &#x2032; &#x2032;   ( x ) = (  x
      2   &#x2212; 1 ) &#x03C6; ( x )   {\displaystyle \varphi ^{\prime \prime
      }(x)=(x^{2}-1)\varphi (x)}  [{\displaystyle \varphi ^{\prime \prime }(x)=
      (x^{2}-1)\varphi (x)}]
    * More generally, its nth derivative is      &#x03C6;  ( n )   ( x ) =
      ( &#x2212; 1  )  n    He  n   &#x2061; ( x ) &#x03C6; ( x ) ,
      {\displaystyle \varphi ^{(n)}(x)=(-1)^{n}\operatorname {He} _{n}
      (x)\varphi (x),}  [{\displaystyle \varphi ^{(n)}(x)=(-1)^{n}\operatorname
      {He} _{n}(x)\varphi (x),}] where      He  n   &#x2061; ( x )
      {\displaystyle \operatorname {He} _{n}(x)}  [{\displaystyle \operatorname
      {He} _{n}(x)}] is the nth (probabilist) Hermite_polynomial.[14]
    * The probability that a normally distributed variable     X
      {\displaystyle X}  [X] with known     &#x03BC;   {\displaystyle \mu }
      [\mu ] and     &#x03C3;   {\displaystyle \sigma }  [\sigma ] is in a
      particular set, can be calculated by using the fact that the fraction
      Z = ( X &#x2212; &#x03BC; )  /  &#x03C3;   {\displaystyle Z=(X-\mu )/
      \sigma }  [{\displaystyle Z=(X-\mu )/\sigma }] has a standard normal
      distribution.
**** Moments[edit] ****
See also: List_of_integrals_of_Gaussian_functions
The plain and absolute moments of a variable     X   {\displaystyle X}  [X] are
the expected values of      X  p     {\displaystyle X^{p}}  [{\displaystyle X^
{p}}] and      |  X   |   p     {\displaystyle |X|^{p}}  [{\displaystyle |X|^
{p}}], respectively. If the expected value     &#x03BC;   {\displaystyle \mu }
[\mu ] of     X   {\displaystyle X}  [X] is zero, these parameters are called
central moments. Usually we are interested only in moments with integer order
&#xA0; p   {\displaystyle \ p}  [\ p].
If     X   {\displaystyle X}  [X] has a normal distribution, these moments
exist and are finite for any     p   {\displaystyle p}  [p] whose real part is
greater than â1. For any non-negative integer     p   {\displaystyle p}  [p],
the plain central moments are:[15]
         E &#x2061;  [  X  p   ]  =   {    0    if&#xA0;  p  &#xA0;is odd,
      &#x03C3;  p   ( p &#x2212; 1 ) ! !    if&#xA0;  p  &#xA0;is even.
      {\displaystyle \operatorname {E} \left[X^{p}\right]={\begin{cases}0&
      {\text{if }}p{\text{ is odd,}}\\\sigma ^{p}(p-1)!!&{\text{if }}p{\text
      { is even.}}\end{cases}}}  [{\displaystyle \operatorname {E} \left[X^
      {p}\right]={\begin{cases}0&{\text{if }}p{\text{ is odd,}}\\\sigma ^{p}(p-
      1)!!&{\text{if }}p{\text{ is even.}}\end{cases}}}]
Here     n ! !   {\displaystyle n!!}  [n!!] denotes the double_factorial, that
is, the product of all numbers from     n   {\displaystyle n}  [n] to 1 that
have the same parity as     n .   {\displaystyle n.}  [n.]
The central absolute moments coincide with plain moments for all even orders,
but are nonzero for odd orders. For any non-negative integer     p ,
{\displaystyle p,}  [p,]
         E &#x2061;  [   |  X   |   p    ]  =  &#x03C3;  p   ( p &#x2212; 1 ) !
      ! &#x22C5;     {       2 &#x03C0;       if&#xA0;  p  &#xA0;is odd      1
      if&#xA0;  p  &#xA0;is even        }  =  &#x03C3;  p   &#x22C5;     2  p
      /  2   &#x0393;  (    p + 1  2   )    &#x03C0;      {\displaystyle
      \operatorname {E} \left[|X|^{p}\right]=\sigma ^{p}(p-1)!!\cdot \left.
      {\begin{cases}{\sqrt {\frac {2}{\pi }}}&{\text{if }}p{\text{ is odd}}\\1&
      {\text{if }}p{\text{ is even}}\end{cases}}\right\}=\sigma ^{p}\cdot
      {\frac {2^{p/2}\Gamma \left({\frac {p+1}{2}}\right)}{\sqrt {\pi }}}}  [
      {\displaystyle \operatorname {E} \left[|X|^{p}\right]=\sigma ^{p}(p-
      1)!!\cdot \left.{\begin{cases}{\sqrt {\frac {2}{\pi }}}&{\text{if }}p
      {\text{ is odd}}\\1&{\text{if }}p{\text{ is even}}\end
      {cases}}\right\}=\sigma ^{p}\cdot {\frac {2^{p/2}\Gamma \left({\frac
      {p+1}{2}}\right)}{\sqrt {\pi }}}}]
The last formula is valid also for any non-integer     p > &#x2212; 1.
{\displaystyle p>-1.}  [{\displaystyle p>-1.}] When the mean     &#x03BC;
&#x2260; 0 ,   {\displaystyle \mu \neq 0,}  [{\displaystyle \mu \neq 0,}] the
plain and absolute moments can be expressed in terms of confluent
hypergeometric_functions         1    F  1     {\displaystyle {}_{1}F_{1}}  [
{}_{1}F_{1}] and     U .   {\displaystyle U.}  [U.][citation_needed]
         E &#x2061;  [  X  p   ]  =  &#x03C3;  p   &#x22C5; ( &#x2212; i   2
      )  p   U  (  &#x2212;   p 2   ,   1 2   , &#x2212;   1 2     (   &#x03BC;
      &#x03C3;   )   2    )  ,   {\displaystyle \operatorname {E} \left[X^
      {p}\right]=\sigma ^{p}\cdot (-i{\sqrt {2}})^{p}U\left(-{\frac {p}{2}},
      {\frac {1}{2}},-{\frac {1}{2}}\left({\frac {\mu }{\sigma }}\right)^
      {2}\right),}  [{\displaystyle \operatorname {E} \left[X^{p}\right]=\sigma
      ^{p}\cdot (-i{\sqrt {2}})^{p}U\left(-{\frac {p}{2}},{\frac {1}{2}},-
      {\frac {1}{2}}\left({\frac {\mu }{\sigma }}\right)^{2}\right),}]
         E &#x2061;  [   |  X   |   p    ]  =  &#x03C3;  p   &#x22C5;  2  p  /
      2      &#x0393;  (    1 + p  2   )    &#x03C0;        1    F  1
      (  &#x2212;   p 2   ,   1 2   , &#x2212;   1 2     (   &#x03BC; &#x03C3;
      )   2    )  .   {\displaystyle \operatorname {E} \left[|X|^
      {p}\right]=\sigma ^{p}\cdot 2^{p/2}{\frac {\Gamma \left({\frac {1+p}
      {2}}\right)}{\sqrt {\pi }}}{}_{1}F_{1}\left(-{\frac {p}{2}},{\frac {1}
      {2}},-{\frac {1}{2}}\left({\frac {\mu }{\sigma }}\right)^{2}\right).}  [
      {\displaystyle \operatorname {E} \left[|X|^{p}\right]=\sigma ^{p}\cdot 2^
      {p/2}{\frac {\Gamma \left({\frac {1+p}{2}}\right)}{\sqrt {\pi }}}{}_{1}F_
      {1}\left(-{\frac {p}{2}},{\frac {1}{2}},-{\frac {1}{2}}\left({\frac {\mu
      }{\sigma }}\right)^{2}\right).}]
These expressions remain valid even if     p   {\displaystyle p}  [p] is not
integer. See also generalized_Hermite_polynomials.
Order Non-central moment                   Central moment
1        &#x03BC;   {\displaystyle \mu }      0   {\displaystyle 0}  [
      [\mu ]                               {\displaystyle 0}]
          &#x03BC;  2   +  &#x03C3;  2
2     {\displaystyle \mu ^{2}+\sigma ^{2}}     &#x03C3;  2     {\displaystyle
      [{\displaystyle \mu ^{2}+\sigma ^    \sigma ^{2}}  [\sigma ^{2}]
      {2}}]
          &#x03BC;  3   + 3 &#x03BC;
      &#x03C3;  2     {\displaystyle \mu ^    0   {\displaystyle 0}  [
3     {3}+3\mu \sigma ^{2}}  [             {\displaystyle 0}]
      {\displaystyle \mu ^{3}+3\mu \sigma
      ^{2}}]
          &#x03BC;  4   + 6  &#x03BC;  2
      &#x03C3;  2   + 3  &#x03C3;  4          3  &#x03C3;  4     {\displaystyle
4     {\displaystyle \mu ^{4}+6\mu ^       3\sigma ^{4}}  [{\displaystyle
      {2}\sigma ^{2}+3\sigma ^{4}}  [      3\sigma ^{4}}]
      {\displaystyle \mu ^{4}+6\mu ^
      {2}\sigma ^{2}+3\sigma ^{4}}]
          &#x03BC;  5   + 10  &#x03BC;  3
      &#x03C3;  2   + 15 &#x03BC;
      &#x03C3;  4     {\displaystyle \mu ^    0   {\displaystyle 0}  [
5     {5}+10\mu ^{3}\sigma ^{2}+15\mu      {\displaystyle 0}]
      \sigma ^{4}}  [{\displaystyle \mu ^
      {5}+10\mu ^{3}\sigma ^{2}+15\mu
      \sigma ^{4}}]
          &#x03BC;  6   + 15  &#x03BC;  4
      &#x03C3;  2   + 45  &#x03BC;  2
      &#x03C3;  4   + 15  &#x03C3;  6         15  &#x03C3;  6
6     {\displaystyle \mu ^{6}+15\mu ^      {\displaystyle 15\sigma ^{6}}  [
      {4}\sigma ^{2}+45\mu ^{2}\sigma ^    {\displaystyle 15\sigma ^{6}}]
      {4}+15\sigma ^{6}}  [{\displaystyle
      \mu ^{6}+15\mu ^{4}\sigma ^{2}+45\mu
      ^{2}\sigma ^{4}+15\sigma ^{6}}]
          &#x03BC;  7   + 21  &#x03BC;  5
      &#x03C3;  2   + 105  &#x03BC;  3
      &#x03C3;  4   + 105 &#x03BC;
      &#x03C3;  6     {\displaystyle \mu ^    0   {\displaystyle 0}  [
7     {7}+21\mu ^{5}\sigma ^{2}+105\mu ^   {\displaystyle 0}]
      {3}\sigma ^{4}+105\mu \sigma ^{6}}
      [{\displaystyle \mu ^{7}+21\mu ^
      {5}\sigma ^{2}+105\mu ^{3}\sigma ^
      {4}+105\mu \sigma ^{6}}]
          &#x03BC;  8   + 28  &#x03BC;  6
      &#x03C3;  2   + 210  &#x03BC;  4
      &#x03C3;  4   + 420  &#x03BC;  2
      &#x03C3;  6   + 105  &#x03C3;  8
      {\displaystyle \mu ^{8}+28\mu ^         105  &#x03C3;  8
8     {6}\sigma ^{2}+210\mu ^{4}\sigma ^   {\displaystyle 105\sigma ^{8}}  [
      {4}+420\mu ^{2}\sigma ^{6}+105\sigma {\displaystyle 105\sigma ^{8}}]
      ^{8}}  [{\displaystyle \mu ^
      {8}+28\mu ^{6}\sigma ^{2}+210\mu ^
      {4}\sigma ^{4}+420\mu ^{2}\sigma ^
      {6}+105\sigma ^{8}}]
The expectation of     X   {\displaystyle X}  [X] conditioned on the event that
X   {\displaystyle X}  [X] lies in an interval     [ a , b ]   {\displaystyle
[a,b]}  [[a,b]] is given by
         E &#x2061;  [  X &#x2223; a < X < b  ]  = &#x03BC; &#x2212;  &#x03C3;
      2      f ( b ) &#x2212; f ( a )   F ( b ) &#x2212; F ( a )
      {\displaystyle \operatorname {E} \left[X\mid a<X<b\right]=\mu -\sigma ^
      {2}{\frac {f(b)-f(a)}{F(b)-F(a)}}}  [{\displaystyle \operatorname {E}
      \left[X\mid a<X<b\right]=\mu -\sigma ^{2}{\frac {f(b)-f(a)}{F(b)-F(a)}}}]
where     f   {\displaystyle f}  [f] and     F   {\displaystyle F}  [F]
respectively are the density and the cumulative distribution function of     X
{\displaystyle X}  [X]. For     b = &#x221E;   {\displaystyle b=\infty }
[b=\infty ] this is known as the inverse_Mills_ratio. Note that above, density
f   {\displaystyle f}  [f] of     X   {\displaystyle X}  [X] is used instead of
standard normal density as in inverse Mills ratio, so here we have
&#x03C3;  2     {\displaystyle \sigma ^{2}}  [\sigma ^{2}] instead of
&#x03C3;   {\displaystyle \sigma }  [\sigma ].
**** Fourier transform and characteristic function[edit] ****
The Fourier_transform of a normal density     f   {\displaystyle f}  [f] with
mean     &#x03BC;   {\displaystyle \mu }  [\mu ] and standard deviation
&#x03C3;   {\displaystyle \sigma }  [\sigma ] is[16]
            f &#x005E;    ( t ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;   f
      ( x )  e  &#x2212; i t x    d x =  e  &#x2212; i &#x03BC; t    e
      &#x2212;   1 2   ( &#x03C3; t  )  2       {\displaystyle {\hat {f}}
      (t)=\int _{-\infty }^{\infty }f(x)e^{-itx}\,dx=e^{-i\mu t}e^{-{\frac {1}
      {2}}(\sigma t)^{2}}}  [{\displaystyle {\hat {f}}(t)=\int _{-\infty }^
      {\infty }f(x)e^{-itx}\,dx=e^{-i\mu t}e^{-{\frac {1}{2}}(\sigma t)^{2}}}]
where     i   {\displaystyle i}  [i] is the imaginary_unit. If the mean
&#x03BC; = 0   {\displaystyle \mu =0}  [\mu =0], the first factor is 1, and the
Fourier transform is, apart from a constant factor, a normal density on the
frequency_domain, with mean 0 and standard deviation     1  /  &#x03C3;
{\displaystyle 1/\sigma }  [1/\sigma ]. In particular, the standard normal
distribution     &#x03C6;   {\displaystyle \varphi }  [\varphi ] is an
eigenfunction of the Fourier transform.
In probability theory, the Fourier transform of the probability distribution of
a real-valued random variable     X   {\displaystyle X}  [X] is closely
connected to the characteristic_function      &#x03C6;  X   ( t )
{\displaystyle \varphi _{X}(t)}  [\varphi _{X}(t)] of that variable, which is
defined as the expected_value of      e  i t X     {\displaystyle e^{itX}}  [e^
{{itX}}], as a function of the real variable     t   {\displaystyle t}  [t]
(the frequency parameter of the Fourier transform). This definition can be
analytically extended to a complex-value variable     t   {\displaystyle t}
[t].[17] The relation between both is:
          &#x03C6;  X   ( t ) =    f &#x005E;    ( &#x2212; t )
      {\displaystyle \varphi _{X}(t)={\hat {f}}(-t)}  [{\displaystyle \varphi _
      {X}(t)={\hat {f}}(-t)}]
**** Moment and cumulant generating functions[edit] ****
The moment_generating_function of a real random variable     X   {\displaystyle
X}  [X] is the expected value of      e  t X     {\displaystyle e^{tX}}  [
{\displaystyle e^{tX}}], as a function of the real parameter     t
{\displaystyle t}  [t]. For a normal distribution with density     f
{\displaystyle f}  [f], mean     &#x03BC;   {\displaystyle \mu }  [\mu ] and
deviation     &#x03C3;   {\displaystyle \sigma }  [\sigma ], the moment
generating function exists and is equal to
         M ( t ) = E &#x2061; [  e  t X   ] =    f &#x005E;    ( i t ) =  e
      &#x03BC; t    e     1 2     &#x03C3;  2    t  2       {\displaystyle M
      (t)=\operatorname {E} [e^{tX}]={\hat {f}}(it)=e^{\mu t}e^{{\tfrac {1}
      {2}}\sigma ^{2}t^{2}}}  [{\displaystyle M(t)=\operatorname {E} [e^{tX}]=
      {\hat {f}}(it)=e^{\mu t}e^{{\tfrac {1}{2}}\sigma ^{2}t^{2}}}]
The cumulant_generating_function is the logarithm of the moment generating
function, namely
         g ( t ) = ln &#x2061; M ( t ) = &#x03BC; t +    1 2     &#x03C3;  2
      t  2     {\displaystyle g(t)=\ln M(t)=\mu t+{\tfrac {1}{2}}\sigma ^{2}t^
      {2}}  [{\displaystyle g(t)=\ln M(t)=\mu t+{\tfrac {1}{2}}\sigma ^{2}t^
      {2}}]
Since this is a quadratic polynomial in     t   {\displaystyle t}  [t], only
the first two cumulants are nonzero, namely the mean     &#x03BC;
{\displaystyle \mu }  [\mu ] and the variance      &#x03C3;  2
{\displaystyle \sigma ^{2}}  [\sigma ^{2}].
***** Cumulative distribution function[edit] *****
The cumulative_distribution_function (CDF) of the standard normal distribution,
usually denoted with the capital Greek letter     &#x03A6;   {\displaystyle
\Phi }  [\Phi ] (phi), is the integral
         &#x03A6; ( x ) =   1  2 &#x03C0;     &#x222B;  &#x2212; &#x221E;   x
      e  &#x2212;  t  2    /  2    d t   {\displaystyle \Phi (x)={\frac {1}
      {\sqrt {2\pi }}}\int _{-\infty }^{x}e^{-t^{2}/2}\,dt}  [{\displaystyle
      \Phi (x)={\frac {1}{\sqrt {2\pi }}}\int _{-\infty }^{x}e^{-t^{2}/2}\,dt}]
The related error_function     erf &#x2061; ( x )   {\displaystyle
\operatorname {erf} (x)}  [\operatorname{erf}(x)] gives the probability of a
random variable with normal distribution of mean 0 and variance 1/2 falling in
the range     [ &#x2212; x , x ]   {\displaystyle [-x,x]}  [[-x,x]]; that is
         erf &#x2061; ( x ) =   2  &#x03C0;     &#x222B;  0   x    e  &#x2212;
      t  2      d t   {\displaystyle \operatorname {erf} (x)={\frac {2}{\sqrt
      {\pi }}}\int _{0}^{x}e^{-t^{2}}\,dt}  [{\displaystyle \operatorname {erf}
      (x)={\frac {2}{\sqrt {\pi }}}\int _{0}^{x}e^{-t^{2}}\,dt}]
These integrals cannot be expressed in terms of elementary functions, and are
often said to be special_functions. However, many numerical approximations are
known; see below.
The two functions are closely related, namely
         &#x03A6; ( x ) =   1 2    [  1 + erf &#x2061;  (   x  2    )   ]
      {\displaystyle \Phi (x)={\frac {1}{2}}\left[1+\operatorname {erf} \left(
      {\frac {x}{\sqrt {2}}}\right)\right]}  [{\displaystyle \Phi (x)={\frac
      {1}{2}}\left[1+\operatorname {erf} \left({\frac {x}{\sqrt
      {2}}}\right)\right]}]
For a generic normal distribution with density     f   {\displaystyle f}  [f],
mean     &#x03BC;   {\displaystyle \mu }  [\mu ] and deviation     &#x03C3;
{\displaystyle \sigma }  [\sigma ], the cumulative distribution function is
         F ( x ) = &#x03A6;  (    x &#x2212; &#x03BC;  &#x03C3;   )  =   1 2
      [  1 + erf &#x2061;  (    x &#x2212; &#x03BC;   &#x03C3;   2      )   ]
      {\displaystyle F(x)=\Phi \left({\frac {x-\mu }{\sigma }}\right)={\frac
      {1}{2}}\left[1+\operatorname {erf} \left({\frac {x-\mu }{\sigma {\sqrt
      {2}}}}\right)\right]}  [{\displaystyle F(x)=\Phi \left({\frac {x-\mu }
      {\sigma }}\right)={\frac {1}{2}}\left[1+\operatorname {erf} \left({\frac
      {x-\mu }{\sigma {\sqrt {2}}}}\right)\right]}]
The complement of the standard normal CDF,     Q ( x ) = 1 &#x2212; &#x03A6;
( x )   {\displaystyle Q(x)=1-\Phi (x)}  [Q(x)=1-\Phi (x)], is often called the
Q-function, especially in engineering texts.[18][19] It gives the probability
that the value of a standard normal random variable     X   {\displaystyle X}
[X] will exceed     x   {\displaystyle x}  [x]:     P ( X > x )
{\displaystyle P(X>x)}  [{\displaystyle P(X>x)}]. Other definitions of the
Q   {\displaystyle Q}  [Q]-function, all of which are simple transformations of
&#x03A6;   {\displaystyle \Phi }  [\Phi ], are also used occasionally.[20]
The graph of the standard normal CDF     &#x03A6;   {\displaystyle \Phi }
[\Phi ] has 2-fold rotational_symmetry around the point (0,1/2); that is,
&#x03A6; ( &#x2212; x ) = 1 &#x2212; &#x03A6; ( x )   {\displaystyle \Phi (-
x)=1-\Phi (x)}  [\Phi (-x)=1-\Phi (x)]. Its antiderivative (indefinite
integral) is
         &#x222B; &#x03A6; ( x )  d x = x &#x03A6; ( x ) + &#x03C6; ( x ) + C .
      {\displaystyle \int \Phi (x)\,dx=x\Phi (x)+\varphi (x)+C.}  [
      {\displaystyle \int \Phi (x)\,dx=x\Phi (x)+\varphi (x)+C.}]
The CDF of the standard normal distribution can be expanded by Integration_by
parts into a series:
         &#x03A6; ( x ) =   1 2   +   1  2 &#x03C0;    &#x22C5;  e  &#x2212;  x
      2    /  2    [  x +    x  3   3   +    x  5    3 &#x22C5; 5    + &#x22EF;
      +    x  2 n + 1    ( 2 n + 1 ) ! !    + &#x22EF;  ]    {\displaystyle
      \Phi (x)={\frac {1}{2}}+{\frac {1}{\sqrt {2\pi }}}\cdot e^{-x^{2}/2}\left
      [x+{\frac {x^{3}}{3}}+{\frac {x^{5}}{3\cdot 5}}+\cdots +{\frac {x^{2n+1}}
      {(2n+1)!!}}+\cdots \right]}  [{\displaystyle \Phi (x)={\frac {1}{2}}+
      {\frac {1}{\sqrt {2\pi }}}\cdot e^{-x^{2}/2}\left[x+{\frac {x^{3}}{3}}+
      {\frac {x^{5}}{3\cdot 5}}+\cdots +{\frac {x^{2n+1}}{(2n+1)!!}}+\cdots
      \right]}]
where     ! !   {\displaystyle !!}  [!!] denotes the double_factorial.
An asymptotic_expansion of the CDF for large x can also be derived using
integration by parts; see Error_function#Asymptotic_expansion.[21]
**** Standard deviation and coverage[edit] ****
Further information: Interval_estimation and Coverage_probability
For the normal distribution, the values less than one standard deviation away
from the mean account for 68.27% of the set; while two standard deviations from
the mean account for 95.45%; and three standard deviations account for 99.73%.
About 68% of values drawn from a normal distribution are within one standard
deviation Ï away from the mean; about 95% of the values lie within two
standard deviations; and about 99.7% are within three standard deviations. This
fact is known as the 68-95-99.7_(empirical)_rule, or the 3-sigma rule.
More precisely, the probability that a normal deviate lies in the range between
&#x03BC; &#x2212; n &#x03C3;   {\displaystyle \mu -n\sigma }  [{\displaystyle
\mu -n\sigma }] and     &#x03BC; + n &#x03C3;   {\displaystyle \mu +n\sigma }
[{\displaystyle \mu +n\sigma }] is given by
         F ( &#x03BC; + n &#x03C3; ) &#x2212; F ( &#x03BC; &#x2212; n &#x03C3;
      ) = &#x03A6; ( n ) &#x2212; &#x03A6; ( &#x2212; n ) = erf &#x2061;  (   n
      2    )  .   {\displaystyle F(\mu +n\sigma )-F(\mu -n\sigma )=\Phi (n)-
      \Phi (-n)=\operatorname {erf} \left({\frac {n}{\sqrt {2}}}\right).}  [
      {\displaystyle F(\mu +n\sigma )-F(\mu -n\sigma )=\Phi (n)-\Phi (-
      n)=\operatorname {erf} \left({\frac {n}{\sqrt {2}}}\right).}]
To 12 significant figures, the values for     n = 1 , 2 , &#x2026; , 6
{\displaystyle n=1,2,\ldots ,6}  [{\displaystyle n=1,2,\ldots ,6}] are:[22]
                  p = F
               ( &#x03BC; + n
               &#x03C3; )
               &#x2212; F           i.e.&#xA0;       or&#xA0;  1
               ( &#x03BC;       1 &#x2212; p     &#xA0;in&#xA0;
               &#x2212; n       {\displaystyle   p
   n           &#x03C3; )       {\text{i.e. }}1- {\displaystyle
{\displaystyle {\displaystyle   p}  [            {\text{or }}1    OEIS
n}  [n]        p=F(\mu +n\sigma {\displaystyle   {\text{ in }}p}
               )-F(\mu -n\sigma {\text{i.e. }}1- [{\displaystyle
               )}  [            p}]              {\text{or }}1
               {\displaystyle                    {\text{ in }}p}]
               p=F(\mu +n\sigma
               )-F(\mu -n\sigma
               )}]
1              0.682689492137   0.317310507863   3 .15148718753   OEIS: A178647
2              0.954499736104   0.045500263896   21 .9778945080   OEIS: A110894
3              0.997300203937   0.002699796063   370 .398347345   OEIS: A270712
4              0.999936657516   0.000063342484   15787 .1927673
5              0.999999426697   0.000000573303   1744277 .89362
6              0.999999998027   0.000000001973   506797345 .897
**** Quantile function[edit] ****
Further information: Quantile_function_Â§ Normal_distribution
The quantile_function of a distribution is the inverse of the cumulative
distribution function. The quantile function of the standard normal
distribution is called the probit_function, and can be expressed in terms of
the inverse error_function:
          &#x03A6;  &#x2212; 1   ( p ) =   2    erf  &#x2212; 1   &#x2061; ( 2
      p &#x2212; 1 ) ,  p &#x2208; ( 0 , 1 ) .   {\displaystyle \Phi ^{-1}(p)=
      {\sqrt {2}}\operatorname {erf} ^{-1}(2p-1),\quad p\in (0,1).}  [
      {\displaystyle \Phi ^{-1}(p)={\sqrt {2}}\operatorname {erf} ^{-1}(2p-
      1),\quad p\in (0,1).}]
For a normal random variable with mean     &#x03BC;   {\displaystyle \mu }
[\mu ] and variance      &#x03C3;  2     {\displaystyle \sigma ^{2}}  [\sigma ^
{2}], the quantile function is
          F  &#x2212; 1   ( p ) = &#x03BC; + &#x03C3;  &#x03A6;  &#x2212; 1
      ( p ) = &#x03BC; + &#x03C3;   2    erf  &#x2212; 1   &#x2061; ( 2 p
      &#x2212; 1 ) ,  p &#x2208; ( 0 , 1 ) .   {\displaystyle F^{-1}(p)=\mu
      +\sigma \Phi ^{-1}(p)=\mu +\sigma {\sqrt {2}}\operatorname {erf} ^{-1}
      (2p-1),\quad p\in (0,1).}  [{\displaystyle F^{-1}(p)=\mu +\sigma \Phi ^{-
      1}(p)=\mu +\sigma {\sqrt {2}}\operatorname {erf} ^{-1}(2p-1),\quad p\in
      (0,1).}]
The quantile      &#x03A6;  &#x2212; 1   ( p )   {\displaystyle \Phi ^{-1}(p)}
[\Phi ^{{-1}}(p)] of the standard normal distribution is commonly denoted as
z  p     {\displaystyle z_{p}}  [{\displaystyle z_{p}}]. These values are used
in hypothesis_testing, construction of confidence_intervals and Q-Q_plots. A
normal random variable     X   {\displaystyle X}  [X] will exceed     &#x03BC;
+  z  p   &#x03C3;   {\displaystyle \mu +z_{p}\sigma }  [{\displaystyle \mu +z_
{p}\sigma }] with probability     1 &#x2212; p   {\displaystyle 1-p}  [1-p],
and will lie outside the interval     &#x03BC; &#x00B1;  z  p   &#x03C3;
{\displaystyle \mu \pm z_{p}\sigma }  [{\displaystyle \mu \pm z_{p}\sigma }]
with probability     2 ( 1 &#x2212; p )   {\displaystyle 2(1-p)}  [
{\displaystyle 2(1-p)}]. In particular, the quantile      z  0.975
{\displaystyle z_{0.975}}  [{\displaystyle z_{0.975}}] is 1.96; therefore a
normal random variable will lie outside the interval     &#x03BC; &#x00B1; 1.96
&#x03C3;   {\displaystyle \mu \pm 1.96\sigma }  [\mu \pm 1.96\sigma ] in only
5% of cases.
The following table gives the quantile      z  p     {\displaystyle z_{p}}  [
{\displaystyle z_{p}}] such that     X   {\displaystyle X}  [X] will lie in the
range     &#x03BC; &#x00B1;  z  p   &#x03C3;   {\displaystyle \mu \pm z_
{p}\sigma }  [{\displaystyle \mu \pm z_{p}\sigma }] with a specified
probability     p   {\displaystyle p}  [p]. These values are useful to
determine tolerance_interval for sample_averages and other statistical
estimators with normal (or asymptotically normal) distributions:.[23][24] NOTE:
the following table shows       2    erf  &#x2212; 1   &#x2061; ( p ) =
&#x03A6;  &#x2212; 1    (    p + 1  2   )    {\displaystyle {\sqrt
{2}}\operatorname {erf} ^{-1}(p)=\Phi ^{-1}\left({\frac {p+1}{2}}\right)}  [
{\displaystyle {\sqrt {2}}\operatorname {erf} ^{-1}(p)=\Phi ^{-1}\left({\frac
{p+1}{2}}\right)}], not      &#x03A6;  &#x2212; 1   ( p )   {\displaystyle \Phi
^{-1}(p)}  [\Phi ^{{-1}}(p)] as defined above.
                        z  p                                    z  p
   p                {\displaystyle z_      p                {\displaystyle z_
{\displaystyle p}   {p}}  [             {\displaystyle p}   {p}}  [
[p]                 {\displaystyle z_   [p]                 {\displaystyle z_
                    {p}}]                                   {p}}]
0.80                1.281551565545     0.999               3.290526731492
0.90                1.644853626951      0.9999              3.890591886413
0.95                1.959963984540      0.99999             4.417173413469
0.98                2.326347874041      0.999999            4.891638475699
0.99                2.575829303549      0.9999999           5.326723886384
0.995               2.807033768344      0.99999999          5.730728868236
0.998               3.090232306168      0.999999999         6.109410204869
For small     p   {\displaystyle p}  [p], the quantile function has the useful
asymptotic expansion      &#x03A6;  &#x2212; 1   ( p ) = &#x2212;   ln &#x2061;
1  p  2     &#x2212; ln &#x2061; ln &#x2061;   1  p  2     &#x2212; ln &#x2061;
( 2 &#x03C0; )   +   o   ( 1 ) .   {\displaystyle \Phi ^{-1}(p)=-{\sqrt {\ln
{\frac {1}{p^{2}}}-\ln \ln {\frac {1}{p^{2}}}-\ln(2\pi )}}+{\mathcal {o}}(1).}
[{\displaystyle \Phi ^{-1}(p)=-{\sqrt {\ln {\frac {1}{p^{2}}}-\ln \ln {\frac
{1}{p^{2}}}-\ln(2\pi )}}+{\mathcal {o}}(1).}]
***** Zero-variance limit[edit] *****
In the limit when     &#x03C3;   {\displaystyle \sigma }  [\sigma ] tends to
zero, the probability density     f ( x )   {\displaystyle f(x)}  [f(x)]
eventually tends to zero at any     x &#x2260; &#x03BC;   {\displaystyle x\neq
\mu }  [{\displaystyle x\neq \mu }], but grows without limit if     x =
&#x03BC;   {\displaystyle x=\mu }  [{\displaystyle x=\mu }], while its integral
remains equal to 1. Therefore, the normal distribution cannot be defined as an
ordinary function when     &#x03C3; = 0   {\displaystyle \sigma =0}  [\sigma
=0].
However, one can define the normal distribution with zero variance as a
generalized_function; specifically, as Dirac's_"delta_function"     &#x03B4;
{\displaystyle \delta }  [\delta ] translated by the mean     &#x03BC;
{\displaystyle \mu }  [\mu ], that is     f ( x ) = &#x03B4; ( x &#x2212;
&#x03BC; ) .   {\displaystyle f(x)=\delta (x-\mu ).}  [{\displaystyle f
(x)=\delta (x-\mu ).}] Its CDF is then the Heaviside_step_function translated
by the mean     &#x03BC;   {\displaystyle \mu }  [\mu ], namely
         F ( x ) =   {    0    if&#xA0;  x < &#x03BC;     1    if&#xA0;  x
      &#x2265; &#x03BC;         {\displaystyle F(x)={\begin{cases}0&{\text{if
      }}x<\mu \\1&{\text{if }}x\geq \mu \end{cases}}}  [{\displaystyle F(x)=
      {\begin{cases}0&{\text{if }}x<\mu \\1&{\text{if }}x\geq \mu \end
      {cases}}}]
***** Central limit theorem[edit] *****
As the number of discrete events increases, the function begins to resemble a
normal distribution
Comparison of probability density functions,     p ( k )   {\displaystyle p(k)}
[p(k)] for the sum of     n   {\displaystyle n}  [n] fair 6-sided dice to show
their convergence to a normal distribution with increasing     n a
{\displaystyle na}  [{\displaystyle na}], in accordance to the central limit
theorem. In the bottom-right graph, smoothed profiles of the previous graphs
are rescaled, superimposed and compared with a normal distribution (black
curve).
Main article: Central_limit_theorem
The central limit theorem states that under certain (fairly common) conditions,
the sum of many random variables will have an approximately normal
distribution. More specifically, where      X  1   , &#x2026; ,  X  n
{\displaystyle X_{1},\ldots ,X_{n}}  [{\displaystyle X_{1},\ldots ,X_{n}}] are
independent_and_identically_distributed random variables with the same
arbitrary distribution, zero mean, and variance      &#x03C3;  2
{\displaystyle \sigma ^{2}}  [\sigma ^{2}] and     Z   {\displaystyle Z}  [Z]
is their mean scaled by       n     {\displaystyle {\sqrt {n}}}  [{\sqrt {n}}]
         Z =   n    (    1 n    &#x2211;  i = 1   n    X  i    )
      {\displaystyle Z={\sqrt {n}}\left({\frac {1}{n}}\sum _{i=1}^{n}X_
      {i}\right)}  [Z={\sqrt {n}}\left({\frac {1}{n}}\sum _{i=1}^{n}X_
      {i}\right)]
Then, as     n   {\displaystyle n}  [n] increases, the probability distribution
of     Z   {\displaystyle Z}  [Z] will tend to the normal distribution with
zero mean and variance      &#x03C3;  2     {\displaystyle \sigma ^{2}}
[\sigma ^{2}].
The theorem can be extended to variables     (  X  i   )   {\displaystyle (X_
{i})}  [(X_{i})] that are not independent and/or not identically distributed if
certain constraints are placed on the degree of dependence and the moments of
the distributions.
Many test_statistics, scores, and estimators encountered in practice contain
sums of certain random variables in them, and even more estimators can be
represented as sums of random variables through the use of influence_functions.
The central limit theorem implies that those statistical parameters will have
asymptotically normal distributions.
The central limit theorem also implies that certain distributions can be
approximated by the normal distribution, for example:
    * The binomial_distribution     B ( n , p )   {\displaystyle B(n,p)}  [B
      (n,p)] is approximately_normal with mean     n p   {\displaystyle np}
      [np] and variance     n p ( 1 &#x2212; p )   {\displaystyle np(1-p)}  [np
      (1-p)] for large     n   {\displaystyle n}  [n] and for     p
      {\displaystyle p}  [p] not too close to 0 or 1.
    * The Poisson_distribution with parameter     &#x03BB;   {\displaystyle
      \lambda }  [\lambda ] is approximately normal with mean     &#x03BB;
      {\displaystyle \lambda }  [\lambda ] and variance     &#x03BB;
      {\displaystyle \lambda }  [\lambda ], for large values of     &#x03BB;
      {\displaystyle \lambda }  [\lambda ].[25]
    * The chi-squared_distribution      &#x03C7;  2   ( k )   {\displaystyle
      \chi ^{2}(k)}  [{\displaystyle \chi ^{2}(k)}] is approximately normal
      with mean     k   {\displaystyle k}  [k] and variance     2 k
      {\displaystyle 2k}  [2k], for large     k   {\displaystyle k}  [k].
    * The Student's_t-distribution     t ( &#x03BD; )   {\displaystyle t(\nu )}
      [{\displaystyle t(\nu )}] is approximately normal with mean 0 and
      variance 1 when     &#x03BD;   {\displaystyle \nu }  [\nu ] is large.
Whether these approximations are sufficiently accurate depends on the purpose
for which they are needed, and the rate of convergence to the normal
distribution. It is typically the case that such approximations are less
accurate in the tails of the distribution.
A general upper bound for the approximation error in the central limit theorem
is given by the BerryâEsseen_theorem, improvements of the approximation are
given by the Edgeworth_expansions.
***** Maximum entropy[edit] *****
Of all probability distributions over the reals with a specified mean
&#x03BC;   {\displaystyle \mu }  [\mu ] and variance      &#x03C3;  2
{\displaystyle \sigma ^{2}}  [\sigma ^{2}], the normal distribution     N
( &#x03BC; ,  &#x03C3;  2   )   {\displaystyle N(\mu ,\sigma ^{2})}  [N(\mu
,\sigma ^{2})] is the one with maximum_entropy.[26] If     X   {\displaystyle
X}  [X] is a continuous_random_variable with probability_density     f ( x )
{\displaystyle f(x)}  [f(x)], then the entropy of     X   {\displaystyle X}
[X] is defined as[27][28][29]
         H ( X ) = &#x2212;  &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x )
      log &#x2061; f ( x )  d x =    1 2    ( 1 + log &#x2061; ( 2  &#x03C3;  2
      &#x03C0; ) )   {\displaystyle H(X)=-\int _{-\infty }^{\infty }f(x)\log f
      (x)\,dx={\tfrac {1}{2}}(1+\log(2\sigma ^{2}\pi ))}  [{\displaystyle H
      (X)=-\int _{-\infty }^{\infty }f(x)\log f(x)\,dx={\tfrac {1}{2}}(1+\log
      (2\sigma ^{2}\pi ))}]
where     f ( x ) log &#x2061; f ( x )   {\displaystyle f(x)\log f(x)}  [
{\displaystyle f(x)\log f(x)}] is understood to be zero whenever     f ( x ) =
0   {\displaystyle f(x)=0}  [f(x)=0]. This functional can be maximized, subject
to the constraints that the distribution is properly normalized and has a
specified variance, by using variational_calculus. A function with two Lagrange
multipliers is defined:
         L =  &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x ) ln &#x2061; ( f
      ( x ) )  d x &#x2212;  &#x03BB;  0    (  1 &#x2212;  &#x222B;  &#x2212;
      &#x221E;   &#x221E;   f ( x )  d x  )  &#x2212; &#x03BB;  (   &#x03C3;  2
      &#x2212;  &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x ) ( x &#x2212;
      &#x03BC;  )  2    d x  )    {\displaystyle L=\int _{-\infty }^{\infty }f
      (x)\ln(f(x))\,dx-\lambda _{0}\left(1-\int _{-\infty }^{\infty }f
      (x)\,dx\right)-\lambda \left(\sigma ^{2}-\int _{-\infty }^{\infty }f(x)
      (x-\mu )^{2}\,dx\right)}  [{\displaystyle L=\int _{-\infty }^{\infty }f
      (x)\ln(f(x))\,dx-\lambda _{0}\left(1-\int _{-\infty }^{\infty }f
      (x)\,dx\right)-\lambda \left(\sigma ^{2}-\int _{-\infty }^{\infty }f(x)
      (x-\mu )^{2}\,dx\right)}]
where     f ( x )   {\displaystyle f(x)}  [f(x)] is, for now, regarded as some
density function with mean     &#x03BC;   {\displaystyle \mu }  [\mu ] and
standard deviation     &#x03C3;   {\displaystyle \sigma }  [\sigma ].
At maximum entropy, a small variation     &#x03B4; f ( x )   {\displaystyle
\delta f(x)}  [{\displaystyle \delta f(x)}] about     f ( x )   {\displaystyle
f(x)}  [f(x)] will produce a variation     &#x03B4; L   {\displaystyle \delta
L}  [\delta L] about     L   {\displaystyle L}  [L] which is equal to 0:
         0 = &#x03B4; L =  &#x222B;  &#x2212; &#x221E;   &#x221E;   &#x03B4; f
      ( x )  (  ln &#x2061; ( f ( x ) ) + 1 +  &#x03BB;  0   + &#x03BB; ( x
      &#x2212; &#x03BC;  )  2    )   d x   {\displaystyle 0=\delta L=\int _{-
      \infty }^{\infty }\delta f(x)\left(\ln(f(x))+1+\lambda _{0}+\lambda (x-
      \mu )^{2}\right)\,dx}  [{\displaystyle 0=\delta L=\int _{-\infty }^
      {\infty }\delta f(x)\left(\ln(f(x))+1+\lambda _{0}+\lambda (x-\mu )^
      {2}\right)\,dx}]
Since this must hold for any small     &#x03B4; f ( x )   {\displaystyle \delta
f(x)}  [{\displaystyle \delta f(x)}], the term in brackets must be zero, and
solving for     f ( x )   {\displaystyle f(x)}  [f(x)] yields:
         f ( x ) =  e  &#x2212;  &#x03BB;  0   &#x2212; 1 &#x2212; &#x03BB; ( x
      &#x2212; &#x03BC;  )  2       {\displaystyle f(x)=e^{-\lambda _{0}-1-
      \lambda (x-\mu )^{2}}}  [f(x)=e^{-\lambda _{0}-1-\lambda (x-\mu )^{2}}]
Using the constraint equations to solve for      &#x03BB;  0     {\displaystyle
\lambda _{0}}  [\lambda _{0}] and     &#x03BB;   {\displaystyle \lambda }
[\lambda ] yields the density of the normal distribution:
         f ( x , &#x03BC; , &#x03C3; ) =   1  2 &#x03C0;  &#x03C3;  2       e
      &#x2212;    ( x &#x2212; &#x03BC;  )  2     2  &#x03C3;  2
      {\displaystyle f(x,\mu ,\sigma )={\frac {1}{\sqrt {2\pi \sigma ^{2}}}}e^
      {-{\frac {(x-\mu )^{2}}{2\sigma ^{2}}}}}  [{\displaystyle f(x,\mu ,\sigma
      )={\frac {1}{\sqrt {2\pi \sigma ^{2}}}}e^{-{\frac {(x-\mu )^{2}}{2\sigma
      ^{2}}}}}]
***** Operations on normal deviates[edit] *****
The family of normal distributions is closed under linear transformations: if X
is normally distributed with mean Î¼ and standard deviation Ï, then the
variable Y = aX + b, for any real numbers a and b, is also normally
distributed, with mean aÎ¼ + b and standard deviation |a|Ï.
Also if X1 and X2 are two independent normal random variables, with means Î¼1,
Î¼2 and standard deviations Ï1, Ï2, then their sum X1 + X2 will also be
normally distributed,[proof] with mean Î¼1 + Î¼2 and variance      &#x03C3;  1
2   +  &#x03C3;  2   2     {\displaystyle \sigma _{1}^{2}+\sigma _{2}^{2}}
[\sigma _{1}^{2}+\sigma _{2}^{2}].
In particular, if X and Y are independent normal deviates with zero mean and
variance Ï2, then X + Y and X â Y are also independent and normally
distributed, with zero mean and variance 2Ï2. This is a special case of the
polarization_identity.[30]
Also, if X1, X2 are two independent normal deviates with mean Î¼ and deviation
Ï, and a, b are arbitrary real numbers, then the variable
          X  3   =    a  X  1   + b  X  2   &#x2212; ( a + b ) &#x03BC;    a  2
      +  b  2      + &#x03BC;   {\displaystyle X_{3}={\frac {aX_{1}+bX_{2}-
      (a+b)\mu }{\sqrt {a^{2}+b^{2}}}}+\mu }  [X_{3}={\frac {aX_{1}+bX_{2}-
      (a+b)\mu }{\sqrt {a^{2}+b^{2}}}}+\mu ]
is also normally distributed with mean Î¼ and deviation Ï. It follows that the
normal distribution is stable (with exponent Î± = 2).
More generally, any linear_combination of independent normal deviates is a
normal deviate.
**** Infinite divisibility and CramÃ©r's theorem[edit] ****
For any positive integer n, any normal distribution with mean Î¼ and variance
Ï2 is the distribution of the sum of n independent normal deviates, each with
mean Î¼/n and variance Ï2/n. This property is called infinite_divisibility.
[31]
Conversely, if X1 and X2 are independent random variables and their sum X1 + X2
has a normal distribution, then both X1 and X2 must be normal deviates.[32]
This result is known as CramÃ©râs_decomposition_theorem, and is equivalent to
saying that the convolution of two distributions is normal if and only if both
are normal. CramÃ©r's theorem implies that a linear combination of independent
non-Gaussian variables will never have an exactly normal distribution, although
it may approach it arbitrarily closely.[33]
**** Bernstein's theorem[edit] ****
Bernstein's theorem states that if X and Y are independent and X + Y and X â
Y are also independent, then both X and Y must necessarily have normal
distributions.[34][35]
More generally, if X1, ..., Xn are independent random variables, then two
distinct linear combinations âakXk and âbkXk will be independent if and
only if all Xk's are normal and âakbkÏ 2
k  = 0, where Ï 2
k  denotes the variance of Xk.[34]
***** Other properties[edit] *****
   1. If the characteristic function ÏX of some random variable X is of the
      form ÏX(t) = eQ(t), where Q(t) is a polynomial, then the Marcinkiewicz
      theorem (named after JÃ³zef_Marcinkiewicz) asserts that Q can be at most
      a quadratic polynomial, and therefore X is a normal random variable.[33]
      The consequence of this result is that the normal distribution is the
      only distribution with a finite number (two) of non-zero cumulants.
   2. If X and Y are jointly_normal and uncorrelated, then they are
      independent. The requirement that X and Y should be jointly normal is
      essential; without it the property does not hold.[36][37][proof] For non-
      normal random variables uncorrelatedness does not imply independence.
   3. The KullbackâLeibler_divergence of one normal distribution X1 â¼ N
      (Î¼1, Ï21 )from another X2 â¼ N(Î¼2, Ï22 )is given by:[38]
                D   K L    (  X  1    &#x2016;   X  2   ) =    (  &#x03BC;  1
            &#x2212;  &#x03BC;  2    )  2     2  &#x03C3;  2   2      +   1 2
            (     &#x03C3;  1   2    &#x03C3;  2   2     &#x2212; 1 &#x2212; ln
            &#x2061;    &#x03C3;  1   2    &#x03C3;  2   2      )  .
            {\displaystyle D_{\mathrm {KL} }(X_{1}\,\|\,X_{2})={\frac {(\mu _
            {1}-\mu _{2})^{2}}{2\sigma _{2}^{2}}}+{\frac {1}{2}}\left({\frac
            {\sigma _{1}^{2}}{\sigma _{2}^{2}}}-1-\ln {\frac {\sigma _{1}^{2}}
            {\sigma _{2}^{2}}}\right).}  [{\displaystyle D_{\mathrm {KL} }(X_
            {1}\,\|\,X_{2})={\frac {(\mu _{1}-\mu _{2})^{2}}{2\sigma _{2}^
            {2}}}+{\frac {1}{2}}\left({\frac {\sigma _{1}^{2}}{\sigma _{2}^
            {2}}}-1-\ln {\frac {\sigma _{1}^{2}}{\sigma _{2}^{2}}}\right).}]
      The Hellinger_distance between the same distributions is equal to
                H  2   (  X  1   ,  X  2   ) = 1 &#x2212;     2  &#x03C3;  1
            &#x03C3;  2      &#x03C3;  1   2   +  &#x03C3;  2   2        e
            &#x2212;   1 4      (  &#x03BC;  1   &#x2212;  &#x03BC;  2    )  2
            &#x03C3;  1   2   +  &#x03C3;  2   2        .   {\displaystyle H^
            {2}(X_{1},X_{2})=1-{\sqrt {\frac {2\sigma _{1}\sigma _{2}}{\sigma _
            {1}^{2}+\sigma _{2}^{2}}}}e^{-{\frac {1}{4}}{\frac {(\mu _{1}-\mu _
            {2})^{2}}{\sigma _{1}^{2}+\sigma _{2}^{2}}}}.}  [{\displaystyle H^
            {2}(X_{1},X_{2})=1-{\sqrt {\frac {2\sigma _{1}\sigma _{2}}{\sigma _
            {1}^{2}+\sigma _{2}^{2}}}}e^{-{\frac {1}{4}}{\frac {(\mu _{1}-\mu _
            {2})^{2}}{\sigma _{1}^{2}+\sigma _{2}^{2}}}}.}]
   4. The Fisher_information_matrix for a normal distribution is diagonal and
      takes the form
   5.      I   =   (      1  &#x03C3;  2       0     0     1  2  &#x03C3;  4
      )     {\displaystyle {\mathcal {I}}={\begin{pmatrix}{\frac {1}{\sigma ^
      {2}}}&0\\0&{\frac {1}{2\sigma ^{4}}}\end{pmatrix}}}  [{\mathcal {I}}=
      {\begin{pmatrix}{\frac {1}{\sigma ^{2}}}&0\\0&{\frac {1}{2\sigma ^
      {4}}}\end{pmatrix}}]
   6. The conjugate_prior of the mean of a normal distribution is another
      normal distribution.[39] Specifically, if x1, â¦, xn are iid N(Î¼, Ï2)
      and the prior is Î¼ ~ N(Î¼0, Ï2
      0), then the posterior distribution for the estimator of Î¼ will be
   7.    &#x03BC; &#x2223;  x  1   , &#x2026; ,  x  n   &#x223C;   N
      (        &#x03C3;  2   n    &#x03BC;  0   +  &#x03C3;  0   2      x
      &#x00AF;         &#x03C3;  2   n   +  &#x03C3;  0   2      ,   (    n
      &#x03C3;  2     +   1  &#x03C3;  0   2      )   &#x2212; 1    )
      {\displaystyle \mu \mid x_{1},\ldots ,x_{n}\sim {\mathcal {N}}\left(
      {\frac {{\frac {\sigma ^{2}}{n}}\mu _{0}+\sigma _{0}^{2}{\bar {x}}}{
      {\frac {\sigma ^{2}}{n}}+\sigma _{0}^{2}}},\left({\frac {n}{\sigma ^
      {2}}}+{\frac {1}{\sigma _{0}^{2}}}\right)^{-1}\right)}  [{\displaystyle
      \mu \mid x_{1},\ldots ,x_{n}\sim {\mathcal {N}}\left({\frac {{\frac
      {\sigma ^{2}}{n}}\mu _{0}+\sigma _{0}^{2}{\bar {x}}}{{\frac {\sigma ^{2}}
      {n}}+\sigma _{0}^{2}}},\left({\frac {n}{\sigma ^{2}}}+{\frac {1}{\sigma _
      {0}^{2}}}\right)^{-1}\right)}]
   8. The family of normal distributions not only forms an exponential_family
      (EF), but in fact forms a natural_exponential_family (NEF) with quadratic
      variance_function (NEF-QVF). Many properties of normal distributions
      generalize to properties of NEF-QVF distributions, NEF distributions, or
      EF distributions generally. NEF-QVF distributions comprises 6 families,
      including Poisson, Gamma, binomial, and negative binomial distributions,
      while many of the common families studied in probability and statistics
      are NEF or EF.
   9. In information_geometry, the family of normal distributions forms a
      statistical_manifold with constant_curvature â1. The same family is
      flat with respect to the (Â±1)-connections â(e) and â(m).[40]
***** Related distributions[edit] *****
**** Operations on a single random variable[edit] ****
If X is distributed normally with mean Î¼ and variance Ï2, then
    * The exponential of X is distributed log-normally: eX ~ ln(N (Î¼, Ï2)).
    * The absolute value of X has folded_normal_distribution: |X| ~ Nf (Î¼,
      Ï2). If Î¼ = 0 this is known as the half-normal_distribution.
    * The absolute value of normalized residuals, |X â Î¼|/Ï, has chi
      distribution with one degree of freedom: |X â Î¼|/Ï ~ Ï1(|X â Î¼|/
      Ï).
    * The square of X/Ï has the noncentral_chi-squared_distribution with one
      degree of freedom: X2/Ï2 ~ Ï21(Î¼2/Ï2). If Î¼ = 0, the distribution is
      called simply chi-squared.
    * The distribution of the variable X restricted to an interval [a, b] is
      called the truncated_normal_distribution.
    * (X â Î¼)â2 has a LÃ©vy_distribution with location 0 and scale Ïâ2.
**** Combination of two independent random variables[edit] ****
If X1 and X2 are two independent standard normal random variables with mean 0
and variance 1, then
    * Their sum and difference is distributed normally with mean zero and
      variance two: X1 Â± X2 â¼ N(0, 2).
    * Their product Z = X1Â·X2 follows the "product-normal" distribution[41]
      with density function fZ(z) = Ïâ1K0(|z|), where K0 is the modified
      Bessel_function_of_the_second_kind. This distribution is symmetric around
      zero, unbounded at z = 0, and has the characteristic_function ÏZ(t) = (1
      + t2)â1/2.
    * Their ratio follows the standard Cauchy_distribution: X1 / X2 â¼ Cauchy
      (0, 1).
    * Their Euclidean norm        X  1   2   +  X  2   2       {\displaystyle
      {\sqrt {X_{1}^{2}+X_{2}^{2}}}}  [{\displaystyle {\sqrt {X_{1}^{2}+X_{2}^
      {2}}}}] has the Rayleigh_distribution.
**** Combination of two or more independent random variables[edit] ****
    * If X1, X2, ..., Xn are independent standard normal random variables, then
      the sum of their squares has the chi-squared_distribution with n degrees
      of freedom
                X  1   2   + &#x22EF; +  X  n   2   &#x223C;  &#x03C7;  n   2
            .   {\displaystyle X_{1}^{2}+\cdots +X_{n}^{2}\sim \chi _{n}^{2}.}
            [{\displaystyle X_{1}^{2}+\cdots +X_{n}^{2}\sim \chi _{n}^{2}.}]
    * If X1, X2, ..., Xn are independent normally distributed random variables
      with means Î¼ and variances Ï2, then their sample_mean is independent
      from the sample standard_deviation,[42] which can be demonstrated using
      Basu's_theorem or Cochran's_theorem.[43] The ratio of these two
      quantities will have the Student's_t-distribution with n â 1 degrees of
      freedom:
               t =      X &#x00AF;   &#x2212; &#x03BC;   S  /    n      =
            1 n   (  X  1   + &#x22EF; +  X  n   ) &#x2212; &#x03BC;     1  n
            ( n &#x2212; 1 )     [  (  X  1   &#x2212;   X &#x00AF;    )  2   +
            &#x22EF; + (  X  n   &#x2212;   X &#x00AF;    )  2    ]
            &#x223C;  t  n &#x2212; 1   .   {\displaystyle t={\frac {{\overline
            {X}}-\mu }{S/{\sqrt {n}}}}={\frac {{\frac {1}{n}}(X_{1}+\cdots +X_
            {n})-\mu }{\sqrt {{\frac {1}{n(n-1)}}\left[(X_{1}-{\overline {X}})^
            {2}+\cdots +(X_{n}-{\overline {X}})^{2}\right]}}}\sim t_{n-1}.}  [
            {\displaystyle t={\frac {{\overline {X}}-\mu }{S/{\sqrt {n}}}}=
            {\frac {{\frac {1}{n}}(X_{1}+\cdots +X_{n})-\mu }{\sqrt {{\frac {1}
            {n(n-1)}}\left[(X_{1}-{\overline {X}})^{2}+\cdots +(X_{n}-
            {\overline {X}})^{2}\right]}}}\sim t_{n-1}.}]
    * ' If X1, ..., Xn, Y1, ..., Ym are independent standard normal random
      variables, then the ratio of their normalized sums of squares will have
      the F-distribution with (n, m) degrees of freedom:[44]
               F =     (   X  1   2   +  X  2   2   + &#x22EF; +  X  n   2    )
            /  n    (   Y  1   2   +  Y  2   2   + &#x22EF; +  Y  m   2    )
            /  m    &#x223C;  F  n , m   .   {\displaystyle F={\frac {\left(X_
            {1}^{2}+X_{2}^{2}+\cdots +X_{n}^{2}\right)/n}{\left(Y_{1}^{2}+Y_
            {2}^{2}+\cdots +Y_{m}^{2}\right)/m}}\sim F_{n,m}.}  [{\displaystyle
            F={\frac {\left(X_{1}^{2}+X_{2}^{2}+\cdots +X_{n}^{2}\right)/n}
            {\left(Y_{1}^{2}+Y_{2}^{2}+\cdots +Y_{m}^{2}\right)/m}}\sim F_
            {n,m}.}]
**** Operations on the density function[edit] ****
The split_normal_distribution is most directly defined in terms of joining
scaled sections of the density functions of different normal distributions and
rescaling the density to integrate to one. The truncated_normal_distribution
results from rescaling a section of a single density function.
**** Extensions[edit] ****
The notion of normal distribution, being one of the most important
distributions in probability theory, has been extended far beyond the standard
framework of the univariate (that is one-dimensional) case (Case 1). All these
extensions are also called normal or Gaussian laws, so a certain ambiguity in
names exists.
    * The multivariate_normal_distribution describes the Gaussian law in the k-
      dimensional Euclidean_space. A vector X â Rk is multivariate-normally
      distributed if any linear combination of its components âk
      j=1aj Xj has a (univariate) normal distribution. The variance of X is a
      kÃk symmetric positive-definite matrix V. The multivariate normal
      distribution is a special case of the elliptical_distributions. As such,
      its iso-density loci in the k = 2 case are ellipses and in the case of
      arbitrary k are ellipsoids.
    * Rectified_Gaussian_distribution a rectified version of normal
      distribution with all the negative elements reset to 0
    * Complex_normal_distribution deals with the complex normal vectors. A
      complex vector X â Ck is said to be normal if both its real and
      imaginary components jointly possess a 2k-dimensional multivariate normal
      distribution. The variance-covariance structure of X is described by two
      matrices: the variance matrix Î, and the relation matrix C.
    * Matrix_normal_distribution describes the case of normally distributed
      matrices.
    * Gaussian_processes are the normally distributed stochastic_processes.
      These can be viewed as elements of some infinite-dimensional Hilbert
      space H, and thus are the analogues of multivariate normal vectors for
      the case k = â. A random element h â H is said to be normal if for
      any constant a â H the scalar_product (a, h) has a (univariate) normal
      distribution. The variance structure of such Gaussian random element can
      be described in terms of the linear covariance operator K: H â H.
      Several Gaussian processes became popular enough to have their own names:
          o Brownian_motion,
          o Brownian_bridge,
          o OrnsteinâUhlenbeck_process.
    * Gaussian_q-distribution is an abstract mathematical construction that
      represents a "q-analogue" of the normal distribution.
    * the q-Gaussian is an analogue of the Gaussian distribution, in the sense
      that it maximises the Tsallis_entropy, and is one type of Tsallis
      distribution. Note that this distribution is different from the Gaussian
      q-distribution above.
A random variable X has a two-piece normal distribution if it has a
distribution
          f  X   ( x ) = N ( &#x03BC; ,  &#x03C3;  1   2   )  &#xA0;if&#xA0;  x
      &#x2264; &#x03BC;   {\displaystyle f_{X}(x)=N(\mu ,\sigma _{1}^{2}){\text
      { if }}x\leq \mu }  [{\displaystyle f_{X}(x)=N(\mu ,\sigma _{1}^{2})
      {\text{ if }}x\leq \mu }]
          f  X   ( x ) = N ( &#x03BC; ,  &#x03C3;  2   2   )  &#xA0;if&#xA0;  x
      &#x2265; &#x03BC;   {\displaystyle f_{X}(x)=N(\mu ,\sigma _{2}^{2}){\text
      { if }}x\geq \mu }  [{\displaystyle f_{X}(x)=N(\mu ,\sigma _{2}^{2})
      {\text{ if }}x\geq \mu }]
where Î¼ is the mean and Ï1 and Ï2 are the standard deviations of the
distribution to the left and right of the mean respectively.
The mean, variance and third central moment of this distribution have been
determined[45]
         E &#x2061; ( X ) = &#x03BC; +    2 &#x03C0;    (  &#x03C3;  2
      &#x2212;  &#x03C3;  1   )   {\displaystyle \operatorname {E} (X)=\mu +
      {\sqrt {\frac {2}{\pi }}}(\sigma _{2}-\sigma _{1})}  [{\displaystyle
      \operatorname {E} (X)=\mu +{\sqrt {\frac {2}{\pi }}}(\sigma _{2}-\sigma _
      {1})}]
         V &#x2061; ( X ) =  (  1 &#x2212;   2 &#x03C0;    )  (  &#x03C3;  2
      &#x2212;  &#x03C3;  1    )  2   +  &#x03C3;  1    &#x03C3;  2
      {\displaystyle \operatorname {V} (X)=\left(1-{\frac {2}{\pi }}\right)
      (\sigma _{2}-\sigma _{1})^{2}+\sigma _{1}\sigma _{2}}  [{\displaystyle
      \operatorname {V} (X)=\left(1-{\frac {2}{\pi }}\right)(\sigma _{2}-\sigma
      _{1})^{2}+\sigma _{1}\sigma _{2}}]
         T &#x2061; ( X ) =    2 &#x03C0;    (  &#x03C3;  2   &#x2212;
      &#x03C3;  1   )  [   (    4 &#x03C0;   &#x2212; 1  )  (  &#x03C3;  2
      &#x2212;  &#x03C3;  1    )  2   +  &#x03C3;  1    &#x03C3;  2    ]
      {\displaystyle \operatorname {T} (X)={\sqrt {\frac {2}{\pi }}}(\sigma _
      {2}-\sigma _{1})\left[\left({\frac {4}{\pi }}-1\right)(\sigma _{2}-\sigma
      _{1})^{2}+\sigma _{1}\sigma _{2}\right]}  [{\displaystyle \operatorname
      {T} (X)={\sqrt {\frac {2}{\pi }}}(\sigma _{2}-\sigma _{1})\left[\left(
      {\frac {4}{\pi }}-1\right)(\sigma _{2}-\sigma _{1})^{2}+\sigma _{1}\sigma
      _{2}\right]}]
where E(X), V(X) and T(X) are the mean, variance, and third central moment
respectively.
One of the main practical uses of the Gaussian law is to model the empirical
distributions of many different random variables encountered in practice. In
such case a possible extension would be a richer family of distributions,
having more than two parameters and therefore being able to fit the empirical
distribution more accurately. The examples of such extensions are:
    * Pearson_distribution â a four-parameter family of probability
      distributions that extend the normal law to include different skewness
      and kurtosis values.
    * The generalized_normal_distribution, also known as the exponential power
      distribution, allows for distribution tails with thicker or thinner
      asymptotic behaviors.
***** Normality tests[edit] *****
Main article: Normality_tests
Normality tests assess the likelihood that the given data set {x1, ..., xn}
comes from a normal distribution. Typically the null_hypothesis H0 is that the
observations are distributed normally with unspecified mean Î¼ and variance
Ï2, versus the alternative Ha that the distribution is arbitrary. Many tests
(over 40) have been devised for this problem, the more prominent of them are
outlined below:
    * "Visual" tests are more intuitively appealing but subjective at the same
      time, as they rely on informal human judgement to accept or reject the
      null hypothesis.
          o Q-Q_plotâ is a plot of the sorted values from the data set
            against the expected values of the corresponding quantiles from the
            standard normal distribution. That is, it's a plot of point of the
            form (Î¦â1(pk), x(k)), where plotting points pk are equal to
            pk = (k â Î±)/(n + 1 â 2Î±) and Î± is an adjustment constant,
            which can be anything between 0 and 1. If the null hypothesis is
            true, the plotted points should approximately lie on a straight
            line.
          o P-P_plotâ similar to the Q-Q plot, but used much less frequently.
            This method consists of plotting the points (Î¦(z(k)), pk), where
            z  ( k )   = (  x  ( k )   &#x2212;    &#x03BC; &#x005E;    )  /
            &#x03C3; &#x005E;       {\displaystyle \textstyle z_{(k)}=(x_{(k)}-
            {\hat {\mu }})/{\hat {\sigma }}}  [{\displaystyle \textstyle z_{
            (k)}=(x_{(k)}-{\hat {\mu }})/{\hat {\sigma }}}]. For normally
            distributed data this plot should lie on a 45Â° line between (0, 0)
            and (1, 1).
          o Shapiro-Wilk_test employs the fact that the line in the Q-Q plot
            has the slope of Ï. The test compares the least squares estimate
            of that slope with the value of the sample variance, and rejects
            the null hypothesis if these two quantities differ significantly.
          o Normal_probability_plot (rankit plot)
    * Moment tests:
          o D'Agostino's_K-squared_test
          o JarqueâBera_test
    * Empirical distribution function tests:
          o Lilliefors_test (an adaptation of the KolmogorovâSmirnov_test)
          o AndersonâDarling_test
***** Estimation of parameters[edit] *****
See also: Maximum_likelihood_Â§ Continuous_distribution,_continuous_parameter
space
It is often the case that we don't know the parameters of the normal
distribution, but instead want to estimate them. That is, having a sample (x1,
..., xn) from a normal N(Î¼, Ï2) population we would like to learn the
approximate values of parameters Î¼ and Ï2. The standard approach to this
problem is the maximum_likelihood method, which requires maximization of the
log-likelihood function:
         ln &#x2061;   L   ( &#x03BC; ,  &#x03C3;  2   ) =  &#x2211;  i = 1   n
      ln &#x2061; f (  x  i   &#x2223; &#x03BC; ,  &#x03C3;  2   ) = &#x2212;
      n 2   ln &#x2061; ( 2 &#x03C0; ) &#x2212;   n 2   ln &#x2061;  &#x03C3;
      2   &#x2212;   1  2  &#x03C3;  2       &#x2211;  i = 1   n   (  x  i
      &#x2212; &#x03BC;  )  2   .   {\displaystyle \ln {\mathcal {L}}(\mu
      ,\sigma ^{2})=\sum _{i=1}^{n}\ln f(x_{i}\mid \mu ,\sigma ^{2})=-{\frac
      {n}{2}}\ln(2\pi )-{\frac {n}{2}}\ln \sigma ^{2}-{\frac {1}{2\sigma ^
      {2}}}\sum _{i=1}^{n}(x_{i}-\mu )^{2}.}  [{\displaystyle \ln {\mathcal
      {L}}(\mu ,\sigma ^{2})=\sum _{i=1}^{n}\ln f(x_{i}\mid \mu ,\sigma ^{2})=-
      {\frac {n}{2}}\ln(2\pi )-{\frac {n}{2}}\ln \sigma ^{2}-{\frac {1}{2\sigma
      ^{2}}}\sum _{i=1}^{n}(x_{i}-\mu )^{2}.}]
Taking derivatives with respect to Î¼ and Ï2 and solving the resulting system
of first order conditions yields the maximum likelihood estimates:
            &#x03BC; &#x005E;    =   x &#x00AF;   &#x2261;   1 n    &#x2211;  i
      = 1   n    x  i   ,      &#x03C3; &#x005E;     2   =   1 n    &#x2211;  i
      = 1   n   (  x  i   &#x2212;   x &#x00AF;    )  2   .   {\displaystyle
      {\hat {\mu }}={\overline {x}}\equiv {\frac {1}{n}}\sum _{i=1}^{n}x_
      {i},\qquad {\hat {\sigma }}^{2}={\frac {1}{n}}\sum _{i=1}^{n}(x_{i}-
      {\overline {x}})^{2}.}  [{\hat {\mu }}={\overline {x}}\equiv {\frac {1}
      {n}}\sum _{i=1}^{n}x_{i},\qquad {\hat {\sigma }}^{2}={\frac {1}{n}}\sum _
      {i=1}^{n}(x_{i}-{\overline {x}})^{2}.]
**** Sample mean[edit] ****
See also: Standard_error_of_the_mean
Estimator         &#x03BC; &#x005E;       {\displaystyle \textstyle {\hat {\mu
}}}  [{\displaystyle \textstyle {\hat {\mu }}}] is called the sample_mean,
since it is the arithmetic mean of all observations. The statistic        x
&#x00AF;      {\displaystyle \textstyle {\overline {x}}}  [{\displaystyle
\textstyle {\overline {x}}}] is complete and sufficient for Î¼, and therefore
by the LehmannâScheffÃ©_theorem,         &#x03BC; &#x005E;
{\displaystyle \textstyle {\hat {\mu }}}  [{\displaystyle \textstyle {\hat {\mu
}}}] is the uniformly_minimum_variance_unbiased (UMVU) estimator.[46] In finite
samples it is distributed normally:
            &#x03BC; &#x005E;    &#x223C;   N   ( &#x03BC; ,  &#x03C3;  2    /
      n ) .   {\displaystyle {\hat {\mu }}\sim {\mathcal {N}}(\mu ,\sigma ^{2}/
      n).}  [{\displaystyle {\hat {\mu }}\sim {\mathcal {N}}(\mu ,\sigma ^{2}/
      n).}]
The variance of this estimator is equal to the Î¼Î¼-element of the inverse
Fisher_information_matrix         I    &#x2212; 1      {\displaystyle
\textstyle {\mathcal {I}}^{-1}}  [{\displaystyle \textstyle {\mathcal {I}}^{-
1}}]. This implies that the estimator is finite-sample_efficient. Of practical
importance is the fact that the standard_error of         &#x03BC; &#x005E;
{\displaystyle \textstyle {\hat {\mu }}}  [{\displaystyle \textstyle {\hat {\mu
}}}] is proportional to      1  /    n      {\displaystyle \textstyle 1/{\sqrt
{n}}}  [{\displaystyle \textstyle 1/{\sqrt {n}}}], that is, if one wishes to
decrease the standard error by a factor of 10, one must increase the number of
points in the sample by a factor of 100. This fact is widely used in
determining sample sizes for opinion polls and the number of trials in Monte
Carlo_simulations.
From the standpoint of the asymptotic_theory,         &#x03BC; &#x005E;
{\displaystyle \textstyle {\hat {\mu }}}  [{\displaystyle \textstyle {\hat {\mu
}}}] is consistent, that is, it converges_in_probability to Î¼ as n â â.
The estimator is also asymptotically_normal, which is a simple corollary of the
fact that it is normal in finite samples:
           n   (    &#x03BC; &#x005E;    &#x2212; &#x03BC; )    &#x2192;  d
      N   ( 0 ,  &#x03C3;  2   ) .   {\displaystyle {\sqrt {n}}({\hat {\mu }}-
      \mu )\,{\xrightarrow {d}}\,{\mathcal {N}}(0,\sigma ^{2}).}  [
      {\displaystyle {\sqrt {n}}({\hat {\mu }}-\mu )\,{\xrightarrow {d}}\,
      {\mathcal {N}}(0,\sigma ^{2}).}]
**** Sample variance[edit] ****
See also: Standard_deviation_Â§ Estimation, and Variance_Â§ Estimation
The estimator          &#x03C3; &#x005E;     2      {\displaystyle \textstyle
{\hat {\sigma }}^{2}}  [{\displaystyle \textstyle {\hat {\sigma }}^{2}}] is
called the sample_variance, since it is the variance of the sample (x1, ...,
xn). In practice, another estimator is often used instead of the
&#x03C3; &#x005E;     2      {\displaystyle \textstyle {\hat {\sigma }}^{2}}  [
{\displaystyle \textstyle {\hat {\sigma }}^{2}}]. This other estimator is
denoted s2, and is also called the sample variance, which represents a certain
ambiguity in terminology; its square root s is called the sample standard
deviation. The estimator s2 differs from          &#x03C3; &#x005E;     2
{\displaystyle \textstyle {\hat {\sigma }}^{2}}  [{\displaystyle \textstyle
{\hat {\sigma }}^{2}}] by having (n â 1) instead of n in the denominator (the
so-called Bessel's_correction):
          s  2   =   n  n &#x2212; 1        &#x03C3; &#x005E;     2   =   1  n
      &#x2212; 1     &#x2211;  i = 1   n   (  x  i   &#x2212;   x &#x00AF;    )
      2   .   {\displaystyle s^{2}={\frac {n}{n-1}}{\hat {\sigma }}^{2}={\frac
      {1}{n-1}}\sum _{i=1}^{n}(x_{i}-{\overline {x}})^{2}.}  [{\displaystyle s^
      {2}={\frac {n}{n-1}}{\hat {\sigma }}^{2}={\frac {1}{n-1}}\sum _{i=1}^{n}
      (x_{i}-{\overline {x}})^{2}.}]
The difference between s2 and          &#x03C3; &#x005E;     2
{\displaystyle \textstyle {\hat {\sigma }}^{2}}  [{\displaystyle \textstyle
{\hat {\sigma }}^{2}}] becomes negligibly small for large n's. In finite
samples however, the motivation behind the use of s2 is that it is an unbiased
estimator of the underlying parameter Ï2, whereas          &#x03C3; &#x005E;
2      {\displaystyle \textstyle {\hat {\sigma }}^{2}}  [{\displaystyle
\textstyle {\hat {\sigma }}^{2}}] is biased. Also, by the LehmannâScheffÃ©
theorem the estimator s2 is uniformly minimum variance unbiased (UMVU),[46]
which makes it the "best" estimator among all unbiased ones. However it can be
shown that the biased estimator          &#x03C3; &#x005E;     2
{\displaystyle \textstyle {\hat {\sigma }}^{2}}  [{\displaystyle \textstyle
{\hat {\sigma }}^{2}}] is "better" than the s2 in terms of the mean_squared
error (MSE) criterion. In finite samples both s2 and          &#x03C3; &#x005E;
2      {\displaystyle \textstyle {\hat {\sigma }}^{2}}  [{\displaystyle
\textstyle {\hat {\sigma }}^{2}}] have scaled chi-squared_distribution with (n
â 1) degrees of freedom:
          s  2   &#x223C;    &#x03C3;  2    n &#x2212; 1    &#x22C5;  &#x03C7;
      n &#x2212; 1   2   ,      &#x03C3; &#x005E;     2   &#x223C;    &#x03C3;
      2   n   &#x22C5;  &#x03C7;  n &#x2212; 1   2   .   {\displaystyle s^
      {2}\sim {\frac {\sigma ^{2}}{n-1}}\cdot \chi _{n-1}^{2},\qquad {\hat
      {\sigma }}^{2}\sim {\frac {\sigma ^{2}}{n}}\cdot \chi _{n-1}^{2}.}  [
      {\displaystyle s^{2}\sim {\frac {\sigma ^{2}}{n-1}}\cdot \chi _{n-1}^
      {2},\qquad {\hat {\sigma }}^{2}\sim {\frac {\sigma ^{2}}{n}}\cdot \chi _
      {n-1}^{2}.}]
The first of these expressions shows that the variance of s2 is equal to 2Ï4/
(nâ1), which is slightly greater than the ÏÏ-element of the inverse Fisher
information matrix         I    &#x2212; 1      {\displaystyle \textstyle
{\mathcal {I}}^{-1}}  [{\displaystyle \textstyle {\mathcal {I}}^{-1}}]. Thus,
s2 is not an efficient estimator for Ï2, and moreover, since s2 is UMVU, we
can conclude that the finite-sample efficient estimator for Ï2 does not exist.
Applying the asymptotic theory, both estimators s2 and          &#x03C3;
&#x005E;     2      {\displaystyle \textstyle {\hat {\sigma }}^{2}}  [
{\displaystyle \textstyle {\hat {\sigma }}^{2}}] are consistent, that is they
converge in probability to Ï2 as the sample size n â â. The two estimators
are also both asymptotically normal:
           n   (     &#x03C3; &#x005E;     2   &#x2212;  &#x03C3;  2   )
      &#x2243;   n   (  s  2   &#x2212;  &#x03C3;  2   )    &#x2192;  d       N
      ( 0 , 2  &#x03C3;  4   ) .   {\displaystyle {\sqrt {n}}({\hat {\sigma }}^
      {2}-\sigma ^{2})\simeq {\sqrt {n}}(s^{2}-\sigma ^{2})\,{\xrightarrow
      {d}}\,{\mathcal {N}}(0,2\sigma ^{4}).}  [{\displaystyle {\sqrt {n}}({\hat
      {\sigma }}^{2}-\sigma ^{2})\simeq {\sqrt {n}}(s^{2}-\sigma ^{2})\,
      {\xrightarrow {d}}\,{\mathcal {N}}(0,2\sigma ^{4}).}]
In particular, both estimators are asymptotically efficient for Ï2.
**** Confidence intervals[edit] ****
See also: Studentization
By Cochran's_theorem, for normal distributions the sample mean         &#x03BC;
&#x005E;       {\displaystyle \textstyle {\hat {\mu }}}  [{\displaystyle
\textstyle {\hat {\mu }}}] and the sample variance s2 are independent, which
means there can be no gain in considering their joint_distribution. There is
also a converse theorem: if in a sample the sample mean and sample variance are
independent, then the sample must have come from the normal distribution. The
independence between         &#x03BC; &#x005E;       {\displaystyle \textstyle
{\hat {\mu }}}  [{\displaystyle \textstyle {\hat {\mu }}}] and s can be
employed to construct the so-called t-statistic:
         t =       &#x03BC; &#x005E;    &#x2212; &#x03BC;   s  /    n      =
      x &#x00AF;   &#x2212; &#x03BC;     1  n ( n &#x2212; 1 )    &#x2211; (  x
      i   &#x2212;   x &#x00AF;    )  2      &#x223C;  t  n &#x2212; 1
      {\displaystyle t={\frac {{\hat {\mu }}-\mu }{s/{\sqrt {n}}}}={\frac {
      {\overline {x}}-\mu }{\sqrt {{\frac {1}{n(n-1)}}\sum (x_{i}-{\overline
      {x}})^{2}}}}\sim t_{n-1}}  [{\displaystyle t={\frac {{\hat {\mu }}-\mu }
      {s/{\sqrt {n}}}}={\frac {{\overline {x}}-\mu }{\sqrt {{\frac {1}{n(n-
      1)}}\sum (x_{i}-{\overline {x}})^{2}}}}\sim t_{n-1}}]
This quantity t has the Student's_t-distribution with (n â 1) degrees of
freedom, and it is an ancillary_statistic (independent of the value of the
parameters). Inverting the distribution of this t-statistics will allow us to
construct the confidence_interval for Î¼;[47] similarly, inverting the Ï2
distribution of the statistic s2 will give us the confidence interval for Ï2:
[48]
         &#x03BC; &#x2208;  [     &#x03BC; &#x005E;    &#x2212;  t  n &#x2212;
      1 , 1 &#x2212; &#x03B1;  /  2     1  n    s ,    &#x03BC; &#x005E;    +
      t  n &#x2212; 1 , 1 &#x2212; &#x03B1;  /  2     1  n    s  ]  &#x2248;
      [     &#x03BC; &#x005E;    &#x2212;  |   z  &#x03B1;  /  2    |    1  n
      s ,    &#x03BC; &#x005E;    +  |   z  &#x03B1;  /  2    |    1  n    s  ]
      ,   {\displaystyle \mu \in \left[{\hat {\mu }}-t_{n-1,1-\alpha /2}{\frac
      {1}{\sqrt {n}}}s,{\hat {\mu }}+t_{n-1,1-\alpha /2}{\frac {1}{\sqrt
      {n}}}s\right]\approx \left[{\hat {\mu }}-|z_{\alpha /2}|{\frac {1}{\sqrt
      {n}}}s,{\hat {\mu }}+|z_{\alpha /2}|{\frac {1}{\sqrt {n}}}s\right],}  [
      {\displaystyle \mu \in \left[{\hat {\mu }}-t_{n-1,1-\alpha /2}{\frac {1}
      {\sqrt {n}}}s,{\hat {\mu }}+t_{n-1,1-\alpha /2}{\frac {1}{\sqrt
      {n}}}s\right]\approx \left[{\hat {\mu }}-|z_{\alpha /2}|{\frac {1}{\sqrt
      {n}}}s,{\hat {\mu }}+|z_{\alpha /2}|{\frac {1}{\sqrt {n}}}s\right],}]
          &#x03C3;  2   &#x2208;  [     ( n &#x2212; 1 )  s  2     &#x03C7;  n
      &#x2212; 1 , 1 &#x2212; &#x03B1;  /  2   2     ,    ( n &#x2212; 1 )  s
      2     &#x03C7;  n &#x2212; 1 , &#x03B1;  /  2   2      ]  &#x2248;  [   s
      2   &#x2212;  |   z  &#x03B1;  /  2    |     2   n     s  2   ,  s  2   +
      |   z  &#x03B1;  /  2    |     2   n     s  2    ]  ,   {\displaystyle
      \sigma ^{2}\in \left[{\frac {(n-1)s^{2}}{\chi _{n-1,1-\alpha /2}^{2}}},
      {\frac {(n-1)s^{2}}{\chi _{n-1,\alpha /2}^{2}}}\right]\approx \left[s^
      {2}-|z_{\alpha /2}|{\frac {\sqrt {2}}{\sqrt {n}}}s^{2},s^{2}+|z_{\alpha /
      2}|{\frac {\sqrt {2}}{\sqrt {n}}}s^{2}\right],}  [{\displaystyle \sigma ^
      {2}\in \left[{\frac {(n-1)s^{2}}{\chi _{n-1,1-\alpha /2}^{2}}},{\frac {
      (n-1)s^{2}}{\chi _{n-1,\alpha /2}^{2}}}\right]\approx \left[s^{2}-|z_
      {\alpha /2}|{\frac {\sqrt {2}}{\sqrt {n}}}s^{2},s^{2}+|z_{\alpha /2}|
      {\frac {\sqrt {2}}{\sqrt {n}}}s^{2}\right],}]
where tk,p and Ï 2
k,p  are the pth quantiles of the t- and Ï2-distributions respectively. These
confidence intervals are of the confidence_level 1 â Î±, meaning that the
true values Î¼ and Ï2 fall outside of these intervals with probability (or
significance_level) Î±. In practice people usually take Î± = 5%, resulting in
the 95% confidence intervals. The approximate formulas in the display above
were derived from the asymptotic distributions of         &#x03BC; &#x005E;
{\displaystyle \textstyle {\hat {\mu }}}  [{\displaystyle \textstyle {\hat {\mu
}}}] and s2. The approximate formulas become valid for large values of n, and
are more convenient for the manual calculation since the standard normal
quantiles zÎ±/2 do not depend on n. In particular, the most popular value of Î±
= 5%, results in |z0.025| = 1.96.
***** Bayesian analysis of the normal distribution[edit] *****
Bayesian analysis of normally distributed data is complicated by the many
different possibilities that may be considered:
    * Either the mean, or the variance, or neither, may be considered a fixed
      quantity.
    * When the variance is unknown, analysis may be done directly in terms of
      the variance, or in terms of the precision, the reciprocal of the
      variance. The reason for expressing the formulas in terms of precision is
      that the analysis of most cases is simplified.
    * Both univariate and multivariate cases need to be considered.
    * Either conjugate or improper prior_distributions may be placed on the
      unknown variables.
    * An additional set of cases occurs in Bayesian_linear_regression, where in
      the basic model the data is assumed to be normally distributed, and
      normal priors are placed on the regression_coefficients. The resulting
      analysis is similar to the basic cases of independent_identically
      distributed data, but more complex.
The formulas for the non-linear-regression cases are summarized in the
conjugate_prior article.
**** Sum of two quadratics[edit] ****
*** Scalar form[edit] ***
The following auxiliary formula is useful for simplifying the posterior update
equations, which otherwise become fairly tedious.
         a ( x &#x2212; y  )  2   + b ( x &#x2212; z  )  2   = ( a + b )   (  x
      &#x2212;    a y + b z   a + b     )   2   +    a b   a + b    ( y
      &#x2212; z  )  2     {\displaystyle a(x-y)^{2}+b(x-z)^{2}=(a+b)\left(x-
      {\frac {ay+bz}{a+b}}\right)^{2}+{\frac {ab}{a+b}}(y-z)^{2}}  [a(x-y)^
      {2}+b(x-z)^{2}=(a+b)\left(x-{\frac {ay+bz}{a+b}}\right)^{2}+{\frac {ab}
      {a+b}}(y-z)^{2}]
This equation rewrites the sum of two quadratics in x by expanding the squares,
grouping the terms in x, and completing_the_square. Note the following about
the complex constant factors attached to some of the terms:
   1. The factor        a y + b z   a + b      {\displaystyle {\frac {ay+bz}
      {a+b}}}  [{\frac {ay+bz}{a+b}}] has the form of a weighted_average of y
      and z.
   2.       a b   a + b    =   1    1 a   +   1 b      = (  a  &#x2212; 1   +
      b  &#x2212; 1    )  &#x2212; 1   .   {\displaystyle {\frac {ab}{a+b}}=
      {\frac {1}{{\frac {1}{a}}+{\frac {1}{b}}}}=(a^{-1}+b^{-1})^{-1}.}  [
      {\frac {ab}{a+b}}={\frac {1}{{\frac {1}{a}}+{\frac {1}{b}}}}=(a^{-1}+b^{-
      1})^{-1}.] This shows that this factor can be thought of as resulting
      from a situation where the reciprocals of quantities a and b add
      directly, so to combine a and b themselves, it's necessary to
      reciprocate, add, and reciprocate the result again to get back into the
      original units. This is exactly the sort of operation performed by the
      harmonic_mean, so it is not surprising that        a b   a + b
      {\displaystyle {\frac {ab}{a+b}}}  [{\frac {ab}{a+b}}] is one-half the
      harmonic_mean of a and b.
*** Vector form[edit] ***
A similar formula can be written for the sum of two vector quadratics: If x, y,
z are vectors of length k, and A and B are symmetric, invertible_matrices of
size     k &#x00D7; k   {\displaystyle k\times k}  [k\times k], then
               (  y  &#x2212;  x   ) &#x2032;   A  (  y  &#x2212;  x  ) + (  x
      &#x2212;  z   ) &#x2032;   B  (  x  &#x2212;  z  )     =      (  x
      &#x2212;  c   ) &#x2032;  (  A  +  B  ) (  x  &#x2212;  c  ) + (  y
      &#x2212;  z   ) &#x2032;  (   A   &#x2212; 1   +   B   &#x2212; 1    )
      &#x2212; 1   (  y  &#x2212;  z  )       {\displaystyle {\begin{aligned}&
      (\mathbf {y} -\mathbf {x} )'\mathbf {A} (\mathbf {y} -\mathbf {x} )+
      (\mathbf {x} -\mathbf {z} )'\mathbf {B} (\mathbf {x} -\mathbf {z} )\\={}&
      (\mathbf {x} -\mathbf {c} )'(\mathbf {A} +\mathbf {B} )(\mathbf {x} -
      \mathbf {c} )+(\mathbf {y} -\mathbf {z} )'(\mathbf {A} ^{-1}+\mathbf {B}
      ^{-1})^{-1}(\mathbf {y} -\mathbf {z} )\end{aligned}}}  [{\displaystyle
      {\begin{aligned}&(\mathbf {y} -\mathbf {x} )'\mathbf {A} (\mathbf {y} -
      \mathbf {x} )+(\mathbf {x} -\mathbf {z} )'\mathbf {B} (\mathbf {x} -
      \mathbf {z} )\\={}&(\mathbf {x} -\mathbf {c} )'(\mathbf {A} +\mathbf {B}
      )(\mathbf {x} -\mathbf {c} )+(\mathbf {y} -\mathbf {z} )'(\mathbf {A} ^{-
      1}+\mathbf {B} ^{-1})^{-1}(\mathbf {y} -\mathbf {z} )\end{aligned}}}]
where
          c  = (  A  +  B   )  &#x2212; 1   (  A   y  +  B   z  )
      {\displaystyle \mathbf {c} =(\mathbf {A} +\mathbf {B} )^{-1}(\mathbf {A}
      \mathbf {y} +\mathbf {B} \mathbf {z} )}  [{\displaystyle \mathbf {c} =
      (\mathbf {A} +\mathbf {B} )^{-1}(\mathbf {A} \mathbf {y} +\mathbf {B}
      \mathbf {z} )}]
Note that the form xâ² A x is called a quadratic_form and is a scalar:
           x  &#x2032;   A   x  =  &#x2211;  i , j    a  i j    x  i    x  j
      {\displaystyle \mathbf {x} '\mathbf {A} \mathbf {x} =\sum _{i,j}a_{ij}x_
      {i}x_{j}}  [\mathbf {x} '\mathbf {A} \mathbf {x} =\sum _{i,j}a_{ij}x_
      {i}x_{j}]
In other words, it sums up all possible combinations of products of pairs of
elements from x, with a separate coefficient for each. In addition, since
x  i    x  j   =  x  j    x  i     {\displaystyle x_{i}x_{j}=x_{j}x_{i}}  [x_
{i}x_{j}=x_{j}x_{i}], only the sum      a  i j   +  a  j i     {\displaystyle
a_{ij}+a_{ji}}  [a_{ij}+a_{ji}] matters for any off-diagonal elements of A, and
there is no loss of generality in assuming that A is symmetric. Furthermore, if
A is symmetric, then the form       x  &#x2032;   A   y  =   y  &#x2032;   A
x  .   {\displaystyle \mathbf {x} '\mathbf {A} \mathbf {y} =\mathbf {y}
'\mathbf {A} \mathbf {x} .}  [{\displaystyle \mathbf {x} '\mathbf {A} \mathbf
{y} =\mathbf {y} '\mathbf {A} \mathbf {x} .}]
**** Sum of differences from the mean[edit] ****
Another useful formula is as follows:
          &#x2211;  i = 1   n   (  x  i   &#x2212; &#x03BC;  )  2   =  &#x2211;
      i = 1   n   (  x  i   &#x2212;    x &#x00AF;     )  2   + n (    x
      &#x00AF;    &#x2212; &#x03BC;  )  2     {\displaystyle \sum _{i=1}^{n}(x_
      {i}-\mu )^{2}=\sum _{i=1}^{n}(x_{i}-{\bar {x}})^{2}+n({\bar {x}}-\mu )^
      {2}}  [\sum _{i=1}^{n}(x_{i}-\mu )^{2}=\sum _{i=1}^{n}(x_{i}-{\bar {x}})^
      {2}+n({\bar {x}}-\mu )^{2}]
where        x &#x00AF;    =   1 n    &#x2211;  i = 1   n    x  i   .
{\displaystyle {\bar {x}}={\frac {1}{n}}\sum _{i=1}^{n}x_{i}.}  [{\bar {x}}=
{\frac {1}{n}}\sum _{i=1}^{n}x_{i}.]
**** With known variance[edit] ****
For a set of i.i.d. normally distributed data points X of size n where each
individual point x follows     x &#x223C;   N   ( &#x03BC; ,  &#x03C3;  2   )
{\displaystyle x\sim {\mathcal {N}}(\mu ,\sigma ^{2})}  [x\sim {\mathcal {N}}
(\mu ,\sigma ^{2})] with known variance Ï2, the conjugate_prior distribution
is also normally distributed.
This can be shown more easily by rewriting the variance as the precision, i.e.
using Ï = 1/Ï2. Then if     x &#x223C;   N   ( &#x03BC; , 1  /  &#x03C4; )
{\displaystyle x\sim {\mathcal {N}}(\mu ,1/\tau )}  [x\sim {\mathcal {N}}(\mu
,1/\tau )] and     &#x03BC; &#x223C;   N   (  &#x03BC;  0   , 1  /   &#x03C4;
0   ) ,   {\displaystyle \mu \sim {\mathcal {N}}(\mu _{0},1/\tau _{0}),}  [\mu
\sim {\mathcal {N}}(\mu _{0},1/\tau _{0}),] we proceed as follows.
First, the likelihood_function is (using the formula above for the sum of
differences from the mean):
             p (  X  &#x2223; &#x03BC; , &#x03C4; )    =  &#x220F;  i = 1   n
      &#x03C4;  2 &#x03C0;     exp &#x2061;  (  &#x2212;   1 2   &#x03C4; (  x
      i   &#x2212; &#x03BC;  )  2    )        =   (   &#x03C4;  2 &#x03C0;    )
      n  /  2   exp &#x2061;  (  &#x2212;   1 2   &#x03C4;  &#x2211;  i = 1   n
      (  x  i   &#x2212; &#x03BC;  )  2    )        =   (   &#x03C4;  2
      &#x03C0;    )   n  /  2   exp &#x2061;  [  &#x2212;   1 2   &#x03C4;
      (   &#x2211;  i = 1   n   (  x  i   &#x2212;    x &#x00AF;     )  2   + n
      (    x &#x00AF;    &#x2212; &#x03BC;  )  2    )   ]  .
      {\displaystyle {\begin{aligned}p(\mathbf {X} \mid \mu ,\tau )&=\prod _
      {i=1}^{n}{\sqrt {\frac {\tau }{2\pi }}}\exp \left(-{\frac {1}{2}}\tau (x_
      {i}-\mu )^{2}\right)\\&=\left({\frac {\tau }{2\pi }}\right)^{n/2}\exp
      \left(-{\frac {1}{2}}\tau \sum _{i=1}^{n}(x_{i}-\mu )^{2}\right)\\&=\left
      ({\frac {\tau }{2\pi }}\right)^{n/2}\exp \left[-{\frac {1}{2}}\tau \left
      (\sum _{i=1}^{n}(x_{i}-{\bar {x}})^{2}+n({\bar {x}}-\mu )^
      {2}\right)\right].\end{aligned}}}  [{\displaystyle {\begin{aligned}p
      (\mathbf {X} \mid \mu ,\tau )&=\prod _{i=1}^{n}{\sqrt {\frac {\tau }{2\pi
      }}}\exp \left(-{\frac {1}{2}}\tau (x_{i}-\mu )^{2}\right)\\&=\left({\frac
      {\tau }{2\pi }}\right)^{n/2}\exp \left(-{\frac {1}{2}}\tau \sum _{i=1}^
      {n}(x_{i}-\mu )^{2}\right)\\&=\left({\frac {\tau }{2\pi }}\right)^{n/
      2}\exp \left[-{\frac {1}{2}}\tau \left(\sum _{i=1}^{n}(x_{i}-{\bar {x}})^
      {2}+n({\bar {x}}-\mu )^{2}\right)\right].\end{aligned}}}]
Then, we proceed as follows:
             p ( &#x03BC; &#x2223;  X  )    &#x221D; p (  X  &#x2223; &#x03BC;
      ) p ( &#x03BC; )       =   (   &#x03C4;  2 &#x03C0;    )   n  /  2   exp
      &#x2061;  [  &#x2212;   1 2   &#x03C4;  (   &#x2211;  i = 1   n   (  x  i
      &#x2212;    x &#x00AF;     )  2   + n (    x &#x00AF;    &#x2212;
      &#x03BC;  )  2    )   ]      &#x03C4;  0    2 &#x03C0;     exp &#x2061;
      (  &#x2212;   1 2    &#x03C4;  0   ( &#x03BC; &#x2212;  &#x03BC;  0    )
      2    )        &#x221D; exp &#x2061;  (  &#x2212;   1 2    (  &#x03C4;
      (   &#x2211;  i = 1   n   (  x  i   &#x2212;    x &#x00AF;     )  2   + n
      (    x &#x00AF;    &#x2212; &#x03BC;  )  2    )  +  &#x03C4;  0
      ( &#x03BC; &#x2212;  &#x03BC;  0    )  2    )   )        &#x221D; exp
      &#x2061;  (  &#x2212;   1 2    (  n &#x03C4; (    x &#x00AF;    &#x2212;
      &#x03BC;  )  2   +  &#x03C4;  0   ( &#x03BC; &#x2212;  &#x03BC;  0    )
      2    )   )        = exp &#x2061;  (  &#x2212;   1 2   ( n &#x03C4; +
      &#x03C4;  0   )   (  &#x03BC; &#x2212;     n &#x03C4;    x &#x00AF;    +
      &#x03C4;  0    &#x03BC;  0     n &#x03C4; +  &#x03C4;  0        )   2   +
      n &#x03C4;  &#x03C4;  0     n &#x03C4; +  &#x03C4;  0      (    x
      &#x00AF;    &#x2212;  &#x03BC;  0    )  2    )        &#x221D; exp
      &#x2061;  (  &#x2212;   1 2   ( n &#x03C4; +  &#x03C4;  0   )
      (  &#x03BC; &#x2212;     n &#x03C4;    x &#x00AF;    +  &#x03C4;  0
      &#x03BC;  0     n &#x03C4; +  &#x03C4;  0        )   2    )
      {\displaystyle {\begin{aligned}p(\mu \mid \mathbf {X} )&\propto p(\mathbf
      {X} \mid \mu )p(\mu )\\&=\left({\frac {\tau }{2\pi }}\right)^{n/2}\exp
      \left[-{\frac {1}{2}}\tau \left(\sum _{i=1}^{n}(x_{i}-{\bar {x}})^{2}+n(
      {\bar {x}}-\mu )^{2}\right)\right]{\sqrt {\frac {\tau _{0}}{2\pi }}}\exp
      \left(-{\frac {1}{2}}\tau _{0}(\mu -\mu _{0})^{2}\right)\\&\propto \exp
      \left(-{\frac {1}{2}}\left(\tau \left(\sum _{i=1}^{n}(x_{i}-{\bar {x}})^
      {2}+n({\bar {x}}-\mu )^{2}\right)+\tau _{0}(\mu -\mu _{0})^
      {2}\right)\right)\\&\propto \exp \left(-{\frac {1}{2}}\left(n\tau ({\bar
      {x}}-\mu )^{2}+\tau _{0}(\mu -\mu _{0})^{2}\right)\right)\\&=\exp \left(-
      {\frac {1}{2}}(n\tau +\tau _{0})\left(\mu -{\dfrac {n\tau {\bar {x}}+\tau
      _{0}\mu _{0}}{n\tau +\tau _{0}}}\right)^{2}+{\frac {n\tau \tau _{0}}
      {n\tau +\tau _{0}}}({\bar {x}}-\mu _{0})^{2}\right)\\&\propto \exp \left
      (-{\frac {1}{2}}(n\tau +\tau _{0})\left(\mu -{\dfrac {n\tau {\bar
      {x}}+\tau _{0}\mu _{0}}{n\tau +\tau _{0}}}\right)^{2}\right)\end
      {aligned}}}  [{\displaystyle {\begin{aligned}p(\mu \mid \mathbf {X}
      )&\propto p(\mathbf {X} \mid \mu )p(\mu )\\&=\left({\frac {\tau }{2\pi
      }}\right)^{n/2}\exp \left[-{\frac {1}{2}}\tau \left(\sum _{i=1}^{n}(x_
      {i}-{\bar {x}})^{2}+n({\bar {x}}-\mu )^{2}\right)\right]{\sqrt {\frac
      {\tau _{0}}{2\pi }}}\exp \left(-{\frac {1}{2}}\tau _{0}(\mu -\mu _{0})^
      {2}\right)\\&\propto \exp \left(-{\frac {1}{2}}\left(\tau \left(\sum _
      {i=1}^{n}(x_{i}-{\bar {x}})^{2}+n({\bar {x}}-\mu )^{2}\right)+\tau _{0}
      (\mu -\mu _{0})^{2}\right)\right)\\&\propto \exp \left(-{\frac {1}
      {2}}\left(n\tau ({\bar {x}}-\mu )^{2}+\tau _{0}(\mu -\mu _{0})^
      {2}\right)\right)\\&=\exp \left(-{\frac {1}{2}}(n\tau +\tau _{0})\left
      (\mu -{\dfrac {n\tau {\bar {x}}+\tau _{0}\mu _{0}}{n\tau +\tau _
      {0}}}\right)^{2}+{\frac {n\tau \tau _{0}}{n\tau +\tau _{0}}}({\bar {x}}-
      \mu _{0})^{2}\right)\\&\propto \exp \left(-{\frac {1}{2}}(n\tau +\tau _
      {0})\left(\mu -{\dfrac {n\tau {\bar {x}}+\tau _{0}\mu _{0}}{n\tau +\tau _
      {0}}}\right)^{2}\right)\end{aligned}}}]
In the above derivation, we used the formula above for the sum of two
quadratics and eliminated all constant factors not involving Î¼. The result is
the kernel of a normal distribution, with mean        n &#x03C4;    x &#x00AF;
+  &#x03C4;  0    &#x03BC;  0     n &#x03C4; +  &#x03C4;  0
{\displaystyle {\frac {n\tau {\bar {x}}+\tau _{0}\mu _{0}}{n\tau +\tau _{0}}}}
[{\frac {n\tau {\bar {x}}+\tau _{0}\mu _{0}}{n\tau +\tau _{0}}}] and precision
n &#x03C4; +  &#x03C4;  0     {\displaystyle n\tau +\tau _{0}}  [n\tau +\tau _
{0}], i.e.
         p ( &#x03BC; &#x2223;  X  ) &#x223C;   N    (     n &#x03C4;    x
      &#x00AF;    +  &#x03C4;  0    &#x03BC;  0     n &#x03C4; +  &#x03C4;  0
      ,   1  n &#x03C4; +  &#x03C4;  0       )    {\displaystyle p(\mu \mid
      \mathbf {X} )\sim {\mathcal {N}}\left({\frac {n\tau {\bar {x}}+\tau _
      {0}\mu _{0}}{n\tau +\tau _{0}}},{\frac {1}{n\tau +\tau _{0}}}\right)}  [p
      (\mu \mid \mathbf {X} )\sim {\mathcal {N}}\left({\frac {n\tau {\bar
      {x}}+\tau _{0}\mu _{0}}{n\tau +\tau _{0}}},{\frac {1}{n\tau +\tau _
      {0}}}\right)]
This can be written as a set of Bayesian update equations for the posterior
parameters in terms of the prior parameters:
              &#x03C4;  0  &#x2032;     =  &#x03C4;  0   + n &#x03C4;
      &#x03BC;  0  &#x2032;     =    n &#x03C4;    x &#x00AF;    +  &#x03C4;  0
      &#x03BC;  0     n &#x03C4; +  &#x03C4;  0             x &#x00AF;       =
      1 n    &#x2211;  i = 1   n    x  i         {\displaystyle {\begin
      {aligned}\tau _{0}'&=\tau _{0}+n\tau \\\mu _{0}'&={\frac {n\tau {\bar
      {x}}+\tau _{0}\mu _{0}}{n\tau +\tau _{0}}}\\{\bar {x}}&={\frac {1}
      {n}}\sum _{i=1}^{n}x_{i}\end{aligned}}}  [{\begin{aligned}\tau _
      {0}'&=\tau _{0}+n\tau \\\mu _{0}'&={\frac {n\tau {\bar {x}}+\tau _{0}\mu
      _{0}}{n\tau +\tau _{0}}}\\{\bar {x}}&={\frac {1}{n}}\sum _{i=1}^{n}x_
      {i}\end{aligned}}]
That is, to combine n data points with total precision of nÏ (or equivalently,
total variance of n/Ï2) and mean of values        x &#x00AF;
{\displaystyle {\bar {x}}}  [{\bar {x}}], derive a new total precision simply
by adding the total precision of the data to the prior total precision, and
form a new mean through a precision-weighted average, i.e. a weighted_average
of the data mean and the prior mean, each weighted by the associated total
precision. This makes logical sense if the precision is thought of as
indicating the certainty of the observations: In the distribution of the
posterior mean, each of the input components is weighted by its certainty, and
the certainty of this distribution is the sum of the individual certainties.
(For the intuition of this, compare the expression "the whole is (or is not)
greater than the sum of its parts". In addition, consider that the knowledge of
the posterior comes from a combination of the knowledge of the prior and
likelihood, so it makes sense that we are more certain of it than of either of
its components.)
The above formula reveals why it is more convenient to do Bayesian_analysis of
conjugate_priors for the normal distribution in terms of the precision. The
posterior precision is simply the sum of the prior and likelihood precisions,
and the posterior mean is computed through a precision-weighted average, as
described above. The same formulas can be written in terms of variance by
reciprocating all the precisions, yielding the more ugly formulas
                &#x03C3;  0   2    &#x2032;     =   1    n  &#x03C3;  2     +
      1  &#x03C3;  0   2             &#x03BC;  0  &#x2032;     =       n    x
      &#x00AF;      &#x03C3;  2     +    &#x03BC;  0    &#x03C3;  0   2
      n  &#x03C3;  2     +   1  &#x03C3;  0   2               x &#x00AF;
      =   1 n    &#x2211;  i = 1   n    x  i         {\displaystyle {\begin
      {aligned}{\sigma _{0}^{2}}'&={\frac {1}{{\frac {n}{\sigma ^{2}}}+{\frac
      {1}{\sigma _{0}^{2}}}}}\\\mu _{0}'&={\frac {{\frac {n{\bar {x}}}{\sigma ^
      {2}}}+{\frac {\mu _{0}}{\sigma _{0}^{2}}}}{{\frac {n}{\sigma ^{2}}}+
      {\frac {1}{\sigma _{0}^{2}}}}}\\{\bar {x}}&={\frac {1}{n}}\sum _{i=1}^
      {n}x_{i}\end{aligned}}}  [{\begin{aligned}{\sigma _{0}^{2}}'&={\frac {1}{
      {\frac {n}{\sigma ^{2}}}+{\frac {1}{\sigma _{0}^{2}}}}}\\\mu _{0}'&=
      {\frac {{\frac {n{\bar {x}}}{\sigma ^{2}}}+{\frac {\mu _{0}}{\sigma _{0}^
      {2}}}}{{\frac {n}{\sigma ^{2}}}+{\frac {1}{\sigma _{0}^{2}}}}}\\{\bar
      {x}}&={\frac {1}{n}}\sum _{i=1}^{n}x_{i}\end{aligned}}]
**** With known mean[edit] ****
For a set of i.i.d. normally distributed data points X of size n where each
individual point x follows     x &#x223C;   N   ( &#x03BC; ,  &#x03C3;  2   )
{\displaystyle x\sim {\mathcal {N}}(\mu ,\sigma ^{2})}  [x\sim {\mathcal {N}}
(\mu ,\sigma ^{2})] with known mean Î¼, the conjugate_prior of the variance has
an inverse_gamma_distribution or a scaled_inverse_chi-squared_distribution. The
two are equivalent except for having different parameterizations. Although the
inverse gamma is more commonly used, we use the scaled inverse chi-squared for
the sake of convenience. The prior for Ï2 is as follows:
         p (  &#x03C3;  2   &#x2223;  &#x03BD;  0   ,  &#x03C3;  0   2   ) =
      (  &#x03C3;  0   2      &#x03BD;  0   2    )   &#x03BD;  0    /  2
      &#x0393;  (    &#x03BD;  0   2   )     &#xA0;    exp &#x2061;
      [    &#x2212;  &#x03BD;  0    &#x03C3;  0   2     2  &#x03C3;  2      ]
      (  &#x03C3;  2    )  1 +    &#x03BD;  0   2        &#x221D;    exp
      &#x2061;  [    &#x2212;  &#x03BD;  0    &#x03C3;  0   2     2  &#x03C3;
      2      ]    (  &#x03C3;  2    )  1 +    &#x03BD;  0   2
      {\displaystyle p(\sigma ^{2}\mid \nu _{0},\sigma _{0}^{2})={\frac {
      (\sigma _{0}^{2}{\frac {\nu _{0}}{2}})^{\nu _{0}/2}}{\Gamma \left({\frac
      {\nu _{0}}{2}}\right)}}~{\frac {\exp \left[{\frac {-\nu _{0}\sigma _{0}^
      {2}}{2\sigma ^{2}}}\right]}{(\sigma ^{2})^{1+{\frac {\nu _{0}}
      {2}}}}}\propto {\frac {\exp \left[{\frac {-\nu _{0}\sigma _{0}^{2}}
      {2\sigma ^{2}}}\right]}{(\sigma ^{2})^{1+{\frac {\nu _{0}}{2}}}}}}  [
      {\displaystyle p(\sigma ^{2}\mid \nu _{0},\sigma _{0}^{2})={\frac {
      (\sigma _{0}^{2}{\frac {\nu _{0}}{2}})^{\nu _{0}/2}}{\Gamma \left({\frac
      {\nu _{0}}{2}}\right)}}~{\frac {\exp \left[{\frac {-\nu _{0}\sigma _{0}^
      {2}}{2\sigma ^{2}}}\right]}{(\sigma ^{2})^{1+{\frac {\nu _{0}}
      {2}}}}}\propto {\frac {\exp \left[{\frac {-\nu _{0}\sigma _{0}^{2}}
      {2\sigma ^{2}}}\right]}{(\sigma ^{2})^{1+{\frac {\nu _{0}}{2}}}}}}]
The likelihood_function from above, written in terms of the variance, is:
             p (  X  &#x2223; &#x03BC; ,  &#x03C3;  2   )    =   (   1  2
      &#x03C0;  &#x03C3;  2      )   n  /  2   exp &#x2061;  [  &#x2212;   1  2
      &#x03C3;  2       &#x2211;  i = 1   n   (  x  i   &#x2212; &#x03BC;  )  2
      ]        =   (   1  2 &#x03C0;  &#x03C3;  2      )   n  /  2   exp
      &#x2061;  [  &#x2212;   S  2  &#x03C3;  2       ]        {\displaystyle
      {\begin{aligned}p(\mathbf {X} \mid \mu ,\sigma ^{2})&=\left({\frac {1}
      {2\pi \sigma ^{2}}}\right)^{n/2}\exp \left[-{\frac {1}{2\sigma ^{2}}}\sum
      _{i=1}^{n}(x_{i}-\mu )^{2}\right]\\&=\left({\frac {1}{2\pi \sigma ^
      {2}}}\right)^{n/2}\exp \left[-{\frac {S}{2\sigma ^{2}}}\right]\end
      {aligned}}}  [{\displaystyle {\begin{aligned}p(\mathbf {X} \mid \mu
      ,\sigma ^{2})&=\left({\frac {1}{2\pi \sigma ^{2}}}\right)^{n/2}\exp \left
      [-{\frac {1}{2\sigma ^{2}}}\sum _{i=1}^{n}(x_{i}-\mu )^
      {2}\right]\\&=\left({\frac {1}{2\pi \sigma ^{2}}}\right)^{n/2}\exp \left
      [-{\frac {S}{2\sigma ^{2}}}\right]\end{aligned}}}]
where
         S =  &#x2211;  i = 1   n   (  x  i   &#x2212; &#x03BC;  )  2   .
      {\displaystyle S=\sum _{i=1}^{n}(x_{i}-\mu )^{2}.}  [S=\sum _{i=1}^{n}(x_
      {i}-\mu )^{2}.]
Then:
             p (  &#x03C3;  2   &#x2223;  X  )    &#x221D; p (  X  &#x2223;
      &#x03C3;  2   ) p (  &#x03C3;  2   )       =   (   1  2 &#x03C0;
      &#x03C3;  2      )   n  /  2   exp &#x2061;  [  &#x2212;   S  2  &#x03C3;
      2       ]     (  &#x03C3;  0   2      &#x03BD;  0   2    )    &#x03BD;  0
      2      &#x0393;  (    &#x03BD;  0   2   )     &#xA0;    exp &#x2061;
      [    &#x2212;  &#x03BD;  0    &#x03C3;  0   2     2  &#x03C3;  2      ]
      (  &#x03C3;  2    )  1 +    &#x03BD;  0   2              &#x221D;   (   1
      &#x03C3;  2     )   n  /  2     1  (  &#x03C3;  2    )  1 +    &#x03BD;
      0   2        exp &#x2061;  [  &#x2212;   S  2  &#x03C3;  2      +
      &#x2212;  &#x03BD;  0    &#x03C3;  0   2     2  &#x03C3;  2       ]
      =   1  (  &#x03C3;  2    )  1 +     &#x03BD;  0   + n  2        exp
      &#x2061;  [  &#x2212;     &#x03BD;  0    &#x03C3;  0   2   + S   2
      &#x03C3;  2       ]        {\displaystyle {\begin{aligned}p(\sigma ^
      {2}\mid \mathbf {X} )&\propto p(\mathbf {X} \mid \sigma ^{2})p(\sigma ^
      {2})\\&=\left({\frac {1}{2\pi \sigma ^{2}}}\right)^{n/2}\exp \left[-
      {\frac {S}{2\sigma ^{2}}}\right]{\frac {(\sigma _{0}^{2}{\frac {\nu _{0}}
      {2}})^{\frac {\nu _{0}}{2}}}{\Gamma \left({\frac {\nu _{0}}{2}}\right)}}~
      {\frac {\exp \left[{\frac {-\nu _{0}\sigma _{0}^{2}}{2\sigma ^
      {2}}}\right]}{(\sigma ^{2})^{1+{\frac {\nu _{0}}{2}}}}}\\&\propto \left(
      {\frac {1}{\sigma ^{2}}}\right)^{n/2}{\frac {1}{(\sigma ^{2})^{1+{\frac
      {\nu _{0}}{2}}}}}\exp \left[-{\frac {S}{2\sigma ^{2}}}+{\frac {-\nu _
      {0}\sigma _{0}^{2}}{2\sigma ^{2}}}\right]\\&={\frac {1}{(\sigma ^{2})^{1+
      {\frac {\nu _{0}+n}{2}}}}}\exp \left[-{\frac {\nu _{0}\sigma _{0}^{2}+S}
      {2\sigma ^{2}}}\right]\end{aligned}}}  [{\displaystyle {\begin{aligned}p
      (\sigma ^{2}\mid \mathbf {X} )&\propto p(\mathbf {X} \mid \sigma ^{2})p
      (\sigma ^{2})\\&=\left({\frac {1}{2\pi \sigma ^{2}}}\right)^{n/2}\exp
      \left[-{\frac {S}{2\sigma ^{2}}}\right]{\frac {(\sigma _{0}^{2}{\frac
      {\nu _{0}}{2}})^{\frac {\nu _{0}}{2}}}{\Gamma \left({\frac {\nu _{0}}
      {2}}\right)}}~{\frac {\exp \left[{\frac {-\nu _{0}\sigma _{0}^{2}}
      {2\sigma ^{2}}}\right]}{(\sigma ^{2})^{1+{\frac {\nu _{0}}
      {2}}}}}\\&\propto \left({\frac {1}{\sigma ^{2}}}\right)^{n/2}{\frac {1}{
      (\sigma ^{2})^{1+{\frac {\nu _{0}}{2}}}}}\exp \left[-{\frac {S}{2\sigma ^
      {2}}}+{\frac {-\nu _{0}\sigma _{0}^{2}}{2\sigma ^{2}}}\right]\\&={\frac
      {1}{(\sigma ^{2})^{1+{\frac {\nu _{0}+n}{2}}}}}\exp \left[-{\frac {\nu _
      {0}\sigma _{0}^{2}+S}{2\sigma ^{2}}}\right]\end{aligned}}}]
The above is also a scaled inverse chi-squared distribution where
              &#x03BD;  0  &#x2032;     =  &#x03BD;  0   + n      &#x03BD;  0
      &#x2032;     &#x03C3;  0   2    &#x2032;     =  &#x03BD;  0    &#x03C3;
      0   2   +  &#x2211;  i = 1   n   (  x  i   &#x2212; &#x03BC;  )  2
      {\displaystyle {\begin{aligned}\nu _{0}'&=\nu _{0}+n\\\nu _{0}'{\sigma _
      {0}^{2}}'&=\nu _{0}\sigma _{0}^{2}+\sum _{i=1}^{n}(x_{i}-\mu )^{2}\end
      {aligned}}}  [{\begin{aligned}\nu _{0}'&=\nu _{0}+n\\\nu _{0}'{\sigma _
      {0}^{2}}'&=\nu _{0}\sigma _{0}^{2}+\sum _{i=1}^{n}(x_{i}-\mu )^{2}\end
      {aligned}}]
or equivalently
              &#x03BD;  0  &#x2032;     =  &#x03BD;  0   + n        &#x03C3;  0
      2    &#x2032;     =     &#x03BD;  0    &#x03C3;  0   2   +  &#x2211;  i =
      1   n   (  x  i   &#x2212; &#x03BC;  )  2      &#x03BD;  0   + n
      {\displaystyle {\begin{aligned}\nu _{0}'&=\nu _{0}+n\\{\sigma _{0}^
      {2}}'&={\frac {\nu _{0}\sigma _{0}^{2}+\sum _{i=1}^{n}(x_{i}-\mu )^{2}}
      {\nu _{0}+n}}\end{aligned}}}  [{\begin{aligned}\nu _{0}'&=\nu _{0}+n\\
      {\sigma _{0}^{2}}'&={\frac {\nu _{0}\sigma _{0}^{2}+\sum _{i=1}^{n}(x_
      {i}-\mu )^{2}}{\nu _{0}+n}}\end{aligned}}]
Reparameterizing in terms of an inverse_gamma_distribution, the result is:
              &#x03B1; &#x2032;     = &#x03B1; +   n 2        &#x03B2; &#x2032;
      = &#x03B2; +     &#x2211;  i = 1   n   (  x  i   &#x2212; &#x03BC;  )  2
      2         {\displaystyle {\begin{aligned}\alpha '&=\alpha +{\frac {n}
      {2}}\\\beta '&=\beta +{\frac {\sum _{i=1}^{n}(x_{i}-\mu )^{2}}{2}}\end
      {aligned}}}  [{\begin{aligned}\alpha '&=\alpha +{\frac {n}{2}}\\\beta
      '&=\beta +{\frac {\sum _{i=1}^{n}(x_{i}-\mu )^{2}}{2}}\end{aligned}}]
**** With unknown mean and unknown variance[edit] ****
For a set of i.i.d. normally distributed data points X of size n where each
individual point x follows     x &#x223C;   N   ( &#x03BC; ,  &#x03C3;  2   )
{\displaystyle x\sim {\mathcal {N}}(\mu ,\sigma ^{2})}  [x\sim {\mathcal {N}}
(\mu ,\sigma ^{2})] with unknown mean Î¼ and unknown variance Ï2, a combined
(multivariate) conjugate_prior is placed over the mean and variance, consisting
of a normal-inverse-gamma_distribution. Logically, this originates as follows:
   1. From the analysis of the case with unknown mean but known variance, we
      see that the update equations involve sufficient_statistics computed from
      the data consisting of the mean of the data points and the total variance
      of the data points, computed in turn from the known variance divided by
      the number of data points.
   2. From the analysis of the case with unknown variance but known mean, we
      see that the update equations involve sufficient statistics over the data
      consisting of the number of data points and sum_of_squared_deviations.
   3. Keep in mind that the posterior update values serve as the prior
      distribution when further data is handled. Thus, we should logically
      think of our priors in terms of the sufficient statistics just described,
      with the same semantics kept in mind as much as possible.
   4. To handle the case where both mean and variance are unknown, we could
      place independent priors over the mean and variance, with fixed estimates
      of the average mean, total variance, number of data points used to
      compute the variance prior, and sum of squared deviations. Note however
      that in reality, the total variance of the mean depends on the unknown
      variance, and the sum of squared deviations that goes into the variance
      prior (appears to) depend on the unknown mean. In practice, the latter
      dependence is relatively unimportant: Shifting the actual mean shifts the
      generated points by an equal amount, and on average the squared
      deviations will remain the same. This is not the case, however, with the
      total variance of the mean: As the unknown variance increases, the total
      variance of the mean will increase proportionately, and we would like to
      capture this dependence.
   5. This suggests that we create a conditional prior of the mean on the
      unknown variance, with a hyperparameter specifying the mean of the
      pseudo-observations associated with the prior, and another parameter
      specifying the number of pseudo-observations. This number serves as a
      scaling parameter on the variance, making it possible to control the
      overall variance of the mean relative to the actual variance parameter.
      The prior for the variance also has two hyperparameters, one specifying
      the sum of squared deviations of the pseudo-observations associated with
      the prior, and another specifying once again the number of pseudo-
      observations. Note that each of the priors has a hyperparameter
      specifying the number of pseudo-observations, and in each case this
      controls the relative variance of that prior. These are given as two
      separate hyperparameters so that the variance (aka the confidence) of the
      two priors can be controlled separately.
   6. This leads immediately to the normal-inverse-gamma_distribution, which is
      the product of the two distributions just defined, with conjugate_priors
      used (an inverse_gamma_distribution over the variance, and a normal
      distribution over the mean, conditional on the variance) and with the
      same four parameters just defined.
The priors are normally defined as follows:
             p ( &#x03BC; &#x2223;  &#x03C3;  2   ;  &#x03BC;  0   ,  n  0   )
      &#x223C;   N   (  &#x03BC;  0   ,  &#x03C3;  2    /   n  0   )     p
      (  &#x03C3;  2   ;  &#x03BD;  0   ,  &#x03C3;  0   2   )    &#x223C; I
      &#x03C7;  2   (  &#x03BD;  0   ,  &#x03C3;  0   2   ) = I G (  &#x03BD;
      0    /  2 ,  &#x03BD;  0    &#x03C3;  0   2    /  2 )
      {\displaystyle {\begin{aligned}p(\mu \mid \sigma ^{2};\mu _{0},n_
      {0})&\sim {\mathcal {N}}(\mu _{0},\sigma ^{2}/n_{0})\\p(\sigma ^{2};\nu _
      {0},\sigma _{0}^{2})&\sim I\chi ^{2}(\nu _{0},\sigma _{0}^{2})=IG(\nu _
      {0}/2,\nu _{0}\sigma _{0}^{2}/2)\end{aligned}}}  [{\begin{aligned}p(\mu
      \mid \sigma ^{2};\mu _{0},n_{0})&\sim {\mathcal {N}}(\mu _{0},\sigma ^
      {2}/n_{0})\\p(\sigma ^{2};\nu _{0},\sigma _{0}^{2})&\sim I\chi ^{2}(\nu _
      {0},\sigma _{0}^{2})=IG(\nu _{0}/2,\nu _{0}\sigma _{0}^{2}/2)\end
      {aligned}}]
The update equations can be derived, and look as follows:
                x &#x00AF;       =   1 n    &#x2211;  i = 1   n    x  i
      &#x03BC;  0  &#x2032;     =     n  0    &#x03BC;  0   + n    x &#x00AF;
      n  0   + n         n  0  &#x2032;     =  n  0   + n      &#x03BD;  0
      &#x2032;     =  &#x03BD;  0   + n      &#x03BD;  0  &#x2032;     &#x03C3;
      0   2    &#x2032;     =  &#x03BD;  0    &#x03C3;  0   2   +  &#x2211;  i
      = 1   n   (  x  i   &#x2212;    x &#x00AF;     )  2   +     n  0   n    n
      0   + n    (  &#x03BC;  0   &#x2212;    x &#x00AF;     )  2
      {\displaystyle {\begin{aligned}{\bar {x}}&={\frac {1}{n}}\sum _{i=1}^
      {n}x_{i}\\\mu _{0}'&={\frac {n_{0}\mu _{0}+n{\bar {x}}}{n_{0}+n}}\\n_
      {0}'&=n_{0}+n\\\nu _{0}'&=\nu _{0}+n\\\nu _{0}'{\sigma _{0}^{2}}'&=\nu _
      {0}\sigma _{0}^{2}+\sum _{i=1}^{n}(x_{i}-{\bar {x}})^{2}+{\frac {n_{0}n}
      {n_{0}+n}}(\mu _{0}-{\bar {x}})^{2}\end{aligned}}}  [{\displaystyle
      {\begin{aligned}{\bar {x}}&={\frac {1}{n}}\sum _{i=1}^{n}x_{i}\\\mu _
      {0}'&={\frac {n_{0}\mu _{0}+n{\bar {x}}}{n_{0}+n}}\\n_{0}'&=n_{0}+n\\\nu
      _{0}'&=\nu _{0}+n\\\nu _{0}'{\sigma _{0}^{2}}'&=\nu _{0}\sigma _{0}^
      {2}+\sum _{i=1}^{n}(x_{i}-{\bar {x}})^{2}+{\frac {n_{0}n}{n_{0}+n}}(\mu _
      {0}-{\bar {x}})^{2}\end{aligned}}}]
The respective numbers of pseudo-observations add the number of actual
observations to them. The new mean hyperparameter is once again a weighted
average, this time weighted by the relative numbers of observations. Finally,
the update for      &#x03BD;  0  &#x2032;     &#x03C3;  0   2    &#x2032;
{\displaystyle \nu _{0}'{\sigma _{0}^{2}}'}  [\nu _{0}'{\sigma _{0}^{2}}'] is
similar to the case with known mean, but in this case the sum of squared
deviations is taken with respect to the observed data mean rather than the true
mean, and as a result a new "interaction term" needs to be added to take care
of the additional error source stemming from the deviation between prior and
data mean.
[Proof]
The prior distributions are
             p ( &#x03BC; &#x2223;  &#x03C3;  2   ;  &#x03BC;  0   ,  n  0   )
      &#x223C;   N   (  &#x03BC;  0   ,  &#x03C3;  2    /   n  0   ) =   1  2
      &#x03C0;    &#x03C3;  2    n  0        exp &#x2061;  (  &#x2212;    n  0
      2  &#x03C3;  2      ( &#x03BC; &#x2212;  &#x03BC;  0    )  2    )
      &#x221D; (  &#x03C3;  2    )  &#x2212; 1  /  2   exp &#x2061;
      (  &#x2212;    n  0    2  &#x03C3;  2      ( &#x03BC; &#x2212;  &#x03BC;
      0    )  2    )      p (  &#x03C3;  2   ;  &#x03BD;  0   ,  &#x03C3;  0
      2   )    &#x223C; I  &#x03C7;  2   (  &#x03BD;  0   ,  &#x03C3;  0   2
      ) = I G (  &#x03BD;  0    /  2 ,  &#x03BD;  0    &#x03C3;  0   2    /  2
      )       =    (  &#x03C3;  0   2    &#x03BD;  0    /  2  )   &#x03BD;  0
      /  2     &#x0393; (  &#x03BD;  0    /  2 )    &#xA0;    exp &#x2061;
      [    &#x2212;  &#x03BD;  0    &#x03C3;  0   2     2  &#x03C3;  2      ]
      (  &#x03C3;  2    )  1 +  &#x03BD;  0    /  2            &#x221D;
      (  &#x03C3;  2    )  &#x2212; ( 1 +  &#x03BD;  0    /  2 )    exp
      &#x2061;  [    &#x2212;  &#x03BD;  0    &#x03C3;  0   2     2  &#x03C3;
      2      ]  .       {\displaystyle {\begin{aligned}p(\mu \mid \sigma ^
      {2};\mu _{0},n_{0})&\sim {\mathcal {N}}(\mu _{0},\sigma ^{2}/n_{0})=
      {\frac {1}{\sqrt {2\pi {\frac {\sigma ^{2}}{n_{0}}}}}}\exp \left(-{\frac
      {n_{0}}{2\sigma ^{2}}}(\mu -\mu _{0})^{2}\right)\\&\propto (\sigma ^{2})^
      {-1/2}\exp \left(-{\frac {n_{0}}{2\sigma ^{2}}}(\mu -\mu _{0})^
      {2}\right)\\p(\sigma ^{2};\nu _{0},\sigma _{0}^{2})&\sim I\chi ^{2}(\nu _
      {0},\sigma _{0}^{2})=IG(\nu _{0}/2,\nu _{0}\sigma _{0}^{2}/2)\\&={\frac {
      (\sigma _{0}^{2}\nu _{0}/2)^{\nu _{0}/2}}{\Gamma (\nu _{0}/2)}}~{\frac
      {\exp \left[{\frac {-\nu _{0}\sigma _{0}^{2}}{2\sigma ^{2}}}\right]}{
      (\sigma ^{2})^{1+\nu _{0}/2}}}\\&\propto {(\sigma ^{2})^{-(1+\nu _{0}/
      2)}}\exp \left[{\frac {-\nu _{0}\sigma _{0}^{2}}{2\sigma ^
      {2}}}\right].\end{aligned}}}  [{\displaystyle {\begin{aligned}p(\mu \mid
      \sigma ^{2};\mu _{0},n_{0})&\sim {\mathcal {N}}(\mu _{0},\sigma ^{2}/n_
      {0})={\frac {1}{\sqrt {2\pi {\frac {\sigma ^{2}}{n_{0}}}}}}\exp \left(-
      {\frac {n_{0}}{2\sigma ^{2}}}(\mu -\mu _{0})^{2}\right)\\&\propto (\sigma
      ^{2})^{-1/2}\exp \left(-{\frac {n_{0}}{2\sigma ^{2}}}(\mu -\mu _{0})^
      {2}\right)\\p(\sigma ^{2};\nu _{0},\sigma _{0}^{2})&\sim I\chi ^{2}(\nu _
      {0},\sigma _{0}^{2})=IG(\nu _{0}/2,\nu _{0}\sigma _{0}^{2}/2)\\&={\frac {
      (\sigma _{0}^{2}\nu _{0}/2)^{\nu _{0}/2}}{\Gamma (\nu _{0}/2)}}~{\frac
      {\exp \left[{\frac {-\nu _{0}\sigma _{0}^{2}}{2\sigma ^{2}}}\right]}{
      (\sigma ^{2})^{1+\nu _{0}/2}}}\\&\propto {(\sigma ^{2})^{-(1+\nu _{0}/
      2)}}\exp \left[{\frac {-\nu _{0}\sigma _{0}^{2}}{2\sigma ^
      {2}}}\right].\end{aligned}}}]
Therefore, the joint prior is
             p ( &#x03BC; ,  &#x03C3;  2   ;  &#x03BC;  0   ,  n  0   ,
      &#x03BD;  0   ,  &#x03C3;  0   2   )    = p ( &#x03BC; &#x2223;  &#x03C3;
      2   ;  &#x03BC;  0   ,  n  0   )  p (  &#x03C3;  2   ;  &#x03BD;  0   ,
      &#x03C3;  0   2   )       &#x221D; (  &#x03C3;  2    )  &#x2212;
      (  &#x03BD;  0   + 3 )  /  2   exp &#x2061;  [  &#x2212;   1  2  &#x03C3;
      2       (   &#x03BD;  0    &#x03C3;  0   2   +  n  0   ( &#x03BC;
      &#x2212;  &#x03BC;  0    )  2    )   ]  .       {\displaystyle {\begin
      {aligned}p(\mu ,\sigma ^{2};\mu _{0},n_{0},\nu _{0},\sigma _{0}^{2})&=p
      (\mu \mid \sigma ^{2};\mu _{0},n_{0})\,p(\sigma ^{2};\nu _{0},\sigma _
      {0}^{2})\\&\propto (\sigma ^{2})^{-(\nu _{0}+3)/2}\exp \left[-{\frac {1}
      {2\sigma ^{2}}}\left(\nu _{0}\sigma _{0}^{2}+n_{0}(\mu -\mu _{0})^
      {2}\right)\right].\end{aligned}}}  [{\displaystyle {\begin{aligned}p(\mu
      ,\sigma ^{2};\mu _{0},n_{0},\nu _{0},\sigma _{0}^{2})&=p(\mu \mid \sigma
      ^{2};\mu _{0},n_{0})\,p(\sigma ^{2};\nu _{0},\sigma _{0}^{2})\\&\propto
      (\sigma ^{2})^{-(\nu _{0}+3)/2}\exp \left[-{\frac {1}{2\sigma ^{2}}}\left
      (\nu _{0}\sigma _{0}^{2}+n_{0}(\mu -\mu _{0})^{2}\right)\right].\end
      {aligned}}}]
The likelihood_function from the section above with known variance is:
             p (  X  &#x2223; &#x03BC; ,  &#x03C3;  2   )    =   (   1  2
      &#x03C0;  &#x03C3;  2      )   n  /  2   exp &#x2061;  [  &#x2212;   1  2
      &#x03C3;  2       (   &#x2211;  i = 1   n   (  x  i   &#x2212; &#x03BC;
      )  2    )   ]        {\displaystyle {\begin{aligned}p(\mathbf {X} \mid
      \mu ,\sigma ^{2})&=\left({\frac {1}{2\pi \sigma ^{2}}}\right)^{n/2}\exp
      \left[-{\frac {1}{2\sigma ^{2}}}\left(\sum _{i=1}^{n}(x_{i}-\mu )^
      {2}\right)\right]\end{aligned}}}  [{\begin{aligned}p(\mathbf {X} \mid \mu
      ,\sigma ^{2})&=\left({\frac {1}{2\pi \sigma ^{2}}}\right)^{n/2}\exp \left
      [-{\frac {1}{2\sigma ^{2}}}\left(\sum _{i=1}^{n}(x_{i}-\mu )^
      {2}\right)\right]\end{aligned}}]
Writing it in terms of variance rather than precision, we get:
             p (  X  &#x2223; &#x03BC; ,  &#x03C3;  2   )    =   (   1  2
      &#x03C0;  &#x03C3;  2      )   n  /  2   exp &#x2061;  [  &#x2212;   1  2
      &#x03C3;  2       (   &#x2211;  i = 1   n   (  x  i   &#x2212;    x
      &#x00AF;     )  2   + n (    x &#x00AF;    &#x2212; &#x03BC;  )  2    )
      ]        &#x221D;    &#x03C3;  2     &#x2212; n  /  2   exp &#x2061;
      [  &#x2212;   1  2  &#x03C3;  2       (  S + n (    x &#x00AF;
      &#x2212; &#x03BC;  )  2    )   ]        {\displaystyle {\begin{aligned}p
      (\mathbf {X} \mid \mu ,\sigma ^{2})&=\left({\frac {1}{2\pi \sigma ^
      {2}}}\right)^{n/2}\exp \left[-{\frac {1}{2\sigma ^{2}}}\left(\sum _{i=1}^
      {n}(x_{i}-{\bar {x}})^{2}+n({\bar {x}}-\mu )^{2}\right)\right]\\&\propto
      {\sigma ^{2}}^{-n/2}\exp \left[-{\frac {1}{2\sigma ^{2}}}\left(S+n({\bar
      {x}}-\mu )^{2}\right)\right]\end{aligned}}}  [{\begin{aligned}p(\mathbf
      {X} \mid \mu ,\sigma ^{2})&=\left({\frac {1}{2\pi \sigma ^{2}}}\right)^
      {n/2}\exp \left[-{\frac {1}{2\sigma ^{2}}}\left(\sum _{i=1}^{n}(x_{i}-
      {\bar {x}})^{2}+n({\bar {x}}-\mu )^{2}\right)\right]\\&\propto {\sigma ^
      {2}}^{-n/2}\exp \left[-{\frac {1}{2\sigma ^{2}}}\left(S+n({\bar {x}}-\mu
      )^{2}\right)\right]\end{aligned}}]
where     S =  &#x2211;  i = 1   n   (  x  i   &#x2212;    x &#x00AF;     )  2
.   {\displaystyle S=\sum _{i=1}^{n}(x_{i}-{\bar {x}})^{2}.}  [S=\sum _{i=1}^
{n}(x_{i}-{\bar {x}})^{2}.]
Therefore, the posterior is (dropping the hyperparameters as conditioning
factors):
             p ( &#x03BC; ,  &#x03C3;  2   &#x2223;  X  )    &#x221D; p
      ( &#x03BC; ,  &#x03C3;  2   )  p (  X  &#x2223; &#x03BC; ,  &#x03C3;  2
      )       &#x221D; (  &#x03C3;  2    )  &#x2212; (  &#x03BD;  0   + 3 )  /
      2   exp &#x2061;  [  &#x2212;   1  2  &#x03C3;  2       (   &#x03BD;  0
      &#x03C3;  0   2   +  n  0   ( &#x03BC; &#x2212;  &#x03BC;  0    )  2    )
      ]     &#x03C3;  2     &#x2212; n  /  2   exp &#x2061;  [  &#x2212;   1  2
      &#x03C3;  2       (  S + n (    x &#x00AF;    &#x2212; &#x03BC;  )  2
      )   ]        = (  &#x03C3;  2    )  &#x2212; (  &#x03BD;  0   + n + 3 )
      /  2   exp &#x2061;  [  &#x2212;   1  2  &#x03C3;  2       (   &#x03BD;
      0    &#x03C3;  0   2   + S +  n  0   ( &#x03BC; &#x2212;  &#x03BC;  0
      )  2   + n (    x &#x00AF;    &#x2212; &#x03BC;  )  2    )   ]        =
      (  &#x03C3;  2    )  &#x2212; (  &#x03BD;  0   + n + 3 )  /  2   exp
      &#x2061;  [  &#x2212;   1  2  &#x03C3;  2       (   &#x03BD;  0
      &#x03C3;  0   2   + S +     n  0   n    n  0   + n    (  &#x03BC;  0
      &#x2212;    x &#x00AF;     )  2   + (  n  0   + n )   (  &#x03BC;
      &#x2212;     n  0    &#x03BC;  0   + n    x &#x00AF;       n  0   + n
      )   2    )   ]        &#x221D; (  &#x03C3;  2    )  &#x2212; 1  /  2
      exp &#x2061;  [  &#x2212;     n  0   + n   2  &#x03C3;  2
      (  &#x03BC; &#x2212;     n  0    &#x03BC;  0   + n    x &#x00AF;       n
      0   + n     )   2    ]         &#x00D7; (  &#x03C3;  2    )  &#x2212;
      (  &#x03BD;  0    /  2 + n  /  2 + 1 )   exp &#x2061;  [  &#x2212;   1  2
      &#x03C3;  2       (   &#x03BD;  0    &#x03C3;  0   2   + S +     n  0   n
      n  0   + n    (  &#x03BC;  0   &#x2212;    x &#x00AF;     )  2    )   ]
      =    N    &#x03BC; &#x2223;  &#x03C3;  2      (      n  0    &#x03BC;  0
      + n    x &#x00AF;       n  0   + n    ,    &#x03C3;  2     n  0   + n
      )  &#x22C5;    I G     &#x03C3;  2      (    1 2   (  &#x03BD;  0   + n )
      ,   1 2    (   &#x03BD;  0    &#x03C3;  0   2   + S +     n  0   n    n
      0   + n    (  &#x03BC;  0   &#x2212;    x &#x00AF;     )  2    )   )  .
      {\displaystyle {\begin{aligned}p(\mu ,\sigma ^{2}\mid \mathbf {X}
      )&\propto p(\mu ,\sigma ^{2})\,p(\mathbf {X} \mid \mu ,\sigma ^
      {2})\\&\propto (\sigma ^{2})^{-(\nu _{0}+3)/2}\exp \left[-{\frac {1}
      {2\sigma ^{2}}}\left(\nu _{0}\sigma _{0}^{2}+n_{0}(\mu -\mu _{0})^
      {2}\right)\right]{\sigma ^{2}}^{-n/2}\exp \left[-{\frac {1}{2\sigma ^
      {2}}}\left(S+n({\bar {x}}-\mu )^{2}\right)\right]\\&=(\sigma ^{2})^{-(\nu
      _{0}+n+3)/2}\exp \left[-{\frac {1}{2\sigma ^{2}}}\left(\nu _{0}\sigma _
      {0}^{2}+S+n_{0}(\mu -\mu _{0})^{2}+n({\bar {x}}-\mu )^
      {2}\right)\right]\\&=(\sigma ^{2})^{-(\nu _{0}+n+3)/2}\exp \left[-{\frac
      {1}{2\sigma ^{2}}}\left(\nu _{0}\sigma _{0}^{2}+S+{\frac {n_{0}n}{n_
      {0}+n}}(\mu _{0}-{\bar {x}})^{2}+(n_{0}+n)\left(\mu -{\frac {n_{0}\mu _
      {0}+n{\bar {x}}}{n_{0}+n}}\right)^{2}\right)\right]\\&\propto (\sigma ^
      {2})^{-1/2}\exp \left[-{\frac {n_{0}+n}{2\sigma ^{2}}}\left(\mu -{\frac
      {n_{0}\mu _{0}+n{\bar {x}}}{n_{0}+n}}\right)^{2}\right]\\&\quad \times
      (\sigma ^{2})^{-(\nu _{0}/2+n/2+1)}\exp \left[-{\frac {1}{2\sigma ^
      {2}}}\left(\nu _{0}\sigma _{0}^{2}+S+{\frac {n_{0}n}{n_{0}+n}}(\mu _{0}-
      {\bar {x}})^{2}\right)\right]\\&={\mathcal {N}}_{\mu \mid \sigma ^
      {2}}\left({\frac {n_{0}\mu _{0}+n{\bar {x}}}{n_{0}+n}},{\frac {\sigma ^
      {2}}{n_{0}+n}}\right)\cdot {\rm {IG}}_{\sigma ^{2}}\left({\frac {1}{2}}
      (\nu _{0}+n),{\frac {1}{2}}\left(\nu _{0}\sigma _{0}^{2}+S+{\frac {n_
      {0}n}{n_{0}+n}}(\mu _{0}-{\bar {x}})^{2}\right)\right).\end{aligned}}}  [
      {\begin{aligned}p(\mu ,\sigma ^{2}\mid \mathbf {X} )&\propto p(\mu
      ,\sigma ^{2})\,p(\mathbf {X} \mid \mu ,\sigma ^{2})\\&\propto (\sigma ^
      {2})^{-(\nu _{0}+3)/2}\exp \left[-{\frac {1}{2\sigma ^{2}}}\left(\nu _
      {0}\sigma _{0}^{2}+n_{0}(\mu -\mu _{0})^{2}\right)\right]{\sigma ^{2}}^{-
      n/2}\exp \left[-{\frac {1}{2\sigma ^{2}}}\left(S+n({\bar {x}}-\mu )^
      {2}\right)\right]\\&=(\sigma ^{2})^{-(\nu _{0}+n+3)/2}\exp \left[-{\frac
      {1}{2\sigma ^{2}}}\left(\nu _{0}\sigma _{0}^{2}+S+n_{0}(\mu -\mu _{0})^
      {2}+n({\bar {x}}-\mu )^{2}\right)\right]\\&=(\sigma ^{2})^{-(\nu _
      {0}+n+3)/2}\exp \left[-{\frac {1}{2\sigma ^{2}}}\left(\nu _{0}\sigma _
      {0}^{2}+S+{\frac {n_{0}n}{n_{0}+n}}(\mu _{0}-{\bar {x}})^{2}+(n_
      {0}+n)\left(\mu -{\frac {n_{0}\mu _{0}+n{\bar {x}}}{n_{0}+n}}\right)^
      {2}\right)\right]\\&\propto (\sigma ^{2})^{-1/2}\exp \left[-{\frac {n_
      {0}+n}{2\sigma ^{2}}}\left(\mu -{\frac {n_{0}\mu _{0}+n{\bar {x}}}{n_
      {0}+n}}\right)^{2}\right]\\&\quad \times (\sigma ^{2})^{-(\nu _{0}/2+n/
      2+1)}\exp \left[-{\frac {1}{2\sigma ^{2}}}\left(\nu _{0}\sigma _{0}^
      {2}+S+{\frac {n_{0}n}{n_{0}+n}}(\mu _{0}-{\bar {x}})^
      {2}\right)\right]\\&={\mathcal {N}}_{\mu \mid \sigma ^{2}}\left({\frac
      {n_{0}\mu _{0}+n{\bar {x}}}{n_{0}+n}},{\frac {\sigma ^{2}}{n_
      {0}+n}}\right)\cdot {\rm {IG}}_{\sigma ^{2}}\left({\frac {1}{2}}(\nu _
      {0}+n),{\frac {1}{2}}\left(\nu _{0}\sigma _{0}^{2}+S+{\frac {n_{0}n}{n_
      {0}+n}}(\mu _{0}-{\bar {x}})^{2}\right)\right).\end{aligned}}]
In other words, the posterior distribution has the form of a product of a
normal distribution over p(Î¼ | Ï2) times an inverse gamma distribution over p
(Ï2), with parameters that are the same as the update equations above.
***** Occurrence and applications[edit] *****
The occurrence of normal distribution in practical problems can be loosely
classified into four categories:
   1. Exactly normal distributions;
   2. Approximately normal laws, for example when such approximation is
      justified by the central_limit_theorem; and
   3. Distributions modeled as normal â the normal distribution being the
      distribution with maximum_entropy for a given mean and variance.
   4. Regression problems â the normal distribution being found after
      systematic effects have been modeled sufficiently well.
**** Exact normality[edit] ****
The ground state of a quantum_harmonic_oscillator has the Gaussian
distribution.
Certain quantities in physics are distributed normally, as was first
demonstrated by James_Clerk_Maxwell. Examples of such quantities are:
    * Probability density function of a ground state in a quantum_harmonic
      oscillator.
    * The position of a particle that experiences diffusion. If initially the
      particle is located at a specific point (that is its probability
      distribution is the dirac_delta_function), then after time t its location
      is described by a normal distribution with variance t, which satisfies
      the diffusion_equation       &#x2202;  &#x2202; t    f ( x , t ) =   1 2
      &#x2202;  2    &#x2202;  x  2      f ( x , t )   {\displaystyle {\frac
      {\partial }{\partial t}}f(x,t)={\frac {1}{2}}{\frac {\partial ^{2}}
      {\partial x^{2}}}f(x,t)}  [{\displaystyle {\frac {\partial }{\partial
      t}}f(x,t)={\frac {1}{2}}{\frac {\partial ^{2}}{\partial x^{2}}}f(x,t)}].
      If the initial location is given by a certain density function     g ( x
      )   {\displaystyle g(x)}  [g(x)], then the density at time t is the
      convolution of g and the normal PDF.
**** Approximate normality[edit] ****
Approximately normal distributions occur in many situations, as explained by
the central_limit_theorem. When the outcome is produced by many small effects
acting additively and independently, its distribution will be close to normal.
The normal approximation will not be valid if the effects act multiplicatively
(instead of additively), or if there is a single external influence that has a
considerably larger magnitude than the rest of the effects.
    * In counting problems, where the central limit theorem includes a
      discrete-to-continuum approximation and where infinitely_divisible and
      decomposable distributions are involved, such as
          o Binomial_random_variables, associated with binary response
            variables;
          o Poisson_random_variables, associated with rare events;
    * Thermal_radiation has a BoseâEinstein distribution on very short time
      scales, and a normal distribution on longer timescales due to the central
      limit theorem.
**** Assumed normality[edit] ****
Histogram of sepal widths for Iris versicolor from Fisher's Iris_flower_data
set, with superimposed best-fitting normal distribution.
     I can only recognize the occurrence of the normal curve â the
     Laplacian curve of errors â as a very abnormal phenomenon. It is
     roughly approximated to in certain distributions; for this reason,
     and on account for its beautiful simplicity, we may, perhaps, use it
     as a first approximation, particularly in theoretical investigations.
     â Pearson_(1901)
There are statistical methods to empirically test that assumption, see the
above Normality_tests section.
    * In biology, the logarithm of various variables tend to have a normal
      distribution, that is, they tend to have a log-normal_distribution (after
      separation on male/female subpopulations), with examples including:
          o Measures of size of living tissue (length, height, skin area,
            weight);[49]
          o The length of inert appendages (hair, claws, nails, teeth) of
            biological specimens, in the direction of growth; presumably the
            thickness of tree bark also falls under this category;
          o Certain physiological measurements, such as blood pressure of adult
            humans.
    * In finance, in particular the BlackâScholes_model, changes in the
      logarithm of exchange rates, price indices, and stock market indices are
      assumed normal (these variables behave like compound_interest, not like
      simple interest, and so are multiplicative). Some mathematicians such as
      Benoit_Mandelbrot have argued that log-Levy_distributions, which
      possesses heavy_tails would be a more appropriate model, in particular
      for the analysis for stock_market_crashes. The use of the assumption of
      normal distribution occurring in financial models has also been
      criticized by Nassim_Nicholas_Taleb in his works.
    * Measurement_errors in physical experiments are often modeled by a normal
      distribution. This use of a normal distribution does not imply that one
      is assuming the measurement errors are normally distributed, rather using
      the normal distribution produces the most conservative predictions
      possible given only knowledge about the mean and variance of the errors.
      [50]
    * In standardized_testing, results can be made to have a normal
      distribution by either selecting the number and difficulty of questions
      (as in the IQ_test) or transforming the raw test scores into "output"
      scores by fitting them to the normal distribution. For example, the SAT's
      traditional range of 200â800 is based on a normal distribution with a
      mean of 500 and a standard deviation of 100.
Fitted cumulative normal distribution to October rainfalls, see distribution
fitting
    * Many scores are derived from the normal distribution, including
      percentile_ranks ("percentiles" or "quantiles"), normal_curve
      equivalents, stanines, z-scores, and T-scores. Additionally, some
      behavioral statistical procedures assume that scores are normally
      distributed; for example, t-tests and ANOVAs. Bell_curve_grading assigns
      relative grades based on a normal distribution of scores.
    * In hydrology the distribution of long duration river discharge or
      rainfall, e.g. monthly and yearly totals, is often thought to be
      practically normal according to the central_limit_theorem.[51] The blue
      picture, made with CumFreq, illustrates an example of fitting the normal
      distribution to ranked October rainfalls showing the 90% confidence_belt
      based on the binomial_distribution. The rainfall data are represented by
      plotting_positions as part of the cumulative_frequency_analysis.
**** Produced normality[edit] ****
In regression_analysis, lack of normality in residuals simply indicates that
the model postulated is inadequate in accounting for the tendency in the data
and needs to be augmented; in other words, normality in residuals can always be
achieved given a properly constructed model.
***** Generating values from normal distribution[edit] *****
The bean_machine, a device invented by Francis_Galton, can be called the first
generator of normal random variables. This machine consists of a vertical board
with interleaved rows of pins. Small balls are dropped from the top and then
bounce randomly left or right as they hit the pins. The balls are collected
into bins at the bottom and settle down into a pattern resembling the Gaussian
curve.
In computer simulations, especially in applications of the Monte-Carlo_method,
it is often desirable to generate values that are normally distributed. The
algorithms listed below all generate the standard normal deviates, since a N
(Î¼, Ï2
) can be generated as X = Î¼ + ÏZ, where Z is standard normal. All these
algorithms rely on the availability of a random_number_generator U capable of
producing uniform random variates.
    * The most straightforward method is based on the probability_integral
      transform property: if U is distributed uniformly on (0,1), then Î¦â1
      (U) will have the standard normal distribution. The drawback of this
      method is that it relies on calculation of the probit_function Î¦â1,
      which cannot be done analytically. Some approximate methods are described
      in Hart_(1968) and in the erf article. Wichura gives a fast algorithm for
      computing this function to 16 decimal places,[52] which is used by R to
      compute random variates of the normal distribution.
    * An easy to program approximate approach, that relies on the central_limit
      theorem, is as follows: generate 12 uniform U(0,1) deviates, add them all
      up, and subtract 6 â the resulting random variable will have
      approximately standard normal distribution. In truth, the distribution
      will be IrwinâHall, which is a 12-section eleventh-order polynomial
      approximation to the normal distribution. This random deviate will have a
      limited range of (â6, 6).[53]
    * The BoxâMuller_method uses two independent random numbers U and V
      distributed uniformly on (0,1). Then the two random variables X and Y
               X =   &#x2212; 2 ln &#x2061; U    cos &#x2061; ( 2 &#x03C0; V )
            ,  Y =   &#x2212; 2 ln &#x2061; U    sin &#x2061; ( 2 &#x03C0; V )
            .   {\displaystyle X={\sqrt {-2\ln U}}\,\cos(2\pi V),\qquad Y=
            {\sqrt {-2\ln U}}\,\sin(2\pi V).}  [X={\sqrt {-2\ln U}}\,\cos(2\pi
            V),\qquad Y={\sqrt {-2\ln U}}\,\sin(2\pi V).]
      will both have the standard normal distribution, and will be independent.
      This formulation arises because for a bivariate_normal random vector (X,
      Y) the squared norm X2 + Y2 will have the chi-squared_distribution with
      two degrees of freedom, which is an easily generated exponential_random
      variable corresponding to the quantity â2ln(U) in these equations; and
      the angle is distributed uniformly around the circle, chosen by the
      random variable V.
    * The Marsaglia_polar_method is a modification of the BoxâMuller method
      which does not require computation of the sine and cosine functions. In
      this method, U and V are drawn from the uniform (â1,1) distribution,
      and then S = U2 + V2 is computed. If S is greater or equal to 1, then the
      method starts over, otherwise the two quantities
               X = U     &#x2212; 2 ln &#x2061; S  S    ,  Y = V     &#x2212; 2
            ln &#x2061; S  S      {\displaystyle X=U{\sqrt {\frac {-2\ln S}
            {S}}},\qquad Y=V{\sqrt {\frac {-2\ln S}{S}}}}  [{\displaystyle X=U
            {\sqrt {\frac {-2\ln S}{S}}},\qquad Y=V{\sqrt {\frac {-2\ln S}
            {S}}}}]
      are returned. Again, X and Y are independent, standard normal random
      variables.
    * The Ratio method[54] is a rejection method. The algorithm proceeds as
      follows:
          o Generate two independent uniform deviates U and V;
          o Compute X = √8/e (V â 0.5)/U;
          o Optional: if X2 â¤ 5 â 4e1/4U then accept X and terminate
            algorithm;
          o Optional: if X2 â¥ 4eâ1.35/U + 1.4 then reject X and start over
            from step 1;
          o If X2 â¤ â4 lnU then accept X, otherwise start over the
            algorithm.
      The two optional steps allow the evaluation of the logarithm in the last
      step to be avoided in most cases. These steps can be greatly improved[55]
      so that the logarithm is rarely evaluated.
    * The ziggurat_algorithm[56] is faster than the BoxâMuller transform and
      still exact. In about 97% of all cases it uses only two random numbers,
      one random integer and one random uniform, one multiplication and an if-
      test. Only in 3% of the cases, where the combination of those two falls
      outside the "core of the ziggurat" (a kind of rejection sampling using
      logarithms), do exponentials and more uniform random numbers have to be
      employed.
    * Integer arithmetic can be used to sample from the standard normal
      distribution.[57] This method is exact in the sense that it satisfies the
      conditions of ideal approximation;[58] i.e., it is equivalent to sampling
      a real number from the standard normal distribution and rounding this to
      the nearest representable floating point number.
    * There is also some investigation[59] into the connection between the fast
      Hadamard_transform and the normal distribution, since the transform
      employs just addition and subtraction and by the central limit theorem
      random numbers from almost any distribution will be transformed into the
      normal distribution. In this regard a series of Hadamard transforms can
      be combined with random permutations to turn arbitrary data sets into a
      normally distributed data.
***** Numerical approximations for the normal CDF[edit] *****
The standard normal CDF is widely used in scientific and statistical computing.
The values Î¦(x) may be approximated very accurately by a variety of methods,
such as numerical_integration, Taylor_series, asymptotic_series and continued
fractions. Different approximations are used depending on the desired level of
accuracy.
    * Zelen_&_Severo_(1964) give the approximation for Î¦(x) for x > 0 with the
      absolute error |Îµ(x)| < 7.5Â·10â8 (algorithm 26.2.17):
               &#x03A6; ( x ) = 1 &#x2212; &#x03C6; ( x )  (   b  1   t +  b  2
            t  2   +  b  3    t  3   +  b  4    t  4   +  b  5    t  5    )  +
            &#x03B5; ( x ) ,  t =   1  1 +  b  0   x    ,   {\displaystyle \Phi
            (x)=1-\varphi (x)\left(b_{1}t+b_{2}t^{2}+b_{3}t^{3}+b_{4}t^{4}+b_
            {5}t^{5}\right)+\varepsilon (x),\qquad t={\frac {1}{1+b_{0}x}},}  [
            {\displaystyle \Phi (x)=1-\varphi (x)\left(b_{1}t+b_{2}t^{2}+b_
            {3}t^{3}+b_{4}t^{4}+b_{5}t^{5}\right)+\varepsilon (x),\qquad t=
            {\frac {1}{1+b_{0}x}},}]
      where Ï(x) is the standard normal PDF, and b0 = 0.2316419, b1 =
      0.319381530, b2 = â0.356563782, b3 = 1.781477937, b4 = â1.821255978,
      b5 = 1.330274429.
    * Hart_(1968) lists some dozens of approximations â by means of rational
      functions, with or without exponentials â for the
erfc() function. His algorithms vary in the degree of complexity and the
resulting precision, with maximum absolute precision of 24 digits. An algorithm
by West_(2009) combines Hart's algorithm 5666 with a continued_fraction
approximation in the tail to provide a fast computation algorithm with a 16-
digit precision.
Cody_(1969) after recalling Hart68 solution is not suited for erf, gives a
solution for both erf and erfc, with maximal relative error bound, via Rational
Chebyshev_Approximation.
Marsaglia_(2004) suggested a simple algorithm[note_2] based on the Taylor
series expansion
         &#x03A6; ( x ) =   1 2   + &#x03C6; ( x )  (  x +    x  3   3   +    x
      5    3 &#x22C5; 5    +    x  7    3 &#x22C5; 5 &#x22C5; 7    +    x  9
      3 &#x22C5; 5 &#x22C5; 7 &#x22C5; 9    + &#x22EF;  )    {\displaystyle
      \Phi (x)={\frac {1}{2}}+\varphi (x)\left(x+{\frac {x^{3}}{3}}+{\frac {x^
      {5}}{3\cdot 5}}+{\frac {x^{7}}{3\cdot 5\cdot 7}}+{\frac {x^{9}}{3\cdot
      5\cdot 7\cdot 9}}+\cdots \right)}  [{\displaystyle \Phi (x)={\frac {1}
      {2}}+\varphi (x)\left(x+{\frac {x^{3}}{3}}+{\frac {x^{5}}{3\cdot 5}}+
      {\frac {x^{7}}{3\cdot 5\cdot 7}}+{\frac {x^{9}}{3\cdot 5\cdot 7\cdot
      9}}+\cdots \right)}]
for calculating Î¦(x) with arbitrary precision. The drawback of this algorithm
is comparatively slow calculation time (for example it takes over 300
iterations to calculate the function with 16 digits of precision when x = 10).
The GNU_Scientific_Library calculates values of the standard normal CDF using
Hart's algorithms and approximations with Chebyshev_polynomials.
Shore (1982) introduced simple approximations that may be incorporated in
stochastic optimization models of engineering and operations research, like
reliability engineering and inventory analysis. Denoting p=Î¦(z), the simplest
approximation for the quantile function is:
         z =  &#x03A6;  &#x2212; 1   ( p ) = 5.5556  [  1 &#x2212;   (    1
      &#x2212; p  p   )   0.1186    ]  ,  p &#x2265; 1  /  2   {\displaystyle
      z=\Phi ^{-1}(p)=5.5556\left[1-\left({\frac {1-p}{p}}\right)^
      {0.1186}\right],\qquad p\geq 1/2}  [{\displaystyle z=\Phi ^{-1}
      (p)=5.5556\left[1-\left({\frac {1-p}{p}}\right)^{0.1186}\right],\qquad
      p\geq 1/2}]
This approximation delivers for z a maximum absolute error of 0.026 (for
0.5 â¤ p â¤ 0.9999, corresponding to 0 â¤ z â¤ 3.719). For p < 1/2 replace
p by 1 â p and change sign. Another approximation, somewhat less accurate, is
the single-parameter approximation:
         z = &#x2212; 0.4115  {     1 &#x2212; p  p   + log &#x2061;  [    1
      &#x2212; p  p   ]  &#x2212; 1  }  ,  p &#x2265; 1  /  2   {\displaystyle
      z=-0.4115\left\{{\frac {1-p}{p}}+\log \left[{\frac {1-p}{p}}\right]-
      1\right\},\qquad p\geq 1/2}  [{\displaystyle z=-0.4115\left\{{\frac {1-p}
      {p}}+\log \left[{\frac {1-p}{p}}\right]-1\right\},\qquad p\geq 1/2}]
The latter had served to derive a simple approximation for the loss integral of
the normal distribution, defined by
             L ( z )    =  &#x222B;  z   &#x221E;   ( u &#x2212; z ) &#x03C6;
      ( u )  d u =  &#x222B;  z   &#x221E;   [ 1 &#x2212; &#x03A6; ( u ) ]  d u
      L ( z )    &#x2248;   {    0.4115  (    p  1 &#x2212; p     )  &#x2212; z
      ,   p < 1  /  2 ,        0.4115  (     1 &#x2212; p  p    )  ,   p
      &#x2265; 1  /  2.            or, equivalently,      L ( z )    &#x2248;
      {    0.4115  {  1 &#x2212; log &#x2061;  [   p  1 &#x2212; p    ]   }  ,
      p < 1  /  2 ,        0.4115     1 &#x2212; p  p    ,   p &#x2265; 1  /
      2.             {\displaystyle {\begin{aligned}L(z)&=\int _{z}^{\infty }
      (u-z)\varphi (u)\,du=\int _{z}^{\infty }[1-\Phi (u)]\,du\\[5pt]L
      (z)&\approx {\begin{cases}0.4115\left({\dfrac {p}{1-p}}\right)-z,&p<1/
      2,\\\\0.4115\left({\dfrac {1-p}{p}}\right),&p\geq 1/2.\end{cases}}\\[5pt]
      {\text{or, equivalently,}}\\L(z)&\approx {\begin{cases}0.4115\left\{1-
      \log \left[{\frac {p}{1-p}}\right]\right\},&p<1/2,\\\\0.4115{\dfrac {1-p}
      {p}},&p\geq 1/2.\end{cases}}\end{aligned}}}  [{\displaystyle {\begin
      {aligned}L(z)&=\int _{z}^{\infty }(u-z)\varphi (u)\,du=\int _{z}^{\infty
      }[1-\Phi (u)]\,du\\[5pt]L(z)&\approx {\begin{cases}0.4115\left({\dfrac
      {p}{1-p}}\right)-z,&p<1/2,\\\\0.4115\left({\dfrac {1-p}{p}}\right),&p\geq
      1/2.\end{cases}}\\[5pt]{\text{or, equivalently,}}\\L(z)&\approx {\begin
      {cases}0.4115\left\{1-\log \left[{\frac {p}{1-p}}\right]\right\},&p<1/
      2,\\\\0.4115{\dfrac {1-p}{p}},&p\geq 1/2.\end{cases}}\end{aligned}}}]
This approximation is particularly accurate for the right far-tail (maximum
error of 10â3 for zâ¥1.4). Highly accurate approximations for the CDF, based
on Response_Modeling_Methodology (RMM, Shore, 2011, 2012), are shown in Shore
(2005).
Some more approximations can be found at: Error_function#Approximation_with
elementary_functions. In particular, small relative error on the whole domain
for the CDF     &#x03A6;   {\displaystyle \Phi }  [\Phi ] and the quantile
function      &#x03A6;  &#x2212; 1     {\displaystyle \Phi ^{-1}}  [\Phi ^{-1}]
as well, is achieved via an explicitly invertible formula by Sergei Winitzki in
2008.
***** History[edit] *****
**** Development[edit] ****
Some authors[60][61] attribute the credit for the discovery of the normal
distribution to de_Moivre, who in 1738[note_3] published in the second edition
of his "The_Doctrine_of_Chances" the study of the coefficients in the binomial
expansion of (a + b)n. De Moivre proved that the middle term in this expansion
has the approximate magnitude of     2  /    2 &#x03C0; n     {\displaystyle 2/
{\sqrt {2\pi n}}}  [2/{\sqrt {2\pi n}}], and that "If m or Â½n be a Quantity
infinitely great, then the Logarithm of the Ratio, which a Term distant from
the middle by the Interval â, has to the middle Term, is     &#x2212;    2
&#x2113; &#x2113;  n     {\displaystyle -{\frac {2\ell \ell }{n}}}  [-{\frac
{2\ell \ell }{n}}]."[62] Although this theorem can be interpreted as the first
obscure expression for the normal probability law, Stigler points out that de
Moivre himself did not interpret his results as anything more than the
approximate rule for the binomial coefficients, and in particular de Moivre
lacked the concept of the probability density function.[63]
Carl_Friedrich_Gauss discovered the normal distribution in 1809 as a way to
rationalize the method_of_least_squares.
In 1809 Gauss published his monograph "Theoria motus corporum coelestium in
sectionibus conicis solem ambientium" where among other things he introduces
several important statistical concepts, such as the method_of_least_squares,
the method_of_maximum_likelihood, and the normal distribution. Gauss used M,
Mâ², Mâ²â², â¦ to denote the measurements of some unknown quantity V, and
sought the "most probable" estimator of that quantity: the one that maximizes
the probability Ï(M â V) Â· Ï(Mâ² â V) Â· Ï(Mâ²â² â V) Â· â¦ of
obtaining the observed experimental results. In his notation ÏÎ is the
probability law of the measurement errors of magnitude Î. Not knowing what the
function Ï is, Gauss requires that his method should reduce to the well-known
answer: the arithmetic mean of the measured values.[note_4] Starting from these
principles, Gauss demonstrates that the only law that rationalizes the choice
of arithmetic mean as an estimator of the location parameter, is the normal law
of errors:[64]
         &#x03C6;   &#x0394;   =   h  &#x221A; &#x03C0;      e  &#x2212;  h h
      &#x0394; &#x0394;   ,   {\displaystyle \varphi {\mathit {\Delta }}={\frac
      {h}{\surd \pi }}\,e^{-\mathrm {hh} \Delta \Delta },}  [{\displaystyle
      \varphi {\mathit {\Delta }}={\frac {h}{\surd \pi }}\,e^{-\mathrm {hh}
      \Delta \Delta },}]
where h is "the measure of the precision of the observations". Using this
normal law as a generic model for errors in the experiments, Gauss formulates
what is now known as the non-linear weighted least squares (NWLS) method.[65]
Marquis_de_Laplace proved the central_limit_theorem in 1810, consolidating the
importance of the normal distribution in statistics.
Although Gauss was the first to suggest the normal distribution law, Laplace
made significant contributions.[note_5] It was Laplace who first posed the
problem of aggregating several observations in 1774,[66] although his own
solution led to the Laplacian_distribution. It was Laplace who first calculated
the value of the integral_â«_eât2 dt_=_√Ï in 1782, providing the
normalization constant for the normal distribution.[67] Finally, it was Laplace
who in 1810 proved and presented to the Academy the fundamental central_limit
theorem, which emphasized the theoretical importance of the normal
distribution.[68]
It is of interest to note that in 1809 an American mathematician Adrain
published two derivations of the normal probability law, simultaneously and
independently from Gauss.[69] His works remained largely unnoticed by the
scientific community, until in 1871 they were "rediscovered" by Abbe.[70]
In the middle of the 19th century Maxwell demonstrated that the normal
distribution is not just a convenient mathematical tool, but may also occur in
natural phenomena:[71] "The number of particles whose velocity, resolved in a
certain direction, lies between x and x + dx is
         N &#x2061;   1  &#x03B1;    &#x03C0;        e  &#x2212;    x  2
      &#x03B1;  2        d x   {\displaystyle \operatorname {N} {\frac {1}
      {\alpha \;{\sqrt {\pi }}}}\;e^{-{\frac {x^{2}}{\alpha ^{2}}}}\,dx}  [
      {\displaystyle \operatorname {N} {\frac {1}{\alpha \;{\sqrt {\pi }}}}\;e^
      {-{\frac {x^{2}}{\alpha ^{2}}}}\,dx}]
**** Naming[edit] ****
Since its introduction, the normal distribution has been known by many
different names: the law of error, the law of facility of errors, Laplace's
second law, Gaussian law, etc. Gauss himself apparently coined the term with
reference to the "normal equations" involved in its applications, with normal
having its technical meaning of orthogonal rather than "usual".[72] However, by
the end of the 19th century some authors[note_6] had started using the name
normal distribution, where the word "normal" was used as an adjective â the
term now being seen as a reflection of the fact that this distribution was seen
as typical, common â and thus "normal". Peirce (one of those authors) once
defined "normal" thus: "...the 'normal' is not the average (or any other kind
of mean) of what actually occurs, but of what would, in the long run, occur
under certain circumstances."[73] Around the turn of the 20th century Pearson
popularized the term normal as a designation for this distribution.[74]
     Many years ago I called the LaplaceâGaussian curve the normal
     curve, which name, while it avoids an international question of
     priority, has the disadvantage of leading people to believe that all
     other distributions of frequency are in one sense or another
     'abnormal'.
     â Pearson_(1920)
Also, it was Pearson who first wrote the distribution in terms of the standard
deviation Ï as in modern notation. Soon after this, in year 1915, Fisher added
the location parameter to the formula for normal distribution, expressing it in
the way it is written nowadays:
         d f =   1  2  &#x03C3;  2   &#x03C0;     e  &#x2212; ( x &#x2212; m  )
      2    /  ( 2  &#x03C3;  2   )    d x   {\displaystyle df={\frac {1}{\sqrt
      {2\sigma ^{2}\pi }}}e^{-(x-m)^{2}/(2\sigma ^{2})}\,dx}  [{\displaystyle
      df={\frac {1}{\sqrt {2\sigma ^{2}\pi }}}e^{-(x-m)^{2}/(2\sigma ^
      {2})}\,dx}]
The term "standard normal", which denotes the normal distribution with zero
mean and unit variance came into general use around the 1950s, appearing in the
popular textbooks by P.G. Hoel (1947) "Introduction to mathematical statistics"
and A.M. Mood (1950) "Introduction to the theory of statistics".[75]
When the name is used, the "Gaussian distribution" was named_after Carl
Friedrich_Gauss, who introduced the distribution in 1809 as a way of
rationalizing the method_of_least_squares as outlined above. Among English
speakers, both "normal distribution" and "Gaussian distribution" are in common
use, with different terms preferred by different communities.
***** See also[edit] *****
    * [icon]Statistics_portal
    * Wrapped_normal_distribution â the Normal distribution applied to a
      circular domain
    * Bates_distribution â similar to the IrwinâHall distribution, but
      rescaled back into the 0 to 1 range
    * BehrensâFisher_problem â the long-standing problem of testing whether
      two normal samples with different variances have same means;
    * Bhattacharyya_distance â method used to separate mixtures of normal
      distributions
    * ErdÅsâKac_theoremâon the occurrence of the normal distribution in
      number_theory
    * Gaussian_blurâconvolution, which uses the normal distribution as a
      kernel
    * Normally_distributed_and_uncorrelated_does_not_imply_independent
    * Standard_normal_table
    * Sub-Gaussian_distribution
    * Sum_of_normally_distributed_random_variables
    * Tweedie_distribution â The normal distribution is a member of the
      family of Tweedie exponential_dispersion_models
    * Z-testâ using the normal distribution
    * Stein's_lemma
***** Notes[edit] *****
   1. ^ For the proof see Gaussian_integral.
   2. ^ For example, this algorithm is given in the article Bc_programming
      language.
   3. ^ De Moivre first published his findings in 1733, in a pamphlet
      "Approximatio ad Summam Terminorum Binomii (a + b)n in Seriem Expansi"
      that was designated for private circulation only. But it was not until
      the year 1738 that he made his results publicly available. The original
      pamphlet was reprinted several times, see for example Walker_(1985).
   4. ^ "It has been customary certainly to regard as an axiom the hypothesis
      that if any quantity has been determined by several direct observations,
      made under the same circumstances and with equal care, the arithmetical
      mean of the observed values affords the most probable value, if not
      rigorously, yet very nearly at least, so that it is always most safe to
      adhere to it." â Gauss_(1809, section 177)
   5. ^ "My custom of terming the curve the GaussâLaplacian or normal curve
      saves us from proportioning the merit of discovery between the two great
      astronomer mathematicians." quote from Pearson_(1905, p. 189)
   6. ^ Besides those specifically referenced here, such use is encountered in
      the works of Peirce, Galton (Galton_(1889, chapter V)) and Lexis (Lexis_
      (1878), Rohrbasser_&_VÃ©ron_(2003)) c. 1875.[citation_needed]
***** References[edit] *****
**** Citations[edit] ****
   1. ^ Normal_Distribution, Gale Encyclopedia of Psychology
   2. ^ Casella_&_Berger_(2001, p. 102)
   3. ^ Lyon, A. (2014). Why_are_Normal_Distributions_Normal?, The British
      Journal for the Philosophy of Science.
   4. ^ Stigler_(1982)
   5. ^ Halperin,_Hartley_&_Hoel_(1965, item 7)
   6. ^ McPherson_(1990, p. 110)
   7. ^ Bernardo_&_Smith_(2000, p. 121)
   8. ^Cover, Thomas M.; Thomas, Joy A. (2006). Elements of Information Theory.
      John Wiley and Sons. p. 254.
   9. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
  10. ^Park, Sung Y.; Bera, Anil K. (2009). "Maximum_Entropy_Autoregressive
      Conditional_Heteroskedasticity_Model" (PDF). Journal of Econometrics. 150
      (2): 219â230. CiteSeerX 10.1.1.511.9750. doi:10.1016/
      j.jeconom.2008.12.014. Retrieved June 2, 2011.
  11. ^ Geary RC(1936) The distribution of the "Student's" ratio for the non-
      normal samples". Supplement to the Journal of the Royal Statistical
      Society 3 (2): 178â184
  12. ^ Lukas E (1942) A characterization of the normal distribution. Annals of
      Mathematical Statistics 13: 91â93
  13. ^ a b c Patel_&_Read_(1996, [2.1.4])
  14. ^ Fan_(1991, p. 1258)
  15. ^ Patel_&_Read_(1996, [2.1.8])
  16. ^Papoulis, Athanasios. Probability, Random Variables and Stochastic
      Processes (4th Edition). p. 148.
  17. ^ Bryc_(1995, p. 23)
  18. ^ Bryc_(1995, p. 24)
  19. ^Scott, Clayton; Nowak, Robert (August 7, 2003). "The_Q-function".
      Connexions.
  20. ^Barak, Ohad (April 6, 2006). "Q_Function_and_Error_Function" (PDF). Tel
      Aviv University. Archived from the_original (PDF) on March 25, 2009.
  21. ^Weisstein,_Eric_W. "Normal_Distribution_Function". MathWorld.
  22. ^Abramowitz,_Milton; Stegun,_Irene_Ann, eds. (1983) [June 1964]. "Chapter
      26,_eqn_26.2.12". Handbook_of_Mathematical_Functions_with_Formulas,
      Graphs,_and_Mathematical_Tables. Applied Mathematics Series. 55 (Ninth
      reprint with additional corrections of tenth original printing with
      corrections (December 1972); first ed.). Washington D.C.; New York:
      United States Department of Commerce, National Bureau of Standards; Dover
      Publications. p. 932. ISBN 978-0-486-61272-0. LCCN 64-60036. MR 0167642.
      LCCN 65-12253.
  23. ^"Wolfram|Alpha:_Computational_Knowledge_Engine". Wolframalpha.com.
      Retrieved March 3, 2017.
  24. ^"Wolfram|Alpha:_Computational_Knowledge_Engine". Wolframalpha.com.
  25. ^"Wolfram|Alpha:_Computational_Knowledge_Engine". Wolframalpha.com.
      Retrieved March 3, 2017.
  26. ^"Normal_Approximation_to_Poisson_Distribution". Stat.ucla.edu. Retrieved
      March 3, 2017.
  27. ^ Cover_&_Thomas_(2006, p. 254)
  28. ^Williams, David (2001). Weighing the odds : a course in probability and
      statistics (Reprinted. ed.). Cambridge [u.a.]: Cambridge Univ. Press.
      pp. 197â199. ISBN 978-0-521-00618-7.
  29. ^Smith, JosÃ© M. Bernardo; Adrian F. M. (2000). Bayesian theory (Reprint
      ed.). Chichester [u.a.]: Wiley. pp. 209, 366. ISBN 978-0-471-49464-5.
  30. ^ O'Hagan, A. (1994) Kendall's Advanced Theory of statistics, Vol 2B,
      Bayesian Inference, Edward Arnold.
  31. ISBN 0-340-52922-9 (Section 5.40)
  32. ^ Bryc_(1995, p. 27)
  33. ^ Patel_&_Read_(1996, [2.3.6])
  34. ^ Galambos_&_Simonelli_(2004, Theorem 3.5)
  35. ^ a b Bryc_(1995, p. 35)
  36. ^ a b Lukacs_&_King_(1954)
  37. ^Quine, M.P. (1993). "On_three_characterisations_of_the_normal
      distribution". Probability and Mathematical Statistics. 14 (2):
      257â263.
  38. ^ UIUC,_Lecture_21._The_Multivariate_Normal_Distribution, 21.6:
      "Individually Gaussian Versus Jointly Gaussian".
  39. ^ Edward L. Melnick and Aaron Tenenbein, "Misspecifications of the Normal
      Distribution", The_American_Statistician, volume 36, number 4 November
      1982, pages 372â373
  40. ^"Kullback_Leibler_(KL)_Distance_of_Two_Normal_(Gaussian)_Probability
      Distributions". Allisons.org. December 5, 2007. Retrieved March 3, 2017.
  41. ^Jordan, Michael I. (February 8, 2010). "Stat260:_Bayesian_Modeling_and
      Inference:_The_Conjugate_Prior_for_the_Normal_Distribution" (PDF).
  42. ^ Amari_&_Nagaoka_(2000)
  43. ^Weisstein, Eric W. "Normal_Product_Distribution". MathWorld.
      wolfram.com.
  44. ^Lukacs, Eugene (1942). "A Characterization of the Normal Distribution".
      The_Annals_of_Mathematical_Statistics. 13 (1): 91â3. doi:10.1214/aoms/
      1177731647. ISSN 0003-4851. JSTOR 2236166.
  45. ^Basu, D.; Laha, R. G. (1954). "On Some Characterizations of the Normal
      Distribution". SankhyÄ. 13 (4): 359â62. ISSN 0036-4452.
      JSTOR 25048183.
  46. ^Lehmann, E. L. (1997). Testing Statistical Hypotheses (2nd ed.).
      Springer. p. 199. ISBN 978-0-387-94919-2.
  47. ^John, S (1982). "The three parameter two-piece normal family of
      distributions and its fitting". Communications in Statistics - Theory and
      Methods. 11 (8): 879â885. doi:10.1080/03610928208828279.
  48. ^ a b Krishnamoorthy_(2006, p. 127)
  49. ^ Krishnamoorthy_(2006, p. 130)
  50. ^ Krishnamoorthy_(2006, p. 133)
  51. ^ Huxley_(1932)
  52. ^Jaynes, Edwin T. (2003). Probability_Theory:_The_Logic_of_Science.
      Cambridge University Press. pp. 592â593. ISBN 9780521592710.
  53. ^Oosterbaan, Roland J. (1994). "Chapter_6:_Frequency_and_Regression
      Analysis_of_Hydrologic_Data" (PDF). In Ritzema, Henk P. (ed.). Drainage
      Principles and Applications, Publication 16 (second revised ed.).
      Wageningen, The Netherlands: International Institute for Land Reclamation
      and Improvement (ILRI). pp. 175â224. ISBN 978-90-70754-33-4.
  54. ^Wichura, Michael J. (1988). "Algorithm AS241: The Percentage Points of
      the Normal Distribution". Applied Statistics. 37 (3): 477â84. doi:
      10.2307/2347330. JSTOR 2347330.
  55. ^ Johnson,_Kotz_&_Balakrishnan_(1995, Equation (26.48))
  56. ^ Kinderman_&_Monahan_(1977)
  57. ^ Leva_(1992)
  58. ^ Marsaglia_&_Tsang_(2000)
  59. ^ Karney_(2016)
  60. ^ Monahan_(1985, section 2)
  61. ^ Wallace_(1996)
  62. ^ Johnson,_Kotz_&_Balakrishnan_(1994, p. 85)
  63. ^ Le_Cam_&_Lo_Yang_(2000, p. 74)
  64. ^ De Moivre, Abraham (1733), Corollary I â see Walker_(1985, p. 77)
  65. ^ Stigler_(1986, p. 76)
  66. ^ Gauss_(1809, section 177)
  67. ^ Gauss_(1809, section 179)
  68. ^ Laplace_(1774, Problem III)
  69. ^ Pearson_(1905, p. 189)
  70. ^ Stigler_(1986, p. 144)
  71. ^ Stigler_(1978, p. 243)
  72. ^ Stigler_(1978, p. 244)
  73. ^ Maxwell_(1860, p. 23)
  74. ^ Jaynes, Edwin J.; Probability_Theory:_The_Logic_of_Science,_Ch_7
  75. ^ Peirce, Charles S. (c. 1909 MS), Collected_Papers v. 6, paragraph 327
  76. ^ Kruskal_&_Stigler_(1997)
  77. ^"Earliest_usesâ¦_(entry_STANDARD_NORMAL_CURVE)".
**** Sources[edit] ****
    * Aldrich, John; Miller, Jeff. "Earliest_Uses_of_Symbols_in_Probability_and
      Statistics".
Aldrich, John; Miller, Jeff. "Earliest_Known_Uses_of_Some_of_the_Words_of
Mathematics".
 In particular, the entries for "bell-shaped_and_bell_curve", "normal_
(distribution)", "Gaussian", and "Error,_law_of_error,_theory_of_errors,_etc.".
Amari, Shun-ichi; Nagaoka, Hiroshi (2000). Methods of Information Geometry.
Oxford University Press. ISBN 978-0-8218-0531-2.
Bernardo, JosÃ© M.; Smith, Adrian F. M. (2000). Bayesian Theory. Wiley.
ISBN 978-0-471-49464-5.
Bryc, Wlodzimierz (1995). The Normal Distribution: Characterizations with
Applications. Springer-Verlag. ISBN 978-0-387-97990-8.
Casella, George; Berger, Roger L. (2001). Statistical Inference (2nd ed.).
Duxbury. ISBN 978-0-534-24312-8.
Cody, William J. (1969). "Rational_Chebyshev_Approximations_for_the_Error
Function". Mathematics of Computation. 23 (107): 631â638. doi:10.1090/S0025-
5718-1969-0247736-4.
Cover, Thomas M.; Thomas, Joy A. (2006). Elements of Information Theory. John
Wiley and Sons.
de_Moivre,_Abraham (1738). The_Doctrine_of_Chances. ISBN 978-0-8218-2103-9.
Fan, Jianqing (1991). "On the optimal rates of convergence for nonparametric
deconvolution problems". The Annals of Statistics. 19 (3): 1257â1272. doi:
10.1214/aos/1176348248. JSTOR 2241949.
Galton, Francis (1889). Natural_Inheritance (PDF). London, UK: Richard Clay and
Sons.
Galambos, Janos; Simonelli, Italo (2004). Products of Random Variables:
Applications to Problems of Physics and to Arithmetical Functions. Marcel
Dekker, Inc. ISBN 978-0-8247-5402-0.
Gauss,_Carolo_Friderico (1809). Theoria motvs corporvm coelestivm in
sectionibvs conicis Solem ambientivm [Theory of the Motion of the Heavenly
Bodies Moving about the Sun in Conic Sections] (in Latin). English_translation.
Gould,_Stephen_Jay (1981). The_Mismeasure_of_Man (first ed.). W. W. Norton.
ISBN 978-0-393-01489-1.
Halperin, Max; Hartley, Herman O.; Hoel, Paul G. (1965). "Recommended Standards
for Statistical Symbols and Notation. COPSS Committee on Symbols and Notation".
The American Statistician. 19 (3): 12â14. doi:10.2307/2681417. JSTOR 2681417.
Hart, John F.; et al. (1968). Computer Approximations. New York, NY: John Wiley
& Sons, Inc. ISBN 978-0-88275-642-4.
Hazewinkel,_Michiel, ed. (2001) [1994], "Normal_Distribution", Encyclopedia_of
Mathematics, Springer Science+Business Media B.V. / Kluwer Academic Publishers,
ISBN 978-1-55608-010-4
Herrnstein, Richard J.; Murray,_Charles (1994). The_Bell_Curve:_Intelligence
and_Class_Structure_in_American_Life. Free_Press. ISBN 978-0-02-914673-6.
Huxley, Julian S. (1932). Problems of Relative Growth. London. ISBN 978-0-486-
61114-3. OCLC 476909537.
Johnson, Norman L.; Kotz, Samuel; Balakrishnan, Narayanaswamy (1994).
Continuous Univariate Distributions, Volume 1. Wiley. ISBN 978-0-471-58495-7.
Johnson, Norman L.; Kotz, Samuel; Balakrishnan, Narayanaswamy (1995).
Continuous Univariate Distributions, Volume 2. Wiley. ISBN 978-0-471-58494-0.
Karney, C. F. F. (2016). "Sampling exactly from the normal distribution". ACM
Transactions on Mathematical Software. 42 (1): 3:1â14. arXiv:1303.6257. doi:
10.1145/2710016.
Kinderman, Albert J.; Monahan, John F. (1977). "Computer Generation of Random
Variables Using the Ratio of Uniform Deviates". ACM Transactions on
Mathematical Software. 3 (3): 257â260. doi:10.1145/355744.355750.
Krishnamoorthy, Kalimuthu (2006). Handbook of Statistical Distributions with
Applications. Chapman & Hall/CRC. ISBN 978-1-58488-635-8.
Kruskal, William H.; Stigler, Stephen M. (1997). Spencer, Bruce D. (ed.).
Normative Terminology: 'Normal' in Statistics and Elsewhere. Statistics and
Public Policy. Oxford University Press. ISBN 978-0-19-852341-3.
Laplace,_Pierre-Simon_de (1774). "MÃ©moire_sur_la_probabilitÃ©_des_causes_par
les_Ã©vÃ©nements". MÃ©moires de l'AcadÃ©mie Royale des Sciences de Paris
(Savants Ã©trangers), Tome 6: 621â656.
 Translated by Stephen M. Stigler in Statistical Science 1 (3), 1986:
JSTOR 2245476.
Laplace, Pierre-Simon (1812). ThÃ©orie analytique des probabilitÃ©s [Analytical
theory_of_probabilities].
Le Cam, Lucien; Lo Yang, Grace (2000). Asymptotics in Statistics: Some Basic
Concepts (second ed.). Springer. ISBN 978-0-387-95036-5.
Leva, Joseph L. (1992). "A_fast_normal_random_number_generator" (PDF). ACM
Transactions on Mathematical Software. 18 (4): 449â453.
CiteSeerX 10.1.1.544.5806. doi:10.1145/138351.138364. Archived from the
original (PDF) on July 16, 2010.
Lexis, Wilhelm (1878). "Sur la durÃ©e normale de la vie humaine et sur la
thÃ©orie de la stabilitÃ© des rapports statistiques". Annales de DÃ©mographie
Internationale. Paris. II: 447â462.
Lukacs, Eugene; King, Edgar P. (1954). "A Property of Normal Distribution". The
Annals of Mathematical Statistics. 25 (2): 389â394. doi:10.1214/aoms/
1177728796. JSTOR 2236741.
McPherson, Glen (1990). Statistics in Scientific Investigation: Its Basis,
Application and Interpretation. Springer-Verlag. ISBN 978-0-387-97137-7.
Marsaglia,_George; Tsang, Wai Wan (2000). "The Ziggurat Method for Generating
Random Variables". Journal of Statistical Software. 5 (8). doi:10.18637/
jss.v005.i08.
Marsaglia, George (2004). "Evaluating the Normal Distribution". Journal of
Statistical Software. 11 (4). doi:10.18637/jss.v011.i04.
Maxwell,_James_Clerk (1860). "V. Illustrations of the dynamical theory of
gases. â Part I: On the motions and collisions of perfectly elastic spheres".
Philosophical Magazine. Series 4. 19 (124): 19â32. doi:10.1080/
14786446008642818.
Monahan, J. F. (1985). "Accuracy in random number generation". Mathematics of
Computation. 45 (172): 559â568. doi:10.1090/S0025-5718-1985-0804945-X.
Patel, Jagdish K.; Read, Campbell B. (1996). Handbook of the Normal
Distribution (2nd ed.). CRC Press. ISBN 978-0-8247-9342-5.
Pearson,_Karl (1901). "On_Lines_and_Planes_of_Closest_Fit_to_Systems_of_Points
in_Space" (PDF). Philosophical_Magazine. 6. 2 (11): 559â572. doi:10.1080/
14786440109462720.
Pearson,_Karl (1905). "'Das Fehlergesetz und seine Verallgemeinerungen durch
Fechner und Pearson'. A rejoinder". Biometrika. 4 (1): 169â212. doi:10.2307/
2331536. JSTOR 2331536.
Pearson, Karl (1920). "Notes on the History of Correlation". Biometrika. 13
(1): 25â45. doi:10.1093/biomet/13.1.25. JSTOR 2331722.
Rohrbasser, Jean-Marc; VÃ©ron, Jacques (2003). "Wilhelm_Lexis:_The_Normal
Length_of_Life_as_an_Expression_of_the_"Nature_of_Things"". Population. 58 (3):
303â322. doi:10.3917/pope.303.0303.
Shore, H (1982). "Simple Approximations for the Inverse Cumulative Function,
the Density Function and the Loss Integral of the Normal Distribution". Journal
of the Royal Statistical Society. Series C (Applied Statistics). 31 (2):
108â114. doi:10.2307/2347972. JSTOR 2347972.
Shore, H (2005). "Accurate RMM-Based Approximations for the CDF of the Normal
Distribution". Communications in Statistics â Theory and Methods. 34 (3):
507â513. doi:10.1081/sta-200052102.
Shore, H (2011). "Response Modeling Methodology". WIREs Comput Stat. 3 (4):
357â372. doi:10.1002/wics.151.
Shore, H (2012). "Estimating Response Modeling Methodology Models". WIREs
Comput Stat. 4 (3): 323â333. doi:10.1002/wics.1199.
Stigler,_Stephen_M. (1978). "Mathematical Statistics in the Early States". The
Annals of Statistics. 6 (2): 239â265. doi:10.1214/aos/1176344123.
JSTOR 2958876.
Stigler, Stephen M. (1982). "A Modest Proposal: A New Standard for the Normal".
The American Statistician. 36 (2): 137â138. doi:10.2307/2684031.
JSTOR 2684031.
Stigler, Stephen M. (1986). The History of Statistics: The Measurement of
Uncertainty before 1900. Harvard University Press. ISBN 978-0-674-40340-6.
Stigler, Stephen M. (1999). Statistics on the Table. Harvard University Press.
ISBN 978-0-674-83601-3.
Walker, Helen M. (1985). "De_Moivre_on_the_Law_of_Normal_Probability" (PDF). In
Smith, David Eugene (ed.). A Source Book in Mathematics. Dover. ISBN 978-0-486-
64690-9.
Wallace,_C._S. (1996). "Fast pseudo-random generators for normal and
exponential variates". ACM Transactions on Mathematical Software. 22 (1):
119â127. doi:10.1145/225545.225554.
Weisstein,_Eric_W. "Normal_Distribution". MathWorld.
West, Graeme (2009). "Better_Approximations_to_Cumulative_Normal_Functions"
(PDF). Wilmott Magazine: 70â76.
Zelen, Marvin; Severo, Norman C. (1964). Probability_Functions_(chapter_26).
Handbook_of_mathematical_functions_with_formulas,_graphs,_and_mathematical
tables, by Abramowitz,_M.; and Stegun,_I._A.: National Bureau of Standards. New
York, NY: Dover. ISBN 978-0-486-61272-0.
***** External links[edit] *****
 Wikimedia Commons has media related to Normal_distribution.
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Normal_distribution",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Normal_distribution_calculator
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
                                          * normal (Gaussian)
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
index.php?title=Normal_distribution&oldid=908137280"
Categories:
    * Continuous_distributions
    * Conjugate_prior_distributions
    * Normal_distribution
    * Exponential_family_distributions
    * Stable_distributions
    * Location-scale_family_probability_distributions
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_June_2011
    * Use_mdy_dates_from_August_2012
    * Pages_using_deprecated_image_syntax
    * Articles_with_unsourced_statements_from_June_2010
    * CS1_Latin-language_sources_(la)
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
    * Alemannisch
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * ØªÛØ±Ú©Ø¬Ù
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
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
    * Gaeilge
    * Galego
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Latina
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * à¤®à¤°à¤¾à¤ à¥
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Basa_Sunda
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ××Ö´×××©
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 27 July 2019, at 18:18 (UTC).
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
