The following text has been accessed from https://en.wikipedia.org/wiki/Correlation_and_dependence at Fri Aug 9 02:27:42 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Correlation and dependence ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about correlation and dependence in statistical data. For other
uses, see correlation_(disambiguation).
Statistical concept
Several sets of (x, y) points, with the Pearson correlation coefficient of x
and y for each set. Note that the correlation reflects the noisiness and
direction of a linear relationship (top row), but not the slope of that
relationship (middle), nor many aspects of nonlinear relationships (bottom).
N.B.: the figure in the center has a slope of 0 but in that case the
correlation coefficient is undefined because the variance of Y is zero.
In statistics, dependence or association is any statistical relationship,
whether causal or not, between two random_variables or bivariate_data. In the
broadest sense correlation is any statistical association, though it commonly
refers to the degree to which a pair of variables are linearly related.
Familiar examples of dependent phenomena include the correlation between the
physical statures of parents and their offspring, and the correlation between
the demand for a limited supply product and its price.[citation_needed]
Correlations are useful because they can indicate a predictive relationship
that can be exploited in practice. For example, an electrical utility may
produce less power on a mild day based on the correlation between electricity
demand and weather. In this example, there is a causal_relationship, because
extreme weather causes people to use more electricity for heating or cooling.
However, in general, the presence of a correlation is not sufficient to infer
the presence of a causal relationship (i.e., correlation_does_not_imply
causation).
Formally, random variables are dependent if they do not satisfy a mathematical
property of probabilistic_independence. In informal parlance, correlation is
synonymous with dependence. However, when used in a technical sense,
correlation refers to any of several specific types of relationship between
mean_values.[clarification_needed] There are several correlation_coefficients,
often denoted     &#x03C1;   {\displaystyle \rho }  [\rho ] or     r
{\displaystyle r}  [r], measuring the degree of correlation. The most common of
these is the Pearson_correlation_coefficient, which is sensitive only to a
linear relationship between two variables (which may be present even when one
variable is a nonlinear function of the other). Other correlation coefficients
have been developed to be more robust than the Pearson correlation â that is,
more sensitive to nonlinear relationships.[1][2][3] Mutual_information can also
be applied to measure dependence between two variables.
⁰
***** Contents *****
    * 1_Pearson's_product-moment_coefficient
          o 1.1_Definition
          o 1.2_Symmetry_property
          o 1.3_Correlation_and_independence
          o 1.4_Sample_correlation_coefficient
    * 2_Example
    * 3_Rank_correlation_coefficients
    * 4_Other_measures_of_dependence_among_random_variables
    * 5_Sensitivity_to_the_data_distribution
    * 6_Correlation_matrices
    * 7_Uncorrelatedness_and_independence_of_stochastic_processes
    * 8_Common_misconceptions
          o 8.1_Correlation_and_causality
          o 8.2_Correlation_and_linearity
    * 9_Bivariate_normal_distribution
    * 10_See_also
    * 11_References
    * 12_Further_reading
    * 13_External_links
***** Pearson's product-moment coefficient[edit] *****
Main article: Pearson_product-moment_correlation_coefficient
**** Definition[edit] ****
The most familiar measure of dependence between two quantities is the Pearson
product-moment_correlation_coefficient, or "Pearson's correlation coefficient",
commonly called simply "the correlation coefficient". It is obtained by
dividing the covariance of the two variables by the product of their standard
deviations. Karl_Pearson developed the coefficient from a similar but slightly
different idea by Francis_Galton.[4]
The population correlation coefficient      &#x03C1;  X , Y     {\displaystyle
\rho _{X,Y}}  [{\displaystyle \rho _{X,Y}}] between two random_variables     X
{\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y] with expected_values
&#x03BC;  X     {\displaystyle \mu _{X}}  [\mu _{X}] and      &#x03BC;  Y
{\displaystyle \mu _{Y}}  [{\displaystyle \mu _{Y}}] and standard_deviations
&#x03C3;  X     {\displaystyle \sigma _{X}}  [\sigma _{X}] and      &#x03C3;  Y
{\displaystyle \sigma _{Y}}  [\sigma_Y] is defined as
    &#x03C1;  X , Y   = corr &#x2061; ( X , Y ) =    cov &#x2061; ( X , Y )
