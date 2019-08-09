The following text has been accessed from https://en.wikipedia.org/wiki/Stone%E2%80%93Weierstrass_theorem at Fri Aug 9 02:35:09 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** StoneâWeierstrass theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematical_analysis, the Weierstrass approximation theorem states that
every continuous_function defined on a closed interval [a, b] can be uniformly
approximated as closely as desired by a polynomial function. Because
polynomials are among the simplest functions, and because computers can
directly evaluate polynomials, this theorem has both practical and theoretical
relevance, especially in polynomial_interpolation. The original version of this
result was established by Karl_Weierstrass in 1885 using the Weierstrass
transform.
Marshall_H._Stone considerably generalized the theorem (Stone_1937) and
simplified the proof (Stone_1948). His result is known as the
StoneâWeierstrass theorem. The StoneâWeierstrass theorem generalizes the
Weierstrass approximation theorem in two directions both regressive and
progressive: instead of the real interval [a, b], an arbitrary compact
Hausdorff_space X is considered, and instead of the algebra of polynomial
functions, approximation with elements from more general subalgebras of C(X) is
investigated. The StoneâWeierstrass theorem is a vital result in the study of
the algebra of continuous_functions_on_a_compact_Hausdorff_space.
Further, there is a generalization of the StoneâWeierstrass theorem to
noncompact Tychonoff_spaces, namely, any continuous function on a Tychonoff
space is approximated uniformly_on_compact_sets by algebras of the type
appearing in the StoneâWeierstrass theorem and described below.
A different generalization of Weierstrass' original theorem is Mergelyan's
theorem, which generalizes it to functions defined on certain subsets of the
complex_plane.
⁰
***** Contents *****
    * 1_Weierstrass_approximation_theorem
          o 1.1_Applications
    * 2_StoneâWeierstrass_theorem,_real_version
          o 2.1_Locally_compact_version
          o 2.2_Applications
    * 3_StoneâWeierstrass_theorem,_complex_version
    * 4_StoneâWeierstrass_theorem,_quaternion_version
    * 5_StoneâWeierstrass_theorem,_C*-algebra_version
    * 6_Lattice_versions
    * 7_Bishop's_theorem
    * 8_Nachbin's_theorem
    * 9_See_also
    * 10_Notes
    * 11_References
          o 11.1_Historical_works
    * 12_External_links
***** Weierstrass approximation theorem[edit] *****
The statement of the approximation theorem as originally discovered by
Weierstrass is as follows:
      Weierstrass Approximation Theorem. Suppose âfâ is a continuous real-
      valued function defined on the real interval [a, b]. For every Îµ > 0,
      there exists a polynomial p such that for all x in [a, b], we have
      |âfâ(x) â p(x)| < Îµ, or equivalently, the supremum_norm ||âfâ
      â p|| < Îµ.
A constructive proof of this theorem using Bernstein_polynomials is outlined on
that page.
**** Applications[edit] ****
As a consequence of the Weierstrass approximation theorem, one can show that
the space C[a, b] is separable: the polynomial functions are dense, and each
polynomial function can be uniformly approximated by one with rational
coefficients; there are only countably_many polynomials with rational
coefficients. Since C[a, b] is Hausdorff and separable it follows that C[a, b]
has cardinality equal to 2âµ0 â the same cardinality as the cardinality_of
the_reals. (Remark: This cardinality result also follows from the fact that a
continuous function on the reals is uniquely determined by its restriction to
the rationals.)
***** StoneâWeierstrass theorem, real version[edit] *****
The set C[a, b] of continuous real-valued functions on [a, b], together with
the supremum norm ||âfâ|| = supa â¤ x â¤ b |âfâ(x)|, is a Banach
algebra, (that is, an associative_algebra and a Banach_space such that
||âfg|| â¤ ||âfâ||Â·||g|| for all âf, g). The set of all polynomial
functions forms a subalgebra of C[a, b] (that is, a vector_subspace of C[a, b]
that is closed under multiplication of functions), and the content of the
Weierstrass approximation theorem is that this subalgebra is dense in C[a, b].
Stone starts with an arbitrary compact Hausdorff space X and considers the
algebra C(X, R) of real-valued continuous functions on X, with the topology of
uniform_convergence. He wants to find subalgebras of C(X, R) which are dense.
It turns out that the crucial property that a subalgebra must satisfy is that
it separates_points: a set A of functions defined on X is said to separate
points if, for every two different points x and y in X there exists a function
p in A with p(x) â  p(y). Now we may state:
      StoneâWeierstrass Theorem (real numbers). Suppose X is a compact
      Hausdorff space and A is a subalgebra of C(X, R) which contains a non-
      zero constant function. Then A is dense in C(X, R) if_and_only_if it
      separates points.
