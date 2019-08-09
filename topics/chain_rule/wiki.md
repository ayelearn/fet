The following text has been accessed from https://en.wikipedia.org/wiki/Chain_rule at Thu Aug 8 23:14:31 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Chain rule ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the chain rule in calculus. For the chain rule in
probability theory, see Chain_rule_(probability). For other uses, see Chain
rule_(disambiguation).
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
In calculus, the chain rule is a formula for computing the derivative of the
composition of two or more functions. That is, if f and g are functions, then
the chain rule expresses the derivative of their composition f â g â the
function which maps x to     f ( g ( x ) )   {\displaystyle f(g(x))}  [f(g
(x))]â in terms of the derivatives of f and g and the product_of_functions as
follows:
         ( f &#x2218; g  ) &#x2032;  = (  f &#x2032;  &#x2218; g ) &#x22C5;  g
      &#x2032;  .   {\displaystyle (f\circ g)'=(f'\circ g)\cdot g'.}  [(f\circ
      g)'=(f'\circ g)\cdot g'.]
Alternatively, by letting F = f â g (equiv., F(x) = f(g(x)) for all x), one
can also write the chain rule in Lagrange's_notation, as follows:
          F &#x2032;  ( x ) =  f &#x2032;  ( g ( x ) )  g &#x2032;  ( x ) .
      {\displaystyle F'(x)=f'(g(x))g'(x).}  [F'(x)=f'(g(x))g'(x).]
The chain rule may also be rewritten in Leibniz's_notation in the following
way. If a variable z depends on the variable y, which itself depends on the
variable x (i.e., y and z are dependent_variables), then z, via the
intermediate variable of y, depends on x as well. In which case, the chain rule
states that:
            d z   d x    =    d z   d y    &#x22C5;    d y   d x    .
      {\displaystyle {\frac {dz}{dx}}={\frac {dz}{dy}}\cdot {\frac {dy}{dx}}.}
      [{\frac  {dz}{dx}}={\frac  {dz}{dy}}\cdot {\frac  {dy}{dx}}.]
The two versions of the chain rule are related, in the sense that if     z = f
( y )    {\displaystyle z=f(y)\!}  [{\displaystyle z=f(y)\!}] and     y = g ( x
)    {\displaystyle y=g(x)\!}  [{\displaystyle y=g(x)\!}], then
            d z   d x    =    d z   d y    &#x22C5;    d y   d x    =  f
      &#x2032;  ( y )  g &#x2032;  ( x ) =  f &#x2032;  ( g ( x ) )  g &#x2032;
      ( x ) .   {\displaystyle {\frac {dz}{dx}}={\frac {dz}{dy}}\cdot {\frac
      {dy}{dx}}=f'(y)g'(x)=f'(g(x))g'(x).}  [{\displaystyle {\frac {dz}{dx}}=
      {\frac {dz}{dy}}\cdot {\frac {dy}{dx}}=f'(y)g'(x)=f'(g(x))g'(x).}][1]
In integration, the counterpart to the chain rule is the substitution_rule.
⁰
***** Contents *****
    * 1_History
    * 2_One_dimension
          o 2.1_First_example
          o 2.2_Statement
          o 2.3_Further_examples
                # 2.3.1_Absence_of_formulas
                # 2.3.2_Composites_of_more_than_two_functions
                # 2.3.3_Quotient_rule
                # 2.3.4_Derivatives_of_inverse_functions
          o 2.4_Higher_derivatives
          o 2.5_Proofs
                # 2.5.1_First_proof
                # 2.5.2_Second_proof
                # 2.5.3_Third_proof
                # 2.5.4_Proof_via_infinitesimals
    * 3_Multivariable_case
          o 3.1_Case_of_f(g1(x),_..._,_gk(x))
                # 3.1.1_Example:_arithmetic_operations
          o 3.2_General_rule
                # 3.2.1_Example
                # 3.2.2_Higher_derivatives_of_multivariable_functions
    * 4_Further_generalizations
    * 5_See_also
    * 6_References
    * 7_External_links
***** History[edit] *****
The chain rule seems to have first been used by Gottfried_Wilhelm_Leibniz. He
used it to calculate the derivative of       a + b z + c  z  2
{\displaystyle {\sqrt {a+bz+cz^{2}}}}  [\sqrt{a + bz + cz^2}] as the composite
of the square root function and the function     a + b z + c  z  2
{\displaystyle a+bz+cz^{2}\!}  [{\displaystyle a+bz+cz^{2}\!}]. He first
mentioned it in a 1676 memoir (with a sign error in the calculation). The
common notation of chain rule is due to Leibniz.[2] Guillaume_de_l'HÃ´pital
used the chain rule implicitly in his Analyse_des_infiniment_petits. The chain
rule does not appear in any of Leonhard_Euler's analysis books, even though
they were written over a hundred years after Leibniz's discovery.
***** One dimension[edit] *****
**** First example[edit] ****
Suppose that a skydiver jumps from an aircraft. Assume that t seconds after his
jump, his height above sea level in meters is given by g(t) = 4000 â 4.9t2.
One model for the atmospheric_pressure at a height h is f(h) = 101325
eâ0.0001h. These two equations can be differentiated and combined in various
ways to produce the following data:
    * gâ²(t) = â9.8t is the velocity of the skydiver at time t.
    * fâ²(h) = â10.1325eâ0.0001h is the rate of change in atmospheric
      pressure with respect to height at the height h and is proportional to
      the buoyant_force on the skydiver at h meters above sea level. (The true
      buoyant force depends on the volume of the skydiver.)
    * (f â g)(t) is the atmospheric pressure the skydiver experiences t
      seconds after his jump.
    * (f â g)â²(t) is the rate of change in atmospheric pressure with
      respect to time at t seconds after the skydiver's jump, and is
      proportional to the buoyant force on the skydiver at t seconds after his
      jump.
Here, the chain rule gives a method for computing (f â g)â²(t) in terms of
fâ² and gâ². While it is always possible to directly apply the definition of
the derivative to compute the derivative of a composite function, this is
usually very difficult. The utility of the chain rule is that it turns a
complicated derivative into several easy derivatives.
The chain rule states that, under appropriate conditions,
         ( f &#x2218; g  ) &#x2032;  ( t ) =  f &#x2032;  ( g ( t ) ) &#x22C5;
      g &#x2032;  ( t ) .   {\displaystyle (f\circ g)'(t)=f'(g(t))\cdot g'(t).}
      [(f \circ g)'(t) = f'(g(t))\cdot g'(t).]
In this example, this equals
         ( f &#x2218; g  ) &#x2032;  ( t ) =   (     &#x2212;   10.1325  e
      &#x2212; 0.0001 ( 4000 &#x2212; 4.9  t  2   )     )   &#x22C5;
      (     &#x2212;   9.8 t   )   .   {\displaystyle (f\circ g)'(t)={\big (}
      {\mathord {-}}10.1325e^{-0.0001(4000-4.9t^{2})}{\big )}\cdot {\big (}
      {\mathord {-}}9.8t{\big )}.}  [(f \circ g)'(t) = \big(\mathord{-
      }10.1325e^{-0.0001(4000 - 4.9t^2)}\big)\cdot\big(\mathord{-}9.8t\big).]
