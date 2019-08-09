The following text has been accessed from https://en.wikipedia.org/wiki/Statistical_process_control at Fri Aug 9 03:53:32 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Statistical process control ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Statistical process control (SPC) is a method of quality_control which employs
statistical_methods to monitor and control a process. This helps to ensure that
the process operates efficiently, producing more specification-conforming
products with less waste (rework or scrap). SPC can be applied to any process
where the "conforming product" (product meeting specifications) output can be
measured. Key tools used in SPC include run_charts, control_charts, a focus on
continuous_improvement, and the_design_of_experiments. An example of a process
where SPC is applied is manufacturing lines.
SPC must be practiced in 2 phases: The first phase is the initial establishment
of the process, and the second phase is the regular production use of the
process. In the second phase, a decision of the period to be examined must be
made, depending upon the change in 5M&E conditions (Man, Machine, Material,
Method, Movement, Environment) and wear rate of parts used in the manufacturing
process (machine parts, jigs, and fixtures).
An advantage of SPC over other methods of quality control, such as
"inspection", is that it emphasizes early detection and prevention of problems,
rather than the correction of problems after they have occurred.
In addition to reducing waste, SPC can lead to a reduction in the time required
to produce the product. SPC makes it less likely the finished product will need
to be reworked or scrapped.
⁰
***** Contents *****
    * 1_History
          o 1.1_"Common"_and_"special"_sources_of_variation
          o 1.2_Application_to_non-manufacturing_processes
    * 2_Variation_in_manufacturing
    * 3_Application_of_SPC
          o 3.1_Control_charts
                # 3.1.1_Stable_process
                # 3.1.2_Excessive_variations
                # 3.1.3_Process_stability_metrics
    * 4_Mathematics_of_control_charts
    * 5_See_also
    * 6_References
    * 7_Bibliography
    * 8_External_links
***** History[edit] *****
SPC was pioneered by Walter_A._Shewhart at Bell_Laboratories in the early
1920s. Shewhart developed the control chart in 1924 and the concept of a state
of statistical control. Statistical control is equivalent to the concept of
exchangeability[1][2] developed by logician William_Ernest_Johnson also in 1924
in his book Logic, Part III: The Logical Foundations of Science.[3] Along with
a team at AT&T that included Harold_Dodge and Harry Romig he worked to put
sampling inspection on a rational statistical basis as well. Shewhart consulted
with Colonel Leslie E. Simon in the application of control charts to munitions
manufacture at the Army's Picatinny_Arsenal in 1934. That successful
application helped convince Army Ordnance to engage AT&T's George Edwards to
consult on the use of statistical quality control among its divisions and
contractors at the outbreak of World War II.
W._Edwards_Deming invited Shewhart to speak at the Graduate School of the U.S.
Department of Agriculture, and served as the editor of Shewhart's book
Statistical Method from the Viewpoint of Quality Control (1939) which was the
result of that lecture. Deming was an important architect of the quality
control short courses that trained American industry in the new techniques
during WWII. The graduates of these wartime courses formed a new professional
society in 1945, the American Society for Quality Control, which elected
Edwards as its first president. Deming traveled to Japan during the Allied
Occupation and met with the Union of Japanese Scientists and Engineers (JUSE)
in an effort to introduce SPC methods to Japanese industry .[4][5]
**** "Common" and "special" sources of variation[edit] ****
Main article: Common_cause_and_special_cause_(statistics)
Shewhart read the new statistical theories coming out of Britain, especially
the work of William_Sealy_Gosset, Karl_Pearson, and Ronald_Fisher. However, he
understood that data from physical processes seldom produced a "normal
distribution curve"; that is, a Gaussian_distribution or "bell_curve". He
discovered that data from measurements of variation in manufacturing did not
always behave the way as data from measurements of natural phenomena (for
example, Brownian_motion of particles). Shewhart concluded that while every
process displays variation, some processes display variation that is natural to
the process ("common" sources of variation)- these processes were described as
'in (statistical) control'. Other processes additionally display variation that
is not present in the causal system of the process at all times ("special"
sources of variation), and these were described as 'not in control'.[6]
**** Application to non-manufacturing processes[edit] ****
In 1988, the Software_Engineering_Institute suggested that SPC could be applied
to non-manufacturing processes, such as software engineering processes, in the
Capability_Maturity_Model (CMM). The Level 4 and Level 5 practices of the
Capability Maturity Model Integration (CMMI) use this concept.
The notion that SPC is a useful tool when applied to non-repetitive, knowledge-
intensive processes such as research and development or systems engineering has
encountered skepticism and remains controversial.[7][8]
In his seminal article No Silver Bullet, Fred_Brooks points out that the
complexity, conformance requirements, changeability, and invisibility of
software[9][10] results in inherent and essential variation that cannot be
removed. This implies that SPC is less effective in the domain of software
development than in, e.g., manufacturing.
***** Variation in manufacturing[edit] *****
In manufacturing, quality is defined as conformance to specification. However,
no two products or characteristics are ever exactly the same, because any
process contains many sources of variability. In mass-manufacturing,
traditionally, the quality of a finished article is ensured by post-
manufacturing inspection of the product. Each article (or a sample of articles
from a production lot) may be accepted or rejected according to how well it
meets its design specifications. In contrast, SPC uses statistical tools to
observe the performance of the production process in order to detect
significant variations before they result in the production of a sub-standard
article. Any source of variation at any point of time in a process will fall
into one of two classes.
      1) "Common Causes" - sometimes referred to as nonassignable, normal
      sources of variation. It refers to many sources of variation that
      consistently acts on process. These types of causes produce a stable and
      repeatable distribution over time.
      2) "Special Causes" - sometimes referred to as assignable sources of
      variation. It refers to any factor causing variation that affects only
      some of the process output. They are often intermittent and
      unpredictable.
