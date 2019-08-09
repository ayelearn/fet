The following text has been accessed from https://en.wikipedia.org/wiki/Banach_space at Fri Aug 9 02:38:43 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Banach space ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, more specifically in functional_analysis, a Banach space
(pronounced [Ëbanax]) is a complete normed_vector_space. Thus, a Banach space
is a vector space with a metric that allows the computation of vector_length
and distance between vectors and is complete in the sense that a Cauchy
sequence of vectors always converges to a well defined limit that is within the
space.
Banach spaces are named after the Polish mathematician Stefan_Banach, who
introduced this concept and studied it systematically in 1920â1922 along with
Hans_Hahn and Eduard_Helly.[1] Banach spaces originally grew out of the study
of function_spaces by Hilbert, FrÃ©chet, and Riesz earlier in the century.
Banach spaces play a central role in functional analysis. In other areas of
analysis, the spaces under study are often Banach spaces.
⁰
***** Contents *****
    * 1_Definition
    * 2_General_theory
          o 2.1_Linear_operators,_isomorphisms
          o 2.2_Basic_notions
          o 2.3_Classical_spaces
          o 2.4_Banach_algebras
                # 2.4.1_Examples
          o 2.5_Dual_space
                # 2.5.1_Weak_topologies
                # 2.5.2_Examples_of_dual_spaces
                # 2.5.3_Bidual
          o 2.6_Banach's_theorems
          o 2.7_Reflexivity
          o 2.8_Weak_convergences_of_sequences
                # 2.8.1_Results_involving_the_â1_basis
                # 2.8.2_Sequences,_weak_and_weak*_compactness
    * 3_Schauder_bases
    * 4_Tensor_product
          o 4.1_Tensor_products_and_the_approximation_property
    * 5_Some_classification_results
          o 5.1_Characterizations_of_Hilbert_space_among_Banach_spaces
          o 5.2_Metric_classification
          o 5.3_Topological_classification
          o 5.4_Spaces_of_continuous_functions
    * 6_Examples
    * 7_Derivatives
    * 8_Generalizations
    * 9_See_also
    * 10_Notes
    * 11_References
    * 12_External_links
***** Definition[edit] *****
A Banach space is a vector_space X over the field R of real numbers, or over
the field C of complex numbers, which is equipped with a norm     &#x2016;
&#x22C5;  &#x2016;  X     {\displaystyle \|\cdot \|_{X}}  [{\displaystyle
\|\cdot \|_{X}}] and which is complete with respect to the distance function
induced by the norm, that is to say, for every Cauchy_sequence {xn}  in X,
there exists an element x in X such that
          lim  n &#x2192; &#x221E;    x  n   = x ,   {\displaystyle \lim _{n\to
      \infty }x_{n}=x,}  [\lim _{n\to \infty }x_{n}=x,]
or equivalently:
          lim  n &#x2192; &#x221E;     &#x2016;   x  n   &#x2212; x  &#x2016;
      X   = 0.   {\displaystyle \lim _{n\to \infty }\left\|x_{n}-x\right\|_
      {X}=0.}  [\lim _{n\to \infty }\left\|x_{n}-x\right\|_{X}=0.]
The vector space structure allows one to relate the behavior of Cauchy
sequences to that of converging series_of_vectors. A normed space X is a Banach
space if and only if each absolutely_convergent series in X converges in X,[2]
          &#x2211;  n = 1   &#x221E;   &#x2016;  v  n    &#x2016;  X   <
      &#x221E;   implies that    &#x2211;  n = 1   &#x221E;    v  n   &#xA0;
      &#xA0;  converges in  &#xA0; &#xA0; X .   {\displaystyle \sum _{n=1}^
      {\infty }\|v_{n}\|_{X}<\infty \quad {\text{implies that}}\quad \sum _
      {n=1}^{\infty }v_{n}\ \ {\text{converges in}}\ \ X.}  [\sum _{n=1}^
      {\infty }\|v_{n}\|_{X}<\infty \quad {\text{implies that}}\quad \sum _
      {n=1}^{\infty }v_{n}\ \ {\text{converges in}}\ \ X.]
Completeness of a normed space is preserved if the given norm is replaced by an
equivalent one.
All norms on a finite-dimensional vector space are equivalent. Every finite-
dimensional normed space over R or C is a Banach space.[3]
***** General theory[edit] *****
**** Linear operators, isomorphisms[edit] ****
Main article: Bounded_operator
If X and Y are normed spaces over the same ground_field K, the set of all
continuous K-linear_maps T : X â Y is denoted by B(X, Y). In infinite-
dimensional spaces, not all linear maps are continuous. A linear mapping from a
normed space X to another normed space is continuous if and only if it is
bounded on the closed unit_ball of X. Thus, the vector space B(X, Y) can be
given the operator_norm
         &#x2016; T &#x2016; = sup  {  &#x2016; T x  &#x2016;  Y   &#x2223; x
      &#x2208; X , &#xA0; &#x2016; x  &#x2016;  X   &#x2264; 1  }  .
      {\displaystyle \|T\|=\sup \left\{\|Tx\|_{Y}\mid x\in X,\ \|x\|_{X}\leq
      1\right\}.}  [\|T\|=\sup \left\{\|Tx\|_{Y}\mid x\in X,\ \|x\|_{X}\leq
      1\right\}.]
For Y a Banach space, the space B(X, Y) is a Banach space with respect to this
norm.
If X is a Banach space, the space B(X) = B(X, X) forms a unital Banach_algebra;
the multiplication operation is given by the composition of linear maps.
If X and Y are normed spaces, they are isomorphic normed spaces if there exists
a linear bijection T : X â Y such that T and its inverse T â1 are
continuous. If one of the two spaces X or Y is complete (or reflexive,
separable, etc.) then so is the other space. Two normed spaces X and Y are
isometrically isomorphic if in addition, T is an isometry, i.e., ||T(x)|| =
||x|| for every x in X. The BanachâMazur_distance d(X, Y) between two
isomorphic but not isometric spaces X and Y gives a measure of how much the two
spaces X and Y differ.
**** Basic notions[edit] ****
Every normed space X can be isometrically embedded in a Banach space. More
precisely, for every normed space X, there exist a Banach space Y and a mapping
T : X â Y such that T is an isometric_mapping and T(X) is dense in Y. If Z is
another Banach space such that there is an isometric isomorphism from X onto a
dense subset of Z, then Z is isometrically isomorphic to Y.
This Banach space Y is the completion of the normed space X. The underlying
metric space for Y is the same as the metric completion of X, with the vector
space operations extended from X to Y. The completion of X is often denoted by
X &#x005E;      {\displaystyle {\widehat {X}}}  [{\widehat {X}}].
The cartesian product X Ã Y of two normed spaces is not canonically equipped
with a norm. However, several equivalent norms are commonly used,[4] such as
         &#x2016; ( x , y )  &#x2016;  1   = &#x2016; x &#x2016; + &#x2016; y
      &#x2016; ,  &#x2016; ( x , y )  &#x2016;  &#x221E;   = max ( &#x2016; x
      &#x2016; , &#x2016; y &#x2016; )   {\displaystyle \|(x,y)\|_
      {1}=\|x\|+\|y\|,\qquad \|(x,y)\|_{\infty }=\max(\|x\|,\|y\|)}  [\|
      (x,y)\|_{1}=\|x\|+\|y\|,\qquad \|(x,y)\|_{\infty }=\max(\|x\|,\|y\|)]
and give rise to isomorphic normed spaces. In this sense, the product X Ã Y
(or the direct sum X â Y) is complete if and only if the two factors are
complete.
If M is a closed linear_subspace of a normed space X, there is a natural norm
on the quotient space Xâ/âM,
         &#x2016; x + M &#x2016; =  inf  m &#x2208; M   &#x2016; x + m &#x2016;
      .   {\displaystyle \|x+M\|=\inf \limits _{m\in M}\|x+m\|.}  [\|x+M\|=\inf
      \limits _{m\in M}\|x+m\|.]
The quotient Xâ/âM is a Banach space when X is complete.[5] The quotient
map from X onto Xâ/âM, sending x in X to its class x + M, is linear, onto
and has norm 1, except when M = X, in which case the quotient is the null
space.
The closed linear subspace M of X is said to be a complemented subspace of X if
M is the range of a bounded linear projection P from X onto M. In this case,
the space X is isomorphic to the direct sum of M and Ker(P), the kernel of the
projection P.
Suppose that X and Y are Banach spaces and that T â B(X, Y). There exists a
canonical factorization of T as[5]
         T =  T  1   &#x2218; &#x03C0; , &#xA0; &#xA0; &#xA0; T : X &#xA0;
      &#x27F6; &#x03C0;   &#xA0; X  /  Ker &#x2061; ( T ) &#xA0;   &#x27F6;  T
      1     &#xA0; Y   {\displaystyle T=T_{1}\circ \pi ,\ \ \ T:X\ {\overset
      {\pi }{\longrightarrow }}\ X/\operatorname {Ker} (T)\ {\overset {T_{1}}
      {\longrightarrow }}\ Y}  [T=T_{1}\circ \pi ,\ \ \ T:X\ {\overset {\pi }
      {\longrightarrow }}\ X/\operatorname {Ker} (T)\ {\overset {T_{1}}
      {\longrightarrow }}\ Y]
where the first map Ï is the quotient map, and the second map T1 sends every
class x + Ker(T) in the quotient to the image T(x) in Y. This is well defined
because all elements in the same class have the same image. The mapping T1 is a
linear bijection from Xâ/âKer(T) onto the range T(X), whose inverse need
not be bounded.
**** Classical spaces[edit] ****
Basic examples[6] of Banach spaces include: the Lp_spaces and their special
cases, the sequence_spaces âp that consist of scalar sequences indexed by N;
among them, the space â1 of absolutely_summable sequences and the space â2
of square summable sequences; the space c0 of sequences tending to zero and the
space ââ of bounded sequences; the space C(K) of continuous scalar
functions on a compact Hausdorff space K, equipped with the max norm,
         &#x2016; f  &#x2016;  C ( K )   = max {  |  f ( x )  |  : x &#x2208; K
      } ,  f &#x2208; C ( K ) .   {\displaystyle \|f\|_{C(K)}=\max\{|f(x)|:x\in
      K\},\quad f\in C(K).}  [\|f\|_{C(K)}=\max\{|f(x)|:x\in K\},\quad f\in C
      (K).]
