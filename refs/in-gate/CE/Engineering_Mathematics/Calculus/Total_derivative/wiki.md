The following text has been accessed from https://en.wikipedia.org/wiki/Total_derivative at Thu Aug 8 23:41:36 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Total derivative ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (July 2013)(Learn_how_and_when
 to_remove_this_template_message)
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
In mathematics, the total derivative of a function     f   {\displaystyle f}
[f] at a point is the best linear_approximation near this point of the function
with respect to its arguments. Unlike partial_derivatives, the total derivative
approximates the function with respect to all of its arguments, not just a
single one. In many situations, this is the same as considering all partial
derivatives simultaneously. The term "total derivative" is primarily used when
f   {\displaystyle f}  [f] is a function of several variables, because when
f   {\displaystyle f}  [f] is a function of a single variable, the total
derivative is the same as the derivative of the function.[1]:198â203
"Total derivative" is sometimes also used as a synonym for the material
derivative in fluid_mechanics.
⁰
***** Contents *****
    * 1_The_total_derivative_as_a_linear_map
    * 2_The_total_derivative_as_a_differential_form
    * 3_The_chain_rule_for_total_derivatives
          o 3.1_Example:_Differentiation_with_direct_dependencies
          o 3.2_Example:_Differentiation_with_indirect_dependencies
    * 4_Total_differential_equation
    * 5_Application_to_equation_systems
    * 6_References
    * 7_External_links
***** The total derivative as a linear map[edit] *****
Let     U &#x2286;   R   n     {\displaystyle U\subseteq \mathbf {R} ^{n}}  [
{\displaystyle U\subseteq \mathbf {R} ^{n}}] be an open_subset. Then a function
f : U &#x2192;   R   m     {\displaystyle f:U\rightarrow \mathbf {R} ^{m}}  [
{\displaystyle f:U\rightarrow \mathbf {R} ^{m}}] is said to be (totally)
differentiable at a point     a &#x2208; U   {\displaystyle a\in U}  [
{\displaystyle a\in U}] if there exists a linear_transformation     d  f  a   :
R   n   &#x2192;   R   m     {\displaystyle df_{a}:\mathbf {R} ^{n}\rightarrow
\mathbf {R} ^{m}}  [{\displaystyle df_{a}:\mathbf {R} ^{n}\rightarrow \mathbf
{R} ^{m}}] such that
          lim  x &#x2192; a      &#x2016; f ( x ) &#x2212; f ( a ) &#x2212; d
      f  a   ( x &#x2212; a ) &#x2016;   &#x2016; x &#x2212; a &#x2016;    = 0.
      {\displaystyle \lim _{x\rightarrow a}{\frac {\|f(x)-f(a)-df_{a}(x-a)\|}
      {\|x-a\|}}=0.}  [{\displaystyle \lim _{x\rightarrow a}{\frac {\|f(x)-f
      (a)-df_{a}(x-a)\|}{\|x-a\|}}=0.}]
The linear_map     d  f  a     {\displaystyle df_{a}}  [{\displaystyle df_{a}}]
is called the (total) derivative or (total) differential of     f
{\displaystyle f}  [f] at     a   {\displaystyle a}  [a]. Other notations for
the total derivative include      D  a   f   {\displaystyle D_{a}f}  [
{\displaystyle D_{a}f}] and     D f ( a )   {\displaystyle Df(a)}  [Df(a)]. A
function is (totally) differentiable if its total derivative exists at every
point in its domain.
Conceptually, the definition of the total derivative expresses the idea that
d  f  a     {\displaystyle df_{a}}  [{\displaystyle df_{a}}] is the best linear
approximation to     f   {\displaystyle f}  [f] at the point     a
{\displaystyle a}  [a]. This can be made precise by quantifying the error in
the linear approximation determined by     d  f  a     {\displaystyle df_{a}}
[{\displaystyle df_{a}}]. To do so, write
         f ( a + h ) = f ( a ) + d  f  a   ( h ) + &#x03B5; ( h ) ,
      {\displaystyle f(a+h)=f(a)+df_{a}(h)+\varepsilon (h),}  [{\displaystyle f
      (a+h)=f(a)+df_{a}(h)+\varepsilon (h),}]
where     &#x03B5; ( h )   {\displaystyle \varepsilon (h)}  [\varepsilon(h)]
equals the error in the approximation. To say that the derivative of     f
{\displaystyle f}  [f] at     a   {\displaystyle a}  [a] is     d  f  a
{\displaystyle df_{a}}  [{\displaystyle df_{a}}] is equivalent to the statement
         &#x03B5; ( h ) = o ( &#x2016; h &#x2016; ) ,   {\displaystyle
      \varepsilon (h)=o(\lVert h\rVert ),}  [{\displaystyle \varepsilon (h)=o
      (\lVert h\rVert ),}]
