The following text has been accessed from https://en.wikipedia.org/wiki/Vector_calculus at Fri Aug 9 01:05:44 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Vector calculus ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with Geometric_calculus or Matrix_calculus.
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (February 2016)(Learn_how_and
 when_to_remove_this_template_message)
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
Vector calculus, or vector analysis, is a branch of mathematics concerned with
differentiation and integration of vector_fields, primarily in 3-dimensional
Euclidean_space       R   3   .   {\displaystyle \mathbb {R} ^{3}.}  [\mathbb
{R} ^{3}.] The term "vector calculus" is sometimes used as a synonym for the
broader subject of multivariable_calculus, which includes vector calculus as
well as partial_differentiation and multiple_integration. Vector calculus plays
an important role in differential_geometry and in the study of partial
differential_equations. It is used extensively in physics and engineering,
especially in the description of electromagnetic_fields, gravitational_fields
and fluid_flow.
Vector calculus was developed from quaternion analysis by J._Willard_Gibbs and
Oliver_Heaviside near the end of the 19th century, and most of the notation and
terminology was established by Gibbs and Edwin_Bidwell_Wilson in their 1901
book, Vector_Analysis. In the conventional form using cross_products, vector
calculus does not generalize to higher dimensions, while the alternative
approach of geometric_algebra, which uses exterior_products does generalize, as
discussed_below.
⁰
***** Contents *****
    * 1_Basic_objects
          o 1.1_Scalar_fields
          o 1.2_Vector_fields
          o 1.3_Vectors_and_pseudovectors
    * 2_Vector_algebra
    * 3_Operators_and_theorems
          o 3.1_Differential_operators
          o 3.2_Integral_theorems
    * 4_Applications
          o 4.1_Linear_approximations
          o 4.2_Optimization
          o 4.3_Physics_and_engineering
    * 5_Generalizations
          o 5.1_Different_3-manifolds
          o 5.2_Other_dimensions
    * 6_See_also
    * 7_References
    * 8_External_links
***** Basic objects[edit] *****
**** Scalar fields[edit] ****
Main article: Scalar_field
A scalar_field associates a scalar value to every point in a space. The scalar
may either be a mathematical_number or a physical_quantity. Examples of scalar
fields in applications include the temperature distribution throughout space,
the pressure distribution in a fluid, and spin-zero quantum fields, such as the
Higgs_field. These fields are the subject of scalar_field_theory.
**** Vector fields[edit] ****
Main article: Vector_field
A vector_field is an assignment of a vector to each point in a subset of space.
[1] A vector field in the plane, for instance, can be visualized as a
collection of arrows with a given magnitude and direction each attached to a
point in the plane. Vector fields are often used to model, for example, the
speed and direction of a moving fluid throughout space, or the strength and
direction of some force, such as the magnetic or gravitational force, as it
changes from point to point.
**** Vectors and pseudovectors[edit] ****
In more advanced treatments, one further distinguishes pseudovector fields and
pseudoscalar fields, which are identical to vector fields and scalar fields
except that they change sign under an orientation-reversing map: for example,
the curl of a vector field is a pseudovector field, and if one reflects a
vector field, the curl points in the opposite direction. This distinction is
clarified and elaborated in geometric algebra, as described below.
***** Vector algebra[edit] *****
Main article: Euclidean_vector_Â§ Basic_properties
The algebraic (non-differential) operations in vector calculus are referred to
as vector_algebra, being defined for a vector space and then globally applied
to a vector field. The basic algebraic operations consist of:
Operation             Notation                     Description
                           v   1   +   v   2
                      {\displaystyle \mathbf {v} _ Addition of two vector
Vector_addition       {1}+\mathbf {v} _{2}}  [     fields, yielding a vector
                      {\displaystyle \mathbf {v} _ field.
                      {1}+\mathbf {v} _{2}}]
                         a  v    {\displaystyle    Multiplication of a scalar
Scalar_multiplication a\mathbf {v} }  [            field and a vector field,
                      {\displaystyle a\mathbf {v}  yielding a vector field.
                      }]
                           v   1   &#x22C5;   v
                      2     {\displaystyle \mathbf Multiplication of two vector
Dot_product           {v} _{1}\cdot \mathbf {v} _  fields, yielding a scalar
                      {2}}  [{\displaystyle        field.
                      \mathbf {v} _{1}\cdot
                      \mathbf {v} _{2}}]
                           v   1   &#x00D7;   v    Multiplication of two vector
                      2     {\displaystyle \mathbf fields in       R   3
Cross_product         {v} _{1}\times \mathbf {v} _ {\displaystyle \mathbb {R} ^
                      {2}}  [{\displaystyle        {3}}  [\mathbb {R} ^{3}],
                      \mathbf {v} _{1}\times       yielding a (pseudo)vector
                      \mathbf {v} _{2}}]           field.
