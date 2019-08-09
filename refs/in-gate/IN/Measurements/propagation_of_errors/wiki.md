The following text has been accessed from https://en.wikipedia.org/wiki/Propagation_of_uncertainty at Fri Aug 9 01:26:05 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Propagation of uncertainty ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For the propagation of uncertainty through time, see Chaos_theory
Â§ Sensitivity_to_initial_conditions.
In statistics, propagation of uncertainty (or propagation of error) is the
effect of variables' uncertainties (or errors, more specifically random_errors)
on the uncertainty of a function based on them. When the variables are the
values of experimental measurements they have uncertainties_due_to_measurement
limitations (e.g., instrument precision) which propagate due to the combination
of variables in the function.
The uncertainty u can be expressed in a number of ways. It may be defined by
the absolute_error Îx. Uncertainties can also be defined by the relative_error
(Îx)/x, which is usually written as a percentage. Most commonly, the
uncertainty on a quantity is quantified in terms of the standard_deviation, Ï,
the positive square root of variance, Ï2. The value of a quantity and its
error are then expressed as an interval x Â± u. If the statistical probability
distribution of the variable is known or can be assumed, it is possible to
derive confidence_limits to describe the region within which the true value of
the variable may be found. For example, the 68% confidence limits for a one-
dimensional variable belonging to a normal_distribution are approximately Â±
one standard deviation Ï from the central value x, which means that the region
x Â± Ï will cover the true value in roughly 68% of cases.
If the uncertainties are correlated then covariance must be taken into account.
Correlation can arise from two different sources. First, the measurement errors
may be correlated. Second, when the underlying values are correlated across a
population, the uncertainties in the group averages will be correlated.[1]
⁰
***** Contents *****
    * 1_Linear_combinations
    * 2_Non-linear_combinations
          o 2.1_Simplification
          o 2.2_Example
          o 2.3_Caveats_and_warnings
                # 2.3.1_Reciprocal
                # 2.3.2_Shifted_reciprocal
    * 3_Example_formulae
    * 4_Example_calculations
          o 4.1_Inverse_tangent_function
          o 4.2_Resistance_measurement
    * 5_See_also
    * 6_References
    * 7_Further_reading
    * 8_External_links
***** Linear combinations[edit] *****
Let     {  f  k   (  x  1   ,  x  2   , &#x2026; ,  x  n   ) }   {\displaystyle
\{f_{k}(x_{1},x_{2},\dots ,x_{n})\}}  [\{f_{k}(x_{1},x_{2},\dots ,x_{n})\}] be
a set of m functions which are linear combinations of     n   {\displaystyle n}
[n] variables      x  1   ,  x  2   , &#x2026; ,  x  n     {\displaystyle x_
{1},x_{2},\dots ,x_{n}}  [x_{1},x_{2},\dots ,x_{n}] with combination
coefficients      A  k 1   ,  A  k 2   , &#x2026; ,  A  k n   , ( k = 1 ,
&#x2026; , m )   {\displaystyle A_{k1},A_{k2},\dots ,A_{kn},(k=1,\dots ,m)}  [
{\displaystyle A_{k1},A_{k2},\dots ,A_{kn},(k=1,\dots ,m)}]:
          f  k   =  &#x2211;  i = 1   n    A  k i    x  i    &#xA0;or&#xA0;   f
      =  A x  &#xA0; .   {\displaystyle f_{k}=\sum _{i=1}^{n}A_{ki}x_{i}{\text
      { or }}\mathrm {f} =\mathrm {Ax} \ .}  [{\displaystyle f_{k}=\sum _{i=1}^
      {n}A_{ki}x_{i}{\text{ or }}\mathrm {f} =\mathrm {Ax} \ .}]
Also let the variance-covariance_matrix of x = (x1, ..., xn) be denoted by
&#x03A3;  x      {\displaystyle \Sigma ^{x}\,}  [{\displaystyle \Sigma ^
{x}\,}].
          &#x03A3;  x   =   (     &#x03C3;  1   2      &#x03C3;  12
      &#x03C3;  13     &#x22EF;      &#x03C3;  12      &#x03C3;  2   2
      &#x03C3;  23     &#x22EF;      &#x03C3;  13      &#x03C3;  23
      &#x03C3;  3   2     &#x22EF;     &#x22EE;   &#x22EE;   &#x22EE;
      &#x22F1;    )   =   (      &#x03A3;   11   x       &#x03A3;   12   x
      &#x03A3;   13   x     &#x22EF;       &#x03A3;   12   x       &#x03A3;
      22   x       &#x03A3;   23   x     &#x22EF;       &#x03A3;   13   x
      &#x03A3;   23   x       &#x03A3;   33   x     &#x22EF;     &#x22EE;
      &#x22EE;   &#x22EE;   &#x22F1;    )     {\displaystyle \Sigma ^{x}=
      {\begin{pmatrix}\sigma _{1}^{2}&\sigma _{12}&\sigma _{13}&\cdots \\\sigma
      _{12}&\sigma _{2}^{2}&\sigma _{23}&\cdots \\\sigma _{13}&\sigma _
      {23}&\sigma _{3}^{2}&\cdots \\\vdots &\vdots &\vdots &\ddots \end
      {pmatrix}}={\begin{pmatrix}{\Sigma }_{11}^{x}&{\Sigma }_{12}^{x}&{\Sigma
      }_{13}^{x}&\cdots \\{\Sigma }_{12}^{x}&{\Sigma }_{22}^{x}&{\Sigma }_{23}^
      {x}&\cdots \\{\Sigma }_{13}^{x}&{\Sigma }_{23}^{x}&{\Sigma }_{33}^
      {x}&\cdots \\\vdots &\vdots &\vdots &\ddots \end{pmatrix}}}  [
      {\displaystyle \Sigma ^{x}={\begin{pmatrix}\sigma _{1}^{2}&\sigma _
      {12}&\sigma _{13}&\cdots \\\sigma _{12}&\sigma _{2}^{2}&\sigma _
      {23}&\cdots \\\sigma _{13}&\sigma _{23}&\sigma _{3}^{2}&\cdots \\\vdots
      &\vdots &\vdots &\ddots \end{pmatrix}}={\begin{pmatrix}{\Sigma }_{11}^
      {x}&{\Sigma }_{12}^{x}&{\Sigma }_{13}^{x}&\cdots \\{\Sigma }_{12}^{x}&
      {\Sigma }_{22}^{x}&{\Sigma }_{23}^{x}&\cdots \\{\Sigma }_{13}^{x}&{\Sigma
      }_{23}^{x}&{\Sigma }_{33}^{x}&\cdots \\\vdots &\vdots &\vdots &\ddots
      \end{pmatrix}}}]
Then, the variance-covariance matrix      &#x03A3;  f      {\displaystyle
\Sigma ^{f}\,}  [{\displaystyle \Sigma ^{f}\,}] of f is given by
           &#x03A3;   i j   f   =  &#x2211;  k   n    &#x2211;  &#x2113;   n
      A  i k     &#x03A3;   k &#x2113;   x    A  j &#x2113;   ,
      {\displaystyle {\Sigma }_{ij}^{f}=\sum _{k}^{n}\sum _{\ell }^{n}A_{ik}
      {\Sigma }_{k\ell }^{x}A_{j\ell },}  [{\displaystyle {\Sigma }_{ij}^
      {f}=\sum _{k}^{n}\sum _{\ell }^{n}A_{ik}{\Sigma }_{k\ell }^{x}A_{j\ell
      },}]
