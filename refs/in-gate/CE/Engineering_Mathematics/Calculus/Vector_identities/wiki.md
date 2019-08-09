The following text has been accessed from https://en.wikipedia.org/wiki/Vector_calculus_identities at Thu Aug 8 23:41:31 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Vector calculus identities ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
See also: Vector_algebra_relations
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (August 2017)(Learn_how_and
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
The following identities are important in vector_calculus:
⁰
***** Contents *****
    * 1_Operator_notations
          o 1.1_Gradient
          o 1.2_Divergence
          o 1.3_Curl
          o 1.4_Laplacian
          o 1.5_Special_notations
    * 2_Properties
          o 2.1_Distributive_properties
          o 2.2_Product_rule
          o 2.3_Quotient_rule
          o 2.4_Chain_rule
          o 2.5_Dot_product_rule
          o 2.6_Cross_product_rule
    * 3_Second_derivatives
          o 3.1_Curl_of_gradient_is_zero
          o 3.2_Divergence_of_curl_is_zero
          o 3.3_Divergence_of_gradient
          o 3.4_Curl_of_curl
    * 4_Summary_of_important_identities
          o 4.1_Addition_and_multiplication
          o 4.2_Differentiation
                # 4.2.1_Gradient
                # 4.2.2_Divergence
                # 4.2.3_Curl
                # 4.2.4_Second_derivatives
                # 4.2.5_Third_derivatives
          o 4.3_Integration
                # 4.3.1_Surfaceâvolume_integrals
                # 4.3.2_Curveâsurface_integrals
    * 5_See_also
    * 6_References
    * 7_Further_reading
***** Operator notations[edit] *****
**** Gradient[edit] ****
Main article: Gradient
For a function     f ( x , y , z )   {\displaystyle f(x,y,z)}  [f(x,y,z)]in
three-dimensional Cartesian_coordinate variables, the gradient is the vector
field:
         grad &#x2061; ( f ) &#xA0; = &#xA0; &#x2207; f &#xA0; = &#xA0;
      &#x2202; f   &#x2202; x      i  +     &#x2202; f   &#x2202; y      j  +
      &#x2202; f   &#x2202; z      k  &#xA0; = &#xA0; (     &#x2202; f
      &#x2202; x     ,     &#x2202; f   &#x2202; y     ,     &#x2202; f
      &#x2202; z     )   {\displaystyle \operatorname {grad} (f)\ =\ \nabla f\
      =\ {\tfrac {\partial f}{\partial x}}\mathbf {i} +{\tfrac {\partial f}
      {\partial y}}\mathbf {j} +{\tfrac {\partial f}{\partial z}}\mathbf {k} \
      =\ ({\tfrac {\partial f}{\partial x}},{\tfrac {\partial f}{\partial y}},
      {\tfrac {\partial f}{\partial z}})}  [{\displaystyle \operatorname {grad}
      (f)\ =\ \nabla f\ =\ {\tfrac {\partial f}{\partial x}}\mathbf {i} +
      {\tfrac {\partial f}{\partial y}}\mathbf {j} +{\tfrac {\partial f}
      {\partial z}}\mathbf {k} \ =\ ({\tfrac {\partial f}{\partial x}},{\tfrac
      {\partial f}{\partial y}},{\tfrac {\partial f}{\partial z}})}]
where i, j, k are the standard unit_vectors for the x, y, z-axes. More
generally, for a function of n variables     &#x03C8; (  x  1   , &#x2026; ,  x
n   )   {\displaystyle \psi (x_{1},\ldots ,x_{n})}  [{\displaystyle \psi (x_
{1},\ldots ,x_{n})}], also called a scalar field, the gradient is the vector
field:
        &#x2207; &#x03C8; = (     &#x2202; &#x03C8;   &#x2202;  x  1
     , &#x2026; ,     &#x2202; &#x03C8;   &#x2202;  x  n       ) .
     {\displaystyle \nabla \psi =({\tfrac {\partial \psi }{\partial x_
     {1}}},\ldots ,{\tfrac {\partial \psi }{\partial x_{n}}}).}  [
     {\displaystyle \nabla \psi =({\tfrac {\partial \psi }{\partial x_
     {1}}},\ldots ,{\tfrac {\partial \psi }{\partial x_{n}}}).}]
For a vector field      A  = (  A  1   , &#x2026; ,  A  n   )   {\displaystyle
\mathbf {A} =(A_{1},\ldots ,A_{n})}  [{\displaystyle \mathbf {A} =(A_{1},\ldots
,A_{n})}] written as a 1 Ã n row vector, also called a tensor field of order
1, the gradient or covariant_derivative is the n Ã n Jacobian_matrix:
        &#x2207;   A  =   J    A    =   (    &#x2202;  A  i     &#x2202;
     x  j      )    i j   .   {\displaystyle \nabla \!\mathbf {A} =\mathbf
     {J} _{\mathbf {A} }=\left({\frac {\partial A_{i}}{\partial x_
     {j}}}\right)_{\!ij}.}  [{\displaystyle \nabla \!\mathbf {A} =\mathbf
     {J} _{\mathbf {A} }=\left({\frac {\partial A_{i}}{\partial x_
     {j}}}\right)_{\!ij}.}]
For a tensor_field      A    {\displaystyle \mathbf {A} }  [\mathbf {A} ] of
any order k, the gradient     grad &#x2061; (  A  ) = &#x2207;   A
{\displaystyle \operatorname {grad} (\mathbf {A} )=\nabla \!\mathbf {A} }  [
{\displaystyle \operatorname {grad} (\mathbf {A} )=\nabla \!\mathbf {A} }]is a
tensor field of order k + 1.
**** Divergence[edit] ****
Main article: Divergence
In Cartesian coordinates, the divergence of a continuously_differentiable
vector_field      F  =  F  x    i  +  F  y    j  +  F  z    k    {\displaystyle
\mathbf {F} =F_{x}\mathbf {i} +F_{y}\mathbf {j} +F_{z}\mathbf {k} }  [
{\displaystyle \mathbf {F} =F_{x}\mathbf {i} +F_{y}\mathbf {j} +F_{z}\mathbf
{k} }] is the scalar-valued function:
         div &#x2061;  F  &#xA0; = &#xA0; &#x2207; &#x22C5;  F  &#xA0; = &#xA0;
      (    &#x2202;  &#x2202; x     ,    &#x2202;  &#x2202; y     ,    &#x2202;
      &#x2202; z     ) &#x22C5; (  F  x   ,  F  y   ,  F  z   ) &#xA0; = &#xA0;
      &#x2202;  F  x     &#x2202; x     +     &#x2202;  F  y     &#x2202; y
      +     &#x2202;  F  z     &#x2202; z     .   {\displaystyle \operatorname
      {div} \mathbf {F} \ =\ \nabla \cdot \mathbf {F} \ =\ ({\tfrac {\partial }
      {\partial x}},{\tfrac {\partial }{\partial y}},{\tfrac {\partial }
      {\partial z}})\cdot (F_{x},F_{y},F_{z})\ =\ {\tfrac {\partial F_{x}}
      {\partial x}}+{\tfrac {\partial F_{y}}{\partial y}}+{\tfrac {\partial F_
      {z}}{\partial z}}.}  [{\displaystyle \operatorname {div} \mathbf {F} \ =\
      \nabla \cdot \mathbf {F} \ =\ ({\tfrac {\partial }{\partial x}},{\tfrac
      {\partial }{\partial y}},{\tfrac {\partial }{\partial z}})\cdot (F_{x},F_
      {y},F_{z})\ =\ {\tfrac {\partial F_{x}}{\partial x}}+{\tfrac {\partial F_
      {y}}{\partial y}}+{\tfrac {\partial F_{z}}{\partial z}}.}]
The divergence of a tensor_field      A    {\displaystyle \mathbf {A} }
[\mathbf {A} ]of non-zero order k, is written as     div &#x2061; (  A  ) =
&#x2207; &#x22C5;  A    {\displaystyle \operatorname {div} (\mathbf {A}
)=\nabla \cdot \mathbf {A} }  [\operatorname {div} (\mathbf {A} )=\nabla \cdot
\mathbf {A} ], a contraction to a tensor field of order k - 1. Specifically,
the divergence of a vector is a scalar. The divergence of a higher order tensor
field may be found by decomposing the tensor field into a sum of outer products
and using the identity,
         &#x2207; &#x22C5; (  B  &#x2297;     A  &#x005E;    ) =     A
      &#x005E;    ( &#x2207; &#x22C5;  B  ) + (  B  &#x22C5; &#x2207; )     A
      &#x005E;      {\displaystyle \nabla \cdot (\mathbf {B} \otimes {\hat
      {\mathbf {A} }})={\hat {\mathbf {A} }}(\nabla \cdot \mathbf {B} )+
      (\mathbf {B} \cdot \nabla ){\hat {\mathbf {A} }}}  [\nabla \cdot (\mathbf
      {B} \otimes {\hat {\mathbf {A} }})={\hat {\mathbf {A} }}(\nabla \cdot
      \mathbf {B} )+(\mathbf {B} \cdot \nabla ){\hat {\mathbf {A} }}]
