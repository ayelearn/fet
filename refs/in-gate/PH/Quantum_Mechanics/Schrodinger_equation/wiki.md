The following text has been accessed from https://en.wikipedia.org/wiki/Schr%C3%B6dinger_equation at Fri Aug 9 03:12:04 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** SchrÃ¶dinger equation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For a more general introduction to the topic, see Introduction_to_quantum
mechanics.
Linear partial differential equation whose solution describes the quantum-
mechanical system.
Part of a series on
Quantum_mechanics
   i &#x210F;   &#x2202;  &#x2202; t     |  &#x03C8; ( t ) &#x27E9; =    H
&#x005E;     |  &#x03C8; ( t ) &#x27E9;   {\displaystyle i\hbar {\frac
{\partial }{\partial t}}|\psi (t)\rangle ={\hat {H}}|\psi (t)\rangle }  [
{\displaystyle i\hbar {\frac {\partial }{\partial t}}|\psi (t)\rangle ={\hat
{H}}|\psi (t)\rangle }]
SchrÃ¶dinger equation
    * Introduction
    * Glossary
    * History
Background
    * Classical_mechanics
    * Old_quantum_theory
    * Braâket_notation
    * Hamiltonian
    * Interference
Fundamentals
    * Coherence
    * Decoherence
    * Complementarity
    * Energy_level
    * Entanglement
    * Hamiltonian
    * Uncertainty_principle
    * Ground_state
    * Interference
    * Measurement
    * Nonlocality
    * Observable
    * Operator
    * Quantum
    * Quantum_fluctuation
    * Quantum_foam
    * Quantum_levitation
    * Quantum_number
    * Quantum_noise
    * Quantum_realm
    * Quantum_state
    * Quantum_system
    * Quantum_teleportation
    * Qubit
    * Spin
    * Superposition
    * Symmetry
    * (Spontaneous)_symmetry_breaking
    * Vacuum_state
    * Wave_propagation
    * Wave_function
          o Wave_function_collapse
          o Waveâparticle_duality
          o Matter_wave
Effects
    * Zeeman_effect
    * Stark_effect
    * AharonovâBohm_effect
    * Landau_quantization
    * Quantum_Hall_effect
    * Quantum_Zeno_effect
    * Quantum_tunnelling
    * Photoelectric_effect
    * Casimir_effect
Experiments
    * Afshar
    * Bell's_inequality
    * DavissonâGermer
    * Double-slit
    * ElitzurâVaidman
    * FranckâHertz
    * LeggettâGarg_inequality
    * MachâZehnder
    * Popper
    * Quantum_eraser (delayed-choice)
    * SchrÃ¶dinger's_cat
    * Quantum_suicide_and_immortality
    * Stern–Gerlach
    * Wheeler's_delayed-choice
Formulations
    * Overview
    * Heisenberg
    * Interaction
    * Matrix
    * Phase-space
    * SchrÃ¶dinger
    * Sum-over-histories_(path-integral)
    * HellmannâFeynman_theorem
Equations
    * Dirac
    * KleinâGordon
    * Pauli
    * Rydberg
    * SchrÃ¶dinger
Interpretations
    * Overview
    * Consistent_histories
    * Copenhagen
    * de_BroglieâBohm
    * Ensemble
    * Hidden-variable
    * Many-worlds
    * Objective_collapse
    * Bayesian
    * Quantum_logic
    * Relational
    * Stochastic
    * Scale_relativity
    * Transactional
Advanced topics
    * Quantum_annealing
    * Quantum_chaos
    * Quantum_computing
    * Density_matrix
    * Quantum_field_theory
    * Fractional_quantum_mechanics
    * Quantum_gravity
    * Quantum_information_science
    * Quantum_machine_learning
    * Perturbation_theory_(quantum_mechanics)
    * Relativistic_quantum_mechanics
    * Scattering_theory
    * Spontaneous_parametric_down-conversion
    * Quantum_statistical_mechanics
Scientists
    * Aharonov
    * Bell
    * Blackett
    * Bloch
    * Bohm
    * Bohr
    * Born
    * Bose
    * de_Broglie
    * Candlin
    * Compton
    * Dirac
    * Davisson
    * Debye
    * Ehrenfest
    * Einstein
    * Everett
    * Fock
    * Fermi
    * Feynman
    * Glauber
    * Gutzwiller
    * Heisenberg
    * Hilbert
    * Jordan
    * Kramers
    * Pauli
    * Lamb
    * Landau
    * Laue
    * Moseley
    * Millikan
    * Onnes
    * Planck
    * Rabi
    * Raman
    * Rydberg
    * SchrÃ¶dinger
    * Sommerfeld
    * von_Neumann
    * Weyl
    * Wien
    * Wigner
    * Zeeman
    * Zeilinger
    * Goudsmit
    * Uhlenbeck
    * Yang
    * v
    * t
    * e
SchrÃ¶dinger's equation inscribed on the gravestone of Annemarie and Erwin
SchrÃ¶dinger. (Newton's dot notation for the time derivative is used.)
The SchrÃ¶dinger equation is a linear partial_differential_equation that
describes the wave_function or state function of a quantum-mechanical system.
[1]:1â2 It is a key result in quantum_mechanics, and its discovery was a
significant landmark in the development of the subject. The equation is named
after Erwin_SchrÃ¶dinger, who postulated the equation in 1925, and published it
in 1926, forming the basis for the work that resulted in his Nobel_Prize_in
Physics in 1933.[2][3]
In classical_mechanics, Newton's_second_law (F = ma)[note_1] is used to make a
mathematical prediction as to what path a given physical system will take over
time following a set of known initial conditions. Solving this equation gives
the position and the momentum of the physical system as a function of the
external force      F    {\displaystyle \mathbf {F} }  [\mathbf {F} ] on the
system. Those two parameters are sufficient to describe its state at each time
instant. In quantum mechanics, the analogue of Newton's law is SchrÃ¶dinger's
equation.
The concept of a wave function is a fundamental postulate_of_quantum_mechanics;
the wave function defines the state of the system at each spatial position, and
time. Using these postulates, SchrÃ¶dinger's equation can be derived from the
fact that the time-evolution operator must be unitary, and must therefore be
generated by the exponential of a self-adjoint_operator, which is the quantum
Hamiltonian. This derivation is explained below.
In the Copenhagen_interpretation of quantum mechanics, the wave function is the
most complete description that can be given of a physical system. Solutions to
SchrÃ¶dinger's equation describe not only molecular, atomic, and subatomic
systems, but also macroscopic_systems, possibly even the whole universe.[4]:
292ff SchrÃ¶dinger's equation is central to all applications of quantum
mechanics, including quantum_field_theory, which combines special_relativity
with quantum mechanics. Theories of quantum_gravity, such as string_theory,
also do not modify SchrÃ¶dinger's equation.[citation_needed]
The SchrÃ¶dinger equation is not the only way to study quantum mechanical
systems and make predictions. The other formulations of quantum mechanics
include matrix_mechanics, introduced by Werner_Heisenberg, and the path
integral_formulation, developed chiefly by Richard_Feynman. Paul_Dirac
incorporated matrix mechanics and the SchrÃ¶dinger equation into a single
formulation.
⁰
***** Contents *****
    * 1_Equation
          o 1.1_Time-dependent_equation
          o 1.2_Time-independent_equation
    * 2_Derivation
    * 3_Implications
          o 3.1_Energy
          o 3.2_Quantization
          o 3.3_Quantum_tunneling
          o 3.4_Particles_as_waves
                # 3.4.1_Measurement_and_uncertainty
    * 4_Interpretation_of_the_wave_function
    * 5_Historical_background_and_development
    * 6_The_wave_equation_for_particles
          o 6.1_Consistency_with_energy_conservation
          o 6.2_Linearity
          o 6.3_Consistency_with_the_de_Broglie_relations
          o 6.4_Wave_and_particle_motion
    * 7_Nonrelativistic_quantum_mechanics
          o 7.1_Time-independent
          o 7.2_One-dimensional_examples
                # 7.2.1_Free_particle
                # 7.2.2_Constant_potential
                # 7.2.3_Harmonic_oscillator
          o 7.3_Three-dimensional_examples
                # 7.3.1_Hydrogen_atom
                # 7.3.2_Two-electron_atoms_or_ions
          o 7.4_Time-dependent
    * 8_Solution_methods
    * 9_Properties
          o 9.1_Linearity
          o 9.2_Momentum_space_SchrÃ¶dinger_equation
          o 9.3_Real_energy_eigenstates
          o 9.4_Space_and_time_derivatives
          o 9.5_Local_conservation_of_probability
          o 9.6_Positive_energy
          o 9.7_Analytic_continuation_to_diffusion
          o 9.8_Regularity
    * 10_Relativistic_quantum_mechanics
    * 11_Quantum_field_theory
    * 12_First_order_form
    * 13_See_also
    * 14_Notes
    * 15_References
    * 16_Further_reading
    * 17_External_links
***** Equation[edit] *****
**** Time-dependent equation[edit] ****
The form of the SchrÃ¶dinger equation depends on the physical situation (see
below for special cases). The most general form is the time-dependent
SchrÃ¶dinger equation (TDSE), which gives a description of a system evolving
with time:[5]:143
A wave_function that satisfies the nonrelativistic SchrÃ¶dinger equation with V
= 0. In other words, this corresponds to a particle traveling freely through
empty space. The real_part of the wave_function is plotted here.
Time-dependent SchrÃ¶dinger equation (general)
   i &#x210F;   d  d t    | &#x03A8; ( t ) &#x27E9; =    H &#x005E;    |
&#x03A8; ( t ) &#x27E9;   {\displaystyle i\hbar {\frac {d}{dt}}\vert \Psi
(t)\rangle ={\hat {H}}\vert \Psi (t)\rangle }  [{\displaystyle i\hbar {\frac
{d}{dt}}\vert \Psi (t)\rangle ={\hat {H}}\vert \Psi (t)\rangle }]
where     i   {\displaystyle i}  [i] is the imaginary_unit,     &#x210F; =   h
2 &#x03C0;      {\displaystyle \hbar ={\frac {h}{2\pi }}}  [\hbar ={\frac  {h}
{2\pi }}] is the reduced Planck_constant,     &#x03A8;   {\displaystyle \Psi }
[\Psi ] (the Greek letter psi) is the state vector of the quantum system,     t
{\displaystyle t}  [t] is time, and        H &#x005E;      {\displaystyle {\hat
{H}}}  [{\hat {H}}] is the Hamiltonian operator. The position-space_wave
function of the quantum system is nothing but the components in the expansion
of the state vector in terms of the position eigenvector     |  r  &#x27E9;
{\displaystyle \vert \mathbf {r} \rangle }  [{\displaystyle \vert \mathbf {r}
\rangle }]. It is a scalar function, expressed as     &#x03A8; (  r  , t ) =
&#x27E8;  r  | &#x03A8; &#x27E9;   {\displaystyle \Psi (\mathbf {r} ,t)=\langle
\mathbf {r} \vert \Psi \rangle }  [{\displaystyle \Psi (\mathbf {r} ,t)=\langle
\mathbf {r} \vert \Psi \rangle }]. Similarly, the momentum-space_wave_function
can be defined as        &#x03A8; &#x007E;    (  p  , t ) = &#x27E8;  p  |
&#x03A8; &#x27E9;   {\displaystyle {\tilde {\Psi }}(\mathbf {p} ,t)=\langle
\mathbf {p} \vert \Psi \rangle }  [{\displaystyle {\tilde {\Psi }}(\mathbf {p}
,t)=\langle \mathbf {p} \vert \Psi \rangle }], where     |  p  &#x27E9;
{\displaystyle \vert \mathbf {p} \rangle }  [{\displaystyle \vert \mathbf {p}
\rangle }] is the momentum eigenvector.
Each of these three rows is a wave function which satisfies the time-dependent
SchrÃ¶dinger equation for a harmonic_oscillator. Left: The real part (blue) and
imaginary part (red) of the wave function. Right: The probability_distribution
of finding the particle with this wave function at a given position. The top
two rows are examples of stationary_states, which correspond to standing_waves.
The bottom row is an example of a state which is not a stationary state. The
right column illustrates why stationary states are called "stationary".
The most famous example is the nonrelativistic SchrÃ¶dinger equation for the
wave function in position space     &#x03A8; (  r  , t )   {\displaystyle \Psi
(\mathbf {r} ,t)}  [\Psi (\mathbf {r} ,t)] of a single particle subject to a
potential     V (  r  , t )   {\displaystyle V(\mathbf {r} ,t)}  [
{\displaystyle V(\mathbf {r} ,t)}], such as that due to an electric_field.[6]
[note_2]
Time-dependent SchrÃ¶dinger equation in position basis
(single nonrelativistic particle)
   i &#x210F;   &#x2202;  &#x2202; t    &#x03A8; (  r  , t ) =  [     &#x2212;
&#x210F;  2     2 m     &#x2207;  2   + V (  r  , t )  ]  &#x03A8; (  r  , t )
{\displaystyle i\hbar {\frac {\partial }{\partial t}}\Psi (\mathbf {r}
,t)=\left[{\frac {-\hbar ^{2}}{2m}}\nabla ^{2}+V(\mathbf {r} ,t)\right]\Psi
(\mathbf {r} ,t)}  [{\displaystyle i\hbar {\frac {\partial }{\partial t}}\Psi
(\mathbf {r} ,t)=\left[{\frac {-\hbar ^{2}}{2m}}\nabla ^{2}+V(\mathbf {r}
,t)\right]\Psi (\mathbf {r} ,t)}]
where     m   {\displaystyle m}  [m] is the particle's mass, and      &#x2207;
2     {\displaystyle \nabla ^{2}}  [\nabla ^{2}] is the Laplacian.
This is also a diffusion_equation, but unlike the heat_equation, this one is
also a wave equation given the imaginary_unit present in the transient term.
The term "SchrÃ¶dinger equation" can refer to both the general equation, or the
specific nonrelativistic version. The general equation is indeed quite general,
used throughout quantum mechanics, for everything from the Dirac_equation to
quantum_field_theory, by plugging in diverse expressions for the Hamiltonian.
The specific nonrelativistic version is a strictly classical approximation to
reality and yields accurate results in many situations, but only to a certain
extent (see relativistic_quantum_mechanics and relativistic_quantum_field
theory).
To apply the SchrÃ¶dinger equation, write down the Hamiltonian for the system,
accounting for the kinetic and potential energies of the particles constituting
the system, then insert it into the SchrÃ¶dinger equation. The resulting
partial differential equation is solved for the wave function, which contains
information about the system.
**** Time-independent equation[edit] ****
The time-dependent SchrÃ¶dinger equation described above predicts that wave
functions can form standing_waves, called stationary_states.[note_3] These
states are particularly important as their individual study later simplifies
the task of solving the time-dependent SchrÃ¶dinger equation for any state.
Stationary states can also be described by a simpler form of the SchrÃ¶dinger
equation, the time-independent SchrÃ¶dinger equation (TISE).
Time-independent SchrÃ¶dinger equation (general)
      H &#x005E;    &#x2061;  |  &#x03A8; &#x27E9; = E  |  &#x03A8; &#x27E9;
{\displaystyle \operatorname {\hat {H}} |\Psi \rangle =E|\Psi \rangle }  [
{\displaystyle \operatorname {\hat {H}} |\Psi \rangle =E|\Psi \rangle }]
where     E   {\displaystyle E}  [E] is a constant equal to the energy level of
the system. This is only used when the Hamiltonian itself is not dependent on
time explicitly. However, even in this case the total wave function still has a
time dependency.
In the language of linear_algebra, this equation is an eigenvalue_equation.
Therefore, the wave function is an eigenfunction of the Hamiltonian operator
with corresponding eigenvalue(s)     E   {\displaystyle E}  [E].
As before, the most common manifestation is the nonrelativistic SchrÃ¶dinger
equation for a single particle moving in an electric field (but not a magnetic
field):
Time-independent SchrÃ¶dinger equation (single nonrelativistic particle)
    [     &#x2212;  &#x210F;  2     2 m     &#x2207;  2   + V (  r  )  ]
&#x03A8; (  r  ) = E &#x03A8; (  r  )   {\displaystyle \left[{\frac {-\hbar ^
{2}}{2m}}\nabla ^{2}+V(\mathbf {r} )\right]\Psi (\mathbf {r} )=E\Psi (\mathbf
{r} )}  [{\displaystyle \left[{\frac {-\hbar ^{2}}{2m}}\nabla ^{2}+V(\mathbf
{r} )\right]\Psi (\mathbf {r} )=E\Psi (\mathbf {r} )}]
with definitions as above. Here, the form of the Hamiltonian operator comes
from classical mechanics, where the Hamiltonian function is the sum of the
kinetic and potential energies. That is,     H = T + V =     |   |   p   |    |
2     2 m    + V ( x , y , z )   {\displaystyle H=T+V={\frac {||\mathbf {p} ||^
{2}}{2m}}+V(x,y,z)}  [{\displaystyle H=T+V={\frac {||\mathbf {p} ||^{2}}{2m}}+V
(x,y,z)}] for a single particle in the non-relativistic limit.
The time-independent SchrÃ¶dinger equation is discussed further below.
***** Derivation[edit] *****
By assuming the Dirac-von_Neumann_axioms, a modern approach to understanding
the Schrödinger equation is outlined as follows. Suppose the wave_function
&#x03C8; (  t  0   )   {\displaystyle \psi (t_{0})}  [{\displaystyle \psi (t_
{0})}] represents a unit vector defined on a complex Hilbert_space at some
initial time      t  0     {\displaystyle t_{0}}  [t_{0}]. The unitarity
principle requires that there must exist a linear operator,        U &#x005E;
( t )   {\displaystyle {\hat {U}}(t)}  [{\displaystyle {\hat {U}}(t)}], such
that for any time     t >  t  0     {\displaystyle t>t_{0}}  [{\displaystyle
t>t_{0}}],
         &#x03C8; ( t ) =    U &#x005E;    ( t ) &#x03C8; (  t  0   )    
      .   {\displaystyle \psi (t)={\hat {U}}(t)\psi (t_{0}).}  [           (1)
      {\displaystyle \psi (t)={\hat {U}}(t)\psi (t_{0}).}]
Given that     &#x03C8; ( t )   {\displaystyle \psi (t)}  [\psi(t)] must remain
a unit vector, the operator        U &#x005E;    ( t )   {\displaystyle {\hat
{U}}(t)}  [{\displaystyle {\hat {U}}(t)}] must therefore be a unitary
transformation. As such, there exists an exponential_map such that        U
&#x005E;    ( t ) =  e  &#x2212;   i &#x210F;       H  &#x005E;    t
{\displaystyle {\hat {U}}(t)=e^{-{\frac {i}{\hbar }}{\hat {\mathcal {H}}}t}}  [
{\displaystyle {\hat {U}}(t)=e^{-{\frac {i}{\hbar }}{\hat {\mathcal {H}}}t}}]
where         H  &#x005E;      {\displaystyle {\hat {\mathcal {H}}}}  [
{\displaystyle {\hat {\mathcal {H}}}}] is a Hermitian_operator (given by the
fact that the Lie_algebra of the unitary_group is generated by Hermitian
operators). Therefore, the first-order Taylor expansion of        U &#x005E;
( t )   {\displaystyle {\hat {U}}(t)}  [{\displaystyle {\hat {U}}(t)}] centered
at      t  0     {\displaystyle t_{0}}  [t_{0}] takes the form
            U &#x005E;    ( t ) &#x2248; 1 &#x2212;   i &#x210F;   ( t &#x2212;
      t  0   )     H  &#x005E;    .   {\displaystyle {\hat {U}}(t)\approx 1-
      {\frac {i}{\hbar }}(t-t_{0}){\hat {\mathcal {H}}}.}  [{\displaystyle
      {\hat {U}}(t)\approx 1-{\frac {i}{\hbar }}(t-t_{0}){\hat {\mathcal
      {H}}}.}]
