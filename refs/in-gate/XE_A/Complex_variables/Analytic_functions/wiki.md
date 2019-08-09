The following text has been accessed from https://en.wikipedia.org/wiki/Analytic_function at Fri Aug 9 00:03:37 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Analytic function ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with analytic_expression or analytic_signal.
This article is about both real and complex analytic functions. For analytic
functions in complex analysis specifically, see holomorphic_function.
Mathematical_analysis â Complex analysis
Complex_analysis
[Gamma_abs_3D.png]
Complex_numbers
    * Real_number
    * Imaginary_number
    * Complex_plane
    * Complex_conjugate
    * Unit_complex_number
Complex_functions
    * Complex-valued_function
    * Analytic function
    * Holomorphic_function
    * CauchyâRiemann_equations
    * Formal_power_series
Basic_Theory
    * Zeros_and_poles
    * Cauchy's_integral_theorem
    * Local_primitive
    * Cauchy's_integral_formula
    * Winding_number
    * Laurent_series
    * Isolated_singularity
    * Residue_theorem
    * Conformal_map
    * Schwarz_lemma
    * Harmonic_function
    * Laplace's_equation
Geometric_function_theory
People
    * Augustin-Louis_Cauchy
    * Leonhard_Euler
    * Carl_Friedrich_Gauss
    * Jacques_Hadamard
    * Kiyoshi_Oka
    * Bernhard_Riemann
    * Karl_Weierstrass
    * [Nuvola_apps_kmplot.svg] Analysis_portal
    * v
    * t
    * e
In mathematics, an analytic function is a function that is locally given by a
convergent power_series. There exist both real analytic functions and complex
analytic functions, categories that are similar in some ways, but different in
others. Functions of each type are infinitely_differentiable, but complex
analytic functions exhibit properties that do not hold generally for real
analytic functions. A function is analytic if and only if its Taylor_series
about x0 converges to the function in some neighborhood for every x0 in its
domain.
⁰
***** Contents *****
    * 1_Definitions
    * 2_Examples
    * 3_Alternative_characterizations
    * 4_Properties_of_analytic_functions
    * 5_Analyticity_and_differentiability
    * 6_Real_versus_complex_analytic_functions
    * 7_Analytic_functions_of_several_variables
    * 8_See_also
    * 9_Notes
    * 10_References
    * 11_External_links
***** Definitions[edit] *****
Formally, a function     f   {\displaystyle f}  [f] is real analytic on an open
set     D   {\displaystyle D}  [D] in the real_line if for any      x  0
&#x2208; D   {\displaystyle x_{0}\in D}  [x_0\in D] one can write
         f ( x ) =  &#x2211;  n = 0   &#x221E;    a  n     (  x &#x2212;  x  0
      )   n   =  a  0   +  a  1   ( x &#x2212;  x  0   ) +  a  2   ( x &#x2212;
      x  0    )  2   +  a  3   ( x &#x2212;  x  0    )  3   + &#x22EF;
      {\displaystyle f(x)=\sum _{n=0}^{\infty }a_{n}\left(x-x_{0}\right)^{n}=a_
      {0}+a_{1}(x-x_{0})+a_{2}(x-x_{0})^{2}+a_{3}(x-x_{0})^{3}+\cdots }  [f
      (x)=\sum _{n=0}^{\infty }a_{n}\left(x-x_{0}\right)^{n}=a_{0}+a_{1}(x-x_
      {0})+a_{2}(x-x_{0})^{2}+a_{3}(x-x_{0})^{3}+\cdots ]
in which the coefficients      a  0   ,  a  1   , &#x2026;   {\displaystyle a_
{0},a_{1},\dots }  [{\displaystyle a_{0},a_{1},\dots }] are real numbers and
the series is convergent to     f ( x )   {\displaystyle f(x)}  [f(x)] for
x   {\displaystyle x}  [x] in a neighborhood of      x  0     {\displaystyle x_
{0}}  [x_{0}].
Alternatively, an analytic function is an infinitely_differentiable_function
such that the Taylor_series at any point      x  0     {\displaystyle x_{0}}
[x_{0}] in its domain
         T ( x ) =  &#x2211;  n = 0   &#x221E;       f  ( n )   (  x  0   )   n
      !    ( x &#x2212;  x  0    )  n     {\displaystyle T(x)=\sum _{n=0}^
      {\infty }{\frac {f^{(n)}(x_{0})}{n!}}(x-x_{0})^{n}}  [T(x)=\sum _{n=0}^
      {\infty }{\frac {f^{(n)}(x_{0})}{n!}}(x-x_{0})^{n}]
