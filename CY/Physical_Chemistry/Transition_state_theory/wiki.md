The following text has been accessed from https://en.wikipedia.org/wiki/Transition_state_theory at Fri Aug 9 02:04:51 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Transition state theory ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Figure 1: Reaction coordinate diagram for the bimolecular nucleophilic
substitution (SN2) reaction between bromomethane and the hydroxide anion
Transition state theory (TST) explains the reaction_rates of elementary
chemical_reactions. The theory assumes a special type of chemical_equilibrium
(quasi-equilibrium) between reactants and activated transition_state complexes.
[1]
TST is used primarily to understand qualitatively how chemical reactions take
place. TST has been less successful in its original goal of calculating
absolute reaction rate constants because the calculation of absolute reaction
rates requires precise knowledge of potential energy surfaces,[2] but it has
been successful in calculating the standard enthalpy of activation (ÎHâ¡,
also written Îâ¡HÉµ), the standard entropy_of_activation (ÎSâ¡ or
Îâ¡SÉµ), and the standard Gibbs_energy of activation (ÎGâ¡ or Îâ¡GÉµ) for
a particular reaction if its rate constant has been experimentally determined.
(The â¡ notation refers to the value of interest at the transition state;
ÎHâ¡ is the difference between the enthalpy of the transition state and that
of the reactants.)
This theory was developed simultaneously in 1935 by Henry_Eyring, then at
Princeton_University, and by Meredith_Gwynne_Evans and Michael_Polanyi of the
University_of_Manchester.[3][4] TST is also referred to as "activated-complex
theory," "absolute-rate theory," and "theory of absolute reaction rates."[5]
Before the development of TST, the Arrhenius rate law was widely used to
determine energies for the reaction barrier. The Arrhenius_equation derives
from empirical observations and ignores any mechanistic considerations, such as
whether one or more reactive intermediates are involved in the conversion of a
reactant to a product.[6] Therefore, further development was necessary to
understand the two parameters associated with this law, the pre-exponential
factor (A) and the activation energy (Ea). TST, which led to the Eyring
equation, successfully addresses these two issues; however, 46 years elapsed
between the publication of the Arrhenius rate law, in 1889, and the Eyring
equation derived from TST, in 1935. During that period, many scientists and
researchers contributed significantly to the development of the theory.
⁰
***** Contents *****
    * 1_Theory
    * 2_Development
          o 2.1_Thermodynamic_treatment
          o 2.2_Kinetic-theory_treatment
          o 2.3_Statistical-mechanical_treatment
          o 2.4_Potential_energy_surfaces
    * 3_Justification_for_the_Eyring_equation
          o 3.1_Quasi-equilibrium_assumption
          o 3.2_Plausibility_argument
    * 4_Inferences_from_transition_state_theory_and_relationship_with_Arrhenius
      theory
    * 5_Limitations_of_transition_state_theory
    * 6_Generalized_transition_state_theory
          o 6.1_Microcanonical_variational_TST
          o 6.2_Canonical_variational_TST
          o 6.3_Improved_canonical_variational_TST
          o 6.4_Nonadiabatic_TST
          o 6.5_Semiclassical_TST
    * 7_Applications_of_TST:_enzymatic_reactions
    * 8_See_also
    * 9_Notes
    * 10_References
    * 11_External_links
***** Theory[edit] *****
The basic ideas behind transition state theory are as follows:
   1. Rates of reaction can be studied by examining activated complexes near
      the saddle_point of a potential_energy_surface. The details of how these
      complexes are formed are not important. The saddle point itself is called
      the transition state.
   2. The activated complexes are in a special equilibrium (quasi-equilibrium)
      with the reactant molecules.
   3. The activated complexes can convert into products, and kinetic theory can
      be used to calculate the rate of this conversion.
***** Development[edit] *****
In the development of TST, three approaches were taken as summarized below
**** Thermodynamic treatment[edit] ****
In 1884, Jacobus_van't_Hoff proposed the Van_'t_Hoff_equation describing the
temperature dependence of the equilibrium constant for a reversible reaction:
           A        &#x21BD;     &#x2212;         &#x2212;     &#x21C0;
      B     {\displaystyle {\ce {{A}<=> {B}}}}  [{\displaystyle {\ce {{A}<=>
      {B}}}}]
            d ln &#x2061; K   d T    =    &#x0394; U   R  T  2
      {\displaystyle {\frac {d\ln K}{dT}}={\frac {\Delta U}{RT^{2}}}}  [{\frac
      {d\ln K}{dT}}={\frac {\Delta U}{RT^{2}}}]
where ÎU is the change in internal energy, K is the equilibrium_constant of
the reaction, R is the universal_gas_constant, and T is thermodynamic
temperature. Based on experimental work, in 1889, Svante_Arrhenius proposed a
similar expression for the rate constant of a reaction, given as follows:
            d ln &#x2061; k   d T    =    &#x0394; E   R  T  2
      {\displaystyle {\frac {d\ln k}{dT}}={\frac {\Delta E}{RT^{2}}}}  [{\frac
      {d\ln k}{dT}}={\frac {\Delta E}{RT^{2}}}]
Integration of this expression leads to the Arrhenius_equation
         k = A  e  &#x2212;  E  a    /  R T     {\displaystyle k=Ae^{-E_{a}/
      RT}}  [k=Ae^{-E_{a}/RT}]
