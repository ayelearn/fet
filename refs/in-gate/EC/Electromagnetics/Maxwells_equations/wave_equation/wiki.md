The following text has been accessed from https://en.wikipedia.org/wiki/Wave_equation at Fri Aug 9 03:43:31 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Wave equation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Second-order linear differential equation important in physics
Not to be confused with Wave_function.
A pulse traveling through a string with fixed endpoints as modeled by the wave
equation.
Spherical waves coming from a point source.
A solution to the 2D wave equation
The wave equation is an important second-order linear partial_differential
equation for the description of wavesâas they occur in classical
physicsâsuch as mechanical_waves (e.g. water waves, sound_waves and seismic
waves) or light waves. It arises in fields like acoustics, electromagnetics,
and fluid_dynamics.
Historically, the problem of a vibrating_string such as that of a musical
instrument was studied by Jean_le_Rond_d'Alembert, Leonhard_Euler, Daniel
Bernoulli, and Joseph-Louis_Lagrange.[1][2][3][4] In 1746, dâAlembert
discovered the one-dimensional wave equation, and within ten years Euler
discovered the three-dimensional wave equation.[5]
⁰
***** Contents *****
    * 1_Introduction
    * 2_Wave_equation_in_one_space_dimension
          o 2.1_Derivation_of_the_wave_equation
                # 2.1.1_From_Hooke's_law
                # 2.1.2_Stress_pulse_in_a_bar
          o 2.2_General_solution
                # 2.2.1_Algebraic_approach
                # 2.2.2_Plane_wave_eigenmodes
    * 3_Scalar_wave_equation_in_three_space_dimensions
          o 3.1_Spherical_waves
                # 3.1.1_Monochromatic_spherical_wave
          o 3.2_Solution_of_a_general_initial-value_problem
    * 4_Scalar_wave_equation_in_two_space_dimensions
    * 5_Scalar_wave_equation_in_general_dimension_and_Kirchhoff's_formulae
          o 5.1_Odd_dimensions
          o 5.2_Even_dimensions
    * 6_Problems_with_boundaries
          o 6.1_One_space_dimension
                # 6.1.1_The_SturmâLiouville_formulation
                # 6.1.2_Investigation_by_numerical_methods
          o 6.2_Several_space_dimensions
    * 7_Inhomogeneous_wave_equation_in_one_dimension
    * 8_Other_coordinate_systems
    * 9_Further_generalizations
          o 9.1_Elastic_waves
          o 9.2_Dispersion_relation
    * 10_See_also
    * 11_Notes
    * 12_References
    * 13_External_links
***** Introduction[edit] *****
The wave equation is a partial_differential_equation that may constrain some
scalar function u = u (x1, x2, …, xn; t) of a time variable t and one or more
spatial variables x1, x2, … xn. The quantity u may be, for example, the
pressure in a liquid or gas, or the displacement, along some specific
direction, of the particles of a vibrating solid away from their resting
positions. The equation is
             &#x2202;  2   u   &#x2202;  t  2       =   c  2
      (       &#x2202;  2   u   &#x2202;  x  1   2      +     &#x2202;  2   u
      &#x2202;  x  2   2      + &#x22EF; +     &#x2202;  2   u   &#x2202;  x  n
      2        )     {\displaystyle {\frac {\partial ^{2}u}{\partial t^
      {2}}}\;=\;c^{2}{\bigl (}{\frac {\partial ^{2}u}{\partial x_{1}^{2}}}+
      {\frac {\partial ^{2}u}{\partial x_{2}^{2}}}+\cdots +{\frac {\partial ^
      {2}u}{\partial x_{n}^{2}}}{\bigr )}}  [{\displaystyle {\frac {\partial ^
      {2}u}{\partial t^{2}}}\;=\;c^{2}{\bigl (}{\frac {\partial ^{2}u}{\partial
      x_{1}^{2}}}+{\frac {\partial ^{2}u}{\partial x_{2}^{2}}}+\cdots +{\frac
      {\partial ^{2}u}{\partial x_{n}^{2}}}{\bigr )}}]
where c is a fixed non-negative real coefficient.
Using the notations of Newtonian_mechanics and vector_calculus, the wave
equation can be written more compactly as
            u &#x00A8;    =  c  2    &#x2207;  2   u   {\displaystyle {\ddot
      {u}}=c^{2}\nabla ^{2}u}  [{\displaystyle {\ddot {u}}=c^{2}\nabla ^{2}u}]
where         &#x25FB;  &#x00A8;      {\displaystyle {\ddot {\scriptstyle
\square }}}  [{\displaystyle {\ddot {\scriptstyle \square }}}] denotes double
time derivative, â is the nabla_operator, and â2 = â Â· â is the
(spatial) Laplacian_operator:
      u &#x00A8;    =     &#x2202;  2   u   &#x2202;  t  2        &#x2207; =
(     &#x2202;  &#x2202;  x  1      ,   &#x2202;  &#x2202;  x  2      ,
&#x2026; ,   &#x2202;  &#x2202;  x  n        )      &#x2207;  2   =    &#x2202;
2    &#x2202;  x  1   2      +    &#x2202;  2    &#x2202;  x  2   2      +
&#x22EF; +    &#x2202;  2    &#x2202;  x  n   2        {\displaystyle {\ddot
{u}}={\frac {\partial ^{2}u}{\partial t^{2}}}\quad \quad \nabla ={\bigl (}
{\frac {\partial }{\partial x_{1}}},{\frac {\partial }{\partial x_{2}}},\ldots
,{\frac {\partial }{\partial x_{n}}}{\bigr )}\quad \quad \nabla ^{2}={\frac
{\partial ^{2}}{\partial x_{1}^{2}}}+{\frac {\partial ^{2}}{\partial x_{2}^
{2}}}+\cdots +{\frac {\partial ^{2}}{\partial x_{n}^{2}}}}  [{\displaystyle
{\ddot {u}}={\frac {\partial ^{2}u}{\partial t^{2}}}\quad \quad \nabla ={\bigl
(}{\frac {\partial }{\partial x_{1}}},{\frac {\partial }{\partial x_
{2}}},\ldots ,{\frac {\partial }{\partial x_{n}}}{\bigr )}\quad \quad \nabla ^
{2}={\frac {\partial ^{2}}{\partial x_{1}^{2}}}+{\frac {\partial ^{2}}{\partial
x_{2}^{2}}}+\cdots +{\frac {\partial ^{2}}{\partial x_{n}^{2}}}}]
A solution of this equation can be quite complicated, but it can be analyzed as
a linear combination of simple solutions that are sinusoidal plane_waves with
various directions of propagation and wavelengths but all with the same
propagation speed c. This analysis is possible because the wave equation is
linear; so that any multiple of a solution is also a solution, and the sum of
any two solutions is again a solution. This property is called the
superposition_principle in physics.
The wave equation alone does not specify a physical solution; a unique solution
is usually obtained by setting a problem with further conditions, such as
initial_conditions, which prescribe the amplitude and phase of the wave.
Another important class of problems occurs in enclosed spaces specified by
boundary_conditions, for which the solutions represent standing_waves, or
harmonics, analogous to the harmonics of musical instruments.
The wave equation is the simplest example of a hyperbolic_differential
equation. It, and its modifications, play fundamental roles in continuum
mechanics, quantum_mechanics, plasma_physics, general_relativity, geophysics,
and many other scientific and technical disciplines.
***** Wave equation in one space dimension[edit] *****
French scientist Jean-Baptiste_le_Rond_d'Alembert (b. 1717) discovered the wave
equation in one space dimension.[5]
The wave equation in one space dimension can be written as follows:
             &#x2202;  2   u   &#x2202;  t  2      =  c  2       &#x2202;  2
      u   &#x2202;  x  2        {\displaystyle {\partial ^{2}u \over \partial
      t^{2}}=c^{2}{\partial ^{2}u \over \partial x^{2}}}  [{\displaystyle
      {\partial ^{2}u \over \partial t^{2}}=c^{2}{\partial ^{2}u \over \partial
      x^{2}}}].
This equation is typically described as having only one space dimension x,
because the only other independent_variable is the time t. Nevertheless, the
dependent_variable u may represent a second space dimension, if, for example,
the displacement u takes place in y-direction, as in the case of a string that
is located in the xây plane.
**** Derivation of the wave equation[edit] ****
The wave equation in one space dimension can be derived in a variety of
different physical settings. Most famously, it can be derived for the case of a
string that is vibrating in a two-dimensional plane, with each of its elements
being pulled in opposite directions by the force of tension.[6]
Another physical setting for derivation of the wave equation in one space
dimension utilizes Hooke's_Law. In the theory_of_elasticity, Hooke's Law is an
approximation for certain materials, stating that the amount by which a
material body is deformed (the strain) is linearly related to the force causing
the deformation (the stress).
*** From Hooke's law[edit] ***
The wave equation in the one-dimensional case can be derived from Hooke's Law
in the following way: Imagine an array of little weights of mass m
interconnected with massless springs of length h. The springs have a spring
constant of k:
      [Array_of_masses.svg]
Here the dependent variable u(x) measures the distance from the equilibrium of
the mass situated at x, so that u(x) essentially measures the magnitude of a
disturbance (i.e. strain) that is traveling in an elastic material. The forces
exerted on the mass m at the location x + h are:
              F   N e w t o n       = m &#x22C5; a ( t ) = m &#x22C5;
      &#x2202;  2    &#x2202;  t  2      u ( x + h , t )      F   H o o k e
      =  F  x + 2 h   &#x2212;  F  x   = k  [  u ( x + 2 h , t ) &#x2212; u ( x
      + h , t )  ]  &#x2212; k [ u ( x + h , t ) &#x2212; u ( x , t ) ]
      {\displaystyle {\begin{aligned}F_{\rm {Newton}}&=m\cdot a(t)=m\cdot
      {\frac {\partial ^{2}}{\partial t^{2}}}u(x+h,t)\\F_{\rm {Hooke}}&=F_
      {x+2h}-F_{x}=k\left[{u(x+2h,t)-u(x+h,t)}\right]-k[u(x+h,t)-u(x,t)]\end
      {aligned}}}  [{\displaystyle {\begin{aligned}F_{\rm {Newton}}&=m\cdot a
      (t)=m\cdot {\frac {\partial ^{2}}{\partial t^{2}}}u(x+h,t)\\F_{\rm
      {Hooke}}&=F_{x+2h}-F_{x}=k\left[{u(x+2h,t)-u(x+h,t)}\right]-k[u(x+h,t)-u
      (x,t)]\end{aligned}}}]
The equation of motion for the weight at the location x + h is given by
equating these two forces:
            &#x2202;  2    &#x2202;  t  2      u ( x + h , t ) =   k m   [ u
      ( x + 2 h , t ) &#x2212; u ( x + h , t ) &#x2212; u ( x + h , t ) + u ( x
      , t ) ]   {\displaystyle {\partial ^{2} \over \partial t^{2}}u(x+h,t)={k
      \over m}[u(x+2h,t)-u(x+h,t)-u(x+h,t)+u(x,t)]}  [{\displaystyle {\partial
      ^{2} \over \partial t^{2}}u(x+h,t)={k \over m}[u(x+2h,t)-u(x+h,t)-u
      (x+h,t)+u(x,t)]}]
