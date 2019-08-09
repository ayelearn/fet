The following text has been accessed from https://en.wikipedia.org/wiki/Chemical_potential at Fri Aug 9 02:03:41 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Chemical potential ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Conjugate_variables
of_thermodynamics
Pressure           Volume
(Stress)           (Strain)
Temperature        Entropy
Chemical potential Particle_number
In thermodynamics, chemical potential of a species is energy that can be
absorbed or released due to a change of the particle_number of the given
species, e.g. in a chemical reaction or phase_transition. The chemical
potential of a species in a mixture is defined as the rate of change of free
energy of a thermodynamic_system with respect to the change in the number of
atoms or molecules of the species that are added to the system. Thus, it is the
partial_derivative of the free energy with respect to the amount of the
species, all other species' concentrations in the mixture remaining constant.
The molar chemical potential is also known as partial molar free energy[1].
When both temperature and pressure are held constant, chemical potential is the
partial molar Gibbs_free_energy. At chemical_equilibrium or in phase
equilibrium the total sum of the product of chemical potentials and
stoichiometric_coefficients is zero, as the free energy is at a minimum.[2][3]
[4]
In semiconductor physics, the chemical potential of a system of electrons at a
temperature of zero Kelvin is known as the Fermi_energy.[5]
⁰
***** Contents *****
    * 1_Overview
    * 2_Thermodynamic_definition
    * 3_Applications
    * 4_History
    * 5_Electrochemical,_internal,_external,_and_total_chemical_potential
    * 6_Systems_of_particles
          o 6.1_Electrons_in_solids
          o 6.2_Sub-nuclear_particles
          o 6.3_Ideal_vs._non-ideal_solutions
    * 7_See_also
    * 8_References
    * 9_External_links
***** Overview[edit] *****
Particles tend to move from higher chemical potential to lower chemical
potential. In this way, chemical potential is a generalization of "potentials"
in_physics such as gravitational_potential. When a ball rolls down a hill, it
is moving from a higher gravitational potential (higher internal energy thus
higher potential for work) to a lower gravitational potential (lower internal
energy). In the same way, as molecules move, react, dissolve, melt, etc., they
will always tend naturally to go from a higher chemical potential to a lower
one, changing the particle_number, which is conjugate_variable to chemical
potential.
A simple example is a system of dilute molecules diffusing in a homogeneous
environment. In this system, the molecules tend to move from areas with high
concentration to low concentration, until eventually the concentration is the
same everywhere.
The microscopic explanation for this is based in kinetic_theory and the random
motion of molecules. However, it is simpler to describe the process in terms of
chemical potentials: For a given temperature, a molecule has a higher chemical
potential in a higher-concentration area, and a lower chemical potential in a
low concentration area. Movement of molecules from higher chemical potential to
lower chemical potential is accompanied by a release of free energy. Therefore,
it is a spontaneous_process.
Another example, not based on concentration but on phase, is a glass of liquid
water with ice cubes in it. Above 0 Â°C, an H2O molecule that is in the liquid
phase (liquid water) has a lower chemical potential than a water molecule that
is in the solid phase (ice). When some of the ice melts, H2O molecules convert
from solid to liquid where their chemical potential is lower, so the ice cubes
shrink. Below 0 Â°C, the molecules in the ice phase have the lower chemical
potential, so the ice cubes grow. At the temperature of the melting_point,
0 Â°C, the chemical potentials in water and ice are the same; the ice cubes
neither grow nor shrink, and the system is in equilibrium.
A third example is illustrated by the chemical reaction of dissociation of a
weak_acid HA (such as acetic_acid, A = CH3COOâ):
      HA â H+ + Aâ