or, in matrix notation:
          &#x03A3;  f   =  A   &#x03A3;  x     A   &#x22A4;   .
      {\displaystyle \Sigma ^{f}=\mathrm {A} \Sigma ^{x}\mathrm {A} ^{\top }.}
      [{\displaystyle \Sigma ^{f}=\mathrm {A} \Sigma ^{x}\mathrm {A} ^{\top
      }.}]
This is the most general expression for the propagation of error from one set
of variables onto another. When the errors on x are uncorrelated the general
expression simplifies to
           &#x03A3;   i j   f   =  &#x2211;  k   n    A  i k     &#x03A3;   k
      x    A  j k   .   {\displaystyle {\Sigma }_{ij}^{f}=\sum _{k}^{n}A_{ik}
      {\Sigma }_{k}^{x}A_{jk}.}  [{\displaystyle {\Sigma }_{ij}^{f}=\sum _{k}^
      {n}A_{ik}{\Sigma }_{k}^{x}A_{jk}.}]
where       &#x03A3;   k   x   =  &#x03C3;   x  k     2     {\displaystyle
{\Sigma }_{k}^{x}=\sigma _{x_{k}}^{2}}  [{\displaystyle {\Sigma }_{k}^
{x}=\sigma _{x_{k}}^{2}}] is the variance of k-th element of the x vector. Note
that even though the errors on x may be uncorrelated, the errors on f are in
general correlated; in other words, even if       &#x03A3;  x
{\displaystyle \mathrm {\Sigma ^{x}} }  [{\mathrm  {\Sigma ^{x}}}] is a
diagonal matrix,       &#x03A3;  f      {\displaystyle \mathrm {\Sigma ^{f}} }
[{\mathrm  {\Sigma ^{f}}}] is in general a full matrix.
The general expressions for a scalar-valued function, f, are a little simpler:
         f =  &#x2211;  i   n    a  i    x  i   : f =  a  x    {\displaystyle
      f=\sum _{i}^{n}a_{i}x_{i}:f=\mathrm {a} x\,}  [{\displaystyle f=\sum _
      {i}^{n}a_{i}x_{i}:f=\mathrm {a} x\,}]
          &#x03C3;  f   2   =  &#x2211;  i   n    &#x2211;  j   n    a  i
      &#x03A3;   i j   x    a  j   =  a   &#x03A3;  x     a   &#x22A4;
      {\displaystyle \sigma _{f}^{2}=\sum _{i}^{n}\sum _{j}^{n}a_{i}{\Sigma }_
      {ij}^{x}a_{j}=\mathrm {a} \Sigma ^{x}\mathrm {a} ^{\top }}  [
      {\displaystyle \sigma _{f}^{2}=\sum _{i}^{n}\sum _{j}^{n}a_{i}{\Sigma }_
      {ij}^{x}a_{j}=\mathrm {a} \Sigma ^{x}\mathrm {a} ^{\top }}]
(where a is a row vector).
Each covariance term,      &#x03C3;  i j     {\displaystyle \sigma _{ij}}
[\sigma _{ij}] can be expressed in terms of the correlation_coefficient
&#x03C1;  i j      {\displaystyle \rho _{ij}\,}  [\rho _{{ij}}\,] by
&#x03C3;  i j   =  &#x03C1;  i j    &#x03C3;  i    &#x03C3;  j
{\displaystyle \sigma _{ij}=\rho _{ij}\sigma _{i}\sigma _{j}\,}  [\sigma _{
{ij}}=\rho _{{ij}}\sigma _{i}\sigma _{j}\,], so that an alternative expression
for the variance of f is
          &#x03C3;  f   2   =  &#x2211;  i   n    a  i   2    &#x03C3;  i   2
      +  &#x2211;  i   n    &#x2211;  j ( j &#x2260; i )   n    a  i    a  j
      &#x03C1;  i j    &#x03C3;  i    &#x03C3;  j   .   {\displaystyle \sigma _
      {f}^{2}=\sum _{i}^{n}a_{i}^{2}\sigma _{i}^{2}+\sum _{i}^{n}\sum _{j(j\neq
      i)}^{n}a_{i}a_{j}\rho _{ij}\sigma _{i}\sigma _{j}.}  [{\displaystyle
      \sigma _{f}^{2}=\sum _{i}^{n}a_{i}^{2}\sigma _{i}^{2}+\sum _{i}^{n}\sum _
      {j(j\neq i)}^{n}a_{i}a_{j}\rho _{ij}\sigma _{i}\sigma _{j}.}]
In the case that the variables in x are uncorrelated this simplifies further to
          &#x03C3;  f   2   =  &#x2211;  i   n    a  i   2    &#x03C3;  i   2
      .   {\displaystyle \sigma _{f}^{2}=\sum _{i}^{n}a_{i}^{2}\sigma _{i}^
      {2}.}  [{\displaystyle \sigma _{f}^{2}=\sum _{i}^{n}a_{i}^{2}\sigma _{i}^
      {2}.}]
In the simplest case of identical coefficients and variances, we find
          &#x03C3;  f   =   n   a &#x03C3; .   {\displaystyle \sigma _{f}=
      {\sqrt {n}}a\sigma .}  [{\displaystyle \sigma _{f}={\sqrt {n}}a\sigma .}]
***** Non-linear combinations[edit] *****
See also: Taylor_expansions_for_the_moments_of_functions_of_random_variables
When f is a set of non-linear combination of the variables x, an interval
propagation could be performed in order to compute intervals which contain all
consistent values for the variables. In a probabilistic approach, the function
f must usually be linearized by approximation to a first-order Taylor_series
expansion, though in some cases, exact formulas can be derived that do not
depend on the expansion as is the case for the exact variance of products.[2]
The Taylor expansion would be:
          f  k   &#x2248;  f  k   0   +  &#x2211;  i   n      &#x2202;  f  k
      &#x2202;   x  i        x  i     {\displaystyle f_{k}\approx f_{k}^
      {0}+\sum _{i}^{n}{\frac {\partial f_{k}}{\partial {x_{i}}}}x_{i}}  [f_
      {k}\approx f_{k}^{0}+\sum _{i}^{n}{\frac  {\partial f_{k}}{\partial {x_
      {i}}}}x_{i}]
where     &#x2202;  f  k    /  &#x2202;  x  i     {\displaystyle \partial f_
{k}/\partial x_{i}}  [\partial f_{k}/\partial x_{i}] denotes the partial
derivative of fk with respect to the i-th variable, evaluated at the mean value
of all components of vector x. Or in matrix_notation,
          f  &#x2248;   f   0   +  J   x     {\displaystyle \mathrm {f} \approx
      \mathrm {f} ^{0}+\mathrm {J} \mathrm {x} \,}  [{\mathrm  {f}}\approx
      {\mathrm  {f}}^{0}+{\mathrm  {J}}{\mathrm  {x}}\,]
