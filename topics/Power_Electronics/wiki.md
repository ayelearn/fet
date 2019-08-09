The following text has been accessed from https://en.wikipedia.org/wiki/Power_electronics at Thu Aug 8 22:48:57 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Power electronics ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the technology of power electronics. For the musical
genre, see power_electronics_(music).
 This article may require cleanup to meet Wikipedia's quality_standards. The
 specific problem is: Formatting of mathematical formulas. Please help improve
 this_article if you can. (March 2018)(Learn_how_and_when_to_remove_this
 template_message)
An HVDC thyristor valve tower 16.8 m tall in a hall at Baltic Cable AB in
Sweden
A battery_charger is an example of a piece of power electronics
A PCs power supply is an example of a piece of power electronics, whether
inside or outside of the cabinet
Power electronics is the application of solid-state_electronics to the control
and conversion of electric power.
The first high power electronic devices were mercury-arc_valves. In modern
systems the conversion is performed with semiconductor switching devices such
as diodes, thyristors and transistors, pioneered by R._D._Middlebrook and
others beginning in the 1950s. In contrast to electronic systems concerned with
transmission and processing of signals and data, in power electronics
substantial amounts of electrical energy are processed. An AC/DC converter
(rectifier) is the most typical power electronics device found in many consumer
electronic devices, e.g. television sets, personal computers, battery_chargers,
etc. The power range is typically from tens of watts to several hundred watts.
In industry a common application is the variable_speed_drive_(VSD) that is used
to control an induction_motor. The power range of VSDs start from a few hundred
watts and end at tens of megawatts.
The power conversion systems can be classified according to the type of the
input and output power
    * AC to DC (rectifier)
    * DC to AC (inverter)
    * DC to DC (DC-to-DC_converter)
    * AC to AC (AC-to-AC_converter)
⁰
***** Contents *****
    * 1_History
    * 2_Devices
    * 3_DC/AC_converters_(inverters)
          o 3.1_Single-phase_half-bridge_inverter
          o 3.2_Single-phase_full-bridge_inverter
          o 3.3_Three-phase_voltage_source_inverter
          o 3.4_Current_source_inverters
          o 3.5_Multilevel_inverters
    * 4_AC/AC_converters
    * 5_Simulations_of_power_electronic_systems
    * 6_Applications
          o 6.1_Inverters
          o 6.2_Smart_grid
    * 7_Notes
    * 8_References
    * 9_External_links
***** History[edit] *****
Power electronics started with the development of the mercury arc rectifier.
Invented by Peter_Cooper_Hewitt in 1902, it was used to convert alternating
current (AC) into direct current (DC). From the 1920s on, research continued on
applying thyratrons and grid-controlled mercury arc valves to power
transmission. Uno_Lamm developed a mercury valve with grading electrodes making
them suitable for high_voltage_direct_current power transmission. In 1933
selenium rectifiers were invented.[1]
In 1947, the bipolar point-contact transistor was invented by Walter_H.
Brattain and John_Bardeen under the direction of William_Shockley at Bell_Labs.
In 1948 Shockley's invention of the bipolar_junction_transistor (BJT) improved
the stability and performance of transistors, and reduced costs. By the 1950s,
higher power semiconductor diodes became available and started replacing vacuum
tubes. In 1956 the silicon_controlled_rectifier (SCR) was introduced by General
Electric, greatly increasing the range of power electronics applications.[2]
A breakthrough in power electronics came with the invention of the MOSFET
(metal-oxide-semiconductor field-effect transistor) by Mohamed_Atalla and Dawon
Kahng at Bell Labs in 1959. Generations of MOSFET transistors enabled power
designers to achieve performance and density levels not possible with bipolar
transistors.[3]
By the 1960s, the improved switching speed of bipolar_junction_transistors had
allowed for high frequency DC/DC converters. In 1976, power_MOSFETs became
commercially available. In 1982, the Insulated Gate Bipolar Transistor (IGBT)
was introduced.
***** Devices[edit] *****
See also: Power_semiconductor_device
 This section includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 section by introducing more precise citations. (December 2013)(Learn_how_and
 when_to_remove_this_template_message)
