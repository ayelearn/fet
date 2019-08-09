The following text has been accessed from https://en.wikipedia.org/wiki/Hahn%E2%80%93Banach_theorem at Fri Aug 9 02:38:57 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** HahnâBanach theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, the HahnâBanach theorem is a central tool in functional
analysis. It allows the extension of bounded_linear_functionals defined on a
subspace of some vector_space to the whole space, and it also shows that there
are "enough" continuous linear functionals defined on every normed_vector_space
to make the study of the dual_space "interesting". Another version of the
HahnâBanach theorem is known as the HahnâBanach separation theorem or the
separating_hyperplane_theorem, and has numerous uses in convex_geometry.
The theorem is named for the mathematicians Hans_Hahn and Stefan_Banach, who
proved it independently in the late 1920s. The special case of the theorem for
the space     C  [  a , b  ]    {\displaystyle C\left[a,b\right]}  [
{\displaystyle C\left[a,b\right]}] of continuous functions on an interval was
proved earlier (in 1912) by Eduard_Helly,[1] and a more general extension
theorem, the M._Riesz_extension_theorem, from which the HahnâBanach theorem
can be derived, was proved in 1923 by Marcel_Riesz.[2]
⁰
***** Contents *****
    * 1_Formulation
    * 2_Important_consequences
    * 3_HahnâBanach_separation_theorem
    * 4_Geometric_HahnâBanach_theorem
    * 5_Relation_to_axiom_of_choice
    * 6_Consequences
          o 6.1_Topological_vector_spaces
          o 6.2_The_dual_space_C[a,_b]*
    * 7_See_also
    * 8_Notes
    * 9_References
***** Formulation[edit] *****
The most general formulation of the theorem needs some preparation. Given a
real vector_space V, a function f : V â R is called sublinear if
    * Positive_homogeneity: f(Î³x) = Î³ f(x) for all Î³ â R+, x â V,
    * Subadditivity: f(x + y) â¤ f(x) + f(y) for all x, y â V.
Every seminorm on V (in particular, every norm on V) is sublinear. Other
sublinear functions can be useful as well, especially Minkowski_functionals of
convex sets.
HahnâBanach theorem (Rudin_1991, Th. 3.2). If p : V â R is a sublinear
function, and Ï : U â R is a linear_functional on a linear_subspace U â V
which is dominated by p on U, i.e.
         &#x03C6; ( x ) &#x2264; p ( x )  &#x2200; x &#x2208; U
      {\displaystyle \varphi (x)\leq p(x)\qquad \forall x\in U}  [\varphi(x)
      \leq p(x)\qquad\forall x \in U]
then there exists a linear extension Ï : V â R of Ï to the whole space V,
i.e., there exists a linear functional Ï such that
         &#x03C8; ( x ) = &#x03C6; ( x )  &#x2200; x &#x2208; U ,
      {\displaystyle \psi (x)=\varphi (x)\qquad \forall x\in U,}  [\psi
      (x)=\varphi(x)\qquad\forall x\in U,]
         &#x03C8; ( x ) &#x2264; p ( x )  &#x2200; x &#x2208; V .
      {\displaystyle \psi (x)\leq p(x)\qquad \forall x\in V.}  [\psi(x) \le p
      (x)\qquad\forall x\in V.]
HahnâBanach theorem (alternative version). Set K = R or C and let V be a K-
vector space with a seminorm p : V â R. If Ï : U â K is a K-linear
functional on a K-linear subspace U of V which is dominated by p on U in
absolute value,
          |  &#x03C6; ( x )  |  &#x2264; p ( x )  &#x2200; x &#x2208; U
      {\displaystyle |\varphi (x)|\leq p(x)\qquad \forall x\in U}  [|\varphi
      (x)|\leq p(x)\qquad\forall x \in U]