where J is the Jacobian_matrix. Since f0 is a constant it does not contribute
to the error on f. Therefore, the propagation of error follows the linear case,
above, but replacing the linear coefficients, Aki and Akj by the partial
derivatives,        &#x2202;  f  k     &#x2202;  x  i        {\displaystyle
{\frac {\partial f_{k}}{\partial x_{i}}}}  [{\frac  {\partial f_{k}}{\partial
x_{i}}}] and        &#x2202;  f  k     &#x2202;  x  j        {\displaystyle
{\frac {\partial f_{k}}{\partial x_{j}}}}  [{\frac  {\partial f_{k}}{\partial
x_{j}}}]. In matrix notation,[3]
           &#x03A3;    f    =  J    &#x03A3;    x      J   &#x22A4;   .
      {\displaystyle \mathrm {\Sigma } ^{\mathrm {f} }=\mathrm {J} \mathrm
      {\Sigma } ^{\mathrm {x} }\mathrm {J} ^{\top }.}  [{\displaystyle \mathrm
      {\Sigma } ^{\mathrm {f} }=\mathrm {J} \mathrm {\Sigma } ^{\mathrm {x}
      }\mathrm {J} ^{\top }.}]
That is, the Jacobian of the function is used to transform the rows and columns
of the variance-covariance matrix of the argument. Note this is equivalent to
the matrix expression for the linear case with      J = A    {\displaystyle
\mathrm {J=A} }  [\mathrm{J = A}].
**** Simplification[edit] ****
Neglecting correlations or assuming independent variables yields a common
formula among engineers and experimental scientists to calculate error
propagation, the variance formula:[4]
          s  f   =     (    &#x2202; f   &#x2202; x    )   2    s  x   2   +
      (    &#x2202; f   &#x2202; y    )   2    s  y   2   +   (    &#x2202; f
      &#x2202; z    )   2    s  z   2   + &#x22EF;     {\displaystyle s_{f}=
      {\sqrt {\left({\frac {\partial f}{\partial x}}\right)^{2}s_{x}^{2}+\left(
      {\frac {\partial f}{\partial y}}\right)^{2}s_{y}^{2}+\left({\frac
      {\partial f}{\partial z}}\right)^{2}s_{z}^{2}+\cdots }}}  [{\displaystyle
      s_{f}={\sqrt {\left({\frac {\partial f}{\partial x}}\right)^{2}s_{x}^
      {2}+\left({\frac {\partial f}{\partial y}}\right)^{2}s_{y}^{2}+\left(
      {\frac {\partial f}{\partial z}}\right)^{2}s_{z}^{2}+\cdots }}}]
where      s  f     {\displaystyle s_{f}}  [s_{f}] represents the standard
deviation of the function     f   {\displaystyle f}  [f],      s  x
{\displaystyle s_{x}}  [s_{x}] represents the standard deviation of     x
{\displaystyle x}  [x],      s  y     {\displaystyle s_{y}}  [s_{y}] represents
the standard deviation of     y   {\displaystyle y}  [y], and so forth.
It is important to note that this formula is based on the linear
characteristics of the gradient of     f   {\displaystyle f}  [f] and therefore
it is a good estimation for the standard deviation of     f   {\displaystyle f}
[f] as long as      s  x   ,  s  y   ,  s  z   , &#x2026;   {\displaystyle s_
{x},s_{y},s_{z},\ldots }  [{\displaystyle s_{x},s_{y},s_{z},\ldots }] are small
enough. Specifically, the linear approximation of     f   {\displaystyle f}
[f] has to be close to     f   {\displaystyle f}  [f] inside a neighborhood of
radius      s  x   ,  s  y   ,  s  z   , &#x2026;   {\displaystyle s_{x},s_
{y},s_{z},\ldots }  [{\displaystyle s_{x},s_{y},s_{z},\ldots }].[5]
**** Example[edit] ****
Any non-linear differentiable function,     f ( a , b )   {\displaystyle f
(a,b)}  [f(a,b)], of two variables,     a   {\displaystyle a}  [a] and     b
{\displaystyle b}  [b], can be expanded as
         f &#x2248;  f  0   +    &#x2202; f   &#x2202; a    a +    &#x2202; f
      &#x2202; b    b   {\displaystyle f\approx f^{0}+{\frac {\partial f}
      {\partial a}}a+{\frac {\partial f}{\partial b}}b}  [f\approx f^{0}+{\frac
      {\partial f}{\partial a}}a+{\frac  {\partial f}{\partial b}}b]
hence:
          &#x03C3;  f   2   &#x2248;   |    &#x2202; f   &#x2202; a    |   2
      &#x03C3;  a   2   +   |    &#x2202; f   &#x2202; b    |   2    &#x03C3;
      b   2   + 2    &#x2202; f   &#x2202; a       &#x2202; f   &#x2202; b
      &#x03C3;  a b     {\displaystyle \sigma _{f}^{2}\approx \left|{\frac
      {\partial f}{\partial a}}\right|^{2}\sigma _{a}^{2}+\left|{\frac
      {\partial f}{\partial b}}\right|^{2}\sigma _{b}^{2}+2{\frac {\partial f}
      {\partial a}}{\frac {\partial f}{\partial b}}\sigma _{ab}}  [
      {\displaystyle \sigma _{f}^{2}\approx \left|{\frac {\partial f}{\partial
      a}}\right|^{2}\sigma _{a}^{2}+\left|{\frac {\partial f}{\partial
      b}}\right|^{2}\sigma _{b}^{2}+2{\frac {\partial f}{\partial a}}{\frac
      {\partial f}{\partial b}}\sigma _{ab}}]
where      &#x03C3;  f     {\displaystyle \sigma _{f}}  [{\displaystyle \sigma
_{f}}] is the standard deviation of the function     f   {\displaystyle f}
[f],      &#x03C3;  a     {\displaystyle \sigma _{a}}  [{\displaystyle \sigma _
{a}}] is the standard deviation of     a   {\displaystyle a}  [a],
&#x03C3;  b     {\displaystyle \sigma _{b}}  [{\displaystyle \sigma _{b}}] is
the standard deviation of     b   {\displaystyle b}  [b] and      &#x03C3;  a b
{\displaystyle \sigma _{ab}}  [\sigma_{ab}] is the covariance between     a
{\displaystyle a}  [a] and     b   {\displaystyle b}  [b].
In the particular case that     f = a b    {\displaystyle f=ab\!}  [f=ab\!],
&#x2202; f   &#x2202; a    = b ,    &#x2202; f   &#x2202; b    = a
{\displaystyle {\frac {\partial f}{\partial a}}=b,{\frac {\partial f}{\partial
b}}=a}  [{\frac  {\partial f}{\partial a}}=b,{\frac  {\partial f}{\partial
b}}=a]. Then
          &#x03C3;  f   2   &#x2248;  b  2    &#x03C3;  a   2   +  a  2
      &#x03C3;  b   2   + 2 a b   &#x03C3;  a b     {\displaystyle \sigma _{f}^
      {2}\approx b^{2}\sigma _{a}^{2}+a^{2}\sigma _{b}^{2}+2ab\,\sigma _{ab}}
      [\sigma _{f}^{2}\approx b^{2}\sigma _{a}^{2}+a^{2}\sigma _{b}^
      {2}+2ab\,\sigma _{{ab}}]
