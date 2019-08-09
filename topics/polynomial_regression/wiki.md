The following text has been accessed from https://en.wikipedia.org/wiki/Polynomial_regression at Fri Aug 9 02:54:19 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Polynomial regression ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 It has been suggested that Polynomial_least_squares be merged into this
 article. (Discuss)Proposed since April 2018.
Part of a series on Statistics
Regression_analysis
[Linear_regression.svg]
Models
    * Linear_regression
    * Simple_regression
    * Polynomial regression
    * General_linear_model
    * Generalized_linear_model
    * Discrete_choice
    * Binomial_regression
    * Binary_regression
    * Logistic_regression
    * Multinomial_logit
    * Mixed_logit
    * Probit
    * Multinomial_probit
    * Ordered_logit
    * Ordered_probit
    * Poisson
    * Multilevel_model
    * Fixed_effects
    * Random_effects
    * Mixed_model
    * Nonlinear_regression
    * Nonparametric
    * Semiparametric
    * Robust
    * Quantile
    * Isotonic
    * Principal_components
    * Least_angle
    * Local
    * Segmented
    * Errors-in-variables
Estimation
    * Least_squares
    * Linear
    * Non-linear
    * Ordinary
    * Weighted
    * Generalized
    * Partial
    * Total
    * Non-negative
    * Ridge_regression
    * Regularized
    * Least_absolute_deviations
    * Iteratively_reweighted
    * Bayesian
    * Bayesian_multivariate
Background
    * Regression_validation
    * Mean_and_predicted_response
    * Errors_and_residuals
    * Goodness_of_fit
    * Studentized_residual
    * GaussâMarkov_theorem
    * [Fisher_iris_versicolor_sepalwidth.svg] Statistics_portal
    * v
    * t
    * e
In statistics, polynomial regression is a form of regression_analysis in which
the relationship between the independent_variable x and the dependent_variable
y is modelled as an nth degree polynomial in x. Polynomial regression fits a
nonlinear relationship between the value of x and the corresponding conditional
mean of y, denoted E(y |x), and has been used to describe nonlinear phenomena
such as the growth rate of tissues,[1] the distribution of carbon isotopes in
lake sediments,[2] and the progression of disease epidemics.[3] Although
polynomial regression fits a nonlinear model to the data, as a statistical
estimation problem it is linear, in the sense that the regression function E
(y | x) is linear in the unknown parameters that are estimated from the data.
For this reason, polynomial regression is considered to be a special case of
multiple_linear_regression.
The explanatory (independent) variables resulting from the polynomial expansion
of the "baseline" variables are known as higher-degree terms. Such variables
are also used in classification settings.[4]
⁰
***** Contents *****
    * 1_History
    * 2_Definition_and_example
    * 3_Matrix_form_and_calculation_of_estimates
    * 4_Interpretation
    * 5_Alternative_approaches
    * 6_See_also
    * 7_Notes
    * 8_References
    * 9_External_links
***** History[edit] *****
Polynomial regression models are usually fit using the method of least_squares.
The least-squares method minimizes the variance of the unbiased estimators of
the coefficients, under the conditions of the Gauss–Markov_theorem. The least-
squares method was published in 1805 by Legendre and in 1809 by Gauss. The
first design of an experiment for polynomial regression appeared in an 1815
paper of Gergonne.[5][6] In the twentieth century, polynomial regression played
an important role in the development of regression_analysis, with a greater
emphasis on issues of design and inference.[7] More recently, the use of
polynomial models has been complemented by other methods, with non-polynomial
models having advantages for some classes of problems.[citation_needed]
***** Definition and example[edit] *****
A cubic polynomial regression fit to a simulated data set. The confidence_band
is a 95% simultaneous confidence band constructed using the ScheffÃ© approach.
The goal of regression analysis is to model the expected value of a dependent
variable y in terms of the value of an independent variable (or vector of
independent variables) x. In simple linear regression, the model
         y =  &#x03B2;  0   +  &#x03B2;  1   x + &#x03B5; ,    {\displaystyle
      y=\beta _{0}+\beta _{1}x+\varepsilon ,\,}  [{\displaystyle y=\beta _
      {0}+\beta _{1}x+\varepsilon ,\,}]