In the statement of the chain rule, f and g play slightly different roles
because f' is evaluated at     g ( t )    {\displaystyle g(t)\!}  [
{\displaystyle g(t)\!}], whereas g' is evaluated at t. This is necessary to
make the units work out correctly.
For example, suppose that we want to compute the rate of change in atmospheric
pressure ten seconds after the skydiver jumps. This is (f â g)â²(10) and has
units of pascals per second. The factor gâ²(10) in the chain rule is the
velocity of the skydiver ten seconds after his jump, and it is expressed in
meters per second.      f &#x2032;  ( g ( 10 ) )    {\displaystyle f'(g(10))\!}
[{\displaystyle f'(g(10))\!}] is the change in pressure with respect to height
at the height g(10) and is expressed in pascals per meter. The product of
f &#x2032;  ( g ( 10 ) )    {\displaystyle f'(g(10))\!}  [{\displaystyle f'(g
(10))\!}] and      g &#x2032;  ( 10 )    {\displaystyle g'(10)\!}  [
{\displaystyle g'(10)\!}] therefore has the correct units of pascals per
second.
Here, notice that it is not possible to evaluate f anywhere else. For instance,
the 10 in the problem represents ten seconds, while the expression      f
&#x2032;  ( 10 )    {\displaystyle f'(10)\!}  [{\displaystyle f'(10)\!}] would
represent the change in pressure at a height of ten meters, which is not what
we wanted. Similarly, while gâ²(10) = â98 has a unit of meters per second,
the expression fâ²(gâ²(10)) would represent the change in pressure at a
height of â98 meters, which is again not what we wanted. However, g(10) is
3020 meters above sea level, the height of the skydiver ten seconds after his
jump, and this has the correct units for an input to f.
**** Statement[edit] ****
The simplest form of the chain rule is for real-valued functions of one real
variable. It states that if g is a function that is differentiable at a point c
(i.e. the derivative gâ²(c) exists) and f is a function that is differentiable
at g(c), then the composite function f â g is differentiable at c, and the
derivative is[3]
         ( f &#x2218; g  ) &#x2032;  ( c ) =  f &#x2032;  ( g ( c ) ) &#x22C5;
      g &#x2032;  ( c ) .   {\displaystyle (f\circ g)'(c)=f'(g(c))\cdot g'(c).}
      [ (f\circ g)'(c) = f'(g(c))\cdot g'(c). ]
The rule is sometimes abbreviated as
         ( f &#x2218; g  ) &#x2032;  = (  f &#x2032;  &#x2218; g ) &#x22C5;  g
      &#x2032;  .   {\displaystyle (f\circ g)'=(f'\circ g)\cdot g'.}  [
      {\displaystyle (f\circ g)'=(f'\circ g)\cdot g'.}]
If y = f(u) and u = g(x), then this abbreviated form is written in Leibniz
notation as:
            d y   d x    =    d y   d u    &#x22C5;    d u   d x    .
      {\displaystyle {\frac {dy}{dx}}={\frac {dy}{du}}\cdot {\frac {du}{dx}}.}
      [{\frac {dy}{dx}}={\frac {dy}{du}}\cdot {\frac {du}{dx}}.][1]
The points where the derivatives are evaluated may also be stated explicitly:
               d y   d x    |   x = c   =       d y   d u    |   u = g ( c )
      &#x22C5;       d u   d x    |   x = c   .   {\displaystyle \left.{\frac
      {dy}{dx}}\right|_{x=c}=\left.{\frac {dy}{du}}\right|_{u=g(c)}\cdot \left.
      {\frac {du}{dx}}\right|_{x=c}.}  [{\displaystyle \left.{\frac {dy}
      {dx}}\right|_{x=c}=\left.{\frac {dy}{du}}\right|_{u=g(c)}\cdot \left.
      {\frac {du}{dx}}\right|_{x=c}.}]
Carrying the same reasoning further, given n functions      f  1   , &#x2026; ,
f  n      {\displaystyle f_{1},\ldots ,f_{n}\!}  [{\displaystyle f_{1},\ldots
,f_{n}\!}] with the composite function      f  1   &#x2218; (  f  2   &#x2218;
&#x22EF; (  f  n &#x2212; 1   &#x2218;  f  n   ) )    {\displaystyle f_{1}\circ
(f_{2}\circ \cdots (f_{n-1}\circ f_{n}))\!}  [{\displaystyle f_{1}\circ (f_
{2}\circ \cdots (f_{n-1}\circ f_{n}))\!}], if each function      f  i
{\displaystyle f_{i}\!}  [{\displaystyle f_{i}\!}] is differentiable at its
immediate input, then the composite function is also differentiable by the
repeated application of Chain Rule, where the derivative is (in Leibniz's
notation):
            d  f  1     d x    =    d  f  1     d  f  2         d  f  2     d
      f  3      &#x22EF;    d  f  n     d x    .   {\displaystyle {\frac {df_
      {1}}{dx}}={\frac {df_{1}}{df_{2}}}{\frac {df_{2}}{df_{3}}}\cdots {\frac
      {df_{n}}{dx}}.}  [{\displaystyle {\frac {df_{1}}{dx}}={\frac {df_{1}}{df_
      {2}}}{\frac {df_{2}}{df_{3}}}\cdots {\frac {df_{n}}{dx}}.}][4]
**** Further examples[edit] ****
*** Absence of formulas[edit] ***
It may be possible to apply the chain rule even when there are no formulas for
the functions which are being differentiated. This can happen when the
derivatives are measured directly. Suppose that a car is driving up a tall
mountain. The car's speedometer measures its speed directly. If the grade is
known, then the rate of ascent can be calculated using trigonometry. Suppose
that the car is ascending at 2.5 km/h. Standard models for the Earth's
atmosphere imply that the temperature drops about 6.5 Â°C per kilometer
ascended (called the lapse_rate). To find the temperature drop per hour, we
apply the chain rule. Let the function g(t) be the altitude of the car at time
t, and let the function f(h) be the temperature h kilometers above sea level. f
and g are not known exactly: For example, the altitude where the car starts is
not known and the temperature on the mountain is not known. However, their
derivatives are known: fâ² is â6.5 Â°C/km, and gâ² is 2.5 km/h. The chain
rule states that the derivative of the composite function is the product of the
derivative of f and the derivative of g. This is â6.5 Â°C/km â 2.5 km/h =
â16.25 Â°C/h.
One of the reasons why this computation is possible is because fâ² is a
constant function. This is because the above model is very simple. A more
accurate description of how the temperature near the car varies over time would
require an accurate model of how the temperature varies at different altitudes.
This model may not have a constant derivative. To compute the temperature
change in such a model, it would be necessary to know g and not just gâ²,
because without knowing g it is not possible to know where to evaluate fâ².
*** Composites of more than two functions[edit] ***
The chain rule can be applied to composites of more than two functions. To take
the derivative of a composite of more than two functions, notice that the
composite of f, g, and h (in that order) is the composite of f with g â h.
The chain rule states that to compute the derivative of f â g â h, it is
sufficient to compute the derivative of f and the derivative of g â h. The
derivative of f can be calculated directly, and the derivative of g â h can
be calculated by applying the chain rule again.
For concreteness, consider the function
         y =  e  sin &#x2061; (  x  2   )   .   {\displaystyle y=e^{\sin(x^
      {2})}.}  [{\displaystyle y=e^{\sin(x^{2})}.}]
This can be decomposed as the composite of three functions:
             y    = f ( u ) =  e  u   ,     u    = g ( v ) = sin &#x2061; v =
      sin &#x2061; (  x  2   ) ,     v    = h ( x ) =  x  2   .
      {\displaystyle {\begin{aligned}y&=f(u)=e^{u},\\[6pt]u&=g(v)=\sin v=\sin
      (x^{2}),\\[6pt]v&=h(x)=x^{2}.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}y&=f(u)=e^{u},\\[6pt]u&=g(v)=\sin v=\sin(x^{2}),\\[6pt]v&=h
      (x)=x^{2}.\end{aligned}}}]
Their derivatives are:
                d y   d u       =  f &#x2032;  ( u ) =  e  u   =  e  sin
      &#x2061; (  x  2   )   ,        d u   d v       =  g &#x2032;  ( v ) =
      cos &#x2061; v = cos &#x2061; (  x  2   ) ,        d v   d x       =  h
      &#x2032;  ( x ) = 2 x .       {\displaystyle {\begin{aligned}{\frac {dy}
      {du}}&=f'(u)=e^{u}=e^{\sin(x^{2})},\\[6pt]{\frac {du}{dv}}&=g'(v)=\cos
      v=\cos(x^{2}),\\[6pt]{\frac {dv}{dx}}&=h'(x)=2x.\end{aligned}}}  [
      {\displaystyle {\begin{aligned}{\frac {dy}{du}}&=f'(u)=e^{u}=e^{\sin(x^
      {2})},\\[6pt]{\frac {du}{dv}}&=g'(v)=\cos v=\cos(x^{2}),\\[6pt]{\frac
      {dv}{dx}}&=h'(x)=2x.\end{aligned}}}]
The chain rule states that the derivative of their composite at the point x = a
is:
             ( f &#x2218; g &#x2218; h  ) &#x2032;  ( a )    =  f &#x2032;  (
      ( g &#x2218; h ) ( a ) ) &#x22C5; ( g &#x2218; h  ) &#x2032;  ( a )
      =  f &#x2032;  ( ( g &#x2218; h ) ( a ) ) &#x22C5;  g &#x2032;  ( h ( a )
      ) &#x22C5;  h &#x2032;  ( a ) = (  f &#x2032;  &#x2218; g &#x2218; h )
      ( a ) &#x22C5; (  g &#x2032;  &#x2218; h ) ( a ) &#x22C5;  h &#x2032;
      ( a ) .       {\displaystyle {\begin{aligned}(f\circ g\circ h)'(a)&=f'(
      (g\circ h)(a))\cdot (g\circ h)'(a)\\[10pt]&=f'((g\circ h)(a))\cdot g'(h
      (a))\cdot h'(a)=(f'\circ g\circ h)(a)\cdot (g'\circ h)(a)\cdot h'(a).\end
      {aligned}}}  [{\displaystyle {\begin{aligned}(f\circ g\circ h)'(a)&=f'(
      (g\circ h)(a))\cdot (g\circ h)'(a)\\[10pt]&=f'((g\circ h)(a))\cdot g'(h
      (a))\cdot h'(a)=(f'\circ g\circ h)(a)\cdot (g'\circ h)(a)\cdot h'(a).\end
      {aligned}}}]
