The following text has been accessed from https://en.wikipedia.org/wiki/Continuity_equation at Fri Aug 9 00:52:36 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Continuity equation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Continuum_mechanics
Laws
Conservations
    * Mass
    * Momentum
    * Energy
Inequalities
    * ClausiusâDuhem_(entropy)
Solid_mechanics
    * Deformation
    * Elasticity
          o linear
    * Plasticity
    * Hooke's_law
    * Stress
    * Finite_strain
    * Infinitesimal_strain
    * Compatibility
    * Bending
    * Contact_mechanics
          o frictional
    * Material_failure_theory
    * Fracture_mechanics
Fluid_mechanics
Fluids
    * Statics Â· Dynamics
    * Archimedes'_principle Â· Bernoulli's_principle
    * NavierâStokes_equations
    * Poiseuille_equation Â· Pascal's_law
    * Viscosity
          o (Newtonian Â· non-Newtonian)
    * Buoyancy Â· Mixing Â· Pressure
Liquids
    * Surface_tension
    * Capillary_action
Gases
    * Atmosphere
    * Boyle's_law
    * Charles's_law
    * Gay-Lussac's_law
    * Combined_gas_law
Plasma
Rheology
    * Viscoelasticity
    * Rheometry
    * Rheometer
Smart_fluids
    * Electrorheological
    * Magnetorheological
    * Ferrofluids
Scientists
    * Bernoulli
    * Boyle
    * Cauchy
    * Charles
    * Euler
    * Gay-Lussac
    * Hooke
    * Pascal
    * Newton
    * Navier
    * Stokes
    * v
    * t
    * e
A continuity equation in physics is an equation that describes the transport of
some quantity. It is particularly simple and powerful when applied to a
conserved_quantity, but it can be generalized to apply to any extensive
quantity. Since mass, energy, momentum, electric_charge and other
natural quantities are conserved under their respective appropriate conditions,
a variety of physical phenomena may be described using continuity equations.
Continuity equations are a stronger, local form of conservation_laws. For
example, a weak version of the law of conservation_of_energy states that energy
can neither be created nor destroyedâi.e., the total amount of energy in the
universe is fixed. This statement does not rule out the possibility that a
quantity of energy could disappear from one point while simultaneously
appearing at another point. A stronger statement is that energy is locally
conserved: energy can neither be created nor destroyed, nor can it "teleport"
from one place to anotherâit can only move by a continuous flow. A continuity
equation is the mathematical way to express this kind of statement. For
example, the continuity equation for electric_charge states that the amount of
electric charge in any volume of space can only change by the amount of
electric_current flowing into or out of that volume through its boundaries.
Continuity equations more generally can include "source" and "sink" terms,
which allow them to describe quantities that are often but not always
conserved, such as the density of a molecular species which can be created or
destroyed by chemical reactions. In an everyday example, there is a continuity
equation for the number of people alive; it has a "source term" to account for
people being born, and a "sink term" to account for people dying.
Any continuity equation can be expressed in an "integral form" (in terms of a
flux_integral), which applies to any finite region, or in a "differential form"
(in terms of the divergence operator) which applies at a point.
Continuity equations underlie more specific transport_equations such as the
convectionâdiffusion_equation, Boltzmann_transport_equation, and
NavierâStokes_equations.
Flows governed by continuity equations can be visualized using a Sankey
diagram.
⁰
***** Contents *****
    * 1_General_equation
          o 1.1_Definition_of_flux
          o 1.2_Integral_form
          o 1.3_Differential_form
    * 2_Electromagnetism
    * 3_Fluid_dynamics
    * 4_Energy_and_heat
    * 5_Probability_distributions
    * 6_Quantum_mechanics
    * 7_Relativistic_version
          o 7.1_Special_relativity
          o 7.2_General_relativity
    * 8_Particle_physics
    * 9_Noether's_theorem
    * 10_See_also
    * 11_References
    * 12_Further_reading
***** General equation[edit] *****
**** Definition of flux[edit] ****
Main article: Flux
A continuity equation is useful when a flux can be defined. To define flux,
first there must be a quantity q which can flow or move, such as mass, energy,
electric_charge, momentum, number of molecules, etc. Let Ï be the volume
density of this quantity, that is, the amount of q per unit volume.
The way that this quantity q is flowing is described by its flux. The flux of q
is a vector_field, which we denote as j. Here are some examples and properties
of flux:
    * The dimension of flux is "amount of q flowing per unit time, through a
      unit area". For example, in the mass continuity equation for flowing
      water, if 1 gram per second of water is flowing through a pipe with
      cross-sectional area 1 cm2, then the average mass flux j inside the pipe
      is (1 gram / second) / cm2, and its direction is along the pipe in the
      direction that the water is flowing. Outside the pipe, where there is no
      water, the flux is zero.
    * If there is a velocity_field u which describes the relevant flowâin
      other words, if all of the quantity q at a point x is moving with
      velocity u(x)âthen the flux is by definition equal to the density times
      the velocity field:
                j  = &#x03C1;  u    {\displaystyle \mathbf {j} =\rho \mathbf
            {u} }  [\mathbf{j} = \rho \mathbf{u}]
      For example, if in the mass continuity equation for flowing water, u is
      the water's velocity at each point, and Ï is the water's density at each
      point, then j would be the mass flux.
    * In a well-known example, the flux of electric_charge is the electric
      current_density.