Vinegar contains acetic acid. When acid molecules dissociate, the concentration
of the undissociated acid molecules (HA) decreases and the concentrations of
the product ions (H+ and Aâ) increase. Thus the chemical potential of HA
decreases and the sum of the chemical potentials of H+ and Aâ increases. When
the sums of chemical potential of reactants and products are equal the system
is at equilibrium and there is no tendency for the reaction to proceed in
either the forward or backward direction. This explains why vinegar is acidic,
because acetic acid dissociates to some extent, releasing hydrogen_ions into
the solution.
Chemical potentials are important in many aspects of equilibrium_chemistry,
including melting, boiling, evaporation, solubility, osmosis, partition
coefficient, liquid-liquid_extraction and chromatography. In each case there is
a characteristic constant which is a function of the chemical potentials of the
species at equilibrium.
In electrochemistry, ions do not always tend to go from higher to lower
chemical potential, but they do always go from higher to lower electrochemical
potential. The electrochemical potential completely characterizes all of the
influences on an ion's motion, while the chemical potential includes everything
except the electric_force. (See below for more on this terminology.)
***** Thermodynamic definition[edit] *****
The chemical potential Î¼i of species i (atomic, molecular or nuclear) is
defined, as all intensive quantities are, by the phenomenological fundamental
equation_of_thermodynamics expressed in the form, which holds for both
reversible and irreversible processes[6]
          d  U = T   d  S &#x2212; P   d  V    {\displaystyle \mathrm {d}
      U=T\,\mathrm {d} S-P\,\mathrm {d} V\,}  [\mathrm{d}U= T\,\mathrm{d}S -
      P\,\mathrm{d}V\,]    +  &#x2211;  i = 1   n    &#x03BC;  i    d   N  i
      {\displaystyle +\sum _{i=1}^{n}\mu _{i}\mathrm {d} N_{i}\,}  [
      {\displaystyle +\sum _{i=1}^{n}\mu _{i}\mathrm {d} N_{i}\,}] ,
where dU is the infinitesimal change of internal_energy U, dS the infinitesimal
change of entropy S, and dV is the infinitesimal change of volume V for a
thermodynamic_system in thermal equilibrium, and dNi is the infinitesimal
change of particle number Ni of species i as particles are added or subtracted.
T is absolute_temperature, S is entropy, P is pressure, and V is volume. Other
work terms, such as those involving electric, magnetic or gravitational fields
may be added.
From the above equation the chemical potential is given by
          &#x03BC;  i   =   (    &#x2202; U   &#x2202;  N  i      )   S , V ,
      N  j &#x2260; i       {\displaystyle \mu _{i}=\left({\frac {\partial U}
      {\partial N_{i}}}\right)_{S,V,N_{j\neq i}}}  [{\displaystyle \mu _
      {i}=\left({\frac {\partial U}{\partial N_{i}}}\right)_{S,V,N_{j\neq i}}}]
      .
This is an inconvenient expression for condensed matter systems, such as
chemical solutions, as it is hard to control the volume and entropy to be
constant while particles are added. A more convenient expression may be
obtained by making a Legendre_transformation to another thermodynamic
potential: the Gibbs_free_energy     G = U + P V &#x2212; T S   {\displaystyle
G=U+PV-TS}  [{\displaystyle G=U+PV-TS}]. The differential of this is      d  G
=  d  U + P  d  V + V  d  P &#x2212; T  d  S &#x2212; S  d  T   {\displaystyle
\mathrm {d} G=\mathrm {d} U+P\mathrm {d} V+V\mathrm {d} P-T\mathrm {d} S-
S\mathrm {d} T}  [{\displaystyle \mathrm {d} G=\mathrm {d} U+P\mathrm {d}
V+V\mathrm {d} P-T\mathrm {d} S-S\mathrm {d} T}] and using the above expression
for      d  U   {\displaystyle \mathrm {d} U}  [\mathrm {d} U] a differential
relation for      d  G   {\displaystyle \mathrm {d} G}  [{\displaystyle \mathrm
{d} G}] is obtained
          d  G = &#x2212; S   d  T + V   d  P    {\displaystyle \mathrm {d} G=-
      S\,\mathrm {d} T+V\,\mathrm {d} P\,}  [{\displaystyle \mathrm {d} G=-
      S\,\mathrm {d} T+V\,\mathrm {d} P\,}]     +  &#x2211;  i = 1   n
      &#x03BC;  i    d   N  i      {\displaystyle +\sum _{i=1}^{n}\mu _
      {i}\mathrm {d} N_{i}\,}  [{\displaystyle +\sum _{i=1}^{n}\mu _{i}\mathrm
      {d} N_{i}\,}] .
As a consequence, another expression for      &#x03BC;  i     {\displaystyle
\mu _{i}}  [{\displaystyle \mu _{i}}] results
          &#x03BC;  i   =   (    &#x2202; G   &#x2202;  N  i      )   T , P ,
      N  j &#x2260; i       {\displaystyle \mu _{i}=\left({\frac {\partial G}
      {\partial N_{i}}}\right)_{T,P,N_{j\neq i}}}  [{\displaystyle \mu _
      {i}=\left({\frac {\partial G}{\partial N_{i}}}\right)_{T,P,N_{j\neq i}}}]
