The following text has been accessed from https://en.wikipedia.org/wiki/Thermistor at Fri Aug 9 01:29:57 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Thermistor ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
                                 Thermistor
[NTC_bead.jpg]
Negative temperature coefficient (NTC) thermistor, bead type, insulated wires
Type              Passive
Working principle Electric_resistance
Electronic_symbol
[Thermistor.svg]
Thermistor symbol
A thermistor is a type of resistor whose resistance is dependent on
temperature, more so than in standard resistors. The word is a portmanteau of
thermal and resistor. Thermistors are widely used as inrush_current_limiters,
temperature sensors (negative temperature coefficient or NTC type typically),
self-resetting_overcurrent_protectors, and self-regulating heating_elements
(positive temperature coefficient or PTC type typically).
Thermistors are of two opposite fundamental types:
    * With NTC thermistors, resistance decreases as temperature rises. An NTC
      is commonly used as a temperature sensor, or in series with a circuit as
      an inrush current limiter.
    * With PTC thermistors, resistance increases as temperature rises. PTC
      thermistors are commonly installed in series with a circuit, and used to
      protect against overcurrent conditions, as resettable fuses.
Thermistors are generally produced using powdered metal oxides.[1] With vastly
improved formulas and techniques over the past 20 years, NTC thermistors can
now achieve precision accuracies over wide temperature ranges such as such as
Â±0.1 Â°C or Â±0.2 Â°C from 0 Â°C to 70 Â°C with excellent long-term stability.
NTC thermistor elements come in many styles [2] such as axial-leaded glass-
encapsulated (DO-35, DO-34 and DO-41 diodes), glass-coated chips, epoxy-coated
with bare or insulated lead wire and surface-mount, as well as rods and discs.
The typical operating temperature range of a thermistor is â55 Â°C to
+150 Â°C, though some glass-body thermistors have a maximal operating
temperature of +300 Â°C.
Thermistors differ from resistance_temperature_detectors (RTDs) in that the
material used in a thermistor is generally a ceramic or polymer, while RTDs use
pure metals. The temperature response is also different; RTDs are useful over
larger temperature ranges, while thermistors typically achieve a greater
precision within a limited temperature range, typically â90 Â°C to 130 Â°C.
[3]
⁰
***** Contents *****
    * 1_Basic_operation
    * 2_SteinhartâHart_equation
    * 3_B_or_Î²_parameter_equation
    * 4_Conduction_model
          o 4.1_NTC_(negative_temperature_coefficient)
          o 4.2_PTC_(positive_temperature_coefficient)
    * 5_Self-heating_effects
    * 6_Applications
          o 6.1_PTC
          o 6.2_NTC
    * 7_History
    * 8_See_also
    * 9_References
    * 10_External_links
***** Basic operation[edit] *****
Assuming, as a first-order approximation, that the relationship between
resistance and temperature is linear, then
         &#x0394; R = k &#x0394; T ,   {\displaystyle \Delta R=k\Delta T,}  [
      {\displaystyle \Delta R=k\Delta T,}]
where
         &#x0394; R   {\displaystyle \Delta R}  [\Delta R], change in
      resistance,
         &#x0394; T   {\displaystyle \Delta T}  [\Delta T], change in
      temperature,
         k   {\displaystyle k}  [k], first-order temperature_coefficient_of
      resistance.
Thermistors can be classified into two types, depending on the sign of     k
{\displaystyle k}  [k]. If     k   {\displaystyle k}  [k] is positive, the
resistance increases with increasing temperature, and the device is called a
positive_temperature_coefficient (PTC) thermistor, or posistor. If     k
{\displaystyle k}  [k] is negative, the resistance decreases with increasing
temperature, and the device is called a negative_temperature_coefficient (NTC)
thermistor. Resistors that are not thermistors are designed to have a     k
{\displaystyle k}  [k] as close to 0 as possible, so that their resistance
remains nearly constant over a wide temperature range.
Instead of the temperature coefficient k, sometimes the temperature coefficient
of resistance      &#x03B1;  T     {\displaystyle \alpha _{T}}  [\alpha _{T}]
("alpha sub T") is used. It is defined as[4]
          &#x03B1;  T   =   1  R ( T )       d R   d T    .   {\displaystyle
      \alpha _{T}={\frac {1}{R(T)}}{\frac {dR}{dT}}.}  [\alpha _{T}={\frac  {1}
      {R(T)}}{\frac  {dR}{dT}}.]