where k is the rate constant. A was referred to as the frequency factor (now
called the pre-exponential coefficient), and Ea is regarded as the activation
energy. By the early 20th century many had accepted the Arrhenius equation, but
the physical interpretation of A and Ea remained vague. This led many
researchers in chemical kinetics to offer different theories of how chemical
reactions occurred in an attempt to relate A and Ea to the molecular dynamics
directly responsible for chemical reactions.[citation_needed]
In 1910, French chemist RenÃ©_Marcelin introduced the concept of standard Gibbs
energy of activation. His relation can be written as
         k &#x221D; exp &#x2061;  (    &#x2212;  &#x0394;  &#x2021;    G
      &#x2296;     R T    )    {\displaystyle k\propto \exp \left({\frac {-
      \Delta ^{\ddagger }G^{\ominus }}{RT}}\right)}  [k\propto \exp \left(
      {\frac {-\Delta ^{\ddagger }G^{\ominus }}{RT}}\right)]
At about the same time as Marcelin was working on his formulation, Dutch
chemists Philip Abraham Kohnstamm, Frans Eppo Cornelis Scheffer, and Wiedold
Frans Brandsma introduced standard entropy of activation and the standard
enthalpy of activation. They proposed the following rate constant equation
         k &#x221D; exp &#x2061;  (     &#x0394;  &#x2021;    S  &#x2296;    R
      )  exp &#x2061;  (    &#x2212;  &#x0394;  &#x2021;    H  &#x2296;     R T
      )    {\displaystyle k\propto \exp \left({\frac {\Delta ^{\ddagger }S^
      {\ominus }}{R}}\right)\exp \left({\frac {-\Delta ^{\ddagger }H^{\ominus
      }}{RT}}\right)}  [k\propto \exp \left({\frac {\Delta ^{\ddagger }S^
      {\ominus }}{R}}\right)\exp \left({\frac {-\Delta ^{\ddagger }H^{\ominus
      }}{RT}}\right)]
However, the nature of the constant was still unclear.
**** Kinetic-theory treatment[edit] ****
In early 1900, Max_Trautz and William_Lewis studied the rate of the reaction
using collision_theory, based on the kinetic_theory_of_gases. Collision_theory
treats reacting molecules as hard spheres colliding with one another; this
theory neglects entropy changes, since it assumes that the collision between
molecules are completely elastic.
Lewis applied his treatment to the following reaction and obtained good
agreement with experimental result.
2HI â H2 + I2
However, later when the same treatment was applied to other reactions, there
were large discrepancies between theoretical and experimental results.
**** Statistical-mechanical treatment[edit] ****
Statistical_mechanics played a significant role in the development of TST.
However, the application of statistical mechanics to TST was developed very
slowly given the fact that in mid-19th century, James_Clerk_Maxwell, Ludwig
Boltzmann, and Leopold_Pfaundler published several papers discussing reaction
equilibrium and rates in terms of molecular motions and the statistical
distribution of molecular speeds.
It was not until 1912 when the French chemist A. Berthoud used the
MaxwellâBoltzmann_distribution law to obtain an expression for the rate
constant.
            d ln &#x2061; k   d T    =    a &#x2212; b T   R  T  2
      {\displaystyle {\frac {d\ln k}{dT}}={\frac {a-bT}{RT^{2}}}}  [{\frac
      {d\ln k}{dT}}={\frac {a-bT}{RT^{2}}}]
where a and b are constants related to energy terms.
Two years later, RenÃ©_Marcelin made an essential contribution by treating the
progress of a chemical reaction as a motion of a point in phase_space. He then
applied Gibbs' statistical-mechanical procedures and obtained an expression
similar to the one he had obtained earlier from thermodynamic consideration.
In 1915, another important contribution came from British physicist James Rice.
Based on his statistical analysis, he concluded that the rate constant is
proportional to the "critical increment". His ideas were further developed by
Richard_Chace_Tolman. In 1919, Austrian physicist Karl_Ferdinand_Herzfeld
applied statistical_mechanics to the equilibrium_constant and kinetic theory to
the rate constant of the reverse reaction, kâ1, for the reversible
dissociation of a diatomic molecule.[7]
          AB   &#x21CC;   k  &#x2212; 1      k 1      A  +  B
      {\displaystyle {\ce {AB <=>[k_1][k_{-1}] {A}+ {B}}}}  [{\displaystyle
      {\ce {AB <=>[k_1][k_{-1}] {A}+ {B}}}}]
He obtained the following equation for the rate constant of the forward
reaction[8]
          k  1   =     k   B    T  h    (  1 &#x2212;  e  &#x2212;    h
      &#x03BD;    k  B   T       )  exp &#x2061;  (    &#x2212;  E  &#x2296;
      R T    )    {\displaystyle k_{1}={\frac {k_{\mathrm {B} }T}{h}}\left(1-e^
      {-{\frac {h\nu }{k_{B}T}}}\right)\exp \left({\frac {-E^{\ominus }}
      {RT}}\right)}  [{\displaystyle k_{1}={\frac {k_{\mathrm {B} }T}{h}}\left
      (1-e^{-{\frac {h\nu }{k_{B}T}}}\right)\exp \left({\frac {-E^{\ominus }}
      {RT}}\right)}]