where      B  &#x22C5; &#x2207;   {\displaystyle \mathbf {B} \cdot \nabla }
[\mathbf {B} \cdot \nabla ] is the directional_derivative in the direction of
B    {\displaystyle \mathbf {B} }  [\mathbf {B} ] multiplied by its magnitude.
Specifically, for the outer product of two vectors,
         &#x2207; &#x22C5;  (   b    a    T     )  =  a  ( &#x2207; &#x22C5;  b
      ) + (  b  &#x22C5; &#x2207; )  a  .   {\displaystyle \nabla \cdot \left
      (\mathbf {b} \mathbf {a} ^{\mathrm {T} }\right)=\mathbf {a} (\nabla \cdot
      \mathbf {b} )+(\mathbf {b} \cdot \nabla )\mathbf {a} .}  [{\displaystyle
      \nabla \cdot \left(\mathbf {b} \mathbf {a} ^{\mathrm {T} }\right)=\mathbf
      {a} (\nabla \cdot \mathbf {b} )+(\mathbf {b} \cdot \nabla )\mathbf {a}
      .}]
**** Curl[edit] ****
Main article: Curl_(mathematics)
In Cartesian coordinates, for      F  =  F  x    i  +  F  y    j  +  F  z    k
{\displaystyle \mathbf {F} =F_{x}\mathbf {i} +F_{y}\mathbf {j} +F_{z}\mathbf
{k} }  [{\displaystyle \mathbf {F} =F_{x}\mathbf {i} +F_{y}\mathbf {j} +F_
{z}\mathbf {k} }] the curl is the vector field:
         curl &#x2061;  F  &#xA0; = &#xA0; &#x2207; &#x00D7;  F  &#xA0; =
      &#xA0;  |      i     j     k        &#x2202;  &#x2202; x        &#x2202;
      &#x2202; y        &#x2202;  &#x2202; z         F  x      F  y      F  z
      |  &#xA0; = &#xA0;  (      &#x2202;  F  z     &#x2202; y      &#x2212;
      &#x2202;  F  y     &#x2202; z      )    i  +  (      &#x2202;  F  x
      &#x2202; z      &#x2212;      &#x2202;  F  z     &#x2202; x      )    j
      +  (      &#x2202;  F  y     &#x2202; x      &#x2212;      &#x2202;  F  x
      &#x2202; y      )    k    {\displaystyle \operatorname {curl} \mathbf {F}
      \ =\ \nabla \times \mathbf {F} \ =\ \left|{\begin{matrix}\mathbf {i}
      &\mathbf {j} &\mathbf {k} \\{\frac {\partial }{\partial x}}&{\frac
      {\partial }{\partial y}}&{\frac {\partial }{\partial z}}\\F_{x}&F_{y}&F_
      {z}\end{matrix}}\right|\ =\ \left({\tfrac {\partial F_{z}}{\partial y}}{-
      }{\tfrac {\partial F_{y}}{\partial z}}\right)\!\mathbf {i} +\left({\tfrac
      {\partial F_{x}}{\partial z}}{-}{\tfrac {\partial F_{z}}{\partial
      x}}\right)\!\mathbf {j} +\left({\tfrac {\partial F_{y}}{\partial x}}{-}
      {\tfrac {\partial F_{x}}{\partial y}}\right)\!\mathbf {k} }  [
      {\displaystyle \operatorname {curl} \mathbf {F} \ =\ \nabla \times
      \mathbf {F} \ =\ \left|{\begin{matrix}\mathbf {i} &\mathbf {j} &\mathbf
      {k} \\{\frac {\partial }{\partial x}}&{\frac {\partial }{\partial y}}&
      {\frac {\partial }{\partial z}}\\F_{x}&F_{y}&F_{z}\end{matrix}}\right|\
      =\ \left({\tfrac {\partial F_{z}}{\partial y}}{-}{\tfrac {\partial F_{y}}
      {\partial z}}\right)\!\mathbf {i} +\left({\tfrac {\partial F_{x}}
      {\partial z}}{-}{\tfrac {\partial F_{z}}{\partial x}}\right)\!\mathbf {j}
      +\left({\tfrac {\partial F_{y}}{\partial x}}{-}{\tfrac {\partial F_{x}}
      {\partial y}}\right)\!\mathbf {k} }]
where i, j, and k are the unit_vectors for the x-, y-, and z-axes,
respectively. In Einstein_notation, the vector field      F  = (  F  1   ,  F
2   ,  F  3   )   {\displaystyle \mathbf {F} =(F_{1},F_{2},F_{3})}  [
{\displaystyle \mathbf {F} =(F_{1},F_{2},F_{3})}]has curl given by:
         &#x2207; &#x00D7;  F  &#xA0; = &#xA0;  &#x03B5;  i j k      &#x2202;
      F  k     &#x2202;  x  j        {\displaystyle \nabla \times \mathbf {F} \
      =\ \varepsilon ^{ijk}{\frac {\partial F_{k}}{\partial x^{j}}}}  [
      {\displaystyle \nabla \times \mathbf {F} \ =\ \varepsilon ^{ijk}{\frac
      {\partial F_{k}}{\partial x^{j}}}}]
where     &#x03B5; = &#x00B1; 1   {\displaystyle \varepsilon =\pm 1}  [
{\displaystyle \varepsilon =\pm 1}] or 0 is the Levi-Civita_parity_symbol.
**** Laplacian[edit] ****
Main article: Laplace_operator
In Cartesian_coordinates, the Laplacian of a function     f ( x , y , z )
{\displaystyle f(x,y,z)}  [f(x,y,z)] is
         &#x0394; f =  &#x2207;  2   f = ( &#x2207; &#x22C5; &#x2207; ) f =
      &#x2202;  2   f   &#x2202;  x  2      +     &#x2202;  2   f   &#x2202;  y
      2      +     &#x2202;  2   f   &#x2202;  z  2      .   {\displaystyle
      \Delta f=\nabla ^{2}f=(\nabla \cdot \nabla )f={\frac {\partial ^{2}f}
      {\partial x^{2}}}+{\frac {\partial ^{2}f}{\partial y^{2}}}+{\frac
      {\partial ^{2}f}{\partial z^{2}}}.}  [{\displaystyle \Delta f=\nabla ^
      {2}f=(\nabla \cdot \nabla )f={\frac {\partial ^{2}f}{\partial x^{2}}}+
      {\frac {\partial ^{2}f}{\partial y^{2}}}+{\frac {\partial ^{2}f}{\partial
      z^{2}}}.}]
For a tensor_field,      A    {\displaystyle \mathbf {A} }  [\mathbf {A} ], the
laplacian is generally written as:
         &#x0394;  A  =  &#x2207;  2    A  = ( &#x2207; &#x22C5; &#x2207; )  A
      {\displaystyle \Delta \mathbf {A} =\nabla ^{2}\mathbf {A} =(\nabla \cdot
      \nabla )\mathbf {A} }  [\Delta \mathbf {A} =\nabla ^{2}\mathbf {A} =
      (\nabla \cdot \nabla )\mathbf {A} ]
and is a tensor field of the same order.
**** Special notations[edit] ****
In Feynman subscript notation,
          &#x2207;   B      (  A  &#x22C5;  B  )  &#xA0; = &#xA0;  A   &#x00D7;
      (  &#x2207;  &#x00D7;   B   )   +   (   A   &#x22C5;  &#x2207;  )   B
      {\displaystyle \nabla _{\mathbf {B} }\!\left(\mathbf {A{\cdot }B}
      \right)\ =\ \mathbf {A} {\times }\!\left(\nabla {\times }\mathbf {B}
      \right)\,+\,\left(\mathbf {A} {\cdot }\nabla \right)\mathbf {B} }  [
      {\displaystyle \nabla _{\mathbf {B} }\!\left(\mathbf {A{\cdot }B}
      \right)\ =\ \mathbf {A} {\times }\!\left(\nabla {\times }\mathbf {B}
      \right)\,+\,\left(\mathbf {A} {\cdot }\nabla \right)\mathbf {B} }]
where the notation âB means the subscripted gradient operates on only the
factor B.[1][2]
Less general but similar is the Hestenes overdot notation in geometric_algebra.
[3] The above identity is then expressed as:
            &#x2207; &#x02D9;     (   A   &#x22C5;      B  &#x02D9;     )
      &#xA0; = &#xA0;  A   &#x00D7;    (  &#x2207;  &#x00D7;   B   )   +
      (   A   &#x22C5;  &#x2207;  )   B    {\displaystyle {\dot {\nabla }}\left
      (\mathbf {A} {\cdot }{\dot {\mathbf {B} }}\right)\ =\ \mathbf {A} {\times
      }\!\left(\nabla {\times }\mathbf {B} \right)\,+\,\left(\mathbf {A} {\cdot
      }\nabla \right)\mathbf {B} }  [{\displaystyle {\dot {\nabla }}\left
      (\mathbf {A} {\cdot }{\dot {\mathbf {B} }}\right)\ =\ \mathbf {A} {\times
      }\!\left(\nabla {\times }\mathbf {B} \right)\,+\,\left(\mathbf {A} {\cdot
      }\nabla \right)\mathbf {B} }]
where overdots define the scope of the vector derivative. The dotted vector, in
this case B, is differentiated, while the (undotted) A is held constant.
For the remainder of this article, Feynman subscript notation will be used
where appropriate.
***** Properties[edit] *****
For scalar fields     &#x03C8;   {\displaystyle \psi }  [\psi ],     &#x03D5;
{\displaystyle \phi }  [\phi ] and vector fields      A    {\displaystyle
\mathbf {A} }  [\mathbf {A} ],      B    {\displaystyle \mathbf {B} }  [\mathbf
{B} ], we have the following derivative identities.
**** Distributive properties[edit] ****
         &#x2207; ( &#x03C8; + &#x03D5; ) &#xA0; = &#xA0; &#x2207; &#x03C8; +
      &#x2207; &#x03D5;   {\displaystyle \nabla (\psi +\phi )\ =\ \nabla \psi
      +\nabla \phi }  [{\displaystyle \nabla (\psi +\phi )\ =\ \nabla \psi
      +\nabla \phi }]
         &#x2207; (  A  +  B  ) &#xA0; = &#xA0; &#x2207;   A  + &#x2207;  B
      {\displaystyle \nabla (\mathbf {A} +\mathbf {B} )\ =\ \nabla \!\mathbf
      {A} +\nabla \mathbf {B} }  [{\displaystyle \nabla (\mathbf {A} +\mathbf
      {B} )\ =\ \nabla \!\mathbf {A} +\nabla \mathbf {B} }]
         &#x2207;   &#x22C5;   (  A  +  B  ) &#xA0; = &#xA0; &#x2207;  &#x22C5;
      A  + &#x2207;  &#x22C5;   B    {\displaystyle \nabla \,{\cdot }\,(\mathbf
      {A} +\mathbf {B} )\ =\ \nabla {\cdot }\mathbf {A} +\nabla {\cdot }\mathbf
      {B} }  [{\displaystyle \nabla \,{\cdot }\,(\mathbf {A} +\mathbf {B} )\ =\
      \nabla {\cdot }\mathbf {A} +\nabla {\cdot }\mathbf {B} }]
         &#x2207;  &#x00D7;  (  A  +  B  ) &#xA0; = &#xA0; &#x2207;  &#x00D7;
      A  + &#x2207;  &#x00D7;   B    {\displaystyle \nabla {\times }(\mathbf
      {A} +\mathbf {B} )\ =\ \nabla {\times }\mathbf {A} +\nabla {\times
      }\mathbf {B} }  [{\displaystyle \nabla {\times }(\mathbf {A} +\mathbf {B}
      )\ =\ \nabla {\times }\mathbf {A} +\nabla {\times }\mathbf {B} }]
