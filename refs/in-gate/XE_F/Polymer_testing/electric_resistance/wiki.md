The following text has been accessed from https://en.wikipedia.org/wiki/Electrical_resistance_and_conductance at Fri Aug 9 03:02:58 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Electrical resistance and conductance ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about specific applications of conductivity and resistivity in
electrical elements. For other types of conductivity, see Conductivity. For
electrical conductivity in general, see Electrical_resistivity_and
conductivity.
"Resistive" redirects here. For the term used when referring to touchscreens,
see resistive_touchscreen.
Part of a series of articles about
Electromagnetism
[Solenoid]
    * Electricity
    * Magnetism
Electrostatics
    * Conductor
    * Coulomb's_law
    * Electric_charge
    * Electric_dipole_moment
    * Electric_field
    * Electric_flux / potential_energy
    * Electrostatic_discharge
    * Gauss's_law
    * Induction
    * Insulator
    * Polarization_density
    * Static_electricity
    * Triboelectricity
Magnetostatics
    * AmpÃ¨re's_law
    * BiotâSavart_law
    * Gauss's_law_for_magnetism
    * Magnetic_field
    * Magnetic_flux
    * Magnetic_dipole_moment
    * Magnetization
    * Magnetomotive_force
Electrodynamics
    * Lorentz_force_law
    * Electromagnetic_induction
    * Faraday's_law
    * Lenz's_law
    * Displacement_current
    * Magnetic_potential
    * Maxwell's_equations
    * Electromagnetic_field
    * Electromagnetic_pulse
    * Electromagnetic_radiation
    * Maxwell_tensor
    * Poynting_vector
    * LiÃ©nardâWiechert_potential
    * Jefimenko's_equations
    * Eddy_current
    * London_equations
    * Mathematical_descriptions_of_the_electromagnetic_field
Electrical_network
    * Alternating_current
    * Capacitance
    * Direct_current
    * Electric_current
    * Electric_potential
    * Electromotive_force
    * Impedance
    * Inductance
    * Ohm's_law
    * Parallel_circuit
    * Resistance
    * Resonant_cavities
    * Series_circuit
    * Voltage
    * Waveguides
Covariant_formulation
    * Electromagnetic_tensor
      (stressâenergy_tensor)
    * Four-current
    * Electromagnetic_four-potential
Scientists
    * AmpÃ¨re
    * Biot
    * Coulomb
    * Faraday
    * Gauss
    * Heaviside
    * Henry
    * Hertz
    * Lenz
    * Lorentz
    * Maxwell
    * Ãrsted
    * Savart
    * Tesla
    * Volta
    * Weber
    * v
    * t
    * e
The electrical resistance of an object is a measure of its opposition to the
flow of electric current. The inverse quantity is electrical conductance, and
is the ease with which an electric current passes. Electrical resistance shares
some conceptual parallels with the notion of mechanical friction. The SI unit
of electrical resistance is the ohm (Î©), while electrical conductance is
measured in siemens (S).
The resistance of an object depends in large part on the material it is made
ofâobjects made of electrical_insulators like rubber tend to have very high
resistance and low conductivity, while objects made of electrical_conductors
like metals tend to have very low resistance and high conductivity. This
material dependence is quantified by resistivity_or_conductivity. However,
resistance and conductance are extensive_rather_than_bulk_properties, meaning
that they also depend on the size and shape of an object. For example, a wire's
resistance is higher if it is long and thin, and lower if it is short and
thick. All objects show some resistance, except for superconductors, which have
a resistance of zero.
The resistance (R) of an object is defined as the ratio of voltage across it
(V) to current through it (I), while the conductance (G) is the inverse:
         R =   V I   ,  G =   I V   =   1 R     {\displaystyle R={V \over
      I},\qquad G={I \over V}={\frac {1}{R}}}  [R = {V\over I}, \qquad G =
      {I\over V} = \frac{1}{R}]
