The following text has been accessed from https://en.wikipedia.org/wiki/Complex_analysis at Fri Aug 9 03:39:59 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Complex analysis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Branch of mathematics studying functions of a complex variable
"Complex analytic" redirects here. For the class of functions often called
"complex analytic", see Holomorphic_function.
Not to be confused with Complexity_theory.
Color_wheel_graph of the function f(z) = (z2 â 1)(z + 2 â i)2 / (z2 + 2 -
2i).
Hue represents the argument, brightness the magnitude.
Mathematical_analysis â Complex analysis
Complex analysis
[Gamma_abs_3D.png]
Complex_numbers
    * Real_number
    * Imaginary_number
    * Complex_plane
    * Complex_conjugate
    * Unit_complex_number
Complex_functions
    * Complex-valued_function
    * Analytic_function
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
Complex analysis, traditionally known as the theory of functions of a complex
variable, is the branch of mathematical_analysis that investigates functions of
complex_numbers. It is useful in many branches of mathematics, including
algebraic_geometry, number_theory, analytic_combinatorics, applied_mathematics;
as well as in physics, including the branches of hydrodynamics, thermodynamics,
and particularly quantum_mechanics. By extension, use of complex analysis also
has applications in engineering fields such as nuclear, aerospace, mechanical
and electrical_engineering.[citation_needed]
As a differentiable_function of a complex variable is equal to the sum of its
Taylor_series (that is, it is analytic), complex analysis is particularly
concerned with analytic functions of a complex variable (that is, holomorphic
functions).
⁰
***** Contents *****
    * 1_History
    * 2_Complex_functions
    * 3_Holomorphic_functions
    * 4_Major_results
    * 5_See_also
    * 6_References
    * 7_External_links
***** History[edit] *****
The Mandelbrot_set, a fractal
Complex analysis is one of the classical branches in mathematics, with roots in
the 18th century and just prior. Important mathematicians associated with
complex numbers include Euler, Gauss, Riemann, Cauchy, Weierstrass, and many
more in the 20th century. Complex analysis, in particular the theory of
conformal_mappings, has many physical applications and is also used throughout
analytic_number_theory. In modern times, it has become very popular through a
new boost from complex_dynamics and the pictures of fractals produced by
iterating holomorphic_functions. Another important application of complex
analysis is in string_theory which studies conformal invariants in quantum
field_theory.
***** Complex functions[edit] *****
An exponential function An of a discrete (integer) variable n, similar to
geometric_progression
A complex function is a function from complex_numbers to complex numbers. In
other words, it is a function that has a subset of the complex numbers as a
domain and the complex numbers as a codomain. Complex functions are generally
supposed to have a domain that contains a nonempty open_subset of the complex
plane.
For any complex function, the values     z   {\displaystyle z}  [z] from the
domain and their images     f ( z )   {\displaystyle f(z)}  [f(z)] in the range
may be separated into real and imaginary parts:
         z = x + i y   &#xA0;and&#xA0;   f ( z ) = f ( x + i y ) = u ( x , y )
      + i v ( x , y ) ,   {\displaystyle z=x+iy\quad {\text{ and }}\quad f(z)=f
      (x+iy)=u(x,y)+iv(x,y),}  [{\displaystyle z=x+iy\quad {\text{ and }}\quad
      f(z)=f(x+iy)=u(x,y)+iv(x,y),}]
where     x , y , u ( x , y ) , v ( x , y )   {\displaystyle x,y,u(x,y),v(x,y)}
[{\displaystyle x,y,u(x,y),v(x,y)}] are all real-valued.
In other words, a complex function     f :  C  &#x2192;  C    {\displaystyle f:
\mathbb {C} \to \mathbb {C} }  [{\displaystyle f:\mathbb {C} \to \mathbb {C} }]
may be decomposed into
         u :   R   2   &#x2192;  R     {\displaystyle u:\mathbb {R} ^{2}\to
      \mathbb {R} \quad }  [{\displaystyle u:\mathbb {R} ^{2}\to \mathbb {R}
      \quad }] and      v :   R   2   &#x2192;  R  ,   {\displaystyle \quad v:
      \mathbb {R} ^{2}\to \mathbb {R} ,}  [{\displaystyle \quad v:\mathbb {R} ^
      {2}\to \mathbb {R} ,}]