and the change in Gibbs free energy of a system that is held at constant
temperature and pressure is simply
          d  G =  &#x2211;  i = 1   n    &#x03BC;  i    d   N  i
      {\displaystyle \mathrm {d} G=\sum _{i=1}^{n}\mu _{i}\mathrm {d} N_{i}\,}
      [{\displaystyle \mathrm {d} G=\sum _{i=1}^{n}\mu _{i}\mathrm {d} N_
      {i}\,}] .
In thermodynamic equilibrium, when the system concerned is at constant
temperature and pressure but can exchange particles with its external
environment, the Gibbs free energy is at its minimum for the system, that is
d  G = 0   {\displaystyle \mathrm {d} G=0}  [{\displaystyle \mathrm {d} G=0}].
It follows that
          &#x03BC;  1   d  N  1   +  &#x03BC;  2   d  N  2   + . . . = 0
      {\displaystyle \mu _{1}dN_{1}+\mu _{2}dN_{2}+...=0\,}  [{\displaystyle
      \mu _{1}dN_{1}+\mu _{2}dN_{2}+...=0\,}] .
Use of this equality provides the means to establish the equilibrium_constant
for a chemical reaction.
By making further Legendre transformations from U to other thermodynamic
potentials like the Enthalpy     H = U + P V   {\displaystyle H=U+PV}  [H = U +
PV] and Helmholtz_free_energy     F = U &#x2212; T S   {\displaystyle F=U-TS}
[{\displaystyle F=U-TS}], expressions for the chemical potential may be
obtained in terms of these:
          &#x03BC;  i   =   (    &#x2202; H   &#x2202;  N  i      )   S , P ,
      N  j &#x2260; i      &#xA0;and&#xA0;  &#xA0;  &#x03BC;  i   =
      (    &#x2202; F   &#x2202;  N  i      )   T , V ,  N  j &#x2260; i
      {\displaystyle \mu _{i}=\left({\frac {\partial H}{\partial N_
      {i}}}\right)_{S,P,N_{j\neq i}}{\text{ and }}\ \mu _{i}=\left({\frac
      {\partial F}{\partial N_{i}}}\right)_{T,V,N_{j\neq i}}}  [{\displaystyle
      \mu _{i}=\left({\frac {\partial H}{\partial N_{i}}}\right)_{S,P,N_{j\neq
      i}}{\text{  and  }}\ \mu _{i}=\left({\frac {\partial F}{\partial N_
      {i}}}\right)_{T,V,N_{j\neq i}}}] .
These different forms for the chemical potential are all equivalent, meaning
that they have the same physical content, and may be useful in different
physical situations.
***** Applications[edit] *****
The GibbsâDuhem_equation is useful because it relates individual chemical
potentials. For example, in a binary mixture, at constant temperature and
pressure, the chemical potentials of the two participants are related by
         d  &#x03BC;   B    = &#x2212;    n   A     n   B      d  &#x03BC;   A
      {\displaystyle d\mu _{\mathrm {B} }=-{\frac {n_{\mathrm {A} }}{n_{\mathrm
      {B} }}}d\mu _{\mathrm {A} }}  [{\displaystyle d\mu _{\mathrm {B} }=-
      {\frac {n_{\mathrm {A} }}{n_{\mathrm {B} }}}d\mu _{\mathrm {A} }}]
Every instance of phase or chemical equilibrium is characterized by a constant.
For instance, the melting of ice is characterized by a temperature, known as
the melting_point at which solid and liquid phases are in equilibrium with each
other. Chemical potentials can be used to explain the slopes of lines on a
phase_diagram by using the Clapeyron_equation, which in turn can be derived
from the GibbsâDuhem equation.[7] They are used to explain colligative
properties such as melting-point_depression by the application of pressure.[8]
Both Raoult's_law and Henry's_law can be derived in a simple manner using
chemical potentials.[9]
***** History[edit] *****
Chemical potential was first described by the American engineer, chemist and
mathematical physicist Josiah_Willard_Gibbs. He defined it as follows:
     If to any homogeneous mass in a state of hydrostatic_stress we
     suppose an infinitesimal quantity of any substance to be added, the
     mass remaining homogeneous and its entropy and volume remaining
     unchanged, the increase of the energy of the mass divided by the
     quantity of the substance added is the potential for that substance
     in the mass considered.
Gibbs later noted[citation_needed] also that for the purposes of this
definition, any chemical_element or combination of elements in given
proportions may be considered a substance, whether capable or not of existing
by itself as a homogeneous body. This freedom to choose the boundary of the
system allows chemical potential to be applied to a huge range of systems. The
term can be used in thermodynamics and physics for any system undergoing
change. Chemical potential is also referred to as partial molar Gibbs energy
(see also partial_molar_property). Chemical potential is measured in units of
energy/particle or, equivalently, energy/mole.
In his 1873 paper A Method of Geometrical Representation of the Thermodynamic
Properties of Substances by Means of Surfaces, Gibbs introduced the preliminary
outline of the principles of his new equation able to predict or estimate the
tendencies of various natural processes to ensue when bodies or systems are
brought into contact. By studying the interactions of homogeneous substances in
contact, i.e. bodies, being in composition part solid, part liquid, and part
vapor, and by using a three-dimensional volumeâentropyâinternal_energy
graph, Gibbs was able to determine three states of equilibrium, i.e.
"necessarily stable", "neutral", and "unstable", and whether or not changes
will ensue. In 1876, Gibbs built on this framework by introducing the concept
of chemical potential so to take into account chemical reactions and states of
bodies that are chemically different from each other. In his own words, to
summarize his results in 1873, Gibbs states:[citation_needed]
     If we wish to express in a single equation the necessary and
     sufficient condition of thermodynamic equilibrium for a substance
     when surrounded by a medium of constant pressure P and temperature T,
     this equation may be written:
               &#x03B4; ( &#x03F5; &#x2212; T &#x03B7; + P &#x03BD; ) = 0
           {\displaystyle \displaystyle \delta (\epsilon -T\eta +P\nu )=0}
           [\displaystyle \delta (\epsilon -T\eta +P\nu )=0]
     where Î´ refers to the variation produced by any variations in the
     state of the parts of the body, and (when different parts of the body
     are in different states) in the proportion in which the body is
     divided between the different states. The condition of stable
     equilibrium is that the value of the expression in the parenthesis
     shall be a minimum.
In this description, as used by Gibbs, Îµ refers to the internal_energy of the
body, Î· refers to the entropy of the body, and Î½ is the volume of the body.
***** Electrochemical, internal, external, and total chemical potential[edit]
*****
The abstract definition of chemical potential given aboveâtotal change in
free energy per extra mole of substanceâis more specifically called total
chemical potential.[10][11] If two locations have different total chemical
potentials for a species, some of it may be due to potentials associated with
"external" force fields (Electric_potential_energy differences, gravitational
potential_energy differences, etc.), while the rest would be due to "internal"
factors (density, temperature, etc.)[10] Therefore, the total chemical
potential can be split into internal chemical potential and external chemical
potential:
          &#x03BC;   t o t    =  &#x03BC;   i n t    +  &#x03BC;   e x t
      {\displaystyle \mu _{\mathrm {tot} }=\mu _{\mathrm {int} }+\mu _{\mathrm
      {ext} }\,}  [\mu _{\mathrm {tot} }=\mu _{\mathrm {int} }+\mu _{\mathrm
      {ext} }\,]
where
          &#x03BC;   e x t    = q V + m g h + &#x22EF;   {\displaystyle \mu _
      {\mathrm {ext} }=qV+mgh+\cdots }  [\mu _{\mathrm {ext} }=qV+mgh+\cdots ]
