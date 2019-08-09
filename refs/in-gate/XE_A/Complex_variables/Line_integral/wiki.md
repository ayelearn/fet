The following text has been accessed from https://en.wikipedia.org/wiki/Line_integral at Fri Aug 9 00:03:20 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Line integral ******
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
    * Line integral
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
In mathematics, a line integral is an integral where the function to be
integrated is evaluated along a curve.[1] The terms path integral, curve
integral, and curvilinear integral are also used; contour_integral as well,
although that is typically reserved for line_integrals_in_the_complex_plane.
The function to be integrated may be a scalar_field or a vector_field. The
value of the line integral is the sum of values of the field at all points on
the curve, weighted by some scalar function on the curve (commonly arc_length
or, for a vector field, the scalar_product of the vector field with a
differential vector in the curve). This weighting distinguishes the line
integral from simpler integrals defined on intervals. Many simple formulae in
physics (for example, W = F Â· s) have natural continuous analogs in terms of
line integrals (W = â«C F Â· ds). The line integral finds the work done on an
object moving through an electric or gravitational field, for example.
⁰
***** Contents *****
    * 1_Vector_calculus
          o 1.1_Line_integral_of_a_scalar_field
                # 1.1.1_Definition
                # 1.1.2_Derivation
          o 1.2_Line_integral_of_a_vector_field
                # 1.2.1_Definition
                # 1.2.2_Derivation
          o 1.3_Path_independence
          o 1.4_Applications
    * 2_Flow_across_a_curve
    * 3_Complex_line_integral
          o 3.1_Example
          o 3.2_Relation_between_the_line_integral_of_a_vector_field_and_the
            complex_line_integral
    * 4_Geometric_Line_integral
    * 5_Quantum_mechanics
    * 6_See_also
    * 7_References
    * 8_External_links
***** Vector calculus[edit] *****
In qualitative terms, a line integral in vector calculus can be thought of as a
measure of the total effect of a given tensor_field along a given curve. For
example, the line integral over a scalar field (rank 0 tensor) can be
interpreted as the area under the field carved out by a particular curve. This
can be visualized as the surface created by z = f(x,y) and a curve C in the x-
y plane. The line integral of f would be the area of the "curtain" created when
the points of the surface that are directly over C are carved out.
**** Line integral of a scalar field[edit] ****
The line integral over a scalar field f can be thought of as the area under the
curve C along a surface z = f(x,y), described by the field.
*** Definition[edit] ***
For some scalar_field     f :  U  &#x2286;   R   n   &#x2192;  R
{\displaystyle f:\mathbb {U} \subseteq \mathbb {R} ^{n}\rightarrow \mathbb {R}
}  [{\displaystyle f:\mathbb {U} \subseteq \mathbb {R} ^{n}\rightarrow \mathbb
{R} }], the line integral along a piecewise_smooth curve       C   &#x2282;  U
{\displaystyle {\mathcal {C}}\subset \mathbb {U} }  [{\displaystyle {\mathcal
{C}}\subset \mathbb {U} }] is defined as
          &#x222B;   C    f (  r  )  d s =  &#x222B;  a   b   f  (   r  ( t )
      )   |    r  &#x2032;  ( t )  |   d t .   {\displaystyle \int _{\mathcal
      {C}}f(\mathbf {r} )\,ds=\int _{a}^{b}f\left(\mathbf {r}
      (t)\right)|\mathbf {r} '(t)|\,dt.}  [{\displaystyle \int _{\mathcal {C}}f
      (\mathbf {r} )\,ds=\int _{a}^{b}f\left(\mathbf {r} (t)\right)|\mathbf {r}
      '(t)|\,dt.}]
