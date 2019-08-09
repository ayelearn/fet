The following text has been accessed from https://en.wikipedia.org/wiki/Sign_test at Fri Aug 9 02:53:37 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Sign test ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The sign test is a statistical method to test for consistent differences
between pairs of observations, such as the weight of subjects before and after
treatment. Given pairs of observations (such as weight pre- and post-treatment)
for each subject, the sign test determines if one member of the pair (such as
pre-treatment) tends to be greater than (or less than) the other member of the
pair (such as post-treatment).
The paired observations may be designated x and y. For comparisons of paired
observations (x,y), the sign test is most useful if comparisons can only be
expressed as x > y, x = y, or x < y. If, instead, the observations can be
expressed as numeric quantities (x = 7, y = 18), or as ranks (rank of x = 1st,
rank of y = 8th), then the paired t-test[1] or the Wilcoxon_signed-rank_test[2]
will usually have greater power than the sign test to detect consistent
differences.
If X and Y are quantitative variables, the sign test can be used to test_the
hypothesis that the difference between the X and Y has zero median, assuming
continuous distributions of the two random_variables X and Y, in the situation
when we can draw paired_samples from X and Y.[3]
The sign test can also test if the median of a collection of numbers is
significantly greater than or less than a specified value. For example, given a
list of student grades in a class, the sign test can determine if the median
grade is significantly different from, say, 75 out of 100.
The sign test is a non-parametric_test which makes very few assumptions about
the nature of the distributions under test â this means that it has very
general applicability but may lack the statistical_power of the alternative
tests.
The two conditions for the paired-sample sign test are that a sample must be
randomly selected from each population, and the samples must be dependent, or
paired. Independent samples cannot be meaningfully paired. Since the test is
nonparametric, the samples need not come from normally distributed populations.
Also, the test works for left-tailed, right-tailed, and two-tailed tests.
⁰
***** Contents *****
    * 1_Method
    * 2_Assumptions
    * 3_Significance_testing
    * 4_Example_of_two-sided_sign_test_for_matched_pairs
    * 5_Example_of_one-sided_sign_test_for_matched_pairs
    * 6_Example_of_sign_test_for_median_of_a_single_sample
    * 7_Examples_of_computer_software_for_the_sign_test
          o 7.1_Excel_software_for_the_sign_test
          o 7.2_R_software_for_the_sign_test
    * 8_History
    * 9_Relationship_to_other_statistical_tests
          o 9.1_Wilcoxon_signed-rank_test
          o 9.2_Paired_t-test
          o 9.3_McNemar's_test
          o 9.4_Friedman_test
          o 9.5_Trinomial_test
    * 10_See_also
    * 11_References
***** Method[edit] *****
Let p = Pr(X > Y), and then test the null_hypothesis H0: p = 0.50. In other
words, the null hypothesis states that given a random pair of measurements (xi,
yi), then xi and yi are equally likely to be larger than the other.
To test the null hypothesis, independent pairs of sample data are collected
from the populations {(x1, y1), (x2, y2), . . ., (xn, yn)}. Pairs are omitted
for which there is no difference so that there is a possibility of a reduced
sample of m pairs.[4]
Then let W be the number of pairs for which yi − xi > 0. Assuming that H0 is
true, then W follows a binomial_distribution W ~ b(m, 0.5).
***** Assumptions[edit] *****
Let Zi = Yi – Xi for i = 1, ... , n.
   1. The differences Zi are assumed to be independent.
   2. Each Zi comes from the same continuous population.
   3. The values Xi and Yi represent are ordered (at least the ordinal_scale),
      so the comparisons "greater than", "less than", and "equal to" are
      meaningful.
