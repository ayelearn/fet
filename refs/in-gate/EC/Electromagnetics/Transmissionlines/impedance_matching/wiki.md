The following text has been accessed from https://en.wikipedia.org/wiki/Impedance_matching at Fri Aug 9 03:43:39 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Impedance matching ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Impedance mismatch" redirects here. For the computer science concept, see
object-relational_impedance_mismatch.
 This article has multiple issues. Please help improve_it or discuss these
 issues on the talk_page. (Learn_how_and_when_to_remove_these_template
 messages)
                     This article's lead_section does not adequately summarize
                     key points of its contents. Please consider expanding the
 [Wiki_letter_w.svg] lead to provide_an_accessible_overview of all important
                     aspects of the article. Please discuss this issue on the
                     article's talk_page. (December 2016)
  This article includes a list_of_references, but its sources remain unclear
  because it has insufficient inline_citations. Please help to improve this
  article by introducing more precise citations. (December 2013)(Learn_how_and
  when_to_remove_this_template_message)
 (Learn_how_and_when_to_remove_this_template_message)
[Schematic_diagram_of_source_and_load_circuit_impedance]
Source and load circuit impedance
In electronics, impedance matching is the practice of designing the input
impedance of an electrical_load or the output_impedance of its corresponding
signal source to maximize_the_power_transfer or minimize signal_reflection from
the load.
In the case of a complex source impedance ZS and load impedance ZL, maximum
power transfer is obtained when
          Z   S    =  Z   L    &#x2217;      {\displaystyle Z_{\mathrm {S} }=Z_
      {\mathrm {L} }^{*}\,}  [Z_{{\mathrm  S}}=Z_{{\mathrm  L}}^{*}\,]
where the asterisk indicates the complex_conjugate of the variable. Where ZS
represents the characteristic_impedance of a transmission_line, minimum
reflection is obtained when
          Z   S    =  Z   L       {\displaystyle Z_{\mathrm {S} }=Z_{\mathrm
      {L} }\,}  [Z_{{\mathrm  S}}=Z_{{\mathrm  L}}\,]
The concept of impedance matching found first applications in electrical
engineering, but is relevant in other applications in which a form of energy,
not necessarily electrical, is transferred between a source and a load. An
alternative to impedance matching is impedance_bridging, in which the load
impedance is chosen to be much larger than the source impedance and maximizing
voltage transfer, rather than power, is the goal.
⁰
***** Contents *****
    * 1_Theory
          o 1.1_Reflection-less_matching
          o 1.2_Maximum_power_transfer_matching
    * 2_Power_transfer
    * 3_Impedance-matching_devices
          o 3.1_Transformers
          o 3.2_Resistive_network
          o 3.3_Stepped_transmission_line
          o 3.4_Filters
                # 3.4.1_L-section
    * 4_Power_factor_correction
    * 5_Transmission_lines
          o 5.1_Single-source_transmission_line_driving_a_load
                # 5.1.1_Load-end_conditions
                # 5.1.2_Source-end_conditions
                      # 5.1.2.1_Source-end_impedance
                      # 5.1.2.2_Transfer_function
    * 6_Electrical_examples
          o 6.1_Telephone_systems
          o 6.2_Loudspeaker_amplifiers
    * 7_Non-electrical_examples
          o 7.1_Acoustics
          o 7.2_Optics
          o 7.3_Mechanics
    * 8_See_also
    * 9_Notes
    * 10_References
    * 11_External_links
***** Theory[edit] *****
Impedance is the opposition by a system to the flow of energy from a source.
For constant signals, this impedance can also be constant. For varying signals,
it usually changes with frequency. The energy involved can be electrical,
mechanical, acoustic, magnetic, or thermal. The concept of electrical impedance
is perhaps the most commonly known. Electrical impedance, like electrical
resistance, is measured in ohms. In general, impedance has a complex value;
this means that loads generally have a resistance component (symbol: R) which
forms the real part of Z and a reactance component (symbol: X) which forms the
imaginary part of Z.
In simple cases (such as low-frequency or direct-current power transmission)
the reactance may be negligible or zero; the impedance can be considered a pure
resistance, expressed as a real number. In the following summary we will
consider the general case when resistance and reactance are both significant,
and the special case in which the reactance is negligible.
**** Reflection-less matching[edit] ****
Impedance matching to minimize reflections is achieved by making the load
impedance equal to the source impedance. If the source impedance, load
impedance and transmission line characteristic_impedance are purely resistive,
then reflection-less matching is the same as maximum power transfer matching.
[1]
**** Maximum power transfer matching[edit] ****
Complex conjugate matching is used when maximum power transfer is required,
namely
          Z   l o a d    =  Z   s o u r c e    &#x2217;      {\displaystyle Z_
      {\mathsf {load}}=Z_{\mathsf {source}}^{*}\,}  [Z_{{\mathsf  {load}}}=Z_{
      {\mathsf  {source}}}^{*}\,]
