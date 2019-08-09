The following text has been accessed from https://en.wikipedia.org/wiki/Taylor%27s_theorem at Fri Aug 9 00:01:48 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Taylor's theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The exponential function y = ex (red) and the corresponding Taylor polynomial
of degree four (dashed green) around the origin.
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
    * Taylor's theorem
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
In calculus, Taylor's theorem gives an approximation of a k-times
differentiable function around a given point by a k-th order Taylor polynomial.
For analytic_functions the Taylor polynomials at a given point are finite-order
truncations of its Taylor_series, which completely determines the function in
some neighborhood of the point. It can be thought of as the extension of linear
approximation to higher order polynomials, and in the case of k equals 2 is
often referred to as a quadratic approximation.[1] The exact content of
"Taylor's theorem" is not universally agreed upon. Indeed, there are several
versions of it applicable in different situations, and some of them contain
explicit estimates on the approximation error of the function by its Taylor
polynomial.
Taylor's theorem is named after the mathematician Brook_Taylor, who stated a
version of it in 1712. Yet an explicit expression of the error was not provided
until much later on by Joseph-Louis_Lagrange. An earlier version of the result
was already mentioned in 1671 by James_Gregory.[2]
Taylor's theorem is taught in introductory-level calculus courses and is one of
the central elementary tools in mathematical_analysis. Within pure_mathematics
it is the starting point of more advanced asymptotic_analysis and is commonly
used in more applied fields of numerics, as well as in mathematical_physics.
Taylor's theorem also generalizes to multivariate and vector_valued functions
f &#x003A;   R   n   &#x2192;   R   m     {\displaystyle f\colon \mathbb {R} ^
{n}\to \mathbb {R} ^{m}}  [{\displaystyle f\colon \mathbb {R} ^{n}\to \mathbb
{R} ^{m}}] on any dimensions n and m. This generalization of Taylor's theorem
is the basis for the definition of so-called jets, which appear in differential
geometry and partial_differential_equations.
⁰
***** Contents *****
    * 1_Motivation
    * 2_Taylor's_theorem_in_one_real_variable
          o 2.1_Statement_of_the_theorem
          o 2.2_Explicit_formulas_for_the_remainder
          o 2.3_Estimates_for_the_remainder
          o 2.4_Example
    * 3_Relationship_to_analyticity
          o 3.1_Taylor_expansions_of_real_analytic_functions
          o 3.2_Taylor's_theorem_and_convergence_of_Taylor_series
          o 3.3_Taylor's_theorem_in_complex_analysis
          o 3.4_Example
    * 4_Generalizations_of_Taylor's_theorem
          o 4.1_Higher-order_differentiability
          o 4.2_Taylor's_theorem_for_multivariate_functions
          o 4.3_Example_in_two_dimensions
    * 5_Proofs
          o 5.1_Proof_for_Taylor's_theorem_in_one_real_variable
          o 5.2_Derivation_for_the_mean_value_forms_of_the_remainder
          o 5.3_Derivation_for_the_integral_form_of_the_remainder
          o 5.4_Derivation_for_the_Cauchy_form_of_the_remainder
          o 5.5_Derivation_for_the_remainder_of_multivariate_Taylor_polynomials
    * 6_See_also
    * 7_Footnotes
    * 8_References
    * 9_External_links
***** Motivation[edit] *****
Graph of f(x) = ex (blue) with its linear_approximation P1(x) = 1 + x (red) at
a = 0.
If a real-valued function f is differentiable at the point a then it has a
linear_approximation at the point a. This means that there exists a function h1
such that
         f ( x ) = f ( a ) +  f &#x2032;  ( a ) ( x &#x2212; a ) +  h  1   ( x
      ) ( x &#x2212; a ) ,   lim  x &#x2192; a    h  1   ( x ) = 0.
      {\displaystyle f(x)=f(a)+f'(a)(x-a)+h_{1}(x)(x-a),\quad \lim _{x\to a}h_
      {1}(x)=0.}  [{\displaystyle f(x)=f(a)+f'(a)(x-a)+h_{1}(x)(x-a),\quad \lim
      _{x\to a}h_{1}(x)=0.}]
Here
          P  1   ( x ) = f ( a ) +  f &#x2032;  ( a ) ( x &#x2212; a )
      {\displaystyle P_{1}(x)=f(a)+f'(a)(x-a)}  [{\displaystyle P_{1}(x)=f
      (a)+f'(a)(x-a)}]
is the linear approximation of f at the point a. The graph of y = P1(x) is the
tangent_line to the graph of f at x = a. The error in the approximation is
          R  1   ( x ) = f ( x ) &#x2212;  P  1   ( x ) =  h  1   ( x ) ( x
      &#x2212; a ) .   {\displaystyle R_{1}(x)=f(x)-P_{1}(x)=h_{1}(x)(x-a).}  [
      {\displaystyle R_{1}(x)=f(x)-P_{1}(x)=h_{1}(x)(x-a).}]
Note that this goes to zero a little bit faster than x − a as x tends to a,
given the limiting behavior of h1.
Graph of f(x) = ex (blue) with its quadratic approximation P2(x) = 1 + x + x2/
2 (red) at a = 0. Note the improvement in the approximation.
If we wanted a better approximation to f, we might instead try a quadratic
polynomial instead of a linear function. Instead of just matching one
derivative of f at a, we can match two derivatives, thus producing a polynomial
that has the same slope and concavity as f at a. The quadratic polynomial in
question is
          P  2   ( x ) = f ( a ) +  f &#x2032;  ( a ) ( x &#x2212; a ) +     f
      &#x2033;  ( a )  2   ( x &#x2212; a  )  2   .   {\displaystyle P_{2}(x)=f
      (a)+f'(a)(x-a)+{\frac {f''(a)}{2}}(x-a)^{2}.}  [{\displaystyle P_{2}(x)=f
      (a)+f'(a)(x-a)+{\frac {f''(a)}{2}}(x-a)^{2}.}]
Taylor's theorem ensures that the quadratic approximation is, in a sufficiently
small neighborhood of the point a, a better approximation than the linear
approximation. Specifically,
         f ( x ) =  P  2   ( x ) +  h  2   ( x ) ( x &#x2212; a  )  2   ,   lim
      x &#x2192; a    h  2   ( x ) = 0.   {\displaystyle f(x)=P_{2}(x)+h_{2}(x)
      (x-a)^{2},\quad \lim _{x\to a}h_{2}(x)=0.}  [{\displaystyle f(x)=P_{2}
      (x)+h_{2}(x)(x-a)^{2},\quad \lim _{x\to a}h_{2}(x)=0.}]
Here the error in the approximation is
          R  2   ( x ) = f ( x ) &#x2212;  P  2   ( x ) =  h  2   ( x ) ( x
      &#x2212; a  )  2   ,   {\displaystyle R_{2}(x)=f(x)-P_{2}(x)=h_{2}(x)(x-
      a)^{2},}  [{\displaystyle R_{2}(x)=f(x)-P_{2}(x)=h_{2}(x)(x-a)^{2},}]
which, given the limiting behavior of      h  2     {\displaystyle h_{2}}  [h_
{2}], goes to zero faster than     ( x &#x2212; a  )  2     {\displaystyle (x-
a)^{2}}  [{\displaystyle (x-a)^{2}}] as x tends to a.
Approximation of f(x) = 1/(1 + x2) (blue) by its Taylor polynomials Pk of order
k = 1, ..., 16 centered at x = 0 (red) and x = 1 (green). The approximations do
not improve at all outside (â1, 1) and (1 â â2, 1 + â2) respectively.
Similarly, we might get still better approximations to f if we use polynomials
of higher degree, since then we can match even more derivatives with f at the
selected base point.
In general, the error in approximating a function by a polynomial of degree k
will go to zero a little bit faster than (x − a)k as x tends to a. But this
might not always be the case: it is also possible that increasing the degree of
the approximating polynomial does not increase the quality of approximation at
all even if the function f to be approximated is infinitely many times
differentiable. An example of this behavior is given below, and it is related
to the fact that unlike analytic_functions, more general functions are not
(locally) determined by the values of their derivatives at a single point.
Taylor's theorem is of asymptotic nature: it only tells us that the error Rk in
an approximation by a k-th order Taylor polynomial Pk tends to zero faster than
any nonzero k-th degree polynomial as x â a. It does not tell us how large
the error is in any concrete neighborhood of the center of expansion, but for
this purpose there are explicit formulae for the remainder term (given below)
which are valid under some additional regularity assumptions on f. These
enhanced versions of Taylor's theorem typically lead to uniform_estimates for
the approximation error in a small neighborhood of the center of expansion, but
the estimates do not necessarily hold for neighborhoods which are too large,
even if the function f is analytic. In that situation one may have to select
several Taylor polynomials with different centers of expansion to have reliable
Taylor-approximations of the original function (see animation on the right.)
There are several things we might do with the remainder term:
   1. Estimate the error in using a polynomial Pk(x) of degree k to estimate f
      (x) on a given interval (a â r, a + r). (The interval and the degree k
      are fixed; we want to find the error.)
   2. Find the smallest degree k for which the polynomial Pk(x) approximates f
      (x) to within a given error (or tolerance) on a given interval (a â r,
      a + r) . (The interval and the error are fixed; we want to find the
      degree.)
   3. Find the largest interval (a â r, a + r) on which Pk(x) approximates f
      (x) to within a given error ("tolerance"). (The degree and the error are
      fixed; we want to find the interval.)
***** Taylor's theorem in one real variable[edit] *****
**** Statement of the theorem[edit] ****
The precise statement of the most basic version of Taylor's theorem is as
follows:
     Taylor's theorem.[3][4][5] Let k ≥ 1 be an integer and let the
     function f : R → R be k times differentiable at the point a ∈ R. Then
     there exists a function hk : R → R such that
              f ( x ) = f ( a ) +  f &#x2032;  ( a ) ( x &#x2212; a ) +
           f &#x2033;  ( a )   2 !    ( x &#x2212; a  )  2   + &#x22EF; +
           f  ( k )   ( a )   k !    ( x &#x2212; a  )  k   +  h  k   ( x
           ) ( x &#x2212; a  )  k   ,   {\displaystyle f(x)=f(a)+f'(a)(x-
           a)+{\frac {f''(a)}{2!}}(x-a)^{2}+\cdots +{\frac {f^{(k)}(a)}
           {k!}}(x-a)^{k}+h_{k}(x)(x-a)^{k},}  [f(x)=f(a)+f'(a)(x-a)+
           {\frac {f''(a)}{2!}}(x-a)^{2}+\cdots +{\frac {f^{(k)}(a)}{k!}}
           (x-a)^{k}+h_{k}(x)(x-a)^{k},]
          and     lim  x &#x2192; a    h  k   ( x ) = 0   {\displaystyle
     {\mbox{and}}\quad \lim _{x\to a}h_{k}(x)=0}  [{\displaystyle {\mbox
     {and}}\quad \lim _{x\to a}h_{k}(x)=0}]. This is called the Peano form
     of the remainder.
The polynomial appearing in Taylor's theorem is the k-th order Taylor
polynomial
          P  k   ( x ) = f ( a ) +  f &#x2032;  ( a ) ( x &#x2212; a ) +     f
      &#x2033;  ( a )   2 !    ( x &#x2212; a  )  2   + &#x22EF; +     f  ( k )
      ( a )   k !    ( x &#x2212; a  )  k     {\displaystyle P_{k}(x)=f(a)+f'
      (a)(x-a)+{\frac {f''(a)}{2!}}(x-a)^{2}+\cdots +{\frac {f^{(k)}(a)}{k!}}
      (x-a)^{k}}  [P_{k}(x)=f(a)+f'(a)(x-a)+{\frac {f''(a)}{2!}}(x-a)^
      {2}+\cdots +{\frac {f^{(k)}(a)}{k!}}(x-a)^{k}]
