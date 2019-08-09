The following text has been accessed from https://en.wikipedia.org/wiki/Stokes%27_theorem at Fri Aug 9 02:35:31 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Stokes' theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the generalized theorem. For the classical theorem, see
KelvinâStokes_theorem. For the equation governing viscous drag in fluids, see
Stokes'_law.
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
In vector_calculus, and more generally differential_geometry, Stokes' theorem
(sometimes spelled Stokes's theorem, and also called the generalized Stokes
theorem or the StokesâCartan theorem[1]) is a statement about the integration
of differential_forms on manifolds, which both simplifies and generalizes
several theorems from vector_calculus. Stokes' theorem says that the integral
of a differential form Ï over the boundary of some orientable manifold Î© is
equal to the integral of its exterior_derivative dÏ over the whole of Î©,
i.e.,
          &#x222B;  &#x2202; &#x03A9;   &#x03C9; =  &#x222B;  &#x03A9;   d
      &#x03C9;  .   {\displaystyle \int _{\partial \Omega }\omega =\int _
      {\Omega }d\omega \,.}  [{\displaystyle \int _{\partial \Omega }\omega
      =\int _{\Omega }d\omega \,.}]
Stokes' theorem was formulated in its modern form by Ãlie_Cartan in 1945,[2]
following earlier work on the generalization of the theorems of vector calculus
by Vito_Volterra, Ãdouard_Goursat, and Henri_PoincarÃ©.[3][4]
This modern form of Stokes' theorem is a vast generalization of a classical
result that Lord_Kelvin communicated to George_Stokes in a letter dated July 2,
1850.[5][6][7] Stokes set the theorem as a question on the 1854 Smith's_Prize
exam, which led to the result bearing his name. It was first published by
Hermann_Hankel in 1861.[7][8] This classical KelvinâStokes_theorem relates
the surface_integral of the curl of a vector_field F over a surface in
Euclidean three-space to the line_integral of the vector field over its
boundary: Let Î³: [a, b] â R2 be a piecewise smooth Jordan_plane_curve. The
Jordan_curve_theorem implies that Î³ divides R2 into two components, a compact
one and another that is non-compact. Let D denote the compact part that is
bounded by Î³ and suppose Ï: D â R3 is smooth, with S := Ï(D). If Î is the
space_curve defined by Î(t) = Ï(Î³(t))[note_1] and F is a smooth vector field
on R3, then:[9][10][11]
             &#x222E;       &#x0393;   &#x2061;  F   &#x22C5;  d   &#x0393;   =
      &#x222C;  S   &#x2207; &#x00D7;  F   &#x22C5;  d  S    {\displaystyle
      \oint _{\Gamma }\mathbf {F} \,\cdot \,d{\mathbf {\Gamma } }=\iint _
      {S}\nabla \times \mathbf {F} \,\cdot \,d\mathbf {S} }  [\oint _{\Gamma
      }\mathbf {F} \,\cdot \,d{\mathbf {\Gamma } }=\iint _{S}\nabla \times
      \mathbf {F} \,\cdot \,d\mathbf {S} ]
This classical statement, along with the classical divergence_theorem, the
fundamental_theorem_of_calculus, and Green's_theorem are simply special cases
of the general formulation stated above.
⁰
***** Contents *****
    * 1_Introduction
    * 2_Formulation_for_smooth_manifolds_with_boundary
    * 3_Topological_preliminaries;_integration_over_chains
    * 4_Underlying_principle
    * 5_Generalization_to_rough_sets
    * 6_Special_cases
          o 6.1_KelvinâStokes_theorem
          o 6.2_Green's_theorem
                # 6.2.1_In_electromagnetism
          o 6.3_Divergence_theorem
    * 7_See_also
    * 8_Footnotes
    * 9_References
    * 10_Further_reading
    * 11_External_links
***** Introduction[edit] *****
The fundamental_theorem_of_calculus states that the integral of a function f
over the interval [a, b] can be calculated by finding an antiderivative F of f:
          &#x222B;  a   b   f ( x )  d x = F ( b ) &#x2212; F ( a )  .
      {\displaystyle \int _{a}^{b}f(x)\,dx=F(b)-F(a)\,.}  [{\displaystyle \int
      _{a}^{b}f(x)\,dx=F(b)-F(a)\,.}]
Stokes' theorem is a vast generalization of this theorem in the following
sense.
    * By the choice of F, dF/dx = f(x). In the parlance of differential_forms,
      this is saying that f(x) dx is the exterior_derivative of the 0-form,
      i.e. function, F: in other words, that dF = f dx. The general Stokes
      theorem applies to higher differential forms Ï instead of just 0-forms
      such as F.
    * A closed interval [a, b] is a simple example of a one-dimensional
      manifold_with_boundary. Its boundary is the set consisting of the two
      points a and b. Integrating f over the interval may be generalized to
      integrating forms on a higher-dimensional manifold. Two technical
      conditions are needed: the manifold has to be orientable, and the form
      has to be compactly_supported in order to give a well-defined integral.
    * The two points a and b form the boundary of the closed interval. More
      generally, Stokes' theorem applies to oriented manifolds M with boundary.
      The boundary âM of M is itself a manifold and inherits a natural
      orientation from that of M. For example, the natural orientation of the
      interval gives an orientation of the two boundary points. Intuitively, a
      inherits the opposite orientation as b, as they are at opposite ends of
      the interval. So, "integrating" F over two boundary points a, b is taking
      the difference F(b) â F(a).
