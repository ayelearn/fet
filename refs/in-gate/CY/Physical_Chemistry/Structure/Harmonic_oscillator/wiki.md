The following text has been accessed from https://en.wikipedia.org/wiki/Harmonic_oscillator at Fri Aug 9 02:04:12 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Harmonic oscillator ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Physical system that responds to a restoring force inversely proportional to
displacement
This article is about the harmonic oscillator in classical mechanics. For its
uses in quantum_mechanics, see quantum_harmonic_oscillator.
Part of a series of articles about
Classical_mechanics
      F &#x2192;    = m    a &#x2192;      {\displaystyle {\vec {F}}=m{\vec
{a}}}  [{\vec {F}}=m{\vec {a}}]
Second_law_of_motion
    * History
    * Timeline
Branches
    * Applied
    * Celestial
    * Continuum
    * Dynamics
    * Kinematics
    * Kinetics
    * Statics
    * Statistical
Fundamentals
    * Acceleration
    * Angular_momentum
    * Couple
    * D'Alembert's_principle
    * Energy
          o kinetic
          o potential
    * Force
    * Frame_of_reference
    * Inertial_frame_of_reference
    * Impulse
    * Inertia / Moment_of_inertia
    * Mass
    *
      Mechanical_power
    * Mechanical_work
    *
      Moment
    * Momentum
    * Space
    * Speed
    * Time
    * Torque
    * Velocity
    * Virtual_work
Formulations
    * Newton's_laws_of_motion
    * Analytical_mechanics
          o Lagrangian_mechanics
          o Hamiltonian_mechanics
          o Routhian_mechanics
          o HamiltonâJacobi_equation
          o Appell's_equation_of_motion
          o UdwadiaâKalaba_equation
          o Koopmanâvon_Neumann_mechanics
Core topics
    * Damping (ratio)
    * Displacement
    * Equations_of_motion
    * Euler's_laws_of_motion
    * Fictitious_force
    * Friction
    * Harmonic oscillator
    * Inertial / Non-inertial_reference_frame
    * Mechanics_of_planar_particle_motion
    * Motion (linear)
    * Newton's_law_of_universal_gravitation
    * Newton's_laws_of_motion
    * Relative_velocity
    * Rigid_body
          o dynamics
          o Euler's_equations
    * Simple_harmonic_motion
    * Vibration
Rotation
    * Circular_motion
    * Rotating_reference_frame
    * Centripetal_force
    * Centrifugal_force
          o reactive
    * Coriolis_force
    * Pendulum
    * Tangential_speed
    * Rotational_speed
    * Angular_acceleration / displacement / frequency / velocity
Scientists
    * Galileo
    * Huygens
    * Newton
    * Kepler
    * Horrocks
    * Halley
    * Euler
    * d'Alembert
    * Clairaut
    * Lagrange
    * Laplace
    * Hamilton
    * Poisson
    * Daniel_Bernoulli
    * Johann_Bernoulli
    * Cauchy
    * v
    * t
    * e
In classical_mechanics, a harmonic oscillator is a system that, when displaced
from its equilibrium position, experiences a restoring_force F proportional to
the displacement x:
            F &#x2192;    = &#x2212; k    x &#x2192;    ,   {\displaystyle
      {\vec {F}}=-k{\vec {x}},}  [{\displaystyle {\vec {F}}=-k{\vec {x}},}]
where k is a positive constant.
If F is the only force acting on the system, the system is called a simple
harmonic oscillator, and it undergoes simple_harmonic_motion: sinusoidal
oscillations about the equilibrium point, with a constant amplitude and a
constant frequency (which does not depend on the amplitude).
If a frictional force (damping) proportional to the velocity is also present,
the harmonic oscillator is described as a damped oscillator. Depending on the
friction coefficient, the system can:
    * Oscillate with a frequency lower than in the undamped case, and an
      amplitude decreasing with time (underdamped oscillator).
    * Decay to the equilibrium position, without oscillations (overdamped
      oscillator).
The boundary solution between an underdamped oscillator and an overdamped
oscillator occurs at a particular value of the friction coefficient and is
called critically_damped.
If an external time-dependent force is present, the harmonic oscillator is
described as a driven oscillator.
Mechanical examples include pendulums (with small_angles_of_displacement),
masses connected to springs, and acoustical_systems. Other analogous_systems
include electrical harmonic oscillators such as RLC_circuits. The harmonic
oscillator model is very important in physics, because any mass subject to a
force in stable equilibrium acts as a harmonic oscillator for small vibrations.
Harmonic oscillators occur widely in nature and are exploited in many manmade
devices, such as clocks and radio circuits. They are the source of virtually
all sinusoidal vibrations and waves.
⁰
***** Contents *****
    * 1_Simple_harmonic_oscillator
    * 2_Damped_harmonic_oscillator
    * 3_Driven_harmonic_oscillators
          o 3.1_Step_input
          o 3.2_Sinusoidal_driving_force
    * 4_Parametric_oscillators
    * 5_Universal_oscillator_equation
          o 5.1_Transient_solution
          o 5.2_Steady-state_solution
                # 5.2.1_Amplitude_part
                # 5.2.2_Phase_part
          o 5.3_Full_solution
    * 6_Equivalent_systems
    * 7_Application_to_a_conservative_force
    * 8_Examples
          o 8.1_Simple_pendulum
          o 8.2_Spring/mass_system
                # 8.2.1_Energy_variation_in_the_springâdamping_system
    * 9_Definition_of_terms
    * 10_See_also
    * 11_Notes
    * 12_References
    * 13_External_links
***** Simple harmonic oscillator[edit] *****
Main article: Simple_harmonic_motion
Mass-spring harmonic oscillator
Simple harmonic motion
A simple harmonic oscillator is an oscillator that is neither driven nor
damped. It consists of a mass m, which experiences a single force F, which
pulls the mass in the direction of the point x = 0 and depends only on the
mass's position x and a constant k. Balance of forces (Newton's_second_law) for
the system is
         F = m a = m      d   2   x    d   t  2      = m    x &#x00A8;    =
      &#x2212; k x .   {\displaystyle F=ma=m{\frac {\mathrm {d} ^{2}x}{\mathrm
      {d} t^{2}}}=m{\ddot {x}}=-kx.}  [F=ma=m{\frac {\mathrm {d} ^{2}x}{\mathrm
      {d} t^{2}}}=m{\ddot {x}}=-kx.]
Solving this differential_equation, we find that the motion is described by the
function
         x ( t ) = A cos &#x2061; ( &#x03C9; t + &#x03C6; ) ,   {\displaystyle
      x(t)=A\cos(\omega t+\varphi ),}  [{\displaystyle x(t)=A\cos(\omega
      t+\varphi ),}]
where
         &#x03C9; =    k m    .   {\displaystyle \omega ={\sqrt {\frac {k}
      {m}}}.}  [{\displaystyle \omega ={\sqrt {\frac {k}{m}}}.}]
The motion is periodic, repeating itself in a sinusoidal fashion with constant
amplitude A. In addition to its amplitude, the motion of a simple harmonic
oscillator is characterized by its period     T = 2 &#x03C0;  /  &#x03C9;
{\displaystyle T=2\pi /\omega }  [{\displaystyle T=2\pi /\omega }], the time
for a single oscillation or its frequency     f = 1  /  T   {\displaystyle f=1/
T}  [{\displaystyle f=1/T}], the number of cycles per unit time. The position
at a given time t also depends on the phase Ï, which determines the starting
point on the sine wave. The period and frequency are determined by the size of
the mass m and the force constant k, while the amplitude and phase are
determined by the starting position and velocity.
The velocity and acceleration of a simple harmonic oscillator oscillate with
the same frequency as the position, but with shifted phases. The velocity is
maximal for zero displacement, while the acceleration is in the direction
opposite to the displacement.
The potential energy stored in a simple harmonic oscillator at position x is
         U =   1 2   k  x  2   .   {\displaystyle U={\frac {1}{2}}kx^{2}.}  [
      {\displaystyle U={\frac {1}{2}}kx^{2}.}]
