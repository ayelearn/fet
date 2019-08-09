The following text has been accessed from https://en.wikipedia.org/wiki/Directional_derivative at Fri Aug 9 00:02:26 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Directional derivative ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This section needs additional citations for verification. Relevant discussion may be
 found on the talk_page. Please help improve_this_article by adding_citations_to_reliable
 sources. Unsourced material may be challenged and removed.
 Find sources: "Directional_derivative" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (October 2012)(Learn_how_and_when_to_remove_this_template_message)
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
    * Directional derivative
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
In mathematics, the directional derivative of a multivariate differentiable
function along a given vector v at a given point x intuitively represents the
instantaneous rate of change of the function, moving through x with a velocity
specified by v. It therefore generalizes the notion of a partial_derivative, in
which the rate of change is taken along one of the curvilinear coordinate
curves, all other coordinates being constant.
The directional derivative is a special case of the Gateaux_derivative.
⁰
***** Contents *****
    * 1_Notation
    * 2_Definition
          o 2.1_Using_only_direction_of_vector
          o 2.2_Restriction_to_a_unit_vector
    * 3_Properties
    * 4_In_differential_geometry
          o 4.1_The_Lie_derivative
          o 4.2_The_Riemann_tensor
    * 5_In_group_theory
          o 5.1_Translations
          o 5.2_Rotations
    * 6_Normal_derivative
    * 7_In_the_continuum_mechanics_of_solids
          o 7.1_Derivatives_of_scalar-valued_functions_of_vectors
          o 7.2_Derivatives_of_vector-valued_functions_of_vectors
          o 7.3_Derivatives_of_scalar-valued_functions_of_second-order_tensors
          o 7.4_Derivatives_of_tensor-valued_functions_of_second-order_tensors
    * 8_See_also
    * 9_Notes
    * 10_References
    * 11_External_links
***** Notation[edit] *****
Let τ be a curve whose tangent vector at some chosen point is v. The
directional derivative of a function f with respect to v may be denoted by any
of the following
    *     &#x2207;   v     f  (  x  ) ,   {\displaystyle \nabla _{\mathbf {v} }
      {f}(\mathbf {x} ),}  [{\displaystyle \nabla _{\mathbf {v} }{f}(\mathbf
      {x} ),}]
    *     f   v   &#x2032;  (  x  ) ,   {\displaystyle f'_{\mathbf {v} }
      (\mathbf {x} ),}  [{\displaystyle f'_{\mathbf {v} }(\mathbf {x} ),}]
    *     D   v    f (  x  ) ,   {\displaystyle D_{\mathbf {v} }f(\mathbf {x}
      ),}  [{\displaystyle D_{\mathbf {v} }f(\mathbf {x} ),}]
    *    D f (  x  ) (  v  ) ,   {\displaystyle Df(\mathbf {x} )(\mathbf {v}
      ),}  [{\displaystyle Df(\mathbf {x} )(\mathbf {v} ),}]
    *     &#x2202;   v    f (  x  ) ,   {\displaystyle \partial _{\mathbf {v}
      }f(\mathbf {x} ),}  [{\displaystyle \partial _{\mathbf {v} }f(\mathbf {x}
      ),}]
    *       &#x2202;  f (  x  )    &#x2202;   v      ,   {\displaystyle {\frac
      {\partial {f(\mathbf {x} )}}{\partial {\mathbf {v} }}},}  [{\displaystyle
      {\frac {\partial {f(\mathbf {x} )}}{\partial {\mathbf {v} }}},}]
    *     v  &#x22C5;  &#x2207; f (  x  )  ,   {\displaystyle \mathbf {v} \cdot
      {\nabla f(\mathbf {x} )},}  [{\displaystyle \mathbf {v} \cdot {\nabla f
      (\mathbf {x} )},}]
    *     v  &#x22C5;    &#x2202; f (  x  )   &#x2202;  x     .
      {\displaystyle \mathbf {v} \cdot {\frac {\partial f(\mathbf {x} )}
      {\partial \mathbf {x} }}.}  [{\displaystyle \mathbf {v} \cdot {\frac
      {\partial f(\mathbf {x} )}{\partial \mathbf {x} }}.}]
***** Definition[edit] *****
A contour_plot of     f ( x , y ) =  x  2   +  y  2     {\displaystyle f
(x,y)=x^{2}+y^{2}}  [f(x, y)=x^2 + y^2], showing the gradient vector in black,
and the unit vector      u    {\displaystyle \mathbf {u} }  [\mathbf {u} ]
scaled by the directional derivative in the direction of      u
{\displaystyle \mathbf {u} }  [\mathbf {u} ] in orange. The gradient vector is
longer because the gradient points in the direction of greatest rate of
increase of a function.
The directional derivative of a scalar_function
         f (  x  ) = f (  x  1   ,  x  2   , &#x2026; ,  x  n   )
      {\displaystyle f(\mathbf {x} )=f(x_{1},x_{2},\ldots ,x_{n})}  [
      {\displaystyle f(\mathbf {x} )=f(x_{1},x_{2},\ldots ,x_{n})}]
along a vector
          v  = (  v  1   , &#x2026; ,  v  n   )   {\displaystyle \mathbf {v} =
      (v_{1},\ldots ,v_{n})}  [{\displaystyle \mathbf {v} =(v_{1},\ldots ,v_
      {n})}]
is the function      &#x2207;   v     f    {\displaystyle \nabla _{\mathbf {v}
}{f}}  [{\displaystyle \nabla _{\mathbf {v} }{f}}] defined by the limit[1]
          &#x2207;   v     f  (  x  ) =  lim  h &#x2192; 0      f (  x  + h  v
      ) &#x2212; f (  x  )  h   .   {\displaystyle \nabla _{\mathbf {v} }{f}
      (\mathbf {x} )=\lim _{h\rightarrow 0}{\frac {f(\mathbf {x} +h\mathbf {v}
      )-f(\mathbf {x} )}{h}}.}  [{\displaystyle \nabla _{\mathbf {v} }{f}
      (\mathbf {x} )=\lim _{h\rightarrow 0}{\frac {f(\mathbf {x} +h\mathbf {v}
      )-f(\mathbf {x} )}{h}}.}]
This definition is valid in a broad range of contexts, for example where the
norm of a vector (and hence a unit vector) is undefined.[2]
If the function f is differentiable at x, then the directional derivative
exists along any vector v, and one has
          &#x2207;   v     f  (  x  ) = &#x2207; f (  x  ) &#x22C5;  v
      {\displaystyle \nabla _{\mathbf {v} }{f}(\mathbf {x} )=\nabla f(\mathbf
      {x} )\cdot \mathbf {v} }  [{\displaystyle \nabla _{\mathbf {v} }{f}
      (\mathbf {x} )=\nabla f(\mathbf {x} )\cdot \mathbf {v} }]
where the     &#x2207;   {\displaystyle \nabla }  [\nabla ] on the right
denotes the gradient and     &#x22C5;   {\displaystyle \cdot }  [\cdot ] is the
dot_product.[3] This follows from defining a path     h ( t ) = x + t v
{\displaystyle h(t)=x+tv}  [{\displaystyle h(t)=x+tv}] and using the definition
of the derivative as a limit which can be calculated along this path to get:
             0 =  lim  t &#x2192; 0      f ( x + t v ) &#x2212; f ( x )
      &#x2212; t &#x2217;  D  f   ( x ) ( v )  t   =  lim  t &#x2192; 0      f
      ( x + t v ) &#x2212; f ( x )  t   &#x2212;  D  f   ( x ) ( v ) =
      &#x2207;  v   f ( x ) &#x2212;  D  f   ( x ) ( v )     &#x2192; &#x2207;
      f (  x  ) &#x22C5;  v  =  D  f   ( x ) ( v ) =  &#x2207;   v     f  (  x
      )       {\displaystyle {\begin{aligned}0=\lim _{t\rightarrow 0}{\frac {f
      (x+tv)-f(x)-t*D_{f}(x)(v)}{t}}=\lim _{t\rightarrow 0}{\frac {f(x+tv)-f
      (x)}{t}}-D_{f}(x)(v)=\nabla _{v}f(x)-D_{f}(x)(v)\\\rightarrow \nabla f
      (\mathbf {x} )\cdot \mathbf {v} =D_{f}(x)(v)=\nabla _{\mathbf {v} }{f}
      (\mathbf {x} )\end{aligned}}}  [{\displaystyle {\begin{aligned}0=\lim _
      {t\rightarrow 0}{\frac {f(x+tv)-f(x)-t*D_{f}(x)(v)}{t}}=\lim _
      {t\rightarrow 0}{\frac {f(x+tv)-f(x)}{t}}-D_{f}(x)(v)=\nabla _{v}f(x)-D_
      {f}(x)(v)\\\rightarrow \nabla f(\mathbf {x} )\cdot \mathbf {v} =D_{f}(x)
      (v)=\nabla _{\mathbf {v} }{f}(\mathbf {x} )\end{aligned}}}]