**** Product rule[edit] ****
We have the following generalizations of the product_rule in single variable
calculus.
         &#x2207; ( &#x03C8; &#x03D5; ) &#xA0; = &#xA0; &#x03D5;  &#x2207;
      &#x03C8;  +  &#x03C8;  &#x2207; &#x03D5;   {\displaystyle \nabla (\psi
      \phi )\ =\ \phi \,\nabla \psi \,+\,\psi \,\nabla \phi }  [{\displaystyle
      \nabla (\psi \phi )\ =\ \phi \,\nabla \psi \,+\,\psi \,\nabla \phi }]
         &#x2207; ( &#x03C8;  A  ) &#xA0; = &#xA0; ( &#x2207; &#x03C8;  )   T
      A   +  &#x03C8;  &#x2207;   A  &#xA0; = &#xA0; &#x2207; &#x03C8; &#x2297;
      A   +  &#x03C8;  &#x2207;   A    {\displaystyle \nabla (\psi \mathbf {A}
      )\ =\ (\nabla \psi )^{\mathbf {T} }\mathbf {A} \,+\,\psi \,\nabla
      \!\mathbf {A} \ =\ \nabla \psi \otimes \mathbf {A} \,+\,\psi \,\nabla
      \!\mathbf {A} }  [{\displaystyle \nabla (\psi \mathbf {A} )\ =\ (\nabla
      \psi )^{\mathbf {T} }\mathbf {A} \,+\,\psi \,\nabla \!\mathbf {A} \ =\
      \nabla \psi \otimes \mathbf {A} \,+\,\psi \,\nabla \!\mathbf {A} }]
         &#x2207;   &#x22C5;   ( &#x03C8;  A  ) &#xA0; = &#xA0; &#x03C8;
      &#x2207;  &#x22C5;   A   +  ( &#x2207; &#x03C8; )  &#x22C5;   A
      {\displaystyle \nabla \,{\cdot }\,(\psi \mathbf {A} )\ =\ \psi \,\nabla
      {\cdot }\mathbf {A} \,+\,(\nabla \psi ){\cdot }\mathbf {A} }  [
      {\displaystyle \nabla \,{\cdot }\,(\psi \mathbf {A} )\ =\ \psi \,\nabla
      {\cdot }\mathbf {A} \,+\,(\nabla \psi ){\cdot }\mathbf {A} }]
         &#x2207;  &#x00D7;  ( &#x03C8;  A  ) &#xA0; = &#xA0; &#x03C8;
      ( &#x2207;  &#x00D7;   A  )  +  ( &#x2207; &#x03C8; )  &#x00D7;   A
      {\displaystyle \nabla {\times }(\psi \mathbf {A} )\ =\ \psi \,(\nabla
      {\times }\mathbf {A} )\,+\,(\nabla \psi ){\times }\mathbf {A} }  [
      {\displaystyle \nabla {\times }(\psi \mathbf {A} )\ =\ \psi \,(\nabla
      {\times }\mathbf {A} )\,+\,(\nabla \psi ){\times }\mathbf {A} }]
In the second formula, the transposed gradient     ( &#x2207; &#x03C8;  )   T
{\displaystyle (\nabla \psi )^{\mathbf {T} }}  [{\displaystyle (\nabla \psi )^
{\mathbf {T} }}] is an n Ã 1 column vector,      A    {\displaystyle \mathbf
{A} }  [\mathbf {A} ] is a 1 Ã n row vector, and their product is an n Ã n
matrix: this may also be considered as the tensor_product of two vectors, or of
a covector and a vector.
**** Quotient rule[edit] ****
         &#x2207;   (   &#x03C8; &#x03D5;   )  &#xA0; = &#xA0;    &#x03D5;
      &#x2207; &#x03C8; &#x2212; ( &#x2207;  &#x03D5; ) &#x03C8;   &#x03D5;  2
      {\displaystyle \nabla \!\left({\frac {\psi }{\phi }}\right)\ =\ {\frac
      {\phi \,\nabla \psi -(\nabla \!\phi )\psi }{\phi ^{2}}}}  [{\displaystyle
      \nabla \!\left({\frac {\psi }{\phi }}\right)\ =\ {\frac {\phi \,\nabla
      \psi -(\nabla \!\phi )\psi }{\phi ^{2}}}}]
         &#x2207;   &#x22C5;    (    A  &#x03D5;   )  &#xA0; = &#xA0;
      &#x03D5;  &#x2207;  &#x22C5;   A  &#x2212; ( &#x2207;  &#x03D5; )
      &#x22C5;   A    &#x03D5;  2       {\displaystyle \nabla \,{\cdot }\!\left
      ({\frac {\mathbf {A} }{\phi }}\right)\ =\ {\frac {\phi \,\nabla {\cdot
      }\mathbf {A} -(\nabla \!\phi ){\cdot }\mathbf {A} }{\phi ^{2}}}}  [
      {\displaystyle \nabla \,{\cdot }\!\left({\frac {\mathbf {A} }{\phi
      }}\right)\ =\ {\frac {\phi \,\nabla {\cdot }\mathbf {A} -(\nabla \!\phi )
      {\cdot }\mathbf {A} }{\phi ^{2}}}}]
         &#x2207;   &#x00D7;    (    A  &#x03D5;   )  &#xA0; = &#xA0;
      &#x03D5;  &#x2207;  &#x00D7;   A  &#x2212; ( &#x2207;  &#x03D5; )
      &#x00D7;   A    &#x03D5;  2       {\displaystyle \nabla \,{\times
      }\!\left({\frac {\mathbf {A} }{\phi }}\right)\ =\ {\frac {\phi \,\nabla
      {\times }\mathbf {A} -(\nabla \!\phi ){\times }\mathbf {A} }{\phi ^{2}}}}
      [{\displaystyle \nabla \,{\times }\!\left({\frac {\mathbf {A} }{\phi
      }}\right)\ =\ {\frac {\phi \,\nabla {\times }\mathbf {A} -(\nabla \!\phi
      ){\times }\mathbf {A} }{\phi ^{2}}}}]
**** Chain rule[edit] ****
Let     f ( x )   {\displaystyle f(x)}  [{\displaystyle f(x)}] be a one-
variable function from scalars to scalars,      r  ( t ) = (  r  1   ( t ) ,
&#x2026; ,  r  n   ( t ) )   {\displaystyle \mathbf {r} (t)=(r_{1}(t),\ldots
,r_{n}(t))}  [{\displaystyle \mathbf {r} (t)=(r_{1}(t),\ldots ,r_{n}(t))}] a
parametrized curve, and     F :   R   n   &#x2192;  R    {\displaystyle F:
\mathbb {R} ^{n}\to \mathbb {R} }  [{\displaystyle F:\mathbb {R} ^{n}\to
\mathbb {R} }] a function from vectors to scalars. We have the following
special cases of the multi-variable chain_rule.
         &#x2207; ( f &#x2218; F )  =  (  f &#x2032;   &#x2218; F )  &#x2207;
      F   {\displaystyle \nabla (f\circ F)\,=\,(f'\!\circ F)\,\nabla \!F}  [
      {\displaystyle \nabla (f\circ F)\,=\,(f'\!\circ F)\,\nabla \!F}]
         ( F &#x2218;  r   ) &#x2032;  = ( &#x2207;  F &#x2218;  r  ) &#x22C5;
      r  &#x2032;    {\displaystyle (F\circ \mathbf {r} )'=(\nabla \!F\circ
      \mathbf {r} )\cdot \mathbf {r} '}  [{\displaystyle (F\circ \mathbf {r}
      )'=(\nabla \!F\circ \mathbf {r} )\cdot \mathbf {r} '}]
         &#x2207; ( F &#x2218;  A  ) &#xA0; = &#xA0; ( &#x2207;  F &#x2218;  A
      )  &#x2207;   A    {\displaystyle \nabla (F\circ \mathbf {A} )\ =\
      (\nabla \!F\circ \mathbf {A} )\,\nabla \!\mathbf {A} }  [{\displaystyle
      \nabla (F\circ \mathbf {A} )\ =\ (\nabla \!F\circ \mathbf {A} )\,\nabla
      \!\mathbf {A} }]