***** Damped harmonic oscillator[edit] *****
Dependence of the system behavior on the value of the damping ratio Î¶
[File:Oscillatory motion acceleration.ogv]Play_media
Video clip demonstrating a damped harmonic oscillator consisting of a mass on a
low friction air_track.
In real oscillators, friction, or damping, slows the motion of the system. Due
to frictional force, the velocity decreases in proportion to the acting
frictional force. While in a simple undriven harmonic oscillator the only force
acting on the mass is the restoring force, in a damped harmonic oscillator
there is in addition a frictional force which is always in a direction to
oppose the motion. In many vibrating systems the frictional force Ff can be
modeled as being proportional to the velocity v of the object: Ff = âcv,
where c is called the viscous damping coefficient.
The balance of forces (Newton's_second_law) for damped harmonic oscillators is
then
         F = &#x2212; k x &#x2212; c     d  x    d  t    = m      d   2   x
      d   t  2      ,   {\displaystyle F=-kx-c{\frac {\mathrm {d} x}{\mathrm
      {d} t}}=m{\frac {\mathrm {d} ^{2}x}{\mathrm {d} t^{2}}},}  [
      {\displaystyle F=-kx-c{\frac {\mathrm {d} x}{\mathrm {d} t}}=m{\frac
      {\mathrm {d} ^{2}x}{\mathrm {d} t^{2}}},}][1][2][3]
which can be rewritten into the form
              d   2   x    d   t  2      + 2 &#x03B6;  &#x03C9;  0       d  x
      d  t    +  &#x03C9;  0   2   x = 0 ,   {\displaystyle {\frac {\mathrm {d}
      ^{2}x}{\mathrm {d} t^{2}}}+2\zeta \omega _{0}{\frac {\mathrm {d} x}
      {\mathrm {d} t}}+\omega _{0}^{2}x=0,}  [{\displaystyle {\frac {\mathrm
      {d} ^{2}x}{\mathrm {d} t^{2}}}+2\zeta \omega _{0}{\frac {\mathrm {d} x}
      {\mathrm {d} t}}+\omega _{0}^{2}x=0,}]
where
          &#x03C9;  0   =    k m      {\displaystyle \omega _{0}={\sqrt {\frac
      {k}{m}}}}  [{\displaystyle \omega _{0}={\sqrt {\frac {k}{m}}}}] is called
      the "undamped angular_frequency of the oscillator",
         &#x03B6; =   c  2   m k        {\displaystyle \zeta ={\frac {c}{2
      {\sqrt {mk}}}}}  [{\displaystyle \zeta ={\frac {c}{2{\sqrt {mk}}}}}] is
      called the "damping ratio".
Step_response of a damped harmonic oscillator; curves are plotted for three
values of Î¼ = Ï1 = Ï0√1 â Î¶2. Time is in units of the decay time Ï = 1/
(Î¶Ï0).
The value of the damping ratio Î¶ critically determines the behavior of the
system. A damped harmonic oscillator can be:
    * Overdamped (Î¶ > 1): The system returns (exponentially_decays) to steady
      state without oscillating. Larger values of the damping ratio Î¶ return
      to equilibrium more slowly.
    * Critically damped (Î¶ = 1): The system returns to steady state as quickly
      as possible without oscillating (although overshoot can occur). This is
      often desired for the damping of systems such as doors.
    * Underdamped (Î¶ < 1): The system oscillates (with a slightly different
      frequency than the undamped case) with the amplitude gradually decreasing
      to zero. The angular_frequency of the underdamped harmonic oscillator is
      given by      &#x03C9;  1   =  &#x03C9;  0     1 &#x2212;  &#x03B6;  2
      ,   {\displaystyle \omega _{1}=\omega _{0}{\sqrt {1-\zeta ^{2}}},}
      [\omega _{1}=\omega _{0}{\sqrt {1-\zeta ^{2}}},] the exponential_decay of
      the underdamped harmonic oscillator is given by     &#x03BB; =  &#x03C9;
      0   &#x03B6; .   {\displaystyle \lambda =\omega _{0}\zeta .}  [\lambda
      =\omega _{0}\zeta .]
The Q_factor of a damped oscillator is defined as
         Q = 2 &#x03C0; &#x00D7;   energy stored energy lost per cycle   .
      {\displaystyle Q=2\pi \times {\frac {\text{energy stored}}{\text{energy
      lost per cycle}}}.}  [{\displaystyle Q=2\pi \times {\frac {\text{energy
      stored}}{\text{energy lost per cycle}}}.}]
Q is related to the damping ratio by the equation     Q =   1  2 &#x03B6;    .
{\displaystyle Q={\frac {1}{2\zeta }}.}  [Q={\frac {1}{2\zeta }}.]
***** Driven harmonic oscillators[edit] *****
Driven harmonic oscillators are damped oscillators further affected by an
externally applied force F(t).
Newton's_second_law takes the form
         F ( t ) &#x2212; k x &#x2212; c     d  x    d  t    = m      d   2   x
      d   t  2      .   {\displaystyle F(t)-kx-c{\frac {\mathrm {d} x}{\mathrm
      {d} t}}=m{\frac {\mathrm {d} ^{2}x}{\mathrm {d} t^{2}}}.}  [F(t)-kx-c
      {\frac {\mathrm {d} x}{\mathrm {d} t}}=m{\frac {\mathrm {d} ^{2}x}
      {\mathrm {d} t^{2}}}.]
It is usually rewritten into the form
              d   2   x    d   t  2      + 2 &#x03B6;  &#x03C9;  0       d  x
      d  t    +  &#x03C9;  0   2   x =    F ( t )  m   .   {\displaystyle
      {\frac {\mathrm {d} ^{2}x}{\mathrm {d} t^{2}}}+2\zeta \omega _{0}{\frac
      {\mathrm {d} x}{\mathrm {d} t}}+\omega _{0}^{2}x={\frac {F(t)}{m}}.}  [
      {\frac {\mathrm {d} ^{2}x}{\mathrm {d} t^{2}}}+2\zeta \omega _{0}{\frac
      {\mathrm {d} x}{\mathrm {d} t}}+\omega _{0}^{2}x={\frac {F(t)}{m}}.]
This equation can be solved exactly for any driving force, using the solutions
z(t) that satisfy the unforced equation
              d   2   z    d   t  2      + 2 &#x03B6;  &#x03C9;  0       d  z
      d  t    +  &#x03C9;  0   2   z = 0 ,   {\displaystyle {\frac {\mathrm {d}
      ^{2}z}{\mathrm {d} t^{2}}}+2\zeta \omega _{0}{\frac {\mathrm {d} z}
      {\mathrm {d} t}}+\omega _{0}^{2}z=0,}  [{\frac {\mathrm {d} ^{2}z}
      {\mathrm {d} t^{2}}}+2\zeta \omega _{0}{\frac {\mathrm {d} z}{\mathrm {d}
      t}}+\omega _{0}^{2}z=0,]
and which can be expressed as damped sinusoidal oscillations:
         z ( t ) = A   e   &#x2212; &#x03B6;  &#x03C9;  0   t   sin &#x2061;
      (    1 &#x2212;  &#x03B6;  2      &#x03C9;  0   t + &#x03C6;  )  ,
      {\displaystyle z(t)=A\mathrm {e} ^{-\zeta \omega _{0}t}\sin \left({\sqrt
      {1-\zeta ^{2}}}\omega _{0}t+\varphi \right),}  [{\displaystyle z
      (t)=A\mathrm {e} ^{-\zeta \omega _{0}t}\sin \left({\sqrt {1-\zeta ^
      {2}}}\omega _{0}t+\varphi \right),}]
in the case where Î¶ â¤ 1. The amplitude A and phase Ï determine the behavior
needed to match the initial conditions.
**** Step input[edit] ****
See also: Step_response
In the case Î¶ < 1 and a unit step input with x(0) = 0:
            F ( t )  m   =   {     &#x03C9;  0   2     t &#x2265; 0     0   t <
      0         {\displaystyle {\frac {F(t)}{m}}={\begin{cases}\omega _{0}^
      {2}&t\geq 0\\0&t<0\end{cases}}}  [{\displaystyle {\frac {F(t)}{m}}=
      {\begin{cases}\omega _{0}^{2}&t\geq 0\\0&t<0\end{cases}}}]
the solution is
         x ( t ) = 1 &#x2212;   e   &#x2212; &#x03B6;  &#x03C9;  0   t      sin
      &#x2061;  (    1 &#x2212;  &#x03B6;  2      &#x03C9;  0   t + &#x03C6;  )
      sin &#x2061; ( &#x03C6; )    ,   {\displaystyle x(t)=1-\mathrm {e} ^{-
      \zeta \omega _{0}t}{\frac {\sin \left({\sqrt {1-\zeta ^{2}}}\omega _
      {0}t+\varphi \right)}{\sin(\varphi )}},}  [{\displaystyle x(t)=1-\mathrm
      {e} ^{-\zeta \omega _{0}t}{\frac {\sin \left({\sqrt {1-\zeta ^{2}}}\omega
      _{0}t+\varphi \right)}{\sin(\varphi )}},}]
