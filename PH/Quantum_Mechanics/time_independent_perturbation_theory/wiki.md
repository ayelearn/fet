The following text has been accessed from https://en.wikipedia.org/wiki/Perturbation_theory_(quantum_mechanics)#Time-independent_perturbation_theory at Fri Aug 9 03:11:48 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Perturbation theory (quantum mechanics) ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
application of mathematical perturbation theory to approximating Hamiltonians
of quantum mechanical systems
In quantum_mechanics, perturbation theory is a set of approximation schemes
directly related to mathematical perturbation for describing a complicated
quantum_system in terms of a simpler one. The idea is to start with a simple
system for which a mathematical solution is known, and add an additional
"perturbing" Hamiltonian representing a weak disturbance to the system. If the
disturbance is not too large, the various physical quantities associated with
the perturbed system (e.g. its energy_levels and eigenstates) can be expressed
as "corrections" to those of the simple system. These corrections, being small
compared to the size of the quantities themselves, can be calculated using
approximate methods such as asymptotic_series. The complicated system can
therefore be studied based on knowledge of the simpler one. In effect, it is
describing a complicated unsolved system using a simple, solved system.
⁰
***** Contents *****
    * 1_Approximate_Hamiltonians
    * 2_Applying_perturbation_theory
          o 2.1_Limitations
                # 2.1.1_Large_perturbations
                # 2.1.2_Non-adiabatic_states
                # 2.1.3_Difficult_computations
    * 3_Time-independent_perturbation_theory
          o 3.1_First_order_corrections
          o 3.2_Second-order_and_higher_corrections
          o 3.3_Effects_of_degeneracy
          o 3.4_Generalization_to_multi-parameter_case
                # 3.4.1_Hamiltonian_and_force_operator
                # 3.4.2_Perturbation_theory_as_power_series_expansion
                # 3.4.3_HellmannâFeynman_theorems
                # 3.4.4_Correction_of_energy_and_state
                # 3.4.5_Effective_Hamiltonian
    * 4_Time-dependent_perturbation_theory
          o 4.1_Method_of_variation_of_constants
          o 4.2_Method_of_Dyson_series
    * 5_Strong_perturbation_theory
    * 6_Examples
          o 6.1_Example_of_first_order_perturbation_theory_â_ground_state
            energy_of_the_quartic_oscillator
          o 6.2_Example_of_first_and_second_order_perturbation_theory_â
            quantum_pendulum
    * 7_References
***** Approximate Hamiltonians[edit] *****
Perturbation theory is an important tool for describing real quantum systems,
as it turns out to be very difficult to find exact solutions to the
SchrÃ¶dinger_equation for Hamiltonians of even moderate complexity. The
Hamiltonians to which we know exact solutions, such as the hydrogen_atom, the
quantum_harmonic_oscillator and the particle_in_a_box, are too idealized to
adequately describe most systems. Using perturbation theory, we can use the
known solutions of these simple Hamiltonians to generate solutions for a range
of more complicated systems.
***** Applying perturbation theory[edit] *****
Perturbation theory is applicable if the problem at hand cannot be solved
exactly, but can be formulated by adding a "small" term to the mathematical
description of the exactly solvable problem.
For example, by adding a perturbative electric_potential to the quantum
mechanical model of the hydrogen atom, tiny shifts in the spectral_lines of
hydrogen caused by the presence of an electric_field (the Stark_effect) can be
calculated. This is only approximate because the sum of a Coulomb_potential
with a linear potential is unstable (has no true bound states) although the
tunneling_time (decay_rate) is very long. This instability shows up as a
broadening of the energy spectrum lines, which perturbation theory fails to
reproduce entirely.
The expressions produced by perturbation theory are not exact, but they can
lead to accurate results as long as the expansion parameter, say Î±, is very
small. Typically, the results are expressed in terms of finite power_series in
Î± that seem to converge to the exact values when summed to higher order. After
a certain order n ~ 1/Î± however, the results become increasingly worse since
the series are usually divergent (being asymptotic_series). There exist ways to
convert them into convergent series, which can be evaluated for large-expansion
parameters, most efficiently by the variational_method.
In the theory of quantum_electrodynamics (QED), in which the electronâphoton
interaction is treated perturbatively, the calculation of the electron's
magnetic_moment has been found to agree with experiment to eleven decimal
places.[1] In QED and other quantum_field_theories, special calculation
techniques known as Feynman_diagrams are used to systematically sum the power
series terms.
**** Limitations[edit] ****
*** Large perturbations[edit] ***
Under some circumstances, perturbation theory is an invalid approach to take.
This happens when the system we wish to describe cannot be described by a small
perturbation imposed on some simple system. In quantum_chromodynamics, for
instance, the interaction of quarks with the gluon field cannot be treated
perturbatively at low energies because the coupling_constant (the expansion
parameter) becomes too large.[clarification_needed]
*** Non-adiabatic states[edit] ***
Perturbation theory also fails to describe states that are not generated
adiabatically from the "free model", including bound_states and various
collective phenomena such as solitons.[citation_needed] Imagine, for example,
that we have a system of free (i.e. non-interacting) particles, to which an
attractive interaction is introduced. Depending on the form of the interaction,
this may create an entirely new set of eigenstates corresponding to groups of
particles bound to one another. An example of this phenomenon may be found in
conventional superconductivity, in which the phonon-mediated attraction between
conduction_electrons leads to the formation of correlated electron pairs known
as Cooper_pairs. When faced with such systems, one usually turns to other
approximation schemes, such as the variational_method and the WKB
approximation. This is because there is no analogue of a bound_particle in the
unperturbed model and the energy of a soliton typically goes as the inverse of
the expansion parameter. However, if we "integrate" over the solitonic
phenomena, the nonperturbative corrections in this case will be tiny; of the
order of exp(â1/g) or exp(â1/g2) in the perturbation parameter g.
Perturbation theory can only detect solutions "close" to the unperturbed
solution, even if there are other solutions for which the perturbative
expansion is not valid.[citation_needed]
*** Difficult computations[edit] ***
The problem of non-perturbative systems has been somewhat alleviated by the
advent of modern computers. It has become practical to obtain numerical non-
perturbative solutions for certain problems, using methods such as density
functional_theory. These advances have been of particular benefit to the field
of quantum_chemistry.[2] Computers have also been used to carry out
perturbation theory calculations to extraordinarily high levels of precision,
which has proven important in particle_physics for generating theoretical
results that can be compared with experiment.
***** Time-independent perturbation theory[edit] *****
Time-independent perturbation theory is one of two categories of perturbation
theory, the other being time-dependent perturbation (see next section). In
time-independent perturbation theory the perturbation Hamiltonian is static
(i.e., possesses no time dependence). Time-independent perturbation theory was
presented by Erwin_SchrÃ¶dinger in a 1926 paper,[3] shortly after he produced
his theories in wave mechanics. In this paper SchrÃ¶dinger referred to earlier
work of Lord_Rayleigh,[4] who investigated harmonic vibrations of a string
perturbed by small inhomogeneities. This is why this perturbation theory is
often referred to as RayleighâSchrÃ¶dinger perturbation theory.[5]
**** First order corrections[edit] ****
We begin[6] with an unperturbed Hamiltonian H0, which is also assumed to have
no time dependence. It has known energy levels and eigenstates, arising from
the time-independent SchrÃ¶dinger_equation:
          H  0    |  n  ( 0 )   &#x27E9;  =  E  n   ( 0 )    |  n  ( 0 )
      &#x27E9;  ,  n = 1 , 2 , 3 , &#x22EF;   {\displaystyle H_{0}\left|n^{
      (0)}\right\rangle =E_{n}^{(0)}\left|n^{(0)}\right\rangle ,\qquad
      n=1,2,3,\cdots }  [H_{0}\left|n^{(0)}\right\rangle =E_{n}^{(0)}\left|n^{
      (0)}\right\rangle ,\qquad n=1,2,3,\cdots ]
For simplicity, we have assumed that the energies are discrete. The (0)
superscripts denote that these quantities are associated with the unperturbed
system. Note the use of braâket_notation.
We now introduce a perturbation to the Hamiltonian. Let V be a Hamiltonian
representing a weak physical disturbance, such as a potential energy produced
by an external field. (Thus, V is formally a Hermitian_operator.) Let Î» be a
dimensionless parameter that can take on values ranging continuously from 0 (no
perturbation) to 1 (the full perturbation). The perturbed Hamiltonian is
         H =  H  0   + &#x03BB; V   {\displaystyle H=H_{0}+\lambda V}  [H=H_
      {0}+\lambda V]
The energy levels and eigenstates of the perturbed Hamiltonian are again given
by the SchrÃ¶dinger equation,
          (   H  0   + &#x03BB; V  )   |  n &#x27E9; =  E  n    |  n &#x27E9; .
      {\displaystyle \left(H_{0}+\lambda V\right)|n\rangle =E_{n}|n\rangle .}
      [\left(H_{0}+\lambda V\right)|n\rangle =E_{n}|n\rangle .]
Our goal is to express En and      |  n &#x27E9;   {\displaystyle |n\rangle }
[|n\rangle ] in terms of the energy levels and eigenstates of the old
Hamiltonian. If the perturbation is sufficiently weak, we can write them as a
(Maclaurin) power_series in Î»,
              E  n      =  E  n   ( 0 )   + &#x03BB;  E  n   ( 1 )   +
      &#x03BB;  2    E  n   ( 2 )   + &#x22EF;      |  n &#x27E9;    =  |  n
      ( 0 )   &#x27E9;  + &#x03BB;  |  n  ( 1 )   &#x27E9;  +  &#x03BB;  2    |
      n  ( 2 )   &#x27E9;  + &#x22EF;       {\displaystyle {\begin{aligned}E_
      {n}&=E_{n}^{(0)}+\lambda E_{n}^{(1)}+\lambda ^{2}E_{n}^{(2)}+\cdots
      \\|n\rangle &=\left|n^{(0)}\right\rangle +\lambda \left|n^{
      (1)}\right\rangle +\lambda ^{2}\left|n^{(2)}\right\rangle +\cdots \end
      {aligned}}}  [{\begin{aligned}E_{n}&=E_{n}^{(0)}+\lambda E_{n}^{
      (1)}+\lambda ^{2}E_{n}^{(2)}+\cdots \\|n\rangle &=\left|n^{
      (0)}\right\rangle +\lambda \left|n^{(1)}\right\rangle +\lambda ^
      {2}\left|n^{(2)}\right\rangle +\cdots \end{aligned}}]
where
              E  n   ( k )      =   1  k !        d  k    E  n     d  &#x03BB;
      k         |    &#x03BB; = 0        |  n  ( k )   &#x27E9;     =   1  k !
      d  k    |  n &#x27E9;   d  &#x03BB;  k         |    &#x03BB; = 0.
      {\displaystyle {\begin{aligned}E_{n}^{(k)}&={\frac {1}{k!}}{\frac {d^
      {k}E_{n}}{d\lambda ^{k}}}{\bigg |}_{\lambda =0}\\\left|n^{
      (k)}\right\rangle &={\frac {1}{k!}}{\frac {d^{k}|n\rangle }{d\lambda ^
      {k}}}{\bigg |}_{\lambda =0.}\end{aligned}}}  [{\displaystyle {\begin
      {aligned}E_{n}^{(k)}&={\frac {1}{k!}}{\frac {d^{k}E_{n}}{d\lambda ^{k}}}
      {\bigg |}_{\lambda =0}\\\left|n^{(k)}\right\rangle &={\frac {1}{k!}}
      {\frac {d^{k}|n\rangle }{d\lambda ^{k}}}{\bigg |}_{\lambda =0.}\end
      {aligned}}}]
When k = 0, these reduce to the unperturbed values, which are the first term in
each series. Since the perturbation is weak, the energy levels and eigenstates
should not deviate too much from their unperturbed values, and the terms should
rapidly become smaller as we go to higher order.
Substituting the power series expansion into the SchrÃ¶dinger equation, we
obtain
    (   H  0   + &#x03BB; V  )   (   |  n  ( 0 )   &#x27E9;  + &#x03BB;  |  n
( 1 )   &#x27E9;  + &#x22EF;  )  =  (   E  n   ( 0 )   + &#x03BB;  E  n   ( 1 )
+ &#x22EF;  )   (   |  n  ( 0 )   &#x27E9;  + &#x03BB;  |  n  ( 1 )   &#x27E9;
+ &#x22EF;  )  .   {\displaystyle \left(H_{0}+\lambda V\right)\left(\left|n^{
(0)}\right\rangle +\lambda \left|n^{(1)}\right\rangle +\cdots \right)=\left(E_
{n}^{(0)}+\lambda E_{n}^{(1)}+\cdots \right)\left(\left|n^{(0)}\right\rangle
+\lambda \left|n^{(1)}\right\rangle +\cdots \right).}  [{\displaystyle \left(H_
{0}+\lambda V\right)\left(\left|n^{(0)}\right\rangle +\lambda \left|n^{
(1)}\right\rangle +\cdots \right)=\left(E_{n}^{(0)}+\lambda E_{n}^{(1)}+\cdots
\right)\left(\left|n^{(0)}\right\rangle +\lambda \left|n^{(1)}\right\rangle
+\cdots \right).}]

Expanding this equation and comparing coefficients of each power of Î» results
in an infinite series of simultaneous_equations. The zeroth-order equation is
simply the SchrÃ¶dinger equation for the unperturbed system.
The first-order equation is
          H  0    |  n  ( 1 )   &#x27E9;  + V  |  n  ( 0 )   &#x27E9;  =  E  n
      ( 0 )    |  n  ( 1 )   &#x27E9;  +  E  n   ( 1 )    |  n  ( 0 )
      &#x27E9;  .   {\displaystyle H_{0}\left|n^{(1)}\right\rangle +V\left|n^{
      (0)}\right\rangle =E_{n}^{(0)}\left|n^{(1)}\right\rangle +E_{n}^{
      (1)}\left|n^{(0)}\right\rangle .}  [{\displaystyle H_{0}\left|n^{
      (1)}\right\rangle +V\left|n^{(0)}\right\rangle =E_{n}^{(0)}\left|n^{
      (1)}\right\rangle +E_{n}^{(1)}\left|n^{(0)}\right\rangle .}]
Operating through by     &#x27E8;  n  ( 0 )    |    {\displaystyle \langle n^{
(0)}|}  [\langle n^{(0)}|], the first term on the left-hand side cancels the
first term on the right-hand side. (Recall, the unperturbed Hamiltonian is
Hermitian). This leads to the first-order energy shift,
          E  n   ( 1 )   =  &#x27E8;  n  ( 0 )   |  V  |  n  ( 0 )   &#x27E9;
      .   {\displaystyle E_{n}^{(1)}=\left\langle n^{(0)}\right|V\left|n^{
      (0)}\right\rangle .}  [{\displaystyle E_{n}^{(1)}=\left\langle n^{
      (0)}\right|V\left|n^{(0)}\right\rangle .}]
This is simply the expectation_value of the perturbation Hamiltonian while the
system is in the unperturbed state.
This result can be interpreted in the following way: suppose the perturbation
is applied, but we keep the system in the quantum state      |   n  ( 0 )
&#x27E9;   {\displaystyle |n^{(0)}\rangle }  [|n^{(0)}\rangle ], which is a
valid quantum state though no longer an energy eigenstate. The perturbation
causes the average energy of this state to increase by     &#x27E8;  n  ( 0 )
|  V  |   n  ( 0 )   &#x27E9;   {\displaystyle \langle n^{(0)}|V|n^{(0)}\rangle
}  [\langle n^{(0)}|V|n^{(0)}\rangle ]. However, the true energy shift is
slightly different, because the perturbed eigenstate is not exactly the same as
|   n  ( 0 )   &#x27E9;   {\displaystyle |n^{(0)}\rangle }  [|n^{(0)}\rangle ].
These further shifts are given by the second and higher order corrections to
the energy.
Before we compute the corrections to the energy eigenstate, we need to address
the issue of normalization. We may suppose
          &#x27E8;  n  ( 0 )   |     n  ( 0 )   &#x27E9;  = 1 ,
      {\displaystyle \left\langle n^{(0)}\right|\left.n^{(0)}\right\rangle =1,}
      [\left\langle n^{(0)}\right|\left.n^{(0)}\right\rangle =1,]
but perturbation theory assumes we also have     &#x27E8; n  |  n &#x27E9; = 1
{\displaystyle \langle n|n\rangle =1}  [\langle n|n\rangle =1].
It follows that at first order in Î», we must have
          (   &#x27E8;  n  ( 0 )   |  + &#x03BB;  &#x27E8;  n  ( 1 )   |   )
      (   |  n  ( 0 )   &#x27E9;  + &#x03BB;  |  n  ( 1 )   &#x27E9;   )  = 1
      {\displaystyle \left(\left\langle n^{(0)}\right|+\lambda \left\langle n^{
      (1)}\right|\right)\left(\left|n^{(0)}\right\rangle +\lambda \left|n^{
      (1)}\right\rangle \right)=1}  [\left(\left\langle n^{(0)}\right|+\lambda
      \left\langle n^{(1)}\right|\right)\left(\left|n^{(0)}\right\rangle
      +\lambda \left|n^{(1)}\right\rangle \right)=1]
          &#x27E8;  n  ( 0 )   |     n  ( 0 )   &#x27E9;  + &#x03BB;  &#x27E8;
      n  ( 0 )   |     n  ( 1 )   &#x27E9;  + &#x03BB;  &#x27E8;  n  ( 1 )   |
      n  ( 0 )   &#x27E9;  +    &#x03BB;  2    &#x27E8;  n  ( 1 )   |     n
      ( 1 )   &#x27E9;    = 1   {\displaystyle \left\langle n^{
      (0)}\right|\left.n^{(0)}\right\rangle +\lambda \left\langle n^{
      (0)}\right|\left.n^{(1)}\right\rangle +\lambda \left\langle n^{
      (1)}\right|\left.n^{(0)}\right\rangle +{\cancel {\lambda ^{2}\left\langle
      n^{(1)}\right|\left.n^{(1)}\right\rangle }}=1}  [\left\langle n^{
      (0)}\right|\left.n^{(0)}\right\rangle +\lambda \left\langle n^{
      (0)}\right|\left.n^{(1)}\right\rangle +\lambda \left\langle n^{
      (1)}\right|\left.n^{(0)}\right\rangle +{\cancel {\lambda ^{2}\left\langle
      n^{(1)}\right|\left.n^{(1)}\right\rangle }}=1]
          &#x27E8;  n  ( 0 )   |     n  ( 1 )   &#x27E9;  +  &#x27E8;  n  ( 1 )
      |     n  ( 0 )   &#x27E9;  = 0.   {\displaystyle \left\langle n^{
      (0)}\right|\left.n^{(1)}\right\rangle +\left\langle n^{
      (1)}\right|\left.n^{(0)}\right\rangle =0.}  [\left\langle n^{
      (0)}\right|\left.n^{(1)}\right\rangle +\left\langle n^{
      (1)}\right|\left.n^{(0)}\right\rangle =0.]
Since the overall phase is not determined in quantum mechanics, without_loss_of
generality, in time independent theory we may assume     &#x27E8;  n  ( 0 )
|   n  ( 1 )   &#x27E9;   {\displaystyle \langle n^{(0)}|n^{(1)}\rangle }  [
{\displaystyle \langle n^{(0)}|n^{(1)}\rangle }] is purely real. Therefore,
          &#x27E8;  n  ( 0 )   |     n  ( 1 )   &#x27E9;  =  &#x27E8;  n  ( 1 )
      |     n  ( 0 )   &#x27E9;  ,   {\displaystyle \left\langle n^{
      (0)}\right|\left.n^{(1)}\right\rangle =\left\langle n^{
      (1)}\right|\left.n^{(0)}\right\rangle ,}  [{\displaystyle \left\langle n^
      {(0)}\right|\left.n^{(1)}\right\rangle =\left\langle n^{
      (1)}\right|\left.n^{(0)}\right\rangle ,}]
leading to
          &#x27E8;  n  ( 0 )   |     n  ( 1 )   &#x27E9;  = 0.   {\displaystyle
      \left\langle n^{(0)}\right|\left.n^{(1)}\right\rangle =0.}  [\left\langle
      n^{(0)}\right|\left.n^{(1)}\right\rangle =0.]