&#x03C3;  X    &#x03C3;  Y      =    E &#x2061; [ ( X &#x2212;  &#x03BC;  X   )
( Y &#x2212;  &#x03BC;  Y   ) ]    &#x03C3;  X    &#x03C3;  Y
{\displaystyle \rho _{X,Y}=\operatorname {corr} (X,Y)={\operatorname {cov}
(X,Y) \over \sigma _{X}\sigma _{Y}}={\operatorname {E} [(X-\mu _{X})(Y-\mu _
{Y})] \over \sigma _{X}\sigma _{Y}}}  [{\displaystyle \rho _{X,Y}=\operatorname
{corr} (X,Y)={\operatorname {cov} (X,Y) \over \sigma _{X}\sigma _{Y}}=
{\operatorname {E} [(X-\mu _{X})(Y-\mu _{Y})] \over \sigma _{X}\sigma _{Y}}}]
where     E   {\displaystyle \operatorname {E} }  [\operatorname {E} ] is the
expected_value operator,     cov   {\displaystyle \operatorname {cov} }
[\operatorname {cov} ] means covariance, and     corr   {\displaystyle
\operatorname {corr} }  [\operatorname {corr}] is a widely used alternative
notation for the correlation coefficient. The Pearson correlation is defined
only if both standard deviations are finite and positive. An alternative
formula purely in terms of moments is
    &#x03C1;  X , Y   =    E &#x2061; ( X Y ) &#x2212; E &#x2061; ( X ) E
&#x2061; ( Y )     E &#x2061; (  X  2   ) &#x2212; E &#x2061; ( X  )  2
&#x22C5;   E &#x2061; (  Y  2   ) &#x2212; E &#x2061; ( Y  )  2
{\displaystyle \rho _{X,Y}={\operatorname {E} (XY)-\operatorname {E}
(X)\operatorname {E} (Y) \over {\sqrt {\operatorname {E} (X^{2})-\operatorname
{E} (X)^{2}}}\cdot {\sqrt {\operatorname {E} (Y^{2})-\operatorname {E} (Y)^
{2}}}}}  [{\displaystyle \rho _{X,Y}={\operatorname {E} (XY)-\operatorname {E}
(X)\operatorname {E} (Y) \over {\sqrt {\operatorname {E} (X^{2})-\operatorname
{E} (X)^{2}}}\cdot {\sqrt {\operatorname {E} (Y^{2})-\operatorname {E} (Y)^
{2}}}}}]
**** Symmetry property[edit] ****
The correlation coefficient is symmetric:     corr &#x2061; ( X , Y ) = corr
&#x2061; ( Y , X )   {\displaystyle \operatorname {corr} (X,Y)=\operatorname
{corr} (Y,X)}  [{\displaystyle \operatorname {corr} (X,Y)=\operatorname {corr}
(Y,X)}]. This is verified by the commutative property of multiplication.
**** Correlation and independence[edit] ****
It is a corollary of the CauchyâSchwarz_inequality that the absolute_value of
the Pearson correlation coefficient is not bigger than 1. The correlation
coefficient is +1 in the case of a perfect direct (increasing) linear
relationship (correlation), â1 in the case of a perfect decreasing (inverse)
linear relationship (anticorrelation),[5] and some value in the open_interval
( &#x2212; 1 , 1 )   {\displaystyle (-1,1)}  [(-1,1)] in all other cases,
indicating the degree of linear_dependence between the variables. As it
approaches zero there is less of a relationship (closer to uncorrelated). The
closer the coefficient is to either â1 or 1, the stronger the correlation
between the variables.
If the variables are independent, Pearson's correlation coefficient is 0, but
the converse is not true because the correlation coefficient detects only
linear dependencies between two variables.
       X , Y  &#xA0;independent      &#x21D2;   &#x03C1;  X , Y   = 0  ( X , Y
&#xA0;uncorrelated  )      &#x03C1;  X , Y   = 0  ( X , Y  &#xA0;uncorrelated
)     &#x21CF;  X , Y  &#xA0;independent        {\displaystyle {\begin
{aligned}X,Y{\text{ independent}}\quad &\Rightarrow \quad \rho _{X,Y}=0\quad
(X,Y{\text{ uncorrelated}})\\\rho _{X,Y}=0\quad (X,Y{\text
{ uncorrelated}})\quad &\nRightarrow \quad X,Y{\text{ independent}}\end
{aligned}}}  [{\displaystyle {\begin{aligned}X,Y{\text{ independent}}\quad
&\Rightarrow \quad \rho _{X,Y}=0\quad (X,Y{\text{ uncorrelated}})\\\rho _
{X,Y}=0\quad (X,Y{\text{ uncorrelated}})\quad &\nRightarrow \quad X,Y{\text
{ independent}}\end{aligned}}}]
For example, suppose the random variable     X   {\displaystyle X}  [X] is
symmetrically distributed about zero, and     Y =  X  2     {\displaystyle Y=X^
{2}}  [{\displaystyle Y=X^{2}}]. Then     Y   {\displaystyle Y}  [Y] is
completely determined by     X   {\displaystyle X}  [X], so that     X
{\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y] are perfectly
dependent, but their correlation is zero; they are uncorrelated. However, in
the special case when     X   {\displaystyle X}  [X] and     Y   {\displaystyle
Y}  [Y] are jointly_normal, uncorrelatedness is equivalent to independence.
**** Sample correlation coefficient[edit] ****
Given a series of     n   {\displaystyle n}  [n] measurements of the pair
(  X  i   ,  Y  i   )   {\displaystyle (X_{i},Y_{i})}  [{\displaystyle (X_
{i},Y_{i})}] indexed by     i = 1 , &#x2026; , n   {\displaystyle i=1,\ldots
,n}  [i=1,\ldots ,n], the sample correlation coefficient can be used to
estimate the population Pearson correlation      &#x03C1;  X , Y
{\displaystyle \rho _{X,Y}}  [{\displaystyle \rho _{X,Y}}] between     X
{\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y]. The sample
correlation coefficient is defined as
          r  x y      =    d e f          &#x2211;  i = 1   n   (  x  i
      &#x2212;    x &#x00AF;    ) (  y  i   &#x2212;    y &#x00AF;    )   ( n
      &#x2212; 1 )  s  x    s  y      =     &#x2211;  i = 1   n   (  x  i
      &#x2212;    x &#x00AF;    ) (  y  i   &#x2212;    y &#x00AF;    )
      &#x2211;  i = 1   n   (  x  i   &#x2212;    x &#x00AF;     )  2
      &#x2211;  i = 1   n   (  y  i   &#x2212;    y &#x00AF;     )  2      ,
      {\displaystyle r_{xy}\quad {\overset {\underset {\mathrm {def} }{}}
      {=}}\quad {\frac {\sum \limits _{i=1}^{n}(x_{i}-{\bar {x}})(y_{i}-{\bar
      {y}})}{(n-1)s_{x}s_{y}}}={\frac {\sum \limits _{i=1}^{n}(x_{i}-{\bar
      {x}})(y_{i}-{\bar {y}})}{\sqrt {\sum \limits _{i=1}^{n}(x_{i}-{\bar
      {x}})^{2}\sum \limits _{i=1}^{n}(y_{i}-{\bar {y}})^{2}}}},}  [
      {\displaystyle r_{xy}\quad {\overset {\underset {\mathrm {def} }{}}
      {=}}\quad {\frac {\sum \limits _{i=1}^{n}(x_{i}-{\bar {x}})(y_{i}-{\bar
      {y}})}{(n-1)s_{x}s_{y}}}={\frac {\sum \limits _{i=1}^{n}(x_{i}-{\bar
      {x}})(y_{i}-{\bar {y}})}{\sqrt {\sum \limits _{i=1}^{n}(x_{i}-{\bar
      {x}})^{2}\sum \limits _{i=1}^{n}(y_{i}-{\bar {y}})^{2}}}},}]
