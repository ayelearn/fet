The following text has been accessed from https://en.wikipedia.org/wiki/Median at Fri Aug 9 01:25:10 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Median ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the statistical concept. For other uses, see Median_
(disambiguation).
Finding the median in sets of data with an odd and even number of values
The median is the value separating the higher half from the lower half of a
data sample (a population or a probability_distribution). For a data set, it
may be thought of as the "middle" value. For example, in the data set {1, 3, 3,
6, 7, 8, 9}, the median is 6, the fourth largest, and also the fourth smallest,
number in the sample. For a continuous_probability_distribution, the median is
the value such that a number is equally likely to fall above or below it.
The median is a commonly used measure of the properties of a data set in
statistics and probability_theory. The basic advantage of the median in
describing data compared to the mean (often simply described as the "average")
is that it is not skewed so much by a small proportion of extremely large or
small values, and so it may give a better idea of a "typical" value. For
example, in understanding statistics like household income or assets, which
vary greatly, the mean may be skewed by a small number of extremely high or low
values. Median income, for example, may be a better way to suggest what a
"typical" income is.
Because of this, the median is of central importance in robust_statistics, as
it is the most resistant_statistic, having a breakdown_point of 50%: so long as
no more than half the data are contaminated, the median will not give an
arbitrarily large or small result.
⁰
***** Contents *****
    * 1_Finite_set_of_numbers
    * 2_Probability_distributions
          o 2.1_Medians_of_particular_distributions
    * 3_Populations
          o 3.1_Optimality_property
          o 3.2_Unimodal_distributions
          o 3.3_Inequality_relating_means_and_medians
    * 4_Jensen's_inequality_for_medians
    * 5_Medians_for_samples
          o 5.1_The_sample_median
                # 5.1.1_Efficient_computation_of_the_sample_median
                # 5.1.2_Easy_explanation_of_the_sample_median
                # 5.1.3_Sampling_distribution
          o 5.2_Other_estimators
          o 5.3_Coefficient_of_dispersion
    * 6_Multivariate_median
          o 6.1_Marginal_median
          o 6.2_Centerpoint
    * 7_Other_median-related_concepts
          o 7.1_Interpolated_median
          o 7.2_Pseudo-median
          o 7.3_Variants_of_regression
          o 7.4_Median_filter
          o 7.5_Cluster_analysis
          o 7.6_Medianâmedian_line
    * 8_Median-unbiased_estimators
    * 9_History
    * 10_See_also
    * 11_References
    * 12_External_links
***** Finite set of numbers[edit] *****
The median of a finite list of numbers can be found by arranging all the
numbers from smallest to greatest.
If there is an odd number of numbers, the middle one is picked. For example,
consider the list of numbers
      1, 3, 3, 6, 7, 8, 9
This list contains seven numbers. The median is the fourth of them, which is 6.
If there is an even number of observations, then there is no single middle
value; the median is then usually defined to be the mean of the two middle
values.[1][2] For example, in the data set
      1, 2, 3, 4, 5, 6, 8, 9
