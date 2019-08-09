The following text has been accessed from https://en.wikipedia.org/wiki/Differential_equation at Fri Aug 9 01:24:19 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Differential equation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with Difference_equation.
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (August 2009)(Learn_how_and
 when_to_remove_this_template_message)
Visualization of heat transfer in a pump casing, created by solving the heat
equation. Heat is being generated internally in the casing and being cooled at
the boundary, providing a steady_state temperature distribution.
A differential equation is a mathematical equation that relates some function
with its derivatives. In applications, the functions usually represent physical
quantities, the derivatives represent their rates of change, and the
differential equation defines a relationship between the two. Because such
relations are extremely common, differential equations play a prominent role in
many disciplines including engineering, physics, economics, and biology.
In pure_mathematics, differential equations are studied from several different
perspectives, mostly concerned with their solutionsâthe set of functions that
satisfy the equation. Only the simplest differential equations are solvable by
explicit formulas; however, some properties of solutions of a given
differential equation may be determined without finding their exact form.
If a closed-form_expression for the solution is not available, the solution may
be numerically approximated using computers. The theory of dynamical_systems
puts emphasis on qualitative analysis of systems described by differential
equations, while many numerical_methods have been developed to determine
solutions with a given degree of accuracy.
⁰
***** Contents *****
    * 1_History
    * 2_Example
    * 3_Types
          o 3.1_Ordinary_differential_equations
          o 3.2_Partial_differential_equations
          o 3.3_Non-linear_differential_equations
          o 3.4_Equation_order
          o 3.5_Examples
    * 4_Existence_of_solutions
    * 5_Related_concepts
    * 6_Connection_to_difference_equations
    * 7_Applications
          o 7.1_Pure_Mathematics
          o 7.2_Physics
                # 7.2.1_Classical_mechanics
                # 7.2.2_Electrodynamics
                # 7.2.3_General_relativity
                # 7.2.4_Quantum_mechanics
          o 7.3_Engineering
          o 7.4_Biology_and_Medicine
                # 7.4.1_Predator-prey_equations
          o 7.5_Chemistry
          o 7.6_Economics_and_Finance
    * 8_See_also
    * 9_References
    * 10_Further_reading
    * 11_External_links
***** History[edit] *****
Differential equations first came into existence with the invention_of_calculus
by Newton and Leibniz. In Chapter 2 of his 1671 work Methodus_fluxionum_et
Serierum_Infinitarum,[1] Isaac Newton listed three kinds of differential
equations:
                 d y   d x    = f ( x )         d y   d x    = f ( x , y )
      x  1      &#x2202; y   &#x2202;  x  1      +  x  2      &#x2202; y
      &#x2202;  x  2      = y       {\displaystyle {\begin{aligned}&{\frac {dy}
      {dx}}=f(x)\\[5pt]&{\frac {dy}{dx}}=f(x,y)\\[5pt]&x_{1}{\frac {\partial y}
      {\partial x_{1}}}+x_{2}{\frac {\partial y}{\partial x_{2}}}=y\end
      {aligned}}}  [{\displaystyle {\begin{aligned}&{\frac {dy}{dx}}=f(x)\\
      [5pt]&{\frac {dy}{dx}}=f(x,y)\\[5pt]&x_{1}{\frac {\partial y}{\partial x_
      {1}}}+x_{2}{\frac {\partial y}{\partial x_{2}}}=y\end{aligned}}}]