where the time-dependence of u(x) has been made explicit.
If the array of weights consists of N weights spaced evenly over the length L =
Nh of total mass M = Nm, and the total spring_constant of the array K = k/N we
can write the above equation as:
            &#x2202;  2    &#x2202;  t  2      u ( x + h , t ) =    K  L  2
      M      u ( x + 2 h , t ) &#x2212; 2 u ( x + h , t ) + u ( x , t )   h  2
      .   {\displaystyle {\partial ^{2} \over \partial t^{2}}u(x+h,t)={KL^{2}
      \over M}{u(x+2h,t)-2u(x+h,t)+u(x,t) \over h^{2}}.}  [{\displaystyle
      {\partial ^{2} \over \partial t^{2}}u(x+h,t)={KL^{2} \over M}{u(x+2h,t)-
      2u(x+h,t)+u(x,t) \over h^{2}}.}]
Taking the limit N â â, h â 0 and assuming smoothness one gets:
             &#x2202;  2   u ( x , t )   &#x2202;  t  2      =    K  L  2    M
      &#x2202;  2   u ( x , t )   &#x2202;  x  2      ,   {\displaystyle
      {\partial ^{2}u(x,t) \over \partial t^{2}}={KL^{2} \over M}{\partial ^
      {2}u(x,t) \over \partial x^{2}},}  [{\displaystyle {\partial ^{2}u(x,t)
      \over \partial t^{2}}={KL^{2} \over M}{\partial ^{2}u(x,t) \over \partial
      x^{2}},}]
which is from the definition of a second_derivative. KL2/M is the square of the
propagation speed in this particular case.
1-d standing wave as a superposition of two waves traveling in opposite
directions
*** Stress pulse in a bar[edit] ***
In the case of a stress pulse propagating through a beam the beam acts much
like an infinite number of springs in series and can be taken as an extension
of the equation derived for Hooke's law. A beam of constant cross-section made
from a linear elastic material has a stiffness K given by
         K =    E A  L   ,   {\displaystyle K={EA \over L},}  [{\displaystyle
      K={EA \over L},}]
Where A is the cross-sectional area and E is the Young's_modulus of the
material. The wave equation becomes
             &#x2202;  2   u ( x , t )   &#x2202;  t  2      =    E A L  M
      &#x2202;  2   u ( x , t )   &#x2202;  x  2      .   {\displaystyle
      {\partial ^{2}u(x,t) \over \partial t^{2}}={EAL \over M}{\partial ^{2}u
      (x,t) \over \partial x^{2}}.}  [{\displaystyle {\partial ^{2}u(x,t) \over
      \partial t^{2}}={EAL \over M}{\partial ^{2}u(x,t) \over \partial x^
      {2}}.}]
AL is equal to the volume of the beam and therefore
            A L  M   =   1 &#x03C1;   ,   {\displaystyle {\frac {AL}{M}}={\frac
      {1}{\rho }},}  [{\displaystyle {\frac {AL}{M}}={\frac {1}{\rho }},}]
where     &#x03C1;   {\displaystyle \rho }  [\rho ] is the density of the
material. The wave equation reduces to
             &#x2202;  2   u ( x , t )   &#x2202;  t  2      =   E &#x03C1;
      &#x2202;  2   u ( x , t )   &#x2202;  x  2      .   {\displaystyle {\frac
      {\partial ^{2}u(x,t)}{\partial t^{2}}}={E \over \rho }{\partial ^{2}u
      (x,t) \over \partial x^{2}}.}  [{\displaystyle {\frac {\partial ^{2}u
      (x,t)}{\partial t^{2}}}={E \over \rho }{\partial ^{2}u(x,t) \over
      \partial x^{2}}.}]
The speed of a stress wave in a bar is therefore         E &#x03C1;
{\displaystyle {\sqrt {\tfrac {E}{\rho }}}}  [{\displaystyle {\sqrt {\tfrac {E}
{\rho }}}}].
**** General solution[edit] ****
*** Algebraic approach[edit] ***
The one-dimensional wave equation is unusual for a partial_differential
equation in that a relatively simple general solution may be found. Defining
new variables:[7]
             &#x03BE;    = x &#x2212; c t     &#x03B7;    = x + c t
      {\displaystyle {\begin{aligned}\xi &=x-ct\\\eta &=x+ct\end{aligned}}}  [
      {\displaystyle {\begin{aligned}\xi &=x-ct\\\eta &=x+ct\end{aligned}}}]
changes the wave equation into
             &#x2202;  2   u   &#x2202; &#x03BE; &#x2202; &#x03B7;    = 0 ,
      {\displaystyle {\frac {\partial ^{2}u}{\partial \xi \partial \eta }}=0,}
      [{\displaystyle {\frac {\partial ^{2}u}{\partial \xi \partial \eta
      }}=0,}]
which leads to the general solution
         u ( &#x03BE; , &#x03B7; ) = F ( &#x03BE; ) + G ( &#x03B7; )
      {\displaystyle u(\xi ,\eta )=F(\xi )+G(\eta )}  [u(\xi, \eta) = F(\xi) +
      G(\eta)]
or equivalently:
         u ( x , t ) = F ( x &#x2212; c t ) + G ( x + c t ) .   {\displaystyle
      u(x,t)=F(x-ct)+G(x+ct).}  [{\displaystyle u(x,t)=F(x-ct)+G(x+ct).}]
In other words, solutions of the 1D wave equation are sums of a right traveling
function F and a left traveling function G. "Traveling" means that the shape of
these individual arbitrary functions with respect to x stays constant, however
the functions are translated left and right with time at the speed c. This was
derived by Jean_le_Rond_d'Alembert.[8]
Another way to arrive at this result is to note that the wave equation may be
"factored":
          [    &#x2202;  &#x2202; t    &#x2212; c   &#x2202;  &#x2202; x     ]
      [    &#x2202;  &#x2202; t    + c   &#x2202;  &#x2202; x     ]  u = 0.
      {\displaystyle \left[{\frac {\partial }{\partial t}}-c{\frac {\partial }
      {\partial x}}\right]\left[{\frac {\partial }{\partial t}}+c{\frac
      {\partial }{\partial x}}\right]u=0.}  [{\displaystyle \left[{\frac
      {\partial }{\partial t}}-c{\frac {\partial }{\partial x}}\right]\left[
      {\frac {\partial }{\partial t}}+c{\frac {\partial }{\partial
      x}}\right]u=0.}]
As a result, if we define v thus,
            &#x2202; u   &#x2202; t    + c    &#x2202; u   &#x2202; x    = v ,
      {\displaystyle {\frac {\partial u}{\partial t}}+c{\frac {\partial u}
      {\partial x}}=v,}  [{\displaystyle {\frac {\partial u}{\partial t}}+c
      {\frac {\partial u}{\partial x}}=v,}]
then
            &#x2202; v   &#x2202; t    &#x2212; c    &#x2202; v   &#x2202; x
      = 0.   {\displaystyle {\frac {\partial v}{\partial t}}-c{\frac {\partial
      v}{\partial x}}=0.}  [{\displaystyle {\frac {\partial v}{\partial t}}-c
      {\frac {\partial v}{\partial x}}=0.}]
From this, v must have the form G(x + ct), and from this the correct form of
the full solution u can be deduced.[9]
For an initial value problem, the arbitrary functions F and G can be determined
to satisfy initial conditions:
         u ( x , 0 ) = f ( x )   {\displaystyle u(x,0)=f(x)}  [{\displaystyle u
      (x,0)=f(x)}]
          u  t   ( x , 0 ) = g ( x ) .   {\displaystyle u_{t}(x,0)=g(x).}  [
      {\displaystyle u_{t}(x,0)=g(x).}]
The result is d'Alembert's_formula:
         u ( x , t ) =    f ( x &#x2212; c t ) + f ( x + c t )  2   +   1  2 c
      &#x222B;  x &#x2212; c t   x + c t   g ( s ) d s   {\displaystyle u(x,t)=
      {\frac {f(x-ct)+f(x+ct)}{2}}+{\frac {1}{2c}}\int _{x-ct}^{x+ct}g(s)ds}
      [u(x,t) = \frac{f(x-ct) + f(x+ct)}{2} + \frac{1}{2c} \int_{x-ct}^{x+ct} g
      (s) ds]
In the classical sense if f(x) â Ck and g(x) â Ckâ1 then u(t, x) â Ck.
However, the waveforms F and G may also be generalized functions, such as the
delta-function. In that case, the solution may be interpreted as an impulse
that travels to the right or the left.
The basic wave equation is a linear_differential_equation and so it will adhere
to the superposition_principle. This means that the net displacement caused by
two or more waves is the sum of the displacements which would have been caused
by each wave individually. In addition, the behavior of a wave can be analyzed
by breaking up the wave into components, e.g. the Fourier_transform breaks up a
wave into sinusoidal components.
*** Plane wave eigenmodes[edit] ***
Another way to solve for the solutions to the one-dimensional wave equation is
to first analyze its frequency eigenmodes. A so-called eigenmode is a solution
that oscillates in time with a well-defined constant angular frequency
&#x03C9;   {\displaystyle \omega }  [\omega ], with which the temporal part of
the wave function for such eigenmode takes a specific form      e  &#x2212; i
&#x03C9; t     {\displaystyle e^{-i\omega t}}  [e^{{-i\omega t}}]. The rest of
the wave function is then only dependent on the spatial variable     x
{\displaystyle x}  [x], hence amounting to separation_of_variables. Now writing
the wave function as
          u  &#x03C9;   ( x , t ) =  e  &#x2212; i &#x03C9; t   f ( x ) ,
      {\displaystyle u_{\omega }(x,t)=e^{-i\omega t}f(x),}  [u_{\omega }
      (x,t)=e^{{-i\omega t}}f(x),]
we can obtain an ordinary_differential_equation for the spatial part     f ( x
)   {\displaystyle f(x)}  [f(x)]
             &#x2202;  2    u  &#x03C9;     &#x2202;  t  2      =    &#x2202;
      2    &#x2202;  t  2       (   e  &#x2212; i &#x03C9; t   f ( x )  )  =
      &#x2212;  &#x03C9;  2    e  &#x2212; i &#x03C9; t   f ( x ) =  c  2
      &#x2202;  2    &#x2202;  x  2       (   e  &#x2212; i &#x03C9; t   f ( x
      )  )  ,   {\displaystyle {\frac {\partial ^{2}u_{\omega }}{\partial t^
      {2}}}={\frac {\partial ^{2}}{\partial t^{2}}}\left(e^{-i\omega t}f
      (x)\right)=-\omega ^{2}e^{-i\omega t}f(x)=c^{2}{\frac {\partial ^{2}}
      {\partial x^{2}}}\left(e^{-i\omega t}f(x)\right),}  [{\displaystyle
      {\frac {\partial ^{2}u_{\omega }}{\partial t^{2}}}={\frac {\partial ^{2}}
      {\partial t^{2}}}\left(e^{-i\omega t}f(x)\right)=-\omega ^{2}e^{-i\omega
      t}f(x)=c^{2}{\frac {\partial ^{2}}{\partial x^{2}}}\left(e^{-i\omega t}f
      (x)\right),}]
Therefore:
            d  2    d  x  2      f ( x ) = &#x2212;   (   &#x03C9; c   )   2
      f ( x ) ,   {\displaystyle {\frac {d^{2}}{dx^{2}}}f(x)=-\left({\frac
      {\omega }{c}}\right)^{2}f(x),}  [{\displaystyle {\frac {d^{2}}{dx^{2}}}f
      (x)=-\left({\frac {\omega }{c}}\right)^{2}f(x),}]
which is precisely an eigenvalue_equation for     f ( x )   {\displaystyle f
(x)}  [f(x)], hence the name eigenmode. It has the well-known plane_wave
solutions
         f ( x ) = A  e  &#x00B1; i k x   ,   {\displaystyle f(x)=Ae^{\pm
      ikx},}  [{\displaystyle f(x)=Ae^{\pm ikx},}]
