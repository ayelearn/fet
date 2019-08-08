The following text has been accessed from https://en.wikipedia.org/wiki/Green%27s_theorem at Thu Aug 8 23:25:28 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Green's theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the theorem in the plane relating double integrals and
line integrals. For Green's theorems relating volume integrals involving the
Laplacian to surface integrals, see Green's_identities.
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
In mathematics, Green's theorem gives the relationship between a line_integral
around a simple_closed_curve C and a double_integral over the plane region D
bounded by C. It is named after George_Green, though its first proof is due to
Bernhard_Riemann[1] and is the two-dimensional special case of the more general
KelvinâStokes_theorem.
⁰
***** Contents *****
    * 1_Theorem
    * 2_Proof_when_D_is_a_simple_region
    * 3_Proof_for_rectifiable_Jordan_curves
    * 4_Validity_under_different_hypotheses
          o 4.1_Measure-theoretic_assumptions
    * 5_Multiply-connected_regions
    * 6_Relationship_to_Stokes'_theorem
    * 7_Relationship_to_the_divergence_theorem
    * 8_Area_calculation
    * 9_See_also
    * 10_References
    * 11_Further_reading
    * 12_External_links
***** Theorem[edit] *****
Let C be a positively oriented, piecewise smooth, simple_closed_curve in a
plane, and let D be the region bounded by C. If L and M are functions of (x, y)
defined on an open_region containing D and having continuous partial
derivatives there, then
      [\ointctrclockwise]      C     {\displaystyle {\scriptstyle C}}  [
      {\displaystyle {\scriptstyle C}}]     ( L  d x + M  d y ) =  &#x222C;  D
      (     &#x2202; M   &#x2202; x    &#x2212;    &#x2202; L   &#x2202; y
      )   d x  d y   {\displaystyle (L\,dx+M\,dy)=\iint _{D}\left({\frac
      {\partial M}{\partial x}}-{\frac {\partial L}{\partial
      y}}\right)\,dx\,dy}  [{\displaystyle (L\,dx+M\,dy)=\iint _{D}\left({\frac
      {\partial M}{\partial x}}-{\frac {\partial L}{\partial
      y}}\right)\,dx\,dy}]

where the path of integration along C is anticlockwise.[2][3]
In physics, Green's theorem finds many applications. One is solving two-
dimensional flow integrals, stating that the sum of fluid outflowing from a
volume is equal to the total outflow summed about an enclosing area. In plane
geometry, and in particular, area surveying, Green's theorem can be used to
determine the area and centroid of plane figures solely by integrating over the
perimeter.
***** Proof when D is a simple region[edit] *****
If D is a simple type I region with its boundary consisting of the curves C1,
C2, C3, C4, half of Green's theorem can be demonstrated.
The following is a proof of half of the theorem for the simplified area D, a
type I region where C1 and C3 are curves connected by vertical lines (possibly
of zero length). A similar proof exists for the other half of the theorem when
D is a type II region where C2 and C4 are curves connected by horizontal lines
(again, possibly of zero length). Putting these two parts together, the theorem
is thus proven for regions of type III (defined as regions which are both type
I and type II). The general case can then be deduced from this special case by
decomposing D into a set of type III regions.
If it can be shown that if
             &#x222E;       C   &#x2061; L  d x =  &#x222C;  D    (  &#x2212;
      &#x2202; L   &#x2202; y     )   d A   ( 1 )    {\displaystyle \oint _
      {C}L\,dx=\iint _{D}\left(-{\frac {\partial L}{\partial
      y}}\right)\,dA\qquad \mathrm {(1)} }  [\oint _{C}L\,dx=\iint _{D}\left(-
      {\frac {\partial L}{\partial y}}\right)\,dA\qquad \mathrm {(1)} ]
and
             &#x222E;       C   &#x2061; M  d y =  &#x222C;  D    (    &#x2202;
      M   &#x2202; x    )   d A   ( 2 )    {\displaystyle \oint _{C}M\,dy=\iint
      _{D}\left({\frac {\partial M}{\partial x}}\right)\,dA\qquad \mathrm {(2)}
      }  [\oint _{C}M\,dy=\iint _{D}\left({\frac {\partial M}{\partial
      x}}\right)\,dA\qquad \mathrm {(2)} ]
are true, then Green's theorem follows immediately for the region D. We can
prove (1) easily for regions of type I, and (2) for regions of type II. Green's
theorem then follows for regions of type III.
Assume region D is a type I region and can thus be characterized, as pictured
on the right, by
         D = { ( x , y ) &#x2223; a &#x2264; x &#x2264; b ,  g  1   ( x )
      &#x2264; y &#x2264;  g  2   ( x ) }   {\displaystyle D=\{(x,y)\mid a\leq
      x\leq b,g_{1}(x)\leq y\leq g_{2}(x)\}}  [{\displaystyle D=\{(x,y)\mid
      a\leq x\leq b,g_{1}(x)\leq y\leq g_{2}(x)\}}]
where g1 and g2 are continuous_functions on [a, b]. Compute the double integral
in (1):
              &#x222C;  D      &#x2202; L   &#x2202; y     d A    =  &#x222B;
      a   b     &#x222B;   g  1   ( x )    g  2   ( x )      &#x2202; L
      &#x2202; y    ( x , y )  d y  d x       =  &#x222B;  a   b     {   L ( x
      ,  g  2   ( x ) ) &#x2212; L ( x ,  g  1   ( x ) )   }    d x .   ( 3 )
      {\displaystyle {\begin{aligned}\iint _{D}{\frac {\partial L}{\partial
      y}}\,dA&=\int _{a}^{b}\,\int _{g_{1}(x)}^{g_{2}(x)}{\frac {\partial L}
      {\partial y}}(x,y)\,dy\,dx\\&=\int _{a}^{b}{\Big \{}L(x,g_{2}(x))-L(x,g_
      {1}(x)){\Big \}}\,dx.\qquad \mathrm {(3)} \end{aligned}}}  [{\begin
      {aligned}\iint _{D}{\frac {\partial L}{\partial y}}\,dA&=\int _{a}^
      {b}\,\int _{g_{1}(x)}^{g_{2}(x)}{\frac {\partial L}{\partial y}}
      (x,y)\,dy\,dx\\&=\int _{a}^{b}{\Big \{}L(x,g_{2}(x))-L(x,g_{1}(x)){\Big
      \}}\,dx.\qquad \mathrm {(3)} \end{aligned}}]