This implies Weierstrassâ original statement since the polynomials on [a, b]
form a subalgebra of C[a, b] which contains the constants and separates points.
**** Locally compact version[edit] ****
A version of the StoneâWeierstrass theorem is also true when X is only
locally_compact. Let C0(X, R) be the space of real-valued continuous functions
on X which vanish_at_infinity; that is, a continuous function âfâ is in C0
(X, R) if, for every Îµ > 0, there exists a compact set K â X such that â|
f |â < Îµ on X \ K. Again, C0(X, R) is a Banach_algebra with the supremum
norm. A subalgebra A of C0(X, R) is said to vanish nowhere if not all of the
elements of A simultaneously vanish at a point; that is, for every x in X,
there is some âfâ in A such that âfâ(x) â  0. The theorem generalizes
as follows:
      StoneâWeierstrass Theorem (locally compact spaces). Suppose X is a
      locally compact Hausdorff space and A is a subalgebra of C0(X, R). Then A
      is dense in C0(X, R) (given the topology of uniform_convergence) if and
      only if it separates points and vanishes nowhere.
This version clearly implies the previous version in the case when X is
compact, since in that case C0(X, R) = C(X, R). There are also more general
versions of the StoneâWeierstrass that weaken the assumption of local
compactness.[1]
**** Applications[edit] ****
The StoneâWeierstrass theorem can be used to prove the following two
statements which go beyond Weierstrass's result.
    * If âfâ is a continuous real-valued function defined on the set [a, b]
      Ã [c, d] and Îµ > 0, then there exists a polynomial function p in two
      variables such that |âfâ(x, y) â p(x, y)â| < Îµ for all x in [a,
      b] and y in [c, d].[citation_needed]
    * If X and Y are two compact Hausdorff spaces and f : X Ã Y â R is a
      continuous function, then for every Îµ > 0 there exist n > 0 and
      continuous functions âf1, ..., âfnâ on X and continuous functions
      g1, ..., gn on Y such that ||âf â â fiâgiâ|| < Îµ.[citation
      needed]
The theorem has many other applications to analysis, including:
    * Fourier_series: The set of linear combinations of functions en(x) =
      e2Ïinx, n â Z is dense in C([0, 1]/{0, 1}), where we identify the
      endpoints of the interval [0, 1] to obtain a circle. An important
      consequence of this is that the en are an orthonormal_basis of the space
      L2([0,_1]) of square-integrable_functions on [0, 1].
***** StoneâWeierstrass theorem, complex version[edit] *****
Slightly more general is the following theorem, where we consider the algebra C
(X, C) of complex-valued continuous functions on the compact space X, again
with the topology of uniform convergence. This is a C*-algebra with the *-
operation given by pointwise complex_conjugation.
      StoneâWeierstrass Theorem (complex numbers). Let X be a compact
      Hausdorff space and let S be a subset of C(X, C) which separates_points.
      Then the complex unital *-algebra generated by S is dense in C(X, C).
The complex unital *-algebra generated by S consists of all those functions
that can be obtained from the elements of S by throwing in the constant
function 1 and adding them, multiplying them, conjugating them, or multiplying
them with complex scalars, and repeating finitely many times.
This theorem implies the real version, because if a sequence of complex-valued
functions uniformly approximate a given function âfâ, then the real parts
of those functions uniformly approximate the real part of âfâ. As in the
real case, an analog of this theorem is true for locally compact Hausdorff
spaces.
***** StoneâWeierstrass theorem, quaternion version[edit] *****
Following John_C.Holladay_(1957) : consider the algebra C(X, H) of quaternion-
valued continuous functions on the compact space X, again with the topology of
uniform convergence. If a quaternion q is written in the form
q = a + ib;+ jc + kd then the scalar part a is the real number
(q â iqi â jqj â kqk)/4. Likewise being the scalar part of âqi, âqj
and âqk : b,c and d are respectively the real numbers
(âqi â iq + jqk â kqj)/4, (âqj â iqk â jq + kqi)/4 and
(âqk + iqj â jqk â kq)/4. Then we may state :
      StoneâWeierstrass Theorem (quaternion numbers). Suppose X is a compact
      Hausdorff space and A is a subalgebra of C(X, H) which contains a non-
      zero constant function. Then A is dense in C(X, H) if and only if it
      separates_points.
