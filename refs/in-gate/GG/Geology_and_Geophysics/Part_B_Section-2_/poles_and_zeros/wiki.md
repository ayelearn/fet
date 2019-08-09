The following text has been accessed from https://en.wikipedia.org/wiki/Zeros_and_poles at Thu Aug 8 23:27:03 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Zeros and poles ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
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
    * Analytic_function
    * Holomorphic_function
    * CauchyâRiemann_equations
    * Formal_power_series
Basic_Theory
    * Zeros and poles
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
In complex_analysis (a branch of mathematics), zeros of holomorphic
functionsâwhich are points z where f(z) = 0âplay an important role.
For meromorphic_functions, particularly, there is a duality between zeros and
poles. A function f of a complex_variable z is meromorphic in the neighbourhood
of a point z0 if either f or its reciprocal function 1/f is holomorphic in some
neighbourhood of z0 (that is, if f or 1/f  is differentiable in a neighbourhood
of z0). If z0 is a zero of 1/f , then it is a pole of f.
Thus a pole is a certain type of singularity of a function, nearby which the
function behaves relatively regularly, in contrast to essential_singularities,
such as 0 for the logarithm_function, and branch_points, such as 0 for the
complex square_root_function.
⁰
***** Contents *****
    * 1_Definitions
    * 2_At_infinity
    * 3_Examples
    * 4_Function_on_a_curve
    * 5_See_also
    * 6_References
    * 7_External_links
***** Definitions[edit] *****
A function_of_a_complex_variable z is holomorphic in an open_domain U if it is
differentiable with respect to z at every point of U. Equivalently, it is
holomorphic if it is analytic, that is, if its Taylor_series exists at every
point of U, and converges to the function in some neighbourhood of the point. A
function is meromorphic in U if every point of U has a neighbourhood such that
either f or 1/f is holomorphic in it.
A zero of a meromorphic function f is a complex number z such that f(z) = 0. A
pole of f is a zero of 1/f.
If f is a function that is meromorphic in a neighbourhood of a point      z  0
{\displaystyle z_{0}}  [z_{0}] of the complex_plane, then there exists an
integer n such that
         ( z &#x2212;  z  0    )  n   f ( z )   {\displaystyle (z-z_{0})^{n}f
      (z)}  [{\displaystyle (z-z_{0})^{n}f(z)}]
is holomorphic and nonzero in a neighbourhood of      z  0     {\displaystyle
z_{0}}  [z_{0}] (this is a consequence of the analytic property). If n > 0,
then      z  0     {\displaystyle z_{0}}  [z_{0}] is a pole of order (or
multiplicity) n of f. If n < 0, then      z  0     {\displaystyle z_{0}}  [z_
{0}] is a zero of order      |  n  |    {\displaystyle |n|}  [{\displaystyle
|n|}] of f. Simple zero and simple pole are terms used for zeroes and poles of
order      |  n  |  = 1.   {\displaystyle |n|=1.}  [{\displaystyle |n|=1.}]
Degree is sometimes used synonymously to order.
This characterization of zeros and poles implies that zeros and poles are
isolated, that is, every zero or pole has a neighbourhood that does not contain
any other zero and pole.
Because of the order of zeros and poles being defined as a non-negative number
n and the symmetry between them, it is often useful to consider a pole of order
n as a zero of order ân and a zero of order n as a pole of order ân. In
this case a point that is neither a pole nor a zero is viewed as a pole (or
zero) of order 0.
A meromorphic function may have infinitely many zeros and poles. This is the
case for the gamma_function (see the image in the infobox), which is
meromorphic in the whole complex plane, and has a simple pole at every non-
positive integer. The Riemann_zeta_function is also meromorphic in the whole
complex plane, with a single pole of order 1 at z = 1. Its zeros in the left
halfplane are all the negative even integers, and the Riemann_hypothesis is the
conjecture that all other zeros are along Re(z) = 1/2.
In a neighbourhood of a point      z  0   ,   {\displaystyle z_{0},}  [
{\displaystyle z_{0},}] a nonzero meromorphic function f is the sum of a
Laurent_series with at most finite principal part (the terms with negative
index values):
         f ( z ) =  &#x2211;  k &#x2265; &#x2212; n    a  k   ( z &#x2212;  z
      0    )  k   ,   {\displaystyle f(z)=\sum _{k\geq -n}a_{k}(z-z_{0})^{k},}
      [{\displaystyle f(z)=\sum _{k\geq -n}a_{k}(z-z_{0})^{k},}]
where n is an integer, and      a  &#x2212; n   &#x2260; 0.   {\displaystyle a_
{-n}\neq 0.}  [{\displaystyle a_{-n}\neq 0.}] Again, if n > 0 (the sum starts
with      a  &#x2212;  |  n  |    ( z &#x2212;  z  0    )  &#x2212;  |  n  |
{\displaystyle a_{-|n|}(z-z_{0})^{-|n|}}  [{\displaystyle a_{-|n|}(z-z_{0})^{-
|n|}}], the principal part has n terms), one has a pole of order n, and if n
â¤ 0 (the sum starts with      a   |  n  |    ( z &#x2212;  z  0    )   |  n
|      {\displaystyle a_{|n|}(z-z_{0})^{|n|}}  [{\displaystyle a_{|n|}(z-z_
{0})^{|n|}}], there is no principal part), one has a zero of order      |  n  |
{\displaystyle |n|}  [{\displaystyle |n|}].
***** At infinity[edit] *****
A function     z &#x21A6; f ( z )   {\displaystyle z\mapsto f(z)}  [
{\displaystyle z\mapsto f(z)}] is meromorphic at infinity if it is meromorphic
in some neighbourhood of infinity (that is outside some disk), and there is an
integer n such that
          lim  z &#x2192; &#x221E;      f ( z )   z  n       {\displaystyle
      \lim _{z\to \infty }{\frac {f(z)}{z^{n}}}}  [{\displaystyle \lim _{z\to
      \infty }{\frac {f(z)}{z^{n}}}}]