Now compute the line integral in (1). C can be rewritten as the union of four
curves: C1, C2, C3, C4.
With C1, use the parametric_equations: x = x, y = g1(x), a â¤ x â¤ b. Then
          &#x222B;   C  1     L ( x , y )  d x =  &#x222B;  a   b   L ( x ,  g
      1   ( x ) )  d x .   {\displaystyle \int _{C_{1}}L(x,y)\,dx=\int _{a}^
      {b}L(x,g_{1}(x))\,dx.}  [\int _{C_{1}}L(x,y)\,dx=\int _{a}^{b}L(x,g_{1}
      (x))\,dx.]
With C3, use the parametric equations: x = x, y = g2(x), a â¤ x â¤ b. Then
          &#x222B;   C  3     L ( x , y )  d x = &#x2212;  &#x222B;  &#x2212;
      C  3     L ( x , y )  d x = &#x2212;  &#x222B;  a   b   L ( x ,  g  2
      ( x ) )  d x .   {\displaystyle \int _{C_{3}}L(x,y)\,dx=-\int _{-C_{3}}L
      (x,y)\,dx=-\int _{a}^{b}L(x,g_{2}(x))\,dx.}  [\int _{C_{3}}L(x,y)\,dx=-
      \int _{-C_{3}}L(x,y)\,dx=-\int _{a}^{b}L(x,g_{2}(x))\,dx.]
The integral over C3 is negated because it goes in the negative direction from
b to a, as C is oriented positively (anticlockwise). On C2 and C4, x remains
constant, meaning
          &#x222B;   C  4     L ( x , y )  d x =  &#x222B;   C  2     L ( x , y
      )  d x = 0.   {\displaystyle \int _{C_{4}}L(x,y)\,dx=\int _{C_{2}}L
      (x,y)\,dx=0.}  [\int _{C_{4}}L(x,y)\,dx=\int _{C_{2}}L(x,y)\,dx=0.]
Therefore,
              &#x222B;  C   L  d x    =  &#x222B;   C  1     L ( x , y )  d x +
      &#x222B;   C  2     L ( x , y )  d x +  &#x222B;   C  3     L ( x , y )
      d x +  &#x222B;   C  4     L ( x , y )  d x       =  &#x222B;  a   b   L
      ( x ,  g  1   ( x ) )  d x &#x2212;  &#x222B;  a   b   L ( x ,  g  2
      ( x ) )  d x .   ( 4 )        {\displaystyle {\begin{aligned}\int _
      {C}L\,dx&=\int _{C_{1}}L(x,y)\,dx+\int _{C_{2}}L(x,y)\,dx+\int _{C_{3}}L
      (x,y)\,dx+\int _{C_{4}}L(x,y)\,dx\\&=\int _{a}^{b}L(x,g_{1}(x))\,dx-\int
      _{a}^{b}L(x,g_{2}(x))\,dx.\qquad \mathrm {(4)} \end{aligned}}}  [
      {\displaystyle {\begin{aligned}\int _{C}L\,dx&=\int _{C_{1}}L
      (x,y)\,dx+\int _{C_{2}}L(x,y)\,dx+\int _{C_{3}}L(x,y)\,dx+\int _{C_{4}}L
      (x,y)\,dx\\&=\int _{a}^{b}L(x,g_{1}(x))\,dx-\int _{a}^{b}L(x,g_{2}
      (x))\,dx.\qquad \mathrm {(4)} \end{aligned}}}]
Combining (3) with (4), we get (1) for regions of type I. A similar treatment
yields (2) for regions of type II. Putting the two together, we get the result
for regions of type III.
***** Proof for rectifiable Jordan curves[edit] *****
We are going to prove the following
Theorem. Let     &#x0393;   {\displaystyle \Gamma }  [\Gamma ] be a
rectifiable, positively oriented Jordan_curve in       R   2     {\displaystyle
\mathbf {R} ^{2}}  [{\displaystyle \mathbf {R} ^{2}}] and let     R
{\displaystyle R}  [R] denote its inner region. Suppose that     A , B :   R
&#x00AF;   &#x27F6;  R    {\displaystyle A,B:{\overline {R}}\longrightarrow
\mathbf {R} }  [{\displaystyle A,B:{\overline {R}}\longrightarrow \mathbf {R}
}] are continuous functions with the property that     A   {\displaystyle A}
[A] has second partial derivative at every point of     R   {\displaystyle R}
[R],     B   {\displaystyle B}  [B] has first partial derivative at every point
of     R   {\displaystyle R}  [R] and that the functions      D  1   B
{\displaystyle D_{1}B}  [{\displaystyle D_{1}B}],      D  2   A : R &#x27F6;  R
{\displaystyle D_{2}A:R\longrightarrow \mathbf {R} }  [{\displaystyle D_{2}A:
R\longrightarrow \mathbf {R} }] are Riemann-integrable over     R
{\displaystyle R}  [R]. Then
    &#x222B;  &#x0393;   A  d x + B  d y =  &#x222B;  R      (   D  1   B ( x ,