To obtain the first-order correction to the energy eigenstate, we insert our
expression for the first-order energy correction back into the result shown
above equating the first-order coefficients of Î». We then make use of the
resolution_of_the_identity,
             V  |  n  ( 0 )   &#x27E9;     =  (   &#x2211;  k &#x2260; n    |
      k  ( 0 )   &#x27E9;   &#x27E8;  k  ( 0 )   |   )  V  |  n  ( 0 )
      &#x27E9;  +  (   |  n  ( 0 )   &#x27E9;   &#x27E8;  n  ( 0 )   |   )  V
      |  n  ( 0 )   &#x27E9;        =  &#x2211;  k &#x2260; n    |  k  ( 0 )
      &#x27E9;   &#x27E8;  k  ( 0 )   |  V  |  n  ( 0 )   &#x27E9;  +  E  n
      ( 1 )    |  n  ( 0 )   &#x27E9;  ,       {\displaystyle {\begin
      {aligned}V\left|n^{(0)}\right\rangle &=\left(\sum _{k\neq n}\left|k^{
      (0)}\right\rangle \left\langle k^{(0)}\right|\right)V\left|n^{
      (0)}\right\rangle +\left(\left|n^{(0)}\right\rangle \left\langle n^{
      (0)}\right|\right)V\left|n^{(0)}\right\rangle \\&=\sum _{k\neq n}\left|k^
      {(0)}\right\rangle \left\langle k^{(0)}\right|V\left|n^{(0)}\right\rangle
      +E_{n}^{(1)}\left|n^{(0)}\right\rangle ,\end{aligned}}}  [{\begin
      {aligned}V\left|n^{(0)}\right\rangle &=\left(\sum _{k\neq n}\left|k^{
      (0)}\right\rangle \left\langle k^{(0)}\right|\right)V\left|n^{
      (0)}\right\rangle +\left(\left|n^{(0)}\right\rangle \left\langle n^{
      (0)}\right|\right)V\left|n^{(0)}\right\rangle \\&=\sum _{k\neq n}\left|k^
      {(0)}\right\rangle \left\langle k^{(0)}\right|V\left|n^{(0)}\right\rangle
      +E_{n}^{(1)}\left|n^{(0)}\right\rangle ,\end{aligned}}]
where the      |   k  ( 0 )   &#x27E9;   {\displaystyle |k^{(0)}\rangle }  [|k^
{(0)}\rangle ] are in the orthogonal_complement of      |   n  ( 0 )   &#x27E9;
{\displaystyle |n^{(0)}\rangle }  [|n^{(0)}\rangle ].
The first-order equation may thus be expressed as
          (   E  n   ( 0 )   &#x2212;  H  0    )   |  n  ( 1 )   &#x27E9;  =
      &#x2211;  k &#x2260; n    |  k  ( 0 )   &#x27E9;   &#x27E8;  k  ( 0 )   |
      V  |  n  ( 0 )   &#x27E9;  .   {\displaystyle \left(E_{n}^{(0)}-H_
      {0}\right)\left|n^{(1)}\right\rangle =\sum _{k\neq n}\left|k^{
      (0)}\right\rangle \left\langle k^{(0)}\right|V\left|n^{(0)}\right\rangle
      .}  [{\displaystyle \left(E_{n}^{(0)}-H_{0}\right)\left|n^{
      (1)}\right\rangle =\sum _{k\neq n}\left|k^{(0)}\right\rangle \left\langle
      k^{(0)}\right|V\left|n^{(0)}\right\rangle .}]
For the moment, suppose that the zeroth-order energy level is not degenerate,
i.e. there is no eigenstate of H0 in the orthogonal complement of      |   n
( 0 )   &#x27E9;   {\displaystyle |n^{(0)}\rangle }  [|n^{(0)}\rangle ] with
the energy      E  n   ( 0 )     {\displaystyle E_{n}^{(0)}}  [E_{n}^{(0)}].
After renaming the summation dummy index above as      k &#x2032;
{\displaystyle k'}  [k'], we can pick any     k &#x2260; n   {\displaystyle
k\neq n}  [k\neq n], and multiply through by     &#x27E8;  k  ( 0 )    |
{\displaystyle \langle k^{(0)}|}  [\langle k^{(0)}|] giving
          (   E  n   ( 0 )   &#x2212;  E  k   ( 0 )    )   &#x27E8;  k  ( 0 )
      |  n  ( 1 )   &#x27E9;  =  &#x27E8;  k  ( 0 )   |  V  |  n  ( 0 )
      &#x27E9;  .   {\displaystyle \left(E_{n}^{(0)}-E_{k}^{
      (0)}\right)\left\langle k^{(0)}\right.\left|n^{(1)}\right\rangle
      =\left\langle k^{(0)}\right|V\left|n^{(0)}\right\rangle .}  [
      {\displaystyle \left(E_{n}^{(0)}-E_{k}^{(0)}\right)\left\langle k^{
      (0)}\right.\left|n^{(1)}\right\rangle =\left\langle k^{
      (0)}\right|V\left|n^{(0)}\right\rangle .}]
We see that the above     &#x27E8;  k  ( 0 )    |   n  ( 1 )   &#x27E9;
{\displaystyle \langle k^{(0)}|n^{(1)}\rangle }  [{\displaystyle \langle k^{
(0)}|n^{(1)}\rangle }] also gives us the component of the first-order
correction along      |   k  ( 0 )   &#x27E9;   {\displaystyle |k^{(0)}\rangle
}  [|k^{(0)}\rangle ].
Thus, in total, we get,
          |  n  ( 1 )   &#x27E9;  =  &#x2211;  k &#x2260; n       &#x27E8;  k
      ( 0 )   |  V  |  n  ( 0 )   &#x27E9;     E  n   ( 0 )   &#x2212;  E  k
      ( 0 )       |  k  ( 0 )   &#x27E9;  .   {\displaystyle \left|n^{
      (1)}\right\rangle =\sum _{k\neq n}{\frac {\left\langle k^{
      (0)}\right|V\left|n^{(0)}\right\rangle }{E_{n}^{(0)}-E_{k}^{
      (0)}}}\left|k^{(0)}\right\rangle .}  [{\displaystyle \left|n^{
      (1)}\right\rangle =\sum _{k\neq n}{\frac {\left\langle k^{
      (0)}\right|V\left|n^{(0)}\right\rangle }{E_{n}^{(0)}-E_{k}^{
      (0)}}}\left|k^{(0)}\right\rangle .}]
The first-order change in the n-th energy eigenket has a contribution from each
of the energy eigenstates k â  n. Each term is proportional to the matrix
element     &#x27E8;  k  ( 0 )    |  V  |   n  ( 0 )   &#x27E9;
{\displaystyle \langle k^{(0)}|V|n^{(0)}\rangle }  [\langle k^{(0)}|V|n^{
(0)}\rangle ], which is a measure of how much the perturbation mixes eigenstate
n with eigenstate k; it is also inversely proportional to the energy difference
between eigenstates k and n, which means that the perturbation deforms the
eigenstate to a greater extent if there are more eigenstates at nearby
energies. We see also that the expression is singular if any of these states
have the same energy as state n, which is why we assumed that there is no
degeneracy.
**** Second-order and higher corrections[edit] ****
We can find the higher-order deviations by a similar procedure, though the
calculations become quite tedious with our current formulation. Our
normalization prescription gives that
         2  &#x27E8;  n  ( 0 )   |     n  ( 2 )   &#x27E9;  +  &#x27E8;  n  ( 1
      )   |     n  ( 1 )   &#x27E9;  = 0.   {\displaystyle 2\left\langle n^{
      (0)}\right|\left.n^{(2)}\right\rangle +\left\langle n^{
      (1)}\right|\left.n^{(1)}\right\rangle =0.}  [2\left\langle n^{
      (0)}\right|\left.n^{(2)}\right\rangle +\left\langle n^{
      (1)}\right|\left.n^{(1)}\right\rangle =0.]
Up to second order, the expressions for the energies and (normalized)
eigenstates are:
          E  n   ( &#x03BB; ) =  E  n   ( 0 )   + &#x03BB;  &#x27E8;  n  ( 0 )
      |  V  |  n  ( 0 )   &#x27E9;  +  &#x03BB;  2    &#x2211;  k &#x2260; n
      |   &#x27E8;  k  ( 0 )   |  V  |  n  ( 0 )   &#x27E9;   |   2     E  n
      ( 0 )   &#x2212;  E  k   ( 0 )      + O (  &#x03BB;  3   )
      {\displaystyle E_{n}(\lambda )=E_{n}^{(0)}+\lambda \left\langle n^{
      (0)}\right|V\left|n^{(0)}\right\rangle +\lambda ^{2}\sum _{k\neq n}{\frac
      {\left|\left\langle k^{(0)}\right|V\left|n^{(0)}\right\rangle \right|^
      {2}}{E_{n}^{(0)}-E_{k}^{(0)}}}+O(\lambda ^{3})}  [E_{n}(\lambda )=E_{n}^{
      (0)}+\lambda \left\langle n^{(0)}\right|V\left|n^{(0)}\right\rangle
      +\lambda ^{2}\sum _{k\neq n}{\frac {\left|\left\langle k^{
      (0)}\right|V\left|n^{(0)}\right\rangle \right|^{2}}{E_{n}^{(0)}-E_{k}^{
      (0)}}}+O(\lambda ^{3})]
              |  n ( &#x03BB; ) &#x27E9; =  |  n  ( 0 )   &#x27E9;     +
      &#x03BB;  &#x2211;  k &#x2260; n    |  k  ( 0 )   &#x27E9;      &#x27E8;
      k  ( 0 )   |  V  |  n  ( 0 )   &#x27E9;     E  n   ( 0 )   &#x2212;  E  k
      ( 0 )      +  &#x03BB;  2    &#x2211;  k &#x2260; n    &#x2211;  &#x2113;
      &#x2260; n    |  k  ( 0 )   &#x27E9;      &#x27E8;  k  ( 0 )   |  V  |
      &#x2113;  ( 0 )   &#x27E9;   &#x27E8;  &#x2113;  ( 0 )   |  V  |  n  ( 0
      )   &#x27E9;     (   E  n   ( 0 )   &#x2212;  E  k   ( 0 )    )   (   E
      n   ( 0 )   &#x2212;  E  &#x2113;   ( 0 )    )           &#x2212;
      &#x03BB;  2    &#x2211;  k &#x2260; n    |  k  ( 0 )   &#x27E9;
      &#x27E8;  n  ( 0 )   |  V  |  n  ( 0 )   &#x27E9;   &#x27E8;  k  ( 0 )
      |  V  |  n  ( 0 )   &#x27E9;     (   E  n   ( 0 )   &#x2212;  E  k   ( 0
      )    )   2     &#x2212;   1 2    &#x03BB;  2    |  n  ( 0 )   &#x27E9;
      &#x2211;  k &#x2260; n       &#x27E8;  n  ( 0 )   |  V  |  k  ( 0 )
      &#x27E9;   &#x27E8;  k  ( 0 )   |  V  |  n  ( 0 )   &#x27E9;     (   E  n
      ( 0 )   &#x2212;  E  k   ( 0 )    )   2     + O (  &#x03BB;  3   ) .
      {\displaystyle {\begin{aligned}|n(\lambda )\rangle =\left|n^{
      (0)}\right\rangle &+\lambda \sum _{k\neq n}\left|k^{(0)}\right\rangle
      {\frac {\left\langle k^{(0)}\right|V\left|n^{(0)}\right\rangle }{E_{n}^{
      (0)}-E_{k}^{(0)}}}+\lambda ^{2}\sum _{k\neq n}\sum _{\ell \neq n}\left|k^
      {(0)}\right\rangle {\frac {\left\langle k^{(0)}\right|V\left|\ell ^{
      (0)}\right\rangle \left\langle \ell ^{(0)}\right|V\left|n^{
      (0)}\right\rangle }{\left(E_{n}^{(0)}-E_{k}^{(0)}\right)\left(E_{n}^{
      (0)}-E_{\ell }^{(0)}\right)}}\\&-\lambda ^{2}\sum _{k\neq n}\left|k^{
      (0)}\right\rangle {\frac {\left\langle n^{(0)}\right|V\left|n^{
      (0)}\right\rangle \left\langle k^{(0)}\right|V\left|n^{(0)}\right\rangle
      }{\left(E_{n}^{(0)}-E_{k}^{(0)}\right)^{2}}}-{\frac {1}{2}}\lambda ^
      {2}\left|n^{(0)}\right\rangle \sum _{k\neq n}{\frac {\left\langle n^{
      (0)}\right|V\left|k^{(0)}\right\rangle \left\langle k^{
      (0)}\right|V\left|n^{(0)}\right\rangle }{\left(E_{n}^{(0)}-E_{k}^{
      (0)}\right)^{2}}}+O(\lambda ^{3}).\end{aligned}}}  [{\begin{aligned}|n
      (\lambda )\rangle =\left|n^{(0)}\right\rangle &+\lambda \sum _{k\neq
      n}\left|k^{(0)}\right\rangle {\frac {\left\langle k^{(0)}\right|V\left|n^
      {(0)}\right\rangle }{E_{n}^{(0)}-E_{k}^{(0)}}}+\lambda ^{2}\sum _{k\neq
      n}\sum _{\ell \neq n}\left|k^{(0)}\right\rangle {\frac {\left\langle k^{
      (0)}\right|V\left|\ell ^{(0)}\right\rangle \left\langle \ell ^{
      (0)}\right|V\left|n^{(0)}\right\rangle }{\left(E_{n}^{(0)}-E_{k}^{
      (0)}\right)\left(E_{n}^{(0)}-E_{\ell }^{(0)}\right)}}\\&-\lambda ^{2}\sum
      _{k\neq n}\left|k^{(0)}\right\rangle {\frac {\left\langle n^{
      (0)}\right|V\left|n^{(0)}\right\rangle \left\langle k^{
      (0)}\right|V\left|n^{(0)}\right\rangle }{\left(E_{n}^{(0)}-E_{k}^{
      (0)}\right)^{2}}}-{\frac {1}{2}}\lambda ^{2}\left|n^{(0)}\right\rangle
      \sum _{k\neq n}{\frac {\left\langle n^{(0)}\right|V\left|k^{
      (0)}\right\rangle \left\langle k^{(0)}\right|V\left|n^{(0)}\right\rangle
      }{\left(E_{n}^{(0)}-E_{k}^{(0)}\right)^{2}}}+O(\lambda ^{3}).\end
      {aligned}}]
Extending the process further, the third-order energy correction can be shown
to be [7]
          E  n   ( 3 )   =  &#x2211;  k &#x2260; n    &#x2211;  m &#x2260; n
      &#x27E8;  n  ( 0 )    |  V  |   m  ( 0 )   &#x27E9; &#x27E8;  m  ( 0 )
      |  V  |   k  ( 0 )   &#x27E9; &#x27E8;  k  ( 0 )    |  V  |   n  ( 0 )
      &#x27E9;    (   E  n   ( 0 )   &#x2212;  E  m   ( 0 )    )   (   E  n
      ( 0 )   &#x2212;  E  k   ( 0 )    )     &#x2212; &#x27E8;  n  ( 0 )    |
      V  |   n  ( 0 )   &#x27E9;  &#x2211;  m &#x2260; n       |  &#x27E8;  n
      ( 0 )    |  V  |   m  ( 0 )   &#x27E9;   |   2      (   E  n   ( 0 )
      &#x2212;  E  m   ( 0 )    )   2     .   {\displaystyle E_{n}^{(3)}=\sum _
      {k\neq n}\sum _{m\neq n}{\frac {\langle n^{(0)}|V|m^{(0)}\rangle \langle
      m^{(0)}|V|k^{(0)}\rangle \langle k^{(0)}|V|n^{(0)}\rangle }{\left(E_{n}^{
      (0)}-E_{m}^{(0)}\right)\left(E_{n}^{(0)}-E_{k}^{(0)}\right)}}-\langle n^{
      (0)}|V|n^{(0)}\rangle \sum _{m\neq n}{\frac {|\langle n^{(0)}|V|m^{
      (0)}\rangle |^{2}}{\left(E_{n}^{(0)}-E_{m}^{(0)}\right)^{2}}}.}  [
      {\displaystyle E_{n}^{(3)}=\sum _{k\neq n}\sum _{m\neq n}{\frac {\langle
      n^{(0)}|V|m^{(0)}\rangle \langle m^{(0)}|V|k^{(0)}\rangle \langle k^{
      (0)}|V|n^{(0)}\rangle }{\left(E_{n}^{(0)}-E_{m}^{(0)}\right)\left(E_{n}^{
      (0)}-E_{k}^{(0)}\right)}}-\langle n^{(0)}|V|n^{(0)}\rangle \sum _{m\neq
      n}{\frac {|\langle n^{(0)}|V|m^{(0)}\rangle |^{2}}{\left(E_{n}^{(0)}-E_
      {m}^{(0)}\right)^{2}}}.}]
Corrections to fifth order (energies) and fourth order (states) in compact
notation
If we introduce the notation,
          V  n m   &#x2261; &#x27E8;  n  ( 0 )    |  V  |   m  ( 0 )   &#x27E9;
      {\displaystyle V_{nm}\equiv \langle n^{(0)}|V|m^{(0)}\rangle }  [V_
      {nm}\equiv \langle n^{(0)}|V|m^{(0)}\rangle ],
          E  n m   &#x2261;  E  n   ( 0 )   &#x2212;  E  m   ( 0 )
      {\displaystyle E_{nm}\equiv E_{n}^{(0)}-E_{m}^{(0)}}  [E_{nm}\equiv E_
      {n}^{(0)}-E_{m}^{(0)}],