with phase Ï given by
         cos &#x2061; &#x03C6; = &#x03B6; .   {\displaystyle \cos \varphi
      =\zeta .}  [{\displaystyle \cos \varphi =\zeta .}]
The time an oscillator needs to adapt to changed external conditions is of the
order Ï = 1/(Î¶Ï0). In physics, the adaptation is called relaxation, and Ï
is called the relaxation time.
In electrical engineering, a multiple of Ï is called the settling time, i.e.
the time necessary to ensure the signal is within a fixed departure from final
value, typically within 10%. The term overshoot refers to the extent the
response maximum exceeds final value, and undershoot refers to the extent the
response falls below final value for times following the response maximum.
**** Sinusoidal driving force[edit] ****
Steady-state variation of amplitude with relative frequency     &#x03C9;  /
&#x03C9;  0     {\displaystyle \omega /\omega _{0}}  [\omega /\omega _{0}] and
damping     &#x03B6;   {\displaystyle \zeta }  [\zeta ] of a driven simple
harmonic_oscillator
In the case of a sinusoidal driving force:
              d   2   x    d   t  2      + 2 &#x03B6;  &#x03C9;  0       d  x
      d  t    +  &#x03C9;  0   2   x =   1 m    F  0   sin &#x2061; ( &#x03C9;
      t ) ,   {\displaystyle {\frac {\mathrm {d} ^{2}x}{\mathrm {d} t^
      {2}}}+2\zeta \omega _{0}{\frac {\mathrm {d} x}{\mathrm {d} t}}+\omega _
      {0}^{2}x={\frac {1}{m}}F_{0}\sin(\omega t),}  [{\frac {\mathrm {d} ^{2}x}
      {\mathrm {d} t^{2}}}+2\zeta \omega _{0}{\frac {\mathrm {d} x}{\mathrm {d}
      t}}+\omega _{0}^{2}x={\frac {1}{m}}F_{0}\sin(\omega t),]
where      F  0     {\displaystyle F_{0}}  [F_{0}] is the driving amplitude,
and     &#x03C9;   {\displaystyle \omega }  [\omega ] is the driving frequency
for a sinusoidal driving mechanism. This type of system appears in AC-driven
RLC_circuits (resistorâinductorâcapacitor) and driven spring systems having
internal mechanical resistance or external air_resistance.
The general solution is a sum of a transient solution that depends on initial
conditions, and a steady_state that is independent of initial conditions and
depends only on the driving amplitude      F  0     {\displaystyle F_{0}}  [F_
{0}], driving frequency     &#x03C9;   {\displaystyle \omega }  [\omega ],
undamped angular frequency      &#x03C9;  0     {\displaystyle \omega _{0}}
[\omega _{0}], and the damping ratio     &#x03B6;   {\displaystyle \zeta }
[\zeta ].
The steady-state solution is proportional to the driving force with an induced
phase change     &#x03C6;   {\displaystyle \varphi }  [\varphi ]:
         x ( t ) =    F  0    m  Z  m   &#x03C9;    sin &#x2061; ( &#x03C9; t +
      &#x03C6; ) ,   {\displaystyle x(t)={\frac {F_{0}}{mZ_{m}\omega }}\sin
      (\omega t+\varphi ),}  [{\displaystyle x(t)={\frac {F_{0}}{mZ_{m}\omega
      }}\sin(\omega t+\varphi ),}]
where
          Z  m   =     (  2  &#x03C9;  0   &#x03B6;  )   2   +   1  &#x03C9;  2
      (  &#x03C9;  0   2   &#x2212;  &#x03C9;  2    )  2       {\displaystyle
      Z_{m}={\sqrt {\left(2\omega _{0}\zeta \right)^{2}+{\frac {1}{\omega ^
      {2}}}(\omega _{0}^{2}-\omega ^{2})^{2}}}}  [{\displaystyle Z_{m}={\sqrt
      {\left(2\omega _{0}\zeta \right)^{2}+{\frac {1}{\omega ^{2}}}(\omega _
      {0}^{2}-\omega ^{2})^{2}}}}]
is the absolute value of the impedance or linear_response_function, and
         &#x03C6; = arctan &#x2061;  (    2 &#x03C9;  &#x03C9;  0   &#x03B6;
      &#x03C9;  2   &#x2212;  &#x03C9;  0   2      )  + n &#x03C0;
      {\displaystyle \varphi =\arctan \left({\frac {2\omega \omega _{0}\zeta }
      {\omega ^{2}-\omega _{0}^{2}}}\right)+n\pi }  [{\displaystyle \varphi
      =\arctan \left({\frac {2\omega \omega _{0}\zeta }{\omega ^{2}-\omega _
      {0}^{2}}}\right)+n\pi }]
is the phase of the oscillation relative to the driving force. The phase value
is usually taken to be between â180Â° and 0 (that is, it represents a phase
lag, for both positive and negative values of the arctan argument).
For a particular driving frequency called the resonance, or resonant frequency
&#x03C9;  r   =  &#x03C9;  0     1 &#x2212; 2  &#x03B6;  2       {\displaystyle
\omega _{r}=\omega _{0}{\sqrt {1-2\zeta ^{2}}}}  [{\displaystyle \omega _
{r}=\omega _{0}{\sqrt {1-2\zeta ^{2}}}}], the amplitude (for a given      F  0
{\displaystyle F_{0}}  [F_{0}]) is maximal. This resonance effect only occurs
when     &#x03B6; < 1  /    2     {\displaystyle \zeta <1/{\sqrt {2}}}  [
{\displaystyle \zeta <1/{\sqrt {2}}}], i.e. for significantly underdamped
systems. For strongly underdamped systems the value of the amplitude can become
quite large near the resonant frequency.
The transient solutions are the same as the unforced (     F  0   = 0
{\displaystyle F_{0}=0}  [F_{0}=0]) damped harmonic oscillator and represent
the systems response to other events that occurred previously. The transient
solutions typically die out rapidly enough that they can be ignored.
***** Parametric oscillators[edit] *****
Main article: Parametric_oscillator
A parametric_oscillator is a driven harmonic oscillator in which the drive
energy is provided by varying the parameters of the oscillator, such as the
damping or restoring force. A familiar example of parametric oscillation is
"pumping" on a playground swing.[4][5][6] A person on a moving swing can
increase the amplitude of the swing's oscillations without any external drive
force (pushes) being applied, by changing the moment of inertia of the swing by
rocking back and forth ("pumping") or alternately standing and squatting, in
rhythm with the swing's oscillations. The varying of the parameters drives the
system. Examples of parameters that may be varied are its resonance frequency
&#x03C9;   {\displaystyle \omega }  [\omega ] and damping     &#x03B2;
{\displaystyle \beta }  [\beta ].
Parametric oscillators are used in many applications. The classical varactor
parametric oscillator oscillates when the diode's capacitance is varied
periodically. The circuit that varies the diode's capacitance is called the
"pump" or "driver". In microwave electronics, waveguide/YAG based parametric
oscillators operate in the same fashion. The designer varies a parameter
periodically to induce oscillations.
Parametric oscillators have been developed as low-noise amplifiers, especially
in the radio and microwave frequency range. Thermal noise is minimal, since a
reactance (not a resistance) is varied. Another common use is frequency
conversion, e.g., conversion from audio to radio frequencies. For example, the
Optical_parametric_oscillator converts an input laser wave into two output
waves of lower frequency (     &#x03C9;  s   ,  &#x03C9;  i     {\displaystyle
\omega _{s},\omega _{i}}  [\omega _{s},\omega _{i}]).
Parametric resonance occurs in a mechanical system when a system is
parametrically excited and oscillates at one of its resonant frequencies.
Parametric excitation differs from forcing, since the action appears as a time
varying modification on a system parameter. This effect is different from
regular resonance because it exhibits the instability phenomenon.
***** Universal oscillator equation[edit] *****
The equation
              d   2   q    d   &#x03C4;  2      + 2 &#x03B6;     d  q    d
      &#x03C4;    + q = 0   {\displaystyle {\frac {\mathrm {d} ^{2}q}{\mathrm
      {d} \tau ^{2}}}+2\zeta {\frac {\mathrm {d} q}{\mathrm {d} \tau }}+q=0}  [
      {\frac {\mathrm {d} ^{2}q}{\mathrm {d} \tau ^{2}}}+2\zeta {\frac {\mathrm
      {d} q}{\mathrm {d} \tau }}+q=0]
