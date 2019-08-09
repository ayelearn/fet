The following text has been accessed from https://en.wikipedia.org/wiki/Free_electron_model at Thu Aug 8 22:57:04 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Free electron model ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the solid-state model for metals. For the model of a free
electron gas, see Fermi_gas.
 This article needs additional citations for verification. Please help improve_this
 article by adding_citations_to_reliable_sources. Unsourced material may be challenged
 and removed.
 Find sources: "Free_electron_model" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (September 2008)(Learn_how_and_when_to_remove_this_template_message)
In solid-state_physics, the free electron model is a simple model for the
behaviour of charge_carriers in a metallic solid. It was developed in 1927,[1]
principally by Arnold_Sommerfeld who combined the classical Drude_model with
quantum_mechanical FermiâDirac_statistics and hence it is also known as the
DrudeâSommerfeld model.
Given its simplicity, it is surprisingly successful in explaining many
experimental phenomena, especially
    * the WiedemannâFranz_law which relates electrical_conductivity and
      thermal_conductivity;
    * the temperature dependence of the electron_heat_capacity;
    * the shape of the electronic density_of_states;
    * the range of binding energy values;
    * electrical conductivities;
    * the Seebeck_coefficient of the thermoelectric_effect;
    * thermal_electron_emission and field_electron_emission from bulk metals.
      [citation_needed]
The free electron model solved many of the inconsistencies related to the Drude
model and gave insight into several other properties of metals. The model
considers that metals are composed of a quantum electron gas where ions play
almost no role. The model can be very predictive when applied to alkali and
noble_metals.
⁰
***** Contents *****
    * 1_Ideas_and_assumptions
    * 2_From_the_Drude_model
    * 3_Properties_of_an_electron_gas
          o 3.1_Density_of_states
          o 3.2_Fermi_Level_-_Electron_Chemical_Potential
          o 3.3_Compressibility_of_metals_and_degeneracy_pressure
    * 4_Additional_predictions
          o 4.1_Heat_capacity
          o 4.2_Mean_free_path
    * 5_Inaccuracies_and_extensions
    * 6_See_also
    * 7_References
***** Ideas and assumptions[edit] *****
In the free electron model four main assumptions are taken into account:
    * Free electron approximation: The interaction between the ions and the
      valence electrons is mostly neglected, except in boundary conditions. The
      ions only keep the charge neutrality in the metal. Unlike in the Drude
      model, the ions are not necessarily the source of collisions.
    * Independent_electron_approximation: The interactions between electrons
      are ignored. The electrostatic fields in metals are weak because of the
      screening_effect.
    * Relaxation-time approximation: There is some unknown scattering mechanism
      such that the electron probability of collision is inversely proportional
      to the relaxation time     &#x03C4;   {\displaystyle \tau }  [\tau ],
      which represents the average time between collisions. The collisions do
      not depend on the electronic configuration.
    * Pauli_exclusion_principle: Each quantum state of the system can only be
      occupied by a single electron. This restriction of available electron
      states is taken into account by FermiâDirac_statistics (see also Fermi
      gas). Main predictions of the free-electron model are derived by the
      Sommerfeld_expansion of the FermiâDirac occupancy for energies around
      the Fermi_level.
The name of the model comes from the first two assumptions, as each electron
can be treated as free_particle with a respective quadratic relation between
energy and momentum.
The crystal lattice is not explicitly taken into account in the free electron
model, but a quantum-mechanical justification was given a year later (1928) by
Bloch's_theorem: an unbound electron moves in a periodic potential as a free
electron in vacuum, except for the electron_mass me becoming an effective_mass
m* which may deviate considerably from me (one can even use negative effective
mass to describe conduction by electron_holes). Effective masses can be derived
from band_structure computations that were not originally taken into account in
the free electron model.
***** From the Drude model[edit] *****
Main article: Drude_model
Many physical properties follow directly from the Drude model as some equations
do not depend on the statistical distribution of the particles. Taking the
classical_velocity_distribution of an ideal gas or the velocity distribution of
a Fermi gas only changes the results related to the speed of the electrons.
Mainly, the free electron model and the Drude model predict the same DC
electrical conductivity Ï for Ohm's_law, that is
          J  = &#x03C3;  E     {\displaystyle \mathbf {J} =\sigma \mathbf {E}
      \quad }  [{\displaystyle \mathbf {J} =\sigma \mathbf {E} \quad }] with
      &#x03C3; =    n  e  2   &#x03C4;   m  e     ,   {\displaystyle \quad
      \sigma ={\frac {ne^{2}\tau }{m_{e}}},}  [{\displaystyle \quad \sigma =
      {\frac {ne^{2}\tau }{m_{e}}},}]