Illustration of how the flux j of a quantity q passes through an open surface
S. (dS is differential vector_area).
    * If there is an imaginary surface S, then the surface_integral of flux
      over S is equal to the amount of q that is passing through the surface S
      per unit time:
   (  Rate that&#xA0;  q  &#xA0;is flowing through the imaginary surface&#xA0;
S ) =  &#x222C;  S    j  &#x22C5; d  S    {\displaystyle ({\text{Rate that }}q
{\text{ is flowing through the imaginary surface }}S)=\iint _{S}\mathbf {j}
\cdot d\mathbf {S} }  [{\displaystyle ({\text{Rate that }}q{\text{ is flowing
through the imaginary surface }}S)=\iint _{S}\mathbf {j} \cdot d\mathbf {S} }]
      in which â¬S dS is a surface_integral.
(Note that the concept that is here called "flux" is alternatively termed "flux
density" in some literature, in which context "flux" denotes the surface
integral of flux density. See the main article on Flux for details.)
**** Integral form[edit] ****
The integral form of the continuity equation states that:
    * The amount of q in a region increases when additional q flows inward
      through the surface of the region, and decreases when it flows outward;
    * The amount of q in a region increases when new q is created inside the
      region, and decreases when q is destroyed;
    * Apart from these two processes, there is no other way for the amount of q
      in a region to change.
Mathematically, the integral form of the continuity equation expressing the
rate of increase of q within a volume V is:
      d q   d t    +   {\displaystyle {\frac {dq}{dt}}+}  [\frac{d q}{d t} + ]
[\oiint]     S    {\displaystyle \scriptstyle S}  [\scriptstyle S]      j
&#x22C5; d  S  = &#x03A3;   {\displaystyle \mathbf {j} \cdot d\mathbf {S}
=\Sigma }  [\mathbf{j} \cdot d\mathbf{S} = \Sigma]
where
In the integral form of the continuity equation, S is any imaginary closed
surface that fully encloses a volume V, like any of the surfaces on the left. S
can not be a surface with boundaries, like those on the right. (Surfaces are
blue, boundaries are red.)
    * S is any imaginary closed_surface, that encloses a volume V,
    * [\oiint]S dS denotes a surface_integral over that closed surface,
    * q is the total amount of the quantity in the volume V,
    * j is the flux of q,
    * t is time,
    * Î£ is the net rate that q is being generated inside the volume V. When q
      is being generated, it is called a source of q, and it makes Î£ more
      positive. When q is being destroyed, it is called a sink of q, and it
      makes Î£ more negative. This term is sometimes written as     d q  /  d t
      |    g e n      {\displaystyle dq/dt|_{\rm {gen}}}  [{\displaystyle dq/
      dt|_{\rm {gen}}}] or the total change of q from its generation or
      destruction inside the control volume.
In a simple example, V could be a building, and q could be the number of people
in the building. The surface S would consist of the walls, doors, roof, and
foundation of the building. Then the continuity equation states that the number
of people in the building increases when people enter the building (an inward
flux through the surface), decreases when people exit the building (an outward
flux through the surface), increases when someone in the building gives birth
(a source, Î£ > 0), and decreases when someone in the building dies (a sink, Î£
< 0).
**** Differential form[edit] ****
See also: Conservation_law and conservation_form
By the divergence_theorem, a general continuity equation can also be written in
a "differential form":
      &#x2202; &#x03C1;   &#x2202; t    + &#x2207; &#x22C5;  j  = &#x03C3;
{\displaystyle {\frac {\partial \rho }{\partial t}}+\nabla \cdot \mathbf {j}
=\sigma \,}  [\frac{\partial \rho}{\partial t} + \nabla \cdot \mathbf{j} =
\sigma\,]
where
    * ââ is divergence,
    * Ï is the amount of the quantity q per unit volume,
    * j is the flux of q,
    * t is time,
    * Ï is the generation of q per unit volume per unit time. Terms that
      generate q (i.e. Ï > 0) or remove q (i.e. Ï < 0) are referred to as a
      "sources" and "sinks" respectively.
This general equation may be used to derive any continuity equation, ranging
from as simple as the volume continuity equation to as complicated as the
NavierâStokes_equations. This equation also generalizes the advection
equation. Other equations in physics, such as Gauss's_law_of_the_electric_field
and Gauss's_law_for_gravity, have a similar mathematical form to the continuity
equation, but are not usually referred to by the term "continuity equation",
because j in those cases does not represent the flow of a real physical
quantity.
In the case that q is a conserved_quantity that cannot be created or destroyed
(such as energy), Ï = 0 and the equations becomes:
            &#x2202; &#x03C1;   &#x2202; t    + &#x2207; &#x22C5;  j  = 0
      {\displaystyle {\frac {\partial \rho }{\partial t}}+\nabla \cdot \mathbf
      {j} =0\,}  [\frac{\partial \rho}{\partial t} + \nabla \cdot \mathbf{j} =
      0\,]