the median is the mean of the middle two numbers: this is     ( 4 + 5 )  /  2
{\displaystyle (4+5)/2}  [{\displaystyle (4+5)/2}], which is     4.5
{\displaystyle 4.5}  [{\displaystyle 4.5}]. (In more technical terms, this
interprets the median as the fully trimmed mid-range).
The formula used to find the index of the middle number of a data set of n
numerically ordered numbers is     ( n + 1 )  /  2   {\displaystyle (n+1)/2}  [
{\displaystyle (n+1)/2}]. This either gives the middle number (for an odd
number of values) or the halfway point between the two middle values. For
example, with 14 values, the formula will give an index of 7.5, and the median
will be taken by averaging the seventh (the floor of this index) and eighth
(the ceiling of this index) values. So the median can be represented by the
following formula:
          m e d i a n  ( a ) =     a  &#x230A; ( &#x0023; x + 1 ) &#x00F7; 2
      &#x230B;   +  a  &#x2308; ( &#x0023; x + 1 ) &#x00F7; 2 &#x2309;    2
      {\displaystyle \mathrm {median} (a)={\frac {a_{\lfloor (\#x+1)\div
      2\rfloor }+a_{\lceil (\#x+1)\div 2\rceil }}{2}}}  [{\displaystyle \mathrm
      {median} (a)={\frac {a_{\lfloor (\#x+1)\div 2\rfloor }+a_{\lceil
      (\#x+1)\div 2\rceil }}{2}}}]
        Comparison of common averages of values { 1, 2, 2, 3, 4, 7, 9 }
Type            Description                          Example             Result
                Sum of values of a data set divided
                by number of values:         x
                &#x00AF;    =   1 n    &#x2211;  i =
Arithmetic_mean 1   n    x  i      {\displaystyle    (1+2+2+3+4+7+9) / 7    4
                \scriptstyle {\bar {x}}={\frac {1}
                {n}}\sum _{i=1}^{n}x_{i}}
                [\scriptstyle {\bar  {x}}={\frac
                {1}{n}}\sum _{{i=1}}^{n}x_{i}]
      Median    Middle value separating the greater  1, 2, 2, 3, 4, 7, 9    3
                and lesser halves of a data set
        Mode    Most frequent value in a data set    1, 2, 2, 3, 4, 7, 9    2
One can find the median using the Stem-and-Leaf_Plot.
There is no widely accepted standard notation for the median, but some authors
represent the median of a variable x either as xÍ or as Î¼1/2[1] sometimes
also M.[3][4] In any of these cases, the use of these or other symbols for the
median needs to be explicitly defined when they are introduced.
The median is used primarily for skewed distributions, which it summarizes
differently from the arithmetic_mean. Consider the multiset { 1, 2, 2, 2, 3, 14
}. The median is 2 in this case, (as is the mode), and it might be seen as a
better indication of central_tendency (less susceptible to the exceptionally
large value in data) than the arithmetic_mean of 4.
The median is a popular summary_statistic used in descriptive_statistics, since
it is simple to understand and easy to calculate, while also giving a measure
that is more robust in the presence of outlier values than is the mean. The
widely cited empirical relationship between the relative locations of the mean
and the median for skewed distributions is, however, not generally true.[5]
There are, however, various relationships for the absolute difference between
them; see below.
With an even number of observations (as shown above) no value need be exactly
at the value of the median. Nonetheless, the value of the median is uniquely
determined with the usual definition. A related concept, in which the outcome
is forced to correspond to a member of the sample, is the medoid.
In a population, at most half have values strictly less than the median and at
most half have values strictly greater than it. If each group contains less
than half the population, then some of the population is exactly equal to the
median. For example, if a < b < c, then the median of the list {a, b, c} is b,
and, if a < b < c < d, then the median of the list {a, b, c, d} is the mean of
b and c; i.e., it is (b + c)/2. Indeed, as it is based on the middle data in a
group, it is not necessary to even know the value of extreme results in order
to calculate a median. For example, in a psychology test investigating the time
needed to solve a problem, if a small number of people failed to solve the
problem at all in the given time a median can still be calculated.[6]
The median can be used as a measure of location when a distribution is skewed,
when end-values are not known, or when one requires reduced importance to be
attached to outliers, e.g., because they may be measurement errors.
A median is only defined on ordered one-dimensional data, and is independent of
any distance_metric. A geometric_median, on the other hand, is defined in any
number of dimensions.
The median is one of a number of ways of summarising the typical values
associated with members of a statistical population; thus, it is a possible
location_parameter. The median is the 2nd quartile, 5th decile, and 50th
percentile. Since the median is the same as the second quartile, its
calculation is illustrated in the article on quartiles. A median can be worked
out for ranked but not numerical classes (e.g. working out a median grade when
students are graded from A to F), although the result might be halfway between
grades if there is an even number of cases.
When the median is used as a location parameter in descriptive statistics,
there are several choices for a measure of variability: the range, the
interquartile_range, the mean_absolute_deviation, and the median_absolute
deviation.
For practical purposes, different measures of location and dispersion are often
compared on the basis of how well the corresponding population values can be
estimated from a sample of data. The median, estimated using the sample median,
has good properties in this regard. While it is not usually optimal if a given
population distribution is assumed, its properties are always reasonably good.
For example, a comparison of the efficiency of candidate estimators shows that
the sample mean is more statistically efficient than the sample median when
data are uncontaminated by data from heavy-tailed distributions or from
mixtures of distributions, but less efficient otherwise, and that the
efficiency of the sample median is higher than that for a wide range of
distributions. More specifically, the median has a 64% efficiency compared to
the minimum-variance mean (for large normal samples), which is to say the
variance of the median will be ~50% greater than the variance of the meanâsee
asymptotic_efficiency and references therein.
***** Probability distributions[edit] *****
Geometric visualisation of the mode, median and mean of an arbitrary
probability density function.[7]
For any probability_distribution on the real line R with cumulative
distribution_function F, regardless of whether it is any kind of continuous
probability distribution, in particular an absolutely_continuous_distribution
(which has a probability_density_function), or a discrete probability
distribution, a median is by definition any real number m that satisfies the
inequalities
         P &#x2061; ( X &#x2264; m ) &#x2265;   1 2    &#xA0;and&#xA0;  P
      &#x2061; ( X &#x2265; m ) &#x2265;   1 2       {\displaystyle
      \operatorname {P} (X\leq m)\geq {\frac {1}{2}}{\text{ and }}\operatorname
      {P} (X\geq m)\geq {\frac {1}{2}}\,\!}  [\operatorname {P} (X\leq m)\geq
      {\frac {1}{2}}{\text{ and }}\operatorname {P} (X\geq m)\geq {\frac {1}
      {2}}\,\!]
or, equivalently, the inequalities
          &#x222B;  ( &#x2212; &#x221E; , m ]   d F ( x ) &#x2265;   1 2
      &#xA0;and&#xA0;   &#x222B;  [ m , &#x221E; )   d F ( x ) &#x2265;   1 2
      {\displaystyle \int _{(-\infty ,m]}dF(x)\geq {\frac {1}{2}}{\text{ and
      }}\int _{[m,\infty )}dF(x)\geq {\frac {1}{2}}\,\!}  [\int _{(-\infty
      ,m]}dF(x)\geq {\frac {1}{2}}{\text{ and }}\int _{[m,\infty )}dF(x)\geq
      {\frac {1}{2}}\,\!]
in which a LebesgueâStieltjes_integral is used. For an absolutely continuous
probability distribution with probability_density_function Æ, the median
satisfies
         P &#x2061; ( X &#x2264; m ) = P &#x2061; ( X &#x2265; m ) =  &#x222B;
      &#x2212; &#x221E;   m   f ( x )  d x =   1 2   .     {\displaystyle
      \operatorname {P} (X\leq m)=\operatorname {P} (X\geq m)=\int _{-\infty }^
      {m}f(x)\,dx={\frac {1}{2}}.\,\!}  [\operatorname {P} (X\leq
      m)=\operatorname {P} (X\geq m)=\int _{-\infty }^{m}f(x)\,dx={\frac {1}
      {2}}.\,\!]
Any probability_distribution on R has at least one median, but in specific
cases there may be more than one median. Specifically, if a probability density
is zero on an interval [a, b], and the cumulative_distribution_function at a is
1/2, any value between a and b will also be a median.
**** Medians of particular distributions[edit] ****
The medians of certain types of distributions can be easily calculated from
their parameters; furthermore, they exist even for some distributions lacking a
well-defined mean, such as the Cauchy_distribution:
    * The median of a symmetric unimodal_distribution coincides with the mode.
    * The median of a symmetric_distribution which possesses a mean Î¼ also
      takes the value Î¼.
          o The median of a normal_distribution with mean Î¼ and variance Ï2
            is Î¼. In fact, for a normal distribution, mean = median = mode.
          o The median of a uniform_distribution in the interval [a, b] is
            (a + b) / 2, which is also the mean.
    * The median of a Cauchy_distribution with location parameter x0 and scale
      parameter y is x0, the location parameter.
    * The median of a power_law_distribution xâa, with exponent a > 1 is 21/
      (a â 1)xmin, where xmin is the minimum value for which the power law
      holds[8]
    * The median of an exponential_distribution with rate_parameter Î» is the
      natural logarithm of 2 divided by the rate parameter: Î»â1ln 2.
    * The median of a Weibull_distribution with shape parameter k and scale
      parameter Î» is Î»(ln 2)1/k.
***** Populations[edit] *****
**** Optimality property[edit] ****
The mean absolute error of a real variable c with respect to the random
variable X is
         E (  |  X &#x2212; c  |  )    {\displaystyle E(\left|X-c\right|)\,}
      [E(\left|X-c\right|)\,]
Provided that the probability distribution of X is such that the above
expectation exists, then m is a median of X if and only if m is a minimizer of
the mean absolute error with respect to X.[9] In particular, m is a sample
median if and only if m minimizes the arithmetic mean of the absolute
deviations.
More generally, a median is defined as a minimum of
         E (  |  X &#x2212; c  |  &#x2212;  |  X  |  ) ,   {\displaystyle E(|X-
      c|-|X|),}  [{\displaystyle E(|X-c|-|X|),}]
as discussed below in the section on multivariate_medians (specifically, the
spatial_median).
This optimization-based definition of the median is useful in statistical data-
analysis, for example, in k-medians_clustering.
**** Unimodal distributions[edit] ****
Comparison of mean, median and mode of two log-normal_distributions with
different skewness.
It can be shown for a unimodal distribution that the median        X &#x007E;
{\displaystyle {\tilde {X}}}  [{\tilde {X}}] and the mean        X &#x00AF;
{\displaystyle {\bar {X}}}  [{\bar {X}}] lie within (3/5)1/2 â 0.7746
standard deviations of each other.[10] In symbols,
            |     X &#x007E;    &#x2212;    X &#x00AF;     |  &#x03C3;
      &#x2264;   (   3 5   )    1 2      {\displaystyle {\frac {\left|{\tilde
      {X}}-{\bar {X}}\right|}{\sigma }}\leq \left({\frac {3}{5}}\right)^{\frac
      {1}{2}}}  [{\displaystyle {\frac {\left|{\tilde {X}}-{\bar {X}}\right|}
      {\sigma }}\leq \left({\frac {3}{5}}\right)^{\frac {1}{2}}}]
where |Â·| is the absolute value.
A similar relation holds between the median and the mode: they lie within 31/
2 â 1.732 standard deviations of each other:
             |     X &#x007E;    &#x2212;  m o d e   |   &#x03C3;   &#x2264;  3
      1 2    .   {\displaystyle {\frac {|{\tilde {X}}-\mathrm {mode} |}{\sigma
      }}\leq 3^{\frac {1}{2}}.}  [{\displaystyle {\frac {|{\tilde {X}}-\mathrm
      {mode} |}{\sigma }}\leq 3^{\frac {1}{2}}.}]
**** Inequality relating means and medians[edit] ****
If the distribution has finite variance, then the distance between the median
and the mean is bounded by one standard_deviation.
This bound was proved by Mallows,[11] who used Jensen's_inequality twice, as
follows. We have
              |  &#x03BC; &#x2212; m  |  =  |  E &#x2061; ( X &#x2212; m )  |
      &#x2264; E &#x2061; (  |  X &#x2212; m  |  )       &#x2264; E &#x2061;
      (  |  X &#x2212; &#x03BC;  |  )       &#x2264;   E &#x2061;  (  ( X
      &#x2212; &#x03BC;  )  2    )    = &#x03C3; .       {\displaystyle {\begin
      {aligned}|\mu -m|=|\operatorname {E} (X-m)|&\leq \operatorname {E} (|X-
      m|)\\&\leq \operatorname {E} (|X-\mu |)\\&\leq {\sqrt {\operatorname {E}
      \left((X-\mu )^{2}\right)}}=\sigma .\end{aligned}}}  [{\displaystyle
      {\begin{aligned}|\mu -m|=|\operatorname {E} (X-m)|&\leq \operatorname {E}
      (|X-m|)\\&\leq \operatorname {E} (|X-\mu |)\\&\leq {\sqrt {\operatorname
      {E} \left((X-\mu )^{2}\right)}}=\sigma .\end{aligned}}}]
The first and third inequalities come from Jensen's inequality applied to the
absolute-value function and the square function, which are each convex. The
second inequality comes from the fact that a median minimizes the absolute
deviation function
         a &#x21A6; E &#x2061; (  |  X &#x2212; a  |  ) .    {\displaystyle
      a\mapsto \operatorname {E} (|X-a|).\,}  [{\displaystyle a\mapsto
      \operatorname {E} (|X-a|).\,}]
This proof also follows directly from Cantelli's_inequality.[12] The result can
be generalized to obtain a multivariate version of the inequality,[13] as
follows:
             &#x2016; &#x03BC; &#x2212; m &#x2016; = &#x2016; E &#x2061; ( X
      &#x2212; m ) &#x2016;    &#x2264; E &#x2061; &#x2016; X &#x2212; m
      &#x2016;       &#x2264; E &#x2061; ( &#x2016; X &#x2212; &#x03BC;
      &#x2016; )       &#x2264;   E &#x2061;  (  &#x2016; X &#x2212; &#x03BC;
      &#x2016;  2    )    =   trace &#x2061;  (  var &#x2061; ( X )  )
      {\displaystyle {\begin{aligned}\|\mu -m\|=\|\operatorname {E} (X-
      m)\|&\leq \operatorname {E} \|X-m\|\\&\leq \operatorname {E} (\|X-\mu
      \|)\\&\leq {\sqrt {\operatorname {E} \left(\|X-\mu \|^{2}\right)}}={\sqrt
      {\operatorname {trace} \left(\operatorname {var} (X)\right)}}\end
      {aligned}}}  [{\displaystyle {\begin{aligned}\|\mu -m\|=\|\operatorname
      {E} (X-m)\|&\leq \operatorname {E} \|X-m\|\\&\leq \operatorname {E} (\|X-
      \mu \|)\\&\leq {\sqrt {\operatorname {E} \left(\|X-\mu \|^{2}\right)}}=
      {\sqrt {\operatorname {trace} \left(\operatorname {var} (X)\right)}}\end
      {aligned}}}]
where m is a spatial_median, that is, a minimizer of the function     a
&#x21A6; E &#x2061; ( &#x2016; X &#x2212; a &#x2016; ) .    {\displaystyle
a\mapsto \operatorname {E} (\|X-a\|).\,}  [{\displaystyle a\mapsto
\operatorname {E} (\|X-a\|).\,}] The spatial median is unique when the data-
set's dimension is two or more.[14][15] An alternative proof uses the one-sided
Chebyshev inequality; it appears in an_inequality_on_location_and_scale
parameters.
***** Jensen's inequality for medians[edit] *****
Jensen's inequality states that for any random variable x with a finite
expectation E(x) and for any convex function f
         f [ E ( x ) ] &#x2264; E [ f ( x ) ]   {\displaystyle f[E(x)]\leq E[f
      (x)]}  [{\displaystyle f[E(x)]\leq E[f(x)]}]
