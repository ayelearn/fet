The following text has been accessed from https://en.wikipedia.org/wiki/Norton%27s_theorem at Thu Aug 8 22:53:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Norton's theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
DC circuit analysis technique
This article is about the theorem in electrical circuits. For Norton's theorem
for queueing networks, see flow-equivalent_server_method.
[text]
Any black_box containing resistances only and voltage and current sources can
be replaced by an equivalent circuit consisting of an equivalent_current_source
in parallel connection with an equivalent resistance.
Edward Lawry Norton
Norton's theorem holds, to illustrate in DC circuit_theory terms (see that
image):
    * Any linear electrical_network with voltage and current sources and only
      resistances can be replaced at terminals AâB by an equivalent current
      source Ino in parallel connection with an equivalent resistance Rno.
    * This equivalent current Ino is the current obtained at terminals A-B of
      the network with terminals A-B short_circuited.
    * This equivalent resistance Rno is the resistance obtained at terminals A-
      B of the network with all its voltage sources short_circuited and all its
      current sources open_circuited.
For alternating_current (AC) systems the theorem can be applied to reactive
impedances as well as resistances.
The Norton equivalent circuit is used to represent any network of linear
sources and impedances at a given frequency.
Norton's theorem and its dual, ThÃ©venin's_theorem, are widely used for circuit
analysis simplification and to study circuit's initial-condition and steady-
state response.
Norton's theorem was independently derived in 1926 by Siemens_&_Halske
researcher Hans_Ferdinand_Mayer (1895â1980) and Bell_Labs engineer Edward
Lawry_Norton (1898â1983).[1][2][3][4][5][dead_link][citation_needed]
To find the equivalent,
   1. Find the Norton current Ino. Calculate the output current, IAB, with a
      short_circuit as the load (meaning 0 resistance between A and B). This is
      Ino.
   2. Find the Norton resistance Rno. When there are no dependent_sources (all
      current and voltage sources are independent), there are two methods of
      determining the Norton impedance Rno.
                * Calculate the output voltage, VAB, when in open_circuit
                  condition (i.e., no load resistor â meaning infinite load
                  resistance). Rno equals this VAB divided by Ino.
            or
                * Replace independent voltage sources with short circuits and
                  independent current sources with open circuits. The total
                  resistance across the output port is the Norton impedance
                  Rno.
This is equivalent to calculating the Thevenin resistance.
      However, when there are dependent sources, the more general method must
      be used. This method is not shown below in the diagrams.
                * Connect a constant current source at the output terminals of
                  the circuit with a value of 1 ampere and calculate the
                  voltage at its terminals. This voltage divided by the 1 A
                  current is the Norton impedance Rno. This method must be used
                  if the circuit contains dependent sources, but it can be used
                  in all cases even when there are no dependent sources.
⁰
***** Contents *****
    * 1_Example_of_a_Norton_equivalent_circuit
    * 2_Conversion_to_a_ThÃ©venin_equivalent
    * 3_Queueing_theory
    * 4_See_also
    * 5_References
    * 6_Bibliography
    * 7_External_links
***** Example of a Norton equivalent circuit[edit] *****
   1. The original circuit
   2. Calculating the equivalent output current
   3. Calculating the equivalent resistance
   4. Design the Norton equivalent circuit
In the example, the total currentItotal is given by:
          I   t o t a l    =    15  V    2   k  &#x03A9; + 1  k  &#x03A9;
      &#x2016; ( 1   k  &#x03A9; + 1   k  &#x03A9; )    = 5.625  m A  .
      {\displaystyle I_{\mathrm {total} }={15\mathrm {V} \over 2\,\mathrm {k}
      \Omega +1\mathrm {k} \Omega \|(1\,\mathrm {k} \Omega +1\,\mathrm {k}
      \Omega )}=5.625\mathrm {mA} .}  [{\displaystyle I_{\mathrm {total} }=
      {15\mathrm {V}  \over 2\,\mathrm {k} \Omega +1\mathrm {k} \Omega \|
      (1\,\mathrm {k} \Omega +1\,\mathrm {k} \Omega )}=5.625\mathrm {mA} .}]
The current through the load is then, using the current_divider_rule:
          I   n o    =    1   k  &#x03A9; + 1   k  &#x03A9;   ( 1   k  &#x03A9;
      + 1   k  &#x03A9; + 1   k  &#x03A9; )    &#x22C5;  I   t o t a l
      {\displaystyle I_{\mathrm {no} }={1\,\mathrm {k} \Omega +1\,\mathrm {k}
      \Omega \over (1\,\mathrm {k} \Omega +1\,\mathrm {k} \Omega +1\,\mathrm
      {k} \Omega )}\cdot I_{\mathrm {total} }}  [{\displaystyle I_{\mathrm {no}
      }={1\,\mathrm {k} \Omega +1\,\mathrm {k} \Omega  \over (1\,\mathrm {k}
      \Omega +1\,\mathrm {k} \Omega +1\,\mathrm {k} \Omega )}\cdot I_{\mathrm
      {total} }}]
         = 2  /  3 &#x22C5; 5.625  m A  = 3.75  m A  .   {\displaystyle =2/
      3\cdot 5.625\mathrm {mA} =3.75\mathrm {mA} .}  [=2/3\cdot 5.625\mathrm
      {mA} =3.75\mathrm {mA} .]
