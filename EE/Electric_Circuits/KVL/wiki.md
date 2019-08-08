The following text has been accessed from https://en.wikipedia.org/wiki/Kirchhoff%27s_circuit_laws#Kirchhoff&#039;s_voltage_law_(KVL) at Thu Aug 8 22:53:41 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Kirchhoff's circuit laws ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other laws named after Gustav Kirchhoff, see Kirchhoff's_laws_
(disambiguation).
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (November 2017)(Learn_how_and
 when_to_remove_this_template_message)
Kirchhoff's laws are two equalities that deal with the current and potential
difference (commonly known as voltage) in the lumped_element_model of
electrical_circuits. They were first described in 1845 by German physicist
Gustav_Kirchhoff.[1] This generalized the work of Georg_Ohm and preceded the
work of James_Clerk_Maxwell. Widely used in electrical_engineering, they are
also called Kirchhoff's rules or simply Kirchhoff's laws. These laws can be
applied in time and frequency domains and form the basis for network_analysis.
Both of Kirchhoff's laws can be understood as corollaries of Maxwell's
equations in the low-frequency limit. They are accurate for DC circuits, and
for AC circuits at frequencies where the wavelengths of electromagnetic
radiation are very large compared to the circuits.
⁰
***** Contents *****
    * 1_Kirchhoff's_current_law_(KCL)
          o 1.1_Uses
    * 2_Kirchhoff's_voltage_law_(KVL)
          o 2.1_Generalization
    * 3_Limitations
    * 4_Example
    * 5_See_also
    * 6_References
    * 7_External_links
***** Kirchhoff's current law (KCL)[edit] *****
The current entering any junction is equal to the current leaving that
junction. i2 + i3 = i1 + i4
This law is also called Kirchhoff's first law, Kirchhoff's point rule, or
Kirchhoff's junction rule (or nodal rule).
This law states that, for any node (junction) in an electrical_circuit, the sum
of currents flowing into that node is equal to the sum of currents flowing out
of that node; or equivalently:
     The algebraic sum of currents in a network of conductors meeting at a
     point is zero.
Recalling that current is a signed (positive or negative) quantity reflecting
direction towards or away from a node, this principle can be succinctly stated
as:
          &#x2211;  k = 1   n     I   k   = 0   {\displaystyle \sum _{k=1}^{n}
      {I}_{k}=0}  [\sum _{k=1}^{n}{I}_{k}=0]
where n is the total number of branches with currents flowing towards or away
from the node.
The law is based on the conservation of charge where the charge (measured in
coulombs) is the product of the current (in amperes) and the time (in seconds).
If the net charge in a region is constant, the KCL will hold on the boundaries
of the region.[2][3] This means that KCL relies on the fact that the net charge
in the wires and components is constant.
**** Uses[edit] ****
A matrix version of Kirchhoff's current law is the basis of most circuit
simulation_software, such as SPICE. Kirchhoff's current law is used with Ohm's
law to perform nodal_analysis.
KCL is applicable to any lumped network irrespective of the nature of the
network; whether unilateral or bilateral, active or passive, linear or non-
linear.
***** Kirchhoff's voltage law (KVL)[edit] *****
The sum of all the voltages around a loop is equal to zero.
v1 + v2 + v3 +v4 = 0
This law is also called Kirchhoff's second law, Kirchhoff's loop (or mesh)
rule, and Kirchhoff's second rule.
This law states that
     The directed sum of the potential_differences (voltages) around any
     closed loop is zero.
Similarly to KCL, it can be stated as:
          &#x2211;  k = 1   n    V  k   = 0   {\displaystyle \sum _{k=1}^{n}V_
      {k}=0}  [\sum _{k=1}^{n}V_{k}=0]
Here, n is the total number of voltages measured.
Derivation of Kirchhoff's voltage law
A similar derivation can be found in The Feynman Lectures on Physics, Volume
II, Chapter 22: AC Circuits.[3]

