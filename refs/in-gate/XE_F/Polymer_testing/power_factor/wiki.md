The following text has been accessed from https://en.wikipedia.org/wiki/Power_factor at Fri Aug 9 03:02:52 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Power factor ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For the firearms cartridge ranking system, see Power_factor_(shooting_sports).
In electrical_engineering, the power factor of an AC electrical power system is
defined as the ratio of the real_power absorbed by the load to the apparent
power flowing in the circuit, and is a dimensionless_number in the closed
interval of â1 to 1. A power factor of less than one indicates the voltage
and current are not in phase, reducing the instantaneous product of the two.
Real_power is the instantaneous product of voltage and current and represents
the capacity of the electricity for performing work. Apparent power is the
average product of current and voltage. Due to energy stored in the load and
returned to the source, or due to a non-linear load that distorts the wave
shape of the current drawn from the source, the apparent power may be greater
than the real power. A negative power factor occurs when the device (which is
normally the load) generates power, which then flows back towards the source.
In an electric power system, a load with a low power factor draws more current
than a load with a high power factor for the same amount of useful power
transferred. The higher currents increase the energy lost in the distribution
system, and require larger wires and other equipment. Because of the costs of
larger equipment and wasted energy, electrical utilities will usually charge a
higher cost to industrial or commercial customers where there is a low power
factor.
Power-factor correction increases the power factor of a load, improving
efficiency for the distribution system to which it is attached. Linear loads
with low power factor (such as induction_motors) can be corrected with a
passive network of capacitors or inductors. Non-linear loads, such as
rectifiers, distort the current drawn from the system. In such cases, active or
passive power factor correction may be used to counteract the distortion and
raise the power factor. The devices for correction of the power factor may be
at a central substation, spread out over a distribution system, or built into
power-consuming equipment.
⁰
***** Contents *****
    * 1_Linear_circuits
          o 1.1_Definition_and_calculation
                # 1.1.1_Power_triangle
                # 1.1.2_Increasing_the_power_factor
                # 1.1.3_Decreasing_the_power_factor
                # 1.1.4_Lagging_and_leading_power_factors
          o 1.2_Power_factor_correction_of_linear_loads
    * 2_Non-linear_loads
          o 2.1_Non-sinusoidal_components
          o 2.2_Distortion_power_factor
          o 2.3_Distortion_in_three-phase_networks
          o 2.4_Switched-mode_power_supplies
          o 2.5_Power_factor_correction_(PFC)_in_non-linear_loads
                # 2.5.1_Passive_PFC
                # 2.5.2_Active_PFC
                # 2.5.3_Dynamic_PFC
    * 3_Importance_in_distribution_systems
    * 4_Measurement_techniques
    * 5_Mnemonics
    * 6_References
    * 7_External_links
***** Linear circuits[edit] *****
Instantaneous and average power calculated from AC voltage and current with a
zero power factor (Ï = 90Â°, cos(Ï) = 0). The blue line shows all the power
is stored temporarily in the load during the first quarter cycle and returned
to the grid during the second quarter cycle, so no real power is consumed.
Instantaneous and average power calculated from AC voltage and current with a
lagging power factor (Ï = 45Â°, cos(Ï) â 0.71). The blue line shows some of
the power is returned to the grid during the part of the cycle labeled Ï.
In a purely resistive AC circuit, voltage and current waveforms are in step (or
in_phase), changing polarity at the same instant in each cycle. All the power
entering the load is consumed (or dissipated).
Where reactive loads are present, such as with capacitors or inductors, energy
storage in the loads results in a phase difference between the current and
voltage waveforms. During each cycle of the AC voltage, extra energy, in
addition to any energy consumed in the load, is temporarily stored in the load
in electric or magnetic_fields, and then returned to the power grid a fraction
of the period later.
In the electric_power_grid, reactive loads thus cause a continuous "ebb and
flow" of nonproductive power. A circuit with a low power factor will use higher
currents to transfer a given quantity of real power than a circuit with a high
power factor, causing increased losses due to resistive_heating in power lines,
and requiring higher rated conductors and transformers be installed. A linear
load does not change the shape of the waveform of the current, but may change
the relative timing (phase) between voltage and current.
Electrical circuits containing dominantly resistive loads (incandescent lamps,
heating elements) have a power factor of almost 1.0, but circuits containing
inductive or capacitive loads (electric motors, solenoid valves, transformers,
fluorescent_lamp_ballasts, and others) can have a power factor well below 1.
**** Definition and calculation[edit] ****
AC_power flow has two components:
    * Real power or active power (    P   {\displaystyle P}  [P]) (sometimes
      called average power[1]), expressed in watts (W)
    * Reactive power (    Q   {\displaystyle Q}  [Q]), usually expressed in
      reactive_volt-amperes (var)[2]
