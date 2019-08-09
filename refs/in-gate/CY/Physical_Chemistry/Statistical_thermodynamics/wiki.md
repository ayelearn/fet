The following text has been accessed from https://en.wikipedia.org/wiki/Statistical_mechanics at Fri Aug 9 02:04:31 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Statistical mechanics ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Physics of large number of particles' statistical behavior
Statistical mechanics
[Increasing_disorder.svg]
    * Thermodynamics
    * Kinetic_theory
Particle_statistics
    * Spin-statistics_theorem
    * Identical_particles
    * MaxwellâBoltzmann
    * BoseâEinstein
    * FermiâDirac
    * Parastatistics
    * Anyonic_Statistics
    * Braid_Statistics
Thermodynamic_ensembles
    * NVE Microcanonical
    * NVT Canonical
    * ÂµVT Grand_canonical
    * NPH Isoenthalpicâisobaric
    * NPT Isothermalâisobaric
Models
    * Debye
    * Einstein
    * Ising
    * Potts
Potentials
    * Internal_energy
    * Enthalpy
    * Helmholtz_free_energy
    * Gibbs_free_energy
    * Grand_potential_/_Landau_free_energy
Scientists
    * Maxwell
    * Boltzmann
    * Gibbs
    * Einstein
    * Ehrenfest
    * von_Neumann
    * Tolman
    * Debye
    * Fermi
    * Bose
    * v
    * t
    * e
Statistical mechanics is one of the pillars of modern physics. It is necessary
for the fundamental study of any physical system that has a large number of
degrees_of_freedom. The approach is based on statistical methods, probability
theory and the microscopic physical laws.[1][2][3][note_1]
It can be used to explain the thermodynamic behaviour of large systems. This
branch of statistical mechanics, which treats and extends classical
thermodynamics, is known as statistical thermodynamics or equilibrium
statistical mechanics.
Statistical mechanics shows how the concepts from macroscopic observations
(such as temperature and pressure) are related to the description of
microscopic state that fluctuates around an average state. It connects
thermodynamic quantities (such as heat_capacity) to microscopic behavior,
whereas, in classical_thermodynamics, the only available option would be to
measure and tabulate such quantities for various materials.[1]
Statistical mechanics can also be used to study systems that are out of
equilibrium. An important subbranch known as non-equilibrium statistical
mechanics deals with the issue of microscopically modelling the speed of
irreversible_processes that are driven by imbalances. Examples of such
processes include chemical reactions or flows of particles and heat. The
fluctuationâdissipation_theorem is the basic knowledge obtained from applying
non-equilibrium_statistical_mechanics to study the simplest non-equilibrium
situation of a steady state current flow in a system of many particles.
⁰
***** Contents *****
    * 1_Principles:_mechanics_and_ensembles
    * 2_Statistical_thermodynamics
          o 2.1_Fundamental_postulate
          o 2.2_Three_thermodynamic_ensembles
          o 2.3_Calculation_methods
                # 2.3.1_Exact
                # 2.3.2_Monte_Carlo
                # 2.3.3_Other
    * 3_Non-equilibrium_statistical_mechanics
          o 3.1_Stochastic_methods
          o 3.2_Near-equilibrium_methods
          o 3.3_Hybrid_methods
    * 4_Applications_outside_thermodynamics
    * 5_History
    * 6_See_also
    * 7_Notes
    * 8_References
    * 9_External_links
***** Principles: mechanics and ensembles[edit] *****
Main articles: Mechanics and Statistical_ensemble
In physics, there are two types of mechanics usually examined: classical
mechanics and quantum_mechanics. For both types of mechanics, the standard
mathematical approach is to consider two concepts:
   1. The complete state of the mechanical system at a given time,
      mathematically encoded as a phase_point (classical mechanics) or a pure
      quantum_state_vector (quantum mechanics).
   2. An equation of motion which carries the state forward in time: Hamilton's
      equations (classical mechanics) or the time-dependent_SchrÃ¶dinger
      equation (quantum mechanics)