is known as the universal oscillator equation, since all second-order linear
oscillatory systems can be reduced to this form.[citation_needed] This is done
through nondimensionalization.
If the forcing function is f(t) = cos(Ït) = cos(ÏtcÏ) = cos(ÏÏ), where
Ï = Ïtc, the equation becomes
              d   2   q    d   &#x03C4;  2      + 2 &#x03B6;     d  q    d
      &#x03C4;    + q = cos &#x2061; ( &#x03C9; &#x03C4; ) .   {\displaystyle
      {\frac {\mathrm {d} ^{2}q}{\mathrm {d} \tau ^{2}}}+2\zeta {\frac {\mathrm
      {d} q}{\mathrm {d} \tau }}+q=\cos(\omega \tau ).}  [{\frac {\mathrm {d} ^
      {2}q}{\mathrm {d} \tau ^{2}}}+2\zeta {\frac {\mathrm {d} q}{\mathrm {d}
      \tau }}+q=\cos(\omega \tau ).]
The solution to this differential equation contains two parts: the "transient"
and the "steady-state".
**** Transient solution[edit] ****
The solution based on solving the ordinary_differential_equation is for
arbitrary constants c1 and c2
          q  t   ( &#x03C4; ) =   {      e   &#x2212; &#x03B6; &#x03C4;
      (   c  1     e   &#x03C4;    &#x03B6;  2   &#x2212; 1     +  c  2     e
      &#x2212; &#x03C4;    &#x03B6;  2   &#x2212; 1      )    &#x03B6; > 1
      &#xA0;(overdamping)        e   &#x2212; &#x03B6; &#x03C4;   (  c  1   +
      c  2   &#x03C4; ) =   e   &#x2212; &#x03C4;   (  c  1   +  c  2
      &#x03C4; )   &#x03B6; = 1  &#xA0;(critical damping)        e   &#x2212;
      &#x03B6; &#x03C4;    [   c  1   cos &#x2061;  (    1 &#x2212;  &#x03B6;
      2     &#x03C4;  )  +  c  2   sin &#x2061;  (    1 &#x2212;  &#x03B6;  2
      &#x03C4;  )   ]    &#x03B6; < 1  &#xA0;(underdamping)
      {\displaystyle q_{t}(\tau )={\begin{cases}\mathrm {e} ^{-\zeta \tau
      }\left(c_{1}\mathrm {e} ^{\tau {\sqrt {\zeta ^{2}-1}}}+c_{2}\mathrm {e} ^
      {-\tau {\sqrt {\zeta ^{2}-1}}}\right)&\zeta >1{\text{
      (overdamping)}}\\\mathrm {e} ^{-\zeta \tau }(c_{1}+c_{2}\tau )=\mathrm
      {e} ^{-\tau }(c_{1}+c_{2}\tau )&\zeta =1{\text{ (critical
      damping)}}\\\mathrm {e} ^{-\zeta \tau }\left[c_{1}\cos \left({\sqrt {1-
      \zeta ^{2}}}\tau \right)+c_{2}\sin \left({\sqrt {1-\zeta ^{2}}}\tau
      \right)\right]&\zeta <1{\text{ (underdamping)}}\end{cases}}}  [
      {\displaystyle q_{t}(\tau )={\begin{cases}\mathrm {e} ^{-\zeta \tau
      }\left(c_{1}\mathrm {e} ^{\tau {\sqrt {\zeta ^{2}-1}}}+c_{2}\mathrm {e} ^
      {-\tau {\sqrt {\zeta ^{2}-1}}}\right)&\zeta >1{\text{
      (overdamping)}}\\\mathrm {e} ^{-\zeta \tau }(c_{1}+c_{2}\tau )=\mathrm
      {e} ^{-\tau }(c_{1}+c_{2}\tau )&\zeta =1{\text{ (critical
      damping)}}\\\mathrm {e} ^{-\zeta \tau }\left[c_{1}\cos \left({\sqrt {1-
      \zeta ^{2}}}\tau \right)+c_{2}\sin \left({\sqrt {1-\zeta ^{2}}}\tau
      \right)\right]&\zeta <1{\text{ (underdamping)}}\end{cases}}}]
The transient solution is independent of the forcing function.
**** Steady-state solution[edit] ****
Apply the "complex_variables method" by solving the auxiliary equation below
and then finding the real part of its solution:
              d   2   q    d   &#x03C4;  2      + 2 &#x03B6;     d  q    d
      &#x03C4;    + q = cos &#x2061; ( &#x03C9; &#x03C4; ) +  i  sin &#x2061;
      ( &#x03C9; &#x03C4; ) =   e    i  &#x03C9; &#x03C4;   .   {\displaystyle
      {\frac {\mathrm {d} ^{2}q}{\mathrm {d} \tau ^{2}}}+2\zeta {\frac {\mathrm
      {d} q}{\mathrm {d} \tau }}+q=\cos(\omega \tau )+\mathrm {i} \sin(\omega
      \tau )=\mathrm {e} ^{\mathrm {i} \omega \tau }.}  [{\displaystyle {\frac
      {\mathrm {d} ^{2}q}{\mathrm {d} \tau ^{2}}}+2\zeta {\frac {\mathrm {d} q}
      {\mathrm {d} \tau }}+q=\cos(\omega \tau )+\mathrm {i} \sin(\omega \tau
      )=\mathrm {e} ^{\mathrm {i} \omega \tau }.}]
Supposing the solution is of the form
          q  s   ( &#x03C4; ) = A   e    i  ( &#x03C9; &#x03C4; + &#x03C6; )
      .   {\displaystyle q_{s}(\tau )=A\mathrm {e} ^{\mathrm {i} (\omega \tau
      +\varphi )}.}  [{\displaystyle q_{s}(\tau )=A\mathrm {e} ^{\mathrm {i}
      (\omega \tau +\varphi )}.}]
Its derivatives from zeroth to second order are
          q  s   = A   e    i  ( &#x03C9; &#x03C4; + &#x03C6; )   ,      d   q
      s      d  &#x03C4;    =  i  &#x03C9; A   e    i  ( &#x03C9; &#x03C4; +
      &#x03C6; )   ,       d   2    q  s      d   &#x03C4;  2      = &#x2212;
      &#x03C9;  2   A   e    i  ( &#x03C9; &#x03C4; + &#x03C6; )   .
      {\displaystyle q_{s}=A\mathrm {e} ^{\mathrm {i} (\omega \tau +\varphi
      )},\quad {\frac {\mathrm {d} q_{s}}{\mathrm {d} \tau }}=\mathrm {i}
      \omega A\mathrm {e} ^{\mathrm {i} (\omega \tau +\varphi )},\quad {\frac
      {\mathrm {d} ^{2}q_{s}}{\mathrm {d} \tau ^{2}}}=-\omega ^{2}A\mathrm {e}
      ^{\mathrm {i} (\omega \tau +\varphi )}.}  [{\displaystyle q_{s}=A\mathrm
      {e} ^{\mathrm {i} (\omega \tau +\varphi )},\quad {\frac {\mathrm {d} q_
      {s}}{\mathrm {d} \tau }}=\mathrm {i} \omega A\mathrm {e} ^{\mathrm {i}
      (\omega \tau +\varphi )},\quad {\frac {\mathrm {d} ^{2}q_{s}}{\mathrm {d}
      \tau ^{2}}}=-\omega ^{2}A\mathrm {e} ^{\mathrm {i} (\omega \tau +\varphi
      )}.}]
Substituting these quantities into the differential equation gives
         &#x2212;  &#x03C9;  2   A   e    i  ( &#x03C9; &#x03C4; + &#x03C6; )
      + 2 &#x03B6;  i  &#x03C9; A   e    i  ( &#x03C9; &#x03C4; + &#x03C6; )
      + A   e    i  ( &#x03C9; &#x03C4; + &#x03C6; )   = ( &#x2212;  &#x03C9;
      2   A + 2 &#x03B6;  i  &#x03C9; A + A )   e    i  ( &#x03C9; &#x03C4; +
      &#x03C6; )   =   e    i  &#x03C9; &#x03C4;   .   {\displaystyle -\omega ^
      {2}A\mathrm {e} ^{\mathrm {i} (\omega \tau +\varphi )}+2\zeta \mathrm {i}
      \omega A\mathrm {e} ^{\mathrm {i} (\omega \tau +\varphi )}+A\mathrm {e} ^
      {\mathrm {i} (\omega \tau +\varphi )}=(-\omega ^{2}A+2\zeta \mathrm {i}
      \omega A+A)\mathrm {e} ^{\mathrm {i} (\omega \tau +\varphi )}=\mathrm {e}
      ^{\mathrm {i} \omega \tau }.}  [{\displaystyle -\omega ^{2}A\mathrm {e} ^
      {\mathrm {i} (\omega \tau +\varphi )}+2\zeta \mathrm {i} \omega A\mathrm
      {e} ^{\mathrm {i} (\omega \tau +\varphi )}+A\mathrm {e} ^{\mathrm {i}
      (\omega \tau +\varphi )}=(-\omega ^{2}A+2\zeta \mathrm {i} \omega
      A+A)\mathrm {e} ^{\mathrm {i} (\omega \tau +\varphi )}=\mathrm {e} ^
      {\mathrm {i} \omega \tau }.}]
Dividing by the exponential term on the left results in
         &#x2212;  &#x03C9;  2   A + 2 &#x03B6;  i  &#x03C9; A + A =   e
      &#x2212;  i  &#x03C6;   = cos &#x2061; &#x03C6; &#x2212;  i  sin &#x2061;
      &#x03C6; .   {\displaystyle -\omega ^{2}A+2\zeta \mathrm {i} \omega
      A+A=\mathrm {e} ^{-\mathrm {i} \varphi }=\cos \varphi -\mathrm {i} \sin
      \varphi .}  [{\displaystyle -\omega ^{2}A+2\zeta \mathrm {i} \omega
      A+A=\mathrm {e} ^{-\mathrm {i} \varphi }=\cos \varphi -\mathrm {i} \sin
      \varphi .}]
Equating the real and imaginary parts results in two independent equations
         A ( 1 &#x2212;  &#x03C9;  2   ) = cos &#x2061; &#x03C6; ,  2 &#x03B6;
      &#x03C9; A = &#x2212; sin &#x2061; &#x03C6; .   {\displaystyle A(1-\omega
      ^{2})=\cos \varphi ,\quad 2\zeta \omega A=-\sin \varphi .}  [
      {\displaystyle A(1-\omega ^{2})=\cos \varphi ,\quad 2\zeta \omega A=-\sin
      \varphi .}]
*** Amplitude part[edit] ***
Bode_plot of the frequency response of an ideal harmonic oscillator
Squaring both equations and adding them together gives
                A  2   ( 1 &#x2212;  &#x03C9;  2    )  2      =  cos  2
      &#x2061; &#x03C6;     ( 2 &#x03B6; &#x03C9; A  )  2      =  sin  2
      &#x2061; &#x03C6;     }  &#x21D2;  A  2   [ ( 1 &#x2212;  &#x03C9;  2
      )  2   + ( 2 &#x03B6; &#x03C9;  )  2   ] = 1.   {\displaystyle \left.
      {\begin{aligned}A^{2}(1-\omega ^{2})^{2}&=\cos ^{2}\varphi \\(2\zeta
      \omega A)^{2}&=\sin ^{2}\varphi \end{aligned}}\right\}\Rightarrow A^{2}[
      (1-\omega ^{2})^{2}+(2\zeta \omega )^{2}]=1.}  [{\displaystyle \left.
      {\begin{aligned}A^{2}(1-\omega ^{2})^{2}&=\cos ^{2}\varphi \\(2\zeta
      \omega A)^{2}&=\sin ^{2}\varphi \end{aligned}}\right\}\Rightarrow A^{2}[
      (1-\omega ^{2})^{2}+(2\zeta \omega )^{2}]=1.}]