is used, where Îµ is an unobserved random error with mean zero conditioned on a
scalar variable x. In this model, for each unit increase in the value of x, the
conditional expectation of y increases by Î²1 units.
In many settings, such a linear relationship may not hold. For example, if we
are modeling the yield of a chemical synthesis in terms of the temperature at
which the synthesis takes place, we may find that the yield improves by
increasing amounts for each unit increase in temperature. In this case, we
might propose a quadratic model of the form
         y =  &#x03B2;  0   +  &#x03B2;  1   x +  &#x03B2;  2    x  2   +
      &#x03B5; .    {\displaystyle y=\beta _{0}+\beta _{1}x+\beta _{2}x^
      {2}+\varepsilon .\,}  [{\displaystyle y=\beta _{0}+\beta _{1}x+\beta _
      {2}x^{2}+\varepsilon .\,}]
In this model, when the temperature is increased from x to x + 1 units, the
expected yield changes by      &#x03B2;  1   +  &#x03B2;  2   ( 2 x + 1 ) .
{\displaystyle \beta _{1}+\beta _{2}(2x+1).}  [{\displaystyle \beta _{1}+\beta
_{2}(2x+1).}] (This can be seen by replacing x in this equation with x+1 and
subtracting the equation in x from the equation in x+1.) For infinitesimal
changes in x, the effect on y is given by the total_derivative with respect to
x:      &#x03B2;  1   + 2  &#x03B2;  2   x .   {\displaystyle \beta _{1}+2\beta
_{2}x.}  [{\displaystyle \beta _{1}+2\beta _{2}x.}] The fact that the change in
yield depends on x is what makes the relationship between x and y nonlinear
even though the model is linear in the parameters to be estimated.
In general, we can model the expected value of y as an nth degree polynomial,
yielding the general polynomial regression model
         y =  &#x03B2;  0   +  &#x03B2;  1   x +  &#x03B2;  2    x  2   +
      &#x03B2;  3    x  3   + &#x22EF; +  &#x03B2;  n    x  n   + &#x03B5; .
      {\displaystyle y=\beta _{0}+\beta _{1}x+\beta _{2}x^{2}+\beta _{3}x^
      {3}+\cdots +\beta _{n}x^{n}+\varepsilon .\,}  [{\displaystyle y=\beta _
      {0}+\beta _{1}x+\beta _{2}x^{2}+\beta _{3}x^{3}+\cdots +\beta _{n}x^
      {n}+\varepsilon .\,}]
Conveniently, these models are all linear from the point of view of estimation,
since the regression function is linear in terms of the unknown parameters Î²0,
Î²1, .... Therefore, for least_squares analysis, the computational and
inferential problems of polynomial regression can be completely addressed using
the techniques of multiple_regression. This is done by treating x, x2, ... as
being distinct independent variables in a multiple regression model.
***** Matrix form and calculation of estimates[edit] *****
The polynomial regression model
          y  i    =   &#x03B2;  0   +  &#x03B2;  1    x  i   +  &#x03B2;  2
      x  i   2   + &#x22EF; +  &#x03B2;  m    x  i   m   +  &#x03B5;  i
      &#xA0; ( i = 1 , 2 , &#x2026; , n )   {\displaystyle y_{i}\,=\,\beta _
      {0}+\beta _{1}x_{i}+\beta _{2}x_{i}^{2}+\cdots +\beta _{m}x_{i}^
      {m}+\varepsilon _{i}\ (i=1,2,\dots ,n)}  [{\displaystyle y_{i}\,=\,\beta
      _{0}+\beta _{1}x_{i}+\beta _{2}x_{i}^{2}+\cdots +\beta _{m}x_{i}^
      {m}+\varepsilon _{i}\ (i=1,2,\dots ,n)}]
