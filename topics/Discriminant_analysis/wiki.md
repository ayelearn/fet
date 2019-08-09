The following text has been accessed from https://en.wikipedia.org/wiki/Linear_discriminant_analysis at Fri Aug 9 02:54:36 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Linear discriminant analysis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with latent_Dirichlet_allocation.
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
Linear discriminant analysis (LDA), normal discriminant analysis (NDA), or
discriminant function analysis is a generalization of Fisher's linear
discriminant, a method used in statistics, pattern_recognition and machine
learning to find a linear_combination of features that characterizes or
separates two or more classes of objects or events. The resulting combination
may be used as a linear_classifier, or, more commonly, for dimensionality
reduction before later classification.
LDA is closely related to analysis_of_variance (ANOVA) and regression_analysis,
which also attempt to express one dependent_variable as a linear combination of
other features or measurements.[1][2] However, ANOVA uses categorical
independent_variables and a continuous dependent_variable, whereas discriminant
analysis has continuous independent_variables and a categorical dependent
variable (i.e. the class label).[3] Logistic_regression and probit_regression
are more similar to LDA than ANOVA is, as they also explain a categorical
variable by the values of continuous independent variables. These other methods
are preferable in applications where it is not reasonable to assume that the
independent variables are normally distributed, which is a fundamental
assumption of the LDA method.
LDA is also closely related to principal_component_analysis (PCA) and factor
analysis in that they both look for linear combinations of variables which best
explain the data.[4] LDA explicitly attempts to model the difference between
the classes of data. PCA on the other hand does not take into account any
difference in class, and factor analysis builds the feature combinations based
on differences rather than similarities. Discriminant analysis is also
different from factor analysis in that it is not an interdependence technique:
a distinction between independent variables and dependent variables (also
called criterion variables) must be made.
LDA works when the measurements made on independent variables for each
observation are continuous quantities. When dealing with categorical
independent variables, the equivalent technique is discriminant correspondence
analysis.[5][6]
Discriminant analysis is used when groups are known a priori (unlike in cluster
analysis). Each case must have a score on one or more quantitative predictor
measures, and a score on a group measure.[7] In simple terms, discriminant
function analysis is classification - the act of distributing things into
groups, classes or categories of the same type.
⁰
***** Contents *****
    * 1_History
    * 2_LDA_for_two_classes
    * 3_Assumptions
    * 4_Discriminant_functions
    * 5_Discrimination_rules
    * 6_Eigenvalues
    * 7_Effect_size
    * 8_Canonical_discriminant_analysis_for_k_classes
    * 9_Fisher's_linear_discriminant
    * 10_Multiclass_LDA
    * 11_Incremental_LDA
    * 12_Practical_use
    * 13_Applications
          o 13.1_Bankruptcy_prediction
          o 13.2_Face_recognition
          o 13.3_Marketing
          o 13.4_Biomedical_studies
          o 13.5_Earth_science
    * 14_Comparison_to_logistic_regression
    * 15_Linear_discriminant_in_high_dimension
    * 16_See_also
    * 17_References
    * 18_Further_reading
    * 19_External_links
***** History[edit] *****
The original dichotomous discriminant analysis was developed by Sir Ronald
Fisher in 1936.[8] It is different from an ANOVA or MANOVA, which is used to
predict one (ANOVA) or multiple (MANOVA) continuous dependent variables by one
or more independent categorical variables. Discriminant function analysis is
useful in determining whether a set of variables is effective in predicting
category membership.[9]
***** LDA for two classes[edit] *****
Consider a set of observations        x &#x2192;      {\displaystyle {\vec
{x}}}  [{\vec {x}}] (also called features, attributes, variables or
measurements) for each sample of an object or event with known class     y
{\displaystyle y}  [y]. This set of samples is called the training_set. The
classification problem is then to find a good predictor for the class     y
{\displaystyle y}  [y] of any sample of the same distribution (not necessarily
from the training set) given only an observation        x &#x2192;
{\displaystyle {\vec {x}}}  [{\vec {x}}].[10]:338
LDA approaches the problem by assuming that the conditional probability_density
functions     p (    x &#x2192;     |  y = 0 )   {\displaystyle p({\vec
{x}}|y=0)}  [p({\vec {x}}|y=0)] and     p (    x &#x2192;     |  y = 1 )
{\displaystyle p({\vec {x}}|y=1)}  [p({\vec {x}}|y=1)] are both normally
distributed with mean and covariance parameters      (      &#x03BC; &#x2192;
0   ,  &#x03A3;  0    )    {\displaystyle \left({\vec {\mu }}_{0},\Sigma _
{0}\right)}  [\left({\vec {\mu }}_{0},\Sigma _{0}\right)] and
(      &#x03BC; &#x2192;     1   ,  &#x03A3;  1    )    {\displaystyle \left(
{\vec {\mu }}_{1},\Sigma _{1}\right)}  [\left({\vec {\mu }}_{1},\Sigma _
{1}\right)], respectively. Under this assumption, the Bayes optimal solution is
to predict points as being from the second class if the log of the likelihood
ratios is bigger than some threshold T, so that:
         (    x &#x2192;    &#x2212;     &#x03BC; &#x2192;     0    )  T
      &#x03A3;  0   &#x2212; 1   (    x &#x2192;    &#x2212;     &#x03BC;
      &#x2192;     0   ) + ln &#x2061;  |   &#x03A3;  0    |  &#x2212; (    x
      &#x2192;    &#x2212;     &#x03BC; &#x2192;     1    )  T    &#x03A3;  1
      &#x2212; 1   (    x &#x2192;    &#x2212;     &#x03BC; &#x2192;     1   )
      &#x2212; ln &#x2061;  |   &#x03A3;  1    |  &#xA0; > &#xA0; T
      {\displaystyle ({\vec {x}}-{\vec {\mu }}_{0})^{T}\Sigma _{0}^{-1}({\vec
      {x}}-{\vec {\mu }}_{0})+\ln |\Sigma _{0}|-({\vec {x}}-{\vec {\mu }}_{1})^
      {T}\Sigma _{1}^{-1}({\vec {x}}-{\vec {\mu }}_{1})-\ln |\Sigma _{1}|\ >\
      T}  [({\vec {x}}-{\vec {\mu }}_{0})^{T}\Sigma _{0}^{-1}({\vec {x}}-{\vec
      {\mu }}_{0})+\ln |\Sigma _{0}|-({\vec {x}}-{\vec {\mu }}_{1})^{T}\Sigma _
      {1}^{-1}({\vec {x}}-{\vec {\mu }}_{1})-\ln |\Sigma _{1}|\ >\ T]
Without any further assumptions, the resulting classifier is referred to as QDA
(quadratic_discriminant_analysis).
LDA instead makes the additional simplifying homoscedasticity assumption (i.e.
that the class covariances are identical, so      &#x03A3;  0   =  &#x03A3;  1
= &#x03A3;   {\displaystyle \Sigma _{0}=\Sigma _{1}=\Sigma }  [\Sigma _
{0}=\Sigma _{1}=\Sigma ]) and that the covariances have full rank. In this
case, several terms cancel:
             x &#x2192;     T    &#x03A3;  0   &#x2212; 1      x &#x2192;    =
      x &#x2192;     T    &#x03A3;  1   &#x2212; 1      x &#x2192;
      {\displaystyle {\vec {x}}^{T}\Sigma _{0}^{-1}{\vec {x}}={\vec {x}}^
      {T}\Sigma _{1}^{-1}{\vec {x}}}  [{\vec {x}}^{T}\Sigma _{0}^{-1}{\vec
      {x}}={\vec {x}}^{T}\Sigma _{1}^{-1}{\vec {x}}]
             x &#x2192;     T      &#x03A3;  i     &#x2212; 1       &#x03BC;
      &#x2192;     i   =       &#x03BC; &#x2192;     i     T      &#x03A3;  i
      &#x2212; 1      x &#x2192;      {\displaystyle {\vec {x}}^{T}{\Sigma _
      {i}}^{-1}{\vec {\mu }}_{i}={{\vec {\mu }}_{i}}^{T}{\Sigma _{i}}^{-1}{\vec
      {x}}}  [{\displaystyle {\vec {x}}^{T}{\Sigma _{i}}^{-1}{\vec {\mu }}_{i}=
      {{\vec {\mu }}_{i}}^{T}{\Sigma _{i}}^{-1}{\vec {x}}}] because
      &#x03A3;  i     {\displaystyle \Sigma _{i}}  [\Sigma _{i}] is Hermitian