This      &#x03B1;  T     {\displaystyle \alpha _{T}}  [\alpha _{T}]
coefficient should not be confused with the     a   {\displaystyle a}  [a]
parameter below.
***** SteinhartâHart equation[edit] *****
Main article: SteinhartâHart_equation
In practical devices, the linear approximation model (above) is accurate only
over a limited temperature range. Over wider temperature ranges, a more complex
resistanceâtemperature transfer_function provides a more faithful
characterization of the performance. The SteinhartâHart_equation is a widely
used third-order approximation:
           1 T   = a + b ln &#x2061; R + c  ( ln &#x2061; R  )  3   ,
      {\displaystyle {\frac {1}{T}}=a+b\ln R+c\,(\ln R)^{3},}  [{\displaystyle
      {\frac {1}{T}}=a+b\ln R+c\,(\ln R)^{3},}]
where a, b and c are called the SteinhartâHart parameters and must be
specified for each device. T is the absolute_temperature, and R is the
resistance. To give resistance as a function of temperature, the above can be
rearranged into
         R = exp &#x2061;  [  ( x &#x2212; y  )  1  /  3   &#x2212; ( x + y  )
      1  /  3    ]  ,   {\displaystyle R=\exp \left[(x-y)^{1/3}-(x+y)^{1/
      3}\right],}  [{\displaystyle R=\exp \left[(x-y)^{1/3}-(x+y)^{1/
      3}\right],}]
where
             y    =   1  2 c     (  a &#x2212;   1 T    )  ,     x    =
      (   b  3 c    )   3   +  y  2     .       {\displaystyle {\begin
      {aligned}y&={\frac {1}{2c}}\left(a-{\frac {1}{T}}\right),\\x&={\sqrt
      {\left({\frac {b}{3c}}\right)^{3}+y^{2}}}.\end{aligned}}}  [
      {\displaystyle {\begin{aligned}y&={\frac {1}{2c}}\left(a-{\frac {1}
      {T}}\right),\\x&={\sqrt {\left({\frac {b}{3c}}\right)^{3}+y^{2}}}.\end
      {aligned}}}]
The error in the SteinhartâHart equation is generally less than 0.02 Â°C in
the measurement of temperature over a 200 Â°C range.[5] As an example, typical
values for a thermistor with a resistance of 3 kÎ© at room temperature (25 Â°C
= 298.15 K) are:
             a    = 1.40 &#x00D7;  10  &#x2212; 3   ,     b    = 2.37 &#x00D7;
      10  &#x2212; 4   ,     c    = 9.90 &#x00D7;  10  &#x2212; 8   .
      {\displaystyle {\begin{aligned}a&=1.40\times 10^{-3},\\b&=2.37\times 10^
      {-4},\\c&=9.90\times 10^{-8}.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}a&=1.40\times 10^{-3},\\b&=2.37\times 10^{-4},\\c&=9.90\times
      10^{-8}.\end{aligned}}}]
***** B or Î² parameter equation[edit] *****
NTC thermistors can also be characterised with the B (or Î²) parameter
equation, which is essentially the SteinhartâHart_equation with     a = 1  /
T  0   &#x2212; ( 1  /  B ) ln &#x2061;  R  0     {\displaystyle a=1/T_{0}-(1/
B)\ln R_{0}}  [{\displaystyle a=1/T_{0}-(1/B)\ln R_{0}}],     b = 1  /  B
{\displaystyle b=1/B}  [b=1/B] and     c = 0   {\displaystyle c=0}  [c=0],
           1 T   =   1  T  0     +   1 B   ln &#x2061;   R  R  0     ,
      {\displaystyle {\frac {1}{T}}={\frac {1}{T_{0}}}+{\frac {1}{B}}\ln {\frac
      {R}{R_{0}}},}  [{\displaystyle {\frac {1}{T}}={\frac {1}{T_{0}}}+{\frac
      {1}{B}}\ln {\frac {R}{R_{0}}},}]
where the temperatures are in kelvins, and R0 is the resistance at temperature
T0 (25 Â°C = 298.15 K). Solving for R yields
         R =  R  0    e  B  (    1 T   &#x2212;   1  T  0      )
      {\displaystyle R=R_{0}e^{B\left({\frac {1}{T}}-{\frac {1}{T_
      {0}}}\right)}}  [{\displaystyle R=R_{0}e^{B\left({\frac {1}{T}}-{\frac
      {1}{T_{0}}}\right)}}]
or, alternatively,
         R =  r  &#x221E;    e  B  /  T   ,   {\displaystyle R=r_{\infty }e^{B/
      T},}  [{\displaystyle R=r_{\infty }e^{B/T},}]