According to the BanachâMazur_theorem, every Banach space is isometrically
isomorphic to a subspace of some C(K).[7] For every separable Banach space X,
there is a closed subspace M of â1 such that X â â1/M.[8]
Any Hilbert_space serves as an example of a Banach space. A Hilbert space H on
K = R, C is complete for a norm of the form
         &#x2016; x  &#x2016;  H   =   &#x27E8; x , x &#x27E9;   ,
      {\displaystyle \|x\|_{H}={\sqrt {\langle x,x\rangle }},}  [\|x\|_{H}=
      {\sqrt {\langle x,x\rangle }},]
where
         &#x27E8; &#x22C5; , &#x22C5; &#x27E9; : H &#x00D7; H &#x2192;  K
      {\displaystyle \langle \cdot ,\cdot \rangle :H\times H\to \mathbf {K} }
      [\langle \cdot ,\cdot \rangle :H\times H\to \mathbf {K} ]
is the inner_product, linear in its first argument that satisfies the
following:
             &#x2200; x , y &#x2208; H :  &#x27E8; y , x &#x27E9;    =
      &#x27E8; x , y &#x27E9;  &#x00AF;   ,     &#x2200; x &#x2208; H :
      &#x27E8; x , x &#x27E9;    &#x2265; 0 ,     &#x27E8; x , x &#x27E9; = 0
      &#x21D4; x    = 0.       {\displaystyle {\begin{aligned}\forall x,y\in H:
      \quad \langle y,x\rangle &={\overline {\langle x,y\rangle }},\\\forall
      x\in H:\quad \langle x,x\rangle &\geq 0,\\\langle x,x\rangle
      =0\Leftrightarrow x&=0.\end{aligned}}}  [{\begin{aligned}\forall x,y\in
      H:\quad \langle y,x\rangle &={\overline {\langle x,y\rangle }},\\\forall
      x\in H:\quad \langle x,x\rangle &\geq 0,\\\langle x,x\rangle
      =0\Leftrightarrow x&=0.\end{aligned}}]
For example, the space L2 is a Hilbert space.
The Hardy_spaces, the Sobolev_spaces are examples of Banach spaces that are
related to Lp spaces and have additional structure. They are important in
different branches of analysis, Harmonic_analysis and Partial_differential
equations among others.
**** Banach algebras[edit] ****
A Banach_algebra is a Banach space A over K = R or C, together with a structure
of algebra_over_K, such that the product map A Ã A â (a, b) â¦ ab â A is
continuous. An equivalent norm on A can be found so that ||ab|| â¤ ||a|| ||b||
for all a, b â A.
*** Examples[edit] ***
    * The Banach space C(K), with the pointwise product, is a Banach algebra.
    * The disk_algebra A(D) consists of functions holomorphic in the open unit
      disk D â C and continuous on its closure: D. Equipped with the max norm
      on D, the disk algebra A(D) is a closed subalgebra of C(D).
    * The Wiener_algebra A(T) is the algebra of functions on the unit circle T
      with absolutely convergent Fourier series. Via the map associating a
      function on T to the sequence of its Fourier coefficients, this algebra
      is isomorphic to the Banach algebra â1(Z), where the product is the
      convolution of sequences.
    * For every Banach space X, the space B(X) of bounded linear operators on
      X, with the composition of maps as product, is a Banach algebra.
    * A C*-algebra is a complex Banach algebra A with an antilinear involution
      a â¦ aâ such that ||aâa|| = ||a||2. The space B(H) of bounded linear
      operators on a Hilbert space H is a fundamental example of C*-algebra.
      The GelfandâNaimark_theorem states that every C*-algebra is
      isometrically isomorphic to a C*-subalgebra of some B(H). The space C(K)
      of complex continuous functions on a compact Hausdorff space K is an
      example of commutative C*-algebra, where the involution associates to
      every function  f  its complex_conjugate  f .
**** Dual space[edit] ****
Main article: Dual_space
If X is a normed space and K the underlying field (either the real or the
complex numbers), the continuous_dual_space is the space of continuous linear
maps from X into K, or continuous linear functionals. The notation for the
continuous dual is Xââ² = B(X, K) in this article.[9] Since K is a Banach
space (using the absolute_value as norm), the dual Xââ² is a Banach space,
for every normed space X.
The main tool for proving the existence of continuous linear functionals is the
HahnâBanach_theorem.
      HahnâBanach theorem. Let X be a vector_space over the field K = R, C.
      Let further
          * Y â X be a linear_subspace,
          * p : X â R be a sublinear_function and
          *  f  : Y â K be a linear_functional so that Re( f (y)) â¤ p(y)
            for all y in Y.
      Then, there exists a linear functional F : X â K so that
               F   |   Y   = f ,   and   &#x2200; x &#x2208; X , &#xA0; &#xA0;
            Re &#x2061; ( F ( x ) ) &#x2264; p ( x ) .   {\displaystyle F|_
            {Y}=f,\quad {\text{and}}\quad \forall x\in X,\ \ \operatorname {Re}
            (F(x))\leq p(x).}  [F|_{Y}=f,\quad {\text{and}}\quad \forall x\in
            X,\ \ \operatorname {Re} (F(x))\leq p(x).]
In particular, every continuous linear functional on a subspace of a normed
space can be continuously extended to the whole space, without increasing the
norm of the functional.[10] An important special case is the following: for
every vector x in a normed space X, there exists a continuous linear functional
 f  on X such that
         f ( x ) = &#x2016; x  &#x2016;  X   ,  &#x2016; f  &#x2016;   X
      &#x2032;    &#x2264; 1.   {\displaystyle f(x)=\|x\|_{X},\quad \|f\|_
      {X'}\leq 1.}  [f(x)=\|x\|_{X},\quad \|f\|_{X'}\leq 1.]
When x is not equal to the 0 vector, the functional  f  must have norm one, and
is called a norming functional for x.
The HahnâBanach_separation_theorem states that two disjoint non-empty convex
sets in a real Banach space, one of them open, can be separated by a closed
affine hyperplane. The open convex set lies strictly on one side of the
hyperplane, the second convex set lies on the other side but may touch the
hyperplane.[11]
A subset S in a Banach space X is total if the linear_span of S is dense in X.
The subset S is total in X if and only if the only continuous linear functional
that vanishes on S is the 0 functional: this equivalence follows from the
HahnâBanach theorem.
If X is the direct sum of two closed linear subspaces M and N, then the dual
Xââ² of X is isomorphic to the direct sum of the duals of M and N.[12] If M
is a closed linear subspace in X, one can associate the orthogonal of M in the
dual,
          M  &#x22A5;   =  {   x &#x2032;  &#x2208;  X &#x2032;  :  x &#x2032;
      ( m ) = 0 , &#xA0; &#x2200; m &#x2208; M  }  .   {\displaystyle M^{\perp
      }=\left\{x'\in X':x'(m)=0,\ \forall m\in M\right\}.}  [M^{\perp }=\left\
      {x'\in X':x'(m)=0,\ \forall m\in M\right\}.]
The orthogonal M â¥ is a closed linear subspace of the dual. The dual of M is
isometrically isomorphic to Xââ²â/âM â¥. The dual of Xâ/âM is
isometrically isomorphic to M â¥.[13]
The dual of a separable Banach space need not be separable, but:
      Theorem.[14] Let X be a normed space. If Xââ² is separable, then X is
      separable.
When Xââ² is separable, the above criterion for totality can be used for
proving the existence of a countable total subset in X.
*** Weak topologies[edit] ***
The weak_topology on a Banach space X is the coarsest_topology on X for which
all elements xââ² in the continuous dual space Xââ² are continuous. The
norm topology is therefore finer than the weak topology. It follows from the
HahnâBanach separation theorem that the weak topology is Hausdorff, and that
a norm-closed convex_subset of a Banach space is also weakly closed.[15] A
norm-continuous linear map between two Banach spaces X and Y is also weakly
continuous, i.e., continuous from the weak topology of X to that of Y.[16]
If X is infinite-dimensional, there exist linear maps which are not continuous.
The space Xâ of all linear maps from X to the underlying field K (this space
Xâ is called the algebraic_dual_space, to distinguish it from Xââ²) also
induces a topology on X which is finer than the weak topology, and much less
used in functional analysis.
On a dual space Xââ², there is a topology weaker than the weak topology of
Xââ², called weak*_topology. It is the coarsest topology on Xââ² for
which all evaluation maps xâ²âââXââ² â xâ²(x), xâââX, are
continuous. Its importance comes from the BanachâAlaoglu_theorem.
      BanachâAlaoglu Theorem. Let X be a normed_vector_space. Then the closed
      unit_ball Bââ² = {xâ² â Xââ² : ||xâ²|| â¤ 1}  of the dual
      space is compact in the weak* topology.
