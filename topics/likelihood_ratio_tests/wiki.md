The following text has been accessed from https://en.wikipedia.org/wiki/Likelihood-ratio_test at Fri Aug 9 02:53:49 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Likelihood-ratio test ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Statistical test used for comparing the goodness of fit of two statistical
models
Not to be confused with the use of likelihood_ratios_in_diagnostic_testing.
In statistics, the likelihood-ratio test assesses the goodness_of_fit of two
competing statistical_models based on the ratio of their likelihoods,
specifically one found by maximization over the entire parameter_space and
another found after imposing some constraint. If the constraint (i.e., the null
hypothesis) is supported by the observed_data, the two likelihoods should not
differ by more than sampling_error.[1] Thus the likelihood-ratio test tests
whether this ratio is significantly_different from one, or equivalently whether
its natural_logarithm is significantly different from zero.
The likelihood-ratio test is the oldest of the three classical approaches to
hypothesis testing, together with the Lagrange_multiplier_test and the Wald
test.[2] In fact, the latter two can be conceptualized as approximations to the
likelihood-ratio test, and are asymptotically equivalent.[3][4][5] In the case
of comparing two models each of which has no unknown parameters, use of the
likelihood-ratio test can be justified by the NeymanâPearson_lemma. The lemma
demonstrates that the test has the highest power among all competitors.[6]
⁰
***** Contents *****
    * 1_Definition
          o 1.1_General
          o 1.2_Case_of_simple_hypotheses
    * 2_Interpretation
          o 2.1_An_example
    * 3_Asymptotic_distribution:_Wilksâ_theorem
    * 4_See_also
    * 5_References
    * 6_Further_reading
    * 7_External_links
***** Definition[edit] *****
**** General[edit] ****
Suppose that we have a statistical_model with parameter_space     &#x0398;
{\displaystyle \Theta }  [\Theta ]. A null_hypothesis is often stated by saying
that the parameter     &#x03B8;   {\displaystyle \theta }  [\theta ] is in a
specified subset      &#x0398;  0     {\displaystyle \Theta _{0}}  [\Theta_0]
of     &#x0398;   {\displaystyle \Theta }  [\Theta ]. The alternative
hypothesis is thus that     &#x03B8;   {\displaystyle \theta }  [\theta ] is in
the complement of      &#x0398;  0     {\displaystyle \Theta _{0}}  [\Theta_0],
i.e. in     &#x0398; &#x2216;  &#x0398;  0     {\displaystyle \Theta
\smallsetminus \Theta _{0}}  [{\displaystyle \Theta \smallsetminus \Theta _
{0}}], which is denoted by      &#x0398;  0   &#x2201;     {\displaystyle
\Theta _{0}^{\complement }}  [{\displaystyle \Theta _{0}^{\complement }}]. The
likelihood ratio test statistic for the null hypothesis      H  0    :
&#x03B8; &#x2208;  &#x0398;  0     {\displaystyle H_{0}\,:\,\theta \in \Theta _
{0}}  [{\displaystyle H_{0}\,:\,\theta \in \Theta _{0}}] is given by:[7]
         L R = &#x2212; 2 ln &#x2061;  [     sup  &#x03B8; &#x2208;  &#x0398;
      0       L   ( &#x03B8; )    sup  &#x03B8; &#x2208; &#x0398;     L
      ( &#x03B8; )    ]    {\displaystyle LR=-2\ln \left[{\frac {\sup _{\theta
      \in \Theta _{0}}{\mathcal {L}}(\theta )}{\sup _{\theta \in \Theta }
      {\mathcal {L}}(\theta )}}\right]}  [{\displaystyle LR=-2\ln \left[{\frac
      {\sup _{\theta \in \Theta _{0}}{\mathcal {L}}(\theta )}{\sup _{\theta \in
      \Theta }{\mathcal {L}}(\theta )}}\right]}]