where       E  &#x2296;      {\displaystyle \textstyle E^{\ominus }}
[\textstyle E^{\ominus }] is the dissociation energy at absolute zero, kB is
the Boltzmann_constant, h is the Planck_constant, T is thermodynamic
temperature, Ï is vibrational_frequency of the bond. This expression is very
important since it is the first time that the factor kBT/h, which is a critical
component of TST, has appeared in a rate equation.
In 1920, the American chemist Richard_Chace_Tolman further developed Rice's
idea of the critical increment. He concluded that critical increment (now
referred to as activation energy) of a reaction is equal to the average energy
of all molecules undergoing reaction minus the average energy of all reactant
molecules.
**** Potential energy surfaces[edit] ****
The concept of potential energy surface was very important in the development
of TST. The foundation of this concept was laid by RenÃ©_Marcelin in 1913. He
theorized that the progress of a chemical reaction could be described as a
point in a potential energy surface with coordinates in atomic momenta and
distances.
In 1931, Henry_Eyring and Michael_Polanyi constructed a potential energy
surface for the reaction below. This surface is a three-dimensional diagram
based on quantum-mechanical principles as well as experimental data on
vibrational frequencies and energies of dissociation.
H + H2 â H2 + H
A year after the Eyring and Polanyi construction, Hans Pelzer and Eugene_Wigner
made an important contribution by following the progress of a reaction on a
potential energy surface. The importance of this work was that it was the first
time that the concept of col or saddle point in the potential energy surface
was discussed. They concluded that the rate of a reaction is determined by the
motion of the system through that col.
It has been typically assumed that the rate-limiting or lowest saddle point is
located on the same energy surface as the initial ground state. However, it was
recently found that this could be incorrect for processes occurring in
semiconductors and insulators, where an initial excited state could go through
a saddle point lower than the one on the surface of the initial ground state.
[9]
***** Justification for the Eyring equation[edit] *****
One of the most important features introduced by Eyring, Polanyi and Evans was
the notion that activated complexes are in quasi-equilibrium with the
reactants. The rate is then directly proportional to the concentration of these
complexes multiplied by the frequency (kBT/h) with which they are converted
into products. Below, a non-rigorous plausibility argument is given for the
functional form of the Eyring equation. However, the key statistical mechanical
factor kBT/h will not be justified, and the argument presented below does not
constitute a true "derivation" of the Eyring equation.[10]
**** Quasi-equilibrium assumption[edit] ****
Quasi-equilibrium is different from classical chemical equilibrium, but can be
described using the same thermodynamic treatment.[5] Consider the reaction
below
           A  +  B        &#x21BD;     &#x2212;         &#x2212;     &#x21C0;
      [ AB ]   &#x2021;    &#x27F6;  P     {\displaystyle {\ce {{A}+{B}<=>{
      [AB]^{\ddagger }}->{P}}}}  [{\displaystyle {\ce {{A}+{B}<=>{[AB]^
      {\ddagger }}->{P}}}}]
Figure 2: Potential energy diagram
where complete equilibrium is achieved between all the species in the system
including activated complexes, [AB]â¡ . Using statistical mechanics,
concentration of [AB]â¡ can be calculated in terms of the concentration of A
and B.
TST assumes that even when the reactants and products are not in equilibrium
with each other, the activated complexes are in quasi-equilibrium with the
reactants. As illustrated in Figure 2, at any instant of time, there are a few
activated complexes, and some were reactant molecules in the immediate past,
which are designated [ABl]â¡ (since they are moving from left to right). The
remainder of them were product molecules in the immediate past ([ABr]â¡).
Since the system is in complete equilibrium, the concentrations of [ABl] â¡
and [ABr]â¡ are equal, so that each concentration is equal to one-half of the
total concentration of activated complexes:[citation_needed]
         [   AB   r    ]  &#x2021;   = [   AB   l    ]  &#x2021;   =   1 2
      [  AB   ]  &#x2021;     {\displaystyle [{\ce {AB}}_{r}]^{\ddagger }=[{\ce
      {AB}}_{l}]^{\ddagger }={\frac {1}{2}}[{\ce {AB}}]^{\ddagger }}  [
      {\displaystyle [{\ce {AB}}_{r}]^{\ddagger }=[{\ce {AB}}_{l}]^{\ddagger }=
      {\frac {1}{2}}[{\ce {AB}}]^{\ddagger }}]
In TST, it is assumed that the flux of activated complexes in the two
directions are independent of each other. That is, if all the product molecules
were suddenly removed from the reaction system, the flow of [ABr]â¡ stops, but
there is still a flow from left to right. Hence, to be technically correct, the
reactants are in equilibrium only with [ABl]â¡, the activated complexes that
were reactants in the immediate past.
**** Plausibility argument[edit] ****
The activated complexes do not follow a Boltzmann distribution of energies, but
an "equilibrium constant" can still be derived from the distribution they do
follow. The equilibrium_constant Kâ¡ for the quasi-equilibrium can be written
as
          K  &#x2021;   =     [ AB ]   &#x2021;     [ A ]   [ B ]
      {\displaystyle K^{\ddagger }={\frac {\ce {[AB]^{\ddagger }}}{\ce {[A]
      [B]}}}}  [{\displaystyle K^{\ddagger }={\frac {\ce {[AB]^{\ddagger }}}
      {\ce {[A][B]}}}}].
So, the concentration of the transition state ABâ¡ is
         [  AB   ]  &#x2021;   =  K  &#x2021;   [  A  ] [  B  ]
      {\displaystyle [{\ce {AB}}]^{\ddagger }=K^{\ddagger }[{\ce {A}}][{\ce
      {B}}]}  [{\displaystyle [{\ce {AB}}]^{\ddagger }=K^{\ddagger }[{\ce {A}}]
      [{\ce {B}}]}].