In even simpler terms, one can consider the points as boundaries of curves,
that is as 0-dimensional boundaries of 1-dimensional manifolds. So, just as one
can find the value of an integral (f dx = dF) over a 1-dimensional manifold (
[a, b]) by considering the anti-derivative (F) at the 0-dimensional boundaries
({a, b}), one can generalize the fundamental theorem of calculus, with a few
additional caveats, to deal with the value of integrals (dÏ) over n-
dimensional manifolds (Î©) by considering the antiderivative (Ï) at the (n â
1)-dimensional boundaries (âÎ©) of the manifold.
So the fundamental theorem reads:
          &#x222B;  [ a , b ]   f ( x )  d x =  &#x222B;  [ a , b ]   d F =
      &#x222B;  { a  }  &#x2212;   &#x222A; { b  }  +     F = F ( b ) &#x2212;
      F ( a )  .   {\displaystyle \int _{[a,b]}f(x)\,dx=\int _{[a,b]}dF=\int _
      {\{a\}^{-}\cup \{b\}^{+}}F=F(b)-F(a)\,.}  [{\displaystyle \int _{[a,b]}f
      (x)\,dx=\int _{[a,b]}dF=\int _{\{a\}^{-}\cup \{b\}^{+}}F=F(b)-F(a)\,.}]
***** Formulation for smooth manifolds with boundary[edit] *****
Let Î© be an oriented smooth_manifold with boundary of dimension n and let Î±
be a smooth n-differential_form that is compactly_supported on Î©. First,
suppose that Î± is compactly supported in the domain of a single, oriented
coordinate_chart {U, Ï}. In this case, we define the integral of Î± over Î© as
          &#x222B;  &#x03A9;   &#x03B1; =  &#x222B;  &#x03C6; ( U )
      (  &#x03C6;  &#x2212; 1   )   &#x2217;   &#x03B1;  ,   {\displaystyle
      \int _{\Omega }\alpha =\int _{\varphi (U)}\left(\varphi ^{-1}\right)^
      {*}\alpha \,,}  [{\displaystyle \int _{\Omega }\alpha =\int _{\varphi
      (U)}\left(\varphi ^{-1}\right)^{*}\alpha \,,}]
i.e., via the pullback of Î± to Rn.
More generally, the integral of Î± over Î© is defined as follows: Let {Ïi} be
a partition_of_unity associated with a locally_finite cover {Ui, Ïi} of
(consistently oriented) coordinate charts, then define the integral
          &#x222B;  &#x03A9;   &#x03B1; &#x2261;  &#x2211;  i    &#x222B;   U
      i      &#x03C8;  i   &#x03B1;  ,   {\displaystyle \int _{\Omega }\alpha
      \equiv \sum _{i}\int _{U_{i}}\psi _{i}\alpha \,,}  [{\displaystyle \int _
      {\Omega }\alpha \equiv \sum _{i}\int _{U_{i}}\psi _{i}\alpha \,,}]
where each term in the sum is evaluated by pulling back to Rn as described
above. This quantity is well-defined; that is, it does not depend on the choice
of the coordinate charts, nor the partition of unity.
The generalized Stokes theorem reads:
Theorem. (StokesâCartan) If     &#x03C9;   {\displaystyle \omega }  [\omega ]
is a smooth     ( n &#x2212; 1 )   {\displaystyle (n-1)}  [(n-1)]-form with
compact_support on smooth     n   {\displaystyle n}  [n]-dimensional manifold-
with-boundary     &#x03A9;   {\displaystyle \Omega }  [\Omega ],     &#x2202;
&#x03A9;   {\displaystyle \partial \Omega }  [\partial\Omega] denotes the
boundary of     &#x03A9;   {\displaystyle \Omega }  [\Omega ] given the induced
orientation, and     i : &#x2202; &#x03A9; &#x21AA; &#x03A9;   {\displaystyle
i:\partial \Omega \hookrightarrow \Omega }  [{\displaystyle i:\partial \Omega
\hookrightarrow \Omega }] is the inclusion_map, then
          &#x222B;  &#x03A9;   d &#x03C9; =  &#x222B;  &#x2202; &#x03A9;    i
      &#x2217;   &#x03C9;   {\displaystyle \int _{\Omega }d\omega =\int _
      {\partial \Omega }i^{*}\omega }  [{\displaystyle \int _{\Omega }d\omega
      =\int _{\partial \Omega }i^{*}\omega }].