For a wide variety of materials and conditions, V and I are directly
proportional to each other, and therefore R and G are constants (although they
will depend on the size and shape of the object, the material it is made of,
and other factors like temperature or strain). This proportionality is called
Ohm's_law, and materials that satisfy it are called ohmic materials.
In other cases, such as a transformer, diode or battery, V and I are not
directly proportional. The ratio V/I is sometimes still useful, and is referred
to as a "chordal resistance" or "static resistance",[1][2] since it corresponds
to the inverse slope of a chord between the origin and an IâV_curve. In other
situations, the derivative        d V   d I        {\displaystyle {\frac {dV}
{dI}}\,\!}  [ \frac{dV}{dI} \,\!] may be most useful; this is called the
"differential resistance".
⁰
***** Contents *****
    * 1_Introduction
    * 2_Conductors_and_resistors
    * 3_Ohm's_law
    * 4_Relation_to_resistivity_and_conductivity
    * 5_Measuring_resistance
    * 6_Typical_resistances
    * 7_Static_and_differential_resistance
    * 8_AC_circuits
          o 8.1_Impedance_and_admittance
          o 8.2_Frequency_dependence_of_resistance
    * 9_Energy_dissipation_and_Joule_heating
    * 10_Dependence_of_resistance_on_other_conditions
          o 10.1_Temperature_dependence
          o 10.2_Strain_dependence
          o 10.3_Light_illumination_dependence
    * 11_Superconductivity
    * 12_See_also
    * 13_References
    * 14_External_links
***** Introduction[edit] *****
The hydraulic_analogy compares electric current flowing through circuits to
water flowing through pipes. When a pipe (left) is filled with hair (right), it
takes a larger pressure to achieve the same flow of water. Pushing electric
current through a large resistance is like pushing water through a pipe clogged
with hair: It requires a larger push (electromotive_force) to drive the same
flow (electric_current).
In the hydraulic_analogy, current flowing through a wire (or resistor) is like
water flowing through a pipe, and the voltage_drop across the wire is like the
pressure_drop that pushes water through the pipe. Conductance is proportional
to how much flow occurs for a given pressure, and resistance is proportional to
how much pressure is required to achieve a given flow. (Conductance and
resistance are reciprocals.)
The voltage_drop (i.e., difference between voltages on one side of the resistor
and the other), not the voltage itself, provides the driving force pushing
current through a resistor. In hydraulics, it is similar: The pressure
difference between two sides of a pipe, not the pressure itself, determines the
flow through it. For example, there may be a large water pressure above the
pipe, which tries to push water down through the pipe. But there may be an
equally large water pressure below the pipe, which tries to push water back up
through the pipe. If these pressures are equal, no water flows. (In the image
at right, the water pressure below the pipe is zero.)
The resistance and conductance of a wire, resistor, or other element is mostly
determined by two properties:
    * geometry (shape), and
    * material
Geometry is important because it is more difficult to push water through a
long, narrow pipe than a wide, short pipe. In the same way, a long, thin copper
wire has higher resistance (lower conductance) than a short, thick copper wire.
Materials are important as well. A pipe filled with hair restricts the flow of
water more than a clean pipe of the same shape and size. Similarly, electrons
can flow freely and easily through a copper wire, but cannot flow as easily
through a steel wire of the same shape and size, and they essentially cannot
flow at all through an insulator like rubber, regardless of its shape. The
difference between copper, steel, and rubber is related to their microscopic
structure and electron_configuration, and is quantified by a property called
resistivity.
In addition to geometry and material, there are various other factors that
influence resistance and conductance, such as temperature; see below.
***** Conductors and resistors[edit] *****
A 6.5 MÎ© resistor, as identified by its electronic_color_code
(blueâgreenâblack-yellow-red). An ohmmeter could be used to verify this
value.
Substances in which electricity can flow are called conductors. A piece of
conducting material of a particular resistance meant for use in a circuit is
called a resistor. Conductors are made of high-conductivity materials such as
metals, in particular copper and aluminium. Resistors, on the other hand, are
made of a wide variety of materials depending on factors such as the desired
resistance, amount of energy that it needs to dissipate, precision, and costs.
***** Ohm's law[edit] *****
Main article: Ohm's_law
The current-voltage_characteristics of four devices: Two resistors, a diode,
and a battery. The horizontal axis is voltage_drop, the vertical axis is
current. Ohm's law is satisfied when the graph is a straight line through the
origin. Therefore, the two resistors are ohmic, but the diode and battery are
not.
For many materials, the current I through the material is proportional to the
voltage V applied across it:
         I &#x221D; V   {\displaystyle I\propto V}  [I \propto V]
