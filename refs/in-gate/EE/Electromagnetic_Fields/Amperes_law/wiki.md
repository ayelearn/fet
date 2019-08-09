The following text has been accessed from https://en.wikipedia.org/wiki/Amp%C3%A8re%27s_circuital_law at Thu Aug 8 22:56:01 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** AmpÃ¨re's circuital law ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"AmpÃ¨re's law" redirects here. For the law describing forces between current-
carrying wires, see AmpÃ¨re's_force_law.
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
    * AmpÃ¨re's law
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
In classical_electromagnetism, AmpÃ¨re's circuital law (not to be confused with
AmpÃ¨re's_force_law that AndrÃ©-Marie_AmpÃ¨re discovered in 1823)[1] relates
the integrated magnetic_field around a closed loop to the electric_current
passing through the loop. James_Clerk_Maxwell (not AmpÃ¨re) derived it using
hydrodynamics in his 1861 paper "On_Physical_Lines_of_Force"[2] and it is now
one of the Maxwell_equations, which form the basis of classical
electromagnetism.
⁰
***** Contents *****
    * 1_Maxwell's_original_circuital_law
          o 1.1_Equivalent_forms
          o 1.2_Explanation
          o 1.3_Ambiguities_and_sign_conventions
    * 2_Free_current_versus_bound_current
    * 3_Shortcomings_of_the_original_formulation_of_the_circuital_law
          o 3.1_Displacement_current
    * 4_Extending_the_original_law:_the_MaxwellâAmpÃ¨re_equation
          o 4.1_Proof_of_equivalence
    * 5_AmpÃ¨re's_circuital_law_in_cgs_units
    * 6_See_also
    * 7_Notes
    * 8_Further_reading
    * 9_External_links
***** Maxwell's original circuital law[edit] *****
The original form of Maxwell's circuital law, which he derived in his 1855
paper "On Faraday's Lines of Force"[3] based on an analogy to hydrodynamics,
relates magnetic_fields to electric_currents that produce them. It determines
the magnetic field associated with a given current, or the current associated
with a given magnetic field.
The original circuital law is only a correct law of physics in a magnetostatic
situation, where the system is static except possibly for continuous steady
currents within closed loops. For systems with electric fields that change over
time, the original law (as given in this section) must be modified to include a
term known as Maxwell's correction (see below).
**** Equivalent forms[edit] ****
The original circuital law can be written in several different forms, which are
all ultimately equivalent:
    * An "integral form" and a "differential form". The forms are exactly
      equivalent, and related by the KelvinâStokes_theorem.(see the "proof"
      section below)
    * Forms using SI_units, and those using cgs_units. Other units are
      possible, but rare. This section will use SI units, with cgs units
      discussed later.
    * Forms using either B_or_H_magnetic_fields. These two forms use the total
      current density and free current density, respectively. The B and H
      fields are related by the constitutive_equation: B = Î¼0H where Î¼0 is
      the magnetic_constant.
