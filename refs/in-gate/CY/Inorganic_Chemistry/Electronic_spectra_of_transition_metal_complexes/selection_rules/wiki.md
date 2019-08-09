The following text has been accessed from https://en.wikipedia.org/wiki/Selection_rule at Fri Aug 9 02:07:31 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Selection rule ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In physics and chemistry, a selection rule, or transition rule, formally
constrains the possible transitions of a system from one quantum_state to
another. Selection rules have been derived for electromagnetic transitions in
molecules, in atoms, in atomic_nuclei, and so on. The selection rules may
differ according to the technique used to observe the transition. The selection
rule also plays a role in chemical_reactions, where some are formally spin
forbidden_reactions, that is, reactions where the spin state changes at least
once from reactants to products.
In the following, mainly atomic and molecular transitions are considered.
⁰
***** Contents *****
    * 1_Overview
    * 2_Examples
          o 2.1_Electronic_spectra
          o 2.2_Vibrational_spectra
          o 2.3_Rotational_spectra
          o 2.4_Coupled_transitions
          o 2.5_Angular_momentum
                # 2.5.1_Summary_table
          o 2.6_Surface
    * 3_See_also
    * 4_Notes
    * 5_References
    * 6_Further_reading
    * 7_External_links
***** Overview[edit] *****
In quantum_mechanics the basis for a spectroscopic selection rule is the value
of the transition moment integral[1]
         &#x222B;  &#x03C8;  1   &#x2217;   &#x03BC;  &#x03C8;  2   d &#x03C4;
      {\displaystyle \int \psi _{1}^{*}\mu \psi _{2}d\tau }  [\int \psi _{1}^
      {*}\mu \psi _{2}d\tau ],
where      &#x03C8;  1     {\displaystyle \psi _{1}}  [\psi _{1}] and
&#x03C8;  2     {\displaystyle \psi _{2}}  [\psi _{2}] are the wave_functions
of the two states involved in the transition and Âµ is the transition_moment
operator. This integral represents the propagator (and thus the probability) of
the transition between states; therefore if the value of this integral is zero
the transition is forbidden. In practice, the integral itself does not need to
be calculated to determine a selection rule. It is sufficient to determine the
symmetry of transition moment function,      &#x03C8;  1   &#x2217;   &#x03BC;
&#x03C8;  2   .   {\displaystyle \psi _{1}^{*}\mu \psi _{2}.}  [{\displaystyle
\psi _{1}^{*}\mu \psi _{2}.}] If the symmetry of this function spans the
totally symmetric representation of the point_group to which the atom or
molecule belongs then its value is (in general) not zero and the transition is
allowed. Otherwise, the transition is forbidden.
The transition moment integral is zero if the transition moment function,
&#x03C8;  1   &#x2217;   &#x03BC;  &#x03C8;  2     {\displaystyle \psi _{1}^
{*}\mu \psi _{2}}  [\psi _{1}^{*}\mu \psi _{2}], is anti-symmetric or odd, i.e.
y ( x ) = &#x2212; y ( &#x2212; x )   {\displaystyle y(x)=-y(-x)}  [
{\displaystyle y(x)=-y(-x)}] holds. The symmetry of the transition moment
function is the direct_product of the parities of its three components. The
symmetry characteristics of each component can be obtained from standard
character_tables. Rules for obtaining the symmetries of a direct product can be
found in texts on character tables. [2]
 ________Symmetry_characteristics_of_transition_moment_operator[2]_________