Therefore,
         A = A ( &#x03B6; , &#x03C9; ) = sign &#x2061;  (    &#x2212; sin
      &#x2061; &#x03C6;   2 &#x03B6; &#x03C9;    )    1  ( 1 &#x2212;  &#x03C9;
      2    )  2   + ( 2 &#x03B6; &#x03C9;  )  2      .   {\displaystyle A=A
      (\zeta ,\omega )=\operatorname {sign} \left({\frac {-\sin \varphi }
      {2\zeta \omega }}\right){\frac {1}{\sqrt {(1-\omega ^{2})^{2}+(2\zeta
      \omega )^{2}}}}.}  [{\displaystyle A=A(\zeta ,\omega )=\operatorname
      {sign} \left({\frac {-\sin \varphi }{2\zeta \omega }}\right){\frac {1}
      {\sqrt {(1-\omega ^{2})^{2}+(2\zeta \omega )^{2}}}}.}]
Compare this result with the theory section on resonance, as well as the
"magnitude part" of the RLC_circuit. This amplitude function is particularly
important in the analysis and understanding of the frequency_response of
second-order systems.
*** Phase part[edit] ***
To solve for Ï, divide both equations to get
         tan &#x2061; &#x03C6; = &#x2212;    2 &#x03B6; &#x03C9;   1 &#x2212;
      &#x03C9;  2      =    2 &#x03B6; &#x03C9;    &#x03C9;  2   &#x2212; 1
      &#x21D2; &#x03C6; &#x2261; &#x03C6; ( &#x03B6; , &#x03C9; ) = arctan
      &#x2061;  (    2 &#x03B6; &#x03C9;    &#x03C9;  2   &#x2212; 1    )  + n
      &#x03C0; .   {\displaystyle \tan \varphi =-{\frac {2\zeta \omega }{1-
      \omega ^{2}}}={\frac {2\zeta \omega }{\omega ^{2}-1}}\Rightarrow \varphi
      \equiv \varphi (\zeta ,\omega )=\arctan \left({\frac {2\zeta \omega }
      {\omega ^{2}-1}}\right)+n\pi .}  [{\displaystyle \tan \varphi =-{\frac
      {2\zeta \omega }{1-\omega ^{2}}}={\frac {2\zeta \omega }{\omega ^{2}-
      1}}\Rightarrow \varphi \equiv \varphi (\zeta ,\omega )=\arctan \left(
      {\frac {2\zeta \omega }{\omega ^{2}-1}}\right)+n\pi .}]