where      r  &#x221E;   =  R  0    e  &#x2212; B  /   T  0
{\displaystyle r_{\infty }=R_{0}e^{-B/T_{0}}}  [{\displaystyle r_{\infty }=R_
{0}e^{-B/T_{0}}}].
This can be solved for the temperature:
         T =   B  ln &#x2061; ( R  /   r  &#x221E;   )    .   {\displaystyle T=
      {\frac {B}{\ln(R/r_{\infty })}}.}  [{\displaystyle T={\frac {B}{\ln(R/r_
      {\infty })}}.}]
The B-parameter equation can also be written as     ln &#x2061; R = B  /  T +
ln &#x2061;  r  &#x221E;     {\displaystyle \ln R=B/T+\ln r_{\infty }}  [
{\displaystyle \ln R=B/T+\ln r_{\infty }}]. This can be used to convert the
function of resistance vs. temperature of a thermistor into a linear function
of     ln &#x2061; R   {\displaystyle \ln R}  [\ln R] vs.     1  /  T
{\displaystyle 1/T}  [1/T]. The average slope of this function will then yield
an estimate of the value of the B parameter.
***** Conduction model[edit] *****
**** NTC (negative temperature coefficient)[edit] ****
A failed (blown) NTC thermistor that worked as an inrush current limiter in a
switched-mode_power_supply
Many NTC thermistors are made from a pressed disc, rod, plate, bead or cast
chip of semiconducting material such as sintered metal oxides. They work
because raising the temperature of a semiconductor increases the number of
active charge_carriers[6] it promotes them into the conduction_band. The more
charge carriers that are available, the more current a material can conduct. In
certain materials like ferric oxide (Fe2O3) with titanium (Ti) doping an n-type
semiconductor is formed and the charge carriers are electrons. In materials
such as nickel oxide (NiO) with lithium (Li) doping a p-type semiconductor is
created, where holes are the charge carriers.[7]
This is described in the formula
         I = n &#x22C5; A &#x22C5; v &#x22C5; e ,   {\displaystyle I=n\cdot
      A\cdot v\cdot e,}  [{\displaystyle I=n\cdot A\cdot v\cdot e,}]
where
         I   {\displaystyle I}  [I] = electric current (amperes),
         n   {\displaystyle n}  [n] = density of charge carriers (count/m3),
         A   {\displaystyle A}  [A] = cross-sectional area of the material
      (m2),
         v   {\displaystyle v}  [v] = drift velocity of electrons (m/s),
         e   {\displaystyle e}  [e] = charge of an electron (    e = 1.602
      &#x00D7;  10  &#x2212; 19     {\displaystyle e=1.602\times 10^{-19}}  [
      {\displaystyle e=1.602\times 10^{-19}}] coulomb).
