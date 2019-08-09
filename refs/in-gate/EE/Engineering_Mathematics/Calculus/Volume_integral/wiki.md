The following text has been accessed from https://en.wikipedia.org/wiki/Volume_integral at Thu Aug 8 22:51:03 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Volume integral ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Part of a series of articles about
Calculus
    * Fundamental_theorem
    * Limits_of_functions
    * Continuity
    * Mean_value_theorem
    * Rolle's_theorem
Differential
Definitions
    * Derivative (generalizations)
    * Differential
          o infinitesimal
          o of_a_function
          o total
Concepts
    * Differentiation_notation
    * Second_derivative
    * Third_derivative
    * Change_of_variables
    * Implicit_differentiation
    * Related_rates
    * Taylor's_theorem
Rules_and_identities
    * Sum
    * Product
    * Chain
    * Power
    * Quotient
    * Inverse
    * General_Leibniz
    * FaÃ _di_Bruno's_formula
Integral
    * Lists_of_integrals
Definitions
    * Antiderivative
    * Integral (improper)
    * Riemann_integral
    * Lebesgue_integration
    * Contour_integration
Integration by
    * Parts
    * Discs
    * Cylindrical_shells
    * Substitution (trigonometric)
    * Partial_fractions
    * Order
    * Reduction_formulae
Series
    * Geometric (arithmetico-geometric)
    * Harmonic
    * Alternating
    * Power
    * Binomial
    * Taylor
Convergence_tests
    * Summand_limit_(term_test)
    * Ratio
    * Root
    * Integral
    * Direct_comparison
    *
      Limit_comparison
    * Alternating_series
    * Cauchy_condensation
    * Dirichlet
    * Abel
Vector
    * Gradient
    * Divergence
    * Curl
    * Laplacian
    * Directional_derivative
    * Identities
Theorems
    * Divergence
    * Gradient
    * Green's
    * KelvinâStokes
    * Stokes
Multivariable
Formalisms
    * Matrix
    * Tensor
    * Exterior
    * Geometric
Definitions
    * Partial_derivative
    * Multiple_integral
    * Line_integral
    * Surface_integral
    * Volume integral
    * Jacobian
    * Hessian
Specialized
    * Fractional
    * Malliavin
    * Stochastic
    * Variations
Glossary_of_calculus
    * Glossary_of_calculus
    * v
    * t
    * e
In mathematics—in particular, in multivariable_calculus—a volume integral
refers to an integral over a 3-dimensional domain, that is, it is a special
case of multiple_integrals. Volume integrals are especially important in
physics for many applications, for example, to calculate flux densities.
⁰
***** Contents *****
    * 1_In_coordinates
    * 2_Example_1
    * 3_See_also
    * 4_External_links
***** In coordinates[edit] *****
It can also mean a triple_integral within a region     D &#x2282;   R   3
{\displaystyle D\subset \mathbb {R} ^{3}}  [{\displaystyle D\subset \mathbb {R}
^{3}}] of a function     f ( x , y , z ) ,   {\displaystyle f(x,y,z),}  [f
(x,y,z),] and is usually written as:
          &#x222D;  D   f ( x , y , z )  d x  d y  d z .   {\displaystyle
      \iiint _{D}f(x,y,z)\,dx\,dy\,dz.}  [{\displaystyle \iiint _{D}f
      (x,y,z)\,dx\,dy\,dz.}]
A volume integral in cylindrical_coordinates is
          &#x222D;  D   f ( &#x03C1; , &#x03C6; , z ) &#x03C1;  d &#x03C1;  d
      &#x03C6;  d z ,   {\displaystyle \iiint _{D}f(\rho ,\varphi ,z)\rho
      \,d\rho \,d\varphi \,dz,}  [{\displaystyle \iiint _{D}f(\rho ,\varphi
      ,z)\rho \,d\rho \,d\varphi \,dz,}]