with wave_number     k = &#x03C9;  /  c   {\displaystyle k=\omega /c}  [ k =
\omega/c ].
The total wave function for this eigenmode is then the linear combination
          u  &#x03C9;   ( x , t ) =  e  &#x2212; i &#x03C9; t    (  A  e
      &#x2212; i k x   + B  e  i k x    )  = A  e  &#x2212; i ( k x + &#x03C9;
      t )   + B  e  i ( k x &#x2212; &#x03C9; t )   ,   {\displaystyle u_
      {\omega }(x,t)=e^{-i\omega t}\left(Ae^{-ikx}+Be^{ikx}\right)=Ae^{-i
      (kx+\omega t)}+Be^{i(kx-\omega t)},}  [u_{\omega }(x,t)=e^{{-i\omega
      t}}\left(Ae^{{-ikx}}+Be^{{ikx}}\right)=Ae^{{-i(kx+\omega t)}}+Be^{{i(kx-
      \omega t)}},]
where complex numbers     A , B   {\displaystyle A,B}  [A,B] depend in general
on any initial and boundary conditions of the problem.
Eigenmodes are useful in constructing a full solution to the wave equation,
because each of them evolves in time trivially with the phase factor      e
&#x2212; i &#x03C9; t     {\displaystyle e^{-i\omega t}}  [e^{-i\omega t}]. so
that a full solution can be decomposed into an eigenmode_expansion
         u ( x , t ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;   s ( &#x03C9; )
      u  &#x03C9;   ( x , t ) d &#x03C9;   {\displaystyle u(x,t)=\int _{-\infty
      }^{\infty }s(\omega )u_{\omega }(x,t)d\omega }  [ u(x,t) = \int_{-
      \infty}^\infty s(\omega) u_\omega(x,t) d\omega ]
or in terms of the plane waves,
             u ( x , t )    =  &#x222B;  &#x2212; &#x221E;   &#x221E;    s  +
      ( &#x03C9; )  e  &#x2212; i ( k x + &#x03C9; t )   d &#x03C9; +  &#x222B;
      &#x2212; &#x221E;   &#x221E;    s  &#x2212;   ( &#x03C9; )  e  i ( k x
      &#x2212; &#x03C9; t )   d &#x03C9;       =  &#x222B;  &#x2212; &#x221E;
      &#x221E;    s  +   ( &#x03C9; )  e  &#x2212; i k ( x + c t )   d &#x03C9;
      +  &#x222B;  &#x2212; &#x221E;   &#x221E;    s  &#x2212;   ( &#x03C9; )
      e  i k ( x &#x2212; c t )   d &#x03C9;       = F ( x &#x2212; c t ) + G
      ( x + c t )       {\displaystyle {\begin{aligned}u(x,t)&=\int _{-\infty
      }^{\infty }s_{+}(\omega )e^{-i(kx+\omega t)}d\omega +\int _{-\infty }^
      {\infty }s_{-}(\omega )e^{i(kx-\omega t)}d\omega \\&=\int _{-\infty }^
      {\infty }s_{+}(\omega )e^{-ik(x+ct)}d\omega +\int _{-\infty }^{\infty }s_
      {-}(\omega )e^{ik(x-ct)}d\omega \\&=F(x-ct)+G(x+ct)\end{aligned}}}  [
      {\begin{aligned}u(x,t)&=\int _{{-\infty }}^{\infty }s_{+}(\omega )e^{{-i
      (kx+\omega t)}}d\omega +\int _{{-\infty }}^{\infty }s_{-}(\omega )e^{{i
      (kx-\omega t)}}d\omega \\&=\int _{{-\infty }}^{\infty }s_{+}(\omega )e^{
      {-ik(x+ct)}}d\omega +\int _{{-\infty }}^{\infty }s_{-}(\omega )e^{{ik(x-
      ct)}}d\omega \\&=F(x-ct)+G(x+ct)\end{aligned}}]
which is exactly in the same form as in the algebraic approach. Functions
s  &#x00B1;   ( &#x03C9; )   {\displaystyle s_{\pm }(\omega )}  [ s_\pm(\omega)
] are known as the Fourier_component and are determined by initial and boundary
conditions. This is a so-called frequency-domain method, alternative to direct
time-domain propagations, such as FDTD method, of the wave_packet     u ( x , t
)   {\displaystyle u(x,t)}  [ u(x,t) ], which is complete for representing
waves in absence of time dilations. Completeness of the Fourier expansion for
representing waves in the presence of time dilations has been challenged by
chirp wave solutions allowing for time variation of     &#x03C9;
{\displaystyle \omega }  [\omega ].[10] The chirp wave solutions seem
particularly implied by very large but previously inexplicable radar residuals
in the flyby_anomaly, and differ from the sinusoidal solutions in being
receivable at any distance only at proportionally shifted frequencies and time
dilations, corresponding to past chirp states of the source.
***** Scalar wave equation in three space dimensions[edit] *****
Swiss mathematician and physicist Leonhard_Euler (b. 1707) discovered the wave
equation in three space dimensions.[5]
A solution of the initial-value problem for the wave equation in three space
dimensions can be obtained from the corresponding solution for a spherical
wave. The result can then be also used to obtain the same solution in two space
dimensions.
**** Spherical waves[edit] ****
The wave equation can be solved using the technique of separation_of_variables.
To obtain a solution with constant frequencies, let us first Fourier transform
the wave equation in time as
         &#x03A8; (    r &#x2192;    , t ) =  &#x222B;  &#x2212; &#x221E;
      &#x221E;   &#x03A8; (    r &#x2192;    , &#x03C9; )  e  &#x2212; i
      &#x03C9; t   d &#x03C9; .   {\displaystyle \Psi ({\vec {r}},t)=\int _{-
      \infty }^{\infty }\Psi ({\vec {r}},\omega )e^{-i\omega t}d\omega .}
      [\Psi ({\vec  {r}},t)=\int _{{-\infty }}^{{\infty }}\Psi ({\vec
      {r}},\omega )e^{{-i\omega t}}d\omega .]
So we get,
          (   &#x2207;  2   +    &#x03C9;  2    c  2      )  &#x03A8; (    r
      &#x2192;    , &#x03C9; ) = 0.   {\displaystyle \left(\nabla ^{2}+{\frac
      {\omega ^{2}}{c^{2}}}\right)\Psi ({\vec {r}},\omega )=0.}  [
      {\displaystyle \left(\nabla ^{2}+{\frac {\omega ^{2}}{c^{2}}}\right)\Psi
      ({\vec {r}},\omega )=0.}]
This is the Helmholtz_equation and can be solved using separation of variables.
If spherical coordinates are used to describe a problem, then the solution to
the angular part of the Helmholtz equation is given by spherical_harmonics and
the radial equation now becomes [11]
          [     d  2    d  r  2      +   2 r     d  d r    +  k  2   &#x2212;
      l ( l + 1 )   r  2      ]   f  l m   ( r ) = 0   {\displaystyle \left[
      {\frac {d^{2}}{dr^{2}}}+{\frac {2}{r}}{\frac {d}{dr}}+k^{2}-{\frac {l
      (l+1)}{r^{2}}}\right]f_{lm}(r)=0}  [\left[{\frac  {d^{2}}{dr^{2}}}+{\frac
      {2}{r}}{\frac  {d}{dr}}+k^{2}-{\frac  {l(l+1)}{r^{2}}}\right]f_{{lm}}
      (r)=0]
Here     k &#x2261;   &#x03C9; c     {\displaystyle k\equiv {\frac {\omega }
{c}}}  [k\equiv {\frac  {\omega }{c}}] and the complete solution is now given
by
         &#x03A8; (    r &#x2192;    , &#x03C9; ) =  &#x2211;  l m    [   A  l
      m   ( 1 )    h  l   ( 1 )   ( k r ) +  A  l m   ( 2 )    h  l   ( 2 )
      ( k r )  ]   Y  l m   ( &#x03B8; , &#x03D5; ) ,   {\displaystyle \Psi (
      {\vec {r}},\omega )=\sum _{lm}\left[A_{lm}^{(1)}h_{l}^{(1)}(kr)+A_{lm}^{
      (2)}h_{l}^{(2)}(kr)\right]Y_{lm}(\theta ,\phi ),}  [{\displaystyle \Psi (
      {\vec {r}},\omega )=\sum _{lm}\left[A_{lm}^{(1)}h_{l}^{(1)}(kr)+A_{lm}^{
      (2)}h_{l}^{(2)}(kr)\right]Y_{lm}(\theta ,\phi ),}]
where      h  l   ( 1 )   ( k r )   {\displaystyle h_{l}^{(1)}(kr)}  [
{\displaystyle h_{l}^{(1)}(kr)}] and      h  l   ( 2 )   ( k r )
{\displaystyle h_{l}^{(2)}(kr)}  [{\displaystyle h_{l}^{(2)}(kr)}] are the
spherical_Hankel_functions. To gain a better understanding of the nature of
these spherical waves, let us go back and look at the case when     l = 0
{\displaystyle l=0}  [l=0]. In this case, there is no angular dependence and
the amplitude depends only on the radial distance i.e.     &#x03A8; (    r
&#x2192;    , t ) &#x2192; u ( r , t )   {\displaystyle \Psi ({\vec
{r}},t)\rightarrow u(r,t)}  [\Psi ({\vec  {r}},t)\rightarrow u(r,t)]. In this
case, the wave equation reduces to
          (   &#x2207;  2   &#x2212;   1  c  2        &#x2202;  2    &#x2202;
      t  2       )  &#x03A8; (    r &#x2192;    , t ) = 0 &#x2192;
      (     &#x2202;  2    &#x2202;  r  2      +   2 r     &#x2202;  &#x2202; r
      &#x2212;   1  c  2        &#x2202;  2    &#x2202;  t  2       )  u ( r ,
      t ) = 0   {\displaystyle \left(\nabla ^{2}-{\frac {1}{c^{2}}}{\frac
      {\partial ^{2}}{\partial t^{2}}}\right)\Psi ({\vec {r}},t)=0\rightarrow
      \left({\frac {\partial ^{2}}{\partial r^{2}}}+{\frac {2}{r}}{\frac
      {\partial }{\partial r}}-{\frac {1}{c^{2}}}{\frac {\partial ^{2}}
      {\partial t^{2}}}\right)u(r,t)=0}  [\left(\nabla ^{2}-{\frac  {1}{c^{2}}}
      {\frac  {\partial ^{2}}{\partial t^{2}}}\right)\Psi ({\vec
      {r}},t)=0\rightarrow \left({\frac  {\partial ^{2}}{\partial r^{2}}}+
      {\frac  {2}{r}}{\frac  {\partial }{\partial r}}-{\frac  {1}{c^{2}}}{\frac
      {\partial ^{2}}{\partial t^{2}}}\right)u(r,t)=0]