It has been shown[16] that if x is a real variable with a unique median m and f
is a C function then
         f ( m ) &#x2264; Median &#x2061; [ f ( x ) ]   {\displaystyle f(m)\leq
      \operatorname {Median} [f(x)]}  [{\displaystyle f(m)\leq \operatorname
      {Median} [f(x)]}]
A C function is a real valued function, defined on the set of real numbers R,
with the property that for any real t
          f  &#x2212; 1    (   ( &#x2212; &#x221E; , t ]   )  = { x &#x2208; R
      &#x2223; f ( x ) &#x2264; t }   {\displaystyle f^{-1}\left(\,(-\infty
      ,t]\,\right)=\{x\in R\mid f(x)\leq t\}}  [{\displaystyle f^{-1}\left(\,(-
      \infty ,t]\,\right)=\{x\in R\mid f(x)\leq t\}}]
is a closed interval, a singleton or an empty_set.
***** Medians for samples[edit] *****
**** The sample median[edit] ****
***  Efficient computation of the sample median[edit] ***
Even though comparison-sorting n items requires Î©(n log n) operations,
selection_algorithms can compute the k'th-smallest_of_n_items with only Î(n)
operations. This includes the median, which is the n/2'th order statistic (or
for an even number of samples, the arithmetic_mean of the two middle order
statistics).
Selection algorithms still have the downside of requiring Î©(n) memory, that
is, they need to have the full sample (or a linear-sized portion of it) in
memory. Because this, as well as the linear time requirement, can be
prohibitive, several estimation procedures for the median have been developed.
A simple one is the median of three rule, which estimates the median as the
median of a three-element subsample; this is commonly used as a subroutine in
the quicksort sorting algorithm, which uses an estimate of its input's median.
A more robust_estimator is Tukey's ninther, which is the median of three rule
applied with limited recursion:[17] if A is the sample laid out as an array,
and
      med3(A) = median(A[1], A[n/2], A[n]),
then
      ninther(A) = med3(med3(A[1 ... 1/3n]), med3(A[1/3n ... 2/3n]), med3(A[2/
      3n ... n]))
The remedian is an estimator for the median that requires linear time but sub-
linear memory, operating in a single pass over the sample.[18]
*** Easy explanation of the sample median[edit] ***
In individual series (if number of observation is very low) first one must
arrange all the observations in order. Then count(n) is the total number of
observation in given data.
If n is odd then Median (M) = value of ((n + 1)/2)th item term.
If n is even then Median (M) = value of [(n/2)th item term + (n/2 + 1)th item
term]/2
  For an odd number of values
As an example, we will calculate the sample median for the following set of
observations: 1, 5, 2, 8, 7.
Start by sorting the values: 1, 2, 5, 7, 8.
In this case, the median is 5 since it is the middle observation in the ordered
list.
The median is the ((n + 1)/2)th item, where n is the number of values. For
example, for the list {1, 2, 5, 7, 8}, we have n = 5, so the median is the (
(5 + 1)/2)th item.
      median = (6/2)th item
      median = 3rd item
      median = 5
  For an even number of values
As an example, we will calculate the sample median for the following set of
observations: 1, 6, 2, 8, 7, 2.
Start by sorting the values: 1, 2, 2, 6, 7, 8.
In this case, the arithmetic mean of the two middlemost terms is (2 + 6)/2 = 4.
Therefore, the median is 4 since it is the arithmetic mean of the middle
observations in the ordered list.
*** Sampling distribution[edit] ***
The distributions of both the sample mean and the sample median were determined
by Laplace.[19] The distribution of the sample median from a population with a
density function     f ( x )   {\displaystyle f(x)}  [f(x)] is asymptotically
normal with mean     m   {\displaystyle m}  [m] and variance[20]
           1  4 n f ( m  )  2        {\displaystyle {\frac {1}{4nf(m)^{2}}}}  [
      {\frac {1}{4nf(m)^{2}}}]
