The following text has been accessed from https://en.wikipedia.org/wiki/Geostatistics at Thu Aug 8 23:35:00 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Geostatistics ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with statistical_geography.
A branch of statistics focusing on spatial data sets
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (January 2009)(Learn_how_and
 when_to_remove_this_template_message)
Geostatistics is a branch of statistics focusing on spatial or spatiotemporal
datasets. Developed originally to predict probability_distributions of ore
grades for mining operations,[1] it is currently applied in diverse disciplines
including petroleum_geology, hydrogeology, hydrology, meteorology,
oceanography, geochemistry, geometallurgy, geography, forestry, environmental
control, landscape_ecology, soil_science, and agriculture (esp. in precision
farming). Geostatistics is applied in varied branches of geography,
particularly those involving the spread of diseases (epidemiology), the
practice of commerce and military planning (logistics), and the development of
efficient spatial_networks. Geostatistical algorithms are incorporated in many
places, including geographic_information_systems (GIS) and the R_statistical
environment.[2]
⁰
***** Contents *****
    * 1_Background
    * 2_Methods
          o 2.1_Estimation
                # 2.1.1_Kriging
                # 2.1.2_Indicator_kriging
          o 2.2_Simulation
    * 3_Definitions_and_tools
    * 4_Main_scientific_journals_related_to_geostatistics
    * 5_Scientific_organisations_related_to_geostatistics
    * 6_Related_software
    * 7_See_also
    * 8_Notes
    * 9_References
    * 10_External_links
***** Background[edit] *****
Geostatistics is intimately related to interpolation methods, but extends far
beyond simple interpolation problems. Geostatistical techniques rely on
statistical models that are based on random function (or random_variable)
theory to model the uncertainty associated with spatial estimation and
simulation.
A number of simpler interpolation methods/algorithms, such as inverse_distance
weighting, bilinear_interpolation and nearest-neighbor_interpolation, were
already well known before geostatistics.[3] Geostatistics goes beyond the
interpolation problem by considering the studied phenomenon at unknown
locations as a set of correlated random variables.
Let Z(x) be the value of the variable of interest at a certain location x. This
value is unknown (e.g. temperature, rainfall, piezometric_level, geological
facies, etc.). Although there exists a value at location x that could be
measured, geostatistics considers this value as random since it was not
measured, or has not been measured yet. However, the randomness of Z(x) is not
complete, but defined by a cumulative_distribution_function (CDF) that depends
on certain information that is known about the value Z(x):
         F (   z   ,  x  ) = Prob &#x2061; { Z (  x  ) &#x2A7D;   z   &#x2223;
      information  } .   {\displaystyle F({\mathit {z}},\mathbf {x}
      )=\operatorname {Prob} \lbrace Z(\mathbf {x} )\leqslant {\mathit {z}}\mid
      {\text{information}}\rbrace .}  [F({\mathit {z}},\mathbf {x}
      )=\operatorname {Prob} \lbrace Z(\mathbf {x} )\leqslant {\mathit {z}}\mid
      {\text{information}}\rbrace .]
Typically, if the value of Z is known at locations close to x (or in the
neighborhood of x) one can constrain the CDF of Z(x) by this neighborhood: if a
high spatial continuity is assumed, Z(x) can only have values similar to the
ones found in the neighborhood. Conversely, in the absence of spatial
continuity Z(x) can take any value. The spatial continuity of the random
variables is described by a model of spatial continuity that can be either a
parametric function in the case of variogram-based geostatistics, or have a
non-parametric form when using other methods such as multiple-point_simulation
[4] or pseudo-genetic techniques.
By applying a single spatial model on an entire domain, one makes the
assumption that Z is a stationary_process. It means that the same statistical
properties are applicable on the entire domain. Several geostatistical methods
provide ways of relaxing this stationarity assumption.
In this framework, one can distinguish two modeling goals:
   1. Estimating the value for Z(x), typically by the expectation, the median
      or the mode of the CDF f(z,x). This is usually denoted as an estimation
      problem.
   2. Sampling from the entire probability density function f(z,x) by actually
      considering each possible outcome of it at each location. This is
      generally done by creating several alternative maps of Z, called
      realizations. Consider a domain discretized in N grid nodes (or pixels).
      Each realization is a sample of the complete N-dimensional joint
      distribution function
               F (  z  ,  x  ) = Prob &#x2061; { Z (   x   1   ) &#x2A7D;  z  1
            , Z (   x   2   ) &#x2A7D;  z  2   , . . . , Z (   x   N   )
            &#x2A7D;  z  N   } .   {\displaystyle F(\mathbf {z} ,\mathbf {x}
            )=\operatorname {Prob} \lbrace Z(\mathbf {x} _{1})\leqslant z_{1},Z
            (\mathbf {x} _{2})\leqslant z_{2},...,Z(\mathbf {x} _{N})\leqslant
            z_{N}\rbrace .}  [F(\mathbf {z} ,\mathbf {x} )=\operatorname {Prob}
            \lbrace Z(\mathbf {x} _{1})\leqslant z_{1},Z(\mathbf {x} _
            {2})\leqslant z_{2},...,Z(\mathbf {x} _{N})\leqslant z_{N}\rbrace
            .]
      In this approach, the presence of multiple solutions to the interpolation
      problem is acknowledged. Each realization is considered as a possible
      scenario of what the real variable could be. All associated workflows are
      then considering ensemble of realizations, and consequently ensemble of
      predictions that allow for probabilistic forecasting. Therefore,
      geostatistics is often used to generate or update spatial models when
      solving inverse_problems.[5][6]