exists and is a nonzero complex number.
In this case, the point_at_infinity is a pole of order n if n > 0, and a zero
of order n if n < 0.
For example, a polynomial of degree n has a pole of degree n at infinity.
The complex_plane extended by a point at infinity is called the Riemann_sphere.
If f is a function that is meromorphic on the whole Riemann sphere, then it has
a finite number of zeros and poles, and the sum of the orders of its poles
equals the sum of the orders of its zeros.
Every rational_function is meromorphic on the whole Riemann sphere, and, in
this case, the sum of orders of the zeros or of the poles is the maximum of the
degrees of the numerator and the denominator.
***** Examples[edit] *****
A pole of order 9, at infinity, for a polynomial_complex_function of degree 9,
such as     f ( z ) =  z  9     {\displaystyle f(z)=z^{9}}  [{\displaystyle f
(z)=z^{9}}]
    * The function
               f ( z ) =   3 z     {\displaystyle f(z)={\frac {3}{z}}}  [f(z) =
            \frac{3}{z}]
      is meromorphic on the whole Riemann sphere. It has a pole of order 1 or
      simple pole at     z = 0 ,   {\displaystyle z=0,}  [{\displaystyle z=0,}]
      and a simple zero at infinity.
    * The function
               f ( z ) =    z + 2   ( z &#x2212; 5  )  2   ( z + 7  )  3
            {\displaystyle f(z)={\frac {z+2}{(z-5)^{2}(z+7)^{3}}}}  [f(z) =
            \frac{z+2}{(z-5)^2(z+7)^3}]
      is meromorphic on the whole Riemann sphere. It has a pole of order 2 at
      z = 5 ,   {\displaystyle z=5,}  [{\displaystyle z=5,}] and a pole of
      order 3 at     z = &#x2212; 7   {\displaystyle z=-7}  [ z = -7]. It has a
      simple zero at     z = &#x2212; 2 ,   {\displaystyle z=-2,}  [
      {\displaystyle z=-2,}] and a quadruple zero at infinity.
    * The function
               f ( z ) =    z &#x2212; 4    e  z   &#x2212; 1
            {\displaystyle f(z)={\frac {z-4}{e^{z}-1}}}  [f(z) = \frac{z-4}
            {e^z-1}]
      is meromorphic in the whole complex plane, but not at infinity. It has
      poles of order 1 at     z = 2 &#x03C0; n i  &#xA0;for&#xA0;  n &#x2208;
      Z    {\displaystyle z=2\pi ni{\text{ for }}n\in \mathbb {Z} }  [
      {\displaystyle z=2\pi ni{\text{ for }}n\in \mathbb {Z} }]. This can be
      seen by writing the Taylor_series of      e  z     {\displaystyle e^{z}}
      [ e^z] around the origin.
    * The function
               f ( z ) = z   {\displaystyle f(z)=z}  [f(z) = z]
      has a single pole at infinity of order 1, and a single zero at the
      origin.
All above examples except for the third are rational_functions. For a general
discussion of zeros and poles of such functions, see Poleâzero_plot
Â§ Continuous-time_systems.
***** Function on a curve[edit] *****
The concept of zeros and poles extends naturally to functions on a complex
curve, that is complex_analytic_manifold of dimension one (over the complex
numbers). The simplest examples of such curves are the complex_plane and the
Riemann_surface. This extension is done by transferring structures and
properties through charts, which are analytic isomorphisms.
More precisely, let f be a function from a complex curve M to the complex
numbers. This function is holomorphic (resp. meromorphic) in a neighbourhood of
a point z of M if there is a chart     &#x03D5;   {\displaystyle \phi }  [\phi
] such that     f &#x2218;  &#x03D5;  &#x2212; 1     {\displaystyle f\circ \phi
^{-1}}  [{\displaystyle f\circ \phi ^{-1}}] is holomorphic (resp. meromorphic)
in a neighbourhood of     &#x03D5; ( z ) .   {\displaystyle \phi (z).}  [
{\displaystyle \phi (z).}] Then, z is a pole or a zero of order n if the same
is true for     &#x03D5; ( z ) .   {\displaystyle \phi (z).}  [{\displaystyle
\phi (z).}]
If the curve is compact, and the function f is meromorphic on the whole curve,
then the number of zeros and poles is finite, and the sum of the orders of the
poles equals the sum of the orders of the zeros. This is one of the basic facts
that are involved in RiemannâRoch_theorem.
***** See also[edit] *****
    * Control_theory#Stability
    * Filter_design
    * Filter_(signal_processing)
    * GaussâLucas_theorem
    * Hurwitz's_theorem_(complex_analysis)
    * Marden's_theorem
    * Nyquist_stability_criterion
    * Poleâzero_plot
    * Residue_(complex_analysis)
    * RouchÃ©'s_theorem
    * Sendov's_conjecture
***** References[edit] *****
    * Conway,_John_B. (1986). Functions of One Complex Variable I. Springer.
      ISBN 0-387-90328-3.
Conway, John B. (1995). Functions of One Complex Variable II. Springer. ISBN 0-
387-94460-5.
Henrici,_Peter (1974). Applied and Computational Complex Analysis 1. John_Wiley
&_Sons.
***** External links[edit] *****
    * Weisstein,_Eric_W. "Pole". MathWorld.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Zeros_and_poles&oldid=901661946"
Categories:
    * Complex_analysis
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
    * CatalÃ 
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * LietuviÅ³
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 13 June 2019, at 12:31 (UTC).
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