i.e., into two real-valued functions (    u   {\displaystyle u}  [u],     v
{\displaystyle v}  [v]) of two real variables (    x   {\displaystyle x}  [x],
y   {\displaystyle y}  [y]).
Similarly, any complex-valued function f on an arbitrary set X can be
considered as an ordered_pair of two real-valued_functions: (Re f, Im f) or,
alternatively, as a vector-valued_function from X into       R   2   .
{\displaystyle \mathbb {R} ^{2}.}  [{\displaystyle \mathbb {R} ^{2}.}]
Some properties of complex-valued functions (such as continuity) are nothing
more than the corresponding properties of vector valued functions of two real
variables. Other concepts of complex analysis, such as differentiability are
direct generalizations of the similar concepts for real functions, but may have
very different properties. In particular, every differentiable_complex_function
is analytic (see next section), and two differentiable functions that are equal
in a neighborhood of a point are equal on the intersection of their domain (if
the domains are connected). The latter property is the basis of the principle
of analytic_continuation which allows extending every real analytic_function in
a unique way for getting a complex analytic function whose domain is the whole
complex plane with a finite number of curve_arcs removed. Many basic and
special complex functions are defined in this way, including exponential
functions, logarithmic_functions, and trigonometric_functions.
***** Holomorphic functions[edit] *****
Main article: Holomorphic_function
Complex functions that are differentiable at every point of an open_subset
&#x03A9;   {\displaystyle \Omega }  [\Omega ] of the complex plane are said to
be holomorphic on     &#x03A9;   {\displaystyle \Omega }  [\Omega ]. In the
context of complex analysis, the derivative of     f   {\displaystyle f}  [f]
at      z  0     {\displaystyle z_{0}}  [z_{0}] is defined to be
          f &#x2032;  (  z  0   ) =  lim  z &#x2192;  z  0        f ( z )
      &#x2212; f (  z  0   )   z &#x2212;  z  0      ,  z &#x2208;  C  .
      {\displaystyle f'(z_{0})=\lim _{z\to z_{0}}{\frac {f(z)-f(z_{0})}{z-z_
      {0}}},\quad z\in \mathbb {C} .}  [{\displaystyle f'(z_{0})=\lim _{z\to z_
      {0}}{\frac {f(z)-f(z_{0})}{z-z_{0}}},\quad z\in \mathbb {C} .}]