converges to     f ( x )   {\displaystyle f(x)}  [f(x)] for     x
{\displaystyle x}  [x] in a neighborhood of      x  0     {\displaystyle x_{0}}
[x_{0}] pointwise.[a] The set of all real analytic functions on a given set
D   {\displaystyle D}  [D] is often denoted by      C   &#x03C9;   ( D )
{\displaystyle C^{\,\omega }(D)}  [{\displaystyle C^{\,\omega }(D)}].
A function     f   {\displaystyle f}  [f] defined on some subset of the real
line is said to be real analytic at a point     x   {\displaystyle x}  [x] if
there is a neighborhood     D   {\displaystyle D}  [D] of     x
{\displaystyle x}  [x] on which     f   {\displaystyle f}  [f] is real
analytic.
The definition of a complex analytic function is obtained by replacing, in the
definitions above, "real" with "complex" and "real line" with "complex plane".
A function is complex analytic if and only if it is holomorphic i.e. it is
complex differentiable. For this reason the terms "holomorphic" and "analytic"
are often used interchangeably for such functions.[1]
***** Examples[edit] *****
Typical examples of analytic functions are:
    * All elementary_functions:
          o All polynomials: if a polynomial has degree n, any terms of degree
            larger than n in its Taylor series expansion must immediately
            vanish to 0, and so this series will be trivially convergent.
            Furthermore, every polynomial is its own Maclaurin_series.
          o The exponential_function is analytic. Any Taylor series for this
            function converges not only for x close enough to x0 (as in the
            definition) but for all values of x (real or complex).
          o The trigonometric_functions, logarithm, and the power_functions are
            analytic on any open set of their domain.
    * Most special_functions (at least in some range of the complex plane):
          o hypergeometric_functions
                # Bessel_functions
          o gamma_function
Typical examples of functions that are not analytic are:
    * The absolute_value function when defined on the set of real numbers or
      complex numbers is not everywhere analytic because it is not
      differentiable at 0. Piecewise_defined functions (functions given by
      different formulae in different regions) are typically not analytic where
      the pieces meet.
    * The complex_conjugate function z → z* is not complex analytic, although
      its restriction to the real line is the identity function and therefore
      real analytic, and it is real analytic as a function from       R   2
      {\displaystyle \mathbb {R} ^{2}}  [{\mathbb  {R}}^{{2}}] to       R   2
      {\displaystyle \mathbb {R} ^{2}}  [{\mathbb  {R}}^{{2}}].
    * Other non-analytic_smooth_functions.
***** Alternative characterizations[edit] *****
The following conditions are equivalent:
1.     f   {\displaystyle f}  [f] is real analytic on an open set     D
{\displaystyle D}  [D].
2. There is a complex analytic extension of     f   {\displaystyle f}  [f] to
an open set     G &#x2282;  C    {\displaystyle G\subset \mathbb {C} }  [
{\displaystyle G\subset \mathbb {C} }] which contains     D   {\displaystyle D}
[D].
3.     f   {\displaystyle f}  [f] is real smooth and for every compact_set
K &#x2282; D   {\displaystyle K\subset D}  [{\displaystyle K\subset D}] there
exists a constant     C   {\displaystyle C}  [C] such that for every     x
&#x2208; K   {\displaystyle x\in K}  [x\in K] and every non-negative integer
k   {\displaystyle k}  [k] the following bound holds[2]
                |      d  k   f   d  x  k      ( x )  |  &#x2264;  C  k + 1   k
            !   {\displaystyle \left|{\frac {d^{k}f}{dx^{k}}}(x)\right|\leq C^
            {k+1}k!}  [\left|{\frac {d^{k}f}{dx^{k}}}(x)\right|\leq C^{k+1}k!]