where       x &#x00AF;     {\displaystyle {\overline {x}}}  [{\overline {x}}]
and       y &#x00AF;     {\displaystyle {\overline {y}}}  [{\overline {y}}] are
the sample means of     X   {\displaystyle X}  [X] and     Y   {\displaystyle
Y}  [Y], and      s  x     {\displaystyle s_{x}}  [s_{x}] and      s  y
{\displaystyle s_{y}}  [s_{y}] are the corrected_sample_standard_deviations of
X   {\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y].
Equivalent expressions for      r  x y     {\displaystyle r_{xy}}  [r_{xy}] are
              r  x y      =    &#x2211;  x  i    y  i   &#x2212; n    x
      &#x00AF;       y &#x00AF;      n  s  x  &#x2032;   s  y  &#x2032;
      =    n &#x2211;  x  i    y  i   &#x2212; &#x2211;  x  i   &#x2211;  y  i
      n &#x2211;  x  i   2   &#x2212; ( &#x2211;  x  i    )  2     &#xA0;   n
      &#x2211;  y  i   2   &#x2212; ( &#x2211;  y  i    )  2        .
      {\displaystyle {\begin{aligned}r_{xy}&={\frac {\sum x_{i}y_{i}-n{\bar
      {x}}{\bar {y}}}{ns'_{x}s'_{y}}}\\[5pt]&={\frac {n\sum x_{i}y_{i}-\sum x_
      {i}\sum y_{i}}{{\sqrt {n\sum x_{i}^{2}-(\sum x_{i})^{2}}}~{\sqrt {n\sum
      y_{i}^{2}-(\sum y_{i})^{2}}}}}.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}r_{xy}&={\frac {\sum x_{i}y_{i}-n{\bar {x}}{\bar {y}}}{ns'_
      {x}s'_{y}}}\\[5pt]&={\frac {n\sum x_{i}y_{i}-\sum x_{i}\sum y_{i}}{{\sqrt
      {n\sum x_{i}^{2}-(\sum x_{i})^{2}}}~{\sqrt {n\sum y_{i}^{2}-(\sum y_{i})^
      {2}}}}}.\end{aligned}}}]
where      s  x  &#x2032;    {\displaystyle s'_{x}}  [{\displaystyle s'_{x}}]
and      s  y  &#x2032;    {\displaystyle s'_{y}}  [{\displaystyle s'_{y}}] are
the uncorrected_sample_standard_deviations of     X   {\displaystyle X}  [X]
and     Y   {\displaystyle Y}  [Y].
If     x   {\displaystyle x}  [x] and     y   {\displaystyle y}  [y] are
results of measurements that contain measurement error, the realistic limits on
the correlation coefficient are not â1 to +1 but a smaller range.[6] For the
case of a linear model with a single independent variable, the coefficient_of
determination_(R_squared) is the square of      r  x y     {\displaystyle r_
{xy}}  [r_{xy}], Pearson's product-moment coefficient.
***** Example[edit] *****
Consider the joint probability distribution of     X   {\displaystyle X}  [X]
and     Y   {\displaystyle Y}  [Y] given in the table below.
   P &#x2061; ( X =