|Transition_type________|Âµ_transforms_as____|note_______________________|
|Electric_dipole________|x,_y,_z_______________|Optical_spectra____________|
|Electric_quadrupole____|x2,_y2,_z2,_xy,_xz,_yz|Constraint_x2_+_y2_+_z2_=_0|
|Electric_polarizability|x2,_y2,_z2,_xy,_xz,_yz|Raman_spectra______________|
|Magnetic_dipole________|Rx,_Ry,_Rz____________|Optical_spectra_(weak)_____|
***** Examples[edit] *****
**** Electronic spectra[edit] ****
The Laporte_rule is a selection rule formally stated as follows: In a
centrosymmetric environment, transitions between like atomic_orbitals such as
s-s, p-p, d-d, or f-f, transitions are forbidden. The Laporte rule applies to
electric_dipole_transitions, so the operator has u symmetry (meaning ungerade,
odd).[3] p orbitals also have u symmetry, so the symmetry of the transition
moment function is given by the triple_product u×u×u, which has u symmetry. The
transitions are therefore forbidden. Likewise, d orbitals have g symmetry
(meaning gerade, even), so the triple product g×u×g also has u symmetry and the
transition is forbidden.[4]
The wave function of a single electron is the product of a space-dependent wave
function and a spin wave function. Spin is directional and can be said to have
odd parity. It follows that transitions in which the spin "direction" changes
are forbidden. In formal terms, only states with the same total spin_quantum
number are "spin-allowed".[5] In crystal_field_theory, d-d transitions that are
spin-forbidden are much weaker than spin-allowed transitions. Both can be
observed, in spite of the Laporte rule, because the actual transitions are
coupled to vibrations that are anti-symmetric and have the same symmetry as the
dipole moment operator.[6]
**** Vibrational spectra[edit] ****
Main articles: infrared_spectroscopy and Raman_spectroscopy
In vibrational spectroscopy, transitions are observed between different
vibrational_states. In a fundamental vibration, the molecule is excited from
its ground_state (v = 0) to the first excited state (v = 1). The symmetry of
the ground-state wave function is the same as that of the molecule. It is,
therefore, a basis for the totally symmetric representation in the point_group
of the molecule. It follows that, for a vibrational transition to be allowed,
the symmetry of the excited state wave function must be the same as the
symmetry of the transition moment operator.[7]
In infrared_spectroscopy, the transition moment operator transforms as either x
and/or y and/or z. The excited state wave function must also transform as at
least one of these vectors. In Raman_spectroscopy, the operator transforms as
one of the second-order terms in the right-most column of the character table,
below.[2]
            Character table for the Td point group
   E 8 C3 3 C2 6 S4 6 Ïd
A1 1 1    1    1    1                  x2 + y2 + z2
A2 1 1    1    -1   -1
E  2 -1   2    0    0                  (2 z2 - x2 - y2,x2 - y2)
T1 3 0    -1   1    -1    (Rx, Ry, Rz)
T2 3 0    -1   -1   1     (x, y, z)    (xy, xz, yz)
The molecule methane, CH4, may be used as an example to illustrate the
application of these principles. The molecule is tetrahedral and has Td
symmetry. The vibrations of methane span the representations A1 + E + 2T2.[8]
Examination of the character table shows that all four vibrations are Raman-
active, but only the T2 vibrations can be seen in the infrared spectrum.[9]
In the harmonic_approximation, it can be shown that overtones are forbidden in
both infrared and Raman spectra. However, when anharmonicity is taken into
account, the transitions are weakly allowed.[10]
**** Rotational spectra[edit] ****
Main article: Rigid_rotor
The selection_rule for rotational transitions, derived from the symmetries of
the rotational wave functions in a rigid rotor, is ÎJ = Â±1, where J is a
rotational quantum number.[11]
**** Coupled transitions[edit] ****
Coupling_in_science
Classical coupling
    * Rotationalâvibrational_coupling
Quantum_coupling
    * Quantum-mechanical_coupling
    * Roâvibrational_spectroscopy
    * Vibronic_coupling
    * Rovibronic_coupling
    * Angular_momentum_coupling
    * NMR_coupling or J-coupling
    * v
    * t
    * e
The infrared spectrum of HCl gas
There are many types of coupled transition such as are observed in vibration-
rotation spectra. The excited-state wave function is the product of two wave
functions such as vibrational and rotational. The general principle is that the
symmetry of the excited state is obtained as the direct product of the
symmetries of the component wave functions.[12] In rovibronic transitions, the
excited states involve three wave functions.
The infrared spectrum of hydrogen_chloride gas shows rotational fine structure
superimposed on the vibrational spectrum. This is typical of the infrared
spectra of heteronuclear diatomic molecules. It shows the so-called P and R
branches. The Q branch, located at the vibration frequency, is absent.
Symmetric_top molecules display the Q branch. This follows from the application
of selection rules.[13]
Resonance_Raman_spectroscopy involves a kind of vibronic coupling. It results
in much-increased intensity of fundamental and overtone transitions as the
vibrations "steal" intensity from an allowed electronic transition.[14] In
spite of appearances, the selection rules are the same as in Raman
spectroscopy.[15]
**** Angular momentum[edit] ****
      See also angular_momentum_coupling
