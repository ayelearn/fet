The following text has been accessed from https://en.wikipedia.org/wiki/Electric_displacement_field at Thu Aug 8 22:55:36 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Electric displacement field ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Vector field related to displacement current and flux density
In physics, the electric displacement field, denoted by D, is a vector_field
that appears in Maxwell's_equations. It accounts for the effects of free_and
bound_charge within materials. "D" stands for "displacement", as in the related
concept of displacement_current in dielectrics. In free_space, the electric
displacement field is equivalent to flux_density, a concept that lends
understanding to Gauss's_law. In the International_System_of_Units (SI), it is
expressed in units of coulomb per meter square (C⋅mâ2).
⁰
***** Contents *****
    * 1_Definition
    * 2_History
    * 3_Example:_Displacement_field_in_a_capacitor
    * 4_See_also
    * 5_References
***** Definition[edit] *****
In a dielectric material, the presence of an electric_field E causes the bound
charges in the material (atomic nuclei and their electrons) to slightly
separate, inducing a local electric_dipole_moment. The electric displacement
field "D" is defined as
          D  &#x2261;  &#x03B5;  0    E  +  P  ,   {\displaystyle \mathbf {D}
      \equiv \varepsilon _{0}\mathbf {E} +\mathbf {P} ,}  [\mathbf{D} \equiv
      \varepsilon_{0} \mathbf{E} + \mathbf{P},]
where      &#x03B5;  0     {\displaystyle \varepsilon _{0}}  [\varepsilon_{0}]
is the vacuum_permittivity (also called permittivity of free space), and P is
the (macroscopic) density of the permanent and induced electric dipole moments
in the material, called the polarization_density.
The displacement field satisfies Gauss's_law in a dielectric:
         &#x2207; &#x22C5;  D  = &#x03C1; &#x2212;  &#x03C1;  b   =  &#x03C1;
      f     {\displaystyle \nabla \cdot \mathbf {D} =\rho -\rho _{\text
      {b}}=\rho _{\text{f}}}  [ \nabla\cdot\mathbf{D} = \rho -\rho_\text{b} =
      \rho_\text{f} ]
In this equation,      &#x03C1;  f     {\displaystyle \rho _{\text{f}}}  [
{\displaystyle \rho _{\text{f}}}] is the number of free charges per unit
volume. These charges are the ones that have made the volume non-neutral, and
they are sometimes referred to as the space_charge. This equation says, in
effect, that the flux lines of D must begin and end on the free charges. In
contrast      &#x03C1;  b     {\displaystyle \rho _{\text{b}}}  [{\displaystyle
\rho _{\text{b}}}] is the density of all those charges that are part of a
dipole, each of which is neutral. In the example of an insulating dielectric
between metal capacitor plates, the only free charges are on the metal plates
and dielectric contains only dipoles. If the dielectric is replaced by a doped
semiconductor or an ionised gas, etc, then electrons move relative to the ions,
and if the system is finite they both contribute to      &#x03C1;  f
{\displaystyle \rho _{\text{f}}}  [{\displaystyle \rho _{\text{f}}}] at the
edges.
Proof
Separate the total volume charge density into free and bound charges:
         &#x03C1; =  &#x03C1;  f   +  &#x03C1;  b     {\displaystyle \rho =\rho
      _{\text{f}}+\rho _{\text{b}}}  [ \rho = \rho_\text{f} + \rho_\text{b} ]
The density can be rewritten as a function of the polarization P:
         &#x03C1; =  &#x03C1;  f   &#x2212; &#x2207; &#x22C5;  P  .
      {\displaystyle \rho =\rho _{\text{f}}-\nabla \cdot \mathbf {P} .}  [ \rho
      = \rho_\text{f} -\nabla\cdot\mathbf{P}. ]