**** Explanation[edit] ****
The integral form of the original circuital law is a line_integral of the
magnetic_field around some closed_curve C (arbitrary but must be closed). The
curve C in turn bounds both a surface S which the electric_current passes
through (again arbitrary but not closedâsince no three-dimensional volume is
enclosed by S), and encloses the current. The mathematical statement of the law
is a relation between the total amount of magnetic field around some path (line
integral) due to the current which passes through that enclosed path (surface
integral).[4][5]
In terms of total current, (which is the sum of both free current and bound
current) the line integral of the magnetic_B-field (in teslas, T) around closed
curve C is proportional to the total current Ienc passing through a surface S
(enclosed by C). In terms of free current, the line integral of the magnetic_H-
field (in amperes per metre, AÂ·mâ1) around closed curve C equals the free
current If,enc through a surface S.
               Forms of the original circuital law written in SI units
                              Integral form            Differential form
                                     &#x222E;       C
                              &#x2061;  B  &#x22C5;  d
                              l  =  &#x03BC;  0
                              &#x222C;  S    J
                              &#x22C5;  d   S  =
                              &#x03BC;  0    I   e n c
                              {\displaystyle \oint _
                              {C}\mathbf {B} \cdot         &#x2207;  &#x00D7;
                              \mathrm {d} {\boldsymbol B  =  &#x03BC;  0    J
                              {l}}=\mu _{0}\iint _     {\displaystyle \mathbf
      Using B-field and total {S}\mathbf {J} \cdot     {\nabla } \times \mathbf
      current                 \mathrm {d} \mathbf {S}  {B} =\mu _{0}\mathbf {J}
                              =\mu _{0}I_{\mathrm      }  [\mathbf{\nabla}
                              {enc} }}  [              \times \mathbf{B} =
                              {\displaystyle \oint _   \mu_0 \mathbf{J} ]
                              {C}\mathbf {B} \cdot
                              \mathrm {d} {\boldsymbol
                              {l}}=\mu _{0}\iint _
                              {S}\mathbf {J} \cdot
                              \mathrm {d} \mathbf {S}
                              =\mu _{0}I_{\mathrm
                              {enc} }}]
                                     &#x222E;       C
                              &#x2061;  H  &#x22C5;  d
                              l  =  &#x222C;  S     J
                              f    &#x22C5;  d   S  =
                              I   f , e n c                &#x2207;  &#x00D7;
                              {\displaystyle \oint _   H  =   J    f
                              {C}\mathbf {H} \cdot     {\displaystyle \mathbf
                              \mathrm {d} {\boldsymbol {\nabla } \times \mathbf
      Using H-field and free  {l}}=\iint _{S}\mathbf   {H} =\mathbf {J} _
      current                 {J} _{\mathrm {f} }\cdot {\mathrm {f} }}  [
                              \mathrm {d} \mathbf {S}  {\displaystyle \mathbf
                              =I_{\mathrm {f,enc} }}   {\nabla } \times \mathbf
                              [{\displaystyle \oint _  {H} =\mathbf {J} _
                              {C}\mathbf {H} \cdot     {\mathrm {f} }}]
                              \mathrm {d} {\boldsymbol
                              {l}}=\iint _{S}\mathbf
                              {J} _{\mathrm {f} }\cdot
                              \mathrm {d} \mathbf {S}
                              =I_{\mathrm {f,enc} }}]
    * J is the total current_density (in amperes per square metre, AÂ·mâ2),
    * Jf is the free current density only,
    * â®C is the closed line_integral around the closed curve C,
    * â¬S denotes a 2-D surface_integral over S enclosed by C,
    * Â· is the vector dot_product,
    * dl is an infinitesimal element (a differential) of the curve C (i.e. a
      vector with magnitude equal to the length of the infinitesimal line
      element, and direction given by the tangent to the curve C)
    * dS is the vector_area of an infinitesimal element of surface S (that is,
      a vector with magnitude equal to the area of the infinitesimal surface
      element, and direction normal to surface S. The direction of the normal
      must correspond with the orientation of C by the right hand rule), see
      below for further explanation of the curve C and surface S.
    * â Ã is the curl operator.
**** Ambiguities and sign conventions[edit] ****
There are a number of ambiguities in the above definitions that require
clarification and a choice of convention.
   1. First, three of these terms are associated with sign ambiguities: the
      line integral â®C could go around the loop in either direction
      (clockwise or counterclockwise); the vector area dS could point in either
      of the two directions normal to the surface; and Ienc is the net current
      passing through the surface S, meaning the current passing through in one
      direction, minus the current in the other directionâbut either
      direction could be chosen as positive. These ambiguities are resolved by
      the right-hand_rule: With the palm of the right-hand toward the area of
      integration, and the index-finger pointing along the direction of line-
      integration, the outstretched thumb points in the direction that must be
      chosen for the vector area dS. Also the current passing in the same
      direction as dS must be counted as positive. The right_hand_grip_rule can
      also be used to determine the signs.
   2. Second, there are infinitely many possible surfaces S that have the curve
      C as their border. (Imagine a soap film on a wire loop, which can be
      deformed by moving the wire). Which of those surfaces is to be chosen? If
      the loop does not lie in a single plane, for example, there is no one
      obvious choice. The answer is that it does not matter; by Stoke's
      theorem, the integral is the same for any surface with boundary C, since
      the integrand is the curl of a smooth field (i.e. exact). In practice,
      one usually chooses the most convenient surface (with the given boundary)
      to integrate over.
***** Free current versus bound current[edit] *****
The electric current that arises in the simplest textbook situations would be
classified as "free current"âfor example, the current that passes through a
wire or battery. In contrast, "bound current" arises in the context of bulk
materials that can be magnetized and/or polarized. (All materials can to some
extent.)
When a material is magnetized (for example, by placing it in an external
magnetic field), the electrons remain bound to their respective atoms, but
behave as if they were orbiting the nucleus in a particular direction, creating
a microscopic current. When the currents from all these atoms are put together,
they create the same effect as a macroscopic current, circulating perpetually
around the magnetized object. This magnetization_current JM is one contribution
to "bound current".
The other source of bound current is bound_charge. When an electric field is
applied, the positive and negative bound charges can separate over atomic
distances in polarizable_materials, and when the bound charges move, the
polarization changes, creating another contribution to the "bound current", the
polarization current JP.
The total current density J due to free and bound charges is then:
          J  =   J    f    +   J    M    +   J    P     ,   {\displaystyle
      \mathbf {J} =\mathbf {J} _{\mathrm {f} }+\mathbf {J} _{\mathrm {M}
      }+\mathbf {J} _{\mathrm {P} }\,,}  [{\displaystyle \mathbf {J} =\mathbf
      {J} _{\mathrm {f} }+\mathbf {J} _{\mathrm {M} }+\mathbf {J} _{\mathrm {P}
      }\,,}]
