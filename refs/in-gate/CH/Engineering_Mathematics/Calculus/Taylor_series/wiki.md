The following text has been accessed from https://en.wikipedia.org/wiki/Taylor_series at Fri Aug 9 01:13:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















[This_is_a_good_article._Follow_the_link_for_more_information.]
****** Taylor series ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other notions of series expansion, see Series_(mathematics).
As the degree of the Taylor polynomial rises, it approaches the correct
function. This image shows sin x and its Taylor approximations, polynomials of
degree 1, 3, 5, 7, 9, 11 and 13.
Part of a series of articles about
Calculus
    * Fundamental_theorem
    * Limits_of_functions
    * Continuity
    * Mean_value_theorem
    * Rolle's_theorem
Differential
Definitions
    * Derivative (generalizations)
    * Differential
          o infinitesimal
          o of_a_function
          o total
Concepts
    * Differentiation_notation
    * Second_derivative
    * Third_derivative
    * Change_of_variables
    * Implicit_differentiation
    * Related_rates
    * Taylor's_theorem
Rules_and_identities
    * Sum
    * Product
    * Chain
    * Power
    * Quotient
    * Inverse
    * General_Leibniz
    * FaÃ _di_Bruno's_formula
Integral
    * Lists_of_integrals
Definitions
    * Antiderivative
    * Integral (improper)
    * Riemann_integral
    * Lebesgue_integration
    * Contour_integration
Integration by
    * Parts
    * Discs
    * Cylindrical_shells
    * Substitution (trigonometric)
    * Partial_fractions
    * Order
    * Reduction_formulae
Series
    * Geometric (arithmetico-geometric)
    * Harmonic
    * Alternating
    * Power
    * Binomial
    * Taylor
Convergence_tests
    * Summand_limit_(term_test)
    * Ratio
    * Root
    * Integral
    * Direct_comparison
    *
      Limit_comparison
    * Alternating_series
    * Cauchy_condensation
    * Dirichlet
    * Abel
Vector
    * Gradient
    * Divergence
    * Curl
    * Laplacian
    * Directional_derivative
    * Identities
Theorems
    * Divergence
    * Gradient
    * Green's
    * KelvinâStokes
    * Stokes
Multivariable
Formalisms
    * Matrix
    * Tensor
    * Exterior
    * Geometric
Definitions
    * Partial_derivative
    * Multiple_integral
    * Line_integral
    * Surface_integral
    * Volume_integral
    * Jacobian
    * Hessian
Specialized
    * Fractional
    * Malliavin
    * Stochastic
    * Variations
Glossary_of_calculus
    * Glossary_of_calculus
    * v
    * t
    * e
In mathematics, a Taylor series is a representation of a function as an
infinite_sum of terms that are calculated from the values of the function's
derivatives at a single point.[1][2] [3]
In the West, the subject was formulated by the Scottish mathematician James
Gregory and formally introduced by the English mathematician Brook_Taylor in
1715. If the Taylor series is centered at zero, then that series is also called
a Maclaurin series, after the Scottish mathematician Colin_Maclaurin, who made
extensive use of this special case of Taylor series in the 18th century.
A function can be approximated by using a finite number of terms of its Taylor
series. Taylor's_theorem gives quantitative estimates on the error introduced
by the use of such an approximation. The polynomial formed by taking some
initial terms of the Taylor series is called a Taylor polynomial. The Taylor
series of a function is the limit of that function's Taylor polynomials as the
degree increases, provided that the limit exists. A function may not be equal
to its Taylor series, even if its Taylor series converges at every point. A
function that is equal to its Taylor series in an open_interval (or a disc in
the complex_plane) is known as an analytic_function in that interval.
⁰
***** Contents *****
    * 1_Definition
    * 2_Examples
    * 3_History
    * 4_Analytic_functions
    * 5_Approximation_error_and_convergence
          o 5.1_Generalization
    * 6_List_of_Maclaurin_series_of_some_common_functions
          o 6.1_Exponential_function
          o 6.2_Natural_logarithm
          o 6.3_Geometric_series
          o 6.4_Binomial_series
          o 6.5_Trigonometric_functions
          o 6.6_Hyperbolic_functions
    * 7_Calculation_of_Taylor_series
          o 7.1_First_example
          o 7.2_Second_example
          o 7.3_Third_example
    * 8_Taylor_series_as_definitions
    * 9_Taylor_series_in_several_variables
          o 9.1_Example
    * 10_Comparison_with_Fourier_series
    * 11_See_also
    * 12_Notes
    * 13_References
    * 14_External_links