The polarization P is defined to be a vector field whose divergence yields the
density of bound charges Ïb in the material. The electric field satisfies the
equation:
         &#x2207; &#x22C5;  E  =   1  &#x03B5;  0     &#x03C1; =   1  &#x03B5;
      0     (  &#x03C1;  f   &#x2212; &#x2207; &#x22C5;  P  )   {\displaystyle
      \nabla \cdot \mathbf {E} ={\frac {1}{\varepsilon _{0}}}\rho ={\frac {1}
      {\varepsilon _{0}}}(\rho _{\text{f}}-\nabla \cdot \mathbf {P} )}
      [\nabla\cdot\mathbf{E} = \frac{1}{\varepsilon_0} \rho = \frac{1}
      {\varepsilon_0}(\rho_\text{f} -\nabla\cdot\mathbf{P})]
and hence
         &#x2207; &#x22C5; (  &#x03B5;  0    E  +  P  ) =  &#x03C1;  f
      {\displaystyle \nabla \cdot (\varepsilon _{0}\mathbf {E} +\mathbf {P}
      )=\rho _{\text{f}}}  [\nabla\cdot (\varepsilon_0\mathbf{E} + \mathbf{P})
      = \rho_\text{f} ]
Electrostatic forces on ions or electrons in the material are governed by the
electric field E in the material via the Lorentz_Force. Also, D is not
determined exclusively by the free charge. As E has a curl of zero in
electrostatic situations, it follows that
         &#x2207; &#x00D7;  D  = &#x2207; &#x00D7;  P    {\displaystyle \nabla
      \times \mathbf {D} =\nabla \times \mathbf {P} }  [\nabla \times \mathbf
      {D} = \nabla \times \mathbf{P}]
The effect of this equation can be seen in the case of an object with a "frozen
in" polarization like a bar electret, the electric analogue to a bar magnet.
There is no free charge in such a material, but the inherent polarization gives
rise to an electric field, demonstrating that the D field is not determined
entirely by the free charge. The electric field is determined by using the
above relation along with other boundary conditions on the polarization_density
to yield the bound charges, which will, in turn, yield the electric field.
In a linear, homogeneous, isotropic dielectric with instantaneous response to
changes in the electric field, P depends linearly on the electric field,
          P  =  &#x03B5;  0   &#x03C7;  E  ,   {\displaystyle \mathbf {P}
      =\varepsilon _{0}\chi \mathbf {E} ,}  [\mathbf{P} = \varepsilon_{0} \chi
      \mathbf{E},]
where the constant of proportionality     &#x03C7;   {\displaystyle \chi }
[\chi ] is called the electric_susceptibility of the material. Thus
          D  =  &#x03B5;  0   ( 1 + &#x03C7; )  E  = &#x03B5;  E
      {\displaystyle \mathbf {D} =\varepsilon _{0}(1+\chi )\mathbf {E}
      =\varepsilon \mathbf {E} }  [\mathbf{D} = \varepsilon_{0} (1+\chi)
      \mathbf{E} = \varepsilon \mathbf{E}]