The BanachâAlaoglu theorem depends on Tychonoff's_theorem about infinite
products of compact spaces. When X is separable, the unit ball Bââ² of the
dual is a metrizable compact in the weak* topology.[17]
*** Examples of dual spaces[edit] ***
The dual of c0 is isometrically isomorphic to â1: for every bounded linear
functional âfâ on c0, there is a unique element y = {yn} â â1 such that
         f ( x ) =  &#x2211;  n &#x2208;  N     x  n    y  n   ,  x = {  x  n
      } &#x2208;  c  0   , &#xA0; &#xA0;  and  &#xA0; &#xA0; &#x2016; f
      &#x2016;  (  c  0    ) &#x2032;    = &#x2016; y  &#x2016;   &#x2113;  1
      .   {\displaystyle f(x)=\sum _{n\in \mathbf {N} }x_{n}y_{n},\qquad x=\{x_
      {n}\}\in c_{0},\ \ {\text{and}}\ \ \|f\|_{(c_{0})'}=\|y\|_{\ell _{1}}.}
      [f(x)=\sum _{n\in \mathbf {N} }x_{n}y_{n},\qquad x=\{x_{n}\}\in c_{0},\ \
      {\text{and}}\ \ \|f\|_{(c_{0})'}=\|y\|_{\ell _{1}}.]
The dual of â1 is isometrically isomorphic to ââ. The dual of Lp([0,_1])
is isometrically isomorphic to Lq([0, 1]) when 1 â¤ p < â and â1/p + 1/q =
1.
For every vector y in a Hilbert space H, the mapping
         x &#x2208; H &#x2192;  f  y   ( x ) = &#x27E8; x , y &#x27E9;
      {\displaystyle x\in H\to f_{y}(x)=\langle x,y\rangle }  [x\in H\to f_{y}
      (x)=\langle x,y\rangle ]
defines a continuous linear functional âfyâ on H. The Riesz_representation
theorem states that every continuous linear functional on H is of the form
âfyâ for a uniquely defined vector y in H. The mapping y â H â âfyâ
is an antilinear isometric bijection from H onto its dual Hââ². When the
scalars are real, this map is an isometric isomorphism.
When K is a compact Hausdorff topological space, the dual M(K) of C(K) is the
space of Radon_measures in the sense of Bourbaki.[18] The subset P(K) of M(K)
consisting of non-negative measures of mass 1 (probability_measures) is a
convex w*-closed subset of the unit ball of M(K). The extreme_points of P(K)
are the Dirac_measures on K. The set of Dirac measures on K, equipped with the
w*-topology, is homeomorphic to K.
      BanachâStone_Theorem. If K and L are compact Hausdorff spaces and if C
      (K) and C(L) are isometrically isomorphic, then the topological spaces K
      and L are homeomorphic.[19][20]
The result has been extended by Amir[21] and Cambern[22] to the case when the
multiplicative BanachâMazur_distance between C(K) and C(L) is < 2. The
theorem is no longer true when the distance is = 2.[23]
In the commutative Banach_algebra C(K), the maximal_ideals are precisely
kernels of Dirac mesures on K,
          I  x   = ker &#x2061;  &#x03B4;  x   = { f &#x2208; C ( K ) : f ( x )
      = 0 } ,  x &#x2208; K .   {\displaystyle I_{x}=\ker \delta _{x}=\{f\in C
      (K):f(x)=0\},\quad x\in K.}  [I_{x}=\ker \delta _{x}=\{f\in C(K):f
      (x)=0\},\quad x\in K.]
More generally, by the GelfandâMazur_theorem, the maximal ideals of a unital
commutative Banach algebra can be identified with its charactersânot merely
as sets but as topological spaces: the former with the hull-kernel_topology and
the latter with the w*-topology. In this identification, the maximal ideal
space can be viewed as a w*-compact subset of the unit ball in the dual
Aââ².
      Theorem. If K is a compact Hausdorff space, then the maximal ideal space
      Î of the Banach algebra C(K) is homeomorphic to K.[19]
Not every unital commutative Banach algebra is of the form C(K) for some
compact Hausdorff space K. However, this statement holds if one places C(K) in
the smaller category of commutative C*-algebras. Gelfand's representation
theorem for commutative C*-algebras states that every commutative unital C*-
algebra A is isometrically isomorphic to a C(K) space.[24] The Hausdorff
compact space K here is again the maximal ideal space, also called the spectrum
of A in the C*-algebra context.
*** Bidual[edit] ***
If X is a normed space, the (continuous) dual Xââ²â² of the dual Xââ² is
called bidual, or second dual of X. For every normed space X, there is a
natural map,
           {     F  X   : X &#x2192;  X &#x2033;       F  X   ( x ) ( f ) = f
      ( x )   &#x2200; x &#x2208; X , &#x2200; f &#x2208;  X &#x2032;
      {\displaystyle {\begin{cases}F_{X}:X\to X''\\F_{X}(x)(f)=f(x)&\forall
      x\in X,\forall f\in X'\end{cases}}}  [{\begin{cases}F_{X}:X\to X''\\F_{X}
      (x)(f)=f(x)&\forall x\in X,\forall f\in X'\end{cases}}]
This defines FX(x) as a continuous linear functional on Xââ², i.e., an
element of Xââ²â². The map FX : x â FX(x) is a linear map from X to
Xââ²â². As a consequence of the existence of a norming_functional  f  for
every x in X, this map FX is isometric, thus injective.
For example, the dual of X = c0 is identified with â1, and the dual of â1
is identified with ââ, the space of bounded scalar sequences. Under these
identifications, FX is the inclusion map from c0 to ââ. It is indeed
isometric, but not onto.
If FX is surjective, then the normed space X is called reflexive (see below).
Being the dual of a normed space, the bidual Xââ²â² is complete, therefore,
every reflexive normed space is a Banach space.
Using the isometric embedding FX, it is customary to consider a normed space X
as a subset of its bidual. When X is a Banach space, it is viewed as a closed
linear subspace of Xââ²â². If X is not reflexive, the unit ball of X is a
proper subset of the unit ball of Xââ²â². The Goldstine_theorem states that
the unit ball of a normed space is weakly*-dense in the unit ball of the
bidual. In other words, for every xââ²â² in the bidual, there exists a net
{xj}  in X so that
          sup  j   &#x2016;  x  j   &#x2016; &#x2264; &#x2016;  x &#x2033;
      &#x2016; , &#xA0; &#xA0;  x &#x2033;  ( f ) =  lim  j   f (  x  j   ) ,
      f &#x2208;  X &#x2032;  .   {\displaystyle \sup _{j}\|x_{j}\|\leq
      \|x''\|,\ \ x''(f)=\lim _{j}f(x_{j}),\quad f\in X'.}  [\sup _{j}\|x_
      {j}\|\leq \|x''\|,\ \ x''(f)=\lim _{j}f(x_{j}),\quad f\in X'.]
The net may be replaced by a weakly*-convergent sequence when the dual Xââ²
is separable. On the other hand, elements of the bidual of â1 that are not in
â1 cannot be weak*-limit of sequences in â1, since â1 is weakly
sequentially_complete.
**** Banach's theorems[edit] ****
Here are the main general results about Banach spaces that go back to the time
of Banach's book (Banach_(1932)) and are related to the Baire_category_theorem.
According to this theorem, a complete metric space (such as a Banach space, a
FrÃ©chet_space or an F-space) cannot be equal to a union of countably many
closed subsets with empty interiors. Therefore, a Banach space cannot be the
union of countably many closed subspaces, unless it is already equal to one of
them; a Banach space with a countable Hamel_basis is finite-dimensional.
      BanachâSteinhaus_Theorem. Let X be a Banach space and Y be a normed
      vector_space. Suppose that F is a collection of continuous linear
      operators from X to Y. The uniform boundedness principle states that if
      for all x in X we have supTâF ||T(x)||Y < â, then supTâF ||T||Y <
      â.
The BanachâSteinhaus theorem is not limited to Banach spaces. It can be
extended for example to the case where X is a FrÃ©chet_space, provided the
conclusion is modified as follows: under the same hypothesis, there exists a
neighborhood U of 0 in X such that all T in F are uniformly bounded on U,
          sup  T &#x2208; F    sup  x &#x2208; U    &#x2016; T ( x )  &#x2016;
      Y   < &#x221E; .   {\displaystyle \sup _{T\in F}\sup _{x\in U}\;\|T(x)\|_
      {Y}<\infty .}  [\sup _{T\in F}\sup _{x\in U}\;\|T(x)\|_{Y}<\infty .]
      The_Open_Mapping_Theorem. Let X and Y be Banach spaces and T : X â Y be
      a surjective continuous linear operator, then T is an open map.
      Corollary. Every one-to-one bounded linear operator from a Banach space
      onto a Banach space is an isomorphism.
      The First Isomorphism Theorem for Banach spaces. Suppose that X and Y are
      Banach spaces and that T â B(X, Y). Suppose further that the range of T
      is closed in Y. Then X/âKer(T) is isomorphic to T(X).
This result is a direct consequence of the preceding Banach isomorphism theorem
and of the canonical factorization of bounded linear maps.
      Corollary. If a Banach space X is the internal direct sum of closed
      subspaces M1, ..., Mn, then X is isomorphic to M1 â ... â Mn.
This is another consequence of Banach's isomorphism theorem, applied to the
continuous bijection from M1 â ... â Mn onto X sending (m1, ..., mn) to the
sum m1 + ... + mn.
      The_Closed_Graph_Theorem. Let T : X â Y be a linear mapping between
      Banach spaces. The graph of T is closed in X Ã Y if and only if T is
      continuous.
**** Reflexivity[edit] ****
Main article: Reflexive_space
The normed space X is called reflexive when the natural map
           {     F  X   : X &#x2192;  X &#x2033;       F  X   ( x ) ( f ) = f
      ( x )   &#x2200; x &#x2208; X , &#x2200; f &#x2208;  X &#x2032;
      {\displaystyle {\begin{cases}F_{X}:X\to X''\\F_{X}(x)(f)=f(x)&\forall
      x\in X,\forall f\in X'\end{cases}}}  [{\begin{cases}F_{X}:X\to X''\\F_{X}
      (x)(f)=f(x)&\forall x\in X,\forall f\in X'\end{cases}}]
is surjective. Reflexive normed spaces are Banach spaces.
      Theorem. If X is a reflexive Banach space, every closed subspace of X and
      every quotient space of X are reflexive.
This is a consequence of the HahnâBanach theorem. Further, by the open
mapping theorem, if there is a bounded linear operator from the Banach space X
onto the Banach space Y, then Y is reflexive.
      Theorem. If X is a Banach space, then X is reflexive if and only if
      Xââ² is reflexive.
      Corollary. Let X be a reflexive Banach space. Then X is separable if and
      only if Xââ² is separable.
Indeed, if the dual Yââ² of a Banach space Y is separable, then Y is
separable. If X is reflexive and separable, then the dual of Xââ² is
separable, so Xââ² is separable.
      Theorem. Suppose that X1, ..., Xn are normed spaces and that X = X1 â
      ... â Xn. Then X is reflexive if and only if each Xj is reflexive.
Hilbert spaces are reflexive. The Lp spaces are reflexive when 1 < p < â.
More generally, uniformly_convex_spaces are reflexive, by the MilmanâPettis
theorem. The spaces c0, â1, L1([0, 1]), C([0, 1]) are not reflexive. In these
examples of non-reflexive spaces X, the bidual Xââ²â² is "much larger" than
X. Namely, under the natural isometric embedding of X into Xââ²â² given by
the HahnâBanach theorem, the quotient Xââ²â²â/âX is infinite-
dimensional, and even nonseparable. However, Robert C. James has constructed an
example[25] of a non-reflexive space, usually called "the James space" and
denoted by J,[26] such that the quotient Jââ²â²â/âJ is one-dimensional.
Furthermore, this space J is isometrically isomorphic to its bidual.
      Theorem. A Banach space X is reflexive if and only if its unit ball is
      compact in the weak_topology.
When X is reflexive, it follows that all closed and bounded convex_subsets of X
are weakly compact. In a Hilbert space H, the weak compactness of the unit ball
is very often used in the following way: every bounded sequence in H has weakly
convergent subsequences.
Weak compactness of the unit ball provides a tool for finding solutions in
reflexive spaces to certain optimization_problems. For example, every convex
continuous function on the unit ball B of a reflexive space attains its minimum
at some point in B.
As a special case of the preceding result, when X is a reflexive space over R,
every continuous linear functional  f  in Xââ² attains its maximum || f ||
on the unit ball of X. The following theorem_of_Robert_C._James provides a
converse statement.
      James' Theorem. For a Banach space the following two properties are
      equivalent:
          * X is reflexive.
          * for all  f  in Xââ² there exists x in X with ||x|| â¤ 1, so
            that  f (x) = || f ||.
The theorem can be extended to give a characterization of weakly compact convex
sets.
On every non-reflexive Banach space X, there exist continuous linear
functionals that are not norm-attaining. However, the BishopâPhelps theorem
[27] states that norm-attaining functionals are norm dense in the dual Xââ²
of X.
**** Weak convergences of sequences[edit] ****
A sequence {xn}  in a Banach space X is weakly convergent to a vector x â X
if  f (xn) converges to  f (x) for every continuous linear functional  f  in
the dual Xââ². The sequence {xn}  is a weakly Cauchy sequence if  f (xn)
converges to a scalar limit L( f ), for every  f  in Xââ². A sequence { fn }
in the dual Xââ² is weakly* convergent to a functional  f  â Xââ² if
 fn (x) converges to  f (x) for every x in X. Weakly Cauchy sequences, weakly
convergent and weakly* convergent sequences are norm bounded, as a consequence
of the BanachâSteinhaus theorem.
When the sequence {xn}  in X is a weakly Cauchy sequence, the limit L above
defines a bounded linear functional on the dual Xââ², i.e., an element L of
the bidual of X, and L is the limit of {xn}  in the weak*-topology of the
bidual. The Banach space X is weakly sequentially complete if every weakly
Cauchy sequence is weakly convergent in X. It follows from the preceding
discussion that reflexive spaces are weakly sequentially complete.
      Theorem. [28] For every measure Î¼, the space L1(Î¼) is weakly
      sequentially complete.
An orthonormal sequence in a Hilbert space is a simple example of a weakly
convergent sequence, with limit equal to the 0 vector. The unit_vector_basis of
âp, 1 < p < â, or of c0, is another example of a weakly null sequence,
i.e., a sequence that converges weakly to 0. For every weakly null sequence in
a Banach space, there exists a sequence of convex combinations of vectors from
the given sequence that is norm-converging to 0.[29]
The unit vector basis of â1 is not weakly Cauchy. Weakly Cauchy sequences in
â1 are weakly convergent, since L1-spaces are weakly sequentially complete.
Actually, weakly convergent sequences in â1 are norm convergent.[30] This
means that â1 satisfies Schur's_property.
*** Results involving the â1 basis[edit] ***
Weakly Cauchy sequences and the â1 basis are the opposite cases of the
dichotomy established in the following deep result of H. P. Rosenthal.[31]
      Theorem.[32] Let {xn}  be a bounded sequence in a Banach space. Either
      {xn}  has a weakly Cauchy subsequence, or it admits a subsequence
      equivalent to the standard unit vector basis of â1.
A complement to this result is due to Odell and Rosenthal (1975).
      Theorem.[33] Let X be a separable Banach space. The following are
      equivalent:
          * The space X does not contain a closed subspace isomorphic to â1.
          * Every element of the bidual Xââ²â² is the weak*-limit of a
            sequence {xn}  in X.
By the Goldstine theorem, every element of the unit ball Bââ²â² of
Xââ²â² is weak*-limit of a net in the unit ball of X. When X does not
contain â1, every element of Bââ²â² is weak*-limit of a sequence in the
unit ball of X.[34]
When the Banach space X is separable, the unit ball of the dual Xââ²,
equipped with the weak*-topology, is a metrizable compact space K,[17] and
every element xââ²â² in the bidual Xââ²â² defines a bounded function on
K:
          x &#x2032;  &#x2208; K &#x21A6;  x &#x2033;  (  x &#x2032;  ) ,   |
      x &#x2033;  (  x &#x2032;  )  |  &#x2264;  &#x2016;  x &#x2033;  &#x2016;
      .   {\displaystyle x'\in K\mapsto x''(x'),\quad \left|x''(x')\right|\leq
      \left\|x''\right\|.}  [x'\in K\mapsto x''(x'),\quad \left|x''
      (x')\right|\leq \left\|x''\right\|.]
This function is continuous for the compact topology of K if and only if
xââ²â² is actually in X, considered as subset of Xââ²â². Assume in
addition for the rest of the paragraph that X does not contain â1. By the
preceding result of Odell and Rosenthal, the function xââ²â² is the
pointwise_limit on K of a sequence {xn} â X of continuous functions on K, it
is therefore a first_Baire_class_function on K. The unit ball of the bidual is
a pointwise compact subset of the first Baire class on K.[35]
*** Sequences, weak and weak* compactness[edit] ***
When X is separable, the unit ball of the dual is weak*-compact by
BanachâAlaoglu and metrizable for the weak* topology,[17] hence every bounded
sequence in the dual has weakly* convergent subsequences. This applies to
separable reflexive spaces, but more is true in this case, as stated below.
The weak topology of a Banach space X is metrizable if and only if X is finite-
dimensional.[36] If the dual Xââ² is separable, the weak topology of the
unit ball of X is metrizable. This applies in particular to separable reflexive
Banach spaces. Although the weak topology of the unit ball is not metrizable in
general, one can characterize weak compactness using sequences.
      EberleinâÅ mulian_theorem.[37] A set A in a Banach space is relatively
      weakly compact if and only if every sequence {an}  in A has a weakly
      convergent subsequence.
A Banach space X is reflexive if and only if each bounded sequence in X has a
weakly convergent subsequence.[38]
A weakly compact subset A in â1 is norm-compact. Indeed, every sequence in A
has weakly convergent subsequences by EberleinâÅ mulian, that are norm
convergent by the Schur property of â1.
***** Schauder bases[edit] *****
Main article: Schauder_basis
A Schauder basis in a Banach space X is a sequence {en}nââ¥â0 of vectors
in X with the property that for every vector x in X, there exist uniquely
defined scalars {xn}nââ¥â0 depending on x, such that
         x =  &#x2211;  n = 0   &#x221E;    x  n    e  n   ,    i.e.,    x =
      lim  n    P  n   ( x ) , &#xA0;  P  n   ( x ) :=  &#x2211;  k = 0   n
      x  k    e  k   .   {\displaystyle x=\sum _{n=0}^{\infty }x_{n}e_{n},\quad
      {\textit {i.e.,}}\quad x=\lim _{n}P_{n}(x),\ P_{n}(x):=\sum _{k=0}^{n}x_
      {k}e_{k}.}  [x=\sum _{n=0}^{\infty }x_{n}e_{n},\quad {\textit
      {i.e.,}}\quad x=\lim _{n}P_{n}(x),\ P_{n}(x):=\sum _{k=0}^{n}x_{k}e_{k}.]
Banach spaces with a Schauder basis are necessarily separable, because the
countable set of finite linear combinations with rational coefficients (say) is
dense.
It follows from the BanachâSteinhaus theorem that the linear mappings {Pn}
are uniformly bounded by some constant C. Let {eâ
n}  denote the coordinate functionals which assign to every x in X the
coordinate xn of x in the above expansion. They are called biorthogonal
functionals. When the basis vectors have norm 1, the coordinate functionals
{eâ
n}  have norm  â¤ 2C in the dual of X.
Most classical separable spaces have explicit bases. The Haar_system {hn}  is a
basis for Lp([0, 1]), 1 â¤ p < â. The trigonometric_system is a basis in Lp
(T) when 1 < p < â. The Schauder_system is a basis in the space C([0, 1]).
[39] The question of whether the disk algebra A(D) has a basis[40] remained
open for more than forty years, until BoÄkarev showed in 1974 that A(D) admits
a basis constructed from the Franklin_system.[41]
Since every vector x in a Banach space X with a basis is the limit of Pn(x),
with Pn of finite rank and uniformly bounded, the space X satisfies the bounded
approximation_property. The first example by Enflo of a space failing the
approximation property was at the same time the first example of a separable
Banach space without a Schauder basis.[42]
Robert C. James characterized reflexivity in Banach spaces with a basis: the
space X with a Schauder basis is reflexive if and only if the basis is both
shrinking_and_boundedly_complete.[43] In this case, the biorthogonal
functionals form a basis of the dual of X.
***** Tensor product[edit] *****
Main article: Tensor_product
[Tensor-diagramB.jpg]
Let X and Y be two K-vector spaces. The tensor_product X â Y of X and Y is a
K-vector space Z with a bilinear mapping T : X Ã Y â Z which has the
following universal_property:
      If T1 : X Ã Y â Z1 is any bilinear mapping into a K-vector space Z1,
      then there exists a unique linear mapping  f  : Z â Z1 such that T1 = f
      â T.
The image under T of a couple (x, y) in X Ã Y is denoted by x â y, and
called a simple tensor. Every element z in X â Y is a finite sum of such
simple tensors.
There are various norms that can be placed on the tensor product of the
underlying vector spaces, amongst others the projective_cross_norm and
injective_cross_norm introduced by A._Grothendieck in 1955.[44]
In general, the tensor product of complete spaces is not complete again. When
working with Banach spaces, it is customary to say that the projective tensor
product[45] of two Banach spaces X and Y is the completion     X     &#x2297;
&#x005E;     &#x03C0;   Y   {\displaystyle X{\widehat {\otimes }}_{\pi }Y}  [X
{\widehat {\otimes }}_{\pi }Y] of the algebraic tensor product X â Y equipped
with the projective tensor norm, and similarly for the injective tensor product
[46]     X     &#x2297; &#x005E;     &#x03B5;   Y   {\displaystyle X{\widehat
{\otimes }}_{\varepsilon }Y}  [X{\widehat {\otimes }}_{\varepsilon }Y].
Grothendieck proved in particular that[47]
             C ( K )     &#x2297; &#x005E;     &#x03B5;   Y    &#x2243; C ( K ,
      Y ) ,      L  1   ( [ 0 , 1 ] )     &#x2297; &#x005E;     &#x03C0;   Y
      &#x2243;  L  1   ( [ 0 , 1 ] , Y ) ,       {\displaystyle {\begin
      {aligned}C(K){\widehat {\otimes }}_{\varepsilon }Y&\simeq C(K,Y),\\L^{1}(
      [0,1]){\widehat {\otimes }}_{\pi }Y&\simeq L^{1}([0,1],Y),\end{aligned}}}
      [{\begin{aligned}C(K){\widehat {\otimes }}_{\varepsilon }Y&\simeq C
      (K,Y),\\L^{1}([0,1]){\widehat {\otimes }}_{\pi }Y&\simeq L^{1}(
      [0,1],Y),\end{aligned}}]
where K is a compact Hausdorff space, C(K, Y) the Banach space of continuous
functions from K to Y and L1([0, 1], Y) the space of Bochner-measurable and
integrable functions from [0, 1] to Y, and where the isomorphisms are
isometric. The two isomorphisms above are the respective extensions of the map
sending the tensor  f ââây to the vector-valued function s â K â  f 
(s)y â Y.
**** Tensor products and the approximation property[edit] ****
Let X be a Banach space. The tensor product      X &#x2032;      &#x2297;
&#x005E;     &#x03B5;   X   {\displaystyle X'{\widehat {\otimes }}_{\varepsilon
}X}  [X'{\widehat {\otimes }}_{\varepsilon }X] is identified isometrically with
the closure in B(X) of the set of finite rank operators. When X has the
approximation_property, this closure coincides with the space of compact
operators on X.
For every Banach space Y, there is a natural norm 1 linear map
         Y     &#x2297; &#x005E;     &#x03C0;   X &#x2192; Y     &#x2297;
      &#x005E;     &#x03B5;   X   {\displaystyle Y{\widehat {\otimes }}_{\pi
      }X\to Y{\widehat {\otimes }}_{\varepsilon }X}  [Y{\widehat {\otimes }}_
      {\pi }X\to Y{\widehat {\otimes }}_{\varepsilon }X]
