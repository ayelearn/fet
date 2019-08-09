The following text has been accessed from https://en.wikipedia.org/wiki/Maxwell_relations at Fri Aug 9 01:46:00 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Maxwell relations ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Thermodynamics
[Carnot_heat_engine_2.svg]
The classical Carnot_heat_engine
Branches
    * Classical
    * Statistical
    * Chemical
    * Quantum_thermodynamics
    * Equilibrium / Non-equilibrium
Laws
    * Zeroth
    * First
    * Second
    * Third
Systems
State
    * Equation_of_state
    * Ideal_gas
    * Real_gas
    * State_of_matter
    * Equilibrium
    * Control_volume
    * Instruments
Processes
    * Isobaric
    * Isochoric
    * Isothermal
    * Adiabatic
    * Isentropic
    * Isenthalpic
    * Quasistatic
    * Polytropic
    * Free_expansion
    * Reversibility
    * Irreversibility
    * Endoreversibility
Cycles
    * Heat_engines
    * Heat_pumps
    * Thermal_efficiency
System_properties
Note: Conjugate_variables in italics
    * Property_diagrams
    * Intensive_and_extensive_properties
Process_functions
    * Work
    * Heat
Functions_of_state
    * Temperature / Entropy (introduction)
    * Pressure / Volume
    * Chemical_potential / Particle_number
    * Vapor_quality
    * Reduced_properties
Material_properties
    * Property_databases
                                                     T              &#x2202; S
                                                  {\displaystyle {\displaystyle
                                                  T}  [T]        \partial S}