where      J    {\displaystyle \mathbf {J} }  [\mathbf {J} ] is the current
density,      E    {\displaystyle \mathbf {E} }  [\mathbf {E} ] is the external
electric field,     n   {\displaystyle n}  [n] is the electronic_density
(number of electrons/volume) and     e   {\displaystyle e}  [e] is the electron
electric_charge.
Other quantities that remain the same under the free electron model as under
Drude's are the AC susceptibility, the plasma_frequency, the magnetoresistance,
and the Hall coefficient related to the Hall_effect.
***** Properties of an electron gas[edit] *****
Main article: Fermi_gas
Many properties of the free electron model follow directly from equations
related to the Fermi gas, as the independent electron approximation leads to an
ensemble of non-interacting electrons. For a three-dimensional electron gas we
can define the Fermi_energy as
          E   F    =    &#x210F;  2    2  m  e        (  3  &#x03C0;  2   n  )
      2 3    ,   {\displaystyle E_{\rm {F}}={\frac {\hbar ^{2}}{2m_{e}}}\left
      (3\pi ^{2}n\right)^{\frac {2}{3}},}  [{\displaystyle E_{\rm {F}}={\frac
      {\hbar ^{2}}{2m_{e}}}\left(3\pi ^{2}n\right)^{\frac {2}{3}},}]
where     &#x210F;   {\displaystyle \hbar }  [\hbar ] is the reduced Planck
constant. The Fermi_energy defines the energy of the highest energy electron at
zero temperature. For metals the Fermi energy is in the order of units of
electronvolts above the free electron band minimum energy.[2]
In three dimensions, the density_of_states of a gas of fermions is proportional
to the square root of the kinetic energy of the particles.
**** Density of states[edit] ****
The 3D density_of_states (number of energy states, per energy per volume) of a
non-interacting electron gas is given by:
         g ( E ) =    m  e     &#x03C0;  2    &#x210F;  3        2  m  e   E
      =   3 2     n  E   F         E  E   F       ,   {\displaystyle g(E)=
      {\frac {m_{e}}{\pi ^{2}\hbar ^{3}}}{\sqrt {2m_{e}E}}={\frac {3}{2}}{\frac
      {n}{E_{\rm {F}}}}{\sqrt {\frac {E}{E_{\rm {F}}}}},}  [{\displaystyle g
      (E)={\frac {m_{e}}{\pi ^{2}\hbar ^{3}}}{\sqrt {2m_{e}E}}={\frac {3}{2}}
      {\frac {n}{E_{\rm {F}}}}{\sqrt {\frac {E}{E_{\rm {F}}}}},}]
