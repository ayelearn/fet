The following text has been accessed from https://en.wikipedia.org/wiki/Uniform_boundedness_principle at Fri Aug 9 02:38:40 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Uniform boundedness principle ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, the uniform boundedness principle or BanachâSteinhaus theorem
is one of the fundamental results in functional_analysis. Together with the
HahnâBanach_theorem and the open_mapping_theorem, it is considered one of the
cornerstones of the field. In its basic form, it asserts that for a family of
continuous_linear_operators (and thus bounded operators) whose domain is a
Banach_space, pointwise boundedness is equivalent to uniform boundedness in
operator norm.
The theorem was first published in 1927 by Stefan_Banach and Hugo_Steinhaus but
it was also proven independently by Hans_Hahn.
⁰
***** Contents *****
    * 1_Theorem
    * 2_Proof
    * 3_Corollaries
    * 4_Example:_pointwise_convergence_of_Fourier_series
    * 5_Generalisations
    * 6_See_also
    * 7_References
***** Theorem[edit] *****
Theorem (Uniform Boundedness Principle). Let X be a Banach_space and Y a normed
vector_space. Suppose that F is a collection of continuous linear operators
from X to Y. If for all x in X one has
          sup  T &#x2208; F   &#x2016; T ( x )  &#x2016;  Y   < &#x221E; ,
      {\displaystyle \sup \nolimits _{T\in F}\|T(x)\|_{Y}<\infty ,}
      [\sup\nolimits_{T \in F} \|T(x)\|_Y  < \infty, ]
then
          sup  T &#x2208; F , &#x2016; x &#x2016; = 1   &#x2016; T ( x )
      &#x2016;  Y   =  sup  T &#x2208; F   &#x2016; T  &#x2016;  B ( X , Y )
      < &#x221E; .   {\displaystyle \sup \nolimits _{T\in F,\|x\|=1}\|T(x)\|_
      {Y}=\sup \nolimits _{T\in F}\|T\|_{B(X,Y)}<\infty .}  [\sup \nolimits _{
      {T\in F,\|x\|=1}}\|T(x)\|_{Y}=\sup \nolimits _{{T\in F}}\|T\|_{{B
      (X,Y)}}<\infty .]
***** Proof[edit] *****
The completeness of X enables the following short proof, using the Baire
category_theorem.
Proof. Suppose that for every x in the Banach space X, one has:
          sup  T &#x2208; F   &#x2016; T ( x )  &#x2016;  Y   < &#x221E; .
      {\displaystyle \sup \nolimits _{T\in F}\|T(x)\|_{Y}<\infty .}
      [\sup\nolimits_{T \in F} \|T (x)\|_Y  < \infty.]
For every integer     n &#x2208;  N    {\displaystyle n\in \mathbb {N} }  [n\in
\mathbb {N} ], let
          X  n   =  {  x &#x2208; X &#xA0; : &#xA0;  sup  T &#x2208; F
      &#x2016; T ( x )  &#x2016;  Y   &#x2264; n  }  .   {\displaystyle X_
      {n}=\left\{x\in X\ :\ \sup \nolimits _{T\in F}\|T(x)\|_{Y}\leq
      n\right\}.}  [ X_n = \left  \{x \in X \ : \ \sup\nolimits_{T \in F} \|T
      (x)\|_Y \le n \right \}. ]
The set      X  n     {\displaystyle X_{n}}  [X_{n}] is a closed_set and by the
assumption,
          &#x22C3;  n &#x2208;  N     X  n   = X &#x2260; &#x2205; .
      {\displaystyle \bigcup \nolimits _{n\in \mathbf {N} }X_{n}=X\neq
      \varnothing .}  [\bigcup\nolimits_{n \in \mathbf{N}} X_n = X \neq
      \varnothing.]
