The following text has been accessed from https://en.wikipedia.org/wiki/Power_supply at Fri Aug 9 03:36:24 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Power supply ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other uses, see Power_supply_(disambiguation).
A simple general purpose desktop power supply used in electronic labs, with
power output connector seen at lower-left and power input connector (not shown)
located at the rear
A power supply is an electrical device that supplies electric_power to an
electrical_load. The primary function of a power supply is to convert electric
current from a source to the correct voltage, current, and frequency to power
the load. As a result, power supplies are sometimes referred to as electric
power_converters. Some power supplies are separate standalone pieces of
equipment, while others are built into the load appliances that they power.
Examples of the latter include power supplies found in desktop_computers and
consumer_electronics devices. Other functions that power supplies may perform
include limiting the current drawn by the load to safe levels, shutting off the
current in the event of an electrical_fault, power conditioning to prevent
electronic_noise or voltage_surges on the input from reaching the load, power-
factor_correction, and storing energy so it can continue to power the load in
the event of a temporary interruption in the source power (uninterruptible
power_supply).
All power supplies have a power input connection, which receives energy in the
form of electric current from a source, and one or more power output
connections that deliver current to the load. The source power may come from
the electric_power_grid, such as an electrical_outlet, energy_storage devices
such as batteries or fuel_cells, generators or alternators, solar_power
converters, or another power supply. The input and output are usually hardwired
circuit connections, though some power supplies employ wireless_energy_transfer
to power their loads without wired connections. Some power supplies have other
types of inputs and outputs as well, for functions such as external monitoring
and control.
⁰
***** Contents *****
    * 1_General_classification
          o 1.1_Functional
          o 1.2_Packaging
          o 1.3_Power_conversion_method
    * 2_Types
          o 2.1_DC_power_supply
                # 2.1.1_AC-to-DC_supply
                # 2.1.2_Switched-mode_power_supply
                # 2.1.3_Linear_regulator
          o 2.2_AC_power_supplies
                # 2.2.1_AC_adapter
          o 2.3_Programmable_power_supply
          o 2.4_Uninterruptible_power_supply
          o 2.5_High-voltage_power_supply
          o 2.6_Bipolar_power_supply
    * 3_Specification
    * 4_Thermal_Management
    * 5_Overload_protection
          o 5.1_Current_limiting
    * 6_Applications
          o 6.1_Computers
          o 6.2_Electric_Vehicles
          o 6.3_Welding
          o 6.4_Aircraft
          o 6.5_Automation
          o 6.6_Medical
    * 7_See_also
    * 8_References
    * 9_External_links