then the energy corrections to fifth order can be written
              E  n   ( 1 )      =  V  n n        E  n   ( 2 )      =     |   V
      n  k  2       |   2     E  n  k  2            E  n   ( 3 )      =     V
      n  k  3      V   k  3    k  2      V   k  2   n      E  n  k  2      E  n
      k  3        &#x2212;  V  n n       |   V  n  k  3       |   2     E  n  k
      3     2          E  n   ( 4 )      =     V  n  k  4      V   k  4    k  3
      V   k  3    k  2      V   k  2   n      E  n  k  2      E  n  k  3      E
      n  k  4        &#x2212;     |   V  n  k  4       |   2     E  n  k  4
      2         |   V  n  k  2       |   2     E  n  k  2       &#x2212;  V  n
      n       V  n  k  4      V   k  4    k  3      V   k  3   n      E  n  k
      3     2    E  n  k  4        &#x2212;  V  n n       V  n  k  4      V   k
      4    k  2      V   k  2   n      E  n  k  2      E  n  k  4     2      +
      V  n n   2       |   V  n  k  4       |   2     E  n  k  4     3
      =     V  n  k  4      V   k  4    k  3      V   k  3    k  2      V   k
      2   n      E  n  k  2      E  n  k  3      E  n  k  4        &#x2212;  E
      n   ( 2 )       |   V  n  k  4       |   2     E  n  k  4     2
      &#x2212; 2  V  n n       V  n  k  4      V   k  4    k  3      V   k  3
      n      E  n  k  3     2    E  n  k  4        +  V  n n   2       |   V  n
      k  4       |   2     E  n  k  4     3          E  n   ( 5 )      =     V
      n  k  5      V   k  5    k  4      V   k  4    k  3      V   k  3    k  2
      V   k  2   n      E  n  k  2      E  n  k  3      E  n  k  4      E  n  k
      5        &#x2212;     V  n  k  5      V   k  5    k  4      V   k  4   n
      E  n  k  4     2    E  n  k  5            |   V  n  k  2       |   2
      E  n  k  2       &#x2212;     V  n  k  5      V   k  5    k  2      V   k
      2   n      E  n  k  2      E  n  k  5     2          |   V  n  k  2
      |   2     E  n  k  2       &#x2212;     |   V  n  k  5       |   2     E
      n  k  5     2         V  n  k  3      V   k  3    k  2      V   k  2   n
      E  n  k  2      E  n  k  3               &#x2212;  V  n n       V  n  k
      5      V   k  5    k  4      V   k  4    k  3      V   k  3   n      E  n
      k  3     2    E  n  k  4      E  n  k  5        &#x2212;  V  n n       V
      n  k  5      V   k  5    k  4      V   k  4    k  2      V   k  2   n
      E  n  k  2      E  n  k  4     2    E  n  k  5        &#x2212;  V  n n
      V  n  k  5      V   k  5    k  3      V   k  3    k  2      V   k  2   n
      E  n  k  2      E  n  k  3      E  n  k  5     2      +  V  n n       |
      V  n  k  5       |   2     E  n  k  5     2         |   V  n  k  3
      |   2     E  n  k  3     2     + 2  V  n n       |   V  n  k  5       |
      2     E  n  k  5     3         |   V  n  k  2       |   2     E  n  k  2
      +  V  n n   2       V  n  k  5      V   k  5    k  4      V   k  4   n
      E  n  k  4     3    E  n  k  5        +  V  n n   2       V  n  k  5
      V   k  5    k  3      V   k  3   n      E  n  k  3     2    E  n  k  5
      2      +  V  n n   2       V  n  k  5      V   k  5    k  2      V   k  2
      n      E  n  k  2      E  n  k  5     3      &#x2212;  V  n n   3       |
      V  n  k  5       |   2     E  n  k  5     4           =     V  n  k  5
      V   k  5    k  4      V   k  4    k  3      V   k  3    k  2      V   k
      2   n      E  n  k  2      E  n  k  3      E  n  k  4      E  n  k  5
      &#x2212; 2  E  n   ( 2 )       V  n  k  5      V   k  5    k  4      V
      k  4   n      E  n  k  4     2    E  n  k  5        &#x2212;     |   V  n
      k  5       |   2     E  n  k  5     2         V  n  k  3      V   k  3
      k  2      V   k  2   n      E  n  k  2      E  n  k  3
      &#x2212; 2  V  n n    (      V  n  k  5      V   k  5    k  4      V   k
      4    k  3      V   k  3   n      E  n  k  3     2    E  n  k  4      E  n
      k  5        &#x2212;     V  n  k  5      V   k  5    k  4      V   k  4
      k  2      V   k  2   n      E  n  k  2      E  n  k  4     2    E  n  k
      5        +     |   V  n  k  5       |   2     E  n  k  5     2         |
      V  n  k  3       |   2     E  n  k  3     2     + 2  E  n   ( 2 )       |
      V  n  k  5       |   2     E  n  k  5     3      )         +  V  n n   2
      (  2     V  n  k  5      V   k  5    k  4      V   k  4   n      E  n  k
      4     3    E  n  k  5        +     V  n  k  5      V   k  5    k  3
      V   k  3   n      E  n  k  3     2    E  n  k  5     2       )  &#x2212;
      V  n n   3       |   V  n  k  5       |   2     E  n  k  5     4
      {\displaystyle {\begin{aligned}E_{n}^{(1)}&=V_{nn}\\E_{n}^{(2)}&={\frac
      {|V_{nk_{2}}|^{2}}{E_{nk_{2}}}}\\E_{n}^{(3)}&={\frac {V_{nk_{3}}V_{k_
      {3}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{3}}}}-V_{nn}{\frac {|V_{nk_{3}}|^
      {2}}{E_{nk_{3}}^{2}}}\\E_{n}^{(4)}&={\frac {V_{nk_{4}}V_{k_{4}k_{3}}V_{k_
      {3}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{3}}E_{nk_{4}}}}-{\frac {|V_{nk_
      {4}}|^{2}}{E_{nk_{4}}^{2}}}{\frac {|V_{nk_{2}}|^{2}}{E_{nk_{2}}}}-V_{nn}
      {\frac {V_{nk_{4}}V_{k_{4}k_{3}}V_{k_{3}n}}{E_{nk_{3}}^{2}E_{nk_{4}}}}-V_
      {nn}{\frac {V_{nk_{4}}V_{k_{4}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{4}}^
      {2}}}+V_{nn}^{2}{\frac {|V_{nk_{4}}|^{2}}{E_{nk_{4}}^{3}}}\\&={\frac {V_
      {nk_{4}}V_{k_{4}k_{3}}V_{k_{3}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{3}}E_
      {nk_{4}}}}-E_{n}^{(2)}{\frac {|V_{nk_{4}}|^{2}}{E_{nk_{4}}^{2}}}-2V_{nn}
      {\frac {V_{nk_{4}}V_{k_{4}k_{3}}V_{k_{3}n}}{E_{nk_{3}}^{2}E_{nk_{4}}}}+V_
      {nn}^{2}{\frac {|V_{nk_{4}}|^{2}}{E_{nk_{4}}^{3}}}\\E_{n}^{(5)}&={\frac
      {V_{nk_{5}}V_{k_{5}k_{4}}V_{k_{4}k_{3}}V_{k_{3}k_{2}}V_{k_{2}n}}{E_{nk_
      {2}}E_{nk_{3}}E_{nk_{4}}E_{nk_{5}}}}-{\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_
      {k_{4}n}}{E_{nk_{4}}^{2}E_{nk_{5}}}}{\frac {|V_{nk_{2}}|^{2}}{E_{nk_
      {2}}}}-{\frac {V_{nk_{5}}V_{k_{5}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{5}}^
      {2}}}{\frac {|V_{nk_{2}}|^{2}}{E_{nk_{2}}}}-{\frac {|V_{nk_{5}}|^{2}}{E_
      {nk_{5}}^{2}}}{\frac {V_{nk_{3}}V_{k_{3}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_
      {nk_{3}}}}\\&\quad -V_{nn}{\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_{k_{4}k_
      {3}}V_{k_{3}n}}{E_{nk_{3}}^{2}E_{nk_{4}}E_{nk_{5}}}}-V_{nn}{\frac {V_{nk_
      {5}}V_{k_{5}k_{4}}V_{k_{4}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{4}}^{2}E_
      {nk_{5}}}}-V_{nn}{\frac {V_{nk_{5}}V_{k_{5}k_{3}}V_{k_{3}k_{2}}V_{k_
      {2}n}}{E_{nk_{2}}E_{nk_{3}}E_{nk_{5}}^{2}}}+V_{nn}{\frac {|V_{nk_{5}}|^
      {2}}{E_{nk_{5}}^{2}}}{\frac {|V_{nk_{3}}|^{2}}{E_{nk_{3}}^{2}}}+2V_{nn}
      {\frac {|V_{nk_{5}}|^{2}}{E_{nk_{5}}^{3}}}{\frac {|V_{nk_{2}}|^{2}}{E_
      {nk_{2}}}}\\&\quad +V_{nn}^{2}{\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_{k_{4}n}}
      {E_{nk_{4}}^{3}E_{nk_{5}}}}+V_{nn}^{2}{\frac {V_{nk_{5}}V_{k_{5}k_{3}}V_
      {k_{3}n}}{E_{nk_{3}}^{2}E_{nk_{5}}^{2}}}+V_{nn}^{2}{\frac {V_{nk_{5}}V_
      {k_{5}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{5}}^{3}}}-V_{nn}^{3}{\frac {|V_
      {nk_{5}}|^{2}}{E_{nk_{5}}^{4}}}\\&={\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_{k_
      {4}k_{3}}V_{k_{3}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{3}}E_{nk_{4}}E_{nk_
      {5}}}}-2E_{n}^{(2)}{\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_{k_{4}n}}{E_{nk_
      {4}}^{2}E_{nk_{5}}}}-{\frac {|V_{nk_{5}}|^{2}}{E_{nk_{5}}^{2}}}{\frac {V_
      {nk_{3}}V_{k_{3}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{3}}}}\\&\quad -2V_
      {nn}\left({\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_{k_{4}k_{3}}V_{k_{3}n}}{E_
      {nk_{3}}^{2}E_{nk_{4}}E_{nk_{5}}}}-{\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_{k_
      {4}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{4}}^{2}E_{nk_{5}}}}+{\frac {|V_{nk_
      {5}}|^{2}}{E_{nk_{5}}^{2}}}{\frac {|V_{nk_{3}}|^{2}}{E_{nk_{3}}^{2}}}+2E_
      {n}^{(2)}{\frac {|V_{nk_{5}}|^{2}}{E_{nk_{5}}^{3}}}\right)\\&\quad +V_
      {nn}^{2}\left(2{\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_{k_{4}n}}{E_{nk_{4}}^
      {3}E_{nk_{5}}}}+{\frac {V_{nk_{5}}V_{k_{5}k_{3}}V_{k_{3}n}}{E_{nk_{3}}^
      {2}E_{nk_{5}}^{2}}}\right)-V_{nn}^{3}{\frac {|V_{nk_{5}}|^{2}}{E_{nk_
      {5}}^{4}}}\end{aligned}}}  [{\begin{aligned}E_{n}^{(1)}&=V_{nn}\\E_{n}^{
      (2)}&={\frac {|V_{nk_{2}}|^{2}}{E_{nk_{2}}}}\\E_{n}^{(3)}&={\frac {V_{nk_
      {3}}V_{k_{3}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{3}}}}-V_{nn}{\frac {|V_
      {nk_{3}}|^{2}}{E_{nk_{3}}^{2}}}\\E_{n}^{(4)}&={\frac {V_{nk_{4}}V_{k_
      {4}k_{3}}V_{k_{3}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{3}}E_{nk_{4}}}}-
      {\frac {|V_{nk_{4}}|^{2}}{E_{nk_{4}}^{2}}}{\frac {|V_{nk_{2}}|^{2}}{E_
      {nk_{2}}}}-V_{nn}{\frac {V_{nk_{4}}V_{k_{4}k_{3}}V_{k_{3}n}}{E_{nk_{3}}^
      {2}E_{nk_{4}}}}-V_{nn}{\frac {V_{nk_{4}}V_{k_{4}k_{2}}V_{k_{2}n}}{E_{nk_
      {2}}E_{nk_{4}}^{2}}}+V_{nn}^{2}{\frac {|V_{nk_{4}}|^{2}}{E_{nk_{4}}^
      {3}}}\\&={\frac {V_{nk_{4}}V_{k_{4}k_{3}}V_{k_{3}k_{2}}V_{k_{2}n}}{E_{nk_
      {2}}E_{nk_{3}}E_{nk_{4}}}}-E_{n}^{(2)}{\frac {|V_{nk_{4}}|^{2}}{E_{nk_
      {4}}^{2}}}-2V_{nn}{\frac {V_{nk_{4}}V_{k_{4}k_{3}}V_{k_{3}n}}{E_{nk_{3}}^
      {2}E_{nk_{4}}}}+V_{nn}^{2}{\frac {|V_{nk_{4}}|^{2}}{E_{nk_{4}}^{3}}}\\E_
      {n}^{(5)}&={\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_{k_{4}k_{3}}V_{k_{3}k_{2}}V_
      {k_{2}n}}{E_{nk_{2}}E_{nk_{3}}E_{nk_{4}}E_{nk_{5}}}}-{\frac {V_{nk_{5}}V_
      {k_{5}k_{4}}V_{k_{4}n}}{E_{nk_{4}}^{2}E_{nk_{5}}}}{\frac {|V_{nk_{2}}|^
      {2}}{E_{nk_{2}}}}-{\frac {V_{nk_{5}}V_{k_{5}k_{2}}V_{k_{2}n}}{E_{nk_
      {2}}E_{nk_{5}}^{2}}}{\frac {|V_{nk_{2}}|^{2}}{E_{nk_{2}}}}-{\frac {|V_
      {nk_{5}}|^{2}}{E_{nk_{5}}^{2}}}{\frac {V_{nk_{3}}V_{k_{3}k_{2}}V_{k_
      {2}n}}{E_{nk_{2}}E_{nk_{3}}}}\\&\quad -V_{nn}{\frac {V_{nk_{5}}V_{k_{5}k_
      {4}}V_{k_{4}k_{3}}V_{k_{3}n}}{E_{nk_{3}}^{2}E_{nk_{4}}E_{nk_{5}}}}-V_{nn}
      {\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_{k_{4}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_
      {nk_{4}}^{2}E_{nk_{5}}}}-V_{nn}{\frac {V_{nk_{5}}V_{k_{5}k_{3}}V_{k_{3}k_
      {2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{3}}E_{nk_{5}}^{2}}}+V_{nn}{\frac {|V_
      {nk_{5}}|^{2}}{E_{nk_{5}}^{2}}}{\frac {|V_{nk_{3}}|^{2}}{E_{nk_{3}}^
      {2}}}+2V_{nn}{\frac {|V_{nk_{5}}|^{2}}{E_{nk_{5}}^{3}}}{\frac {|V_{nk_
      {2}}|^{2}}{E_{nk_{2}}}}\\&\quad +V_{nn}^{2}{\frac {V_{nk_{5}}V_{k_{5}k_
      {4}}V_{k_{4}n}}{E_{nk_{4}}^{3}E_{nk_{5}}}}+V_{nn}^{2}{\frac {V_{nk_{5}}V_
      {k_{5}k_{3}}V_{k_{3}n}}{E_{nk_{3}}^{2}E_{nk_{5}}^{2}}}+V_{nn}^{2}{\frac
      {V_{nk_{5}}V_{k_{5}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{5}}^{3}}}-V_{nn}^
      {3}{\frac {|V_{nk_{5}}|^{2}}{E_{nk_{5}}^{4}}}\\&={\frac {V_{nk_{5}}V_{k_
      {5}k_{4}}V_{k_{4}k_{3}}V_{k_{3}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{3}}E_
      {nk_{4}}E_{nk_{5}}}}-2E_{n}^{(2)}{\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_{k_
      {4}n}}{E_{nk_{4}}^{2}E_{nk_{5}}}}-{\frac {|V_{nk_{5}}|^{2}}{E_{nk_{5}}^
      {2}}}{\frac {V_{nk_{3}}V_{k_{3}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_
      {3}}}}\\&\quad -2V_{nn}\left({\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_{k_{4}k_
      {3}}V_{k_{3}n}}{E_{nk_{3}}^{2}E_{nk_{4}}E_{nk_{5}}}}-{\frac {V_{nk_{5}}V_
      {k_{5}k_{4}}V_{k_{4}k_{2}}V_{k_{2}n}}{E_{nk_{2}}E_{nk_{4}}^{2}E_{nk_
      {5}}}}+{\frac {|V_{nk_{5}}|^{2}}{E_{nk_{5}}^{2}}}{\frac {|V_{nk_{3}}|^
      {2}}{E_{nk_{3}}^{2}}}+2E_{n}^{(2)}{\frac {|V_{nk_{5}}|^{2}}{E_{nk_{5}}^
      {3}}}\right)\\&\quad +V_{nn}^{2}\left(2{\frac {V_{nk_{5}}V_{k_{5}k_{4}}V_
      {k_{4}n}}{E_{nk_{4}}^{3}E_{nk_{5}}}}+{\frac {V_{nk_{5}}V_{k_{5}k_{3}}V_
      {k_{3}n}}{E_{nk_{3}}^{2}E_{nk_{5}}^{2}}}\right)-V_{nn}^{3}{\frac {|V_{nk_
      {5}}|^{2}}{E_{nk_{5}}^{4}}}\end{aligned}}]