x , Y = y )
{\displaystyle         y = &#x2212; 1      y = 0               y = 1
\operatorname {P}   {\displaystyle y=-  {\displaystyle y=0} {\displaystyle y=1}
(X=x,Y=y)}  [       1}  [y=-1]          [y=0]               [y=1]
{\displaystyle
\operatorname {P}
(X=x,Y=y)}]
   x = 0               0                   1  /  3             0
{\displaystyle x=0} {\displaystyle 0}   {\displaystyle 1/3} {\displaystyle 0}
[x=0]               [{\displaystyle 0}] [1/3]               [{\displaystyle 0}]
   x = 1               1  /  3             0                   1  /  3
{\displaystyle x=1} {\displaystyle 1/3} {\displaystyle 0}   {\displaystyle 1/3}
[x=1]               [1/3]               [{\displaystyle 0}] [1/3]
For this joint distribution, the marginal distributions are:
         P &#x2061; ( X = x ) =   {    1  /  3     for&#xA0;  x = 0     2  /  3
      for&#xA0;  x = 1         {\displaystyle \operatorname {P} (X=x)={\begin
      {cases}1/3&\quad {\text{for }}x=0\\2/3&\quad {\text{for }}x=1\end
      {cases}}}  [{\displaystyle \operatorname {P} (X=x)={\begin{cases}1/
      3&\quad {\text{for }}x=0\\2/3&\quad {\text{for }}x=1\end{cases}}}]
         P &#x2061; ( Y = y ) =   {    1  /  3     for&#xA0;  y = &#x2212; 1
      1  /  3     for&#xA0;  y = 0     1  /  3     for&#xA0;  y = 1
      {\displaystyle \operatorname {P} (Y=y)={\begin{cases}1/3&\quad {\text{for
      }}y=-1\\1/3&\quad {\text{for }}y=0\\1/3&\quad {\text{for }}y=1\end
      {cases}}}  [{\displaystyle \operatorname {P} (Y=y)={\begin{cases}1/
      3&\quad {\text{for }}y=-1\\1/3&\quad {\text{for }}y=0\\1/3&\quad {\text
      {for }}y=1\end{cases}}}]
This yields the following expectations and variances:
          &#x03BC;  X   = 2  /  3   {\displaystyle \mu _{X}=2/3}  [
      {\displaystyle \mu _{X}=2/3}]
          &#x03BC;  Y   = 0   {\displaystyle \mu _{Y}=0}  [{\displaystyle \mu _
      {Y}=0}]
          &#x03C3;  X   2   = 2  /  9   {\displaystyle \sigma _{X}^{2}=2/9}  [
      {\displaystyle \sigma _{X}^{2}=2/9}]
          &#x03C3;  Y   2   = 2  /  3   {\displaystyle \sigma _{Y}^{2}=2/3}  [
      {\displaystyle \sigma _{Y}^{2}=2/3}]
Therefore:
              &#x03C1;  X , Y      =   1   &#x03C3;  X    &#x03C3;  Y      E
      &#x2061; [ ( X &#x2212;  &#x03BC;  X   ) ( Y &#x2212;  &#x03BC;  Y   ) ]
      =   1   &#x03C3;  X    &#x03C3;  Y       &#x2211;  x , y    ( x &#x2212;
      &#x03BC;  X   ) ( y &#x2212;  &#x03BC;  Y   ) P &#x2061; ( X = x , Y = y
      )        = ( 1 &#x2212; 2  /  3 ) ( &#x2212; 1 &#x2212; 0 )   1 3   + ( 0
      &#x2212; 2  /  3 ) ( 0 &#x2212; 0 )   1 3   + ( 1 &#x2212; 2  /  3 ) ( 1
      &#x2212; 0 )   1 3   = 0.       {\displaystyle {\begin{aligned}\rho _
      {X,Y}&={\frac {1}{\sigma _{X}\sigma _{Y}}}\operatorname {E} [(X-\mu _{X})
      (Y-\mu _{Y})]\\[5pt]&={\frac {1}{\sigma _{X}\sigma _{Y}}}\sum _{x,y}{(x-
      \mu _{X})(y-\mu _{Y})\operatorname {P} (X=x,Y=y)}\\[5pt]&=(1-2/3)(-1-0)
      {\frac {1}{3}}+(0-2/3)(0-0){\frac {1}{3}}+(1-2/3)(1-0){\frac {1}
      {3}}=0.\end{aligned}}}  [{\displaystyle {\begin{aligned}\rho _{X,Y}&=
      {\frac {1}{\sigma _{X}\sigma _{Y}}}\operatorname {E} [(X-\mu _{X})(Y-\mu
      _{Y})]\\[5pt]&={\frac {1}{\sigma _{X}\sigma _{Y}}}\sum _{x,y}{(x-\mu _
      {X})(y-\mu _{Y})\operatorname {P} (X=x,Y=y)}\\[5pt]&=(1-2/3)(-1-0){\frac
      {1}{3}}+(0-2/3)(0-0){\frac {1}{3}}+(1-2/3)(1-0){\frac {1}{3}}=0.\end
      {aligned}}}]
***** Rank correlation coefficients[edit] *****
Main articles: Spearman's_rank_correlation_coefficient and Kendall_tau_rank
correlation_coefficient
Rank_correlation coefficients, such as Spearman's_rank_correlation_coefficient
and Kendall's_rank_correlation_coefficient_(Ï) measure the extent to which, as
one variable increases, the other variable tends to increase, without requiring
that increase to be represented by a linear relationship. If, as the one
variable increases, the other decreases, the rank correlation coefficients will
be negative. It is common to regard these rank correlation coefficients as
alternatives to Pearson's coefficient, used either to reduce the amount of
calculation or to make the coefficient less sensitive to non-normality in
distributions. However, this view has little mathematical basis, as rank
correlation coefficients measure a different type of relationship than the
Pearson_product-moment_correlation_coefficient, and are best seen as measures
of a different type of association, rather than as alternative measure of the
population correlation coefficient.[7][8]
To illustrate the nature of rank correlation, and its difference from linear
correlation, consider the following four pairs of numbers     ( x , y )
{\displaystyle (x,y)}  [(x,y)]:
      (0, 1), (10, 100), (101, 500), (102, 2000).