Consider some arbitrary circuit. Approximate the circuit with lumped elements,
so that (time-varying) magnetic fields are contained to each component and the
field in the region exterior to the circuit is negligible. Based on this
assumption, the Maxwell-Faraday_equation reveals that
   &#x2207; &#x00D7;  E  = &#x2212;    &#x2202;  B    &#x2202; t    =  0
{\displaystyle \nabla \times \mathbf {E} =-{\frac {\partial \mathbf {B} }
{\partial t}}=\mathbf {0} }  [{\displaystyle \nabla \times \mathbf {E} =-{\frac
{\partial \mathbf {B} }{\partial t}}=\mathbf {0} }]
in the exterior region. If each of the components have a finite volume, then
the exterior region is simply_connected, and thus the electric field is
conservative in that region. Therefore, for any loop in the circuit, we find
that
   &#x2211;  V  i   = &#x2212; &#x2211;  &#x222B;     P    i      E  &#x22C5;
d   l  =    &#x222E;      &#x2061;  E  &#x22C5;  d   l  = 0   {\displaystyle
\sum V_{i}=-\sum \int _{{\mathcal {P}}_{i}}\mathbf {E} \cdot \mathrm {d}
\mathbf {l} =\oint \mathbf {E} \cdot \mathrm {d} \mathbf {l} =0}  [
{\displaystyle \sum V_{i}=-\sum \int _{{\mathcal {P}}_{i}}\mathbf {E} \cdot
\mathrm {d} \mathbf {l} =\oint \mathbf {E} \cdot \mathrm {d} \mathbf {l} =0}]
where        P    i     {\textstyle {\mathcal {P}}_{i}}  [{\textstyle {\mathcal
{P}}_{i}}] are paths around the exterior of each of the components, from one
terminal to another.
**** Generalization[edit] ****
In the low-frequency limit, the voltage drop around any loop is zero. This
includes imaginary loops arranged arbitrarily in space â not limited to the
loops delineated by the circuit elements and conductors. In the low-frequency
limit, this is a corollary of Faraday's_law_of_induction (which is one of
Maxwell's_equations).
This has practical application in situations involving "static_electricity".
***** Limitations[edit] *****
KCL and KVL both depend on the lumped_element_model being applicable to the
circuit in question. When the model is not applicable, the laws do not apply.
KCL and KVL result from the assumptions of the lumped element model.
KCL is dependent on the assumption that the net charge in any wire, junction or
lumped component is constant. Whenever the electric field between parts of the
circuit is non-negligible, such as when two wires are capacitively_coupled,
this may not be the case. This occurs in high-frequency AC circuits, where the
lumped element model is no longer applicable.[4] For example, in a transmission
line, the charge density in the conductor will constantly be oscillating.
In a transmission line, the net charge in different parts of the conductor
changes with time. In the direct physical sense, this violates KCL.
On the other hand, KVL relies on the fact that the action of time-varying
magnetic fields are confined to individual components, such as inductors. In
reality, the induced electric field produced by an inductor is not confined,
but the leaked fields are often negligible.
Modelling real circuits with lumped elements
The lumped element approximation for a circuit is accurate at low enough
frequencies. At higher frequencies, leaked fluxes and varying charge densities
in conductors become significant. To an extent, it is possible to still model
such circuits using parasitic_components. If frequencies are too high, it may
be more appropriate to simulate the fields directly using finite_element
modelling or other_techniques.
To model circuits so that KVL and KCL can still be used, it's important to
understand the distinction between physical circuit elements and the ideal
lumped elements. For example, a wire is not an ideal conductor. Unlike an ideal
conductor, wires can inductively and capacitively couple to each other (and to
themselves), and have a finite propagation delay. Real conductors can be
modeled in terms of lumped elements by considering parasitic_capacitances
distributed between the conductors to model capacitive coupling, or parasitic_
(mutual)_inductances to model inductive coupling.[4] Wires also have some self-
inductance, which is the reason that decoupling_capacitors are necessary.
***** Example[edit] *****
[Kirshhoff-example.svg]
Assume an electric network consisting of two voltage sources and three
resistors.
According to the first law we have
          i  1   &#x2212;  i  2   &#x2212;  i  3   = 0    {\displaystyle i_{1}-
      i_{2}-i_{3}=0\,}  [i_{1}-i_{2}-i_{3}=0\,]