In general, electric (charge) radiation or magnetic (current, magnetic moment)
radiation can be classified into multipoles EÎ» (electric) or MÎ» (magnetic) of
order 2Î», e.g., E1 for electric dipole, E2 for quadrupole, or E3 for octupole.
In transitions where the change in angular momentum between the initial and
final states makes several multipole radiations possible, usually the lowest-
order multipoles are overwhelmingly more likely, and dominate the transition.
[16]
The emitted particle carries away an angular momentum Î», which for the photon
must be at least 1, since it is a vector particle (i.e., it has JP = 1â).
Thus, there is no E0 (electric monopoles) or M0 (magnetic_monopoles, which do
not seem to exist) radiation.
Since the total angular momentum has to be conserved during the transition, we
have that
           J    i    =   J    f    +  &#x03BB;    {\displaystyle \mathbf {J} _
      {\mathrm {i} }=\mathbf {J} _{\mathrm {f} }+{\boldsymbol {\lambda }}}  [
      {\mathbf  J}_{{{\mathrm  {i}}}}={\mathbf  {J}}_{{{\mathrm  {f}}}}+
      {\boldsymbol  {\lambda }}]
where     &#x2016;  &#x03BB;  &#x2016; =   &#x03BB; ( &#x03BB; + 1 )
&#x210F;   {\displaystyle \Vert {\boldsymbol {\lambda }}\Vert ={\sqrt {\lambda
(\lambda +1)}}\,\hbar }  [\Vert {\boldsymbol  {\lambda }}\Vert ={\sqrt
{\lambda (\lambda +1)}}\,\hbar ], and its z-projection is given by
&#x03BB;  z   = &#x03BC;  &#x210F;   {\displaystyle \lambda _{z}=\mu \,\hbar }
[\lambda _{z}=\mu \,\hbar ];       J    i      {\displaystyle \mathbf {J} _
{\mathrm {i} }}  [{\mathbf  J}_{{{\mathrm  {i}}}}] and       J    f
{\displaystyle \mathbf {J} _{\mathrm {f} }}  [{\mathbf  J}_{{{\mathrm  {f}}}}]
are, respectively, the initial and final angular momenta of the atom. The
corresponding quantum numbers Î» and Î¼ (z-axis angular momentum) must satisfy
          |   J   i    &#x2212;  J   f     |  &#x2264; &#x03BB; &#x2264;  J   i
      +  J   f      {\displaystyle |J_{\mathrm {i} }-J_{\mathrm {f} }|\leq
      \lambda \leq J_{\mathrm {i} }+J_{\mathrm {f} }}  [|J_{{{\mathrm  {i}}}}-
      J_{{{\mathrm  {f}}}}|\leq \lambda \leq J_{{{\mathrm  {i}}}}+J_{{{\mathrm
      {f}}}}]
and
         &#x03BC; =  M   i    &#x2212;  M   f     .   {\displaystyle \mu =M_
      {\mbox{i}}-M_{\mbox{f}}\,.}  [\mu =M_{{{\mbox{i}}}}-M_{{{\mbox{f}}}}\,.]
Parity is also preserved. For electric multipole transitions
         &#x03C0; (  E  &#x03BB; ) =  &#x03C0;   i     &#x03C0;   f    =
      ( &#x2212; 1  )  &#x03BB;      {\displaystyle \pi (\mathrm {E} \lambda
      )=\pi _{\mathrm {i} }\pi _{\mathrm {f} }=(-1)^{\lambda }\,}  [\pi (
      {\mathrm  {E}}\lambda )=\pi _{{{\mathrm  {i}}}}\pi _{{{\mathrm  {f}}}}=(-
      1)^{{\lambda }}\,]
while for magnetic multipoles
         &#x03C0; (  M  &#x03BB; ) =  &#x03C0;   i     &#x03C0;   f    =
      ( &#x2212; 1  )  &#x03BB; + 1    .   {\displaystyle \pi (\mathrm {M}
      \lambda )=\pi _{\mathrm {i} }\pi _{\mathrm {f} }=(-1)^{\lambda +1}\,.}
      [\pi ({\mathrm  {M}}\lambda )=\pi _{{{\mathrm  {i}}}}\pi _{{{\mathrm
      {f}}}}=(-1)^{{\lambda +1}}\,.]