i.e., the external potential is the sum of electric potential, gravitational
potential, etc. (q and m are the charge and mass of the species, respectively,
V and h are the voltage and height of the container, respectively, and g is the
acceleration_due_to_gravity.) The internal chemical potential includes
everything else besides the external potentials, such as density, temperature,
and enthalpy. This formalism can be understood by assuming that the total
energy of a system,     U   {\displaystyle U}  [U], is the sum of two parts: an
internal energy,      U   i n t      {\displaystyle U_{\mathrm {int} }}  [
{\displaystyle U_{\mathrm {int} }}], and an external energy due to the
interaction of each particle with an external field,      U   e x t    = N ( q
V + m g h + &#x22EF; )   {\displaystyle U_{\mathrm {ext} }=N(qV+mgh+\cdots )}
[{\displaystyle U_{\mathrm {ext} }=N(qV+mgh+\cdots )}]. The definition of
chemical potential applied to      U   i n t    +  U   e x t
{\displaystyle U_{\mathrm {int} }+U_{\mathrm {ext} }}  [{\displaystyle U_
{\mathrm {int} }+U_{\mathrm {ext} }}] yields the above expression for
&#x03BC;   t o t      {\displaystyle \mu _{\mathrm {tot} }}  [{\displaystyle
\mu _{\mathrm {tot} }}].
The phrase "chemical potential" sometimes means "total chemical potential", but
that is not universal.[10] In some fields, in particular electrochemistry,
semiconductor_physics, and solid-state_physics, the term "chemical potential"
means internal chemical potential, while the term electrochemical_potential is
used to mean total chemical potential.[12][13][14][15][16]
***** Systems of particles[edit] *****
**** Electrons in solids[edit] ****
Main article: Fermi_level
Electrons in solids have a chemical potential, defined the same way as the
chemical potential of a chemical species: The change in free energy when
electrons are added or removed from the system. In the case of electrons, the
chemical potential is usually expressed in energy per particle rather than
energy per mole, and the energy per particle is conventionally given in units
of electronvolt (eV).
Chemical potential plays an especially important role in solid-state_physics
and is closely related to the concepts of work_function, Fermi_energy, and
Fermi_level. For example, n-type silicon has a higher internal chemical
potential of electrons than p-type silicon. In a pân_junction diode at
equilibrium the chemical potential (internal chemical potential) varies from
the p-type to the n-type side, while the total_chemical_potential
(electrochemical potential, or, Fermi_level) is constant throughout the diode.
As described above, when describing chemical potential, one has to say
"relative to what". In the case of electrons in semiconductors, internal
chemical potential is often specified relative to some convenient point in the
band structure, e.g., to the bottom of the conduction band. It may also be
specified "relative to vacuum", to yield a quantity known as work_function,
however work function varies from surface to surface even on a completely
homogeneous material. Total chemical potential on the other hand is usually
specified relative to electrical_ground.
In atomic physics, the chemical potential of the electrons in an atom is
sometimes[17] said to be the negative of the atom's electronegativity.
Likewise, the process of chemical potential equalization is sometimes referred
to as the process of electronegativity_equalization. This connection comes from
the Mulliken_electronegativity scale. By inserting the energetic definitions of
the ionization_potential and electron_affinity into the Mulliken
electronegativity, it is seen that the Mulliken chemical potential is a finite
difference approximation of the electronic energy with respect to the number of
electrons., i.e.,
          &#x03BC;   M u l l i k e n    = &#x2212;  &#x03C7;   M u l l i k e n
      = &#x2212;    I P + E A  2   =   [    &#x03B4; E [ N ]   &#x03B4; N    ]
      N =  N  0       {\displaystyle \mu _{\mathrm {Mulliken} }=-\chi _{\mathrm
      {Mulliken} }=-{\frac {IP+EA}{2}}=\left[{\frac {\delta E[N]}{\delta
      N}}\right]_{N=N_{0}}}  [\mu _{\mathrm {Mulliken} }=-\chi _{\mathrm
      {Mulliken} }=-{\frac {IP+EA}{2}}=\left[{\frac {\delta E[N]}{\delta
      N}}\right]_{N=N_{0}}]