where a superscript * indicates the complex_conjugate. A conjugate match is
different from a reflection-less match when either the source or load has a
reactive component.
If the source has a reactive component, but the load is purely resistive, then
matching can be achieved by adding a reactance of the same magnitude but
opposite sign to the load. This simple matching network, consisting of a single
element, will usually achieve a perfect match at only a single frequency. This
is because the added element will either be a capacitor or an inductor, whose
impedance in both cases is frequency dependent, and will not, in general,
follow the frequency dependence of the source impedance. For wide bandwidth
applications, a more complex network must be designed.
***** Power transfer[edit] *****
Main article: Maximum_power_theorem
Whenever a source of power with a fixed output impedance such as an electric
signal source, a radio transmitter or a mechanical sound (e.g., a loudspeaker)
operates into a load, the maximum possible power is delivered to the load when
the impedance of the load (load_impedance or input_impedance) is equal to the
complex_conjugate of the impedance of the source (that is, its internal
impedance or output_impedance). For two impedances to be complex conjugates
their resistances must be equal, and their reactances must be equal in
magnitude but of opposite signs. In low-frequency or DC systems (or systems
with purely resistive sources and loads) the reactances are zero, or small
enough to be ignored. In this case, maximum power transfer occurs when the
resistance of the load is equal to the resistance of the source (see maximum
power_theorem for a mathematical proof).
Impedance matching is not always necessary. For example, if a source with a low
impedance is connected to a load with a high impedance the power that can pass
through the connection is limited by the higher impedance. This maximum-voltage
connection is a common configuration called impedance_bridging or voltage
bridging, and is widely used in signal processing. In such applications,
delivering a high voltage (to minimize signal degradation during transmission
or to consume less power by reducing currents) is often more important than
maximum power transfer.
In older audio systems (reliant on transformers and passive filter networks,
and based on the telephone system), the source and load resistances were
matched at 600 ohms. One reason for this was to maximize power transfer, as
there were no amplifiers available that could restore lost signal. Another
reason was to ensure correct operation of the hybrid_transformers used at
central exchange equipment to separate outgoing from incoming speech, so these
could be amplified or fed to a four-wire_circuit. Most modern audio circuits,
on the other hand, use active amplification and filtering and can use voltage-
bridging connections for greatest accuracy. Strictly speaking, impedance
matching only applies when both source and load devices are linear; however,
matching may be obtained between nonlinear devices within certain operating
ranges.
***** Impedance-matching devices[edit] *****
Adjusting the source impedance or the load impedance, in general, is called
"impedance matching". There are three ways to improve an impedance mismatch,
all of which are called "impedance matching":
    * Devices intended to present an apparent load to the source of
      Zload = Zsource* (complex conjugate matching). Given a source with a
      fixed voltage and fixed source impedance, the maximum_power_theorem says
      this is the only way to extract the maximum power from the source.
    * Devices intended to present an apparent load of Zload = Zline (complex
      impedance matching), to avoid echoes. Given a transmission line source
      with a fixed source impedance, this "reflectionless impedance matching"
      at the end of the transmission line is the only way to avoid reflecting
      echoes back to the transmission line.
    * Devices intended to present an apparent source resistance as close to
      zero as possible, or presenting an apparent source voltage as high as
      possible. This is the only way to maximize energy efficiency, and so it
      is used at the beginning of electrical power lines. Such an impedance
      bridging connection also minimizes distortion and electromagnetic
      interference; it is also used in modern audio amplifiers and signal-
      processing devices.