and the above decision criterion becomes a threshold on the dot_product
            w &#x2192;    &#x22C5;    x &#x2192;    > c   {\displaystyle {\vec
      {w}}\cdot {\vec {x}}>c}  [{\vec {w}}\cdot {\vec {x}}>c]
for some threshold constant c, where
            w &#x2192;    =  &#x03A3;  &#x2212; 1   (     &#x03BC; &#x2192;
      1   &#x2212;     &#x03BC; &#x2192;     0   )   {\displaystyle {\vec
      {w}}=\Sigma ^{-1}({\vec {\mu }}_{1}-{\vec {\mu }}_{0})}  [{\vec
      {w}}=\Sigma ^{-1}({\vec {\mu }}_{1}-{\vec {\mu }}_{0})]
         c =   1 2   ( T &#x2212;       &#x03BC; &#x2192;     0     T
      &#x03A3;  &#x2212; 1        &#x03BC; &#x2192;     0    +       &#x03BC;
      &#x2192;     1     T    &#x03A3;  &#x2212; 1        &#x03BC; &#x2192;
      1    )   {\displaystyle c={\frac {1}{2}}(T-{{\vec {\mu }}_{0}}^{T}\Sigma
      ^{-1}{{\vec {\mu }}_{0}}+{{\vec {\mu }}_{1}}^{T}\Sigma ^{-1}{{\vec {\mu
      }}_{1}})}  [{\displaystyle c={\frac {1}{2}}(T-{{\vec {\mu }}_{0}}^
      {T}\Sigma ^{-1}{{\vec {\mu }}_{0}}+{{\vec {\mu }}_{1}}^{T}\Sigma ^{-1}{
      {\vec {\mu }}_{1}})}]
This means that the criterion of an input        x &#x2192;      {\displaystyle
{\vec {x}}}  [{\displaystyle {\vec {x}}}] being in a class     y
{\displaystyle y}  [y] is purely a function of this linear combination of the
known observations.
It is often useful to see this conclusion in geometrical terms: the criterion
of an input        x &#x2192;      {\displaystyle {\vec {x}}}  [{\displaystyle
{\vec {x}}}] being in a class     y   {\displaystyle y}  [y] is purely a
function of projection of multidimensional-space point        x &#x2192;
{\displaystyle {\vec {x}}}  [{\displaystyle {\vec {x}}}] onto vector        w
&#x2192;      {\displaystyle {\vec {w}}}  [{\displaystyle {\vec {w}}}] (thus,
we only consider its direction). In other words, the observation belongs to
y   {\displaystyle y}  [y] if corresponding        x &#x2192;
{\displaystyle {\vec {x}}}  [{\displaystyle {\vec {x}}}] is located on a
certain side of a hyperplane perpendicular to        w &#x2192;
{\displaystyle {\vec {w}}}  [{\displaystyle {\vec {w}}}]. The location of the
plane is defined by the threshold c.
***** Assumptions[edit] *****
The assumptions of discriminant analysis are the same as those for MANOVA. The
analysis is quite sensitive to outliers and the size of the smallest group must
be larger than the number of predictor variables.[7]
    * Multivariate_normality: Independent variables are normal for each level
      of the grouping variable.[9][7]
    * Homogeneity of variance/covariance (homoscedasticity): Variances among
      group variables are the same across levels of predictors. Can be tested
      with Box's_M statistic.[9] It has been suggested, however, that linear
      discriminant analysis be used when covariances are equal, and that
      quadratic_discriminant_analysis may be used when covariances are not
      equal.[7]
    * Multicollinearity: Predictive power can decrease with an increased
      correlation between predictor variables.[7]
    * Independence: Participants are assumed to be randomly sampled, and a
      participant's score on one variable is assumed to be independent of
      scores on that variable for all other participants.[9][7]
