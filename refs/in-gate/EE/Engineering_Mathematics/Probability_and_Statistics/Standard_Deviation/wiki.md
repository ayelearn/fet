The following text has been accessed from https://en.wikipedia.org/wiki/Standard_deviation at Thu Aug 8 22:52:09 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Standard deviation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
dispersion of the values of a random variable around its expected value
For other uses, see Standard_deviation_(disambiguation).
A plot of normal_distribution (or bell-shaped curve) where each band has a
width of 1 standard deviation â See also: 68â95â99.7_rule.
Cumulative probability of a normal distribution with expected value 0 and
standard deviation 1
In statistics, the standard deviation (SD, also represented by the lower case
Greek letter sigma Ï for the population standard deviation or the Latin letter
s for the sample standard deviation) is a measure that is used to quantify the
amount of variation or dispersion of a set of data values.[1] A low standard
deviation indicates that the data points tend to be close to the mean (also
called the expected value) of the set, while a high standard deviation
indicates that the data points are spread out over a wider range of values.
The standard deviation of a random_variable, statistical_population, data_set,
or probability_distribution is the square_root of its variance. It is
algebraically simpler, though in practice less robust, than the average
absolute_deviation.[2][3] A useful property of the standard deviation is that,
unlike the variance, it is expressed in the same units as the data.
In addition to expressing the variability of a population, the standard
deviation is commonly used to measure confidence in statistical conclusions.
For example, the margin_of_error in polling data is determined by calculating
the expected standard deviation in the results if the same poll were to be
conducted multiple times. This derivation of a standard deviation is often
called the "standard_error" of the estimate or "standard error of the mean"
when referring to a mean. It is computed as the standard deviation of all the
means that would be computed from that population if an infinite number of
samples were drawn and a mean for each sample were computed.
The standard deviation of a population and the standard error of a statistic
derived from that population (such as the mean) are quite different but related
(related by the inverse of the square root of the number of observations). The
reported margin of error of a poll is computed from the standard error of the
mean (or alternatively from the product of the standard deviation of the
population and the inverse of the square root of the sample size, which is the
same thing) and is typically about twice the standard deviationâthe half-
width of a 95 percent confidence_interval.
In science, many researchers report the standard deviation of experimental
data, and only effects that fall much farther than two standard deviations away
from what would have been expected are considered statistically
significantânormal random error or variation in the measurements is in this
way distinguished from likely genuine effects or associations. The standard
deviation is also important in finance, where the standard deviation on the
rate_of_return on an investment is a measure of the volatility of the
investment.
When only a sample of data from a population is available, the term standard
deviation of the sample or sample standard deviation can refer to either the
above-mentioned quantity as applied to those data or to a modified quantity
that is an unbiased estimate of the population standard deviation (the standard
deviation of the entire population).
⁰
***** Contents *****
    * 1_Basic_examples
          o 1.1_Sample_standard_deviation_of_metabolic_rate_of_northern_fulmars
          o 1.2_Population_standard_deviation_of_grades_of_eight_students
          o 1.3_Standard_deviation_of_average_height_for_adult_men
    * 2_Definition_of_population_values
          o 2.1_Discrete_random_variable
          o 2.2_Continuous_random_variable
    * 3_Estimation
          o 3.1_Uncorrected_sample_standard_deviation
          o 3.2_Corrected_sample_standard_deviation
          o 3.3_Unbiased_sample_standard_deviation
          o 3.4_Confidence_interval_of_a_sampled_standard_deviation
          o 3.5_Bounds_on_standard_deviation
    * 4_Identities_and_mathematical_properties
    * 5_Interpretation_and_application
          o 5.1_Application_examples
                # 5.1.1_Experiment,_industrial_and_hypothesis_testing
                # 5.1.2_Weather
                # 5.1.3_Finance
          o 5.2_Geometric_interpretation
          o 5.3_Chebyshev's_inequality
          o 5.4_Rules_for_normally_distributed_data
    * 6_Relationship_between_standard_deviation_and_mean
          o 6.1_Standard_deviation_of_the_mean
    * 7_Rapid_calculation_methods
          o 7.1_Weighted_calculation
    * 8_History
    * 9_See_also
    * 10_References
    * 11_External_links
***** Basic examples[edit] *****
**** Sample standard deviation of metabolic rate of northern fulmars[edit] ****
Logan[4] gives the following example. Furness and Bryant[5] measured the
resting metabolic_rate for 8 male and 6 female breeding northern_fulmars. The
table shows the Furness data set.
 Furness data set on metabolic rates of
            northern fulmars
Sex  Metabolic rate Sex    Metabolic rate
Male 525.8          Female 727.7
Male 605.7          Female 1086.5
Male 843.3          Female 1091.0
Male 1195.5         Female 1361.3
Male 1945.6         Female 1490.5
Male 2135.6         Female 1956.1
Male 2308.7
Male 2950.0
The graph shows the metabolic rate for males and females. By visual inspection,
it appears that the variability of the metabolic rate is greater for males than
for females.
[Graph_of_metabolic_rates_for_northern_fulmars]
The sample standard deviation of the metabolic rate for the female fulmars is
calculated as follows. The formula for the sample standard deviation is
         s =     1  N &#x2212; 1     &#x2211;  i = 1   N   (  x  i   &#x2212;
      x &#x00AF;     )  2     ,   {\displaystyle s={\sqrt {{\frac {1}{N-1}}\sum
      _{i=1}^{N}(x_{i}-{\bar {x}})^{2}}},}  [{\displaystyle s={\sqrt {{\frac
      {1}{N-1}}\sum _{i=1}^{N}(x_{i}-{\bar {x}})^{2}}},}]
where      {  x  1   ,   x  2   ,  &#x2026; ,   x  N   }    {\displaystyle
\textstyle \{x_{1},\,x_{2},\,\ldots ,\,x_{N}\}}  [{\displaystyle \textstyle \
{x_{1},\,x_{2},\,\ldots ,\,x_{N}\}}] are the observed values of the sample
items,         x &#x00AF;       {\displaystyle \textstyle {\bar {x}}}  [
{\displaystyle \textstyle {\bar {x}}}] is the mean value of these observations,
and N is the number of observations in the sample.
In the sample standard deviation formula, for this example, the numerator is
the sum of the squared deviation of each individual animal's metabolic rate
from the mean metabolic rate. The table below shows the calculation of this sum
of squared deviations for the female fulmars. For females, the sum of squared
deviations is 886047.09, as shown in the table.
               Sum of squares calculation for female fulmars
Animal Sex    Metabolic rate Mean   Difference from mean Squared difference
                                                         from mean
1      Female 727.7          1285.5 -557.8               311140.84
2      Female 1086.5         1285.5 -199.0               39601.00
3      Female 1091.0         1285.5 -194.5               37830.25
4      Female 1361.3         1285.5 75.8                 5745.64
5      Female 1490.5         1285.5 205.0                42025.00
6      Female 1956.1         1285.5 670.6                449704.36
Mean of metabolic rates      1285.5 Sum of squared       886047.09
                                    differences
The denominator in the sample standard deviation formula is N â 1, where N is
the number of animals. In this example, there are N = 6 females, so the
denominator is 6 â 1 = 5. The sample standard deviation for the female
fulmars is therefore
         s =      &#x2211;  i = 1   N   (  x  i   &#x2212;    x &#x00AF;     )
      2     N &#x2212; 1     =    886047.09 5    = 420.96.   {\displaystyle s=
      {\sqrt {\frac {\sum _{i=1}^{N}(x_{i}-{\bar {x}})^{2}}{N-1}}}={\sqrt
      {\frac {886047.09}{5}}}=420.96.}  [{\displaystyle s={\sqrt {\frac {\sum _
      {i=1}^{N}(x_{i}-{\bar {x}})^{2}}{N-1}}}={\sqrt {\frac {886047.09}
      {5}}}=420.96.}]
For the male fulmars, a similar calculation gives a sample standard deviation
of 894.37, approximately twice as large as the standard deviation for the
females. The graph shows the metabolic rate data, the means (red dots), and the
standard deviations (red lines) for females and males.
[Graph_of_standard_deviation_of_metabolic_rate_of_fulmars]
Use of the sample standard deviation implies that these 14 fulmars are a sample
from a larger population of fulmars. If these 14 fulmars comprised the entire
population (perhaps the last 14 surviving fulmars), then instead of the sample
standard deviation, the calculation would use the population standard
deviation. In the population standard deviation formula, the denominator is N
instead of N - 1. It is rare that measurements can be taken for an entire
population, so, by default, statistical computer_programs calculate the sample
standard deviation. Similarly, journal articles report the sample standard
deviation unless otherwise specified.
**** Population standard deviation of grades of eight students[edit] ****
Suppose that the entire population of interest was eight students in a
particular class. For a finite set of numbers, the population standard
deviation is found by taking the square_root of the average of the squared
deviations of the values subtracted from their average value. The marks of a
class of eight students (that is, a statistical_population) are the following
eight values:
         2 , &#xA0; 4 , &#xA0; 4 , &#xA0; 4 , &#xA0; 5 , &#xA0; 5 , &#xA0; 7 ,
      &#xA0; 9.   {\displaystyle 2,\ 4,\ 4,\ 4,\ 5,\ 5,\ 7,\ 9.}  [2,\ 4,\ 4,\
      4,\ 5,\ 5,\ 7,\ 9.]
These eight data points have the mean (average) of 5:
         &#x03BC; =    2 + 4 + 4 + 4 + 5 + 5 + 7 + 9  8   = 5.   {\displaystyle
      \mu ={\frac {2+4+4+4+5+5+7+9}{8}}=5.}  [{\displaystyle \mu ={\frac
      {2+4+4+4+5+5+7+9}{8}}=5.}]