obtained by extending the identity map of the algebraic tensor product.
Grothendieck related the approximation_problem to the question of whether this
map is one-to-one when Y is the dual of X. Precisely, for every Banach space X,
the map
          X &#x2032;      &#x2297; &#x005E;     &#x03C0;   X &#xA0; &#x27F6;  X
      &#x2032;      &#x2297; &#x005E;     &#x03B5;   X   {\displaystyle X'
      {\widehat {\otimes }}_{\pi }X\ \longrightarrow X'{\widehat {\otimes }}_
      {\varepsilon }X}  [X'{\widehat {\otimes }}_{\pi }X\ \longrightarrow X'
      {\widehat {\otimes }}_{\varepsilon }X]
is one-to-one if and only if X has the approximation property.[48]
Grothendieck conjectured that     X     &#x2297; &#x005E;     &#x03C0;   Y
{\displaystyle X{\widehat {\otimes }}_{\pi }Y}  [X{\widehat {\otimes }}_{\pi
}Y] and     X     &#x2297; &#x005E;     &#x03B5;   Y   {\displaystyle X
{\widehat {\otimes }}_{\varepsilon }Y}  [X{\widehat {\otimes }}_{\varepsilon
}Y] must be different whenever X and Y are infinite-dimensional Banach spaces.
This was disproved by Gilles_Pisier in 1983.[49] Pisier constructed an
infinite-dimensional Banach space X such that     X     &#x2297; &#x005E;
&#x03C0;   X   {\displaystyle X{\widehat {\otimes }}_{\pi }X}  [X{\widehat
{\otimes }}_{\pi }X] and     X     &#x2297; &#x005E;     &#x03B5;   X
{\displaystyle X{\widehat {\otimes }}_{\varepsilon }X}  [X{\widehat {\otimes
}}_{\varepsilon }X] are equal. Furthermore, just as Enflo's example, this space
X is a "hand-made" space that fails to have the approximation property. On the
other hand, Szankowski proved that the classical space B(â2) does not have
the approximation property.[50]
***** Some classification results[edit] *****
**** Characterizations of Hilbert space among Banach spaces[edit] ****
A necessary and sufficient condition for the norm of a Banach space X to be
associated to an inner product is the parallelogram_identity:
         &#x2200; x , y &#x2208; X :  &#x2016; x + y  &#x2016;  2   + &#x2016;
      x &#x2212; y  &#x2016;  2   = 2  (  &#x2016; x  &#x2016;  2   + &#x2016;
      y  &#x2016;  2    )  .   {\displaystyle \forall x,y\in X:\qquad \|x+y\|^
      {2}+\|x-y\|^{2}=2\left(\|x\|^{2}+\|y\|^{2}\right).}  [\forall x,y\in X:
      \qquad \|x+y\|^{2}+\|x-y\|^{2}=2\left(\|x\|^{2}+\|y\|^{2}\right).]
