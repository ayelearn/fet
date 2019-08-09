The following text has been accessed from https://en.wikipedia.org/wiki/Maximum_modulus_principle at Fri Aug 9 02:37:43 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Maximum modulus principle ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
A plot of the modulus of cos(z) (in red) for z in the unit_disk centered at the
origin (shown in blue). As predicted by the theorem, the maximum of the modulus
cannot be inside of the disk (so the highest value on the red surface is
somewhere along its edge).
In mathematics, the maximum modulus principle in complex_analysis states that
if f is a holomorphic_function, then the modulus |f | cannot exhibit a true
local_maximum that is properly within the domain of f.
In other words, either f is a constant_function, or, for any point z0 inside
the domain of f there exist other points arbitrarily close to z0 at which |f |
takes larger values.
⁰
***** Contents *****
    * 1_Formal_statement
    * 2_Sketches_of_proofs
          o 2.1_Using_the_maximum_principle_for_harmonic_functions
          o 2.2_Using_Gauss's_mean_value_theorem
    * 3_Physical_interpretation
    * 4_Applications
    * 5_References
    * 6_External_links
***** Formal statement[edit] *****
Let f be a function holomorphic on some connected open subset D of the complex
plane â and taking complex values. If z0 is a point in D such that
          |  f (  z  0   )  |  &#x2265;  |  f ( z )  |    {\displaystyle |f(z_
      {0})|\geq |f(z)|}  [|f(z_{0})|\geq |f(z)|]
for all z in a neighborhood of z0, then the function f is constant on D.
By switching to the reciprocal, we can get the minimum modulus principle. It
states that if f is holomorphic within a bounded domain D, continuous up to the
boundary of D, and non-zero at all points, then |f(z)| takes its minimum value
on the boundary of D.
Alternatively, the maximum modulus principle can be viewed as a special case of
the open_mapping_theorem, which states that a nonconstant holomorphic function
maps open sets to open sets. If |f| attains a local maximum at z, then the
image of a sufficiently small open neighborhood of z cannot be open. Therefore,
f is constant.
***** Sketches of proofs[edit] *****
**** Using the maximum principle for harmonic functions[edit] ****
One can use the equality
         log &#x2061; f ( z ) = ln &#x2061;  |  f ( z )  |  + i arg &#x2061; f
      ( z )   {\displaystyle \log f(z)=\ln |f(z)|+i\arg f(z)}  [{\displaystyle
      \log f(z)=\ln |f(z)|+i\arg f(z)}]
for complex natural_logarithms to deduce that ln |f(z)| is a harmonic_function.
Since z0 is a local maximum for this function also, it follows from the maximum
principle that |f(z)| is constant. Then, using the CauchyâRiemann_equations
we show that fâ²(z) = 0, and thus that f(z) is constant as well. Similar
reasoning shows that |f| can only have a local minimum (which necessarily has
value 0) at an isolated zero of f(z).
**** Using Gauss's mean value theorem[edit] ****
Another proof works by using Gauss's mean value theorem to "force" all points
within overlapping open disks to assume the same value. The disks are laid such
that their centers form a polygonal path from the value where f(z) is maximized
to any other point in the domain, while being totally contained within the
domain. Thus the existence of a maximum value implies that all the values in
the domain are the same, thus f(z) is constant.
***** Physical interpretation[edit] *****
A physical interpretation of this principle comes from the heat_equation. That
is, since log |f(z)| is harmonic, it is thus the steady state of a heat flow on
the region D. Suppose a strict maximum was attained on the interior of D, the
heat at this maximum would be dispersing to the points around it, which would
contradict the assumption that this represents the steady state of a system.
***** Applications[edit] *****
The maximum modulus principle has many uses in complex analysis, and may be
used to prove the following:
    * The fundamental_theorem_of_algebra.
    * Schwarz's_lemma, a result which in turn has many generalisations and
      applications in complex analysis.
    * The PhragmÃ©nâLindelÃ¶f_principle, an extension to unbounded domains.
    * The BorelâCarathÃ©odory_theorem, which bounds an analytic function in
      terms of its real part.
    * The Hadamard_three-lines_theorem, a result about the behaviour of bounded
      holomorphic functions on a line between two other parallel lines in the
      complex plane.
***** References[edit] *****
    * Titchmarsh,_E._C. (1939). The Theory of Functions (2nd ed.). Oxford
      University Press.
 (See chapter 5.)
E. D. Solomentsev (2001) [1994], "Maximum-modulus_principle", in Hazewinkel,
Michiel (ed.), Encyclopedia_of_Mathematics, Springer Science+Business Media
B.V. / Kluwer Academic Publishers, ISBN 978-1-55608-010-4
***** External links[edit] *****
    * Weisstein,_Eric_W. "Maximum_Modulus_Principle". MathWorld.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Maximum_modulus_principle&oldid=848845825"
Categories:
    * Mathematical_principles
    * Theorems_in_complex_analysis
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
    * EspaÃ±ol
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * æ¥æ¬èª
    * Ð ÑÑÑÐºÐ¸Ð¹
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 4 July 2018, at 19:07 (UTC).
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