First, calculate the deviations of each data point from the mean, and square
the result of each:
             ( 2 &#x2212; 5  )  2   = ( &#x2212; 3  )  2   = 9    ( 5 &#x2212;
      5  )  2   =  0  2   = 0     ( 4 &#x2212; 5  )  2   = ( &#x2212; 1  )  2
      = 1    ( 5 &#x2212; 5  )  2   =  0  2   = 0     ( 4 &#x2212; 5  )  2   =
      ( &#x2212; 1  )  2   = 1    ( 7 &#x2212; 5  )  2   =  2  2   = 4     ( 4
      &#x2212; 5  )  2   = ( &#x2212; 1  )  2   = 1    ( 9 &#x2212; 5  )  2   =
      4  2   = 16.       {\displaystyle {\begin{array}{lll}(2-5)^{2}=(-3)^
      {2}=9&&(5-5)^{2}=0^{2}=0\\(4-5)^{2}=(-1)^{2}=1&&(5-5)^{2}=0^{2}=0\\(4-5)^
      {2}=(-1)^{2}=1&&(7-5)^{2}=2^{2}=4\\(4-5)^{2}=(-1)^{2}=1&&(9-5)^{2}=4^
      {2}=16.\\\end{array}}}  [{\begin{array}{lll}(2-5)^{2}=(-3)^{2}=9&&(5-5)^
      {2}=0^{2}=0\\(4-5)^{2}=(-1)^{2}=1&&(5-5)^{2}=0^{2}=0\\(4-5)^{2}=(-1)^
      {2}=1&&(7-5)^{2}=2^{2}=4\\(4-5)^{2}=(-1)^{2}=1&&(9-5)^{2}=4^{2}=16.\\\end
      {array}}]
The variance is the mean of these values:
          &#x03C3;  2   =    9 + 1 + 1 + 1 + 0 + 0 + 4 + 16  8   = 4.
      {\displaystyle \sigma ^{2}={\frac {9+1+1+1+0+0+4+16}{8}}=4.}  [
      {\displaystyle \sigma ^{2}={\frac {9+1+1+1+0+0+4+16}{8}}=4.}]
and the population standard deviation is equal to the square root of the
variance:
         &#x03C3; =   4   = 2.   {\displaystyle \sigma ={\sqrt {4}}=2.}  [
      {\displaystyle \sigma ={\sqrt {4}}=2.}]
This formula is valid only if the eight values with which we began form the
complete population. If the values instead were a random sample drawn from some
large parent population (for example, they were 8 marks randomly and
independently chosen from a class of 2 million), then one often divides by 7 
(which is n â 1) instead of 8 (which is n) in the denominator of the last
formula. In that case the result of the original formula would be called the
sample standard deviation. Dividing by n â 1 rather than by n gives an
unbiased estimate of the variance of the larger parent population. This is
known as Bessel's_correction.[6]
**** Standard deviation of average height for adult men[edit] ****
If the population of interest is approximately normally distributed, the
standard deviation provides information on the proportion of observations above
or below certain values. For example, the average_height_for_adult_men in the
United_States is about 70 inches (177.8 cm), with a standard deviation of
around 3 inches (7.62 cm). This means that most men (about 68%, assuming a
normal_distribution) have a height within 3 inches (7.62 cm) of the mean
(67â73 inches (170.18â185.42 cm)) – one standard deviation – and almost all
men (about 95%) have a height within 6 inches (15.24 cm) of the mean
(64â76 inches (162.56â193.04 cm)) – two standard deviations. If the
standard deviation were zero, then all men would be exactly 70 inches
(177.8 cm) tall. If the standard deviation were 20 inches (50.8 cm), then men
would have much more variable heights, with a typical range of about
50â90 inches (127â228.6 cm). Three standard deviations account for 99.7% of
the sample population being studied, assuming the distribution is normal (bell-
shaped). (See the 68-95-99.7_rule, or the empirical rule, for more
information.)
***** Definition of population values[edit] *****
Let X be a random_variable with mean value Î¼:
         E &#x2061; [ X ] = &#x03BC; .     {\displaystyle \operatorname {E}
      [X]=\mu .\,\!}  [\operatorname {E} [X]=\mu .\,\!]
Here the operator E denotes the average or expected_value of X. Then the
standard deviation of X is the quantity
             &#x03C3;    =   E &#x2061; [ ( X &#x2212; &#x03BC;  )  2   ]
      =   E &#x2061; [  X  2   ] + E &#x2061; [ &#x2212; 2 &#x03BC; X ] + E
      &#x2061; [  &#x03BC;  2   ]         =   E &#x2061; [  X  2   ] &#x2212; 2
      &#x03BC; E &#x2061; [ X ] +  &#x03BC;  2           =   E &#x2061; [  X  2
      ] &#x2212; 2  &#x03BC;  2   +  &#x03BC;  2           =   E &#x2061; [  X
      2   ] &#x2212;  &#x03BC;  2           =   E &#x2061; [  X  2   ] &#x2212;
      ( E &#x2061; [ X ]  )  2           {\displaystyle {\begin{aligned}\sigma
      &={\sqrt {\operatorname {E} [(X-\mu )^{2}]}}\\&={\sqrt {\operatorname {E}
      [X^{2}]+\operatorname {E} [-2\mu X]+\operatorname {E} [\mu ^{2}]}}\\&=
      {\sqrt {\operatorname {E} [X^{2}]-2\mu \operatorname {E} [X]+\mu ^
      {2}}}\\&={\sqrt {\operatorname {E} [X^{2}]-2\mu ^{2}+\mu ^{2}}}\\&={\sqrt
      {\operatorname {E} [X^{2}]-\mu ^{2}}}\\&={\sqrt {\operatorname {E} [X^
      {2}]-(\operatorname {E} [X])^{2}}}\end{aligned}}}  [{\displaystyle
      {\begin{aligned}\sigma &={\sqrt {\operatorname {E} [(X-\mu )^{2}]}}\\&=
      {\sqrt {\operatorname {E} [X^{2}]+\operatorname {E} [-2\mu
      X]+\operatorname {E} [\mu ^{2}]}}\\&={\sqrt {\operatorname {E} [X^{2}]-
      2\mu \operatorname {E} [X]+\mu ^{2}}}\\&={\sqrt {\operatorname {E} [X^
      {2}]-2\mu ^{2}+\mu ^{2}}}\\&={\sqrt {\operatorname {E} [X^{2}]-\mu ^
      {2}}}\\&={\sqrt {\operatorname {E} [X^{2}]-(\operatorname {E} [X])^
      {2}}}\end{aligned}}}]
(derived using the properties_of_expected_value).
In other words, the standard deviation Ï (sigma) is the square root of the
variance of X; i.e., it is the square root of the average value of (X â Î¼)2.
The standard deviation of a (univariate) probability distribution is the same
as that of a random variable having that distribution. Not all random variables
have a standard deviation, since these expected values need not exist. For
example, the standard deviation of a random variable that follows a Cauchy
distribution is undefined because its expected value Î¼ is undefined.
**** Discrete random variable[edit] ****
In the case where X takes random values from a finite data set x1, x2, ..., xN,
with each value having the same probability, the standard deviation is
         &#x03C3; =     1 N    [  (  x  1   &#x2212; &#x03BC;  )  2   + (  x  2
      &#x2212; &#x03BC;  )  2   + &#x22EF; + (  x  N   &#x2212; &#x03BC;  )  2
      ]    ,   &#xA0; &#xA0; w h e r e &#xA0; &#xA0;   &#x03BC; =   1 N   (  x
      1   + &#x22EF; +  x  N   ) ,   {\displaystyle \sigma ={\sqrt {{\frac {1}
      {N}}\left[(x_{1}-\mu )^{2}+(x_{2}-\mu )^{2}+\cdots +(x_{N}-\mu )^
      {2}\right]}},{\rm {\ \ where\ \ }}\mu ={\frac {1}{N}}(x_{1}+\cdots +x_
      {N}),}  [\sigma ={\sqrt {{\frac {1}{N}}\left[(x_{1}-\mu )^{2}+(x_{2}-\mu
      )^{2}+\cdots +(x_{N}-\mu )^{2}\right]}},{\rm {\ \ where\ \ }}\mu ={\frac
      {1}{N}}(x_{1}+\cdots +x_{N}),]
or, using summation notation,
         &#x03C3; =     1 N    &#x2211;  i = 1   N   (  x  i   &#x2212;
      &#x03BC;  )  2     ,   &#xA0; &#xA0; w h e r e &#xA0; &#xA0;   &#x03BC; =
      1 N    &#x2211;  i = 1   N    x  i   .   {\displaystyle \sigma ={\sqrt {
      {\frac {1}{N}}\sum _{i=1}^{N}(x_{i}-\mu )^{2}}},{\rm {\ \ where\ \ }}\mu
      ={\frac {1}{N}}\sum _{i=1}^{N}x_{i}.}  [\sigma ={\sqrt {{\frac {1}
      {N}}\sum _{i=1}^{N}(x_{i}-\mu )^{2}}},{\rm {\ \ where\ \ }}\mu ={\frac
      {1}{N}}\sum _{i=1}^{N}x_{i}.]
If, instead of having equal probabilities, the values have different
probabilities, let x1 have probability p1, x2 have probability p2, ..., xN have
probability pN. In this case, the standard deviation will be
         &#x03C3; =    &#x2211;  i = 1   N    p  i   (  x  i   &#x2212;
      &#x03BC;  )  2     ,   &#xA0; &#xA0; w h e r e &#xA0; &#xA0;   &#x03BC; =
      &#x2211;  i = 1   N    p  i    x  i   .   {\displaystyle \sigma ={\sqrt
      {\sum _{i=1}^{N}p_{i}(x_{i}-\mu )^{2}}},{\rm {\ \ where\ \ }}\mu =\sum _
      {i=1}^{N}p_{i}x_{i}.}  [\sigma ={\sqrt {\sum _{i=1}^{N}p_{i}(x_{i}-\mu )^
      {2}}},{\rm {\ \ where\ \ }}\mu =\sum _{i=1}^{N}p_{i}x_{i}.]