Therefore, the rate equation for the production of product is
            d [  P  ]   d t    =  k  &#x2021;   [  AB   ]  &#x2021;   =  k
      &#x2021;    K  &#x2021;   [  A  ] [  B  ] = k [  A  ] [  B  ]
      {\displaystyle {\frac {d[{\ce {P}}]}{dt}}=k^{\ddagger }[{\ce {AB}}]^
      {\ddagger }=k^{\ddagger }K^{\ddagger }[{\ce {A}}][{\ce {B}}]=k[{\ce {A}}]
      [{\ce {B}}]}  [{\displaystyle {\frac {d[{\ce {P}}]}{dt}}=k^{\ddagger }[
      {\ce {AB}}]^{\ddagger }=k^{\ddagger }K^{\ddagger }[{\ce {A}}][{\ce
      {B}}]=k[{\ce {A}}][{\ce {B}}]}],
where the rate constant k is given by
         k =  k  &#x2021;    K  &#x2021;     {\displaystyle k=k^{\ddagger }K^
      {\ddagger }}  [k=k^{\ddagger }K^{\ddagger }].
Here, kâ¡ is directly proportional to the frequency of the vibrational mode
responsible for converting the activated complex to the product; the frequency
of this vibrational mode is     &#x03BD;   {\displaystyle \nu }  [\nu ]. Every
vibration does not necessarily lead to the formation of product, so a
proportionality constant     &#x03BA;   {\displaystyle \kappa }  [\kappa ],
referred to as the transmission coefficient, is introduced to account for this
effect. So kâ¡ can be rewritten as
          k  &#x2021;   = &#x03BA; &#x03BD;   {\displaystyle k^{\ddagger
      }=\kappa \nu }  [k^{\ddagger }=\kappa \nu ].