It has been suggested that discriminant analysis is relatively robust to slight
violations of these assumptions,[11] and it has also been shown that
discriminant analysis may still be reliable when using dichotomous variables
(where multivariate normality is often violated).[12]
***** Discriminant functions[edit] *****
Discriminant analysis works by creating one or more linear combinations of
predictors, creating a new latent_variable for each function. These functions
are called discriminant functions. The number of functions possible is either
Ng-1 where Ng = number of groups, or p (the number of predictors), whichever is
smaller. The first function created maximizes the differences between groups on
that function. The second function maximizes differences on that function, but
also must not be correlated with the previous function. This continues with
subsequent functions with the requirement that the new function not be
correlated with any of the previous functions.
Given group     j   {\displaystyle j}  [j], with       R   j     {\displaystyle
\mathbb {R} _{j}}  [{\mathbb  {R}}_{j}] sets of sample space, there is a
discriminant rule such that if     x &#x2208;   R   j     {\displaystyle x\in
\mathbb {R} _{j}}  [x\in {\mathbb  {R}}_{j}], then     x &#x2208; j
{\displaystyle x\in j}  [x\in j]. Discriminant analysis then, finds âgoodâ
regions of       R   j     {\displaystyle \mathbb {R} _{j}}  [{\mathbb  {R}}_
{j}] to minimize classification error, therefore leading to a high percent
correct classified in the classification table.[13]
Each function is given a discriminant score[clarification_needed] to determine
how well it predicts group placement.
    * Structure Correlation Coefficients: The correlation between each
      predictor and the discriminant score of each function. This is a zero-
      order correlation (i.e., not corrected for the other predictors). [14]
    * Standardized Coefficients: Each predictor's weight in the linear
      combination that is the discriminant function. Like in a regression
      equation, these coefficients are partial (i.e., corrected for the other
      predictors). Indicates the unique contribution of each predictor in
      predicting group assignment.
    * Functions at Group Centroids: Mean discriminant scores for each grouping
      variable are given for each function. The farther apart the means are,
      the less error there will be in classification.
***** Discrimination rules[edit] *****
    * Maximum_likelihood: Assigns x to the group that maximizes population
      (group) density.[15]
    * Bayes Discriminant Rule: Assigns x to the group that maximizes
      &#x03C0;  i    f  i   ( x )   {\displaystyle \pi _{i}f_{i}(x)}  [\pi _
      {i}f_{i}(x)], where Ïi represents the prior_probability of that
      classification, and      f  i   ( x )   {\displaystyle f_{i}(x)}  [f_{i}
      (x)] represents the population density.[15]
    * Fisher's_linear_discriminant_rule: Maximizes the ratio between SSbetween
      and SSwithin, and finds a linear combination of the predictors to predict
      group.[15]
***** Eigenvalues[edit] *****
An eigenvalue in discriminant analysis is the characteristic root of each
function.[clarification_needed] It is an indication of how well that function
differentiates the groups, where the larger the eigenvalue, the better the
function differentiates.[7] This however, should be interpreted with caution,
as eigenvalues have no upper limit.[9][7] The eigenvalue can be viewed as a
ratio of SSbetween and SSwithin as in ANOVA when the dependent variable is the
discriminant function, and the groups are the levels of the IV[clarification
needed].[9] This means that the largest eigenvalue is associated with the first
function, the second largest with the second, etc..
***** Effect size[edit] *****
Some suggest the use of eigenvalues as effect_size measures, however, this is
generally not supported.[9] Instead, the canonical_correlation is the preferred
measure of effect size. It is similar to the eigenvalue, but is the square root
of the ratio of SSbetween and SStotal. It is the correlation between groups and
the function.[9] Another popular measure of effect size is the percent of
variance[clarification_needed] for each function. This is calculated by: (Î»x/
Î£Î»i) X 100 where Î»x is the eigenvalue for the function and Î£Î»i is the sum
of all eigenvalues. This tells us how strong the prediction is for that
particular function compared to the others.[9] Percent correctly classified can
also be analyzed as an effect size. The kappa value can describe this while
correcting for chance agreement.[9]Kappa normalizes across all categorizes
rather than biased by a significantly good or poorly performing classes.
[clarification_needed][16]
***** Canonical discriminant analysis for k classes[edit] *****
Canonical discriminant analysis (CDA) finds axes (k â 1 canonical
coordinates, k being the number of classes) that best separate the categories.
These linear functions are uncorrelated and define, in effect, an optimal
k â 1 space through the n-dimensional cloud of data that best separates (the
projections in that space of) the k groups. See âMulticlass_LDAâ for
details below.
***** Fisher's linear discriminant[edit] *****
The terms Fisher's linear discriminant and LDA are often used interchangeably,
although Fisher's original article[1] actually describes a slightly different
discriminant, which does not make some of the assumptions of LDA such as
normally_distributed classes or equal class covariances.
Suppose two classes of observations have means         &#x03BC; &#x2192;     0
,     &#x03BC; &#x2192;     1     {\displaystyle {\vec {\mu }}_{0},{\vec {\mu
}}_{1}}  [{\vec {\mu }}_{0},{\vec {\mu }}_{1}] and covariances      &#x03A3;  0
,  &#x03A3;  1     {\displaystyle \Sigma _{0},\Sigma _{1}}  [\Sigma _{0},\Sigma
_{1}]. Then the linear combination of features        w &#x2192;    &#x22C5;
x &#x2192;      {\displaystyle {\vec {w}}\cdot {\vec {x}}}  [{\vec {w}}\cdot
{\vec {x}}] will have means        w &#x2192;    &#x22C5;     &#x03BC; &#x2192;
i     {\displaystyle {\vec {w}}\cdot {\vec {\mu }}_{i}}  [{\vec {w}}\cdot {\vec
{\mu }}_{i}] and variances         w &#x2192;     T    &#x03A3;  i      w
&#x2192;      {\displaystyle {\vec {w}}^{T}\Sigma _{i}{\vec {w}}}  [{\vec {w}}^
{T}\Sigma _{i}{\vec {w}}] for     i = 0 , 1   {\displaystyle i=0,1}  [i=0,1].
Fisher defined the separation between these two distributions to be the ratio
of the variance between the classes to the variance within the classes:
         S =    &#x03C3;  between   2    &#x03C3;  within   2     =    (    w
      &#x2192;    &#x22C5;     &#x03BC; &#x2192;     1   &#x2212;    w &#x2192;
      &#x22C5;     &#x03BC; &#x2192;     0    )  2         w &#x2192;     T
      &#x03A3;  1      w &#x2192;    +     w &#x2192;     T    &#x03A3;  0
      w &#x2192;       =    (    w &#x2192;    &#x22C5; (     &#x03BC; &#x2192;
      1   &#x2212;     &#x03BC; &#x2192;     0   )  )  2         w &#x2192;
      T   (  &#x03A3;  0   +  &#x03A3;  1   )    w &#x2192;
      {\displaystyle S={\frac {\sigma _{\text{between}}^{2}}{\sigma _{\text
      {within}}^{2}}}={\frac {({\vec {w}}\cdot {\vec {\mu }}_{1}-{\vec
      {w}}\cdot {\vec {\mu }}_{0})^{2}}{{\vec {w}}^{T}\Sigma _{1}{\vec {w}}+
      {\vec {w}}^{T}\Sigma _{0}{\vec {w}}}}={\frac {({\vec {w}}\cdot ({\vec
      {\mu }}_{1}-{\vec {\mu }}_{0}))^{2}}{{\vec {w}}^{T}(\Sigma _{0}+\Sigma _
      {1}){\vec {w}}}}}  [S={\frac {\sigma _{\text{between}}^{2}}{\sigma _
      {\text{within}}^{2}}}={\frac {({\vec {w}}\cdot {\vec {\mu }}_{1}-{\vec
      {w}}\cdot {\vec {\mu }}_{0})^{2}}{{\vec {w}}^{T}\Sigma _{1}{\vec {w}}+
      {\vec {w}}^{T}\Sigma _{0}{\vec {w}}}}={\frac {({\vec {w}}\cdot ({\vec
      {\mu }}_{1}-{\vec {\mu }}_{0}))^{2}}{{\vec {w}}^{T}(\Sigma _{0}+\Sigma _
      {1}){\vec {w}}}}]
This measure is, in some sense, a measure of the signal-to-noise_ratio for the
class labelling. It can be shown that the maximum separation occurs when
            w &#x2192;    &#x221D; (  &#x03A3;  0   +  &#x03A3;  1    )
      &#x2212; 1   (     &#x03BC; &#x2192;     1   &#x2212;     &#x03BC;
      &#x2192;     0   )   {\displaystyle {\vec {w}}\propto (\Sigma _{0}+\Sigma
      _{1})^{-1}({\vec {\mu }}_{1}-{\vec {\mu }}_{0})}  [{\vec {w}}\propto
      (\Sigma _{0}+\Sigma _{1})^{-1}({\vec {\mu }}_{1}-{\vec {\mu }}_{0})]
