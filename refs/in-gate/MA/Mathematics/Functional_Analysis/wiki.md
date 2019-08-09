The following text has been accessed from https://en.wikipedia.org/wiki/Functional_analysis at Fri Aug 9 02:38:35 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Functional analysis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For the assessment and treatment of human behavior, see Functional_analysis_
(psychology).
One of the possible modes of vibration of an idealized circular drum_head.
These modes are eigenfunctions of a linear operator on a function space, a
common construction in functional analysis.
Functional analysis is a branch of mathematical_analysis, the core of which is
formed by the study of vector_spaces endowed with some kind of limit-related
structure (e.g. inner_product, norm, topology, etc.) and the linear_functions
defined on these spaces and respecting these structures in a suitable sense.
The historical roots of functional analysis lie in the study of spaces_of
functions and the formulation of properties of transformations of functions
such as the Fourier_transform as transformations defining continuous, unitary
etc. operators between function spaces. This point of view turned out to be
particularly useful for the study of differential and integral_equations.
The usage of the word functional as a noun goes back to the calculus_of
variations, implying a function_whose_argument_is_a_function. The term was
first used in Hadamard's 1910 book on that subject. However, the general
concept of a functional had previously been introduced in 1887 by the Italian
mathematician and physicist Vito_Volterra.[1][2] The theory of nonlinear
functionals was continued by students of Hadamard, in particular FrÃ©chet and
LÃ©vy. Hadamard also founded the modern school of linear functional analysis
further developed by Riesz and the group of Polish mathematicians around Stefan
Banach.
In modern introductory texts to functional analysis, the subject is seen as the
study of vector spaces endowed with a topology, in particular infinite-
dimensional_spaces. In contrast, linear_algebra deals mostly with finite-
dimensional spaces, and does not use topology. An important part of functional
analysis is the extension of the theory of measure, integration, and
probability to infinite dimensional spaces, also known as infinite dimensional
analysis.
⁰
***** Contents *****
    * 1_Normed_vector_spaces
          o 1.1_Hilbert_spaces
          o 1.2_Banach_spaces
    * 2_Major_and_foundational_results
          o 2.1_Uniform_boundedness_principle
          o 2.2_Spectral_theorem
          o 2.3_HahnâBanach_theorem
          o 2.4_Open_mapping_theorem
          o 2.5_Closed_graph_theorem
          o 2.6_Other_topics
    * 3_Foundations_of_mathematics_considerations
    * 4_Points_of_view
    * 5_See_also
    * 6_References
    * 7_Further_reading
    * 8_External_links