And so, substituting the above expansion into (1) thus yields
         &#x03C8; ( t ) = &#x03C8; (  t  0   ) &#x2212;   i &#x210F;   ( t
      &#x2212;  t  0   )     H  &#x005E;    &#x03C8; (  t  0   ) ,
      {\displaystyle \psi (t)=\psi (t_{0})-{\frac {i}{\hbar }}(t-t_{0}){\hat
      {\mathcal {H}}}\psi (t_{0}),}  [{\displaystyle \psi (t)=\psi (t_{0})-
      {\frac {i}{\hbar }}(t-t_{0}){\hat {\mathcal {H}}}\psi (t_{0}),}]
which, when rearranged and taken in the limit     t &#x2192;  t  0
{\displaystyle t\rightarrow t_{0}}  [{\displaystyle t\rightarrow t_{0}}],
provides an equation of the same form as the Schrödinger equation
         i &#x210F;    d &#x03C8;   d t    =     H  &#x005E;    &#x03C8; ,
      {\displaystyle i\hbar {\frac {d\psi }{dt}}={\hat {\mathcal {H}}}\psi ,}
      [{\displaystyle i\hbar {\frac {d\psi }{dt}}={\hat {\mathcal {H}}}\psi ,}]
where the ordinary definition for the derivative was used. However, the
operator         H  &#x005E;      {\displaystyle {\hat {\mathcal {H}}}}  [
{\displaystyle {\hat {\mathcal {H}}}}] used here denotes an arbitrary Hermitian
operator. Nonetheless, by using the correspondence_principle it is possible to
show that, in the classical limit and using appropriate units, the expectation
value of         H  &#x005E;      {\displaystyle {\hat {\mathcal {H}}}}  [
{\displaystyle {\hat {\mathcal {H}}}}] indeed corresponds to the Hamiltonian of
the system, that is,     &#x27E8;     H  &#x005E;    &#x27E9; =   H
{\displaystyle \langle {\hat {\mathcal {H}}}\rangle ={\mathcal {H}}}  [
{\displaystyle \langle {\hat {\mathcal {H}}}\rangle ={\mathcal {H}}}].[7]
***** Implications[edit] *****
**** Energy[edit] ****
The Hamiltonian is constructed in the same manner as in classical mechanics.
However, in classical mechanics, the Hamiltonian is a scalar-valued function,
whereas in quantum mechanics, it is an operator on a space of functions. It is
not surprising that the eigenvalues of        H &#x005E;      {\displaystyle
{\hat {H}}}  [{\hat {H}}] are the energy levels of the system.
**** Quantization[edit] ****
The SchrÃ¶dinger equation predicts that if certain properties of a system are
measured, the result may be quantized, meaning that only specific discrete
values can occur. One example is energy quantization: the energy of an electron
in an atom is always one of the quantized_energy_levels, a fact discovered via
atomic_spectroscopy. (Energy quantization is discussed below.) Another example
is quantization_of_angular_momentum. This was an assumption in the earlier Bohr
model_of_the_atom, but it is a prediction of the SchrÃ¶dinger equation.
Another result of the SchrÃ¶dinger equation is that not every measurement gives
a quantized result in quantum mechanics. For example, position, momentum, time,
and (in some situations) energy can have any value across a continuous range.
[8]:165â167
**** Quantum tunneling[edit] ****
Main article: Quantum_tunneling
Quantum_tunneling through a barrier. A particle coming from the left does not
have enough energy to climb the barrier. However, it can sometimes "tunnel" to
the other side.
In classical physics, when a ball is rolled slowly up a large hill, it will
come to a stop and roll back, because it doesn't have enough energy to get over
the top of the hill to the other side. However, the SchrÃ¶dinger equation
predicts that there is a small probability that the ball will get to the other
side of the hill, even if it has too little energy to reach the top. This is
called quantum_tunneling. It is related to the distribution of energy: although
the ball's assumed position seems to be on one side of the hill, there is a
chance of finding it on the other side.
**** Particles as waves[edit] ****
Main articles: Matter_wave, Waveâparticle_duality, and Double-slit_experiment
A double slit experiment showing the accumulation of electrons on a screen as
time passes.
The nonrelativistic SchrÃ¶dinger equation is a type of partial_differential
equation called a wave_equation. Therefore, it is often said particles can
exhibit behavior usually attributed to waves. In some modern interpretations
this description is reversed â the quantum state, i.e. wave, is the only
genuine physical reality, and under the appropriate conditions it can show
features of particle-like behavior. However, Ballentine[9]:Chapter 4, p.99
shows that such an interpretation has problems. Ballentine points out that
whilst it is arguable to associate a physical wave with a single particle,
there is still only one SchrÃ¶dinger wave equation for many particles. He
points out:
      "If a physical wave field were associated with a particle, or if a
      particle were identified with a wave packet, then corresponding to N
      interacting particles there should be N interacting waves in ordinary
      three-dimensional space. But according to (4.6) that is not the case;
      instead there is one "wave" function in an abstract 3N-dimensional
      configuration space. The misinterpretation of psi as a physical wave in
      ordinary space is possible only because the most common applications of
      quantum mechanics are to one-particle states, for which configuration
      space and ordinary space are isomorphic."
Two-slit_diffraction is a famous example of the strange behaviors that waves
regularly display, that are not intuitively associated with particles. The
overlapping waves from the two slits cancel each other out in some locations,
and reinforce each other in other locations, causing a complex pattern to
emerge. Intuitively, one would not expect this pattern from firing a single
particle at the slits, because the particle should pass through one slit or the
other, not a complex overlap of both.
However, since the SchrÃ¶dinger equation is a wave_equation, a single particle
fired through a double-slit does show this same pattern (figure on right). The
experiment must be repeated many times for the complex pattern to emerge.
Although this is counterintuitive, the prediction is correct; in particular,
electron_diffraction and neutron_diffraction are well understood and widely
used in science and engineering.
Related to diffraction, particles also display superposition and interference.
The superposition property allows the particle to be in a quantum_superposition
of two or more quantum states at the same time. However, a "quantum state" in
quantum mechanics means the probability that a system will be, for example at a
position x, not that the system will actually be at position x. It does not
imply that the particle itself may be in two classical states at once. Indeed,
quantum mechanics is generally unable to assign values for properties prior to
measurement at all.
*** Measurement and uncertainty[edit] ***
Main articles: Measurement_in_quantum_mechanics, Heisenberg_uncertainty
principle, and Interpretations_of_quantum_mechanics
In classical mechanics, a particle has, at every moment, an exact position and
an exact momentum. These values change deterministically as the particle moves
according to Newton's_laws. Under the Copenhagen_interpretation of quantum
mechanics, particles do not have exactly determined properties, and when they
are measured, the result is randomly drawn from a probability_distribution. The
SchrÃ¶dinger equation predicts what the probability distributions are, but
fundamentally cannot predict the exact result of each measurement.
The Heisenberg_uncertainty_principle is one statement of the inherent
measurement uncertainty in quantum mechanics. It states that the more precisely
a particle's position is known, the less precisely its momentum is known, and
vice versa.
The SchrÃ¶dinger equation describes the (deterministic) evolution of the wave
function of a particle. However, even if the wave function is known exactly,
the result of a specific measurement on the wave function is uncertain.
***** Interpretation of the wave function[edit] *****
Main article: Interpretations_of_quantum_mechanics
The SchrÃ¶dinger equation provides a way to calculate the wave function of a
system and how it changes dynamically in time. However, the SchrÃ¶dinger
equation does not directly say what, exactly, the wave function is.
Interpretations_of_quantum_mechanics address questions such as what the
relation is between the wave function, the underlying reality, and the results
of experimental measurements.
An important aspect is the relationship between the SchrÃ¶dinger equation and
wave_function_collapse. In the oldest Copenhagen_interpretation, particles
follow the SchrÃ¶dinger equation except during wave function collapse, during
which they behave entirely differently. The advent of quantum_decoherence
theory allowed alternative approaches (such as the Everett_many-worlds
interpretation and consistent_histories), wherein the SchrÃ¶dinger equation is
always satisfied, and wave function collapse should be explained as a
consequence of the SchrÃ¶dinger equation.
In 1952, Erwin_SchrÃ¶dinger gave a lecture during which he commented,
      Nearly every result [a quantum theorist] pronounces is about the
      probability of this or that or that ... happeningâwith usually a great
      many alternatives. The idea that they be not alternatives but all really
      happen simultaneously seems lunatic to him, just impossible.[10]
David_Deutsch regarded this as the earliest known reference to a many-worlds
interpretation of quantum mechanics, an interpretation generally credited to
Hugh_Everett_III,[11] while Jeffrey_A._Barrett took the more modest position
that it indicates a "similarity in ... general views" between SchrÃ¶dinger and
Everett.[12]
***** Historical background and development[edit] *****
Erwin_SchrÃ¶dinger
Main article: Theoretical_and_experimental_justification_for_the_SchrÃ¶dinger
equation
Following Max_Planck's quantization of light (see black-body_radiation), Albert
Einstein interpreted Planck's quanta to be photons, particles_of_light, and
proposed that the energy_of_a_photon_is_proportional_to_its_frequency, one of
the first signs of waveâparticle_duality. Since energy and momentum are
related in the same way as frequency and wave_number in special_relativity, it
followed that the momentum     p   {\displaystyle p}  [p] of a photon is
inversely proportional to its wavelength     &#x03BB;   {\displaystyle \lambda
}  [\lambda ], or proportional to its wave number     k   {\displaystyle k}
[k]:
         p =   h &#x03BB;   = &#x210F; k ,   {\displaystyle p={\frac {h}
      {\lambda }}=\hbar k,}  [{\displaystyle p={\frac {h}{\lambda }}=\hbar k,}]
where     h   {\displaystyle h}  [h] is Planck's_constant and     &#x210F; =  h
/   2 &#x03C0;    {\displaystyle \hbar ={h}/{2\pi }}  [{\displaystyle \hbar =
{h}/{2\pi }}] is the reduced Planck constant (or the Dirac constant). Louis_de
Broglie hypothesized that this is true for all particles, even particles which
have mass such as electrons. He showed that, assuming that the matter waves
propagate along with their particle counterparts, electrons form standing
waves, meaning that only certain discrete rotational frequencies about the
nucleus of an atom are allowed.[13] These quantized orbits correspond to
discrete energy_levels, and de Broglie reproduced the Bohr_model formula for
the energy levels. The Bohr model was based on the assumed quantization of
angular momentum     L   {\displaystyle L}  [L] according to:
         L = n   h  2 &#x03C0;    = n &#x210F; .   {\displaystyle L=n{h \over
      2\pi }=n\hbar .}  [L=n{h \over 2\pi }=n\hbar .]
According to de Broglie the electron is described by a wave and a whole number
of wavelengths must fit along the circumference of the electron's orbit:
         n &#x03BB; = 2 &#x03C0; r .    {\displaystyle n\lambda =2\pi r.\,}
      [n\lambda =2\pi r.\,]
This approach essentially confined the electron wave in one dimension, along a
circular orbit of radius     r   {\displaystyle r}  [r].
In 1921, prior to de Broglie, Arthur C. Lunn at the University of Chicago had
used the same argument based on the completion of the relativistic
energyâmomentum 4-vector to derive what we now call the de Broglie relation.
[14] Unlike de Broglie, Lunn went on to formulate the differential equation now
known as the SchrÃ¶dinger equation, and solve for its energy eigenvalues for
the hydrogen atom. Unfortunately the paper was rejected by the Physical Review,
as recounted by Kamen.[15]
Following up on de Broglie's ideas, physicist Peter_Debye made an offhand
comment that if particles behaved as waves, they should satisfy some sort of
wave equation. Inspired by Debye's remark, SchrÃ¶dinger decided to find a
proper 3-dimensional wave equation for the electron. He was guided by William
R._Hamilton's analogy between mechanics and optics, encoded in the observation
that the zero-wavelength limit of optics resembles a mechanical systemâthe
trajectories of light_rays become sharp tracks that obey Fermat's_principle, an
analog of the principle_of_least_action.[16] A modern version of his reasoning
is reproduced below. The equation he found is:[17]
         i &#x210F;   &#x2202;  &#x2202; t    &#x03A8; (  r  ,  t ) = &#x2212;
      &#x210F;  2    2 m     &#x2207;  2   &#x03A8; (  r  ,  t ) + V (  r  )
      &#x03A8; (  r  ,  t ) .   {\displaystyle i\hbar {\frac {\partial }
      {\partial t}}\Psi (\mathbf {r} ,\,t)=-{\frac {\hbar ^{2}}{2m}}\nabla ^
      {2}\Psi (\mathbf {r} ,\,t)+V(\mathbf {r} )\Psi (\mathbf {r} ,\,t).}
      [i\hbar {\frac {\partial }{\partial t}}\Psi (\mathbf {r} ,\,t)=-{\frac
      {\hbar ^{2}}{2m}}\nabla ^{2}\Psi (\mathbf {r} ,\,t)+V(\mathbf {r} )\Psi
      (\mathbf {r} ,\,t).]
However, by that time, Arnold_Sommerfeld had refined_the_Bohr_model with
relativistic_corrections.[18][19] SchrÃ¶dinger used the relativistic energy
momentum relation to find what is now known as the KleinâGordon_equation in a
Coulomb_potential (in natural_units):
           (  E +    e  2   r    )   2   &#x03C8; ( x ) = &#x2212;  &#x2207;  2
      &#x03C8; ( x ) +  m  2   &#x03C8; ( x ) .   {\displaystyle \left(E+{e^{2}
      \over r}\right)^{2}\psi (x)=-\nabla ^{2}\psi (x)+m^{2}\psi (x).}  [\left
      (E+{e^{2} \over r}\right)^{2}\psi (x)=-\nabla ^{2}\psi (x)+m^{2}\psi
      (x).]
He found the standing waves of this relativistic equation, but the relativistic
corrections disagreed with Sommerfeld's formula. Discouraged, he put away his
calculations and secluded himself in an isolated mountain cabin in December
1925.[20][failed_verification]
While at the cabin, SchrÃ¶dinger decided that his earlier nonrelativistic
calculations were novel enough to publish, and decided to leave off the problem
of relativistic corrections for the future. Despite the difficulties in solving
the differential equation for hydrogen (he had sought help from his friend the
mathematician Hermann_Weyl[21]:3) SchrÃ¶dinger showed that his nonrelativistic
version of the wave equation produced the correct spectral energies of hydrogen
in a paper published in 1926.[21]:1[22] In the equation, SchrÃ¶dinger computed
the hydrogen_spectral_series by treating a hydrogen_atom's electron as a wave
&#x03A8; (  x  , t )   {\displaystyle \Psi (\mathbf {x} ,t)}  [{\displaystyle
\Psi (\mathbf {x} ,t)}], moving in a potential_well     V   {\displaystyle V}
[V], created by the proton. This computation accurately reproduced the energy
levels of the Bohr_model. In a paper, SchrÃ¶dinger himself explained this
equation as follows:
    The already ... mentioned psi-function.... is now the means for
âpredicting probability of measurement results. In it is embodied the â
    momentarily attained sum of theoretically based future expectation,
    somewhat as laid down in a catalog.
â Erwin SchrÃ¶dinger[23]
This 1926 paper was enthusiastically endorsed by Einstein, who saw the matter-
waves as an intuitive depiction of nature, as opposed to Heisenberg's matrix
mechanics, which he considered overly formal.[24]
The SchrÃ¶dinger equation details the behavior of     &#x03A8;   {\displaystyle
\Psi }  [\Psi ] but says nothing of its nature. SchrÃ¶dinger tried to interpret
it as a charge density in his fourth paper, but he was unsuccessful.[25]:219 In
1926, just a few days after SchrÃ¶dinger's fourth and final paper was
published, Max_Born successfully interpreted     &#x03A8;   {\displaystyle \Psi
}  [\Psi ] as the probability_amplitude, whose modulus squared is equal to
probability_density.[25]:220 SchrÃ¶dinger, though, always opposed a statistical
or probabilistic approach, with its associated discontinuitiesâmuch like
Einstein, who believed that quantum mechanics was a statistical approximation
to an underlying deterministic_theoryâand never reconciled with the
Copenhagen_interpretation.[26]
Louis de Broglie in his later years proposed a real valued wave_function
connected to the complex wave function by a proportionality constant and
developed the De_BroglieâBohm_theory.
***** The wave equation for particles[edit] *****
Main article: Waveâparticle_duality
The SchrÃ¶dinger equation is a variation on the diffusion_equation where the
diffusion constant is imaginary. A spike of heat will decay in amplitude and
spread out; however, because the imaginary i is the generator of rotations in
the complex plane, a spike in the amplitude of a matter wave will also rotate
in the complex plane over time. The solutions are therefore functions which
describe wave-like motions. Wave equations in physics can normally be derived
from other physical laws â the wave equation for mechanical_vibrations on
strings and in matter can be derived from Newton's_laws, where the wave
function represents the displacement of matter, and electromagnetic_waves from
Maxwell's_equations, where the wave functions are electric and magnetic fields.
The basis for SchrÃ¶dinger's equation, on the other hand, is the energy of the
system and a separate postulate_of_quantum_mechanics: the wave function is a
description of the system.[27] The SchrÃ¶dinger equation is therefore a new
concept in itself; as Feynman put it:
âWhere did we get that (equation) from? Nowhere. It is not possible to derive â
    it from anything you know. It came out of the mind of SchrÃ¶dinger.
â Richard Feynman[28]
The foundation of the equation is structured to be a linear differential
equation based on classical energy conservation, and consistent with the De
Broglie relations. The solution is the wave function Ï, which contains all the
information that can be known about the system. In the Copenhagen
interpretation, the modulus of Ï is related to the probability the particles
are in some spatial configuration at some instant of time. Solving the equation
for Ï can be used to predict how the particles will behave under the influence
of the specified potential and with each other.
The SchrÃ¶dinger equation was developed principally from the De_Broglie
hypothesis, a wave equation that would describe particles,[29] and can be
constructed as shown informally in the following sections.[30] For a more
rigorous description of SchrÃ¶dinger's equation, see also Resnick et al.[31]
**** Consistency with energy conservation[edit] ****
The total energy E of a particle is the sum of kinetic energy     T
{\displaystyle T}  [T] and potential energy     V   {\displaystyle V}  [V],
this sum is also the frequent expression for the Hamiltonian     H
{\displaystyle H}  [H] in classical mechanics:
         E = T + V = H     {\displaystyle E=T+V=H\,\!}  [E=T+V=H\,\!]
Explicitly, for a particle in one dimension with position     x
{\displaystyle x}  [x], mass     m   {\displaystyle m}  [m] and momentum     p
{\displaystyle p}  [p], and potential energy     V   {\displaystyle V}  [V]
which generally varies_with_position and time     t   {\displaystyle t}  [t]:
         E =    p  2    2 m    + V ( x , t ) = H .   {\displaystyle E={\frac
      {p^{2}}{2m}}+V(x,t)=H.}  [E={\frac {p^{2}}{2m}}+V(x,t)=H.]
For three dimensions, the position_vector r and momentum vector p must be used:
         E =     p  &#x22C5;  p    2 m    + V (  r  , t ) = H   {\displaystyle
      E={\frac {\mathbf {p} \cdot \mathbf {p} }{2m}}+V(\mathbf {r} ,t)=H}  [E=
      {\frac {\mathbf {p} \cdot \mathbf {p} }{2m}}+V(\mathbf {r} ,t)=H]