In all these cases, y is an unknown function of x (or of      x  1
{\displaystyle x_{1}}  [x_{1}] and      x  2     {\displaystyle x_{2}}  [x_
{2}]), and f is a given function.
He solves these examples and others using infinite series and discusses the
non-uniqueness of solutions.
Jacob_Bernoulli proposed the Bernoulli_differential_equation in 1695.[2] This
is an ordinary_differential_equation of the form
          y &#x2032;  + P ( x ) y = Q ( x )  y  n      {\displaystyle y'+P
      (x)y=Q(x)y^{n}\,}  [y'+P(x)y=Q(x)y^{n}\,]
for which the following year Leibniz obtained solutions by simplifying it.[3]
Historically, the problem of a vibrating string such as that of a musical
instrument was studied by Jean_le_Rond_d'Alembert, Leonhard_Euler, Daniel
Bernoulli, and Joseph-Louis_Lagrange.[4][5][6][7] In 1746, dâAlembert
discovered the one-dimensional wave_equation, and within ten years Euler
discovered the three-dimensional wave equation.[8]
The EulerâLagrange_equation was developed in the 1750s by Euler and Lagrange
in connection with their studies of the tautochrone problem. This is the
problem of determining a curve on which a weighted particle will fall to a
fixed point in a fixed amount of time, independent of the starting point.
Lagrange solved this problem in 1755 and sent the solution to Euler. Both
further developed Lagrange's method and applied it to mechanics, which led to
the formulation of Lagrangian_mechanics.
In 1822, Fourier published his work on heat_flow in ThÃ©orie analytique de la
chaleur (The Analytic Theory of Heat),[9] in which he based his reasoning on
Newton's_law_of_cooling, namely, that the flow of heat between two adjacent
molecules is proportional to the extremely small difference of their
temperatures. Contained in this book was Fourier's proposal of his heat
equation for conductive diffusion of heat. This partial differential equation
is now taught to every student of mathematical physics.
***** Example[edit] *****
For example, in classical_mechanics, the motion of a body is described by its
position and velocity as the time value varies. Newton's_laws allow these
variables to be expressed dynamically (given the position, velocity,
acceleration and various forces acting on the body) as a differential equation
for the unknown position of the body as a function of time.
In some cases, this differential equation (called an equation_of_motion) may be
solved explicitly.
An example of modelling a real world problem using differential equations is
the determination of the velocity of a ball falling through the air,
considering only gravity and air resistance. The ball's acceleration towards
the ground is the acceleration due to gravity minus the acceleration due to air
resistance. Gravity is considered constant, and air resistance may be modeled
as proportional to the ball's velocity. This means that the ball's
acceleration, which is a derivative of its velocity, depends on the velocity
(and the velocity depends on time). Finding the velocity as a function of time
involves solving a differential equation and verifying its validity.
***** Types[edit] *****
Differential equations can be divided into several types. Apart from describing
the properties of the equation itself, these classes of differential equations
can help inform the choice of approach to a solution. Commonly used
distinctions include whether the equation is: Ordinary/Partial, Linear/Non-
linear, and Homogeneous/heterogeneous. This list is far from exhaustive; there
are many other properties and subclasses of differential equations which can be
very useful in specific contexts.
**** Ordinary differential equations[edit] ****
Main articles: Ordinary_differential_equation and Linear_differential_equation
An ordinary_differential_equation (ODE) is an equation containing an unknown
function_of_one_real_or_complex_variable x, its derivatives, and some given
functions of x. The unknown function is generally represented by a variable
(often denoted y), which, therefore, depends on x. Thus x is often called the
independent_variable of the equation. The term "ordinary" is used in contrast
with the term partial_differential_equation, which may be with respect to more
than one independent variable.
Linear_differential_equations are the differential equations that are linear in
the unknown function and its derivatives. Their theory is well developed, and,
in many cases, one may express their solutions in terms of integrals.
Most ODEs that are encountered in physics are linear, and, therefore, most
special_functions may be defined as solutions of linear differential equations
(see Holonomic_function).
As, in general, the solutions of a differential equation cannot be expressed by
a closed-form_expression, numerical_methods are commonly used for solving
differential equations on a computer.
**** Partial differential equations[edit] ****
Main article: Partial_differential_equation
A partial_differential_equation (PDE) is a differential equation that contains
unknown multivariable_functions and their partial_derivatives. (This is in
contrast to ordinary_differential_equations, which deal with functions of a
single variable and their derivatives.) PDEs are used to formulate problems
involving functions of several variables, and are either solved in closed form,
or used to create a relevant computer_model.
PDEs can be used to describe a wide variety of phenomena in nature such as
sound, heat, electrostatics, electrodynamics, fluid_flow, elasticity, or
quantum_mechanics. These seemingly distinct physical phenomena can be
formalized similarly in terms of PDEs. Just as ordinary differential equations
often model one-dimensional dynamical_systems, partial differential equations
often model multidimensional_systems. PDEs find their generalization in
stochastic_partial_differential_equations.
**** Non-linear differential equations[edit] ****
Main article: Non-linear_differential_equations
A non-linear differential equation is a differential equation that is not a
linear_equation in the unknown function and its derivatives (the linearity or
non-linearity in the arguments of the function are not considered here). There
are very few methods of solving nonlinear differential equations exactly; those
that are known typically depend on the equation having particular symmetries.
Nonlinear differential equations can exhibit very complicated behavior over
extended time intervals, characteristic of chaos. Even the fundamental
questions of existence, uniqueness, and extendability of solutions for
nonlinear differential equations, and well-posedness of initial and boundary
value problems for nonlinear PDEs are hard problems and their resolution in
special cases is considered to be a significant advance in the mathematical
theory (cf. NavierâStokes_existence_and_smoothness). However, if the
differential equation is a correctly formulated representation of a meaningful
physical process, then one expects it to have a solution.[10]
Linear differential equations frequently appear as approximations to nonlinear
equations. These approximations are only valid under restricted conditions. For
example, the harmonic oscillator equation is an approximation to the nonlinear
pendulum equation that is valid for small amplitude oscillations (see below).
**** Equation order[edit] ****
Differential equations are described by their order, determined by the term
with the highest_derivatives. An equation containing only first derivatives is
a first-order differential equation, an equation containing the second
derivative is a second-order differential equation, and so on.[11][12]
Differential equations that describe natural phenomena almost always have only
first and second order derivatives in them, but there are some exceptions, such
as the thin_film_equation, which is a fourth order partial differential
equation.
**** Examples[edit] ****
In the first group of examples, u is an unknown function of x, and c and Ï are
constants that are supposed to be known. Two broad classifications of both
ordinary and partial differential equations consists of distinguishing between
linear and nonlinear differential equations, and between homogeneous
differential_equations and heterogeneous ones.
    * heterogeneous first-order linear constant coefficient ordinary
      differential equation:
                  d u   d x    = c u +  x  2   .   {\displaystyle {\frac {du}
            {dx}}=cu+x^{2}.}  [{\frac {du}{dx}}=cu+x^{2}.]
    * Homogeneous second-order linear ordinary differential equation:
                   d  2   u   d  x  2      &#x2212; x    d u   d x    + u = 0.
            {\displaystyle {\frac {d^{2}u}{dx^{2}}}-x{\frac {du}{dx}}+u=0.}  [
            {\frac {d^{2}u}{dx^{2}}}-x{\frac {du}{dx}}+u=0.]
    * Homogeneous second-order linear constant coefficient ordinary
      differential equation describing the harmonic_oscillator:
                   d  2   u   d  x  2      +  &#x03C9;  2   u = 0.
            {\displaystyle {\frac {d^{2}u}{dx^{2}}}+\omega ^{2}u=0.}  [{\frac
            {d^{2}u}{dx^{2}}}+\omega ^{2}u=0.]
    * heterogeneous first-order nonlinear ordinary differential equation:
                  d u   d x    =  u  2   + 4.   {\displaystyle {\frac {du}
            {dx}}=u^{2}+4.}  [{\frac {du}{dx}}=u^{2}+4.]
    * Second-order nonlinear (due to sine function) ordinary differential
      equation describing the motion of a pendulum of length L:
               L     d  2   u   d  x  2      + g sin &#x2061; u = 0.
            {\displaystyle L{\frac {d^{2}u}{dx^{2}}}+g\sin u=0.}  [L{\frac {d^
            {2}u}{dx^{2}}}+g\sin u=0.]
In the next group of examples, the unknown function u depends on two variables
x and t or x and y.
    * Homogeneous first-order linear partial differential equation:
                  &#x2202; u   &#x2202; t    + t    &#x2202; u   &#x2202; x
            = 0.   {\displaystyle {\frac {\partial u}{\partial t}}+t{\frac
            {\partial u}{\partial x}}=0.}  [{\frac {\partial u}{\partial t}}+t
            {\frac {\partial u}{\partial x}}=0.]
    * Homogeneous second-order linear constant coefficient partial differential
      equation of elliptic type, the Laplace_equation:
                   &#x2202;  2   u   &#x2202;  x  2      +     &#x2202;  2   u
            &#x2202;  y  2      = 0.   {\displaystyle {\frac {\partial ^{2}u}
            {\partial x^{2}}}+{\frac {\partial ^{2}u}{\partial y^{2}}}=0.}  [
            {\frac {\partial ^{2}u}{\partial x^{2}}}+{\frac {\partial ^{2}u}
            {\partial y^{2}}}=0.]
    * Homogeneous third-order non-linear partial differential equation :
                  &#x2202; u   &#x2202; t    = 6 u    &#x2202; u   &#x2202; x
            &#x2212;     &#x2202;  3   u   &#x2202;  x  3      .
            {\displaystyle {\frac {\partial u}{\partial t}}=6u{\frac {\partial
            u}{\partial x}}-{\frac {\partial ^{3}u}{\partial x^{3}}}.}  [{\frac
            {\partial u}{\partial t}}=6u{\frac {\partial u}{\partial x}}-{\frac
            {\partial ^{3}u}{\partial x^{3}}}.]