Over large changes in temperature, calibration is necessary. Over small changes
in temperature, if the right semiconductor is used, the resistance of the
material is linearly proportional to the temperature. There are many different
semiconducting thermistors with a range from about 0.01 kelvin to 2,000 kelvins
(â273.14 Â°C to 1,700 Â°C).[citation_needed]
The IEC standard symbol for a NTC thermistor includes a "âtÂ°" under the
rectangle.[8]
**** PTC (positive temperature coefficient)[edit] ****
Most PTC thermistors are made from doped polycrystalline ceramic (containing
barium_titanate (BaTiO3) and other compounds) which have the property that
their resistance rises suddenly at a certain critical temperature. Barium
titanate is ferroelectric and its dielectric_constant varies with temperature.
Below the Curie_point temperature, the high dielectric_constant prevents the
formation of potential barriers between the crystal grains, leading to a low
resistance. In this region the device has a small negative temperature
coefficient. At the Curie point temperature, the dielectric constant drops
sufficiently to allow the formation of potential barriers at the grain
boundaries, and the resistance increases sharply with temperature. At even
higher temperatures, the material reverts to NTC behaviour.
Another type of thermistor is a silistor, a thermally sensitive silicon
resistor. Silistors employ silicon as the semiconductive component material.
Unlike ceramic PTC thermistors, silistors have an almost linear resistance-
temperature characteristic.[9]
Barium titanate thermistors can be used as self-controlled heaters; for a given
voltage, the ceramic will heat to a certain temperature, but the power used
will depend on the heat loss from the ceramic.
The dynamics of PTC thermistors being powered also is extremely useful. When
first connected to a voltage source, a large current corresponding to the low,
cold, resistance flows, but as the thermistor self-heats, the current is
reduced until a limiting current (and corresponding peak device temperature) is
reached. The current-limiting effect can replace fuses. In the degaussing
circuits of many CRT monitors and televisions an appropriately chosen
thermistor is connected in series with the degaussing coil. This results in a
smooth current decrease for an improved degaussing effect. Some of these
degaussing circuits have auxiliary heating elements to heat the thermistor (and
reduce the resulting current) further.
Another type of PTC thermistor is the polymer PTC, which is sold under brand
names such as "Polyswitch" "Semifuse", and "Multifuse". This consists of
plastic with carbon grains embedded in it. When the plastic is cool, the carbon
grains are all in contact with each other, forming a conductive path through
the device. When the plastic heats up, it expands, forcing the carbon grains
apart, and causing the resistance of the device to rise, which then causes
increased heating and rapid resistance increase. Like the BaTiO3 thermistor,
this device has a highly nonlinear resistance/temperature response useful for
thermal or circuit control, not for temperature measurement. Besides circuit
elements used to limit current, self-limiting heaters can be made in the form
of wires or strips, useful for heat_tracing. PTC thermistors 'latch' into a hot
/ high resistance state: once hot, they stay in that high resistance state,
until cooled. The effect can be used as a primitive latch/memory_circuit, the
effect being enhanced by using two PTC thermistors in series, with one
thermistor cool, and the other thermistor hot.[10]
The IEC standard symbol for a PTC thermistor includes a "+tÂ°" under the
rectangle.[11]
***** Self-heating effects[edit] *****
When a current flows through a thermistor, it generates heat, which raises the
temperature of the thermistor above that of its environment. If the thermistor
is being used to measure the temperature of the environment, this electrical
heating may introduce a significant error if a correction is not made.
Alternatively, this effect itself can be exploited. It can, for example, make a
sensitive air-flow device employed in a sailplane rate-of-climb instrument, the
electronic variometer, or serve as a timer for a relay as was formerly done in
telephone_exchanges.
The electrical power input to the thermistor is just
          P  E   = I V ,   {\displaystyle P_{E}=IV,}  [{\displaystyle P_
      {E}=IV,}]
where I is current, and V is the voltage drop across the thermistor. This power
is converted to heat, and this heat energy is transferred to the surrounding
environment. The rate of transfer is well described by Newton's_law_of_cooling:
          P  T   = K ( T ( R ) &#x2212;  T  0   ) ,   {\displaystyle P_{T}=K(T
      (R)-T_{0}),}  [{\displaystyle P_{T}=K(T(R)-T_{0}),}]
where T(R) is the temperature of the thermistor as a function of its resistance
R,      T  0     {\displaystyle T_{0}}  [T_{0}] is the temperature of the
surroundings, and K is the dissipation constant, usually expressed in units of
milliwatts per degree Celsius. At equilibrium, the two rates must be equal:
          P  E   =  P  T   .   {\displaystyle P_{E}=P_{T}.}  [{\displaystyle P_
      {E}=P_{T}.}]
The current and voltage across the thermistor depend on the particular circuit
configuration. As a simple example, if the voltage across the thermistor is
held fixed, then by Ohm's_law we have     I = V  /  R   {\displaystyle I=V/R}
[I=V/R], and the equilibrium equation can be solved for the ambient temperature
as a function of the measured resistance of the thermistor:
          T  0   = T ( R ) &#x2212;    V  2    K R    .   {\displaystyle T_
      {0}=T(R)-{\frac {V^{2}}{KR}}.}  [{\displaystyle T_{0}=T(R)-{\frac {V^{2}}
      {KR}}.}]