This formalism can be extended to any fixed number of particles: the total
energy of the system is then the total kinetic energies of the particles, plus
the total potential energy, again the Hamiltonian. However, there can be
interactions between the particles (an N-body_problem), so the potential energy
V can change as the spatial configuration of particles changes, and possibly
with time. The potential energy, in general, is not the sum of the separate
potential energies for each particle, it is a function of all the spatial
positions of the particles. Explicitly:
         E =  &#x2211;  n = 1   N        p   n   &#x22C5;   p   n     2  m  n
      + V (   r   1   ,   r   2   &#x22EF;   r   N   , t ) = H
      {\displaystyle E=\sum _{n=1}^{N}{\frac {\mathbf {p} _{n}\cdot \mathbf {p}
      _{n}}{2m_{n}}}+V(\mathbf {r} _{1},\mathbf {r} _{2}\cdots \mathbf {r} _
      {N},t)=H\,\!}  [E=\sum _{n=1}^{N}{\frac {\mathbf {p} _{n}\cdot \mathbf
      {p} _{n}}{2m_{n}}}+V(\mathbf {r} _{1},\mathbf {r} _{2}\cdots \mathbf {r}
      _{N},t)=H\,\!]
**** Linearity[edit] ****
The simplest wave function is a plane_wave of the form:
         &#x03A8; (  r  , t ) = A  e  i (  k  &#x22C5;  r  &#x2212; &#x03C9; t
      )     {\displaystyle \Psi (\mathbf {r} ,t)=Ae^{i(\mathbf {k} \cdot
      \mathbf {r} -\omega t)}}  [{\displaystyle \Psi (\mathbf {r} ,t)=Ae^{i
      (\mathbf {k} \cdot \mathbf {r} -\omega t)}}]
where the A is the amplitude, k the wave vector, and     &#x03C9;
{\displaystyle \omega }  [\omega ] the angular frequency, of the plane wave. In
general, physical situations are not purely described by plane waves, so for
generality the superposition_principle is required; any wave can be made by
superposition of sinusoidal plane waves. So if the equation is linear, a linear
combination of plane waves is also an allowed solution. Hence a necessary and
separate requirement is that the SchrÃ¶dinger equation is a linear_differential
equation.
For discrete      k    {\displaystyle \mathbf {k} }  [\mathbf {k} ] the sum is
a superposition of plane waves:
         &#x03A8; (  r  , t ) =  &#x2211;  n = 1   &#x221E;    A  n    e  i
      (   k   n   &#x22C5;  r  &#x2212;  &#x03C9;  n   t )       {\displaystyle
      \Psi (\mathbf {r} ,t)=\sum _{n=1}^{\infty }A_{n}e^{i(\mathbf {k} _
      {n}\cdot \mathbf {r} -\omega _{n}t)}\,\!}  [\Psi (\mathbf {r} ,t)=\sum _
      {n=1}^{\infty }A_{n}e^{i(\mathbf {k} _{n}\cdot \mathbf {r} -\omega _
      {n}t)}\,\!]
for some real amplitude coefficients      A  n     {\displaystyle A_{n}}  [A_
{n}], and for continuous      k    {\displaystyle \mathbf {k} }  [\mathbf {k} ]
the sum becomes an integral, the Fourier_transform of a momentum space wave
function:[32]
         &#x03A8; (  r  , t ) =   1  (   2 &#x03C0;    )  3      &#x222B;
      &#x03A6; (  k  )  e  i (  k  &#x22C5;  r  &#x2212; &#x03C9; t )    d  3
      k      {\displaystyle \Psi (\mathbf {r} ,t)={\frac {1}{({\sqrt {2\pi }})^
      {3}}}\int \Phi (\mathbf {k} )e^{i(\mathbf {k} \cdot \mathbf {r} -\omega
      t)}d^{3}\mathbf {k} \,\!}  [\Psi (\mathbf {r} ,t)={\frac {1}{({\sqrt
      {2\pi }})^{3}}}\int \Phi (\mathbf {k} )e^{i(\mathbf {k} \cdot \mathbf {r}
      -\omega t)}d^{3}\mathbf {k} \,\!]
where      d  3    k  = d  k  x   d  k  x   d  k  z     {\displaystyle d^
{3}\mathbf {k} =dk_{x}dk_{x}dk_{z}}  [{\displaystyle d^{3}\mathbf {k} =dk_
{x}dk_{x}dk_{z}}]is the differential volume element in k-space, and the
integrals are taken over all      k    {\displaystyle \mathbf {k} }  [\mathbf
{k} ]-space. The momentum wave function     &#x03A6; (  k  )   {\displaystyle
\Phi (\mathbf {k} )}  [{\displaystyle \Phi (\mathbf {k} )}] arises in the
integrand since the position and momentum space wave functions are Fourier
transforms of each other.
**** Consistency with the de Broglie relations[edit] ****
Diagrammatic summary of the quantities related to the wave function, as used in
De broglie's hypothesis and development of the SchrÃ¶dinger equation.[29]
Einstein's_light_quanta_hypothesis (1905) states that the energy E of a quantum
of light or photon is proportional to its frequency     &#x03BD;
{\displaystyle \nu }  [\nu ] (or angular_frequency,     &#x03C9; = 2 &#x03C0;
&#x03BD;   {\displaystyle \omega =2\pi \nu }  [{\displaystyle \omega =2\pi \nu
}])
         E = h &#x03BD; = &#x210F; &#x03C9;     {\displaystyle E=h\nu =\hbar
      \omega \,\!}  [E=h\nu =\hbar \omega \,\!]
Likewise De_Broglie's_hypothesis (1924) states that any particle can be
associated with a wave, and that the momentum     p   {\displaystyle p}  [p] of
the particle is inversely proportional to the wavelength     &#x03BB;
{\displaystyle \lambda }  [\lambda ] of such a wave (or proportional to the
wavenumber,     k =    2 &#x03C0;  &#x03BB;     {\displaystyle k={\frac {2\pi }
{\lambda }}}  [k={\frac {2\pi }{\lambda }}]), in one dimension, by:
         p =   h &#x03BB;   = &#x210F; k  ,   {\displaystyle p={\frac {h}
      {\lambda }}=\hbar k\;,}  [p={\frac {h}{\lambda }}=\hbar k\;,]
while in three dimensions, wavelength Î» is related to the magnitude of the
wavevector k:
          p  = &#x210F;  k   ,   |   k   |  =    2 &#x03C0;  &#x03BB;    .
      {\displaystyle \mathbf {p} =\hbar \mathbf {k} \,,\quad |\mathbf {k} |=
      {\frac {2\pi }{\lambda }}\,.}  [\mathbf {p} =\hbar \mathbf {k} \,,\quad
      |\mathbf {k} |={\frac {2\pi }{\lambda }}\,.]
The PlanckâEinstein and de Broglie relations illuminate the deep connections
between energy with time, and space with momentum, and express waveâparticle
duality. In practice, natural_units comprising     &#x210F; = 1
{\displaystyle \hbar =1}  [\hbar = 1] are used, as the De Broglie equations
reduce to identities: allowing momentum, wave number, energy and frequency to
be used interchangeably, to prevent duplication of quantities, and reduce the
number of dimensions of related quantities. For familiarity SI units are still
used in this article.
SchrÃ¶dinger's insight,[citation_needed] late in 1925, was to express the phase
of a plane_wave as a complex phase_factor using these relations:
         &#x03A8; = A  e  i (  k  &#x22C5;  r  &#x2212; &#x03C9; t )   = A  e
      i (  p  &#x22C5;  r  &#x2212; E t )  /  &#x210F;     {\displaystyle \Psi
      =Ae^{i(\mathbf {k} \cdot \mathbf {r} -\omega t)}=Ae^{i(\mathbf {p} \cdot
      \mathbf {r} -Et)/\hbar }}  [\Psi =Ae^{i(\mathbf {k} \cdot \mathbf {r} -
      \omega t)}=Ae^{i(\mathbf {p} \cdot \mathbf {r} -Et)/\hbar }]
and to realize that the first order partial_derivatives with respect to space
were
         &#x2207; &#x03A8; =    i &#x210F;     p  A  e  i (  p  &#x22C5;  r
      &#x2212; E t )  /  &#x210F;   =    i &#x210F;     p  &#x03A8; .
      {\displaystyle \nabla \Psi ={\dfrac {i}{\hbar }}\mathbf {p} Ae^{i(\mathbf
      {p} \cdot \mathbf {r} -Et)/\hbar }={\dfrac {i}{\hbar }}\mathbf {p} \Psi
      .}  [{\displaystyle \nabla \Psi ={\dfrac {i}{\hbar }}\mathbf {p} Ae^{i
      (\mathbf {p} \cdot \mathbf {r} -Et)/\hbar }={\dfrac {i}{\hbar }}\mathbf
      {p} \Psi .}]
Taking partial derivatives with respect to time gives
             &#x2202; &#x03A8;   &#x2202; t     = &#x2212;     i E  &#x210F;
      A  e  i (  p  &#x22C5;  r  &#x2212; E t )  /  &#x210F;   = &#x2212;     i
      E  &#x210F;    &#x03A8; .   {\displaystyle {\dfrac {\partial \Psi }
      {\partial t}}=-{\dfrac {iE}{\hbar }}Ae^{i(\mathbf {p} \cdot \mathbf {r} -
      Et)/\hbar }=-{\dfrac {iE}{\hbar }}\Psi .}  [{\displaystyle {\dfrac
      {\partial \Psi }{\partial t}}=-{\dfrac {iE}{\hbar }}Ae^{i(\mathbf {p}
      \cdot \mathbf {r} -Et)/\hbar }=-{\dfrac {iE}{\hbar }}\Psi .}]
Another postulate of quantum mechanics is that all observables are represented
by linear Hermitian_operators which act on the wave function, and the
eigenvalues of the operator are the values the observable takes. The previous
derivatives are consistent with the energy_operator (or Hamiltonian operator),
corresponding to the time derivative,
            E &#x005E;    &#x03A8; = i &#x210F;    &#x2202;  &#x2202; t
      &#x03A8; = E &#x03A8;   {\displaystyle {\hat {E}}\Psi =i\hbar {\dfrac
      {\partial }{\partial t}}\Psi =E\Psi }  [{\hat {E}}\Psi =i\hbar {\dfrac
      {\partial }{\partial t}}\Psi =E\Psi ]
where E are the energy eigenvalues, and the momentum_operator, corresponding to
the spatial derivatives (the gradient     &#x2207;   {\displaystyle \nabla }
[\nabla ]),
             p  &#x005E;    &#x03A8; = &#x2212; i &#x210F; &#x2207; &#x03A8; =
      p  &#x03A8;   {\displaystyle {\hat {\mathbf {p} }}\Psi =-i\hbar \nabla
      \Psi =\mathbf {p} \Psi }  [{\hat {\mathbf {p} }}\Psi =-i\hbar \nabla \Psi
      =\mathbf {p} \Psi ]
where p is a vector of the momentum eigenvalues. In the above, the "hats" ( Ë
) indicate these observables are operators, not simply ordinary numbers or
vectors. The energy and momentum operators are differential_operators, while
the potential energy operator     V   {\displaystyle V}  [V] is just a
multiplicative factor.
Substituting the energy and momentum operators into the classical energy
conservation equation obtains the operator:
         E =      p  &#x22C5;  p    2 m     + V  &#x2192;     E &#x005E;    =
      p  &#x005E;    &#x22C5;     p  &#x005E;      2 m     + V   {\displaystyle
      E={\dfrac {\mathbf {p} \cdot \mathbf {p} }{2m}}+V\quad \rightarrow \quad
      {\hat {E}}={\dfrac {{\hat {\mathbf {p} }}\cdot {\hat {\mathbf {p} }}}
      {2m}}+V}  [E={\dfrac {\mathbf {p} \cdot \mathbf {p} }{2m}}+V\quad
      \rightarrow \quad {\hat {E}}={\dfrac {{\hat {\mathbf {p} }}\cdot {\hat
      {\mathbf {p} }}}{2m}}+V]
so in terms of derivatives with respect to time and space, acting this operator
on the wave function Î¨ immediately led SchrÃ¶dinger to his equation:[citation
needed]
         i &#x210F;     &#x2202; &#x03A8;   &#x2202; t     = &#x2212;
      &#x210F;  2    2 m      &#x2207;  2   &#x03A8; + V &#x03A8;
      {\displaystyle i\hbar {\dfrac {\partial \Psi }{\partial t}}=-{\dfrac
      {\hbar ^{2}}{2m}}\nabla ^{2}\Psi +V\Psi }  [i\hbar {\dfrac {\partial \Psi
      }{\partial t}}=-{\dfrac {\hbar ^{2}}{2m}}\nabla ^{2}\Psi +V\Psi ]
Waveâparticle duality can be assessed from these equations as follows. The
kinetic energy T is related to the square of momentum p. As the particle's
momentum increases, the kinetic energy increases more rapidly, but since the
wave number |k| increases the wavelength Î» decreases. In terms of ordinary
scalar and vector quantities (not operators):
          p  &#x22C5;  p  &#x221D;  k  &#x22C5;  k  &#x221D; T &#x221D;    1
      &#x03BB;  2        {\displaystyle \mathbf {p} \cdot \mathbf {p} \propto
      \mathbf {k} \cdot \mathbf {k} \propto T\propto {\dfrac {1}{\lambda ^
      {2}}}}  [\mathbf {p} \cdot \mathbf {p} \propto \mathbf {k} \cdot \mathbf
      {k} \propto T\propto {\dfrac {1}{\lambda ^{2}}}]
The kinetic energy is also proportional to the second spatial derivatives, so
it is also proportional to the magnitude of the curvature of the wave, in terms
of operators:
            T &#x005E;    &#x03A8; =    &#x2212;  &#x210F;  2     2 m
      &#x2207; &#x22C5; &#x2207; &#x03A8;  &#x221D;   &#x2207;  2   &#x03A8;  .
      {\displaystyle {\hat {T}}\Psi ={\frac {-\hbar ^{2}}{2m}}\nabla \cdot
      \nabla \Psi \,\propto \,\nabla ^{2}\Psi \,.}  [{\hat {T}}\Psi ={\frac {-
      \hbar ^{2}}{2m}}\nabla \cdot \nabla \Psi \,\propto \,\nabla ^{2}\Psi \,.]
As the curvature increases, the amplitude of the wave alternates between
positive and negative more rapidly, and also shortens the wavelength. So the
inverse relation between momentum and wavelength is consistent with the energy
the particle has, and so the energy of the particle has a connection to a wave,
all in the same mathematical formulation.[29]
**** Wave and particle motion[edit] ****
Increasing levels of wavepacket localization, meaning the particle has a more
localized position.
In the limit Ä§ â 0, the particle's position and momentum become known
exactly. This is equivalent to the classical particle.
SchrÃ¶dinger required that a wave_packet solution near position      r
{\displaystyle \mathbf {r} }  [\mathbf {r} ] with wave vector near      k
{\displaystyle \mathbf {k} }  [\mathbf {k} ] will move along the trajectory
determined by classical mechanics for times short enough for the spread in
k    {\displaystyle \mathbf {k} }  [\mathbf {k} ] (and hence in velocity) not
to substantially increase the spread in r. Since, for a given spread in k, the
spread in velocity is proportional to Planck's constant     &#x210F;
{\displaystyle \hbar }  [\hbar ], it is sometimes said that in the limit as
&#x210F;   {\displaystyle \hbar }  [\hbar ] approaches zero, the equations of
classical mechanics are restored from quantum mechanics.[33] Great care is
required in how that limit is taken, and in what cases.
The limiting short-wavelength is equivalent to     &#x210F;   {\displaystyle
\hbar }  [\hbar ] tending to zero because this is limiting case of increasing
the wave packet localization to the definite position of the particle (see
images right). Using the Heisenberg_uncertainty_principle for position and
momentum, the products of uncertainty in position and momentum become zero as
&#x210F; &#x27F6; 0   {\displaystyle \hbar \longrightarrow 0}  [{\displaystyle
\hbar \longrightarrow 0}]:
         &#x03C3; ( x ) &#x03C3; (  p  x   ) &#x2A7E;   &#x210F; 2    &#x2192;
      &#x03C3; ( x ) &#x03C3; (  p  x   ) &#x2A7E; 0     {\displaystyle \sigma
      (x)\sigma (p_{x})\geqslant {\frac {\hbar }{2}}\quad \rightarrow \quad
      \sigma (x)\sigma (p_{x})\geqslant 0\,\!}  [\sigma (x)\sigma (p_
      {x})\geqslant {\frac {\hbar }{2}}\quad \rightarrow \quad \sigma (x)\sigma
      (p_{x})\geqslant 0\,\!]
where Ï denotes the (root mean square) measurement_uncertainty in x and px
(and similarly for the y and z directions) which implies the position and
momentum can only be known to arbitrary precision in this limit.
One simple way to compare classical to quantum mechanics is to consider the
time-evolution of the expected position and expected momentum, which can then
be compared to the time-evolution of the ordinary position and momentum in
classical mechanics. The quantum expectation values satisfy the Ehrenfest
theorem. For a one-dimensional quantum particle moving in a potential     V
{\displaystyle V}  [V], the Ehrenfest theorem says[34]
         m   d  d t    &#x27E8; x &#x27E9; = &#x27E8; p &#x27E9; ;    d  d t
      &#x27E8; p &#x27E9; = &#x2212;  &#x27E8;   V &#x2032;  ( X )  &#x27E9;  .
      {\displaystyle m{\frac {d}{dt}}\langle x\rangle =\langle p\rangle ;\quad
      {\frac {d}{dt}}\langle p\rangle =-\left\langle V'(X)\right\rangle .}  [
      {\displaystyle m{\frac {d}{dt}}\langle x\rangle =\langle p\rangle ;\quad
      {\frac {d}{dt}}\langle p\rangle =-\left\langle V'(X)\right\rangle .}]
Although the first of these equations is consistent with the classical
behavior, the second is not: If the pair     ( &#x27E8; X &#x27E9; , &#x27E8; P
&#x27E9; )   {\displaystyle (\langle X\rangle ,\langle P\rangle )}  [
{\displaystyle (\langle X\rangle ,\langle P\rangle )}] were to satisfy Newton's
second law, the right-hand side of the second equation would have to be
         &#x2212;  V &#x2032;   (  &#x27E8; X &#x27E9;  )    {\displaystyle -
      V'\left(\left\langle X\right\rangle \right)}  [{\displaystyle -V'\left
      (\left\langle X\right\rangle \right)}],
which is typically not the same as     &#x2212;  &#x27E8;   V &#x2032;  ( X )
&#x27E9;    {\displaystyle -\left\langle V'(X)\right\rangle }  [{\displaystyle
-\left\langle V'(X)\right\rangle }]. In the case of the quantum harmonic
oscillator, however,      V &#x2032;    {\displaystyle V'}  [V'] is linear and
this distinction disappears, so that in this very special case, the expected
position and expected momentum do exactly follow the classical trajectories.
For general systems, the best we can hope for is that the expected position and
momentum will approximately follow the classical trajectories. If the wave
function is highly concentrated around a point      x  0     {\displaystyle x_
{0}}  [x_{0}], then      V &#x2032;   (  &#x27E8; X &#x27E9;  )
{\displaystyle V'\left(\left\langle X\right\rangle \right)}  [{\displaystyle
V'\left(\left\langle X\right\rangle \right)}] and      &#x27E8;   V &#x2032;
( X )  &#x27E9;    {\displaystyle \left\langle V'(X)\right\rangle }  [
{\displaystyle \left\langle V'(X)\right\rangle }] will be almost the same,
since both will be approximately equal to      V &#x2032;  (  x  0   )
{\displaystyle V'(x_{0})}  [{\displaystyle V'(x_{0})}]. In that case, the
expected position and expected momentum will remain very close to the classical
trajectories, at least for as long as the wave function remains highly
localized in position.[35] When Planck's constant is small, it is possible to
have a state that is well localized in both position and momentum. The small
uncertainty in momentum ensures that the particle remains well localized in
position for a long time, so that expected position and momentum continue to
closely track the classical trajectories.
The SchrÃ¶dinger equation in its general form
         i &#x210F;   &#x2202;  &#x2202; t    &#x03A8;  (   r  , t  )  =    H
      &#x005E;    &#x03A8;  (   r  , t  )      {\displaystyle i\hbar {\frac
      {\partial }{\partial t}}\Psi \left(\mathbf {r} ,t\right)={\hat {H}}\Psi
      \left(\mathbf {r} ,t\right)\,\!}  [i\hbar {\frac {\partial }{\partial
      t}}\Psi \left(\mathbf {r} ,t\right)={\hat {H}}\Psi \left(\mathbf {r}
      ,t\right)\,\!]