***** Significance testing[edit] *****
Since the test statistic is expected to follow a binomial_distribution, the
standard binomial_test is used to calculate significance. The normal
approximation_to_the_binomial_distribution can be used for large sample sizes,
m > 25.[4]
The left-tail value is computed by Pr(W â¤ w), which is the p-value for the
alternative H1: p < 0.50. This alternative means that the X measurements tend
to be higher.
The right-tail value is computed by Pr(W â¥ w), which is the p-value for the
alternative H1: p > 0.50. This alternative means that the Y measurements tend
to be higher.
For a two-sided alternative H1 the p-value is twice the smaller tail-value.
***** Example of two-sided sign test for matched pairs[edit] *****
Zar gives the following example of the sign test for matched pairs. Data are
collected on the length of the left hind leg and left foreleg for 10 deer.[5]
Deer Hind leg length (cm) Foreleg length (cm) Difference
1    142                  138                 +
2    140                  136                 +
3    144                  147                 â
4    144                  139                 +
5    142                  143                 â
6    146                  141                 +
7    149                  143                 +
8    150                  145                 +
9    142                  136                 +
10   148                  146                 +
The null hypothesis is that there is no difference between the hind leg and
foreleg length in deer. The alternative hypothesis is that there is a
difference between hind leg length and foreleg length. Note that this is a two-
tailed test, rather than a one-tailed test. For the two tailed test, the
alternative hypothesis is that hind leg length may be either greater than or
less than foreleg length. A one-sided test could be that hind leg length is
greater than foreleg length, so that the difference can only be in one
direction (greater than).
There are n=10 deer. There are 8 positive differences and 2 negative
differences. If the null hypothesis is true, that there is no difference in
hind leg and foreleg lengths, then the expected number of positive differences
is 5 out of 10. What is the probability that the observed result of 8 positive
differences, or a more extreme result, would occur if there is no difference in
leg lengths?
Because the test is two-sided, a result as extreme or more extreme than 8
positive differences includes the results of 8, 9, or 10 positive differences,
and the results of 0, 1, or 2 positive differences. The probability of 8 or
more positives among 10 deer or 2 or fewer positives among 10 deer is the same
as the probability of 8 or more heads or 2 or fewer heads in 10 flips of a fair
coin. The probabilities can be calculated using the binomial_test, with the
probability of heads = probability of tails = 0.5.
    * Probability of 0 heads in 10 flips of fair coin = 0.00098
    * Probability of 1 heads in 10 flips of fair coin = 0.00977
    * Probability of 2 heads in 10 flips of fair coin = 0.04395
    * Probability of 8 heads in 10 flips of fair coin = 0.04395
    * Probability of 9 heads in 10 flips of fair coin = 0.00977
    * Probability of 10 heads in 10 flips of fair coin = 0.00098
The two-sided probability of a result as extreme as 8 of 10 positive difference
is the sum of these probabilities:
      0.00098 + 0.00977 + 0.04395 + 0.04395 + 0.00977 + 0.00098 = 0.109375.
Thus, the probability of observing a results as extreme as 8 of 10 positive
differences in leg lengths, if there is no difference in leg lengths, is
p = 0.109375. The null hypothesis is not rejected at a significance level of
p = 0.05. With a larger sample size, the evidence might be sufficient to reject
the null hypothesis.
Because the observations can be expressed as numeric quantities (actual leg
length), the paired t-test or Wilcoxon signed rank test will usually have
greater power than the sign test to detect consistent differences. For this
example, the paired t-test for differences indicates that there is a
significant difference between hind leg length and foreleg length (p = 0.007).
If the observed result was 9 positive differences in 10 comparisons, the sign
test would be significant. Only coin flips with 0, 1, 9, or 10 heads would be
as extreme as or more extreme than the observed result.
    * Probability of 0 heads in 10 flips of fair coin = 0.00098
    * Probability of 1 heads in 10 flips of fair coin = 0.00977
    * Probability of 9 heads in 10 flips of fair coin = 0.00977
    * Probability of 10 heads in 10 flips of fair coin = 0.00098
The probability of a result as extreme as 9 of 10 positive difference is the
sum of these probabilities:
      0.00098 + 0.00977 + 0.00977 + 0.00098 = 0.0215.
