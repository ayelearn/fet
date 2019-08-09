The following text has been accessed from https://en.wikipedia.org/wiki/Zener_diode at Fri Aug 9 01:26:55 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Zener diode ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
              Zener diode
[Zener_Diode.JPG]
Zener diode
Type              Active
Working principle Zener_effect
Invented          Clarence_Melvin_Zener
Pin configuration anode and cathode
Electronic_symbol
[Zener_diode_symbol-2.svg]
A Zener diode is a type of diode that allows current to flow not only from its
anode to its cathode, but also in the reverse direction, when the Zener voltage
is reached.
Zener diodes have a highly doped pân_junction. Normal diodes break_down with
a reverse voltage, but the voltage and sharpness of the knee are not as well
defined as for a Zener diode. Normal diodes are not designed to operate in the
breakdown region, whereas Zener diodes operate reliably in this region.
Zener reverse breakdown is due to electron quantum_tunnelling caused by a high-
strength electric field. However, many diodes described as "Zener" diodes rely
instead on avalanche_breakdown. Both breakdown types are used in Zener diodes
with the Zener effect predominating at lower voltages and avalanche breakdown
at higher voltages.
Zener diodes are widely used in electronic equipment of all kinds and are one
of the basic building blocks of electronic circuits. They are used to generate
low-power stabilized supply rails from a higher voltage and to provide
reference voltages for circuits, especially stabilized power supplies. They are
also used to protect circuits from overvoltage, especially electrostatic
discharge (ESD).
⁰
***** Contents *****
    * 1_History
    * 2_Operation
    * 3_Construction
          o 3.1_Surface_Zeners
          o 3.2_Subsurface_Zeners
    * 4_Uses
          o 4.1_Waveform_clipper
          o 4.2_Voltage_shifter
          o 4.3_Voltage_regulator
    * 5_See_also
    * 6_References
    * 7_Further_reading
    * 8_External_links