**** Sub-nuclear particles[edit] ****
In recent years, thermal_physics has applied the definition of chemical
potential to systems in particle_physics and its associated processes. For
example, in a quarkâgluon_plasma or other QCD_matter, at every point in space
there is a chemical potential for photons, a chemical potential for electrons,
a chemical potential for baryon_number, electric_charge, and so forth.
In the case of photons, photons are bosons and can very easily and rapidly
appear or disappear. Therefore, the chemical potential of photons is always and
everywhere zero. The reason is, if the chemical potential somewhere was higher
than zero, photons would spontaneously disappear from that area until the
chemical potential went back to zero; likewise if the chemical potential
somewhere was less than zero, photons would spontaneously appear until the
chemical potential went back to zero. Since this process occurs extremely
rapidly (at least, it occurs rapidly in the presence of dense charged matter),
it is safe to assume that the photon chemical potential is never different from
zero.
Electric charge is different, because it is conserved, i.e. it can be neither
created nor destroyed. It can, however, diffuse. The "chemical potential of
electric charge" controls this diffusion: Electric charge, like anything else,
will tend to diffuse from areas of higher chemical potential to areas of lower
chemical potential.[18] Other conserved quantities like baryon_number are the
same. In fact, each conserved quantity is associated with a chemical potential
and a corresponding tendency to diffuse to equalize it out.[19]
In the case of electrons, the behavior depends on temperature and context. At
low temperatures, with no positrons present, electrons cannot be created or
destroyed. Therefore, there is an electron chemical potential that might vary
in space, causing diffusion. At very high temperatures, however, electrons and
positrons can spontaneously appear out of the vacuum (pair_production), so the
chemical potential of electrons by themselves becomes a less useful quantity
than the chemical potential of the conserved quantities like (electrons minus
positrons).
The chemical potentials of bosons and fermions is related to the number of
particles and the temperature by BoseâEinstein_statistics and FermiâDirac
statistics respectively.
**** Ideal vs. non-ideal solutions[edit] ****
The chemical potential of component i in solution for (left) ideal and (right)
real solutions.
Generally the chemical potential is given as a sum of an ideal contribution and
an excess contribution:
          &#x03BC;  i   =  &#x03BC;  i   ideal   +  &#x03BC;  i   excess   ,
      {\displaystyle \mu _{i}=\mu _{i}^{\text{ideal}}+\mu _{i}^{\text
      {excess}},}  [{\displaystyle \mu _{i}=\mu _{i}^{\text{ideal}}+\mu _{i}^
      {\text{excess}},}]