where     o   {\displaystyle o}  [o] is little-o_notation and indicates that
&#x03B5; ( h )   {\displaystyle \varepsilon (h)}  [\varepsilon(h)] is much
smaller than     &#x2016; h &#x2016;   {\displaystyle \lVert h\rVert }  [
{\displaystyle \lVert h\rVert }] as     h &#x2192; 0   {\displaystyle h\to 0}
[h \to 0]. The total derivative     d  f  a     {\displaystyle df_{a}}  [
{\displaystyle df_{a}}] is the unique linear transformation for which the error
term is this small, and this is the sense in which it is the best linear
approximation to     f   {\displaystyle f}  [f].
The function     f   {\displaystyle f}  [f] is differentiable if and only if
each of its components      f  i   &#x003A; U &#x2192;  R    {\displaystyle f_
{i}\colon U\to \mathbf {R} }  [{\displaystyle f_{i}\colon U\to \mathbf {R} }]
is differentiable, so when studying total derivatives, it is often possible to
work one coordinate at a time in the codomain. However, the same is not true of
the coordinates in the domain. It is true that if     f   {\displaystyle f}
[f] is differentiable at     a   {\displaystyle a}  [a], then each partial
derivative     &#x2202; f  /  &#x2202;  x  i     {\displaystyle \partial f/
\partial x_{i}}  [\partial f/\partial x_{i}] exists at     a   {\displaystyle
a}  [a]. The converse is false: It can happen that all of the partial
derivatives of     f   {\displaystyle f}  [f] at     a   {\displaystyle a}  [a]
exist, but     f   {\displaystyle f}  [f] is not differentiable at     a
{\displaystyle a}  [a]. This means that the function is very "rough" at     a
{\displaystyle a}  [a], to such an extreme that its behavior cannot be
adequately described by its behavior in the coordinate directions. When     f
{\displaystyle f}  [f] is not so rough, this cannot happen. More precisely, if
all the partial derivatives of     f   {\displaystyle f}  [f] at     a
{\displaystyle a}  [a] exist and are continuous in a neighborhood of     a
{\displaystyle a}  [a], then     f   {\displaystyle f}  [f] is differentiable
at     a   {\displaystyle a}  [a]. When this happens, then in addition, the
total derivative of     f   {\displaystyle f}  [f] is the linear transformation
corresponding to the Jacobian_matrix of partial derivatives at that point.[2]
***** The total derivative as a differential form[edit] *****
When the function under consideration is real-valued, the total derivative can
be recast using differential_forms. For example, suppose that     f &#x003A;
R   n   &#x2192;  R    {\displaystyle f\colon \mathbf {R} ^{n}\to \mathbf {R} }
[{\displaystyle f\colon \mathbf {R} ^{n}\to \mathbf {R} }] is a differentiable
function of variables      x  1   , &#x2026; ,  x  n     {\displaystyle x_
{1},\ldots ,x_{n}}  [x_{1},\ldots ,x_{n}]. The total derivative of     f
{\displaystyle f}  [f] at     a   {\displaystyle a}  [a] may be written in
terms of its Jacobian matrix, which in this instance simplifies to the
gradient:
         d  f  a   =   (       &#x2202; f   &#x2202;  x  1      ,   &#x22EF;
      ,      &#x2202; f   &#x2202;  x  n         )   .   {\displaystyle df_{a}=
      {\begin{pmatrix}{\frac {\partial f}{\partial x_{1}}},&\cdots &,&{\frac
      {\partial f}{\partial x_{n}}}\end{pmatrix}}.}  [{\displaystyle df_{a}=
      {\begin{pmatrix}{\frac {\partial f}{\partial x_{1}}},&\cdots &,&{\frac
      {\partial f}{\partial x_{n}}}\end{pmatrix}}.}]
The linear approximation property of the total derivative implies that if
         &#x0394; x =    (    &#x0394;  x  1   ,   &#x22EF;   ,   &#x0394;  x
      n      )    T     {\displaystyle \Delta x={\begin{pmatrix}\Delta x_
      {1},&\cdots &,&\Delta x_{n}\end{pmatrix}}^{T}}  [{\displaystyle \Delta x=
      {\begin{pmatrix}\Delta x_{1},&\cdots &,&\Delta x_{n}\end{pmatrix}}^{T}}]