***** General classification[edit] *****
A rackmount, adjustable regulated DC power supply
**** Functional[edit] ****
Power supplies are categorized in various ways, including by functional
features. For example, a regulated_power_supply is one that maintains constant
output voltage or current despite variations in load current or input voltage.
Conversely, the output of an unregulated power supply can change significantly
when its input voltage or load current changes. Adjustable power supplies allow
the output voltage or current to be programmed by mechanical controls (e.g.,
knobs on the power supply front panel), or by means of a control input, or
both. An adjustable regulated power supply is one that is both adjustable and
regulated. An isolated power supply has a power output that is electrically
independent of its power input; this is in contrast to other power supplies
that share a common connection between power input and output.
**** Packaging[edit] ****
Power supplies are packaged in different ways and classified accordingly. A
bench power supply is a stand-alone desktop unit used in applications such as
circuit test and development. Open frame power supplies have only a partial
mechanical enclosure, sometimes consisting of only a mounting base; these are
typically built into machinery or other equipment. Rack_mount power supplies
are designed to be secured into standard electronic equipment racks. An
integrated power supply is one that shares a common printed_circuit_board with
its load. An external power supply, AC adapter or power brick, is a power
supply located in the load's AC power cord that plugs into a wall outlet; a
wall wart is an external supply integrated with the outlet plug itself. These
are popular in consumer electronics because of their safety; the hazardous 120
or 240 volt main current is transformed down to a safer voltage before it
enters the appliance body.
**** Power conversion method[edit] ****
Power supplies can be broadly divided into linear and switching types. Linear
power converters process the input power directly, with all active power
conversion components operating in their linear operating regions. In switching
power converters, the input power is converted to AC or to DC pulses before
processing, by components that operate predominantly in non-linear modes (e.g.,
transistors that spend most of their time in cutoff or saturation). Power is
"lost" (converted to heat) when components operate in their linear regions and,
consequently, switching converters are usually more efficient than linear
converters because their components spend less time in linear operating
regions.
***** Types[edit] *****
**** DC power supply[edit] ****
A DC power supply is one that supplies a constant DC voltage to its load.
Depending on its design, a DC power supply may be powered from a DC source or
from an AC source such as the power mains.
*** AC-to-DC supply[edit] ***
Schematic of basic AC-to-DC power supply, showing (from L-R) transformer, full-
wave bridge rectifier, filter capacitor and resistor load
DC power supplies use AC mains_electricity as an energy source. Such power
supplies will employ a transformer to convert the input voltage to a higher or
lower AC voltage. A rectifier is used to convert the transformer output voltage
to a varying DC voltage, which in turn is passed through an electronic_filter
to convert it to an unregulated DC voltage.
The filter removes most, but not all of the AC voltage variations; the
remaining AC voltage is known as ripple. The electric load's tolerance of
ripple dictates the minimum amount of filtering that must be provided by a
power supply. In some applications, high ripple is tolerated and therefore no
filtering is required. For example, in some battery charging applications it is
possible to implement a mains-powered DC power supply with nothing more than a
transformer and a single rectifier diode, with a resistor in series with the
output to limit charging current.
*** Switched-mode power supply[edit] ***
Main article: Switched-mode_power_supply
In a switched-mode_power_supply (SMPS), the AC mains input is directly
rectified and then filtered to obtain a DC voltage. The resulting DC voltage is
then switched on and off at a high frequency by electronic switching circuitry,
thus producing an AC current that will pass through a high-frequency
transformer or inductor. Switching occurs at a very high frequency (typically
10 kHz â 1 MHz), thereby enabling the use of transformers and filter
capacitors that are much smaller, lighter, and less expensive than those found
in linear power supplies operating at mains frequency. After the inductor or
transformer secondary, the high frequency AC is rectified and filtered to
produce the DC output voltage. If the SMPS uses an adequately insulated high-
frequency transformer, the output will be electrically_isolated from the mains;
this feature is often essential for safety.
Switched-mode power supplies are usually regulated, and to keep the output
voltage constant, the power supply employs a feedback controller that monitors
current drawn by the load. The switching duty_cycle increases as power output
requirements increase.
SMPSs often include safety features such as current limiting or a crowbar
circuit to help protect the device and the user from harm.[1] In the event that
an abnormal high-current power draw is detected, the switched-mode supply can
assume this is a direct short and will shut itself down before damage is done.
PC power supplies often provide a power_good signal to the motherboard; the
absence of this signal prevents operation when abnormal supply voltages are
present.
Some SMPSs have an absolute limit on their minimum current output.[2] They are
only able to output above a certain power level and cannot function below that
point. In a no-load condition the frequency of the power slicing circuit
increases to great speed, causing the isolated transformer to act as a Tesla
coil, causing damage due to the resulting very high voltage power spikes.
Switched-mode supplies with protection circuits may briefly turn on but then
shut down when no load has been detected. A very small low-power dummy_load
such as a ceramic power resistor or 10-watt light bulb can be attached to the
supply to allow it to run with no primary load attached.
The switch-mode power supplies used in computers have historically had low
power_factors and have also been significant sources of line interference (due
to induced power_line_harmonics and transients). In simple switch-mode power
supplies, the input stage may distort the line voltage waveform, which can
adversely affect other loads (and result in poor power quality for other
utility customers), and cause unnecessary heating in wires and distribution
equipment. Furthermore, customers incur higher electric bills when operating
lower power factor loads. To circumvent these problems, some computer switch-
mode power supplies perform power factor correction, and may employ input
filters or additional switching stages to reduce line interference.
*** Linear regulator[edit] ***
The function of a linear_voltage_regulator is to convert a varying DC voltage
to a constant, often specific, lower DC voltage. In addition, they often
provide a current_limiting function to protect the power supply and load from
overcurrent (excessive, potentially destructive current).
A constant output voltage is required in many power supply applications, but
the voltage provided by many energy sources will vary with changes in load
impedance. Furthermore, when an unregulated DC power supply is the energy
source, its output voltage will also vary with changing input voltage. To
circumvent this, some power supplies use a linear voltage regulator to maintain
the output voltage at a steady value, independent of fluctuations in input
voltage and load impedance. Linear regulators can also reduce the magnitude of
ripple and noise on the output voltage.
**** AC power supplies[edit] ****
An AC power supply typically takes the voltage from a wall outlet (mains
supply) and uses a transformer to step up or step down the voltage to the
desired voltage. Some filtering may take place as well. In some cases, the
source voltage is the same as the output voltage; this is called an isolation
transformer. Other AC power supply transformers do not provide mains isolation;
these are called autotransformers; a variable output autotransformer is known
as a variac. Other kinds of AC power supplies are designed to provide a nearly
constant_current, and output voltage may vary depending on impedance of the
load. In cases when the power source is direct current, (like an automobile
storage battery), an inverter and step-up transformer may be used to convert it
to AC power. Portable AC power may be provided by an alternator powered by a
diesel or gasoline engine (for example, at a construction site, in an
automobile or boat, or backup power generation for emergency services) whose
current is passed to a regulator circuit to provide a constant voltage at the
output. Some kinds of AC power conversion do not use a transformer. If the
output voltage and input voltage are the same, and primary purpose of the
device is to filter AC power, it may be called a line_conditioner. If the
device is designed to provide backup power, it may be called an uninterruptable
power_supply. A circuit may be designed with a voltage_multiplier topology to
directly step-up AC power; formerly, such an application was a vacuum tube AC/
DC_receiver.
In modern use, AC power supplies can be divided into single_phase and three
phase systems. "The primary difference between single phase and three phase AC
power is the constancy of delivery." [3] AC power Supplies can also be used to
change the frequency as well as the voltage, they are often used by
manufacturers to check the suitability of their products for use in other
countries. 230 V 50 Hz or 115 60 Hz or even 400 Hz for avionics testing.
*** AC adapter[edit] ***
Switch-mode mobile phone charger
Main article: AC_adapter
An AC adapter is a power supply built into an AC_mains_power_plug. AC adapters
are also known by various other names such as "plug pack" or "plug-in adapter",
or by slang terms such as "wall wart". AC adapters typically have a single AC
or DC output that is conveyed over a hardwired cable to a connector, but some
adapters have multiple outputs that may be conveyed over one or more cables.
"Universal" AC adapters have interchangeable input connectors to accommodate
different AC mains voltages.
Adapters with AC outputs may consist only of a passive transformer (plus a few
diodes in DC-output adapters), or they may employ switch-mode circuitry. AC
adapters consume power (and produce electric and magnetic fields) even when not
connected to a load; for this reason they are sometimes known as "electricity
vampires", and may be plugged into power_strips to allow them to be
conveniently turned on and off.
**** Programmable power supply[edit] ****
Programmable power supplies
A programmable power supply is one that allows remote control of its operation
through an analog input or digital interface such as RS232 or GPIB. Controlled
properties may include voltage, current, and in the case of AC output power
supplies, frequency. They are used in a wide variety of applications, including
automated equipment testing, crystal_growth monitoring, semiconductor
fabrication, and x-ray generators.
Programmable power supplies typically employ an integral microcomputer to
control and monitor power supply operation. Power supplies equipped with a
computer interface may use proprietary communication protocols or standard
protocols and device control languages such as SCPI.
**** Uninterruptible power supply[edit] ****
Main article: Uninterruptible_power_supply
An uninterruptible power supply (UPS) takes its power from two or more sources
simultaneously. It is usually powered directly from the AC mains, while
simultaneously charging a storage battery. Should there be a dropout or failure
of the mains, the battery instantly takes over so that the load never
experiences an interruption. Instantly here should be defined as the speed of
electricity within conductors which is somewhat near the speed of light. That
definition is important because transmission of high speed data and
communications service must have continuity/NO break of that service. Some
manufacturers use a quasi standard of 4 milliseconds. However, with high speed
data even 4 ms of time in transitioning from one source to another is not fast
enough. The transition must be made in a break before make method. The UPS
meeting that requirement is referred to as a True UPS or a Hybrid UPS. How much
time the UPS will provide is most often based on batteries and in conjunction
with generators. That time can range from a quasi minimum 5 to 15 minutes to
literally hours or even days. In many computer installations, only enough time
on batteries to give the operators time to shut down the system in an orderly
way. Other UPS schemes may use an internal combustion engine or turbine to
supply power during a utility power outage and the amount of battery time is
then dependent upon how long it takes the generator to be on line and the
criticality of the equipment served. Such a scheme is found in hospitals, data
centers, call centers, cell sites and telephone central offices.
**** High-voltage power supply[edit] ****
A 30 kV high-voltage power supply with Federal Standard connector, used in
electron microscopes
A high-voltage power supply is one that outputs hundreds or thousands of volts.
A special output connector is used that prevents arcing, insulation breakdown
and accidental human contact. Federal Standard connectors are typically used
for applications above 20 kV, though other types of connectors (e.g., SHV
connector) may be used at lower voltages. Some high-voltage power supplies
provide an analog input or digital communication interface that can be used to
control the output voltage. High-voltage power supplies are commonly used to
accelerate and manipulate electron and ion beams in equipment such as x-ray
generators, electron_microscopes, and focused_ion_beam columns, and in a
variety of other applications, including electrophoresis and electrostatics.
High-voltage power supplies typically apply the bulk of their input energy to a
power_inverter, which in turn drives a voltage_multiplier or a high turns
ratio, high-voltage transformer, or both (usually a transformer followed by a
multiplier) to produce high voltage. The high voltage is passed out of the
power supply through the special connector and is also applied to a voltage
divider that converts it to a low-voltage metering signal compatible with low-
voltage circuitry. The metering signal is used by a closed-loop controller that
regulates the high voltage by controlling inverter input power, and it may also
be conveyed out of the power supply to allow external circuitry to monitor the
high-voltage output.
**** Bipolar power supply[edit] ****
A bipolar power supply (Kepco BOP 6-125MG)
A bipolar power supply operates in all four quadrants of the voltage/current
Cartesian plane, meaning that it will generate positive and negative voltages
and currents as required to maintain regulation.[4] When its output is
controlled by a low-level analog signal, it is effectively a low-bandwidth
operational_amplifier with high output power and seamless zero-crossings. This
type of power supply is commonly used to power magnetic devices in scientific
applications.[example_needed]
***** Specification[edit] *****
The suitability of a particular power supply for an application is determined
by various attributes of the power supply, which are typically listed in the
power supply's specification. Commonly specified attributes for a power supply
include:
    * Input voltage type (AC or DC) and range
    * Efficiency of power conversion
    * The amount of voltage and current it can supply to its load
    * How stable its output voltage or current is under varying line and load
      conditions
    * How long it can supply energy without refueling or recharging (applies to
      power supplies that employ portable energy sources)
    * Operating and storage temperature ranges
