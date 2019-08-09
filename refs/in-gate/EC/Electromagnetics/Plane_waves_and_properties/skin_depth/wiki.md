The following text has been accessed from https://en.wikipedia.org/wiki/Skin_effect at Fri Aug 9 03:42:38 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Skin effect ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Skin depth" redirects here. For the depth (layers) of biological/organic skin,
see skin.
Distribution of current flow in a cylindrical conductor, shown in cross
section. For alternating_current, the current density decreases exponentially
from the surface towards the inside. The skin depth, Î´, is defined as the
depth where the current density is just 1/e (about 37%) of the value at the
surface; it depends on the frequency of the current and the electrical and
magnetic properties of the conductor.
Each 3-wire bundle in this power transmission installation acts as a single
conductor. A single wire using the same amount of metal per kilometer would
have higher losses due to the skin effect.
Skin effect is the tendency of an alternating_electric_current (AC) to become
distributed within a conductor such that the current_density is largest near
the surface of the conductor, and decreases with greater depths in the
conductor. The electric current flows mainly at the "skin" of the conductor,
between the outer surface and a level called the skin depth. The skin effect
causes the effective resistance of the conductor to increase at higher
frequencies where the skin depth is smaller, thus reducing the effective cross-
section of the conductor. The skin effect is due to opposing eddy_currents
induced by the changing magnetic field resulting from the alternating current.
At 60 Hz in copper, the skin depth is about 8.5 mm. At high frequencies the
skin depth becomes much smaller. Increased AC resistance due to the skin effect
can be mitigated by using specially woven litz_wire. Because the interior of a
large conductor carries so little of the current, tubular conductors such as
pipe can be used to save weight and cost.
⁰
***** Contents *****
    * 1_Cause
    * 2_Formula
    * 3_Current_density_in_a_round_conductor
    * 4_Impedance_of_round_wire
          o 4.1_Inductance
          o 4.2_Resistance
    * 5_Material_effect_on_skin_depth
    * 6_Mitigation
    * 7_Examples
    * 8_Skin_effect_reduction_of_the_internal_inductance_of_a_conductor
          o 8.1_Inductance_per_length_in_a_coaxial_cable
          o 8.2_Characteristics_of_telephone_cable_as_a_function_of_frequency
    * 9_See_also
    * 10_Notes
    * 11_References
    * 12_External_links
***** Cause[edit] *****
Skin depth is due to the circulating eddy_currents (arising from a changing H
field) cancelling the current flow in the center of a conductor and reinforcing
it in the skin.
Conductors, typically in the form of wires, may be used to transmit electrical
energy or signals using an alternating_current flowing through that conductor.
The charge carriers constituting that current, usually electrons, are driven by
an electric field due to the source of electrical energy. An alternating
current in a conductor produces an alternating magnetic field in and around the
conductor. When the intensity of current in a conductor changes, the magnetic
field also changes. The change in the magnetic field, in turn, creates an
electric field which opposes the change in current intensity. This opposing
electric field is called âcounter-electromotive_forceâ (back EMF). The back
EMF is strongest at the center of the conductor, and forces the conducting
electrons to the outside of the conductor, as shown in the diagram on the
right.[1] [2]
An alternating current may also be induced in a conductor due to an alternating
magnetic field according to the law of induction. An electromagnetic_wave
impinging on a conductor will therefore generally produce such a current; this
explains the reflection of electromagnetic waves from metals.
Regardless of the driving force, the current_density is found to be greatest at
the conductor's surface, with a reduced magnitude deeper in the conductor. That
decline in current density is known as the skin effect and the skin depth is a
measure of the depth at which the current density falls to 1/e of its value
near the surface. Over 98% of the current will flow within a layer 4 times the
skin depth from the surface. This behavior is distinct from that of direct
current which usually will be distributed evenly over the cross-section of the
wire.
The effect was first described in a paper by Horace_Lamb in 1883 for the case
of spherical conductors, and was generalised to conductors of any shape by
Oliver_Heaviside in 1885. The skin effect has practical consequences in the
analysis and design of radio-frequency and microwave circuits, transmission
lines (or waveguides), and antennas. It is also important at mains frequencies
(50â60 Hz) in AC electrical_power_transmission_and_distribution systems.
Although the term "skin effect" is most often associated with applications
involving transmission of electric currents, the skin depth also describes the
exponential decay of the electric and magnetic fields, as well as the density
of induced currents, inside a bulk material when a plane wave impinges on it at
normal incidence.
***** Formula[edit] *****
The AC current_density J in a conductor decreases_exponentially from its value
at the surface JS according to the depth d from the surface, as follows:[3]:362
         J =  J   S      e  &#x2212;  ( 1 + j ) d  /  &#x03B4;
      {\displaystyle J=J_{\mathrm {S} }\,e^{-{(1+j)d/\delta }}}  [
      {\displaystyle J=J_{\mathrm {S} }\,e^{-{(1+j)d/\delta }}}]