is a small vector (where the     T   {\displaystyle T}  [T] denotes transpose,
so that this vector is a column vector), then
         f ( a + &#x0394; x ) &#x2212; f ( a ) &#x2248; d  f  a   ( &#x0394; x
      ) =  &#x2211;  i = 1   n      &#x2202; f   &#x2202;  x  i      &#x0394;
      x  i   .   {\displaystyle f(a+\Delta x)-f(a)\approx df_{a}(\Delta x)=\sum
      _{i=1}^{n}{\frac {\partial f}{\partial x_{i}}}\Delta x_{i}.}  [
      {\displaystyle f(a+\Delta x)-f(a)\approx df_{a}(\Delta x)=\sum _{i=1}^{n}
      {\frac {\partial f}{\partial x_{i}}}\Delta x_{i}.}]
Heuristically, this suggests that if     d  x  1   , &#x2026; , d  x  n
{\displaystyle dx_{1},\ldots ,dx_{n}}  [{\displaystyle dx_{1},\ldots ,dx_{n}}]
are infinitesimal increments in the coordinate directions, then
         d  f  a   ( x ) =  &#x2211;  i = 1   n      &#x2202; f   &#x2202;  x
      i      ( a ) d  x  i   .   {\displaystyle df_{a}(x)=\sum _{i=1}^{n}{\frac
      {\partial f}{\partial x_{i}}}(a)dx_{i}.}  [{\displaystyle df_{a}(x)=\sum
      _{i=1}^{n}{\frac {\partial f}{\partial x_{i}}}(a)dx_{i}.}]
The theory of differential_forms is one way to give a precise meaning to
infinitesimal increments such as     d  x  i     {\displaystyle dx_{i}}  [
{\displaystyle dx_{i}}]. In this theory,     d  x  i     {\displaystyle dx_{i}}
[{\displaystyle dx_{i}}] is a linear_functional on the vector space       R   n
{\displaystyle \mathbf {R} ^{n}}  [\mathbf {R} ^{n}]. Evaluating     d  x  i
{\displaystyle dx_{i}}  [{\displaystyle dx_{i}}] at a vector     h
{\displaystyle h}  [h] in       R   n     {\displaystyle \mathbf {R} ^{n}}
[\mathbf {R} ^{n}] measures how much     h   {\displaystyle h}  [h] points in
the     i   {\displaystyle i}  [i]th coordinate direction. The total derivative
d  f  a     {\displaystyle df_{a}}  [{\displaystyle df_{a}}] is a linear
combination of linear functionals and hence is itself a linear functional. The
evaluation     d  f  a   ( h )   {\displaystyle df_{a}(h)}  [{\displaystyle df_
{a}(h)}] measures how much     h   {\displaystyle h}  [h] points in the
direction determined by     f   {\displaystyle f}  [f] at     a
{\displaystyle a}  [a], and this direction is the gradient. This point of view
makes the total derivative an instance of the exterior_derivative.
Suppose now that     f   {\displaystyle f}  [f] is a vector-valued function,
that is,     f &#x003A;   R   n   &#x2192;   R   m     {\displaystyle f\colon
\mathbf {R} ^{n}\to \mathbf {R} ^{m}}  [{\displaystyle f\colon \mathbf {R} ^
{n}\to \mathbf {R} ^{m}}]. In this case, the components      f  i
{\displaystyle f_{i}}  [f_{i}] of     f   {\displaystyle f}  [f] are real-
valued functions, so they have associated differential forms     d  f  i
{\displaystyle df_{i}}  [{\displaystyle df_{i}}]. The total derivative     d f
{\displaystyle df}  [df] amalgamates these forms into a single object and is
therefore an instance of a vector-valued_differential_form.
***** The chain rule for total derivatives[edit] *****
Main article: Chain_rule
The chain rule has a particularly elegant statement in terms of total
derivatives. It says that, for two functions     f   {\displaystyle f}  [f] and
g   {\displaystyle g}  [g], the total derivative of the composite     g
&#x2218; f   {\displaystyle g\circ f}  [g\circ f] at     a   {\displaystyle a}
[a] satisfies
         d ( g &#x2218; f  )  a   = d  g  f ( a )   &#x2218; d  f  a   .
      {\displaystyle d(g\circ f)_{a}=dg_{f(a)}\circ df_{a}.}  [{\displaystyle d
      (g\circ f)_{a}=dg_{f(a)}\circ df_{a}.}]
If the total derivatives of     f   {\displaystyle f}  [f] and     g
{\displaystyle g}  [g] are identified with their Jacobian matrices, then the
composite on the right-hand side is simply matrix multiplication. This is
enormously useful in applications, as it makes it possible to account for
essentially arbitrary dependencies among the arguments of a composite function.
**** Example: Differentiation with direct dependencies[edit] ****
Suppose that f is a function of two variables, x and y. If these two variables
are independent, so that the domain of f is       R   2     {\displaystyle
\mathbf {R} ^{2}}  [\mathbf{R}^2], then the behavior of f may be understood in
terms of its partial derivatives in the x and y directions. However, in some
situations, x and y may be dependent. For example, it might happen that f is
constrained to a curve     y = y ( x )   {\displaystyle y=y(x)}  [
{\displaystyle y=y(x)}]. In this case, we are actually interested in the
behavior of the composite function     f ( x , y ( x ) )   {\displaystyle f(x,y
(x))}  [{\displaystyle f(x,y(x))}]. The partial derivative of f with respect to
x does not give the true rate of change of f with respect to changing x because
changing x necessarily changes y. However, the chain rule for the total
derivative takes such dependencies into account. Write     &#x03B3; ( x ) = ( x
, y ( x ) )   {\displaystyle \gamma (x)=(x,y(x))}  [{\displaystyle \gamma (x)=
(x,y(x))}]. Then, the chain rule says
         d ( f &#x2218; &#x03B3;  )   x  0     = d  f  (  x  0   , y (  x  0
      ) )   &#x2218; d  &#x03B3;   x  0     .   {\displaystyle d(f\circ \gamma
      )_{x_{0}}=df_{(x_{0},y(x_{0}))}\circ d\gamma _{x_{0}}.}  [{\displaystyle
      d(f\circ \gamma )_{x_{0}}=df_{(x_{0},y(x_{0}))}\circ d\gamma _{x_{0}}.}]
