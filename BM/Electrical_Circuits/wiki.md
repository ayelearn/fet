The following text has been accessed from https://en.wikipedia.org/wiki/Electrical_network at Fri Aug 9 02:45:02 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Electrical network ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For electrical power transmission grids and distribution networks, see
Electrical_grid.
 This article needs additional citations for verification. Please help improve_this
 article by adding_citations_to_reliable_sources. Unsourced material may be
 challenged and removed.
 Find sources: "Electrical_network" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (March 2016)(Learn_how_and_when_to_remove_this_template_message)
A simple electric circuit made up of a voltage source and a resistor. Here,
V = i R   {\displaystyle V=iR}  [V=iR], according to Ohm's_law.
An electrical network is an interconnection of electrical_components (e.g.,
batteries, resistors, inductors, capacitors, switches, transistors) or a model
of such an interconnection, consisting of electrical_elements (e.g., voltage
sources, current_sources, resistances, inductances, capacitances). An
electrical circuit is a network consisting of a closed loop, giving a return
path for the current. Linear electrical networks, a special type consisting
only of sources (voltage or current), linear lumped elements (resistors,
capacitors, inductors), and linear distributed elements (transmission lines),
have the property that signals are linearly_superimposable. They are thus more
easily analyzed, using powerful frequency_domain methods such as Laplace
transforms, to determine DC_response, AC_response, and transient_response.
A resistive circuit is a circuit containing only resistors and ideal current
and voltage sources. Analysis of resistive circuits is less complicated than
analysis of circuits containing capacitors and inductors. If the sources are
constant (DC) sources, the result is a DC_circuit. The effective resistance and
current distribution properties of arbitrary resistor networks can be modeled
in terms of their graph measures and geometrical properties.[1]
A network that contains active electronic components is known as an electronic
circuit. Such networks are generally nonlinear and require more complex design
and analysis tools.
⁰
***** Contents *****
    * 1_Classification
          o 1.1_By_passivity
          o 1.2_By_linearity
          o 1.3_By_lumpiness
    * 2_Classification_of_sources
          o 2.1_Independent
          o 2.2_Dependent
    * 3_Electrical_laws
    * 4_Design_methods
    * 5_Network_simulation_software
          o 5.1_Linearization_around_operating_point
          o 5.2_Piecewise-linear_approximation
    * 6_See_also
          o 6.1_Representation
          o 6.2_Design_and_analysis_methodologies
          o 6.3_Measurement
          o 6.4_Analogies
          o 6.5_Specific_topologies
    * 7_References
***** Classification[edit] *****
**** By passivity[edit] ****
An active network is a network that contains an active source â either a
voltage_source or current_source.
A passive network is a network that does not contain an active source.
An active network contains one or more sources of electromotive_force. It
consists of active elements like a battery or a transistor. Active elements can
inject power to the circuit, provide power gain, and control the current flow
within the circuit.
Passive networks do not contain any sources of electromotive force. They
consist of passive elements like resistors and capacitors. These elements are
not capable of the same functions as active elements.
**** By linearity[edit] ****
A network is linear if its signals obey the principle of superposition;
otherwise it is non-linear.
**** By lumpiness[edit] ****
Discrete passive components (resistors, capacitors and inductors) are called
lumped elements because all of their, respectively, resistance, capacitance and
inductance is assumed to be located ("lumped") at one place. This design
philosophy is called the lumped_element_model and networks so designed are
called lumped element circuits. This is the conventional approach to circuit
design. At high enough frequencies the lumped assumption no longer holds
because there is a significant fraction of a wavelength across the component
dimensions. A new design model is needed for such cases called the distributed
element_model. Networks designed to this model are called distributed_element
circuits.
A distributed element circuit that includes some lumped components is called a
semi-lumped design. An example of a semi-lumped circuit is the combline_filter.
***** Classification of sources[edit] *****
Sources can be classified as independent sources and dependent sources.
**** Independent[edit] ****
An ideal independent source maintains the same voltage or current regardless of
the other elements present in the circuit. Its value is either constant (DC) or
sinusoidal (AC). The strength of voltage or current is not changed by any
variation in the connected network.
**** Dependent[edit] ****
Dependent_sources depend upon a particular element of the circuit for
delivering the power or voltage or current depending upon the type of source it
is.
***** Electrical laws[edit] *****
A number of electrical laws apply to all electrical networks. These include:
    * Kirchhoff's_current_law: The sum of all currents entering a node is equal
      to the sum of all currents leaving the node.
    * Kirchhoff's_voltage_law: The directed sum of the electrical potential
      differences around a loop must be zero.
    * Ohm's_law: The voltage across a resistor is equal to the product of the
      resistance and the current flowing through it.
    * Norton's_theorem: Any network of voltage or current sources and resistors
      is electrically equivalent to an ideal current source in parallel with a
      single resistor.
    * ThÃ©venin's_theorem: Any network of voltage or current sources and
      resistors is electrically equivalent to a single voltage source in series
      with a single resistor.
    * Superposition_theorem: In a linear network with several independent
      sources, the response in a particular branch when all the sources are
      acting simultaneously is equal to the linear sum of individual responses
      calculated by taking one independent source at a time.