over a wide range of voltages and currents. Therefore, the resistance and
conductance of objects or electronic components made of these materials is
constant. This relationship is called Ohm's_law, and materials which obey it
are called ohmic materials. Examples of ohmic components are wires and
resistors. The current-voltage_(IV)_graph of an ohmic device consists of a
straight line through the origin with positive slope.
Other components and materials used in electronics do not obey Ohm's law; the
current is not proportional to the voltage, so the resistance varies with the
voltage and current through them. These are called nonlinear or nonohmic.
Examples include diodes and fluorescent_lamps. The IV curve of a nonohmic
device is a curved line.
***** Relation to resistivity and conductivity[edit] *****
Main article: Electrical_resistivity_and_conductivity
A piece of resistive material with electrical contacts on both ends.
The resistance of a given object depends primarily on two factors: What
material it is made of, and its shape. For a given material, the resistance is
inversely proportional to the cross-sectional area; for example, a thick copper
wire has lower resistance than an otherwise-identical thin copper wire. Also,
for a given material, the resistance is proportional to the length; for
example, a long copper wire has higher resistance than an otherwise-identical
short copper wire. The resistance R and conductance G of a conductor of uniform
cross section, therefore, can be computed as
             R    = &#x03C1;   &#x2113; A   ,     G    = &#x03C3;   A &#x2113;
      .       {\displaystyle {\begin{aligned}R&=\rho {\frac {\ell }{A}},\\
      [5pt]G&=\sigma {\frac {A}{\ell }}.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}R&=\rho {\frac {\ell }{A}},\\[5pt]G&=\sigma {\frac {A}
      {\ell }}.\end{aligned}}}]
