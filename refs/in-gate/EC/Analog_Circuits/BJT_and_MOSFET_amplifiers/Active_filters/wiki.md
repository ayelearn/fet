The following text has been accessed from https://en.wikipedia.org/wiki/Active_filter at Fri Aug 9 03:37:19 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Active filter ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article has multiple issues. Please help improve_it or discuss these issues on the talk_page. (Learn_how
 and_when_to_remove_these_template_messages)
  This article needs additional citations for verification. Please help improve_this_article by adding_citations_to_reliable
  sources. Unsourced material may be challenged and removed.
  Find sources: "Active_filter" â news Â· newspapers Â· books Â· scholar Â· JSTOR (November 2011)(Learn_how_and_when_to
  remove_this_template_message)
  This article is in list format, but may read better as prose. You can help by converting_this_article, if
  appropriate. Editing_help is available. (April 2018)
 (Learn_how_and_when_to_remove_this_template_message)
Not to be confused with Active_power_filter.
An example of high-pass active filter of the SallenâKey topology. The
operational amplifier is used as a buffer amplifier.
An active filter is a type of analog_circuit implementing an electronic_filter
using active_components, typically an amplifier. Amplifiers included in a
filter design can be used to improve the cost, performance and predictability
of a filter.[1]
An amplifier prevents the load impedance of the following stage from affecting
the characteristics of the filter. An active filter can have complex poles and
zeros without using a bulky or expensive inductor. The shape of the response,
the Q (quality_factor), and the tuned frequency can often be set with
inexpensive variable resistors.[2] In some active filter circuits, one
parameter can be adjusted without affecting the others.[1]
⁰
***** Contents *****
    * 1_Types
    * 2_Design_of_active_filters
          o 2.1_Comparison_to_passive_filters
    * 3_See_also
    * 4_References
    * 5_External_links
***** Types[edit] *****
Using active elements has some limitations. Basic filter design equations
neglect the finite bandwidth of amplifiers. Available active devices have
limited bandwidth, so they are often impractical at high frequencies.
Amplifiers consume power and inject noise into a system. Certain circuit
topologies may be impractical if no DC path is provided for bias current to the
amplifier elements. Power handling capability is limited by the amplifier
stages.[3]
Active filter circuit configurations (electronic_filter_topology) include:
    * Sallen-Key,_and_VCVS filters (low sensitivity to component tolerance)
    * State_variable_filters and biquadratic or biquad_filters
    * Dual Amplifier Bandpass (DABP)
    * Wien notch
    * Multiple_Feedback_Filters
    * Fliege (lowest component count for 2 opamp but with good controllability
      over frequency and type)
    * Akerberg_Mossberg (one of the topologies that offer complete and
      independent control over gain, frequency, and type)
Active filters can implement the same transfer functions as passive_filters.
Common transfer functions are:
    * High-pass_filter â attenuation of frequencies below their cut-off
      points.
    * Low-pass_filter â attenuation of frequencies above their cut-off
      points.
    * Band-pass_filter â attenuation of frequencies both above and below
      those they allow to pass.
    * Band-stop_filter (Notch filter) â attenuation of certain frequencies
      while allowing all others to pass.[4]
      Combinations are possible, such as notch and high-pass (in a rumble
      filter where most of the offending rumble comes from a particular
      frequency). Another example is an elliptic_filter.
***** Design of active filters[edit] *****
See also: Filter_design
To design filters, the specifications that need to be established include:
    * The range of desired frequencies (the passband) together with the shape
      of the frequency response. This indicates the variety of filter (see
      above) and the center or corner frequencies.
    * Input and output impedance requirements. These limit the circuit
      topologies available; for example, most, but not all active filter
      topologies provide a buffered (low impedance) output. However, remember
      that the internal output impedance of operational_amplifiers, if used,
      may rise markedly at high frequencies and reduce the attenuation from
      that expected. Be aware that some high-pass filter topologies present the
      input with almost a short circuit to high frequencies.
    * Dynamic range of the active elements. The amplifier should not saturate
      (run into the power supply rails) at expected input signals, nor should
      it be operated at such low amplitudes that noise dominates.
    * The degree to which unwanted signals should be rejected.
          o In the case of narrow-band bandpass filters, the Q determines the -
            3 dB bandwidth but also the degree of rejection of frequencies far
            removed from the center frequency; if these two requirements are in
            conflict then a staggered-tuning bandpass filter may be needed.
          o For notch filters, the degree to which unwanted signals at the
            notch frequency must be rejected determines the accuracy of the
            components, but not the Q, which is governed by desired steepness
            of the notch, i.e. the bandwidth around the notch before
            attenuation becomes small.
          o For high-pass and low-pass (as well as band-pass filters far from
            the center frequency), the required rejection may determine the
            slope of attenuation needed, and thus the "order" of the filter. A
            second-order all-pole filter gives an ultimate slope of about 12 dB
            per octave (40 dB/decade), but the slope close to the corner
            frequency is much less, sometimes necessitating a notch be added to
            the filter.
    * The allowable "ripple" (variation from a flat response, in decibels)
      within the passband of high-pass and low-pass filters, along with the
      shape of the frequency response curve near the corner frequency,
      determine the damping ratio or damping factor (= 1/(2Q)). This also
      affects the phase response, and the time response to a square-wave input.
      Several important response shapes (damping ratios) have well-known names:
          o Chebyshev_filter â peaking/ripple in the passband before the
            corner; Q>0.7071 for 2nd-order filters.
          o Butterworth_filter â maximally flat amplitude response; Q=0.7071
            for 2nd-order filters
          o LinkwitzâRiley_filter â desirable properties for audio
            crossover applications, fastest rise time with no overshoot; Q =
            0.5 (critically_damped)
          o Paynter or transitional Thompson-Butterworth or "compromise" filter
            â faster fall-off than Bessel; Q=0.639 for 2nd-order filters
          o Bessel_filter â maximally flat group delay; Q=0.577 for 2nd-order
            filters. It provides good linear phase.
          o Elliptic_filter or Cauer filter â add a notch (or "zero") just
            outside the passband, to give a much greater slope in this region
            than the combination of order and damping ratio without the notch.
            The output is similar to the ideal filter(i.e., good flat response
            of both pass band and the stop band).