y ) &#x2212;  D  2   A ( x , y )  )   d ( x , y ) .   {\displaystyle \int _
{\Gamma }A\,dx+B\,dy=\int _{R}\,\,\left(D_{1}B(x,y)-D_{2}A(x,y)\right)\,d
(x,y).}
[{\displaystyle \int _{\Gamma }A\,dx+B\,dy=\int _{R}\,\,\left(D_{1}B(x,y)-D_
{2}A(x,y)\right)\,d(x,y).}]
We need the following lemmas:
Lemma 1 (Decomposition Lemma). Assume     &#x0393;   {\displaystyle \Gamma }
[\Gamma ] is a rectifiable, positively oriented Jordan curve in the plane and
let     R   {\displaystyle R}  [R] be its inner region. For every positive real
&#x03B4;   {\displaystyle \delta }  [\delta ], let       F   ( &#x03B4; )
{\displaystyle {\mathcal {F}}(\delta )}  [{\displaystyle {\mathcal {F}}(\delta
)}] denote the collection of squares in the plane bounded by the lines     x =
m &#x03B4; , y = m &#x03B4;   {\displaystyle x=m\delta ,y=m\delta }  [
{\displaystyle x=m\delta ,y=m\delta }], where     m   {\displaystyle m}  [m]
runs through the set of integers. Then, for this     &#x03B4;   {\displaystyle
\delta }  [\delta ], there exists a decomposition of       R &#x00AF;
{\displaystyle {\overline {R}}}  [{\overline {R}}] into a finite number of non-
overlapping subregions in such a manner that
(i) Each one of the subregions contained in     R   {\displaystyle R}  [R], say
R  1   ,  R  2   , &#x2026; ,  R  k     {\displaystyle R_{1},R_{2},\ldots ,R_
{k}}  [{\displaystyle R_{1},R_{2},\ldots ,R_{k}}], is a square from       F
( &#x03B4; )   {\displaystyle {\mathcal {F}}(\delta )}  [{\displaystyle
{\mathcal {F}}(\delta )}].
(ii) Each one of the remaining subregions, say      R  k + 1   , &#x2026; ,  R
s     {\displaystyle R_{k+1},\ldots ,R_{s}}  [{\displaystyle R_{k+1},\ldots ,R_
{s}}], has as boundary a rectifiable Jordan curve formed by a finite number of
arcs of     &#x0393;   {\displaystyle \Gamma }  [\Gamma ] and parts of the
sides of some square from       F   ( &#x03B4; )   {\displaystyle {\mathcal
{F}}(\delta )}  [{\displaystyle {\mathcal {F}}(\delta )}].
(iii) Each one of the border regions      R  k + 1   , &#x2026; ,  R  s
{\displaystyle R_{k+1},\ldots ,R_{s}}  [{\displaystyle R_{k+1},\ldots ,R_{s}}]
can be enclosed in a square of edge-length     2 &#x03B4;   {\displaystyle
2\delta }  [2\delta].
(iv) If      &#x0393;  i     {\displaystyle \Gamma _{i}}  [\Gamma _{i}] is the
positively oriented boundary curve of      R  i     {\displaystyle R_{i}}  [R_
{i}], then     &#x0393; =  &#x0393;  1   +  &#x0393;  2   + &#x22EF; +
&#x0393;  s   .   {\displaystyle \Gamma =\Gamma _{1}+\Gamma _{2}+\cdots +\Gamma
_{s}.}  [{\displaystyle \Gamma =\Gamma _{1}+\Gamma _{2}+\cdots +\Gamma _{s}.}]
(v) The number     s &#x2212; k   {\displaystyle s-k}  [{\displaystyle s-k}] of
border regions is no greater than     4   (    &#x039B; &#x03B4;   + 1  )
{\displaystyle 4\!\left({\frac {\Lambda }{\delta }}+1\right)}  [{\displaystyle
4\!\left({\frac {\Lambda }{\delta }}+1\right)}], where     &#x039B;
{\displaystyle \Lambda }  [\Lambda ] is the length of     &#x0393;
{\displaystyle \Gamma }  [\Gamma ].
Lemma 2. Let     &#x0393;   {\displaystyle \Gamma }  [\Gamma ] be a rectifiable
curve in the plane and let      &#x0394;  &#x0393;   ( h )   {\displaystyle
\Delta _{\Gamma }(h)}  [{\displaystyle \Delta _{\Gamma }(h)}] be the set of
points in the plane whose distance from (the range of)     &#x0393;
{\displaystyle \Gamma }  [\Gamma ] is at most     h   {\displaystyle h}  [h].
The outer Jordan content of this set satisfies       c &#x00AF;      &#x0394;
&#x0393;   ( h ) &#x2264; 2 h &#x039B; + &#x03C0;  h  2     {\displaystyle
{\overline {c}}\,\,\Delta _{\Gamma }(h)\leq 2h\Lambda +\pi h^{2}}  [
{\displaystyle {\overline {c}}\,\,\Delta _{\Gamma }(h)\leq 2h\Lambda +\pi h^
{2}}].
Lemma 3. Let     &#x0393;   {\displaystyle \Gamma }  [\Gamma ] be a rectifiable
curve in       R   2     {\displaystyle \mathbf {R} ^{2}}  [{\displaystyle
\mathbf {R} ^{2}}] and let     f :  range of&#xA0;  &#x0393; &#x27F6;  R
{\displaystyle f:{\text{range of }}\Gamma \longrightarrow \mathbf {R} }  [
{\displaystyle f:{\text{range of }}\Gamma \longrightarrow \mathbf {R} }] be a
continuous function. Then
          |   &#x222B;  &#x0393;   f ( x , y )  d y  |    {\displaystyle
      \left\vert \int _{\Gamma }f(x,y)\,dy\right\vert }  [{\displaystyle
      \left\vert \int _{\Gamma }f(x,y)\,dy\right\vert }] and
          |   &#x222B;  &#x0393;   f ( x , y )  d x  |    {\displaystyle
      \left\vert \int _{\Gamma }f(x,y)\,dx\right\vert }  [{\displaystyle
      \left\vert \int _{\Gamma }f(x,y)\,dx\right\vert }] are     &#x2264;   1 2
      &#x039B;  &#x03A9;  f   ,   {\displaystyle \leq {\frac {1}{2}}\Lambda
      \Omega _{f},}  [{\displaystyle \leq {\frac {1}{2}}\Lambda \Omega _
      {f},}]where      &#x03A9;  f     {\displaystyle \Omega _{f}}  [
      {\displaystyle \Omega _{f}}] is the oscillation of     f   {\displaystyle
      f}  [f] on the range of     &#x0393;   {\displaystyle \Gamma }  [\Gamma
      ].
Now we are in position to prove the Theorem:
Proof of Theorem. Let     &#x03B5;   {\displaystyle \varepsilon }  [\varepsilon
] be an arbitrary positive real number. By continuity of     A   {\displaystyle
A}  [A],     B   {\displaystyle B}  [B] and compactness of       R &#x00AF;
{\displaystyle {\overline {R}}}  [{\overline {R}}], given     &#x03B5; > 0
{\displaystyle \varepsilon >0}  [\varepsilon >0], there exists     0 < &#x03B4;
< 1   {\displaystyle 0<\delta <1}  [0<\delta<1] such that whenever two points
of       R &#x00AF;     {\displaystyle {\overline {R}}}  [{\overline {R}}] are
less than     2   2    &#x03B4;   {\displaystyle 2{\sqrt {2}}\,\delta }  [
{\displaystyle 2{\sqrt {2}}\,\delta }] apart, their images under     A , B
{\displaystyle A,B}  [A,B] are less than     &#x03B5;   {\displaystyle
\varepsilon }  [\varepsilon ] apart. For this     &#x03B4;   {\displaystyle
\delta }  [\delta ], consider the decomposition given by the previous Lemma. We
have
          &#x222B;  &#x0393;   A  d x + B  d y =  &#x2211;  i = 1   k
      &#x222B;   &#x0393;  i     A  d x + B  d y  +  &#x2211;  i = k + 1   s
      &#x222B;   &#x0393;  i     A  d x + B  d y .   {\displaystyle \int _
      {\Gamma }A\,dx+B\,dy=\sum _{i=1}^{k}\int _{\Gamma _{i}}A\,dx+B\,dy\quad
      +\sum _{i=k+1}^{s}\int _{\Gamma _{i}}A\,dx+B\,dy.}  [{\displaystyle \int
      _{\Gamma }A\,dx+B\,dy=\sum _{i=1}^{k}\int _{\Gamma _{i}}A\,dx+B\,dy\quad
      +\sum _{i=k+1}^{s}\int _{\Gamma _{i}}A\,dx+B\,dy.}]