***** Existence of solutions[edit] *****
Solving differential equations is not like solving algebraic_equations. Not
only are their solutions often unclear, but whether solutions are unique or
exist at all are also notable subjects of interest.
For first order initial value problems, the Peano_existence_theorem gives one
set of circumstances in which a solution exists. Given any point     ( a , b )
{\displaystyle (a,b)}  [(a,b)] in the xy-plane, define some rectangular region
Z   {\displaystyle Z}  [Z], such that     Z = [ l , m ] &#x00D7; [ n , p ]
{\displaystyle Z=[l,m]\times [n,p]}  [Z=[l,m]\times [n,p]] and     ( a , b )
{\displaystyle (a,b)}  [(a,b)] is in the interior of     Z   {\displaystyle Z}
[Z]. If we are given a differential equation         d  y    d  x    = g ( x ,
y )   {\displaystyle {\frac {\mathrm {d} y}{\mathrm {d} x}}=g(x,y)}  [{\frac
{\mathrm {d} y}{\mathrm {d} x}}=g(x,y)] and the condition that     y = b
{\displaystyle y=b}  [y=b] when     x = a   {\displaystyle x=a}  [x=a], then
there is locally a solution to this problem if     g ( x , y )   {\displaystyle
g(x,y)}  [g(x,y)] and        &#x2202; g   &#x2202; x      {\displaystyle {\frac
{\partial g}{\partial x}}}  [{\frac {\partial g}{\partial x}}] are both
continuous on     Z   {\displaystyle Z}  [Z]. This solution exists on some
interval with its center at     a   {\displaystyle a}  [a]. The solution may
not be unique. (See Ordinary_differential_equation for other results.)
However, this only helps us with first order initial_value_problems. Suppose we
had a linear initial value problem of the nth order:
          f  n   ( x )      d   n   y    d   x  n      + &#x22EF; +  f  1   ( x
      )     d  y    d  x    +  f  0   ( x ) y = g ( x )   {\displaystyle f_{n}
      (x){\frac {\mathrm {d} ^{n}y}{\mathrm {d} x^{n}}}+\cdots +f_{1}(x){\frac
      {\mathrm {d} y}{\mathrm {d} x}}+f_{0}(x)y=g(x)}  [f_{n}(x){\frac {\mathrm
      {d} ^{n}y}{\mathrm {d} x^{n}}}+\cdots +f_{1}(x){\frac {\mathrm {d} y}
      {\mathrm {d} x}}+f_{0}(x)y=g(x)]