***** Electromagnetism[edit] *****
Main article: Charge_conservation
In electromagnetic_theory, the continuity equation is an empirical law
expressing (local) charge_conservation. Mathematically it is an automatic
consequence of Maxwell's_equations, although charge conservation is more
fundamental than Maxwell's equations. It states that the divergence of the
current_density J (in amperes per square metre) is equal to the negative rate
of change of the charge_density Ï (in coulombs per cubic metre),
         &#x2207; &#x22C5;  J  = &#x2212;    &#x2202; &#x03C1;   &#x2202; t
      {\displaystyle \nabla \cdot \mathbf {J} =-{\partial \rho \over \partial
      t}}  [ \nabla \cdot \mathbf{J} = - {\partial \rho \over \partial t} ]
      Consistency with Maxwell's equations
      One of Maxwell's_equations, AmpÃ¨re's_law_(with_Maxwell's_correction),
      states that
               &#x2207; &#x00D7;  H  =  J  +    &#x2202;  D    &#x2202; t    .
            {\displaystyle \nabla \times \mathbf {H} =\mathbf {J} +{\frac
            {\partial \mathbf {D} }{\partial t}}.}  [ \nabla \times \mathbf{H}
            = \mathbf{J} + \frac{\partial \mathbf{D}}{\partial t}. ]
      Taking the divergence of both sides (the divergence and partial
      derivative in time commute) results in
               &#x2207; &#x22C5; ( &#x2207; &#x00D7;  H  ) = &#x2207; &#x22C5;
            J  +    &#x2202; ( &#x2207; &#x22C5;  D  )   &#x2202; t    ,
            {\displaystyle \nabla \cdot (\nabla \times \mathbf {H} )=\nabla
            \cdot \mathbf {J} +{\frac {\partial (\nabla \cdot \mathbf {D} )}
            {\partial t}},}  [ \nabla \cdot ( \nabla \times \mathbf{H} ) =
            \nabla \cdot \mathbf{J} + \frac{\partial (\nabla \cdot \mathbf{D})}
            {\partial t}, ]
      but the divergence of a curl is zero, so that
               &#x2207; &#x22C5;  J  +    &#x2202; ( &#x2207; &#x22C5;  D  )
            &#x2202; t    = 0.   {\displaystyle \nabla \cdot \mathbf {J} +
            {\frac {\partial (\nabla \cdot \mathbf {D} )}{\partial t}}=0.}
            [ \nabla \cdot \mathbf{J} + \frac{\partial (\nabla \cdot \mathbf
            {D})}{\partial t} = 0. ]
      Another one of Maxwell's equations, Gauss's_law, states that
               &#x2207; &#x22C5;  D  = &#x03C1; ,    {\displaystyle \nabla
            \cdot \mathbf {D} =\rho ,\,}  [ \nabla \cdot \mathbf{D} = \rho,\, ]
      substitution into the previous equation yields the continuity equation
               &#x2207; &#x22C5;  J  +    &#x2202; &#x03C1;   &#x2202; t    =
            0.    {\displaystyle \nabla \cdot \mathbf {J} +{\partial \rho \over
            \partial t}=0.\,}  [ \nabla \cdot \mathbf{J} + {\partial \rho \over
            \partial t} = 0.\,]
Current is the movement of charge. The continuity equation says that if charge
is moving out of a differential volume (i.e. divergence of current density is
positive) then the amount of charge within that volume is going to decrease, so
the rate of change of charge density is negative. Therefore, the continuity
equation amounts to a conservation of charge.
If magnetic_monopoles exist, there would be a continuity equation for monopole
currents as well, see the monopole article for background and the duality
between electric and magnetic currents.
***** Fluid dynamics[edit] *****
See also: Mass_flux and Vorticity_equation
In fluid_dynamics, the continuity equation states that the rate at which mass
enters a system is equal to the rate at which mass leaves the system plus the
accumulation of mass within the system.[1][2] The differential form of the
continuity equation is:[1]
            &#x2202; &#x03C1;   &#x2202; t    + &#x2207; &#x22C5; ( &#x03C1;  u
      ) = 0   {\displaystyle {\frac {\partial \rho }{\partial t}}+\nabla \cdot
      (\rho \mathbf {u} )=0}  [{\displaystyle {\frac {\partial \rho }{\partial
      t}}+\nabla \cdot (\rho \mathbf {u} )=0}]
where
    * Ï is fluid density,
    * t is time,
    * u is the flow_velocity vector_field.
The time derivative can be understood as the accumulation (or loss) of mass in
the system, while the divergence term represents the difference in flow in
versus flow out. In this context, this equation is also one of the Euler
equations_(fluid_dynamics). The NavierâStokes_equations form a vector
continuity equation describing the conservation of linear_momentum.
If the fluid is an incompressible_flow (Ï is constant), the mass continuity
equation simplifies to a volume continuity equation:[1]
         &#x2207; &#x22C5;  u  = 0 ,   {\displaystyle \nabla \cdot \mathbf {u}
      =0,}  [\nabla \cdot \mathbf{u} = 0,]
