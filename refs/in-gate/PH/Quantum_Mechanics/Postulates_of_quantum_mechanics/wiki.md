The following text has been accessed from https://en.wikipedia.org/wiki/Mathematical_formulation_of_quantum_mechanics at Fri Aug 9 03:11:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Mathematical formulation of quantum mechanics ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Mathematical structures that allow quantum mechanics to be explained
Part of a series on
Quantum_mechanics
   i &#x210F;   &#x2202;  &#x2202; t     |  &#x03C8; ( t ) &#x27E9; =    H
&#x005E;     |  &#x03C8; ( t ) &#x27E9;   {\displaystyle i\hbar {\frac
{\partial }{\partial t}}|\psi (t)\rangle ={\hat {H}}|\psi (t)\rangle }  [
{\displaystyle i\hbar {\frac {\partial }{\partial t}}|\psi (t)\rangle ={\hat
{H}}|\psi (t)\rangle }]
SchrÃ¶dinger_equation
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
The mathematical formulations of quantum mechanics are those mathematical
formalisms that permit a rigorous description of quantum_mechanics. Such are
distinguished from mathematical formalisms for theories developed prior to the
early 1900s by the use of abstract mathematical structures, such as infinite-
dimensional Hilbert_spaces and operators on these spaces. Many of these
structures are drawn from functional_analysis, a research area within pure
mathematics that was influenced in part by the needs of quantum mechanics. In
brief, values of physical observables such as energy and momentum were no
longer considered as values of functions on phase_space, but as eigenvalues;
more precisely as spectral_values of linear operators in Hilbert space.[1]
These formulations of quantum mechanics continue to be used today. At the heart
of the description are ideas of quantum_state and quantum observables which are
radically different from those used in previous models of physical reality.
While the mathematics permits calculation of many quantities that can be
measured experimentally, there is a definite theoretical limit to values that
can be simultaneously measured. This limitation was first elucidated by
Heisenberg through a thought_experiment, and is represented mathematically in
the new formalism by the non-commutativity of operators representing quantum
observables.
Prior to the emergence of quantum mechanics as a separate theory, the
mathematics used in physics consisted mainly of formal mathematical_analysis,
beginning with calculus, and increasing in complexity up to differential
geometry and partial_differential_equations. Probability_theory was used in
statistical_mechanics. Geometric intuition played a strong role in the first
two and, accordingly, theories_of_relativity were formulated entirely in terms
of geometric concepts. The phenomenology of quantum physics arose roughly
between 1895 and 1915, and for the 10 to 15 years before the emergence of
quantum theory (around 1925) physicists continued to think of quantum theory
within the confines of what is now called classical_physics, and in particular
within the same mathematical structures. The most sophisticated example of this
is the SommerfeldâWilsonâIshiwara_quantization rule, which was formulated
entirely on the classical phase_space.
⁰
***** Contents *****
    * 1_History_of_the_formalism
          o 1.1_The_"old_quantum_theory"_and_the_need_for_new_mathematics
          o 1.2_The_"new_quantum_theory"
          o 1.3_Later_developments
    * 2_Mathematical_structure_of_quantum_mechanics
          o 2.1_Postulates_of_quantum_mechanics
          o 2.2_Pictures_of_dynamics
          o 2.3_Representations
          o 2.4_Time_as_an_operator
          o 2.5_Spin
          o 2.6_Pauli's_principle
    * 3_The_problem_of_measurement
          o 3.1_The_relative_state_interpretation
    * 4_List_of_mathematical_tools
    * 5_Notes
    * 6_References