***** StoneâWeierstrass theorem, C*-algebra version[edit] *****
The space of complex-valued continuous functions on a compact Hausdorff space X
i.e. C(X, C) is the canonical example of a unital commutative_C*-algebra
A     {\displaystyle {\mathfrak {A}}}  [{\mathfrak {A}}]. The space X may be
viewed as the space of pure states on       A     {\displaystyle {\mathfrak
{A}}}  [{\mathfrak {A}}], with the weak-* topology. Following the above cue, a
non-commutative extension of the StoneâWeierstrass theorem, which has remain
unsolved, is as follows:
      Conjecture. If a unital C*-algebra       A     {\displaystyle {\mathfrak
      {A}}}  [{\mathfrak {A}}] has a C*-subalgebra       B     {\displaystyle
      {\mathfrak {B}}}  [{\mathfrak {B}}] which separates the pure states of
      A     {\displaystyle {\mathfrak {A}}}  [{\mathfrak {A}}], then       A
      =   B     {\displaystyle {\mathfrak {A}}={\mathfrak {B}}}  [{\mathfrak
      {A}}={\mathfrak  {B}}].
In 1960, Jim Glimm proved a weaker version of the above conjecture.
      StoneâWeierstrass theorem (C*-algebras).[2] If a unital C*-algebra
      A     {\displaystyle {\mathfrak {A}}}  [{\mathfrak {A}}] has a C*-
      subalgebra       B     {\displaystyle {\mathfrak {B}}}  [{\mathfrak {B}}]
      which separates the pure state space (i.e. the weak-* closure of the pure
      states) of       A     {\displaystyle {\mathfrak {A}}}  [{\mathfrak
      {A}}], then       A   =   B     {\displaystyle {\mathfrak {A}}={\mathfrak
      {B}}}  [{\mathfrak  {A}}={\mathfrak  {B}}].
***** Lattice versions[edit] *****
Let X be a compact Hausdorff space. Stone's original proof of the theorem used
the idea of lattices in C(X, R). A subset L of C(X, R) is called a lattice if
for any two elements âf, g â L, the functions max{âf, g}, min{âf, g}
also belong to L. The lattice version of the StoneâWeierstrass theorem
states:
      StoneâWeierstrass Theorem (lattices). Suppose X is a compact Hausdorff
      space with at least two points and L is a lattice in C(X, R) with the
      property that for any two distinct elements x and y of X and any two real
      numbers a and b there exists an element âfâ â L with âfâ(x) = a
      and âfâ(y) = b. Then L is dense in C(X, R).
The above versions of StoneâWeierstrass can be proven from this version once
one realizes that the lattice property can also be formulated using the
absolute_value |âfâ| which in turn can be approximated by polynomials in
âfâ. A variant of the theorem applies to linear subspaces of C(X, R) closed
under max (Hewitt_&_Stromberg_1965, Theorem 7.29):
      StoneâWeierstrass Theorem. Suppose X is a compact Hausdorff space and B
      is a family of functions in C(X, R) such that
         1. B separates points.
         2. B contains the constant function 1.
         3. If âfâ â B then afâ â B for all constants a â R.
         4. If âf,â g â B, then âfâ + g, max{âf, g} â B.
      Then B is dense in C(X, R).
More precise information is available:
      Suppose X is a compact Hausdorff space with at least two points and L is
      a lattice in C(X, R). The function Ï â C(X, R) belongs to the closure
      of L if and only if for each pair of distinct points x and y in X and for
      each Îµ > 0 there exists some âfâ â L for which |âfâ(x) â Ï
      (x)| < Îµ and |âfâ(y) â Ï(y)| < Îµ.
***** Bishop's theorem[edit] *****
Another generalization of the StoneâWeierstrass theorem is due to Errett
Bishop. Bishop's theorem is as follows (Bishop_1961):
      Let A be a closed subalgebra of the Banach_space C(X, C) of continuous
      complex-valued functions on a compact Hausdorff space X. Suppose that
      âfâ â C(X, C) has the following property:
            âfâ|S â AS for every maximal set S â X such that all real
            functions of AS are constant.
      Then âfâ â A.
Glicksberg_(1962) gives a short proof of Bishop's theorem using the
KreinâMilman_theorem in an essential way, as well as the HahnâBanach
theorem : the process of Louis_de_Branges_(1959). See also Rudin_(1973, Â§5.7).
***** Nachbin's theorem[edit] *****
Nachbin's theorem gives an analog for StoneâWeierstrass theorem for algebras
of complex valued smooth functions on a smooth manifold (Nachbin_1949).
Nachbin's theorem is as follows (Llavona_1986):
      Let A be a subalgebra of the algebra Câ(M) of smooth functions on a
      finite dimensional smooth manifold M. Suppose that A separates the points
      of M and also separates the tangent vectors of M: for each point m â M
      and tangent vector v at the tangent space at m, there is a f â A such
      that df(x)(v) â  0. Then A is dense in Câ(M).
***** See also[edit] *****
    * MÃ¼ntzâSzÃ¡sz_theorem.
    * Bernstein_polynomial.
    * Runge's_phenomenon shows that finding a polynomial P such that âfâ(x)
      = P(x) for some finely spaced x = xn is a bad way to attempt to find a
      polynomial approximating âfâ uniformly. However, as is shown in
      Walter_Rudin's Principles of Mathematical Analysis, one can easily find a
      polynomial P uniformly approximating âfâ by convolving âfâ with a
      polynomial kernel.
    * Mergelyan's_theorem, concerning polynomial approximations of complex
      functions.