Most processes have many sources of variation; most of them are minor and may
be ignored. If the dominant assignable sources of variation are detected,
potentially they can be identified and removed. When they are removed, the
process is said to be "stable". When a process is stable, its variation should
remain within a known set of limits. That is, at least, until another
assignable source of variation occurs. For example, a breakfast cereal
packaging line may be designed to fill each cereal box with 500 grams of
cereal. Some boxes will have slightly more than 500 grams, and some will have
slightly less. When the package weights are measured, the data will demonstrate
a distribution of net weights. If the production process, its inputs, or its
environment (for example, the machine on the line) change, the distribution of
the data will change. For example, as the cams and pulleys of the machinery
wear, the cereal filling machine may put more than the specified amount of
cereal into each box. Although this might benefit the customer, from the
manufacturer's point of view, this is wasteful and increases the cost of
production. If the manufacturer finds the change and its source in a timely
manner, the change can be corrected (for example, the cams and pulleys
replaced).
***** Application of SPC[edit] *****
The application of SPC involves three main phases of activity:
   1. Understanding the process and the specification limits.
   2. Eliminating assignable (special) sources of variation, so that the
      process is stable.
   3. Monitoring the ongoing production process, assisted by the use of control
      charts, to detect significant changes of mean or variation.
**** Control charts[edit] ****
The data from measurements of variations at points on the process map is
monitored using control_charts. Control charts attempt to differentiate
"assignable" ("special") sources of variation from "common" sources. "Common"
sources, because they are an expected part of the process, are of much less
concern to the manufacturer than "assignable" sources. Using control charts is
a continuous activity, ongoing over time.
*** Stable process[edit] ***
When the process does not trigger any of the control chart "detection rules"
for the control chart, it is said to be "stable". A process_capability analysis
may be performed on a stable process to predict the ability of the process to
produce "conforming product" in the future.
A stable process can be demonstrated by a process signature that is free of
variances outside of the capability index. A process signature is the plotted
points compared with the capability index.
*** Excessive variations[edit] ***
When the process triggers any of the control chart "detection rules", (or
alternatively, the process capability is low), other activities may be
performed to identify the source of the excessive variation. The tools used in
these extra activities include: Ishikawa_diagram, designed_experiments, and
Pareto_charts. Designed experiments are a means of objectively quantifying the
relative importance (strength) of sources of variation. Once the sources of
(special cause) variation are identified, they can be minimized or eliminated.
Steps to eliminating a source of variation might include: development of
standards, staff training, error-proofing, and changes to the process itself or
its inputs.
*** Process stability metrics[edit] ***
When monitoring many processes with control charts, it is sometimes useful to
calculate quantitative measures of the stability of the processes. These
metrics can then be used to identify/prioritize the processes that are most in
need of corrective actions. These metrics can also be viewed as supplementing
the traditional process_capability metrics. Several metrics have been proposed,
as described in Ramirez and Runger. [11] They are (1) a Stability Ratio which
compares the long-term variability to the short-term variability, (2) an ANOVA
Test which compares the within-subgroup variation to the between-subgroup
variation, and (3) an Instability Ratio which compares the number of subgroups
that have one or more violations of the Western_Electric_rules to the total
number of subgroups.
***** Mathematics of control charts[edit] *****
Digital control charts use logic-based rules that determine "derived values"
which signal the need for correction. For example,
      derived value = last value + average_absolute_difference between the last
      N numbers.
***** See also[edit] *****
    * Process_capability_index
    * Quality_assurance
    * Industrial_engineering
    * ANOVA_Gauge_R&R
    * Stochastic_control
    * Electronic_design_automation
    * Process_Window_Index
    * Reliability_engineering
    * Six_sigma
    * Total_quality_management
