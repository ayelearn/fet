The following text has been accessed from https://en.wikipedia.org/wiki/Biasing at Fri Aug 9 03:37:01 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Biasing ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Predetermined voltages or currents establishing proper operating conditions in
electronic components
This article is about biasing in electronics. For other uses, see Biasing_
(disambiguation).
A graphical representation of the current and voltage properties of a
transistor; the bias is selected so that the operating point permits maximum
signal amplitude without distortion.
Biasing in electronics means establishing predetermined voltages or currents at
various points of an electronic_circuit for the purpose of establishing proper
operating conditions in electronic_components. Many electronic devices such as
diodes, transistors and vacuum_tubes, whose function is processing time-varying
(AC) signals also require a steady (DC) current or voltage to operate
correctlyâa bias. The AC signal applied to them is superposed on this DC bias
current or voltage. The operating_point of a device, also known as bias point,
quiescent point, or Q-point, is the DC voltage or current at a specified
terminal of an active device (a transistor or vacuum tube) with no input signal
applied. A bias circuit is a portion of the device's circuit which supplies
this steady current or voltage.
⁰
***** Contents *****
    * 1_Overview
    * 2_Importance_in_linear_circuits
    * 3_Bipolar_junction_transistors
    * 4_Vacuum_tubes_(thermionic_valves)
    * 5_Microphones
    * 6_See_also
    * 7_References
    * 8_Further_reading
***** Overview[edit] *****
In electronics, bias usually refers to a fixed DC voltage or current applied to
a terminal of an electronic_component such as a diode, transistor or vacuum
tube in a circuit in which AC signals are also present, in order to establish
proper operating conditions for the component. For example, a bias voltage is
applied to a transistor in an electronic_amplifier to allow the transistor to
operate in a particular region of its transconductance curve. For vacuum tubes,
a grid_bias voltage is often applied to the grid electrodes for the same
reason.
In electronic_engineering, the term bias has the following meanings:[citation
needed]
   1. A systematic deviation of a value from a reference value
   2. The amount by which the average of a set of values departs from a
      reference value
   3. Electrical, mechanical, magnetic, or other force applied to a device to
      establish a reference level to operate the device
   4. In telegraph signaling systems, the development of a positive or negative
      DC_voltage at a point on a telephone_line that should remain at a
      specified reference level, e.g. zero.[citation_needed]
In magnetic_tape_recording, the term bias is also used for a high-frequency
signal added to the audio_signal and applied to the recording_head, to improve
the quality of the recording on the tape. This is called tape_bias.
***** Importance in linear circuits[edit] *****
Linear circuits involving transistors typically require specific DC voltages
and currents for correct operation, which can be achieved using a biasing
circuit. As an example of the need for careful biasing, consider a transistor
amplifier. In linear amplifiers, a small input signal gives larger output
signal without any change in shape (low distortion): the input signal causes
the output signal to vary up and down about the Q-point in a manner strictly
proportional to the input. However, because the relationship between input and
output for a transistor is not linear across its full operating range, the
transistor amplifier only approximates linear operation. For low distortion,
the transistor must be biased so the output signal swing does not drive the
transistor into a region of extremely nonlinear operation. For a bipolar
junction transistor amplifier, this requirement means that the transistor must
stay in the active_mode, and avoid cut-off or saturation. The same requirement
applies to a MOSFET amplifier, although the terminology differs a little: the
MOSFET must stay in the active_mode, and avoid cutoff or ohmic operation.
***** Bipolar junction transistors[edit] *****
Main article: Bipolar_transistor_biasing
For bipolar_junction_transistors the bias point is chosen to keep the
transistor operating in the active mode, using a variety of circuit techniques,
establishing the Q-point DC voltage and current. A small signal is then applied
on top of the bias. The Q-point is typically near the middle of the DC load
line, so as to obtain the maximum available peak-to-peak signal amplitude
without distortion due to clipping as the transistor reaches saturation or cut-
off. The process of obtaining an appropriate DC collector current at a certain
DC collector voltage by setting up the operating point is called biasing.
***** Vacuum tubes (thermionic valves)[edit] *****
Grid_bias is the DC voltage provided at the control grid of a vacuum tube
relative to the cathode for the purpose of establishing the zero input signal
or steady state operating condition of the tube.[1][2]
    * In a typical Class_A voltage_amplifier, and class A and AB1 power stages
      of audio_power_amplifiers, the DC bias voltage is negative relative to
      the cathode potential. The instantaneous grid voltage (sum of DC bias and
      AC input signal) does not reach the point where grid current begins.
    * Class_B_amplifiers using general purpose tubes are biased negatively to
      the projected plate current cutoff point. The bias voltage source must
      have low resistance and be able to supply the grid current.[3] When tubes
      designed for class B are employed, the bias can be as little as zero.
    * Class_C_amplifiers are biased negatively at a point well beyond plate
      current cutoff. Grid current occurs during significantly less than 180
      degrees of the input frequency cycle.