A number of methods exist for both geostatistical estimation and multiple
realizations approaches. Several reference books provide a comprehensive
overview of the discipline.[7][3][8][9][10][11][12][13][14][15][16]
***** Methods[edit] *****
**** Estimation[edit] ****
*** Kriging[edit] ***
Main article: Kriging
Kriging is a group of geostatistical techniques to interpolate the value of a
random field (e.g., the elevation, z, of the landscape as a function of the
geographic location) at an unobserved location from observations of its value
at nearby locations.
*** Indicator kriging[edit] ***
Main article: Multiple-indicator_kriging
Multiple-indicator kriging (MIK) is a recent advance on other techniques for
mineral deposit modeling and resource block model estimation, such as ordinary
kriging. Initially, MIK showed considerable promise as a new method that could
more accurately estimate overall global mineral deposit concentrations or
grades.
**** Simulation[edit] ****
    * Aggregation
    * Dissagregation
    * Turning_bands
    * Cholesky_decomposition
    * Truncated Gaussian
    * Plurigaussian
    * Annealing
    * Spectral simulation
    * Sequential Indicator
    * Sequential Gaussian
    * Dead Leave
    * Transition_probabilities
    * Markov_chain_geostatistics
    * Markov_mesh_models
    * Support_vector_machine
    * Boolean_simulation
    * Genetic models
    * Pseudo-genetic models
    * Cellular_automata
    * Multiple-Point Geostatistics
***** Definitions and tools[edit] *****
    * Regionalized_variable_theory
    * Covariance_function
    * Semi-variance
    * Variogram
    * Kriging
    * Range_(geostatistics)
    * Sill_(geostatistics)
    * Nugget_effect
    * Training_image
***** Main scientific journals related to geostatistics[edit] *****
    * Water_Resources_Research
    * Advances_in_Water_Resources
    * Ground_Water
    * Mathematical_Geosciences
    * Computers_&_Geosciences
    * Computational_Geosciences
    * J._Soil_Science_Society_of_America
    * Environmetrics[dead_link]
    * Remote_Sensing_of_the_Environment
    * Stochastic_Environmental_Research_and_Risk_Assessment
***** Scientific organisations related to geostatistics[edit] *****
    * European_Forum_for_Geography_and_Statistics (EFGS; formerly the European
      Forum for Geostatistics)
    * GeoEnvia promotes the use of geostatistical methods in environmental
      applications
    * International_Association_for_Mathematical_Geosciences
***** Related software[edit] *****
    * GsLib A classical open-source package dedicated to geostatistics, source
      code in Fortran 77 and 90.
    * PyGSLIB A python module built with codified GSLIB source code wrapped
      into python and Cython functions for drillhole processing, block
      modeling, computational geometry, VTK support and non-linear
      geostatistics
    * SGeMS An open-source package dedicated to geostatistics with user-
      friendly interface, source code in C++ with the GsTL a dedicated
      geostatistics C++ template library.
    * Isatis A complete proprietary solution for geostatistics and resource
      estimation.
    * Geostat A complete proprietary solution for geostatistics, geological
      modelling and resource estimation, see SGS_Genesis.
    * The_R_programming_language has around 20 other packages dedicated to
      geostatistics, and around 30 dedicated to other areas of spatial
      statistics.
    * D-STEM[17] is a software based on the MATLAB language able to handle
      spatiotemporal univariate and multivariate_datasets. The software allows
      users to produce dynamic maps of the observed variables over geographic
      regions.
    * GeoStats.jl High-performance implementations of geostatistical algorithms
      for the Julia programming language.
    * GeostatsPy GSLIB and other data analytics and geostatistical
      functionality for spatial modeling in an open-source Python package.
