The following text has been accessed from https://en.wikipedia.org/wiki/Numerical_integration at Fri Aug 9 02:42:49 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Numerical integration ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Numerical integration is used to calculate a numerical approximation for the
value     S   {\displaystyle S}  [S], the area under the curve defined by     f
( x )   {\displaystyle f(x)}  [f(x)].
In analysis, numerical integration comprises a broad family of algorithms for
calculating the numerical value of a definite integral, and by extension, the
term is also sometimes used to describe the numerical_solution_of_differential
equations. This article focuses on calculation of definite integrals. The term
numerical quadrature (often abbreviated to quadrature) is more or less a
synonym for numerical integration, especially as applied to one-dimensional
integrals. Some authors refer to numerical integration over more than one
dimension as cubature;[1] others take quadrature to include higher-dimensional
integration.
The basic problem in numerical integration is to compute an approximate
solution to a definite integral
          &#x222B;  a   b   f ( x )  d x   {\displaystyle \int _{a}^{b}f
      (x)\,dx}  [{\displaystyle \int _{a}^{b}f(x)\,dx}]
to a given degree of accuracy. If f(x) is a smooth function integrated over a
small number of dimensions, and the domain of integration is bounded, there are
many methods for approximating the integral to the desired precision.
⁰
***** Contents *****
    * 1_History
    * 2_Reasons_for_numerical_integration
    * 3_Methods_for_one-dimensional_integrals
          o 3.1_Quadrature_rules_based_on_interpolating_functions
          o 3.2_Generalized_midpoint_rule_formula
          o 3.3_Adaptive_algorithms
          o 3.4_Extrapolation_methods
          o 3.5_Conservative_(a_priori)_error_estimation
          o 3.6_Integrals_over_infinite_intervals
    * 4_Multidimensional_integrals
          o 4.1_Monte_Carlo
          o 4.2_Sparse_grids
          o 4.3_Bayesian_Quadrature
    * 5_Connection_with_differential_equations
    * 6_See_also
    * 7_References
    * 8_External_links
***** History[edit] *****
Main article: Quadrature_(mathematics)
The term "numerical integration" first appears in 1915 in the publication A
Course in Interpolation and Numeric Integration for the Mathematical Laboratory
by David_Gibb.[2]
Quadrature is a historical mathematical term that means calculating area.
Quadrature problems have served as one of the main sources of mathematical
analysis. Mathematicians_of_Ancient_Greece, according to the Pythagorean
doctrine, understood calculation of area as the process of constructing
geometrically a square having the same area (squaring). That is why the process
was named quadrature. For example, a quadrature_of_the_circle, Lune_of
Hippocrates, The_Quadrature_of_the_Parabola. This construction must be
performed only by means of compass_and_straightedge.
The ancient Babylonians used the trapezoidal_rule to integrate the motion of
Jupiter along the ecliptic.[3]
Antique method to find the Geometric_mean
For a quadrature of a rectangle with the sides a and b it is necessary to
construct a square with the side     x =   a b     {\displaystyle x={\sqrt
{ab}}}  [x={\sqrt {ab}}] (the Geometric_mean of a and b). For this purpose it
is possible to use the following fact: if we draw the circle with the sum of a
and b as the diameter, then the height BH (from a point of their connection to
crossing with a circle) equals their geometric mean. The similar geometrical
construction solves a problem of a quadrature for a parallelogram and a
triangle.
                      The area of a segment of a parabola
Problems of quadrature for curvilinear figures are much more difficult. The
quadrature_of_the_circle with compass and straightedge had been proved in the
19th century to be impossible. Nevertheless, for some figures (for example the
Lune_of_Hippocrates) a quadrature can be performed. The quadratures of a sphere
surface and a parabola_segment done by Archimedes became the highest
achievement of the antique analysis.
    * The area of the surface of a sphere is equal to quadruple the area of a
      great_circle of this sphere.
    * The area of a segment of the parabola cut from it by a straight line is
      4/3 the area of the triangle inscribed in this segment.