These are combined to the complex power (    S   {\displaystyle S}  [S])
expressed volt-amperes (VA). The magnitude of the complex power is the apparent
power (     |  S  |    {\displaystyle |S|}  [|S|]), also expressed in volt-
amperes (VA).
The VA and var are non-SI units mathematically identical to the watt, but are
used in engineering practice instead of the watt to state what quantity is
being expressed. The SI explicitly disallows using units for this purpose or as
the only source of information about a physical quantity as used.[3]
The power factor is defined as the ratio of real power to apparent power. As
power is transferred along a transmission line, it does not consist purely of
real power that can do work once transferred to the load, but rather consists
of a combination of real and reactive power, called apparent power. The power
factor describes the amount of real power transmitted along a transmission line
relative to the total apparent power flowing in the line.[4][5]
*** Power triangle[edit] ***
[Power_triangle_diagram.jpg]
One can relate the various components of AC power by using the power triangle
in vector space. Real power extends horizontally in the Ã® direction as it
represents a purely real component of AC power. Reactive power extends in the
direction of Äµ as it represents a purely imaginary component of AC power.
Complex power (and its magnitude, Apparent power) represents a combination of
both real and reactive power, and therefore can be calculated by using the
vector sum of these two components. We can conclude that the mathematical
relationship between these components is:
             S    = P + j Q      |  S   |   2      =  P  2   +  Q  2        |
      S  |     =    P  2   +  Q  2         cos &#x2061; &#x03B8;  , power
      factor     =    P  , real power     |  S  |   , apparent power
      or      p o w e r f a c t o r    =  cos(atan(Q/P))       it follows that.
      . .      Q    = P &#x2217; T a n ( A c o s ( p o w e r f a c t o r ) )
      {\displaystyle {\begin{aligned}S&=P+jQ\\|S|^{2}&=P^{2}+Q^{2}\\[3pt]|S|&=
      {\sqrt {P^{2}+Q^{2}}}\\\cos \theta {\text{, power factor}}&={\frac {P
      {\text{, real power}}}{|S|{\text{, apparent power}}}}\\{\text
      {or}}\\powerfactor&={\text{cos(atan(Q/P))}}\\{\text{it follows that. .
      .}}\\Q&=P*Tan(Acos(powerfactor))\end{aligned}}}  [{\displaystyle {\begin
      {aligned}S&=P+jQ\\|S|^{2}&=P^{2}+Q^{2}\\[3pt]|S|&={\sqrt {P^{2}+Q^
      {2}}}\\\cos \theta {\text{, power factor}}&={\frac {P{\text{, real
      power}}}{|S|{\text{, apparent power}}}}\\{\text{or}}\\powerfactor&={\text
      {cos(atan(Q/P))}}\\{\text{it follows that. . .}}\\Q&=P*Tan(Acos
      (powerfactor))\end{aligned}}}]
*** Increasing the power factor[edit] ***
[Increased_power_factor.jpg]
As the power factor (i.e. cos Î¸) increases, the ratio of real power to
apparent power (which = cos Î¸), increases and approaches unity (1), while the
angle Î¸ decreases and the reactive power decreases. [As cos Î¸ â 1, its
maximum possible value, Î¸ â 0 and so Q â 0, as the load becomes less
reactive and more purely resistive].
*** Decreasing the power factor[edit] ***
[Decreased_power_factor.jpg]
As the power factor decreases, the ratio of real power to apparent power also
decreases, as the angle Î¸ increases and reactive power increases.
*** Lagging and leading power factors[edit] ***
There is also a difference between a lagging and leading power factor. The
terms refer to whether the phase of the current is leading or lagging the phase
of the voltage. A lagging power factor signifies that the load is inductive, as
the load will âconsumeâ reactive power, and therefore the reactive
component     Q   {\displaystyle Q}  [Q] is positive as reactive power travels
through the circuit and is âconsumedâ by the inductive load. A leading
power factor signifies that the load is capacitive, as the load âsuppliesâ
reactive power, and therefore the reactive component     Q   {\displaystyle Q}
[Q] is negative as reactive power is being supplied to the circuit.
[Lagging-Leading.jpg]
If Î¸ is the phase_angle between the current and voltage, then the power factor
is equal to the cosine of the angle,     cos &#x2061; &#x03B8;   {\displaystyle
\cos \theta }  [\cos \theta ]:
          |  P  |  =  |  S  |  cos &#x2061; &#x03B8;   {\displaystyle
      |P|=|S|\cos \theta }  [|P|=|S|\cos \theta ]