Thus, parity does not change for E-even or M-odd multipoles, while it changes
for E-odd or M-even multipoles.
These considerations generate different sets of transitions rules depending on
the multipole order and type. The expression forbidden_transitions is often
used; this does not mean that these transitions cannot occur, only that they
are electric-dipole-forbidden. These transitions are perfectly possible; they
merely occur at a lower rate. If the rate for an E1 transition is non-zero, the
transition is said to be permitted; if it is zero, then M1, E2, etc.
transitions can still produce radiation, albeit with much lower transitions
rates. These are the so-called forbidden transitions. The transition rate
decreases by a factor of about 1000 from one multipole to the next one, so the
lowest multipole transitions are most likely to occur.[17]
Semi-forbidden transitions (resulting in so-called intercombination lines) are
electric dipole (E1) transitions for which the selection rule that the spin
does not change is violated. This is a result of the failure of LS_coupling.
*** Summary table[edit] ***
   J = L + S   {\displaystyle J=L+S}  [J=L+S] is the total angular momentum,
L   {\displaystyle L}  [L] is the Azimuthal_quantum_number,     S
{\displaystyle S}  [S] is the Spin_quantum_number, and      M  J
{\displaystyle M_{J}}  [M_{J}] is the secondary_total_angular_momentum_quantum
number. Which transitions are allowed is based on the Hydrogen-like_atom. The
symbol     &#x21AE;   {\displaystyle \not \leftrightarrow }  [\not
\leftrightarrow ] is used to indicate a forbidden transition.
Allowed          Electric dipole Magnetic       Electric        Magnetic        Electric        Magnetic
transitions      (E1)            dipole (M1)    quadrupole (E2) quadrupole (M2) octupole (E3)   octupole (M3)
                                                                                       &#x0394; J = 0 ,
                                                                                &#x00B1; 1 , &#x00B1; 2 ,
                                                                                &#x00B1; 3     ( 0 &#x21AE; 0 ,
                                                                                1 , 2 ; &#xA0;       1 2
                                                       &#x0394; J = 0 ,         &#x21AE;       1 2       ,
                                                &#x00B1; 1 , &#x00B1; 2     ( J 3 2       ; &#xA0; 1 &#x21AE; 1
                                                = 0 &#x21AE; 0 , 1 ; &#xA0;     )       {\displaystyle {\begin
                                                1 2       &#x21AE;       1 2    {matrix}\Delta J=0,\pm 1,\pm
                        &#x0394; J = 0 ,        )       {\displaystyle {\begin  2,\pm 3\\(0\not \leftrightarrow
                 &#x00B1; 1     ( J = 0         {matrix}\Delta J=0,\pm 1,\pm    0,1,2;\ {\begin{matrix}{1 \over
                 &#x21AE; 0 )                   2\\(J=0\not \leftrightarrow     2}\end{matrix}}\not
                 {\displaystyle {\begin         0,1;\ {\begin{matrix}{1 \over   \leftrightarrow {\begin{matrix}
                 {matrix}\Delta J=0,\pm 1\\     2}\end{matrix}}\not             {1 \over 2}\end{matrix}},
             (1) (J=0\not \leftrightarrow       \leftrightarrow {\begin{matrix} {\begin{matrix}{3 \over 2}\end
                 0)\end{matrix}}}  [{\begin     {1 \over 2}\end{matrix}})\end   {matrix}};\ 1\not
                 {matrix}\Delta J=0,\pm 1\\     {matrix}}}  [{\begin            \leftrightarrow 1)\end
                 (J=0\not \leftrightarrow       {matrix}\Delta J=0,\pm 1,\pm    {matrix}}}  [{\begin
                 0)\end{matrix}}]               2\\(J=0\not \leftrightarrow     {matrix}\Delta J=0,\pm 1,\pm
                                                0,1;\ {\begin{matrix}{1 \over   2,\pm 3\\(0\not \leftrightarrow
                                                2}\end{matrix}}\not             0,1,2;\ {\begin{matrix}{1 \over
                                                \leftrightarrow {\begin{matrix} 2}\end{matrix}}\not
Rigorous                                        {1 \over 2}\end{matrix}})\end   \leftrightarrow {\begin{matrix}
rules                                           {matrix}}]                      {1 \over 2}\end{matrix}},
                                                                                {\begin{matrix}{3 \over 2}\end
                                                                                {matrix}};\ 1\not
                                                                                \leftrightarrow 1)\end
                                                                                {matrix}}]
                                                   &#x0394;  M  J   = 0 ,          &#x0394;  M  J   = 0 ,
                    &#x0394;  M  J   = 0 ,      &#x00B1; 1 , &#x00B1; 2         &#x00B1; 1 , &#x00B1; 2 ,
             (2) &#x00B1; 1   {\displaystyle    {\displaystyle \Delta M_        &#x00B1; 3   {\displaystyle
                 \Delta M_{J}=0,\pm 1}  [\Delta {J}=0,\pm 1,\pm 2}  [\Delta M_  \Delta M_{J}=0,\pm 1,\pm 2,\pm
                 M_{J}=0,\pm 1]                 {J}=0,\pm 1,\pm 2]              3}  [\Delta M_{J}=0,\pm 1,\pm
                                                                                2,\pm 3]
                     &#x03C0;                                                                       &#x03C0;
                 f    = &#x2212;                                                                f    =
                 &#x03C0;   i                                                                   &#x03C0;   i
                 {\displaystyle      &#x03C0;   f    =              &#x03C0;   f    = &#x2212;  {\displaystyle
                 \pi _{\mathrm   &#x03C0;   i                   &#x03C0;   i                    \pi _{\mathrm
             (3) {f} }=-\pi _    {\displaystyle \pi _{\mathrm   {\displaystyle \pi _{\mathrm    {f} }=\pi _
                 {\mathrm {i}    {f} }=\pi _{\mathrm {i} }\,}   {f} }=-\pi _{\mathrm {i} }\,}   {\mathrm {i}
                 }\,}  [\pi _{{  [\pi _{{{\mathrm  {f}}}}=\pi _ [\pi _{{{\mathrm  {f}}}}=-\pi _ }\,}  [\pi _{{
                 {\mathrm        {{{\mathrm  {i}}}}\,]          {{{\mathrm  {i}}}}\,]           {\mathrm
                 {f}}}}=-\pi _{{                                                                {f}}}}=\pi _{{
                 {\mathrm                                                                       {\mathrm
                 {i}}}}\,]                                                                      {i}}}}\,]
                                 No electron
                                 jump                                           One electron
                 One electron                   None or one     One electron    jump            One electron
                 jump               &#x0394; L  electron jump   jump                            jump
                                 = 0                                               &#x0394; L =
                    &#x0394; L = {\displaystyle    &#x0394; L =    &#x0394; L = &#x00B1; 1 ,       &#x0394; L =
                 &#x00B1; 1      \Delta L=0}  [ 0 , &#x00B1; 2  &#x00B1; 1      &#x00B1; 3      0 , &#x00B1; 2
             (4) {\displaystyle  {\displaystyle {\displaystyle  {\displaystyle  {\displaystyle  {\displaystyle
                 \Delta L=\pm 1} \Delta L=0}],  \Delta L=0,\pm  \Delta L=\pm 1} \Delta L=\pm    \Delta L=0,\pm
                 [{\displaystyle    &#x0394; n  2}  [           [{\displaystyle 1,\pm 3}  [     2}  [
                 \Delta L=\pm    = 0            {\displaystyle  \Delta L=\pm    {\displaystyle  {\displaystyle
                 1}]             {\displaystyle \Delta L=0,\pm  1}]             \Delta L=\pm    \Delta L=0,\pm
                                 \Delta n=0}  [ 2}]                             1,\pm 3}]       2}]
                                 {\displaystyle
                                 \Delta n=0}]
                 If     &#x0394;
                 S = 0
                 {\displaystyle
                 \Delta S=0}  [
                 {\displaystyle                                                 If     &#x0394; S = 0
LS coupling      \Delta S=0}]                                                   {\displaystyle \Delta S=0}  [
                                                If     &#x0394; S = 0           {\displaystyle \Delta S=0}]
                        &#x0394; If             {\displaystyle \Delta S=0}  [
                 L = 0 ,         &#x0394; S = 0 {\displaystyle \Delta S=0}]            &#x0394; L = 0 ,
                 &#x00B1; 1      {\displaystyle                                 &#x00B1; 1 , &#x00B1; 2 ,
                 ( L = 0         \Delta S=0}  [        &#x0394; L = 0 ,         &#x00B1; 3     ( L = 0 &#x21AE;
                 &#x21AE; 0 )    {\displaystyle &#x00B1; 1 , &#x00B1; 2     ( L 0 , 1 , 2 ; &#xA0; 1 &#x21AE; 1
                 {\displaystyle  \Delta S=0}]   = 0 &#x21AE; 0 , 1 )            )       {\displaystyle {\begin
             (5) {\begin                        {\displaystyle {\begin          {matrix}\Delta L=0,\pm 1,\pm
                 {matrix}\Delta     &#x0394; L  {matrix}\Delta L=0,\pm 1,\pm    2,\pm 3\\(L=0\not
                 L=0,\pm 1\\     = 0            2\\(L=0\not \leftrightarrow     \leftrightarrow 0,1,2;\ 1\not
                 (L=0\not        {\displaystyle 0,1)\end{matrix}}}  [{\begin    \leftrightarrow 1)\end
                 \leftrightarrow \Delta L=0\,}  {matrix}\Delta L=0,\pm 1,\pm    {matrix}}}  [{\begin
                 0)\end          [\Delta L=0\,] 2\\(L=0\not \leftrightarrow     {matrix}\Delta L=0,\pm 1,\pm
                 {matrix}}}  [                  0,1)\end{matrix}}]              2,\pm 3\\(L=0\not
                 {\begin                                                        \leftrightarrow 0,1,2;\ 1\not
                 {matrix}\Delta                                                 \leftrightarrow 1)\end
                 L=0,\pm 1\\                                                    {matrix}}]
                 (L=0\not
                 \leftrightarrow
                 0)\end
                 {matrix}}]
                                                                                If     &#x0394;
                                                If     &#x0394;                 S = &#x00B1; 1
                                                S = &#x00B1; 1                  {\displaystyle  If     &#x0394;
                                                {\displaystyle  If     &#x0394; \Delta S=\pm 1} S = &#x00B1; 1
                                                \Delta S=\pm 1} S = &#x00B1; 1  [{\displaystyle {\displaystyle
                                                [{\displaystyle {\displaystyle  \Delta S=\pm    \Delta S=\pm 1}
                                                \Delta S=\pm    \Delta S=\pm 1} 1}]             [{\displaystyle
                                                1}]             [{\displaystyle                 \Delta S=\pm
                                                                \Delta S=\pm           &#x0394; 1}]
                                                       &#x0394; 1}]             L = 0 ,
                                                L = 0 ,                         &#x00B1; 1 ,           &#x0394;
                                                &#x00B1; 1 ,           &#x0394; &#x00B1; 2 ,    L = 0 ,
                 If     &#x0394; S = &#x00B1; 1 &#x00B1; 2 ,    L = 0 ,         &#x00B1; 3 ,    &#x00B1; 1 ,
                 {\displaystyle \Delta S=\pm 1} &#x00B1; 3      &#x00B1; 1      &#x00B1; 4      &#x00B1; 2
                 [{\displaystyle \Delta S=\pm   ( L = 0         ( L = 0         ( L = 0         ( L = 0
                 1}]                            &#x21AE; 0 )    &#x21AE; 0 )    &#x21AE; 0 , 1  &#x21AE; 0 )
Intermediate (6)                                {\displaystyle  {\displaystyle  )               {\displaystyle
coupling            &#x0394; L = 0 , &#x00B1; 1 {\begin         {\begin         {\displaystyle  {\begin
                 , &#x00B1; 2    {\displaystyle {matrix}\Delta  {matrix}\Delta  {\begin         {matrix}\Delta
                 \Delta L=0,\pm 1,\pm 2\,}      L=0,\pm 1,\\\pm L=0,\pm 1\\     {matrix}\Delta  L=0,\pm 1,\\\pm
                 [\Delta L=0,\pm 1,\pm 2\,]     2,\pm 3\\       (L=0\not        L=0,\pm 1,\\\pm 2\\(L=0\not
                                                (L=0\not        \leftrightarrow 2,\pm 3,\pm 4\\ \leftrightarrow
                                                \leftrightarrow 0)\end          (L=0\not        0)\end
                                                0)\end          {matrix}}}  [   \leftrightarrow {matrix}}}  [
                                                {matrix}}}  [   {\begin         0,1)\end        {\begin
                                                {\begin         {matrix}\Delta  {matrix}}}  [   {matrix}\Delta
                                                {matrix}\Delta  L=0,\pm 1\\     {\begin         L=0,\pm 1,\\\pm
                                                L=0,\pm 1,\\\pm (L=0\not        {matrix}\Delta  2\\(L=0\not
                                                2,\pm 3\\       \leftrightarrow L=0,\pm 1,\\\pm \leftrightarrow
                                                (L=0\not        0)\end          2,\pm 3,\pm 4\\ 0)\end
                                                \leftrightarrow {matrix}}]      (L=0\not        {matrix}}]
                                                0)\end                          \leftrightarrow
                                                {matrix}}]                      0,1)\end
                                                                                {matrix}}]
