The following text has been accessed from https://en.wikipedia.org/wiki/Equivalent_circuit at Thu Aug 8 22:47:34 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Equivalent circuit ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In electrical engineering and science, an equivalent circuit refers to a
theoretical circuit that retains all of the electrical characteristics of a
given circuit. Often, an equivalent circuit is sought that simplifies
calculation, and more broadly, that is a simplest form of a more complex
circuit in order to aid analysis.[1] In its most common form, an equivalent
circuit is made up of linear, passive elements. However, more complex
equivalent circuits are used that approximate the nonlinear behavior of the
original circuit as well. These more complex circuits often are called
macromodels of the original circuit. An example of a macromodel is the Boyle
circuit for the 741 operational amplifier.[2]
⁰
***** Contents *****
    * 1_Examples
          o 1.1_ThÃ©venin_and_Norton_equivalents
          o 1.2_DC_and_AC_equivalent_circuits
          o 1.3_Two-port_networks
          o 1.4_Delta_and_Wye_circuits
    * 2_In_biology
    * 3_See_also
    * 4_References
***** Examples[edit] *****
**** ThÃ©venin and Norton equivalents[edit] ****
One of linear circuit theory's most surprising properties relates to the
ability to treat any two-terminal circuit no matter how complex as behaving as
only a source and an impedance, which have either of two simple equivalent
circuit forms:[1][3]
    * ThÃ©venin_equivalent - Any linear two-terminal circuit can be replaced by
      a single voltage_source and a series impedance.
    * Norton_equivalent - Any linear two-terminal circuit can be replaced by a
      current_source and a parallel impedance.
However, the single impedance can be of arbitrary complexity (as a function of
frequency) and may be irreducible to a simpler form.
**** DC and AC equivalent circuits[edit] ****
In linear_circuits, due to the superposition_principle, the output of a circuit
is equal to the sum of the output due to its DC sources alone, and the output
from its AC sources alone. Therefore, the DC and AC response of a circuit is
often analyzed independently, using separate DC and AC equivalent circuits
which have the same response as the original circuit to DC and AC currents
respectively. The composite response is calculated by adding the DC and AC
responses:
    * A DC equivalent of a circuit can be constructed by replacing all
      capacitances with open circuits, inductances with short circuits, and
      reducing AC sources to zero (replacing AC voltage sources by short
      circuits and AC current sources by open circuits.)
    * An AC equivalent circuit can be constructed by reducing all DC sources to
      zero (replacing DC voltage sources with short circuits and DC current
      sources with open circuits)
This technique is often extended to small-signal nonlinear circuits like tube
and transistor circuits, by linearizing the circuit about the DC bias point Q-
point, using an AC equivalent circuit made by calculating the equivalent small
signal AC resistance of the nonlinear components at the bias point.
**** Two-port networks[edit] ****
Main article: Two-port_network
Linear four-terminal circuits in which a signal is applied to one pair of
terminals and an output is taken from another, are often modeled as two-port
networks. These can be represented by simple equivalent circuits of impedances
and dependent sources. To be analyzed as a two port network the currents
applied to the circuit must satisfy the port_condition: the current entering
one terminal of a port must be equal to the current leaving the other terminal
of the port.[4] By linearizing a nonlinear circuit about its operating_point,
such a two-port representation can be made for transistors: see hybrid_pi and
h-parameter circuits.
**** Delta and Wye circuits[edit] ****
In three_phase_power circuits, three phase sources and loads can be connected
in two different ways, called a "delta" connection and a "wye" connection. In
analyzing circuits, sometimes it simplifies the analysis to convert between
equivalent wye and delta circuits. This can be done with the wye-delta
transform.
***** In biology[edit] *****
Equivalent circuits can be used to electrically describe and model either a)
continuous materials or biological systems in which current does not actually
flow in defined circuits, or, b) distributed reactances, such as found in
electrical lines or windings, that do not represent actual discrete components
[citation_needed]. For example, a cell_membrane can be modelled as a
capacitance (i.e. the lipid_bilayer) in parallel with resistance-DC voltage
source combinations (i.e. ion_channels powered by an ion gradient across the
membrane).
***** See also[edit] *****
    * Equivalent_impedance_transforms
    * Miller_theorem
    * Lumped_element_model
***** References[edit] *****
   1. ^ a bJohnson, D.H. (2003a). "Origins_of_the_equivalent_circuit_concept:
      the_voltage-source_equivalent" (PDF). Proceedings of the IEEE. 91 (4):
      636â640. doi:10.1109/JPROC.2003.811716.
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
   3. ^Richard C. Dorf (1997). The_Electrical_Engineering_Handbook. New York:
      CRC Press. Fig. 27.4, p. 711. ISBN 978-0-8493-8574-2.
   4. ^Johnson, D.H. (2003b). "Origins_of_the_equivalent_circuit_concept:_the
      current-source_equivalent" (PDF). Proceedings of the IEEE. 91 (5):
      817â821. doi:10.1109/JPROC.2003.811795.
   5. ^ P.R. Gray; P.J. Hurst; S.H. Lewis; R.G. Meyer (2001). Analysis_and
      Design_of_Analog_Integrated_Circuits (Fourth ed.). New York: Wiley.
      pp. Â§3.2, p. 172. ISBN 978-0-471-32168-2.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Equivalent_circuit&oldid=897121733"
Categories:
    * Circuit_theorems
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_May_2019
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
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 14 May 2019, at 22:33 (UTC).
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