where Î´ is called the skin depth. The skin depth is thus defined as the depth
below the surface of the conductor at which the current density has fallen to
1/e (about 0.37) of JS. The imaginary part of the exponent indicates that the
phase of the current density is delayed 1 radian for each skin depth of
penetration. One full wavelength in the conductor requires 2Ï skin depths, at
which point the current density is attenuated to eâ2Ï (-54.6 dB) of its
surface value. The wavelength in the conductor is much shorter than the
wavelength in vacuum, or equivalently, the phase_velocity in the conductor is
very much slower than the speed_of_light in vacuum. For example, a 1 MHz radio
wave has a wavelength in vacuum Î»0 of about 300 m, whereas in copper, the
wavelength is reduced to only about 0.5 mm with a phase velocity of only about
500 m/s. As a consequence of Snell's_law and this very tiny phase velocity in
the conductor, any wave entering the conductor, even at grazing incidence,
refracts essentially in the direction perpendicular to the conductor's surface.
The general formula for the skin depth is:[4][5]
         &#x03B4; =     2 &#x03C1;   &#x03C9; &#x03BC;           1 +
      (  &#x03C1; &#x03C9; &#x03F5;  )   2     + &#x03C1; &#x03C9; &#x03F5;
      {\displaystyle \delta ={\sqrt {{2\rho } \over {\omega \mu }}}\;\;{\sqrt {
      {\sqrt {1+\left({\rho \omega \epsilon }\right)^{2}}}+\rho \omega \epsilon
      }}}  [\delta= \sqrt{{2\rho }\over{\omega\mu}}
      \; \;  \sqrt{ \sqrt{1 + \left({\rho\omega\epsilon}\right)^2 }
      + \rho\omega\epsilon}  ]
where
         &#x03C1;   {\displaystyle \rho }  [\rho ] = resistivity of the
      conductor
         &#x03C9;   {\displaystyle \omega }  [\omega ] = angular_frequency of
      current = 2Ï Ã frequency
         &#x03BC;   {\displaystyle \mu }  [\mu ] =      &#x03BC;  r
      {\displaystyle \mu _{r}}  [ \mu_r ]     &#x03BC;  0     {\displaystyle
      \mu _{0}}  [ \mu_0 ]
          &#x03BC;  r     {\displaystyle \mu _{r}}  [ \mu_r ] = relative
      magnetic_permeability of the conductor
          &#x03BC;  0     {\displaystyle \mu _{0}}  [ \mu_0 ] = the
      permeability_of_free_space
         &#x03F5;   {\displaystyle \epsilon }  [\epsilon ] =      &#x03F5;  r
      {\displaystyle \epsilon _{r}}  [ \epsilon_r ]     &#x03F5;  0
      {\displaystyle \epsilon _{0}}  [ \epsilon_0 ]
          &#x03F5;  r     {\displaystyle \epsilon _{r}}  [ \epsilon_r ] =
      relative permittivity of the material
          &#x03F5;  0     {\displaystyle \epsilon _{0}}  [ \epsilon_0 ] = the
      permittivity_of_free_space
At frequencies much below     1  /  &#x03C1; &#x03F5;   {\displaystyle 1/\rho
\epsilon }  [1/\rho \epsilon] the quantity inside the large radical is close to
unity and the formula is more usually given as:
         &#x03B4; =     2 &#x03C1;   &#x03C9; &#x03BC;       {\displaystyle
      \delta ={\sqrt {{2\rho } \over {\omega \mu }}}}  [\delta=\sqrt{{2\rho
      }\over{\omega\mu}}].
This formula is valid at frequencies away from strong atomic or molecular
resonances (where     &#x03F5;   {\displaystyle \epsilon }  [\epsilon ] would
have a large imaginary part) and at frequencies that are much below both the
material's plasma_frequency (dependent on the density of free electrons in the
material) and the reciprocal of the mean time between collisions involving the
conduction electrons. In good conductors such as metals all of those conditions
are ensured at least up to microwave frequencies, justifying this formula's
validity.[note_1] For example, in the case of copper, this would be true for
frequencies much below 1018 Hz.
However, in very poor conductors, at sufficiently high frequencies, the factor
under the large radical increases. At frequencies much higher than     1  /
&#x03C1; &#x03F5;   {\displaystyle 1/\rho \epsilon }  [1/\rho \epsilon] it can
be shown that the skin depth, rather than continuing to decrease, approaches an
asymptotic value:
         &#x03B4; &#x2248;  2 &#x03C1;     &#x03F5; &#x03BC;
      {\displaystyle \delta \approx {2\rho }{\sqrt {\epsilon \over \mu }}}
      [\delta \approx  {2 \rho} \sqrt{\epsilon \over \mu} ]
This departure from the usual formula only applies for materials of rather low
conductivity and at frequencies where the vacuum wavelength is not much larger
than the skin depth itself. For instance, bulk silicon (undoped) is a poor
conductor and has a skin depth of about 40 meters at 100 kHz (λ = 3000 m).
However, as the frequency is increased well into the megahertz range, its skin
depth never falls below the asymptotic value of 11 meters. The conclusion is
that in poor solid conductors such as undoped silicon, the skin effect doesn't
need to be taken into account in most practical situations: any current is
equally distributed throughout the material's cross-section regardless of its
frequency.
***** Current density in a round conductor[edit] *****
When the skin depth is not small with respect to the radius of the wire,
current_density may be described in terms of Bessel_functions. The current
density inside round wire away from the influences of other fields, as function
of distance from the axis is given by Weeks.[6]:38
Current density in round wire for various skin depths. Numbers shown on each
curve are the ratio of skin depth to wire radius. The curve shown with the
infinity sign is the zero frequency (DC) case. All curves are normalized so
that the current density at the surface is the same. The horizontal axis is the
position within the wire with the left and right extremes being the surface of
the wire. The vertical axis is relative current density.
           J   r   =    k  I    2 &#x03C0; R        J  0   ( k r )    J  1
      ( k R )    =   J   R       J  0   ( k r )    J  0   ( k R )
      {\displaystyle \mathbf {J} _{r}={\frac {k\mathbf {I} }{2\pi R}}{\frac {J_
      {0}(kr)}{J_{1}(kR)}}=\mathbf {J} _{R}{\frac {J_{0}(kr)}{J_{0}(kR)}}}  [
      {\displaystyle \mathbf {J} _{r}={\frac {k\mathbf {I} }{2\pi R}}{\frac {J_
      {0}(kr)}{J_{1}(kR)}}=\mathbf {J} _{R}{\frac {J_{0}(kr)}{J_{0}(kR)}}}]