The capabilities and economy of power electronics system are determined by the
active devices that are available. Their characteristics and limitations are a
key element in the design of power electronics systems. Formerly, the mercury
arc_valve, the high-vacuum and gas-filled diode thermionic rectifiers, and
triggered devices such as the thyratron and ignitron were widely used in power
electronics. As the ratings of solid-state devices improved in both voltage and
current-handling capacity, vacuum devices have been nearly entirely replaced by
solid-state devices.
Power electronic devices may be used as switches, or as amplifiers.[4] An ideal
switch is either open or closed and so dissipates no power; it withstands an
applied voltage and passes no current, or passes any amount of current with no
voltage drop. Semiconductor devices used as switches can approximate this ideal
property and so most power electronic applications rely on switching devices on
and off, which makes systems very efficient as very little power is wasted in
the switch. By contrast, in the case of the amplifier, the current through the
device varies continuously according to a controlled input. The voltage and
current at the device terminals follow a load_line, and the power dissipation
inside the device is large compared with the power delivered to the load.
Several attributes dictate how devices are used. Devices such as diodes conduct
when a forward voltage is applied and have no external control of the start of
conduction. Power devices such as silicon_controlled_rectifiers and thyristors
(as well as the mercury valve and thyratron) allow control of the start of
conduction, but rely on periodic reversal of current flow to turn them off.
Devices such as gate turn-off thyristors, BJT and MOSFET transistors provide
full switching control and can be turned on or off without regard to the
current flow through them. Transistor devices also allow proportional
amplification, but this is rarely used for systems rated more than a few
hundred watts. The control input characteristics of a device also greatly
affect design; sometimes the control input is at a very high voltage with
respect to ground and must be driven by an isolated source.
As efficiency is at a premium in a power electronic converter, the losses that
a power electronic device generates should be as low as possible.
Devices vary in switching speed. Some diodes and thyristors are suited for
relatively slow speed and are useful for power_frequency switching and control;
certain thyristors are useful at a few kilohertz. Devices such as MOSFETS and
BJTs can switch at tens of kilohertz up to a few megahertz in power
applications, but with decreasing power levels. Vacuum tube devices dominate
high power (hundreds of kilowatts) at very high frequency (hundreds or
thousands of megahertz) applications. Faster switching devices minimize energy
lost in the transitions from on to off and back, but may create problems with
radiated electromagnetic interference. Gate drive (or equivalent) circuits must
be designed to supply sufficient drive current to achieve the full switching
speed possible with a device. A device without sufficient drive to switch
rapidly may be destroyed by excess heating.
Practical devices have non-zero voltage drop and dissipate power when on, and
take some time to pass through an active region until they reach the "on" or
"off" state. These losses are a significant part of the total lost power in a
converter.
Power handling and dissipation of devices is also a critical factor in design.
Power electronic devices may have to dissipate tens or hundreds of watts of
waste heat, even switching as efficiently as possible between conducting and
non-conducting states. In the switching mode, the power controlled is much
larger than the power dissipated in the switch. The forward voltage drop in the
conducting state translates into heat that must be dissipated. High power
semiconductors require specialized heat_sinks or active cooling systems to
manage their junction temperature; exotic semiconductors such as silicon
carbide have an advantage over straight silicon in this respect, and germanium,
once the main-stay of solid-state electronics is now little used due to its
unfavorable high temperature properties.
Semiconductor devices exist with ratings up to a few kilovolts in a single
device. Where very high voltage must be controlled, multiple devices must be
used in series, with networks to equalize voltage across all devices. Again,
switching speed is a critical factor since the slowest-switching device will
have to withstand a disproportionate share of the overall voltage. Mercury
valves were once available with ratings to 100 kV in a single unit, simplifying
their application in HVDC systems.
The current rating of a semiconductor device is limited by the heat generated
within the dies and the heat developed in the resistance of the interconnecting
leads. Semiconductor devices must be designed so that current is evenly
distributed within the device across its internal junctions (or channels); once
a "hot spot" develops, breakdown effects can rapidly destroy the device.
Certain SCRs are available with current ratings to 3000 amperes in a single
unit.

***** DC/AC converters (inverters)[edit] *****
Main article: power_inverter
DC to AC converters produce an AC output waveform from a DC source.
Applications include adjustable_speed_drives (ASD), uninterruptible_power
supplies (UPS), Flexible_AC_transmission_systems (FACTS), voltage compensators,
and photovoltaic inverters. Topologies for these converters can be separated
into two distinct categories: voltage source inverters and current source
inverters. Voltage source inverters (VSIs) are named so because the
independently controlled output is a voltage waveform. Similarly, current
source inverters (CSIs) are distinct in that the controlled AC output is a
current waveform.
DC to AC power conversion is the result of power switching devices, which are
commonly fully controllable semiconductor power switches. The output waveforms
are therefore made up of discrete values, producing fast transitions rather
than smooth ones. For some applications, even a rough approximation of the
sinusoidal waveform of AC power is adequate. Where a near sinusoidal waveform
is required, the switching devices are operated much faster than the desired
output frequency, and the time they spend in either state is controlled so the
averaged output is nearly sinusoidal. Common modulation techniques include the
carrier-based technique, or Pulse-width_modulation, space-vector_technique, and
the selective-harmonic technique.[5]
Voltage source inverters have practical uses in both single-phase and three-
phase applications. Single-phase VSIs utilize half-bridge and full-bridge
configurations, and are widely used for power supplies, single-phase UPSs, and
elaborate high-power topologies when used in multicell configurations. Three-
phase VSIs are used in applications that require sinusoidal voltage waveforms,
such as ASDs, UPSs, and some types of FACTS devices such as the STATCOM. They
are also used in applications where arbitrary voltages are required as in the
case of active power filters and voltage compensators.[5]
Current source inverters are used to produce an AC output current from a DC
current supply. This type of inverter is practical for three-phase applications
in which high-quality voltage waveforms are required.
A relatively new class of inverters, called multilevel inverters, has gained
widespread interest. Normal operation of CSIs and VSIs can be classified as
two-level inverters, due to the fact that power switches connect to either the
positive or to the negative DC bus. If more than two voltage levels were
available to the inverter output terminals, the AC output could better
approximate a sine wave. It is for this reason that multilevel inverters,
although more complex and costly, offer higher performance.[6]
Each inverter type differs in the DC links used, and in whether or not they
require freewheeling_diodes. Either can be made to operate in square-wave or
pulse-width modulation (PWM) mode, depending on its intended usage. Square-wave
mode offers simplicity, while PWM can be implemented several different ways and
produces higher quality waveforms.[5]
Voltage Source Inverters (VSI) feed the output inverter section from an
approximately constant-voltage source.[5]
The desired quality of the current output waveform determines which modulation
technique needs to be selected for a given application. The output of a VSI is
composed of discrete values. In order to obtain a smooth current waveform, the
loads need to be inductive at the select harmonic frequencies. Without some
sort of inductive filtering between the source and load, a capacitive load will
cause the load to receive a choppy current waveform, with large and frequent
current spikes.[5]
There are three main types of VSIs:
   1. Single-phase half-bridge inverter
   2. Single-phase full-bridge inverter
   3. Three-phase voltage source inverter