When the assumptions of LDA are satisfied, the above equation is equivalent to
LDA.
Be sure to note that the vector        w &#x2192;      {\displaystyle {\vec
{w}}}  [{\vec {w}}] is the normal to the discriminant hyperplane. As an
example, in a two dimensional problem, the line that best divides the two
groups is perpendicular to        w &#x2192;      {\displaystyle {\vec {w}}}  [
{\vec {w}}].
Generally, the data points to be discriminated are projected onto        w
&#x2192;      {\displaystyle {\vec {w}}}  [{\vec {w}}]; then the threshold that
best separates the data is chosen from analysis of the one-dimensional
distribution. There is no general rule for the threshold. However, if
projections of points from both classes exhibit approximately the same
distributions, a good choice would be the hyperplane between projections of the
two means,        w &#x2192;    &#x22C5;     &#x03BC; &#x2192;     0
{\displaystyle {\vec {w}}\cdot {\vec {\mu }}_{0}}  [{\vec {w}}\cdot {\vec {\mu
}}_{0}] and        w &#x2192;    &#x22C5;     &#x03BC; &#x2192;     1
{\displaystyle {\vec {w}}\cdot {\vec {\mu }}_{1}}  [{\vec {w}}\cdot {\vec {\mu
}}_{1}]. In this case the parameter c in threshold condition        w &#x2192;
&#x22C5;    x &#x2192;    > c   {\displaystyle {\vec {w}}\cdot {\vec {x}}>c}  [
{\vec {w}}\cdot {\vec {x}}>c] can be found explicitly:
         c =    w &#x2192;    &#x22C5;   1 2   (     &#x03BC; &#x2192;     0
      +     &#x03BC; &#x2192;     1   ) =   1 2       &#x03BC; &#x2192;     1
      T    &#x03A3;  1   &#x2212; 1       &#x03BC; &#x2192;     1   &#x2212;
      1 2       &#x03BC; &#x2192;     0   T    &#x03A3;  0   &#x2212; 1
      &#x03BC; &#x2192;     0     {\displaystyle c={\vec {w}}\cdot {\frac {1}
      {2}}({\vec {\mu }}_{0}+{\vec {\mu }}_{1})={\frac {1}{2}}{\vec {\mu }}_
      {1}^{T}\Sigma _{1}^{-1}{\vec {\mu }}_{1}-{\frac {1}{2}}{\vec {\mu }}_{0}^
      {T}\Sigma _{0}^{-1}{\vec {\mu }}_{0}}  [{\displaystyle c={\vec {w}}\cdot
      {\frac {1}{2}}({\vec {\mu }}_{0}+{\vec {\mu }}_{1})={\frac {1}{2}}{\vec
      {\mu }}_{1}^{T}\Sigma _{1}^{-1}{\vec {\mu }}_{1}-{\frac {1}{2}}{\vec {\mu
      }}_{0}^{T}\Sigma _{0}^{-1}{\vec {\mu }}_{0}}].
