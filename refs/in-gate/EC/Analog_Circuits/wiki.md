The following text has been accessed from https://en.wikipedia.org/wiki/Analogue_electronics at Fri Aug 9 03:36:18 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Analogue electronics ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Analogue electronics (American_English: analog electronics) are electronic
systems with a continuously variable signal, in contrast to digital_electronics
where signals usually take only_two_levels. The term "analogue" describes the
proportional relationship between a signal and a voltage or current that
represents the signal. The word analogue is derived from the Greek word
Î±Î½Î¬Î»Î¿Î³Î¿Ï (analogos) meaning "proportional".[1]
⁰
***** Contents *****
    * 1_Analogue_signals
    * 2_Inherent_noise
    * 3_Analogue_vs_digital_electronics
          o 3.1_Noise
          o 3.2_Precision
          o 3.3_Design_difficulty
    * 4_Circuit_classification
    * 5_See_also
    * 6_References
***** Analogue signals[edit] *****
Main article: Analogue_signal
An analogue signal uses some attribute of the medium to convey the signal's
information. For example, an aneroid_barometer uses the angular_position of a
needle as the signal to convey the information of changes in atmospheric
pressure.[2] Electrical signals may represent information by changing their
voltage, current, frequency, or total charge. Information is converted from
some other physical form (such as sound, light, temperature, pressure,
position) to an electrical signal by a transducer which converts one type of
energy into another (e.g. a microphone).[3]
The signals take any value from a given range, and each unique signal value
represents different information. Any change in the signal is meaningful, and
each level of the signal represents a different level of the phenomenon that it
represents. For example, suppose the signal is being used to represent
temperature, with one volt representing one degree Celsius. In such a system,
10 volts would represent 10 degrees, and 10.1 volts would represent 10.1
degrees.
Another method of conveying an analogue signal is to use modulation. In this,
some base carrier signal has one of its properties altered: amplitude
modulation (AM) involves altering the amplitude of a sinusoidal voltage
waveform by the source information, frequency_modulation (FM) changes the
frequency. Other techniques, such as phase_modulation or changing the phase of
the carrier signal, are also used.[4]
In an analogue sound recording, the variation in pressure of a sound striking a
microphone creates a corresponding variation in the current passing through it
or voltage across it. An increase in the volume of the sound causes the
fluctuation of the current or voltage to increase proportionally while keeping
the same waveform or shape.
Mechanical, pneumatic, hydraulic, and other systems may also use analogue
signals.
***** Inherent noise[edit] *****
Analogue systems invariably include noise that is random disturbances or
variations, some caused by the random_thermal_vibrations of atomic particles.
Since all variations of an analogue signal are significant, any disturbance is
equivalent to a change in the original signal and so appears as noise.[5] As
the signal is copied and re-copied, or transmitted over long distances, these
random variations become more significant and lead to signal degradation. Other
sources of noise may include crosstalk from other signals or poorly designed
components. These disturbances are reduced by shielding and by using low-noise
amplifiers (LNA).[6]
***** Analogue vs digital electronics[edit] *****
Since the information is encoded differently in analogue and digital
electronics, the way they process a signal is consequently different. All
operations that can be performed on an analogue signal such as amplification,
filtering, limiting, and others, can also be duplicated in the digital domain.
Every digital circuit is also an analogue circuit, in that the behaviour of any
digital circuit can be explained using the rules of analogue circuits.
The use of microelectronics has made digital devices cheap and widely
available.
**** Noise[edit] ****
The effect of noise on an analogue circuit is a function of the level of noise.
The greater the noise level, the more the analogue signal is disturbed, slowly
becoming less usable. Because of this, analogue signals are said to "fail
gracefully". Analogue signals can still contain intelligible information with
very high levels of noise. Digital circuits, on the other hand, are not
affected at all by the presence of noise until a certain threshold is reached,
at which point they fail catastrophically. For digital telecommunications, it
is possible to increase the noise threshold with the use of error_detection_and
correction coding schemes and algorithms. Nevertheless, there is still a point
at which catastrophic failure of the link occurs.[7][8]
In digital electronics, because the information is quantized, as long as the
signal stays inside a range of values, it represents the same information. In
digital circuits the signal is regenerated at each logic_gate, lessening or
removing noise.[9][failed_verification] In analogue circuits, signal loss can
be regenerated with amplifiers. However, noise is cumulative throughout the
system and the amplifier itself will add to the noise according to its noise
figure.[10][11]
**** Precision[edit] ****
A number of factors affect how precise a signal is, mainly the noise present in
the original signal and the noise added by processing (see signal-to-noise
ratio). Fundamental physical limits such as the shot_noise in components limits
the resolution of analogue signals. In digital electronics additional precision
is obtained by using additional digits to represent the signal. The practical
limit in the number of digits is determined by the performance of the analogue-
to-digital_converter (ADC), since digital operations can usually be performed
without loss of precision. The ADC takes an analogue signal and changes it into
a series of binary_numbers. The ADC may be used in simple digital display
devices, e. g., thermometers or light meters but it may also be used in digital
sound recording and in data acquisition. However, a digital-to-analogue
converter (DAC) is used to change a digital signal to an analogue signal. A DAC
takes a series of binary numbers and converts it to an analogue signal. It is
common to find a DAC in the gain-control system of an op-amp which in turn may
be used to control digital amplifiers and filters.[12]
**** Design difficulty[edit] ****
Analogue circuits are typically harder to design, requiring more skill than
comparable digital systems.[citation_needed] This is one of the main reasons
that digital systems have become more common than analogue devices. An analogue
circuit is usually designed by hand, and the process is much less automated
than for digital systems. Since the early 2000s, there were some platforms that
were developed which enabled Analog design to be defined using software - which
allows faster prototyping. However, if a digital electronic device is to
interact with the real world, it will always need an analogue interface.[13]
For example, every digital_radio receiver has an analogue preamplifier as the
first stage in the receive chain.
***** Circuit classification[edit] *****
Analogue circuits can be entirely passive, consisting of resistors, capacitors
and inductors. Active circuits also contain active elements like transistors.
Many passive analogue circuits are built from lumped elements. That is,
discrete components. However, an alternative is distributed_element_circuits
built from pieces of transmission_line.
***** See also[edit] *****
    * Analogue_computer
    * Analogue_signal
    * Digital â for a comparison with analogue
    * Digital_electronics
    * Analogue_recording_vs._digital_recording
    * Analogue_chip
    * Analogue_verification
    * Electronic_circuit