The second law applied to the closed circuit s1 gives
         &#x2212;  R  2    i  2   +    E    1   &#x2212;  R  1    i  1   = 0
      {\displaystyle -R_{2}i_{2}+{\mathcal {E}}_{1}-R_{1}i_{1}=0}  [-R_{2}i_
      {2}+{\mathcal {E}}_{1}-R_{1}i_{1}=0]
The second law applied to the closed circuit s2 gives
         &#x2212;  R  3    i  3   &#x2212;    E    2   &#x2212;    E    1   +
      R  2    i  2   = 0   {\displaystyle -R_{3}i_{3}-{\mathcal {E}}_{2}-
      {\mathcal {E}}_{1}+R_{2}i_{2}=0}  [-R_{3}i_{3}-{\mathcal {E}}_{2}-
      {\mathcal {E}}_{1}+R_{2}i_{2}=0]
Thus we get a system_of_linear_equations in      i  1   ,  i  2   ,  i  3
{\displaystyle i_{1},i_{2},i_{3}}  [i_{1},i_{2},i_{3}]:
           {     i  1   &#x2212;  i  2   &#x2212;  i  3     = 0     &#x2212;  R
      2    i  2   +    E    1   &#x2212;  R  1    i  1     = 0     &#x2212;  R
      3    i  3   &#x2212;    E    2   &#x2212;    E    1   +  R  2    i  2
      = 0         {\displaystyle {\begin{cases}i_{1}-i_{2}-i_{3}&=0\\-R_{2}i_
      {2}+{\mathcal {E}}_{1}-R_{1}i_{1}&=0\\-R_{3}i_{3}-{\mathcal {E}}_{2}-
      {\mathcal {E}}_{1}+R_{2}i_{2}&=0\end{cases}}}  [{\begin{cases}i_{1}-i_
      {2}-i_{3}&=0\\-R_{2}i_{2}+{\mathcal {E}}_{1}-R_{1}i_{1}&=0\\-R_{3}i_{3}-
      {\mathcal {E}}_{2}-{\mathcal {E}}_{1}+R_{2}i_{2}&=0\end{cases}}]
Which is equivalent to
           {     i  1   + ( &#x2212;  i  2   ) + ( &#x2212;  i  3   )   = 0
      R  1    i  1   +  R  2    i  2   + 0  i  3     =    E    1       0  i  1
      +  R  2    i  2   &#x2212;  R  3    i  3     =    E    1   +    E    2
      {\displaystyle {\begin{cases}i_{1}+(-i_{2})+(-i_{3})&=0\\R_{1}i_{1}+R_
      {2}i_{2}+0i_{3}&={\mathcal {E}}_{1}\\0i_{1}+R_{2}i_{2}-R_{3}i_{3}&=
      {\mathcal {E}}_{1}+{\mathcal {E}}_{2}\end{cases}}}  [{\displaystyle
      {\begin{cases}i_{1}+(-i_{2})+(-i_{3})&=0\\R_{1}i_{1}+R_{2}i_{2}+0i_{3}&=
      {\mathcal {E}}_{1}\\0i_{1}+R_{2}i_{2}-R_{3}i_{3}&={\mathcal {E}}_{1}+
      {\mathcal {E}}_{2}\end{cases}}}]
Assuming
          R  1   = 100 &#x03A9; , &#xA0;  R  2   = 200 &#x03A9; , &#xA0;  R  3
      = 300 &#x03A9;   {\displaystyle R_{1}=100\Omega ,\ R_{2}=200\Omega ,\ R_
      {3}=300\Omega }  [{\displaystyle R_{1}=100\Omega ,\ R_{2}=200\Omega ,\ R_
      {3}=300\Omega }]
            E    1   = 3  V  ,    E    2   = 4  V    {\displaystyle {\mathcal
      {E}}_{1}=3{\text{V}},{\mathcal {E}}_{2}=4{\text{V}}}  [{\displaystyle
      {\mathcal {E}}_{1}=3{\text{V}},{\mathcal {E}}_{2}=4{\text{V}}}]
the solution is
           {     i  1   =   1 1100    A       i  2   =   4 275    A       i  3
      = &#x2212;   3 220    A          {\displaystyle {\begin{cases}i_{1}=
      {\frac {1}{1100}}{\text{A}}\\[6pt]i_{2}={\frac {4}{275}}{\text{A}}\\
      [6pt]i_{3}=-{\frac {3}{220}}{\text{A}}\end{cases}}}  [{\displaystyle
      {\begin{cases}i_{1}={\frac {1}{1100}}{\text{A}}\\[6pt]i_{2}={\frac {4}
      {275}}{\text{A}}\\[6pt]i_{3}=-{\frac {3}{220}}{\text{A}}\end{cases}}}]
    i  3     {\displaystyle i_{3}}  [i_{3}] has a negative sign, which means
that the direction of      i  3     {\displaystyle i_{3}}  [i_{3}] is opposite
to the assumed direction i.e.      i  3     {\displaystyle i_{3}}  [i_{3}] is
directed upwards.
***** See also[edit] *****
    * [icon]Electronics_portal
    * Faraday's_law_of_induction
    * Lumped_matter_discipline
***** References[edit] *****
   1. ^Oldham, Kalil T. Swain (2008). The doctrine of description: Gustav
      Kirchhoff, classical physics, and the "purpose of all science" in 19th-
      century Germany (Ph. D.). University of California, Berkeley. p. 52.
      Docket 3331743.
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
   3. ^Athavale, Prashant. "Kirchoff's_current_law_and_Kirchoff's_voltage_law"
      (PDF). Johns Hopkins University. Retrieved 6 December 2018.
   4. ^ a b"The_Feynman_Lectures_on_Physics_Vol._II_Ch._22:_AC_Circuits".
      www.feynmanlectures.caltech.edu. Retrieved 2018-12-06.
   5. ^ a b Ralph Morrison, Grounding and Shielding Techniques in
      Instrumentation Wiley-Interscience (1986)
   6. ISBN 0471838055
    * Paul, Clayton R. (2001). Fundamentals of Electric Circuit Analysis. John
      Wiley & Sons. ISBN 0-471-37195-5.
Serway, Raymond A.; Jewett, John W. (2004). Physics for Scientists and
Engineers (6th ed.). Brooks/Cole. ISBN 0-534-40842-7.
Tipler, Paul (2004). Physics for Scientists and Engineers: Electricity,
Magnetism, Light, and Elementary Modern Physics (5th ed.). W. H. Freeman.
ISBN 0-7167-0810-8.
Graham, Howard Johnson, Martin (2002). High-speed signal propagation : advanced
black magic (10. printing. ed.). Upper Saddle River, NJ: Prentice Hall PTR.
ISBN 0-13-084408-X.
***** External links[edit] *****
 Wikimedia Commons has media related to Kirchhoff's_circuit_laws.
    * Divider_Circuits_and_Kirchhoff's_Laws chapter from Lessons_In_Electric
      Circuits_Vol_1_DC free ebook and Lessons_In_Electric_Circuits series.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Kirchhoff%27s_circuit_laws&oldid=908246444"
Categories:
    * Circuit_theorems
    * Conservation_equations
    * Linear_electronic_circuits
    * Voltage
    * 1845_in_science
    * Gustav_Kirchhoff
Hidden categories:
    * Articles_lacking_in-text_citations_from_November_2017
    * All_articles_lacking_in-text_citations
    * Commons_category_link_is_on_Wikidata
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * á áá­á
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LatvieÅ¡u
    * Limburgs
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * ÙØµØ±Ù
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * PiemontÃ¨is
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Sardu
    * à·à·à¶à·à¶½
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 28 July 2019, at 13:19 (UTC).
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