***** History of the formalism[edit] *****
**** The "old quantum theory" and the need for new mathematics[edit] ****
Main article: Old_quantum_theory
In the 1890s, Planck was able to derive the blackbody_spectrum which was later
used to avoid the classical ultraviolet_catastrophe by making the unorthodox
assumption that, in the interaction of electromagnetic_radiation with matter,
energy could only be exchanged in discrete units which he called quanta. Planck
postulated a direct proportionality between the frequency of radiation and the
quantum of energy at that frequency. The proportionality constant, h, is now
called Planck's_constant in his honor.
In 1905, Einstein explained certain features of the photoelectric_effect by
assuming that Planck's energy quanta were actual particles, which were later
dubbed photons.
[light_at_the_right_frequency.]
All of these developments were phenomenological and challenged the theoretical
physics of the time. Bohr_and_Sommerfeld went on to modify classical_mechanics
in an attempt to deduce the Bohr_model from first principles. They proposed
that, of all closed classical orbits traced by a mechanical system in its phase
space, only the ones that enclosed an area which was a multiple of Planck's
constant were actually allowed. The most sophisticated version of this
formalism was the so-called SommerfeldâWilsonâIshiwara_quantization.
Although the Bohr model of the hydrogen atom could be explained in this way,
the spectrum of the helium atom (classically an unsolvable 3-body_problem)
could not be predicted. The mathematical status of quantum theory remained
uncertain for some time.
In 1923 de_Broglie proposed that waveâparticle_duality applied not only to
photons but to electrons and every other physical system.
The situation changed rapidly in the years 1925â1930, when working
mathematical foundations were found through the groundbreaking work of Erwin
SchrÃ¶dinger, Werner_Heisenberg, Max_Born, Pascual_Jordan, and the foundational
work of John_von_Neumann, Hermann_Weyl and Paul_Dirac, and it became possible
to unify several different approaches in terms of a fresh set of ideas. The
physical interpretation of the theory was also clarified in these years after
Werner_Heisenberg discovered the uncertainty relations and Niels_Bohr
introduced the idea of complementarity.
**** The "new quantum theory"[edit] ****
Werner_Heisenberg's matrix_mechanics was the first successful attempt at
replicating the observed quantization of atomic_spectra. Later in the same
year, SchrÃ¶dinger created his wave_mechanics. SchrÃ¶dinger's formalism was
considered easier to understand, visualize and calculate as it led to
differential_equations, which physicists were already familiar with solving.
Within a year, it was shown that the two theories were equivalent.
SchrÃ¶dinger himself initially did not understand the fundamental probabilistic
nature of quantum mechanics, as he thought that the absolute_square of the wave
function of an electron should be interpreted as the charge_density of an
object smeared out over an extended, possibly infinite, volume of space. It was
Max_Born who introduced the interpretation of the absolute_square of the wave
function as the probability distribution of the position of a pointlike object.
Born's idea was soon taken over by Niels Bohr in Copenhagen who then became the
"father" of the Copenhagen_interpretation of quantum mechanics. SchrÃ¶dinger's
wave_function can be seen to be closely related to the classical
HamiltonâJacobi_equation. The correspondence to classical mechanics was even
more explicit, although somewhat more formal, in Heisenberg's matrix mechanics.
In his PhD thesis project, Paul_Dirac[2] discovered that the equation for the
operators in the Heisenberg_representation, as it is now called, closely
translates to classical equations for the dynamics of certain quantities in the
Hamiltonian formalism of classical mechanics, when one expresses them through
Poisson_brackets, a procedure now known as canonical_quantization.
To be more precise, already before SchrÃ¶dinger, the young postdoctoral fellow
Werner_Heisenberg invented his matrix_mechanics, which was the first correct
quantum mechanicsââ the essential breakthrough. Heisenberg's matrix
mechanics formulation was based on algebras of infinite matrices, a very
radical formulation in light of the mathematics of classical physics, although
he started from the index-terminology of the experimentalists of that time, not
even aware that his "index-schemes" were matrices, as Born soon pointed out to
him. In fact, in these early years, linear_algebra was not generally popular
with physicists in its present form.
Although SchrÃ¶dinger himself after a year proved the equivalence of his wave-
mechanics and Heisenberg's matrix mechanics, the reconciliation of the two
approaches and their modern abstraction as motions in Hilbert space is
generally attributed to Paul_Dirac, who wrote a lucid account in his 1930
classic The_Principles_of_Quantum_Mechanics. He is the third, and possibly most
important, pillar of that field (he soon was the only one to have discovered a
relativistic generalization of the theory). In his above-mentioned account, he
introduced the braâket_notation, together with an abstract formulation in
terms of the Hilbert_space used in functional_analysis; he showed that
SchrÃ¶dinger's and Heisenberg's approaches were two different representations
of the same theory, and found a third, most general one, which represented the
dynamics of the system. His work was particularly fruitful in all kinds of
generalizations of the field.
The first complete mathematical formulation of this approach, known as the
Diracâvon_Neumann_axioms, is generally credited to John_von_Neumann's 1932
book Mathematical_Foundations_of_Quantum_Mechanics, although Hermann_Weyl had
already referred to Hilbert spaces (which he called unitary spaces) in his 1927
classic paper and book. It was developed in parallel with a new approach to the
mathematical spectral_theory based on linear_operators rather than the
quadratic_forms that were David_Hilbert's approach a generation earlier. Though
theories of quantum mechanics continue to evolve to this day, there is a basic
framework for the mathematical formulation of quantum mechanics which underlies
most approaches and can be traced back to the mathematical work of John_von
Neumann. In other words, discussions about interpretation_of_the_theory, and
extensions to it, are now mostly conducted on the basis of shared assumptions
about the mathematical foundations.
**** Later developments[edit] ****
The application of the new quantum theory to electromagnetism resulted in
quantum_field_theory, which was developed starting around 1930. Quantum field
theory has driven the development of more sophisticated formulations of quantum
mechanics, of which the ones presented here are simple special cases.
    * Path_integral_formulation
    * Phase_space_formulation of quantum mechanics & geometric_quantization
    * Signed particle formulation[3]
    * quantum_field_theory_in_curved_spacetime
    * axiomatic, algebraic and constructive_quantum_field_theory
    * C*_algebra formalism
    * Generalized_statistical_model_of_quantum_mechanics
On a different front, von Neumann originally dispatched quantum_measurement
with his infamous postulate on the collapse_of_the_wavefunction, raising a host
of philosophical problems. Over the intervening 70 years, the problem of
measurement became an active research area and itself spawned some new
formulations of quantum mechanics.
    * Relative_state/Many-worlds_interpretation of quantum mechanics
    * Decoherence
    * Consistent_histories formulation of quantum mechanics
    * Quantum_logic formulation of quantum mechanics