In Leibniz notation, this is:
            d y   d x    =       d y   d u    |   u = g ( h ( a ) )   &#x22C5;
      d u   d v    |   v = h ( a )   &#x22C5;       d v   d x    |   x = a   ,
      {\displaystyle {\frac {dy}{dx}}=\left.{\frac {dy}{du}}\right|_{u=g(h
      (a))}\cdot \left.{\frac {du}{dv}}\right|_{v=h(a)}\cdot \left.{\frac {dv}
      {dx}}\right|_{x=a},}  [\frac{dy}{dx} = \left.\frac{dy}{du}\right|_{u=g(h
      (a))}\cdot\left.\frac{du}{dv}\right|_{v=h(a)}\cdot\left.\frac{dv}
      {dx}\right|_{x=a},]
or for short,
            d y   d x    =    d y   d u    &#x22C5;    d u   d v    &#x22C5;
      d v   d x    .   {\displaystyle {\frac {dy}{dx}}={\frac {dy}{du}}\cdot
      {\frac {du}{dv}}\cdot {\frac {dv}{dx}}.}  [\frac{dy}{dx} = \frac{dy}
      {du}\cdot\frac{du}{dv}\cdot\frac{dv}{dx}.]
The derivative function is therefore:
            d y   d x    =  e  sin &#x2061; (  x  2   )   &#x22C5; cos &#x2061;
      (  x  2   ) &#x22C5; 2 x .   {\displaystyle {\frac {dy}{dx}}=e^{\sin(x^
      {2})}\cdot \cos(x^{2})\cdot 2x.}  [{\displaystyle {\frac {dy}{dx}}=e^
      {\sin(x^{2})}\cdot \cos(x^{2})\cdot 2x.}]
Another way of computing this derivative is to view the composite function f
â g â h as the composite of f â g and h. Applying the chain rule in this
manner would yield:
         ( f &#x2218; g &#x2218; h  ) &#x2032;  ( a ) = ( f &#x2218; g  )
      &#x2032;  ( h ( a ) ) &#x22C5;  h &#x2032;  ( a ) =  f &#x2032;  ( g ( h
      ( a ) ) ) &#x22C5;  g &#x2032;  ( h ( a ) ) &#x22C5;  h &#x2032;  ( a ) .
      {\displaystyle (f\circ g\circ h)'(a)=(f\circ g)'(h(a))\cdot h'(a)=f'(g(h
      (a)))\cdot g'(h(a))\cdot h'(a).}  [(f \circ g \circ h)'(a) = (f \circ g)'
      (h(a))\cdot h'(a) = f'(g(h(a)))\cdot g'(h(a))\cdot h'(a).]
This is the same as what was computed above. This should be expected because (f
â g) â h = f â (g â h).
Sometimes, it is necessary to differentiate an arbitrarily long composition of
the form      f  1   &#x2218;  f  2   &#x2218; &#x22EF; &#x2218;  f  n &#x2212;
1   &#x2218;  f  n      {\displaystyle f_{1}\circ f_{2}\circ \cdots \circ f_{n-
1}\circ f_{n}\!}  [{\displaystyle f_{1}\circ f_{2}\circ \cdots \circ f_{n-
1}\circ f_{n}\!}]. In this case, define
          f  a  .  .  b   =  f  a   &#x2218;  f  a + 1   &#x2218; &#x22EF;
      &#x2218;  f  b &#x2212; 1   &#x2218;  f  b     {\displaystyle f_
      {a\,.\,.\,b}=f_{a}\circ f_{a+1}\circ \cdots \circ f_{b-1}\circ f_{b}}  [
      {\displaystyle f_{a\,.\,.\,b}=f_{a}\circ f_{a+1}\circ \cdots \circ f_{b-
      1}\circ f_{b}}]
where      f  a  .  .  a   =  f  a     {\displaystyle f_{a\,.\,.\,a}=f_{a}}  [
{\displaystyle f_{a\,.\,.\,a}=f_{a}}] and      f  a  .  .  b   ( x ) = x
{\displaystyle f_{a\,.\,.\,b}(x)=x}  [{\displaystyle f_{a\,.\,.\,b}(x)=x}] when
b < a   {\displaystyle b<a}  [b < a]. Then the chain rule takes the form
         D  f  1  .  .  n   = ( D  f  1   &#x2218;  f  2  .  .  n   ) ( D  f  2
      &#x2218;  f  3  .  .  n   ) &#x22EF; ( D  f  n &#x2212; 1   &#x2218;  f
      n  .  .  n   ) D  f  n   =  &#x220F;  k = 1   n    [  D  f  k   &#x2218;
      f  ( k + 1 )  .  .  n    ]    {\displaystyle Df_{1\,.\,.\,n}=(Df_{1}\circ
      f_{2\,.\,.\,n})(Df_{2}\circ f_{3\,.\,.\,n})\cdots (Df_{n-1}\circ f_
      {n\,.\,.\,n})Df_{n}=\prod _{k=1}^{n}\left[Df_{k}\circ f_{
      (k+1)\,.\,.\,n}\right]}  [{\displaystyle Df_{1\,.\,.\,n}=(Df_{1}\circ f_
      {2\,.\,.\,n})(Df_{2}\circ f_{3\,.\,.\,n})\cdots (Df_{n-1}\circ f_
      {n\,.\,.\,n})Df_{n}=\prod _{k=1}^{n}\left[Df_{k}\circ f_{
      (k+1)\,.\,.\,n}\right]}]
or, in the Lagrange notation,
          f  1  .  .  n  &#x2032;  ( x ) =  f  1  &#x2032;   (   f  2  .  .  n
      ( x )  )    f  2  &#x2032;   (   f  3  .  .  n   ( x )  )  &#x22EF;  f  n
      &#x2212; 1  &#x2032;   (   f  n  .  .  n   ( x )  )    f  n  &#x2032;
      ( x ) =  &#x220F;  k = 1   n    f  k  &#x2032;   (   f  ( k + 1  .  .  n
      )   ( x )  )    {\displaystyle f_{1\,.\,.\,n}'(x)=f_{1}'\left(f_
      {2\,.\,.\,n}(x)\right)\;f_{2}'\left(f_{3\,.\,.\,n}(x)\right)\cdots f_{n-
      1}'\left(f_{n\,.\,.\,n}(x)\right)\;f_{n}'(x)=\prod _{k=1}^{n}f_{k}'\left
      (f_{(k+1\,.\,.\,n)}(x)\right)}  [{\displaystyle f_{1\,.\,.\,n}'(x)=f_
      {1}'\left(f_{2\,.\,.\,n}(x)\right)\;f_{2}'\left(f_{3\,.\,.\,n}
      (x)\right)\cdots f_{n-1}'\left(f_{n\,.\,.\,n}(x)\right)\;f_{n}'(x)=\prod
      _{k=1}^{n}f_{k}'\left(f_{(k+1\,.\,.\,n)}(x)\right)}]
*** Quotient rule[edit] ***
See also: Quotient_rule
The chain rule can be used to derive some well-known differentiation rules. For
example, the quotient rule is a consequence of the chain rule and the product
rule. To see this, write the function f(x)/g(x) as the product f(x) Â· 1/g(x).
First apply the product rule:
               d  d x     (    f ( x )   g ( x )    )     =   d  d x     (  f
      ( x ) &#x22C5;   1  g ( x )     )        =  f &#x2032;  ( x ) &#x22C5;
      1  g ( x )    + f ( x ) &#x22C5;   d  d x     (   1  g ( x )    )  .
      {\displaystyle {\begin{aligned}{\frac {d}{dx}}\left({\frac {f(x)}{g
      (x)}}\right)&={\frac {d}{dx}}\left(f(x)\cdot {\frac {1}{g
      (x)}}\right)\\&=f'(x)\cdot {\frac {1}{g(x)}}+f(x)\cdot {\frac {d}
      {dx}}\left({\frac {1}{g(x)}}\right).\end{aligned}}}  [\begin{align}
      \frac{d}{dx}\left(\frac{f(x)}{g(x)}\right)
      &= \frac{d}{dx}\left(f(x)\cdot\frac{1}{g(x)}\right) \\
      &= f'(x)\cdot\frac{1}{g(x)} + f(x)\cdot\frac{d}{dx}\left(\frac{1}{g
      (x)}\right).
      \end{align}]