Put     &#x03C6; :=  D  1   B &#x2212;  D  2   A   {\displaystyle \varphi :=D_
{1}B-D_{2}A}  [{\displaystyle \varphi :=D_{1}B-D_{2}A}].
For each     i &#x2208; { 1 , &#x2026; , k }   {\displaystyle i\in \{1,\ldots
,k\}}  [{\displaystyle i\in \{1,\ldots ,k\}}], the curve      &#x0393;  i
{\displaystyle \Gamma _{i}}  [\Gamma _{i}] is a positively oriented square, for
which Green's formula holds. Hence
          &#x2211;  i = 1   k    &#x222B;   &#x0393;  i     A  d x + B  d y =
      &#x2211;  i = 1   k    &#x222B;   R  i       &#x03C6; =  &#x222B;
      &#x22C3;  i = 1   k    R  i      &#x03C6; .   {\displaystyle \sum _{i=1}^
      {k}\int _{\Gamma _{i}}A\,dx+B\,dy=\sum _{i=1}^{k}\int _{R_{i}}\,\,\varphi
      =\int _{\bigcup _{i=1}^{k}R_{i}}\,\varphi .}  [{\displaystyle \sum _
      {i=1}^{k}\int _{\Gamma _{i}}A\,dx+B\,dy=\sum _{i=1}^{k}\int _{R_
      {i}}\,\,\varphi =\int _{\bigcup _{i=1}^{k}R_{i}}\,\varphi .}]
Every point of a border region is at a distance no greater than     2   2
&#x03B4;   {\displaystyle 2{\sqrt {2}}\,\delta }  [{\displaystyle 2{\sqrt
{2}}\,\delta }] from     &#x0393;   {\displaystyle \Gamma }  [\Gamma ]. Thus,
if     K   {\displaystyle K}  [K] is the union of all border regions, then
K &#x2282;  &#x0394;  &#x0393;   ( 2   2    &#x03B4; )   {\displaystyle
K\subset \Delta _{\Gamma }(2{\sqrt {2}}\,\delta )}  [{\displaystyle K\subset
\Delta _{\Gamma }(2{\sqrt {2}}\,\delta )}]; hence     c ( K ) &#x2264;   c
&#x00AF;     &#x0394;  &#x0393;   ( 2   2    &#x03B4; ) &#x2264; 4   2
&#x03B4; + 8 &#x03C0;  &#x03B4;  2     {\displaystyle c(K)\leq {\overline
{c}}\,\Delta _{\Gamma }(2{\sqrt {2}}\,\delta )\leq 4{\sqrt {2}}\,\delta +8\pi
\delta ^{2}}  [{\displaystyle c(K)\leq {\overline {c}}\,\Delta _{\Gamma }(2
{\sqrt {2}}\,\delta )\leq 4{\sqrt {2}}\,\delta +8\pi \delta ^{2}}], by Lemma 2.
Notice that
          &#x222B;  R   &#x03C6;   &#x2212;  &#x222B;   &#x22C3;  i = 1   k
      R  i     &#x03C6; =  &#x222B;  K   &#x03C6; .   {\displaystyle \int _
      {R}\varphi \,\,-\int _{\bigcup _{i=1}^{k}R_{i}}\varphi =\int _{K}\varphi
      .}  [{\displaystyle \int _{R}\varphi \,\,-\int _{\bigcup _{i=1}^{k}R_
      {i}}\varphi =\int _{K}\varphi .}] This yields
          |   &#x2211;  i = 1   k    &#x222B;   &#x0393;  i     A  d x + B  d y
      &#x2212;  &#x222B;  R   &#x03C6;  |  &#x2264; M &#x03B4; ( 1 + &#x03C0;
      2    &#x03B4; )  &#xA0;for some&#xA0;  M > 0.   {\displaystyle \left\vert
      \sum _{i=1}^{k}\int _{\Gamma _{i}}A\,dx+B\,dy\quad -\int _{R}\varphi
      \right\vert \leq M\delta (1+\pi {\sqrt {2}}\,\delta ){\text{ for some
      }}M>0.}  [{\displaystyle \left\vert \sum _{i=1}^{k}\int _{\Gamma _
      {i}}A\,dx+B\,dy\quad -\int _{R}\varphi \right\vert \leq M\delta (1+\pi
      {\sqrt {2}}\,\delta ){\text{ for some }}M>0.}]
We may as well choose     &#x03B4;   {\displaystyle \delta }  [\delta ] so that
the RHS of the last inequality is     < &#x03B5; .   {\displaystyle
<\varepsilon .}  [{\displaystyle <\varepsilon .}]
The remark in the beginning of this proof implies that the oscillations of
A   {\displaystyle A}  [A] and     B   {\displaystyle B}  [B] on every border
region is at most     &#x03B5;   {\displaystyle \varepsilon }  [\varepsilon ].
We have
          |   &#x2211;  i = k + 1   s    &#x222B;   &#x0393;  i     A  d x + B
      d y  |  &#x2264;   1 2   &#x03B5;  &#x2211;  i = k + 1   s    &#x039B;  i
      .   {\displaystyle \left\vert \sum _{i=k+1}^{s}\int _{\Gamma _
      {i}}A\,dx+B\,dy\right\vert \leq {\frac {1}{2}}\varepsilon \sum _{i=k+1}^
      {s}\Lambda _{i}.}  [{\displaystyle \left\vert \sum _{i=k+1}^{s}\int _
      {\Gamma _{i}}A\,dx+B\,dy\right\vert \leq {\frac {1}{2}}\varepsilon \sum _
      {i=k+1}^{s}\Lambda _{i}.}]
By Lemma 1(iii),
          &#x2211;  i = k + 1   s    &#x039B;  i   &#x2264; &#x039B; + ( 4
      &#x03B4; )  4   (    &#x039B; &#x03B4;   + 1  )  &#x2264; 17 &#x039B; +
      16.   {\displaystyle \sum _{i=k+1}^{s}\Lambda _{i}\leq \Lambda +(4\delta
      )\,4\!\left({\frac {\Lambda }{\delta }}+1\right)\leq 17\Lambda +16.}  [
      {\displaystyle \sum _{i=k+1}^{s}\Lambda _{i}\leq \Lambda +(4\delta
      )\,4\!\left({\frac {\Lambda }{\delta }}+1\right)\leq 17\Lambda +16.}]