In an ideal solution, the chemical potential of species i (Î¼i) is dependent on
temperature and pressure. Î¼i0(T,P) is defined as the chemical potential of
pure species i. Given this definition the chemical potential of species i in an
ideal solution is:
          &#x03BC;  i   ideal   &#x2248;  &#x03BC;  i 0   + R T ln &#x2061;
      (  x  i   )   {\displaystyle \mu _{i}^{\text{ideal}}\approx \mu _
      {i0}+RT\ln(x_{i})}  [{\displaystyle \mu _{i}^{\text{ideal}}\approx \mu _
      {i0}+RT\ln(x_{i})}]
where R is the gas constant and      x  i     {\displaystyle x_{i}}  [x_{i}] is
the mole fraction of species i contained in the solution. Note that the
approximation is only valid for      x  i     {\displaystyle x_{i}}  [x_{i}]
not approaching zero.
This equation assumes that      &#x03BC;  i     {\displaystyle \mu _{i}}  [\mu
_{i}] only depends on the mole fraction (     x  i     {\displaystyle x_{i}}
[x_{i}]) contained in the solution. This neglects intermolecular interaction
between species i with itself and other species [i-(jâ i)]. This can be
corrected for by factoring in the coefficient of activity of species i, defined
as Î³i. This correction yields:
          &#x03BC;  i   =  &#x03BC;  i 0   ( T , P ) + R T ln &#x2061; (  x  i
      ) + R T ln &#x2061; (  &#x03B3;  i   ) =  &#x03BC;  i 0   ( T , P ) + R T
      ln &#x2061; (  x  i    &#x03B3;  i   )   {\displaystyle \mu _{i}=\mu _
      {i0}(T,P)+RT\ln(x_{i})+RT\ln(\gamma _{i})=\mu _{i0}(T,P)+RT\ln(x_
      {i}\gamma _{i})}  [{\displaystyle \mu _{i}=\mu _{i0}(T,P)+RT\ln(x_
      {i})+RT\ln(\gamma _{i})=\mu _{i0}(T,P)+RT\ln(x_{i}\gamma _{i})}]
The figures to the right give a rough picture of the ideal and non-ideal
situation.
***** See also[edit] *****
    * Chemical_equilibrium
    * Electrochemical_potential
    * Equilibrium_chemistry
    * Excess_chemical_potential
    * Fugacity
    * Partial_molar_property
    * Thermodynamic_activity
    * Thermodynamic_equilibrium