A related topic is the relationship to classical mechanics. Any new physical
theory is supposed to reduce to successful old theories in some approximation.
For quantum mechanics, this translates into the need to study the so-called
classical_limit_of_quantum_mechanics. Also, as Bohr emphasized, human cognitive
abilities and language are inextricably linked to the classical realm, and so
classical descriptions are intuitively more accessible than quantum ones. In
particular, quantization, namely the construction of a quantum theory whose
classical limit is a given and known classical theory, becomes an important
area of quantum physics in itself.
Finally, some of the originators of quantum theory (notably Einstein and
SchrÃ¶dinger) were unhappy with what they thought were the philosophical
implications of quantum mechanics. In particular, Einstein took the position
that quantum mechanics must be incomplete, which motivated research into so-
called hidden-variable theories. The issue of hidden variables has become in
part an experimental issue with the help of quantum_optics.
    * de_BroglieâBohmâBell pilot_wave formulation of quantum mechanics
    * Bell's_inequalities
    * KochenâSpecker_theorem
***** Mathematical structure of quantum mechanics[edit] *****
A physical system is generally described by three basic ingredients: states;
observables; and dynamics (or law of time_evolution) or, more generally, a
group_of_physical_symmetries. A classical description can be given in a fairly
direct way by a phase_space model of mechanics: states are points in a
symplectic phase space, observables are real-valued functions on it, time
evolution is given by a one-parameter group of symplectic transformations of
the phase space, and physical symmetries are realized by symplectic
transformations. A quantum description normally consists of a Hilbert_space of
states, observables are self_adjoint_operators on the space of states, time
evolution is given by a one-parameter_group of unitary transformations on the
Hilbert space of states, and physical symmetries are realized by unitary
transformations. (It is possible, to map this Hilbert-space picture to a phase
space_formulation, invertibly. See below.)
**** Postulates of quantum mechanics[edit] ****
The following summary of the mathematical framework of quantum mechanics can be
partly traced back to the Diracâvon_Neumann_axioms.
    * Each physical system is associated with a (topologically) separable
      complex Hilbert_space H with inner_product â¨Ï|Ïâ©. Rays (that is,
      subspaces of complex dimension 1) in H are associated with quantum_states
      of the system. In other words, quantum states can be identified with
      equivalence classes of vectors of length 1 in H, where two vectors
      represent the same state if they differ only by a phase_factor.
      Separability is a mathematically convenient hypothesis, with the physical
      interpretation that countably many observations are enough to uniquely
      determine the state. "A quantum mechanical state is a ray in projective
      Hilbert_space, not a vector. Many textbooks fail to make this
      distinction, which could be partly a result of the fact that the
      SchrÃ¶dinger_equation itself involves Hilbert-space "vectors", with the
      result that the imprecise use of "state vector" rather than ray is very
      difficult to avoid."[4]
    * The Hilbert space of a composite system is the Hilbert space tensor
      product of the state spaces associated with the component systems (for
      instance, J. M. Jauch, Foundations of quantum mechanics, section 11.7).
      For a non-relativistic system consisting of a finite number of
      distinguishable particles, the component systems are the individual
      particles.
    * Physical symmetries act on the Hilbert space of quantum states unitarily
      or antiunitarily due to Wigner's_theorem (supersymmetry is another matter
      entirely).
    * Physical observables are represented by Hermitian matrices on H.
    * The expectation_value (in the sense of probability theory) of the
      observable A for the system in state represented by the unit vector Ï
      â H is
               &#x27E8; &#x03C8; &#x2223; A &#x2223; &#x03C8; &#x27E9;
            {\displaystyle \langle \psi \mid A\mid \psi \rangle }  [\langle
            \psi \mid A\mid \psi \rangle ]
    * By spectral_theory, we can associate a probability_measure to the values
      of A in any state Ï. We can also show that the possible values of the
      observable A in any state must belong to the spectrum of A. In the
      special case A has only discrete_spectrum, the possible outcomes of
      measuring A are its eigenvalues. More precisely, if we represent the
      state Ï in the basis formed by the eigenvectors of A, then the square of
      the modulus of the component attached to a given eigenvector is the
      probability of observing its corresponding eigenvalue.
    * More generally, a state can be represented by a so-called density
      operator, which is a trace_class, nonnegative self-adjoint operator Ï
      normalized to be of trace 1. The expected value of A in the state Ï is
               tr &#x2061; ( A &#x03C1; )   {\displaystyle \operatorname {tr}
            (A\rho )}  [\operatorname {tr} (A\rho )]
    * If ÏÏ is the orthogonal projector onto the one-dimensional subspace of
      H spanned by |Ï&#x27e9;, then
               tr &#x2061; ( A  &#x03C1;  &#x03C8;   ) =  &#x27E8;  &#x03C8;
            &#x2223; A &#x2223; &#x03C8;  &#x27E9;    {\displaystyle
            \operatorname {tr} (A\rho _{\psi })=\left\langle \psi \mid A\mid
            \psi \right\rangle }  [\operatorname {tr} (A\rho _{\psi
            })=\left\langle \psi \mid A\mid \psi \right\rangle ]
    * Density operators are those that are in the closure of the convex_hull of
      the one-dimensional orthogonal projectors. Conversely, one-dimensional
      orthogonal projectors are extreme_points of the set of density operators.
      Physicists also call one-dimensional orthogonal projectors pure states
      and other density operators mixed states.
One can in this formalism state Heisenberg's uncertainty_principle and prove it
as a theorem, although the exact historical sequence of events, concerning who
derived what and under which framework, is the subject of historical
investigations outside the scope of this article.
Furthermore, to the postulates of quantum mechanics one should also add basic
statements on the properties of spin and Pauli's exclusion_principle, see
below.
**** Pictures of dynamics[edit] ****
Main article: Dynamical_pictures
    * In the so-called SchrÃ¶dinger_picture of quantum mechanics, the dynamics
      is given as follows:
