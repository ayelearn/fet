The following text has been accessed from https://en.wikipedia.org/wiki/Gradient at Thu Aug 8 23:41:48 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Gradient ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the gradient of a multivariate function. For direction
and steepness of a line on a graph, see Slope. For the slope of a road or other
physical feature, see Grade_(slope). For the similarly spelled unit of angle
also known as gon, see Gradian. For other uses, see Gradient_(disambiguation).
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (January 2018)(Learn_how_and
 when_to_remove_this_template_message)
Multi-variable generalization of the derivative of a function
In the above two images, the values of the function are represented in black
and white, black representing higher values, and its corresponding gradient is
represented by blue arrows.
In vector_calculus, the gradient is a multi-variable generalization of the
derivative.[1] Whereas the ordinary derivative of a function of a single
variable is a scalar-valued_function, the gradient of a function of several
variables is a vector-valued_function. Specifically, the gradient of a
differentiable_function     f   {\displaystyle f}  [f] of several_variables, at
a point     P   {\displaystyle P}  [P], is the vector whose components are the
partial_derivatives of     f   {\displaystyle f}  [f] at     P   {\displaystyle
P}  [P].[2][3][4][5][6][7][8][9][10]
Much as the derivative of a function of a single variable represents the slope
of the tangent to the graph of the function,[11] if at a point     P
{\displaystyle P}  [P], the gradient of a function of several variables is not
the zero vector, it has the direction of greatest increase of the function at
P   {\displaystyle P}  [P], and its magnitude is the rate of increase in that
direction.[12][13][14][15][16][17][18]
The magnitude and direction of the gradient vector are independent of the
particular coordinate_representation.[19][20]
The Jacobian is the generalization of the gradient for vector-valued functions
of several variables and differentiable_maps between Euclidean_spaces or, more
generally, manifolds.[21][22] A further generalization for a function between
Banach_spaces is the FrÃ©chet_derivative.
⁰
***** Contents *****
    * 1_Motivation
    * 2_Definition
          o 2.1_Cartesian_coordinates
          o 2.2_Cylindrical_and_spherical_coordinates
          o 2.3_General_coordinates
    * 3_Gradient_and_the_derivative_or_differential
          o 3.1_Linear_approximation_to_a_function
          o 3.2_Differential_or_(exterior)_derivative
          o 3.3_Gradient_as_a_derivative
                # 3.3.1_Linearity
                # 3.3.2_Product_rule
                # 3.3.3_Chain_rule
    * 4_Further_properties_and_applications
          o 4.1_Level_sets
          o 4.2_Conservative_vector_fields_and_the_gradient_theorem
    * 5_Generalizations
          o 5.1_Gradient_of_a_vector
          o 5.2_Riemannian_manifolds
    * 6_See_also
    * 7_Notes
    * 8_References
    * 9_Further_reading
    * 10_External_links