***** History[edit] *****
The device was named after Clarence_Zener, who discovered the Zener_effect.
***** Operation[edit] *****
Current-voltage characteristic of a Zener diode with a breakdown voltage of 17
V. Notice the change of voltage scale between the forward biased (positive)
direction and the reverse biased (negative) direction.
Temperature coefficient of Zener voltage against nominal Zener voltage.
A conventional solid-state diode allows significant current if it is reverse-
biased above its reverse breakdown_voltage. When the reverse bias breakdown
voltage is exceeded, a conventional diode is subject to high current due to
avalanche_breakdown. Unless this current is limited by circuitry, the diode may
be permanently damaged due to overheating. A Zener diode exhibits almost the
same properties, except the device is specially designed so as to have a
reduced breakdown voltage, the so-called Zener voltage. By contrast with the
conventional device, a reverse-biased Zener diode exhibits a controlled
breakdown and allows the current to keep the voltage across the Zener diode
close to the Zener breakdown voltage. For example, a diode with a Zener
breakdown voltage of 3.2 V exhibits a voltage drop of very nearly 3.2 V across
a wide range of reverse currents. The Zener diode is therefore ideal for
applications such as the generation of a reference_voltage (e.g. for an
amplifier stage), or as a voltage stabilizer for low-current applications.[1]
Another mechanism that produces a similar effect is the avalanche effect as in
the avalanche_diode.[1] The two types of diode are in fact constructed the same
way and both effects are present in diodes of this type. In silicon diodes up
to about 5.6 volts, the Zener_effect is the predominant effect and shows a
marked negative temperature_coefficient. Above 5.6 volts, the avalanche_effect
becomes predominant and exhibits a positive temperature coefficient.[2]
In a 5.6 V diode, the two effects occur together, and their temperature
coefficients nearly cancel each other out, thus the 5.6 V diode is useful in
temperature-critical applications. An alternative, which is used for voltage
references that need to be highly stable over long periods of time, is to use a
Zener diode with a temperature coefficient (TC) of +2 mV/Â°C (breakdown voltage
6.2â6.3 V) connected in series with a forward-biased silicon diode (or a
transistor B-E junction) manufactured on the same chip.[3] The forward-biased
diode has a temperature coefficient of â2 mV/Â°C, causing the TCs to cancel
out.
Modern manufacturing techniques have produced devices with voltages lower than
5.6 V with negligible temperature coefficients,[citation_needed] but as higher-
voltage devices are encountered, the temperature coefficient rises
dramatically. A 75 V diode has 10 times the coefficient of a 12 V diode.
[citation_needed]
Zener and avalanche diodes, regardless of breakdown voltage, are usually
marketed under the umbrella term of "Zener diode".
Under 5.6 V, where the Zener effect dominates, the IV curve near breakdown is
much more rounded, which calls for more care in targeting its biasing
conditions. The IV curve for Zeners above 5.6 V (being dominated by Avalanche),
is much sharper at breakdown.
***** Construction[edit] *****
The Zener diode's operation depends on the heavy doping of its p-n_junction.
The depletion region formed in the diode is very thin (<1 Âµm) and the electric
field is consequently very high (about 500 kV/m) even for a small reverse bias
voltage of about 5 V, allowing electrons to tunnel from the valence band of the
p-type material to the conduction band of the n-type material.
At the atomic scale, this tunneling corresponds to the transport of valence
band electrons into the empty conduction band states; as a result of the
reduced barrier between these bands and high electric fields that are induced
due to the high levels of doping on both sides.[2] The breakdown voltage can be
controlled quite accurately in the doping process. While tolerances within
0.07% are available, the most widely used tolerances are 5% and 10%. Breakdown
voltage for commonly available Zener diodes can vary widely from 1.2 V to 200
V.
For diodes that are lightly doped the breakdown is dominated by the avalanche
effect rather than the Zener effect. Consequently, the breakdown voltage is
higher (over 5.6 V) for these devices.[4]
**** Surface Zeners[edit] ****
The emitter-base junction of a bipolar NPN_transistor behaves as a Zener diode,
with breakdown voltage at about 6.8 V for common bipolar processes and about 10
V for lightly doped base regions in BiCMOS processes. Older processes with poor
control of doping characteristics had the variation of Zener voltage up to Â±1
V, newer processes using ion implantation can achieve no more than Â±0.25 V.
The NPN transistor structure can be employed as a surface Zener diode, with
collector and emitter connected together as its cathode and base region as
anode. In this approach the base doping profile usually narrows towards the
surface, creating a region with intensified electric field where the avalanche
breakdown occurs. The hot_carriers produced by acceleration in the intense
field sometime shoot into the oxide layer above the junction and become trapped
there. The accumulation of trapped charges can then cause 'Zener walkout', a
corresponding change of the Zener voltage of the junction. The same effect can
be achieved by radiation_damage.
The emitter-base Zener diodes can handle only smaller currents as the energy is
dissipated in the base depletion region which is very small. Higher amount of
dissipated energy (higher current for longer time, or a short very high current
spike) causes thermal damage to the junction and/or its contacts. Partial
damage of the junction can shift its Zener voltage. Total destruction of the
Zener junction by overheating it and causing migration of metallization across
the junction ("spiking") can be used intentionally as a 'Zener zap' antifuse.
[5]
**** Subsurface Zeners[edit] ****
Buried zener structure
A subsurface Zener diode, also called 'buried Zener', is a device similar to
the Surface Zener, but with the avalanche region located deeper in the
structure, typically several micrometers below the oxide. The hot carriers then
lose energy by collisions with the semiconductor lattice before reaching the
oxide layer and cannot be trapped there. The Zener walkout phenomenon therefore
does not occur here, and the buried Zeners have voltage constant over their
entire lifetime. Most buried Zeners have breakdown voltage of 5â7 volts.
Several different junction structures are used.[6]
***** Uses[edit] *****
Zener diode shown with typical packages. Reverse current     &#x2212;  i  Z
{\displaystyle -i_{Z}}  [-i_{Z}] is shown.
Zener diodes are widely used as voltage references and as shunt regulators to
regulate the voltage across small circuits. When connected in parallel with a
variable voltage source so that it is reverse biased, a Zener diode conducts
when the voltage reaches the diode's reverse breakdown voltage. From that point
on, the low impedance of the diode keeps the voltage across the diode at that
value.[7]
[Zener_diode_voltage_regulator.svg]
In this circuit, a typical voltage reference or regulator, an input voltage,
Uin, is regulated down to a stable output voltage Uout. The breakdown voltage
of diode D is stable over a wide current range and holds Uout approximately
constant even though the input voltage may fluctuate over a wide range. Because
of the low impedance of the diode when operated like this, resistor R is used
to limit current through the circuit.
In the case of this simple reference, the current flowing in the diode is
determined using Ohm's law and the known voltage drop across the resistor R;
          I  diode   =     U  in   &#x2212;  U  out    R     {\displaystyle I_
      {\text{diode}}={\frac {U_{\text{in}}-U_{\text{out}}}{R}}}  [
      {\displaystyle I_{\text{diode}}={\frac {U_{\text{in}}-U_{\text{out}}}
      {R}}}]