It follows, for example, that the Lebesgue_space Lp([0, 1]) is a Hilbert space
only when p = 2. If this identity is satisfied, the associated inner product is
given by the polarization_identity. In the case of real scalars, this gives:
         &#x27E8; x , y &#x27E9; =    1 4     (  &#x2016; x + y  &#x2016;  2
      &#x2212; &#x2016; x &#x2212; y  &#x2016;  2    )  .   {\displaystyle
      \langle x,y\rangle ={\tfrac {1}{4}}\left(\|x+y\|^{2}-\|x-y\|^{2}\right).}
      [\langle x,y\rangle ={\tfrac {1}{4}}\left(\|x+y\|^{2}-\|x-y\|^
      {2}\right).]
For complex scalars, defining the inner_product so as to be C-linear in x,
antilinear in y, the polarization identity gives:
         &#x27E8; x , y &#x27E9; =    1 4     (  &#x2016; x + y  &#x2016;  2
      &#x2212; &#x2016; x &#x2212; y  &#x2016;  2   + i  (  &#x2016; x + i y
      &#x2016;  2   &#x2212; &#x2016; x &#x2212; i y  &#x2016;  2    )   )  .
      {\displaystyle \langle x,y\rangle ={\tfrac {1}{4}}\left(\|x+y\|^{2}-\|x-
      y\|^{2}+i\left(\|x+iy\|^{2}-\|x-iy\|^{2}\right)\right).}  [\langle
      x,y\rangle ={\tfrac {1}{4}}\left(\|x+y\|^{2}-\|x-y\|^{2}+i\left(\|x+iy\|^
      {2}-\|x-iy\|^{2}\right)\right).]
To see that the parallelogram law is sufficient, one observes in the real case
that < x, y > is symmetric, and in the complex case, that it satisfies the
Hermitian_symmetry property and < ix, y > = i < x, y >. The parallelogram law
implies that < x, y > is additive in x. It follows that it is linear over the
rationals, thus linear by continuity.
Several characterizations of spaces isomorphic (rather than isometric) to
Hilbert spaces are available. The parallelogram law can be extended to more
than two vectors, and weakened by the introduction of a two-sided inequality
with a constant c â¥ 1: KwapieÅ proved that if
          c  &#x2212; 2    &#x2211;  k = 1   n     &#x2016;  x  k   &#x2016;
      2   &#x2264;  Ave  &#x00B1;   &#x2061;   &#x2016;   &#x2211;  k = 1   n
      &#x00B1;  x  k    &#x2016;   2   &#x2264;  c  2    &#x2211;  k = 1   n
      &#x2016;  x  k   &#x2016;   2     {\displaystyle c^{-2}\sum _{k=1}^
      {n}\left\|x_{k}\right\|^{2}\leq \operatorname {Ave} _{\pm }\left\|\sum _
      {k=1}^{n}\pm x_{k}\right\|^{2}\leq c^{2}\sum _{k=1}^{n}\left\|x_
      {k}\right\|^{2}}  [c^{-2}\sum _{k=1}^{n}\left\|x_{k}\right\|^{2}\leq
      \operatorname {Ave} _{\pm }\left\|\sum _{k=1}^{n}\pm x_{k}\right\|^
      {2}\leq c^{2}\sum _{k=1}^{n}\left\|x_{k}\right\|^{2}]
for every integer n and all families of vectors {x1, ..., xn} â X, then the
Banach space X is isomorphic to a Hilbert space.[51] Here, AveÂ± denotes the
average over the 2n possible choices of signs Â±1. In the same article,
KwapieÅ proved that the validity of a Banach-valued Parseval's_theorem for the
Fourier transform characterizes Banach spaces isomorphic to Hilbert spaces.
Lindenstrauss and Tzafriri proved that a Banach space in which every closed
linear subspace is complemented (that is, is the range of a bounded linear
projection) is isomorphic to a Hilbert space.[52] The proof rests upon
Dvoretzky's_theorem about Euclidean sections of high-dimensional centrally
symmetric convex bodies. In other words, Dvoretzky's theorem states that for
every integer n, any finite-dimensional normed space, with dimension
sufficiently large compared to n, contains subspaces nearly isometric to the n-
dimensional Euclidean space.
The next result gives the solution of the so-called homogeneous space problem.
An infinite-dimensional Banach space X is said to be homogeneous if it is
isomorphic to all its infinite-dimensional closed subspaces. A Banach space
isomorphic to â2 is homogeneous, and Banach asked for the converse.[53]
      Theorem.[54] A Banach space isomorphic to all its infinite-dimensional
      closed subspaces is isomorphic to a separable Hilbert space.
An infinite-dimensional Banach space is hereditarily indecomposable when no
subspace of it can be isomorphic to the direct sum of two infinite-dimensional
Banach spaces. The Gowers dichotomy theorem[54] asserts that every infinite-
dimensional Banach space X contains, either a subspace Y with unconditional
basis, or a hereditarily indecomposable subspace Z, and in particular, Z is not
isomorphic to its closed hyperplanes.[55] If X is homogeneous, it must
therefore have an unconditional basis. It follows then from the partial
solution obtained by Komorowski and TomczakâJaegermann, for spaces with an
unconditional basis,[56] that X is isomorphic to â2.
**** Metric classification[edit] ****
If     T : X &#x2192; Y   {\displaystyle T:X\to Y}  [{\displaystyle T:X\to Y}]
is an isometry from the Banach space     X   {\displaystyle X}  [X] onto the
Banach space     Y   {\displaystyle Y}  [Y], then the Mazur-Ulam_theorem states
that     T   {\displaystyle T}  [T] must be an affine transformation. In
particular, if     T (  0  X   ) =  0  Y     {\displaystyle T(0_{X})=0_{Y}}  [
{\displaystyle T(0_{X})=0_{Y}}], this is     T   {\displaystyle T}  [T] maps
the zero of     X   {\displaystyle X}  [X] to the zero of     Y
{\displaystyle Y}  [Y], then     T   {\displaystyle T}  [T] must be linear.
This result implies that the metric in Banach spaces, and more generally in
normed spaces, completely captures their linear structure.
**** Topological classification[edit] ****
Finite dimensional Banach spaces are homeomorphic as topological spaces, if and
only if they have the same dimension as real vector spaces.
AndersonâKadec_theorem (1965â66) proves[57] that any two infinite-
dimensional separable Banach spaces are homeomorphic as topological spaces.
Kadec's theorem was extended by Torunczyk, who proved[58] that any two Banach
spaces are homeomorphic if and only if they have the same density_character,
the minimum cardinality of a dense subset.
**** Spaces of continuous functions[edit] ****
When two compact Hausdorff spaces K1 and K2 are homeomorphic, the Banach spaces
C(K1) and C(K2) are isometric. Conversely, when K1 is not homeomorphic to K2,
the (multiplicative) BanachâMazur distance between C(K1) and C(K2) must be
greater than or equal to 2, see above the results_by_Amir_and_Cambern. Although
uncountable compact metric spaces can have different homeomorphy types, one has
the following result due to Milutin:[59]
      Theorem.[60] Let K be an uncountable compact metric space. Then C(K) is
      isomorphic to C([0, 1]).