This phase function is particularly important in the analysis and understanding
of the frequency_response of second-order systems.
**** Full solution[edit] ****
Combining the amplitude and phase portions results in the steady-state solution
          q  s   ( &#x03C4; ) = A ( &#x03B6; , &#x03C9; ) cos &#x2061;
      ( &#x03C9; &#x03C4; + &#x03C6; ( &#x03B6; , &#x03C9; ) ) = A cos &#x2061;
      ( &#x03C9; &#x03C4; + &#x03C6; ) .   {\displaystyle q_{s}(\tau )=A(\zeta
      ,\omega )\cos(\omega \tau +\varphi (\zeta ,\omega ))=A\cos(\omega \tau
      +\varphi ).}  [{\displaystyle q_{s}(\tau )=A(\zeta ,\omega )\cos(\omega
      \tau +\varphi (\zeta ,\omega ))=A\cos(\omega \tau +\varphi ).}]
The solution of original universal oscillator equation is a superposition (sum)
of the transient and steady-state solutions:
         q ( &#x03C4; ) =  q  t   ( &#x03C4; ) +  q  s   ( &#x03C4; ) .
      {\displaystyle q(\tau )=q_{t}(\tau )+q_{s}(\tau ).}  [{\displaystyle q
      (\tau )=q_{t}(\tau )+q_{s}(\tau ).}]
For a more complete description of how to solve the above equation, see linear
ODEs_with_constant_coefficients.
***** Equivalent systems[edit] *****
Main article: System_equivalence
Harmonic oscillators occurring in a number of areas of engineering are
equivalent in the sense that their mathematical models are identical (see
universal_oscillator_equation above). Below is a table showing analogous
quantities in four harmonic oscillator systems in mechanics and electronics. If
analogous parameters on the same line in the table are given numerically equal
values, the behavior of the oscillators – their output waveform, resonant
frequency, damping factor, etc. – are the same.
Translational       Rotational          Series_RLC_circuit  Parallel_RLC
mechanical          mechanical                              circuit
                                                            Flux_linkage
Position     x      Angle     &#x03B8;  Charge     q        &#x03C6;
{\displaystyle x}   {\displaystyle      {\displaystyle q}   {\displaystyle
[x]                 \theta }  [\theta ] [q]                 \varphi }  [\varphi
                                                            ]
Velocity         d  Angular_velocity    Current         d   Voltage         d
x    d  t           d  &#x03B8;    d  t q    d  t           &#x03C6;    d  t
{\displaystyle      {\displaystyle      {\displaystyle      {\displaystyle
{\frac {\mathrm {d} {\frac {\mathrm {d} {\frac {\mathrm {d} {\frac {\mathrm {d}
x}{\mathrm {d} t}}} \theta }{\mathrm    q}{\mathrm {d} t}}} \varphi }{\mathrm
[{\displaystyle     {d} t}}}  [         [{\displaystyle     {d} t}}}  [
{\frac {\mathrm {d} {\displaystyle      {\frac {\mathrm {d} {\displaystyle
x}{\mathrm {d}      {\frac {\mathrm {d} q}{\mathrm {d}      {\frac {\mathrm {d}
t}}}]               \theta }{\mathrm    t}}}]               \varphi }{\mathrm
                    {d} t}}}]                               {d} t}}}]
Mass     m          Moment_of_inertia   Inductance     L    Capacitance     C
{\displaystyle m}   I   {\displaystyle  {\displaystyle L}   {\displaystyle C}
[m]                 I}  [I]             [L]                 [C]
Spring_constant     Torsion_constant    Elastance     1  /  Magnetic_reluctance
k   {\displaystyle  &#x03BC;            C   {\displaystyle  1  /  L
k}  [k]             {\displaystyle \mu  1/C}  [1/C]         {\displaystyle 1/L}
                    }  [\mu ]                               [1/L]
                    Rotational_friction                     Conductance     G =
Damping     c       &#x0393;            Resistance     R    1  /  R
{\displaystyle c}   {\displaystyle      {\displaystyle R}   {\displaystyle G=1/
[c]                 \Gamma }  [\Gamma ] [R]                 R}  [{\displaystyle
                                                            G=1/R}]
Drive force     F   Drive torque        Voltage     e       Current     i
( t )               &#x03C4; ( t )      {\displaystyle e}   {\displaystyle i}
{\displaystyle F    {\displaystyle \tau [e]                 [i]
(t)}  [F(t)]        (t)}  [\tau (t)]
    Undamped resonant_frequency      f  n     {\displaystyle f_{n}}  [f_{n}]:
     1  2 &#x03C0;       1  2 &#x03C0;       1  2 &#x03C0;       1  2 &#x03C0;
k m                 &#x03BC; I          1  L C              1  L C
{\displaystyle      {\displaystyle      {\displaystyle      {\displaystyle
{\frac {1}{2\pi }}  {\frac {1}{2\pi }}  {\frac {1}{2\pi }}  {\frac {1}{2\pi }}
{\sqrt {\frac {k}   {\sqrt {\frac {\mu  {\sqrt {\frac {1}   {\sqrt {\frac {1}
{m}}}}  [           }{I}}}}  [          {LC}}}}  [          {LC}}}}  [
{\displaystyle      {\displaystyle      {\displaystyle      {\displaystyle
{\frac {1}{2\pi }}  {\frac {1}{2\pi }}  {\frac {1}{2\pi }}  {\frac {1}{2\pi }}
{\sqrt {\frac {k}   {\sqrt {\frac {\mu  {\sqrt {\frac {1}   {\sqrt {\frac {1}
{m}}}}]             }{I}}}}]            {LC}}}}]            {LC}}}}]
            Damping_ratio     &#x03B6;   {\displaystyle \zeta }  [\zeta ]:
     c 2      1  k       &#x0393; 2          R 2      C L        G 2      L C
m                   1  I &#x03BC;       {\displaystyle      {\displaystyle
{\displaystyle      {\displaystyle      {\frac {R}{2}}      {\frac {G}{2}}
{\frac {c}{2}}      {\frac {\Gamma }    {\sqrt {\frac {C}   {\sqrt {\frac {L}
{\sqrt {\frac {1}   {2}}{\sqrt {\frac   {L}}}}  [           {C}}}}  [
{km}}}}  [          {1}{I\mu }}}}  [    {\displaystyle      {\displaystyle
{\displaystyle      {\displaystyle      {\frac {R}{2}}      {\frac {G}{2}}
{\frac {c}{2}}      {\frac {\Gamma }    {\sqrt {\frac {C}   {\sqrt {\frac {L}
{\sqrt {\frac {1}   {2}}{\sqrt {\frac   {L}}}}]             {C}}}}]
{km}}}}]            {1}{I\mu }}}}]
                                          Differential equation:
                       I    &#x03B8;
                    &#x00A8;    +
                    &#x0393;                                   C    &#x03C6;
   m    x &#x00A8;  &#x03B8; &#x02D9;      L    q &#x00A8;  &#x00A8;    + G
+ c    x &#x02D9;   + &#x03BC; &#x03B8; + R    q &#x02D9;   &#x03C6; &#x02D9;
+ k x = F           = &#x03C4;          + q  /  C = e       + &#x03C6;  /  L =
{\displaystyle m    {\displaystyle I    {\displaystyle L    i   {\displaystyle
{\ddot {x}}+c{\dot  {\ddot {\theta      {\ddot {q}}+R{\dot  C{\ddot {\varphi
{x}}+kx=F}  [       }}+\Gamma {\dot     {q}}+q/C=e}  [      }}+G{\dot {\varphi
{\displaystyle m    {\theta }}+\mu      {\displaystyle L    }}+\varphi /L=i}  [
{\ddot {x}}+c{\dot  \theta =\tau }  [   {\ddot {q}}+R{\dot  {\displaystyle C
{x}}+kx=F}]         {\displaystyle I    {q}}+q/C=e}]        {\ddot {\varphi
                    {\ddot {\theta                          }}+G{\dot {\varphi
                    }}+\Gamma {\dot                         }}+\varphi /L=i}]
                    {\theta }}+\mu
                    \theta =\tau }]
***** Application to a conservative force[edit] *****
The problem of the simple harmonic oscillator occurs frequently in physics,
because a mass at equilibrium under the influence of any conservative_force, in
the limit of small motions, behaves as a simple harmonic oscillator.
A conservative force is one that is associated with a potential_energy. The
potential-energy function of a harmonic oscillator is
         V ( x ) =   1 2   k  x  2   .   {\displaystyle V(x)={\frac {1}{2}}kx^
      {2}.}  [{\displaystyle V(x)={\frac {1}{2}}kx^{2}.}]