***** Motivation[edit] *****
Gradient of the 2D function f(x, y) = xeâ(x2 + y2) is plotted as blue arrows
over the pseudocolor plot of the function.
Consider a room where the temperature is given by a scalar_field, T, so at each
point (x, y, z) the temperature is T(x, y, z). (Assume that the temperature
does not change over time.) At each point in the room, the gradient of T at
that point will show the direction in which the temperature rises most quickly.
The magnitude of the gradient will determine how fast the temperature rises in
that direction.
Consider a surface whose height above sea level at point (x, y) is H(x, y). The
gradient of H at a point is a vector pointing in the direction of the steepest
slope or grade at that point. The steepness of the slope at that point is given
by the magnitude of the gradient vector.
The gradient can also be used to measure how a scalar field changes in other
directions, rather than just the direction of greatest change, by taking a dot
product. Suppose that the steepest slope on a hill is 40%. If a road goes
directly up the hill, then the steepest slope on the road will also be 40%. If,
instead, the road goes around the hill at an angle, then it will have a
shallower slope. For example, if the angle between the road and the uphill
direction, projected onto the horizontal plane, is 60Â°, then the steepest
slope along the road will be 20%, which is 40% times the cosine of 60Â°.
This observation can be mathematically stated as follows. If the hill height
function H is differentiable, then the gradient of H dotted with a unit_vector
gives the slope of the hill in the direction of the vector. More precisely,
when H is differentiable, the dot product of the gradient of H with a given
unit vector is equal to the directional_derivative of H in the direction of
that unit vector.
***** Definition[edit] *****
The gradient of the function f(x,y) = â(cos2x + cos2y)2 depicted as a
projected vector_field on the bottom plane.
The gradient (or gradient vector field) of a scalar function f(x1, x2, x3, ...,
xn) is denoted âf or ââf where â (the nabla_symbol) denotes the vector
differential_operator, del. The notation grad f is also commonly used for the
gradient. The gradient of f is defined as the unique vector field whose dot
product with any unit vector v at each point x is the directional derivative of
f along v. That is,
           (   &#x2207; f ( x )   )   &#x22C5;  v  =  D   v    f ( x ) .
      {\displaystyle {\big (}\nabla f(x){\big )}\cdot \mathbf {v} =D_{\mathbf
      {v} }f(x).}  [{\displaystyle {\big (}\nabla f(x){\big )}\cdot \mathbf {v}
      =D_{\mathbf {v} }f(x).}]
When a function also depends on a parameter such as time, the gradient often
refers simply to the vector of its spatial derivatives only (see Spatial
gradient).
**** Cartesian coordinates[edit] ****
In the three-dimensional Cartesian_coordinate_system with a Euclidean_metric,
the gradient, if it exists, is given by:
         &#x2207; f =    &#x2202; f   &#x2202; x     i  +    &#x2202; f
      &#x2202; y     j  +    &#x2202; f   &#x2202; z     k  ,   {\displaystyle
      \nabla f={\frac {\partial f}{\partial x}}\mathbf {i} +{\frac {\partial f}
      {\partial y}}\mathbf {j} +{\frac {\partial f}{\partial z}}\mathbf {k} ,}
      [{\displaystyle \nabla f={\frac {\partial f}{\partial x}}\mathbf {i} +
      {\frac {\partial f}{\partial y}}\mathbf {j} +{\frac {\partial f}{\partial
      z}}\mathbf {k} ,}]
where i, j, k are the standard unit vectors in the directions of the x, y and z
coordinates, respectively. For example, the gradient of the function
         f ( x , y , z ) = 2 x + 3  y  2   &#x2212; sin &#x2061; ( z )
      {\displaystyle f(x,y,z)=2x+3y^{2}-\sin(z)}  [{\displaystyle f
      (x,y,z)=2x+3y^{2}-\sin(z)}]
is
         &#x2207; f = 2  i  + 6 y  j  &#x2212; cos &#x2061; ( z )  k  .
      {\displaystyle \nabla f=2\mathbf {i} +6y\mathbf {j} -\cos(z)\mathbf {k}
      .}  [{\displaystyle \nabla f=2\mathbf {i} +6y\mathbf {j} -\cos(z)\mathbf
      {k} .}]
In some applications it is customary to represent the gradient as a row_vector
or column_vector of its components in a rectangular coordinate system.
**** Cylindrical and spherical coordinates[edit] ****
Main article: Del_in_cylindrical_and_spherical_coordinates
In cylindrical_coordinates with a Euclidean metric, the gradient is given by:
[23]
         &#x2207; f ( &#x03C1; , &#x03C6; , z ) =    &#x2202; f   &#x2202;
      &#x03C1;      e   &#x03C1;   +   1 &#x03C1;      &#x2202; f   &#x2202;
      &#x03C6;      e   &#x03C6;   +    &#x2202; f   &#x2202; z      e   z   ,
      {\displaystyle \nabla f(\rho ,\varphi ,z)={\frac {\partial f}{\partial
      \rho }}\mathbf {e} _{\rho }+{\frac {1}{\rho }}{\frac {\partial f}
      {\partial \varphi }}\mathbf {e} _{\varphi }+{\frac {\partial f}{\partial
      z}}\mathbf {e} _{z},}  [{\displaystyle \nabla f(\rho ,\varphi ,z)={\frac
      {\partial f}{\partial \rho }}\mathbf {e} _{\rho }+{\frac {1}{\rho }}
      {\frac {\partial f}{\partial \varphi }}\mathbf {e} _{\varphi }+{\frac
      {\partial f}{\partial z}}\mathbf {e} _{z},}]