For the proof of the results Archimedes used the Method_of_exhaustion of
Eudoxus.
In medieval Europe the quadrature meant calculation of area by any method. More
often the Method_of_indivisibles was used; it was less rigorous, but more
simple and powerful. With its help Galileo_Galilei and Gilles_de_Roberval found
the area of a cycloid arch, GrÃ©goire_de_Saint-Vincent investigated the area
under a hyperbola (Opus Geometricum, 1647), and Alphonse_Antonio_de_Sarasa, de
Saint-Vincent's pupil and commentator, noted the relation of this area to
logarithms.
John_Wallis algebrised this method: he wrote in his Arithmetica Infinitorum
(1656) series that we now call the definite_integral, and he calculated their
values. Isaac_Barrow and James_Gregory made further progress: quadratures for
some algebraic_curves and spirals. Christiaan_Huygens successfully performed a
quadrature of some Solids_of_revolution.
The quadrature of the hyperbola by Saint-Vincent and de Sarasa provided a new
function, the natural_logarithm, of critical importance.
With the invention of integral_calculus came a universal method for area
calculation. In response, the term quadrature has become traditional, and
instead the modern phrase "computation of a univariate definite integral" is
more common.
***** Reasons for numerical integration[edit] *****
There are several reasons for carrying out numerical integration.
   1. The integrand f(x) may be known only at certain points, such as obtained
      by sampling. Some embedded_systems and other computer applications may
      need numerical integration for this reason.
   2. A formula for the integrand may be known, but it may be difficult or
      impossible to find an antiderivative that is an elementary_function. An
      example of such an integrand is f(x) = exp(âx2), the antiderivative of
      which (the error_function, times a constant) cannot be written in
      elementary_form.
   3. It may be possible to find an antiderivative symbolically, but it may be
      easier to compute a numerical approximation than to compute the
      antiderivative. That may be the case if the antiderivative is given as an
      infinite series or product, or if its evaluation requires a special
      function that is not available.
***** Methods for one-dimensional integrals[edit] *****
Numerical integration methods can generally be described as combining
evaluations of the integrand to get an approximation to the integral. The
integrand is evaluated at a finite set of points called integration points and
a weighted sum of these values is used to approximate the integral. The
integration points and weights depend on the specific method used and the
accuracy required from the approximation.
An important part of the analysis of any numerical integration method is to
study the behavior of the approximation error as a function of the number of
integrand evaluations. A method that yields a small error for a small number of
evaluations is usually considered superior. Reducing the number of evaluations
of the integrand reduces the number of arithmetic operations involved, and
therefore reduces the total round-off_error. Also, each evaluation takes time,
and the integrand may be arbitrarily complicated.
A 'brute force' kind of numerical integration can be done, if the integrand is
reasonably well-behaved (i.e. piecewise continuous and of bounded_variation),
by evaluating the integrand with very small increments.
**** Quadrature rules based on interpolating functions[edit] ****
A large class of quadrature rules can be derived by constructing interpolating
functions that are easy to integrate. Typically these interpolating functions
are polynomials. In practice, since polynomials of very high degree tend to
oscillate wildly, only polynomials of low degree are used, typically linear and
quadratic.
Illustration of the rectangle rule.
The simplest method of this type is to let the interpolating function be a
constant function (a polynomial of degree zero) that passes through the point
(     a + b  2   , f  (    a + b  2   )   )    {\displaystyle \left({\frac
{a+b}{2}},f\left({\frac {a+b}{2}}\right)\right)}  [{\displaystyle \left({\frac
{a+b}{2}},f\left({\frac {a+b}{2}}\right)\right)}]. This is called the midpoint
rule or rectangle_rule
          &#x222B;  a   b   f ( x )  d x &#x2248; ( b &#x2212; a ) f  (    a +
      b  2   )  .   {\displaystyle \int _{a}^{b}f(x)\,dx\approx (b-a)f\left(
      {\frac {a+b}{2}}\right).}  [{\displaystyle \int _{a}^{b}f(x)\,dx\approx
      (b-a)f\left({\frac {a+b}{2}}\right).}]
Illustration of the trapezoidal rule.
The interpolating function may be a straight line (an affine_function, i.e. a
polynomial of degree 1) passing through the points      (  a , f ( a )  )
{\displaystyle \left(a,f(a)\right)}  [{\displaystyle \left(a,f(a)\right)}] and
(  b , f ( b )  )    {\displaystyle \left(b,f(b)\right)}  [{\displaystyle \left
(b,f(b)\right)}]. This is called the trapezoidal_rule
          &#x222B;  a   b   f ( x )  d x &#x2248; ( b &#x2212; a )  (    f ( a
      ) + f ( b )  2   )  .   {\displaystyle \int _{a}^{b}f(x)\,dx\approx (b-
      a)\left({\frac {f(a)+f(b)}{2}}\right).}  [{\displaystyle \int _{a}^{b}f
      (x)\,dx\approx (b-a)\left({\frac {f(a)+f(b)}{2}}\right).}]
Illustration of Simpson's rule.
For either one of these rules, we can make a more accurate approximation by
breaking up the interval     [ a , b ]   {\displaystyle [a,b]}  [ [a,b] ] into
some number     n   {\displaystyle n}  [n] of subintervals, computing an
approximation for each subinterval, then adding up all the results. This is
called a composite rule, extended rule, or iterated rule. For example, the
composite trapezoidal rule can be stated as
          &#x222B;  a   b   f ( x )  d x &#x2248;    b &#x2212; a  n    (     f
      ( a )  2   +  &#x2211;  k = 1   n &#x2212; 1    (  f  (  a + k    b
      &#x2212; a  n    )   )  +    f ( b )  2    )  ,   {\displaystyle \int _
      {a}^{b}f(x)\,dx\approx {\frac {b-a}{n}}\left({f(a) \over 2}+\sum _{k=1}^
      {n-1}\left(f\left(a+k{\frac {b-a}{n}}\right)\right)+{f(b) \over
      2}\right),}  [{\displaystyle \int _{a}^{b}f(x)\,dx\approx {\frac {b-a}
      {n}}\left({f(a) \over 2}+\sum _{k=1}^{n-1}\left(f\left(a+k{\frac {b-a}
      {n}}\right)\right)+{f(b) \over 2}\right),}]