***** Normed vector spaces[edit] *****
The basic and historically first class of spaces studied in functional analysis
are complete normed_vector_spaces over the real or complex_numbers. Such spaces
are called Banach_spaces. An important example is a Hilbert_space, where the
norm arises from an inner product. These spaces are of fundamental importance
in many areas, including the mathematical_formulation_of_quantum_mechanics.
More generally, functional analysis includes the study of FrÃ©chet_spaces and
other topological_vector_spaces not endowed with a norm.
An important object of study in functional analysis are the continuous linear
operators defined on Banach and Hilbert spaces. These lead naturally to the
definition of C*-algebras and other operator_algebras.
**** Hilbert spaces[edit] ****
Hilbert_spaces can be completely classified: there is a unique Hilbert space up
to isomorphism for every cardinality of the orthonormal_basis.[3] Finite-
dimensional Hilbert spaces are fully understood in linear_algebra, and
infinite-dimensional separable Hilbert spaces are isomorphic to ____&#x2113;
2___(__&#x2135;__0___)____{\displaystyle_\ell_^{\,2}(\aleph__{0})\,}__[\ell^
{\,2}(\aleph_0)\,]. Separability being important for applications, functional
analysis of Hilbert spaces consequently mostly deals with this space. One of
the open problems in functional analysis is to prove that every bounded linear
operator on a Hilbert space has a proper invariant_subspace. Many special cases
of this invariant_subspace_problem have already been proven.
**** Banach spaces[edit] ****
General Banach_spaces are more complicated than Hilbert spaces, and cannot be
classified in such a simple manner as those. In particular, many Banach spaces
lack a notion analogous to an orthonormal_basis.
Examples of Banach spaces are ____L___p_____{\displaystyle_L^{\,p}}__[L^{\,p}]-
spaces for any real number     p &#x2265; 1   {\displaystyle p\geq 1}  [p\geq
1] . Given also a measure     &#x03BC;   {\displaystyle \mu }  [\mu ] on set
X   {\displaystyle X}  [X], then      L   p   ( X )   {\displaystyle L^{\,p}
(X)}  [L^{\,p}(X)], sometimes also denoted      L   p   ( X , &#x03BC; )
{\displaystyle L^{\,p}(X,\mu )}  [L^{\,p}(X,\mu)] or      L   p   ( &#x03BC; )
{\displaystyle L^{\,p}(\mu )}  [L^{\,p}(\mu)], has as its vectors equivalence
classes     [  f  ]   {\displaystyle [\,f\,]}  [[\,f\,]] of measurable
functions whose absolute_value's     p   {\displaystyle p}  [p]-th power has
finite integral, that is, functions     f    {\displaystyle f\,}  [f\,] for
which one has
          &#x222B;  X     |  f ( x )  |   p    d &#x03BC; ( x ) < + &#x221E;
      {\displaystyle \int _{X}\left|f(x)\right|^{p}\,d\mu (x)<+\infty }  [\int_
      {X}\left|f(x)\right|^p\,d\mu(x)<+\infty].
If     &#x03BC;   {\displaystyle \mu }  [\mu ] is the counting_measure, then
the integral may be replaced by a sum. That is, we require
          &#x2211;  x &#x2208; X     |  f ( x )  |   p   < + &#x221E;
      {\displaystyle \sum _{x\in X}\left|f(x)\right|^{p}<+\infty }  [\sum_{x\in
      X}\left|f(x)\right|^p<+\infty].
Then it is not necessary to deal with equivalence classes, and the space is
denoted      &#x2113;  &#xA0; p   ( X )   {\displaystyle \ell ^{\ p}(X)}
[\ell^{\ p}(X)], written more simply       &#x2113;   p &#xA0;
{\displaystyle \,\ell ^{\,p\ }}  [\,\ell^{\,p\ }] in the case when     X
{\displaystyle X}  [X] is the set of non-negative integers.
In Banach spaces, a large part of the study involves the dual_space: the space
of all continuous linear maps from the space into its underlying field, so-
called functionals. A Banach space can be canonically identified with a
subspace of its bidual, which is the dual of its dual space. The corresponding
map is an isometry but in general not onto. A general Banach space and its
bidual need not even be isometrically isomorphic in any way, contrary to the
finite-dimensional situation. This is explained in the dual space article.
Also, the notion of derivative can be extended to arbitrary functions between
Banach spaces. See, for instance, the FrÃ©chet_derivative article.
***** Major and foundational results[edit] *****
Important results of functional analysis include:
**** Uniform boundedness principle[edit] ****
Main article: Banach-Steinhaus_theorem
The uniform_boundedness_principle or BanachâSteinhaus_theorem is one of the
fundamental results in functional analysis. Together with the HahnâBanach
theorem and the open_mapping_theorem, it is considered one of the cornerstones
of the field. In its basic form, it asserts that for a family of continuous
linear_operators (and thus bounded operators) whose domain is a Banach_space,
pointwise boundedness is equivalent to uniform boundedness in operator norm.
The theorem was first published in 1927 by Stefan_Banach and Hugo_Steinhaus but
it was also proven independently by Hans_Hahn.
     Theorem (Uniform Boundedness Principle). Let X be a Banach_space and
     Y be a normed_vector_space. Suppose that F is a collection of
     continuous linear operators from X to Y. If for all x in X one has
               sup  T &#x2208; F   &#x2016; T ( x )  &#x2016;  Y   <
           &#x221E; ,   {\displaystyle \sup \nolimits _{T\in F}\|T(x)\|_
           {Y}<\infty ,}  [\sup\nolimits_{T \in F} \|T(x)\|_Y  < \infty, ]
     then
               sup  T &#x2208; F   &#x2016; T  &#x2016;  B ( X , Y )   <
           &#x221E; .   {\displaystyle \sup \nolimits _{T\in F}\|T\|_{B
           (X,Y)}<\infty .}  [\sup\nolimits_{T \in F} \|T\|_{B(X,Y)}  <
           \infty.]