or
           (    &#x03C3;  f   f   )   2   &#x2248;   (    &#x03C3;  a   a   )
      2   +   (    &#x03C3;  b   b   )   2   + 2  (    &#x03C3;  a   a   )
      (    &#x03C3;  b   b   )   &#x03C1;  a b     {\displaystyle \left({\frac
      {\sigma _{f}}{f}}\right)^{2}\approx \left({\frac {\sigma _{a}}
      {a}}\right)^{2}+\left({\frac {\sigma _{b}}{b}}\right)^{2}+2\left({\frac
      {\sigma _{a}}{a}}\right)\left({\frac {\sigma _{b}}{b}}\right)\rho _{ab}}
      [{\displaystyle \left({\frac {\sigma _{f}}{f}}\right)^{2}\approx \left(
      {\frac {\sigma _{a}}{a}}\right)^{2}+\left({\frac {\sigma _{b}}
      {b}}\right)^{2}+2\left({\frac {\sigma _{a}}{a}}\right)\left({\frac
      {\sigma _{b}}{b}}\right)\rho _{ab}}]
where      &#x03C1;  a b     {\displaystyle \rho _{ab}}  [{\displaystyle \rho _
{ab}}] is the correlation between     a   {\displaystyle a}  [a] and     b
{\displaystyle b}  [b].
When the variables     a   {\displaystyle a}  [a] and     b   {\displaystyle b}
[b] are uncorrelated,      &#x03C1;  a b   = 0   {\displaystyle \rho _{ab}=0}
[{\displaystyle \rho _{ab}=0}]. Then
           (    &#x03C3;  f   f   )   2   &#x2248;   (    &#x03C3;  a   a   )
      2   +   (    &#x03C3;  b   b   )   2   .   {\displaystyle \left({\frac
      {\sigma _{f}}{f}}\right)^{2}\approx \left({\frac {\sigma _{a}}
      {a}}\right)^{2}+\left({\frac {\sigma _{b}}{b}}\right)^{2}.}  [
      {\displaystyle \left({\frac {\sigma _{f}}{f}}\right)^{2}\approx \left(
      {\frac {\sigma _{a}}{a}}\right)^{2}+\left({\frac {\sigma _{b}}
      {b}}\right)^{2}.}]
