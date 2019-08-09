The following text has been accessed from https://en.wikipedia.org/wiki/Schwarz_lemma at Fri Aug 9 02:37:52 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Schwarz lemma ******
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
    * Zeros_and_poles
    * Cauchy's_integral_theorem
    * Local_primitive
    * Cauchy's_integral_formula
    * Winding_number
    * Laurent_series
    * Isolated_singularity
    * Residue_theorem
    * Conformal_map
    * Schwarz lemma
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
In mathematics, the Schwarz lemma, named after Hermann_Amandus_Schwarz, is a
result in complex_analysis about holomorphic_functions from the open unit_disk
to itself. The lemma is less celebrated than stronger theorems, such as the
Riemann_mapping_theorem, which it helps to prove. It is, however, one of the
simplest results capturing the rigidity of holomorphic functions.
⁰
***** Contents *****
    * 1_Statement
    * 2_Proof
    * 3_Schwarz–Pick_theorem
    * 4_Proof_of_Schwarz–Pick_theorem
    * 5_Further_generalizations_and_related_results
    * 6_References
***** Statement[edit] *****
     Schwarz Lemma. Let      D  = { z :  |  z  |  < 1 }   {\displaystyle
     \mathbf {D} =\{z:|z|<1\}}  [{\displaystyle \mathbf {D} =\{z:|z|<1\}}]
     be the open unit_disk in the complex_plane      C    {\displaystyle
     \mathbb {C} }  [\mathbb {C} ] centered at the origin and let     f :
     D  &#x2192;  C    {\displaystyle f:\mathbf {D} \rightarrow \mathbb
     {C} }  [{\displaystyle f:\mathbf {D} \rightarrow \mathbb {C} }] be a
     holomorphic_map such that     f ( 0 ) = 0   {\displaystyle f(0)=0}
     [f(0)=0] and      |  f ( z )  |  &#x2264; 1   {\displaystyle |f
     (z)|\leq 1}  [{\displaystyle |f(z)|\leq 1}] on      D
     {\displaystyle \mathbf {D} }  [\mathbf{D}].
     Then,      |  f ( z )  |  &#x2264;  |  z  |  &#xA0; &#x2200; z
     &#x2208;  D    {\displaystyle |f(z)|\leq |z|\ \forall z\in \mathbf
     {D} }  [{\displaystyle |f(z)|\leq |z|\ \forall z\in \mathbf {D} }]
     and      |   f &#x2032;  ( 0 )  |  &#x2264; 1   {\displaystyle |f'
     (0)|\leq 1}  [|f'(0)| \leq 1].
     Moreover, if      |  f ( z )  |  =  |  z  |    {\displaystyle |f
     (z)|=|z|}  [|f(z)|=|z|] for some non-zero     z   {\displaystyle z}
     [z] or      |   f &#x2032;  ( 0 )  |  = 1   {\displaystyle |f'(0)|=1}
     [|f'(0)| = 1], then     f ( z ) = a z   {\displaystyle f(z)=az}  [f
     (z)=az] for some     a &#x2208;  C    {\displaystyle a\in \mathbb {C}
     }  [a \in \mathbb{C}] with      |  a  |  = 1   {\displaystyle |a|=1}
     [|a|=1].[1]