where
          &#x03C9;   {\displaystyle \quad \omega }  [{\displaystyle \quad
      \omega }] = angular_frequency of current = 2Ï Ã frequency
          r =   {\displaystyle \quad r=}  [{\displaystyle \quad r=}] distance
      from the axis of the wire
          R =   {\displaystyle \quad R=}  [{\displaystyle \quad R=}] radius of
      the wire
            J   r   =   {\displaystyle \quad \mathbf {J} _{r}=}  [
      {\displaystyle \quad \mathbf {J} _{r}=}] current density phasor at
      distance, r, from the axis of the wire
            J   R   =   {\displaystyle \quad \mathbf {J} _{R}=}  [
      {\displaystyle \quad \mathbf {J} _{R}=}] current density phasor at the
      surface of the wire
           I  =   {\displaystyle \quad \mathbf {I} =}  [{\displaystyle \quad
      \mathbf {I} =}] total current phasor
           J  0   =   {\displaystyle \quad J_{0}=}  [{\displaystyle \quad J_
      {0}=}] Bessel function of the first kind, order 0
           J  1   =   {\displaystyle \quad J_{1}=}  [{\displaystyle \quad J_
      {1}=}] Bessel function of the first kind, order 1
          k =     &#x2212; j &#x03C9; &#x03BC;  &#x03C1;    =    1 &#x2212; j
      &#x03B4;     {\displaystyle \quad k={\sqrt {\frac {-j\omega \mu }{\rho
      }}}={\frac {1-j}{\delta }}}  [{\displaystyle \quad k={\sqrt {\frac {-
      j\omega \mu }{\rho }}}={\frac {1-j}{\delta }}}] the wave_number in the
      conductor
          &#x03B4; =     2 &#x03C1;   &#x03C9; &#x03BC;       {\displaystyle
      \quad \delta ={\sqrt {\frac {2\rho }{\omega \mu }}}}  [{\displaystyle
      \quad \delta ={\sqrt {\frac {2\rho }{\omega \mu }}}}] also called skin
      depth.
          &#x03C1;   {\displaystyle \quad \rho }  [{\displaystyle \quad \rho }]
      = resistivity of the conductor
           &#x03BC;  r     {\displaystyle \quad \mu _{r}}  [{\displaystyle
      \quad \mu _{r}}] = relative magnetic_permeability of the conductor
           &#x03BC;  0     {\displaystyle \quad \mu _{0}}  [{\displaystyle
      \quad \mu _{0}}] = the permeability_of_free_space = 4Ï x 10â7 H/m
          &#x03BC;   {\displaystyle \quad \mu }  [{\displaystyle \quad \mu }] =
      &#x03BC;  r     {\displaystyle \mu _{r}}  [ \mu_r ]     &#x03BC;  0
      {\displaystyle \mu _{0}}  [ \mu_0 ]
Since     k   {\displaystyle k}  [k] is complex, the Bessel functions are also
complex. The amplitude and phase of the current density varies with depth.
***** Impedance of round wire[edit] *****
The internal impedance per unit length of a segment of round wire is given by:
[6]:40
           Z   i n t   =    k &#x03C1;   2 &#x03C0; R        J  0   ( k R )
      J  1   ( k R )      {\displaystyle \mathbf {Z} _{int}={\frac {k\rho }
      {2\pi R}}{\frac {J_{0}(kR)}{J_{1}(kR)}}}  [{\displaystyle \mathbf {Z} _
      {int}={\frac {k\rho }{2\pi R}}{\frac {J_{0}(kR)}{J_{1}(kR)}}}].