where     m   {\displaystyle m}  [m] is the median of     f ( x )
{\displaystyle f(x)}  [f(x)] and     n   {\displaystyle n}  [n] is the sample
size.
These results have also been extended.[21] It is now known for the     p
{\displaystyle p}  [p]-th quantile that the distribution of the sample     p
{\displaystyle p}  [p]-th quantile is asymptotically normal around the     p
{\displaystyle p}  [p]-th quantile with variance equal to
            p ( 1 &#x2212; p )   n f (  x  p    )  2        {\displaystyle
      {\frac {p(1-p)}{nf(x_{p})^{2}}}}  [{\frac {p(1-p)}{nf(x_{p})^{2}}}]
where     f (  x  p   )   {\displaystyle f(x_{p})}  [f(x_{p})] is the value of
the distribution density at the     p   {\displaystyle p}  [p]-th quantile.
In the case of a discrete variable, the sampling distribution of the median for
small-samples can be investigated as follows. We take the sample size to be an
odd number     N = 2 n + 1   {\displaystyle N=2n+1}  [{\displaystyle N=2n+1}].
If a given value     v   {\displaystyle v}  [v] is to be the median of the
sample then two conditions must be satisfied. The first is that at most     n
{\displaystyle n}  [n] observations can have a value of     v &#x2212; 1
{\displaystyle v-1}  [{\displaystyle v-1}] or less. The second is that at most
n   {\displaystyle n}  [n] observations can have a value of     v + 1
{\displaystyle v+1}  [{\displaystyle v+1}] or more. Let     i   {\displaystyle
i}  [i] be the number of observations which have a value of     v &#x2212; 1
{\displaystyle v-1}  [{\displaystyle v-1}] or less and let     k
{\displaystyle k}  [k] be the number of observations which have a value of
v + 1   {\displaystyle v+1}  [{\displaystyle v+1}] or more. Then     i
{\displaystyle i}  [i] and     k   {\displaystyle k}  [k] both have a minimum
value of 0 and a maximum of     n   {\displaystyle n}  [n]. If an observation
has a value below     v   {\displaystyle v}  [v], it is not relevant how far
below     v   {\displaystyle v}  [v] it is and conversely, if an observation
has a value above     v   {\displaystyle v}  [v], it is not relevant how far
above     v   {\displaystyle v}  [v] it is. We can therefore represent the
observations as following a trinomial distribution with probabilities     F ( v
&#x2212; 1 )   {\displaystyle F(v-1)}  [{\displaystyle F(v-1)}],     f ( v )
{\displaystyle f(v)}  [{\displaystyle f(v)}] and     1 &#x2212; F ( v )
{\displaystyle 1-F(v)}  [{\displaystyle 1-F(v)}]. The probability that the
median     m   {\displaystyle m}  [m] will have a value     v   {\displaystyle
v}  [v] is then given by
         Pr ( m = v ) =  &#x2211;  i = 0   n    &#x2211;  k = 0   n      N !
      i ! ( N &#x2212; i &#x2212; k ) ! k !    [ F ( v &#x2212; 1 )  ]  i   [ f
      ( v )  ]  N &#x2212; i &#x2212; k   [ 1 &#x2212; F ( v )  ]  k   .
      {\displaystyle \Pr(m=v)=\sum _{i=0}^{n}\sum _{k=0}^{n}{\frac {N!}{i!(N-i-
      k)!k!}}[F(v-1)]^{i}[f(v)]^{N-i-k}[1-F(v)]^{k}.}  [{\displaystyle \Pr
      (m=v)=\sum _{i=0}^{n}\sum _{k=0}^{n}{\frac {N!}{i!(N-i-k)!k!}}[F(v-1)]^
      {i}[f(v)]^{N-i-k}[1-F(v)]^{k}.}]
Summing this over all values of     v   {\displaystyle v}  [v] defines a proper
distribution and gives a unit sum. In practice, the function     f ( v )
{\displaystyle f(v)}  [{\displaystyle f(v)}] will often not be known but it can
be estimated from an observed frequency distribution. An example is given in
the following table where the actual distribution is not known but a sample of
3,800 observations allows a sufficiently accurate assessment of     f ( v )
{\displaystyle f(v)}  [{\displaystyle f(v)}].
v    0     0.5   1     1.5   2     2.5   3     3.5   4     4.5   5
f(v) 0.000 0.008 0.010 0.013 0.083 0.108 0.328 0.220 0.202 0.023 0.005
F(v) 0.000 0.008 0.018 0.031 0.114 0.222 0.550 0.770 0.972 0.995 1.000
Using these data it is possible to investigate the effect of sample size on the
standard errors of the mean and median. The observed mean is 3.16, the observed
raw median is 3 and the observed interpolated median is 3.174. The following
table gives some comparison statistics. The standard error of the median is
given both from the above expression for     p r ( m = v )   {\displaystyle pr
(m=v)}  [{\displaystyle pr(m=v)}] and from the asymptotic approximation given
earlier.
Sample size                                         3     9     15    21
Statistic
Expected value of median                            3.198 3.191 3.174 3.161
Standard error of median (above formula)            0.482 0.305 0.257 0.239
Standard error of median (asymptotic approximation) 0.879 0.508 0.393 0.332
Standard error of mean                              0.421 0.243 0.188 0.159
The expected value of the median falls slightly as sample size increases while,
as would be expected, the standard errors of both the median and the mean are
proportionate to the inverse square root of the sample size. The asymptotic
approximation errs on the side of caution by overestimating the standard error.
In the case of a continuous variable, the following argument can be used. If a
given value     v   {\displaystyle v}  [v] is to be the median, then one
observation must take the value     v   {\displaystyle v}  [v]. The elemental
probability of this is     f ( v )  d v   {\displaystyle f(v)\,dv}  [
{\displaystyle f(v)\,dv}]. Then, of the remaining     2 n   {\displaystyle 2n}
[2n] observations, exactly     n   {\displaystyle n}  [n] of them must be above
v   {\displaystyle v}  [v] and the remaining     n   {\displaystyle n}  [n]
below. The probability of this is the     n   {\displaystyle n}  [n]th term of
a binomial distribution with parameters     F ( v )   {\displaystyle F(v)}  [
{\displaystyle F(v)}] and     2 n   {\displaystyle 2n}  [2n]. Finally we
multiply by     2 n + 1   {\displaystyle 2n+1}  [2n+1] since any of the
observations in the sample can be the median observation. Hence the elemental
probability of the median at the point     v   {\displaystyle v}  [v] is given
by
         f ( v )    ( 2 n ) !   n ! n !    [ F ( v )  ]  n   [ 1 &#x2212; F ( v
      )  ]  n   ( 2 n + 1 )  d v .   {\displaystyle f(v){\frac {(2n)!}{n!n!}}[F
      (v)]^{n}[1-F(v)]^{n}(2n+1)\,dv.}  [{\displaystyle f(v){\frac {(2n)!}
      {n!n!}}[F(v)]^{n}[1-F(v)]^{n}(2n+1)\,dv.}]
Now we introduce the beta function. For integer arguments     &#x03B1;
{\displaystyle \alpha }  [\alpha ] and     &#x03B2;   {\displaystyle \beta }
[\beta ], this can be expressed as      B  ( &#x03B1; , &#x03B2; ) = ( &#x03B1;
&#x2212; 1 ) ! ( &#x03B2; &#x2212; 1 ) !  /  ( &#x03B1; + &#x03B2; &#x2212; 1 )
!   {\displaystyle \mathrm {B} (\alpha ,\beta )=(\alpha -1)!(\beta -1)!/(\alpha
+\beta -1)!}  [{\displaystyle \mathrm {B} (\alpha ,\beta )=(\alpha -1)!(\beta -
1)!/(\alpha +\beta -1)!}]. Also, we note that     f ( v ) = d F ( v )  /  d v
{\displaystyle f(v)=dF(v)/dv}  [{\displaystyle f(v)=dF(v)/dv}]. Using these
relationships and setting both     &#x03B1;   {\displaystyle \alpha }  [\alpha
] and     &#x03B2;   {\displaystyle \beta }  [\beta ] equal to     ( n + 1 )
{\displaystyle (n+1)}  [{\displaystyle (n+1)}] allows the last expression to be
written as
            [ F ( v )  ]  n   [ 1 &#x2212; F ( v )  ]  n      B  ( n + 1 , n +
      1 )     d F ( v )   {\displaystyle {\frac {[F(v)]^{n}[1-F(v)]^{n}}
      {\mathrm {B} (n+1,n+1)}}\,dF(v)}  [{\displaystyle {\frac {[F(v)]^{n}[1-F
      (v)]^{n}}{\mathrm {B} (n+1,n+1)}}\,dF(v)}]
