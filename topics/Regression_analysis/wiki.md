The following text has been accessed from https://en.wikipedia.org/wiki/Regression_analysis at Thu Aug 8 22:52:11 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Regression analysis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Part of a series on Statistics
Regression analysis
[Linear_regression.svg]
Models
    * Linear_regression
    * Simple_regression
    * Polynomial_regression
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
Machine_learning and
data_mining
[Kernel_Machine.svg]
Problems
    * Classification
    * Clustering
    * Regression
    * Anomaly_detection
    * AutoML
    * Association_rules
    * Reinforcement_learning
    * Structured_prediction
    * Feature_engineering
    * Feature_learning
    * Online_learning
    * Semi-supervised_learning
    * Unsupervised_learning
    * Learning_to_rank
    * Grammar_induction
Supervised_learning
(classification • regression)
    * Decision_trees
    * Ensembles
          o Bagging
          o Boosting
          o Random_forest
    * k-NN
    * Linear_regression
    * Naive_Bayes
    * Artificial_neural_networks
    * Logistic_regression
    * Perceptron
    * Relevance_vector_machine_(RVM)
    * Support_vector_machine_(SVM)
Clustering
    * BIRCH
    * CURE
    * Hierarchical
    * k-means
    * Expectationâmaximization_(EM)
    *
      DBSCAN
    * OPTICS
    * Mean-shift
Dimensionality_reduction
    * Factor_analysis
    * CCA
    * ICA
    * LDA
    * NMF
    * PCA
    * t-SNE
Structured_prediction
    * Graphical_models
          o Bayes_net
          o Conditional_random_field
          o Hidden_Markov
Anomaly_detection
    * k-NN
    * Local_outlier_factor
Artificial_neural_networks
    * Autoencoder
    * Deep_learning
    * DeepDream
    * Multilayer_perceptron
    * RNN
          o LSTM
          o GRU
    * Restricted_Boltzmann_machine
    * GAN
    * SOM
    * Convolutional_neural_network
          o U-Net
Reinforcement_learning
    * Q-learning
    * SARSA
    * Temporal_difference_(TD)
Theory
    * Biasâvariance_dilemma
    * Computational_learning_theory
    * Empirical_risk_minimization
    * Occam_learning
    * PAC_learning
    * Statistical_learning
    * VC_theory
Machine-learning venues
    * NIPS
    * ICML
    * ML
    * JMLR
    * ArXiv:cs.LG
Glossary_of_artificial_intelligence
    * Glossary_of_artificial_intelligence
Related articles
    * List_of_datasets_for_machine-learning_research
    * Outline_of_machine_learning
    * v
    * t
    * e
In statistical_modeling, regression analysis is a set of statistical processes
for estimating the relationships among variables. It includes many techniques
for modeling and analyzing several variables, when the focus is on the
relationship between a dependent_variable and one or more independent_variables
(or 'predictors'). More specifically, regression analysis helps one understand
how the typical value of the dependent variable (or 'criterion variable')
changes when any one of the independent variables is varied, while the other
independent variables are held fixed.
Most commonly, regression analysis estimates the conditional_expectation of the
dependent variable given the independent variables â that is, the average
value of the dependent variable when the independent variables are fixed. Less
commonly, the focus is on a quantile, or other location_parameter of the
conditional distribution of the dependent variable given the independent
variables. In all cases, a function of the independent variables called the
regression function is to be estimated. In regression analysis, it is also of
interest to characterize the variation of the dependent variable around the
prediction of the regression function using a probability_distribution. A
related but distinct approach is Necessary Condition Analysis[1] (NCA), which
estimates the maximum (rather than average) value of the dependent variable for
a given value of the independent variable (ceiling line rather than central
line) in order to identify what value of the independent variable is necessary
but_not_sufficient for a given value of the dependent variable.
Regression analysis is widely used for prediction and forecasting, where its
use has substantial overlap with the field of machine_learning. Regression
analysis is also used to understand which among the independent variables are
related to the dependent variable, and to explore the forms of these
relationships. In restricted circumstances, regression analysis can be used to
infer causal_relationships between the independent and dependent variables.
However this can lead to illusions or false relationships, so caution is
advisable.
Many techniques for carrying out regression analysis have been developed.
Familiar methods such as linear_regression and ordinary_least_squares
regression are parametric, in that the regression function is defined in terms
of a finite number of unknown parameters that are estimated from the data.
Nonparametric_regression refers to techniques that allow the regression
function to lie in a specified set of functions, which may be infinite-
dimensional.
The performance of regression analysis methods in practice depends on the form
of the data_generating_process, and how it relates to the regression approach
being used. Since the true form of the data-generating process is generally not
known, regression analysis often depends to some extent on making assumptions
about this process. These assumptions are sometimes testable if a sufficient
quantity of data is available. Regression models for prediction are often
useful even when the assumptions are moderately violated, although they may not
perform optimally. However, in many applications, especially with small effects
or questions of causality based on observational_data, regression methods can
give misleading results.[2][3]
In a narrower sense, regression may refer specifically to the estimation of
continuous response (dependent) variables, as opposed to the discrete response
variables used in classification.[4] The case of a continuous dependent
variable may be more specifically referred to as metric regression to
distinguish it from related problems.[5]
⁰
***** Contents *****
    * 1_History
    * 2_Regression_models
          o 2.1_Necessary_number_of_independent_measurements
    * 3_Underlying_assumptions
    * 4_Linear_regression
          o 4.1_General_linear_model
          o 4.2_Diagnostics
          o 4.3_Limited_dependent_variables
    * 5_Nonlinear_regression
    * 6_Interpolation_and_extrapolation
    * 7_Power_and_sample_size_calculations
    * 8_Other_methods
    * 9_Software
    * 10_See_also
    * 11_References
    * 12_Further_reading
    * 13_External_links