The value of R must satisfy two conditions:
   1. R must be small enough that the current through D keeps D in reverse
      breakdown. The value of this current is given in the data sheet for D.
      For example, the common BZX79C5V6[8] device, a 5.6 V 0.5 W Zener diode,
      has a recommended reverse current of 5 mA. If insufficient current exists
      through D, then Uout is unregulated and less than the nominal breakdown
      voltage (this differs from voltage-regulator_tubes where the output
      voltage is higher than nominal and could rise as high as Uin). When
      calculating R, allowance must be made for any current through the
      external load, not shown in this diagram, connected across Uout.
   2. R must be large enough that the current through D does not destroy the
      device. If the current through D is ID, its breakdown voltage VB and its
      maximum power dissipation Pmax correlate as such:      I  D    V  B   <
      P  max     {\displaystyle I_{D}V_{B}<P_{\text{max}}}  [{\displaystyle I_
      {D}V_{B}<P_{\text{max}}}].
A load may be placed across the diode in this reference circuit, and as long as
the Zener stays in reverse breakdown, the diode provides a stable voltage
source to the load. Zener diodes in this configuration are often used as stable
references for more advanced voltage regulator circuits.
Shunt regulators are simple, but the requirements that the ballast resistor be
small enough to avoid excessive voltage drop during worst-case operation (low
input voltage concurrent with high load current) tends to leave a lot of
current flowing in the diode much of the time, making for a fairly wasteful
regulator with high quiescent power dissipation, only suitable for smaller
loads.
These devices are also encountered, typically in series with a base-emitter
junction, in transistor stages where selective choice of a device centered on
the avalanche or Zener point can be used to introduce compensating temperature
co-efficient balancing of the transistor pân_junction. An example of this
kind of use would be a DC error_amplifier used in a regulated_power_supply
circuit feedback loop system.
Zener diodes are also used in surge_protectors to limit transient voltage
spikes.
Another application of the Zener diode is the use of noise caused by its
avalanche_breakdown in a random_number_generator.
**** Waveform clipper[edit] ****
Examples of a waveform clipper
Two Zener diodes facing each other in series clip both halves of an input
signal. Waveform_clippers can be used not only to reshape a signal, but also to
prevent voltage spikes from affecting circuits that are connected to the power
supply.[9]
**** Voltage shifter[edit] ****
Examples of a voltage shifter
A Zener diode can be applied to a circuit with a resistor to act as a voltage
shifter. This circuit lowers the output voltage by a quantity that is equal to
the Zener diode's breakdown voltage.
**** Voltage regulator[edit] ****
Examples of a voltage regulator
A Zener diode can be applied in a voltage_regulator circuit to regulate the
voltage applied to a load, such as in a linear_regulator.
***** See also[edit] *****
 Wikimedia Commons has media related to Zener_diodes.
    * Backward_diode
    * E-series_of_preferred_numbers
    * Transient_voltage_suppression_diode
***** References[edit] *****
   1. ^ a bMillman, Jacob (1979). Microelectronics. McGraw Hill. pp. 45â48.
      ISBN 978-0071005968.
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
   3. ^ a bDorf, Richard C., ed. (1993). The Electrical Engineering Handbook.
      Boca Raton: CRC Press. p. 457. ISBN 0-8493-0185-8.
   4. ^Calibration: Philosophy in Practice. Fluke. 1994. pp. 7â10.
      ISBN 0963865005.
   5. ^ Rakesh Kumar Garg, Ashish Dixit, Pavan Yadav, Basic Electronics, p.
      150, Firewall Media, 2008
   6. ISBN 8131803023.
   7. ^Comer, Donald T. (1996). "Zener Zap Anti-Fuse Trim in VLSI Circuits".
      VLSI Design. 5: 89. doi:10.1155/1996/23706.
   8. ^Hastings, Alan (2005). The Art of Analog Layout (Second ed.). Prentice
      Hall. ISBN 9780131464100.
   9. ^Horowitz, Paul; Hill, Winfield (1989). The Art of Electronics (2nd ed.).
      Cambridge University Press. pp. 68â69. ISBN 0-521-37095-7.
  10. ^"BZX79C5V6_â_5.6V,_0.5W_Zener_Diode_-_data_sheet". Fairchild
      Semiconductor. Retrieved July 22, 2014.
  11. ^Diffenderfer, Robert (2005). Electronic_Devices:_Systems_and
      Applications. Thomas Delmar Learning. pp. 95â100. ISBN 1401835147.
      Retrieved July 22, 2014.
***** Further reading[edit] *****
    * TVS/Zener Theory and Design Considerations; ON Semiconductor; 127 pages;
      2005; HBD854/D. (Free_PDF_download)
***** External links[edit] *****
    * Zener_Diode_Axial_Part_Number_Table
    * v
    * t
    * e