The time_evolution of the state is given by a differentiable function from the
real numbers R, representing instants of time, to the Hilbert space of system
states. This map is characterized by a differential equation as follows: If |Ï
(t)&#x27e9; denotes the state of the system at any one time t, the following
SchrÃ¶dinger_equation holds:
SchrÃ¶dinger equation (general)
   i &#x210F;   d  d t     |  &#x03C8; ( t )  &#x27E9;  = H  |  &#x03C8; ( t )
&#x27E9;    {\displaystyle i\hbar {\frac {d}{dt}}\left|\psi (t)\right\rangle
=H\left|\psi (t)\right\rangle }  [i\hbar {\frac {d}{dt}}\left|\psi
(t)\right\rangle =H\left|\psi (t)\right\rangle ]
where H is a densely defined self-adjoint operator, called the system
Hamiltonian, i is the imaginary_unit and Ä§ is the reduced_Planck_constant. As
an observable, H corresponds to the total energy of the system.
Alternatively, by Stone's_theorem one can state that there is a strongly
continuous one-parameter unitary map U(t): H â H such that
          |  &#x03C8; ( t + s )  &#x27E9;  = U ( t )  |  &#x03C8; ( s )
      &#x27E9;    {\displaystyle \left|\psi (t+s)\right\rangle =U(t)\left|\psi
      (s)\right\rangle }  [\left|\psi (t+s)\right\rangle =U(t)\left|\psi
      (s)\right\rangle ]
for all times s, t. The existence of a self-adjoint Hamiltonian H such that
         U ( t ) =  e  &#x2212; ( i  /  &#x210F; ) t H     {\displaystyle U
      (t)=e^{-(i/\hbar )tH}}  [U(t)=e^{-(i/\hbar )tH}]
is a consequence of Stone's_theorem_on_one-parameter_unitary_groups. It is
assumed that H does not depend on time and that the perturbation starts at t0 =
0; otherwise one must use the Dyson_series, formally written as
         U ( t ) =   T    [  exp &#x2061;  (  &#x2212;   i &#x210F;    &#x222B;
      t  0     t      d    t &#x2032;   H (  t &#x2032;  )  )   ]   ,
      {\displaystyle U(t)={\mathcal {T}}\left[\exp \left(-{\frac {i}{\hbar
      }}\int _{t_{0}}^{t}\,{\rm {d}}t'\,H(t')\right)\right]\,,}  [U(t)=
      {\mathcal {T}}\left[\exp \left(-{\frac {i}{\hbar }}\int _{t_{0}}^{t}\,
      {\rm {d}}t'\,H(t')\right)\right]\,,]
where       T     {\displaystyle {\mathcal {T}}}  [{\mathcal {T}}] is Dyson's
time-ordering symbol.
(This symbol permutes a product of noncommuting operators of the form
          B  1   (  t  1   ) &#x22C5;  B  2   (  t  2   ) &#x22C5; &#x22EF;
      &#x22C5;  B  n   (  t  n   )   {\displaystyle B_{1}(t_{1})\cdot B_{2}(t_
      {2})\cdot \dots \cdot B_{n}(t_{n})}  [B_{1}(t_{1})\cdot B_{2}(t_{2})\cdot
      \dots \cdot B_{n}(t_{n})]
into the uniquely determined re-ordered expression
          B   i  1     (  t   i  1     ) &#x22C5;  B   i  2     (  t   i  2
      ) &#x22C5; &#x22EF; &#x22C5;  B   i  n     (  t   i  n     )
      {\displaystyle B_{i_{1}}(t_{i_{1}})\cdot B_{i_{2}}(t_{i_{2}})\cdot \dots
      \cdot B_{i_{n}}(t_{i_{n}})}  [B_{i_{1}}(t_{i_{1}})\cdot B_{i_{2}}(t_{i_
      {2}})\cdot \dots \cdot B_{i_{n}}(t_{i_{n}})] with      t   i  1
      &#x2265;  t   i  2     &#x2265; &#x22EF; &#x2265;  t   i  n      .
      {\displaystyle t_{i_{1}}\geq t_{i_{2}}\geq \dots \geq t_{i_{n}}\,.}  [t_
      {i_{1}}\geq t_{i_{2}}\geq \dots \geq t_{i_{n}}\,.]
The result is a causal chain, the primary cause in the past on the utmost
r.h.s., and finally the present effect on the utmost l.h.s. .)
    * The Heisenberg_picture of quantum mechanics focuses on observables and
      instead of considering states as varying in time, it regards the states
      as fixed and the observables as changing. To go from the SchrÃ¶dinger to
      the Heisenberg picture one needs to define time-independent states and
      time-dependent operators thus:
          | &#x03C8; &#x27E9;  =  |  &#x03C8; ( 0 )  &#x27E9;    {\displaystyle
      \left|\psi \right\rangle =\left|\psi (0)\right\rangle }  [\left|\psi
      \right\rangle =\left|\psi (0)\right\rangle ]
         A ( t ) = U ( &#x2212; t ) A U ( t ) .    {\displaystyle A(t)=U(-t)AU
      (t).\quad }  [A(t)=U(-t)AU(t).\quad ]
