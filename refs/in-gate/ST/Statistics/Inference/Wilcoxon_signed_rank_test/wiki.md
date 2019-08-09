The following text has been accessed from https://en.wikipedia.org/wiki/Wilcoxon_signed-rank_test at Fri Aug 9 02:53:35 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Wilcoxon signed-rank test ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The Wilcoxon signed-rank test is a non-parametric statistical_hypothesis_test
used to compare two related samples, matched samples, or repeated measurements
on a single sample to assess whether their population mean ranks differ (i.e.
it is a paired_difference_test). It can be used as an alternative to the paired
Student's_t-test (also known as "t-test for matched pairs" or "t-test for
dependent samples") when the population cannot be assumed to be normally
distributed.[1] A Wilcoxon signed-rank test is a nonparametric test that can be
used to determine whether two dependent samples were selected from populations
having the same distribution.
⁰
***** Contents *****
    * 1_History
    * 2_Assumptions
    * 3_Test_procedure
          o 3.1_Example
          o 3.2_Historical_T_statistic
    * 4_Limitation
    * 5_Effect_size
    * 6_Software_implementations
    * 7_See_also
    * 8_References
    * 9_External_links
***** History[edit] *****
The test is named for Frank_Wilcoxon (1892â1965) who, in a single paper,
proposed both it and the rank-sum_test for two independent samples (Wilcoxon,
1945).[2] The test was popularized by Sidney_Siegel (1956) in his influential
textbook on non-parametric statistics.[3] Siegel used the symbol T for a value
related to, but not the same as,     W   {\displaystyle W}  [W]. In
consequence, the test is sometimes referred to as the Wilcoxon T test, and the
test statistic is reported as a value of T.
***** Assumptions[edit] *****
   1. Data are paired and come from the same population.
   2. Each pair is chosen randomly and independently[citation_needed].
   3. The data are measured on at least an interval_scale when, as is usual,
      within-pair differences are calculated to perform the test (though it
      does suffice that within-pair comparisons are on an ordinal_scale).