where      r  : [ a , b ] &#x2192;   C     {\displaystyle \mathbf {r} :
[a,b]\rightarrow {\mathcal {C}}}  [{\displaystyle \mathbf {r} :[a,b]\rightarrow
{\mathcal {C}}}] is an arbitrary bijective parametrization of the curve       C
{\displaystyle {\mathcal {C}}}  [{\mathcal {C}}] such that      r  ( a )
{\displaystyle \mathbf {r} (a)}  [{\displaystyle \mathbf {r} (a)}] and      r
( b )   {\displaystyle \mathbf {r} (b)}  [{\displaystyle \mathbf {r} (b)}] give
the endpoints of       C     {\displaystyle {\mathcal {C}}}  [{\mathcal {C}}]
and     a < b   {\displaystyle a<b}  [a<b]. Here, and in the rest of the
article, the absolute value bars denote the standard_(euclidean)_norm of a
vector.
The function     f   {\displaystyle f}  [f] is called the integrand, the curve
C     {\displaystyle {\mathcal {C}}}  [{\mathcal {C}}] is the domain of
integration, and the symbol     d s   {\displaystyle ds}  [ds] may be
intuitively interpreted as an elementary arc_length. Line integrals of scalar
fields over a curve       C     {\displaystyle {\mathcal {C}}}  [{\mathcal
{C}}] do not depend on the chosen parametrization      r    {\displaystyle
\mathbf {r} }  [\mathbf {r} ] of       C     {\displaystyle {\mathcal {C}}}  [
{\mathcal {C}}].
Geometrically, when the scalar field     f   {\displaystyle f}  [f] is defined
over a plane     ( n = 2 )   {\displaystyle (n=2)}  [{\displaystyle (n=2)}],
its graph is a surface     z = f ( x , y )   {\displaystyle z=f(x,y)}  [z=f
(x,y)] in space, and the line integral gives the (signed) cross-sectional area
bounded by the curve       C     {\displaystyle {\mathcal {C}}}  [{\mathcal
{C}}] and the graph of     f   {\displaystyle f}  [f]. See the animation to the
right.
*** Derivation[edit] ***
For a line integral over a scalar field, the integral can be constructed from a
Riemann_sum using the above definitions of f, C and a parametrization r of C.
This can be done by partitioning the interval [a,b] into n sub-intervals [ti-1,
ti] of length Ît = (b â a)/n, then r(ti) denotes some point, call it a
sample point, on the curve C. We can use the set of sample points {r(ti) : 1
â¤ i â¤ n} to approximate the curve C by a polygonal_path by introducing a
straight line piece between each of the sample points r(ti-1) and r(ti). We
then label the distance between each of the sample points on the curve as Îsi.
The product of f(r(ti)) and Îsi can be associated with the signed area of a
rectangle with a height and width of f(r(ti)) and Îsi respectively. Taking the
limit of the sum of the terms as the length of the partitions approaches zero
gives us
         I =  lim  &#x0394;  s  i   &#x2192; 0    &#x2211;  i = 1   n   f (  r
      (  t  i   ) )  &#x0394;  s  i   .   {\displaystyle I=\lim _{\Delta s_
      {i}\rightarrow 0}\sum _{i=1}^{n}f(\mathbf {r} (t_{i}))\,\Delta s_{i}.}  [
      {\displaystyle I=\lim _{\Delta s_{i}\rightarrow 0}\sum _{i=1}^{n}f
      (\mathbf {r} (t_{i}))\,\Delta s_{i}.}]
We note that, by the mean_value_theorem, the distance between subsequent points
on the curve, is
         &#x0394;  s  i   =  |   r  (  t  i   + &#x0394; t ) &#x2212;  r  (  t
      i   )  |  &#x2248;  |    r  &#x2032;  (  t  i   )  |   &#x0394; t .
      {\displaystyle \Delta s_{i}=|\mathbf {r} (t_{i}+\Delta t)-\mathbf {r} (t_
      {i})|\approx |\mathbf {r} '(t_{i})|\,\Delta t.}  [{\displaystyle \Delta
      s_{i}=|\mathbf {r} (t_{i}+\Delta t)-\mathbf {r} (t_{i})|\approx |\mathbf
      {r} '(t_{i})|\,\Delta t.}]
Substituting this in the above Riemann sum yields
         I =  lim  &#x0394; t &#x2192; 0    &#x2211;  i = 1   n   f (  r  (  t
      i   ) )  |    r  &#x2032;  (  t  i   )  |   &#x0394; t   {\displaystyle
      I=\lim _{\Delta t\rightarrow 0}\sum _{i=1}^{n}f(\mathbf {r} (t_
      {i}))|\mathbf {r} '(t_{i})|\,\Delta t}  [{\displaystyle I=\lim _{\Delta
      t\rightarrow 0}\sum _{i=1}^{n}f(\mathbf {r} (t_{i}))|\mathbf {r} '(t_
      {i})|\,\Delta t}]
