The following text has been accessed from https://en.wikipedia.org/wiki/Partial_derivative at Fri Aug 9 01:06:36 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Partial derivative ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
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
    * Partial derivative
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
In mathematics, a partial derivative of a function_of_several_variables is its
derivative with respect to one of those variables, with the others held
constant (as opposed to the total_derivative, in which all variables are
allowed to vary). Partial derivatives are used in vector_calculus and
differential_geometry.
The partial derivative of a function     f ( x , y , &#x2026; )
{\displaystyle f(x,y,\dots )}  [{\displaystyle f(x,y,\dots )}] with respect to
the variable     x   {\displaystyle x}  [x] is variously denoted by
          f  x  &#x2032;  ,  f  x   ,  &#x2202;  x   f , &#xA0;  D  x   f ,  D
      1   f ,   &#x2202;  &#x2202; x    f ,  &#xA0;or&#xA0;     &#x2202; f
      &#x2202; x    .   {\displaystyle f'_{x},f_{x},\partial _{x}f,\ D_{x}f,D_
      {1}f,{\frac {\partial }{\partial x}}f,{\text{ or }}{\frac {\partial f}
      {\partial x}}.}  [{\displaystyle f'_{x},f_{x},\partial _{x}f,\ D_{x}f,D_
      {1}f,{\frac {\partial }{\partial x}}f,{\text{ or }}{\frac {\partial f}
      {\partial x}}.}]
Sometimes, for     z = f ( x , y , &#x2026; ) ,   {\displaystyle z=f(x,y,\ldots
),}  [{\displaystyle z=f(x,y,\ldots ),}] the partial derivative of     z
{\displaystyle z}  [z] with respect to     x   {\displaystyle x}  [x] is
denoted as         &#x2202; z   &#x2202; x     .   {\displaystyle {\tfrac
{\partial z}{\partial x}}.}  [{\displaystyle {\tfrac {\partial z}{\partial
x}}.}] Since a partial derivative generally has the same arguments as the
original function, its functional dependence is sometimes explicitly signified
by the notation, such as in:
          f  x   ( x , y , &#x2026; ) ,    &#x2202; f   &#x2202; x    ( x , y ,
      &#x2026; ) .   {\displaystyle f_{x}(x,y,\ldots ),{\frac {\partial f}
      {\partial x}}(x,y,\ldots ).}  [{\displaystyle f_{x}(x,y,\ldots ),{\frac
      {\partial f}{\partial x}}(x,y,\ldots ).}]
The symbol used to denote partial derivatives is â. One of the first known
uses of this symbol in mathematics is by Marquis_de_Condorcet from 1770, who
used it for partial differences. The modern partial derivative notation was
created by Adrien-Marie_Legendre (1786), though he later abandoned it; Carl
Gustav_Jacob_Jacobi reintroduced the symbol again in 1841.[1]
⁰
***** Contents *****
    * 1_Introduction
    * 2_Definition
          o 2.1_Basic_definition
          o 2.2_Formal_definition
    * 3_Examples
          o 3.1_Geometry
          o 3.2_Optimization
          o 3.3_Thermodynamics_and_mathematical_physics
          o 3.4_Image_resizing
          o 3.5_Economics
    * 4_Notation
    * 5_Antiderivative_analogue
    * 6_Higher_order_partial_derivatives
    * 7_See_also
    * 8_Notes
    * 9_References
    * 10_External_links
***** Introduction[edit] *****
Suppose that f is a function of more than one variable. For instance,
         z = f ( x , y ) =  x  2   + x y +  y  2   .   {\displaystyle z=f
      (x,y)=x^{2}+xy+y^{2}.}  [{\displaystyle z=f(x,y)=x^{2}+xy+y^{2}.}]
A graph of z = x2 + xy + y2. For the partial derivative at (1, 1) that leaves y
constant, the corresponding tangent line is parallel to the xz-plane.
A slice of the graph above showing the function in the xz-plane at y = 1. Note
that the two axes are shown here with different scales. The slope of the
tangent line is 3.
The graph of this function defines a surface in Euclidean_space. To every point
on this surface, there are an infinite number of tangent_lines. Partial
differentiation is the act of choosing one of these lines and finding its
slope. Usually, the lines of most interest are those that are parallel to the
x z   {\displaystyle xz}  [xz]-plane, and those that are parallel to the yz-
plane (which result from holding either y or x constant, respectively).
To find the slope of the line tangent to the function at     P ( 1 , 1 )
{\displaystyle P(1,1)}  [{\displaystyle P(1,1)}] and parallel to the     x z
{\displaystyle xz}  [xz]-plane, we treat     y   {\displaystyle y}  [y] as a
constant. The graph and this plane are shown on the right. Below, we see how
the function looks on the plane     y = 1   {\displaystyle y=1}  [y=1] . By
finding the derivative of the equation while assuming that     y
{\displaystyle y}  [y] is a constant, we find that the slope of    f
{\displaystyle f}  [f] at the point     ( x , y )   {\displaystyle (x,y)}  [
(x,y)] is:
            &#x2202; z   &#x2202; x    = 2 x + y .   {\displaystyle {\frac
      {\partial z}{\partial x}}=2x+y.}  [{\displaystyle {\frac {\partial z}
      {\partial x}}=2x+y.}]
So at     ( 1 , 1 )   {\displaystyle (1,1)}  [(1,1)], by substitution, the
slope is 3. Therefore,
            &#x2202; z   &#x2202; x    = 3   {\displaystyle {\frac {\partial z}
      {\partial x}}=3}  [\frac{\partial z}{\partial x} = 3]