***** Proof[edit] *****
The proof is a straightforward application of the maximum_modulus_principle on
the function
         g ( z ) =   {       f ( z )  z        if&#xA0;   z &#x2260; 0      f
      &#x2032;  ( 0 )     if&#xA0;   z = 0 ,         {\displaystyle g(z)=
      {\begin{cases}{\frac {f(z)}{z}}\,&{\mbox{if }}z\neq 0\\f'(0)&{\mbox{if
      }}z=0,\end{cases}}}  [g(z)={\begin{cases}{\frac  {f(z)}{z}}\,&{\mbox{if
      }}z\neq 0\\f'(0)&{\mbox{if }}z=0,\end{cases}}]
which is holomorphic on the whole of D, including at the origin (because f is
differentiable at the origin and fixes zero). Now if Dr = {z : |z| â¤ r}
denotes the closed disk of radius r centered at the origin, then the maximum
modulus principle implies that, for r < 1, given any z in Dr, there exists zr
on the boundary of Dr such that
          |  g ( z )  |  &#x2264;  |  g (  z  r   )  |  =     |  f (  z  r   )
      |     |   z  r    |     &#x2264;   1 r   .   {\displaystyle |g(z)|\leq |g
      (z_{r})|={\frac {|f(z_{r})|}{|z_{r}|}}\leq {\frac {1}{r}}.}  [|g(z)|\leq
      |g(z_{r})|={\frac  {|f(z_{r})|}{|z_{r}|}}\leq {\frac  {1}{r}}.]
As     r &#x2192; 1   {\displaystyle r\rightarrow 1}  [r\rightarrow 1] we get
|  g ( z )  |  &#x2264; 1   {\displaystyle |g(z)|\leq 1}  [|g(z)|\leq 1].
Moreover, suppose that |f(z)| = |z| for some non-zero z in D, or |fâ²(0)| = 1.
Then, |g(z)| = 1 at some point of D. So by the maximum modulus principle, g(z)
is equal to a constant a such that |a| = 1. Therefore, f(z) = az, as desired.
***** Schwarz–Pick theorem[edit] *****
A variant of the Schwarz lemma, known as the Schwarz–Pick theorem (after Georg
Pick), characterizes the analytic automorphisms of the unit disc, i.e.
bijective holomorphic_mappings of the unit disc to itself:
Let f : D â D be holomorphic. Then, for all z1, z2 â D,
          |    f (  z  1   ) &#x2212; f (  z  2   )   1 &#x2212;    f (  z  1
      )  &#x00AF;   f (  z  2   )    |  &#x2264;  |     z  1   &#x2212;  z  2
      1 &#x2212;    z  1   &#x00AF;    z  2      |    {\displaystyle \left|
      {\frac {f(z_{1})-f(z_{2})}{1-{\overline {f(z_{1})}}f(z_{2})}}\right|\leq
      \left|{\frac {z_{1}-z_{2}}{1-{\overline {z_{1}}}z_{2}}}\right|}  [\left|
      {\frac  {f(z_{1})-f(z_{2})}{1-\overline {f(z_{1})}f(z_{2})}}\right|\leq
      \left|{\frac  {z_{1}-z_{2}}{1-\overline {z_{1}}z_{2}}}\right|]
and, for all z â D,
            |   f &#x2032;  ( z )  |   1 &#x2212;   |  f ( z )  |   2
      &#x2264;   1  1 &#x2212;   | z |   2      .   {\displaystyle {\frac
      {\left|f'(z)\right|}{1-\left|f(z)\right|^{2}}}\leq {\frac {1}{1-
      \left|z\right|^{2}}}.}  [{\frac  {\left|f'(z)\right|}{1-\left|f
      (z)\right|^{2}}}\leq {\frac  {1}{1-\left|z\right|^{2}}}.]
The expression
         d (  z  1   ,  z  2   ) =  tanh  &#x2212; 1   &#x2061;  |     z  1
      &#x2212;  z  2     1 &#x2212;    z  1   &#x00AF;    z  2      |
      {\displaystyle d(z_{1},z_{2})=\tanh ^{-1}\left|{\frac {z_{1}-z_{2}}{1-
      {\overline {z_{1}}}z_{2}}}\right|}  [d(z_{1},z_{2})=\tanh ^{{-1}}\left|
      {\frac  {z_{1}-z_{2}}{1-\overline {z_{1}}z_{2}}}\right|]
