The following text has been accessed from https://en.wikipedia.org/wiki/Principal_component_analysis at Fri Aug 9 02:54:46 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Principal component analysis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
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
PCA of a multivariate_Gaussian_distribution centered at (1,3) with a standard
deviation of 3 in roughly the (0.866, 0.5) direction and of 1 in the orthogonal
direction. The vectors shown are the eigenvectors of the covariance_matrix
scaled by the square root of the corresponding eigenvalue, and shifted so their
tails are at the mean.
Principal component analysis (PCA) is a statistical procedure that uses an
orthogonal_transformation to convert a set of observations of possibly
correlated variables (entities each of which takes on various numerical values)
into a set of values of linearly_uncorrelated variables called principal
components. This transformation is defined in such a way that the first
principal component has the largest possible variance (that is, accounts for as
much of the variability in the data as possible), and each succeeding component
in turn has the highest variance possible under the constraint that it is
orthogonal to the preceding components. The resulting vectors (each being a
linear_combination of the variables and containing n observations) are an
uncorrelated orthogonal_basis_set. PCA is sensitive to the relative scaling of
the original variables.
PCA was invented in 1901 by Karl_Pearson,[1] as an analogue of the principal
axis_theorem in mechanics; it was later independently developed and named by
Harold_Hotelling in the 1930s.[2] Depending on the field of application, it is
also named the discrete KarhunenâLoÃ¨ve transform (KLT) in signal_processing,
the Hotelling transform in multivariate quality control, proper orthogonal
decomposition (POD) in mechanical engineering, singular_value_decomposition
(SVD) of X (Golub and Van Loan, 1983), eigenvalue_decomposition (EVD) of XTX in
linear algebra, factor_analysis (for a discussion of the differences between
PCA and factor analysis see Ch. 7 of Jolliffe's Principal Component Analysis),
[3] EckartâYoung_theorem (Harman, 1960), or empirical_orthogonal_functions
(EOF) in meteorological science, empirical_eigenfunction_decomposition
(Sirovich, 1987), empirical_component_analysis (Lorenz, 1956), quasiharmonic
modes (Brooks et al., 1988), spectral_decomposition in noise and vibration, and
empirical_modal_analysis in structural dynamics.
PCA is mostly used as a tool in exploratory_data_analysis and for making
predictive_models. It is often used to visualize genetic distance and
relatedness between populations. PCA can be done by eigenvalue_decomposition of
a data covariance (or correlation) matrix or singular_value_decomposition of a
data_matrix, usually after a normalization step of the initial data. The
normalization of each attribute consists of mean centering â subtracting each
data value from its variable's measured mean so that its empirical mean
(average) is zero â and, possibly, normalizing each variable's variance to
make it equal to 1; see Z-scores.[4] The results of a PCA are usually discussed
in terms of component scores, sometimes called factor scores (the transformed
variable values corresponding to a particular data point), and loadings (the
weight by which each standardized original variable should be multiplied to get
the component score).[5] If component scores are standardized to unit variance,
loadings must contain the data variance in them (and that is the magnitude of
eigenvalues). If component scores are not standardized (therefore they contain
the data variance) then loadings must be unit-scaled, ("normalized") and these
weights are called eigenvectors; they are the cosines of orthogonal rotation of
variables into principal components or back.
PCA is the simplest of the true eigenvector-based multivariate analyses. Often,
its operation can be thought of as revealing the internal structure of the data
in a way that best explains the variance in the data. If a multivariate_dataset
is visualised as a set of coordinates in a high-dimensional data space (1 axis
per variable), PCA can supply the user with a lower-dimensional picture, a
projection of this object when viewed from its most informative viewpoint
[citation_needed]. This is done by using only the first few principal
components so that the dimensionality of the transformed data is reduced.
PCA is closely related to factor_analysis. Factor analysis typically
incorporates more domain specific assumptions about the underlying structure
and solves eigenvectors of a slightly different matrix.
PCA is also related to canonical_correlation_analysis_(CCA). CCA defines
coordinate systems that optimally describe the cross-covariance between two
datasets while PCA defines a new orthogonal_coordinate_system that optimally
describes variance in a single dataset.[6][7]
⁰
***** Contents *****
    * 1_Intuition
    * 2_Details
          o 2.1_First_component
          o 2.2_Further_components
          o 2.3_Covariances
          o 2.4_Dimensionality_reduction
          o 2.5_Singular_value_decomposition
    * 3_Further_considerations
    * 4_Table_of_symbols_and_abbreviations
    * 5_Properties_and_limitations_of_PCA
          o 5.1_Properties
          o 5.2_Limitations
          o 5.3_PCA_and_information_theory
    * 6_Computing_PCA_using_the_covariance_method
          o 6.1_Organize_the_data_set
          o 6.2_Calculate_the_empirical_mean
          o 6.3_Calculate_the_deviations_from_the_mean
          o 6.4_Find_the_covariance_matrix
          o 6.5_Find_the_eigenvectors_and_eigenvalues_of_the_covariance_matrix
          o 6.6_Rearrange_the_eigenvectors_and_eigenvalues
          o 6.7_Compute_the_cumulative_energy_content_for_each_eigenvector
          o 6.8_Select_a_subset_of_the_eigenvectors_as_basis_vectors
          o 6.9_Project_the_z-scores_of_the_data_onto_the_new_basis
    * 7_Derivation_of_PCA_using_the_covariance_method
    * 8_Covariance-free_computation
          o 8.1_Iterative_computation
          o 8.2_The_NIPALS_method
          o 8.3_Online/sequential_estimation
    * 9_PCA_and_qualitative_variables
    * 10_Applications
          o 10.1_Quantitative_finance
          o 10.2_Neuroscience
    * 11_Relation_with_other_methods
          o 11.1_Correspondence_analysis
          o 11.2_Factor_analysis
          o 11.3_K-means_clustering
          o 11.4_Non-negative_matrix_factorization
    * 12_Generalizations
          o 12.1_Sparse_PCA
          o 12.2_Nonlinear_PCA
          o 12.3_Robust_PCA
    * 13_Similar_techniques
          o 13.1_Independent_component_analysis
          o 13.2_Network_component_analysis
    * 14_Software/source_code
    * 15_See_also
    * 16_References
    * 17_Further_reading
    * 18_External_links
***** Intuition[edit] *****
PCA can be thought of as fitting a p-dimensional ellipsoid to the data, where
each axis of the ellipsoid represents a principal component. If some axis of
the ellipsoid is small, then the variance along that axis is also small, and by
omitting that axis and its corresponding principal component from our
representation of the dataset, we lose only a commensurately small amount of
information.
To find the axes of the ellipsoid, we must first subtract the mean of each
variable from the dataset to center the data around the origin. Then, we
compute the covariance_matrix of the data and calculate the eigenvalues and
corresponding eigenvectors of this covariance matrix. Then we must normalize
each of the orthogonal eigenvectors to become unit vectors. Once this is done,
each of the mutually orthogonal, unit eigenvectors can be interpreted as an
axis of the ellipsoid fitted to the data. This choice of basis will transform
our covariance matrix into a diagonalised form with the diagonal elements
representing the variance of each axis. The proportion of the variance that
each eigenvector represents can be calculated by dividing the eigenvalue
corresponding to that eigenvector by the sum of all eigenvalues.
This procedure is sensitive to the scaling of the data, and there is no
consensus as to how to best scale the data to obtain optimal results.
***** Details[edit] *****
PCA is mathematically defined as an orthogonal linear_transformation that
transforms the data to a new coordinate_system such that the greatest variance
by some projection of the data comes to lie on the first coordinate (called the
first principal component), the second greatest variance on the second
coordinate, and so on.[3]
Consider a data matrix, X, with column-wise zero empirical_mean (the sample
mean of each column has been shifted to zero), where each of the n rows
represents a different repetition of the experiment, and each of the p columns
gives a particular kind of feature (say, the results from a particular sensor).
Mathematically, the transformation is defined by a set of p-dimensional vectors
of weights or coefficients       w   ( k )   = (  w  1   , &#x2026; ,  w  p
)  ( k )     {\displaystyle \mathbf {w} _{(k)}=(w_{1},\dots ,w_{p})_{(k)}}
[\mathbf {w} _{(k)}=(w_{1},\dots ,w_{p})_{(k)}] that map each row vector
x   ( i )     {\displaystyle \mathbf {x} _{(i)}}  [\mathbf{x}_{(i)}] of X to a
new vector of principal component scores       t   ( i )   = (  t  1   ,
&#x2026; ,  t  l    )  ( i )     {\displaystyle \mathbf {t} _{(i)}=(t_{1},\dots
,t_{l})_{(i)}}  [{\displaystyle \mathbf {t} _{(i)}=(t_{1},\dots ,t_{l})_{
(i)}}], given by
            t  k     ( i )   =   x   ( i )   &#x22C5;   w   ( k )     f o r   i
      = 1 , &#x2026; , n  k = 1 , &#x2026; , l   {\displaystyle {t_{k}}_{
      (i)}=\mathbf {x} _{(i)}\cdot \mathbf {w} _{(k)}\qquad \mathrm {for}
      \qquad i=1,\dots ,n\qquad k=1,\dots ,l}  [{\displaystyle {t_{k}}_{
      (i)}=\mathbf {x} _{(i)}\cdot \mathbf {w} _{(k)}\qquad \mathrm {for}
      \qquad i=1,\dots ,n\qquad k=1,\dots ,l}]
in such a way that the individual variables      t  1   , &#x2026; ,  t  l
{\displaystyle t_{1},\dots ,t_{l}}  [{\displaystyle t_{1},\dots ,t_{l}}] of t
considered over the data set successively inherit the maximum possible variance
from X, with each coefficient vector w constrained to be a unit_vector (where
l   {\displaystyle l}  [l] is usually selected to be less than     p
{\displaystyle p}  [p] to reduce dimensionality).
**** First component[edit] ****
In order to maximize variance, the first weight vector w(1) thus has to satisfy
           w   ( 1 )   =    arg  m a x   &#x2016;  w  &#x2016; = 1
      {   &#x2211;  i     (  t  1   )   ( i )   2    }  =    arg  m a x
      &#x2016;  w  &#x2016; = 1      {   &#x2211;  i     (    x   ( i )
      &#x22C5;  w   )   2    }    {\displaystyle \mathbf {w} _{(1)}={\underset
      {\Vert \mathbf {w} \Vert =1}{\operatorname {\arg \,max} }}\,\left\{\sum _
      {i}\left(t_{1}\right)_{(i)}^{2}\right\}={\underset {\Vert \mathbf {w}
      \Vert =1}{\operatorname {\arg \,max} }}\,\left\{\sum _{i}\left(\mathbf
      {x} _{(i)}\cdot \mathbf {w} \right)^{2}\right\}}  [{\mathbf  {w}}_{{
      (1)}}={\underset  {\Vert {\mathbf  {w}}\Vert =1}{\operatorname {\arg
      \,max}}}\,\left\{\sum _{i}\left(t_{1}\right)_{{(i)}}^{2}\right\}=
      {\underset  {\Vert {\mathbf  {w}}\Vert =1}{\operatorname {\arg
      \,max}}}\,\left\{\sum _{i}\left({\mathbf  {x}}_{{(i)}}\cdot {\mathbf
      {w}}\right)^{2}\right\}]