Otsu's_method is related to Fisher's linear discriminant, and was created to
binarize the histogram of pixels in a grayscale image by optimally picking the
black/white threshold that minimizes intra-class variance and maximizes inter-
class variance within/between grayscales assigned to black and white pixel
classes.
***** Multiclass LDA[edit] *****
In the case where there are more than two classes, the analysis used in the
derivation of the Fisher discriminant can be extended to find a subspace which
appears to contain all of the class variability.[17] This generalization is due
to C._R._Rao.[18] Suppose that each of C classes has a mean      &#x03BC;  i
{\displaystyle \mu _{i}}  [\mu _{i}] and the same covariance     &#x03A3;
{\displaystyle \Sigma }  [\Sigma ]. Then the scatter between class variability
may be defined by the sample covariance of the class means
          &#x03A3;  b   =   1 C    &#x2211;  i = 1   C   (  &#x03BC;  i
      &#x2212; &#x03BC; ) (  &#x03BC;  i   &#x2212; &#x03BC;  )  T
      {\displaystyle \Sigma _{b}={\frac {1}{C}}\sum _{i=1}^{C}(\mu _{i}-\mu )
      (\mu _{i}-\mu )^{T}}  [\Sigma _{b}={\frac {1}{C}}\sum _{i=1}^{C}(\mu _
      {i}-\mu )(\mu _{i}-\mu )^{T}]
where     &#x03BC;   {\displaystyle \mu }  [\mu ] is the mean of the class
means. The class separation in a direction        w &#x2192;
{\displaystyle {\vec {w}}}  [{\vec {w}}] in this case will be given by
         S =        w &#x2192;     T    &#x03A3;  b      w &#x2192;          w
      &#x2192;     T   &#x03A3;    w &#x2192;         {\displaystyle S={\frac {
      {\vec {w}}^{T}\Sigma _{b}{\vec {w}}}{{\vec {w}}^{T}\Sigma {\vec {w}}}}}
      [S={\frac {{\vec {w}}^{T}\Sigma _{b}{\vec {w}}}{{\vec {w}}^{T}\Sigma
      {\vec {w}}}}]
This means that when        w &#x2192;      {\displaystyle {\vec {w}}}  [{\vec
{w}}] is an eigenvector of      &#x03A3;  &#x2212; 1    &#x03A3;  b
{\displaystyle \Sigma ^{-1}\Sigma _{b}}  [\Sigma ^{-1}\Sigma _{b}] the
separation will be equal to the corresponding eigenvalue.
If      &#x03A3;  &#x2212; 1    &#x03A3;  b     {\displaystyle \Sigma ^{-
1}\Sigma _{b}}  [\Sigma ^{-1}\Sigma _{b}] is diagonalizable, the variability
between features will be contained in the subspace spanned by the eigenvectors
corresponding to the C â 1 largest eigenvalues (since      &#x03A3;  b
{\displaystyle \Sigma _{b}}  [\Sigma _{b}] is of rank C â 1 at most). These
eigenvectors are primarily used in feature reduction, as in PCA. The
eigenvectors corresponding to the smaller eigenvalues will tend to be very
sensitive to the exact choice of training data, and it is often necessary to
use regularisation as described in the next section.
If classification is required, instead of dimension_reduction, there are a
number of alternative techniques available. For instance, the classes may be
partitioned, and a standard Fisher discriminant or LDA used to classify each
partition. A common example of this is "one against the rest" where the points
from one class are put in one group, and everything else in the other, and then
LDA applied. This will result in C classifiers, whose results are combined.
Another common method is pairwise classification, where a new classifier is
created for each pair of classes (giving C(C â 1)/2 classifiers in total),
with the individual classifiers combined to produce a final classification.
***** Incremental LDA[edit] *****
The typical implementation of the LDA technique requires that all the samples
are available in advance. However, there are situations where the entire data
set is not available and the input data are observed as a stream. In this case,
it is desirable for the LDA feature extraction to have the ability to update
the computed LDA features by observing the new samples without running the
algorithm on the whole data set. For example, in many real-time applications
such as mobile robotics or on-line face recognition, it is important to update
the extracted LDA features as soon as new observations are available. An LDA
feature extraction technique that can update the LDA features by simply
observing new samples is an incremental LDA algorithm, and this idea has been
extensively studied over the last two decades.[19] Chatterjee and Roychowdhury
proposed an incremental self-organized LDA algorithm for updating the LDA
features.[20] In other work, Demir and Ozmehmet proposed online local learning
algorithms for updating LDA features incrementally using error-correcting and
the Hebbian learning rules.[21] Later, Aliyari et al. derived fast incremental
algorithms to update the LDA features by observing the new samples.[19]
***** Practical use[edit] *****
In practice, the class means and covariances are not known. They can, however,
be estimated from the training set. Either the maximum_likelihood_estimate or
the maximum_a_posteriori estimate may be used in place of the exact value in
the above equations. Although the estimates of the covariance may be considered
optimal in some sense, this does not mean that the resulting discriminant
obtained by substituting these values is optimal in any sense, even if the
assumption of normally distributed classes is correct.
Another complication in applying LDA and Fisher's discriminant to real data
occurs when the number of measurements of each sample (i.e., the dimensionality
of each data vector) exceeds the number of samples in each class.[4] In this
case, the covariance estimates do not have full rank, and so cannot be
inverted. There are a number of ways to deal with this. One is to use a pseudo
inverse instead of the usual matrix inverse in the above formulae. However,
better numeric stability may be achieved by first projecting the problem onto
the subspace spanned by      &#x03A3;  b     {\displaystyle \Sigma _{b}}
[\Sigma _{b}].[22] Another strategy to deal with small sample size is to use a
shrinkage_estimator of the covariance matrix, which can be expressed
mathematically as
         &#x03A3; = ( 1 &#x2212; &#x03BB; ) &#x03A3; + &#x03BB; I
      {\displaystyle \Sigma =(1-\lambda )\Sigma +\lambda I\,}  [\Sigma =(1-
      \lambda )\Sigma +\lambda I\,]