**** Surface[edit] ****
In surface_vibrational_spectroscopy, the surface selection rule is applied to
identify the peaks observed in vibrational spectra. When a molecule is adsorbed
on a substrate, the molecule induces opposite image charges in the substrate.
The dipole_moment of the molecule and the image charges perpendicular to the
surface reinforce each other. In contrast, the dipole moments of the molecule
and the image charges parallel to the surface cancel out. Therefore, only
molecular vibrational peaks giving rise to a dynamic dipole moment
perpendicular to the surface will be observed in the vibrational spectrum.
***** See also[edit] *****
    * Superselection_rule
    * Spin_forbidden_reactions
***** Notes[edit] *****
   1. ^ Harris & Bertolucci, p. 130
   2. ^ a b cSalthouse, J.A.; Ware, M.J. (1972). Point group character tables
      and related data. Cambridge_University_Press. ISBN 0-521-08139-4.
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
   4. ^ Anything with u (German ungerade) symmetry is antisymmetric with
      respect to the centre of symmetry. g (German gerade) signifies symmetric
      with respect to the centre of symmetry. If the transition moment function
      has u symmetry, the positive and negative parts will be equal to each
      other, so the integral has a value of zero.
   5. ^ Harris & Berolucci, p. 330
   6. ^ Harris & Berolucci, p. 336
   7. ^ Cotton Section 9.6, Selection rules and polarizations
   8. ^ Cotton, Section 10.6 Selection rules for fundamental vibrational
      transitions
   9. ^ Cotton, Chapter 10 Molecular Vibrations
  10. ^ Cotton p. 327
  11. ^Califano, S. (1976). Vibrational states. Wiley. ISBN 0-471-12996-8.
  12.  Chapter 9, Anharmonicity
  13. ^Kroto, H.W. (1992). Molecular Rotation Spectra. new York: Dover. ISBN 0-
      486-49540-X.
  14. ^ Harris & Berolucci, p. 339
  15. ^ Harris & Berolucci, p. 123
  16. ^Long, D.A. (2001). The Raman Effect: A Unified Treatment of the Theory
      of Raman Scattering by Molecules. Wiley. ISBN 0-471-49028-8.
  17.  Chapter 7, Vibrational Resonance Raman Scattering
  18. ^ Harris & Berolucci, p. 198
  19. ^Softley, T.P. (1994). Atomic Spectra. Oxford: Oxford_University_Press.
      ISBN 0-19-855688-8.
  20. ^Condon, E.V.; Shortley, G.H. (1953). The Theory of Atomic Spectra.
      Cambridge University Press. ISBN 0-521-09209-4.