where     E &#x2265; 0   {\textstyle E\geq 0}  [{\textstyle E\geq 0}] is the
energy of a given electron. This formula takes into account the spin degeneracy
but does not consider a possible energy shift due to the bottom of the
conduction_band. For 2D the density of states is constant and for 1D is
inversely proportional to the square root of the electron energy.
**** Fermi Level - Electron Chemical Potential[edit] ****
The chemical_potential     &#x03BC;   {\displaystyle \mu }  [\mu ] of electrons
is also known as the Fermi_Level and like the Fermi_Energy often denoted      E
F      {\displaystyle E_{\rm {F}}}  [{\displaystyle E_{\rm {F}}}]. The
Sommerfeld_expansion is used to calculate the Fermi Level (    T > 0
{\displaystyle T>0}  [T>0]) at higher temperatures, that is
          E   F    ( T ) =  E   F    ( T = 0 )  [  1 &#x2212;    &#x03C0;  2
      12     (   T  T   F      )   2   &#x2212;    &#x03C0;  4   80     (   T
      T   F      )   4   + &#x22EF;  ]  ,   {\displaystyle E_{\rm {F}}(T)=E_
      {\rm {F}}(T=0)\left[1-{\frac {\pi ^{2}}{12}}\left({\frac {T}{T_{\rm
      {F}}}}\right)^{2}-{\frac {\pi ^{4}}{80}}\left({\frac {T}{T_{\rm
      {F}}}}\right)^{4}+\cdots \right],}  [{\displaystyle E_{\rm {F}}(T)=E_{\rm
      {F}}(T=0)\left[1-{\frac {\pi ^{2}}{12}}\left({\frac {T}{T_{\rm
      {F}}}}\right)^{2}-{\frac {\pi ^{4}}{80}}\left({\frac {T}{T_{\rm
      {F}}}}\right)^{4}+\cdots \right],}]
where     T   {\displaystyle T}  [T] is the temperature and we define      T
F    =  E   F     /   k   B      {\textstyle T_{\rm {F}}=E_{\rm {F}}/k_{\rm
{B}}}  [{\textstyle T_{\rm {F}}=E_{\rm {F}}/k_{\rm {B}}}] as the Fermi
temperature (     k   B      {\displaystyle k_{\rm {B}}}  [k_{\rm B}] is
Boltzmann_constant). The perturbative approach is justified as the Fermi
temperature is usually of about 105 K for a metal, hence at room temperature or
lower the Fermi energy      E   F    ( T = 0 )   {\displaystyle E_{\rm {F}}
(T=0)}  [{\displaystyle E_{\rm {F}}(T=0)}] and the chemical potential      E
F    ( T > 0 )   {\displaystyle E_{\rm {F}}(T>0)}  [{\displaystyle E_{\rm {F}}
(T>0)}] are practically equivalent.
**** Compressibility of metals and degeneracy pressure[edit] ****
The total energy per unit volume (at     T = 0   {\textstyle T=0}  [{\textstyle
T=0}]) can also be calculated by integrating over the phase_space of the
system, we obtain
         u ( 0 ) =   3 5   n  E   F    ,   {\displaystyle u(0)={\frac {3}
      {5}}nE_{\rm {F}},}  [{\displaystyle u(0)={\frac {3}{5}}nE_{\rm {F}},}]
which does not depend on temperature. Compare with the energy per electron of
an ideal gas:       3 2    k   B    T   {\textstyle {\frac {3}{2}}k_{\rm {B}}T}
[{\textstyle {\frac {3}{2}}k_{\rm {B}}T}], which is null at zero temperature.
For an ideal gas to have the same energy as the electron gas, the temperatures
would need to be of the order of the Fermi temperature. Thermodynamically, this
energy of the electron gas corresponds to a zero-temperature pressure given by
         P = &#x2212;   (    &#x2202; U   &#x2202; V    )   T , &#x03BC;   =
      2 3   u ( 0 ) ,   {\displaystyle P=-\left({\frac {\partial U}{\partial
      V}}\right)_{T,\mu }={\frac {2}{3}}u(0),}  [{\displaystyle P=-\left({\frac
      {\partial U}{\partial V}}\right)_{T,\mu }={\frac {2}{3}}u(0),}]