**** Continuous random variable[edit] ****
The standard deviation of a continuous_real-valued_random_variable X with
probability_density_function p(x) is
         &#x03C3; =    &#x222B;   X    ( x &#x2212; &#x03BC;  )  2    p ( x )
      d   x   ,   &#xA0; &#xA0; w h e r e &#xA0; &#xA0;   &#x03BC; =  &#x222B;
      X    x  p ( x )    d   x ,   {\displaystyle \sigma ={\sqrt {\int _
      {\mathbf {X} }(x-\mu )^{2}\,p(x)\,{\rm {d}}x}},{\rm {\ \ where\ \ }}\mu
      =\int _{\mathbf {X} }x\,p(x)\,{\rm {d}}x,}  [{\displaystyle \sigma =
      {\sqrt {\int _{\mathbf {X} }(x-\mu )^{2}\,p(x)\,{\rm {d}}x}},{\rm {\ \
      where\ \ }}\mu =\int _{\mathbf {X} }x\,p(x)\,{\rm {d}}x,}]
and where the integrals are definite_integrals taken for x ranging over the set
of possible values of the random variable X.
In the case of a parametric_family_of_distributions, the standard deviation can
be expressed in terms of the parameters. For example, in the case of the log-
normal_distribution with parameters Î¼ and Ï2, the standard deviation is
           (  e   &#x03C3;  2     &#x2212; 1 )  e  2 &#x03BC; +  &#x03C3;  2
      .   {\displaystyle {\sqrt {(e^{\sigma ^{2}}-1)e^{2\mu +\sigma ^{2}}}}.}
      [{\displaystyle {\sqrt {(e^{\sigma ^{2}}-1)e^{2\mu +\sigma ^{2}}}}.}]
***** Estimation[edit] *****
See also: Sample_variance
Main article: Unbiased_estimation_of_standard_deviation
One can find the standard deviation of an entire population in cases (such as
standardized_testing) where every member of a population is sampled. In cases
where that cannot be done, the standard deviation Ï is estimated by examining
a random sample taken from the population and computing a statistic of the
sample, which is used as an estimate of the population standard deviation. Such
a statistic is called an estimator, and the estimator (or the value of the
estimator, namely the estimate) is called a sample standard deviation, and is
denoted by s (possibly with modifiers).
Unlike in the case of estimating the population mean, for which the sample_mean
is a simple estimator with many desirable properties (unbiased, efficient,
maximum likelihood), there is no single estimator for the standard deviation
with all these properties, and unbiased_estimation_of_standard_deviation is a
very technically involved problem. Most often, the standard deviation is
estimated using the corrected_sample_standard_deviation (using N â 1),
defined below, and this is often referred to as the "sample standard
deviation", without qualifiers. However, other estimators are better in other
respects: the uncorrected estimator (using N) yields lower mean squared error,
while using N â 1.5 (for the normal distribution) almost completely
eliminates bias.
**** Uncorrected sample standard deviation[edit] ****
The formula for the population standard deviation (of a finite population) can
be applied to the sample, using the size of the sample as the size of the
population (though the actual population size from which the sample is drawn
may be much larger). This estimator, denoted by sN, is known as the uncorrected
sample standard deviation, or sometimes the standard deviation of the sample
(considered as the entire population), and is defined as follows:[citation
needed]
          s  N   =     1 N    &#x2211;  i = 1   N   (  x  i   &#x2212;    x
      &#x00AF;     )  2     ,   {\displaystyle s_{N}={\sqrt {{\frac {1}{N}}\sum
      _{i=1}^{N}(x_{i}-{\bar {x}})^{2}}},}  [{\displaystyle s_{N}={\sqrt {
      {\frac {1}{N}}\sum _{i=1}^{N}(x_{i}-{\bar {x}})^{2}}},}]
where      {  x  1   ,   x  2   ,  &#x2026; ,   x  N   }    {\displaystyle
\textstyle \{x_{1},\,x_{2},\,\ldots ,\,x_{N}\}}  [{\displaystyle \textstyle \
{x_{1},\,x_{2},\,\ldots ,\,x_{N}\}}] are the observed values of the sample
items and         x &#x00AF;       {\displaystyle \textstyle {\bar {x}}}  [
{\displaystyle \textstyle {\bar {x}}}] is the mean value of these observations,
while the denominator N stands for the size of the sample: this is the square
root of the sample variance, which is the average of the squared_deviations
about the sample mean.
This is a consistent_estimator (it converges in probability to the population
value as the number of samples goes to infinity), and is the maximum-likelihood
estimate when the population is normally distributed.[citation_needed] However,
this is a biased_estimator, as the estimates are generally too low. The bias
decreases as sample size grows, dropping off as 1/N, and thus is most
significant for small or moderate sample sizes; for     N > 75   {\displaystyle
N>75}  [{\displaystyle N>75}] the bias is below 1%. Thus for very large sample
sizes, the uncorrected sample standard deviation is generally acceptable. This
estimator also has a uniformly smaller mean_squared_error than the corrected
sample standard deviation.
**** Corrected sample standard deviation[edit] ****
If the biased sample_variance (the second central_moment of the sample, which
is a downward-biased estimate of the population variance) is used to compute an
estimate of the population's standard deviation, the result is
          s  N   =     1 N    &#x2211;  i = 1   N   (  x  i   &#x2212;   x
      &#x00AF;    )  2     .   {\displaystyle s_{N}={\sqrt {{\frac {1}{N}}\sum
      _{i=1}^{N}(x_{i}-{\overline {x}})^{2}}}.}  [s_{N}={\sqrt {{\frac {1}
      {N}}\sum _{i=1}^{N}(x_{i}-{\overline {x}})^{2}}}.]
Here taking the square root introduces further downward bias, by Jensen's
inequality, due to the square root's being a concave_function. The bias in the
variance is easily corrected, but the bias from the square root is more
difficult to correct, and depends on the distribution in question.
An unbiased estimator for the variance is given by applying Bessel's
correction, using N â 1 instead of N to yield the unbiased sample variance,
denoted s2:
          s  2   =   1  N &#x2212; 1     &#x2211;  i = 1   N   (  x  i
      &#x2212;   x &#x00AF;    )  2   .   {\displaystyle s^{2}={\frac {1}{N-
      1}}\sum _{i=1}^{N}(x_{i}-{\overline {x}})^{2}.}  [s^{2}={\frac {1}{N-
      1}}\sum _{i=1}^{N}(x_{i}-{\overline {x}})^{2}.]
This estimator is unbiased if the variance exists and the sample values are
drawn independently with replacement. N â 1 corresponds to the number of
degrees_of_freedom in the vector of deviations from the mean,      (  x  1
&#x2212;   x &#x00AF;   ,  &#x2026; ,   x  n   &#x2212;   x &#x00AF;   ) .
{\displaystyle \textstyle (x_{1}-{\overline {x}},\;\dots ,\;x_{n}-{\overline
{x}}).}  [{\displaystyle \textstyle (x_{1}-{\overline {x}},\;\dots ,\;x_{n}-
{\overline {x}}).}]
Taking square roots reintroduces bias (because the square root is a nonlinear
function, which does not commute with the expectation), yielding the corrected
sample standard deviation, denoted by s:
         s =     1  N &#x2212; 1     &#x2211;  i = 1   N   (  x  i   &#x2212;
      x &#x00AF;    )  2     .   {\displaystyle s={\sqrt {{\frac {1}{N-1}}\sum
      _{i=1}^{N}(x_{i}-{\overline {x}})^{2}}}.}  [s={\sqrt {{\frac {1}{N-
      1}}\sum _{i=1}^{N}(x_{i}-{\overline {x}})^{2}}}.]
As explained above, while s2 is an unbiased estimator for the population
variance, s is still a biased estimator for the population standard deviation,
though markedly less biased than the uncorrected sample standard deviation.
This estimator is commonly used and generally known simply as the "sample
standard deviation". The bias may still be large for small samples (N less than
10). As sample size increases, the amount of bias decreases. We obtain more
information and the difference between       1 N     {\displaystyle {\frac {1}
{N}}}  [{\frac  {1}{N}}] and       1  N &#x2212; 1      {\displaystyle {\frac
{1}{N-1}}}  [{\displaystyle {\frac {1}{N-1}}}] becomes smaller.
**** Unbiased sample standard deviation[edit] ****
For unbiased_estimation_of_standard_deviation, there is no formula that works
across all distributions, unlike for mean and variance. Instead, s is used as a
basis, and is scaled by a correction factor to produce an unbiased estimate.
For the normal distribution, an unbiased estimator is given by s/c4, where the
correction factor (which depends on N) is given in terms of the Gamma_function,
and equals:
          c  4   ( N )  =     2  N &#x2212; 1           &#x0393;  (   N 2   )
      &#x0393;  (    N &#x2212; 1  2   )     .   {\displaystyle c_{4}(N)\,=\,
      {\sqrt {\frac {2}{N-1}}}\,\,\,{\frac {\Gamma \left({\frac {N}{2}}\right)}
      {\Gamma \left({\frac {N-1}{2}}\right)}}.}  [c_{4}(N)\,=\,{\sqrt {\frac
      {2}{N-1}}}\,\,\,{\frac {\Gamma \left({\frac {N}{2}}\right)}{\Gamma \left(
      {\frac {N-1}{2}}\right)}}.]
This arises because the sampling distribution of the sample standard deviation
follows a (scaled) chi_distribution, and the correction factor is the mean of
the chi distribution.
An approximation can be given by replacing N â 1 with N â 1.5, yielding:
            &#x03C3; &#x005E;    =     1  N &#x2212; 1.5     &#x2211;  i = 1
      N   (  x  i   &#x2212;    x &#x00AF;     )  2     ,   {\displaystyle
      {\hat {\sigma }}={\sqrt {{\frac {1}{N-1.5}}\sum _{i=1}^{N}(x_{i}-{\bar
      {x}})^{2}}},}  [{\displaystyle {\hat {\sigma }}={\sqrt {{\frac {1}{N-
      1.5}}\sum _{i=1}^{N}(x_{i}-{\bar {x}})^{2}}},}]