at the point     ( 1 , 1 )   {\displaystyle (1,1)}  [(1,1)]. That is, the
partial derivative of     z   {\displaystyle z}  [z] with respect to     x
{\displaystyle x}  [x] at     ( 1 , 1 )   {\displaystyle (1,1)}  [(1,1)] is 3,
as shown in the graph.
***** Definition[edit] *****
**** Basic definition[edit] ****
The function f can be reinterpreted as a family of functions of one variable
indexed by the other variables:
         f ( x , y ) =  f  y   ( x ) =  x  2   + x y +  y  2   .
      {\displaystyle f(x,y)=f_{y}(x)=x^{2}+xy+y^{2}.}  [{\displaystyle f
      (x,y)=f_{y}(x)=x^{2}+xy+y^{2}.}]
In other words, every value of y defines a function, denoted fy , which is a
function of one variable x.[a] That is,
          f  y   ( x ) =  x  2   + x y +  y  2   .   {\displaystyle f_{y}(x)=x^
      {2}+xy+y^{2}.}  [{\displaystyle f_{y}(x)=x^{2}+xy+y^{2}.}]
Note that in this section the subscript notation fy denotes a function
contingent on a fixed value of y, and not a partial derivative.
Once a value of y is chosen, say a, then f(x,y) determines a function fa which
traces a curve x2 + ax + a2 on the     x z   {\displaystyle xz}  [xz]-plane:
          f  a   ( x ) =  x  2   + a x +  a  2   .   {\displaystyle f_{a}(x)=x^
      {2}+ax+a^{2}.}  [{\displaystyle f_{a}(x)=x^{2}+ax+a^{2}.}]
In this expression, a is a constant, not a variable, so fa is a function of
only one real variable, that being x. Consequently, the definition of the
derivative for a function of one variable applies:
          f  a  &#x2032;  ( x ) = 2 x + a .   {\displaystyle f_{a}'(x)=2x+a.}
      [{\displaystyle f_{a}'(x)=2x+a.}]
The above procedure can be performed for any choice of a. Assembling the
derivatives together into a function gives a function which describes the
variation of f in the x direction:
            &#x2202; f   &#x2202; x    ( x , y ) = 2 x + y .   {\displaystyle
      {\frac {\partial f}{\partial x}}(x,y)=2x+y.}  [{\displaystyle {\frac
      {\partial f}{\partial x}}(x,y)=2x+y.}]
This is the partial derivative of f with respect to x. Here â is a rounded d
called the partial derivative symbol. To distinguish it from the letter d, â
is sometimes pronounced "tho" or "partial".
In general, the partial derivative of an n-ary function f(x1, ..., xn) in the
direction xi at the point (a1, ..., an) is defined to be:
            &#x2202; f   &#x2202;  x  i      (  a  1   , &#x2026; ,  a  n   ) =
      lim  h &#x2192; 0      f (  a  1   , &#x2026; ,  a  i   + h , &#x2026; ,
      a  n   ) &#x2212; f (  a  1   , &#x2026; ,  a  i   , &#x2026; ,  a  n   )
      h   .   {\displaystyle {\frac {\partial f}{\partial x_{i}}}(a_{1},\ldots
      ,a_{n})=\lim _{h\to 0}{\frac {f(a_{1},\ldots ,a_{i}+h,\ldots ,a_{n})-f(a_
      {1},\ldots ,a_{i},\dots ,a_{n})}{h}}.}  [{\displaystyle {\frac {\partial
      f}{\partial x_{i}}}(a_{1},\ldots ,a_{n})=\lim _{h\to 0}{\frac {f(a_
      {1},\ldots ,a_{i}+h,\ldots ,a_{n})-f(a_{1},\ldots ,a_{i},\dots ,a_{n})}
      {h}}.}]
In the above difference quotient, all the variables except xi are held fixed.
That choice of fixed values determines a function of one variable
          f   a  1   , &#x2026; ,  a  i &#x2212; 1   ,  a  i + 1   , &#x2026; ,
      a  n     (  x  i   ) = f (  a  1   , &#x2026; ,  a  i &#x2212; 1   ,  x
      i   ,  a  i + 1   , &#x2026; ,  a  n   ) ,   {\displaystyle f_{a_
      {1},\ldots ,a_{i-1},a_{i+1},\ldots ,a_{n}}(x_{i})=f(a_{1},\ldots ,a_{i-
      1},x_{i},a_{i+1},\ldots ,a_{n}),}  [f_{a_{1},\ldots ,a_{i-1},a_
      {i+1},\ldots ,a_{n}}(x_{i})=f(a_{1},\ldots ,a_{i-1},x_{i},a_{i+1},\ldots
      ,a_{n}),]
and by definition,
            d  f   a  1   , &#x2026; ,  a  i &#x2212; 1   ,  a  i + 1   ,
      &#x2026; ,  a  n       d  x  i      (  a  i   ) =    &#x2202; f
      &#x2202;  x  i      (  a  1   , &#x2026; ,  a  n   ) .   {\displaystyle
      {\frac {df_{a_{1},\ldots ,a_{i-1},a_{i+1},\ldots ,a_{n}}}{dx_{i}}}(a_
      {i})={\frac {\partial f}{\partial x_{i}}}(a_{1},\ldots ,a_{n}).}  [\frac
      {df_{a_1,\ldots,a_{i-1},a_{i+1},\ldots,a_n}}{dx_i}(a_i) = \frac{\partial
      f}{\partial x_i}(a_1,\ldots,a_n).]