***** References[edit] *****
   1. ^ Opacity, Walter F. Huebner, W. David Barfield,
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
   3. ISBN 1461487978, p. 105, https://books.google.de/books?id=ib-
      8BAAAQBAJ&pg=PA105&dq=partial+molar+free+energy+%22molar+chemical+potential%22&hl=de&sa=X&ved=0ahUKEwi9lbXjosnYAhUCzaQKHap3ChQQ6AEIKDAA#v=onepage&q=partial%20molar%20free%20energy%20%22molar%20chemical%20potential%22&f=false
   4. ^ Atkins, Peter; de Paula, Julio (2006). Atkins' Physical Chemistry (8th
      ed.). Oxford University Press. ISBN 978-0-19-870072-2.
   5.  Page references in this article refer specifically to the 8th edition of
      this book.
   6. ^ Baierlein, Ralph (April 2001). "The_elusive_chemical_potential" (PDF).
      American Journal of Physics. 69 (4): 423â434. Bibcode:
      2001AmJPh..69..423B. doi:10.1119/1.1336839.
   7. ^ Job, G.; Herrmann, F. (February 2006). "Chemical_potentialâa_quantity
      in_search_of_recognition" (PDF). European Journal of Physics. 27 (2):
      353â371. Bibcode:2006EJPh...27..353J. CiteSeerX 10.1.1.568.9205. doi:
      10.1088/0143-0807/27/2/018.
   8. ^Kittel,_Charles; Herbert_Kroemer (1980-01-15). Thermal Physics (2nd
      Edition). W. H. Freeman. p. 357.
   9.
  10. ^ Statistical Physics, F Mandl, (Wiley, London, 11971)
  11. ISBN 0_471_56658_6, page 88
  12. ^ Atkins, Section 4.1, p 126
  13. ^ Atkins, Section 5.5, pp 150-155
  14. ^ Atkins, Section 5.3, pp 143-145
  15. ^ a b c Thermal_Physics by Kittel and Kroemer, second edition, page 124.
  16. ^ Thermodynamics in Earth and Planetary Sciences by Jibamitra Ganguly,
      google_books_link. This text uses "internal", "external", and "total
      chemical potential" as in this article.
  17. ^ Electrochemical Methods by Bard and Faulkner, 2nd edition, Section
      2.2.4(a),4-5.
  18. ^ Electrochemistry at Metal and Semiconductor Electrodes, by Norio Sato,
      pages 4-5, google_books_link
  19. ^ Physics Of Transition Metal Oxides, by Sadamichi Maekawa, p323, google
      books_link
  20. ^ The Physics of Solids: Essentials and Beyond, by Eleftherios N.
      Economou, page 140, google_books_link. In this text, total chemical
      potential is usually called "electrochemical potential", but sometimes
      just "chemical potential". The internal chemical potential is referred to
      by the unwieldy phrase "chemical potential in the absence of the
      [electric] field".
  21. ^ Solid State Physics by Ashcroft and Mermin, page 257 note 36. Page 593
      of the same book uses, instead, an unusual "flipped" definition where
      "chemical potential" is the total chemical potential which is constant in
      equilibrium, and "electrochemical potential" is the internal chemical
      potential; presumably this unusual terminology was an unintentional
      mistake.
  22. ^ Morell, Christophe, Introduction to Density Functional Theory of
      Chemical Reactivity: The so-called Conceptual DFT (http://inac.cea.fr/
      Phocea/file.php?class=pisp&reload=1261486766&file=christophe.morell/
      files/98/
      introduction_to_Density_Functional_Theory_of_Chemical_Reactivity.pdf),
      retrieved May 2016
  23. ^Baierlein, Ralph (2003). Thermal Physics. Cambridge University Press.
      ISBN 978-0-521-65838-6. OCLC 39633743.
  24. ^ Hadrons_and_Quark-Gluon_Plasma, by Jean Letessier, Johann Rafelski, p91
***** External links[edit] *****
    * Chemical_Potential
    * Chemical_Potentials
    * Values_of_the_chemical_potential_of_1300_substances
    * G._Cook_and_R._H._Dickerson_"Understanding_the_chemical_potential",
      American_Journal_of_Physics_63_pp._737-742_(1995)
    * T._A._Kaplan_"The_Chemical_Potential",_Journal_of_Statistical_Physics_122
      pp._1237-1260_(2006)

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Chemical_potential&oldid=906189159"
Categories:
    * Physical_chemistry
    * Potentials
    * Chemical_thermodynamics
    * Thermodynamic_properties
    * Chemical_engineering_thermodynamics
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2011
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
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 14 July 2019, at 07:00 (UTC).
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
