The following text has been accessed from https://en.wikipedia.org/wiki/Riesz_representation_theorem at Fri Aug 9 02:38:49 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Riesz representation theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
There are several well-known theorems in functional_analysis known as the Riesz
representation theorem. They are named in honor of Frigyes_Riesz.
This article will describe his theorem concerning the dual of a Hilbert_space,
which is sometimes called the FrÃ©chetâRiesz theorem. For the theorems
relating linear_functionals to measures, see RieszâMarkovâKakutani
representation_theorem.
***** The Hilbert space representation theorem[edit] *****
This theorem establishes an important connection between a Hilbert_space and
its continuous_dual_space. If the underlying field is the real_numbers, the two
are isometrically isomorphic; if the underlying field is the complex_numbers,
the two are isometrically anti-isomorphic. The (anti-) isomorphism is a
particular natural one as will be described next; a natural_isomorphism.
Let H be a Hilbert space, and let H* denote its dual space, consisting of all
continuous_linear_functionals from H into the field      R    {\displaystyle
\mathbb {R} }  [\mathbb {R} ] or      C    {\displaystyle \mathbb {C} }
[\mathbb {C} ]. If     x   {\displaystyle x}  [x] is an element of H, then the
function      &#x03C6;  x   ,   {\displaystyle \varphi _{x},}  [{\displaystyle
\varphi _{x},}] for all     y   {\displaystyle y}  [y] in H defined by:
    &#x03C6;  x   ( y ) =  &#x27E8;  y , x  &#x27E9;  ,   {\displaystyle