In other words, the different choices of a index a family of one-variable
functions just as in the example above. This expression also shows that the
computation of partial derivatives reduces to the computation of one-variable
derivatives.
An important example of a function of several variables is the case of a
scalar-valued_function f(x1, ..., xn) on a domain in Euclidean space       R
n     {\displaystyle \mathbb {R} ^{n}}  [\mathbb {R} ^{n}] (e.g., on       R
2     {\displaystyle \mathbb {R} ^{2}}  [\R^2] or       R   3
{\displaystyle \mathbb {R} ^{3}}  [\mathbb{R} ^{3}]). In this case f has a
partial derivative âf/âxj with respect to each variable xj. At the point a,
these partial derivatives define the vector
         &#x2207; f ( a ) =  (     &#x2202; f   &#x2202;  x  1      ( a ) ,
      &#x2026; ,    &#x2202; f   &#x2202;  x  n      ( a )  )  .
      {\displaystyle \nabla f(a)=\left({\frac {\partial f}{\partial x_{1}}}
      (a),\ldots ,{\frac {\partial f}{\partial x_{n}}}(a)\right).}  [\nabla f
      (a)=\left({\frac {\partial f}{\partial x_{1}}}(a),\ldots ,{\frac
      {\partial f}{\partial x_{n}}}(a)\right).]
This vector is called the gradient of f at a. If f is differentiable at every
point in some domain, then the gradient is a vector-valued function âf which
takes the point a to the vector âf(a). Consequently, the gradient produces a
vector_field.
A common abuse_of_notation is to define the del_operator (â) as follows in
three-dimensional Euclidean_space       R   3     {\displaystyle \mathbb {R} ^
{3}}  [\mathbb{R} ^{3}] with unit_vectors         i  &#x005E;    ,     j
&#x005E;    ,     k  &#x005E;      {\displaystyle {\hat {\mathbf {i} }},{\hat
{\mathbf {j} }},{\hat {\mathbf {k} }}}  [{\hat  {{\mathbf  {i}}}},{\hat  {
{\mathbf  {j}}}},{\hat  {{\mathbf  {k}}}}]:
         &#x2207; =  [   &#x2202;  &#x2202; x    ]      i  &#x005E;    +
      [   &#x2202;  &#x2202; y    ]      j  &#x005E;    +  [   &#x2202;
      &#x2202; z    ]      k  &#x005E;      {\displaystyle \nabla =\left[{\frac
      {\partial }{\partial x}}\right]{\hat {\mathbf {i} }}+\left[{\frac
      {\partial }{\partial y}}\right]{\hat {\mathbf {j} }}+\left[{\frac
      {\partial }{\partial z}}\right]{\hat {\mathbf {k} }}}  [{\displaystyle
      \nabla =\left[{\frac {\partial }{\partial x}}\right]{\hat {\mathbf {i}
      }}+\left[{\frac {\partial }{\partial y}}\right]{\hat {\mathbf {j}
      }}+\left[{\frac {\partial }{\partial z}}\right]{\hat {\mathbf {k} }}}]
Or, more generally, for n-dimensional Euclidean space       R   n
{\displaystyle \mathbb {R} ^{n}}  [\mathbb {R} ^{n}] with coordinates      x  1
, &#x2026; ,  x  n     {\displaystyle x_{1},\ldots ,x_{n}}  [x_{1},\ldots ,x_
{n}] and unit vectors          e  &#x005E;     1   , &#x2026; ,      e
&#x005E;     n     {\displaystyle {\hat {\mathbf {e} }}_{1},\ldots ,{\hat
{\mathbf {e} }}_{n}}  [{\displaystyle {\hat {\mathbf {e} }}_{1},\ldots ,{\hat
{\mathbf {e} }}_{n}}]:
         &#x2207; =  &#x2211;  j = 1   n    [   &#x2202;  &#x2202;  x  j      ]
      e  &#x005E;     j   =  [   &#x2202;  &#x2202;  x  1      ]       e
      &#x005E;     1   +  [   &#x2202;  &#x2202;  x  2      ]       e  &#x005E;
      2   + &#x2026; +  [   &#x2202;  &#x2202;  x  n      ]       e  &#x005E;
      n     {\displaystyle \nabla =\sum _{j=1}^{n}\left[{\frac {\partial }
      {\partial x_{j}}}\right]{\hat {\mathbf {e} }}_{j}=\left[{\frac {\partial
      }{\partial x_{1}}}\right]{\hat {\mathbf {e} }}_{1}+\left[{\frac {\partial
      }{\partial x_{2}}}\right]{\hat {\mathbf {e} }}_{2}+\ldots +\left[{\frac
      {\partial }{\partial x_{n}}}\right]{\hat {\mathbf {e} }}_{n}}  [
      {\displaystyle \nabla =\sum _{j=1}^{n}\left[{\frac {\partial }{\partial
      x_{j}}}\right]{\hat {\mathbf {e} }}_{j}=\left[{\frac {\partial }{\partial
      x_{1}}}\right]{\hat {\mathbf {e} }}_{1}+\left[{\frac {\partial }{\partial
      x_{2}}}\right]{\hat {\mathbf {e} }}_{2}+\ldots +\left[{\frac {\partial }
      {\partial x_{n}}}\right]{\hat {\mathbf {e} }}_{n}}]