Conventionally,      &#x222B;  &#x2202; &#x03A9;    i  &#x2217;   &#x03C9;
{\textstyle \int _{\partial \Omega }i^{*}\omega }  [{\textstyle \int _{\partial
\Omega }i^{*}\omega }] is abbreviated as      &#x222B;  &#x2202; &#x03A9;
&#x03C9;   {\textstyle \int _{\partial \Omega }\omega }  [{\textstyle \int _
{\partial \Omega }\omega }], since the pullback of a differential form by the
inclusion map is simply its restriction to its domain:      i  &#x2217;
&#x03C9; = &#x03C9;   |   &#x2202; &#x03A9;     {\displaystyle i^{*}\omega
=\omega |_{\partial \Omega }}  [{\displaystyle i^{*}\omega =\omega |_{\partial
\Omega }}]. Here     d   {\displaystyle d}  [d] is the exterior_derivative,
which is defined using the manifold structure only. The right-hand side is
sometimes written as        &#x222E;     &#x2202; &#x03A9;   &#x2061; &#x03C9;
{\textstyle \oint _{\partial \Omega }\omega }  [{\textstyle \oint _{\partial
\Omega }\omega }] to stress the fact that the     ( n &#x2212; 1 )
{\displaystyle (n-1)}  [(n-1)]-manifold     &#x2202; &#x03A9;   {\displaystyle
\partial \Omega }  [\partial\Omega] has no boundary.[note_2] (This fact is also
an implication of Stokes' theorem, since for a given smooth     n
{\displaystyle n}  [n]-dimensional manifold     &#x03A9;   {\displaystyle
\Omega }  [\Omega ], application of the theorem twice gives      &#x222B;
&#x2202; ( &#x2202; &#x03A9; )   &#x03C9; =  &#x222B;  &#x03A9;   d ( d
&#x03C9; ) = 0   {\textstyle \int _{\partial (\partial \Omega )}\omega =\int _
{\Omega }d(d\omega )=0}  [{\textstyle \int _{\partial (\partial \Omega )}\omega
=\int _{\Omega }d(d\omega )=0}] for any     ( n &#x2212; 2 )   {\displaystyle
(n-2)}  [{\displaystyle (n-2)}]-form     &#x03C9;   {\displaystyle \omega }
[\omega ], which implies that     &#x2202; ( &#x2202; &#x03A9; ) = &#x2205;
{\displaystyle \partial (\partial \Omega )=\emptyset }  [{\displaystyle
\partial (\partial \Omega )=\emptyset }].) The right-hand side of the equation
is often used to formulate integral laws; the left-hand side then leads to
equivalent differential formulations (see below).
The theorem is often used in situations where     &#x03A9;   {\displaystyle
\Omega }  [\Omega ] is an embedded oriented submanifold of some bigger
manifold, often       R   k     {\displaystyle \mathbf {R} ^{k}}  [
{\displaystyle \mathbf {R} ^{k}}], on which the form     &#x03C9;
{\displaystyle \omega }  [\omega ] is defined.
***** Topological preliminaries; integration over chains[edit] *****
Let M be a smooth_manifold. A (smooth) singular k-simplex in M is defined as a
smooth_map from the standard simplex in Rk to M. The group Ck(M, Z) of singular
k-chains on M is defined to be the free_abelian_group on the set of singular k-
simplices in M. These groups, together with the boundary map, â, define a
chain_complex. The corresponding homology (resp. cohomology) group is
isomorphic to the usual singular_homology group Hk(M, Z) (resp. the singular
cohomology group Hk(M, Z)), defined using continuous rather than smooth
simplices in M.
On the other hand, the differential forms, with exterior derivative, d, as the
connecting map, form a cochain complex, which defines the de_Rham_cohomology
groups Hk
dR(M, R).
Differential k-forms can be integrated over a k-simplex in a natural way, by
pulling back to Rk. Extending by linearity allows one to integrate over chains.
This gives a linear map from the space of k-forms to the kth group of singular
cochains, Ck(M, Z), the linear functionals on Ck(M, Z). In other words, a k-
form Ï defines a functional
         I ( &#x03C9; ) ( c ) =     &#x222E;       c   &#x2061; &#x03C9;
      {\displaystyle I(\omega )(c)=\oint _{c}\omega }  [I(\omega )(c)=\oint _
      {c}\omega ]
on the k-chains. Stokes' theorem says that this is a chain map from de Rham
cohomology to singular cohomology with real coefficients; the exterior
derivative, d, behaves like the dual of â on forms. This gives a homomorphism
from de Rham cohomology to singular cohomology. On the level of forms, this
means:
   1. closed forms, i.e., dÏ = 0, have zero integral over boundaries, i.e.
      over manifolds that can be written as ââc Mc, and
   2. exact forms, i.e., Ï = dÏ, have zero integral over cycles, i.e. if the
      boundaries sum up to the empty set: âc Mc = â.
De_Rham's_theorem shows that this homomorphism is in fact an isomorphism. So
the converse to 1 and 2 above hold true. In other words, if {ci} are cycles
generating the kth homology group, then for any corresponding real numbers,
{ai}, there exist a closed form, Ï, such that
             &#x222E;        c  i     &#x2061; &#x03C9; =  a  i    ,
      {\displaystyle \oint _{c_{i}}\omega =a_{i}\,,}  [{\displaystyle \oint _
      {c_{i}}\omega =a_{i}\,,}]
and this form is unique up to exact forms.
Stokes' theorem on smooth manifolds can be derived from Stokes' theorem for
chains in smooth manifolds, and vice versa.[12] Formally stated, the latter
reads:[13]
Theorem. (Stokes' theorem for chains) If     c   {\displaystyle c}  [c] is a
smooth     k   {\displaystyle k}  [k]-chain in a smooth manifold     M
{\displaystyle M}  [M], and     &#x03C9;   {\displaystyle \omega }  [\omega ]
is a smooth     ( k &#x2212; 1 )   {\displaystyle (k-1)}  [(k-1)]-form on     M
{\displaystyle M}  [M], then
          &#x222B;  &#x2202; c   &#x03C9; =  &#x222B;  c   d &#x03C9;
      {\displaystyle \int _{\partial c}\omega =\int _{c}d\omega }  [
      {\displaystyle \int _{\partial c}\omega =\int _{c}d\omega }].
***** Underlying principle[edit] *****
[Stokes_patch.svg]
To simplify these topological arguments, it is worthwhile to examine the
underlying principle by considering an example for d = 2 dimensions. The
essential idea can be understood by the diagram on the left, which shows that,
in an oriented tiling of a manifold, the interior paths are traversed in
opposite directions; their contributions to the path integral thus cancel each
other pairwise. As a consequence, only the contribution from the boundary
remains. It thus suffices to prove Stokes' theorem for sufficiently fine
tilings (or, equivalently, simplices), which usually is not difficult.
***** Generalization to rough sets[edit] *****
A region (here called D instead of Î©) with piecewise smooth boundary. This is
a manifold_with_corners, so its boundary is not a smooth manifold.
The formulation above, in which Î© is a smooth manifold with boundary, does not
suffice in many applications. For example, if the domain of integration is
defined as the plane region between two x-coordinates and the graphs of two
functions, it will often happen that the domain has corners. In such a case,
the corner points mean that Î© is not a smooth manifold with boundary, and so
the statement of Stokes' theorem given above does not apply. Nevertheless, it
is possible to check that the conclusion of Stokes' theorem is still true. This
is because Î© and its boundary are well-behaved away from a small set of points
(a measure_zero set).
A version of Stokes' theorem that extends to rough domains was proved by
Whitney.[14] Assume that D is a connected bounded open subset of Rn. Call D a
standard domain if it satisfies the following property: There exists a subset P
of âD, open in âD, whose complement in âD has Hausdorff_(n_â_1)-measure
zero; and such that every point of P has a generalized normal vector. This is a
vector v(x) such that, if a coordinate system is chosen so that v(x) is the
first basis vector, then, in an open neighborhood around x, there exists a
smooth function f(x2, â¦, xn) such that P is the graph { x1 = f(x2, â¦, xn) }
and D is the region { x1 < f(x2, â¦, xn) }. Whitney remarks that the boundary
of a standard domain is the union of a set of zero Hausdorff (n â 1)-measure
and a finite or countable union of smooth (n â 1)-manifolds, each of which
has the domain on only one side. He then proves that if D is a standard domain
in Rn, Ï is an (n â 1)-form which is defined, continuous, and bounded on D
âª P, smooth on D, integrable on P, and such that dÏ is integrable on D, then
Stokes' theorem holds, that is,
          &#x222B;  P   &#x03C9; =  &#x222B;  D   d &#x03C9;  .
      {\displaystyle \int _{P}\omega =\int _{D}d\omega \,.}  [{\displaystyle
      \int _{P}\omega =\int _{D}d\omega \,.}]
The study of measure-theoretic properties of rough sets leads to geometric
measure_theory. Even more general versions of Stokes' theorem have been proved
by Federer and by Harrison.[15]
***** Special cases[edit] *****
The general form of the Stokes theorem using differential forms is more
powerful and easier to use than the special cases. The traditional versions can
be formulated using Cartesian_coordinates without the machinery of differential
geometry, and thus are more accessible. Further, they are older and their names
are more familiar as a result. The traditional forms are often considered more
convenient by practicing scientists and engineers but the non-naturalness of
the traditional formulation becomes apparent when using other coordinate
systems, even familiar ones like spherical or cylindrical coordinates. There is
potential for confusion in the way names are applied, and the use of dual
formulations.
**** KelvinâStokes theorem[edit] ****
An illustration of the KelvinâStokes theorem, with surface Î£, its boundary
âÎ£ and the "normal" vector n.
This is a (dualized) (1 + 1)-dimensional case, for a 1-form (dualized because
it is a statement about vector_fields). This special case is often just
referred to as Stokes' theorem in many introductory university vector calculus
courses and is used in physics and engineering. It is also sometimes known as
the curl theorem.
The classical KelvinâStokes_theorem relates the surface_integral of the curl
of a vector_field over a surface Î£ in Euclidean three-space to the line
integral of the vector field over its boundary. It is a special case of the
general Stokes theorem (with n = 2) once we identify a vector field with a 1-
form using the metric on Euclidean 3-space. The curve of the line integral,
âÎ£, must have positive orientation, meaning that âÎ£ points
counterclockwise when the surface_normal, n, points toward the viewer.
One consequence of the KelvinâStokes theorem is that the field_lines of a
vector field with zero curl cannot be closed contours. The formula can be
rewritten as:
Suppose F=(P(x,y,z),Q(x,y,z),R(x,y,z)) is defined in region with smooth surface
Î£ and has first-order continuous partial_derivatives. Then
                &#x222C;  &#x03A3;     (    (     &#x2202; R   &#x2202; y
      &#x2212;    &#x2202; Q   &#x2202; z     )   d y  d z +  (     &#x2202; P
      &#x2202; z    &#x2212;    &#x2202; R   &#x2202; x     )   d z  d x +
      (     &#x2202; Q   &#x2202; x    &#x2212;    &#x2202; P   &#x2202; y
      )   d x  d y   )       =         &#x222E;       &#x2202; &#x03A3;
      &#x2061;   (   P  d x + Q  d y + R  d z   )    ,       {\displaystyle
      {\begin{aligned}&\iint _{\Sigma }{\Bigg (}\left({\frac {\partial R}
      {\partial y}}-{\frac {\partial Q}{\partial z}}\right)\,dy\,dz+\left(
      {\frac {\partial P}{\partial z}}-{\frac {\partial R}{\partial
      x}}\right)\,dz\,dx+\left({\frac {\partial Q}{\partial x}}-{\frac
      {\partial P}{\partial y}}\right)\,dx\,dy{\Bigg )}\\[4pt]={}&\oint _
      {\partial \Sigma }{\Big (}P\,dx+Q\,dy+R\,dz{\Big )}\,,\end{aligned}}}  [
      {\displaystyle {\begin{aligned}&\iint _{\Sigma }{\Bigg (}\left({\frac
      {\partial R}{\partial y}}-{\frac {\partial Q}{\partial
      z}}\right)\,dy\,dz+\left({\frac {\partial P}{\partial z}}-{\frac
      {\partial R}{\partial x}}\right)\,dz\,dx+\left({\frac {\partial Q}
      {\partial x}}-{\frac {\partial P}{\partial y}}\right)\,dx\,dy{\Bigg )}\\
      [4pt]={}&\oint _{\partial \Sigma }{\Big (}P\,dx+Q\,dy+R\,dz{\Big
      )}\,,\end{aligned}}}]

where P, Q and R are the components of F, and âÎ£ is boundary of region with
smooth surface Î£.
**** Green's theorem[edit] ****
Green's_theorem is immediately recognizable as the third integrand of both
sides in the integral in terms of P, Q, and R cited above.
*** In electromagnetism[edit] ***
Two of the four Maxwell_equations involve curls of 3-D vector fields, and their
differential and integral forms are related by the KelvinâStokes_theorem.
Caution must be taken to avoid cases with moving boundaries: the partial time
derivatives are intended to exclude such cases. If moving boundaries are
included, interchange of integration and differentiation introduces terms
related to boundary motion not included in the results below (see
Differentiation_under_the_integral_sign):
 _____________________________________________________________________________________________________________
|Name                         |Differential  |Integral form (using KelvinâStokes theorem plus relativisti|
|_____________________________|form__________|invariance,_â«_â/ât_â¦_â_d/dt_â«_â|�)
|                             |    &#x2207;  |                                                                |
|                             |&#x00D7;  E  =|                                                                |
|                             |&#x2212;      |                                                                |
|                             |&#x2202;  B   |                                                                |
|                             |&#x2202; t    |            &#x222E;       C   &#x2061;  E  &#x22C5; d  l     = |
|                             |{\displaystyle|&#x222C;  S   &#x2207; &#x00D7;  E  &#x22C5; d  A        =      |
|                             |\quad \nabla  |&#x2212;  &#x222C;  S      &#x2202;  B    &#x2202; t    &#x22C5;|
|                             |\times \mathbf|d  A         {\displaystyle {\begin{aligned}\quad \oint _       |
|                             |{E} =-{\frac  |{C}\mathbf {E} \cdot d\mathbf {l} &=\iint _{S}\nabla \times     |
|MaxwellâFaraday equation|{\partial     |\mathbf {E} \cdot d\mathbf {A} \\&=-\iint _{S}{\frac {\partial  |
|Faraday's_law_of_induction:  |\mathbf {B} } |\mathbf {B} }{\partial t}}\cdot d\mathbf {A} \end{aligned}}\quad|
|                             |{\partial     |}  [{\displaystyle {\begin{aligned}\quad \oint _{C}\mathbf {E}  |
|                             |t}}\quad }  [ |\cdot d\mathbf {l} &=\iint _{S}\nabla \times \mathbf {E} \cdot  |
|                             |{\displaystyle|d\mathbf {A} \\&=-\iint _{S}{\frac {\partial \mathbf {B} }      |
|                             |\quad \nabla  |{\partial t}}\cdot d\mathbf {A} \end{aligned}}\quad }] (with C  |
|                             |\times \mathbf|and S not necessarily stationary)                               |
|                             |{E} =-{\frac  |                                                                |
|                             |{\partial     |                                                                |
|                             |\mathbf {B} } |                                                                |
|                             |{\partial     |                                                                |
|_____________________________|t}}\quad_}]___|________________________________________________________________|
|                             |    &#x2207;  |                                                                |
|                             |&#x00D7;  H  =|                                                                |
|                             |J  +          |                                                                |
|                             |&#x2202;  D   |                                                                |
|                             |&#x2202; t    |            &#x222E;       C   &#x2061;  H  &#x22C5; d  l     = |
|                             |{\displaystyle|&#x222C;  S   &#x2207; &#x00D7;  H  &#x22C5; d  A        =      |
|                             |\quad \nabla  |&#x222C;  S    J  &#x22C5; d  A  +  &#x222C;  S      &#x2202;  D|
|                             |\times \mathbf|&#x2202; t    &#x22C5; d  A         {\displaystyle {\begin      |
|                             |{H} =\mathbf  |{aligned}\quad \oint _{C}\mathbf {H} \cdot d\mathbf {l} &=\iint |
|                             |{J} +{\frac   |_{S}\nabla \times \mathbf {H} \cdot d\mathbf {A} \\&=\iint _    |
|AmpÃ¨re's_law              |{\partial     |{S}\mathbf {J} \cdot d\mathbf {A} +\iint _{S}{\frac {\partial   |
|(with Maxwell's extension):  |\mathbf {D} } |\mathbf {D} }{\partial t}}\cdot d\mathbf {A} \end{aligned}}\quad|
|                             |{\partial     |}  [{\displaystyle {\begin{aligned}\quad \oint _{C}\mathbf {H}  |
|                             |t}}\quad }  [ |\cdot d\mathbf {l} &=\iint _{S}\nabla \times \mathbf {H} \cdot  |
|                             |{\displaystyle|d\mathbf {A} \\&=\iint _{S}\mathbf {J} \cdot d\mathbf {A} +\iint|
|                             |\quad \nabla  |_{S}{\frac {\partial \mathbf {D} }{\partial t}}\cdot d\mathbf   |
|                             |\times \mathbf|{A} \end{aligned}}\quad }] (with C and S not necessarily        |
|                             |{H} =\mathbf  |stationary)                                                     |
|                             |{J} +{\frac   |                                                                |
|                             |{\partial     |                                                                |
|                             |\mathbf {D} } |                                                                |
|                             |{\partial     |                                                                |
|_____________________________|t}}\quad_}]___|________________________________________________________________|
The above listed subset of Maxwell's equations are valid for electromagnetic
fields expressed in SI_units. In other systems of units, such as CGS or
Gaussian_units, the scaling factors for the terms differ. For example, in
Gaussian units, Faraday's law of induction and AmpÃ¨re's law take the forms:
[16][17]
             &#x2207; &#x00D7;  E     = &#x2212;   1 c      &#x2202;  B
      &#x2202; t     ,     &#x2207; &#x00D7;  H     =   1 c      &#x2202;  D
      &#x2202; t    +    4 &#x03C0;  c    J   ,       {\displaystyle {\begin
      {aligned}\nabla \times \mathbf {E} &=-{\frac {1}{c}}{\frac {\partial
      \mathbf {B} }{\partial t}}\,,\\\nabla \times \mathbf {H} &={\frac {1}{c}}
      {\frac {\partial \mathbf {D} }{\partial t}}+{\frac {4\pi }{c}}\mathbf {J}
      \,,\end{aligned}}}  [{\displaystyle {\begin{aligned}\nabla \times \mathbf
      {E} &=-{\frac {1}{c}}{\frac {\partial \mathbf {B} }{\partial
      t}}\,,\\\nabla \times \mathbf {H} &={\frac {1}{c}}{\frac {\partial
      \mathbf {D} }{\partial t}}+{\frac {4\pi }{c}}\mathbf {J} \,,\end
      {aligned}}}]
respectively, where c is the speed_of_light in vacuum.
**** Divergence theorem[edit] ****
Likewise, the OstrogradskyâGauss_theorem (also known as the divergence
theorem or Gauss's theorem)
          &#x222B;   V o l    &#x2207; &#x22C5;  F    d   V o l    =
      &#x222E;       &#x2202;  V o l    &#x2061;  F  &#x22C5; d  &#x03A3;
      {\displaystyle \int _{\mathrm {Vol} }\nabla \cdot \mathbf {F} \,d_
      {\mathrm {Vol} }=\oint _{\partial \mathrm {Vol} }\mathbf {F} \cdot d
      {\boldsymbol {\Sigma }}}  [{\displaystyle \int _{\mathrm {Vol} }\nabla
      \cdot \mathbf {F} \,d_{\mathrm {Vol} }=\oint _{\partial \mathrm {Vol}
      }\mathbf {F} \cdot d{\boldsymbol {\Sigma }}}]
is a special case if we identify a vector field with the (n â 1)-form
obtained by contracting the vector field with the Euclidean volume form. An
application of this is the case F = fc where c is an arbitrary constant vector.
Working out the divergence of the product gives
          c  &#x22C5;  &#x222B;   V o l    &#x2207; f   d   V o l    =  c
      &#x22C5;     &#x222E;       &#x2202;  V o l    &#x2061; f  d  &#x03A3;
      .   {\displaystyle \mathbf {c} \cdot \int _{\mathrm {Vol} }\nabla f\,d_
      {\mathrm {Vol} }=\mathbf {c} \cdot \oint _{\partial \mathrm {Vol} }f\,d
      {\boldsymbol {\Sigma }}\,.}  [{\displaystyle \mathbf {c} \cdot \int _
      {\mathrm {Vol} }\nabla f\,d_{\mathrm {Vol} }=\mathbf {c} \cdot \oint _
      {\partial \mathrm {Vol} }f\,d{\boldsymbol {\Sigma }}\,.}]
Since this holds for all c we find
          &#x222B;   V o l    &#x2207; f   d   V o l    =     &#x222E;
      &#x2202;  V o l    &#x2061; f  d  &#x03A3;   .   {\displaystyle \int _
      {\mathrm {Vol} }\nabla f\,d_{\mathrm {Vol} }=\oint _{\partial \mathrm
      {Vol} }f\,d{\boldsymbol {\Sigma }}\,.}  [{\displaystyle \int _{\mathrm
      {Vol} }\nabla f\,d_{\mathrm {Vol} }=\oint _{\partial \mathrm {Vol} }f\,d
      {\boldsymbol {\Sigma }}\,.}]
***** See also[edit] *****
    * ChandrasekharâWentzel_lemma
***** Footnotes[edit] *****
   1. ^ Î³ and Î are both loops, however, Î is not necessarily a Jordan_curve
   2. ^ For mathematicians this fact is known, therefore the circle is
      redundant and often omitted. However, one should keep in mind here that
      in thermodynamics, where frequently expressions as â®W {dtotalU} appear
      (wherein the total derivative, see below, should not be confused with the
      exterior one), the integration path W is a one-dimensional closed line on
      a much higher-dimensional manifold. That is, in a thermodynamic
      application, where U is a function of the temperature Î±1 := T, the
      volume Î±2 := V, and the electrical polarization Î±3 := P of the sample,
      one has
               {  d  total   U } =  &#x2211;  i = 1   3      &#x2202; U
            &#x2202;  &#x03B1;  i       d  &#x03B1;  i    ,   {\displaystyle \
            {d_{\text{total}}U\}=\sum _{i=1}^{3}{\frac {\partial U}{\partial
            \alpha _{i}}}\,d\alpha _{i}\,,}  [{\displaystyle \{d_{\text
            {total}}U\}=\sum _{i=1}^{3}{\frac {\partial U}{\partial \alpha _
            {i}}}\,d\alpha _{i}\,,}]
      and the circle is really necessary, e.g. if one considers the
      differential consequences of the integral postulate
                   &#x222E;       W    {  d  total   U }      =   !      0  .
            {\displaystyle \oint _{W}\,\{d_{\text{total}}U\}\,{\stackrel {!}
            {=}}\,0\,.}  [{\displaystyle \oint _{W}\,\{d_{\text{total}}U\}\,
            {\stackrel {!}{=}}\,0\,.}]
***** References[edit] *****
   1. ^Physics_of_Collisional_Plasmas_â_Introduction_to_|_Michel_Moisan_|
      Springer.
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
   3. ^Cartan, Ãlie (1945). Les SystÃ¨mes DiffÃ©rentiels ExtÃ©rieurs et leurs
      Applications GÃ©omÃ©triques. Paris: Hermann.
   4. ^Katz, Victor J. (1979-01-01). "The History of Stokes' Theorem".
      Mathematics Magazine. 52 (3): 146â156. doi:10.2307/2690275.
      JSTOR 2690275.
   5. ^Katz, Victor J. (1999). "5. Differential Forms". In James, I. M. (ed.).
      History of Topology. Amsterdam: Elsevier. pp. 111â122.
      ISBN 9780444823755.
   6. ^ See:
          o Katz, Victor J. (May 1979). "The history of Stokes' theorem".
            Mathematics Magazine. 52 (3): 146â156.
   7. The letter from Thomson to Stokes appears in:Thomson,_William; Stokes,
      George_Gabriel (1990). Wilson, David B. (ed.). The_Correspondence_between
      Sir_George_Gabriel_Stokes_and_Sir_William_Thomson,_Baron_Kelvin_of_Largs,
      Volume_1:_1846â1869. Cambridge, England: Cambridge University Press.
      pp. 96â97.
   8. Neither Thomson nor Stokes published a proof of the theorem. The first
      published proof appeared in 1861 in:Hankel,_Hermann (1861). Zur
      allgemeinen_Theorie_der_Bewegung_der_FlÃ¼ssigkeiten [On the general
      theory of the movement of fluids]. GÃ¶ttingen, Germany: Dieterische
      University Buchdruckerei. pp. 34â37.
   9.  Hankel doesn't mention the author of the theorem.
  10. In a footnote, Larmor mentions earlier researchers who had integrated,
      over a surface, the curl of a vector field. See:Stokes,_George_Gabriel
      (1905). Larmor, Joseph; Strutt, John William, Baron Rayleigh (eds.).
      Mathematical_and_Physical_Papers_by_the_late_Sir_George_Gabriel_Stokes.
      5. Cambridge, England: University of Cambridge Press. pp. 320â321.
  11. ^Darrigol, Olivier (2000). Electrodynamics from AmpÃ¨re to Einstein.
      Oxford, England. p. 146. ISBN 0198505930.
  12. ^ a b Spivak (1965), p. vii, Preface.
  13. ^ See:
          o The 1854 Smith's Prize Examination is available online at: Clerk
            Maxwell_Foundation. Maxwell took this examination and tied for
            first place with Edward_John_Routh. See:Clerk_Maxwell,_James
            (1990). Harman, P. M. (ed.). The_Scientific_Letters_and_Papers_of
            James_Clerk_Maxwell,_Volume_I:_1846â1862. Cambridge, England:
            Cambridge University Press. p. 237, footnote 2.
  14.  See also Smith's_prize or the Clerk_Maxwell_Foundation.
  15. Clerk_Maxwell,_James (1873). A_Treatise_on_Electricity_and_Magnetism. 1.
      Oxford, England: Clarendon Press. pp. 25â27.
  16.  In a footnote on page 27, Maxwell mentions that Stokes used the theorem
      as question 8 in the Smith's Prize Examination of 1854. This footnote
      appears to have been the cause of the theorem's being known as "Stokes'
      theorem".
  17. ^Stewart, James (2010). Essential_Calculus:_Early_Transcendentals. Cole.
  18. ^ This proof is based on the Lecture Notes given by Prof. Robert Scheichl
      (University_of_Bath, U.K) [1], please refer the [2]
  19. ^ This_proof_is_also_same_to_the_proof_shown_in
  20. ^Renteln, Paul (2014). Manifolds, Tensors, and Forms. Cambridge, UK:
      Cambridge University Press. pp. 158â175. ISBN 9781107324893.
  21. ^Lee, John M. (2013). Introduction to Smooth Manifolds. New York:
      Springer. p. 481. ISBN 9781441999818.
  22. ^ Whitney, Geometric Integration Theory, III.14.
  23. ^Harrison, J. (October 1993). "Stokes' theorem for nonsmooth chains".
      Bulletin of the American Mathematical Society. New Series. 29 (2). arXiv:
      math/9310231.
  24. ^Jackson, J. D. (1975). Classical Electrodynamics (2nd ed.). New York,
      NY: Wiley.
  25. ^Born, M.; Wolf, E. (1980). Principles of Optics (6th ed.). Cambridge,
      England: Cambridge University Press.
***** Further reading[edit] *****
    * Grunsky,_Helmut (1983). The General Stokes' Theorem. Boston: Pitman.
      ISBN 0-273-08510-7.
Katz, Victor J. (May 1979). "The History of Stokes' Theorem". Mathematics
Magazine. 52 (3): 146â156. doi:10.2307/2690275. JSTOR 2690275.
Loomis,_Lynn_Harold; Sternberg,_Shlomo (2014). Advanced_Calculus. Hackensack,
New Jersey: World Scientific. ISBN 978-981-4583-93-0.
Madsen,_Ib; Tornehave, JÃ¸rgen (1997). From_Calculus_to_Cohomology:_De_Rham
cohomology_and_characteristic_classes. Cambridge, UK: Cambridge University
Press. ISBN 0-521-58956-8.
Marsden,_Jerrold_E.; Anthony, Tromba (2003). Vector Calculus (5th ed.). W. H.
Freeman.
Lee, John (2003). Introduction_to_Smooth_Manifolds. Springer-Verlag. ISBN 978-
0-387-95448-6.
Rudin,_Walter (1976). Principles_of_Mathematical_Analysis. New York, NY:
McGrawâHill. ISBN 0-07-054235-X.
Spivak,_Michael (1965). Calculus_on_Manifolds:_A_Modern_Approach_to_Classical
Theorems_of_Advanced_Calculus. San Francisco: Benjamin Cummings. ISBN 0-8053-
9021-9.
Stewart, James (2009). Calculus:_Concepts_and_Contexts. Cengage Learning.
pp. 960â967. ISBN 0-495-55742-0.
Stewart, James (2003). Calculus: Early Transcendental Functions (5th ed.).
Brooks/Cole.
Tu,_Loring_W. (2011). An Introduction to Manifolds (2nd ed.). New York:
Springer. ISBN 978-1-4419-7399-3.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Stokes_formula", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Proof_of_the_Divergence_Theorem_and_Stokes'_Theorem
Calculus_3_â_Stokes_Theorem_from_lamar.edu â an expository explanation

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Stokes%27_theorem&oldid=908012226"
Categories:
    * Differential_topology
    * Differential_forms
    * Duality_theories
    * Integration_on_manifolds
    * Theorems_in_calculus
    * Theorems_in_differential_geometry
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
    * Asturianu
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * Lumbaart
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 26 July 2019, at 20:14 (UTC).
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