This equation can be rewritten as
             &#x2202;  2   ( r u )   &#x2202;  t  2      &#x2212;  c  2
      &#x2202;  2   ( r u )   &#x2202;  r  2      = 0 ;    {\displaystyle
      {\frac {\partial ^{2}(ru)}{\partial t^{2}}}-c^{2}{\frac {\partial ^{2}
      (ru)}{\partial r^{2}}}=0;\,}  [ \frac{\partial^2(ru)}{\partial t^2} -c^2
      \frac{\partial^2(ru)}{\partial r^2}=0; \,]
where the quantity     r u   {\displaystyle ru}  [ru] satisfies the one-
dimensional wave equation. Therefore, there are solutions in the form
         u ( r , t ) =   1 r   F ( r &#x2212; c t ) +   1 r   G ( r + c t ) ,
      {\displaystyle u(r,t)={\frac {1}{r}}F(r-ct)+{\frac {1}{r}}G(r+ct),}  [u
      (r,t)={\frac  {1}{r}}F(r-ct)+{\frac  {1}{r}}G(r+ct),]
where F and G are general solutions to the one-dimensional wave equation, and
can be interpreted as respectively an outgoing or incoming spherical wave. Such
waves are generated by a point_source, and they make possible sharp signals
whose form is altered only by a decrease in amplitude as r increases (see an
illustration of a spherical wave on the top right). Such waves exist only in
cases of space with odd dimensions.[citation_needed]
For physical examples of non-spherical wave solutions to the 3D wave equation
that do possess angular dependence, see dipole_radiation.
*** Monochromatic spherical wave[edit] ***
Cut-away of spherical wavefronts, with a wavelength of 10 units, propagating
from a point source.
Although the word "monochromatic" is not exactly accurate since it refers to
light or electromagnetic_radiation with well-defined frequency, the spirit is
to discover the eigenmode of the wave equation in three dimensions. Following
the derivation in the previous section on Plane_wave_eigenmodes, if we again
restrict our solutions to spherical waves that oscillate in time with well-
defined constant angular frequency     &#x03C9;   {\displaystyle \omega }
[\omega ], then the transformed function     r u ( r , t )   {\displaystyle ru
(r,t)}  [ ru(r,t) ] has simply plane wave solutions,
         r u ( r , t ) = A  e  i ( &#x03C9; t &#x00B1; k r )     {\displaystyle
      ru(r,t)=Ae^{i(\omega t\pm kr)}}  [ r u(r,t) = Ae^{i(\omega t\pm kr)}],
or
         u ( r , t ) =   A r    e  i  (  &#x03C9; t &#x00B1; k r  )
      {\displaystyle u(r,t)={\frac {A}{r}}e^{i\left(\omega t\pm kr\right)}}
      [ u(r,t)= \frac{A}{r} e^{i \left( \omega t \pm kr \right)}  ].
From this we can observe that the peak intensity of the spherical wave
oscillation, characterized as the squared wave amplitude
         I =  |  u ( r , t )   |   2   =     |  A   |   2     r  2
      {\displaystyle I=|u(r,t)|^{2}={\frac {|A|^{2}}{r^{2}}}}  [ I = |u
      (r,t)|^2= \frac{|A|^2}{r^2} ].
drops at the rate proportional to     1  /   r  2     {\displaystyle 1/r^{2}}
[ 1/r^2 ], an example of the inverse-square_law.
**** Solution of a general initial-value problem[edit] ****
The wave equation is linear in u and it is left unaltered by translations in
space and time. Therefore, we can generate a great variety of solutions by
translating and summing spherical waves. Let Ï(Î¾, Î·, Î¶) be an arbitrary
function of three independent variables, and let the spherical wave form F be a
delta function: that is, let F be a weak limit of continuous functions whose
integral is unity, but whose support (the region where the function is non-
zero) shrinks to the origin. Let a family of spherical waves have center at
(Î¾, Î·, Î¶), and let r be the radial distance from that point. Thus
          r  2   = ( x &#x2212; &#x03BE;  )  2   + ( y &#x2212; &#x03B7;  )  2
      + ( z &#x2212; &#x03B6;  )  2   .   {\displaystyle r^{2}=(x-\xi )^{2}+(y-
      \eta )^{2}+(z-\zeta )^{2}.}  [r^{2}=(x-\xi )^{2}+(y-\eta )^{2}+(z-\zeta
      )^{2}.]
If u is a superposition of such waves with weighting function Ï, then
         u ( t , x , y , z ) =   1  4 &#x03C0; c    &#x222D; &#x03C6;
      ( &#x03BE; , &#x03B7; , &#x03B6; )    &#x03B4; ( r &#x2212; c t )  r   d
      &#x03BE;  d &#x03B7;  d &#x03B6; ;   {\displaystyle u(t,x,y,z)={\frac {1}
      {4\pi c}}\iiint \varphi (\xi ,\eta ,\zeta ){\frac {\delta (r-ct)}{r}}d\xi
      \,d\eta \,d\zeta ;}  [{\displaystyle u(t,x,y,z)={\frac {1}{4\pi c}}\iiint
      \varphi (\xi ,\eta ,\zeta ){\frac {\delta (r-ct)}{r}}d\xi \,d\eta
      \,d\zeta ;}]
the denominator 4Ïc is a convenience.
From the definition of the delta function, u may also be written as
         u ( t , x , y , z ) =   t  4 &#x03C0;     &#x222C;  S   &#x03C6; ( x +
      c t &#x03B1; , y + c t &#x03B2; , z + c t &#x03B3; ) d &#x03C9; ,
      {\displaystyle u(t,x,y,z)={\frac {t}{4\pi }}\iint _{S}\varphi (x+ct\alpha
      ,y+ct\beta ,z+ct\gamma )d\omega ,}  [{\displaystyle u(t,x,y,z)={\frac {t}
      {4\pi }}\iint _{S}\varphi (x+ct\alpha ,y+ct\beta ,z+ct\gamma )d\omega ,}]
where Î±, Î², and Î³ are coordinates on the unit sphere S, and Ï is the area
element on S. This result has the interpretation that u(t, x) is t times the
mean value of Ï on a sphere of radius ct centered at x:
         u ( t , x , y , z ) = t  M  c t   [ &#x03D5; ] .   {\displaystyle u
      (t,x,y,z)=tM_{ct}[\phi ].}  [u(t,x,y,z)=tM_{{ct}}[\phi ].]
It follows that
         u ( 0 , x , y , z ) = 0 ,   u  t   ( 0 , x , y , z ) = &#x03D5; ( x ,
      y , z ) .   {\displaystyle u(0,x,y,z)=0,\quad u_{t}(0,x,y,z)=\phi
      (x,y,z).}  [u(0,x,y,z)=0,\quad u_{t}(0,x,y,z)=\phi (x,y,z).]
The mean value is an even function of t, and hence if
         v ( t , x , y , z ) =   &#x2202;  &#x2202; t     (  t  M  c t
      [ &#x03C8; ]  )  ,   {\displaystyle v(t,x,y,z)={\frac {\partial }
      {\partial t}}\left(tM_{ct}[\psi ]\right),}  [{\displaystyle v(t,x,y,z)=
      {\frac {\partial }{\partial t}}\left(tM_{ct}[\psi ]\right),}]
then
         v ( 0 , x , y , z ) = &#x03C8; ( x , y , z ) ,   v  t   ( 0 , x , y ,
      z ) = 0.   {\displaystyle v(0,x,y,z)=\psi (x,y,z),\quad v_{t}
      (0,x,y,z)=0.}  [v(0,x,y,z)=\psi (x,y,z),\quad v_{t}(0,x,y,z)=0.]
These formulas provide the solution for the initial-value problem for the wave
equation. They show that the solution at a given point P, given (t, x, y, z)
depends only on the data on the sphere of radius ct that is intersected by the
light cone drawn backwards from P. It does not depend upon data on the interior
of this sphere. Thus the interior of the sphere is a lacuna for the solution.
This phenomenon is called Huygens'_principle. It is true for odd numbers of
space dimension, where for one dimension the integration is performed over the
boundary of an interval with respect to the Dirac measure. It is not satisfied
in even space dimensions. The phenomenon of lacunas has been extensively
investigated in Atiyah, Bott and GÃ¥rding (1970, 1973).
***** Scalar wave equation in two space dimensions[edit] *****
In two space dimensions, the wave equation is
          u  t t   =  c  2    (   u  x x   +  u  y y    )  .    {\displaystyle
      u_{tt}=c^{2}\left(u_{xx}+u_{yy}\right).\,}  [ u_{tt} = c^2 \left( u_{xx}
      + u_{yy} \right). \,]
We can use the three-dimensional theory to solve this problem if we regard u as
a function in three dimensions that is independent of the third dimension. If
         u ( 0 , x , y ) = 0 ,   u  t   ( 0 , x , y ) = &#x03D5; ( x , y ) ,
      {\displaystyle u(0,x,y)=0,\quad u_{t}(0,x,y)=\phi (x,y),\,}  [ u
      (0,x,y)=0, \quad u_t(0,x,y) = \phi(x,y), \,]
then the three-dimensional solution formula becomes
         u ( t , x , y ) = t  M  c t   [ &#x03D5; ] =   t  4 &#x03C0;
      &#x222C;  S   &#x03D5; ( x + c t &#x03B1; ,  y + c t &#x03B2; ) d
      &#x03C9; ,    {\displaystyle u(t,x,y)=tM_{ct}[\phi ]={\frac {t}{4\pi
      }}\iint _{S}\phi (x+ct\alpha ,\,y+ct\beta )d\omega ,\,}  [ u(t,x,y) = tM_
      {ct}[\phi] = \frac{t}{4\pi} \iint_S \phi(x + ct\alpha,\, y + ct\beta)
      d\omega,\,]
where Î± and Î² are the first two coordinates on the unit sphere, and dÏ is
the area element on the sphere. This integral may be rewritten as a double
integral over the disc D with center (x,y) and radius ct:
         u ( t , x , y ) =   1  2 &#x03C0; c t     &#x222C;  D      &#x03D5;
      ( x + &#x03BE; , y + &#x03B7; )   ( c t  )  2   &#x2212;  &#x03BE;  2
      &#x2212;  &#x03B7;  2      d &#x03BE;  d &#x03B7; .    {\displaystyle u
      (t,x,y)={\frac {1}{2\pi ct}}\iint _{D}{\frac {\phi (x+\xi ,y+\eta )}
      {\sqrt {(ct)^{2}-\xi ^{2}-\eta ^{2}}}}d\xi \,d\eta .\,}  [{\displaystyle
      u(t,x,y)={\frac {1}{2\pi ct}}\iint _{D}{\frac {\phi (x+\xi ,y+\eta )}
      {\sqrt {(ct)^{2}-\xi ^{2}-\eta ^{2}}}}d\xi \,d\eta .\,}]