Intuitively, the directional derivative of f at a point x represents the rate
of_change of f, in the direction of v with respect to time, when moving past x.
**** Using only direction of vector[edit] ****
The angle Î± between the tangent A and the horizontal will be maximum if the
cutting plane contains the direction of the gradient A.
In a Euclidean_space, some authors[4] define the directional derivative to be
with respect to an arbitrary nonzero vector v after normalization, thus being
independent of its magnitude and depending only on its direction.[5]
This definition gives the rate of increase of f per unit of distance moved in
the direction given by v. In this case, one has
          &#x2207;   v     f  (  x  ) =  lim  h &#x2192; 0      f (  x  + h  v
      ) &#x2212; f (  x  )   h  |   v   |     ,   {\displaystyle \nabla _
      {\mathbf {v} }{f}(\mathbf {x} )=\lim _{h\rightarrow 0}{\frac {f(\mathbf
      {x} +h\mathbf {v} )-f(\mathbf {x} )}{h|\mathbf {v} |}},}  [{\displaystyle
      \nabla _{\mathbf {v} }{f}(\mathbf {x} )=\lim _{h\rightarrow 0}{\frac {f
      (\mathbf {x} +h\mathbf {v} )-f(\mathbf {x} )}{h|\mathbf {v} |}},}]
or in case f is differentiable at x,
          &#x2207;   v     f  (  x  ) = &#x2207; f (  x  ) &#x22C5;    v    |
      v   |     .   {\displaystyle \nabla _{\mathbf {v} }{f}(\mathbf {x}
      )=\nabla f(\mathbf {x} )\cdot {\frac {\mathbf {v} }{|\mathbf {v} |}}.}  [
      {\displaystyle \nabla _{\mathbf {v} }{f}(\mathbf {x} )=\nabla f(\mathbf
      {x} )\cdot {\frac {\mathbf {v} }{|\mathbf {v} |}}.}]
**** Restriction to a unit vector[edit] ****
In the context of a function on a Euclidean_space, some texts restrict the
vector v to being a unit_vector. With this restriction, both the above
definitions are equivalent.[6]
***** Properties[edit] *****
Many of the familiar properties of the ordinary derivative hold for the
directional derivative. These include, for any functions f and g defined in a
neighborhood of, and differentiable at, p:
   1. sum_rule:
                &#x2207;   v    ( f + g ) =  &#x2207;   v    f +  &#x2207;   v
            g .   {\displaystyle \nabla _{\mathbf {v} }(f+g)=\nabla _{\mathbf
            {v} }f+\nabla _{\mathbf {v} }g.}  [{\displaystyle \nabla _{\mathbf
            {v} }(f+g)=\nabla _{\mathbf {v} }f+\nabla _{\mathbf {v} }g.}]
   2. constant_factor_rule: For any constant c,
   3.     &#x2207;   v    ( c f ) = c  &#x2207;   v    f .   {\displaystyle
      \nabla _{\mathbf {v} }(cf)=c\nabla _{\mathbf {v} }f.}  [{\displaystyle
      \nabla _{\mathbf {v} }(cf)=c\nabla _{\mathbf {v} }f.}]
   4. product_rule (or Leibniz's rule):
   5.     &#x2207;   v    ( f g ) = g  &#x2207;   v    f + f  &#x2207;   v    g
      .   {\displaystyle \nabla _{\mathbf {v} }(fg)=g\nabla _{\mathbf {v}
      }f+f\nabla _{\mathbf {v} }g.}  [{\displaystyle \nabla _{\mathbf {v} }
      (fg)=g\nabla _{\mathbf {v} }f+f\nabla _{\mathbf {v} }g.}]
   6. chain_rule: If g is differentiable at p and h is differentiable at g(p),
      then
   7.     &#x2207;   v    ( h &#x2218; g ) (  p  ) =  h &#x2032;  ( g (  p  ) )
      &#x2207;   v    g (  p  ) .   {\displaystyle \nabla _{\mathbf {v} }
      (h\circ g)(\mathbf {p} )=h'(g(\mathbf {p} ))\nabla _{\mathbf {v} }g
      (\mathbf {p} ).}  [{\displaystyle \nabla _{\mathbf {v} }(h\circ g)
      (\mathbf {p} )=h'(g(\mathbf {p} ))\nabla _{\mathbf {v} }g(\mathbf {p}
      ).}]
***** In differential geometry[edit] *****
See also: Tangent_space_Â§ Tangent_vectors_as_directional_derivatives
Let M be a differentiable_manifold and p a point of M. Suppose that f is a
function defined in a neighborhood of p, and differentiable at p. If v is a
tangent_vector to M at p, then the directional derivative of f along v, denoted
variously as df(v) (see Exterior_derivative),      &#x2207;   v    f (  p  )
{\displaystyle \nabla _{\mathbf {v} }f(\mathbf {p} )}  [{\displaystyle \nabla _
{\mathbf {v} }f(\mathbf {p} )}] (see Covariant_derivative),      L   v    f
(  p  )   {\displaystyle L_{\mathbf {v} }f(\mathbf {p} )}  [{\displaystyle L_
{\mathbf {v} }f(\mathbf {p} )}] (see Lie_derivative), or        v     p    ( f
)   {\displaystyle {\mathbf {v} }_{\mathbf {p} }(f)}  [{\displaystyle {\mathbf
{v} }_{\mathbf {p} }(f)}] (see Tangent_space_Â§ Definition_via_derivations),
can be defined as follows. Let Î³ : [â1, 1] â M be a differentiable curve
with Î³(0) = p and Î³â²(0) = v. Then the directional derivative is defined by
          &#x2207;   v    f (  p  ) =       d  d &#x03C4;    f &#x2218;
      &#x03B3; ( &#x03C4; )  |   &#x03C4; = 0   .   {\displaystyle \nabla _
      {\mathbf {v} }f(\mathbf {p} )=\left.{\frac {d}{d\tau }}f\circ \gamma
      (\tau )\right|_{\tau =0}.}  [{\displaystyle \nabla _{\mathbf {v} }f
      (\mathbf {p} )=\left.{\frac {d}{d\tau }}f\circ \gamma (\tau )\right|_
      {\tau =0}.}]
This definition can be proven independent of the choice of Î³, provided Î³ is
selected in the prescribed manner so that Î³â²(0) = v.
**** The Lie derivative[edit] ****
The Lie_derivative of a vector field       W  &#x03BC;   ( x )
{\displaystyle \scriptstyle W^{\mu }(x)}  [\scriptstyle W^\mu(x)] along a
vector field       V  &#x03BC;   ( x )    {\displaystyle \scriptstyle V^{\mu }
(x)}  [\scriptstyle V^\mu(x)] is given by the difference of two directional
derivatives (with vanishing torsion):
            L    V    W  &#x03BC;   = ( V &#x22C5; &#x2207; )  W  &#x03BC;
      &#x2212; ( W &#x22C5; &#x2207; )  V  &#x03BC;   .   {\displaystyle
      {\mathcal {L}}_{V}W^{\mu }=(V\cdot \nabla )W^{\mu }-(W\cdot \nabla )V^
      {\mu }.}  [{\displaystyle {\mathcal {L}}_{V}W^{\mu }=(V\cdot \nabla )W^
      {\mu }-(W\cdot \nabla )V^{\mu }.}]
In particular, for a scalar field      &#x03D5; ( x )    {\displaystyle
\scriptstyle \phi (x)}  [\scriptstyle \phi(x)], the Lie derivative reduces to
the standard directional derivative:
            L    V   &#x03D5; = ( V &#x22C5; &#x2207; ) &#x03D5; .
      {\displaystyle {\mathcal {L}}_{V}\phi =(V\cdot \nabla )\phi .}  [
      {\displaystyle {\mathcal {L}}_{V}\phi =(V\cdot \nabla )\phi .}]
**** The Riemann tensor[edit] ****
Directional derivatives are often used in introductory derivations of the
Riemann_curvature_tensor. Consider a curved rectangle with an infinitesimal
vector Î´ along one edge and Î´â² along the other. We translate a covector S
along Î´ then Î´â² and then subtract the translation along Î´â² and then Î´.
Instead of building the directional derivative using partial derivatives, we
use the covariant_derivative. The translation operator for Î´ is thus
         1 +  &#x2211;  &#x03BD;    &#x03B4;  &#x03BD;    D  &#x03BD;   = 1 +
      &#x03B4; &#x22C5; D ,   {\displaystyle 1+\sum _{\nu }\delta ^{\nu }D_{\nu
      }=1+\delta \cdot D,}  [{\displaystyle 1+\sum _{\nu }\delta ^{\nu }D_{\nu
      }=1+\delta \cdot D,}]
