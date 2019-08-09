The following text has been accessed from https://en.wikipedia.org/wiki/Central_tendency at Fri Aug 9 02:26:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Central tendency ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For the graph/network concept, see Centrality.
In statistics, a central tendency (or measure of central tendency) is a central
or typical value for a probability_distribution.[1] It may also be called a
center or location of the distribution. Colloquially, measures of central
tendency are often called averages. The term central tendency dates from the
late 1920s.[2]
The most common measures of central tendency are the arithmetic_mean, the
median and the mode. A central tendency can be calculated for either a finite
set of values or for a theoretical distribution, such as the normal
distribution. Occasionally authors use central tendency to denote "the tendency
of quantitative data to cluster around some central value."[2][3]
The central tendency of a distribution is typically contrasted with its
dispersion or variability; dispersion and central tendency are the often
characterized properties of distributions. Analysis may judge whether data has
a strong or a weak central tendency based on its dispersion.
⁰
***** Contents *****
    * 1_Measures
    * 2_Solutions_to_variational_problems
          o 2.1_Uniqueness
          o 2.2_Information_geometry
    * 3_Relationships_between_the_mean,_median_and_mode
    * 4_See_also
    * 5_References
***** Measures[edit] *****
The following may be applied to one-dimensional data. Depending on the
circumstances, it may be appropriate to transform the data before calculating a
central tendency. Examples are squaring the values or taking logarithms.
Whether a transformation is appropriate and what it should be, depend heavily
on the data being analyzed.
  Arithmetic_mean or simply, mean
      the sum of all measurements divided by the number of observations in the
      data set.
  Median
      the middle value that separates the higher half from the lower half of
      the data set. The median and the mode are the only measures of central
      tendency that can be used for ordinal_data, in which values are ranked
      relative to each other but are not measured absolutely.
  Mode
      the most frequent value in the data set. This is the only central
      tendency measure that can be used with nominal_data, which have purely
      qualitative category assignments.
  Geometric_mean
      the nth_root of the product of the data values, where there are n of
      these. This measure is valid only for data that are measured absolutely
      on a strictly positive scale.
  Harmonic_mean
      the reciprocal of the arithmetic mean of the reciprocals of the data
      values. This measure too is valid only for data that are measured
      absolutely on a strictly positive scale.
  Weighted_arithmetic_mean
      an arithmetic mean that incorporates weighting to certain data elements.
  Truncated_mean or trimmed mean
      the arithmetic mean of data values after a certain number or proportion
      of the highest and lowest data values have been discarded.
        Interquartile_mean
            a truncated mean based on data within the interquartile_range.
  Midrange
      the arithmetic mean of the maximum and minimum values of a data set.
  Midhinge
      the arithmetic mean of the first and third quartiles.
  Trimean
      the weighted arithmetic mean of the median and two quartiles.
  Winsorized_mean
      an arithmetic mean in which extreme values are replaced by values closer
      to the median.
Any of the above may be applied to each dimension of multi-dimensional data,
but the results may not be invariant to rotations of the multi-dimensional
space. In addition, there are the
  Geometric_median
      which minimizes the sum of distances to the data points. This is the same
      as the median when applied to one-dimensional data, but it is not the
      same as taking the median of each dimension independently. It is not
      invariant to different rescaling of the different dimensions.
  Quadratic_mean (often known as the root_mean_square)
      useful in engineering, but not often used in statistics. This is because
      it is not a good indicator of the center of the distribution when the
      distribution includes negative values.
  Simplicial_depth
      the probability that a randomly chosen simplex with vertices from the
      given distribution will contain the given center
  Tukey_median
      a point with the property that every halfspace containing it also
      contains many sample points
