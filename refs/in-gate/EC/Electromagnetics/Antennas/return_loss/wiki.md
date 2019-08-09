The following text has been accessed from https://en.wikipedia.org/wiki/Return_loss at Fri Aug 9 03:43:01 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Return loss ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In telecommunications, return loss is the loss of power in the signal returned/
reflected by a discontinuity in a transmission_line or optical_fiber. This
discontinuity can be a mismatch with the terminating load or with a device
inserted in the line. It is usually expressed as a ratio in decibels (dB);
         R L (  d B  ) = 10  log  10   &#x2061;    P   i     P   r
      {\displaystyle RL(\mathrm {dB} )=10\log _{10}{P_{\mathrm {i} } \over P_
      {\mathrm {r} }}}  [RL(\mathrm{dB}) = 10 \log_{10} {P_\mathrm i \over
      P_\mathrm r}]
      where RL(dB) is the return loss in dB, Pi is the incident power and Pr is
      the reflected power.
Return loss is related to both standing_wave_ratio (SWR) and reflection
coefficient (Î). Increasing return loss corresponds to lower SWR. Return loss
is a measure of how well devices or lines are matched. A match is good if the
return loss is high. A high return loss is desirable and results in a lower
insertion_loss.
Return loss is used in modern practice in preference to SWR because it has
better resolution for small values of reflected wave.[1]
⁰
***** Contents *****
    * 1_Sign
    * 2_Electrical
    * 3_Optical
    * 4_See_also
    * 5_Notes
    * 6_References
***** Sign[edit] *****
Properly, loss quantities, when expressed in decibels, should be positive
numbers.[note_1] However, return loss has historically been expressed as a
negative number, and this convention is still widely found in the literature.
[1]
The correct definition of return loss is the difference in dB between the
incident power sent towards the Device Under Test (DUT) and the power
reflected, resulting in a positive sign:
         R L (  d B  ) = 10  log  10   &#x2061;    P   i     P   r
      {\displaystyle RL(\mathrm {dB} )=10\log _{10}{P_{\mathrm {i} } \over P_
      {\mathrm {r} }}}  [RL(\mathrm{dB}) = 10 \log_{10} {P_\mathrm i \over
      P_\mathrm r}]
However taking the ratio of reflected to incident power results in a negative
sign for return loss;
         R  L &#x2032;  (  d B  ) = 10  log  10   &#x2061;    P   r     P   i
      {\displaystyle RL'(\mathrm {dB} )=10\log _{10}{P_{\mathrm {r} } \over P_
      {\mathrm {i} }}}  [RL'(\mathrm{dB}) = 10 \log_{10} {P_\mathrm r \over
      P_\mathrm i}]
      where RL'(dB) is the negative of RL(dB).
Return loss with a positive sign is identical to the magnitude of Î when
expressed in decibels but of opposite sign. That is, return loss with a
negative sign is more properly called reflection coefficient.[1] The S-
parameter S11 from two-port_network theory is frequently also called return
loss,[2] but is actually equal to Î.
Caution is required when discussing increasing or decreasing return loss since
these terms strictly have the opposite meaning when return loss is defined as a
negative quantity.
***** Electrical[edit] *****
In metallic conductor systems, reflections of a signal traveling down a
conductor can occur at a discontinuity or impedance mismatch. The ratio of the
amplitude of the reflected wave Vr to the amplitude of the incident wave Vi is
known as the reflection_coefficient     &#x0393;   {\displaystyle \Gamma }
[\Gamma ].
           &#x0393;   =    V   r     V   i        {\displaystyle {\mathit
      {\Gamma }}={V_{\mathrm {r} } \over V_{\mathrm {i} }}}  [\mathit \Gamma =
      {V_\mathrm r \over V_\mathrm i}]
When the source and load impedances are known values, the reflection
coefficient is given by
           &#x0393;   =     Z   L    &#x2212;  Z   S       Z   L    +  Z   S
      {\displaystyle {\mathit {\Gamma }}={{Z_{\mathrm {L} }-Z_{\mathrm {S} }}
      \over {Z_{\mathrm {L} }+Z_{\mathrm {S} }}}}  [\mathit \Gamma = {
      {Z_\mathrm L - Z_\mathrm S} \over {Z_\mathrm L + Z_\mathrm S} }]