with Jf  the "free" or "conduction" current density.
All current is fundamentally the same, microscopically. Nevertheless, there are
often practical reasons for wanting to treat bound current differently from
free current. For example, the bound current usually originates over atomic
dimensions, and one may wish to take advantage of a simpler theory intended for
larger dimensions. The result is that the more microscopic AmpÃ¨re's circuital
law, expressed in terms of B and the microscopic current (which includes free,
magnetization and polarization currents), is sometimes put into the equivalent
form below in terms of H and the free current only. For a detailed definition
of free current and bound current, and the proof that the two formulations are
equivalent, see the "proof" section below.
***** Shortcomings of the original formulation of the circuital law[edit] *****
There are two important issues regarding the circuital law that require closer
scrutiny. First, there is an issue regarding the continuity_equation for
electrical charge. In vector calculus, the identity for the divergence_of_a
curl states that the divergence of the curl of a vector field must always be
zero. Hence
         &#x2207; &#x22C5; ( &#x2207; &#x00D7;  B  ) = 0  ,   {\displaystyle
      \nabla \cdot (\nabla \times \mathbf {B} )=0\,,}  [{\displaystyle \nabla
      \cdot (\nabla \times \mathbf {B} )=0\,,}]
and so the original AmpÃ¨re's circuital law implies that
         &#x2207; &#x22C5;  J  = 0  .   {\displaystyle \nabla \cdot \mathbf {J}
      =0\,.}  [{\displaystyle \nabla \cdot \mathbf {J} =0\,.}]
But in general, reality follows the continuity_equation_for_electric_charge:
         &#x2207; &#x22C5;  J  = &#x2212;    &#x2202; &#x03C1;   &#x2202; t
      ,   {\displaystyle \nabla \cdot \mathbf {J} =-{\frac {\partial \rho }
      {\partial t}}\,,}  [{\displaystyle \nabla \cdot \mathbf {J} =-{\frac
      {\partial \rho }{\partial t}}\,,}]
which is nonzero for a time-varying charge density. An example occurs in a
capacitor circuit where time-varying charge densities exist on the plates.[6]
[7][8][9][10]
Second, there is an issue regarding the propagation of electromagnetic waves.
For example, in free_space, where
          J  =  0   .   {\displaystyle \mathbf {J} =\mathbf {0} \,.}  [
      {\displaystyle \mathbf {J} =\mathbf {0} \,.}]
The circuital law implies that
         &#x2207; &#x00D7;  B  =  0   ,   {\displaystyle \nabla \times \mathbf
      {B} =\mathbf {0} \,,}  [{\displaystyle \nabla \times \mathbf {B} =\mathbf
      {0} \,,}]
but to maintain consistency with the continuity_equation_for_electric_charge,
we must have
         &#x2207; &#x00D7;  B  =   1  c  2        &#x2202;  E    &#x2202; t
      .   {\displaystyle \nabla \times \mathbf {B} ={\frac {1}{c^{2}}}{\frac
      {\partial \mathbf {E} }{\partial t}}\,.}  [{\displaystyle \nabla \times
      \mathbf {B} ={\frac {1}{c^{2}}}{\frac {\partial \mathbf {E} }{\partial
      t}}\,.}]
To treat these situations, the contribution of displacement_current must be
added to the current term in the circuital law.
James_Clerk_Maxwell conceived of displacement current as a polarization current
in the dielectric vortex sea, which he used to model the magnetic field
hydrodynamically and mechanically.[11] He added this displacement_current to
AmpÃ¨re's circuital law at equation 112 in his 1861 paper "On_Physical_Lines_of
Force".[12]
**** Displacement current[edit] ****
Main article: Displacement_current
In free_space, the displacement current is related to the time rate of change
of electric field.
In a dielectric the above contribution to displacement current is present too,
but a major contribution to the displacement current is related to the
polarization of the individual molecules of the dielectric material. Even
though charges cannot flow freely in a dielectric, the charges in molecules can
move a little under the influence of an electric field. The positive and
negative charges in molecules separate under the applied field, causing an
increase in the state of polarization, expressed as the polarization_density P.
A changing state of polarization is equivalent to a current.
Both contributions to the displacement current are combined by defining the
displacement current as:[6]
           J    D    =   &#x2202;  &#x2202; t     D  (  r  ,  t )  ,
      {\displaystyle \mathbf {J} _{\mathrm {D} }={\frac {\partial }{\partial
      t}}\mathbf {D} (\mathbf {r} ,\,t)\,,}  [{\displaystyle \mathbf {J} _
      {\mathrm {D} }={\frac {\partial }{\partial t}}\mathbf {D} (\mathbf {r}
      ,\,t)\,,}]