Superficially, this definition is formally analogous to that of the derivative
of a real function. However, complex derivatives and differentiable functions
behave in significantly different ways compared to their real counterparts. In
particular, for this limit to exist, the value of the difference quotient must
approach the same complex number, regardless of the manner in which we approach
z  0     {\displaystyle z_{0}}  [z_{0}] in the complex plane. Consequently,
complex differentiability has much stronger implications than real
differentiability. For instance, holomorphic functions are infinitely
differentiable, whereas the existence of the nth derivative need not imply the
existence of the (n + 1)th derivative for real functions. Furthermore, all
holomorphic functions satisfy the stronger condition of analyticity, meaning
that the function is, at every point in its domain, locally given by a
convergent power series. In essence, this means that functions holomorphic on
&#x03A9;   {\displaystyle \Omega }  [\Omega ] can be approximated arbitrarily
well by polynomials in some neighborhood of every point in     &#x03A9;
{\displaystyle \Omega }  [\Omega ]. This stands in sharp contrast to
differentiable real functions; even infinitely_differentiable_real_functions
can_be_nowhere_analytic.
Most elementary functions, including the exponential_function, the
trigonometric_functions, and all polynomial_functions, extended appropriately
to complex arguments as functions      C  &#x2192;  C    {\displaystyle \mathbb
{C} \to \mathbb {C} }  [{\displaystyle \mathbb {C} \to \mathbb {C} }], are
holomorphic over the entire complex plane, making them entire functions, while
rational functions     p  /  q   {\displaystyle p/q}  [p/q], where p and q are
polynomials, are holomorphic on domains that exclude points where q is zero.
Such functions that are holomorphic everywhere except a set of isolated points
are known as meromorphic functions. On the other hand, the functions     z
&#x21A6; &#x211C; ( z )   {\displaystyle z\mapsto \Re (z)}  [{\displaystyle
z\mapsto \Re (z)}],     z &#x21A6;  |  z  |    {\displaystyle z\mapsto |z|}  [
{\displaystyle z\mapsto |z|}], and     z &#x21A6;    z &#x00AF;
{\displaystyle z\mapsto {\bar {z}}}  [{\displaystyle z\mapsto {\bar {z}}}] are
not holomorphic anywhere on the complex plane, as can be shown by their failure
to satisfy the CauchyâRiemann conditions (see below).
An important property of holomorphic functions is the relationship between the
partial derivatives of their real and imaginary components, known as the
CauchyâRiemann_conditions. If     f :  C  &#x2192;  C    {\displaystyle f:
\mathbb {C} \to \mathbb {C} }  [{\displaystyle f:\mathbb {C} \to \mathbb {C}
}], defined by     f ( z ) = f ( x + i y ) = u ( x , y ) + i v ( x , y )
{\displaystyle f(z)=f(x+iy)=u(x,y)+iv(x,y)}  [{\displaystyle f(z)=f(x+iy)=u
(x,y)+iv(x,y)}], where     x , y , u ( x , y ) , v ( x , y ) &#x2208;  R
{\displaystyle x,y,u(x,y),v(x,y)\in \mathbb {R} }  [{\displaystyle x,y,u(x,y),v
(x,y)\in \mathbb {R} }], is holomorphic on a region     &#x03A9;
{\displaystyle \Omega }  [\Omega ], then    ( &#x2202; f  /  &#x2202;    z
&#x00AF;    ) (  z  0   ) = 0   {\displaystyle (\partial f/\partial {\bar {z}})
(z_{0})=0}  [{\displaystyle (\partial f/\partial {\bar {z}})(z_{0})=0}] must
hold for all      z  0   &#x2208; &#x03A9;   {\displaystyle z_{0}\in \Omega }
[{\displaystyle z_{0}\in \Omega }]. Here, the differential operator
&#x2202;  /  &#x2202;    z &#x00AF;      {\displaystyle \partial /\partial
{\bar {z}}}  [{\displaystyle \partial /\partial {\bar {z}}}] is defined as
( 1  /  2 ) ( &#x2202;  /  &#x2202; x + i &#x2202;  /  &#x2202; y )
{\displaystyle (1/2)(\partial /\partial x+i\partial /\partial y)}  [
{\displaystyle (1/2)(\partial /\partial x+i\partial /\partial y)}]. In terms of
the real and imaginary parts of the function, u and v, this is equivalent to
the pair of equations      u  x   =  v  y     {\displaystyle u_{x}=v_{y}}  [
{\displaystyle u_{x}=v_{y}}] and      u  y   = &#x2212;  v  x
{\displaystyle u_{y}=-v_{x}}  [{\displaystyle u_{y}=-v_{x}}], where the
subscripts indicate partial differentiation. However, the CauchyâRiemann
conditions do not characterize holomorphic functions, without additional
continuity conditions (see LoomanâMenchoff_theorem).
Holomorphic functions exhibit some remarkable features. For instance, Picard's
theorem asserts that the range of an entire function can only take three
possible forms:      C    {\displaystyle \mathbb {C} }  [\mathbb {C} ],      C
&#x2216; {  z  0   }   {\displaystyle \mathbb {C} \smallsetminus \{z_{0}\}}  [
{\displaystyle \mathbb {C} \smallsetminus \{z_{0}\}}], or     {  z  0   }
{\displaystyle \{z_{0}\}}  [{\displaystyle \{z_{0}\}}] for some      z  0
&#x2208;  C    {\displaystyle z_{0}\in \mathbb {C} }  [z_{0}\in {\mathbb
{C}}]. In other words, if two distinct complex numbers     z   {\displaystyle
z}  [z] and     w   {\displaystyle w}  [w] are not in the range of entire
function     f   {\displaystyle f}  [f], then     f   {\displaystyle f}  [f] is
a constant function. Moreover, given a holomorphic function     f
{\displaystyle f}  [f] defined on an open set     U   {\displaystyle U}  [U],
the analytic_continuation of     f   {\displaystyle f}  [f] to a larger open
set     V &#x2283; U   {\displaystyle V\supset U}  [{\displaystyle V\supset U}]
is unique. As a result, the value of a holomorphic function over an arbitrarily
small region in fact determines the value of the function everywhere to which
it can be extended as a holomorphic function.
See also: analytic_function, coherent_sheaf and vector_bundles.
***** Major results[edit] *****
One of the central tools in complex analysis is the line_integral. The line
integral around a closed path of a function that is holomorphic everywhere
inside the area bounded by the closed path is always zero, as is stated by the
Cauchy_integral_theorem. The values of such a holomorphic function inside a
disk can be computed by a path integral on the disk's boundary (as shown in
Cauchy's_integral_formula). Path integrals in the complex plane are often used
to determine complicated real integrals, and here the theory of residues among
others is applicable (see methods_of_contour_integration). A "pole" (or
isolated_singularity) of a function is a point where the function's value
becomes unbounded, or "blows up". If a function has such a pole, then one can
compute the function's residue there, which can be used to compute path
integrals involving the function; this is the content of the powerful residue
theorem. The remarkable behavior of holomorphic functions near essential
singularities is described by Picard's_Theorem. Functions that have only poles
but no essential_singularities are called meromorphic. Laurent_series are the
complex-valued equivalent to Taylor_series, but can be used to study the
behavior of functions near singularities through infinite sums of more well
understood functions, such as polynomials.
A bounded_function that is holomorphic in the entire complex plane must be
constant; this is Liouville's_theorem. It can be used to provide a natural and
short proof for the fundamental_theorem_of_algebra which states that the field
of complex numbers is algebraically_closed.
If a function is holomorphic throughout a connected domain then its values are
fully determined by its values on any smaller subdomain. The function on the
larger domain is said to be analytically_continued from its values on the
smaller domain. This allows the extension of the definition of functions, such
as the Riemann_zeta_function, which are initially defined in terms of infinite
sums that converge only on limited domains to almost the entire complex plane.
Sometimes, as in the case of the natural_logarithm, it is impossible to
analytically continue a holomorphic function to a non-simply connected domain
in the complex plane but it is possible to extend it to a holomorphic function
on a closely related surface known as a Riemann_surface.
All this refers to complex analysis in one variable. There is also a very rich
theory of complex_analysis_in_more_than_one_complex_dimension in which the
analytic properties such as power_series expansion carry over whereas most of
the geometric properties of holomorphic functions in one complex dimension
(such as conformality) do not carry over. The Riemann_mapping_theorem about the
conformal relationship of certain domains in the complex plane, which may be
the most important result in the one-dimensional theory, fails dramatically in
higher dimensions.
A major use of certain complex spaces is in quantum_mechanics as wave
functions.
***** See also[edit] *****
    * Analytic_continuation
    * Complex_dynamics
    * List_of_complex_analysis_topics
    * Monodromy_theorem
    * Real_analysis
    * Runge's_theorem
    * Several_complex_variables