**** Caveats and warnings[edit] ****
Error estimates for non-linear functions are biased on account of using a
truncated series expansion. The extent of this bias depends on the nature of
the function. For example, the bias on the error calculated for log(1+x)
increases as x increases, since the expansion to x is a good approximation only
when x is near zero.
For highly non-linear functions, there exist five categories of probabilistic
approaches for uncertainty propagation;[6] see Uncertainty
Quantification#Methodologies_for_forward_uncertainty_propagation for details.
*** Reciprocal[edit] ***
In the special case of the inverse or reciprocal     1  /  B   {\displaystyle
1/B}  [1/B], where     B = N ( 0 , 1 )   {\displaystyle B=N(0,1)}  [B=N(0,1)],
the distribution is a reciprocal_normal_distribution, and there is no definable
variance. For such inverse_distributions and for ratio_distributions, there can
be defined probabilities for intervals, which can be computed either by Monte
Carlo_simulation or, in some cases, by using the GearyâHinkley
transformation.[7]
*** Shifted reciprocal[edit] ***
The statistics, mean and variance, of the shifted reciprocal function       1
p &#x2212; B      {\displaystyle {\frac {1}{p-B}}}  [{\frac  {1}{p-B}}] for
B = N ( &#x03BC; , &#x03C3; )   {\displaystyle B=N(\mu ,\sigma )}  [B=N(\mu
,\sigma )], however, exist in a principal_value sense if the difference between
the shift or pole     p   {\displaystyle p}  [p] and the mean     &#x03BC;
{\displaystyle \mu }  [\mu ] is real. The mean of this transformed random
variable is then indeed the scaled Dawson's_function        2  &#x03C3;   F
(    p &#x2212; &#x03BC;     2   &#x03C3;    )    {\displaystyle {\frac {\sqrt
{2}}{\sigma }}F\left({\frac {p-\mu }{{\sqrt {2}}\sigma }}\right)}  [{\frac  {
{\sqrt  {2}}}{\sigma }}F\left({\frac  {p-\mu }{{\sqrt  {2}}\sigma }}\right)].
[8] In contrast, if the shift     p &#x2212; &#x03BC;   {\displaystyle p-\mu }
[p-\mu ] is purely complex, the mean exists and is a scaled Faddeeva_function,
whose exact expression depends on the sign of the imaginary part,     Im
&#x2061; ( p &#x2212; &#x03BC; )   {\displaystyle \operatorname {Im} (p-\mu )}
[\operatorname {Im}(p-\mu )]. In both cases, the variance is a simple function
of the mean.[9] Therefore, the variance has to be considered in a principal
value sense if     p &#x2212; &#x03BC;   {\displaystyle p-\mu }  [p-\mu ] is
real, while it exists if the imaginary part of     p &#x2212; &#x03BC;
{\displaystyle p-\mu }  [p-\mu ] is non-zero. Note that these means and
variances are exact, as they do not recur to linearisation of the ratio. The
exact covariance of two ratios with a pair of different poles      p  1
{\displaystyle p_{1}}  [p_{1}] and      p  2     {\displaystyle p_{2}}  [p_{2}]
is similarly available.[10] The case of the inverse of a complex normal
variable     B   {\displaystyle B}  [B], shifted or not, exhibits different
characteristics.[8]
***** Example formulae[edit] *****
This table shows the variances of simple functions of the real variables     A
, B    {\displaystyle A,B\!}  [A,B\!], with standard deviations      &#x03C3;
A   ,  &#x03C3;  B   ,    {\displaystyle \sigma _{A},\sigma _{B},\,}  [
{\displaystyle \sigma _{A},\sigma _{B},\,}] covariance      &#x03C3;  A B
{\displaystyle \sigma _{AB}}  [\sigma _{{AB}}] and exactly known real-valued
constants     a , b    {\displaystyle a,b\,}  [a,b\,] (i.e.,      &#x03C3;  a
=  &#x03C3;  b   = 0   {\displaystyle \sigma _{a}=\sigma _{b}=0}  [\sigma _
{a}=\sigma _{b}=0]).
      Function                Variance                 Standard Deviation
                                  &#x03C3;  f   2   =
                              a  2    &#x03C3;  A   2      &#x03C3;  f   =  |
         f = a A              {\displaystyle \sigma _  a  |   &#x03C3;  A
      {\displaystyle f=aA\,}  {f}^{2}=a^{2}\sigma _    {\displaystyle \sigma _
      [f=aA\,]                {A}^{2}}  [\sigma _{f}^  {f}=|a|\sigma _{A}}
                              {2}=a^{2}\sigma _{A}^    [\sigma_f = |a|\sigma_A]
                              {2}]
                                  &#x03C3;  f   2   =      &#x03C3;  f   =    a
                              a  2    &#x03C3;  A   2  2    &#x03C3;  A   2   +
                              +  b  2    &#x03C3;  B   b  2    &#x03C3;  B   2
                              2   + 2 a b   &#x03C3;   + 2 a b   &#x03C3;  A B
         f = a A + b B        A B     {\displaystyle   {\displaystyle \sigma _
      {\displaystyle          \sigma _{f}^{2}=a^       {f}={\sqrt {a^{2}\sigma
      f=aA+bB\,}  [           {2}\sigma _{A}^{2}+b^    _{A}^{2}+b^{2}\sigma _
      {\displaystyle          {2}\sigma _{B}^          {B}^{2}+2ab\,\sigma _
      f=aA+bB\,}]             {2}+2ab\,\sigma _{AB}}   {AB}}}}  [\sigma _{f}=
                              [\sigma _{f}^{2}=a^      {\sqrt  {a^{2}\sigma _
                              {2}\sigma _{A}^{2}+b^    {A}^{2}+b^{2}\sigma _
                              {2}\sigma _{B}^          {B}^{2}+2ab\,\sigma _{
                              {2}+2ab\,\sigma _{{AB}}] {AB}}}}]
                                  &#x03C3;  f   2   =      &#x03C3;  f   =    a
                              a  2    &#x03C3;  A   2  2    &#x03C3;  A   2   +
                              +  b  2    &#x03C3;  B   b  2    &#x03C3;  B   2
                              2   &#x2212; 2 a b       &#x2212; 2 a b
                              &#x03C3;  A B            &#x03C3;  A B
         f = a A &#x2212; b B {\displaystyle \sigma _  {\displaystyle \sigma _
      {\displaystyle f=aA-    {f}^{2}=a^{2}\sigma _    {f}={\sqrt {a^{2}\sigma
      bB\,}  [{\displaystyle  {A}^{2}+b^{2}\sigma _    _{A}^{2}+b^{2}\sigma _
      f=aA-bB\,}]             {B}^{2}-2ab\,\sigma _    {B}^{2}-2ab\,\sigma _
                              {AB}}  [\sigma _{f}^     {AB}}}}  [\sigma _{f}=
                              {2}=a^{2}\sigma _{A}^    {\sqrt  {a^{2}\sigma _
                              {2}+b^{2}\sigma _{B}^    {A}^{2}+b^{2}\sigma _
                              {2}-2ab\,\sigma _{{AB}}] {B}^{2}-2ab\,\sigma _{
                                                       {AB}}}}]
                                  &#x03C3;  f   2          &#x03C3;  f
                              &#x2248;  f  2    [      &#x2248;  | f |
                              (    &#x03C3;  A   A   ) (    &#x03C3;  A   A   )
                              2   +   (    &#x03C3;  B 2   +   (    &#x03C3;  B
                              B   )   2   + 2          B   )   2   + 2
                              &#x03C3;  A B    A B     &#x03C3;  A B    A B
                              ]    {\displaystyle      {\displaystyle \sigma _
                              \sigma _{f}^{2}\approx   {f}\approx
                              f^{2}\left[\left({\frac  \left|f\right|{\sqrt
                              {\sigma _{A}}            {\left({\frac {\sigma _
         f = A B              {A}}\right)^{2}+\left(   {A}}{A}}\right)^
      {\displaystyle f=AB\,}  {\frac {\sigma _{B}}     {2}+\left({\frac {\sigma
      [f=AB\,]                {B}}\right)^{2}+2{\frac  _{B}}{B}}\right)^{2}+2
                              {\sigma _{AB}}           {\frac {\sigma _{AB}}
                              {AB}}\right]}  [         {AB}}}}}  [
                              {\displaystyle \sigma _  {\displaystyle \sigma _
                              {f}^{2}\approx f^        {f}\approx
                              {2}\left[\left({\frac    \left|f\right|{\sqrt
                              {\sigma _{A}}            {\left({\frac {\sigma _
                              {A}}\right)^{2}+\left(   {A}}{A}}\right)^
                              {\frac {\sigma _{B}}     {2}+\left({\frac {\sigma
                              {B}}\right)^{2}+2{\frac  _{B}}{B}}\right)^{2}+2
                              {\sigma _{AB}}           {\frac {\sigma _{AB}}
                              {AB}}\right]}][11][12]   {AB}}}}}]
                                  &#x03C3;  f   2          &#x03C3;  f
                              &#x2248;  f  2    [      &#x2248;  | f |
                              (    &#x03C3;  A   A   ) (    &#x03C3;  A   A   )
                              2   +   (    &#x03C3;  B 2   +   (    &#x03C3;  B
                              B   )   2   &#x2212; 2   B   )   2   &#x2212; 2
                              &#x03C3;  A B    A B     &#x03C3;  A B    A B
                              ]    {\displaystyle      {\displaystyle \sigma _
                              \sigma _{f}^{2}\approx   {f}\approx
                              f^{2}\left[\left({\frac  \left|f\right|{\sqrt
         f =   A B            {\sigma _{A}}            {\left({\frac {\sigma _
      {\displaystyle f={\frac {A}}\right)^{2}+\left(   {A}}{A}}\right)^
      {A}{B}}\,}  [f={\frac   {\frac {\sigma _{B}}     {2}+\left({\frac {\sigma
      {A}{B}}\,]              {B}}\right)^{2}-2{\frac  _{B}}{B}}\right)^{2}-2
                              {\sigma _{AB}}           {\frac {\sigma _{AB}}
                              {AB}}\right]}  [\sigma _ {AB}}}}}  [\sigma _
                              {f}^{2}\approx f^        {f}\approx
                              {2}\left[\left({\frac    \left|f\right|{\sqrt
                              {\sigma _{A}}            {\left({\frac  {\sigma _
                              {A}}\right)^{2}+\left(   {A}}{A}}\right)^
                              {\frac  {\sigma _{B}}    {2}+\left({\frac
                              {B}}\right)^{2}-2{\frac  {\sigma _{B}}
                              {\sigma _{{AB}}}         {B}}\right)^{2}-2{\frac
                              {AB}}\right]][13]        {\sigma _{{AB}}}{AB}}}}]
                                  &#x03C3;  f   2
                              &#x2248;   (   a   b         &#x03C3;  f
                              A   b &#x2212; 1         &#x2248;  |   a   b    A
                              &#x03C3;  A     )   2    b &#x2212; 1
                              =   (     f   b          &#x03C3;  A     |  =  |
                              &#x03C3;  A     A   )    f   b    &#x03C3;  A
                              2     {\displaystyle     A   |    {\displaystyle
                              \sigma _{f}^{2}\approx   \sigma _{f}\approx
         f = a  A  b          \left({a}{b}{A}^{b-1}    \left|{a}{b}{A}^{b-1}
      {\displaystyle f=aA^    {\sigma _{A}}\right)^    {\sigma _
      {b}\,}  [f=aA^{{b}}\,]  {2}=\left({\frac {{f}{b} {A}}\right|=\left|{\frac
                              {\sigma _{A}}}           {{f}{b}{\sigma _{A}}}
                              {A}}\right)^{2}}         {A}}\right|}  [\sigma _
                              [\sigma _{f}^{2}\approx  {f}\approx \left|{a}{b}
                              \left({a}{b}{A}^{{b-1}}  {A}^{{b-1}}{\sigma _
                              {\sigma _{A}}\right)^    {A}}\right|=\left|{\frac
                              {2}=\left({\frac  {{f}   {{f}{b}{\sigma _{A}}}
                              {b}{\sigma _{A}}}        {A}}\right|]
                              {A}}\right)^{2}]
                                  &#x03C3;  f   2          &#x03C3;  f
                              &#x2248;   (  a          &#x2248;  |  a
                              &#x03C3;  A   A    )   2 &#x03C3;  A   A    |
         f = a ln &#x2061;    {\displaystyle \sigma _  {\displaystyle \sigma _
      ( b A )                 {f}^{2}\approx \left(a   {f}\approx \left|a{\frac
      {\displaystyle f=a\ln   {\frac {\sigma _{A}}     {\sigma _{A}}
      (bA)\,}  [f=a\ln(bA)\,] {A}}\right)^{2}}         {A}}\right|}  [\sigma _
                              [\sigma _{f}^{2}\approx  {f}\approx \left|a{\frac
                              \left(a{\frac  {\sigma _ {\sigma _{A}}
                              {A}}{A}}\right)^{2}][14] {A}}\right|]
                                  &#x03C3;  f   2          &#x03C3;  f
                              &#x2248;   (  a          &#x2248;  |  a
                              &#x03C3;  A    A ln      &#x03C3;  A    A ln
         f = a  log  10       &#x2061; ( 10 )     )    &#x2061; ( 10 )     |
      &#x2061; ( b A )        2     {\displaystyle     {\displaystyle \sigma _
      {\displaystyle f=a\log  \sigma _{f}^{2}\approx   {f}\approx \left|a{\frac
      _{10}(bA)\,}  [         \left(a{\frac {\sigma _  {\sigma _{A}}{A\ln
      {\displaystyle f=a\log  {A}}{A\ln(10)}}\right)^  (10)}}\right|}  [\sigma
      _{10}(bA)\,}]           {2}}  [\sigma _{f}^      _{f}\approx \left|a
                              {2}\approx \left(a{\frac {\frac  {\sigma _{A}}
                              {\sigma _{A}}{A\ln       {A\ln(10)}}\right|]
                              (10)}}\right)^{2}][14]
                                  &#x03C3;  f   2          &#x03C3;  f
                              &#x2248;  f  2     (  b  &#x2248;  |  f  (  b
                              &#x03C3;  A    )   2     &#x03C3;  A    )   |
         f = a  e  b A        {\displaystyle \sigma _  {\displaystyle \sigma _
      {\displaystyle f=ae^    {f}^{2}\approx f^        {f}\approx \left|f\left
      {bA}\,}  [f=ae^{        {2}\left(b\sigma _       (b\sigma _
      {bA}}\,]                {A}\right)^{2}}  [\sigma {A}\right)\right|}
                              _{f}^{2}\approx f^       [\sigma _{f}\approx
                              {2}\left(b\sigma _       \left|f\left(b\sigma _
                              {A}\right)^{2}][15]      {A}\right)\right|]
                                  &#x03C3;  f   2          &#x03C3;  f
                              &#x2248;  f  2   ( b ln  &#x2248;  |  f ( b ln
                              &#x2061; ( a )  &#x03C3; &#x2061; ( a )  &#x03C3;
                              A    )  2                A   )  |
         f =  a  b A          {\displaystyle \sigma _  {\displaystyle \sigma _
      {\displaystyle f=a^     {f}^{2}\approx f^{2}     {f}\approx \left|f(b\ln
      {bA}\,}  [f=a^{{bA}}\,] (b\ln(a)\sigma _{A})^    (a)\sigma _{A})\right|}
                              {2}}  [{\displaystyle    [{\displaystyle \sigma _
                              \sigma _{f}^{2}\approx   {f}\approx \left|f(b\ln
                              f^{2}(b\ln(a)\sigma _    (a)\sigma _{A})\right|}]
                              {A})^{2}}]
                                  &#x03C3;  f   2
                              &#x2248;   [  a b cos        &#x03C3;  f
                              &#x2061; ( b A )         &#x2248;  |  a b cos
         f = a sin &#x2061;   &#x03C3;  A    ]   2     &#x2061; ( b A )
      ( b A )                 {\displaystyle \sigma _  &#x03C3;  A    |
      {\displaystyle f=a\sin  {f}^{2}\approx \left     {\displaystyle \sigma _
      (bA)\,}  [              [ab\cos(bA)\sigma _      {f}\approx \left|ab\cos
      {\displaystyle f=a\sin  {A}\right]^{2}}  [       (bA)\sigma _{A}\right|}
      (bA)\,}]                {\displaystyle \sigma _  [{\displaystyle \sigma _
                              {f}^{2}\approx \left     {f}\approx \left|ab\cos
                              [ab\cos(bA)\sigma _      (bA)\sigma _{A}\right|}]
                              {A}\right]^{2}}]
                                  &#x03C3;  f   2
                              &#x2248;   [  a b sin        &#x03C3;  f
                              &#x2061; ( b A )         &#x2248;  |  a b sin
         f = a cos &#x2061;   &#x03C3;  A    ]   2     &#x2061; ( b A )
      (  b A  )               {\displaystyle \sigma _  &#x03C3;  A    |
      {\displaystyle f=a\cos  {f}^{2}\approx \left     {\displaystyle \sigma _
      \left(bA\right)\,}  [   [ab\sin(bA)\sigma _      {f}\approx \left|ab\sin
      {\displaystyle f=a\cos  {A}\right]^{2}}  [       (bA)\sigma _{A}\right|}
      \left(bA\right)\,}]     {\displaystyle \sigma _  [{\displaystyle \sigma _
                              {f}^{2}\approx \left     {f}\approx \left|ab\sin
                              [ab\sin(bA)\sigma _      (bA)\sigma _{A}\right|}]
                              {A}\right]^{2}}]
                                  &#x03C3;  f   2          &#x03C3;  f
                              &#x2248;   [  a b  sec   &#x2248;  |  a b  sec  2
                              2   &#x2061; ( b A )     &#x2061; ( b A )
         f = a tan &#x2061;   &#x03C3;  A    ]   2     &#x03C3;  A    |
      (  b A  )               {\displaystyle \sigma _  {\displaystyle \sigma _
      {\displaystyle f=a\tan  {f}^{2}\approx \left     {f}\approx \left|ab\sec
      \left(bA\right)\,}  [   [ab\sec ^{2}(bA)\sigma _ ^{2}(bA)\sigma _
      {\displaystyle f=a\tan  {A}\right]^{2}}  [       {A}\right|}  [
      \left(bA\right)\,}]     {\displaystyle \sigma _  {\displaystyle \sigma _
                              {f}^{2}\approx \left     {f}\approx \left|ab\sec
                              [ab\sec ^{2}(bA)\sigma _ ^{2}(bA)\sigma _
                              {A}\right]^{2}}]         {A}\right|}]
                                  &#x03C3;  f   2          &#x03C3;  f
                              &#x2248;  f  2    [      &#x2248;  | f |
                              (    B A    &#x03C3;  A  (    B A    &#x03C3;  A
                              )   2   +   (  ln        )   2   +   (  ln
                              &#x2061; ( A )  &#x03C3; &#x2061; ( A )  &#x03C3;
                              B    )   2   + 2    B ln B    )   2   + 2    B ln
                              &#x2061; ( A )  A        &#x2061; ( A )  A
                              &#x03C3;  A B    ]       &#x03C3;  A B
                              {\displaystyle \sigma _  {\displaystyle \sigma _
                              {f}^{2}\approx f^        {f}\approx
                              {2}\left[\left({\frac    \left|f\right|{\sqrt
         f =  A  B            {B}{A}}\sigma _          {\left({\frac {B}
      {\displaystyle f=A^     {A}\right)^{2}+\left(\ln {A}}\sigma _{A}\right)^
      {B}\,}  [f=A^{B}\,]     (A)\sigma _{B}\right)^   {2}+\left(\ln(A)\sigma _
                              {2}+2{\frac {B\ln(A)}    {B}\right)^{2}+2{\frac
                              {A}}\sigma _{AB}\right]} {B\ln(A)}{A}}\sigma _
                              [\sigma _{f}^{2}\approx  {AB}}}}  [\sigma _
                              f^{2}\left[\left({\frac  {f}\approx
                              {B}{A}}\sigma _          \left|f\right|{\sqrt
                              {A}\right)^{2}+\left(\ln {\left({\frac  {B}
                              (A)\sigma _{B}\right)^   {A}}\sigma _{A}\right)^
                              {2}+2{\frac  {B\ln(A)}   {2}+\left(\ln(A)\sigma _
                              {A}}\sigma _{            {B}\right)^{2}+2{\frac
                              {AB}}\right]]            {B\ln(A)}{A}}\sigma _{
                                                       {AB}}}}]
                                  &#x03C3;  f   2          &#x03C3;  f
                              &#x2248;   (   A f   )   &#x2248;     (   A f   )
                              2    a  2    &#x03C3;  A 2    a  2    &#x03C3;  A
                              2   +   (   B f   )   2  2   +   (   B f   )   2
                              b  2    &#x03C3;  B   2  b  2    &#x03C3;  B   2
                              &#x00B1; 2 a b    A B    &#x00B1; 2 a b    A B
                              f  2       &#x03C3;  A B f  2       &#x03C3;  A B
                              {\displaystyle \sigma _  {\displaystyle \sigma _
                              {f}^{2}\approx \left(    {f}\approx {\sqrt {\left
         f =   a  A  2        {\frac {A}{f}}\right)^   ({\frac {A}{f}}\right)^
      &#x00B1; b  B  2        {2}a^{2}\sigma _{A}^     {2}a^{2}\sigma _{A}^
      {\displaystyle f={\sqrt {2}+\left({\frac {B}     {2}+\left({\frac {B}
      {aA^{2}\pm bB^{2}}}\,}  {f}}\right)^{2}b^        {f}}\right)^{2}b^
      [{\displaystyle f=      {2}\sigma _{B}^{2}\pm    {2}\sigma _{B}^{2}\pm
      {\sqrt {aA^{2}\pm bB^   2ab{\frac {AB}{f^        2ab{\frac {AB}{f^
      {2}}}\,}]               {2}}}\,\sigma _{AB}}  [  {2}}}\,\sigma _{AB}}}}
                              {\displaystyle \sigma _  [{\displaystyle \sigma _
                              {f}^{2}\approx \left(    {f}\approx {\sqrt {\left
                              {\frac {A}{f}}\right)^   ({\frac {A}{f}}\right)^
                              {2}a^{2}\sigma _{A}^     {2}a^{2}\sigma _{A}^
                              {2}+\left({\frac {B}     {2}+\left({\frac {B}
                              {f}}\right)^{2}b^        {f}}\right)^{2}b^
                              {2}\sigma _{B}^{2}\pm    {2}\sigma _{B}^{2}\pm
                              2ab{\frac {AB}{f^        2ab{\frac {AB}{f^
                              {2}}}\,\sigma _{AB}}]    {2}}}\,\sigma _{AB}}}}]