which means that the divergence of velocity field is zero everywhere.
Physically, this is equivalent to saying that the local volume dilation rate is
zero, hence a flow of water through a converging pipe will adjust solely by
increasing its velocity as water is largely incompressible.
***** Energy and heat[edit] *****
Conservation_of_energy says that energy cannot be created or destroyed. (See
below for the nuances associated with general relativity.) Therefore, there is
a continuity equation for energy flow:
            &#x2202; u   &#x2202; t    + &#x2207; &#x22C5;  q  = 0
      {\displaystyle {\frac {\partial u}{\partial t}}+\nabla \cdot \mathbf {q}
      =0}  [ \frac{ \partial u}{\partial t} + \nabla \cdot \mathbf{q} = 0]
where
    * u = local energy_density (energy per unit volume),
    * q = energy_flux (transfer of energy per unit cross-sectional area per
      unit time) as a vector,
An important practical example is the_flow_of_heat. When heat flows inside a
solid, the continuity equation can be combined with Fourier's_law (heat flux is
proportional to temperature gradient) to arrive at the heat_equation. The
equation of heat flow may also have source terms: Although energy cannot be
created or destroyed, heat can be created from other types of energy, for
example via friction or joule_heating.
***** Probability distributions[edit] *****
If there is a quantity that moves continuously according to a stochastic
(random) process, like the location of a single dissolved molecule with
Brownian_motion, then there is a continuity equation for its probability
distribution. The flux in this case is the probability per unit area per unit
time that the particle passes through a surface. According to the continuity
equation, the negative divergence of this flux equals the rate of change of the
probability_density. The continuity equation reflects the fact that the
molecule is always somewhereâthe integral of its probability distribution is
always equal to 1âand that it moves by a continuous motion (no teleporting).
***** Quantum mechanics[edit] *****
Quantum_mechanics is another domain where there is a continuity equation
related to conservation of probability. The terms in the equation require the
following definitions, and are slightly less obvious than the other examples
above, so they are outlined here:
    * The wavefunction Î¨ for a single particle in position_space (rather than
      momentum_space), that is, a function of position r and time t, Î¨ = Î¨(r,
      t).
    * The probability_density_function is:
         &#x03C1; (  r  , t ) =  &#x03A8;  &#x2217;   (  r  , t ) &#x03A8; (  r
      , t ) =  |  &#x03A8; (  r  , t )   |   2     {\displaystyle \rho (\mathbf
      {r} ,t)=\Psi ^{*}(\mathbf {r} ,t)\Psi (\mathbf {r} ,t)=|\Psi (\mathbf {r}
      ,t)|^{2}}  [{\displaystyle \rho (\mathbf {r} ,t)=\Psi ^{*}(\mathbf {r}
      ,t)\Psi (\mathbf {r} ,t)=|\Psi (\mathbf {r} ,t)|^{2}}]
    * The probability of finding the particle within V at t is denoted and
      defined by:
         P =  P   r  &#x2208; V   ( t ) =  &#x222B;  V    &#x03A8;  &#x2217;
      &#x03A8; d V =  &#x222B;  V    |  &#x03A8;   |   2   d V   {\displaystyle
      P=P_{\mathbf {r} \in V}(t)=\int _{V}\Psi ^{*}\Psi dV=\int _{V}|\Psi |^
      {2}dV}  [{\displaystyle P=P_{\mathbf {r} \in V}(t)=\int _{V}\Psi ^{*}\Psi
      dV=\int _{V}|\Psi |^{2}dV}]
    * The probability_current (aka probability flux):
          j  (  r  , t ) =   &#x210F;  2 m i     [   &#x03A8;  &#x2217;
      (  &#x2207; &#x03A8;  )  &#x2212; &#x03A8;  (  &#x2207;  &#x03A8;
      &#x2217;    )   ]  .   {\displaystyle \mathbf {j} (\mathbf {r} ,t)={\frac
      {\hbar }{2mi}}\left[\Psi ^{*}\left(\nabla \Psi \right)-\Psi \left(\nabla
      \Psi ^{*}\right)\right].}  [ \mathbf{j}(\mathbf{r},t) = \frac{\hbar}{2mi}
      \left [ \Psi^{*} \left ( \nabla \Psi \right ) - \Psi \left ( \nabla \Psi^
      {*} \right ) \right ]. ]
With these definitions the continuity equation reads:
         &#x2207; &#x22C5;  j  +    &#x2202; &#x03C1;   &#x2202; t    = 0
      &#x21CC; &#x2207; &#x22C5;  j  +    &#x2202;  |  &#x03A8;   |   2
      &#x2202; t    = 0.   {\displaystyle \nabla \cdot \mathbf {j} +{\frac
      {\partial \rho }{\partial t}}=0\rightleftharpoons \nabla \cdot \mathbf
      {j} +{\frac {\partial |\Psi |^{2}}{\partial t}}=0.}  [ \nabla \cdot
      \mathbf{j} + \frac{\partial \rho}{\partial t} = 0 \rightleftharpoons
      \nabla \cdot \mathbf{j} + \frac{\partial |\Psi|^2}{\partial t} = 0.]