where Îµ = Îµ0 Îµr is the permittivity, and Îµr = 1 + Ï the relative
permittivity of the material.
In linear, homogeneous, isotropic media, Îµ is a constant. However, in linear
anisotropic media it is a tensor, and in nonhomogeneous media it is a function
of position inside the medium. It may also depend upon the electric field
(nonlinear materials) and have a time dependent response. Explicit time
dependence can arise if the materials are physically moving or changing in time
(e.g. reflections off a moving interface give rise to Doppler_shifts). A
different form of time dependence can arise in a time-invariant medium, as
there can be a time delay between the imposition of the electric field and the
resulting polarization of the material. In this case, P is a convolution of the
impulse_response susceptibility Ï and the electric field E. Such a convolution
takes on a simpler form in the frequency_domain: by Fourier_transforming the
relationship and applying the convolution_theorem, one obtains the following
relation for a linear_time-invariant medium:
          D ( &#x03C9; )  = &#x03B5; ( &#x03C9; )  E  ( &#x03C9; ) ,
      {\displaystyle \mathbf {D(\omega )} =\varepsilon (\omega )\mathbf {E}
      (\omega ),}  [ \mathbf{D(\omega)} = \varepsilon (\omega) \mathbf{E}
      (\omega) , ]
where     &#x03C9;   {\displaystyle \omega }  [\omega ] is the frequency of the
applied field. The constraint of causality leads to the KramersâKronig
relations, which place limitations upon the form of the frequency dependence.
The phenomenon of a frequency-dependent permittivity is an example of material
dispersion. In fact, all physical materials have some material dispersion
because they cannot respond instantaneously to applied fields, but for many
problems (those concerned with a narrow enough bandwidth) the frequency-
dependence of Îµ can be neglected.
At a boundary,     (   D  1    &#x2212;   D  2    ) &#x22C5;     n  &#x005E;
=  D  1 , &#x22A5;   &#x2212;  D  2 , &#x22A5;   =  &#x03C3;  f
{\displaystyle (\mathbf {D_{1}} -\mathbf {D_{2}} )\cdot {\hat {\mathbf {n}
}}=D_{1,\perp }-D_{2,\perp }=\sigma _{\text{f}}}  [(\mathbf{D_1} - \mathbf
{D_2})\cdot \hat{\mathbf{n}} = D_{1,\perp} - D_{2,\perp} = \sigma_\text{f} ],
where Ïf is the free charge density and the unit normal        n &#x005E;
{\displaystyle \mathbf {\hat {n}} }  [\mathbf {\hat {n}} ] points in the
direction from medium 2 to medium 1.[1]
***** History[edit] *****
Gauss's law was formulated by Carl Friedrich Gauss in 1835, but was not
published until 1867[citation_needed], meaning that the formulation and use of
D were not earlier than 1835, and probably not earlier than the 1860s.
The earliest known use of the term is from the year 1864, in James Clerk
Maxwell's paper A Dynamical Theory of the Electromagnetic Field. Maxwell used
calculus to exhibit Michael Faraday's theory, that light is an electromagnetic
phenomenon. Maxwell introduced the term D, specific capacity of electric
induction, in a form different from the modern and familiar notations.[2]
It was Oliver_Heaviside who reformulated the complicated Maxwell's equations to
the modern form. It wasn't until 1884 that Heaviside, concurrently with Willard
Gibbs and Heinrich Hertz, grouped the equations together into a distinct set.
This group of four equations was known_variously as the HertzâHeaviside
equations and the MaxwellâHertz equations, and is sometimes still known as
the MaxwellâHeaviside equations; hence, it was probably Heaviside who lent D
the present significance it now has.
***** Example: Displacement field in a capacitor[edit] *****
A parallel plate capacitor. Using an imaginary box, it is possible to use
Gauss's law to explain the relationship between electric displacement and free
charge.
Consider an infinite parallel plate capacitor where the space between the
plates is empty or contains a neutral, insulating medium. In this case there
are no free charges present except on the metal capacitor plates. Since the
flux lines D end on free charges, and there are the same number of uniformly
distributed charges of opposite sign on both plates, then the flux lines must
all simply traverse the capacitor from one side to the other, and |D| = 0
outside the capacitor. In SI units, the charge density on the plates is equal
to the value of the D field between the plates. This follows directly from
Gauss's_law, by integrating over a small rectangular box straddling one plate
of the capacitor:
      [\oiint]        A      {\displaystyle \scriptstyle _{A}}  [{\displaystyle
      \scriptstyle _{A}}]      D  &#x22C5;  d   A  =  Q  f r e e
      {\displaystyle \mathbf {D} \cdot \mathrm {d} \mathbf {A} =Q_{free}}  [
      {\displaystyle \mathbf {D} \cdot \mathrm {d} \mathbf {A} =Q_{free}}]
On the sides of the box, dA is perpendicular to the field, so the integral over
this section is zero, as is the integral on the face that is outside the
capacitor where D is zero. The only surface that contributes to the integral is
therefore the surface of the box inside the capacitor, and hence
          |   D   |  A =  |   Q  free    |    {\displaystyle |\mathbf {D}
      |A=|Q_{\text{free}}|}  [{\displaystyle |\mathbf {D} |A=|Q_{\text
      {free}}|}],
where A is the surface area of the top face of the box and      Q  free    /  A
=  &#x03C1;  f     {\displaystyle Q_{\text{free}}/A=\rho _{f}}  [{\displaystyle
Q_{\text{free}}/A=\rho _{f}}] is the free surface charge density on the
positive plate. If the space between the capacitor plates is filled with a
linear homogeneous isotropic dielectric with permittivity     &#x03B5; =
&#x03B5;  0    &#x03B5;  r     {\displaystyle \varepsilon =\varepsilon _
{0}\varepsilon _{r}}  [{\displaystyle \varepsilon =\varepsilon _{0}\varepsilon
_{r}}], then there is a polarization induced in the medium,      D  =  &#x03B5;
0    E  +  P  = &#x03B5;  E    {\displaystyle \mathbf {D} =\varepsilon _
{0}\mathbf {E} +\mathbf {P} =\varepsilon \mathbf {E} }  [{\displaystyle \mathbf
{D} =\varepsilon _{0}\mathbf {E} +\mathbf {P} =\varepsilon \mathbf {E} }] and
so the voltage difference between the plates is
         V =  |   E   |  d =     |   D   |  d  &#x03B5;   =     |   Q  free
      |  d   &#x03B5; A      {\displaystyle V=|\mathbf {E} |d={\frac {|\mathbf
      {D} |d}{\varepsilon }}={\frac {|Q_{\text{free}}|d}{\varepsilon A}}}  [
      {\displaystyle V=|\mathbf {E} |d={\frac {|\mathbf {D} |d}{\varepsilon }}=
      {\frac {|Q_{\text{free}}|d}{\varepsilon A}}}]