The error in this approximation decays quadratically (as 1/N2), and it is
suited for all but the smallest samples or highest precision: for N = 3 the
bias is equal to 1.3%, and for N = 9 the bias is already less than 0.1%. A more
accurate approximation is to replace     N &#x2212; 1.5   {\displaystyle N-1.5}
[{\displaystyle N-1.5}] above with     N &#x2212; 1.5 + 1  /  ( 8 ( N &#x2212;
1 ) )   {\displaystyle N-1.5+1/(8(N-1))}  [{\displaystyle N-1.5+1/(8(N-1))}]
[7].
For other distributions, the correct formula depends on the distribution, but a
rule of thumb is to use the further refinement of the approximation:
            &#x03C3; &#x005E;    =     1  N &#x2212; 1.5 &#x2212;    1 4
      &#x03B3;  2       &#x2211;  i = 1   N   (  x  i   &#x2212;    x &#x00AF;
      )  2     ,   {\displaystyle {\hat {\sigma }}={\sqrt {{\frac {1}{N-1.5-
      {\tfrac {1}{4}}\gamma _{2}}}\sum _{i=1}^{N}(x_{i}-{\bar {x}})^{2}}},}  [
      {\displaystyle {\hat {\sigma }}={\sqrt {{\frac {1}{N-1.5-{\tfrac {1}
      {4}}\gamma _{2}}}\sum _{i=1}^{N}(x_{i}-{\bar {x}})^{2}}},}]
where Î³2 denotes the population excess_kurtosis. The excess kurtosis may be
either known beforehand for certain distributions, or estimated from the data.
[citation_needed]
**** Confidence interval of a sampled standard deviation[edit] ****
See also: Margin_of_error, Variance_Â§ Distribution_of_the_sample_variance, and
Student's_t-distribution_Â§ Robust_parametric_modeling
The standard deviation we obtain by sampling a distribution is itself not
absolutely accurate, both for mathematical reasons (explained here by the
confidence interval) and for practical reasons of measurement (measurement
error). The mathematical effect can be described by the confidence_interval or
CI. To show how a larger sample will make the confidence interval narrower,
consider the following examples: A small population of N = 2 has only 1 degree
of freedom for estimating the standard deviation. The result is that a 95% CI
of the SD runs from 0.45 Ã SD to 31.9 Ã SD; the_factors_here_are_as_follows:
         Pr  (   q   &#x03B1; 2    < k    s  2    &#x03C3;  2     <  q  1
      &#x2212;   &#x03B1; 2      )  = 1 &#x2212; &#x03B1; ,   {\displaystyle
      \Pr \left(q_{\frac {\alpha }{2}}<k{\frac {s^{2}}{\sigma ^{2}}}<q_{1-
      {\frac {\alpha }{2}}}\right)=1-\alpha ,}  [{\displaystyle \Pr \left(q_
      {\frac {\alpha }{2}}<k{\frac {s^{2}}{\sigma ^{2}}}<q_{1-{\frac {\alpha }
      {2}}}\right)=1-\alpha ,}]
where      q  p     {\displaystyle q_{p}}  [{\displaystyle q_{p}}] is the p-th
quantile of the chi-square distribution with k degrees of freedom, and     1
&#x2212; &#x03B1;   {\displaystyle 1-\alpha }  [1-\alpha] is the confidence
level. This is equivalent to the following:
         Pr  (  k    s  2    q  1 &#x2212;   &#x03B1; 2       <  &#x03C3;  2
      < k    s  2    q   &#x03B1; 2       )  = 1 &#x2212; &#x03B1; .
      {\displaystyle \Pr \left(k{\frac {s^{2}}{q_{1-{\frac {\alpha }
      {2}}}}}<\sigma ^{2}<k{\frac {s^{2}}{q_{\frac {\alpha }{2}}}}\right)=1-
      \alpha .}  [{\displaystyle \Pr \left(k{\frac {s^{2}}{q_{1-{\frac {\alpha
      }{2}}}}}<\sigma ^{2}<k{\frac {s^{2}}{q_{\frac {\alpha }{2}}}}\right)=1-
      \alpha .}]
With k = 1,      q  0.025   = 0.000982   {\displaystyle q_{0.025}=0.000982}  [
{\displaystyle q_{0.025}=0.000982}] and      q  0.975   = 5.024
{\displaystyle q_{0.975}=5.024}  [{\displaystyle q_{0.975}=5.024}]. The
reciprocals of the square roots of these two numbers give us the factors 0.45
and 31.9 given above.
A larger population of N = 10 has 9 degrees of freedom for estimating the
standard deviation. The same computations as above give us in this case a 95%
CI running from 0.69 Ã SD to 1.83 Ã SD. So even with a sample population of
10, the actual SD can still be almost a factor 2 higher than the sampled SD.
For a sample population N=100, this is down to 0.88 Ã SD to 1.16 Ã SD. To be
more certain that the sampled SD is close to the actual SD we need to sample a
large number of points.
These same formulae can be used to obtain confidence intervals on the variance
of residuals from a least_squares fit under standard normal theory, where k is
now the number of degrees_of_freedom for error.
**** Bounds on standard deviation[edit] ****
For a set of N > 4 data spanning a range of values R, an upper bound on the
standard deviation s is given by s = 0.6R [8]. An estimate of the standard
deviation for N > 100 data taken to be approximately normal follows from the
heuristic that 95% of the area under the normal curve lies roughly two standard
deviations to either side of the mean, so that, with 95% probability the total
range of values R represents four standard deviations so that s â R/4. This
so-called range rule is useful in sample_size estimation, as the range of
possible values is easier to estimate than the standard deviation. Other
divisors K(N) of the range such that s â R/K(N) are available for other
values of N and for non-normal distributions [9].
***** Identities and mathematical properties[edit] *****
The standard deviation is invariant under changes in location, and scales
directly with the scale of the random variable. Thus, for a constant c and
random variables X and Y:
         &#x03C3; ( c ) = 0    {\displaystyle \sigma (c)=0\,}  [\sigma (c)=0\,]
         &#x03C3; ( X + c ) = &#x03C3; ( X ) ,    {\displaystyle \sigma
      (X+c)=\sigma (X),\,}  [\sigma (X+c)=\sigma (X),\,]
         &#x03C3; ( c X ) =  |  c  |  &#x03C3; ( X ) .    {\displaystyle \sigma
      (cX)=|c|\sigma (X).\,}  [\sigma (cX)=|c|\sigma (X).\,]
The standard deviation of the sum of two random variables can be related to
their individual standard deviations and the covariance between them:
         &#x03C3; ( X + Y ) =   var &#x2061; ( X ) + var &#x2061; ( Y ) + 2
      cov &#x2061; ( X , Y )   .    {\displaystyle \sigma (X+Y)={\sqrt
      {\operatorname {var} (X)+\operatorname {var} (Y)+2\,\operatorname {cov}
      (X,Y)}}.\,}  [\sigma (X+Y)={\sqrt {\operatorname {var} (X)+\operatorname
      {var} (Y)+2\,\operatorname {cov} (X,Y)}}.\,]
where      var  =   &#x03C3;  2      {\displaystyle \textstyle \operatorname
{var} \,=\,\sigma ^{2}}  [{\displaystyle \textstyle \operatorname {var}
\,=\,\sigma ^{2}}] and      cov    {\displaystyle \textstyle \operatorname
{cov} }  [{\displaystyle \textstyle \operatorname {cov} }] stand for variance
and covariance, respectively.
The calculation of the sum of squared deviations can be related to moments
calculated directly from the data. In the following formula, the letter E is
interpreted to mean expected value, i.e., mean.
         &#x03C3; ( X ) =   E &#x2061; [ ( X &#x2212; E &#x2061; [ X ]  )  2
      ]   =   E &#x2061; [  X  2   ] &#x2212; ( E &#x2061; [ X ]  )  2     .
      {\displaystyle \sigma (X)={\sqrt {\operatorname {E} [(X-\operatorname {E}
      [X])^{2}]}}={\sqrt {\operatorname {E} [X^{2}]-(\operatorname {E} [X])^
      {2}}}.}  [{\displaystyle \sigma (X)={\sqrt {\operatorname {E} [(X-
      \operatorname {E} [X])^{2}]}}={\sqrt {\operatorname {E} [X^{2}]-
      (\operatorname {E} [X])^{2}}}.}]
The sample standard deviation can be computed as:
         s ( X ) =    N  N &#x2212; 1       E &#x2061; [ ( X &#x2212; E
      &#x2061; [ X ]  )  2   ]   .   {\displaystyle s(X)={\sqrt {\frac {N}{N-
      1}}}{\sqrt {\operatorname {E} [(X-\operatorname {E} [X])^{2}]}}.}  [
      {\displaystyle s(X)={\sqrt {\frac {N}{N-1}}}{\sqrt {\operatorname {E} [
      (X-\operatorname {E} [X])^{2}]}}.}]