where Ï is the axial distance, Ï is the azimuthal or azimuth angle, z is the
axial coordinate, and eÏ, eÏ and ez are unit vectors pointing along the
coordinate directions.
In spherical_coordinates, the gradient is given by:[23]
         &#x2207; f ( r , &#x03B8; , &#x03C6; ) =    &#x2202; f   &#x2202; r
      e   r   +   1 r      &#x2202; f   &#x2202; &#x03B8;      e   &#x03B8;   +
      1  r sin &#x2061; &#x03B8;       &#x2202; f   &#x2202; &#x03C6;      e
      &#x03C6;   ,   {\displaystyle \nabla f(r,\theta ,\varphi )={\frac
      {\partial f}{\partial r}}\mathbf {e} _{r}+{\frac {1}{r}}{\frac {\partial
      f}{\partial \theta }}\mathbf {e} _{\theta }+{\frac {1}{r\sin \theta }}
      {\frac {\partial f}{\partial \varphi }}\mathbf {e} _{\varphi },}  [
      {\displaystyle \nabla f(r,\theta ,\varphi )={\frac {\partial f}{\partial
      r}}\mathbf {e} _{r}+{\frac {1}{r}}{\frac {\partial f}{\partial \theta
      }}\mathbf {e} _{\theta }+{\frac {1}{r\sin \theta }}{\frac {\partial f}
      {\partial \varphi }}\mathbf {e} _{\varphi },}]
where r is the radial distance, Ï is the azimuthal angle and Î¸ is the polar
angle, and er, eÎ¸ and eÏ are again local unit vectors pointing in the
coordinate directions (i.e. the normalized covariant_basis).
For the gradient in other orthogonal_coordinate_systems, see Orthogonal
coordinates_(Differential_operators_in_three_dimensions).
**** General coordinates[edit] ****
We consider general_coordinates, which we write as x1, ..., xi, ..., xn, where
n is the number of dimensions of the domain. Here, the upper index refers to
the position in the list of the coordinate or component, so x2 refers to the
second componentânot the quantity x squared. The index variable i refers to
an arbitrary element xi. Using Einstein_notation, the gradient can then be
written as:
         &#x2207; f =    &#x2202; f   &#x2202;  x  i       g  i j     e   j
      {\displaystyle \nabla f={\frac {\partial f}{\partial x^{i}}}g^{ij}\mathbf
      {e} _{j}}  [{\displaystyle \nabla f={\frac {\partial f}{\partial x^
      {i}}}g^{ij}\mathbf {e} _{j}}] ( Note that its dual is      d  f =
      &#x2202; f   &#x2202;  x  i        e   i     {\displaystyle \mathrm {d}
      f={\frac {\partial f}{\partial x^{i}}}\mathbf {e} ^{i}}  [{\displaystyle
      \mathrm {d} f={\frac {\partial f}{\partial x^{i}}}\mathbf {e} ^{i}}] ),
where       e   i   = &#x2202;  x   /  &#x2202;  x  i     {\displaystyle
\mathbf {e} _{i}=\partial \mathbf {x} /\partial x^{i}}  [{\displaystyle \mathbf
{e} _{i}=\partial \mathbf {x} /\partial x^{i}}] and       e   i   =  d   x  i
{\displaystyle \mathbf {e} ^{i}=\mathrm {d} x^{i}}  [{\displaystyle \mathbf {e}
^{i}=\mathrm {d} x^{i}}] refer to the unnormalized local covariant_and
contravariant_bases respectively,      g  i j     {\displaystyle g^{ij}}  [g^
{ij}] is the inverse_metric_tensor, and the Einstein summation convention
implies summation over i and j.
If the coordinates are orthogonal we can easily express the gradient (and the
differential) in terms of the normalized bases, which we refer to as          e
&#x005E;     i     {\displaystyle {\hat {\mathbf {e} }}_{i}}  [{\hat {\mathbf
{e} }}_{i}] and          e  &#x005E;     i     {\displaystyle {\hat {\mathbf
{e} }}^{i}}  [{\displaystyle {\hat {\mathbf {e} }}^{i}}], using the scale
factors (also known as LamÃ©_coefficients)      h  i   = &#x2016;   e   i
&#x2016; = 1   /  &#x2016;   e   i    &#x2016;   {\displaystyle h_{i}=\lVert
\mathbf {e} _{i}\rVert =1\,/\lVert \mathbf {e} ^{i}\,\rVert }  [{\displaystyle
h_{i}=\lVert \mathbf {e} _{i}\rVert =1\,/\lVert \mathbf {e} ^{i}\,\rVert }] :
         &#x2207; f =  &#x2211;  i = 1   n       &#x2202; f   &#x2202;  x  i
      1  h  i         e &#x005E;     i     {\displaystyle \nabla f=\sum _{i=1}^
      {n}\,{\frac {\partial f}{\partial x^{i}}}{\frac {1}{h_{i}}}\mathbf {\hat
      {e}} _{i}}  [{\displaystyle \nabla f=\sum _{i=1}^{n}\,{\frac {\partial f}
      {\partial x^{i}}}{\frac {1}{h_{i}}}\mathbf {\hat {e}} _{i}}] ( and      d
      f =  &#x2211;  i = 1   n       &#x2202; f   &#x2202;  x  i        1  h  i
      e &#x005E;     i     {\displaystyle \mathrm {d} f=\sum _{i=1}^{n}\,{\frac
      {\partial f}{\partial x^{i}}}{\frac {1}{h_{i}}}\mathbf {\hat {e}} ^{i}}
      [{\displaystyle \mathrm {d} f=\sum _{i=1}^{n}\,{\frac {\partial f}
      {\partial x^{i}}}{\frac {1}{h_{i}}}\mathbf {\hat {e}} ^{i}}] ),