This impedance is a complex quantity corresponding to a resistance (real) in
series with the reactance (imaginary) due to the wire's internal self-
inductance, per unit length.
**** Inductance[edit] ****
A portion of a wire's inductance can be attributed to the magnetic field inside
the wire itself which is termed the internal inductance; this accounts for the
inductive reactance (imaginary part of the impedance) given by the above
formula. In most cases this is a small portion of a wire's inductance which
includes the effect of induction from magnetic fields outside of the wire
produced by the current in the wire. Unlike that external inductance, the
internal inductance is reduced by the skin effect, that is, at frequencies
where the skin depth is no longer large compared to the conductor's size. [7]
This small component of inductance approaches a value of       &#x03BC;  8
&#x03C0;      {\displaystyle {\frac {\mu }{8\pi }}}  [{\displaystyle {\frac
{\mu }{8\pi }}}] at low frequencies, regardless of the wire's radius. Its
reduction with increasing frequency, as the ratio of the skin depth to the
wire's radius falls below about 1, is plotted in the accompanying graph, and
accounts for the reduction in the telephone cable inductance with increasing
frequency in the table_below.
The internal component of a round wire's inductance vs. the ratio of skin depth
to radius. That component of the self inductance is reduced below Î¼ / 8Ï as
the skin depth becomes small (as frequency increases).
The ratio AC resistance to DC resistance of a round wire versus the ratio of
the wireâs radius to the skin depth. As the skin depth becomes small relative
to the radius, the ratio of AC to DC resistance approaches one half of the
ratio of the radius to the skin depth.
**** Resistance[edit] ****
The most important effect of the skin effect on the impedance of a single wire,
however, is the increase of the wire's resistance, and consequent losses. The
effective resistance due to a current confined near the surface of a large
conductor (much thicker than Î´) can be solved as if the current flowed
uniformly through a layer of thickness Î´ based on the DC resistivity of that
material. The effective cross-sectional area is approximately equal to Î´ times
the conductor's circumference. Thus a long cylindrical conductor such as a
wire, having a diameter D large compared to Î´, has a resistance approximately
that of a hollow tube with wall thickness Î´ carrying direct current. The AC
resistance of a wire of length L and resistivity     &#x03C1;   {\displaystyle
\rho }  [\rho ] is:
         R &#x2248;    L &#x03C1;   &#x03C0; ( D &#x2212; &#x03B4; ) &#x03B4;
      &#x2248;    L &#x03C1;   &#x03C0; D &#x03B4;      {\displaystyle R\approx
      {{L\rho } \over {\pi (D-\delta )\delta }}\approx {{L\rho } \over {\pi
      D\delta }}}  [{\displaystyle R\approx {{L\rho } \over {\pi (D-\delta
      )\delta }}\approx {{L\rho } \over {\pi D\delta }}}]
The final approximation above assumes     D &#x226B; &#x03B4;   {\displaystyle
D\gg \delta }  [D \gg \delta].
A convenient formula (attributed to F.E._Terman) for the diameter DW of a wire
of circular cross-section whose resistance will increase by 10% at frequency f
is:[8]
          D   W    =    200 &#xA0;  m m    f  /   H z       {\displaystyle D_
      {\mathrm {W} }={\frac {200~\mathrm {mm} }{\sqrt {f/\mathrm {Hz} }}}}
      [D_\mathrm{W} = {\frac{200~\mathrm{mm}}{\sqrt{f/\mathrm{Hz}}}}]