To compute the derivative of 1/g(x), notice that it is the composite of g with
the reciprocal function, that is, the function that sends x to 1/x. The
derivative of the reciprocal function is     &#x2212; 1  /   x  2
{\displaystyle -1/x^{2}\!}  [{\displaystyle -1/x^{2}\!}]. By applying the chain
rule, the last expression becomes:
          f &#x2032;  ( x ) &#x22C5;   1  g ( x )    + f ( x ) &#x22C5;
      (  &#x2212;   1  g ( x  )  2      &#x22C5;  g &#x2032;  ( x )  )  =     f
      &#x2032;  ( x ) g ( x ) &#x2212; f ( x )  g &#x2032;  ( x )   g ( x  )  2
      ,   {\displaystyle f'(x)\cdot {\frac {1}{g(x)}}+f(x)\cdot \left(-{\frac
      {1}{g(x)^{2}}}\cdot g'(x)\right)={\frac {f'(x)g(x)-f(x)g'(x)}{g(x)^
      {2}}},}  [f'(x)\cdot\frac{1}{g(x)} + f(x)\cdot\left(-\frac{1}{g
      (x)^2}\cdot g'(x)\right)
      = \frac{f'(x) g(x) - f(x) g'(x)}{g(x)^2},]
which is the usual formula for the quotient rule.
*** Derivatives of inverse functions[edit] ***
Main article: Inverse_functions_and_differentiation
Suppose that y = g(x) has an inverse_function. Call its inverse function f so
that we have x = f(y). There is a formula for the derivative of f in terms of
the derivative of g. To see this, note that f and g satisfy the formula
         f ( g ( x ) ) = x .   {\displaystyle f(g(x))=x.}  [f(g(x)) = x.]
And because the functions     f ( g ( x ) )    {\displaystyle f(g(x))\!}  [
{\displaystyle f(g(x))\!}] and x are equal, their derivatives must be equal.
The derivative of x is the constant function with value 1, and the derivative
of     f ( g ( x ) )    {\displaystyle f(g(x))\!}  [{\displaystyle f(g(x))\!}]
is determined by the chain rule. Therefore, we have that:
          f &#x2032;  ( g ( x ) )  g &#x2032;  ( x ) = 1.   {\displaystyle f'(g
      (x))g'(x)=1.}  [f'(g(x)) g'(x) = 1.]
To express f' as a function of an independent variable y, we substitute     f
( y )    {\displaystyle f(y)\!}  [{\displaystyle f(y)\!}] for x wherever it
appears. Then we can solve for f'.
              f &#x2032;  ( g ( f ( y ) ) )  g &#x2032;  ( f ( y ) )    = 1
      f &#x2032;  ( y )  g &#x2032;  ( f ( y ) )    = 1      f &#x2032;  ( y )
      =   1   g &#x2032;  ( f ( y ) )    .       {\displaystyle {\begin
      {aligned}f'(g(f(y)))g'(f(y))&=1\\[5pt]f'(y)g'(f(y))&=1\\[5pt]f'(y)={\frac
      {1}{g'(f(y))}}.\end{aligned}}}  [{\displaystyle {\begin{aligned}f'(g(f
      (y)))g'(f(y))&=1\\[5pt]f'(y)g'(f(y))&=1\\[5pt]f'(y)={\frac {1}{g'(f
      (y))}}.\end{aligned}}}]
For example, consider the function g(x) = ex. It has an inverse f(y) = ln y.
Because gâ²(x) = ex, the above formula says that
           d  d y    ln &#x2061; y =   1  e  ln &#x2061; y     =   1 y   .
      {\displaystyle {\frac {d}{dy}}\ln y={\frac {1}{e^{\ln y}}}={\frac {1}
      {y}}.}  [\frac{d}{dy}\ln y = \frac{1}{e^{\ln y}} = \frac{1}{y}.]
This formula is true whenever g is differentiable and its inverse f is also
differentiable. This formula can fail when one of these conditions is not true.
For example, consider g(x) = x3. Its inverse is f(y) = y1/3, which is not
differentiable at zero. If we attempt to use the above formula to compute the
derivative of f at zero, then we must evaluate 1/gâ²(f(0)). Since f(0) = 0 and
gâ²(0) = 0, we must evaluate 1/0, which is undefined. Therefore, the formula
fails in this case. This is not surprising because f is not differentiable at
zero.
**** Higher derivatives[edit] ****
FaÃ _di_Bruno's_formula generalizes the chain rule to higher derivatives.
Assuming that y = f(u) and u = g(x), then the first few derivatives are:
                d y   d x       =    d y   d u       d u   d x            d  2
      y   d  x  2         =     d  2   y   d  u  2        (    d u   d x    )
      2   +    d y   d u        d  2   u   d  x  2              d  3   y   d  x
      3         =     d  3   y   d  u  3        (    d u   d x    )   3   + 3
      d  2   y   d  u  2         d u   d x        d  2   u   d  x  2      +
      d y   d u        d  3   u   d  x  3              d  4   y   d  x  4
      =     d  4   y   d  u  4        (    d u   d x    )   4   + 6      d  3
      y   d  u  3        (    d u   d x    )   2       d  2   u   d  x  2
      +     d  2   y   d  u  2       (  4     d u   d x        d  3   u   d  x
      3      + 3    (     d  2   u   d  x  2      )   2    )  +    d y   d u
      d  4   u   d  x  4      .       {\displaystyle {\begin{aligned}{\frac
      {dy}{dx}}&={\frac {dy}{du}}{\frac {du}{dx}}\\[4pt]{\frac {d^{2}y}{dx^
      {2}}}&={\frac {d^{2}y}{du^{2}}}\left({\frac {du}{dx}}\right)^{2}+{\frac
      {dy}{du}}{\frac {d^{2}u}{dx^{2}}}\\[4pt]{\frac {d^{3}y}{dx^{3}}}&={\frac
      {d^{3}y}{du^{3}}}\left({\frac {du}{dx}}\right)^{3}+3\,{\frac {d^{2}y}{du^
      {2}}}{\frac {du}{dx}}{\frac {d^{2}u}{dx^{2}}}+{\frac {dy}{du}}{\frac {d^
      {3}u}{dx^{3}}}\\[4pt]{\frac {d^{4}y}{dx^{4}}}&={\frac {d^{4}y}{du^
      {4}}}\left({\frac {du}{dx}}\right)^{4}+6\,{\frac {d^{3}y}{du^{3}}}\left(
      {\frac {du}{dx}}\right)^{2}{\frac {d^{2}u}{dx^{2}}}+{\frac {d^{2}y}{du^
      {2}}}\left(4\,{\frac {du}{dx}}{\frac {d^{3}u}{dx^{3}}}+3\,\left({\frac
      {d^{2}u}{dx^{2}}}\right)^{2}\right)+{\frac {dy}{du}}{\frac {d^{4}u}{dx^
      {4}}}.\end{aligned}}}  [{\displaystyle {\begin{aligned}{\frac {dy}{dx}}&=
      {\frac {dy}{du}}{\frac {du}{dx}}\\[4pt]{\frac {d^{2}y}{dx^{2}}}&={\frac
      {d^{2}y}{du^{2}}}\left({\frac {du}{dx}}\right)^{2}+{\frac {dy}{du}}{\frac
      {d^{2}u}{dx^{2}}}\\[4pt]{\frac {d^{3}y}{dx^{3}}}&={\frac {d^{3}y}{du^
      {3}}}\left({\frac {du}{dx}}\right)^{3}+3\,{\frac {d^{2}y}{du^{2}}}{\frac
      {du}{dx}}{\frac {d^{2}u}{dx^{2}}}+{\frac {dy}{du}}{\frac {d^{3}u}{dx^
      {3}}}\\[4pt]{\frac {d^{4}y}{dx^{4}}}&={\frac {d^{4}y}{du^{4}}}\left(
      {\frac {du}{dx}}\right)^{4}+6\,{\frac {d^{3}y}{du^{3}}}\left({\frac {du}
      {dx}}\right)^{2}{\frac {d^{2}u}{dx^{2}}}+{\frac {d^{2}y}{du^{2}}}\left
      (4\,{\frac {du}{dx}}{\frac {d^{3}u}{dx^{3}}}+3\,\left({\frac {d^{2}u}{dx^
      {2}}}\right)^{2}\right)+{\frac {dy}{du}}{\frac {d^{4}u}{dx^{4}}}.\end
      {aligned}}}]
**** Proofs[edit] ****
*** First proof[edit] ***
One proof of the chain rule begins with the definition of the derivative:
         ( f &#x2218; g  ) &#x2032;  ( a ) =  lim  x &#x2192; a      f ( g ( x
      ) ) &#x2212; f ( g ( a ) )   x &#x2212; a    .   {\displaystyle (f\circ
      g)'(a)=\lim _{x\to a}{\frac {f(g(x))-f(g(a))}{x-a}}.}  [(f \circ g)'(a) =
      \lim_{x \to a} \frac{f(g(x)) - f(g(a))}{x - a}.]
Assume for the moment that     g ( x )    {\displaystyle g(x)\!}  [
{\displaystyle g(x)\!}] does not equal     g ( a )    {\displaystyle g(a)\!}  [
{\displaystyle g(a)\!}] for any x near a. Then the previous expression is equal
to the product of two factors:
          lim  x &#x2192; a      f ( g ( x ) ) &#x2212; f ( g ( a ) )   g ( x )
      &#x2212; g ( a )    &#x22C5;    g ( x ) &#x2212; g ( a )   x &#x2212; a
      .   {\displaystyle \lim _{x\to a}{\frac {f(g(x))-f(g(a))}{g(x)-g
      (a)}}\cdot {\frac {g(x)-g(a)}{x-a}}.}  [\lim_{x \to a} \frac{f(g(x)) - f
      (g(a))}{g(x) - g(a)} \cdot \frac{g(x) - g(a)}{x - a}.]