is closely related to the HamiltonâJacobi_equation (HJE)
         &#x2212;   &#x2202;  &#x2202; t    S (  q  i   , t ) = H  (   q  i   ,
      &#x2202; S   &#x2202;  q  i      , t  )      {\displaystyle -{\frac
      {\partial }{\partial t}}S(q_{i},t)=H\left(q_{i},{\frac {\partial S}
      {\partial q_{i}}},t\right)\,\!}  [{\displaystyle -{\frac {\partial }
      {\partial t}}S(q_{i},t)=H\left(q_{i},{\frac {\partial S}{\partial q_
      {i}}},t\right)\,\!}]
where     S   {\displaystyle S}  [S] is the classical action and     H
{\displaystyle H}  [H] is the Hamiltonian_function (not operator). Here the
generalized_coordinates      q  i     {\displaystyle q_{i}}  [q_{i}] for     i
= 1 , 2 , 3   {\displaystyle i=1,2,3}  [{\displaystyle i=1,2,3}] (used in the
context of the HJE) can be set to the position in Cartesian coordinates as
r  = (  q  1   ,  q  2   ,  q  3   ) = ( x , y , z )   {\displaystyle \mathbf
{r} =(q_{1},q_{2},q_{3})=(x,y,z)}  [{\displaystyle \mathbf {r} =(q_{1},q_{2},q_
{3})=(x,y,z)}].[33]
Substituting
         &#x03A8; =   &#x03C1; (  r  , t )    e  i S (  r  , t )  /  &#x210F;
      {\displaystyle \Psi ={\sqrt {\rho (\mathbf {r} ,t)}}e^{iS(\mathbf {r}
      ,t)/\hbar }\,\!}  [\Psi ={\sqrt {\rho (\mathbf {r} ,t)}}e^{iS(\mathbf {r}
      ,t)/\hbar }\,\!]
where     &#x03C1;   {\displaystyle \rho }  [\rho ] is the probability density,
into the SchrÃ¶dinger equation and then taking the limit     &#x210F; &#x27F6;
0   {\displaystyle \hbar \longrightarrow 0}  [{\displaystyle \hbar
\longrightarrow 0}] in the resulting equation yield the HamiltonâJacobi
equation.
The implications are as follows:
    * The motion of a particle, described by a (short-wavelength) wave packet
      solution to the SchrÃ¶dinger equation, is also described by the
      HamiltonâJacobi equation of motion.
    * The SchrÃ¶dinger equation includes the wave function, so its wave packet
      solution implies the position of a (quantum) particle is fuzzily spread
      out in wave fronts. On the contrary, the HamiltonâJacobi equation
      applies to a (classical) particle of definite position and momentum,
      instead the position and momentum at all times (the trajectory) are
      deterministic and can be simultaneously known.
***** Nonrelativistic quantum mechanics[edit] *****
The quantum mechanics of particles without accounting for the effects of
special_relativity, for example particles propagating at speeds much less than
light, is known as nonrelativistic quantum mechanics. Following are several
forms of SchrÃ¶dinger's equation in this context for different situations: time
independence and dependence, one and three spatial dimensions, and one and N
particles.
In actuality, the particles constituting the system do not have the numerical
labels used in theory. The language of mathematics forces us to label the
positions of particles one way or another, otherwise there would be confusion
between symbols representing which variables are for which particle.[31]
**** Time-independent[edit] ****
If the Hamiltonian is not an explicit function of time, the equation is
separable into a product of spatial and temporal parts. In general, the wave
function takes the form:
         &#x03A8; (  space coords  , t ) = &#x03C8; (  space coords  ) &#x03C4;
      ( t )  .   {\displaystyle \Psi ({\text{space coords}},t)=\psi ({\text
      {space coords}})\tau (t)\,.}  [\Psi ({\text{space coords}},t)=\psi (
      {\text{space coords}})\tau (t)\,.]
where Ï(space coords) is a function of all the spatial coordinate(s) of the
particle(s) constituting the system only, and Ï(t) is a function of time only.
Substituting for ψ into the SchrÃ¶dinger equation for the relevant number of
particles in the relevant number of dimensions, solving by separation_of
variables implies the general solution of the time-dependent equation has the
form:[17]
         &#x03A8; (  space coords  , t ) = &#x03C8; (  space coords  )  e
      &#x2212; i  E t  /  &#x210F;     .   {\displaystyle \Psi ({\text{space
      coords}},t)=\psi ({\text{space coords}})e^{-i{Et/\hbar }}\,.}  [\Psi (
      {\text{space coords}},t)=\psi ({\text{space coords}})e^{-i{Et/\hbar
      }}\,.]
Since the time dependent phase factor is always the same, only the spatial part
needs to be solved for in time independent problems. Additionally, the energy
operator Ã = iÄ§â/ât can always be replaced by the energy eigenvalue E,
thus the time independent SchrÃ¶dinger equation is an eigenvalue equation for
the Hamiltonian operator:[5]:143ff
            H &#x005E;    &#x03C8; = E &#x03C8;   {\displaystyle {\hat {H}}\psi
      =E\psi }  [{\hat {H}}\psi =E\psi ]
This is true for any number of particles in any number of dimensions (in a time
independent potential). This case describes the standing_wave solutions of the
time-dependent equation, which are the states with definite energy (instead of
a probability distribution of different energies). In physics, these standing
waves are called "stationary_states" or "energy_eigenstates"; in chemistry they
are called "atomic_orbitals" or "molecular_orbitals". Superpositions of energy
eigenstates change their properties according to the relative phases between
the energy levels.
The energy eigenvalues from this equation form a discrete spectrum of values,
so mathematically energy must be quantized. More specifically, the energy
eigenstates form a basis â any wave function may be written as a sum over the
discrete energy states or an integral over continuous energy states, or more
generally as an integral over a measure. This is the spectral_theorem in
mathematics, and in a finite state space it is just a statement of the
completeness of the eigenvectors of a Hermitian_matrix.
**** One-dimensional examples[edit] ****
For a particle in one dimension, the Hamiltonian is:
            H &#x005E;    =       p &#x005E;     2    2 m    + V ( x )  ,     p
      &#x005E;    = &#x2212; i &#x210F;   d  d x      {\displaystyle {\hat
      {H}}={\frac {{\hat {p}}^{2}}{2m}}+V(x)\,,\quad {\hat {p}}=-i\hbar {\frac
      {d}{dx}}}  [{\hat {H}}={\frac {{\hat {p}}^{2}}{2m}}+V(x)\,,\quad {\hat
      {p}}=-i\hbar {\frac {d}{dx}}]
and substituting this into the general SchrÃ¶dinger equation gives:
          [  &#x2212;    &#x210F;  2    2 m       d  2    d  x  2      + V ( x
      )  ]  &#x03C8; ( x ) = E &#x03C8; ( x )   {\displaystyle \left[-{\frac
      {\hbar ^{2}}{2m}}{\frac {d^{2}}{dx^{2}}}+V(x)\right]\psi (x)=E\psi (x)}
      [{\displaystyle \left[-{\frac {\hbar ^{2}}{2m}}{\frac {d^{2}}{dx^{2}}}+V
      (x)\right]\psi (x)=E\psi (x)}]
This is the only case the SchrÃ¶dinger equation is an ordinary differential
equation, rather than a partial differential equation. The general solutions
are always of the form:
         &#x03A8; ( x , t ) = &#x03C8; ( x )  e  &#x2212; i E t  /  &#x210F;
      .   {\displaystyle \Psi (x,t)=\psi (x)e^{-iEt/\hbar }\,.}  [\Psi
      (x,t)=\psi (x)e^{-iEt/\hbar }\,.]
For N particles in one dimension, the Hamiltonian is:
            H &#x005E;    =  &#x2211;  n = 1   N         p &#x005E;     n   2
      2  m  n      + V (  x  1   ,  x  2   , &#x22EF;  x  N   )  ,      p
      &#x005E;     n   = &#x2212; i &#x210F;   &#x2202;  &#x2202;  x  n
      {\displaystyle {\hat {H}}=\sum _{n=1}^{N}{\frac {{\hat {p}}_{n}^{2}}{2m_
      {n}}}+V(x_{1},x_{2},\cdots x_{N})\,,\quad {\hat {p}}_{n}=-i\hbar {\frac
      {\partial }{\partial x_{n}}}}  [{\hat {H}}=\sum _{n=1}^{N}{\frac {{\hat
      {p}}_{n}^{2}}{2m_{n}}}+V(x_{1},x_{2},\cdots x_{N})\,,\quad {\hat {p}}_
      {n}=-i\hbar {\frac {\partial }{\partial x_{n}}}]
where the position of particle n is xn. The corresponding SchrÃ¶dinger equation
is:
         &#x2212;    &#x210F;  2   2    &#x2211;  n = 1   N     1  m  n
      &#x2202;  2    &#x2202;  x  n   2      &#x03C8; (  x  1   ,  x  2   ,
      &#x22EF;  x  N   ) + V (  x  1   ,  x  2   , &#x22EF;  x  N   ) &#x03C8;
      (  x  1   ,  x  2   , &#x22EF;  x  N   ) = E &#x03C8; (  x  1   ,  x  2
      , &#x22EF;  x  N   )  .   {\displaystyle -{\frac {\hbar ^{2}}{2}}\sum _
      {n=1}^{N}{\frac {1}{m_{n}}}{\frac {\partial ^{2}}{\partial x_{n}^
      {2}}}\psi (x_{1},x_{2},\cdots x_{N})+V(x_{1},x_{2},\cdots x_{N})\psi (x_
      {1},x_{2},\cdots x_{N})=E\psi (x_{1},x_{2},\cdots x_{N})\,.}  [-{\frac
      {\hbar ^{2}}{2}}\sum _{n=1}^{N}{\frac {1}{m_{n}}}{\frac {\partial ^{2}}
      {\partial x_{n}^{2}}}\psi (x_{1},x_{2},\cdots x_{N})+V(x_{1},x_{2},\cdots
      x_{N})\psi (x_{1},x_{2},\cdots x_{N})=E\psi (x_{1},x_{2},\cdots x_
      {N})\,.]
so the general solutions have the form:
         &#x03A8; (  x  1   ,  x  2   , &#x22EF;  x  N   , t ) =  e  &#x2212; i
      E t  /  &#x210F;   &#x03C8; (  x  1   ,  x  2   &#x22EF;  x  N   )
      {\displaystyle \Psi (x_{1},x_{2},\cdots x_{N},t)=e^{-iEt/\hbar }\psi (x_
      {1},x_{2}\cdots x_{N})}  [\Psi (x_{1},x_{2},\cdots x_{N},t)=e^{-iEt/\hbar
      }\psi (x_{1},x_{2}\cdots x_{N})]
For non-interacting distinguishable particles,[36] the potential of the system
only influences each particle separately, so the total potential energy is the
sum of potential energies for each particle:
         V (  x  1   ,  x  2   , &#x22EF;  x  N   ) =  &#x2211;  n = 1   N   V
      (  x  n   )  .   {\displaystyle V(x_{1},x_{2},\cdots x_{N})=\sum _{n=1}^
      {N}V(x_{n})\,.}  [V(x_{1},x_{2},\cdots x_{N})=\sum _{n=1}^{N}V(x_{n})\,.]
and the wave function can be written as a product of the wave functions for
each particle:
         &#x03A8; (  x  1   ,  x  2   , &#x22EF;  x  N   , t ) =  e  &#x2212; i
      E t  /  &#x210F;     &#x220F;  n = 1   N   &#x03C8; (  x  n   )  ,
      {\displaystyle \Psi (x_{1},x_{2},\cdots x_{N},t)=e^{-i{Et/\hbar }}\prod _
      {n=1}^{N}\psi (x_{n})\,,}  [\Psi (x_{1},x_{2},\cdots x_{N},t)=e^{-i{Et/
      \hbar }}\prod _{n=1}^{N}\psi (x_{n})\,,]
For non-interacting identical_particles, the potential is still a sum, but wave
function is a bit more complicated â it is a sum over the permutations of
products of the separate wave functions to account for particle exchange. In
general for interacting particles, the above decompositions are not possible.
*** Free particle[edit] ***
For no potential, V = 0, so the particle is free and the equation reads:[5]:
151ff
         &#x2212; E &#x03C8; =    &#x210F;  2    2 m        d  2   &#x03C8;   d
      x  2         {\displaystyle -E\psi ={\frac {\hbar ^{2}}{2m}}{d^{2}\psi
      \over dx^{2}}\,}  [-E\psi ={\frac {\hbar ^{2}}{2m}}{d^{2}\psi  \over dx^
      {2}}\,]
which has oscillatory solutions for E > 0 (the Cn are arbitrary constants):
          &#x03C8;  E   ( x ) =  C  1    e  i   2 m E  /   &#x210F;  2      x
      +  C  2    e  &#x2212; i   2 m E  /   &#x210F;  2      x
      {\displaystyle \psi _{E}(x)=C_{1}e^{i{\sqrt {2mE/\hbar ^{2}}}\,x}+C_{2}e^
      {-i{\sqrt {2mE/\hbar ^{2}}}\,x}\,}  [\psi _{E}(x)=C_{1}e^{i{\sqrt {2mE/
      \hbar ^{2}}}\,x}+C_{2}e^{-i{\sqrt {2mE/\hbar ^{2}}}\,x}\,]
and exponential solutions for E < 0
          &#x03C8;  &#x2212;  |  E  |    ( x ) =  C  1    e    2 m  |  E  |   /
      &#x210F;  2      x   +  C  2    e  &#x2212;   2 m  |  E  |   /   &#x210F;
      2      x   .    {\displaystyle \psi _{-|E|}(x)=C_{1}e^{{\sqrt {2m|E|/
      \hbar ^{2}}}\,x}+C_{2}e^{-{\sqrt {2m|E|/\hbar ^{2}}}\,x}.\,}  [\psi _{-
      |E|}(x)=C_{1}e^{{\sqrt {2m|E|/\hbar ^{2}}}\,x}+C_{2}e^{-{\sqrt {2m|E|/
      \hbar ^{2}}}\,x}.\,]
The exponentially growing solutions have an infinite norm, and are not
physical. They are not allowed in a finite volume with periodic or fixed
boundary conditions.
See also free_particle and wavepacket for more discussion on the free particle.
*** Constant potential[edit] ***
[Animation_of_a_de_Broglie_wave_incident_on_a_barrier.]
For a constant potential, V = V0, the solution is oscillatory for E > V0 and
exponential for E < V0, corresponding to energies that are allowed or
disallowed in classical mechanics. Oscillatory solutions have a classically
allowed energy and correspond to actual classical motions, while the
exponential solutions have a disallowed energy and describe a small amount of
quantum bleeding into the classically disallowed region, due to quantum
tunneling. If the potential V0 grows to infinity, the motion is classically
confined to a finite region. Viewed far enough away, every solution is reduced
to an exponential; the condition that the exponential is decreasing restricts
the energy levels to a discrete set, called the allowed energies.[32]
*** Harmonic oscillator[edit] ***
A harmonic_oscillator in classical mechanics (AâB) and quantum mechanics
(CâH). In (AâB), a ball, attached to a spring, oscillates back and forth.
(CâH) are six solutions to the SchrÃ¶dinger Equation for this situation. The
horizontal axis is position, the vertical axis is the real part (blue) or
imaginary part (red) of the wave_function. Stationary_states, or energy
eigenstates, which are solutions to the time-independent SchrÃ¶dinger equation,
are shown in C, D, E, F, but not G or H.
Main article: Quantum_harmonic_oscillator
The SchrÃ¶dinger equation for this situation is
         E &#x03C8; = &#x2212;    &#x210F;  2    2 m       d  2    d  x  2
      &#x03C8; +   1 2   m  &#x03C9;  2    x  2   &#x03C8;   {\displaystyle
      E\psi =-{\frac {\hbar ^{2}}{2m}}{\frac {d^{2}}{dx^{2}}}\psi +{\frac {1}
      {2}}m\omega ^{2}x^{2}\psi }  [E\psi =-{\frac {\hbar ^{2}}{2m}}{\frac {d^
      {2}}{dx^{2}}}\psi +{\frac {1}{2}}m\omega ^{2}x^{2}\psi ]
This is an example of a quantum-mechanical system whose wave function can be
solved for exactly. Furthermore, it can be used to describe approximately a
wide variety of other systems, including vibrating_atoms,_molecules,[37] and
atoms or ions in lattices,[38] and approximating other potentials near
equilibrium points. It is also the basis_of_perturbation_methods in quantum
mechanics.
The solutions in position space are
          &#x03C8;  n   ( x ) =    1   2  n    n !     &#x22C5;   (    m
      &#x03C9;   &#x03C0; &#x210F;    )   1  /  4   &#x22C5;  e  &#x2212;    m
      &#x03C9;  x  2     2 &#x210F;      &#x22C5;    H    n    (      m
      &#x03C9;  &#x210F;    x  )  ,   {\displaystyle \psi _{n}(x)={\sqrt {\frac
      {1}{2^{n}\,n!}}}\cdot \left({\frac {m\omega }{\pi \hbar }}\right)^{1/
      4}\cdot e^{-{\frac {m\omega x^{2}}{2\hbar }}}\cdot {\mathcal {H}}_
      {n}\left({\sqrt {\frac {m\omega }{\hbar }}}x\right),}  [{\displaystyle
      \psi _{n}(x)={\sqrt {\frac {1}{2^{n}\,n!}}}\cdot \left({\frac {m\omega }
      {\pi \hbar }}\right)^{1/4}\cdot e^{-{\frac {m\omega x^{2}}{2\hbar
      }}}\cdot {\mathcal {H}}_{n}\left({\sqrt {\frac {m\omega }{\hbar
      }}}x\right),}]
where     n = 0 , 1 , 2 , . . .   {\displaystyle n=0,1,2,...}  [{\displaystyle
n=0,1,2,...}], and the functions        H    n     {\displaystyle {\mathcal
{H}}_{n}}  [{\displaystyle {\mathcal {H}}_{n}}] are the Hermite_polynomials of
order     n   {\displaystyle n}  [{\displaystyle n}]. The solution set may be
generated by
    &#x03C8;  n   ( x ) =   1  n !      (     m &#x03C9;   2 &#x210F;     )   n
(  x &#x2212;   &#x210F;  m &#x03C9;      d  d x     )   n     (    m &#x03C9;
&#x03C0; &#x210F;    )    1 4     e    &#x2212; m &#x03C9;  x  2     2 &#x210F;
{\displaystyle \psi _{n}(x)={\frac {1}{\sqrt {n!}}}\left({\sqrt {\frac {m\omega
}{2\hbar }}}\right)^{n}\left(x-{\frac {\hbar }{m\omega }}{\frac {d}
{dx}}\right)^{n}\left({\frac {m\omega }{\pi \hbar }}\right)^{\frac {1}{4}}e^
{\frac {-m\omega x^{2}}{2\hbar }}}  [{\displaystyle \psi _{n}(x)={\frac {1}
{\sqrt {n!}}}\left({\sqrt {\frac {m\omega }{2\hbar }}}\right)^{n}\left(x-{\frac
{\hbar }{m\omega }}{\frac {d}{dx}}\right)^{n}\left({\frac {m\omega }{\pi \hbar
}}\right)^{\frac {1}{4}}e^{\frac {-m\omega x^{2}}{2\hbar }}}]
The eigenvalues are
    E  n   =  (  n +   1 2    )  &#x210F; &#x03C9;   {\displaystyle E_{n}=\left
(n+{\frac {1}{2}}\right)\hbar \omega }  [{\displaystyle E_{n}=\left(n+{\frac
{1}{2}}\right)\hbar \omega }]. The case     n = 0   {\displaystyle n=0}  [
{\displaystyle n=0}] is called the zero-point_energy and the wave function is a
Gaussian.[39]
**** Three-dimensional examples[edit] ****
The extension from one dimension to three dimensions is straightforward, all
position and momentum operators are replaced by their three-dimensional
expressions and the partial derivative with respect to space is replaced by the
gradient operator.
The Hamiltonian for one particle in three dimensions is:
            H &#x005E;    =        p  &#x005E;    &#x22C5;     p  &#x005E;
      2 m    + V (  r  )  ,      p  &#x005E;    = &#x2212; i &#x210F; &#x2207;
      {\displaystyle {\hat {H}}={\frac {{\hat {\mathbf {p} }}\cdot {\hat
      {\mathbf {p} }}}{2m}}+V(\mathbf {r} )\,,\quad {\hat {\mathbf {p} }}=-
      i\hbar \nabla }  [{\hat {H}}={\frac {{\hat {\mathbf {p} }}\cdot {\hat
      {\mathbf {p} }}}{2m}}+V(\mathbf {r} )\,,\quad {\hat {\mathbf {p} }}=-
      i\hbar \nabla ]