Using these two concepts, the state at any other time, past or future, can in
principle be calculated. There is however a disconnection between these laws
and everyday life experiences, as we do not find it necessary (nor even
theoretically possible) to know exactly at a microscopic level the simultaneous
positions and velocities of each molecule while carrying out processes at the
human scale (for example, when performing a chemical reaction). Statistical
mechanics fills this disconnection between the laws of mechanics and the
practical experience of incomplete knowledge, by adding some uncertainty about
which state the system is in.
Whereas ordinary mechanics only considers the behaviour of a single state,
statistical mechanics introduces the statistical_ensemble, which is a large
collection of virtual, independent copies of the system in various states. The
statistical ensemble is a probability_distribution over all possible states of
the system. In classical statistical mechanics, the ensemble is a probability
distribution over phase points (as opposed to a single phase point in ordinary
mechanics), usually represented as a distribution in a phase_space with
canonical_coordinates. In quantum statistical mechanics, the ensemble is a
probability distribution over pure states,[note_2] and can be compactly
summarized as a density_matrix.
As is usual for probabilities, the ensemble can be interpreted in different
ways:[1]
    * an ensemble can be taken to represent the various possible states that a
      single system could be in (epistemic_probability, a form of knowledge),
      or
    * the members of the ensemble can be understood as the states of the
      systems in experiments repeated on independent systems which have been
      prepared in a similar but imperfectly controlled manner (empirical
      probability), in the limit of an infinite number of trials.
These two meanings are equivalent for many purposes, and will be used
interchangeably in this article.
However the probability is interpreted, each state in the ensemble evolves over
time according to the equation of motion. Thus, the ensemble itself (the
probability distribution over states) also evolves, as the virtual systems in
the ensemble continually leave one state and enter another. The ensemble
evolution is given by the Liouville_equation (classical mechanics) or the von
Neumann_equation (quantum mechanics). These equations are simply derived by the
application of the mechanical equation of motion separately to each virtual
system contained in the ensemble, with the probability of the virtual system
being conserved over time as it evolves from state to state.
One special class of ensemble is those ensembles that do not evolve over time.
These ensembles are known as equilibrium ensembles and their condition is known
as statistical equilibrium. Statistical equilibrium occurs if, for each state
in the ensemble, the ensemble also contains all of its future and past states
with probabilities equal to the probability of being in that state.[note_3] The
study of equilibrium ensembles of isolated systems is the focus of statistical
thermodynamics. Non-equilibrium statistical mechanics addresses the more
general case of ensembles that change over time, and/or ensembles of non-
isolated systems.
***** Statistical thermodynamics[edit] *****
The primary goal of statistical thermodynamics (also known as equilibrium
statistical mechanics) is to derive the classical_thermodynamics of materials
in terms of the properties of their constituent particles and the interactions
between them. In other words, statistical thermodynamics provides a connection
between the macroscopic properties of materials in thermodynamic_equilibrium,
and the microscopic behaviours and motions occurring inside the material.
Whereas statistical mechanics proper involves dynamics, here the attention is
focussed on statistical equilibrium (steady state). Statistical equilibrium
does not mean that the particles have stopped moving (mechanical_equilibrium),
rather, only that the ensemble is not evolving.
**** Fundamental postulate[edit] ****
A sufficient (but not necessary) condition for statistical equilibrium with an
isolated system is that the probability distribution is a function only of
conserved properties (total energy, total particle numbers, etc.).[1] There are
many different equilibrium ensembles that can be considered, and only some of
them correspond to thermodynamics.[1] Additional postulates are necessary to
motivate why the ensemble for a given system should have one form or another.
A common approach found in many textbooks is to take the equal a priori
probability postulate.[2] This postulate states that
      For an isolated system with an exactly known energy and exactly known
      composition, the system can be found withequal probabilityin any
      microstate consistent with that knowledge.
The equal a priori probability postulate therefore provides a motivation for
the microcanonical_ensemble described below. There are various arguments in
favour of the equal a priori probability postulate:
    * Ergodic_hypothesis: An ergodic system is one that evolves over time to
      explore "all accessible" states: all those with the same energy and
      composition. In an ergodic system, the microcanonical ensemble is the
      only possible equilibrium ensemble with fixed energy. This approach has
      limited applicability, since most systems are not ergodic.
    * Principle_of_indifference: In the absence of any further information, we
      can only assign equal probabilities to each compatible situation.
    * Maximum_information_entropy: A more elaborate version of the principle of
      indifference states that the correct ensemble is the ensemble that is
      compatible with the known information and that has the largest Gibbs
      entropy (information_entropy).[4]