For a finite population with equal probabilities at all points, we have
             1 N    &#x2211;  i = 1   N   (  x  i   &#x2212;   x &#x00AF;    )
      2     =     1 N    (   &#x2211;  i = 1   N    x  i   2    )  &#x2212;
      (   x &#x00AF;    )  2     =    (    1 N    &#x2211;  i = 1   N    x  i
      2    )  &#x2212;   (    1 N    &#x2211;  i = 1   N    x  i    )   2     .
      {\displaystyle {\sqrt {{\frac {1}{N}}\sum _{i=1}^{N}(x_{i}-{\overline
      {x}})^{2}}}={\sqrt {{\frac {1}{N}}\left(\sum _{i=1}^{N}x_{i}^{2}\right)-(
      {\overline {x}})^{2}}}={\sqrt {\left({\frac {1}{N}}\sum _{i=1}^{N}x_{i}^
      {2}\right)-\left({\frac {1}{N}}\sum _{i=1}^{N}x_{i}\right)^{2}}}.}  [
      {\displaystyle {\sqrt {{\frac {1}{N}}\sum _{i=1}^{N}(x_{i}-{\overline
      {x}})^{2}}}={\sqrt {{\frac {1}{N}}\left(\sum _{i=1}^{N}x_{i}^{2}\right)-(
      {\overline {x}})^{2}}}={\sqrt {\left({\frac {1}{N}}\sum _{i=1}^{N}x_{i}^
      {2}\right)-\left({\frac {1}{N}}\sum _{i=1}^{N}x_{i}\right)^{2}}}.}]
This means that the standard deviation is equal to the square root of the
difference between the average of the squares of the values and the square of
the average value. See computational_formula_for_the_variance for proof, and
for an analogous result for the sample standard deviation.
***** Interpretation and application[edit] *****
Further information: Prediction_interval and Confidence_interval
Example of samples from two populations with the same mean but different
standard deviations. Red population has mean 100 and SD 10; blue population has
mean 100 and SD 50.
A large standard deviation indicates that the data points can spread far from
the mean and a small standard deviation indicates that they are clustered
closely around the mean.
For example, each of the three populations {0, 0, 14, 14}, {0, 6, 8, 14} and
{6, 6, 8, 8} has a mean of 7. Their standard deviations are 7, 5, and 1,
respectively. The third population has a much smaller standard deviation than
the other two because its values are all close to 7. It will have the same
units as the data points themselves. If, for instance, the data set {0, 6, 8,
14} represents the ages of a population of four siblings in years, the standard
deviation is 5 years. As another example, the population {1000, 1006, 1008,
1014} may represent the distances traveled by four athletes, measured in
meters. It has a mean of 1007 meters, and a standard deviation of 5 meters.
Standard deviation may serve as a measure of uncertainty. In physical science,
for example, the reported standard deviation of a group of repeated
measurements gives the precision of those measurements. When deciding whether
measurements agree with a theoretical prediction, the standard deviation of
those measurements is of crucial importance: if the mean of the measurements is
too far away from the prediction (with the distance measured in standard
deviations), then the theory being tested probably needs to be revised. This
makes sense since they fall outside the range of values that could reasonably
be expected to occur, if the prediction were correct and the standard deviation
appropriately quantified. See prediction_interval.
While the standard deviation does measure how far typical values tend to be
from the mean, other measures are available. An example is the mean_absolute
deviation, which might be considered a more direct measure of average distance,
compared to the root_mean_square_distance inherent in the standard deviation.
**** Application examples[edit] ****
The practical value of understanding the standard deviation of a set of values
is in appreciating how much variation there is from the average (mean).
*** Experiment, industrial and hypothesis testing[edit] ***
Standard deviation is often used to compare real-world data against a model to
test the model. For example, in industrial applications the weight of products
coming off a production line may need to comply with a legally required value.
By weighing some fraction of the products an average weight can be found, which
will always be slightly different to the long-term average. By using standard
deviations, a minimum and maximum value can be calculated that the averaged
weight will be within some very high percentage of the time (99.9% or more). If
it falls outside the range then the production process may need to be
corrected. Statistical tests such as these are particularly important when the
testing is relatively expensive. For example, if the product needs to be opened
and drained and weighed, or if the product was otherwise used up by the test.
In experimental science, a theoretical model of reality is used. Particle
physics conventionally uses a standard of "5 sigma" for the declaration of a
discovery.[10] A five-sigma level translates to one chance in 3.5 million that
a random fluctuation would yield the result. This level of certainty was
required in order to assert that a particle consistent with the Higgs_boson had
been discovered in two independent experiments at CERN,[11] and this was also
the significance level leading to the declaration of the first_detection_of
gravitational_waves.[12]
*** Weather[edit] ***
As a simple example, consider the average daily maximum temperatures for two
cities, one inland and one on the coast. It is helpful to understand that the
range of daily maximum temperatures for cities near the coast is smaller than
for cities inland. Thus, while these two cities may each have the same average
maximum temperature, the standard deviation of the daily maximum temperature
for the coastal city will be less than that of the inland city as, on any
particular day, the actual maximum temperature is more likely to be farther
from the average maximum temperature for the inland city than for the coastal
one.
*** Finance[edit] ***
In finance, standard deviation is often used as a measure of the risk
associated with price-fluctuations of a given asset (stocks, bonds, property,
etc.), or the risk of a portfolio of assets[13] (actively managed mutual funds,
index mutual funds, or ETFs). Risk is an important factor in determining how to
efficiently manage a portfolio of investments because it determines the
variation in returns on the asset and/or portfolio and gives investors a
mathematical basis for investment decisions (known as mean-variance
optimization). The fundamental concept of risk is that as it increases, the
expected return on an investment should increase as well, an increase known as
the risk premium. In other words, investors should expect a higher return on an
investment when that investment carries a higher level of risk or uncertainty.
When evaluating investments, investors should estimate both the expected return
and the uncertainty of future returns. Standard deviation provides a quantified
estimate of the uncertainty of future returns.
For example, assume an investor had to choose between two stocks. Stock A over
the past 20 years had an average return of 10 percent, with a standard
deviation of 20 percentage_points (pp) and Stock B, over the same period, had
average returns of 12 percent but a higher standard deviation of 30 pp. On the
basis of risk and return, an investor may decide that Stock A is the safer
choice, because Stock B's additional two percentage points of return is not
worth the additional 10 pp standard deviation (greater risk or uncertainty of
the expected return). Stock B is likely to fall short of the initial investment
(but also to exceed the initial investment) more often than Stock A under the
same circumstances, and is estimated to return only two percent more on
average. In this example, Stock A is expected to earn about 10 percent, plus or
minus 20 pp (a range of 30 percent to â10 percent), about two-thirds of the
future year returns. When considering more extreme possible returns or outcomes
in future, an investor should expect results of as much as 10 percent plus or
minus 60 pp, or a range from 70 percent to â50 percent, which includes
outcomes for three standard deviations from the average return (about 99.7
percent of probable returns).
Calculating the average (or arithmetic mean) of the return of a security over a
given period will generate the expected return of the asset. For each period,
subtracting the expected return from the actual return results in the
difference from the mean. Squaring the difference in each period and taking the
average gives the overall variance of the return of the asset. The larger the
variance, the greater risk the security carries. Finding the square root of
this variance will give the standard deviation of the investment tool in
question.
Population standard deviation is used to set the width of Bollinger_Bands, a
widely adopted technical_analysis tool. For example, the upper Bollinger Band
is given as x + nÏx. The most commonly used value for n is 2; there is about a
five percent chance of going outside, assuming a normal distribution of
returns.
Financial time series are known to be non-stationary series, whereas the
statistical calculations above, such as standard deviation, apply only to
stationary series. To apply the above statistical tools to non-stationary
series, the series first must be transformed to a stationary series, enabling
use of statistical tools that now have a valid basis from which to work.
**** Geometric interpretation[edit] ****
To gain some geometric insights and clarification, we will start with a
population of three values, x1, x2, x3. This defines a point P = (x1, x2, x3)
in R3. Consider the line L = {(r, r, r) : r â R}. This is the "main diagonal"
going through the origin. If our three given values were all equal, then the
standard deviation would be zero and P would lie on L. So it is not
unreasonable to assume that the standard deviation is related to the distance
of P to L. That is indeed the case. To move orthogonally from L to the point P,
one begins at the point:
         M = (   x &#x00AF;   ,   x &#x00AF;   ,   x &#x00AF;   )
      {\displaystyle M=({\overline {x}},{\overline {x}},{\overline {x}})}  [M=(
      {\overline {x}},{\overline {x}},{\overline {x}})]
whose coordinates are the mean of the values we started out with.
Derivation of     M = (   x &#x00AF;   ,   x &#x00AF;   ,   x &#x00AF;   )
{\displaystyle M=({\overline {x}},{\overline {x}},{\overline {x}})}  [M=(
{\overline {x}},{\overline {x}},{\overline {x}})]
   M   {\displaystyle M}  [M] is on     L   {\displaystyle L}  [L] therefore
M = ( &#x2113; , &#x2113; , &#x2113; )   {\displaystyle M=(\ell ,\ell ,\ell )}
[{\displaystyle M=(\ell ,\ell ,\ell )}] for some     &#x2113; &#x2208;  R
{\displaystyle \ell \in \mathbb {R} }  [{\displaystyle \ell \in \mathbb {R} }].
The line     L   {\displaystyle L}  [L] is to be orthogonal to the vector from
M   {\displaystyle M}  [M] to     P   {\displaystyle P}  [P]. Therefore:
             L &#x22C5; ( P &#x2212; M )    = 0     ( r , r , r ) &#x22C5; (  x
      1   &#x2212; &#x2113; ,  x  2   &#x2212; &#x2113; ,  x  3   &#x2212;
      &#x2113; )    = 0     r (  x  1   &#x2212; &#x2113; +  x  2   &#x2212;
      &#x2113; +  x  3   &#x2212; &#x2113; )    = 0     r  (   &#x2211;  i    x
      i   &#x2212; 3 &#x2113;  )     = 0      &#x2211;  i    x  i   &#x2212; 3
      &#x2113;    = 0       1 3    &#x2211;  i    x  i      = &#x2113;       x
      &#x00AF;      = &#x2113;       {\displaystyle {\begin{aligned}L\cdot (P-
      M)&=0\\[4pt](r,r,r)\cdot (x_{1}-\ell ,x_{2}-\ell ,x_{3}-\ell )&=0\\[4pt]r
      (x_{1}-\ell +x_{2}-\ell +x_{3}-\ell )&=0\\[4pt]r\left(\sum _{i}x_{i}-
      3\ell \right)&=0\\[4pt]\sum _{i}x_{i}-3\ell &=0\\[4pt]{\frac {1}{3}}\sum
      _{i}x_{i}&=\ell \\[4pt]{\overline {x}}&=\ell \end{aligned}}}  [
      {\displaystyle {\begin{aligned}L\cdot (P-M)&=0\\[4pt](r,r,r)\cdot (x_{1}-
      \ell ,x_{2}-\ell ,x_{3}-\ell )&=0\\[4pt]r(x_{1}-\ell +x_{2}-\ell +x_{3}-
      \ell )&=0\\[4pt]r\left(\sum _{i}x_{i}-3\ell \right)&=0\\[4pt]\sum _{i}x_
      {i}-3\ell &=0\\[4pt]{\frac {1}{3}}\sum _{i}x_{i}&=\ell \\[4pt]{\overline
      {x}}&=\ell \end{aligned}}}]
A little algebra shows that the distance between P and M (which is the same as
the orthogonal distance between P and the line L)        &#x2211;  i   (  x  i
&#x2212;   x &#x00AF;    )  2       {\displaystyle {\sqrt {\sum \limits _{i}(x_
{i}-{\overline {x}})^{2}}}}  [{\sqrt {\sum \limits _{i}(x_{i}-{\overline {x}})^
{2}}}] is equal to the standard deviation of the vector (x1, x2, x3),
multiplied by the square root of the number of dimensions of the vector (3 in
this case).
**** Chebyshev's inequality[edit] ****
Main article: Chebyshev's_inequality
An observation is rarely more than a few standard deviations away from the
mean. Chebyshev's inequality ensures that, for all distributions for which the
standard deviation is defined, the amount of data within a number of standard
deviations of the mean is at least as much as given in the following table.
Distance from mean                      Minimum population
     2    &#x03C3;   {\displaystyle
{\sqrt {2}}\,\sigma }  [{\displaystyle  50%
{\sqrt {2}}\,\sigma }]
2Ï                                   75%
3Ï                                   89%
4Ï                                   94%
5Ï                                   96%
6Ï                                   97%
                                           1 &#x2212;   1  k  2
   k &#x03C3;   {\displaystyle k\sigma  {\displaystyle 1-{\frac {1}{k^{2}}}}  [
}  [k\sigma ]                           {\displaystyle 1-{\frac {1}{k^{2}}}}]
                                        [14]
     1  1 &#x2212; &#x2113;