which is the Riemann sum for the integral
         I =  &#x222B;  a   b   f (  r  ( t ) )  |    r  &#x2032;  ( t )  |   d
      t .   {\displaystyle I=\int _{a}^{b}f(\mathbf {r} (t))|\mathbf {r} '
      (t)|\,dt.}  [I=\int _{a}^{b}f(\mathbf {r} (t))|\mathbf {r} '(t)|\,dt.]
**** Line integral of a vector field[edit] ****
*** Definition[edit] ***
For a vector_field F : U â Rn â Rn, the line integral along a piecewise
smooth curve C â U, in the direction of r, is defined as
          &#x222B;  C    F  (  r  ) &#x22C5;  d  r  =  &#x222B;  a   b    F
      (  r  ( t ) ) &#x22C5;   r  &#x2032;  ( t )  d t .   {\displaystyle \int
      _{C}\mathbf {F} (\mathbf {r} )\cdot \,d\mathbf {r} =\int _{a}^{b}\mathbf
      {F} (\mathbf {r} (t))\cdot \mathbf {r} '(t)\,dt.}  [{\displaystyle \int _
      {C}\mathbf {F} (\mathbf {r} )\cdot \,d\mathbf {r} =\int _{a}^{b}\mathbf
      {F} (\mathbf {r} (t))\cdot \mathbf {r} '(t)\,dt.}]
where Â· is the dot_product and r: [a, b] â C is a bijective parametrization
of the curve C such that r(a) and r(b) give the endpoints of C.
A line integral of a scalar field is thus a line integral of a vector field
where the vectors are always tangential to the line.
Line integrals of vector fields are independent of the parametrization r in
absolute_value, but they do depend on its orientation. Specifically, a reversal
in the orientation of the parametrization changes the sign of the line
integral.
From the viewpoint of differential_geometry, the line integral of a vector
field along a curve is the integral of the corresponding 1-form under the
musical_isomorphism (which takes the vector field to the corresponding covector
field) over the curve considered as an immersed 1-manifold.
*** Derivation[edit] ***
The trajectory of a particle (in red) along a curve inside a vector field.
Starting from a, the particle traces the path C along the vector field F. The
dot product (green line) of its tangent vector (red arrow) and the field vector
(blue arrow) defines an area under a curve, which is equivalent to the path's
line integral. (Click on image for a detailed description.)
The line integral of a vector field can be derived in a manner very similar to
the case of a scalar field, but this time with the inclusion of a dot product.
Again using the above definitions of F, C and its parametrization r(t), we
construct the integral from a Riemann_sum. We partition the interval [a,b]
(which is the range of the values of the parameter t) into n intervals of
length Ît = (b â a)/n. Letting ti be the ith point on [a,b], then r(ti)
gives us the position of the ith point on the curve. However, instead of
calculating up the distances between subsequent points, we need to calculate
their displacement vectors, Îri. As before, evaluating F at all the points on
the curve and taking the dot product with each displacement vector gives us the
infinitesimal contribution of each partition of F on C. Letting the size of the
partitions go to zero gives us a sum
         I =  lim  &#x0394; t &#x2192; 0    &#x2211;  i = 1   n    F  (  r
      (  t  i   ) ) &#x22C5; &#x0394;   r   i     {\displaystyle I=\lim _
      {\Delta t\rightarrow 0}\sum _{i=1}^{n}\mathbf {F} (\mathbf {r} (t_
      {i}))\cdot \Delta \mathbf {r} _{i}}  [I=\lim _{\Delta t\rightarrow 0}\sum
      _{i=1}^{n}\mathbf {F} (\mathbf {r} (t_{i}))\cdot \Delta \mathbf {r} _{i}]