If     g    {\displaystyle g\!}  [{\displaystyle g\!}] oscillates near a, then
it might happen that no matter how close one gets to a, there is always an even
closer x such that     g ( x )    {\displaystyle g(x)\!}  [{\displaystyle g
(x)\!}] equals     g ( a )    {\displaystyle g(a)\!}  [{\displaystyle g(a)\!}].
For example, this happens for g(x) = x2sin(1 / x) near the point a = 0.
Whenever this happens, the above expression is undefined because it involves
division_by_zero. To work around this, introduce a function    Q
{\displaystyle Q\!}  [Q\!] as follows:
         Q ( y ) =   {       f ( y ) &#x2212; f ( g ( a ) )   y &#x2212; g ( a
      )    ,   y &#x2260; g ( a ) ,      f &#x2032;  ( g ( a ) ) ,   y = g ( a
      ) .         {\displaystyle Q(y)={\begin{cases}{\frac {f(y)-f(g(a))}{y-g
      (a)}},&y\neq g(a),\\f'(g(a)),&y=g(a).\end{cases}}}  [Q(y) = \begin{cases}
      \frac{f(y) - f(g(a))}{y - g(a)}, & y \neq g(a), \\
      f'(g(a)), & y = g(a).
      \end{cases}]
We will show that the difference_quotient for f â g is always equal to:
         Q ( g ( x ) ) &#x22C5;    g ( x ) &#x2212; g ( a )   x &#x2212; a    .
      {\displaystyle Q(g(x))\cdot {\frac {g(x)-g(a)}{x-a}}.}  [Q(g(x)) \cdot
      \frac{g(x) - g(a)}{x - a}.]
Whenever g(x) is not equal to g(a), this is clear because the factors of g(x)
â g(a) cancel. When g(x) equals g(a), then the difference quotient for f â
g is zero because f(g(x)) equals f(g(a)), and the above product is zero because
it equals fâ²(g(a)) times zero. So the above product is always equal to the
difference quotient, and to show that the derivative of f â g at a exists and
to determine its value, we need only show that the limit as x goes to a of the
above product exists and determine its value.
To do this, recall that the limit of a product exists if the limits of its
factors exist. When this happens, the limit of the product of these two factors
will equal the product of the limits of the factors. The two factors are Q(g
(x)) and (g(x) â g(a)) / (x â a). The latter is the difference quotient for
g at a, and because g is differentiable at a by assumption, its limit as x
tends to a exists and equals gâ²(a).
As for Q(g(x)), notice that Q is defined wherever f is. Furthermore, f is
differentiable at f(a) by assumption, so Q is continuous at g(a), by definition
of the derivative. The function g is continuous at a because it is
differentiable at a, and therefore Q â g is continuous at a. So its limit as
x goes to a exists and equals Q(g(a)), which is fâ²(g(a)).
This shows that the limits of both factors exist and that they equal fâ²(g(a))
and gâ²(a), respectively. Therefore, the derivative of f â g at a exists and
equals fâ²(g(a))gâ²(a).[4]
*** Second proof[edit] ***
Another way of proving the chain rule is to measure the error in the linear
approximation determined by the derivative. This proof has the advantage that
it generalizes to several variables. It relies on the following equivalent
definition of differentiability at a point: A function g is differentiable at a
if there exists a real number gâ²(a) and a function Îµ(h) that tends to zero
as h tends to zero, and furthermore
         g ( a + h ) &#x2212; g ( a ) =  g &#x2032;  ( a ) h + &#x03B5; ( h ) h
      .   {\displaystyle g(a+h)-g(a)=g'(a)h+\varepsilon (h)h.}  [{\displaystyle
      g(a+h)-g(a)=g'(a)h+\varepsilon (h)h.}]
Here the left-hand side represents the true difference between the value of g
at a and at a + h, whereas the right-hand side represents the approximation
determined by the derivative plus an error term.
In the situation of the chain rule, such a function Îµ exists because g is
assumed to be differentiable at a. Again by assumption, a similar function also
exists for f at g(a). Calling this function Î·, we have
         f ( g ( a ) + k ) &#x2212; f ( g ( a ) ) =  f &#x2032;  ( g ( a ) ) k
      + &#x03B7; ( k ) k .   {\displaystyle f(g(a)+k)-f(g(a))=f'(g(a))k+\eta
      (k)k.}  [{\displaystyle f(g(a)+k)-f(g(a))=f'(g(a))k+\eta (k)k.}]
The above definition imposes no constraints on Î·(0), even though it is assumed
that Î·(k) tends to zero as k tends to zero. If we set Î·(0) = 0, then Î· is
continuous at 0.
Proving the theorem requires studying the difference f(g(a + h)) â f(g(a)) as
h tends to zero. The first step is to substitute for g(a + h) using the
definition of differentiability of g at a:
         f ( g ( a + h ) ) &#x2212; f ( g ( a ) ) = f ( g ( a ) +  g &#x2032;
      ( a ) h + &#x03B5; ( h ) h ) &#x2212; f ( g ( a ) ) .   {\displaystyle f
      (g(a+h))-f(g(a))=f(g(a)+g'(a)h+\varepsilon (h)h)-f(g(a)).}  [f(g(a + h))
      - f(g(a)) = f(g(a) + g'(a) h + \varepsilon(h) h) - f(g(a)).]
The next step is to use the definition of differentiability of f at g(a). This
requires a term of the form f(g(a) + k) for some k. In the above equation, the
correct k varies with h. Set kh = gâ²(a) h + Îµ(h) h and the right hand side
becomes f(g(a) + kh) â f(g(a)). Applying the definition of the derivative
gives:
         f ( g ( a ) +  k  h   ) &#x2212; f ( g ( a ) ) =  f &#x2032;  ( g ( a
      ) )  k  h   + &#x03B7; (  k  h   )  k  h   .   {\displaystyle f(g(a)+k_
      {h})-f(g(a))=f'(g(a))k_{h}+\eta (k_{h})k_{h}.}  [{\displaystyle f(g(a)+k_
      {h})-f(g(a))=f'(g(a))k_{h}+\eta (k_{h})k_{h}.}]
To study the behavior of this expression as h tends to zero, expand kh. After
regrouping the terms, the right-hand side becomes:
          f &#x2032;  ( g ( a ) )  g &#x2032;  ( a ) h + [  f &#x2032;  ( g ( a
      ) ) &#x03B5; ( h ) + &#x03B7; (  k  h   )  g &#x2032;  ( a ) + &#x03B7;
      (  k  h   ) &#x03B5; ( h ) ] h .   {\displaystyle f'(g(a))g'(a)h+[f'(g
      (a))\varepsilon (h)+\eta (k_{h})g'(a)+\eta (k_{h})\varepsilon (h)]h.}  [
      {\displaystyle f'(g(a))g'(a)h+[f'(g(a))\varepsilon (h)+\eta (k_{h})g'
      (a)+\eta (k_{h})\varepsilon (h)]h.}]
Because Îµ(h) and Î·(kh) tend to zero as h tends to zero, the first two
bracketed terms tend to zero as h tends to zero. Applying the same theorem on
products of limits as in the first proof, the third bracketed term also tends
zero. Because the above expression is equal to the difference f(g(a + h)) â f
(g(a)), by the definition of the derivative f â g is differentiable at a and
its derivative is fâ²(g(a)) gâ²(a).
The role of Q in the first proof is played by Î· in this proof. They are
related by the equation:
         Q ( y ) =  f &#x2032;  ( g ( a ) ) + &#x03B7; ( y &#x2212; g ( a ) ) .
      {\displaystyle Q(y)=f'(g(a))+\eta (y-g(a)).}  [{\displaystyle Q(y)=f'(g
      (a))+\eta (y-g(a)).}]
The need to define Q at g(a) is analogous to the need to define Î· at zero.
*** Third proof[edit] ***
Constantin_CarathÃ©odory's alternative definition of the differentiability of a
function can be used to give an elegant proof of the chain rule.[5]
Under this definition, a function f is differentiable at a point a if and only
if there is a function q, continuous at a and such that f(x) â f(a) = q(x)(x
â a). There is at most one such function, and if f is differentiable at a
then f â²(a) = q(a).
Given the assumptions of the chain rule and the fact that differentiable
functions and compositions of continuous functions are continuous, we have that
there exist functions q, continuous at g(a) and r, continuous at a and such
that,
         f ( g ( x ) ) &#x2212; f ( g ( a ) ) = q ( g ( x ) ) ( g ( x )
      &#x2212; g ( a ) )   {\displaystyle f(g(x))-f(g(a))=q(g(x))(g(x)-g(a))}
      [{\displaystyle f(g(x))-f(g(a))=q(g(x))(g(x)-g(a))}]