Commonly-used abbreviations used in power supply specifications:
    * SCP - Short circuit protection
    * OPP - Overpower (overload) protection
    * OCP - Overcurrent protection
    * OTP - Overtemperature protection
    * OVP - Overvoltage protection
    * UVP - Undervoltage protection
***** Thermal Management[edit] *****
The power supply of an electrical system tends to generate much heat. The
higher the efficiency, the more heat is pulled away from the unit. There are
many ways to manage the heat of a power supply unit. The types of cooling
generally fall into two categories -- convection and conduction. Common
convection methods for cooling electronic power supplies include natural air
flow, forced air flow, or other liquid flow over the unit. Common conduction
cooling methods include heat_sinks, cold plates, and thermal compounds. [5]
***** Overload protection[edit] *****
Power supplies often have protection from short_circuit or overload that could
damage the supply or cause a fire. Fuses and circuit_breakers are two commonly
used mechanisms for overload protection.[6]
A fuse contains a short piece of wire which melts if too much current flows.
This effectively disconnects the power supply from its load, and the equipment
stops working until the problem that caused the overload is identified and the
fuse is replaced. Some power supplies use a very thin wire_link soldered in
place as a fuse. Fuses in power supply units may be replaceable by the end
user, but fuses in consumer equipment may require tools to access and change.
A circuit breaker contains an element that heats, bends and triggers a spring
which shuts the circuit down. Once the element cools, and the problem is
identified the breaker can be reset and the power restored.
Some PSUs use a thermal_cutout buried in the transformer rather than a fuse.
The advantage is it allows greater current to be drawn for limited time than
the unit can supply continuously. Some such cutouts are self resetting, some
are single use only.
**** Current limiting[edit] ****
Some supplies use current limiting instead of cutting off power if overloaded.
The two types of current limiting used are electronic limiting and impedance
limiting. The former is common on lab bench PSUs, the latter is common on
supplies of less than 3 watts output.
A foldback_current_limiter reduces the output current to much less than the
maximum non-fault current.
***** Applications[edit] *****
Power supplies are a fundamental component of many electronic devices and
therefore used in a diverse range of applications. This list is a small sample
of the many applications of power supplies.
**** Computers[edit] ****
Main article: Power_supply_unit_(computer)
A modern computer power supply is a switch-mode power supply that converts AC
power from the mains supply, to several DC voltages. Switch-mode supplies
replaced linear supplies due to cost, weight, and size improvement. The diverse
collection of output voltages also have widely varying current draw
requirements.
**** Electric Vehicles[edit] ****
Electric_vehicles are those which rely on energy created through electricity
generation. A power supply unit is part of the necessary design to convert high
voltage vehicle battery power.[7]
**** Welding[edit] ****
Main article: Welding_power_supply
Arc_welding uses electricity to join metals by melting them. The electricity is
provided by a welding power supply, and can either be AC or DC. Arc welding
requires high currents typically between 100 and 350 amperes. Some types of
welding can use as few as 10 amperes, while some applications of spot_welding
employ currents as high as 60,000 amperes for an extremely short time. Welding
power supplies consisted of transformers or engines driving generators; modern
welding equipment uses semiconductors and may include microprocessor control.
**** Aircraft[edit] ****
Both commercial and military avionic systems require either a DC-DC or AC/DC
power supply to convert energy into usable voltage. These may often operate_at
400Hz in the interest of weight savings.
**** Automation[edit] ****
This refers to conveyors, assembly lines, bar code readers, cameras, motors,
pumps, semi-fabricated manufacturing and more.
**** Medical[edit] ****
These include ventilators, infusion pumps, surgical and dental instruments,
imaging and beds.
***** See also[edit] *****
    * [icon]Electronics_portal
    * [icon]Energy_portal
    * AC_adapter
    * Capacitive_power_supply
    * Electricity_generation
    * High_voltage
    * Mains_electricity_by_country
    * Motorâgenerator
    * Power_cord
    * Sense_(electronics)
    * Voltage_regulator
    * Category:Power_supply_manufacturers
