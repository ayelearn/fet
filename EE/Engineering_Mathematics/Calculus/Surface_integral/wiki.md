The following text has been accessed from https://en.wikipedia.org/wiki/Surface_integral at Thu Aug 8 22:51:13 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Surface integral ******
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
    * Partial_derivative
    * Multiple_integral
    * Line_integral
    * Surface integral
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
 This article needs additional citations for verification. Please help improve_this_article by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and removed.
 Find sources: "Surface_integral" â news Â· newspapers Â· books Â· scholar Â· JSTOR (January
 2017)(Learn_how_and_when_to_remove_this_template_message)
In mathematics, a surface integral is a generalization of multiple_integrals to
integration over surfaces. It can be thought of as the double_integral analogue
of the line_integral. Given a surface, one may integrate over its scalar_fields
(that is, functions which return scalars as values), and vector_fields (that
is, functions which return vectors as values).
Surface integrals have applications in physics, particularly with the theories
of classical_electromagnetism.
The definition of surface integral relies on splitting the surface into small
surface elements.
An illustration of a single surface element. These elements are made
infinitesimally small, by the limiting process, so as to approximate the
surface.
⁰
***** Contents *****
    * 1_Surface_integrals_of_scalar_fields
    * 2_Surface_integrals_of_vector_fields
    * 3_Surface_integrals_of_differential_2-forms
    * 4_Theorems_involving_surface_integrals
    * 5_Advanced_issues
    * 6_See_also
    * 7_References
    * 8_External_links
***** Surface integrals of scalar fields[edit] *****
To find an explicit formula for the surface integral, we need to parameterize
the surface of interest, S, by considering a system of curvilinear_coordinates
on S, like the latitude_and_longitude on a sphere. Let such a parameterization
be x(s, t), where (s, t) varies in some region T in the plane. Then, the
surface integral is given by
          &#x222C;  S   f   d  S =  &#x222C;  T   f (  x  ( s , t ) )  &#x2016;
      &#x2202;  x    &#x2202; s    &#x00D7;    &#x2202;  x    &#x2202; t
      &#x2016;   d  s   d  t   {\displaystyle \iint \limits _{S}f\,\mathrm {d}
      S=\iint \limits _{T}f(\mathbf {x} (s,t))\left\|{\partial \mathbf {x}
      \over \partial s}\times {\partial \mathbf {x} \over \partial
      t}\right\|\mathrm {d} s\,\mathrm {d} t}  [{\displaystyle \iint \limits _
      {S}f\,\mathrm {d} S=\iint \limits _{T}f(\mathbf {x} (s,t))\left\|
      {\partial \mathbf {x}  \over \partial s}\times {\partial \mathbf {x}
      \over \partial t}\right\|\mathrm {d} s\,\mathrm {d} t}]
where the expression between bars on the right-hand side is the magnitude of
the cross_product of the partial_derivatives of x(s, t), and is known as the
surface element. The surface integral can also be expressed in the equivalent
form
          &#x222C;  S   f   d  &#x03A3; =  &#x222C;  T   f (  x  ( s , t ) )
      g     d  s   d  t   {\displaystyle \iint \limits _{S}f\,\mathrm {d}
      \Sigma =\iint \limits _{T}f(\mathbf {x} (s,t)){\sqrt {g}}\,\mathrm {d}
      s\,\mathrm {d} t}  [{\displaystyle \iint \limits _{S}f\,\mathrm {d}
      \Sigma =\iint \limits _{T}f(\mathbf {x} (s,t)){\sqrt {g}}\,\mathrm {d}
      s\,\mathrm {d} t}]
where g is the determinant of the first_fundamental_form of the surface mapping
x(s, t).[1][2]
For example, if we want to find the surface_area of the graph of some scalar
function, say     z = f  ( x , y )   {\displaystyle z=f\,(x,y)}  [z=f\,(x,y)],
we have
         A =  &#x222C;  S     d  &#x03A3; =  &#x222C;  T    &#x2016;
      &#x2202;  r    &#x2202; x    &#x00D7;    &#x2202;  r    &#x2202; y
      &#x2016;   d  x   d  y   {\displaystyle A=\iint \limits _{S}\,\mathrm {d}
      \Sigma =\iint \limits _{T}\left\|{\partial \mathbf {r} \over \partial
      x}\times {\partial \mathbf {r} \over \partial y}\right\|\mathrm {d}
      x\,\mathrm {d} y}  [{\displaystyle A=\iint \limits _{S}\,\mathrm {d}
      \Sigma =\iint \limits _{T}\left\|{\partial \mathbf {r}  \over \partial
      x}\times {\partial \mathbf {r}  \over \partial y}\right\|\mathrm {d}
      x\,\mathrm {d} y}]