where the electric_displacement_field is defined as:
          D  =  &#x03B5;  0    E  +  P  =  &#x03B5;  0    &#x03B5;   r     E
      ,   {\displaystyle \mathbf {D} =\varepsilon _{0}\mathbf {E} +\mathbf {P}
      =\varepsilon _{0}\varepsilon _{\mathrm {r} }\mathbf {E} \,,}  [
      {\displaystyle \mathbf {D} =\varepsilon _{0}\mathbf {E} +\mathbf {P}
      =\varepsilon _{0}\varepsilon _{\mathrm {r} }\mathbf {E} \,,}]
where Îµ0 is the electric_constant, Îµr the relative_static_permittivity, and P
is the polarization_density. Substituting this form for D in the expression for
displacement current, it has two components:
           J    D    =  &#x03B5;  0      &#x2202;  E    &#x2202; t    +
      &#x2202;  P    &#x2202; t     .   {\displaystyle \mathbf {J} _{\mathrm
      {D} }=\varepsilon _{0}{\frac {\partial \mathbf {E} }{\partial t}}+{\frac
      {\partial \mathbf {P} }{\partial t}}\,.}  [{\displaystyle \mathbf {J} _
      {\mathrm {D} }=\varepsilon _{0}{\frac {\partial \mathbf {E} }{\partial
      t}}+{\frac {\partial \mathbf {P} }{\partial t}}\,.}]