For a coordinate_parametrization     &#x03A6; :   R   n   &#x2192;   R   n
{\displaystyle \Phi :\mathbb {R} ^{n}\to \mathbb {R} ^{n}}  [{\displaystyle
\Phi :\mathbb {R} ^{n}\to \mathbb {R} ^{n}}] we have:
         &#x2207; &#x22C5; (  A  &#x2218; &#x03A6; ) =  t r    (   ( &#x2207;
      A  &#x2218; &#x03A6; )    J   &#x03A6;     )    {\displaystyle \nabla
      \cdot (\mathbf {A} \circ \Phi )=\mathrm {tr} \!\left(\,(\nabla \!\mathbf
      {A} \circ \Phi )\,\mathbf {J} _{\Phi }\,\right)}  [{\displaystyle \nabla
      \cdot (\mathbf {A} \circ \Phi )=\mathrm {tr} \!\left(\,(\nabla \!\mathbf
      {A} \circ \Phi )\,\mathbf {J} _{\Phi }\,\right)}]
Here we take the trace of the product of two n Ã n matrices: the gradient of A
and the Jacobian of Î¦.
**** Dot product rule[edit] ****
             &#x2207; (  A  &#x22C5;  B  )   &#xA0; = &#xA0; (  A   &#x22C5;
      &#x2207; )  B   +  (  B    &#x22C5;  &#x2207; )  A   +   A   &#x00D7;
      ( &#x2207;  &#x00D7;   B  )  +   B   &#x00D7;  ( &#x2207;  &#x00D7;   A
      )      &#xA0; = &#xA0;  A     J    B    +  B     J    A    &#xA0; =
      &#xA0;  A   &#x2207;  B  +  B   &#x2207;   A        {\displaystyle
      {\begin{aligned}\nabla (\mathbf {A} \cdot \mathbf {B} )&\ =\ (\mathbf {A}
      {\cdot }\nabla )\mathbf {B} \,+\,(\mathbf {B} \,{\cdot }\nabla )\mathbf
      {A} \,+\,\mathbf {A} {\times }(\nabla {\times }\mathbf {B} )\,+\,\mathbf
      {B} {\times }(\nabla {\times }\mathbf {A} )\\&\ =\ \mathbf {A} \,\mathbf
      {J} _{\mathbf {B} }+\mathbf {B} \,\mathbf {J} _{\mathbf {A} }\ =\ \mathbf
      {A} \,\nabla \mathbf {B} +\mathbf {B} \,\nabla \!\mathbf {A} \end
      {aligned}}}  [{\displaystyle {\begin{aligned}\nabla (\mathbf {A} \cdot
      \mathbf {B} )&\ =\ (\mathbf {A} {\cdot }\nabla )\mathbf {B} \,+\,(\mathbf
      {B} \,{\cdot }\nabla )\mathbf {A} \,+\,\mathbf {A} {\times }(\nabla
      {\times }\mathbf {B} )\,+\,\mathbf {B} {\times }(\nabla {\times }\mathbf
      {A} )\\&\ =\ \mathbf {A} \,\mathbf {J} _{\mathbf {B} }+\mathbf {B}
      \,\mathbf {J} _{\mathbf {A} }\ =\ \mathbf {A} \,\nabla \mathbf {B}
      +\mathbf {B} \,\nabla \!\mathbf {A} \end{aligned}}}]
where       J    A    = &#x2207;   A  = ( &#x2202;  A  i    /  &#x2202;  x  j
)  i j     {\displaystyle \mathbf {J} _{\mathbf {A} }=\nabla \!\mathbf {A} =
(\partial A_{i}/\partial x_{j})_{ij}}  [{\displaystyle \mathbf {J} _{\mathbf
{A} }=\nabla \!\mathbf {A} =(\partial A_{i}/\partial x_{j})_{ij}}] denotes the
Jacobian_matrix of the vector field      A  = (  A  1   , &#x2026; ,  A  n   )
{\displaystyle \mathbf {A} =(A_{1},\ldots ,A_{n})}  [{\displaystyle \mathbf {A}
=(A_{1},\ldots ,A_{n})}].
Alternatively, using Feynman subscript notation,
         &#x2207; (  A  &#x22C5;  B  ) =  &#x2207;   A    (  A  &#x22C5;  B  )
      +  &#x2207;   B    (  A  &#x22C5;  B  ) &#xA0; .   {\displaystyle \nabla
      (\mathbf {A} \cdot \mathbf {B} )=\nabla _{\mathbf {A} }(\mathbf {A} \cdot
      \mathbf {B} )+\nabla _{\mathbf {B} }(\mathbf {A} \cdot \mathbf {B} )\ .}
      [\nabla (\mathbf {A} \cdot \mathbf {B} )=\nabla _{\mathbf {A} }(\mathbf
      {A} \cdot \mathbf {B} )+\nabla _{\mathbf {B} }(\mathbf {A} \cdot \mathbf
      {B} )\ .]
See these notes.[4]
As a special case, when A = B,
            1 2    &#x2207;  (   A  &#x22C5;  A   )  &#xA0; = &#xA0; (  A
      &#x22C5; &#x2207; )  A  +  A  &#x00D7; ( &#x2207; &#x00D7;  A  ) &#xA0; =
      &#xA0;  A     J    A    &#xA0; = &#xA0;  A   &#x2207;   A  .
      {\displaystyle {\tfrac {1}{2}}\nabla \left(\mathbf {A} \cdot \mathbf {A}
      \right)\ =\ (\mathbf {A} \cdot \nabla )\mathbf {A} +\mathbf {A} \times
      (\nabla \times \mathbf {A} )\ =\ \mathbf {A} \,\mathbf {J} _{\mathbf {A}
      }\ =\ \mathbf {A} \,\nabla \!\mathbf {A} .}  [{\displaystyle {\tfrac {1}
      {2}}\nabla \left(\mathbf {A} \cdot \mathbf {A} \right)\ =\ (\mathbf {A}
      \cdot \nabla )\mathbf {A} +\mathbf {A} \times (\nabla \times \mathbf {A}
      )\ =\ \mathbf {A} \,\mathbf {J} _{\mathbf {A} }\ =\ \mathbf {A} \,\nabla
      \!\mathbf {A} .}]
The generalization of the dot product formula to Riemannian manifolds is a
defining property of a Riemannian_connection, which differentiates a vector
field to give a vector-valued 1-form.
**** Cross product rule[edit] ****
         &#x2207; &#x22C5; (  A  &#x00D7;  B  ) = ( &#x2207; &#x00D7;  A  )
      &#x22C5;  B  &#x2212;  A  &#x22C5; ( &#x2207; &#x00D7;  B  )
      {\displaystyle \nabla \cdot (\mathbf {A} \times \mathbf {B} )=(\nabla
      \times \mathbf {A} )\cdot \mathbf {B} -\mathbf {A} \cdot (\nabla \times
      \mathbf {B} )}  [\nabla \cdot (\mathbf {A} \times \mathbf {B} )=(\nabla
      \times \mathbf {A} )\cdot \mathbf {B} -\mathbf {A} \cdot (\nabla \times
      \mathbf {B} )]
             &#x2207; &#x00D7; (  A  &#x00D7;  B  )    =  A  ( &#x2207;
      &#x22C5;  B  ) &#x2212;  B  ( &#x2207; &#x22C5;  A  ) + (  B  &#x22C5;
      &#x2207; )  A  &#x2212; (  A  &#x22C5; &#x2207; )  B        = ( &#x2207;
      &#x22C5;  B  +  B  &#x22C5; &#x2207; )  A  &#x2212; ( &#x2207; &#x22C5;
      A  +  A  &#x22C5; &#x2207; )  B        = &#x2207; &#x22C5; (  B    A    T
      ) &#x2212; &#x2207; &#x22C5; (  A    B    T    )       = &#x2207;
      &#x22C5; (  B    A    T    &#x2212;  A    B    T    )
      {\displaystyle {\begin{aligned}\nabla \times (\mathbf {A} \times \mathbf
      {B} )&=\mathbf {A} (\nabla \cdot \mathbf {B} )-\mathbf {B} (\nabla \cdot
      \mathbf {A} )+(\mathbf {B} \cdot \nabla )\mathbf {A} -(\mathbf {A} \cdot
      \nabla )\mathbf {B} \\&=(\nabla \cdot \mathbf {B} +\mathbf {B} \cdot
      \nabla )\mathbf {A} -(\nabla \cdot \mathbf {A} +\mathbf {A} \cdot \nabla
      )\mathbf {B} \\&=\nabla \cdot (\mathbf {B} \mathbf {A} ^{\mathrm {T} })-
      \nabla \cdot (\mathbf {A} \mathbf {B} ^{\mathrm {T} })\\&=\nabla \cdot
      (\mathbf {B} \mathbf {A} ^{\mathrm {T} }-\mathbf {A} \mathbf {B} ^
      {\mathrm {T} })\end{aligned}}}  [{\displaystyle {\begin{aligned}\nabla
      \times (\mathbf {A} \times \mathbf {B} )&=\mathbf {A} (\nabla \cdot
      \mathbf {B} )-\mathbf {B} (\nabla \cdot \mathbf {A} )+(\mathbf {B} \cdot
      \nabla )\mathbf {A} -(\mathbf {A} \cdot \nabla )\mathbf {B} \\&=(\nabla
      \cdot \mathbf {B} +\mathbf {B} \cdot \nabla )\mathbf {A} -(\nabla \cdot
      \mathbf {A} +\mathbf {A} \cdot \nabla )\mathbf {B} \\&=\nabla \cdot
      (\mathbf {B} \mathbf {A} ^{\mathrm {T} })-\nabla \cdot (\mathbf {A}
      \mathbf {B} ^{\mathrm {T} })\\&=\nabla \cdot (\mathbf {B} \mathbf {A} ^
      {\mathrm {T} }-\mathbf {A} \mathbf {B} ^{\mathrm {T} })\end{aligned}}}]