By expressing the total derivative using Jacobian matrices, this becomes:
            d f ( x , y ( x ) )   d x    (  x  0   ) =    &#x2202; f   &#x2202;
      x    (  x  0   , y (  x  0   ) ) &#x22C5;    &#x2202; x   &#x2202; x
      (  x  0   ) +    &#x2202; f   &#x2202; y    (  x  0   , y (  x  0   ) )
      &#x22C5;    &#x2202; y   &#x2202; x    (  x  0   ) .   {\displaystyle
      {\frac {df(x,y(x))}{dx}}(x_{0})={\frac {\partial f}{\partial x}}(x_{0},y
      (x_{0}))\cdot {\frac {\partial x}{\partial x}}(x_{0})+{\frac {\partial f}
      {\partial y}}(x_{0},y(x_{0}))\cdot {\frac {\partial y}{\partial x}}(x_
      {0}).}  [{\displaystyle {\frac {df(x,y(x))}{dx}}(x_{0})={\frac {\partial
      f}{\partial x}}(x_{0},y(x_{0}))\cdot {\frac {\partial x}{\partial x}}(x_
      {0})+{\frac {\partial f}{\partial y}}(x_{0},y(x_{0}))\cdot {\frac
      {\partial y}{\partial x}}(x_{0}).}]
Suppressing the evaluation at      x  0     {\displaystyle x_{0}}  [x_{0}] for
legibility, we may also write this as
            d f ( x , y ( x ) )   d x    =    &#x2202; f   &#x2202; x
      &#x2202; x   &#x2202; x    +    &#x2202; f   &#x2202; y       &#x2202; y
      &#x2202; x    .   {\displaystyle {\frac {df(x,y(x))}{dx}}={\frac
      {\partial f}{\partial x}}{\frac {\partial x}{\partial x}}+{\frac
      {\partial f}{\partial y}}{\frac {\partial y}{\partial x}}.}  [
      {\displaystyle {\frac {df(x,y(x))}{dx}}={\frac {\partial f}{\partial x}}
      {\frac {\partial x}{\partial x}}+{\frac {\partial f}{\partial y}}{\frac
      {\partial y}{\partial x}}.}]
This gives a straightforward formula for the derivative of     f ( x , y ( x )
)   {\displaystyle f(x,y(x))}  [{\displaystyle f(x,y(x))}] in terms of the
partial derivatives of     f   {\displaystyle f}  [f] and the derivative of
y ( x )   {\displaystyle y(x)}  [y(x)].
For example, suppose
         f ( x , y ) = x y .   {\displaystyle f(x,y)=xy.}  [{\displaystyle f
      (x,y)=xy.}]