Hence the density function of the median is a symmetric beta distribution over
the unit interval which supports     F ( v )   {\displaystyle F(v)}  [
{\displaystyle F(v)}]. Its mean, as we would expect, is 0.5 and its variance is
1  /  ( 4 ( N + 2 ) )   {\displaystyle 1/(4(N+2))}  [{\displaystyle 1/(4
(N+2))}]. The corresponding variance of the sample median is
           1  4 ( N + 2 ) f ( m  )  2      .   {\displaystyle {\frac {1}{4
      (N+2)f(m)^{2}}}.}  [{\displaystyle {\frac {1}{4(N+2)f(m)^{2}}}.}]
However this finding can only be used if the density function     f ( v )
{\displaystyle f(v)}  [{\displaystyle f(v)}] is known or can be assumed. As
this will not always be the case, the median variance has to be estimated
sometimes from the sample data.
  Estimation of variance from sample data
The value of     ( 2 f ( x )  )  &#x2212; 2     {\displaystyle (2f(x))^{-2}}  [
(2f(x))^{-2}]âthe asymptotic value of      n  &#x2212;   1 2     ( &#x03BD;
&#x2212; m )   {\displaystyle n^{-{\frac {1}{2}}}(\nu -m)}  [n^{-{\frac {1}
{2}}}(\nu -m)] where     &#x03BD;   {\displaystyle \nu }  [\nu ] is the
population medianâhas been studied by several authors. The standard "delete
one" jackknife method produces inconsistent results.[22] An alternativeâthe
"delete k" methodâwhere     k   {\displaystyle k}  [k] grows with the sample
size has been shown to be asymptotically consistent.[23] This method may be
computationally expensive for large data sets. A bootstrap estimate is known to
be consistent,[24] but converges very slowly (order of      n  &#x2212;   1 4
{\displaystyle n^{-{\frac {1}{4}}}}  [n^{-{\frac {1}{4}}}]).[25] Other methods
have been proposed but their behavior may differ between large and small
samples.[26]
  Efficiency
The efficiency of the sample median, measured as the ratio of the variance of
the mean to the variance of the median, depends on the sample size and on the
underlying population distribution. For a sample of size     N = 2 n + 1
{\displaystyle N=2n+1}  [N=2n+1] from the normal_distribution, the efficiency
for large N is
           2 &#x03C0;      N + 2  N     {\displaystyle {\frac {2}{\pi }}{\frac
      {N+2}{N}}}  [{\displaystyle {\frac {2}{\pi }}{\frac {N+2}{N}}}]
The efficiency tends to       2 &#x03C0;     {\displaystyle {\frac {2}{\pi }}}
[{\displaystyle {\frac {2}{\pi }}}] as     N   {\displaystyle N}  [N] tends to
infinity.
**** Other estimators[edit] ****
For univariate distributions that are symmetric about one median, the
HodgesâLehmann_estimator is a robust and highly efficient_estimator of the
population median.[27]
If data are represented by a statistical_model specifying a particular family
of probability_distributions, then estimates of the median can be obtained by
fitting that family of probability distributions to the data and calculating
the theoretical median of the fitted distribution.[citation_needed] Pareto
interpolation is an application of this when the population is assumed to have
a Pareto_distribution.
**** Coefficient of dispersion[edit] ****
The coefficient of dispersion (CD) is defined as the ratio of the average
absolute deviation from the median to the median of the data.[28] It is a
statistical measure used by the states of Iowa, New_York and South_Dakota in
estimating dues taxes.[29][30][31] In symbols
         C D =   1 n      &#x2211;  |  m &#x2212; x  |   m     {\displaystyle
      CD={\frac {1}{n}}{\frac {\sum |m-x|}{m}}}  [CD={\frac {1}{n}}{\frac {\sum
      |m-x|}{m}}]
where n is the sample size, m is the sample median and x is a variate. The sum
is taken over the whole sample.
Confidence intervals for a two-sample test in which the sample sizes are large
have been derived by Bonett and Seier[28] This test assumes that both samples
have the same median but differ in the dispersion around it. The confidence
interval (CI) is bounded inferiorly by
         exp &#x2061;  [  log &#x2061;  (    t  a    t  b     )  &#x2212;  z
      &#x03B1;     (  var &#x2061;  [  log &#x2061;  (    t  a    t  b     )
      ]   )    1 2     ]    {\displaystyle \exp \left[\log \left({\frac {t_{a}}
      {t_{b}}}\right)-z_{\alpha }\left(\operatorname {var} \left[\log \left(
      {\frac {t_{a}}{t_{b}}}\right)\right]\right)^{\frac {1}{2}}\right]}  [
      {\displaystyle \exp \left[\log \left({\frac {t_{a}}{t_{b}}}\right)-z_
      {\alpha }\left(\operatorname {var} \left[\log \left({\frac {t_{a}}{t_
      {b}}}\right)\right]\right)^{\frac {1}{2}}\right]}]
where tj is the mean absolute deviation of the jth sample, var() is the
variance and zÎ± is the value from the normal distribution for the chosen value
of Î±: for Î± = 0.05, zÎ± = 1.96. The following formulae are used in the
derivation of these confidence intervals
         var &#x2061; [ log &#x2061; (  t  a   ) ] =   1 n    [     s  a   2
      t  a   2     +   (     x  a   &#x2212;    x &#x00AF;      t  a     )   2
      &#x2212; 1  ]    {\displaystyle \operatorname {var} [\log(t_{a})]={\frac
      {1}{n}}\left[{\frac {s_{a}^{2}}{t_{a}^{2}}}+\left({\frac {x_{a}-{\bar
      {x}}}{t_{a}}}\right)^{2}-1\right]}  [{\displaystyle \operatorname {var}
      [\log(t_{a})]={\frac {1}{n}}\left[{\frac {s_{a}^{2}}{t_{a}^{2}}}+\left(
      {\frac {x_{a}-{\bar {x}}}{t_{a}}}\right)^{2}-1\right]}]
         var &#x2061;  [  log &#x2061;  (    t  a    t  b     )   ]  = var
      &#x2061; [ log &#x2061; (  t  a   ) ] + var &#x2061; [ log &#x2061; (  t
      b   ) ] &#x2212; 2 r ( var &#x2061; [ log &#x2061; (  t  a   ) ] var
      &#x2061; [ log &#x2061; (  t  b   ) ]  )   1 2      {\displaystyle
      \operatorname {var} \left[\log \left({\frac {t_{a}}{t_
      {b}}}\right)\right]=\operatorname {var} [\log(t_{a})]+\operatorname {var}
      [\log(t_{b})]-2r(\operatorname {var} [\log(t_{a})]\operatorname {var}
      [\log(t_{b})])^{\frac {1}{2}}}  [{\displaystyle \operatorname {var} \left
      [\log \left({\frac {t_{a}}{t_{b}}}\right)\right]=\operatorname {var}
      [\log(t_{a})]+\operatorname {var} [\log(t_{b})]-2r(\operatorname {var}
      [\log(t_{a})]\operatorname {var} [\log(t_{b})])^{\frac {1}{2}}}]