As we go from each pair to the next pair     x   {\displaystyle x}  [x]
increases, and so does     y   {\displaystyle y}  [y]. This relationship is
perfect, in the sense that an increase in     x   {\displaystyle x}  [x] is
always accompanied by an increase in     y   {\displaystyle y}  [y]. This means
that we have a perfect rank correlation, and both Spearman's and Kendall's
correlation coefficients are 1, whereas in this example Pearson product-moment
correlation coefficient is 0.7544, indicating that the points are far from
lying on a straight line. In the same way if     y   {\displaystyle y}  [y]
always decreases when     x   {\displaystyle x}  [x] increases, the rank
correlation coefficients will be â1, while the Pearson product-moment
correlation coefficient may or may not be close to â1, depending on how close
the points are to a straight line. Although in the extreme cases of perfect
rank correlation the two coefficients are both equal (being both +1 or both
â1), this is not generally the case, and so values of the two coefficients
cannot meaningfully be compared.[7] For example, for the three pairs (1, 1)
(2, 3) (3, 2) Spearman's coefficient is 1/2, while Kendall's coefficient is 1/
3.
***** Other measures of dependence among random variables[edit] *****
See also: Pearson_product-moment_correlation_coefficient_Â§ Variants
The information given by a correlation coefficient is not enough to define the
dependence structure between random variables.[9] The correlation coefficient
completely defines the dependence structure only in very particular cases, for
example when the distribution is a multivariate_normal_distribution. (See
diagram above.) In the case of elliptical_distributions it characterizes the
(hyper-)ellipses of equal density; however, it does not completely characterize
the dependence structure (for example, a multivariate_t-distribution's degrees
of freedom determine the level of tail dependence).
Distance_correlation[10][11] was introduced to address the deficiency of
Pearson's correlation that it can be zero for dependent random variables; zero
distance correlation implies independence.
The Randomized Dependence Coefficient[12] is a computationally efficient,
copula-based measure of dependence between multivariate random variables. RDC
is invariant with respect to non-linear scalings of random variables, is
capable of discovering a wide range of functional association patterns and
takes value zero at independence.
For two binary variables, the odds_ratio measures their dependence, and takes
range non-negative numbers, possibly infinity:     [ 0 , + &#x221E; ]
{\displaystyle [0,+\infty ]}  [{\displaystyle [0,+\infty ]}]. Related
statistics such as Yule's_Y and Yule's_Q normalize this to the correlation-like
range     [ &#x2212; 1 , 1 ]   {\displaystyle [-1,1]}  [[-1, 1]]. The odds
ratio is generalized by the logistic_model to model cases where the dependent
variables are discrete and there may be one or more independent variables.
The correlation_ratio, entropy-based mutual_information, total_correlation,
dual_total_correlation and polychoric_correlation are all also capable of
detecting more general dependencies, as is consideration of the copula between
them, while the coefficient_of_determination generalizes the correlation
coefficient to multiple_regression.
***** Sensitivity to the data distribution[edit] *****
Further information: Pearson_product-moment_correlation_coefficient
Â§ Sensitivity_to_the_data_distribution
The degree of dependence between variables     X   {\displaystyle X}  [X] and
Y   {\displaystyle Y}  [Y] does not depend on the scale on which the variables
are expressed. That is, if we are analyzing the relationship between     X
{\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y], most correlation
measures are unaffected by transforming     X   {\displaystyle X}  [X] to
a + bX and     Y   {\displaystyle Y}  [Y] to c + dY, where a, b, c, and d are
constants (b and d being positive). This is true of some correlation statistics
as well as their population analogues. Some correlation statistics, such as the
rank correlation coefficient, are also invariant to monotone_transformations of
the marginal distributions of     X   {\displaystyle X}  [X] and/or     Y
{\displaystyle Y}  [Y].
Pearson/Spearman correlation coefficients between     X   {\displaystyle X}
[X] and     Y   {\displaystyle Y}  [Y] are shown when the two variables' ranges
are unrestricted, and when the range of     X   {\displaystyle X}  [X] is
restricted to the interval (0,1).
Most correlation measures are sensitive to the manner in which     X
{\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y] are sampled.
Dependencies tend to be stronger if viewed over a wider range of values. Thus,
if we consider the correlation coefficient between the heights of fathers and
their sons over all adult males, and compare it to the same correlation
coefficient calculated when the fathers are selected to be between 165 cm and
170 cm in height, the correlation will be weaker in the latter case. Several
techniques have been developed that attempt to correct for range restriction in
one or both variables, and are commonly used in meta-analysis; the most common
are Thorndike's case II and case III equations.[13]
Various correlation measures in use may be undefined for certain joint
distributions of X and Y. For example, the Pearson correlation coefficient is
defined in terms of moments, and hence will be undefined if the moments are
undefined. Measures of dependence based on quantiles are always defined.
Sample-based statistics intended to estimate population measures of dependence
may or may not have desirable statistical properties such as being unbiased, or
asymptotically_consistent, based on the spatial structure of the population
from which the data were sampled.
Sensitivity to the data distribution can be used to an advantage. For example,
scaled_correlation is designed to use the sensitivity to the range in order to
pick out correlations between fast components of time series.[14] By reducing
the range of values in a controlled manner, the correlations on long time scale
are filtered out and only the correlations on short time scales are revealed.
***** Correlation matrices[edit] *****
See also: Covariance_matrix_Â§ Correlation_matrix
The correlation matrix of     n   {\displaystyle n}  [n] random variables
X  1   , &#x2026; ,  X  n     {\displaystyle X_{1},\ldots ,X_{n}}  [X_
{1},\ldots ,X_{n}] is the     n &#x00D7; n   {\displaystyle n\times n}
[n\times n] matrix whose     ( i , j )   {\displaystyle (i,j)}  [(i,j)] entry
is     corr &#x2061; (  X  i   ,  X  j   )   {\displaystyle \operatorname
{corr} (X_{i},X_{j})}  [{\displaystyle \operatorname {corr} (X_{i},X_{j})}]. If
the measures of correlation used are product-moment coefficients, the
correlation matrix is the same as the covariance_matrix of the standardized
random_variables      X  i    /  &#x03C3; (  X  i   )   {\displaystyle X_{i}/
\sigma (X_{i})}  [{\displaystyle X_{i}/\sigma (X_{i})}] for     i = 1 ,
&#x2026; , n   {\displaystyle i=1,\dots ,n}  [i=1,\dots ,n]. This applies both
to the matrix of population correlations (in which case     &#x03C3;
{\displaystyle \sigma }  [\sigma ] is the population standard deviation), and
to the matrix of sample correlations (in which case     &#x03C3;
{\displaystyle \sigma }  [\sigma ] denotes the sample standard deviation).
Consequently, each is necessarily a positive-semidefinite_matrix. Moreover, the
correlation matrix is strictly positive_definite if no variable can have all
its values exactly generated as a linear function of the values of the others.
The correlation matrix is symmetric because the correlation between      X  i
{\displaystyle X_{i}}  [X_{i}] and      X  j     {\displaystyle X_{j}}  [X_{j}]
is the same as the correlation between      X  j     {\displaystyle X_{j}}  [X_
{j}] and      X  i     {\displaystyle X_{i}}  [X_{i}].
A correlation matrix appears, for example, in one formula for the coefficient
of_multiple_determination, a measure of goodness of fit in multiple_regression.
In statistical_modelling, correlation matrices representing the relationships
between variables are categorized into different correlation structures, which
are distinguished by factors such as the number of parameters required to
estimate them. For example, in an exchangeable correlation matrix, all pairs of
variables are modelled as having the same correlation, so all non-diagonal
elements of the matrix are equal to each other. On the other hand, an
autoregressive matrix is often used when variables represent a time series,
since correlations are likely to be greater when measurements are closer in
time. Other examples include independent, unstructured, M-dependent, and
Toeplitz.
***** Uncorrelatedness and independence of stochastic processes[edit] *****
Similarly for two stochastic processes       {  X  t   }   t &#x2208;   T
{\displaystyle \left\{X_{t}\right\}_{t\in {\mathcal {T}}}}  [{\displaystyle
\left\{X_{t}\right\}_{t\in {\mathcal {T}}}}] and       {  Y  t   }   t &#x2208;
T       {\displaystyle \left\{Y_{t}\right\}_{t\in {\mathcal {T}}}}  [
{\displaystyle \left\{Y_{t}\right\}_{t\in {\mathcal {T}}}}]: If they are
independent, then they are uncorrelated.[15]:p. 151
***** Common misconceptions[edit] *****
**** Correlation and causality[edit] ****
Main article: Correlation_does_not_imply_causation
See also: Normally_distributed_and_uncorrelated_does_not_imply_independent
The conventional dictum that "correlation_does_not_imply_causation" means that
correlation cannot be used to infer a causal relationship between the
variables.[16] This dictum should not be taken to mean that correlations cannot
indicate the potential existence of causal relations. However, the causes
underlying the correlation, if any, may be indirect and unknown, and high
correlations also overlap with identity relations (tautologies), where no
causal process exists. Consequently, a correlation between two variables is not
a sufficient condition to establish a causal relationship (in either
direction).
A correlation between age and height in children is fairly causally
transparent, but a correlation between mood and health in people is less so.
Does improved mood lead to improved health, or does good health lead to good
mood, or both? Or does some other factor underlie both? In other words, a
correlation can be taken as evidence for a possible causal relationship, but
cannot indicate what the causal relationship, if any, might be.
**** Correlation and linearity[edit] ****
Four sets of data with the same correlation of 0.816
The Pearson correlation coefficient indicates the strength of a linear
relationship between two variables, but its value generally does not completely
characterize their relationship.[17] In particular, if the conditional_mean of
Y   {\displaystyle Y}  [Y] given     X   {\displaystyle X}  [X], denoted     E
&#x2061; ( Y &#x2223; X )   {\displaystyle \operatorname {E} (Y\mid X)}  [
{\displaystyle \operatorname {E} (Y\mid X)}], is not linear in     X
{\displaystyle X}  [X], the correlation coefficient will not fully determine
the form of     E &#x2061; ( Y &#x2223; X )   {\displaystyle \operatorname {E}
(Y\mid X)}  [{\displaystyle \operatorname {E} (Y\mid X)}].
The adjacent image shows scatter_plots of Anscombe's_quartet, a set of four
different pairs of variables created by Francis_Anscombe.[18] The four     y
{\displaystyle y}  [y] variables have the same mean (7.5), variance (4.12),
correlation (0.816) and regression line (y = 3 + 0.5x). However, as can be seen
on the plots, the distribution of the variables is very different. The first
one (top left) seems to be distributed normally, and corresponds to what one
would expect when considering two variables correlated and following the
assumption of normality. The second one (top right) is not distributed
normally; while an obvious relationship between the two variables can be
observed, it is not linear. In this case the Pearson correlation coefficient
does not indicate that there is an exact functional relationship: only the
extent to which that relationship can be approximated by a linear relationship.
In the third case (bottom left), the linear relationship is perfect, except for
one outlier which exerts enough influence to lower the correlation coefficient
from 1 to 0.816. Finally, the fourth example (bottom right) shows another
example when one outlier is enough to produce a high correlation coefficient,
even though the relationship between the two variables is not linear.
These examples indicate that the correlation coefficient, as a summary
statistic, cannot replace visual examination of the data. Note that the
examples are sometimes said to demonstrate that the Pearson correlation assumes
that the data follow a normal_distribution, but this is not correct.[4]
***** Bivariate normal distribution[edit] *****
If a pair     ( X , Y )   {\displaystyle (X,Y)}  [(X,Y)] of random variables
follows a bivariate_normal_distribution, the conditional mean     E &#x2061;
( X &#x2223; Y )   {\displaystyle \operatorname {E} (X\mid Y)}  [\operatorname
{E}(X\mid Y)] is a linear function of     Y   {\displaystyle Y}  [Y], and the
conditional mean     E &#x2061; ( Y &#x2223; X )   {\displaystyle \operatorname
{E} (Y\mid X)}  [{\displaystyle \operatorname {E} (Y\mid X)}] is a linear
function of     X   {\displaystyle X}  [X]. The correlation coefficient
&#x03C1;  X , Y     {\displaystyle \rho _{X,Y}}  [{\displaystyle \rho _{X,Y}}]
between     X   {\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y],
along with the marginal means and variances of     X   {\displaystyle X}  [X]
and     Y   {\displaystyle Y}  [Y], determines this linear relationship:
         E &#x2061; ( Y &#x2223; X ) = E &#x2061; ( Y ) +  &#x03C1;  X , Y
      &#x22C5;  &#x03C3;  Y      X &#x2212; E &#x2061; ( X )   &#x03C3;  X
      ,   {\displaystyle \operatorname {E} (Y\mid X)=\operatorname {E} (Y)+\rho
      _{X,Y}\cdot \sigma _{Y}{\frac {X-\operatorname {E} (X)}{\sigma _{X}}},}
      [{\displaystyle \operatorname {E} (Y\mid X)=\operatorname {E} (Y)+\rho _
      {X,Y}\cdot \sigma _{Y}{\frac {X-\operatorname {E} (X)}{\sigma _{X}}},}]