***** Notes[edit] *****
   1. ^Willard, Stephen (1970). General Topology. Addison-Wesley. p. 293.
      ISBN 0-486-43479-6.
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
   3. ^Glimm,_James (1960). "A StoneâWeierstrass Theorem for C*-algebras".
      Annals_of_Mathematics. Second Series. 72 (2): 216â244 [Theorem 1]. doi:
      10.2307/1970133. JSTOR 1970133.
***** References[edit] *****
    * John C.Holladay (1957), "The_StoneâWeierstrass_theorem_for_quaternions"
      (PDF), Proc. Amer. Math. Soc., 8: 656, doi:10.1090/S0002-9939-1957-
      0087047-7
.
Louis_de_Branges (1959), "The StoneâWeierstrass theorem", Proc. Amer. Math.
Soc., 10: 822â824, doi:10.1090/s0002-9939-1959-0113131-7
.
Jan_Brinkhuis & Vladimir Tikhomirov (2005) Optimization: Insights and
Applications, Princeton_University_Press
ISBN 978-0-691-10287-0 MR
2168305.
Glimm, James (1960), "A StoneâWeierstrass Theorem for C*-algebras", Annals of
Mathematics, Second Series, 72 (2): 216â244, doi:10.2307/1970133,
JSTOR 1970133
Bishop, Errett (1961), "A_generalization_of_the_StoneâWeierstrass_theorem",
Pacific Journal of Mathematics, 11 (3): 777â783, doi:10.2140/pjm.1961.11.777
.
Glicksberg, Irving (1962), "Measures Orthogonal to Algebras and Sets of
Antisymmetry", Transactions of the American Mathematical Society, Transactions
of the American Mathematical Society, Vol. 105, No. 3, 105 (3): 415â435, doi:
10.2307/1993729, JSTOR 1993729
.
Hewitt, E; Stromberg, K (1965), Real and abstract analysis, Springer-Verlag
.
Rudin,_Walter (1976), Principles of mathematical analysis (3rd. ed.), McGraw-
Hill, ISBN 978-0-07-054235-8
.
Rudin,_Walter (1973), Functional analysis, McGraw-Hill, ISBN 0-07-054236-8
.
Nachbin, L. (1949), "Sur les algÃ¨bres denses de fonctions diffÃ¨rentiables sur
une variÃ©tÃ©", C. R. Acad. Sci. Paris, 228: 1549â1551
Llavona, JosÃ© G. (1986), Approximation of continuously differentiable
functions, Amsterdam: North-Holland, ISBN 9780080872414
JG Burkill, Lectures_On_Approximation_By_Polynomials (PDF)
.
**** Historical works[edit] ****
The historical publication of Weierstrass (in German_language) is freely
available from the digital online archive of the Berlin_Brandenburgische
Akademie_der_Wissenschaften:
    * K. Weierstrass (1885). Ãber die analytische Darstellbarkeit sogenannter
      willkÃ¼rlicher Functionen einer reellen VerÃ¤nderlichen. Sitzungsberichte
      der KÃ¶niglich PreuÃischen Akademie der Wissenschaften zu Berlin, 1885
      (II).
      Erste_Mitteilung (part 1) pp. 633â639, Zweite_Mitteilung (part 2) pp.
      789â805.
Important historical works of Stone include:
    * Stone,_M._H. (1937), "Applications of the Theory of Boolean Rings to
      General Topology", Transactions of the American Mathematical Society,
      Transactions of the American Mathematical Society, Vol. 41, No. 3, 41
      (3): 375â481, doi:10.2307/1989788, JSTOR 1989788
.
Stone,_M._H. (1948), "The Generalized Weierstrass Approximation Theorem",
Mathematics Magazine, 21 (4): 167â184, doi:10.2307/3029750, JSTOR 3029750
; 21 (5), 237â254.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "StoneâWeierstrass_theorem",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
                                              * BNF: cb15014506g (data)
Authority_control [Edit_this_at_Wikidata]     * GND: 4341745-0
                                              * LCCN: sh94005265
                                              * SUDOC: 092475205

Retrieved from "https://en.wikipedia.org/w/
index.php?title=StoneâWeierstrass_theorem&oldid=867254821"
Categories:
    * Continuous_mappings
    * Theorems_in_analysis
    * Theorems_in_approximation_theory
    * 1885_in_mathematics
    * 1937_in_mathematics
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_July_2018
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_SUDOC_identifiers
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
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * ä¸­æ
Edit_links
    * This page was last edited on 4 November 2018, at 17:02 (UTC).
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