By the Baire_category_theorem for the non-empty complete_metric_space X, there
exists m such that      X  m     {\displaystyle X_{m}}  [ X_m] has non-empty
interior, i.e., there exist      x  0   &#x2208;  X  m     {\displaystyle x_
{0}\in X_{m}}  [x_0 \in X_m] and Îµ > 0 such that
             B  &#x03B5;   (  x  0   )  &#x00AF;   := { x &#x2208; X  :
      &#x2016; x &#x2212;  x  0   &#x2016; &#x2264; &#x03B5; } &#x2286;  X  m
      .   {\displaystyle {\overline {B_{\varepsilon }(x_{0})}}:=\{x\in X\,:
      \,\|x-x_{0}\|\leq \varepsilon \}\subseteq X_{m}.}  [ \overline
      {B_\varepsilon (x_0)} := \{x \in X \,:\, \|x - x_0\| \le \varepsilon \}
      \subseteq  X_m.]
Let u â X with ÇuÇ ≤ 1 and T â F. One has that:
             &#x2016; T ( u )  &#x2016;  Y      =  &#x03B5;  &#x2212; 1
      &#x2016;  T  (   x  0   + &#x03B5; u  )  &#x2212; T (  x  0   )  &#x2016;
      Y     [  by linearity of&#xA0;  T ]       &#x2264;  &#x03B5;  &#x2212; 1
      (    &#x2016;  T (  x  0   + &#x03B5; u )  &#x2016;   Y   +   &#x2016;  T
      (  x  0   )  &#x2016;   Y    )        &#x2264;  &#x03B5;  &#x2212; 1
      ( m + m ) .   [  since  &#xA0;  x  0   + &#x03B5; u , &#xA0;  x  0
      &#x2208;  X  m   ]       {\displaystyle {\begin{aligned}\|T(u)\|_
      {Y}&=\varepsilon ^{-1}\left\|T\left(x_{0}+\varepsilon u\right)-T(x_
      {0})\right\|_{Y}&[{\text{by linearity of }}T]\\&\leq \varepsilon ^{-
      1}\left(\left\|T(x_{0}+\varepsilon u)\right\|_{Y}+\left\|T(x_
      {0})\right\|_{Y}\right)\\&\leq \varepsilon ^{-1}(m+m).&[{\text{since}}\
      x_{0}+\varepsilon u,\ x_{0}\in X_{m}]\\\end{aligned}}}  [\begin{align}
      \|T(u) \|_Y &= \varepsilon^{-1} \left \|T \left( x_0 + \varepsilon u
      \right) - T(x_0) \right \|_Y    & [\text{by linearity of } T ] \\
      &\leq \varepsilon^{-1} \left ( \left\| T (x_0 + \varepsilon u) \right\|_Y
      + \left\| T (x_0) \right\|_Y \right ) \\
      &\leq \varepsilon^{-1} (m + m).   & [ \text{since} \ x_0 + \varepsilon u,
      \ x_0 \in X_m ] \\
      \end{align}]
Taking the supremum over u in the unit ball of X and over     T &#x2208; F
{\displaystyle T\in F}  [{\displaystyle T\in F}], it follows that
          sup  T &#x2208; F   &#x2016; T  &#x2016;  B ( X , Y )   &#x2264; 2
      &#x03B5;  &#x2212; 1   m < &#x221E; .   {\displaystyle \sup \nolimits _
      {T\in F}\|T\|_{B(X,Y)}\leq 2\varepsilon ^{-1}m<\infty .}
      [ \sup\nolimits_{T \in F} \|T\|_{B(X,Y)}  \leq 2 \varepsilon^{-1} m <
      \infty.]