&#x03C3;   {\displaystyle {\frac {1}       &#x2113;   {\displaystyle \ell }
{\sqrt {1-\ell }}}\,\sigma }  [         [\ell ]
{\displaystyle {\frac {1}{\sqrt {1-\ell
}}}\,\sigma }]
**** Rules for normally distributed data[edit] ****
Dark blue is one standard deviation on either side of the mean. For the normal
distribution, this accounts for 68.27 percent of the set; while two standard
deviations from the mean (medium and dark blue) account for 95.45 percent;
three standard deviations (light, medium, and dark blue) account for 99.73
percent; and four standard deviations account for 99.994 percent. The two
points of the curve that are one standard deviation from the mean are also the
inflection_points.
The central_limit_theorem states that the distribution of an average of many
independent, identically distributed random variables tends toward the famous
bell-shaped normal distribution with a probability_density_function of
         f ( x ; &#x03BC; ,  &#x03C3;  2   ) =   1  &#x03C3;   2 &#x03C0;
      e  &#x2212;   1 2     (    x &#x2212; &#x03BC;  &#x03C3;   )   2
      {\displaystyle f(x;\mu ,\sigma ^{2})={\frac {1}{\sigma {\sqrt {2\pi
      }}}}e^{-{\frac {1}{2}}\left({\frac {x-\mu }{\sigma }}\right)^{2}}}  [f
      (x;\mu ,\sigma ^{2})={\frac {1}{\sigma {\sqrt {2\pi }}}}e^{-{\frac {1}
      {2}}\left({\frac {x-\mu }{\sigma }}\right)^{2}}]
where Î¼ is the expected_value of the random variables, Ï equals their
distribution's standard deviation divided by n1/2, and n is the number of
random variables. The standard deviation therefore is simply a scaling variable
that adjusts how broad the curve will be, though it also appears in the
normalizing_constant.
If a data distribution is approximately normal, then the proportion of data
values within z standard deviations of the mean is defined by:
          Proportion  = erf &#x2061;  (   z  2    )    {\displaystyle {\text
      {Proportion}}=\operatorname {erf} \left({\frac {z}{\sqrt {2}}}\right)}  [
      {\displaystyle {\text{Proportion}}=\operatorname {erf} \left({\frac {z}
      {\sqrt {2}}}\right)}]
where      erf    {\displaystyle \textstyle \operatorname {erf} }  [
{\displaystyle \textstyle \operatorname {erf} }] is the error_function. The
proportion that is less than or equal to a number, x, is given by the
cumulative_distribution_function:
          Proportion  &#x2264; x =   1 2    [  1 + erf &#x2061;  (    x
      &#x2212; &#x03BC;   &#x03C3;   2      )   ]  =   1 2    [  1 + erf
      &#x2061;  (   z  2    )   ]    {\displaystyle {\text{Proportion}}\leq x=
      {\frac {1}{2}}\left[1+\operatorname {erf} \left({\frac {x-\mu }{\sigma
      {\sqrt {2}}}}\right)\right]={\frac {1}{2}}\left[1+\operatorname {erf}
      \left({\frac {z}{\sqrt {2}}}\right)\right]}  [{\displaystyle {\text
      {Proportion}}\leq x={\frac {1}{2}}\left[1+\operatorname {erf} \left(
      {\frac {x-\mu }{\sigma {\sqrt {2}}}}\right)\right]={\frac {1}{2}}\left
      [1+\operatorname {erf} \left({\frac {z}{\sqrt {2}}}\right)\right]}].[15]
If a data distribution is approximately normal then about 68 percent of the
data values are within one standard deviation of the mean (mathematically,
Î¼ Â± Ï, where Î¼ is the arithmetic mean), about 95 percent are within two
standard deviations (Î¼ Â± 2Ï), and about 99.7 percent lie within three
standard deviations (Î¼ Â± 3Ï). This is known as the 68-95-99.7_rule, or the
empirical rule.
For various values of z, the percentage of values expected to lie in and
outside the symmetric interval, CI = (âzÏ, zÏ), are as follows:
Percentage within(z)
z(Percentage within)
Confidence  Proportion within Proportion without
interval    Percentage        Percentage       Fraction
0.318 639Ï�25%               75%              3 / 4
0.674490Ï50%               50%              1 / 2
0.994458Ï68%               32%              1 / 3.125
1Ï       68.2689492%       31.7310508%      1 / 3.1514872
1.281552Ï80%               20%              1 / 5
1.644854Ï90%               10%              1 / 10
1.959964Ï95%               5%               1 / 20
2Ï       95.4499736%       4.5500264%       1 / 21.977895
2.575829Ï99%               1%               1 / 100
3Ï       99.7300204%       0.2699796%       1 / 370.398
3.290527Ï99.9%             0.1%             1 / 1000
3.890592Ï99.99%            0.01%            1 / 10000
4Ï       99.993666%        0.006334%        1 / 15787
4.417173Ï99.999%           0.001%           1 / 100000
                                               1 / 147159.5358
4.5Ï     99.9993204653751% 0.0006795346249% 3.4 / 1000000 (on each side of
                                               mean)
4.891638Ï99.9999%          0.0001%          1 / 1000000
5Ï       99.9999426697%    0.0000573303%    1 / 1744278
5.326724Ï99.99999%         0.00001%         1 / 10000000
5.730729Ï99.999999%        0.000001%        1 / 100000000
6Ï       99.9999998027%    0.0000001973%    1 / 506797346
6.109410Ï99.9999999%       0.0000001%       1 / 1000000000
6.466951Ï99.99999999%      0.00000001%      1 / 10000000000
6.806502Ï99.999999999%     0.000000001%     1 / 100000000000
7Ï       99.9999999997440% 0.000000000256%  1 / 390682215445
***** Relationship between standard deviation and mean[edit] *****
The mean and the standard deviation of a set of data are descriptive_statistics
usually reported together. In a certain sense, the standard deviation is a
"natural" measure of statistical_dispersion if the center of the data is
measured about the mean. This is because the standard deviation from the mean
is smaller than from any other point. The precise statement is the following:
suppose x1, ..., xn are real numbers and define the function:
         &#x03C3; ( r ) =     1  N &#x2212; 1     &#x2211;  i = 1   N   (  x  i
      &#x2212; r  )  2     .   {\displaystyle \sigma (r)={\sqrt {{\frac {1}{N-
      1}}\sum _{i=1}^{N}(x_{i}-r)^{2}}}.}  [\sigma (r)={\sqrt {{\frac {1}{N-
      1}}\sum _{i=1}^{N}(x_{i}-r)^{2}}}.]
Using calculus or by completing_the_square, it is possible to show that Ï(r)
has a unique minimum at the mean:
         r =   x &#x00AF;   .    {\displaystyle r={\overline {x}}.\,}  [r=
      {\overline {x}}.\,]
Variability can also be measured by the coefficient_of_variation, which is the
ratio of the standard deviation to the mean. It is a dimensionless_number.
**** Standard deviation of the mean[edit] ****
Main article: Standard_error_of_the_mean
Often, we want some information about the precision of the mean we obtained. We
can obtain this by determining the standard deviation of the sampled mean.
Assuming statistical independence of the values in the sample, the standard
deviation of the mean is related to the standard deviation of the distribution
by:
          &#x03C3;  mean   =   1  N    &#x03C3;   {\displaystyle \sigma _{\text
      {mean}}={\frac {1}{\sqrt {N}}}\sigma }  [\sigma _{\text{mean}}={\frac {1}
      {\sqrt {N}}}\sigma ]