Combining these, we finally get
          |   &#x222B;  &#x0393;   A  d x + B  d y  &#x2212;  &#x222B;  R
      &#x03C6;  |  < C &#x03B5; ,   {\displaystyle \left\vert \int _{\Gamma
      }A\,dx+B\,dy\quad -\int _{R}\varphi \right\vert <C\varepsilon ,}  [
      {\displaystyle \left\vert \int _{\Gamma }A\,dx+B\,dy\quad -\int _
      {R}\varphi \right\vert <C\varepsilon ,}]
for some     C > 0   {\displaystyle C>0}  [C>0]. Since this is true for every
&#x03B5; > 0   {\displaystyle \varepsilon >0}  [\varepsilon >0], we are done.
***** Validity under different hypotheses[edit] *****
The hypothesis of the last theorem are not the only ones under which Green's
formula is true. Another common set of conditions is the following:
The functions     A , B :   R &#x00AF;   &#x27F6;  R    {\displaystyle A,B:
{\overline {R}}\longrightarrow \mathbf {R} }  [{\displaystyle A,B:{\overline
{R}}\longrightarrow \mathbf {R} }] are still assumed to be continuous. However,
we now require them to be FrÃ©chet-differentiable at every point of     R
{\displaystyle R}  [R]. This implies the existence of all directional
derivatives, in particular      D   e  i     A =:  D  i   A ,  D   e  i     B
=:  D  i   B ,  i = 1 , 2   {\displaystyle D_{e_{i}}A=:D_{i}A,D_{e_{i}}B=:D_
{i}B,\,i=1,2}  [{\displaystyle D_{e_{i}}A=:D_{i}A,D_{e_{i}}B=:D_{i}B,\,i=1,2}],
where, as usual,     (  e  1   ,  e  2   )   {\displaystyle (e_{1},e_{2})}  [
{\displaystyle (e_{1},e_{2})}] is the canonical ordered basis of       R   2
{\displaystyle \mathbf {R} ^{2}}  [\mathbf{R}^2]. In addition, we require the
function      D  1   B &#x2212;  D  2   A   {\displaystyle D_{1}B-D_{2}A}  [
{\displaystyle D_{1}B-D_{2}A}] to be Riemann-integrable over     R
{\displaystyle R}  [R].

As a corollary of this, we get the Cauchy Integral Theorem for rectifiable
Jordan curves:
Theorem (Cauchy). If     &#x0393;   {\displaystyle \Gamma }  [\Gamma ] is a
rectifiable Jordan curve in      C    {\displaystyle \mathbf {C} }  [\mathbf
{C} ] and if     f :  closure of inner region of&#xA0;  &#x0393; &#x27F6;  C
{\displaystyle f:{\text{closure of inner region of }}\Gamma \longrightarrow
\mathbf {C} }  [{\displaystyle f:{\text{closure of inner region of }}\Gamma
\longrightarrow \mathbf {C} }] is a continuous mapping holomorphic throughout
the inner region of     &#x0393;   {\displaystyle \Gamma }  [\Gamma ], then
          &#x222B;  &#x0393;   f = 0 ,   {\displaystyle \int _{\Gamma }f=0,}  [
      {\displaystyle \int _{\Gamma }f=0,}]
the integral being a complex contour integral.
Proof. We regard the complex plane as       R   2     {\displaystyle \mathbf
{R} ^{2}}  [{\displaystyle \mathbf {R} ^{2}}]. Now, define     u , v :   R
&#x00AF;   &#x27F6;  R    {\displaystyle u,v:{\overline {R}}\longrightarrow
\mathbf {R} }  [{\displaystyle u,v:{\overline {R}}\longrightarrow \mathbf {R}
}] to be such that     f ( x + i y ) = u ( x , y ) + i v ( x , y ) .
{\displaystyle f(x+iy)=u(x,y)+iv(x,y).}  [{\displaystyle f(x+iy)=u(x,y)+iv
(x,y).}] These functions are clearly continuous. It is well known that     u
{\displaystyle u}  [u] and     v   {\displaystyle v}  [v] are FrÃ©chet-
differentiable and that they satisfy the Cauchy-Riemann equations:      D  1
v +  D  2   u =  D  1   u &#x2212;  D  2   v =  zero function    {\displaystyle
D_{1}v+D_{2}u=D_{1}u-D_{2}v={\text{zero function}}}  [{\displaystyle D_{1}v+D_
{2}u=D_{1}u-D_{2}v={\text{zero function}}}].
Now, analysing the sums used to define the complex contour integral in
question, it is easy to realize that
          &#x222B;  &#x0393;   f =  &#x222B;  &#x0393;   u  d x &#x2212; v  d y
      + i  &#x222B;  &#x0393;   v  d x + u  d y ,   {\displaystyle \int _
      {\Gamma }f=\int _{\Gamma }u\,dx-v\,dy\quad +i\int _{\Gamma }v\,dx+u\,dy,}
      [{\displaystyle \int _{\Gamma }f=\int _{\Gamma }u\,dx-v\,dy\quad +i\int _
      {\Gamma }v\,dx+u\,dy,}]
the integrals on the RHS being usual line integrals. These remarks allow us to
apply Green's Theorem to each one of these line integrals, finishing the proof.
**** Measure-theoretic assumptions[edit] ****
Green's formula also holds when, besides continuity assumptions,
(i) The functions      D  i   A ,  D  i   B ,  i = 1 , 2   {\displaystyle D_
{i}A,D_{i}B,\,i=1,2}  [{\displaystyle D_{i}A,D_{i}B,\,i=1,2}], are defined at
every point of     R   {\displaystyle R}  [R], with the exception of a
countable subset.
(ii) The function      D  1   B &#x2212;  D  2   A   {\displaystyle D_{1}B-D_
{2}A}  [{\displaystyle D_{1}B-D_{2}A}] is Lebesgue-integrable over     R
{\displaystyle R}  [R].
***** Multiply-connected regions[edit] *****
Theorem. Let      &#x0393;  0   ,  &#x0393;  1   , &#x2026; ,  &#x0393;  n
{\displaystyle \Gamma _{0},\Gamma _{1},\ldots ,\Gamma _{n}}  [{\displaystyle
\Gamma _{0},\Gamma _{1},\ldots ,\Gamma _{n}}] be positively oriented
rectifiable Jordan curves in       R   2     {\displaystyle \mathbf {R} ^{2}}
[{\displaystyle \mathbf {R} ^{2}}] satisfying
              &#x0393;  i   &#x2282;  R  0   ,     if&#xA0;  1 &#x2264; i
      &#x2264; n      &#x0393;  i   &#x2282;   R   2   &#x2216;    R &#x00AF;
      j   ,     if&#xA0;  1 &#x2264; i , j &#x2264; n  &#xA0;and&#xA0;  i
      &#x2260; j ,       {\displaystyle {\begin{aligned}\Gamma _{i}\subset R_
      {0},&&{\text{if }}1\leq i\leq n\\\Gamma _{i}\subset \mathbf {R} ^
      {2}\smallsetminus {\overline {R}}_{j},&&{\text{if }}1\leq i,j\leq n{\text
      { and }}i\neq j,\end{aligned}}}  [{\displaystyle {\begin{aligned}\Gamma _
      {i}\subset R_{0},&&{\text{if }}1\leq i\leq n\\\Gamma _{i}\subset \mathbf
      {R} ^{2}\smallsetminus {\overline {R}}_{j},&&{\text{if }}1\leq i,j\leq n
      {\text{ and }}i\neq j,\end{aligned}}}]
