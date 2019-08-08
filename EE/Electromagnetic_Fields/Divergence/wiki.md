The following text has been accessed from https://en.wikipedia.org/wiki/Divergence at Thu Aug 8 22:56:15 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Divergence ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Vector operator producing the scalar quantity of a flow at a point
This article is about divergence in vector calculus. For divergence of infinite
series, see Divergent_series. For divergence in statistics, see Divergence_
(statistics). For other uses, see Divergence_(disambiguation).
[A_vector_field_with_diverging_vectors,_a_vector_field_with_converging_vectors,
and_a_vector_field_with_parallel_vectors_that_neither_diverge_nor_converge]
The divergence of different vector fields. The divergence of vectors from point
(x,y) equals the sum of the partial derivative-with-respect-to-x of the x-
component and the partial derivative-with-respect-to-y of the y-component at
that point:     &#x2207;  &#x22C5; (  V  ( x , y ) ) =    &#x2202; &#xA0;    V
x   ( x , y )    &#x2202;  x     +    &#x2202; &#xA0;    V   y   ( x , y )
&#x2202;  y       {\displaystyle \nabla \!\cdot (\mathbf {V} (x,y))={\frac
{\partial \ {\mathbf {V} _{x}(x,y)}}{\partial {x}}}+{\frac {\partial \ {\mathbf
{V} _{y}(x,y)}}{\partial {y}}}}  [{\displaystyle \nabla \!\cdot (\mathbf {V}
(x,y))={\frac {\partial \ {\mathbf {V} _{x}(x,y)}}{\partial {x}}}+{\frac
{\partial \ {\mathbf {V} _{y}(x,y)}}{\partial {y}}}}]
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
In vector_calculus, divergence is a vector_operator that produces a scalar
field, giving the quantity of a vector_field's source at each point. More
technically, the divergence represents the volume density of the outward flux
of a vector field from an infinitesimal volume around a given point.
As an example, consider air as it is heated or cooled. The velocity of the air
at each point defines a vector field. While air is heated in a region, it
expands in all directions, and thus the velocity field points outward from that
region. The divergence of the velocity field in that region would thus have a
positive value. While the air is cooled and thus contracting, the divergence of
the velocity has a negative value.
⁰
***** Contents *****
    * 1_Physical_interpretation_of_divergence
    * 2_Definition
          o 2.1_Cartesian_coordinates
          o 2.2_Cylindrical_coordinates
          o 2.3_Spherical_coordinates
          o 2.4_General_coordinates
    * 3_Decomposition_theorem
    * 4_Properties
    * 5_Relation_with_the_exterior_derivative
    * 6_Generalizations
    * 7_See_also
    * 8_Notes
    * 9_Citations
    * 10_References
    * 11_External_links
***** Physical interpretation of divergence[edit] *****
In physical terms, the divergence of a three-dimensional vector field is the
extent to which the vector field flux behaves like a source at a given point.
It is a local measure of its "outgoingness" â the extent to which there is
more of some quantity exiting an infinitesimal region of space than entering
it. If the divergence is nonzero at some point then there is compression or
expansion at that point. (Note that we are imagining the vector field to be
like the velocity vector field of a fluid (in motion) when we use the terms
flux and so on.)
More rigorously, the divergence of a vector field F at a point p can be defined
as the limit of the net flux of F across the smooth boundary of a three-
dimensional region V divided by the volume of V as V shrinks to p. Formally,
             div &#x2061;  F   |   p   =  lim  V &#x2192; { p }    &#x222C;  S
      ( V )       F  &#x22C5;    n &#x005E;       |  V  |      d S ,
      {\displaystyle \left.\operatorname {div} \mathbf {F} \right|_{p}=\lim _
      {V\rightarrow \{p\}}\iint _{S(V)}{\frac {\mathbf {F} \cdot \mathbf {\hat
      {n}} }{|V|}}\,dS,}  [{\displaystyle \left.\operatorname {div} \mathbf {F}
      \right|_{p}=\lim _{V\rightarrow \{p\}}\iint _{S(V)}{\frac {\mathbf {F}
      \cdot \mathbf {\hat {n}} }{|V|}}\,dS,}]