then there exists a linear extension Ï : V â K of Ï to the whole space V,
i.e., there exists a K-linear functional Ï such that
         &#x03C8; ( x ) = &#x03C6; ( x )  &#x2200; x &#x2208; U ,
      {\displaystyle \psi (x)=\varphi (x)\qquad \forall x\in U,}  [\psi
      (x)=\varphi(x)\qquad\forall x\in U,]
          |  &#x03C8; ( x )  |  &#x2264; p ( x )  &#x2200; x &#x2208; V .
      {\displaystyle |\psi (x)|\leq p(x)\qquad \forall x\in V.}  [|\psi(x)| \le
      p(x)\qquad\forall x\in V.]
In the complex case of the alternate version, the C-linearity assumptions
demand, in addition to the assumptions for the real case, that for every vector
x â U, we have ix â U and Ï(ix) = iÏ(x).
The extension Ï is in general not uniquely specified by Ï and the proof gives
no explicit method as to how to find Ï. The usual proof for the case of an
infinite dimensional space V uses Zorn's_lemma or, equivalently, the axiom_of
choice. It is now known (see below) that the ultrafilter_lemma, which is
slightly weaker than the axiom of choice, is actually strong enough.
It is possible to relax slightly the subadditivity condition on p, requiring
only that (Reed and Simon, 1980):
         p ( a x + b y ) &#x2264;  |  a  |   p ( x ) +  |  b  |   p ( y ) ,  x
      , y &#x2208; V ,   |  a  |  +  |  b  |  &#x2264; 1.   {\displaystyle p
      (ax+by)\leq |a|\,p(x)+|b|\,p(y),\qquad x,y\in V,\quad |a|+|b|\leq 1.}  [p
      (ax+by)\leq|a| \, p(x) + |b| \, p(y),\qquad x,y\in V,\quad |a|+|b|\leq1.]
It is further possible to relax the positive homogeneity and the subadditivity
conditions on p, requiring only that p is convex (Schechter, 1996).
This reveals the intimate connection between the HahnâBanach theorem and
convexity.
The Mizar_project has completely formalized and automatically checked the proof
of the HahnâBanach theorem in the HAHNBAN file.[3]
***** Important consequences[edit] *****
The theorem has several important consequences, some of which are also
sometimes called "HahnâBanach theorem":
    * If V is a normed vector space with linear subspace U (not necessarily
      closed) and if Ï : U â K is continuous and linear, then there exists
      an extension Ï : V â K of Ï which is also continuous and linear and
      which has the same norm as Ï (see Banach_space for a discussion of the
      norm of a linear map). In other words, in the category of normed vector
      spaces, the space K is an injective_object.
    * If V is a normed vector space with linear subspace U (not necessarily
      closed) and if z is an element of V not in the closure of U, then there
      exists a continuous linear map Ï : V â K with Ï(x) = 0 for all x in
      U, Ï(z) = 1, and ||Ï|| = dist(z, U)â1.
    * In particular, if V is a normed vector space and z is an element of V,
      then there exists a continuous linear map Ï : V â K such that Ï(z) =
      ||z|| and ||Ï|| â¤ 1. This implies that the natural_injection J from a
      normed space V into its double_dual Vâ²â² is isometric.
***** HahnâBanach separation theorem[edit] *****
See also: Hyperplane_separation_theorem
Another version of HahnâBanach theorem is known as the HahnâBanach
separation theorem.[4] It has numerous uses in convex_geometry,[5] optimization
theory, and economics. The separation theorem is derived from the original form
of the theorem.
Theorem. Set K = R or C and let V be a topological_vector_space over K. If A, B
are convex, non-empty disjoint subsets of V, then:
    * If A is open, then there exists a continuous linear map Î» : V â K and
      t â R such that Re(Î»(a)) < t â¤ Re(Î»(b)) for all a â A, b â B.
    * If V is locally convex, A is compact, and B closed, then there exists a
      continuous linear map Î» : V â K and s, t â R such that Re(Î»(a)) < t
      < s < Re(Î»(b)) for all a â A, b â B.