where      R  i     {\displaystyle R_{i}}  [R_{i}] is the inner region of
&#x0393;  i     {\displaystyle \Gamma _{i}}  [\Gamma _{i}]. Let
         D =  R  0   &#x2216; (    R &#x00AF;    1   &#x222A;    R &#x00AF;
      2   &#x222A; &#x22EF; &#x222A;    R &#x00AF;    n   ) .   {\displaystyle
      D=R_{0}\smallsetminus ({\overline {R}}_{1}\cup {\overline {R}}_{2}\cup
      \cdots \cup {\overline {R}}_{n}).}  [{\displaystyle D=R_{0}\smallsetminus
      ({\overline {R}}_{1}\cup {\overline {R}}_{2}\cup \cdots \cup {\overline
      {R}}_{n}).}]
Suppose     p :   D &#x00AF;   &#x27F6;  R    {\displaystyle p:{\overline
{D}}\longrightarrow \mathbf {R} }  [{\displaystyle p:{\overline
{D}}\longrightarrow \mathbf {R} }] and     q :   D &#x00AF;   &#x27F6;  R
{\displaystyle q:{\overline {D}}\longrightarrow \mathbf {R} }  [{\displaystyle
q:{\overline {D}}\longrightarrow \mathbf {R} }] are continuous functions whose
restriction to     D   {\displaystyle D}  [D] is FrÃ©chet-differentiable. If
the function
         ( x , y ) &#x27FC;    &#x2202; q   &#x2202;  e  1      ( x , y )
      &#x2212;    &#x2202; p   &#x2202;  e  2      ( x , y )   {\displaystyle
      (x,y)\longmapsto {\frac {\partial q}{\partial e_{1}}}(x,y)-{\frac
      {\partial p}{\partial e_{2}}}(x,y)}  [{\displaystyle (x,y)\longmapsto
      {\frac {\partial q}{\partial e_{1}}}(x,y)-{\frac {\partial p}{\partial e_
      {2}}}(x,y)}]
is Riemann-integrable over     D   {\displaystyle D}  [D], then
                &#x222B;   &#x0393;  0     p ( x , y )  d x + q ( x , y )  d y
      &#x2212;  &#x2211;  i = 1   n    &#x222B;   &#x0393;  i     p ( x , y )
      d x + q ( x , y )  d y     =       &#x222B;  D    {     &#x2202; q
      &#x2202;  e  1      ( x , y ) &#x2212;    &#x2202; p   &#x2202;  e  2
      ( x , y )  }   d ( x , y ) .       {\displaystyle {\begin{aligned}&\int _
      {\Gamma _{0}}p(x,y)\,dx+q(x,y)\,dy-\sum _{i=1}^{n}\int _{\Gamma _{i}}p
      (x,y)\,dx+q(x,y)\,dy\\[5pt]={}&\int _{D}\left\{{\frac {\partial q}
      {\partial e_{1}}}(x,y)-{\frac {\partial p}{\partial e_{2}}}
      (x,y)\right\}\,d(x,y).\end{aligned}}}  [{\displaystyle {\begin
      {aligned}&\int _{\Gamma _{0}}p(x,y)\,dx+q(x,y)\,dy-\sum _{i=1}^{n}\int _
      {\Gamma _{i}}p(x,y)\,dx+q(x,y)\,dy\\[5pt]={}&\int _{D}\left\{{\frac
      {\partial q}{\partial e_{1}}}(x,y)-{\frac {\partial p}{\partial e_{2}}}
      (x,y)\right\}\,d(x,y).\end{aligned}}}]
***** Relationship to Stokes' theorem[edit] *****
Green's theorem is a special case of the KelvinâStokes_theorem, when applied
to a region in the     x y   {\displaystyle xy}  [xy]-plane.
We can augment the two-dimensional field into a three-dimensional field with a
z component that is always 0. Write F for the vector-valued function      F  =
( L , M , 0 )   {\displaystyle \mathbf {F} =(L,M,0)}  [\mathbf {F} =(L,M,0)].
Start with the left side of Green's theorem:
             &#x222E;       C   &#x2061; ( L  d x + M  d y ) =     &#x222E;
      C   &#x2061; ( L , M , 0 ) &#x22C5; ( d x , d y , d z ) =     &#x222E;
      C   &#x2061;  F  &#x22C5; d  r  .   {\displaystyle \oint _{C}
      (L\,dx+M\,dy)=\oint _{C}(L,M,0)\cdot (dx,dy,dz)=\oint _{C}\mathbf {F}
      \cdot d\mathbf {r} .}  [{\displaystyle \oint _{C}(L\,dx+M\,dy)=\oint _{C}
      (L,M,0)\cdot (dx,dy,dz)=\oint _{C}\mathbf {F} \cdot d\mathbf {r} .}]
The KelvinâStokes theorem:
             &#x222E;       C   &#x2061;  F  &#x22C5; d  r  =  &#x222C;  S
      &#x2207; &#x00D7;  F  &#x22C5;    n &#x005E;     d S .   {\displaystyle
      \oint _{C}\mathbf {F} \cdot d\mathbf {r} =\iint _{S}\nabla \times \mathbf
      {F} \cdot \mathbf {\hat {n}} \,dS.}  [{\displaystyle \oint _{C}\mathbf
      {F} \cdot d\mathbf {r} =\iint _{S}\nabla \times \mathbf {F} \cdot \mathbf
      {\hat {n}} \,dS.}]