where |V| is the volume of V, S(V) is the boundary of V, and the integral is a
surface_integral with nÌ being the outward unit normal to that surface. The
result, div F, is a function of p. From this definition it also becomes obvious
that div F can be seen as the source density of the flux of F.
In light of the physical interpretation, a vector field with zero divergence
everywhere is called incompressible or solenoidal â in which case any closed
surface has no net flux across it.
The intuition that the sum of all sources minus the sum of all sinks should
give the net flux outwards of a region is made precise by the divergence
theorem.
***** Definition[edit] *****
**** Cartesian coordinates[edit] ****
In three-dimensional Cartesian coordinates, the divergence of a continuously
differentiable vector_field      F  =  F  x    i  +  F  y    j  +  F  z    k
{\displaystyle \mathbf {F} =F_{x}\mathbf {i} +F_{y}\mathbf {j} +F_{z}\mathbf
{k} }  [{\displaystyle \mathbf {F} =F_{x}\mathbf {i} +F_{y}\mathbf {j} +F_
{z}\mathbf {k} }] is defined as the scalar-valued function:
         div &#x2061;  F  = &#x2207; &#x22C5;  F  =  (    &#x2202;  &#x2202; x
      ,   &#x2202;  &#x2202; y    ,   &#x2202;  &#x2202; z     )  &#x22C5; (  F
      x   ,  F  y   ,  F  z   ) =    &#x2202;  F  x     &#x2202; x    +
      &#x2202;  F  y     &#x2202; y    +    &#x2202;  F  z     &#x2202; z    .
      {\displaystyle \operatorname {div} \mathbf {F} =\nabla \cdot \mathbf {F}
      =\left({\frac {\partial }{\partial x}},{\frac {\partial }{\partial y}},
      {\frac {\partial }{\partial z}}\right)\cdot (F_{x},F_{y},F_{z})={\frac
      {\partial F_{x}}{\partial x}}+{\frac {\partial F_{y}}{\partial y}}+{\frac
      {\partial F_{z}}{\partial z}}.}  [{\displaystyle \operatorname {div}
      \mathbf {F} =\nabla \cdot \mathbf {F} =\left({\frac {\partial }{\partial
      x}},{\frac {\partial }{\partial y}},{\frac {\partial }{\partial
      z}}\right)\cdot (F_{x},F_{y},F_{z})={\frac {\partial F_{x}}{\partial x}}+
      {\frac {\partial F_{y}}{\partial y}}+{\frac {\partial F_{z}}{\partial
      z}}.}]
Although expressed in terms of coordinates, the result is invariant under
rotations, as the physical interpretation suggests. This is because the trace
of the Jacobian_matrix of an N-dimensional vector field F in N-dimensional
space is invariant under any invertible linear transformation.
The common notation for the divergence â Â· F is a convenient mnemonic, where
the dot denotes an operation reminiscent of the dot_product: take the
components of the â operator (see del), apply them to the corresponding
components of F, and sum the results. Because applying an operator is different
from multiplying the components, this is considered an abuse_of_notation.
The divergence of a continuously differentiable second-order tensor_field Îµ is
a first-order tensor field:[1]
           div &#x2192;   (  &#x03B5;  ) =   [        &#x2202;  &#x03B5;  x x
      &#x2202; x     +     &#x2202;  &#x03B5;  y x     &#x2202; y     +
      &#x2202;  &#x03B5;  z x     &#x2202; z             &#x2202;  &#x03B5;  x
      y     &#x2202; x     +     &#x2202;  &#x03B5;  y y     &#x2202; y     +
      &#x2202;  &#x03B5;  z y     &#x2202; z             &#x2202;  &#x03B5;  x
      z     &#x2202; x     +     &#x2202;  &#x03B5;  y z     &#x2202; y     +
      &#x2202;  &#x03B5;  z z     &#x2202; z        ]   .   {\displaystyle
      {\overrightarrow {\operatorname {div} }}(\mathbf {\varepsilon } )={\begin
      {bmatrix}{\dfrac {\partial \varepsilon _{xx}}{\partial x}}+{\dfrac
      {\partial \varepsilon _{yx}}{\partial y}}+{\dfrac {\partial \varepsilon _
      {zx}}{\partial z}}\\{\dfrac {\partial \varepsilon _{xy}}{\partial x}}+
      {\dfrac {\partial \varepsilon _{yy}}{\partial y}}+{\dfrac {\partial
      \varepsilon _{zy}}{\partial z}}\\{\dfrac {\partial \varepsilon _{xz}}
      {\partial x}}+{\dfrac {\partial \varepsilon _{yz}}{\partial y}}+{\dfrac
      {\partial \varepsilon _{zz}}{\partial z}}\end{bmatrix}}.}  [
      {\displaystyle {\overrightarrow {\operatorname {div} }}(\mathbf
      {\varepsilon } )={\begin{bmatrix}{\dfrac {\partial \varepsilon _{xx}}
      {\partial x}}+{\dfrac {\partial \varepsilon _{yx}}{\partial y}}+{\dfrac
      {\partial \varepsilon _{zx}}{\partial z}}\\{\dfrac {\partial \varepsilon
      _{xy}}{\partial x}}+{\dfrac {\partial \varepsilon _{yy}}{\partial y}}+
      {\dfrac {\partial \varepsilon _{zy}}{\partial z}}\\{\dfrac {\partial
      \varepsilon _{xz}}{\partial x}}+{\dfrac {\partial \varepsilon _{yz}}
      {\partial y}}+{\dfrac {\partial \varepsilon _{zz}}{\partial z}}\end
      {bmatrix}}.}]
**** Cylindrical coordinates[edit] ****
For a vector expressed in local unit cylindrical_coordinates as
          F  =   e   r    F  r   +   e   &#x03B8;    F  &#x03B8;   +   e   z
      F  z   ,   {\displaystyle \mathbf {F} =\mathbf {e} _{r}F_{r}+\mathbf {e}
      _{\theta }F_{\theta }+\mathbf {e} _{z}F_{z},}  [{\displaystyle \mathbf
      {F} =\mathbf {e} _{r}F_{r}+\mathbf {e} _{\theta }F_{\theta }+\mathbf {e}
      _{z}F_{z},}]