generating the equation
          [  &#x2212;    &#x210F;  2    2 m     &#x2207;  2   + V (  r  )  ]
      &#x03C8; (  r  ) = E &#x03C8; (  r  )   {\displaystyle \left[-{\frac
      {\hbar ^{2}}{2m}}\nabla ^{2}+V(\mathbf {r} )\right]\psi (\mathbf {r}
      )=E\psi (\mathbf {r} )}  [{\displaystyle \left[-{\frac {\hbar ^{2}}
      {2m}}\nabla ^{2}+V(\mathbf {r} )\right]\psi (\mathbf {r} )=E\psi (\mathbf
      {r} )}]
with stationary state solutions of the form
         &#x03A8; (  r  , t ) = &#x03C8; (  r  )  e  &#x2212; i E t  /
      &#x210F;   ,   {\displaystyle \Psi (\mathbf {r} ,t)=\psi (\mathbf {r} )e^
      {-iEt/\hbar },}  [{\displaystyle \Psi (\mathbf {r} ,t)=\psi (\mathbf {r}
      )e^{-iEt/\hbar },}]
where the position of the particle is      r    {\displaystyle \mathbf {r} }
[\mathbf {r} ].
For     N   {\displaystyle N}  [N] particles in three dimensions, the
Hamiltonian is
            H &#x005E;    =  &#x2211;  n = 1   N           p  &#x005E;     n
      &#x22C5;      p  &#x005E;     n     2  m  n      + V (   r   1   ,   r
      2   , &#x22EF;   r   N   )  ,       p  &#x005E;     n   = &#x2212; i
      &#x210F;  &#x2207;  n     {\displaystyle {\hat {H}}=\sum _{n=1}^{N}{\frac
      {{\hat {\mathbf {p} }}_{n}\cdot {\hat {\mathbf {p} }}_{n}}{2m_{n}}}+V
      (\mathbf {r} _{1},\mathbf {r} _{2},\cdots \mathbf {r} _{N})\,,\quad {\hat
      {\mathbf {p} }}_{n}=-i\hbar \nabla _{n}}  [{\hat {H}}=\sum _{n=1}^{N}
      {\frac {{\hat {\mathbf {p} }}_{n}\cdot {\hat {\mathbf {p} }}_{n}}{2m_
      {n}}}+V(\mathbf {r} _{1},\mathbf {r} _{2},\cdots \mathbf {r} _
      {N})\,,\quad {\hat {\mathbf {p} }}_{n}=-i\hbar \nabla _{n}]
where the position of particle n is rn and the gradient operators are partial
derivatives with respect to the particle's position coordinates. In Cartesian
coordinates, for particle n, the position vector is rn = (xn, yn, zn) while the
gradient and Laplacian_operator are respectively:
          &#x2207;  n   =   e   x     &#x2202;  &#x2202;  x  n      +   e   y
      &#x2202;  &#x2202;  y  n      +   e   z     &#x2202;  &#x2202;  z  n
      ,   &#x2207;  n   2   =  &#x2207;  n   &#x22C5;  &#x2207;  n   =
      &#x2202;  2     &#x2202;  x  n     2     +    &#x2202;  2     &#x2202;  y
      n     2     +    &#x2202;  2     &#x2202;  z  n     2
      {\displaystyle \nabla _{n}=\mathbf {e} _{x}{\frac {\partial }{\partial x_
      {n}}}+\mathbf {e} _{y}{\frac {\partial }{\partial y_{n}}}+\mathbf {e} _
      {z}{\frac {\partial }{\partial z_{n}}}\,,\quad \nabla _{n}^{2}=\nabla _
      {n}\cdot \nabla _{n}={\frac {\partial ^{2}}{{\partial x_{n}}^{2}}}+{\frac
      {\partial ^{2}}{{\partial y_{n}}^{2}}}+{\frac {\partial ^{2}}{{\partial
      z_{n}}^{2}}}}  [\nabla _{n}=\mathbf {e} _{x}{\frac {\partial }{\partial
      x_{n}}}+\mathbf {e} _{y}{\frac {\partial }{\partial y_{n}}}+\mathbf {e} _
      {z}{\frac {\partial }{\partial z_{n}}}\,,\quad \nabla _{n}^{2}=\nabla _
      {n}\cdot \nabla _{n}={\frac {\partial ^{2}}{{\partial x_{n}}^{2}}}+{\frac
      {\partial ^{2}}{{\partial y_{n}}^{2}}}+{\frac {\partial ^{2}}{{\partial
      z_{n}}^{2}}}]
The SchrÃ¶dinger equation is:
         &#x2212;    &#x210F;  2   2    &#x2211;  n = 1   N     1  m  n
      &#x2207;  n   2   &#x03A8; (   r   1   ,   r   2   , &#x22EF;   r   N   )
      + V (   r   1   ,   r   2   , &#x22EF;   r   N   ) &#x03A8; (   r   1   ,
      r   2   , &#x22EF;   r   N   ) = E &#x03A8; (   r   1   ,   r   2   ,
      &#x22EF;   r   N   )   {\displaystyle -{\frac {\hbar ^{2}}{2}}\sum _
      {n=1}^{N}{\frac {1}{m_{n}}}\nabla _{n}^{2}\Psi (\mathbf {r} _{1},\mathbf
      {r} _{2},\cdots \mathbf {r} _{N})+V(\mathbf {r} _{1},\mathbf {r} _
      {2},\cdots \mathbf {r} _{N})\Psi (\mathbf {r} _{1},\mathbf {r} _
      {2},\cdots \mathbf {r} _{N})=E\Psi (\mathbf {r} _{1},\mathbf {r} _
      {2},\cdots \mathbf {r} _{N})}  [-{\frac {\hbar ^{2}}{2}}\sum _{n=1}^{N}
      {\frac {1}{m_{n}}}\nabla _{n}^{2}\Psi (\mathbf {r} _{1},\mathbf {r} _
      {2},\cdots \mathbf {r} _{N})+V(\mathbf {r} _{1},\mathbf {r} _{2},\cdots
      \mathbf {r} _{N})\Psi (\mathbf {r} _{1},\mathbf {r} _{2},\cdots \mathbf
      {r} _{N})=E\Psi (\mathbf {r} _{1},\mathbf {r} _{2},\cdots \mathbf {r} _
      {N})]
with stationary state solutions:
         &#x03A8; (   r   1   ,   r   2   &#x22EF;   r   N   , t ) =  e
      &#x2212; i E t  /  &#x210F;   &#x03C8; (   r   1   ,   r   2   &#x22EF;
      r   N   )   {\displaystyle \Psi (\mathbf {r} _{1},\mathbf {r} _{2}\cdots
      \mathbf {r} _{N},t)=e^{-iEt/\hbar }\psi (\mathbf {r} _{1},\mathbf {r} _
      {2}\cdots \mathbf {r} _{N})}  [\Psi (\mathbf {r} _{1},\mathbf {r} _
      {2}\cdots \mathbf {r} _{N},t)=e^{-iEt/\hbar }\psi (\mathbf {r} _
      {1},\mathbf {r} _{2}\cdots \mathbf {r} _{N})]
Again, for non-interacting distinguishable particles the potential is the sum
of particle potentials
         V (   r   1   ,   r   2   , &#x22EF;   r   N   ) =  &#x2211;  n = 1
      N   V (   r   n   )   {\displaystyle V(\mathbf {r} _{1},\mathbf {r} _
      {2},\cdots \mathbf {r} _{N})=\sum _{n=1}^{N}V(\mathbf {r} _{n})}  [V
      (\mathbf {r} _{1},\mathbf {r} _{2},\cdots \mathbf {r} _{N})=\sum _{n=1}^
      {N}V(\mathbf {r} _{n})]
and the wave function is a product of the particle wave functions
         &#x03A8; (   r   1   ,   r   2   &#x22EF;   r   N   , t ) =  e
      &#x2212; i  E t  /  &#x210F;     &#x220F;  n = 1   N   &#x03C8; (   r   n
      )  .   {\displaystyle \Psi (\mathbf {r} _{1},\mathbf {r} _{2}\cdots
      \mathbf {r} _{N},t)=e^{-i{Et/\hbar }}\prod _{n=1}^{N}\psi (\mathbf {r} _
      {n})\,.}  [\Psi (\mathbf {r} _{1},\mathbf {r} _{2}\cdots \mathbf {r} _
      {N},t)=e^{-i{Et/\hbar }}\prod _{n=1}^{N}\psi (\mathbf {r} _{n})\,.]
For non-interacting identical particles, the potential is a sum but the wave
function is a sum over permutations of products. The previous two equations do
not apply to interacting particles.
Following are examples where exact solutions are known. See the main articles
for further details.
*** Hydrogen atom[edit] ***
The SchrÃ¶dinger equation the hydrogen_atom (or a hydrogen-like atom) is[27]
[29]
         E &#x03C8; = &#x2212;    &#x210F;  2    2 &#x03BC;     &#x2207;  2
      &#x03C8; &#x2212;    q  2    4 &#x03C0;  &#x03B5;  0   r    &#x03C8;
      {\displaystyle E\psi =-{\frac {\hbar ^{2}}{2\mu }}\nabla ^{2}\psi -{\frac
      {q^{2}}{4\pi \varepsilon _{0}r}}\psi }  [{\displaystyle E\psi =-{\frac
      {\hbar ^{2}}{2\mu }}\nabla ^{2}\psi -{\frac {q^{2}}{4\pi \varepsilon _
      {0}r}}\psi }]
where     q   {\displaystyle q}  [q] is the electron charge,      r
{\displaystyle \mathbf {r} }  [\mathbf {r} ] is the position of the electron
relative to the nucleus,     r =  |   r   |    {\displaystyle r=|\mathbf {r} |}
[{\displaystyle r=|\mathbf {r} |}] is the magnitude of the relative position,
the potential term is due to the Coulomb_interaction, wherein      &#x03B5;  0
{\displaystyle \varepsilon _{0}}  [\varepsilon _{0}] is the permittivity_of
free_space and
         &#x03BC; =     m  q    m  p      m  q   +  m  p        {\displaystyle
      \mu ={\frac {m_{q}m_{p}}{m_{q}+m_{p}}}}  [{\displaystyle \mu ={\frac {m_
      {q}m_{p}}{m_{q}+m_{p}}}}]
is the 2-body reduced_mass of the hydrogen nucleus (just a proton) of mass
m  p     {\displaystyle m_{p}}  [{\displaystyle m_{p}}] and the electron of
mass      m  q     {\displaystyle m_{q}}  [{\displaystyle m_{q}}]. The negative
sign arises in the potential term since the proton and electron are oppositely
charged. The reduced mass in place of the electron mass is used since the
electron and proton together orbit each other about a common centre of mass,
and constitute a two-body problem to solve. The motion of the electron is of
principle interest here, so the equivalent one-body problem is the motion of
the electron using the reduced mass.
The SchrÃ¶dinger for a hydrogen atom can be solved by separation of variables.
[40] In this case, spherical_polar_coordinates are the most convenient. Thus,
         &#x03C8; ( r , &#x03B8; , &#x03D5; ) = R ( r )  Y  &#x2113;   m
      ( &#x03B8; , &#x03D5; ) = R ( r ) &#x0398; ( &#x03B8; ) &#x03A6;
      ( &#x03D5; ) ,   {\displaystyle \psi (r,\theta ,\phi )=R(r)Y_{\ell }^{m}
      (\theta ,\phi )=R(r)\Theta (\theta )\Phi (\phi ),}  [{\displaystyle \psi
      (r,\theta ,\phi )=R(r)Y_{\ell }^{m}(\theta ,\phi )=R(r)\Theta (\theta
      )\Phi (\phi ),}]
where R are radial functions and      Y  l   m   ( &#x03B8; , &#x03D5; )
{\displaystyle Y_{l}^{m}(\theta ,\phi )}  [{\displaystyle Y_{l}^{m}(\theta
,\phi )}] are spherical_harmonics of degree     &#x2113;   {\displaystyle \ell
}  [\ell ] and order     m   {\displaystyle m}  [m]. This is the only atom for
which the SchrÃ¶dinger equation has been solved for exactly. Multi-electron
atoms require approximate methods. The family of solutions are:[41]
          &#x03C8;  n &#x2113; m   ( r , &#x03B8; , &#x03D5; ) =      (   2  n
      a  0      )    3      ( n &#x2212; &#x2113; &#x2212; 1 ) !   2 n [ ( n +
      &#x2113; ) ! ]       e  &#x2212; r  /  n  a  0       (    2 r   n  a  0
      )   &#x2113;    L  n &#x2212; &#x2113; &#x2212; 1   2 &#x2113; + 1
      (    2 r   n  a  0      )  &#x22C5;  Y  &#x2113;   m   ( &#x03B8; ,
      &#x03D5; )   {\displaystyle \psi _{n\ell m}(r,\theta ,\phi )={\sqrt {
      {\left({\frac {2}{na_{0}}}\right)}^{3}{\frac {(n-\ell -1)!}{2n[(n+\ell
      )!]}}}}e^{-r/na_{0}}\left({\frac {2r}{na_{0}}}\right)^{\ell }L_{n-\ell -
      1}^{2\ell +1}\left({\frac {2r}{na_{0}}}\right)\cdot Y_{\ell }^{m}(\theta
      ,\phi )}  [\psi _{n\ell m}(r,\theta ,\phi )={\sqrt {{\left({\frac {2}{na_
      {0}}}\right)}^{3}{\frac {(n-\ell -1)!}{2n[(n+\ell )!]}}}}e^{-r/na_
      {0}}\left({\frac {2r}{na_{0}}}\right)^{\ell }L_{n-\ell -1}^{2\ell
      +1}\left({\frac {2r}{na_{0}}}\right)\cdot Y_{\ell }^{m}(\theta ,\phi )]
where:
    *     a  0   =    4 &#x03C0;  &#x03B5;  0    &#x210F;  2      m  q    q  2
      {\displaystyle a_{0}={\frac {4\pi \varepsilon _{0}\hbar ^{2}}{m_{q}q^
      {2}}}}  [{\displaystyle a_{0}={\frac {4\pi \varepsilon _{0}\hbar ^{2}}{m_
      {q}q^{2}}}}] is the Bohr_radius,
    *     L  n &#x2212; &#x2113; &#x2212; 1   2 &#x2113; + 1   ( &#x22EF; )
      {\displaystyle L_{n-\ell -1}^{2\ell +1}(\cdots )}  [L_{n-\ell -1}^{2\ell
      +1}(\cdots )] are the generalized_Laguerre_polynomials of degree     n
      &#x2212; &#x2113; &#x2212; 1   {\displaystyle n-\ell -1}  [{\displaystyle
      n-\ell -1}].
    *    n , &#x2113; , m   {\displaystyle n,\ell ,m}  [{\displaystyle n,\ell
      ,m}] are the principal, azimuthal, and magnetic quantum_numbers
      respectively, which take the values:
             n    = 1 , 2 , 3 , &#x2026;     &#x2113;    = 0 , 1 , 2 , &#x2026;
      , n &#x2212; 1     m    = &#x2212; &#x2113; , &#x2026; , &#x2113;
      {\displaystyle {\begin{aligned}n&=1,2,3,\dots \\\ell &=0,1,2,\dots ,n-
      1\\m&=-\ell ,\dots ,\ell \\\end{aligned}}}  [{\begin
      {aligned}n&=1,2,3,\dots \\\ell &=0,1,2,\dots ,n-1\\m&=-\ell ,\dots ,\ell
      \\\end{aligned}}]
The generalized_Laguerre_polynomials are defined differently by different
authors. See main article on them and the hydrogen atom.
*** Two-electron atoms or ions[edit] ***
The equation for any two-electron system, such as the neutral helium_atom (He,
Z = 2   {\displaystyle Z=2}  [{\displaystyle Z=2}]), the negative hydrogen ion
(Hâ,     Z = 1   {\displaystyle Z=1}  [{\displaystyle Z=1}]), or the positive
lithium ion (Li+,     Z = 3   {\displaystyle Z=3}  [{\displaystyle Z=3}]) is:
[30]
         E &#x03C8; = &#x2212;  &#x210F;  2    [    1  2 &#x03BC;
      (   &#x2207;  1   2   +  &#x2207;  2   2    )  +   1 M    &#x2207;  1
      &#x22C5;  &#x2207;  2    ]  &#x03C8; +    e  2    4 &#x03C0;  &#x03B5;  0
      [    1  r  12     &#x2212; Z  (    1  r  1     +   1  r  2      )   ]
      &#x03C8;   {\displaystyle E\psi =-\hbar ^{2}\left[{\frac {1}{2\mu }}\left
      (\nabla _{1}^{2}+\nabla _{2}^{2}\right)+{\frac {1}{M}}\nabla _{1}\cdot
      \nabla _{2}\right]\psi +{\frac {e^{2}}{4\pi \varepsilon _{0}}}\left[
      {\frac {1}{r_{12}}}-Z\left({\frac {1}{r_{1}}}+{\frac {1}{r_
      {2}}}\right)\right]\psi }  [E\psi =-\hbar ^{2}\left[{\frac {1}{2\mu
      }}\left(\nabla _{1}^{2}+\nabla _{2}^{2}\right)+{\frac {1}{M}}\nabla _
      {1}\cdot \nabla _{2}\right]\psi +{\frac {e^{2}}{4\pi \varepsilon _
      {0}}}\left[{\frac {1}{r_{12}}}-Z\left({\frac {1}{r_{1}}}+{\frac {1}{r_
      {2}}}\right)\right]\psi ]
where r1 is the relative position of one electron (r1 = |r1| is its relative
magnitude), r2 is the relative position of the other electron (r2 = |r2| is the
magnitude), r12 = |r12| is the magnitude of the separation between them given
by
          |    r   12    |  =  |    r   2   &#x2212;   r   1    |
      {\displaystyle |\mathbf {r} _{12}|=|\mathbf {r} _{2}-\mathbf {r} _
      {1}|\,\!}  [|\mathbf {r} _{12}|=|\mathbf {r} _{2}-\mathbf {r} _{1}|\,\!]
Î¼ is again the two-body reduced mass of an electron with respect to the
nucleus of mass M, so this time
         &#x03BC; =     m  e   M    m  e   + M        {\displaystyle \mu =
      {\frac {m_{e}M}{m_{e}+M}}\,\!}  [\mu ={\frac {m_{e}M}{m_{e}+M}}\,\!]
and Z is the atomic_number for the element (not a quantum_number).
The cross-term of two Laplacians
           1 M    &#x2207;  1   &#x22C5;  &#x2207;  2       {\displaystyle
      {\frac {1}{M}}\nabla _{1}\cdot \nabla _{2}\,\!}  [{\frac {1}{M}}\nabla _
      {1}\cdot \nabla _{2}\,\!]
is known as the mass polarization term, which arises due to the motion of
atomic_nuclei. The wave function is a function of the two electron's positions:
         &#x03C8; = &#x03C8; (   r   1   ,   r   2   ) .   {\displaystyle \psi
      =\psi (\mathbf {r} _{1},\mathbf {r} _{2}).}  [\psi =\psi (\mathbf {r} _
      {1},\mathbf {r} _{2}).]
There is no closed form solution for this equation.
**** Time-dependent[edit] ****
This is the equation of motion for the quantum state. In the most general form,
it is written:[5]:143ff
         i &#x210F;   &#x2202;  &#x2202; t    &#x03A8; =    H &#x005E;
      &#x03A8; .   {\displaystyle i\hbar {\frac {\partial }{\partial t}}\Psi =
      {\hat {H}}\Psi .}  [i\hbar {\frac {\partial }{\partial t}}\Psi ={\hat
      {H}}\Psi .]