**** Single-phase half-bridge inverter[edit] ****
Figure 8: The AC input for an ASD.
FIGURE 9: Single-Phase Half-Bridge Voltage Source Inverter
The single-phase voltage source half-bridge inverters, are meant for lower
voltage applications and are commonly used in power supplies.[5] Figure 9 shows
the circuit schematic of this inverter.
Low-order current harmonics get injected back to the source voltage by the
operation of the inverter. This means that two large capacitors are needed for
filtering purposes in this design.[5] As Figure 9 illustrates, only one switch
can be on at time in each leg of the inverter. If both switches in a leg were
on at the same time, the DC source will be shorted out.
Inverters can use several modulation techniques to control their switching
schemes. The carrier-based PWM technique compares the AC output waveform, vc,
to a carrier voltage signal, vÎ. When vc is greater than vÎ, S+ is on, and
when vc is less than vÎ, S- is on. When the AC output is at frequency fc with
its amplitude at vc, and the triangular carrier signal is at frequency fÎ with
its amplitude at vÎ, the PWM becomes a special sinusoidal case of the carrier
based PWM.[5] This case is dubbed sinusoidal pulse-width modulation (SPWM).For
this, the modulation index, or amplitude-modulation ratio, is defined as ma =
vc/vâ.
The normalized carrier frequency, or frequency-modulation ratio, is calculated
using the equation mf = fâ/fc.
If the over-modulation region, ma, exceeds one, a higher fundamental AC output
voltage will be observed, but at the cost of saturation. For SPWM, the
harmonics of the output waveform are at well-defined frequencies and
amplitudes. This simplifies the design of the filtering components needed for
the low-order current harmonic injection from the operation of the inverter.
The maximum output amplitude in this mode of operation is half of the source
voltage. If the maximum output amplitude, ma, exceeds 3.24, the output waveform
of the inverter becomes a square wave.[5]
As was true for PWM, both switches in a leg for square wave modulation cannot
be turned on at the same time, as this would cause a short across the voltage
source. The switching scheme requires that both S+ and S- be on for a half
cycle of the AC output period.[5] The fundamental AC output amplitude is equal
to vo1 = vaN = 2vi/Ï.
Its harmonics have an amplitude of voh = vo1/h.
Therefore, the AC output voltage is not controlled by the inverter, but rather
by the magnitude of the DC input voltage of the inverter.[5]
Using selective harmonic elimination (SHE) as a modulation technique allows the
switching of the inverter to selectively eliminate intrinsic harmonics. The
fundamental component of the AC output voltage can also be adjusted within a
desirable range. Since the AC output voltage obtained from this modulation
technique has odd half and odd quarter wave symmetry, even harmonics do not
exist.[5] Any undesirable odd (N-1) intrinsic harmonics from the output
waveform can be eliminated.
**** Single-phase full-bridge inverter[edit] ****
FIGURE 3: Single-Phase Voltage Source Full-Bridge Inverter
FIGURE 4: Carrier and Modulating Signals for the Bipolar Pulsewidth Modulation
Technique
The full-bridge inverter is similar to the half bridge-inverter, but it has an
additional leg to connect the neutral point to the load.[5] Figure 3 shows the
circuit schematic of the single-phase voltage source full-bridge inverter.
To avoid shorting out the voltage source, S1+ and S1- cannot be on at the same
time, and S2+ and S2- also cannot be on at the same time. Any modulating
technique used for the full-bridge configuration should have either the top or
the bottom switch of each leg on at any given time. Due to the extra leg, the
maximum amplitude of the output waveform is Vi, and is twice as large as the
maximum achievable output amplitude for the half-bridge configuration.[5]
States 1 and 2 from Table 2 are used to generate the AC output voltage with
bipolar SPWM. The AC output voltage can take on only two values, either Vi or
âVi. To generate these same states using a half-bridge configuration, a
carrier based technique can be used. S+ being on for the half-bridge
corresponds to S1+ and S2- being on for the full-bridge. Similarly, S- being on
for the half-bridge corresponds to S1- and S2+ being on for the full bridge.
The output voltage for this modulation technique is more or less sinusoidal,
with a fundamental component that has an amplitude in the linear region of less
than or equal to one[5] vo1 =vab1= vi • ma.
Unlike the bipolar PWM technique, the unipolar approach uses states 1, 2, 3 and
4 from Table 2 to generate its AC output voltage. Therefore, the AC output
voltage can take on the values Vi, 0 or âV [1]i. To generate these states,
two sinusoidal modulating signals, Vc and âVc, are needed, as seen in Figure
4.
Vc is used to generate VaN, while âVc is used to generate VbN. The following
relationship is called unipolar carrier-based SPWM vo1 =2 • vaN1= vi • ma.
The phase voltages VaN and VbN are identical, but 180 degrees out of phase with
each other. The output voltage is equal to the difference of the two phase
voltages, and do not contain any even harmonics. Therefore, if mf is taken,
even the AC output voltage harmonics will appear at normalized odd frequencies,
fh. These frequencies are centered on double the value of the normalized
carrier frequency. This particular feature allows for smaller filtering
components when trying to obtain a higher quality output waveform.[5]
As was the case for the half-bridge SHE, the AC output voltage contains no even
harmonics due to its odd half and odd quarter wave symmetry.[5]
**** Three-phase voltage source inverter[edit] ****
FIGURE 5: Three-Phase Voltage Source Inverter Circuit Schematic
FIGURE 6: Three-Phase Square-Wave Operation a) Switch State S1 b) Switch State
S3 c) S1 Output d) S3 Output
Single-phase VSIs are used primarily for low power range applications, while
three-phase VSIs cover both medium and high power range applications.[5] Figure
5 shows the circuit schematic for a three-phase VSI.
Switches in any of the three legs of the inverter cannot be switched off
simultaneously due to this resulting in the voltages being dependent on the
respective line current's polarity. States 7 and 8 produce zero AC line
voltages, which result in AC line currents freewheeling through either the
upper or the lower components. However, the line voltages for states 1 through
6 produce an AC line voltage consisting of the discrete values of Vi, 0 or
âVi.[5]
For three-phase SPWM, three modulating signals that are 120 degrees out of
phase with one another are used in order to produce out of phase load voltages.
In order to preserve the PWM features with a single carrier signal, the
normalized carrier frequency, mf, needs to be a multiple of three. This keeps
the magnitude of the phase voltages identical, but out of phase with each other
by 120 degrees.[5] The maximum achievable phase voltage amplitude in the linear
region, ma less than or equal to one, is vphase = vi / 2. The maximum
achievable line voltage amplitude is Vab1 = vab • √3 / 2
The only way to control the load voltage is by changing the input DC voltage.
**** Current source inverters[edit] ****
FIGURE 7: Three-Phase Current Source Inverter
Figure 8: Synchronized-Pulse-Width-Modulation Waveforms for a Three-Phase
Current Source Inverter a) Carrier and Modulating Signals b) S1 State c) S3
State d) Output Current
Figure 9: Space-Vector Representation in Current Source Inverters
Current source inverters convert DC current into an AC current waveform. In
applications requiring sinusoidal AC waveforms, magnitude, frequency, and phase
should all be controlled. CSIs have high changes in current over time, so
capacitors are commonly employed on the AC side, while inductors are commonly
employed on the DC side.[5] Due to the absence of freewheeling diodes, the
power circuit is reduced in size and weight, and tends to be more reliable than
VSIs.[6] Although single-phase topologies are possible, three-phase CSIs are
more practical.
In its most generalized form, a three-phase CSI employs the same conduction
sequence as a six-pulse rectifier. At any time, only one common-cathode switch
and one common-anode switch are on.[6]
As a result, line currents take discrete values of âii, 0 and ii. States are
chosen such that a desired waveform is output and only valid states are used.
This selection is based on modulating techniques, which include carrier-based
PWM, selective harmonic elimination, and space-vector techniques.[5]
Carrier-based techniques used for VSIs can also be implemented for CSIs,
resulting in CSI line currents that behave in the same way as VSI line
voltages. The digital circuit utilized for modulating signals contains a
switching pulse generator, a shorting pulse generator, a shorting pulse
distributor, and a switching and shorting pulse combiner. A gating signal is
produced based on a carrier current and three modulating signals.[5]
A shorting pulse is added to this signal when no top switches and no bottom
switches are gated, causing the RMS currents to be equal in all legs. The same
methods are utilized for each phase, however, switching variables are 120
degrees out of phase relative to one another, and the current pulses are
shifted by a half-cycle with respect to output currents. If a triangular
carrier is used with sinusoidal modulating signals, the CSI is said to be
utilizing synchronized-pulse-width-modulation (SPWM). If full over-modulation
is used in conjunction with SPWM the inverter is said to be in square-wave
operation.[5]
The second CSI modulation category, SHE is also similar to its VSI counterpart.
Utilizing the gating signals developed for a VSI and a set of synchronizing
sinusoidal current signals, results in symmetrically distributed shorting
pulses and, therefore, symmetrical gating patterns. This allows any arbitrary
number of harmonics to be eliminated.[5] It also allows control of the
fundamental line current through the proper selection of primary switching
angles. Optimal switching patterns must have quarter-wave and half-wave
symmetry, as well as symmetry about 30 degrees and 150 degrees. Switching
patterns are never allowed between 60 degrees and 120 degrees. The current
ripple can be further reduced with the use of larger output capacitors, or by
increasing the number of switching pulses.[6]
The third category, space-vector-based modulation, generates PWM load line
currents that equal load line currents, on average. Valid switching states and
time selections are made digitally based on space vector transformation.
Modulating signals are represented as a complex vector using a transformation
equation. For balanced three-phase sinusoidal signals, this vector becomes a
fixed module, which rotates at a frequency, Ï. These space vectors are then
used to approximate the modulating signal. If the signal is between arbitrary
vectors, the vectors are combined with the zero vectors I7, I8, or I9.[5] The
following equations are used to ensure that the generated currents and the
current vectors are on average equivalent.
**** Multilevel inverters[edit] ****
FIGURE 10: Three-Level Neutral-Clamped Inverter
A relatively new class called multilevel inverters has gained widespread
interest. Normal operation of CSIs and VSIs can be classified as two-level
inverters because the power switches connect to either the positive or the
negative DC bus.[6] If more than two voltage levels were available to the
inverter output terminals, the AC output could better approximate a sine wave.
[5] For this reason multilevel inverters, although more complex and costly,
offer higher performance.[6] A three-level neutral-clamped inverter is shown in
Figure 10.
Control methods for a three-level inverter only allow two switches of the four
switches in each leg to simultaneously change conduction states. This allows
smooth commutation and avoids shoot through by only selecting valid states.[6]
It may also be noted that since the DC bus voltage is shared by at least two
power valves, their voltage ratings can be less than a two-level counterpart.
Carrier-based and space-vector modulation techniques are used for multilevel
topologies. The methods for these techniques follow those of classic inverters,
but with added complexity. Space-vector modulation offers a greater number of
fixed voltage vectors to be used in approximating the modulation signal, and
therefore allows more effective space vector PWM strategies to be accomplished
at the cost of more elaborate algorithms. Due to added complexity and number of
semiconductor devices, multilevel inverters are currently more suitable for
high-power high-voltage applications.[6] This technology reduces the harmonics
hence improves overall efficiency of the scheme.
***** AC/AC converters[edit] *****
Main article: AC/AC_converter
Converting AC power to AC power allows control of the voltage, frequency, and
phase of the waveform applied to a load from a supplied AC system .[7] The two
main categories that can be used to separate the types of converters are
whether the frequency of the waveform is changed.[8] AC/AC_converter that don't
allow the user to modify the frequencies are known as AC Voltage Controllers,
or AC Regulators. AC converters that allow the user to change the frequency are
simply referred to as frequency converters for AC to AC conversion. Under
frequency converters there are three different types of converters that are
typically used: cycloconverter, matrix converter, DC link converter (aka AC/DC/
AC converter).
AC voltage controller: The purpose of an AC Voltage Controller, or AC
Regulator, is to vary the RMS voltage across the load while at a constant
frequency.[7] Three control methods that are generally accepted are ON/OFF
Control, Phase-Angle Control, and Pulse Width Modulation AC Chopper Control
(PWM AC Chopper Control).[9] All three of these methods can be implemented not
only in single-phase circuits, but three-phase circuits as well.
    * ON/OFF Control: Typically used for heating loads or speed control of
      motors, this control method involves turning the switch on for n integral
      cycles and turning the switch off for m integral cycles. Because turning
      the switches on and off causes undesirable harmonics to be created, the
      switches are turned on and off during zero-voltage and zero-current
      conditions (zero-crossing), effectively reducing the distortion.[9]
    * Phase-Angle Control: Various circuits exist to implement a phase-angle
      control on different waveforms, such as half-wave or full-wave voltage
      control. The power electronic components that are typically used are
      diodes, SCRs, and Triacs. With the use of these components, the user can
      delay the firing angle in a wave which will only cause part of the wave
      to be in output.[7]
    * PWM AC Chopper Control: The other two control methods often have poor
      harmonics, output current quality, and input power factor. In order to
      improve these values PWM can be used instead of the other methods. What
      PWM AC Chopper does is have switches that turn on and off several times
      within alternate half-cycles of input voltage.[9]