where     &#x2113;   {\displaystyle \ell }  [\ell ] is the length of the
conductor, measured in metres (m), A is the cross-sectional area of the
conductor measured in square_metres (mÂ²), Ï (sigma) is the electrical
conductivity measured in siemens per meter (SÂ·mâ1), and Ï (rho) is the
electrical_resistivity (also called specific electrical resistance) of the
material, measured in ohm-metres (Î©Â·m). The resistivity and conductivity are
proportionality constants, and therefore depend only on the material the wire
is made of, not the geometry of the wire. Resistivity and conductivity are
reciprocals:     &#x03C1; = 1  /  &#x03C3;   {\displaystyle \rho =1/\sigma }
[\rho=1/\sigma]. Resistivity is a measure of the material's ability to oppose
electric current.
This formula is not exact, as it assumes the current_density is totally uniform
in the conductor, which is not always true in practical situations. However,
this formula still provides a good approximation for long thin conductors such
as wires.
Another situation for which this formula is not exact is with alternating
current (AC), because the skin_effect inhibits current flow near the center of
the conductor. For this reason, the geometrical cross-section is different from
the effective cross-section in which current actually flows, so resistance is
higher than expected. Similarly, if two conductors near each other carry AC
current, their resistances increase due to the proximity_effect. At commercial
power_frequency, these effects are significant for large conductors carrying
large currents, such as busbars in an electrical_substation,[3] or large power
cables carrying more than a few hundred amperes.
The resistivity of different materials varies by an enormous amount: For
example, the conductivity of teflon is about 1030 times lower than the
conductivity of copper. Why is there such a difference? Loosely speaking, a
metal has large numbers of "delocalized" electrons that are not stuck in any
one place, but free to move across large distances, whereas in an insulator
(like teflon), each electron is tightly bound to a single molecule, and a great
force is required to pull it away. Semiconductors lie between these two
extremes. More details can be found in the article: Electrical_resistivity_and
conductivity. For the case of electrolyte solutions, see the article:
Conductivity_(electrolytic).
Resistivity varies with temperature. In semiconductors, resistivity also
changes when exposed to light. See below.
***** Measuring resistance[edit] *****
Main article: Ohmmeter
An instrument for measuring resistance is called an ohmmeter. Simple ohmmeters
cannot measure low resistances accurately because the resistance of their
measuring leads causes a voltage drop that interferes with the measurement, so
more accurate devices use four-terminal_sensing.
***** Typical resistances[edit] *****
See also: Electrical_resistivities_of_the_elements_(data_page) and Electrical
resistivity_and_conductivity
Component                                  Resistance (Î©)
1 meter of copper wire with 1 mm diameter 0.02[4]
1 km overhead_power_line (typical)        0.03[5]
AA_battery (typical internal_resistance)   0.1[6]
Incandescent_light_bulb filament (typical) 200â1000[7]
Human body                                 1000 to 100,000[8]
***** Static and differential resistance[edit] *****
See also: Small-signal_model
[Differential_versus_chordal_resistance]
The IV_curve of a non-ohmic device (purple). The static resistance at point A
is the inverse slope of line B through the origin. The differential resistance
at A is the inverse slope of tangent_line C.
[Negative_differential_resistance]
The IV_curve of a component with negative_differential_resistance, an unusual
phenomenon where the IV curve is non-monotonic.
Many electrical elements, such as diodes and batteries do not satisfy Ohm's
law. These are called non-ohmic or non-linear, and their IâV_curves are not
straight lines through the origin.
Resistance and conductance can still be defined for non-ohmic elements.
However, unlike ohmic resistance, non-linear resistance is not constant but
varies with the voltage or current through the device; i.e., its operating
point. There are two types of resistance:[1][2]
    * Static resistance (also called chordal or DC resistance) â This
      corresponds to the usual definition of resistance; the voltage divided by
      the current
                R   s t a t i c    =   V I      {\displaystyle R_{\mathrm
            {static} }={\frac {V}{I}}\,}  [R_\mathrm{static} = \frac {V}{I}
            \,].
      It is the slope of the line (chord) from the origin through the point on
      the curve. Static resistance determines the power dissipation in an
      electrical component. Points on the IV curve located in the 2nd or 4th
      quadrants, for which the slope of the chordal line is negative, have
      negative static resistance. Passive devices, which have no source of
      energy, cannot have negative static resistance. However active devices
      such as transistors or op-amps can synthesize negative static resistance
      with feedback, and it is used in some circuits such as gyrators.
    * Differential resistance (also called dynamic, incremental or small signal
      resistance) â Differential_resistance is the derivative of the voltage
      with respect to the current; the slope of the IV curve at a point
                R   d i f f    =    d V   d I       {\displaystyle R_{\mathrm
            {diff} }={\frac {dV}{dI}}\,}  [R_\mathrm{diff} = \frac {dV}{dI}
            \,].
      If the IV curve is nonmonotonic (with peaks and troughs), the curve has a
      negative slope in some regionsâso in these regions the device has
      negative_differential_resistance. Devices with negative differential
      resistance can amplify a signal applied to them, and are used to make
      amplifiers and oscillators. These include tunnel_diodes, Gunn_diodes,
      IMPATT_diodes, magnetron tubes, and unijunction_transistors.