where     V   {\textstyle V}  [{\textstyle V}] is the volume and     U ( T ) =
u ( T ) V   {\textstyle U(T)=u(T)V}  [{\textstyle U(T)=u(T)V}] is the total
energy, the derivative performed at temperature and chemical potential
constant. This pressure is called the electron_degeneracy_pressure and does not
come from repulsion or motion of the electrons but from the restriction that no
more than two electrons (due to the two values of spin) can occupy the same
energy level. This pressure defines the compressibility or bulk_modulus of the
metal
         B = &#x2212; V   (    &#x2202; P   &#x2202; V    )   T , &#x03BC;   =
      5 3   P =   2 3   n  E   F    .   {\displaystyle B=-V\left({\frac
      {\partial P}{\partial V}}\right)_{T,\mu }={\frac {5}{3}}P={\frac {2}
      {3}}nE_{\rm {F}}.}  [{\displaystyle B=-V\left({\frac {\partial P}
      {\partial V}}\right)_{T,\mu }={\frac {5}{3}}P={\frac {2}{3}}nE_{\rm
      {F}}.}]
This expression gives the right order of magnitude for the bulk modulus for
alkali metals and noble metals, which show that this pressure is as important
as other effects inside the metal. For other metals the crystalline structure
has to be taken into account.
***** Additional predictions[edit] *****
**** Heat capacity[edit] ****
Further information: Electron_heat_capacity
One open problem in solid-state physics before the arrival of the free electron
model was related to the low heat_capacity of metals. Even when the Drude model
was a good approximation for the Lorenz number of the Wiedemann-Franz law, the
classical argument is based on the idea that the volumetric_heat_capacity of an
ideal gas is
          c  V   Drude   =   3 2   n  k   B      {\displaystyle c_{V}^{\text
      {Drude}}={\frac {3}{2}}nk_{\rm {B}}}  [{\displaystyle c_{V}^{\text
      {Drude}}={\frac {3}{2}}nk_{\rm {B}}}].
If this was the case, the heat capacity of a metal could be much higher due to
this electronic contribution. Nevertheless, such a large heat capacity was
never measured, raising suspicions about the argument. By using Sommerfeld's
expansion one can obtain corrections of the energy density at finite
temperature and obtain the volumetric heat capacity of an electron gas, given
by:
          c  V   =   (    &#x2202; u   &#x2202; T    )   n   =    &#x03C0;  2
      2     T  T   F      n  k   B      {\displaystyle c_{V}=\left({\frac
      {\partial u}{\partial T}}\right)_{n}={\frac {\pi ^{2}}{2}}{\frac {T}{T_
      {\rm {F}}}}nk_{\rm {B}}}  [{\displaystyle c_{V}=\left({\frac {\partial u}
      {\partial T}}\right)_{n}={\frac {\pi ^{2}}{2}}{\frac {T}{T_{\rm {F}}}}nk_
      {\rm {B}}}],
where the prefactor to     n  k  B     {\displaystyle nk_{B}}  [{\displaystyle
nk_{B}}]is considerably smaller than the 3/2 found in      c  V   Drude
{\textstyle c_{V}^{\text{Drude}}}  [{\textstyle c_{V}^{\text{Drude}}}], about
100 times smaller at room temperature and much smaller at lower     T
{\textstyle T}  [{\textstyle T}]. The good estimation of the Lorenz number in
the Drude model was a result of the classical mean velocity of electron being
about 100 larger than the quantum version, compensating the large value of the
classical heat capacity. The free electron model calculation of the Lorenz
factor is about twice the value of Drude's and its closer to the experimental
value. With this heat capacity the free electron model is also able to predict
the right order of magnitude and temperature dependence at low T for the
Seebeck_coefficient of the thermoelectric_effect.
Evidently, the electronic contribution alone does not predict the
DulongâPetit_law, i.e. the observation that the heat capacity of a metal is
constant at high temperatures. The free electron model can be improved in this
sense by adding the lattice vibrations contribution. Two famous schemes to
include the lattice into the problem are the Einstein_solid model and Debye
model. With the addition of the later, the volumetric heat capacity of a metal
at low temperatures can be more precisely written in the form,
          c  V   &#x2248; &#x03B3; T + A  T  3     {\displaystyle c_{V}\approx
      \gamma T+AT^{3}}  [{\displaystyle c_{V}\approx \gamma T+AT^{3}}],