In general, 8 of 10 positive differences is not significant (p = 0.11), but 9
of 10 positive differences is significant (p = 0.0215).
***** Example of one-sided sign test for matched pairs[edit] *****
Conover[6] gives the following example using a one-sided sign test for matched
pairs. A manufacturer produces two products, A and B. The manufacturer wishes
to know if consumers prefer product B over product A. A sample of 10 consumers
are each given product A and product B, and asked which product they prefer.
The null hypothesis is that consumers do not prefer product B over product A.
The alternative hypothesis is that consumers prefer product B over product A.
Note that this is a one-sided (directional) test.
At the end of the study, 8 consumers preferred product B, 1 consumer preferred
product A, and one reported no preference.
    * Number of +'s (preferred B) = 8
    * Number of â's (preferred A) = 1
    * Number of ties (no preference) = 1
The tie is excluded from the analysis, giving n = number of +'s and â's =
8 + 1 = 9.
What is the probability of a result as extreme as 8 positives in favor of B in
9 pairs, if the null hypothesis is true, that consumers have no preference for
B over A? This is the probability of 8 or more heads in 9 flips of a fair coin,
and can be calculated using the binomial distribution with p(heads) = p(tails)
= 0.5.
P(8 or 9 heads in 9 flips of a fair coin) = 0.0195. The null hypothesis is
rejected, and the manufacturer concludes that consumers prefer product B over
product A.
***** Example of sign test for median of a single sample[edit] *****
Sprent [7] gives the following example of a sign test for a median. In a
clinical trial, survival time (weeks) is collected for 10 subjects with non-
Hodgkins lymphoma. The exact survival time was not known for one subject who
was still alive after 362 weeks, when the study ended. The subjects' survival
times were
      49, 58, 75, 110, 112, 132, 151, 276, 281, 362+
The plus sign indicates the subject still alive at the end of the study. The
researcher wished to determine if the median survival time was less than or
greater than 200 weeks.
The null hypothesis is that median survival is 200 weeks. The alternative
hypothesis is that median survival is not 200 weeks. Notice that this is a two-
sided test: the alternative median may be greater than or less than 200 weeks.
If the null hypothesis is true, that the median survival is 200 weeks, then, in
a random sample approximately half the subjects should survive less than 200
weeks, and half should survive more than 200 weeks. Observations below 200 are
assigned a minus (â); observations above 200 are assigned a plus (+). For the
subject survival times, there are 7 observations below 200 weeks (â) and 3
observations above 200 weeks (+) for the n=10 subjects.
Because any one observation is equally likely to be above or below the
population median, the number of plus scores will have a binomial distribution
with mean = 0.5. What is the probability of a result as extreme as 7 in 10
subjects being below the median? This is exactly the same as the probability of
a result as extreme as 7 heads in 10 tosses of a fair coin. Because this is a
two-sided test, an extreme result can be either three or fewer heads or seven
or more heads.
The probability of observing k heads in 10 tosses of a fair coin, with p(heads)
= 0.5, is given by the binomial formula:
      Pr(Number of heads = k) = Choose(10, k) Ã 0.5^10
The probability for each value of k is given in the table below.
k  0      1      2      3      4      5      6      7      8      9      10
Pr 0.0010 0.0098 0.0439 0.1172 0.2051 0.2461 0.2051 0.1172 0.0439 0.0098 0.0010
The probability of 0, 1, 2, 3, 7, 8, 9, or 10 heads in 10 tosses is the sum of
their individual probabilities:
      0.0010 + 0.0098 + 0.0439 + 0.1172 + 0.1172 + 0.0439 + 0.0098 + 0.0010 =
      0.3438.
Thus, the probability of observing 3 or fewer plus signs or 7 or more plus
signs in the survival data, if the median survival is 200 weeks, is 0.3438. The
expected number of plus signs is 5 if the null hypothesis is true. Observing 3
or fewer, or 7 or more pluses is not significantly different from 5. The null
hypothesis is not rejected. Because of the extremely small sample size, this
sample has low power to detect a difference.
***** Examples of computer software for the sign test[edit] *****
The sign test is a special case of the binomial test where the probability of
success under the null hypothesis is p=0.5. Thus, the sign test can be
performed using the binomial test, which is provided in most statistical
software programs. On-line calculators for the sign test can be founded by
searching for "sign test calculator". Many websites offer the binomial test,
but generally offer only a two-sided version.
**** Excel software for the sign test[edit] ****
A template for the sign test using Excel is available at http://www.real-
statistics.com/non-parametric-tests/sign-test/
**** R software for the sign test[edit] ****
In R, the binomial test can be performed using the function binom.test().
The syntax for the function is
binom.test(x, n, p = 0.5, alternative = c("two.sided", "less", "greater"),
conf.level = 0.95)
where
    * x = number of successes, or a vector of length 2 giving the numbers of
      successes and failures, respectively
    * n = number of trials; ignored if x has length 2
    * p = hypothesized probability of success
    * alternative =indicates the alternative hypothesis and must be one of
      "two.sided", "greater" or "less"
    * conf.level = confidence level for the returned confidence interval.