and the states to fourth order can be written
              |   n  ( 1 )   &#x27E9;    =    V   k  1   n    E  n  k  1
      |   k  1   ( 0 )   &#x27E9;      |   n  ( 2 )   &#x27E9;    =  (      V
      k  1    k  2      V   k  2   n      E  n  k  1      E  n  k  2
      &#x2212;     V  n n    V   k  1   n     E  n  k  1     2      )   |   k
      1   ( 0 )   &#x27E9; &#x2212;   1 2       V  n  k  1      V   k  1   n
      E   k  1   n   2      |   n  ( 0 )   &#x27E9;      |   n  ( 3 )
      &#x27E9;    =   [   &#x2212;     V   k  1    k  2      V   k  2    k  3
      V   k  3   n      E   k  1   n    E  n  k  2      E  n  k  3        +
      V  n n    V   k  1    k  2      V   k  2   n      E   k  1   n    E  n  k
      2         (    1  E  n  k  1       +   1  E  n  k  2        )  &#x2212;
      |   V  n n     |   2    V   k  1   n     E   k  1   n   3     +     |   V
      n  k  2       |   2    V   k  1   n      E   k  1   n    E  n  k  2
      (    1  E  n  k  1       +   1  2  E  n  k  2         )    ]    |   k  1
      ( 0 )   &#x27E9;        +   [   &#x2212;     V  n  k  2      V   k  2
      k  1      V   k  1   n   +  V   k  2   n    V   k  1    k  2      V  n  k
      1       2  E  n  k  2     2    E  n  k  1        +     |   V  n  k  1
      |   2    V  n n     E  n  k  1     3       ]    |   n  ( 0 )   &#x27E9;
      |   n  ( 4 )   &#x27E9;    =   [       V   k  1    k  2      V   k  2
      k  3      V   k  3    k  4      V   k  4    k  2     +  V   k  3    k  2
      V   k  1    k  2      V   k  4    k  3      V   k  2    k  4       2  E
      k  1   n    E   k  2    k  3     2    E   k  2    k  4        &#x2212;
      V   k  2    k  3      V   k  3    k  4      V   k  4   n    V   k  1    k
      2        E   k  1   n    E   k  2   n    E  n  k  3      E  n  k  4
      +    V   k  1    k  2      E   k  1   n      (      |   V   k  2    k  3
      |   2    V   k  2    k  2       E   k  2    k  3     3     &#x2212;     |
      V  n  k  3       |   2    V   k  2   n      E   k  3   n   2    E   k  2
      n       )         +     V  n n    V   k  1    k  2      V   k  3   n    V
      k  2    k  3        E   k  1   n    E  n  k  3      E   k  2   n
      (    1  E  n  k  3       +   1  E   k  2   n     +   1  E   k  1   n
      )  +     |   V   k  2   n     |   2    V   k  1    k  3        E  n  k  2
      E   k  1   n       (     V   k  3   n     E  n  k  1      E  n  k  3
      &#x2212;    V   k  3    k  1      E   k  3    k  1     2      )  &#x2212;
      V  n n    (   V   k  3    k  2      V   k  1    k  3      V   k  2    k
      1     +  V   k  3    k  1      V   k  2    k  3      V   k  1    k  2
      )    2  E   k  1   n    E   k  1    k  3     2    E   k  1    k  2
      +     |   V  n n     |   2     E   k  1   n      (      V   k  1   n    V
      n n     E   k  1   n   3     +     V   k  1    k  2      V   k  2   n
      E   k  2   n   3      )  &#x2212;     |   V   k  1    k  2       |   2
      V  n n    V   k  1   n      E   k  1   n    E   k  1    k  2     3
      ]    |   k  1   ( 0 )   &#x27E9; +   1 2    [      V  n  k  1      V   k
      1    k  2        E  n  k  1      E   k  2   n   2       (      V   k  2
      n    V  n n     E   k  2   n     &#x2212;     V   k  2    k  3      V   k
      3   n     E  n  k  3        )              &#x2212;     V   k  1   n    V
      k  2    k  1        E   k  1   n   2    E  n  k  2         (      V   k
      3    k  2      V  n  k  3       E  n  k  3       +     V  n n    V  n  k
      2       E  n  k  2        )  +     |   V  n  k  1       |   2     E   k
      1   n   2      (     3  |   V  n  k  2       |   2     4  E   k  2   n
      2      &#x2212;    2  |   V  n n     |   2     E   k  1   n   2      )
      &#x2212;     V   k  2    k  3      V   k  3    k  1      |   V  n  k  1
      |   2      E  n  k  3     2    E  n  k  1      E  n  k  2         ]   |
      n  ( 0 )   &#x27E9;       {\displaystyle {\begin{aligned}|n^{(1)}\rangle
      &={\frac {V_{k_{1}n}}{E_{nk_{1}}}}|k_{1}^{(0)}\rangle \\|n^{(2)}\rangle
      &=\left({\frac {V_{k_{1}k_{2}}V_{k_{2}n}}{E_{nk_{1}}E_{nk_{2}}}}-{\frac
      {V_{nn}V_{k_{1}n}}{E_{nk_{1}}^{2}}}\right)|k_{1}^{(0)}\rangle -{\frac {1}
      {2}}{\frac {V_{nk_{1}}V_{k_{1}n}}{E_{k_{1}n}^{2}}}|n^{(0)}\rangle \\|n^{
      (3)}\rangle &={\Bigg [}-{\frac {V_{k_{1}k_{2}}V_{k_{2}k_{3}}V_{k_{3}n}}
      {E_{k_{1}n}E_{nk_{2}}E_{nk_{3}}}}+{\frac {V_{nn}V_{k_{1}k_{2}}V_{k_{2}n}}
      {E_{k_{1}n}E_{nk_{2}}}}\left({\frac {1}{E_{nk_{1}}}}+{\frac {1}{E_{nk_
      {2}}}}\right)-{\frac {|V_{nn}|^{2}V_{k_{1}n}}{E_{k_{1}n}^{3}}}+{\frac
      {|V_{nk_{2}}|^{2}V_{k_{1}n}}{E_{k_{1}n}E_{nk_{2}}}}\left({\frac {1}{E_
      {nk_{1}}}}+{\frac {1}{2E_{nk_{2}}}}\right){\Bigg ]}|k_{1}^{(0)}\rangle
      \\&\quad +{\Bigg [}-{\frac {V_{nk_{2}}V_{k_{2}k_{1}}V_{k_{1}n}+V_{k_
      {2}n}V_{k_{1}k_{2}}V_{nk_{1}}}{2E_{nk_{2}}^{2}E_{nk_{1}}}}+{\frac {|V_
      {nk_{1}}|^{2}V_{nn}}{E_{nk_{1}}^{3}}}{\Bigg ]}|n^{(0)}\rangle \\|n^{
      (4)}\rangle &={\Bigg [}{\frac {V_{k_{1}k_{2}}V_{k_{2}k_{3}}V_{k_{3}k_
      {4}}V_{k_{4}k_{2}}+V_{k_{3}k_{2}}V_{k_{1}k_{2}}V_{k_{4}k_{3}}V_{k_{2}k_
      {4}}}{2E_{k_{1}n}E_{k_{2}k_{3}}^{2}E_{k_{2}k_{4}}}}-{\frac {V_{k_{2}k_
      {3}}V_{k_{3}k_{4}}V_{k_{4}n}V_{k_{1}k_{2}}}{E_{k_{1}n}E_{k_{2}n}E_{nk_
      {3}}E_{nk_{4}}}}+{\frac {V_{k_{1}k_{2}}}{E_{k_{1}n}}}\left({\frac {|V_{k_
      {2}k_{3}}|^{2}V_{k_{2}k_{2}}}{E_{k_{2}k_{3}}^{3}}}-{\frac {|V_{nk_{3}}|^
      {2}V_{k_{2}n}}{E_{k_{3}n}^{2}E_{k_{2}n}}}\right)\\&\quad +{\frac {V_
      {nn}V_{k_{1}k_{2}}V_{k_{3}n}V_{k_{2}k_{3}}}{E_{k_{1}n}E_{nk_{3}}E_{k_
      {2}n}}}\left({\frac {1}{E_{nk_{3}}}}+{\frac {1}{E_{k_{2}n}}}+{\frac {1}
      {E_{k_{1}n}}}\right)+{\frac {|V_{k_{2}n}|^{2}V_{k_{1}k_{3}}}{E_{nk_{2}}E_
      {k_{1}n}}}\left({\frac {V_{k_{3}n}}{E_{nk_{1}}E_{nk_{3}}}}-{\frac {V_{k_
      {3}k_{1}}}{E_{k_{3}k_{1}}^{2}}}\right)-{\frac {V_{nn}\left(V_{k_{3}k_
      {2}}V_{k_{1}k_{3}}V_{k_{2}k_{1}}+V_{k_{3}k_{1}}V_{k_{2}k_{3}}V_{k_{1}k_
      {2}}\right)}{2E_{k_{1}n}E_{k_{1}k_{3}}^{2}E_{k_{1}k_{2}}}}\\&\quad +
      {\frac {|V_{nn}|^{2}}{E_{k_{1}n}}}\left({\frac {V_{k_{1}n}V_{nn}}{E_{k_
      {1}n}^{3}}}+{\frac {V_{k_{1}k_{2}}V_{k_{2}n}}{E_{k_{2}n}^{3}}}\right)-
      {\frac {|V_{k_{1}k_{2}}|^{2}V_{nn}V_{k_{1}n}}{E_{k_{1}n}E_{k_{1}k_{2}}^
      {3}}}{\Bigg ]}|k_{1}^{(0)}\rangle +{\frac {1}{2}}\left[{\frac {V_{nk_
      {1}}V_{k_{1}k_{2}}}{E_{nk_{1}}E_{k_{2}n}^{2}}}\left({\frac {V_{k_{2}n}V_
      {nn}}{E_{k_{2}n}}}-{\frac {V_{k_{2}k_{3}}V_{k_{3}n}}{E_{nk_
      {3}}}}\right)\right.\\&\quad \left.-{\frac {V_{k_{1}n}V_{k_{2}k_{1}}}{E_
      {k_{1}n}^{2}E_{nk_{2}}}}\left({\frac {V_{k_{3}k_{2}}V_{nk_{3}}}{E_{nk_
      {3}}}}+{\frac {V_{nn}V_{nk_{2}}}{E_{nk_{2}}}}\right)+{\frac {|V_{nk_
      {1}}|^{2}}{E_{k_{1}n}^{2}}}\left({\frac {3|V_{nk_{2}}|^{2}}{4E_{k_{2}n}^
      {2}}}-{\frac {2|V_{nn}|^{2}}{E_{k_{1}n}^{2}}}\right)-{\frac {V_{k_{2}k_
      {3}}V_{k_{3}k_{1}}|V_{nk_{1}}|^{2}}{E_{nk_{3}}^{2}E_{nk_{1}}E_{nk_
      {2}}}}\right]|n^{(0)}\rangle \end{aligned}}}  [{\displaystyle {\begin
      {aligned}|n^{(1)}\rangle &={\frac {V_{k_{1}n}}{E_{nk_{1}}}}|k_{1}^{
      (0)}\rangle \\|n^{(2)}\rangle &=\left({\frac {V_{k_{1}k_{2}}V_{k_{2}n}}
      {E_{nk_{1}}E_{nk_{2}}}}-{\frac {V_{nn}V_{k_{1}n}}{E_{nk_{1}}^
      {2}}}\right)|k_{1}^{(0)}\rangle -{\frac {1}{2}}{\frac {V_{nk_{1}}V_{k_
      {1}n}}{E_{k_{1}n}^{2}}}|n^{(0)}\rangle \\|n^{(3)}\rangle &={\Bigg [}-
      {\frac {V_{k_{1}k_{2}}V_{k_{2}k_{3}}V_{k_{3}n}}{E_{k_{1}n}E_{nk_{2}}E_
      {nk_{3}}}}+{\frac {V_{nn}V_{k_{1}k_{2}}V_{k_{2}n}}{E_{k_{1}n}E_{nk_
      {2}}}}\left({\frac {1}{E_{nk_{1}}}}+{\frac {1}{E_{nk_{2}}}}\right)-{\frac
      {|V_{nn}|^{2}V_{k_{1}n}}{E_{k_{1}n}^{3}}}+{\frac {|V_{nk_{2}}|^{2}V_{k_
      {1}n}}{E_{k_{1}n}E_{nk_{2}}}}\left({\frac {1}{E_{nk_{1}}}}+{\frac {1}{2E_
      {nk_{2}}}}\right){\Bigg ]}|k_{1}^{(0)}\rangle \\&\quad +{\Bigg [}-{\frac
      {V_{nk_{2}}V_{k_{2}k_{1}}V_{k_{1}n}+V_{k_{2}n}V_{k_{1}k_{2}}V_{nk_{1}}}
      {2E_{nk_{2}}^{2}E_{nk_{1}}}}+{\frac {|V_{nk_{1}}|^{2}V_{nn}}{E_{nk_{1}}^
      {3}}}{\Bigg ]}|n^{(0)}\rangle \\|n^{(4)}\rangle &={\Bigg [}{\frac {V_{k_
      {1}k_{2}}V_{k_{2}k_{3}}V_{k_{3}k_{4}}V_{k_{4}k_{2}}+V_{k_{3}k_{2}}V_{k_
      {1}k_{2}}V_{k_{4}k_{3}}V_{k_{2}k_{4}}}{2E_{k_{1}n}E_{k_{2}k_{3}}^{2}E_{k_
      {2}k_{4}}}}-{\frac {V_{k_{2}k_{3}}V_{k_{3}k_{4}}V_{k_{4}n}V_{k_{1}k_{2}}}
      {E_{k_{1}n}E_{k_{2}n}E_{nk_{3}}E_{nk_{4}}}}+{\frac {V_{k_{1}k_{2}}}{E_{k_
      {1}n}}}\left({\frac {|V_{k_{2}k_{3}}|^{2}V_{k_{2}k_{2}}}{E_{k_{2}k_{3}}^
      {3}}}-{\frac {|V_{nk_{3}}|^{2}V_{k_{2}n}}{E_{k_{3}n}^{2}E_{k_
      {2}n}}}\right)\\&\quad +{\frac {V_{nn}V_{k_{1}k_{2}}V_{k_{3}n}V_{k_{2}k_
      {3}}}{E_{k_{1}n}E_{nk_{3}}E_{k_{2}n}}}\left({\frac {1}{E_{nk_{3}}}}+
      {\frac {1}{E_{k_{2}n}}}+{\frac {1}{E_{k_{1}n}}}\right)+{\frac {|V_{k_
      {2}n}|^{2}V_{k_{1}k_{3}}}{E_{nk_{2}}E_{k_{1}n}}}\left({\frac {V_{k_{3}n}}
      {E_{nk_{1}}E_{nk_{3}}}}-{\frac {V_{k_{3}k_{1}}}{E_{k_{3}k_{1}}^
      {2}}}\right)-{\frac {V_{nn}\left(V_{k_{3}k_{2}}V_{k_{1}k_{3}}V_{k_{2}k_
      {1}}+V_{k_{3}k_{1}}V_{k_{2}k_{3}}V_{k_{1}k_{2}}\right)}{2E_{k_{1}n}E_{k_
      {1}k_{3}}^{2}E_{k_{1}k_{2}}}}\\&\quad +{\frac {|V_{nn}|^{2}}{E_{k_
      {1}n}}}\left({\frac {V_{k_{1}n}V_{nn}}{E_{k_{1}n}^{3}}}+{\frac {V_{k_
      {1}k_{2}}V_{k_{2}n}}{E_{k_{2}n}^{3}}}\right)-{\frac {|V_{k_{1}k_{2}}|^
      {2}V_{nn}V_{k_{1}n}}{E_{k_{1}n}E_{k_{1}k_{2}}^{3}}}{\Bigg ]}|k_{1}^{
      (0)}\rangle +{\frac {1}{2}}\left[{\frac {V_{nk_{1}}V_{k_{1}k_{2}}}{E_{nk_
      {1}}E_{k_{2}n}^{2}}}\left({\frac {V_{k_{2}n}V_{nn}}{E_{k_{2}n}}}-{\frac
      {V_{k_{2}k_{3}}V_{k_{3}n}}{E_{nk_{3}}}}\right)\right.\\&\quad \left.-
      {\frac {V_{k_{1}n}V_{k_{2}k_{1}}}{E_{k_{1}n}^{2}E_{nk_{2}}}}\left({\frac
      {V_{k_{3}k_{2}}V_{nk_{3}}}{E_{nk_{3}}}}+{\frac {V_{nn}V_{nk_{2}}}{E_{nk_
      {2}}}}\right)+{\frac {|V_{nk_{1}}|^{2}}{E_{k_{1}n}^{2}}}\left({\frac
      {3|V_{nk_{2}}|^{2}}{4E_{k_{2}n}^{2}}}-{\frac {2|V_{nn}|^{2}}{E_{k_{1}n}^
      {2}}}\right)-{\frac {V_{k_{2}k_{3}}V_{k_{3}k_{1}}|V_{nk_{1}}|^{2}}{E_{nk_
      {3}}^{2}E_{nk_{1}}E_{nk_{2}}}}\right]|n^{(0)}\rangle \end{aligned}}}]
All terms involved kj should be summed over kj such that the denominator does
not vanish.
**** Effects of degeneracy[edit] ****
Suppose that two or more energy eigenstates are degenerate. The first-order
energy shift is not well defined, since there is no unique way to choose a
basis of eigenstates for the unperturbed system. The various eigenstates for a
given energy will perturb with different energies, or may well possess no
continuous family of perturbations at all.
This is manifested in the calculation of the perturbed eigenstate via the fact
that the operator
          E  n   ( 0 )   &#x2212;  H  0     {\displaystyle E_{n}^{(0)}-H_{0}}
      [E_{n}^{(0)}-H_{0}]
does not have a well-defined inverse.
Let D denote the subspace spanned by these degenerate eigenstates. No matter
how small the perturbation is, in the degenerate subspace D the energy
differences between the eigenstates of H are non-zero, so complete mixing of at
least some of these states is assured. Typically, the eigenvalues will split,
and the eigenspaces will become simple (one-dimensional), or at least of
smaller dimension than D.
The successful perturbations will not be "small" relative to a poorly chosen
basis of D. Instead, we consider the perturbation "small" if the new eigenstate
is close to the subspace D. The new Hamiltonian must be diagonalized in D, or a
slight variation of D, so to speak. These perturbed eigenstates in D are now
the basis for the perturbation expansion,
          |  n &#x27E9; =  &#x2211;  k &#x2208; D    &#x03B1;  n k    |   k
      ( 0 )   &#x27E9; + &#x03BB;  |   n  ( 1 )   &#x27E9; .   {\displaystyle
      |n\rangle =\sum _{k\in D}\alpha _{nk}|k^{(0)}\rangle +\lambda |n^{
      (1)}\rangle .}  [{\displaystyle |n\rangle =\sum _{k\in D}\alpha _{nk}|k^{
      (0)}\rangle +\lambda |n^{(1)}\rangle .}]
For the first-order perturbation, we need solve the perturbed Hamiltonian
restricted to the degenerate subspace D,
         V  |   k  ( 0 )   &#x27E9; =  &#x03F5;  k    |   k  ( 0 )   &#x27E9; +
      small   &#x2200;  |   k  ( 0 )   &#x27E9; &#x2208; D ,   {\displaystyle
      V|k^{(0)}\rangle =\epsilon _{k}|k^{(0)}\rangle +{\text{small}}\qquad
      \forall |k^{(0)}\rangle \in D,}  [{\displaystyle V|k^{(0)}\rangle
      =\epsilon _{k}|k^{(0)}\rangle +{\text{small}}\qquad \forall |k^{
      (0)}\rangle \in D,}]
simultaneously for all the degenerate eigenstates, where      &#x03F5;  k
{\displaystyle \epsilon _{k}}  [\epsilon _{k}] are first-order corrections to
the degenerate energy levels, and "small" is a vector of     O ( &#x03BB; )
{\displaystyle O(\lambda )}  [{\displaystyle O(\lambda )}] orthogonal to D.
This amounts to diagonalizing the matrix
         &#x27E8;  k  ( 0 )    |  V  |   l  ( 0 )   &#x27E9; =  V  k l
      &#x2200;   |   k  ( 0 )   &#x27E9; ,  |   l  ( 0 )   &#x27E9; &#x2208; D
      .   {\displaystyle \langle k^{(0)}|V|l^{(0)}\rangle =V_{kl}\qquad \forall
      \;|k^{(0)}\rangle ,|l^{(0)}\rangle \in D.}  [\langle k^{(0)}|V|l^{
      (0)}\rangle =V_{kl}\qquad \forall \;|k^{(0)}\rangle ,|l^{(0)}\rangle \in
      D.]
This procedure is approximate, since we neglected states outside the D subspace
("small"). The splitting of degenerate energies      &#x03F5;  k
{\displaystyle \epsilon _{k}}  [\epsilon _{k}] is generally observed. Although
the splitting may be small,     O ( &#x03BB; )   {\displaystyle O(\lambda )}  [
{\displaystyle O(\lambda )}], compared to the range of energies found in the
system, it is crucial in understanding certain details, such as spectral lines
in Electron_Spin_Resonance experiments.
Higher-order corrections due to other eigenstates outside D can be found in the
same way as for the non-degenerate case,
          (   E  n   ( 0 )   &#x2212;  H  0    )   |   n  ( 1 )   &#x27E9; =
      &#x2211;  k &#x2209; D    (  &#x27E8;  k  ( 0 )    |  V  |   n  ( 0 )
      &#x27E9;  )   |   k  ( 0 )   &#x27E9; .   {\displaystyle \left(E_{n}^{
      (0)}-H_{0}\right)|n^{(1)}\rangle =\sum _{k\not \in D}\left(\langle k^{
      (0)}|V|n^{(0)}\rangle \right)|k^{(0)}\rangle .}  [\left(E_{n}^{(0)}-H_
      {0}\right)|n^{(1)}\rangle =\sum _{k\not \in D}\left(\langle k^{(0)}|V|n^{
      (0)}\rangle \right)|k^{(0)}\rangle .]
The operator on the left-hand side is not singular when applied to eigenstates
outside D, so we can write
          |   n  ( 1 )   &#x27E9; =  &#x2211;  k &#x2209; D      &#x27E8;  k
      ( 0 )    |  V  |   n  ( 0 )   &#x27E9;    E  n   ( 0 )   &#x2212;  E  k
      ( 0 )       |   k  ( 0 )   &#x27E9; ,   {\displaystyle |n^{(1)}\rangle
      =\sum _{k\not \in D}{\frac {\langle k^{(0)}|V|n^{(0)}\rangle }{E_{n}^{
      (0)}-E_{k}^{(0)}}}|k^{(0)}\rangle ,}  [|n^{(1)}\rangle =\sum _{k\not \in
      D}{\frac {\langle k^{(0)}|V|n^{(0)}\rangle }{E_{n}^{(0)}-E_{k}^{(0)}}}|k^
      {(0)}\rangle ,]