such that
         y (  x  0   ) =  y  0   ,  y &#x2032;  (  x  0   ) =  y  0  &#x2032;
      ,  y &#x2033;  (  x  0   ) =  y  0  &#x2033;  , &#x22EF;   {\displaystyle
      y(x_{0})=y_{0},y'(x_{0})=y'_{0},y''(x_{0})=y''_{0},\cdots }  [y(x_{0})=y_
      {0},y'(x_{0})=y'_{0},y''(x_{0})=y''_{0},\cdots ]
For any nonzero      f  n   ( x )   {\displaystyle f_{n}(x)}  [f_{{n}}(x)], if
{  f  0   ,  f  1   , &#x22EF; }   {\displaystyle \{f_{0},f_{1},\cdots \}}  [\
{f_{0},f_{1},\cdots \}] and     g   {\displaystyle g}  [g] are continuous on
some interval containing      x  0     {\displaystyle x_{0}}  [x_{0}],     y
{\displaystyle y}  [y] is unique and exists.[13]
***** Related concepts[edit] *****
    * A delay_differential_equation (DDE) is an equation for a function of a
      single variable, usually called time, in which the derivative of the
      function at a certain time is given in terms of the values of the
      function at earlier times.
    * An integro-differential_equation (IDE) is an equation that combines
      aspects of a differential equation and an integral_equation.
    * A stochastic_differential_equation (SDE) is an equation in which the
      unknown quantity is a stochastic_process and the equation involves some
      known stochastic processes, for example, the Wiener_process in the case
      of diffusion equations.
    * A differential_algebraic_equation (DAE) is a differential equation
      comprising differential and algebraic terms, given in implicit form.
***** Connection to difference equations[edit] *****
See also: Time_scale_calculus
The theory of differential equations is closely related to the theory of
difference_equations, in which the coordinates assume only discrete values, and
the relationship involves values of the unknown function or functions and
values at nearby coordinates. Many methods to compute numerical solutions of
differential equations or study the properties of differential equations
involve the approximation of the solution of a differential equation by the
solution of a corresponding difference equation.
***** Applications[edit] *****
The study of differential equations is a wide field in pure and applied
mathematics, physics, and engineering. All of these disciplines are concerned
with the properties of differential equations of various types. Pure
mathematics focuses on the existence and uniqueness of solutions, while applied
mathematics emphasizes the rigorous justification of the methods for
approximating solutions. Differential equations play an important role in
modeling virtually every physical, technical, or biological process, from
celestial motion, to bridge design, to interactions between neurons.
Differential equations such as those used to solve real-life problems may not
necessarily be directly solvable, i.e. do not have closed_form solutions.
Instead, solutions can be approximated using numerical_methods.
Many fundamental laws of physics and chemistry can be formulated as
differential equations. In biology and economics, differential equations are
used to model the behavior of complex systems. The mathematical theory of
differential equations first developed together with the sciences where the
equations had originated and where the results found application. However,
diverse problems, sometimes originating in quite distinct scientific fields,
may give rise to identical differential equations. Whenever this happens,
mathematical theory behind the equations can be viewed as a unifying principle
behind diverse phenomena. As an example, consider the propagation of light and
sound in the atmosphere, and of waves on the surface of a pond. All of them may
be described by the same second-order partial_differential_equation, the wave
equation, which allows us to think of light and sound as forms of waves, much
like familiar waves in the water. Conduction of heat, the theory of which was
developed by Joseph_Fourier, is governed by another second-order partial
differential equation, the heat_equation. It turns out that many diffusion
processes, while seemingly different, are described by the same equation; the
BlackâScholes equation in finance is, for instance, related to the heat
equation.
**** Pure Mathematics[edit] ****
    * Ricci_flow - used to prove the PoincarÃ©_conjecture