Since the units are consistent, the power factor is by definition a
dimensionless_number between â1 and 1. When power factor is equal to 0, the
energy flow is entirely reactive and stored energy in the load returns to the
source on each cycle. When the power factor is 1, all the energy supplied by
the source is consumed by the load. Power factors are usually stated as
"leading" or "lagging" to show the sign of the phase angle. Capacitive loads
are leading (current leads voltage), and inductive loads are lagging (current
lags voltage).
If a purely resistive load is connected to a power supply, current and voltage
will change polarity in step, the power factor will be 1, and the electrical
energy flows in a single direction across the network in each cycle. Inductive
loads such as induction motors (any type of wound coil) consume reactive power
with current waveform lagging the voltage. Capacitive loads such as capacitor
banks or buried cable generate reactive power with current phase leading the
voltage. Both types of loads will absorb energy during part of the AC cycle,
which is stored in the device's magnetic or electric field, only to return this
energy back to the source during the rest of the cycle.
For example, to get 1 kW of real power, if the power factor is unity, 1 kVA of
apparent power needs to be transferred (1 kW Ã· 1 = 1 kVA). At low values of
power factor, more apparent power needs to be transferred to get the same real
power. To get 1 kW of real power at 0.2 power factor, 5 kVA of apparent power
needs to be transferred (1 kW Ã· 0.2 = 5 kVA). This apparent power must be
produced and transmitted to the load, and is subject to the losses in the
production and transmission processes.
Electrical loads consuming alternating_current_power consume both real power
and reactive power. The vector sum of real and reactive power is the apparent
power. The presence of reactive power causes the real power to be less than the
apparent power, and so, the electric load has a power factor of less than 1.
A negative power factor (0 to â1) can result from returning power to the
source, such as in the case of a building fitted with solar panels when surplus
power is fed back into the supply.[6][7][8]
**** Power factor correction of linear loads[edit] ****
A high power factor is generally desirable in a power delivery system to reduce
losses and improve voltage regulation at the load. Compensating elements near
an electrical load will reduce the apparent power demand on the supply system.
Power factor correction may be applied by an electric_power_transmission
utility to improve the stability and efficiency of the network. Individual
electrical customers who are charged by their utility for low power factor may
install correction equipment to increase their power factor so as to reduce
costs.
Power factor correction brings the power factor of an AC power circuit closer
to 1 by supplying or absorbing reactive power, adding capacitors or inductors
that act to cancel the inductive or capacitive effects of the load,
respectively. In the case of offsetting the inductive effect of motor loads,
capacitors can be locally connected. These capacitors help to generate reactive
power to meet the demand of the inductive loads. This will keep that reactive
power from having to flow all the way from the utility generator to the load.
In the electricity industry, inductors are said to consume reactive power and
capacitors are said to supply it, even though reactive power is just energy
moving back and forth on each AC cycle.
The reactive elements in power factor correction devices can create voltage
fluctuations and harmonic noise when switched on or off. They will supply or
sink reactive power regardless of whether there is a corresponding load
operating nearby, increasing the system's no-load losses. In the worst case,
reactive elements can interact with the system and with each other to create
resonant conditions, resulting in system instability and severe overvoltage
fluctuations. As such, reactive elements cannot simply be applied without
engineering analysis.
1. Reactive_Power_Control_Relay; 2. Network connection points; 3. Slow-blow
Fuses; 4. Inrush Limiting Contactors; 5. Capacitors (single-phase or three-
phase units, delta-connection); 6. Transformer (for controls and ventilation
fans)
An automatic power factor correction unit consists of a number of capacitors
that are switched by means of contactors. These contactors are controlled by a
regulator that measures power factor in an electrical network. Depending on the
load and power factor of the network, the power factor controller will switch
the necessary blocks of capacitors in steps to make sure the power factor stays
above a selected value.
In place of a set of switched capacitors, an unloaded synchronous_motor can
supply reactive power. The reactive_power drawn by the synchronous motor is a
function of its field excitation. It is referred to as a synchronous_condenser.
It is started and connected to the electrical_network. It operates at a leading
power factor and puts vars onto the network as required to support a system's
voltage or to maintain the system power factor at a specified level.
The synchronous condenser's installation and operation are identical to those
of large electric_motors. Its principal advantage is the ease with which the
amount of correction can be adjusted; it behaves like a variable capacitor.
Unlike with capacitors, the amount of reactive power supplied is proportional
to voltage, not the square of voltage; this improves voltage stability on large
networks. Synchronous condensers are often used in connection with high-voltage
direct-current transmission projects or in large industrial plants such as
steel_mills.
For power factor correction of high-voltage power systems or large, fluctuating
industrial loads, power electronic devices such as the Static_VAR_compensator
or STATCOM are increasingly used. These systems are able to compensate sudden
changes of power factor much more rapidly than contactor-switched capacitor
banks, and being solid-state require less maintenance than synchronous
condensers.
***** Non-linear loads[edit] *****
Examples of non-linear loads on a power system are rectifiers (such as used in
a power supply), and arc discharge devices such as fluorescent_lamps, electric
welding machines, or arc_furnaces. Because current in these systems is
interrupted by a switching action, the current contains frequency components
that are multiples of the power system frequency. Distortion power factor is a
measure of how much the harmonic distortion of a load current decreases the
average power transferred to the load.
Sinusoidal voltage and non-sinusoidal current give a distortion power factor of
0.75 for this computer power supply load.
**** Non-sinusoidal components[edit] ****
In linear circuits having only sinusoidal currents and voltages of one
frequency, the power factor arises only from the difference in phase between
the current and voltage. This is "displacement power factor".[9]
Non-linear loads change the shape of the current waveform from a sine_wave to
some other form. Non-linear loads create harmonic currents in addition to the
original (fundamental frequency) AC current. This is of importance in practical
power systems that contain non-linear loads such as rectifiers, some forms of
electric lighting, electric_arc_furnaces, welding equipment, switched-mode
power_supplies, variable speed drives and other devices. Filters consisting of
linear capacitors and inductors can prevent harmonic currents from entering the
supplying system.
To measure the real power or reactive power, a wattmeter designed to work
properly with non-sinusoidal currents must be used.
**** Distortion power factor[edit] ****
The distortion power factor is the distortion component associated with the
harmonic voltages and currents present in the system.
               distortion power factor      =    I  1    I  r m s           =
      I  1     I  1   2   +  I  2   2   +  I  3   2   +  I  4   2   + &#x22EF;
      =   1  1 +     I  2   2   +  I  3   2   +  I  4   2   + &#x22EF;   I  1
      2              =   1  1 + T H  D  i   2            {\displaystyle {\begin
      {aligned}{\mbox{distortion power factor}}&={\frac {I_{1}}{I_{rms}}}\\&=
      {\frac {I_{1}}{\sqrt {I_{1}^{2}+I_{2}^{2}+I_{3}^{2}+I_{4}^{2}+\cdots
      }}}\\&={\frac {1}{\sqrt {1+{\frac {I_{2}^{2}+I_{3}^{2}+I_{4}^{2}+\cdots }
      {I_{1}^{2}}}}}}\\&={\frac {1}{\sqrt {1+THD_{i}^{2}}}}\\\end{aligned}}}  [
      {\displaystyle {\begin{aligned}{\mbox{distortion power factor}}&={\frac
      {I_{1}}{I_{rms}}}\\&={\frac {I_{1}}{\sqrt {I_{1}^{2}+I_{2}^{2}+I_{3}^
      {2}+I_{4}^{2}+\cdots }}}\\&={\frac {1}{\sqrt {1+{\frac {I_{2}^{2}+I_{3}^
      {2}+I_{4}^{2}+\cdots }{I_{1}^{2}}}}}}\\&={\frac {1}{\sqrt {1+THD_{i}^
      {2}}}}\\\end{aligned}}}]
      THD    i     {\displaystyle {\mbox{THD}}_{i}}  [{\mbox{THD}}_{i}] is the