where the quantity inside the brackets is called the likelihood ratio. Here,
the     sup   {\displaystyle \sup }  [\sup ] notation refers to the supremum
function. As all likelihoods are positive, and as the constrained maximum
cannot exceed the unconstrained maximum, the likelihood ratio is bounded
between zero and one.
Often the likelihood-ratio test statistic is expressed as a difference between
the log-likelihoods,     L R = &#x2212; 2  [  &#x2113; (  &#x03B8;  0   )
&#x2212; &#x2113; (    &#x03B8; &#x005E;    )  ]    {\displaystyle LR=-2\left
[\ell (\theta _{0})-\ell ({\hat {\theta }})\right]}  [{\displaystyle LR=-2\left
[\ell (\theta _{0})-\ell ({\hat {\theta }})\right]}], where      &#x03B8;  0
&#x2208;  &#x0398;  0     {\displaystyle \theta _{0}\in \Theta _{0}}  [
{\displaystyle \theta _{0}\in \Theta _{0}}] and        &#x03B8; &#x005E;
&#x2208; &#x0398;   {\displaystyle {\hat {\theta }}\in \Theta }  [
{\displaystyle {\hat {\theta }}\in \Theta }] denote the respective arguments_of
the_maxima. The reason for multiplying by negative two is mathematical so that,
by Wilks'_theorem,     L R   {\displaystyle LR}  [LR] has an asymptotic Ï2-
distribution under the null hypothesis.[8] The finite_sample_distributions of
likelihood-ratio tests are generally unknown.[9]
The likelihood-ratio test requires that the models be nested—i.e. the more
complex model can be transformed into the simpler model by imposing constraints
on the former's parameters. Many common test statistics are tests for nested
models and can be phrased as log-likelihood ratios or approximations thereof:
e.g. the Z-test, the F-test, the G-test, and Pearson's_chi-squared_test; for an
illustration with the one-sample_t-test, see below.
If the models are not nested, then instead of the likelihood-ratio test, there
is a generalization of the test that can usually be used: for details, see
relative_likelihood.
**** Case of simple hypotheses[edit] ****
Main article: NeymanâPearson_lemma
A simple-vs.-simple hypothesis test has completely specified models under both
the null hypothesis and the alternative hypothesis, which for convenience are
written in terms of fixed values of a notional parameter     &#x03B8;
{\displaystyle \theta }  [\theta ]:
              H  0      :   &#x03B8; =  &#x03B8;  0   ,      H  1      :
      &#x03B8; =  &#x03B8;  1   .       {\displaystyle {\begin{aligned}H_{0}&:
      &\theta =\theta _{0},\\H_{1}&:&\theta =\theta _{1}.\end{aligned}}}  [
      \begin{align}
      H_0 &:& \theta=\theta_0 ,\\
      H_1 &:& \theta=\theta_1 .
      \end{align}
      ]
In this case, under either hypothesis, the distribution of the data is fully
specified: there are no unknown parameters to estimate. For this case, a
variant of the likelihood-ratio test is available:[10][11]
         &#x03BB; ( x ) =      L   (  &#x03B8;  0   &#x2223; x )     L
      (  &#x03B8;  1   &#x2223; x )      {\displaystyle \lambda (x)={\frac {
      {\mathcal {L}}(\theta _{0}\mid x)}{{\mathcal {L}}(\theta _{1}\mid x)}}}
      [{\displaystyle \lambda (x)={\frac {{\mathcal {L}}(\theta _{0}\mid x)}{
      {\mathcal {L}}(\theta _{1}\mid x)}}}]
(Some older references may use the reciprocal of the function above as the
definition.[12] Thus, the likelihood ratio is small if the alternative model is
better than the null model.
The likelihood-ratio test provides the decision rule as follows:
      If     &#x03BB; > c   {\displaystyle \lambda >c}  [{\displaystyle \lambda
      >c}], do not reject      H  0     {\displaystyle H_{0}}  [H_{0}];
      If     &#x03BB; < c   {\displaystyle \lambda <c}  [{\displaystyle \lambda
      <c}], reject      H  0     {\displaystyle H_{0}}  [H_{0}];
      Reject with probability     q   {\displaystyle q}  [q] if     &#x03BB; =
      c .   {\displaystyle \lambda =c.}  [{\displaystyle \lambda =c.}]
The values     c   {\displaystyle c}  [c] and     q   {\displaystyle q}  [q]
are usually chosen to obtain a specified significance_level     &#x03B1;
{\displaystyle \alpha }  [\alpha ], via the relation
         q &#x22C5; P ( &#x03BB; = c &#x2223;  H  0   ) + P ( &#x03BB; < c
      &#x2223;  H  0   ) = &#x03B1; .   {\displaystyle q\cdot P(\lambda =c\mid
      H_{0})+P(\lambda <c\mid H_{0})=\alpha .}  [{\displaystyle q\cdot P
      (\lambda =c\mid H_{0})+P(\lambda <c\mid H_{0})=\alpha .}]