Given an arbitrary potential-energy function     V ( x )   {\displaystyle V(x)}
[V(x)], one can do a Taylor_expansion in terms of     x   {\displaystyle x}
[x] around an energy minimum (    x =  x  0     {\displaystyle x=x_{0}}  [x=x_
{0}]) to model the behavior of small perturbations from equilibrium.
         V ( x ) = V (  x  0   ) +  V &#x2032;  (  x  0   ) &#x22C5; ( x
      &#x2212;  x  0   ) +   1 2    V  ( 2 )   (  x  0   ) &#x22C5; ( x
      &#x2212;  x  0    )  2   + O ( x &#x2212;  x  0    )  3   .
      {\displaystyle V(x)=V(x_{0})+V'(x_{0})\cdot (x-x_{0})+{\frac {1}{2}}V^{
      (2)}(x_{0})\cdot (x-x_{0})^{2}+O(x-x_{0})^{3}.}  [{\displaystyle V(x)=V
      (x_{0})+V'(x_{0})\cdot (x-x_{0})+{\frac {1}{2}}V^{(2)}(x_{0})\cdot (x-x_
      {0})^{2}+O(x-x_{0})^{3}.}]
Because     V (  x  0   )   {\displaystyle V(x_{0})}  [V(x_{0})] is a minimum,
the first derivative evaluated at      x  0     {\displaystyle x_{0}}  [x_{0}]
must be zero, so the linear term drops out:
         V ( x ) = V (  x  0   ) +   1 2    V  ( 2 )   (  x  0   ) &#x22C5; ( x
      &#x2212;  x  0    )  2   + O ( x &#x2212;  x  0    )  3   .
      {\displaystyle V(x)=V(x_{0})+{\frac {1}{2}}V^{(2)}(x_{0})\cdot (x-x_{0})^
      {2}+O(x-x_{0})^{3}.}  [{\displaystyle V(x)=V(x_{0})+{\frac {1}{2}}V^{(2)}
      (x_{0})\cdot (x-x_{0})^{2}+O(x-x_{0})^{3}.}]
The constant_term V(x0) is arbitrary and thus may be dropped, and a coordinate
transformation allows the form of the simple harmonic oscillator to be
retrieved:
         V ( x ) &#x2248;   1 2    V  ( 2 )   ( 0 ) &#x22C5;  x  2   =   1 2
      k  x  2   .   {\displaystyle V(x)\approx {\frac {1}{2}}V^{(2)}(0)\cdot x^
      {2}={\frac {1}{2}}kx^{2}.}  [{\displaystyle V(x)\approx {\frac {1}{2}}V^{
      (2)}(0)\cdot x^{2}={\frac {1}{2}}kx^{2}.}]
Thus, given an arbitrary potential-energy function     V ( x )   {\displaystyle
V(x)}  [V(x)] with a non-vanishing second derivative, one can use the solution
to the simple harmonic oscillator to provide an approximate solution for small
perturbations around the equilibrium point.
***** Examples[edit] *****
**** Simple pendulum[edit] ****
A simple_pendulum exhibits approximately simple harmonic motion under the
conditions of no damping and small amplitude.
Assuming no damping, the differential equation governing a simple pendulum of
length     l   {\displaystyle l}  [l], where     g   {\displaystyle g}  [g] is
the local acceleration_of_gravity, is
             d  2   &#x03B8;   d  t  2      +   g l   sin &#x2061; &#x03B8; =
      0.   {\displaystyle {\frac {d^{2}\theta }{dt^{2}}}+{\frac {g}{l}}\sin
      \theta =0.}  [{\displaystyle {\frac {d^{2}\theta }{dt^{2}}}+{\frac {g}
      {l}}\sin \theta =0.}]
If the maximal displacement of the pendulum is small, we can use the
approximation     sin &#x2061; &#x03B8; &#x2248; &#x03B8;   {\displaystyle \sin
\theta \approx \theta }  [\sin \theta \approx \theta ] and instead consider the
equation
             d  2   &#x03B8;   d  t  2      +   g l   &#x03B8; = 0.
      {\displaystyle {\frac {d^{2}\theta }{dt^{2}}}+{\frac {g}{l}}\theta =0.}
      [{\displaystyle {\frac {d^{2}\theta }{dt^{2}}}+{\frac {g}{l}}\theta =0.}]
The general solution to this differential equation is
         &#x03B8; ( t ) = A cos &#x2061;  (     g l    t + &#x03C6;  )  ,
      {\displaystyle \theta (t)=A\cos \left({\sqrt {\frac {g}{l}}}t+\varphi
      \right),}  [{\displaystyle \theta (t)=A\cos \left({\sqrt {\frac {g}
      {l}}}t+\varphi \right),}]
where     A   {\displaystyle A}  [A] and     &#x03C6;   {\displaystyle \varphi
}  [\varphi ] are constants that depends on the initial conditions. Using as
initial conditions     &#x03B8; ( 0 ) =  &#x03B8;  0     {\displaystyle \theta
(0)=\theta _{0}}  [{\displaystyle \theta (0)=\theta _{0}}] and        &#x03B8;
&#x02D9;    ( 0 ) = 0   {\displaystyle {\dot {\theta }}(0)=0}  [{\displaystyle
{\dot {\theta }}(0)=0}], the solution is given by
         &#x03B8; ( t ) =  &#x03B8;  0   cos &#x2061;  (     g l    t  )  ,
      {\displaystyle \theta (t)=\theta _{0}\cos \left({\sqrt {\frac {g}
      {l}}}t\right),}  [{\displaystyle \theta (t)=\theta _{0}\cos \left({\sqrt
      {\frac {g}{l}}}t\right),}]
where      &#x03B8;  0     {\displaystyle \theta _{0}}  [\theta _{0}] is the
largest angle attained by the pendulum (that is,      &#x03B8;  0
{\displaystyle \theta _{0}}  [\theta _{0}] is the amplitude of the pendulum).
The period, the time for one complete oscillation, is given by the expression
         &#x03C4; = 2 &#x03C0;    l g    =    2 &#x03C0;  &#x03C9;   ,
      {\displaystyle \tau =2\pi {\sqrt {\frac {l}{g}}}={\frac {2\pi }{\omega
      }},}  [{\displaystyle \tau =2\pi {\sqrt {\frac {l}{g}}}={\frac {2\pi }
      {\omega }},}]
which is a good approximation of the actual period when      &#x03B8;  0
{\displaystyle \theta _{0}}  [\theta _{0}] is small. Notice that in this
approximation the period     &#x03C4;   {\displaystyle \tau }  [\tau ] is
independent of the amplitude      &#x03B8;  0     {\displaystyle \theta _{0}}
[\theta _{0}]. In the above equation,     &#x03C9;   {\displaystyle \omega }
[\omega ] represents the angular frequency.
**** Spring/mass system[edit] ****
Springâmass system in equilibrium (A), compressed (B) and stretched (C)
states
When a spring is stretched or compressed by a mass, the spring develops a
restoring force. Hooke's_law gives the relationship of the force exerted by the
spring when the spring is compressed or stretched a certain length:
         F ( t ) = &#x2212; k x ( t ) ,   {\displaystyle F(t)=-kx(t),}  [
      {\displaystyle F(t)=-kx(t),}]
where F is the force, k is the spring constant, and x is the displacement of
the mass with respect to the equilibrium position. The minus sign in the
equation indicates that the force exerted by the spring always acts in a
direction that is opposite to the displacement (i.e. the force always acts
towards the zero position), and so prevents the mass from flying off to
infinity.
By using either force balance or an energy method, it can be readily shown that
the motion of this system is given by the following differential equation:
         F ( t ) = &#x2212; k x ( t ) = m     d   2     d   t  2      x ( t ) =
      m a ,   {\displaystyle F(t)=-kx(t)=m{\frac {\mathrm {d} ^{2}}{\mathrm {d}
      t^{2}}}x(t)=ma,}  [{\displaystyle F(t)=-kx(t)=m{\frac {\mathrm {d} ^{2}}
      {\mathrm {d} t^{2}}}x(t)=ma,}]
the latter being Newton's_second_law_of_motion.
If the initial displacement is A, and there is no initial velocity, the
solution of this equation is given by
         x ( t ) = A cos &#x2061;  (     k m    t  )  .   {\displaystyle x
      (t)=A\cos \left({\sqrt {\frac {k}{m}}}t\right).}  [{\displaystyle x
      (t)=A\cos \left({\sqrt {\frac {k}{m}}}t\right).}]