where     &#x03B3;   {\displaystyle \gamma }  [\gamma ] and     A
{\displaystyle A}  [A] are constants of related to the material. The linear
term comes from the electronic contribution while the cubic term comes from
Debye model. At high temperature this expression is no longer correct, the
electronic heat capacity can be neglected, and the total heat capacity of the
metal tends to a constant.
**** Mean free path[edit] ****
Notice that without the relaxation time approximation, there is no reason for
the electrons to deflect their motion, as there are no interactions, thus the
mean_free_path should be infinite. Drude model considered the mean free path of
electrons to be close to the distance between ions in the material, implying
the earlier conclusion that the diffusive_motion of the electrons was due to
collisions with the ions. The mean free paths in the free electron model are
instead given by     &#x03BB; =  v   F    &#x03C4;   {\textstyle \lambda =v_
{\rm {F}}\tau }  [{\textstyle \lambda =v_{\rm {F}}\tau }] (where      v   F
=   2  E   F     /   m  e       {\textstyle v_{\rm {F}}={\sqrt {2E_{\rm {F}}/m_
{e}}}}  [{\textstyle v_{\rm {F}}={\sqrt {2E_{\rm {F}}/m_{e}}}}] is the Fermi
speed) and are in the order of hundreds of Ã¥ngstrÃ¶ms, at least one order of
magnitude larger than any possible classical calculation. The mean free path is
then not a result of electron-ion collisions but instead is related to
imperfections in the material, either due to defects and impurities in the
metal, or due to thermal fluctuations.[3]
***** Inaccuracies and extensions[edit] *****
The free electron model presents several inadequacies that are contradicted by
experimental observation. We list some inaccuracies below:
  Temperature dependence
      The free electron model presents several physical quantities that have
      the wrong temperature dependence, or no dependence at all like the
      electrical conductivity. The thermal conductivity and specific heat are
      well predicted for alkali metals at low temperatures, but fails to
      predict high temperature behaviour coming from ion motion and phonon
      scattering.
  Hall effect and magnetoresistance
      The Hall coefficient has a constant value RH = -1/(ne) in Drude's model
      and in the free electron model. This value is independent of temperature
      and the strength of the magnetic field. The Hall coefficient is actually
      dependent on the band_structure and the difference with the model can be
      quite dramatic when studying elements like magnesium and aluminium that
      have a strong magnetic field dependence. The free electron model also
      predicts that the traverse magnetoresistance, the resistance in the
      direction of the current, does not depend on the strength of the field.
      In almost all the cases it does.
  Directional
      The conductivity of some metals can depend of the orientation of the
      sample with respect to the electric field. Sometimes even the electrical
      current is not parallel to the field. This possibility is not described
      because the model does not integrate the crystallinity of metals, i.e.
      the existence of a periodic lattice of ions.
  Diversity in the conductivity
      Not all materials are electrical_conductors, some do not conduct
      electricity very well (insulators), some can conduct when impurities are
      added like semiconductors. Semimetals, with narrow conduction bands also
      exist. This diversity is not predicted by the model and can only by
      explained by analysing the valence_and_conduction_bands. Additionally,
      electrons are not the only charge carriers in a metal, electron vacancies
      or holes can be seen as quasiparticles carrying positive electric charge.
      Conduction of holes leads to an opposite sign for the Hall and Seebeck
      coefficients predicted by the model.
Other inadequacies are present in the Wiedemann-Franz law at intermediate
temperatures and the frequency-dependence of metals in the optical spectrum.
More exact values for the electrical conductivity and Wiedemann-Franz law can
be obtained by softening the relaxation-time approximation by appealing to
Boltzmann_transport_equations or Kubo_formula.
The spin is mostly neglected in the free electron model and its consequences
can lead to emergent magnetic phenomena like Pauli_paramagnetism and
ferromagnetism.
An immediate continuation to the free electron model can be obtained by
assuming the empty_lattice_approximation, which forms the basis of the band
structure model known as the nearly_free_electron_model.
Adding repulsive interactions between electrons does not change very much the
picture presented here. Lev_Landau showed that a Fermi gas under repulsive
interactions, can be seen as a gas of equivalent quasiparticles that slightly
modify the properties of the metal. Landau's model is now known as the Fermi
liquid_theory. More exotic phenomena like superconductivity, where interactions
can be attractive, require a more refined theory.
***** See also[edit] *****
    * Bloch_wave
    * Electronic_entropy
    * Tight_binding
    * Two-dimensional_electron_gas
    * BoseâEinstein_statistics
    * Fermi_surface
    * White_dwarf