There are also simple proofs not using the Baire theorem (Sokal_2011).
***** Corollaries[edit] *****
Corollary. If a sequence of bounded operators (Tn) converges pointwise, that
is, the limit of {Tn(x)} exists for all x in X, then these pointwise limits
define a bounded operator T.
Note it is not claimed above that Tn converges to T in operator norm, i.e.
uniformly on bounded sets. (However, since {Tn} is bounded in operator norm,
and the limit operator T is continuous, a standard "3-Îµ"_estimate shows that
Tn converges to T uniformly on compact sets.)
Corollary. Any weakly bounded subset S in a normed space Y is bounded.
Indeed, the elements of S define a pointwise bounded family of continuous
linear forms on the Banach space X = Y*, continuous dual of Y. By the uniform
boundedness principle, the norms of elements of S, as functionals on X, that
is, norms in the second dual Y**, are bounded. But for every s in S, the norm
in the second dual coincides with the norm in Y, by a consequence of the
HahnâBanach_theorem.
Let L(X, Y) denote the continuous operators from X to Y, with the operator
norm. If the collection F is unbounded in L(X, Y), then by the uniform
boundedness principle, we have:
         R =  {  x &#x2208; X &#xA0; : &#xA0;  sup  T &#x2208; F   &#x2016; T x
      &#x2016;  Y   = &#x221E;  }  &#x2260; &#x2205;   {\displaystyle R=\left\
      {x\in X\ :\ \sup \nolimits _{T\in F}\|Tx\|_{Y}=\infty \right\}\neq
      \varnothing }  [ R = \left \{ x \in X  \ : \ \sup\nolimits_{T \in F}
      \|Tx\|_Y = \infty \right \} \neq \varnothing]
In fact, R is dense in X. The complement of R in X is the countable union of
closed sets ∪Xn. By the argument used in proving the theorem, each Xn is
nowhere_dense, i.e. the subset ∪Xn is of first category. Therefore R is the
complement of a subset of first category in a Baire space. By definition of a
Baire space, such sets (called residual sets) are dense. Such reasoning leads
to the principle of condensation of singularities, which can be formulated as
follows:
Theorem. Let X be a Banach space, {Yn} a sequence of normed vector spaces, and
Fn a unbounded family in L(X, Yn). Then the set
         R =  {  x &#x2208; X &#xA0; : &#xA0; &#x2200; n &#x2208;  N  :  sup  T
      &#x2208;  F  n     &#x2016; T x  &#x2016;   Y  n     = &#x221E;  }
      {\displaystyle R=\left\{x\in X\ :\ \forall n\in \mathbf {N} :\sup
      \nolimits _{T\in F_{n}}\|Tx\|_{Y_{n}}=\infty \right\}}  [ R = \left \{ x
      \in X \ : \ \forall n \in \mathbf{N} : \sup\nolimits_{T \in F_n} \|Tx\|_
      {Y_n} = \infty \right \}]
is of second category, and thus dense in X.
Proof. The complement of R is the countable union
          &#x22C3;  n , m    {  x &#x2208; X &#xA0; : &#xA0;  sup  T &#x2208;
      F  n     &#x2016; T x  &#x2016;   Y  n     &#x2264; m  }
      {\displaystyle \bigcup \nolimits _{n,m}\left\{x\in X\ :\ \sup \nolimits _
      {T\in F_{n}}\|Tx\|_{Y_{n}}\leq m\right\}}  [\bigcup\nolimits_{n,m} \left
      \{ x \in X \ : \ \sup\nolimits_{T \in F_n} \|Tx\|_{Y_n} \le m \right \}]
of sets of first category. Therefore its residual set R is dense.
***** Example: pointwise convergence of Fourier series[edit] *****
Let      T    {\displaystyle \mathbb {T} }  [\mathbb {T} ] be the circle, and
let     C (  T  )   {\displaystyle C(\mathbb {T} )}  [C(\mathbb{T})] be the
Banach space of continuous functions on      T    {\displaystyle \mathbb {T} }
[\mathbb {T} ], with the uniform_norm. Using the uniform boundedness principle,
one can show that there exists an element in     C (  T  )   {\displaystyle C
(\mathbb {T} )}  [C(\mathbb{T})] for which the Fourier series does not converge
pointwise.
For     f &#x2208; C (  T  )   {\displaystyle f\in C(\mathbb {T} )}  [f \in C
(\mathbb{T})], its Fourier_series is defined by
          &#x2211;  k &#x2208;  Z       f &#x005E;    ( k )  e  i k x   =
      &#x2211;  k &#x2208;  Z      1  2 &#x03C0;     (   &#x222B;  0   2
      &#x03C0;   f ( t )  e  &#x2212; i k t   d t  )   e  i k x   ,
      {\displaystyle \sum _{k\in \mathbf {Z} }{\hat {f}}(k)e^{ikx}=\sum _{k\in
      \mathbf {Z} }{\frac {1}{2\pi }}\left(\int _{0}^{2\pi }f(t)e^{-
      ikt}dt\right)e^{ikx},}  [\sum_{k \in \mathbf{Z}} \hat{f}(k) e^{ikx} =
      \sum_{k \in \mathbf{Z}}\frac{1}{2\pi} \left (\int_0 ^{2 \pi} f(t) e^{-
      ikt} dt \right) e^{ikx},]