where ea is the unit vector in direction a, the divergence is[2]
         div &#x2061;  F  = &#x2207; &#x22C5;  F  =   1 r     &#x2202;
      &#x2202; r     (  r  F  r    )  +   1 r      &#x2202;  F  &#x03B8;
      &#x2202; &#x03B8;    +    &#x2202;  F  z     &#x2202; z    .
      {\displaystyle \operatorname {div} \mathbf {F} =\nabla \cdot \mathbf {F}
      ={\frac {1}{r}}{\frac {\partial }{\partial r}}\left(rF_{r}\right)+{\frac
      {1}{r}}{\frac {\partial F_{\theta }}{\partial \theta }}+{\frac {\partial
      F_{z}}{\partial z}}.}  [{\displaystyle \operatorname {div} \mathbf {F}
      =\nabla \cdot \mathbf {F} ={\frac {1}{r}}{\frac {\partial }{\partial
      r}}\left(rF_{r}\right)+{\frac {1}{r}}{\frac {\partial F_{\theta }}
      {\partial \theta }}+{\frac {\partial F_{z}}{\partial z}}.}]
The use of local coordinates is vital for the validity of the expression. If we
consider x the position vector and the functions     r (  x  )   {\displaystyle
r(\mathbf {x} )}  [{\displaystyle r(\mathbf {x} )}],     &#x03B8; (  x  )
{\displaystyle \theta (\mathbf {x} )}  [{\displaystyle \theta (\mathbf {x} )}],
and     z (  x  )   {\displaystyle z(\mathbf {x} )}  [{\displaystyle z(\mathbf
{x} )}], which assign the corresponding global cylindrical coordinate to a
vector, in general     r (  F  (  x  ) ) &#x2260;  F  r   (  x  )
{\displaystyle r(\mathbf {F} (\mathbf {x} ))\neq F_{r}(\mathbf {x} )}  [
{\displaystyle r(\mathbf {F} (\mathbf {x} ))\neq F_{r}(\mathbf {x} )}],
&#x03B8; (  F  (  x  ) ) &#x2260;  F  &#x03B8;   (  x  )   {\displaystyle
\theta (\mathbf {F} (\mathbf {x} ))\neq F_{\theta }(\mathbf {x} )}  [
{\displaystyle \theta (\mathbf {F} (\mathbf {x} ))\neq F_{\theta }(\mathbf {x}
)}], and     z (  F  (  x  ) ) &#x2260;  F  z   (  x  )   {\displaystyle z
(\mathbf {F} (\mathbf {x} ))\neq F_{z}(\mathbf {x} )}  [{\displaystyle z
(\mathbf {F} (\mathbf {x} ))\neq F_{z}(\mathbf {x} )}]. In particular, if we
consider the identity function      F  (  x  ) =  x    {\displaystyle \mathbf
{F} (\mathbf {x} )=\mathbf {x} }  [{\displaystyle \mathbf {F} (\mathbf {x}
)=\mathbf {x} }], we find that:
         &#x03B8; (  F  (  x  ) ) = &#x03B8; &#x2260;  F  &#x03B8;   (  x  ) =
      0   {\displaystyle \theta (\mathbf {F} (\mathbf {x} ))=\theta \neq F_
      {\theta }(\mathbf {x} )=0}  [{\displaystyle \theta (\mathbf {F} (\mathbf
      {x} ))=\theta \neq F_{\theta }(\mathbf {x} )=0}].
**** Spherical coordinates[edit] ****
In spherical_coordinates, with Î¸ the angle with the z axis and Ï the rotation
around the z axis, and      F    {\displaystyle \mathbf {F} }  [\mathbf {F} ]
again written in local unit coordinates, the divergence is[3]
         div &#x2061;  F  = &#x2207; &#x22C5;  F  =   1  r  2       &#x2202;
      &#x2202; r     (   r  2    F  r    )  +   1  r sin &#x2061; &#x03B8;
      &#x2202;  &#x2202; &#x03B8;    ( sin &#x2061; &#x03B8;   F  &#x03B8;   )
      +   1  r sin &#x2061; &#x03B8;       &#x2202;  F  &#x03C6;     &#x2202;
      &#x03C6;    .   {\displaystyle \operatorname {div} \mathbf {F} =\nabla
      \cdot \mathbf {F} ={\frac {1}{r^{2}}}{\frac {\partial }{\partial r}}\left
      (r^{2}F_{r}\right)+{\frac {1}{r\sin \theta }}{\frac {\partial }{\partial
      \theta }}(\sin \theta \,F_{\theta })+{\frac {1}{r\sin \theta }}{\frac
      {\partial F_{\varphi }}{\partial \varphi }}.}  [{\displaystyle
      \operatorname {div} \mathbf {F} =\nabla \cdot \mathbf {F} ={\frac {1}{r^
      {2}}}{\frac {\partial }{\partial r}}\left(r^{2}F_{r}\right)+{\frac {1}
      {r\sin \theta }}{\frac {\partial }{\partial \theta }}(\sin \theta \,F_
      {\theta })+{\frac {1}{r\sin \theta }}{\frac {\partial F_{\varphi }}
      {\partial \varphi }}.}]