Matrix converters and cycloconverters: Cycloconverters are widely used in
industry for ac to ac conversion, because they are able to be used in high-
power applications. They are commutated direct frequency converters that are
synchronised by a supply line. The cycloconverters output voltage waveforms
have complex harmonics with the higher order harmonics being filtered by the
machine inductance. Causing the machine current to have fewer harmonics, while
the remaining harmonics causes losses and torque pulsations. Note that in a
cycloconverter, unlike other converters, there are no inductors or capacitors,
i.e. no storage devices. For this reason, the instantaneous input power and the
output power are equal.[10]
    * Single-Phase to Single-Phase Cycloconverters: Single-Phase to Single-
      Phase Cycloconverters started drawing more interest recently[when?]
      because of the decrease in both size and price of the power electronics
      switches. The single-phase high frequency ac voltage can be either
      sinusoidal or trapezoidal. These might be zero voltage intervals for
      control purpose or zero voltage commutation.
    * Three-Phase to Single-Phase Cycloconverters: There are two kinds of
      three-phase to single-phase cycloconverters: 3Ï to 1Ï half wave
      cycloconverters and 3Ï to 1Ï bridge cycloconverters. Both positive and
      negative converters can generate voltage at either polarity, resulting in
      the positive converter only supplying positive current, and the negative
      converter only supplying negative current.