The surface     S   {\displaystyle S}  [S] is just the region in the plane
D   {\displaystyle D}  [D], with the unit normal        n &#x005E;
{\displaystyle \mathbf {\hat {n}} }  [\mathbf {\hat {n}} ] pointing up (in the
positive     z   {\displaystyle z}  [z] direction) to match the "positive
orientation" definitions for both theorems.
The expression inside the integral becomes
         &#x2207; &#x00D7;  F  &#x22C5;    n &#x005E;    =  [   (     &#x2202;
      0   &#x2202; y    &#x2212;    &#x2202; M   &#x2202; z     )   i  +
      (     &#x2202; L   &#x2202; z    &#x2212;    &#x2202; 0   &#x2202; x
      )   j  +  (     &#x2202; M   &#x2202; x    &#x2212;    &#x2202; L
      &#x2202; y     )   k   ]  &#x22C5;  k  =  (     &#x2202; M   &#x2202; x
      &#x2212;    &#x2202; L   &#x2202; y     )  .   {\displaystyle \nabla
      \times \mathbf {F} \cdot \mathbf {\hat {n}} =\left[\left({\frac {\partial
      0}{\partial y}}-{\frac {\partial M}{\partial z}}\right)\mathbf {i} +\left
      ({\frac {\partial L}{\partial z}}-{\frac {\partial 0}{\partial
      x}}\right)\mathbf {j} +\left({\frac {\partial M}{\partial x}}-{\frac
      {\partial L}{\partial y}}\right)\mathbf {k} \right]\cdot \mathbf {k}
      =\left({\frac {\partial M}{\partial x}}-{\frac {\partial L}{\partial
      y}}\right).}  [\nabla \times \mathbf {F} \cdot \mathbf {\hat {n}} =\left
      [\left({\frac {\partial 0}{\partial y}}-{\frac {\partial M}{\partial
      z}}\right)\mathbf {i} +\left({\frac {\partial L}{\partial z}}-{\frac
      {\partial 0}{\partial x}}\right)\mathbf {j} +\left({\frac {\partial M}
      {\partial x}}-{\frac {\partial L}{\partial y}}\right)\mathbf {k}
      \right]\cdot \mathbf {k} =\left({\frac {\partial M}{\partial x}}-{\frac
      {\partial L}{\partial y}}\right).]
Thus we get the right side of Green's theorem
          &#x222C;  S   &#x2207; &#x00D7;  F  &#x22C5;    n &#x005E;     d S =
      &#x222C;  D    (     &#x2202; M   &#x2202; x    &#x2212;    &#x2202; L
      &#x2202; y     )   d A .   {\displaystyle \iint _{S}\nabla \times \mathbf
      {F} \cdot \mathbf {\hat {n}} \,dS=\iint _{D}\left({\frac {\partial M}
      {\partial x}}-{\frac {\partial L}{\partial y}}\right)\,dA.}  [\iint _
      {S}\nabla \times \mathbf {F} \cdot \mathbf {\hat {n}} \,dS=\iint _
      {D}\left({\frac {\partial M}{\partial x}}-{\frac {\partial L}{\partial
      y}}\right)\,dA.]
Green's theorem is also a straightforward result of the general Stokes' theorem
using differential_forms and exterior_derivatives:
                  &#x222E;       C   &#x2061; L  d x + M  d y =     &#x222E;
      &#x2202; D   &#x2061; &#x03C9; =  &#x222B;  D    d &#x03C9;     =
      &#x222B;  D      &#x2202; L   &#x2202; y     d y &#x2227;  d x +
      &#x2202; M   &#x2202; x     d x &#x2227;  d y =  &#x222C;  D
      (     &#x2202; M   &#x2202; x    &#x2212;    &#x2202; L   &#x2202; y
      )   d x  d y .       {\displaystyle {\begin{aligned}&\oint _
      {C}L\,dx+M\,dy=\oint _{\partial D}\omega =\int _{D}\,d\omega \\[5pt]=
      {}&\int _{D}{\frac {\partial L}{\partial y}}\,dy\wedge \,dx+{\frac
      {\partial M}{\partial x}}\,dx\wedge \,dy=\iint _{D}\left({\frac {\partial
      M}{\partial x}}-{\frac {\partial L}{\partial y}}\right)\,dx\,dy.\end
      {aligned}}}  [{\displaystyle {\begin{aligned}&\oint _{C}L\,dx+M\,dy=\oint
      _{\partial D}\omega =\int _{D}\,d\omega \\[5pt]={}&\int _{D}{\frac
      {\partial L}{\partial y}}\,dy\wedge \,dx+{\frac {\partial M}{\partial
      x}}\,dx\wedge \,dy=\iint _{D}\left({\frac {\partial M}{\partial x}}-
      {\frac {\partial L}{\partial y}}\right)\,dx\,dy.\end{aligned}}}]
***** Relationship to the divergence theorem[edit] *****
Considering only two-dimensional vector fields, Green's theorem is equivalent
to the two-dimensional version of the divergence_theorem:
          &#x222D;  V    (   &#x2207;  &#x22C5;  F   )   d V =   {\displaystyle
      \iiint _{V}\left(\mathbf {\nabla } \cdot \mathbf {F} \right)\,dV=}
      [\iiint _{V}\left(\mathbf {\nabla } \cdot \mathbf {F} \right)\,dV=]
      [\oiint]    &#x2202;  V    {\displaystyle \partial \scriptstyle V}  [
      {\displaystyle \partial \scriptstyle V}]     (  F  &#x22C5;    n &#x005E;
      )  d S .   {\displaystyle (\mathbf {F} \cdot \mathbf {\hat {n}} )\,dS.}
      [{\displaystyle (\mathbf {F} \cdot \mathbf {\hat {n}} )\,dS.}]