and the solution, the wave function, is a function of all the particle
coordinates of the system and time. Following are specific cases.
For one particle in one dimension, the Hamiltonian
            H &#x005E;    =       p &#x005E;     2    2 m    + V ( x , t )  ,
      p &#x005E;    = &#x2212; i &#x210F;   &#x2202;  &#x2202; x
      {\displaystyle {\hat {H}}={\frac {{\hat {p}}^{2}}{2m}}+V(x,t)\,,\quad
      {\hat {p}}=-i\hbar {\frac {\partial }{\partial x}}}  [{\hat {H}}={\frac {
      {\hat {p}}^{2}}{2m}}+V(x,t)\,,\quad {\hat {p}}=-i\hbar {\frac {\partial }
      {\partial x}}]
generates the equation:
         i &#x210F;   &#x2202;  &#x2202; t    &#x03A8; ( x , t ) = &#x2212;
      &#x210F;  2    2 m       &#x2202;  2    &#x2202;  x  2      &#x03A8; ( x
      , t ) + V ( x , t ) &#x03A8; ( x , t )   {\displaystyle i\hbar {\frac
      {\partial }{\partial t}}\Psi (x,t)=-{\frac {\hbar ^{2}}{2m}}{\frac
      {\partial ^{2}}{\partial x^{2}}}\Psi (x,t)+V(x,t)\Psi (x,t)}  [i\hbar
      {\frac {\partial }{\partial t}}\Psi (x,t)=-{\frac {\hbar ^{2}}{2m}}{\frac
      {\partial ^{2}}{\partial x^{2}}}\Psi (x,t)+V(x,t)\Psi (x,t)]
For N particles in one dimension, the Hamiltonian is:
            H &#x005E;    =  &#x2211;  n = 1   N         p &#x005E;     n   2
      2  m  n      + V (  x  1   ,  x  2   , &#x22EF;  x  N   , t )  ,      p
      &#x005E;     n   = &#x2212; i &#x210F;   &#x2202;  &#x2202;  x  n
      {\displaystyle {\hat {H}}=\sum _{n=1}^{N}{\frac {{\hat {p}}_{n}^{2}}{2m_
      {n}}}+V(x_{1},x_{2},\cdots x_{N},t)\,,\quad {\hat {p}}_{n}=-i\hbar {\frac
      {\partial }{\partial x_{n}}}}  [{\hat {H}}=\sum _{n=1}^{N}{\frac {{\hat
      {p}}_{n}^{2}}{2m_{n}}}+V(x_{1},x_{2},\cdots x_{N},t)\,,\quad {\hat {p}}_
      {n}=-i\hbar {\frac {\partial }{\partial x_{n}}}]
where the position of particle n is xn, generating the equation:
         i &#x210F;   &#x2202;  &#x2202; t    &#x03A8; (  x  1   ,  x  2
      &#x22EF;  x  N   , t ) = &#x2212;    &#x210F;  2   2    &#x2211;  n = 1
      N     1  m  n        &#x2202;  2    &#x2202;  x  n   2      &#x03A8; (  x
      1   ,  x  2   &#x22EF;  x  N   , t ) + V (  x  1   ,  x  2   &#x22EF;  x
      N   , t ) &#x03A8; (  x  1   ,  x  2   &#x22EF;  x  N   , t )  .
      {\displaystyle i\hbar {\frac {\partial }{\partial t}}\Psi (x_{1},x_
      {2}\cdots x_{N},t)=-{\frac {\hbar ^{2}}{2}}\sum _{n=1}^{N}{\frac {1}{m_
      {n}}}{\frac {\partial ^{2}}{\partial x_{n}^{2}}}\Psi (x_{1},x_{2}\cdots
      x_{N},t)+V(x_{1},x_{2}\cdots x_{N},t)\Psi (x_{1},x_{2}\cdots x_{N},t)\,.}
      [i\hbar {\frac {\partial }{\partial t}}\Psi (x_{1},x_{2}\cdots x_{N},t)=-
      {\frac {\hbar ^{2}}{2}}\sum _{n=1}^{N}{\frac {1}{m_{n}}}{\frac {\partial
      ^{2}}{\partial x_{n}^{2}}}\Psi (x_{1},x_{2}\cdots x_{N},t)+V(x_{1},x_
      {2}\cdots x_{N},t)\Psi (x_{1},x_{2}\cdots x_{N},t)\,.]
For one particle in three dimensions, the Hamiltonian is:
            H &#x005E;    =        p  &#x005E;    &#x22C5;     p  &#x005E;
      2 m    + V (  r  , t )  ,      p  &#x005E;    = &#x2212; i &#x210F;
      &#x2207;   {\displaystyle {\hat {H}}={\frac {{\hat {\mathbf {p} }}\cdot
      {\hat {\mathbf {p} }}}{2m}}+V(\mathbf {r} ,t)\,,\quad {\hat {\mathbf {p}
      }}=-i\hbar \nabla }  [{\hat {H}}={\frac {{\hat {\mathbf {p} }}\cdot {\hat
      {\mathbf {p} }}}{2m}}+V(\mathbf {r} ,t)\,,\quad {\hat {\mathbf {p} }}=-
      i\hbar \nabla ]
generating the equation:
         i &#x210F;   &#x2202;  &#x2202; t    &#x03A8; (  r  , t ) = &#x2212;
      &#x210F;  2    2 m     &#x2207;  2   &#x03A8; (  r  , t ) + V (  r  , t )
      &#x03A8; (  r  , t )   {\displaystyle i\hbar {\frac {\partial }{\partial
      t}}\Psi (\mathbf {r} ,t)=-{\frac {\hbar ^{2}}{2m}}\nabla ^{2}\Psi
      (\mathbf {r} ,t)+V(\mathbf {r} ,t)\Psi (\mathbf {r} ,t)}  [i\hbar {\frac
      {\partial }{\partial t}}\Psi (\mathbf {r} ,t)=-{\frac {\hbar ^{2}}
      {2m}}\nabla ^{2}\Psi (\mathbf {r} ,t)+V(\mathbf {r} ,t)\Psi (\mathbf {r}
      ,t)]
For N particles in three dimensions, the Hamiltonian is:
            H &#x005E;    =  &#x2211;  n = 1   N           p  &#x005E;     n
      &#x22C5;      p  &#x005E;     n     2  m  n      + V (   r   1   ,   r
      2   , &#x22EF;   r   N   , t )  ,       p  &#x005E;     n   = &#x2212; i
      &#x210F;  &#x2207;  n     {\displaystyle {\hat {H}}=\sum _{n=1}^{N}{\frac
      {{\hat {\mathbf {p} }}_{n}\cdot {\hat {\mathbf {p} }}_{n}}{2m_{n}}}+V
      (\mathbf {r} _{1},\mathbf {r} _{2},\cdots \mathbf {r} _{N},t)\,,\quad
      {\hat {\mathbf {p} }}_{n}=-i\hbar \nabla _{n}}  [{\hat {H}}=\sum _{n=1}^
      {N}{\frac {{\hat {\mathbf {p} }}_{n}\cdot {\hat {\mathbf {p} }}_{n}}{2m_
      {n}}}+V(\mathbf {r} _{1},\mathbf {r} _{2},\cdots \mathbf {r} _
      {N},t)\,,\quad {\hat {\mathbf {p} }}_{n}=-i\hbar \nabla _{n}]
where the position of particle n is rn, generating the equation:[5]:141
         i &#x210F;   &#x2202;  &#x2202; t    &#x03A8; (   r   1   ,   r   2
      , &#x22EF;   r   N   , t ) = &#x2212;    &#x210F;  2   2    &#x2211;  n =
      1   N     1  m  n      &#x2207;  n   2   &#x03A8; (   r   1   ,   r   2
      , &#x22EF;   r   N   , t ) + V (   r   1   ,   r   2   , &#x22EF;   r   N
      , t ) &#x03A8; (   r   1   ,   r   2   , &#x22EF;   r   N   , t )
      {\displaystyle i\hbar {\frac {\partial }{\partial t}}\Psi (\mathbf {r} _
      {1},\mathbf {r} _{2},\cdots \mathbf {r} _{N},t)=-{\frac {\hbar ^{2}}
      {2}}\sum _{n=1}^{N}{\frac {1}{m_{n}}}\nabla _{n}^{2}\Psi (\mathbf {r} _
      {1},\mathbf {r} _{2},\cdots \mathbf {r} _{N},t)+V(\mathbf {r} _
      {1},\mathbf {r} _{2},\cdots \mathbf {r} _{N},t)\Psi (\mathbf {r} _
      {1},\mathbf {r} _{2},\cdots \mathbf {r} _{N},t)}  [i\hbar {\frac
      {\partial }{\partial t}}\Psi (\mathbf {r} _{1},\mathbf {r} _{2},\cdots
      \mathbf {r} _{N},t)=-{\frac {\hbar ^{2}}{2}}\sum _{n=1}^{N}{\frac {1}{m_
      {n}}}\nabla _{n}^{2}\Psi (\mathbf {r} _{1},\mathbf {r} _{2},\cdots
      \mathbf {r} _{N},t)+V(\mathbf {r} _{1},\mathbf {r} _{2},\cdots \mathbf
      {r} _{N},t)\Psi (\mathbf {r} _{1},\mathbf {r} _{2},\cdots \mathbf {r} _
      {N},t)]
This last equation is in a very high dimension, so the solutions are not easy
to visualize.
***** Solution methods[edit] *****
 This article is in list format, but may read better as prose. You can help by
 converting_this_article, if appropriate. Editing_help is available. (October
 2016)
General techniques:
    * Separation of
      variables
    * Perturbation
      theory
    * The
      variational
      method        Methods for special cases:
    * Quantum_Monte     * List_of_quantum-mechanical_systems_with_analytical
      Carlo methods       solutions
    * Density           * HartreeâFock method and post_HartreeâFock methods
      functional
      theory
    * The WKB
      approximation
      and semi-
      classical
      expansion
***** Properties[edit] *****
The SchrÃ¶dinger equation has the following properties: some are useful, but
there are shortcomings. Ultimately, these properties arise from the Hamiltonian
used, and the solutions to the equation.
**** Linearity[edit] ****
See also: Linear_differential_equation
In the development above, the SchrÃ¶dinger equation was made to be linear for
generality, though this has other implications. If two wave functions Ï1 and
Ï2 are solutions, then so is any linear_combination of the two:
          &#x03C8; = a  &#x03C8;  1   + b  &#x03C8;  2      {\displaystyle
      \displaystyle \psi =a\psi _{1}+b\psi _{2}}  [\displaystyle \psi =a\psi _
      {1}+b\psi _{2}]
where a and b are any complex numbers (the sum can be extended for any number
of wave functions). This property allows superpositions_of_quantum_states to be
solutions of the SchrÃ¶dinger equation. Even more generally, it holds that a
general solution to the SchrÃ¶dinger equation can be found by taking a weighted
sum over all single state solutions achievable. For example, consider a wave
function Î¨(x, t) such that the wave function is a product of two functions:
one time independent, and one time dependent. If states of definite energy
found using the time independent SchrÃ¶dinger equation are given by ÏE(x) with
amplitude An and time dependent phase factor is given by
          e   &#x2212; i  E  n   t   /  &#x210F;   ,   {\displaystyle e^{{-iE_
      {n}t}/\hbar },}  [e^{{-iE_{n}t}/\hbar },]
then a valid general solution is
          &#x03A8; ( x , t ) =  &#x2211;  n    A  n    &#x03C8;   E  n     ( x
      )  e   &#x2212; i  E  n   t   /  &#x210F;   .    {\displaystyle
      \displaystyle \Psi (x,t)=\sum \limits _{n}A_{n}\psi _{E_{n}}(x)e^{{-iE_
      {n}t}/\hbar }.}  [\displaystyle \Psi (x,t)=\sum \limits _{n}A_{n}\psi _
      {E_{n}}(x)e^{{-iE_{n}t}/\hbar }.]
Additionally, the ability to scale solutions allows one to solve for a wave
function without normalizing it first. If one has a set of normalized solutions
Ïn, then
          &#x03A8; =  &#x2211;  n    A  n    &#x03C8;  n      {\displaystyle
      \displaystyle \Psi =\sum \limits _{n}A_{n}\psi _{n}}  [\displaystyle \Psi
      =\sum \limits _{n}A_{n}\psi _{n}]
can be normalized by ensuring that
           &#x2211;  n    |   A  n     |   2   = 1.    {\displaystyle
      \displaystyle \sum \limits _{n}|A_{n}|^{2}=1.}  [\displaystyle \sum
      \limits _{n}|A_{n}|^{2}=1.]
This is much more convenient than having to verify that
           &#x222B;  &#x2212; &#x221E;   &#x221E;    |  &#x03A8; ( x )   |   2
      d x =  &#x222B;  &#x2212; &#x221E;   &#x221E;   &#x03A8; ( x )  &#x03A8;
      &#x2217;   ( x )  d x = 1.    {\displaystyle \displaystyle \int \limits _
      {-\infty }^{\infty }|\Psi (x)|^{2}\,dx=\int \limits _{-\infty }^{\infty
      }\Psi (x)\Psi ^{*}(x)\,dx=1.}  [\displaystyle \int \limits _{-\infty }^
      {\infty }|\Psi (x)|^{2}\,dx=\int \limits _{-\infty }^{\infty }\Psi
      (x)\Psi ^{*}(x)\,dx=1.]
**** Momentum space SchrÃ¶dinger equation[edit] ****
The SchrÃ¶dinger equation     i &#x210F;  &#x2202;  t    |  &#x03C8; &#x27E9; =
H &#x005E;     |  &#x03C8; &#x27E9;   {\displaystyle i\hbar \partial _{t}|\psi
\rangle ={\hat {H}}|\psi \rangle }  [{\displaystyle i\hbar \partial _{t}|\psi
\rangle ={\hat {H}}|\psi \rangle }] is often presented in the position basis
form     i &#x210F;  &#x2202;  t   &#x03C8; ( x ) = &#x2212;    &#x210F;  2
2 m     &#x2207;  2   &#x03C8; ( x ) + V ( x ) &#x03C8; ( x )   {\displaystyle
i\hbar \partial _{t}\psi (x)=-{\frac {\hbar ^{2}}{2m}}\nabla ^{2}\psi (x)+V
(x)\psi (x)}  [{\displaystyle i\hbar \partial _{t}\psi (x)=-{\frac {\hbar ^{2}}
{2m}}\nabla ^{2}\psi (x)+V(x)\psi (x)}] (with     &#x27E8; x  |  &#x03C8;
&#x27E9; &#x2261; &#x03C8; ( x )   {\displaystyle \langle x|\psi \rangle \equiv
\psi (x)}  [{\displaystyle \langle x|\psi \rangle \equiv \psi (x)}]). But as a
vector operator equation it has a valid representation in any arbitrary
complete basis of kets in Hilbert_space. For example, in the momentum space
basis the equation reads
    i &#x210F;  &#x2202;  t   f ( p ) =    p  2    2 m    f ( p ) + (    V
&#x007E;    &#x2217; f ) ( p )    {\displaystyle \displaystyle i\hbar \partial
_{t}f(p)={\frac {p^{2}}{2m}}f(p)+({\tilde {V}}*f)(p)}  [{\displaystyle
\displaystyle i\hbar \partial _{t}f(p)={\frac {p^{2}}{2m}}f(p)+({\tilde {V}}*f)
(p)}]
where      |  p &#x27E9;   {\displaystyle |p\rangle }  [{\displaystyle
|p\rangle }] is the plane wave state of definite momentum     p
{\displaystyle p}  [p],     &#x27E8; p  |  &#x03C8; &#x27E9; &#x2261; f ( p ) =
&#x222B; &#x03C8; ( x )  e  &#x2212; i p x   d x   {\displaystyle \langle
p|\psi \rangle \equiv f(p)=\int \psi (x)e^{-ipx}dx}  [{\displaystyle \langle
p|\psi \rangle \equiv f(p)=\int \psi (x)e^{-ipx}dx}],        V &#x007E;
{\displaystyle {\tilde {V}}}  [{\displaystyle {\tilde {V}}}] is the Fourier
transform of     V   {\displaystyle V}  [V], and     &#x2217;   {\displaystyle
*}  [{\displaystyle *}] denotes Fourier_convolution.
In the 1D example with absence of a potential,        V &#x007E;    = 0
{\displaystyle {\tilde {V}}=0}  [{\displaystyle {\tilde {V}}=0}] (or similarly
V &#x007E;    ( k ) &#x221D; &#x03B4; ( k )   {\displaystyle {\tilde {V}}
(k)\propto \delta (k)}  [{\displaystyle {\tilde {V}}(k)\propto \delta (k)}] in
the case of a background potential constant throughout space), each stationary
state of energy     &#x210F; &#x03C9; =  q  2    /  2 m   {\displaystyle \hbar
\omega =q^{2}/2m}  [{\displaystyle \hbar \omega =q^{2}/2m}] is of the form
    f  q   ( p ) = (  c  +   &#x03B4; ( p &#x2212; q ) +  c  &#x2212;
&#x03B4; ( p + q ) )  e  &#x2212; i &#x03C9; t     {\displaystyle f_{q}(p)=(c_
{+}\delta (p-q)+c_{-}\delta (p+q))e^{-i\omega t}}  [{\displaystyle f_{q}(p)=(c_
{+}\delta (p-q)+c_{-}\delta (p+q))e^{-i\omega t}}]
for arbitrary complex coefficients      c  &#x00B1;     {\displaystyle c_{\pm
}}  [{\displaystyle c_{\pm }}]. Such a wave function, as expected in free
space, is a superposition of plane waves moving right and left with momenta
&#x00B1; q   {\displaystyle \pm q}  [{\displaystyle \pm q}]; upon momentum
measurement the state would collapse to one of definite momentum     &#x00B1; q
{\displaystyle \pm q}  [{\displaystyle \pm q}] with probability     &#x221D;  |
c  &#x00B1;     |   2     {\displaystyle \propto |c_{\pm }|^{2}}  [
{\displaystyle \propto |c_{\pm }|^{2}}].
A version of the momentum space SchrÃ¶dinger equation is often used in solid-
state_physics, as Bloch's_theorem ensures the periodic crystal lattice
potential couples     f ( p )   {\displaystyle f(p)}  [{\displaystyle f(p)}]
with     f ( p + K )   {\displaystyle f(p+K)}  [{\displaystyle f(p+K)}] for
only discrete reciprocal_lattice vectors     K   {\displaystyle K}  [K]. This
makes it convenient to solve the momentum space SchrÃ¶dinger equation at each
point in the Brillouin_zone independently of the other points in the Brillouin
zone.
**** Real energy eigenstates[edit] ****
For the time-independent equation, an additional feature of linearity follows:
if two wave functions Ï1 and ψ2 are solutions to the time-independent equation
with the same energy E, then so is any linear combination:
            H &#x005E;    ( a  &#x03C8;  1   + b  &#x03C8;  2   ) = a    H
      &#x005E;     &#x03C8;  1   + b    H &#x005E;     &#x03C8;  2   = E ( a
      &#x03C8;  1   + b  &#x03C8;  2   ) .   {\displaystyle {\hat {H}}(a\psi _
      {1}+b\psi _{2})=a{\hat {H}}\psi _{1}+b{\hat {H}}\psi _{2}=E(a\psi _
      {1}+b\psi _{2}).}  [{\hat {H}}(a\psi _{1}+b\psi _{2})=a{\hat {H}}\psi _
      {1}+b{\hat {H}}\psi _{2}=E(a\psi _{1}+b\psi _{2}).]