The dissipation constant is a measure of the thermal connection of the
thermistor to its surroundings. It is generally given for the thermistor in
still air and in well-stirred oil. Typical values for a small glass-bead
thermistor are 1.5 mW/Â°C in still air and 6.0 mW/Â°C in stirred oil. If the
temperature of the environment is known beforehand, then a thermistor may be
used to measure the value of the dissipation constant. For example, the
thermistor may be used as a flow-rate sensor, since the dissipation constant
increases with the rate of flow of a fluid past the thermistor.
The power dissipated in a thermistor is typically maintained at a very low
level to ensure insignificant temperature measurement error due to self-
heating. However, some thermistor applications depend upon significant "self-
heating" to raise the body temperature of the thermistor well above the ambient
temperature, so the sensor then detects even subtle changes in the thermal
conductivity of the environment. Some of these applications include liquid-
level detection, liquid-flow measurement and air-flow measurement.[4]
***** Applications[edit] *****
**** PTC[edit] ****
    * As current-limiting devices for circuit protection, as replacements for
      fuses. Current through the device causes a small amount of resistive
      heating. If the current is large enough to generate more heat than the
      device can lose to its surroundings, the device heats up, causing its
      resistance to increase. This creates a self-reinforcing effect that
      drives the resistance upwards, therefore limiting the current.
    * As timers in the degaussing_coil circuit of most CRT displays. When the
      display unit is initially switched on, current flows through the
      thermistor and degaussing coil. The coil and thermistor are intentionally
      sized so that the current flow will heat the thermistor to the point that
      the degaussing coil shuts off in under a second. For effective
      degaussing, it is necessary that the magnitude of the alternating
      magnetic field produced by the degaussing coil decreases smoothly and
      continuously, rather than sharply switching off or decreasing in steps;
      the PTC thermistor accomplishes this naturally as it heats up. A
      degaussing circuit using a PTC thermistor is simple, reliable (for its
      simplicity), and inexpensive.
    * As heater in automotive industry to provide additional heat inside cabin
      with diesel engine or to heat diesel in cold climatic conditions before
      engine injection.
    * In temperature compensated synthesizer voltage controlled oscillators.
      [12]
    * In lithium_battery protection circuits.[13]
    * In an electrically actuated Wax_motor to provide the heat necessary to
      expand the wax.
    * Many electric motors and dry type power transformers incorporate PTC
      thermistors in their windings. When used in conjunction with a monitoring
      relay they provide overtemperature protection to prevent insulation
      damage. The equipment manufacturer selects a thermistor with a highly
      non-linear response curve where resistance increases dramatically at the
      maximum allowable winding temperature, causing the relay to operate.
**** NTC[edit] ****
    * As a resistance_thermometer for low-temperature measurements of the order
      of 10 K.
    * As an inrush_current_limiter device in power supply circuits, they
      present a higher resistance initially, which prevents large currents from
      flowing at turn-on, and then heat up and become much lower resistance to
      allow higher current flow during normal operation. These thermistors are
      usually much larger than measuring type thermistors, and are purposely
      designed for this application.[14]
    * As sensors in automotive applications to monitor fluid temperatures like
      the engine coolant, cabin air, external air or engine oil temperature,
      and feed the relative readings to control units like the ECU and to the
      dashboard.
    * To monitor the temperature of an incubator.
    * Thermistors are also commonly used in modern digital_thermostats and to
      monitor the temperature of battery packs while charging.
    * Thermistors are often used in the hot ends of 3D_printers; they monitor
      the heat produced and allow the printer's control circuitry to keep a
      constant temperature for melting the plastic filament.
    * In the food handling and processing industry, especially for food storage
      systems and food preparation. Maintaining the correct temperature is
      critical to prevent foodborne_illness.
    * Throughout the consumer appliance industry for measuring temperature.
      Toasters, coffee makers, refrigerators, freezers, hair dryers, etc. all
      rely on thermistors for proper temperature control.
    * NTC thermistors come in bare and lugged forms, the former is for point
      sensing to achieve high accuracy for specific points, such as laser diode
      die, etc.[15]
    * For measurement of temperature profile inside the sealed cavity of a
      convective (thermal) inertial_sensor[16].
    * Thermistor Probe Assemblies [17] offer protection of the sensor in harsh
      environments.  The thermistor sensing element can be packaged into a
      variety of enclosures for use in industries such as HVAC/R, Building
      Automation, Pool/Spa, Energy and Industrial Electronics. Enclosures can
      be made out of stainless steel, aluminum, copper brass or plastic and
      configurations include threaded (NPT, etc), flanged (with mounting holes
      for ease of installation) and straight (flat tip, pointed tip, radius
      tip, etc.). Thermistor probe assemblies are very rugged and are highly
      customizable to fit the application needs. Probe assemblies have gained
      in popularity over the years as improvements in research, engineering and
      manufacturing techniques have been made.