And the equivalent resistance looking back into the circuit is:
          R   n o    = 1   k  &#x03A9; + ( 2   k  &#x03A9; &#x2016; ( 1   k
      &#x03A9; + 1   k  &#x03A9; ) ) = 2   k  &#x03A9; .   {\displaystyle R_
      {\mathrm {no} }=1\,\mathrm {k} \Omega +(2\,\mathrm {k} \Omega \|
      (1\,\mathrm {k} \Omega +1\,\mathrm {k} \Omega ))=2\,\mathrm {k} \Omega .}
      [{\displaystyle R_{\mathrm {no} }=1\,\mathrm {k} \Omega +(2\,\mathrm {k}
      \Omega \|(1\,\mathrm {k} \Omega +1\,\mathrm {k} \Omega ))=2\,\mathrm {k}
      \Omega .}]
So the equivalent circuit is a 3.75 mA current source in parallel with a 2 kÎ©
resistor.
***** Conversion to a ThÃ©venin equivalent[edit] *****
To a ThÃ©venin equivalent
A Norton equivalent circuit is related to the ThÃ©venin_equivalent by the
equations:
          R   t h    =  R   n o       {\displaystyle R_{\rm {th}}=R_{\rm
      {no}}\!}  [{\displaystyle R_{\rm {th}}=R_{\rm {no}}\!}]
          V   t h    =  I   n o     R   n o       {\displaystyle V_{\rm
      {th}}=I_{\rm {no}}R_{\rm {no}}\!}  [{\displaystyle V_{\rm {th}}=I_{\rm
      {no}}R_{\rm {no}}\!}]
            V   t h     R   t h      =  I   n o       {\displaystyle {\frac {V_
      {\rm {th}}}{R_{\rm {th}}}}=I_{\rm {no}}\!}  [{\displaystyle {\frac {V_
      {\rm {th}}}{R_{\rm {th}}}}=I_{\rm {no}}\!}]
***** Queueing theory[edit] *****
The passive circuit equivalent of "Norton's theorem" in queuing_theory is
called the Chandy_Herzog_Woo_theorem.[6][7] In a reversible_queueing_system, it
is often possible to replace an uninteresting subset of queues by a single
(FCFS or PS) queue with an appropriately chosen service rate.[8]
***** See also[edit] *****
    * Ohm's_Law
    * Millman's_theorem
    * Source_transformation
    * Superposition_theorem
    * ThÃ©venin's_theorem
    * Maximum_power_transfer_theorem
    * Extra_element_theorem
***** References[edit] *****
   1. ^ Mayer
   2. ^ Norton
   3. ^ Johnson (2003b)
   4. ^ Brittain
   5. ^ Dorf
   6. ^ Johnson (2003a)
   7. ^ Gunther
   8. ^ Chandy et al.
***** Bibliography[edit] *****
    * Brittain, J.E. (March 1990). "Thevenin's_theorem". IEEE Spectrum. 27 (3):
      42. doi:10.1109/6.48845. Retrieved 1 February 2013.
Chandy, K. M.; Herzog, U.; Woo, L. (Jan 1975). "Parametric_Analysis_of_Queuing
Networks". IBM Journal of Research and Development. 19 (1): 36â42. doi:
10.1147/rd.191.0036.
Dorf, Richard C.; Svoboda, James A. (2010). "Chapter_5_â_Circuit_Theorems".
Introduction to Electric Circuits (8th ed.). Hoboken, NJ: John Wiley & Sons.
pp. 162â207. ISBN 978-0-470-52157-1. Archived from the_original on 2012-04-
30. Retrieved 2018-12-08.
Gunther, N.J. (2004). Analyzing_computer_systems_performance :_with_PERL::PDQ
(Online-Ausg. ed.). Berlin: Springer. p. 281. ISBN 978-3-540-20865-5.
Johnson, D.H. (2003). "Origins_of_the_equivalent_circuit_concept:_the_voltage-
source_equivalent" (PDF). Proceedings of the IEEE. 91 (4): 636â640. doi:
10.1109/JPROC.2003.811716. hdl:1911/19968.
Johnson, D.H. (2003). "Origins_of_the_equivalent_circuit_concept:_the_current-
source_equivalent" (PDF). Proceedings of the IEEE. 91 (5): 817â821. doi:
10.1109/JPROC.2003.811795.
Mayer, H. F. (1926). "Ueber das Ersatzschema der VerstÃ¤rkerrÃ¶hre (On
equivalent circuits for electronic amplifiers]". Telegraphen- und Fernsprech-
Technik. 15: 335â337.
Norton, E. L. (1926). "Technical Report TM26â0â1860 â Design of finite
networks for uniform frequency characteristic". Bell Laboratories.
***** External links[edit] *****
    * Norton's_theorem_at_allaboutcircuits.com

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Norton%27s_theorem&oldid=891002514"
Categories:
    * Circuit_theorems
    * Linear_electronic_circuits
Hidden categories:
    * Articles_with_short_description
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_September_2018
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2018
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
    * á áá­á
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Shqip
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * ä¸­æ
Edit_links
    * This page was last edited on 5 April 2019, at 00:08 (UTC).
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