***** History[edit] *****
The earliest form of regression was the method_of_least_squares, which was
published by Legendre in 1805,[6] and by Gauss in 1809.[7] Legendre and Gauss
both applied the method to the problem of determining, from astronomical
observations, the orbits of bodies about the Sun (mostly comets, but also later
the then newly discovered minor planets). Gauss published a further development
of the theory of least squares in 1821,[8] including a version of the
GaussâMarkov_theorem.
The term "regression" was coined by Francis_Galton in the nineteenth century to
describe a biological phenomenon. The phenomenon was that the heights of
descendants of tall ancestors tend to regress down towards a normal average (a
phenomenon also known as regression_toward_the_mean).[9][10] For Galton,
regression had only this biological meaning,[11][12] but his work was later
extended by Udny_Yule and Karl_Pearson to a more general statistical context.
[13][14] In the work of Yule and Pearson, the joint_distribution of the
response and explanatory variables is assumed to be Gaussian. This assumption
was weakened by R.A._Fisher in his works of 1922 and 1925.[15][16][17] Fisher
assumed that the conditional_distribution of the response variable is Gaussian,
but the joint distribution need not be. In this respect, Fisher's assumption is
closer to Gauss's formulation of 1821.
In the 1950s and 1960s, economists used electromechanical desk "calculators" to
calculate regressions. Before 1970, it sometimes took up to 24 hours to receive
the result from one regression.[18]
Regression methods continue to be an area of active research. In recent
decades, new methods have been developed for robust_regression, regression
involving correlated responses such as time_series and growth_curves,
regression in which the predictor (independent variable) or response variables
are curves, images, graphs, or other complex data objects, regression methods
accommodating various types of missing data, nonparametric_regression, Bayesian
methods for regression, regression in which the predictor variables are
measured with error, regression with more predictor variables than
observations, and causal inference with regression.
***** Regression models[edit] *****
Regression models involve the following parameters and variables:
    * The unknown parameters, denoted as     &#x03B2;   {\displaystyle \beta }
      [\beta ], which may represent a scalar or a vector.
    * The independent variables,     X   {\displaystyle X}  [X].
    * The dependent variable,     Y   {\displaystyle Y}  [Y].
In various fields_of_application, different terminologies are used in place of
dependent_and_independent_variables.
A regression model relates     Y   {\displaystyle Y}  [Y] to a function of
X   {\displaystyle X}  [X] and     &#x03B2;   {\displaystyle \beta }  [\beta ].
         Y &#x2248; f ( X , &#x03B2; ) .   {\displaystyle Y\approx f(X,\beta
      ).}  [{\displaystyle Y\approx f(X,\beta ).}]
The approximation is usually formalized as     E &#x2061; ( Y  |  X ) = f ( X ,
&#x03B2; )   {\displaystyle \operatorname {E} (Y|X)=f(X,\beta )}  [
{\displaystyle \operatorname {E} (Y|X)=f(X,\beta )}]. To carry out regression
analysis, the form of the function     f   {\displaystyle f}  [f] must be
specified. Sometimes the form of this function is based on knowledge about the
relationship between     Y   {\displaystyle Y}  [Y] and     X   {\displaystyle
X}  [X] that does not rely on the data. If no such knowledge is available, a
flexible or convenient form for     f   {\displaystyle f}  [f] is chosen.
Assume now that the vector of unknown parameters     &#x03B2;   {\displaystyle
\beta }  [\beta ] is of length     k   {\displaystyle k}  [k]. In order to
perform a regression analysis the user must provide information about the
dependent variable     Y   {\displaystyle Y}  [Y]:
    * If     N   {\displaystyle N}  [N] data points of the form     ( Y , X )
      {\displaystyle (Y,X)}  [{\displaystyle (Y,X)}] are observed, where     N
      < k   {\displaystyle N<k}  [{\displaystyle N<k}], most classical
      approaches to regression analysis cannot be performed: since the system
      of equations defining the regression model is underdetermined, there are
      not enough data to recover     &#x03B2;   {\displaystyle \beta }  [\beta
      ].
    * If exactly     N = k   {\displaystyle N=k}  [{\displaystyle N=k}] data
      points are observed, and the function     f   {\displaystyle f}  [f] is
      linear, the equations     Y = f ( X , &#x03B2; )   {\displaystyle Y=f
      (X,\beta )}  [{\displaystyle Y=f(X,\beta )}] can be solved exactly rather
      than approximately. This reduces to solving a set of     N
      {\displaystyle N}  [N] equations with     N   {\displaystyle N}  [N]
      unknowns (the elements of     &#x03B2; )   {\displaystyle \beta )}  [
      {\displaystyle \beta )}], which has a unique solution as long as the
      X   {\displaystyle X}  [X] are linearly independent. If     f
      {\displaystyle f}  [f] is nonlinear, a solution may not exist, or many
      solutions may exist.
    * The most common situation is where     N > k   {\displaystyle N>k}  [
      {\displaystyle N>k}] data points are observed. In this case, there is
      enough information in the data to estimate a unique value for
      &#x03B2;   {\displaystyle \beta }  [\beta ] that best fits the data in
      some sense, and the regression model when applied to the data can be
      viewed as an overdetermined_system in     &#x03B2;   {\displaystyle \beta
      }  [\beta ].
In the last case, the regression analysis provides the tools for:
   1. Finding a solution for unknown parameters     &#x03B2;   {\displaystyle
      \beta }  [\beta ] that will, for example, minimize the distance between
      the measured and predicted values of the dependent variable     Y
      {\displaystyle Y}  [Y] (also known as method of least_squares).
   2. Under certain statistical assumptions, the regression analysis uses the
      surplus of information to provide statistical information about the
      unknown parameters     &#x03B2;   {\displaystyle \beta }  [\beta ] and
      predicted values of the dependent variable     Y   {\displaystyle Y}
      [Y].