where the subintervals have the form     [ a + k h , a + ( k + 1 ) h ] &#x2282;
[ a , b ] ,   {\displaystyle [a+kh,a+(k+1)h]\subset [a,b],}  [{\displaystyle
[a+kh,a+(k+1)h]\subset [a,b],}] with     h =    b &#x2212; a  n
{\displaystyle h={\frac {b-a}{n}}}  [{\displaystyle h={\frac {b-a}{n}}}] and
k = 0 , &#x2026; , n &#x2212; 1.   {\displaystyle k=0,\ldots ,n-1.}  [
{\displaystyle k=0,\ldots ,n-1.}] Here we used subintervals of the same length
h   {\displaystyle h}  [h] but one could also use intervals of varying length
(  h  k   )   k     {\displaystyle \left(h_{k}\right)_{k}}  [{\displaystyle
\left(h_{k}\right)_{k}}].
Interpolation with polynomials evaluated at equally spaced points in     [ a ,
b ]   {\displaystyle [a,b]}  [ [a,b] ] yields the NewtonâCotes_formulas, of
which the rectangle rule and the trapezoidal rule are examples. Simpson's_rule,
which is based on a polynomial of order 2, is also a NewtonâCotes formula.
Quadrature rules with equally spaced points have the very convenient property
of nesting. The corresponding rule with each interval subdivided includes all
the current points, so those integrand values can be re-used.
If we allow the intervals between interpolation points to vary, we find another
group of quadrature formulas, such as the Gaussian_quadrature formulas. A
Gaussian quadrature rule is typically more accurate than a NewtonâCotes rule,
which requires the same number of function evaluations, if the integrand is
smooth (i.e., if it is sufficiently differentiable). Other quadrature methods
with varying intervals include ClenshawâCurtis_quadrature (also called FejÃ©r
quadrature) methods, which do nest.
Gaussian quadrature rules do not nest, but the related GaussâKronrod
quadrature_formulas do.
**** Generalized midpoint rule formula[edit] ****
A generalized midpoint rule formula is given by
          &#x222B;  0   1    f ( x ) d x  =  &#x2211;  m = 1   M     &#x2211;
      n = 0   &#x221E;           (  &#x2212; 1  )    n    + 1       (  2 M  )
      n + 1     (  n + 1  )  !            f   ( n )      ( x )   |    x =    m
      &#x2212; 1  /  2  M          {\displaystyle \int _{0}^{1}{f(x)dx}=\sum _
      {m=1}^{M}{\sum _{n=0}^{\infty }{{\frac {{{\left({-1}\right)}^{n}}+1}{{
      {\left({2M}\right)}^{n+1}}\left({n+1}\right)!}}{{\left.{{f^{\left
      (n\right)}}\left(x\right)}\right|}_{x={\frac {m-1/2}{M}}}}}}}  [
      {\displaystyle \int _{0}^{1}{f(x)dx}=\sum _{m=1}^{M}{\sum _{n=0}^{\infty
      }{{\frac {{{\left({-1}\right)}^{n}}+1}{{{\left({2M}\right)}^{n+1}}\left(
      {n+1}\right)!}}{{\left.{{f^{\left(n\right)}}\left(x\right)}\right|}_{x=
      {\frac {m-1/2}{M}}}}}}}]
or
          &#x222B;  0   1    f ( x ) d x  =  lim  M &#x2192; &#x221E;
      &#x2211;  m = 1   M     &#x2211;  n = 0   N           (  &#x2212; 1  )
      n    + 1       (  2 M  )    n + 1     (  n + 1  )  !            f   ( n )
      ( x )   |    x =    m &#x2212; 1  /  2  M        ,   {\displaystyle \int
      _{0}^{1}{f(x)dx}=\lim _{M\to \infty }\sum _{m=1}^{M}{\sum _{n=0}^{N}{
      {\frac {{{\left({-1}\right)}^{n}}+1}{{{\left({2M}\right)}^{n+1}}\left(
      {n+1}\right)!}}{{\left.{{f^{\left(n\right)}}\left(x\right)}\right|}_{x=
      {\frac {m-1/2}{M}}}}}},}  [{\displaystyle \int _{0}^{1}{f(x)dx}=\lim _
      {M\to \infty }\sum _{m=1}^{M}{\sum _{n=0}^{N}{{\frac {{{\left({-
      1}\right)}^{n}}+1}{{{\left({2M}\right)}^{n+1}}\left({n+1}\right)!}}{
      {\left.{{f^{\left(n\right)}}\left(x\right)}\right|}_{x={\frac {m-1/2}
      {M}}}}}},}]