The rate of change of f with respect to x is usually the partial derivative of
f with respect to x; in this case,
            &#x2202; f   &#x2202; x    = y .   {\displaystyle {\frac {\partial
      f}{\partial x}}=y.}  [{\displaystyle {\frac {\partial f}{\partial
      x}}=y.}]
However, if y depends on x, the partial derivative does not give the true rate
of change of f as x changes because the partial derivative assumes that y is
fixed. Suppose we are constrained to the line
         y = x .   {\displaystyle y=x.}  [{\displaystyle y=x.}]
Then
         f ( x , y ) = f ( x , x ) =  x  2   ,   {\displaystyle f(x,y)=f
      (x,x)=x^{2},}  [{\displaystyle f(x,y)=f(x,x)=x^{2},}]
and the total derivative of f with respect to x is
            d f   d x    = 2 x ,   {\displaystyle {\frac {df}{dx}}=2x,}  [
      {\displaystyle {\frac {df}{dx}}=2x,}]
which we see is not equal to the partial derivative     &#x2202; f  /  &#x2202;
x   {\displaystyle \partial f/\partial x}  [\partial f/\partial x]. Instead of
immediately substituting for y in terms of x, however, we can also use the
chain rule as above:
            d f   d x    =    &#x2202; f   &#x2202; x    +    &#x2202; f
      &#x2202; y       d y   d x    = y + x &#x22C5; 1 = x + y = 2 x .
      {\displaystyle {\frac {df}{dx}}={\frac {\partial f}{\partial x}}+{\frac
      {\partial f}{\partial y}}{\frac {dy}{dx}}=y+x\cdot 1=x+y=2x.}  [
      {\displaystyle {\frac {df}{dx}}={\frac {\partial f}{\partial x}}+{\frac
      {\partial f}{\partial y}}{\frac {dy}{dx}}=y+x\cdot 1=x+y=2x.}]
**** Example: Differentiation with indirect dependencies[edit] ****
While one can often perform substitutions to eliminate indirect dependencies,
the chain_rule provides for a more efficient and general technique. Suppose
L ( t ,  x  1   , &#x2026; ,  x  n   )   {\displaystyle L(t,x_{1},\dots ,x_
{n})}  [{\displaystyle L(t,x_{1},\dots ,x_{n})}] is a function of time     t
{\displaystyle t}  [t] and     n   {\displaystyle n}  [n] variables      x  i
{\displaystyle x_{i}}  [x_{i}] which themselves depend on time. Then, the time
derivative of     L   {\displaystyle L}  [L] is
            d L   d t    =   d  d t    L   (   t ,  x  1   ( t ) , &#x2026; ,
      x  n   ( t )   )   .   {\displaystyle {\frac {dL}{dt}}={\frac {d}{dt}}L
      {\bigl (}t,x_{1}(t),\ldots ,x_{n}(t){\bigr )}.}  [{\displaystyle {\frac
      {dL}{dt}}={\frac {d}{dt}}L{\bigl (}t,x_{1}(t),\ldots ,x_{n}(t){\bigr
      )}.}]
The chain rule expresses this derivative in terms of the partial derivatives of
L   {\displaystyle L}  [L] and the time derivatives of the functions      x  i
{\displaystyle x_{i}}  [x_{i}]:
            d L   d t    =    &#x2202; L   &#x2202; t    +  &#x2211;  i = 1   n
      &#x2202; L   &#x2202;  x  i         d  x  i     d t    =   (     &#x2202;
      &#x2202; t    +  &#x2211;  i = 1   n      d  x  i     d t      &#x2202;
      &#x2202;  x  i        )   ( L ) .   {\displaystyle {\frac {dL}{dt}}=
      {\frac {\partial L}{\partial t}}+\sum _{i=1}^{n}{\frac {\partial L}
      {\partial x_{i}}}{\frac {dx_{i}}{dt}}={\biggl (}{\frac {\partial }
      {\partial t}}+\sum _{i=1}^{n}{\frac {dx_{i}}{dt}}{\frac {\partial }
      {\partial x_{i}}}{\biggr )}(L).}  [{\displaystyle {\frac {dL}{dt}}={\frac
      {\partial L}{\partial t}}+\sum _{i=1}^{n}{\frac {\partial L}{\partial x_
      {i}}}{\frac {dx_{i}}{dt}}={\biggl (}{\frac {\partial }{\partial t}}+\sum
      _{i=1}^{n}{\frac {dx_{i}}{dt}}{\frac {\partial }{\partial x_{i}}}{\biggr
      )}(L).}]