The first term on the right hand side is present everywhere, even in a vacuum.
It doesn't involve any actual movement of charge, but it nevertheless has an
associated magnetic field, as if it were an actual current. Some authors apply
the name displacement current to only this contribution.[13]
The second term on the right hand side is the displacement current as
originally conceived by Maxwell, associated with the polarization of the
individual molecules of the dielectric material.
Maxwell's original explanation for displacement current focused upon the
situation that occurs in dielectric media. In the modern post-aether era, the
concept has been extended to apply to situations with no material media
present, for example, to the vacuum between the plates of a charging vacuum
capacitor. The displacement current is justified today because it serves
several requirements of an electromagnetic theory: correct prediction of
magnetic fields in regions where no free current flows; prediction of wave
propagation of electromagnetic fields; and conservation of electric charge in
cases where charge density is time-varying. For greater discussion see
Displacement_current.
***** Extending the original law: the MaxwellâAmpÃ¨re equation[edit] *****
Next, the circuital equation is extended by including the polarization current,
thereby remedying the limited applicability of the original circuital law.
Treating free charges separately from bound charges, The equation including
Maxwell's correction in terms of the H-field is (the H-field is used because it
includes the magnetization currents, so JM does not appear explicitly, see H-
field and also Note):[14]
             &#x222E;       C   &#x2061;  H  &#x22C5;  d   l  =  &#x222C;  S
      (    J    f    +    &#x2202;  D    &#x2202; t     )  &#x22C5;  d   S
      {\displaystyle \oint _{C}\mathbf {H} \cdot \mathrm {d} {\boldsymbol
      {l}}=\iint _{S}\left(\mathbf {J} _{\mathrm {f} }+{\frac {\partial \mathbf
      {D} }{\partial t}}\right)\cdot \mathrm {d} \mathbf {S} }  [{\displaystyle
      \oint _{C}\mathbf {H} \cdot \mathrm {d} {\boldsymbol {l}}=\iint _{S}\left
      (\mathbf {J} _{\mathrm {f} }+{\frac {\partial \mathbf {D} }{\partial
      t}}\right)\cdot \mathrm {d} \mathbf {S} }]
(integral form), where H is the magnetic_H_field (also called "auxiliary
magnetic field", "magnetic field intensity", or just "magnetic field"), D is
the electric_displacement_field, and Jf is the enclosed conduction current or
free_current density. In differential form,
          &#x2207;  &#x00D7;  H  =   J    f    +    &#x2202;  D    &#x2202; t
      .   {\displaystyle \mathbf {\nabla } \times \mathbf {H} =\mathbf {J} _
      {\mathrm {f} }+{\frac {\partial \mathbf {D} }{\partial t}}\,.}  [
      {\displaystyle \mathbf {\nabla } \times \mathbf {H} =\mathbf {J} _
      {\mathrm {f} }+{\frac {\partial \mathbf {D} }{\partial t}}\,.}]
On the other hand, treating all charges on the same footing (disregarding
whether they are bound or free charges), the generalized AmpÃ¨re's equation,
also called the MaxwellâAmpÃ¨re equation, is in integral form (see the
"proof" section below):
       &#x222E;       C   &#x2061;  B  &#x22C5;  d   l  =  &#x222C;  S
(   &#x03BC;  0    J  +  &#x03BC;  0    &#x03B5;  0      &#x2202;  E
&#x2202; t     )  &#x22C5;  d   S    {\displaystyle \oint _{C}\mathbf {B} \cdot
\mathrm {d} {\boldsymbol {l}}=\iint _{S}\left(\mu _{0}\mathbf {J} +\mu _
{0}\varepsilon _{0}{\frac {\partial \mathbf {E} }{\partial t}}\right)\cdot
\mathrm {d} \mathbf {S} }  [{\displaystyle \oint _{C}\mathbf {B} \cdot \mathrm
{d} {\boldsymbol {l}}=\iint _{S}\left(\mu _{0}\mathbf {J} +\mu _{0}\varepsilon
_{0}{\frac {\partial \mathbf {E} }{\partial t}}\right)\cdot \mathrm {d} \mathbf
{S} }]
In differential form,
    &#x2207;  &#x00D7;  B  =  &#x03BC;  0    J  +  &#x03BC;  0    &#x03B5;  0
&#x2202;  E    &#x2202; t      {\displaystyle \mathbf {\nabla } \times \mathbf
{B} =\mu _{0}\mathbf {J} +\mu _{0}\varepsilon _{0}{\frac {\partial \mathbf {E}
}{\partial t}}}  [{\displaystyle \mathbf {\nabla } \times \mathbf {B} =\mu _
{0}\mathbf {J} +\mu _{0}\varepsilon _{0}{\frac {\partial \mathbf {E} }{\partial
t}}}]
In both forms J includes magnetization_current density[15] as well as
conduction and polarization current densities. That is, the current density on
the right side of the AmpÃ¨reâMaxwell equation is:
           J    f    +   J    D    +   J    M    =   J    f    +   J    P    +
      J    M    +  &#x03B5;  0      &#x2202;  E    &#x2202; t    =  J  +
      &#x03B5;  0      &#x2202;  E    &#x2202; t     ,   {\displaystyle \mathbf
      {J} _{\mathrm {f} }+\mathbf {J} _{\mathrm {D} }+\mathbf {J} _{\mathrm {M}
      }=\mathbf {J} _{\mathrm {f} }+\mathbf {J} _{\mathrm {P} }+\mathbf {J} _
      {\mathrm {M} }+\varepsilon _{0}{\frac {\partial \mathbf {E} }{\partial
      t}}=\mathbf {J} +\varepsilon _{0}{\frac {\partial \mathbf {E} }{\partial
      t}}\,,}  [{\displaystyle \mathbf {J} _{\mathrm {f} }+\mathbf {J} _
      {\mathrm {D} }+\mathbf {J} _{\mathrm {M} }=\mathbf {J} _{\mathrm {f}
      }+\mathbf {J} _{\mathrm {P} }+\mathbf {J} _{\mathrm {M} }+\varepsilon _
      {0}{\frac {\partial \mathbf {E} }{\partial t}}=\mathbf {J} +\varepsilon _
      {0}{\frac {\partial \mathbf {E} }{\partial t}}\,,}]