**** Formal definition[edit] ****
Like ordinary derivatives, the partial derivative is defined as a limit. Let U
be an open_subset of       R   n     {\displaystyle \mathbb {R} ^{n}}  [\mathbb
{R} ^{n}] and     f : U &#x2192;  R    {\displaystyle f:U\to \mathbb {R} }  [
{\displaystyle f:U\to \mathbb {R} }] a function. The partial derivative of f at
the point      a  = (  a  1   , &#x2026; ,  a  n   ) &#x2208; U
{\displaystyle \mathbf {a} =(a_{1},\ldots ,a_{n})\in U}  [{\displaystyle
\mathbf {a} =(a_{1},\ldots ,a_{n})\in U}] with respect to the i-th variable xi
is defined as
           &#x2202;  &#x2202;  x  i      f (  a  ) =  lim  h &#x2192; 0      f
      (  a  1   , &#x2026; ,  a  i &#x2212; 1   ,  a  i   + h ,  a  i + 1   ,
      &#x2026; ,  a  n   ) &#x2212; f (  a  1   , &#x2026; ,  a  i   , &#x2026;
      ,  a  n   )  h     {\displaystyle {\frac {\partial }{\partial x_{i}}}f
      (\mathbf {a} )=\lim _{h\to 0}{\frac {f(a_{1},\ldots ,a_{i-1},a_{i}+h,a_
      {i+1},\ldots ,a_{n})-f(a_{1},\ldots ,a_{i},\dots ,a_{n})}{h}}}  [
      {\displaystyle {\frac {\partial }{\partial x_{i}}}f(\mathbf {a} )=\lim _
      {h\to 0}{\frac {f(a_{1},\ldots ,a_{i-1},a_{i}+h,a_{i+1},\ldots ,a_{n})-f
      (a_{1},\ldots ,a_{i},\dots ,a_{n})}{h}}}]
Even if all partial derivatives âf/âxi(a) exist at a given point a, the
function need not be continuous there. However, if all partial derivatives
exist in a neighborhood of a and are continuous there, then f is totally
differentiable in that neighborhood and the total derivative is continuous. In
this case, it is said that f is a C1 function. This can be used to generalize
for vector valued functions,     f : U &#x2192;   R   m   ,   {\displaystyle f:
U\to \mathbb {R} ^{m},}  [{\displaystyle f:U\to \mathbb {R} ^{m},}] by
carefully using a componentwise argument.
The partial derivative        &#x2202; f   &#x2202; x      {\displaystyle
{\frac {\partial f}{\partial x}}}  [\frac{\partial f}{\partial x}] can be seen
as another function defined on U and can again be partially differentiated. If
all mixed second order partial derivatives are continuous at a point (or on a
set), f is termed a C2 function at that point (or on that set); in this case,
the partial derivatives can be exchanged by Clairaut's_theorem:
             &#x2202;  2   f   &#x2202;  x  i   &#x2202;  x  j      =
      &#x2202;  2   f   &#x2202;  x  j   &#x2202;  x  i      .   {\displaystyle
      {\frac {\partial ^{2}f}{\partial x_{i}\partial x_{j}}}={\frac {\partial ^
      {2}f}{\partial x_{j}\partial x_{i}}}.}  [{\displaystyle {\frac {\partial
      ^{2}f}{\partial x_{i}\partial x_{j}}}={\frac {\partial ^{2}f}{\partial x_
      {j}\partial x_{i}}}.}]
***** Examples[edit] *****
**** Geometry[edit] ****
The volume of a cone depends on height and radius
The volume V of a cone depends on the cone's height h and its radius r
according to the formula
         V ( r , h ) =    &#x03C0;  r  2   h  3   .   {\displaystyle V(r,h)=
      {\frac {\pi r^{2}h}{3}}.}  [V(r, h) = \frac{\pi r^2 h}{3}.]
The partial derivative of V with respect to r is
            &#x2202; V   &#x2202; r    =    2 &#x03C0; r h  3   ,
      {\displaystyle {\frac {\partial V}{\partial r}}={\frac {2\pi rh}{3}},}
      [\frac{ \partial V}{\partial r} = \frac{ 2 \pi r h}{3},]
which represents the rate with which a cone's volume changes if its radius is
varied and its height is kept constant. The partial derivative with respect to
h   {\displaystyle h}  [h] equals        &#x03C0;  r  2    3   ,
{\displaystyle {\frac {\pi r^{2}}{3}},}  [{\displaystyle {\frac {\pi r^{2}}
{3}},}] which represents the rate with which the volume changes if its height
is varied and its radius is kept constant.
By contrast, the total_derivative of V with respect to r and h are respectively
            d V   d r    =      2 &#x03C0; r h  3  &#x23DE;      &#x2202; V
      &#x2202; r     +      &#x03C0;  r  2    3  &#x23DE;      &#x2202; V
      &#x2202; h        d h   d r      {\displaystyle {\frac {dV}
      {dr}}=\overbrace {\frac {2\pi rh}{3}} ^{\frac {\partial V}{\partial
      r}}+\overbrace {\frac {\pi r^{2}}{3}} ^{\frac {\partial V}{\partial h}}
      {\frac {dh}{dr}}}  [{\displaystyle {\frac {dV}{dr}}=\overbrace {\frac
      {2\pi rh}{3}} ^{\frac {\partial V}{\partial r}}+\overbrace {\frac {\pi r^
      {2}}{3}} ^{\frac {\partial V}{\partial h}}{\frac {dh}{dr}}}]