**** Necessary number of independent measurements[edit] ****
Consider a regression model which has three unknown parameters,      &#x03B2;
0     {\displaystyle \beta _{0}}  [\beta _{0}],      &#x03B2;  1
{\displaystyle \beta _{1}}  [\beta _{1}], and      &#x03B2;  2
{\displaystyle \beta _{2}}  [\beta _{2}]. Suppose an experimenter performs 10
measurements all at exactly the same value of independent variable vector     X
{\displaystyle X}  [X] (which contains the independent variables      X  1
{\displaystyle X_{1}}  [X_{1}],      X  2     {\displaystyle X_{2}}  [X_{2}],
and      X  3     {\displaystyle X_{3}}  [X_3]). In this case, regression
analysis fails to give a unique set of estimated values for the three unknown
parameters; the experimenter did not provide enough information. The best one
can do is to estimate the average value and the standard deviation of the
dependent variable     Y   {\displaystyle Y}  [Y]. Similarly, measuring at two
different values of     X   {\displaystyle X}  [X] would give enough data for a
regression with two unknowns, but not for three or more unknowns.
If the experimenter had performed measurements at three different values of the
independent variable vector     X   {\displaystyle X}  [ X], then regression
analysis would provide a unique set of estimates for the three unknown
parameters in     &#x03B2;   {\displaystyle \beta }  [\beta ].
In the case of general_linear_regression, the above statement is equivalent to
the requirement that the matrix      X  &#x22A4;   X   {\displaystyle X^{\top
}X}  [X^{\top }X] is invertible.
When the number of measurements,     N   {\displaystyle N}  [N], is larger than
the number of unknown parameters,     k   {\displaystyle k}  [k], and the
measurement errors      &#x03F5;  i     {\displaystyle \epsilon _{i}}
[\epsilon _{i}] are normally distributed then the excess of information
contained in     ( N &#x2212; k )   {\displaystyle (N-k)}  [{\displaystyle (N-
k)}] measurements is used to make statistical predictions about the unknown
parameters. This excess of information is referred to as the degrees_of_freedom
of the regression.
***** Underlying assumptions[edit] *****
Classical assumptions for regression analysis include:
    * The sample is representative of the population for the inference
      prediction.
    * The error is a random_variable with a mean of zero conditional on the
      explanatory variables.
    * The independent variables are measured with no error. (Note: If this is
      not so, modeling may be done instead using errors-in-variables_model
      techniques).
    * The independent variables (predictors) are linearly_independent, i.e. it
      is not possible to express any predictor as a linear combination of the
      others.
    * The errors are uncorrelated, that is, the varianceâcovariance_matrix of
      the errors is diagonal and each non-zero element is the variance of the
      error.
    * The variance of the error is constant across observations
      (homoscedasticity). If not, weighted_least_squares or other methods might
      instead be used.
These are sufficient conditions for the least-squares estimator to possess
desirable properties; in particular, these assumptions imply that the parameter
estimates will be unbiased, consistent, and efficient in the class of linear
unbiased estimators. It is important to note that actual data rarely satisfies
the assumptions. That is, the method is used even though the assumptions are
not true. Variation from the assumptions can sometimes be used as a measure of
how far the model is from being useful. Many of these assumptions may be
relaxed in more advanced treatments. Reports of statistical analyses usually
include analyses of tests on the sample data and methodology for the fit and
usefulness of the model.
Independent and dependent variables often refer to values measured at point
locations. There may be spatial trends and spatial autocorrelation in the
variables that violate statistical assumptions of regression. Geographic
weighted regression is one technique to deal with such data.[19] Also,
variables may include values aggregated by areas. With aggregated data the
modifiable_areal_unit_problem can cause extreme variation in regression
parameters.[20] When analyzing data aggregated by political boundaries, postal
codes or census areas results may be very distinct with a different choice of
units.
***** Linear regression[edit] *****
Main article: Linear_regression
See simple_linear_regression for a derivation of these formulas and a numerical
example
In linear regression, the model specification is that the dependent variable,
y  i     {\displaystyle y_{i}}  [y_{i}] is a linear_combination of the
parameters (but need not be linear in the independent variables). For example,
in simple_linear_regression for modeling     n   {\displaystyle n}  [n] data
points there is one independent variable:      x  i     {\displaystyle x_{i}}
[x_{i}], and two parameters,      &#x03B2;  0     {\displaystyle \beta _{0}}
[\beta _{0}] and      &#x03B2;  1     {\displaystyle \beta _{1}}  [\beta _{1}]:
      straight line:      y  i   =  &#x03B2;  0   +  &#x03B2;  1    x  i   +
      &#x03B5;  i   ,  i = 1 , &#x2026; , n .    {\displaystyle y_{i}=\beta _
      {0}+\beta _{1}x_{i}+\varepsilon _{i},\quad i=1,\dots ,n.\!}  [y_{i}=\beta
      _{0}+\beta _{1}x_{i}+\varepsilon _{i},\quad i=1,\dots ,n.\!]
In multiple linear regression, there are several independent variables or
functions of independent variables.
Adding a term in      x  i   2     {\displaystyle x_{i}^{2}}  [{\displaystyle
x_{i}^{2}}] to the preceding regression gives:
      parabola:      y  i   =  &#x03B2;  0   +  &#x03B2;  1    x  i   +
      &#x03B2;  2    x  i   2   +  &#x03B5;  i   , &#xA0; i = 1 , &#x2026; , n
      .    {\displaystyle y_{i}=\beta _{0}+\beta _{1}x_{i}+\beta _{2}x_{i}^
      {2}+\varepsilon _{i},\ i=1,\dots ,n.\!}  [y_{i}=\beta _{0}+\beta _{1}x_
      {i}+\beta _{2}x_{i}^{2}+\varepsilon _{i},\ i=1,\dots ,n.\!]
This is still linear regression; although the expression on the right hand side
is quadratic in the independent variable      x  i     {\displaystyle x_{i}}
[x_{i}], it is linear in the parameters      &#x03B2;  0     {\displaystyle
\beta _{0}}  [\beta _{0}],      &#x03B2;  1     {\displaystyle \beta _{1}}
[\beta _{1}] and      &#x03B2;  2   .   {\displaystyle \beta _{2}.}  [\beta _
{2}.]
In both cases,      &#x03B5;  i     {\displaystyle \varepsilon _{i}}
[\varepsilon _{i}] is an error term and the subscript     i   {\displaystyle i}
[i] indexes a particular observation.
Returning our attention to the straight line case: Given a random sample from
the population, we estimate the population parameters and obtain the sample
linear regression model:
             y &#x005E;     i   =     &#x03B2; &#x005E;     0   +     &#x03B2;
      &#x005E;     1    x  i   .   {\displaystyle {\widehat {y}}_{i}={\widehat
      {\beta }}_{0}+{\widehat {\beta }}_{1}x_{i}.}  [{\displaystyle {\widehat
      {y}}_{i}={\widehat {\beta }}_{0}+{\widehat {\beta }}_{1}x_{i}.}]