**** Comparison to passive filters[edit] ****
An active filter can have gain, increasing the power available in a signal
compared to the input. Passive filters dissipate energy from a signal and
cannot have a net power gain. For some ranges of frequencies, for example at
audio frequencies and below, an active filter can realize a given transfer
function without using inductors, which are relatively large and costly
components compared to resistors and capacitors, and which are more expensive
to make with the required high quality and accurate values. This advantage may
not be as important for active filters entirely integrated on a chip because
the available capacitors have relatively low values and so require high value
resistors which take up area of the integrated circuit. Active filters have
good isolation between stages, and can provide high input impedance and low
output impedance; this makes their characteristics independent of the source
and load impedances. Multiple stages can be cascaded when desired to improve
characteristics. In contrast, design of multiple-stage passive filters must
take into account each stage's frequency-dependent loading of the preceding
stage. It is feasible to make active filters tunable over a wide range,
compared with passive filters. Since inductors are not used, filters can be
made in a very compact size and do not produce or interact with magnetic fields
that may be present.
Compared with active filters, passive filters require no additional power
supplies. The amplifying devices of an active filter must provide predictable
gain and performance over the entire frequency range to be processed; the
Gainâbandwidth_product of the amplifier will constrain the maximum frequency
that can be used. [5][6]
***** See also[edit] *****
    * [icon]Electronics_portal
    * Active_power_filter
    * Frequency_dependent_negative_resistor
***** References[edit] *****
   1. ^ a b Don Lancaster, Active-Filter Cookbook, Howard W. Sams and Co., 1975
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
   3. ISBN 0-672-21168-8 pages 8-10
   4. ^"Op-amp_Band_Pass_Filter". Basic Electronics Tutorials. 2013-08-14.
      Retrieved 2018-12-26.
   5. ^ Muhammad H. Rashid, Microelectronic Circuits: Analysis and Design,
      Cengage Learning, 2010
   6. ISBN 0-495-66772-2, page 804
   7. ^"Band_Stop_Filters_are_called_Reject_Filters". Basic Electronics
      Tutorials. 2015-10-20. Retrieved 2018-12-26.
   8. ^ Don Lancaster, Active-Filter Cookbook, Howard W. Sams, 1975
   9. ISBN 0-672-21168-5 Parameter error in {{ISBN}}: Invalid ISBN., pages 8-9
  10. ^"Basic_Introduction_to_Filters_-_Active,_Passive,_and_Switched-Cap_(Rev.
      A)_Analog_&_Mixed-Signal_SNOA224A_-_TI.com". www.ti.com. Retrieved 2018-
      04-26.
***** External links[edit] *****
 Wikimedia Commons has media related to Active_filters.
    * Split-Supply_Analog_Filter_Expert
    * Introduction_to_active_filters
    * Active_filter_design_-_related_articles
    * Analog_Filter_Wizard: Design tool for active filters

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Active_filter&oldid=892611182"
Categories:
    * Linear_filters
    * Analog_circuits
Hidden categories:
    * Pages_with_ISBN_errors
    * Articles_needing_additional_references_from_November_2011
    * All_articles_needing_additional_references
    * Articles_needing_cleanup_from_April_2018
    * All_pages_needing_cleanup
    * Articles_with_sections_that_need_to_be_turned_into_prose_from_April_2018
    * Articles_with_multiple_maintenance_issues
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
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * Magyar
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 15 April 2019, at 18:20 (UTC).
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