It is apparent that the solution at (t, x, y) depends not only on the data on
the light cone where
         ( x &#x2212; &#x03BE;  )  2   + ( y &#x2212; &#x03B7;  )  2   =  c  2
      t  2   ,   {\displaystyle (x-\xi )^{2}+(y-\eta )^{2}=c^{2}t^{2},}  [
      {\displaystyle (x-\xi )^{2}+(y-\eta )^{2}=c^{2}t^{2},}]
but also on data that are interior to that cone.
***** Scalar wave equation in general dimension and Kirchhoff's formulae[edit]
*****
We want to find solutions to utt â Îu = 0 for u : Rn Ã (0, â) â R with
u(x, 0) = g(x) and ut(x, 0) = h(x). See Evans for more details.
**** Odd dimensions[edit] ****
Assume n â¥ 3 is an odd integer and g â Cm+1(Rn), h â Cm(Rn) for m = (n +
1)/2. Let      &#x03B3;  n   = 1 &#x22C5; 3 &#x22C5; 5 &#x22C5; &#x2026;
&#x22C5; ( n &#x2212; 2 )   {\displaystyle \gamma _{n}=1\cdot 3\cdot 5\cdot
\ldots \cdot (n-2)}  [{\displaystyle \gamma _{n}=1\cdot 3\cdot 5\cdot \ldots
\cdot (n-2)}] and let
         u ( x , t ) =   1  &#x03B3;  n      [   &#x2202;  t     (    1 t
      &#x2202;  t    )     n &#x2212; 3  2     (   t  n &#x2212; 2     1   |
      &#x2202;  B  t   ( x )  |      &#x222B;  &#x2202;  B  t   ( x )   g d S
      )  +   (    1 t    &#x2202;  t    )     n &#x2212; 3  2     (   t  n
      &#x2212; 2     1   |  &#x2202;  B  t   ( x )  |      &#x222B;  &#x2202;
      B  t   ( x )   h d S  )   ]    {\displaystyle u(x,t)={\frac {1}{\gamma _
      {n}}}\left[\partial _{t}\left({\frac {1}{t}}\partial _{t}\right)^{\frac
      {n-3}{2}}\left(t^{n-2}{\frac {1}{|\partial B_{t}(x)|}}\int _{\partial B_
      {t}(x)}gdS\right)+\left({\frac {1}{t}}\partial _{t}\right)^{\frac {n-3}
      {2}}\left(t^{n-2}{\frac {1}{|\partial B_{t}(x)|}}\int _{\partial B_{t}
      (x)}hdS\right)\right]}  [{\displaystyle u(x,t)={\frac {1}{\gamma _
      {n}}}\left[\partial _{t}\left({\frac {1}{t}}\partial _{t}\right)^{\frac
      {n-3}{2}}\left(t^{n-2}{\frac {1}{|\partial B_{t}(x)|}}\int _{\partial B_
      {t}(x)}gdS\right)+\left({\frac {1}{t}}\partial _{t}\right)^{\frac {n-3}
      {2}}\left(t^{n-2}{\frac {1}{|\partial B_{t}(x)|}}\int _{\partial B_{t}
      (x)}hdS\right)\right]}]
then
      u â C2(Rn Ã [0, â))
      utt â Îu = 0 in Rn Ã (0, â)
              lim  ( x , t ) &#x2192; (  x  0   , 0 )   u ( x , t )    = g (  x
      0   )      lim  ( x , t ) &#x2192; (  x  0   , 0 )    u  t   ( x , t )
      = h (  x  0   )       {\displaystyle {\begin{aligned}\lim _{(x,t)\to (x^
      {0},0)}u(x,t)&=g(x^{0})\\\lim _{(x,t)\to (x^{0},0)}u_{t}(x,t)&=h(x^
      {0})\end{aligned}}}  [\begin{align}
      \lim_{(x,t)\to (x^0,0)} u(x,t) &= g(x^0) \\
      \lim_{(x,t)\to (x^0,0)} u_t(x,t) &= h(x^0)
      \end{align}]
**** Even dimensions[edit] ****
Assume n â¥ 2 is an even integer and g â Cm+1(Rn), h â Cm(Rn), for m = (n
+ 2)/2. Let      &#x03B3;  n   = 2 &#x22C5; 4 &#x22C5; &#x2026; &#x22C5; n
{\displaystyle \gamma _{n}=2\cdot 4\cdot \ldots \cdot n}  [{\displaystyle
\gamma _{n}=2\cdot 4\cdot \ldots \cdot n}] and let
         u ( x , t ) =   1  &#x03B3;  n      [   &#x2202;  t     (    1 t
      &#x2202;  t    )     n &#x2212; 2  2     (   t  n     1   |   B  t   ( x
      )  |      &#x222B;   B  t   ( x )     g  (  t  2   &#x2212;  |  y
      &#x2212; x   |   2    )   1 2       d y  )  +   (    1 t    &#x2202;  t
      )     n &#x2212; 2  2     (   t  n     1   |   B  t   ( x )  |
      &#x222B;   B  t   ( x )     h  (  t  2   &#x2212;  |  y &#x2212; x   |
      2    )   1 2       d y  )   ]    {\displaystyle u(x,t)={\frac {1}{\gamma
      _{n}}}\left[\partial _{t}\left({\frac {1}{t}}\partial _{t}\right)^{\frac
      {n-2}{2}}\left(t^{n}{\frac {1}{|B_{t}(x)|}}\int _{B_{t}(x)}{\frac {g}{(t^
      {2}-|y-x|^{2})^{\frac {1}{2}}}}dy\right)+\left({\frac {1}{t}}\partial _
      {t}\right)^{\frac {n-2}{2}}\left(t^{n}{\frac {1}{|B_{t}(x)|}}\int _{B_{t}
      (x)}{\frac {h}{(t^{2}-|y-x|^{2})^{\frac {1}{2}}}}dy\right)\right]}  [
      {\displaystyle u(x,t)={\frac {1}{\gamma _{n}}}\left[\partial _{t}\left(
      {\frac {1}{t}}\partial _{t}\right)^{\frac {n-2}{2}}\left(t^{n}{\frac {1}
      {|B_{t}(x)|}}\int _{B_{t}(x)}{\frac {g}{(t^{2}-|y-x|^{2})^{\frac {1}
      {2}}}}dy\right)+\left({\frac {1}{t}}\partial _{t}\right)^{\frac {n-2}
      {2}}\left(t^{n}{\frac {1}{|B_{t}(x)|}}\int _{B_{t}(x)}{\frac {h}{(t^{2}-
      |y-x|^{2})^{\frac {1}{2}}}}dy\right)\right]}]
then
      u â C2(Rn Ã [0, â))
      utt â Îu = 0 in Rn Ã (0, â)
              lim  ( x , t ) &#x2192; (  x  0   , 0 )   u ( x , t )    = g (  x
      0   )      lim  ( x , t ) &#x2192; (  x  0   , 0 )    u  t   ( x , t )
      = h (  x  0   )       {\displaystyle {\begin{aligned}\lim _{(x,t)\to (x^
      {0},0)}u(x,t)&=g(x^{0})\\\lim _{(x,t)\to (x^{0},0)}u_{t}(x,t)&=h(x^
      {0})\end{aligned}}}  [\begin{align}
      \lim_{(x,t)\to (x^0,0)} u(x,t) &= g(x^0)\\
      \lim_{(x,t)\to (x^0,0)} u_t(x,t) &= h(x^0)
      \end{align}]
***** Problems with boundaries[edit] *****
**** One space dimension[edit] ****
*** The SturmâLiouville formulation[edit] ***
A flexible string that is stretched between two points x = 0 and x = L
satisfies the wave equation for t > 0 and 0 < x < L. On the boundary points, u
may satisfy a variety of boundary conditions. A general form that is
appropriate for applications is
         &#x2212;  u  x   ( t , 0 ) + a u ( t , 0 ) = 0 ,   {\displaystyle -u_
      {x}(t,0)+au(t,0)=0,}  [{\displaystyle -u_{x}(t,0)+au(t,0)=0,}]
          u  x   ( t , L ) + b u ( t , L ) = 0 ,   {\displaystyle u_{x}(t,L)+bu
      (t,L)=0,}  [{\displaystyle u_{x}(t,L)+bu(t,L)=0,}]
where a and b are non-negative. The case where u is required to vanish at an
endpoint is the limit of this condition when the respective a or b approaches
infinity. The method of separation_of_variables consists in looking for
solutions of this problem in the special form
         u ( t , x ) = T ( t ) v ( x ) .   {\displaystyle u(t,x)=T(t)v(x).}  [
      {\displaystyle u(t,x)=T(t)v(x).}]
A consequence is that
            T &#x2033;    c  2   T    =    v &#x2033;  v   = &#x2212; &#x03BB;
      .   {\displaystyle {\frac {T''}{c^{2}T}}={\frac {v''}{v}}=-\lambda .}  [
      {\displaystyle {\frac {T''}{c^{2}T}}={\frac {v''}{v}}=-\lambda .}]
The eigenvalue Î» must be determined so that there is a non-trivial solution of
the boundary-value problem
          v &#x2033;  + &#x03BB; v = 0 ,   {\displaystyle v''+\lambda v=0,}  [
      {\displaystyle v''+\lambda v=0,}]
         &#x2212;  v &#x2032;  ( 0 ) + a v ( 0 ) = 0 ,   v &#x2032;  ( L ) + b
      v ( L ) = 0.   {\displaystyle -v'(0)+av(0)=0,\quad v'(L)+bv(L)=0.}  [
      {\displaystyle -v'(0)+av(0)=0,\quad v'(L)+bv(L)=0.}]
This is a special case of the general problem of SturmâLiouville_theory. If a
and b are positive, the eigenvalues are all positive, and the solutions are
trigonometric functions. A solution that satisfies square-integrable initial
conditions for u and ut can be obtained from expansion of these functions in
the appropriate trigonometric series.
*** Investigation by numerical methods[edit] ***
Approximating the continuous string with a finite number of equidistant mass
points one gets the following physical model:
Figure 1: Three consecutive mass points of the discrete model for a string
If each mass point has the mass m, the tension of the string is f, the
separation between the mass points is Îx and ui, i = 1, ..., n are the offset
of these n points from their equilibrium points (i.e. their position on a
straight line between the two attachment points of the string) the vertical
component of the force towards point i + 1 is
             u  i + 1   &#x2212;  u  i     &#x0394; x    f       
      {\displaystyle {\frac {u_{i+1}-u_{i}}{\Delta x}}f}  [        (1)
      {\displaystyle {\frac {u_{i+1}-u_{i}}{\Delta x}}f}]
and the vertical component of the force towards point i â 1 is
             u  i &#x2212; 1   &#x2212;  u  i     &#x0394; x    f       
      {\displaystyle {\frac {u_{i-1}-u_{i}}{\Delta x}}f}  [               (2)
      {\displaystyle {\frac {u_{i-1}-u_{i}}{\Delta x}}f}]
Taking the sum of these two forces and dividing with the mass m one gets for
the vertical motion:
             u &#x00A8;     i   =  (   f  m &#x0394; x    )   (   u
      i + 1   +  u  i &#x2212; 1   &#x2212; 2  u  i    )
      {\displaystyle {\ddot {u}}_{i}=\left({\frac {f}{m\Delta            (3)
      x}}\right)\left(u_{i+1}+u_{i-1}-2u_{i}\right)}  [{\displaystyle    
      {\ddot {u}}_{i}=\left({\frac {f}{m\Delta x}}\right)\left(u_
      {i+1}+u_{i-1}-2u_{i}\right)}]