of the function f at the point a. The Taylor polynomial is the unique
"asymptotic best fit" polynomial in the sense that if there exists a function
hk : R → R and a k-th order polynomial p such that
         f ( x ) = p ( x ) +  h  k   ( x ) ( x &#x2212; a  )  k   ,   lim  x
      &#x2192; a    h  k   ( x ) = 0 ,   {\displaystyle f(x)=p(x)+h_{k}(x)(x-
      a)^{k},\quad \lim _{x\to a}h_{k}(x)=0,}  [f(x)=p(x)+h_{k}(x)(x-a)^
      {k},\quad \lim _{x\to a}h_{k}(x)=0,]
then p = Pk. Taylor's theorem describes the asymptotic behavior of the
remainder term
         &#xA0;  R  k   ( x ) = f ( x ) &#x2212;  P  k   ( x ) ,
      {\displaystyle \ R_{k}(x)=f(x)-P_{k}(x),}  [\ R_{k}(x)=f(x)-P_{k}(x),]
which is the approximation_error when approximating f with its Taylor
polynomial. Using the little-o_notation, the statement in Taylor's theorem
reads as
          R  k   ( x ) = o (  |  x &#x2212; a   |   k   ) ,  x &#x2192; a .
      {\displaystyle R_{k}(x)=o(|x-a|^{k}),\quad x\to a.}  [R_{k}(x)=o(|x-a|^
      {k}),\quad x\to a.]
**** Explicit formulas for the remainder[edit] ****
Under stronger regularity assumptions on f there are several precise formulae
for the remainder term Rk of the Taylor polynomial, the most common ones being
the following.
     Mean-value forms of the remainder. Let f : R → R be k + 1 times
     differentiable on the open_interval with f(k) continuous on the
     closed_interval between a and x.[6] Then
               R  k   ( x ) =     f  ( k + 1 )   (  &#x03BE;  L   )   ( k
           + 1 ) !    ( x &#x2212; a  )  k + 1     {\displaystyle R_{k}
           (x)={\frac {f^{(k+1)}(\xi _{L})}{(k+1)!}}(x-a)^{k+1}}  [R_{k}
           (x)={\frac {f^{(k+1)}(\xi _{L})}{(k+1)!}}(x-a)^{k+1}]
     for some real number ξL between a and x. This is the Lagrange form[7]
     of the remainder. Similarly,
               R  k   ( x ) =     f  ( k + 1 )   (  &#x03BE;  C   )   k !
           ( x &#x2212;  &#x03BE;  C    )  k   ( x &#x2212; a )
           {\displaystyle R_{k}(x)={\frac {f^{(k+1)}(\xi _{C})}{k!}}(x-\xi
           _{C})^{k}(x-a)}  [R_{k}(x)={\frac {f^{(k+1)}(\xi _{C})}{k!}}(x-
           \xi _{C})^{k}(x-a)]
     for some real number ξC between a and x. This is the Cauchy form[8]
     of the remainder.
These refinements of Taylor's theorem are usually proved using the mean_value
theorem, whence the name. Also other similar expressions can be found. For
example, if G(t) is continuous on the closed interval and differentiable with a
non-vanishing derivative on the open interval between a and x, then
          R  k   ( x ) =     f  ( k + 1 )   ( &#x03BE; )   k !    ( x &#x2212;
      &#x03BE;  )  k      G ( x ) &#x2212; G ( a )    G &#x2032;  ( &#x03BE; )
      {\displaystyle R_{k}(x)={\frac {f^{(k+1)}(\xi )}{k!}}(x-\xi )^{k}{\frac
      {G(x)-G(a)}{G'(\xi )}}}  [R_{k}(x)={\frac {f^{(k+1)}(\xi )}{k!}}(x-\xi )^
      {k}{\frac {G(x)-G(a)}{G'(\xi )}}]
for some number ξ between a and x. This version covers the Lagrange and Cauchy
forms of the remainder as special cases, and is proved below using Cauchy's
mean_value_theorem.
The statement for the integral form of the remainder is more advanced than the
previous ones, and requires understanding of Lebesgue_integration_theory for
the full generality. However, it holds also in the sense of Riemann_integral
provided the (k + 1)th derivative of f is continuous on the closed interval
[a,x].
     Integral form of the remainder.[9] Let f(k) be absolutely_continuous
     on the closed_interval between a and x. Then
               R  k   ( x ) =  &#x222B;  a   x       f  ( k + 1 )   ( t )
           k !    ( x &#x2212; t  )  k    d t .   {\displaystyle R_{k}
           (x)=\int _{a}^{x}{\frac {f^{(k+1)}(t)}{k!}}(x-t)^{k}\,dt.}  [R_
           {k}(x)=\int _{a}^{x}{\frac {f^{(k+1)}(t)}{k!}}(x-t)^{k}\,dt.]
Due to absolute_continuity of f(k) on the closed_interval between a and x, its
derivative f(k+1) exists as an L1-function, and the result can be proven by a
formal calculation using fundamental_theorem_of_calculus and integration_by
parts.
**** Estimates for the remainder[edit] ****
It is often useful in practice to be able to estimate the remainder term
appearing in the Taylor approximation, rather than having an exact formula for
it. Suppose that f is (k + 1)-times continuously differentiable in an interval
I containing a. Suppose that there are real constants q and Q such that
         q &#x2264;  f  ( k + 1 )   ( x ) &#x2264; Q   {\displaystyle q\leq f^{
      (k+1)}(x)\leq Q}  [q\leq f^{(k+1)}(x)\leq Q]
throughout I. Then the remainder term satisfies the inequality[10]
         q    ( x &#x2212; a  )  k + 1     ( k + 1 ) !    &#x2264;  R  k   ( x
      ) &#x2264; Q    ( x &#x2212; a  )  k + 1     ( k + 1 ) !    ,
      {\displaystyle q{\frac {(x-a)^{k+1}}{(k+1)!}}\leq R_{k}(x)\leq Q{\frac {
      (x-a)^{k+1}}{(k+1)!}},}  [q{\frac {(x-a)^{k+1}}{(k+1)!}}\leq R_{k}(x)\leq
      Q{\frac {(x-a)^{k+1}}{(k+1)!}},]
if x > a, and a similar estimate if x < a. This is a simple consequence of the
Lagrange form of the remainder. In particular, if
          |   f  ( k + 1 )   ( x )  |  &#x2264; M   {\displaystyle |f^{(k+1)}
      (x)|\leq M}  [{\displaystyle |f^{(k+1)}(x)|\leq M}]
on an interval I = (a − r,a + r) with some     r > 0   {\displaystyle r>0}
[r>0] , then
          |   R  k   ( x )  |  &#x2264; M     |  x &#x2212; a   |   k + 1
      ( k + 1 ) !    &#x2264; M    r  k + 1    ( k + 1 ) !      {\displaystyle
      |R_{k}(x)|\leq M{\frac {|x-a|^{k+1}}{(k+1)!}}\leq M{\frac {r^{k+1}}{
      (k+1)!}}}  [{\displaystyle |R_{k}(x)|\leq M{\frac {|x-a|^{k+1}}{
      (k+1)!}}\leq M{\frac {r^{k+1}}{(k+1)!}}}]
for all x∈(a â r,a + r). The second inequality is called a uniform_estimate,
because it holds uniformly for all x on the interval (a â r,a + r).
**** Example[edit] ****
Approximation of ex (blue) by its Taylor polynomials Pk of order k = 1,...,7
centered at x = 0 (red).
Suppose that we wish to approximate the function f(x) = ex on the interval
[−1,1] while ensuring that the error in the approximation is no more than 10−5.
In this example we pretend that we only know the following properties of the
exponential function:
         ( &#x2217; )   e  0   = 1 ,    d  d x     e  x   =  e  x   ,   e  x
      > 0 ,  x &#x2208;  R  .   {\displaystyle (*)\qquad e^{0}=1,\qquad {\frac
      {d}{dx}}e^{x}=e^{x},\qquad e^{x}>0,\qquad x\in \mathbb {R} .}  [(*)\qquad
      e^{0}=1,\qquad {\frac {d}{dx}}e^{x}=e^{x},\qquad e^{x}>0,\qquad x\in
      \mathbb {R} .]
From these properties it follows that f(k)(x) = ex for all k, and in
particular, f(k)(0) = 1. Hence the k-th order Taylor polynomial of f at 0 and
its remainder term in the Lagrange form are given by
          P  k   ( x ) = 1 + x +    x  2    2 !    + &#x22EF; +    x  k    k !
      ,   R  k   ( x ) =    e  &#x03BE;    ( k + 1 ) !     x  k + 1   ,
      {\displaystyle P_{k}(x)=1+x+{\frac {x^{2}}{2!}}+\cdots +{\frac {x^{k}}
      {k!}},\qquad R_{k}(x)={\frac {e^{\xi }}{(k+1)!}}x^{k+1},}  [P_{k}(x)=1+x+
      {\frac {x^{2}}{2!}}+\cdots +{\frac {x^{k}}{k!}},\qquad R_{k}(x)={\frac
      {e^{\xi }}{(k+1)!}}x^{k+1},]
where ξ is some number between 0 and x. Since ex is increasing by (*), we can
simply use ex â¤ 1 for x â [−1, 0] to estimate the remainder on the
subinterval [−1, 0]. To obtain an upper bound for the remainder on [0,1], we
use the property eξ<ex for 0<ξ<x to estimate
          e  x   = 1 + x +    e  &#x03BE;   2    x  2   < 1 + x +    e  x   2
      x  2   ,  0 < x &#x2264; 1   {\displaystyle e^{x}=1+x+{\frac {e^{\xi }}
      {2}}x^{2}<1+x+{\frac {e^{x}}{2}}x^{2},\qquad 0<x\leq 1}  [e^{x}=1+x+
      {\frac {e^{\xi }}{2}}x^{2}<1+x+{\frac {e^{x}}{2}}x^{2},\qquad 0<x\leq 1]
using the second order Taylor expansion. Then we solve for ex to deduce that
          e  x   &#x2264;    1 + x   1 &#x2212;    x  2   2      = 2    1 + x
      2 &#x2212;  x  2      &#x2264; 4 ,  0 &#x2264; x &#x2264; 1
      {\displaystyle e^{x}\leq {\frac {1+x}{1-{\frac {x^{2}}{2}}}}=2{\frac
      {1+x}{2-x^{2}}}\leq 4,\qquad 0\leq x\leq 1}  [e^{x}\leq {\frac {1+x}{1-
      {\frac {x^{2}}{2}}}}=2{\frac {1+x}{2-x^{2}}}\leq 4,\qquad 0\leq x\leq 1]
simply by maximizing the numerator and minimizing the denominator. Combining
these estimates for ex we see that
          |   R  k   ( x )  |  &#x2264;    4  |  x   |   k + 1     ( k + 1 ) !
      &#x2264;   4  ( k + 1 ) !    ,  &#x2212; 1 &#x2264; x &#x2264; 1 ,
      {\displaystyle |R_{k}(x)|\leq {\frac {4|x|^{k+1}}{(k+1)!}}\leq {\frac {4}
      {(k+1)!}},\qquad -1\leq x\leq 1,}  [|R_{k}(x)|\leq {\frac {4|x|^{k+1}}{
      (k+1)!}}\leq {\frac {4}{(k+1)!}},\qquad -1\leq x\leq 1,]
so the required precision is certainly reached, when
           4  ( k + 1 ) !    <  10  &#x2212; 5    &#x27FA;  4 &#x22C5;  10  5
      < ( k + 1 ) !  &#x27FA;  k &#x2265; 9.   {\displaystyle {\frac {4}{
      (k+1)!}}<10^{-5}\quad \Longleftrightarrow \quad 4\cdot 10^{5}<(k+1)!\quad
      \Longleftrightarrow \quad k\geq 9.}  [{\displaystyle {\frac {4}{
      (k+1)!}}<10^{-5}\quad \Longleftrightarrow \quad 4\cdot 10^{5}<(k+1)!\quad
      \Longleftrightarrow \quad k\geq 9.}]