By the mean_value_theorem, we see that the displacement vector between adjacent
points on the curve is
         &#x0394;   r   i   =  r  (  t  i   + &#x0394; t ) &#x2212;  r  (  t  i
      ) &#x2248;   r  &#x2032;  (  t  i   )  &#x0394; t   {\displaystyle \Delta
      \mathbf {r} _{i}=\mathbf {r} (t_{i}+\Delta t)-\mathbf {r} (t_{i})\approx
      \mathbf {r} '(t_{i})\,\Delta t}  [{\displaystyle \Delta \mathbf {r} _
      {i}=\mathbf {r} (t_{i}+\Delta t)-\mathbf {r} (t_{i})\approx \mathbf {r} '
      (t_{i})\,\Delta t}]
Substituting this in the above Riemann sum yields
         I =  lim  &#x0394; t &#x2192; 0    &#x2211;  i = 1   n    F  (  r
      (  t  i   ) ) &#x22C5;   r  &#x2032;  (  t  i   )  &#x0394; t
      {\displaystyle I=\lim _{\Delta t\rightarrow 0}\sum _{i=1}^{n}\mathbf {F}
      (\mathbf {r} (t_{i}))\cdot \mathbf {r} '(t_{i})\,\Delta t}  [
      {\displaystyle I=\lim _{\Delta t\rightarrow 0}\sum _{i=1}^{n}\mathbf {F}
      (\mathbf {r} (t_{i}))\cdot \mathbf {r} '(t_{i})\,\Delta t}]
which is the Riemann sum for the integral defined above.
**** Path independence[edit] ****
Main article: Gradient_theorem
If a vector field F is the gradient of a scalar_field G (i.e. if F is
conservative), that is,
         &#x2207; G =  F  ,   {\displaystyle \nabla G=\mathbf {F} ,}  [\nabla
      G=\mathbf {F} ,]
then the derivative of the composition of G and r(t) is
            d G (  r  ( t ) )   d t    = &#x2207; G (  r  ( t ) ) &#x22C5;   r
      &#x2032;  ( t ) =  F  (  r  ( t ) ) &#x22C5;   r  &#x2032;  ( t )
      {\displaystyle {\frac {dG(\mathbf {r} (t))}{dt}}=\nabla G(\mathbf {r}
      (t))\cdot \mathbf {r} '(t)=\mathbf {F} (\mathbf {r} (t))\cdot \mathbf {r}
      '(t)}  [{\frac {dG(\mathbf {r} (t))}{dt}}=\nabla G(\mathbf {r} (t))\cdot
      \mathbf {r} '(t)=\mathbf {F} (\mathbf {r} (t))\cdot \mathbf {r} '(t)]
which happens to be the integrand for the line integral of F on r(t). It
follows, given a path C, that
          &#x222B;  C    F  (  r  ) &#x22C5;  d  r  =  &#x222B;  a   b    F
      (  r  ( t ) ) &#x22C5;   r  &#x2032;  ( t )  d t =  &#x222B;  a   b
      d G (  r  ( t ) )   d t     d t = G (  r  ( b ) ) &#x2212; G (  r  ( a )
      ) .   {\displaystyle \int _{C}\mathbf {F} (\mathbf {r} )\cdot \,d\mathbf
      {r} =\int _{a}^{b}\mathbf {F} (\mathbf {r} (t))\cdot \mathbf {r} '
      (t)\,dt=\int _{a}^{b}{\frac {dG(\mathbf {r} (t))}{dt}}\,dt=G(\mathbf {r}
      (b))-G(\mathbf {r} (a)).}  [\int _{C}\mathbf {F} (\mathbf {r} )\cdot
      \,d\mathbf {r} =\int _{a}^{b}\mathbf {F} (\mathbf {r} (t))\cdot \mathbf
      {r} '(t)\,dt=\int _{a}^{b}{\frac {dG(\mathbf {r} (t))}{dt}}\,dt=G(\mathbf
      {r} (b))-G(\mathbf {r} (a)).]