where N is the number of observations in the sample used to estimate the mean.
This can easily be proven with (see basic_properties_of_the_variance):
             var &#x2061; ( X )    &#x2261;  &#x03C3;  X   2       var &#x2061;
      (  X  1   +  X  2   )    &#x2261; var &#x2061; (  X  1   ) + var &#x2061;
      (  X  2   )       {\displaystyle {\begin{aligned}\operatorname {var}
      (X)&\equiv \sigma _{X}^{2}\\\operatorname {var} (X_{1}+X_{2})&\equiv
      \operatorname {var} (X_{1})+\operatorname {var} (X_{2})\\\end{aligned}}}
      [{\displaystyle {\begin{aligned}\operatorname {var} (X)&\equiv \sigma _
      {X}^{2}\\\operatorname {var} (X_{1}+X_{2})&\equiv \operatorname {var} (X_
      {1})+\operatorname {var} (X_{2})\\\end{aligned}}}]
(Statistical Independence is assumed.)
             var &#x2061; ( c  X  1   )    &#x2261;  c  2    var &#x2061; (  X
      1   )       {\displaystyle {\begin{aligned}\operatorname {var} (cX_
      {1})&\equiv c^{2}\,\operatorname {var} (X_{1})\end{aligned}}}  [
      {\displaystyle {\begin{aligned}\operatorname {var} (cX_{1})&\equiv c^
      {2}\,\operatorname {var} (X_{1})\end{aligned}}}]
hence
             var &#x2061; (  mean  )    = var &#x2061;  (    1 N    &#x2211;  i
      = 1   N    X  i    )  =   1  N  2     var &#x2061;  (   &#x2211;  i = 1
      N    X  i    )        =   1  N  2      &#x2211;  i = 1   N   var &#x2061;
      (  X  i   ) =   N  N  2     var &#x2061; ( X ) =   1 N   var &#x2061; ( X
      ) .       {\displaystyle {\begin{aligned}\operatorname {var} ({\text
      {mean}})&=\operatorname {var} \left({\frac {1}{N}}\sum _{i=1}^{N}X_
      {i}\right)={\frac {1}{N^{2}}}\operatorname {var} \left(\sum _{i=1}^{N}X_
      {i}\right)\\&={\frac {1}{N^{2}}}\sum _{i=1}^{N}\operatorname {var} (X_
      {i})={\frac {N}{N^{2}}}\operatorname {var} (X)={\frac {1}
      {N}}\operatorname {var} (X).\end{aligned}}}  [{\begin
      {aligned}\operatorname {var} ({\text{mean}})&=\operatorname {var} \left(
      {\frac {1}{N}}\sum _{i=1}^{N}X_{i}\right)={\frac {1}{N^{2}}}\operatorname
      {var} \left(\sum _{i=1}^{N}X_{i}\right)\\&={\frac {1}{N^{2}}}\sum _{i=1}^
      {N}\operatorname {var} (X_{i})={\frac {N}{N^{2}}}\operatorname {var} (X)=
      {\frac {1}{N}}\operatorname {var} (X).\end{aligned}}]
Resulting in:
          &#x03C3;  mean   =   &#x03C3;  N    .   {\displaystyle \sigma _{\text
      {mean}}={\frac {\sigma }{\sqrt {N}}}.}  [\sigma _{\text{mean}}={\frac
      {\sigma }{\sqrt {N}}}.]
It should be emphasized that in order to estimate the standard deviation of the
mean      &#x03C3;  mean     {\displaystyle \sigma _{\text{mean}}}  [\sigma _
{\text{mean}}] it is necessary to know the standard deviation of the entire
population     &#x03C3;   {\displaystyle \sigma }  [\sigma ] beforehand.
However, in most applications this parameter is unknown. For example, if a
series of 10 measurements of a previously unknown quantity is performed in a
laboratory, it is possible to calculate the resulting sample mean and sample
standard deviation, but it is impossible to calculate the standard deviation of
the mean.
***** Rapid calculation methods[edit] *****
See also: Algorithms_for_calculating_variance
The following two formulas can represent a running (repeatedly updated)
standard deviation. A set of two power sums s1 and s2 are computed over a set
of N values of x, denoted as x1, ..., xN:
         &#xA0;  s  j   =  &#x2211;  k = 1   N     x  k   j    .
      {\displaystyle \ s_{j}=\sum _{k=1}^{N}{x_{k}^{j}}.}  [\ s_{j}=\sum _
      {k=1}^{N}{x_{k}^{j}}.]
Given the results of these running summations, the values N, s1, s2 can be used
at any time to compute the current value of the running standard deviation:
         &#x03C3; =    N  s  2   &#x2212;  s  1   2    N     {\displaystyle
      \sigma ={\frac {\sqrt {Ns_{2}-s_{1}^{2}}}{N}}}  [\sigma ={\frac {\sqrt
      {Ns_{2}-s_{1}^{2}}}{N}}]
Where N, as mentioned above, is the size of the set of values (or can also be
regarded as s0).
Similarly for sample standard deviation,
         s =     N  s  2   &#x2212;  s  1   2     N ( N &#x2212; 1 )     .
      {\displaystyle s={\sqrt {\frac {Ns_{2}-s_{1}^{2}}{N(N-1)}}}.}  [s={\sqrt
      {\frac {Ns_{2}-s_{1}^{2}}{N(N-1)}}}.]
In a computer implementation, as the three sj sums become large, we need to
consider round-off_error, arithmetic_overflow, and arithmetic_underflow. The
method below calculates the running sums method with reduced rounding errors.
[16] This is a "one pass" algorithm for calculating variance of n samples
without the need to store prior data during the calculation. Applying this
method to a time series will result in successive values of standard deviation
corresponding to n data points as n grows larger with each new sample, rather
than a constant-width sliding window calculation.
For k = 1, ..., n:
              A  0      = 0      A  k      =  A  k &#x2212; 1   +     x  k
      &#x2212;  A  k &#x2212; 1    k         {\displaystyle {\begin{aligned}A_
      {0}&=0\\A_{k}&=A_{k-1}+{\frac {x_{k}-A_{k-1}}{k}}\end{aligned}}}  [
      {\begin{aligned}A_{0}&=0\\A_{k}&=A_{k-1}+{\frac {x_{k}-A_{k-1}}{k}}\end
      {aligned}}]
where A is the mean value.
              Q  0      = 0      Q  k      =  Q  k &#x2212; 1   +    k &#x2212;
      1  k   (  x  k   &#x2212;  A  k &#x2212; 1    )  2   =  Q  k &#x2212; 1
      + (  x  k   &#x2212;  A  k &#x2212; 1   ) (  x  k   &#x2212;  A  k   )
      {\displaystyle {\begin{aligned}Q_{0}&=0\\Q_{k}&=Q_{k-1}+{\frac {k-1}{k}}
      (x_{k}-A_{k-1})^{2}=Q_{k-1}+(x_{k}-A_{k-1})(x_{k}-A_{k})\\\end{aligned}}}
      [{\begin{aligned}Q_{0}&=0\\Q_{k}&=Q_{k-1}+{\frac {k-1}{k}}(x_{k}-A_{k-
      1})^{2}=Q_{k-1}+(x_{k}-A_{k-1})(x_{k}-A_{k})\\\end{aligned}}]
Note:      Q  1   = 0   {\displaystyle Q_{1}=0}  [Q_{1}=0] since     k &#x2212;
1 = 0   {\displaystyle k-1=0}  [k-1=0] or      x  1   =  A  1
{\displaystyle x_{1}=A_{1}}  [x_{1}=A_{1}]
Sample variance:
          s  n   2   =    Q  n    n &#x2212; 1      {\displaystyle s_{n}^{2}=
      {\frac {Q_{n}}{n-1}}}  [s_{n}^{2}={\frac {Q_{n}}{n-1}}]
Population variance:
          &#x03C3;  n   2   =    Q  n   n     {\displaystyle \sigma _{n}^{2}=
      {\frac {Q_{n}}{n}}}  [\sigma _{n}^{2}={\frac {Q_{n}}{n}}]
**** Weighted calculation[edit] ****
When the values xi are weighted with unequal weights wi, the power sums s0, s1,
s2 are each computed as:
         &#xA0;  s  j   =  &#x2211;  k = 1   N    w  k    x  k   j   .
      {\displaystyle \ s_{j}=\sum _{k=1}^{N}w_{k}x_{k}^{j}.\,}  [{\displaystyle
      \ s_{j}=\sum _{k=1}^{N}w_{k}x_{k}^{j}.\,}]
And the standard deviation equations remain unchanged. s0 is now the sum of the
weights and not the number of samples N.
The incremental method with reduced rounding errors can also be applied, with
some additional complexity.
A running sum of weights must be computed for each k from 1 to n:
              W  0      = 0      W  k      =  W  k &#x2212; 1   +  w  k
      {\displaystyle {\begin{aligned}W_{0}&=0\\W_{k}&=W_{k-1}+w_{k}\end
      {aligned}}}  [{\begin{aligned}W_{0}&=0\\W_{k}&=W_{k-1}+w_{k}\end
      {aligned}}]
