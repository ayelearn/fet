The following text has been accessed from https://en.wikipedia.org/wiki/Poynting_vector at Fri Aug 9 03:43:29 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Poynting vector ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Dipole_radiation of a dipole vertically in the page showing electric field
strength (colour) and Poynting vector (arrows) in the plane of the page.
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
    * Poynting vector
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
In physics, the Poynting vector represents the directional energy_flux (the
energy transfer per unit area per unit time) of an electromagnetic_field. The
SI unit of the Poynting vector is the watt per square metre (W/m2). It is named
after its discoverer John_Henry_Poynting who first derived it in 1884.[1]:132
Oliver_Heaviside also discovered it independently.
⁰
***** Contents *****
    * 1_Definition
    * 2_Interpretation
    * 3_Formulation_in_terms_of_microscopic_fields
    * 4_Time-averaged_Poynting_vector
    * 5_Examples_and_applications
          o 5.1_Coaxial_cable
          o 5.2_Resistive_dissipation
          o 5.3_Plane_waves
          o 5.4_Radiation_pressure
          o 5.5_Static_fields
    * 6_Adding_the_curl_of_a_vector_field
    * 7_References
    * 8_Further_reading
***** Definition[edit] *****
In Poynting's original paper and in many textbooks, the Poynting vector is
defined as[2][3][4]
          S  =  E  &#x00D7;  H  ,   {\displaystyle \mathbf {S} =\mathbf {E}
      \times \mathbf {H} ,}  [\mathbf {S} =\mathbf {E} \times \mathbf {H} ,]
where bold letters represent vectors and
    * E is the electric_field vector;
    * H is the magnetic_field's auxiliary field vector.
This expression is often called the Abraham form.[5] The Poynting vector is
usually denoted by S or N.
In the "microscopic" version of Maxwell's equations, this definition must be
replaced by a definition in terms of the electric field E and the magnetic
field B (it is described later in the article).
It is also possible to combine the electric_displacement_field D with the
magnetic field B to get the Minkowski form of the Poynting vector, or use D and
H to construct yet another version. The choice has been controversial: Pfeifer
et al.[6] summarize and to a certain extent resolve the century-long dispute
between proponents of the Abraham and Minkowski forms (see AbrahamâMinkowski
controversy).
The Poynting vector represents the particular case of an energy flux vector for
electromagnetic energy. However, any type of energy has its direction of
movement in space, as well as its density, so energy flux vectors can be
defined for other types of energy as well, e.g., for mechanical_energy. The
UmovâPoynting vector[7] discovered by Nikolay_Umov in 1874 describes energy
flux in liquid and elastic media in a completely generalized view.
***** Interpretation[edit] *****
A DC circuit consisting of a battery (V) and resistor (R), showing the
direction of the Poynting vector (S, blue arrows) in the space surrounding it,
along with the fields it is derived from; the electric_field (E, red arrows)
and the magnetic_field (H, green arrows). In the region around the battery the
Poynting vector is directed outward, indicating power flowing out of the
battery into the fields; in the region around the resistor the vector is
directed inward, indicating field power flowing into the resistor. Across any
plane P between the battery and resistor, the Poynting flux is in the direction
of the resistor. The magnitudes (lengths) of the vectors are not shown
accurately; only the directions are significant.
The Poynting vector appears in Poynting's_theorem (see that article for the
derivation), an energy-conservation law:
            &#x2202; u   &#x2202; t    = &#x2212;  &#x2207;  &#x22C5;  S
      &#x2212;   J   f     &#x22C5;  E  ,   {\displaystyle {\frac {\partial u}
      {\partial t}}=-\mathbf {\nabla } \cdot \mathbf {S} -\mathbf {J_{\mathrm
      {f} }} \cdot \mathbf {E} ,}  [{\frac {\partial u}{\partial t}}=-\mathbf
      {\nabla } \cdot \mathbf {S} -\mathbf {J_{\mathrm {f} }} \cdot \mathbf {E}
      ,]