where     &#x2207; &#x22C5;  F    {\displaystyle \nabla \cdot \mathbf {F} }
[\nabla \cdot \mathbf {F} ] is the divergence on the two-dimensional vector
field      F    {\displaystyle \mathbf {F} }  [\mathbf {F} ], and        n
&#x005E;      {\displaystyle \mathbf {\hat {n}} }  [\mathbf {\hat {n}} ] is the
outward-pointing unit normal vector on the boundary.
To see this, consider the unit normal        n &#x005E;      {\displaystyle
\mathbf {\hat {n}} }  [\mathbf {\hat {n}} ] in the right side of the equation.
Since in Green's theorem     d  r  = ( d x , d y )   {\displaystyle d\mathbf
{r} =(dx,dy)}  [d\mathbf {r} =(dx,dy)] is a vector pointing tangential along
the curve, and the curve C is the positively oriented (i.e. anticlockwise)
curve along the boundary, an outward normal would be a vector which points 90Â°
to the right of this; one choice would be     ( d y , &#x2212; d x )
{\displaystyle (dy,-dx)}  [(dy,-dx)]. The length of this vector is       d  x
2   + d  y  2     = d s .   {\displaystyle {\sqrt {dx^{2}+dy^{2}}}=ds.}  [
{\sqrt {dx^{2}+dy^{2}}}=ds.] So     ( d y , &#x2212; d x ) =    n &#x005E;
d s .   {\displaystyle (dy,-dx)=\mathbf {\hat {n}} \,ds.}  [(dy,-dx)=\mathbf
{\hat {n}} \,ds.]
Start with the left side of Green's theorem:
             &#x222E;       C   &#x2061; ( L  d x + M  d y ) =     &#x222E;
      C   &#x2061; ( M , &#x2212; L ) &#x22C5; ( d y , &#x2212; d x ) =
      &#x222E;       C   &#x2061; ( M , &#x2212; L ) &#x22C5;    n &#x005E;
      d s .   {\displaystyle \oint _{C}(L\,dx+M\,dy)=\oint _{C}(M,-L)\cdot
      (dy,-dx)=\oint _{C}(M,-L)\cdot \mathbf {\hat {n}} \,ds.}  [{\displaystyle
      \oint _{C}(L\,dx+M\,dy)=\oint _{C}(M,-L)\cdot (dy,-dx)=\oint _{C}(M,-
      L)\cdot \mathbf {\hat {n}} \,ds.}]
Applying the two-dimensional divergence theorem with      F  = ( M , &#x2212; L
)   {\displaystyle \mathbf {F} =(M,-L)}  [\mathbf {F} =(M,-L)], we get the
right side of Green's theorem:
             &#x222E;       C   &#x2061; ( M , &#x2212; L ) &#x22C5;    n
      &#x005E;     d s =  &#x222C;  D    (  &#x2207; &#x22C5; ( M , &#x2212; L
      )  )   d A =  &#x222C;  D    (     &#x2202; M   &#x2202; x    &#x2212;
      &#x2202; L   &#x2202; y     )   d A .   {\displaystyle \oint _{C}(M,-
      L)\cdot \mathbf {\hat {n}} \,ds=\iint _{D}\left(\nabla \cdot (M,-
      L)\right)\,dA=\iint _{D}\left({\frac {\partial M}{\partial x}}-{\frac
      {\partial L}{\partial y}}\right)\,dA.}  [{\displaystyle \oint _{C}(M,-
      L)\cdot \mathbf {\hat {n}} \,ds=\iint _{D}\left(\nabla \cdot (M,-
      L)\right)\,dA=\iint _{D}\left({\frac {\partial M}{\partial x}}-{\frac
      {\partial L}{\partial y}}\right)\,dA.}]
***** Area calculation[edit] *****
Green's theorem can be used to compute area by line integral.[4] The area of a
planar region     D   {\displaystyle D}  [D] is given by
         A =  &#x222C;  D   d A .   {\displaystyle A=\iint _{D}dA.}  [
      {\displaystyle A=\iint _{D}dA.}]
Choose     L   {\displaystyle L}  [L] and     M   {\displaystyle M}  [M] such
that        &#x2202; M   &#x2202; x    &#x2212;    &#x2202; L   &#x2202; y    =
1   {\displaystyle {\frac {\partial M}{\partial x}}-{\frac {\partial L}
{\partial y}}=1}  [{\frac {\partial M}{\partial x}}-{\frac {\partial L}
{\partial y}}=1], the area is given by
         A =     &#x222E;       C   &#x2061; ( L  d x + M  d y ) .
      {\displaystyle A=\oint _{C}(L\,dx+M\,dy).}  [A = \oint_{C} (L\, dx + M\,
      dy).]
Possible formulas for the area of     D   {\displaystyle D}  [D] include[4]
         A =     &#x222E;       C   &#x2061; x  d y = &#x2212;     &#x222E;
      C   &#x2061; y  d x =    1 2        &#x222E;       C   &#x2061;
      ( &#x2212; y  d x + x  d y ) .   {\displaystyle A=\oint _{C}x\,dy=-\oint
      _{C}y\,dx={\tfrac {1}{2}}\oint _{C}(-y\,dx+x\,dy).}  [{\displaystyle
      A=\oint _{C}x\,dy=-\oint _{C}y\,dx={\tfrac {1}{2}}\oint _{C}(-
      y\,dx+x\,dy).}]
***** See also[edit] *****
    * Planimeter
    * Method_of_image_charges â A method used in electrostatics that takes
      advantage of the uniqueness theorem (derived from Green's theorem)
    * Shoelace_formula â A special case of Green's theorem for simple
      polygons
***** References[edit] *****
   1. ^ George Green, An Essay on the Application of Mathematical Analysis to
      the Theories of Electricity and Magnetism (Nottingham, England: T.
      Wheelhouse, 1828). Green did not actually derive the form of "Green's
      theorem" which appears in this article; rather, he derived a form of the
      "divergence theorem", which appears on pages_10â12 of his Essay.
      In 1846, the form of "Green's theorem" which appears in this article was
      first published, without proof, in an article by Augustin_Cauchy: A.
      Cauchy (1846) "Sur_les_intÃ©grales_qui_s'Ã©tendent_Ã _tous_les_points
      d'une_courbe_fermÃ©e" (On integrals that extend over all of the points of
      a closed curve), Comptes rendus, 23: 251â255. (The equation appears at
      the bottom of page 254, where (S) denotes the line integral of a function
      k along the curve s that encloses the area S.)
      A proof of the theorem was finally provided in 1851 by Bernhard_Riemann
      in his inaugural dissertation: Bernhard Riemann (1851) Grundlagen_fÃ¼r
      eine_allgemeine_Theorie_der_Functionen_einer_verÃ¤nderlichen_complexen
      GrÃ¶sse (Basis for a general theory of functions of a variable complex
      quantity), (GÃ¶ttingen, (Germany): Adalbert Rente, 1867); see pages
      8â9.
   2. ^Riley, K. F.; Hobson, M. P.; Bence, S. J. (2010). Mathematical Methods
      for Physics and Engineering. Cambridge University Press. ISBN 978-0-521-
      86153-3.
   3. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   4. ^Spiegel, M. R.; Lipschutz, S.; Spellman, D. (2009). Vector Analysis.
      Schaumâs Outlines (2nd ed.). McGraw Hill. ISBN 978-0-07-161545-7.
   5. ^ a bStewart, James. Calculus (6th ed.). Thomson, Brooks/Cole.
***** Further reading[edit] *****
    * Marsden, Jerrold E.; Tromba, Anthony J. (2003). "The_Integral_Theorems_of
      Vector_Analysis". Vector Calculus (Fifth ed.). New York: Freeman.
      pp. 518â608. ISBN 0-7167-4992-0.
***** External links[edit] *****
    * Green's_Theorem_on_MathWorld

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Green%27s_theorem&oldid=907090550"
Categories:
    * Theorems_in_calculus
Hidden categories:
    * Articles_containing_proofs
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
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * LietuviÅ³
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * áá¶áá¶ááááá
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 20 July 2019, at 12:22 (UTC).
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
