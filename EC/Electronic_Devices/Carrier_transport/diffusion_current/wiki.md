The following text has been accessed from https://en.wikipedia.org/wiki/Diffusion_current at Fri Aug 9 03:39:21 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Diffusion current ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article needs attention from an expert in Physics. Please add a reason or
 a talk parameter to this template to explain the issue with the article.
 WikiProject_Physics may be able to help recruit an expert. (February 2019)
Diffusion Current is a current in a semiconductor caused by the diffusion of
charge carriers (holes and/or electrons). This is the current which is due to
the transport of charges occurring because of non-uniform concentration of
charged particles in a semiconductor. The drift current, by contrast, is due to
the motion of charge carriers due to the force exerted on them by an electric
field. Diffusion current can be in the same or opposite direction of a drift
current. The diffusion current and drift current together are described by the
driftâdiffusion_equation.[1]
It is necessary to consider the part of diffusion current when describing many
semiconductor devices. For example, the current near the depletion_region of a
pân_junction is dominated by the diffusion current. Inside the depletion
region, both diffusion current and drift current are present. At equilibrium in
a pân junction, the forward diffusion current in the depletion region is
balanced with a reverse drift current, so that the net current is zero.
The diffusion_constant for a doped material can be determined with the Haynes
â_Shockley_experiment. Alternatively, if the carrier mobility is known, the
diffusion coefficient may be determined from the Einstein_relation_on
electrical_mobility.
⁰
***** Contents *****
    * 1_Overview
          o 1.1_Diffusion_current_versus_drift_current
          o 1.2_Carrier_actions
    * 2_Derivation
    * 3_Example
    * 4_See_also
    * 5_References
***** Overview[edit] *****
**** Diffusion current versus drift current[edit] ****
Further information: Drift_current
The following table compares the two types of current:
      Diffusion current                    Drift current
      Diffusion current movement caused by Drift current movement caused by
      variation in the carrier             electric fields.
      concentration.
      Direction of the diffusion current   Direction of the drift current is
      depends on the slope of the carrier  always in the direction of the
      concentration.                       electric field.
      Obeys Fick's_law:     J = &#x2212; q Obeys Ohm's_law:     J = q &#x03C1;
      D    d &#x03C1;   d x                &#x03BC; E   {\displaystyle J=q\rho
      {\displaystyle J=-qD{\frac {d\rho }  \mu E}  [{\displaystyle J=q\rho \mu
      {dx}}}  [{\displaystyle J=-qD{\frac  E}]
      {d\rho }{dx}}}]
**** Carrier actions[edit] ****
No external electric field across the semiconductor is required for a diffusion
current to take place. This is because diffusion takes place due to the change
in concentration of the carrier particles and not the concentrations
themselves. The carrier particles, namely the holes and electrons of a
semiconductor, move from a place of higher concentration to a place of lower
concentration. Hence, due to the flow of holes and electrons there is a
current. This current is called the diffusion current. The drift current and
the diffusion current make up the total current in the conductor. The change in
the concentration of the carrier particles develops a gradient. Due to this
gradient, an electric field is produced in the semiconductor.
***** Derivation[edit] *****
 Some or all of the formulas presented in this article have missing or
 incomplete descriptions of their variables, symbols or constants which may
 create ambiguity or prevent full interpretation. Please assist in recruiting
 an expert or improve_this_article yourself. See the talk_page for details.
 (June 2012)
To derive the diffusion current in a semiconductor diode, the depletion layer
must be large compared to the mean free path. One begins with the equation for
the net current_density J in a semiconductor diode,
         J = q n &#x03BC; E + q D    d n   d x      {\displaystyle
      J=qn\mu E+qD{\frac {dn}{dx}}}  [                                (1)
      J = q n \mu E + q D\frac{dn}{dx}                                
      ]
where D is the diffusion_coefficient for the electron in the considered medium,
n is the number of electrons per unit volume (i.e. number density), q is the
magnitude of charge of an electron, Î¼ is electron mobility in the medium, and
E = âdÎ¦/dx (Î¦ potential difference) is the electric_field as the potential
gradient of the electric_potential. According to the Einstein_relation_on
electrical_mobility     D = &#x03BC;  V  t     {\displaystyle D=\mu V_{t}}  [
{\displaystyle D=\mu V_{t}}] and      V  t   = k T  /  q   {\displaystyle V_
{t}=kT/q}  [{\displaystyle V_{t}=kT/q}]. Thus, substituting E for the potential
gradient in the above equation (1) and multiplying both sides with exp(âÎ¦/
Vt), (1) becomes:
         J  e  &#x2212; &#x03A6;  /   V  t     = q D  (     &#x2212;
      n   V  t     &#x2217;    d &#x03A6;   d x    +    d n   d x
      )   e  &#x2212; &#x03A6;  /   V  t     = q D   d  d x    ( n  e
      &#x2212; &#x03A6;  /   V  t     )   {\displaystyle Je^{-\Phi /
      V_{t}}=qD\left({\frac {-n}{V_{t}}}*{\frac {d\Phi }{dx}}+{\frac     
      {dn}{dx}}\right)e^{-\Phi /V_{t}}=qD{\frac {d}{dx}}(ne^{-\Phi /       (2)
      V_{t}})}  [
      J e^{-\Phi / V_t} = q D\left(\frac{-n}{V_t}*\frac{d\Phi}{dx} +
      \frac{dn}{dx}\right)e^{-\Phi / V_t} = q D  \frac{d}{dx}(n e^{-
      \Phi / V_t})
      ]