There are many methods of achieving grid bias. Combinations of bias methods may
be used on the same tube.
    * Fixed bias: The DC grid potential is determined by connection to an
      appropriate impedance that will pass DC from an appropriate voltage
      source.[2][4]
    * Cathode_bias (self-bias, automatic bias) - The voltage drop across a
      resistor in series with the cathode is utilized. The grid circuit DC
      return is connected to the other end of the resistor, causing the DC grid
      voltage to be negative relative to the cathode.[4]
    * Grid leak bias: When the grid is driven positive during part of the input
      frequency cycle, such as in class C operation, rectification in the grid
      circuit in conjunction with capacitive coupling of the input signal to
      the grid produces negative DC voltage at the grid. A resistor (the grid
      leak) permits discharge of the coupling capacitor and passes the DC grid
      current. The resultant bias voltage is equal to the product of the DC
      grid current and the grid leak resistance.[5][4][6]
    * Bleeder bias: The voltage drop across a portion of a resistance across
      the plate voltage supply determines the grid bias. The cathode is
      connected to a tap on the resistance. The grid is connected to an
      appropriate impedance that provides a DC path either to the negative side
      of the plate voltage supply or to another tap on the same resistance.[1]
      [7][8]
    * Initial velocity bias (contact bias): Due to electrons entering the grid,
      a DC voltage is developed across a grid to cathode resistor, usually in
      the range of 1 to 10 megohms.[9][10][11]
***** Microphones[edit] *****
Electret_microphone elements typically include a junction_field-effect
transistor as an impedance converter to drive other electronics within a few
meters of the microphone. The operating current of this JFET is typically 0.1
to 0.5 mA and is often referred to as bias,[12] which is different from the
phantom_power interface which supplies 48 volts to operate the backplate of a
traditional condenser microphone. Electret microphone bias is sometimes
supplied on a separate conductor.[13]
***** See also[edit] *****
    * Idling_current
    * Small_signal_model
***** References[edit] *****
   1. ^ a bVeley, Victor F. C. (1994). The Benchtop Electronics Reference
      Manual (3rd ed.). New York: Tab Books. pp. 362â365.
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
   3. ^ a b Landee, Davis, Albrecht, Electronic_Designers'_Handbook, New York:
      McGraw-Hill, 1957, p. 2-27.
   4. ^ Landee et al., 1957, p._4-19.
   5. ^ a b cOrr, William I., ed. (1962). The Radio Handbook (16th ed.). New
      Augusta Indiana: Editors and Engineers, LTD. pp. 266â267.
   6. ^Headquarters, Department of the Army (1952). C-W_and_A-M_Radio
      Transmitters_and_Receivers. Washington, D.C.: United States Government
      Publishing Office. p. 97. TM 11-665.
   7. ^Everitt, William Littell (1937). Communication Engineering (2nd ed.).
      New York: McGraw-Hill. pp. 538â539.
   8. ^RCA Manufacturing Co. (1940). Receiving Tube Manual RC-14. Harrison, NJ:
      RCA. p. 38.
   9. ^Ghirardi, Alfred A. (1932). Radio Physics Course (2nd ed.). New York:
      Rinehart Books. pp. 505, 770â771.
  10. ^Giacoletto, Lawrence Joseph (1977). Electronics Designers' Handbook. New
      York: McGraw-Hill. p. 9-27.
  11. ^Tomer, Robert B. (1960). Getting_the_Most_Out_of_Vacuum_Tubes.
      Indianapolis: Howard W. Sams & Co./The Bobbs-Merrill Company. p. 28.
      Archived from the_original on 2009.
  12. ^ Landee et al., 1957, p._2-28.
  13. ^"Phantom_Power_and_Bias_Voltage:_Is_There_A_Difference?". 2007-02-05.
      Archived from the_original on 2009-09-08.
  14. ^ IEC Standard_61938(subscription required)
***** Further reading[edit] *****
    * Boylestad, Robert L.; Nashelsky, Louis (2005). Electronic Devices and
      Circuit Theory. Prentice-Hall Career & Technology.
Patil, P. K.; Chitnis, M. M. (2005). Basic Electricity and Semiconductor
Devices. Phadke Prakashan.
Sedra, Adel; Smith, Kenneth (2004). Microelectronic Circuits. Oxford University
Press. ISBN 0-19-514251-9.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Biasing&oldid=909114683"
Categories:
    * Electronic_engineering
    * Vacuum_tubes
Hidden categories:
    * Pages_containing_links_to_subscription-only_content
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_July_2018
    * Articles_with_unsourced_statements_from_October_2018
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
    * CatalÃ 
    * Dansk
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * ×¢××¨××ª
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Svenska
    * à¹à¸à¸¢
    * ä¸­æ
Edit_links
    * This page was last edited on 3 August 2019, at 05:41 (UTC).
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