In other words, the integral of F over C depends solely on the values of G at
the points r(b) and r(a) and is thus independent of the path between them. For
this reason, a line integral of a conservative vector field is called path
independent.
**** Applications[edit] ****
The line integral has many uses in physics. For example, the work done on a
particle traveling on a curve C inside a force field represented as a vector
field F is the line integral of F on C.
***** Flow across a curve[edit] *****
For a vector_field F : U â R2 â R2, such as     F ( x , y ) = ( P ( x , y )
, Q ( x , y ) )   {\displaystyle F(x,y)=(P(x,y),Q(x,y))}  [F(x,y)=(P(x,y),Q
(x,y))] the line integral across a piecewise_smooth curve C â U, is defined
as
          &#x222B;  C    F  (  r  ) &#x22C5;  d   r   t   =  &#x222B;  a   b
      &#x2212; Q ( x , y )  d x + P ( x , y )  d y =  &#x222B;  a   b   ( P
      (  r  ( t ) ) , Q (  r  ( t ) ) ) &#x22C5; (  r  2  &#x2032;  ( t ) ,
      &#x2212;  r  1  &#x2032;  ( t ) )  d t .   {\displaystyle \int _
      {C}\mathbf {F} (\mathbf {r} )\cdot \,d\mathbf {r} ^{t}=\int _{a}^{b}-Q
      (x,y)\,dx+P(x,y)\,dy=\int _{a}^{b}(P(\mathbf {r} (t)),Q(\mathbf {r}
      (t)))\cdot (r'_{2}(t),-r'_{1}(t))\,dt.}  [{\displaystyle \int _{C}\mathbf
      {F} (\mathbf {r} )\cdot \,d\mathbf {r} ^{t}=\int _{a}^{b}-Q(x,y)\,dx+P
      (x,y)\,dy=\int _{a}^{b}(P(\mathbf {r} (t)),Q(\mathbf {r} (t)))\cdot (r'_
      {2}(t),-r'_{1}(t))\,dt.}]
where Â· is the dot_product and r : [a, b] â C,     r ( t ) = (  r  1   ( t )
,  r  2   ( t ) )   {\displaystyle r(t)=(r_{1}(t),r_{2}(t))}  [r(t)=(r_{1}
(t),r_{2}(t))] is a bijective parametrization of the curve C such that r(a) and
r(b) give the endpoints of C.
***** Complex line integral[edit] *****
In complex_analysis, the line integral is defined in terms of multiplication
and addition of complex numbers. Suppose U is an open_subset of the complex
plane C, f : U â C is a function, and     L &#x2282; U   {\displaystyle
L\subset U}  [L\subset U] is a curve of finite length, parametrized by
&#x03B3; : [ a , b ] &#x2192; L   {\displaystyle \gamma :[a,b]\to L}  [\gamma :
[a,b]\to L], where     &#x03B3; ( t ) = x ( t ) + i y ( t ) .   {\displaystyle
\gamma (t)=x(t)+iy(t).}  [\gamma (t)=x(t)+iy(t).] The line integral
          &#x222B;  L   f ( z )  d z   {\displaystyle \int _{L}f(z)\,dz}  [\int
      _{L}f(z)\,dz]
may be defined by subdividing the interval [a, b] into a = t0 < t1 < ... < tn =
b and considering the expression
          &#x2211;  k = 1   n   f ( &#x03B3; (  t  k   ) ) [ &#x03B3; (  t  k
      ) &#x2212; &#x03B3; (  t  k &#x2212; 1   ) ] =  &#x2211;  k = 1   n   f
      (  &#x03B3;  k   )  &#x0394;  &#x03B3;  k   .   {\displaystyle \sum _
      {k=1}^{n}f(\gamma (t_{k}))[\gamma (t_{k})-\gamma (t_{k-1})]=\sum _{k=1}^
      {n}f(\gamma _{k})\,\Delta \gamma _{k}.}  [{\displaystyle \sum _{k=1}^{n}f
      (\gamma (t_{k}))[\gamma (t_{k})-\gamma (t_{k-1})]=\sum _{k=1}^{n}f(\gamma
      _{k})\,\Delta \gamma _{k}.}]