and for Î´â²,
         1 +  &#x2211;  &#x03BC;    &#x03B4;  &#x2032;  &#x03BC;     D
      &#x03BC;   = 1 +  &#x03B4; &#x2032;  &#x22C5; D .   {\displaystyle 1+\sum
      _{\mu }\delta '^{\mu }D_{\mu }=1+\delta '\cdot D.}  [{\displaystyle
      1+\sum _{\mu }\delta '^{\mu }D_{\mu }=1+\delta '\cdot D.}]
The difference between the two paths is then
         ( 1 +  &#x03B4; &#x2032;  &#x22C5; D ) ( 1 + &#x03B4; &#x22C5; D )  S
      &#x03C1;   &#x2212; ( 1 + &#x03B4; &#x22C5; D ) ( 1 +  &#x03B4; &#x2032;
      &#x22C5; D )  S  &#x03C1;   =  &#x2211;  &#x03BC; , &#x03BD;    &#x03B4;
      &#x2032;  &#x03BC;     &#x03B4;  &#x03BD;   [  D  &#x03BC;   ,  D
      &#x03BD;   ]  S  &#x03C1;   .   {\displaystyle (1+\delta '\cdot D)
      (1+\delta \cdot D)S^{\rho }-(1+\delta \cdot D)(1+\delta '\cdot D)S^{\rho
      }=\sum _{\mu ,\nu }\delta '^{\mu }\delta ^{\nu }[D_{\mu },D_{\nu }]S_
      {\rho }.}  [{\displaystyle (1+\delta '\cdot D)(1+\delta \cdot D)S^{\rho
      }-(1+\delta \cdot D)(1+\delta '\cdot D)S^{\rho }=\sum _{\mu ,\nu }\delta
      '^{\mu }\delta ^{\nu }[D_{\mu },D_{\nu }]S_{\rho }.}]
It can be argued[7] that the noncommutativity of the covariant derivatives
measures the curvature of the manifold:
         [  D  &#x03BC;   ,  D  &#x03BD;   ]  S  &#x03C1;   = &#x00B1;
      &#x2211;  &#x03C3;    R  &#x03C3;       &#x03C1; &#x03BC; &#x03BD;    S
      &#x03C3;   ,   {\displaystyle [D_{\mu },D_{\nu }]S_{\rho }=\pm \sum _
      {\sigma }R^{\sigma }{}_{\rho \mu \nu }S_{\sigma },}  [{\displaystyle [D_
      {\mu },D_{\nu }]S_{\rho }=\pm \sum _{\sigma }R^{\sigma }{}_{\rho \mu \nu
      }S_{\sigma },}]
where R is the Riemann curvature tensor and the sign depends on the sign
convention of the author.
***** In group theory[edit] *****
**** Translations[edit] ****
In the PoincarÃ©_algebra, we can define an infinitesimal translation operator P
as
          P  = i &#x2207; .   {\displaystyle \mathbf {P} =i\nabla .}  [
      {\displaystyle \mathbf {P} =i\nabla .}]
(the i ensures that P is a self-adjoint_operator) For a finite displacement Î»,
the unitary Hilbert_space representation for translations is[8]
         U (  &#x03BB;  ) = exp &#x2061;  (  &#x2212; i  &#x03BB;  &#x22C5;  P
      )  .   {\displaystyle U(\mathbf {\lambda } )=\exp \left(-i\mathbf
      {\lambda } \cdot \mathbf {P} \right).}  [{\displaystyle U(\mathbf
      {\lambda } )=\exp \left(-i\mathbf {\lambda } \cdot \mathbf {P} \right).}]
By using the above definition of the infinitesimal translation operator, we see
that the finite translation operator is an exponentiated directional
derivative:
         U (  &#x03BB;  ) = exp &#x2061;  (   &#x03BB;  &#x22C5; &#x2207;  )  .
      {\displaystyle U(\mathbf {\lambda } )=\exp \left(\mathbf {\lambda } \cdot
      \nabla \right).}  [{\displaystyle U(\mathbf {\lambda } )=\exp \left
      (\mathbf {\lambda } \cdot \nabla \right).}]
This is a translation operator in the sense that it acts on multivariable
functions f(x) as
         U (  &#x03BB;  ) f (  x  ) = exp &#x2061;  (   &#x03BB;  &#x22C5;
      &#x2207;  )  f (  x  ) = f (  x  +  &#x03BB;  ) .   {\displaystyle U
      (\mathbf {\lambda } )f(\mathbf {x} )=\exp \left(\mathbf {\lambda } \cdot
      \nabla \right)f(\mathbf {x} )=f(\mathbf {x} +\mathbf {\lambda } ).}  [
      {\displaystyle U(\mathbf {\lambda } )f(\mathbf {x} )=\exp \left(\mathbf
      {\lambda } \cdot \nabla \right)f(\mathbf {x} )=f(\mathbf {x} +\mathbf
      {\lambda } ).}]
Proof of the last equation
In standard single-variable calculus, the derivative of a smooth function f(x) is
defined by (for small Îµ)
            d f   d x    =    f ( x + &#x03F5; ) &#x2212; f ( x )  &#x03F5;   .
      {\displaystyle {\frac {df}{dx}}={\frac {f(x+\epsilon )-f(x)}{\epsilon }}.}
      [{\displaystyle {\frac {df}{dx}}={\frac {f(x+\epsilon )-f(x)}{\epsilon }}.}]
This can be rearranged to find f(x+Îµ):
         f ( x + &#x03F5; ) = f ( x ) + &#x03F5;     d f   d x    =  (  1 +
      &#x03F5;    d  d x     )  f ( x ) .   {\displaystyle f(x+\epsilon )=f
      (x)+\epsilon \,{\frac {df}{dx}}=\left(1+\epsilon \,{\frac {d}{dx}}\right)f
      (x).}  [{\displaystyle f(x+\epsilon )=f(x)+\epsilon \,{\frac {df}{dx}}=\left
      (1+\epsilon \,{\frac {d}{dx}}\right)f(x).}]
It follows that     [ 1 + &#x03F5;  ( d  /  d x ) ]   {\displaystyle [1+\epsilon
\,(d/dx)]}  [[1+\epsilon\,(d/dx)] ] is a translation operator. This is instantly
generalized[9] to multivariable functions f(x)
         f (  x  +  &#x03F5;  ) =  (  1 +  &#x03F5;  &#x22C5; &#x2207;  )  f (  x
      ) .   {\displaystyle f(\mathbf {x} +\mathbf {\epsilon } )=\left(1+\mathbf
      {\epsilon } \cdot \nabla \right)f(\mathbf {x} ).}  [{\displaystyle f(\mathbf
      {x} +\mathbf {\epsilon } )=\left(1+\mathbf {\epsilon } \cdot \nabla \right)f
      (\mathbf {x} ).}]
Here      &#x03F5;  &#x22C5; &#x2207;   {\displaystyle \mathbf {\epsilon } \cdot
\nabla }  [{\displaystyle \mathbf {\epsilon } \cdot \nabla }] is the directional
derivative along the infinitesimal displacement Îµ. We have found the
infinitesimal version of the translation operator:
         U (  &#x03F5;  ) = 1 +  &#x03F5;  &#x22C5; &#x2207; .   {\displaystyle U
      (\mathbf {\epsilon } )=1+\mathbf {\epsilon } \cdot \nabla .}  [
      {\displaystyle U(\mathbf {\epsilon } )=1+\mathbf {\epsilon } \cdot \nabla
      .}]
It is evident that the group multiplication law[10] U(g)U(f)=U(gf) takes the form
         U (  a  ) U (  b  ) = U (  a + b  ) .   {\displaystyle U(\mathbf {a} )U
      (\mathbf {b} )=U(\mathbf {a+b} ).}  [{\displaystyle U(\mathbf {a} )U(\mathbf
      {b} )=U(\mathbf {a+b} ).}]
So suppose that we take the finite displacement Î» and divide it into N parts
(Nââ is implied everywhere), so that Î»/N=Îµ. In other words,
          &#x03BB;  = N  &#x03F5;  .   {\displaystyle \mathbf {\lambda } =N\mathbf
      {\epsilon } .}  [{\displaystyle \mathbf {\lambda } =N\mathbf {\epsilon } .}]
Then by applying U(Îµ) N times, we can construct U(Î»):
         [ U (  &#x03F5;  )  ]  N   = U ( N  &#x03F5;  ) = U (  &#x03BB;  ) .
      {\displaystyle [U(\mathbf {\epsilon } )]^{N}=U(N\mathbf {\epsilon } )=U
      (\mathbf {\lambda } ).}  [{\displaystyle [U(\mathbf {\epsilon } )]^{N}=U
      (N\mathbf {\epsilon } )=U(\mathbf {\lambda } ).}]
We can now plug in our above expression for U(Îµ):
         [ U (  &#x03F5;  )  ]  N   =   [  1 +  &#x03F5;  &#x22C5; &#x2207;  ]   N
      =   [  1 +     &#x03BB;  &#x22C5; &#x2207;  N    ]   N   .   {\displaystyle
      [U(\mathbf {\epsilon } )]^{N}=\left[1+\mathbf {\epsilon } \cdot \nabla
      \right]^{N}=\left[1+{\frac {\mathbf {\lambda } \cdot \nabla }{N}}\right]^
      {N}.}  [{\displaystyle [U(\mathbf {\epsilon } )]^{N}=\left[1+\mathbf
      {\epsilon } \cdot \nabla \right]^{N}=\left[1+{\frac {\mathbf {\lambda }
      \cdot \nabla }{N}}\right]^{N}.}]
Using the identity[11]
         exp &#x2061; ( x ) =   [  1 +   x N    ]   N   ,   {\displaystyle \exp
      (x)=\left[1+{\frac {x}{N}}\right]^{N},}  [{\displaystyle \exp(x)=\left[1+
      {\frac {x}{N}}\right]^{N},}]
we have
         U (  &#x03BB;  ) = exp &#x2061;  (   &#x03BB;  &#x22C5; &#x2207;  )  .
      {\displaystyle U(\mathbf {\lambda } )=\exp \left(\mathbf {\lambda } \cdot
      \nabla \right).}  [{\displaystyle U(\mathbf {\lambda } )=\exp \left(\mathbf
      {\lambda } \cdot \nabla \right).}]
And since U(Îµ)f(x)=f(x+Îµ) we have
         [ U (  &#x03F5;  )  ]  N   f (  x  ) = f (  x  + N  &#x03F5;  ) = f (  x
      +  &#x03BB;  ) = U (  &#x03BB;  ) f (  x  ) = exp &#x2061;  (   &#x03BB;
      &#x22C5; &#x2207;  )  f (  x  ) ,   {\displaystyle [U(\mathbf {\epsilon }
      )]^{N}f(\mathbf {x} )=f(\mathbf {x} +N\mathbf {\epsilon } )=f(\mathbf {x}
      +\mathbf {\lambda } )=U(\mathbf {\lambda } )f(\mathbf {x} )=\exp \left
      (\mathbf {\lambda } \cdot \nabla \right)f(\mathbf {x} ),}  [{\displaystyle
      [U(\mathbf {\epsilon } )]^{N}f(\mathbf {x} )=f(\mathbf {x} +N\mathbf
      {\epsilon } )=f(\mathbf {x} +\mathbf {\lambda } )=U(\mathbf {\lambda } )f
      (\mathbf {x} )=\exp \left(\mathbf {\lambda } \cdot \nabla \right)f(\mathbf
      {x} ),}]
Q.E.D.
As a technical note, this procedure is only possible because the translation group
forms an Abelian subgroup (Cartan_subalgebra) in the PoincarÃ© algebra. In
particular, the group multiplication law U(a)U(b)=U(a+b) should not be taken for
granted. We also note that PoincarÃ© is a connected Lie group. It is a group of
transformations T(Î¾) that are described by a continuous set of real parameters
&#x03BE;  a      {\displaystyle \scriptstyle \xi ^{a}}  [\scriptstyle \xi^a]. The
group multiplication law takes the form
         T (    &#x03BE; &#x00AF;    ) T ( &#x03BE; ) = T ( f (    &#x03BE;
      &#x00AF;    , &#x03BE; ) ) .   {\displaystyle T({\bar {\xi }})T(\xi )=T(f(
      {\bar {\xi }},\xi )).}  [{\displaystyle T({\bar {\xi }})T(\xi )=T(f({\bar
      {\xi }},\xi )).}]
Taking       &#x03BE;  a      {\displaystyle \scriptstyle \xi ^{a}}  [\scriptstyle
\xi^a]=0 as the coordinates of the identity, we must have
          f  a   ( &#x03BE; , 0 ) =  f  a   ( 0 , &#x03BE; ) =  &#x03BE;  a   .
      {\displaystyle f^{a}(\xi ,0)=f^{a}(0,\xi )=\xi ^{a}.}  [{\displaystyle f^{a}
      (\xi ,0)=f^{a}(0,\xi )=\xi ^{a}.}]
The actual operators on the Hilbert space are represented by unitary operators U(T
(Î¾)). In the above notation we suppressed the T; we now write U(Î») as U(P(Î»)).
For a small neighborhood around the identity, the power series representation
         U ( T ( &#x03BE; ) ) = 1 + i  &#x2211;  a    &#x03BE;  a    t  a   +   1
      2    &#x2211;  b , c    &#x03BE;  b    &#x03BE;  c    t  b c   + &#x22EF;
      {\displaystyle U(T(\xi ))=1+i\sum _{a}\xi ^{a}t_{a}+{\frac {1}{2}}\sum _
      {b,c}\xi ^{b}\xi ^{c}t_{bc}+\cdots }  [U(T(\xi))=1+i\sum_a\xi^a t_a+\frac{1}
      {2}\sum_{b,c}\xi^b\xi^c t_{bc}+\cdots]
is quite good. Suppose that U(T(Î¾)) form a non-projective representation, i.e.
that
         U ( T (    &#x03BE; &#x00AF;    ) ) U ( T ( &#x03BE; ) ) = U ( T ( f
      (    &#x03BE; &#x00AF;    , &#x03BE; ) ) ) .   {\displaystyle U(T({\bar {\xi
      }}))U(T(\xi ))=U(T(f({\bar {\xi }},\xi ))).}  [{\displaystyle U(T({\bar {\xi
      }}))U(T(\xi ))=U(T(f({\bar {\xi }},\xi ))).}]
The expansion of f to second power is
          f  a   (    &#x03BE; &#x00AF;    , &#x03BE; ) =  &#x03BE;  a   +
      &#x03BE; &#x00AF;     a   +  &#x2211;  b , c    f  a b c       &#x03BE;
      &#x00AF;     b    &#x03BE;  c   .   {\displaystyle f^{a}({\bar {\xi }},\xi
      )=\xi ^{a}+{\bar {\xi }}^{a}+\sum _{b,c}f^{abc}{\bar {\xi }}^{b}\xi ^{c}.}
      [{\displaystyle f^{a}({\bar {\xi }},\xi )=\xi ^{a}+{\bar {\xi }}^{a}+\sum _
      {b,c}f^{abc}{\bar {\xi }}^{b}\xi ^{c}.}]
After expanding the representation multiplication equation and equating
coefficients, we have the nontrivial condition
          t  b c   = &#x2212;  t  b    t  c   &#x2212; i  &#x2211;  a    f  a b c
      t  a   .   {\displaystyle t_{bc}=-t_{b}t_{c}-i\sum _{a}f^{abc}t_{a}.}  [
      {\displaystyle t_{bc}=-t_{b}t_{c}-i\sum _{a}f^{abc}t_{a}.}]
Since       t  a b      {\displaystyle \scriptstyle t_{ab}}  [\scriptstyle t_{ab}]
is by definition symmetric in its indices, we have the standard Lie_algebra
commutator:
         [  t  b   ,  t  c   ] = i  &#x2211;  a   ( &#x2212;  f  a b c   +  f  a c
      b   )  t  a   = i  &#x2211;  a    C  a b c    t  a   ,   {\displaystyle [t_
      {b},t_{c}]=i\sum _{a}(-f^{abc}+f^{acb})t_{a}=i\sum _{a}C^{abc}t_{a},}  [
      {\displaystyle [t_{b},t_{c}]=i\sum _{a}(-f^{abc}+f^{acb})t_{a}=i\sum _{a}C^
      {abc}t_{a},}]