and
            d V   d h    =      &#x03C0;  r  2    3  &#x23DE;      &#x2202; V
      &#x2202; h     +      2 &#x03C0; r h  3  &#x23DE;      &#x2202; V
      &#x2202; r        d r   d h      {\displaystyle {\frac {dV}
      {dh}}=\overbrace {\frac {\pi r^{2}}{3}} ^{\frac {\partial V}{\partial
      h}}+\overbrace {\frac {2\pi rh}{3}} ^{\frac {\partial V}{\partial r}}
      {\frac {dr}{dh}}}  [{\displaystyle {\frac {dV}{dh}}=\overbrace {\frac
      {\pi r^{2}}{3}} ^{\frac {\partial V}{\partial h}}+\overbrace {\frac {2\pi
      rh}{3}} ^{\frac {\partial V}{\partial r}}{\frac {dr}{dh}}}]
The difference between the total and partial derivative is the elimination of
indirect dependencies between variables in partial derivatives.
If (for some arbitrary reason) the cone's proportions have to stay the same,
and the height and radius are in a fixed ratio k,
         k =   h r   =    d h   d r    .   {\displaystyle k={\frac {h}{r}}=
      {\frac {dh}{dr}}.}  [{\displaystyle k={\frac {h}{r}}={\frac {dh}{dr}}.}]
This gives the total derivative with respect to r:
            d V   d r    =    2 &#x03C0; r h  3   +    &#x03C0;  r  2    3   k
      {\displaystyle {\frac {dV}{dr}}={\frac {2\pi rh}{3}}+{\frac {\pi r^{2}}
      {3}}k}  [{\displaystyle {\frac {dV}{dr}}={\frac {2\pi rh}{3}}+{\frac {\pi
      r^{2}}{3}}k}]
which simplifies to:
            d V   d r    = k &#x03C0;  r  2     {\displaystyle {\frac {dV}
      {dr}}=k\pi r^{2}}  [{\displaystyle {\frac {dV}{dr}}=k\pi r^{2}}]
Similarly, the total derivative with respect to h is:
            d V   d h    = &#x03C0;  r  2     {\displaystyle {\frac {dV}
      {dh}}=\pi r^{2}}  [{\displaystyle {\frac {dV}{dh}}=\pi r^{2}}]
The total derivative with respect to both r and h of the volume intended as
scalar function of these two variables is given by the gradient vector
         &#x2207; V =  (     &#x2202; V   &#x2202; r    ,    &#x2202; V
      &#x2202; h     )  =  (    2 3   &#x03C0; r h ,   1 3   &#x03C0;  r  2
      )    {\displaystyle \nabla V=\left({\frac {\partial V}{\partial r}},
      {\frac {\partial V}{\partial h}}\right)=\left({\frac {2}{3}}\pi rh,{\frac
      {1}{3}}\pi r^{2}\right)}  [\nabla V = \left(\frac{\partial V}{\partial
      r},\frac{\partial V}{\partial h}\right) = \left(\frac{2}{3}\pi rh, \frac
      {1}{3}\pi r^2\right)].
**** Optimization[edit] ****
Partial derivatives appear in any calculus-based optimization problem with more
than one choice variable. For example, in economics a firm may wish to maximize
profit Ï(x, y) with respect to the choice of the quantities x and y of two
different types of output. The first_order_conditions for this optimization are
Ïx = 0 = Ïy. Since both partial derivatives Ïx and Ïy will generally
themselves be functions of both arguments x and y, these two first order
conditions form a system_of_two_equations_in_two_unknowns.
**** Thermodynamics and mathematical physics[edit] ****
Partial derivatives appear in thermodynamic equations like Gibbs-Duhem_equation
as well in other equations from mathematical_physics. Here the variables being
held constant in partial derivatives can be ratio of simple variables like mole
fractions xi in the following example involving the Gibbs energies in a ternary
mixture system:
             G  2   &#x00AF;    = G + ( 1 &#x2212;  x  2   )   (    &#x2202; G
      &#x2202;  x  2      )     x  1    x  3        {\displaystyle {\bar {G_
      {2}}}=G+(1-x_{2})\left({\frac {\partial G}{\partial x_{2}}}\right)_{\frac
      {x_{1}}{x_{3}}}}  [{\displaystyle {\bar {G_{2}}}=G+(1-x_{2})\left({\frac
      {\partial G}{\partial x_{2}}}\right)_{\frac {x_{1}}{x_{3}}}}]
Express mole_fractions of a component as functions of other components mole
fraction and binary mole ratios:
          x  1   =    1 &#x2212;  x  2     1 +    x  3    x  1
      {\displaystyle x_{1}={\frac {1-x_{2}}{1+{\frac {x_{3}}{x_{1}}}}}}  [
      {\displaystyle x_{1}={\frac {1-x_{2}}{1+{\frac {x_{3}}{x_{1}}}}}}]
          x  3   =    1 &#x2212;  x  2     1 +    x  1    x  3
      {\displaystyle x_{3}={\frac {1-x_{2}}{1+{\frac {x_{1}}{x_{3}}}}}}  [
      {\displaystyle x_{3}={\frac {1-x_{2}}{1+{\frac {x_{1}}{x_{3}}}}}}]