Integrating equation (2) over the depletion region gives
         J =    q D n  e  &#x2212; &#x03A6;  /   V  t        |    0    x  d
      &#x222B;  0    x  d      e  &#x2212; &#x03A6;  /   V  t     d x
      {\displaystyle J={\frac {qDne^{-\Phi /V_{t}}{\big |}_{0}^{x_{d}}}{\int _
      {0}^{x_{d}}e^{-\Phi /V_{t}}dx}}}  [J = \frac{q D n e^{-\Phi /
      V_t}\big|_0^{x_d}}{\int_0^{x_d} e^{-\Phi / V_t}dx}]
which can be written as
         J =    q D  N  c    e  &#x2212;  &#x03A6;  B    /   V  t
      [   e   V  a    /   V  t     &#x2212; 1  ]     &#x222B;  0    x
      d      e  &#x2212;  &#x03A6;  &#x2217;    /   V  t     d x
      {\displaystyle J={\frac {qDN_{c}e^{-\Phi _{B}/V_{t}}\left[e^{V_    
      {a}/V_{t}}-1\right]}{\int _{0}^{x_{d}}e^{-\Phi ^{*}/V_{t}}dx}}}      (3)
      [
      J = \frac{ q D N_c e^{-\Phi_B/ V_t}\left[e^{V_a/ V_t} -
      1\right]}{\int_0^{x_d} e^{-\Phi^*/ V_t} dx}
      ]
where
          &#x03A6;  &#x2217;   =  &#x03A6;  B   +  &#x03A6;  i   &#x2212;  V  a
      {\displaystyle \Phi ^{*}=\Phi _{B}+\Phi _{i}-V_{a}}  [\Phi^* = \Phi_B +
      \Phi_i - V_a]
The denominator in equation (3) can be solved by using the following equation:
         &#x03A6; = &#x2212;    q  N  d     2  E  s   ( x &#x2212;  x  d    )
      2        {\displaystyle \Phi =-{\frac {qN_{d}}{2E_{s}(x-x_{d})^{2}}}}
      [\Phi = - \frac{q N_d}{2E_s (x - x_d)^2}]
Therefore, Î¦* can be written as:
          &#x03A6;  &#x2217;   =    q  N  d   x   E  s      (   x  d
      &#x2212;   x 2    )  = (  &#x03A6;  i   &#x2212;  V  a   )   x
      x  d       {\displaystyle \Phi ^{*}={\frac {qN_{d}x}{E_
      {s}}}\left(x_{d}-{\frac {x}{2}}\right)=(\Phi _{i}-V_{a}){\frac     (4)
      {x}{x_{d}}}}  [                                                    
      \Phi^* = \frac{q N_d x}{E_s} \left(x_d - \frac{x}{2}\right) =
      (\Phi_i - V_a)\frac{x}{x_d}
      ]
Since the x << xd the term (xd â x/2) â xd, using this approximation
equation (3) is solved as follows:
          &#x222B;  0    x  d      e  &#x2212;  &#x03A6;  &#x2217;    /   V  t
      d x =  x  d       &#x03A6;  i   &#x2212;  V  a     V  t
      {\displaystyle \int _{0}^{x_{d}}e^{-\Phi ^{*}/V_{t}}dx=x_{d}{\frac {\Phi
      _{i}-V_{a}}{V_{t}}}}  [\int_0^{x_d} e^{-\Phi^* / V_t}dx = x_d \frac
      {\Phi_i - V_a}{V_t}],
since (Î¦i â Va) > Vt. One obtains the equation of current caused due to
diffusion:
         J =     q  2   D  N  c     V  t       [     2 q   E  s
      (  &#x03A6;  i   &#x2212;  V  a   )  N  d    ]   1  /  2    e
      &#x2212;  &#x03A6;  B    /   V  t     (  e   V  a    /   V  t
      &#x2212; 1 )   {\displaystyle J={\frac {q_{2}DN_{c}}{V_            
      {t}}}\left[{\frac {2q}{E_{s}}}(\Phi _{i}-V_{a})N_{d}\right]^{1/      (5)
      2}e^{-\Phi _{B}/V_{t}}(e^{V_{a}/V_{t}}-1)}  [
      J = \frac{q_2 D N_c}{V_t} \left[\frac{2q}{E_s}( \Phi_i - V_a)
      N_d\right]^{1/2} e^{-\Phi_B / V_t}(e^{V_a / V_t} - 1)
      ]