There are a variety of devices used between a source of energy and a load that
perform "impedance matching". To match electrical impedances, engineers use
combinations of transformers, resistors, inductors, capacitors and transmission
lines. These passive (and active) impedance-matching devices are optimized for
different applications and include baluns, antenna_tuners (sometimes called
ATUs or roller-coasters, because of their appearance), acoustic horns, matching
networks, and terminators.
**** Transformers[edit] ****
Transformers are sometimes used to match the impedances of circuits. A
transformer converts alternating_current at one voltage to the same waveform at
another voltage. The power input to the transformer and output from the
transformer is the same (except for conversion losses). The side with the lower
voltage is at low impedance (because this has the lower number of turns), and
the side with the higher voltage is at a higher impedance (as it has more turns
in its coil).
One example of this method involves a television balun transformer. This
transformer converts a balanced signal from the antenna (via 300-ohm twin-lead)
into an unbalanced signal (75-ohm coaxial cable such as RG-6). To match the
impedances of both devices, both cables must be connected to a matching
transformer with a turns ratio of 2 (such as a 2:1 transformer). In this
example, the 75-ohm cable is connected to the transformer side with fewer
turns; the 300-ohm line is connected to the transformer side with more turns.
The formula for calculating the transformer turns ratio for this example is:
          turns ratio  =    source resistance load resistance
      {\displaystyle {\text{turns ratio}}={\sqrt {\frac {\text{source
      resistance}}{\text{load resistance}}}}}  [{\text{turns ratio}}={\sqrt  {
      {\frac  {{\text{source resistance}}}{{\text{load resistance}}}}}}]
**** Resistive network[edit] ****
Resistive impedance matches are easiest to design and can be achieved with a
simple L_pad consisting of two resistors. Power loss is an unavoidable
consequence of using resistive networks, and they are only (usually) used to
transfer line_level signals.
**** Stepped transmission line[edit] ****
Most lumped-element devices can match a specific range of load impedances. For
example, in order to match an inductive load into a real impedance, a capacitor
needs to be used. If the load impedance becomes capacitive, the matching
element must be replaced by an inductor. In many cases, there is a need to use
the same circuit to match a broad range of load impedance and thus simplify the
circuit design. This issue was addressed by the stepped transmission line,[2]
where multiple, serially placed, quarter-wave dielectric slugs are used to vary
a transmission line's characteristic impedance. By controlling the position of
each element, a broad range of load impedances can be matched without having to
reconnect the circuit.
**** Filters[edit] ****
Filters are frequently used to achieve impedance matching in telecommunications
and radio engineering. In general, it is not theoretically possible to achieve
perfect impedance matching at all frequencies with a network of discrete
components. Impedance matching networks are designed with a definite bandwidth,
take the form of a filter, and use filter theory in their design.
Applications requiring only a narrow bandwidth, such as radio tuners and
transmitters, might use a simple tuned filter such as a stub. This would
provide a perfect match at one specific frequency only. Wide bandwidth matching
requires filters with multiple sections.
*** L-section[edit] ***
Basic schematic for matching R1 to R2 with an L pad. R1 > R2, however, either
R1 or R2 may be the source and the other the load. One of X1 or X2 must be an
inductor and the other must be a capacitor.
L networks for narrowband matching a source or load impedance Z to a
transmission line with characteristic impedance Z0. X and B may each be either
positive (inductor) or negative (capacitor). If Z/Z0 is inside the 1+jx circle
on the Smith_chart (i.e. if Re(Z/Z0)>1), network (a) can be used; otherwise
network (b) can be used.[3]
A simple electrical impedance-matching network requires one capacitor and one
inductor. In the figure to the right, R1 > R2, however, either R1 or R2 may be
the source and the other the load. One of X1 or X2 must be an inductor and the
other must be a capacitor. One reactance is in parallel with the source (or
load), and the other is in series with the load (or source). If a reactance is
in parallel with the source, the effective network matches from high to low
impedance.
The analysis is as follows.[4] Consider a real source impedance of      R  1
{\displaystyle R_{1}}  [R_{1}] and real load impedance of      R  2
{\displaystyle R_{2}}  [R_{2}]. If a reactance      X  1     {\displaystyle X_
{1}}  [X_{1}] is in parallel with the source impedance, the combined impedance
can be written as:
            j  R  1    X  1      R  1   + j  X  1        {\displaystyle {\frac
      {jR_{1}X_{1}}{R_{1}+jX_{1}}}}  [{\frac  {jR_{1}X_{1}}{R_{1}+jX_{1}}}]
If the imaginary part of the above impedance is canceled by the series
reactance, the real part is
          R  2   =     R  1    X  1   2      R  1   2   +  X  1   2
      {\displaystyle R_{2}={\frac {R_{1}X_{1}^{2}}{R_{1}^{2}+X_{1}^{2}}}}  [
      {\displaystyle R_{2}={\frac {R_{1}X_{1}^{2}}{R_{1}^{2}+X_{1}^{2}}}}]