but the effect on the degenerate states is of     O ( &#x03BB; )
{\displaystyle O(\lambda )}  [{\displaystyle O(\lambda )}].
Near-degenerate states should also be treated similarly, when the original
Hamiltonian splits aren't larger than the perturbation in the near-degenerate
subspace. An application is found in the nearly_free_electron_model, where
near-degeneracy, treated properly, gives rise to an energy gap even for small
perturbations. Other eigenstates will only shift the absolute energy of all
near-degenerate states simultaneously.
**** Generalization to multi-parameter case[edit] ****
The generalization of the time-independent perturbation theory to the case
where there are multiple small parameters      x  &#x03BC;   = (  x  1   ,  x
2   , &#x22EF; )   {\displaystyle x^{\mu }=(x^{1},x^{2},\cdots )}  [x^{\mu }=
(x^{1},x^{2},\cdots )] in place of Î» can be formulated more systematically
using the language of differential_geometry, which basically defines the
derivatives of the quantum states and calculates the perturbative corrections
by taking derivatives iteratively at the unperturbed point.
*** Hamiltonian and force operator[edit] ***
From the differential geometric point of view, a parameterized Hamiltonian is
considered as a function defined on the parameter manifold that maps each
particular set of parameters     (  x  1   ,  x  2   , &#x22EF; )
{\displaystyle (x^{1},x^{2},\cdots )}  [(x^{1},x^{2},\cdots )] to an Hermitian
operator H(x Î¼) that acts on the Hilbert space. The parameters here can be
external field, interaction strength, or driving parameters in the quantum
phase_transition. Let En(x Î¼) and      |  n (  x  &#x03BC;   ) &#x27E9;
{\displaystyle |n(x^{\mu })\rangle }  [|n(x^{\mu })\rangle ] be the n-th
eigenenergy and eigenstate of H(x Î¼) respectively. In the language of
differential geometry, the states      |  n (  x  &#x03BC;   ) &#x27E9;
{\displaystyle |n(x^{\mu })\rangle }  [|n(x^{\mu })\rangle ] form a vector
bundle over the parameter manifold, on which derivatives of these states can be
defined. The perturbation theory is to answer the following question: given
E  n   (  x  0   &#x03BC;   )   {\displaystyle E_{n}(x_{0}^{\mu })}  [E_{n}(x_
{0}^{\mu })] and      |  n (  x  0   &#x03BC;   ) &#x27E9;   {\displaystyle |n
(x_{0}^{\mu })\rangle }  [|n(x_{0}^{\mu })\rangle ] at an unperturbed reference
point      x  0   &#x03BC;     {\displaystyle x_{0}^{\mu }}  [x_{0}^{\mu }],
how to estimate the En(x Î¼) and      |  n (  x  &#x03BC;   ) &#x27E9;
{\displaystyle |n(x^{\mu })\rangle }  [|n(x^{\mu })\rangle ] at x Î¼ close to
that reference point.
Without loss of generality, the coordinate system can be shifted, such that the
reference point      x  0   &#x03BC;   = 0   {\displaystyle x_{0}^{\mu }=0}
[x_{0}^{\mu }=0] is set to be the origin. The following linearly parameterized
Hamiltonian is frequently used
         H (  x  &#x03BC;   ) = H ( 0 ) +  x  &#x03BC;    F  &#x03BC;   .
      {\displaystyle H(x^{\mu })=H(0)+x^{\mu }F_{\mu }.}  [H(x^{\mu })=H(0)+x^
      {\mu }F_{\mu }.]
If the parameters x Î¼ are considered as generalized coordinates, then FÎ¼
should be identified as the generalized force operators related to those
coordinates. Different indices Î¼ label the different forces along different
directions in the parameter manifold. For example, if x Î¼ denotes the external
magnetic field in the Î¼-direction, then FÎ¼ should be the magnetization in the
same direction.
*** Perturbation theory as power series expansion[edit] ***
The validity of the perturbation theory lies on the adiabatic assumption, which
assumes the eigenenergies and eigenstates of the Hamiltonian are smooth
functions of parameters such that their values in the vicinity region can be
calculated in power series (like Taylor_expansion) of the parameters:
              E  n   (  x  &#x03BC;   )    =  E  n   +  x  &#x03BC;    &#x2202;
      &#x03BC;    E  n   +   1  2 !     x  &#x03BC;    x  &#x03BD;    &#x2202;
      &#x03BC;    &#x2202;  &#x03BD;    E  n   + &#x22EF;      |  n (  x
      &#x03BC;   )  &#x27E9;     =  |  n &#x27E9; +  x  &#x03BC;    |
      &#x2202;  &#x03BC;   n &#x27E9; +   1  2 !     x  &#x03BC;    x  &#x03BD;
      |   &#x2202;  &#x03BC;    &#x2202;  &#x03BD;   n &#x27E9; + &#x22EF;
      {\displaystyle {\begin{aligned}E_{n}(x^{\mu })&=E_{n}+x^{\mu }\partial _
      {\mu }E_{n}+{\frac {1}{2!}}x^{\mu }x^{\nu }\partial _{\mu }\partial _{\nu
      }E_{n}+\cdots \\\left|n(x^{\mu })\right\rangle &=|n\rangle +x^{\mu
      }|\partial _{\mu }n\rangle +{\frac {1}{2!}}x^{\mu }x^{\nu }|\partial _
      {\mu }\partial _{\nu }n\rangle +\cdots \end{aligned}}}  [{\begin
      {aligned}E_{n}(x^{\mu })&=E_{n}+x^{\mu }\partial _{\mu }E_{n}+{\frac {1}
      {2!}}x^{\mu }x^{\nu }\partial _{\mu }\partial _{\nu }E_{n}+\cdots
      \\\left|n(x^{\mu })\right\rangle &=|n\rangle +x^{\mu }|\partial _{\mu
      }n\rangle +{\frac {1}{2!}}x^{\mu }x^{\nu }|\partial _{\mu }\partial _{\nu
      }n\rangle +\cdots \end{aligned}}]
Here âÎ¼ denotes the derivative with respect to x Î¼. When applying to the
state      |   &#x2202;  &#x03BC;   n &#x27E9;   {\displaystyle |\partial _{\mu
}n\rangle }  [|\partial _{\mu }n\rangle ], it should be understood as the
covariant_derivative if the vector bundle is equipped with non-vanishing
connection. All the terms on the right-hand-side of the series are evaluated at
x Î¼ = 0, e.g. En â¡ En(0) and      |  n &#x27E9; &#x2261;  |  n ( 0 )
&#x27E9;   {\displaystyle |n\rangle \equiv |n(0)\rangle }  [|n\rangle \equiv |n
(0)\rangle ]. This convention will be adopted throughout this subsection, that
all functions without the parameter dependence explicitly stated are assumed to
be evaluated at the origin. The power series may converge slowly or even not
converge when the energy levels are close to each other. The adiabatic
assumption breaks down when there is energy level degeneracy, and hence the
perturbation theory is not applicable in that case.
*** HellmannâFeynman theorems[edit] ***
The above power series expansion can be readily evaluated if there is a
systematic approach to calculate the derivates to any order. Using the chain
rule, the derivatives can be broken down to the single derivative on either the
energy or the state. The HellmannâFeynman_theorems are used to calculate
these single derivatives. The first HellmannâFeynman theorem gives the
derivative of the energy,
          &#x2202;  &#x03BC;    E  n   = &#x27E8; n  |   &#x2202;  &#x03BC;   H
      |  n &#x27E9;   {\displaystyle \partial _{\mu }E_{n}=\langle n|\partial _
      {\mu }H|n\rangle }  [\partial _{\mu }E_{n}=\langle n|\partial _{\mu
      }H|n\rangle ]
The second HellmannâFeynman theorem gives the derivative of the state
(resolved by the complete basis with m â  n),
         &#x27E8; m  |   &#x2202;  &#x03BC;   n &#x27E9; =    &#x27E8; m  |
      &#x2202;  &#x03BC;   H  |  n &#x27E9;    E  n   &#x2212;  E  m      ,
      &#x27E8;  &#x2202;  &#x03BC;   m  |  n &#x27E9; =    &#x27E8; m  |
      &#x2202;  &#x03BC;   H  |  n &#x27E9;    E  m   &#x2212;  E  n      .
      {\displaystyle \langle m|\partial _{\mu }n\rangle ={\frac {\langle
      m|\partial _{\mu }H|n\rangle }{E_{n}-E_{m}}},\qquad \langle \partial _
      {\mu }m|n\rangle ={\frac {\langle m|\partial _{\mu }H|n\rangle }{E_{m}-E_
      {n}}}.}  [\langle m|\partial _{\mu }n\rangle ={\frac {\langle m|\partial
      _{\mu }H|n\rangle }{E_{n}-E_{m}}},\qquad \langle \partial _{\mu
      }m|n\rangle ={\frac {\langle m|\partial _{\mu }H|n\rangle }{E_{m}-E_
      {n}}}.]
For the linearly parameterized Hamiltonian, âÎ¼H simply stands for the
generalized force operator FÎ¼.
The theorems can be simply derived by applying the differential operator âÎ¼
to both sides of the SchrÃ¶dinger_equation     H  |  n &#x27E9; =  E  n    |  n
&#x27E9; ,   {\displaystyle H|n\rangle =E_{n}|n\rangle ,}  [H|n\rangle =E_
{n}|n\rangle ,] which reads
          &#x2202;  &#x03BC;   H  |  n &#x27E9; + H  |   &#x2202;  &#x03BC;   n
      &#x27E9; =  &#x2202;  &#x03BC;    E  n    |  n &#x27E9; +  E  n    |
      &#x2202;  &#x03BC;   n &#x27E9; .   {\displaystyle \partial _{\mu
      }H|n\rangle +H|\partial _{\mu }n\rangle =\partial _{\mu }E_{n}|n\rangle
      +E_{n}|\partial _{\mu }n\rangle .}  [\partial _{\mu }H|n\rangle
      +H|\partial _{\mu }n\rangle =\partial _{\mu }E_{n}|n\rangle +E_
      {n}|\partial _{\mu }n\rangle .]
Then overlap with the state     &#x27E8; m  |    {\displaystyle \langle m|}
[\langle m|] from left and make use of the SchrÃ¶dinger equation     &#x27E8; m
|  H = &#x27E8; m  |   E  m     {\displaystyle \langle m|H=\langle m|E_{m}}
[\langle m|H=\langle m|E_{m}] again,
         &#x27E8; m  |   &#x2202;  &#x03BC;   H  |  n &#x27E9; +  E  m
      &#x27E8; m  |   &#x2202;  &#x03BC;   n &#x27E9; =  &#x2202;  &#x03BC;
      E  n   &#x27E8; m  |  n &#x27E9; +  E  n   &#x27E8; m  |   &#x2202;
      &#x03BC;   n &#x27E9; .   {\displaystyle \langle m|\partial _{\mu
      }H|n\rangle +E_{m}\langle m|\partial _{\mu }n\rangle =\partial _{\mu }E_
      {n}\langle m|n\rangle +E_{n}\langle m|\partial _{\mu }n\rangle .}
      [\langle m|\partial _{\mu }H|n\rangle +E_{m}\langle m|\partial _{\mu
      }n\rangle =\partial _{\mu }E_{n}\langle m|n\rangle +E_{n}\langle
      m|\partial _{\mu }n\rangle .]
Given that the eigenstates of the Hamiltonian always form an orthonormal basis
&#x27E8; m  |  n &#x27E9; =  &#x03B4;  m n     {\displaystyle \langle
m|n\rangle =\delta _{mn}}  [\langle m|n\rangle =\delta _{mn}], the cases of m =
n and m â  n can be discussed separately. The first case will lead to the
first theorem and the second case to the second theorem, which can be shown
immediately by rearranging the terms. With the differential rules given by the
HellmannâFeynman theorems, the perturbative correction to the energies and
states can be calculated systematically.
*** Correction of energy and state[edit] ***
To the second order, the energy correction reads
          E  n   (  x  &#x03BC;   ) = &#x27E8; n  |  H  |  n &#x27E9; +
      &#x27E8; n  |   &#x2202;  &#x03BC;   H  |  n &#x27E9;  x  &#x03BC;   +
      &#x211C;  &#x2211;  m &#x2260; n      &#x27E8; n  |   &#x2202;  &#x03BD;
      H  |  m &#x27E9; &#x27E8; m  |   &#x2202;  &#x03BC;   H  |  n &#x27E9;
      E  n   &#x2212;  E  m       x  &#x03BC;    x  &#x03BD;   + &#x22EF; ,
      {\displaystyle E_{n}(x^{\mu })=\langle n|H|n\rangle +\langle n|\partial _
      {\mu }H|n\rangle x^{\mu }+\Re \sum _{m\neq n}{\frac {\langle n|\partial _
      {\nu }H|m\rangle \langle m|\partial _{\mu }H|n\rangle }{E_{n}-E_{m}}}x^
      {\mu }x^{\nu }+\cdots ,}  [{\displaystyle E_{n}(x^{\mu })=\langle
      n|H|n\rangle +\langle n|\partial _{\mu }H|n\rangle x^{\mu }+\Re \sum _
      {m\neq n}{\frac {\langle n|\partial _{\nu }H|m\rangle \langle m|\partial
      _{\mu }H|n\rangle }{E_{n}-E_{m}}}x^{\mu }x^{\nu }+\cdots ,}]
where     &#x211C;   {\displaystyle \Re }  [\Re ] denotes the real_part
function. The first order derivative âÎ¼En is given by the first
HellmannâFeynman theorem directly. To obtain the second order derivative
âÎ¼âÎ½En, simply applying the differential operator âÎ¼ to the result of
the first order derivative     &#x27E8; n  |   &#x2202;  &#x03BD;   H  |  n
&#x27E9;   {\displaystyle \langle n|\partial _{\nu }H|n\rangle }  [\langle
n|\partial _{\nu }H|n\rangle ], which reads
          &#x2202;  &#x03BC;    &#x2202;  &#x03BD;    E  n   = &#x27E8;
      &#x2202;  &#x03BC;   n  |   &#x2202;  &#x03BD;   H  |  n &#x27E9; +
      &#x27E8; n  |   &#x2202;  &#x03BC;    &#x2202;  &#x03BD;   H  |  n
      &#x27E9; + &#x27E8; n  |   &#x2202;  &#x03BD;   H  |   &#x2202;  &#x03BC;
      n &#x27E9; .   {\displaystyle \partial _{\mu }\partial _{\nu }E_
      {n}=\langle \partial _{\mu }n|\partial _{\nu }H|n\rangle +\langle
      n|\partial _{\mu }\partial _{\nu }H|n\rangle +\langle n|\partial _{\nu
      }H|\partial _{\mu }n\rangle .}  [\partial _{\mu }\partial _{\nu }E_
      {n}=\langle \partial _{\mu }n|\partial _{\nu }H|n\rangle +\langle
      n|\partial _{\mu }\partial _{\nu }H|n\rangle +\langle n|\partial _{\nu
      }H|\partial _{\mu }n\rangle .]
Note that for linearly parameterized Hamiltonian, there is no second derivative
âÎ¼âÎ½H = 0 on the operator level. Resolve the derivative of state by
inserting the complete set of basis,
          &#x2202;  &#x03BC;    &#x2202;  &#x03BD;    E  n   =  &#x2211;  m
      (  &#x27E8;  &#x2202;  &#x03BC;   n  |  m &#x27E9; &#x27E8; m  |
      &#x2202;  &#x03BD;   H  |  n &#x27E9; + &#x27E8; n  |   &#x2202;
      &#x03BD;   H  |  m &#x27E9; &#x27E8; m  |   &#x2202;  &#x03BC;   n
      &#x27E9;  )  ,   {\displaystyle \partial _{\mu }\partial _{\nu }E_
      {n}=\sum _{m}\left(\langle \partial _{\mu }n|m\rangle \langle m|\partial
      _{\nu }H|n\rangle +\langle n|\partial _{\nu }H|m\rangle \langle
      m|\partial _{\mu }n\rangle \right),}  [\partial _{\mu }\partial _{\nu }E_
      {n}=\sum _{m}\left(\langle \partial _{\mu }n|m\rangle \langle m|\partial
      _{\nu }H|n\rangle +\langle n|\partial _{\nu }H|m\rangle \langle
      m|\partial _{\mu }n\rangle \right),]
then all parts can be calculated using the HellmannâFeynman theorems. In
terms of Lie derivatives,     &#x27E8;  &#x2202;  &#x03BC;   n  |  n &#x27E9; =
&#x27E8; n  |   &#x2202;  &#x03BC;   n &#x27E9; = 0   {\displaystyle \langle
\partial _{\mu }n|n\rangle =\langle n|\partial _{\mu }n\rangle =0}  [\langle
\partial _{\mu }n|n\rangle =\langle n|\partial _{\mu }n\rangle =0] according to
the definition of the connection for the vector bundle. Therefore, the case m =
n can be excluded from the summation, which avoids the singularity of the
energy denominator. The same procedure can be carried on for higher order
derivatives, from which higher order corrections are obtained.
The same computational scheme is applicable for the correction of states. The
result to the second order is as follows
              |  n  (  x  &#x03BC;   )   &#x27E9;  =  |  n &#x27E9;    +
      &#x2211;  m &#x2260; n      &#x27E8; m  |   &#x2202;  &#x03BC;   H  |  n
      &#x27E9;    E  n   &#x2212;  E  m       |  m &#x27E9;  x  &#x03BC;
      +  (   &#x2211;  m &#x2260; n    &#x2211;  l &#x2260; n      &#x27E8; m
      |   &#x2202;  &#x03BC;   H  |  l &#x27E9; &#x27E8; l  |   &#x2202;
      &#x03BD;   H  |  n &#x27E9;   (  E  n   &#x2212;  E  m   ) (  E  n
      &#x2212;  E  l   )     |  m &#x27E9; &#x2212;  &#x2211;  m &#x2260; n
      &#x27E8; m  |   &#x2202;  &#x03BC;   H  |  n &#x27E9; &#x27E8; n  |
      &#x2202;  &#x03BD;   H  |  n &#x27E9;   (  E  n   &#x2212;  E  m    )  2
      |  m &#x27E9; &#x2212;   1 2    &#x2211;  m &#x2260; n      &#x27E8; n  |
      &#x2202;  &#x03BC;   H  |  m &#x27E9; &#x27E8; m  |   &#x2202;  &#x03BD;
      H  |  n &#x27E9;   (  E  n   &#x2212;  E  m    )  2       |  m &#x27E9;
      )   x  &#x03BC;    x  &#x03BD;   + &#x22EF; .       {\displaystyle
      {\begin{aligned}\left|n\left(x^{\mu }\right)\right\rangle =|n\rangle
      &+\sum _{m\neq n}{\frac {\langle m|\partial _{\mu }H|n\rangle }{E_{n}-E_
      {m}}}|m\rangle x^{\mu }\\&+\left(\sum _{m\neq n}\sum _{l\neq n}{\frac
      {\langle m|\partial _{\mu }H|l\rangle \langle l|\partial _{\nu
      }H|n\rangle }{(E_{n}-E_{m})(E_{n}-E_{l})}}|m\rangle -\sum _{m\neq n}
      {\frac {\langle m|\partial _{\mu }H|n\rangle \langle n|\partial _{\nu
      }H|n\rangle }{(E_{n}-E_{m})^{2}}}|m\rangle -{\frac {1}{2}}\sum _{m\neq n}
      {\frac {\langle n|\partial _{\mu }H|m\rangle \langle m|\partial _{\nu
      }H|n\rangle }{(E_{n}-E_{m})^{2}}}|m\rangle \right)x^{\mu }x^{\nu }+\cdots
      .\end{aligned}}}  [{\begin{aligned}\left|n\left(x^{\mu
      }\right)\right\rangle =|n\rangle &+\sum _{m\neq n}{\frac {\langle
      m|\partial _{\mu }H|n\rangle }{E_{n}-E_{m}}}|m\rangle x^{\mu }\\&+\left
      (\sum _{m\neq n}\sum _{l\neq n}{\frac {\langle m|\partial _{\mu
      }H|l\rangle \langle l|\partial _{\nu }H|n\rangle }{(E_{n}-E_{m})(E_{n}-E_
      {l})}}|m\rangle -\sum _{m\neq n}{\frac {\langle m|\partial _{\mu
      }H|n\rangle \langle n|\partial _{\nu }H|n\rangle }{(E_{n}-E_{m})^
      {2}}}|m\rangle -{\frac {1}{2}}\sum _{m\neq n}{\frac {\langle n|\partial _
      {\mu }H|m\rangle \langle m|\partial _{\nu }H|n\rangle }{(E_{n}-E_{m})^
      {2}}}|m\rangle \right)x^{\mu }x^{\nu }+\cdots .\end{aligned}}]
Both energy derivatives and state derivatives will be involved in deduction.
Whenever a state derivative is encountered, resolve it by inserting the
complete set of basis, then the Hellmann-Feynman theorem is applicable. Because
differentiation can be calculated systematically, the series expansion approach
to the perturbative corrections can be coded on computers with symbolic
processing software like Mathematica.
*** Effective Hamiltonian[edit] ***
Let H(0) be the Hamiltonian completely restricted either in the low-energy
subspace        H    L     {\displaystyle {\mathcal {H}}_{L}}  [{\mathcal {H}}_
{L}] or in the high-energy subspace        H    H     {\displaystyle {\mathcal
{H}}_{H}}  [{\mathcal {H}}_{H}], such that there is no matrix element in H(0)
connecting the low- and the high-energy subspaces, i.e.     &#x27E8; m  |  H
( 0 )  |  l &#x27E9; = 0   {\displaystyle \langle m|H(0)|l\rangle =0}  [\langle
m|H(0)|l\rangle =0] if     m &#x2208;    H    L   , l &#x2208;    H    H
{\displaystyle m\in {\mathcal {H}}_{L},l\in {\mathcal {H}}_{H}}  [m\in
{\mathcal {H}}_{L},l\in {\mathcal {H}}_{H}]. Let FÎ¼ = âÎ¼H be the coupling
terms connecting the subspaces. Then when the high energy degrees of freedoms
are integrated out, the effective Hamiltonian in the low energy subspace reads
[8]
          H  m n   eff    (  x  &#x03BC;   )  = &#x27E8; m  |  H  |  n &#x27E9;
      +  &#x03B4;  n m   &#x27E8; m  |   &#x2202;  &#x03BC;   H  |  n &#x27E9;
      x  &#x03BC;   +   1  2 !     &#x2211;  l &#x2208;    H    H
      (     &#x27E8; m  |   &#x2202;  &#x03BC;   H  |  l &#x27E9; &#x27E8; l  |
      &#x2202;  &#x03BD;   H  |  n &#x27E9;    E  m   &#x2212;  E  l      +
      &#x27E8; m  |   &#x2202;  &#x03BD;   H  |  l &#x27E9; &#x27E8; l  |
      &#x2202;  &#x03BC;   H  |  n &#x27E9;    E  n   &#x2212;  E  l       )
      x  &#x03BC;    x  &#x03BD;   + &#x22EF; .   {\displaystyle H_{mn}^{\text
      {eff}}\left(x^{\mu }\right)=\langle m|H|n\rangle +\delta _{nm}\langle
      m|\partial _{\mu }H|n\rangle x^{\mu }+{\frac {1}{2!}}\sum _{l\in
      {\mathcal {H}}_{H}}\left({\frac {\langle m|\partial _{\mu }H|l\rangle
      \langle l|\partial _{\nu }H|n\rangle }{E_{m}-E_{l}}}+{\frac {\langle
      m|\partial _{\nu }H|l\rangle \langle l|\partial _{\mu }H|n\rangle }{E_
      {n}-E_{l}}}\right)x^{\mu }x^{\nu }+\cdots .}  [{\displaystyle H_{mn}^
      {\text{eff}}\left(x^{\mu }\right)=\langle m|H|n\rangle +\delta _
      {nm}\langle m|\partial _{\mu }H|n\rangle x^{\mu }+{\frac {1}{2!}}\sum _
      {l\in {\mathcal {H}}_{H}}\left({\frac {\langle m|\partial _{\mu
      }H|l\rangle \langle l|\partial _{\nu }H|n\rangle }{E_{m}-E_{l}}}+{\frac
      {\langle m|\partial _{\nu }H|l\rangle \langle l|\partial _{\mu
      }H|n\rangle }{E_{n}-E_{l}}}\right)x^{\mu }x^{\nu }+\cdots .}]