(See factorial or compute by hand the values 9!=362 880 and 10!=3 628 800.) As
a conclusion, Taylor's theorem leads to the approximation
          e  x   = 1 + x +    x  2    2 !    + &#x22EF; +    x  9    9 !    +
      R  9   ( x ) ,   |   R  9   ( x )  |  <  10  &#x2212; 5   ,  &#x2212; 1
      &#x2264; x &#x2264; 1.   {\displaystyle e^{x}=1+x+{\frac {x^{2}}
      {2!}}+\cdots +{\frac {x^{9}}{9!}}+R_{9}(x),\qquad |R_{9}(x)|<10^{-
      5},\qquad -1\leq x\leq 1.}  [{\displaystyle e^{x}=1+x+{\frac {x^{2}}
      {2!}}+\cdots +{\frac {x^{9}}{9!}}+R_{9}(x),\qquad |R_{9}(x)|<10^{-
      5},\qquad -1\leq x\leq 1.}]
For instance, this approximation provides a decimal_expression e â 2.71828,
correct up to five decimal places.
***** Relationship to analyticity[edit] *****
**** Taylor expansions of real analytic functions[edit] ****
Let I â R be an open_interval. By definition, a function f : I â R is real
analytic if it is locally defined by a convergent power_series. This means that
for every a â I there exists some r > 0 and a sequence of coefficients
ck â R such that (a â r, a + r) â I and
         f ( x ) =  &#x2211;  k = 0   &#x221E;    c  k   ( x &#x2212; a  )  k
      =  c  0   +  c  1   ( x &#x2212; a ) +  c  2   ( x &#x2212; a  )  2   +
      &#x22EF; ,   |  x &#x2212; a  |  < r .   {\displaystyle f(x)=\sum _{k=0}^
      {\infty }c_{k}(x-a)^{k}=c_{0}+c_{1}(x-a)+c_{2}(x-a)^{2}+\cdots ,\qquad
      |x-a|<r.}  [f(x)=\sum _{k=0}^{\infty }c_{k}(x-a)^{k}=c_{0}+c_{1}(x-a)+c_
      {2}(x-a)^{2}+\cdots ,\qquad |x-a|<r.]
In general, the radius_of_convergence of a power series can be computed from
the CauchyâHadamard_formula
           1 R   =  lim&#x2006;sup  k &#x2192; &#x221E;    |   c  k     |    1
      k    .   {\displaystyle {\frac {1}{R}}=\limsup _{k\to \infty }|c_{k}|^
      {\frac {1}{k}}.}  [{\frac {1}{R}}=\limsup _{k\to \infty }|c_{k}|^{\frac
      {1}{k}}.]
This result is based on comparison with a geometric_series, and the same method
shows that if the power series based on a converges for some b â R, it must
converge uniformly on the closed_interval [a â rb, a + rb], where
rb = |b â a|. Here only the convergence of the power series is considered,
and it might well be that (a â R,a + R) extends beyond the domain I of f.
The Taylor polynomials of the real analytic function f at a are simply the
finite truncations
          P  k   ( x ) =  &#x2211;  j = 0   k    c  j   ( x &#x2212; a  )  j
      ,   c  j   =     f  ( j )   ( a )   j !      {\displaystyle P_{k}(x)=\sum
      _{j=0}^{k}c_{j}(x-a)^{j},\qquad c_{j}={\frac {f^{(j)}(a)}{j!}}}  [P_{k}
      (x)=\sum _{j=0}^{k}c_{j}(x-a)^{j},\qquad c_{j}={\frac {f^{(j)}(a)}{j!}}]
of its locally defining power series, and the corresponding remainder terms are
locally given by the analytic functions
          R  k   ( x ) =  &#x2211;  j = k + 1   &#x221E;    c  j   ( x &#x2212;
      a  )  j   = ( x &#x2212; a  )  k    h  k   ( x ) ,   |  x &#x2212; a  |
      < r .   {\displaystyle R_{k}(x)=\sum _{j=k+1}^{\infty }c_{j}(x-a)^{j}=(x-
      a)^{k}h_{k}(x),\qquad |x-a|<r.}  [R_{k}(x)=\sum _{j=k+1}^{\infty }c_{j}
      (x-a)^{j}=(x-a)^{k}h_{k}(x),\qquad |x-a|<r.]
Here the functions
           {     h  k   : ( a &#x2212; r , a + r ) &#x2192;  R       h  k   ( x
      ) = ( x &#x2212; a )  &#x2211;  j = 0   &#x221E;    c  k + 1 + j   ( x
      &#x2212; a  )  j           {\displaystyle {\begin{cases}h_{k}:(a-
      r,a+r)\to \mathbf {R} \\h_{k}(x)=(x-a)\sum _{j=0}^{\infty }c_{k+1+j}(x-
      a)^{j}\end{cases}}}  [{\displaystyle {\begin{cases}h_{k}:(a-r,a+r)\to
      \mathbf {R} \\h_{k}(x)=(x-a)\sum _{j=0}^{\infty }c_{k+1+j}(x-a)^{j}\end
      {cases}}}]
are also analytic, since their defining power series have the same radius of
convergence as the original series. Assuming that [a â r, a + r] â I and
r < R, all these series converge uniformly on (a â r, a + r). Naturally, in
the case of analytic functions one can estimate the remainder term Rk(x) by the
tail of the sequence of the derivatives f′(a) at the center of the expansion,
but using complex_analysis also another possibility arises, which is described
below.
**** Taylor's theorem and convergence of Taylor series[edit] ****
The Taylor series of f will converge in some interval, given that all its
derivatives are bounded over it and do not grow too fast as k goes to infinity.
(However, it is not always the case that the Taylor series of f, if it
converges, will in fact converge to f, as explained below; f is then said to be
non-analytic.)
One might think of the Taylor series
         f ( x ) &#x2248;  &#x2211;  k = 0   &#x221E;    c  k   ( x &#x2212; a
      )  k   =  c  0   +  c  1   ( x &#x2212; a ) +  c  2   ( x &#x2212; a  )
      2   + &#x22EF;   {\displaystyle f(x)\approx \sum _{k=0}^{\infty }c_{k}(x-
      a)^{k}=c_{0}+c_{1}(x-a)+c_{2}(x-a)^{2}+\cdots }  [{\displaystyle f
      (x)\approx \sum _{k=0}^{\infty }c_{k}(x-a)^{k}=c_{0}+c_{1}(x-a)+c_{2}(x-
      a)^{2}+\cdots }]
of an infinitely many times differentiable function f : R â R as its
"infinite order Taylor polynomial" at a. Now the estimates_for_the_remainder
imply that if, for any r, the derivatives of f are known to be bounded over
(a â r,a + r), then for any order k and for any r > 0 there exists a constant
Mk,r > 0 such that
         ( &#x2217; )   |   R  k   ( x )  |  &#x2A7D;  M  k , r       |  x
      &#x2212; a   |   k + 1     ( k + 1 ) !      {\displaystyle (*)\quad |R_
      {k}(x)|\leqslant M_{k,r}{\frac {|x-a|^{k+1}}{(k+1)!}}}  [{\displaystyle
      (*)\quad |R_{k}(x)|\leqslant M_{k,r}{\frac {|x-a|^{k+1}}{(k+1)!}}}]
for every x â (a â r,a + r). Sometimes the constants Mk,r can be chosen in
such way that Mk,r is bounded above, for fixed r and all k. Then the Taylor
series of f converges_uniformly to some analytic function
           {     T  f   : ( a &#x2212; r , a + r ) &#x2192;  R       T  f   ( x
      ) =  &#x2211;  k = 0   &#x221E;       f  ( k )   ( a )   k !    ( x
      &#x2212; a  )  k           {\displaystyle {\begin{cases}T_{f}:(a-
      r,a+r)\to \mathbf {R} \\T_{f}(x)=\sum _{k=0}^{\infty }{\frac {f^{(k)}(a)}
      {k!}}(x-a)^{k}\end{cases}}}  [{\displaystyle {\begin{cases}T_{f}:(a-
      r,a+r)\to \mathbf {R} \\T_{f}(x)=\sum _{k=0}^{\infty }{\frac {f^{(k)}(a)}
      {k!}}(x-a)^{k}\end{cases}}}]
(One also gets convergence even if Mk,r is not bounded above as long as it
grows slowly enough.)
However, even though Tf is always analytic, the case may be that f is not. That
is to say, it may well be that an infinitely many times differentiable function
f has a Taylor series at a which converges on some open neighborhood of a, but
the limit function Tf is different from f. An important example of this
phenomenon is provided by the non-analytic_smooth_function known as a flat
function:
           {    f :  R  &#x2192;  R      f ( x ) =   {     e  &#x2212;   1  x
      2         x > 0     0   x &#x2A7D; 0             .   {\displaystyle
      {\begin{cases}f:\mathbf {R} \to \mathbf {R} \\f(x)={\begin{cases}e^{-
      {\frac {1}{x^{2}}}}&x>0\\0&x\leqslant 0\end{cases}}\end{cases}}.}  [
      {\displaystyle {\begin{cases}f:\mathbf {R} \to \mathbf {R} \\f(x)={\begin
      {cases}e^{-{\frac {1}{x^{2}}}}&x>0\\0&x\leqslant 0\end{cases}}\end
      {cases}}.}]