It is then easily checked that the expected values of all observables are the
same in both pictures
         &#x27E8; &#x03C8; &#x2223; A ( t ) &#x2223; &#x03C8; &#x27E9; =
      &#x27E8; &#x03C8; ( t ) &#x2223; A &#x2223; &#x03C8; ( t ) &#x27E9;
      {\displaystyle \langle \psi \mid A(t)\mid \psi \rangle =\langle \psi
      (t)\mid A\mid \psi (t)\rangle }  [\langle \psi \mid A(t)\mid \psi \rangle
      =\langle \psi (t)\mid A\mid \psi (t)\rangle ]
and that the time-dependent Heisenberg operators satisfy
Heisenberg picture (general)
     d  d t    A ( t ) =   i &#x210F;   [ H , A ( t ) ] +    &#x2202; A ( t )
&#x2202; t    ,   {\displaystyle {\frac {d}{dt}}A(t)={\frac {i}{\hbar }}[H,A
(t)]+{\frac {\partial A(t)}{\partial t}},}  [{\frac {d}{dt}}A(t)={\frac {i}
{\hbar }}[H,A(t)]+{\frac {\partial A(t)}{\partial t}},]
which is true for time-dependent A = A(t). Notice the commutator expression is
purely formal when one of the operators is unbounded. One would specify a
representation for the expression to make sense of it.
    * The so-called Dirac_picture or interaction_picture has time-dependent
      states and observables, evolving with respect to different Hamiltonians.
      This picture is most useful when the evolution of the observables can be
      solved exactly, confining any complications to the evolution of the
      states. For this reason, the Hamiltonian for the observables is called
      "free Hamiltonian" and the Hamiltonian for the states is called
      "interaction Hamiltonian". In symbols:
Dirac picture
   i &#x210F;   d  d t     |  &#x03C8; ( t )  &#x27E9;  =   H    i n t    ( t )
|  &#x03C8; ( t )  &#x27E9;    {\displaystyle i\hbar {\frac {d}{dt}}\left|\psi
(t)\right\rangle ={H}_{\rm {int}}(t)\left|\psi (t)\right\rangle }  [i\hbar
{\frac {d}{dt}}\left|\psi (t)\right\rangle ={H}_{\rm {int}}(t)\left|\psi
(t)\right\rangle ]
   i &#x210F;   d  d t    A ( t ) = [ A ( t ) ,  H  0   ] .   {\displaystyle
i\hbar {d \over dt}A(t)=[A(t),H_{0}].}  [i\hbar {d \over dt}A(t)=[A(t),H_{0}].]
The interaction picture does not always exist, though. In interacting quantum
field theories, Haag's_theorem states that the interaction picture does not
exist. This is because the Hamiltonian cannot be split into a free and an
interacting part within a superselection_sector. Moreover, even if in the
SchrÃ¶dinger picture the Hamiltonian does not depend on time, e.g. H = H0 + V,
in the interaction picture it does, at least, if V does not commute with H0,
since
          H   i n t    ( t ) &#x2261;  e   ( i  /  &#x210F;  ) t  H  0      V
      e   ( &#x2212; i  /  &#x210F;  ) t  H  0       {\displaystyle H_{\rm
      {int}}(t)\equiv e^{{(i/\hbar })tH_{0}}\,V\,e^{{(-i/\hbar })tH_{0}}}  [H_
      {\rm {int}}(t)\equiv e^{{(i/\hbar })tH_{0}}\,V\,e^{{(-i/\hbar })tH_{0}}].
So the above-mentioned Dyson-series has to be used anyhow.
The Heisenberg picture is the closest to classical Hamiltonian mechanics (for
example, the commutators appearing in the above equations directly translate
into the classical Poisson_brackets); but this is already rather "high-browed",
and the SchrÃ¶dinger picture is considered easiest to visualize and understand
by most people, to judge from pedagogical accounts of quantum mechanics. The
Dirac picture is the one used in perturbation_theory, and is specially
associated to quantum_field_theory and many-body_physics.
Similar equations can be written for any one-parameter unitary group of
symmetries of the physical system. Time would be replaced by a suitable
coordinate parameterizing the unitary group (for instance, a rotation angle, or
a translation distance) and the Hamiltonian would be replaced by the conserved
quantity associated to the symmetry (for instance, angular or linear momentum).
**** Representations[edit] ****
The original form of the SchrÃ¶dinger_equation depends on choosing a particular
representation of Heisenberg's canonical_commutation_relations. The Stoneâvon
Neumann_theorem dictates that all irreducible representations of the finite-
dimensional Heisenberg commutation relations are unitarily equivalent. A
systematic understanding of its consequences has led to the phase_space
formulation of quantum mechanics, which works in full phase_space instead of
Hilbert_space, so then with a more intuitive link to the classical_limit
thereof. This picture also simplifies considerations of quantization, the
deformation extension from classical to quantum mechanics.
The quantum_harmonic_oscillator is an exactly solvable system where the
different representations are easily compared. There, apart from the
Heisenberg, or SchrÃ¶dinger (position or momentum), or phase-space
representations, one also encounters the Fock (number) representation and the
SegalâBargmann_(Fock-space_or_coherent_state)_representation (named after
Irving_Segal and Valentine_Bargmann). All four are unitarily equivalent.
**** Time as an operator[edit] ****
The framework presented so far singles out time as the parameter that
everything depends on. It is possible to formulate mechanics in such a way that
time becomes itself an observable associated to a self-adjoint operator. At the
classical level, it is possible to arbitrarily parameterize the trajectories of
particles in terms of an unphysical parameter s, and in that case the time t
becomes an additional generalized coordinate of the physical system. At the
quantum level, translations in s would be generated by a "Hamiltonian" H − E,
where E is the energy operator and H is the "ordinary" Hamiltonian. However,
since s is an unphysical parameter, physical states must be left invariant by
"s-evolution", and so the physical state space is the kernel of H − E (this
requires the use of a rigged_Hilbert_space and a renormalization of the norm).
This is related to the quantization_of_constrained_systems and quantization_of
gauge_theories. It is also possible to formulate a quantum theory of "events"
where time becomes an observable (see D. Edwards).
**** Spin[edit] ****
In addition to their other properties, all particles possess a quantity called
spin, an intrinsic angular momentum. Despite the name, particles do not
literally spin around an axis, and quantum mechanical spin has no
correspondence in classical physics. In the position representation, a spinless
wavefunction has position r and time t as continuous variables, Ï = Ï(r, t),
for spin wavefunctions the spin is an additional discrete variable: Ï = Ï(r,
t, Ï), where Ï takes the values;
         &#x03C3; = &#x2212; S &#x210F; , &#x2212; ( S &#x2212; 1 ) &#x210F; ,
      &#x2026; , 0 , &#x2026; , + ( S &#x2212; 1 ) &#x210F; , + S &#x210F;  .
      {\displaystyle \sigma =-S\hbar ,-(S-1)\hbar ,\dots ,0,\dots ,+(S-1)\hbar
      ,+S\hbar \,.}  [\sigma =-S\hbar ,-(S-1)\hbar ,\dots ,0,\dots ,+(S-1)\hbar
      ,+S\hbar \,.]