Here     m , n &#x2208;    H    L     {\displaystyle m,n\in {\mathcal {H}}_{L}}
[m,n\in {\mathcal {H}}_{L}] are restricted in the low energy subspace. The
above result can be derived by power series expansion of     &#x27E8; m  |  H
(  x  &#x03BC;   )  |  n &#x27E9;   {\displaystyle \langle m|H(x^{\mu
})|n\rangle }  [\langle m|H(x^{\mu })|n\rangle ].
In a formal way it is possible to define an effective Hamiltonian that gives
exactly the low-lying energy states and wavefunctions.[9] In practice, some
kind of approximation (perturbation theory) is generally required.
***** Time-dependent perturbation theory[edit] *****
**** Method of variation of constants[edit] ****
Time-dependent perturbation theory, developed by Paul_Dirac, studies the effect
of a time-dependent perturbation V(t) applied to a time-independent Hamiltonian
H0.[10]
Since the perturbed Hamiltonian is time-dependent, so are its energy levels and
eigenstates. Thus, the goals of time-dependent perturbation theory are slightly
different from time-independent perturbation theory. One is interested in the
following quantities:
    * The time-dependent expectation_value of some observable A, for a given
      initial state.
    * The time-dependent amplitudes[clarification_needed] of those quantum
      states that are energy eigenkets (eigenvectors) in the unperturbed
      system.
The first quantity is important because it gives rise to the classical result
of an A measurement performed on a macroscopic number of copies of the
perturbed system. For example, we could take A to be the displacement in the x-
direction of the electron in a hydrogen atom, in which case the expected value,
when multiplied by an appropriate coefficient, gives the time-dependent
dielectric_polarization of a hydrogen gas. With an appropriate choice of
perturbation (i.e. an oscillating electric potential), this allows one to
calculate the AC permittivity of the gas.
The second quantity looks at the time-dependent probability of occupation for
each eigenstate. This is particularly useful in laser physics, where one is
interested in the populations of different atomic states in a gas when a time-
dependent electric field is applied. These probabilities are also useful for
calculating the "quantum broadening" of spectral_lines (see line_broadening)
and particle_decay in particle_physics and nuclear_physics.
We will briefly examine the method behind Dirac's formulation of time-dependent
perturbation theory. Choose an energy basis       |  n &#x27E9;
{\displaystyle {|n\rangle }}  [{|n\rangle }] for the unperturbed system. (We
drop the (0) superscripts for the eigenstates, because it is not useful to
speak of energy levels and eigenstates for the perturbed system.)
If the unperturbed system is an eigenstate (of the Hamiltonian)      |  j
&#x27E9;   {\displaystyle |j\rangle }  [|j\rangle ] at time t = 0, its state at
subsequent times varies only by a phase (in the SchrÃ¶dinger_picture, where
state vectors evolve in time and operators are constant),
          |  j ( t ) &#x27E9; =  e  &#x2212; i  E  j   t  /  &#x210F;    |  j
      &#x27E9; &#xA0; .   {\displaystyle |j(t)\rangle =e^{-iE_{j}t/\hbar
      }|j\rangle ~.}  [|j(t)\rangle =e^{-iE_{j}t/\hbar }|j\rangle ~.]
Now, introduce a time-dependent perturbing Hamiltonian V(t). The Hamiltonian of
the perturbed system is
         H =  H  0   + V ( t ) &#xA0; .   {\displaystyle H=H_{0}+V(t)~.}  [H=H_
      {0}+V(t)~.]
Let      |  &#x03C8; ( t ) &#x27E9;   {\displaystyle |\psi (t)\rangle }  [|\psi
(t)\rangle ] denote the quantum state of the perturbed system at time t. It
obeys the time-dependent SchrÃ¶dinger equation,
         H  |  &#x03C8; ( t ) &#x27E9; = i &#x210F;   &#x2202;  &#x2202; t
      |  &#x03C8; ( t ) &#x27E9; &#xA0; .   {\displaystyle H|\psi (t)\rangle
      =i\hbar {\frac {\partial }{\partial t}}|\psi (t)\rangle ~.}  [H|\psi
      (t)\rangle =i\hbar {\frac {\partial }{\partial t}}|\psi (t)\rangle ~.]
The quantum state at each instant can be expressed as a linear combination of
the complete eigenbasis of      |  n &#x27E9;   {\displaystyle |n\rangle }
[|n\rangle ]:
          |  &#x03C8; ( t ) &#x27E9; =  &#x2211;  n    c  n   ( t )
      e  &#x2212; i  E  n   t  /  &#x210F;    |  n &#x27E9; &#xA0; ,    
      {\displaystyle |\psi (t)\rangle =\sum _{n}c_{n}(t)e^{-iE_{n}t/      (1)
      \hbar }|n\rangle ~,}  [|\psi (t)\rangle =\sum _{n}c_{n}(t)e^{-
      iE_{n}t/\hbar }|n\rangle ~,]
where the cn(t)s are to be determined complex functions of t which we will
refer to as amplitudes (strictly speaking, they are the amplitudes in the Dirac
picture).
We have explicitly extracted the exponential phase factors     exp &#x2061;
( &#x2212; i  E  n   t  /  &#x210F; )   {\displaystyle \exp(-iE_{n}t/\hbar )}
[\exp(-iE_{n}t/\hbar )] on the right hand side. This is only a matter of
convention, and may be done without loss of generality. The reason we go to
this trouble is that when the system starts in the state      |  j &#x27E9;
{\displaystyle |j\rangle }  [|j\rangle ] and no perturbation is present, the
amplitudes have the convenient property that, for all t, cj(t) = 1 and cn(t) =
0 if n â  j.
The square of the absolute amplitude cn(t) is the probability that the system
is in state n at time t, since
           |   c  n   ( t )  |   2   =   |  &#x27E8; n  |  &#x03C8; ( t )
      &#x27E9;  |   2   &#xA0; .   {\displaystyle \left|c_{n}(t)\right|^
      {2}=\left|\langle n|\psi (t)\rangle \right|^{2}~.}  [\left|c_{n}
      (t)\right|^{2}=\left|\langle n|\psi (t)\rangle \right|^{2}~.]
Plugging into the SchrÃ¶dinger equation and using the fact that â/ât acts
by a product_rule, one obtains
          &#x2211;  n    (  i &#x210F;     d   c  n      d  t    &#x2212;  c  n
      ( t ) V ( t )  )   e  &#x2212; i  E  n   t  /  &#x210F;    |  n &#x27E9;
      = 0 &#xA0; .   {\displaystyle \sum _{n}\left(i\hbar {\frac {\mathrm {d}
      c_{n}}{\mathrm {d} t}}-c_{n}(t)V(t)\right)e^{-iE_{n}t/\hbar }|n\rangle
      =0~.}  [{\displaystyle \sum _{n}\left(i\hbar {\frac {\mathrm {d} c_{n}}
      {\mathrm {d} t}}-c_{n}(t)V(t)\right)e^{-iE_{n}t/\hbar }|n\rangle =0~.}]
By resolving the identity in front of V and multiplying through by the bra
&#x27E8; n  |    {\displaystyle \langle n|}  [{\displaystyle \langle n|}] on
the left, this can be reduced to a set of coupled differential_equations for
the amplitudes,
             d   c  n      d  t    =    &#x2212; i  &#x210F;    &#x2211;  k
      &#x27E8; n  |  V ( t )  |  k &#x27E9;   c  k   ( t )   e  &#x2212; i (  E
      k   &#x2212;  E  n   ) t  /  &#x210F;   &#xA0; .   {\displaystyle {\frac
      {\mathrm {d} c_{n}}{\mathrm {d} t}}={\frac {-i}{\hbar }}\sum _{k}\langle
      n|V(t)|k\rangle \,c_{k}(t)\,e^{-i(E_{k}-E_{n})t/\hbar }~.}  [
      {\displaystyle {\frac {\mathrm {d} c_{n}}{\mathrm {d} t}}={\frac {-i}
      {\hbar }}\sum _{k}\langle n|V(t)|k\rangle \,c_{k}(t)\,e^{-i(E_{k}-E_
      {n})t/\hbar }~.}]
where we have used equation (1) to evaluate the sum on n in the second term,
then used the fact that     &#x27E8; k  |  &#x03A8; ( t ) &#x27E9; =  c  k
( t )  e  &#x2212; i  E  k   t  /  &#x210F;     {\displaystyle \langle k|\Psi
(t)\rangle =c_{k}(t)e^{-iE_{k}t/\hbar }}  [{\displaystyle \langle k|\Psi
(t)\rangle =c_{k}(t)e^{-iE_{k}t/\hbar }}].
The matrix elements of V play a similar role as in time-independent
perturbation theory, being proportional to the rate at which amplitudes are
shifted between states. Note, however, that the direction of the shift is
modified by the exponential phase factor. Over times much longer than the
energy difference Ek â En, the phase winds around 0 several times. If the
time-dependence of V is sufficiently slow, this may cause the state amplitudes
to oscillate. ( E.g., such oscillations are useful for managing radiative
transitions in a laser.)
Up to this point, we have made no approximations, so this set of differential
equations is exact. By supplying appropriate initial values cn(t), we could in
principle find an exact (i.e., non-perturbative) solution. This is easily done
when there are only two energy levels (n = 1, 2), and this solution is useful
for modelling systems like the ammonia molecule.
However, exact solutions are difficult to find when there are many energy
levels, and one instead looks for perturbative solutions. These may be obtained
by expressing the equations in an integral form,
          c  n   ( t ) =  c  n   ( 0 ) +    &#x2212; i  &#x210F;    &#x2211;  k
      &#x222B;  0   t   d  t &#x2032;   &#x27E8; n  |  V (  t &#x2032;  )  |  k
      &#x27E9;   c  k   (  t &#x2032;  )   e  &#x2212; i (  E  k   &#x2212;  E
      n   )  t &#x2032;   /  &#x210F;   &#xA0; .   {\displaystyle c_{n}(t)=c_
      {n}(0)+{\frac {-i}{\hbar }}\sum _{k}\int _{0}^{t}dt'\;\langle n|V
      (t')|k\rangle \,c_{k}(t')\,e^{-i(E_{k}-E_{n})t'/\hbar }~.}  [c_{n}(t)=c_
      {n}(0)+{\frac {-i}{\hbar }}\sum _{k}\int _{0}^{t}dt'\;\langle n|V
      (t')|k\rangle \,c_{k}(t')\,e^{-i(E_{k}-E_{n})t'/\hbar }~.]
Repeatedly substituting this expression for cn back into right hand side,
yields an iterative solution,
          c  n   ( t ) =  c  n   ( 0 )   +  c  n   ( 1 )   +  c  n   ( 2 )   +
      &#x22EF;   {\displaystyle c_{n}(t)=c_{n}^{(0)}+c_{n}^{(1)}+c_{n}^{
      (2)}+\cdots }  [c_{n}(t)=c_{n}^{(0)}+c_{n}^{(1)}+c_{n}^{(2)}+\cdots ]
where, for example, the first-order term is
          c  n   ( 1 )   ( t ) =    &#x2212; i  &#x210F;    &#x2211;  k
      &#x222B;  0   t   d  t &#x2032;   &#x27E8; n  |  V (  t &#x2032;  )  |  k
      &#x27E9;   c  k   ( 0 )     e  &#x2212; i (  E  k   &#x2212;  E  n   )  t
      &#x2032;   /  &#x210F;   &#xA0; .   {\displaystyle c_{n}^{(1)}(t)={\frac
      {-i}{\hbar }}\sum _{k}\int _{0}^{t}dt'\;\langle n|V(t')|k\rangle \,c_{k}^
      {(0)}\,e^{-i(E_{k}-E_{n})t'/\hbar }~.}  [{\displaystyle c_{n}^{(1)}(t)=
      {\frac {-i}{\hbar }}\sum _{k}\int _{0}^{t}dt'\;\langle n|V(t')|k\rangle
      \,c_{k}^{(0)}\,e^{-i(E_{k}-E_{n})t'/\hbar }~.}]
Several further results follow from this, such as Fermi's_golden_rule, which
relates the rate of transitions between quantum states to the density of states
at particular energies; or the Dyson_series, obtained by applying the iterative
method to the time_evolution_operator, which is one of the starting points for
the method of Feynman_diagrams.
**** Method of Dyson series[edit] ****
Time-dependent perturbations can be reorganized through the technique of the
Dyson_series. The SchrÃ¶dinger_equation
         H ( t )  |  &#x03C8; ( t ) &#x27E9; = i &#x210F;    &#x2202;  |
      &#x03C8; ( t ) &#x27E9;   &#x2202; t      {\displaystyle H(t)|\psi
      (t)\rangle =i\hbar {\frac {\partial |\psi (t)\rangle }{\partial t}}}  [H
      (t)|\psi (t)\rangle =i\hbar {\frac {\partial |\psi (t)\rangle }{\partial
      t}}]
has the formal solution
          |  &#x03C8; ( t ) &#x27E9; = T exp &#x2061;   [  &#x2212;   i
      &#x210F;    &#x222B;   t  0     t   d  t &#x2032;  H (  t &#x2032;  )  ]
      |  &#x03C8; (  t  0   ) &#x27E9; &#xA0; ,   {\displaystyle |\psi
      (t)\rangle =T\exp {\left[-{\frac {i}{\hbar }}\int _{t_{0}}^{t}dt'H
      (t')\right]}|\psi (t_{0})\rangle ~,}  [|\psi (t)\rangle =T\exp {\left[-
      {\frac {i}{\hbar }}\int _{t_{0}}^{t}dt'H(t')\right]}|\psi (t_{0})\rangle
      ~,]
where T is the time ordering operator,
         T A (  t  1   ) A (  t  2   ) =   {    A (  t  1   ) A (  t  2   )
      t  1   >  t  2       A (  t  2   ) A (  t  1   )    t  2   >  t  1
      &#xA0; .   {\displaystyle TA(t_{1})A(t_{2})={\begin{cases}A(t_{1})A(t_
      {2})&t_{1}>t_{2}\\A(t_{2})A(t_{1})&t_{2}>t_{1}\end{cases}}~.}  [TA(t_
      {1})A(t_{2})={\begin{cases}A(t_{1})A(t_{2})&t_{1}>t_{2}\\A(t_{2})A(t_
      {1})&t_{2}>t_{1}\end{cases}}~.]
Thus, the exponential represents the following Dyson_series,
          |  &#x03C8; ( t ) &#x27E9; =  [  1 &#x2212;   i &#x210F;    &#x222B;
      t  0     t   d  t  1   H (  t  1   ) &#x2212;   1  &#x210F;  2
      &#x222B;   t  0     t   d  t  1    &#x222B;   t  0      t  1     d  t  2
      H (  t  1   ) H (  t  2   ) + &#x2026;  ]   |  &#x03C8; (  t  0   )
      &#x27E9; &#xA0; .   {\displaystyle |\psi (t)\rangle =\left[1-{\frac {i}
      {\hbar }}\int _{t_{0}}^{t}dt_{1}H(t_{1})-{\frac {1}{\hbar ^{2}}}\int _{t_
      {0}}^{t}dt_{1}\int _{t_{0}}^{t_{1}}dt_{2}H(t_{1})H(t_{2})+\ldots
      \right]|\psi (t_{0})\rangle ~.}  [|\psi (t)\rangle =\left[1-{\frac {i}
      {\hbar }}\int _{t_{0}}^{t}dt_{1}H(t_{1})-{\frac {1}{\hbar ^{2}}}\int _{t_
      {0}}^{t}dt_{1}\int _{t_{0}}^{t_{1}}dt_{2}H(t_{1})H(t_{2})+\ldots
      \right]|\psi (t_{0})\rangle ~.]
Note that in the second term, the 1/2! factor exactly cancels the double
contribution due to the time-ordering operator, etc.
Consider the following perturbation problem
         [  H  0   + &#x03BB; V ( t ) ]  |  &#x03C8; ( t ) &#x27E9; = i
      &#x210F;    &#x2202;  |  &#x03C8; ( t ) &#x27E9;   &#x2202; t    &#xA0; ,
      {\displaystyle [H_{0}+\lambda V(t)]|\psi (t)\rangle =i\hbar {\frac
      {\partial |\psi (t)\rangle }{\partial t}}~,}  [[H_{0}+\lambda V(t)]|\psi
      (t)\rangle =i\hbar {\frac {\partial |\psi (t)\rangle }{\partial t}}~,]
assuming that the parameter Î» is small and that the problem      H  0    |  n
&#x27E9; =  E  n    |  n &#x27E9;   {\displaystyle H_{0}|n\rangle =E_
{n}|n\rangle }  [H_{0}|n\rangle =E_{n}|n\rangle ] has been solved.
Perform the following unitary transformation to the interaction_picture (or
Dirac picture),
          |  &#x03C8; ( t ) &#x27E9; =  e  &#x2212;   i &#x210F;    H  0   ( t
      &#x2212;  t  0   )    |   &#x03C8;  I   ( t ) &#x27E9; &#xA0; .
      {\displaystyle |\psi (t)\rangle =e^{-{\frac {i}{\hbar }}H_{0}(t-t_
      {0})}|\psi _{I}(t)\rangle ~.}  [|\psi (t)\rangle =e^{-{\frac {i}{\hbar
      }}H_{0}(t-t_{0})}|\psi _{I}(t)\rangle ~.]
Consequently, the SchrÃ¶dinger_equation simplifies to
         &#x03BB;  e    i &#x210F;    H  0   ( t &#x2212;  t  0   )   V ( t )
      e  &#x2212;   i &#x210F;    H  0   ( t &#x2212;  t  0   )    |   &#x03C8;
      I   ( t ) &#x27E9; = i &#x210F;    &#x2202;  |   &#x03C8;  I   ( t )
      &#x27E9;   &#x2202; t    &#xA0; ,   {\displaystyle \lambda e^{{\frac {i}
      {\hbar }}H_{0}(t-t_{0})}V(t)e^{-{\frac {i}{\hbar }}H_{0}(t-t_{0})}|\psi _
      {I}(t)\rangle =i\hbar {\frac {\partial |\psi _{I}(t)\rangle }{\partial
      t}}~,}  [\lambda e^{{\frac {i}{\hbar }}H_{0}(t-t_{0})}V(t)e^{-{\frac {i}
      {\hbar }}H_{0}(t-t_{0})}|\psi _{I}(t)\rangle =i\hbar {\frac {\partial
      |\psi _{I}(t)\rangle }{\partial t}}~,]