Specific_heat_capacity    c =   {\displaystyle                  [\partial S]
                        c=}  [c=]                    N              &#x2202; T
                                                  {\displaystyle {\displaystyle
                                                  N}  [N]        \partial T}
                                                                 [\partial T]
                                                     1              &#x2202; V
                                                  {\displaystyle {\displaystyle
                           &#x03B2; = &#x2212;    1}  [1]        \partial V}
Compressibility        {\displaystyle \beta =-                  [\partial V]
                        }  [\beta =-]                V              &#x2202; p
                                                  {\displaystyle {\displaystyle
                                                  V}  [V]        \partial p}
                                                                 [\partial p]
                                                     1              &#x2202; V
                                                  {\displaystyle {\displaystyle
                           &#x03B1; =             1}  [1]        \partial V}
Thermal_expansion      {\displaystyle \alpha =}                 [\partial V]
                        [\alpha =]                   V              &#x2202; T
                                                  {\displaystyle {\displaystyle
                                                  V}  [V]        \partial T}
                                                                 [\partial T]
Equations
    * Carnot's_theorem
    * Clausius_theorem
    * Fundamental_relation
    * Ideal_gas_law
    * Maxwell relations
    * Onsager_reciprocal_relations
    * Bridgman's_equations
    * Table_of_thermodynamic_equations
Potentials
    * Free_energy
    * Free_entropy
    * Internal_energy
         U ( S , V )   {\displaystyle U(S,V)}  [U(S,V)]
    * Enthalpy
         H ( S , p ) = U + p V   {\displaystyle H(S,p)=U+pV}  [H(S,p)=U+pV]
    * Helmholtz_free_energy
         A ( T , V ) = U &#x2212; T S   {\displaystyle A(T,V)=U-TS}  [A(T,V)=U-
      TS]
    * Gibbs_free_energy
         G ( T , p ) = H &#x2212; T S   {\displaystyle G(T,p)=H-TS}  [G(T,p)=H-
      TS]
    * History
    * Culture
History
    * General
    * Entropy
    * Gas_laws
    * "Perpetual_motion"_machines
Philosophy
    * Entropy_and_time
    * Entropy_and_life
    * Brownian_ratchet
    * Maxwell's_demon
    * Heat_death_paradox
    * Loschmidt's_paradox
    * Synergetics
Theories
    * Caloric_theory
    * Theory_of_heat
    * Vis_viva_("living_force")
    * Mechanical_equivalent_of_heat
    * Motive_power
Key_publications
    * "An_Experimental_Enquiry
      Concerning_..._Heat"
    * "On_the_Equilibrium_of
      Heterogeneous_Substances"
    * "Reflections_on_the
      Motive_Power_of_Fire"
Timelines
    * Thermodynamics
    * Heat_engines
    * Art
    * Education
    * Maxwell's_thermodynamic_surface
    * Entropy_as_energy_dispersal
Scientists
    * Bernoulli
    * Boltzmann
    * Carnot
    * Clapeyron
    * Clausius
    * CarathÃ©odory
    * Duhem
    * Gibbs
    * von_Helmholtz
    * Joule
    * Maxwell
    * von_Mayer
    * Onsager
    * Rankine
    * Smeaton
    * Stahl
    * Thompson
    * Thomson
    * van_der_Waals
    * Waterston
    * [Wikipedia book] Book
    * [Category] Category
    * v
    * t
    * e
For electromagnetic equations, see Maxwell's_equations.
Flow chart showing the paths between the Maxwell relations. P: pressure, T:
temperature, V: volume, S: entropy, Î±: coefficient_of_thermal_expansion, Îº:
compressibility, CV: heat_capacity at constant volume, CP: heat_capacity at
constant pressure.
Maxwell's relations are a set of equations in thermodynamics which are
derivable from the symmetry_of_second_derivatives and from the definitions of
the thermodynamic_potentials. These relations are named for the nineteenth-
century physicist James_Clerk_Maxwell.
⁰
***** Contents *****
    * 1_Equations
    * 2_The_four_most_common_Maxwell_relations
          o 2.1_Derivation
    * 3_Derivation_based_on_Jacobians
    * 4_General_Maxwell_relationships
    * 5_See_also
***** Equations[edit] *****
See also: symmetry_of_second_derivatives
The structure of Maxwell relations is a statement of equality among the second
derivatives for continuous functions. It follows directly from the fact that
the order of differentiation of an analytic_function of two variables is
irrelevant (Schwarz_theorem). In the case of Maxwell relations the function
considered is a thermodynamic potential and xi and xj are two different natural
variables for that potential:
Schwarz' theorem (general)
     &#x2202;  &#x2202;  x  j       (    &#x2202; &#x03A6;   &#x2202;  x  i
)  =   &#x2202;  &#x2202;  x  i       (    &#x2202; &#x03A6;   &#x2202;  x  j
)    {\displaystyle {\frac {\partial }{\partial x_{j}}}\left({\frac {\partial
\Phi }{\partial x_{i}}}\right)={\frac {\partial }{\partial x_{i}}}\left({\frac
{\partial \Phi }{\partial x_{j}}}\right)}  [\frac{\partial }{\partial x_j}\left
(\frac{\partial \Phi}{\partial x_i}\right)=
\frac{\partial }{\partial x_i}\left(\frac{\partial \Phi}{\partial x_j}\right)
]
where the partial_derivatives are taken with all other natural variables held
constant. It is seen that for every thermodynamic potential there are n(n â
1)/2 possible Maxwell relations where n is the number of natural variables for
that potential. The substantial increase in the entropy will be verified
according to the relations satisfied by the laws of thermodynamics
***** The four most common Maxwell relations[edit] *****
The four most common Maxwell relations are the equalities of the second
derivatives of each of the four thermodynamic potentials, with respect to their
thermal natural variable (temperature T; or entropy S) and their mechanical
natural variable (pressure P; or volume V):
Maxwell's relations (common)
       +   (    &#x2202; T   &#x2202; V    )   S      =   &#x2212;
(    &#x2202; P   &#x2202; S    )   V      =       &#x2202;  2   U   &#x2202; S
&#x2202; V        +   (    &#x2202; T   &#x2202; P    )   S      =   +
(    &#x2202; V   &#x2202; S    )   P      =       &#x2202;  2   H   &#x2202; S
&#x2202; P        +   (    &#x2202; S   &#x2202; V    )   T      =   +
(    &#x2202; P   &#x2202; T    )   V      =   &#x2212;     &#x2202;  2   F
&#x2202; T &#x2202; V        &#x2212;   (    &#x2202; S   &#x2202; P    )   T
=   +   (    &#x2202; V   &#x2202; T    )   P      =       &#x2202;  2   G
&#x2202; T &#x2202; P            {\displaystyle {\begin{aligned}+\left({\frac
{\partial T}{\partial V}}\right)_{S}&=&-\left({\frac {\partial P}{\partial
S}}\right)_{V}&=&{\frac {\partial ^{2}U}{\partial S\partial V}}\\+\left({\frac
{\partial T}{\partial P}}\right)_{S}&=&+\left({\frac {\partial V}{\partial
S}}\right)_{P}&=&{\frac {\partial ^{2}H}{\partial S\partial P}}\\+\left({\frac
{\partial S}{\partial V}}\right)_{T}&=&+\left({\frac {\partial P}{\partial
T}}\right)_{V}&=&-{\frac {\partial ^{2}F}{\partial T\partial V}}\\-\left({\frac
{\partial S}{\partial P}}\right)_{T}&=&+\left({\frac {\partial V}{\partial
T}}\right)_{P}&=&{\frac {\partial ^{2}G}{\partial T\partial P}}\end
{aligned}}\,\!}  [{\begin{aligned}+\left({\frac  {\partial T}{\partial
V}}\right)_{S}&=&-\left({\frac  {\partial P}{\partial S}}\right)_{V}&=&{\frac
{\partial ^{2}U}{\partial S\partial V}}\\+\left({\frac  {\partial T}{\partial
P}}\right)_{S}&=&+\left({\frac  {\partial V}{\partial S}}\right)_{P}&=&{\frac
{\partial ^{2}H}{\partial S\partial P}}\\+\left({\frac  {\partial S}{\partial
V}}\right)_{T}&=&+\left({\frac  {\partial P}{\partial T}}\right)_{V}&=&-{\frac
{\partial ^{2}F}{\partial T\partial V}}\\-\left({\frac  {\partial S}{\partial
P}}\right)_{T}&=&+\left({\frac  {\partial V}{\partial T}}\right)_{P}&=&{\frac
{\partial ^{2}G}{\partial T\partial P}}\end{aligned}}\,\!]
where the potentials as functions of their natural thermal and mechanical
variables are the internal_energy U(S, V), enthalpy H(S, P), Helmholtz_free
energy F(T, V) and Gibbs_free_energy G(T, P). The thermodynamic_square can be
used as a mnemonic to recall and derive these relations. The usefulness of
these relations lies in their quantifying entropy changes, which are not
directly measurable, in terms of measurable quantities like temperature,
volume, and pressure.
**** Derivation[edit] ****
Maxwell relations are based on simple partial differentiation rules, in
particular the total differential_of_a_function and the symmetry of evaluating
second order partial derivatives.
      Derivation
      Derivation of the Maxwell relation can be deduced from the differential
      forms of the thermodynamic_potentials:
      The differential form of internal energy U is
                   d U    = T d S &#x2212; P d V         {\displaystyle {\begin
            {aligned}dU&=TdS-PdV\\\end{aligned}}\,\!}  [{\displaystyle {\begin
            {aligned}dU&=TdS-PdV\\\end{aligned}}\,\!}]
      This equation resembles total_differentials of the form
               d z =   (    &#x2202; z   &#x2202; x    )   y    d x +
            (    &#x2202; z   &#x2202; y    )   x    d y   {\displaystyle
            dz=\left({\frac {\partial z}{\partial x}}\right)_{y}\!dx+\left(
            {\frac {\partial z}{\partial y}}\right)_{x}\!dy}  [dz = \left(\frac
            {\partial z}{\partial x}\right)_y\!dx +
             \left(\frac{\partial z}{\partial y}\right)_x\!dy]
      It can be shown that for any equation of the form
               d z = M d x + N d y    {\displaystyle dz=Mdx+Ndy\,}  [dz = Mdx +
            Ndy \,]
      that
               M =   (    &#x2202; z   &#x2202; x    )   y   ,  N =
            (    &#x2202; z   &#x2202; y    )   x     {\displaystyle M=\left(
            {\frac {\partial z}{\partial x}}\right)_{y},\quad N=\left({\frac
            {\partial z}{\partial y}}\right)_{x}}  [M = \left(\frac{\partial z}
            {\partial x}\right)_y, \quad
             N = \left(\frac{\partial z}{\partial y}\right)_x]
      Consider, the equation     d U = T d S &#x2212; P d V    {\displaystyle
      dU=TdS-PdV\,}  [dU=TdS-PdV\,]. We can now immediately see that
               T =   (    &#x2202; U   &#x2202; S    )   V   ,  &#x2212; P =
            (    &#x2202; U   &#x2202; V    )   S     {\displaystyle T=\left(
            {\frac {\partial U}{\partial S}}\right)_{V},\quad -P=\left({\frac
            {\partial U}{\partial V}}\right)_{S}}  [T = \left(\frac{\partial U}
            {\partial S}\right)_V, \quad
                   -P = \left(\frac{\partial U}{\partial V}\right)_S]
      Since we also know that for functions with continuous second derivatives,
      the mixed partial derivatives are identical (Symmetry_of_second
      derivatives), that is, that
                 &#x2202;  &#x2202; y      (    &#x2202; z   &#x2202; x    )
            y   =   &#x2202;  &#x2202; x      (    &#x2202; z   &#x2202; y    )
            x   =     &#x2202;  2   z   &#x2202; y &#x2202; x    =     &#x2202;
            2   z   &#x2202; x &#x2202; y      {\displaystyle {\frac {\partial
            }{\partial y}}\left({\frac {\partial z}{\partial x}}\right)_{y}=
            {\frac {\partial }{\partial x}}\left({\frac {\partial z}{\partial
            y}}\right)_{x}={\frac {\partial ^{2}z}{\partial y\partial x}}=
            {\frac {\partial ^{2}z}{\partial x\partial y}}}  [\frac{\partial}
            {\partial y}\left(\frac{\partial z}{\partial x}\right)_y =
            \frac{\partial}{\partial x}\left(\frac{\partial z}{\partial
            y}\right)_x =
            \frac{\partial^2 z}{\partial y \partial x} = \frac{\partial^2 z}
            {\partial x \partial y}]
      we therefore can see that
                 &#x2202;  &#x2202; V      (    &#x2202; U   &#x2202; S    )
            V   =   &#x2202;  &#x2202; S      (    &#x2202; U   &#x2202; V    )
            S     {\displaystyle {\frac {\partial }{\partial V}}\left({\frac
            {\partial U}{\partial S}}\right)_{V}={\frac {\partial }{\partial
            S}}\left({\frac {\partial U}{\partial V}}\right)_{S}}  [ \frac
            {\partial}{\partial V}\left(\frac{\partial U}{\partial S}\right)_V
            =
            \frac{\partial}{\partial S}\left(\frac{\partial U}{\partial
            V}\right)_S ]
      and therefore that
                 (    &#x2202; T   &#x2202; V    )   S   = &#x2212;
            (    &#x2202; P   &#x2202; S    )   V     {\displaystyle \left(
            {\frac {\partial T}{\partial V}}\right)_{S}=-\left({\frac {\partial
            P}{\partial S}}\right)_{V}}  [\left(\frac{\partial T}{\partial
            V}\right)_S = -\left(\frac{\partial P}{\partial S}\right)_V]
      Derivation of Maxwell Relation from Helmholtz Free energy
            The differential form of Helmholtz free energy is
                   d F    = &#x2212; S d T &#x2212; P d V
            {\displaystyle {\begin{aligned}dF&=-SdT-PdV\\\end{aligned}}\,\!}  [
            {\displaystyle {\begin{aligned}dF&=-SdT-PdV\\\end{aligned}}\,\!}]
               &#x2212; S =   (    &#x2202; F   &#x2202; T    )   V   ,
            &#x2212; P =   (    &#x2202; F   &#x2202; V    )   T
            {\displaystyle -S=\left({\frac {\partial F}{\partial T}}\right)_
            {V},\quad -P=\left({\frac {\partial F}{\partial V}}\right)_{T}}  [-
            S=\left({\frac  {\partial F}{\partial T}}\right)_{V},\quad -P=\left
            ({\frac  {\partial F}{\partial V}}\right)_{T}]
      From symmetry of second derivatives
                 &#x2202;  &#x2202; V      (    &#x2202; F   &#x2202; T    )
            V   =   &#x2202;  &#x2202; T      (    &#x2202; F   &#x2202; V    )
            T     {\displaystyle {\frac {\partial }{\partial V}}\left({\frac
            {\partial F}{\partial T}}\right)_{V}={\frac {\partial }{\partial
            T}}\left({\frac {\partial F}{\partial V}}\right)_{T}}  [{\frac
            {\partial }{\partial V}}\left({\frac  {\partial F}{\partial
            T}}\right)_{V}={\frac  {\partial }{\partial T}}\left({\frac
            {\partial F}{\partial V}}\right)_{T}]
      and therefore that
                 (    &#x2202; S   &#x2202; V    )   T   =   (    &#x2202; P
            &#x2202; T    )   V     {\displaystyle \left({\frac {\partial S}
            {\partial V}}\right)_{T}=\left({\frac {\partial P}{\partial
            T}}\right)_{V}}  [\left(\frac{\partial S}{\partial V}\right)_T =
            \left(\frac{\partial P}{\partial T}\right)_V]
      The other two Maxwell relations can be derived from differential form of
      enthalpy         d H    = T d S + V d P         {\displaystyle {\begin
      {aligned}dH&=TdS+VdP\\\end{aligned}}\,\!}  [{\displaystyle {\begin
      {aligned}dH&=TdS+VdP\\\end{aligned}}\,\!}] and the differential form of
      Gibbs free energy         d G    = V d P &#x2212; S d T
      {\displaystyle {\begin{aligned}dG&=VdP-SdT\\\end{aligned}}\,\!}  [
      {\displaystyle {\begin{aligned}dG&=VdP-SdT\\\end{aligned}}\,\!}] in a
      similar way. So all Maxwell Relationships above follow from one of the
      Gibbs_equations.
      Extended derivation
      Combined form first and second law of thermodynamics,
               T d S = d U + P d V   {\displaystyle TdS=dU+PdV}  [TdS = dU+PdV]
            (Eq.1)
      U, S, and V are state functions. Let,
               U = U ( x , y )   {\displaystyle U=U(x,y)}  [U = U(x,y)]
               S = S ( x , y )   {\displaystyle S=S(x,y)}  [S = S(x,y)]
               V = V ( x , y )   {\displaystyle V=V(x,y)}  [V = V(x,y)]
               d U =   (    &#x2202; U   &#x2202; x    )   y    d x +
            (    &#x2202; U   &#x2202; y    )   x    d y   {\displaystyle
            dU=\left({\frac {\partial U}{\partial x}}\right)_{y}\!dx+\left(
            {\frac {\partial U}{\partial y}}\right)_{x}\!dy}  [dU = \left(\frac
            {\partial U}{\partial x}\right)_y\!dx +
             \left(\frac{\partial U}{\partial y}\right)_x\!dy]
               d S =   (    &#x2202; S   &#x2202; x    )   y    d x +
            (    &#x2202; S   &#x2202; y    )   x    d y   {\displaystyle
            dS=\left({\frac {\partial S}{\partial x}}\right)_{y}\!dx+\left(
            {\frac {\partial S}{\partial y}}\right)_{x}\!dy}  [dS = \left(\frac
            {\partial S}{\partial x}\right)_y\!dx +
             \left(\frac{\partial S}{\partial y}\right)_x\!dy]
               d V =   (    &#x2202; V   &#x2202; x    )   y    d x +
            (    &#x2202; V   &#x2202; y    )   x    d y   {\displaystyle
            dV=\left({\frac {\partial V}{\partial x}}\right)_{y}\!dx+\left(
            {\frac {\partial V}{\partial y}}\right)_{x}\!dy}  [dV = \left(\frac
            {\partial V}{\partial x}\right)_y\!dx +
             \left(\frac{\partial V}{\partial y}\right)_x\!dy]
      Substitute them in Eq.1 and one gets,
               T   (    &#x2202; S   &#x2202; x    )   y    d x + T
            (    &#x2202; S   &#x2202; y    )   x    d y =   (    &#x2202; U
            &#x2202; x    )   y    d x +   (    &#x2202; U   &#x2202; y    )
            x    d y + P   (    &#x2202; V   &#x2202; x    )   y    d x + P
            (    &#x2202; V   &#x2202; y    )   x    d y   {\displaystyle
            T\left({\frac {\partial S}{\partial x}}\right)_{y}\!dx+T\left(
            {\frac {\partial S}{\partial y}}\right)_{x}\!dy=\left({\frac
            {\partial U}{\partial x}}\right)_{y}\!dx+\left({\frac {\partial U}
            {\partial y}}\right)_{x}\!dy+P\left({\frac {\partial V}{\partial
            x}}\right)_{y}\!dx+P\left({\frac {\partial V}{\partial y}}\right)_
            {x}\!dy}  [T\left(\frac{\partial S}{\partial x}\right)_y\!dx +
             T\left(\frac{\partial S}{\partial y}\right)_x\!dy = \left(\frac
            {\partial U}{\partial x}\right)_y\!dx +
             \left(\frac{\partial U}{\partial y}\right)_x\!dy + P\left(\frac
            {\partial V}{\partial x}\right)_y\!dx +
             P\left(\frac{\partial V}{\partial y}\right)_x\!dy]
      And also written as,
                 (    &#x2202; U   &#x2202; x    )   y    d x +   (    &#x2202;
            U   &#x2202; y    )   x    d y = T   (    &#x2202; S   &#x2202; x
            )   y    d x + T   (    &#x2202; S   &#x2202; y    )   x    d y
            &#x2212; P   (    &#x2202; V   &#x2202; x    )   y    d x &#x2212;
            P   (    &#x2202; V   &#x2202; y    )   x    d y   {\displaystyle
            \left({\frac {\partial U}{\partial x}}\right)_{y}\!dx+\left({\frac
            {\partial U}{\partial y}}\right)_{x}\!dy=T\left({\frac {\partial S}
            {\partial x}}\right)_{y}\!dx+T\left({\frac {\partial S}{\partial
            y}}\right)_{x}\!dy-P\left({\frac {\partial V}{\partial x}}\right)_
            {y}\!dx-P\left({\frac {\partial V}{\partial y}}\right)_{x}\!dy}
            [\left(\frac{\partial U}{\partial x}\right)_y\!dx +
             \left(\frac{\partial U}{\partial y}\right)_x\!dy = T\left(\frac
            {\partial S}{\partial x}\right)_y\!dx +
             T\left(\frac{\partial S}{\partial y}\right)_x\!dy - P\left(\frac
            {\partial V}{\partial x}\right)_y\!dx -
             P\left(\frac{\partial V}{\partial y}\right)_x\!dy]
      comparing the coefficient of dx and dy, one gets
                 (    &#x2202; U   &#x2202; x    )   y   = T   (    &#x2202; S
            &#x2202; x    )   y   &#x2212; P   (    &#x2202; V   &#x2202; x
            )   y     {\displaystyle \left({\frac {\partial U}{\partial
            x}}\right)_{y}=T\left({\frac {\partial S}{\partial x}}\right)_{y}-
            P\left({\frac {\partial V}{\partial x}}\right)_{y}}  [\left(\frac
            {\partial U}{\partial x}\right)_y = T\left(\frac{\partial S}
            {\partial x}\right)_y - P\left(\frac{\partial V}{\partial
            x}\right)_y]
                 (    &#x2202; U   &#x2202; y    )   x   = T   (    &#x2202; S
            &#x2202; y    )   x   &#x2212; P   (    &#x2202; V   &#x2202; y
            )   x     {\displaystyle \left({\frac {\partial U}{\partial
            y}}\right)_{x}=T\left({\frac {\partial S}{\partial y}}\right)_{x}-
            P\left({\frac {\partial V}{\partial y}}\right)_{x}}  [\left(\frac
            {\partial U}{\partial y}\right)_x = T\left(\frac{\partial S}
            {\partial y}\right)_x - P\left(\frac{\partial V}{\partial
            y}\right)_x]
      Differentiating above equations by y, x respectively
                (     &#x2202;  2   U   &#x2202; y &#x2202; x    )  =
            (    &#x2202; T   &#x2202; y    )   x     (    &#x2202; S
            &#x2202; x    )   y   + T  (     &#x2202;  2   S   &#x2202; y
            &#x2202; x    )  &#x2212;   (    &#x2202; P   &#x2202; y    )   x
            (    &#x2202; V   &#x2202; x    )   y   &#x2212; P  (     &#x2202;
            2   V   &#x2202; y &#x2202; x    )    {\displaystyle \left({\frac
            {\partial ^{2}U}{\partial y\partial x}}\right)=\left({\frac
            {\partial T}{\partial y}}\right)_{x}\left({\frac {\partial S}
            {\partial x}}\right)_{y}+T\left({\frac {\partial ^{2}S}{\partial
            y\partial x}}\right)-\left({\frac {\partial P}{\partial y}}\right)_
            {x}\left({\frac {\partial V}{\partial x}}\right)_{y}-P\left({\frac
            {\partial ^{2}V}{\partial y\partial x}}\right)}  [\left(\frac
            {\partial^2U}{\partial y\partial x}\right) = \left(\frac{\partial
            T}{\partial y}\right)_x \left(\frac{\partial S}{\partial
            x}\right)_y + T\left(\frac{\partial^2 S}{\partial y\partial
            x}\right) - \left(\frac{\partial P}{\partial y}\right)_x \left
            (\frac{\partial V}{\partial x}\right)_y - P\left(\frac{\partial^2
            V}{\partial y\partial x}\right)] (Eq.2)
            and
                (     &#x2202;  2   U   &#x2202; x &#x2202; y    )  =
            (    &#x2202; T   &#x2202; x    )   y     (    &#x2202; S
            &#x2202; y    )   x   + T  (     &#x2202;  2   S   &#x2202; x
            &#x2202; y    )  &#x2212;   (    &#x2202; P   &#x2202; x    )   y
            (    &#x2202; V   &#x2202; y    )   x   &#x2212; P  (     &#x2202;
            2   V   &#x2202; x &#x2202; y    )    {\displaystyle \left({\frac
            {\partial ^{2}U}{\partial x\partial y}}\right)=\left({\frac
            {\partial T}{\partial x}}\right)_{y}\left({\frac {\partial S}
            {\partial y}}\right)_{x}+T\left({\frac {\partial ^{2}S}{\partial
            x\partial y}}\right)-\left({\frac {\partial P}{\partial x}}\right)_
            {y}\left({\frac {\partial V}{\partial y}}\right)_{x}-P\left({\frac
            {\partial ^{2}V}{\partial x\partial y}}\right)}  [\left(\frac
            {\partial^2U}{\partial x\partial y}\right) = \left(\frac{\partial
            T}{\partial x}\right)_y \left(\frac{\partial S}{\partial
            y}\right)_x + T\left(\frac{\partial^2 S}{\partial x\partial
            y}\right) - \left(\frac{\partial P}{\partial x}\right)_y \left
            (\frac{\partial V}{\partial y}\right)_x - P\left(\frac{\partial^2
            V}{\partial x\partial y}\right)] (Eq.3)
      U, S, and V are exact differentials, therefore,
                (     &#x2202;  2   U   &#x2202; y &#x2202; x    )  =
            (     &#x2202;  2   U   &#x2202; x &#x2202; y    )
            {\displaystyle \left({\frac {\partial ^{2}U}{\partial y\partial
            x}}\right)=\left({\frac {\partial ^{2}U}{\partial x\partial
            y}}\right)}  [\left(\frac{\partial^2U}{\partial y\partial x}\right)
            = \left(\frac{\partial^2U}{\partial x\partial y}\right)]
                (     &#x2202;  2   S   &#x2202; y &#x2202; x    )  =
            (     &#x2202;  2   S   &#x2202; x &#x2202; y    )
            {\displaystyle \left({\frac {\partial ^{2}S}{\partial y\partial
            x}}\right)=\left({\frac {\partial ^{2}S}{\partial x\partial
            y}}\right)}  [{\displaystyle \left({\frac {\partial ^{2}S}{\partial
            y\partial x}}\right)=\left({\frac {\partial ^{2}S}{\partial
            x\partial y}}\right)}]
                (     &#x2202;  2   V   &#x2202; y &#x2202; x    )  =
            (     &#x2202;  2   V   &#x2202; x &#x2202; y    )
            {\displaystyle \left({\frac {\partial ^{2}V}{\partial y\partial
            x}}\right)=\left({\frac {\partial ^{2}V}{\partial x\partial
            y}}\right)}  [{\displaystyle \left({\frac {\partial ^{2}V}{\partial
            y\partial x}}\right)=\left({\frac {\partial ^{2}V}{\partial
            x\partial y}}\right)}]
      Subtract eqn(2) and (3) and one gets
                 (    &#x2202; T   &#x2202; y    )   x     (    &#x2202; S
            &#x2202; x    )   y   &#x2212;   (    &#x2202; P   &#x2202; y    )
            x     (    &#x2202; V   &#x2202; x    )   y   =   (    &#x2202; T
            &#x2202; x    )   y     (    &#x2202; S   &#x2202; y    )   x
            &#x2212;   (    &#x2202; P   &#x2202; x    )   y     (    &#x2202;
            V   &#x2202; y    )   x     {\displaystyle \left({\frac {\partial
            T}{\partial y}}\right)_{x}\left({\frac {\partial S}{\partial
            x}}\right)_{y}-\left({\frac {\partial P}{\partial y}}\right)_
            {x}\left({\frac {\partial V}{\partial x}}\right)_{y}=\left({\frac
            {\partial T}{\partial x}}\right)_{y}\left({\frac {\partial S}
            {\partial y}}\right)_{x}-\left({\frac {\partial P}{\partial
            x}}\right)_{y}\left({\frac {\partial V}{\partial y}}\right)_{x}}
            [\left(\frac{\partial T}{\partial y}\right)_x \left(\frac{\partial
            S}{\partial x}\right)_y - \left(\frac{\partial P}{\partial
            y}\right)_x \left(\frac{\partial V}{\partial x}\right)_y = \left
            (\frac{\partial T}{\partial x}\right)_y \left(\frac{\partial S}
            {\partial y}\right)_x - \left(\frac{\partial P}{\partial
            x}\right)_y \left(\frac{\partial V}{\partial y}\right)_x]
            Note: The above is called the general expression for Maxwell's
            thermodynamical relation.
        Maxwell's first relation
            Allow x = S and y = V and one gets
                 (    &#x2202; T   &#x2202; V    )   S   = &#x2212;
            (    &#x2202; P   &#x2202; S    )   V     {\displaystyle \left(
            {\frac {\partial T}{\partial V}}\right)_{S}=-\left({\frac {\partial
            P}{\partial S}}\right)_{V}}  [\left(\frac{\partial T}{\partial
            V}\right)_S = -\left(\frac{\partial P}{\partial S}\right)_V]
        Maxwell's second relation
            Allow x = T and y = V and one gets
                 (    &#x2202; S   &#x2202; V    )   T   =   (    &#x2202; P
            &#x2202; T    )   V     {\displaystyle \left({\frac {\partial S}
            {\partial V}}\right)_{T}=\left({\frac {\partial P}{\partial
            T}}\right)_{V}}  [\left(\frac{\partial S}{\partial V}\right)_T =
            \left(\frac{\partial P}{\partial T}\right)_V]
        Maxwell's third relation
            Allow x = S and y = P and one gets
                 (    &#x2202; T   &#x2202; P    )   S   =   (    &#x2202; V
            &#x2202; S    )   P     {\displaystyle \left({\frac {\partial T}
            {\partial P}}\right)_{S}=\left({\frac {\partial V}{\partial
            S}}\right)_{P}}  [\left(\frac{\partial T}{\partial P}\right)_S =
            \left(\frac{\partial V}{\partial S}\right)_P]
        Maxwell's fourth relation
            Allow x = T and y = P and one gets
                 (    &#x2202; S   &#x2202; P    )   T   = &#x2212;
            (    &#x2202; V   &#x2202; T    )   P     {\displaystyle \left(
            {\frac {\partial S}{\partial P}}\right)_{T}=-\left({\frac {\partial
            V}{\partial T}}\right)_{P}}  [\left(\frac{\partial S}{\partial
            P}\right)_T = -\left(\frac{\partial V}{\partial T}\right)_P]
        Maxwell's fifth relation
            Allow x = P and y = V
                 (    &#x2202; T   &#x2202; P    )   V     (    &#x2202; S
            &#x2202; V    )   P     {\displaystyle \left({\frac {\partial T}
            {\partial P}}\right)_{V}\left({\frac {\partial S}{\partial
            V}}\right)_{P}}  [\left(\frac{\partial T}{\partial P}\right)_V
            \left(\frac{\partial S}{\partial V}\right)_P]    &#x2212;
            (    &#x2202; T   &#x2202; V    )   P     (    &#x2202; S
            &#x2202; P    )   V     {\displaystyle -\left({\frac {\partial T}
            {\partial V}}\right)_{P}\left({\frac {\partial S}{\partial
            P}}\right)_{V}}  [-\left(\frac{\partial T}{\partial V}\right)_P
            \left(\frac{\partial S}{\partial P}\right)_V] = 1
        Maxwell's sixth relation
            Allow x = T and y = S and one gets
                 (    &#x2202; P   &#x2202; T    )   S     (    &#x2202; V
            &#x2202; S    )   T   &#x2212;   (    &#x2202; P   &#x2202; S    )
            T     (    &#x2202; V   &#x2202; T    )   S     {\displaystyle
            \left({\frac {\partial P}{\partial T}}\right)_{S}\left({\frac
            {\partial V}{\partial S}}\right)_{T}-\left({\frac {\partial P}
            {\partial S}}\right)_{T}\left({\frac {\partial V}{\partial
            T}}\right)_{S}}  [\left(\frac{\partial P}{\partial T}\right)_S
            \left(\frac{\partial V}{\partial S}\right)_T -\left(\frac{\partial
            P}{\partial S}\right)_T \left(\frac{\partial V}{\partial
            T}\right)_S] = 1
***** Derivation based on Jacobians[edit] *****
If we view the first law of thermodynamics,
             d U    = T d S &#x2212; P d V         {\displaystyle {\begin
      {aligned}dU&=TdS-PdV\\\end{aligned}}\,\!}  [{\displaystyle {\begin
      {aligned}dU&=TdS-PdV\\\end{aligned}}\,\!}]
as a statement about differential forms, and take the exterior derivative of
this equation, we get
         0 = d T d S &#x2212; d P d V   {\displaystyle 0=dTdS-dPdV}  [
      {\displaystyle 0=dTdS-dPdV}]
since     d ( d U ) = 0   {\displaystyle d(dU)=0}  [{\displaystyle d(dU)=0}].
This leads to the fundamental identity
         d P d V = d T d S .   {\displaystyle dPdV=dTdS.}  [{\displaystyle
      dPdV=dTdS.}]
The physical meaning of this identity can be seen by noting that the two sides
are the equivalent ways of writing the work done in an infinitesimal Carnot
cycle. An equivalent way of writing the identity is
            &#x2202; ( T , S )   &#x2202; ( P , V )    = 1.   {\displaystyle
      {\frac {\partial (T,S)}{\partial (P,V)}}=1.}  [{\displaystyle {\frac
      {\partial (T,S)}{\partial (P,V)}}=1.}]