Differential quotients can be formed at constant ratios like those above:
           (    &#x2202;  x  1     &#x2202;  x  2      )     x  1    x  3
      = &#x2212;    x  1    1 &#x2212;  x  2        {\displaystyle \left({\frac
      {\partial x_{1}}{\partial x_{2}}}\right)_{\frac {x_{1}}{x_{3}}}=-{\frac
      {x_{1}}{1-x_{2}}}}  [{\displaystyle \left({\frac {\partial x_{1}}
      {\partial x_{2}}}\right)_{\frac {x_{1}}{x_{3}}}=-{\frac {x_{1}}{1-x_
      {2}}}}]
           (    &#x2202;  x  3     &#x2202;  x  2      )     x  1    x  3
      = &#x2212;    x  3    1 &#x2212;  x  2        {\displaystyle \left({\frac
      {\partial x_{3}}{\partial x_{2}}}\right)_{\frac {x_{1}}{x_{3}}}=-{\frac
      {x_{3}}{1-x_{2}}}}  [{\displaystyle \left({\frac {\partial x_{3}}
      {\partial x_{2}}}\right)_{\frac {x_{1}}{x_{3}}}=-{\frac {x_{3}}{1-x_
      {2}}}}]
Ratios X, Y, Z of mole fractions can be written for ternary and multicomponent
systems:
         X =    x  3     x  1   +  x  3        {\displaystyle X={\frac {x_{3}}
      {x_{1}+x_{3}}}}  [{\displaystyle X={\frac {x_{3}}{x_{1}+x_{3}}}}]
         Y =    x  3     x  2   +  x  3        {\displaystyle Y={\frac {x_{3}}
      {x_{2}+x_{3}}}}  [{\displaystyle Y={\frac {x_{3}}{x_{2}+x_{3}}}}]
         Z =    x  2     x  1   +  x  2        {\displaystyle Z={\frac {x_{2}}
      {x_{1}+x_{2}}}}  [{\displaystyle Z={\frac {x_{2}}{x_{1}+x_{2}}}}]
which can be used for solving partial_differential_equations like:
           (    &#x2202;  &#x03BC;  2     &#x2202;  n  1      )    n  2   ,  n
      3     =   (    &#x2202;  &#x03BC;  1     &#x2202;  n  2      )    n  1
      ,  n  3       {\displaystyle \left({\frac {\partial \mu _{2}}{\partial n_
      {1}}}\right)_{n_{2},n_{3}}=\left({\frac {\partial \mu _{1}}{\partial n_
      {2}}}\right)_{n_{1},n_{3}}}  [{\displaystyle \left({\frac {\partial \mu _
      {2}}{\partial n_{1}}}\right)_{n_{2},n_{3}}=\left({\frac {\partial \mu _
      {1}}{\partial n_{2}}}\right)_{n_{1},n_{3}}}]
This equality can be rearranged to have differential quotient of mole fractions
on one side.
**** Image resizing[edit] ****
Partial derivatives are key to target-aware image resizing algorithms. Widely
known as seam_carving, these algorithms require each pixel in an image to be
assigned a numerical 'energy' to describe their dissimilarity against
orthogonal adjacent pixels. The algorithm then progressively removes rows or
columns with the lowest energy. The formula established to determine a pixel's
energy (magnitude of gradient at a pixel) depends heavily on the constructs of
partial derivatives.
**** Economics[edit] ****
Partial derivatives play a prominent role in economics, in which most functions
describing economic behaviour posit that the behaviour depends on more than one
variable. For example, a societal consumption_function may describe the amount
spent on consumer goods as depending on both income and wealth; the marginal
propensity_to_consume is then the partial derivative of the consumption
function with respect to income.
***** Notation[edit] *****
Further information: â
For the following examples, let     f   {\displaystyle f}  [f] be a function in
x , y   {\displaystyle x,y}  [x,y] and     z   {\displaystyle z}  [z].
First-order partial derivatives:
            &#x2202; f   &#x2202; x    =  f  x   =  &#x2202;  x   f .
      {\displaystyle {\frac {\partial f}{\partial x}}=f_{x}=\partial _{x}f.}
      [\frac{ \partial f}{ \partial x} = f_x = \partial_x f.]
Second-order partial derivatives:
             &#x2202;  2   f   &#x2202;  x  2      =  f  x x   =  &#x2202;  x x
      f =  &#x2202;  x   2   f .   {\displaystyle {\frac {\partial ^{2}f}
      {\partial x^{2}}}=f_{xx}=\partial _{xx}f=\partial _{x}^{2}f.}  [
      {\displaystyle {\frac {\partial ^{2}f}{\partial x^{2}}}=f_{xx}=\partial _
      {xx}f=\partial _{x}^{2}f.}]
Second-order mixed_derivatives:
             &#x2202;  2   f   &#x2202; y  &#x2202; x    =   &#x2202;  &#x2202;
      y     (    &#x2202; f   &#x2202; x    )  = (  f  x    )  y   =  f  x y
      =  &#x2202;  y x   f =  &#x2202;  y    &#x2202;  x   f .   {\displaystyle
      {\frac {\partial ^{2}f}{\partial y\,\partial x}}={\frac {\partial }
      {\partial y}}\left({\frac {\partial f}{\partial x}}\right)=(f_{x})_{y}=f_
      {xy}=\partial _{yx}f=\partial _{y}\partial _{x}f.}  [{\displaystyle
      {\frac {\partial ^{2}f}{\partial y\,\partial x}}={\frac {\partial }
      {\partial y}}\left({\frac {\partial f}{\partial x}}\right)=(f_{x})_{y}=f_
      {xy}=\partial _{yx}f=\partial _{y}\partial _{x}f.}]
Higher-order partial and mixed derivatives:
             &#x2202;  i + j + k   f   &#x2202;  x  i   &#x2202;  y  j
      &#x2202;  z  k      =  f  ( i , j , k )   =  &#x2202;  x   i    &#x2202;
      y   j    &#x2202;  z   k   f .   {\displaystyle {\frac {\partial ^
      {i+j+k}f}{\partial x^{i}\partial y^{j}\partial z^{k}}}=f^{
      (i,j,k)}=\partial _{x}^{i}\partial _{y}^{j}\partial _{z}^{k}f.}  [
      {\displaystyle {\frac {\partial ^{i+j+k}f}{\partial x^{i}\partial y^
      {j}\partial z^{k}}}=f^{(i,j,k)}=\partial _{x}^{i}\partial _{y}^
      {j}\partial _{z}^{k}f.}]