The residual,      e  i   =  y  i   &#x2212;     y &#x005E;     i
{\displaystyle e_{i}=y_{i}-{\widehat {y}}_{i}}  [e_{i}=y_{i}-{\widehat {y}}_
{i}], is the difference between the value of the dependent variable predicted
by the model,         y &#x005E;     i     {\displaystyle {\widehat {y}}_{i}}
[{\displaystyle {\widehat {y}}_{i}}], and the true value of the dependent
variable,      y  i     {\displaystyle y_{i}}  [y_{i}]. One method of
estimation is ordinary_least_squares. This method obtains parameter estimates
that minimize the sum of squared residuals, SSR:
         S S R =  &#x2211;  i = 1   n    e  i   2   .    {\displaystyle
      SSR=\sum _{i=1}^{n}e_{i}^{2}.\,}  [{\displaystyle SSR=\sum _{i=1}^{n}e_
      {i}^{2}.\,}]
Minimization of this function results in a set of normal_equations, a set of
simultaneous linear equations in the parameters, which are solved to yield the
parameter estimators,         &#x03B2; &#x005E;     0   ,     &#x03B2; &#x005E;
1     {\displaystyle {\widehat {\beta }}_{0},{\widehat {\beta }}_{1}}  [
{\widehat {\beta }}_{0},{\widehat {\beta }}_{1}].
Illustration of linear regression on a data set.
In the case of simple regression, the formulas for the least squares estimates
are
             &#x03B2; &#x005E;     1   =    &#x2211; (  x  i   &#x2212;    x
      &#x00AF;    ) (  y  i   &#x2212;    y &#x00AF;    )   &#x2211; (  x  i
      &#x2212;    x &#x00AF;     )  2        {\displaystyle {\widehat {\beta
      }}_{1}={\frac {\sum (x_{i}-{\bar {x}})(y_{i}-{\bar {y}})}{\sum (x_{i}-
      {\bar {x}})^{2}}}}  [{\displaystyle {\widehat {\beta }}_{1}={\frac {\sum
      (x_{i}-{\bar {x}})(y_{i}-{\bar {y}})}{\sum (x_{i}-{\bar {x}})^{2}}}}]
       &#x03B2; &#x005E;     0   =    y &#x00AF;    &#x2212;     &#x03B2;
&#x005E;     1      x &#x00AF;      {\displaystyle {\widehat {\beta }}_{0}=
{\bar {y}}-{\widehat {\beta }}_{1}{\bar {x}}}  [{\displaystyle {\widehat {\beta
}}_{0}={\bar {y}}-{\widehat {\beta }}_{1}{\bar {x}}}]
where        x &#x00AF;      {\displaystyle {\bar {x}}}  [{\bar {x}}] is the
mean (average) of the     x   {\displaystyle x}  [x] values and        y
&#x00AF;      {\displaystyle {\bar {y}}}  [{\bar {y}}] is the mean of the     y
{\displaystyle y}  [y] values.
Under the assumption that the population error term has a constant variance,
the estimate of that variance is given by:
             &#x03C3; &#x005E;     &#x03B5;   2   =    S S R   n &#x2212; 2
      .    {\displaystyle {\hat {\sigma }}_{\varepsilon }^{2}={\frac {SSR}{n-
      2}}.\,}  [{\displaystyle {\hat {\sigma }}_{\varepsilon }^{2}={\frac {SSR}
      {n-2}}.\,}]
This is called the mean_square_error (MSE) of the regression. The denominator
is the sample size reduced by the number of model parameters estimated from the
same data,     ( n &#x2212; p )   {\displaystyle (n-p)}  [{\displaystyle (n-
p)}] for     p   {\displaystyle p}  [p] regressors or     ( n &#x2212; p
&#x2212; 1 )   {\displaystyle (n-p-1)}  [{\displaystyle (n-p-1)}] if an
intercept is used.[21] In this case,     p = 1   {\displaystyle p=1}  [p=1] so
the denominator is     n &#x2212; 2   {\displaystyle n-2}  [n-2].
The standard_errors of the parameter estimates are given by
             &#x03C3; &#x005E;      &#x03B2;  1     =     &#x03C3; &#x005E;
      &#x03B5;      1  &#x2211; (  x  i   &#x2212;    x &#x00AF;     )  2
      {\displaystyle {\hat {\sigma }}_{\beta _{1}}={\hat {\sigma }}_
      {\varepsilon }{\sqrt {\frac {1}{\sum (x_{i}-{\bar {x}})^{2}}}}}  [
      {\displaystyle {\hat {\sigma }}_{\beta _{1}}={\hat {\sigma }}_
      {\varepsilon }{\sqrt {\frac {1}{\sum (x_{i}-{\bar {x}})^{2}}}}}]
             &#x03C3; &#x005E;      &#x03B2;  0     =     &#x03C3; &#x005E;
      &#x03B5;       1 n   +       x &#x00AF;     2    &#x2211; (  x  i
      &#x2212;    x &#x00AF;     )  2        =     &#x03C3; &#x005E;
      &#x03B2;  1         &#x2211;  x  i   2    n      {\displaystyle {\hat
      {\sigma }}_{\beta _{0}}={\hat {\sigma }}_{\varepsilon }{\sqrt {{\frac {1}
      {n}}+{\frac {{\bar {x}}^{2}}{\sum (x_{i}-{\bar {x}})^{2}}}}}={\hat
      {\sigma }}_{\beta _{1}}{\sqrt {\frac {\sum x_{i}^{2}}{n}}}}  [
      {\displaystyle {\hat {\sigma }}_{\beta _{0}}={\hat {\sigma }}_
      {\varepsilon }{\sqrt {{\frac {1}{n}}+{\frac {{\bar {x}}^{2}}{\sum (x_{i}-
      {\bar {x}})^{2}}}}}={\hat {\sigma }}_{\beta _{1}}{\sqrt {\frac {\sum x_
      {i}^{2}}{n}}}}].
Under the further assumption that the population error term is normally
distributed, the researcher can use these estimated standard errors to create
confidence_intervals and conduct hypothesis_tests about the population
parameters.
**** General linear model[edit] ****
For a derivation, see linear_least_squares
For a numerical example, see linear_regression
In the more general multiple regression model, there are     p   {\displaystyle
p}  [p] independent variables:
          y  i   =  &#x03B2;  1    x  i 1   +  &#x03B2;  2    x  i 2   +
      &#x22EF; +  &#x03B2;  p    x  i p   +  &#x03B5;  i   ,    {\displaystyle
      y_{i}=\beta _{1}x_{i1}+\beta _{2}x_{i2}+\cdots +\beta _{p}x_
      {ip}+\varepsilon _{i},\,}  [y_{i}=\beta _{1}x_{i1}+\beta _{2}x_
      {i2}+\cdots +\beta _{p}x_{ip}+\varepsilon _{i},\,]