This expression is often used in physics for a gauge_transformation of the
Lagrangian, as two Lagrangians that differ only by the total time derivative of
a function of time and the     n   {\displaystyle n}  [n] generalized
coordinates lead to the same equations of motion. An interesting example
concerns the resolution of causality concerning the WheelerâFeynman_time-
symmetric_theory. The operator in brackets (in the final expression above) is
also called the total derivative operator (with respect to     t
{\displaystyle t}  [t]).
For example, the total derivative of     f ( x ( t ) , y ( t ) )
{\displaystyle f(x(t),y(t))}  [{\displaystyle f(x(t),y(t))}] is
            d f   d t    =    &#x2202; f   &#x2202; x       d x   d t    +
      &#x2202; f   &#x2202; y       d y   d t    .   {\displaystyle {\frac {df}
      {dt}}={\partial f \over \partial x}{dx \over dt}+{\partial f \over
      \partial y}{dy \over dt}.}  [{\displaystyle {\frac {df}{dt}}={\partial f
      \over \partial x}{dx \over dt}+{\partial f \over \partial y}{dy \over
      dt}.}]
Here there is no     &#x2202; f  /  &#x2202; t   {\displaystyle \partial f/
\partial t}  [{\displaystyle \partial f/\partial t}] term since     f
{\displaystyle f}  [f] itself does not depend on the independent variable     t
{\displaystyle t}  [t] directly.
***** Total differential equation[edit] *****
Main article: Total_differential_equation
A total differential equation is a differential_equation expressed in terms of
total derivatives. Since the exterior_derivative is coordinate-free, in a sense
that can be given a technical meaning, such equations are intrinsic and
geometric.
***** Application to equation systems[edit] *****
In economics, it is common for the total derivative to arise in the context of
a system of equations.[1]:pp. 217â220 For example, a simple supply-demand
system might specify the quantity q of a product demanded as a function D of
its price p and consumers' income I, the latter being an exogenous_variable,
and might specify the quantity supplied by producers as a function S of its
price and two exogenous resource cost variables r and w. The resulting system
of equations
         q = D ( p , I ) ,   {\displaystyle q=D(p,I),}  [q=D(p,I),]
         q = S ( p , r , w ) ,   {\displaystyle q=S(p,r,w),}  [q=S(p,r,w),]
determines the market equilibrium values of the variables p and q. The total
derivative     d p  /  d r   {\displaystyle dp/dr}  [{\displaystyle dp/dr}] of
p with respect to r, for example, gives the sign and magnitude of the reaction
of the market price to the exogenous variable r. In the indicated system, there
are a total of six possible total derivatives, also known in this context as
comparative_static_derivatives: dp / dr, dp / dw, dp / dI, dq / dr, dq / dw,
and dq / dI. The total derivatives are found by totally differentiating the
system of equations, dividing through by, say dr, treating dq / dr and dp / dr
as the unknowns, setting dI = dw = 0, and solving the two totally
differentiated equations simultaneously, typically by using Cramer's_rule.
***** References[edit] *****
   1. ^ a bChiang,_Alpha_C. (1984). Fundamental Methods of Mathematical
      Economics (Third ed.). McGraw-Hill. ISBN 0-07-010813-7.
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
   3. ^Abraham,_Ralph; Marsden,_J._E.; Ratiu,_Tudor (2012). Manifolds,_Tensor
      Analysis,_and_Applications. Springer Science & Business Media. p. 78.
    * A. D. Polyanin and V. F. Zaitsev, Handbook of Exact Solutions for
      Ordinary Differential Equations (2nd edition), Chapman & Hall/CRC Press,
      Boca Raton, 2003.
ISBN 1-58488-297-2
From thesaurus.maths.org total_derivative
***** External links[edit] *****
    * Weisstein,_Eric_W. "Total_Derivative". MathWorld.
http://www.sv.rkriz.net/classes/ESM4714/methods/df2D.html

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Total_derivative&oldid=903158589"
Categories:
    * Multivariable_calculus
    * Differential_calculus
    * Differential_operators
    * Lagrangian_mechanics
    * Mathematical_analysis
Hidden categories:
    * Articles_lacking_in-text_citations_from_July_2013
    * All_articles_lacking_in-text_citations
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
    * Deutsch
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 23 June 2019, at 23:51 (UTC).
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