When dealing with functions of multiple variables, some of these variables may
be related to each other, thus it may be necessary to specify explicitly which
variables are being held constant to avoid ambiguity. In fields such as
statistical_mechanics, the partial derivative of     f   {\displaystyle f}  [f]
with respect to     x   {\displaystyle x}  [x], holding     y   {\displaystyle
y}  [y] and     z   {\displaystyle z}  [z] constant, is often expressed as
           (    &#x2202; f   &#x2202; x    )   y , z   .   {\displaystyle \left
      ({\frac {\partial f}{\partial x}}\right)_{y,z}.}  [\left( \frac{\partial
      f}{\partial x} \right)_{y,z}.]
Conventionally, for clarity and simplicity of notation, the partial derivative
function and the value of the function at a specific point are conflated by
including the function arguments when the partial derivative symbol (Leibniz
notation) is used. Thus, an expression like
            &#x2202; f ( x , y , z )   &#x2202; x      {\displaystyle {\frac
      {\partial f(x,y,z)}{\partial x}}}  [{\frac  {\partial f(x,y,z)}{\partial
      x}}]
is used for the function, while
            &#x2202; f ( u , v , w )   &#x2202; u      {\displaystyle {\frac
      {\partial f(u,v,w)}{\partial u}}}  [{\displaystyle {\frac {\partial f
      (u,v,w)}{\partial u}}}]
might be used for the value of the function at the point     ( x , y , z ) =
( u , v , w )   {\displaystyle (x,y,z)=(u,v,w)}  [{\displaystyle (x,y,z)=
(u,v,w)}]. However, this convention breaks down when we want to evaluate the
partial derivative at a point like     ( x , y , z ) = ( 17 , u + v ,  v  2   )
{\displaystyle (x,y,z)=(17,u+v,v^{2})}  [{\displaystyle (x,y,z)=(17,u+v,v^
{2})}]. In such a case, evaluation of the function must be expressed in an
unwieldy manner as
            &#x2202; f ( x , y , z )   &#x2202; x    ( 17 , u + v ,  v  2   )
      {\displaystyle {\frac {\partial f(x,y,z)}{\partial x}}(17,u+v,v^{2})}  [
      {\displaystyle {\frac {\partial f(x,y,z)}{\partial x}}(17,u+v,v^{2})}]
or
               &#x2202; f ( x , y , z )   &#x2202; x    |   ( x , y , z ) =
      ( 17 , u + v ,  v  2   )     {\displaystyle \left.{\frac {\partial f
      (x,y,z)}{\partial x}}\right|_{(x,y,z)=(17,u+v,v^{2})}}  [{\displaystyle
      \left.{\frac {\partial f(x,y,z)}{\partial x}}\right|_{(x,y,z)=(17,u+v,v^
      {2})}}]
in order to use the Leibniz notation. Thus, in these cases, it may be
preferable to use the Euler differential operator notation with      D  i
{\displaystyle D_{i}}  [D_{i}] as the partial derivative symbol with respect to
the ith variable. For instance, one would write      D  1   f ( 17 , u + v ,  v
2   )   {\displaystyle D_{1}f(17,u+v,v^{2})}  [{\displaystyle D_{1}f(17,u+v,v^
{2})}] for the example described above, while the expression      D  1   f
{\displaystyle D_{1}f}  [{\displaystyle D_{1}f}] represents the partial
derivative function with respect to the 1st variable.[2]
For higher order partial derivatives, the partial derivative (function) of
D  i   f   {\displaystyle D_{i}f}  [{\displaystyle D_{i}f}] with respect to the
jth variable is denoted      D  j   (  D  i   f ) =  D  i , j   f
{\displaystyle D_{j}(D_{i}f)=D_{i,j}f}  [{\displaystyle D_{j}(D_{i}f)=D_
{i,j}f}]. That is,      D  j   &#x2218;  D  i   =  D  i , j     {\displaystyle
D_{j}\circ D_{i}=D_{i,j}}  [{\displaystyle D_{j}\circ D_{i}=D_{i,j}}], so that
the variables are listed in the order in which the derivatives are taken, and
thus, in reverse order of how the composition of operators is usually notated.
Of course, Clairaut's_theorem implies that      D  i , j   =  D  j , i
{\displaystyle D_{i,j}=D_{j,i}}  [{\displaystyle D_{i,j}=D_{j,i}}] as long as
comparatively mild regularity conditions on f are satisfied.
***** Antiderivative analogue[edit] *****
There is a concept for partial derivatives that is analogous to antiderivatives
for regular derivatives. Given a partial derivative, it allows for the partial
recovery of the original function.
Consider the example of
            &#x2202; z   &#x2202; x    = 2 x + y .   {\displaystyle {\frac
      {\partial z}{\partial x}}=2x+y.}  [{\displaystyle {\frac {\partial z}
      {\partial x}}=2x+y.}]
The "partial" integral can be taken with respect to x (treating y as constant,
in a similar manner to partial differentiation):
         z = &#x222B;    &#x2202; z   &#x2202; x     d x =  x  2   + x y + g
      ( y )   {\displaystyle z=\int {\frac {\partial z}{\partial x}}\,dx=x^
      {2}+xy+g(y)}  [z = \int \frac{\partial z}{\partial x} \,dx = x^2 + xy + g
      (y)]