where     E &#x2061; ( X )   {\displaystyle \operatorname {E} (X)}
[\operatorname {E}(X)] and     E &#x2061; ( Y )   {\displaystyle \operatorname
{E} (Y)}  [{\displaystyle \operatorname {E} (Y)}] are the expected values of
X   {\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y], respectively,
and      &#x03C3;  X     {\displaystyle \sigma _{X}}  [\sigma _{X}] and
&#x03C3;  Y     {\displaystyle \sigma _{Y}}  [\sigma_Y] are the standard
deviations of     X   {\displaystyle X}  [X] and     Y   {\displaystyle Y}
[Y], respectively.
***** See also[edit] *****
    * [icon]Statistics_portal
Further information: Correlation_(disambiguation)
    * Autocorrelation
    * Canonical_correlation
    * Coefficient_of_determination
    * Cointegration
    * Concordance_correlation_coefficient
    * Cophenetic_correlation
    * Copula
    * Correlation_function
    * Correlation_gap
    * Covariance
    * Covariance_and_correlation
    * Cross-correlation
    * Ecological_correlation
    * Fraction_of_variance_unexplained
    * Genetic_correlation
    * Goodman_and_Kruskal's_lambda
    * Illusory_correlation
    * Interclass_correlation
    * Intraclass_correlation
    * Lift_(data_mining)
    * Mean_dependence
    * Modifiable_areal_unit_problem
    * Multiple_correlation
    * Point-biserial_correlation_coefficient
    * Quadrant_count_ratio
    * Spurious_correlation
    * Statistical_arbitrage
    * Subindependence