***** Test procedure[edit] *****
Let     N   {\displaystyle N}  [N] be the sample size, i.e., the number of
pairs. Thus, there are a total of 2N data points. For pairs     i = 1 , . . . ,
N   {\displaystyle i=1,...,N}  [i = 1, ..., N], let      x  1 , i
{\displaystyle x_{1,i}}  [x_{1,i}] and      x  2 , i     {\displaystyle x_
{2,i}}  [x_{2,i}] denote the measurements.
      H0: difference between the pairs follows a symmetric distribution around
      zero
      H1: difference between the pairs does not follow a symmetric distribution
      around zero.
   1. For     i = 1 , . . . , N   {\displaystyle i=1,...,N}  [i = 1, ..., N],
      calculate      |   x  2 , i   &#x2212;  x  1 , i    |    {\displaystyle
      |x_{2,i}-x_{1,i}|}  [|x_{2,i} - x_{1,i}|] and     sgn &#x2061; (  x  2 ,
      i   &#x2212;  x  1 , i   )   {\displaystyle \operatorname {sgn} (x_{2,i}-
      x_{1,i})}  [\sgn(x_{2,i} - x_{1,i})], where     sgn   {\displaystyle
      \operatorname {sgn} }  [\operatorname {sgn} ] is the sign_function.
   2. Exclude pairs with      |   x  2 , i   &#x2212;  x  1 , i    |  = 0
      {\displaystyle |x_{2,i}-x_{1,i}|=0}  [|x_{2,i} - x_{1,i}| = 0]. Let
      N  r     {\displaystyle N_{r}}  [N_r] be the reduced sample size.
   3. Order the remaining      N  r     {\displaystyle N_{r}}  [N_r] pairs from
      smallest absolute difference to largest absolute difference,      |   x
      2 , i   &#x2212;  x  1 , i    |    {\displaystyle |x_{2,i}-x_{1,i}|}
      [|x_{2,i} - x_{1,i}|].
   4. Rank the pairs, starting with the pair with the smallest non-zero
      absolute difference as 1. Ties receive a rank equal to the average of the
      ranks they span. Let      R  i     {\displaystyle R_{i}}  [R_{i}] denote
      the rank.
   5. Calculate the test_statistic     W   {\displaystyle W}  [W]
               W =  &#x2211;  i = 1    N  r     [ sgn &#x2061; (  x  2 , i
            &#x2212;  x  1 , i   ) &#x22C5;  R  i   ]   {\displaystyle W=\sum _
            {i=1}^{N_{r}}[\operatorname {sgn}(x_{2,i}-x_{1,i})\cdot R_{i}]}
            [W=\sum _{{i=1}}^{{N_{r}}}[\operatorname{sgn}(x_{{2,i}}-x_{
            {1,i}})\cdot R_{i}]], the sum of the signed ranks.
   6. Under null hypothesis,     W   {\displaystyle W}  [W] follows a specific
      distribution with no simple expression. This distribution has an expected
      value of 0 and a variance of         N  r   (  N  r   + 1 ) ( 2  N  r   +
      1 )  6     {\displaystyle {\frac {N_{r}(N_{r}+1)(2N_{r}+1)}{6}}}  [{\frac
      {N_{r}(N_{r}+1)(2N_{r}+1)}{6}}].
               W   {\displaystyle W}  [W] can be compared to a critical value
            from a reference table.[1]
            The two-sided test consists in rejecting      H  0
            {\displaystyle H_{0}}  [H_{0}] if      |  W  |  >  W  c r i t i c a
            l ,  N  r       {\displaystyle |W|>W_{critical,N_{r}}}  [
            {\displaystyle |W|>W_{critical,N_{r}}}].
   7. As      N  r     {\displaystyle N_{r}}  [N_r] increases, the sampling
      distribution of     W   {\displaystyle W}  [W] converges to a normal
      distribution. Thus,
            For      N  r   &#x2265; 20   {\displaystyle N_{r}\geq 20}  [
            {\displaystyle N_{r}\geq 20}], a z-score can be calculated as     z
            =   W  &#x03C3;  W       {\displaystyle z={\frac {W}{\sigma _{W}}}}
            [{\displaystyle z={\frac {W}{\sigma _{W}}}}], where      &#x03C3;
            W   =      N  r   (  N  r   + 1 ) ( 2  N  r   + 1 )  6
            {\displaystyle \sigma _{W}={\sqrt {\frac {N_{r}(N_{r}+1)(2N_{r}+1)}
            {6}}}}  [{\displaystyle \sigma _{W}={\sqrt {\frac {N_{r}(N_{r}+1)
            (2N_{r}+1)}{6}}}}].
            To perform a two-sided test, reject      H  0     {\displaystyle H_
            {0}}  [H_{0}] if      z  c r i t i c a l   <  |  z  |
            {\displaystyle z_{critical}<|z|}  [{\displaystyle z_
            {critical}<|z|}].
            Alternatively, one-sided tests can be performed with either the
            exact or the approximate distribution. p-values can also be
            calculated.
   8. For      N  r   < 20   {\displaystyle N_{r}<20}  [{\displaystyle N_
      {r}<20}] the exact distribution needs to be used.

**** Example[edit] ****
                                                 x  2 , i   &#x2212;  x  1                                                             x  2 , i   &#x2212;  x  1 , i     {\displaystyle x_
                                             , i     {\displaystyle x_                                                             {2,i}-x_{1,i}}  [x_{2,i} - x_{1,i}]
                                             {2,i}-x_{1,i}}  [x_{2,i} - x_                               x  2 , i       x  1 , i      sgn                                          sgn
   i               x  2 , i       x  1 , i   {1,i}]                                      i           {\displaystyle {\displaystyle {\displaystyle     abs            R  i       &#x22C5;  R  i
{\displaystyle {\displaystyle {\displaystyle    sgn                                   {\displaystyle x_{2,i}}  [x_  x_{1,i}}  [x_  \operatorname  {\displaystyle {\displaystyle {\displaystyle
i}  [i]        x_{2,i}}  [x_  x_{1,i}}  [x_  {\displaystyle     abs                   i}  [i]        {2,i}]         {1,i}]         {sgn} }        {\text{abs}}}  R_{i}}  [R_    \operatorname
               {2,i}]         {1,i}]         \operatorname  {\displaystyle                                                         [\operatorname [\text{abs}]   {i}]           {sgn} \cdot R_
                                             {sgn} }        {\text{abs}}}                                                          {sgn} ]                                      {i}}  [\sgn
                                             [\operatorname [\text{abs}]   order by                                                                                             \cdot R_i]
                                             {sgn} ]                       absolute   5              140            140                          0                             