***** Second derivatives[edit] *****
**** Curl of gradient is zero[edit] ****
The curl of the gradient of any continuously twice-differentiable scalar_field
&#xA0; &#x03D5;   {\displaystyle \ \phi }  [\ \phi ] is always the zero_vector:
         &#x2207; &#x00D7; ( &#x2207; &#x03D5; ) =  0    {\displaystyle \nabla
      \times (\nabla \phi )=\mathbf {0} }  [\nabla \times (\nabla \phi
      )=\mathbf {0} ]
**** Divergence of curl is zero[edit] ****
The divergence of the curl of any vector_field A is always zero:
         &#x2207; &#x22C5; ( &#x2207; &#x00D7;  A  ) = 0   {\displaystyle
      \nabla \cdot (\nabla \times \mathbf {A} )=0}  [\nabla \cdot (\nabla
      \times \mathbf {A} )=0]
The above two vanishing properties are a special case of the vanishing of the
square of the exterior_derivative in the De_Rham chain_complex.
**** Divergence of gradient[edit] ****
The Laplacian of a scalar field is the divergence of its gradient:
          &#x2207;  2   &#x03C8; = &#x2207; &#x22C5; ( &#x2207; &#x03C8; )
      {\displaystyle \nabla ^{2}\psi =\nabla \cdot (\nabla \psi )}  [\nabla ^
      {2}\psi =\nabla \cdot (\nabla \psi )]
The result is a scalar quantity.
**** Curl of curl[edit] ****
         &#x2207; &#x00D7;  (  &#x2207; &#x00D7;  A   )  = &#x2207; ( &#x2207;
      &#x22C5;  A  ) &#x2212;  &#x2207;  2    A    {\displaystyle \nabla \times
      \left(\nabla \times \mathbf {A} \right)=\nabla (\nabla \cdot \mathbf {A}
      )-\nabla ^{2}\mathbf {A} }  [\nabla \times \left(\nabla \times \mathbf
      {A} \right)=\nabla (\nabla \cdot \mathbf {A} )-\nabla ^{2}\mathbf {A} ]
Here â2 is the vector_Laplacian operating on the vector field A.
***** Summary of important identities[edit] *****
**** Addition and multiplication[edit] ****
    *     A  +  B  =  B  +  A    {\displaystyle \mathbf {A} +\mathbf {B}
      =\mathbf {B} +\mathbf {A} }  [{\displaystyle \mathbf {A} +\mathbf {B}
      =\mathbf {B} +\mathbf {A} }]
    *     A  &#x22C5;  B  =  B  &#x22C5;  A    {\displaystyle \mathbf {A} \cdot
      \mathbf {B} =\mathbf {B} \cdot \mathbf {A} }  [{\displaystyle \mathbf {A}
      \cdot \mathbf {B} =\mathbf {B} \cdot \mathbf {A} }]
    *     A  &#x00D7;  B  =  &#x2212; B  &#x00D7;  A    {\displaystyle \mathbf
      {A} \times \mathbf {B} =\mathbf {-B} \times \mathbf {A} }  [
      {\displaystyle \mathbf {A} \times \mathbf {B} =\mathbf {-B} \times
      \mathbf {A} }]
    *    (  A  +  B  ) &#x22C5;  C  =  A  &#x22C5;  C  +  B  &#x22C5;  C
      {\displaystyle (\mathbf {A} +\mathbf {B} )\cdot \mathbf {C} =\mathbf {A}
      \cdot \mathbf {C} +\mathbf {B} \cdot \mathbf {C} }  [{\displaystyle
      (\mathbf {A} +\mathbf {B} )\cdot \mathbf {C} =\mathbf {A} \cdot \mathbf
      {C} +\mathbf {B} \cdot \mathbf {C} }]
    *    (  A  +  B  ) &#x00D7;  C  =  A  &#x00D7;  C  +  B  &#x00D7;  C
      {\displaystyle (\mathbf {A} +\mathbf {B} )\times \mathbf {C} =\mathbf {A}
      \times \mathbf {C} +\mathbf {B} \times \mathbf {C} }  [{\displaystyle
      (\mathbf {A} +\mathbf {B} )\times \mathbf {C} =\mathbf {A} \times \mathbf
      {C} +\mathbf {B} \times \mathbf {C} }]
    *     A  &#x22C5; (  B  &#x00D7;  C  ) =  B  &#x22C5; (  C  &#x00D7;  A  )
      =  C  &#x22C5; (  A  &#x00D7;  B  )   {\displaystyle \mathbf {A} \cdot
      (\mathbf {B} \times \mathbf {C} )=\mathbf {B} \cdot (\mathbf {C} \times
      \mathbf {A} )=\mathbf {C} \cdot (\mathbf {A} \times \mathbf {B} )}  [
      {\displaystyle \mathbf {A} \cdot (\mathbf {B} \times \mathbf {C}
      )=\mathbf {B} \cdot (\mathbf {C} \times \mathbf {A} )=\mathbf {C} \cdot
      (\mathbf {A} \times \mathbf {B} )}] (scalar_triple_product)
    *     A  &#x00D7; (  B  &#x00D7;  C  ) = (  A  &#x22C5;  C  )  B  &#x2212;
      (  A  &#x22C5;  B  )  C    {\displaystyle \mathbf {A} \times (\mathbf {B}
      \times \mathbf {C} )=(\mathbf {A} \cdot \mathbf {C} )\mathbf {B} -
      (\mathbf {A} \cdot \mathbf {B} )\mathbf {C} }  [{\displaystyle \mathbf
      {A} \times (\mathbf {B} \times \mathbf {C} )=(\mathbf {A} \cdot \mathbf
      {C} )\mathbf {B} -(\mathbf {A} \cdot \mathbf {B} )\mathbf {C} }] (vector
      triple_product)
    *    (  A  &#x00D7;  B  ) &#x00D7;  C  = (  A  &#x22C5;  C  )  B  &#x2212;
      (  B  &#x22C5;  C  )  A    {\displaystyle (\mathbf {A} \times \mathbf {B}
      )\times \mathbf {C} =(\mathbf {A} \cdot \mathbf {C} )\mathbf {B} -
      (\mathbf {B} \cdot \mathbf {C} )\mathbf {A} }  [{\displaystyle (\mathbf
      {A} \times \mathbf {B} )\times \mathbf {C} =(\mathbf {A} \cdot \mathbf
      {C} )\mathbf {B} -(\mathbf {B} \cdot \mathbf {C} )\mathbf {A} }] (vector
      triple_product)
    *     A  &#x00D7; (  B  &#x00D7;  C  ) = (  A  &#x00D7;  B  ) &#x00D7;  C
      +  B  &#x00D7; (  A  &#x00D7;  C  )   {\displaystyle \mathbf {A} \times
      (\mathbf {B} \times \mathbf {C} )=(\mathbf {A} \times \mathbf {B} )\times
      \mathbf {C} +\mathbf {B} \times (\mathbf {A} \times \mathbf {C} )}  [
      {\displaystyle \mathbf {A} \times (\mathbf {B} \times \mathbf {C} )=
      (\mathbf {A} \times \mathbf {B} )\times \mathbf {C} +\mathbf {B} \times
      (\mathbf {A} \times \mathbf {C} )}] (Jacobi_identity)
    *     A  &#x00D7; (  B  &#x00D7;  C  ) +  C  &#x00D7; (  A  &#x00D7;  B  )
      +  B  &#x00D7; (  C  &#x00D7;  A  ) = 0   {\displaystyle \mathbf {A}
      \times (\mathbf {B} \times \mathbf {C} )+\mathbf {C} \times (\mathbf {A}
      \times \mathbf {B} )+\mathbf {B} \times (\mathbf {C} \times \mathbf {A}
      )=0}  [{\displaystyle \mathbf {A} \times (\mathbf {B} \times \mathbf {C}
      )+\mathbf {C} \times (\mathbf {A} \times \mathbf {B} )+\mathbf {B} \times
      (\mathbf {C} \times \mathbf {A} )=0}] (Jacobi_identity)
    *    (  A  &#x00D7;  B  ) &#x22C5; (  C  &#x00D7;  D  ) =  (   A  &#x22C5;
      C   )   (   B  &#x22C5;  D   )  &#x2212;  (   B  &#x22C5;  C   )   (   A
      &#x22C5;  D   )    {\displaystyle (\mathbf {A} \times \mathbf {B} )\cdot
      (\mathbf {C} \times \mathbf {D} )=\left(\mathbf {A} \cdot \mathbf {C}
      \right)\left(\mathbf {B} \cdot \mathbf {D} \right)-\left(\mathbf {B}
      \cdot \mathbf {C} \right)\left(\mathbf {A} \cdot \mathbf {D} \right)}  [
      {\displaystyle (\mathbf {A} \times \mathbf {B} )\cdot (\mathbf {C} \times
      \mathbf {D} )=\left(\mathbf {A} \cdot \mathbf {C} \right)\left(\mathbf
      {B} \cdot \mathbf {D} \right)-\left(\mathbf {B} \cdot \mathbf {C}
      \right)\left(\mathbf {A} \cdot \mathbf {D} \right)}]
    *     (  A  &#x22C5; (  B  &#x00D7;  C  ) )   D  = (  A  &#x22C5;  D  )
      (   B  &#x00D7;  C   )  +  (   B  &#x22C5;  D   )   (   C  &#x00D7;  A
      )  +  (   C  &#x22C5;  D   )   (   A  &#x00D7;  B   )    {\displaystyle
      \!(\mathbf {A} \cdot (\mathbf {B} \times \mathbf {C} ))\,\mathbf {D} =
      (\mathbf {A} \cdot \mathbf {D} )\left(\mathbf {B} \times \mathbf {C}
      \right)+\left(\mathbf {B} \cdot \mathbf {D} \right)\left(\mathbf {C}
      \times \mathbf {A} \right)+\left(\mathbf {C} \cdot \mathbf {D}
      \right)\left(\mathbf {A} \times \mathbf {B} \right)}  [{\displaystyle \!
      (\mathbf {A} \cdot (\mathbf {B} \times \mathbf {C} ))\,\mathbf {D} =
      (\mathbf {A} \cdot \mathbf {D} )\left(\mathbf {B} \times \mathbf {C}
      \right)+\left(\mathbf {B} \cdot \mathbf {D} \right)\left(\mathbf {C}
      \times \mathbf {A} \right)+\left(\mathbf {C} \cdot \mathbf {D}
      \right)\left(\mathbf {A} \times \mathbf {B} \right)}]
    *     (  A  &#x00D7;  B  ) &#x00D7; (  C  &#x00D7;  D  ) =  (   A  &#x22C5;
      (  B  &#x00D7;  D  )  )   C  &#x2212;  (   A  &#x22C5;  (   B  &#x00D7;
      C   )   )   D    {\displaystyle \!(\mathbf {A} \times \mathbf {B} )\times
      (\mathbf {C} \times \mathbf {D} )=\left(\mathbf {A} \cdot (\mathbf {B}
      \times \mathbf {D} )\right)\mathbf {C} -\left(\mathbf {A} \cdot \left
      (\mathbf {B} \times \mathbf {C} \right)\right)\mathbf {D} }  [
      {\displaystyle \!(\mathbf {A} \times \mathbf {B} )\times (\mathbf {C}
      \times \mathbf {D} )=\left(\mathbf {A} \cdot (\mathbf {B} \times \mathbf
      {D} )\right)\mathbf {C} -\left(\mathbf {A} \cdot \left(\mathbf {B} \times
      \mathbf {C} \right)\right)\mathbf {D} }]
**** Differentiation[edit] ****
*** Gradient[edit] ***
    *    &#x2207; ( &#x03C8; + &#x03D5; ) = &#x2207; &#x03C8; + &#x2207;
      &#x03D5;   {\displaystyle \nabla (\psi +\phi )=\nabla \psi +\nabla \phi }
      [{\displaystyle \nabla (\psi +\phi )=\nabla \psi +\nabla \phi }]
    *    &#x2207; ( &#x03C8; &#x03D5; ) = &#x03D5; &#x2207; &#x03C8; + &#x03C8;
      &#x2207; &#x03D5;   {\displaystyle \nabla (\psi \phi )=\phi \nabla \psi
      +\psi \nabla \phi }  [{\displaystyle \nabla (\psi \phi )=\phi \nabla \psi
      +\psi \nabla \phi }]
    *    &#x2207; ( &#x03C8;  A  ) = &#x2207; &#x03C8; &#x2297;  A  + &#x03C8;
      &#x2207;  A    {\displaystyle \nabla (\psi \mathbf {A} )=\nabla \psi
      \otimes \mathbf {A} +\psi \nabla \mathbf {A} }  [{\displaystyle \nabla
      (\psi \mathbf {A} )=\nabla \psi \otimes \mathbf {A} +\psi \nabla \mathbf
      {A} }]
    *    &#x2207; (  A  &#x22C5;  B  ) = (  A  &#x22C5; &#x2207; )  B  + (  B
      &#x22C5; &#x2207; )  A  +  A  &#x00D7; ( &#x2207; &#x00D7;  B  ) +  B
      &#x00D7;  (  &#x2207; &#x00D7;  A   )    {\displaystyle \nabla (\mathbf
      {A} \cdot \mathbf {B} )=(\mathbf {A} \cdot \nabla )\mathbf {B} +(\mathbf
      {B} \cdot \nabla )\mathbf {A} +\mathbf {A} \times (\nabla \times \mathbf
      {B} )+\mathbf {B} \times \left(\nabla \times \mathbf {A} \right)}  [
      {\displaystyle \nabla (\mathbf {A} \cdot \mathbf {B} )=(\mathbf {A} \cdot
      \nabla )\mathbf {B} +(\mathbf {B} \cdot \nabla )\mathbf {A} +\mathbf {A}
      \times (\nabla \times \mathbf {B} )+\mathbf {B} \times \left(\nabla
      \times \mathbf {A} \right)}]