Electronic_components
                                         * Complementary_MOS (CMOS)
                                         * Depletion-load_NMOS
                                         * Fin_field-effect_transistor (FinFET)
                                         * Floating-gate_MOSFET (FGMOS)
                                         * Insulated-gate_bipolar_transistor
                                           (IGBT)
                                         * LDMOS
                   MOS_transistors       * MOS_field-effect_transistor (MOSFET)
                                         * Multi-gate_field-effect_transistor
                                           (MuGFET)
                                         * NMOS
                                         * PMOS
                                         * Power_MOSFET
                                         * Thin-film_transistor (TFT)
                                         * VMOS
                                         * Bipolar_junction_transistor (BJT)
                                         * Darlington_transistor
                                         * Diffusion_transistor
                                         * Field-effect_transistor (FET)
                                         * JFET
                                         * Light-emitting_transistor (LET)
                                         * Organic_field-effect_transistor
                                           (OFET)
                   Other_transistors     * Organic_light-emitting_transistor
                                           (OLET)
                                         * Pentode_transistor
                                         * Point-contact_transistor
                                         * Programmable_unijunction_transistor
Semiconductor                              (PUT)
devices                                  * Static_induction_transistor (SIT)
                                         * Tetrode_transistor
                                         * Unijunction_transistor (UJT)
                                         * Avalanche_diode
                                         * Constant-current_diode (CLD, CRD)
                                         * Laser_diode (LD)
                                         * Light-emitting_diode (LED)
                   Diodes                * Photodiode
                                         * PIN_diode
                                         * Schottky_diode
                                         * Step_recovery_diode
                                         * Zener diode
                                         * DIAC
                                         * Heterostructure_barrier_varactor
                                         * Integrated_circuit (IC)
                                         * Memistor
                                         * Memory_cell
                                         * Memristor
                                         * Organic_semiconductor
                                         * Photodetector
                   Other devices         * Solaristor
                                         * Quantum_circuit
                                         * Silicon_controlled_rectifier (SCR)
                                         * Static_induction_thyristor (SITh)
                                         * Three-dimensional_integrated_circuit
                                           (3D IC)
                                         * Thyristor
                                         * TRIAC
                                         * Varicap
                       * Linear_regulator
                       * Low-dropout_regulator
                       * Switching_regulator
                       * Buck
                       * Boost
Voltage_regulators     * Buckâboost
                       * Split-pi
                       * Äuk
                       * SEPIC
                       * Charge_pump
                       * Switched_capacitor
                       * Acorn_tube
                       * Audion
                       * Beam_tetrode
                       * Barretter
                       * Compactron
                       * Diode
                       * Fleming_valve
Vacuum_tubes           * Nonode
                       * Nuvistor
                       * Pentagrid (Hexode, Heptode, Octode)
                       * Pentode
                       * Photomultiplier
                       * Phototube
                       * Tetrode
                       * Triode
                       * Backward-wave_oscillator (BWO)
                       * Cavity_magnetron
                       * Crossed-field_amplifier (CFA)
                       * Gyrotron
Vacuum_tubes (RF)      * Inductive_output_tube (IOT)
                       * Klystron
                       * Maser
                       * Sutton_tube
                       * Traveling-wave_tube (TWT)
                       * Beam_deflection_tube
                       * Charactron
                       * Iconoscope
                       * Magic_eye_tube
Cathode_ray_tubes      * Monoscope
                       * Selectron_tube
                       * Storage_tube
                       * Trochotron
                       * Video_camera_tube
                       * Williams_tube
                       * Cold_cathode
                       * Crossatron
                       * Dekatron
                       * Ignitron
                       * Krytron
Gas-filled_tubes       * Mercury-arc_valve
                       * Neon_lamp
                       * Nixie_tube
                       * Thyratron
                       * Trigatron
                       * Voltage-regulator_tube
                       * Potentiometer
Adjustable                   o digital
                       * Variable_capacitor
                       * Varicap
                       * Connector
                             o audio_and_video
                             o electrical_power
                             o RF
                       * Electrolytic_detector
                       * Ferrite
                       * Fuse
Passive                      o resettable
                       * Resistor
                       * Switch
                       * Thermistor
                       * Transformer
                       * Varistor
                       * Wire
                             o Wollaston_wire
                       * Capacitor
                             o types
                       * Ceramic_resonator
                       * Crystal_oscillator
Reactive               * Inductor
                       * Parametron
                       * Relay
                             o reed_relay
                             o mercury_switch
Authority_control [Edit_this_at_Wikidata]     * GND: 4190693-7

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Zener_diode&oldid=907989932"
Categories:
    * Diodes
    * Voltage_stability
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_February_2013
    * Articles_with_unsourced_statements_from_November_2017
    * Commons_category_link_is_on_Wikidata
    * Wikipedia_articles_with_GND_identifiers
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * à²à²¨à³à²¨à²¡
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * Latina
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * Simple_English
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à°¤à±à°²à±à°à±
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 26 July 2019, at 16:58 (UTC).
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