***** References[edit] *****
Harris, D.C.; Bertolucci, M.D. (1978). Symmetry and Spectroscopy. Oxford
University Press. ISBN 0-19-855152-5.

Cotton, F.A. (1990). Chemical Applications of Group Theory (3rd ed.). Wiley.
ISBN 978-0-471-51094-9.
***** Further reading[edit] *****
    * Stanton, L. (1973). "Selection rules for pure rotation and vibration-
      rotation hyper-Raman spectra". Journal of Raman Spectroscopy. 1 (1):
      53â70. Bibcode:1973JRSp....1...53S. doi:10.1002/jrs.1250010105.
Bower, D.I; Maddams, W.F. (1989). The vibrational spectroscopy of polymers.
Cambridge University Press. ISBN 0-521-24633-4.
 Section 4.1.5: Selection rules for Raman activity.
Sherwood, P.M.A. (1972). Vibrational Spectroscopy of Solids. Cambridge
University Press. ISBN 0-521-08482-2.
 Chapter 4: The interaction of radiation with a crystal.
***** External links[edit] *****
    * National_Institute_of_Standards_and_Technology
    * University_of_Oxford_-_Lecture_Notes_-_Atomic_Physics_B1
    * Lecture_notes_from_The_University_of_Sheffield

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Selection_rule&oldid=896135854"
Categories:
    * Quantum_mechanics
    * Spectroscopy
    * Nuclear_magnetic_resonance
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * Deutsch
    * FranÃ§ais
    * Italiano
    * ×¢××¨××ª
    * æ¥æ¬èª
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 8 May 2019, at 14:32 (UTC).
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