Complex analytic functions are exactly equivalent to holomorphic_functions, and
are thus much more easily characterized.
For the case of an analytic function with several variables (see below), the
real analyticity can be characterized using the FourierâBrosâIagolnitzer
transform. The third characterization has also a direct generalization for the
multivariate case.[3]
***** Properties of analytic functions[edit] *****
    * The sums, products, and compositions of analytic functions are analytic.
    * The reciprocal of an analytic function that is nowhere zero is analytic,
      as is the inverse of an invertible analytic function whose derivative is
      nowhere zero. (See also the Lagrange_inversion_theorem.)
    * Any analytic function is smooth, that is, infinitely differentiable. The
      converse is not true for real functions; in fact, in a certain sense, the
      real analytic functions are sparse compared to all real infinitely
      differentiable functions. For the complex numbers, the converse does
      hold, and in fact any function differentiable once on an open set is
      analytic on that set (see "analyticity and differentiability" below).
    * For any open_set Î© â C, the set A(Î©) of all analytic functions u :
       Î© â C is a FrÃ©chet_space with respect to the uniform convergence on
      compact sets. The fact that uniform limits on compact sets of analytic
      functions are analytic is an easy consequence of Morera's_theorem. The
      set       A  &#x221E;   ( &#x03A9; )    {\displaystyle \scriptstyle A_
      {\infty }(\Omega )}  [\scriptstyle A_{\infty }(\Omega )] of all bounded
      analytic functions with the supremum_norm is a Banach_space.
A polynomial cannot be zero at too many points unless it is the zero polynomial
(more precisely, the number of zeros is at most the degree of the polynomial).
A similar but weaker statement holds for analytic functions. If the set of
zeros of an analytic function Æ has an accumulation_point inside its domain,
then Æ is zero everywhere on the connected_component containing the
accumulation point. In other words, if (rn) is a sequence of distinct numbers
such that Æ(rn) = 0 for all n and this sequence converges to a point r in the
domain of D, then Æ is identically zero on the connected component of D
containing r. This is known as the Principle_of_Permanence.
Also, if all the derivatives of an analytic function at a point are zero, the
function is constant on the corresponding connected component.
These statements imply that while analytic functions do have more degrees_of
freedom than polynomials, they are still quite rigid.
***** Analyticity and differentiability[edit] *****
As noted above, any analytic function (real or complex) is infinitely
differentiable (also known as smooth, or Câ). (Note that this
differentiability is in the sense of real variables; compare complex
derivatives below.) There exist smooth real functions that are not analytic:
see non-analytic_smooth_function. In fact there are many such functions.
The situation is quite different when one considers complex analytic functions
and complex derivatives. It can be proved that any_complex_function
differentiable_(in_the_complex_sense)_in_an_open_set_is_analytic. Consequently,
in complex_analysis, the term analytic function is synonymous with holomorphic
function.
***** Real versus complex analytic functions[edit] *****
Real and complex analytic functions have important differences (one could
notice that even from their different relationship with differentiability).
Analyticity of complex functions is a more restrictive property, as it has more
restrictive necessary conditions and complex analytic functions have more
structure than their real-line counterparts.[4]
According to Liouville's_theorem, any bounded complex analytic function defined
on the whole complex plane is constant. The corresponding statement for real
analytic functions, with the complex plane replaced by the real line, is
clearly false; this is illustrated by
         f ( x ) =   1   x  2   + 1    .   {\displaystyle f(x)={\frac {1}{x^
      {2}+1}}.}  [f(x)={\frac {1}{x^{2}+1}}.]