As the mass density is
         &#x03C1; =   m  &#x0394; x      {\displaystyle \rho ={\frac {m}{\Delta
      x}}}  [\rho = \frac{m}{\Delta x}]
this can be written
             u &#x00A8;     i   =  (   f  &#x03C1;   &#x0394; x   2
      )   (   u  i + 1   +  u  i &#x2212; 1   &#x2212; 2  u  i    )
      {\displaystyle {\ddot {u}}_{i}=\left({\frac {f}{\rho {\Delta     (4)
      x}^{2}}}\right)\left(u_{i+1}+u_{i-1}-2u_{i}\right)}  [           
      {\displaystyle {\ddot {u}}_{i}=\left({\frac {f}{\rho {\Delta
      x}^{2}}}\right)\left(u_{i+1}+u_{i-1}-2u_{i}\right)}]
The wave equation is obtained by letting Îx â 0 in which case ui(t) takes
the form u(x, t) where u(x, t) is continuous function of two variables,
u &#x00A8;     i     {\displaystyle {\ddot {u}}_{i}}  [\ddot u_i] takes the
form       &#x2202;  2   u   &#x2202;  t  2      {\displaystyle \partial ^{2}u
\over \partial t^{2}}  [\partial^2 u \over \partial t^2] and
             u  i + 1   +  u  i &#x2212; 1   &#x2212; 2  u  i      &#x0394; x
      2     &#x2192;     &#x2202;  2   u   &#x2202;  x  2        {\displaystyle
      {\frac {u_{i+1}+u_{i-1}-2u_{i}}{{\Delta x}^{2}}}\to {\frac {\partial ^
      {2}u}{\partial x^{2}}}}  [{\displaystyle {\frac {u_{i+1}+u_{i-1}-2u_{i}}{
      {\Delta x}^{2}}}\to {\frac {\partial ^{2}u}{\partial x^{2}}}}]
But the discrete formulation (3) of the equation of state with a finite number
of mass point is just the suitable one for a numerical_propagation of the
string motion. The boundary condition
         u ( 0 , t ) = u ( L , t ) = 0   {\displaystyle u(0,t)=u(L,t)=0}  [u
      (0,t) = u(L,t) = 0]
where L is the length of the string takes in the discrete formulation the form
that for the outermost points u1 and un the equation of motion are
             u &#x00A8;     1   =    (   c  &#x0394; x    )    2
      (   u  2   &#x2212; 2  u  1    )    {\displaystyle {\ddot {u}}_    
      {1}={\left({\frac {c}{\Delta x}}\right)}^{2}\left(u_{2}-2u_          (5)
      {1}\right)}  [{\displaystyle {\ddot {u}}_{1}={\left({\frac {c}
      {\Delta x}}\right)}^{2}\left(u_{2}-2u_{1}\right)}]
and
             u &#x00A8;     n   =    (   c  &#x0394; x    )    2
      (   u  n &#x2212; 1   &#x2212; 2  u  n    )    {\displaystyle      
      {\ddot {u}}_{n}={\left({\frac {c}{\Delta x}}\right)}^{2}\left        (6)
      (u_{n-1}-2u_{n}\right)}  [{\displaystyle {\ddot {u}}_{n}={\left
      ({\frac {c}{\Delta x}}\right)}^{2}\left(u_{n-1}-2u_{n}\right)}]
while for 1 < i < n
             u &#x00A8;     i   =    (   c  &#x0394; x    )    2
      (   u  i + 1   +  u  i &#x2212; 1   &#x2212; 2  u  i    )
      {\displaystyle {\ddot {u}}_{i}={\left({\frac {c}{\Delta           (7)
      x}}\right)}^{2}\left(u_{i+1}+u_{i-1}-2u_{i}\right)}  [            
      {\displaystyle {\ddot {u}}_{i}={\left({\frac {c}{\Delta
      x}}\right)}^{2}\left(u_{i+1}+u_{i-1}-2u_{i}\right)}]
where     c =     f &#x03C1;     .   {\displaystyle c={\sqrt {\tfrac {f}{\rho
}}}.}  [{\displaystyle c={\sqrt {\tfrac {f}{\rho }}}.}]
If the string is approximated with 100 discrete mass points one gets the 100
coupled second order differential equations (5), (6) and (7) or equivalently
200 coupled first order differential equations.
Propagating these up to the times
           L c   k 0.05 k = 0 , &#x22EF; , 5   {\displaystyle {\frac {L}
      {c}}k0.05k=0,\cdots ,5}  [{\displaystyle {\frac {L}{c}}k0.05k=0,\cdots
      ,5}]
using an 8th order multistep_method the 6 states displayed in figure 2 are
found:
Figure 2: The string at 6 consecutive epochs, the first (red) corresponding to
the initial time with the string in rest
Figure 3: The string at 6 consecutive epochs
Figure 4: The string at 6 consecutive epochs
Figure 5: The string at 6 consecutive epochs
Figure 6: The string at 6 consecutive epochs
Figure 7: The string at 6 consecutive epochs
The red curve is the initial state at time zero at which the string is "let
free" in a predefined shape[12] with all         u &#x02D9;     i   = 0
{\displaystyle {\dot {u}}_{i}=0}  [{\displaystyle {\dot {u}}_{i}=0}]. The blue
curve is the state at time        L c    ( 0.25 ) ,   {\displaystyle {\tfrac
{L}{c}}(0.25),}  [{\displaystyle {\tfrac {L}{c}}(0.25),}] i.e. after a time
that corresponds to the time a wave that is moving with the nominal wave
velocity     c =     f &#x03C1;       {\displaystyle c={\sqrt {\tfrac {f}{\rho
}}}}  [{\displaystyle c={\sqrt {\tfrac {f}{\rho }}}}] would need for one fourth
of the length of the string.
Figure 3 displays the shape of the string at the times        L c    k ( 0.05 )
, k = 6 , &#x22EF; , 11   {\displaystyle {\tfrac {L}{c}}k(0.05),k=6,\cdots ,11}
[{\displaystyle {\tfrac {L}{c}}k(0.05),k=6,\cdots ,11}]. The wave travels in
direction right with the speed     c =     f &#x03C1;       {\displaystyle c=
{\sqrt {\tfrac {f}{\rho }}}}  [{\displaystyle c={\sqrt {\tfrac {f}{\rho }}}}]
without being actively constraint by the boundary conditions at the two
extremes of the string. The shape of the wave is constant, i.e. the curve is
indeed of the form f(x â ct).
Figure 4 displays the shape of the string at the times        L c    k ( 0.05 )
, k = 12 , &#x22EF; , 17   {\displaystyle {\tfrac {L}{c}}k(0.05),k=12,\cdots
,17}  [{\displaystyle {\tfrac {L}{c}}k(0.05),k=12,\cdots ,17}]. The constraint
on the right extreme starts to interfere with the motion preventing the wave to
raise the end of the string.
Figure 5 displays the shape of the string at the times        L c    k ( 0.05 )
, k = 18 , &#x22EF; , 23   {\displaystyle {\tfrac {L}{c}}k(0.05),k=18,\cdots
,23}  [{\displaystyle {\tfrac {L}{c}}k(0.05),k=18,\cdots ,23}] when the
direction of motion is reversed. The red, green and blue curves are the states
at the times        L c    k ( 0.05 ) , k = 18 , &#x22EF; , 20   {\displaystyle
{\tfrac {L}{c}}k(0.05),k=18,\cdots ,20}  [{\displaystyle {\tfrac {L}{c}}k
(0.05),k=18,\cdots ,20}] while the 3 black curves correspond to the states at
times        L c    k ( 0.05 ) , k = 21 , &#x22EF; , 23   {\displaystyle
{\tfrac {L}{c}}k(0.05),k=21,\cdots ,23}  [{\displaystyle {\tfrac {L}{c}}k
(0.05),k=21,\cdots ,23}] with the wave starting to move back towards left.
Figure 6 and figure 7 finally display the shape of the string at the times
L c    k ( 0.05 ) , k = 24 , &#x22EF; , 29   {\displaystyle {\tfrac {L}{c}}k
(0.05),k=24,\cdots ,29}  [{\displaystyle {\tfrac {L}{c}}k(0.05),k=24,\cdots
,29}] and        L c    k ( 0.05 ) , k = 30 , &#x22EF; , 35   {\displaystyle
{\tfrac {L}{c}}k(0.05),k=30,\cdots ,35}  [{\displaystyle {\tfrac {L}{c}}k
(0.05),k=30,\cdots ,35}]. The wave now travels towards left and the constraints
at the end points are not active any more. When finally the other extreme of
the string the direction will again be reversed in a way similar to what is
displayed in figure 6.
**** Several space dimensions[edit] ****
A solution of the wave equation in two dimensions with a zero-displacement
boundary condition along the entire outer edge.
The one-dimensional initial-boundary value theory may be extended to an
arbitrary number of space dimensions. Consider a domain D in m-dimensional x
space, with boundary B. Then the wave equation is to be satisfied if x is in D
and t > 0. On the boundary of D, the solution u shall satisfy
            &#x2202; u   &#x2202; n    + a u = 0 ,    {\displaystyle {\frac
      {\partial u}{\partial n}}+au=0,\,}  [{\displaystyle {\frac {\partial u}
      {\partial n}}+au=0,\,}]
where n is the unit outward normal to B, and a is a non-negative function
defined on B. The case where u vanishes on B is a limiting case for a
approaching infinity. The initial conditions are
         u ( 0 , x ) = f ( x ) ,   u  t   ( 0 , x ) = g ( x ) ,
      {\displaystyle u(0,x)=f(x),\quad u_{t}(0,x)=g(x),\,}  [ u(0,x) = f(x),
      \quad u_t(0,x)=g(x), \,]
where f and g are defined in D. This problem may be solved by expanding f and g
in the eigenfunctions of the Laplacian in D, which satisfy the boundary
conditions. Thus the eigenfunction v satisfies
         &#x2207; &#x22C5; &#x2207; v + &#x03BB; v = 0 ,    {\displaystyle
      \nabla \cdot \nabla v+\lambda v=0,\,}  [ \nabla \cdot \nabla v + \lambda
      v = 0, \,]
in D, and
            &#x2202; v   &#x2202; n    + a v = 0 ,    {\displaystyle {\frac
      {\partial v}{\partial n}}+av=0,\,}  [{\displaystyle {\frac {\partial v}
      {\partial n}}+av=0,\,}]
on B.
In the case of two space dimensions, the eigenfunctions may be interpreted as
the modes of vibration of a drumhead stretched over the boundary B. If B is a
circle, then these eigenfunctions have an angular component that is a
trigonometric function of the polar angle Î¸, multiplied by a Bessel_function
(of integer order) of the radial component. Further details are in Helmholtz
equation.
If the boundary is a sphere in three space dimensions, the angular components
of the eigenfunctions are spherical_harmonics, and the radial components are
Bessel_functions of half-integer order.
***** Inhomogeneous wave equation in one dimension[edit] *****
See also: Inhomogeneous_electromagnetic_wave_equation
The inhomogeneous wave equation in one dimension is the following:
          c  2    u  x x   ( x , t ) &#x2212;  u  t t   ( x , t ) = s ( x , t )
      {\displaystyle c^{2}u_{xx}(x,t)-u_{tt}(x,t)=s(x,t)\,}  [{\displaystyle c^
      {2}u_{xx}(x,t)-u_{tt}(x,t)=s(x,t)\,}]