so it is solved through the above Dyson_series,
          |   &#x03C8;  I   ( t ) &#x27E9; =  [  1 &#x2212;    i &#x03BB;
      &#x210F;    &#x222B;   t  0     t   d  t  1    e    i &#x210F;    H  0
      (  t  1   &#x2212;  t  0   )   V (  t  1   )  e  &#x2212;   i &#x210F;
      H  0   (  t  1   &#x2212;  t  0   )   &#x2212;    &#x03BB;  2    &#x210F;
      2      &#x222B;   t  0     t   d  t  1    &#x222B;   t  0      t  1     d
      t  2    e    i &#x210F;    H  0   (  t  1   &#x2212;  t  0   )   V (  t
      1   )  e  &#x2212;   i &#x210F;    H  0   (  t  1   &#x2212;  t  0   )
      e    i &#x210F;    H  0   (  t  2   &#x2212;  t  0   )   V (  t  2   )  e
      &#x2212;   i &#x210F;    H  0   (  t  2   &#x2212;  t  0   )   + &#x2026;
      ]   |  &#x03C8; (  t  0   ) &#x27E9; &#xA0; ,   {\displaystyle |\psi _{I}
      (t)\rangle =\left[1-{\frac {i\lambda }{\hbar }}\int _{t_{0}}^{t}dt_{1}e^{
      {\frac {i}{\hbar }}H_{0}(t_{1}-t_{0})}V(t_{1})e^{-{\frac {i}{\hbar }}H_
      {0}(t_{1}-t_{0})}-{\frac {\lambda ^{2}}{\hbar ^{2}}}\int _{t_{0}}^{t}dt_
      {1}\int _{t_{0}}^{t_{1}}dt_{2}e^{{\frac {i}{\hbar }}H_{0}(t_{1}-t_{0})}V
      (t_{1})e^{-{\frac {i}{\hbar }}H_{0}(t_{1}-t_{0})}e^{{\frac {i}{\hbar }}H_
      {0}(t_{2}-t_{0})}V(t_{2})e^{-{\frac {i}{\hbar }}H_{0}(t_{2}-t_
      {0})}+\ldots \right]|\psi (t_{0})\rangle ~,}  [|\psi _{I}(t)\rangle
      =\left[1-{\frac {i\lambda }{\hbar }}\int _{t_{0}}^{t}dt_{1}e^{{\frac {i}
      {\hbar }}H_{0}(t_{1}-t_{0})}V(t_{1})e^{-{\frac {i}{\hbar }}H_{0}(t_{1}-t_
      {0})}-{\frac {\lambda ^{2}}{\hbar ^{2}}}\int _{t_{0}}^{t}dt_{1}\int _{t_
      {0}}^{t_{1}}dt_{2}e^{{\frac {i}{\hbar }}H_{0}(t_{1}-t_{0})}V(t_{1})e^{-
      {\frac {i}{\hbar }}H_{0}(t_{1}-t_{0})}e^{{\frac {i}{\hbar }}H_{0}(t_{2}-
      t_{0})}V(t_{2})e^{-{\frac {i}{\hbar }}H_{0}(t_{2}-t_{0})}+\ldots
      \right]|\psi (t_{0})\rangle ~,]
as a perturbation series with small Î».
Using the solution of the unperturbed problem      H  0    |  n &#x27E9; =  E
n    |  n &#x27E9;   {\displaystyle H_{0}|n\rangle =E_{n}|n\rangle }  [H_
{0}|n\rangle =E_{n}|n\rangle ] and      &#x2211;  n    |  n &#x27E9; &#x27E8; n
|  = 1   {\displaystyle \sum _{n}|n\rangle \langle n|=1}  [\sum _{n}|n\rangle
\langle n|=1] (for the sake of simplicity assume a pure discrete spectrum),
yields, to first order,
          |   &#x03C8;  I   ( t ) &#x27E9; =  [  1 &#x2212;    i &#x03BB;
      &#x210F;    &#x2211;  m    &#x2211;  n    &#x222B;   t  0     t   d  t  1
      &#x27E8; m  |  V (  t  1   )  |  n &#x27E9;  e  &#x2212;   i &#x210F;
      (  E  n   &#x2212;  E  m   ) (  t  1   &#x2212;  t  0   )    |  m
      &#x27E9; &#x27E8; n  |  + &#x2026;  ]   |  &#x03C8; (  t  0   ) &#x27E9;
      &#xA0; .   {\displaystyle |\psi _{I}(t)\rangle =\left[1-{\frac {i\lambda
      }{\hbar }}\sum _{m}\sum _{n}\int _{t_{0}}^{t}dt_{1}\langle m|V(t_
      {1})|n\rangle e^{-{\frac {i}{\hbar }}(E_{n}-E_{m})(t_{1}-t_{0})}|m\rangle
      \langle n|+\ldots \right]|\psi (t_{0})\rangle ~.}  [|\psi _{I}(t)\rangle
      =\left[1-{\frac {i\lambda }{\hbar }}\sum _{m}\sum _{n}\int _{t_{0}}^
      {t}dt_{1}\langle m|V(t_{1})|n\rangle e^{-{\frac {i}{\hbar }}(E_{n}-E_{m})
      (t_{1}-t_{0})}|m\rangle \langle n|+\ldots \right]|\psi (t_{0})\rangle ~.]
Thus, the system, initially in the unperturbed state      |  &#x03B1; &#x27E9;
=  |  &#x03C8; (  t  0   ) &#x27E9;   {\displaystyle |\alpha \rangle =|\psi (t_
{0})\rangle }  [|\alpha \rangle =|\psi (t_{0})\rangle ], by dint of the
perturbation can go into the state      |  &#x03B2; &#x27E9;   {\displaystyle
|\beta \rangle }  [|\beta \rangle ]. The corresponding transition probability
amplitude to first order is
          A  &#x03B1; &#x03B2;   = &#x2212;    i &#x03BB;  &#x210F;    &#x222B;
      t  0     t   d  t  1   &#x27E8; &#x03B2;  |  V (  t  1   )  |  &#x03B1;
      &#x27E9;  e  &#x2212;   i &#x210F;   (  E  &#x03B1;   &#x2212;  E
      &#x03B2;   ) (  t  1   &#x2212;  t  0   )   &#xA0; ,   {\displaystyle A_
      {\alpha \beta }=-{\frac {i\lambda }{\hbar }}\int _{t_{0}}^{t}dt_
      {1}\langle \beta |V(t_{1})|\alpha \rangle e^{-{\frac {i}{\hbar }}(E_
      {\alpha }-E_{\beta })(t_{1}-t_{0})}~,}  [A_{\alpha \beta }=-{\frac
      {i\lambda }{\hbar }}\int _{t_{0}}^{t}dt_{1}\langle \beta |V(t_{1})|\alpha
      \rangle e^{-{\frac {i}{\hbar }}(E_{\alpha }-E_{\beta })(t_{1}-t_{0})}~,]
as detailed in the previous sectionââwhile the corresponding transition
probability to a continuum is furnished by Fermi's_golden_rule.
As an aside, note that time-independent perturbation theory is also organized
inside this time-dependent perturbation theory Dyson series. To see this, write
the unitary evolution operator, obtained from the above Dyson_series, as
         U ( t ) = 1 &#x2212;    i &#x03BB;  &#x210F;    &#x222B;   t  0     t
      d  t  1    e    i &#x210F;    H  0   (  t  1   &#x2212;  t  0   )   V
      (  t  1   )  e  &#x2212;   i &#x210F;    H  0   (  t  1   &#x2212;  t  0
      )   &#x2212;    &#x03BB;  2    &#x210F;  2      &#x222B;   t  0     t   d
      t  1    &#x222B;   t  0      t  1     d  t  2    e    i &#x210F;    H  0
      (  t  1   &#x2212;  t  0   )   V (  t  1   )  e  &#x2212;   i &#x210F;
      H  0   (  t  1   &#x2212;  t  0   )    e    i &#x210F;    H  0   (  t  2
      &#x2212;  t  0   )   V (  t  2   )  e  &#x2212;   i &#x210F;    H  0
      (  t  2   &#x2212;  t  0   )   + &#x22EF;   {\displaystyle U(t)=1-{\frac
      {i\lambda }{\hbar }}\int _{t_{0}}^{t}dt_{1}e^{{\frac {i}{\hbar }}H_{0}(t_
      {1}-t_{0})}V(t_{1})e^{-{\frac {i}{\hbar }}H_{0}(t_{1}-t_{0})}-{\frac
      {\lambda ^{2}}{\hbar ^{2}}}\int _{t_{0}}^{t}dt_{1}\int _{t_{0}}^{t_
      {1}}dt_{2}e^{{\frac {i}{\hbar }}H_{0}(t_{1}-t_{0})}V(t_{1})e^{-{\frac {i}
      {\hbar }}H_{0}(t_{1}-t_{0})}e^{{\frac {i}{\hbar }}H_{0}(t_{2}-t_{0})}V(t_
      {2})e^{-{\frac {i}{\hbar }}H_{0}(t_{2}-t_{0})}+\cdots }  [U(t)=1-{\frac
      {i\lambda }{\hbar }}\int _{t_{0}}^{t}dt_{1}e^{{\frac {i}{\hbar }}H_{0}(t_
      {1}-t_{0})}V(t_{1})e^{-{\frac {i}{\hbar }}H_{0}(t_{1}-t_{0})}-{\frac
      {\lambda ^{2}}{\hbar ^{2}}}\int _{t_{0}}^{t}dt_{1}\int _{t_{0}}^{t_
      {1}}dt_{2}e^{{\frac {i}{\hbar }}H_{0}(t_{1}-t_{0})}V(t_{1})e^{-{\frac {i}
      {\hbar }}H_{0}(t_{1}-t_{0})}e^{{\frac {i}{\hbar }}H_{0}(t_{2}-t_{0})}V(t_
      {2})e^{-{\frac {i}{\hbar }}H_{0}(t_{2}-t_{0})}+\cdots ]
and take the perturbation V to be time-independent.
Using the identity resolution
          &#x2211;  n    |  n &#x27E9; &#x27E8; n  |  = 1   {\displaystyle \sum
      _{n}|n\rangle \langle n|=1}  [\sum _{n}|n\rangle \langle n|=1]
with      H  0    |  n &#x27E9; =  E  n    |  n &#x27E9;   {\displaystyle H_
{0}|n\rangle =E_{n}|n\rangle }  [H_{0}|n\rangle =E_{n}|n\rangle ] for a pure
discrete spectrum, write
             U ( t ) = 1    &#x2212;  {     i &#x03BB;  &#x210F;    &#x222B;
      t  0     t   d  t  1    &#x2211;  m    &#x2211;  n   &#x27E8; m  |  V  |
      n &#x27E9;  e  &#x2212;   i &#x210F;   (  E  n   &#x2212;  E  m   ) (  t
      1   &#x2212;  t  0   )    |  m &#x27E9; &#x27E8; n  |   }        &#x2212;
      {     &#x03BB;  2    &#x210F;  2      &#x222B;   t  0     t   d  t  1
      &#x222B;   t  0      t  1     d  t  2    &#x2211;  m    &#x2211;  n
      &#x2211;  q    e  &#x2212;   i &#x210F;   (  E  n   &#x2212;  E  m   )
      (  t  1   &#x2212;  t  0   )   &#x27E8; m  |  V  |  n &#x27E9; &#x27E8; n
      |  V  |  q &#x27E9;  e  &#x2212;   i &#x210F;   (  E  q   &#x2212;  E  n
      ) (  t  2   &#x2212;  t  0   )    |  m &#x27E9; &#x27E8; q  |   }  +
      &#x22EF;       {\displaystyle {\begin{aligned}U(t)=1&-\left\{{\frac
      {i\lambda }{\hbar }}\int _{t_{0}}^{t}dt_{1}\sum _{m}\sum _{n}\langle
      m|V|n\rangle e^{-{\frac {i}{\hbar }}(E_{n}-E_{m})(t_{1}-t_{0})}|m\rangle
      \langle n|\right\}\\&-\left\{{\frac {\lambda ^{2}}{\hbar ^{2}}}\int _{t_
      {0}}^{t}dt_{1}\int _{t_{0}}^{t_{1}}dt_{2}\sum _{m}\sum _{n}\sum _{q}e^{-
      {\frac {i}{\hbar }}(E_{n}-E_{m})(t_{1}-t_{0})}\langle m|V|n\rangle
      \langle n|V|q\rangle e^{-{\frac {i}{\hbar }}(E_{q}-E_{n})(t_{2}-t_
      {0})}|m\rangle \langle q|\right\}+\cdots \end{aligned}}}  [{\begin
      {aligned}U(t)=1&-\left\{{\frac {i\lambda }{\hbar }}\int _{t_{0}}^{t}dt_
      {1}\sum _{m}\sum _{n}\langle m|V|n\rangle e^{-{\frac {i}{\hbar }}(E_{n}-
      E_{m})(t_{1}-t_{0})}|m\rangle \langle n|\right\}\\&-\left\{{\frac
      {\lambda ^{2}}{\hbar ^{2}}}\int _{t_{0}}^{t}dt_{1}\int _{t_{0}}^{t_
      {1}}dt_{2}\sum _{m}\sum _{n}\sum _{q}e^{-{\frac {i}{\hbar }}(E_{n}-E_{m})
      (t_{1}-t_{0})}\langle m|V|n\rangle \langle n|V|q\rangle e^{-{\frac {i}
      {\hbar }}(E_{q}-E_{n})(t_{2}-t_{0})}|m\rangle \langle q|\right\}+\cdots
      \end{aligned}}]
It is evident that, at second order, one must sum on all the intermediate
states. Assume      t  0   = 0   {\displaystyle t_{0}=0}  [t_{0}=0] and the
asymptotic limit of larger times. This means that, at each contribution of the
perturbation series, one has to add a multiplicative factor      e  &#x2212;
&#x03F5; t     {\displaystyle e^{-\epsilon t}}  [e^{-\epsilon t}] in the
integrands for Îµ arbitrarily small. Thus the limit t â â gives back the
final state of the system by eliminating all oscillating terms, but keeping the
secular ones. The integrals are thus computable, and, separating the diagonal
terms from the others yields
             U ( t ) = 1    &#x2212;    i &#x03BB;  &#x210F;    &#x2211;  n
      &#x27E8; n  |  V  |  n &#x27E9; t &#x2212;    i  &#x03BB;  2    &#x210F;
      &#x2211;  m &#x2260; n      &#x27E8; n  |  V  |  m &#x27E9; &#x27E8; m  |
      V  |  n &#x27E9;    E  n   &#x2212;  E  m      t &#x2212;   1 2
      &#x03BB;  2    &#x210F;  2      &#x2211;  m , n   &#x27E8; n  |  V  |  m
      &#x27E9; &#x27E8; m  |  V  |  n &#x27E9;  t  2   + &#x2026;       +
      &#x03BB;  &#x2211;  m &#x2260; n      &#x27E8; m  |  V  |  n &#x27E9;
      E  n   &#x2212;  E  m       |  m &#x27E9; &#x27E8; n  |  +  &#x03BB;  2
      &#x2211;  m &#x2260; n    &#x2211;  q &#x2260; n    &#x2211;  n
      &#x27E8; m  |  V  |  n &#x27E9; &#x27E8; n  |  V  |  q &#x27E9;   (  E  n
      &#x2212;  E  m   ) (  E  q   &#x2212;  E  n   )     |  m &#x27E9;
      &#x27E8; q  |  + &#x2026;       {\displaystyle {\begin{aligned}U(t)=1&-
      {\frac {i\lambda }{\hbar }}\sum _{n}\langle n|V|n\rangle t-{\frac
      {i\lambda ^{2}}{\hbar }}\sum _{m\neq n}{\frac {\langle n|V|m\rangle
      \langle m|V|n\rangle }{E_{n}-E_{m}}}t-{\frac {1}{2}}{\frac {\lambda ^{2}}
      {\hbar ^{2}}}\sum _{m,n}\langle n|V|m\rangle \langle m|V|n\rangle t^
      {2}+\ldots \\&+\lambda \sum _{m\neq n}{\frac {\langle m|V|n\rangle }{E_
      {n}-E_{m}}}|m\rangle \langle n|+\lambda ^{2}\sum _{m\neq n}\sum _{q\neq
      n}\sum _{n}{\frac {\langle m|V|n\rangle \langle n|V|q\rangle }{(E_{n}-E_
      {m})(E_{q}-E_{n})}}|m\rangle \langle q|+\ldots \end{aligned}}}  [
      {\displaystyle {\begin{aligned}U(t)=1&-{\frac {i\lambda }{\hbar }}\sum _
      {n}\langle n|V|n\rangle t-{\frac {i\lambda ^{2}}{\hbar }}\sum _{m\neq n}
      {\frac {\langle n|V|m\rangle \langle m|V|n\rangle }{E_{n}-E_{m}}}t-{\frac
      {1}{2}}{\frac {\lambda ^{2}}{\hbar ^{2}}}\sum _{m,n}\langle n|V|m\rangle
      \langle m|V|n\rangle t^{2}+\ldots \\&+\lambda \sum _{m\neq n}{\frac
      {\langle m|V|n\rangle }{E_{n}-E_{m}}}|m\rangle \langle n|+\lambda ^
      {2}\sum _{m\neq n}\sum _{q\neq n}\sum _{n}{\frac {\langle m|V|n\rangle
      \langle n|V|q\rangle }{(E_{n}-E_{m})(E_{q}-E_{n})}}|m\rangle \langle
      q|+\ldots \end{aligned}}}]
where the time secular series yields the eigenvalues of the perturbed problem
specified above, recursively; whereas the remaining time-constant part yields
the corrections to the stationary eigenfunctions also given above (     |  n
( &#x03BB; ) &#x27E9; = U ( 0 ; &#x03BB; )  |  n &#x27E9; )   {\displaystyle |n
(\lambda )\rangle =U(0;\lambda )|n\rangle )}  [|n(\lambda )\rangle =U(0;\lambda
)|n\rangle )].)
The unitary evolution operator is applicable to arbitrary eigenstates of the
unperturbed problem and, in this case, yields a secular series that holds at
small times.
***** Strong perturbation theory[edit] *****
In a similar way as for small perturbations, it is possible to develop a strong
perturbation theory. Consider as usual the SchrÃ¶dinger_equation
         H ( t )  |  &#x03C8; ( t ) &#x27E9; = i &#x210F;    &#x2202;  |
      &#x03C8; ( t ) &#x27E9;   &#x2202; t      {\displaystyle H(t)|\psi
      (t)\rangle =i\hbar {\frac {\partial |\psi (t)\rangle }{\partial t}}}  [H
      (t)|\psi (t)\rangle =i\hbar {\frac {\partial |\psi (t)\rangle }{\partial
      t}}]
and we consider the question if a dual Dyson series exists that applies in the
limit of a perturbation increasingly large. This question can be answered in an
affirmative way [11] and the series is the well-known adiabatic series.[12]
This approach is quite general and can be shown in the following way. Consider
the perturbation problem
         [  H  0   + &#x03BB; V ( t ) ]  |  &#x03C8; ( t ) &#x27E9; = i
      &#x210F;    &#x2202;  |  &#x03C8; ( t ) &#x27E9;   &#x2202; t
      {\displaystyle [H_{0}+\lambda V(t)]|\psi (t)\rangle =i\hbar {\frac
      {\partial |\psi (t)\rangle }{\partial t}}}  [[H_{0}+\lambda V(t)]|\psi
      (t)\rangle =i\hbar {\frac {\partial |\psi (t)\rangle }{\partial t}}]
being Î»â â. Our aim is to find a solution in the form
          |  &#x03C8; &#x27E9; =  |   &#x03C8;  0   &#x27E9; +   1 &#x03BB;
      |   &#x03C8;  1   &#x27E9; +   1  &#x03BB;  2      |   &#x03C8;  2
      &#x27E9; + &#x2026;   {\displaystyle |\psi \rangle =|\psi _{0}\rangle +
      {\frac {1}{\lambda }}|\psi _{1}\rangle +{\frac {1}{\lambda ^{2}}}|\psi _
      {2}\rangle +\ldots }  [|\psi \rangle =|\psi _{0}\rangle +{\frac {1}
      {\lambda }}|\psi _{1}\rangle +{\frac {1}{\lambda ^{2}}}|\psi _{2}\rangle
      +\ldots ]
but a direct substitution into the above equation fails to produce useful
results. This situation can be adjusted making a rescaling of the time variable
as     &#x03C4; = &#x03BB; t   {\displaystyle \tau =\lambda t}  [\tau =\lambda
t] producing the following meaningful equations
         V ( t )  |   &#x03C8;  0   &#x27E9; = i &#x210F;    &#x2202;  |
      &#x03C8;  0   &#x27E9;   &#x2202; &#x03C4;      {\displaystyle V(t)|\psi
      _{0}\rangle =i\hbar {\frac {\partial |\psi _{0}\rangle }{\partial \tau
      }}}  [V(t)|\psi _{0}\rangle =i\hbar {\frac {\partial |\psi _{0}\rangle }
      {\partial \tau }}]
         V ( t )  |   &#x03C8;  1   &#x27E9; +  H  0    |   &#x03C8;  0
      &#x27E9; = i &#x210F;    &#x2202;  |   &#x03C8;  1   &#x27E9;   &#x2202;
      &#x03C4;      {\displaystyle V(t)|\psi _{1}\rangle +H_{0}|\psi _
      {0}\rangle =i\hbar {\frac {\partial |\psi _{1}\rangle }{\partial \tau }}}
      [V(t)|\psi _{1}\rangle +H_{0}|\psi _{0}\rangle =i\hbar {\frac {\partial
      |\psi _{1}\rangle }{\partial \tau }}]
         &#x22EE;   {\displaystyle \vdots }  [\vdots ]