total_harmonic_distortion of the load current.
         T H  D  i   =      &#x2211;  h = 2   &#x221E;    I  h   2      I  1
      =     I  2   2   +  I  3   2   +  I  4   2   + &#x22EF;   I  1
      {\displaystyle THD_{i}={\frac {\sqrt {\displaystyle \sum _{h=2}^{\infty
      }I_{h}^{2}}}{I_{1}}}={\frac {\sqrt {I_{2}^{2}+I_{3}^{2}+I_{4}^{2}+\cdots
      }}{I_{1}}}}  [{\displaystyle THD_{i}={\frac {\sqrt {\displaystyle \sum _
      {h=2}^{\infty }I_{h}^{2}}}{I_{1}}}={\frac {\sqrt {I_{2}^{2}+I_{3}^{2}+I_
      {4}^{2}+\cdots }}{I_{1}}}}]
    I  1     {\displaystyle I_{1}}  [I_{1}] is the fundamental component of the
current and      I   rms      {\displaystyle I_{\mbox{rms}}}  [I_{\mbox{rms}}]
is the total current â both are root_mean_square-values (distortion power
factor can also be used to describe individual order harmonics, using the
corresponding current in place of total current). This definition with respect
to total harmonic distortion assumes that the voltage stays undistorted
(sinusoidal, without harmonics). This simplification is often a good
approximation for stiff voltage sources (not being affected by changes in load
downstream in the distribution network). Total harmonic distortion of typical
generators from current distortion in the network is on the order of 1â2%,
which can have larger scale implications but can be ignored in common practice.
[10]
The result when multiplied with the displacement power factor (DPF) is the
overall, true power factor or just power factor (PF):
           PF   =    cos &#x2061;  &#x03C6;    1 + T H  D  i   2
      {\displaystyle {\mbox{PF}}={\frac {\cos {\varphi }}{\sqrt {1+THD_{i}^
      {2}}}}}  [{\displaystyle {\mbox{PF}}={\frac {\cos {\varphi }}{\sqrt
      {1+THD_{i}^{2}}}}}]