where current density JD is the displacement current, and J is the current
density contribution actually due to movement of charges, both free and bound.
Because ââââD = Ï, the charge continuity issue with AmpÃ¨re's original
formulation is no longer a problem.[16] Because of the term in Îµ0âE/ât,
wave propagation in free space now is possible.
With the addition of the displacement current, Maxwell was able to hypothesize
(correctly) that light was a form of electromagnetic_wave. See electromagnetic
wave_equation for a discussion of this important discovery.
**** Proof of equivalence[edit] ****
      Proof that the formulations of the circuital law in terms of free current
      are equivalent to the formulations involving total current.
      In this proof, we will show that the equation
               &#x2207; &#x00D7;  H  =   J    f    +    &#x2202;  D    &#x2202;
            t      {\displaystyle \nabla \times \mathbf {H} =\mathbf {J} _
            {\mathrm {f} }+{\frac {\partial \mathbf {D} }{\partial t}}}  [
            {\displaystyle \nabla \times \mathbf {H} =\mathbf {J} _{\mathrm {f}
            }+{\frac {\partial \mathbf {D} }{\partial t}}}]
      is equivalent to the equation
                 1  &#x03BC;  0     (  &#x2207;  &#x00D7;  B  ) =  J  +
            &#x03B5;  0      &#x2202;  E    &#x2202; t     .   {\displaystyle
            {\frac {1}{\mu _{0}}}(\mathbf {\nabla } \times \mathbf {B}
            )=\mathbf {J} +\varepsilon _{0}{\frac {\partial \mathbf {E} }
            {\partial t}}\,.}  [{\displaystyle {\frac {1}{\mu _{0}}}(\mathbf
            {\nabla } \times \mathbf {B} )=\mathbf {J} +\varepsilon _{0}{\frac
            {\partial \mathbf {E} }{\partial t}}\,.}]
      Note that we are only dealing with the differential forms, not the
      integral forms, but that is sufficient since the differential and
      integral forms are equivalent in each case, by the KelvinâStokes
      theorem.
      We introduce the polarization_density P, which has the following relation
      to E and D:
                D  =  &#x03B5;  0    E  +  P   .   {\displaystyle \mathbf {D}
            =\varepsilon _{0}\mathbf {E} +\mathbf {P} \,.}  [{\displaystyle
            \mathbf {D} =\varepsilon _{0}\mathbf {E} +\mathbf {P} \,.}]
      Next, we introduce the magnetization_density M, which has the following
      relation to B and H:
                 1  &#x03BC;  0      B  =  H  +  M    {\displaystyle {\frac {1}
            {\mu _{0}}}\mathbf {B} =\mathbf {H} +\mathbf {M} }  [{\displaystyle
            {\frac {1}{\mu _{0}}}\mathbf {B} =\mathbf {H} +\mathbf {M} }]
      and the following relation to the bound current:
                     J    b o u n d       = &#x2207; &#x00D7;  M  +    &#x2202;
            P    &#x2202; t          =   J    M    +   J    P     ,
            {\displaystyle {\begin{aligned}\mathbf {J} _{\mathrm {bound}
            }&=\nabla \times \mathbf {M} +{\frac {\partial \mathbf {P} }
            {\partial t}}\\&=\mathbf {J} _{\mathrm {M} }+\mathbf {J} _{\mathrm
            {P} }\,,\end{aligned}}}  [{\displaystyle {\begin{aligned}\mathbf
            {J} _{\mathrm {bound} }&=\nabla \times \mathbf {M} +{\frac
            {\partial \mathbf {P} }{\partial t}}\\&=\mathbf {J} _{\mathrm {M}
            }+\mathbf {J} _{\mathrm {P} }\,,\end{aligned}}}]
      where
                 J    M    = &#x2207; &#x00D7;  M   ,   {\displaystyle \mathbf
            {J} _{\mathrm {M} }=\nabla \times \mathbf {M} \,,}  [{\displaystyle
            \mathbf {J} _{\mathrm {M} }=\nabla \times \mathbf {M} \,,}]
      is called the magnetization_current density, and
                 J    P    =    &#x2202;  P    &#x2202; t     ,
            {\displaystyle \mathbf {J} _{\mathrm {P} }={\frac {\partial \mathbf
            {P} }{\partial t}}\,,}  [{\displaystyle \mathbf {J} _{\mathrm {P}
            }={\frac {\partial \mathbf {P} }{\partial t}}\,,}]
      is the polarization current density. Taking the equation for B:
                     1  &#x03BC;  0     (  &#x2207;  &#x00D7;  B  )    =
            &#x2207;  &#x00D7;  (   H  +  M   )        =  &#x2207;  &#x00D7;  H
            +   J    M          =   J    f    +   J    P    +  &#x03B5;  0
            &#x2202;  E    &#x2202; t    +   J    M     .       {\displaystyle
            {\begin{aligned}{\frac {1}{\mu _{0}}}(\mathbf {\nabla } \times
            \mathbf {B} )&=\mathbf {\nabla } \times \left(\mathbf {H} +\mathbf
            {M} \right)\\&=\mathbf {\nabla } \times \mathbf {H} +\mathbf {J} _
            {\mathrm {M} }\\&=\mathbf {J} _{\mathrm {f} }+\mathbf {J} _{\mathrm
            {P} }+\varepsilon _{0}{\frac {\partial \mathbf {E} }{\partial
            t}}+\mathbf {J} _{\mathrm {M} }\,.\end{aligned}}}  [{\displaystyle
            {\begin{aligned}{\frac {1}{\mu _{0}}}(\mathbf {\nabla } \times
            \mathbf {B} )&=\mathbf {\nabla } \times \left(\mathbf {H} +\mathbf
            {M} \right)\\&=\mathbf {\nabla } \times \mathbf {H} +\mathbf {J} _
            {\mathrm {M} }\\&=\mathbf {J} _{\mathrm {f} }+\mathbf {J} _{\mathrm
            {P} }+\varepsilon _{0}{\frac {\partial \mathbf {E} }{\partial
            t}}+\mathbf {J} _{\mathrm {M} }\,.\end{aligned}}}]
      Consequently, referring to the definition of the bound current:
                     1  &#x03BC;  0     (  &#x2207;  &#x00D7;  B  )    =   J
            f    +   J    b o u n d    +  &#x03B5;  0      &#x2202;  E
            &#x2202; t          =  J  +  &#x03B5;  0      &#x2202;  E
            &#x2202; t     ,       {\displaystyle {\begin{aligned}{\frac {1}
            {\mu _{0}}}(\mathbf {\nabla } \times \mathbf {B} )&=\mathbf {J} _
            {\mathrm {f} }+\mathbf {J} _{\mathrm {bound} }+\varepsilon _{0}
            {\frac {\partial \mathbf {E} }{\partial t}}\\&=\mathbf {J}
            +\varepsilon _{0}{\frac {\partial \mathbf {E} }{\partial t}}\,,\end
            {aligned}}}  [{\displaystyle {\begin{aligned}{\frac {1}{\mu _{0}}}
            (\mathbf {\nabla } \times \mathbf {B} )&=\mathbf {J} _{\mathrm {f}
            }+\mathbf {J} _{\mathrm {bound} }+\varepsilon _{0}{\frac {\partial
            \mathbf {E} }{\partial t}}\\&=\mathbf {J} +\varepsilon _{0}{\frac
            {\partial \mathbf {E} }{\partial t}}\,,\end{aligned}}}]
      as was to be shown.