This formula for the increase in AC resistance is accurate only for an isolated
wire. For nearby wires, e.g. in a cable or a coil, the AC resistance is also
affected by proximity_effect, which can cause an additional increase in the AC
resistance.
***** Material effect on skin depth[edit] *****
In a good conductor, skin depth is proportional to square root of the
resistivity. This means that better conductors have a reduced skin depth. The
overall resistance of the better conductor remains lower even with the reduced
skin depth. However the better conductor will show a higher ratio between its
AC and DC resistance, when compared with a conductor of higher resistivity. For
example, at 60 Hz, a 2000_MCM (1000 square millimetre) copper conductor has 23%
more resistance than it does at DC. The same size conductor in aluminum has
only 10% more resistance with 60 Hz AC than it does with DC.[9]
Skin depth also varies as the inverse square root of the permeability of the
conductor. In the case of iron, its conductivity is about 1/7 that of copper.
However being ferromagnetic its permeability is about 10,000 times greater.
This reduces the skin depth for iron to about 1/38 that of copper, about 220
micrometres at 60 Hz. Iron wire is thus useless for AC power lines (except to
add mechanical strength by serving as a core to a non ferromagnetic conductor
like aluminum). The skin effect also reduces the effective thickness of
laminations in power transformers, increasing their losses.
Iron rods work well for direct-current (DC) welding but it is impossible to use
them at frequencies much higher than 60 Hz. At a few kilohertz, the welding rod
will glow red hot as current flows through the greatly increased AC resistance
resulting from the skin effect, with relatively little power remaining for the
arc itself. Only non-magnetic rods can be used for high-frequency welding.
At 1 megahertz the skin effect depth in wet soil is about 5.0 m, in seawater
it's about 0.25 m.[10]
***** Mitigation[edit] *****
A type of cable called litz_wire (from the German Litzendraht, braided wire) is
used to mitigate the skin effect for frequencies of a few kilohertz to about
one megahertz. It consists of a number of insulated wire strands woven together
in a carefully designed pattern, so that the overall magnetic field acts
equally on all the wires and causes the total current to be distributed equally
among them. With the skin effect having little effect on each of the thin
strands, the bundle does not suffer the same increase in AC resistance that a
solid conductor of the same cross-sectional area would due to the skin effect.
[11]
Litz wire is often used in the windings of high-frequency transformers to
increase their efficiency by mitigating both skin effect and proximity_effect.
Large power transformers are wound with stranded conductors of similar
construction to litz wire, but employing a larger cross-section corresponding
to the larger skin depth at mains frequencies.[12] Conductive threads composed
of carbon_nanotubes[13] have been demonstrated as conductors for antennas from
medium wave to microwave frequencies. Unlike standard antenna conductors, the
nanotubes are much smaller than the skin depth, allowing full utilization of
the thread's cross-section resulting in an extremely light antenna.
High-voltage, high-current overhead_power_lines often use aluminum_cable_with_a
steel_reinforcing_core; the higher resistance of the steel core is of no
consequence since it is located far below the skin depth where essentially no
AC current flows.
In applications where high currents (up to thousands of amperes) flow, solid
conductors are usually replaced by tubes, completely eliminating the inner
portion of the conductor where little current flows. This hardly affects the AC
resistance, but considerably reduces the weight of the conductor. The high
strength but low weight of tubes substantially increases span capability.
Tubular conductors are typical in electric power switchyards where the distance
between supporting insulators may be several meters. Long spans generally
exhibit physical sag but this does not affect electrical performance. To avoid
losses, the conductivity of the tube material must be high.
In high current situations where conductors (round or flat busbar) may be
between 5 and 50 mm thick the skin effect also occurs at sharp bends where the
metal is compressed inside the bend and stretched outside the bend. The shorter
path at the inner surface results in a lower resistance, which causes most of
the current to be concentrated close to the inner bend surface. This will cause
an increase in temperature rise in that region compared with the straight
(unbent) area of the same conductor. A similar skin effect occurs at the
corners of rectangular conductors (viewed in cross-section), where the magnetic
field is more concentrated at the corners than in the sides. This results in
superior performance (i.e. higher current with lower temperature rise) from
wide thin conductors â e.g. "ribbon" conductors, where the effects from
corners is effectively eliminated.
It follows that a transformer with a round core will be more efficient than an
equivalent-rated transformer having a square or rectangular core of the same
material.
Solid or tubular conductors may be silver-plated to take advantage of silver's
higher conductivity. This technique is particularly used at VHF to microwave
frequencies where the small skin depth requires only a very thin layer of
silver, making the improvement in conductivity very cost effective. Silver
plating is similarly used on the surface of waveguides used for transmission of
microwaves. This reduces attenuation of the propagating wave due to resistive
losses affecting the accompanying eddy currents; the skin effect confines such
eddy currents to a very thin surface layer of the waveguide structure. The skin
effect itself isn't actually combatted in these cases, but the distribution of
currents near the conductor's surface makes the use of precious metals (having
a lower resistivity) practical. Although it has a lower conductivity than
copper and silver, gold plating is also used, because unlike copper and silver,
it does not corrode. A thin oxidized layer of copper or silver would have a low
conductivity, and so would cause large power losses as the majority of the
current would still flow through this layer.
Recently, a method of layering non-magnetic and ferromagnetic materials with
nanometer scale thicknesses has been shown to mitigate the increased resistance
from the skin effect for very high frequency applications[14]. A working theory
is that the behavior of ferromagnetic materials in high frequencies results in
fields and/or currents that oppose those generated by relatively nonmagnetic
materials, but more work is needed to verify the exact mechanisms. As
experiments have shown, this has potential to greatly improve the efficiency of
conductors operating in tens of GHz or higher. This has strong ramifications
for 5G communications.
***** Examples[edit] *****
Skin depth vs. frequency for some materials at room temperature, red vertical
line denotes 50 Hz frequency:
    * Mn-Zn â magnetically soft ferrite
    * Al â metallic aluminum
    * Cu â metallic copper
    * steel 410 â magnetic stainless_steel
    * Fe-Si â grain-oriented_electrical_steel
    * Fe-Ni â high-permeability permalloy (80%Ni-20%Fe)
We can derive a practical formula for skin depth as follows:
         &#x03B4; =     2 &#x03C1;   ( 2 &#x03C0; f ) (  &#x03BC;  0
      &#x03BC;  r   )     &#x2248; 503     &#x03C1;   &#x03BC;  r   f
      {\displaystyle \delta ={\sqrt {{2\rho } \over {(2\pi f)(\mu _{0}\mu _
      {r})}}}\approx 503\,{\sqrt {\frac {\rho }{\mu _{r}f}}}}  [\delta=\sqrt{
      {2\rho }\over{(2 \pi f) (\mu_0 \mu_r)}} \approx 503\,\sqrt{\frac{\rho}
      {\mu_r f}}]
where
         &#x03B4; =   {\displaystyle \delta =}  [\delta =] the skin depth in
      meters
          &#x03BC;  r   =   {\displaystyle \mu _{r}=}  [\mu_r = ] the relative
      permeability of the medium (for copper,      &#x03BC;  r
      {\displaystyle \mu _{r}}  [\mu _{r}] = 1.00)
         &#x03C1; =   {\displaystyle \rho =}  [\rho = ] the resistivity of the
      medium in Î©Â·m, also equal to the reciprocal of its conductivity:
      &#x03C1; = 1  /  &#x03C3;   {\displaystyle \rho =1/\sigma }  [\rho = 1/
      \sigma  ] (for copper, Ï = 1.68Ã10â8 Î©Â·m)
         f =   {\displaystyle f=}  [f = ] the frequency of the current in Hz
Gold is a good conductor with a resistivity of 2.44Ã10â8 Î©Â·m and is
essentially nonmagnetic:      &#x03BC;  r   =   {\displaystyle \mu _{r}=}
[\mu_r = ] 1, so its skin depth at a frequency of 50 Hz is given by
         &#x03B4; = 503      2.44 &#x22C5;  10  &#x2212; 8     1 &#x22C5; 50
      = 11.1   m m    {\displaystyle \delta =503\,{\sqrt {\frac {2.44\cdot 10^
      {-8}}{1\cdot 50}}}=11.1\,\mathrm {mm} }  [\delta = 503 \,\sqrt{\frac{2.44
      \cdot 10^{-8}}{1 \cdot 50}}= 11.1\,\mathrm{mm} ]