**** Spectral theorem[edit] ****
Main article: Spectral_theorem
There are many theorems known as the spectral_theorem, but one in particular
has many applications in functional analysis.
Theorem:[4] Let A be a bounded self-adjoint operator on a Hilbert space H. Then
there is a measure_space (X, Σ, μ) and a real-valued essentially_bounded
measurable function f on X and a unitary operator U:H → L2μ(X) such that
          U  &#x2217;   T U = A    {\displaystyle U^{*}TU=A\;}  [ U^* T U = A
      \;]
where T is the multiplication_operator:
         [ T &#x03C6; ] ( x ) = f ( x ) &#x03C6; ( x ) .    {\displaystyle
      [T\varphi ](x)=f(x)\varphi (x).\;}  [ [T \varphi](x) = f(x) \varphi(x).
      \;]
and     &#x2016; T &#x2016; = &#x2016; f  &#x2016;  &#x221E;     {\displaystyle
\|T\|=\|f\|_{\infty }}  [\|T\|=\|f\|_{\infty }]
This is the beginning of the vast research area of functional analysis called
operator_theory; see also the spectral_measure.
There is also an analogous spectral theorem for bounded normal_operators on
Hilbert spaces. The only difference in the conclusion is that now     f
{\displaystyle f}  [f] may be complex-valued.
**** HahnâBanach theorem[edit] ****
Main article: HahnâBanach_theorem
The HahnâBanach_theorem is a central tool in functional analysis. It allows
the extension of bounded_linear_functionals defined on a subspace of some
vector_space to the whole space, and it also shows that there are "enough"
continuous linear functionals defined on every normed_vector_space to make the
study of the dual_space "interesting".
HahnâBanach theorem:[5] If p : V â R is a sublinear_function, and Ï : U
â R is a linear_functional on a linear_subspace U â V which is dominated by
p on U, i.e.
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
**** Open mapping theorem[edit] ****
Main article: Open_mapping_theorem_(functional_analysis)
The open_mapping_theorem, also known as the BanachâSchauder theorem (named
after Stefan_Banach and Juliusz_Schauder), is a fundamental result which states
that if a continuous_linear_operator between Banach_spaces is surjective then
it is an open_map. More precisely,:[5]
      Open mapping theorem. If X and Y are Banach spaces and A : X â Y is a
      surjective continuous linear operator, then A is an open map (i.e. if U
      is an open_set in X, then A(U) is open in Y).
The proof uses the Baire_category_theorem, and completeness of both X and Y is
essential to the theorem. The statement of the theorem is no longer true if
either space is just assumed to be a normed_space, but is true if X and Y are
taken to be FrÃ©chet_spaces.
**** Closed graph theorem[edit] ****
Main article: Closed_graph_theorem
The closed graph theorem states the following: If X is a topological_space and
Y is a compact Hausdorff_space, then the graph of a linear map T from X to Y is
closed if and only if T is continuous.[6]
**** Other topics[edit] ****
Main article: List_of_functional_analysis_topics
***** Foundations of mathematics considerations[edit] *****
Most spaces considered in functional analysis have infinite dimension. To show
the existence of a vector_space_basis for such spaces may require Zorn's_lemma.
However, a somewhat different concept, Schauder_basis, is usually more relevant
in functional analysis. Many very important theorems require the HahnâBanach
theorem, usually proved using axiom_of_choice, although the strictly weaker
Boolean_prime_ideal_theorem suffices. The Baire_category_theorem, needed to
prove many important theorems, also requires a form of axiom of choice.
***** Points of view[edit] *****
Functional analysis in its present form[update] includes the following
tendencies:
    * Abstract analysis. An approach to analysis based on topological_groups,
      topological_rings, and topological_vector_spaces.
    * Geometry of Banach_spaces contains many topics. One is combinatorial
      approach connected with Jean_Bourgain; another is a characterization of
      Banach spaces in which various forms of the law_of_large_numbers hold.
    * Noncommutative_geometry. Developed by Alain_Connes, partly building on
      earlier notions, such as George_Mackey's approach to ergodic_theory.
    * Connection with quantum_mechanics. Either narrowly defined as in
      mathematical_physics, or broadly interpreted by, e.g. Israel_Gelfand, to
      include most types of representation_theory.