Given an ideal massless spring,     m   {\displaystyle m}  [m] is the mass on
the end of the spring. If the spring itself has mass, its effective_mass must
be included in     m   {\displaystyle m}  [m].
*** Energy variation in the springâdamping system[edit] ***
In terms of energy, all systems have two types of energy: potential_energy and
kinetic_energy. When a spring is stretched or compressed, it stores elastic
potential energy, which then is transferred into kinetic energy. The potential
energy within a spring is determined by the equation     U = k  x  2    /  2.
{\displaystyle U=kx^{2}/2.}  [{\displaystyle U=kx^{2}/2.}]
When the spring is stretched or compressed, kinetic energy of the mass gets
converted into potential energy of the spring. By conservation of energy,
assuming the datum is defined at the equilibrium position, when the spring
reaches its maximal potential energy, the kinetic energy of the mass is zero.
When the spring is released, it tries to return to equilibrium, and all its
potential energy converts to kinetic energy of the mass.
***** Definition of terms[edit] *****
Symbol                 Definition              Dimensions              SI units
                                                   L  T  &#x2212; 2
   a   {\displaystyle                          {\displaystyle \mathbf
a}  [a]                Acceleration of mass    {LT^{-2}} }  [          m/s2
                                               {\displaystyle \mathbf
                                               {LT^{-2}} }]
   A   {\displaystyle  Peak amplitude of           L    {\displaystyle
A}  [A]                oscillation             \mathbf {L} }  [\mathbf m
                                               {L} ]
                                                   M  T  &#x2212; 1
   c   {\displaystyle  Viscous damping         {\displaystyle \mathbf
c}  [c]                coefficient             {MT^{-1}} }  [          NÂ·s/m
                                               {\displaystyle \mathbf
                                               {MT^{-1}} }]
                                                    T  &#x2212; 1
   f   {\displaystyle                          {\displaystyle \mathbf
f}  [f]                Frequency               {T^{-1}} }  [           Hz
                                               {\displaystyle \mathbf
                                               {T^{-1}} }]
                                                   M L  T  &#x2212; 2
   F   {\displaystyle                          {\displaystyle \mathbf
F}  [F]                Drive force             {MLT^{-2}} }  [         N
                                               {\displaystyle \mathbf
                                               {MLT^{-2}} }]
                                                   L  T  &#x2212; 2
   g   {\displaystyle  Acceleration of gravity {\displaystyle \mathbf
g}  [g]                at the Earth's surface  {LT^{-2}} }  [          m/s2
                                               {\displaystyle \mathbf
                                               {LT^{-2}} }]
                       Imaginary unit,
   i   {\displaystyle  &#x2212; 1              â                  â
i}  [i]                {\displaystyle {\sqrt
                       {-1}}}  [{\sqrt {-1}}]
                                                   M  T  &#x2212; 2
   k   {\displaystyle                          {\displaystyle \mathbf
k}  [k]                Spring constant         {MT^{-2}} }  [          N/m
                                               {\displaystyle \mathbf
                                               {MT^{-2}} }]
   m , M                                           M    {\displaystyle
{\displaystyle m,M}  [ Mass                    \mathbf {M} }  [\mathbf kg
{\displaystyle m,M}]                           {M} ]
   Q   {\displaystyle  Quality factor          â                  â
Q}  [Q]
   T   {\displaystyle                              T    {\displaystyle
T}  [T]                Period of oscillation   \mathbf {T} }  [\mathbf s
                                               {T} ]
   t   {\displaystyle                              T    {\displaystyle
t}  [t]                Time                    \mathbf {T} }  [\mathbf s
                                               {T} ]
                                                   M  L  2    T
                                               &#x2212; 2
   U   {\displaystyle  Potential energy stored {\displaystyle \mathbf  J
U}  [U]                in oscillator           {ML^{2}T^{-2}} }  [
                                               {\displaystyle \mathbf
                                               {ML^{2}T^{-2}} }]
   x   {\displaystyle                              L    {\displaystyle
x}  [x]                Position of mass        \mathbf {L} }  [\mathbf m
                                               {L} ]
   &#x03B6;
{\displaystyle \zeta } Damping ratio           â                  â
[\zeta ]
   &#x03C6;
{\displaystyle \varphi Phase shift             â                  rad
}  [\varphi ]
                                                    T  &#x2212; 1
   &#x03C9;                                    {\displaystyle \mathbf
{\displaystyle \omega  Angular frequency       {T^{-1}} }  [           rad/s
}  [\omega ]                                   {\displaystyle \mathbf
                                               {T^{-1}} }]
                                                    T  &#x2212; 1
    &#x03C9;  0        Natural resonant        {\displaystyle \mathbf
{\displaystyle \omega  angular frequency       {T^{-1}} }  [           rad/s
_{0}}  [\omega _{0}]                           {\displaystyle \mathbf
                                               {T^{-1}} }]
***** See also[edit] *****
    * Anharmonic_oscillator
    * Critical_speed
    * Effective_mass_(spring-mass_system)
    * Normal_mode
    * Parametric_oscillator
    * Phasor
    * Q_factor
    * Quantum_harmonic_oscillator
    * Radial_harmonic_oscillator
    * Spring_pendulum
***** Notes[edit] *****
   1. ^ Fowles_&_Cassiday_(1986, p. 86)
   2. ^ Kreyszig_(1972, p. 65)
   3. ^ Tipler_(1998, pp. 369,389)
   4. ^Case, William. "Two_ways_of_driving_a_child's_swing". Archived from the
      original on 9 December 2011. Retrieved 27 November 2011.
   5. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   6. ^Case, W. B. (1996). "The pumping of a swing from the standing position".
      American Journal of Physics. 64 (3): 215â220. Bibcode:
      1996AmJPh..64..215C. doi:10.1119/1.18209.
   7. ^Roura, P.; Gonzalez, J.A. (2010). "Towards a more realistic description
      of swing pumping due to the exchange of angular momentum". European
      Journal of Physics. 31 (5): 1195â1207. Bibcode:2010EJPh...31.1195R.
      doi:10.1088/0143-0807/31/5/020.
***** References[edit] *****
    * Fowles, Grant R.; Cassiday, George L. (1986), Analytic Mechanics (5th
      ed.), Fort Worth: Saunders_College_Publishing, ISBN 0-03-96746-5,
      LCCN 93085193CS1 maint: Ignored ISBN errors (link)
Hayek, Sabih I. (15 Apr 2003). "Mechanical Vibration and Damping". Encyclopedia
of Applied Physics. WILEY-VCH Verlag GmbH & Co KGaA. doi:10.1002/
3527600434.eap231. ISBN 9783527600434.
Kreyszig,_Erwin (1972), Advanced Engineering Mathematics (3rd ed.), New York:
Wiley, ISBN 0-471-50728-8
Serway, Raymond A.; Jewett, John W. (2003). Physics for Scientists and
Engineers. Brooks/Cole. ISBN 0-534-40842-7.
Tipler, Paul (1998). Physics for Scientists and Engineers: Vol. 1 (4th ed.). W.
H. Freeman. ISBN 1-57259-492-6.
Wylie, C. R. (1975). Advanced Engineering Mathematics (4th ed.). McGraw-Hill.
ISBN 0-07-072180-7.
***** External links[edit] *****
 Wikimedia Commons has media related to Harmonic_oscillation.
    * The_Harmonic_Oscillator from The_Feynman_Lectures_on_Physics
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Oscillator,_harmonic",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Harmonic_Oscillator from The Chaos Hypertextbook
A_Java_applet_of_harmonic_oscillator_with_damping_proportional_to_velocity_or
damping_caused_by_dry_friction

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Harmonic_oscillator&oldid=906436579"
Categories:
    * Mechanical_vibrations
    * Ordinary_differential_equations
    * Oscillators
Hidden categories:
    * Use_American_English_from_February_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_October_2018
    * CS1_maint:_Ignored_ISBN_errors
    * Commons_category_link_is_locally_defined
    * Articles_containing_video_clips
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
    * Asturianu
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * LietuviÅ³
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * à·à·à¶à·à¶½
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 15 July 2019, at 20:36 (UTC).
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