can be expressed in matrix form in terms of a design matrix      X
{\displaystyle \mathbf {X} }  [\mathbf {X} ], a response vector        y
&#x2192;      {\displaystyle {\vec {y}}}  [\vec y], a parameter vector
&#x03B2; &#x2192;      {\displaystyle {\vec {\beta }}}  [{\displaystyle {\vec
{\beta }}}], and a vector        &#x03B5; &#x2192;      {\displaystyle {\vec
{\varepsilon }}}  [{\displaystyle {\vec {\varepsilon }}}] of random errors. The
i-th row of      X    {\displaystyle \mathbf {X} }  [\mathbf {X} ] and        y
&#x2192;      {\displaystyle {\vec {y}}}  [\vec y] will contain the x and y
value for the i-th data sample. Then the model can be written as a system of
linear equations:
           [     y  1        y  2        y  3       &#x22EE;      y  n      ]
      =   [    1    x  1      x  1   2     &#x2026;    x  1   m       1    x  2
      x  2   2     &#x2026;    x  2   m       1    x  3      x  3   2
      &#x2026;    x  3   m       &#x22EE;   &#x22EE;   &#x22EE;   &#x22F1;
      &#x22EE;     1    x  n      x  n   2     &#x2026;    x  n   m      ]
      [     &#x03B2;  0        &#x03B2;  1        &#x03B2;  2       &#x22EE;
      &#x03B2;  m      ]   +   [     &#x03B5;  1        &#x03B5;  2
      &#x03B5;  3       &#x22EE;      &#x03B5;  n      ]   ,   {\displaystyle
      {\begin{bmatrix}y_{1}\\y_{2}\\y_{3}\\\vdots \\y_{n}\end{bmatrix}}={\begin
      {bmatrix}1&x_{1}&x_{1}^{2}&\dots &x_{1}^{m}\\1&x_{2}&x_{2}^{2}&\dots &x_
      {2}^{m}\\1&x_{3}&x_{3}^{2}&\dots &x_{3}^{m}\\\vdots &\vdots &\vdots
      &\ddots &\vdots \\1&x_{n}&x_{n}^{2}&\dots &x_{n}^{m}\end{bmatrix}}{\begin
      {bmatrix}\beta _{0}\\\beta _{1}\\\beta _{2}\\\vdots \\\beta _{m}\end
      {bmatrix}}+{\begin{bmatrix}\varepsilon _{1}\\\varepsilon _
      {2}\\\varepsilon _{3}\\\vdots \\\varepsilon _{n}\end{bmatrix}},}  [
      {\displaystyle {\begin{bmatrix}y_{1}\\y_{2}\\y_{3}\\\vdots \\y_{n}\end
      {bmatrix}}={\begin{bmatrix}1&x_{1}&x_{1}^{2}&\dots &x_{1}^{m}\\1&x_{2}&x_
      {2}^{2}&\dots &x_{2}^{m}\\1&x_{3}&x_{3}^{2}&\dots &x_{3}^{m}\\\vdots
      &\vdots &\vdots &\ddots &\vdots \\1&x_{n}&x_{n}^{2}&\dots &x_{n}^{m}\end
      {bmatrix}}{\begin{bmatrix}\beta _{0}\\\beta _{1}\\\beta _{2}\\\vdots
      \\\beta _{m}\end{bmatrix}}+{\begin{bmatrix}\varepsilon _{1}\\\varepsilon
      _{2}\\\varepsilon _{3}\\\vdots \\\varepsilon _{n}\end{bmatrix}},}]
which when using pure matrix notation is written as
            y &#x2192;    =  X     &#x03B2; &#x2192;    +    &#x03B5; &#x2192;
      .    {\displaystyle {\vec {y}}=\mathbf {X} {\vec {\beta }}+{\vec
      {\varepsilon }}.\,}  [{\displaystyle {\vec {y}}=\mathbf {X} {\vec {\beta
      }}+{\vec {\varepsilon }}.\,}]
The vector of estimated polynomial regression coefficients (using ordinary
least_squares estimation) is
              &#x03B2; &#x2192;   &#x005E;    = (   X    T     X   )  &#x2212;
      1      X    T       y &#x2192;    ,    {\displaystyle {\widehat {\vec
      {\beta }}}=(\mathbf {X} ^{\mathsf {T}}\mathbf {X} )^{-1}\;\mathbf {X} ^
      {\mathsf {T}}{\vec {y}},\,}  [{\displaystyle {\widehat {\vec {\beta }}}=
      (\mathbf {X} ^{\mathsf {T}}\mathbf {X} )^{-1}\;\mathbf {X} ^{\mathsf {T}}
      {\vec {y}},\,}]