Lead, in contrast, is a relatively poor conductor (among metals) with a
resistivity of 2.2Ã10â7 Î©Â·m, about 9 times that of gold. Its skin depth at
50 Hz is likewise found to be about 33 mm, or       9   = 3   {\displaystyle
{\sqrt {9}}=3}  [\sqrt{9} = 3 ] times that of gold.
Highly magnetic materials have a reduced skin depth owing to their large
permeability      &#x03BC;  r     {\displaystyle \mu _{r}}  [\mu _{r}] as was
pointed out above for the case of iron, despite its poorer conductivity. A
practical consequence is seen by users of induction_cookers, where some types
of stainless_steel cookware are unusable because they are not ferromagnetic.
At very high frequencies the skin depth for good conductors becomes tiny. For
instance, the skin depths of some common metals at a frequency of 10 GHz
(microwave region) are less than a micrometer:
 Skin depth at microwave
       frequencies
Conductor Skin depth (Î¼m)
Aluminum  0.820
Copper    0.652
Gold      0.753
Silver    0.634
Thus at microwave frequencies, most of the current flows in an extremely thin
region near the surface. Ohmic losses of waveguides at microwave frequencies
are therefore only dependent on the surface coating of the material. A layer of
silver 3 Î¼m thick evaporated on a piece of glass is thus an excellent
conductor at such frequencies.
In copper, the skin depth can be seen to fall according to the square root of
frequency:
   Skin depth in copper
Frequency Skin depth (Î¼m)
50 Hz    9220
60 Hz    8420
10 kHz   652
100 kHz  206
1 MHz    65.2
10 MHz   20.6
100 MHz  6.52
1 GHz    2.06
In Engineering Electromagnetics, Hayt points out[page needed] that in a power
station a busbar for alternating_current at 60 Hz with a radius larger than
one-third of an inch (8 mm) is a waste of copper, and in practice bus bars for
heavy AC current are rarely more than half an inch (12 mm) thick except for
mechanical reasons.
***** Skin effect reduction of the internal inductance of a conductor[edit]
*****
Refer to the diagram below showing the inner and outer conductors of a coaxial
cable. Since the skin effect causes a current at high frequencies to flow
mainly at the surface of a conductor, it can be seen that this will reduce the
magnetic field inside the wire, that is, beneath the depth at which the bulk of
the current flows. It can be shown that this will have a minor effect on the
self-inductance of the wire itself; see Skilling[15] or Hayt[16] for a
mathematical treatment of this phenomenon.
Note that the inductance considered in this context refers to a bare conductor,
not the inductance of a coil used as a circuit element. The inductance of a
coil is dominated by the mutual inductance between the turns of the coil which
increases its inductance according to the square of the number of turns.
However, when only a single wire is involved, then in addition to the "external
inductance" involving magnetic fields outside of the wire (due to the total
current in the wire) as seen in the white region of the figure below, there is
also a much smaller component of "internal inductance" due to the portion of
the magnetic field inside the wire itself, the green region in figure B. That
small component of the inductance is reduced when the current is concentrated
toward the skin of the conductor, that is, when the skin depth is not much
larger than the wire's radius, as will become the case at higher frequencies.
For a single wire, this reduction becomes of diminishing significance as the
wire becomes longer in comparison to its diameter, and is usually neglected.
However the presence of a second conductor in the case of a transmission line
reduces the extent of the external magnetic field (and of the total self-
inductance) regardless of the wire's length, so that the inductance decrease
due to the skin effect can still be important, For instance, in the case of a
telephone twisted pair, below, the inductance of the conductors substantially
decreases at higher frequencies where the skin effect becomes important. On the
other hand, when the external component of the inductance is magnified due to
the geometry of a coil (due to the mutual inductance between the turns), the
significance of the internal inductance component is even further dwarfed and
is ignored.
**** Inductance per length in a coaxial cable[edit] ****
Let the dimensions a, b, and c be the inner conductor radius, the shield (outer
conductor) inside radius and the shield outer radius respectively, as seen in
the crossection of figure A below.
Four stages of skin effect in a coax showing the effect on inductance. Diagrams
show a cross-section of the coaxial cable. Color code: black=overall insulating
sheath, tan=conductor, white=dielectric, green=current into the diagram,
blue=current coming out of the diagram, dashed black lines with
arrowheads=magnetic flux (B). The width of the dashed black lines is intended
to show relative strength of the magnetic field integrated over the
circumference at that radius. The four stages, A, B, C, and D are: non-
energized, low frequency, middle frequency and high frequency respectively.
There are three regions that may contain induced magnetic fields: the center
conductor, the dielectric and the outer conductor. In stage B, current covers
the conductors uniformly and there is a significant magnetic field in all three
regions. As the frequency is increased and the skin effect takes hold (C and D)
the magnetic field in the dielectric region is unchanged as it is proportional
to the total current flowing in the center conductor. In C, however, there is a
reduced magnetic field in the deeper sections of the inner conductor and the
outer sections of the shield (outer conductor). Thus there is less energy
stored in the magnetic field given the same total current, corresponding to a
reduced inductance. At an even higher frequency, D, the skin depth is tiny: all
current is confined to the surface of the conductors. The only magnetic field
is in the regions between the conductors; only the "external inductance"
remains.
For a given current, the total energy stored in the magnetic fields must be the
same as the calculated electrical energy attributed to that current flowing
through the inductance of the coax; that energy is proportional to the cable's
measured inductance.
The magnetic field inside a coaxial cable can be divided into three regions,
each of which will therefore contribute to the electrical inductance seen by a
length of cable.[17]
The inductance      L  cen      {\displaystyle L_{\text{cen}}\,}  [ L_\text
{cen} \, ] is associated with the magnetic field in the region with radius
r < a    {\displaystyle r<a\,}  [ r < a \, ], the region inside the center
conductor.
The inductance      L  ext      {\displaystyle L_{\text{ext}}\,}  [ L_\text
{ext} \, ] is associated with the magnetic field in the region     a < r < b
{\displaystyle a<r<b\,}  [ a < r < b \, ], the region between the two
conductors (containing a dielectric, possibly air).
The inductance      L  shd      {\displaystyle L_{\text{shd}}\,}  [ L_\text
{shd} \, ] is associated with the magnetic field in the region     b < r < c
{\displaystyle b<r<c\,}  [ b < r < c \, ], the region inside the shield
conductor.
The net electrical inductance is due to all three contributions:
          L  total   =  L  cen   +  L  shd   +  L  ext      {\displaystyle L_
      {\text{total}}=L_{\text{cen}}+L_{\text{shd}}+L_{\text{ext}}\,}  [ L_\text
      {total} = L_\text{cen} + L_\text{shd} + L_\text{ext}\, ]
    L  ext      {\displaystyle L_{\text{ext}}\,}  [ L_\text{ext} \, ] is not