Examples of the sign test using the R function binom.test
The sign test example from Zar [5] compared the length of hind legs and
forelegs of deer. The hind leg was longer than the foreleg in 8 of 10 deer.
Thus, there are x=8 successes in n=10 trials. The hypothesized probability of
success (defined as hind leg longer than foreleg) is p = 0.5 under the null
hypothesis that hind legs and forelegs do not differ in length. The alternative
hypothesis is that hind leg length may be either greater than or less than
foreleg length, which is a two sided test, specified as
alternative="two.sided".
The R command binom.test(x=8, n=10, p=0.5, alternative="two.sided") gives
p=0.1094, as in the example.
The sign test example in Conover [6] examined consumer preference for product A
vs. product B. The null hypothesis was that consumers do not prefer product B
over product A. The alternative hypothesis was that consumers prefer product B
over product A, a one-sided test. In the study, 8 of 9 consumers who expressed
a preference preferred product B over product A.
The R command binom.test(x=8, n=9, p=0.5, alternative="greater") gives
p=0.01953, as in the example.
***** History[edit] *****
See also: History_of_statistics
Conover [6] and Sprent [7] describe John_Arbuthnot's use of the sign test in
1710. Arbuthnot examined birth records in London for each of the 82 years from
1629 to 1710. In every year, the number of males born in London exceeded the
number of females. If the null hypothesis of equal number of births is true,
the probability of the observed outcome is 1/282, leading Arbuthnot to conclude
that the probability of male and female births were not exactly equal.
For his publications in 1692 and 1710, Arbuthnot is credited with "â¦ the
first use of significance tests â¦" [8] , the first example of reasoning about
statistical significance and moral certainty, [9] and "â¦ perhaps the first
published report of a nonparametric test â¦".[6]
Hald [9] further describes the impact of Arbuthnot's research.
"Nicholas Bernoulli (1710â1713) completes the analysis of Arbuthnot's data by
showing that the larger part of the variation of the yearly number of male
births can be explained as binomial with p = 18/35. This is the first example
of fitting a binomial to data. Hence we here have a test of significance
rejecting the hypothesis p = 0.5 followed by an estimation of p and a
discussion of the goodness of fit â¦"
***** Relationship to other statistical tests[edit] *****
**** Wilcoxon signed-rank test[edit] ****
The sign test requires only that the observations in a pair be ordered, for
example x > y. In some cases, the observations for all subjects can be assigned
a rank value (1, 2, 3, ...). If the observations can be ranked, and each
observation in a pair is a random sample from a symmetric distribution, then
the Wilcoxon_signed-rank_test is appropriate. The Wilcoxon test will generally
have greater power to detect differences than the sign test. The asymptotic
relative_efficiency of the sign test to the Wilcoxon signed rank test, under
these circumstances, is 0.67.[6]
**** Paired t-test[edit] ****
If the paired observations are numeric quantities (such as the actual length of
the hind leg and foreleg in the Zar example), and the differences between
paired observations are random samples from a single normal distribution, then
the paired_t-test is appropriate. The paired t-test will generally have greater
power to detect differences than the sign test. The asymptotic relative
efficiency of the sign test to the paired t-test, under these circumstances, is
0.637. However, if the distribution of the differences between pairs is not
normal, but instead is heavy-tailed (platykurtic_distribution), the sign test
can have more power than the paired t-test, with asymptotic_relative_efficiency
of 2.0 relative to the paired t-test and 1.3 relative to the Wilcoxon signed
rank test.[6]
**** McNemar's test[edit] ****
In some applications, the observations within each pair can only take the
values 0 or 1. For example, 0 may indicate failure and 1 may indicate success.
There are 4 possible pairs: {0,0}, {0,1}, {1,0}, and {1,1}. In these cases, the
same procedure as the sign test is used, but is known as McNemar's_test.[6]
**** Friedman_test[edit] ****
Instead of paired observations such as (Product A, Product B), the data may
consist of three or more levels (Product A, Product B, Product C). If the
individual observations can be ordered in the same way as for the sign test,
for example B > C > A, then the Friedman_test may be used.[5]
**** Trinomial test[edit] ****
Bian, McAleer and Wong[10] proposed in 2011 a non-parametric test for paired
data when there are many ties. They showed that their trinomial test is
superior to the sign test in presence of ties.
***** See also[edit] *****
    * Wilcoxon_signed-rank_test â A more powerful variant of the sign test,
      but one which also assumes a symmetric distribution and interval data.
    * Median_test â An unpaired alternative to the sign test.