***** Definition[edit] *****
The Taylor series of a real or complex-valued_function f (x) that is infinitely
differentiable at a real or complex_number a is the power_series
         f ( a ) +     f &#x2032;  ( a )   1 !    ( x &#x2212; a ) +     f
      &#x2033;  ( a )   2 !    ( x &#x2212; a  )  2   +     f &#x2034;  ( a )
      3 !    ( x &#x2212; a  )  3   + &#x22EF; ,   {\displaystyle f(a)+{\frac
      {f'(a)}{1!}}(x-a)+{\frac {f''(a)}{2!}}(x-a)^{2}+{\frac {f'''(a)}{3!}}(x-
      a)^{3}+\cdots ,}  [{\displaystyle f(a)+{\frac {f'(a)}{1!}}(x-a)+{\frac
      {f''(a)}{2!}}(x-a)^{2}+{\frac {f'''(a)}{3!}}(x-a)^{3}+\cdots ,}]
where n! denotes the factorial of n and f(n)(a) denotes the nth derivative of f
evaluated at the point a. In the more compact sigma_notation, this can be
written as
          &#x2211;  n = 0   &#x221E;       f  ( n )   ( a )   n !    ( x
      &#x2212; a  )  n   .   {\displaystyle \sum _{n=0}^{\infty }{\frac {f^{
      (n)}(a)}{n!}}(x-a)^{n}.}  [{\displaystyle \sum _{n=0}^{\infty }{\frac {f^
      {(n)}(a)}{n!}}(x-a)^{n}.}]
The derivative of order zero of f is defined to be f itself and (x â a)0 and
0! are both defined to be 1. When a = 0, the series is also called a Maclaurin
series.[4]
***** Examples[edit] *****
The Taylor series for any polynomial is the polynomial itself.
The Maclaurin series for 1/1 â x is the geometric_series
         1 + x +  x  2   +  x  3   + &#x22EF;   {\displaystyle 1+x+x^{2}+x^
      {3}+\cdots }  [1+x+x^{2}+x^{3}+\cdots ]
so the Taylor series for 1/x at a = 1 is
         1 &#x2212; ( x &#x2212; 1 ) + ( x &#x2212; 1  )  2   &#x2212; ( x
      &#x2212; 1  )  3   + &#x22EF; .   {\displaystyle 1-(x-1)+(x-1)^{2}-(x-1)^
      {3}+\cdots .}  [{\displaystyle 1-(x-1)+(x-1)^{2}-(x-1)^{3}+\cdots .}]
By integrating the above Maclaurin series, we find the Maclaurin series for log
(1 â x), where log denotes the natural_logarithm:
         &#x2212; x &#x2212;    1 2     x  2   &#x2212;    1 3     x  3
      &#x2212;    1 4     x  4   &#x2212; &#x22EF;   {\displaystyle -x-{\tfrac
      {1}{2}}x^{2}-{\tfrac {1}{3}}x^{3}-{\tfrac {1}{4}}x^{4}-\cdots }  [
      {\displaystyle -x-{\tfrac {1}{2}}x^{2}-{\tfrac {1}{3}}x^{3}-{\tfrac {1}
      {4}}x^{4}-\cdots }]
and the corresponding Taylor series for log x at a = 1 is
         ( x &#x2212; 1 ) &#x2212;    1 2    ( x &#x2212; 1  )  2   +    1 3
      ( x &#x2212; 1  )  3   &#x2212;    1 4    ( x &#x2212; 1  )  4   +
      &#x22EF; ,   {\displaystyle (x-1)-{\tfrac {1}{2}}(x-1)^{2}+{\tfrac {1}
      {3}}(x-1)^{3}-{\tfrac {1}{4}}(x-1)^{4}+\cdots ,}  [{\displaystyle (x-1)-
      {\tfrac {1}{2}}(x-1)^{2}+{\tfrac {1}{3}}(x-1)^{3}-{\tfrac {1}{4}}(x-1)^
      {4}+\cdots ,}]
and more generally, the corresponding Taylor series for log x at some a = x0
is:
         log &#x2061;  x  0   +   1  x  0     ( x &#x2212;  x  0   ) &#x2212;
      1  x  0   2         (  x &#x2212;  x  0    )   2   2   + &#x22EF; .
      {\displaystyle \log x_{0}+{\frac {1}{x_{0}}}(x-x_{0})-{\frac {1}{x_{0}^
      {2}}}{\frac {\left(x-x_{0}\right)^{2}}{2}}+\cdots .}  [{\displaystyle
      \log x_{0}+{\frac {1}{x_{0}}}(x-x_{0})-{\frac {1}{x_{0}^{2}}}{\frac
      {\left(x-x_{0}\right)^{2}}{2}}+\cdots .}]
The Taylor series for the exponential_function ex at a = 0 is
              &#x2211;  n = 0   &#x221E;      x  n    n !       =    x  0    0
      !    +    x  1    1 !    +    x  2    2 !    +    x  3    3 !    +    x
      4    4 !    +    x  5    5 !    + &#x22EF;       = 1 + x +    x  2   2
      +    x  3   6   +    x  4   24   +    x  5   120   + &#x22EF; .
      {\displaystyle {\begin{aligned}\sum _{n=0}^{\infty }{\frac {x^{n}}{n!}}&=
      {\frac {x^{0}}{0!}}+{\frac {x^{1}}{1!}}+{\frac {x^{2}}{2!}}+{\frac {x^
      {3}}{3!}}+{\frac {x^{4}}{4!}}+{\frac {x^{5}}{5!}}+\cdots \\&=1+x+{\frac
      {x^{2}}{2}}+{\frac {x^{3}}{6}}+{\frac {x^{4}}{24}}+{\frac {x^{5}}
      {120}}+\cdots .\end{aligned}}}  [{\displaystyle {\begin{aligned}\sum _
      {n=0}^{\infty }{\frac {x^{n}}{n!}}&={\frac {x^{0}}{0!}}+{\frac {x^{1}}
      {1!}}+{\frac {x^{2}}{2!}}+{\frac {x^{3}}{3!}}+{\frac {x^{4}}{4!}}+{\frac
      {x^{5}}{5!}}+\cdots \\&=1+x+{\frac {x^{2}}{2}}+{\frac {x^{3}}{6}}+{\frac
      {x^{4}}{24}}+{\frac {x^{5}}{120}}+\cdots .\end{aligned}}}]
The above expansion holds because the derivative of ex with respect to x is
also ex and e0 equals 1. This leaves the terms (x â 0)n in the numerator and
n! in the denominator for each term in the infinite sum.
***** History[edit] *****
The Greek philosopher Zeno considered the problem of summing an infinite series
to achieve a finite result, but rejected it as an impossibility[5]; the result
was Zeno's_paradox. Later, Aristotle proposed a philosophical resolution of the
paradox, but the mathematical content was apparently unresolved until taken up
by Archimedes, as it had been prior to Aristotle by the Presocratic Atomist
Democritus. It was through Archimedes's method_of_exhaustion that an infinite
number of progressive subdivisions could be performed to achieve a finite
result.[6] Liu_Hui independently employed a similar method a few centuries
later.[7]
In the 14th century, the earliest examples of the use of Taylor series and
closely related methods were given by Madhava_of_Sangamagrama.[1][2] Though no
record of his work survives, writings of later Indian_mathematicians suggest
that he found a number of special cases of the Taylor series, including those
for the trigonometric_functions of sine, cosine, tangent, and arctangent. The
Kerala_School_of_Astronomy_and_Mathematics further expanded his works with
various series expansions and rational approximations until the 16th century.
In the 17th century, James_Gregory also worked in this area and published
several Maclaurin series. It was not until 1715 however that a general method
for constructing these series for all functions for which they exist was
finally provided by Brook_Taylor,[8] after whom the series are now named.
The Maclaurin series was named after Colin_Maclaurin, a professor in Edinburgh,
who published the special case of the Taylor result in the 18th century.
***** Analytic functions[edit] *****
The function e(â1/x2) is not analytic at x = 0: the Taylor series is
identically 0, although the function is not.
Main article: analytic_function
If f (x) is given by a convergent power series in an open disc (or interval in
the real line) centred at b in the complex plane, it is said to be analytic in
this disc. Thus for x in this disc, f is given by a convergent power series
         f ( x ) =  &#x2211;  n = 0   &#x221E;    a  n   ( x &#x2212; b  )  n
      .   {\displaystyle f(x)=\sum _{n=0}^{\infty }a_{n}(x-b)^{n}.}  [f(x)=\sum
      _{n=0}^{\infty }a_{n}(x-b)^{n}.]
Differentiating by x the above formula n times, then setting x = b gives:
             f  ( n )   ( b )   n !    =  a  n     {\displaystyle {\frac {f^{
      (n)}(b)}{n!}}=a_{n}}  [{\frac {f^{(n)}(b)}{n!}}=a_{n}]
and so the power series expansion agrees with the Taylor series. Thus a
function is analytic in an open disc centred at b if and only if its Taylor
series converges to the value of the function at each point of the disc.
If f (x) is equal to its Taylor series for all x in the complex plane, it is
called entire. The polynomials, exponential_function ex, and the trigonometric
functions sine and cosine, are examples of entire functions. Examples of
functions that are not entire include the square_root, the logarithm, the
trigonometric_function tangent, and its inverse, arctan. For these functions
the Taylor series do not converge if x is far from b. That is, the Taylor
series diverges at x if the distance between x and b is larger than the radius
of_convergence. The Taylor series can be used to calculate the value of an
entire function at every point, if the value of the function, and of all of its
derivatives, are known at a single point.
Uses of the Taylor series for analytic functions include:
   1. The partial sums (the Taylor_polynomials) of the series can be used as
      approximations of the function. These approximations are good if
      sufficiently many terms are included.
   2. Differentiation and integration of power series can be performed term by
      term and is hence particularly easy.
   3. An analytic_function is uniquely extended to a holomorphic_function on an
      open_disk in the complex_plane. This makes the machinery of complex
      analysis available.
   4. The (truncated) series can be used to compute function values
      numerically, (often by recasting the polynomial into the Chebyshev_form
      and evaluating it with the Clenshaw_algorithm).
   5. Algebraic operations can be done readily on the power series
      representation; for instance, Euler's_formula follows from Taylor series
      expansions for trigonometric and exponential functions. This result is of
      fundamental importance in such fields as harmonic_analysis.
   6. Approximations using the first few terms of a Taylor series can make
      otherwise unsolvable problems possible for a restricted domain; this
      approach is often used in physics.
***** Approximation error and convergence[edit] *****
Main article: Taylor's_theorem
The sine function (blue) is closely approximated by its Taylor polynomial of
degree 7 (pink) for a full period centered at the origin.
The Taylor polynomials for log(1 + x) only provide accurate approximations in
the range â1 < x â¤ 1. For x > 1, Taylor polynomials of higher degree
provide worse approximations.
The Taylor approximations for log(1 + x) (black). For x > 1, the approximations
diverge.
Pictured on the right is an accurate approximation of sin x around the point x
= 0. The pink curve is a polynomial of degree seven:
         sin &#x2061;  ( x )  &#x2248; x &#x2212;    x  3    3 !    +    x  5
      5 !    &#x2212;    x  7    7 !    .    {\displaystyle \sin \left
      (x\right)\approx x-{\frac {x^{3}}{3!}}+{\frac {x^{5}}{5!}}-{\frac {x^{7}}
      {7!}}.\!}  [\sin \left(x\right)\approx x-{\frac {x^{3}}{3!}}+{\frac {x^
      {5}}{5!}}-{\frac {x^{7}}{7!}}.\!]
The error in this approximation is no more than |x|9/9!. In particular, for
â1 < x < 1, the error is less than 0.000003.
In contrast, also shown is a picture of the natural logarithm function log(1 +
x) and some of its Taylor_polynomials around a = 0. These approximations
converge to the function only in the region â1 < x â¤ 1; outside of this
region the higher-degree Taylor polynomials are worse approximations for the
function. This is similar to Runge's_phenomenon.[citation_needed]
The error incurred in approximating a function by its nth-degree Taylor
polynomial is called the remainder or residual and is denoted by the function
Rn(x). Taylor's_theorem can be used to obtain a bound on the size of the
remainder.
In general, Taylor series need not be convergent at all. And in fact the set of
functions with a convergent Taylor series is a meager_set in the FrÃ©chet_space
of smooth_functions. And even if the Taylor series of a function f does
converge, its limit need not in general be equal to the value of the function
f (x). For example, the function
         f ( x ) =   {     e  &#x2212;   1  x  2          if&#xA0;  x &#x2260;
      0     0    if&#xA0;  x = 0         {\displaystyle f(x)={\begin{cases}e^{-
      {\frac {1}{x^{2}}}}&{\text{if }}x\neq 0\\0&{\text{if }}x=0\end{cases}}}
      [{\displaystyle f(x)={\begin{cases}e^{-{\frac {1}{x^{2}}}}&{\text{if
      }}x\neq 0\\0&{\text{if }}x=0\end{cases}}}]
is infinitely_differentiable at x = 0, and has all derivatives zero there.
Consequently, the Taylor series of f (x) about x = 0 is identically zero.
However, f (x) is not the zero function, so does not equal its Taylor series
around the origin. Thus, f (x) is an example of a non-analytic_smooth_function.
In real_analysis, this example shows that there are infinitely_differentiable
functions f (x) whose Taylor series are not equal to f (x) even if they
converge. By contrast, the holomorphic_functions studied in complex_analysis
always possess a convergent Taylor series, and even the Taylor series of
meromorphic_functions, which might have singularities, never converge to a
value different from the function itself. The complex function eâ1/z2,
however, does not approach 0 when z approaches 0 along the imaginary axis, so
it is not continuous in the complex plane and its Taylor series is undefined at
0.
More generally, every sequence of real or complex numbers can appear as
coefficients in the Taylor series of an infinitely differentiable function
defined on the real line, a consequence of Borel's_lemma. As a result, the
radius_of_convergence of a Taylor series can be zero. There are even infinitely
differentiable functions defined on the real line whose Taylor series have a
radius of convergence 0 everywhere.[9]
A function cannot be written as a Taylor series centred at a singularity; in
these cases, one can often still achieve a series expansion if one allows also
negative powers of the variable x; see Laurent_series. For example, f (x) =
eâ1/x2 can be written as a Laurent series.
**** Generalization[edit] ****
There is, however, a generalization[10][11] of the Taylor series that does
converge to the value of the function itself for any bounded continuous
function on (0,â), using the calculus of finite_differences. Specifically,
one has the following theorem, due to Einar_Hille, that for any t > 0,
          lim  h &#x2192;  0  +      &#x2211;  n = 0   &#x221E;      t  n    n
      !        &#x0394;  h   n   f ( a )   h  n     = f ( a + t ) .
      {\displaystyle \lim _{h\to 0^{+}}\sum _{n=0}^{\infty }{\frac {t^{n}}{n!}}
      {\frac {\Delta _{h}^{n}f(a)}{h^{n}}}=f(a+t).}  [\lim _{h\to 0^{+}}\sum _
      {n=0}^{\infty }{\frac {t^{n}}{n!}}{\frac {\Delta _{h}^{n}f(a)}{h^{n}}}=f
      (a+t).]
Here În
h is the nth finite difference operator with step size h. The series is
precisely the Taylor series, except that divided differences appear in place of
differentiation: the series is formally similar to the Newton_series. When the
function f is analytic at a, the terms in the series converge to the terms of
the Taylor series, and in this sense generalizes the usual Taylor series.
In general, for any infinite sequence ai, the following power series identity
holds:
          &#x2211;  n = 0   &#x221E;      u  n    n !     &#x0394;  n    a  i
      =  e  &#x2212; u    &#x2211;  j = 0   &#x221E;      u  j    j !     a  i
      + j   .   {\displaystyle \sum _{n=0}^{\infty }{\frac {u^{n}}{n!}}\Delta ^
      {n}a_{i}=e^{-u}\sum _{j=0}^{\infty }{\frac {u^{j}}{j!}}a_{i+j}.}  [\sum _
      {n=0}^{\infty }{\frac {u^{n}}{n!}}\Delta ^{n}a_{i}=e^{-u}\sum _{j=0}^
      {\infty }{\frac {u^{j}}{j!}}a_{i+j}.]
So in particular,
         f ( a + t ) =  lim  h &#x2192;  0  +      e  &#x2212;   t h
      &#x2211;  j = 0   &#x221E;   f ( a + j h )     (   t h   )   j    j !
      .   {\displaystyle f(a+t)=\lim _{h\to 0^{+}}e^{-{\frac {t}{h}}}\sum _
      {j=0}^{\infty }f(a+jh){\frac {\left({\frac {t}{h}}\right)^{j}}{j!}}.}  [
      {\displaystyle f(a+t)=\lim _{h\to 0^{+}}e^{-{\frac {t}{h}}}\sum _{j=0}^
      {\infty }f(a+jh){\frac {\left({\frac {t}{h}}\right)^{j}}{j!}}.}]
The series on the right is the expectation_value of f (a + X), where X is a
Poisson-distributed random_variable that takes the value jh with probability
eât/hÂ·(t/h)j/j!. Hence,
         f ( a + t ) =  lim  h &#x2192;  0  +      &#x222B;  &#x2212; &#x221E;
      &#x221E;   f ( a + x ) d  P    t h   , h   ( x ) .   {\displaystyle f
      (a+t)=\lim _{h\to 0^{+}}\int _{-\infty }^{\infty }f(a+x)dP_{{\frac {t}
      {h}},h}(x).}  [{\displaystyle f(a+t)=\lim _{h\to 0^{+}}\int _{-\infty }^
      {\infty }f(a+x)dP_{{\frac {t}{h}},h}(x).}]
The law_of_large_numbers implies that the identity holds.[12]
***** List of Maclaurin series of some common functions[edit] *****
See also: List_of_mathematical_series
Several important Maclaurin series expansions follow.[13] All these expansions
are valid for complex arguments x.
**** Exponential function[edit] ****
The exponential_function ex (in blue), and the sum of the first n + 1 terms of
its Taylor series at 0 (in red).
The exponential_function      e  x     {\displaystyle e^{x}}  [e^{x}] (with
base e) has Maclaurin series
          e  x   =  &#x2211;  n = 0   &#x221E;      x  n    n !    = 1 + x +
      x  2    2 !    +    x  3    3 !    + &#x22EF;   {\displaystyle e^{x}=\sum
      _{n=0}^{\infty }{\frac {x^{n}}{n!}}=1+x+{\frac {x^{2}}{2!}}+{\frac {x^
      {3}}{3!}}+\cdots }  [{\displaystyle e^{x}=\sum _{n=0}^{\infty }{\frac {x^
      {n}}{n!}}=1+x+{\frac {x^{2}}{2!}}+{\frac {x^{3}}{3!}}+\cdots }].
It converges for all x.
**** Natural logarithm[edit] ****
The natural_logarithm (with base e) has Maclaurin series
             log &#x2061; ( 1 &#x2212; x )    = &#x2212;  &#x2211;  n = 1
      &#x221E;      x  n   n   = &#x2212; x &#x2212;    x  2   2   &#x2212;
      x  3   3   &#x2212; &#x22EF; ,     log &#x2061; ( 1 + x )    =  &#x2211;
      n = 1   &#x221E;   ( &#x2212; 1  )  n + 1      x  n   n   = x &#x2212;
      x  2   2   +    x  3   3   &#x2212; &#x22EF; .       {\displaystyle
      {\begin{aligned}\log(1-x)&=-\sum _{n=1}^{\infty }{\frac {x^{n}}{n}}=-x-
      {\frac {x^{2}}{2}}-{\frac {x^{3}}{3}}-\cdots ,\\\log(1+x)&=\sum _{n=1}^
      {\infty }(-1)^{n+1}{\frac {x^{n}}{n}}=x-{\frac {x^{2}}{2}}+{\frac {x^{3}}
      {3}}-\cdots .\end{aligned}}}  [{\displaystyle {\begin{aligned}\log(1-
      x)&=-\sum _{n=1}^{\infty }{\frac {x^{n}}{n}}=-x-{\frac {x^{2}}{2}}-{\frac
      {x^{3}}{3}}-\cdots ,\\\log(1+x)&=\sum _{n=1}^{\infty }(-1)^{n+1}{\frac
      {x^{n}}{n}}=x-{\frac {x^{2}}{2}}+{\frac {x^{3}}{3}}-\cdots .\end
      {aligned}}}]
They converge for      |  x  |  < 1   {\displaystyle |x|<1}  [|x|<1]. Also log
(1-x) converges for x=-1 and log(1+x) converges for x=1.
**** Geometric series[edit] ****
The geometric_series and its derivatives have Maclaurin series
               1  1 &#x2212; x       =  &#x2211;  n = 0   &#x221E;    x  n
      1  ( 1 &#x2212; x  )  2         =  &#x2211;  n = 1   &#x221E;   n  x  n
      &#x2212; 1         1  ( 1 &#x2212; x  )  3         =  &#x2211;  n = 2
      &#x221E;      ( n &#x2212; 1 ) n  2    x  n &#x2212; 2   .
      {\displaystyle {\begin{aligned}{\frac {1}{1-x}}&=\sum _{n=0}^{\infty }x^
      {n}\\{\frac {1}{(1-x)^{2}}}&=\sum _{n=1}^{\infty }nx^{n-1}\\{\frac {1}{
      (1-x)^{3}}}&=\sum _{n=2}^{\infty }{\frac {(n-1)n}{2}}x^{n-2}.\end
      {aligned}}}  [{\displaystyle {\begin{aligned}{\frac {1}{1-x}}&=\sum _
      {n=0}^{\infty }x^{n}\\{\frac {1}{(1-x)^{2}}}&=\sum _{n=1}^{\infty }nx^{n-
      1}\\{\frac {1}{(1-x)^{3}}}&=\sum _{n=2}^{\infty }{\frac {(n-1)n}{2}}x^{n-
      2}.\end{aligned}}}]
All are convergent for      |  x  |  < 1   {\displaystyle |x|<1}  [|x|<1].
These are special cases of the binomial_series given in the next section.
**** Binomial series[edit] ****
The binomial_series is the power series
         ( 1 + x  )  &#x03B1;   =  &#x2211;  n = 0   &#x221E;      (   &#x03B1;
      n   )     x  n     {\displaystyle (1+x)^{\alpha }=\sum _{n=0}^{\infty }
      {\binom {\alpha }{n}}x^{n}}  [{\displaystyle (1+x)^{\alpha }=\sum _{n=0}^
      {\infty }{\binom {\alpha }{n}}x^{n}}]
whose coefficients are the generalized binomial_coefficients
            (   &#x03B1; n   )    =  &#x220F;  k = 1   n      &#x03B1; &#x2212;
      k + 1  k   =    &#x03B1; ( &#x03B1; &#x2212; 1 ) &#x22EF; ( &#x03B1;
      &#x2212; n + 1 )   n !    .   {\displaystyle {\binom {\alpha }{n}}=\prod
      _{k=1}^{n}{\frac {\alpha -k+1}{k}}={\frac {\alpha (\alpha -1)\cdots
      (\alpha -n+1)}{n!}}.}  [{\displaystyle {\binom {\alpha }{n}}=\prod _
      {k=1}^{n}{\frac {\alpha -k+1}{k}}={\frac {\alpha (\alpha -1)\cdots
      (\alpha -n+1)}{n!}}.}]
(If  n = 0, this product is an empty_product and has value 1.) It converges for
|  x  |  < 1   {\displaystyle |x|<1}  [|x|<1] for any real or complex number
Î±.
When Î± = â1, this is essentially the infinite geometric series mentioned in
the previous section. The special cases Î± = 1/2 and Î± = â1/2 give the
square_root function and its inverse:
             ( 1 + x  )   1 2       = 1 +    1 2    x &#x2212;    1 8     x  2
      +    1 16     x  3   &#x2212;    5 128     x  4   +    7 256     x  5
      &#x2212; &#x2026; ,     ( 1 + x  )  &#x2212;   1 2        = 1 &#x2212;
      1 2    x +    3 8     x  2   &#x2212;    5 16     x  3   +    35 128
      x  4   &#x2212;    63 256     x  5   + &#x2026; .       {\displaystyle
      {\begin{aligned}(1+x)^{\frac {1}{2}}&=1+{\tfrac {1}{2}}x-{\tfrac {1}
      {8}}x^{2}+{\tfrac {1}{16}}x^{3}-{\tfrac {5}{128}}x^{4}+{\tfrac {7}
      {256}}x^{5}-\ldots ,\\(1+x)^{-{\frac {1}{2}}}&=1-{\tfrac {1}{2}}x+{\tfrac
      {3}{8}}x^{2}-{\tfrac {5}{16}}x^{3}+{\tfrac {35}{128}}x^{4}-{\tfrac {63}
      {256}}x^{5}+\ldots .\end{aligned}}}  [{\displaystyle {\begin{aligned}
      (1+x)^{\frac {1}{2}}&=1+{\tfrac {1}{2}}x-{\tfrac {1}{8}}x^{2}+{\tfrac {1}
      {16}}x^{3}-{\tfrac {5}{128}}x^{4}+{\tfrac {7}{256}}x^{5}-\ldots ,\\(1+x)^
      {-{\frac {1}{2}}}&=1-{\tfrac {1}{2}}x+{\tfrac {3}{8}}x^{2}-{\tfrac {5}
      {16}}x^{3}+{\tfrac {35}{128}}x^{4}-{\tfrac {63}{256}}x^{5}+\ldots .\end
      {aligned}}}]
When only the linear_term is retained, this simplifies to the binomial
approximation.
**** Trigonometric functions[edit] ****
The usual trigonometric_functions and their inverses have the following
Maclaurin series:
             sin &#x2061; x    =  &#x2211;  n = 0   &#x221E;      ( &#x2212; 1
      )  n     ( 2 n + 1 ) !     x  2 n + 1       = x &#x2212;    x  3    3 !
      +    x  5    5 !    &#x2212; &#x22EF;     for all&#xA0;  x     cos
      &#x2061; x    =  &#x2211;  n = 0   &#x221E;      ( &#x2212; 1  )  n
      ( 2 n ) !     x  2 n       = 1 &#x2212;    x  2    2 !    +    x  4    4
      !    &#x2212; &#x22EF;     for all&#xA0;  x     tan &#x2061; x    =
      &#x2211;  n = 1   &#x221E;       B  2 n   ( &#x2212; 4  )  n    (  1
      &#x2212;  4  n    )    ( 2 n ) !     x  2 n &#x2212; 1       = x +    x
      3   3   +    2  x  5    15   + &#x22EF;     for&#xA0;   |  x  |  <
      &#x03C0; 2       sec &#x2061; x    =  &#x2211;  n = 0   &#x221E;
      ( &#x2212; 1  )  n    E  2 n     ( 2 n ) !     x  2 n       = 1 +    x  2
      2   +    5  x  4    24   + &#x22EF;     for&#xA0;   |  x  |  <   &#x03C0;
      2       arcsin &#x2061; x    =  &#x2211;  n = 0   &#x221E;      ( 2 n ) !
      4  n   ( n !  )  2   ( 2 n + 1 )     x  2 n + 1       = x +    x  3   6
      +    3  x  5    40   + &#x22EF;     for&#xA0;   |  x  |  &#x2264; 1
      arccos &#x2061; x    =   &#x03C0; 2   &#x2212; arcsin &#x2061; x       =
      &#x03C0; 2   &#x2212;  &#x2211;  n = 0   &#x221E;      ( 2 n ) !    4  n
      ( n !  )  2   ( 2 n + 1 )     x  2 n + 1       =   &#x03C0; 2   &#x2212;
      x &#x2212;    x  3   6   &#x2212;    3  x  5    40   &#x2212; &#x22EF;
      for&#xA0;   |  x  |  &#x2264; 1     arctan &#x2061; x    =  &#x2211;  n =
      0   &#x221E;      ( &#x2212; 1  )  n     2 n + 1     x  2 n + 1       = x
      &#x2212;    x  3   3   +    x  5   5   &#x2212; &#x22EF;     for&#xA0;
      |  x  |  &#x2264; 1 , &#xA0; x &#x2260; &#x00B1; i       {\displaystyle
      {\begin{aligned}\sin x&=\sum _{n=0}^{\infty }{\frac {(-1)^{n}}{
      (2n+1)!}}x^{2n+1}&&=x-{\frac {x^{3}}{3!}}+{\frac {x^{5}}{5!}}-\cdots &&
      {\text{for all }}x\\[6pt]\cos x&=\sum _{n=0}^{\infty }{\frac {(-1)^{n}}{
      (2n)!}}x^{2n}&&=1-{\frac {x^{2}}{2!}}+{\frac {x^{4}}{4!}}-\cdots &&{\text
      {for all }}x\\[6pt]\tan x&=\sum _{n=1}^{\infty }{\frac {B_{2n}(-4)^
      {n}\left(1-4^{n}\right)}{(2n)!}}x^{2n-1}&&=x+{\frac {x^{3}}{3}}+{\frac
      {2x^{5}}{15}}+\cdots &&{\text{for }}|x|<{\frac {\pi }{2}}\\[6pt]\sec
      x&=\sum _{n=0}^{\infty }{\frac {(-1)^{n}E_{2n}}{(2n)!}}x^{2n}&&=1+{\frac
      {x^{2}}{2}}+{\frac {5x^{4}}{24}}+\cdots &&{\text{for }}|x|<{\frac {\pi }
      {2}}\\[6pt]\arcsin x&=\sum _{n=0}^{\infty }{\frac {(2n)!}{4^{n}(n!)^{2}
      (2n+1)}}x^{2n+1}&&=x+{\frac {x^{3}}{6}}+{\frac {3x^{5}}{40}}+\cdots &&
      {\text{for }}|x|\leq 1\\[6pt]\arccos x&={\frac {\pi }{2}}-\arcsin x\\&=
      {\frac {\pi }{2}}-\sum _{n=0}^{\infty }{\frac {(2n)!}{4^{n}(n!)^{2}
      (2n+1)}}x^{2n+1}&&={\frac {\pi }{2}}-x-{\frac {x^{3}}{6}}-{\frac {3x^{5}}
      {40}}-\cdots &&{\text{for }}|x|\leq 1\\[6pt]\arctan x&=\sum _{n=0}^
      {\infty }{\frac {(-1)^{n}}{2n+1}}x^{2n+1}&&=x-{\frac {x^{3}}{3}}+{\frac
      {x^{5}}{5}}-\cdots &&{\text{for }}|x|\leq 1,\ x\neq \pm i\end{aligned}}}
      [{\displaystyle {\begin{aligned}\sin x&=\sum _{n=0}^{\infty }{\frac {(-
      1)^{n}}{(2n+1)!}}x^{2n+1}&&=x-{\frac {x^{3}}{3!}}+{\frac {x^{5}}{5!}}-
      \cdots &&{\text{for all }}x\\[6pt]\cos x&=\sum _{n=0}^{\infty }{\frac {(-
      1)^{n}}{(2n)!}}x^{2n}&&=1-{\frac {x^{2}}{2!}}+{\frac {x^{4}}{4!}}-\cdots
      &&{\text{for all }}x\\[6pt]\tan x&=\sum _{n=1}^{\infty }{\frac {B_{2n}(-
      4)^{n}\left(1-4^{n}\right)}{(2n)!}}x^{2n-1}&&=x+{\frac {x^{3}}{3}}+{\frac
      {2x^{5}}{15}}+\cdots &&{\text{for }}|x|<{\frac {\pi }{2}}\\[6pt]\sec
      x&=\sum _{n=0}^{\infty }{\frac {(-1)^{n}E_{2n}}{(2n)!}}x^{2n}&&=1+{\frac
      {x^{2}}{2}}+{\frac {5x^{4}}{24}}+\cdots &&{\text{for }}|x|<{\frac {\pi }
      {2}}\\[6pt]\arcsin x&=\sum _{n=0}^{\infty }{\frac {(2n)!}{4^{n}(n!)^{2}
      (2n+1)}}x^{2n+1}&&=x+{\frac {x^{3}}{6}}+{\frac {3x^{5}}{40}}+\cdots &&
      {\text{for }}|x|\leq 1\\[6pt]\arccos x&={\frac {\pi }{2}}-\arcsin x\\&=
      {\frac {\pi }{2}}-\sum _{n=0}^{\infty }{\frac {(2n)!}{4^{n}(n!)^{2}
      (2n+1)}}x^{2n+1}&&={\frac {\pi }{2}}-x-{\frac {x^{3}}{6}}-{\frac {3x^{5}}
      {40}}-\cdots &&{\text{for }}|x|\leq 1\\[6pt]\arctan x&=\sum _{n=0}^
      {\infty }{\frac {(-1)^{n}}{2n+1}}x^{2n+1}&&=x-{\frac {x^{3}}{3}}+{\frac
      {x^{5}}{5}}-\cdots &&{\text{for }}|x|\leq 1,\ x\neq \pm i\end{aligned}}}]
All angles are expressed in radians. The numbers Bk appearing in the expansions
of tan x are the Bernoulli_numbers. The Ek in the expansion of sec x are Euler
numbers.
**** Hyperbolic functions[edit] ****
The hyperbolic_functions have Maclaurin series closely related to the series
for the corresponding trigonometric functions:
             sinh &#x2061; x    =  &#x2211;  n = 0   &#x221E;      x  2 n + 1
      ( 2 n + 1 ) !        = x +    x  3    3 !    +    x  5    5 !    +
      &#x22EF;     for all&#xA0;  x     cosh &#x2061; x    =  &#x2211;  n = 0
      &#x221E;      x  2 n    ( 2 n ) !        = 1 +    x  2    2 !    +    x
      4    4 !    + &#x22EF;     for all&#xA0;  x     tanh &#x2061; x    =
      &#x2211;  n = 1   &#x221E;       B  2 n    4  n    (   4  n   &#x2212; 1
      )    ( 2 n ) !     x  2 n &#x2212; 1       = x &#x2212;    x  3   3   +
      2  x  5    15   &#x2212;    17  x  7    315   + &#x22EF;     for&#xA0;
      |  x  |  <   &#x03C0; 2       arsinh &#x2061; x    =  &#x2211;  n = 0
      &#x221E;      ( &#x2212; 1  )  n   ( 2 n ) !    4  n   ( n !  )  2   ( 2
      n + 1 )     x  2 n + 1         for&#xA0;   |  x  |  &#x2264; 1     artanh
      &#x2061; x    =  &#x2211;  n = 0   &#x221E;      x  2 n + 1    2 n + 1
      for&#xA0;   |  x  |  &#x2264; 1 , &#xA0; x &#x2260; &#x00B1; 1
      {\displaystyle {\begin{aligned}\sinh x&=\sum _{n=0}^{\infty }{\frac {x^
      {2n+1}}{(2n+1)!}}&&=x+{\frac {x^{3}}{3!}}+{\frac {x^{5}}{5!}}+\cdots &&
      {\text{for all }}x\\[6pt]\cosh x&=\sum _{n=0}^{\infty }{\frac {x^{2n}}{
      (2n)!}}&&=1+{\frac {x^{2}}{2!}}+{\frac {x^{4}}{4!}}+\cdots &&{\text{for
      all }}x\\[6pt]\tanh x&=\sum _{n=1}^{\infty }{\frac {B_{2n}4^{n}\left(4^
      {n}-1\right)}{(2n)!}}x^{2n-1}&&=x-{\frac {x^{3}}{3}}+{\frac {2x^{5}}
      {15}}-{\frac {17x^{7}}{315}}+\cdots &&{\text{for }}|x|<{\frac {\pi }
      {2}}\\[6pt]\operatorname {arsinh} x&=\sum _{n=0}^{\infty }{\frac {(-1)^
      {n}(2n)!}{4^{n}(n!)^{2}(2n+1)}}x^{2n+1}&&&&{\text{for }}|x|\leq 1\\
      [6pt]\operatorname {artanh} x&=\sum _{n=0}^{\infty }{\frac {x^{2n+1}}
      {2n+1}}&&&&{\text{for }}|x|\leq 1,\ x\neq \pm 1\end{aligned}}}  [
      {\displaystyle {\begin{aligned}\sinh x&=\sum _{n=0}^{\infty }{\frac {x^
      {2n+1}}{(2n+1)!}}&&=x+{\frac {x^{3}}{3!}}+{\frac {x^{5}}{5!}}+\cdots &&
      {\text{for all }}x\\[6pt]\cosh x&=\sum _{n=0}^{\infty }{\frac {x^{2n}}{
      (2n)!}}&&=1+{\frac {x^{2}}{2!}}+{\frac {x^{4}}{4!}}+\cdots &&{\text{for
      all }}x\\[6pt]\tanh x&=\sum _{n=1}^{\infty }{\frac {B_{2n}4^{n}\left(4^
      {n}-1\right)}{(2n)!}}x^{2n-1}&&=x-{\frac {x^{3}}{3}}+{\frac {2x^{5}}
      {15}}-{\frac {17x^{7}}{315}}+\cdots &&{\text{for }}|x|<{\frac {\pi }
      {2}}\\[6pt]\operatorname {arsinh} x&=\sum _{n=0}^{\infty }{\frac {(-1)^
      {n}(2n)!}{4^{n}(n!)^{2}(2n+1)}}x^{2n+1}&&&&{\text{for }}|x|\leq 1\\
      [6pt]\operatorname {artanh} x&=\sum _{n=0}^{\infty }{\frac {x^{2n+1}}
      {2n+1}}&&&&{\text{for }}|x|\leq 1,\ x\neq \pm 1\end{aligned}}}]
The numbers Bk appearing in the series for tanh x are the Bernoulli_numbers.
***** Calculation of Taylor series[edit] *****
Several methods exist for the calculation of Taylor series of a large number of
functions. One can attempt to use the definition of the Taylor series, though
this often requires generalizing the form of the coefficients according to a
readily apparent pattern. Alternatively, one can use manipulations such as
substitution, multiplication or division, addition or subtraction of standard
Taylor series to construct the Taylor series of a function, by virtue of Taylor
series being power series. In some cases, one can also derive the Taylor series
by repeatedly applying integration_by_parts. Particularly convenient is the use
of computer_algebra_systems to calculate Taylor series.
**** First example[edit] ****
In order to compute the 7th degree Maclaurin polynomial for the function
         f ( x ) = log &#x2061; ( cos &#x2061; x ) ,  x &#x2208;  (  &#x2212;
      &#x03C0; 2   ,   &#x03C0; 2    )    {\displaystyle f(x)=\log(\cos
      x),\quad x\in \left(-{\frac {\pi }{2}},{\frac {\pi }{2}}\right)}  [
      {\displaystyle f(x)=\log(\cos x),\quad x\in \left(-{\frac {\pi }{2}},
      {\frac {\pi }{2}}\right)}] ,
one may first rewrite the function as
         f ( x ) = log &#x2061;   (   1 + ( cos &#x2061; x &#x2212; 1 )   )
      {\displaystyle f(x)=\log {\bigl (}1+(\cos x-1){\bigr )}\!}  [
      {\displaystyle f(x)=\log {\bigl (}1+(\cos x-1){\bigr )}\!}].
The Taylor series for the natural logarithm is (using the big_O_notation)
         log &#x2061; ( 1 + x ) = x &#x2212;    x  2   2   +    x  3   3   +  O
      (  x  4   )     {\displaystyle \log(1+x)=x-{\frac {x^{2}}{2}}+{\frac {x^
      {3}}{3}}+{O}\left(x^{4}\right)\!}  [{\displaystyle \log(1+x)=x-{\frac {x^
      {2}}{2}}+{\frac {x^{3}}{3}}+{O}\left(x^{4}\right)\!}]
and for the cosine function
         cos &#x2061; x &#x2212; 1 = &#x2212;    x  2   2   +    x  4   24
      &#x2212;    x  6   720   +  O   (  x  8   )     {\displaystyle \cos x-1=-
      {\frac {x^{2}}{2}}+{\frac {x^{4}}{24}}-{\frac {x^{6}}{720}}+{O}\left(x^
      {8}\right)\!}  [{\displaystyle \cos x-1=-{\frac {x^{2}}{2}}+{\frac {x^
      {4}}{24}}-{\frac {x^{6}}{720}}+{O}\left(x^{8}\right)\!}].
The latter series expansion has a zero constant_term, which enables us to
substitute the second series into the first one and to easily omit terms of
higher order than the 7th degree by using the big O notation:
             f ( x )    = log &#x2061;   (   1 + ( cos &#x2061; x &#x2212; 1 )
      )         = ( cos &#x2061; x &#x2212; 1 ) &#x2212;    1 2    ( cos
      &#x2061; x &#x2212; 1  )  2   +    1 3    ( cos &#x2061; x &#x2212; 1  )
      3   +  O   (  ( cos &#x2061; x &#x2212; 1  )  4    )        =
      (  &#x2212;    x  2   2   +    x  4   24   &#x2212;    x  6   720   +  O
      (  x  8   )   )  &#x2212;   1 2     (  &#x2212;    x  2   2   +    x  4
      24   +  O   (  x  6   )   )   2   +   1 3     (  &#x2212;    x  2   2   +
      O  (  x  4   )   )   3   +  O   (  x  8   )        = &#x2212;    x  2   2
      +    x  4   24   &#x2212;    x  6   720   &#x2212;    x  4   8   +    x
      6   48   &#x2212;    x  6   24   + O  (  x  8   )        = &#x2212;    x
      2   2   &#x2212;    x  4   12   &#x2212;    x  6   45   + O  (  x  8   )
      .        {\displaystyle {\begin{aligned}f(x)&=\log {\bigl (}1+(\cos x-1)
      {\bigr )}\\&=(\cos x-1)-{\tfrac {1}{2}}(\cos x-1)^{2}+{\tfrac {1}{3}}
      (\cos x-1)^{3}+{O}\left((\cos x-1)^{4}\right)\\&=\left(-{\frac {x^{2}}
      {2}}+{\frac {x^{4}}{24}}-{\frac {x^{6}}{720}}+{O}\left(x^
      {8}\right)\right)-{\frac {1}{2}}\left(-{\frac {x^{2}}{2}}+{\frac {x^{4}}
      {24}}+{O}\left(x^{6}\right)\right)^{2}+{\frac {1}{3}}\left(-{\frac {x^
      {2}}{2}}+O\left(x^{4}\right)\right)^{3}+{O}\left(x^{8}\right)\\&=-{\frac
      {x^{2}}{2}}+{\frac {x^{4}}{24}}-{\frac {x^{6}}{720}}-{\frac {x^{4}}{8}}+
      {\frac {x^{6}}{48}}-{\frac {x^{6}}{24}}+O\left(x^{8}\right)\\&=-{\frac
      {x^{2}}{2}}-{\frac {x^{4}}{12}}-{\frac {x^{6}}{45}}+O\left(x^
      {8}\right).\end{aligned}}\!}  [{\displaystyle {\begin{aligned}f(x)&=\log
      {\bigl (}1+(\cos x-1){\bigr )}\\&=(\cos x-1)-{\tfrac {1}{2}}(\cos x-1)^
      {2}+{\tfrac {1}{3}}(\cos x-1)^{3}+{O}\left((\cos x-1)^{4}\right)\\&=\left
      (-{\frac {x^{2}}{2}}+{\frac {x^{4}}{24}}-{\frac {x^{6}}{720}}+{O}\left(x^
      {8}\right)\right)-{\frac {1}{2}}\left(-{\frac {x^{2}}{2}}+{\frac {x^{4}}
      {24}}+{O}\left(x^{6}\right)\right)^{2}+{\frac {1}{3}}\left(-{\frac {x^
      {2}}{2}}+O\left(x^{4}\right)\right)^{3}+{O}\left(x^{8}\right)\\&=-{\frac
      {x^{2}}{2}}+{\frac {x^{4}}{24}}-{\frac {x^{6}}{720}}-{\frac {x^{4}}{8}}+
      {\frac {x^{6}}{48}}-{\frac {x^{6}}{24}}+O\left(x^{8}\right)\\&=-{\frac
      {x^{2}}{2}}-{\frac {x^{4}}{12}}-{\frac {x^{6}}{45}}+O\left(x^
      {8}\right).\end{aligned}}\!}]
Since the cosine is an even_function, the coefficients for all the odd powers
x, x3, x5, x7, ... have to be zero.
**** Second example[edit] ****
Suppose we want the Taylor series at 0 of the function
         g ( x ) =    e  x    cos &#x2061; x    .    {\displaystyle g(x)={\frac
      {e^{x}}{\cos x}}.\!}  [g(x)={\frac {e^{x}}{\cos x}}.\!]
We have for the exponential function
          e  x   =  &#x2211;  n = 0   &#x221E;      x  n    n !    = 1 + x +
      x  2    2 !    +    x  3    3 !    +    x  4    4 !    + &#x22EF;
      {\displaystyle e^{x}=\sum _{n=0}^{\infty }{\frac {x^{n}}{n!}}=1+x+{\frac
      {x^{2}}{2!}}+{\frac {x^{3}}{3!}}+{\frac {x^{4}}{4!}}+\cdots \!}  [
      {\displaystyle e^{x}=\sum _{n=0}^{\infty }{\frac {x^{n}}{n!}}=1+x+{\frac
      {x^{2}}{2!}}+{\frac {x^{3}}{3!}}+{\frac {x^{4}}{4!}}+\cdots \!}]
and, as in the first example,
         cos &#x2061; x = 1 &#x2212;    x  2    2 !    +    x  4    4 !
      &#x2212; &#x22EF;    {\displaystyle \cos x=1-{\frac {x^{2}}{2!}}+{\frac
      {x^{4}}{4!}}-\cdots \!}  [{\displaystyle \cos x=1-{\frac {x^{2}}{2!}}+
      {\frac {x^{4}}{4!}}-\cdots \!}]
Assume the power series is
            e  x    cos &#x2061; x    =  c  0   +  c  1   x +  c  2    x  2   +
      c  3    x  3   + &#x22EF;    {\displaystyle {\frac {e^{x}}{\cos x}}=c_
      {0}+c_{1}x+c_{2}x^{2}+c_{3}x^{3}+\cdots \!}  [{\displaystyle {\frac {e^
      {x}}{\cos x}}=c_{0}+c_{1}x+c_{2}x^{2}+c_{3}x^{3}+\cdots \!}]
Then multiplication with the denominator and substitution of the series of the
cosine yields
              e  x      =  (   c  0   +  c  1   x +  c  2    x  2   +  c  3
      x  3   + &#x22EF;  )  cos &#x2061; x       =  (   c  0   +  c  1   x +  c
      2    x  2   +  c  3    x  3   +  c  4    x  4   + &#x22EF;  )   (  1
      &#x2212;    x  2    2 !    +    x  4    4 !    &#x2212; &#x22EF;  )
      =  c  0   &#x2212;    c  0   2    x  2   +    c  0    4 !     x  4   +  c
      1   x &#x2212;    c  1   2    x  3   +    c  1    4 !     x  5   +  c  2
      x  2   &#x2212;    c  2   2    x  4   +    c  2    4 !     x  6   +  c  3
      x  3   &#x2212;    c  3   2    x  5   +    c  3    4 !     x  7   +  c  4
      x  4   + &#x22EF;        {\displaystyle {\begin{aligned}e^{x}&=\left(c_
      {0}+c_{1}x+c_{2}x^{2}+c_{3}x^{3}+\cdots \right)\cos x\\&=\left(c_{0}+c_
      {1}x+c_{2}x^{2}+c_{3}x^{3}+c_{4}x^{4}+\cdots \right)\left(1-{\frac {x^
      {2}}{2!}}+{\frac {x^{4}}{4!}}-\cdots \right)\\&=c_{0}-{\frac {c_{0}}
      {2}}x^{2}+{\frac {c_{0}}{4!}}x^{4}+c_{1}x-{\frac {c_{1}}{2}}x^{3}+{\frac
      {c_{1}}{4!}}x^{5}+c_{2}x^{2}-{\frac {c_{2}}{2}}x^{4}+{\frac {c_{2}}
      {4!}}x^{6}+c_{3}x^{3}-{\frac {c_{3}}{2}}x^{5}+{\frac {c_{3}}{4!}}x^{7}+c_
      {4}x^{4}+\cdots \end{aligned}}\!}  [{\displaystyle {\begin{aligned}e^
      {x}&=\left(c_{0}+c_{1}x+c_{2}x^{2}+c_{3}x^{3}+\cdots \right)\cos
      x\\&=\left(c_{0}+c_{1}x+c_{2}x^{2}+c_{3}x^{3}+c_{4}x^{4}+\cdots
      \right)\left(1-{\frac {x^{2}}{2!}}+{\frac {x^{4}}{4!}}-\cdots
      \right)\\&=c_{0}-{\frac {c_{0}}{2}}x^{2}+{\frac {c_{0}}{4!}}x^{4}+c_{1}x-
      {\frac {c_{1}}{2}}x^{3}+{\frac {c_{1}}{4!}}x^{5}+c_{2}x^{2}-{\frac {c_
      {2}}{2}}x^{4}+{\frac {c_{2}}{4!}}x^{6}+c_{3}x^{3}-{\frac {c_{3}}{2}}x^
      {5}+{\frac {c_{3}}{4!}}x^{7}+c_{4}x^{4}+\cdots \end{aligned}}\!}]
Collecting the terms up to fourth order yields
          e  x   =  c  0   +  c  1   x +  (   c  2   &#x2212;    c  0   2    )
      x  2   +  (   c  3   &#x2212;    c  1   2    )   x  3   +  (   c  4
      &#x2212;    c  2   2   +    c  0    4 !     )   x  4   + &#x22EF;
      {\displaystyle e^{x}=c_{0}+c_{1}x+\left(c_{2}-{\frac {c_{0}}{2}}\right)x^
      {2}+\left(c_{3}-{\frac {c_{1}}{2}}\right)x^{3}+\left(c_{4}-{\frac {c_{2}}
      {2}}+{\frac {c_{0}}{4!}}\right)x^{4}+\cdots \!}  [{\displaystyle e^{x}=c_
      {0}+c_{1}x+\left(c_{2}-{\frac {c_{0}}{2}}\right)x^{2}+\left(c_{3}-{\frac
      {c_{1}}{2}}\right)x^{3}+\left(c_{4}-{\frac {c_{2}}{2}}+{\frac {c_{0}}
      {4!}}\right)x^{4}+\cdots \!}]
The values of      c  i     {\displaystyle c_{i}}  [c_{i}] can be found by
comparison of coefficients with the top expression for      e  x
{\displaystyle e^{x}}  [e^{x}], yielding:
            e  x    cos &#x2061; x    = 1 + x +  x  2   +    2  x  3    3   +
      x  4   2   + &#x22EF; .    {\displaystyle {\frac {e^{x}}{\cos x}}=1+x+x^
      {2}+{\frac {2x^{3}}{3}}+{\frac {x^{4}}{2}}+\cdots .\!}  [{\displaystyle
      {\frac {e^{x}}{\cos x}}=1+x+x^{2}+{\frac {2x^{3}}{3}}+{\frac {x^{4}}
      {2}}+\cdots .\!}]
**** Third example[edit] ****
Here we employ a method called "indirect expansion" to expand the given
function. This method uses the known Taylor expansion of the exponential
function. In order to expand (1 + x)ex as a Taylor series in x, we use the
known Taylor series of function ex:
          e  x   =  &#x2211;  n = 0   &#x221E;      x  n    n !    = 1 + x +
      x  2    2 !    +    x  3    3 !    +    x  4    4 !    + &#x22EF; .
      {\displaystyle e^{x}=\sum _{n=0}^{\infty }{\frac {x^{n}}{n!}}=1+x+{\frac
      {x^{2}}{2!}}+{\frac {x^{3}}{3!}}+{\frac {x^{4}}{4!}}+\cdots .}  [
      {\displaystyle e^{x}=\sum _{n=0}^{\infty }{\frac {x^{n}}{n!}}=1+x+{\frac
      {x^{2}}{2!}}+{\frac {x^{3}}{3!}}+{\frac {x^{4}}{4!}}+\cdots .}]
Thus,
             ( 1 + x )  e  x      =  e  x   + x  e  x   =  &#x2211;  n = 0
      &#x221E;      x  n    n !    +  &#x2211;  n = 0   &#x221E;      x  n + 1
      n !    = 1 +  &#x2211;  n = 1   &#x221E;      x  n    n !    +  &#x2211;
      n = 0   &#x221E;      x  n + 1    n !          = 1 +  &#x2211;  n = 1
      &#x221E;      x  n    n !    +  &#x2211;  n = 1   &#x221E;      x  n
      ( n &#x2212; 1 ) !    = 1 +  &#x2211;  n = 1   &#x221E;    (    1  n !
      +   1  ( n &#x2212; 1 ) !     )   x  n         = 1 +  &#x2211;  n = 1
      &#x221E;      n + 1   n !     x  n         =  &#x2211;  n = 0   &#x221E;
      n + 1   n !     x  n   .       {\displaystyle {\begin{aligned}(1+x)e^
      {x}&=e^{x}+xe^{x}=\sum _{n=0}^{\infty }{\frac {x^{n}}{n!}}+\sum _{n=0}^
      {\infty }{\frac {x^{n+1}}{n!}}=1+\sum _{n=1}^{\infty }{\frac {x^{n}}
      {n!}}+\sum _{n=0}^{\infty }{\frac {x^{n+1}}{n!}}\\&=1+\sum _{n=1}^{\infty
      }{\frac {x^{n}}{n!}}+\sum _{n=1}^{\infty }{\frac {x^{n}}{(n-1)!}}=1+\sum
      _{n=1}^{\infty }\left({\frac {1}{n!}}+{\frac {1}{(n-1)!}}\right)x^
      {n}\\&=1+\sum _{n=1}^{\infty }{\frac {n+1}{n!}}x^{n}\\&=\sum _{n=0}^
      {\infty }{\frac {n+1}{n!}}x^{n}.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}(1+x)e^{x}&=e^{x}+xe^{x}=\sum _{n=0}^{\infty }{\frac {x^{n}}
      {n!}}+\sum _{n=0}^{\infty }{\frac {x^{n+1}}{n!}}=1+\sum _{n=1}^{\infty }
      {\frac {x^{n}}{n!}}+\sum _{n=0}^{\infty }{\frac {x^{n+1}}{n!}}\\&=1+\sum
      _{n=1}^{\infty }{\frac {x^{n}}{n!}}+\sum _{n=1}^{\infty }{\frac {x^{n}}{
      (n-1)!}}=1+\sum _{n=1}^{\infty }\left({\frac {1}{n!}}+{\frac {1}{(n-
      1)!}}\right)x^{n}\\&=1+\sum _{n=1}^{\infty }{\frac {n+1}{n!}}x^
      {n}\\&=\sum _{n=0}^{\infty }{\frac {n+1}{n!}}x^{n}.\end{aligned}}}]
***** Taylor series as definitions[edit] *****
Classically, algebraic_functions are defined by an algebraic equation, and
transcendental_functions (including those discussed above) are defined by some
property that holds for them, such as a differential_equation. For example, the
exponential_function is the function which is equal to its own derivative
everywhere, and assumes the value 1 at the origin. However, one may equally
well define an analytic_function by its Taylor series.
Taylor series are used to define functions and "operators" in diverse areas of
mathematics. In particular, this is true in areas where the classical
definitions of functions break down. For example, using Taylor series, one may
extend analytic functions to sets of matrices and operators, such as the matrix
exponential or matrix_logarithm.
In other areas, such as formal analysis, it is more convenient to work directly
with the power_series themselves. Thus one may define a solution of a
differential equation as a power series which, one hopes to prove, is the
Taylor series of the desired solution.
***** Taylor series in several variables[edit] *****
The Taylor series may also be generalized to functions of more than one
variable with[14][15]
             T (  x  1   , &#x2026; ,  x  d   )    =  &#x2211;   n  1   = 0
      &#x221E;   &#x22EF;  &#x2211;   n  d   = 0   &#x221E;      (  x  1
      &#x2212;  a  1    )   n  1     &#x22EF; (  x  d   &#x2212;  a  d    )   n
      d        n  1   ! &#x22EF;  n  d   !      (     &#x2202;   n  1   +
      &#x22EF; +  n  d     f   &#x2202;  x  1    n  1     &#x22EF; &#x2202;  x
      d    n  d        )  (  a  1   , &#x2026; ,  a  d   )       = f (  a  1
      , &#x2026; ,  a  d   ) +  &#x2211;  j = 1   d      &#x2202; f (  a  1   ,
      &#x2026; ,  a  d   )   &#x2202;  x  j      (  x  j   &#x2212;  a  j   ) +
      1  2 !     &#x2211;  j = 1   d    &#x2211;  k = 1   d       &#x2202;  2
      f (  a  1   , &#x2026; ,  a  d   )   &#x2202;  x  j   &#x2202;  x  k
      (  x  j   &#x2212;  a  j   ) (  x  k   &#x2212;  a  k   ) +         +   1
      3 !     &#x2211;  j = 1   d    &#x2211;  k = 1   d    &#x2211;  l = 1   d
      &#x2202;  3   f (  a  1   , &#x2026; ,  a  d   )   &#x2202;  x  j
      &#x2202;  x  k   &#x2202;  x  l      (  x  j   &#x2212;  a  j   ) (  x  k
      &#x2212;  a  k   ) (  x  l   &#x2212;  a  l   ) + &#x22EF;
      {\displaystyle {\begin{aligned}T(x_{1},\ldots ,x_{d})&=\sum _{n_{1}=0}^
      {\infty }\cdots \sum _{n_{d}=0}^{\infty }{\frac {(x_{1}-a_{1})^{n_
      {1}}\cdots (x_{d}-a_{d})^{n_{d}}}{n_{1}!\cdots n_{d}!}}\,\left({\frac
      {\partial ^{n_{1}+\cdots +n_{d}}f}{\partial x_{1}^{n_{1}}\cdots \partial
      x_{d}^{n_{d}}}}\right)(a_{1},\ldots ,a_{d})\\&=f(a_{1},\ldots ,a_
      {d})+\sum _{j=1}^{d}{\frac {\partial f(a_{1},\ldots ,a_{d})}{\partial x_
      {j}}}(x_{j}-a_{j})+{\frac {1}{2!}}\sum _{j=1}^{d}\sum _{k=1}^{d}{\frac
      {\partial ^{2}f(a_{1},\ldots ,a_{d})}{\partial x_{j}\partial x_{k}}}(x_
      {j}-a_{j})(x_{k}-a_{k})+\\&\qquad \qquad +{\frac {1}{3!}}\sum _{j=1}^
      {d}\sum _{k=1}^{d}\sum _{l=1}^{d}{\frac {\partial ^{3}f(a_{1},\ldots ,a_
      {d})}{\partial x_{j}\partial x_{k}\partial x_{l}}}(x_{j}-a_{j})(x_{k}-a_
      {k})(x_{l}-a_{l})+\cdots \end{aligned}}}  [{\displaystyle {\begin
      {aligned}T(x_{1},\ldots ,x_{d})&=\sum _{n_{1}=0}^{\infty }\cdots \sum _
      {n_{d}=0}^{\infty }{\frac {(x_{1}-a_{1})^{n_{1}}\cdots (x_{d}-a_{d})^{n_
      {d}}}{n_{1}!\cdots n_{d}!}}\,\left({\frac {\partial ^{n_{1}+\cdots +n_
      {d}}f}{\partial x_{1}^{n_{1}}\cdots \partial x_{d}^{n_{d}}}}\right)(a_
      {1},\ldots ,a_{d})\\&=f(a_{1},\ldots ,a_{d})+\sum _{j=1}^{d}{\frac
      {\partial f(a_{1},\ldots ,a_{d})}{\partial x_{j}}}(x_{j}-a_{j})+{\frac
      {1}{2!}}\sum _{j=1}^{d}\sum _{k=1}^{d}{\frac {\partial ^{2}f(a_{1},\ldots
      ,a_{d})}{\partial x_{j}\partial x_{k}}}(x_{j}-a_{j})(x_{k}-a_
      {k})+\\&\qquad \qquad +{\frac {1}{3!}}\sum _{j=1}^{d}\sum _{k=1}^{d}\sum
      _{l=1}^{d}{\frac {\partial ^{3}f(a_{1},\ldots ,a_{d})}{\partial x_
      {j}\partial x_{k}\partial x_{l}}}(x_{j}-a_{j})(x_{k}-a_{k})(x_{l}-a_
      {l})+\cdots \end{aligned}}}]
For example, for a function     f ( x , y )   {\displaystyle f(x,y)}  [f(x,y)]
that depends on two variables, x and y, the Taylor series to second order about
the point (a, b) is
         f ( a , b ) + ( x &#x2212; a )  f  x   ( a , b ) + ( y &#x2212; b )  f
      y   ( a , b ) +   1  2 !      (   ( x &#x2212; a  )  2    f  x x   ( a ,
      b ) + 2 ( x &#x2212; a ) ( y &#x2212; b )  f  x y   ( a , b ) + ( y
      &#x2212; b  )  2    f  y y   ( a , b )   )     {\displaystyle f(a,b)+(x-
      a)f_{x}(a,b)+(y-b)f_{y}(a,b)+{\frac {1}{2!}}{\Big (}(x-a)^{2}f_{xx}
      (a,b)+2(x-a)(y-b)f_{xy}(a,b)+(y-b)^{2}f_{yy}(a,b){\Big )}}  [
      {\displaystyle f(a,b)+(x-a)f_{x}(a,b)+(y-b)f_{y}(a,b)+{\frac {1}{2!}}
      {\Big (}(x-a)^{2}f_{xx}(a,b)+2(x-a)(y-b)f_{xy}(a,b)+(y-b)^{2}f_{yy}(a,b)
      {\Big )}}]
where the subscripts denote the respective partial_derivatives.
A second-order Taylor series expansion of a scalar-valued function of more than
one variable can be written compactly as
         T (  x  ) = f (  a  ) + (  x  &#x2212;  a   )   T    D f (  a  ) +   1
      2 !    (  x  &#x2212;  a   )   T     {   D  2   f (  a  )  }  (  x
      &#x2212;  a  ) + &#x22EF; ,   {\displaystyle T(\mathbf {x} )=f(\mathbf
      {a} )+(\mathbf {x} -\mathbf {a} )^{\mathsf {T}}Df(\mathbf {a} )+{\frac
      {1}{2!}}(\mathbf {x} -\mathbf {a} )^{\mathsf {T}}\left\{D^{2}f(\mathbf
      {a} )\right\}(\mathbf {x} -\mathbf {a} )+\cdots ,}  [{\displaystyle T
      (\mathbf {x} )=f(\mathbf {a} )+(\mathbf {x} -\mathbf {a} )^{\mathsf
      {T}}Df(\mathbf {a} )+{\frac {1}{2!}}(\mathbf {x} -\mathbf {a} )^{\mathsf
      {T}}\left\{D^{2}f(\mathbf {a} )\right\}(\mathbf {x} -\mathbf {a} )+\cdots
      ,}]
where D f (a) is the gradient of f evaluated at x = a and D2 f (a) is the
Hessian_matrix. Applying the multi-index_notation the Taylor series for several
variables becomes
         T (  x  ) =  &#x2211;   |  &#x03B1;  |  &#x2265; 0      (  x  &#x2212;
      a   )  &#x03B1;     &#x03B1; !     (     &#x2202;   &#x03B1;    f  )
      (  a  ) ,   {\displaystyle T(\mathbf {x} )=\sum _{|\alpha |\geq 0}{\frac
      {(\mathbf {x} -\mathbf {a} )^{\alpha }}{\alpha !}}\left({\mathrm
      {\partial } ^{\alpha }}f\right)(\mathbf {a} ),}  [{\displaystyle T
      (\mathbf {x} )=\sum _{|\alpha |\geq 0}{\frac {(\mathbf {x} -\mathbf {a}
      )^{\alpha }}{\alpha !}}\left({\mathrm {\partial } ^{\alpha }}f\right)
      (\mathbf {a} ),}]
which is to be understood as a still more abbreviated multi-index version of
the first equation of this paragraph, with a full analogy to the single
variable case.
**** Example[edit] ****
Second-order Taylor series approximation (in orange) of a function f (x,y) = ex
log(1 + y) around the origin.
In order to compute a second-order Taylor series expansion around point (a, b)
= (0, 0) of the function
         f ( x , y ) =  e  x   log &#x2061; ( 1 + y ) ,   {\displaystyle f
      (x,y)=e^{x}\log(1+y),}  [{\displaystyle f(x,y)=e^{x}\log(1+y),}]
one first computes all the necessary partial derivatives:
              f  x      =  e  x   log &#x2061; ( 1 + y )      f  y      =    e
      x    1 + y         f  x x      =  e  x   log &#x2061; ( 1 + y )      f  y
      y      = &#x2212;    e  x    ( 1 + y  )  2           f  x y      =  f  y
      x   =    e  x    1 + y    .       {\displaystyle {\begin{aligned}f_
      {x}&=e^{x}\log(1+y)\\[6pt]f_{y}&={\frac {e^{x}}{1+y}}\\[6pt]f_{xx}&=e^
      {x}\log(1+y)\\[6pt]f_{yy}&=-{\frac {e^{x}}{(1+y)^{2}}}\\[6pt]f_{xy}&=f_
      {yx}={\frac {e^{x}}{1+y}}.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}f_{x}&=e^{x}\log(1+y)\\[6pt]f_{y}&={\frac {e^{x}}{1+y}}\\[6pt]f_
      {xx}&=e^{x}\log(1+y)\\[6pt]f_{yy}&=-{\frac {e^{x}}{(1+y)^{2}}}\\[6pt]f_
      {xy}&=f_{yx}={\frac {e^{x}}{1+y}}.\end{aligned}}}]
Evaluating these derivatives at the origin gives the Taylor coefficients
              f  x   ( 0 , 0 )    = 0      f  y   ( 0 , 0 )    = 1      f  x x
      ( 0 , 0 )    = 0      f  y y   ( 0 , 0 )    = &#x2212; 1      f  x y
      ( 0 , 0 )    =  f  y x   ( 0 , 0 ) = 1.       {\displaystyle {\begin
      {aligned}f_{x}(0,0)&=0\\f_{y}(0,0)&=1\\f_{xx}(0,0)&=0\\f_{yy}(0,0)&=-
      1\\f_{xy}(0,0)&=f_{yx}(0,0)=1.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}f_{x}(0,0)&=0\\f_{y}(0,0)&=1\\f_{xx}(0,0)&=0\\f_{yy}(0,0)&=-
      1\\f_{xy}(0,0)&=f_{yx}(0,0)=1.\end{aligned}}}]
Substituting these values in to the general formula
         T ( x , y ) = f ( a , b ) + ( x &#x2212; a )  f  x   ( a , b ) + ( y
      &#x2212; b )  f  y   ( a , b ) +   1  2 !      (   ( x &#x2212; a  )  2
      f  x x   ( a , b ) + 2 ( x &#x2212; a ) ( y &#x2212; b )  f  x y   ( a ,
      b ) + ( y &#x2212; b  )  2    f  y y   ( a , b )   )   + &#x22EF;
      {\displaystyle T(x,y)=f(a,b)+(x-a)f_{x}(a,b)+(y-b)f_{y}(a,b)+{\frac {1}
      {2!}}{\Big (}(x-a)^{2}f_{xx}(a,b)+2(x-a)(y-b)f_{xy}(a,b)+(y-b)^{2}f_{yy}
      (a,b){\Big )}+\cdots }  [{\displaystyle T(x,y)=f(a,b)+(x-a)f_{x}(a,b)+(y-
      b)f_{y}(a,b)+{\frac {1}{2!}}{\Big (}(x-a)^{2}f_{xx}(a,b)+2(x-a)(y-b)f_
      {xy}(a,b)+(y-b)^{2}f_{yy}(a,b){\Big )}+\cdots }]
produces
             T ( x , y )    = 0 + 0 ( x &#x2212; 0 ) + 1 ( y &#x2212; 0 ) +   1
      2     (   0 ( x &#x2212; 0  )  2   + 2 ( x &#x2212; 0 ) ( y &#x2212; 0 )
      + ( &#x2212; 1 ) ( y &#x2212; 0  )  2     )   + &#x22EF;       = y + x y
      &#x2212;    y  2   2   + &#x22EF;       {\displaystyle {\begin{aligned}T
      (x,y)&=0+0(x-0)+1(y-0)+{\frac {1}{2}}{\Big (}0(x-0)^{2}+2(x-0)(y-0)+(-1)
      (y-0)^{2}{\Big )}+\cdots \\&=y+xy-{\frac {y^{2}}{2}}+\cdots \end
      {aligned}}}  [{\displaystyle {\begin{aligned}T(x,y)&=0+0(x-0)+1(y-0)+
      {\frac {1}{2}}{\Big (}0(x-0)^{2}+2(x-0)(y-0)+(-1)(y-0)^{2}{\Big )}+\cdots
      \\&=y+xy-{\frac {y^{2}}{2}}+\cdots \end{aligned}}}]
Since log(1 + y) is analytic in |y| < 1, we have
          e  x   log &#x2061; ( 1 + y ) = y + x y &#x2212;    y  2   2   +
      &#x22EF; ,   |  y  |  < 1.   {\displaystyle e^{x}\log(1+y)=y+xy-{\frac
      {y^{2}}{2}}+\cdots ,\qquad |y|<1.}  [{\displaystyle e^{x}\log(1+y)=y+xy-
      {\frac {y^{2}}{2}}+\cdots ,\qquad |y|<1.}]
***** Comparison with Fourier series[edit] *****
Main article: Fourier_series
The trigonometric Fourier_series enables one to express a periodic_function (or
a function defined on a closed interval [a,b]) as an infinite sum of
trigonometric_functions (sines and cosines). In this sense, the Fourier series
is analogous to Taylor series, since the latter allows one to express a
function as an infinite sum of powers. Nevertheless, the two series differ from
each other in several relevant issues:
    * The finite truncations of the Taylor series of f (x) about the point x =
      a are all exactly equal to f at a. In contrast, the Fourier series is
      computed by integrating over an entire interval, so there is generally no
      such point where all the finite truncations of the series are exact.
    * The computation of Taylor series requires the knowledge of the function
      on an arbitrary small neighbourhood of a point, whereas the computation
      of the Fourier series requires knowing the function on its whole domain
      interval. In a certain sense one could say that the Taylor series is
      "local" and the Fourier series is "global".
    * The Taylor series is defined for a function which has infinitely many
      derivatives at a single point, whereas the Fourier series is defined for
      any integrable function. In particular, the function could be nowhere
      differentiable. (For example, f (x) could be a Weierstrass_function.)
    * The convergence of both series has very different properties. Even if the
      Taylor series has positive convergence radius, the resulting series may
      not coincide with the function; but if the function is analytic then the
      series converges pointwise to the function, and uniformly on every
      compact subset of the convergence interval. Concerning the Fourier
      series, if the function is square-integrable then the series converges in
      quadratic_mean, but additional requirements are needed to ensure the
      pointwise or uniform convergence (for instance, if the function is
      periodic and of class C1 then the convergence is uniform).
    * Finally, in practice one wants to approximate the function with a finite
      number of terms, say with a Taylor polynomial or a partial sum of the
      trigonometric series, respectively. In the case of the Taylor series the
      error is very small in a neighbourhood of the point where it is computed,
      while it may be very large at a distant point. In the case of the Fourier
      series the error is distributed along the domain of the function.
***** See also[edit] *****
    * Asymptotic_expansion
    * Generating_function
    * Laurent_series
    * Madhava_series
    * Newton's_divided_difference_interpolation
    * PadÃ©_approximant
    * Puiseux_series
    * Shift_operator
***** Notes[edit] *****
   1. ^ a b"Neither_Newton_nor_Leibniz_â_The_Pre-History_of_Calculus_and
      Celestial_Mechanics_in_Medieval_Kerala" (PDF). MAT 314. Canisius College.
      Archived (PDF) from the original on 2015-02-23. Retrieved 2006-07-09.
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
   3. ^ a bS. G. Dani (2012). "Ancient Indian Mathematics â A Conspectus".
      Resonance. 17 (3): 236â246. doi:10.1007/s12045-012-0022-y.
   4. ^ {{Ranjan Roy, The Discovery of the Series Formula for Ï by Leibniz,
      Gregory and Nilakantha, Mathematics Magazine Vol. 63, No. 5 (Dec., 1990),
      pp. 291-306.}}
   5. ^ Thomas_&_Finney_1996, Â§8.9
   6. ^Lindberg, David (2007). The Beginnings of Western Science (2nd ed.).
      University of Chicago Press. p. 33. ISBN 978-0-226-48205-7.
   7. ^Kline, M. (1990). Mathematical Thought from Ancient to Modern Times. New
      York: Oxford University Press. pp. 35â37. ISBN 0-19-506135-7.
   8. ^Boyer, C.; Merzbach,_U. (1991). A History of Mathematics (Second revised
      ed.). John Wiley and Sons. pp. 202â203. ISBN 0-471-09763-2.
   9. ^Taylor, Brook (1715). Methodus Incrementorum Directa et Inversa [Direct
      and Reverse Methods of Incrementation] (in Latin). London. p. 21â23
      (Prop. VII, Thm. 3, Cor. 2).
  10.  Translated into English inStruik, D. J. (1969). A Source Book in
      Mathematics 1200â1800. Cambridge, Massachusetts: Harvard University
      Press. pp. 329â332.
  11. ^Rudin,_Walter (1980), Real and Complex Analysis, New Dehli: McGraw-Hill,
      p. 418, Exercise 13, ISBN 0-07-099557-5
  12. ^Feller,_William (1971), An introduction to probability theory and its
      applications, Volume 2 (3rd ed.), Wiley, pp. 230â232
  13. .
  14. ^Hille,_Einar; Phillips,_Ralph_S. (1957), Functional analysis and semi-
      groups, AMS Colloquium Publications, 31, American Mathematical Society,
      pp. 300â327
  15. .
  16. ^Feller,_William (1970). An introduction to probability theory and its
      applications. 2 (3 ed.). p. 231.
  17. ^ Most of these can be found in (Abramowitz_&_Stegun_1970).
  18. ^Lars_HÃ¶rmander (1990), The analysis of partial differential operators,
      volume 1, Springer, Eqq. 1.1.7 and 1.1.7â²
  19. ^Duistermaat; Kolk (2010), Distributions: Theory and applications,
      Birkhauser, ch. 6
***** References[edit] *****
    * Abramowitz,_Milton; Stegun,_Irene_A. (1970), Handbook_of_Mathematical
      Functions_with_Formulas,_Graphs,_and_Mathematical_Tables, New York: Dover
      Publications, Ninth printing
Thomas, George B., Jr.; Finney, Ross L. (1996), Calculus and Analytic Geometry
(9th ed.), Addison Wesley, ISBN 0-201-53174-7
Greenberg, Michael (1998), Advanced Engineering Mathematics (2nd ed.), Prentice
Hall, ISBN 0-13-321431-1
***** External links[edit] *****
Taylor seriesat Wikipedia's sister_projects
    * Definitions from Wiktionary
    * Media from Wikimedia Commons
    * Textbooks from Wikibooks
    * Resources from Wikiversity
    * Data from Wikidata
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Taylor_series", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Weisstein,_Eric_W. "Taylor_Series". MathWorld.
Taylor_polynomial - practical introduction
Madhava_of_Sangamagramma
"Discussion_of_the_Parker-Sochacki_Method"
Another_Taylor_visualisation — where you can choose the point of the
approximation and the number of derivatives
Taylor_series_revisited_for_numerical_methods at Numerical_Methods_for_the_STEM
Undergraduate
Cinderella_2:_Taylor_expansion
Taylor_series
Inverse_trigonometric_functions_Taylor_series
"Essence_of_Calculus:_Taylor_series" – via YouTube.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Taylor_series&oldid=908539498"
Categories:
    * Real_analysis
    * Complex_analysis
    * Series_expansions
Hidden categories:
    * CS1_Latin-language_sources_(la)
    * Good_articles
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_November_2017
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
    * Wikibooks
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐ°ÑÒ¡Ð¾ÑÑÑÐ°
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Boarisch
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * PiemontÃ¨is
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * à·à·à¶à·à¶½
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 30 July 2019, at 11:03 (UTC).
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