where we cannot use Einstein notation, since it is impossible to avoid the
repetition of more than two indices. Despite the use of upper and lower
indices,         e &#x005E;     i     {\displaystyle \mathbf {\hat {e}} _{i}}
[{\displaystyle \mathbf {\hat {e}} _{i}}],         e &#x005E;     i
{\displaystyle \mathbf {\hat {e}} ^{i}}  [{\displaystyle \mathbf {\hat {e}} ^
{i}}], and      h  i     {\displaystyle h_{i}}  [h_{i}] are neither
contravariant nor covariant.
The latter expression evaluates to the expressions given above for cylindrical
and spherical coordinates.
***** Gradient and the derivative or differential[edit] *****
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
**** Linear approximation to a function[edit] ****
The gradient of a function f from the Euclidean space Rn to R at any particular
point x0 in Rn characterizes the best linear_approximation to f at x0. The
approximation is as follows:
         f ( x ) &#x2248; f (  x  0   ) + ( &#x2207; f  )   x  0     &#x22C5;
      ( x &#x2212;  x  0   )   {\displaystyle f(x)\approx f(x_{0})+(\nabla f)_
      {x_{0}}\cdot (x-x_{0})}  [{\displaystyle f(x)\approx f(x_{0})+(\nabla f)_
      {x_{0}}\cdot (x-x_{0})}]
for x close to x0, where (âf )x0 is the gradient of f computed at x0, and the
dot denotes the dot product on Rn. This equation is equivalent to the first two
terms in the multivariable_Taylor_series expansion of f at x0.
**** Differential or (exterior) derivative[edit] ****
The best linear approximation to a differentiable function
         f &#x003A;   R   n   &#x2192;  R    {\displaystyle f\colon \mathbf {R}
      ^{n}\to \mathbf {R} }  [{\displaystyle f\colon \mathbf {R} ^{n}\to
      \mathbf {R} }]
at a point x in Rn is a linear map from Rn to R which is often denoted by dfx
or Df(x) and called the differential or (total)_derivative of f at x. The
gradient is therefore related to the differential by the formula
         ( &#x2207; f  )  x   &#x22C5; v = d  f  x   ( v )   {\displaystyle
      (\nabla f)_{x}\cdot v=df_{x}(v)}  [{\displaystyle (\nabla f)_{x}\cdot
      v=df_{x}(v)}]
for any v â Rn. The function df, which maps x to dfx, is called the
differential or exterior_derivative of f and is an example of a differential_1-
form.
If Rn is viewed as the space of (dimension n) column vectors (of real numbers),
then one can regard df as the row vector with components
          (     &#x2202; f   &#x2202;  x  1      , &#x2026; ,    &#x2202; f
      &#x2202;  x  n       )  ,   {\displaystyle \left({\frac {\partial f}
      {\partial x_{1}}},\dots ,{\frac {\partial f}{\partial x_{n}}}\right),}  [
      {\displaystyle \left({\frac {\partial f}{\partial x_{1}}},\dots ,{\frac
      {\partial f}{\partial x_{n}}}\right),}]