***** References[edit] *****
   1. ^ Croxton, Frederick Emory; Cowden, Dudley Johnstone; Klein, Sidney
      (1968) Applied General Statistics, Pitman.
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
   3. ISBN 9780273403159 (page 625)
   4. ^ Dietrich, Cornelius Frank (1991) Uncertainty, Calibration and
      Probability: The Statistics of Scientific and Industrial Measurement 2nd
      Edition, A. Higler.
   5. ISBN 9780750300605 (Page 331)
   6. ^ Aitken, Alexander Craig (1957) Statistical Mathematics 8th Edition.
      Oliver & Boyd.
   7. ISBN 9780050013007 (Page 95)
   8. ^ a bRodgers, J. L.; Nicewander, W. A. (1988). "Thirteen ways to look at
      the correlation coefficient". The American Statistician. 42 (1): 59â66.
      doi:10.1080/00031305.1988.10475524. JSTOR 2685263.
   9. ^ Dowdy, S. and Wearden, S. (1983). "Statistics for Research", Wiley.
  10. ISBN 0-471-08602-9 pp 230
  11. ^Francis, DP; Coats AJ; Gibson D (1999). "How high can a correlation
      coefficient be?". Int J Cardiol. 69 (2): 185â199. doi:10.1016/S0167-
      5273(99)00028-5.
  12. ^ a b Yule, G.U and Kendall, M.G. (1950), "An Introduction to the Theory
      of Statistics", 14th Edition (5th Impression 1968). Charles Griffin & Co.
      pp 258â270
  13. ^ Kendall, M. G. (1955) "Rank Correlation Methods", Charles Griffin & Co.
  14. ^Mahdavi Damghani B. (2013). "The Non-Misleading Value of Inferred
      Correlation: An Introduction to the Cointelation Model". Wilmott
      Magazine. 2013 (67): 50â61. doi:10.1002/wilm.10252.
  15. ^SzÃ©kely, G. J. Rizzo; Bakirov, N. K. (2007). "Measuring and testing
      independence by correlation of distances". Annals_of_Statistics. 35 (6):
      2769â2794. arXiv:0803.4101. doi:10.1214/009053607000000505.
  16. ^SzÃ©kely, G. J.; Rizzo, M. L. (2009). "Brownian_distance_covariance".
      Annals of Applied Statistics. 3 (4): 1233â1303. arXiv:1010.0297. doi:
      10.1214/09-AOAS312. PMC 2889501. PMID 20574547.
  17. ^ Lopez-Paz D. and Hennig P. and SchÃ¶lkopf B. (2013). "The Randomized
      Dependence Coefficient", "Conference_on_Neural_Information_Processing
      Systems" Reprint
  18. ^Thorndike, Robert Ladd (1947). Research problems and techniques (Report
      No. 3). Washington DC: US Govt. print. off.
  19. ^NikoliÄ, D; Muresan, RC; Feng, W; Singer, W (2012). "Scaled correlation
      analysis: a better way to compute a cross-correlogram". European Journal
      of Neuroscience. 35 (5): 1â21. doi:10.1111/j.1460-9568.2011.07987.x.
      PMID 22324876.
  20. ^Park, Kun Il (2018). Fundamentals of Probability and Stochastic
      Processes with Applications to Communications. Springer. ISBN 978-3-319-
      68074-3.
  21. ^Aldrich, John (1995). "Correlations Genuine and Spurious in Pearson and
      Yule". Statistical Science. 10 (4): 364â376. doi:10.1214/ss/1177009870.
      JSTOR 2246135.
  22. ^Mahdavi Damghani, Babak (2012). "The Misleading Value of Measured
      Correlation". Wilmott. 2012 (1): 64â73. doi:10.1002/wilm.10167.
  23. ^Anscombe, Francis J. (1973). "Graphs in statistical analysis". The
      American Statistician. 27 (1): 17â21. doi:10.2307/2682899.
      JSTOR 2682899.