Here, the "constant"_of_integration is no longer a constant, but instead a
function of all the variables of the original function except x. The reason for
this is that all the other variables are treated as constant when taking the
partial derivative, so any function which does not involve     x
{\displaystyle x}  [x] will disappear when taking the partial derivative, and
we have to account for this when we take the antiderivative. The most general
way to represent this is to have the "constant" represent an unknown function
of all the other variables.
Thus the set of functions      x  2   + x y + g ( y )   {\displaystyle x^
{2}+xy+g(y)}  [x^2 + xy + g(y)], where g is any one-argument function,
represents the entire set of functions in variables x,y that could have
produced the x-partial derivative     2 x + y   {\displaystyle 2x+y}  [2x + y].
If all the partial derivatives of a function are known (for example, with the
gradient), then the antiderivatives can be matched via the above process to
reconstruct the original function up to a constant. Unlike in the single-
variable case, however, not every set of functions can be the set of all
(first) partial derivatives of a single function. In other words, not every
vector field is conservative.
***** Higher order partial derivatives[edit] *****
Second and higher order partial derivatives are defined analogously to the
higher order derivatives of univariate functions. For the function     f ( x ,
y , . . . )   {\displaystyle f(x,y,...)}  [f(x, y, ...)] the "own" second
partial derivative with respect to x is simply the partial derivative of the
partial derivative (both with respect to x):[3]:316â318
             &#x2202;  2   f   &#x2202;  x  2      &#x2261; &#x2202;
      &#x2202; f  /  &#x2202; x   &#x2202; x    &#x2261;    &#x2202;  f  x
      &#x2202; x    &#x2261;  f  x x   .   {\displaystyle {\frac {\partial ^
      {2}f}{\partial x^{2}}}\equiv \partial {\frac {\partial f/\partial x}
      {\partial x}}\equiv {\frac {\partial f_{x}}{\partial x}}\equiv f_{xx}.}
      [{\displaystyle {\frac {\partial ^{2}f}{\partial x^{2}}}\equiv \partial
      {\frac {\partial f/\partial x}{\partial x}}\equiv {\frac {\partial f_{x}}
      {\partial x}}\equiv f_{xx}.}]
The cross partial derivative with respect to x and y is obtained by taking the
partial derivative of f with respect to x, and then taking the partial
derivative of the result with respect to y, to obtain
             &#x2202;  2   f   &#x2202; y  &#x2202; x    &#x2261; &#x2202;
      &#x2202; f  /  &#x2202; x   &#x2202; y    &#x2261;    &#x2202;  f  x
      &#x2202; y    &#x2261;  f  x y   .   {\displaystyle {\frac {\partial ^
      {2}f}{\partial y\,\partial x}}\equiv \partial {\frac {\partial f/\partial
      x}{\partial y}}\equiv {\frac {\partial f_{x}}{\partial y}}\equiv f_{xy}.}
      [\frac{{\partial ^2 f}}{{\partial y\, \partial x}} \equiv \partial \frac{
      {\partial f / \partial x}}{{\partial y}} \equiv \frac{{\partial f_x}}{
      {\partial y}} \equiv f_{{xy}}.]
Schwarz's_theorem states that if the second derivatives are continuous the
expression for the cross partial derivative is unaffected by which variable the
partial derivative is taken with respect to first and which is taken second.
That is,
             &#x2202;  2   f   &#x2202; x  &#x2202; y    =     &#x2202;  2   f
      &#x2202; y  &#x2202; x      {\displaystyle {\frac {\partial ^{2}f}
      {\partial x\,\partial y}}={\frac {\partial ^{2}f}{\partial y\,\partial
      x}}}  [\frac {{\partial ^2 f}}{{\partial x\, \partial y}} = \frac{
      {\partial ^2 f}}{{\partial y\, \partial x}}]
or equivalently      f  x y   =  f  y x   .   {\displaystyle f_{xy}=f_{yx}.}
[f_{{xy}}=f_{{yx}}.]
Own and cross partial derivatives appear in the Hessian_matrix which is used in
the second_order_conditions in optimization problems.
***** See also[edit] *****
    * d'Alembertian_operator
    * Chain_rule
    * Curl_(mathematics)
    * Directional_derivative
    * Divergence
    * Exterior_derivative
    * Jacobian_matrix_and_determinant
    * Laplacian
    * Multivariable_calculus
    * Symmetry_of_second_derivatives
    * Triple_product_rule, also known as the cyclic chain rule.
***** Notes[edit] *****
   1. ^ This can also be expressed as the adjointness between the product_space
      and function_space constructions.
***** References[edit] *****
   1. ^Miller, Jeff (2009-06-14). "Earliest_Uses_of_Symbols_of_Calculus".
      Earliest Uses of Various Mathematical Symbols. Retrieved 2009-02-20.
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
   3. ^Spivak, M. (1965). Calculus_on_Manifolds. New York: W. A. Benjamin, Inc.
      p. 44. ISBN 9780805390216.
   4. ^ Chiang,_Alpha_C. Fundamental Methods of Mathematical Economics, McGraw-
      Hill, third edition, 1984.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Partial_derivative",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Partial_Derivatives at MathWorld

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Partial_derivative&oldid=908260879"
Categories:
    * Multivariable_calculus
    * Differential_operators
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
    * Asturianu
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
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
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * LietuviÅ³
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 28 July 2019, at 15:31 (UTC).
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