**** General coordinates[edit] ****
Using Einstein_notation we can consider the divergence in general_coordinates,
which we write as x1, ..., xi, ...,xn, where n is the number of dimensions of
the domain. Here, the upper index refers to the number of the coordinate or
component, so x2 refers to the second component, and not the quantity x
squared. The index variable i is used to refer to an arbitrary element, such as
xi. The divergence can then be written via the Voss-Weyl formula[4], as:
         div &#x2061; (  F  ) =   1 &#x03C1;      &#x2202;  (  &#x03C1;   F  i
      )    &#x2202;  x  i      ,   {\displaystyle \operatorname {div} (\mathbf
      {F} )={\frac {1}{\rho }}{\frac {\partial \left(\rho \,F^{i}\right)}
      {\partial x^{i}}},}  [{\displaystyle \operatorname {div} (\mathbf {F} )=
      {\frac {1}{\rho }}{\frac {\partial \left(\rho \,F^{i}\right)}{\partial x^
      {i}}},}]
where     &#x03C1;   {\displaystyle \rho }  [\rho ] is the local coefficient of
the volume_element and Fi  are the components of F with respect to the local
unnormalized covariant_basis (sometimes written as       e   i   = &#x2202;  x
/  &#x2202;  x  i     {\displaystyle \mathbf {e} _{i}=\partial \mathbf {x} /
\partial x^{i}}  [{\displaystyle \mathbf {e} _{i}=\partial \mathbf {x} /
\partial x^{i}}]). The Einstein notation implies summation over i, since it
appears as both an upper and lower index.
The volume coefficient     &#x03C1;   {\displaystyle \rho }  [\rho ] is a
function of position which depends on the coordinate system. In Cartesian,
cylindrical and spherical coordinates, using the same conventions as before, we
have     &#x03C1; = 1   {\displaystyle \rho =1}  [\rho =1],     &#x03C1; = r
{\displaystyle \rho =r}  [{\displaystyle \rho =r}] and     &#x03C1; =  r  2
sin &#x2061;  &#x03B8;    {\displaystyle \rho =r^{2}\sin {\theta }}  [
{\displaystyle \rho =r^{2}\sin {\theta }}], respectively. It can also be
expressed as     &#x03C1; =   det &#x2061;  g  a b       {\displaystyle \rho =
{\sqrt {\operatorname {det} g_{ab}}}}  [{\displaystyle \rho ={\sqrt
{\operatorname {det} g_{ab}}}}], where      g  a b     {\displaystyle g_{ab}}
[g_{ab}] is the metric_tensor. Since the determinant is a scalar quantity which
doesn't depend on the indices, we can suppress them and simply write
&#x03C1; =   det &#x2061; g     {\displaystyle \rho ={\sqrt {\operatorname
{det} g}}}  [{\displaystyle \rho ={\sqrt {\operatorname {det} g}}}]. Another
expression comes from computing the determinant of the Jacobian for
transforming from Cartesian coordinates, which for n = 3 gives     &#x03C1; =
|    &#x2202; ( x , y , z )   &#x2202; (  x  1   ,  x  2   ,  x  3   )    |  .
{\displaystyle \rho =\left|{\frac {\partial (x,y,z)}{\partial (x^{1},x^{2},x^
{3})}}\right|.}  [{\displaystyle \rho =\left|{\frac {\partial (x,y,z)}{\partial
(x^{1},x^{2},x^{3})}}\right|.}]
Some conventions expect all local basis elements to be normalized to unit
length, as was done in the previous sections. If we write          e  &#x005E;
i     {\displaystyle {\hat {\mathbf {e} }}_{i}}  [{\hat {\mathbf {e} }}_{i}]
for the normalized basis, and         F &#x005E;     i     {\displaystyle {\hat
{F}}^{i}}  [{\displaystyle {\hat {F}}^{i}}] for the components of F with
respect to it, we have that
          F  =  F  i     e   i   =  F  i    &#x2016;    e   i    &#x2016;
      e   i    &#x2016;    e   i    &#x2016;    =  F  i      g  i i           e
      &#x005E;     i   =     F &#x005E;     i        e  &#x005E;     i   ,
      {\displaystyle \mathbf {F} =F^{i}\mathbf {e} _{i}=F^{i}{\lVert {\mathbf
      {e} _{i}}\rVert }{\frac {\mathbf {e} _{i}}{\lVert {\mathbf {e} _
      {i}}\rVert }}=F^{i}{\sqrt {g_{ii}}}\,{\hat {\mathbf {e} }}_{i}={\hat
      {F}}^{i}{\hat {\mathbf {e} }}_{i},}  [{\displaystyle \mathbf {F} =F^
      {i}\mathbf {e} _{i}=F^{i}{\lVert {\mathbf {e} _{i}}\rVert }{\frac
      {\mathbf {e} _{i}}{\lVert {\mathbf {e} _{i}}\rVert }}=F^{i}{\sqrt {g_
      {ii}}}\,{\hat {\mathbf {e} }}_{i}={\hat {F}}^{i}{\hat {\mathbf {e} }}_
      {i},}]