and the N-th symmetric partial sum is
          S  N   ( f ) ( x ) =  &#x2211;  k = &#x2212; N   N      f &#x005E;
      ( k )  e  i k x   =   1  2 &#x03C0;     &#x222B;  0   2 &#x03C0;   f ( t
      )  D  N   ( x &#x2212; t )  d t ,   {\displaystyle S_{N}(f)(x)=\sum _{k=-
      N}^{N}{\hat {f}}(k)e^{ikx}={\frac {1}{2\pi }}\int _{0}^{2\pi }f(t)D_{N}
      (x-t)\,dt,}  [ S_N(f)(x) = \sum_{k=-N}^N \hat{f}(k) e^{ikx} =  \frac{1}{2
      \pi} \int_0 ^{2 \pi} f(t) D_N(x - t) \, dt,]
where DN is the N-th Dirichlet_kernel. Fix     x &#x2208;  T    {\displaystyle
x\in \mathbb {T} }  [x \in \mathbb{T}] and consider the convergence of {SN(f)
(x)}. The functional ÏN,x :     C (  T  ) &#x2192;  C    {\displaystyle C
(\mathbb {T} )\rightarrow \mathbb {C} }  [C(\mathbb{T})\rightarrow \mathbb{C}]
defined by
          &#x03C6;  N , x   ( f ) =  S  N   ( f ) ( x ) ,  f &#x2208; C (  T  )
      ,   {\displaystyle \varphi _{N,x}(f)=S_{N}(f)(x),\qquad f\in C(\mathbb
      {T} ),}  [\varphi_{N, x} (f) =  S_N(f)(x), \qquad f \in C(\mathbb{T}),]
is bounded. The norm of ÏN,x, in the dual of     C (  T  )   {\displaystyle C
(\mathbb {T} )}  [C(\mathbb{T})], is the norm of the signed measure (2Ï)â1DN
(xât) dt, namely
          &#x2016;  &#x03C6;  N , x   &#x2016;  =   1  2 &#x03C0;     &#x222B;
      0   2 &#x03C0;    |   D  N   ( x &#x2212; t )  |   d t =   1  2 &#x03C0;
      &#x222B;  0   2 &#x03C0;    |   D  N   ( s )  |   d s =   &#x2016;  D  N
      &#x2016;    L  1   (  T  )   .   {\displaystyle \left\|\varphi _
      {N,x}\right\|={\frac {1}{2\pi }}\int _{0}^{2\pi }\left|D_{N}(x-
      t)\right|\,dt={\frac {1}{2\pi }}\int _{0}^{2\pi }\left|D_{N}
      (s)\right|\,ds=\left\|D_{N}\right\|_{L^{1}(\mathbb {T} )}.}
      [\left\|\varphi _{{N,x}}\right\|={\frac  {1}{2\pi }}\int _{0}^{{2\pi
      }}\left|D_{N}(x-t)\right|\,dt={\frac  {1}{2\pi }}\int _{0}^{{2\pi
      }}\left|D_{N}(s)\right|\,ds=\left\|D_{N}\right\|_{{L^{1}({\mathbb
      {T}})}}.]
One can verify that
           1  2 &#x03C0;     &#x222B;  0   2 &#x03C0;    |   D  N   ( t )  |
      d t &#x2265;   1  2 &#x03C0;     &#x222B;  0   2 &#x03C0;      |  sin
      &#x2061;  (  ( N +    1 2    ) t  )   |   t  /  2     d t &#x2192;
      &#x221E; .   {\displaystyle {\frac {1}{2\pi }}\int _{0}^{2\pi }|D_{N}
      (t)|\,dt\geq {\frac {1}{2\pi }}\int _{0}^{2\pi }{\frac {\left|\sin \left(
      (N+{\tfrac {1}{2}})t\right)\right|}{t/2}}\,dt\to \infty .}  [
      {\displaystyle {\frac {1}{2\pi }}\int _{0}^{2\pi }|D_{N}(t)|\,dt\geq
      {\frac {1}{2\pi }}\int _{0}^{2\pi }{\frac {\left|\sin \left((N+{\tfrac
      {1}{2}})t\right)\right|}{t/2}}\,dt\to \infty .}]