Using the chain_rule one can show by mathematical_induction that for any
order k,
          f  ( k )   ( x ) =   {        p  k   ( x )   x  3 k     &#x22C5;  e
      &#x2212;   1  x  2         x > 0     0   x &#x2A7D; 0
      {\displaystyle f^{(k)}(x)={\begin{cases}{\frac {p_{k}(x)}{x^{3k}}}\cdot
      e^{-{\frac {1}{x^{2}}}}&x>0\\0&x\leqslant 0\end{cases}}}  [{\displaystyle
      f^{(k)}(x)={\begin{cases}{\frac {p_{k}(x)}{x^{3k}}}\cdot e^{-{\frac {1}
      {x^{2}}}}&x>0\\0&x\leqslant 0\end{cases}}}]
for some polynomial pk of degree 2(k â 1). The function      e  &#x2212;   1
x  2         {\displaystyle e^{-{\frac {1}{x^{2}}}}}  [e^{-{\frac {1}{x^{2}}}}]
tends to zero faster than any polynomial as x â 0, so f is infinitely many
times differentiable and f(k)(0) = 0 for every positive integer k. Now the
estimates for the remainder for the Taylor polynomials show that the Taylor
series of f converges uniformly to the zero function on the whole real axis.
Nothing is wrong in here:
    * The Taylor series of f converges uniformly to the zero function Tf
      (x) = 0.
    * The zero function is analytic and every coefficient in its Taylor series
      is zero.
    * The function f is infinitely many times differentiable, but not analytic.
    * For any k â N and r > 0 there exists Mk,r > 0 such that the remainder
      term for the k-th order Taylor polynomial of f satisfies (*), and is
      bounded above, for all k and fixed r.
**** Taylor's theorem in complex analysis[edit] ****
Taylor's theorem generalizes to functions f : C â C which are complex
differentiable in an open subset U â C of the complex_plane. However, its
usefulness is dwarfed by other general theorems in complex_analysis. Namely,
stronger versions of related results can be deduced for complex_differentiable
functions f : U â C using Cauchy's_integral_formula as follows.
Let r > 0 such that the closed_disk B(z, r) âª S(z, r) is contained in U. Then
Cauchy's integral formula with a positive parametrization γ(t)=z + reit of the
circle S(z, r) with t â [0, 2Ï] gives
         f ( z ) =   1  2 &#x03C0; i     &#x222B;  &#x03B3;      f ( w )   w
      &#x2212; z     d w ,   f &#x2032;  ( z ) =   1  2 &#x03C0; i     &#x222B;
      &#x03B3;      f ( w )   ( w &#x2212; z  )  2       d w ,  &#x2026; ,   f
      ( k )   ( z ) =    k !   2 &#x03C0; i     &#x222B;  &#x03B3;      f ( w )
      ( w &#x2212; z  )  k + 1       d w .   {\displaystyle f(z)={\frac {1}
      {2\pi i}}\int _{\gamma }{\frac {f(w)}{w-z}}\,dw,\quad f'(z)={\frac {1}
      {2\pi i}}\int _{\gamma }{\frac {f(w)}{(w-z)^{2}}}\,dw,\quad \ldots ,\quad
      f^{(k)}(z)={\frac {k!}{2\pi i}}\int _{\gamma }{\frac {f(w)}{(w-z)^
      {k+1}}}\,dw.}  [{\displaystyle f(z)={\frac {1}{2\pi i}}\int _{\gamma }
      {\frac {f(w)}{w-z}}\,dw,\quad f'(z)={\frac {1}{2\pi i}}\int _{\gamma }
      {\frac {f(w)}{(w-z)^{2}}}\,dw,\quad \ldots ,\quad f^{(k)}(z)={\frac {k!}
      {2\pi i}}\int _{\gamma }{\frac {f(w)}{(w-z)^{k+1}}}\,dw.}]
Here all the integrands are continuous on the circle S(z, r), which justifies
differentiation under the integral sign. In particular, if f is once complex
differentiable on the open set U, then it is actually infinitely many times
complex_differentiable on U. One also obtains the Cauchy's estimates[11]
          |   f  ( k )   ( z )  |  &#x2A7D;    k !   2 &#x03C0;     &#x222B;
      &#x03B3;      M  r     |  w &#x2212; z   |   k + 1       d w =    k !  M
      r     r  k     ,   M  r   =  max   |  w &#x2212; c  |  = r    |  f ( w )
      |    {\displaystyle |f^{(k)}(z)|\leqslant {\frac {k!}{2\pi }}\int _
      {\gamma }{\frac {M_{r}}{|w-z|^{k+1}}}\,dw={\frac {k!M_{r}}{r^{k}}},\quad
      M_{r}=\max _{|w-c|=r}|f(w)|}  [{\displaystyle |f^{(k)}(z)|\leqslant
      {\frac {k!}{2\pi }}\int _{\gamma }{\frac {M_{r}}{|w-z|^{k+1}}}\,dw={\frac
      {k!M_{r}}{r^{k}}},\quad M_{r}=\max _{|w-c|=r}|f(w)|}]
for any z â U and r > 0 such that B(z, r) âª S(c, r) â U. These estimates
imply that the complex Taylor_series
          T  f   ( z ) =  &#x2211;  k = 0   &#x221E;       f  ( k )   ( c )   k
      !    ( z &#x2212; c  )  k     {\displaystyle T_{f}(z)=\sum _{k=0}^{\infty
      }{\frac {f^{(k)}(c)}{k!}}(z-c)^{k}}  [T_{f}(z)=\sum _{k=0}^{\infty }
      {\frac {f^{(k)}(c)}{k!}}(z-c)^{k}]
of f converges uniformly on any open_disk B(c, r) â U with S(c, r) â U into
some function Tf. Furthermore, using the contour integral formulae for the
derivatives f(k)(c),
              T  f   ( z )    =  &#x2211;  k = 0   &#x221E;      ( z &#x2212; c
      )  k     2 &#x03C0; i     &#x222B;  &#x03B3;      f ( w )   ( w &#x2212;
      c  )  k + 1       d w       =   1  2 &#x03C0; i     &#x222B;  &#x03B3;
      f ( w )   w &#x2212; c     &#x2211;  k = 0   &#x221E;     (    z &#x2212;
      c   w &#x2212; c    )   k    d w       =   1  2 &#x03C0; i     &#x222B;
      &#x03B3;      f ( w )   w &#x2212; c     (   1  1 &#x2212;    z &#x2212;
      c   w &#x2212; c       )   d w       =   1  2 &#x03C0; i     &#x222B;
      &#x03B3;      f ( w )   w &#x2212; z     d w = f ( z ) ,
      {\displaystyle {\begin{aligned}T_{f}(z)&=\sum _{k=0}^{\infty }{\frac {(z-
      c)^{k}}{2\pi i}}\int _{\gamma }{\frac {f(w)}{(w-c)^{k+1}}}\,dw\\&={\frac
      {1}{2\pi i}}\int _{\gamma }{\frac {f(w)}{w-c}}\sum _{k=0}^{\infty }\left(
      {\frac {z-c}{w-c}}\right)^{k}\,dw\\&={\frac {1}{2\pi i}}\int _{\gamma }
      {\frac {f(w)}{w-c}}\left({\frac {1}{1-{\frac {z-c}{w-c}}}}\right)\,dw\\&=
      {\frac {1}{2\pi i}}\int _{\gamma }{\frac {f(w)}{w-z}}\,dw=f(z),\end
      {aligned}}}  [{\displaystyle {\begin{aligned}T_{f}(z)&=\sum _{k=0}^
      {\infty }{\frac {(z-c)^{k}}{2\pi i}}\int _{\gamma }{\frac {f(w)}{(w-c)^
      {k+1}}}\,dw\\&={\frac {1}{2\pi i}}\int _{\gamma }{\frac {f(w)}{w-c}}\sum
      _{k=0}^{\infty }\left({\frac {z-c}{w-c}}\right)^{k}\,dw\\&={\frac {1}
      {2\pi i}}\int _{\gamma }{\frac {f(w)}{w-c}}\left({\frac {1}{1-{\frac {z-
      c}{w-c}}}}\right)\,dw\\&={\frac {1}{2\pi i}}\int _{\gamma }{\frac {f(w)}
      {w-z}}\,dw=f(z),\end{aligned}}}]
so any complex_differentiable function f in an open set U â C is in fact
complex_analytic. All that is said for real analytic functions here holds also
for complex analytic functions with the open interval I replaced by an open
subset U â C and a-centered intervals (a â r, a + r) replaced by c-centered
disks B(c, r). In particular, the Taylor expansion holds in the form
         f ( z ) =  P  k   ( z ) +  R  k   ( z ) ,   P  k   ( z ) =  &#x2211;
      j = 0   k       f  ( j )   ( c )   j !    ( z &#x2212; c  )  j   ,
      {\displaystyle f(z)=P_{k}(z)+R_{k}(z),\quad P_{k}(z)=\sum _{j=0}^{k}
      {\frac {f^{(j)}(c)}{j!}}(z-c)^{j},}  [f(z)=P_{k}(z)+R_{k}(z),\quad P_{k}
      (z)=\sum _{j=0}^{k}{\frac {f^{(j)}(c)}{j!}}(z-c)^{j},]
where the remainder term Rk is complex analytic. Methods of complex analysis
provide some powerful results regarding Taylor expansions. For example, using
Cauchy's integral formula for any positively oriented Jordan_curve γ which
parametrizes the boundary âW â U of a region W â U, one obtains
expressions for the derivatives f(j)(c) as above, and modifying slightly the
computation for Tf(z) = f(z), one arrives at the exact formula
          R  k   ( z ) =  &#x2211;  j = k + 1   &#x221E;      ( z &#x2212; c  )
      j     2 &#x03C0; i     &#x222B;  &#x03B3;      f ( w )   ( w &#x2212; c
      )  j + 1       d w =    ( z &#x2212; c  )  k + 1     2 &#x03C0; i
      &#x222B;  &#x03B3;      f ( w )  d w   ( w &#x2212; c  )  k + 1   ( w
      &#x2212; z )    ,  z &#x2208; W .   {\displaystyle R_{k}(z)=\sum _
      {j=k+1}^{\infty }{\frac {(z-c)^{j}}{2\pi i}}\int _{\gamma }{\frac {f(w)}{
      (w-c)^{j+1}}}\,dw={\frac {(z-c)^{k+1}}{2\pi i}}\int _{\gamma }{\frac {f
      (w)\,dw}{(w-c)^{k+1}(w-z)}},\qquad z\in W.}  [{\displaystyle R_{k}
      (z)=\sum _{j=k+1}^{\infty }{\frac {(z-c)^{j}}{2\pi i}}\int _{\gamma }
      {\frac {f(w)}{(w-c)^{j+1}}}\,dw={\frac {(z-c)^{k+1}}{2\pi i}}\int _
      {\gamma }{\frac {f(w)\,dw}{(w-c)^{k+1}(w-z)}},\qquad z\in W.}]
The important feature here is that the quality of the approximation by a Taylor
polynomial on the region W â U is dominated by the values of the function f
itself on the boundary âW â U. Similarly, applying Cauchy's estimates to
the series expression for the remainder, one obtains the uniform estimates
          |   R  k   ( z )  |  &#x2A7D;  &#x2211;  j = k + 1   &#x221E;       M
      r    |  z &#x2212; c   |   j     r  j     =    M  r    r  k + 1         |
      z &#x2212; c   |   k + 1     1 &#x2212;     |  z &#x2212; c  |   r
      &#x2A7D;     M  r    &#x03B2;  k + 1     1 &#x2212; &#x03B2;    ,      |
      z &#x2212; c  |   r   &#x2A7D; &#x03B2; < 1.   {\displaystyle |R_{k}
      (z)|\leqslant \sum _{j=k+1}^{\infty }{\frac {M_{r}|z-c|^{j}}{r^{j}}}=
      {\frac {M_{r}}{r^{k+1}}}{\frac {|z-c|^{k+1}}{1-{\frac {|z-c|}
      {r}}}}\leqslant {\frac {M_{r}\beta ^{k+1}}{1-\beta }},\qquad {\frac {|z-
      c|}{r}}\leqslant \beta <1.}  [{\displaystyle |R_{k}(z)|\leqslant \sum _
      {j=k+1}^{\infty }{\frac {M_{r}|z-c|^{j}}{r^{j}}}={\frac {M_{r}}{r^{k+1}}}
      {\frac {|z-c|^{k+1}}{1-{\frac {|z-c|}{r}}}}\leqslant {\frac {M_{r}\beta ^
      {k+1}}{1-\beta }},\qquad {\frac {|z-c|}{r}}\leqslant \beta <1.}]