*** Divergence[edit] ***
    *    &#x2207; &#x22C5; (  A  +  B  ) = &#x2207; &#x22C5;  A  + &#x2207;
      &#x22C5;  B    {\displaystyle \nabla \cdot (\mathbf {A} +\mathbf {B}
      )=\nabla \cdot \mathbf {A} +\nabla \cdot \mathbf {B} }  [{\displaystyle
      \nabla \cdot (\mathbf {A} +\mathbf {B} )=\nabla \cdot \mathbf {A} +\nabla
      \cdot \mathbf {B} }]
    *    &#x2207; &#x22C5;  (  &#x03C8;  A   )  = &#x03C8; &#x2207; &#x22C5;  A
      +  A  &#x22C5; &#x2207; &#x03C8;   {\displaystyle \nabla \cdot \left(\psi
      \mathbf {A} \right)=\psi \nabla \cdot \mathbf {A} +\mathbf {A} \cdot
      \nabla \psi }  [{\displaystyle \nabla \cdot \left(\psi \mathbf {A}
      \right)=\psi \nabla \cdot \mathbf {A} +\mathbf {A} \cdot \nabla \psi }]
    *    &#x2207; &#x22C5;  (   A  &#x00D7;  B   )  = ( &#x2207; &#x00D7;  A  )
      &#x22C5;  B  &#x2212; ( &#x2207; &#x00D7;  B  ) &#x22C5;  A
      {\displaystyle \nabla \cdot \left(\mathbf {A} \times \mathbf {B} \right)=
      (\nabla \times \mathbf {A} )\cdot \mathbf {B} -(\nabla \times \mathbf {B}
      )\cdot \mathbf {A} }  [{\displaystyle \nabla \cdot \left(\mathbf {A}
      \times \mathbf {B} \right)=(\nabla \times \mathbf {A} )\cdot \mathbf {B}
      -(\nabla \times \mathbf {B} )\cdot \mathbf {A} }]
*** Curl[edit] ***
    *    &#x2207; &#x00D7; (  A  +  B  ) = &#x2207; &#x00D7;  A  + &#x2207;
      &#x00D7;  B    {\displaystyle \nabla \times (\mathbf {A} +\mathbf {B}
      )=\nabla \times \mathbf {A} +\nabla \times \mathbf {B} }  [{\displaystyle
      \nabla \times (\mathbf {A} +\mathbf {B} )=\nabla \times \mathbf {A}
      +\nabla \times \mathbf {B} }]
    *    &#x2207; &#x00D7;  (  &#x03C8;  A   )  = &#x03C8;  ( &#x2207; &#x00D7;
      A  ) + &#x2207; &#x03C8; &#x00D7;  A    {\displaystyle \nabla \times
      \left(\psi \mathbf {A} \right)=\psi \,(\nabla \times \mathbf {A} )+\nabla
      \psi \times \mathbf {A} }  [{\displaystyle \nabla \times \left(\psi
      \mathbf {A} \right)=\psi \,(\nabla \times \mathbf {A} )+\nabla \psi
      \times \mathbf {A} }]
    *    &#x2207; &#x00D7;  (  &#x03C8; &#x2207; &#x03D5;  )  = &#x2207;
      &#x03C8; &#x00D7; &#x2207; &#x03D5;   {\displaystyle \nabla \times \left
      (\psi \nabla \phi \right)=\nabla \psi \times \nabla \phi }  [
      {\displaystyle \nabla \times \left(\psi \nabla \phi \right)=\nabla \psi
      \times \nabla \phi }]
    *    &#x2207; &#x00D7;  (   A  &#x00D7;  B   )  =  A   (  &#x2207; &#x22C5;
      B   )  &#x2212;  B   (  &#x2207; &#x22C5;  A   )  +  (   B  &#x22C5;
      &#x2207;  )   A  &#x2212;  (   A  &#x22C5; &#x2207;  )   B
      {\displaystyle \nabla \times \left(\mathbf {A} \times \mathbf {B}
      \right)=\mathbf {A} \left(\nabla \cdot \mathbf {B} \right)-\mathbf {B}
      \left(\nabla \cdot \mathbf {A} \right)+\left(\mathbf {B} \cdot \nabla
      \right)\mathbf {A} -\left(\mathbf {A} \cdot \nabla \right)\mathbf {B} }
      [{\displaystyle \nabla \times \left(\mathbf {A} \times \mathbf {B}
      \right)=\mathbf {A} \left(\nabla \cdot \mathbf {B} \right)-\mathbf {B}
      \left(\nabla \cdot \mathbf {A} \right)+\left(\mathbf {B} \cdot \nabla
      \right)\mathbf {A} -\left(\mathbf {A} \cdot \nabla \right)\mathbf {B} }]