with initial conditions given by
         u ( x , 0 ) = f ( x )    {\displaystyle u(x,0)=f(x)\,}  [u(x,0)=f(x)
      \,]
          u  t   ( x , 0 ) = g ( x )    {\displaystyle u_{t}(x,0)=g(x)\,}  [u_t
      (x,0)=g(x) \,]
The function s(x, t) is often called the source function because in practice it
describes the effects of the sources of waves on the medium carrying them.
Physical examples of source functions include the force driving a wave on a
string, or the charge or current density in the Lorenz_gauge of
electromagnetism.
One method to solve the initial value problem (with the initial values as posed
above) is to take advantage of a special property of the wave equation in an
odd number of space dimensions, namely that its solutions respect causality.
That is, for any point (xi, ti), the value of u(xi, ti) depends only on the
values of f(xi + cti) and f(xi â cti) and the values of the function g(x)
between (xi â cti) and (xi + cti). This can be seen in d'Alembert's_formula,
stated above, where these quantities are the only ones that show up in it.
Physically, if the maximum propagation speed is c, then no part of the wave
that can't propagate to a given point by a given time can affect the amplitude
at the same point and time.
In terms of finding a solution, this causality property means that for any
given point on the line being considered, the only area that needs to be
considered is the area encompassing all the points that could causally affect
the point being considered. Denote the area that casually affects point (xi,
ti) as RC. Suppose we integrate the inhomogeneous wave equation over this
region.
          &#x222C;   R  C      (   c  2    u  x x   ( x , t ) &#x2212;  u  t t
      ( x , t )  )  d x d t =  &#x222C;   R  C     s ( x , t ) d x d t .
      {\displaystyle \iint \limits _{R_{C}}\left(c^{2}u_{xx}(x,t)-u_{tt}
      (x,t)\right)dxdt=\iint \limits _{R_{C}}s(x,t)dxdt.}  [\iint \limits_{R_C}
      \left ( c^2 u_{x x}(x,t) - u_{t t}(x,t) \right ) dx dt = \iint \limits_
      {R_C} s(x,t) dx dt. ]
To simplify this greatly, we can use Green's_theorem to simplify the left side
to get the following:
          &#x222B;   L  0   +  L  1   +  L  2      (  &#x2212;  c  2    u  x
      ( x , t ) d t &#x2212;  u  t   ( x , t ) d x  )  =  &#x222C;   R  C     s
      ( x , t ) d x d t .   {\displaystyle \int _{L_{0}+L_{1}+L_{2}}\left(-c^
      {2}u_{x}(x,t)dt-u_{t}(x,t)dx\right)=\iint \limits _{R_{C}}s(x,t)dxdt.}
      [\int_{ L_0 + L_1 + L_2 } \left ( - c^2 u_x(x,t) dt - u_t(x,t) dx \right
      ) = \iint \limits_{R_C} s(x,t) dx dt. ]
The left side is now the sum of three line integrals along the bounds of the
causality region. These turn out to be fairly easy to compute
          &#x222B;   x  i   &#x2212; c  t  i      x  i   + c  t  i     &#x2212;
      u  t   ( x , 0 ) d x = &#x2212;  &#x222B;   x  i   &#x2212; c  t  i
      x  i   + c  t  i     g ( x ) d x .   {\displaystyle \int _{x_{i}-ct_{i}}^
      {x_{i}+ct_{i}}-u_{t}(x,0)dx=-\int _{x_{i}-ct_{i}}^{x_{i}+ct_{i}}g(x)dx.}
      [\int^{x_i + c t_i}_{x_i - c t_i} - u_t(x,0) dx = - \int^{x_i + c t_i}_
      {x_i - c t_i} g(x) dx.]
In the above, the term to be integrated with respect to time disappears because
the time interval involved is zero, thus dt = 0.
For the other two sides of the region, it is worth noting that x Â± ct is a
constant, namely xi Â± cti, where the sign is chosen appropriately. Using this,
we can get the relation dx Â± cdt = 0, again choosing the right sign:
              &#x222B;   L  1      (  &#x2212;  c  2    u  x   ( x , t ) d t
      &#x2212;  u  t   ( x , t ) d x  )     =  &#x222B;   L  1      (  c  u  x
      ( x , t ) d x + c  u  t   ( x , t ) d t  )        = c  &#x222B;   L  1
      d u ( x , t )       = c u (  x  i   ,  t  i   ) &#x2212; c f (  x  i   +
      c  t  i   ) .       {\displaystyle {\begin{aligned}\int _{L_{1}}\left(-c^
      {2}u_{x}(x,t)dt-u_{t}(x,t)dx\right)&=\int _{L_{1}}\left(cu_{x}(x,t)dx+cu_
      {t}(x,t)dt\right)\\&=c\int _{L_{1}}du(x,t)\\&=cu(x_{i},t_{i})-cf(x_
      {i}+ct_{i}).\end{aligned}}}  [\begin{align}
      \int_{L_1} \left ( - c^2 u_x(x,t) dt - u_t(x,t) dx \right ) &= \int_{L_1}
      \left ( c u_x(x,t) dx + c u_t(x,t) dt \right)\\
      &= c \int_{L_1} d u(x,t) \\
      &= c u(x_i,t_i) - c f(x_i + c t_i).
      \end{align}]
And similarly for the final boundary segment:
              &#x222B;   L  2      (  &#x2212;  c  2    u  x   ( x , t ) d t
      &#x2212;  u  t   ( x , t ) d x  )     = &#x2212;  &#x222B;   L  2
      (  c  u  x   ( x , t ) d x + c  u  t   ( x , t ) d t  )        = &#x2212;
      c  &#x222B;   L  2     d u ( x , t )       = c u (  x  i   ,  t  i   )
      &#x2212; c f (  x  i   &#x2212; c  t  i   ) .       {\displaystyle
      {\begin{aligned}\int _{L_{2}}\left(-c^{2}u_{x}(x,t)dt-u_{t}
      (x,t)dx\right)&=-\int _{L_{2}}\left(cu_{x}(x,t)dx+cu_{t}
      (x,t)dt\right)\\&=-c\int _{L_{2}}du(x,t)\\&=cu(x_{i},t_{i})-cf(x_{i}-ct_
      {i}).\end{aligned}}}  [\begin{align}
      \int_{L_2} \left ( - c^2 u_x(x,t) dt - u_t(x,t) dx \right ) &= - \int_
      {L_2} \left ( c u_x(x,t) dx + c u_t(x,t) dt \right )\\
      &= - c \int_{L_2} d u(x,t) \\
      &= c u(x_i,t_i) - c f(x_i - c t_i).
      \end{align}]
Adding the three results together and putting them back in the original
integral:
              &#x222C;   R  C     s ( x , t ) d x d t    = &#x2212;  &#x222B;
      x  i   &#x2212; c  t  i      x  i   + c  t  i     g ( x ) d x + c u (  x
      i   ,  t  i   ) &#x2212; c f (  x  i   + c  t  i   ) + c u (  x  i   ,  t
      i   ) &#x2212; c f (  x  i   &#x2212; c  t  i   )       = 2 c u (  x  i
      ,  t  i   ) &#x2212; c f (  x  i   + c  t  i   ) &#x2212; c f (  x  i
      &#x2212; c  t  i   ) &#x2212;  &#x222B;   x  i   &#x2212; c  t  i      x
      i   + c  t  i     g ( x ) d x       {\displaystyle {\begin{aligned}\iint
      _{R_{C}}s(x,t)dxdt&=-\int _{x_{i}-ct_{i}}^{x_{i}+ct_{i}}g(x)dx+cu(x_
      {i},t_{i})-cf(x_{i}+ct_{i})+cu(x_{i},t_{i})-cf(x_{i}-ct_{i})\\&=2cu(x_
      {i},t_{i})-cf(x_{i}+ct_{i})-cf(x_{i}-ct_{i})-\int _{x_{i}-ct_{i}}^{x_
      {i}+ct_{i}}g(x)dx\end{aligned}}}  [\begin{align}
      \iint_{R_C} s(x,t) dx dt &= - \int^{x_i + c t_i}_{x_i - c t_i} g(x) dx +
      c u(x_i,t_i) - c f(x_i + c t_i) + c u(x_i,t_i) - c f(x_i - c t_i) \\
      &= 2 c u(x_i,t_i)  - c f(x_i + c t_i) - c f(x_i - c t_i) - \int^{x_i + c
      t_i}_{x_i - c t_i} g(x) dx
      \end{align}]