where ZS is the impedance toward the source and ZL is the impedance toward the
load.
Return loss is the negative of the magnitude of the reflection coefficient in
dB. Since power is proportional to the square of the voltage, return loss is
given by,
         R L (  d B  ) = &#x2212; 20  log  10   &#x2061;  |   &#x0393;   |
      {\displaystyle RL(\mathrm {dB} )=-20\log _{10}\left|{\mathit {\Gamma
      }}\right|}  [RL(\mathrm{dB}) = -20 \log_{10} \left| \mathit \Gamma
      \right|]
where the vertical bars indicate magnitude. Thus, a large positive return loss
indicates the reflected power is small relative to the incident power, which
indicates good impedance match from source to load.
When the actual transmitted (incident) power and the reflected power are known
(i.e., through measurements and/or calculations), then the return loss in dB
can be calculated as the difference between the incident power Pi (in absolute
decibel units, e.g., dBm) and the reflected power Pr (also in absolute decibel
units),
         R L (  d B  ) =  P   i    (  d B  ) &#x2212;  P   r    (  d B  )
      {\displaystyle RL(\mathrm {dB} )=P_{\mathrm {i} }(\mathrm {dB} )-P_
      {\mathrm {r} }(\mathrm {dB} )\,}  [{\displaystyle RL(\mathrm {dB} )=P_
      {\mathrm {i} }(\mathrm {dB} )-P_{\mathrm {r} }(\mathrm {dB} )\,}]
***** Optical[edit] *****
In optics (particularly in fiberoptics) a loss that takes place at
discontinuities of refractive_index, especially at an air-glass interface such
as a fiber endface. At those interfaces, a fraction of the optical signal is
reflected back toward the source. This reflection phenomenon is also called
"Fresnel_reflection loss," or simply "Fresnel loss."
Fiber optic transmission systems use lasers to transmit signals over optical
fiber, and a high optical return loss (ORL) can cause the laser to stop
transmitting correctly. The measurement of ORL is becoming more important in
the characterization of optical networks as the use of wavelength-division
multiplexing increases. These systems use lasers that have a lower tolerance
for ORL, and introduce elements into the network that are located in close
proximity to the laser.
          ORL  (  d B  ) = 10  log  10   &#x2061;    P   i     P   r
      {\displaystyle {\text{ORL}}(\mathrm {dB} )=10\log _{10}{P_{\mathrm {i} }
      \over P_{\mathrm {r} }}}  [\text{ORL}(\mathrm{dB}) = 10 \log_{10}
      {P_\mathrm i \over P_\mathrm r}]
where       P   r       {\displaystyle \scriptstyle P_{\mathrm {r} }}
[\scriptstyle P_\mathrm r] is the reflected power and       P   i
{\displaystyle \scriptstyle P_{\mathrm {i} }}  [\scriptstyle P_\mathrm i] is
the incident, or input, power.
***** See also[edit] *****
    * Hybrid_balance
    * Mismatch_loss
    * Signal_reflection
    * Time-domain_reflectometer
          o Optical_time_domain_reflectometer
***** Notes[edit] *****
   1. ^ Except for cases where an active device succeeds in reflecting back
      more power than was sent into it. This is the case, for instance, with
      the tunnel_diode_amplifier.
***** References[edit] *****
  Notes
   1. ^ a b c Trevor S. Bird, "Definition_and_Misuse_of_Return_Loss", IEEE
      Antennas & Propagation Magazine, vol.51, iss.2, pp.166-167, April 2009.
   2. ^ Noel G. Barton, Jacques Periaux, "Coupling of fluids, structures, and
      waves in aeronautics", proceedings of a French-Australian workshop in
      Melbourne, Australia, 3â6 December 2001, p.187, Springer, 2003
   3. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   4. ISBN 3-540-40222-5.
  Bibliography
    * Federal_Standard_1037C and from MIL-STD-188
    * Optical_Return_Loss_TestingâEnsuring_High-Quality_Transmission EXFO
      Application note #044

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Return_loss&oldid=887880844"
Categories:
    * Wave_mechanics
    * Radio_electronics
    * Engineering_ratios
    * Electrical_parameters
    * Fiber_optics
Hidden categories:
    * Use_dmy_dates_from_September_2010
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
    * EspaÃ±ol
    * Bahasa_Indonesia
    * Italiano
    * æ¥æ¬èª
    * Polski
Edit_links
    * This page was last edited on 15 March 2019, at 12:40 (UTC).
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