The NeymanâPearson_lemma states that this likelihood-ratio test is the most
powerful among all level     &#x03B1;   {\displaystyle \alpha }  [\alpha ]
tests for this case.[6][11]
***** Interpretation[edit] *****
The likelihood ratio is a function of the data     x   {\displaystyle x}  [x];
therefore, it is a statistic. The likelihood-ratio test rejects the null
hypothesis if the value of this statistic is too small. How small is too small
depends on the significance level of the test, i.e. on what probability of
Type I_error is considered tolerable (Type I errors consist of the rejection of
a null hypothesis that is true).
The numerator corresponds to the likelihood of an observed outcome under the
null_hypothesis. The denominator corresponds to the maximum likelihood of an
observed outcome, varying parameters over the whole parameter space. The
numerator of this ratio is less than the denominator; so, the likelihood ratio
is between 0 and 1. Low values of the likelihood ratio mean that the observed
result was much less likely to occur under the null hypothesis as compared to
the alternative. High values of the statistic mean that the observed outcome
was nearly as likely to occur under the null hypothesis as the alternative, and
so the null hypothesis cannot be rejected.
**** An example[edit] ****
The following example is adapted and abridged from Stuart_et_al._(1999,
Â§22.2).
Suppose that we have a random sample, of size n, from a population that is
normally-distributed. Both the mean, μ, and the standard deviation, σ, of the
population are unknown. We want to test whether the mean is equal to a given
value, μ0.
Thus, our null hypothesis is H0:  μ = μ0  and our alternative hypothesis is H1:
  μ â  μ0. The likelihood function is
           L   ( &#x03BC; , &#x03C3; &#x2223; x ) =   (  2 &#x03C0;  &#x03C3;
      2    )   &#x2212; n  /  2   exp &#x2061;  (  &#x2212;  &#x2211;  i = 1
      n      (  x  i   &#x2212; &#x03BC;  )  2     2  &#x03C3;  2       )  .
      {\displaystyle {\mathcal {L}}(\mu ,\sigma \mid x)=\left(2\pi \sigma ^
      {2}\right)^{-n/2}\exp \left(-\sum _{i=1}^{n}{\frac {(x_{i}-\mu )^{2}}
      {2\sigma ^{2}}}\right).}  [{\displaystyle {\mathcal {L}}(\mu ,\sigma \mid
      x)=\left(2\pi \sigma ^{2}\right)^{-n/2}\exp \left(-\sum _{i=1}^{n}{\frac
      {(x_{i}-\mu )^{2}}{2\sigma ^{2}}}\right).}]
With some calculation (omitted here), it can then be shown that
         &#x03BB; =   (  1 +    t  2    n &#x2212; 1     )   &#x2212; n  /  2
      {\displaystyle \lambda =\left(1+{\frac {t^{2}}{n-1}}\right)^{-n/2}}  [
      {\displaystyle \lambda =\left(1+{\frac {t^{2}}{n-1}}\right)^{-n/2}}]
where t is the t-statistic with n â 1 degrees of freedom. Hence we may use
the known exact distribution of t2 to draw inferences.
***** Asymptotic distribution: Wilksâ theorem[edit] *****
Main article: Wilks'_theorem
If the distribution of the likelihood ratio corresponding to a particular null
and alternative hypothesis can be explicitly determined then it can directly be
used to form decision regions (to sustain or reject the null hypothesis). In
most cases, however, the exact distribution of the likelihood ratio
corresponding to specific hypotheses is very difficult to determine.[citation
needed]
Assuming H0 is true, there is a fundamental result by Samuel_S._Wilks: As the
sample size     n   {\displaystyle n}  [n] approaches ___&#x221E;___
{\displaystyle_\infty_}__[\infty_], the test statistic     &#x2212; 2 log
&#x2061; ( &#x03BB; )   {\displaystyle -2\log(\lambda )}  [{\displaystyle -
2\log(\lambda )}] asymptotically will be chi-squared_distributed (     &#x03C7;
2     {\displaystyle \chi ^{2}}  [\chi ^{2}]) with degrees_of_freedom equal to
the difference in dimensionality of     &#x0398;   {\displaystyle \Theta }
[\Theta ] and      &#x0398;  0     {\displaystyle \Theta _{0}}  [\Theta_0].[13]
This implies that for a great variety of hypotheses, we can calculate the
likelihood ratio     &#x03BB;   {\displaystyle \lambda }  [\lambda ] for the
data and then compare     &#x2212; 2 log &#x2061; ( &#x03BB; )   {\displaystyle
-2\log(\lambda )}  [{\displaystyle -2\log(\lambda )}] to the      &#x03C7;  2
{\displaystyle \chi ^{2}}  [\chi ^{2}] value corresponding to a desired
statistical_significance as an approximate statistical test. Other extensions
exist.[which?]
***** See also[edit] *****
    * Akaike_information_criterion
    * Bayes_factor
    * Johansen_test
    * Model_selection
    * Vuong's_closeness_test
    * Sup-LR_test
    * Error_exponents_in_hypothesis_testing