***** AmpÃ¨re's circuital law in cgs units[edit] *****
In cgs units, the integral form of the equation, including Maxwell's
correction, reads
             &#x222E;       C   &#x2061;  B  &#x22C5;  d   l  =   1 c
      &#x222C;  S    (  4 &#x03C0;  J  +    &#x2202;  E    &#x2202; t     )
      &#x22C5;  d   S   ,   {\displaystyle \oint _{C}\mathbf {B} \cdot \mathrm
      {d} {\boldsymbol {l}}={\frac {1}{c}}\iint _{S}\left(4\pi \mathbf {J} +
      {\frac {\partial \mathbf {E} }{\partial t}}\right)\cdot \mathrm {d}
      \mathbf {S} \,,}  [{\displaystyle \oint _{C}\mathbf {B} \cdot \mathrm {d}
      {\boldsymbol {l}}={\frac {1}{c}}\iint _{S}\left(4\pi \mathbf {J} +{\frac
      {\partial \mathbf {E} }{\partial t}}\right)\cdot \mathrm {d} \mathbf {S}
      \,,}]
where c is the speed_of_light.
The differential form of the equation (again, including Maxwell's correction)
is
          &#x2207;  &#x00D7;  B  =   1 c    (  4 &#x03C0;  J  +    &#x2202;  E
      &#x2202; t     )   .   {\displaystyle \mathbf {\nabla } \times \mathbf
      {B} ={\frac {1}{c}}\left(4\pi \mathbf {J} +{\frac {\partial \mathbf {E} }
      {\partial t}}\right)\,.}  [{\displaystyle \mathbf {\nabla } \times
      \mathbf {B} ={\frac {1}{c}}\left(4\pi \mathbf {J} +{\frac {\partial
      \mathbf {E} }{\partial t}}\right)\,.}]
***** See also[edit] *****
    * BiotâSavart_law              [icon]     * Book:_Maxwell's_equations
    * Displacement_current                  * Faraday's_law_of_induction
    * Capacitance                           * Bound_charge
    * AmpÃ¨rian_magnetic_dipole_model     * Electric_current
    * Electromagnetic_wave_equation         * Vector_calculus
    * Maxwell's_equations                   * Stokes'_theorem