assuming m < n which is required for the matrix to be invertible; then since
X    {\displaystyle \mathbf {X} }  [\mathbf {X} ] is a Vandermonde_matrix, the
invertibility condition is guaranteed to hold if all the      x  i
{\displaystyle x_{i}}  [x_{i}] values are distinct. This is the unique least-
squares solution.
***** Interpretation[edit] *****
Although polynomial regression is technically a special case of multiple linear
regression, the interpretation of a fitted polynomial regression model requires
a somewhat different perspective. It is often difficult to interpret the
individual coefficients in a polynomial regression fit, since the underlying
monomials can be highly correlated. For example, x and x2 have correlation
around 0.97 when x is uniformly_distributed on the interval (0, 1). Although
the correlation can be reduced by using orthogonal_polynomials, it is generally
more informative to consider the fitted regression function as a whole. Point-
wise or simultaneous confidence_bands can then be used to provide a sense of
the uncertainty in the estimate of the regression function.
***** Alternative approaches[edit] *****
Polynomial regression is one example of regression analysis using basis
functions to model a functional relationship between two quantities. More
specifically, it replaces     x &#x2208;   R    d  x       {\displaystyle x\in
\mathbb {R} ^{d_{x}}}  [{\displaystyle x\in \mathbb {R} ^{d_{x}}}] in linear
regression with polynomial basis     &#x03C6; ( x ) &#x2208;   R    d  &#x03C6;
{\displaystyle \varphi (x)\in \mathbb {R} ^{d_{\varphi }}}  [{\displaystyle
\varphi (x)\in \mathbb {R} ^{d_{\varphi }}}], e.g.     [ 1 , x ]      &#x2192;
&#x03C6;      [ 1 , x ,  x  2   , &#x2026; ,  x  d   ]   {\displaystyle [1,x]
{\mathbin {\stackrel {\varphi }{\rightarrow }}}[1,x,x^{2},\ldots ,x^{d}]}  [
{\displaystyle [1,x]{\mathbin {\stackrel {\varphi }{\rightarrow }}}[1,x,x^
{2},\ldots ,x^{d}]}]. A drawback of polynomial bases is that the basis
functions are "non-local", meaning that the fitted value of y at a given value
x = x0 depends strongly on data values with x far from x0.[8] In modern
statistics, polynomial basis-functions are used along with new basis_functions,
such as splines, radial_basis_functions, and wavelets. These families of basis
functions offer a more parsimonious fit for many types of data.
The goal of polynomial regression is to model a non-linear relationship between
the independent and dependent variables (technically, between the independent
variable and the conditional mean of the dependent variable). This is similar
to the goal of nonparametric_regression, which aims to capture non-linear
regression relationships. Therefore, non-parametric regression approaches such
as smoothing can be useful alternatives to polynomial regression. Some of these
methods make use of a localized form of classical polynomial regression.[9] An
advantage of traditional polynomial regression is that the inferential
framework of multiple regression can be used (this also holds when using other
families of basis functions such as splines).
A final alternative is to use kernelized models such as support_vector
regression with a polynomial_kernel.
***** See also[edit] *****
    * Curve_fitting
    * Line_regression
    * Local_polynomial_regression
    * Polynomial_and_rational_function_modeling
    * Polynomial_interpolation
    * Response_surface_methodology
    * Smoothing_spline
***** Notes[edit] *****
    * Microsoft Excel makes use of polynomial regression when fitting a
      trendline to data points on an X Y scatter plot.[10]
***** References[edit] *****
   1. ^Shaw, P; et al. (2006). "Intellectual_ability_and_cortical_development
      in_children_and_adolescents". Nature. 440 (7084): 676â679. doi:10.1038/
      nature04513. PMID 16572172.
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
   3. ^Barker, PA; Street-Perrott, FA; Leng, MJ; Greenwood, PB; Swain, DL;
      Perrott, RA; Telford, RJ; Ficken, KJ (2001). "A 14,000-Year Oxygen
      Isotope Record from Diatom Silica in Two Alpine Lakes on Mt. Kenya".
      Science. 292 (5525): 2307â2310. doi:10.1126/science.1059612.
      PMID 11423656.
   4. ^Greenland, Sander (1995). "Dose-Response and Trend Analysis in
      Epidemiology: Alternatives to Categorical Analysis". Epidemiology. 6 (4):
      356â365. doi:10.1097/00001648-199507000-00005. JSTOR 3702080.
      PMID 7548341.
   5. ^Yin-Wen Chang; Cho-Jui Hsieh; Kai-Wei Chang; Michael Ringgaard; Chih-Jen
      Lin (2010). "Training_and_testing_low-degree_polynomial_data_mappings_via
      linear_SVM". Journal_of_Machine_Learning_Research. 11: 1471â1490.
   6. ^Gergonne,_J._D. (November 1974) [1815]. "The_application_of_the_method
      of_least_squares_to_the_interpolation_of_sequences". Historia Mathematica
      (Translated by Ralph St. John and S._M._Stigler from the 1815 French
      ed.). 1 (4): 439â447. doi:10.1016/0315-0860(74)90034-2.
   7. ^Stigler,_Stephen_M. (November 1974). "Gergonne's_1815_paper_on_the
      design_and_analysis_of_polynomial_regression_experiments". Historia
      Mathematica. 1 (4): 431â439. doi:10.1016/0315-0860(74)90033-0.
   8. ^Smith,_Kirstine (1918). "On_the_Standard_Deviations_of_Adjusted_and
      Interpolated_Values_of_an_Observed_Polynomial_Function_and_its_Constants
      and_the_Guidance_They_Give_Towards_a_Proper_Choice_of_the_Distribution_of
      the_Observations". Biometrika. 12 (1/2): 1â85. doi:10.2307/2331929.
      JSTOR 2331929.
   9. ^  Such "non-local" behavior is a property of analytic_functions that are
      not constant (everywhere). Such "non-local" behavior has been widely
      discussed in statistics:
          o Magee, Lonnie (1998). "Nonlocal Behavior in Polynomial
            Regressions". The American Statistician. 52 (1): 20â22. doi:
            10.2307/2685560. JSTOR 2685560.
  10. ^Fan, Jianqing (1996). Local Polynomial Modelling and Its Applications:
      From linear regression to nonlinear regression. Monographs on Statistics
      and Applied Probability. Chapman & Hall/CRC. ISBN 978-0-412-98321-4.
  11. ^Stevenson, Christopher. "Tutorial:_Polynomial_Regression_in_Excel".
      facultystaff.richmond.edu. Retrieved 22 January 2017.
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
Least_squares and regression_analysis
                               * Least_squares