*** Second derivatives[edit] ***
DCG chart: A simple chart depicting all rules pertaining to second derivatives.
D, C, G, L and CC stand for divergence, curl, gradient, Laplacian and curl of
curl, respectively. Arrows indicate existence of second derivatives. Blue
circle in the middle represents curl of curl, whereas the other two red circles
(dashed) mean that DD and GG do not exist.
    *    &#x2207; &#x22C5; ( &#x2207; &#x00D7;  A  ) = 0   {\displaystyle
      \nabla \cdot (\nabla \times \mathbf {A} )=0}  [{\displaystyle \nabla
      \cdot (\nabla \times \mathbf {A} )=0}]
    *    &#x2207; &#x00D7; ( &#x2207; &#x03C8; ) =  0    {\displaystyle \nabla
      \times (\nabla \psi )=\mathbf {0} }  [{\displaystyle \nabla \times
      (\nabla \psi )=\mathbf {0} }]
    *    &#x2207; &#x22C5; ( &#x2207; &#x03C8; ) =  &#x2207;  2   &#x03C8;
      {\displaystyle \nabla \cdot (\nabla \psi )=\nabla ^{2}\psi }  [
      {\displaystyle \nabla \cdot (\nabla \psi )=\nabla ^{2}\psi }] (scalar
      Laplacian)
    *    &#x2207;  (  &#x2207; &#x22C5;  A   )  &#x2212; &#x2207; &#x00D7;
      (  &#x2207; &#x00D7;  A   )  =  &#x2207;  2    A    {\displaystyle \nabla
      \left(\nabla \cdot \mathbf {A} \right)-\nabla \times \left(\nabla \times
      \mathbf {A} \right)=\nabla ^{2}\mathbf {A} }  [{\displaystyle \nabla
      \left(\nabla \cdot \mathbf {A} \right)-\nabla \times \left(\nabla \times
      \mathbf {A} \right)=\nabla ^{2}\mathbf {A} }] (vector_Laplacian)
    *    &#x2207; &#x22C5; ( &#x03D5; &#x2207; &#x03C8; ) = &#x03D5;  &#x2207;
      2   &#x03C8; + &#x2207; &#x03D5; &#x22C5; &#x2207; &#x03C8;
      {\displaystyle \nabla \cdot (\phi \nabla \psi )=\phi \nabla ^{2}\psi
      +\nabla \phi \cdot \nabla \psi }  [{\displaystyle \nabla \cdot (\phi
      \nabla \psi )=\phi \nabla ^{2}\psi +\nabla \phi \cdot \nabla \psi }]
    *    &#x03C8;  &#x2207;  2   &#x03D5; &#x2212; &#x03D5;  &#x2207;  2
      &#x03C8; = &#x2207; &#x22C5;  (  &#x03C8; &#x2207; &#x03D5; &#x2212;
      &#x03D5; &#x2207; &#x03C8;  )    {\displaystyle \psi \nabla ^{2}\phi -
      \phi \nabla ^{2}\psi =\nabla \cdot \left(\psi \nabla \phi -\phi \nabla
      \psi \right)}  [{\displaystyle \psi \nabla ^{2}\phi -\phi \nabla ^{2}\psi
      =\nabla \cdot \left(\psi \nabla \phi -\phi \nabla \psi \right)}]
    *     &#x2207;  2   ( &#x03D5; &#x03C8; ) = &#x03D5;  &#x2207;  2
      &#x03C8; + 2 ( &#x2207; &#x03D5; ) &#x22C5; ( &#x2207; &#x03C8; ) +
      (  &#x2207;  2   &#x03D5; ) &#x03C8;   {\displaystyle \nabla ^{2}(\phi
      \psi )=\phi \nabla ^{2}\psi +2(\nabla \phi )\cdot (\nabla \psi )+(\nabla
      ^{2}\phi )\psi }  [{\displaystyle \nabla ^{2}(\phi \psi )=\phi \nabla ^
      {2}\psi +2(\nabla \phi )\cdot (\nabla \psi )+(\nabla ^{2}\phi )\psi }]
    *     &#x2207;  2   ( &#x03C8;  A  ) =  A   &#x2207;  2   &#x03C8; + 2
      ( &#x2207; &#x03C8; &#x22C5; &#x2207; )  A  + &#x03C8;  &#x2207;  2    A
      {\displaystyle \nabla ^{2}(\psi \mathbf {A} )=\mathbf {A} \nabla ^{2}\psi
      +2(\nabla \psi \cdot \nabla )\mathbf {A} +\psi \nabla ^{2}\mathbf {A} }
      [{\displaystyle \nabla ^{2}(\psi \mathbf {A} )=\mathbf {A} \nabla ^
      {2}\psi +2(\nabla \psi \cdot \nabla )\mathbf {A} +\psi \nabla ^{2}\mathbf
      {A} }]
    *     &#x2207;  2   (  A  &#x22C5;  B  ) &#xA0; = &#xA0;  A   &#x22C5;
      &#x2207;  2    B   &#x2212;   B   &#x22C5;   &#x2207;  2     A   +  2
      &#x2207;  &#x22C5;   ( (  B  &#x22C5; &#x2207; )  A   +   B   &#x00D7;
      ( &#x2207;  &#x00D7;   A  ) )   {\displaystyle \nabla ^{2}(\mathbf {A}
      \cdot \mathbf {B} )\ =\ \mathbf {A} {\cdot }\nabla ^{2}\mathbf {B} \,-
      \,\mathbf {B} {\cdot }\nabla ^{2}\!\mathbf {A} \,+\,2\nabla {\cdot }\,(
      (\mathbf {B} \cdot \nabla )\mathbf {A} \,+\,\mathbf {B} {\times }(\nabla
      {\times }\mathbf {A} ))}  [{\displaystyle \nabla ^{2}(\mathbf {A} \cdot
      \mathbf {B} )\ =\ \mathbf {A} {\cdot }\nabla ^{2}\mathbf {B} \,-\,\mathbf
      {B} {\cdot }\nabla ^{2}\!\mathbf {A} \,+\,2\nabla {\cdot }\,((\mathbf {B}
      \cdot \nabla )\mathbf {A} \,+\,\mathbf {B} {\times }(\nabla {\times
      }\mathbf {A} ))}] (Green's_vector_identity)
*** Third derivatives[edit] ***
    *     &#x2207;  2   ( &#x2207; &#x03C8; ) = &#x2207; ( &#x2207; &#x22C5;
      ( &#x2207; &#x03C8; ) ) = &#x2207; (  &#x2207;  2   &#x03C8; )
      {\displaystyle \nabla ^{2}(\nabla \psi )=\nabla (\nabla \cdot (\nabla
      \psi ))=\nabla (\nabla ^{2}\psi )}  [\nabla ^{2}(\nabla \psi )=\nabla
      (\nabla \cdot (\nabla \psi ))=\nabla (\nabla ^{2}\psi )]
    *     &#x2207;  2   ( &#x2207; &#x22C5;  A  ) = &#x2207; &#x22C5;
      ( &#x2207; ( &#x2207; &#x22C5;  A  ) ) = &#x2207; &#x22C5; (  &#x2207;  2
      A  )   {\displaystyle \nabla ^{2}(\nabla \cdot \mathbf {A} )=\nabla \cdot
      (\nabla (\nabla \cdot \mathbf {A} ))=\nabla \cdot (\nabla ^{2}\mathbf {A}
      )}  [{\displaystyle \nabla ^{2}(\nabla \cdot \mathbf {A} )=\nabla \cdot
      (\nabla (\nabla \cdot \mathbf {A} ))=\nabla \cdot (\nabla ^{2}\mathbf {A}
      )}]
    *     &#x2207;  2   ( &#x2207; &#x00D7;  A  ) = &#x2212; &#x2207; &#x00D7;
      ( &#x2207; &#x00D7; ( &#x2207; &#x00D7;  A  ) ) = &#x2207; &#x00D7;
      (  &#x2207;  2    A  )   {\displaystyle \nabla ^{2}(\nabla \times \mathbf
      {A} )=-\nabla \times (\nabla \times (\nabla \times \mathbf {A} ))=\nabla
      \times (\nabla ^{2}\mathbf {A} )}  [{\displaystyle \nabla ^{2}(\nabla
      \times \mathbf {A} )=-\nabla \times (\nabla \times (\nabla \times \mathbf
      {A} ))=\nabla \times (\nabla ^{2}\mathbf {A} )}]
**** Integration[edit] ****
Below, the curly symbol â means "boundary_of".
*** Surfaceâvolume integrals[edit] ***
In the following surfaceâvolume integral theorems, V denotes a three-
dimensional volume with a corresponding two-dimensional boundary S = âV (a
closed_surface):
    * [\oiint]     &#x2202; V    {\displaystyle \scriptstyle \partial V}
      [\scriptstyle \partial V]      A  &#x22C5; d  S  &#xA0; = &#xA0;
      &#x222D;  V    (  &#x2207; &#x22C5;  A   )  d V   {\displaystyle \mathbf
      {A} \cdot d\mathbf {S} \ =\ \iiint _{V}\left(\nabla \cdot \mathbf {A}
      \right)dV}  [{\displaystyle \mathbf {A} \cdot d\mathbf {S} \ =\ \iiint _
      {V}\left(\nabla \cdot \mathbf {A} \right)dV}] (Divergence_theorem)
    * [\oiint]     &#x2202; V    {\displaystyle \scriptstyle \partial V}
      [\scriptstyle \partial V]     &#x03C8;  d  S  &#xA0; = &#xA0;  &#x222D;
      V   &#x2207; &#x03C8;  d V   {\displaystyle \psi \,d\mathbf {S} \ =\
      \iiint _{V}\nabla \psi \,dV}  [{\displaystyle \psi \,d\mathbf {S} \ =\
      \iiint _{V}\nabla \psi \,dV}]
    * [\oiint]     &#x2202; V    {\displaystyle \scriptstyle \partial V}
      [\scriptstyle \partial V]      (      n  &#x005E;    &#x00D7;  A   )  d S
      =  &#x222D;  V    (  &#x2207; &#x00D7;  A   )  d V   {\displaystyle \left
      ({\hat {\mathbf {n} }}\times \mathbf {A} \right)dS=\iiint _{V}\left
      (\nabla \times \mathbf {A} \right)dV}  [\left({\hat {\mathbf {n} }}\times
      \mathbf {A} \right)dS=\iiint _{V}\left(\nabla \times \mathbf {A}
      \right)dV]
    * [\oiint]     &#x2202; V    {\displaystyle \scriptstyle \partial V}
      [\scriptstyle \partial V]     &#x03C8;  (  &#x2207; &#x03C6; &#x22C5;
      n  &#x005E;     )  d S =  &#x222D;  V    (  &#x03C8;  &#x2207;  2
      &#x03C6; + &#x2207; &#x03C6; &#x22C5; &#x2207; &#x03C8;  )  d V
      {\displaystyle \psi \left(\nabla \varphi \cdot {\hat {\mathbf {n}
      }}\right)dS=\iiint _{V}\left(\psi \nabla ^{2}\varphi +\nabla \varphi
      \cdot \nabla \psi \right)dV}  [\psi \left(\nabla \varphi \cdot {\hat
      {\mathbf {n} }}\right)dS=\iiint _{V}\left(\psi \nabla ^{2}\varphi +\nabla
      \varphi \cdot \nabla \psi \right)dV] (Green's_first_identity)
    * [\oiint]     &#x2202; V    {\displaystyle \scriptstyle \partial V}
      [\scriptstyle \partial V]      [   (  &#x03C8; &#x2207; &#x03C6; &#x2212;
      &#x03C6; &#x2207; &#x03C8;  )  &#x22C5;     n  &#x005E;     ]  d S =
      {\displaystyle \left[\left(\psi \nabla \varphi -\varphi \nabla \psi
      \right)\cdot {\hat {\mathbf {n} }}\right]dS=}  [{\displaystyle \left
      [\left(\psi \nabla \varphi -\varphi \nabla \psi \right)\cdot {\hat
      {\mathbf {n} }}\right]dS=}] [\oiint]     &#x2202; V    {\displaystyle
      \scriptstyle \partial V}  [\scriptstyle \partial V]      [  &#x03C8;
      &#x2202; &#x03C6;   &#x2202; n    &#x2212; &#x03C6;    &#x2202; &#x03C8;
      &#x2202; n     ]  d S   {\displaystyle \left[\psi {\frac {\partial
      \varphi }{\partial n}}-\varphi {\frac {\partial \psi }{\partial
      n}}\right]dS}  [\left[\psi {\frac {\partial \varphi }{\partial n}}-
      \varphi {\frac {\partial \psi }{\partial n}}\right]dS]      =  &#x222D;
      V    (  &#x03C8;  &#x2207;  2   &#x03C6; &#x2212; &#x03C6;  &#x2207;  2
      &#x03C8;  )  d V    {\displaystyle \displaystyle =\iiint _{V}\left(\psi
      \nabla ^{2}\varphi -\varphi \nabla ^{2}\psi \right)dV}  [{\displaystyle
      \displaystyle =\iiint _{V}\left(\psi \nabla ^{2}\varphi -\varphi \nabla ^
      {2}\psi \right)dV}] (Green's_second_identity)
    *     &#x222D;  V    (   A  &#x22C5; &#x2207; &#x03C8;  )  d V =
      {\displaystyle \iiint _{V}\left(\mathbf {A} \cdot \nabla \psi \right)dV=}
      [{\displaystyle \iiint _{V}\left(\mathbf {A} \cdot \nabla \psi
      \right)dV=}] [\oiint]     &#x2202; V    {\displaystyle \scriptstyle
      \partial V}  [\scriptstyle \partial V]      (  &#x03C8;  A   )  &#x22C5;
      n  &#x005E;     d S &#x2212;  &#x222D;  V    (  &#x03C8;  &#x2207;
      &#x22C5;   A   )  d V   {\displaystyle \left(\psi \mathbf {A}
      \right)\cdot {\hat {\mathbf {n} }}\,dS-\iiint _{V}\left(\psi \,\nabla
      {\cdot }\mathbf {A} \right)dV}  [{\displaystyle \left(\psi \mathbf {A}
      \right)\cdot {\hat {\mathbf {n} }}\,dS-\iiint _{V}\left(\psi \,\nabla
      {\cdot }\mathbf {A} \right)dV}] (Integration_by_parts)