\varphi _{x}(y)=\left\langle y,x\right\rangle ,}  [\varphi _{x}(y)=\left\langle
y,x\right\rangle ,]
where     &#x27E8; &#x22C5; , &#x22C5; &#x27E9;   {\displaystyle \langle \cdot
,\cdot \rangle }  [\langle \cdot ,\cdot \rangle ] denotes the inner_product of
the Hilbert space, is an element of H*. The Riesz representation theorem states
that every element of H* can be written uniquely in this form.
Riesz-FrÃ©chet representation theorem. Let     H   {\displaystyle H}  [H] be a
Hilbert space and     &#x03C6; &#x2208;  H  &#x2217;     {\displaystyle \varphi
\in H^{*}}  [{\displaystyle \varphi \in H^{*}}]. Then there exists     f
&#x2208; H   {\displaystyle f\in H}  [{\displaystyle f\in H}] such that for any
x &#x2208; H   {\displaystyle x\in H}  [x\in H],     &#x03C6; ( x ) = &#x27E8;
f , x &#x27E9;   {\displaystyle \varphi (x)=\langle f,x\rangle }  [
{\displaystyle \varphi (x)=\langle f,x\rangle }]. Moreover     &#x2016; f
&#x2016;  H   = &#x2016; &#x03C6;  &#x2016;  H &#x2217;     {\displaystyle
\|f\|_{H}=\|\varphi \|_{H*}}  [{\displaystyle \|f\|_{H}=\|\varphi \|_{H*}}]
Proof. Let     M = { u &#x2208; H &#xA0;  |  &#xA0; &#x03C6; ( u ) = 0 }
{\displaystyle M=\{u\in H\ |\ \varphi (u)=0\}}  [{\displaystyle M=\{u\in H\ |\
\varphi (u)=0\}}]. Clearly     M   {\displaystyle M}  [M] is closed subspace of
H   {\displaystyle H}  [H]. If     M = H   {\displaystyle M=H}  [{\displaystyle
M=H}], then we can trivially choose     v = 0   {\displaystyle v=0}  [v=0]. Now
assume     M &#x2260; H   {\displaystyle M\neq H}  [{\displaystyle M\neq H}].
Then      M  &#x22A5;     {\displaystyle M^{\perp }}  [{\displaystyle M^{\perp
}}] is one-dimensional. Indeed, let      v  1   ,  v  2     {\displaystyle v_
{1},v_{2}}  [v_{1},v_{2}] be nonzero vectors in      M  &#x22A5;
{\displaystyle M^{\perp }}  [{\displaystyle M^{\perp }}]. Then there is nonzero
real number     &#x03BB;   {\displaystyle \lambda }  [\lambda ], such that
&#x03BB; &#x03C6; (  v  1   ) = &#x03C6; (  v  2   )   {\displaystyle \lambda
\varphi (v_{1})=\varphi (v_{2})}  [{\displaystyle \lambda \varphi (v_
{1})=\varphi (v_{2})}]. Observe that     &#x03BB;  v  1   &#x2212;  v  2
&#x2208;  M  &#x22A5;     {\displaystyle \lambda v_{1}-v_{2}\in M^{\perp }}  [
{\displaystyle \lambda v_{1}-v_{2}\in M^{\perp }}] and     &#x03C6; ( &#x03BB;
v  1   &#x2212;  v  2   ) = 0   {\displaystyle \varphi (\lambda v_{1}-v_{2})=0}
[{\displaystyle \varphi (\lambda v_{1}-v_{2})=0}], so     &#x03BB;  v  1
&#x2212;  v  2   &#x2208; M   {\displaystyle \lambda v_{1}-v_{2}\in M}  [
{\displaystyle \lambda v_{1}-v_{2}\in M}]. This means that     &#x03BB;  v  1
&#x2212;  v  2   = 0   {\displaystyle \lambda v_{1}-v_{2}=0}  [{\displaystyle
\lambda v_{1}-v_{2}=0}]. Now let     g   {\displaystyle g}  [g] be unit vector
in      M  &#x22A5;     {\displaystyle M^{\perp }}  [{\displaystyle M^{\perp
}}]. For arbitrary     x &#x2208; H   {\displaystyle x\in H}  [x\in H], let
v   {\displaystyle v}  [v] be the orthogonal projections of     x
{\displaystyle x}  [x] onto      M  &#x22A5;     {\displaystyle M^{\perp }}  [
{\displaystyle M^{\perp }}] respectively. Then     v = &#x27E8; g , v &#x27E9;
g   {\displaystyle v=\langle g,v\rangle g}  [{\displaystyle v=\langle
g,v\rangle g}] and     &#x27E8; g , x &#x2212; v &#x27E9; = 0   {\displaystyle
\langle g,x-v\rangle =0}  [{\displaystyle \langle g,x-v\rangle =0}] (from the
properties of orthogonal projections), so that     x &#x2212; v &#x2208; M
{\displaystyle x-v\in M}  [{\displaystyle x-v\in M}] and     &#x27E8; g , x
&#x27E9; = &#x27E8; g , v &#x27E9;   {\displaystyle \langle g,x\rangle =\langle
g,v\rangle }  [{\displaystyle \langle g,x\rangle =\langle g,v\rangle }]. Thus
&#x03C6; ( x ) = &#x03C6; ( v + x &#x2212; v ) = &#x03C6; ( &#x27E8; g , v
&#x27E9; g ) + &#x03C6; ( x &#x2212; v ) = &#x27E8; g , v &#x27E9; &#x03C6; ( g
) = &#x27E8; g , x &#x27E9; &#x03C6; ( g )   {\displaystyle \varphi (x)=\varphi
(v+x-v)=\varphi (\langle g,v\rangle g)+\varphi (x-v)=\langle g,v\rangle \varphi
(g)=\langle g,x\rangle \varphi (g)}  [{\displaystyle \varphi (x)=\varphi (v+x-
v)=\varphi (\langle g,v\rangle g)+\varphi (x-v)=\langle g,v\rangle \varphi
(g)=\langle g,x\rangle \varphi (g)}]. Hence     f = &#x03C6; ( g ) g
{\displaystyle f=\varphi (g)g}  [{\displaystyle f=\varphi (g)g}]. We also see
&#x2016; f  &#x2016;  H   = &#x03C6; ( g )   {\displaystyle \|f\|_{H}=\varphi
(g)}  [{\displaystyle \|f\|_{H}=\varphi (g)}]. From the Cauchy-Bunyakovsky-
Schwartz inequality     &#x03C6; ( x ) &#x2264; &#x2016; g &#x2016; &#x2016; x
&#x2016; &#x03C6; ( g )   {\displaystyle \varphi (x)\leq \|g\|\|x\|\varphi (g)}
[{\displaystyle \varphi (x)\leq \|g\|\|x\|\varphi (g)}], thus for     x
{\displaystyle x}  [x] with unit norm     &#x03C6; ( x ) &#x2264; &#x03C6; ( g
)   {\displaystyle \varphi (x)\leq \varphi (g)}  [{\displaystyle \varphi
(x)\leq \varphi (g)}]. This implies that     &#x2016; &#x03C6;  &#x2016;  H
&#x2217;   = &#x03C6; ( g )   {\displaystyle \|\varphi \|_{H*}=\varphi (g)}  [
{\displaystyle \|\varphi \|_{H*}=\varphi (g)}].
Given any continuous linear functional g in H*, the corresponding element
x  g   &#x2208; H   {\displaystyle x_{g}\in H}  [{\displaystyle x_{g}\in H}]
can be constructed uniquely by      x  g   = g (  e  1   )  e  1   + g (  e  2
)  e  2   + . . .   {\displaystyle x_{g}=g(e_{1})e_{1}+g(e_{2})e_{2}+...}  [
{\displaystyle x_{g}=g(e_{1})e_{1}+g(e_{2})e_{2}+...}], where     {  e  i   }
{\displaystyle \{e_{i}\}}  [\{e_{i}\}] is an orthonormal_basis of H, and the
value of      x  g     {\displaystyle x_{g}}  [{\displaystyle x_{g}}] does not
vary by choice of basis. Thus, if     y &#x2208; H , y =  a  1    e  1   +  a
2    e  2   + . . .   {\displaystyle y\in H,y=a_{1}e_{1}+a_{2}e_{2}+...}  [
{\displaystyle y\in H,y=a_{1}e_{1}+a_{2}e_{2}+...}], then     g ( y ) =  a  1
g (  e  1   ) +  a  2   g (  e  2   ) + . . . = &#x27E8;  x  g   , y &#x27E9; .
{\displaystyle g(y)=a_{1}g(e_{1})+a_{2}g(e_{2})+...=\langle x_{g},y\rangle .}
[{\displaystyle g(y)=a_{1}g(e_{1})+a_{2}g(e_{2})+...=\langle x_{g},y\rangle .}]
Theorem. The mapping     &#x03A6;   {\displaystyle \Phi }  [\Phi ]: H â H*
defined by     &#x03A6; ( x )   {\displaystyle \Phi (x)}  [\Phi (x)] =
&#x03C6;  x     {\displaystyle \varphi _{x}}  [\varphi _{x}] is an isometric
(anti-) isomorphism, meaning that:
    *    &#x03A6;   {\displaystyle \Phi }  [\Phi ] is bijective.
    * The norms of     x   {\displaystyle x}  [x] and      &#x03C6;  x
      {\displaystyle \varphi _{x}}  [\varphi _{x}] agree:     &#x2016; x
      &#x2016; = &#x2016; &#x03A6; ( x ) &#x2016;   {\displaystyle \Vert x\Vert
      =\Vert \Phi (x)\Vert }  [\Vert x\Vert =\Vert \Phi (x)\Vert ].
    *    &#x03A6;   {\displaystyle \Phi }  [\Phi ] is additive:     &#x03A6;
      (  x  1   +  x  2   ) = &#x03A6; (  x  1   ) + &#x03A6; (  x  2   )
      {\displaystyle \Phi (x_{1}+x_{2})=\Phi (x_{1})+\Phi (x_{2})}  [\Phi (x_
      {1}+x_{2})=\Phi (x_{1})+\Phi (x_{2})].
    * If the base field is      R    {\displaystyle \mathbb {R} }  [\mathbb {R}
      ], then     &#x03A6; ( &#x03BB; x ) = &#x03BB; &#x03A6; ( x )
      {\displaystyle \Phi (\lambda x)=\lambda \Phi (x)}  [\Phi (\lambda
      x)=\lambda \Phi (x)] for all real numbers Î».
    * If the base field is      C    {\displaystyle \mathbb {C} }  [\mathbb {C}
      ], then     &#x03A6; ( &#x03BB; x ) =    &#x03BB; &#x00AF;    &#x03A6;
      ( x )   {\displaystyle \Phi (\lambda x)={\bar {\lambda }}\Phi (x)}  [\Phi
      (\lambda x)={\bar {\lambda }}\Phi (x)] for all complex numbers Î», where
      &#x03BB; &#x00AF;      {\displaystyle {\bar {\lambda }}}  [{\bar {\lambda
      }}] denotes the complex_conjugation of     &#x03BB;   {\displaystyle
      \lambda }  [\lambda ].