***** References[edit] *****
   1. ^Baguley, Thomas (2012), Serious_Stats:_A_Guide_to_Advanced_Statistics
      for_the_Behavioral_Sciences, Palgrave Macmillan, p. 281,
      ISBN 9780230363557
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
   3. .
   4. ^Corder, Gregory W.; Foreman, Dale I. (2014), "3.6_Statistical_Power",
      Nonparametric Statistics: A Step-by-Step Approach (2nd ed.), John Wiley &
      Sons, ISBN 9781118840429
   5. .
   6. ^ The_Sign_Test_for_a_Median // STAT 415 Intro Mathematical Statistics.
      Penn State University.
   7. ^ a bMendenhall W, Wackerly DD, Scheaffer RL (1989), "15: Nonparametric
      statistics", Mathematical statistics with applications (Fourth ed.), PWS-
      Kent, pp. 674â679, ISBN 0-534-92026-8
   8. ^ a b cZar, Jerold H. (1999), "Chapter 24: More on Dichotomous
      Variables", Biostatistical Analysis (Fourth ed.), Prentice-Hall,
      pp. 516â570, ISBN 0-13-081542-X
   9. ^ a b c d e f gConover, W.J. (1999), "Chapter 3.4: The Sign Test",
      Practical Nonparametric Statistics (Third ed.), Wiley, pp. 157â176,
      ISBN 0-471-16068-7
  10.
  11. ^ a bSprent, P. (1989), Applied Nonparametric Statistical Methods (Second
      ed.), Chapman & Hall, ISBN 0-412-44980-3
  12. ^Bellhouse, P. (2001), "John Arbuthnot", in Statisticians of the
      Centuries by C.C. Heyde and E. Seneta, Springer, pp. 39â42, ISBN 0-387-
      95329-9
  13. ^ a bHald, Anders (1998), "Chapter 4. Chance or Design: Tests of
      Significance", A History of Mathematical Statistics from 1750 to 1930,
      Wiley, p. 65
  14. ^Bian G, McAleer M, Wong WK (2011), A trinomial test for paired data when
      there are many ties., Mathematics and Computers in Simulation, 81(6),
      pp. 1153â1160
    * Gibbons,_J.D. and Chakraborti, S. (1992). Nonparametric Statistical
      Inference. Marcel Dekker Inc., New York.
    * Kitchens, L.J.(2003). Basic Statistics and Data Analysis. Duxbury.
    * Conover, W. J. (1980). Practical Nonparametric Statistics, 2nd ed. Wiley,
      New York.
    * Lehmann, E. L. (1975). Nonparametrics: Statistical Methods Based on
      Ranks. Holden and Day, San Francisco.
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
index.php?title=Sign_test&oldid=904417969"
Categories:
    * Statistical_tests
    * Nonparametric_statistics
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
    * Deutsch
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * Nederlands
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
Edit_links
    * This page was last edited on 2 July 2019, at 01:08 (UTC).
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