changed by the skin effect and is given by the frequently cited formula for
inductance L per length D of a coaxial cable:
         L  /  D =    &#x03BC;  0    2 &#x03C0;    ln &#x2061;  (   b a   )
      {\displaystyle L/D={\frac {\mu _{0}}{2\pi }}\ln \left({\frac {b}
      {a}}\right)\,}  [ L/D = \frac{\mu_0}{2 \pi} \ln  \left( \frac {b}{a}
      \right)   \, ]
At low frequencies, all three inductances are fully present so that      L  DC
=  L  cen   +  L  shd   +  L  ext      {\displaystyle L_{\text{DC}}=L_{\text
{cen}}+L_{\text{shd}}+L_{\text{ext}}\,}  [ L_\text{DC} = L_\text{cen} + L_\text
{shd} + L_\text{ext}\, ].
At high frequencies, only the dielectric region has magnetic flux, so that
L  &#x221E;   =  L  ext      {\displaystyle L_{\infty }=L_{\text{ext}}\,}
[ L_\infty = L_\text{ext}\, ].
Most discussions of coaxial transmission lines assume they will be used for
radio frequencies, so equations are supplied corresponding only to the latter
case.
As the skin effect increases, the currents are concentrated near the outside of
the inner conductor (r=a) and the inside of the shield (r=b). Since there is
essentially no current deeper in the inner conductor, there is no magnetic
field beneath the surface of the inner conductor. Since the current in the
inner conductor is balanced by the opposite current flowing on the inside of
the outer conductor, there is no remaining magnetic field in the outer
conductor itself where     b < r < c    {\displaystyle b<r<c\,}  [ b < r < c \,
]. Only      L  ext     {\displaystyle L_{\text{ext}}}  [ L_\text{ext} ]
contributes to the electrical inductance at these higher frequencies.
Although the geometry is different, a twisted pair used in telephone lines is
similarly affected: at higher frequencies the inductance decreases by more than
20% as can be seen in the following table.
**** Characteristics of telephone cable as a function of frequency[edit] ****
Representative parameter data for 24 gauge PIC telephone cable at 21 Â°C
(70 Â°F).
Frequency (Hz) R (Î©/kmL (mH/km) G (Î¼S/kmC (nF/km)
1              172.24    0.6129    0.000      51.57
1k             172.28    0.6125    0.072      51.57
10k            172.70    0.6099    0.531      51.57
100k           191.63    0.5807    3.327      51.57
1M             463.59    0.5062    29.111     51.57
2M             643.14    0.4862    53.205     51.57
5M             999.41    0.4675    118.074    51.57
More extensive tables and tables for other gauges, temperatures and types are
available in Reeve.[18] Chen[19] gives the same data in a parameterized form
that he states is usable up to 50 MHz.
Chen[19] gives an equation of this form for telephone twisted pair:
         L ( f ) =     l  0   +  l  &#x221E;     (   f  f  m     )   b     1 +
      (   f  f  m     )   b         {\displaystyle L(f)={\frac {l_{0}+l_{\infty
      }\left({\frac {f}{f_{m}}}\right)^{b}}{1+\left({\frac {f}{f_{m}}}\right)^
      {b}}}\,}  [{\displaystyle L(f)={\frac {l_{0}+l_{\infty }\left({\frac {f}
      {f_{m}}}\right)^{b}}{1+\left({\frac {f}{f_{m}}}\right)^{b}}}\,}]
***** See also[edit] *****
    * Proximity_effect_(electromagnetism)
    * Penetration_depth
    * Eddy_currents
    * Litz_wire
    * Transformer
    * Induction_Cooking
    * Induction_heating
    * Magnetic_Reynolds_number
***** Notes[edit] *****
   1. ^ Note that the above equation for the current density inside the
      conductor as a function of depth applies to cases where the usual
      approximation for the skin depth holds. In the extreme cases where it
      doesn't, the exponential decrease with respect to the skin depth still
      applies to the magnitude of the induced currents, however the imaginary
      part of the exponent in that equation, and thus the phase velocity inside
      the material, are altered with respect to that equation.
***** References[edit] *****
   1. ^ "These emf's are greater at the center than at the circumference, so
      the potential difference tends to establish currents that oppose the
      current at the center and assist it at the circumference"Fink, Donald G.;
      Beaty, H. Wayne (2000). Standard Handbook for Electrical Engineers (14th
      ed.). McGraw-Hill. p. 2â50. ISBN 978-0-07-022005-8.
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
   3. ^ "To understand skin effect, you must first understand how eddy currents
      operate..."Johnson, Howard; Graham, Martain (2003). High-Speed Signal
      propagation Advanced Black Magic (3rd ed.). Prentice Hall. p. 58-78.
      ISBN 978-0-13-084408-8.
   4. ^Hayt, William H. (1989), Engineering Electromagnetics (5th ed.), McGraw-
      Hill, ISBN 978-0070274068
   5. ^ Vander_Vorst,_Rosen_&_Kotsuka_(2006)
   6. ^ The formula as shown is algebraically equivalent to the formula found
      on page 130 Jordan_(1968, p. 130)
   7. ^ a bWeeks, Walter L. (1981), Transmission and Distribution of Electrical
      Energy, Harper & Row, ISBN 978-0060469825
   8. ^ Hayt_(1981, pp. 303)
   9. ^ Terman_1943, p. ??
  10. ^Fink, Donald G.; Beatty, H. Wayne, eds. (1978), Standard Handbook for
      Electrical Engineers (11th ed.), McGraw Hill, p. Table 18â21
  11. ^ Popovic_&_Popovic_1999, p. 385
  12. ^ Xi_Nan_&_Sullivan_2005
  13. ^Central Electricity Generating Board (1982). Modern Power Station
      Practice. Pergamon Press.
  14. ^"Spinning_Carbon_Nanotubes_Spawns_New_Wireless_Applications".
      Sciencedaily.com. 2009-03-09. Retrieved 2011-11-08.
  15. ^ [A. Rahimi and Y.-K. Yoon "Study on Cu/Ni Nano Superlattice Conductors
      for Reduced RF Loss," IEEE Microwave and Wireless Components Letters,
      vol. 26, no. 4, Mar. 16, 2016, pp. 258-260 http://ieeexplore.ieee.org/
      stamp/stamp.jsp?arnumber=7434554]
  16. ^ Skilling_(1951, pp. 157â159)
  17. ^ Hayt_(1981, pp. 434â439)
  18. ^ Hayt_(1981, p. 434)
  19. ^ Reeve_(1995, p. 558)
  20. ^ a b Chen_(2004, p. 26)
    * Chen, Walter Y. (2004), Home Networking Basics, Prentice Hall, ISBN 978-
      0-13-016511-4
Hayt, William (1981), Engineering Electromagnetics (4th ed.), McGraw-Hill,
ISBN 978-0-07-027395-5
Hayt, William Hart (2006), Engineering Electromagnetics (7th ed.), New York:
McGraw Hill, ISBN 978-0-07-310463-8
Nahin, Paul J. Oliver Heaviside: Sage in Solitude. New York: IEEE Press, 1988.
ISBN 0-87942-238-6.
Ramo, S., J. R. Whinnery, and T. Van Duzer. Fields and Waves in Communication
Electronics. New York: John Wiley & Sons, Inc., 1965.
Ramo, Whinnery, Van Duzer (1994). Fields and Waves in Communications
Electronics. John Wiley and Sons.CS1 maint: Multiple names: authors list (link)
Reeve, Whitman D. (1995), Subscriber Loop Signaling and Transmission Handbook,
IEEE Press, ISBN 978-0-7803-0440-6
Skilling, Hugh H. (1951), Electric Transmission Lines, McGraw-Hill
Terman,_F._E. (1943), Radio Engineers' Handbook, New York: McGraw-Hill
Xi Nan; Sullivan, C. R. (2005), "An_equivalent_complex_permeability_model_for
litz-wire_windings", Industry Applications Conference, 3: 2229â2235, doi:
10.1109/IAS.2005.1518758, ISBN 978-0-7803-9208-3, ISSN 0197-2618
Jordan, Edward Conrad (1968), Electromagnetic Waves and Radiating Systems,
Prentice Hall, ISBN 978-0-13-249995-8
Vander Vorst, Andre; Rosen, Arye; Kotsuka, Youji (2006), RF/Microwave
Interaction with Biological Tissues, John Wiley and Sons, Inc., ISBN 978-0-471-
73277-8
Popovic, Zoya; Popovic, Branko (1999), Chapter 20,The Skin Effect, Introductory
Electromagnetics, Prentice-Hall, ISBN 978-0-201-32678-9
***** External links[edit] *****
 Wikimedia Commons has media related to Skin_effect.
    * 100%_Skin_Depths_Table
    * Conductor_Bulk_Resistivity_&_Skin_Depths
    * Calculator_for_Skin_Effect_Depth
    * Skin_Effect_Relevance_in_Speaker_Cables

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Skin_effect&oldid=907007701"
Categories:
    * Electromagnetism
    * Electrical_parameters
Hidden categories:
    * Wikipedia_articles_needing_page_number_citations_from_October_2016
    * CS1_maint:_Multiple_names:_authors_list
    * Commons_category_link_from_Wikidata
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 19 July 2019, at 20:20 (UTC).
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