that can be solved once we know the solution of the leading_order equation. But
we know that in this case we can use the adiabatic_approximation. When     V
( t )   {\displaystyle V(t)}  [V(t)] does not depend on time one gets the
Wigner-Kirkwood_series that is often used in statistical_mechanics. Indeed, in
this case we introduce the unitary transformation
          |  &#x03C8; ( t ) &#x27E9; =  e  &#x2212;   i &#x210F;   &#x03BB; V
      ( t &#x2212;  t  0   )    |   &#x03C8;  F   ( t ) &#x27E9;
      {\displaystyle |\psi (t)\rangle =e^{-{\frac {i}{\hbar }}\lambda V(t-t_
      {0})}|\psi _{F}(t)\rangle }  [|\psi (t)\rangle =e^{-{\frac {i}{\hbar
      }}\lambda V(t-t_{0})}|\psi _{F}(t)\rangle ]
that defines a free picture as we are trying to eliminate the interaction term.
Now, in dual way with respect to the small perturbations, we have to solve the
SchrÃ¶dinger_equation
          e    i &#x210F;   &#x03BB; V ( t &#x2212;  t  0   )    H  0    e
      &#x2212;   i &#x210F;   &#x03BB; V ( t &#x2212;  t  0   )    |   &#x03C8;
      F   ( t ) &#x27E9; = i &#x210F;    &#x2202;  |   &#x03C8;  F   ( t )
      &#x27E9;   &#x2202; t      {\displaystyle e^{{\frac {i}{\hbar }}\lambda V
      (t-t_{0})}H_{0}e^{-{\frac {i}{\hbar }}\lambda V(t-t_{0})}|\psi _{F}
      (t)\rangle =i\hbar {\frac {\partial |\psi _{F}(t)\rangle }{\partial t}}}
      [e^{{\frac {i}{\hbar }}\lambda V(t-t_{0})}H_{0}e^{-{\frac {i}{\hbar
      }}\lambda V(t-t_{0})}|\psi _{F}(t)\rangle =i\hbar {\frac {\partial |\psi
      _{F}(t)\rangle }{\partial t}}]
and we see that the expansion parameter Î» appears only into the exponential
and so, the corresponding Dyson_series, a dual Dyson series, is meaningful at
large Î»s and is
          |   &#x03C8;  F   ( t ) &#x27E9; =  [  1 &#x2212;   i &#x210F;
      &#x222B;   t  0     t   d  t  1    e    i &#x210F;   &#x03BB; V (  t  1
      &#x2212;  t  0   )    H  0    e  &#x2212;   i &#x210F;   &#x03BB; V (  t
      1   &#x2212;  t  0   )   &#x2212;   1  &#x210F;  2      &#x222B;   t  0
      t   d  t  1    &#x222B;   t  0      t  1     d  t  2    e    i &#x210F;
      &#x03BB; V (  t  1   &#x2212;  t  0   )    H  0    e  &#x2212;   i
      &#x210F;   &#x03BB; V (  t  1   &#x2212;  t  0   )    e    i &#x210F;
      &#x03BB; V (  t  2   &#x2212;  t  0   )    H  0    e  &#x2212;   i
      &#x210F;   &#x03BB; V (  t  2   &#x2212;  t  0   )   + &#x2026;  ]   |
      &#x03C8; (  t  0   ) &#x27E9; .   {\displaystyle |\psi _{F}(t)\rangle
      =\left[1-{\frac {i}{\hbar }}\int _{t_{0}}^{t}dt_{1}e^{{\frac {i}{\hbar
      }}\lambda V(t_{1}-t_{0})}H_{0}e^{-{\frac {i}{\hbar }}\lambda V(t_{1}-t_
      {0})}-{\frac {1}{\hbar ^{2}}}\int _{t_{0}}^{t}dt_{1}\int _{t_{0}}^{t_
      {1}}dt_{2}e^{{\frac {i}{\hbar }}\lambda V(t_{1}-t_{0})}H_{0}e^{-{\frac
      {i}{\hbar }}\lambda V(t_{1}-t_{0})}e^{{\frac {i}{\hbar }}\lambda V(t_{2}-
      t_{0})}H_{0}e^{-{\frac {i}{\hbar }}\lambda V(t_{2}-t_{0})}+\ldots
      \right]|\psi (t_{0})\rangle .}  [|\psi _{F}(t)\rangle =\left[1-{\frac {i}
      {\hbar }}\int _{t_{0}}^{t}dt_{1}e^{{\frac {i}{\hbar }}\lambda V(t_{1}-t_
      {0})}H_{0}e^{-{\frac {i}{\hbar }}\lambda V(t_{1}-t_{0})}-{\frac {1}{\hbar
      ^{2}}}\int _{t_{0}}^{t}dt_{1}\int _{t_{0}}^{t_{1}}dt_{2}e^{{\frac {i}
      {\hbar }}\lambda V(t_{1}-t_{0})}H_{0}e^{-{\frac {i}{\hbar }}\lambda V(t_
      {1}-t_{0})}e^{{\frac {i}{\hbar }}\lambda V(t_{2}-t_{0})}H_{0}e^{-{\frac
      {i}{\hbar }}\lambda V(t_{2}-t_{0})}+\ldots \right]|\psi (t_{0})\rangle .]
After the rescaling in time     &#x03C4; = &#x03BB; t   {\displaystyle \tau
=\lambda t}  [\tau =\lambda t] we can see that this is indeed a series in     1
/  &#x03BB;   {\displaystyle 1/\lambda }  [1/\lambda ] justifying in this way
the name of dual Dyson series. The reason is that we have obtained this series
simply interchanging H0 and V and we can go from one to another applying this
exchange. This is called duality principle in perturbation theory. The choice
H  0   =  p  2    /  2 m   {\displaystyle H_{0}=p^{2}/2m}  [H_{0}=p^{2}/2m]
yields, as already said, a Wigner-Kirkwood_series that is a gradient expansion.
The Wigner-Kirkwood_series is a semiclassical series with eigenvalues given
exactly as for WKB_approximation.[13]
***** Examples[edit] *****
**** Example of first order perturbation theory â ground state energy of the
quartic oscillator[edit] ****
Consider the quantum harmonic oscillator with the quartic potential
perturbation and the Hamiltonian
         H = &#x2212;    &#x210F;  2    2 m       &#x2202;  2    &#x2202;  x  2
      +    m  &#x03C9;  2    x  2    2   + &#x03BB;  x  4     {\displaystyle
      H=-{\frac {\hbar ^{2}}{2m}}{\frac {\partial ^{2}}{\partial x^{2}}}+{\frac
      {m\omega ^{2}x^{2}}{2}}+\lambda x^{4}}  [H=-{\frac {\hbar ^{2}}{2m}}
      {\frac {\partial ^{2}}{\partial x^{2}}}+{\frac {m\omega ^{2}x^{2}}
      {2}}+\lambda x^{4}]
The ground state of the harmonic oscillator is
          &#x03C8;  0   =   (   &#x03B1; &#x03C0;   )    1 4     e  &#x2212;
      &#x03B1;  x  2    /  2     {\displaystyle \psi _{0}=\left({\frac {\alpha
      }{\pi }}\right)^{\frac {1}{4}}e^{-\alpha x^{2}/2}}  [\psi _{0}=\left(
      {\frac {\alpha }{\pi }}\right)^{\frac {1}{4}}e^{-\alpha x^{2}/2}]
(    &#x03B1; = m &#x03C9;  /  &#x210F;   {\displaystyle \alpha =m\omega /\hbar
}  [\alpha =m\omega /\hbar ]) and the energy of unperturbed ground state is
          E  0   ( 0 )   =    1 2    &#x210F; &#x03C9; .    {\displaystyle E_
      {0}^{(0)}={\tfrac {1}{2}}\hbar \omega .\,}  [{\displaystyle E_{0}^{(0)}=
      {\tfrac {1}{2}}\hbar \omega .\,}]
Using the first order correction formula we get
          E  0   ( 1 )   = &#x03BB;   (   &#x03B1; &#x03C0;   )    1 2
      &#x222B;  e  &#x2212; &#x03B1;  x  2    /  2    x  4    e  &#x2212;
      &#x03B1;  x  2    /  2   d x = &#x03BB;   (   &#x03B1; &#x03C0;   )    1
      2       &#x2202;  2    &#x2202;  &#x03B1;  2      &#x222B;  e  &#x2212;
      &#x03B1;  x  2     d x   {\displaystyle E_{0}^{(1)}=\lambda \left({\frac
      {\alpha }{\pi }}\right)^{\frac {1}{2}}\int e^{-\alpha x^{2}/2}x^{4}e^{-
      \alpha x^{2}/2}dx=\lambda \left({\frac {\alpha }{\pi }}\right)^{\frac {1}
      {2}}{\frac {\partial ^{2}}{\partial \alpha ^{2}}}\int e^{-\alpha x^
      {2}}dx}  [E_{0}^{(1)}=\lambda \left({\frac {\alpha }{\pi }}\right)^{\frac
      {1}{2}}\int e^{-\alpha x^{2}/2}x^{4}e^{-\alpha x^{2}/2}dx=\lambda \left(
      {\frac {\alpha }{\pi }}\right)^{\frac {1}{2}}{\frac {\partial ^{2}}
      {\partial \alpha ^{2}}}\int e^{-\alpha x^{2}}dx]
or
          E  0   ( 1 )   = &#x03BB;   (   &#x03B1; &#x03C0;   )    1 2
      &#x2202;  2    &#x2202;  &#x03B1;  2        (   &#x03C0; &#x03B1;   )
      1 2    = &#x03BB;   3 4     1  &#x03B1;  2     =   3 4       &#x210F;  2
      &#x03BB;    m  2    &#x03C9;  2        {\displaystyle E_{0}^{(1)}=\lambda
      \left({\frac {\alpha }{\pi }}\right)^{\frac {1}{2}}{\frac {\partial ^{2}}
      {\partial \alpha ^{2}}}\left({\frac {\pi }{\alpha }}\right)^{\frac {1}
      {2}}=\lambda {\frac {3}{4}}{\frac {1}{\alpha ^{2}}}={\frac {3}{4}}{\frac
      {\hbar ^{2}\lambda }{m^{2}\omega ^{2}}}}  [E_{0}^{(1)}=\lambda \left(
      {\frac {\alpha }{\pi }}\right)^{\frac {1}{2}}{\frac {\partial ^{2}}
      {\partial \alpha ^{2}}}\left({\frac {\pi }{\alpha }}\right)^{\frac {1}
      {2}}=\lambda {\frac {3}{4}}{\frac {1}{\alpha ^{2}}}={\frac {3}{4}}{\frac
      {\hbar ^{2}\lambda }{m^{2}\omega ^{2}}}]
**** Example of first and second order perturbation theory â quantum pendulum
[edit] ****
Consider the quantum mathematical pendulum with the Hamiltonian
         H = &#x2212;    &#x210F;  2    2 m  a  2         &#x2202;  2
      &#x2202;  &#x03D5;  2      &#x2212; &#x03BB; cos &#x2061; &#x03D5;
      {\displaystyle H=-{\frac {\hbar ^{2}}{2ma^{2}}}{\frac {\partial ^{2}}
      {\partial \phi ^{2}}}-\lambda \cos \phi }  [H=-{\frac {\hbar ^{2}}{2ma^
      {2}}}{\frac {\partial ^{2}}{\partial \phi ^{2}}}-\lambda \cos \phi ]
with the potential energy     &#x2212; &#x03BB; cos &#x2061; &#x03D5;
{\displaystyle -\lambda \cos \phi }  [-\lambda \cos \phi ] taken as the
perturbation i.e.
         V = &#x2212; cos &#x2061; &#x03D5;   {\displaystyle V=-\cos \phi }  [
      {\displaystyle V=-\cos \phi }]
The unperturbed normalized quantum wave functions are those of the rigid rotor
and are given by
          &#x03C8;  n   ( &#x03D5; ) =    e  i n &#x03D5;    2 &#x03C0;
      {\displaystyle \psi _{n}(\phi )={\frac {e^{in\phi }}{\sqrt {2\pi }}}}
      [\psi _{n}(\phi )={\frac {e^{in\phi }}{\sqrt {2\pi }}}]
and the energies
          E  n   ( 0 )   =     &#x210F;  2    n  2     2 m  a  2
      {\displaystyle E_{n}^{(0)}={\frac {\hbar ^{2}n^{2}}{2ma^{2}}}}  [E_{n}^{
      (0)}={\frac {\hbar ^{2}n^{2}}{2ma^{2}}}]
The first order energy correction to the rotor due to the potential energy is
          E  n   ( 1 )   = &#x2212;   1  2 &#x03C0;    &#x222B;  e  &#x2212; i
      n &#x03D5;   cos &#x2061; &#x03D5;  e  i n &#x03D5;   = &#x2212;   1  2
      &#x03C0;    &#x222B; cos &#x2061; &#x03D5; = 0   {\displaystyle E_{n}^{
      (1)}=-{\frac {1}{2\pi }}\int e^{-in\phi }\cos \phi e^{in\phi }=-{\frac
      {1}{2\pi }}\int \cos \phi =0}  [E_{n}^{(1)}=-{\frac {1}{2\pi }}\int e^{-
      in\phi }\cos \phi e^{in\phi }=-{\frac {1}{2\pi }}\int \cos \phi =0]
Using the formula for the second order correction one gets
          E  n   ( 2 )   =    m  a  2     2  &#x03C0;  2    &#x210F;  2
      &#x2211;  k       |  &#x222B;  e  &#x2212; i k &#x03D5;   cos &#x2061;
      &#x03D5;  e  i n &#x03D5;    |   2     n  2   &#x2212;  k  2
      {\displaystyle E_{n}^{(2)}={\frac {ma^{2}}{2\pi ^{2}\hbar ^{2}}}\sum _{k}
      {\frac {\left|\int e^{-ik\phi }\cos \phi e^{in\phi }\right|^{2}}{n^{2}-k^
      {2}}}}  [E_{n}^{(2)}={\frac {ma^{2}}{2\pi ^{2}\hbar ^{2}}}\sum _{k}{\frac
      {\left|\int e^{-ik\phi }\cos \phi e^{in\phi }\right|^{2}}{n^{2}-k^{2}}}]
or
          E  n   ( 2 )   =    m  a  2     2  &#x210F;  2       &#x2211;  k
      |  (   &#x03B4;  n , 1 &#x2212; k   +  &#x03B4;  n , &#x2212; 1 &#x2212;
      k    )  |   2     n  2   &#x2212;  k  2        {\displaystyle E_{n}^{
      (2)}={\frac {ma^{2}}{2\hbar ^{2}}}\sum _{k}{\frac {\left|\left(\delta _
      {n,1-k}+\delta _{n,-1-k}\right)\right|^{2}}{n^{2}-k^{2}}}}  [E_{n}^{(2)}=
      {\frac {ma^{2}}{2\hbar ^{2}}}\sum _{k}{\frac {\left|\left(\delta _{n,1-
      k}+\delta _{n,-1-k}\right)\right|^{2}}{n^{2}-k^{2}}}]
or
          E  n   ( 2 )   =    m  a  2     2  &#x210F;  2       (    1  2 n
      &#x2212; 1    +   1  &#x2212; 2 n &#x2212; 1     )  =    m  a  2
      &#x210F;  2       1  4  n  2   &#x2212; 1      {\displaystyle E_{n}^{
      (2)}={\frac {ma^{2}}{2\hbar ^{2}}}\left({\frac {1}{2n-1}}+{\frac {1}{-2n-
      1}}\right)={\frac {ma^{2}}{\hbar ^{2}}}{\frac {1}{4n^{2}-1}}}  [E_{n}^{
      (2)}={\frac {ma^{2}}{2\hbar ^{2}}}\left({\frac {1}{2n-1}}+{\frac {1}{-2n-
      1}}\right)={\frac {ma^{2}}{\hbar ^{2}}}{\frac {1}{4n^{2}-1}}]
***** References[edit] *****
   1. ^Aoyama, Tatsumi; Hayakawa, Masashi; Kinoshita, Toichiro; Nio, Makiko
      (2012). "Tenth-order QED lepton anomalous magnetic moment: Eighth-order
      vertices containing a second-order vacuum polarization". Physical Review
      D. 85 (3): 033007. arXiv:1110.2826. Bibcode:2012PhRvD..85c3007A. doi:
      10.1103/PhysRevD.85.033007.
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
   3. ^van Mourik, T.; Buhl, M.; Gaigeot, M.-P. (10 February 2014). "Density
      functional_theory_across_chemistry,_physics_and_biology". Philosophical
      Transactions of the Royal Society A: Mathematical, Physical and
      Engineering Sciences. 372 (2011): 20120488â20120488. doi:10.1098/
      rsta.2012.0488. PMC 3928866. PMID 24516181.
   4. ^SchrÃ¶dinger, E. (1926). "Quantisierung als Eigenwertproblem"
      [Quantification of the eigen value problem]. Annalen der Physik (in
      German). 80 (13): 437â490. Bibcode:1926AnP...385..437S. doi:10.1002/
      andp.19263851302.
   5. ^Rayleigh, J. W. S. (1894). Theory of Sound. I (2nd ed.). London:
      Macmillan. pp. 115â118. ISBN 978-1-152-06023-4.
   6. ^Sulejmanpasic, Tin; Ãnsal, Mithat (2018-07-01). "Aspects of
      perturbation theory in quantum mechanics: The BenderWuMathematicaÂ®
      package". Computer Physics Communications. 228: 273â289. doi:10.1016/
      j.cpc.2017.11.018. ISSN 0010-4655.
   7. ^ Sakurai, J.J., and Napolitano, J. (1964,2011). Modern quantum mechanics
      (2nd ed.), Addison Wesley
   8. ISBN 978-0-8053-8291-4. Chapter 5
   9. ^Landau, L. D.; Lifschitz, E. M. (1977). Quantum Mechanics: Non-
      relativistic Theory (3rd ed.). ISBN 978-0-08-019012-9.
  10. ^Bir, GennadiÄ­ Levikovich; Pikus, GrigoriÄ­ Ezekielevich (1974).
      "Chapter_15:_Perturbation_theory_for_the_degenerate_case". Symmetry and
      Strain-induced Effects in Semiconductors. ISBN 978-0-470-07321-6.
  11. ^Soliverez, Carlos E. (1981). "General_Theory_of_Effective_Hamiltonians".
      Physical Review A. 24 (1): 4â9. Bibcode:1981PhRvA..24....4S. doi:
      10.1103/PhysRevA.24.4 – via Academia.Edu.
  12. ^ Albert_Messiah (1966). Quantum Mechanics, North Holland, John Wiley &
      Sons.
  13. ISBN 0486409244; J. J. Sakurai (1994). Modern Quantum Mechanics (Addison-
      Wesley)
  14. ISBN 9780201539295.
  15. ^Frasca, M. (1998). "Duality in Perturbation Theory and the Quantum
      Adiabatic Approximation". Physical Review A. 58 (5): 3439â3442. arXiv:
      hep-th/9801069. Bibcode:1998PhRvA..58.3439F. doi:10.1103/
      PhysRevA.58.3439.
  16. ^Mostafazadeh, A. (1997). "Quantum adiabatic approximation and the
      geometric phase". Physical Review A. 55 (3): 1653â1664. arXiv:hep-th/
      9606053. Bibcode:1997PhRvA..55.1653M. doi:10.1103/PhysRevA.55.1653.
  17. ^Frasca, Marco (2007). "A strongly perturbed quantum system is a
      semiclassical system". Proceedings of the Royal Society A: Mathematical,
      Physical and Engineering Sciences. 463 (2085): 2195â2200. arXiv:hep-th/
      0603182. Bibcode:2007RSPSA.463.2195F. doi:10.1098/rspa.2007.1879.

Retrieved from "https://en.wikipedia.org/w/index.php?title=Perturbation_theory_
(quantum_mechanics)&oldid=909771794"
Categories:
    * Perturbation_theory
    * Quantum_mechanics
    * Mathematical_physics
Hidden categories:
    * CS1_German-language_sources_(de)
    * Use_American_English_from_April_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * Wikipedia_articles_needing_clarification_from_April_2017
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_November_2018
    * Wikipedia_articles_needing_clarification_from_September_2016
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
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Bahasa_Melayu
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 14:18 (UTC).
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