where r is the Pearson correlation coefficient between the squared deviation
scores
          d  i a   =  |   x  i a   &#x2212;     x &#x00AF;     a    |
      {\displaystyle d_{ia}=|x_{ia}-{\bar {x}}_{a}|}  [d_{ia}=|x_{ia}-{\bar
      {x}}_{a}|] and      d  i b   =  |   x  i b   &#x2212;     x &#x00AF;
      b    |    {\displaystyle d_{ib}=|x_{ib}-{\bar {x}}_{b}|}  [d_{ib}=|x_
      {ib}-{\bar {x}}_{b}|]
a and b here are constants equal to 1 and 2, x is a variate and s is the
standard deviation of the sample.
***** Multivariate median[edit] *****
Previously, this article discussed the univariate median, when the sample or
population had one-dimension. When the dimension is two or higher, there are
multiple concepts that extend the definition of the univariate median; each
such multivariate median agrees with the univariate median when the dimension
is exactly one.[27][32][33][34]
**** Marginal median[edit] ****
The marginal median is defined for vectors defined with respect to a fixed set
of coordinates. A marginal median is defined to be the vector whose components
are univariate medians. The marginal median is easy to compute, and its
properties were studied by Puri and Sen.[27][35]
**** Centerpoint[edit] ****
An alternative generalization of the median in higher dimensions is the
centerpoint.
***** Other median-related concepts[edit] *****
**** Interpolated median[edit] ****
When dealing with a discrete variable, it is sometimes useful to regard the
observed values as being midpoints of underlying continuous intervals. An
example of this is a Likert scale, on which opinions or preferences are
expressed on a scale with a set number of possible responses. If the scale
consists of the positive integers, an observation of 3 might be regarded as
representing the interval from 2.50 to 3.50. It is possible to estimate the
median of the underlying variable. If, say, 22% of the observations are of
value 2 or below and 55.0% are of 3 or below (so 33% have the value 3), then
the median     m   {\displaystyle m}  [m] is 3 since the median is the smallest
value of     x   {\displaystyle x}  [x] for which     F ( x )   {\displaystyle
F(x)}  [F(x)] is greater than a half. But the interpolated median is somewhere
between 2.50 and 3.50. First we add half of the interval width     w
{\displaystyle w}  [w] to the median to get the upper bound of the median
interval. Then we subtract that proportion of the interval width which equals
the proportion of the 33% which lies above the 50% mark. In other words, we
split up the interval width pro rata to the numbers of observations. In this
case, the 33% is split into 28% below the median and 5% above it so we subtract
5/33 of the interval width from the upper bound of 3.50 to give an interpolated
median of 3.35. More formally, if the values     f ( x )   {\displaystyle f(x)}
[f(x)] are known, the interpolated median can be calculated from
          m  int   = m + w  [    1 2   &#x2212;    F ( m ) &#x2212;   1 2     f
      ( m )     ]  .   {\displaystyle m_{\text{int}}=m+w\left[{\frac {1}{2}}-
      {\frac {F(m)-{\frac {1}{2}}}{f(m)}}\right].}  [{\displaystyle m_{\text
      {int}}=m+w\left[{\frac {1}{2}}-{\frac {F(m)-{\frac {1}{2}}}{f
      (m)}}\right].}]
Alternatively, if in an observed sample there are     k   {\displaystyle k}
[k] scores above the median category,     j   {\displaystyle j}  [j] scores in
it and     i   {\displaystyle i}  [i] scores below it then the interpolated
median is given by
          m  int   = m +   w 2    [    k &#x2212; i  j   ]  .   {\displaystyle
      m_{\text{int}}=m+{\frac {w}{2}}\left[{\frac {k-i}{j}}\right].}  [
      {\displaystyle m_{\text{int}}=m+{\frac {w}{2}}\left[{\frac {k-i}
      {j}}\right].}]
**** Pseudo-median[edit] ****
Main article: Pseudomedian
For univariate distributions that are symmetric about one median, the
HodgesâLehmann_estimator is a robust and highly efficient estimator of the
population median; for non-symmetric distributions, the HodgesâLehmann
estimator is a robust and highly efficient estimator of the population pseudo-
median, which is the median of a symmetrized distribution and which is close to
the population median.[36] The HodgesâLehmann estimator has been generalized
to multivariate distributions.[37]
**** Variants of regression[edit] ****
The TheilâSen_estimator is a method for robust linear_regression based on
finding medians of slopes.[38]
**** Median filter[edit] ****
Main article: Median_filter
In the context of image_processing of monochrome raster_images there is a type
of noise, known as the salt_and_pepper_noise, when each pixel independently
becomes black (with some small probability) or white (with some small
probability), and is unchanged otherwise (with the probability close to 1). An
image constructed of median values of neighborhoods (like 3Ã3 square) can
effectively reduce_noise in this case.[citation_needed]
**** Cluster analysis[edit] ****
Main article: k-medians_clustering
In cluster_analysis, the k-medians_clustering algorithm provides a way of
defining clusters, in which the criterion of maximising the distance between
cluster-means that is used in k-means_clustering, is replaced by maximising the
distance between cluster-medians.
**** Medianâmedian line[edit] ****
This is a method of robust regression. The idea dates back to Wald in 1940 who
suggested dividing a set of bivariate data into two halves depending on the
value of the independent parameter     x   {\displaystyle x}  [x]: a left half
with values less than the median and a right half with values greater than the
median.[39] He suggested taking the means of the dependent     y
{\displaystyle y}  [y] and independent     x   {\displaystyle x}  [x] variables
of the left and the right halves and estimating the slope of the line joining
these two points. The line could then be adjusted to fit the majority of the
points in the data set.
Nair and Shrivastava in 1942 suggested a similar idea but instead advocated
dividing the sample into three equal parts before calculating the means of the
subsamples.[40] Brown and Mood in 1951 proposed the idea of using the medians
of two subsamples rather the means.[41] Tukey combined these ideas and
recommended dividing the sample into three equal size subsamples and estimating
the line based on the medians of the subsamples.[42]
***** Median-unbiased estimators[edit] *****
Main article: Bias_of_an_estimator_Â§ Median-unbiased_estimators
Any mean-unbiased_estimator minimizes the risk (expected_loss) with respect to
the squared-error loss_function, as observed by Gauss. A median-unbiased
estimator minimizes the risk with respect to the absolute-deviation loss
function, as observed by Laplace. Other loss_functions are used in statistical
theory, particularly in robust_statistics.
The theory of median-unbiased estimators was revived by George_W._Brown in
1947:[43]
     An estimate of a one-dimensional parameter Î¸ will be said to be
     median-unbiased if, for fixed Î¸, the median of the distribution of
     the estimate is at the value Î¸; i.e., the estimate underestimates
     just as often as it overestimates. This requirement seems for most
     purposes to accomplish as much as the mean-unbiased requirement and
     has the additional property that it is invariant under one-to-one
     transformation.
     â page 584