The integral is then the limit of this Riemann_sum as the lengths of the
subdivision intervals approach zero.
If the parametrization     &#x03B3;   {\displaystyle \gamma }  [\gamma ] is
continuously_differentiable, the line integral can be evaluated as an integral
of a function of a real variable:
          &#x222B;  L   f ( z )  d z =  &#x222B;  a   b   f ( &#x03B3; ( t ) )
      &#x03B3;   &#x2032;  ( t )  d t .   {\displaystyle \int _{L}f(z)\,dz=\int
      _{a}^{b}f(\gamma (t))\,\gamma \,'(t)\,dt.}  [\int _{L}f(z)\,dz=\int _{a}^
      {b}f(\gamma (t))\,\gamma \,'(t)\,dt.]
When     L   {\displaystyle L}  [L] is a closed curve, that is, its initial and
final points coincide, the notation
             &#x222E;       L   &#x2061; f ( z )  d z   {\displaystyle \oint _
      {L}f(z)\,dz}  [\oint _{L}f(z)\,dz]
is often used for the line integral of f along     L   {\displaystyle L}  [L].
A closed curve line integral is sometimes referred to as a cyclic integral in
engineering applications.
The line integral with respect to the conjugate complex differential        d z
&#x00AF;     {\displaystyle {\overline {dz}}}  [{\overline {dz}}] is defined[2]
to be
          &#x222B;  L   f     d z  &#x00AF;   :=     &#x222B;  L     f &#x00AF;
      d z  &#x00AF;   =  &#x222B;  a   b   f ( &#x03B3; ( t ) )      &#x03B3;
      &#x2032;  ( t )  &#x00AF;    d t .   {\displaystyle \int _{L}f\,
      {\overline {dz}}:={\overline {\int _{L}{\overline {f}}\,dz}}=\int _{a}^
      {b}f(\gamma (t))\,{\overline {\gamma '(t)}}\,dt.}  [{\displaystyle \int _
      {L}f\,{\overline {dz}}:={\overline {\int _{L}{\overline {f}}\,dz}}=\int _
      {a}^{b}f(\gamma (t))\,{\overline {\gamma '(t)}}\,dt.}]
The line integrals of complex functions can be evaluated using a number of
techniques: the integral may be split into real and imaginary parts reducing
the problem to that of evaluating two real-valued line integrals, the Cauchy
integral_formula may be used in other circumstances. If the line integral is a
closed curve in a region where the function is analytic and containing no
singularities, then the value of the integral is simply zero; this is a
consequence of the Cauchy_integral_theorem. The residue_theorem allows contour
integrals to be used in the complex plane to find integrals of real-valued
functions of a real variable (see residue_theorem for an example).
**** Example[edit] ****
Consider the function f(z)=1/z, and let the contour L be the unit_circle about
0, parametrized by z(t)=eit with t in [0, 2Ï] (which generates the circle
counterclockwise). Substituting, we find
                 &#x222E;       L   &#x2061; f ( z )  d z    =  &#x222B;  0   2
      &#x03C0;     1  e  i t     i  e  i t    d t = i  &#x222B;  0   2 &#x03C0;
      e  &#x2212; i t    e  i t    d t       = i  &#x222B;  0   2 &#x03C0;    d
      t = i ( 2 &#x03C0; &#x2212; 0 ) = 2 &#x03C0; i .       {\displaystyle
      {\begin{aligned}\oint _{L}f(z)\,dz&=\int _{0}^{2\pi }{1 \over e^{it}}ie^
      {it}\,dt=i\int _{0}^{2\pi }e^{-it}e^{it}\,dt\\&=i\int _{0}^{2\pi }\,dt=i
      (2\pi -0)=2\pi i.\end{aligned}}}  [{\begin{aligned}\oint _{L}f
      (z)\,dz&=\int _{0}^{2\pi }{1 \over e^{it}}ie^{it}\,dt=i\int _{0}^{2\pi
      }e^{-it}e^{it}\,dt\\&=i\int _{0}^{2\pi }\,dt=i(2\pi -0)=2\pi i.\end
      {aligned}}]
Here we have used the fact that any complex number z can be written as reit
where r is the modulus of z. On the unit circle this is fixed to 1, so the only
variable left is the angle, which is denoted by t. This answer can be also
verified by Cauchy's_integral_formula.
**** Relation between the line integral of a vector field and the complex line
integral[edit] ****
Viewing complex numbers as 2-dimensional vectors, the line integral of a 2-
dimensional vector field corresponds to the real part of the line integral of
the conjugate of the corresponding complex function of a complex variable. More
specifically, if      r  ( t ) = ( x ( t ) , y ( t ) )   {\displaystyle \mathbf
{r} (t)=(x(t),y(t))}  [\mathbf {r} (t)=(x(t),y(t))] is a parameterization of L
and     f ( z ) = u ( z ) + i v ( z )   {\displaystyle f(z)=u(z)+iv(z)}  [f
(z)=u(z)+iv(z)], then:
          &#x222B;  L      f ( z )  &#x00AF;    d z =  &#x222B;  L      f
      &#x00AF;     d x + i  &#x222B;  L      f &#x00AF;     d y =  &#x222B;  L
      ( u , v ) &#x22C5; d  r  + i  &#x222B;  L   ( &#x2212; v , u ) &#x22C5; d
      r  ,   {\displaystyle \int _{L}{\overline {f(z)}}\,dz=\int _{L}{\bar
      {f}}\,dx+i\int _{L}{\bar {f}}\,dy=\int _{L}(u,v)\cdot d\mathbf {r} +i\int
      _{L}(-v,u)\cdot d\mathbf {r} ,}  [\int _{L}{\overline {f(z)}}\,dz=\int _
      {L}{\bar {f}}\,dx+i\int _{L}{\bar {f}}\,dy=\int _{L}(u,v)\cdot d\mathbf
      {r} +i\int _{L}(-v,u)\cdot d\mathbf {r} ,]
provided that both integrals on the right hand side exist, and that the
parametrization     &#x03B3;   {\displaystyle \gamma }  [\gamma ] of L has the
same orientation as      r    {\displaystyle \mathbf {r} }  [\mathbf {r} ]
(just expand the Riemann sum for the lefthand integral and take the limit).
By Green's_theorem, the area of a region enclosed by a smooth, closed,
positively oriented curve     L   {\displaystyle L}  [L] is given by the
integral
           1  2 i     &#x222B;  L     z &#x00AF;    d z   {\displaystyle {\frac
      {1}{2i}}\int _{L}{\overline {z}}\;dz}  [{\frac {1}{2i}}\int _{L}
      {\overline {z}}\;dz]
This fact is used, for example, in the proof of the area_theorem.
Due to the CauchyâRiemann_equations the curl of the vector field
corresponding to the conjugate of a holomorphic_function is zero. This relates
through Stokes'_theorem both types of line integral being zero.
***** Geometric Line integral[edit] *****
A curve     &#x03B3;   {\displaystyle \gamma }  [\gamma ] embedded in some
vectorspace     V   {\displaystyle V}  [V] is a pure geometric object, hence it
does not need a specific coordinate representation to exist. Let     F
{\displaystyle F}  [F] be a one form (for example force) or a linear function
on     V   {\displaystyle V}  [V] that takes vectors     v   {\displaystyle v}
[v] from     V   {\displaystyle V}  [V] and maps them into the reals. Then one
can integrate F along a one dimensional object like that curve     &#x03B3;
{\displaystyle \gamma }  [\gamma ]
          &#x222B;  &#x03B3;   F   {\displaystyle \int _{\gamma }F}  [
      {\displaystyle \int _{\gamma }F}]
Intuitively one feeds this linear function with all the infinitesimal tangent
vectors that are attached at each point of     &#x03B3;   {\displaystyle \gamma
}  [\gamma ]. In coordinates      x  i     {\displaystyle x^{i}}  [
{\displaystyle x^{i}}] the one form has the representation (Note that one sums
over_repeated_indices)
          &#x222B;  &#x03B3;   F =  &#x222B;  &#x03B3;    f  i   ( x ) d  x  i
      {\displaystyle \int _{\gamma }F=\int _{\gamma }f_{i}(x)dx^{i}}  [
      {\displaystyle \int _{\gamma }F=\int _{\gamma }f_{i}(x)dx^{i}}]