Other fundamental postulates for statistical mechanics have also been proposed.
[5]
**** Three thermodynamic ensembles[edit] ****
Main articles: Microcanonical_ensemble, Canonical_ensemble, and Grand_canonical
ensemble
There are three equilibrium ensembles with a simple form that can be defined
for any isolated_system bounded inside a finite volume.[1] These are the most
often discussed ensembles in statistical thermodynamics. In the macroscopic
limit (defined below) they all correspond to classical thermodynamics.
  Microcanonical_ensemble
      describes a system with a precisely given energy and fixed composition
      (precise number of particles). The microcanonical ensemble contains with
      equal probability each possible state that is consistent with that energy
      and composition.
  Canonical_ensemble
      describes a system of fixed composition that is in thermal_equilibrium
      [note_4] with a heat_bath of a precise temperature. The canonical
      ensemble contains states of varying energy but identical composition; the
      different states in the ensemble are accorded different probabilities
      depending on their total energy.
  Grand_canonical_ensemble
      describes a system with non-fixed composition (uncertain particle
      numbers) that is in thermal and chemical equilibrium with a thermodynamic
      reservoir. The reservoir has a precise temperature, and precise chemical
      potentials for various types of particle. The grand canonical ensemble
      contains states of varying energy and varying numbers of particles; the
      different states in the ensemble are accorded different probabilities
      depending on their total energy and total particle numbers.
For systems containing many particles (the thermodynamic_limit), all three of
the ensembles listed above tend to give identical behaviour. It is then simply
a matter of mathematical convenience which ensemble is used.[6] The Gibbs
theorem about equivalence of ensembles[7] was developed into the theory of
concentration_of_measure phenomenon,[8] which has applications in many areas of
science, from functional analysis to methods of artificial_intelligence and big
data technology.[9]
Important cases where the thermodynamic ensembles do not give identical results
include:
    * Microscopic systems.
    * Large systems at a phase transition.
    * Large systems with long-range interactions.
In these cases the correct thermodynamic ensemble must be chosen as there are
observable differences between these ensembles not just in the size of
fluctuations, but also in average quantities such as the distribution of
particles. The correct ensemble is that which corresponds to the way the system
has been prepared and characterizedâin other words, the ensemble that
reflects the knowledge about that system.[2]
                  Thermodynamic ensembles[1]
                  Microcanonical       Canonical            Grand_canonical
      Fixed             N, E, V              N, T, V              Î¼, T, V
      variables
                                                                *     Grand
                                                                    partition
                                                                     function
                                           *   Canonical        *        Z   =
                                               partition           &#x2211;  k
                                                function           e  &#x2212;
                                           *        Z =              (  E  k
                                              &#x2211;  k            &#x2212;
                      *   Number of          e  &#x2212;  E       &#x03BC;  N  k
                         microstates         k    /   k  B         )  /   k  B
      Microscopic     *       W                  T                    T
      features          {\displaystyle       {\displaystyle       {\displaystyle
                           W}  [W]           Z=\sum _{k}e^          {\mathcal
                                               {-E_{k}/k_          {Z}}=\sum _
                                                {B}T}}            {k}e^{-(E_{k}-
                                             [Z=\sum _{k}e^       \mu N_{k})/k_
                                               {-E_{k}/k_           {B}T}}  [
                                                 {B}T}]             {\mathcal
                                                                   {Z}}=\sum _
                                                                  {k}e^{-(E_{k}-
                                                                  \mu N_{k})/k_
                                                                      {B}T}]
                                                                *     Grand
                                                                    potential
                                           * Helmholtz_free     *    &#x03A9; =
                      *   Boltzmann              energy           &#x2212;  k  B
                           entropy         *        F =           T log &#x2061;
                      *     S =  k  B        &#x2212;  k  B           Z
                        log &#x2061; W       T log &#x2061;       {\displaystyle
      Macroscopic       {\displaystyle            Z                \Omega =-k_
      function          S=k_{B}\log W}       {\displaystyle         {B}T\log
                              [              F=-k_{B}T\log          {\mathcal
                        {\displaystyle           Z}  [               {Z}}}  [
                         S=k_{B}\log         {\displaystyle       {\displaystyle
                             W}]             F=-k_{B}T\log         \Omega =-k_
                                                  Z}]               {B}T\log
                                                                    {\mathcal
                                                                      {Z}}}]