Further properties of median-unbiased estimators have been reported.[44][45]
[46][47] Median-unbiased estimators are invariant under one-to-one
transformations.
There are methods of construction median-unbiased estimators that are optimal
(in a sense analogous to minimum-variance property considered for mean-unbiased
estimators). Such constructions exist for probability distributions having
monotone_likelihood-functions.[48][49] One such procedure is an analogue of the
RaoâBlackwell_procedure for mean-unbiased estimators: The procedure holds for
a smaller class of probability distributions than does the RaoâBlackwell
procedure but for a larger class of loss_functions.[50]
***** History[edit] *****
The idea of the median appeared in the 13th century in the Talmud [51][52]
(further[citation_needed] for possible older mentions)
The idea of the median also appeared later in Edward_Wright's book on
navigation (Certaine Errors in Navigation) in 1599 in a section concerning the
determination of location with a compass. Wright felt that this value was the
most likely to be the correct value in a series of observations.
In 1757, Roger_Joseph_Boscovich developed a regression method based on the L1
norm and therefore implicitly on the median.[53]
In 1774, Laplace suggested the median be used as the standard estimator of the
value of a posterior pdf. The specific criterion was to minimize the expected
magnitude of the error;      |  &#x03B1; &#x2212;  &#x03B1;  &#x2217;    |
{\displaystyle |\alpha -\alpha ^{*}|}  [|\alpha -\alpha ^{*}|] where
&#x03B1;  &#x2217;     {\displaystyle \alpha ^{*}}  [\alpha ^{*}] is the
estimate and     &#x03B1;   {\displaystyle \alpha }  [\alpha ] is the true
value. Laplaces's criterion was generally rejected for 150 years in favor of
the least_squares method of Gauss and Legendre which minimizes     ( &#x03B1;
&#x2212;  &#x03B1;  &#x2217;    )  2     {\displaystyle (\alpha -\alpha ^{*})^
{2}}  [(\alpha -\alpha ^{*})^{2}] to obtain the mean.[54] The distribution of
both the sample mean and the sample median were determined by Laplace in the
early 1800s.[19][55]
Antoine_Augustin_Cournot in 1843 was the first[56] to use the term median
(valeur mÃ©diane) for the value that divides a probability distribution into
two equal halves. Gustav_Theodor_Fechner used the median (Centralwerth) in
sociological and psychological phenomena.[57] It had earlier been used only in
astronomy and related fields. Gustav_Fechner popularized the median into the
formal analysis of data, although it had been used previously by Laplace.[57]
Francis_Galton used the English term median in 1881,[58] having earlier used
the terms middle-most value in 1869, and the medium in 1880.[59][60]
***** See also[edit] *****
    * [icon]Statistics_portal
    * Medoids which are a generalisation of the median in higher dimensions
    * Central_tendency
          o Mean
          o Mode
    * Absolute_deviation
    * Bias_of_an_estimator
    * Concentration_of_measure for Lipschitz_functions
    * Median_(geometry)
    * Median_graph
    * Median_search
    * Median_slope
    * Median_voter_theory
    * Weighted_median