So the collection {ÏN,x} is unbounded in     C (  T   )  &#x2217;
{\displaystyle C(\mathbb {T} )^{\ast }}  [C(\mathbb{T})^\ast], the dual of
C (  T  )   {\displaystyle C(\mathbb {T} )}  [C(\mathbb{T})]. Therefore by the
uniform boundedness principle, for any     x &#x2208;  T    {\displaystyle x\in
\mathbb {T} }  [x \in \mathbb{T}], the set of continuous functions whose
Fourier series diverges at x is dense in     C (  T  )   {\displaystyle C
(\mathbb {T} )}  [C(\mathbb{T})].
More can be concluded by applying the principle of condensation of
singularities. Let {xm} be a dense sequence in      T    {\displaystyle \mathbb
{T} }  [\mathbb {T} ]. Define ÏN,xm in the similar way as above. The principle
of condensation of singularities then says that the set of continuous functions
whose Fourier series diverges at each xm is dense in     C (  T  )
{\displaystyle C(\mathbb {T} )}  [C(\mathbb{T})] (however, the Fourier series
of a continuous function f converges to f(x) for almost every     x &#x2208;  T
{\displaystyle x\in \mathbb {T} }  [x \in \mathbb{T}], by Carleson's_theorem).
***** Generalisations[edit] *****
The least restrictive setting for the uniform boundedness principle is a
barrelled_space where the following generalised version of the theorem holds
(Bourbaki_1987, Theorem III.2.1):
Theorem. Given a barrelled space X and a locally_convex_space Y, then any
family of pointwise bounded continuous_linear_mappings from X to Y is
equicontinuous (even uniformly_equicontinuous).
Alternatively, the statement also holds whenever X is a Baire_space and Y is a
locally convex space (Shtern_2001).
DieudonnÃ©_(1970) proves a weaker form of this theorem with FrÃ©chet_spaces
rather than the usual Banach spaces. Specifically,
Theorem. Let X be a FrÃ©chet space, Y a normed space, and H a set of continuous
linear mappings of X into Y. If for every x in X
          sup  u &#x2208; H   &#x2016; u ( x ) &#x2016; < &#x221E; ,
      {\displaystyle \sup \nolimits _{u\in H}\|u(x)\|<\infty ,}
      [\sup\nolimits_{u\in H}\|u(x)\|<\infty,]
then the family H is equicontinuous.
***** See also[edit] *****
    * Barrelled_space, a topological_vector_space with minimum requirements for
      the BanachâSteinhaus theorem to hold
***** References[edit] *****
    * Banach,_Stefan; Steinhaus,_Hugo (1927), "Sur_le_principe_de_la
      condensation_de_singularitÃ©s" (PDF), Fundamenta_Mathematicae, 9: 50â61
. (in French)
Bourbaki,_Nicolas (1987), Topological vector spaces, Elements of mathematics,
Springer, ISBN 978-3-540-42338-6
DieudonnÃ©,_Jean (1970), Treatise on analysis, Volume 2, Academic Press
.
Rudin,_Walter (1966), Real and complex analysis, McGraw-Hill
.
Shtern, A.I. (2001) [1994], "b/b015200", in Hazewinkel,_Michiel (ed.),
Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. / Kluwer
Academic Publishers, ISBN 978-1-55608-010-4
.
Sokal,_Alan (2011), "A really simple elementary proof of the uniform
boundedness theorem", Amer. Math. Monthly, 118: 450â452, arXiv:1005.1585,
doi:10.4169/amer.math.monthly.118.05.450
.
    * v
    * t
    * e
Functional_analysis (topics)
                       * Asplund
                       * Banach (list)
                       * Banach_Lattice
                       * Barrelled
                       * Bornological
                       * Brauner
                       * F-space
                       * Finite-dimensional
                       * FrÃ©chet (tame)
                       * Hilbert (pre-Hilbert
                       * Polarization_identity)
                       * LF-space
TVS types              * Locally_convex (Seminorms/Minkowski_functionals)
                       * Mackey
                       * Montel
                       * Nuclear
                       * Normed (norm)
                       * Quasinormed
                       * Reflexive
                       * Riesz
                       * Smith
                       * Stereotype
                       * Strictly_convex
                       * Webbed
                       * Topological_tensor_product (of_Hilbert_spaces)
                       * Dual
                       * Dual_space (Dual_norm)
                       * Operator
                       * Ultraweak
                       * Weak (polar
Mapping topologies     * operator)
                       * Mackey
                       * Strong (polar
                       * operator)
                       * Ultrastrong
                       * Uniform_convergence
                       * Adjoint
                       * Bilinear (form
                       * operator
                       * sesquilinear)
                       * (Un)Bounded
                       * Closed
                       * Compact (on_Hilbert_spaces)
                       * (Dis)Continuous
                       * Densely_defined
Linear_operators       * Fredholm
                       * HilbertâSchmidt
                       * Functionals (positive)
                       * Normal
                       * Nuclear
                       * Self-adjoint
                       * Strictly_singular
                       * Trace_class
                       * Transpose
                       * Unitary
                       * Banach_algebras
                       * C*-algebras
                       * Spectrum (C*-algebra
Operator_theory        * radius)
                       * Spectral_theory (of_ODEs
                       * Spectral_theorem)
                       * Polar_decomposition
                       * Singular_value_decomposition
                       * BanachâAlaoglu
                       * BanachâMazur
                       * BanachâSaks
                       * BanachâSchauder_(open_mapping)
                       * BanachâSteinhaus (Uniform boundedness)
                       * Bessel's_inequality
                       * CauchyâSchwarz_inequality
                       * Closed_graph
                       * Closed_range
                       * EberleinâÅ mulian
                       * Freudenthal_spectral
Theorems               * GelfandâMazur
                       * GelfandâNaimark
                       * Goldstine
                       * HahnâBanach (hyperplane_separation)
                       * Kakutani_fixed-point
                       * KreinâMilman
                       * Lomonosov's_invariant_subspace
                       * MackeyâArens
                       * Mazur's_lemma
                       * M._Riesz_extension
                       * Riesz_representation
                       * Parseval's_identity
                       * Schauder_fixed-point
                       * Abstract_Wiener_space
                       * Bochner_space
                       * Differentiation_in_FrÃ©chet_spaces
                       * Derivatives (FrÃ©chet
                       * Gateaux
                       * functional
                       * holomorphic)
                       * Integrals (Bochner
                       * Dunford
                       * GelfandâPettis
Analysis               * regulated
                       * PaleyâWiener
                       * weak)
                       * Functional_calculus (Borel
                       * continuous
                       * holomorphic)
                       * Inverse_function_theorem (NashâMoser_theorem)
                       * Measures (Lebesgue
                       * Projection-valued
                       * Vector)
                       * Weakly_measurable_function
                       * Absolutely_convex
                       * Absorbing
                       * Balanced
                       * Bounded
                       * Convex
Types of sets          * Convex_cone_(subset)
                       * Linear_cone_(subset)
                       * Radial
                       * Star-shaped
                       * Symmetric
                       * Zonotope
                       * Algebraic_interior_(core)
                       * Bounding_points
Subsets / set         * Convex_hull
operations             * Extreme_point
                       * Interior
                       * Minkowski_addition
                       * Polar

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Uniform_boundedness_principle&oldid=900771239"
Categories:
    * Functional_analysis
    * Mathematical_principles
    * Theorems_in_functional_analysis
Hidden categories:
    * Articles_with_French-language_external_links
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * ÄeÅ¡tina
    * Deutsch
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Sicilianu
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
Edit_links
    * This page was last edited on 7 June 2019, at 13:54 (UTC).
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