***** See also[edit] *****
    * Multivariate_interpolation
    * Spline_interpolation
    * Geodemographic_segmentation
    * Remote_sensing
    * Pedometrics
***** Notes[edit] *****
   1. ^ Krige, Danie G. (1951). "A statistical approach to some basic mine
      valuation problems on the Witwatersrand". J. of the Chem., Metal. and
      Mining Soc. of South Africa 52 (6): 119â139
   2. ^ Hemakumara, GPTS, & Rainis, Ruslan. (2015). Geo-statistical modeling to
      evaluate the socio-economic impacts of households in the context of low-
      lying areas conversion in Colombo metropolitan region-Sri Lanka. Paper
      presented at the AIP Conference Proceedings.
   3. ^ a b Isaaks, E. H. and Srivastava, R. M. (1989), An Introduction to
      Applied Geostatistics, Oxford University Press, New York, USA.
   4. ^ Mariethoz, Gregoire, Caers, Jef (2014). Multiple-point geostatistics:
      modeling with training images. Wiley-Blackwell, Chichester, UK, 364 p.
   5. ^ Hansen, T.M., Journel, A.G., Tarantola, A. and Mosegaard, K. (2006).
      "Linear inverse Gaussian theory and geostatistics", Geophysics 71
   6. ^ Kitanidis, P.K. and Vomvoris, E.G. (1983). "A geostatistical approach
      to the inverse problem in groundwater modeling (steady state) and one-
      dimensional simulations", Water Resources Research 19(3):677-690
   7. ^ Remy, N., et al. (2009), Applied Geostatistics with SGeMS: A User's
      Guide, 284 pp., Cambridge University Press, Cambridge.
   8. ^  Deutsch, C.V., Journel, A.G, (1997). GSLIB: Geostatistical Software
      Library and User's Guide (Applied Geostatistics Series), Second Edition,
      Oxford University Press, 369 pp., http://www.gslib.com/
   9. ^ ChilÃ¨s, J.-P., and P. Delfiner (1999), Geostatistics - Modeling
      Spatial Uncertainty, John Wiley & Sons, Inc., New York, USA.
  10. ^ LantuÃ©joul, C. (2002), Geostatistical simulation: Models and
      algorithms, 232 pp., Springer, Berlin.
  11. ^ Journel, A. G. and Huijbregts, C.J. (1978) Mining Geostatistics,
      Academic Press.
  12. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
  13. ISBN 0-12-391050-1
  14. ^ Kitanidis, P.K. (1997) Introduction to Geostatistics: Applications in
      Hydrogeology, Cambridge University Press.
  15. ^ Wackernagel, H. (2003). Multivariate geostatistics, Third edition,
      Springer-Verlag, Berlin, 387 pp.
  16. ^ Pyrcz, M. J. and Deutsch, C.V., (2014). Geostatistical Reservoir
      Modeling, 2nd Edition, Oxford University Press, 448 pp.
  17. ^ Tahmasebi, P., Hezarkhani, A., Sahimi, M., 2012, Multiple-point
      geostatistical modeling based on the cross-correlation functions,
      Computational Geosciences, 16(3):779-79742,
  18. ^Schnetzler, Manu. "Statios_-_WinGslib".
  19. ^ Finazzi, F. and FassÃ², A. (2014). "D-STEM: A Software for the Analysis
      and Mapping of Environmental Space-Time Variables", Journal of
      Statistical Software 62(6)