***** References[edit] *****
   1. ^Sommerfeld,_Arnold (1928-01-01). "Zur Elektronentheorie der Metalle auf
      Grund der Fermischen Statistik". Zeitschrift fÃ¼r Physik (in German). 47
      (1â2): 1â32. Bibcode:1928ZPhy...47....1S. doi:10.1007/bf01391052.
      ISSN 0044-3328.
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
   3. ^Nave, Rod. "Fermi_Energies,_Fermi_Temperatures,_and_Fermi_Velocities".
      HyperPhysics. Retrieved 2018-03-21.
   4. ^Tsymbal, Evgeny (2008). "Electronic_Transport" (PDF). University of
      Nebraska-Lincoln. Retrieved 2018-04-21.
  General
    * Kittel,_Charles (1953). Introduction to Solid State Phsysics. University
      of Michigan: Wiley.
Ashcroft,_Neil; Mermin,_N._David (1976). Solid State Physics. New York: Holt,
Rinehart and Winston. ISBN 978-0-03-083993-1.
Sommerfeld,_Arnold; Bethe,_Hans (1933). Elektronentheorie der Metalle. Berlin
Heidelberg: Springer Verlag. ISBN 978-3642950025.
    * v
    * t
    * e
Atomic models
                    * Dalton_model (Billiard ball model)
                    * Thomson_model (Plum pudding model)
                    * Lewis_model (Cubical atom model)
                    * Nagaoka_model (Saturnian model)
Single_atoms        * Rutherford_model (Planetary model)
                    * Bohr_model (RutherfordâBohr model)
                    * BohrâSommerfeld_model (Refined Bohr model)
                    * GryziÅski_model (Free-fall model)
                    * Schrodinger_model (Electron cloud model)
                    * Dirac-Gordon_model (Relativistic atomic model)
                    * Einstein_solid
                    * Debye_model
                    * Drude_model
Atoms in solids     * Free electron model
                    * Nearly_free_electron_model
                    * Band_structure
                    * Density_functional_theory
                    * Ideal_gas
Atoms in fluids     * Van_der_Waals_gas
                    * Newtonian_fluid
                    * BoseâEinstein_condensate
                    * Felix_Bloch
                    * Niels_Bohr
                    * Satyendra_Nath_Bose
                    * John_Dalton
                    * Peter_Debye
                    * Paul_Dirac
                    * Paul_Drude
                    * Albert_Einstein
                    * Walter_Gordon
Scientists          * MichaÅ_GryziÅski
                    * Irving_Langmuir
                    * Gilbert_N._Lewis
                    * Hantaro_Nagaoka
                    * Isaac_Newton
                    * Ernest_Rutherford
                    * Erwin_SchrÃ¶dinger
                    * Arnold_Sommerfeld
                    * J._J._Thomson
                    * Johannes_Diderik_van_der_Waals
    * [Wikipedia book] Book:Atomic_models
    * [Category] Category:Atoms
    * [Portal] Portal:Physics / Chemistry

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Free_electron_model&oldid=909710684"
Categories:
    * Concepts_in_physics
    * Condensed_matter_physics
    * Electronic_band_structures
    * Electron
Hidden categories:
    * CS1_German-language_sources_(de)
    * Articles_needing_additional_references_from_September_2008
    * All_articles_needing_additional_references
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_May_2018
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
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * Magyar
    * æ¥æ¬èª
    * Norsk_nynorsk
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 7 August 2019, at 03:16 (UTC).
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
