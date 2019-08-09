The following text has been accessed from https://en.wikipedia.org/wiki/Precision_rectifier at Fri Aug 9 01:27:34 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Precision rectifier ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The precision rectifier, also known as a super diode, is a configuration
obtained with an operational_amplifier in order to have a circuit behave like
an ideal diode and rectifier.[1] It is very useful for high-precision signal
processing. With the help of precision rectifier the high-precision signal
processing can be done very easily
The op-amp-based precision rectifier should not be confused with the power
MOSFET-based active_rectification ideal diode.

***** Basic circuit[edit] *****
A simple precision rectifier circuit
The basic circuit implementing such a feature is shown on the right, where
R  L     {\displaystyle R_{\text{L}}}  [{\displaystyle R_{\text{L}}}] can be
any load. When the input voltage is negative, there is a negative voltage on
the diode, so it works like an open circuit, no current flows through the load,
and the output voltage is zero.
When the input is positive, it is amplified by the operational amplifier, which
switches the diode on. Current flows through the load and, because of the
feedback, the output voltage is equal to the input voltage.
The actual threshold of the super diode is very close to zero, but is not zero.
It equals the actual threshold of the diode, divided by the gain of the
operational amplifier.
This basic configuration has a problem, so it is not commonly used. When the
input becomes (even slightly) negative, the operational amplifier runs open-
loop, as there is no feedback signal through the diode. For a typical
operational amplifier with high open-loop gain, the output saturates. If the
input then becomes positive again, the op-amp has to get out of the saturated
state before positive amplification can take place again. This change generates
some ringing and takes some time, greatly reducing the frequency_response of
the circuit.
***** Improved circuit[edit] *****
An improved precision rectifier circuit.
An alternative version is given on the right.
In this case, when the input is greater than zero, D1 is off, and D2 is on, so
the output is zero because the other end of      R  2     {\displaystyle R_{2}}
[R_{2}] is connected to the virtual ground and there is no current through
R  2     {\displaystyle R_{2}}  [R_{2}]. When the input is less than zero, D1
is on, and D2 is off, so the output is like the input with an amplification of
&#x2212;  R  2    /   R  1     {\displaystyle -R_{2}/R_{1}}  [-R_{2}/R_{1}].
Its inputâoutput relationship is the following:
[Super_diode_improved]
This circuit has the benefit that the op-amp never goes into saturation, but
its output must change by two diode voltage drops (about 1.2 V) each time the
input signal crosses zero. Hence, the slew_rate of the operational amplifier
and its frequency response (gainâbandwidth_product) will limit high-frequency
performance, especially for low signal levels, although an error of less than
1% at 100 kHz is possible.
Similar circuitry can be used to create a precision full-wave_rectifier
circuit.
***** Peak detector[edit] *****
With a little modification, the basic precision rectifier can be used for
detecting signal level peaks. In the following circuit, a capacitor retains the
peak voltage level of the signal, and a switch is used for resetting the
detected level. When the input Vin exceeds Vc(voltage across capacitor), the
diode is forward biased and the circuit becomes voltage follower. Consequently,
the output voltage Vo follows Vin as long as Vin exceeds Vc. When Vin drops
below Vc, the diode becomes reverse biased and the capacitor holds the charge
till input voltage again attains a value greater than Vc.
[Peak_detector]
***** References[edit] *****
   1. ^ Paul Horowitz and Winfield Hill, The_Art_of_Electronics. 2nd ed.
      Cambridge University Press, Cambridge, 1989
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
   3. ISBN 0-521-37095-7.
***** External links[edit] *****
    * Precision_half-wave_rectifier
    * Precision_full-wave_rectifier
    * Single_op-amp_full-wave_rectifier_circuits
    * Rod_Elliott's_improved_version
    * Patent_from_1982_(expired)_detailing_a_simple_very_accurate_design

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Precision_rectifier&oldid=897782896"
Categories:
    * Analog_circuits
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
    * Italiano
    * LietuviÅ³
    * Suomi
Edit_links
    * This page was last edited on 19 May 2019, at 10:32 (UTC).
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