For the equilibrium constant Kâ¡, statistical mechanics leads to a temperature
dependent expression given as
          K  &#x2021;   =     k  B   T   h &#x03BD;     K   &#x2021; &#x2032;
      {\displaystyle K^{\ddagger }={\frac {k_{B}T}{h\nu }}K^{\ddagger '}}  [K^
      {\ddagger }={\frac {k_{B}T}{h\nu }}K^{\ddagger '}] (     K   &#x2021;
      &#x2032;    =:  e    &#x2212; &#x0394;  G  &#x2021;     R T
      {\displaystyle K^{\ddagger '}=:e^{\frac {-\Delta G^{\ddagger }}{RT}}}  [
      {\displaystyle K^{\ddagger '}=:e^{\frac {-\Delta G^{\ddagger }}{RT}}}]).
Combining the new expressions for kâ¡ and Kâ¡, a new rate constant expression
can be written, which is given as
         k =  k  &#x2021;    K  &#x2021;   = &#x03BA;     k  B   T  h    e
      &#x2212; &#x0394;  G  &#x2021;     R T     = &#x03BA;     k  B   T  h
      K   &#x2021; &#x2032;      {\displaystyle k=k^{\ddagger }K^{\ddagger
      }=\kappa {\frac {k_{B}T}{h}}e^{\frac {-\Delta G^{\ddagger }}{RT}}=\kappa
      {\frac {k_{B}T}{h}}K^{\ddagger '}}  [{\displaystyle k=k^{\ddagger }K^
      {\ddagger }=\kappa {\frac {k_{B}T}{h}}e^{\frac {-\Delta G^{\ddagger }}
      {RT}}=\kappa {\frac {k_{B}T}{h}}K^{\ddagger '}}].
Since, by definition, ÎGâ¡ = ÎHâ¡ âTÎSâ¡, the rate constant expression
can be expanded, to give an alternative form of the Eyring equation:
         k = &#x03BA;     k  B   T  h    e    &#x0394;  S  &#x2021;    R     e
      &#x2212; &#x0394;  H  &#x2021;     R T       {\displaystyle k=\kappa
      {\frac {k_{B}T}{h}}e^{\frac {\Delta S^{\ddagger }}{R}}e^{\frac {-\Delta
      H^{\ddagger }}{RT}}}  [k=\kappa {\frac {k_{B}T}{h}}e^{\frac {\Delta S^
      {\ddagger }}{R}}e^{\frac {-\Delta H^{\ddagger }}{RT}}].
For correct dimensionality, the equation needs to have an extra factor of
(câ)1âm for reactions that are not unimolecular:
         k = &#x03BA;     k  B   T  h    e    &#x0394;  S  &#x2021;    R     e
      &#x2212; &#x0394;  H  &#x2021;     R T     (  c  &#x2296;    )  1
      &#x2212; m     {\displaystyle k=\kappa {\frac {k_{B}T}{h}}e^{\frac
      {\Delta S^{\ddagger }}{R}}e^{\frac {-\Delta H^{\ddagger }}{RT}}(c^
      {\ominus })^{1-m}}  [{\displaystyle k=\kappa {\frac {k_{B}T}{h}}e^{\frac
      {\Delta S^{\ddagger }}{R}}e^{\frac {-\Delta H^{\ddagger }}{RT}}(c^
      {\ominus })^{1-m}}],
where câ is the standard concentration 1 mol Lâ1 and m is the molecularity.
***** Inferences from transition state theory and relationship with Arrhenius
theory[edit] *****
The rate constant expression from transition state theory can be used to
calculate the ÎGâ¡, ÎHâ¡, ÎSâ¡, and even ÎVâ¡ (the volume of
activation) using experimental rate data. These so-called activation parameters
give insight into the nature of a transition_state, including energy content
and degree of order, compared to the starting materials and has become a
standard tool for elucidation of reaction mechanisms in physical_organic
chemistry. The free energy of activation, ÎGâ¡, is defined in transition
state theory to be the energy such that     &#x0394;  G  &#x2021;   = &#x2212;
R T ln &#x2061;  K   &#x2021; &#x2032;      {\displaystyle \Delta G^{\ddagger
}=-RT\ln K^{\ddagger '}}  [{\displaystyle \Delta G^{\ddagger }=-RT\ln K^
{\ddagger '}}] holds. The parameters ÎHâ¡ and ÎSâ¡ can then be inferred by
determining ÎGâ¡ = ÎHâ¡ â TÎSâ¡ at different temperatures.
Because the functional form of the Eyring and Arrhenius equations are similar,
it is tempting to relate the activation parameters with the activation energy
and pre-exponential factors of the Arrhenius treatment. However, the Arrhenius
equation was derived from experimental data and models the macroscopic rate
using only two parameters, irrespective of the number of transition states in a
mechanism. In contrast, activation parameters can be found for every transition
state of a multistep mechanism, at least in principle. Thus, although the
enthalpy of activation, ÎHâ¡, is often equated with Arrhenius's activation
energy Ea, they are not equivalent. For a condensed-phase or unimolecular gas-
phase reaction step, Ea = ÎHâ¡ + RT. For other gas-phase reactions, Ea =
ÎHâ¡ + (1 â Înâ¡)RT, where Înâ¡ is the change in the number of
molecules on forming the transition state.[11] (Thus, for a bimolecular gas-
phase process, Ea = ÎHâ¡ + 2RT.)
The entropy of activation, ÎSâ¡, gives the extent to which transition state
(including any solvent molecules involved in or perturbed by the reaction) is
more disordered compared to the starting materials. It offers a concrete
interpretation of the pre-exponential factor A in the Arrhenius equation; for a
unimolecular, single-step process, the rough equivalence A = (kBT/h) exp(1 +
ÎSâ¡/R) (or A = (kBT/h) exp(2 + ÎSâ¡/R) for bimolecular gas-phase
reactions) holds. For a unimolecular process, a negative value indicates a more
ordered, rigid transition state than the ground state, while a positive value
reflects a transition state with looser bonds and/or greater conformational
freedom. It is important to note that, for reasons of dimensionality, reactions
that are bimolecular or higher have ÎSâ¡ values that depend on the standard
state chosen (standard concentration, in particular). For most recent
publications, 1 mol Lâ1 or 1 molar is chosen. Since this choice is a human
construct, based on our definitions of units for molar quantity and volume, the
magnitude and sign of ÎSâ¡ for a single reaction is meaningless by itself;
only comparisons of the value with that of a reference reaction of "known" (or
assumed) mechanism, made at the same standard state, is valid.[12]
The volume of activation is found by taking the partial derivative of ÎGâ¡
with respect to pressure (holding temperature constant):     &#x0394;  V
&#x2021;   := ( &#x2202; &#x0394;  G  &#x2021;    /  &#x2202; P  )  T
{\displaystyle \Delta V^{\ddagger }:=(\partial \Delta G^{\ddagger }/\partial
P)_{T}}  [{\displaystyle \Delta V^{\ddagger }:=(\partial \Delta G^{\ddagger }/
\partial P)_{T}}]. It gives information regarding the size, and hence, degree
of bonding at the transition state. An associative mechanism will likely have a
negative volume of activation, while a dissociative mechanism will likely have
a positive value.
Given the relationship between equilibrium constant and the forward and reverse
rate constants,     K =  k  1    /   k  &#x2212; 1     {\displaystyle K=k_{1}/
k_{-1}}  [{\displaystyle K=k_{1}/k_{-1}}], the Eyring equation implies that
         &#x0394;  G  &#x2218;   = &#x0394;  G  1   &#x2021;   &#x2212;
      &#x0394;  G  &#x2212; 1   &#x2021;     {\displaystyle \Delta G^{\circ
      }=\Delta G_{1}^{\ddagger }-\Delta G_{-1}^{\ddagger }}  [{\displaystyle
      \Delta G^{\circ }=\Delta G_{1}^{\ddagger }-\Delta G_{-1}^{\ddagger }}].
Another implication of TST is the CurtinâHammett_principle: the product ratio
of a kinetically-controlled_reaction from R to two products A and B will
reflect the difference in the free energies of activation from R to the
respective products, assuming there is a single transition state to each one:
            [  A  ]   [  B  ]    =  e  &#x2212; &#x0394; &#x0394;  G  &#x2021;
      /  R T     {\displaystyle {\frac {[\mathrm {A} ]}{[\mathrm {B} ]}}=e^{-
      \Delta \Delta G^{\ddagger }/RT}}  [{\displaystyle {\frac {[\mathrm {A} ]}
      {[\mathrm {B} ]}}=e^{-\Delta \Delta G^{\ddagger }/RT}}] (    &#x0394;
      &#x0394;  G  &#x2021;   = &#x0394;  G   A    &#x2021;   &#x2212; &#x0394;
      G   B    &#x2021;     {\displaystyle \Delta \Delta G^{\ddagger }=\Delta
      G_{\mathrm {A} }^{\ddagger }-\Delta G_{\mathrm {B} }^{\ddagger }}  [
      {\displaystyle \Delta \Delta G^{\ddagger }=\Delta G_{\mathrm {A} }^
      {\ddagger }-\Delta G_{\mathrm {B} }^{\ddagger }}]).
The "1.36 rule": For a thermodynamically-controlled_reaction, every difference
of RT ln 10 â (1.987 Ã 10â3 kcal/mol K)(298 K)(2.303) â 1.36 kcal/mol in
the free energies of products A and B results in a factor of 10 in selectivity
at room temperature (298 K):
            [  A  ]   [  B  ]    =  10  &#x2212; &#x0394;  G  &#x2218;    /
      ( 1.36 &#xA0;  k c a l  /  m o l  )     {\displaystyle {\frac {[\mathrm
      {A} ]}{[\mathrm {B} ]}}=10^{-\Delta G^{\circ }/(1.36\ \mathrm {kcal/mol}
      )}}  [{\displaystyle {\frac {[\mathrm {A} ]}{[\mathrm {B} ]}}=10^{-\Delta
      G^{\circ }/(1.36\ \mathrm {kcal/mol} )}}] (    &#x0394;  G  &#x2218;   =
      G   A    &#x2212;  G   B      {\displaystyle \Delta G^{\circ }=G_{\mathrm
      {A} }-G_{\mathrm {B} }}  [{\displaystyle \Delta G^{\circ }=G_{\mathrm {A}
      }-G_{\mathrm {B} }}]).