Also, if a complex analytic function is defined in an open ball around a point
x0, its power series expansion at x0 is convergent in the whole open ball
(holomorphic_functions_are_analytic). This statement for real analytic
functions (with open ball meaning an open interval of the real line rather than
an open disk of the complex plane) is not true in general; the function of the
example above gives an example for x0 = 0 and a ball of radius exceeding 1,
since the power series 1 â x2 + x4 â x6... diverges for |x| > 1.
Any real analytic function on some open_set on the real line can be extended to
a complex analytic function on some open set of the complex plane. However, not
every real analytic function defined on the whole real line can be extended to
a complex function defined on the whole complex plane. The function Æ(x)
defined in the paragraph above is a counterexample, as it is not defined for
x = Â±i. This explains why the Taylor series of Æ(x) diverges for |x| > 1,
i.e., the radius_of_convergence is 1 because the complexified function has a
pole at distance 1 from the evaluation point 0 and no further poles within the
open disc of radius 1 around the evaluation point.
***** Analytic functions of several variables[edit] *****
One can define analytic functions in several variables by means of power series
in those variables (see power_series). Analytic functions of several variables
have some of the same properties as analytic functions of one variable.
However, especially for complex analytic functions, new and interesting
phenomena show up when working in 2 or more dimensions:
    * Zero sets of complex analytic functions in more than one variable are
      never discrete due to Hartogs's_extension_theorem.
    * Domains_of_holomorphy for single valued functions consist of arbitrary
      open sets. However, in several complex variables the characterization of
      domains of holomorphy leads to the notion of pseudoconvexity.
***** See also[edit] *****
    * CauchyâRiemann_equations
    * Holomorphic_function
    * PaleyâWiener_theorem
    * Quasi-analytic_function
    * Infinite_compositions_of_analytic_functions
***** Notes[edit] *****
   1. ^ This implies uniform_convergence as well in a (possibly smaller)
      neighborhood of      x  0     {\displaystyle x_{0}}  [x_{0}].
   1. ^Churchill; Brown; Verhey (1948). Complex Variables and Applications.
      McGraw-Hill. p. 46. ISBN 0-07-010855-2. A function f of the complex
      variable z is analytic at point z0 if its derivative exists not only at z
      but at each point z in some neighborhood of z0. It is analytic in a
      region R if it is analytic at every point in R. The term holomorphic is
      also used in the literature do denote analyticity
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
   3. ^ Krantz_&_Parks_2002, p. 15.
   4. ^Komatsu, Hikosaburo (1960). "A_characterization_of_real_analytic
      functions". Proceedings of the Japan Academy. 36 (3): 90â93. doi:
      10.3792/pja/1195524081. ISSN 0021-4280.
   5. ^ Krantz_&_Parks_2002.
***** References[edit] *****
    * Conway,_John_B. (1978). Functions of One Complex Variable I. Graduate
      Texts_in_Mathematics 11 (2nd ed.). Springer-Verlag. ISBN 978-0-387-90328-
      6.
Krantz,_Steven; Parks,_Harold_R. (2002). A Primer of Real Analytic Functions
(2nd ed.). BirkhÃ¤user. ISBN 0-8176-4264-1.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Analytic_function", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Weisstein,_Eric_W. "Analytic_Function". MathWorld.
Solver_for_all_zeros_of_a_complex_analytic_function_that_lie_within_a
rectangular_region_by_Ivan_B._Ivanov
Authority_control [Edit_this_at_Wikidata]     * NDL: 00564621

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Analytic_function&oldid=909784891"
Categories:
    * Analytic_functions
Hidden categories:
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
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
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * LietuviÅ³
    * Magyar
    * à´®à´²à´¯à´¾à´³à´
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 16:03 (UTC).
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