Computational_statistics       * Linear_least_squares
                               * Non-linear_least_squares
                               * Iteratively_reweighted_least_squares
                               * Pearson_product-moment_correlation
                               * Rank_correlation (Spearman's_rho
Correlation_and_dependence     * Kendall's_tau)
                               * Partial_correlation
                               * Confounding_variable
                               * Ordinary_least_squares
Regression_analysis            * Partial_least_squares
                               * Total_least_squares
                               * Ridge_regression
                                                   * Simple_linear_regression
                                                   * Ordinary_least_squares
                           Linear_regression       * Generalized_least_squares
                                                   * Weighted_least_squares
                                                   * General_linear_model
                                                   * Polynomial regression
                           Predictor structure     * Growth_curve_(statistics)
                                                   * Segmented_regression
Regression as a                                    * Local_regression
statistical_model                                  * Nonlinear_regression
                                                   * Nonparametric
                           Non-standard            * Semiparametric
                                                   * Robust
                                                   * Quantile
                                                   * Isotonic
                                                   * Generalized_linear_model
                           Non-normal errors       * Binomial
                                                   * Poisson
                                                   * Logistic
                               * Analysis_of_variance
Decomposition_of_variance      * Analysis_of_covariance
                               * Multivariate_AOV
                               * Stepwise_regression
                               * Model_selection
                                     o Mallows's_Cp
Model exploration                    o AIC
                                     o BIC
                               * Model_specification
                               * Regression_validation
                               * Mean_and_predicted_response
                               * GaussâMarkov_theorem
Background                     * Errors_and_residuals
                               * Goodness_of_fit
                               * Studentized_residual
                               * Minimum_mean-square_error
                               * Response_surface_methodology
Design_of_experiments          * Optimal_design
                               * Bayesian_design
                               * Numerical_analysis
                               * Approximation_theory
                               * Numerical_integration
Numerical approximation        * Gaussian_quadrature
                               * Orthogonal_polynomials
                               * Chebyshev_polynomials
                               * Chebyshev_nodes
                               * Curve_fitting
                               * Calibration_curve
Applications                   * Numerical_smoothing_and_differentiation
                               * System_identification
                               * Moving_least_squares
    * Regression_analysis_category
    * Statistics_category
    * Statistics_portal
    * Statistics_outline
    * Statistics_topics
***** External links[edit] *****
    * Curve_Fitting, PhET Interactive simulations, University of Colorado at
      Boulder

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Polynomial_regression&oldid=904977508"
Categories:
    * Regression_analysis
Hidden categories:
    * Articles_to_be_merged_from_April_2018
    * All_articles_to_be_merged
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_March_2018
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÄeÅ¡tina
    * Eesti
    * FranÃ§ais
    * æ¥æ¬èª
    * Polski
    * ä¸­æ
Edit_links
    * This page was last edited on 5 July 2019, at 23:00 (UTC).
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