1              125            110            1              15             difference 3              130            125            1              5              1.5            1.5
2              115            122             â1      7                         9              140            135            1              5              1.5            1.5
3              130            125            1              5                         2              115            122             â1      7              3               â3
4              140            120            1              20                        6              115            124             â1      9              4               â4
5              140            140                          0                         10             135            145             â1      10             5               â5
6              115            124             â1      9                         8              125            137             â1      12             6               â6
7              140            123            1              17                        1              125            110            1              15             7              7
8              125            137             â1      12                        7              140            123            1              17             8              8
9              140            135            1              5                         4              140            120            1              20             9              9
10             135            145             â1      10

    sgn   {\displaystyle \operatorname {sgn} }  [\operatorname {sgn} ] is the
sign_function,      abs    {\displaystyle {\text{abs}}}  [\text{abs}] is the
absolute_value, and      R  i     {\displaystyle R_{i}}  [R_{i}] is the rank.
Notice that pairs 3 and 9 are tied in absolute value. They would be ranked 1
and 2, so each gets the average of those ranks, 1.5.
         W = 1.5 + 1.5 &#x2212; 3 &#x2212; 4 &#x2212; 5 &#x2212; 6 + 7 + 8 + 9
      = 9   {\displaystyle W=1.5+1.5-3-4-5-6+7+8+9=9}  [{\displaystyle
      W=1.5+1.5-3-4-5-6+7+8+9=9}]
          |  W  |  <  W  c r i t ( &#x03B1; = 0.05 , &#xA0; 9  , two-sided  )
      = 33   {\displaystyle |W|<W_{crit(\alpha =0.05,\ 9{\text{, two-
      sided}})}=33}  [{\displaystyle |W|<W_{crit(\alpha =0.05,\ 9{\text{, two-
      sided}})}=33}]
         &#x2234;  failed to reject&#xA0;   H  0     {\displaystyle \therefore
      {\text{failed to reject }}H_{0}}  [{\displaystyle \therefore {\text
      {failed to reject }}H_{0}}] that the two medians are the same.
      The     p   {\displaystyle p}  [p]-value for this result is     0.6113
      {\displaystyle 0.6113}  [{\displaystyle 0.6113}]
**** Historical T statistic[edit] ****
In historical sources a different statistic, denoted by Siegel as the T
statistic, was used. The T statistic is the smaller of the two sums of ranks of
given sign; in the example, therefore, T would equal 3+4+5+6=18. Low values of
T are required for significance. T is easier to calculate by hand than W and
the test is equivalent to the two-sided test described above; however, the
distribution of the statistic under      H  0     {\displaystyle H_{0}}  [H_
{0}] has to be adjusted.
         T >  T  c r i t ( &#x03B1; = 0.05 , &#xA0; 9  , two-sided  )   = 5
      {\displaystyle T>T_{crit(\alpha =0.05,\ 9{\text{, two-sided}})}=5}  [
      {\displaystyle T>T_{crit(\alpha =0.05,\ 9{\text{, two-sided}})}=5}]
         &#x2234;  failed to reject&#xA0;   H  0     {\displaystyle \therefore
      {\text{failed to reject }}H_{0}}  [{\displaystyle \therefore {\text
      {failed to reject }}H_{0}}] that the two medians are the same.