with C the structure_constant. The generators for translations are partial
derivative operators, which commute:
          [    &#x2202;  &#x2202;  x  b      ,   &#x2202;  &#x2202;  x  c       ]
      = 0.   {\displaystyle \left[{\frac {\partial }{\partial x^{b}}},{\frac
      {\partial }{\partial x^{c}}}\right]=0.}  [{\displaystyle \left[{\frac
      {\partial }{\partial x^{b}}},{\frac {\partial }{\partial x^{c}}}\right]=0.}]
This implies that the structure constants vanish and thus the quadratic
coefficients in the f expansion vanish as well. This means that f is simply
additive:
          f  abelian   a   (    &#x03BE; &#x00AF;    , &#x03BE; ) =  &#x03BE;  a
      +     &#x03BE; &#x00AF;     a   ,   {\displaystyle f_{\text{abelian}}^{a}(
      {\bar {\xi }},\xi )=\xi ^{a}+{\bar {\xi }}^{a},}  [{\displaystyle f_{\text
      {abelian}}^{a}({\bar {\xi }},\xi )=\xi ^{a}+{\bar {\xi }}^{a},}]
and thus for abelian groups,
         U ( T (    &#x03BE; &#x00AF;    ) ) U ( T ( &#x03BE; ) ) = U ( T
      (    &#x03BE; &#x00AF;    + &#x03BE; ) ) .   {\displaystyle U(T({\bar {\xi
      }}))U(T(\xi ))=U(T({\bar {\xi }}+\xi )).}  [{\displaystyle U(T({\bar {\xi
      }}))U(T(\xi ))=U(T({\bar {\xi }}+\xi )).}]