where      x  i j     {\displaystyle x_{ij}}  [x_{ij}] is the     i
{\displaystyle i}  [i]-th observation on the     j   {\displaystyle j}  [j]-th
independent variable. If the first independent variable takes the value 1 for
all     i   {\displaystyle i}  [i],      x  i 1   = 1   {\displaystyle x_
{i1}=1}  [{\displaystyle x_{i1}=1}], then      &#x03B2;  1     {\displaystyle
\beta _{1}}  [\beta _{1}] is called the regression_intercept.
The least squares parameter estimates are obtained from     p   {\displaystyle
p}  [p] normal equations. The residual can be written as
          &#x03B5;  i   =  y  i   &#x2212;     &#x03B2; &#x005E;     1    x  i
      1   &#x2212; &#x22EF; &#x2212;     &#x03B2; &#x005E;     p    x  i p   .
      {\displaystyle \varepsilon _{i}=y_{i}-{\hat {\beta }}_{1}x_{i1}-\cdots -
      {\hat {\beta }}_{p}x_{ip}.}  [\varepsilon _{i}=y_{i}-{\hat {\beta }}_
      {1}x_{i1}-\cdots -{\hat {\beta }}_{p}x_{ip}.]
The normal equations are
          &#x2211;  i = 1   n    &#x2211;  k = 1   p    x  i j    x  i k
      &#x03B2; &#x005E;     k   =  &#x2211;  i = 1   n    x  i j    y  i   ,
      &#xA0; j = 1 , &#x2026; , p .    {\displaystyle \sum _{i=1}^{n}\sum _
      {k=1}^{p}x_{ij}x_{ik}{\hat {\beta }}_{k}=\sum _{i=1}^{n}x_{ij}y_{i},\
      j=1,\dots ,p.\,}  [{\displaystyle \sum _{i=1}^{n}\sum _{k=1}^{p}x_{ij}x_
      {ik}{\hat {\beta }}_{k}=\sum _{i=1}^{n}x_{ij}y_{i},\ j=1,\dots ,p.\,}]
In matrix notation, the normal equations are written as
          (  X  &#x22A4;   X )    &#x03B2; &#x005E;    =    X  &#x22A4;   Y  ,
      {\displaystyle \mathbf {(X^{\top }X){\hat {\boldsymbol {\beta }}}={}X^
      {\top }Y} ,\,}  [\mathbf {(X^{\top }X){\hat {\boldsymbol {\beta }}}={}X^
      {\top }Y} ,\,]
where the     i j   {\displaystyle ij}  [ij] element of      X
{\displaystyle \mathbf {X} }  [\mathbf {X} ] is      x  i j     {\displaystyle
x_{ij}}  [x_{ij}], the     i   {\displaystyle i}  [i] element of the column
vector     Y   {\displaystyle Y}  [Y] is      y  i     {\displaystyle y_{i}}
[y_{i}], and the     j   {\displaystyle j}  [j] element of        &#x03B2;
&#x005E;      {\displaystyle {\hat {\boldsymbol {\beta }}}}  [{\displaystyle
{\hat {\boldsymbol {\beta }}}}] is         &#x03B2; &#x005E;     j
{\displaystyle {\hat {\beta }}_{j}}  [{\hat {\beta }}_{j}]. Thus      X
{\displaystyle \mathbf {X} }  [\mathbf {X} ] is     n &#x00D7; p
{\displaystyle n\times p}  [n\times p],     Y   {\displaystyle Y}  [Y] is     n
&#x00D7; 1   {\displaystyle n\times 1}  [n\times 1], and        &#x03B2;
&#x005E;      {\displaystyle {\hat {\boldsymbol {\beta }}}}  [{\displaystyle
{\hat {\boldsymbol {\beta }}}}] is     p &#x00D7; 1   {\displaystyle p\times 1}
[p\times 1]. The solution is
             &#x03B2; &#x005E;    =   (  X  &#x22A4;   X  )  &#x2212; 1    X
      &#x22A4;   Y  .    {\displaystyle \mathbf {{\hat {\boldsymbol {\beta }}}=
      {}(X^{\top }X)^{-1}X^{\top }Y} .\,}  [\mathbf {{\hat {\boldsymbol {\beta
      }}}={}(X^{\top }X)^{-1}X^{\top }Y} .\,]