where d is their separation.
Introducing the dielectric increases Îµ by a factor      &#x03B5;  r
{\displaystyle \varepsilon _{r}}  [\varepsilon _{r}] and either the voltage
difference between the plates will be smaller by this factor, or the charge
must be higher. The partial cancellation of fields in the dielectric allows a
larger amount of free charge to dwell on the two plates of the capacitor per
unit potential drop than would be possible if the plates were separated by
vacuum.
If the distance d between the plates of a finite parallel plate capacitor is
much smaller than its lateral dimensions we can approximate it using the
infinite case and obtain its capacitance as
         C =    Q  free   V   &#x2248;    Q  free     |   E   |  d    =   A d
      &#x03B5; ,   {\displaystyle C={\frac {Q_{\text{free}}}{V}}\approx {\frac
      {Q_{\text{free}}}{|\mathbf {E} |d}}={\frac {A}{d}}\varepsilon ,}  [C =
      \frac{Q_\text{free}}{V} \approx \frac{Q_\text{free}}{|\mathbf{E}| d} =
      \frac{A}{d} \varepsilon,]
***** See also[edit] *****
    * History_of_Maxwell's_equations#The_term_Maxwell's_equations
    * Polarization_density
    * Electric_susceptibility
    * Magnetizing_field
    * Electric_dipole_moment
***** References[edit] *****
   1. ^David Griffiths. Introduction to Electrodynamics (3rd 1999 ed.).
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
   3. ^ A Dynamical Theory of the Electromagnetic Field PART V. â THEORY OF
      CONDENSERS, page 494[full_citation_needed]

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Electric_displacement_field&oldid=905789691"
Categories:
    * Electric_and_magnetic_fields_in_matter
Hidden categories:
    * Articles_with_incomplete_citations_from_July_2017
    * Use_American_English_from_March_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_March_2016
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
    * Boarisch
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * á¥áá áá£áá
    * Magyar
    * à¤®à¤°à¤¾à¤ à¥
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 11 July 2019, at 12:47 (UTC).
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