so that dfx(v) is given by matrix multiplication. Assuming the standard
Euclidean metric on Rn, the gradient is then the corresponding column vector,
i.e.,
         ( &#x2207; f  )  i   = d  f  i    T    .   {\displaystyle (\nabla f)_
      {i}=df_{i}^{\mathsf {T}}.}  [{\displaystyle (\nabla f)_{i}=df_{i}^
      {\mathsf {T}}.}]
**** Gradient as a derivative[edit] ****
Let U be an open_set in Rn. If the function f : U â R is differentiable, then
the differential of f is the (FrÃ©chet) derivative of f. Thus âf is a
function from U to the space Rn such that
          lim  h &#x2192; 0       |  f ( x + h ) &#x2212; f ( x ) &#x2212;
      &#x2207; f ( x ) &#x22C5; h  |    &#x2016; h &#x2016;    = 0 ,
      {\displaystyle \lim _{h\to 0}{\frac {|f(x+h)-f(x)-\nabla f(x)\cdot h|}
      {\|h\|}}=0,}  [{\displaystyle \lim _{h\to 0}{\frac {|f(x+h)-f(x)-\nabla f
      (x)\cdot h|}{\|h\|}}=0,}]
where Â· is the dot product.
As a consequence, the usual properties of the derivative hold for the gradient:
*** Linearity[edit] ***
The gradient is linear in the sense that if f and g are two real-valued
functions differentiable at the point a â Rn, and Î± and Î² are two
constants, then Î±f + Î²g is differentiable at a, and moreover
         &#x2207;  (  &#x03B1; f + &#x03B2; g  )  ( a ) = &#x03B1; &#x2207; f
      ( a ) + &#x03B2; &#x2207; g ( a ) .   {\displaystyle \nabla \left(\alpha
      f+\beta g\right)(a)=\alpha \nabla f(a)+\beta \nabla g(a).}  [\nabla \left
      (\alpha f+\beta g\right)(a)=\alpha \nabla f(a)+\beta \nabla g(a).]
*** Product_rule[edit] ***
If f and g are real-valued functions differentiable at a point a â Rn, then
the product rule asserts that the product fg is differentiable at a, and
         &#x2207; ( f g ) ( a ) = f ( a ) &#x2207; g ( a ) + g ( a ) &#x2207; f
      ( a ) .   {\displaystyle \nabla (fg)(a)=f(a)\nabla g(a)+g(a)\nabla f(a).}
      [\nabla (fg)(a)=f(a)\nabla g(a)+g(a)\nabla f(a).]
*** Chain_rule[edit] ***
Suppose that f : A â R is a real-valued function defined on a subset A of Rn,
and that f is differentiable at a point a. There are two forms of the chain
rule applying to the gradient. First, suppose that the function g is a
parametric_curve; that is, a function g : I â Rn maps a subset I â R into
Rn. If g is differentiable at a point c â I such that g(c) = a, then
         ( f &#x2218; g  ) &#x2032;  ( c ) = &#x2207; f ( a ) &#x22C5;  g
      &#x2032;  ( c ) ,   {\displaystyle (f\circ g)'(c)=\nabla f(a)\cdot g'
      (c),}  [(f\circ g)'(c)=\nabla f(a)\cdot g'(c),]
where â is the composition_operator: ( fâââg)(x) = f(g(x)).
More generally, if instead I â Rk, then the following holds:
         &#x2207; ( f &#x2218; g ) ( c ) =   (   D g ( c )    )     T
      (   &#x2207; f ( a )   )   ,   {\displaystyle \nabla (f\circ g)(c)={\big
      (}Dg(c){\big )}^{\mathsf {T}}{\big (}\nabla f(a){\big )},}  [
      {\displaystyle \nabla (f\circ g)(c)={\big (}Dg(c){\big )}^{\mathsf {T}}
      {\big (}\nabla f(a){\big )},}]
where (Dg)T denotes the transpose Jacobian_matrix.
For the second form of the chain rule, suppose that h : I â R is a real
valued function on a subset I of R, and that h is differentiable at the point f
(a) â I. Then
         &#x2207; ( h &#x2218; f ) ( a ) =  h &#x2032;    (   f ( a )   )
      &#x2207; f ( a ) .   {\displaystyle \nabla (h\circ f)(a)=h'{\big (}f(a)
      {\big )}\nabla f(a).}  [{\displaystyle \nabla (h\circ f)(a)=h'{\big (}f
      (a){\big )}\nabla f(a).}]