where     I   {\displaystyle I}  [I] is the identity matrix, and     &#x03BB;
{\displaystyle \lambda }  [\lambda ] is the shrinkage intensity or
regularisation parameter. This leads to the framework of regularized
discriminant analysis[23] or shrinkage discriminant analysis.[24]
Also, in many practical cases linear discriminants are not suitable. LDA and
Fisher's discriminant can be extended for use in non-linear classification via
the kernel_trick. Here, the original observations are effectively mapped into a
higher dimensional non-linear space. Linear classification in this non-linear
space is then equivalent to non-linear classification in the original space.
The most commonly used example of this is the kernel_Fisher_discriminant.
LDA can be generalized to multiple_discriminant_analysis, where c becomes a
categorical_variable with N possible states, instead of only two. Analogously,
if the class-conditional densities     p (    x &#x2192;    &#x2223; c = i )
{\displaystyle p({\vec {x}}\mid c=i)}  [{\displaystyle p({\vec {x}}\mid c=i)}]
are normal with shared covariances, the sufficient_statistic for     P ( c
&#x2223;    x &#x2192;    )   {\displaystyle P(c\mid {\vec {x}})}  [
{\displaystyle P(c\mid {\vec {x}})}] are the values of N projections, which are
the subspace spanned by the N means, affine_projected by the inverse covariance
matrix. These projections can be found by solving a generalized_eigenvalue
problem, where the numerator is the covariance matrix formed by treating the
means as the samples, and the denominator is the shared covariance matrix. See
âMulticlass_LDAâ above for details.
***** Applications[edit] *****
In addition to the examples given below, LDA is applied in positioning and
product_management.
**** Bankruptcy prediction[edit] ****
In bankruptcy_prediction based on accounting ratios and other financial
variables, linear discriminant analysis was the first statistical method
applied to systematically explain which firms entered bankruptcy vs. survived.
Despite limitations including known nonconformance of accounting ratios to the
normal distribution assumptions of LDA, Edward_Altman's 1968_model is still a
leading model in practical applications.
**** Face recognition[edit] ****
In computerised face_recognition, each face is represented by a large number of
pixel values. Linear discriminant analysis is primarily used here to reduce the
number of features to a more manageable number before classification. Each of
the new dimensions is a linear combination of pixel values, which form a
template. The linear combinations obtained using Fisher's linear discriminant
are called Fisher faces, while those obtained using the related principal
component_analysis are called eigenfaces.
**** Marketing[edit] ****
In marketing, discriminant analysis was once often used to determine the
factors which distinguish different types of customers and/or products on the
basis of surveys or other forms of collected data. Logistic_regression or other
methods are now more commonly used. The use of discriminant analysis in
marketing can be described by the following steps:
   1. Formulate the problem and gather dataâIdentify the salient attributes
      consumers use to evaluate products in this categoryâUse quantitative
      marketing_research techniques (such as surveys) to collect data from a
      sample of potential customers concerning their ratings of all the product
      attributes. The data collection stage is usually done by marketing
      research professionals. Survey questions ask the respondent to rate a
      product from one to five (or 1 to 7, or 1 to 10) on a range of attributes
      chosen by the researcher. Anywhere from five to twenty attributes are
      chosen. They could include things like: ease of use, weight, accuracy,
      durability, colourfulness, price, or size. The attributes chosen will
      vary depending on the product being studied. The same question is asked
      about all the products in the study. The data for multiple products is
      codified and input into a statistical program such as R, SPSS or SAS.
      (This step is the same as in Factor analysis).
   2. Estimate the Discriminant Function Coefficients and determine the
      statistical significance and validityâChoose the appropriate
      discriminant analysis method. The direct method involves estimating the
      discriminant function so that all the predictors are assessed
      simultaneously. The stepwise method enters the predictors sequentially.
      The two-group method should be used when the dependent variable has two
      categories or states. The multiple discriminant method is used when the
      dependent variable has three or more categorical states. Use Wilks's
      Lambda to test for significance in SPSS or F stat in SAS. The most common
      method used to test validity is to split the sample into an estimation or
      analysis sample, and a validation or holdout sample. The estimation
      sample is used in constructing the discriminant function. The validation
      sample is used to construct a classification matrix which contains the
      number of correctly classified and incorrectly classified cases. The
      percentage of correctly classified cases is called the hit ratio.
   3. Plot the results on a two dimensional map, define the dimensions, and
      interpret the results. The statistical program (or a related module) will
      map the results. The map will plot each product (usually in two-
      dimensional space). The distance of products to each other indicate
      either how different they are. The dimensions must be labelled by the
      researcher. This requires subjective judgement and is often very
      challenging. See perceptual_mapping.
**** Biomedical studies[edit] ****
The main application of discriminant analysis in medicine is the assessment of
severity state of a patient and prognosis of disease outcome. For example,
during retrospective analysis, patients are divided into groups according to
severity of disease â mild, moderate and severe form. Then results of
clinical and laboratory analyses are studied in order to reveal variables which
are statistically different in studied groups. Using these variables,
discriminant functions are built which help to objectively classify disease in
a future patient into mild, moderate or severe form.
In biology, similar principles are used in order to classify and define groups
of different biological objects, for example, to define phage types of
Salmonella enteritidis based on Fourier transform infrared spectra,[25] to
detect animal source of Escherichia coli studying its virulence factors[26]
etc.
**** Earth science[edit] ****
This method can be used to separate the alteration zones. For example, when
different data from various zones are available, discriminant analysis can find
the pattern within the data and classify it effectively.[27]
***** Comparison to logistic regression[edit] *****
Discriminant function analysis is very similar to logistic_regression, and both
can be used to answer the same research questions.[9] Logistic regression does
not have as many assumptions and restrictions as discriminant analysis.
However, when discriminant analysisâ assumptions are met, it is more powerful
than logistic regression.[28] Unlike logistic regression, discriminant analysis
can be used with small sample sizes. It has been shown that when sample sizes
are equal, and homogeneity of variance/covariance holds, discriminant analysis
is more accurate.[7] With all this being considered, logistic regression has
become the common choice, since the assumptions of discriminant analysis are
rarely met.[8][7]
***** Linear discriminant in high dimension[edit] *****
Geometric anomalities in high dimension lead to the well-known curse_of
dimensionality. Nevertheless, proper utilization of concentration_of_measure
phenomena can make computation easier.[29] An important case of these blessing
of dimensionality phenomena was highlighted by Donoho and Tanner: if a sample
is essentially high-dimensional then each point can be separated from the rest
of the sample by linear inequality, with high probability, even for
exponentially large samples.[30] These linear inequalities can be selected in
the standard (Fisher's) form of the linear discriminant for a rich family of
probability distribution.[31] In particular, such theorems are proven for log-
concave distributions including multidimensional_normal_distribution (the proof
is based on the concentration inequalities for long-concave measures[32]) and
for product measures on a multidimensional cube (this is proven using
Talagrand's_concentration_inequality for product probability spaces). Data
separability by classical linear discriminants simplifies the problem of error
correction for artificial_intelligence systems in high dimension.
***** See also[edit] *****
    * Data_mining
    * Decision_tree_learning
    * Factor_analysis
    * Kernel_Fisher_discriminant_analysis
    * Logit (for logistic_regression)
    * Multiple_discriminant_analysis
    * Multidimensional_scaling
    * Pattern_recognition
    * Perceptron
    * Preference_regression
    * Quadratic_classifier
    * Statistical_classification
***** References[edit] *****
   1. ^ a bFisher,_R._A. (1936). "The Use of Multiple Measurements in Taxonomic
      Problems". Annals_of_Eugenics. 7 (2): 179â188. doi:10.1111/j.1469-
      1809.1936.tb02137.x. hdl:2440/15227.
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
   3. ^McLachlan, G. J. (2004). Discriminant Analysis and Statistical Pattern
      Recognition. Wiley Interscience. ISBN 978-0-471-69115-0. MR 1190469.
   4. ^ Analyzing Quantitative Data: An Introduction for Social Researchers,
      Debra Wetcher-Hendricks, p.288
   5. ^ a bMartinez, A. M.; Kak, A. C. (2001). "PCA_versus_LDA" (PDF). IEEE
      Transactions_on_Pattern_Analysis_and_Machine_Intelligence. 23 (=2):
      228â233. doi:10.1109/34.908974.
   6. ^ Abdi, H. (2007) "Discriminant_correspondence_analysis." In: N.J.
      Salkind (Ed.): Encyclopedia of Measurement and Statistic. Thousand Oaks
      (CA): Sage. pp. 270â275.
   7. ^Perriere, G.; Thioulouse, J. (2003). "Use of Correspondence Discriminant
      Analysis to predict the subcellular location of bacterial proteins".
      Computer Methods and Programs in Biomedicine. 70 (2): 99â105. doi:
      10.1016/s0169-2607(02)00011-1. PMID 12507786.
   8. ^ a b c d e f g h i j BÃKEOÄLU ÃOKLUK, Ã, & BÃYÃKÃZTÃRK, Å.
      (2008). Discriminant_function_analysis:_Concept_and_application. EÄitim
      araÅtÄ±rmalarÄ± dergisi, (33), 73-92.
   9. ^ a b Cohen et al. Applied Multiple Regression/Correlation Analysis for
      the Behavioural Sciences 3rd ed. (2003). Taylor & Francis Group.
  10. ^ a b c d e f g h i j k Green, S.B. Salkind, N. J. & Akey, T. M. (2008).
      Using SPSS for Windows and Macintosh: Analyzing and understanding data.
      New Jersey: Prentice Hall.
  11. ^Venables, W. N.; Ripley,_B._D. (2002). Modern Applied Statistics with S
      (4th ed.). Springer Verlag. ISBN 978-0-387-95457-8.
  12. ^ Lachenbruch, P. A. (1975). Discriminant analysis. NY: Hafner
  13. ^ Klecka, William R. (1980). Discriminant analysis. Quantitative
      Applications in the Social Sciences Series, No. 19. Thousand Oaks, CA:
      Sage Publications.
  14. ^ Hardle, W., Simar, L. (2007). Applied Multivariate Statistical
      Analysis. Springer Berlin Heidelberg. pp. 289â303.
  15. ^ Garson, G. D. (2008). Discriminant function analysis. https://
      web.archive.org/web/20080312065328/http://www2.chass.ncsu.edu/garson/
      pA765/discrim.htm.
  16. ^ a b c Hardle, W., Simar, L. (2007). Applied_Multivariate_Statistical
      Analysis. Springer Berlin Heidelberg. pp. 289-303.
  17. ^Israel, Steven A. (June 2006). "Performance Metrics: How and When".
      Geocarto International. 21 (2): 23â32. doi:10.1080/10106040608542380.
      ISSN 1010-6049.
  18. ^ Garson, G. D. (2008). Discriminant function analysis."Archived_copy".
      Archived from the_original on 2008-03-12. Retrieved 2008-03-04.CS1 maint:
      Archived copy as title (link)
  19.  .
  20. ^Rao,_R._C. (1948). "The utilization of multiple measurements in problems
      of biological classification". Journal of the Royal Statistical Society,
      Series B. 10 (2): 159â203. JSTOR 2983775.
  21. ^ a bAliyari Ghassabeh, Youness; Rudzicz, Frank; Moghaddam, Hamid
      Abrishami (2015-06-01). "Fast incremental LDA feature extraction".
      Pattern Recognition. 48 (6): 1999â2012. doi:10.1016/
      j.patcog.2014.12.012.
  22. ^Chatterjee, C.; Roychowdhury, V.P. (1997-05-01). "On self-organizing
      algorithms and networks for class-separability features". IEEE
      Transactions on Neural Networks. 8 (3): 663â678. doi:10.1109/72.572105.
      ISSN 1045-9227. PMID 18255669.
  23. ^Demir, G. K.; Ozmehmet, K. (2005-03-01). "Online Local Learning
      Algorithms for Linear Discriminant Analysis". Pattern Recogn. Lett. 26
      (4): 421â431. doi:10.1016/j.patrec.2004.08.005. ISSN 0167-8655.
  24. ^Yu, H.; Yang, J. (2001). "A direct LDA algorithm for high-dimensional
      data â with application to face recognition". Pattern Recognition. 34
      (10): 2067â2069. CiteSeerX 10.1.1.70.3507. doi:10.1016/s0031-3203
      (00)00162-x.
  25. ^Friedman, J. H. (1989). "Regularized_Discriminant_Analysis" (PDF).
      Journal_of_the_American_Statistical_Association. 84 (405): 165â175.
      CiteSeerX 10.1.1.382.2682. doi:10.2307/2289860. JSTOR 2289860.
      MR 0999675.
  26. ^AhdesmÃ¤ki, M.; Strimmer, K. (2010). "Feature selection in omics
      prediction problems using cat scores and false nondiscovery rate
      control". Annals of Applied Statistics. 4 (1): 503â519. arXiv:
      0903.2003. doi:10.1214/09-aoas277.
  27. ^Preisner, O; Guiomar, R; Machado, J; Menezes, JC; Lopes, JA (2010).
      "Application_of_Fourier_transform_infrared_spectroscopy_and_chemometrics
      for_differentiation_of_Salmonella_enterica_serovar_Enteritidis_phage
      types". Appl Environ Microbiol. 76 (11): 3538â3544. doi:10.1128/
      aem.01589-09. PMC 2876429.
  28. ^David, DE; Lynne, AM; Han, J; Foley, SL (2010). "Evaluation_of_virulence
      factor_profiling_in_the_characterization_of_veterinary_Escherichia_coli
      isolates". Appl Environ Microbiol. 76 (22): 7509â7513. doi:10.1128/
      aem.00726-10. PMC 2976202. PMID 20889790.
  29. ^Tahmasebi, P.; Hezarkhani, A.; Mortazavi, M. (2010). "Application_of
      discriminant_analysis_for_alteration_separation;_sungun_copper_deposit,
      East_Azerbaijan,_Iran._Australian" (PDF). Journal of Basic and Applied
      Sciences. 6 (4): 564â576.
  30. ^Trevor Hastie; Robert Tibshirani; Jerome Friedman. The Elements of
      Statistical Learning. Data Mining, Inference, and Prediction (second
      ed.). Springer. p. 128.
  31. ^ Kainen P.C. (1997) Utilizing_geometric_anomalies_of_high_dimension:
      When_complexity_makes_computation_easier. In: KÃ¡rnÃ½ M., Warwick K.
      (eds) Computer Intensive Methods in Control and Signal Processing: The
      Curse of Dimensionality, Springer, 1997, pp. 282â294.
  32. ^ Donoho, D., Tanner, J. (2009) Observed_universality_of_phase
      transitions_in_high-dimensional_geometry,_with_implications_for_modern
      data_analysis_and_signal_processing, Phil. Trans. R. Soc. A 367,
      4273â4293.
  33. ^ Gorban, A.N., Golubkov, A., Grechuk, B., Mirkes, E.M., Tyukin, I.Y.
      (2018) Correction_of_AI_systems_by_linear_discriminants:_Probabilistic
      foundations, Information Sciences 466, 303-322.
  34. ^ GuÃ©don, O., Milman, E. (2011) Interpolating_thin-shell_and_sharp
      large-deviation_estimates_for_isotropic_log-concave_measures, Geom.
      Funct. Anal. 21 (5), 1043â1068.
***** Further reading[edit] *****
    * Duda, R. O.; Hart, P. E.; Stork, D. H. (2000). Pattern Classification
      (2nd ed.). Wiley Interscience. ISBN 978-0-471-05669-0. MR 1802993.
Hilbe, J. M. (2009). Logistic Regression Models. Chapman & Hall/CRC Press.
ISBN 978-1-4200-7575-5.
Mika, S.; et al. (1999). Fisher Discriminant Analysis with Kernels. IEEE
Conference on Neural Networks for Signal Processing IX. pp. 41â48.
CiteSeerX 10.1.1.35.9904. doi:10.1109/NNSP.1999.788121. ISBN 978-0-7803-5673-3.
McFarland, H. Richard; Donald, St. P. Richards (2001). "Exact Misclassification
Probabilities for Plug-In Normal Quadratic Discriminant Functions. I. The
Equal-Means Case". Journal of Multivariate Analysis. 77 (1): 21â53. doi:
10.1006/jmva.2000.1924.
McFarland, H. Richard; Donald, St. P. Richards (2002). "Exact Misclassification
Probabilities for Plug-In Normal Quadratic Discriminant Functions. II. The
Heterogeneous Case". Journal of Multivariate Analysis. 82 (2): 299â330. doi:
10.1006/jmva.2001.2034.
Haghighat, M.; Abdel-Mottaleb, M.; Alhalabi, W. (2016). "Discriminant
Correlation Analysis: Real-Time Feature Level Fusion for Multimodal Biometric
Recognition". IEEE Transactions on Information Forensics and Security. 11 (9):
1984â1996. doi:10.1109/TIFS.2016.2569061.
***** External links[edit] *****
 Wikiversity has learning resources about Discriminant_function_analysis
    * Discriminant_Correlation_Analysis_(DCA)_of_the_Haghighat_article_(see
      above)
    * ALGLIB contains open-source LDA implementation in C# / C++ / Pascal /
      VBA.
    * Psychometrica.de[permanent_dead_link] open-source LDA implementation in
      Java
    * LDA_tutorial_using_MS_Excel
    * Biomedical_statistics._Discriminant_analysis
    * StatQuest:_Linear_Discriminant_Analysis_(LDA)_clearly_explained on
      YouTube
    * Course_notes,_Discriminant_function_analysis_by_G._David_Garson,_NC_State
      University
    * Discriminant_analysis_tutorial_in_Microsoft_Excel_by_Kardi_Teknomo
    * Course_notes,_Discriminant_function_analysis_by_David_W._Stockburger,
      Missouri_State_University
    * Discriminant_function_analysis_(DA)_by_John_Poulsen_and_Aaron_French,_San
      Francisco_State_University
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
                 * Discriminant analysis
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
index.php?title=Linear_discriminant_analysis&oldid=906535399"
Categories:
    * Classification_algorithms
    * Market_research
    * Market_segmentation
    * Statistical_classification
Hidden categories:
    * CS1_maint:_Archived_copy_as_title
    * Wikipedia_articles_needing_clarification_from_April_2019
    * Wikipedia_articles_needing_clarification_from_April_2012
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_December_2017
    * Articles_with_permanently_dead_external_links
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
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Hrvatski
    * Bahasa_Indonesia
    * Magyar
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Basa_Sunda
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 16 July 2019, at 13:45 (UTC).
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