**** Diagnostics[edit] ****
Main article: Regression_diagnostics
See also: Category:Regression_diagnostics.
Once a regression model has been constructed, it may be important to confirm
the goodness_of_fit of the model and the statistical_significance of the
estimated parameters. Commonly used checks of goodness of fit include the R-
squared, analyses of the pattern of residuals and hypothesis testing.
Statistical significance can be checked by an F-test of the overall fit,
followed by t-tests of individual parameters.
Interpretations of these diagnostic tests rest heavily on the model
assumptions. Although examination of the residuals can be used to invalidate a
model, the results of a t-test or F-test are sometimes more difficult to
interpret if the model's assumptions are violated. For example, if the error
term does not have a normal distribution, in small samples the estimated
parameters will not follow normal distributions and complicate inference. With
relatively large samples, however, a central_limit_theorem can be invoked such
that hypothesis testing may proceed using asymptotic approximations.
**** Limited dependent variables[edit] ****
Limited_dependent_variables, which are response variables that are categorical
variables or are variables constrained to fall only in a certain range, often
arise in econometrics.
The response variable may be non-continuous ("limited" to lie on some subset of
the real line). For binary (zero or one) variables, if analysis proceeds with
least-squares linear regression, the model is called the linear_probability
model. Nonlinear models for binary dependent variables include the probit and
logit_model. The multivariate_probit model is a standard method of estimating a
joint relationship between several binary dependent variables and some
independent variables. For categorical_variables with more than two values
there is the multinomial_logit. For ordinal_variables with more than two
values, there are the ordered_logit and ordered_probit models. Censored
regression_models may be used when the dependent variable is only sometimes
observed, and Heckman_correction type models may be used when the sample is not
randomly selected from the population of interest. An alternative to such
procedures is linear regression based on polychoric_correlation (or polyserial
correlations) between the categorical variables. Such procedures differ in the
assumptions made about the distribution of the variables in the population. If
the variable is positive with low values and represents the repetition of the
occurrence of an event, then count models like the Poisson_regression or the
negative_binomial model may be used.
***** Nonlinear regression[edit] *****
Main article: Nonlinear_regression
When the model function is not linear in the parameters, the sum of squares
must be minimized by an iterative procedure. This introduces many complications
which are summarized in Differences_between_linear_and_non-linear_least
squares.
***** Interpolation and extrapolation[edit] *****
In the middle, the interpolated straight line represents the best balance
between the points above and below this line. The dotted lines represent the
two extreme lines. The first curves represent the estimated values. The outer
curves represent a prediction for a new measurement.[22]
Regression models predict a value of the Y variable given known values of the X
variables. Prediction within the range of values in the dataset used for model-
fitting is known informally as interpolation. Prediction outside this range of
the data is known as extrapolation. Performing extrapolation relies strongly on
the regression assumptions. The further the extrapolation goes outside the
data, the more room there is for the model to fail due to differences between
the assumptions and the sample data or the true values.
It is generally advised[citation_needed] that when performing extrapolation,
one should accompany the estimated value of the dependent variable with a
prediction_interval that represents the uncertainty. Such intervals tend to
expand rapidly as the values of the independent variable(s) moved outside the
range covered by the observed data.
For such reasons and others, some tend to say that it might be unwise to
undertake extrapolation.[23]
However, this does not cover the full set of modeling errors that may be made:
in particular, the assumption of a particular form for the relation between Y
and X. A properly conducted regression analysis will include an assessment of
how well the assumed form is matched by the observed data, but it can only do
so within the range of values of the independent variables actually available.
This means that any extrapolation is particularly reliant on the assumptions
being made about the structural form of the regression relationship. Best-
practice advice here[citation_needed] is that a linear-in-variables and linear-
in-parameters relationship should not be chosen simply for computational
convenience, but that all available knowledge should be deployed in
constructing a regression model. If this knowledge includes the fact that the
dependent variable cannot go outside a certain range of values, this can be
made use of in selecting the model â even if the observed dataset has no
values particularly near such bounds. The implications of this step of choosing
an appropriate functional form for the regression can be great when
extrapolation is considered. At a minimum, it can ensure that any extrapolation
arising from a fitted model is "realistic" (or in accord with what is known).
***** Power and sample size calculations[edit] *****
There are no generally agreed methods for relating the number of observations
versus the number of independent variables in the model. One rule of thumb
conjectured by Good and Hardin is     N =  m  n     {\displaystyle N=m^{n}}
[N=m^{n}], where     N   {\displaystyle N}  [N] is the sample size,     n
{\displaystyle n}  [n] is the number of independent variables and     m
{\displaystyle m}  [m] is the number of observations needed to reach the
desired precision if the model had only one independent variable.[24] For
example, a researcher is building a linear regression model using a dataset
that contains 1000 patients (    N   {\displaystyle N}  [N]). If the researcher
decides that five observations are needed to precisely define a straight line
(    m   {\displaystyle m}  [m]), then the maximum number of independent
variables the model can support is 4, because
      log &#x2061;  1000    log &#x2061;  5     = 4.29   {\displaystyle {\frac
{\log {1000}}{\log {5}}}=4.29}  [{\frac {\log {1000}}{\log {5}}}=4.29].
***** Other methods[edit] *****
Although the parameters of a regression model are usually estimated using the
method of least squares, other methods which have been used include:
    * Bayesian_methods, e.g. Bayesian_linear_regression
    * Percentage regression, for situations where reducing percentage errors is
      deemed more appropriate.[25]
    * Least_absolute_deviations, which is more robust in the presence of
      outliers, leading to quantile_regression
    * Nonparametric_regression, requires a large number of observations and is
      computationally intensive
    * Scenario_Optimization, leading to Interval_Predictor_Models
    * Distance metric learning, which is learned by the search of a meaningful
      distance metric in a given input space.[26]
***** Software[edit] *****
For a more comprehensive list, see List_of_statistical_packages.
All major statistical software packages perform least_squares regression
analysis and inference. Simple_linear_regression and multiple regression using
least squares can be done in some spreadsheet applications and on some
calculators. While many statistical software packages can perform various types
of nonparametric and robust regression, these methods are less standardized;
different software packages implement different methods, and a method with a
given name may be implemented differently in different packages. Specialized
regression software has been developed for use in fields such as survey
analysis and neuroimaging.
***** See also[edit] *****
    * [icon]Statistics_portal
    * Curve_fitting
    * Estimation_Theory
    * Forecasting
    * Fraction_of_variance_unexplained
    * Function_approximation
    * Generalized_linear_models
    * Kriging (a linear least squares estimation algorithm)
    * Local_regression
    * Modifiable_areal_unit_problem
    * Multivariate_adaptive_regression_splines
    * Multivariate_normal_distribution
    * Pearson_product-moment_correlation_coefficient
    * Quasi-variance
    * Prediction_interval
    * Regression_validation
    * Robust_regression
    * Segmented_regression
    * Signal_processing
    * Stepwise_regression
    * Trend_estimation