Solving for u(xi, ti) we arrive at
         u (  x  i   ,  t  i   ) =    f (  x  i   + c  t  i   ) + f (  x  i
      &#x2212; c  t  i   )  2   +   1  2 c     &#x222B;   x  i   &#x2212; c  t
      i      x  i   + c  t  i     g ( x ) d x +   1  2 c     &#x222B;  0    t
      i      &#x222B;   x  i   &#x2212; c  (   t  i   &#x2212; t  )     x  i
      + c  (   t  i   &#x2212; t  )    s ( x , t ) d x d t .   {\displaystyle u
      (x_{i},t_{i})={\frac {f(x_{i}+ct_{i})+f(x_{i}-ct_{i})}{2}}+{\frac {1}
      {2c}}\int _{x_{i}-ct_{i}}^{x_{i}+ct_{i}}g(x)dx+{\frac {1}{2c}}\int _{0}^
      {t_{i}}\int _{x_{i}-c\left(t_{i}-t\right)}^{x_{i}+c\left(t_{i}-t\right)}s
      (x,t)dxdt.}  [u(x_i,t_i) = \frac{f(x_i + c t_i) + f(x_i - c t_i)}{2} +
      \frac{1}{2 c}\int^{x_i + c t_i}_{x_i - c t_i} g(x) dx + \frac{1}{2
      c}\int^{t_i}_0 \int^{x_i + c \left ( t_i - t \right )}_{x_i - c \left
      ( t_i - t \right )} s(x,t) dx dt.]
In the last equation of the sequence, the bounds of the integral over the
source function have been made explicit. Looking at this solution, which is
valid for all choices (xi, ti) compatible with the wave equation, it is clear
that the first two terms are simply d'Alembert's formula, as stated above as
the solution of the homogeneous wave equation in one dimension. The difference
is in the third term, the integral over the source.
***** Other coordinate systems[edit] *****
In three dimensions, the wave equation, when written in elliptic_cylindrical
coordinates, may be solved by separation of variables, leading to the Mathieu
differential_equation.
***** Further generalizations[edit] *****
**** Elastic waves[edit] ****
The elastic wave equation (also known as the Navier-Cauchy_equation) in three
dimensions describes the propagation of waves in an isotropic homogeneous
elastic medium. Most solid materials are elastic, so this equation describes
such phenomena as seismic_waves in the Earth and ultrasonic waves used to
detect flaws in materials. While linear, this equation has a more complex form
than the equations given above, as it must account for both longitudinal and
transverse motion:
         &#x03C1;     u  &#x00A8;    =  f  + ( &#x03BB; + 2 &#x03BC; ) &#x2207;
      ( &#x2207; &#x22C5;  u  ) &#x2212; &#x03BC; &#x2207; &#x00D7; ( &#x2207;
      &#x00D7;  u  )   {\displaystyle \rho {\ddot {\mathbf {u} }}=\mathbf {f} +
      (\lambda +2\mu )\nabla (\nabla \cdot \mathbf {u} )-\mu \nabla \times
      (\nabla \times \mathbf {u} )}  [{\displaystyle \rho {\ddot {\mathbf {u}
      }}=\mathbf {f} +(\lambda +2\mu )\nabla (\nabla \cdot \mathbf {u} )-\mu
      \nabla \times (\nabla \times \mathbf {u} )}]
where:
    * Î» and Î¼ are the so-called LamÃ©_parameters describing the elastic
      properties of the medium,
    * Ï is the density,
    * f is the source function (driving force),
    * and u is the displacement vector.
By using     &#x2207; &#x00D7; ( &#x2207; &#x00D7;  u  ) = &#x2207; ( &#x2207;
&#x22C5;  u  ) &#x2212; &#x2207; &#x22C5; &#x2207;  u  = &#x2207; ( &#x2207;
&#x22C5;  u  ) &#x2212; &#x0394;  u    {\displaystyle \nabla \times (\nabla
\times \mathbf {u} )=\nabla (\nabla \cdot \mathbf {u} )-\nabla \cdot \nabla
\mathbf {u} =\nabla (\nabla \cdot \mathbf {u} )-\Delta \mathbf {u} }  [
{\displaystyle \nabla \times (\nabla \times \mathbf {u} )=\nabla (\nabla \cdot
\mathbf {u} )-\nabla \cdot \nabla \mathbf {u} =\nabla (\nabla \cdot \mathbf {u}
)-\Delta \mathbf {u} }] the elastic wave equation can be rewritten into the
more common form of the Navier-Cauchy_equation.
Note that in the elastic wave equation, both force and displacement are vector
quantities. Thus, this equation is sometimes known as the vector wave equation.
As an aid to understanding, the reader will observe that if f and â â u are
set to zero, this becomes (effectively) Maxwell's equation for the propagation
of the electric field E, which has only transverse waves.
**** Dispersion relation[edit] ****
In dispersive wave phenomena, the speed of wave propagation varies with the
wavelength of the wave, which is reflected by a dispersion_relation
         &#x03C9; = &#x03C9; (  k  ) ,   {\displaystyle \omega =\omega (\mathbf
      {k} ),}  [\omega =\omega ({\mathbf  {k}}),]
where Ï is the angular_frequency and k is the wavevector describing plane_wave
solutions. For light waves, the dispersion relation is Ï = Â±c |k|, but in
general, the constant speed c gets replaced by a variable phase_velocity:
          v   p    =    &#x03C9; ( k )  k   .   {\displaystyle v_{\mathrm {p}
      }={\frac {\omega (k)}{k}}.}  [v_{{\mathrm  {p}}}={\frac  {\omega (k)}
      {k}}.]
***** See also[edit] *****
    * Acoustic_attenuation
    * Acoustic_wave_equation
    * Bateman_transform
    * Electromagnetic_wave_equation
    * Helmholtz_equation
    * Inhomogeneous_electromagnetic_wave_equation
    * Laplace_operator
    * Mathematics_of_oscillation
    * Maxwell's_equations
    * SchrÃ¶dinger_equation
    * Standing_wave
    * Vibrations_of_a_circular_membrane
    * WheelerâFeynman_absorber_theory
***** Notes[edit] *****
   1. ^ Cannon,_John_T.;_Dostrovsky,_Sigalia_(1981)._The_evolution_of_dynamics,
      vibration_theory_from_1687_to_1742._Studies_in_the_History_of_Mathematics
      and_Physical_Sciences._6._New_York:_Springer-Verlag._pp. ix_+_184
      pp.ISBN 978-0-3879-0626-3.
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
   3. GRAY, JW (July 1983). "BOOK REVIEWS". Bulletin (New Series) of the
      American Mathematical Society. 9 (1).
   4.  (retrieved 13 Nov 2012).
   5. ^ Gerard F Wheeler. The_Vibrating_String_Controversy, (retrieved 13 Nov
      2012). Am. J. Phys., 1987, v55, n1, p33â37.
   6. ^ For a special collection of the 9 groundbreaking papers by the three
      authors, see First_Appearance_of_the_wave_equation:_D'Alembert,_Leonhard
      Euler,_Daniel_Bernoulli._â_the_controversy_about_vibrating_strings
      (retrieved 13 Nov 2012). Herman HJ Lynge and Son.
   7. ^ For de Lagrange's contributions to the acoustic wave equation, one can
      consult Acoustics:_An_Introduction_to_Its_Physical_Principles_and
      Applications Allan D. Pierce, Acoustical Soc of America, 1989; page 18
      (retrieved 9 Dec 2012).
   8. ^ a b c Speiser, David. Discovering_the_Principles_of_Mechanics
      1600â1800, p. 191 (Basel: BirkhÃ¤user, 2008).
   9. ^ Tipler, Paul and Mosca, Gene. Physics_for_Scientists_and_Engineers,
      Volume_1:_Mechanics,_Oscillations_and_Waves;_Thermodynamics, pp.
      470â471 (Macmillan, 2004).
  10. ^Eric_W._Weisstein. "d'Alembert's_Solution". MathWorld. Retrieved 2009-
      01-21.
  11. ^ D'Alembert (1747) "Recherches_sur_la_courbe_que_forme_une_corde_tenduÃ«
      mise_en_vibration" (Researches on the curve that a tense cord forms
      [when] set into vibration), Histoire de l'acadÃ©mie royale des sciences
      et belles lettres de Berlin, vol. 3, pages 214â219.
          o See also: D'Alembert (1747) "Suite_des_recherches_sur_la_courbe_que
            forme_une_corde_tenduÃ«_mise_en_vibration" (Further researches on
            the curve that a tense cord forms [when] set into vibration),
            Histoire de l'acadÃ©mie royale des sciences et belles lettres de
            Berlin, vol. 3, pages 220â249.
          o See also: D'Alembert (1750) "Addition_au_mÃ©moire_sur_la_courbe_que
            forme_une_corde_tenduÃ«_mise_en_vibration," Histoire de l'acadÃ©mie
            royale des sciences et belles lettres de Berlin, vol. 6, pages
            355â360.
  12. ^ http://math.arizona.edu/~kglasner/math456/linearwave.pdf.
  13. ^V Guruprasad (2015), "Observational_evidence_for_travelling_wave_modes
      bearing_distance_proportional_shifts", EPL, 110 (5): 54001, arXiv:
      1507.08222, Bibcode:2015EL....11054001G, doi:10.1209/0295-5075/110/54001
  14. ^ John David Jackson, Classical Electrodynamics, 3rd Edition, Wiley, page
      425.
  15. ISBN 978-0-471-30932-1
  16. ^ The initial state for "Investigation by numerical methods" is set with
      quadratic splines as follows:
               u ( 0 , x ) =  u  0    (  1 &#x2212;   (    x &#x2212;  x  1
            x  1     )   2    )    {\displaystyle u(0,x)=u_{0}\left(1-\left(
            {\frac {x-x_{1}}{x_{1}}}\right)^{2}\right)}  [{\displaystyle u
            (0,x)=u_{0}\left(1-\left({\frac {x-x_{1}}{x_{1}}}\right)^
            {2}\right)}] for     0 &#x2264; x &#x2264;  x  2     {\displaystyle
            0\leq x\leq x_{2}}  [0 \le x \le x_2]
               u ( 0 , x ) =  u  0     (    x &#x2212;  x  3     x  1     )   2
            {\displaystyle u(0,x)=u_{0}\left({\frac {x-x_{3}}{x_{1}}}\right)^
            {2}}  [{\displaystyle u(0,x)=u_{0}\left({\frac {x-x_{3}}{x_
            {1}}}\right)^{2}}] for      x  2   &#x2264; x &#x2264;  x  3
            {\displaystyle x_{2}\leq x\leq x_{3}}  [x_2 \le x \le x_3]
               u ( 0 , x ) = 0   {\displaystyle u(0,x)=0}  [u(0,x)= 0] for
            x  3   &#x2264; x &#x2264; L   {\displaystyle x_{3}\leq x\leq L}
            [x_3 \le x \le L]
      with      x  1   =    1 10    L ,  x  2   =  x  1   +     1 2      x  1
      ,  x  3   =  x  2   +     1 2      x  1     {\displaystyle x_{1}={\tfrac
      {1}{10}}L,x_{2}=x_{1}+{\sqrt {\tfrac {1}{2}}}x_{1},x_{3}=x_{2}+{\sqrt
      {\tfrac {1}{2}}}x_{1}}  [{\displaystyle x_{1}={\tfrac {1}{10}}L,x_{2}=x_
      {1}+{\sqrt {\tfrac {1}{2}}}x_{1},x_{3}=x_{2}+{\sqrt {\tfrac {1}{2}}}x_
      {1}}]
***** References[edit] *****
    * M. F. Atiyah, R. Bott, L. Garding, "Lacunas_for_hyperbolic_differential
      operators_with_constant_coefficients_I", Acta Math., 124 (1970),
      109â189.
    * M.F. Atiyah, R. Bott, and L. Garding, "Lacunas_for_hyperbolic
      differential_operators_with_constant_coefficients_II", Acta Math., 131
      (1973), 145â206.
    * R. Courant, D. Hilbert, Methods of Mathematical Physics, vol II.
      Interscience (Wiley) New York, 1962.
    * L. Evans, "Partial Differential Equations". American Mathematical Society
      Providence, 1998.
    * "Linear_Wave_Equations", EqWorld: The World of Mathematical Equations.
    * "Nonlinear_Wave_Equations", EqWorld: The World of Mathematical Equations.
    * William C. Lane, "MISN-0-201_The_Wave_Equation_and_Its_Solutions",
      Project_PHYSNET.
***** External links[edit] *****
    * Nonlinear_Wave_Equations by Stephen_Wolfram and Rob Knapp, Nonlinear_Wave
      Equation_Explorer by Wolfram_Demonstrations_Project.
    * Mathematical aspects of wave equations are discussed on the Dispersive
      PDE_Wiki.
    * Graham W Griffiths and William E. Schiesser (2009). Linear_and_nonlinear
      waves. Scholarpedia, 4(7):4308. doi:10.4249/scholarpedia.4308
 Wikimedia Commons has media related to Wave_equation.
Authority_control [Edit_this_at_Wikidata]     * NDL: 00562751

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Wave_equation&oldid=908398212"
Categories:
    * Concepts_in_physics
    * Hyperbolic_partial_differential_equations
    * Wave_mechanics
Hidden categories:
    * Use_American_English_from_February_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_February_2014
    * Commons_category_link_from_Wikidata
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Alemannisch
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * à¨ªà©°à¨à¨¾à¨¬à©
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 29 July 2019, at 13:27 (UTC).
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