***** Further properties and applications[edit] *****
**** Level sets[edit] ****
See also: Level_set_Â§ Level_sets_versus_the_gradient
A level surface, or isosurface, is the set of all points where some function
has a given value.
If f is differentiable, then the dot product (âf )x â v of the gradient at
a point x with a vector v gives the directional derivative of f at x in the
direction v. It follows that in this case the gradient of f is orthogonal to
the level_sets of f. For example, a level surface in three-dimensional space is
defined by an equation of the form F(x, y, z) = c. The gradient of F is then
normal to the surface.
More generally, any embedded hypersurface in a Riemannian manifold can be cut
out by an equation of the form F(P) = 0 such that dF is nowhere zero. The
gradient of F is then normal to the hypersurface.
Similarly, an affine_algebraic_hypersurface may be defined by an equation F(x1,
..., xn) = 0, where F is a polynomial. The gradient of F is zero at a singular
point of the hypersurface (this is the definition of a singular point). At a
non-singular point, it is a nonzero normal vector.
**** Conservative vector fields and the gradient theorem[edit] ****
Main article: Gradient_theorem
The gradient of a function is called a gradient field. A (continuous) gradient
field is always a conservative_vector_field: its line_integral along any path
depends only on the endpoints of the path, and can be evaluated by the gradient
theorem (the fundamental theorem of calculus for line integrals). Conversely, a
(continuous) conservative vector field is always the gradient of a function.
***** Generalizations[edit] *****
**** Gradient of a vector[edit] ****
See also: Covariant_derivative
Since the total derivative of a vector field is a linear_mapping from vectors
to vectors, it is a tensor quantity.
In rectangular coordinates, the gradient of a vector field f = ( f1, f2, f3) is
defined by:
         &#x2207;  f  =  g  j k      &#x2202;  f  i     &#x2202;  x  j        e
      i   &#x2297;   e   k   ,   {\displaystyle \nabla \mathbf {f} =g^{jk}
      {\frac {\partial f^{i}}{\partial x^{j}}}\mathbf {e} _{i}\otimes \mathbf
      {e} _{k},}  [{\displaystyle \nabla \mathbf {f} =g^{jk}{\frac {\partial f^
      {i}}{\partial x^{j}}}\mathbf {e} _{i}\otimes \mathbf {e} _{k},}]
(where the Einstein_summation_notation is used and the tensor_product of the
vectors ei and ek is a dyadic_tensor of type (2,0)). Overall, this expression
equals the transpose of the Jacobian matrix:
            &#x2202;  f  i     &#x2202;  x  j      =    &#x2202; (  f  1   ,  f
      2   ,  f  3   )   &#x2202; (  x  1   ,  x  2   ,  x  3   )    .
      {\displaystyle {\frac {\partial f^{i}}{\partial x^{j}}}={\frac {\partial
      (f^{1},f^{2},f^{3})}{\partial (x^{1},x^{2},x^{3})}}.}  [{\displaystyle
      {\frac {\partial f^{i}}{\partial x^{j}}}={\frac {\partial (f^{1},f^{2},f^
      {3})}{\partial (x^{1},x^{2},x^{3})}}.}]
In curvilinear coordinates, or more generally on a curved manifold, the
gradient involves Christoffel_symbols:
         &#x2207;  f  =  g  j k    (     &#x2202;  f  i     &#x2202;  x  j
      +    &#x0393;  i     j l    f  l    )    e   i   &#x2297;   e   k   ,
      {\displaystyle \nabla \mathbf {f} =g^{jk}\left({\frac {\partial f^{i}}
      {\partial x^{j}}}+{\Gamma ^{i}}_{jl}f^{l}\right)\mathbf {e} _{i}\otimes
      \mathbf {e} _{k},}  [{\displaystyle \nabla \mathbf {f} =g^{jk}\left(
      {\frac {\partial f^{i}}{\partial x^{j}}}+{\Gamma ^{i}}_{jl}f^
      {l}\right)\mathbf {e} _{i}\otimes \mathbf {e} _{k},}]
where gjk are the components of the inverse metric_tensor and the ei are the
coordinate basis vectors.
Expressed more invariantly, the gradient of a vector field f can be defined by
the Levi-Civita_connection and metric tensor:[24]
          &#x2207;  a    f  b   =  g  a c    &#x2207;  c    f  b   ,
      {\displaystyle \nabla ^{a}f^{b}=g^{ac}\nabla _{c}f^{b},}  [{\displaystyle
      \nabla ^{a}f^{b}=g^{ac}\nabla _{c}f^{b},}]