The Maxwell relations now follow directly. For example,
           (      &#x2202; S   &#x2202; V       )    T   =    &#x2202; ( T , S
      )   &#x2202; ( T , V )    =    &#x2202; ( P , V )   &#x2202; ( T , V )
      =   (      &#x2202; P   &#x2202; T       )    V   ,   {\displaystyle
      {\Bigl (}{\frac {\partial S}{\partial V}}{\Bigr )}_{T}={\frac {\partial
      (T,S)}{\partial (T,V)}}={\frac {\partial (P,V)}{\partial (T,V)}}={\Bigl
      (}{\frac {\partial P}{\partial T}}{\Bigr )}_{V},}  [{\displaystyle {\Bigl
      (}{\frac {\partial S}{\partial V}}{\Bigr )}_{T}={\frac {\partial (T,S)}
      {\partial (T,V)}}={\frac {\partial (P,V)}{\partial (T,V)}}={\Bigl (}
      {\frac {\partial P}{\partial T}}{\Bigr )}_{V},}]
The critical step is the penultimate one. The other Maxwell relations follow in
similar fashion. For example,
           (      &#x2202; T   &#x2202; V       )    S   =    &#x2202; ( T , S
      )   &#x2202; ( V , S )    =    &#x2202; ( P , V )   &#x2202; ( V , S )
      = &#x2212;   (      &#x2202; P   &#x2202; S       )    V   .
      {\displaystyle {\Bigl (}{\frac {\partial T}{\partial V}}{\Bigr )}_{S}=
      {\frac {\partial (T,S)}{\partial (V,S)}}={\frac {\partial (P,V)}{\partial
      (V,S)}}=-{\Bigl (}{\frac {\partial P}{\partial S}}{\Bigr )}_{V}.}  [
      {\displaystyle {\Bigl (}{\frac {\partial T}{\partial V}}{\Bigr )}_{S}=
      {\frac {\partial (T,S)}{\partial (V,S)}}={\frac {\partial (P,V)}{\partial
      (V,S)}}=-{\Bigl (}{\frac {\partial P}{\partial S}}{\Bigr )}_{V}.}]