Note: Critical T values (     T  c r i t     {\displaystyle T_{crit}}  [
{\displaystyle T_{crit}}]) by values of      N  r     {\displaystyle N_{r}}
[N_r] can be found in appendices of statistics textbooks, for example in Table
B-3 of Nonparametric Statistics: A Step-by-Step Approach, 2nd Edition by Dale
I. Foreman and Gregory W. Corder (https://www.oreilly.com/library/view/
nonparametric-statistics-a/9781118840429/bapp02.xhtml).
***** Limitation[edit] *****
As demonstrated in the example, when the difference between the groups is zero,
the observations are discarded. This is of particular concern if the samples
are taken from a discrete distribution. In these scenarios the modification to
the Wilcoxon test by Pratt 1959, provides an alternative which incorporates the
zero differences.[4][5] This modification is more robust for data on an ordinal
scale.[5]
***** Effect size[edit] *****
Main article: MannâWhitney_U_test_Â§ Rank-biserial_correlation
To compute an effect_size for the signed-rank test, one can use the rank-
biserial_correlation.
If the test statistic W is reported, the rank correlation r is equal to the
test statistic W divided by the total rank sum S, or r = W/S. [6] Using the
above example, the test statistic is W = 9. The sample size of 9 has a total
rank sum of S = (1 + 2 + 3 + 4 + 5 + 6 + 7 + 8 + 9) = 45. Hence, the rank
correlation is 9/45, so r = 0.20.
If the test statistic T is reported, an equivalent way to compute the rank
correlation is with the difference in proportion between the two rank sums,
which is the Kerby (2014) simple difference formula.[6] To continue with the
current example, the sample size is 9, so the total rank sum is 45. T is the
smaller of the two rank sums, so T is 3 + 4 + 5 + 6 = 18. From this information
alone, the remaining rank sum can be computed, because it is the total sum S
minus T, or in this case 45 - 18 = 27. Next, the two rank-sum proportions are
27/45 = 60% and 18/45 = 40%. Finally, the rank correlation is the difference
between the two proportions (.60 minus .40), hence r = .20.
***** Software implementations[edit] *****
    * R includes an implementation of the test as wilcox.test(x,y,
      paired=TRUE), where x and y are vectors of equal length.[7]
    * ALGLIB includes implementation of the Wilcoxon signed-rank test in C++,
      C#, Delphi, Visual Basic, etc.
    * GNU_Octave implements various one-tailed and two-tailed versions of the
      test in the wilcoxon_test function.
    * SciPy includes an implementation of the Wilcoxon signed-rank test in
      Python
    * Accord.NET includes an implementation of the Wilcoxon signed-rank test in
      C# for .NET applications
    * MATLAB implements this test using "Wilcoxon rank sum test" as [p,h] =
      signrank(x,y) also returns a logical value indicating the test decision.
      The result h = 1 indicates a rejection of the null hypothesis, and h = 0
      indicates a failure to reject the null hypothesis at the 5% significance
      level
***** See also[edit] *****
    * MannâWhitneyâWilcoxon_test (the variant for two independent samples)
    * Sign_test (Like Wilcoxon test, but without the assumption of symmetric
      distribution of the differences around the median, and without using the
      magnitude of the difference)
***** References[edit] *****
   1. ^ a bLowry, Richard. "Concepts_&_Applications_of_Inferential_Statistics".
      Retrieved 5 November 2018.
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
   3. ^Wilcoxon, Frank (Dec 1945). "Individual_comparisons_by_ranking_methods"
      (PDF). Biometrics Bulletin. 1 (6): 80â83. doi:10.2307/3001968.
      JSTOR 3001968.
   4. ^Siegel, Sidney (1956). Non-parametric_statistics_for_the_behavioral
      sciences. New York: McGraw-Hill. pp. 75â83.
   5. ^Pratt, J (1959). "Remarks on zeros and ties in the Wilcoxon signed rank
      procedures". Journal of the American Statistical Association. 54 (287):
      655â667. doi:10.1080/01621459.1959.10501526.
   6. ^ a bDerrick, B; White, P (2017). "Comparing Two Samples from an
      Individual Likert Question". International Journal of Mathematics and
      Statistics. 18 (3): 1â13.
   7. ^ a bKerby, Dave S. (2014), "The simple difference formula: An approach
      to teaching nonparametric correlation.", Comprehensive Psychology, 3:
      11.IT.3.1, doi:10.2466/11.IT.3.1
   8. ^Dalgaard, Peter (2008). Introductory_Statistics_with_R. Springer Science
      & Business Media. pp. 99â100. ISBN 978-0-387-79053-4.
***** External links[edit] *****
    * Wilcoxon_Signed-Rank_Test_in_R
    * Example_of_using_the_Wilcoxon_signed-rank_test
    * An_online_version_of_the_test
    * A_table_of_critical_values_for_the_Wilcoxon_signed-rank_test
    * Brief_guide_by_experimental_psychologist_Karl_L._Weunsch - Nonparametric
      effect size estimators (Copyright 2015 by Karl L. Weunsch)
    * Kerby, D. S. (2014). The simple difference formula: An approach to
      teaching nonparametric correlation. Comprehensive Psychology, volume 3,
      article 1. doi:10.2466/11.IT.3.1. link_to_article
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
                           * Signed rank (Wilcoxon)
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

Retrieved from "https://en.wikipedia.org/w/index.php?title=Wilcoxon_signed-
rank_test&oldid=909176560"
Categories:
    * Statistical_tests
    * Nonparametric_statistics
    * U-statistics
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_February_2017
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
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
Edit_links
    * This page was last edited on 3 August 2019, at 17:09 (UTC).
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