With recent device advances, newer forms of cycloconverters are being
developed, such as matrix converters. The first change that is first noticed is
that matrix converters utilize bi-directional, bipolar switches. A single phase
to a single phase matrix converter consists of a matrix of 9 switches
connecting the three input phases to the tree output phase. Any input phase and
output phase can be connected together at any time without connecting any two
switches from the same phase at the same time; otherwise this will cause a
short circuit of the input phases. Matrix converters are lighter, more compact
and versatile than other converter solutions. As a result, they are able to
achieve higher levels of integration, higher temperature operation, broad
output frequency and natural bi-directional power flow suitable to regenerate
energy back to the utility.
The matrix converters are subdivided into two types: direct and indirect
converters. A direct matrix converter with three-phase input and three-phase
output, the switches in a matrix converter must be bi-directional, that is,
they must be able to block voltages of either polarity and to conduct current
in either direction. This switching strategy permits the highest possible
output voltage and reduces the reactive line-side current. Therefore, the power
flow through the converter is reversible. Because of its commutation problem
and complex control keep it from being broadly utilized in industry.
Unlike the direct matrix converters, the indirect matrix converters has the
same functionality, but uses separate input and output sections that are
connected through a dc link without storage elements. The design includes a
four-quadrant current source rectifier and a voltage source inverter. The input
section consists of bi-directional bipolar switches. The commutation strategy
can be applied by changing the switching state of the input section while the
output section is in a freewheeling mode. This commutation algorithm is
significantly less complexity and higher reliability as compared to a
conventional direct matrix converter.[11]
DC link converters: DC Link Converters, also referred to as AC/DC/AC
converters, convert an AC input to an AC output with the use of a DC link in
the middle. Meaning that the power in the converter is converted to DC from AC
with the use of a rectifier, and then it is converted back to AC from DC with
the use of an inverter. The end result is an output with a lower voltage and
variable (higher or lower) frequency.[9] Due to their wide area of application,
the AC/DC/AC converters are the most common contemporary solution. Other
advantages to AC/DC/AC converters is that they are stable in overload and no-
load conditions, as well as they can be disengaged from a load without damage.
[12]
Hybrid matrix converter: Hybrid matrix converters are relatively new for AC/AC
converters. These converters combine the AC/DC/AC design with the matrix
converter design. Multiple types of hybrid converters have been developed in
this new category, an example being a converter that uses uni-directional
switches and two converter stages without the dc-link; without the capacitors
or inductors needed for a dc-link, the weight and size of the converter is
reduced. Two sub-categories exist from the hybrid converters, named hybrid
direct matrix converter (HDMC) and hybrid indirect matrix converter (HIMC).
HDMC convert the voltage and current in one stage, while the HIMC utilizes
separate stages, like the AC/DC/AC converter, but without the use of an
intermediate storage element.[13][14]
Applications: Below is a list of common applications that each converter is
used in.
    * AC Voltage Controller: Lighting Control; Domestic and Industrial Heating;
      Speed Control of Fan,Pump or Hoist Drives, Soft Starting of Induction
      Motors, Static AC Switches[7] (Temperature Control, Transformer Tap
      Changing, etc.)
    * Cycloconverter: High-Power Low-Speed Reversible AC Motor Drives; Constant
      Frequency Power Supply with Variable Input Frequency; Controllable VAR
      Generators for Power Factor Correction; AC System Interties Linking Two
      Independent Power Systems.[7]
    * Matrix Converter: Currently the application of matrix converters are
      limited due to non-availability of bilateral monolithic switches capable
      of operating at high frequency, complex control law implementation,
      commutation and other reasons. With these developments, matrix converters
      could replace cycloconverters in many areas.[7]
    * DC Link: Can be used for individual or multiple load applications of
      machine building and construction.[12]