**** Distortion in three-phase networks[edit] ****
In practice, the local effects of distortion current on devices in a three-
phase_distribution_network rely on the magnitude of certain order harmonics
rather than the total harmonic distortion.
For example, the triplen, or zero-sequence, harmonics (3rd, 9th, 15th, etc.)
have the property of being in-phase when compared line-to-line. In a delta-wye
transformer, these harmonics can result in circulating currents in the delta
windings and result in greater resistive_heating. In a wye-configuration of a
transformer, triplen harmonics will not create these currents, but they will
result in a non-zero current in the neutral_wire. This could overload the
neutral wire in some cases and create error in kilowatt-hour metering systems
and billing revenue.[11][12] The presence of current harmonics in a transformer
also result in larger eddy_currents in the magnetic core of the transformer.
Eddy current losses generally increase as the square of the frequency, lowering
the transformer's efficiency, dissipating additional heat, and reducing its
service life.[13]
Negative-sequence harmonics (5th, 11th, 17th, etc.) combine 120 degrees out of
phase, similarly to the fundamental harmonic but in a reversed sequence. In
generators and motors, these currents produce magnetic fields which oppose the
rotation of the shaft and sometimes result in damaging mechanical vibrations.
[14]
**** Switched-mode power supplies[edit] ****
Main article: switched-mode_power_supply_Â§ Power_factor
A particularly important class of non-linear loads is the millions of personal
computers that typically incorporate switched-mode_power_supplies (SMPS) with
rated output power ranging from a few watts to more than 1 kW. Historically,
these very-low-cost power supplies incorporated a simple full-wave rectifier
that conducted only when the mains instantaneous voltage exceeded the voltage
on the input capacitors. This leads to very high ratios_of_peak-to-average
input current, which also lead to a low distortion power factor and potentially
serious phase and neutral loading concerns.
A typical switched-mode power supply first converts the AC mains to a DC bus by
means of a bridge_rectifier or a similar circuit. The output voltage is then
derived from this DC bus. The problem with this is that the rectifier is a non-
linear device, so the input current is highly non-linear. That means that the
input current has energy at harmonics of the frequency of the voltage.
This presents a particular problem for the power companies, because they cannot
compensate for the harmonic current by adding simple capacitors or inductors,
as they could for the reactive power drawn by a linear load. Many jurisdictions
are beginning to legally require power factor correction for all power supplies
above a certain power level.
Regulatory agencies such as the EU have set harmonic limits as a method of
improving power factor. Declining component cost has hastened implementation of
two different methods. To comply with current EU standard EN61000-3-2, all
switched-mode power supplies with output power more than 75 W must include
passive power factor correction, at least. 80_Plus power supply certification
requires a power factor of 0.9 or more.[15]
**** Power factor correction (PFC) in non-linear loads[edit] ****
*** Passive PFC[edit] ***
The simplest way to control the harmonic current is to use a filter that passes
current only at line_frequency (50 or 60 Hz). The filter consists of capacitors
or inductors, and makes a non-linear device look more like a linear load. An
example of passive PFC is a valley-fill_circuit.
A disadvantage of passive PFC is that it requires larger inductors or
capacitors than an equivalent power active PFC circuit.[16][17][18] Also, in
practice, passive PFC is often less effective at improving the power factor.
[19][20][21][22][23]
*** Active PFC[edit] ***
Specifications taken from the packaging of a 610 W PC_power_supply showing
active PFC rating
Active PFC is the use of power_electronics to change the waveform of current
drawn by a load to improve the power factor.[24] Some types of the active PFC
are buck, boost, buck-boost and synchronous_condenser. Active power factor
correction can be single-stage or multi-stage.
In the case of a switched-mode power supply, a boost_converter is inserted
between the bridge rectifier and the main input capacitors. The boost converter
attempts to maintain a constant DC bus voltage on its output while drawing a
current that is always in phase with and at the same frequency as the line
voltage. Another switched-mode converter inside the power supply produces the
desired output voltage from the DC bus. This approach requires additional
semiconductor switches and control electronics, but permits cheaper and smaller
passive components. It is frequently used in practice.
For a three-phase SMPS, the Vienna_rectifier configuration may be used to
substantially improve the power factor.
SMPSs with passive PFC can achieve power factor of about 0.7â0.75, SMPSs with
active PFC, up to 0.99 power factor, while a SMPS without any power factor
correction have a power factor of only about 0.55â0.65.[25]
Due to their very wide input voltage range, many power supplies with active PFC
can automatically adjust to operate on AC power from about 100 V (Japan) to
240 V (Europe). That feature is particularly welcome in power supplies for
laptops.
*** Dynamic PFC[edit] ***
Dynamic power factor correction (DPFC), sometimes referred to as "real-time
power factor correction," is used for electrical stabilization in cases of
rapid load changes (e.g. at large manufacturing sites). DPFC is useful when
standard power factor correction would cause over or under correction.[26] DPFC
uses semiconductor switches, typically thyristors, to quickly connect and
disconnect capacitors or inductors to improve power factor.
***** Importance in distribution systems[edit] *****
75 MVAr capacitor bank in a 150 kV substation
Power factors below 1.0 require a utility to generate more than the minimum
volt-amperes necessary to supply the real power (watts). This increases
generation and transmission costs. For example, if the load power factor were
as low as 0.7, the apparent power would be 1.4 times the real power used by the
load. Line current in the circuit would also be 1.4 times the current required
at 1.0 power factor, so the losses in the circuit would be doubled (since they
are proportional to the square of the current). Alternatively, all components
of the system such as generators, conductors, transformers, and switchgear
would be increased in size (and cost) to carry the extra current. When the
power factor is close to unity, for the same KVA rating of the transformer more
load can be connected.[27]
Utilities typically charge additional costs to commercial customers who have a
power factor below some limit, which is typically 0.9 to 0.95. Engineers are
often interested in the power factor of a load as one of the factors that
affect the efficiency of power transmission.
With the rising cost of energy and concerns over the efficient delivery of
power, active PFC has become more common in consumer electronics.[28] Current
Energy_Star guidelines for computers[29] call for a power factor of â¥ 0.9 at
100% of rated output in the PC's_power_supply. According to a white paper
authored by Intel and the U.S._Environmental_Protection_Agency, PCs with
internal power supplies will require the use of active power factor correction
to meet the ENERGY STAR 5.0 Program Requirements for Computers.[30]
In Europe, EN_61000-3-2 requires power factor correction be incorporated into
consumer products.
Small customers, such as households, are not usually charged for reactive power
and so power factor metering equipment for such customers will not be
installed.
***** Measurement techniques[edit] *****
The power factor in a single-phase circuit (or balanced three-phase circuit)
can be measured with the wattmeter-ammeter-voltmeter method, where the power in
watts is divided by the product of measured voltage and current. The power
factor of a balanced polyphase circuit is the same as that of any phase. The
power factor of an unbalanced poly phase circuit is not uniquely defined.
A direct reading power factor meter can be made with a moving_coil_meter of the
electrodynamic type, carrying two perpendicular coils on the moving part of the
instrument. The field of the instrument is energized by the circuit current
flow. The two moving coils, A and B, are connected in parallel with the circuit
load. One coil, A, will be connected through a resistor and the second coil, B,
through an inductor, so that the current in coil B is delayed with respect to
current in A. At unity power factor, the current in A is in phase with the
circuit current, and coil A provides maximum torque, driving the instrument
pointer toward the 1.0 mark on the scale. At zero power factor, the current in
coil B is in phase with circuit current, and coil B provides torque to drive
the pointer towards 0. At intermediate values of power factor, the torques
provided by the two coils add and the pointer takes up intermediate positions.
[31]
Another electromechanical instrument is the polarized-vane type.[32] In this
instrument a stationary field coil produces a rotating magnetic field, just
like a polyphase motor. The field coils are connected either directly to
polyphase voltage sources or to a phase-shifting reactor if a single-phase
application. A second stationary field coil, perpendicular to the voltage
coils, carries a current proportional to current in one phase of the circuit.
The moving system of the instrument consists of two vanes that are magnetized
by the current coil. In operation the moving vanes take up a physical angle
equivalent to the electrical angle between the voltage source and the current
source. This type of instrument can be made to register for currents in both
directions, giving a four-quadrant display of power factor or phase angle.
Digital instruments exist that directly measure the time lag between voltage
and current waveforms. Low-cost instruments of this type measure the peak of
the waveforms. More sophisticated versions measure the peak of the fundamental
harmonic only, thus giving a more accurate reading for phase angle on distorted
waveforms. Calculating power factor from voltage and current phases is only
accurate if both waveforms are sinusoidal.[33]
Power Quality Analyzers, often referred to as Power Analyzers, make a digital
recording of the voltage and current waveform (typically either one phase or
three phase) and accurately calculate true power (watts), apparent power (VA)
power factor, AC voltage, AC current, DC voltage, DC current, frequency,
IEC61000-3-2/3-12 Harmonic measurement, IEC61000-3-3/3-11 flicker measurement,
individual phase voltages in delta applications where there is no neutral line,
total harmonic distortion, phase and amplitude of individual voltage or current
harmonics, etc.[34][35]
***** Mnemonics[edit] *****
English-language power engineering students are advised to remember: "ELI the
ICE man" or "ELI on ICE" â the voltage E leads the current I in an inductor
L; the current leads the voltage in a capacitor C.
Another common mnemonic is CIVIL â in a capacitor (C) the current (I) leads
voltage (V), voltage (V) leads current (I) in an inductor (L).
***** References[edit] *****
   1. ^Boylestad, Robert (2002-03-04). Introductory Circuit Analysis (10th
      ed.). p. 857. ISBN 978-0-13-097417-4.
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
   3. ^"SI_Units_â_Electricity_and_Magnetism". CH: International
      Electrotechnical Commission. Archived from the_original on 2007-12-11.
      Retrieved 14 June 2013.
   4. ^The_International_System_of_Units_(SI)_[SI_brochure] (PDF). Â§ 5.3.2
      (p. 132, 40 in the PDF file): BIPM. 2006.
   5. ^Authoritative Dictionary of Standards Terms (7th ed.), IEEE, 2000,
      ISBN 978-0-7381-2601-2, Std. 100
   6. .
   7. ^Trial-Use Standard Definitions for the Measurement of Electric Power
      Quantities Under Sinusoidal, Nonsinusoidal, Balanced, or Unbalanced
      Conditions, IEEE, 2000, ISBN 978-0-7381-1963-2, Std. 1459â2000
   8. . Note 1, section 3.1.1.1, when defining the quantities for power factor,
      asserts that real power only flows to the load and can never be negative.
      As of 2013, one of the authors acknowledged that this note was incorrect,
      and is being revised for the next edition. See http://powerstandards.com/
      Shymanski/draft.pdf
   9. ^Duddell, W. (1901), "On the resistance and electromotive forces of the
      electric arc", Philosophical Transactions of the Royal Society A:
      Mathematical, Physical and Engineering Sciences, 203 (359â371):
      512â15, doi:10.1098/rsta.1904.0022, The fact that the solid arc has, at
      low frequencies, a negative power factor, indicates that the arc is
      supplying power to the alternatorâ¦
  10. ^Zhang, S. (July 2006), "Analysis of some measurement issues in bushing
      power factor tests in the field", IEEE Transactions on Power Delivery, 21
      (3): 1350â56, doi:10.1109/tpwrd.2006.874616, â¦(the measurement) gives
      both negative power factor and negative resistive current (power loss)
  11. ^Almarshoud, A. F.; et al. (2004), "Performance of Grid-Connected
      Induction Generator under Naturally Commutated AC Voltage Controller",
      Electric Power Components and Systems, 32 (7): 691â700, doi:10.1080/
      15325000490461064, Accordingly, the generator will consume active power
      from the grid, which leads to negative power factor.
  12. ^Ewald Fuchs; Mohammad A. S. Masoum (14 July 2015). Power_Quality_in
      Power_Systems_and_Electrical_Machines. Elsevier Science. pp. 432â.
      ISBN 978-0-12-800988-8. The DPF it the cosine of the angle between these
      two quantities
  13. ^Sankaran, C. (1999), Effects_of_Harmonics_on_Power_Systems, Electro-
      Test, ...and voltage-time relationship deviates from the pure sine
      function. The distortion at the point of generation is very small (about
      1% to 2%), but nonetheless it exists.
  14. ^"Single-phase_load_harmonics_vs._three-phase_load_harmonics" (PDF),
      Power System Harmonics, Pacific Gas and Electric
  15. .
  16. ^"Harmonic_Effects" (PDF), Harmonics and IEEE 519, CA: EnergyLogix
      Solutions
  17. .
  18. ^Sankaran, C. (1999), "Transformers", Effects_of_Harmonics_on_Power
      Systems, Electro-Test
  19. .
  20. ^Sankaran, C. (1999), "Motors", Effects_of_Harmonics_on_Power_Systems,
      Electro-Test, The interaction between the positive and negative sequence
      magnetic fields and currents produces torsional oscillations of the motor
      shaft. These oscillations result in shaft vibrations.
  21. ^"What is an 80 PLUS certified power supply?", Certified_Power_Supplies
      and_Manufacturers, 80 Plus
  22. ^Schramm, Ben (Fall 2006), "Power_Supply_Design_Principles:_Techniques
      and_Solutions,_Part_3", Newsletter, Nuvation, archived from the_original
      on 2007-03-09
  23. ^Wolfle, W.H.; Hurley, W.G. (2003), "Quasi-active_power_factor_correction
      with_a_variable_inductive_filter:_theory,_design_and_practice", Xplore,
      IEEE, 18 (1), pp. 248â255, doi:10.1109/TPEL.2002.807135
  24. .
  25. ^WÃ¶lfle, W. H.; Hurley, W. G., "Quasi-active Power Factor Correction:
      The Role of Variable Inductance", Power_electronics (project), IE:
      Nuigalway
  26. ^ATX_Power_Supply_Units_Roundup, xBit labs, archived from the_original on
      2008-11-20, The power factor is the measure of reactive power. It is the
      ratio of active power to the total of active and reactive power. It is
      about 0.65 with an ordinary PSU, but PSUs with active PFC have a power
      factor of 0.97â0.99. [â¦] hardware reviewers sometimes make no
      difference between the power factor and the efficiency factor. Although
      both these terms describe the effectiveness of a power supply, it is a
      gross mistake to confuse them. [â¦] There is a very small effect from
      passive PFC â the power factor grows only from 0.65 to 0.7â0.75.
  27. ^The_Active_PFC_Market_is_Expected_to_Grow_at_an_Annually_Rate_of_12.3%
      Till_2011, Find articles, Mar 16, 2006, archived from the_original on
      September 1, 2009, Higher-powered products are also likely to use active
      PFC, since it would be the most cost effective way to bring products into
      compliance with the EN standard.
  28. ^Power_Factor_Correction, TECHarp, Passive PFC [â¦] the power factor is
      low at 60â80%. [â¦] Active PFC ... a power factor of up to 95%
  29. .
  30. ^Why_we_need_PFC_in_PSU, Silverstone Technology, archived from the
      original on 2008-12-22, Normally, the power factor value of electronic
      device without power factor correction is approximately 0.5. [â¦]
      Passive PFC [â¦] 70~80% [â¦] Active PFC [â¦] 90~99.9%
  31. .
  32. ^Brooks, Tom (Mar 2004), "PFC_options_for_power_supplies", Taiyo,
      Electronic products, archived from the_original on 2008-12-02, The
      disadvantages of passive PFC techniques are that they typically yield a
      power factor of only 0.60 to 0.70 [â¦] Dual-stage active PFC technology
      [yields] a power factor typically greater than 0.98
  33. .
  34. ^Power_Factor_Correction_(PFC)_Basics (PDF) (application note) (42047),
      Fairchild Semiconductor, 2004
  35. .
  36. ^Sugawara, I.; Suzuki, Y.; Takeuchi, A.; Teshima, T. (19â23 Oct 1997),
      "Experimental studies on active and passive PFC circuits", INTELEC 97,
      19th International Telecommunications Energy Conference, pp. 571â78,
      doi:10.1109/INTLEC.1997.646051, ISBN 978-0-7803-3996-5
  37. .
  38. ^Chavez, C.; Houdek, J. A. (9â11 Oct 2007). Dynamic Harmonic Mitigation
      and power factor correction. IEE. Electrical Power Quality. pp. 1â5.
      doi:10.1109/EPQU.2007.4424144. ISBN 978-84-690-9441-9.
  39. ^"Power_Factor_â_Importance,_Calculation_and_Correction_techniques". 23
      November 2018.
  40. ^Power_Factor_Correction_Handbook (PDF), ON Semiconductor, 2007
  41. .
  42. ^Program_Requirements_for_Computers (PDF) (Version 5.0 ed.), US: Energy
      Star
  43. .
  44. ^Bolioli, T.; Duggirala, M.; Haines, E.; Kolappan, R.; Wong, H. (2009),
      Version_5.0_System_Implementation (PDF) (white paper), Energy Star
  45. .
  46. ^Fink,_Donald_G.; Beaty, H. Wayne (1978), Standard Handbook for
      Electrical Engineers (11 ed.), New York: McGraw-Hill, p. 3â29 paragraph
      80, ISBN 978-0-07-020974-9
  47. ^Manual of Electric Instruments Construction and Operating Principles,
      Schenectady, New York: General Electric, Meter and Instrument Department,
      1949, pp. 66â68, GET-1087A
  48. ^"The_Fundamentals_of_FFT-Based_Signal_Analysis_and_Measurement_in
      LabVIEW_and_LabWindows/CVI". National Instruments Corporation. Retrieved
      6 November 2017.
  49. ^"WT3000E_Series_Precision_Power_Analyzers" (PDF). Yokogawa Corporation.
      Retrieved 6 November 2017.
  50. ^"Fluke_1760_Three-Phase_Power_Quality_Recorder" (PDF). Fluke
      Corporation. Retrieved 6 November 2017.
***** External links[edit] *****
    * Harmonics_and_how_they_relate_to_power_factor (PDF), U Texas
.
NIST_Team_Demystifies_Utility_of_Power_Factor_Correction_Devices, NIST,
December 15, 2009
.
Power_factor_calculation_and_correction, US
.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Power_factor&oldid=908349648"
Categories:
    * Electrical_parameters
    * AC_power
    * Electrical_engineering
    * Engineering_ratios
Hidden categories:
    * CS1:_long_volume_value
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
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * LatvieÅ¡u
    * Bahasa_Melayu
    * áá¼ááºáá¬áá¬áá¬
    * Nederlands
    * æ¥æ¬èª
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Ù¾ÙØ¬Ø§Ø¨Û
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * Suomi
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 29 July 2019, at 04:59 (UTC).
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