is the distance of the points z1, z2 in the PoincarÃ©_metric, i.e. the metric
in the PoincarÃ© disc model for hyperbolic_geometry in dimension two. The
Schwarz–Pick theorem then essentially states that a holomorphic map of the unit
disk into itself decreases the distance of points in the PoincarÃ© metric. If
equality holds throughout in one of the two inequalities above (which is
equivalent to saying that the holomorphic map preserves the distance in the
PoincarÃ© metric), then f must be an analytic automorphism of the unit disc,
given by a MÃ¶bius_transformation mapping the unit disc to itself.
An analogous statement on the upper_half-plane H can be made as follows:
     Let f : H â H be holomorphic. Then, for all z1, z2 â H,
               |    f (  z  1   ) &#x2212; f (  z  2   )      f (  z  1
           )  &#x00AF;   &#x2212; f (  z  2   )    |  &#x2264;    |   z  1
           &#x2212;  z  2    |   |     z  1   &#x00AF;   &#x2212;  z  2
           |    .   {\displaystyle \left|{\frac {f(z_{1})-f(z_{2})}{
           {\overline {f(z_{1})}}-f(z_{2})}}\right|\leq {\frac {\left|z_
           {1}-z_{2}\right|}{\left|{\overline {z_{1}}}-z_{2}\right|}}.}
           [\left|{\frac  {f(z_{1})-f(z_{2})}{\overline {f(z_{1})}-f(z_
           {2})}}\right|\leq {\frac  {\left|z_{1}-z_{2}\right|}
           {\left|\overline {z_{1}}-z_{2}\right|}}.]
This is an easy consequence of the Schwarz–Pick theorem mentioned above: One
just needs to remember that the Cayley_transform W(z) = (z â i)/(z + i) maps
the upper half-plane H conformally onto the unit disc D. Then, the map
W o f o Wâ1 is a holomorphic map from D onto D. Using the Schwarz–Pick
theorem on this map, and finally simplifying the results by using the formula
for W, we get the desired result. Also, for all z â H,
            |   f &#x2032;  ( z )  |    Im  ( f ( z ) )    &#x2264;   1   Im
      ( z )    .   {\displaystyle {\frac {\left|f'(z)\right|}{{\text{Im}}(f
      (z))}}\leq {\frac {1}{{\text{Im}}(z)}}.}  [{\frac  {\left|f'(z)\right|}{
      {\text{Im}}(f(z))}}\leq {\frac  {1}{{\text{Im}}(z)}}.]
If equality holds for either the one or the other expressions, then f must be a
MÃ¶bius_transformation with real coefficients. That is, if equality holds, then
         f ( z ) =    a z + b   c z + d      {\displaystyle f(z)={\frac {az+b}
      {cz+d}}}  [f(z)={\frac  {az+b}{cz+d}}]
with a, b, c, d â R, and ad â bc > 0.
***** Proof of Schwarz–Pick theorem[edit] *****
The proof of the Schwarz–Pick theorem follows from Schwarz's lemma and the fact
that a MÃ¶bius_transformation of the form
            z &#x2212;  z  0        z  0   &#x00AF;   z &#x2212; 1    ,   |   z
      0    |  < 1 ,   {\displaystyle {\frac {z-z_{0}}{{\overline {z_{0}}}z-
      1}},\qquad |z_{0}|<1,}  [{\frac  {z-z_{0}}{\overline {z_{0}}z-1}},\qquad
      |z_{0}|<1,]
maps the unit circle to itself. Fix z1 and define the MÃ¶bius transformations
         M ( z ) =     z  1   &#x2212; z   1 &#x2212;    z  1   &#x00AF;   z
      ,  &#x03C6; ( z ) =    f (  z  1   ) &#x2212; z   1 &#x2212;    f (  z  1
      )  &#x00AF;   z    .   {\displaystyle M(z)={\frac {z_{1}-z}{1-{\overline
      {z_{1}}}z}},\qquad \varphi (z)={\frac {f(z_{1})-z}{1-{\overline {f(z_
      {1})}}z}}.}  [M(z)={\frac  {z_{1}-z}{1-\overline {z_{1}}z}},\qquad
      \varphi (z)={\frac  {f(z_{1})-z}{1-\overline {f(z_{1})}z}}.]