For uncorrelated variables (     &#x03C1;  A B   = 0   {\displaystyle \rho _
{AB}=0}  [\rho _{{AB}}=0]) the covariance terms are also zero, as      &#x03C3;
A B   =  &#x03C1;  A B    &#x03C3;  A    &#x03C3;  B      {\displaystyle \sigma
_{AB}=\rho _{AB}\sigma _{A}\sigma _{B}\,}  [\sigma _{{AB}}=\rho _{{AB}}\sigma _
{A}\sigma _{B}\,].
In this case, expressions for more complicated functions can be derived by
combining simpler functions. For example, repeated multiplication, assuming no
correlation gives
         f = A B C ;    (    &#x03C3;  f   f   )   2   &#x2248;   (    &#x03C3;
      A   A   )   2   +   (    &#x03C3;  B   B   )   2   +   (    &#x03C3;  C
      C   )   2   .   {\displaystyle f=ABC;\qquad \left({\frac {\sigma _{f}}
      {f}}\right)^{2}\approx \left({\frac {\sigma _{A}}{A}}\right)^{2}+\left(
      {\frac {\sigma _{B}}{B}}\right)^{2}+\left({\frac {\sigma _{C}}
      {C}}\right)^{2}.}  [{\displaystyle f=ABC;\qquad \left({\frac {\sigma _
      {f}}{f}}\right)^{2}\approx \left({\frac {\sigma _{A}}{A}}\right)^
      {2}+\left({\frac {\sigma _{B}}{B}}\right)^{2}+\left({\frac {\sigma _{C}}
      {C}}\right)^{2}.}]