**** Example[edit] ****
Complex plot of f(z) = 1/(1 + z2). Modulus is shown by elevation and argument
by coloring: cyan=0, blue = Ï/3, violet = 2Ï/3, red = Ï, yellow=4Ï/3,
green=5Ï/3.
The function
           {    f :  R  &#x2192;  R      f ( x ) =   1  1 +  x  2
      {\displaystyle {\begin{cases}f:\mathbf {R} \to \mathbf {R} \\f(x)={\frac
      {1}{1+x^{2}}}\end{cases}}}  [{\displaystyle {\begin{cases}f:\mathbf {R}
      \to \mathbf {R} \\f(x)={\frac {1}{1+x^{2}}}\end{cases}}}]
is real_analytic, that is, locally determined by its Taylor series. This
function was plotted above to illustrate the fact that some elementary
functions cannot be approximated by Taylor polynomials in neighborhoods of the
center of expansion which are too large. This kind of behavior is easily
understood in the framework of complex analysis. Namely, the function f extends
into a meromorphic_function
           {    f :  C  &#x222A; { &#x221E; } &#x2192;  C  &#x222A; { &#x221E;
      }     f ( z ) =   1  1 +  z  2              {\displaystyle {\begin
      {cases}f:\mathbf {C} \cup \{\infty \}\to \mathbf {C} \cup \{\infty \}\\f
      (z)={\frac {1}{1+z^{2}}}\end{cases}}}  [{\displaystyle {\begin{cases}f:
      \mathbf {C} \cup \{\infty \}\to \mathbf {C} \cup \{\infty \}\\f(z)={\frac
      {1}{1+z^{2}}}\end{cases}}}]
on the compactified complex plane. It has simple poles at z = i and z = âi,
and it is analytic elsewhere. Now its Taylor series centered at z0 converges on
any disc B(z0, r) with r < |z â z0|, where the same Taylor series converges
at z â C. Therefore, Taylor series of f centered at 0 converges on B(0, 1)
and it does not converge for any z â C with |z| > 1 due to the poles at i and
âi. For the same reason the Taylor series of f centered at 1 converges on B
(1, â2) and does not converge for any z â C with |z â 1| > â2.
***** Generalizations of Taylor's theorem[edit] *****
**** Higher-order differentiability[edit] ****
A function f: Rn â R is differentiable at a â Rn if_and_only_if there
exists a linear_functional L : Rn â R and a function h : Rn â R such that
         f (  x  ) = f (  a  ) + L (  x  &#x2212;  a  ) + h (  x  )  |   x
      &#x2212;  a   |  ,   lim   x  &#x2192;  a    h (  x  ) = 0.
      {\displaystyle f({\boldsymbol {x}})=f({\boldsymbol {a}})+L({\boldsymbol
      {x}}-{\boldsymbol {a}})+h({\boldsymbol {x}})|{\boldsymbol {x}}-
      {\boldsymbol {a}}|,\qquad \lim _{{\boldsymbol {x}}\to {\boldsymbol {a}}}h
      ({\boldsymbol {x}})=0.}  [{\displaystyle f({\boldsymbol {x}})=f(
      {\boldsymbol {a}})+L({\boldsymbol {x}}-{\boldsymbol {a}})+h({\boldsymbol
      {x}})|{\boldsymbol {x}}-{\boldsymbol {a}}|,\qquad \lim _{{\boldsymbol
      {x}}\to {\boldsymbol {a}}}h({\boldsymbol {x}})=0.}]
If this is the case, then L = df(a) is the (uniquely defined) differential of f
at the point a. Furthermore, then the partial_derivatives of f exist at a and
the differential of f at a is given by
         d f (  a  ) (  v  ) =    &#x2202; f   &#x2202;  x  1      (  a  )  v
      1   + &#x22EF; +    &#x2202; f   &#x2202;  x  n      (  a  )  v  n   .
      {\displaystyle df({\boldsymbol {a}})({\boldsymbol {v}})={\frac {\partial
      f}{\partial x_{1}}}({\boldsymbol {a}})v_{1}+\cdots +{\frac {\partial f}
      {\partial x_{n}}}({\boldsymbol {a}})v_{n}.}  [df({\boldsymbol {a}})(
      {\boldsymbol {v}})={\frac {\partial f}{\partial x_{1}}}({\boldsymbol
      {a}})v_{1}+\cdots +{\frac {\partial f}{\partial x_{n}}}({\boldsymbol
      {a}})v_{n}.]
Introduce the multi-index_notation
          |  &#x03B1;  |  =  &#x03B1;  1   + &#x22EF; +  &#x03B1;  n   ,
      &#x03B1; ! =  &#x03B1;  1   ! &#x22EF;  &#x03B1;  n   ! ,    x   &#x03B1;
      =  x  1    &#x03B1;  1     &#x22EF;  x  n    &#x03B1;  n
      {\displaystyle |\alpha |=\alpha _{1}+\cdots +\alpha _{n},\quad \alpha
      !=\alpha _{1}!\cdots \alpha _{n}!,\quad {\boldsymbol {x}}^{\alpha }=x_
      {1}^{\alpha _{1}}\cdots x_{n}^{\alpha _{n}}}  [|\alpha |=\alpha _
      {1}+\cdots +\alpha _{n},\quad \alpha !=\alpha _{1}!\cdots \alpha _
      {n}!,\quad {\boldsymbol {x}}^{\alpha }=x_{1}^{\alpha _{1}}\cdots x_{n}^
      {\alpha _{n}}]
for α â Nn and x â Rn. If all the k-th order partial_derivatives of f : Rn
→ R are continuous at a ∈ Rn, then by Clairaut's_theorem, one can change the
order of mixed derivatives at a, so the notation
          D  &#x03B1;   f =     &#x2202;   |  &#x03B1;  |    f   &#x2202;  x  1
      &#x03B1;  1     &#x22EF; &#x2202;  x  n    &#x03B1;  n        ,   |
      &#x03B1;  |  &#x2264; k   {\displaystyle D^{\alpha }f={\frac {\partial ^
      {|\alpha |}f}{\partial x_{1}^{\alpha _{1}}\cdots \partial x_{n}^{\alpha _
      {n}}}},\qquad |\alpha |\leq k}  [D^{\alpha }f={\frac {\partial ^{|\alpha
      |}f}{\partial x_{1}^{\alpha _{1}}\cdots \partial x_{n}^{\alpha _
      {n}}}},\qquad |\alpha |\leq k]
for the higher order partial_derivatives is justified in this situation. The
same is true if all the (k − 1)-th order partial derivatives of f exist in some
neighborhood of a and are differentiable at a.[12] Then we say that f is k
times differentiable at the point a.
**** Taylor's theorem for multivariate functions[edit] ****
     Multivariate version of Taylor's theorem.[13] Let f : Rn → R be a k
     times differentiable function at the point a∈Rn. Then there exists
     hα : Rn→R such that
                   f (  x  ) =  &#x2211;   |  &#x03B1;  |  &#x2264; k
           D  &#x03B1;   f (  a  )   &#x03B1; !    (  x  &#x2212;  a   )
           &#x03B1;   +  &#x2211;   |  &#x03B1;  |  = k    h  &#x03B1;
           (  x  ) (  x  &#x2212;  a   )  &#x03B1;   ,        and     lim
           x  &#x2192;  a     h  &#x03B1;   (  x  ) = 0.
           {\displaystyle {\begin{aligned}&f({\boldsymbol {x}})=\sum _
           {|\alpha |\leq k}{\frac {D^{\alpha }f({\boldsymbol {a}})}
           {\alpha !}}({\boldsymbol {x}}-{\boldsymbol {a}})^{\alpha }+\sum
           _{|\alpha |=k}h_{\alpha }({\boldsymbol {x}})({\boldsymbol {x}}-
           {\boldsymbol {a}})^{\alpha },\\&{\mbox{and}}\quad \lim _{
           {\boldsymbol {x}}\to {\boldsymbol {a}}}h_{\alpha }({\boldsymbol
           {x}})=0.\end{aligned}}}  [{\begin{aligned}&f({\boldsymbol
           {x}})=\sum _{|\alpha |\leq k}{\frac {D^{\alpha }f({\boldsymbol
           {a}})}{\alpha !}}({\boldsymbol {x}}-{\boldsymbol {a}})^{\alpha
           }+\sum _{|\alpha |=k}h_{\alpha }({\boldsymbol {x}})(
           {\boldsymbol {x}}-{\boldsymbol {a}})^{\alpha },\\&{\mbox
           {and}}\quad \lim _{{\boldsymbol {x}}\to {\boldsymbol {a}}}h_
           {\alpha }({\boldsymbol {x}})=0.\end{aligned}}]
If the function f : Rn → R is k + 1 times continuously_differentiable in the
closed_ball B, then one can derive an exact formula for the remainder in terms
of (k+1)-th order partial_derivatives of f in this neighborhood. Namely,
              f (  x  ) =  &#x2211;   |  &#x03B1;  |  &#x2264; k       D
      &#x03B1;   f (  a  )   &#x03B1; !    (  x  &#x2212;  a   )  &#x03B1;   +
      &#x2211;   |  &#x03B2;  |  = k + 1    R  &#x03B2;   (  x  ) (  x
      &#x2212;  a   )  &#x03B2;   ,       R  &#x03B2;   (  x  ) =     |
      &#x03B2;  |    &#x03B2; !     &#x222B;  0   1   ( 1 &#x2212; t  )   |
      &#x03B2;  |  &#x2212; 1    D  &#x03B2;   f   (    a  + t (  x  &#x2212;
      a  )   )    d t .       {\displaystyle {\begin{aligned}&f({\boldsymbol
      {x}})=\sum _{|\alpha |\leq k}{\frac {D^{\alpha }f({\boldsymbol {a}})}
      {\alpha !}}({\boldsymbol {x}}-{\boldsymbol {a}})^{\alpha }+\sum _{|\beta
      |=k+1}R_{\beta }({\boldsymbol {x}})({\boldsymbol {x}}-{\boldsymbol {a}})^
      {\beta },\\&R_{\beta }({\boldsymbol {x}})={\frac {|\beta |}{\beta !}}\int
      _{0}^{1}(1-t)^{|\beta |-1}D^{\beta }f{\big (}{\boldsymbol {a}}+t(
      {\boldsymbol {x}}-{\boldsymbol {a}}){\big )}\,dt.\end{aligned}}}  [
      {\begin{aligned}&f({\boldsymbol {x}})=\sum _{|\alpha |\leq k}{\frac {D^
      {\alpha }f({\boldsymbol {a}})}{\alpha !}}({\boldsymbol {x}}-{\boldsymbol
      {a}})^{\alpha }+\sum _{|\beta |=k+1}R_{\beta }({\boldsymbol {x}})(
      {\boldsymbol {x}}-{\boldsymbol {a}})^{\beta },\\&R_{\beta }({\boldsymbol
      {x}})={\frac {|\beta |}{\beta !}}\int _{0}^{1}(1-t)^{|\beta |-1}D^{\beta
      }f{\big (}{\boldsymbol {a}}+t({\boldsymbol {x}}-{\boldsymbol {a}}){\big
      )}\,dt.\end{aligned}}]