***** References[edit] *****
   1. ^ a bWeisstein,_Eric_W. "Statistical_Median". MathWorld.
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
   3. ^ Simon, Laura J.; "Descriptive_statistics" Archived 2010-07-30 at the
      Wayback_Machine, Statistical Education Resource Kit, Pennsylvania State
      Department of Statistics
   4. ^David J. Sheskin (27 August 2003). Handbook_of_Parametric_and
      Nonparametric_Statistical_Procedures:_Third_Edition. CRC Press. pp. 7â.
      ISBN 978-1-4200-3626-8. Retrieved 25 February 2013.
   5. ^Derek Bissell (1994). Statistical_Methods_for_Spc_and_Tqm. CRC Press.
      pp. 26â. ISBN 978-0-412-39440-9. Retrieved 25 February 2013.
   6. ^"Journal_of_Statistics_Education,_v13n2:_Paul_T._von_Hippel".
      amstat.org.
   7. ^Robson, Colin (1994). Experiment, Design and Statistics in Psychology.
      Penguin. pp. 42â45. ISBN 0-14-017648-9.
   8. ^"AP_Statistics_Review_-_Density_Curves_and_the_Normal_Distributions".
      Retrieved 16 March 2015.
   9. ^ Newman,_Mark_EJ._"Power_laws,_Pareto_distributions_and_Zipf's_law."
      Contemporary_physics_46.5_(2005):_323â351.
  10. ^Stroock, Daniel (2011). Probability Theory. Cambridge University Press.
      p. 43. ISBN 978-0-521-13250-3.
  11. ^Basu, S.; Dasgupta, A. (1997). "The Mean, Median, and Mode of Unimodal
      Distributions:A Characterization". Theory of Probability and Its
      Applications. 41 (2): 210â223. doi:10.1137/S0040585X97975447.
  12. ^Mallows, Colin (August 1991). "Another comment on O'Cinneide". The
      American Statistician. 45 (3): 257. doi:10.1080/00031305.1991.10475815.
  13. ^ K.Van_Steen_Notes_on_probability_and_statistics
  14. ^PichÃ©, Robert (2012). Random Vectors and Random Sequences. Lambert
      Academic Publishing. ISBN 978-3659211966.
  15. ^Kemperman, Johannes H. B. (1987). Dodge, Yadolah (ed.). "The median of a
      finite measure on a Banach space: Statistical data analysis based on the
      L1-norm and related methods". Papers from the First International
      Conference held at NeuchÃ¢tel, August 31âSeptember 4, 1987. Amsterdam:
      North-Holland Publishing Co.: 217â230. MR 0949228.
  16. ^Milasevic, Philip; Ducharme, Gilles R. (1987). "Uniqueness of the
      spatial median". Annals_of_Statistics. 15 (3): 1332â1333. doi:10.1214/
      aos/1176350511. MR 0902264.
  17. ^Merkle, M. (2005). "Jensen's inequality for medians". Statistics &
      Probability Letters. 71 (3): 277â281. doi:10.1016/j.spl.2004.11.010.
  18. ^Bentley, Jon L.; McIlroy, M. Douglas (1993). "Engineering_a_sort
      function". SoftwareâPractice and Experience. 23 (11): 1249â1265. doi:
      10.1002/spe.4380231105.
  19. ^Rousseeuw, Peter J.; Bassett, Gilbert W. Jr. (1990). "The_remedian:_a
      robust_averaging_method_for_large_data_sets" (PDF). J. Amer. Stat. Soc.
      85 (409): 97â104. doi:10.1080/01621459.1990.10475311.
  20. ^ a bStigler,_Stephen (December 1973). "Studies in the History of
      Probability and Statistics. XXXII: Laplace, Fisher and the Discovery of
      the Concept of Sufficiency". Biometrika. 60 (3): 439â445. doi:10.1093/
      biomet/60.3.439. JSTOR 2334992. MR 0326872.
  21. ^Rider, Paul R. (1960). "Variance of the median of small samples from
      several special populations". J._Amer._Statist._Assoc. 55 (289):
      148â150. doi:10.1080/01621459.1960.10482056.
  22. ^Stuart, Alan; Ord, Keith (1994). Kendall's Advanced Theory of
      Statistics. London: Arnold. ISBN 0340614307.
  23. ^Efron, B. (1982). The Jackknife, the Bootstrap and other Resampling
      Plans. Philadelphia: SIAM. ISBN 0898711797.
  24. ^Shao, J.; Wu, C. F. (1989). "A General Theory for Jackknife Variance
      Estimation". Ann._Stat. 17 (3): 1176â1197. doi:10.1214/aos/1176347263.
      JSTOR 2241717.
  25. ^Efron, B. (1979). "Bootstrap Methods: Another Look at the Jackknife".
      Ann._Stat. 7 (1): 1â26. doi:10.1214/aos/1176344552. JSTOR 2958830.
  26. ^Hall, P.; Martin, M. A. (1988). "Exact Convergence Rate of Bootstrap
      Quantile Variance Estimator". Probab Theory Related Fields. 80 (2):
      261â268. doi:10.1007/BF00356105.
  27. ^JimÃ©nez-Gamero, M. D.; Munoz-GarcÃ­a, J.; Pino-MejÃ­as, R. (2004).
      "Reduced_bootstrap_for_the_median". Statistica Sinica. 14 (4):
      1179â1198.
  28. ^ a b cHettmansperger, Thomas P.; McKean, Joseph W. (1998). Robust
      nonparametric statistical methods. Kendall's Library of Statistics. 5.
      London: Edward Arnold. ISBN 0-340-54937-8. MR 1604954.
  29. ^ a bBonett, DG; Seier, E (2006). "Confidence interval for a coefficient
      of dispersion in non-normal distributions". Biometrical Journal. 48 (1):
      144â148. doi:10.1002/bimj.200410148.
  30. ^"Statistical_Calculation_Definitions_for_Mass_Appraisal" (PDF).
      Iowa.gov. Archived from the_original (PDF) on 11 November 2010. Median
      Ratio: The ratio located midway between the highest ratio and the lowest
      ratio when individual ratios for a class of realty are ranked in
      ascending or descending order. The median ratio is most frequently used
      to determine the level of assessment for a given class of real estate.
  31. ^"Assessment_equity_in_New_York:_Results_from_the_2010_market_value
      survey". Archived from the_original on 6 November 2012.
  32. ^"Summary_of_the_Assessment_Process" (PDF). state.sd.us. South Dakota
      Department of Revenue - Property/Special Taxes Division. Archived from
      the_original (PDF) on 10 May 2009.
  33. ^ Small, Christopher G. "A survey of multidimensional medians."
      International Statistical Review/Revue Internationale de Statistique
      (1990): 263â277. doi:10.2307/1403809 JSTOR 1403809
  34. ^ Niinimaa, A., and H. Oja. "Multivariate median." Encyclopedia of
      statistical sciences (1999).
  35. ^ Mosler, Karl. Multivariate Dispersion, Central Regions, and Depth: The
      Lift Zonoid Approach. Vol. 165. Springer Science & Business Media, 2012.
  36. ^ Puri, Madan L.; Sen, Pranab K.; Nonparametric Methods in Multivariate
      Analysis, John Wiley & Sons, New York, NY, 197l. (Reprinted by Krieger
      Publishing)
  37. ^Pratt, William K.; Cooper, Ted J.; Kabir, Ihtisham (1985-07-11).
      "Pseudomedian Filter". Architectures and Algorithms for Digital Image
      Processing II. 0534: 34. doi:10.1117/12.946562.
  38. ^Oja, Hannu (2010). Multivariate nonparametric methods with R: An
      approach based on spatial signs and ranks. Lecture Notes in Statistics.
      199. New York, NY: Springer. pp. xiv+232. doi:10.1007/978-1-4419-0468-3.
      ISBN 978-1-4419-0467-6. MR 2598854.
  39. ^Wilcox, Rand R. (2001), "TheilâSen estimator", Fundamentals_of_Modern
      Statistical_Methods:_Substantially_Improving_Power_and_Accuracy,
      Springer-Verlag, pp. 207â210, ISBN 978-0-387-95157-7
  40. .
  41. ^Wald, A. (1940). "The Fitting of Straight Lines if Both Variables are
      Subject to Error". Annals_of_Mathematical_Statistics. 11 (3): 282â300.
      doi:10.1214/aoms/1177731868. JSTOR 2235677.
  42. ^Nair, K. R.; Shrivastava, M. P. (1942). "On a Simple Method of Curve
      Fitting". SankhyÄ: The Indian Journal of Statistics. 6 (2): 121â132.
      JSTOR 25047749.
  43. ^Brown, G. W.; Mood, A. M. (1951). "On Median Tests for Linear
      Hypotheses". Proc Second Berkeley Symposium on Mathematical Statistics
      and Probability. Berkeley, CA: University of California Press.
      pp. 159â166. Zbl 0045.08606.
  44. ^Tukey, J. W. (1977). Exploratory Data Analysis. Reading, MA: Addison-
      Wesley. ISBN 0201076160.
  45. ^Brown, George W. (1947). "On Small-Sample Estimation". Annals_of
      Mathematical_Statistics. 18 (4): 582â585. doi:10.1214/aoms/1177730349.
      JSTOR 2236236.
  46. ^Lehmann,_Erich_L. (1951). "A General Concept of Unbiasedness". Annals_of
      Mathematical_Statistics. 22 (4): 587â592. doi:10.1214/aoms/1177729549.
      JSTOR 2236928.
  47. ^Birnbaum,_Allan (1961). "A Unified Theory of Estimation, I". Annals_of
      Mathematical_Statistics. 32 (1): 112â135. doi:10.1214/aoms/1177705145.
      JSTOR 2237612.
  48. ^van der Vaart, H. Robert (1961). "Some Extensions of the Idea of Bias".
      Annals_of_Mathematical_Statistics. 32 (2): 436â447. doi:10.1214/aoms/
      1177705051. JSTOR 2237754. MR 0125674.
  49. ^Pfanzagl, Johann; with the assistance of R. HambÃ¶ker (1994). Parametric
      Statistical Theory. Walter de Gruyter. ISBN 3-11-013863-8. MR 1291393.
  50. ^ Pfanzagl, Johann. "On optimal median unbiased estimators in the
      presence of nuisance parameters." The Annals of Statistics (1979):
      187â193.
  51. ^ Brown, L. D.; Cohen, Arthur; Strawderman, W. E. A Complete Class
      Theorem for Strict Monotone Likelihood Ratio With Applications. Ann.
      Statist. 4 (1976), no. 4, 712â722. doi:10.1214/aos/1176343543. http://
      projecteuclid.org/euclid.aos/1176343543.
  52. ^ Page 713: Brown, L. D.; Cohen, Arthur; Strawderman, W. E. A Complete
      Class Theorem for Strict Monotone Likelihood Ratio With Applications.
      Ann. Statist. 4 (1976), no. 4, 712â722. doi:10.1214/aos/1176343543.
      http://projecteuclid.org/euclid.aos/1176343543.
  53. ^ Talmud_and_Modern_Economics
  54. ^ Modern_Economic_Theory_in_the_Talmud by Yisrael_Aumann
  55. ^Stigler, S. M. (1986). The History of Statistics: The Measurement of
      Uncertainty Before 1900. Harvard University Press. ISBN 0674403401.
  56. ^Jaynes, E.T. (2007). Probability theory : the logic of science (5.
      print. ed.). Cambridge [u.a.]: Cambridge Univ. Press. p. 172. ISBN 978-0-
      521-59271-0.
  57. ^ Laplace PS de (1818) DeuxiÃ¨me supplÃ©ment Ã  la ThÃ©orie Analytique
      des ProbabilitÃ©s, Paris, Courcier
  58. ^Howarth, Richard (2017). Dictionary of Mathematical Geosciences: With
      Historical Notes. Springer. p. 374.
  59. ^ a b Keynes, J.M. (1921) A_Treatise_on_Probability. Pt II Ch XVII Â§5 (p
      201) (2006 reprint, Cosimo Classics,
  60. ISBN 9781596055308 : multiple other reprints)
  61. ^ Galton F (1881) "Report of the Anthropometric Committee" pp 245â260.
      Report_of_the_51st_Meeting_of_the_British_Association_for_the_Advancement
      of_Science
  62. ^ encyclopediaofmath.org
  63. ^ personal.psu.edu
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Median_(in_statistics)",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Median_as_a_weighted_arithmetic_mean_of_all_Sample_Observations
On-line_calculator
Calculating_the_median
A_problem_involving_the_mean,_the_median,_and_the_mode.
Weisstein,_Eric_W. "Statistical_Median". MathWorld.
Python_script for Median computations and income_inequality_metrics
Fast_Computation_of_the_Median_by_Successive_Binning
'Mean,_median,_mode_and_skewness', A tutorial devised for first-year psychology
students at Oxford University, based on a worked example.
This article incorporates material from Median_of_a_distribution on PlanetMath,
which is licensed under the Creative_Commons_Attribution/Share-Alike_License.
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
index.php?title=Median&oldid=909340863"
Categories:
    * Means
    * Robust_statistics
Hidden categories:
    * Webarchive_template_wayback_links
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_May_2012
    * Articles_with_unsourced_statements_from_October_2015
    * Wikipedia_articles_incorporating_text_from_PlanetMath
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
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * ChiShona
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Hrvatski
    * Ido
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
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
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 4 August 2019, at 20:00 (UTC).
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