and
         g ( x ) &#x2212; g ( a ) = r ( x ) ( x &#x2212; a ) .   {\displaystyle
      g(x)-g(a)=r(x)(x-a).}  [{\displaystyle g(x)-g(a)=r(x)(x-a).}]
Therefore,
         f ( g ( x ) ) &#x2212; f ( g ( a ) ) = q ( g ( x ) ) r ( x ) ( x
      &#x2212; a ) ,   {\displaystyle f(g(x))-f(g(a))=q(g(x))r(x)(x-a),}  [
      {\displaystyle f(g(x))-f(g(a))=q(g(x))r(x)(x-a),}]
but the function given by h(x) = q(g(x))r(x) is continuous at a, and we get,
for this a
         ( f ( g ( a ) )  ) &#x2032;  = q ( g ( a ) ) r ( a ) =  f &#x2032;
      ( g ( a ) )  g &#x2032;  ( a ) .   {\displaystyle (f(g(a)))'=q(g(a))r
      (a)=f'(g(a))g'(a).}  [{\displaystyle (f(g(a)))'=q(g(a))r(a)=f'(g(a))g'
      (a).}]
A similar approach works for continuously differentiable (vector-)functions of
many variables. This method of factoring also allows a unified approach to
stronger forms of differentiability, when the derivative is required to be
Lipschitz_continuous, HÃ¶lder_continuous, etc. Differentiation itself can be
viewed as the polynomial_remainder_theorem (the little BÃ©zout theorem, or
factor theorem), generalized to an appropriate class of functions.[citation
needed]
*** Proof via infinitesimals[edit] ***
If     y = f ( x )   {\displaystyle y=f(x)}  [y=f(x)] and     x = g ( t )
{\displaystyle x=g(t)}  [x=g(t)] then choosing infinitesimal     &#x0394; t
&#x2260; 0   {\displaystyle \Delta t\not =0}  [\Delta t\not =0] we compute the
corresponding     &#x0394; x = g ( t + &#x0394; t ) &#x2212; g ( t )
{\displaystyle \Delta x=g(t+\Delta t)-g(t)}  [\Delta x=g(t+\Delta t)-g(t)] and
then the corresponding     &#x0394; y = f ( x + &#x0394; x ) &#x2212; f ( x )
{\displaystyle \Delta y=f(x+\Delta x)-f(x)}  [\Delta y=f(x+\Delta x)-f(x)], so
that
            &#x0394; y   &#x0394; t    =    &#x0394; y   &#x0394; x
      &#x0394; x   &#x0394; t      {\displaystyle {\frac {\Delta y}{\Delta t}}=
      {\frac {\Delta y}{\Delta x}}{\frac {\Delta x}{\Delta t}}}  [{\frac
      {\Delta y}{\Delta t}}={\frac  {\Delta y}{\Delta x}}{\frac  {\Delta x}
      {\Delta t}}]
and applying the standard_part we obtain
            d y   d t    =    d y   d x       d x   d t      {\displaystyle
      {\frac {dy}{dt}}={\frac {dy}{dx}}{\frac {dx}{dt}}}  [{\frac  {dy}{dt}}=
      {\frac  {dy}{dx}}{\frac  {dx}{dt}}]
which is the chain rule.
***** Multivariable case[edit] *****
The generalization of the chain rule to multi-variable_functions is rather
technical. However, it is simpler to write in the case of functions of the form
         f (  g  1   ( x ) , &#x2026; ,  g  k   ( x ) ) .   {\displaystyle f(g_
      {1}(x),\dots ,g_{k}(x)).}  [{\displaystyle f(g_{1}(x),\dots ,g_{k}(x)).}]
As this case occurs often in the study of functions of a single variable, it is
worth describing it separately.
**** Case of f(g1(x), ... , gk(x))[edit] ****
For writing the chain rule for a function of the form
      f(g1(x), ... , gk(x)),
one needs the partial_derivatives of f with respect to its k arguments. The
usual notations for partial derivatives involve names for the arguments of the
function. As these arguments are not named in the above formula, it is simpler
and clearer to denote by
          D  i   f   {\displaystyle D_{i}f}  [{\displaystyle D_{i}f}]
the derivative of f with respect to its ith argument, and by
          D  i   f ( z )   {\displaystyle D_{i}f(z)}  [{\displaystyle D_{i}f
      (z)}]
the value of this derivative at z.
With this notation, the chain rule is
           d  d x    f (  g  1   ( x ) , &#x2026; ,  g  k   ( x ) ) =  &#x2211;
      i = 1   k    (    d  d x      g  i    ( x )  )   D  i   f (  g  1   ( x )
      , &#x2026; ,  g  k   ( x ) ) .   {\displaystyle {\frac {d}{dx}}f(g_{1}
      (x),\dots ,g_{k}(x))=\sum _{i=1}^{k}\left({\frac {d}{dx}}{g_{i}}
      (x)\right)D_{i}f(g_{1}(x),\dots ,g_{k}(x)).}  [{\displaystyle {\frac {d}
      {dx}}f(g_{1}(x),\dots ,g_{k}(x))=\sum _{i=1}^{k}\left({\frac {d}{dx}}{g_
      {i}}(x)\right)D_{i}f(g_{1}(x),\dots ,g_{k}(x)).}]
*** Example: arithmetic operations[edit] ***
If the function f is addition, that is, if
         f ( u , v ) = u + v ,   {\displaystyle f(u,v)=u+v,}  [{\displaystyle f
      (u,v)=u+v,}]
then      D  1   f =  D  2   f = 1   {\displaystyle D_{1}f=D_{2}f=1}  [
{\displaystyle D_{1}f=D_{2}f=1}] (the constant function 1). Thus, the chain
rule gives
           d  d x    ( g ( x ) + h ( x ) ) =   d  d x    g ( x ) +   d  d x
      h ( x ) .   {\displaystyle {\frac {d}{dx}}(g(x)+h(x))={\frac {d}{dx}}g
      (x)+{\frac {d}{dx}}h(x).}  [{\displaystyle {\frac {d}{dx}}(g(x)+h(x))=
      {\frac {d}{dx}}g(x)+{\frac {d}{dx}}h(x).}]
For multiplication
         f ( u , v ) = u v ,   {\displaystyle f(u,v)=uv,}  [{\displaystyle f
      (u,v)=uv,}]
the partials are      D  1   f = v   {\displaystyle D_{1}f=v}  [{\displaystyle
D_{1}f=v}] and      D  2   f = u .   {\displaystyle D_{2}f=u.}  [{\displaystyle
D_{2}f=u.}] Thus,
           d  d x    ( g ( x ) h ( x ) ) = h ( x )   d  d x    g ( x ) + g ( x
      )   d  d x    h ( x ) .   {\displaystyle {\frac {d}{dx}}(g(x)h(x))=h(x)
      {\frac {d}{dx}}g(x)+g(x){\frac {d}{dx}}h(x).}  [{\displaystyle {\frac {d}
      {dx}}(g(x)h(x))=h(x){\frac {d}{dx}}g(x)+g(x){\frac {d}{dx}}h(x).}]
The case of exponentiation
         f ( u , v ) =  u  v     {\displaystyle f(u,v)=u^{v}}  [{\displaystyle
      f(u,v)=u^{v}}]
is slightly more complicated, as
          D  1   f = v  u  v &#x2212; 1   ,   {\displaystyle D_{1}f=vu^{v-1},}
      [{\displaystyle D_{1}f=vu^{v-1},}]
and, as      u  v   =  e  v ln &#x2061; u   ,   {\displaystyle u^{v}=e^{v\ln
u},}  [{\displaystyle u^{v}=e^{v\ln u},}]
          D  2   f =  u  v   ln &#x2061; u .   {\displaystyle D_{2}f=u^{v}\ln
      u.}  [{\displaystyle D_{2}f=u^{v}\ln u.}]
It follows that
           d  d x    ( g ( x  )  h ( x )   ) = h ( x ) g ( x  )  h ( x )
      &#x2212; 1     d  d x    g ( x ) + g ( x  )  h ( x )   ln &#x2061; g ( x
      )   d  d x    h ( x ) .   {\displaystyle {\frac {d}{dx}}(g(x)^{h(x)})=h
      (x)g(x)^{h(x)-1}{\frac {d}{dx}}g(x)+g(x)^{h(x)}\ln g(x){\frac {d}{dx}}h
      (x).}  [{\displaystyle {\frac {d}{dx}}(g(x)^{h(x)})=h(x)g(x)^{h(x)-1}
      {\frac {d}{dx}}g(x)+g(x)^{h(x)}\ln g(x){\frac {d}{dx}}h(x).}]