where      r  = ( x , y , z ) = ( x , y , f ( x , y ) )   {\displaystyle
\mathbf {r} =(x,y,z)=(x,y,f(x,y))}  [\mathbf{r}=(x, y, z)=(x, y, f(x,y))]. So
that        &#x2202;  r    &#x2202; x    = ( 1 , 0 ,  f  x   ( x , y ) )
{\displaystyle {\partial \mathbf {r} \over \partial x}=(1,0,f_{x}(x,y))}  [
{\partial \mathbf{r} \over \partial x}=(1, 0, f_x(x,y))], and        &#x2202;
r    &#x2202; y    = ( 0 , 1 ,  f  y   ( x , y ) )   {\displaystyle {\partial
\mathbf {r} \over \partial y}=(0,1,f_{y}(x,y))}  [{\partial \mathbf{r} \over
\partial y}=(0, 1, f_y(x,y))]. So,
             A      =  &#x222C;  T    &#x2016;   (  1 , 0 ,    &#x2202; f
      &#x2202; x     )  &#x00D7;  (  0 , 1 ,    &#x2202; f   &#x2202; y     )
      &#x2016;   d  x   d  y         =  &#x222C;  T    &#x2016;  (  &#x2212;
      &#x2202; f   &#x2202; x    , &#x2212;    &#x2202; f   &#x2202; y    , 1
      )  &#x2016;   d  x   d  y         =  &#x222C;  T       (    &#x2202; f
      &#x2202; x    )   2   +   (    &#x2202; f   &#x2202; y    )   2   + 1
      d  x   d  y       {\displaystyle {\begin{aligned}A&{}=\iint \limits _
      {T}\left\|\left(1,0,{\partial f \over \partial x}\right)\times \left(0,1,
      {\partial f \over \partial y}\right)\right\|\mathrm {d} x\,\mathrm {d}
      y\\&{}=\iint \limits _{T}\left\|\left(-{\partial f \over \partial x},-
      {\partial f \over \partial y},1\right)\right\|\mathrm {d} x\,\mathrm {d}
      y\\&{}=\iint \limits _{T}{\sqrt {\left({\partial f \over \partial
      x}\right)^{2}+\left({\partial f \over \partial y}\right)^
      {2}+1}}\,\,\mathrm {d} x\,\mathrm {d} y\end{aligned}}}  [{\displaystyle
      {\begin{aligned}A&{}=\iint \limits _{T}\left\|\left(1,0,{\partial f \over
      \partial x}\right)\times \left(0,1,{\partial f \over \partial
      y}\right)\right\|\mathrm {d} x\,\mathrm {d} y\\&{}=\iint \limits _
      {T}\left\|\left(-{\partial f \over \partial x},-{\partial f \over
      \partial y},1\right)\right\|\mathrm {d} x\,\mathrm {d} y\\&{}=\iint
      \limits _{T}{\sqrt {\left({\partial f \over \partial x}\right)^{2}+\left(
      {\partial f \over \partial y}\right)^{2}+1}}\,\,\mathrm {d} x\,\mathrm
      {d} y\end{aligned}}}]