using one of the properties of the metric tensor. By dotting both sides of the
last equality with the contravariant element          e  &#x005E;     i
{\displaystyle {\hat {\mathbf {e} }}^{i}}  [{\displaystyle {\hat {\mathbf {e}
}}^{i}}], we can conclude that      F  i   =     F &#x005E;     i    /     g  i
i       {\displaystyle F^{i}={\hat {F}}^{i}/{\sqrt {g_{ii}}}}  [{\displaystyle
F^{i}={\hat {F}}^{i}/{\sqrt {g_{ii}}}}]. After substituting, the formula
becomes:
         div &#x2061; (  F  ) =   1 &#x03C1;      &#x2202;  (    &#x03C1;   g
      i i          F &#x005E;     i    )    &#x2202;  x  i      =   1  det
      &#x2061; g       &#x2202;  (      det &#x2061; g   g  i i           F
      &#x005E;     i    )    &#x2202;  x  i        {\displaystyle \operatorname
      {div} (\mathbf {F} )={\frac {1}{\rho }}{\frac {\partial \left({\frac
      {\rho }{\sqrt {g_{ii}}}}{\hat {F}}^{i}\right)}{\partial x^{i}}}={\frac
      {1}{\sqrt {\operatorname {det} g}}}{\frac {\partial \left({\sqrt {\frac
      {\operatorname {det} g}{g_{ii}}}}\,{\hat {F}}^{i}\right)}{\partial x^
      {i}}}}  [{\displaystyle \operatorname {div} (\mathbf {F} )={\frac {1}
      {\rho }}{\frac {\partial \left({\frac {\rho }{\sqrt {g_{ii}}}}{\hat {F}}^
      {i}\right)}{\partial x^{i}}}={\frac {1}{\sqrt {\operatorname {det} g}}}
      {\frac {\partial \left({\sqrt {\frac {\operatorname {det} g}{g_{ii}}}}\,
      {\hat {F}}^{i}\right)}{\partial x^{i}}}}].
See Â§ Generalizations for further discussion.
***** Decomposition theorem[edit] *****
Main article: Helmholtz_decomposition
It can be shown that any stationary flux v(r) that is at least twice
continuously differentiable in R3 and vanishes sufficiently fast for |r| â
â can be decomposed into an irrotational part E(r) and a source-free part B
(r). Moreover, these parts are explicitly determined by the respective source
densities (see above) and circulation densities (see the article Curl):
For the irrotational part one has
          E  = &#x2212; &#x2207; &#x03A6; (  r  ) ,   {\displaystyle \mathbf
      {E} =-\nabla \Phi (\mathbf {r} ),}  [{\displaystyle \mathbf {E} =-\nabla
      \Phi (\mathbf {r} ),}]
with
         &#x03A6; (  r  ) =  &#x222B;    R   3       d  3     r  &#x2032;
      div &#x2061;  v  (   r  &#x2032;  )   4 &#x03C0;  |   r  &#x2212;   r
      &#x2032;   |     .   {\displaystyle \Phi (\mathbf {r} )=\int _{\mathbb
      {R} ^{3}}\,d^{3}\mathbf {r} '\;{\frac {\operatorname {div} \mathbf {v}
      (\mathbf {r} ')}{4\pi \left|\mathbf {r} -\mathbf {r} '\right|}}.}  [
      {\displaystyle \Phi (\mathbf {r} )=\int _{\mathbb {R} ^{3}}\,d^{3}\mathbf
      {r} '\;{\frac {\operatorname {div} \mathbf {v} (\mathbf {r} ')}{4\pi
      \left|\mathbf {r} -\mathbf {r} '\right|}}.}]
The source-free part, B, can be similarly written: one only has to replace the
scalar potential Î¦(r) by a vector potential A(r) and the terms ââÎ¦ by
+â Ã A, and the source density div v by the circulation density â Ã v.
This "decomposition theorem" is a by-product of the stationary case of
electrodynamics. It is a special case of the more general Helmholtz
decomposition which works in dimensions greater than three as well.
***** Properties[edit] *****
Main article: Vector_calculus_identities
The following properties can all be derived from the ordinary differentiation
rules of calculus. Most importantly, the divergence is a linear_operator, i.e.,
         div &#x2061; ( a  F  + b  G  ) = a div &#x2061;  F  + b div &#x2061;
      G    {\displaystyle \operatorname {div} (a\mathbf {F} +b\mathbf {G}
      )=a\operatorname {div} \mathbf {F} +b\operatorname {div} \mathbf {G} }  [
      {\displaystyle \operatorname {div} (a\mathbf {F} +b\mathbf {G}
      )=a\operatorname {div} \mathbf {F} +b\operatorname {div} \mathbf {G} }]
for all vector fields F and G and all real_numbers a and b.
There is a product_rule of the following type: if Ï is a scalar-valued
function and F is a vector field, then
         div &#x2061; ( &#x03C6;  F  ) = grad &#x2061; &#x03C6; &#x22C5;  F  +
      &#x03C6; div &#x2061;  F  ,   {\displaystyle \operatorname {div} (\varphi
      \mathbf {F} )=\operatorname {grad} \varphi \cdot \mathbf {F} +\varphi
      \operatorname {div} \mathbf {F} ,}  [{\displaystyle \operatorname {div}
      (\varphi \mathbf {F} )=\operatorname {grad} \varphi \cdot \mathbf {F}
      +\varphi \operatorname {div} \mathbf {F} ,}]
or in more suggestive notation
         &#x2207; &#x22C5; ( &#x03C6;  F  ) = ( &#x2207; &#x03C6; ) &#x22C5;  F
      + &#x03C6; ( &#x2207; &#x22C5;  F  ) .   {\displaystyle \nabla \cdot
      (\varphi \mathbf {F} )=(\nabla \varphi )\cdot \mathbf {F} +\varphi
      (\nabla \cdot \mathbf {F} ).}  [{\displaystyle \nabla \cdot (\varphi
      \mathbf {F} )=(\nabla \varphi )\cdot \mathbf {F} +\varphi (\nabla \cdot
      \mathbf {F} ).}]
