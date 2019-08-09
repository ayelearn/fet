The following text has been accessed from https://en.wikipedia.org/wiki/Geopotential at Fri Aug 9 01:58:59 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Geopotential ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
                        This article relies largely or entirely on a single
[Question_book-new.svg] source. Relevant discussion may be found on the talk
                        page. Please help improve_this_article by introducing
                        citations to additional sources. (July 2014)
 It has been suggested that Geopotential_model be merged into this article.
 (Discuss)Proposed since November 2018.
Geopotential is the potential of the Earth's gravity_field. For convenience it
is often defined as the negative of the potential_energy per unit mass, so that
the gravity vector is obtained as the gradient of this potential, without the
negation.
⁰
***** Contents *****
    * 1_Definition
    * 2_Mathematical_formula
    * 3_See_also
    * 4_References
***** Definition[edit] *****
For geophysical applications, gravity is distinguished from gravitation.
Gravity is defined as the resultant of gravitation and the centrifugal_force
caused by the Earth's_rotation. The global_mean_sea_surface is close to one of
the equipotential surfaces of the geopotential of gravity     W
{\displaystyle W}  [W]. This equipotential surface, or surface of constant
geopotential, is called the geoid.[1]. How the gravitational force and the
centrifugal force add up to a force orthogonal to the geoid is illustrated in
the figure (not to scale). At latitude 50 deg the off-set between the
gravitational force (red line in the figure) and the local vertical (green line
in the figure) is in fact 0.098 deg. For a mass point (atmosphere) in motion
the centrifugal force no more matches the gravitational and the vector sum is
not exactly orthogonal to the Earth surface. This is the cause of the coriolis
effect for atmospheric motion.
Balance between gravitational and centrifugal force on the Earth surface
.
The geoid is a gently undulating surface due to the irregular mass distribution
inside the Earth; it may be approximated however by an ellipsoid_of_revolution
called the reference_ellipsoid. The currently most widely used reference
ellipsoid, that of the Geodetic Reference System 1980 (GRS80), approximates the
geoid to within a little over Â±100 m. One can construct a simple model
geopotential     U   {\displaystyle U}  [U] that has as one of its
equipotential surfaces this reference ellipsoid, with the same model potential
U  0     {\displaystyle U_{0}}  [U_{0}] as the true potential      W  0
{\displaystyle W_{0}}  [W_{0}] of the geoid; this model is called a normal
potential. The difference     T = W &#x2212; U   {\displaystyle T=W-U}  [T=W-U]
is called the disturbing potential. Many observable quantities of the gravity
field, such as gravity anomalies and deflections of the plumbline, can be
expressed in this disturbing potential.
In practical terrestrial work, e.g., levelling, an alternative version of the
geopotential is used called geopotential number     C   {\displaystyle C}  [C],
which are reckoned from the geoid upward:
         C = &#x2212; ( W &#x2212;  W  0   )   {\displaystyle C=-(W-W_{0})}
      [C=-(W-W_{0})],
where      W  0     {\displaystyle W_{0}}  [W_{0}] is the geopotential of the
geoid.
***** Mathematical formula[edit] *****
For the purpose of satellite orbital_mechanics, the geopotential is typically
described by a series expansion into spherical_harmonics (spectral
representation). In this context the geopotential is taken as the potential of
the gravitational field of the Earth, that is, leaving out the centrifugal
potential.
Solving for geopotential (Î¦) in the simple case of a sphere:
         &#x03A6; ( h ) =  &#x222B;  0   h   g  d z &#xA0;   {\displaystyle
      \Phi (h)=\int _{0}^{h}g\,dz\ }  [\Phi (h)=\int _{0}^{h}g\,dz\ ][2]
         &#x03A6; =  &#x222B;  0   z    [    G m   ( a + z  )  2      ]  d z
      {\displaystyle \Phi =\int _{0}^{z}\left[{\frac {Gm}{(a+z)^{2}}}\right]dz}
      [\Phi =\int _{0}^{z}\left[{\frac  {Gm}{(a+z)^{2}}}\right]dz]
Integrate to get
         &#x03A6; = G m  [    1 a   &#x2212;   1  a + z     ]    {\displaystyle
      \Phi =Gm\left[{\frac {1}{a}}-{\frac {1}{a+z}}\right]}  [\Phi =Gm\left[
      {\frac  {1}{a}}-{\frac  {1}{a+z}}\right]]
where:
      G=6.673x10â11 Nm2/kg2 is the gravitational constant,
      m=5.975x1024 kg is the mass of the earth,
      a=6.378x106 m is the average radius of the earth,
      z is the height in meters
      Î¦ is the geopotential at height z, which is in units of [m2/s2] or [J/
      kg].
***** See also[edit] *****
    * Geoid
    * Physical_geodesy
    * Geopotential_height
    * Geopotential_model
***** References[edit] *****
   1. ^Heiskanen,_Weikko_Aleksanteri; Moritz, Helmut (1967). Physical Geodesy.
      W.H._Freeman. ISBN 0-7167-0233-9.
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
   3. ^Holton,_James_R. (2004). An Introduction to Dynamic Meteorology (4th
      ed.). Burlington: Elsevier. ISBN 0-12-354015-1.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Geopotential&oldid=878186806"
Categories:
    * Gravimetry
Hidden categories:
    * Articles_needing_additional_references_from_July_2014
    * All_articles_needing_additional_references
    * Articles_to_be_merged_from_November_2018
    * All_articles_to_be_merged
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
    * Italiano
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 13 January 2019, at 15:24 (UTC).
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