***** References[edit] *****
   1. ^ Necessary_Condition_Analysis
   2. ^David A. Freedman (27 April 2009). Statistical_Models:_Theory_and
      Practice. Cambridge University Press. ISBN 978-1-139-47731-4.
   3. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   4. ^ R. Dennis Cook; Sanford Weisberg Criticism_and_Influence_Analysis_in
      Regression, Sociological Methodology, Vol. 13. (1982), pp. 313â361
   5. ^Christopher M. Bishop (2006). Pattern Recognition and Machine Learning.
      Springer. p. 3. Cases [...] in which the aim is to assign each input
      vector to one of a finite number of discrete categories, are called
      classification problems. If the desired output consists of one or more
      continuous dependent variables, then the task is called regression.
   6. ^Waegeman, Willem; De Baets, Bernard; Boullart, Luc (2008). "ROC_analysis
      in_ordinal_regression_learning". Pattern Recognition Letters. 29: 1â9.
      doi:10.1016/j.patrec.2007.07.019.
   7. ^ A.M._Legendre. Nouvelles_mÃ©thodes_pour_la_dÃ©termination_des_orbites
      des_comÃ¨tes, Firmin Didot, Paris, 1805. âSur la MÃ©thode des moindres
      quarrÃ©sâ appears as an appendix.
   8. ^ C.F._Gauss. Theoria Motus Corporum Coelestium in Sectionibus Conicis
      Solem Ambientum. (1809)
   9. ^ C.F. Gauss. Theoria_combinationis_observationum_erroribus_minimis
      obnoxiae. (1821/1823)
  10. ^ Mogull, Robert G. (2004). Second-Semester Applied Statistics. Kendall/
      Hunt Publishing Company. p. 59. ISBN 978-0-7575-1181-3.
  11. ^Galton, Francis (1989). "Kinship and Correlation (reprinted 1989)".
      Statistical Science. 4 (2): 80â86. doi:10.1214/ss/1177012581.
      JSTOR 2245330.
  12. ^ Francis_Galton. "Typical laws of heredity", Nature 15 (1877),
      492â495, 512â514, 532â533. (Galton uses the term "reversion" in
      this paper, which discusses the size of peas.)
  13. ^ Francis Galton. Presidential address, Section H, Anthropology. (1885)
      (Galton uses the term "regression" in this paper, which discusses the
      height of humans.)
  14. ^Yule,_G._Udny (1897). "On_the_Theory_of_Correlation". Journal of the
      Royal Statistical Society. 60 (4): 812â54. doi:10.2307/2979746.
      JSTOR 2979746.
  15. ^Pearson,_Karl; Yule, G.U.; Blanchard, Norman; Lee,Alice (1903). "The_Law
      of_Ancestral_Heredity". Biometrika. 2 (2): 211â236. doi:10.1093/biomet/
      2.2.211. JSTOR 2331683.
  16. ^Fisher, R.A. (1922). "The_goodness_of_fit_of_regression_formulae,_and
      the_distribution_of_regression_coefficients". Journal of the Royal
      Statistical Society. 85 (4): 597â612. doi:10.2307/2341124.
      JSTOR 2341124. PMC 1084801.
  17. ^Ronald_A._Fisher (1954). Statistical_Methods_for_Research_Workers
      (Twelfth ed.). Edinburgh: Oliver and Boyd. ISBN 978-0-05-002170-5.
  18. ^Aldrich, John (2005). "Fisher and Regression". Statistical Science. 20
      (4): 401â417. doi:10.1214/088342305000000331. JSTOR 20061201.
  19. ^ Rodney Ramcharan. Regressions:_Why_Are_Economists_Obessessed_with_Them?
      March 2006. Accessed 2011-12-03.
  20. ^Fotheringham, A. Stewart; Brunsdon, Chris; Charlton, Martin (2002).
      Geographically weighted regression: the analysis of spatially varying
      relationships (Reprint ed.). Chichester, England: John Wiley. ISBN 978-0-
      471-49616-8.
  21. ^Fotheringham, AS; Wong, DWS (1 January 1991). "The modifiable areal unit
      problem in multivariate statistical analysis". Environment and Planning
      A. 23 (7): 1025â1044. doi:10.1068/a231025.
  22. ^ Steel, R.G.D, and Torrie, J. H., Principles and Procedures of
      Statistics with Special Reference to the Biological Sciences., McGraw
      Hill, 1960, page 288.
  23. ^Rouaud, Mathieu (2013). Probability,_Statistics_and_Estimation (PDF).
      p. 60.
  24. ^ Chiang, C.L, (2003) Statistical methods of analysis, World Scientific.
  25. ISBN 981-238-310-7 - page_274_section_9.7.4_"interpolation_vs
      extrapolation"
  26. ^Good,_P._I.; Hardin, J. W. (2009). Common Errors in Statistics (And How
      to Avoid Them) (3rd ed.). Hoboken, New Jersey: Wiley. p. 211. ISBN 978-0-
      470-45798-6.
  27. ^Tofallis, C. (2009). "Least Squares Percentage Regression". Journal of
      Modern Applied Statistical Methods. 7: 526â534. doi:10.2139/
      ssrn.1406472. SSRN 1406472.
  28. ^YangJing Long (2009). "Human_age_estimation_by_metric_learning_for
      regression_problems" (PDF). Proc. International Conference on Computer
      Analysis of Images and Patterns: 74â82. Archived from the_original
      (PDF) on 2010-01-08.
***** Further reading[edit] *****
    * William_H._Kruskal and Judith_M._Tanur, ed. (1978), "Linear Hypotheses,"
      International Encyclopedia of Statistics. Free Press, v. 1,
      Evan J. Williams, "I. Regression," pp. 523â41.
      Julian_C._Stanley, "II. Analysis of Variance," pp. 541â554.
    * Lindley,_D.V. (1987). "Regression and correlation analysis," New
      Palgrave:_A_Dictionary_of_Economics, v. 4, pp. 120â23.
    * Birkes, David and Dodge,_Y., Alternative Methods of Regression.
ISBN 0-471-56881-3
Chatfield, C. (1993) "Calculating_Interval_Forecasts," Journal of Business and
Economic Statistics, 11. pp. 121â135.
Draper, N.R.; Smith, H. (1998). Applied Regression Analysis (3rd ed.). John
Wiley. ISBN 978-0-471-17082-2.
Fox, J. (1997). Applied Regression Analysis, Linear Models and Related Methods.
Sage
Hardle, W., Applied Nonparametric Regression (1990),
ISBN 0-521-42950-1
Meade, Nigel; Islam, Towhidul (1995). "Prediction intervals for growth curve
forecasts". Journal of Forecasting. 14 (5): 413â430. doi:10.1002/
for.3980140502.
A. Sen, M. Srivastava, Regression Analysis — Theory, Methods, and Applications,
Springer-Verlag, Berlin, 2011 (4th printing).
T. Strutz: Data Fitting and Uncertainty (A practical introduction to weighted
least squares and beyond). Vieweg+Teubner,
ISBN 978-3-8348-1022-9.
Malakooti, B. (2013). Operations_and_Production_Systems_with_Multiple
Objectives. John Wiley & Sons.
***** External links[edit] *****
 Wikimedia Commons has media related to Regression_analysis.
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Regression_analysis",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Earliest_Uses:_Regression â basic history and references
Regression_of_Weakly_Correlated_Data â how linear regression mistakes can
appear when Y-range is much smaller than X-range
    * v
    * t
    * e