Two different solutions with the same energy are called degenerate.[32]
In an arbitrary potential, if a wave function Ï solves the time-independent
equation, so does its complex_conjugate, denoted Ï*. By taking linear
combinations, the real and imaginary parts of Ï are each solutions. If there
is no degeneracy they can only differ by a factor.
In the time-dependent equation, complex conjugate waves move in opposite
directions. If Î¨(x, t) is one solution, then so is Î¨*(x, ât). The symmetry
of complex conjugation is called time-reversal_symmetry.
**** Space and time derivatives[edit] ****
Continuity of the wave function and its first spatial derivative (in the x
direction, y and z coordinates not shown), at some time t.
The SchrÃ¶dinger equation is first order in time and second in space, which
describes the time evolution of a quantum state (meaning it determines the
future amplitude from the present).
Explicitly for one particle in 3-dimensional Cartesian coordinates â the
equation is
         i &#x210F;    &#x2202; &#x03A8;   &#x2202; t    = &#x2212;    &#x210F;
      2    2 m     (      &#x2202;  2   &#x03A8;   &#x2202;  x  2      +
      &#x2202;  2   &#x03A8;   &#x2202;  y  2      +     &#x2202;  2   &#x03A8;
      &#x2202;  z  2       )  + V ( x , y , z , t ) &#x03A8; .
      {\displaystyle i\hbar {\partial \Psi \over \partial t}=-{\hbar ^{2} \over
      2m}\left({\partial ^{2}\Psi \over \partial x^{2}}+{\partial ^{2}\Psi
      \over \partial y^{2}}+{\partial ^{2}\Psi \over \partial z^{2}}\right)+V
      (x,y,z,t)\Psi .\,\!}  [i\hbar {\partial \Psi  \over \partial t}=-{\hbar ^
      {2} \over 2m}\left({\partial ^{2}\Psi  \over \partial x^{2}}+{\partial ^
      {2}\Psi  \over \partial y^{2}}+{\partial ^{2}\Psi  \over \partial z^
      {2}}\right)+V(x,y,z,t)\Psi .\,\!]
The first time partial derivative implies the initial value (at t = 0) of the
wave function
         &#x03A8; ( x , y , z , 0 )     {\displaystyle \Psi (x,y,z,0)\,\!}
      [\Psi (x,y,z,0)\,\!]
is an arbitrary constant. Likewise â the second order derivatives with
respect to space implies the wave function and its first order spatial
derivatives
              &#x03A8; (  x  b   ,  y  b   ,  z  b   , t )        &#x2202;
      &#x2202; x    &#x03A8; (  x  b   ,  y  b   ,  z  b   , t )    &#x2202;
      &#x2202; y    &#x03A8; (  x  b   ,  y  b   ,  z  b   , t )    &#x2202;
      &#x2202; z    &#x03A8; (  x  b   ,  y  b   ,  z  b   , t )
      {\displaystyle {\begin{aligned}&\Psi (x_{b},y_{b},z_{b},t)\\&{\frac
      {\partial }{\partial x}}\Psi (x_{b},y_{b},z_{b},t)\quad {\frac {\partial
      }{\partial y}}\Psi (x_{b},y_{b},z_{b},t)\quad {\frac {\partial }{\partial
      z}}\Psi (x_{b},y_{b},z_{b},t)\end{aligned}}\,\!}  [{\begin{aligned}&\Psi
      (x_{b},y_{b},z_{b},t)\\&{\frac {\partial }{\partial x}}\Psi (x_{b},y_
      {b},z_{b},t)\quad {\frac {\partial }{\partial y}}\Psi (x_{b},y_{b},z_
      {b},t)\quad {\frac {\partial }{\partial z}}\Psi (x_{b},y_{b},z_{b},t)\end
      {aligned}}\,\!]
are all arbitrary constants at a given set of points, where xb, yb, zb are a
set of points describing boundary b (derivatives are evaluated at the
boundaries). Typically there are one or two boundaries, such as the step
potential and particle_in_a_box respectively.
As the first order derivatives are arbitrary, the wave function can be a
continuously_differentiable_function of space, since at any boundary the
gradient of the wave function can be matched.
On the contrary, wave equations in physics are usually second order in time,
notable are the family of classical wave_equations and the quantum
KleinâGordon_equation.
**** Local conservation of probability[edit] ****
Main articles: Probability_current and Continuity_equation
The SchrÃ¶dinger equation is consistent with probability_conservation.
Multiplying the SchrÃ¶dinger equation on the right by the complex conjugate
wave function, and multiplying the wave function to the left of the complex
conjugate of the SchrÃ¶dinger equation, and subtracting, gives the continuity
equation for probability:[42]
           &#x2202;  &#x2202; t    &#x03C1;  (   r  , t  )  + &#x2207; &#x22C5;
      j  = 0 ,   {\displaystyle {\partial \over \partial t}\rho \left(\mathbf
      {r} ,t\right)+\nabla \cdot \mathbf {j} =0,}  [{\partial  \over \partial
      t}\rho \left(\mathbf {r} ,t\right)+\nabla \cdot \mathbf {j} =0,]
where
         &#x03C1; =  |  &#x03A8;   |   2   =  &#x03A8;  &#x2217;   (  r  , t )
      &#x03A8; (  r  , t )     {\displaystyle \rho =|\Psi |^{2}=\Psi ^{*}
      (\mathbf {r} ,t)\Psi (\mathbf {r} ,t)\,\!}  [\rho =|\Psi |^{2}=\Psi ^{*}
      (\mathbf {r} ,t)\Psi (\mathbf {r} ,t)\,\!]
is the probability_density (probability per unit volume, * denotes complex
conjugate), and
          j  =   1  2 m     (   &#x03A8;  &#x2217;       p  &#x005E;
      &#x03A8; &#x2212; &#x03A8;     p  &#x005E;     &#x03A8;  &#x2217;    )
      {\displaystyle \mathbf {j} ={1 \over 2m}\left(\Psi ^{*}{\hat {\mathbf {p}
      }}\Psi -\Psi {\hat {\mathbf {p} }}\Psi ^{*}\right)\,\!}  [\mathbf {j} ={1
      \over 2m}\left(\Psi ^{*}{\hat {\mathbf {p} }}\Psi -\Psi {\hat {\mathbf
      {p} }}\Psi ^{*}\right)\,\!]
is the probability_current (flow per unit area).
Hence predictions from the SchrÃ¶dinger equation do not violate probability
conservation.
**** Positive energy[edit] ****
If the potential is bounded from below, meaning there is a minimum value of
potential energy, the eigenfunctions of the SchrÃ¶dinger equation have energy
which is also bounded from below. This can be seen most easily by using the
variational_principle, as follows. (See also below).
For any linear operator Ã bounded from below, the eigenvector with the
smallest eigenvalue is the vector Ï that minimizes the quantity
         &#x27E8; &#x03C8;  |     A &#x005E;     |  &#x03C8; &#x27E9;
      {\displaystyle \langle \psi |{\hat {A}}|\psi \rangle }  [\langle \psi |
      {\hat {A}}|\psi \rangle ]
over all Ï which are normalized.[42] In this way, the smallest eigenvalue is
expressed through the variational_principle. For the SchrÃ¶dinger Hamiltonian
Ä¤ bounded from below, the smallest eigenvalue is called the ground state
energy. That energy is the minimum value of
         &#x27E8; &#x03C8;  |     H &#x005E;     |  &#x03C8; &#x27E9; =
      &#x222B;  &#x03C8;  &#x2217;   (  r  )  [  &#x2212;    &#x210F;  2    2 m
      &#x2207;  2   &#x03C8; (  r  ) + V (  r  ) &#x03C8; (  r  )  ]   d  3
      r  = &#x222B;  [     &#x210F;  2    2 m     |  &#x2207; &#x03C8;   |   2
      + V (  r  )  |  &#x03C8;   |   2    ]   d  3    r  = &#x27E8;    H
      &#x005E;    &#x27E9;   {\displaystyle \langle \psi |{\hat {H}}|\psi
      \rangle =\int \psi ^{*}(\mathbf {r} )\left[-{\frac {\hbar ^{2}}
      {2m}}\nabla ^{2}\psi (\mathbf {r} )+V(\mathbf {r} )\psi (\mathbf {r}
      )\right]d^{3}\mathbf {r} =\int \left[{\frac {\hbar ^{2}}{2m}}|\nabla \psi
      |^{2}+V(\mathbf {r} )|\psi |^{2}\right]d^{3}\mathbf {r} =\langle {\hat
      {H}}\rangle }  [\langle \psi |{\hat {H}}|\psi \rangle =\int \psi ^{*}
      (\mathbf {r} )\left[-{\frac {\hbar ^{2}}{2m}}\nabla ^{2}\psi (\mathbf {r}
      )+V(\mathbf {r} )\psi (\mathbf {r} )\right]d^{3}\mathbf {r} =\int \left[
      {\frac {\hbar ^{2}}{2m}}|\nabla \psi |^{2}+V(\mathbf {r} )|\psi |^
      {2}\right]d^{3}\mathbf {r} =\langle {\hat {H}}\rangle ]
(using integration_by_parts). Due to the complex_modulus of Ï2 (which is
positive definite), the right hand side is always greater than the lowest value
of V(x). In particular, the ground state energy is positive when V(x) is
everywhere positive.
For potentials which are bounded below and are not infinite over a region,
there is a ground state which minimizes the integral above. This lowest energy
wave function is real and positive definite â meaning the wave function can
increase and decrease, but is positive for all positions. It physically cannot
be negative: if it were, smoothing out the bends at the sign change (to
minimize the wave function) rapidly reduces the gradient contribution to the
integral and hence the kinetic energy, while the potential energy changes
linearly and less quickly. The kinetic and potential energy are both changing
at different rates, so the total energy is not constant, which can't happen
(conservation). The solutions are consistent with SchrÃ¶dinger equation if this
wave function is positive definite.
The lack of sign changes also shows that the ground state is nondegenerate,
since if there were two ground states with common energy E, not proportional to
each other, there would be a linear combination of the two that would also be a
ground state resulting in a zero solution.
**** Analytic continuation to diffusion[edit] ****
See also: Path_integral_formulation_(The_SchrÃ¶dinger_equation)
The above properties (positive definiteness of energy) allow the analytic
continuation of the SchrÃ¶dinger equation to be identified as a stochastic
process. This can be interpreted as the HuygensâFresnel_principle applied to
De Broglie waves; the spreading wavefronts are diffusive probability
amplitudes.[42] For a free particle (not subject to a potential) in a random
walk, substituting Ï = it into the time-dependent SchrÃ¶dinger equation gives:
[43]
           &#x2202;  &#x2202; &#x03C4;    X (  r  , &#x03C4; ) =   &#x210F;  2
      m     &#x2207;  2   X (  r  , &#x03C4; )  ,  X (  r  , &#x03C4; ) =
      &#x03A8; (  r  , &#x03C4;  /  i )   {\displaystyle {\partial \over
      \partial \tau }X(\mathbf {r} ,\tau )={\frac {\hbar }{2m}}\nabla ^{2}X
      (\mathbf {r} ,\tau )\,,\quad X(\mathbf {r} ,\tau )=\Psi (\mathbf {r}
      ,\tau /i)}  [{\partial  \over \partial \tau }X(\mathbf {r} ,\tau )={\frac
      {\hbar }{2m}}\nabla ^{2}X(\mathbf {r} ,\tau )\,,\quad X(\mathbf {r} ,\tau
      )=\Psi (\mathbf {r} ,\tau /i)]
which has the same form as the diffusion_equation, with diffusion coefficient
Ä§/2m.
**** Regularity[edit] ****
On the space      L  2     {\displaystyle L^{2}}  [L^{2}] of square-integrable
densities, the SchrÃ¶dinger semigroup      e  i t    H &#x005E;
{\displaystyle e^{it{\hat {H}}}}  [{\displaystyle e^{it{\hat {H}}}}] is a
unitary evolution, and therefore surjective. The flows satisfy the SchrÃ¶dinger
equation     i  &#x2202;  t   u =    H &#x005E;    u   {\displaystyle i\partial
_{t}u={\hat {H}}u}  [{\displaystyle i\partial _{t}u={\hat {H}}u}], where the
derivative is taken in the distribution sense. However, since        H &#x005E;
{\displaystyle {\hat {H}}}  [{\hat {H}}] for most physically reasonable
Hamiltonians (e.g., the Laplace_operator, possibly modified by a potential) is
unbounded in      L  2     {\displaystyle L^{2}}  [L^{2}], this shows that the
semigroup flows lack Sobolev regularity in general. Instead, solutions of the
SchrÃ¶dinger equation satisfy a Strichartz_estimate.
***** Relativistic quantum mechanics[edit] *****
Relativistic_quantum_mechanics is obtained where quantum mechanics and special
relativity simultaneously apply. In general, one wishes to build relativistic
wave_equations from the relativistic energyâmomentum_relation
          E  2   = ( p c  )  2   + (  m  0    c  2    )  2    ,
      {\displaystyle E^{2}=(pc)^{2}+(m_{0}c^{2})^{2}\,,}  [E^{2}=(pc)^{2}+(m_
      {0}c^{2})^{2}\,,]
instead of classical energy equations. The KleinâGordon_equation and the
Dirac_equation are two such equations. The KleinâGordon equation,
           1  c  2        &#x2202;  2    &#x2202;  t  2      &#x03C8; &#x2212;
      &#x2207;  2   &#x03C8; +     m  2    c  2     &#x210F;  2     &#x03C8; =
      0.   {\displaystyle {\frac {1}{c^{2}}}{\frac {\partial ^{2}}{\partial t^
      {2}}}\psi -\nabla ^{2}\psi +{\frac {m^{2}c^{2}}{\hbar ^{2}}}\psi =0.}  [
      {\frac {1}{c^{2}}}{\frac {\partial ^{2}}{\partial t^{2}}}\psi -\nabla ^
      {2}\psi +{\frac {m^{2}c^{2}}{\hbar ^{2}}}\psi =0.],
was the first such equation to be obtained, even before the nonrelativistic
one, and applies to massive spinless particles. The Dirac equation arose from
taking the "square root" of the KleinâGordon equation by factorizing the
entire relativistic wave operator into a product of two operators â one of
these is the operator for the entire Dirac equation. Entire Dirac equation:
          (  &#x03B2; m  c  2   + c  (   &#x2211;  n  =  &#x2061; 1   3
      &#x03B1;  n    p  n    )   )  &#x03C8; = i &#x210F;    &#x2202; &#x03C8;
      &#x2202; t      {\displaystyle \left(\beta mc^{2}+c\left(\sum _{n\mathop
      {=} 1}^{3}\alpha _{n}p_{n}\right)\right)\psi =i\hbar {\frac {\partial
      \psi }{\partial t}}}  [{\displaystyle \left(\beta mc^{2}+c\left(\sum _
      {n\mathop {=} 1}^{3}\alpha _{n}p_{n}\right)\right)\psi =i\hbar {\frac
      {\partial \psi }{\partial t}}}]
The general form of the SchrÃ¶dinger equation remains true in relativity, but
the Hamiltonian is less obvious. For example, the Dirac Hamiltonian for a
particle of mass m and electric charge q in an electromagnetic field (described
by the electromagnetic_potentials Ï and A) is:
             H &#x005E;     Dirac   =  &#x03B3;  0    [  c  &#x03B3;  &#x22C5;
      (      p  &#x005E;    &#x2212; q  A   )  + m  c  2   +  &#x03B3;  0   q
      &#x03D5;  ]   ,   {\displaystyle {\hat {H}}_{\text{Dirac}}=\gamma ^
      {0}\left[c{\boldsymbol {\gamma }}\cdot \left({\hat {\mathbf {p} }}-
      q\mathbf {A} \right)+mc^{2}+\gamma ^{0}q\phi \right]\,,}  [{\hat {H}}_
      {\text{Dirac}}=\gamma ^{0}\left[c{\boldsymbol {\gamma }}\cdot \left({\hat
      {\mathbf {p} }}-q\mathbf {A} \right)+mc^{2}+\gamma ^{0}q\phi \right]\,,]
in which the Î³ = (Î³1, Î³2, Î³3) and Î³0 are the Dirac gamma_matrices related
to the spin of the particle. The Dirac equation is true for all spin-
&#x200b;1⁄2 particles, and the solutions to the equation are 4-component spinor
fields with two components corresponding to the particle and the other two for
the antiparticle.
For the KleinâGordon equation, the general form of the SchrÃ¶dinger equation
is inconvenient to use, and in practice the Hamiltonian is not expressed in an
analogous way to the Dirac Hamiltonian. The equations for relativistic quantum
fields can be obtained in other ways, such as starting from a Lagrangian
density and using the EulerâLagrange_equations for fields, or use the
representation_theory_of_the_Lorentz_group in which certain representations can
be used to fix the equation for a free particle of given spin (and mass).
In general, the Hamiltonian to be substituted in the general SchrÃ¶dinger
equation is not just a function of the position and momentum operators (and
possibly time), but also of spin matrices. Also, the solutions to a
relativistic wave equation, for a massive particle of spin s, are complex-
valued 2(2s + 1)-component spinor_fields.
***** Quantum field theory[edit] *****
The general equation is also valid and used in quantum_field_theory, both in
relativistic and nonrelativistic situations. However, the solution Ï is no
longer interpreted as a "wave", but should be interpreted as an operator acting
on states existing in a Fock_space.[citation_needed]
***** First order form[edit] *****
The SchrÃ¶dinger equation can also be derived from a first order form[44][45]
[46] similar to the manner in which the KleinâGordon_equation can be derived
from the Dirac_equation. In 1D the first order equation is given by
             &#x2212; i  &#x2202;  z   &#x03C8; = ( i &#x03B7;  &#x2202;  t   +
      &#x03B7;  &#x2020;   m ) &#x03C8;       {\displaystyle {\begin{aligned}-
      i\partial _{z}\psi =(i\eta \partial _{t}+\eta ^{\dagger }m)\psi \end
      {aligned}}}
      [{\displaystyle {\begin{aligned}-i\partial _{z}\psi =(i\eta \partial _
      {t}+\eta ^{\dagger }m)\psi \end{aligned}}}]
This equation allows for the inclusion of spin in nonrelativistic quantum
mechanics. Squaring the above equation yields the SchrÃ¶dinger equation in 1D.
The matrices     &#x03B7;   {\displaystyle \eta }  [\eta ] obey the following
properties
              &#x03B7;  2   = 0     (  &#x03B7;  &#x2020;    )  2   = 0
      {  &#x03B7; ,  &#x03B7;  &#x2020;    }  = 2 I       {\displaystyle
      {\begin{aligned}\eta ^{2}=0\\(\eta ^{\dagger })^{2}=0\\\left\lbrace \eta
      ,\eta ^{\dagger }\right\rbrace =2I\end{aligned}}}
      [{\displaystyle {\begin{aligned}\eta ^{2}=0\\(\eta ^{\dagger })^
      {2}=0\\\left\lbrace \eta ,\eta ^{\dagger }\right\rbrace =2I\end
      {aligned}}}]
The 3 dimensional version of the equation is given by
             &#x2212; i  &#x03B3;  i    &#x2202;  i   &#x03C8; = ( i &#x03B7;
      &#x2202;  t   +  &#x03B7;  &#x2020;   m ) &#x03C8;       {\displaystyle
      {\begin{aligned}-i\gamma _{i}\partial _{i}\psi =(i\eta \partial _{t}+\eta
      ^{\dagger }m)\psi \end{aligned}}}
      [{\displaystyle {\begin{aligned}-i\gamma _{i}\partial _{i}\psi =(i\eta
      \partial _{t}+\eta ^{\dagger }m)\psi \end{aligned}}}]