Analogously, every 1.36 kcal/mol difference in the free energy of activation
results in a factor of 10 in selectivity for a kinetically-controlled process
at room temperature:[13]
            [  A  ]   [  B  ]    =  10  &#x2212; &#x0394; &#x0394;  G  &#x2021;
      /  ( 1.36 &#xA0;  k c a l  /  m o l  )     {\displaystyle {\frac {
      [\mathrm {A} ]}{[\mathrm {B} ]}}=10^{-\Delta \Delta G^{\ddagger }/(1.36\
      \mathrm {kcal/mol} )}}  [{\displaystyle {\frac {[\mathrm {A} ]}{[\mathrm
      {B} ]}}=10^{-\Delta \Delta G^{\ddagger }/(1.36\ \mathrm {kcal/mol} )}}]
      (    &#x0394; &#x0394;  G  &#x2021;   = &#x0394;  G   A    &#x2021;
      &#x2212; &#x0394;  G   B    &#x2021;     {\displaystyle \Delta \Delta G^
      {\ddagger }=\Delta G_{\mathrm {A} }^{\ddagger }-\Delta G_{\mathrm {B} }^
      {\ddagger }}  [{\displaystyle \Delta \Delta G^{\ddagger }=\Delta G_
      {\mathrm {A} }^{\ddagger }-\Delta G_{\mathrm {B} }^{\ddagger }}]).