***** References[edit] *****
   1. ^ Quoting US patent #4937722, High efficiency direct coupled switched
      mode power supply: The power supply can also include crowbar circuit
      protecting it against damage by clamping the output to ground if it
      exceeds a particular voltage."Archived_copy". Archived from the_original
      on 2013-04-21. Retrieved 2008-05-08.CS1 maint: Archived copy as title
      (link)
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
   3. ^ Quoting US Patent #5402059: A problem can occur when loads on the
      output of a switching power supply become disconnected from the supply.
      When this occurs, the output current from the power supply becomes
      reduced (or eliminated if all loads become disconnected). If the output
      current becomes small enough, the output voltage of the power supply can
      reach the peak value of the secondary voltage of the transformer of the
      power supply. This occurs because with a very small output current, the
      inductor in the L-C low-pass filter does not drop much voltage (if any at
      all). The capacitor in the L-C low-pass filter therefore charges up to
      the peak voltage of the secondary of the transformer. This peak voltage
      is generally considerably higher than the average voltage of the
      secondary of the transformer. The higher voltage which occurs across the
      capacitor, and therefore also at the output of the power supply, can
      damage components within the power supply. The higher voltage can also
      damage any remaining electrical loads connected to the power
      supply."Archived_copy". Archived from the_original on 2012-09-07.
      Retrieved 2008-05-08.CS1 maint: Archived copy as title (link)
   4. ^"What's_the_Difference_Between_Single_Phase_and_Three_Phase_AC_Power
      Supplies?". Aegis Power Systems. Aegis Power Systems. Retrieved 28
      December 2015.
   5. ^"Bipolar_Power_Supplies_Run_The_Voltage_Gamut". Electronic Design. 2012-
      10-19. Retrieved 2018-07-26.
   6. ^"Overview_of_Cooling_Methods_for_AC_and_DC_Power_Supplies". Aegis Power
      Systems. Aegis Power Systems.
   7. ^ Malmstadt, Enke and Crouch, Electronics and Instrumentation for
      Scientists, The Benjamin/Cummings Publishing Company, Inc., 1981,
   8. ISBN 0-8053-6917-1, Chapter 3.
   9. ^"Electric_Vehicle_Power_Converters". Aegis Power Systems. Aegis Power
      Systems.
***** External links[edit] *****
 Look up power_supply in Wiktionary, the free dictionary.
 Wikimedia Commons has media related to Power_supplies.
    * Understanding_Linear_Power_Supply_Operation
    * Load_Power_Sources_for_Peak_Efficiency,_James_Colotti,_EDN_1979_October_5

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Power_supply&oldid=909606033"
Categories:
    * Power_supplies
Hidden categories:
    * CS1_maint:_Archived_copy_as_title
    * All_articles_needing_examples
    * Articles_needing_examples_from_July_2018
    * Commons_category_link_is_locally_defined
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
    * Asturianu
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Jawa
    * Magyar
    * à´®à´²à´¯à´¾à´³à´
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Svenska
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * ä¸­æ
Edit_links
    * This page was last edited on 6 August 2019, at 12:58 (UTC).
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