**** Calculation methods[edit] ****
Once the characteristic state function for an ensemble has been calculated for
a given system, that system is 'solved' (macroscopic observables can be
extracted from the characteristic state function). Calculating the
characteristic state function of a thermodynamic ensemble is not necessarily a
simple task, however, since it involves considering every possible state of the
system. While some hypothetical systems have been exactly solved, the most
general (and realistic) case is too complex for an exact solution. Various
approaches exist to approximate the true ensemble and allow calculation of
average quantities.
*** Exact[edit] ***
There are some cases which allow exact solutions.
    * For very small microscopic systems, the ensembles can be directly
      computed by simply enumerating over all possible states of the system
      (using exact diagonalization in quantum mechanics, or integral over all
      phase space in classical mechanics).
    * Some large systems consist of many separable microscopic systems, and
      each of the subsystems can be analysed independently. Notably, idealized
      gases of non-interacting particles have this property, allowing exact
      derivations of MaxwellâBoltzmann_statistics, FermiâDirac_statistics,
      and BoseâEinstein_statistics.[2]
    * A few large systems with interaction have been solved. By the use of
      subtle mathematical techniques, exact solutions have been found for a few
      toy_models.[10] Some examples include the Bethe_ansatz, square-lattice
      Ising_model in zero field, hard_hexagon_model.
*** Monte Carlo[edit] ***
Main article: Monte_Carlo_method
One approximate approach that is particularly well suited to computers is the
Monte_Carlo_method, which examines just a few of the possible states of the
system, with the states chosen randomly (with a fair weight). As long as these
states form a representative sample of the whole set of states of the system,
the approximate characteristic function is obtained. As more and more random
samples are included, the errors are reduced to an arbitrarily low level.
    * The MetropolisâHastings_algorithm is a classic Monte Carlo method which
      was initially used to sample the canonical ensemble.
    * Path_integral_Monte_Carlo, also used to sample the canonical ensemble.
*** Other[edit] ***
    * For rarefied non-ideal gases, approaches such as the cluster_expansion
      use perturbation_theory to include the effect of weak interactions,
      leading to a virial_expansion.[3]
    * For dense fluids, another approximate approach is based on reduced
      distribution functions, in particular the radial_distribution_function.
      [3]
    * Molecular_dynamics computer simulations can be used to calculate
      microcanonical_ensemble averages, in ergodic systems. With the inclusion
      of a connection to a stochastic heat bath, they can also model canonical
      and grand canonical conditions.
    * Mixed methods involving non-equilibrium statistical mechanical results
      (see below) may be useful.
***** Non-equilibrium statistical mechanics[edit] *****
See also: Non-equilibrium_thermodynamics
There are many physical phenomena of interest that involve quasi-thermodynamic
processes out of equilibrium, for example:
    * heat_transport_by_the_internal_motions_in_a_material, driven by a
      temperature imbalance,
    * electric_currents_carried_by_the_motion_of_charges_in_a_conductor, driven
      by a voltage imbalance,
    * spontaneous chemical_reactions driven by a decrease in free energy,
    * friction, dissipation, quantum_decoherence,
    * systems being pumped by external forces (optical_pumping, etc.),
    * and irreversible processes in general.
All of these processes occur over time with characteristic rates, and these
rates are of importance for engineering. The field of non-equilibrium
statistical mechanics is concerned with understanding these non-equilibrium
processes at the microscopic level. (Statistical thermodynamics can only be
used to calculate the final result, after the external imbalances have been
removed and the ensemble has settled back down to equilibrium.)
In principle, non-equilibrium statistical mechanics could be mathematically
exact: ensembles for an isolated system evolve over time according to
deterministic equations such as Liouville's_equation or its quantum equivalent,
the von_Neumann_equation. These equations are the result of applying the
mechanical equations of motion independently to each state in the ensemble.
Unfortunately, these ensemble evolution equations inherit much of the
complexity of the underlying mechanical motion, and so exact solutions are very
difficult to obtain. Moreover, the ensemble evolution equations are fully
reversible and do not destroy information (the ensemble's Gibbs_entropy is
preserved). In order to make headway in modelling irreversible processes, it is
necessary to consider additional factors besides probability and reversible
mechanics.
Non-equilibrium mechanics is therefore an active area of theoretical research
as the range of validity of these additional assumptions continues to be
explored. A few approaches are described in the following subsections.
**** Stochastic methods[edit] ****
One approach to non-equilibrium statistical mechanics is to incorporate
stochastic (random) behaviour into the system. Stochastic behaviour destroys
information contained in the ensemble. While this is technically inaccurate
(aside from hypothetical_situations_involving_black_holes, a system cannot in
itself cause loss of information), the randomness is added to reflect that
information of interest becomes converted over time into subtle correlations
within the system, or to correlations between the system and environment. These
correlations appear as chaotic or pseudorandom influences on the variables of
interest. By replacing these correlations with randomness proper, the
calculations can be made much easier.
    * Boltzmann_transport_equation: An early form of stochastic mechanics
      appeared even before the term "statistical mechanics" had been coined, in
      studies of kinetic_theory. James_Clerk_Maxwell had demonstrated that
      molecular collisions would lead to apparently chaotic motion inside a
      gas. Ludwig_Boltzmann subsequently showed that, by taking this molecular
      chaos for granted as a complete randomization, the motions of particles
      in a gas would follow a simple Boltzmann_transport_equation that would
      rapidly restore a gas to an equilibrium state (see H-theorem).
      The Boltzmann_transport_equation and related approaches are important
      tools in non-equilibrium statistical mechanics due to their extreme
      simplicity. These approximations work well in systems where the
      "interesting" information is immediately (after just one collision)
      scrambled up into subtle correlations, which essentially restricts them
      to rarefied gases. The Boltzmann transport equation has been found to be
      very useful in simulations of electron transport in lightly doped
      semiconductors (in transistors), where the electrons are indeed analogous
      to a rarefied gas.
      A quantum technique related in theme is the random_phase_approximation.
    * BBGKY_hierarchy: In liquids and dense gases, it is not valid to
      immediately discard the correlations between particles after one
      collision. The BBGKY_hierarchy
      (BogoliubovâBornâGreenâKirkwoodâYvon hierarchy) gives a method
      for deriving Boltzmann-type equations but also extending them beyond the
      dilute gas case, to include correlations after a few collisions.
    * Keldysh_formalism (a.k.a. NEGFânon-equilibrium Green functions): A
      quantum approach to including stochastic dynamics is found in the Keldysh
      formalism. This approach often used in electronic quantum_transport
      calculations.