In this case, due to the continuity of (k+1)-th order partial_derivatives in
the compact_set B, one immediately obtains the uniform estimates
          |   R  &#x03B2;   (  x  )  |  &#x2264;   1  &#x03B2; !     max   |
      &#x03B1;  |  =  |  &#x03B2;  |     max   y  &#x2208; B    |   D  &#x03B1;
      f (  y  )  |  ,   x  &#x2208; B .   {\displaystyle \left|R_{\beta }(
      {\boldsymbol {x}})\right|\leq {\frac {1}{\beta !}}\max _{|\alpha |=|\beta
      |}\max _{{\boldsymbol {y}}\in B}|D^{\alpha }f({\boldsymbol {y}})|,\qquad
      {\boldsymbol {x}}\in B.}  [\left|R_{\beta }({\boldsymbol {x}})\right|\leq
      {\frac {1}{\beta !}}\max _{|\alpha |=|\beta |}\max _{{\boldsymbol {y}}\in
      B}|D^{\alpha }f({\boldsymbol {y}})|,\qquad {\boldsymbol {x}}\in B.]
**** Example in two dimensions[edit] ****
For example, the third-order Taylor polynomial of a smooth function f: R2 â R
is, denoting x − a = v,
              P  3   (  x  ) = f (  a  ) +        &#x2202; f   &#x2202;  x  1
      (  a  )  v  1   +    &#x2202; f   &#x2202;  x  2      (  a  )  v  2   +
      &#x2202;  2   f   &#x2202;  x  1   2      (  a  )    v  1   2    2 !    +
      &#x2202;  2   f   &#x2202;  x  1   &#x2202;  x  2      (  a  )  v  1    v
      2   +     &#x2202;  2   f   &#x2202;  x  2   2      (  a  )    v  2   2
      2 !          +     &#x2202;  3   f   &#x2202;  x  1   3      (  a  )    v
      1   3    3 !    +     &#x2202;  3   f   &#x2202;  x  1   2   &#x2202;  x
      2      (  a  )     v  1   2    v  2     2 !    +     &#x2202;  3   f
      &#x2202;  x  1   &#x2202;  x  2   2      (  a  )     v  1    v  2   2
      2 !    +     &#x2202;  3   f   &#x2202;  x  2   3      (  a  )    v  2
      3    3 !          {\displaystyle {\begin{aligned}P_{3}({\boldsymbol
      {x}})=f({\boldsymbol {a}})+{}&{\frac {\partial f}{\partial x_{1}}}(
      {\boldsymbol {a}})v_{1}+{\frac {\partial f}{\partial x_{2}}}({\boldsymbol
      {a}})v_{2}+{\frac {\partial ^{2}f}{\partial x_{1}^{2}}}({\boldsymbol
      {a}}){\frac {v_{1}^{2}}{2!}}+{\frac {\partial ^{2}f}{\partial x_
      {1}\partial x_{2}}}({\boldsymbol {a}})v_{1}v_{2}+{\frac {\partial ^{2}f}
      {\partial x_{2}^{2}}}({\boldsymbol {a}}){\frac {v_{2}^{2}}{2!}}\\&+{\frac
      {\partial ^{3}f}{\partial x_{1}^{3}}}({\boldsymbol {a}}){\frac {v_{1}^
      {3}}{3!}}+{\frac {\partial ^{3}f}{\partial x_{1}^{2}\partial x_{2}}}(
      {\boldsymbol {a}}){\frac {v_{1}^{2}v_{2}}{2!}}+{\frac {\partial ^{3}f}
      {\partial x_{1}\partial x_{2}^{2}}}({\boldsymbol {a}}){\frac {v_{1}v_{2}^
      {2}}{2!}}+{\frac {\partial ^{3}f}{\partial x_{2}^{3}}}({\boldsymbol {a}})
      {\frac {v_{2}^{3}}{3!}}\end{aligned}}}  [{\displaystyle {\begin
      {aligned}P_{3}({\boldsymbol {x}})=f({\boldsymbol {a}})+{}&{\frac
      {\partial f}{\partial x_{1}}}({\boldsymbol {a}})v_{1}+{\frac {\partial f}
      {\partial x_{2}}}({\boldsymbol {a}})v_{2}+{\frac {\partial ^{2}f}
      {\partial x_{1}^{2}}}({\boldsymbol {a}}){\frac {v_{1}^{2}}{2!}}+{\frac
      {\partial ^{2}f}{\partial x_{1}\partial x_{2}}}({\boldsymbol {a}})v_{1}v_
      {2}+{\frac {\partial ^{2}f}{\partial x_{2}^{2}}}({\boldsymbol {a}}){\frac
      {v_{2}^{2}}{2!}}\\&+{\frac {\partial ^{3}f}{\partial x_{1}^{3}}}(
      {\boldsymbol {a}}){\frac {v_{1}^{3}}{3!}}+{\frac {\partial ^{3}f}
      {\partial x_{1}^{2}\partial x_{2}}}({\boldsymbol {a}}){\frac {v_{1}^{2}v_
      {2}}{2!}}+{\frac {\partial ^{3}f}{\partial x_{1}\partial x_{2}^{2}}}(
      {\boldsymbol {a}}){\frac {v_{1}v_{2}^{2}}{2!}}+{\frac {\partial ^{3}f}
      {\partial x_{2}^{3}}}({\boldsymbol {a}}){\frac {v_{2}^{3}}{3!}}\end
      {aligned}}}]
***** Proofs[edit] *****
**** Proof for Taylor's theorem in one real variable[edit] ****
Let[14]
          h  k   ( x ) =   {       f ( x ) &#x2212; P ( x )   ( x &#x2212; a  )
      k        x &#x2260; a     0   x = a         {\displaystyle h_{k}(x)=
      {\begin{cases}{\frac {f(x)-P(x)}{(x-a)^{k}}}&x\not =a\\0&x=a\end{cases}}}
      [h_{k}(x)={\begin{cases}{\frac {f(x)-P(x)}{(x-a)^{k}}}&x\not
      =a\\0&x=a\end{cases}}]
where, as in the statement of Taylor's theorem,
         P ( x ) = f ( a ) +  f &#x2032;  ( a ) ( x &#x2212; a ) +     f
      &#x2033;  ( a )   2 !    ( x &#x2212; a  )  2   + &#x22EF; +     f  ( k )
      ( a )   k !    ( x &#x2212; a  )  k   .   {\displaystyle P(x)=f(a)+f'(a)
      (x-a)+{\frac {f''(a)}{2!}}(x-a)^{2}+\cdots +{\frac {f^{(k)}(a)}{k!}}(x-
      a)^{k}.}  [P(x)=f(a)+f'(a)(x-a)+{\frac {f''(a)}{2!}}(x-a)^{2}+\cdots +
      {\frac {f^{(k)}(a)}{k!}}(x-a)^{k}.]
It is sufficient to show that
          lim  x &#x2192; a    h  k   ( x ) = 0.   {\displaystyle \lim _{x\to
      a}h_{k}(x)=0.}  [{\displaystyle \lim _{x\to a}h_{k}(x)=0.}]