***** References[edit] *****
    * Ahlfors,_L., Complex Analysis, 3 ed. (McGraw-Hill, 1979).
    * Stephen_D._Fisher, Complex Variables, 2 ed. (Dover, 1999).
    * CarathÃ©odory,_C., Theory of Functions of a Complex Variable (Chelsea,
      New York). [2 volumes.]
    * Henrici,_P., Applied and Computational Complex Analysis (Wiley). [Three
      volumes: 1974, 1977, 1986.]
    * Kreyszig,_E., Advanced Engineering Mathematics, 10 ed., Ch. 13â18
      (Wiley, 2011).
    * Markushevich, A.I.,Theory of Functions of a Complex Variable (Prentice-
      Hall, 1965). [Three volumes.]
    * Marsden & Hoffman, Basic Complex Analysis. 3 ed. (Freeman, 1999).
    * Needham,_T., Visual Complex Analysis (Oxford, 1997).
    * Rudin,_W., Real and Complex Analysis, 3 ed. (McGraw-Hill, 1986).
    * Scheidemann, V., Introduction to complex analysis in several variables
      (Birkhauser, 2005)
    * Shaw, W.T., Complex Analysis with Mathematica (Cambridge, 2006).
    * Spiegel,_Murray_R. Theory and Problems of Complex Variables â with an
      introduction to Conformal Mapping and its applications (McGraw-Hill,
      1964).
    * Stein & Shakarchi, Complex Analysis (Princeton, 2003).
    * Ablowitz & Fokas, Complex Variables: Introduction and Applications
      (Cambridge, 2003).
***** External links[edit] *****
Complex analysisat Wikipedia's sister_projects
    * Definitions from Wiktionary
    * Media from Wikimedia Commons
    * Quotations from Wikiquote
    * Wolfram_Research's_MathWorld_Complex_Analysis_Page

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Complex_analysis&oldid=895768887"
Categories:
    * Complex_analysis
Hidden categories:
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_June_2018
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
    * Wikibooks
    * Wikiquote
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * ÐÐ°ÑÒ¡Ð¾ÑÑÑÐ°
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * ÐÑÐ¾Ð½
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * Lumbaart
    * Magyar
    * Malti
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * à·à·à¶à·à¶½
    * Simple_English
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
    * This page was last edited on 6 May 2019, at 11:47 (UTC).
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