**** Near-equilibrium methods[edit] ****
Another important class of non-equilibrium statistical mechanical models deals
with systems that are only very slightly perturbed from equilibrium. With very
small perturbations, the response can be analysed in linear_response_theory. A
remarkable result, as formalized by the fluctuation-dissipation_theorem, is
that the response of a system when near equilibrium is precisely related to the
fluctuations that occur when the system is in total equilibrium. Essentially, a
system that is slightly away from equilibriumâwhether put there by external
forces or by fluctuationsârelaxes towards equilibrium in the same way, since
the system cannot tell the difference or "know" how it came to be away from
equilibrium.[3]:664
This provides an indirect avenue for obtaining numbers such as ohmic
conductivity and thermal_conductivity by extracting results from equilibrium
statistical mechanics. Since equilibrium statistical mechanics is
mathematically well defined and (in some cases) more amenable for calculations,
the fluctuation-dissipation connection can be a convenient shortcut for
calculations in near-equilibrium statistical mechanics.
A few of the theoretical tools used to make this connection include:
    * Fluctuationâdissipation_theorem
    * Onsager_reciprocal_relations
    * GreenâKubo_relations
    * LandauerâBÃ¼ttiker_formalism
    * MoriâZwanzig_formalism
**** Hybrid methods[edit] ****
An advanced approach uses a combination of stochastic methods and linear
response theory. As an example, one approach to compute quantum coherence
effects (weak_localization, conductance_fluctuations) in the conductance of an
electronic system is the use of the Green-Kubo relations, with the inclusion of
stochastic dephasing by interactions between various electrons by use of the
Keldysh method.[11][12]
***** Applications outside thermodynamics[edit] *****
The ensemble formalism also can be used to analyze general mechanical systems
with uncertainty in knowledge about the state of a system. Ensembles are also
used in:
    * propagation_of_uncertainty over time,[1]
    * regression_analysis of gravitational orbits,
    * ensemble_forecasting of weather,
    * dynamics of neural_networks,
    * bounded-rational potential_games in game theory and economics.