Other more complex laws may be needed if the network contains nonlinear or
reactive components. Non-linear self-regenerative heterodyning systems can be
approximated. Applying these laws results in a set of simultaneous_equations
that can be solved either algebraically or numerically.
***** Design methods[edit] *****
Linear network_analysis
Elements
[Resistance][Capacitor_button.svg][Inductor_button.svg][Reactance][Impedance]
[Voltage_button.svg]
[Conductance][Elastance_button.svg][Blank_button.svg][Susceptance_button.svg]
[Admittance_button.svg][Current_button.svg]
Components
[Resistor_button.svg] [Capacitor_button.svg] [Inductor_button.svg] [Ohm's_law
button.svg]
Series_and_parallel_circuits
[Series_resistor_button.svg][Parallel_resistor_button.svg][Series_capacitor
button.svg][Parallel_capacitor_button.svg][Series_inductor_button.svg]
[Parallel_inductor_button.svg]
Impedance_transforms
[Y-Î_transform] [Î-Y_transform] [star-polygon_transforms] [Dual_button.svg]
Generator theorems                       Network theorems
[Thevenin_button.svg][Norton_button.svg] [KCL_button.svg][KVL_button.svg]
[Millman_button.svg]                     [Tellegen_button.svg]
Network analysis methods
[KCL_button.svg] [KVL_button.svg] [Superposition_button.svg]
Two-port_parameters
[z-parameters][y-parameters][h-parameters][g-parameters][Abcd-parameter
button.svg][S-parameters]
                                             * view
                                             * talk
                                             * edit
See also: Network_analysis_(electrical_circuits)
To design any electrical circuit, either analog or digital, electrical
engineers need to be able to predict the voltages and currents at all places
within the circuit. Simple linear_circuits can be analyzed by hand using
complex_number_theory. In more complex cases the circuit may be analyzed with
specialized computer_programs or estimation techniques such as the piecewise-
linear model.
Circuit simulation software, such as HSPICE (an analog circuit simulator),[2]
and languages such as VHDL-AMS and verilog-AMS allow engineers to design
circuits without the time, cost and risk of error involved in building circuit
prototypes.
***** Network simulation software[edit] *****
More complex circuits can be analyzed numerically with software such as SPICE
or GNUCAP, or symbolically using software such as SapWin.
**** Linearization around operating point[edit] ****
When faced with a new circuit, the software first tries to find a steady_state
solution, that is, one where all nodes conform to Kirchhoff's current law and
the voltages across and through each element of the circuit conform to the
voltage/current equations governing that element.
Once the steady state solution is found, the operating points of each element
in the circuit are known. For a small signal analysis, every non-linear element
can be linearized around its operation point to obtain the small-signal
estimate of the voltages and currents. This is an application of Ohm's Law. The
resulting linear circuit matrix can be solved with Gaussian_elimination.
**** Piecewise-linear approximation[edit] ****
Software such as the PLECS interface to Simulink uses piecewise-linear
approximation of the equations governing the elements of a circuit. The circuit
is treated as a completely linear network of ideal_diodes. Every time a diode
switches from on to off or vice versa, the configuration of the linear network
changes. Adding more detail to the approximation of equations increases the
accuracy of the simulation, but also increases its running time.
***** See also[edit] *****
 Wikimedia Commons has media related to electric_circuits.
 Look up electrical_circuit in Wiktionary, the free dictionary.
    * Digital_circuit
    * Ground_(electricity)
    * Impedance
    * Load
    * Memristor
    * Open-circuit_voltage
    * Short_circuit
    * Voltage_drop
**** Representation[edit] ****
    * Circuit_diagram
    * Schematic
    * Netlist
**** Design and analysis methodologies[edit] ****
    * Network_analysis_(electrical_circuits)
    * Mathematical_methods_in_electronics
    * Superposition_theorem
    * Topology_(electronics)
    * Mesh_analysis
    * Prototype_filter
**** Measurement[edit] ****
    * Network_analyzer_(electrical)
    * Network_analyzer_(AC_power)
    * Continuity_test
**** Analogies[edit] ****
    * Hydraulic_analogy
    * Mechanical-electrical_analogies
    * Impedance_analogy
    * Mobility_analogy
**** Specific topologies[edit] ****
    * Bridge_circuit
    * LC_circuit
    * RC_circuit
    * RL_circuit
    * RLC_circuit
    * Potential_divider
    * Series_and_parallel_circuits
***** References[edit] *****
   1. ^Kumar, Ankush; Vidhyadhiraja, N. S.; Kulkarni, G. U . (2017). "Current
      distribution_in_conducting_nanowire_networks". Journal of Applied
      Physics. 122: 045101. Bibcode:2017JAP...122d5101K. doi:10.1063/1.4985792.
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
   3. ^"HSPICE" (PDF). HSpice. Stanford University, Electrical Engineering
      Department. 1999.
    * [Nuvola_apps_ksim.png]Electronics_portal
Authority_control [Edit_this_at_Wikidata]     * GND: 4052056-0
                                              * NDL: 00561333

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Electrical_network&oldid=908959802"
Categories:
    * Electricity
    * Electrical_engineering
Hidden categories:
    * Articles_needing_additional_references_from_March_2016
    * All_articles_needing_additional_references
    * Commons_category_link_is_locally_defined
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_NDL_identifiers
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
    * Afrikaans
    * á áá­á
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * KreyÃ²l_ayisyen
    * Latina
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Bahasa_Melayu
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * à¤¨à¥à¤ªà¤¾à¤²à¥
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Occitan
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Runa_Simi
    * Ð ÑÑÐ¸Ð½ÑÑÐºÑÐ¹
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * TÃ¼rkmenÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * Wolof
    * å´è¯­
    * ä¸­æ
Edit_links
    * This page was last edited on 2 August 2019, at 03:50 (UTC).
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