***** Solutions to variational problems[edit] *****
Several measures of central tendency can be characterized as solving a
variational problem, in the sense of the calculus_of_variations, namely
minimizing variation from the center. That is, given a measure of statistical
dispersion, one asks for a measure of central tendency that minimizes
variation: such that variation from the center is minimal among all choices of
center. In a quip, "dispersion precedes location". This center may or may not
be unique. In the sense of Lp_spaces, the correspondence is:
Lp   dispersion                 central tendency
L0   variation_ratio            mode
L1   average_absolute_deviation median
L1   average_absolute_deviation geometric_median
L2   standard_deviation         mean
Lâmaximum_deviation          midrange
The associated functions are called p-norms: respectively 0-"norm", 1-norm, 2-
norm, and â-norm. The function corresponding to the L0 space is not a norm,
and is thus often referred to in quotes: 0-"norm".
In equations, for a given (finite) data set X, thought of as a vector      x  =
(  x  1   , &#x2026; ,  x  n   )   {\displaystyle \mathbf {x} =(x_{1},\ldots
,x_{n})}  [{\displaystyle \mathbf {x} =(x_{1},\ldots ,x_{n})}], the dispersion
about a point c is the "distance" from x to the constant vector      c  = ( c ,
&#x2026; , c )   {\displaystyle \mathbf {c} =(c,\ldots ,c)}  [{\displaystyle
\mathbf {c} =(c,\ldots ,c)}] in the p-norm (normalized by the number of points
n):
          f  p   ( c ) =   &#x2016;   x  &#x2212;  c   &#x2016;   p   :=
      (     1 n    &#x2211;  i = 1   n     |   x  i   &#x2212; c  |   p      )
      1  /  p   .   {\displaystyle f_{p}(c)=\left\|\mathbf {x} -\mathbf {c}
      \right\|_{p}:={\bigg (}{\frac {1}{n}}\sum _{i=1}^{n}\left|x_{i}-c\right|^
      {p}{\bigg )}^{1/p}.}  [{\displaystyle f_{p}(c)=\left\|\mathbf {x} -
      \mathbf {c} \right\|_{p}:={\bigg (}{\frac {1}{n}}\sum _{i=1}^{n}\left|x_
      {i}-c\right|^{p}{\bigg )}^{1/p}.}]
Note that for     p = 0   {\displaystyle p=0}  [p=0] and     p = &#x221E;
{\displaystyle p=\infty }  [{\displaystyle p=\infty }] these functions are
defined by taking limits, respectively as     p &#x2192; 0   {\displaystyle
p\to 0}  [{\displaystyle p\to 0}] and     p &#x2192; &#x221E;   {\displaystyle
p\to \infty }  [{\displaystyle p\to \infty }]. For     p = 0   {\displaystyle
p=0}  [p=0] the limiting values are      0  0   = 0   {\displaystyle 0^{0}=0}
[0^{0}=0] and      a  0   = 1   {\displaystyle a^{0}=1}  [a^{0}=1] for     a
&#x2260; 0   {\displaystyle a\neq 0}  [a\neq 0], so the difference becomes
simply equality, so the 0-norm counts the number of unequal points. For     p =
&#x221E;   {\displaystyle p=\infty }  [{\displaystyle p=\infty }] the largest
number dominates, and thus the â-norm is the maximum difference.
**** Uniqueness[edit] ****
The mean (L2 center) and midrange (Lâ center) are unique (when they exist),
while the median (L1 center) and mode (L0 center) are not in general unique.
This can be understood in terms of convexity of the associated functions
(coercive_functions).
The 2-norm and â-norm are strictly_convex, and thus (by convex optimization)
the minimizer is unique (if it exists), and exists for bounded distributions.
Thus standard deviation about the mean is lower than standard deviation about
any other point, and the maximum deviation about the midrange is lower than the
maximum deviation about any other point.
The 1-norm is not strictly convex, whereas strict convexity is needed to ensure
uniqueness of the minimizer. Correspondingly, the median (in this sense of
minimizing) is not in general unique, and in fact any point between the two
central points of a discrete distribution minimizes average absolute deviation.
The 0-"norm" is not convex (hence not a norm). Correspondingly, the mode is not
unique â for example, in a uniform distribution any point is the mode.
**** Information geometry[edit] ****
The notion of a "center" as minimizing variation can be generalized in
information_geometry as a distribution that minimizes divergence (a generalized
distance) from a data set. The most common case is maximum_likelihood
estimation, where the maximum likelihood estimate (MLE) maximizes likelihood
(minimizes expected surprisal), which can be interpreted geometrically by using
entropy to measure variation: the MLE minimizes cross_entropy (equivalently,
relative_entropy, KullbackâLeibler divergence).
A simple example of this is for the center of nominal data: instead of using
the mode (the only single-valued "center"), one often uses the empirical
measure (the frequency_distribution divided by the sample_size) as a "center".
For example, given binary_data, say heads or tails, if a data set consists of 2
heads and 1 tails, then the mode is "heads", but the empirical measure is 2/
3 heads, 1/3 tails, which minimizes the cross-entropy (total surprisal) from
the data set. This perspective is also used in regression_analysis, where least
squares finds the solution that minimizes the distances from it, and
analogously in logistic_regression, a maximum likelihood estimate minimizes the
surprisal (information distance).
***** Relationships between the mean, median and mode[edit] *****
Main article: Nonparametric_skew_Â§ Relationships_between_the_mean,_median_and
mode
For unimodal_distributions the following bounds are known and are sharp:[4]
             |  &#x03B8; &#x2212; &#x03BC;  |   &#x03C3;   &#x2264;   3   ,
      {\displaystyle {\frac {|\theta -\mu |}{\sigma }}\leq {\sqrt {3}},}  [
      {\frac  {|\theta -\mu |}{\sigma }}\leq {\sqrt  {3}},]
             |  &#x03BD; &#x2212; &#x03BC;  |   &#x03C3;   &#x2264;   0.6   ,
      {\displaystyle {\frac {|\nu -\mu |}{\sigma }}\leq {\sqrt {0.6}},}  [
      {\frac  {|\nu -\mu |}{\sigma }}\leq {\sqrt  {0.6}},]
             |  &#x03B8; &#x2212; &#x03BD;  |   &#x03C3;   &#x2264;   3   ,
      {\displaystyle {\frac {|\theta -\nu |}{\sigma }}\leq {\sqrt {3}},}  [
      {\frac  {|\theta -\nu |}{\sigma }}\leq {\sqrt  {3}},]