The proof here is based on repeated application of L'HÃ´pital's_rule. Note
that, for each j = 0,1,...,k−1,      f  ( j )   ( a ) =  P  ( j )   ( a )
{\displaystyle f^{(j)}(a)=P^{(j)}(a)}  [f^{(j)}(a)=P^{(j)}(a)]. Hence each of
the first k−1 derivatives of the numerator in      h  k   ( x )
{\displaystyle h_{k}(x)}  [h_{k}(x)] vanishes at     x = a   {\displaystyle
x=a}  [x=a], and the same is true of the denominator. Also, since the condition
that the function f be k times differentiable at a point requires
differentiability up to order kâ1 in a neighborhood of said point (this is
true, because differentiability requires a function to be defined in a whole
neighborhood of a point), the numerator and its k â 2 derivatives are
differentiable in a neighborhood of a. Clearly, the denominator also satisfies
said condition, and additionally, doesn't vanish unless x=a, therefore all
conditions necessary for L'Hopital's rule are fulfilled, and its use is
justified. So
              lim  x &#x2192; a      f ( x ) &#x2212; P ( x )   ( x &#x2212; a
      )  k         =  lim  x &#x2192; a        d  d x    ( f ( x ) &#x2212; P
      ( x ) )     d  d x    ( x &#x2212; a  )  k      = &#x22EF; =  lim  x
      &#x2192; a         d  k &#x2212; 1    d  x  k &#x2212; 1      ( f ( x )
      &#x2212; P ( x ) )      d  k &#x2212; 1    d  x  k &#x2212; 1      ( x
      &#x2212; a  )  k            =   1  k !     lim  x &#x2192; a       f  ( k
      &#x2212; 1 )   ( x ) &#x2212;  P  ( k &#x2212; 1 )   ( x )   x &#x2212; a
      =   1  k !    (  f  ( k )   ( a ) &#x2212;  f  ( k )   ( a ) ) = 0
      {\displaystyle {\begin{aligned}\lim _{x\to a}{\frac {f(x)-P(x)}{(x-a)^
      {k}}}&=\lim _{x\to a}{\frac {{\frac {d}{dx}}(f(x)-P(x))}{{\frac {d}{dx}}
      (x-a)^{k}}}=\cdots =\lim _{x\to a}{\frac {{\frac {d^{k-1}}{dx^{k-1}}}(f
      (x)-P(x))}{{\frac {d^{k-1}}{dx^{k-1}}}(x-a)^{k}}}\\&={\frac {1}{k!}}\lim
      _{x\to a}{\frac {f^{(k-1)}(x)-P^{(k-1)}(x)}{x-a}}\\&={\frac {1}{k!}}(f^{
      (k)}(a)-f^{(k)}(a))=0\end{aligned}}}  [{\begin{aligned}\lim _{x\to a}
      {\frac {f(x)-P(x)}{(x-a)^{k}}}&=\lim _{x\to a}{\frac {{\frac {d}{dx}}(f
      (x)-P(x))}{{\frac {d}{dx}}(x-a)^{k}}}=\cdots =\lim _{x\to a}{\frac {
      {\frac {d^{k-1}}{dx^{k-1}}}(f(x)-P(x))}{{\frac {d^{k-1}}{dx^{k-1}}}(x-a)^
      {k}}}\\&={\frac {1}{k!}}\lim _{x\to a}{\frac {f^{(k-1)}(x)-P^{(k-1)}(x)}
      {x-a}}\\&={\frac {1}{k!}}(f^{(k)}(a)-f^{(k)}(a))=0\end{aligned}}]
where the second to last equality follows by the definition of the derivative
at x = a.
**** Derivation for the mean value forms of the remainder[edit] ****
Let G be any real-valued function, continuous on the closed interval between a
and x and differentiable with a non-vanishing derivative on the open interval
between a and x, and define
         F ( t ) = f ( t ) +  f &#x2032;  ( t ) ( x &#x2212; t ) +     f
      &#x2033;  ( t )   2 !    ( x &#x2212; t  )  2   + &#x22EF; +     f  ( k )
      ( t )   k !    ( x &#x2212; t  )  k   .   {\displaystyle F(t)=f(t)+f'(t)
      (x-t)+{\frac {f''(t)}{2!}}(x-t)^{2}+\cdots +{\frac {f^{(k)}(t)}{k!}}(x-
      t)^{k}.}  [F(t)=f(t)+f'(t)(x-t)+{\frac {f''(t)}{2!}}(x-t)^{2}+\cdots +
      {\frac {f^{(k)}(t)}{k!}}(x-t)^{k}.]
For     t &#x2208; [ a , x ]   {\displaystyle t\in [a,x]}  [{\displaystyle t\in
[a,x]}]. Then, by Cauchy's_mean_value_theorem,
         ( &#x2217; )      F &#x2032;  ( &#x03BE; )    G &#x2032;  ( &#x03BE; )
      =    F ( x ) &#x2212; F ( a )   G ( x ) &#x2212; G ( a )
      {\displaystyle (*)\quad {\frac {F'(\xi )}{G'(\xi )}}={\frac {F(x)-F(a)}{G
      (x)-G(a)}}}  [(*)\quad {\frac {F'(\xi )}{G'(\xi )}}={\frac {F(x)-F(a)}{G
      (x)-G(a)}}]
for some Î¾ on the open interval between a and x. Note that here the numerator
F(x) â F(a) = Rk(x) is exactly the remainder of the Taylor polynomial for f
(x). Compute
              F &#x2032;  ( t ) =      f &#x2032;  ( t ) +   (    f &#x2033;
      ( t ) ( x &#x2212; t ) &#x2212;  f &#x2032;  ( t )   )   +  (      f  ( 3
      )   ( t )   2 !    ( x &#x2212; t  )  2   &#x2212;     f  ( 2 )   ( t )
      1 !    ( x &#x2212; t )  )  + &#x22EF;       &#x22EF; +  (      f  ( k +
      1 )   ( t )   k !    ( x &#x2212; t  )  k   &#x2212;     f  ( k )   ( t )
      ( k &#x2212; 1 ) !    ( x &#x2212; t  )  k &#x2212; 1    )  =     f  ( k
      + 1 )   ( t )   k !    ( x &#x2212; t  )  k   ,       {\displaystyle
      {\begin{aligned}F'(t)={}&f'(t)+{\big (}f''(t)(x-t)-f'(t){\big )}+\left(
      {\frac {f^{(3)}(t)}{2!}}(x-t)^{2}-{\frac {f^{(2)}(t)}{1!}}(x-
      t)\right)+\cdots \\&\cdots +\left({\frac {f^{(k+1)}(t)}{k!}}(x-t)^{k}-
      {\frac {f^{(k)}(t)}{(k-1)!}}(x-t)^{k-1}\right)={\frac {f^{(k+1)}(t)}{k!}}
      (x-t)^{k},\end{aligned}}}  [{\displaystyle {\begin{aligned}F'(t)={}&f'
      (t)+{\big (}f''(t)(x-t)-f'(t){\big )}+\left({\frac {f^{(3)}(t)}{2!}}(x-
      t)^{2}-{\frac {f^{(2)}(t)}{1!}}(x-t)\right)+\cdots \\&\cdots +\left(
      {\frac {f^{(k+1)}(t)}{k!}}(x-t)^{k}-{\frac {f^{(k)}(t)}{(k-1)!}}(x-t)^{k-
      1}\right)={\frac {f^{(k+1)}(t)}{k!}}(x-t)^{k},\end{aligned}}}]
plug it into (*) and rearrange terms to find that
          R  k   ( x ) =     f  ( k + 1 )   ( &#x03BE; )   k !    ( x &#x2212;
      &#x03BE;  )  k      G ( x ) &#x2212; G ( a )    G &#x2032;  ( &#x03BE; )
      .   {\displaystyle R_{k}(x)={\frac {f^{(k+1)}(\xi )}{k!}}(x-\xi )^{k}
      {\frac {G(x)-G(a)}{G'(\xi )}}.}  [R_{k}(x)={\frac {f^{(k+1)}(\xi )}{k!}}
      (x-\xi )^{k}{\frac {G(x)-G(a)}{G'(\xi )}}.]
This is the form of the remainder term mentioned after the actual statement of
Taylor's theorem with remainder in the mean value form. The Lagrange form of
the remainder is found by choosing     &#xA0; G ( t ) = ( t &#x2212; x  )  k +
1     {\displaystyle \ G(t)=(t-x)^{k+1}}  [{\displaystyle \ G(t)=(t-x)^{k+1}}]
and the Cauchy form by choosing     &#xA0; G ( t ) = t &#x2212; a
{\displaystyle \ G(t)=t-a}  [\ G(t)=t-a].
Remark. Using this method one can also recover the integral form of the
remainder by choosing
         G ( t ) =  &#x222B;  a   t       f  ( k + 1 )   ( s )   k !    ( x
      &#x2212; s  )  k    d s ,   {\displaystyle G(t)=\int _{a}^{t}{\frac {f^{
      (k+1)}(s)}{k!}}(x-s)^{k}\,ds,}  [G(t)=\int _{a}^{t}{\frac {f^{(k+1)}(s)}
      {k!}}(x-s)^{k}\,ds,]
but the requirements for f needed for the use of mean value theorem are too
strong, if one aims to prove the claim in the case that f(k) is only absolutely
continuous. However, if one uses Riemann_integral instead of Lebesgue_integral,
the assumptions cannot be weakened.
**** Derivation for the integral form of the remainder[edit] ****
Due to absolute_continuity of f(k) on the closed_interval between a and x its
derivative f(k+1) exists as an L1-function, and we can use fundamental_theorem
of_calculus and integration_by_parts. This same proof applies for the Riemann
integral assuming that f(k) is continuous on the closed interval and
differentiable on the open_interval between a and x, and this leads to the same
result than using the mean value theorem.
The fundamental_theorem_of_calculus states that
         f ( x ) = f ( a ) +  &#x222B;  a   x     f &#x2032;  ( t )  d t .
      {\displaystyle f(x)=f(a)+\int _{a}^{x}\,f'(t)\,dt.}  [f(x)=f(a)+\int _
      {a}^{x}\,f'(t)\,dt.]
Now we can integrate_by_parts and use the fundamental theorem of calculus again
to see that
             f ( x )    = f ( a ) +   (   x  f &#x2032;  ( x ) &#x2212; a  f
      &#x2032;  ( a )   )   &#x2212;  &#x222B;  a   x   t  f &#x2033;  ( t )  d
      t       = f ( a ) + x  (   f &#x2032;  ( a ) +  &#x222B;  a   x    f
      &#x2033;  ( t )  d t  )  &#x2212; a  f &#x2032;  ( a ) &#x2212;  &#x222B;
      a   x   t  f &#x2033;  ( t )  d t       = f ( a ) + ( x &#x2212; a )  f
      &#x2032;  ( a ) +  &#x222B;  a   x    ( x &#x2212; t )  f &#x2033;  ( t )
      d t ,       {\displaystyle {\begin{aligned}f(x)&=f(a)+{\Big (}xf'(x)-af'
      (a){\Big )}-\int _{a}^{x}tf''(t)\,dt\\&=f(a)+x\left(f'(a)+\int _{a}^
      {x}f''(t)\,dt\right)-af'(a)-\int _{a}^{x}tf''(t)\,dt\\&=f(a)+(x-a)f'
      (a)+\int _{a}^{x}\,(x-t)f''(t)\,dt,\end{aligned}}}  [{\begin{aligned}f
      (x)&=f(a)+{\Big (}xf'(x)-af'(a){\Big )}-\int _{a}^{x}tf''(t)\,dt\\&=f
      (a)+x\left(f'(a)+\int _{a}^{x}f''(t)\,dt\right)-af'(a)-\int _{a}^{x}tf''
      (t)\,dt\\&=f(a)+(x-a)f'(a)+\int _{a}^{x}\,(x-t)f''(t)\,dt,\end{aligned}}]
which is exactly Taylor's theorem with remainder in the integral form in the
case k=1. The general statement is proved using induction. Suppose that
         ( &#x2217; )  f ( x ) = f ( a ) +     f &#x2032;  ( a )   1 !    ( x
      &#x2212; a ) + &#x22EF; +     f  ( k )   ( a )   k !    ( x &#x2212; a  )
      k   +  &#x222B;  a   x       f  ( k + 1 )   ( t )   k !    ( x &#x2212; t
      )  k    d t .   {\displaystyle (*)\quad f(x)=f(a)+{\frac {f'(a)}{1!}}(x-
      a)+\cdots +{\frac {f^{(k)}(a)}{k!}}(x-a)^{k}+\int _{a}^{x}{\frac {f^{
      (k+1)}(t)}{k!}}(x-t)^{k}\,dt.}  [(*)\quad f(x)=f(a)+{\frac {f'(a)}{1!}}
      (x-a)+\cdots +{\frac {f^{(k)}(a)}{k!}}(x-a)^{k}+\int _{a}^{x}{\frac {f^{
      (k+1)}(t)}{k!}}(x-t)^{k}\,dt.]
Integrating the remainder term by parts we arrive at
              &#x222B;  a   x       f  ( k + 1 )   ( t )   k !    ( x &#x2212;
      t  )  k    d t =    &#x2212;   [      f  ( k + 1 )   ( t )   ( k + 1 ) k
      !    ( x &#x2212; t  )  k + 1    ]   a   x   +  &#x222B;  a   x       f
      ( k + 2 )   ( t )   ( k + 1 ) k !    ( x &#x2212; t  )  k + 1    d t
      =   &#xA0;     f  ( k + 1 )   ( a )   ( k + 1 ) !    ( x &#x2212; a  )  k
      + 1   +  &#x222B;  a   x       f  ( k + 2 )   ( t )   ( k + 1 ) !    ( x
      &#x2212; t  )  k + 1    d t .       {\displaystyle {\begin{aligned}\int _
      {a}^{x}{\frac {f^{(k+1)}(t)}{k!}}(x-t)^{k}\,dt=&-\left[{\frac {f^{(k+1)}
      (t)}{(k+1)k!}}(x-t)^{k+1}\right]_{a}^{x}+\int _{a}^{x}{\frac {f^{(k+2)}
      (t)}{(k+1)k!}}(x-t)^{k+1}\,dt\\=&\ {\frac {f^{(k+1)}(a)}{(k+1)!}}(x-a)^
      {k+1}+\int _{a}^{x}{\frac {f^{(k+2)}(t)}{(k+1)!}}(x-t)^{k+1}\,dt.\end
      {aligned}}}  [{\displaystyle {\begin{aligned}\int _{a}^{x}{\frac {f^{
      (k+1)}(t)}{k!}}(x-t)^{k}\,dt=&-\left[{\frac {f^{(k+1)}(t)}{(k+1)k!}}(x-
      t)^{k+1}\right]_{a}^{x}+\int _{a}^{x}{\frac {f^{(k+2)}(t)}{(k+1)k!}}(x-
      t)^{k+1}\,dt\\=&\ {\frac {f^{(k+1)}(a)}{(k+1)!}}(x-a)^{k+1}+\int _{a}^{x}
      {\frac {f^{(k+2)}(t)}{(k+1)!}}(x-t)^{k+1}\,dt.\end{aligned}}}]
Substituting this into the formula in (*) shows that if it holds for the value
k, it must also hold for the value k + 1. Therefore, since it holds for k = 1,
it must hold for every positive integer k.
**** Derivation for the Cauchy form of the remainder[edit] ****
To the integral form of the remainder, we can apply the mean value theorem for
integral.
              &#x222B;  a   x       f  ( k + 1 )   ( t )   k !    ( x &#x2212;
      t  )  k    d  t    =     f  ( k + 1 )   ( &#x03BE; )   k !    ( x
      &#x2212; &#x03BE;  )  k    &#x222B;  a   x    d  t       =     f  ( k + 1
      )   ( &#x03BE; )   k !    ( x &#x2212; &#x03BE;  )  k   ( x &#x2212; a )
      {\displaystyle {\begin{aligned}\int _{a}^{x}{\frac {f^{(k+1)}(t)}{k!}}(x-
      t)^{k}\mathrm {d} t&={\frac {f^{(k+1)}(\xi )}{k!}}(x-\xi )^{k}\int _{a}^
      {x}\mathrm {d} t\\&={\frac {f^{(k+1)}(\xi )}{k!}}(x-\xi )^{k}(x-a)\end
      {aligned}}}  [{\displaystyle {\begin{aligned}\int _{a}^{x}{\frac {f^{
      (k+1)}(t)}{k!}}(x-t)^{k}\mathrm {d} t&={\frac {f^{(k+1)}(\xi )}{k!}}(x-
      \xi )^{k}\int _{a}^{x}\mathrm {d} t\\&={\frac {f^{(k+1)}(\xi )}{k!}}(x-
      \xi )^{k}(x-a)\end{aligned}}}]
,where     &#x03BE; &#x2208; { a + &#x03B8; ( x &#x2212; a ) &#x003A; 0 <
&#x03B8; < 1 }   {\displaystyle \xi \in \{a+\theta (x-a)\colon 0<\theta <1\}}
[{\displaystyle \xi \in \{a+\theta (x-a)\colon 0<\theta <1\}}]
So, The Cauchy form of the remainder is hold.
**** Derivation for the remainder of multivariate Taylor polynomials[edit] ****
We prove the special case, where f : Rn â R has continuous partial
derivatives up to the order k+1 in some closed ball B with center a. The
strategy of the proof is to apply the one-variable case of Taylor's theorem to
the restriction of f to the line segment adjoining x and a.[15] Parametrize the
line segment between a and x by u(t) = a + t(x â a). We apply the one-
variable version of Taylor's theorem to the function g(t) = f(u(t)):
         f (  x  ) = g ( 1 ) = g ( 0 ) +  &#x2211;  j = 1   k     1  j !     g
      ( j )   ( 0 ) &#xA0; + &#xA0;  &#x222B;  0   1      ( 1 &#x2212; t  )  k
      k !     g  ( k + 1 )   ( t )  d t .   {\displaystyle f(\mathbf {x} )=g
      (1)=g(0)+\sum _{j=1}^{k}{\frac {1}{j!}}g^{(j)}(0)\ +\ \int _{0}^{1}{\frac
      {(1-t)^{k}}{k!}}g^{(k+1)}(t)\,dt.}  [f(\mathbf {x} )=g(1)=g(0)+\sum _
      {j=1}^{k}{\frac {1}{j!}}g^{(j)}(0)\ +\ \int _{0}^{1}{\frac {(1-t)^{k}}
      {k!}}g^{(k+1)}(t)\,dt.]
Applying the chain_rule for several variables gives
              g  ( j )   ( t )    =    d  j    d  t  j      f ( u ( t ) ) =
      d  j    d  t  j      f (  a  + t (  x  &#x2212;  a  ) )       =  &#x2211;
      |  &#x03B1;  |  = j    (     j     &#x03B1;     )  (  D  &#x03B1;   f )
      (  a  + t (  x  &#x2212;  a  ) ) (  x  &#x2212;  a   )  &#x03B1;
      {\displaystyle {\begin{aligned}g^{(j)}(t)&={\frac {d^{j}}{dt^{j}}}f(u
      (t))={\frac {d^{j}}{dt^{j}}}f(\mathbf {a} +t(\mathbf {x} -\mathbf {a}
      ))\\&=\sum _{|\alpha |=j}\left({\begin{matrix}j\\\alpha \end
      {matrix}}\right)(D^{\alpha }f)(\mathbf {a} +t(\mathbf {x} -\mathbf {a} ))
      (\mathbf {x} -\mathbf {a} )^{\alpha }\end{aligned}}}  [{\begin{aligned}g^
      {(j)}(t)&={\frac {d^{j}}{dt^{j}}}f(u(t))={\frac {d^{j}}{dt^{j}}}f(\mathbf
      {a} +t(\mathbf {x} -\mathbf {a} ))\\&=\sum _{|\alpha |=j}\left({\begin
      {matrix}j\\\alpha \end{matrix}}\right)(D^{\alpha }f)(\mathbf {a} +t
      (\mathbf {x} -\mathbf {a} ))(\mathbf {x} -\mathbf {a} )^{\alpha }\end
      {aligned}}]
where      (     j     &#x03B1;     )    {\displaystyle \left({\begin
{matrix}j\\\alpha \end{matrix}}\right)}  [\left({\begin{matrix}j\\\alpha \end
{matrix}}\right)] is the multinomial_coefficient. Since       1  j !
(     j     &#x03B1;     )  =   1  &#x03B1; !      {\displaystyle {\frac {1}
{j!}}\left({\begin{matrix}j\\\alpha \end{matrix}}\right)={\frac {1}{\alpha !}}}
[{\frac {1}{j!}}\left({\begin{matrix}j\\\alpha \end{matrix}}\right)={\frac {1}
{\alpha !}}], we get
         f (  x  ) = f (  a  ) +  &#x2211;  1 &#x2264;  |  &#x03B1;  |
      &#x2264; k     1  &#x03B1; !    (  D  &#x03B1;   f ) (  a  ) (  x
      &#x2212;  a   )  &#x03B1;   +  &#x2211;   |  &#x03B1;  |  = k + 1      k
      + 1   &#x03B1; !    (  x  &#x2212;  a   )  &#x03B1;    &#x222B;  0   1
      ( 1 &#x2212; t  )  k   (  D  &#x03B1;   f ) (  a  + t (  x  &#x2212;  a
      ) )  d t .   {\displaystyle f(\mathbf {x} )=f(\mathbf {a} )+\sum _{1\leq
      |\alpha |\leq k}{\frac {1}{\alpha !}}(D^{\alpha }f)(\mathbf {a} )(\mathbf
      {x} -\mathbf {a} )^{\alpha }+\sum _{|\alpha |=k+1}{\frac {k+1}{\alpha !}}
      (\mathbf {x} -\mathbf {a} )^{\alpha }\int _{0}^{1}(1-t)^{k}(D^{\alpha }f)
      (\mathbf {a} +t(\mathbf {x} -\mathbf {a} ))\,dt.}  [{\displaystyle f
      (\mathbf {x} )=f(\mathbf {a} )+\sum _{1\leq |\alpha |\leq k}{\frac {1}
      {\alpha !}}(D^{\alpha }f)(\mathbf {a} )(\mathbf {x} -\mathbf {a} )^
      {\alpha }+\sum _{|\alpha |=k+1}{\frac {k+1}{\alpha !}}(\mathbf {x} -
      \mathbf {a} )^{\alpha }\int _{0}^{1}(1-t)^{k}(D^{\alpha }f)(\mathbf {a}
      +t(\mathbf {x} -\mathbf {a} ))\,dt.}]
***** See also[edit] *****
    * Laurent_series
    * PadÃ©_approximant
    * Newton_series
***** Footnotes[edit] *****
   1. ^  (2013). "Linear_and_quadratic_approximation" Retrieved December 6,
      2018
   2. ^ Kline_1972, p. 442, 464.
   3. ^Genocchi, Angelo; Peano, Giuseppe (1884), Calcolo differenziale e
      principii di calcolo integrale, (N. 67, pp. XVIIâXIX): Fratelli Bocca
      ed.
   4. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   5. ^Spivak,_Michael (1994), Calculus (3rd ed.), Houston, TX: Publish or
      Perish, p. 383, ISBN 978-0-914098-89-8
   6. ^Hazewinkel,_Michiel, ed. (2001) [1994], "Taylor_formula", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
   7. ^ The hypothesis of f(k) being continuous on the closed_interval between
      a and x is not redundant. Although f being k + 1 times differentiable on
      the open_interval between a and x does imply that f(k) is continuous on
      the open_interval between a and x, it does not imply that f(k) is
      continuous on the closed_interval between a and x, i.e. it does not imply
      that f(k) is continuous at the endpoints of that interval. Consider, for
      example, the function f : [0,1] → R defined to equal     sin &#x2061; ( 1
      /  x )   {\displaystyle \sin(1/x)}  [{\displaystyle \sin(1/x)}] on
      ( 0 , 1 ]   {\displaystyle (0,1]}  [{\displaystyle (0,1]}] and with     f
      ( 0 ) = 0   {\displaystyle f(0)=0}  [f(0)=0]. This is not continuous at
      0, but is continuous on     ( 0 , 1 )   {\displaystyle (0,1)}  [(0,1)].
      Moreover, one can show that this function has an antiderivative.
      Therefore that antiderivative is differentiable on     ( 0 , 1 )
      {\displaystyle (0,1)}  [(0,1)], its derivative (the function f) is
      continuous on the open_interval     ( 0 , 1 )   {\displaystyle (0,1)}  [
      (0,1)], but its derivative f is not continuous on the closed_interval
      [ 0 , 1 ]   {\displaystyle [0,1]}  [[0,1]]. So the theorem would not
      apply in this case.
   8. ^ Kline_1998, Â§20.3; Apostol_1967, Â§7.7.
   9. ^ Apostol_1967, Â§7.7.
  10. ^ Apostol_1967, Â§7.5.
  11. ^ Apostol_1967, Â§7.6
  12. ^ Rudin_1987, Â§10.26
  13. ^ This follows from iterated application of the theorem that if the
      partial derivatives of a function f exist in a neighborhood of a and are
      continuous at a, then the function is differentiable at a. See, for
      instance, Apostol_1974, Theorem 12.11.
  14. ^ KÃ¶nigsberger Analysis 2, p. 64 ff.
  15. ^ Stromberg_1981
  16. ^ HÃ¶rmander_1976, pp. 12–13
***** References[edit] *****
    * Apostol,_Tom (1967), Calculus, Wiley, ISBN 0-471-00005-1
.
Apostol, Tom (1974), Mathematical analysis, AddisonâWesley
.
Bartle, Robert G.; Sherbert, Donald R. (2011), Introduction to Real Analysis
(4th ed.), Wiley, ISBN 978-0-471-43331-6
.
HÃ¶rmander,_L. (1976), Linear Partial Differential Operators, Volume 1,
Springer, ISBN 978-3-540-00662-6
.
Kline,_Morris (1972), Mathematical thought from ancient to modern times, Volume
2, Oxford University Press
.
Kline, Morris (1998), Calculus: An Intuitive and Physical Approach, Dover,
ISBN 0-486-40453-6
.
Pedrick, George (1994), A First Course in Analysis, Springer, ISBN 0-387-94108-
8
.
Stromberg, Karl (1981), Introduction to classical real analysis, Wadsworth,
ISBN 978-0-534-98012-2
.
Rudin, Walter (1987), Real and complex analysis (3rd ed.), McGraw-Hill, ISBN 0-
07-054234-1
.
Tao, Terence (2014), Analysis, Volume I (3rd ed.), Hindustan Book Agency,
ISBN 978-93-80250-64-9
.
***** External links[edit] *****
    * Taylor's_theorem at ProofWiki
    * Taylor_Series_Approximation_to_Cosine at cut-the-knot
    * Trigonometric_Taylor_Expansion interactive demonstrative applet
    * Taylor_Series_Revisited at Holistic_Numerical_Methods_Institute

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Taylor%27s_theorem&oldid=901380037"
Categories:
    * Theorems_in_calculus
    * Theorems_in_real_analysis
    * Approximations
Hidden categories:
    * Articles_containing_proofs
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
    * AzÉrbaycanca
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Boarisch
    * CatalÃ 
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 11 June 2019, at 13:59 (UTC).
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