***** References[edit] *****
   1. Armstrong, M and Champigny, N, 1988, A Study on Kriging Small Blocks, CIM
      Bulletin, Vol 82, No 923
   2. Armstrong, M, 1992, Freedom_of_Speech? De Geeostatisticis, July, No 14
   3. Champigny, N, 1992, Geostatistics:_A_tool_that_works, The_Northern_Miner,
      May 18
   4. Clark I, 1979, Practical_Geostatistics, Applied Science Publishers,
      London
   5. David, M, 1977, Geostatistical Ore Reserve Estimation, Elsevier
      Scientific Publishing Company, Amsterdam
   6. Hald, A, 1952, Statistical Theory with Engineering Applications, John
      Wiley & Sons, New York
   7. Honarkhah, Mehrdad; Caers, Jef (2010). "Stochastic Simulation of Patterns
      Using Distance-Based Pattern Modeling". Mathematical Geosciences. 42 (5):
      487â517. doi:10.1007/s11004-010-9276-7.
   8.  (best paper award IAMG 09)
   9. ISO/DIS 11648-1 Statistical aspects of sampling from bulk materials-
      Part1: General principles
  10. Lipschutz, S, 1968, Theory and Problems of Probability, McCraw-Hill Book
      Company, New York.
  11. Matheron, G. 1962. TraitÃ© de gÃ©ostatistique appliquÃ©e. Tome 1,
      Editions Technip, Paris, 334 pp.
  12. Matheron, G. 1989. Estimating and choosing, Springer-Verlag, Berlin.
  13. McGrew, J. Chapman, & Monroe, Charles B., 2000. An introduction to
      statistical problem solving in geography, second edition, McGraw-Hill,
      New York.
  14. Merks, J W, 1992, Geostatistics_or_voodoo_science, The Northern Miner,
      May 18
  15. Merks, J W, Abuse_of_statistics, CIM Bulletin, January 1993, Vol 86, No
      966
  16. Myers, Donald E.; "What_Is_Geostatistics?
  17. Philip, G M and Watson, D F, 1986, Matheronian Geostatistics; Quo Vadis?,
      Mathematical Geology, Vol 18, No 1
  18. Pyrcz, M.J. and Deutsch, C.V., 2014, Geostatistical Reservoir Modeling,
      2nd Edition, Oxford University Press, New York, p. 448
  19. Sharov, A: Quantitative Population Ecology, 1996, https://
      web.archive.org/web/20020605050231/http://www.ento.vt.edu/~sharov/
      PopEcol/popecol.html
  20. Shine, J.A., Wakefield, G.I.: A comparison of supervised imagery
      classification using analyst-chosen and geostatistically-chosen training
      sets, 1999, https://web.archive.org/web/20020424165227/http://
      www.geovista.psu.edu/sites/geocomp99/Gc99/044/gc_044.htm
  21. Strahler, A. H., and Strahler A., 2006, Introducing Physical Geography,
      4th Ed., Wiley.
  22. Tahmasebi, P., Hezarkhani, A., Sahimi, M., 2012, Multiple-point
      geostatistical_modeling_based_on_the_cross-correlation_functions,
      Computational Geosciences, 16(3):779-79742.
  23. Volk, W, 1980, Applied Statistics for Engineers, Krieger Publishing
      Company, Huntington, New York.
***** External links[edit] *****
 Wikimedia Commons has media related to Geostatistics.
    * GeoENVia promotes the use of geostatistical methods in environmental
      applications, and organizes bi-annual conferences.
    * Kriging_link,_contains_explanations_of_variance_in_geostats
    * Arizona_university_geostats_page
    * AI-Geostats, a resource on the internet about geostatistics and spatial
      statistics
    * On-Line_Library_that_chronicles_Matheron's_journey_from_classical
      statistics_to_the_new_science_of_geostatistics
    * http://www.geostatscam.com Is the site of Jan W. Merks, who claims that
      geostatistics is "voodoo science" and a "scientific fraud"
    * [1] It is a group for exchanging of ideas and discussion on multiple
      point geostatistics (MPS).
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
Authority_control [Edit_this_at_Wikidata]     * GND: 4020279-3

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Geostatistics&oldid=909043822"
Categories:
    * Geostatistics
Hidden categories:
    * Articles_with_short_description
    * Articles_lacking_in-text_citations_from_January_2009
    * All_articles_lacking_in-text_citations
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_February_2019
    * Commons_category_link_from_Wikidata
    * Wikipedia_articles_with_GND_identifiers
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Italiano
    * á¥áá áá£áá
    * LietuviÅ³
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Basa_Sunda
    * Suomi
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
Edit_links
    * This page was last edited on 2 August 2019, at 17:46 (UTC).
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