Either form may be quoted. Intuitively, the above quantities indicate this
represents the flow of probability. The chance of finding the particle at some
position r and time t flows like a fluid; hence the term probability current, a
vector_field. The particle itself does not flow deterministically in this
vector_field.
      Consistency with SchrÃ¶dinger equation
      For this derivation see[3] for example. The 3-d time dependent SchrÃ¶dinger
      equation and its complex_conjugate (i â âi throughout) are respectively:
                     &#x2212;    &#x210F;  2    2 m     &#x2207;  2   &#x03A8; + U
            &#x03A8; = i &#x210F;    &#x2202; &#x03A8;   &#x2202; t    ,       &#x2212;
            &#x210F;  2    2 m     &#x2207;  2    &#x03A8;  &#x2217;   + U  &#x03A8;
            &#x2217;   = &#x2212; i &#x210F;    &#x2202;  &#x03A8;  &#x2217;     &#x2202;
            t    ,       {\displaystyle {\begin{aligned}&-{\frac {\hbar ^{2}}{2m}}\nabla
            ^{2}\Psi +U\Psi =i\hbar {\frac {\partial \Psi }{\partial t}},\\&-{\frac
            {\hbar ^{2}}{2m}}\nabla ^{2}\Psi ^{*}+U\Psi ^{*}=-i\hbar {\frac {\partial
            \Psi ^{*}}{\partial t}},\\\end{aligned}}}  [ \begin{align} & -\frac{\hbar^2}
            {2m}\nabla^2 \Psi + U\Psi = i\hbar \frac{\partial \Psi}{\partial t} , \\
            & - \frac{\hbar^2}{2m}\nabla^2 \Psi^{*} + U\Psi^{*} = - i\hbar \frac{\partial
            \Psi^{*}}{\partial t} ,\\
            \end{align}]
      where U is the potential_function. The partial_derivative of Ï with respect to t
      is:
                  &#x2202; &#x03C1;   &#x2202; t    =    &#x2202;  |  &#x03A8;   |   2
            &#x2202; t    =   &#x2202;  &#x2202; t     (   &#x03A8;  &#x2217;   &#x03A8;
            )  =  &#x03A8;  &#x2217;      &#x2202; &#x03A8;   &#x2202; t    + &#x03A8;
            &#x2202;  &#x03A8;  &#x2217;     &#x2202; t    .   {\displaystyle {\frac
            {\partial \rho }{\partial t}}={\frac {\partial |\Psi |^{2}}{\partial t}}=
            {\frac {\partial }{\partial t}}\left(\Psi ^{*}\Psi \right)=\Psi ^{*}{\frac
            {\partial \Psi }{\partial t}}+\Psi {\frac {\partial \Psi ^{*}}{\partial t}}.}
            [ \frac{\partial \rho}{\partial t} = \frac{\partial |\Psi |^2}{\partial t } =
            \frac{\partial}{\partial t} \left ( \Psi^{*} \Psi \right ) =  \Psi^{*} \frac
            {\partial \Psi}{\partial t} + \Psi \frac{\partial\Psi^{*}}{\partial t} .]
      Multiplying the SchrÃ¶dinger equation by Î¨* then solving for Î¨* âÎ¨/ât, and
      similarly multiplying the complex conjugated SchrÃ¶dinger equation by Î¨ then
      solving for Î¨ âÎ¨*/ât;
                     &#x03A8;  &#x2217;      &#x2202; &#x03A8;   &#x2202; t    =   1  i
            &#x210F;     [  &#x2212;     &#x210F;  2    &#x03A8;  &#x2217;     2 m
            &#x2207;  2   &#x03A8; + U  &#x03A8;  &#x2217;   &#x03A8;  ]  ,      &#x03A8;
            &#x2202;  &#x03A8;  &#x2217;     &#x2202; t    = &#x2212;   1  i &#x210F;
            [  &#x2212;     &#x210F;  2   &#x03A8;   2 m     &#x2207;  2    &#x03A8;
            &#x2217;   + U &#x03A8;  &#x03A8;  &#x2217;    ]  ,       {\displaystyle
            {\begin{aligned}&\Psi ^{*}{\frac {\partial \Psi }{\partial t}}={\frac {1}
            {i\hbar }}\left[-{\frac {\hbar ^{2}\Psi ^{*}}{2m}}\nabla ^{2}\Psi +U\Psi ^
            {*}\Psi \right],\\&\Psi {\frac {\partial \Psi ^{*}}{\partial t}}=-{\frac {1}
            {i\hbar }}\left[-{\frac {\hbar ^{2}\Psi }{2m}}\nabla ^{2}\Psi ^{*}+U\Psi \Psi
            ^{*}\right],\\\end{aligned}}}  [ \begin{align} & \Psi^*\frac{\partial \Psi}
            {\partial t} = \frac{1}{i\hbar } \left [ -\frac{\hbar^2\Psi^*}{2m}\nabla^2
            \Psi + U\Psi^*\Psi \right ], \\
            & \Psi \frac{\partial \Psi^*}{\partial t} = - \frac{1}{i\hbar } \left [ -
            \frac{\hbar^2\Psi}{2m}\nabla^2 \Psi^* + U\Psi\Psi^* \right ],\\
            \end{align}]
      substituting into the time derivative of Ï:
                      &#x2202; &#x03C1;   &#x2202; t       =   1  i &#x210F;
            [  &#x2212;     &#x210F;  2    &#x03A8;  &#x2217;     2 m     &#x2207;  2
            &#x03A8; + U  &#x03A8;  &#x2217;   &#x03A8;  ]  &#x2212;   1  i &#x210F;
            [  &#x2212;     &#x210F;  2   &#x03A8;   2 m     &#x2207;  2    &#x03A8;
            &#x2217;   + U &#x03A8;  &#x03A8;  &#x2217;    ]        =   1  i &#x210F;
            [  &#x2212;     &#x210F;  2    &#x03A8;  &#x2217;     2 m     &#x2207;  2
            &#x03A8; + U  &#x03A8;  &#x2217;   &#x03A8;  ]  +   1  i &#x210F;     [  +
            &#x210F;  2   &#x03A8;   2 m     &#x2207;  2    &#x03A8;  &#x2217;   &#x2212;
            U  &#x03A8;  &#x2217;   &#x03A8;  ]        = &#x2212;   1  i &#x210F;
            &#x210F;  2    &#x03A8;  &#x2217;     2 m     &#x2207;  2   &#x03A8; +   1  i
            &#x210F;        &#x210F;  2   &#x03A8;   2 m     &#x2207;  2    &#x03A8;
            &#x2217;         =   &#x210F;  2 i m     [  &#x03A8;  &#x2207;  2    &#x03A8;
            &#x2217;   &#x2212;  &#x03A8;  &#x2217;    &#x2207;  2   &#x03A8;  ]
            {\displaystyle {\begin{aligned}{\frac {\partial \rho }{\partial t}}&={\frac
            {1}{i\hbar }}\left[-{\frac {\hbar ^{2}\Psi ^{*}}{2m}}\nabla ^{2}\Psi +U\Psi ^
            {*}\Psi \right]-{\frac {1}{i\hbar }}\left[-{\frac {\hbar ^{2}\Psi }
            {2m}}\nabla ^{2}\Psi ^{*}+U\Psi \Psi ^{*}\right]\\&={\frac {1}{i\hbar }}\left
            [-{\frac {\hbar ^{2}\Psi ^{*}}{2m}}\nabla ^{2}\Psi +U\Psi ^{*}\Psi \right]+
            {\frac {1}{i\hbar }}\left[+{\frac {\hbar ^{2}\Psi }{2m}}\nabla ^{2}\Psi ^{*}-
            U\Psi ^{*}\Psi \right]\\&=-{\frac {1}{i\hbar }}{\frac {\hbar ^{2}\Psi ^{*}}
            {2m}}\nabla ^{2}\Psi +{\frac {1}{i\hbar }}{\frac {\hbar ^{2}\Psi }{2m}}\nabla
            ^{2}\Psi ^{*}\\&={\frac {\hbar }{2im}}\left[\Psi \nabla ^{2}\Psi ^{*}-\Psi ^
            {*}\nabla ^{2}\Psi \right]\\\end{aligned}}}  [ \begin{align}
            \frac{\partial \rho}{\partial t} & = \frac{1}{i\hbar } \left [ -\frac
            {\hbar^2\Psi^{*}}{2m}\nabla^2 \Psi + U\Psi^{*}\Psi \right ] - \frac{1}{i\hbar
            } \left [ - \frac{\hbar^2\Psi}{2m}\nabla^2 \Psi^{*} + U\Psi\Psi^{*} \right ]
            \\
             & = \frac{1}{i\hbar } \left [ -\frac{\hbar^2\Psi^{*}}{2m}\nabla^2 \Psi +
            U\Psi^{*}\Psi \right ] + \frac{1}{i\hbar } \left [ +\frac{\hbar^2\Psi}
            {2m}\nabla^2 \Psi^{*} - U\Psi^{*}\Psi \right ] \\
             & = - \frac{1}{i\hbar } \frac{\hbar^2\Psi^{*}}{2m}\nabla^2 \Psi  + \frac{1}
            {i\hbar } \frac{\hbar^2\Psi}{2m}\nabla^2 \Psi^{*} \\
             & = \frac{\hbar}{2im} \left [ \Psi\nabla^2 \Psi^{*} - \Psi^{*}\nabla^2 \Psi
            \right ] \\
            \end{align} ]
      The Laplacian operators (â2) in the above result suggest that the right hand side
      is the divergence of j, and the reversed order of terms imply this is the negative
      of j, altogether:
                   &#x2207; &#x22C5;  j     = &#x2207; &#x22C5;  [    &#x210F;  2 m i
            (   &#x03A8;  &#x2217;    (  &#x2207; &#x03A8;  )  &#x2212; &#x03A8;
            (  &#x2207;  &#x03A8;  &#x2217;    )   )   ]        =   &#x210F;  2 m i
            [   &#x03A8;  &#x2217;    (   &#x2207;  2   &#x03A8;  )  &#x2212; &#x03A8;
            (   &#x2207;  2    &#x03A8;  &#x2217;    )   ]        = &#x2212;   &#x210F;
            2 m i     [  &#x03A8;  (   &#x2207;  2    &#x03A8;  &#x2217;    )  &#x2212;
            &#x03A8;  &#x2217;    (   &#x2207;  2   &#x03A8;  )   ]        {\displaystyle
            {\begin{aligned}\nabla \cdot \mathbf {j} &=\nabla \cdot \left[{\frac {\hbar }
            {2mi}}\left(\Psi ^{*}\left(\nabla \Psi \right)-\Psi \left(\nabla \Psi ^
            {*}\right)\right)\right]\\&={\frac {\hbar }{2mi}}\left[\Psi ^{*}\left(\nabla
            ^{2}\Psi \right)-\Psi \left(\nabla ^{2}\Psi ^{*}\right)\right]\\&=-{\frac
            {\hbar }{2mi}}\left[\Psi \left(\nabla ^{2}\Psi ^{*}\right)-\Psi ^{*}\left
            (\nabla ^{2}\Psi \right)\right]\\\end{aligned}}}  [\begin{align} \nabla \cdot
            \mathbf{j} & = \nabla \cdot \left [ \frac{\hbar}{2mi} \left ( \Psi^{*} \left
            ( \nabla \Psi \right ) - \Psi \left ( \nabla \Psi^{*} \right ) \right )
            \right ] \\
             & = \frac{\hbar}{2mi} \left [ \Psi^{*} \left ( \nabla^2 \Psi \right ) - \Psi
            \left ( \nabla^2 \Psi^{*} \right ) \right ] \\
             & = - \frac{\hbar}{2mi} \left [ \Psi \left ( \nabla^2 \Psi^{*} \right ) -
            \Psi^{*} \left ( \nabla^2 \Psi \right ) \right ] \\
            \end{align} ]
      so the continuity equation is:
                       &#x2202; &#x03C1;   &#x2202; t    = &#x2212; &#x2207; &#x22C5;  j
            &#x2202; &#x03C1;   &#x2202; t    + &#x2207; &#x22C5;  j  = 0
            {\displaystyle {\begin{aligned}&{\frac {\partial \rho }{\partial t}}=-\nabla
            \cdot \mathbf {j} \\&{\frac {\partial \rho }{\partial t}}+\nabla \cdot
            \mathbf {j} =0\\\end{aligned}}}  [ \begin{align} & \frac{\partial \rho}
            {\partial t} = - \nabla \cdot \mathbf{j} \\
            & \frac{\partial \rho}{\partial t} + \nabla \cdot \mathbf{j} = 0 \\
            \end{align}]
      The integral form follows as for the general equation.
***** Relativistic version[edit] *****
**** Special relativity[edit] ****
See also: 4-vector
The notation and tools of special_relativity, especially 4-vectors and 4-
gradients, offer a convenient way to write any continuity equation.
The density of a quantity Ï and its current j can be combined into a 4-vector
called a 4-current:
         J =  (  c &#x03C1; ,  j  x   ,  j  y   ,  j  z    )    {\displaystyle
      J=\left(c\rho ,j_{x},j_{y},j_{z}\right)}  [J = \left(c \rho, j_x, j_y,
      j_z \right)]
where c is the speed_of_light. The 4-divergence of this current is:
          &#x2202;  &#x03BC;    J  &#x03BC;   = c    &#x2202; &#x03C1;
      &#x2202; t    + &#x2207; &#x22C5;  j    {\displaystyle \partial _{\mu }J^
      {\mu }=c{\frac {\partial \rho }{\partial t}}+\nabla \cdot \mathbf {j} }
      [{\displaystyle \partial _{\mu }J^{\mu }=c{\frac {\partial \rho }
      {\partial t}}+\nabla \cdot \mathbf {j} }]
where âÎ¼ is the 4-gradient and Î¼ is an index labelling the spacetime
dimension. Then the continuity equation is:
          &#x2202;  &#x03BC;    J  &#x03BC;   = 0   {\displaystyle \partial _
      {\mu }J^{\mu }=0}  [\partial_\mu J^\mu = 0]
in the usual case where there are no sources or sinks, that is, for perfectly
conserved quantities like energy or charge. This continuity equation is
manifestly ("obviously") Lorentz_invariant.
Examples of continuity equations often written in this form include electric
charge conservation
          &#x2202;  &#x03BC;    J  &#x03BC;   = 0   {\displaystyle \partial _
      {\mu }J^{\mu }=0}  [\partial_\mu J^\mu = 0]
where J is the electric 4-current; and energy-momentum conservation
          &#x2202;  &#x03BD;    T  &#x03BC; &#x03BD;   = 0   {\displaystyle
      \partial _{\nu }T^{\mu \nu }=0}  [\partial_\nu T^{\mu\nu} = 0]
where T is the stress-energy_tensor.
**** General relativity[edit] ****
In general_relativity, where spacetime is curved, the continuity equation (in
differential form) for energy, charge, or other conserved quantities involves
the covariant_divergence instead of the ordinary divergence.
For example, the stressâenergy_tensor is a second-order tensor_field
containing energyâmomentum densities, energyâmomentum fluxes, and shear
stresses, of a mass-energy distribution. The differential form of energy-
momentum conservation in general relativity states that the covariant
divergence of the stress-energy tensor is zero:
            T  &#x03BC;     &#x03BD; ; &#x03BC;   = 0.   {\displaystyle {T^{\mu
      }}_{\nu ;\mu }=0.}  [{\displaystyle {T^{\mu }}_{\nu ;\mu }=0.}]