Another product rule for the cross_product of two vector fields F and G in
three dimensions involves the curl and reads as follows:
         div &#x2061; (  F  &#x00D7;  G  ) = curl &#x2061;  F  &#x22C5;  G
      &#x2212;  F  &#x22C5; curl &#x2061;  G  ,   {\displaystyle \operatorname
      {div} (\mathbf {F} \times \mathbf {G} )=\operatorname {curl} \mathbf {F}
      \cdot \mathbf {G} -\mathbf {F} \cdot \operatorname {curl} \mathbf {G} ,}
      [{\displaystyle \operatorname {div} (\mathbf {F} \times \mathbf {G}
      )=\operatorname {curl} \mathbf {F} \cdot \mathbf {G} -\mathbf {F} \cdot
      \operatorname {curl} \mathbf {G} ,}]
or
         &#x2207; &#x22C5; (  F  &#x00D7;  G  ) = ( &#x2207; &#x00D7;  F  )
      &#x22C5;  G  &#x2212;  F  &#x22C5; ( &#x2207; &#x00D7;  G  ) .
      {\displaystyle \nabla \cdot (\mathbf {F} \times \mathbf {G} )=(\nabla
      \times \mathbf {F} )\cdot \mathbf {G} -\mathbf {F} \cdot (\nabla \times
      \mathbf {G} ).}  [{\displaystyle \nabla \cdot (\mathbf {F} \times \mathbf
      {G} )=(\nabla \times \mathbf {F} )\cdot \mathbf {G} -\mathbf {F} \cdot
      (\nabla \times \mathbf {G} ).}]
The Laplacian of a scalar_field is the divergence of the field's gradient:
         div &#x2061; ( &#x2207; &#x03C6; ) = &#x0394; &#x03C6; .
      {\displaystyle \operatorname {div} (\nabla \varphi )=\Delta \varphi .}  [
      {\displaystyle \operatorname {div} (\nabla \varphi )=\Delta \varphi .}]
The divergence of the curl of any vector field (in three dimensions) is equal
to zero:
         &#x2207; &#x22C5; ( &#x2207; &#x00D7;  F  ) = 0.   {\displaystyle
      \nabla \cdot (\nabla \times \mathbf {F} )=0.}  [{\displaystyle \nabla
      \cdot (\nabla \times \mathbf {F} )=0.}]
If a vector field F with zero divergence is defined on a ball in R3, then there
exists some vector field G on the ball with F = curl G. For regions in R3 more
topologically complicated than this, the latter statement might be false (see
PoincarÃ©_lemma). The degree of failure of the truth of the statement, measured
by the homology of the chain_complex
         {  scalar fields on&#xA0;  U } &#xA0;   &#x2192; grad   &#xA0;
      {  vector fields on&#xA0;  U } &#xA0;   &#x2192; curl   &#xA0; {  vector
      fields on&#xA0;  U } &#xA0;   &#x2192; div   &#xA0; {  scalar fields
      on&#xA0;  U }   {\displaystyle \{{\text{scalar fields on }}U\}~{\overset
      {\operatorname {grad} }{\rightarrow }}~\{{\text{vector fields on }}U\}~
      {\overset {\operatorname {curl} }{\rightarrow }}~\{{\text{vector fields
      on }}U\}~{\overset {\operatorname {div} }{\rightarrow }}~\{{\text{scalar
      fields on }}U\}}  [{\displaystyle \{{\text{scalar fields on }}U\}~
      {\overset {\operatorname {grad} }{\rightarrow }}~\{{\text{vector fields
      on }}U\}~{\overset {\operatorname {curl} }{\rightarrow }}~\{{\text{vector
      fields on }}U\}~{\overset {\operatorname {div} }{\rightarrow }}~\{{\text
      {scalar fields on }}U\}}]
serves as a nice quantification of the complicatedness of the underlying region
U. These are the beginnings and main motivations of de_Rham_cohomology.
***** Relation with the exterior derivative[edit] *****
One can express the divergence as a particular case of the exterior derivative,
which takes a 2-form to a 3-form in R3. Define the current two-form as
         j =  F  1    d y &#x2227; d z +  F  2    d z &#x2227; d x +  F  3    d
      x &#x2227; d y .   {\displaystyle j=F_{1}\,dy\wedge dz+F_{2}\,dz\wedge
      dx+F_{3}\,dx\wedge dy.}  [{\displaystyle j=F_{1}\,dy\wedge dz+F_
      {2}\,dz\wedge dx+F_{3}\,dx\wedge dy.}]