For the case     f = A B   {\displaystyle f=AB}  [f=AB] we also have Goodman's
expression[2] for the exact variance: for the uncorrelated case it is
         V ( X Y ) = E ( X  )  2   V ( Y ) + E ( Y  )  2   V ( X ) + E ( ( X
      &#x2212; E ( X )  )  2   ( Y &#x2212; E ( Y )  )  2   )   {\displaystyle
      V(XY)=E(X)^{2}V(Y)+E(Y)^{2}V(X)+E((X-E(X))^{2}(Y-E(Y))^{2})}  [V(XY)=E
      (X)^{2}V(Y)+E(Y)^{2}V(X)+E((X-E(X))^{2}(Y-E(Y))^{2})]
and therefore we have:
          &#x03C3;  f   2   =  A  2    &#x03C3;  B   2   +  B  2    &#x03C3;  A
      2   +  &#x03C3;  A   2    &#x03C3;  B   2     {\displaystyle \sigma _{f}^
      {2}=A^{2}\sigma _{B}^{2}+B^{2}\sigma _{A}^{2}+\sigma _{A}^{2}\sigma _{B}^
      {2}}  [\sigma _{f}^{2}=A^{2}\sigma _{B}^{2}+B^{2}\sigma _{A}^{2}+\sigma _
      {A}^{2}\sigma _{B}^{2}]
***** Example calculations[edit] *****
**** Inverse tangent function[edit] ****
We can calculate the uncertainty propagation for the inverse tangent function
as an example of using partial derivatives to propagate error.
Define
         f ( x ) = arctan &#x2061; ( x ) ,   {\displaystyle f(x)=\arctan(x),}
      [f(x)=\arctan(x),]
where      &#x0394;  x     {\displaystyle \Delta _{x}}  [\Delta_x] is the
absolute uncertainty on our measurement of x. The derivative of f(x) with
respect to x is
            d f   d x    =   1  1 +  x  2      .   {\displaystyle {\frac {df}
      {dx}}={\frac {1}{1+x^{2}}}.}  [{\frac  {df}{dx}}={\frac  {1}{1+x^{2}}}.]
Therefore, our propagated uncertainty is
          &#x0394;  f   &#x2248;    &#x0394;  x    1 +  x  2      ,
      {\displaystyle \Delta _{f}\approx {\frac {\Delta _{x}}{1+x^{2}}},}  [
      {\displaystyle \Delta _{f}\approx {\frac {\Delta _{x}}{1+x^{2}}},}]