**** Physics[edit] ****
    * EulerâLagrange_equation in classical mechanics
    * Hamilton's_equations in classical mechanics
    * Radioactive_decay in nuclear_physics
    * Newton's_law_of_cooling in thermodynamics
    * n-body_problem in celestial_mechanics
    * The wave_equation
    * The heat_equation in thermodynamics
    * Laplace's_equation, which defines harmonic_functions
    * Poisson's_equation
    * The geodesic_equation
    * The NavierâStokes_equations in fluid_dynamics
          o Euler_equations
          o Burgers'_equation
    * The continuity_equation for conservation laws in electromagnetism, fluid
      dynamics, and thermodynamics
    * The Diffusion_equation in stochastic_processes
    * The Convectionâdiffusion_equation in fluid dynamics
    * The CauchyâRiemann_equations in complex_analysis
    * The PoissonâBoltzmann_equation in molecular_dynamics
    * The shallow_water_equations
    * Universal_differential_equation
    * The Lorenz_equations whose solutions exhibit chaotic flow.
    * KdV_equation in fluid dynamics and plasma_physics
    * Potential_vorticity in geophysical_fluid_dynamics
    * Nonlinear_SchrÃ¶dinger_equation in quantum mechanics, water_waves, and
      fiber_optics
    * Eikonal_equation in wave_propagation
    * Wave_action in continuum_mechanics
*** Classical mechanics[edit] ***
So long as the force acting on a particle is known, Newton's_second_law is
sufficient to describe the motion of a particle. Once independent relations for
each force acting on a particle are available, they can be substituted into
Newton's second law to obtain an ordinary_differential_equation, which is
called the equation of motion.
*** Electrodynamics[edit] ***
Maxwell's_equations are a set of partial_differential_equations that, together
with the Lorentz_force law, form the foundation of classical_electrodynamics,
classical optics, and electric_circuits. These fields in turn underlie modern
electrical and communications technologies. Maxwell's equations describe how
electric and magnetic_fields are generated and altered by each other and by
charges and currents. They are named after the Scottish physicist and
mathematician James_Clerk_Maxwell, who published an early form of those
equations between 1861 and 1862.
*** General relativity[edit] ***
The Einstein_field_equations (EFE; also known as "Einstein's equations") are a
set of ten partial_differential_equations in Albert_Einstein's general_theory
of_relativity which describe the fundamental_interaction of gravitation as a
result of spacetime being curved by matter and energy.[14] First published by
Einstein in 1915[15] as a tensor_equation, the EFE equate local spacetime
curvature (expressed by the Einstein_tensor) with the local energy and momentum
within that spacetime (expressed by the stressâenergy_tensor).[16]
*** Quantum mechanics[edit] ***
In quantum mechanics, the analogue of Newton's law is SchrÃ¶dinger's_equation
(a partial differential equation) for a quantum system (usually atoms,
molecules, and subatomic particles whether free, bound, or localized). It is
not a simple algebraic equation, but in general a linear partial_differential
equation, describing the time-evolution of the system's wave_function (also
called a "state function").[17]
**** Engineering[edit] ****
    * Van_der_Pol_oscillator
    * Potential_flow
    * Reynolds-averaged_Navier-Stokes (RANS)
    * Turbulence_kinetic_energy (TKE)
    * Reynolds_transport_theorem
    * Vorticity_equation
    * RayleighâPlesset_equation
    * Acoustic_theory
    * Groundwater_flow_equation
          o Richards_equation
    * Blasius_boundary_layer
    * Optimal_control
          o Linear-quadratic_regulator
    * Total_variation_denoising (Rudin-Osher-Fatemi[18])
    * Magnetohydrodynamics
    * Spherical_harmonics
          o Associated_Legendre_polynomials
    * Elasticity
          o Euler-Bernoulli_beam_theory
          o Timoshenko_beam_theory
    * Neutron diffusion[19]
    * Telegrapher's_equations
    * Buckley-Leverett_equation
    * Traffic_flow
**** Biology and Medicine[edit] ****
    * Allee_effect - population ecology
    * McKendrickâvon_Foerster_equation - age_structure modeling
    * Replicator_dynamics â found in theoretical_biology and evolutionary
      linguistics
    * Verhulst_equation â biological population growth
    * von_Bertalanffy_model â biological individual growth
    * HodgkinâHuxley_model â neural action potentials
    * Nernst-Planck_equation - ion flux across biological membranes
    * HagenâPoiseuille_equation - blood flow
    * Compartmental_models - epidemiology
          o SIR model
          o SIS model
    * Reaction-diffusion_equation - theoretical biology
          o Fisher-KPP_equation - nonlinear traveling waves
          o Fitzhugh-Nagumo - neural activation