Since M(z1) = 0 and the MÃ¶bius transformation is invertible, the composition
Ï(f(Mâ1(z))) maps 0 to 0 and the unit disk is mapped into itself. Thus we
can apply Schwarz's lemma, which is to say
          |  &#x03C6;  (  f (  M  &#x2212; 1   ( z ) )  )   |  =  |    f (  z
      1   ) &#x2212; f (  M  &#x2212; 1   ( z ) )   1 &#x2212;    f (  z  1   )
      &#x00AF;   f (  M  &#x2212; 1   ( z ) )    |  &#x2264;  |  z  |  .
      {\displaystyle \left|\varphi \left(f(M^{-1}(z))\right)\right|=\left|
      {\frac {f(z_{1})-f(M^{-1}(z))}{1-{\overline {f(z_{1})}}f(M^{-1}
      (z))}}\right|\leq |z|.}  [\left|\varphi \left(f(M^{{-1}}
      (z))\right)\right|=\left|{\frac  {f(z_{1})-f(M^{{-1}}(z))}{1-\overline {f
      (z_{1})}f(M^{{-1}}(z))}}\right|\leq |z|.]
Now calling z2 = Mâ1(z) (which will still be in the unit disk) yields the
desired conclusion
          |    f (  z  1   ) &#x2212; f (  z  2   )   1 &#x2212;    f (  z  1
      )  &#x00AF;   f (  z  2   )    |  &#x2264;  |     z  1   &#x2212;  z  2
      1 &#x2212;    z  1   &#x00AF;    z  2      |  .   {\displaystyle \left|
      {\frac {f(z_{1})-f(z_{2})}{1-{\overline {f(z_{1})}}f(z_{2})}}\right|\leq
      \left|{\frac {z_{1}-z_{2}}{1-{\overline {z_{1}}}z_{2}}}\right|.}  [\left|
      {\frac  {f(z_{1})-f(z_{2})}{1-\overline {f(z_{1})}f(z_{2})}}\right|\leq
      \left|{\frac  {z_{1}-z_{2}}{1-\overline {z_{1}}z_{2}}}\right|.]
To prove the second part of the theorem, we rearrange the left-hand side into
the difference quotient and let z2 tend to z1.
***** Further generalizations and related results[edit] *****
The SchwarzâAhlforsâPick_theorem provides an analogous theorem for
hyperbolic manifolds.
De_Branges'_theorem, formerly known as the Bieberbach Conjecture, is an
important extension of the lemma, giving restrictions on the higher derivatives
of f at 0 in case f is injective; that is, univalent.
The Koebe_1/4_theorem provides a related estimate in the case that f is
univalent.
***** References[edit] *****
   1. ^ Theorem 5.34 inRodriguez, Jane P. Gilman, Irwin Kra, Rubi E. (2007).
      Complex analysis : in the spirit of Lipman Bers ([Online] ed.). New York:
      Springer. p. 95. ISBN 978-0-387-74714-9.
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
    * Jurgen Jost, Compact Riemann Surfaces (2002), Springer-Verlag, New York.
ISBN 3-540-43299-X (See Section 2.3)
S. Dineen (1989). The Schwarz Lemma. Oxford. ISBN 0-19-853571-6.
This article incorporates material from Schwarz_lemma on PlanetMath, which is
licensed under the Creative_Commons_Attribution/Share-Alike_License.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Schwarz_lemma&oldid=882967219"
Categories:
    * Riemann_surfaces
    * Lemmas
    * Theorems_in_complex_analysis
Hidden categories:
    * Wikipedia_articles_incorporating_text_from_PlanetMath
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
    * Deutsch
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 12 February 2019, at 13:23 (UTC).
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