where      &#x0394;  f     {\displaystyle \Delta _{f}}  [{\displaystyle \Delta
_{f}}] is the absolute propagated uncertainty.
**** Resistance measurement[edit] ****
A practical application is an experiment in which one measures current, I, and
voltage, V, on a resistor in order to determine the resistance, R, using Ohm's
law, R = V / I.
Given the measured variables with uncertainties, I Â± ÏI and V Â± ÏV, and
neglecting their possible correlation, the uncertainty in the computed
quantity, ÏR, is:
          &#x03C3;  R   &#x2248;    &#x03C3;  V   2     (   1 I   )   2   +
      &#x03C3;  I   2     (    &#x2212; V   I  2     )   2     = R
      (    &#x03C3;  V   V   )   2   +   (    &#x03C3;  I   I   )   2     .
      {\displaystyle \sigma _{R}\approx {\sqrt {\sigma _{V}^{2}\left({\frac {1}
      {I}}\right)^{2}+\sigma _{I}^{2}\left({\frac {-V}{I^{2}}}\right)^{2}}}=R
      {\sqrt {\left({\frac {\sigma _{V}}{V}}\right)^{2}+\left({\frac {\sigma _
      {I}}{I}}\right)^{2}}}.}  [\sigma_R \approx \sqrt{ \sigma_V^2 \left(\frac
      {1}{I}\right)^2 + \sigma_I^2 \left(\frac{-V}{I^2}\right)^2 } = R\sqrt
      { \left(\frac{\sigma_V}{V}\right)^2 + \left(\frac{\sigma_I}{I}\right)^2
      }.]
***** See also[edit] *****
    * Accuracy_and_precision
    * Automatic_differentiation
    * Delta_method
    * Errors_and_residuals_in_statistics
    * Experimental_uncertainty_analysis
    * Interval_finite_element
    * Measurement_uncertainty
    * Probability_bounds_analysis
    * Significance_arithmetic
    * Uncertainty_quantification
    * Random-fuzzy_variable
***** References[edit] *****
   1. ^Kirchner, James. "Data_Analysis_Toolkit_#5:_Uncertainty_Analysis_and
      Error_Propagation" (PDF). Berkeley Seismology Laboratory. University of
      California. Retrieved 22 April 2016.
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
   3. ^ a bGoodman,_Leo (1960). "On the Exact Variance of Products". Journal of
      the American Statistical Association. 55 (292): 708â713. doi:10.2307/
      2281592. JSTOR 2281592.
   4. ^ Ochoa1,Benjamin; Belongie, Serge "Covariance_Propagation_for_Guided
      Matching"
   5. ^Ku, H. H. (October 1966). "Notes_on_the_use_of_propagation_of_error
      formulas". Journal of Research of the National Bureau of Standards. 70C
      (4): 262. doi:10.6028/jres.070c.025. ISSN 0022-4316. Retrieved 3 October
      2012.
   6. ^Clifford, A. A. (1973). Multivariate error analysis: a handbook of error
      propagation and calculation in many-parameter systems. John Wiley & Sons.
      ISBN 978-0470160558.
   7. [page needed]
   8. ^Lee, S. H.; Chen, W. (2009). "A comparative study of uncertainty
      propagation methods for black-box-type problems". Structural and
      Multidisciplinary Optimization. 37 (3): 239â253. doi:10.1007/s00158-
      008-0234-7.
   9. ^Hayya,_Jack; Armstrong, Donald; Gressis, Nicolas (July 1975). "A Note on
      the Ratio of Two Normally Distributed Variables". Management_Science. 21
      (11): 1338â1341. doi:10.1287/mnsc.21.11.1338. JSTOR 2629897.
  10. ^ a bLecomte, Christophe (May 2013). "Exact statistics of systems with
      uncertainties: an analytical theory of rank-one stochastic dynamic
      systems". Journal of Sound and Vibrations. 332 (11): 2750â2776. doi:
      10.1016/j.jsv.2012.12.009.
  11. ^Lecomte, Christophe (May 2013). "Exact statistics of systems with
      uncertainties: an analytical theory of rank-one stochastic dynamic
      systems". Journal of Sound and Vibrations. 332 (11). Section (4.1.1).
      doi:10.1016/j.jsv.2012.12.009.
  12. ^Lecomte, Christophe (May 2013). "Exact statistics of systems with
      uncertainties: an analytical theory of rank-one stochastic dynamic
      systems". Journal of Sound and Vibrations. 332 (11). Eq.(39)-(40). doi:
      10.1016/j.jsv.2012.12.009.
  13. ^"A_Summary_of_Error_Propagation" (PDF). p. 2. Retrieved 2016-04-04.
  14. ^"Propagation_of_Uncertainty_through_Mathematical_Operations" (PDF).
      p. 5. Retrieved 2016-04-04.
  15. ^"Strategies_for_Variance_Estimation" (PDF). p. 37. Retrieved 2013-01-18.
  16. ^ a bHarris, Daniel C. (2003), Quantitative_chemical_analysis (6th ed.),
      Macmillan, p. 56, ISBN 978-0-7167-4464-1
  17. ^"Error_Propagation_tutorial" (PDF). Foothill College. October 9, 2009.
      Retrieved 2012-03-01.
***** Further reading[edit] *****
    * Bevington, Philip R.; Robinson, D. Keith (2002), Data Reduction and Error
      Analysis for the Physical Sciences (3rd ed.), McGraw-Hill, ISBN 978-0-07-
      119926-1
Fornasini, Paolo (2008), The_uncertainty_in_physical_measurements:_an
introduction_to_data_analysis_in_the_physics_laboratory, Springer, p. 161,
ISBN 978-0-387-78649-0
Meyer, Stuart L. (1975), Data Analysis for Scientists and Engineers, Wiley,
ISBN 978-0-471-59995-1
Peralta, M. (2012), Propagation Of Errors: How To Mathematically Predict
Measurement Errors, CreateSpace
Rouaud, M. (2013), Probability,_Statistics_and_Estimation:_Propagation_of
Uncertainties_in_Experimental_Measurement (PDF) (short ed.)
Taylor, J. R. (1997), An Introduction to Error Analysis: The Study of
Uncertainties in Physical Measurements (2nd ed.), University Science Books
***** External links[edit] *****
    * ScienceMathMastery.com - Propagation_of_error_with_single_and_multiple
      independent_variables.
    * A_detailed_discussion_of_measurements_and_the_propagation_of_uncertainty
      explaining the benefits of using error propagation formulas and Monte
      Carlo simulations instead of simple significance_arithmetic
    * GUM, Guide to the Expression of Uncertainty in Measurement
    * EPFL_An_Introduction_to_Error_Propagation, Derivation, Meaning and
      Examples of Cy = Fx Cx Fx'
    * uncertainties_package, a program/library for transparently performing
      calculations with uncertainties (and error correlations).
    * soerp_package, a python program/library for transparently performing
      *second-order* calculations with uncertainties (and error correlations).
    * Joint Committee for Guides in Metrology (2011). JCGM_102:_Evaluation_of
      Measurement_Data_-_Supplement_2_to_the_"Guide_to_the_Expression_of
      Uncertainty_in_Measurement"_-_Extension_to_Any_Number_of_Output
      Quantities (PDF) (Technical report). JCGM. Retrieved 13 February 2013.
Authority_control [Edit_this_at_Wikidata]     * GND: 4479158-6

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Propagation_of_uncertainty&oldid=904889753"
Categories:
    * Algebra_of_random_variables
    * Numerical_analysis
    * Statistical_approximations
    * Statistical_deviation_and_dispersion
Hidden categories:
    * Wikipedia_articles_needing_page_number_citations_from_October_2012
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * Italiano
    * Magyar
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * Suomi
    * Svenska
    * ä¸­æ
Edit_links
    * This page was last edited on 5 July 2019, at 09:31 (UTC).
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