Solving for      X  1     {\displaystyle X_{1}}  [X_{1}]
          |  X  1   |  =    R  1   Q     {\displaystyle \left\vert X_
      {1}\right\vert ={\frac {R_{1}}{Q}}}  [{\displaystyle \left\vert X_
      {1}\right\vert ={\frac {R_{1}}{Q}}}].
          |  X  2   |  = Q  R  2     {\displaystyle \left\vert X_{2}\right\vert
      =QR_{2}}  [{\displaystyle \left\vert X_{2}\right\vert =QR_{2}}].
      where     Q =      R  1   &#x2212;  R  2     R  2        {\displaystyle
      Q={\sqrt {\frac {R_{1}-R_{2}}{R_{2}}}}}  [{\displaystyle Q={\sqrt {\frac
      {R_{1}-R_{2}}{R_{2}}}}}].
Note,      X  1     {\displaystyle X_{1}}  [X_{1}], the reactance in parallel,
has a negative reactance because it is typically a capacitor. This gives the L-
network the additional feature of harmonic suppression since it is a low pass
filter too.
The inverse connection (impedance step-up) is simply the reverseâfor example,
reactance in series with the source. The magnitude of the impedance ratio is
limited by reactance losses such as the Q of the inductor. Multiple L-sections
can be wired in cascade to achieve higher impedance ratios or greater
bandwidth. Transmission_line matching networks can be modeled as infinitely
many L-sections wired in cascade. Optimal matching circuits can be designed for
a particular system using Smith_charts.
***** Power factor correction[edit] *****
Power_factor_correction devices are intended to cancel the reactive and
nonlinear characteristics of a load at the end of a power line. This causes the
load seen by the power line to be purely resistive. For a given true power
required by a load this minimizes the true current supplied through the power
lines, and minimizes power wasted in the resistance of those power lines. For
example, a maximum_power_point_tracker is used to extract the maximum power
from a solar panel and efficiently transfer it to batteries, the power grid or
other loads. The maximum power theorem applies to its "upstream" connection to
the solar panel, so it emulates a load resistance equal to the solar panel
source resistance. However, the maximum power theorem does not apply to its
"downstream" connection. That connection is an impedance_bridging connection;
it emulates a high-voltage, low-resistance source to maximize efficiency.
On the power_grid the overall load is usually inductive. Consequently, power
factor correction is most commonly achieved with banks of capacitors. It is
only necessary for correction to be achieved at one single frequency, the
frequency of the supply. Complex networks are only required when a band of
frequencies must be matched and this is the reason why simple capacitors are
all that is usually required for power factor correction.
***** Transmission lines[edit] *****
[Schematic_diagram_of_coaxial_cable]
Coaxial transmission line with one source and one load
Impedance bridging is unsuitable for RF connections, because it causes power to
be reflected back to the source from the boundary between the high and the low
impedances. The reflection creates a standing_wave if there is reflection at
both ends of the transmission line, which leads to further power waste and may
cause frequency-dependent loss. In these systems, impedance matching is
desirable.
In electrical systems involving transmission_lines (such as radio and fiber
optics)âwhere the length of the line is long compared to the wavelength of
the signal (the signal changes rapidly compared to the time it takes to travel
from source to load)â the impedances at each end of the line must be matched
to the transmission line's characteristic_impedance (     Z  c
{\displaystyle Z_{c}}  [Z_c]) to prevent reflections of the signal at the ends
of the line. (When the length of the line is short compared to the wavelength,
impedance mismatch is the basis of transmission-line impedance transformers;
see previous section.) In radio-frequency (RF) systems, a common value for
source and load impedances is 50 ohms. A typical RF load is a quarter-wave
ground plane antenna (37 ohms with an ideal ground plane); it can be matched to
50 ohms by using a modified ground plane or a coaxial matching section, i.e.,
part or all the feeder of higher impedance.
The general form of the voltage reflection_coefficient for a wave moving from
medium 1 to medium 2 is given by
          &#x0393;  12   =     Z  2   &#x2212;  Z  1      Z  2   +  Z  1
      {\displaystyle \Gamma _{12}={Z_{2}-Z_{1} \over Z_{2}+Z_{1}}}  [\Gamma _{
      {12}}={Z_{2}-Z_{1} \over Z_{2}+Z_{1}}]
while the voltage reflection coefficient for a wave moving from medium 2 to
medium 1 is
          &#x0393;  21   =     Z  1   &#x2212;  Z  2      Z  1   +  Z  2
      {\displaystyle \Gamma _{21}={Z_{1}-Z_{2} \over Z_{1}+Z_{2}}}  [\Gamma _{
      {21}}={Z_{1}-Z_{2} \over Z_{1}+Z_{2}}]
          &#x0393;  21   = &#x2212;  &#x0393;  12      {\displaystyle \Gamma _
      {21}=-\Gamma _{12}\,}  [\Gamma _{{21}}=-\Gamma _{{12}}\,]