***** Geometric HahnâBanach theorem[edit] *****
One form of HahnâBanach theorem is known as the Geometric HahnâBanach
theorem, or Mazur's theorem.[6]
Theorem. Let K be a convex set having a nonempty interior in a real normed
linear vector space X. Suppose V is a linear variety in X containing no
interior points of K. Then there is a closed hyperplane in X containing V but
containing no interior points of K; i.e., there is an element x* â X* and a
constant c such that     &#x27E8; v ,  x  &#x2217;   &#x27E9; = c
{\displaystyle \langle v,x^{*}\rangle =c}  [{\displaystyle \langle v,x^
{*}\rangle =c}] for all v â V and     &#x27E8; v ,  x  &#x2217;   &#x27E9; <
c   {\displaystyle \langle v,x^{*}\rangle <c}  [{\displaystyle \langle v,x^
{*}\rangle <c}] for all k â int(K).
This can be generalized to an arbitrary topological vector space, which need
not be locally convex or even Hausdorff, as:[7]
Theorem. Let M be a vector subspace of the topological vector space X. Suppose
K is a non-empty convex open subset of X with K â© M = â. Then there is a
closed hyperplane N in X containing M with K â© N = â.
***** Relation to axiom of choice[edit] *****
As mentioned earlier, the axiom_of_choice implies the HahnâBanach theorem.
The converse is not true. One way to see that is by noting that the ultrafilter
lemma (or equivalently, the Boolean prime ideal theorem), which is strictly
weaker than the axiom of choice, can be used to show the HahnâBanach theorem,
although the converse is not the case.
The HahnâBanach theorem is equivalent to the following:[8]
      (â): On every Boolean algebra B there exists a "probability charge",
      that is: a nonconstant finitely additive map from B into [0, 1].