From equation (5), one can observe that the current depends exponentially on
the input voltage Va, also the barrier height Î¦B. From equation (5), Va can be
written as the function of electric field intensity, which is as follows:
          E   m a x    =   [     2 q   E  s     (  &#x03A6;  i
      &#x2212;  V  a   )  N  d    ]   1  /  2     {\displaystyle E_
      {\mathrm {max} }=\left[{\frac {2q}{E_{s}}}(\Phi _{i}-V_{a})N_    
      {d}\right]^{1/2}}  [                                               (6)
      E_\mathrm{max} = \left[\frac{2q}{E_s} (\Phi_i - V_a)
      N_d\right]^{1/2}
      ]
Substituting equation (6) in equation (5) gives:
         J = q &#x03BC;  E   m a x     N  c    e  &#x2212;  &#x03A6;
      B    /   V  t     (  e   V  a    /   V  t     &#x2212; 1 )
      {\displaystyle J=q\mu E_{\mathrm {max} }N_{c}e^{-\Phi _{B}/V_     
      {t}}(e^{V_{a}/V_{t}}-1)}  [                                         (7)
      J = q \mu E_\mathrm{max} N_c e^{-\Phi_B  / V_t}(e^{V_a/V_t} -
      1)
      ]
From equation (7), one can observe that when a zero voltage is applied to the
semi-conductor diode, the drift current totally balances the diffusion current.
Hence, the net current in a semiconductor diode at zero potential is always
zero.
As carriers are generated (green:electrons and purple:holes) due to light
shining at the center of an intrinsic semiconductor, they diffuse towards two
ends. Electrons have higher diffusion constant than holes leading to fewer
excess electrons at the center as compared to holes.
***** Example[edit] *****
The equation above can be applied to model semiconductor devices. When the
density of electrons is not in equilibrium, diffusion of electrons will occur.
For example, when a bias is applied to two ends of a chunk of semiconductor, or
a light is shining in one place (see right figure), electron will diffuse from
high density regions (center) to low density regions (two ends), forming a
gradient of electron density. This process generates diffusion current.
***** See also[edit] *****
    * Alternating_current
    * Conduction_band
    * Convectionâdiffusion_equation
    * Direct_current
    * Drift_current
    * Free_electron_model
    * Random_walk
    * Maximal_Entropy_Random_Walk - diffusion in agreement with quantum
      predictions
***** References[edit] *****
   1. ^ McGraw Hill Encyclopaedia of Physics (2nd Edition), C.B. Parker, 1994,
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
   3. ISBN 0-07-051400-3
    * Encyclopaedia of Physics (2nd Edition), R.G. Lerner, G.L. Trigg, VHC
      publishers, 1991, ISBN (Verlagsgesellschaft) 3-527-26954-1, ISBN (VHC
      Inc.) 0-89573-752-3
    * Concepts of Modern Physics (4th Edition), A. Beiser, Physics, McGraw-Hill
      (International), 1987,
ISBN 0-07-100144-1
Solid State Physics (2nd Edition), J.R. Hook, H.E. Hall, Manchester Physics
Series, John Wiley & Sons, 2010,
ISBN 978_0_471_92804_1
Ben G. Streetman, Santay Kumar Banerjee; Solid State Electronic Devices (6th
Edition), Pearson International Edition; pp. 126â135.
"Differences_between_diffusion_current". Diffusion. Archived from the_original
on 13 August 2017. Retrieved 10 September 2011.
"Carrier_Actions_of_Diffusion_Current". Diffusion. Archived from the_original
on 10 August 2011. Retrieved 11 October 2011.
"derivation_of_difussion_current". Archived from the_original on 14 December
2011. Retrieved 15 October 2011.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Diffusion_current&oldid=907800774"
Categories:
    * Semiconductors
Hidden categories:
    * Articles_needing_expert_attention_with_no_reason_or_talk_parameter
    * Articles_needing_expert_attention_from_February_2019
    * All_articles_needing_expert_attention
    * Physics_articles_needing_expert_attention
    * Articles_needing_expert_attention_from_June_2012
    * Wikipedia_articles_needing_factual_verification_from_June_2012
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
    * Italiano
    * æ¥æ¬èª
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 25 July 2019, at 11:14 (UTC).
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