so the reflection coefficient is the same (except for sign), no matter from
which direction the wave approaches the boundary.
There is also a current reflection coefficient, which is the negative of the
voltage reflection coefficient. If the wave encounters an open at the load end,
positive voltage and negative current pulses are transmitted back toward the
source (negative current means the current is going the opposite direction).
Thus, at each boundary there are four reflection coefficients (voltage and
current on one side, and voltage and current on the other side). All four are
the same, except that two are positive and two are negative. The voltage
reflection coefficient and current reflection coefficient on the same side have
opposite signs. Voltage reflection coefficients on opposite sides of the
boundary have opposite signs.
Because they are all the same except for sign it is traditional to interpret
the reflection coefficient as the voltage reflection coefficient (unless
otherwise indicated). Either end (or both ends) of a transmission line can be a
source or a load (or both), so there is no inherent preference for which side
of the boundary is medium 1 and which side is medium 2. With a single
transmission line it is customary to define the voltage reflection coefficient
for a wave incident on the boundary from the transmission line side, regardless
of whether a source or load is connected on the other side.
**** Single-source transmission line driving a load[edit] ****
*** Load-end conditions[edit] ***
In a transmission line, a wave travels from the source along the line. Suppose
the wave hits a boundary (an abrupt change in impedance). Some of the wave is
reflected back, while some keeps moving onwards. (Assume there is only one
boundary, at the load.)
Let
          V  i      {\displaystyle V_{i}\,}  [V_{i}\,] and      I  i
      {\displaystyle I_{i}\,}  [I_{i}\,] be the voltage and current that is
      incident on the boundary from the source side.
          V  t      {\displaystyle V_{t}\,}  [V_{t}\,] and      I  t
      {\displaystyle I_{t}\,}  [I_{t}\,] be the voltage and current that is
      transmitted to the load.
          V  r      {\displaystyle V_{r}\,}  [V_{r}\,] and      I  r
      {\displaystyle I_{r}\,}  [I_{r}\,] be the voltage and current that is
      reflected back toward the source.
On the line side of the boundary      V  i   =  Z  c    I  i
{\displaystyle V_{i}=Z_{c}I_{i}\,}  [V_{i}=Z_{c}I_{i}\,] and      V  r   =
&#x2212;  Z  c    I  r      {\displaystyle V_{r}=-Z_{c}I_{r}\,}  [V_{r}=-Z_
{c}I_{r}\,] and on the load side      V  t   =  Z  L    I  t
{\displaystyle V_{t}=Z_{L}I_{t}\,}  [V_{t}=Z_{L}I_{t}\,] where      V  i
{\displaystyle V_{i}\,}  [V_{i}\,],      V  r      {\displaystyle V_{r}\,}  [V_
{r}\,],      V  t      {\displaystyle V_{t}\,}  [V_{t}\,],      I  i
{\displaystyle I_{i}\,}  [I_{i}\,],      I  r      {\displaystyle I_{r}\,}  [I_
{r}\,],      I  t      {\displaystyle I_{t}\,}  [I_{t}\,], and      Z  c
{\displaystyle Z_{c}\,}  [Z_{c}\,] are phasors.
At a boundary, voltage and current must be continuous, therefore
          V  t   =  V  i   +  V  r      {\displaystyle V_{t}=V_{i}+V_{r}\,}
      [V_{t}=V_{i}+V_{r}\,]
          I  t   =  I  i   +  I  r      {\displaystyle I_{t}=I_{i}+I_{r}\,}
      [I_{t}=I_{i}+I_{r}\,]
All these conditions are satisfied by
          V  r   =  &#x0393;  T L    V  i      {\displaystyle V_{r}=\Gamma _
      {TL}V_{i}\,}  [V_{r}=\Gamma _{{TL}}V_{i}\,]
          I  r   = &#x2212;  &#x0393;  T L    I  i      {\displaystyle I_{r}=-
      \Gamma _{TL}I_{i}\,}  [I_{r}=-\Gamma _{{TL}}I_{i}\,]
          V  t   = ( 1 +  &#x0393;  T L   )  V  i      {\displaystyle V_{t}=
      (1+\Gamma _{TL})V_{i}\,}  [V_{t}=(1+\Gamma _{{TL}})V_{i}\,]
          I  t   = ( 1 &#x2212;  &#x0393;  T L   )  I  i      {\displaystyle I_
      {t}=(1-\Gamma _{TL})I_{i}\,}  [I_{t}=(1-\Gamma _{{TL}})I_{i}\,]