***** See also[edit] *****
    * List_of_functional_analysis_topics
    * Spectral_theory
***** References[edit] *****
   1. ^ acsu.buffalo.edu
   2. ^ History of the Mathematical Sciences
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
   4. ISBN 978-93-86279-16-3 p. 195
   5. ^Riesz, Frigyes; SzÅkefalvi-Nagy, BÃ©la (1990). Functional analysis
      (Dover ed.). New York: Dover Publications. pp. 195â199. ISBN 978-0-486-
      66289-3.
   6. ^Hall, B.C. (2013), Quantum Theory for Mathematicians, Springer, p. 147
   7. ^ a bRudin,_Walter (1991). Functional analysis. McGraw-Hill Science/
      Engineering/Math. ISBN 978-0-07-054236-5.
   8. ^Munkres,_James (2000), Topology (2nd ed.), Upper_Saddle_River:_Prentice
      Hall, pp. 163â172, ISBN 0-13-181629-2
   9. , p. 171
***** Further reading[edit] *****
    * Aliprantis, C.D., Border, K.C.: Infinite Dimensional Analysis: A
      Hitchhiker's Guide, 3rd ed., Springer 2007,
ISBN 978-3-540-32696-0. Online doi:10.1007/3-540-29587-9 (by subscription)
Bachman, G., Narici, L.: Functional analysis, Academic Press, 1966. (reprint
Dover Publications)
Banach_S. Theory_of_Linear_Operations. Volume 38, North-Holland Mathematical
Library, 1987,
ISBN 0-444-70184-2
Brezis,_H.: Analyse Fonctionnelle, Dunod
ISBN 978-2-10-004314-9 or
ISBN 978-2-10-049336-4
Conway,_J._B.: A Course in Functional Analysis, 2nd edition, Springer-Verlag,
1994,
ISBN 0-387-97245-5
Dunford,_N. and Schwartz,_J.T.: Linear Operators, General Theory, John Wiley &
Sons, and other 3 volumes, includes visualization charts
Edwards, R. E.: Functional Analysis, Theory and Applications, Hold, Rinehart
and Winston, 1965.
Eidelman, Yuli, Vitali Milman, and Antonis Tsolomitis: Functional Analysis: An
Introduction, American Mathematical Society, 2004.
Friedman,_A.: Foundations of Modern Analysis, Dover Publications, Paperback
Edition, July 21, 2010
Giles,J.R.: Introduction to the Analysis of Normed Linear Spaces,Cambridge
University Press,2000
Hirsch F., Lacombe G. - "Elements of Functional Analysis", Springer 1999.
Hutson, V., Pym, J.S., Cloud M.J.: Applications of Functional Analysis and
Operator Theory, 2nd edition, Elsevier Science, 2005,
ISBN 0-444-51790-1
Kantorovitz, S.,Introduction to Modern Analysis, Oxford University
Press,2003,2nd ed.2006.
Kolmogorov,_A.N and Fomin,_S.V.: Elements of the Theory of Functions and
Functional Analysis, Dover Publications, 1999
Kreyszig,_E.: Introductory Functional Analysis with Applications, Wiley, 1989.
Lax,_P.: Functional Analysis, Wiley-Interscience, 2002,
ISBN 0-471-55604-1
Lebedev, L.P. and Vorovich, I.I.: Functional Analysis in Mechanics, Springer-
Verlag, 2002
Michel, Anthony N. and Charles J. Herget: Applied Algebra and Functional
Analysis, Dover, 1993.
Pietsch, Albrecht: History of Banach spaces and linear operators, BirkhÃ¤user
Boston Inc., 2007,
ISBN 978-0-8176-4367-6
Reed,_M., Simon,_B.: "Functional Analysis", Academic Press 1980.
Riesz, F. and Sz.-Nagy, B.: Functional Analysis, Dover Publications, 1990
Rudin,_W.: Functional Analysis, McGraw-Hill Science, 1991
Saxe, Karen: Beginning Functional Analysis, Springer, 2001
Schechter, M.: Principles of Functional Analysis, AMS, 2nd edition, 2001
Shilov, Georgi E.: Elementary Functional Analysis, Dover, 1996.
Sobolev,_S.L.: Applications of Functional Analysis in Mathematical Physics,
AMS, 1963
Vogt, D., Meise, R.: Introduction to Functional Analysis, Oxford University
Press, 1997.
Yosida,_K.: Functional Analysis, Springer-Verlag, 6th edition, 1980
***** External links[edit] *****
Functional analysisat Wikipedia's sister_projects
    * Quotations from Wikiquote
    * Textbooks from Wikibooks
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Functional_analysis",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Topics_in_Real_and_Functional_Analysis by Gerald_Teschl, University of Vienna.
Lecture_Notes_on_Functional_Analysis by Yevgeny Vilensky, New York University.
Lecture_videos_on_functional_analysis by Greg_Morrow from University_of
Colorado_Colorado_Springs
An_Introduction_to_Functional_Analysis on Coursera by John Cagnol from Ecole
Centrale_Paris
    * v
    * t
    * e