That is, the state of a single particle with spin S is represented by a (2S +
1)-component spinor of complex-valued wave functions.
Two classes of particles with very different behaviour are bosons which have
integer spin (S = 0, 1, 2...), and fermions possessing half-integer spin
(S = &#x200b;1⁄2, &#x200b;3⁄2, &#x200b;5⁄2, ...).
**** Pauli's principle[edit] ****
The property of spin relates to another basic property concerning systems of N
identical particles: Pauli's exclusion_principle, which is a consequence of the
following permutation behaviour of an N-particle wave function; again in the
position representation one must postulate that for the transposition of any
two of the N particles one always should have
Pauli principle
   &#x03C8; ( &#x2026; ,    r   i   ,  &#x03C3;  i   ,  &#x2026; ,    r   j   ,
&#x03C3;  j   ,  &#x2026; ) = ( &#x2212; 1  )  2 S   &#x22C5; &#x03C8;
( &#x2026; ,    r   j   ,  &#x03C3;  j   ,  &#x2026; ,   r   i   ,  &#x03C3;  i
,  &#x2026; )   {\displaystyle \psi (\dots ,\,\mathbf {r} _{i},\sigma _
{i},\,\dots ,\,\mathbf {r} _{j},\sigma _{j},\,\dots )=(-1)^{2S}\cdot \psi
(\dots ,\,\mathbf {r} _{j},\sigma _{j},\,\dots ,\mathbf {r} _{i},\sigma _
{i},\,\dots )}  [\psi (\dots ,\,\mathbf {r} _{i},\sigma _{i},\,\dots ,\,\mathbf
{r} _{j},\sigma _{j},\,\dots )=(-1)^{2S}\cdot \psi (\dots ,\,\mathbf {r} _
{j},\sigma _{j},\,\dots ,\mathbf {r} _{i},\sigma _{i},\,\dots )]
i.e., on transposition of the arguments of any two particles the wavefunction
should reproduce, apart from a prefactor (−1)2S which is +1 for bosons, but
(−1) for fermions. Electrons are fermions with S = 1/2; quanta of light are
bosons with S = 1. In nonrelativistic quantum mechanics all particles are
either bosons or fermions; in relativistic quantum theories also
"supersymmetric" theories exist, where a particle is a linear combination of a
bosonic and a fermionic part. Only in dimension d = 2 can one construct
entities where (−1)2S is replaced by an arbitrary complex number with magnitude
1, called anyons.
Although spin and the Pauli principle can only be derived from relativistic
generalizations of quantum mechanics the properties mentioned in the last two
paragraphs belong to the basic postulates already in the non-relativistic
limit. Especially, many important properties in natural science, e.g. the
periodic_system of chemistry, are consequences of the two properties.
***** The problem of measurement[edit] *****
The picture given in the preceding paragraphs is sufficient for description of
a completely isolated system. However, it fails to account for one of the main
differences between quantum mechanics and classical mechanics, that is, the
effects of measurement.[5] The von Neumann description of quantum measurement
of an observable A, when the system is prepared in a pure state Ï is the
following (note, however, that von Neumann's description dates back to the
1930s and is based on experiments as performed during that time â more
specifically the ComptonâSimon_experiment; it is not applicable to most
present-day measurements within the quantum domain):
    * Let A have spectral resolution
         A = &#x222B; &#x03BB;  d  E  A   &#x2061; ( &#x03BB; ) ,
      {\displaystyle A=\int \lambda \,d\operatorname {E} _{A}(\lambda ),}
      [A=\int \lambda \,d\operatorname {E} _{A}(\lambda ),]