**** General rule[edit] ****
The simplest way for writing the chain rule in the general case is to use the
total_derivative, which is a linear transformation that captures all
directional_derivatives in a single formula. Consider differentiable functions
f : Rm â Rk and g : Rn â Rm, and a point a in Rn. Let Da g denote the total
derivative of g at a and Dg(a) f denote the total derivative of f at g(a).
These two derivatives are linear transformations Rn â Rm and Rm â Rk,
respectively, so they can be composed. The chain rule for total derivatives is
that their composite is the total derivative of f â g at a:
          D   a    ( f &#x2218; g ) =  D  g (  a  )   f &#x2218;  D   a    g ,
      {\displaystyle D_{\mathbf {a} }(f\circ g)=D_{g(\mathbf {a} )}f\circ D_
      {\mathbf {a} }g,}  [D_{\mathbf{a}}(f \circ g) = D_{g(\mathbf{a})}f \circ
      D_{\mathbf{a}}g,]
or for short,
         D ( f &#x2218; g ) = D f &#x2218; D g .   {\displaystyle D(f\circ
      g)=Df\circ Dg.}  [D(f \circ g) = Df \circ Dg.]
The higher-dimensional chain rule can be proved using a technique similar to
the second proof given above.
Because the total derivative is a linear transformation, the functions
appearing in the formula can be rewritten as matrices. The matrix corresponding
to a total derivative is called a Jacobian_matrix, and the composite of two
derivatives corresponds to the product of their Jacobian matrices. From this
perspective the chain rule therefore says:
          J  f &#x2218; g   (  a  ) =  J  f   ( g (  a  ) )  J  g   (  a  ) ,
      {\displaystyle J_{f\circ g}(\mathbf {a} )=J_{f}(g(\mathbf {a} ))J_{g}
      (\mathbf {a} ),}  [J_{{f\circ g}}({\mathbf  {a}})=J_{{f}}(g({\mathbf
      {a}}))J_{{g}}({\mathbf  {a}}),]
or for short,
          J  f &#x2218; g   = (  J  f   &#x2218; g )  J  g   .   {\displaystyle
      J_{f\circ g}=(J_{f}\circ g)J_{g}.}  [J_{{f\circ g}}=(J_{f}\circ g)J_{g}.]
That is, the Jacobian of a composite function is the product of the Jacobians
of the composed functions (evaluated at the appropriate points).
The higher-dimensional chain rule is a generalization of the one-dimensional
chain rule. If k, m, and n are 1, so that f : R â R and g : R â R, then the
Jacobian matrices of f and g are 1 Ã 1. Specifically, they are:
              J  g   ( a )    =   (     g &#x2032;  ( a )    )   ,      J  f
      ( g ( a ) )    =   (     f &#x2032;  ( g ( a ) )    )   .
      {\displaystyle {\begin{aligned}J_{g}(a)&={\begin{pmatrix}g'(a)\end
      {pmatrix}},\\J_{f}(g(a))&={\begin{pmatrix}f'(g(a))\end{pmatrix}}.\end
      {aligned}}}  [{\begin{aligned}J_{g}(a)&={\begin{pmatrix}g'(a)\end
      {pmatrix}},\\J_{{f}}(g(a))&={\begin{pmatrix}f'(g(a))\end{pmatrix}}.\end
      {aligned}}]
The Jacobian of f â g is the product of these 1 Ã 1 matrices, so it is fâ²
(g(a))âgâ²(a), as expected from the one-dimensional chain rule. In the
language of linear transformations, Da(g) is the function which scales a vector
by a factor of gâ²(a) and Dg(a)(f) is the function which scales a vector by a
factor of fâ²(g(a)). The chain rule says that the composite of these two
linear transformations is the linear transformation Da(f â g), and therefore
it is the function that scales a vector by fâ²(g(a))âgâ²(a).
Another way of writing the chain rule is used when f and g are expressed in
terms of their components as y = f(u) = (f1(u), â¦, fk(u)) and u = g(x) = (g1
(x), â¦, gm(x)). In this case, the above rule for Jacobian matrices is usually
written as:
            &#x2202; (  y  1   , &#x2026; ,  y  k   )   &#x2202; (  x  1   ,
      &#x2026; ,  x  n   )    =    &#x2202; (  y  1   , &#x2026; ,  y  k   )
      &#x2202; (  u  1   , &#x2026; ,  u  m   )       &#x2202; (  u  1   ,
      &#x2026; ,  u  m   )   &#x2202; (  x  1   , &#x2026; ,  x  n   )    .
      {\displaystyle {\frac {\partial (y_{1},\ldots ,y_{k})}{\partial (x_
      {1},\ldots ,x_{n})}}={\frac {\partial (y_{1},\ldots ,y_{k})}{\partial (u_
      {1},\ldots ,u_{m})}}{\frac {\partial (u_{1},\ldots ,u_{m})}{\partial (x_
      {1},\ldots ,x_{n})}}.}  [\frac{\partial(y_1, \ldots, y_k)}{\partial(x_1,
      \ldots, x_n)} = \frac{\partial(y_1, \ldots, y_k)}{\partial(u_1, \ldots,
      u_m)} \frac{\partial(u_1, \ldots, u_m)}{\partial(x_1, \ldots, x_n)}.]
The chain rule for total derivatives implies a chain rule for partial
derivatives. Recall that when the total derivative exists, the partial
derivative in the ith coordinate direction is found by multiplying the Jacobian
matrix by the ith basis vector. By doing this to the formula above, we find:
            &#x2202; (  y  1   , &#x2026; ,  y  k   )   &#x2202;  x  i      =
      &#x2202; (  y  1   , &#x2026; ,  y  k   )   &#x2202; (  u  1   , &#x2026;
      ,  u  m   )       &#x2202; (  u  1   , &#x2026; ,  u  m   )   &#x2202;  x
      i      .   {\displaystyle {\frac {\partial (y_{1},\ldots ,y_{k})}
      {\partial x_{i}}}={\frac {\partial (y_{1},\ldots ,y_{k})}{\partial (u_
      {1},\ldots ,u_{m})}}{\frac {\partial (u_{1},\ldots ,u_{m})}{\partial x_
      {i}}}.}  [\frac{\partial(y_1, \ldots, y_k)}{\partial x_i} = \frac
      {\partial(y_1, \ldots, y_k)}{\partial(u_1, \ldots, u_m)} \frac{\partial
      (u_1, \ldots, u_m)}{\partial x_i}.]
Since the entries of the Jacobian matrix are partial derivatives, we may
simplify the above formula to get:
            &#x2202; (  y  1   , &#x2026; ,  y  k   )   &#x2202;  x  i      =
      &#x2211;  &#x2113; = 1   m      &#x2202; (  y  1   , &#x2026; ,  y  k   )
      &#x2202;  u  &#x2113;         &#x2202;  u  &#x2113;     &#x2202;  x  i
      .   {\displaystyle {\frac {\partial (y_{1},\ldots ,y_{k})}{\partial x_
      {i}}}=\sum _{\ell =1}^{m}{\frac {\partial (y_{1},\ldots ,y_{k})}{\partial
      u_{\ell }}}{\frac {\partial u_{\ell }}{\partial x_{i}}}.}  [\frac
      {\partial(y_1, \ldots, y_k)}{\partial x_i} = \sum_{\ell = 1}^m \frac
      {\partial(y_1, \ldots, y_k)}{\partial u_\ell} \frac{\partial u_\ell}
      {\partial x_i}.]
More conceptually, this rule expresses the fact that a change in the xi
direction may change all of g1 through gm, and any of these changes may affect
f.
In the special case where k = 1, so that f is a real-valued function, then this
formula simplifies even further:
            &#x2202; y   &#x2202;  x  i      =  &#x2211;  &#x2113; = 1   m
      &#x2202; y   &#x2202;  u  &#x2113;         &#x2202;  u  &#x2113;
      &#x2202;  x  i      .   {\displaystyle {\frac {\partial y}{\partial x_
      {i}}}=\sum _{\ell =1}^{m}{\frac {\partial y}{\partial u_{\ell }}}{\frac
      {\partial u_{\ell }}{\partial x_{i}}}.}  [\frac{\partial y}{\partial x_i}
      = \sum_{\ell = 1}^m \frac{\partial y}{\partial u_\ell} \frac{\partial
      u_\ell}{\partial x_i}.]
This can be rewritten as a dot_product. Recalling that u = (g1, â¦, gm), the
partial derivative âu / âxi is also a vector, and the chain rule says that:
            &#x2202; y   &#x2202;  x  i      = &#x2207; y &#x22C5;    &#x2202;
      u    &#x2202;  x  i      .   {\displaystyle {\frac {\partial y}{\partial
      x_{i}}}=\nabla y\cdot {\frac {\partial \mathbf {u} }{\partial x_{i}}}.}
      [{\displaystyle {\frac {\partial y}{\partial x_{i}}}=\nabla y\cdot {\frac
      {\partial \mathbf {u} }{\partial x_{i}}}.}]