Q.E.D.
**** Rotations[edit] ****
The rotation_operator also contains a directional derivative. The rotation
operator for an angle Î¸, i.e. by an amount Î¸=|Î¸| about an axis parallel to
&#x03B8; &#x005E;       {\displaystyle \scriptstyle {\hat {\theta }}}
[\scriptstyle \hat{\theta}]=Î¸/Î¸ is
         U ( R (  &#x03B8;  ) ) = exp &#x2061; ( &#x2212; i  &#x03B8;  &#x22C5;
      L  ) .   {\displaystyle U(R(\mathbf {\theta } ))=\exp(-i\mathbf {\theta }
      \cdot \mathbf {L} ).}  [{\displaystyle U(R(\mathbf {\theta } ))=\exp(-
      i\mathbf {\theta } \cdot \mathbf {L} ).}]
Here L is the vector operator that generates SO(3):
          L  =   (    0   0   0     0   0   1     0   &#x2212; 1   0    )    i
      +   (    0   0   &#x2212; 1     0   0   0     1   0   0    )    j  +
      (    0   1   0     &#x2212; 1   0   0     0   0   0    )    k  .
      {\displaystyle \mathbf {L} ={\begin{pmatrix}0&0&0\\0&0&1\\0&-1&0\end
      {pmatrix}}\mathbf {i} +{\begin{pmatrix}0&0&-1\\0&0&0\\1&0&0\end
      {pmatrix}}\mathbf {j} +{\begin{pmatrix}0&1&0\\-1&0&0\\0&0&0\end
      {pmatrix}}\mathbf {k} .}  [{\displaystyle \mathbf {L} ={\begin
      {pmatrix}0&0&0\\0&0&1\\0&-1&0\end{pmatrix}}\mathbf {i} +{\begin
      {pmatrix}0&0&-1\\0&0&0\\1&0&0\end{pmatrix}}\mathbf {j} +{\begin
      {pmatrix}0&1&0\\-1&0&0\\0&0&0\end{pmatrix}}\mathbf {k} .}]
It may be shown geometrically that an infinitesimal right-handed rotation
changes the position vector x by
          x  &#x2192;  x  &#x2212; &#x03B4;  &#x03B8;  &#x00D7;  x  .
      {\displaystyle \mathbf {x} \rightarrow \mathbf {x} -\delta \mathbf
      {\theta } \times \mathbf {x} .}  [{\displaystyle \mathbf {x} \rightarrow
      \mathbf {x} -\delta \mathbf {\theta } \times \mathbf {x} .}]
So we would expect under infinitesimal rotation:
         U ( R ( &#x03B4;  &#x03B8;  ) ) f (  x  ) = f (  x  &#x2212; &#x03B4;
      &#x03B8;  &#x00D7;  x  ) = f (  x  ) &#x2212; ( &#x03B4;  &#x03B8;
      &#x00D7;  x  ) &#x22C5; &#x2207; f .   {\displaystyle U(R(\delta \mathbf
      {\theta } ))f(\mathbf {x} )=f(\mathbf {x} -\delta \mathbf {\theta }
      \times \mathbf {x} )=f(\mathbf {x} )-(\delta \mathbf {\theta } \times
      \mathbf {x} )\cdot \nabla f.}  [{\displaystyle U(R(\delta \mathbf {\theta
      } ))f(\mathbf {x} )=f(\mathbf {x} -\delta \mathbf {\theta } \times
      \mathbf {x} )=f(\mathbf {x} )-(\delta \mathbf {\theta } \times \mathbf
      {x} )\cdot \nabla f.}]
It follows that
         U ( R ( &#x03B4;  &#x03B8;  ) ) = 1 &#x2212; ( &#x03B4;  &#x03B8;
      &#x00D7;  x  ) &#x22C5; &#x2207; .   {\displaystyle U(R(\delta \mathbf
      {\theta } ))=1-(\delta \mathbf {\theta } \times \mathbf {x} )\cdot \nabla
      .}  [{\displaystyle U(R(\delta \mathbf {\theta } ))=1-(\delta \mathbf
      {\theta } \times \mathbf {x} )\cdot \nabla .}]
Following the same exponentiation procedure as above, we arrive at the rotation
operator in the position basis, which is an exponentiated directional
derivative:[12]
         U ( R (  &#x03B8;  ) ) = exp &#x2061; ( &#x2212; (  &#x03B8;  &#x00D7;
      x  ) &#x22C5; &#x2207; ) .   {\displaystyle U(R(\mathbf {\theta } ))=\exp
      (-(\mathbf {\theta } \times \mathbf {x} )\cdot \nabla ).}  [
      {\displaystyle U(R(\mathbf {\theta } ))=\exp(-(\mathbf {\theta } \times
      \mathbf {x} )\cdot \nabla ).}]
***** Normal derivative[edit] *****
A normal derivative is a directional derivative taken in the direction normal
(that is, orthogonal) to some surface in space, or more generally along a
normal_vector field orthogonal to some hypersurface. See for example Neumann
boundary_condition. If the normal direction is denoted by      n
{\displaystyle \mathbf {n} }  [\mathbf {n} ], then the directional derivative
of a function f is sometimes denoted as        &#x2202; f   &#x2202; n
{\displaystyle {\frac {\partial f}{\partial n}}}  [\frac{ \partial f}{\partial
n}]. In other notations,
            &#x2202; f   &#x2202;  n     = &#x2207; f (  x  ) &#x22C5;  n  =
      &#x2207;   n     f  (  x  ) =    &#x2202; f   &#x2202;  x     &#x22C5;  n
      = D f (  x  ) [  n  ] .   {\displaystyle {\frac {\partial f}{\partial
      \mathbf {n} }}=\nabla f(\mathbf {x} )\cdot \mathbf {n} =\nabla _{\mathbf
      {n} }{f}(\mathbf {x} )={\frac {\partial f}{\partial \mathbf {x} }}\cdot
      \mathbf {n} =Df(\mathbf {x} )[\mathbf {n} ].}  [{\displaystyle {\frac
      {\partial f}{\partial \mathbf {n} }}=\nabla f(\mathbf {x} )\cdot \mathbf
      {n} =\nabla _{\mathbf {n} }{f}(\mathbf {x} )={\frac {\partial f}{\partial
      \mathbf {x} }}\cdot \mathbf {n} =Df(\mathbf {x} )[\mathbf {n} ].}]
***** In the continuum mechanics of solids[edit] *****
Several important results in continuum mechanics require the derivatives of
vectors with respect to vectors and of tensors with respect to vectors and
tensors.[13] The directional directive provides a systematic way of finding
these derivatives.
The definitions of directional derivatives for various situations are given
below. It is assumed that the functions are sufficiently smooth that
derivatives can be taken.
**** Derivatives of scalar-valued functions of vectors[edit] ****
Let     f (  v  )   {\displaystyle f(\mathbf {v} )}  [f(\mathbf{v})] be a real-
valued function of the vector      v    {\displaystyle \mathbf {v} }  [\mathbf
{v} ]. Then the derivative of     f (  v  )   {\displaystyle f(\mathbf {v} )}
[f(\mathbf{v})] with respect to      v    {\displaystyle \mathbf {v} }
[\mathbf {v} ] (or at      v    {\displaystyle \mathbf {v} }  [\mathbf {v} ])
in the direction      u    {\displaystyle \mathbf {u} }  [\mathbf {u} ] is
defined as
            &#x2202; f   &#x2202;  v     &#x22C5;  u  = D f (  v  ) [  u  ] =
      [    d  d &#x03B1;    &#xA0; f (  v  + &#x03B1; &#xA0;  u  )  ]
      &#x03B1; = 0     {\displaystyle {\frac {\partial f}{\partial \mathbf {v}
      }}\cdot \mathbf {u} =Df(\mathbf {v} )[\mathbf {u} ]=\left[{\frac {d}
      {d\alpha }}~f(\mathbf {v} +\alpha ~\mathbf {u} )\right]_{\alpha =0}}  [
        \frac{\partial f}{\partial \mathbf{v}}\cdot\mathbf{u} = Df(\mathbf{v})
      [\mathbf{u}]
           = \left[\frac{d }{d \alpha}~f(\mathbf{v} + \alpha~\mathbf
      {u})\right]_{\alpha = 0}
      ]