***** Further reading[edit] *****
    * Cohen, J.; Cohen P.; West, S.G. & Aiken, L.S. (2002). Applied multiple
      regression/correlation analysis for the behavioral sciences (3rd ed.).
      Psychology Press. ISBN 978-0-8058-2223-6.
Hazewinkel,_Michiel, ed. (2001) [1994], "Correlation_(in_statistics)",
Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. / Kluwer
Academic Publishers, ISBN 978-1-55608-010-4
Oestreicher, J. & D. R. (February 26, 2015). Plague of Equals: A science
thriller of international disease, politics and drug discovery. California:
Omega Cat Press. p. 408. ISBN 978-0963175540.
***** External links[edit] *****
 Look up correlation or dependence in Wiktionary, the free dictionary.
 Wikimedia Commons has media related to Correlation.
 Wikiversity has learning resources about Correlation
    * MathWorld_page_on_the_(cross-)correlation_coefficient/s_of_a_sample
    * Compute_significance_between_two_correlations, for the comparison of two
      correlation values.
    * A_MATLAB_Toolbox_for_computing_Weighted_Correlation_Coefficients
    * [1] Proof-that-the-Sample-Bivariate-Correlation-has-limits-plus-or-minus-
      1
    * Interactive_Flash_simulation_on_the_correlation_of_two_normally
      distributed_variables by Juha Puranen.
    * Correlation_analysis._Biomedical_Statistics
    * R-Psychologist Correlation visualization of correlation between two
      numeric variables
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
index.php?title=Correlation_and_dependence&oldid=908745097"
Categories:
    * Covariance_and_correlation
    * Dimensionless_numbers
Hidden categories:
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_July_2019
    * Wikipedia_articles_needing_clarification_from_August_2018
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Jawa
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Basa_Sunda
    * Suomi
    * Svenska
    * Tagalog
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 31 July 2019, at 18:09 (UTC).
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