***** References[edit] *****
   1. ^Concise Oxford dictionary (10 ed.). Oxford University Press Inc. 1999.
      ISBN 0-19-860287-1.
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
   3. ^Plympton, George Washington (1884). The_aneroid_barometer:_its
      construction_and_use. D. Van Nostran Co.
   4. ^Singmin, Andrew (2001). Beginning_Digital_Electronics_Through_Projects.
      Newnes. p. 9. ISBN 0-7506-7269-2. Signals come from transducers...
   5. ^Miller, Mark R. (2002). Electronics_the_Easy_Way. Barron's Educational
      Series. pp. 232â239. ISBN 0-7641-1981-8. Until the radio came along...
   6. ^Hsu, Hwei Piao (2003). Schaum's_Outline_of_Theory_and_Problems_of
      Analogue_and_Digital_Communications. McGraw-Hill Professional. p. 202.
      ISBN 0-07-140228-4. The presence of noise degrades the performance of
      communication systems.
   7. ^Carr, Joseph J. (2000). Secrets_of_RF_circuit_design. McGraw-Hill
      Professional. p. 423. ISBN 0-07-137067-6. It is common in microwave
      systems...
   8. ^ Richard Langton Gregory, Even Odder Perceptions, p. 161, Psychology
      Press, 1994
   9. ISBN 0415061067.
  10. ^ Robin Blair, Digital Techniques in Broadcasting Transmission, p. 34,
      Focal Press, 2002,
  11. ISBN 0240805089.
  12. ^Chen, Wai-Kai (2005). The_electrical_engineering_handbook. Academic
      Press. p. 101. ISBN 0-12-170960-4. Noise from an analog (or small-signal)
      perspective...
  13. ^ Jon B. Hagen, Radio-Frequency Electronics: Circuits and Applications,
      p. 203, Cambridge University Press, 1996
  14. ISBN 0521553563.
  15. ^ Jonathan Davidson, James Peters, Brian Gracely, Voice Over IP
      Fundamentals, Cisco Press, 2000
  16. ISBN 1578701686.
  17. ^Scherz, Paul (2006). Practical_electronics_for_inventors. McGraw-Hill
      Professional. p. 730. ISBN 0-07-145281-8. In order for analog devices...
      to communicate with digital circuits...
  18. ^Williams, Jim (1991). Analog_circuit_design. Newnes. p. 238. ISBN 0-
      7506-9640-0. Even within companies producing both analog and digital
      products...

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Analogue_electronics&oldid=871180124"
Categories:
    * Analog_circuits
    * Electronic_engineering
Hidden categories:
    * Use_British_English_Oxford_spelling_from_August_2016
    * Articles_containing_explicitly_cited_English-language_text
    * Articles_containing_Greek-language_text
    * All_articles_with_failed_verification
    * Articles_with_failed_verification_from_April_2018
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_March_2010
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
    * Wikiversity
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * æ¥æ¬èª
    * Polski
    * Shqip
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 29 November 2018, at 13:36 (UTC).
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