***** History[edit] *****
In 1738, Swiss physicist and mathematician Daniel_Bernoulli published
Hydrodynamica which laid the basis for the kinetic_theory_of_gases. In this
work, Bernoulli posited the argument, still used to this day, that gases
consist of great numbers of molecules moving in all directions, that their
impact on a surface causes the gas pressure that we feel, and that what we
experience as heat is simply the kinetic energy of their motion.[5]
In 1859, after reading a paper on the diffusion of molecules by Rudolf
Clausius, Scottish physicist James_Clerk_Maxwell formulated the Maxwell
distribution of molecular velocities, which gave the proportion of molecules
having a certain velocity in a specific range.[13] This was the first-ever
statistical law in physics.[14] Maxwell also gave the first mechanical argument
that molecular collisions entail an equalization of temperatures and hence a
tendency towards equilibrium.[15] Five years later, in 1864, Ludwig_Boltzmann,
a young student in Vienna, came across Maxwell's paper and spent much of his
life developing the subject further.
Statistical mechanics proper was initiated in the 1870s with the work of
Boltzmann, much of which was collectively published in his 1896 Lectures on Gas
Theory.[16] Boltzmann's original papers on the statistical interpretation of
thermodynamics, the H-theorem, transport_theory, thermal_equilibrium, the
equation_of_state of gases, and similar subjects, occupy about 2,000 pages in
the proceedings of the Vienna Academy and other societies. Boltzmann introduced
the concept of an equilibrium statistical ensemble and also investigated for
the first time non-equilibrium statistical mechanics, with his H-theorem.
The term "statistical mechanics" was coined by the American mathematical
physicist J._Willard_Gibbs in 1884.[17][note_5] "Probabilistic mechanics" might
today seem a more appropriate term, but "statistical mechanics" is firmly
entrenched.[18] Shortly before his death, Gibbs published in 1902 Elementary
Principles_in_Statistical_Mechanics, a book which formalized statistical
mechanics as a fully general approach to address all mechanical
systemsâmacroscopic or microscopic, gaseous or non-gaseous.[1] Gibbs' methods
were initially derived in the framework classical_mechanics, however they were
of such generality that they were found to adapt easily to the later quantum
mechanics, and still form the foundation of statistical mechanics to this day.
[2]
***** See also[edit] *****
 Fundamentals_of_Statistical_Mechanics â Wikipedia_book
    * Thermodynamics: non-equilibrium, chemical
    * Mechanics: classical, quantum
    * Probability, statistical_ensemble
    * Numerical methods: Monte_Carlo_method, molecular_dynamics
    * Statistical_physics
    * Quantum_statistical_mechanics
    * List_of_notable_textbooks_in_statistical_mechanics
    * List_of_important_publications_in_statistical_mechanics