Ballpark figures: Using the Eyring equation, there is a straightforward
relationship between ÎGâ¡, first-order rate constants, and reaction half-life
at a given temperature. At 298 K, a reaction with ÎGâ¡ = 23 kcal/mol has a
rate constant of k â 8.4 Ã 10â5 sâ1 and a half life of t1/2 â 2.3
hours, figures that are often rounded to k ~ 10â4 sâ1 and t1/2 ~ 2 h. Thus,
a free energy of activation of this magnitude corresponds to a typical reaction
that proceeds to completion overnight at room temperature. For comparison, the
cyclohexane chair_flip has a ÎGâ¡ of about 11 kcal/mol with k ~ 105 sâ1,
making it a dynamic process that takes place rapidly (faster than the NMR
timescale) at room temperature. At the other end of the scale, the cis/trans
isomerization of 2-butene has a ÎGâ¡ of about 60 kcal/mol, corresponding to k
~ 10â31 sâ1 at 298 K. This is a negligible rate: the half-life is 12 orders
of magnitude longer than the age_of_the_universe.[14]
***** Limitations of transition state theory[edit] *****
In general, TST has provided researchers with a conceptual foundation for
understanding how chemical reactions take place. Even though the theory is
widely applicable, it does have limitations. For example, when applied to each
elementary step of a multi-step reaction, the theory assumes that each
intermediate is long-lived enough to reach a Boltzmann distribution of energies
before continuing to the next step. When the intermediates are very short-
lived, TST fails. In such cases, the momentum of the reaction trajectory from
the reactants to the intermediate can carry forward to affect product
selectivity (an example of such a reaction is the thermal decomposition of
diazaobicyclopentanes, presented by Anslyn and Dougherty).
Transition state theory is also based on the assumption that atomic nuclei
behave according to classical_mechanics.[15] It is assumed that unless atoms or
molecules collide with enough energy to form the transition structure, then the
reaction does not occur. However, according to quantum mechanics, for any
barrier with a finite amount of energy, there is a possibility that particles
can still tunnel across the barrier. With respect to chemical reactions this
means that there is a chance that molecules will react, even if they do not
collide with enough energy to traverse the energy barrier.[16] While this
effect is negligible for reactions with large activation energies, it becomes
an important phenomenon for reactions with relatively low energy barriers,
since the tunneling probability increases with decreasing barrier height.
Transition state theory fails for some reactions at high temperature. The
theory assumes the reaction system will pass over the lowest energy saddle
point on the potential energy surface. While this description is consistent for
reactions occurring at relatively low temperatures, at high temperatures,
molecules populate higher energy vibrational modes; their motion becomes more
complex and collisions may lead to transition states far away from the lowest
energy saddle point. This deviation from transition state theory is observed
even in the simple exchange reaction between diatomic hydrogen and a hydrogen
radical.[17]
Given these limitations, several alternatives to transition state theory have
been proposed. A brief discussion of these theories follows.
***** Generalized transition state theory[edit] *****
Any form of TST, such as microcanonical variational TST, canonical_variational
TST, and improved canonical variational TST, in which the transition state is
not necessarily located at the saddle point, is referred to as generalized
transition state theory.
**** Microcanonical variational TST[edit] ****
A fundamental flaw of transition state theory is that it counts any crossing of
the transition state as a reaction from reactants to products or vice versa. In
reality, a molecule may cross this "dividing surface" and turn around, or cross
multiple times and only truly react once. As such, unadjusted TST is said to
provide an upper bound for the rate coefficients. To correct for this,
variational transition state theory varies the location of the dividing surface
that defines a successful reaction in order to minimize the rate for each fixed
energy. [18] The rate expressions obtained in this microcanonical treatment can
be integrated over the energy, taking into account the statistical distribution
over energy states, so as to give the canonical, or thermal rates.
**** Canonical variational TST[edit] ****
A development of transition state theory in which the position of the dividing
surface is varied so as to minimize the rate constant at a given temperature.
**** Improved canonical variational TST[edit] ****
A modification of canonical variational transition state theory in which, for
energies below the threshold energy, the position of the dividing surface is
taken to be that of the microcanonical threshold energy. This forces the
contributions to rate constants to be zero if they are below the threshold
energy. A compromise dividing surface is then chosen so as to minimize the
contributions to the rate constant made by reactants having higher energies.
**** Nonadiabatic_TST[edit] ****
An expansion of TST to the reactions when two spin-states are involved
simultaneously is called nonadiabatic_transition_state_theory_(NA-TST).
**** Semiclassical_TST[edit] ****
Using vibrational perturbation theory, effects such as tunnelling and
variational effects can be accounted for within the SCTST formalism.
***** Applications of TST: enzymatic reactions[edit] *****
Enzymes_catalyze chemical reactions at rates that are astounding relative to
uncatalyzed chemistry at the same reaction conditions. Each catalytic event
requires a minimum of three or often more steps, all of which occur within the
few milliseconds that characterize typical enzymatic reactions. According to
transition state theory, the smallest fraction of the catalytic cycle is spent
in the most important step, that of the transition state. The original
proposals of absolute reaction rate theory for chemical reactions defined the
transition state as a distinct species in the reaction coordinate that
determined the absolute reaction rate. Soon thereafter, Linus_Pauling proposed
that the powerful catalytic action of enzymes could be explained by specific
tight binding to the transition state species [19] Because reaction rate is
proportional to the fraction of the reactant in the transition state complex,
the enzyme was proposed to increase the concentration of the reactive species.
This proposal was formalized by Wolfenden and coworkers at University_of_North
Carolina_at_Chapel_Hill, who hypothesized that the rate increase imposed by
enzymes is proportional to the affinity of the enzyme for the transition state
structure relative to the Michaelis complex.[20] Because enzymes typically
increase the non-catalyzed reaction rate by factors of 1010-1015, and Michaelis
complexes[clarification_needed] often have dissociation constants in the range
of 10â3-10â6 M, it is proposed that transition state complexes are bound
with dissociation constants in the range of 10â14-10â23 M. As substrate
progresses from the Michaelis complex to product, chemistry occurs by enzyme-
induced changes in electron distribution in the substrate.
Enzymes alter the electronic structure by protonation, proton abstraction,
electron transfer, geometric distortion, hydrophobic partitioning, and
interaction with Lewis acids and bases. These are accomplished by sequential
protein and substrate conformational changes. When a combination of
individually weak forces are brought to bear on the substrate, the summation of
the individual energies results in large forces capable of relocating bonding
electrons to cause bond-breaking and bond-making. Analogs that resemble the
transition state structures should therefore provide the most powerful
noncovalent inhibitors known, even if only a small fraction of the transition
state energy is captured.
All chemical transformations pass through an unstable structure called the
transition state, which is poised between the chemical structures of the
substrates and products. The transition states for chemical reactions are
proposed to have lifetimes near 10â13 seconds, on the order of the time of a
single bond vibration. No physical or spectroscopic method is available to
directly observe the structure of the transition state for enzymatic reactions,
yet transition state structure is central to understanding enzyme catalysis
since enzymes work by lowering the activation energy of a chemical
transformation.
It is now accepted that enzymes function to stabilize transition states lying
between reactants and products, and that they would therefore be expected to
bind strongly any inhibitor that closely resembles such a transition state.
Substrates and products often participate in several enzyme reactions, whereas
the transition state tends to be characteristic of one particular enzyme, so
that such an inhibitor tends to be specific for that particular enzyme. The
identification of numerous transition state inhibitors supports the transition
state stabilization hypothesis for enzymatic catalysis.
Currently there is a large number of enzymes known to interact with transition
state analogs, most of which have been designed with the intention of
inhibiting the target enzyme. Examples include HIV-1 protease, racemases, Î²-
lactamases, metalloproteinases, cyclooxygenases and many others.
***** See also[edit] *****
    * CurtinâHammett_principle