Least_squares and regression analysis
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
Regression analysis            * Partial_least_squares
                               * Total_least_squares
                               * Ridge_regression
                                                   * Simple_linear_regression
                                                   * Ordinary_least_squares
                           Linear_regression       * Generalized_least_squares
                                                   * Weighted_least_squares
                                                   * General_linear_model
                                                   * Polynomial_regression
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
    * Regression analysis
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
Quantitative forecasting methods
Historical data forecasts
    * Moving_average
    * Exponential_smoothing
    * Trend_analysis
    * Decomposition_of_time_series
    * NaÃ¯ve_approach
Associative (causal) forecasts
Moving_average
Simple_linear_regression
Regression analysis
Econometric_model
    * v
    * t
    * e
Public_health
                               * Auxology
                               * Biological_hazard
                               * Chief_Medical_Officer
                               * Cultural_competence
                               * Deviance
                               * Environmental_health
                               * Euthenics
                               * Genomics
                               * Globalization_and_disease
                               * Health_economics
                               * Health_literacy
                               * Health_policy
General                              o Health_system
                                     o Health_care_reform
                                     o Public_health_law
                               * Maternal_health
                               * Medical_anthropology
                               * Medical_sociology
                               * Mental_health
                               * Pharmaceutical_policy
                               * Public_health_intervention
                               * Public_health_laboratory
                               * Reproductive_health
                               * Social_psychology
                               * Sociology_of_health_and_illness
                               * Behavior_change
                                     o Theories
                               * Family_planning
                               * Health_promotion
                               * Human_nutrition
                               * Preventive_nutrition
                               * Hygiene
                                     o Food_safety
                                     o Hand_washing
                                     o Infection_control
                                     o Oral_hygiene
                               * Occupational_safety_and_health
                                     o Human_factors_and_ergonomics
                                     o Hygiene
Preventive_healthcare                o Injury_prevention
                                     o Medicine
                                     o Nursing
                               * Patient_safety
                                     o Organization
                               * Pharmacovigilance
                               * Safe_sex
                               * Sanitation
                                     o Emergency
                                     o Fecalâoral_transmission
                                     o Open_defecation
                                     o Sanitary_sewer
                                     o Waterborne_diseases
                               * Smoking_cessation
                               * Vaccination
                               * Vector_control
                               * Biostatistics
                               * Child_mortality
                               * Community_health
                               * Epidemiology
                               * Global_health
                               * Health_impact_assessment
Population_health              * Health_system
                               * Infant_mortality
                               * Open-source_healthcare_software
                               * Public_health_informatics
                               * Social_determinants_of_health
                                     o Health_equity
                                     o Race_and_health
                               * Social_medicine
                               * Caseâcontrol_study
                               * Randomized_controlled_trial
                               * Relative_risk
                               * Statistical_hypothesis_testing
Biological and                       o Analysis_of_variance_(ANOVA)
epidemiological statistics           o Regression analysis
                                     o ROC_curve
                                     o Student's_t-test
                                     o Z-test
                               * Statistical_software
                               * Asymptomatic_carrier
                               * Epidemics
                                     o List
                               * Notifiable_diseases
Infectious and epidemic              o List
disease prevention             * Public_health_surveillance
                                     o Disease_surveillance
                               * Quarantine
                               * Sexually_transmitted_infection
                               * Tropical_disease
                               * Vaccine_trial
                               * Food
                                     o Additive
                                     o Chemistry
                                     o Engineering
                                     o Microbiology
Food hygiene and                     o Processing
safety management                    o Safety
                                     o Safety_scandals
                               * Genetically_modified_food
                               * Good_agricultural_practice
                               * Good_manufacturing_practice
                                     o HACCP
                                     o ISO_22000
                               * Diffusion_of_innovations
                               * Health_belief_model
                               * Health_communication
                               * Health_psychology
Health behavioral              * Positive_deviance
sciences                       * PRECEDE-PROCEED_model
                               * Social_cognitive_theory
                               * Social_norms_approach
                               * Theory_of_planned_behavior
                               * Transtheoretical_model
                                             * Europe
                                                   o Centre_for_Disease
                                                     Prevention_and_Control
                                                   o Committee_on_the
                                                     Environment,_Public_Health
                                                     and_Food_Safety
                                             * India
                                                   o Ministry_of_Health_and
                                                     Family_Welfare
                           Organizations     * U.S.
                                                   o Centers_for_Disease
                                                     Control_and_Prevention
                                                   o City_and_county_health
                                                     departments
                                                   o Council_on_Education_for
                                                     Public_Health
Organizations,                                     o Public_Health_Service
education                                    * World_Health_Organization
and history                                  * World_Toilet_Organization
                                             * Health_education
                                             * Higher education
                                                   o Bachelor_of_Science_in
                           Education                 Public_Health
                                                   o Doctor_of_Public_Health
                                                   o Professional_degrees_of
                                                     public_health
                                                   o Schools_of_public_health
                                             * Sara_Josephine_Baker
                                             * Samuel_Jay_Crumbine
                                             * Carl_Rogers_Darnall
                                             * Joseph_Lister
                           History           * Margaret_Sanger
                                             * John_Snow
                                             * Typhoid_Mary
                                             * Germ_theory_of_disease
                                             * Social_hygiene_movement
    * [Category] Category
    * [Commons page] Commons
    * [WikiProject] WikiProject
                                              * BNF: cb119445648 (data)
Authority_control [Edit_this_at_Wikidata]     * GND: 4129903-6
                                              * LCCN: sh85112392
                                              * NDL: 00564579

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Regression_analysis&oldid=909054093"
Categories:
    * Regression_analysis
    * Estimation_theory
    * Actuarial_science
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_February_2010
    * Articles_with_unsourced_statements_from_March_2011
    * Commons_category_link_is_on_Wikidata
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
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
    * Asturianu
    * AzÉrbaycanca
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Jawa
    * LatvieÅ¡u
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * Suomi
    * Svenska
    * Tagalog
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 2 August 2019, at 19:23 (UTC).
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