***** Simulations of power electronic systems[edit] *****
Output voltage of a full-wave rectifier with controlled thyristors
Power electronic circuits are simulated using computer simulation programs such
as PLECS, PSIM and MATLAB/simulink. Circuits are simulated before they are
produced to test how the circuits respond under certain conditions. Also,
creating a simulation is both cheaper and faster than creating a prototype to
use for testing.[15]
***** Applications[edit] *****
Applications of power electronics range in size from a switched_mode_power
supply in an AC_adapter, battery chargers, audio amplifiers, fluorescent_lamp
ballasts, through variable_frequency_drives and DC motor drives used to operate
pumps, fans, and manufacturing machinery, up to gigawatt-scale high_voltage
direct_current power transmission systems used to interconnect electrical
grids. Power electronic systems are found in virtually every electronic device.
For example:
    * DC/DC_converters are used in most mobile devices (mobile phones, PDA
      etc.) to maintain the voltage at a fixed value whatever the voltage level
      of the battery is. These converters are also used for electronic
      isolation and power_factor correction. A power_optimizer is a type of DC/
      DC converter developed to maximize the energy harvest from solar
      photovoltaic or wind_turbine systems.
    * AC/DC converters (rectifiers) are used every time an electronic device is
      connected to the mains (computer, television etc.). These may simply
      change AC to DC or can also change the voltage level as part of their
      operation.
    * AC/AC converters are used to change either the voltage level or the
      frequency (international power adapters, light dimmer). In power
      distribution networks AC/AC converters may be used to exchange power
      between utility_frequency 50 Hz and 60 Hz power grids.
    * DC/AC converters (inverters) are used primarily in UPS or renewable
      energy systems or emergency_lighting systems. Mains power charges the DC
      battery. If the mains fails, an inverter produces AC electricity at mains
      voltage from the DC battery. Solar_inverter, both smaller string and
      larger central inverters, as well as solar_micro-inverter are used in
      photovoltaics as a component of a PV system.