*** Curveâsurface integrals[edit] ***
In the following curveâsurface integral theorems, S denotes a 2d open surface
with a corresponding 1d boundary C = âS (a closed_curve):
    *        &#x222E;       &#x2202; S   &#x2061;  A  &#x22C5; d  &#x2113;  =
      &#x222C;  S    (  &#x2207; &#x00D7;  A   )  &#x22C5; d  S
      {\displaystyle \oint _{\partial S}\mathbf {A} \cdot d{\boldsymbol {\ell
      }}=\iint _{S}\left(\nabla \times \mathbf {A} \right)\cdot d\mathbf {S} }
      [{\displaystyle \oint _{\partial S}\mathbf {A} \cdot d{\boldsymbol {\ell
      }}=\iint _{S}\left(\nabla \times \mathbf {A} \right)\cdot d\mathbf {S} }]
      (Stokes'_theorem)
    *        &#x222E;       &#x2202; S   &#x2061; &#x03C8; d  &#x2113;  =
      &#x222C;  S    (      n  &#x005E;    &#x00D7; &#x2207; &#x03C8;  )  d S
      {\displaystyle \oint _{\partial S}\psi d{\boldsymbol {\ell }}=\iint _
      {S}\left({\hat {\mathbf {n} }}\times \nabla \psi \right)dS}  [\oint _
      {\partial S}\psi d{\boldsymbol {\ell }}=\iint _{S}\left({\hat {\mathbf
      {n} }}\times \nabla \psi \right)dS]
Integration around a closed curve in the clockwise sense is the negative of the
same line integral in the counterclockwise sense (analogous to interchanging
the limits in a definite_integral):
      [\ointclockwise]      &#x2202; S     {\displaystyle {\scriptstyle
      \partial S}}  [{\scriptstyle \partial S}]      A  &#x22C5;   d
      &#x2113;  = &#x2212;   {\displaystyle \mathbf {A} \cdot {\rm {d}}
      {\boldsymbol {\ell }}=-}  [\mathbf {A} \cdot {\rm {d}}{\boldsymbol {\ell
      }}=-] [\ointctrclockwise]      &#x2202; S     {\displaystyle
      {\scriptstyle \partial S}}  [{\scriptstyle \partial S}]      A  &#x22C5;
      d    &#x2113;  .   {\displaystyle \mathbf {A} \cdot {\rm {d}}{\boldsymbol
      {\ell }}.}  [\mathbf {A} \cdot {\rm {d}}{\boldsymbol {\ell }}.]

***** See also[edit] *****
    * Exterior_calculus_identities
    * Exterior_derivative
    * Vector_calculus
    * Del_in_cylindrical_and_spherical_coordinates
    * Comparison_of_vector_algebra_and_geometric_algebra
***** References[edit] *****
   1. ^Feynman, R. P.; Leighton, R. B.; Sands, M. (1964). The Feynman Lectures
      on Physics. Addison-Wesley. Vol II, p. 27â4. ISBN 0-8053-9049-9.
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
   3. ^Kholmetskii, A. L.; Missevitch, O. V. (2005). "The_Faraday_induction_law
      in_relativity_theory" (PDF). p. 4. arXiv:physics/0504223.
   4. ^Doran,_C.; Lasenby, A. (2003). Geometric algebra for physicists.
      Cambridge University Press. p. 169. ISBN 978-0-521-71595-9.
   5. ^Kelly, P. (2013). "Chapter_1.14_Tensor_Calculus_1:_Tensor_Fields" (PDF).
      Mechanics_Lecture_Notes_Part_III:_Foundations_of_Continuum_Mechanics.
      University of Auckland. Retrieved 7 December 2017.
***** Further reading[edit] *****
    * Balanis, Constantine A. Advanced Engineering Electromagnetics. ISBN 0-
      471-62194-3.
Schey, H. M. (1997). Div Grad Curl and all that: An informal text on vector
calculus. W. W. Norton & Company. ISBN 0-393-96997-5.
Griffiths, David J. (1999). Introduction to Electrodynamics. Prentice Hall.
ISBN 0-13-805326-X.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Vector_calculus_identities&oldid=905898549"
Categories:
    * Vector_calculus
    * Mathematical_identities
    * Mathematics-related_lists
Hidden categories:
    * Articles_lacking_in-text_citations_from_August_2017
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
    * Bosanski
    * Esperanto
    * FranÃ§ais
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 12 July 2019, at 06:28 (UTC).
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