This is an important constraint on the form the Einstein_field_equations take
in general_relativity.[4]
However, the ordinary divergence of the stress-energy tensor does not
necessarily vanish:[5]
          &#x2202;  &#x03BC;    T  &#x03BC; &#x03BD;   = &#x2212;  &#x0393;
      &#x03BC; &#x03BB;   &#x03BC;    T  &#x03BB; &#x03BD;   &#x2212;  &#x0393;
      &#x03BC; &#x03BB;   &#x03BD;    T  &#x03BC; &#x03BB;   ,   {\displaystyle
      \partial _{\mu }T^{\mu \nu }=-\Gamma _{\mu \lambda }^{\mu }T^{\lambda \nu
      }-\Gamma _{\mu \lambda }^{\nu }T^{\mu \lambda },}  [{\displaystyle
      \partial _{\mu }T^{\mu \nu }=-\Gamma _{\mu \lambda }^{\mu }T^{\lambda \nu
      }-\Gamma _{\mu \lambda }^{\nu }T^{\mu \lambda },}]
The right-hand side strictly vanishes for a flat geometry only.
As a consequence, the integral form of the continuity equation is difficult to
define and not necessarily valid for a region within which spacetime is
significantly curved (e.g. around a black hole, or across the whole universe).
[6]
***** Particle physics[edit] *****
Quarks and gluons have color_charge, which is always conserved like electric
charge, and there is a continuity equation for such color charge currents
(explicit expressions for currents are given at gluon_field_strength_tensor).
There are many other quantities in particle physics which are often or always
conserved: baryon_number (proportional to the number of quarks minus the number
of antiquarks), electron_number,_mu_number,_tau_number, isospin, and others.[7]
Each of these has a corresponding continuity equation, possibly including
source / sink terms.
***** Noether's theorem[edit] *****
For more detailed explanations and derivations, see Noether's_theorem.
One reason that conservation equations frequently occur in physics is Noether's
theorem. This states that whenever the laws of physics have a continuous
symmetry, there is a continuity equation for some conserved physical quantity.
The three most famous examples are:
    * The laws of physics are invariant with respect to time-translationâfor
      example, the laws of physics today are the same as they were yesterday.
      This symmetry leads to the continuity equation for conservation_of
      energy.
    * The laws of physics are invariant with respect to space-translationâfor
      example, the laws of physics in Brazil are the same as the laws of
      physics in Argentina. This symmetry leads to the continuity equation for
      conservation_of_momentum.
    * The laws of physics are invariant with respect to orientationâfor
      example, floating in outer space, there is no measurement you can do to
      say "which way is up"; the laws of physics are the same regardless of how
      you are oriented. This symmetry leads to the continuity equation for
      conservation_of_angular_momentum.