***** Notes[edit] *****
   1. ^ The term statistical mechanics is sometimes used to refer to only
      statistical thermodynamics. This article takes the broader view. By some
      definitions, statistical_physics is an even broader term which
      statistically studies any type of physical system, but is often taken to
      be synonymous with statistical mechanics.
   2. ^ The probabilities in quantum statistical mechanics should not be
      confused with quantum_superposition. While a quantum ensemble can contain
      states with quantum superpositions, a single quantum state cannot be used
      to represent an ensemble.
   3. ^ Statistical equilibrium should not be confused with mechanical
      equilibrium. The latter occurs when a mechanical system has completely
      ceased to evolve even on a microscopic scale, due to being in a state
      with a perfect balancing of forces. Statistical equilibrium generally
      involves states that are very far from mechanical equilibrium.
   4. ^ The transitive thermal equilibrium (as in, "X is thermal equilibrium
      with Y") used here means that the ensemble for the first system is not
      perturbed when the system is allowed to weakly interact with the second
      system.
   5. ^ According to Gibbs, the term "statistical", in the context of
      mechanics, i.e. statistical mechanics, was first used by the Scottish
      physicist James_Clerk_Maxwell in 1871. From: J. Clerk Maxwell, Theory of
      Heat (London, England: Longmans, Green, and Co., 1871), p. 309: "In
      dealing with masses of matter, while we do not perceive the individual
      molecules, we are compelled to adopt what I have described as the
      statistical method of calculation, and to abandon the strict dynamical
      method, in which we follow every motion by the calculus."
***** References[edit] *****
   1. ^ a b c d e f g h iGibbs,_Josiah_Willard (1902). Elementary_Principles_in
      Statistical_Mechanics. New York: Charles_Scribner's_Sons.
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
   3. ^ a b c d eTolman,_R._C. (1938). The Principles of Statistical Mechanics.
      Dover_Publications. ISBN 9780486638966.
   4. ^ a b c dBalescu,_Radu (1975). Equilibrium and Non-Equilibrium
      Statistical Mechanics. John Wiley & Sons. ISBN 9780471046004.
   5. ^Jaynes,_E. (1957). "Information Theory and Statistical Mechanics".
      Physical Review. 106 (4): 620â630. Bibcode:1957PhRv..106..620J. doi:
      10.1103/PhysRev.106.620.
   6. ^ a b J. Uffink, "Compendium_of_the_foundations_of_classical_statistical
      physics." (2006)
   7. ^Reif, F. (1965). Fundamentals of Statistical and Thermal Physics.
      McGrawâHill. p. 227. ISBN 9780070518001.
   8. ^Touchette, Hugo (2015). "Equivalence and Nonequivalence of Ensembles:
      Thermodynamic, Macrostate, and Measure Levels". Journal of Statistical
      Physics. 159 (5): 987â1016. arXiv:1403.6608. doi:10.1007/s10955-015-
      1212-2.
   9. ^Ledoux, Michel (2005). The Concentration of Measure Phenomenon.
      Mathematical Surveys and Monographs. 89. doi:10.1090/surv/089.
      ISBN 9780821837924.
  10. .
  11. ^Gorban, A. N.; Tyukin, I. Y. (2018). "Blessing_of_dimensionality:
      Mathematical_foundations_of_the_statistical_physics_of_data".
      Philosophical Transactions of the Royal Society A: Mathematical, Physical
      and Engineering Sciences. 376 (2118): 20170237. doi:10.1098/
      rsta.2017.0237. PMC 5869543.
  12. ^Baxter, Rodney J. (1982). Exactly solved models in statistical
      mechanics. Academic Press Inc. ISBN 9780120831807.
  13. ^Altshuler, B. L.; Aronov, A. G.; Khmelnitsky, D. E. (1982). "Effects of
      electron-electron collisions with small energy transfers on quantum
      localisation". Journal of Physics C: Solid State Physics. 15 (36): 7367.
      Bibcode:1982JPhC...15.7367A. doi:10.1088/0022-3719/15/36/018.
  14. ^Aleiner, I.; Blanter, Y. (2002). "Inelastic_scattering_time_for
      conductance_fluctuations". Physical Review B. 65 (11): 115317. arXiv:
      cond-mat/0105436. Bibcode:2002PhRvB..65k5317A. doi:10.1103/
      PhysRevB.65.115317.
  15. ^ See:
          o Maxwell, J.C. (1860) "Illustrations_of_the_dynamical_theory_of
            gases._Part_I._On_the_motions_and_collisions_of_perfectly_elastic
            spheres," Philosophical Magazine, 4th series, 19 : 19â32.
          o Maxwell, J.C. (1860) "Illustrations_of_the_dynamical_theory_of
            gases._Part_II._On_the_process_of_diffusion_of_two_or_more_kinds_of
            moving_particles_among_one_another," Philosophical Magazine, 4th
            series, 20 : 21â37.
  16. ^Mahon, Basil (2003). The Man Who Changed Everything â the Life of
      James Clerk Maxwell. Hoboken, NJ: Wiley. ISBN 978-0-470-86171-4.
      OCLC 52358254.
  17. ^Gyenis, Balazs (2017). "Maxwell and the normal distribution: A colored
      story of probability, independence, and tendency towards equilibrium".
      Studies in History and Philosophy of Modern Physics. 57: 53â65. arXiv:
      1702.01411. Bibcode:2017SHPMP..57...53G. doi:10.1016/j.shpsb.2017.01.001.
  18. ^Ebeling, Werner; Sokolov, Igor M. (2005). Statistical_Thermodynamics_and
      Stochastic_Theory_of_Nonequilibrium_Systems. Statistical Thermodynamics
      and Stochastic Theory of Nonequilibrium Systems. Edited by Ebeling Werner
      & Sokolov Igor M. Published by World Scientific Press. Series on Advances
      in Statistical Mechanics. 8. pp. 3â12. Bibcode:2005stst.book.....E.
      doi:10.1142/2012. ISBN 978-90-277-1674-3.
  19.  (section 1.2)
  20. ^ J. W. Gibbs, "On the Fundamental Formula of Statistical Mechanics, with
      Applications to Astronomy and Thermodynamics." Proceedings of the
      American Association for the Advancement of Science, 33, 57-58 (1884).
      Reproduced in The Scientific Papers of J. Willard Gibbs, Vol II (1906),
      pp. 16.
  21. ^Mayants, Lazar (1984). The_enigma_of_probability_and_physics. Springer.
      p. 174. ISBN 978-90-277-1674-3.
***** External links[edit] *****
 Wikimedia Commons has media related to Statistical_mechanics.
    * Philosophy_of_Statistical_Mechanics article by Lawrence Sklar for the
      Stanford_Encyclopedia_of_Philosophy.
    * Sklogwiki_-_Thermodynamics,_statistical_mechanics,_and_the_computer
      simulation_of_materials. SklogWiki is particularly orientated towards
      liquids and soft condensed matter.
    * Statistical_Thermodynamics - Historical Timeline
    * Thermodynamics_and_Statistical_Mechanics by Richard Fitzpatrick
    * Lecture_Notes_in_Statistical_Mechanics_and_Mesoscopics by Doron Cohen
    * Videos_of_lecture_series_in_statistical_mechanics on YouTube taught by
      Leonard_Susskind.
    * Vu-Quoc, L., Configuration_integral_(statistical_mechanics), 2008. this
      wiki site is down; see this_article_in_the_web_archive_on_2012_April_28.
    * v
    * t
    * e
Statistical mechanics
Theory                         * Principle_of_maximum_entropy
                               * ergodic_theory
                               * Ensembles
                               * partition_functions
                               * equations_of_state
                               * thermodynamic_potential:
Statistical_thermodynamics           o U
                                     o H
                                     o F
                                     o G
                               * Maxwell_relations
                               * Ferromagnetism_models
                                     o Ising
                                     o Potts
Models                               o Heisenberg
                                     o percolation
                               * Particles with force_field
                                     o depletion_force
                                     o Lennard-Jones_potential
                               * Boltzmann_equation
                               * H-theorem
Mathematical approaches        * Vlasov_equation
                               * BBGKY_hierarchy
                               * stochastic_process
                               * mean_field_theory and conformal_field_theory
                               * Phase_transition
Critical_phenomena             * Critical_exponents
                                     o correlation_length
                                     o size_scaling
                               * Boltzmann
                               * Shannon
Entropy                        * Tsallis
                               * RÃ©nyi
                               * von_Neumann
                               * Statistical_field_theory
                                     o elementary_particle
                                     o superfluidity
Applications                   * condensed_matter_physics
                               * complex_system
                                     o chaos
                                     o information_theory
                                     o Boltzmann_machine
    * v
    * t
    * e
Branches_of_physics
                      * Theoretical
                            o Phenomenology
Divisions             * Computational
                      * Experimental
                      * Applied
                                            * Continuum
                  Classical_mechanics             o Solid
                                                  o Fluid
                                            * Acoustics
                                            * Electrostatics
                  Electrodynamics           * Magnetostatics
                                            * Plasma_physics
Classical                                   * Accelerator_physics
                                            * Thermodynamics
                                            * Condensed_matter
                                                  o Materials
                  Statistical mechanics           o Mesoscopic
                                                  o Polymers
                                                  o Soft
                                                  o Solid-state
                                          * Quantum_electrodynamics
                  Quantum_mechanics       * Quantum_field_theory
                                          * Quantum_gravity
                                          * Quantum_information
                  Relativity              * General
                                          * Special
                                          * Astroparticle
                  Particle_physics        * Nuclear
                                          * Quantum_chromodynamics
Modern                                    * Atomic_physics
                  Atomic,_molecular       * Molecular_physics
                  and_optical_physics     * Optics
                                          * Photonics
                                          * Quantum_optics
                                          * Astrophysics
                                                o Nuclear
                  Cosmology               * Celestial_mechanics
                                          * Solar
                                                o Heliophysics
                                          * Space_physics
                      * Agrophysics
                      * Biophysics
                            o Medical
                            o Neurophysics
                      * Engineering
                      * Geophysics
Interdisciplinary           o Atmospheric
                            o Cloud
                      * Mathematical
                      * Physical_chemistry
                            o Chemical_physics
                      * Quantum_computing
                      * Social_physics
                            o Econophysics
                      * History_of_physics
See also              * Nobel_Prize_in_Physics
                      * Timeline_of_physics_discoveries
                      * Theory_of_everything
                                              * BNE: XX524922
                                              * BNF: cb11958255n (data)
Authority_control [Edit_this_at_Wikidata]     * GND: 4056999-8
                                              * LCCN: sh85127571
                                              * NDL: 00573177
                                              * SUDOC: 027570711

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Statistical_mechanics&oldid=903045264"
Categories:
    * Concepts_in_physics
    * Physics
    * Statistical_mechanics
    * Thermodynamics
Hidden categories:
    * Articles_with_short_description
    * Use_British_English_Oxford_spelling_from_January_2019
    * Use_mdy_dates_from_January_2019
    * Commons_category_link_is_on_Wikidata
    * Wikipedia_articles_with_BNE_identifiers
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
    * Wikipedia_articles_with_SUDOC_identifiers
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
    * à¦à¦¸à¦®à§à¦¯à¦¼à¦¾
    * Asturianu
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * Gaeilge
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Latina
    * Magyar
    * à´®à´²à´¯à´¾à´³à´
    * à¤®à¤°à¤¾à¤ à¥
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * Sicilianu
    * Simple_English
    * SlovenÅ¡Äina
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
    * ä¸­æ
Edit_links
    * This page was last edited on 23 June 2019, at 04:27 (UTC).
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