*** Predator-prey equations[edit] ***
The LotkaâVolterra_equations, also known as the predatorâprey equations,
are a pair of first-order, non-linear, differential equations frequently used
to describe the population_dynamics of two species that interact, one as a
predator and the other as prey.
**** Chemistry[edit] ****
The rate law or rate_equation for a chemical_reaction is a differential
equation that links the reaction_rate with concentrations or pressures of
reactants and constant parameters (normally rate coefficients and partial
reaction_orders).[20] To determine the rate equation for a particular system
one combines the reaction rate with a mass_balance for the system.[21] In
addition, a range of differential equations are present in the study of
thermodynamics and quantum_mechanics.
**** Economics and Finance[edit] ****
    * Sovereign_debt accumulation
          o         D &#x02D9;   &#x23DF;    Change in Debt   =     r D
            &#x23DF;    Interest on Debt   +     G ( t ) &#x2212; T ( t )
            &#x23DF;    Net Borrowing     {\textstyle \underbrace {\dot {D}} _
            {\text{Change in Debt}}=\underbrace {rD} _{\text{Interest on
            Debt}}+\underbrace {G(t)-T(t)} _{\text{Net Borrowing}}}  [
            {\textstyle \underbrace {\dot {D}} _{\text{Change in
            Debt}}=\underbrace {rD} _{\text{Interest on Debt}}+\underbrace {G
            (t)-T(t)} _{\text{Net Borrowing}}}]
    * Economic_growth
          o SolowâSwan_model
                #     k &#x2032;  ( t ) = s [ k ( t )  ]  &#x03B1;   &#x2212;
                  &#x03B4; k ( t )   {\textstyle k'(t)=s[k(t)]^{\alpha }-\delta
                  k(t)}  [{\textstyle k'(t)=s[k(t)]^{\alpha }-\delta k(t)}]
          o Ramsey-Cass-Koopmans_model
          o Dynamic_stochastic_general_equilibrium[22]
    * Stochastic Differential Equations
          o Geometric_Brownian_Motion
          o Ornstein-Uhlenbeck_Process
          o Cox-Ingersoll-Ross_model
    * Hamilton-Jacobi-Bellman_equation
          o Merton's_portfolio_problem
    * Feynman-Kac_formula
          o BlackâScholes_equation
          o Affine_term_structure_modeling[23]
    * Fokker-Planck_equation
          o Dupire equation (local_volatility)
    * Malthusian_growth_model
    * The_VidaleâWolfe_advertising_model
    * Bass_diffusion_model
***** See also[edit] *****
    * Complex_differential_equation
    * Exact_differential_equation
    * Functional_differential_equation
    * Initial_condition
    * Integral_equations
    * Numerical_methods_for_solving_differential_equations
    * PicardâLindelÃ¶f_theorem on existence and uniqueness of solutions
    * Recurrence_relation, also known as 'difference equation'
    * Abstract_differential_equation
***** References[edit] *****
   1. ^ Newton, Isaac. (c.1671). Methodus Fluxionum et Serierum Infinitarum
      (The Method of Fluxions and Infinite Series), published in 1736
      [Opuscula, 1744, Vol. I. p. 66].
   2. ^Bernoulli,_Jacob (1695), "Explicationes, Annotationes & Additiones ad
      ea, quae in Actis sup. de Curva Elastica, Isochrona Paracentrica, &
      Velaria, hinc inde memorata, & paratim controversa legundur; ubi de Linea
      mediarum directionum, alliisque novis", Acta_Eruditorum
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
   4. ^Hairer, Ernst; NÃ¸rsett, Syvert Paul; Wanner, Gerhard (1993), Solving
      ordinary differential equations I: Nonstiff problems, Berlin, New York:
      Springer-Verlag, ISBN 978-3-540-56670-0
   5. ^ Cannon,_John_T.;_Dostrovsky,_Sigalia_(1981)._"The_evolution_of
      dynamics,_vibration_theory_from_1687_to_1742"._Studies_in_the_History_of
      Mathematics_and_Physical_Sciences._6._New_York:_Springer-Verlag:_ix_+_184
      pp.ISBN 0-3879-0626-6.
   6. GRAY, JW (July 1983). "BOOK REVIEWS". Bulletin (New Series) of the
      American Mathematical Society. 9 (1).
   7.  (retrieved 13 Nov 2012).
   8. ^Wheeler, Gerard F.; Crummett, William P. (1987). "The Vibrating String
      Controversy". Am._J._Phys. 55 (1): 33â37. Bibcode:1987AmJPh..55...33W.
      doi:10.1119/1.15311.
   9. ^ For a special collection of the 9 groundbreaking papers by the three
      authors, see First_Appearance_of_the_wave_equation:_D'Alembert,_Leonhard
      Euler,_Daniel_Bernoulli._-_the_controversy_about_vibrating_strings
      (retrieved 13 Nov 2012). Herman HJ Lynge and Son.
  10. ^ For de Lagrange's contributions to the acoustic wave equation, can
      consult Acoustics:_An_Introduction_to_Its_Physical_Principles_and
      Applications Allan D. Pierce, Acoustical Soc of America, 1989; page 18.
      (retrieved 9 Dec 2012)
  11. ^ Speiser, David. Discovering_the_Principles_of_Mechanics_1600-1800, p.
      191 (Basel: BirkhÃ¤user, 2008).
  12. ^Fourier, Joseph (1822). ThÃ©orie_analytique_de_la_chaleur (in French).
      Paris: Firmin Didot PÃ¨re et Fils. OCLC 2688081.
  13. ^Boyce, William E.; DiPrima, Richard C. (1967). Elementary Differential
      Equations and Boundary Value Problems (4th ed.). John Wiley & Sons. p. 3.
  14. ^ Weisstein,_Eric_W. "Ordinary Differential Equation Order." From
      MathWorld--A Wolfram Web Resource. http://mathworld.wolfram.com/
      OrdinaryDifferentialEquationOrder.html
  15. ^ Order_and_degree_of_a_differential_equation, accessed Dec 2015.
  16. ^Zill, Dennis G. A First Course in Differential Equations (5th ed.).
      Brooks/Cole. ISBN 0-534-37388-7.
  17. ^Einstein, Albert (1916). "The_Foundation_of_the_General_Theory_of
      Relativity". Annalen_der_Physik. 354 (7): 769. Bibcode:
      1916AnP...354..769E. doi:10.1002/andp.19163540702. Archived from the
      original (PDF) on 2006-08-29.
  18. ^Einstein,_Albert (November 25, 1915). "Die_Feldgleichungen_der
      Gravitation". Sitzungsberichte der Preussischen Akademie der
      Wissenschaften zu Berlin: 844â847. Retrieved 2006-09-12.
  19. ^Misner,_Charles_W.; Thorne,_Kip_S.; Wheeler,_John_Archibald (1973).
      Gravitation. San Francisco: W._H._Freeman. ISBN 978-0-7167-0344-0
  20.  Chapter 34, p. 916.
  21. ^Griffiths, David J. (2004), Introduction to Quantum Mechanics (2nd ed.),
      Prentice Hall, pp. 1â2, ISBN 0-13-111892-7
  22. ^Rudin, Leonid I.; Osher, Stanley; Fatemi, Emad (1992). "Nonlinear_total
      variation_based_noise_removal_algorithms". Physica D. 60: 259â268.
  23. ^Ragheb, M. (2017). "Neutron_Diffusion_Theory" (PDF).
  24. ^ IUPAC_Gold_Book_definition_of_rate_law. See also: According to IUPAC
      Compendium_of_Chemical_Terminology.
  25. ^ Kenneth A. Connors Chemical Kinetics, the study of reaction rates in
      solution, 1991, VCH Publishers.
  26. ^FernÃ¡ndez-Villaverde, JesÃºs (2010). "The_econometrics_of_DSGE_models"
      (PDF). SERIEs. 1: 3â49.
  27. ^Piazzesi, Monika (2010). "Affine_Term_Structure_Models" (PDF).
***** Further reading[edit] *****
    * Abbott, P.; Neill, H. (2003). Teach Yourself Calculus. pp. 266â277.
Blanchard, P.; Devaney,_R._L.; Hall, G. R. (2006). Differential Equations.
Thompson.
Coddington, E. A.; Levinson, N. (1955). Theory of Ordinary Differential
Equations. McGraw-Hill.
Ince, E. L. (1956). Ordinary Differential Equations. Dover.
Johnson,, W. (1913). A_Treatise_on_Ordinary_and_Partial_Differential_Equations.
John Wiley and Sons.
 In University_of_Michigan_Historical_Math_Collection
Polyanin, A. D.; Zaitsev, V. F. (2003). Handbook of Exact Solutions for
Ordinary Differential Equations (2nd ed.). Boca Raton: Chapman & Hall/CRC
Press. ISBN 1-58488-297-2.
Porter, R. I. (1978). "XIX Differential Equations". Further Elementary
Analysis.
Teschl,_Gerald (2012). Ordinary_Differential_Equations_and_Dynamical_Systems.
Providence: American_Mathematical_Society. ISBN 978-0-8218-8328-0.
Daniel Zwillinger (12 May 2014). Handbook_of_Differential_Equations. Elsevier
Science. ISBN 978-1-4832-6396-0.
***** External links[edit] *****
 Wikiquote has quotations related to: Differential_equation
 Wikibooks has a book on the topic of: Ordinary_Differential_Equations
 Wikiversity has learning resources about Differential_equations
 Wikisource has the text of the 1911_EncyclopÃ¦dia_Britannica article
 Differential_Equation.
    *  Media related to Differential_equations at Wikimedia Commons
    * Lectures_on_Differential_Equations MIT Open CourseWare Videos
    * Online_Notes_/_Differential_Equations Paul Dawkins, Lamar_University
    * Differential_Equations, S.O.S. Mathematics
    * Introduction_to_modeling_via_differential_equations Introduction to
      modeling by means of differential equations, with critical remarks.
    * Mathematical_Assistant_on_Web Symbolic ODE tool, using Maxima
    * Exact_Solutions_of_Ordinary_Differential_Equations
    * Collection_of_ODE_and_DAE_models_of_physical_systems MATLAB models
    * Notes_on_Diffy_Qs:_Differential_Equations_for_Engineers An introductory
      textbook on differential equations by Jiri Lebl of UIUC
    * Khan_Academy_Video_playlist_on_differential_equations Topics covered in a
      first year course in differential equations.
    * MathDiscuss_Video_playlist_on_differential_equations
    * v
    * t
    * e
Areas_of_mathematics
                  * Category_theory
                  * Information_theory
Foundations       * Mathematical_logic
                  * Philosophy_of_mathematics
                  * Set_theory
                  * Abstract
Algebra           * Elementary
                  * Linear
                  * Multilinear
                  * Calculus
                  * Real_analysis
Analysis          * Complex_analysis
                  * Differential equations
                  * Functional_analysis
                  * Combinatorics
Discrete          * Graph_theory
                  * Order_theory
                  * Game_theory
                  * Algebraic
                  * Analytic
Geometry          * Differential
                  * Discrete
                  * Euclidean
                  * Finite
                  * Arithmetic
Number_theory     * Algebraic_number_theory
                  * Analytic_number_theory
                  * Diophantine_geometry
                  * Algebraic
Topology          * Differential
                  * Geometric
                  * Control_theory
                  * Mathematical_economics
                  * Mathematical_finance
Applied           * Mathematical_physics
                  * Mathematical_statistics
                  * Probability
                  * Statistics
                  * Computer_science
                  * Theory_of_computation
Computational     * Numerical_analysis
                  * Optimization
                  * Computer_algebra
                  * History_of_mathematics
Others            * Recreational_mathematics
                  * Mathematics_and_art
                  * Mathematics_education
    * [Category] Category
    * [Portal] Portal
    * [Commons page]Commons
    * [WikiProject]WikiProject
    * v
    * t
    * e
Differential equations
                                           * Differential_operator
                                           * Notation_for_differentiation
                                           * Ordinary
                                           * Partial
               Operations                  * Differential-algebraic
                                           * Integro-differential
                                           * Fractional
                                           * Linear
                                           * Non-linear
                                           * Dependent_and_independent_variables
Classification                             * Homogeneous
                                           * Nonhomogeneous
                                           * Coupled
               Attributes of variables     * Decoupled
                                           * Order
                                           * Degree
                                           * Autonomous
                                           * Exact_differential_equation
                                           * Complex_differential_equation
                                           * Difference (discrete analogue)
               Relation to processes       * stochastic
                                           * Delay
                            * PicardâLindelÃ¶f_theorem (existence and uniqueness)
                            * Wronskian
                            * Phase_portrait
                            * Phase_space
                            * Lyapunov_stability
               Solution     * Asymptotic_stability
               topics       * Exponential_stability
                            * Rate_of_convergence
                            * Series_solutions
                            * Integral solutions
                            * Numerical_integration
                            * Dirac_delta_function
Solutions                   * Inspection
                            * Separation_of_variables                                    [Elmer-pump-
                            * Method_of_undetermined_coefficients                        heatequation.png]
                            * Variation_of_parameters
                            * Integrating_factor
                            * Integral_transforms
               Solution     * Euler_method
               methods      * Finite_difference_method
                            * CrankâNicolson_method
                            * RungeâKutta_methods
                            * Finite_element_method
                            * Finite_volume_method
                            * Galerkin_method
                            * Perturbation_theory
                   * Astronomy
                   * Physics
                   * Continuum_mechanics
                   * Chaos_theory
Applications       * Chemistry
                   * Dynamical_system
                   * Economics
                   * Biology
                   * Geology
                   * Population_dynamics
                   * Isaac_Newton
                   * Gottfried_Wilhelm_Leibniz
                   * Leonhard_Euler
                   * Jacob_Bernoulli
                   * Ãmile_Picard
                   * JÃ³zef_Maria_Hoene-WroÅski
Mathematicians     * Ernst_LindelÃ¶f
                   * Rudolf_Lipschitz
                   * Joseph-Louis_Lagrange
                   * Augustin-Louis_Cauchy
                   * John_Crank
                   * Phyllis_Nicolson
                   * Carl_David_TolmÃ©_Runge
                   * Martin_Kutta
                                              * GND: 4012249-9
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85037890
                                              * NDL: 00560651

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Differential_equation&oldid=909965002"
Categories:
    * Differential_equations
Hidden categories:
    * CS1_French-language_sources_(fr)
    * CS1:_JulianâGregorian_uncertainty
    * Articles_with_inconsistent_citation_formats
    * Articles_lacking_in-text_citations_from_August_2009
    * All_articles_lacking_in-text_citations
    * Commons_category_link_is_on_Wikidata
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
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
    * Wikiquote
    * Wikiversity
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Afrikaans
    * Alemannisch
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AragonÃ©s
    * Asturianu
    * à¦¬à¦¾à¦à¦²à¦¾
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÐ°ÑÒ¡Ð¾ÑÑÑÐ°
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * Ð§ÓÐ²Ð°ÑÐ»Ð°
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * Fiji_Hindi
    * FranÃ§ais
    * Gaeilge
    * Galego
    * è´èª
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * KurdÃ®
    * Latina
    * LatvieÅ¡u
    * ÐÐµÐ·Ð³Ð¸
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Malti
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Occitan
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Ù¾ÙØ¬Ø§Ø¨Û
    * Patois
    * áá¶áá¶ááááá
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * Qaraqalpaqsha
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * à·à·à¶à·à¶½
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * TÃ¼rkmenÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * Winaray
    * å´è¯­
    * ××Ö´×××©
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 8 August 2019, at 19:46 (UTC).
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