for all vectors      u    {\displaystyle \mathbf {u} }  [\mathbf {u} ].
Properties:
   1. If     f (  v  ) =  f  1   (  v  ) +  f  2   (  v  )   {\displaystyle f
      (\mathbf {v} )=f_{1}(\mathbf {v} )+f_{2}(\mathbf {v} )}  [f(\mathbf{v}) =
      f_1(\mathbf{v}) + f_2(\mathbf{v})] then        &#x2202; f   &#x2202;  v
      &#x22C5;  u  =  (     &#x2202;  f  1     &#x2202;  v     +    &#x2202;  f
      2     &#x2202;  v      )  &#x22C5;  u  .   {\displaystyle {\frac
      {\partial f}{\partial \mathbf {v} }}\cdot \mathbf {u} =\left({\frac
      {\partial f_{1}}{\partial \mathbf {v} }}+{\frac {\partial f_{2}}{\partial
      \mathbf {v} }}\right)\cdot \mathbf {u} .}  [{\displaystyle {\frac
      {\partial f}{\partial \mathbf {v} }}\cdot \mathbf {u} =\left({\frac
      {\partial f_{1}}{\partial \mathbf {v} }}+{\frac {\partial f_{2}}{\partial
      \mathbf {v} }}\right)\cdot \mathbf {u} .}]
   2. If     f (  v  ) =  f  1   (  v  ) &#xA0;  f  2   (  v  )
      {\displaystyle f(\mathbf {v} )=f_{1}(\mathbf {v} )~f_{2}(\mathbf {v} )}
      [f(\mathbf{v}) = f_1(\mathbf{v})~ f_2(\mathbf{v})] then        &#x2202; f
      &#x2202;  v     &#x22C5;  u  =  (     &#x2202;  f  1     &#x2202;  v
      &#x22C5;  u   )  &#xA0;  f  2   (  v  ) +  f  1   (  v  ) &#xA0;
      (     &#x2202;  f  2     &#x2202;  v     &#x22C5;  u   )  .
      {\displaystyle {\frac {\partial f}{\partial \mathbf {v} }}\cdot \mathbf
      {u} =\left({\frac {\partial f_{1}}{\partial \mathbf {v} }}\cdot \mathbf
      {u} \right)~f_{2}(\mathbf {v} )+f_{1}(\mathbf {v} )~\left({\frac
      {\partial f_{2}}{\partial \mathbf {v} }}\cdot \mathbf {u} \right).}  [
      {\displaystyle {\frac {\partial f}{\partial \mathbf {v} }}\cdot \mathbf
      {u} =\left({\frac {\partial f_{1}}{\partial \mathbf {v} }}\cdot \mathbf
      {u} \right)~f_{2}(\mathbf {v} )+f_{1}(\mathbf {v} )~\left({\frac
      {\partial f_{2}}{\partial \mathbf {v} }}\cdot \mathbf {u} \right).}]
   3. If     f (  v  ) =  f  1   (  f  2   (  v  ) )   {\displaystyle f(\mathbf
      {v} )=f_{1}(f_{2}(\mathbf {v} ))}  [f(\mathbf{v}) = f_1(f_2(\mathbf{v}))]
      then        &#x2202; f   &#x2202;  v     &#x22C5;  u  =    &#x2202;  f  1
      &#x2202;  f  2      &#xA0;    &#x2202;  f  2     &#x2202;  v     &#x22C5;
      u  .   {\displaystyle {\frac {\partial f}{\partial \mathbf {v} }}\cdot
      \mathbf {u} ={\frac {\partial f_{1}}{\partial f_{2}}}~{\frac {\partial f_
      {2}}{\partial \mathbf {v} }}\cdot \mathbf {u} .}  [{\displaystyle {\frac
      {\partial f}{\partial \mathbf {v} }}\cdot \mathbf {u} ={\frac {\partial
      f_{1}}{\partial f_{2}}}~{\frac {\partial f_{2}}{\partial \mathbf {v}
      }}\cdot \mathbf {u} .}]
**** Derivatives of vector-valued functions of vectors[edit] ****
Let      f  (  v  )   {\displaystyle \mathbf {f} (\mathbf {v} )}  [\mathbf{f}
(\mathbf{v})] be a vector-valued function of the vector      v
{\displaystyle \mathbf {v} }  [\mathbf {v} ]. Then the derivative of      f
(  v  )   {\displaystyle \mathbf {f} (\mathbf {v} )}  [\mathbf{f}(\mathbf{v})]
with respect to      v    {\displaystyle \mathbf {v} }  [\mathbf {v} ] (or at
v    {\displaystyle \mathbf {v} }  [\mathbf {v} ]) in the direction      u
{\displaystyle \mathbf {u} }  [\mathbf {u} ] is the second-order tensor defined
as
            &#x2202;  f    &#x2202;  v     &#x22C5;  u  = D  f  (  v  ) [  u  ]
      =   [    d  d &#x03B1;    &#xA0;  f  (  v  + &#x03B1; &#xA0;  u  )  ]
      &#x03B1; = 0     {\displaystyle {\frac {\partial \mathbf {f} }{\partial
      \mathbf {v} }}\cdot \mathbf {u} =D\mathbf {f} (\mathbf {v} )[\mathbf {u}
      ]=\left[{\frac {d}{d\alpha }}~\mathbf {f} (\mathbf {v} +\alpha ~\mathbf
      {u} )\right]_{\alpha =0}}  [
        \frac{\partial \mathbf{f}}{\partial \mathbf{v}}\cdot\mathbf{u} =
      D\mathbf{f}(\mathbf{v})[\mathbf{u}]
           = \left[\frac{d }{d \alpha}~\mathbf{f}(\mathbf{v} + \alpha~\mathbf
      {u})\right]_{\alpha = 0}
      ]
for all vectors      u    {\displaystyle \mathbf {u} }  [\mathbf {u} ].
Properties:
   1. If      f  (  v  ) =   f   1   (  v  ) +   f   2   (  v  )
      {\displaystyle \mathbf {f} (\mathbf {v} )=\mathbf {f} _{1}(\mathbf {v}
      )+\mathbf {f} _{2}(\mathbf {v} )}  [\mathbf{f}(\mathbf{v}) = \mathbf{f}_1
      (\mathbf{v}) + \mathbf{f}_2(\mathbf{v})] then        &#x2202;  f
      &#x2202;  v     &#x22C5;  u  =  (     &#x2202;   f   1     &#x2202;  v
      +    &#x2202;   f   2     &#x2202;  v      )  &#x22C5;  u  .
      {\displaystyle {\frac {\partial \mathbf {f} }{\partial \mathbf {v}
      }}\cdot \mathbf {u} =\left({\frac {\partial \mathbf {f} _{1}}{\partial
      \mathbf {v} }}+{\frac {\partial \mathbf {f} _{2}}{\partial \mathbf {v}
      }}\right)\cdot \mathbf {u} .}  [{\displaystyle {\frac {\partial \mathbf
      {f} }{\partial \mathbf {v} }}\cdot \mathbf {u} =\left({\frac {\partial
      \mathbf {f} _{1}}{\partial \mathbf {v} }}+{\frac {\partial \mathbf {f} _
      {2}}{\partial \mathbf {v} }}\right)\cdot \mathbf {u} .}]
   2. If      f  (  v  ) =   f   1   (  v  ) &#x00D7;   f   2   (  v  )
      {\displaystyle \mathbf {f} (\mathbf {v} )=\mathbf {f} _{1}(\mathbf {v}
      )\times \mathbf {f} _{2}(\mathbf {v} )}  [\mathbf{f}(\mathbf{v}) =
      \mathbf{f}_1(\mathbf{v})\times\mathbf{f}_2(\mathbf{v})] then
      &#x2202;  f    &#x2202;  v     &#x22C5;  u  =  (     &#x2202;   f   1
      &#x2202;  v     &#x22C5;  u   )  &#x00D7;   f   2   (  v  ) +   f   1
      (  v  ) &#x00D7;  (     &#x2202;   f   2     &#x2202;  v     &#x22C5;  u
      )  .   {\displaystyle {\frac {\partial \mathbf {f} }{\partial \mathbf {v}
      }}\cdot \mathbf {u} =\left({\frac {\partial \mathbf {f} _{1}}{\partial
      \mathbf {v} }}\cdot \mathbf {u} \right)\times \mathbf {f} _{2}(\mathbf
      {v} )+\mathbf {f} _{1}(\mathbf {v} )\times \left({\frac {\partial \mathbf
      {f} _{2}}{\partial \mathbf {v} }}\cdot \mathbf {u} \right).}  [
      {\displaystyle {\frac {\partial \mathbf {f} }{\partial \mathbf {v}
      }}\cdot \mathbf {u} =\left({\frac {\partial \mathbf {f} _{1}}{\partial
      \mathbf {v} }}\cdot \mathbf {u} \right)\times \mathbf {f} _{2}(\mathbf
      {v} )+\mathbf {f} _{1}(\mathbf {v} )\times \left({\frac {\partial \mathbf
      {f} _{2}}{\partial \mathbf {v} }}\cdot \mathbf {u} \right).}]
   3. If      f  (  v  ) =   f   1   (   f   2   (  v  ) )   {\displaystyle
      \mathbf {f} (\mathbf {v} )=\mathbf {f} _{1}(\mathbf {f} _{2}(\mathbf {v}
      ))}  [\mathbf{f}(\mathbf{v}) = \mathbf{f}_1(\mathbf{f}_2(\mathbf{v}))]
      then        &#x2202;  f    &#x2202;  v     &#x22C5;  u  =    &#x2202;   f
      1     &#x2202;   f   2      &#x22C5;  (     &#x2202;   f   2     &#x2202;
      v     &#x22C5;  u   )  .   {\displaystyle {\frac {\partial \mathbf {f} }
      {\partial \mathbf {v} }}\cdot \mathbf {u} ={\frac {\partial \mathbf {f} _
      {1}}{\partial \mathbf {f} _{2}}}\cdot \left({\frac {\partial \mathbf {f}
      _{2}}{\partial \mathbf {v} }}\cdot \mathbf {u} \right).}  [{\displaystyle
      {\frac {\partial \mathbf {f} }{\partial \mathbf {v} }}\cdot \mathbf {u} =
      {\frac {\partial \mathbf {f} _{1}}{\partial \mathbf {f} _{2}}}\cdot \left
      ({\frac {\partial \mathbf {f} _{2}}{\partial \mathbf {v} }}\cdot \mathbf
      {u} \right).}]