If one parametrizes the curve by some parameter     t &#x2208; [ 0 , 1 ]
{\displaystyle t\in [0,1]}  [{\displaystyle t\in [0,1]}], by pullback one
arrives at the well known line integral form
          &#x222B;  0   1    f  i   ( x ( t ) )    &#x2202;  x  i     &#x2202;
      t    d t   {\displaystyle \int _{0}^{1}f_{i}(x(t)){\frac {\partial x^{i}}
      {\partial t}}dt}  [{\displaystyle \int _{0}^{1}f_{i}(x(t)){\frac
      {\partial x^{i}}{\partial t}}dt}]
Note that we made no use of any scalar product hence it is possible to define
line integrals without the use of a metric. Of course with a scalar product in
hand, the metric induces a map that identifies vectors with 1 forms and one
would arrive at the usual definition of line integrals from vector calculus.
          &#x222B;  0   1   &#x27E8;   F   ,    &#x2202;   x     &#x2202; t
      &#x27E9; d t   {\displaystyle \int _{0}^{1}\langle {\textbf {F}},{\frac
      {\partial {\textbf {x}}}{\partial t}}\rangle dt}  [{\displaystyle \int _
      {0}^{1}\langle {\textbf {F}},{\frac {\partial {\textbf {x}}}{\partial
      t}}\rangle dt}]