and a volume integral in spherical_coordinates (using the ISO convention for
angles with     &#x03C6;   {\displaystyle \varphi }  [\varphi ] as the azimuth
and     &#x03B8;   {\displaystyle \theta }  [\theta ] measured from the polar
axis (see more on conventions)) has the form
          &#x222D;  D   f ( r , &#x03B8; , &#x03C6; )  r  2   sin &#x2061;
      &#x03B8;  d r  d &#x03B8;  d &#x03C6; .   {\displaystyle \iiint _{D}f
      (r,\theta ,\varphi )r^{2}\sin \theta \,dr\,d\theta \,d\varphi .}  [
      {\displaystyle \iiint _{D}f(r,\theta ,\varphi )r^{2}\sin \theta
      \,dr\,d\theta \,d\varphi .}]
***** Example 1[edit] *****
Integrating the function     f ( x , y , z ) = 1   {\displaystyle f(x,y,z)=1}
[f(x,y,z)=1] over a unit cube yields the following result:
          &#x222B;  0   1    &#x222B;  0   1    &#x222B;  0   1   1  d x  d y
      d z =  &#x222B;  0   1    &#x222B;  0   1   ( 1 &#x2212; 0 )  d y  d z =
      &#x222B;  0   1   ( 1 &#x2212; 0 ) d z = 1 &#x2212; 0 = 1
      {\displaystyle \int _{0}^{1}\int _{0}^{1}\int _{0}^{1}1\,dx\,dy\,dz=\int
      _{0}^{1}\int _{0}^{1}(1-0)\,dy\,dz=\int _{0}^{1}(1-0)dz=1-0=1}  [
      {\displaystyle \int _{0}^{1}\int _{0}^{1}\int _{0}^{1}1\,dx\,dy\,dz=\int
      _{0}^{1}\int _{0}^{1}(1-0)\,dy\,dz=\int _{0}^{1}(1-0)dz=1-0=1}]
So the volume of the unit cube is 1 as expected. This is rather trivial
however, and a volume integral is far more powerful. For instance if we have a
scalar density function on the unit cube then the volume integral will give the
total mass of the cube. For example for density function:
           {    f :   R   3   &#x2192;  R      ( x , y , z ) &#x27FC; x + y + z
      {\displaystyle {\begin{cases}f:\mathbb {R} ^{3}\to \mathbb {R} \\
      (x,y,z)\longmapsto x+y+z\end{cases}}}  [{\displaystyle {\begin{cases}f:
      \mathbb {R} ^{3}\to \mathbb {R} \\(x,y,z)\longmapsto x+y+z\end{cases}}}]
the total mass of the cube is:
          &#x222B;  0   1    &#x222B;  0   1    &#x222B;  0   1   ( x + y + z )
      d x  d y  d z =  &#x222B;  0   1    &#x222B;  0   1    (    1 2   + y + z
      )   d y  d z =  &#x222B;  0   1   ( 1 + z )  d z =   3 2
      {\displaystyle \int _{0}^{1}\int _{0}^{1}\int _{0}^{1}
      (x+y+z)\,dx\,dy\,dz=\int _{0}^{1}\int _{0}^{1}\left({\frac {1}
      {2}}+y+z\right)\,dy\,dz=\int _{0}^{1}(1+z)\,dz={\frac {3}{2}}}  [
      {\displaystyle \int _{0}^{1}\int _{0}^{1}\int _{0}^{1}
      (x+y+z)\,dx\,dy\,dz=\int _{0}^{1}\int _{0}^{1}\left({\frac {1}
      {2}}+y+z\right)\,dy\,dz=\int _{0}^{1}(1+z)\,dz={\frac {3}{2}}}]
***** See also[edit] *****
    * [icon]Mathematics_portal
    * Divergence_theorem
    * Surface_integral
    * Volume_element
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Multiple_integral", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Weisstein,_Eric_W. "Volume_integral". MathWorld.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Volume_integral&oldid=901116574"
Categories:
    * Multivariable_calculus
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
    * Deutsch
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * Italiano
    * áá¶áá¶ááááá
    * PortuguÃªs
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Tiáº¿ng_Viá»t
Edit_links
    * This page was last edited on 9 June 2019, at 20:17 (UTC).
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