Equivalently, writing this in matrix form gives
           w   ( 1 )   =    arg  m a x   &#x2016;  w  &#x2016; = 1
      { &#x2016;  X w   &#x2016;  2   } =    arg  m a x   &#x2016;  w  &#x2016;
      = 1      {    w   T     X  T     X w   }    {\displaystyle \mathbf {w} _{
      (1)}={\underset {\Vert \mathbf {w} \Vert =1}{\operatorname {\arg \,max}
      }}\,\{\Vert \mathbf {Xw} \Vert ^{2}\}={\underset {\Vert \mathbf {w} \Vert
      =1}{\operatorname {\arg \,max} }}\,\left\{\mathbf {w} ^{T}\mathbf {X^{T}}
      \mathbf {Xw} \right\}}  [{\displaystyle \mathbf {w} _{(1)}={\underset
      {\Vert \mathbf {w} \Vert =1}{\operatorname {\arg \,max} }}\,\{\Vert
      \mathbf {Xw} \Vert ^{2}\}={\underset {\Vert \mathbf {w} \Vert =1}
      {\operatorname {\arg \,max} }}\,\left\{\mathbf {w} ^{T}\mathbf {X^{T}}
      \mathbf {Xw} \right\}}]
Since w(1) has been defined to be a unit vector, it equivalently also satisfies
           w   ( 1 )   =   arg  m a x     {      w   T     X  T     X w      w
      T    w     }    {\displaystyle \mathbf {w} _{(1)}={\operatorname {\arg
      \,max} }\,\left\{{\frac {\mathbf {w} ^{T}\mathbf {X^{T}} \mathbf {Xw} }
      {\mathbf {w} ^{T}\mathbf {w} }}\right\}}  [{\displaystyle \mathbf {w} _{
      (1)}={\operatorname {\arg \,max} }\,\left\{{\frac {\mathbf {w} ^
      {T}\mathbf {X^{T}} \mathbf {Xw} }{\mathbf {w} ^{T}\mathbf {w}
      }}\right\}}]
The quantity to be maximised can be recognised as a Rayleigh_quotient. A
standard result for a positive_semidefinite_matrix such as XTX is that the
quotient's maximum possible value is the largest eigenvalue of the matrix,
which occurs when w is the corresponding eigenvector.
With w(1) found, the first principal component of a data vector x(i) can then
be given as a score t1(i) = x(i) â w(1) in the transformed co-ordinates, or
as the corresponding vector in the original variables, {x(i) â w(1)} w(1).
**** Further components[edit] ****
The kth component can be found by subtracting the first k â 1 principal
components from X:
             X &#x005E;     k   =  X  &#x2212;  &#x2211;  s = 1   k &#x2212; 1
      X    w   ( s )     w   ( s )    T      {\displaystyle \mathbf {\hat {X}}
      _{k}=\mathbf {X} -\sum _{s=1}^{k-1}\mathbf {X} \mathbf {w} _{(s)}\mathbf
      {w} _{(s)}^{\rm {T}}}  [{\mathbf  {{\hat  {X}}}}_{{k}}={\mathbf  {X}}-
      \sum _{{s=1}}^{{k-1}}{\mathbf  {X}}{\mathbf  {w}}_{{(s)}}{\mathbf  {w}}_{
      {(s)}}^{{{\rm {T}}}}]
and then finding the weight vector which extracts the maximum variance from
this new data matrix
           w   ( k )   =    a r g  m a x   &#x2016;  w  &#x2016; = 1
      {  &#x2016;     X &#x005E;     k    w   &#x2016;  2    }  =   arg  m a x
      {       w   T       X &#x005E;     k   T       X &#x005E;     k    w
      w   T    w      }    {\displaystyle \mathbf {w} _{(k)}={\underset {\Vert
      \mathbf {w} \Vert =1}{\operatorname {arg\,max} }}\left\{\Vert \mathbf
      {\hat {X}} _{k}\mathbf {w} \Vert ^{2}\right\}={\operatorname {\arg \,max}
      }\,\left\{{\tfrac {\mathbf {w} ^{T}\mathbf {\hat {X}} _{k}^{T}\mathbf
      {\hat {X}} _{k}\mathbf {w} }{\mathbf {w} ^{T}\mathbf {w} }}\right\}}  [
      {\mathbf  {w}}_{{(k)}}={\underset  {\Vert {\mathbf  {w}}\Vert =1}
      {\operatorname {arg\,max}}}\left\{\Vert {\mathbf  {{\hat  {X}}}}_{{k}}
      {\mathbf  {w}}\Vert ^{2}\right\}={\operatorname {\arg \,max}}\,\left\{
      {\tfrac  {{\mathbf  {w}}^{T}{\mathbf  {{\hat  {X}}}}_{{k}}^{T}{\mathbf  {
      {\hat  {X}}}}_{{k}}{\mathbf  {w}}}{{\mathbf  {w}}^{T}{\mathbf
      {w}}}}\right\}]
It turns out that this gives the remaining eigenvectors of XTX, with the
maximum values for the quantity in brackets given by their corresponding
eigenvalues. Thus the weight vectors are eigenvectors of XTX.
The kth principal component of a data vector x(i) can therefore be given as a
score tk(i) = x(i) â w(k) in the transformed co-ordinates, or as the
corresponding vector in the space of the original variables, {x(i) â w(k)} w
(k), where w(k) is the kth eigenvector of XTX.
The full principal components decomposition of X can therefore be given as
          T  =  X   W    {\displaystyle \mathbf {T} =\mathbf {X} \mathbf {W} }
      [\mathbf{T} = \mathbf{X} \mathbf{W}]
where W is a p-by-p matrix of weights whose columns are the eigenvectors of
XTX. The transpose of W is sometimes called the whitening_or_sphering
transformation. Columns of W multiplied by the square root of corresponding
eigenvalues, i.e. eigenvectors scaled up by the variances, are called loadings
in PCA or in Factor analysis.
**** Covariances[edit] ****
XTX itself can be recognised as proportional to the empirical sample covariance
matrix of the dataset X.
The sample covariance Q between two of the different principal components over
the dataset is given by:
             Q (   P C   ( j )   ,   P C   ( k )   )    &#x221D; (  X    w
      ( j )    )  T   (  X    w   ( k )   )       =   w   ( j )   T     X   T
      X    w   ( k )         =   w   ( j )   T    &#x03BB;  ( k )     w   ( k )
      =  &#x03BB;  ( k )     w   ( j )   T     w   ( k )         {\displaystyle
      {\begin{aligned}Q(\mathrm {PC} _{(j)},\mathrm {PC} _{(k)})&\propto
      (\mathbf {X} \mathbf {w} _{(j)})^{T}(\mathbf {X} \mathbf {w} _{
      (k)})\\&=\mathbf {w} _{(j)}^{T}\mathbf {X} ^{T}\mathbf {X} \mathbf {w} _{
      (k)}\\&=\mathbf {w} _{(j)}^{T}\lambda _{(k)}\mathbf {w} _{(k)}\\&=\lambda
      _{(k)}\mathbf {w} _{(j)}^{T}\mathbf {w} _{(k)}\end{aligned}}}  [
      {\displaystyle {\begin{aligned}Q(\mathrm {PC} _{(j)},\mathrm {PC} _{
      (k)})&\propto (\mathbf {X} \mathbf {w} _{(j)})^{T}(\mathbf {X} \mathbf
      {w} _{(k)})\\&=\mathbf {w} _{(j)}^{T}\mathbf {X} ^{T}\mathbf {X} \mathbf
      {w} _{(k)}\\&=\mathbf {w} _{(j)}^{T}\lambda _{(k)}\mathbf {w} _{
      (k)}\\&=\lambda _{(k)}\mathbf {w} _{(j)}^{T}\mathbf {w} _{(k)}\end
      {aligned}}}]
where the eigenvalue property of w(k) has been used to move from line 2 to line
3. However eigenvectors w(j) and w(k) corresponding to eigenvalues of a
symmetric matrix are orthogonal (if the eigenvalues are different), or can be
orthogonalised (if the vectors happen to share an equal repeated value). The
product in the final line is therefore zero; there is no sample covariance
between different principal components over the dataset.
Another way to characterise the principal components transformation is
therefore as the transformation to coordinates which diagonalise the empirical
sample covariance matrix.
In matrix form, the empirical covariance matrix for the original variables can
be written
          Q  &#x221D;   X   T    X  =  W   &#x039B;    W   T     {\displaystyle
      \mathbf {Q} \propto \mathbf {X} ^{T}\mathbf {X} =\mathbf {W} \mathbf
      {\Lambda } \mathbf {W} ^{T}}  [\mathbf{Q} \propto \mathbf{X}^T \mathbf{X}
      = \mathbf{W} \mathbf{\Lambda} \mathbf{W}^T]
The empirical covariance matrix between the principal components becomes
           W   T    Q   W  &#x221D;   W   T    W    &#x039B;     W   T    W  =
      &#x039B;    {\displaystyle \mathbf {W} ^{T}\mathbf {Q} \mathbf {W}
      \propto \mathbf {W} ^{T}\mathbf {W} \,\mathbf {\Lambda } \,\mathbf {W} ^
      {T}\mathbf {W} =\mathbf {\Lambda } }  [\mathbf{W}^T \mathbf{Q} \mathbf{W}
      \propto \mathbf{W}^T \mathbf{W} \, \mathbf{\Lambda} \, \mathbf{W}^T
      \mathbf{W}
      =  \mathbf{\Lambda} ]
where Î is the diagonal matrix of eigenvalues Î»(k) of XTX. Î»(k) is equal to
the sum of the squares over the dataset associated with each component k, i.e.
Î»(k) = Î£i tk2(i) = Î£i (x(i) â w(k))2.
**** Dimensionality reduction[edit] ****
The transformation T = X W maps a data vector x(i) from an original space of p
variables to a new space of p variables which are uncorrelated over the
dataset. However, not all the principal components need to be kept. Keeping
only the first L principal components, produced by using only the first L
eigenvectors, gives the truncated transformation
           T   L   =  X    W   L     {\displaystyle \mathbf {T} _{L}=\mathbf
      {X} \mathbf {W} _{L}}  [\mathbf{T}_L = \mathbf{X} \mathbf{W}_L]
where the matrix TL now has n rows but only L columns. In other words, PCA
learns a linear transformation     t =  W  T   x , x &#x2208;  R  p   , t
&#x2208;  R  L   ,   {\displaystyle t=W^{T}x,x\in R^{p},t\in R^{L},}  [t=W^
{T}x,x\in R^{p},t\in R^{L},] where the columns of p Ã L matrix W form an
orthogonal basis for the L features (the components of representation t) that
are decorrelated.[8] By construction, of all the transformed data matrices with
only L columns, this score matrix maximises the variance in the original data
that has been preserved, while minimising the total squared reconstruction
error     &#x2016;  T    W   T   &#x2212;   T   L     W   L   T    &#x2016;  2
2     {\displaystyle \|\mathbf {T} \mathbf {W} ^{T}-\mathbf {T} _{L}\mathbf {W}
_{L}^{T}\|_{2}^{2}}  [\|\mathbf {T} \mathbf {W} ^{T}-\mathbf {T} _{L}\mathbf
{W} _{L}^{T}\|_{2}^{2}] or     &#x2016;  X  &#x2212;   X   L    &#x2016;  2   2
{\displaystyle \|\mathbf {X} -\mathbf {X} _{L}\|_{2}^{2}}  [\|\mathbf {X} -
\mathbf {X} _{L}\|_{2}^{2}].
A principal components analysis scatterplot of Y-STR haplotypes calculated from
repeat-count values for 37 Y-chromosomal STR markers from 354 individuals.
PCA has successfully found linear combinations of the different markers, that
separate out different clusters corresponding to different lines of
individuals' Y-chromosomal genetic descent.
Such dimensionality_reduction can be a very useful step for visualising and
processing high-dimensional datasets, while still retaining as much of the
variance in the dataset as possible. For example, selecting L = 2 and keeping
only the first two principal components finds the two-dimensional plane through
the high-dimensional dataset in which the data is most spread out, so if the
data contains clusters these too may be most spread out, and therefore most
visible to be plotted out in a two-dimensional diagram; whereas if two
directions through the data (or two of the original variables) are chosen at
random, the clusters may be much less spread apart from each other, and may in
fact be much more likely to substantially overlay each other, making them
indistinguishable.
Similarly, in regression_analysis, the larger the number of explanatory
variables allowed, the greater is the chance of overfitting the model,
producing conclusions that fail to generalise to other datasets. One approach,
especially when there are strong correlations between different possible
explanatory variables, is to reduce them to a few principal components and then
run the regression against them, a method called principal_component
regression.
Dimensionality reduction may also be appropriate when the variables in a
dataset are noisy. If each column of the dataset contains independent
identically distributed Gaussian noise, then the columns of T will also contain
similarly identically distributed Gaussian noise (such a distribution is
invariant under the effects of the matrix W, which can be thought of as a high-
dimensional rotation of the co-ordinate axes). However, with more of the total
variance concentrated in the first few principal components compared to the
same noise variance, the proportionate effect of the noise is lessâthe first
few components achieve a higher signal-to-noise_ratio. PCA thus can have the
effect of concentrating much of the signal into the first few principal
components, which can usefully be captured by dimensionality reduction; while
the later principal components may be dominated by noise, and so disposed of
without great loss.
**** Singular value decomposition[edit] ****
The principal components transformation can also be associated with another
matrix factorization, the singular_value_decomposition (SVD) of X,
          X  =  U   &#x03A3;    W   T     {\displaystyle \mathbf {X} =\mathbf
      {U} \mathbf {\Sigma } \mathbf {W} ^{T}}  [\mathbf{X} = \mathbf{U}\mathbf
      {\Sigma}\mathbf{W}^T]
Here Î£ is an n-by-p rectangular_diagonal_matrix of positive numbers Ï(k),
called the singular values of X; U is an n-by-n matrix, the columns of which
are orthogonal unit vectors of length n called the left singular vectors of X;
and W is a p-by-p whose columns are orthogonal unit vectors of length p and
called the right singular vectors of X.
In terms of this factorization, the matrix XTX can be written
               X   T    X     =  W    &#x03A3;   T     U   T    U   &#x03A3;
      W   T         =  W    &#x03A3;   T    &#x03A3;    W   T         =  W
      &#x03A3; &#x005E;     2     W   T         {\displaystyle {\begin
      {aligned}\mathbf {X} ^{T}\mathbf {X} &=\mathbf {W} \mathbf {\Sigma } ^
      {T}\mathbf {U} ^{T}\mathbf {U} \mathbf {\Sigma } \mathbf {W} ^
      {T}\\&=\mathbf {W} \mathbf {\Sigma } ^{T}\mathbf {\Sigma } \mathbf {W} ^
      {T}\\&=\mathbf {W} \mathbf {\hat {\Sigma }} ^{2}\mathbf {W} ^{T}\end
      {aligned}}}  [{\displaystyle {\begin{aligned}\mathbf {X} ^{T}\mathbf {X}
      &=\mathbf {W} \mathbf {\Sigma } ^{T}\mathbf {U} ^{T}\mathbf {U} \mathbf
      {\Sigma } \mathbf {W} ^{T}\\&=\mathbf {W} \mathbf {\Sigma } ^{T}\mathbf
      {\Sigma } \mathbf {W} ^{T}\\&=\mathbf {W} \mathbf {\hat {\Sigma }} ^
      {2}\mathbf {W} ^{T}\end{aligned}}}]