where      &#x0393;  T L      {\displaystyle \Gamma _{TL}\,}  [\Gamma _{
{TL}}\,] the reflection_coefficient going from the transmission line to the
load.
          &#x0393;  T L   =     Z  L   &#x2212;  Z  c      Z  L   +  Z  c
      =  &#x0393;  L      {\displaystyle \Gamma _{TL}={Z_{L}-Z_{c} \over Z_
      {L}+Z_{c}}=\Gamma _{L}\,}  [\Gamma _{{TL}}={Z_{L}-Z_{c} \over Z_{L}+Z_
      {c}}=\Gamma _{L}\,][5][6][7]
The purpose of a transmission line is to get the maximum amount of energy to
the other end of the line (or to transmit information with minimal error), so
the reflection is as small as possible. This is achieved by matching the
impedances      Z  L     {\displaystyle Z_{L}}  [Z_{L}] and      Z  c
{\displaystyle Z_{c}}  [Z_c] so that they are equal (    &#x0393; = 0
{\displaystyle \Gamma =0}  [\Gamma =0]).
*** Source-end conditions[edit] ***
At the source end of the transmission line, there may be waves incident both
from the source and from the line; a reflection coefficient for each direction
may be computed with
         &#x2212;  &#x0393;  S T   =  &#x0393;  T S   =     Z  s   &#x2212;  Z
      c      Z  s   +  Z  c      =  &#x0393;  S      {\displaystyle -\Gamma _
      {ST}=\Gamma _{TS}={Z_{s}-Z_{c} \over Z_{s}+Z_{c}}=\Gamma _{S}\,}  [-
      \Gamma _{{ST}}=\Gamma _{{TS}}={Z_{s}-Z_{c} \over Z_{s}+Z_{c}}=\Gamma _
      {S}\,],
where Zs is the source impedance. The source of waves incident from the line
are the reflections from the load end. If the source impedance matches the
line, reflections from the load end will be absorbed at the source end. If the
transmission line is not matched at both ends reflections from the load will be
re-reflected at the source and re-re-reflected at the load end ad infinitum,
losing energy on each transit of the transmission line. This can cause a
resonance condition and strongly frequency-dependent behavior. In a narrow-band
system this can be desirable for matching, but is generally undesirable in a
wide-band system.
** Source-end impedance[edit] **
          Z  i n   =  Z  C      ( 1 +  T  2    &#x0393;  L   )   ( 1 &#x2212;
      T  2    &#x0393;  L   )       {\displaystyle Z_{in}=Z_{C}{\frac {(1+T^
      {2}\Gamma _{L})}{(1-T^{2}\Gamma _{L})}}\,}  [Z_{{in}}=Z_{C}{\frac  {(1+T^
      {2}\Gamma _{L})}{(1-T^{2}\Gamma _{L})}}\,] [8]
where     T &#xA0; ,   {\displaystyle T\ ,}  [T\ ,] is the one-way transfer
function (from either end to the other) when the transmission line is exactly
matched at source and load.     T    {\displaystyle T\,}  [T\,] accounts for
everything that happens to the signal in transit (including delay, attenuation
and dispersion). If there is a perfect match at the load,      &#x0393;  L   =
0    {\displaystyle \Gamma _{L}=0\,}  [\Gamma _{L}=0\,] and      Z  i n   =  Z
C      {\displaystyle Z_{in}=Z_{C}\,}  [Z_{{in}}=Z_{C}\,]
** Transfer function[edit] **
          V  L   =  V  S      T ( 1 &#x2212;  &#x0393;  S   ) ( 1 +  &#x0393;
      L   )   2 ( 1 &#x2212;  T  2    &#x0393;  S    &#x0393;  L   )
      {\displaystyle V_{L}=V_{S}{\frac {T(1-\Gamma _{S})(1+\Gamma _{L})}{2(1-T^
      {2}\Gamma _{S}\Gamma _{L})}}\,}  [V_{L}=V_{S}{\frac  {T(1-\Gamma _{S})
      (1+\Gamma _{L})}{2(1-T^{2}\Gamma _{S}\Gamma _{L})}}\,]
where      V  S      {\displaystyle V_{S}\,}  [V_{S}\,] is the open circuit (or
unloaded) output voltage from the source.
Note that if there is a perfect match at both ends
          &#x0393;  L   = 0    {\displaystyle \Gamma _{L}=0\,}  [\Gamma _
      {L}=0\,] and      &#x0393;  S   = 0    {\displaystyle \Gamma _{S}=0\,}
      [\Gamma _{S}=0\,]
and then
          V  L   =  V  S     T 2      {\displaystyle V_{L}=V_{S}{\frac {T}
      {2}}\,}  [V_{L}=V_{S}{\frac  {T}{2}}\,].