The situation is different for countably_infinite compact Hausdorff spaces.
Every countably infinite compact K is homeomorphic to some closed interval of
ordinal_numbers
         &#x27E8; 1 , &#x03B1; &#x27E9; = { &#x03B3; &#xA0; : &#xA0; 1 &#x2264;
      &#x03B3; &#x2264; &#x03B1; }   {\displaystyle \langle 1,\alpha \rangle =\
      {\gamma \ :\ 1\leq \gamma \leq \alpha \}}  [\langle 1,\alpha \rangle =\
      {\gamma \ :\ 1\leq \gamma \leq \alpha \}]
equipped with the order_topology, where Î± is a countably infinite ordinal.[61]
The Banach space C(K) is then isometric to C(<1, Î± >). When Î±, Î² are two
countably infinite ordinals, and assuming Î± â¤ Î², the spaces C(<1, Î± >) and
C(<1, Î² >) are isomorphic if and only if Î² < Î±Ï.[62] For example, the
Banach spaces
         C ( &#x27E8; 1 , &#x03C9; &#x27E9; ) , &#xA0; C ( &#x27E8; 1 ,
      &#x03C9;  &#x03C9;   &#x27E9; ) , &#xA0; C ( &#x27E8; 1 ,  &#x03C9;
      &#x03C9;  2     &#x27E9; ) , &#xA0; C ( &#x27E8; 1 ,  &#x03C9;   &#x03C9;
      3     &#x27E9; ) , &#x22EF; , C ( &#x27E8; 1 ,  &#x03C9;   &#x03C9;
      &#x03C9;     &#x27E9; ) , &#x22EF;   {\displaystyle C(\langle 1,\omega
      \rangle ),\ C(\langle 1,\omega ^{\omega }\rangle ),\ C(\langle 1,\omega ^
      {\omega ^{2}}\rangle ),\ C(\langle 1,\omega ^{\omega ^{3}}\rangle
      ),\cdots ,C(\langle 1,\omega ^{\omega ^{\omega }}\rangle ),\cdots }  [C
      (\langle 1,\omega \rangle ),\ C(\langle 1,\omega ^{\omega }\rangle ),\ C
      (\langle 1,\omega ^{\omega ^{2}}\rangle ),\ C(\langle 1,\omega ^{\omega ^
      {3}}\rangle ),\cdots ,C(\langle 1,\omega ^{\omega ^{\omega }}\rangle
      ),\cdots ]
are mutually non-isomorphic.
***** Examples[edit] *****
Main article: List_of_Banach_spaces
A glossary of symbols:
    * K = R, C;
    * X is a compact_Hausdorff_space;
    * I is a closed and bounded interval [a, b];
    * p, q are real_numbers with 1 < p, q < â so that  1/p + 1/q = 1.
    * Î£ is a Ï-algebra of sets;
    * Î is an algebra of sets (for spaces only requiring finite additivity,
      such as the ba_space);
    * Î¼ is a measure with variation |Î¼|.
                                                                     Classical Banach spaces
                              weakly
        Dual_space  Reflexive sequentially Norm            Notes
                              complete
                                              &#x2016; x
                                           &#x2016;  2   =
                                           (   &#x2211;  i
                                           = 1   n    |
                                           x  i     |   2
                                           )   1  /  2
                                           {\displaystyle
Kn      Kn          Yes       Yes          \|x\|_{2}=\left Euclidean space
                                           (\sum _{i=1}^
                                           {n}|x_{i}|^
                                           {2}\right)^{1/
                                           2}}  [\|x\|_2 =
                                           \left(\sum_
                                           {i=1}^n
                                           |x_i|^2\right)^
                                           {1/2}]
                                              &#x2016; x
                                           &#x2016;  p   =
                                           (   &#x2211;  i
                                           = 1   n    |
                                           x  i     |   p
                                           )    1 p
                                           {\displaystyle
                                           \|x\|_{p}=\left
ân ân     Yes       Yes          (\sum _{i=1}^
p       q                                  {n}|x_{i}|^
                                           {p}\right)^
                                           {\frac {1}{p}}}
                                           [\|x\|_
                                           {p}=\left(\sum
                                           _{i=1}^{n}|x_
                                           {i}|^
                                           {p}\right)^
                                           {\frac {1}{p}}]
                                              &#x2016; x
                                           &#x2016;
                                           &#x221E;   =
                                           max  1 &#x2264;
                                           i &#x2264; n
                                           |   x  i    |
                                           {\displaystyle
ân ân                            \|x\|_{\infty
â  1           Yes       Yes          }=\max
                                           \nolimits _
                                           {1\leq i\leq
                                           n}|x_{i}|}
                                           [\|x\|_{\infty
                                           }=\max
                                           \nolimits _
                                           {1\leq i\leq
                                           n}|x_{i}|]
                                              &#x2016; x
                                           &#x2016;  p   =
                                           (   &#x2211;  i
                                           = 1   &#x221E;
                                           |   x  i     |
                                           p    )    1 p
                                           {\displaystyle
                                           \|x\|_{p}=\left
                                           (\sum _{i=1}^
âp âq     Yes       Yes          {\infty }|x_
                                           {i}|^
                                           {p}\right)^
                                           {\frac {1}{p}}}
                                           [\|x\|_
                                           {p}=\left(\sum
                                           _{i=1}^{\infty
                                           }|x_{i}|^
                                           {p}\right)^
                                           {\frac {1}{p}}]
                                              &#x2016; x
                                           &#x2016;  1   =
                                           &#x2211;  i = 1
                                           &#x221E;    |
                                           x  i    |
â1 ââNo        Yes          {\displaystyle
                                           \|x\|_{1}=\sum
                                           _{i=1}^{\infty
                                           }|x_{i}|}
                                           [\|x\|_{1}=\sum
                                           _{i=1}^{\infty
                                           }|x_{i}|]
                                              &#x2016; x
                                           &#x2016;
                                           &#x221E;   =
                                           sup  i    |   x
                                           i    |
                                           {\displaystyle
ââba        No        No           \|x\|_{\infty
                                           }=\sup
                                           \nolimits _
                                           {i}|x_{i}|}
                                           [\|x\|_{\infty
                                           }=\sup
                                           \nolimits _
                                           {i}|x_{i}|]
                                              &#x2016; x
                                           &#x2016;
                                           &#x221E;   =
                                           sup  i    |   x
                                           i    |
                                           {\displaystyle
c       â1     No        No           \|x\|_{\infty
                                           }=\sup
                                           \nolimits _
                                           {i}|x_{i}|}
                                           [\|x\|_{\infty
                                           }=\sup
                                           \nolimits _
                                           {i}|x_{i}|]
                                              &#x2016; x
                                           &#x2016;
                                           &#x221E;   =
                                           sup  i    |   x
                                           i    |
                                           {\displaystyle
c0      â1     No        No           \|x\|_{\infty   Isomorphic but not isometric to c.
                                           }=\sup
                                           \nolimits _
                                           {i}|x_{i}|}
                                           [\|x\|_{\infty
                                           }=\sup
                                           \nolimits _
                                           {i}|x_{i}|]
                                              &#x2016; x
                                           &#x2016;  b v
                                           =  |   x  1
                                           |  +  &#x2211;
                                           i = 1
                                           &#x221E;    |
                                           x  i + 1
                                           &#x2212;  x  i
                                           |
bv      ââNo        Yes          {\displaystyle  Isometrically isomorphic to â1.
                                           \|x\|_{bv}=|x_
                                           {1}|+\sum _
                                           {i=1}^{\infty
                                           }|x_{i+1}-x_
                                           {i}|}  [\|x\|_
                                           {bv}=|x_
                                           {1}|+\sum _
                                           {i=1}^{\infty
                                           }|x_{i+1}-x_
                                           {i}|]
                                              &#x2016; x
                                           &#x2016;  b  v
                                           0     =
                                           &#x2211;  i = 1
                                           &#x221E;    |
                                           x  i + 1
                                           &#x2212;  x  i
                                           |
bv0     ââNo        Yes          {\displaystyle  Isometrically isomorphic to â1.
                                           \|x\|_{bv_
                                           {0}}=\sum _
                                           {i=1}^{\infty
                                           }|x_{i+1}-x_
                                           {i}|}  [\|x\|_
                                           {bv_{0}}=\sum _
                                           {i=1}^{\infty
                                           }|x_{i+1}-x_
                                           {i}|]
                                              &#x2016; x
                                           &#x2016;  b s
                                           =  sup  n    |
                                           &#x2211;  i = 1
                                           n    x  i    |
                                           {\displaystyle
                                           \|x\|_{bs}=\sup
                                           \nolimits _
bs      ba          No        No           {n}\left|\sum _ Isometrically isomorphic to ââ.
                                           {i=1}^{n}x_
                                           {i}\right|}
                                           [\|x\|_
                                           {bs}=\sup
                                           \nolimits _
                                           {n}\left|\sum _
                                           {i=1}^{n}x_
                                           {i}\right|]
                                              &#x2016; x
                                           &#x2016;  b s
                                           =  sup  n    |
                                           &#x2211;  i = 1
                                           n    x  i    |
                                           {\displaystyle
                                           \|x\|_{bs}=\sup
                                           \nolimits _
cs      â1     No        No           {n}\left|\sum _ Isometrically isomorphic to c.
                                           {i=1}^{n}x_
                                           {i}\right|}
                                           [\|x\|_
                                           {bs}=\sup
                                           \nolimits _
                                           {n}\left|\sum _
                                           {i=1}^{n}x_
                                           {i}\right|]
                                              &#x2016; f
                                           &#x2016;  B   =
                                           sup  x &#x2208;
                                           X    |  f ( x )
                                           |