where EA is the resolution of the identity (also called projection-valued
measure) associated to A. Then the probability of the measurement outcome lying
in an interval B of R is |EA(B) Ï|2. In other words, the probability is
obtained by integrating the characteristic function of B against the countably
additive measure
         &#x27E8; &#x03C8; &#x2223;  E  A   &#x2061; &#x03C8; &#x27E9; .
      {\displaystyle \langle \psi \mid \operatorname {E} _{A}\psi \rangle .}
      [\langle \psi \mid \operatorname {E} _{A}\psi \rangle .]
    * If the measured value is contained in B, then immediately after the
      measurement, the system will be in the (generally non-normalized) state
      EA(B)Ï. If the measured value does not lie in B, replace B by its
      complement for the above state.
For example, suppose the state space is the n-dimensional complex Hilbert space
Cn and A is a Hermitian matrix with eigenvalues Î»i, with corresponding
eigenvectors Ïi. The projection-valued measure associated with A, EA, is then
          E  A   &#x2061; ( B ) =  |   &#x03C8;  i   &#x27E9; &#x27E8;
      &#x03C8;  i    |  ,   {\displaystyle \operatorname {E} _{A}(B)=|\psi _
      {i}\rangle \langle \psi _{i}|,}  [\operatorname {E} _{A}(B)=|\psi _
      {i}\rangle \langle \psi _{i}|,]
where B is a Borel set containing only the single eigenvalue Î»i. If the system
is prepared in state
          |  &#x03C8; &#x27E9;    {\displaystyle |\psi \rangle \,}  [|\psi
      \rangle \,]
Then the probability of a measurement returning the value Î»i can be calculated
by integrating the spectral measure
         &#x27E8; &#x03C8; &#x2223;  E  A   &#x2061; &#x03C8; &#x27E9;
      {\displaystyle \langle \psi \mid \operatorname {E} _{A}\psi \rangle }
      [\langle \psi \mid \operatorname {E} _{A}\psi \rangle ]
over Bi. This gives trivially
         &#x27E8; &#x03C8;  |   &#x03C8;  i   &#x27E9; &#x27E8;  &#x03C8;  i
      &#x2223; &#x03C8; &#x27E9; =  |  &#x27E8; &#x03C8; &#x2223;  &#x03C8;  i
      &#x27E9;   |   2   .   {\displaystyle \langle \psi |\psi _{i}\rangle
      \langle \psi _{i}\mid \psi \rangle =|\langle \psi \mid \psi _{i}\rangle
      |^{2}.}  [\langle \psi |\psi _{i}\rangle \langle \psi _{i}\mid \psi
      \rangle =|\langle \psi \mid \psi _{i}\rangle |^{2}.]
The characteristic property of the von Neumann measurement scheme is that
repeating the same measurement will give the same results. This is also called
the projection postulate.
A more general formulation replaces the projection-valued measure with a
positive-operator_valued_measure_(POVM). To illustrate, take again the finite-
dimensional case. Here we would replace the rank-1 projections
          |   &#x03C8;  i   &#x27E9; &#x27E8;  &#x03C8;  i    |
      {\displaystyle |\psi _{i}\rangle \langle \psi _{i}|\,}  [|\psi _
      {i}\rangle \langle \psi _{i}|\,]
by a finite set of positive operators
          F  i    F  i   &#x2217;      {\displaystyle F_{i}F_{i}^{*}\,}  [F_
      {i}F_{i}^{*}\,]
whose sum is still the identity operator as before (the resolution of
identity). Just as a set of possible outcomes {Î»1 ... Î»n}  is associated to a
projection-valued measure, the same can be said for a POVM. Suppose the
measurement outcome is Î»i. Instead of collapsing to the (unnormalized) state
          |   &#x03C8;  i   &#x27E9; &#x27E8;  &#x03C8;  i    |  &#x03C8;
      &#x27E9;    {\displaystyle |\psi _{i}\rangle \langle \psi _{i}|\psi
      \rangle \,}  [|\psi _{i}\rangle \langle \psi _{i}|\psi \rangle \,]
after the measurement, the system now will be in the state
          F  i    |  &#x03C8; &#x27E9; .    {\displaystyle F_{i}|\psi \rangle
      .\,}  [F_{i}|\psi \rangle .\,]
Since the Fi Fi* operators need not be mutually orthogonal projections, the
projection postulate of von Neumann no longer holds.
The same formulation applies to general mixed_states.
In von Neumann's approach, the state transformation due to measurement is
distinct from that due to time_evolution in several ways. For example, time
evolution is deterministic and unitary whereas measurement is non-deterministic
and non-unitary. However, since both types of state transformation take one
quantum state to another, this difference was viewed by many as unsatisfactory.
The POVM formalism views measurement as one among many other quantum
operations, which are described by completely_positive_maps which do not
increase the trace.
In any case it seems that the above-mentioned problems can only be resolved if
the time evolution included not only the quantum system, but also, and
essentially, the classical measurement apparatus (see above).
**** The relative state interpretation[edit] ****
An alternative interpretation of measurement is Everett's relative_state
interpretation, which was later dubbed the "many-worlds_interpretation" of
quantum physics.
***** List of mathematical tools[edit] *****
Part of the folklore of the subject concerns the mathematical_physics textbook
Methods_of_Mathematical_Physics put together by Richard_Courant from David
Hilbert's GÃ¶ttingen_University courses. The story is told (by mathematicians)
that physicists had dismissed the material as not interesting in the current
research areas, until the advent of SchrÃ¶dinger's equation. At that point it
was realised that the mathematics of the new quantum mechanics was already laid
out in it. It is also said that Heisenberg had consulted Hilbert about his
matrix_mechanics, and Hilbert observed that his own experience with infinite-
dimensional matrices had derived from differential equations, advice which
Heisenberg ignored, missing the opportunity to unify the theory as Weyl and
Dirac did a few years later. Whatever the basis of the anecdotes, the
mathematics of the theory was conventional at the time, whereas the physics was
radically new.
The main tools include:
    * linear_algebra: complex_numbers, eigenvectors, eigenvalues
    * functional_analysis: Hilbert_spaces, linear_operators, spectral_theory
    * differential_equations: partial_differential_equations, separation_of
      variables, ordinary_differential_equations, SturmâLiouville_theory,
      eigenfunctions
    * harmonic_analysis: Fourier_transforms