Functional analysis (topics)
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
    * v
    * t
    * e
Areas_of_mathematics
                  * Category_theory
                  * Information_theory
Foundations       * Mathematical_logic
                  * Philosophy_of_mathematics
                  * Set_theory
                  * Abstract
Algebra           * Elementary
                  * Linear
                  * Multilinear
                  * Calculus
                  * Real_analysis
Analysis          * Complex_analysis
                  * Differential_equations
                  * Functional analysis
                  * Combinatorics
Discrete          * Graph_theory
                  * Order_theory
                  * Game_theory
                  * Algebraic
                  * Analytic
Geometry          * Differential
                  * Discrete
                  * Euclidean
                  * Finite
                  * Arithmetic
Number_theory     * Algebraic_number_theory
                  * Analytic_number_theory
                  * Diophantine_geometry
                  * Algebraic
Topology          * Differential
                  * Geometric
                  * Control_theory
                  * Mathematical_economics
                  * Mathematical_finance
Applied           * Mathematical_physics
                  * Mathematical_statistics
                  * Probability
                  * Statistics
                  * Computer_science
                  * Theory_of_computation
Computational     * Numerical_analysis
                  * Optimization
                  * Computer_algebra
                  * History_of_mathematics
Others            * Recreational_mathematics
                  * Mathematics_and_art
                  * Mathematics_education
    * [Category] Category
    * [Portal] Portal
    * [Commons page]Commons
    * [WikiProject]WikiProject
                                              * BNE: XX525044
                                              * BNF: cb131627608 (data)
Authority_control [Edit_this_at_Wikidata]     * GND: 4018916-8
                                              * LCCN: sh85052312
                                              * NDL: 00564962
                                              * NKC: ph120399

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Functional_analysis&oldid=909710627"
Categories:
    * Functional_analysis
Hidden categories:
    * Articles_containing_potentially_dated_statements_from_2004
    * All_articles_containing_potentially_dated_statements
    * Wikipedia_articles_with_BNE_identifiers
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
    * Wikipedia_articles_with_NKC_identifiers
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
    * Wikiquote
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * áá¼ááºáá¬áá¬áá¬
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * SlovenÄina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 03:15 (UTC).
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