*** Example[edit] ***
Given u(x, y) = x2 + 2y where x(r, t) = r sin(t) and y(r,t) = sin2(t),
determine the value of âu / âr and âu / ât using the chain rule.
            &#x2202; u   &#x2202; r    =    &#x2202; u   &#x2202; x
      &#x2202; x   &#x2202; r    +    &#x2202; u   &#x2202; y       &#x2202; y
      &#x2202; r    = ( 2 x ) ( sin &#x2061; ( t ) ) + ( 2 ) ( 0 ) = 2 r  sin
      2   &#x2061; ( t ) ,   {\displaystyle {\frac {\partial u}{\partial r}}=
      {\frac {\partial u}{\partial x}}{\frac {\partial x}{\partial r}}+{\frac
      {\partial u}{\partial y}}{\frac {\partial y}{\partial r}}=(2x)(\sin(t))+
      (2)(0)=2r\sin ^{2}(t),}  [{\frac  {\partial u}{\partial r}}={\frac
      {\partial u}{\partial x}}{\frac  {\partial x}{\partial r}}+{\frac
      {\partial u}{\partial y}}{\frac  {\partial y}{\partial r}}=(2x)(\sin(t))+
      (2)(0)=2r\sin ^{2}(t),]
and
                &#x2202; u   &#x2202; t       =    &#x2202; u   &#x2202; x
      &#x2202; x   &#x2202; t    +    &#x2202; u   &#x2202; y       &#x2202; y
      &#x2202; t          = ( 2 x ) ( r cos &#x2061; ( t ) ) + ( 2 ) ( 2 sin
      &#x2061; ( t ) cos &#x2061; ( t ) )       = ( 2 r sin &#x2061; ( t ) )
      ( r cos &#x2061; ( t ) ) + 4 sin &#x2061; ( t ) cos &#x2061; ( t )
      = 2 (  r  2   + 2 ) sin &#x2061; ( t ) cos &#x2061; ( t )       = (  r  2
      + 2 ) sin &#x2061; ( 2 t ) .       {\displaystyle {\begin{aligned}{\frac
      {\partial u}{\partial t}}&={\frac {\partial u}{\partial x}}{\frac
      {\partial x}{\partial t}}+{\frac {\partial u}{\partial y}}{\frac
      {\partial y}{\partial t}}\\&=(2x)(r\cos(t))+(2)(2\sin(t)\cos(t))\\&=
      (2r\sin(t))(r\cos(t))+4\sin(t)\cos(t)\\&=2(r^{2}+2)\sin(t)\cos(t)\\&=(r^
      {2}+2)\sin(2t).\end{aligned}}}  [\begin{align}\frac{\partial u}{\partial
      t}
      &= \frac{\partial u}{\partial x} \frac{\partial x}{\partial t}+\frac
      {\partial u}{\partial y} \frac{\partial y}{\partial t} \\
      &= (2x)(r\cos(t)) + (2)(2\sin(t)\cos(t)) \\
      &= (2r\sin(t))(r\cos(t)) + 4\sin(t)\cos(t) \\
      &= 2(r^2 + 2) \sin(t)\cos(t) \\
      &= (r^2 + 2) \sin(2t).\end{align}]
*** Higher derivatives of multivariable functions[edit] ***
Main article: FaÃ _di_Bruno's_formula_Â§ Multivariate_version
FaÃ  di Bruno's formula for higher-order derivatives of single-variable
functions generalizes to the multivariable case. If y = f(u) is a function of u
= g(x) as above, then the second derivative of f â g is:
             &#x2202;  2   y   &#x2202;  x  i   &#x2202;  x  j      =  &#x2211;
      k    (     &#x2202; y   &#x2202;  u  k          &#x2202;  2    u  k
      &#x2202;  x  i   &#x2202;  x  j       )  +  &#x2211;  k , &#x2113;
      (      &#x2202;  2   y   &#x2202;  u  k   &#x2202;  u  &#x2113;
      &#x2202;  u  k     &#x2202;  x  i         &#x2202;  u  &#x2113;
      &#x2202;  x  j       )  .   {\displaystyle {\frac {\partial ^{2}y}
      {\partial x_{i}\partial x_{j}}}=\sum _{k}\left({\frac {\partial y}
      {\partial u_{k}}}{\frac {\partial ^{2}u_{k}}{\partial x_{i}\partial x_
      {j}}}\right)+\sum _{k,\ell }\left({\frac {\partial ^{2}y}{\partial u_
      {k}\partial u_{\ell }}}{\frac {\partial u_{k}}{\partial x_{i}}}{\frac
      {\partial u_{\ell }}{\partial x_{j}}}\right).}  [{\frac  {\partial ^{2}y}
      {\partial x_{i}\partial x_{j}}}=\sum _{k}\left({\frac  {\partial y}
      {\partial u_{k}}}{\frac  {\partial ^{2}u_{k}}{\partial x_{i}\partial x_
      {j}}}\right)+\sum _{{k,\ell }}\left({\frac  {\partial ^{2}y}{\partial u_
      {k}\partial u_{\ell }}}{\frac  {\partial u_{k}}{\partial x_{i}}}{\frac
      {\partial u_{\ell }}{\partial x_{j}}}\right).]
***** Further generalizations[edit] *****
All extensions of calculus have a chain rule. In most of these, the formula
remains the same, though the meaning of that formula may be vastly different.
One generalization is to manifolds. In this situation, the chain rule
represents the fact that the derivative of f â g is the composite of the
derivative of f and the derivative of g. This theorem is an immediate
consequence of the higher dimensional chain rule given above, and it has
exactly the same formula.
The chain rule is also valid for FrÃ©chet_derivatives in Banach_spaces. The
same formula holds as before. This case and the previous one admit a
simultaneous generalization to Banach_manifolds.
In abstract_algebra, the derivative is interpreted as a morphism of modules of
KÃ¤hler_differentials. A ring_homomorphism of commutative_rings f : R â S
determines a morphism of KÃ¤hler differentials Df : Î©R â Î©S which sends an
element dr to d(f(r)), the exterior differential of f(r). The formula D(f â
g) = Df â Dg holds in this context as well.
The common feature of these examples is that they are expressions of the idea
that the derivative is part of a functor. A functor is an operation on spaces
and functions between them. It associates to each space a new space and to each
function between two spaces a new function between the corresponding new
spaces. In each of the above cases, the functor sends each space to its tangent
bundle and it sends each function to its derivative. For example, in the
manifold case, the derivative sends a Cr-manifold to a Crâ1-manifold (its
tangent bundle) and a Cr-function to its total derivative. There is one
requirement for this to be a functor, namely that the derivative of a composite
must be the composite of the derivatives. This is exactly the formula D(f â
g) = Df â Dg.
There are also chain rules in stochastic_calculus. One of these, ItÅ's_lemma,
expresses the composite of an ItÅ process (or more generally a semimartingale)
dXt with a twice-differentiable function f. In ItÅ's lemma, the derivative of
the composite function depends not only on dXt and the derivative of f but also
on the second derivative of f. The dependence on the second derivative is a
consequence of the non-zero quadratic_variation of the stochastic process,
which broadly speaking means that the process can move up and down in a very
rough way. This variant of the chain rule is not an example of a functor
because the two functions being composed are of different types.
***** See also[edit] *****
    * Integration_by_substitution
    * Leibniz_integral_rule
    * Quotient_rule
    * Triple_product_rule
    * Product_rule
    * Automatic_differentiation, a computational method that makes heavy use of
      the chain rule to compute exact numerical derivatives.
***** References[edit] *****
   1. ^ a b"Chain_Rule_in_Leibniz_Notation". oregonstate.edu. Retrieved 2019-
      07-28.
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
   3. ^RodrÃ­guez, Omar HernÃ¡ndez; LÃ³pez FernÃ¡ndez, Jorge M. (2010). "A
      Semiotic_Reflection_on_the_Didactics_of_the_Chain_Rule". The Mathematics
      Enthusiast. 7 (2): 321â332. Retrieved 2019-08-04.
   4. ^Apostol,_Tom (1974). Mathematical analysis (2nd ed.). Addison Wesley.
      Theorem 5.5.
   5. ^ a b"Chain_Rule_for_Derivative". Math Vault. 2016-06-05. Retrieved 2019-
      07-28.
   6. ^Kuhn, Stephen (1991). "The Derivative Ã¡ la CarathÃ©odory". The_American
      Mathematical_Monthly. 98 (1): 40â44. JSTOR 2324035.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Leibniz_rule", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Weisstein,_Eric_W. "Chain_Rule". MathWorld.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Chain_rule&oldid=909419438"
Categories:
    * Differentiation_rules
    * Theorems_in_calculus
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_February_2016
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
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * BÃ¢n-lÃ¢m-gÃº
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 5 August 2019, at 09:25 (UTC).
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