where âc is the connection.
**** Riemannian manifolds[edit] ****
For any smooth function f on a Riemannian manifold (M, g), the gradient of f is
the vector field âf such that for any vector field X,
         g ( &#x2207; f , X ) =  &#x2202;  X   f ,   {\displaystyle g(\nabla
      f,X)=\partial _{X}f,}  [{\displaystyle g(\nabla f,X)=\partial _{X}f,}]
i.e.,
          g  x     (   ( &#x2207; f  )  x   ,  X  x     )   = (  &#x2202;  X
      f ) ( x ) ,   {\displaystyle g_{x}{\big (}(\nabla f)_{x},X_{x}{\big )}=
      (\partial _{X}f)(x),}  [{\displaystyle g_{x}{\big (}(\nabla f)_{x},X_{x}
      {\big )}=(\partial _{X}f)(x),}]
where gx( , ) denotes the inner_product of tangent vectors at x defined by the
metric g and âX f is the function that takes any point x â M to the
directional derivative of f in the direction X, evaluated at x. In other words,
in a coordinate_chart Ï from an open subset of M to an open subset of Rn,
(âX f )(x) is given by:
          &#x2211;  j = 1   n    X  j     (   &#x03C6; ( x )   )     &#x2202;
      &#x2202;  x  j      ( f &#x2218;  &#x03C6;  &#x2212; 1   )    |
      &#x03C6; ( x )   ,   {\displaystyle \sum _{j=1}^{n}X^{j}{\big (}\varphi
      (x){\big )}{\frac {\partial }{\partial x_{j}}}(f\circ \varphi ^{-1})
      {\Bigg |}_{\varphi (x)},}  [{\displaystyle \sum _{j=1}^{n}X^{j}{\big
      (}\varphi (x){\big )}{\frac {\partial }{\partial x_{j}}}(f\circ \varphi ^
      {-1}){\Bigg |}_{\varphi (x)},}]
where Xj denotes the jth component of X in this coordinate chart.
So, the local form of the gradient takes the form:
         &#x2207; f =  g  i k      &#x2202; f   &#x2202;  x  k         e    i
      .   {\displaystyle \nabla f=g^{ik}{\frac {\partial f}{\partial x^{k}}}
      {\textbf {e}}_{i}.}  [{\displaystyle \nabla f=g^{ik}{\frac {\partial f}
      {\partial x^{k}}}{\textbf {e}}_{i}.}]