where       F     {\displaystyle {\textbf {F}}}  [{\displaystyle {\textbf
{F}}}] is the vector such that     F = &#x27E8;   F   , &#x22C5; &#x27E9;
{\displaystyle F=\langle {\textbf {F}},\cdot \rangle }  [{\displaystyle
F=\langle {\textbf {F}},\cdot \rangle }]
***** Quantum mechanics[edit] *****
The path_integral_formulation of quantum_mechanics actually refers not to path
integrals in this sense but to functional_integrals, that is, integrals over a
space of paths, of a function of a possible path. However, path integrals in
the sense of this article are important in quantum mechanics; for example,
complex contour integration is often used in evaluating probability_amplitudes
in quantum scattering theory.
***** See also[edit] *****
    * Divergence_theorem
    * Gradient_theorem
    * Methods_of_contour_integration
    * Nachbin's_theorem
    * Surface_integral
    * Volume_element
    * Volume_integral
***** References[edit] *****
   1. ^Kwong-Tin Tang (30 November 2006). Mathematical_Methods_for_Engineers
      and_Scientists_2:_Vector_Analysis,_Ordinary_Differential_Equations_and
      Laplace_Transforms. Springer Science & Business Media. ISBN 978-3-540-
      30268-1.
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
   3. ^Ahlfors, Lars (1966). Complex_Analysis (2nd ed.). New York: McGraw-Hill.
      p. 103.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Integral_over_trajectories",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Khan_Academy modules:
    * "Introduction_to_the_Line_Integral"
    * "Line_Integral_Example_1"
    * "Line_Integral_Example_2_(part_1)"
    * "Line_Integral_Example_2_(part_2)"
Path_integral at PlanetMath.org.
Line_integral_of_a_vector_field_â_Interactive

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Line_integral&oldid=900864888"
Categories:
    * Complex_analysis
    * Vector_calculus
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * Ð§ÓÐ²Ð°ÑÐ»Ð°
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 8 June 2019, at 02:48 (UTC).
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