See also: list_of_mathematical_topics_in_quantum_theory
***** Notes[edit] *****
   1. ^ Frederick W. Byron, Robert W. Fuller; Mathematics_of_classical_and
      quantum_physics; Courier Dover Publications, 1992.
   2. ^Dirac, P. A. M. (1925). "The Fundamental Equations of Quantum
      Mechanics". Proceedings of the Royal Society A: Mathematical, Physical
      and Engineering Sciences. 109 (752): 642â653. Bibcode:
      1925RSPSA.109..642D. doi:10.1098/rspa.1925.0150.
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
   4. ^Sellier, Jean Michel (2015). "A signed particle formulation of non-
      relativistic quantum mechanics". Journal of Computational Physics. 297:
      254â265. arXiv:1509.06708. Bibcode:2015JCoPh.297..254S. doi:10.1016/
      j.jcp.2015.05.036.
   5. ^Solem, J. C.; Biedenharn, L. C. (1993). "Understanding geometrical
      phases in quantum mechanics: An elementary example". Foundations of
      Physics. 23 (2): 185â195. Bibcode:1993FoPh...23..185S. doi:10.1007/
      BF01883623.
   6. ^ G._Greenstein_and_A._Zajonc
***** References[edit] *****
    * J._von_Neumann, Mathematical Foundations of Quantum Mechanics (1932),
      Princeton University Press, 1955. Reprinted in paperback form.
    * H._Weyl, The Theory of Groups and Quantum Mechanics, Dover Publications,
      1950.
    * A._Gleason, Measures on the Closed Subspaces of a Hilbert Space, Journal
      of Mathematics and Mechanics, 1957.
    * G._Mackey, Mathematical Foundations of Quantum Mechanics, W. A. Benjamin,
      1963 (paperback reprint by Dover 2004).
    * R._F._Streater and A._S._Wightman, PCT, Spin and Statistics and All That,
      Benjamin 1964 (Reprinted by Princeton University Press)
    * R. Jost, The General Theory of Quantized Fields, American Mathematical
      Society, 1965.
    * J. M. Jauch, Foundations of quantum mechanics, Addison-Wesley Publ. Cy.,
      Reading, Massachusetts, 1968.
    * G. Emch, Algebraic Methods in Statistical Mechanics and Quantum Field
      Theory, Wiley-Interscience, 1972.
    * M._Reed and B._Simon, Methods of Mathematical Physics, vols IâIV,
      Academic Press 1972.
    * T.S._Kuhn, Black-Body_Theory_and_the_Quantum_Discontinuity, 1894â1912,
      Clarendon Press, Oxford and Oxford University Press, New York, 1978.
    * D. Edwards, The Mathematical Foundations of Quantum Mechanics, Synthese,
      42 (1979),pp. 1â70.
    * R. Shankar, "Principles of Quantum Mechanics", Springer, 1980.
    * E. Prugovecki, Quantum Mechanics in Hilbert Space, Dover, 1981.
    * S. Auyang, How is Quantum Field Theory Possible?, Oxford University
      Press, 1995.
    * N. Weaver, "Mathematical Quantization", Chapman & Hall/CRC 2001.
    * G. Giachetta, L. Mangiarotti, G._Sardanashvily, "Geometric and Algebraic
      Topological Methods in Quantum Mechanics", World Scientific, 2005.
    * David McMahon, "Quantum Mechanics Demystified", 2nd Ed., McGraw-Hill
      Professional, 2005.
    * G._Teschl, Mathematical Methods in Quantum Mechanics with Applications to
      SchrÃ¶dinger Operators, http://www.mat.univie.ac.at/~gerald/ftp/book-
      schroe/, American Mathematical Society, 2009.
    * V. Moretti, "Spectral Theory and Quantum Mechanics: Mathematical
      Foundations of Quantum Theories, Symmetries and Introduction to the
      Algebraic Formulation", 2nd Edition, Springer, 2018.
    * B. C. Hall, "Quantum Theory for Mathematicians", Springer, 2013.
    * V. Moretti, "Fundamental Mathematical Structures of Quantum Theory".
      Springer, 2019, https://www.springer.com/it/book/9783030183455#aboutBook
    * K. Landsman, "Foundations of Quantum Theory", Springer 2017
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

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Mathematical_formulation_of_quantum_mechanics&oldid=891047933"
Categories:
    * Quantum_mechanics
    * History_of_physics
Hidden categories:
    * Articles_with_short_description
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
    * Wikiversity
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * à¦¬à¦¾à¦à¦²à¦¾
    * CatalÃ 
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Hrvatski
    * Italiano
    * ×¢××¨××ª
    * Latina
    * Nederlands
    * æ¥æ¬èª
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 5 April 2019, at 09:06 (UTC).
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