where Jf is the current_density of free_charges and u is the electromagnetic
energy density for linear, nondispersive materials, given by
         u =   1 2     (   E  &#x22C5;  D  +  B  &#x22C5;  H   )   ,
      {\displaystyle u={\frac {1}{2}}\!\left(\mathbf {E} \cdot \mathbf {D}
      +\mathbf {B} \cdot \mathbf {H} \right)\!,}  [u={\frac {1}{2}}\!\left
      (\mathbf {E} \cdot \mathbf {D} +\mathbf {B} \cdot \mathbf {H} \right)\!,]
where
    * E is the electric field;
    * D is the electric displacement field;
    * B is the magnetic field;
    * H is the magnetic auxiliary field.[8]:258â260
The first term in the right-hand side represents the electromagnetic energy
flow into a small volume, while the second term subtracts the work done by the
field on free electrical currents, which thereby exits from electromagnetic
energy as dissipation, heat, etc. In this definition, bound electrical currents
are not included in this term, and instead contribute to S and u.
For linear, nondispersive and isotropic (for simplicity) materials, the
constitutive_relations can be written as
          D  = &#x03B5;  E  ,   H  =   1 &#x03BC;    B  ,   {\displaystyle
      \mathbf {D} =\varepsilon \mathbf {E} ,\quad \mathbf {H} ={\frac {1}{\mu
      }}\mathbf {B} ,}  [\mathbf {D} =\varepsilon \mathbf {E} ,\quad \mathbf
      {H} ={\frac {1}{\mu }}\mathbf {B} ,]
where
    * Îµ is the permittivity of the material;
    * Î¼ is the permeability of the material.[8]:258â260
Here Îµ and Î¼ are scalar, real-valued constants independent of position,
direction, and frequency.
In principle, this limits Poynting's theorem in this form to fields in vacuum
and nondispersive linear materials. A generalization to dispersive materials is
possible under certain circumstances at the cost of additional terms.[8]:
262â264
***** Formulation in terms of microscopic fields[edit] *****
The "microscopic" (differential) version of Maxwell's equations admits only the
fundamental fields E and B, without a built-in model of material media. Only
the vacuum permittivity and permeability are used, and there is no D or H. When
this model is used, the Poynting vector is defined as
          S  =   1  &#x03BC;  0      E  &#x00D7;  B  ,   {\displaystyle \mathbf
      {S} ={\frac {1}{\mu _{0}}}\mathbf {E} \times \mathbf {B} ,}  [\mathbf {S}
      ={\frac {1}{\mu _{0}}}\mathbf {E} \times \mathbf {B} ,]
where
    * Î¼0 is the vacuum_permeability;
    * E is the electric field;
    * B is the magnetic field.
This is actually the general expression of the Poynting vector.[9] The
corresponding form of Poynting's_theorem is
            &#x2202; u   &#x2202; t    = &#x2212; &#x2207; &#x22C5;  S
      &#x2212;  J  &#x22C5;  E  ,   {\displaystyle {\frac {\partial u}{\partial
      t}}=-\nabla \cdot \mathbf {S} -\mathbf {J} \cdot \mathbf {E} ,}  [{\frac
      {\partial u}{\partial t}}=-\nabla \cdot \mathbf {S} -\mathbf {J} \cdot
      \mathbf {E} ,]
where J is the total current_density and the energy density u is given by
         u =   1 2     (   &#x03B5;  0     E   2   +   1  &#x03BC;  0       B
      2    )   ,   {\displaystyle u={\frac {1}{2}}\!\left(\varepsilon _
      {0}\mathbf {E} ^{2}+{\frac {1}{\mu _{0}}}\mathbf {B} ^{2}\right)\!,}  [u=
      {\frac {1}{2}}\!\left(\varepsilon _{0}\mathbf {E} ^{2}+{\frac {1}{\mu _
      {0}}}\mathbf {B} ^{2}\right)\!,]