which is the standard formula for the area of a surface described this way. One
can recognize the vector in the second line above as the normal_vector to the
surface.
Note that because of the presence of the cross product, the above formulas only
work for surfaces embedded in three-dimensional space.
This can be seen as integrating a Riemannian_volume_form on the parameterized
surface, where the metric_tensor is given by the first_fundamental_form of the
surface.
***** Surface integrals of vector fields[edit] *****
A vector field on a surface
Consider a vector field v on S, that is, for each x in S, v(x) is a vector.
The surface integral can be defined component-wise according to the definition
of the surface integral of a scalar field; the result is a vector. This applies
for example in the expression of the electric field at some fixed point due to
an electrically charged surface, or the gravity at some fixed point due to a
sheet of material.
Alternatively, if we integrate the normal_component of the vector field, the
result is a scalar. Imagine that we have a fluid flowing through S, such that v
(x) determines the velocity of the fluid at x. The flux is defined as the
quantity of fluid flowing through S per unit time.
This illustration implies that if the vector field is tangent to S at each
point, then the flux is zero because the fluid just flows in parallel to S, and
neither in nor out. This also implies that if v does not just flow along S,
that is, if v has both a tangential and a normal component, then only the
normal component contributes to the flux. Based on this reasoning, to find the
flux, we need to take the dot_product of v with the unit surface_normal n to S
at each point, which will give us a scalar field, and integrate the obtained
field as above. We find the formula
              &#x222C;  S     v   &#x22C5;  d    &#x03A3;      =  &#x222C;  S
      (    v   &#x22C5;   n    )    d  &#x03A3;         =  &#x222C;  T
      (    v   (  x  ( s , t ) ) &#x22C5;    (     &#x2202;  x    &#x2202; s
      &#x00D7;    &#x2202;  x    &#x2202; t     )   &#x2016;  (     &#x2202;  x
      &#x2202; s    &#x00D7;    &#x2202;  x    &#x2202; t     )  &#x2016;     )
      &#x2016;  (     &#x2202;  x    &#x2202; s    &#x00D7;    &#x2202;  x
      &#x2202; t     )  &#x2016;   d  s   d  t         =  &#x222C;  T     v
      (  x  ( s , t ) ) &#x22C5;  (     &#x2202;  x    &#x2202; s    &#x00D7;
      &#x2202;  x    &#x2202; t     )   d  s   d  t .       {\displaystyle
      {\begin{aligned}\iint \limits _{S}{\mathbf {v} }\cdot \mathrm {d}
      {\mathbf {\Sigma } }&=\iint \limits _{S}\left({\mathbf {v} }\cdot
      {\mathbf {n} }\right)\,\mathrm {d} \Sigma \\&{}=\iint \limits _{T}\left(
      {\mathbf {v} }(\mathbf {x} (s,t))\cdot {\left({\partial \mathbf {x} \over
      \partial s}\times {\partial \mathbf {x} \over \partial t}\right) \over
      \left\|\left({\partial \mathbf {x} \over \partial s}\times {\partial
      \mathbf {x} \over \partial t}\right)\right\|}\right)\left\|\left(
      {\partial \mathbf {x} \over \partial s}\times {\partial \mathbf {x} \over
      \partial t}\right)\right\|\mathrm {d} s\,\mathrm {d} t\\&{}=\iint \limits
      _{T}{\mathbf {v} }(\mathbf {x} (s,t))\cdot \left({\partial \mathbf {x}
      \over \partial s}\times {\partial \mathbf {x} \over \partial
      t}\right)\mathrm {d} s\,\mathrm {d} t.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}\iint \limits _{S}{\mathbf {v} }\cdot \mathrm {d}
      {\mathbf {\Sigma } }&=\iint \limits _{S}\left({\mathbf {v} }\cdot
      {\mathbf {n} }\right)\,\mathrm {d} \Sigma \\&{}=\iint \limits _{T}\left(
      {\mathbf {v} }(\mathbf {x} (s,t))\cdot {\left({\partial \mathbf {x}
      \over \partial s}\times {\partial \mathbf {x}  \over \partial t}\right)
      \over \left\|\left({\partial \mathbf {x}  \over \partial s}\times
      {\partial \mathbf {x}  \over \partial
      t}\right)\right\|}\right)\left\|\left({\partial \mathbf {x}  \over
      \partial s}\times {\partial \mathbf {x}  \over \partial
      t}\right)\right\|\mathrm {d} s\,\mathrm {d} t\\&{}=\iint \limits _{T}
      {\mathbf {v} }(\mathbf {x} (s,t))\cdot \left({\partial \mathbf {x}  \over
      \partial s}\times {\partial \mathbf {x}  \over \partial t}\right)\mathrm
      {d} s\,\mathrm {d} t.\end{aligned}}}]
The cross product on the right-hand side of this expression is a (not
necessarily unital) surface normal determined by the parametrization.
This formula defines the integral on the left (note the dot and the vector
notation for the surface element).
We may also interpret this as a special case of integrating 2-forms, where we
identify the vector field with a 1-form, and then integrate its Hodge_dual over
the surface. This is equivalent to integrating     &#x27E8;  v  ,  n  &#x27E9;
d  &#x03A3;   {\displaystyle \langle \mathbf {v} ,\mathbf {n} \rangle \;\mathrm
{d} \Sigma }  [{\displaystyle \langle \mathbf {v} ,\mathbf {n} \rangle
\;\mathrm {d} \Sigma }] over the immersed surface, where      d  &#x03A3;
{\displaystyle \mathrm {d} \Sigma }  [{\displaystyle \mathrm {d} \Sigma }] is
the induced volume form on the surface, obtained by interior_multiplication of
the Riemannian metric of the ambient space with the outward normal of the
surface.
***** Surface integrals of differential 2-forms[edit] *****
Let
         f =  f  z     d  x &#x2227;  d  y +  f  x     d  y &#x2227;  d  z +  f
      y     d  z &#x2227;  d  x   {\displaystyle f=f_{z}\,\mathrm {d} x\wedge
      \mathrm {d} y+f_{x}\,\mathrm {d} y\wedge \mathrm {d} z+f_{y}\,\mathrm {d}
      z\wedge \mathrm {d} x}  [ f=f_{z}\, \mathrm dx \wedge \mathrm dy + f_
      {x}\, \mathrm dy \wedge \mathrm dz + f_{y}\, \mathrm dz  \wedge \mathrm
      dx ]