***** Electrical examples[edit] *****
**** Telephone systems[edit] ****
Telephone systems also use matched impedances to minimise echo on long-distance
lines. This is related to transmission-line theory. Matching also enables the
telephone hybrid_coil (2- to 4-wire conversion) to operate correctly. As the
signals are sent and received on the same two-wire_circuit to the central
office (or exchange), cancellation is necessary at the telephone earpiece so
excessive sidetone is not heard. All devices used in telephone signal paths are
generally dependent on matched cable, source and load impedances. In the local
loop, the impedance chosen is 600 ohms (nominal). Terminating networks are
installed at the exchange to offer the best match to their subscriber lines.
Each country has its own standard for these networks, but they are all designed
to approximate about 600 ohms over the voice_frequency band.
**** Loudspeaker amplifiers[edit] ****
[Schematic_diagram_of_amplifier_and_speaker,_with_two_tubes_and_an_impedance-
matching_transformer]
Typical pushâpull audio tube power amplifier, matched to loudspeaker with an
impedance-matching transformer
Audio_amplifiers typically do not match impedances, but provide an output
impedance that is lower than the load impedance (such as < 0.1 ohm in typical
semiconductor amplifiers), for improved speaker damping. For vacuum_tube
amplifiers, impedance-changing transformers are often used to get a low output
impedance, and to better match the amplifier's performance to the load
impedance. Some tube amplifiers have output transformer taps to adapt the
amplifier output to typical loudspeaker impedances.
The output transformer in vacuum-tube-based amplifiers has two basic functions:
    * Separation of the AC component (which contains the audio signals) from
      the DC component (supplied by the power_supply) in the anode circuit of a
      vacuum-tube-based power stage. A loudspeaker should not be subjected to
      DC current.
    * Reducing the output impedance of power pentodes (such as the EL34) in a
      common-cathode configuration.
The impedance of the loudspeaker on the secondary coil of the transformer will
be transformed to a higher impedance on the primary coil in the circuit of the
power pentodes by the square of the turns_ratio, which forms the impedance
scaling factor.
The output stage in common-drain or common-collector semiconductor-based end
stages with MOSFETs or power_transistors has a very low output impedance. If
they are properly balanced, there is no need for a transformer or a large
electrolytic_capacitor to separate AC from DC current.
***** Non-electrical examples[edit] *****
**** Acoustics[edit] ****
Similar to electrical transmission lines, an impedance matching problem exists
when transferring sound energy from one medium to another. If the acoustic
impedance of the two media are very different most sound energy will be
reflected (or absorbed), rather than transferred across the border. The gel
used in medical_ultrasonography helps transfer acoustic energy from the
transducer to the body and back again. Without the gel, the impedance mismatch
in the transducer-to-air and the air-to-body discontinuity reflects almost all
the energy, leaving very little to go into the body.
The bones in the middle_ear provide impedance matching between the eardrum
(which is acted upon by vibrations in air) and the fluid-filled inner ear.
Horns are used like transformers, matching the impedance of the transducer to
the impedance of the air. This principle is used in both horn_loudspeakers and
musical instruments. Most loudspeaker systems contain impedance matching
mechanisms, especially for low frequencies. Because most driver impedances
which are poorly matched to the impedance of free air at low frequencies (and
because of out-of-phase cancellations between output from the front and rear of
a speaker cone), loudspeaker enclosures both match impedances and prevent
interference. Sound, coupling with air, from a loudspeaker is related to the
ratio of the diameter of the speaker to the wavelength of the sound being
reproduced. That is, larger speakers can produce lower frequencies at a higher
level than smaller speakers for this reason. Elliptical speakers are a complex
case, acting like large speakers lengthwise and small speakers crosswise.
Acoustic impedance matching (or the lack of it) affects the operation of a
megaphone, an echo and soundproofing.
**** Optics[edit] ****
A similar effect occurs when light (or any electromagnetic wave) hits the
interface between two media with different refractive_indices. For non-magnetic
materials, the refractive index is inversely proportional to the material's
characteristic impedance. An optical or wave impedance (that depends on the
propagation direction) can be calculated for each medium, and may be used in
the transmission-line reflection equation
         r =     Z  2   &#x2212;  Z  1      Z  1   +  Z  2
      {\displaystyle r={Z_{2}-Z_{1} \over Z_{1}+Z_{2}}}  [r={Z_{2}-Z_{1} \over
      Z_{1}+Z_{2}}]