**** Derivatives of scalar-valued functions of second-order tensors[edit] ****
Let     f (  S  )   {\displaystyle f(\mathbf {S} )}  [{\displaystyle f(\mathbf
{S} )}] be a real-valued function of the second order tensor      S
{\displaystyle \mathbf {S} }  [\mathbf {S} ]. Then the derivative of     f (  S
)   {\displaystyle f(\mathbf {S} )}  [{\displaystyle f(\mathbf {S} )}] with
respect to      S    {\displaystyle \mathbf {S} }  [\mathbf {S} ] (or at      S
{\displaystyle \mathbf {S} }  [\mathbf {S} ]) in the direction      T
{\displaystyle \mathbf {T} }  [\mathbf {T} ] is the second order tensor defined
as
            &#x2202; f   &#x2202;  S     :  T  = D f (  S  ) [  T  ] =   [    d
      d &#x03B1;    &#xA0; f (  S  + &#x03B1;  T  )  ]   &#x03B1; = 0
      {\displaystyle {\frac {\partial f}{\partial \mathbf {S} }}:\mathbf {T}
      =Df(\mathbf {S} )[\mathbf {T} ]=\left[{\frac {d}{d\alpha }}~f(\mathbf {S}
      +\alpha \mathbf {T} )\right]_{\alpha =0}}  [{\displaystyle {\frac
      {\partial f}{\partial \mathbf {S} }}:\mathbf {T} =Df(\mathbf {S} )
      [\mathbf {T} ]=\left[{\frac {d}{d\alpha }}~f(\mathbf {S} +\alpha \mathbf
      {T} )\right]_{\alpha =0}}]
for all second order tensors      T    {\displaystyle \mathbf {T} }  [\mathbf
{T} ].
Properties:
   1. If     f (  S  ) =  f  1   (  S  ) +  f  2   (  S  )   {\displaystyle f
      (\mathbf {S} )=f_{1}(\mathbf {S} )+f_{2}(\mathbf {S} )}  [{\displaystyle
      f(\mathbf {S} )=f_{1}(\mathbf {S} )+f_{2}(\mathbf {S} )}] then
      &#x2202; f   &#x2202;  S     :  T  =  (     &#x2202;  f  1     &#x2202;
      S     +    &#x2202;  f  2     &#x2202;  S      )  :  T  .
      {\displaystyle {\frac {\partial f}{\partial \mathbf {S} }}:\mathbf {T}
      =\left({\frac {\partial f_{1}}{\partial \mathbf {S} }}+{\frac {\partial
      f_{2}}{\partial \mathbf {S} }}\right):\mathbf {T} .}  [{\displaystyle
      {\frac {\partial f}{\partial \mathbf {S} }}:\mathbf {T} =\left({\frac
      {\partial f_{1}}{\partial \mathbf {S} }}+{\frac {\partial f_{2}}{\partial
      \mathbf {S} }}\right):\mathbf {T} .}]
   2. If     f (  S  ) =  f  1   (  S  ) &#xA0;  f  2   (  S  )
      {\displaystyle f(\mathbf {S} )=f_{1}(\mathbf {S} )~f_{2}(\mathbf {S} )}
      [{\displaystyle f(\mathbf {S} )=f_{1}(\mathbf {S} )~f_{2}(\mathbf {S} )}]
      then        &#x2202; f   &#x2202;  S     :  T  =  (     &#x2202;  f  1
      &#x2202;  S     :  T   )  &#xA0;  f  2   (  S  ) +  f  1   (  S  ) &#xA0;
      (     &#x2202;  f  2     &#x2202;  S     :  T   )  .   {\displaystyle
      {\frac {\partial f}{\partial \mathbf {S} }}:\mathbf {T} =\left({\frac
      {\partial f_{1}}{\partial \mathbf {S} }}:\mathbf {T} \right)~f_{2}
      (\mathbf {S} )+f_{1}(\mathbf {S} )~\left({\frac {\partial f_{2}}{\partial
      \mathbf {S} }}:\mathbf {T} \right).}  [{\displaystyle {\frac {\partial f}
      {\partial \mathbf {S} }}:\mathbf {T} =\left({\frac {\partial f_{1}}
      {\partial \mathbf {S} }}:\mathbf {T} \right)~f_{2}(\mathbf {S} )+f_{1}
      (\mathbf {S} )~\left({\frac {\partial f_{2}}{\partial \mathbf {S} }}:
      \mathbf {T} \right).}]
   3. If     f (  S  ) =  f  1   (  f  2   (  S  ) )   {\displaystyle f(\mathbf
      {S} )=f_{1}(f_{2}(\mathbf {S} ))}  [{\displaystyle f(\mathbf {S} )=f_{1}
      (f_{2}(\mathbf {S} ))}] then        &#x2202; f   &#x2202;  S     :  T  =
      &#x2202;  f  1     &#x2202;  f  2      &#xA0;  (     &#x2202;  f  2
      &#x2202;  S     :  T   )  .   {\displaystyle {\frac {\partial f}{\partial
      \mathbf {S} }}:\mathbf {T} ={\frac {\partial f_{1}}{\partial f_
      {2}}}~\left({\frac {\partial f_{2}}{\partial \mathbf {S} }}:\mathbf {T}
      \right).}  [{\displaystyle {\frac {\partial f}{\partial \mathbf {S} }}:
      \mathbf {T} ={\frac {\partial f_{1}}{\partial f_{2}}}~\left({\frac
      {\partial f_{2}}{\partial \mathbf {S} }}:\mathbf {T} \right).}]