***** AC circuits[edit] *****
**** Impedance and admittance[edit] ****
Main articles: Electrical_impedance and Admittance
The voltage (red) and current (blue) versus time (horizontal axis) for a
capacitor (top) and inductor (bottom). Since the amplitude of the current and
voltage sinusoids are the same, the absolute_value of impedance is 1 for both
the capacitor and the inductor (in whatever units the graph is using). On the
other hand, the phase_difference between current and voltage is â90Â° for the
capacitor; therefore, the complex_phase of the impedance of the capacitor is
â90Â°. Similarly, the phase_difference between current and voltage is +90Â°
for the inductor; therefore, the complex phase of the impedance of the inductor
is +90Â°.
When an alternating current flows through a circuit, the relation between
current and voltage across a circuit element is characterized not only by the
ratio of their magnitudes, but also the difference in their phases. For
example, in an ideal resistor, the moment when the voltage reaches its maximum,
the current also reaches its maximum (current and voltage are oscillating in
phase). But for a capacitor or inductor, the maximum current flow occurs as the
voltage passes through zero and vice versa (current and voltage are oscillating
90Â° out of phase, see image at right). Complex_numbers are used to keep track
of both the phase and magnitude of current and voltage:
         V ( t ) =  Re  (  V  0    e  j &#x03C9; t   ) ,  I ( t ) =  Re  (  I
      0    e  j &#x03C9; t   ) ,  Z =    V  0    I  0     ,  Y =    I  0    V
      0       {\displaystyle V(t)={\text{Re}}(V_{0}e^{j\omega t}),\quad I(t)=
      {\text{Re}}(I_{0}e^{j\omega t}),\quad Z={\frac {V_{0}}{I_{0}}},\quad Y=
      {\frac {I_{0}}{V_{0}}}}  [V(t)=\text{Re}(V_0 e^{j\omega t}), \quad I
      (t)=\text{Re}(I_0 e^{j\omega t}), \quad Z=\frac{V_0}{I_0}, \quad Y=\frac
      {I_0}{V_0}]
where:
    * t is time,
    * V(t) and I(t) are, respectively, voltage and current as a function of
      time,
    * V0, I0, Z, and Y are complex numbers,
    * Z is called impedance,
    * Y is called admittance,
    * Re indicates real_part,
    *    &#x03C9;   {\displaystyle \omega }  [\omega ] is the angular_frequency
      of the AC current,
    *    j =   &#x2212; 1     {\displaystyle j={\sqrt {-1}}}  [j=\sqrt{-1}] is
      the imaginary_unit.
The impedance and admittance may be expressed as complex numbers that can be
broken into real and imaginary parts:
         Z = R + j X ,  Y = G + j B   {\displaystyle Z=R+jX,\quad Y=G+jB}
      [Z=R+jX, \quad Y=G+jB]
where R and G are resistance and conductance respectively, X is reactance, and
B is susceptance. For ideal resistors, Z and Y reduce to R and G respectively,
but for AC networks containing capacitors and inductors, X and B are nonzero.
   Z = 1  /  Y   {\displaystyle Z=1/Y}  [Z=1/Y] for AC circuits, just as     R
= 1  /  G   {\displaystyle R=1/G}  [R=1/G] for DC circuits.
**** Frequency dependence of resistance[edit] ****
A key feature of AC circuits is that the resistance and conductance can be
frequency-dependent, a phenomenon known as the universal_dielectric_response
[9]. One reason, mentioned above is the skin_effect (and the related proximity
effect). Another reason is that the resistivity itself may depend on frequency
(see Drude_model, deep-level_traps, resonant_frequency, KramersâKronig
relations, etc.)
***** Energy dissipation and Joule heating[edit] *****
Main article: Joule_heating
Running current through a material with high resistance creates heat, in a
phenomenon called Joule_heating. In this picture, a cartridge_heater, warmed by
Joule heating, is glowing_red_hot.
Resistors (and other elements with resistance) oppose the flow of electric
current; therefore, electrical energy is required to push current through the
resistance. This electrical energy is dissipated, heating the resistor in the
process. This is called Joule_heating (after James_Prescott_Joule), also called
ohmic heating or resistive heating.
The dissipation of electrical energy is often undesired, particularly in the
case of transmission_losses in power_lines. High_voltage_transmission helps
reduce the losses by reducing the current for a given power.
On the other hand, Joule heating is sometimes useful, for example in electric
stoves and other electric_heaters (also called resistive heaters). As another
example, incandescent_lamps rely on Joule heating: the filament is heated to
such a high temperature that it glows "white hot" with thermal_radiation (also
called incandescence).
The formula for Joule heating is:
         P =  I  2   R   {\displaystyle P=I^{2}R}  [P=I^2R]
where P is the power (energy per unit time) converted from electrical energy to
thermal energy, R is the resistance, and I is the current through the resistor.
***** Dependence of resistance on other conditions[edit] *****
**** Temperature dependence[edit] ****
Main article: Electrical_resistivity_and_conductivity_Â§ Temperature_dependence
Near room temperature, the resistivity of metals typically increases as
temperature is increased, while the resistivity of semiconductors typically
decreases as temperature is increased. The resistivity of insulators and
electrolytes may increase or decrease depending on the system. For the detailed
behavior and explanation, see Electrical_resistivity_and_conductivity.
As a consequence, the resistance of wires, resistors, and other components
often change with temperature. This effect may be undesired, causing an
electronic circuit to malfunction at extreme temperatures. In some cases,
however, the effect is put to good use. When temperature-dependent resistance
of a component is used purposefully, the component is called a resistance
thermometer or thermistor. (A resistance thermometer is made of metal, usually
platinum, while a thermistor is made of ceramic or polymer.)
Resistance thermometers and thermistors are generally used in two ways. First,
they can be used as thermometers: By measuring the resistance, the temperature
of the environment can be inferred. Second, they can be used in conjunction
with Joule_heating (also called self-heating): If a large current is running
through the resistor, the resistor's temperature rises and therefore its
resistance changes. Therefore, these components can be used in a circuit-
protection role similar to fuses, or for feedback in circuits, or for many
other purposes. In general, self-heating can turn a resistor into a nonlinear
and hysteretic circuit element. For more details see Thermistor#Self-heating
effects.
If the temperature T does not vary too much, a linear_approximation is
typically used:
         R ( T ) =  R  0   [ 1 + &#x03B1; ( T &#x2212;  T  0   ) ]
      {\displaystyle R(T)=R_{0}[1+\alpha (T-T_{0})]}  [R(T) = R_0[1+\alpha (T -
      T_0)]]
where     &#x03B1;   {\displaystyle \alpha }  [\alpha ] is called the
temperature coefficient of resistance,      T  0     {\displaystyle T_{0}}  [T_
{0}] is a fixed reference temperature (usually room temperature), and      R  0
{\displaystyle R_{0}}  [R_{0}] is the resistance at temperature      T  0
{\displaystyle T_{0}}  [T_{0}]. The parameter     &#x03B1;   {\displaystyle
\alpha }  [\alpha ] is an empirical parameter fitted from measurement data.
Because the linear approximation is only an approximation,     &#x03B1;
{\displaystyle \alpha }  [\alpha ] is different for different reference
temperatures. For this reason it is usual to specify the temperature that
&#x03B1;   {\displaystyle \alpha }  [\alpha ] was measured at with a suffix,
such as      &#x03B1;  15     {\displaystyle \alpha _{15}}  [\alpha _{15}], and
the relationship only holds in a range of temperatures around the reference.
[10]
The temperature coefficient     &#x03B1;   {\displaystyle \alpha }  [\alpha ]
is typically +3Ã10â3 Kâ1 to +6Ã10â3 Kâ1 for metals near room
temperature. It is usually negative for semiconductors and insulators, with
highly variable magnitude.[11]
**** Strain dependence[edit] ****
Main article: Strain_gauge
Just as the resistance of a conductor depends upon temperature, the resistance
of a conductor depends upon strain. By placing a conductor under tension (a
form of stress that leads to strain in the form of stretching of the
conductor), the length of the section of conductor under tension increases and
its cross-sectional area decreases. Both these effects contribute to increasing
the resistance of the strained section of conductor. Under compression (strain
in the opposite direction), the resistance of the strained section of conductor
decreases. See the discussion on strain_gauges for details about devices
constructed to take advantage of this effect.
**** Light illumination dependence[edit] ****
Main articles: Photoresistor and Photoconductivity
Some resistors, particularly those made from semiconductors, exhibit
photoconductivity, meaning that their resistance changes when light is shining
on them. Therefore, they are called photoresistors (or light dependent
resistors). These are a common type of light_detector.
***** Superconductivity[edit] *****
Main article: Superconductivity
Superconductors are materials that have exactly zero resistance and infinite
conductance, because they can have V=0 and Iâ 0. This also means there is no
joule_heating, or in other words no dissipation of electrical energy.
Therefore, if superconductive wire is made into a closed loop, current flows
around the loop forever. Superconductors require cooling to temperatures near 4
K with liquid_helium for most metallic superconductors like niobiumâtin
alloys, or cooling to temperatures near 77K with liquid_nitrogen for the
expensive, brittle and delicate ceramic high_temperature_superconductors.
Nevertheless, there are many technological_applications_of_superconductivity,
including superconducting_magnets.
***** See also[edit] *****
    * [icon]Electronics_portal
    * Conductance_quantum and its reciprocal, the Von Klitzing constant (under
      Von_Klitzing)
    * Electrical_measurements
    * Contact_resistance
    * Electrical_resistivity_and_conductivity for more information about the
      physical mechanisms for conduction in materials.
    * JohnsonâNyquist_noise
    * Quantum_Hall_effect, a standard for high-accuracy resistance
      measurements.
    * Resistor
    * RKM_code
    * Series_and_parallel_circuits
    * Sheet_resistance
    * SI_electromagnetism_units
    * Thermal_resistance
    * Voltage_divider
    * Voltage_drop
***** References[edit] *****
   1. ^ a bForbes T. Brown (2006). Engineering_System_Dynamics. CRC Press.
      p. 43. ISBN 978-0-8493-9648-9.
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
   3. ^ a bKenneth L. Kaiser (2004). Electromagnetic_Compatibility_Handbook.
      CRC Press. pp. 13â52. ISBN 978-0-8493-2087-3.
   4. ^ Fink and Beaty, Standard Handbook for Electrical Engineers 11th
      Edition, page 17-19
   5. ^ The resistivity of copper is about 1.7Ã10â8 Î©m. See [1].
   6. ^John D. McDonald (2016). Electric_Power_Substations_Engineering,_Second
      Edition. CRC Press. pp. 363â. ISBN 978-1-4200-0731-2.
   7. ^ [2] For a fresh Energizer E91 AA alkaline battery, the internal
      resistance varies from 0.9 Î© at -40 Â°C, to 0.1 Î© at +40 Â°C.
   8. ^ A 60 W light bulb in the USA (120 V mains_electricity) draws RMS
      current 60 W/120 V=500 mA, so its resistance is 120 V/500 mA=240 Î©. The
      resistance of a 60 W light bulb in Europe (230 V mains) is 900 Î©. The
      resistance of a filament is temperature-dependent; these values are for
      when the filament is already heated up and the light is already glowing.
   9. ^ 100,000 Î© for dry skin contact, 1000 Î© for wet or broken skin
      contact. High voltage breaks down the skin, lowering resistance to 500
      Î©. Other factors and conditions are relevant as well. For more details,
      see the electric_shock article, and:"Publication_No._98-131:_Worker
      Deaths_by_Electrocution" (PDF). National_Institute_for_Occupational
      Safety_and_Health. Retrieved 2014-11-02.
  10. ^Zhai, Chongpu; Gan, Yixiang; Hanaor, Dorian; Proust, GwÃ©naÃ«lle (2018).
      "Stress-dependent electrical transport and its universal scaling in
      granular materials". Extreme Mechanics Letters. 22: 83â88. arXiv:
      1712.05938. doi:10.1016/j.eml.2018.05.005.
  11. ^ Ward, MR, Electrical Engineering Science, pp36â40, McGraw-Hill, 1971.
  12. ^ See Electrical_resistivity_and_conductivity for a table. The
      temperature coefficient of resistivity is similar but not identical to
      the temperature coefficient of resistance. The small difference is due to
      thermal_expansion changing the dimensions of the resistor.
***** External links[edit] *****
    * Clemson_Vehicular_Electronics_Laboratory:_Resistance_Calculator
    * Electron_Conductance_Models_Using_Maximal_Entropy_Random_Walks Wolfram
      Demonstrantions Project
                                              * BNF: cb119825351 (data)
Authority_control [Edit_this_at_Wikidata]     * GND: 4128466-5
                                              * LCCN: sh85041986
                                              * NDL: 00561371

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Electrical_resistance_and_conductance&oldid=909458982"
Categories:
    * Electrical_resistance_and_conductance
    * Electricity
    * Physical_quantities
    * Electromagnetism
Hidden categories:
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
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
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Boarisch
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * ChiShona
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Ido
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Kiswahili
    * KreyÃ²l_ayisyen
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * Latina
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Bahasa_Melayu
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * æ¥æ¬èª
    * Nordfriisk
    * Norsk
    * Norsk_nynorsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * à¨ªà©°à¨à¨¾à¨¬à©
    * PlattdÃ¼Ã¼tsch
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Runa_Simi
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Seeltersk
    * Shqip
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * à°¤à±à°²à±à°à±
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * TÃ¼rkmenÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Ø¦ÛÙØºÛØ±ÚÛ_/_Uyghurche
    * Tiáº¿ng_Viá»t
    * æè¨
    * Wolof
    * å´è¯­
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 5 August 2019, at 15:37 (UTC).
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