***** Notes[edit] *****
   1. ^ AmpÃ¨re never utilized the field concept in any of his works; cf.Assis,
      AndrÃ© Koch Torres; Chaib, J. P. M. C; AmpÃ¨re, AndrÃ©-Marie (2015).
      AmpÃ¨re's_electrodynamics:_analysis_of_the_meaning_and_evolution_of
      AmpÃ¨re's_force_between_current_elements,_together_with_a_complete
      translation_of_his_masterpiece:_Theory_of_electrodynamic_phenomena,
      uniquely_deduced_from_experience (PDF). Montreal, QC: Apeiron. ch. 15 p.
      221. ISBN 978-1-987980-03-5.
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
   3. The "AmpÃ¨re circuital law" is thus more properly termed the
      "AmpÃ¨reâMaxwell law." It is named after AmpÃ¨re because of his
      contributions to understanding electric current. Maxwell does not take
      AmpÃ¨re's_force_law as a starting point in deriving any of his equations,
      although he mentions AmpÃ¨re's_force_law in his A_Treatise_on_Electricity
      and_Magnetism vol. 2, part 4, ch. 2 (Â§Â§502-527) & 23 (Â§Â§845-866).
   4. ^Clerk Maxwell, James. "On_Physical_Lines_of_Force".
   5. ^Clerk Maxwell, James. "On_Faraday's_Lines_of_Force".
   6. ^Knoepfel, Heinz E. (2000). Magnetic_Fields:_A_comprehensive_theoretical
      treatise_for_practical_use. Wiley. p. 4. ISBN 0-471-32205-9.
   7. ^Owen, George E. (2003). Electromagnetic_Theory (Reprint of 1963 ed.).
      Courier-Dover Publications. p. 213. ISBN 0-486-42830-3.
   8. ^ a bJackson, John David (1999). Classical Electrodynamics (3rd ed.).
      Wiley. p. 238. ISBN 0-471-30932-X.
   9. ^Griffiths, David J. (1999). Introduction_to_Electrodynamics (3rd ed.).
      Pearson/Addison-Wesley. pp. 322â323. ISBN 0-13-805326-X.
  10. ^Owen, George E. (2003). Electromagnetic_Theory. Mineola, NY: Dover
      Publications. p. 285. ISBN 0-486-42830-3.
  11. ^Billingham, J.; King, A. C. (2006). Wave_Motion. Cambridge University
      Press. p. 179. ISBN 0-521-63450-4.
  12. ^Slater, J. C.; Frank, N. H. (1969). Electromagnetism (Reprint of 1947
      ed.). Courier Dover Publications. p. 83. ISBN 0-486-62263-0.
  13. ^Siegel, Daniel M. (2003). Innovation_in_Maxwell's_Electromagnetic
      Theory:_Molecular_Vortices,_Displacement_Current,_and_Light. Cambridge
      University Press. pp. 96â98. ISBN 0-521-53329-5.
  14. ^Clerk Maxwell, James (1861). "On_Physical_Lines_of_Force" (PDF).
      Philosophical Magazine and Journal of Science.
  15. ^ For example, seeGriffiths,_David_J. (1999). Introduction to
      Electrodynamics. Upper Saddle River, NJ: Prentice Hall. p. 323. ISBN 0-
      13-805326-X.
  16.  andTai L. Chow (2006). Introduction_to_Electromagnetic_Theory. Jones &
      Bartlett. p. 204. ISBN 0-7637-3827-1.
  17. ^Rogalski, Mircea S.; Palmer, Stuart B. (2006). Advanced_University
      Physics. CRC Press. p. 267. ISBN 1-58488-511-4.
  18. ^Rogalski, Mircea S.; Palmer, Stuart B. (2006). Advanced_University
      Physics. CRC Press. p. 251. ISBN 1-58488-511-4.
  19. ^ The magnetization current can be expressed as the curl of the
      magnetization, so its divergence is zero and it does not contribute to
      the continuity equation. See magnetization_current.
***** Further reading[edit] *****
    * Griffiths, David J. (1998). Introduction to Electrodynamics (3rd ed.).
      Prentice Hall. ISBN 0-13-805326-X.
Tipler, Paul (2004). Physics for Scientists and Engineers: Electricity,
Magnetism, Light, and Elementary Modern Physics (5th ed.). W. H. Freeman.
ISBN 0-7167-0810-8.
***** External links[edit] *****
    * MISN-0-138_Ampere's_Law (PDF_file) by Kirby Morgan for Project_PHYSNET.
    * MISN-0-145_The_AmpereâMaxwell_Equation;_Displacement_Current (PDF file)
      by J.S. Kovacs for Project PHYSNET.
    * A_Dynamical_Theory_of_the_Electromagnetic_Field Maxwell's paper of 1864

Retrieved from "https://en.wikipedia.org/w/
index.php?title=AmpÃ¨re%27s_circuital_law&oldid=908639836"
Categories:
    * Electrostatics
    * Magnetostatics
    * Maxwell's_equations
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
    * Asturianu
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * à¤¨à¥à¤ªà¤¾à¤²à¥
    * æ¥æ¬èª
    * Norsk
    * áá¶áá¶ááááá
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * Simple_English
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ä¸­æ
Edit_links
    * This page was last edited on 31 July 2019, at 00:58 (UTC).
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