where      f  ( n )   ( x )   {\displaystyle f^{(n)}(x)}  [{\displaystyle f^{
(n)}(x)}] denotes     n   {\displaystyle n}  [n]-th derivative. For example,
substituting     M = 1   {\displaystyle M=1}  [{\displaystyle M=1}] and
         f ( x ) =   &#x03B8;  1 +  &#x03B8;  2    x  2        {\displaystyle f
      (x)={\frac {\theta }{1+\theta ^{2}x^{2}}}}  [{\displaystyle f(x)={\frac
      {\theta }{1+\theta ^{2}x^{2}}}}]
in the generalized midpoint rule formula, we obtain an equation of the inverse
tangent
          tan  &#x2212; 1   &#x2061; ( &#x03B8; ) = i  &#x2211;  n = 1
      &#x221E;     1  2 n &#x2212; 1     (    1   (  1 + 2 i  /  &#x03B8;  )
      2 n &#x2212; 1     &#x2212;   1   (  1 &#x2212; 2 i  /  &#x03B8;  )   2 n
      &#x2212; 1      )  = 2  &#x2211;  n = 1   &#x221E;      1  2 n &#x2212; 1
      a   n     ( &#x03B8; )     a  n   2    ( &#x03B8; )  +  b  n   2
      ( &#x03B8; )      ,   {\displaystyle \tan ^{-1}(\theta )=i\sum _{n=1}^
      {\infty }{\frac {1}{2n-1}}\left({\frac {1}{\left(1+2i/\theta \right)^{2n-
      1}}}-{\frac {1}{\left(1-2i/\theta \right)^{2n-1}}}\right)=2\sum _{n=1}^
      {\infty }{{\frac {1}{2n-1}}{\frac {{{a}_{n}}\left(\theta \right)}{a_{n}^
      {2}\left(\theta \right)+b_{n}^{2}\left(\theta \right)}}},}  [
      {\displaystyle \tan ^{-1}(\theta )=i\sum _{n=1}^{\infty }{\frac {1}{2n-
      1}}\left({\frac {1}{\left(1+2i/\theta \right)^{2n-1}}}-{\frac {1}{\left
      (1-2i/\theta \right)^{2n-1}}}\right)=2\sum _{n=1}^{\infty }{{\frac {1}
      {2n-1}}{\frac {{{a}_{n}}\left(\theta \right)}{a_{n}^{2}\left(\theta
      \right)+b_{n}^{2}\left(\theta \right)}}},}]
where     i =   &#x2212; 1     {\displaystyle i={\sqrt {-1}}}  [{\displaystyle
i={\sqrt {-1}}}] is imaginary_unit and
               a  1   ( &#x03B8; ) = 2  /  &#x03B8; ,       b  1   ( &#x03B8; )
      = 1 ,       a  n   ( &#x03B8; ) =  a  n &#x2212; 1   ( &#x03B8; )   (  1
      &#x2212; 4  /   &#x03B8;  2    )  + 4  b  n &#x2212; 1   ( &#x03B8; )  /
      &#x03B8; ,       b  n   ( &#x03B8; ) =  b  n &#x2212; 1   ( &#x03B8; )
      (  1 &#x2212; 4  /   &#x03B8;  2    )  &#x2212; 4  a  n &#x2212; 1
      ( &#x03B8; )  /  &#x03B8; .       {\displaystyle {\begin{aligned}&a_{1}
      (\theta )=2/\theta ,\\&b_{1}(\theta )=1,\\&a_{n}(\theta )=a_{n-1}(\theta
      )\,\left(1-4/\theta ^{2}\right)+4b_{n-1}(\theta )/\theta ,\\&b_{n}(\theta
      )=b_{n-1}(\theta )\,\left(1-4/\theta ^{2}\right)-4a_{n-1}(\theta )/\theta
      .\end{aligned}}}  [{\displaystyle {\begin{aligned}&a_{1}(\theta )=2/
      \theta ,\\&b_{1}(\theta )=1,\\&a_{n}(\theta )=a_{n-1}(\theta )\,\left(1-
      4/\theta ^{2}\right)+4b_{n-1}(\theta )/\theta ,\\&b_{n}(\theta )=b_{n-1}
      (\theta )\,\left(1-4/\theta ^{2}\right)-4a_{n-1}(\theta )/\theta .\end
      {aligned}}}]
Since at each odd     n   {\displaystyle n}  [n] the numerator of the integrand
becomes     ( &#x2212; 1  )  n   + 1 = 0   {\displaystyle (-1)^{n}+1=0}  [
{\displaystyle (-1)^{n}+1=0}], the generalized midpoint rule formula can be
reorganized as
          &#x222B;  0   1    f ( x ) d x  = 2  &#x2211;  m = 1   M     &#x2211;
      n = 0   &#x221E;      1      (  2 M  )    2 n + 1     (  2 n + 1  )  !
      f  ( 2 n )    ( x )  |    x =    m &#x2212; 1  /  2  M          .
      {\displaystyle \int _{0}^{1}{f(x)dx}=2\sum _{m=1}^{M}{\sum _{n=0}^{\infty
      }{{\frac {1}{{{\left({2M}\right)}^{2n+1}}\left({2n+1}\right)!}}{{\left.{
      {f^{(2n)}}(x)}\right|}_{x={\frac {m-1/2}{M}}}}}}\,\,.}  [{\displaystyle
      \int _{0}^{1}{f(x)dx}=2\sum _{m=1}^{M}{\sum _{n=0}^{\infty }{{\frac {1}{{
      {\left({2M}\right)}^{2n+1}}\left({2n+1}\right)!}}{{\left.{{f^{(2n)}}
      (x)}\right|}_{x={\frac {m-1/2}{M}}}}}}\,\,.}]
The following example of Mathematica code generates the plot showing difference
between inverse tangent and its approximation truncated at     M = 5
{\displaystyle M=5}  [{\displaystyle M=5}] and     N = 10   {\displaystyle
N=10}  [{\displaystyle N=10}]:
f[theta_, x_] := theta/(1 + theta^2*x^2);

aTan[theta_, M_, nMax_] :=
    2*Sum[(Function[x, Evaluate[D[f[theta, x], {x, 2*n}]]][(m - 1/2)/
        M])/((2*n + 1)!*(2*M)^(2*n + 1)), {m, 1, M}, {n, 0, nMax}];

Plot[{ArcTan[theta] - aTan[theta, 5, 10]}, {theta, -Pi, Pi},
 PlotRange -> All]
For a function     g ( t )   {\displaystyle g(t)}  [ g(t) ] defined over
interval     ( a , b )   {\displaystyle (a,b)}  [(a,b)], its integral is
          &#x222B;  a   b    g ( t ) d t  =  &#x222B;  0   b &#x2212; a    g
      ( &#x03C4; + a ) d &#x03C4;  = ( b &#x2212; a )  &#x222B;  0   1    g (
      ( b &#x2212; a ) x + a ) d x  .   {\displaystyle \int _{a}^{b}{g
      (t)dt}=\int _{0}^{b-a}{g(\tau +a)d\tau }=(b-a)\int _{0}^{1}{g((b-
      a)x+a)dx}.}  [{\displaystyle \int _{a}^{b}{g(t)dt}=\int _{0}^{b-a}{g(\tau
      +a)d\tau }=(b-a)\int _{0}^{1}{g((b-a)x+a)dx}.}]
Therefore, we can apply the generalized midpoint integration formula above by
assuming that     f ( x ) = ( b &#x2212; a )  g ( ( b &#x2212; a ) x + a )
{\displaystyle f(x)=(b-a)\,g((b-a)x+a)}  [{\displaystyle f(x)=(b-a)\,g((b-
a)x+a)}].
**** Adaptive algorithms[edit] ****
Further information: Adaptive_quadrature
If f(x) does not have many derivatives at all points, or if the derivatives
become large, then Gaussian quadrature is often insufficient. In this case, an
algorithm similar to the following will perform better:
def calculate_definite_integral_of_f(f, initial_step_size):
    '''
    This algorithm calculates the definite integral of a function
    from 0 to 1, adaptively, by choosing smaller steps near
    problematic points.
    '''
    x = 0.0
    h = initial_step_size
    accumulator = 0.0
    while x < 1.0:
        if x + h > 1.0:
            h = 1.0 - x # At end of unit interval, adjust last step to end at
1.
        if error_too_big_in_quadrature_of_f_over_range(f, [x,x+h]):
            h = make_h_smaller(h)
        else:
            accumulator += quadrature_of_f_over_range(f, [x,x+h])
            x += h
            if error_too_small_in_quadrature_of_over_range(f, [x,x+h]):
                h = make_h_larger(h) # Avoid wasting time on tiny steps.
    return accumulator
Some details of the algorithm require careful thought. For many cases,
estimating the error from quadrature over an interval for a function f(x) isn't
obvious. One popular solution is to use two different rules of quadrature, and
use their difference as an estimate of the error from quadrature. The other
problem is deciding what "too large" or "very small" signify. A local criterion
for "too large" is that the quadrature error should not be larger than t · h
where t, a real number, is the tolerance we wish to set for global error. Then
again, if h is already tiny, it may not be worthwhile to make it even smaller
even if the quadrature error is apparently large. A global criterion is that
the sum of errors on all the intervals should be less than t. This type of
error analysis is usually called "a posteriori" since we compute the error
after having computed the approximation.
Heuristics for adaptive quadrature are discussed by Forsythe et al. (Section
5.4).
**** Extrapolation methods[edit] ****
The accuracy of a quadrature rule of the Newton-Cotes type is generally a
function of the number of evaluation points. The result is usually more
accurate as the number of evaluation points increases, or, equivalently, as the
width of the step size between the points decreases. It is natural to ask what
the result would be if the step size were allowed to approach zero. This can be
answered by extrapolating the result from two or more nonzero step sizes, using
series_acceleration methods such as Richardson_extrapolation. The extrapolation
function may be a polynomial or rational_function. Extrapolation methods are
described in more detail by Stoer and Bulirsch (Section 3.4) and are
implemented in many of the routines in the QUADPACK library.
**** Conservative (a priori) error estimation[edit] ****
Let     f   {\displaystyle f}  [f] have a bounded first derivative over     [ a
, b ] ,   {\displaystyle [a,b],}  [[a,b],] i.e.     f &#x2208;  C  1   ( [ a ,
b ] ) .   {\displaystyle f\in C^{1}([a,b]).}  [{\displaystyle f\in C^{1}(
[a,b]).}] The mean_value_theorem for     f ,   {\displaystyle f,}  [
{\displaystyle f,}] where     x &#x2208; [ a , b ) ,   {\displaystyle x\in
[a,b),}  [{\displaystyle x\in [a,b),}] gives
         ( x &#x2212; a )  f &#x2032;  (  &#x03BE;  x   ) = f ( x ) &#x2212; f
      ( a ) ,   {\displaystyle (x-a)f'(\xi _{x})=f(x)-f(a),}  [{\displaystyle
      (x-a)f'(\xi _{x})=f(x)-f(a),}]
for some      &#x03BE;  x   &#x2208; ( a , x ]   {\displaystyle \xi _{x}\in
(a,x]}  [{\displaystyle \xi _{x}\in (a,x]}] depending on     x   {\displaystyle
x}  [x]. If we integrate in     x   {\displaystyle x}  [x] from     a
{\displaystyle a}  [a] to     b   {\displaystyle b}  [b] on both sides and take
the absolute values, we obtain
          |   &#x222B;  a   b   f ( x )  d x &#x2212; ( b &#x2212; a ) f ( a )
      |  =  |   &#x222B;  a   b   ( x &#x2212; a )  f &#x2032;  (  v  x   )  d
      x  |  .   {\displaystyle \left|\int _{a}^{b}f(x)\,dx-(b-a)f
      (a)\right|=\left|\int _{a}^{b}(x-a)f'(v_{x})\,dx\right|.}  [
      {\displaystyle \left|\int _{a}^{b}f(x)\,dx-(b-a)f(a)\right|=\left|\int _
      {a}^{b}(x-a)f'(v_{x})\,dx\right|.}]
We can further approximate the integral on the right-hand side by bringing the
absolute value into the integrand, and replacing the term in      f &#x2032;
{\displaystyle f'}  [f'] by an upper bound
          |   &#x222B;  a   b   f ( x )  d x &#x2212; ( b &#x2212; a
      ) f ( a )  |  &#x2264;    ( b &#x2212; a  )  2    2    sup  a
      &#x2264; x &#x2264; b    |   f &#x2032;  ( x )  |  ,
      {\displaystyle \left|\int _{a}^{b}f(x)\,dx-(b-a)f                 (1 )
      (a)\right|\leq {(b-a)^{2} \over 2}\sup _{a\leq x\leq              
      b}\left|f'(x)\right|,}  [{\displaystyle \left|\int _{a}^{b}f
      (x)\,dx-(b-a)f(a)\right|\leq {(b-a)^{2} \over 2}\sup _{a\leq
      x\leq b}\left|f'(x)\right|,}]
where the supremum was used to approximate. Hence, if we approximate the
integral      &#x222B;  a   b   f ( x )  d x   {\displaystyle \int _{a}^{b}f
(x)\,dx}  [\int _{a}^{b}f(x)\,dx] by the quadrature_rule     ( b &#x2212; a ) f
( a )   {\displaystyle (b-a)f(a)}  [{\displaystyle (b-a)f(a)}] our error is no
greater than the right hand side of 1. We can convert this into an error
analysis for the Riemann_sum (*), giving an upper bound of
            n  &#x2212; 1   2    sup  0 &#x2264; x &#x2264; 1    |   f &#x2032;
      ( x )  |    {\displaystyle {n^{-1} \over 2}\sup _{0\leq x\leq 1}\left|f'
      (x)\right|}  [{n^{-1} \over 2}\sup _{0\leq x\leq 1}\left|f'(x)\right|]
for the error term of that particular approximation. (Note that this is
precisely the error we calculated for the example     f ( x ) = x
{\displaystyle f(x)=x}  [f(x)=x].) Using more derivatives, and by tweaking the
quadrature, we can do a similar error analysis using a Taylor_series (using a
partial sum with remainder term) for f. This error analysis gives a strict
upper bound on the error, if the derivatives of f are available.
This integration method can be combined with interval_arithmetic to produce
computer_proofs and verified calculations.
**** Integrals over infinite intervals[edit] ****
Several methods exist for approximate integration over unbounded intervals. The
standard technique involves specially derived quadrature rules, such as Gauss-
Hermite_quadrature for integrals on the whole real line and Gauss-Laguerre
quadrature for integrals on the positive reals.[4] Monte Carlo methods can also
be used, or a change of variables to a finite interval; e.g., for the whole
line one could use
          &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x )  d x =  &#x222B;
      &#x2212; 1   + 1   f  (   t  1 &#x2212;  t  2      )     1 +  t  2
      ( 1 &#x2212;  t  2    )  2       d t ,   {\displaystyle \int _{-\infty }^
      {\infty }f(x)\,dx=\int _{-1}^{+1}f\left({\frac {t}{1-t^{2}}}\right){\frac
      {1+t^{2}}{(1-t^{2})^{2}}}\,dt,}  [{\displaystyle \int _{-\infty }^{\infty
      }f(x)\,dx=\int _{-1}^{+1}f\left({\frac {t}{1-t^{2}}}\right){\frac {1+t^
      {2}}{(1-t^{2})^{2}}}\,dt,}]
and for semi-infinite intervals one could use
              &#x222B;  a   &#x221E;   f ( x )  d x    =  &#x222B;  0   1   f
      (  a +   t  1 &#x2212; t     )     d t   ( 1 &#x2212; t  )  2      ,
      &#x222B;  &#x2212; &#x221E;   a   f ( x )  d x    =  &#x222B;  0   1   f
      (  a &#x2212;    1 &#x2212; t  t    )     d t   t  2     ,
      {\displaystyle {\begin{aligned}\int _{a}^{\infty }f(x)\,dx&=\int _{0}^
      {1}f\left(a+{\frac {t}{1-t}}\right){\frac {dt}{(1-t)^{2}}},\\\int _{-
      \infty }^{a}f(x)\,dx&=\int _{0}^{1}f\left(a-{\frac {1-t}{t}}\right){\frac
      {dt}{t^{2}}},\end{aligned}}}  [{\displaystyle {\begin{aligned}\int _{a}^
      {\infty }f(x)\,dx&=\int _{0}^{1}f\left(a+{\frac {t}{1-t}}\right){\frac
      {dt}{(1-t)^{2}}},\\\int _{-\infty }^{a}f(x)\,dx&=\int _{0}^{1}f\left(a-
      {\frac {1-t}{t}}\right){\frac {dt}{t^{2}}},\end{aligned}}}]
as possible transformations.
***** Multidimensional integrals[edit] *****
The quadrature rules discussed so far are all designed to compute one-
dimensional integrals. To compute integrals in multiple dimensions, one
approach is to phrase the multiple integral as repeated one-dimensional
integrals by applying Fubini's_theorem (the tensor product rule). This approach
requires the function evaluations to grow_exponentially as the number of
dimensions increases. Three methods are known to overcome this so-called curse
of_dimensionality.
A great many additional techniques for forming multidimensional cubature
integration rules for a variety of weighting functions are given in the
monograph by Stroud.[5]
**** Monte Carlo[edit] ****
Main article: Monte_Carlo_integration
Monte_Carlo_methods and quasi-Monte_Carlo_methods are easy to apply to multi-
dimensional integrals. They may yield greater accuracy for the same number of
function evaluations than repeated integrations using one-dimensional methods.
[citation_needed]
A large class of useful Monte Carlo methods are the so-called Markov_chain
Monte_Carlo algorithms, which include the Metropolis-Hastings_algorithm and
Gibbs_sampling.
**** Sparse grids[edit] ****
Sparse_grids were originally developed by Smolyak for the quadrature of high-
dimensional functions. The method is always based on a one-dimensional
quadrature rule, but performs a more sophisticated combination of univariate
results. However, whereas the tensor product rule guarantees that the weights
of all of the cubature points will be positive if the weights of the quadrature
points were positive, Smolyak's rule does not guarantee that the weights will
all be positive.
**** Bayesian Quadrature[edit] ****
Bayesian Quadrature is a statistical approach to the numerical problem of
computing integrals and falls under the field of probabilistic numerics. It can
provide a full handling of the uncertainty over the solution of the integral
expressed as a Gaussian_Process posterior variance. It is also known to provide
very fast convergence rates which can be up to exponential in the number of
quadrature points n.[6]
***** Connection with differential equations[edit] *****
The problem of evaluating the integral
         F ( x ) =  &#x222B;  a   x   f ( u )  d u   {\displaystyle F(x)=\int _
      {a}^{x}f(u)\,du}  [F(x)=\int _{a}^{x}f(u)\,du]
can be reduced to an initial_value_problem for an ordinary_differential
equation by applying the first part of the fundamental_theorem_of_calculus. By
differentiating both sides of the above with respect to the argument x, it is
seen that the function F satisfies
            d F ( x )   d x    = f ( x ) ,  F ( a ) = 0.   {\displaystyle
      {\frac {dF(x)}{dx}}=f(x),\quad F(a)=0.}  [{\frac {dF(x)}{dx}}=f(x),\quad
      F(a)=0.]
Methods developed for ordinary differential equations, such as RungeâKutta
methods, can be applied to the restated problem and thus be used to evaluate
the integral. For instance, the standard fourth-order RungeâKutta method
applied to the differential equation yields Simpson's rule from above.
The differential equation F ' (x) = ƒ(x) has a special form: the right-hand
side contains only the dependent variable (here x) and not the independent
variable (here F). This simplifies the theory and algorithms considerably. The
problem of evaluating integrals is thus best studied in its own right.
***** See also[edit] *****
    * Numerical_methods_for_ordinary_differential_equations
    * Truncation_error_(numerical_integration)
    * ClenshawâCurtis_quadrature
    * Gauss-Kronrod_quadrature
    * Riemann_Sum or Riemann_Integral
    * Trapezoidal_rule
    * Romberg's_method
    * Tanh-sinh_quadrature
***** References[edit] *****
   1. ^Weisstein,_Eric_W. "Cubature". MathWorld.
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
   3. ^"Earliest_Known_Uses_of_Some_of_the_Words_of_Mathematics_(Q)".
      jeff560.tripod.com. Retrieved 31 March 2018.
   4. ^Mathieu Ossendrijver (Jan 29, 2016). "Ancient Babylonian astronomers
      calculated Jupiter's position from the area under a time-velocity graph".
      Science. 351 (6272): 482â484. Bibcode:2016Sci...351..482O. doi:10.1126/
      science.aad8085. PMID 26823423.
   5. ^Leader,_Jeffery_J. (2004). Numerical Analysis and Scientific
      Computation. Addison Wesley. ISBN 978-0-201-73499-7.
   6. ^Stroud, A. H. (1971). Approximate Calculation of Multiple Integrals.
      Cliffs, NJ: Prentice-Hall Inc.
   7. ^Briol, FranÃ§ois-Xavier; Oates, Chris J.; Girolami, Mark; Osborne,
      Michael A. (2015-06-08). "Frank-Wolfe Bayesian Quadrature: Probabilistic
      Integration with Theoretical Guarantees". arXiv:1506.02681 [stat.ML].
    * Philip_J._Davis and Philip_Rabinowitz, Methods of Numerical Integration.
    * George_E._Forsythe, Michael A. Malcolm, and Cleve_B._Moler, Computer
      Methods for Mathematical Computations. Englewood Cliffs, NJ: Prentice-
      Hall, 1977. (See Chapter 5.)
    * Press, W.H.; Teukolsky, S.A.; Vetterling, W.T.; Flannery, B.P. (2007),
      "Chapter_4._Integration_of_Functions", Numerical Recipes: The Art of
      Scientific Computing (3rd ed.), New York: Cambridge University Press,
      ISBN 978-0-521-88068-8
Josef_Stoer and Roland_Bulirsch, Introduction to Numerical Analysis. New York:
Springer-Verlag, 1980. (See Chapter 3.)
Boyer,_C._B., A History of Mathematics, 2nd ed. rev. by Uta_C._Merzbach, New
York: Wiley, 1989
ISBN 0-471-09763-2 (1991 pbk ed.
ISBN 0-471-54397-7).
Eves,_Howard, An Introduction to the History of Mathematics, Saunders, 1990,
ISBN 0-03-029558-0,
***** External links[edit] *****
    * Integration:_Background,_Simulations,_etc. at Holistic Numerical Methods
      Institute
    * Lobatto_Quadrature from Wolfram Mathworld
    * Lobatto_quadrature_formula from Encyclopedia of Mathematics
    * Implementations_of_many_quadrature_and_cubature_formulae within the free
      Tracker_Component_Library.
Authority_control [Edit_this_at_Wikidata]     * NDL: 00571772

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Numerical_integration&oldid=902548159"
Categories:
    * Numerical_analysis
    * Numerical_integration_(quadrature)
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_November_2018
    * Wikipedia_articles_with_NDL_identifiers
    * Articles_with_example_Python_code
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
    * à¦¬à¦¾à¦à¦²à¦¾
    * Bosanski
    * CatalÃ 
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Latina
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * VÃ¨neto
    * ä¸­æ
Edit_links
    * This page was last edited on 19 June 2019, at 15:44 (UTC).
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
