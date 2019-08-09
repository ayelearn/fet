The following text has been accessed from https://en.wikipedia.org/wiki/Instrumentation_amplifier at Fri Aug 9 01:27:10 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Instrumentation amplifier ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
electronic amplifier, a circuit component
This article is about amplifiers for measurement and electronic test equipment.
For amplifiers for musical instruments, see instrument_amplifier.
Typical instrumentation amplifier schematic
An instrumentation (or instrumentational) amplifier (sometimes shorthanded as
In-Amp or InAmp) is a type of differential_amplifier that has been outfitted
with input buffer_amplifiers, which eliminate the need for input impedance
matching and thus make the amplifier particularly suitable for use in
measurement and test_equipment. Additional characteristics include very low DC
offset, low drift, low noise, very high open-loop_gain, very high common-mode
rejection_ratio, and very high input_impedances. Instrumentation amplifiers are
used where great accuracy and stability of the circuit both short and long-term
are required.
Although the instrumentation amplifier is usually shown schematically identical
to a standard operational_amplifier (op-amp), the electronic instrumentation
amp is almost always internally composed of 3 op-amps. These are arranged so
that there is one op-amp to buffer each input (+,â), and one to produce the
desired output with adequate impedance matching for the function.[1][2]
The most commonly used instrumentation amplifier circuit is shown in the
figure. The gain of the circuit is
           A  v    =    V   o u t      V  2   &#x2212;  V  1      =  (  1 +
      2  R  1     R   g a i n       )     R  3    R  2       {\displaystyle {A_
      {v}}={\frac {V_{\mathrm {out} }}{V_{2}-V_{1}}}=\left(1+{2R_{1} \over R_
      {\mathrm {gain} }}\right){R_{3} \over R_{2}}}  [{\displaystyle {A_{v}}=
      {\frac {V_{\mathrm {out} }}{V_{2}-V_{1}}}=\left(1+{2R_{1} \over R_
      {\mathrm {gain} }}\right){R_{3} \over R_{2}}}]
The rightmost amplifier, along with the resistors labelled      R  2
{\displaystyle R_{\text{2}}}  [R_{{{\text{2}}}}] and      R  3
{\displaystyle R_{\text{3}}}  [R_{{{\text{3}}}}] is just the standard
differential amplifier circuit, with gain =      R  3    /   R  2
{\displaystyle R_{\text{3}}/R_{\text{2}}}  [R_{\text{3}}/R_{\text{2}}] and
differential input resistance = 2Â·     R  2     {\displaystyle R_{\text{2}}}
[R_{{{\text{2}}}}]. The two amplifiers on the left are the buffers. With      R
gain     {\displaystyle R_{\text{gain}}}  [R_{{{\text{gain}}}}] removed (open
circuited), they are simple unity gain buffers; the circuit will work in that
state, with gain simply equal to      R  3    /   R  2     {\displaystyle R_
{\text{3}}/R_{\text{2}}}  [R_{\text{3}}/R_{\text{2}}] and high input impedance
because of the buffers. The buffer gain could be increased by putting resistors
between the buffer inverting inputs and ground to shunt away some of the
negative feedback; however, the single resistor      R  gain     {\displaystyle
R_{\text{gain}}}  [R_{{{\text{gain}}}}] between the two inverting inputs is a
much more elegant method: it increases the differential-mode gain of the buffer
pair while leaving the common-mode gain equal to 1. This increases the common-
mode_rejection_ratio (CMRR) of the circuit and also enables the buffers to
handle much larger common-mode signals without clipping than would be the case
if they were separate and had the same gain. Another benefit of the method is
that it boosts the gain using a single resistor rather than a pair, thus
avoiding a resistor-matching problem, and very conveniently allowing the gain
of the circuit to be changed by changing the value of a single resistor. A set
of switch-selectable resistors or even a potentiometer can be used for      R
gain     {\displaystyle R_{\text{gain}}}  [R_{{{\text{gain}}}}], providing easy
changes to the gain of the circuit, without the complexity of having to switch
matched pairs of resistors.
The ideal common-mode gain of an instrumentation amplifier is zero. In the
circuit shown, common-mode gain is caused by mismatch in the resistor ratios
R  2    /   R  3     {\displaystyle R_{\text{2}}/R_{\text{3}}}  [R_{\text{2}}/
R_{\text{3}}] and by the mis-match in common mode gains of the two input op-
amps. Obtaining very closely matched resistors is a significant difficulty in
fabricating these circuits, as is optimizing the common mode performance.[3]
An instrumentation amp can also be built with two op-amps to save on cost, but
the gain must be higher than two (+6 dB).[4][5]
Instrumentation amplifiers can be built with individual op-amps and precision
resistors, but are also available in integrated_circuit form from several
manufacturers (including Texas_Instruments, Analog_Devices, Linear_Technology
and Maxim_Integrated_Products). An IC instrumentation amplifier typically
contains closely matched laser-trimmed resistors, and therefore offers
excellent common-mode rejection. Examples include INA128, AD8221, LT1167 and
MAX4194.
Instrumentation Amplifiers can also be designed using "Indirect Current-
feedback Architecture", which extend the operating range of these amplifiers to
the negative power supply rail, and in some cases the positive power supply
rail. This can be particularly useful in single-supply systems, where the
negative power rail is simply the circuit ground (GND). Examples of parts
utilizing this architecture are MAX4208/MAX4209 and AD8129/AD8130.
⁰
***** Contents *****
    * 1_Types
          o 1.1_Feedback-free_instrumentation_amplifier
    * 2_See_also
    * 3_References
    * 4_External_links