Here     &#x03B7; = (  &#x03B3;  0   + i  &#x03B3;  5   )  /    2
{\displaystyle \eta =(\gamma _{0}+i\gamma _{5})/{\sqrt {2}}}  [{\displaystyle
\eta =(\gamma _{0}+i\gamma _{5})/{\sqrt {2}}}] is a     4 &#x00D7; 4
{\displaystyle 4\times 4}  [4 \times 4] nilpotent_matrix and      &#x03B3;  i
{\displaystyle \gamma _{i}}  [{\displaystyle \gamma _{i}}] are the Dirac gamma
matrices (    i = 1 , 2 , 3   {\displaystyle i=1,2,3}  [i=1,2,3]). The
SchrÃ¶dinger equation in 3D can be obtained by squaring the above equation. In
the nonrelativistic limit     E &#x2212; m &#x2243;  E &#x2032;
{\displaystyle E-m\simeq E'}  [{\displaystyle E-m\simeq E'}] and     E + m
&#x2243; 2 m   {\displaystyle E+m\simeq 2m}  [{\displaystyle E+m\simeq 2m}],
the above equation can be derived from the Dirac equation.[45]
***** See also[edit] *****
    * Eckhaus_equation
    * Fractional_SchrÃ¶dinger_equation
    * List_of_quantum-mechanical_systems_with_analytical_solutions
    * Logarithmic_SchrÃ¶dinger_equation
    * Nonlinear_SchrÃ¶dinger_equation
    * Quantum_carpet
    * Quantum_revival
    * Relation_between_SchrÃ¶dinger's_equation_and_the_path_integral
      formulation_of_quantum_mechanics
    * SchrÃ¶dinger_field
    * SchrÃ¶dinger_picture
    * SchrÃ¶dinger's_cat
    * Theoretical_and_experimental_justification_for_the_SchrÃ¶dinger_equation
***** Notes[edit] *****
   1. ^ While this is the most famous form of Newton's second law, it is not
      the most general, being valid only for objects of constant mass. Newton's
      second law reads      F  =   d  d t    ( m  v  )   {\displaystyle \mathbf
      {F} ={\frac {d}{dt}}(m\mathbf {v} )}  [{\displaystyle \mathbf {F} ={\frac
      {d}{dt}}(m\mathbf {v} )}], the net force acting on a body is equal to the
      total time derivative of the total momentum of that body.
   2. ^ For a charged particle moving under the influence of a magnetic field,
      see the Pauli_equation.
   3. ^ In chemistry, stationary states are atomic and molecular orbitals.
***** References[edit] *****
   1. ^Griffiths, David J. (2004), Introduction to Quantum Mechanics (2nd ed.),
      Prentice Hall, ISBN 978-0-13-111892-8
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
   3. ^"Physicist_Erwin_SchrÃ¶dinger's_Google_doodle_marks_quantum_mechanics
      work". The_Guardian. 13 August 2013. Retrieved 25 August 2013.
   4. ^ SchrÃ¶dinger, E. (1926). "An_Undulatory_Theory_of_the_Mechanics_of
      Atoms_and_Molecules" (PDF). Physical_Review. 28 (6): 1049â1070.
      Bibcode:1926PhRv...28.1049S. doi:10.1103/PhysRev.28.1049. Archived from
      the_original (PDF) on 17 December 2008.
   5. ^Laloe, Franck (2012), Do We Really Understand Quantum Mechanics,
      Cambridge University Press, ISBN 978-1-107-02501-1
   6. ^ a b c d e Shankar, R. (1943). Principles of Quantum Mechanics (2nd
      ed.). Kluwer Academic/Plenum Publishers. ISBN 978-0-306-44790-7.
   7. ^ "Schrodinger_equation". Hyperphysics. Department of Physics and
      Astronomy, George State University.
   8. ^Sakurai, J. J. (1995). Modern Quantum Mechanics. Reading, Massachusetts:
      Addison-Wesley. p. 68.
   9. ^Nouredine Zettili (17 February 2009). Quantum Mechanics: Concepts and
      Applications. John Wiley & Sons. ISBN 978-0-470-02678-6.
  10. ^Ballentine, Leslie (1998), Quantum Mechanics: A Modern Development,
      World Scientific Publishing Co., ISBN 978-9810241056
  11. ^SchrÃ¶dinger,_Erwin (1995). The interpretation of quantum mechanics:
      Dublin seminars (1949â1955) and other unpublished essays. Ox Bow Press.
      ISBN 9781881987086.
  12. ^ David Deutsch, The Beginning of Infinity, page 310
  13. ^Barrett,_Jeffrey_A. (1999). The Quantum Mechanics of Minds and Worlds.
      Oxford_University_Press. p. 63. ISBN 9780191583254.
  14. ^ de Broglie, L. (1925). "Recherches_sur_la_thÃ©orie_des_quanta" [On the
      Theory of Quanta] (PDF). Annales_de_Physique. 10 (3): 22â128. Bibcode:
      1925AnPh...10...22D. doi:10.1051/anphys/192510030022. Archived from the
      original (PDF) on 9 May 2009.
  15.  .
  16. ^Weissman, M.B.; V. V. Iliev; I. Gutman (2008). "A pioneer remembered:
      biographical notes about Arthur Constant Lunn". Communications in
      Mathematical and in Computer Chemistry. 59 (3): 687â708.
  17. ^Kamen, Martin D. (1985). Radiant Science, Dark Politics. Berkeley and
      Los Angeles, California: University of California Press. pp. 29â32.
      ISBN 978-0-520-04929-1.
  18. ^ Schrodinger, E. (1984). Collected papers. Friedrich Vieweg und Sohn.
      ISBN 978-3-7001-0573-2.
  19.  See introduction to first 1926 paper.
  20. ^ a b Encyclopaedia of Physics (2nd Edition), R. G. Lerner, G. L. Trigg,
      VHC publishers, 1991, (Verlagsgesellschaft) 3-527-26954-1, (VHC Inc.)
  21. ISBN 0-89573-752-3
  22. ^ Sommerfeld, A. (1919). Atombau und Spektrallinien. Braunschweig:
      Friedrich Vieweg und Sohn. ISBN 978-3-87144-484-5.
  23. ^ For an English source, seeHaar, T. "The Old Quantum Theory".
  24. ^ Rhodes, R. (1986). Making of the Atomic Bomb. Touchstone. ISBN 978-0-
      671-44133-3.
  25. ^ a bErwin SchrÃ¶dinger (1982). Collected Papers on Wave Mechanics: Third
      Edition. American Mathematical Soc. ISBN 978-0-8218-3524-1.
  26. ^SchrÃ¶dinger, E. (1926). "Quantisierung_als_Eigenwertproblem;_von_Erwin
      SchrÃ¶dinger". Annalen_der_Physik. 384 (4): 361â377. Bibcode:
      1926AnP...384..361S. doi:10.1002/andp.19263840404.
  27. ^ Erwin SchrÃ¶dinger, "The Present situation in Quantum Mechanics", p. 9
      of 22. The English version was translated by John D. Trimmer. The
      translation first appeared first in Proceedings of the American
      Philosophical Society, 124, 323â38. It later appeared as Section I.11
      of Part I of Quantum Theory and Measurement by J. A. Wheeler and W. H.
      Zurek, eds., Princeton University Press, New Jersey 1983.
  28. ^ Einstein, A.; et al. "Letters on Wave Mechanics:
      SchrodingerâPlanckâEinsteinâLorentz".
  29. ^ a b c Moore, W.J. (1992). SchrÃ¶dinger: Life and Thought. Cambridge
      University_Press. ISBN 978-0-521-43767-7.
  30. ^ It is clear that even in his last year of life, as shown in a letter to
      Max Born, that SchrÃ¶dinger never accepted the Copenhagen interpretation.
      [25]:220
  31. ^ a b Molecular Quantum Mechanics Parts I and II: An Introduction to
      Quantum Chemistry (Volume 1), P. W. Atkins, Oxford University Press,
      1977,
  32. ISBN 0-19-855129-0
  33. ^ The New Quantum Universe, T. Hey, P. Walters, Cambridge University
      Press, 2009,
  34. ISBN 978-0-521-56457-1
  35. ^ a b c d Quanta: A handbook of concepts, P. W. Atkins, Oxford University
      Press, 1974,
  36. ISBN 0-19-855493-1
  37. ^ a b Physics of Atoms and Molecules, B. H. Bransden, C. J. Joachain,
      Longman, 1983,
  38. ISBN 0-582-44401-2
  39. ^ a b Quantum Physics of Atoms, Molecules, Solids, Nuclei and Particles
      (2nd Edition), R. Resnick, R. Eisberg, John Wiley & Sons, 1985,
  40. ISBN 978-0-471-87373-0
  41. ^ a b c Quantum Mechanics Demystified, D. McMahon, McGraw Hill (USA),
      2006,
  42. ISBN 0-07-145546-9
  43. ^ a b Analytical Mechanics, L. N. Hand, J. D. Finch, Cambridge University
      Press, 2008,
  44. ISBN 978-0-521-57572-0
  45. ^ Hall_2013 Section 3.7.5
  46. ^ Hall_2013 p. 78
  47. ^N. Zettili (24 February 2009). Quantum Mechanics: Concepts and
      Applications (2nd ed.). p. 458. ISBN 978-0-470-02679-3.
  48. ^ Physical Chemistry, P. W. Atkins, Oxford University Press, 1978,
  49. ISBN 0-19-855148-7
  50. ^ Solid State Physics (2nd Edition), J. R. Hook, H. E. Hall, Manchester
      Physics Series, John Wiley & Sons, 2010,
  51. ISBN 978-0-471-92804-1
  52. ^Townsend, John S. (2012). "Chapter 7: The One-Dimensional Harmonic
      Oscillator". A Modern Approach to Quantum Mechanics. University Science
      Books. pp. 247â250, 254â5, 257, 272. ISBN 978-1-891389-78-8.
  53. ^ Physics for Scientists and Engineers â with Modern Physics (6th
      Edition), P. A. Tipler, G. Mosca, Freeman, 2008,
  54. ISBN 0-7167-8964-7
  55. ^David Griffiths (2008). Introduction_to_elementary_particles. Wiley-VCH.
      pp. 162â. ISBN 978-3-527-40601-2. Retrieved 27 June 2011.
  56. ^ a b c Quantum Mechanics, E. Abers, Pearson Ed., Addison Wesley,
      Prentice Hall Inc, 2004,
  57. ISBN 978-0-13-146100-0
  58. ^Baeumer, Boris; Meerschaert, Mark M.; Naber, Mark (2010). "Stochastic
      models_for_relativistic_diffusion" (PDF). Physical Review E. 82 (1 Pt 1):
      011132. Bibcode:2010PhRvE..82a1132B. doi:10.1103/PhysRevE.82.011132.
      PMID 20866590.
  59. ^Ajaib, Muhammad Adeel (2015). "A Fundamental Form of the SchrÃ¶dinger
      Equation". Found. Phys. 45 (12): 1586â1598. arXiv:1502.04274. Bibcode:
      2015FoPh...45.1586A. doi:10.1007/s10701-015-9944-z.
  60. ^ a bAjaib, Muhammad Adeel (2016). "Non-Relativistic_Limit_of_the_Dirac
      Equation". International Journal of Quantum Foundations.
  61. ^LÃ©vy-Leblond, J-.M. (1967). "Nonrelativistic_particles_and_wave
      equations". Commun. Math. Phys. 6 (4): 286â311. Bibcode:
      1967CMaPh...6..286L. doi:10.1007/BF01646020.
***** Further reading[edit] *****
    * P._A._M._Dirac (1958). The_Principles_of_Quantum_Mechanics (4th ed.).
      Oxford University Press.

ISBN 0-198-51208-2.
B.H. Bransden & C.J. Joachain (2000). Quantum Mechanics (2nd ed.). Prentice
Hall PTR. ISBN 978-0-582-35691-7.
David_J._Griffiths (2004). Introduction to Quantum Mechanics (2nd ed.).
Benjamin Cummings. ISBN 978-0-13-124405-4.
Hall, Brian C. (2013), Quantum Theory for Mathematicians, Graduate Texts in
Mathematics, 267, Springer, ISBN 978-1461471158
David Halliday (2007). Fundamentals of Physics (8th ed.). Wiley. ISBN 978-0-
471-15950-6.
Richard_Liboff (2002). Introductory Quantum Mechanics (4th ed.). Addison
Wesley. ISBN 978-0-8053-8714-8.
Serway, Moses, and Moyer (2004). Modern Physics (3rd ed.). Brooks Cole.
ISBN 978-0-534-49340-0.CS1 maint: Multiple names: authors list (link)
SchrÃ¶dinger, Erwin (December 1926). "An Undulatory Theory of the Mechanics of
Atoms and Molecules". Phys. Rev. 28 (6): 1049â1070. Bibcode:
1926PhRv...28.1049S. doi:10.1103/PhysRev.28.1049.
Teschl,_Gerald (2009). Mathematical_Methods_in_Quantum_Mechanics;_With
Applications_to_SchrÃ¶dinger_Operators. Providence, Rhode Island: American
Mathematical_Society. ISBN 978-0-8218-4660-5.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "SchrÃ¶dinger_equation",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Quantum_Physics â textbook by Benjamin Crowell with a treatment of the time-
independent SchrÃ¶dinger equation
Linear_SchrÃ¶dinger_Equation at EqWorld: The World of Mathematical Equations.
Nonlinear_SchrÃ¶dinger_Equation at EqWorld: The World of Mathematical
Equations.
The_SchrÃ¶dinger_Equation_in_One_Dimension as well as the directory_of_the
book.
All_about_3D_SchrÃ¶dinger_Equation
Mathematical aspects of SchrÃ¶dinger equations are discussed on the Dispersive
PDE_Wiki.
Web-SchrÃ¶dinger:_Interactive_solution_of_the_2D_time-dependent_and_stationary
SchrÃ¶dinger_equation
An_alternate_reasoning_behind_the_SchrÃ¶dinger_Equation
Online software-Periodic_Potential_Lab Solves the time-independent SchrÃ¶dinger
equation for arbitrary periodic potentials.
What_Do_You_Do_With_a_Wavefunction?
The_Young_Double-Slit_Experiment
Schrodinger_solver_in_1,_2_and_3d
    * v
    * t
    * e
Quantum_mechanics
                    * Introduction
                    * History
Background                o timeline
                    * Glossary
                    * Classical_mechanics
                    * Old_quantum_theory
                    * Braâket_notation
                    * Casimir_effect
                    * Complementarity
                    * Density_matrix
                    * Energy_level
                          o ground_state
                          o excited_state
                          o degenerate_levels
                          o Vacuum_state
                          o Zero-point_energy
                          o QED_vacuum
                          o QCD_vacuum
                    * Hamiltonian
                    * Operator
                    * Quantum_coherence
                    * Quantum_decoherence
                    * Measurement
                    * Quantum
                    * Quantum_realm
                    * Quantum_system
                    * Quantum_state
                    * Quantum_number
                    * Quantum_entanglement
                    * Quantum_superposition
Fundamentals        * Quantum_nonlocality
                    * Quantum_tunnelling
                    * Quantum_levitation
                    * Quantum_fluctuation
                    * Quantum_annealing
                    * Quantum_foam
                    * Quantum_noise
                    * Heisenberg_uncertainty_principle
                    * Spontaneous_parametric_down-conversion
                    * Von_Neumann_entropy
                    * Spin
                    * Scattering_theory
                    * Symmetry_in_quantum_mechanics
                    * Symmetry_breaking
                    * Spontaneous_symmetry_breaking
                    * Wave_propagation
                    * Quantum_interference
                    * Wave_function
                          o Wave_function_collapse
                          o Waveâparticle_duality
                          o Matter_wave
                    * Qubit
                    * Qutrit
                    * Observable
                    * Probability_distribution
                    * Formulations
                    * Heisenberg
                    * Interaction
Formulations        * Matrix_mechanics
                    * SchrÃ¶dinger
                    * Path_integral_formulation
                    * Phase_space
                    * Dirac
                    * KleinâGordon
Equations           * Pauli
                    * Rydberg
                    * SchrÃ¶dinger
                    * Interpretations
                    * Bayesian
                    * Consistent_histories
                    * Copenhagen
                    * de_BroglieâBohm
                    * Ensemble
Interpretations     * Hidden_variables
                    * Many_worlds
                    * Objective_collapse
                    * Quantum_logic
                    * Relational
                    * Stochastic
                    * Transactional
                    * Cosmological
                    * Afshar
                    * Bell's_inequality
                    * Cold_Atom_Laboratory
                    * DavissonâGermer
                    * Delayed-choice_quantum_eraser
                    * Double-slit
                    * FranckâHertz_experiment
Experiments         * LeggettâGarg_inequality
                    * Mach-Zehnder_inter.
                    * ElitzurâVaidman
                    * Popper
                    * Quantum_eraser
                    * SchrÃ¶dinger's_cat
                    * Quantum_suicide_and_immortality
                    * SternâGerlach
                    * Wheeler's_delayed_choice
                    * Q-analog
                          o List
                          o Quantum_algebra
                          o Quantum_calculus
                          o Quantum_differential_calculus
                          o Quantum_geometry
                          o Quantum_group
                    * Quantum_Bayesianism
                    * Quantum_biology
                    * Quantum_chemistry
                    * Quantum_chaos
Science             * Quantum_cognition
                    * Quantum_cosmology
                    * Quantum_dynamics
                    * Quantum_economics
                    * Quantum_evolution
                    * Quantum_finance
                    * Quantum_game_theory
                    * Quantum_measurement_problem
                    * Quantum_mind
                    * Quantum_probability
                    * Quantum_social_science
                    * Quantum_stochastic_calculus
                    * Quantum_spacetime
                    * Quantum_algorithms
                    * Quantum_amplifier
                    * Quantum_cellular_automata
                          o Quantum_finite_automata
                    * Quantum_electronics
                    * Quantum_logic_gates
                    * Quantum_clock
                    * Quantum_channel
                    * Quantum_bus
                    * Quantum_circuit
                    * Phase_qubit
                    * Matrix_isolation
                    * Quantum_dot
                    * Quantum_dot_display
                    * Quantum_dot_solar_cell
                    * Quantum_dot_cellular_automaton
                    * Quantum_dot_single-photon_source
                    * Quantum_dot_laser
                    * Quantum_well
                    * Quantum_computing
Technology                o Timeline
                    * Quantum_cryptography
                    * Post-quantum_cryptography
                    * Quantum_error_correction
                    * Quantum_imaging
                    * Quantum_image_processing
                    * Quantum_information
                    * Quantum_key_distribution
                    * Quantum_machine
                    * Quantum_machine_learning
                    * Quantum_metamaterial
                    * Quantum_metrology
                    * Quantum_network
                    * Quantum_neural_network
                    * Quantum_optics
                    * Quantum_programming
                    * Quantum_sensors
                    * Quantum_simulator
                    * Quantum_teleportation
                    * Quantum_levitation
                    * Time_travel
                    * Quantum_complexity_theory
                    * Quantum_statistical_mechanics
                    * Relativistic_quantum_mechanics
                    * Quantum_field_theory
                          o Axiomatic_quantum_field_theory
                          o Quantum_field_theory_in_curved_spacetime
                          o Thermal_quantum_field_theory
Extensions                o Topological_quantum_field_theory
                          o Local_quantum_field_theory
                          o Conformal_field_theory
                          o Two-dimensional_conformal_field_theory
                          o Liouville_field_theory
                          o History
                    * Quantum_gravity
    * [Category] Category
    * [Portal] Physics_Portal
    * [WikiProject] Physics_WikiProject
    * [Commons page] Commons
Authority_control [Edit_this_at_Wikidata]     * GND: 4053332-3

Retrieved from "https://en.wikipedia.org/w/
index.php?title=SchrÃ¶dinger_equation&oldid=909815694"
Categories:
    * SchrÃ¶dinger_equation
    * Differential_equations
    * Wave_mechanics
    * Functions_of_space_and_time
Hidden categories:
    * Articles_with_short_description
    * Use_dmy_dates_from_June_2016
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_February_2019
    * All_articles_with_failed_verification
    * Articles_with_failed_verification_from_September_2018
    * Articles_with_attributed_pull_quotes
    * Articles_with_unsourced_statements_from_January_2014
    * Articles_needing_cleanup_from_October_2016
    * All_pages_needing_cleanup
    * Articles_with_sections_that_need_to_be_turned_into_prose_from_October
      2016
    * Articles_with_unsourced_statements_from_September_2015
    * CS1_maint:_Multiple_names:_authors_list
    * Wikipedia_articles_with_GND_identifiers
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
    * Wikiversity
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
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Interlingua
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Malti
    * ÙØµØ±Ù
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Ù¾ÙØ¬Ø§Ø¨Û
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * æè¨
    * å´è¯­
    * ××Ö´×××©
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 19:39 (UTC).
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