where Îµ0 is the vacuum_permittivity. It can be derived directly from Maxwell's
equations_in_terms_of_total_charge_and_current and the Lorentz_force law only.
The two alternative definitions of the Poynting vector are equal in vacuum or
in non-magnetic materials, where B = Î¼0H. In all other cases, they differ in
that S = (1/Î¼0) E Ã B and the corresponding u are purely radiative, since the
dissipation term âJ â E covers the total current, while the E Ã H
definition has contributions from bound currents which are then excluded from
the dissipation term.[10]
Since only the microscopic fields E and B occur in the derivation of S = (1/
Î¼0) E Ã B, assumptions about any material present are completely avoided, and
Poynting vector and theorem are universally valid, in vacuum as in all kinds of
material. This is especially true[clarification_needed] for the electromagnetic
energy density, in contrast to the "macroscopic" form E Ã H.[10]
***** Time-averaged Poynting vector[edit] *****
The field lines of the time-averaged Poynting vector of an electric dipole
close to a mirror create complex patterns.
The above form for the Poynting vector represents the instantaneous power flow
due to instantaneous electric and magnetic fields. More commonly, problems in
electromagnetics are solved in terms of sinusoidally varying fields at a
specified frequency. The results can then be applied more generally, for
instance, by representing incoherent radiation as a superposition of such waves
at different frequencies and with fluctuating amplitudes.
We would thus not be considering the instantaneous E(t) and H(t) used above,
but rather a complex (vector) amplitude for each which describes a coherent
wave's phase (as well as amplitude) using phasor notation. Note that these
complex amplitude vectors are not functions of time, as they are understood to
refer to oscillations over all time. A phasor such as       E   m
{\displaystyle \mathbf {E_{\mathrm {m} }} }  [{\displaystyle \mathbf {E_
{\mathrm {m} }} }] is understood to signify a sinusoidally varying field whose
instantaneous amplitude E(t) follows the real part of       E   m      e  j
&#x03C9; t     {\displaystyle \mathbf {E_{\mathrm {m} }} e^{j\omega t}}  [
{\displaystyle \mathbf {E_{\mathrm {m} }} e^{j\omega t}}] where Ï is the
(radian) frequency of the sinusoidal wave being considered.
In the time domain it will be seen that the instantaneous power flow will be
fluctuating at a frequency of 2Ï. But what is normally of interest is the
average power flow in which those fluctuations are not considered. In the math
below, this is accomplished by integrating over a full cycle     T = 2 &#x03C0;
/  &#x03C9;   {\displaystyle T=2\pi /\omega }  [{\displaystyle T=2\pi /\omega
}]. The following quantity, still referred to as a "Poynting vector", is
expressed directly in terms of the phasors as:
     S    m    =    1 2      E    m    &#x00D7;   H    m    &#x2217;   ,
{\displaystyle \mathbf {S} _{\mathrm {m} }={\tfrac {1}{2}}\mathbf {E} _{\mathrm
{m} }\times \mathbf {H} _{\mathrm {m} }^{*},}  [{\displaystyle \mathbf {S} _
{\mathrm {m} }={\tfrac {1}{2}}\mathbf {E} _{\mathrm {m} }\times \mathbf {H} _
{\mathrm {m} }^{*},}]
where â denotes the complex conjugate. The time-averaged power flow
(according to the instantaneous Poynting vector averaged over a full cycle, for
instance) is then given by the real part of       S    m      {\displaystyle
\mathbf {S} _{\mathrm {m} }}  [{\displaystyle \mathbf {S} _{\mathrm {m} }}].
The imaginary part is usually ignored, however it signifies "reactive power"
such as the interference due to a standing_wave or the near_field of an
antenna. In a single electromagnetic plane_wave (rather than a standing wave
which can be described as two such waves travelling in opposite directions), E
and H are exactly in phase, so       S    m      {\displaystyle \mathbf {S} _
{\mathrm {m} }}  [{\displaystyle \mathbf {S} _{\mathrm {m} }}] is simply a real
number according to the above definition.
The equivalence of     Re &#x2061; (   S    m    )   {\displaystyle
\operatorname {Re} (\mathbf {S} _{\mathrm {m} })}  [{\displaystyle
\operatorname {Re} (\mathbf {S} _{\mathrm {m} })}] to the time-average of the
instantaneous Poynting vector S can be shown as follows.
              S  ( t )    =  E  ( t ) &#x00D7;  H  ( t )       = Re   (    E
      m     e  j &#x03C9; t    )  &#x00D7; Re   (    H    m     e  j &#x03C9; t
      )        =    1 2      (    E    m     e  j &#x03C9; t   +   E    m
      &#x2217;    e  &#x2212; j &#x03C9; t    )  &#x00D7;    1 2      (    H
      m     e  j &#x03C9; t   +   H    m    &#x2217;    e  &#x2212; j &#x03C9;
      t    )        =    1 4      (    E    m    &#x00D7;   H    m    &#x2217;
      +   E    m    &#x2217;   &#x00D7;   H    m    +   E    m    &#x00D7;   H
      m     e  2 j &#x03C9; t   +   E    m    &#x2217;   &#x00D7;   H    m
      &#x2217;    e  &#x2212; 2 j &#x03C9; t    )        =    1 2    Re
      (    E    m    &#x00D7;   H    m    &#x2217;    )  +    1 2    Re
      (    E    m    &#x00D7;   H    m     e  2 j &#x03C9; t    )   .
      {\displaystyle {\begin{aligned}\mathbf {S} (t)&=\mathbf {E} (t)\times
      \mathbf {H} (t)\\&=\operatorname {Re} \!\left(\mathbf {E} _{\mathrm {m}
      }e^{j\omega t}\right)\times \operatorname {Re} \!\left(\mathbf {H} _
      {\mathrm {m} }e^{j\omega t}\right)\\&={\tfrac {1}{2}}\!\left(\mathbf {E}
      _{\mathrm {m} }e^{j\omega t}+\mathbf {E} _{\mathrm {m} }^{*}e^{-j\omega
      t}\right)\times {\tfrac {1}{2}}\!\left(\mathbf {H} _{\mathrm {m} }e^
      {j\omega t}+\mathbf {H} _{\mathrm {m} }^{*}e^{-j\omega t}\right)\\&=
      {\tfrac {1}{4}}\!\left(\mathbf {E} _{\mathrm {m} }\times \mathbf {H} _
      {\mathrm {m} }^{*}+\mathbf {E} _{\mathrm {m} }^{*}\times \mathbf {H} _
      {\mathrm {m} }+\mathbf {E} _{\mathrm {m} }\times \mathbf {H} _{\mathrm
      {m} }e^{2j\omega t}+\mathbf {E} _{\mathrm {m} }^{*}\times \mathbf {H} _
      {\mathrm {m} }^{*}e^{-2j\omega t}\right)\\&={\tfrac {1}{2}}\operatorname
      {Re} \!\left(\mathbf {E} _{\mathrm {m} }\times \mathbf {H} _{\mathrm {m}
      }^{*}\right)+{\tfrac {1}{2}}\operatorname {Re} \!\left(\mathbf {E} _
      {\mathrm {m} }\times \mathbf {H} _{\mathrm {m} }e^{2j\omega
      t}\right)\!.\end{aligned}}}  [{\displaystyle {\begin{aligned}\mathbf {S}
      (t)&=\mathbf {E} (t)\times \mathbf {H} (t)\\&=\operatorname {Re} \!\left
      (\mathbf {E} _{\mathrm {m} }e^{j\omega t}\right)\times \operatorname {Re}
      \!\left(\mathbf {H} _{\mathrm {m} }e^{j\omega t}\right)\\&={\tfrac {1}
      {2}}\!\left(\mathbf {E} _{\mathrm {m} }e^{j\omega t}+\mathbf {E} _
      {\mathrm {m} }^{*}e^{-j\omega t}\right)\times {\tfrac {1}{2}}\!\left
      (\mathbf {H} _{\mathrm {m} }e^{j\omega t}+\mathbf {H} _{\mathrm {m} }^
      {*}e^{-j\omega t}\right)\\&={\tfrac {1}{4}}\!\left(\mathbf {E} _{\mathrm
      {m} }\times \mathbf {H} _{\mathrm {m} }^{*}+\mathbf {E} _{\mathrm {m} }^
      {*}\times \mathbf {H} _{\mathrm {m} }+\mathbf {E} _{\mathrm {m} }\times
      \mathbf {H} _{\mathrm {m} }e^{2j\omega t}+\mathbf {E} _{\mathrm {m} }^
      {*}\times \mathbf {H} _{\mathrm {m} }^{*}e^{-2j\omega t}\right)\\&=
      {\tfrac {1}{2}}\operatorname {Re} \!\left(\mathbf {E} _{\mathrm {m}
      }\times \mathbf {H} _{\mathrm {m} }^{*}\right)+{\tfrac {1}
      {2}}\operatorname {Re} \!\left(\mathbf {E} _{\mathrm {m} }\times \mathbf
      {H} _{\mathrm {m} }e^{2j\omega t}\right)\!.\end{aligned}}}]
The average of the instantaneous Poynting vector S over time is given by:
         &#x27E8;  S  &#x27E9; =   1 T    &#x222B;  0   T    S  ( t )  d t =
      1 T    &#x222B;  0   T     [     1 2    Re   (    E    m    &#x00D7;   H
      m    &#x2217;    )  +    1 2    Re   (     E    m     &#x00D7;    H    m
      e  2 j &#x03C9; t    )   ]  d t .   {\displaystyle \langle \mathbf {S}
      \rangle ={\frac {1}{T}}\int _{0}^{T}\mathbf {S} (t)\,dt={\frac {1}
      {T}}\int _{0}^{T}\!\left[{\tfrac {1}{2}}\operatorname {Re} \!\left
      (\mathbf {E} _{\mathrm {m} }\times \mathbf {H} _{\mathrm {m} }^
      {*}\right)+{\tfrac {1}{2}}\operatorname {Re} \!\left({\mathbf {E} _
      {\mathrm {m} }}\times {\mathbf {H} _{\mathrm {m} }}e^{2j\omega
      t}\right)\right]dt.}  [{\displaystyle \langle \mathbf {S} \rangle ={\frac
      {1}{T}}\int _{0}^{T}\mathbf {S} (t)\,dt={\frac {1}{T}}\int _{0}^
      {T}\!\left[{\tfrac {1}{2}}\operatorname {Re} \!\left(\mathbf {E} _
      {\mathrm {m} }\times \mathbf {H} _{\mathrm {m} }^{*}\right)+{\tfrac {1}
      {2}}\operatorname {Re} \!\left({\mathbf {E} _{\mathrm {m} }}\times
      {\mathbf {H} _{\mathrm {m} }}e^{2j\omega t}\right)\right]dt.}]
The second term is the double-frequency component having an average value of
zero, so we find:
         &#x27E8;  S  &#x27E9; = Re   (     1 2       E    m     &#x00D7;   H
      m    &#x2217;    )  = Re   (   S    m    )    {\displaystyle \langle
      \mathbf {S} \rangle =\operatorname {Re} \!\left({\tfrac {1}{2}}{\mathbf
      {E} _{\mathrm {m} }}\times \mathbf {H} _{\mathrm {m} }^
      {*}\right)=\operatorname {Re} \!\left(\mathbf {S} _{\mathrm {m} }\right)}
      [{\displaystyle \langle \mathbf {S} \rangle =\operatorname {Re} \!\left(
      {\tfrac {1}{2}}{\mathbf {E} _{\mathrm {m} }}\times \mathbf {H} _{\mathrm
      {m} }^{*}\right)=\operatorname {Re} \!\left(\mathbf {S} _{\mathrm {m}
      }\right)}]
According to some conventions the factor of 1/2 in the above definition may be
left out. Multiplication by 1/2 is required to properly describe the power flow
since the magnitudes of       E    m      {\displaystyle \mathbf {E} _{\mathrm
{m} }}  [{\displaystyle \mathbf {E} _{\mathrm {m} }}] and       H    m
{\displaystyle \mathbf {H} _{\mathrm {m} }}  [{\displaystyle \mathbf {H} _
{\mathrm {m} }}] refer to the peak fields of the oscillating quantities. If
rather the fields are described in terms of their root_mean_square (rms) values
(which are each smaller by the factor       2    /  2   {\displaystyle {\sqrt
{2}}/2}  [{\sqrt  {2}}/2]), then the correct average power flow is obtained
without multiplication by 1/2.
***** Examples and applications[edit] *****
**** Coaxial cable[edit] ****
Poynting vector in a coaxial cable, shown in red.
For example, the Poynting vector within the dielectric insulator of a coaxial
cable is nearly parallel to the wire axis (assuming no fields outside the cable
and a wavelength longer than the diameter of the cable, including DC).
Electrical energy delivered to the load is flowing entirely through the
dielectric between the conductors. Very little energy flows in the conductors
themselves, since the electric field strength is nearly zero. The energy
flowing in the conductors flows radially into the conductors and accounts for
energy lost to resistive heating of the conductor. No energy flows outside the
cable, either, since there the magnetic fields of inner and outer conductors
cancel to zero.
**** Resistive dissipation[edit] ****
If a conductor has significant resistance, then, near the surface of that
conductor, the Poynting vector would be tilted toward and impinge upon the
conductor. Once the Poynting vector enters the conductor, it is bent to a
direction that is almost perpendicular to the surface.[11]:61 This is a
consequence of Snell's_law and the very slow speed of light inside a conductor.
The definition and computation of the speed of light in a conductor can be
given.[12]:402 Inside the conductor, the Poynting vector represents energy flow
from the electromagnetic_field into the wire, producing resistive Joule_heating
in the wire. For a derivation that starts with Snell's law see Reitz page 454.
[13]:454
**** Plane waves[edit] ****
In a propagating sinusoidal linearly_polarized electromagnetic plane_wave of a
fixed frequency, the Poynting vector always points in the direction of
propagation while oscillating in magnitude. The time-averaged magnitude of the
Poynting vector is found as above to be:
         &#x27E8; S &#x27E9; =   1  2 &#x03B7;     |   E   m      |   2
      {\displaystyle \langle S\rangle ={\frac {1}{2\eta }}|E_{\mathrm {m} }|^
      {2}}  [{\displaystyle \langle S\rangle ={\frac {1}{2\eta }}|E_{\mathrm
      {m} }|^{2}}]
where Em is the complex amplitude of the electric field and Î· is the
characteristic impedance of the transmission medium, or just Î·0     &#x2248;
{\displaystyle \approx }  [\approx ] 377Î© for a plane wave in free space. This
directly follows from the above expression for the average Poynting vector
using phasor quantities, and the fact that in a plane wave the magnetic field
H   m      {\displaystyle H_{\mathrm {m} }}  [{\displaystyle H_{\mathrm {m} }}]
is equal to the electric field      E   m      {\displaystyle E_{\mathrm {m} }}
[{\displaystyle E_{\mathrm {m} }}] divided by Î· (and thus exactly in phase).
In optics, the time-averaged value of the radiated flux is technically known as
the irradiance, more often simply referred to as the intensity.
**** Radiation pressure[edit] ****
The density of the linear momentum of the electromagnetic field is S/c2 where S
is the magnitude of the Poynting vector and c is the speed of light in free
space. The radiation_pressure exerted by an electromagnetic wave on the surface
of a target is given by
          P   r a d    =    &#x27E8; S &#x27E9;   c    .   {\displaystyle P_
      {\mathrm {rad} }={\frac {\langle S\rangle }{\mathrm {c} }}.}  [P_{\mathrm
      {rad} }={\frac {\langle S\rangle }{\mathrm {c} }}.]