It measures the amount of "stuff" flowing through a surface per unit time in a
"stuff fluid" of density Ï = 1 dx â§ dy â§ dz moving with local velocity F.
Its exterior_derivative dj is then given by
         d j =  (     &#x2202;  F  1     &#x2202; x    +    &#x2202;  F  2
      &#x2202; y    +    &#x2202;  F  3     &#x2202; z     )  d x &#x2227; d y
      &#x2227; d z = ( &#x2207; &#x22C5;   F   ) &#x03C1; .   {\displaystyle
      dj=\left({\frac {\partial F_{1}}{\partial x}}+{\frac {\partial F_{2}}
      {\partial y}}+{\frac {\partial F_{3}}{\partial z}}\right)dx\wedge
      dy\wedge dz=(\nabla \cdot {\mathbf {F} })\rho .}  [{\displaystyle
      dj=\left({\frac {\partial F_{1}}{\partial x}}+{\frac {\partial F_{2}}
      {\partial y}}+{\frac {\partial F_{3}}{\partial z}}\right)dx\wedge
      dy\wedge dz=(\nabla \cdot {\mathbf {F} })\rho .}]
Thus, the divergence of the vector field F can be expressed as:
         &#x2207; &#x22C5;   F   =  &#x22C6;  d  &#x22C6;    (      F
      &#x266D;     )   .   {\displaystyle \nabla \cdot {\mathbf {F} }={\star }d
      {\star }{\big (}{\mathbf {F} }^{\flat }{\big )}.}  [{\displaystyle \nabla
      \cdot {\mathbf {F} }={\star }d{\star }{\big (}{\mathbf {F} }^{\flat }
      {\big )}.}]
Here the superscript &#x266d; is one of the two musical_isomorphisms, and â
is the Hodge_star_operator. Working with the current two-form and the exterior
derivative is usually easier than working with the vector field and divergence,
because unlike the divergence, the exterior derivative commutes with a change
of (curvilinear) coordinate system.
***** Generalizations[edit] *****
The divergence of a vector field can be defined in any number of dimensions. If
          F  = (  F  1   ,  F  2   , &#x2026;  F  n   ) ,   {\displaystyle
      \mathbf {F} =(F_{1},F_{2},\ldots F_{n}),}  [{\displaystyle \mathbf {F} =
      (F_{1},F_{2},\ldots F_{n}),}]
in a Euclidean coordinate system with coordinates x1, x2, ..., xn, define
         div &#x2061;  F  = &#x2207; &#x22C5;  F  =    &#x2202;  F  1
      &#x2202;  x  1      +    &#x2202;  F  2     &#x2202;  x  2      +
      &#x22EF; +    &#x2202;  F  n     &#x2202;  x  n      .   {\displaystyle
      \operatorname {div} \mathbf {F} =\nabla \cdot \mathbf {F} ={\frac
      {\partial F_{1}}{\partial x_{1}}}+{\frac {\partial F_{2}}{\partial x_
      {2}}}+\cdots +{\frac {\partial F_{n}}{\partial x_{n}}}.}  [{\displaystyle
      \operatorname {div} \mathbf {F} =\nabla \cdot \mathbf {F} ={\frac
      {\partial F_{1}}{\partial x_{1}}}+{\frac {\partial F_{2}}{\partial x_
      {2}}}+\cdots +{\frac {\partial F_{n}}{\partial x_{n}}}.}]
The appropriate expression is more complicated in curvilinear_coordinates.
In the case of one dimension, F reduces to a regular function, and the
divergence reduces to the derivative.
For any n, the divergence is a linear operator, and it satisfies the "product
rule"
         &#x2207; &#x22C5; ( &#x03C6;  F  ) = ( &#x2207; &#x03C6; ) &#x22C5;  F
      + &#x03C6; ( &#x2207; &#x22C5;  F  )   {\displaystyle \nabla \cdot
      (\varphi \mathbf {F} )=(\nabla \varphi )\cdot \mathbf {F} +\varphi
      (\nabla \cdot \mathbf {F} )}  [{\displaystyle \nabla \cdot (\varphi
      \mathbf {F} )=(\nabla \varphi )\cdot \mathbf {F} +\varphi (\nabla \cdot
      \mathbf {F} )}]
for any scalar-valued function Ï.
The divergence of a vector field extends naturally to any differentiable
manifold of dimension n that has a volume_form (or density) Î¼, e.g. a
Riemannian or Lorentzian_manifold. Generalising the construction of a two-form
for a vector field on R3, on such a manifold a vector field X defines an (n â
1)-form j = iX Î¼ obtained by contracting X with Î¼. The divergence is then the
function defined by
         d j = ( div &#x2061; X ) &#x03BC; .   {\displaystyle dj=(\operatorname
      {div} X)\mu .}  [{\displaystyle dj=(\operatorname {div} X)\mu .}]
Standard formulas for the Lie_derivative allow us to reformulate this as
            L    X   &#x03BC; = ( div &#x2061; X ) &#x03BC; .   {\displaystyle
      {\mathcal {L}}_{X}\mu =(\operatorname {div} X)\mu .}  [{\displaystyle
      {\mathcal {L}}_{X}\mu =(\operatorname {div} X)\mu .}]
This means that the divergence measures the rate of expansion of a volume
element as we let it flow with the vector field.
On a pseudo-Riemannian_manifold, the divergence with respect to the metric
volume form can be computed in terms of the Levi-Civita_connection â:
         div &#x2061; X = &#x2207; &#x22C5; X =    X  a     ; a   ,
      {\displaystyle \operatorname {div} X=\nabla \cdot X={X^{a}}_{;a},}  [
      {\displaystyle \operatorname {div} X=\nabla \cdot X={X^{a}}_{;a},}]