***** History[edit] *****
The first NTC thermistor was discovered in 1833 by Michael_Faraday, who
reported on the semiconducting behavior of silver_sulfide. Faraday noticed that
the resistance of silver sulfide decreased dramatically as temperature
increased. (This was also the first documented observation of a semiconducting
material.)[18]
Because early thermistors were difficult to produce and applications for the
technology were limited, commercial production of thermistors did not begin
until the 1930s.[19] A commercially viable thermistor was invented by Samuel
Ruben in 1930.[20]
***** See also[edit] *****
    * Iron-hydrogen_resistor
    * Stretch_sensor
    * Thermocouple
***** References[edit] *****
   1. ^"What_is_a_Thermistor?_How_do_thermistors_work?". EI Sensor
      Technologies. Retrieved 2019-05-13.
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
   3. ^"Thermistors". EI Sensor Technologies. Retrieved 2019-05-13.
   4. ^ "NTC_Thermistors". Micro-chip Technologies. 2010.
   5. ^ a b Thermistor_Terminology. U.S. Sensor.
   6. ^ "Practical_Temperature_Measurements". Agilent Application Note. Agilent
      Semiconductor.
   7. ^ [[#CITEREF|]].
   8. ^L. W Turner, ed. (1976). Electronics Engineer's Reference Book (4 ed.).
      Butterworths. pp. 6-29 to 6-41. ISBN 0408001682.
   9. ^"NTC_thermistor Â»_Resistor_Guide".
  10. ^ "PTC_Thermistors_and_Silistors" The Resistor Guide
  11. ^ Downie, Neil A., The Ultimate Book of Saturday Science (Princeton 2012)
  12. ISBN 0-691-14966-6
  13. ^ "PTC_thermistor_-_Positive_Temperature_Coefficient". Resistor Guide.
  14. ^Patchell, Jim. "Temperature_Compensated_VCO". www.oldcrows.net.
  15. ^ Patent CN 1273423A (China)
  16. ^ Inrush_Current_Limiting_Power_Thermistors. U.S. Sensor
  17. ^"PTC_Thermistors_Guide-_"Publish_By_Analog_Electronic_Technologies"".
  18. ^Mukherjee, Rahul; Basu, Joydeep; Mandal, Pradip; Guha, Prasanta Kumar.
      "A_review_of_micromachined_thermal_accelerometers". Journal of
      Micromechanics and Microengineering. 27 (12). arXiv:1801.07297. Bibcode:
      2017JMiMi..27l3002M. doi:10.1088/1361-6439/aa964d.
  19. ^"Thermistor_Probes". EI Sensor Technologies. Retrieved 2019-05-13.
  20. ^"1833_-_First_Semiconductor_Effect_is_Recorded". Computer History
      Museum. Retrieved 24 June 2014.
  21. ^McGee, Thomas (1988). "Chapter 9". Principles_and_Methods_of_Temperature
      Measurement. John Wiley & Sons. p. 203.
  22. ^Jones, Deric P., ed. (2009). Biomedical_Sensors. Momentum Press. p. 12.
***** External links[edit] *****
 Wikimedia Commons has media related to Thermistors.
    * The_thermistor_at_bucknell.edu
    * Software_for_thermistor_calculation_at_Sourceforge
    * "Thermistors_&_Thermocouples:Matching_the_Tool_to_the_Task_in_Thermal
      Validation" - Journal of Validation Technology
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
                                         * Zener_diode
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
    * v
    * t
    * e
Sensors
                         * Geophone
Acoustic, sound,         * Hydrophone
vibration                * Microphone
                         * Seismometer
                         * Airâfuel_ratio_meter
                         * Blind_spot_monitor
                         * Crankshaft_position_sensor
                         * Curb_feeler
                         * Defect_detector
                         * Engine_coolant_temperature_sensor
                         * Hall_effect_sensor
                         * MAP_sensor
                         * Mass_flow_sensor
                         * Omniview_technology
                         * Oxygen_sensor
Automotive,              * Parking_sensors
transportation           * Radar_gun
                         * Speed_sensor
                         * Speedometer
                         * Throttle_position_sensor
                         * Tire-pressure_monitoring_system
                         * Torque_sensor
                         * Transmission_fluid_temperature_sensor
                         * Turbine_speed_sensor
                         * Variable_reluctance_sensor
                         * Vehicle_speed_sensor
                         * Water_sensor
                         * Wheel_speed_sensor
                         * Breathalyzer
                         * Carbon_dioxide_sensor
                         * Carbon_monoxide_detector
                         * Catalytic_bead_sensor
                         * Chemical_field-effect_transistor
                         * Electrochemical_gas_sensor
                         * Electrolyteâinsulatorâsemiconductor_sensor
                         * Electronic_nose
                         * Fluorescent_chloride_sensors
                         * Holographic_sensor
                         * Hydrocarbon_dew_point analyzer
                         * Hydrogen_sensor
                         * Hydrogen_sulfide_sensor
Chemical                 * Infrared_point_sensor
                         * Ion_selective_electrode
                         * Microwave_chemistry_sensor
                         * Nitrogen_oxide_sensor
                         * Nondispersive_infrared_sensor
                         * Olfactometer
                         * Optode
                         * Oxygen_sensor
                         * Pellistor
                         * pH_glass_electrode
                         * Potentiometric_sensor
                         * Redox_electrode
                         * Smoke_detector
                         * Zinc_oxide_nanorod_sensor
                         * Current_sensor
                         * Electroscope
                         * Galvanometer
                         * Hall_effect_sensor
                         * Hall_probe
Electric, magnetic,      * Magnetic_anomaly_detector
radio                    * Magnetometer
                         * MEMS_magnetic_field_sensor
                         * Metal_detector
                         * Planar_Hall_sensor
                         * Radio_direction_finder
                         * Test_light
                         * Actinometer
                         * Bedwetting_alarm
                         * Ceilometer
                         * Dew_warning
                         * Electrochemical_gas_sensor
                         * Fish_counter
                         * Frequency_domain_sensor
                         * Gas_detector
                         * Hook_gauge_evaporimeter
                         * Humistor
Environment,             * Hygrometer
weather,                 * Leaf_sensor
moisture                 * Psychrometer
                         * Pyranometer
                         * Pyrgeometer
                         * Rain_gauge
                         * Rain_sensor
                         * SNOTEL
                         * Snow_gauge
                         * Soil_moisture_sensor
                         * Stream_gauge
                         * Tide_gauge
                         * Weather_radar
                         * Air_flow_meter
                         * Anemometer
Flow, fluid velocity     * Flow_sensor
                         * Gas_meter
                         * Mass_flow_sensor
                         * Water_metering
                         * Bubble_chamber
                         * Cloud_chamber
                         * GeigerâMÃ¼ller_tube
                         * Geiger_counter
                         * Ionization_chamber
Ionising radiation,      * Neutron_detection
subatomic particles      * Particle_detector
                         * Proportional_counter
                         * Scintillation_counter
                         * Semiconductor_detector
                         * Scintillator
                         * Thermoluminescent_dosimeter
                         * Wire_chamber
                         * Airspeed_indicator
                         * Machmeter
                         * Altimeter
                         * Attitude_indicator
                         * Depth_gauge
                         * Fluxgate_compass
                         * Gyroscope
Navigation               * Inertial_navigation_system
instruments              * Inertial_reference_unit
                         * Magnetic_compass
                         * MHD_sensor
                         * Ring_laser_gyroscope
                         * Turn_coordinator
                         * Variometer
                         * Vibrating_structure_gyroscope
                         * Yaw-rate_sensor
                         * Accelerometer
                         * Angular_rate_sensor
                         * Auxanometer
                         * Capacitive_displacement_sensor
                         * Capacitive_sensing
                         * Gravimeter
                         * Inclinometer
                         * Integrated_circuit_piezoelectric_sensor
                         * Laser_rangefinder
                         * Laser_surface_velocimeter
                         * Lidar
                         * Linear_encoder
Position, angle,         * Linear_variable_differential_transformer
displacement             * Liquid_capacitive_inclinometers
                         * Odometer
                         * Photoelectric_sensor
                         * Piezoelectric_accelerometer
                         * Position_sensor
                         * Rotary_encoder
                         * Rotary_variable_differential_transformer
                         * Selsyn
                         * Sudden_Motion_Sensor
                         * Tachometer
                         * Tilt_sensor
                         * Ultrasonic_thickness_gauge
                         * Variable_reluctance_sensor
                         * Velocity_receiver
                         * Active_pixel_sensor
                         * Angleâsensitive_pixel
                         * Back-illuminated_sensor
                         * Charge-coupled_device
                         * Contact_image_sensor
                         * Electro-optical_sensor
                         * Flame_detector
                         * Infrared
                         * Kinetic_inductance_detector
                         * LED_as_light_sensor
                         * Light-addressable_potentiometric_sensor
                         * Nichols_radiometer
                         * Optical_fiber
                         * Photodetector
Optical, light,          * Photodiode
imaging                  * Photoelectric_sensor
                         * Photoionization_detector
                         * Photomultiplier
                         * Photoresistor
                         * Photoswitch
                         * Phototransistor
                         * Phototube
                         * Position_sensitive_device
                         * Scintillometer
                         * ShackâHartmann_wavefront_sensor
                         * Single-photon_avalanche_diode
                         * Superconducting_nanowire_single-photon_detector
                         * Transition_edge_sensor
                         * Tristimulus_colorimeter
                         * Visible-light_photon_counter
                         * Wavefront_sensor
                         * Barograph
                         * Barometer
                         * Boost_gauge
                         * Bourdon_gauge
                         * Hot-filament_ionization_gauge
                         * Ionization_gauge
                         * McLeod_gauge
Pressure                 * Oscillating_U-tube
                         * Permanent_Downhole_Gauge
                         * Piezometer
                         * Pirani_gauge
                         * Pressure_gauge
                         * Pressure_sensor
                         * Tactile_sensor
                         * Time_pressure_gauge
                         * Bhangmeter
                         * Force_gauge
                         * Hydrometer
                         * Level_sensor
Force, density,          * Load_cell
level                    * Magnetic_level_gauge
                         * Nuclear_density_gauge
                         * Piezoelectric_sensor
                         * Strain_gauge
                         * Torque_sensor
                         * Viscometer
                         * Bimetallic_strip
                         * Bolometer
                         * Calorimeter
                         * Exhaust_gas_temperature_gauge
                         * Flame_detection
                         * Gardon_gauge
                         * Golay_cell
                         * Heat_flux_sensor
Thermal, heat,           * Infrared_thermometer
temperature              * Microbolometer
                         * Microwave_radiometer
                         * Net_radiometer
                         * Quartz_thermometer
                         * Resistance_thermometer
                         * Silicon_bandgap_temperature_sensor
                         * Special_sensor_microwave/imager
                         * Thermistor
                         * Thermocouple
                         * Thermometer
                         * Alarm_sensor
                         * Doppler_radar
                         * Motion_detector
                         * Occupancy_sensor
                         * Passive_infrared_sensor
Proximity, presence      * Proximity_sensor
                         * Reed_switch
                         * Stud_finder
                         * Touch_switch
                         * Triangulation_sensor
                         * Wired_glove
                         * Active_pixel_sensor
                         * Back-illuminated_sensor
                         * Biochip
                         * Biosensor
                         * Capacitance_probe
                         * Carbon_paste_electrode
                         * Catadioptric_sensor
                         * Digital_sensors
                         * Displacement_receiver
                         * Electromechanical_film
                         * Electro-optical_sensor
                         * FabryâPÃ©rot_interferometer
                         * Fisheries_acoustics
                         * Image_sensor
                         * Image_sensor_format
                         * Inductive_sensor
                         * Intelligent_sensor
                         * Lab-on-a-chip
                         * Leaf_sensor
Sensor technology        * Machine_vision
                         * Microelectromechanical_systems
                         * Photoelasticity
                         * Quantum_sensor
                         * Radar
                               o Ground-penetrating_radar
                               o Synthetic_aperture_radar
                         * Radar_tracker
                         * Sensor_array
                         * Sensor_fusion
                         * Sensor_grid
                         * Sensor_node
                         * Soft_sensor
                         * Sonar
                         * Staring_array
                         * Transducer
                         * Ultrasonic_sensor
                         * Video_sensor_technology
                         * Visual_sensor_network
                         * Wheatstone_bridge
                         * Wireless_sensor_network
Related                  * List_of_sensors
Authority_control [Edit_this_at_Wikidata]     * GND: 4128535-9
                                              * NDL: 00570083

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Thermistor&oldid=907483533"
Categories:
    * Heating,_ventilating,_and_air_conditioning
    * Resistive_components
    * Sensors
    * Thermometers
Hidden categories:
    * Pages_using_deprecated_image_syntax
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_May_2013
    * Commons_category_link_is_on_Wikidata
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * à¦¬à¦¾à¦à¦²à¦¾
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
    * Gaeilge
    * Galego
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à°¤à±à°²à±à°à±
    * à¹à¸à¸¢
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 23 July 2019, at 06:44 (UTC).
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