***** Notes[edit] *****
   1. ^ IUPAC, Compendium_of_Chemical_Terminology, 2nd ed. (the "Gold Book")
      (1997). Online corrected version:  (2006–) "transition_state_theory".
      doi:10.1351/goldbook.T06470
   2. ^Truhlar, D. G.; Garrett, B. C.; Klippenstein, S. J. (1996). "Current
      Status of Transition-State Theory". J. Phys. Chem. 100 (31):
      12771â12800. doi:10.1021/jp953748q.
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
   4. ^Laidler, K.; King, C. (1983). "Development of transition-state theory".
      J. Phys. Chem. 87 (15): 2657. doi:10.1021/j100238a002.
   5. ^Laidler, K.; King, C. (1998). "A lifetime of transition-state theory".
      The Chemical Intelligencer. 4 (3): 39.
   6. ^ a bLaidler, K. J. (1969). Theories of Chemical Reaction Rates. McGraw-
      Hill.
   7. ^Anslyn, E. V.; Dougherty, D. A. (2006). "Transition State Theory and
      Related Topics". Modern Physical Organic Chemistry. University Science
      Books. pp. 365â373. ISBN 1891389319.
   8. ^Herzfeld, K. E. (1919). "Zur_Theorie_der_Reaktionsgeschwindigkeiten_in
      Gasen". Annalen der Physik. 364 (15): 635â667. Bibcode:
      1919AnP...364..635H. doi:10.1002/andp.19193641504.
   9. ^ Keith_J._Laidler, Chemical Kinetics (3rd ed., Harper & Row 1987), p.277
  10. ISBN 0-06-043862-2
  11. ^Luo, G.; Kuech, T. F.; Morgan, D. (2018). "Transition state redox during
      dynamical processes in semiconductors and insulators". NPG Asia
      Materials. 10 (4): 45â51. arXiv:1712.01686. Bibcode:
      2018npjAM..10...45L. doi:10.1038/s41427-018-0010-0.
  12. ^ For an introductory treatment of the statistical mechanics and an
      elementary derivation of the Eyring equation, see: Lowry and Richardson,
      Mechanism and Theory in Organic Chemistry, 3rd ed. (Harper & Row, 1987),
      pp. 248-253.
  13. ^Steinfeld, Jeffrey L.; Francisco, Joseph S.; Hase, William L. (1999).
      Chemical Kinetics and Dynamics (2nd ed.). Prentice-Hall. p. 302. ISBN 0-
      13-737123-3.
  14. ^Carpenter, Barry K. (1984). Determination of organic reaction
      mechanisms. New York: Wiley. ISBN 0471893692. OCLC 9894996.
  15. ^Lowry, Thomas H. (1987). Mechanism and theory in organic chemistry.
      Richardson, Kathleen Schueller. (3rd ed.). New York: Harper & Row.
      ISBN 0060440848. OCLC 14214254.
  16. ^Eliel,_Ernest_L._(Ernest_Ludwig) (1994). Stereochemistry of organic
      compounds. Wilen, Samuel H., Mander, Lewis N. New York: Wiley.
      ISBN 0471016705. OCLC 27642721.
  17. ^Eyring, H. (1935). "The Activated Complex in Chemical Reactions". J.
      Chem. Phys. 3 (2): 107â115. Bibcode:1935JChPh...3..107E. doi:10.1063/
      1.1749604.
  18. ^Masel, R. (1996). Principles of Adsorption and Reactions on Solid
      Surfaces. New York: Wiley.
  19. ^Pineda, J. R.; Schwartz, S. D. (2006). "Protein_dynamics_and_catalysis:
      The_problems_of_transition_state_theory_and_the_subtlety_of_dynamic
      control". Phil. Trans. R. Soc. B. 361 (1472): 1433â1438. doi:10.1098/
      rstb.2006.1877. PMC 1647311. PMID 16873129.
  20. ^Truhlar, D.; Garrett, B. (1984). "Variational_Transition_State_Theory".
      Annu. Rev. Phys. Chem. 35: 159â189. Bibcode:1984ARPC...35..159T. doi:
      10.1146/annurev.pc.35.100184.001111.
  21. ^Pauling, L. (1948). "Chemical Achievement and Hope for the Future".
      American Scientist. 36: 50â58.
  22. ^Radzicka, A.; Wolfenden, R. (1995). "A proficient enzyme". Science. 267
      (5194): 90â93. Bibcode:1995Sci...267...90R. doi:10.1126/
      science.7809611. PMID 7809611.
***** References[edit] *****
    * Anslyn, Eric V.; Doughtery, Dennis A., Transition State Theory and
      Related Topics. In Modern Physical Organic Chemistry University Science
      Books: 2006; pp 365â373
    * Cleland, W.W., Isotope Effects: Determination of Enzyme Transition State
      Structure. Methods in Enzymology 1995, 249, 341-373
    * Laidler, K.; King, C., Development of transition-state theory. The
      Journal of Physical Chemistry 1983, 87, (15), 2657
    * Laidler, K., A lifetime of transition-state theory. The Chemical
      Intelligencer 1998, 4, (3), 39
    * Radzicka, A.; Woldenden, R., Transition State and Multisubstrate$Analog
      Inhibitors. Methods in Enzymology 1995, 249, 284-312
    * Schramm, VL., Enzymatic Transition States and Transition State Analog
      Design. Annual Review of Biochemistry 1998, 67, 693-720
    * Schramm, V.L., Enzymatic Transition State Theory and Transition State
      Analogue Design. Journal of Biological Chemistry 2007, 282, (39), 28297-
      28300
***** External links[edit] *****
    * Simple_application_of_TST

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Transition_state_theory&oldid=908055030"
Categories:
    * Chemical_kinetics
    * Chemistry_theories
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_April_2009
    * Articles_with_unsourced_statements_from_December_2018
    * Wikipedia_articles_needing_clarification_from_April_2015
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
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * Magyar
    * ä¸­æ
Edit_links
    * This page was last edited on 27 July 2019, at 03:59 (UTC).
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