where the second expression is the contraction of the vector field valued 1-
form âX with itself and the last expression is the traditional coordinate
expression from Ricci_calculus.
An equivalent expression without using connection is
         div &#x2061; ( X ) =   1  det &#x2061; g     &#x2202;  a    (    det
      &#x2061; g     X  a    )  ,   {\displaystyle \operatorname {div} (X)=
      {\frac {1}{\sqrt {\operatorname {det} g}}}\partial _{a}\left({\sqrt
      {\operatorname {det} g}}\,X^{a}\right),}  [{\displaystyle \operatorname
      {div} (X)={\frac {1}{\sqrt {\operatorname {det} g}}}\partial _{a}\left(
      {\sqrt {\operatorname {det} g}}\,X^{a}\right),}]
where g is the metric and âa denotes the partial derivative with respect to
coordinate xa.
Divergence can also be generalised to tensors. In Einstein_notation, the
divergence of a contravariant_vector FÎ¼ is given by
         &#x2207; &#x22C5;  F  =  &#x2207;  &#x03BC;    F  &#x03BC;   ,
      {\displaystyle \nabla \cdot \mathbf {F} =\nabla _{\mu }F^{\mu },}  [
      {\displaystyle \nabla \cdot \mathbf {F} =\nabla _{\mu }F^{\mu },}]
where âÎ¼ denotes the covariant_derivative.
Equivalently, some authors define the divergence of a mixed_tensor by using the
musical_isomorphism &#x266f;: if T is a (p, q)-tensor (p for the contravariant
vector and q for the covariant one), then we define the divergence of T to be
the (p, q â 1)-tensor
         ( div &#x2061; T ) (  Y  1   , &#x2026; ,  Y  q &#x2212; 1   ) =
      trace    (   X &#x21A6; &#x266F; ( &#x2207; T ) ( X , &#x22C5; ,  Y  1
      , &#x2026; ,  Y  q &#x2212; 1   )   )   ;   {\displaystyle (\operatorname
      {div} T)(Y_{1},\ldots ,Y_{q-1})={\operatorname {trace} }{\Big (}X\mapsto
      \sharp (\nabla T)(X,\cdot ,Y_{1},\ldots ,Y_{q-1}){\Big )};}  [
      {\displaystyle (\operatorname {div} T)(Y_{1},\ldots ,Y_{q-1})=
      {\operatorname {trace} }{\Big (}X\mapsto \sharp (\nabla T)(X,\cdot ,Y_
      {1},\ldots ,Y_{q-1}){\Big )};}]
that is, we take the trace over the first two covariant indices of the
covariant derivative[a]
***** See also[edit] *****
    * Curl
    * Del_in_cylindrical_and_spherical_coordinates
    * Divergence_theorem
    * Gradient
***** Notes[edit] *****
   1. ^  The choice of "first" covariant index of a tensor is intrinsic and
      depends on the ordering of the terms of the Cartesian product of vector
      spaces on which the tensor is given as a multilinear map V Ã V Ã ... Ã
      V â R. But equally well defined choices for the divergence could be
      made by using other indices. Consequently, it is more natural to specify
      the divergence of T with respect to a specified index. There are however
      two important special cases where this choice is essentially irrelevant:
      with a totally symmetric contravariant tensor, when every choice is
      equivalent, and with a totally antisymmetric contravariant tensor (a.k.a.
      a k-vector), when the choice affects only the sign.
***** Citations[edit] *****
   1. ^ Gurtin_1981, p. 30.
   2. ^ Cylindrical_coordinates at Wolfram Mathworld
   3. ^ Spherical_coordinates at Wolfram Mathworld
   4. ^Grinfeld, Pavel. "The_Voss-Weyl_Formula". Retrieved 9 January 2018.
   5. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
***** References[edit] *****
    * Brewer, Jess H. (1999). "DIVERGENCE_of_a_Vector_Field". musr.phas.ubc.ca.
      Archived from the_original on 2007-11-23. Retrieved 2016-08-09.
Rudin, Walter (1976). Principles of mathematical analysis. McGraw-Hill. ISBN 0-
07-054235-X.
Edwards, C. H. (1994). Advanced Calculus of Several Variables. Mineola, NY:
Dover. ISBN 0-486-68336-2.
Gurtin, Morton (1981). An Introduction to Continuum Mechanics. Academic Press.
ISBN 0-12-309750-9.
Theresa, M. Korn; Korn, Granino Arthur. Mathematical Handbook for Scientists
and Engineers: Definitions, Theorems, and Formulas for Reference and Review.
New York: Dover Publications. pp. 157â160. ISBN 0-486-41147-8.
***** External links[edit] *****
 Wikimedia Commons has media related to Divergence.
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Divergence", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
The_idea_of_divergence_of_a_vector_field
Khan_Academy:_Divergence_video_lesson
Sanderson, Grant (June 21, 2018). "Divergence_and_curl:_The_language_of
Maxwell's_equations,_fluid_flow,_and_more". 3Blue1Brown – via YouTube.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Divergence&oldid=909201325"
Categories:
    * Differential_operators
    * Linear_operators_in_calculus
    * Vector_calculus
Hidden categories:
    * Articles_with_short_description
    * Commons_category_link_from_Wikidata
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * LietuviÅ³
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
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
    * à®¤à®®à®¿à®´à¯
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 3 August 2019, at 20:43 (UTC).
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