See Noether's_theorem for proofs and details.
***** See also[edit] *****
    * Conservation_law
    * Conservation_form
    * Dissipative_system
***** References[edit] *****
   1. ^ a b cPedlosky, Joseph (1987). Geophysical fluid dynamics. Springer.
      pp. 10â13. ISBN 978-0-387-96387-7.
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
   3. ^ Clancy, L.J.(1975), Aerodynamics, Section 3.3, Pitman Publishing
      Limited, London
   4. ^ Quantum Mechanics Demystified, D. McMahon, McGraw Hill (USA), 2006,
   5. ISBN 0-07-145546-9
   6. ^D. McMahon (2006). Relativity DeMystified. McGraw Hill (USA). ISBN 0-07-
      145545-0.
   7. ^C.W. Misner; K.S. Thorne; J.A. Wheeler (1973). Gravitation. W.H. Freeman
      & Co. ISBN 0-7167-0344-0.
   8. ^Michael Weiss; John Baez. "Is_Energy_Conserved_in_General_Relativity?".
      Retrieved 2014-04-25.
   9. ^J.A. Wheeler; C. Misner; K.S. Thorne (1973). Gravitation. W.H. Freeman &
      Co. pp. 558â559. ISBN 0-7167-0344-0.
***** Further reading[edit] *****
    * Hydrodynamics, H. Lamb, Cambridge University Press, (2006 digitalization
      of 1932 6th edition)
ISBN 978-0-521-45868-9
Introduction to Electrodynamics (3rd Edition), D.J. Griffiths, Pearson
Education Inc, 1999,
ISBN 81-7758-293-3
Electromagnetism (2nd edition), I.S. Grant, W.R. Phillips, Manchester Physics
Series, 2008
ISBN 0-471-92712-0
Gravitation, J.A. Wheeler, C. Misner, K.S. Thorne, W.H. Freeman & Co, 1973,
ISBN 0-7167-0344-0

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Continuity_equation&oldid=905851119"
Categories:
    * Equations_of_fluid_dynamics
    * Conservation_equations
    * Partial_differential_equations
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * Magyar
    * à¤®à¤°à¤¾à¤ à¥
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * SlovenÅ¡Äina
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 11 July 2019, at 21:27 (UTC).
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