be a differential_2-form defined on the surface S, and let
          x  ( s , t ) = ( x ( s , t ) , y ( s , t ) , z ( s , t ) )
      {\displaystyle \mathbf {x} (s,t)=(x(s,t),y(s,t),z(s,t))\!}  [\mathbf{x}
      (s,t)=( x(s,t), y(s,t), z(s,t))\!]
be an orientation_preserving parametrization of S with     ( s , t )
{\displaystyle (s,t)}  [(s,t)] in D. Changing coordinates from     ( x , y )
{\displaystyle (x,y)}  [(x,y)] to     ( s , t )   {\displaystyle (s,t)}  [(s,
t)], the differential forms transform as
          d  x =    &#x2202; x   &#x2202; s     d  s +    &#x2202; x   &#x2202;
      t     d  t   {\displaystyle \mathrm {d} x={\frac {\partial x}{\partial
      s}}\mathrm {d} s+{\frac {\partial x}{\partial t}}\mathrm {d} t}  [
      {\displaystyle \mathrm {d} x={\frac {\partial x}{\partial s}}\mathrm {d}
      s+{\frac {\partial x}{\partial t}}\mathrm {d} t}]
          d  y =    &#x2202; y   &#x2202; s     d  s +    &#x2202; y   &#x2202;
      t     d  t   {\displaystyle \mathrm {d} y={\frac {\partial y}{\partial
      s}}\mathrm {d} s+{\frac {\partial y}{\partial t}}\mathrm {d} t}  [
      {\displaystyle \mathrm {d} y={\frac {\partial y}{\partial s}}\mathrm {d}
      s+{\frac {\partial y}{\partial t}}\mathrm {d} t}]
So      d  x &#x2227;  d  y   {\displaystyle \mathrm {d} x\wedge \mathrm {d} y}
[ \mathrm dx \wedge \mathrm dy ] transforms to        &#x2202; ( x , y )
&#x2202; ( s , t )     d  s &#x2227;  d  t   {\displaystyle {\frac {\partial
(x,y)}{\partial (s,t)}}\mathrm {d} s\wedge \mathrm {d} t}  [ \frac{\partial
(x,y)}{\partial(s,t)}  \mathrm ds \wedge \mathrm dt ], where        &#x2202;
( x , y )   &#x2202; ( s , t )      {\displaystyle {\frac {\partial (x,y)}
{\partial (s,t)}}}  [ \frac{\partial(x,y)}{\partial(s,t)} ] denotes the
determinant of the Jacobian of the transition function from     ( s , t )
{\displaystyle (s,t)}  [(s, t)] to     ( x , y )   {\displaystyle (x,y)}  [
(x,y)]. The transformation of the other forms are similar.
Then, the surface integral of f on S is given by
          &#x222C;  D    [   f  z   (  x  ( s , t ) )    &#x2202; ( x , y )
      &#x2202; ( s , t )    +  f  x   (  x  ( s , t ) )    &#x2202; ( y , z )
      &#x2202; ( s , t )    +  f  y   (  x  ( s , t ) )    &#x2202; ( z , x )
      &#x2202; ( s , t )     ]    d  s   d  t   {\displaystyle \iint \limits _
      {D}\left[f_{z}(\mathbf {x} (s,t)){\frac {\partial (x,y)}{\partial
      (s,t)}}+f_{x}(\mathbf {x} (s,t)){\frac {\partial (y,z)}{\partial
      (s,t)}}+f_{y}(\mathbf {x} (s,t)){\frac {\partial (z,x)}{\partial
      (s,t)}}\right]\,\mathrm {d} s\,\mathrm {d} t}  [{\displaystyle \iint
      \limits _{D}\left[f_{z}(\mathbf {x} (s,t)){\frac {\partial (x,y)}
      {\partial (s,t)}}+f_{x}(\mathbf {x} (s,t)){\frac {\partial (y,z)}
      {\partial (s,t)}}+f_{y}(\mathbf {x} (s,t)){\frac {\partial (z,x)}
      {\partial (s,t)}}\right]\,\mathrm {d} s\,\mathrm {d} t}]