***** References[edit] *****
   1. ^King,_Gary (1989). Unifying_Political_Methodology :_The_Likelihood
      Theory_of_Statistical_Inference. New York: Cambridge University Press.
      p. 84. ISBN 0-521-36697-6.
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
   3. ^Maddala,_G._S.; Lahiri, Kajal (2010). Introduction to Econometrics
      (Fourth ed.). New York: Wiley. p. 200.
   4. ^Buse, A. (1982). "The Likelihood Ratio, Wald, and Lagrange Multiplier
      Tests: An Expository Note". The_American_Statistician. 36 (3a):
      153â157. doi:10.1080/00031305.1982.10482817.
   5. ^Pickles, Andrew (1985). An Introduction to Likelihood Analysis. Norwich:
      W. H. Hutchins & Sons. pp. 24â27. ISBN 0-86094-190-6.
   6. ^Severini, Thomas A. (2000). Likelihood Methods in Statistics. New York:
      Oxford University Press. pp. 120â121. ISBN 0-19-850650-3.
   7. ^ a bNeyman,_J.; Pearson,_E._S. (1933), "On_the_problem_of_the_most
      efficient_tests_of_statistical_hypotheses" (PDF), Philosophical
      Transactions_of_the_Royal_Society_of_London_A, 231 (694â706):
      289â337, Bibcode:1933RSPTA.231..289N, doi:10.1098/rsta.1933.0009,
      JSTOR 91247
   8. ^Koch,_Karl-Rudolf (1988). Parameter Estimation and Hypothesis Testing in
      Linear Models. New York: Springer. p. 306. ISBN 0-387-18840-1.
   9. ^Silvey, S. D. (1970). Statistical Inference. London: Chapman & Hall.
      pp. 112â114. ISBN 0-412-13820-4.
  10. ^Mittelhammer,_Ron_C.; Judge,_George_G.; Miller, Douglas J. (2000).
      Econometric Foundations. New York: Cambridge University Press. p. 66.
      ISBN 0-521-62394-4.
  11. ^Mood, A. M.; Graybill, F. A.; Boes, D. C. (1974), Introduction to the
      Theory of Statistics (3rd ed.), McGraw-Hill, Â§9.2
  12. ^ a bStuart, A.; Ord, K.; Arnold, S. (1999), Kendall's Advanced Theory of
      Statistics, 2A, Arnold, Â§Â§20.10â20.13
  13. ^Cox,_D._R.; Hinkley,_D._V. (1974), Theoretical Statistics, Chapman_&
      Hall, p. 92, ISBN 0-412-12420-3
  14. ^Wilks,_S._S. (1938), "The large-sample distribution of the likelihood
      ratio for testing composite hypotheses", Annals_of_Mathematical
      Statistics, 9: 60â62, doi:10.1214/aoms/1177732360
***** Further reading[edit] *****
    * Glover, Scott; Dixon, Peter (2004), "Likelihood ratios: A simple and
      flexible statistic for empirical psychologists", Psychonomic_Bulletin_&
      Review, 11 (5): 791â806, doi:10.3758/BF03196706
Held, Leonhard; SabanÃ©s BovÃ©, Daniel (2014), Applied Statistical
InferenceâLikelihood and Bayes, Springer
Kalbfleisch,_J._G. (1985), Probability and Statistical Inference, 2, Springer-
Verlag
Perlman, Michael D.; Wu, Lang (1999), "The emperor's new tests", Statistical
Science, 14 (4): 355â381, doi:10.1214/ss/1009212517
Perneger, Thomas V. (2001), "Sifting the evidence: Likelihood ratios are
alternatives to P values", The_BMJ, 322 (7295): 1184â5, PMC 1120301,
PMID 11379590
Pinheiro, JosÃ© C.; Bates, Douglas M. (2000), Mixed-Effects Models in S and S-
PLUS, Springer-Verlag, pp. 82â93
Solomon, Daniel L. (1975), "A note on the non-equivalence of the Neyman-Pearson
and generalized likelihood ratio tests for testing a simple null versus a
simple alternative hypothesis", The_American_Statistician, 29 (2): 101â102,
doi:10.1080/00031305.1975.10477383
***** External links[edit] *****
    * Practical_application_of_likelihood_ratio_test_described
    * R_Package:_Wald's_Sequential_Probability_Ratio_Test
    * Richard_Lowry's_Predictive_Values_and_Likelihood_Ratios Online Clinical
      Calculator
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
                           * Likelihood-ratio test
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

Retrieved from "https://en.wikipedia.org/w/index.php?title=Likelihood-
ratio_test&oldid=905303520"
Categories:
    * Statistical_ratios
    * Statistical_tests
Hidden categories:
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2018
    * All_articles_with_specifically_marked_weasel-worded_phrases
    * Articles_with_specifically_marked_weasel-worded_phrases_from_March_2019
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
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Basa_Sunda
    * Suomi
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 8 July 2019, at 07:57 (UTC).
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