***** General Maxwell relationships[edit] *****
The above are not the only Maxwell relationships. When other work terms
involving other natural variables besides the volume work are considered or
when the number_of_particles is included as a natural variable, other Maxwell
relations become apparent. For example, if we have a single-component gas, then
the number of particles N  is also a natural variable of the above four
thermodynamic potentials. The Maxwell relationship for the enthalpy with
respect to pressure and particle number would then be:
           (    &#x2202; &#x03BC;   &#x2202; P    )   S , N   =   (    &#x2202;
      V   &#x2202; N    )   S , P    =     &#x2202;  2   H   &#x2202; P
      &#x2202; N      {\displaystyle \left({\frac {\partial \mu }{\partial
      P}}\right)_{S,N}=\left({\frac {\partial V}{\partial N}}\right)_
      {S,P}\qquad ={\frac {\partial ^{2}H}{\partial P\partial N}}}  [
      \left(\frac{\partial \mu}{\partial P}\right)_{S, N} =
      \left(\frac{\partial V}{\partial N}\right)_{S, P}\qquad=
      \frac{\partial^2 H }{\partial P \partial N}
      ]
where Î¼ is the chemical_potential. In addition, there are other thermodynamic
potentials besides the four that are commonly used, and each of these
potentials will yield a set of Maxwell relations.
Each equation can be re-expressed using the relationship
           (    &#x2202; y   &#x2202; x    )   z   = 1  /   (    &#x2202; x
      &#x2202; y    )   z       {\displaystyle \left({\frac {\partial y}
      {\partial x}}\right)_{z}=1\left/\left({\frac {\partial x}{\partial
      y}}\right)_{z}\right.}  [\left(\frac{\partial y}{\partial x}\right)_z
      =
      1\left/\left(\frac{\partial x}{\partial y}\right)_z\right.]
which are sometimes also known as Maxwell relations.
***** See also[edit] *****
    * Table_of_thermodynamic_equations
    * Thermodynamic_equations

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Maxwell_relations&oldid=893349773"
Categories:
    * James_Clerk_Maxwell
    * Thermodynamic_equations
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
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Svenska
    * à¹à¸à¸¢
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 20 April 2019, at 19:29 (UTC).
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