where Î¼ is the mean, Î½ is the median, Î¸ is the mode, and Ï is the standard
deviation.
For every distribution,[5][6]
             |  &#x03BD; &#x2212; &#x03BC;  |   &#x03C3;   &#x2264; 1.
      {\displaystyle {\frac {|\nu -\mu |}{\sigma }}\leq 1.}  [{\frac  {|\nu -
      \mu |}{\sigma }}\leq 1.]
***** See also[edit] *****
    * Expected_value
    * Location_parameter
***** References[edit] *****
   1. ^ Weisberg H.F (1992) Central Tendency and Variability, Sage University
      Paper Series on Quantitative Applications in the Social Sciences,
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
   3. ISBN 0-8039-4007-6 p.2
   4. ^ a b Upton, G.; Cook, I. (2008) Oxford Dictionary of Statistics, OUP
   5. ISBN 978-0-19-954145-4 (entry for "central tendency")
   6. ^ Dodge, Y. (2003) The Oxford Dictionary of Statistical Terms, OUP for
      International_Statistical_Institute.
   7. ISBN 0-19-920613-9 (entry for "central tendency")
   8. ^ Johnson NL, Rogers CA (1951) "The moment problem for unimodal
      distributions". Annals of Mathematical Statistics, 22 (3) 433â439
   9. ^ Hotelling H, Solomons LM (1932) The limits of a measure of skewness.
      Annals Math Stat 3, 141â114
  10. ^ Garver (1932) Concerning the limits of a mesuare of skewness. Ann Math
      Stats 3(4) 141â142
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
index.php?title=Central_tendency&oldid=900598740"
Categories:
    * Summary_statistics
    * Probability_theory
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
    * à¦¬à¦¾à¦à¦²à¦¾
    * CatalÃ 
    * Cymraeg
    * Deutsch
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Bahasa_Melayu
    * Nederlands
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * à·à·à¶à·à¶½
    * Simple_English
    * Ú©ÙØ±Ø¯Û
    * Basa_Sunda
    * Suomi
    * à°¤à±à°²à±à°à±
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 6 June 2019, at 15:45 (UTC).
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