The inverse_map of     &#x03A6;   {\displaystyle \Phi }  [\Phi ] can be
described as follows. Given a non-zero element     &#x03C6;   {\displaystyle
\varphi }  [\varphi ] of H*, the orthogonal_complement of the kernel of
&#x03C6;   {\displaystyle \varphi }  [\varphi ] is a one-dimensional subspace
of H. Take a non-zero element z in that subspace, and set     x =    &#x03C6;
( z )  &#x00AF;   &#x22C5; z  /     &#x2016; z &#x2016;    2     {\displaystyle
x={\overline {\varphi (z)}}\cdot z/{\left\Vert z\right\Vert }^{2}}  [x=
{\overline {\varphi (z)}}\cdot z/{\left\Vert z\right\Vert }^{2}]. Then
&#x03A6; ( x )   {\displaystyle \Phi (x)}  [\Phi (x)] =     &#x03C6;
{\displaystyle \varphi }  [\varphi ].
Historically, the theorem is often attributed simultaneously to Riesz and
FrÃ©chet in 1907 (see references).
In the mathematical treatment of quantum_mechanics, the theorem can be seen as
a justification for the popular braâket_notation. The theorem says that,
every bra     &#x27E8; &#x03C8;  |    {\displaystyle \langle \psi |}  [\langle
\psi |] has a corresponding ket      |  &#x03C8; &#x27E9;   {\displaystyle
|\psi \rangle }  [|\psi \rangle ], and the latter is unique.
***** References[edit] *****
    * M. FrÃ©chet (1907). Sur les ensembles de fonctions et les opÃ©rations
      linÃ©aires. C._R._Acad._Sci._Paris 144, 1414–1416.
    * F. Riesz (1907). Sur une espÃ¨ce de gÃ©omÃ©trie analytique des systÃ¨mes
      de fonctions sommables. C. R. Acad. Sci. Paris 144, 1409–1411.
    * F. Riesz (1909). Sur les opÃ©rations fonctionnelles linÃ©aires. C. R.
      Acad. Sci. Paris 149, 974–977.
    * P._Halmos Measure Theory, D. van Nostrand and Co., 1950.
    * P. Halmos, A Hilbert Space Problem Book, Springer, New York 1982 (problem
      3 contains version for vector spaces with coordinate systems).
    * Walter Rudin, Real and Complex Analysis, McGraw-Hill, 1966,
ISBN 0-07-100276-6.
"Proof_of_Riesz_representation_theorem_for_separable_Hilbert_spaces".
PlanetMath.
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
                       * Riesz representation
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
index.php?title=Riesz_representation_theorem&oldid=894919127"
Categories:
    * Theorems_in_functional_analysis
    * Duality_theories
    * Integral_representations
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 30 April 2019, at 20:47 (UTC).
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