Also commonly used are the two triple_products:
Operation             Notation                     Description
                           v   1   &#x22C5;
                      (    v   2   &#x00D7;   v
                      3    )    {\displaystyle
                      \mathbf {v} _{1}\cdot \left  The dot product of a vector
Scalar_triple_product (\mathbf {v} _{2}\times      and a cross product of two
                      \mathbf {v} _{3}\right)}  [  vectors.
                      {\displaystyle \mathbf {v} _
                      {1}\cdot \left(\mathbf {v} _
                      {2}\times \mathbf {v} _
                      {3}\right)}]
                           v   1   &#x00D7;
                      (    v   2   &#x00D7;   v
                      3    )    {\displaystyle
                      \mathbf {v} _{1}\times \left The cross product of a
Vector_triple_product (\mathbf {v} _{2}\times      vector and a cross product
                      \mathbf {v} _{3}\right)}  [  of two vectors.
                      {\displaystyle \mathbf {v} _
                      {1}\times \left(\mathbf {v}
                      _{2}\times \mathbf {v} _
                      {3}\right)}]
***** Operators and theorems[edit] *****
Main article: Vector_calculus_identities
**** Differential operators[edit] ****
Main articles: Gradient, Divergence, Curl_(mathematics), and Laplacian
Vector calculus studies various differential_operators defined on scalar or
vector fields, which are typically expressed in terms of the del operator
(    &#x2207;   {\displaystyle \nabla }  [\nabla ]), also known as "nabla". The
three basic vector_operators are:
Operation  Notation          Description       Notational     Domain/Range
                                               analogy
              grad &#x2061;
           ( f ) = &#x2207;
           f
           {\displaystyle    Measures the rate                Maps scalar
Gradient   \operatorname     and direction of  Scalar         fields to vector
           {grad} (f)=\nabla change in a       multiplication fields.
           f}                scalar field.
           [\operatorname
           {grad} (f)=\nabla
           f]
              div &#x2061;
           (  F  ) =
           &#x2207; &#x22C5;
           F
           {\displaystyle    Measures the
           \operatorname     scalar of a                      Maps vector
Divergence {div} (\mathbf    source or sink at Dot_product    fields to scalar
           {F} )=\nabla      a given point in                 fields.
           \cdot \mathbf {F} a vector field.
           }  [\operatorname
           {div} (\mathbf
           {F} )=\nabla
           \cdot \mathbf {F}
           ]
              curl &#x2061;
           (  F  ) =
           &#x2207; &#x00D7; Measures the
           F                 tendency to
           {\displaystyle    rotate about a
           \operatorname     point in a vector                Maps vector
           {curl} (\mathbf   field in       R                 fields to
Curl       {F} )=\nabla      3                 Cross_product  (pseudo)vector
           \times \mathbf    {\displaystyle                   fields.
           {F} }             \mathbb {R} ^{3}}
           [\operatorname    [\mathbb {R} ^
           {curl} (\mathbf   {3}].
           {F} )=\nabla
           \times \mathbf
           {F} ]
   f   {\displaystyle f}  [f] denotes a scalar field and     F
{\displaystyle F}  [F] denotes a vector field
Also commonly used are the two Laplace operators:
Operation        Notation             Description           Domain/Range
                    &#x0394; f =
                 &#x2207;  2   f =
                 &#x2207; &#x22C5;    Measures the
                 &#x2207; f           difference between
                 {\displaystyle       the value of the      Maps between scalar
Laplacian        \Delta f=\nabla ^    scalar field with its fields.
                 {2}f=\nabla \cdot    average on
                 \nabla f}  [\Delta   infinitesimal balls.
                 f=\nabla ^
                 {2}f=\nabla \cdot
                 \nabla f]
                     &#x2207;  2    F
                 = &#x2207;
                 ( &#x2207; &#x22C5;
                 F  ) &#x2212;
                 &#x2207; &#x00D7;
                 ( &#x2207; &#x00D7;
                 F  )
                 {\displaystyle       Measures the
                 \nabla ^{2}\mathbf   difference between
                 {F} =\nabla (\nabla  the value of the      Maps between vector
Vector_Laplacian \cdot \mathbf {F} )- vector field with its fields.
                 \nabla \times        average on
                 (\nabla \times       infinitesimal balls.
                 \mathbf {F} )}  [
                 {\displaystyle
                 \nabla ^{2}\mathbf
                 {F} =\nabla (\nabla
                 \cdot \mathbf {F} )-
                 \nabla \times
                 (\nabla \times
                 \mathbf {F} )}]
   f   {\displaystyle f}  [f] denotes a scalar field and     F   {\displaystyle
F}  [F] denotes a vector field
A quantity called the Jacobian_matrix is useful for studying functions when
both the domain and range of the function are multivariable, such as a change
of_variables during integration.
**** Integral theorems[edit] ****
The three basic vector operators have corresponding theorems which generalize
the fundamental_theorem_of_calculus to higher dimensions:
Theorem                   Statement         Description
                              &#x222B;  L
                          &#x2282;   R   n
                          &#x2207; &#x03C6;
                          &#x22C5; d  r
                          &#xA0; = &#xA0;
                          &#x03C6;  (  q  )
                          &#x2212; &#x03C6;
                          (  p  )  &#xA0;
                          &#xA0;
                          &#xA0;for&#xA0;
                          &#xA0; &#xA0; L =
                          L [ p &#x2192; q
                          ]
                          {\displaystyle
                          \int _{L\subset
                          \mathbb {R} ^
                          {n}}\!\!\!\nabla
                          \varphi \cdot
                          d\mathbf {r} \ =\ The line_integral of the gradient of a scalar field over a curve L is equal
Gradient_theorem          \varphi \left     to the change in the scalar field between the endpoints p and q of the curve.
                          (\mathbf {q}
                          \right)-\varphi
                          \left(\mathbf {p}
                          \right)\ \ {\text
                          { for }}\ \ L=L
                          [p\to q]}  [
                          {\displaystyle
                          \int _{L\subset
                          \mathbb {R} ^
                          {n}}\!\!\!\nabla
                          \varphi \cdot
                          d\mathbf {r} \ =\
                          \varphi \left
                          (\mathbf {q}
                          \right)-\varphi
                          \left(\mathbf {p}
                          \right)\ \ {\text
                          { for }}\ \ L=L
                          [p\to q]}]
                                 &#x222B;
                          &#x22EF;
                          &#x222B;  V
                          &#x2282;   R   n
                          &#x23DF;    n
                          ( &#x2207;
                          &#x22C5;  F  )  d
                          V &#xA0; = &#xA0;
                          &#x222E;
                          &#x22EF;
                          &#x222E;
                          &#x2202; V
                          &#x23DF;    n
                          &#x2212; 1    F
                          &#x22C5; d  S
                          {\displaystyle
                          \underbrace {\int
                          \!\cdots \!\int _
                          {V\subset \mathbb
                          {R} ^{n}}} _{n}
                          (\nabla \cdot
                          \mathbf {F}       The integral of the divergence of a vector field over an n-dimensional solid
Divergence_theorem        )\,dV\ =\         V is equal to the flux of the vector field through the (nâ1)-dimensional
                          \underbrace       closed boundary surface of the solid.
                          {\oint \!\!\cdots
                          \!\oint _
                          {\!\!\!\!\partial
                          V}} _{n-1}\mathbf
                          {F} \cdot
                          d\mathbf {S} }  [
                          {\displaystyle
                          \underbrace {\int
                          \!\cdots \!\int _
                          {V\subset \mathbb
                          {R} ^{n}}} _{n}
                          (\nabla \cdot
                          \mathbf {F}
                          )\,dV\ =\
                          \underbrace
                          {\oint \!\!\cdots
                          \!\oint _
                          {\!\!\!\!\partial
                          V}} _{n-1}\mathbf
                          {F} \cdot
                          d\mathbf {S} }]
                              &#x222C;
                          &#x03A3;
                          &#x2282;   R   3
                          ( &#x2207;
                          &#x00D7;  F  )
                          &#x22C5; d
                          &#x03A3;  &#xA0;
                          = &#xA0;
                          &#x222E;
                          &#x2202; &#x03A3;
                          &#x2061;  F
                          &#x22C5; d  r
                          {\displaystyle
                          \iint _{\Sigma
                          \,\subset \mathbb
                          {R} ^{3}}(\nabla
                          \times \mathbf    The integral of the curl of a vector field over a surface Î£ in       R   3
Curl_(KelvinâStokes) {F} )\cdot        {\displaystyle \mathbb {R} ^{3}}  [\mathbb {R} ^{3}] is equal to the
theorem                   d\mathbf {\Sigma  circulation of the vector field around the closed curve bounding the surface.
                          } \ =\ \oint _
                          {\!\!\!\!\partial
                          \Sigma }\mathbf
                          {F} \cdot
                          d\mathbf {r} }  [
                          {\displaystyle
                          \iint _{\Sigma
                          \,\subset \mathbb
                          {R} ^{3}}(\nabla
                          \times \mathbf
                          {F} )\cdot
                          d\mathbf {\Sigma
                          } \ =\ \oint _
                          {\!\!\!\!\partial
                          \Sigma }\mathbf
                          {F} \cdot
                          d\mathbf {r} }]
   &#x03C6;   {\displaystyle \varphi }  [\varphi ] denotes a scalar field and     F   {\displaystyle F}  [F] denotes a
vector field
In two dimensions, the divergence and curl theorems reduce to the Green's
theorem:
Theorem         Statement                      Description
                    &#x222C;  A  &#x2282;   R
                2      (     &#x2202; M
                &#x2202; x    &#x2212;
                &#x2202; L   &#x2202; y     )
                d A &#xA0; = &#xA0;
                &#x222E;           &#x2202; A
                &#x2061;  (  L  d x + M  d y   The integral of the divergence
                )    {\displaystyle \iint _    (or curl) of a vector field
                {A\,\subset \mathbb {R} ^      over some region A in       R
                {2}}\left({\frac {\partial M}  2     {\displaystyle \mathbb
Green's_theorem {\partial x}}-{\frac {\partial {R} ^{2}}  [\mathbb {R} ^{2}]
                L}{\partial y}}\right)\,dA\ =\ equals the flux (or
                \oint _{\!\!\!\!\partial       circulation) of the vector
                A}\left(L\,dx+M\,dy\right)}  [ field over the closed curve
                {\displaystyle \iint _         bounding the region.
                {A\,\subset \mathbb {R} ^
                {2}}\left({\frac {\partial M}
                {\partial x}}-{\frac {\partial
                L}{\partial y}}\right)\,dA\ =\
                \oint _{\!\!\!\!\partial
                A}\left(L\,dx+M\,dy\right)}]
For divergence,     F = ( M , &#x2212; L )   {\displaystyle F=(M,-L)}  [
{\displaystyle F=(M,-L)}]. For curl,     F = ( L , M , 0 )   {\displaystyle F=
(L,M,0)}  [{\displaystyle F=(L,M,0)}]. L and M are functions of (x, y).
***** Applications[edit] *****
**** Linear approximations[edit] ****
Main article: Linear_approximation
Linear approximations are used to replace complicated functions with linear
functions that are almost the same. Given a differentiable function     f ( x ,
y )   {\displaystyle f(x,y)}  [f(x,y)] with real values, one can approximate
f ( x , y )   {\displaystyle f(x,y)}  [f(x,y)] for     ( x , y )
{\displaystyle (x,y)}  [(x,y)] close to     ( a , b )   {\displaystyle (a,b)}
[(a,b)] by the formula
         f ( x , y ) &#x2248; f ( a , b ) +    &#x2202; f   &#x2202; x    ( a ,
      b ) ( x &#x2212; a ) +    &#x2202; f   &#x2202; y    ( a , b ) ( y
      &#x2212; b ) .   {\displaystyle f(x,y)\approx f(a,b)+{\frac {\partial f}
      {\partial x}}(a,b)(x-a)+{\frac {\partial f}{\partial y}}(a,b)(y-b).}  [
      {\displaystyle f(x,y)\approx f(a,b)+{\frac {\partial f}{\partial x}}(a,b)
      (x-a)+{\frac {\partial f}{\partial y}}(a,b)(y-b).}]
The right-hand side is the equation of the plane tangent to the graph of     z
= f ( x , y )   {\displaystyle z=f(x,y)}  [z=f(x,y)] at     ( a , b ) .
{\displaystyle (a,b).}  [(a,b).]
**** Optimization[edit] ****
Main article: Mathematical_optimization
For a continuously differentiable function_of_several_real_variables, a point P
(that is a set of values for the input variables, which is viewed as a point in
Rn) is critical if all of the partial_derivatives of the function are zero at
P, or, equivalently, if its gradient is zero. The critical values are the
values of the function at the critical points.
If the function is smooth, or, at least twice continuously differentiable, a
critical point may be either a local_maximum, a local_minimum or a saddle
point. The different cases may be distinguished by considering the eigenvalues
of the Hessian_matrix of second derivatives.
By Fermat's_theorem, all local maxima_and_minima of a differentiable function
occur at critical points. Therefore, to find the local maxima and minima, it
suffices, theoretically, to compute the zeros of the gradient and the
eigenvalues of the Hessian matrix at these zeros.
**** Physics and engineering[edit] ****
Vector calculus is particularly useful in studying:
    * Center_of_mass
    * Field_theory
    * Kinematics
    * Maxwell's_equations
***** Generalizations[edit] *****
**** Different 3-manifolds[edit] ****
Vector calculus is initially defined for Euclidean_3-space,       R   3   ,
{\displaystyle \mathbb {R} ^{3},}  [\mathbb {R} ^{3},] which has additional
structure beyond simply being a 3-dimensional real vector space, namely: a norm
(giving a notion of length) defined via an inner_product (the dot_product),
which in turn gives a notion of angle, and an orientation, which gives a notion
of left-handed and right-handed. These structures give rise to a volume_form,
and also the cross_product, which is used pervasively in vector calculus.
The gradient and divergence require only the inner product, while the curl and
the cross product also requires the handedness of the coordinate_system to be
taken into account (see cross_product_and_handedness for more detail).
Vector calculus can be defined on other 3-dimensional real vector spaces if
they have an inner product (or more generally a symmetric nondegenerate_form)
and an orientation; note that this is less data than an isomorphism to
Euclidean space, as it does not require a set of coordinates (a frame of
reference), which reflects the fact that vector calculus is invariant under
rotations (the special_orthogonal_group SO(3)).
More generally, vector calculus can be defined on any 3-dimensional oriented
Riemannian_manifold, or more generally pseudo-Riemannian_manifold. This
structure simply means that the tangent_space at each point has an inner
product (more generally, a symmetric nondegenerate form) and an orientation, or
more globally that there is a symmetric nondegenerate metric_tensor and an
orientation, and works because vector calculus is defined in terms of tangent
vectors at each point.
**** Other dimensions[edit] ****
Most of the analytic results are easily understood, in a more general form,
using the machinery of differential_geometry, of which vector calculus forms a
subset. Grad and div generalize immediately to other dimensions, as do the
gradient theorem, divergence theorem, and Laplacian (yielding harmonic
analysis), while curl and cross product do not generalize as directly.
From a general point of view, the various fields in (3-dimensional) vector
calculus are uniformly seen as being k-vector fields: scalar fields are 0-
vector fields, vector fields are 1-vector fields, pseudovector fields are 2-
vector fields, and pseudoscalar fields are 3-vector fields. In higher
dimensions there are additional types of fields (scalar/vector/pseudovector/
pseudoscalar corresponding to 0/1/n−1/n dimensions, which is exhaustive in
dimension 3), so one cannot only work with (pseudo)scalars and (pseudo)vectors.
In any dimension, assuming a nondegenerate form, grad of a scalar function is a
vector field, and div of a vector field is a scalar function, but only in
dimension 3 or 7[2] (and, trivially, in dimension 0 or 1) is the curl of a
vector field a vector field, and only in 3 or 7 dimensions can a cross product
be defined (generalizations in other dimensionalities either require     n
&#x2212; 1   {\displaystyle n-1}  [n-1] vectors to yield 1 vector, or are
alternative Lie_algebras, which are more general antisymmetric bilinear
products). The generalization of grad and div, and how curl may be generalized
is elaborated at Curl:_Generalizations; in brief, the curl of a vector field is
a bivector field, which may be interpreted as the special_orthogonal_Lie
algebra of infinitesimal rotations; however, this cannot be identified with a
vector field because the dimensions differ â there are 3 dimensions of
rotations in 3 dimensions, but 6 dimensions of rotations in 4 dimensions (and
more generally          (   n 2   )    =   1 2   n ( n &#x2212; 1 )
{\displaystyle \textstyle {{\binom {n}{2}}={\frac {1}{2}}n(n-1)}}  [\textstyle
{{\binom {n}{2}}={\frac {1}{2}}n(n-1)}] dimensions of rotations in n
dimensions).
There are two important alternative generalizations of vector calculus. The
first, geometric_algebra, uses k-vector fields instead of vector fields (in 3
or fewer dimensions, every k-vector field can be identified with a scalar
function or vector field, but this is not true in higher dimensions). This
replaces the cross product, which is specific to 3 dimensions, taking in two
vector fields and giving as output a vector field, with the exterior_product,
which exists in all dimensions and takes in two vector fields, giving as output
a bivector (2-vector) field. This product yields Clifford_algebras as the
algebraic structure on vector spaces (with an orientation and nondegenerate
form). Geometric algebra is mostly used in generalizations of physics and other
applied fields to higher dimensions.
The second generalization uses differential_forms (k-covector fields) instead
of vector fields or k-vector fields, and is widely used in mathematics,
particularly in differential_geometry, geometric_topology, and harmonic
analysis, in particular yielding Hodge_theory on oriented pseudo-Riemannian
manifolds. From this point of view, grad, curl, and div correspond to the
exterior_derivative of 0-forms, 1-forms, and 2-forms, respectively, and the key
theorems of vector calculus are all special cases of the general form of
Stokes'_theorem.
From the point of view of both of these generalizations, vector calculus
implicitly identifies mathematically distinct objects, which makes the
presentation simpler but the underlying mathematical structure and
generalizations less clear. From the point of view of geometric algebra, vector
calculus implicitly identifies k-vector fields with vector fields or scalar
functions: 0-vectors and 3-vectors with scalars, 1-vectors and 2-vectors with
vectors. From the point of view of differential forms, vector calculus
implicitly identifies k-forms with scalar fields or vector fields: 0-forms and
3-forms with scalar fields, 1-forms and 2-forms with vector fields. Thus for
example the curl naturally takes as input a vector field or 1-form, but
naturally has as output a 2-vector field or 2-form (hence pseudovector field),
which is then interpreted as a vector field, rather than directly taking a
vector field to a vector field; this is reflected in the curl of a vector field
in higher dimensions not having as output a vector field.
***** See also[edit] *****
    * Real-valued_function
    * Function_of_a_real_variable
    * Function_of_several_real_variables
    * Vector_calculus_identities
    * Del_in_cylindrical_and_spherical_coordinates
    * Directional_derivative
    * Conservative_vector_field
    * Solenoidal_vector_field
    * Laplacian_vector_field
    * Helmholtz_decomposition
    * Orthogonal_coordinates
    * Skew_coordinates
    * Curvilinear_coordinates
    * Tensor
***** References[edit] *****
   1. ^Galbis, Antonio & Maestre, Manuel (2012). Vector_Analysis_Versus_Vector
      Calculus. Springer. p. 12. ISBN 978-1-4614-2199-3.CS1 maint: Uses authors
      parameter (link)
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
   3. ^ http://www.springerlink.com/content/r3p3602pq2t10036/
    * Sandro Caparrini (2002) "The_discovery_of_the_vector_representation_of
      moments_and_angular_velocity", Archive for History of Exact Sciences 56:
      151â81.
    * Michael J. Crowe (1967). A_History_of_Vector_Analysis_:_The_Evolution_of
      the_Idea_of_a_Vectorial_System. Dover Publications; Reprint edition.
      ISBN 978-0-486-67910-5.
J.E. Marsden (1976). Vector Calculus. W. H. Freeman & Company. ISBN 978-0-7167-
0462-1.
H. M. Schey (2005). Div Grad Curl and all that: An informal text on vector
calculus. W. W. Norton & Company. ISBN 978-0-393-92516-6.
Barry Spain (1965) Vector_Analysis, 2nd edition, link from Internet_Archive.
Chen-To Tai (1995). A_historical_study_of_vector_analysis. Technical Report RL
915, Radiation Laboratory, University of Michigan.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Vector_analysis", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Hazewinkel,_Michiel, ed. (2001) [1994], "Vector_algebra", Encyclopedia_of
Mathematics, Springer Science+Business Media B.V. / Kluwer Academic Publishers,
ISBN 978-1-55608-010-4
Vector_Calculus_Video_Lectures from University_of_New_South_Wales on Academic
Earth
A_survey_of_the_improper_use_of_â_in_vector_analysis (1994) Tai, Chen-To
Expanding_vector_analysis_to_an_oblique_coordinate_system
Vector_Analysis: A Text-book for the Use of Students of Mathematics and
Physics, (based upon the lectures of Willard_Gibbs) by Edwin_Bidwell_Wilson,
published 1902.
Earliest_Known_Uses_of_Some_of_the_Words_of_Mathematics:_Vector_Analysis
Authority_control [Edit_this_at_Wikidata]     * NDL: 00560585

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Vector_calculus&oldid=909594997"
Categories:
    * Vector_calculus
Hidden categories:
    * CS1_maint:_Uses_authors_parameter
    * Articles_lacking_in-text_citations_from_February_2016
    * All_articles_lacking_in-text_citations
    * Wikipedia_articles_with_NDL_identifiers
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
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * Ð§ÓÐ²Ð°ÑÐ»Ð°
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * LietuviÅ³
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à°¤à±à°²à±à°à±
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * ä¸­æ
Edit_links
    * This page was last edited on 6 August 2019, at 11:17 (UTC).
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