(The Boolean prime ideal theorem is easily seen to be equivalent to the
statement that there are always probability charges which take only the values
0 and 1.)
In ZF, one can show that the HahnâBanach theorem is enough to derive the
existence of a non-Lebesgue measurable set.[9] Moreover, the HahnâBanach
theorem implies the BanachâTarski_paradox.[10]
For separable Banach_spaces, D. K. Brown and S. G. Simpson proved that the
HahnâBanach theorem follows from WKL0, a weak subsystem of second-order
arithmetic that takes a form of KÅnig's_lemma restricted to binary trees as an
axiom. In fact, they prove that under a weak set of assumptions, the two are
equivalent, an example of reverse_mathematics.[11][12]
***** Consequences[edit] *****
**** Topological vector spaces[edit] ****
If X is a topological vector space, not necessarily Hausdorff or locally
convex, then there exists a non-zero continuous linear form if and only if X
contains a nonempty, proper, convex, open set U.[13] So if the continuous dual
space of X, X*, is non-trivial then by considering X with the weak topology
induced by X*, X becomes a locally convex topological vector space with a non-
trivial topology that is weaker than original topology on X. If in addition, X*
separates points on X (which means that for each x â X there is a linear
functional in X* that's non-zero on x) then X with this weak topology becomes
Hausdorff. This sometimes allows some results from locally convex topological
vector spaces to be applied to non-Hausdorff and non-locally convex spaces.
**** The dual space C[a, b]*[edit] ****
We have the following consequence of the HahnâBanach theorem.
Proposition. Let ââ < a < b < â. Then, F â C[a, b]* if and only if
there exists a (complex) measure Ï : [a, b] â R of bounded variation such
that
         F ( u ) =  &#x222B;  a   b   u ( x ) d &#x03C1; ( x ) ,
      {\displaystyle F(u)=\int _{a}^{b}u(x)d\rho (x),}  [F(u)=\int^b_a u
      (x)d\rho(x),]
for all u â C[a, b]. In addition, |F| = V(Ï), where V(Ï) denotes the total
variation of Ï.
***** See also[edit] *****
    * Fichera's_existence_principle
    * M._Riesz_extension_theorem
    * Separating_axis_theorem
    * Farkas'_lemma
***** Notes[edit] *****
   1. ^O'Connor,_John_J.; Robertson,_Edmund_F., "HahnâBanach_theorem",
      MacTutor_History_of_Mathematics_archive, University_of_St_Andrews
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
   3. .
   4. ^ See M._Riesz_extension_theorem. According toGÈ§rding,_L. (1970).
      "Marcel Riesz in memoriam". Acta Math. 124 (1): IâXI. doi:10.1007/
      bf02394565. MR 0256837.
   5. , the argument was known to Riesz already in 1918.
   6. ^ HAHNBAN_file
   7. ^ Gabriel Nagy, Real_Analysis lecture_notes
   8. ^Harvey, R.; Lawson, H. B. (1983). "An intrinsic characterisation of
      KÃ¤hler manifolds". Invent._Math. 74 (2): 169â198. doi:10.1007/
      BF01394312.
   9. ^Luenberger,_David_G. (1969). Optimization_by_Vector_Space_Methods. New
      York: John Wiley & Sons. pp. 131â134. ISBN 978-0-471-18117-0.
  10. ^ Treves, p. 184
  11. ^Schechter, Eric. Handbook of Analysis and its Foundations. p. 620.
  12. ^Foreman, M.; Wehrung, F. (1991). "The_HahnâBanach_theorem_implies_the
      existence_of_a_non-Lebesgue_measurable_set" (PDF). Fundamenta
      Mathematicae. 138: 13â19.
  13. ^Pawlikowski, Janusz (1991). "The Hahn-Banach theorem implies the Banach-
      Tarski paradox". Fundamenta Mathematicae. 138: 21â22.
  14. ^Brown, D. K.; Simpson, S. G. (1986). "Which set existence axioms are
      needed to prove the separable HahnâBanach theorem?". Annals of Pure and
      Applied Logic. 31: 123â144. doi:10.1016/0168-0072(86)90066-7.
  15.  Source_of_citation.
  16. ^ Simpson, Stephen G. (2009), Subsystems of second order arithmetic,
      Perspectives in Logic (2nd ed.), Cambridge University Press,
  17. ISBN 978-0-521-88439-6, MR
  18. 2517689
  19. ^ Schaefer 1999, p. 47
***** References[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Hahn-Banach_theorem",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Narici, Lawrence; Beckenstein, Edward (1997). "The_HahnâBanach_Theorem:_The
Life_and_Times". Topology and its Applications. 77 (2): 193â211. doi:10.1016/
s0166-8641(96)00142-3.
Schmitt, Lothar M (1992). "An_Equivariant_Version_of_the_Hahn-Banach_Theorem".
Houston J. Of Math. 18: 429â447.
Michael Reed and Barry Simon, Methods of Modern Mathematical Physics, Vol. 1,
Functional Analysis, Section III.3. Academic Press, San Diego, 1980.
ISBN 0-12-585050-6.
Eric Schechter, Handbook of Analysis and Its Foundations, Chapter 12, Academic
Press, 1996.
ISBN 0-12-622760-8.
Rudin,_Walter (1991). Functional analysis. McGraw-Hill Science/Engineering/
Math. ISBN 978-0-07-054236-5.
Terence Tao, The_HahnâBanach_theorem,_Mengerâs_theorem,_and_Hellyâs
theorem
TrÃ¨ves, FranÃ§ois (1995). Topological Vector Spaces, Distributions and
Kernels. Dover_Publications. pp. 136â149, 195â201, 240â252, 335â390,
420â433. ISBN 9780486453521.
Gerd Wittstock, Ein operatorwertiger Hahn-Banach Satz, J._of_Functional
Analysis_40_(1981),_127â150
Eberhard Zeidler, Applied Functional Analysis: main principles and their
applications, Springer, 1995.
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

Retrieved from "https://en.wikipedia.org/w/
index.php?title=HahnâBanach_theorem&oldid=904241416"
Categories:
    * Theorems_in_functional_analysis
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
    * AzÉrbaycanca
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 30 June 2019, at 22:12 (UTC).
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