where
            &#x2202;  x    &#x2202; s    &#x00D7;    &#x2202;  x    &#x2202; t
      =  (     &#x2202; ( y , z )   &#x2202; ( s , t )    ,    &#x2202; ( z , x
      )   &#x2202; ( s , t )    ,    &#x2202; ( x , y )   &#x2202; ( s , t )
      )    {\displaystyle {\partial \mathbf {x} \over \partial s}\times
      {\partial \mathbf {x} \over \partial t}=\left({\frac {\partial (y,z)}
      {\partial (s,t)}},{\frac {\partial (z,x)}{\partial (s,t)}},{\frac
      {\partial (x,y)}{\partial (s,t)}}\right)}  [{\partial \mathbf{x} \over
      \partial s}\times {\partial \mathbf{x} \over \partial t}=\left(\frac
      {\partial(y,z)}{\partial(s,t)}, \frac{\partial(z,x)}{\partial(s,t)},
      \frac{\partial(x,y)}{\partial(s,t)}\right)]
is the surface element normal to S.
Let us note that the surface integral of this 2-form is the same as the surface
integral of the vector field which has as components      f  x
{\displaystyle f_{x}}  [f_{x}],      f  y     {\displaystyle f_{y}}  [f_y] and
f  z     {\displaystyle f_{z}}  [f_z].
***** Theorems involving surface integrals[edit] *****
Various useful results for surface integrals can be derived using differential
geometry and vector_calculus, such as the divergence_theorem, and its
generalization, Stokes'_theorem.
***** Advanced issues[edit] *****
Let us notice that we defined the surface integral by using a parametrization
of the surface S. We know that a given surface might have several
parametrizations. For example, if we move the locations of the North Pole and
the South Pole on a sphere, the latitude and longitude change for all the
points on the sphere. A natural question is then whether the definition of the
surface integral depends on the chosen parametrization. For integrals of scalar
fields, the answer to this question is simple, the value of the surface
integral will be the same no matter what parametrization one uses.
For integrals of vector fields, things are more complicated, because the
surface normal is involved. It can be proven that given two parametrizations of
the same surface, whose surface normals point in the same direction, one
obtains the same value for the surface integral with both parametrizations. If,
however, the normals for these parametrizations point in opposite directions,
the value of the surface integral obtained using one parametrization is the
negative of the one obtained via the other parametrization. It follows that
given a surface, we do not need to stick to any unique parametrization; but,
when integrating vector fields, we do need to decide in advance which direction
the normal will point to and then choose any parametrization consistent with
that direction.
Another issue is that sometimes surfaces do not have parametrizations which
cover the whole surface. The obvious solution is then to split that surface
into several pieces, calculate the surface integral on each piece, and then add
them all up. This is indeed how things work, but when integrating vector
fields, one needs to again be careful how to choose the normal-pointing vector
for each piece of the surface, so that when the pieces are put back together,
the results are consistent. For the cylinder, this means that if we decide that
for the side region the normal will point out of the body, then for the top and
bottom circular parts the normal must point out of the body too.
Lastly, there are surfaces which do not admit a surface normal at each point
with consistent results (for example, the MÃ¶bius_strip). If such a surface is
split into pieces, on each piece a parametrization and corresponding surface
normal is chosen, and the pieces are put back together, we will find that the
normal vectors coming from different pieces cannot be reconciled. This means
that at some junction between two pieces we will have normal vectors pointing
in opposite directions. Such a surface is called non-orientable, and on this
kind of surface, one cannot talk about integrating vector fields.
***** See also[edit] *****
    * Divergence_theorem
    * Stokes'_theorem
    * Line_integral
    * Volume_element
    * Volume_integral
    * Cartesian_coordinate_system
    * Volume_and_surface_area_elements_in_spherical_coordinate_systems
    * Volume_and_surface_area_elements_in_cylindrical_coordinate_systems
    * HolsteinâHerring_method
***** References[edit] *****
   1. ^Edwards, C. H. (1994). Advanced Calculus of Several Variables. Mineola,
      NY: Dover. p. 335. ISBN 0-486-68336-2.
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
   3. ^Hazewinkel, Michiel (2001). Encyclopedia_of_Mathematics. Springer.
      pp. Surface Integral. ISBN 978-1-55608-010-4.
***** External links[edit] *****
    * Surface_Integral_â_from_MathWorld
    * Surface_Integral_â_Theory_and_exercises

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Surface_integral&oldid=878778288"
Categories:
    * Multivariable_calculus
    * Area
    * Surfaces
Hidden categories:
    * Articles_needing_additional_references_from_January_2017
    * All_articles_needing_additional_references
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * áá¶áá¶ááááá
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 16 January 2019, at 21:33 (UTC).
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