**** Static fields[edit] ****
Poynting vector in a static field, where E is the electric field, H the
magnetic field, and S the Poynting vector.
The consideration of the Poynting vector in static fields shows the
relativistic nature of the Maxwell equations and allows a better understanding
of the magnetic component of the Lorentz_force, q(v Ã B). To illustrate, the
accompanying picture is considered, which describes the Poynting vector in a
cylindrical capacitor, which is located in an H field (pointing into the page)
generated by a permanent magnet. Although there are only static electric and
magnetic fields, the calculation of the Poynting vector produces a clockwise
circular flow of electromagnetic energy, with no beginning or end.
While the circulating energy flow may seem nonsensical or paradoxical, it is
necessary to maintain conservation_of_momentum. Momentum density is
proportional to energy flow density, so the circulating flow of energy contains
an angular momentum.[14] This is the cause of the magnetic component of the
Lorentz force which occurs when the capacitor is discharged. During discharge,
the angular momentum contained in the energy flow is depleted as it is
transferred to the charges of the discharge current crossing the magnetic
field.
***** Adding the curl of a vector field[edit] *****
The Poynting vector occurs in Poynting's theorem only through its divergence
â â S, that is, it is only required that the surface_integral of the
Poynting vector around a closed surface describe the net flow of
electromagnetic energy into or out of the enclosed volume. This means that
adding a solenoidal_vector_field (one with zero divergence) to S will result in
another field which satisfies this required property of a Poynting vector field
according to Poynting's theorem. Since the divergence_of_any_curl_is_zero, one
can add the curl of any vector field to the Poynting vector and the resulting
vector field S' will still satisfy Poynting's theorem.[8]:258â260
However the theory of special_relativity, in which energy and momentum are
defined locally and invariantly via the stressâenergy_tensor, shows that the
above-given expression for the Poynting vector is unique.[8]:
258â260,605â612
***** References[edit] *****
   1. ^Stratton, Julius Adams (1941). Electromagnetic_Theory (1st ed.). New
      York: McGraw-Hill. ISBN 978-0-470-13153-4.
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
   3. ^Poynting,_John_Henry (1884). "On the Transfer of Energy in the
      Electromagnetic Field". Philosophical Transactions of the Royal Society
      of London. 175: 343â361. doi:10.1098/rstl.1884.0016.
   4. ^Grant, Ian S.; Phillips, William R. (1990). Electromagnetism (2nd ed.).
      New York: John Wiley & Sons. ISBN 978-0-471-92712-9.
   5. ^Griffiths, David J. (2012). Introduction_to_Electrodynamics (3rd ed.).
      Boston: Addison-Wesley. ISBN 978-0-321-85656-2.
   6. ^Kinsler, Paul; Favaro, Alberto; McCall, Martin W. (2009). "Four Poynting
      Theorems". European Journal of Physics. 30 (5): 983. arXiv:0908.1721.
      Bibcode:2009EJPh...30..983K. doi:10.1088/0143-0807/30/5/007.
   7. ^Pfeifer, Robert N. C.; Nieminen, Timo A.; Heckenberg, Norman R.;
      Rubinsztein-Dunlop, Halina (2007). "Momentum of an Electromagnetic Wave
      in Dielectric Media". Reviews of Modern Physics. 79 (4): 1197. arXiv:
      0710.0461. Bibcode:2007RvMP...79.1197P. doi:10.1103/RevModPhys.79.1197.
   8. ^Umov,_Nikolay_Alekseevich (1874). "Ein_Theorem_Ã¼ber_die
      Wechselwirkungen_in_Endlichen_Entfernungen". Zeitschrift fÃ¼r Mathematik
      und Physik. 19: 97â114.
   9. ^ a b c d eJackson, John David (1998). Classical_Electrodynamics (3rd
      ed.). New York: John Wiley & Sons. ISBN 978-0-471-30932-1.
  10. ^Zangwill, Andrew (2013). Modern Electrodynamics. Cambridge University
      Press. p. 508. ISBN 9780521896979.
  11. ^ a bRichter, Felix; Florian, Matthias; Henneberger, Klaus (2008).
      "Poynting's Theorem and Energy Conservation in the Propagation of Light
      in Bounded Media". Europhysics Letters Association. 81 (6): 67005. arXiv:
      0710.0515. Bibcode:2008EL.....8167005R. doi:10.1209/0295-5075/81/67005.
  12. ^Harrington, Roger F. (2001). Time-Harmonic_Electromagnetic_Fields (2nd
      ed.). McGraw-Hill. ISBN 978-0-471-20806-8.
  13. ^Hayt, William (2011). Engineering_Electromagnetics (4th ed.). New York:
      McGraw-Hill. ISBN 978-0-07-338066-7.
  14. ^Reitz, John R.; Milford, Frederick J.; Christy, Robert W. (2008).
      Foundations_of_Electromagnetic_Theory (4th ed.). Boston: Addison-Wesley.
      ISBN 978-0-321-58174-7.
  15. ^Feynman,_Richard_Phillips (2011). The_Feynman_Lectures_on_Physics. Vol.
      II: Mainly Electromagnetism and Matter (The New Millennium ed.). New
      York: Basic Books. ISBN 978-0-465-02494-0.
***** Further reading[edit] *****
 Wikiquote has quotations related to: Poynting_vector
    * Becker, Richard (1982). Electromagnetic_Fields_and_Interactions (1st
      ed.). Mineola, New York: Dover Publications. ISBN 978-0-486-64290-1.
Edminister, Joseph; Nahvi, Mahmood (2013). Electromagnetics (4th ed.). New
York: McGraw-Hill. ISBN 978-0-07-183149-9.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Poynting_vector&oldid=906355960"
Categories:
    * Electromagnetic_radiation
    * Optics
    * Vectors_(mathematics_and_physics)
Hidden categories:
    * CS1:_long_volume_value
    * Wikipedia_articles_needing_clarification_from_October_2015
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
    * Wikiquote
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Italiano
    * ×¢××¨××ª
    * Lumbaart
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 15 July 2019, at 09:28 (UTC).
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