and places where 1/n is used above must be replaced by wi/Wn:
              A  0      = 0      A  k      =  A  k &#x2212; 1   +    w  k    W
      k     (  x  k   &#x2212;  A  k &#x2212; 1   )      Q  0      = 0      Q
      k      =  Q  k &#x2212; 1   +     w  k    W  k &#x2212; 1     W  k
      (  x  k   &#x2212;  A  k &#x2212; 1    )  2   =  Q  k &#x2212; 1   +  w
      k   (  x  k   &#x2212;  A  k &#x2212; 1   ) (  x  k   &#x2212;  A  k   )
      {\displaystyle {\begin{aligned}A_{0}&=0\\A_{k}&=A_{k-1}+{\frac {w_{k}}{W_
      {k}}}(x_{k}-A_{k-1})\\Q_{0}&=0\\Q_{k}&=Q_{k-1}+{\frac {w_{k}W_{k-1}}{W_
      {k}}}(x_{k}-A_{k-1})^{2}=Q_{k-1}+w_{k}(x_{k}-A_{k-1})(x_{k}-A_{k})\end
      {aligned}}}  [{\begin{aligned}A_{0}&=0\\A_{k}&=A_{k-1}+{\frac {w_{k}}{W_
      {k}}}(x_{k}-A_{k-1})\\Q_{0}&=0\\Q_{k}&=Q_{k-1}+{\frac {w_{k}W_{k-1}}{W_
      {k}}}(x_{k}-A_{k-1})^{2}=Q_{k-1}+w_{k}(x_{k}-A_{k-1})(x_{k}-A_{k})\end
      {aligned}}]
In the final division,
          &#x03C3;  n   2   =    Q  n    W  n        {\displaystyle \sigma _
      {n}^{2}={\frac {Q_{n}}{W_{n}}}\,}  [\sigma _{n}^{2}={\frac {Q_{n}}{W_
      {n}}}\,]
and
          s  n   2   =    Q  n     W  n   &#x2212; 1    ,   {\displaystyle s_
      {n}^{2}={\frac {Q_{n}}{W_{n}-1}},}  [{\displaystyle s_{n}^{2}={\frac {Q_
      {n}}{W_{n}-1}},}]
or
          s  n   2   =    n &#x2032;    n &#x2032;  &#x2212; 1     &#x03C3;  n
      2   ,   {\displaystyle s_{n}^{2}={\frac {n'}{n'-1}}\sigma _{n}^{2},}  [
      {\displaystyle s_{n}^{2}={\frac {n'}{n'-1}}\sigma _{n}^{2},}]
where n is the total number of elements, and n' is the number of elements with
non-zero weights. The above formulas become equal to the simpler formulas given
above if weights are taken as equal to one.
***** History[edit] *****
The term standard deviation was first used[17] in writing by Karl_Pearson[18]
in 1894, following his use of it in lectures. This was as a replacement for
earlier alternative names for the same idea: for example, Gauss used mean
error.[19]
***** See also[edit] *****
    * [icon]Statistics_portal
    * 68â95â99.7_rule
    * Accuracy_and_precision
    * Chebyshev's_inequality An inequality on location and scale parameters
    * Cumulant
    * Deviation_(statistics)
    * Distance_correlation Distance standard deviation
    * Error_bar
    * Geometric_standard_deviation
    * Mahalanobis_distance generalizing number of standard deviations to the
      mean
    * Mean_absolute_error
    * Pooled_standard_deviation
    * Propagation_of_uncertainty
    * Percentile
    * Raw_score
    * Relative_standard_deviation
    * Robust_standard_deviation
    * Root_mean_square
    * Sample_size
    * Samuelson's_inequality
    * Six_Sigma
    * Standard_error
    * Standard_score
    * Volatility_(finance)
    * Yamartino_method for calculating standard deviation of wind direction
***** References[edit] *****
   1. ^Bland, J.M.; Altman, D.G. (1996). "Statistics_notes:_measurement_error".
      BMJ. 312 (7047): 1654. doi:10.1136/bmj.312.7047.1654. PMC 2351401.
      PMID 8664723.
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
   3. ^Gauss,_Carl_Friedrich (1816). "Bestimmung der Genauigkeit der
      Beobachtungen". Zeitschrift fÃ¼r Astronomie und Verwandte Wissenschaften.
      1: 187â197.
   4. ^Walker, Helen (1931). Studies in the History of the Statistical Method.
      Baltimore, MD: Williams & Wilkins Co. pp. 24â25.
   5. ^Logan, Murray (2010), Biostatistical_Design_and_Analysis_Using_R (First
      ed.), Wiley-Blackwell
   6. ^Furness, R.W.; Bryant, D.M. (1996). "Effect of wind on field metabolic
      rates of breeding northern fulmars". Ecology. 77 (4): 1181â1188. doi:
      10.2307/2265587. JSTOR 2265587.
   7. ^Weisstein,_Eric_W. "Bessel's_Correction". MathWorld.
   8. ^Gurland, John; Tripathi, Ram C. (1971), "A Simple Approximation for
      Unbiased Estimation of the Standard Deviation", The American
      Statistician, 25 (4): 30â32, doi:10.2307/2682923, JSTOR 2682923
   9. ^Shiffler, Ronald E.; Harsha, Phillip D. (1980). "Upper and Lower Bounds
      for the Sample Standard Deviation". Teaching Statistics. 2 (3): 84â86.
      doi:10.1111/j.1467-9639.1980.tb00398.x.
  10. ^Browne, Richard H. (2001). "Using the Sample Range as a Basis for
      Calculating Sample Size in Power Calculations". The American
      Statistician. 55 (4): 293â298. doi:10.1198/000313001753272420.
      JSTOR 2685690.
  11. ^"What_does_the_5_sigma_mean?". Physics.org. Retrieved 5 February 2019.
  12. ^"CERN_experiments_observe_particle_consistent_with_long-sought_Higgs
      boson_|_CERN_press_office". Press.web.cern.ch. 4 July 2012. Retrieved 30
      May 2015.
  13. ^LIGO Scientific Collaboration, Virgo Collaboration (2016), "Observation
      of Gravitational Waves from a Binary Black Hole Merger", Physical Review
      Letters, 116 (6): 061102, arXiv:1602.03837, Bibcode:2016PhRvL.116f1102A,
      doi:10.1103/PhysRevLett.116.061102, PMID 26918975
  14. ^"What_is_Standard_Deviation". Pristine. Retrieved 29 October 2011.
  15. ^Ghahramani, Saeed (2000). Fundamentals of Probability (2nd ed.). New
      Jersey: Prentice Hall. p. 438.
  16. ^Eric W. Weisstein. "Distribution_Function". MathWorldâA Wolfram Web
      Resource. Retrieved 30 September 2014.
  17. ^Welford, BP (August 1962). "Note on a Method for Calculating Corrected
      Sums of Squares and Products". Technometrics. 4 (3): 419â420.
      CiteSeerX 10.1.1.302.7503. doi:10.1080/00401706.1962.10490022.
  18. ^Dodge, Yadolah (2003). The Oxford Dictionary of Statistical Terms.
      Oxford University Press. ISBN 978-0-19-920613-1.
  19. ^Pearson,_Karl (1894). "On the dissection of asymmetrical frequency
      curves". Philosophical_Transactions_of_the_Royal_Society_A. 185:
      71â110. Bibcode:1894RSPTA.185...71P. doi:10.1098/rsta.1894.0003.
  20. ^Miller, Jeff. "Earliest_Known_Uses_of_Some_of_the_Words_of_Mathematics".
***** External links[edit] *****
 Wikimedia Commons has media related to Standard_deviation.
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Quadratic_deviation",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
A_simple_way_to_understand_Standard_Deviation
Standard_Deviation â_an_explanation_without_maths

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
                               * Standard deviation
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
    * v
    * t
    * e
Technical_analysis
               * Breakout
               * Dead_cat_bounce
Concepts       * Dow_theory
               * Elliott_wave_principle
               * Market_trend
               * Candlestick
               * Renko
Charts         * Kagi
               * Line
               * Open-high-low-close
               * Point_and_figure
                           * Broadening_top
                           * Cup_and_handle
                           * Double_top_and_double_bottom
                           * Flag_and_pennant
                           * Gap
           Chart           * Head_and_shoulders
                           * Island_reversal
                           * Price_channels
                           * Triangle
                           * Triple_top_and_triple_bottom
Patterns                   * Wedge_pattern
                                   * Doji
                                   * Hammer
                                   * Hanging_man
                       Simple      * Inverted_hammer
                                   * Marubozu
           Candlestick             * Shooting_star
                                   * Spinning_top
                                   * Hikkake_pattern
                       Complex     * Morning_star
                                   * Three_black_crows
                                   * Three_white_soldiers
                          * Bottom
           Support_&      * Fibonacci_retracement
           resistance     * Pivot_point (PP)
                          * Top
                          * Average_directional_index (A.D.X.)
                          * Commodity_channel_index (CCI)
                          * Detrended_price_oscillator (DPO)
                          * Know_sure_thing_oscillator (KST)
                          * Ichimoku_KinkÅ_HyÅ
                          * Moving_average_convergence/divergence (MACD)
           Trend          * Mass_index
                          * Moving_average (MA)
                          * Parabolic_SAR (SAR)
                          * Smart_money_index (SMI)
                          * Trend_line
                          * Trix
                          * Vortex_indicator (VI)
                          * Money_flow_index (MFI)
                          * Relative_strength_index (RSI)
           Momentum       * Stochastic_oscillator
Indicators                * True_strength_index (TSI)
                          * Ultimate_oscillator
                          * Williams_%R (%R)
                          * Accumulation/distribution_line
                          * Ease_of_movement (EMV)
                          * Force_index (FI)
           Volume         * Negative_volume_index (NVI)
                          * On-balance_volume (OBV)
                          * Put/call_ratio (PCR)
                          * Volumeâprice_trend (VPT)
                          * Average_true_range (ATR)
                          * Bollinger_Bands (BB)
           Volatility     * Donchian_channel
                          * Keltner_channel
                          * CBOE_Market_Volatility_Index (VIX)
                          * Standard deviation (Ï)
                          * Advanceâdecline_line (ADL)
           Breadth        * Arms_index (TRIN)
                          * McClellan_oscillator
           Other          * Coppock_curve
                          * Ulcer_index
Authority_control [Edit_this_at_Wikidata]     * GND: 4767332-1
                                              * LCCN: sh85127303

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Standard_deviation&oldid=909718347"
Categories:
    * Statistical_deviation_and_dispersion
    * Summary_statistics
Hidden categories:
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_July_2012
    * Articles_with_unsourced_statements_from_January_2012
    * Articles_with_unsourced_statements_from_August_2017
    * Use_dmy_dates_from_June_2011
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
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
    * Wikibooks
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
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
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Latina
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
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
    * Shqip
    * Sicilianu
    * à·à·à¶à·à¶½
    * Simple_English
    * Ø³ÙÚÙ
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Basa_Sunda
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * Winaray
    * å´è¯­
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 04:44 (UTC).
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