Motor drives are found in pumps, blowers, and mill drives for textile, paper,
cement and other such facilities. Drives may be used for power conversion and
for motion control.[16] For AC motors, applications include variable-frequency
drives, motor_soft_starters and excitation systems.[17]
In hybrid_electric_vehicles (HEVs), power electronics are used in two formats:
series hybrid and parallel hybrid. The difference between a series hybrid and a
parallel hybrid is the relationship of the electric motor to the internal
combustion_engine (ICE). Devices used in electric vehicles consist mostly of
dc/dc converters for battery charging and dc/ac converters to power the
propulsion motor. Electric_trains use power electronic devices to obtain power,
as well as for vector control using pulse_width_modulation (PWM) rectifiers.
The trains obtain their power from power lines. Another new usage for power
electronics is in elevator systems. These systems may use thyristors,
inverters, permanent_magnet motors, or various hybrid systems that incorporate
PWM systems and standard motors.[18]
**** Inverters[edit] ****
In general, inverters are utilized in applications requiring direct conversion
of electrical energy from DC to AC or indirect conversion from AC to AC. DC to
AC conversion is useful for many fields, including power conditioning, harmonic
compensation, motor drives, and renewable energy grid-integration.
In power systems it is often desired to eliminate harmonic content found in
line currents. VSIs can be used as active power filters to provide this
compensation. Based on measured line currents and voltages, a control system
determines reference current signals for each phase. This is fed back through
an outer loop and subtracted from actual current signals to create current
signals for an inner loop to the inverter. These signals then cause the
inverter to generate output currents that compensate for the harmonic content.
This configuration requires no real power consumption, as it is fully fed by
the line; the DC link is simply a capacitor that is kept at a constant voltage
by the control system.[5] In this configuration, output currents are in phase
with line voltages to produce a unity power factor. Conversely, VAR
compensation is possible in a similar configuration where output currents lead
line voltages to improve the overall power factor.[6]
In facilities that require energy at all times, such as hospitals and airports,
UPS systems are utilized. In a standby system, an inverter is brought online
when the normally supplying grid is interrupted. Power is instantaneously drawn
from onsite batteries and converted into usable AC voltage by the VSI, until
grid power is restored, or until backup generators are brought online. In an
online UPS system, a rectifier-DC-link-inverter is used to protect the load
from transients and harmonic content. A battery in parallel with the DC-link is
kept fully charged by the output in case the grid power is interrupted, while
the output of the inverter is fed through a low pass filter to the load. High
power quality and independence from disturbances is achieved.[5]
Various AC motor drives have been developed for speed, torque, and position
control of AC motors. These drives can be categorized as low-performance or as
high-performance, based on whether they are scalar-controlled or vector-
controlled, respectively. In scalar-controlled drives, fundamental stator
current, or voltage frequency and amplitude, are the only controllable
quantities. Therefore, these drives are employed in applications where high
quality control is not required, such as fans and compressors. On the other
hand, vector-controlled drives allow for instantaneous current and voltage
values to be controlled continuously. This high performance is necessary for
applications such as elevators and electric cars.[5]
Inverters are also vital to many renewable energy applications. In photovoltaic
purposes, the inverter, which is usually a PWM VSI, gets fed by the DC
electrical energy output of a photovoltaic module or array. The inverter then
converts this into an AC voltage to be interfaced with either a load or the
utility grid. Inverters may also be employed in other renewable systems, such
as wind turbines. In these applications, the turbine speed usually varies
causing changes in voltage frequency and sometimes in the magnitude. In this
case, the generated voltage can be rectified and then inverted to stabilize
frequency and magnitude.[5]
**** Smart grid[edit] ****
A smart_grid is a modernized electrical_grid that uses information_and
communications_technology to gather and act on information, such as information
about the behaviors of suppliers and consumers, in an automated fashion to
improve the efficiency, reliability, economics, and sustainability of the
production and distribution of electricity.[19][20]
Electric power generated by wind_turbines and hydroelectric turbines by using
induction_generators can cause variances in the frequency at which power is
generated. Power electronic devices are utilized in these systems to convert
the generated ac voltages into high-voltage direct current (HVDC). The HVDC
power can be more easily converted into three phase power that is coherent with
the power associated to the existing power grid. Through these devices, the
power delivered by these systems is cleaner and has a higher associated power
factor. Wind power systems optimum torque is obtained either through a gearbox
or direct drive technologies that can reduce the size of the power electronics
device.[21]
Electric power can be generated through photovoltaic_cells by using power
electronic devices. The produced power is usually then transformed by solar
inverters. Inverters are divided into three different types: central, module-
integrated and string. Central converters can be connected either in parallel
or in series on the DC side of the system. For photovoltaic "farms", a single
central converter is used for the entire system. Module-integrated converters
are connected in series on either the DC or AC side. Normally several modules
are used within a photovoltaic system, since the system requires these
converters on both DC and AC terminals. A string converter is used in a system
that utilizes photovoltaic cells that are facing different directions. It is
used to convert the power generated to each string, or line, in which the
photovoltaic cells are interacting.[21]
Power electronics can be used to help utilities adapt to the rapid increase in
distributed residential/commercial solar_power generation. Germany and parts of
Hawaii, California and New Jersey require costly studies to be conducted before
approving new solar installations. Relatively small-scale ground- or pole-
mounted devices create the potential for a distributed control infrastructure
to monitor and manage the flow of power. Traditional electromechanical systems,
such as capacitor_banks or voltage_regulators at substations, can take minutes
to adjust voltage and can be distant from the solar installations where the
problems originate. If voltage on a neighborhood circuit goes too high, it can
endanger utility crews and cause damage to both utility and customer equipment.
Further, a grid fault causes photovoltaic generators to shut down immediately,
spiking demand for grid power. Smart grid-based regulators are more
controllable than far more numerous consumer devices.[22]
In another approach, a group of 16 western utilities called the Western
Electric Industry Leaders called for mandatory use of "smart inverters". These
devices convert DC to household AC and can also help with power quality. Such
devices could eliminate the need for expensive utility equipment upgrades at a
much lower total cost.[22]
***** Notes[edit] *****
   1. ^Thompson, M.T. "Notes_01" (PDF). Introduction to Power Electronics.
      Thompson Consulting, Inc.
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
   3. ^Kharagpur. "Power_Semiconductor_Devices" (PDF). EE IIT. Retrieved 25
      March 2012.
   4. ^"Rethink_Power_Density_with_GaN". Electronic_Design. 21 April 2017.
      Retrieved 23 July 2019.
   5. ^ Muhammad H. Rashid,POWER ELECTRONICS HANDBOOK DEVICES, CIRCUITS, AND
      APPLICATIONS Third Edition The structure introduced in this work is a
      multilevel inverter, which uses Separate DC Sources. The multilevel
      inverter using cascaded-inverter with SDCS synthesizes a desired voltage
      from several independent sources of DC voltages, which may be obtained
      from batteries, fuel cells, or solar cells. This configuration recently
      becomes very popular in AC power supply and adjustable speed drive
      applications. This new inverter can avoid extra clamping diodes or
      voltage balancing capacitors.Butterworth-Heinemann,2007
   6. ISBN 978-0-12-382036-5
   7. ^ a b c d e f g h i j k l m n o p q r s t u v w x y z aa ab ac ad
      aeRashid, M.H. (2001). Power Electronics Handbook. Academic Press.
      pp. 225â250.
   8. ^ a b c d e f g h iTrzynadlowski, A.M. (2010). Introduction to Modern
      Power Electronics. Wiley. pp. 269â341.
   9. ^ a b c d e fRahsid, M.H. (2010). Power Electronics Handbook: Devices,
      Circuits, and Applications. Elsevier. pp. 147â564. ISBN 978-0-12-
      382036-5.
  10. ^Skvarenina, T.L. (2002). The power electronics handbook Industrial
      electronics series. CRC Press. pp. 94â140. ISBN 978-0-8493-7336-7.
  11. ^ a b c dRashid, M.H. (2005). Digital power electronics and applications
      Electronics & Electrical. Academic Press. ISBN 978-0-12-088757-6.
  12. ^Tolbert, L.M. "CYCLOCONVERTERS". University of Tennessee. Retrieved 23
      March 2012.
  13. ^Klumpner, C. "Power_Electronics_2". Retrieved 23 March 2012.
  14. ^ a bVodovozov, V (2006). Electronic engineering. ISBN 978-9985-69-039-0.
  15. ^Lipo; Kim, Sul (2000). "AC/AC Power Conversion Based on Matric Converter
      Topology with Unidirectional Switches". IEEE Transactions on Industry
      Applications. 36 (1): 139â145. doi:10.1109/28.821808.
  16. ^Wheeler; Wijekoon, Klumpner (July 2008). "Implementation_of_a_Hybrid_AC/
      AC_Direct_Power_Converter_with_Unity_Voltage_Transfer_Ratio" (PDF). IEEE
      Transactions on Power Electronics. 23 (4): 1918â1986. doi:10.1109/
      tpel.2008.924601.
  17. ^Khader, S. "THE_APPLICATION_OF_PSIM_&_MATLAB/_SIMULINK_IN_POWER
      ELECTRONICS_COURSES" (PDF). Retrieved 25 March 2012.
  18. ^Bose, Bimal K. (SeptemberâOctober 1993). "Power Electronics and Motion
      Control â Technology Status and Recent Trends".
  19. ^Bose, Bimal K. (February 2009). "Power Electronics and Motor Drives
      Recent Progress and Perspective".
  20. ^Yano, Masao; Shigery Abe; Eiichi Ohno (2004). "History of Power
      Electronics for Motor Drives in Japan".
  21. ^D. J. Hammerstrom; et al. "Pacific_Northwest_GridWiseâ¢_Testbed
      Demonstration_Projects,_Part_I._Olympic_Peninsula_Project" (PDF).
      Retrieved 2014-01-15.
  22. ^U.S. Department of Energy. "Smart_Grid_/_Department_of_Energy".
      Retrieved 2012-06-18.
  23. ^ a bCarrasco, Juan Manuel; Leopoldo Garcia Franquelo; Jan T.
      Bialasiewecz; Eduardo Galvan; Ramon C. Portillo Guisado; Ma. Angeles
      Martin Prats; Jose Ignacio Leon; Narciso Moreno-Alfonso (August 2006).
      "Power-Electronic Systems for the Grid Integration of Renewable Sources:
      A Survey". 53 (4): 1002. CiteSeerX 10.1.1.116.5024. doi:10.1109/
      tie.2006.878356.
  24. ^ a bLaMonica, Martin (2014-01-21). "Power_Electronics_Could_Help_Grid
      and_Solar_Power_Get_Along_|_MIT_Technology_Review". Technologyreview.com.
      Retrieved 2014-01-22.