***** Types[edit] *****
**** Feedback-free instrumentation amplifier[edit] ****
Feedback-free instrumentation amplifier is the high input impedance
differential amplifier designed without the external feedback network. This
allows reduction in the number of amplifiers (one instead of three), reduced
noise (no thermal noise is brought on by the feedback resistors) and increased
bandwidth (no frequency compensation is needed). Chopper stabilized (or zero
drift) instrumentation amplifiers such as the LTC2053 use a switching input
front end to eliminate DC offset errors and drift.
***** See also[edit] *****
    * [icon]Electronics_portal
    * Isolation_amplifier
    * Operational_amplifier_applications
***** References[edit] *****
   1. ^ R.F. Coughlin, F.F. Driscoll Operational Amplifiers and Linear
      Integrated Circuits (2nd Ed.1982.
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
   3. ISBN 0-13-637785-8) p.161.
   4. ^ Moore, Davis, Coplan Building Scientific Apparatus (2nd Ed. 1989
   5. ISBN 0-201-13189-7)p.407.
   6. ^ Smither, Pugh and Woolard: âCMRR Analysis of the 3-op-amp
      instrumentation amplifier', Electronics letters, Volume 13, Issue 20, 29
      September 1977, page 594.
   7. ^"Don't_fall_in_love_with_one_type_of_instrumentation_amp_-_2002-05-30
      07:00:00". EDN. Retrieved 28 October 2014.
   8. ^"Amplifiers_for_bioelectric_events:_a_design_with_a_minimal_number_of
      parts". Biosemi.com. Retrieved 3 October 2011.
***** External links[edit] *****
 Wikimedia Commons has media related to Instrumentation_amplifiers.
    * Interactive_analysis_of_the_Instrumentation_Amplifier
    * Opamp_Instrumentation_Amplifier
    * The_instrumentation_amplifier
    * Lessons_In_Electric_Circuits_â_Volume_III_â_The_instrumentation
      amplifier
    * A_Practical_Review_of_Common_Mode_and_Instrumentation_Amplifiers (PDF)
    * The_Instrumentation_Amplifier
    * A_Designer's_Guide_to_Instrumentation_Amplifiers_(3rd_Edition)
    * Three_is_a_Crowd_for_Instrumentation_Amplifiers
    * Instrumentation_Amplifier_Solutions,_Circuits_and_Applications
    * Fixed-gain_CMOS_differential_amplifiers_with_no_external_feedback_for_a
      wide_temperature_range_(Cryogenics)

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Instrumentation_amplifier&oldid=905814466"
Categories:
    * Electronic_amplifiers
Hidden categories:
    * Articles_with_short_description
    * Use_dmy_dates_from_July_2014
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * CatalÃ 
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Euskara
    * FranÃ§ais
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 11 July 2019, at 16:25 (UTC).
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