where        &#x03A3; &#x005E;      {\displaystyle \mathbf {\hat {\Sigma }} }
[{\displaystyle \mathbf {\hat {\Sigma }} }] is the square diagonal matrix with
the singular values of X and the excess zeros chopped off that satisfies
&#x03A3; &#x005E;     2    =   &#x03A3;   T    &#x03A3;    {\displaystyle
\mathbf {{\hat {\Sigma }}^{2}} =\mathbf {\Sigma } ^{T}\mathbf {\Sigma } }  [
{\displaystyle \mathbf {{\hat {\Sigma }}^{2}} =\mathbf {\Sigma } ^{T}\mathbf
{\Sigma } }]. Comparison with the eigenvector factorization of XTX establishes
that the right singular vectors W of X are equivalent to the eigenvectors of
XTX, while the singular values Ï(k) of      X    {\displaystyle \mathbf {X} }
[{\displaystyle \mathbf {X} }] are equal to the square-root of the eigenvalues
Î»(k) of XTX.
Using the singular value decomposition the score matrix T can be written
              T     =  X   W        =  U   &#x03A3;    W   T    W        =  U
      &#x03A3;        {\displaystyle {\begin{aligned}\mathbf {T} &=\mathbf {X}
      \mathbf {W} \\&=\mathbf {U} \mathbf {\Sigma } \mathbf {W} ^{T}\mathbf {W}
      \\&=\mathbf {U} \mathbf {\Sigma } \end{aligned}}}  [\begin{align}
      \mathbf{T} & = \mathbf{X} \mathbf{W} \\
                 & = \mathbf{U}\mathbf{\Sigma}\mathbf{W}^T \mathbf{W} \\
                 & = \mathbf{U}\mathbf{\Sigma}
      \end{align}]
so each column of T is given by one of the left singular vectors of X
multiplied by the corresponding singular value. This form is also the polar
decomposition of T.
Efficient algorithms exist to calculate the SVD of X without having to form the
matrix XTX, so computing the SVD is now the standard way to calculate a
principal components analysis from a data matrix[citation_needed], unless only
a handful of components are required.
As with the eigen-decomposition, a truncated n Ã L score matrix TL can be
obtained by considering only the first L largest singular values and their
singular vectors:
           T   L   =   U   L     &#x03A3;   L   =  X    W   L
      {\displaystyle \mathbf {T} _{L}=\mathbf {U} _{L}\mathbf {\Sigma } _
      {L}=\mathbf {X} \mathbf {W} _{L}}  [\mathbf{T}_L = \mathbf{U}_L\mathbf
      {\Sigma}_L = \mathbf{X} \mathbf{W}_L ]