Generalizing the case M = Rn, the gradient of a function is related to its
exterior derivative, since
         (  &#x2202;  X   f ) ( x ) = ( d f  )  x   (  X  x   ) .
      {\displaystyle (\partial _{X}f)(x)=(df)_{x}(X_{x}).}  [{\displaystyle
      (\partial _{X}f)(x)=(df)_{x}(X_{x}).}]
More precisely, the gradient âf is the vector field associated to the
differential 1-form df using the musical_isomorphism
         &#x266F; =  &#x266F;  g   &#x003A;  T  &#x2217;   M &#x2192; T M
      {\displaystyle \sharp =\sharp ^{g}\colon T^{*}M\to TM}  [\sharp =\sharp ^
      {g}\colon T^{*}M\to TM]
(called "sharp") defined by the metric g. The relation between the exterior
derivative and the gradient of a function on Rn is a special case of this in
which the metric is the flat metric given by the dot product.
***** See also[edit] *****
    * Curl
    * Divergence
    * Four-gradient
    * Hessian_matrix
    * Skew_gradient
***** Notes[edit] *****
   1. ^ Beauregard_&_Fraleigh_(1973, p. 84)
   2. ^ Bachman_(2007, p. 76)
   3. ^ Beauregard_&_Fraleigh_(1973, p. 84)
   4. ^ Downing_(2010, p. 316)
   5. ^ Harper_(1976, p. 15)
   6. ^ Kreyszig_(1972, p. 307)
   7. ^ McGraw-Hill_(2007, p. 196)
   8. ^ Moise_(1967, p. 683)
   9. ^ Protter_&_Morrey,_Jr._(1970, p. 714)
  10. ^ Swokowski_et_al._(1994, p. 1038)
  11. ^ Protter_&_Morrey,_Jr._(1970, pp. 21,88)
  12. ^ Bachman_(2007, p. 77)
  13. ^ Downing_(2010, pp. 316â317)
  14. ^ Kreyszig_(1972, p. 309)
  15. ^ McGraw-Hill_(2007, p. 196)
  16. ^ Moise_(1967, p. 684)
  17. ^ Protter_&_Morrey,_Jr._(1970, p. 715)
  18. ^ Swokowski_et_al._(1994, pp. 1036,1038â1039)
  19. ^ Kreyszig_(1972, pp. 308â309)
  20. ^ Stoker_(1969, p. 292)
  21. ^ Beauregard_&_Fraleigh_(1973, pp. 87,248)
  22. ^ Kreyszig_(1972, pp. 333,353,496)
  23. ^ a b Schey_1992, pp. 139â142.
  24. ^ Dubrovin,_Fomenko_&_Novikov_1991, pp. 348â349.
***** References[edit] *****
    * Bachman, David (2007), Advanced Calculus Demystified, New York: McGraw-
      Hill, ISBN 0-07-148121-4
Beauregard, Raymond A.; Fraleigh, John B. (1973), A First Course In Linear
Algebra: with Optional Introduction to Groups, Rings, and Fields, Boston:
Houghton_Mifflin_Company, ISBN 0-395-14017-X
Downing, Douglas, Ph.D. (2010), Barron's E-Z Calculus, New York: Barron's,
ISBN 978-0-7641-4461-5
Dubrovin, B. A.; Fomenko, A. T.; Novikov, S. P. (1991). Modern
GeometryâMethods and Applications: Part I: The Geometry of Surfaces,
Transformation Groups, and Fields. Graduate_Texts_in_Mathematics (2nd ed.).
Springer. ISBN 978-0-387-97663-1.
Harper, Charlie (1976), Introduction to Mathematical Physics, New Jersey:
Prentice-Hall, ISBN 0-13-487538-9
Kreyszig,_Erwin (1972), Advanced Engineering Mathematics (3rd ed.), New York:
Wiley, ISBN 0-471-50728-8
McGraw-Hill Encyclopedia of Science & Technology (10th ed.). New York: McGraw-
Hill. 2007. ISBN 0-07-144143-3.
Moise, Edwin E. (1967), Calculus: Complete, Reading: Addison-Wesley
Protter, Murray H.; Morrey, Jr., Charles B. (1970), College Calculus with
Analytic Geometry (2nd ed.), Reading: Addison-Wesley, LCCN 76087042
Schey, H. M. (1992). Div, Grad, Curl, and All That (2nd ed.). W. W. Norton.
ISBN 0-393-96251-2. OCLC 25048561.
Stoker, J. J. (1969), Differential Geometry, New York: Wiley, ISBN 0-471-82825-
4
Swokowski, Earl W.; Olinick, Michael; Pence, Dennis; Cole, Jeffery A. (1994),
Calculus (6th ed.), Boston: PWS Publishing Company, ISBN 0-534-93624-5
***** Further reading[edit] *****
    * Korn, Theresa M.; Korn, Granino Arthur (2000). Mathematical Handbook for
      Scientists and Engineers: Definitions, Theorems, and Formulas for
      Reference and Review. Dover Publications. pp. 157â160. ISBN 0-486-
      41147-8. OCLC 43864234.
***** External links[edit] *****
 Look up gradient in Wiktionary, the free dictionary.
    * "Gradient". Khan_Academy.
Kuptsov, L.P. (2001) [1994], "Gradient", in Hazewinkel,_Michiel (ed.),
Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. / Kluwer
Academic Publishers, ISBN 978-1-55608-010-4
.
Weisstein,_Eric_W. "Gradient". MathWorld.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Gradient&oldid=909933479"
Categories:
    * Differential_operators
    * Differential_calculus
    * Generalizations_of_the_derivative
    * Linear_operators_in_calculus
    * Vector_calculus
    * Rates
Hidden categories:
    * Articles_lacking_in-text_citations_from_January_2018
    * All_articles_lacking_in-text_citations
    * Articles_with_short_description
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
    * á áá­á
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * Ð§ÓÐ²Ð°ÑÐ»Ð°
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Ido
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * à´®à´²à´¯à´¾à´³à´
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 8 August 2019, at 15:36 (UTC).
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