***** References[edit] *****
    * Issa Batarseh, "Power Electronic Circuits" by John Wiley, 2003.
    * S.K. Mazumder, "High-Frequency Inverters: From Photovoltaic, Wind, and
      Fuel-Cell based Renewable- and Alternative-Energy DER/DG Systems to
      Battery based Energy-Storage Applications", Book Chapter in Power
      Electronics handbook, Editor M.H. Rashid, Academic Press, Burlington,
      Massachusetts, 2010.
    * V. Gureich "Electronic Devices on Discrete Components for Industrial and
      Power Engineering", CRC Press, New York, 2008, 418 p.
    * Editor: Semikron, Authors: Dr. Ulrich Nicolai, Dr. Tobias Reimann, Prof.
      JÃ¼rgen Petzoldt, Josef Lutz: Application Manual IGBT- and MOSFET-power
      modules, 1. edition, ISLE Verlag, 1998,
ISBN 3-932633-24-5 online_version
R. W. Erickson, D. Maksimovic, Fundamentals of Power Electronics, 2nd Ed.,
Springer, 2001,
ISBN 0-7923-7270-0 [1]
Arendt Wintrich; Ulrich Nicolai; Werner Tursky; Tobias Reimann (2010),
Applikationshandbuch_2010 (PDF-Version) (in German) (2. ed.), ISLE Verlag,
ISBN 978-3-938843-56-7
Arendt Wintrich; Ulrich Nicolai; Werner Tursky; Tobias Reimann (2011),
Application_Manual_2011 (PDF) (in German) (2. ed.), ISLE Verlag, ISBN 978-3-
938843-66-6, archived from the_original (PDF-Version) on 2013-09-03
***** External links[edit] *****
    * [icon]Electronics_portal
    * Technology_portal
 Wikimedia Commons has media related to Power_electronics.
Authority_control [Edit_this_at_Wikidata]     * NDL: 00997584

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Power_electronics&oldid=908720626"
Categories:
    * Power_electronics
Hidden categories:
    * Articles_needing_cleanup_from_March_2018
    * All_pages_needing_cleanup
    * Cleanup_tagged_articles_with_a_reason_field_from_March_2018
    * Wikipedia_pages_needing_cleanup_from_March_2018
    * Articles_lacking_in-text_citations_from_December_2013
    * All_articles_lacking_in-text_citations
    * All_articles_with_vague_or_ambiguous_time
    * Vague_or_ambiguous_time_from_March_2012
    * CS1_German-language_sources_(de)
    * Commons_category_link_is_on_Wikidata
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * Magyar
    * áá¼ááºáá¬áá¬áá¬
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 31 July 2019, at 14:55 (UTC).
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