to calculate reflection and transmission coefficients for the interface. For
non-magnetic dielectrics, this equation is equivalent to the Fresnel_equations.
Unwanted reflections can be reduced by the use of an anti-reflection optical
coating.
**** Mechanics[edit] ****
If a body of mass m collides elastically with a second body, maximum energy
transfer to the second body will occur when the second body has the same mass
m. In a head-on collision of equal masses, the energy of the first body will be
completely transferred to the second body (as in Newton's_cradle for example).
In this case, the masses act as "mechanical impedances",[dubious  – discuss]
which must be matched. If      m  1     {\displaystyle m_{1}}  [m_{1}] and
m  2     {\displaystyle m_{2}}  [m_{2}] are the masses of the moving and
stationary bodies, and P is the momentum of the system (which remains constant
throughout the collision), the energy of the second body after the collision
will be E2:
          E  2   =    2  P  2    m  2     (  m  1   +  m  2    )  2
      {\displaystyle E_{2}={\frac {2P^{2}m_{2}}{(m_{1}+m_{2})^{2}}}}  [E_{2}=
      {\frac  {2P^{2}m_{2}}{(m_{1}+m_{2})^{2}}}]
which is analogous to the power-transfer equation.
These principles are useful in the application of highly energetic materials
(explosives). If an explosive charge is placed on a target, the sudden release
of energy causes compression waves to propagate through the target radially
from the point-charge contact. When the compression waves reach areas of high
acoustic impedance mismatch (such as the opposite side of the target), tension
waves reflect back and create spalling. The greater the mismatch, the greater
the effect of creasing and spalling will be. A charge initiated against a wall
with air behind it will do more damage to the wall than a charge initiated
against a wall with soil behind it.
***** See also[edit] *****
    * Power_(physics)
    * Reflection_coefficient
    * Ringing_(signal)
    * Standing_wave_ratio
    * Transmission_line
    * Wet_Transformer
***** Notes[edit] *****
   1. ^ Stutzman_&_Thiele_2012, p. 177, page_link
   2. ^Qian, Chunqui; Brey, William W. (July 2009). "Impedance_matching_with_an
      adjustable_segmented_transmission_line". Journal of Magnetic Resonance.
      199 (1): 104â110. Archived from the_original on 2013-01-04.
   3. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   4. ^Pozar, David. Microwave Engineering (3rd ed.). p. 223.
   5. ^Hayward, Wes (1994). Introduction_to_Radio_Frquency_Design. ARRL.
      p. 138. ISBN 0-87259-492-0.
   6. ^ Kraus_(1984, p. 407)
   7. ^ Sadiku_(1989, pp. 505â507)
   8. ^ Hayt_(1989, pp. 398â401)
   9. ^ Karakash_(1950, pp. 52â57)
***** References[edit] *****
    * Floyd, Thomas (1997), Principles of Electric Circuits (5th ed.), Prentice
      Hall, ISBN 0-13-232224-2
Hayt, William (1989), Engineering_Electromagnetics (5th ed.), McGraw-Hill,
ISBN 0-07-027406-1
Karakash, John J. (1950), Transmission Lines and Filter Networks (1st ed.),
Macmillan
Kraus, John D. (1984), Electromagnetics (3rd ed.), McGraw-Hill, ISBN 0-07-
035423-5
Sadiku, Matthew N. O. (1989), Elements of Electromagnetics (1st ed.), Saunders
College Publishing, ISBN 0030134846
Stutzman, Warren L.; Thiele, Gary (2012), Antenna Theory and Design, John Wiley
& Sons, ISBN 0470576642
Young, E. C. (1988), "maximum power theorem", The Penguin Dictionary of
Electronics, Penguin, ISBN 0-14-051187-3
Young, E. C. (1988), "impedance matching", The Penguin Dictionary of
Electronics, Penguin, ISBN 0-14-051187-3
***** External links[edit] *****
    * Impedance_Matching Impedance Matching with the Smith Chart

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Impedance_matching&oldid=909693253"
Categories:
    * Electronic_design
    * Filter_theory
Hidden categories:
    * Wikipedia_introduction_cleanup_from_December_2016
    * All_pages_needing_cleanup
    * Articles_covered_by_WikiProject_Wikify_from_December_2016
    * All_articles_covered_by_WikiProject_Wikify
    * Articles_lacking_in-text_citations_from_December_2013
    * All_articles_lacking_in-text_citations
    * Articles_with_multiple_maintenance_issues
    * All_accuracy_disputes
    * Articles_with_disputed_statements_from_July_2012
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
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * Bahasa_Melayu
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Simple_English
    * Suomi
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 00:26 (UTC).
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