**** Derivatives of tensor-valued functions of second-order tensors[edit] ****
Let      F  (  S  )   {\displaystyle \mathbf {F} (\mathbf {S} )}  [
{\displaystyle \mathbf {F} (\mathbf {S} )}] be a second order tensor-valued
function of the second order tensor      S    {\displaystyle \mathbf {S} }
[\mathbf {S} ]. Then the derivative of      F  (  S  )   {\displaystyle \mathbf
{F} (\mathbf {S} )}  [{\displaystyle \mathbf {F} (\mathbf {S} )}] with respect
to      S    {\displaystyle \mathbf {S} }  [\mathbf {S} ] (or at      S
{\displaystyle \mathbf {S} }  [\mathbf {S} ]) in the direction      T
{\displaystyle \mathbf {T} }  [\mathbf {T} ] is the fourth order tensor defined
as
            &#x2202;  F    &#x2202;  S     :  T  = D  F  (  S  ) [  T  ] =
      [    d  d &#x03B1;    &#xA0;  F  (  S  + &#x03B1;  T  )  ]   &#x03B1; = 0
      {\displaystyle {\frac {\partial \mathbf {F} }{\partial \mathbf {S} }}:
      \mathbf {T} =D\mathbf {F} (\mathbf {S} )[\mathbf {T} ]=\left[{\frac {d}
      {d\alpha }}~\mathbf {F} (\mathbf {S} +\alpha \mathbf {T} )\right]_{\alpha
      =0}}  [{\displaystyle {\frac {\partial \mathbf {F} }{\partial \mathbf {S}
      }}:\mathbf {T} =D\mathbf {F} (\mathbf {S} )[\mathbf {T} ]=\left[{\frac
      {d}{d\alpha }}~\mathbf {F} (\mathbf {S} +\alpha \mathbf {T} )\right]_
      {\alpha =0}}]
for all second order tensors      T    {\displaystyle \mathbf {T} }  [\mathbf
{T} ].
Properties:
   1. If      F  (  S  ) =   F   1   (  S  ) +   F   2   (  S  )
      {\displaystyle \mathbf {F} (\mathbf {S} )=\mathbf {F} _{1}(\mathbf {S}
      )+\mathbf {F} _{2}(\mathbf {S} )}  [{\displaystyle \mathbf {F} (\mathbf
      {S} )=\mathbf {F} _{1}(\mathbf {S} )+\mathbf {F} _{2}(\mathbf {S} )}]
      then        &#x2202;  F    &#x2202;  S     :  T  =  (     &#x2202;   F
      1     &#x2202;  S     +    &#x2202;   F   2     &#x2202;  S      )  :  T
      .   {\displaystyle {\frac {\partial \mathbf {F} }{\partial \mathbf {S}
      }}:\mathbf {T} =\left({\frac {\partial \mathbf {F} _{1}}{\partial \mathbf
      {S} }}+{\frac {\partial \mathbf {F} _{2}}{\partial \mathbf {S} }}\right):
      \mathbf {T} .}  [{\displaystyle {\frac {\partial \mathbf {F} }{\partial
      \mathbf {S} }}:\mathbf {T} =\left({\frac {\partial \mathbf {F} _{1}}
      {\partial \mathbf {S} }}+{\frac {\partial \mathbf {F} _{2}}{\partial
      \mathbf {S} }}\right):\mathbf {T} .}]
   2. If      F  (  S  ) =   F   1   (  S  ) &#x22C5;   F   2   (  S  )
      {\displaystyle \mathbf {F} (\mathbf {S} )=\mathbf {F} _{1}(\mathbf {S}
      )\cdot \mathbf {F} _{2}(\mathbf {S} )}  [{\displaystyle \mathbf {F}
      (\mathbf {S} )=\mathbf {F} _{1}(\mathbf {S} )\cdot \mathbf {F} _{2}
      (\mathbf {S} )}] then        &#x2202;  F    &#x2202;  S     :  T  =
      (     &#x2202;   F   1     &#x2202;  S     :  T   )  &#x22C5;   F   2
      (  S  ) +   F   1   (  S  ) &#x22C5;  (     &#x2202;   F   2     &#x2202;
      S     :  T   )  .   {\displaystyle {\frac {\partial \mathbf {F} }
      {\partial \mathbf {S} }}:\mathbf {T} =\left({\frac {\partial \mathbf {F}
      _{1}}{\partial \mathbf {S} }}:\mathbf {T} \right)\cdot \mathbf {F} _{2}
      (\mathbf {S} )+\mathbf {F} _{1}(\mathbf {S} )\cdot \left({\frac {\partial
      \mathbf {F} _{2}}{\partial \mathbf {S} }}:\mathbf {T} \right).}  [
      {\displaystyle {\frac {\partial \mathbf {F} }{\partial \mathbf {S} }}:
      \mathbf {T} =\left({\frac {\partial \mathbf {F} _{1}}{\partial \mathbf
      {S} }}:\mathbf {T} \right)\cdot \mathbf {F} _{2}(\mathbf {S} )+\mathbf
      {F} _{1}(\mathbf {S} )\cdot \left({\frac {\partial \mathbf {F} _{2}}
      {\partial \mathbf {S} }}:\mathbf {T} \right).}]
   3. If      F  (  S  ) =   F   1   (   F   2   (  S  ) )   {\displaystyle
      \mathbf {F} (\mathbf {S} )=\mathbf {F} _{1}(\mathbf {F} _{2}(\mathbf {S}
      ))}  [{\displaystyle \mathbf {F} (\mathbf {S} )=\mathbf {F} _{1}(\mathbf
      {F} _{2}(\mathbf {S} ))}] then        &#x2202;  F    &#x2202;  S     :  T
      =    &#x2202;   F   1     &#x2202;   F   2      :  (     &#x2202;   F   2
      &#x2202;  S     :  T   )  .   {\displaystyle {\frac {\partial \mathbf {F}
      }{\partial \mathbf {S} }}:\mathbf {T} ={\frac {\partial \mathbf {F} _{1}}
      {\partial \mathbf {F} _{2}}}:\left({\frac {\partial \mathbf {F} _{2}}
      {\partial \mathbf {S} }}:\mathbf {T} \right).}  [{\displaystyle {\frac
      {\partial \mathbf {F} }{\partial \mathbf {S} }}:\mathbf {T} ={\frac
      {\partial \mathbf {F} _{1}}{\partial \mathbf {F} _{2}}}:\left({\frac
      {\partial \mathbf {F} _{2}}{\partial \mathbf {S} }}:\mathbf {T}
      \right).}]
   4. If     f (  S  ) =  f  1   (   F   2   (  S  ) )   {\displaystyle f
      (\mathbf {S} )=f_{1}(\mathbf {F} _{2}(\mathbf {S} ))}  [{\displaystyle f
      (\mathbf {S} )=f_{1}(\mathbf {F} _{2}(\mathbf {S} ))}] then
      &#x2202; f   &#x2202;  S     :  T  =    &#x2202;  f  1     &#x2202;   F
      2      :  (     &#x2202;   F   2     &#x2202;  S     :  T   )  .
      {\displaystyle {\frac {\partial f}{\partial \mathbf {S} }}:\mathbf {T} =
      {\frac {\partial f_{1}}{\partial \mathbf {F} _{2}}}:\left({\frac
      {\partial \mathbf {F} _{2}}{\partial \mathbf {S} }}:\mathbf {T} \right).}
      [{\displaystyle {\frac {\partial f}{\partial \mathbf {S} }}:\mathbf {T} =
      {\frac {\partial f_{1}}{\partial \mathbf {F} _{2}}}:\left({\frac
      {\partial \mathbf {F} _{2}}{\partial \mathbf {S} }}:\mathbf {T}
      \right).}]
***** See also[edit] *****
    * FrÃ©chet_derivative
    * Gateaux_derivative
    * Derivative_(generalizations)
    * Lie_derivative
    * Differential_form
    * Structure_tensor
    * Tensor_derivative_(continuum_mechanics)
    * Del_in_cylindrical_and_spherical_coordinates
***** Notes[edit] *****
   1. ^R. Wrede; M.R. Spiegel (2010). Advanced Calculus (3rd ed.). Schaum's
      Outline Series. ISBN 978-0-07-162366-7.
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
   3. ^ The applicability extends to functions over spaces without a metric and
      to differentiable_manifolds, such as in general_relativity.
   4. ^ If the dot product is undefined, the gradient is also undefined;
      however, for differentiable f, the directional derivative is still
      defined, and a similar relation exists with the exterior derivative.
   5. ^ Thomas, George B. Jr.; and Finney, Ross L. (1979) Calculus and Analytic
      Geometry, Addison-Wesley Publ. Co., fifth edition, p. 593.
   6. ^ This typically assumes a Euclidean_space â for example, a function of
      several variables typically has no definition of the magnitude of a
      vector, and hence of a unit vector.
   7. ^Hughes-Hallet, Deborah; McCallum, William G.; Gleason, Andrew M. (2012-
      01-01). Calculus :_Single_and_multivariable. John wiley. p. 780.
      ISBN 9780470888612. OCLC 828768012.
   8. ^Zee, A. (2013). Einstein gravity in a nutshell. Princeton: Princeton
      University Press. p. 341. ISBN 9780691145587.
   9. ^Weinberg, Steven (1999). The quantum theory of fields (Reprinted (with
      corr.). ed.). Cambridge [u.a.]: Cambridge Univ. Press.
      ISBN 9780521550017.
  10. ^Zee, A. (2013). Einstein gravity in a nutshell. Princeton: Princeton
      University Press. ISBN 9780691145587.
  11. ^Mexico, Kevin Cahill, University of New (2013). Physical mathematics
      (Repr. ed.). Cambridge: Cambridge University Press. ISBN 978-1107005211.
  12. ^Edwards, Ron Larson, Robert, Bruce H. (2010). Calculus of a single
      variable (9th ed.). Belmont: Brooks/Cole. ISBN 9780547209982.
  13. ^Shankar, R. (1994). Principles of quantum mechanics (2nd ed.). New York:
      Kluwer Academic / Plenum. p. 318. ISBN 9780306447907.
  14. ^ J. E. Marsden and T. J. R. Hughes, 2000, Mathematical Foundations of
      Elasticity, Dover.
***** References[edit] *****
    * Hildebrand, F. B. (1976). Advanced Calculus for Applications. Prentice
      Hall. ISBN 0-13-011189-9.
K.F. Riley; M.P. Hobson; S.J. Bence (2010). Mathematical methods for physics
and engineering. Cambridge University Press. ISBN 978-0-521-86153-3.
***** External links[edit] *****
    * Directional_derivatives at MathWorld.
    * Directional_derivative at PlanetMath.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Directional_derivative&oldid=904603618"
Categories:
    * Differential_calculus
    * Differential_geometry
    * Generalizations_of_the_derivative
    * Multivariable_calculus
Hidden categories:
    * Articles_needing_additional_references_from_October_2012
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
**** In other projects ****
    * Wikimedia_Commons
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * CatalÃ 
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 3 July 2019, at 07:19 (UTC).
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