B(X,    ba(Î)    No        No           {\displaystyle
Î)                                      \|f\|_{B}=\sup
                                           \nolimits _
                                           {x\in X}|f(x)|}
                                           [\|f\|_{B}=\sup
                                           \nolimits _
                                           {x\in X}|f(x)|]
                                              &#x2016; x
                                           &#x2016;  C ( X
                                           )   =  max  x
                                           &#x2208; X    |
                                           f ( x )  |
                                           {\displaystyle
C(X)    rca(X)      No        No           \|x\|_{C
                                           (X)}=\max
                                           \nolimits _
                                           {x\in X}|f(x)|}
                                           [\|x\|_{C
                                           (X)}=\max
                                           \nolimits _
                                           {x\in X}|f(x)|]
                                              &#x2016;
                                           &#x03BC;
                                           &#x2016;  b a
                                           =  sup  A
                                           &#x2208;
                                           &#x03A3;    |
                                           &#x03BC;  |
                                           ( A )
                                           {\displaystyle
ba(Î)?           No        Yes          \|\mu \|_
                                           {ba}=\sup
                                           \nolimits _
                                           {A\in \Sigma
                                           }|\mu |(A)}
                                           [\|\mu \|_
                                           {ba}=\sup
                                           \nolimits _
                                           {A\in \Sigma
                                           }|\mu |(A)]
                                              &#x2016;
                                           &#x03BC;
                                           &#x2016;  b a
                                           =  sup  A
                                           &#x2208;
                                           &#x03A3;    |
                                           &#x03BC;  |
                                           ( A )
                                           {\displaystyle
ca(Î£)?           No        Yes          \|\mu \|_       A closed subspace of ba(Î£).
                                           {ba}=\sup
                                           \nolimits _
                                           {A\in \Sigma
                                           }|\mu |(A)}
                                           [\|\mu \|_
                                           {ba}=\sup
                                           \nolimits _
                                           {A\in \Sigma
                                           }|\mu |(A)]
                                              &#x2016;
                                           &#x03BC;
                                           &#x2016;  b a
                                           =  sup  A
                                           &#x2208;
                                           &#x03A3;    |
                                           &#x03BC;  |
                                           ( A )
                                           {\displaystyle
rca(Î£?           No        Yes          \|\mu \|_       A closed subspace of ca(Î£).
                                           {ba}=\sup
                                           \nolimits _
                                           {A\in \Sigma
                                           }|\mu |(A)}
                                           [\|\mu \|_
                                           {ba}=\sup
                                           \nolimits _
                                           {A\in \Sigma
                                           }|\mu |(A)]
                                              &#x2016; f
                                           &#x2016;  p   =
                                           (  &#x222B;  |
                                           f   |   p    d
                                           &#x03BC;  )
                                           1 p
                                           {\displaystyle
                                           \|f\|_{p}=\left
Lp(Î¼)Lq(Î¼)    Yes       Yes          (\int |f|^
                                           {p}\,d\mu
                                           \right)^{\frac
                                           {1}{p}}}
                                           [\|f\|_
                                           {p}=\left(\int
                                           |f|^{p}\,d\mu
                                           \right)^{\frac
                                           {1}{p}}]
                                              &#x2016; f
                                           &#x2016;  1   =
                                           &#x222B;  |  f
                                           |   d &#x03BC;
L1(Î¼)Lâ(Î¼No        Yes          {\displaystyle  The dual is Lâ(Î¼) if Î¼ is Ï-finite.
                                           \|f\|_{1}=\int
                                           |f|\,d\mu }
                                           [\|f\|_{1}=\int
                                           |f|\,d\mu ]
                                              &#x2016; f
                                           &#x2016;  B V
                                           =  V  f   ( I )
                                           +  lim  x
                                           &#x2192;  a  +
                                           f ( x )
                                           {\displaystyle
                                           \|f\|_{BV}=V_
BV(I)   ?           No        Yes          {f}(I)+\lim     Vf (I) is the total_variation of  f 
                                           \nolimits _
                                           {x\to a^{+}}f
                                           (x)}  [\|f\|_
                                           {BV}=V_{f}
                                           (I)+\lim
                                           \nolimits _
                                           {x\to a^{+}}f
                                           (x)]
                                              &#x2016; f
                                           &#x2016;  B V
                                           =  V  f   ( I ) NBV(I) consists of BV(I) functions such that      lim  x
NBV(I)  ?           No        Yes          {\displaystyle  &#x2192;  a  +     f ( x ) = 0   {\displaystyle \lim
                                           \|f\|_{BV}=V_   \nolimits _{x\to a^{+}}f(x)=0}  [\lim \nolimits _{x\to a^
                                           {f}(I)}         {+}}f(x)=0]
                                           [\|f\|_{BV}=V_
                                           {f}(I)]
                                              &#x2016; f
                                           &#x2016;  B V
                                           =  V  f   ( I )
                                           +  lim  x
                                           &#x2192;  a  +
                                           f ( x )
                                           {\displaystyle
                                           \|f\|_{BV}=V_
AC(I)   K + Lâ(No        Yes          {f}(I)+\lim     Isomorphic to the Sobolev_space W 1,1(I).
                                           \nolimits _
                                           {x\to a^{+}}f
                                           (x)}  [\|f\|_
                                           {BV}=V_{f}
                                           (I)+\lim
                                           \nolimits _
                                           {x\to a^{+}}f
                                           (x)]
                                              &#x2016; f
                                           &#x2016; =
                                           &#x2211;  i = 0
                                           n    sup  x
                                           &#x2208; [ a ,
                                           b ]    |   f
                                           ( i )   ( x )
                                           |
                                           {\displaystyle
Cn([a,                                     \|f\|=\sum _    Isomorphic to Rn â C([a,b]), essentially by Taylor's
b])     rca([a,b])  No        No           {i=0}^{n}\sup   theorem.
                                           \nolimits _
                                           {x\in
                                           [a,b]}\left|f^{
                                           (i)}(x)\right|}
                                           [\|f\|=\sum _
                                           {i=0}^{n}\sup
                                           \nolimits _
                                           {x\in
                                           [a,b]}\left|f^{
                                           (i)}(x)\right|]
***** Derivatives[edit] *****
Several concepts of a derivative may be defined on a Banach space. See the
articles on the FrÃ©chet_derivative and the Gateaux_derivative for details. The
FrÃ©chet derivative allows for an extension of the concept of a directional
derivative to Banach spaces. The Gateaux derivative allows for an extension of
a directional_derivative to locally_convex topological_vector_spaces. FrÃ©chet
differentiability is a stronger condition than Gateaux differentiability. The
quasi-derivative is another generalization of directional derivative that
implies a stronger condition than Gateaux differentiability, but a weaker
condition than FrÃ©chet differentiability.
***** Generalizations[edit] *****
Several important spaces in functional analysis, for instance the space of all
infinitely often differentiable functions R â R, or the space of all
distributions on R, are complete but are not normed vector spaces and hence not
Banach spaces. In FrÃ©chet_spaces one still has a complete metric, while LF-
spaces are complete uniform vector spaces arising as limits of FrÃ©chet spaces.
***** See also[edit] *****
    * Space_(mathematics)
          o Hilbert_space
          o Lp_space
          o Semi-inner-product
          o Sobolev_space
          o Hardy_space
    * Interpolation_space
    * Distortion_problem
    * Smith_space
***** Notes[edit] *****
   1. ^ Bourbaki_1987, V.86
   2. ^ see Theorem 1.3.9, p. 20 in Megginson_(1998).
   3. ^ see Corollary 1.4.18, p. 32 in Megginson_(1998).
   4. ^ see Banach_(1932), p. 182.
   5. ^ a b see pp. 17â19 in Carothers_(2005).
   6. ^ see Banach_(1932), pp. 11-12.
   7. ^ see Banach_(1932), Th. 9 p. 185.
   8. ^ see Theorem 6.1, p. 55 in Carothers_(2005)
   9. ^ Several books about functional analysis use the notation X â for the
      continuous dual, for example Carothers_(2005), Lindenstrauss_&_Tzafriri_
      (1977), Megginson_(1998), Ryan_(2002), Wojtaszczyk_(1991).
  10. ^ Theorem 1.9.6, p. 75 in Megginson_(1998)
  11. ^ see also Theorem 2.2.26, p. 179 in Megginson_(1998)
  12. ^ see p. 19 in Carothers_(2005).
  13. ^ Theorems 1.10.16, 1.10.17 pp.94â95 in Megginson_(1998)
  14. ^ Theorem 1.12.11, p. 112 in Megginson_(1998)
  15. ^ Theorem 2.5.16, p. 216 in Megginson_(1998).
  16. ^ see II.A.8, p. 29 in Wojtaszczyk_(1991)
  17. ^ a b c see Theorem 2.6.23, p. 231 in Megginson_(1998).
  18. ^ see N. Bourbaki, (2004), "Integration I", Springer Verlag,
  19. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
  20. ISBN 3-540-41129-1.
  21. ^ a bEilenberg, Samuel (1942). "Banach Space Methods in Topology". Annals
      of_Mathematics. 43 (3): 568. doi:10.2307/1968812.
  22. ^ see also Banach_(1932), p. 170 for metrizable K and L.
  23. ^ SeeAmir, D. (1965). "On isomorphisms of continuous function spaces".
      Israel J. Math. 3: 205â210. doi:10.1007/bf03008398.
  24. ^Cambern, M. (1966). "A generalized BanachâStone theorem". Proc. Amer.
      Math. Soc. 17: 396â400. doi:10.1090/s0002-9939-1966-0196471-9.
  25.  AndCambern, M. (1967). "On isomorphisms with small bound". Proc. Amer.
      Math. Soc. 18: 1062â1066. doi:10.1090/s0002-9939-1967-0217580-2.
  26. ^Cohen, H. B. (1975). "A bound-two isomorphism between C(X) Banach
      spaces". Proc. Amer. Math. Soc. 50: 215â217. doi:10.1090/s0002-9939-
      1975-0380379-5.
  27. ^ See for exampleArveson, W. (1976). An Invitation to C*-Algebra.
      Springer-Verlag. ISBN 0-387-90176-0.
  28. ^R. C. James (1951). "A_non-reflexive_Banach_space_isometric_with_its
      second_conjugate_space". Proc. Natl. Acad. Sci. U.S.A. 37: 174â177.
      Bibcode:1951PNAS...37..174J. doi:10.1073/pnas.37.3.174. PMC 1063327.
      PMID 16588998.
  29. ^ see Lindenstrauss_&_Tzafriri_(1977), p. 25.
  30. ^bishop, See E.; Phelps, R. (1961). "A proof that every Banach space is
      subreflexive". Bull. Amer. Math. Soc. 67: 97â98. doi:10.1090/s0002-
      9904-1961-10514-4.
  31. ^ see III.C.14, p. 140 in Wojtaszczyk_(1991).
  32. ^ see Corollary 2, p. 11 in Diestel_(1984).
  33. ^ see p. 85 in Diestel_(1984).
  34. ^Rosenthal, Haskell P (1974). "A characterization of Banach spaces
      containing â1". Proc. Natl. Acad. Sci. U.S.A. 71: 2411â2413. arXiv:
      math.FA/9210205. Bibcode:1974PNAS...71.2411R. doi:10.1073/pnas.71.6.2411.
  35.  Rosenthal's proof is for real scalars. The complex version of the result
      is due to L. Dor, inDor, Leonard E (1975). "On sequences spanning a
      complex â1 space". Proc. Amer. Math. Soc. 47: 515â516. doi:10.1090/
      s0002-9939-1975-0358308-x.
  36. ^ see p. 201 in Diestel_(1984).
  37. ^Odell, Edward W.; Rosenthal, Haskell P. (1975), "A double-dual
      characterization of separable Banach spaces containing â1", Israel J.
      Math., 20: 375â384, doi:10.1007/bf02760341
  38. .
  39. ^ Odell and Rosenthal, Sublemma p. 378 and Remark p. 379.
  40. ^ for more on pointwise compact subsets of the Baire class, seeBourgain,
      Jean; Fremlin, D. H.; Talagrand, Michel (1978), "Pointwise Compact Sets
      of Baire-Measurable Functions", Am. J. Math., 100: 845â886, doi:
      10.2307/2373913, JSTOR 2373913
  41. .
  42. ^ see Proposition 2.5.14, p. 215 in Megginson_(1998).
  43. ^ see for example p. 49, II.C.3 in Wojtaszczyk_(1991).
  44. ^ see Corollary 2.8.9, p. 251 in Megginson_(1998).
  45. ^ see Lindenstrauss_&_Tzafriri_(1977) p. 3.
  46. ^ the question appears p. 238, Â§3 in Banach's book, Banach_(1932).
  47. ^ see S. V. BoÄkarev, "Existence of a basis in the space of functions
      analytic in the disc, and some properties of Franklin's system".
      (Russian) Mat. Sb. (N.S.) 95(137) (1974), 3â18, 159.
  48. ^ seeEnflo, P. (1973). "A_counterexample_to_the_approximation_property_in
      Banach_spaces" (PDF). Acta Math. 130: 309â317. doi:10.1007/bf02392270.
      Archived from the_original (PDF) on 2016-03-03. Retrieved 2016-06-02.
  49. ^ see R.C. James, "Bases and reflexivity of Banach spaces". Ann. of Math.
      (2) 52, (1950). 518â527. See also Lindenstrauss_&_Tzafriri_(1977) p. 9.
  50. ^ see A. Grothendieck, "Produits tensoriels topologiques et espaces
      nuclÃ©aires". Mem. Amer. Math. Soc. 1955 (1955), no. 16, 140 pp., and A.
      Grothendieck, "RÃ©sumÃ© de la thÃ©orie mÃ©trique des produits tensoriels
      topologiques". Bol. Soc. Mat. SÃ£o Paulo 8 1953 1â79.
  51. ^ see chap. 2, p. 15 in Ryan_(2002).
  52. ^ see chap. 3, p. 45 in Ryan_(2002).
  53. ^ see Example. 2.19, p. 29, and pp. 49â50 in Ryan_(2002).
  54. ^ see Proposition 4.6, p. 74 in Ryan_(2002).
  55. ^ see Pisier, Gilles (1983), "Counterexamples to a conjecture of
      Grothendieck", Acta Math. 151:181â208.
  56. ^ see Szankowski, Andrzej (1981), "B(H) does not have the approximation
      property", Acta Math. 147: 89â108. Ryan claims that this result is due
      to Per_Enflo, p. 74 in Ryan_(2002).
  57. ^ see KwapieÅ, S. (1970), "A linear topological characterization of
      inner-product spaces", Studia Math. 38:277â278.
  58. ^ see Lindenstrauss, J. and Tzafriri, L. (1971), "On the complemented
      subspaces problem", Israel J. Math. 9:263â269.
  59. ^ see p. 245 in Banach_(1932). The homogeneity property is called
      "propriÃ©tÃ© (15)" there. Banach writes: "on ne connaÃ®t aucun exemple
      d'espace Ã  une infinitÃ© de dimensions qui, sans Ãªtre isomorphe avec
      (L2), possÃ¨de la propriÃ©tÃ© (15)".
  60. ^ a b Gowers, W. T. (1996), "A new dichotomy for Banach spaces", Geom.
      Funct. Anal. 6:1083â1093.
  61. ^ seeGowers, W. T. (1994). "A solution to Banach's hyperplane problem".
      Bull. London Math. Soc. 26: 523â530. doi:10.1112/blms/26.6.523.
  62. ^ seeKomorowski, Ryszard A.; Tomczak-Jaegermann, Nicole (1995). "Banach
      spaces without local unconditional structure". Israel J. Math. 89:
      205â226. arXiv:math/9306211. doi:10.1007/bf02808201.
  63.  and alsoKomorowski, Ryszard A.; Tomczak-Jaegermann, Nicole (1998).
      "Erratum to: Banach spaces without local unconditional structure". Israel
      J. Math. 105: 85â92. arXiv:math/9607205. doi:10.1007/bf02780323.
  64. ^C. Bessaga, A. PeÅczyÅski (1975). Selected_Topics_in_Infinite-
      Dimensional_Topology. Panstwowe wyd. naukowe. pp. 177â230.
  65. ^H. Torunczyk (1981). Characterizing Hilbert Space Topology. Fundamenta
      MAthematicae. pp. 247â262.
  66. ^ Milyutin, AlekseÄ­ A. (1966), "Isomorphism of the spaces of continuous
      functions over compact sets of the cardinality of the continuum".
      (Russian) Teor. FunkciÄ­ Funkcional. Anal. i PriloÅ¾en. Vyp. 2:150â156.
  67. ^ Milutin. See also Rosenthal, Haskell P., "The Banach spaces C(K)" in
      Handbook of the geometry of Banach spaces, Vol. 2, 1547â1602, North-
      Holland, Amsterdam, 2003.
  68. ^ One can take Î± = Ï Î²n, where Î² + 1 is the CantorâBendixson_rank
      of K, and n > 0 is the finite number of points in the Î²-th derived_set K
      (Î²) of K. See Mazurkiewicz,_Stefan; SierpiÅski,_WacÅaw (1920),
      "Contribution Ã  la topologie des ensembles dÃ©nombrables", Fundamenta
      Mathematicae 1: 17â27.
  69. ^ Bessaga, CzesÅaw; PeÅczyÅski, Aleksander (1960), "Spaces of
      continuous functions. IV. On isomorphical classification of spaces of
      continuous functions", Studia Math. 19:53â62.
***** References[edit] *****
    * Banach,_Stefan (1932), ThÃ©orie_des_opÃ©rations_linÃ©aires (PDF),
      Monografie Matematyczne, 1, Warszawa: Subwencji Funduszu Kultury
      Narodowej, Zbl 0005.20901, archived from the_original (PDF) on 2014-01-
      11, retrieved 2016-06-10
.
Beauzamy, Bernard (1985) [1982], Introduction to Banach Spaces and their
Geometry (Second revised ed.), North-Holland
.
Bourbaki,_Nicolas (1987), Topological vector spaces, Elements of mathematics,
Berlin: Springer-Verlag, ISBN 978-3-540-13627-9
.
Carothers, Neal L. (2005), A short course on Banach space theory, London
Mathematical Society Student Texts, 64, Cambridge: Cambridge University Press,
pp. xii+184, ISBN 0-521-84283-2
.
Diestel, Joseph (1984), Sequences and series in Banach spaces, Graduate Texts
in Mathematics, 92, New York: Springer-Verlag, pp. xii+261, ISBN 0-387-90859-5
.
Dunford, Nelson; Schwartz, Jacob T. with the assistance of W. G. Bade and R. G.
Bartle (1958), Linear Operators. I. General Theory, Pure and Applied
Mathematics, 7, New York: Interscience Publishers, Inc., MR 0117523
Lindenstrauss,_Joram; Tzafriri, Lior (1977), Classical Banach Spaces I,
Sequence Spaces, Ergebnisse der Mathematik und ihrer Grenzgebiete, 92, Berlin:
Springer-Verlag, ISBN 3-540-08072-4
.
Megginson,_Robert_E. (1998), An introduction to Banach space theory, Graduate
Texts in Mathematics, 183, New York: Springer-Verlag, pp. xx+596, ISBN 0-387-
98431-3
.
Ryan, Raymond A. (2002), Introduction to Tensor Products of Banach Spaces,
Springer Monographs in Mathematics, London: Springer-Verlag, pp. xiv+225,
ISBN 1-85233-437-1
.
Wojtaszczyk, PrzemysÅaw (1991), Banach spaces for analysts, Cambridge Studies
in Advanced Mathematics, 25, Cambridge: Cambridge University Press,
pp. xiv+382, ISBN 0-521-35618-0
.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Banach_space", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Weisstein,_Eric_W. "Banach_Space". MathWorld.
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
                       * BanachâSteinhaus_(Uniform_boundedness)
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
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85011441
                                              * NDL: 00560500

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Banach_space&oldid=902704907"
Categories:
    * Banach_spaces
    * Science_and_technology_in_Poland
Hidden categories:
    * Wikipedia_articles_with_LCCN_identifiers
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ØªÛØ±Ú©Ø¬Ù
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ú©ÙØ±Ø¯Û
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 20 June 2019, at 17:22 (UTC).
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