***** References[edit] *****
   1. ^ Barlow & Irony (1992)
   2. ^ Bergman (2009)
   3. ^ Zabell (1992)
   4. ^ Deming, W. Edwards, Lectures on statistical control of quality., Nippon
      Kagaku Gijutsu Remmei, 1950
   5. ^ Deming, W. Edwards and Dowd S. John (translator) Lecture to Japanese
      Management, Deming Electronic Network Web Site, 1950 (from a Japanese
      transcript of a lecture by Deming to "80% of Japanese top management"
      given at the Hotel de Yama at Mr. Hakone in August 1950)
   6. ^ "Why SPC?" British Deming Association SPC Press, Inc. 1992
   7. ^ Bob Raczynski and Bill_Curtis (2008) Software Data Violate SPC's
      Underlying Assumptions, IEEE Software, May/June 2008, Vol. 25, No. 3, pp.
      49-51
   8. ^ Robert V. Binder (1997) Can a Manufacturing Quality Model Work for
      Software?, IEEE Software, September/October 1997, pp. 101-105
   9. ^Brooks, F. P. , J. (1987). "No_Silver_BulletâEssence_and_Accidents_of
      Software_Engineering" (PDF). Computer. 20 (4): 10â19.
      CiteSeerX 10.1.1.117.315. doi:10.1109/MC.1987.1663532.
  10. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
  11. ^ Fred P. Brooks (1986) No Silver Bullet â Essence and Accident in
      Software Engineering, Proceedings of the IFIP Tenth World Computing
      Conference 1986, pp. 1069â1076
  12. ^Ramirez, B.; Runger, G. (2006). "Quantitative Techniques to Evaluate
      Process Stability". Quality Engineering. 18 (1). pp. 53â68. doi:
      10.1080/08982110500403581.
***** Bibliography[edit] *****
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (July 2014)(Learn_how_and_when
 to_remove_this_template_message)
    * Barlow, R. E. & Irony, T. Z. (1992) "Foundations of statistical quality
      control" in Ghosh, M. & Pathak, P.K. (eds.) Current Issues in Statistical
      Inference: Essays in Honor of D. Basu, Hayward, CA: Institute of
      Mathematical Statistics, 99-112.
    * Bergman, B. (2009) "Conceptualistic Pragmatism: A framework for Bayesian
      analysis?", IIE Transactions, 41, 86â93
    * Deming, W E (1975) "On probability as a basis for action", The American
      Statistician, 29(4), 146â152
    * â (1982) Out of the Crisis: Quality, Productivity and Competitive
      Position
ISBN 0-521-30553-5
Grant,E. L. (1946) Statistical_quality_control
ISBN 0071004475
Oakland, J (2002) Statistical Process Control
ISBN 0-7506-5766-9
Salacinski, T (2015) SPC - Statistical Process Control. The Warsaw University
of Technology Publishing House.
ISBN 978-83-7814-319-2
Shewhart, W A (1931) Economic Control of Quality of Manufactured Product
ISBN 0-87389-076-0
â (1939) Statistical Method from the Viewpoint of Quality Control
ISBN 0-486-65232-7
Wheeler, D J (2000) Normality and the Process-Behaviour Chart
ISBN 0-945320-56-6
Wheeler, D J & Chambers, D S (1992) Understanding Statistical Process Control
ISBN 0-945320-13-2
Wheeler, Donald J. (1999). Understanding Variation: The Key to Managing Chaos -
2nd Edition. SPC Press, Inc.
ISBN 0-945320-53-1.
Wise, Stephen A. & Fair, Douglas C (1998). Innovative Control Charting:
Practical SPC Solutions for Today's Manufacturing Environment. ASQ Quality
Press.
ISBN 0-87389-385-9
Zabell, S. L. (1992). "Predicting the unpredictable". Synthese. 90 (2): 205.
doi:10.1007/bf00485351.
2019 "A_Complete_Guide_To_Statistical_Process_Control"
***** External links[edit] *****
 Wikimedia Commons has media related to Statistical_process_control.
    * MIT_Course_-_Control_of_Manufacturing_Processes
    * NIST_Engineering_Statistics_Handbook
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

    * v
    * t
    * e
Six_Sigma tools
                  * Project_charter
Define phase      * Voice_of_the_customer
                  * Value_stream_mapping
                  * Business_process_mapping
Measure phase     * Process_capability
                  * Pareto_chart
                  * Root_cause_analysis
Analyse phase     * Failure_mode_and_effects_analysis
                  * Multi-vari_chart
Improve phase     * Design_of_experiments
                  * Kaizen
                  * Control_plan
Control phase     * Statistical process control
                  * 5S
                  * Poka-yoke
DMAIC

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Statistical_process_control&oldid=901710382"
Categories:
    * Statistical_process_control
Hidden categories:
    * Articles_lacking_in-text_citations_from_July_2014
    * All_articles_lacking_in-text_citations
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
    * CatalÃ 
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 13 June 2019, at 19:08 (UTC).
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