The truncation of a matrix M or T using a truncated singular value
decomposition in this way produces a truncated matrix that is the nearest
possible matrix of rank L to the original matrix, in the sense of the
difference between the two having the smallest possible Frobenius_norm, a
result known as the EckartâYoung theorem [1936].
***** Further considerations[edit] *****
Given a set of points in Euclidean_space, the first principal component
corresponds to a line that passes through the multidimensional mean and
minimizes the sum of squares of the distances of the points from the line. The
second principal component corresponds to the same concept after all
correlation with the first principal component has been subtracted from the
points. The singular values (in Î£) are the square roots of the eigenvalues of
the matrix XTX. Each eigenvalue is proportional to the portion of the
"variance" (more correctly of the sum of the squared distances of the points
from their multidimensional mean) that is associated with each eigenvector. The
sum of all the eigenvalues is equal to the sum of the squared distances of the
points from their multidimensional mean. PCA essentially rotates the set of
points around their mean in order to align with the principal components. This
moves as much of the variance as possible (using an orthogonal transformation)
into the first few dimensions. The values in the remaining dimensions,
therefore, tend to be small and may be dropped with minimal loss of information
(see below). PCA is often used in this manner for dimensionality_reduction. PCA
has the distinction of being the optimal orthogonal transformation for keeping
the subspace that has largest "variance" (as defined above). This advantage,
however, comes at the price of greater computational requirements if compared,
for example, and when applicable, to the discrete_cosine_transform, and in
particular to the DCT-II which is simply known as the "DCT". Nonlinear
dimensionality_reduction techniques tend to be more computationally demanding
than PCA.
PCA is sensitive to the scaling of the variables. If we have just two variables
and they have the same sample_variance and are positively correlated, then the
PCA will entail a rotation by 45Â° and the "weights" (they are the cosines of
rotation) for the two variables with respect to the principal component will be
equal. But if we multiply all values of the first variable by 100, then the
first principal component will be almost the same as that variable, with a
small contribution from the other variable, whereas the second component will
be almost aligned with the second original variable. This means that whenever
the different variables have different units (like temperature and mass), PCA
is a somewhat arbitrary method of analysis. (Different results would be
obtained if one used Fahrenheit rather than Celsius for example.) Pearson's
original paper was entitled "On Lines and Planes of Closest Fit to Systems of
Points in Space" â "in space" implies physical Euclidean space where such
concerns do not arise. One way of making the PCA less arbitrary is to use
variables scaled so as to have unit variance, by standardizing the data and
hence use the autocorrelation matrix instead of the autocovariance matrix as a
basis for PCA. However, this compresses (or expands) the fluctuations in all
dimensions of the signal space to unit variance.
Mean subtraction (a.k.a. "mean centering") is necessary for performing
classical PCA to ensure that the first principal component describes the
direction of maximum variance. If mean subtraction is not performed, the first
principal component might instead correspond more or less to the mean of the
data. A mean of zero is needed for finding a basis that minimizes the mean
square_error of the approximation of the data.[9]
Mean-centering is unnecessary if performing a principal components analysis on
a correlation matrix, as the data are already centered after calculating
correlations. Correlations are derived from the cross-product of two standard
scores (Z-scores) or statistical moments (hence the name: Pearson Product-
Moment Correlation). Also see the article by Kromrey & Foster-Johnson (1998) on
"Mean-centering in Moderated Regression: Much Ado About Nothing".
An autoencoder neural_network with a linear hidden layer is similar to PCA.
Upon convergence, the weight vectors of the K neurons in the hidden layer will
form a basis for the space spanned by the first K principal components. Unlike
PCA, this technique will not necessarily produce orthogonal vectors, yet the
principal components can easily be recovered from them using singular value
decomposition.[10]
PCA is a popular primary technique in pattern_recognition. It is not, however,
optimized for class separability.[11] However, it has been used to quantify the
distance between two or more classes by calculating center of mass for each
class in principal component space and reporting Euclidean distance between
center of mass of two or more classes.[12] The linear_discriminant_analysis is
an alternative which is optimized for class separability.
***** Table of symbols and abbreviations[edit] *****
Symbol              Meaning             Dimensions         Indices
    X  = {  X  i j                                            i = 1 &#x2026; n
}   {\displaystyle  data matrix,                           {\displaystyle
\mathbf {X} =\{X_   consisting of the      n &#x00D7; p    i=1\ldots n}  [ i =
{ij}\}}  [          set of all data     {\displaystyle     1 \ldots n ]
{\displaystyle      vectors, one vector n\times p}  [ n        j = 1 &#x2026; p
\mathbf {X} =\{X_   per row             \times p]          {\displaystyle
{ij}\}}]                                                   j=1\ldots p}  [ j =
                                                           1 \ldots p ]
   n                the number of row      1 &#x00D7; 1
{\displaystyle n\,} vectors in the data {\displaystyle     scalar
[n \,]              set                 1\times 1}  [1
                                        \times 1]
   p                the number of          1 &#x00D7; 1
{\displaystyle p\,} elements in each    {\displaystyle     scalar
[p\,]               row vector          1\times 1}  [1
                    (dimension)         \times 1]
                    the number of
                    dimensions in the
                    dimensionally          1 &#x00D7; 1
   L                reduced subspace,   {\displaystyle
{\displaystyle L\,} 1 &#x2264; L        1\times 1}  [1     scalar
[L \,]              &#x2264; p          \times 1]
                    {\displaystyle
                    1\leq L\leq p}  [ 1
                    \le L \le p ]
    u  = {  u  j
}   {\displaystyle  vector of empirical    p &#x00D7; 1       j = 1 &#x2026; p
\mathbf {u} =\{u_   means, one mean for {\displaystyle     {\displaystyle
{j}\}}  [           each column j of    p\times 1}  [ p    j=1\ldots p}  [ j =
{\displaystyle      the data matrix     \times 1]          1 \ldots p ]
\mathbf {u} =\{u_
{j}\}}]
    s  = {  s  j    vector of empirical
}   {\displaystyle  standard               p &#x00D7; 1       j = 1 &#x2026; p
\mathbf {s} =\{s_   deviations, one     {\displaystyle     {\displaystyle
{j}\}}  [           standard deviation  p\times 1}  [ p    j=1\ldots p}  [ j =
{\displaystyle      for each column j   \times 1]          1 \ldots p ]
\mathbf {s} =\{s_   of the data matrix
{j}\}}]
    h  = {  h  i
}   {\displaystyle                         1 &#x00D7; n       i = 1 &#x2026; n
\mathbf {h} =\{h_                       {\displaystyle     {\displaystyle
{i}\}}  [           vector of all 1's   1\times n}  [ 1    i=1\ldots n}  [ i =
{\displaystyle                          \times n]          1 \ldots n ]
\mathbf {h} =\{h_
{i}\}}]
    B  = {  B  i j                                            i = 1 &#x2026; n
}   {\displaystyle                                         {\displaystyle
\mathbf {B} =\{B_   deviations from the    n &#x00D7; p    i=1\ldots n}  [ i =
{ij}\}}  [          mean of each column {\displaystyle     1 \ldots n ]
{\displaystyle      j of the data       n\times p}  [ n        j = 1 &#x2026; p
\mathbf {B} =\{B_   matrix              \times p]          {\displaystyle
{ij}\}}]                                                   j=1\ldots p}  [ j =
                                                           1 \ldots p ]
    Z  = {  Z  i j                                            i = 1 &#x2026; n
}   {\displaystyle  z-scores, computed                     {\displaystyle
\mathbf {Z} =\{Z_   using the mean and     n &#x00D7; p    i=1\ldots n}  [ i =
{ij}\}}  [          standard deviation  {\displaystyle     1 \ldots n ]
{\displaystyle      for each row m of   n\times p}  [ n        j = 1 &#x2026; p
\mathbf {Z} =\{Z_   the data matrix     \times p]          {\displaystyle
{ij}\}}]                                                   j=1\ldots p}  [ j =
                                                           1 \ldots p ]
                                                              j = 1 &#x2026; p
    C  = {  C  j  j                                        {\displaystyle
&#x2032;    }                                              j=1\ldots p}  [ j =
{\displaystyle                             p &#x00D7; p    1 \ldots p ]
\mathbf {C} =\{C_   covariance_matrix   {\displaystyle         j &#x2032;  = 1
{jj'}\}}  [                             p\times p}  [ p    &#x2026; p
{\displaystyle                          \times p ]         {\displaystyle
\mathbf {C} =\{C_                                          j'=1\ldots p}  [
{jj'}\}}]                                                  {\displaystyle
                                                           j'=1\ldots p}]
                                                              j = 1 &#x2026; p
    R  = {  R  j  j                                        {\displaystyle
&#x2032;    }                                              j=1\ldots p}  [ j =
{\displaystyle                             p &#x00D7; p    1 \ldots p ]
\mathbf {R} =\{R_   correlation_matrix  {\displaystyle         j &#x2032;  = 1
{jj'}\}}  [                             p\times p}  [ p    &#x2026; p
{\displaystyle                          \times p ]         {\displaystyle
\mathbf {R} =\{R_                                          j'=1\ldots p}  [
{jj'}\}}]                                                  {\displaystyle
                                                           j'=1\ldots p}]
                                                              j = 1 &#x2026; p
    V  = {  V  j  j                                        {\displaystyle
&#x2032;    }       matrix consisting                      j=1\ldots p}  [ j =
{\displaystyle      of the set of all      p &#x00D7; p    1 \ldots p ]
\mathbf {V} =\{V_   eigenvectors of C,  {\displaystyle         j &#x2032;  = 1
{jj'}\}}  [         one eigenvector per p\times p}  [ p    &#x2026; p
{\displaystyle      column              \times p ]         {\displaystyle
\mathbf {V} =\{V_                                          j'=1\ldots p}  [
{jj'}\}}]                                                  {\displaystyle
                                                           j'=1\ldots p}]
                                                              j = 1 &#x2026; p
    D  = {  D  j  j diagonal_matrix                        {\displaystyle
&#x2032;    }       consisting of the                      j=1\ldots p}  [ j =
{\displaystyle      set of all             p &#x00D7; p    1 \ldots p ]
\mathbf {D} =\{D_   eigenvalues of C    {\displaystyle         j &#x2032;  = 1
{jj'}\}}  [         along its principal p\times p}  [ p    &#x2026; p
{\displaystyle      diagonal, and 0 for \times p ]         {\displaystyle
\mathbf {D} =\{D_   all other elements                     j'=1\ldots p}  [
{jj'}\}}]                                                  {\displaystyle
                                                           j'=1\ldots p}]
                    matrix of basis                           j = 1 &#x2026; p
    W  = {  W  j l  vectors, one vector                    {\displaystyle
}   {\displaystyle  per column, where                      j=1\ldots p}  [ j =
\mathbf {W} =\{W_   each basis vector      p &#x00D7; L    1 \ldots p ]
{jl}\}}  [          is one of the       {\displaystyle        l = 1 &#x2026; L
{\displaystyle      eigenvectors of C,  p\times L}  [ p    {\displaystyle
\mathbf {W} =\{W_   and where the       \times L]          l=1\ldots L}  [
{jl}\}}]            vectors in W are a                     {\displaystyle
                    sub-set of those in                    l=1\ldots L}]
                    V
                    matrix consisting
                    of n row vectors,                         i = 1 &#x2026; n
    T  = {  T  i l  where each vector                      {\displaystyle
}   {\displaystyle  is the projection      n &#x00D7; L    i=1\ldots n}  [ i =
\mathbf {T} =\{T_   of the              {\displaystyle     1 \ldots n ]
{il}\}}  [          corresponding data  n\times L}  [ n       l = 1 &#x2026; L
{\displaystyle      vector from matrix  \times L]          {\displaystyle
\mathbf {T} =\{T_   X onto the basis                       l=1\ldots L}  [
{il}\}}]            vectors contained                      {\displaystyle
                    in the columns of                      l=1\ldots L}]
                    matrix W.
***** Properties and limitations of PCA[edit] *****
**** Properties[edit] ****
Some properties of PCA include:[13]
      Property 1: For any integer q, 1 â¤ q â¤ p, consider the orthogonal
      linear_transformation
               y =   B &#x2032;   x   {\displaystyle y=\mathbf {B'} x}  [y
            =\mathbf{B'}x]
      where     y   {\displaystyle y}  [y] is a q-element vector and       B
      &#x2032;     {\displaystyle \mathbf {B'} }  [\mathbf{B'}] is a (q Ã p)
      matrix, and let       &#x03A3;   y   =   B &#x2032;    &#x03A3;   B
      {\displaystyle \mathbf {\Sigma } _{y}=\mathbf {B'} \mathbf {\Sigma }
      \mathbf {B} }  [{\mathbf  {{\Sigma }}}_{y}={\mathbf  {B'}}{\mathbf
      {\Sigma }}{\mathbf  {B}}] be the variance-covariance matrix for     y
      {\displaystyle y}  [y]. Then the trace of       &#x03A3;   y
      {\displaystyle \mathbf {\Sigma } _{y}}  [{\mathbf  {\Sigma }}_{y}],
      denoted      tr  (   &#x03A3;   y   )   {\displaystyle {\text{tr}}
      (\mathbf {\Sigma } _{y})}  [{\text{tr}}({\mathbf  {\Sigma }}_{y})], is
      maximized by taking      B  =   A   q     {\displaystyle \mathbf {B}
      =\mathbf {A} _{q}}  [\mathbf{B} = \mathbf{A}_q], where       A   q
      {\displaystyle \mathbf {A} _{q}}  [\mathbf{A}_q] consists of the first q
      columns of      A    {\displaystyle \mathbf {A} }  [\mathbf {A} ]
      (   B &#x2032;     {\displaystyle (\mathbf {B'} }  [(\mathbf{B'}] is the
      transposition of      B  )   {\displaystyle \mathbf {B} )}  [\mathbf
      {B})].
      Property 2: Consider again the orthonormal_transformation
               y =   B &#x2032;   x   {\displaystyle y=\mathbf {B'} x}  [y =
            \mathbf{B'}x]
      with     x ,  B  ,  A    {\displaystyle x,\mathbf {B} ,\mathbf {A} }  [x,
      {\mathbf  {B}},{\mathbf  {A}}] and       &#x03A3;   y     {\displaystyle
      \mathbf {\Sigma } _{y}}  [{\mathbf  {\Sigma }}_{y}] defined as before.
      Then      tr  (   &#x03A3;   y   )   {\displaystyle {\text{tr}}(\mathbf
      {\Sigma } _{y})}  [{\text{tr}}({\mathbf  {\Sigma }}_{y})] is minimized by
      taking      B  =   A   q   &#x2217;   ,   {\displaystyle \mathbf {B}
      =\mathbf {A} _{q}^{*},}  [{\mathbf  {B}}={\mathbf  {A}}_{q}^{*},] where
      A   q   &#x2217;     {\displaystyle \mathbf {A} _{q}^{*}}  [\mathbf
      {A}_q^*] consists of the last q columns of      A    {\displaystyle
      \mathbf {A} }  [\mathbf {A} ].
The statistical implication of this property is that the last few PCs are not
simply unstructured left-overs after removing the important PCs. Because these
last PCs have variances as small as possible they are useful in their own
right. They can help to detect unsuspected near-constant linear relationships
between the elements of x, and they may also be useful in regression, in
selecting a subset of variables from x, and in outlier detection.
      Property 3: (Spectral Decomposition of Î£)
                &#x03A3;  =  &#x03BB;  1    &#x03B1;  1    &#x03B1;  1
            &#x2032;  + &#x22EF; +  &#x03BB;  p    &#x03B1;  p    &#x03B1;  p
            &#x2032;    {\displaystyle \mathbf {\Sigma } =\lambda _{1}\alpha _
            {1}\alpha _{1}'+\cdots +\lambda _{p}\alpha _{p}\alpha _{p}'}  [
            {\mathbf  {{\Sigma }}}=\lambda _{{1}}\alpha _{{1}}\alpha _{
            {1}}'+\cdots +\lambda _{{p}}\alpha _{{p}}\alpha _{{p}}']
Before we look at its usage, we first look at diagonal elements,
          Var  (  x  j   ) =  &#x2211;  k = 1   P    &#x03BB;  k    &#x03B1;  k
      j   2     {\displaystyle {\text{Var}}(x_{j})=\sum _{k=1}^{P}\lambda _
      {k}\alpha _{kj}^{2}}  [{\text{Var}}(x_{j})=\sum _{{k=1}}^{P}\lambda _{
      {k}}\alpha _{{kj}}^{2}]
Then, perhaps the main statistical implication of the result is that not only
can we decompose the combined variances of all the elements of x into
decreasing contributions due to each PC, but we can also decompose the whole
covariance_matrix into contributions      &#x03BB;  k    &#x03B1;  k
&#x03B1;  k  &#x2032;    {\displaystyle \lambda _{k}\alpha _{k}\alpha _{k}'}
[\lambda_{k}\alpha_{k}\alpha_{k}'] from each PC. Although not strictly
decreasing, the elements of      &#x03BB;  k    &#x03B1;  k    &#x03B1;  k
&#x2032;    {\displaystyle \lambda _{k}\alpha _{k}\alpha _{k}'}  [\lambda_
{k}\alpha_{k}\alpha_{k}'] will tend to become smaller as     k   {\displaystyle
k}  [k] increases, as      &#x03BB;  k    &#x03B1;  k    &#x03B1;  k  &#x2032;
{\displaystyle \lambda _{k}\alpha _{k}\alpha _{k}'}  [\lambda_{k}\alpha_
{k}\alpha_{k}'] is nonincreasing for increasing     k   {\displaystyle k}  [k],
whereas the elements of      &#x03B1;  k     {\displaystyle \alpha _{k}}
[\alpha _{k}] tend to stay about the same size because of the normalization
constraints:      &#x03B1;  k  &#x2032;   &#x03B1;  k   = 1 , k = 1 , &#x22EF;
, p   {\displaystyle \alpha _{k}'\alpha _{k}=1,k=1,\cdots ,p}  [\alpha _{
{k}}'\alpha _{{k}}=1,k=1,\cdots ,p].
**** Limitations[edit] ****
As noted above, the results of PCA depend on the scaling of the variables. This
can be cured by scaling each feature by its standard deviation, so that one
ends up with dimensionless features with unital variance [14]
The applicability of PCA as described above is limited by certain (tacit)
assumptions [15] made in its derivation. In particular, PCA can capture linear
correlations between the features but fails when this assumption is violated
(see Figure 6a in the reference). In some cases, coordinate transformations can
restore the linearity assumption and PCA can then be applied (see kernel_PCA).
Another limitation is the mean-removal process before constructing the
covariance matrix for PCA. In fields such as astronomy, all the signals are
non-negative, and the mean-removal process will force the mean of some
astrophysical exposures to be zero, which consequently creates unphysical
negative fluxes,[16] and forward modeling has to be performed to recover the
true magnitude of the signals.[17] As an alternative method, non-negative
matrix_factorization focusing only on the non-negative elements in the
matrices, which is well-suited for astrophysical observations.[18][19][20] See
more at Relation_between_PCA_and_Non-negative_Matrix_Factorization.
**** PCA and information theory[edit] ****
Dimensionality reduction loses information, in general. PCA-based
dimensionality reduction tends to minimize that information loss, under certain
signal and noise models.
Under the assumption that
          x  =  s  +  n    {\displaystyle \mathbf {x} =\mathbf {s} +\mathbf {n}
      }  [\mathbf{x}=\mathbf{s}+\mathbf{n}]
i.e., that the data vector      x    {\displaystyle \mathbf {x} }  [\mathbf {x}
] is the sum of the desired information-bearing signal      s    {\displaystyle
\mathbf {s} }  [\mathbf {s} ] and a noise signal      n    {\displaystyle
\mathbf {n} }  [\mathbf {n} ] one can show that PCA can be optimal for
dimensionality reduction, from an information-theoretic point-of-view.
In particular, Linsker showed that if      s    {\displaystyle \mathbf {s} }
[\mathbf {s} ] is Gaussian and      n    {\displaystyle \mathbf {n} }  [\mathbf
{n} ] is Gaussian noise with a covariance matrix proportional to the identity
matrix, the PCA maximizes the mutual_information     I (  y  ;  s  )
{\displaystyle I(\mathbf {y} ;\mathbf {s} )}  [I(\mathbf{y};\mathbf{s})]
between the desired information      s    {\displaystyle \mathbf {s} }
[\mathbf {s} ] and the dimensionality-reduced output      y  =   W   L   T    x
{\displaystyle \mathbf {y} =\mathbf {W} _{L}^{T}\mathbf {x} }  [\mathbf
{y}=\mathbf{W}_L^T\mathbf{x}].[21]
If the noise is still Gaussian and has a covariance matrix proportional to the
identity matrix (i.e., the components of the vector      n    {\displaystyle
\mathbf {n} }  [\mathbf {n} ] are iid), but the information-bearing signal
s    {\displaystyle \mathbf {s} }  [\mathbf {s} ] is non-Gaussian (which is a
common scenario), PCA at least minimizes an upper bound on the information
loss, which is defined as[22][23]
         I (  x  ;  s  ) &#x2212; I (  y  ;  s  ) .   {\displaystyle I(\mathbf
      {x} ;\mathbf {s} )-I(\mathbf {y} ;\mathbf {s} ).}  [I(\mathbf{x};\mathbf
      {s})-I(\mathbf{y};\mathbf{s}).]
The optimality of PCA is also preserved if the noise      n    {\displaystyle
\mathbf {n} }  [\mathbf {n} ] is iid and at least more Gaussian (in terms of
the KullbackâLeibler_divergence) than the information-bearing signal      s
{\displaystyle \mathbf {s} }  [\mathbf {s} ].[24] In general, even if the above
signal model holds, PCA loses its information-theoretic optimality as soon as
the noise      n    {\displaystyle \mathbf {n} }  [\mathbf {n} ] becomes
dependent.
***** Computing PCA using the covariance method[edit] *****
The following is a detailed description of PCA using the covariance method (see
also here) as opposed to the correlation method.[25]
The goal is to transform a given data set X of dimension p to an alternative
data set Y of smaller dimension L. Equivalently, we are seeking to find the
matrix Y, where Y is the KarhunenâLoÃ¨ve transform (KLT) of matrix X:
          Y  =  K L T  {  X  }   {\displaystyle \mathbf {Y} =\mathbb {KLT} \
      {\mathbf {X} \}}  [ \mathbf{Y} = \mathbb{KLT} \{ \mathbf{X} \} ]
**** Organize the data set[edit] ****
Suppose you have data comprising a set of observations of p variables, and you
want to reduce the data so that each observation can be described with only L
variables, L < p. Suppose further, that the data are arranged as a set of n
data vectors       x   1   &#x2026;   x   n     {\displaystyle \mathbf {x} _
{1}\ldots \mathbf {x} _{n}}  [\mathbf{x}_1 \ldots \mathbf{x}_n] with each
x   i     {\displaystyle \mathbf {x} _{i}}  [\mathbf {x} _{i}] representing a
single grouped observation of the p variables.
    * Write       x   1   &#x2026;   x   n     {\displaystyle \mathbf {x} _
      {1}\ldots \mathbf {x} _{n}}  [\mathbf{x}_1 \ldots \mathbf{x}_n] as row
      vectors, each of which has p columns.
    * Place the row vectors into a single matrix X of dimensions n Ã p.
**** Calculate the empirical mean[edit] ****
    * Find the empirical mean along each column j = 1, ..., p.
    * Place the calculated mean values into an empirical mean vector u of
      dimensions p Ã 1.
                u  j   =   1 n    &#x2211;  i = 1   n    X  i j
            {\displaystyle u_{j}={1 \over n}\sum _{i=1}^{n}X_{ij}}  [
            {\displaystyle u_{j}={1 \over n}\sum _{i=1}^{n}X_{ij}}]
**** Calculate the deviations from the mean[edit] ****
Mean subtraction is an integral part of the solution towards finding a
principal component basis that minimizes the mean square error of approximating
the data.[26] Hence we proceed by centering the data as follows:
    * Subtract the empirical mean vector       u   T     {\displaystyle \mathbf
      {u} ^{T}}  [{\displaystyle \mathbf {u} ^{T}}] from each row of the data
      matrix X.
    * Store mean-subtracted data in the n Ã p matrix B.
                B  =  X  &#x2212;  h    u   T     {\displaystyle \mathbf {B}
            =\mathbf {X} -\mathbf {h} \mathbf {u} ^{T}}  [\mathbf{B} = \mathbf
            {X} - \mathbf{h}\mathbf{u}^{T} ]
            where h is an n Ã 1 column vector of all 1s:
                      h  i   = 1     for&#xA0;  i = 1 , &#x2026; , n
                  {\displaystyle h_{i}=1\,\qquad \qquad {\text{for }}i=1,\ldots
                  ,n}  [{\displaystyle h_{i}=1\,\qquad \qquad {\text{for
                  }}i=1,\ldots ,n}]
**** Find the covariance matrix[edit] ****
    * Find the p Ã p empirical covariance_matrix C from matrix B:
                C  =   1  n &#x2212; 1      B   &#x2217;    B    {\displaystyle
            \mathbf {C} ={1 \over {n-1}}\mathbf {B} ^{*}\mathbf {B} }  [
            {\displaystyle \mathbf {C} ={1 \over {n-1}}\mathbf {B} ^{*}\mathbf
            {B} }]
      where     &#x2217;   {\displaystyle *}  [*] is the conjugate_transpose
      operator. If B consists entirely of real numbers, which is the case in
      many applications, the "conjugate transpose" is the same as the regular
      transpose.
    * The reasoning behind using n â 1 instead of n to calculate the
      covariance is Bessel's_correction.
**** Find the eigenvectors and eigenvalues of the covariance matrix[edit] ****
    * Compute the matrix V of eigenvectors which diagonalizes the covariance
      matrix C:
                 V   &#x2212; 1    C   V  =  D    {\displaystyle \mathbf {V} ^
            {-1}\mathbf {C} \mathbf {V} =\mathbf {D} }  [\mathbf{V}^{-1}
            \mathbf{C} \mathbf{V} = \mathbf{D} ]
      where D is the diagonal_matrix of eigenvalues of C. This step will
      typically involve the use of a computer-based algorithm for computing
      eigenvectors and eigenvalues. These algorithms are readily available as
      sub-components of most matrix_algebra systems, such as SAS,[27] R,
      MATLAB,[28][29] Mathematica,[30] SciPy, IDL (Interactive_Data_Language),
      or GNU_Octave as well as OpenCV.
    * Matrix D will take the form of an p Ã p diagonal matrix, where
                D  k l   =  &#x03BB;  k     for&#xA0;  k = l   {\displaystyle
            D_{kl}=\lambda _{k}\qquad {\text{for }}k=l}  [{\displaystyle D_
            {kl}=\lambda _{k}\qquad {\text{for }}k=l}]
      is the jth eigenvalue of the covariance matrix C, and
                D  k l   = 0   for&#xA0;  k &#x2260; l .   {\displaystyle D_
            {kl}=0\qquad {\text{for }}k\neq l.}  [{\displaystyle D_{kl}=0\qquad
            {\text{for }}k\neq l.}]
    * Matrix V, also of dimension p Ã p, contains p column vectors, each of
      length p, which represent the p eigenvectors of the covariance matrix C.
    * The eigenvalues and eigenvectors are ordered and paired. The jth
      eigenvalue corresponds to the jth eigenvector.
    * Matrix V denotes the matrix of right eigenvectors (as opposed to left
      eigenvectors). In general, the matrix of right eigenvectors need not be
      the (conjugate) transpose of the matrix of left eigenvectors.
**** Rearrange the eigenvectors and eigenvalues[edit] ****
    * Sort the columns of the eigenvector matrix V and eigenvalue matrix D in
      order of decreasing eigenvalue.
    * Make sure to maintain the correct pairings between the columns in each
      matrix.
**** Compute the cumulative energy content for each eigenvector[edit] ****
    * The eigenvalues represent the distribution of the source data's energy
      [clarification_needed] among each of the eigenvectors, where the
      eigenvectors form a basis for the data. The cumulative energy content g
      for the jth eigenvector is the sum of the energy content across all of
      the eigenvalues from 1 through j:
                g  j   =  &#x2211;  k = 1   j    D  k k     f o r   j = 1 ,
            &#x2026; , p   {\displaystyle g_{j}=\sum _{k=1}^{j}D_{kk}\qquad
            \mathrm {for} \qquad j=1,\dots ,p}  [{\displaystyle g_{j}=\sum _
            {k=1}^{j}D_{kk}\qquad \mathrm {for} \qquad j=1,\dots ,p}][citation
            needed]
**** Select a subset of the eigenvectors as basis vectors[edit] ****
    * Save the first L columns of V as the p Ã L matrix W:
                W  k l   =  V  k l     f o r   k = 1 , &#x2026; , p  l = 1 ,
            &#x2026; , L   {\displaystyle W_{kl}=V_{kl}\qquad \mathrm {for}
            \qquad k=1,\dots ,p\qquad l=1,\dots ,L}  [{\displaystyle W_{kl}=V_
            {kl}\qquad \mathrm {for} \qquad k=1,\dots ,p\qquad l=1,\dots ,L}]
      where
               1 &#x2264; L &#x2264; p .   {\displaystyle 1\leq L\leq p.}  [1
            \leq L \leq p.]
    * Use the vector g as a guide in choosing an appropriate value for L. The
      goal is to choose a value of L as small as possible while achieving a
      reasonably high value of g on a percentage basis. For example, you may
      want to choose L so that the cumulative energy g is above a certain
      threshold, like 90 percent. In this case, choose the smallest value of L
      such that
                  g  L    g  p     &#x2265; 0.9    {\displaystyle {\frac {g_
            {L}}{g_{p}}}\geq 0.9\,}  [{\displaystyle {\frac {g_{L}}{g_{p}}}\geq
            0.9\,}]
**** Project the z-scores of the data onto the new basis[edit] ****
    * The projected vectors are the columns of the matrix
                T  =  Z  &#x22C5;  W  =  K L T  {  X  } .   {\displaystyle
            \mathbf {T} =\mathbf {Z} \cdot \mathbf {W} =\mathbb {KLT} \{\mathbf
            {X} \}.}  [ \mathbf{T} =  \mathbf{Z} \cdot \mathbf{W} = \mathbb
            {KLT} \{ \mathbf{X} \}.]
    * The rows of matrix T represent the Kosambi-KarhunenâLoÃ¨ve transforms
      (KLT) of the data vectors in the rows of matrix X.
***** Derivation of PCA using the covariance method[edit] *****
Let X be a d-dimensional random vector expressed as column vector. Without loss
of generality, assume X has zero mean.
We want to find     ( &#x2217; )    {\displaystyle (\ast )\,}  [(\ast)\,] a d
Ã d orthonormal_transformation_matrix P so that PX has a diagonal covariance
matrix (i.e. PX is a random vector with all its distinct components pairwise
uncorrelated).
A quick computation assuming     P   {\displaystyle P}  [P] were unitary
yields:
             cov &#x2061; ( P X )    =  E  [ P X &#xA0; ( P X  )  &#x2217;   ]
      =  E  [ P X &#xA0;  X  &#x2217;    P  &#x2217;   ]       = P &#xA0;  E
      [ X  X  &#x2217;   ]  P  &#x2217;         = P &#xA0; cov &#x2061; ( X )
      P  &#x2212; 1         {\displaystyle {\begin{aligned}\operatorname {cov}
      (PX)&=\mathbb {E} [PX~(PX)^{*}]\\&=\mathbb {E} [PX~X^{*}P^
      {*}]\\&=P~\mathbb {E} [XX^{*}]P^{*}\\&=P~\operatorname {cov} (X)P^{-
      1}\\\end{aligned}}}  [{\displaystyle {\begin{aligned}\operatorname {cov}
      (PX)&=\mathbb {E} [PX~(PX)^{*}]\\&=\mathbb {E} [PX~X^{*}P^
      {*}]\\&=P~\mathbb {E} [XX^{*}]P^{*}\\&=P~\operatorname {cov} (X)P^{-
      1}\\\end{aligned}}}]
Hence     ( &#x2217; )    {\displaystyle (\ast )\,}  [(\ast)\,] holds if and
only if     cov &#x2061; ( X )   {\displaystyle \operatorname {cov} (X)}
[\operatorname {cov}(X)] were diagonalisable by     P   {\displaystyle P}  [P].
This is very constructive, as cov(X) is guaranteed to be a non-negative
definite matrix and thus is guaranteed to be diagonalisable by some unitary
matrix.
***** Covariance-free computation[edit] *****
In practical implementations, especially with high_dimensional_data (large p),
the naive covariance method is rarely used because it is not efficient due to
high computational and memory costs of explicitly determining the covariance
matrix. The covariance-free approach avoids the np2 operations of explicitly
calculating and storing the covariance matrix XTX, instead utilizing one of
matrix-free_methods, e.g., based on the function evaluating the product XT(X r)
at the cost of 2np operations.
**** Iterative computation[edit] ****
One way to compute the first principal component efficiently[31] is shown in
the following pseudo-code, for a data matrix X with zero mean, without ever
computing its covariance matrix.
r = a random vector of length p





          r

        =



              r



                |


                r


                |






    {\displaystyle \mathbf {r} ={\frac {\mathbf {r} }{|\mathbf {r} |}}}

[\mathbf{r} = \frac{\mathbf{r}}{|\mathbf{r}|}]
do c times:
      s = 0 (a vector of length p)
      for each row




          x

        &#x2208;

          X



    {\displaystyle \mathbf {x} \in \mathbf {X} }

[\mathbf{x} \in \mathbf{X}]





          s

        =

          s

        +
        (

          x

        &#x22C5;

          r

        )

          x



    {\displaystyle \mathbf {s} =\mathbf {s} +(\mathbf {x} \cdot \mathbf {r}
)\mathbf {x} }

[\mathbf{s} = \mathbf{s} + (\mathbf{x} \cdot \mathbf{r})\mathbf{x}]




        e
        i
        g
        e
        n
        v
        a
        l
        u
        e
        =


            r


            T



          s



    {\displaystyle eigenvalue=\mathbf {r} ^{T}\mathbf {s} }

[{\displaystyle eigenvalue=\mathbf {r} ^{T}\mathbf {s} }]




        e
        r
        r
        o
        r
        =

          |

        e
        i
        g
        e
        n
        v
        a
        l
        u
        e
        &#x22C5;

          r

        &#x2212;

          s


          |



    {\displaystyle error=|eigenvalue\cdot \mathbf {r} -\mathbf {s} |}

[{\displaystyle error=|eigenvalue\cdot \mathbf {r} -\mathbf {s} |}]





          r

        =



              s



                |


                s


                |






    {\displaystyle \mathbf {r} ={\frac {\mathbf {s} }{|\mathbf {s} |}}}

[\mathbf{r} = \frac{\mathbf{s}}{|\mathbf{s}|}]
      exit if



        e
        r
        r
        o
        r
        <
        t
        o
        l
        e
        r
        a
        n
        c
        e


    {\displaystyle error<tolerance}

[{\displaystyle error<tolerance}]
return



        e
        i
        g
        e
        n
        v
        a
        l
        u
        e
        ,

          r



    {\displaystyle eigenvalue,\mathbf {r} }

[{\displaystyle eigenvalue,\mathbf {r} }]
This power_iteration algorithm simply calculates the vector XT(X r),
normalizes, and places the result back in r. The eigenvalue is approximated by
rT (XTX) r, which is the Rayleigh_quotient on the unit vector r for the
covariance matrix XTX. If the largest singular value is well separated from the
next largest one, the vector r gets close to the first principal component of X
within the number of iterations c, which is small relative to p, at the total
cost 2cnp. The power_iteration convergence can be accelerated without
noticeably sacrificing the small cost per iteration using more advanced matrix-
free_methods, such as the Lanczos_algorithm or the Locally Optimal Block
Preconditioned Conjugate Gradient (LOBPCG) method.
Subsequent principal components can be computed one-by-one via deflation or
simultaneously as a block. In the former approach, imprecisions in already
computed approximate principal components additively affect the accuracy of the
subsequently computed principal components, thus increasing the error with
every new computation. The latter approach in the block power method replaces
single-vectors r and s with block-vectors, matrices R and S. Every column of R
approximates one of the leading principal components, while all columns are
iterated simultaneously. The main calculation is evaluation of the product XT(X
R). Implemented, e.g., in LOBPCG, efficient blocking eliminates the
accumulation of the errors, allows using high-level BLAS matrix-matrix product
functions, and typically leads to faster convergence, compared to the single-
vector one-by-one technique.
**** The NIPALS method[edit] ****
Non-linear iterative partial least squares (NIPALS) is a variant the classical
power_iteration with matrix deflation by subtraction implemented for computing
the first few components in a principal component or partial_least_squares
analysis. For very-high-dimensional datasets, such as those generated in the
*omics sciences (e.g., genomics, metabolomics) it is usually only necessary to
compute the first few PCs. The non-linear_iterative_partial_least_squares
(NIPALS) algorithm updates iterative approximations to the leading scores and
loadings t1 and r1T by the power_iteration multiplying on every iteration by X
on the left and on the right, i.e. calculation of the covariance matrix is
avoided, just as in the matrix-free implementation of the power iterations to
XTX, based on the function evaluating the product XT(X r) = ((X r)TX)T.
The matrix deflation by subtraction is performed by subtracting the outer
product, t1r1T from X leaving the deflated residual matrix used to calculate
the subsequent leading PCs.[32] For large data matrices, or matrices that have
a high degree of column collinearity, NIPALS suffers from loss of orthogonality
of PCs due to machine precision round-off_errors accumulated in each iteration
and matrix deflation by subtraction.[33] A GramâSchmidt re-orthogonalization
algorithm is applied to both the scores and the loadings at each iteration step
to eliminate this loss of orthogonality.[34] NIPALS reliance on single-vector
multiplications cannot take advantage of high-level BLAS and results in slow
convergence for clustered leading singular valuesâboth these deficiencies are
resolved in more sophisticated matrix-free block solvers, such as the Locally
Optimal Block Preconditioned Conjugate Gradient (LOBPCG) method.
**** Online/sequential estimation[edit] ****
In an "online" or "streaming" situation with data arriving piece by piece
rather than being stored in a single batch, it is useful to make an estimate of
the PCA projection that can be updated sequentially. This can be done
efficiently, but requires different algorithms.[35]
***** PCA and qualitative variables[edit] *****
In PCA, it is common that we want to introduce qualitative variables as
supplementary elements. For example, many quantitative variables have been
measured on plants. For these plants, some qualitative variables are available
as, for example, the species to which the plant belongs. These data were
subjected to PCA for quantitative variables. When analyzing the results, it is
natural to connect the principal components to the qualitative variable
species. For this, the following results are produced.
    * Identification, on the factorial planes, of the different species e.g.
      using different colors.
    * Representation, on the factorial planes, of the centers of gravity of
      plants belonging to the same species.
    * For each center of gravity and each axis, p-value to judge the
      significance of the difference between the center of gravity and origin.
These results are what is called introducing a qualitative variable as
supplementary element. This procedure is detailed in and Husson, LÃª & PagÃ¨s
2009 and PagÃ¨s 2013. Few software offer this option in an "automatic" way.
This is the case of SPAD that historically, following the work of Ludovic
Lebart, was the first to propose this option, and the R package FactoMineR.
***** Applications[edit] *****
**** Quantitative finance[edit] ****
See also: Portfolio_optimization
In quantitative_finance, principal component analysis can be directly applied
to the risk_management of interest_rate_derivative portfolios.[36] Trading
multiple swap_instruments which are usually a function of 30-500 other market
quotable swap instruments is sought to be reduced to usually 3 or 4 principal
components, representing the path of interest rates on a macro basis.
Converting risks to be represented as those to factor loadings (or multipliers)
provides assessments and understanding beyond that available to simply
collectively viewing risks to individual 30-500 buckets.
PCA has also been applied to equity_portfolios in a similar fashion,[37] both
to portfolio_risk and to risk_return. One application is to reduce portfolio
risk, where allocation_strategies are applied to the "principal portfolios"
instead of the underlying stocks.[38] A second is to enhance portfolio return,
using the principal components to select_stocks with upside potential.[39]
**** Neuroscience[edit] ****
A variant of principal components analysis is used in neuroscience to identify
the specific properties of a stimulus that increase a neuron's probability of
generating an action_potential.[40] This technique is known as spike-triggered
covariance_analysis. In a typical application an experimenter presents a white
noise process as a stimulus (usually either as a sensory input to a test
subject, or as a current injected directly into the neuron) and records a train
of action potentials, or spikes, produced by the neuron as a result.
Presumably, certain features of the stimulus make the neuron more likely to
spike. In order to extract these features, the experimenter calculates the
covariance_matrix of the spike-triggered ensemble, the set of all stimuli
(defined and discretized over a finite time window, typically on the order of
100 ms) that immediately preceded a spike. The eigenvectors of the difference
between the spike-triggered covariance matrix and the covariance matrix of the
prior stimulus ensemble (the set of all stimuli, defined over the same length
time window) then indicate the directions in the space of stimuli along which
the variance of the spike-triggered ensemble differed the most from that of the
prior stimulus ensemble. Specifically, the eigenvectors with the largest
positive eigenvalues correspond to the directions along which the variance of
the spike-triggered ensemble showed the largest positive change compared to the
variance of the prior. Since these were the directions in which varying the
stimulus led to a spike, they are often good approximations of the sought after
relevant stimulus features.
In neuroscience, PCA is also used to discern the identity of a neuron from the
shape of its action potential. Spike_sorting is an important procedure because
extracellular recording techniques often pick up signals from more than one
neuron. In spike sorting, one first uses PCA to reduce the dimensionality of
the space of action potential waveforms, and then performs clustering_analysis
to associate specific action potentials with individual neurons.
PCA as a dimension reduction technique is particularly suited to detect
coordinated activities of large neuronal ensembles. It has been used in
determining collective variables, i.e. order_parameters, during phase
transitions in the brain.[41]
***** Relation with other methods[edit] *****
**** Correspondence analysis[edit] ****
Correspondence_analysis (CA) was developed by Jean-Paul_BenzÃ©cri[42] and is
conceptually similar to PCA, but scales the data (which should be non-negative)
so that rows and columns are treated equivalently. It is traditionally applied
to contingency_tables. CA decomposes the chi-squared_statistic associated to
this table into orthogonal factors.[43] Because CA is a descriptive technique,
it can be applied to tables for which the chi-squared statistic is appropriate
or not. Several variants of CA are available including detrended_correspondence
analysis and canonical_correspondence_analysis. One special extension is
multiple_correspondence_analysis, which may be seen as the counterpart of
principal component analysis for categorical data.[44]
**** Factor analysis[edit] ****
Principal component analysis creates variables that are linear combinations of
the original variables. The new variables have the property that the variables
are all orthogonal. The PCA transformation can be helpful as a pre-processing
step before clustering. PCA is a variance-focused approach seeking to reproduce
the total variable variance, in which components reflect both common and unique
variance of the variable. PCA is generally preferred for purposes of data
reduction (i.e., translating variable space into optimal factor space) but not
when the goal is to detect the latent construct or factors.
Factor_analysis is similar to principal component analysis, in that factor
analysis also involves linear combinations of variables. Different from PCA,
factor analysis is a correlation-focused approach seeking to reproduce the
inter-correlations among variables, in which the factors "represent the common
variance of variables, excluding unique variance".[45] In terms of the
correlation matrix, this corresponds with focusing on explaining the off-
diagonal terms (i.e. shared co-variance), while PCA focuses on explaining the
terms that sit on the diagonal. However, as a side result, when trying to
reproduce the on-diagonal terms, PCA also tends to fit relatively well the off-
diagonal correlations.[46] Results given by PCA and factor analysis are very
similar in most situations, but this is not always the case, and there are some
problems where the results are significantly different. Factor analysis is
generally used when the research purpose is detecting data structure (i.e.,
latent constructs or factors) or causal modeling.
**** K-means clustering[edit] ****
It was asserted in [47][48] that the relaxed solution of k-means_clustering,
specified by the cluster indicators, is given by the principal components, and
the PCA subspace spanned by the principal directions is identical to the
cluster centroid subspace. However, that PCA is a useful relaxation of k-means
clustering was not a new result (see, for example,[49]), and it is
straightforward to uncover counterexamples to the statement that the cluster
centroid subspace is spanned by the principal directions.[50]
**** Non-negative matrix factorization[edit] ****
Fractional residual variance (FRV) plots for PCA and NMF;[20] for PCA, the
theoretical values are the contribution from the residual eigenvalues. In
comparison, the FRV curves for PCA reaches a flat plateau where no signal are
captured effectively; while the NMF FRV curves are declining continuously,
indicating a better ability to capture signal. The FRV curves for NMF also
converges to higher levels than PCA, indicating the less-overfitting property
of NMF.
Non-negative_matrix_factorization (NMF) is a dimension reduction method where
only non-negative elements in the matrices are used, which is therefore a
promising method in astronomy,[18][19][20] in the sense that astrophysical
signals are non-negative. The PCA components are orthogonal to each other,
while the NMF components are all non-negative and therefore constructs a non-
orthogonal basis.
In PCA, the contribution of each component is ranked based on the magnitude of
its corresponding eigenvalue, which is equivalent to the fractional residual
variance (FRV) in analyzing empirical data.[16] For NMF, its components are
ranked based only on the empirical FRV curves.[20] The residual fractional
eigenvalue plots, i.e.,     1 &#x2212;  &#x2211;  i = 1   k    &#x03BB;  i    /
&#x2211;  k = 1   n    &#x03BB;  k     {\displaystyle 1-\sum _{i=1}^{k}\lambda
_{i}/\sum _{k=1}^{n}\lambda _{k}}  [{\displaystyle 1-\sum _{i=1}^{k}\lambda _
{i}/\sum _{k=1}^{n}\lambda _{k}}] as a function of component number     k
{\displaystyle k}  [k] given a total of     n   {\displaystyle n}  [n]
components, for PCA has a flat plateau, where no data is captured to remove the
quasi-static noise, then the curves dropped quickly as an indication of over-
fitting and captures random noise.[16] The FRV curves for NMF is decreasing
continuously [20] when the NMF components are constructed sequentially,[19]
indicating the continuous capturing of quasi-static noise; then converge to
higher levels than PCA,[20] indicating the less over-fitting property of NMF.
***** Generalizations[edit] *****
**** Sparse PCA[edit] ****
Main article: Sparse_PCA
A particular disadvantage of PCA is that the principal components are usually
linear combinations of all input variables. Sparse_PCA overcomes this
disadvantage by finding linear combinations that contain just a few input
variables. It extends the classic method of principal component analysis (PCA)
for the reduction of dimensionality of data by adding sparsity constraint on
the input variables. Several approaches have been proposed, including
    * a regression framework,[51]
    * a convex relaxation/semidefinite programming framework,[52]
    * a generalized power method framework[53]
    * an alternating maximization framework[54]
    * forward-backward greedy search and exact methods using branch-and-bound
      techniques,[55]
    * Bayesian formulation framework.[56]
The methodological and theoretical developments of Sparse PCA as well as its
applications in scientific studies are recently reviewed in a survey paper.[57]
**** Nonlinear PCA[edit] ****
Linear PCA versus nonlinear Principal Manifolds[58] for visualization of breast
cancer microarray data: a) Configuration of nodes and 2D Principal Surface in
the 3D PCA linear manifold. The dataset is curved and cannot be mapped
adequately on a 2D principal plane; b) The distribution in the internal 2D non-
linear principal surface coordinates (ELMap2D) together with an estimation of
the density of points; c) The same as b), but for the linear 2D PCA manifold
(PCA2D). The "basal" breast cancer subtype is visualized more adequately with
ELMap2D and some features of the distribution become better resolved in
comparison to PCA2D. Principal manifolds are produced by the elastic_maps
algorithm. Data are available for public competition.[59] Software is available
for free non-commercial use.[60]
Most of the modern methods for nonlinear_dimensionality_reduction find their
theoretical and algorithmic roots in PCA or K-means. Pearson's original idea
was to take a straight line (or plane) which will be "the best fit" to a set of
data points. Principal curves and manifolds[61] give the natural geometric
framework for PCA generalization and extend the geometric interpretation of PCA
by explicitly constructing an embedded manifold for data approximation, and by
encoding using standard geometric projection onto the manifold, as it is
illustrated by Fig. See also the elastic_map algorithm and principal_geodesic
analysis. Another popular generalization is kernel_PCA, which corresponds to
PCA performed in a reproducing kernel Hilbert space associated with a positive
definite kernel.
In multilinear_subspace_learning,[62] PCA is generalized to multilinear_PCA
(MPCA) that extracts features directly from tensor representations. MPCA is
solved by performing PCA in each mode of the tensor iteratively. MPCA has been
applied to face recognition, gait recognition, etc. MPCA is further extended to
uncorrelated MPCA, non-negative MPCA and robust MPCA.
N-way principal component analysis may be performed with models such as Tucker
decomposition, PARAFAC, multiple factor analysis, co-inertia analysis, STATIS,
and DISTATIS.
**** Robust PCA[edit] ****
While PCA finds the mathematically optimal method (as in minimizing the squared
error), it is still sensitive to outliers in the data that produce large
errors, something that the method tries to avoid in the first place. It is
therefore common practice to remove outliers before computing PCA. However, in
some contexts, outliers can be difficult to identify. For example, in data
mining algorithms like correlation_clustering, the assignment of points to
clusters and outliers is not known beforehand. A recently proposed
generalization of PCA[63] based on a weighted PCA increases robustness by
assigning different weights to data objects based on their estimated relevancy.
Outlier-resistant versions of PCA have also been proposed on L1-norm
formulations (L1-PCA).[64]
Robust_principal_component_analysis (RPCA) via decomposition in low-rank and
sparse matrices is a modification of PCA that works well with respect to
grossly corrupted observations.[65][66][67]
***** Similar techniques[edit] *****
**** Independent component analysis[edit] ****
Independent_component_analysis (ICA) is directed to similar problems as
principal component analysis, but finds additively separable components rather
than successive approximations.
**** Network component analysis[edit] ****
Given a matrix     E   {\displaystyle E}  [E], it tries to decompose it into
two matrices such that     E = A P   {\displaystyle E=AP}  [E=AP
]. A key difference from techniques such as PCA and ICA is that some of the
entries of     A   {\displaystyle A}  [A] are constrained to be 0. Here     P
{\displaystyle P}  [P] is termed the regulatory layer. While in general such a
decomposition can have multiple solutions, they prove that if the following
conditions are satisfied :
   1.    A   {\displaystyle A}  [A] has full column rank
   2. Each column of     A   {\displaystyle A}  [A] must have at least     L
      &#x2212; 1   {\displaystyle L-1}  [L-1] zeroes where     L
      {\displaystyle L}  [L] is the number of columns of     A   {\displaystyle
      A}  [A] (or alternatively the number of rows of     P   {\displaystyle P}
      [P]). The justification for this criterion is that if a node is removed
      from the regulatory layer along with all the output nodes connected to
      it, the result must still be characterized by a connectivity matrix with
      full column rank.
   3.    P   {\displaystyle P}  [P] must have full row rank.
then the decomposition is unique up to multiplication by a scalar.[68]
***** Software/source code[edit] *****
    * ALGLIB - a C++ and C# library that implements PCA and truncated PCA
    * Analytica â The built-in EigenDecomp function computes principal
      components.
    * ELKI â includes PCA for projection, including robust variants of PCA,
      as well as PCA-based clustering_algorithms.
    * Gretl â principal component analysis can be performed either via the
      pca command or via the princomp() function.
    * Julia â Supports PCA with the pca function in the MultivariateStats
      package
    * KNIME â A java based nodal arranging software for Analysis, in this the
      nodes called PCA, PCA compute, PCA Apply, PCA inverse make it easily.
    * Mathematica â Implements principal component analysis with the
      PrincipalComponents command using both covariance and correlation
      methods.
    * MATLAB Statistics Toolbox â The functions princomp and pca (R2012b)
      give the principal components, while the function pcares gives the
      residuals and reconstructed matrix for a low-rank PCA approximation.
    * Matplotlib â Python library have a PCA package in the .mlab module.
    * mlpack â Provides an implementation of principal component analysis in
      C++.
    * NAG_Library â Principal components analysis is implemented via the
      g03aa routine (available in both the Fortran versions of the Library).
    * NMath â Proprietary numerical library containing PCA for the .NET
      Framework.
    * GNU_Octave â Free software computational environment mostly compatible
      with MATLAB, the function princomp gives the principal component.
    * OpenCV
    * Oracle_Database 12c â Implemented via
      DBMS_DATA_MINING.SVDS_SCORING_MODE by specifying setting value
      SVDS_SCORING_PCA
    * Orange_(software) â Integrates PCA in its visual programming
      environment. PCA displays a scree plot (degree of explained variance)
      where user can interactively select the number of principal components.
    * Origin â Contains PCA in its Pro version.
    * Qlucore â Commercial software for analyzing multivariate data with
      instant response using PCA.
    * R â Free statistical package, the functions princomp and prcomp can be
      used for principal component analysis; prcomp uses singular_value
      decomposition which generally gives better numerical accuracy. Some
      packages that implement PCA in R, include, but are not limited to: ade4,
      vegan, ExPosition, dimRed, and FactoMineR.
    * SAS - Proprietary software; for example, see [69]
    * Scikit-learn â Python library for machine learning which contains PCA,
      Probabilistic PCA, Kernel PCA, Sparse PCA and other techniques in the
      decomposition module.
    * Weka â Java library for machine learning which contains modules for
      computing principal components.
***** See also[edit] *****
    * Correspondence_analysis (for contingency tables)
    * Multiple_correspondence_analysis (for qualitative variables)
    * Factor_analysis_of_mixed_data (for quantitative and qualitative
      variables)
    * Canonical_correlation
    * CUR_matrix_approximation (can replace of low-rank SVD approximation)
    * Detrended_correspondence_analysis
    * Dynamic_mode_decomposition
    * Eigenface
    * Exploratory_factor_analysis (Wikiversity)
    * Factorial_code
    * Functional_principal_component_analysis
    * Geometric_data_analysis
    * Independent_component_analysis
    * Kernel_PCA
    * L1-norm_principal_component_analysis
    * Low-rank_approximation
    * Matrix_decomposition
    * Non-negative_matrix_factorization
    * Nonlinear_dimensionality_reduction
    * Oja's_rule
    * Point_distribution_model (PCA applied to morphometry and computer vision)
    * Principal_component_analysis (Wikibooks)
    * Principal_component_regression
    * Singular_spectrum_analysis
    * Singular_value_decomposition
    * Sparse_PCA
    * Transform_coding
    * Weighted_least_squares
***** References[edit] *****
   1. ^Pearson,_K. (1901). "On_Lines_and_Planes_of_Closest_Fit_to_Systems_of
      Points_in_Space". Philosophical Magazine. 2 (11): 559â572. doi:10.1080/
      14786440109462720.
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
   3. ^ Hotelling, H. (1933). Analysis of a complex of statistical variables
      into principal components. Journal_of_Educational_Psychology, 24,
      417â441, and 498â520.
      Hotelling, H (1936). "Relations between two sets of variates".
      Biometrika. 28 (3/4): 321â377. doi:10.2307/2333955. JSTOR 2333955.
   4. ^ a b Jolliffe I.T. Principal Component Analysis, Series: Springer Series
      in Statistics, 2nd ed., Springer, NY, 2002, XXIX, 487 p. 28 illus.
   5. ISBN 978-0-387-95442-4
   6. ^Abdi._H. & Williams, L.J. (2010). "Principal component analysis". Wiley
      Interdisciplinary Reviews: Computational Statistics. 2 (4): 433â459.
      arXiv:1108.4372. doi:10.1002/wics.101.
   7. ^ Shaw P.J.A. (2003) Multivariate statistics for the Environmental
      Sciences, Hodder-Arnold.
   8. ISBN 0-340-80763-6.[page needed]
   9. ^Barnett, T. P. & R. Preisendorfer. (1987). "Origins and levels of
      monthly and seasonal forecast skill for United States surface air
      temperatures determined by canonical correlation analysis". Monthly
      Weather Review. 115 (9): 1825. doi:10.1175/1520-0493(1987)115<1825:
      oaloma>2.0.co;2.
  10. ^Hsu, Daniel; Kakade, Sham M.; Zhang, Tong (2008). "A spectral algorithm
      for learning hidden markov models". arXiv:0811.4413. Bibcode:
      2008arXiv0811.4413H.
  11. ^Bengio, Y.; et al. (2013). "Representation Learning: A Review and New
      Perspectives". IEEE Transactions on Pattern Analysis and Machine
      Intelligence. 35 (8): 1798â1828. arXiv:1206.5538. doi:10.1109/
      TPAMI.2013.50.
  12. ^ A. A. Miranda, Y. A. Le Borgne, and G. Bontempi. New_Routes_from
      Minimal_Approximation_Error_to_Principal_Components, Volume 27, Number 3
      / June, 2008, Neural Processing Letters, Springer
  13. ^Plaut, E (2018). "From Principal Subspaces to Principal Components with
      Linear Autoencoders". arXiv:1804.10253 [stat.ML].
  14. ^Fukunaga, Keinosuke (1990). Introduction_to_Statistical_Pattern
      Recognition. Elsevier. ISBN 978-0-12-269851-4.
  15. ^Alizadeh, Elaheh; Lyons, Samanthe M; Castle, Jordan M; Prasad, Ashok
      (2016). "Measuring_systematic_changes_in_invasive_cancer_cell_shape_using
      Zernike_moments". Integrative Biology. 8 (11): 1183â1193. doi:10.1039/
      C6IB00100A. PMID 27735002.
  16. ^ Jolliffe, I. T. (2002). Principal Component Analysis, second edition
      Springer-Verlag.
  17. ISBN 978-0-387-95442-4.
  18. ^ Leznik, M; Tofallis, C. 2005 Estimating_Invariant_Principal_Components
      Using_Diagonal_Regression.
  19. ^ Jonathon Shlens, A_Tutorial_on_Principal_Component_Analysis.
  20. ^ a b cSoummer, RÃ©mi; Pueyo, Laurent; Larkin, James (2012). "Detection
      and Characterization of Exoplanets and Disks Using Projections on
      Karhunen-LoÃ¨ve Eigenimages". The Astrophysical Journal Letters. 755 (2):
      L28. arXiv:1207.4197. Bibcode:2012ApJ...755L..28S. doi:10.1088/2041-8205/
      755/2/L28.
  21. ^Pueyo, Laurent (2016). "Detection and Characterization of Exoplanets
      using Projections on Karhunen Loeve Eigenimages: Forward Modeling". The
      Astrophysical Journal. 824 (2): 117. arXiv:1604.06097. Bibcode:
      2016ApJ...824..117P. doi:10.3847/0004-637X/824/2/117.
  22. ^ a bBlanton, Michael R.; Roweis, Sam (2007). "K-corrections and filter
      transformations in the ultraviolet, optical, and near infrared". The
      Astronomical Journal. 133 (2): 734â754. arXiv:astro-ph/0606170.
      Bibcode:2007AJ....133..734B. doi:10.1086/510127.
  23. ^ a b cZhu, Guangtun B. (2016-12-19). "Nonnegative Matrix Factorization
      (NMF) with Heteroscedastic Uncertainties and Missing data". arXiv:
      1612.06037 [astro-ph.IM].
  24. ^ a b c d e fRen, Bin; Pueyo, Laurent; Zhu, Guangtun B.; DuchÃªne,
      Gaspard (2018). "Non-negative Matrix Factorization: Robust Extraction of
      Extended Structures". The Astrophysical Journal. 852 (2): 104. arXiv:
      1712.10317. Bibcode:2018ApJ...852..104R. doi:10.3847/1538-4357/aaa1f2.
  25. ^Linsker, Ralph (March 1988). "Self-organization in a perceptual
      network". IEEE Computer. 21 (3): 105â117. doi:10.1109/2.36.
  26. ^Deco & Obradovic (1996). An_Information-Theoretic_Approach_to_Neural
      Computing. New York, NY: Springer.
  27. ^Plumbley, Mark (1991). "Information theory and unsupervised neural
      networks".
  28. Tech Note
  29. ^Geiger, Bernhard; Kubin, Gernot (January 2013). "Signal Enhancement as
      Minimization of Relevant Information Loss". Proc. ITG Conf. On Systems,
      Communication and Coding. arXiv:1205.6935. Bibcode:2012arXiv1205.6935G.
  30. ^"Engineering_Statistics_Handbook_Section_6.5.5.2". Retrieved 19 January
      2015.
  31. ^ A.A. Miranda, Y.-A. Le Borgne, and G. Bontempi. New_Routes_from_Minimal
      Approximation_Error_to_Principal_Components, Volume 27, Number 3 / June,
      2008, Neural Processing Letters, Springer
  32. ^"SAS/STAT(R)_9.3_User's_Guide".
  33. ^ eig_function Matlab documentation
  34. ^ MATLAB_PCA-based_Face_recognition_software
  35. ^ Eigenvalues_function Mathematica documentation
  36. ^ Roweis, Sam. "EM Algorithms for PCA and SPCA." Advances in Neural
      Information Processing Systems. Ed. Michael I. Jordan, Michael J. Kearns,
      and Sara A. Solla The MIT Press, 1998.
  37. ^Geladi, Paul; Kowalski, Bruce (1986). "Partial Least Squares Regression:
      A Tutorial". Analytica Chimica Acta. 185: 1â17. doi:10.1016/0003-2670
      (86)80028-9.
  38. ^Kramer, R. (1998). Chemometric_Techniques_for_Quantitative_Analysis. New
      York: CRC Press.
  39. ^Andrecut, M. (2009). "Parallel GPU Implementation of Iterative PCA
      Algorithms". Journal of Computational Biology. 16 (11): 1593â1599.
      arXiv:0811.1081. doi:10.1089/cmb.2008.0221. PMID 19772385.
  40. ^Warmuth, M. K.; Kuzmin, D. (2008). "Randomized_online_PCA_algorithms
      with_regret_bounds_that_are_logarithmic_in_the_dimension" (PDF). Journal
      of Machine Learning Research. 9: 2287â2320.
  41. ^ The_Pricing_and_Hedging_of_Interest_Rate_Derivatives:_A_Practical_Guide
      to_Swaps, J H M Darbyshire, 2016,
  42. ISBN 978-0995455511
  43. ^ Giorgia Pasini (2017); Principal_Component_Analysis_for_Stock_Portfolio
      Management. International Journal of Pure and Applied Mathematics. Volume
      115 No. 1 2017, 153-167
  44. ^ Libin Yang. An_Application_of_Principal_Component_Analysis_to_Stock
      Portfolio_Management. Department of Economics and Finance, University_of
      Canterbury, January 2015.
  45. ^Hargreaves, CA; Mani, Chandrika Kadirvel (2015). "The_Selection_of
      Winning_Stocks_Using_Principal_Component_Analysis" (PDF). American
      Journal of Marketing Research. 1 (3): 183â188.
  46. ^ Brenner, N., Bialek, W., & de Ruyter van Steveninck, R.R. (2000).
  47. ^Jirsa, Victor; Friedrich, R; Haken, Herman; Kelso, Scott (1994). "A
      theoretical model of phase transitions in the human brain". Biological
      Cybernetics. 71 (1): 27â35. doi:10.1007/bf00198909. PMID 8054384.
  48. ^BenzÃ©cri, J.-P. (1973). L'Analyse des DonnÃ©es. Volume II. L'Analyse
      des Correspondances. Paris, France: Dunod.
  49. ^Greenacre, Michael (1983). Theory and Applications of Correspondence
      Analysis. London: Academic Press. ISBN 978-0-12-299050-2.
  50. ^Le Roux; Brigitte and Henry Rouanet (2004). Geometric_Data_Analysis,
      From_Correspondence_Analysis_to_Structured_Data_Analysis. Dordrecht:
      Kluwer.
  51. ^ Timothy A. Brown. Confirmatory_Factor_Analysis_for_Applied_Research
      Methodology_in_the_social_sciences. Guilford Press, 2006
  52. ^ I.T. Jolliffe. Principal Component Analysis, Second Edition. Chapter 7.
      2002
  53. ^H. Zha; C. Ding; M. Gu; X. He; H.D. Simon (Dec 2001). "Spectral
      Relaxation_for_K-means_Clustering" (PDF). Neural Information Processing
      Systems Vol.14 (NIPS 2001): 1057â1064.
  54. ^Chris Ding; Xiaofeng He (July 2004). "K-means_Clustering_via_Principal
      Component_Analysis" (PDF). Proc. Of Int'l Conf. Machine Learning (ICML
      2004): 225â232.
  55. ^Drineas, P.; A. Frieze; R. Kannan; S. Vempala; V. Vinay (2004).
      "Clustering_large_graphs_via_the_singular_value_decomposition" (PDF).
      Machine Learning. 56 (1â3): 9â33. doi:10.1023/b:
      mach.0000033113.59016.96. Retrieved 2012-08-02.
  56. ^Cohen, M.; S. Elder; C. Musco; C. Musco; M. Persu (2014).
      "Dimensionality reduction for k-means clustering and low rank
      approximation (Appendix B)". arXiv:1410.6801. Bibcode:
      2014arXiv1410.6801C.
  57. ^ Hui Zou; Trevor Hastie; Robert Tibshirani (2006). "Sparse_principal
      component_analysis" (PDF). Journal_of_Computational_and_Graphical
      Statistics. 15 (2): 262â286. CiteSeerX 10.1.1.62.580. doi:10.1198/
      106186006x113430.
  58. ^ Alexandre dâAspremont; Laurent El Ghaoui; Michael I. Jordan; Gert R.
      G. Lanckriet (2007). "A_Direct_Formulation_for_Sparse_PCA_Using
      Semidefinite_Programming" (PDF). SIAM_Review. 49 (3): 434â448. arXiv:
      cs/0406021. doi:10.1137/050645506.
  59. ^ Michel Journee; Yurii Nesterov; Peter Richtarik; Rodolphe Sepulchre
      (2010). "Generalized_Power_Method_for_Sparse_Principal_Component
      Analysis" (PDF). Journal_of_Machine_Learning_Research. 11: 517â553.
      arXiv:0811.4724. Bibcode:2008arXiv0811.4724J. CORE Discussion Paper 2008/
      70.
  60. ^ Peter Richtarik; Martin Takac; S. Damla Ahipasaoglu (2012).
      "Alternating Maximization: Unifying Framework for 8 Sparse PCA
      Formulations and Efficient Parallel Codes". arXiv:1212.4137 [stat.ML].
  61. ^ Baback Moghaddam; Yair Weiss; Shai Avidan (2005). "Spectral Bounds for
      Sparse PCA: Exact and Greedy Algorithms". Advances_in_Neural_Information
      Processing_Systems (PDF). 18. MIT Press.
  62. ^ Yue Guan; Jennifer Dy (2009). "Sparse_Probabilistic_Principal_Component
      Analysis" (PDF). Journal_of_Machine_Learning_Research_Workshop_and
      Conference_Proceedings. 5: 185.
  63. ^ Hui Zou; Lingzhou Xue (2018). "A Selective Overview of Sparse Principal
      Component Analysis". Proceedings_of_the_IEEE. 106 (8): 1311â1320. doi:
      10.1109/JPROC.2018.2846588.
  64. ^ A._N._Gorban, A. Y. Zinovyev, Principal_Graphs_and_Manifolds, In:
      Handbook of Research on Machine Learning Applications and Trends:
      Algorithms, Methods and Techniques, Olivas E.S. et al Eds. Information
      Science Reference, IGI Global: Hershey, PA, USA, 2009. 28â59.
  65. ^Wang, Y.; Klijn, J. G.; Zhang, Y.; Sieuwerts, A. M.; Look, M. P.; Yang,
      F.; Talantov, D.; Timmermans, M.; Meijer-van Gelder, M. E.; Yu, J.; et
      al. (2005). "Gene expression profiles to predict distant metastasis of
      lymph-node-negative primary breast cancer". The_Lancet. 365 (9460):
      671â679. doi:10.1016/S0140-6736(05)17947-1. PMID 15721472.
  66.  Data_online
  67. ^Zinovyev, A. "ViDaExpert_â_Multidimensional_Data_Visualization_Tool".
      Institut_Curie. Paris.
  68.  (free for non-commercial use)
  69. ^ A.N. Gorban, B. Kegl, D.C. Wunsch, A. Zinovyev (Eds.), Principal
      Manifolds_for_Data_Visualisation_and_Dimension_Reduction, LNCSE 58,
      Springer, Berlin â Heidelberg â New York, 2007.
  70. ISBN 978-3-540-73749-0
  71. ^Lu, Haiping; Plataniotis, K.N.; Venetsanopoulos, A.N. (2011). "A_Survey
      of_Multilinear_Subspace_Learning_for_Tensor_Data" (PDF). Pattern
      Recognition. 44 (7): 1540â1551. doi:10.1016/j.patcog.2011.01.004.
  72. ^Kriegel, H. P.; KrÃ¶ger, P.; Schubert, E.; Zimek, A. (2008). A General
      Framework for Increasing the Robustness of PCA-Based Correlation
      Clustering Algorithms. Scientific and Statistical Database Management.
      Lecture Notes in Computer Science. 5069. pp. 418â435.
      CiteSeerX 10.1.1.144.4864. doi:10.1007/978-3-540-69497-7_27. ISBN 978-3-
      540-69476-2.
  73. ^Markopoulos, Panos P.; Karystinos, George N.; Pados, Dimitris A.
      (October 2014). "Optimal Algorithms for L1-subspace Signal Processing".
      IEEE Transactions on Signal Processing. 62 (19): 5046â5058. arXiv:
      1405.6785. Bibcode:2014ITSP...62.5046M. doi:10.1109/TSP.2014.2338077.
  74. ^Emmanuel J. Candes; Xiaodong Li; Yi Ma; John Wright (2011). "Robust
      Principal Component Analysis?". Journal of the ACM. 58 (3): 11. arXiv:
      0912.3599. doi:10.1145/1970392.1970395.
  75. ^T. Bouwmans; E. Zahzah (2014). "Robust PCA via Principal Component
      Pursuit: A Review for a Comparative Evaluation in Video Surveillance".
      Special Issue on Background Models Challenge, Computer Vision and Image
      Understanding. 122: 22â34. doi:10.1016/j.cviu.2013.11.009.
  76. ^T. Bouwmans; A. Sobral; S. Javed; S. Jung; E. Zahzah (2015).
      "Decomposition into Low-rank plus Additive Matrices for Background/
      Foreground Separation: A Review for a Comparative Evaluation with a
      Large-Scale Dataset". Computer Science Review. 23: 1â71. arXiv:
      1511.01245. doi:10.1016/j.cosrev.2016.11.001.
  77. ^Liao, J. C.; Boscolo, R.; Yang, Y.-L.; Tran, L. M.; Sabatti, C.;
      Roychowdhury, V. P. (2003). "Network_component_analysis:_Reconstruction
      of_regulatory_signals_in_biological_systems" (PDF). Proceedings of the
      National Academy of Sciences. 100 (26): 15522â15527. doi:10.1073/
      pnas.2136632100. Retrieved February 10, 2015.
  78. ^"Principal_Components_Analysis". Institute for Digital Research and
      Education. UCLA. Retrieved 29 May 2018.
***** Further reading[edit] *****
    * Jackson, J.E. (1991). A User's Guide to Principal Components (Wiley).
    * Jolliffe, I. T. (1986). Principal_Component_Analysis. Springer Series in
      Statistics. Springer-Verlag. p. 487. CiteSeerX 10.1.1.149.8828. doi:
      10.1007/b98835. ISBN 978-0-387-95442-4.
Jolliffe, I.T. (2002). Principal Component Analysis, second edition (Springer).
Husson FranÃ§ois, LÃª SÃ©bastien & PagÃ¨s JÃ©rÃ´me (2009). Exploratory
Multivariate Analysis by Example Using R. Chapman & Hall/CRC The R Series,
London. 224p.
ISBN 978-2-7535-0938-2
PagÃ¨s JÃ©rÃ´me (2014). Multiple_Factor_Analysis_by_Example_Using_R. Chapman &
Hall/CRC The R Series London 272 p
***** External links[edit] *****
 Wikimedia Commons has media related to Principal_component_analysis.
    * University_of_Copenhagen_video_by_Rasmus_Bro on YouTube
    * Stanford_University_video_by_Andrew_Ng on YouTube
    * A_Tutorial_on_Principal_Component_Analysis
    * A_layman's_introduction_to_principal_component_analysis on YouTube (a
      video of less than 100 seconds.)
    * StatQuest:_Principal_Component_Analysis_(PCA)_clearly_explained on
      YouTube
    * See also the list of Software_implementations
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
                 * Principal components
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
index.php?title=Principal_component_analysis&oldid=909973214"
Categories:
    * Matrix_decompositions
    * Dimension_reduction
Hidden categories:
    * Wikipedia_articles_needing_page_number_citations_from_June_2011
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_May_2018
    * Articles_with_unsourced_statements_from_August_2014
    * Wikipedia_articles_needing_clarification_from_March_2011
    * Articles_with_unsourced_statements_from_March_2011
    * Commons_category_link_from_Wikidata
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Tagalog
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 8 August 2019, at 20:49 (UTC).
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
