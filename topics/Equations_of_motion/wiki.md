The following text has been accessed from https://en.wikipedia.org/wiki/Equations_of_motion at Thu Aug 8 23:17:35 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Equations of motion ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"SUVAT" redirects here. For the village in Azerbaijan, see Suvat,_Azerbaijan.
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
    * Equations of motion
    * Euler's_laws_of_motion
    * Fictitious_force
    * Friction
    * Harmonic_oscillator
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
   v   {\displaystyle v}  [v] vs     t   {\displaystyle t}  [t] graph for a
moving particle under a non uniformed acceleration     a   {\displaystyle a}
[a].
In physics, equations of motion are equations that describe the behavior of a
physical_system in terms of its motion as a function of time.[1] More
specifically, the equations of motion describe the behaviour of a physical
system as a set of mathematical functions in terms of dynamic variables:
normally spatial coordinates and time are used, but others are also possible,
such as momentum components and time. The most general choice are generalized
coordinates which can be any convenient variables characteristic of the
physical system.[2] The functions are defined in a Euclidean_space in classical
mechanics, but are replaced by curved_spaces in relativity. If the dynamics of
a system is known, the equations are the solutions for the differential
equations describing the motion of the dynamics.
There are two main descriptions of motion: dynamics and kinematics. Dynamics is
general, since momenta, forces and energy of the particles are taken into
account. In this instance, sometimes the term refers to the differential
equations that the system satisfies (e.g., Newton's_second_law or
EulerâLagrange_equations), and sometimes to the solutions to those equations.
However, kinematics is simpler as it concerns only variables derived from the
positions of objects, and time. In circumstances of constant acceleration,
these simpler equations of motion are usually referred to as the SUVAT
equations, arising from the definitions of kinematic quantities: displacement
(s), initial velocity (u), final velocity (v), acceleration (a), and time (t).
Equations of motion can therefore be grouped under these main classifiers of
motion. In all cases, the main types of motion are translations, rotations,
oscillations, or any combinations of these.
A differential equation of motion, usually identified as some physical_law and
applying definitions of physical_quantities, is used to set up an equation for
the problem. Solving the differential equation will lead to a general solution
with arbitrary constants, the arbitrariness corresponding to a family of
solutions. A particular solution can be obtained by setting the initial_values,
which fixes the values of the constants.
To state this formally, in general an equation of motion M is a function of the
position r of the object, its velocity (the first time derivative of r, v = dr/
dt), and its acceleration (the second derivative of r, a = d2r/dt2), and time
t. Euclidean_vectors in 3D are denoted throughout in bold. This is equivalent
to saying an equation of motion in r is a second order ordinary_differential
equation (ODE) in r,
         M  [   r  ( t ) ,    r &#x02D9;    ( t ) ,    r &#x00A8;    ( t ) , t
      ]  = 0  ,   {\displaystyle M\left[\mathbf {r} (t),\mathbf {\dot {r}}
      (t),\mathbf {\ddot {r}} (t),t\right]=0\,,}  [M\left[\mathbf {r}
      (t),\mathbf {\dot {r}} (t),\mathbf {\ddot {r}} (t),t\right]=0\,,]
where t is time, and each overdot denotes one time_derivative. The initial
conditions are given by the constant values at t = 0,
          r  ( 0 )  ,     r &#x02D9;    ( 0 )  .   {\displaystyle \mathbf {r}
      (0)\,,\quad \mathbf {\dot {r}} (0)\,.}  [\mathbf {r} (0)\,,\quad \mathbf
      {\dot {r}} (0)\,.]
The solution r(t) to the equation of motion, with specified initial values,
describes the system for all times t after t = 0. Other dynamical variables
like the momentum p of the object, or quantities derived from r and p like
angular_momentum, can be used in place of r as the quantity to solve for from
some equation of motion, although the position of the object at time t is by
far the most sought-after quantity.
Sometimes, the equation will be linear and is more likely to be exactly
solvable. In general, the equation will be non-linear, and cannot be solved
exactly so a variety of approximations must be used. The solutions to nonlinear
equations may show chaotic behavior depending on how sensitive the system is to
the initial conditions.
⁰
***** Contents *****
    * 1_History
    * 2_Kinematic_equations_for_one_particle
          o 2.1_Kinematic_quantities
          o 2.2_Uniform_acceleration
                # 2.2.1_Constant_translational_acceleration_in_a_straight_line
                # 2.2.2_Constant_linear_acceleration_in_any_direction
                # 2.2.3_Applications
                # 2.2.4_Constant_circular_acceleration
          o 2.3_General_planar_motion
          o 2.4_General_3D_motions
    * 3_Dynamic_equations_of_motion
          o 3.1_Newtonian_mechanics
          o 3.2_Applications
    * 4_Analytical_mechanics
    * 5_Electrodynamics
    * 6_General_relativity
          o 6.1_Geodesic_equation_of_motion
          o 6.2_Spinning_objects
    * 7_Analogues_for_waves_and_fields
          o 7.1_Field_equations
          o 7.2_Wave_equations
          o 7.3_Quantum_theory
    * 8_See_also
    * 9_References
***** History[edit] *****
Historically, equations of motion first appeared in classical_mechanics to
describe the motion of massive_objects, a notable application was to celestial
mechanics to predict the motion of the planets as if they orbit like clockwork
(this was how Neptune was predicted before its discovery), and also investigate
the stability_of_the_solar_system.
It is important to observe that the huge body of work involving kinematics,
dynamics and the mathematical models of the universe developed in baby steps
â faltering, getting up and correcting itself â over three millennia and
included contributions of both known names and others who have since faded from
the annals of history.
In antiquity, notwithstanding the success of priests, astrologers and
astronomers in predicting solar and lunar eclipses, the solstices and the
equinoxes of the Sun and the period of the Moon, there was nothing other than a
set of algorithms to help them. Despite the great strides made in the
development of geometry made by Ancient Greeks and surveys in Rome, we were to
wait for another thousand years before the first equations of motion arrive.
The exposure of Europe to the collected works by the Muslims of the Greeks, the
Indians and the Islamic scholars, such as Euclidâs Elements, the works of
Archimedes, and Al-KhwÄrizmÄ«'s treatises [3] began in Spain, and scholars
from all over Europe went to Spain, read, copied and translated the learning
into Latin. The exposure of Europe to Arabic_numerals and their ease in
computations encouraged first the scholars to learn them and then the merchants
and invigorated the spread of knowledge throughout Europe.
By the 13th century the universities of Oxford and Paris had come up, and the
scholars were now studying mathematics and philosophy with lesser worries about
mundane chores of lifeâthe fields were not as clearly demarcated as they are
in the modern times. Of these, compendia and redactions, such as those of
Johannes_Campanus, of Euclid and Aristotle, confronted scholars with ideas
about infinity and the ratio theory of elements as a means of expressing
relations between various quantities involved with moving bodies. These studies
led to a new body of knowledge that is now known as physics.
Of these institutes Merton_College sheltered a group of scholars devoted to
natural science, mainly physics, astronomy and mathematics, of similar in
stature to the intellectuals at the University of Paris. Thomas_Bradwardine,
one of those scholars, extended Aristotelian quantities such as distance and
velocity, and assigned intensity and extension to them. Bradwardine suggested
an exponential law involving force, resistance, distance, velocity and time.
Nicholas_Oresme further extended Bradwardine's arguments. The Merton_school
proved that the quantity of motion of a body undergoing a uniformly accelerated
motion is equal to the quantity of a uniform motion at the speed achieved
halfway through the accelerated motion.
For writers on kinematics before Galileo, since small time intervals could not
be measured, the affinity between time and motion was obscure. They used time
as a function of distance, and in free fall, greater velocity as a result of
greater elevation. Only Domingo_de_Soto, a Spanish theologian, in his
commentary on Aristotle's Physics published in 1545, after defining "uniform
difform" motion (which is uniformly accelerated motion) â the word velocity
wasn't used â as proportional to time, declared correctly that this kind of
motion was identifiable with freely falling bodies and projectiles, without his
proving these propositions or suggesting a formula relating time, velocity and
distance. De Soto's comments are shockingly correct regarding the definitions
of acceleration (acceleration was a rate of change of motion (velocity) in
time) and the observation that during the violent motion of ascent acceleration
would be negative.
Discourses such as these spread throughout Europe and definitely influenced
Galileo and others, and helped in laying the foundation of kinematics.[4]
Galileo deduced the equation s = 1/2gt2 in his work geometrically,[5] using the
Merton_rule, now known as a special case of one of the equations of kinematics.
He couldn't use the now-familiar mathematical reasoning. The relationships
between speed, distance, time and acceleration was not known at the time.
Galileo was the first to show that the path of a projectile is a parabola.
Galileo had an understanding of centrifugal_force and gave a correct definition
of momentum. This emphasis of momentum as a fundamental quantity in dynamics is
of prime importance. He measured momentum by the product of velocity and
weight; mass is a later concept, developed by Huygens and Newton. In the
swinging of a simple pendulum, Galileo says in Discourses[6] that "every
momentum acquired in the descent along an arc is equal to that which causes the
same moving body to ascend through the same arc." His analysis on projectiles
indicates that Galileo had grasped the first law and the second law of motion.
He did not generalize and make them applicable to bodies not subject to the
earth's gravitation. That step was Newton's contribution.
The term "inertia" was used by Kepler who applied it to bodies at rest. (The
first law of motion is now often called the law of inertia.)
Galileo did not fully grasp the third law of motion, the law of the equality of
action and reaction, though he corrected some errors of Aristotle. With Stevin
and others Galileo also wrote on statics. He formulated the principle of the
parallelogram of forces, but he did not fully recognize its scope.
Galileo also was interested by the laws of the pendulum, his first observations
of which were as a young man. In 1583, while he was praying in the cathedral at
Pisa, his attention was arrested by the motion of the great lamp lighted and
left swinging, referencing his own pulse for time keeping. To him the period
appeared the same, even after the motion had greatly diminished, discovering
the isochronism of the pendulum.
More careful experiments carried out by him later, and described in his
Discourses, revealed the period of oscillation varies with the square root of
length but is independent of the mass the pendulum.
Thus we arrive at RenÃ©_Descartes, Isaac_Newton, Gottfried_Leibniz, et al.; and
the evolved forms of the equations of motion that begin to be recognized as the
modern ones.
Later the equations of motion also appeared in electrodynamics, when describing
the motion of charged particles in electric and magnetic fields, the Lorentz
force is the general equation which serves as the definition of what is meant
by an electric_field and magnetic_field. With the advent of special_relativity
and general_relativity, the theoretical modifications to spacetime meant the
classical equations of motion were also modified to account for the finite
speed_of_light, and curvature_of_spacetime. In all these cases the differential
equations were in terms of a function describing the particle's trajectory in
terms of space and time coordinates, as influenced by forces or energy
transformations.[7]
However, the equations of quantum_mechanics can also be considered "equations
of motion", since they are differential equations of the wavefunction, which
describes how a quantum state behaves analogously using the space and time
coordinates of the particles. There are analogs of equations of motion in other
areas of physics, for collections of physical phenomena that can be considered
waves, fluids, or fields.
***** Kinematic equations for one particle[edit] *****
**** Kinematic quantities[edit] ****
Kinematic quantities of a classical particle of mass m: position r, velocity v,
acceleration a.
From the instantaneous position r = r(t), instantaneous meaning at an instant
value of time t, the instantaneous velocity v = v(t) and acceleration a = a(t)
have the general, coordinate-independent definitions;[8]
          v  =    d  r    d t     ,   a  =    d  v    d t    =     d  2    r
      d  t  2          {\displaystyle \mathbf {v} ={\frac {d\mathbf {r} }
      {dt}}\,,\quad \mathbf {a} ={\frac {d\mathbf {v} }{dt}}={\frac {d^
      {2}\mathbf {r} }{dt^{2}}}\,\!}  [\mathbf {v} ={\frac {d\mathbf {r} }
      {dt}}\,,\quad \mathbf {a} ={\frac {d\mathbf {v} }{dt}}={\frac {d^
      {2}\mathbf {r} }{dt^{2}}}\,\!]
Notice that velocity always points in the direction of motion, in other words
for a curved path it is the tangent_vector. Loosely speaking, first order
derivatives are related to tangents of curves. Still for curved paths, the
acceleration is directed towards the center_of_curvature of the path. Again,
loosely speaking, second order derivatives are related to curvature.
The rotational analogues are the "angular vector" (angle the particle rotates
about some axis) Î¸ = Î¸(t), angular velocity Ï = Ï(t), and angular
acceleration Î± = Î±(t):
          &#x03B8;  = &#x03B8;     n  &#x005E;     ,   &#x03C9;  =    d
      &#x03B8;    d t     ,   &#x03B1;  =    d  &#x03C9;    d t     ,
      {\displaystyle {\boldsymbol {\theta }}=\theta {\hat {\mathbf {n}
      }}\,,\quad {\boldsymbol {\omega }}={\frac {d{\boldsymbol {\theta }}}
      {dt}}\,,\quad {\boldsymbol {\alpha }}={\frac {d{\boldsymbol {\omega }}}
      {dt}}\,,}  [{\boldsymbol {\theta }}=\theta {\hat {\mathbf {n} }}\,,\quad
      {\boldsymbol {\omega }}={\frac {d{\boldsymbol {\theta }}}{dt}}\,,\quad
      {\boldsymbol {\alpha }}={\frac {d{\boldsymbol {\omega }}}{dt}}\,,]
where nÌ is a unit_vector in the direction of the axis of rotation, and Î¸ is
the angle the object turns through about the axis.
The following relation holds for a point-like particle, orbiting about some
axis with angular velocity Ï:[9]
          v  =  &#x03C9;  &#x00D7;  r      {\displaystyle \mathbf {v} =
      {\boldsymbol {\omega }}\times \mathbf {r} \,\!}  [\mathbf {v} =
      {\boldsymbol {\omega }}\times \mathbf {r} \,\!]
where r is the position vector of the particle (radial from the rotation axis)
and v the tangential velocity of the particle. For a rotating continuum rigid
body, these relations hold for each point in the rigid body.
**** Uniform acceleration[edit] ****
The differential equation of motion for a particle of constant or uniform
acceleration in a straight line is simple: the acceleration is constant, so the
second derivative of the position of the object is constant. The results of
this case are summarized below.
*** Constant translational acceleration in a straight line[edit] ***
These equations apply to a particle moving linearly, in three dimensions in a
straight line with constant acceleration.[10] Since the position, velocity, and
acceleration are collinear (parallel, and lie on the same line) â only the
magnitudes of these vectors are necessary, and because the motion is along a
straight line, the problem effectively reduces from three dimensions to one.
             v    = a t +  v  0    [ 1 ]       {\displaystyle {\begin
      {aligned}v&=at+v_{0}\quad [1]\\\end{aligned}}}  [{\begin{aligned}v&=at+v_
      {0}\quad [1]\\\end{aligned}}]
             r    =  r  0   +  v  0   t +    1 2     a   t  2    [ 2 ]
      {\displaystyle {\begin{aligned}r&=r_{0}+v_{0}t+{\tfrac {1}{2}}{a}t^
      {2}\quad [2]\\\end{aligned}}}  [{\displaystyle {\begin{aligned}r&=r_
      {0}+v_{0}t+{\tfrac {1}{2}}{a}t^{2}\quad [2]\\\end{aligned}}}]
             r    =  r  0   +    1 2     (  v +  v  0    )  t  [ 3 ]      v  2
      =  v  0   2   + 2 a  (  r &#x2212;  r  0    )   [ 4 ]     r    =  r  0
      + v t &#x2212;    1 2     a   t  2    [ 5 ]       {\displaystyle {\begin
      {aligned}r&=r_{0}+{\tfrac {1}{2}}\left(v+v_{0}\right)t\quad [3]\\v^
      {2}&=v_{0}^{2}+2a\left(r-r_{0}\right)\quad [4]\\r&=r_{0}+vt-{\tfrac {1}
      {2}}{a}t^{2}\quad [5]\\\end{aligned}}}  [{\displaystyle {\begin
      {aligned}r&=r_{0}+{\tfrac {1}{2}}\left(v+v_{0}\right)t\quad [3]\\v^
      {2}&=v_{0}^{2}+2a\left(r-r_{0}\right)\quad [4]\\r&=r_{0}+vt-{\tfrac {1}
      {2}}{a}t^{2}\quad [5]\\\end{aligned}}}]
where:
    * r0 is the particle's initial position
    * r is the particle's final position
    * v0 is the particle's initial velocity
    * v is the particle's final velocity
    * a is the particle's acceleration
    * t is the time_interval
Derivation
Equations [1] and [2] are from integrating the definitions of velocity and
acceleration,[10] subject to the initial conditions r(t0) = r0 and v(t0) = v0;
              v     = &#x222B;  a  d t =  a  t +   v   0    ,  [ 1 ]      r
      = &#x222B; (  a  t +   v   0   ) d t =     a   t  2    2   +   v   0   t
      +   r   0    ,  [ 2 ]       {\displaystyle {\begin{aligned}\mathbf {v}
      &=\int \mathbf {a} dt=\mathbf {a} t+\mathbf {v} _{0}\,,\quad [1]\\\mathbf
      {r} &=\int (\mathbf {a} t+\mathbf {v} _{0})dt={\frac {\mathbf {a} t^{2}}
      {2}}+\mathbf {v} _{0}t+\mathbf {r} _{0}\,,\quad [2]\\\end{aligned}}}  [
      {\begin{aligned}\mathbf {v} &=\int \mathbf {a} dt=\mathbf {a} t+\mathbf
      {v} _{0}\,,\quad [1]\\\mathbf {r} &=\int (\mathbf {a} t+\mathbf {v} _
      {0})dt={\frac {\mathbf {a} t^{2}}{2}}+\mathbf {v} _{0}t+\mathbf {r} _
      {0}\,,\quad [2]\\\end{aligned}}]
in magnitudes,
             v    = a t +  v  0    ,  [ 1 ]     r    =     a   t  2    2   +  v
      0   t +  r  0    .  [ 2 ]       {\displaystyle {\begin{aligned}v&=at+v_
      {0}\,,\quad [1]\\r&={\frac {{a}t^{2}}{2}}+v_{0}t+r_{0}\,.\quad [2]\\\end
      {aligned}}}  [{\begin{aligned}v&=at+v_{0}\,,\quad [1]\\r&={\frac {{a}t^
      {2}}{2}}+v_{0}t+r_{0}\,.\quad [2]\\\end{aligned}}]
Equation [3] involves the average velocity v + v0/2. Intuitively, the velocity
increases linearly, so the average velocity multiplied by time is the distance
traveled while increasing the velocity from v0 to v, as can be illustrated
graphically by plotting velocity against time as a straight line graph.
Algebraically, it follows from solving [1] for
          a  =    (  v  &#x2212;   v   0   )  t     {\displaystyle \mathbf {a}
      ={\frac {(\mathbf {v} -\mathbf {v} _{0})}{t}}}  [\mathbf {a} ={\frac {
      (\mathbf {v} -\mathbf {v} _{0})}{t}}]
and substituting into [2]
          r  =   r   0   +   v   0   t +   t 2   (  v  &#x2212;   v   0   )  ,
      {\displaystyle \mathbf {r} =\mathbf {r} _{0}+\mathbf {v} _{0}t+{\frac {t}
      {2}}(\mathbf {v} -\mathbf {v} _{0})\,,}  [\mathbf {r} =\mathbf {r} _
      {0}+\mathbf {v} _{0}t+{\frac {t}{2}}(\mathbf {v} -\mathbf {v} _{0})\,,]
then simplifying to get
          r  =   r   0   +   t 2   (  v  +   v   0   )   {\displaystyle \mathbf
      {r} =\mathbf {r} _{0}+{\frac {t}{2}}(\mathbf {v} +\mathbf {v} _{0})}
      [\mathbf {r} =\mathbf {r} _{0}+{\frac {t}{2}}(\mathbf {v} +\mathbf {v} _
      {0})]
or in magnitudes
         r =  r  0   +  (    v +  v  0    2   )  t  [ 3 ]   {\displaystyle r=r_
      {0}+\left({\frac {v+v_{0}}{2}}\right)t\quad [3]}  [r=r_{0}+\left({\frac
      {v+v_{0}}{2}}\right)t\quad [3]]
From [3],
         t =  (  r &#x2212;  r  0    )   (   2  v +  v  0      )
      {\displaystyle t=\left(r-r_{0}\right)\left({\frac {2}{v+v_{0}}}\right)}
      [t=\left(r-r_{0}\right)\left({\frac {2}{v+v_{0}}}\right)]
substituting for t in [1]:
             v    = a  (  r &#x2212;  r  0    )   (   2  v +  v  0      )  +  v
      0       v  (  v +  v  0    )     = 2 a  (  r &#x2212;  r  0    )  +  v  0
      (  v +  v  0    )       v  2   + v  v  0      = 2 a  (  r &#x2212;  r  0
      )  +  v  0   v +  v  0   2        v  2      =  v  0   2   + 2 a  (  r
      &#x2212;  r  0    )   [ 4 ]       {\displaystyle {\begin
      {aligned}v&=a\left(r-r_{0}\right)\left({\frac {2}{v+v_{0}}}\right)+v_
      {0}\\v\left(v+v_{0}\right)&=2a\left(r-r_{0}\right)+v_{0}\left(v+v_
      {0}\right)\\v^{2}+vv_{0}&=2a\left(r-r_{0}\right)+v_{0}v+v_{0}^{2}\\v^
      {2}&=v_{0}^{2}+2a\left(r-r_{0}\right)\quad [4]\\\end{aligned}}}  [{\begin
      {aligned}v&=a\left(r-r_{0}\right)\left({\frac {2}{v+v_{0}}}\right)+v_
      {0}\\v\left(v+v_{0}\right)&=2a\left(r-r_{0}\right)+v_{0}\left(v+v_
      {0}\right)\\v^{2}+vv_{0}&=2a\left(r-r_{0}\right)+v_{0}v+v_{0}^{2}\\v^
      {2}&=v_{0}^{2}+2a\left(r-r_{0}\right)\quad [4]\\\end{aligned}}]
From [3],
         2  (  r &#x2212;  r  0    )  &#x2212; v t =  v  0   t   {\displaystyle
      2\left(r-r_{0}\right)-vt=v_{0}t}  [2\left(r-r_{0}\right)-vt=v_{0}t]
substituting into [2]:
             r    =     a   t  2    2   + 2 r &#x2212; 2  r  0   &#x2212; v t +
      r  0       0    =     a   t  2    2   + r &#x2212;  r  0   &#x2212; v t
      r    =  r  0   + v t &#x2212;     a   t  2    2    [ 5 ]
      {\displaystyle {\begin{aligned}r&={\frac {{a}t^{2}}{2}}+2r-2r_{0}-vt+r_
      {0}\\0&={\frac {{a}t^{2}}{2}}+r-r_{0}-vt\\r&=r_{0}+vt-{\frac {{a}t^{2}}
      {2}}\quad [5]\end{aligned}}}  [{\begin{aligned}r&={\frac {{a}t^{2}}
      {2}}+2r-2r_{0}-vt+r_{0}\\0&={\frac {{a}t^{2}}{2}}+r-r_{0}-vt\\r&=r_
      {0}+vt-{\frac {{a}t^{2}}{2}}\quad [5]\end{aligned}}]
Usually only the first 4 are needed, the fifth is optional.
Here a is constant acceleration, or in the case of bodies moving under the
influence of gravity, the standard_gravity g is used. Note that each of the
equations contains four of the five variables, so in this situation it is
sufficient to know three out of the five variables to calculate the remaining
two.
In elementary physics the same formulae are frequently written in different
notation as:
             v    = u + a t  [ 1 ]     s    = u t +    1 2    a  t  2    [ 2 ]
      s    =    1 2    ( u + v ) t  [ 3 ]      v  2      =  u  2   + 2 a s  [ 4
      ]     s    = v t &#x2212;    1 2    a  t  2    [ 5 ]       {\displaystyle
      {\begin{aligned}v&=u+at\quad [1]\\s&=ut+{\tfrac {1}{2}}at^{2}\quad
      [2]\\s&={\tfrac {1}{2}}(u+v)t\quad [3]\\v^{2}&=u^{2}+2as\quad [4]\\s&=vt-
      {\tfrac {1}{2}}at^{2}\quad [5]\\\end{aligned}}}  [{\displaystyle {\begin
      {aligned}v&=u+at\quad [1]\\s&=ut+{\tfrac {1}{2}}at^{2}\quad [2]\\s&=
      {\tfrac {1}{2}}(u+v)t\quad [3]\\v^{2}&=u^{2}+2as\quad [4]\\s&=vt-{\tfrac
      {1}{2}}at^{2}\quad [5]\\\end{aligned}}}]
where u has replaced v0, s replaces r - r0. They are often referred to as the
SUVAT equations, where "SUVAT" is an acronym from the variables: s =
displacement, u = initial velocity, v = final velocity, a = acceleration, t =
time.[11][12]
*** Constant linear acceleration in any direction[edit] ***
Trajectory of a particle with initial position vector r0 and velocity v0,
subject to constant acceleration a, all three quantities in any direction, and
the position r(t) and velocity v(t) after time t.
The initial position, initial velocity, and acceleration vectors need not be
collinear, and take an almost identical form. The only difference is that the
square magnitudes of the velocities require the dot_product. The derivations
are essentially the same as in the collinear case,
              v     =  a  t +   v   0    [ 1 ]      r     =   r   0   +   v   0
      t +    1 2     a   t  2    [ 2 ]      r     =   r   0   +    1 2
      (   v  +   v   0    )  t  [ 3 ]      v  2      =  v  0   2   + 2  a
      &#x22C5;  (   r  &#x2212;   r   0    )   [ 4 ]      r     =   r   0   +
      v  t &#x2212;    1 2     a   t  2    [ 5 ]       {\displaystyle {\begin
      {aligned}\mathbf {v} &=\mathbf {a} t+\mathbf {v} _{0}\quad [1]\\\mathbf
      {r} &=\mathbf {r} _{0}+\mathbf {v} _{0}t+{\tfrac {1}{2}}\mathbf {a} t^
      {2}\quad [2]\\\mathbf {r} &=\mathbf {r} _{0}+{\tfrac {1}{2}}\left(\mathbf
      {v} +\mathbf {v} _{0}\right)t\quad [3]\\v^{2}&=v_{0}^{2}+2\mathbf {a}
      \cdot \left(\mathbf {r} -\mathbf {r} _{0}\right)\quad [4]\\\mathbf {r}
      &=\mathbf {r} _{0}+\mathbf {v} t-{\tfrac {1}{2}}\mathbf {a} t^{2}\quad
      [5]\\\end{aligned}}}  [{\displaystyle {\begin{aligned}\mathbf {v}
      &=\mathbf {a} t+\mathbf {v} _{0}\quad [1]\\\mathbf {r} &=\mathbf {r} _
      {0}+\mathbf {v} _{0}t+{\tfrac {1}{2}}\mathbf {a} t^{2}\quad [2]\\\mathbf
      {r} &=\mathbf {r} _{0}+{\tfrac {1}{2}}\left(\mathbf {v} +\mathbf {v} _
      {0}\right)t\quad [3]\\v^{2}&=v_{0}^{2}+2\mathbf {a} \cdot \left(\mathbf
      {r} -\mathbf {r} _{0}\right)\quad [4]\\\mathbf {r} &=\mathbf {r} _
      {0}+\mathbf {v} t-{\tfrac {1}{2}}\mathbf {a} t^{2}\quad [5]\\\end
      {aligned}}}]
although the Torricelli_equation [4] can be derived using the distributive
property of the dot product as follows:
          v  2   =  v  &#x22C5;  v  = (   v   0   +  a  t ) &#x22C5; (   v   0
      +  a  t ) =  v  0   2   + 2 t (  a  &#x22C5;   v   0   ) +  a  2    t  2
      {\displaystyle v^{2}=\mathbf {v} \cdot \mathbf {v} =(\mathbf {v} _
      {0}+\mathbf {a} t)\cdot (\mathbf {v} _{0}+\mathbf {a} t)=v_{0}^{2}+2t
      (\mathbf {a} \cdot \mathbf {v} _{0})+a^{2}t^{2}}  [v^{2}=\mathbf {v}
      \cdot \mathbf {v} =(\mathbf {v} _{0}+\mathbf {a} t)\cdot (\mathbf {v} _
      {0}+\mathbf {a} t)=v_{0}^{2}+2t(\mathbf {a} \cdot \mathbf {v} _{0})+a^
      {2}t^{2}]
         ( 2  a  ) &#x22C5; (  r  &#x2212;   r   0   ) = ( 2  a  ) &#x22C5;
      (    v   0   t +    1 2     a   t  2    )  = 2 t (  a  &#x22C5;   v   0
      ) +  a  2    t  2   =  v  2   &#x2212;  v  0   2     {\displaystyle
      (2\mathbf {a} )\cdot (\mathbf {r} -\mathbf {r} _{0})=(2\mathbf {a} )\cdot
      \left(\mathbf {v} _{0}t+{\tfrac {1}{2}}\mathbf {a} t^{2}\right)=2t
      (\mathbf {a} \cdot \mathbf {v} _{0})+a^{2}t^{2}=v^{2}-v_{0}^{2}}  [
      {\displaystyle (2\mathbf {a} )\cdot (\mathbf {r} -\mathbf {r} _{0})=
      (2\mathbf {a} )\cdot \left(\mathbf {v} _{0}t+{\tfrac {1}{2}}\mathbf {a}
      t^{2}\right)=2t(\mathbf {a} \cdot \mathbf {v} _{0})+a^{2}t^{2}=v^{2}-v_
      {0}^{2}}]
         &#x2234;  v  2   =  v  0   2   + 2 (  a  &#x22C5; (  r  &#x2212;   r
      0   ) )   {\displaystyle \therefore v^{2}=v_{0}^{2}+2(\mathbf {a} \cdot
      (\mathbf {r} -\mathbf {r} _{0}))}  [\therefore v^{2}=v_{0}^{2}+2(\mathbf
      {a} \cdot (\mathbf {r} -\mathbf {r} _{0}))]
*** Applications[edit] ***
Elementary and frequent examples in kinematics involve projectiles, for example
a ball thrown upwards into the air. Given initial speed u, one can calculate
how high the ball will travel before it begins to fall. The acceleration is
local acceleration of gravity g. At this point one must remember that while
these quantities appear to be scalars, the direction of displacement, speed and
acceleration is important. They could in fact be considered as unidirectional
vectors. Choosing s to measure up from the ground, the acceleration a must be
in fact âg, since the force of gravity acts downwards and therefore also the
acceleration on the ball due to it.
At the highest point, the ball will be at rest: therefore v = 0. Using equation
[4] in the set above, we have:
         s =     v  2   &#x2212;  u  2     &#x2212; 2 g    .   {\displaystyle
      s={\frac {v^{2}-u^{2}}{-2g}}.}  [s={\frac {v^{2}-u^{2}}{-2g}}.]
Substituting and cancelling minus signs gives:
         s =    u  2    2 g    .   {\displaystyle s={\frac {u^{2}}{2g}}.}  [s=
      {\frac {u^{2}}{2g}}.]
*** Constant circular acceleration[edit] ***
The analogues of the above equations can be written for rotation. Again these
axial vectors must all be parallel to the axis of rotation, so only the
magnitudes of the vectors are necessary,
             &#x03C9;    =  &#x03C9;  0   + &#x03B1; t     &#x03B8;    =
      &#x03B8;  0   +  &#x03C9;  0   t +    1 2    &#x03B1;  t  2
      &#x03B8;    =  &#x03B8;  0   +    1 2    (  &#x03C9;  0   + &#x03C9; ) t
      &#x03C9;  2      =  &#x03C9;  0   2   + 2 &#x03B1; ( &#x03B8; &#x2212;
      &#x03B8;  0   )     &#x03B8;    =  &#x03B8;  0   + &#x03C9; t &#x2212;
      1 2    &#x03B1;  t  2         {\displaystyle {\begin{aligned}\omega
      &=\omega _{0}+\alpha t\\\theta &=\theta _{0}+\omega _{0}t+{\tfrac {1}
      {2}}\alpha t^{2}\\\theta &=\theta _{0}+{\tfrac {1}{2}}(\omega _{0}+\omega
      )t\\\omega ^{2}&=\omega _{0}^{2}+2\alpha (\theta -\theta _{0})\\\theta
      &=\theta _{0}+\omega t-{\tfrac {1}{2}}\alpha t^{2}\\\end{aligned}}}  [
      {\begin{aligned}\omega &=\omega _{0}+\alpha t\\\theta &=\theta _
      {0}+\omega _{0}t+{\tfrac {1}{2}}\alpha t^{2}\\\theta &=\theta _{0}+
      {\tfrac {1}{2}}(\omega _{0}+\omega )t\\\omega ^{2}&=\omega _{0}^
      {2}+2\alpha (\theta -\theta _{0})\\\theta &=\theta _{0}+\omega t-{\tfrac
      {1}{2}}\alpha t^{2}\\\end{aligned}}]
where Î± is the constant angular_acceleration, Ï is the angular_velocity, Ï0
is the initial angular velocity, Î¸ is the angle turned through (angular
displacement), Î¸0 is the initial angle, and t is the time taken to rotate from
the initial state to the final state.
**** General planar motion[edit] ****
Main article: General_planar_motion
Position vector r, always points radially from the origin.
Velocity vector v, always tangent to the path of motion.
Acceleration vector a, not parallel to the radial motion but offset by the
angular and Coriolis accelerations, nor tangent to the path but offset by the
centripetal and radial accelerations.
Kinematic vectors in plane polar coordinates. Notice the setup is not
restricted to 2D space, but a plane in any higher dimension.
These are the kinematic equations for a particle traversing a path in a plane,
described by position r = r(t).[13] They are simply the time derivatives of the
position vector in plane polar_coordinates using the definitions of physical
quantities above for angular velocity Ï and angular acceleration Î±. These are
instantaneous quantities which change with time.
The position of the particle is
          r  =  r   (  r ( t ) , &#x03B8; ( t )  )  = r     e &#x005E;     r
      {\displaystyle \mathbf {r} =\mathbf {r} \left(r(t),\theta
      (t)\right)=r\mathbf {\hat {e}} _{r}}  [{\displaystyle \mathbf {r}
      =\mathbf {r} \left(r(t),\theta (t)\right)=r\mathbf {\hat {e}} _{r}}]
where Ãªr and ÃªÎ¸ are the polar unit vectors. Differentiating with respect to
time gives the velocity
          v  =     e &#x005E;     r      d r   d t    + r &#x03C9;     e
      &#x005E;     &#x03B8;     {\displaystyle \mathbf {v} =\mathbf {\hat {e}}
      _{r}{\frac {dr}{dt}}+r\omega \mathbf {\hat {e}} _{\theta }}  [
      {\displaystyle \mathbf {v} =\mathbf {\hat {e}} _{r}{\frac {dr}
      {dt}}+r\omega \mathbf {\hat {e}} _{\theta }}]
with radial component dr/dt and an additional component rÏ due to the
rotation. Differentiating with respect to time again obtains the acceleration
          a  =  (      d  2   r   d  t  2      &#x2212; r  &#x03C9;  2    )
      e &#x005E;     r   +  (  r &#x03B1; + 2 &#x03C9;    d r   d t     )
      e &#x005E;     &#x03B8;     {\displaystyle \mathbf {a} =\left({\frac {d^
      {2}r}{dt^{2}}}-r\omega ^{2}\right)\mathbf {\hat {e}} _{r}+\left(r\alpha
      +2\omega {\frac {dr}{dt}}\right)\mathbf {\hat {e}} _{\theta }}  [
      {\displaystyle \mathbf {a} =\left({\frac {d^{2}r}{dt^{2}}}-r\omega ^
      {2}\right)\mathbf {\hat {e}} _{r}+\left(r\alpha +2\omega {\frac {dr}
      {dt}}\right)\mathbf {\hat {e}} _{\theta }}]
which breaks into the radial acceleration d2r/dt2, centripetal_acceleration
ârÏ2, Coriolis_acceleration 2Ïdr/dt, and angular acceleration rÎ±.
Special cases of motion described be these equations are summarized
qualitatively in the table below. Two have already been discussed above, in the
cases that either the radial components or the angular components are zero, and
the non-zero component of motion describes uniform acceleration.
State of motion    Constant r     r linear in t  r quadratic in r non-linear in
                                                 t              t
                                  Uniform
                                  translation    Uniform        Non-uniform
Constant Î¸      Stationary     (constant      translational  translation
                                  translational  acceleration
                                  velocity)
                   Uniform        Uniform        Angular motion
                   angular motion angular motion in a spiral,   Angular motion
Î¸ linear in t   in a circle    in a spiral,   constant       in a spiral,
                   (constant      constant       radial         varying radial
                   angular        radial         acceleration   acceleration
                   velocity)      velocity
                                  Uniform        Uniform
                   Uniform        angular        angular        Uniform angular
                   angular        acceleration   acceleration   acceleration in
Î¸ quadratic in tacceleration   in a spiral,   in a spiral,   a spiral,
                   in a circle    constant       constant       varying radial
                                  radial         radial         acceleration
                                  velocity       acceleration
                                  Non-uniform    Non-uniform    Non-uniform
                   Non-uniform    angular        angular        angular
                   angular        acceleration   acceleration   acceleration in
Î¸ non-linear in acceleration   in a spiral,   in a spiral,   a spiral,
                   in a circle    constant       constant       varying radial
                                  radial         radial         acceleration
                                  velocity       acceleration
**** General 3D motions[edit] ****
Main article: Spherical_coordinate_system
In 3D space, the equations in spherical coordinates (r, Î¸, Ï) with
corresponding unit vectors Ãªr, ÃªÎ¸ and ÃªÏ, the position, velocity, and
acceleration generalize respectively to
              r     =  r   ( t )  = r     e &#x005E;     r        v     = v
      e &#x005E;     r   + r     d &#x03B8;   d t        e &#x005E;
      &#x03B8;   + r     d &#x03C6;   d t     sin &#x2061; &#x03B8;     e
      &#x005E;     &#x03C6;        a     =  (  a &#x2212; r   (    d &#x03B8;
      d t    )   2   &#x2212; r   (    d &#x03C6;   d t    )   2    sin  2
      &#x2061; &#x03B8;  )      e &#x005E;     r         +  (  r     d  2
      &#x03B8;   d  t  2      + 2 v    d &#x03B8;   d t    &#x2212; r   (    d
      &#x03C6;   d t    )   2   sin &#x2061; &#x03B8; cos &#x2061; &#x03B8;  )
      e &#x005E;     &#x03B8;         +  (  r     d  2   &#x03C6;   d  t  2
      sin &#x2061; &#x03B8; + 2 v     d &#x03C6;   d t     sin &#x2061;
      &#x03B8; + 2 r     d &#x03B8;   d t        d &#x03C6;   d t     cos
      &#x2061; &#x03B8;  )      e &#x005E;     &#x03C6;
      {\displaystyle {\begin{aligned}\mathbf {r} &=\mathbf {r} \left
      (t\right)=r\mathbf {\hat {e}} _{r}\\\mathbf {v} &=v\mathbf {\hat {e}} _
      {r}+r\,{\frac {d\theta }{dt}}\mathbf {\hat {e}} _{\theta }+r\,{\frac
      {d\varphi }{dt}}\,\sin \theta \mathbf {\hat {e}} _{\varphi }\\\mathbf {a}
      &=\left(a-r\left({\frac {d\theta }{dt}}\right)^{2}-r\left({\frac
      {d\varphi }{dt}}\right)^{2}\sin ^{2}\theta \right)\mathbf {\hat {e}} _
      {r}\\&+\left(r{\frac {d^{2}\theta }{dt^{2}}}+2v{\frac {d\theta }{dt}}-
      r\left({\frac {d\varphi }{dt}}\right)^{2}\sin \theta \cos \theta
      \right)\mathbf {\hat {e}} _{\theta }\\&+\left(r{\frac {d^{2}\varphi }{dt^
      {2}}}\,\sin \theta +2v\,{\frac {d\varphi }{dt}}\,\sin \theta +2r\,{\frac
      {d\theta }{dt}}\,{\frac {d\varphi }{dt}}\,\cos \theta \right)\mathbf
      {\hat {e}} _{\varphi }\end{aligned}}\,\!}  [{\displaystyle {\begin
      {aligned}\mathbf {r} &=\mathbf {r} \left(t\right)=r\mathbf {\hat {e}} _
      {r}\\\mathbf {v} &=v\mathbf {\hat {e}} _{r}+r\,{\frac {d\theta }
      {dt}}\mathbf {\hat {e}} _{\theta }+r\,{\frac {d\varphi }{dt}}\,\sin
      \theta \mathbf {\hat {e}} _{\varphi }\\\mathbf {a} &=\left(a-r\left(
      {\frac {d\theta }{dt}}\right)^{2}-r\left({\frac {d\varphi }{dt}}\right)^
      {2}\sin ^{2}\theta \right)\mathbf {\hat {e}} _{r}\\&+\left(r{\frac {d^
      {2}\theta }{dt^{2}}}+2v{\frac {d\theta }{dt}}-r\left({\frac {d\varphi }
      {dt}}\right)^{2}\sin \theta \cos \theta \right)\mathbf {\hat {e}} _
      {\theta }\\&+\left(r{\frac {d^{2}\varphi }{dt^{2}}}\,\sin \theta +2v\,
      {\frac {d\varphi }{dt}}\,\sin \theta +2r\,{\frac {d\theta }{dt}}\,{\frac
      {d\varphi }{dt}}\,\cos \theta \right)\mathbf {\hat {e}} _{\varphi }\end
      {aligned}}\,\!}]
In the case of a constant Ï this reduces to the planar equations above.
***** Dynamic equations of motion[edit] *****
**** Newtonian mechanics[edit] ****
Main article: Newtonian_mechanics
The first general equation of motion developed was Newton's_second_law of
motion, in its most general form states the rate of change of momentum p = p(t)
= mv(t) of an object equals the force F = F(x(t), v(t), t) acting on it,[14]
          F  =    d  p    d t      {\displaystyle \mathbf {F} ={\frac {d\mathbf
      {p} }{dt}}}  [\mathbf {F} ={\frac {d\mathbf {p} }{dt}}]
The force in the equation is not the force the object exerts. Replacing
momentum by mass times velocity, the law is also written more famously as
          F  = m  a    {\displaystyle \mathbf {F} =m\mathbf {a} }  [\mathbf {F}
      =m\mathbf {a} ]
since m is a constant in Newtonian_mechanics.
Newton's second law applies to point-like particles, and to all points in a
rigid_body. They also apply to each point in a mass continua, like deformable
solids or fluids, but the motion of the system must be accounted for, see
material_derivative. In the case the mass is not constant, it is not sufficient
to use the product_rule for the time derivative on the mass and velocity, and
Newton's second law requires some modification consistent with conservation_of
momentum, see variable-mass_system.
It may be simple to write down the equations of motion in vector form using
Newton's laws of motion, but the components may vary in complicated ways with
spatial coordinates and time, and solving them is not easy. Often there is an
excess of variables to solve for the problem completely, so Newton's laws are
not always the most efficient way to determine the motion of a system. In
simple cases of rectangular geometry, Newton's laws work fine in Cartesian
coordinates, but in other coordinate systems can become dramatically complex.
The momentum form is preferable since this is readily generalized to more
complex systems, generalizes to special and general_relativity (see four-
momentum).[14] It can also be used with the momentum conservation. However,
Newton's laws are not more fundamental than momentum conservation, because
Newton's laws are merely consistent with the fact that zero resultant force
acting on an object implies constant momentum, while a resultant force implies
the momentum is not constant. Momentum conservation is always true for an
isolated system not subject to resultant forces.
For a number of particles (see many_body_problem), the equation of motion for
one particle i influenced by other particles is[8][15]
            d   p   i     d t    =   F   E   +  &#x2211;  i &#x2260; j     F
      i j       {\displaystyle {\frac {d\mathbf {p} _{i}}{dt}}=\mathbf {F} _
      {E}+\sum _{i\neq j}\mathbf {F} _{ij}\,\!}  [{\frac {d\mathbf {p} _{i}}
      {dt}}=\mathbf {F} _{E}+\sum _{i\neq j}\mathbf {F} _{ij}\,\!]
where pi is the momentum of particle i, Fij is the force on particle i by
particle j, and FE is the resultant external force due to any agent not part of
system. Particle i does not exert a force on itself.
Euler's_laws_of_motion are similar to Newton's laws, but they are applied
specifically to the motion of rigid_bodies. The NewtonâEuler_equations
combine the forces and torques acting on a rigid body into a single equation.
Newton's second law for rotation takes a similar form to the translational
case,[16]
          &#x03C4;  =    d  L    d t     ,   {\displaystyle {\boldsymbol {\tau
      }}={\frac {d\mathbf {L} }{dt}}\,,}  [{\boldsymbol {\tau }}={\frac
      {d\mathbf {L} }{dt}}\,,]
by equating the torque acting on the body to the rate of change of its angular
momentum L. Analogous to mass times acceleration, the moment_of_inertia tensor
I depends on the distribution of mass about the axis of rotation, and the
angular acceleration is the rate of change of angular velocity,
          &#x03C4;  =  I  &#x22C5;  &#x03B1;  .   {\displaystyle {\boldsymbol
      {\tau }}=\mathbf {I} \cdot {\boldsymbol {\alpha }}.}  [{\boldsymbol {\tau
      }}=\mathbf {I} \cdot {\boldsymbol {\alpha }}.]
Again, these equations apply to point like particles, or at each point of a
rigid body.
Likewise, for a number of particles, the equation of motion for one particle i
is[17]
            d   L   i     d t    =   &#x03C4;   E   +  &#x2211;  i &#x2260; j
      &#x03C4;   i j    ,   {\displaystyle {\frac {d\mathbf {L} _{i}}{dt}}=
      {\boldsymbol {\tau }}_{E}+\sum _{i\neq j}{\boldsymbol {\tau }}_{ij}\,,}
      [{\frac {d\mathbf {L} _{i}}{dt}}={\boldsymbol {\tau }}_{E}+\sum _{i\neq
      j}{\boldsymbol {\tau }}_{ij}\,,]
where Li is the angular momentum of particle i, Ïij the torque on particle i
by particle j, and ÏE is resultant external torque (due to any agent not part
of system). Particle i does not exert a torque on itself.
**** Applications[edit] ****
Some examples[18] of Newton's law include describing the motion of a simple
pendulum,
         &#x2212; m g sin &#x2061; &#x03B8; = m     d  2   ( l &#x03B8; )   d
      t  2       &#x21D2;      d  2   &#x03B8;   d  t  2      = &#x2212;   g l
      sin &#x2061; &#x03B8;  ,   {\displaystyle -mg\sin \theta =m{\frac {d^{2}
      (l\theta )}{dt^{2}}}\quad \Rightarrow \quad {\frac {d^{2}\theta }{dt^
      {2}}}=-{\frac {g}{l}}\sin \theta \,,}  [{\displaystyle -mg\sin \theta =m
      {\frac {d^{2}(l\theta )}{dt^{2}}}\quad \Rightarrow \quad {\frac {d^
      {2}\theta }{dt^{2}}}=-{\frac {g}{l}}\sin \theta \,,}]
and a damped,_sinusoidally_driven_harmonic_oscillator,
          F  0   sin &#x2061; ( &#x03C9; t ) = m  (      d  2   x   d  t  2
      + 2 &#x03B6;  &#x03C9;  0      d x   d t    +  &#x03C9;  0   2   x  )   .
      {\displaystyle F_{0}\sin(\omega t)=m\left({\frac {d^{2}x}{dt^{2}}}+2\zeta
      \omega _{0}{\frac {dx}{dt}}+\omega _{0}^{2}x\right)\,.}  [F_{0}\sin
      (\omega t)=m\left({\frac {d^{2}x}{dt^{2}}}+2\zeta \omega _{0}{\frac {dx}
      {dt}}+\omega _{0}^{2}x\right)\,.]
For describing the motion of masses due to gravity, Newton's_law_of_gravity can
be combined with Newton's second law. For two examples, a ball of mass m thrown
in the air, in air currents (such as wind) described by a vector field of
resistive forces R = R(r, t),
         &#x2212;    G m M    |   r    |   2          e &#x005E;     r   +  R
      = m     d  2    r    d  t  2      + 0  &#x21D2;      d  2    r    d  t  2
      = &#x2212;    G M    |   r    |   2          e &#x005E;     r   +  A
      {\displaystyle -{\frac {GmM}{|\mathbf {r} |^{2}}}\mathbf {\hat {e}} _
      {r}+\mathbf {R} =m{\frac {d^{2}\mathbf {r} }{dt^{2}}}+0\quad \Rightarrow
      \quad {\frac {d^{2}\mathbf {r} }{dt^{2}}}=-{\frac {GM}{|\mathbf {r} |^
      {2}}}\mathbf {\hat {e}} _{r}+\mathbf {A} \,\!}  [-{\frac {GmM}{|\mathbf
      {r} |^{2}}}\mathbf {\hat {e}} _{r}+\mathbf {R} =m{\frac {d^{2}\mathbf {r}
      }{dt^{2}}}+0\quad \Rightarrow \quad {\frac {d^{2}\mathbf {r} }{dt^{2}}}=-
      {\frac {GM}{|\mathbf {r} |^{2}}}\mathbf {\hat {e}} _{r}+\mathbf {A} \,\!]
where G is the gravitational_constant, M the mass of the Earth, and A = R/m is
the acceleration of the projectile due to the air currents at position r and
time t.
The classical N-body_problem for N particles each interacting with each other
due to gravity is a set of N nonlinear coupled second order ODEs,
             d  2     r   i     d  t  2      = G  &#x2211;  i &#x2260; j
      m  i    m  j      |    r   j   &#x2212;   r   i     |   3      (   r   j
      &#x2212;   r   i   )   {\displaystyle {\frac {d^{2}\mathbf {r} _{i}}{dt^
      {2}}}=G\sum _{i\neq j}{\frac {m_{i}m_{j}}{|\mathbf {r} _{j}-\mathbf {r} _
      {i}|^{3}}}(\mathbf {r} _{j}-\mathbf {r} _{i})}  [{\frac {d^{2}\mathbf {r}
      _{i}}{dt^{2}}}=G\sum _{i\neq j}{\frac {m_{i}m_{j}}{|\mathbf {r} _{j}-
      \mathbf {r} _{i}|^{3}}}(\mathbf {r} _{j}-\mathbf {r} _{i})]
where i = 1, 2, â¦, N labels the quantities (mass, position, etc.) associated
with each particle.
***** Analytical mechanics[edit] *****
Main articles: Analytical_mechanics, Lagrangian_mechanics and Hamiltonian
mechanics
As the system evolves, q traces a path through configuration_space (only some
are shown). The path taken by the system (red) has a stationary action (Î´S =
0) under small changes in the configuration of the system (Î´q).[19]
Using all three coordinates of 3D space is unnecessary if there are constraints
on the system. If the system has N degrees_of_freedom, then one can use a set
of N generalized_coordinates q(t) = [q1(t), q2(t) ... qN(t)], to define the
configuration of the system. They can be in the form of arc_lengths or angles.
They are a considerable simplification to describe motion, since they take
advantage of the intrinsic constraints that limit the system's motion, and the
number of coordinates is reduced to a minimum. The time_derivatives of the
generalized coordinates are the generalized velocities
            q &#x02D9;    =    d  q    d t     .   {\displaystyle \mathbf {\dot
      {q}} ={\frac {d\mathbf {q} }{dt}}\,.}  [{\displaystyle \mathbf {\dot {q}}
      ={\frac {d\mathbf {q} }{dt}}\,.}]
The EulerâLagrange_equations are[2][20]
           d  d t     (    &#x2202; L   &#x2202;    q &#x02D9;       )  =
      &#x2202; L   &#x2202;  q      ,   {\displaystyle {\frac {d}{dt}}\left(
      {\frac {\partial L}{\partial \mathbf {\dot {q}} }}\right)={\frac
      {\partial L}{\partial \mathbf {q} }}\,,}  [{\frac {d}{dt}}\left({\frac
      {\partial L}{\partial \mathbf {\dot {q}} }}\right)={\frac {\partial L}
      {\partial \mathbf {q} }}\,,]
where the Lagrangian is a function of the configuration q and its time rate of
change dq/dt (and possibly time t)
         L = L  [   q  ( t ) ,    q &#x02D9;    ( t ) , t  ]   .
      {\displaystyle L=L\left[\mathbf {q} (t),\mathbf {\dot {q}}
      (t),t\right]\,.}  [L=L\left[\mathbf {q} (t),\mathbf {\dot {q}}
      (t),t\right]\,.]
Setting up the Lagrangian of the system, then substituting into the equations
and evaluating the partial derivatives and simplifying, a set of coupled N
second order ODEs in the coordinates are obtained.
Hamilton's_equations are[2][20]
            p &#x02D9;    = &#x2212;    &#x2202; H   &#x2202;  q      ,     q
      &#x02D9;    = +    &#x2202; H   &#x2202;  p      ,   {\displaystyle
      \mathbf {\dot {p}} =-{\frac {\partial H}{\partial \mathbf {q} }}\,,\quad
      \mathbf {\dot {q}} =+{\frac {\partial H}{\partial \mathbf {p} }}\,,}
      [\mathbf {\dot {p}} =-{\frac {\partial H}{\partial \mathbf {q} }}\,,\quad
      \mathbf {\dot {q}} =+{\frac {\partial H}{\partial \mathbf {p} }}\,,]
where the Hamiltonian
         H = H  [   q  ( t ) ,  p  ( t ) , t  ]   ,   {\displaystyle H=H\left
      [\mathbf {q} (t),\mathbf {p} (t),t\right]\,,}  [H=H\left[\mathbf {q}
      (t),\mathbf {p} (t),t\right]\,,]
is a function of the configuration q and conjugate "generalized"_momenta
          p  =    &#x2202; L   &#x2202;    q &#x02D9;        ,   {\displaystyle
      \mathbf {p} ={\frac {\partial L}{\partial \mathbf {\dot {q}} }}\,,}  [
      {\displaystyle \mathbf {p} ={\frac {\partial L}{\partial \mathbf {\dot
      {q}} }}\,,}]
in which â/âq = (â/âq1, â/âq2, â¦, â/âqN) is a shorthand
notation for a vector of partial_derivatives with respect to the indicated
variables (see for example matrix_calculus for this denominator notation), and
possibly time t,
Setting up the Hamiltonian of the system, then substituting into the equations
and evaluating the partial derivatives and simplifying, a set of coupled 2N
first order ODEs in the coordinates qi and momenta pi are obtained.
The HamiltonâJacobi_equation is[2]
         &#x2212;    &#x2202; S (  q  , t )   &#x2202; t    = H  (   q  ,  p  ,
      t  )   .   {\displaystyle -{\frac {\partial S(\mathbf {q} ,t)}{\partial
      t}}=H\left(\mathbf {q} ,\mathbf {p} ,t\right)\,.}  [-{\frac {\partial S
      (\mathbf {q} ,t)}{\partial t}}=H\left(\mathbf {q} ,\mathbf {p}
      ,t\right)\,.]
where
         S [  q  , t ] =  &#x222B;   t  1      t  2     L (  q  ,    q &#x02D9;
      , t )  d t  ,   {\displaystyle S[\mathbf {q} ,t]=\int _{t_{1}}^{t_{2}}L
      (\mathbf {q} ,\mathbf {\dot {q}} ,t)\,dt\,,}  [S[\mathbf {q} ,t]=\int _
      {t_{1}}^{t_{2}}L(\mathbf {q} ,\mathbf {\dot {q}} ,t)\,dt\,,]
is Hamilton's principal function, also called the classical_action is a
functional of L. In this case, the momenta are given by
          p  =    &#x2202; S   &#x2202;  q      .   {\displaystyle \mathbf {p}
      ={\frac {\partial S}{\partial \mathbf {q} }}\,.}  [{\displaystyle \mathbf
      {p} ={\frac {\partial S}{\partial \mathbf {q} }}\,.}]
Although the equation has a simple general form, for a given Hamiltonian it is
actually a single first order non-linear PDE, in N + 1 variables. The action S
allows identification of conserved quantities for mechanical systems, even when
the mechanical problem itself cannot be solved fully, because any
differentiable symmetry of the action of a physical system has a corresponding
conservation_law, a theorem due to Emmy_Noether.
All classical equations of motion can be derived from the variational_principle
known as Hamilton's_principle_of_least_action
         &#x03B4; S = 0  ,   {\displaystyle \delta S=0\,,}  [\delta S=0\,,]
stating the path the system takes through the configuration_space is the one
with the least action S.
***** Electrodynamics[edit] *****
Lorentz_force f on a charged_particle (of charge q) in motion (instantaneous
velocity v). The E_field and B_field vary in space and time.
In electrodynamics, the force on a charged particle of charge q is the Lorentz
force:[21]
          F  = q  (   E  +  v  &#x00D7;  B   )      {\displaystyle \mathbf {F}
      =q\left(\mathbf {E} +\mathbf {v} \times \mathbf {B} \right)\,\!}
      [\mathbf {F} =q\left(\mathbf {E} +\mathbf {v} \times \mathbf {B}
      \right)\,\!]
Combining with Newton's second law gives a first order differential equation of
motion, in terms of position of the particle:
         m     d  2    r    d  t  2      = q  (   E  +    d  r    d t
      &#x00D7;  B   )      {\displaystyle m{\frac {d^{2}\mathbf {r} }{dt^
      {2}}}=q\left(\mathbf {E} +{\frac {d\mathbf {r} }{dt}}\times \mathbf {B}
      \right)\,\!}  [m{\frac {d^{2}\mathbf {r} }{dt^{2}}}=q\left(\mathbf {E} +
      {\frac {d\mathbf {r} }{dt}}\times \mathbf {B} \right)\,\!]
or its momentum:
            d  p    d t    = q  (   E  +     p  &#x00D7;  B   m    )
      {\displaystyle {\frac {d\mathbf {p} }{dt}}=q\left(\mathbf {E} +{\frac
      {\mathbf {p} \times \mathbf {B} }{m}}\right)\,\!}  [{\frac {d\mathbf {p}
      }{dt}}=q\left(\mathbf {E} +{\frac {\mathbf {p} \times \mathbf {B} }
      {m}}\right)\,\!]
The same equation can be obtained using the Lagrangian (and applying Lagrange's
equations above) for a charged particle of mass m and charge q:[22]
         L =    1 2    m    r &#x02D9;    &#x22C5;    r &#x02D9;    + q  A
      &#x22C5;     r  &#x02D9;    &#x2212; q &#x03D5;   {\displaystyle L=
      {\tfrac {1}{2}}m\mathbf {\dot {r}} \cdot \mathbf {\dot {r}} +q\mathbf {A}
      \cdot {\dot {\mathbf {r} }}-q\phi }  [{\displaystyle L={\tfrac {1}
      {2}}m\mathbf {\dot {r}} \cdot \mathbf {\dot {r}} +q\mathbf {A} \cdot
      {\dot {\mathbf {r} }}-q\phi }]
where A and Ï are the electromagnetic scalar and vector potential fields. The
Lagrangian indicates an additional detail: the canonical_momentum in Lagrangian
mechanics is given by:
          P  =    &#x2202; L   &#x2202;     r  &#x02D9;       = m     r
      &#x02D9;    + q  A    {\displaystyle \mathbf {P} ={\frac {\partial L}
      {\partial {\dot {\mathbf {r} }}}}=m{\dot {\mathbf {r} }}+q\mathbf {A} }
      [\mathbf {P} ={\frac {\partial L}{\partial {\dot {\mathbf {r} }}}}=m{\dot
      {\mathbf {r} }}+q\mathbf {A} ]
instead of just mv, implying the motion of a charged particle is fundamentally
determined by the mass and charge of the particle. The Lagrangian expression
was first used to derive the force equation.
Alternatively the Hamiltonian (and substituting into the equations):[20]
         H =     (   P  &#x2212; q  A   )   2    2 m    + q &#x03D5;
      {\displaystyle H={\frac {\left(\mathbf {P} -q\mathbf {A} \right)^{2}}
      {2m}}+q\phi \,\!}  [H={\frac {\left(\mathbf {P} -q\mathbf {A} \right)^
      {2}}{2m}}+q\phi \,\!]
can derive the Lorentz force equation.
***** General relativity[edit] *****
**** Geodesic equation of motion[edit] ****
Geodesics on a sphere are arcs of great_circles (yellow curve). On a
2D–manifold (such as the sphere shown), the direction of the accelerating
geodesic is uniquely fixed if the separation vector Î¾ is orthogonal to the
"fiducial geodesic" (green curve). As the separation vector Î¾0 changes to Î¾
after a distance s, the geodesics are not parallel (geodesic deviation).[23]
Main articles: Geodesics_in_general_relativity and Geodesic_equation
The above equations are valid in flat spacetime. In curved_space spacetime,
things become mathematically more complicated since there is no straight line;
this is generalized and replaced by a geodesic of the curved spacetime (the
shortest length of curve between two points). For curved manifolds with a
metric_tensor g, the metric provides the notion of arc length (see line_element
for details), the differential arc length is given by:[24]
         d s =    g  &#x03B1; &#x03B2;   d  x  &#x03B1;   d  x  &#x03B2;
      {\displaystyle ds={\sqrt {g_{\alpha \beta }dx^{\alpha }dx^{\beta }}}}
      [ds={\sqrt {g_{\alpha \beta }dx^{\alpha }dx^{\beta }}}]
and the geodesic equation is a second-order differential equation in the
coordinates, the general solution is a family of geodesics:[25]
             d  2    x  &#x03BC;     d  s  2      = &#x2212;  &#x0393;
      &#x03BC;       &#x03B1; &#x03B2;      d  x  &#x03B1;     d s       d  x
      &#x03B2;     d s      {\displaystyle {\frac {d^{2}x^{\mu }}{ds^{2}}}=-
      \Gamma ^{\mu }{}_{\alpha \beta }{\frac {dx^{\alpha }}{ds}}{\frac {dx^
      {\beta }}{ds}}}  [{\frac {d^{2}x^{\mu }}{ds^{2}}}=-\Gamma ^{\mu }{}_
      {\alpha \beta }{\frac {dx^{\alpha }}{ds}}{\frac {dx^{\beta }}{ds}}]
where Î Î¼Î±Î² is a Christoffel_symbol_of_the_second_kind, which contains the
metric (with respect to the coordinate system).
Given the mass-energy distribution provided by the stressâenergy_tensor
T Î±Î², the Einstein_field_equations are a set of non-linear second-order
partial differential equations in the metric, and imply the curvature of space
time is equivalent to a gravitational field (see equivalence_principle). Mass
falling in curved spacetime is equivalent to a mass falling in a gravitational
field - because gravity_is_a_fictitious_force. The relative acceleration of one
geodesic to another in curved spacetime is given by the geodesic_deviation
equation:
             D  2    &#x03BE;  &#x03B1;     d  s  2      = &#x2212;  R
      &#x03B1;       &#x03B2; &#x03B3; &#x03B4;      d  x  &#x03B1;     d s
      &#x03BE;  &#x03B3;      d  x  &#x03B4;     d s      {\displaystyle {\frac
      {D^{2}\xi ^{\alpha }}{ds^{2}}}=-R^{\alpha }{}_{\beta \gamma \delta }
      {\frac {dx^{\alpha }}{ds}}\xi ^{\gamma }{\frac {dx^{\delta }}{ds}}}  [
      {\frac {D^{2}\xi ^{\alpha }}{ds^{2}}}=-R^{\alpha }{}_{\beta \gamma \delta
      }{\frac {dx^{\alpha }}{ds}}\xi ^{\gamma }{\frac {dx^{\delta }}{ds}}]
where Î¾Î± = x2Î± â x1Î± is the separation vector between two geodesics, D/ds
(not just d/ds) is the covariant_derivative, and RÎ±Î²Î³Î´ is the Riemann
curvature_tensor, containing the Christoffel symbols. In other words, the
geodesic deviation equation is the equation of motion for masses in curved
spacetime, analogous to the Lorentz force equation for charges in an
electromagnetic field.[26]
For flat spacetime, the metric is a constant tensor so the Christoffel symbols
vanish, and the geodesic equation has the solutions of straight lines. This is
also the limiting case when masses move according to Newton's_law_of_gravity.
**** Spinning objects[edit] ****
In general relativity, rotational motion is described by the relativistic
angular_momentum tensor, including the spin_tensor, which enter the equations
of motion under covariant_derivatives with respect to proper_time. The
MathissonâPapapetrouâDixon_equations describe the motion of spinning
objects moving in a gravitational_field.
***** Analogues for waves and fields[edit] *****
Unlike the equations of motion for describing particle mechanics, which are
systems of coupled ordinary differential equations, the analogous equations
governing the dynamics of waves and fields are always partial_differential
equations, since the waves or fields are functions of space and time. For a
particular solution, boundary_conditions along with initial conditions need to
be specified.
Sometimes in the following contexts, the wave or field equations are also
called "equations of motion".
**** Field equations[edit] ****
Equations that describe the spatial dependence and time_evolution of fields are
called field_equations. These include
    * Maxwell's_equations for the electromagnetic_field,
    * Poisson's_equation for Newtonian_gravitational or electrostatic field
      potentials,
    * the Einstein_field_equation for gravitation (Newton's_law_of_gravity is a
      special case for weak gravitational fields and low velocities of
      particles).
This terminology is not universal: for example although the NavierâStokes
equations govern the velocity_field of a fluid, they are not usually called
"field equations", since in this context they represent the momentum of the
fluid and are called the "momentum equations" instead.
**** Wave equations[edit] ****
Equations of wave motion are called wave_equations. The solutions to a wave
equation give the time-evolution and spatial dependence of the amplitude.
Boundary conditions determine if the solutions describe traveling_waves or
standing_waves.
From classical equations of motion and field equations; mechanical,
gravitational_wave, and electromagnetic_wave equations can be derived. The
general linear wave equation in 3D is:
           1  v  2         &#x2202;  2   X   &#x2202;  t  2      =  &#x2207;  2
      X   {\displaystyle {\frac {1}{v^{2}}}{\frac {\partial ^{2}X}{\partial t^
      {2}}}=\nabla ^{2}X}  [{\frac {1}{v^{2}}}{\frac {\partial ^{2}X}{\partial
      t^{2}}}=\nabla ^{2}X]
where X = X(r, t) is any mechanical or electromagnetic field amplitude, say:
[27]
    * the transverse or longitudinal displacement of a vibrating rod, wire,
      cable, membrane etc.,
    * the fluctuating pressure of a medium, sound_pressure,
    * the electric_fields E or D, or the magnetic_fields B or H,
    * the voltage V or current I in an alternating_current circuit,
and v is the phase_velocity. Nonlinear equations model the dependence of phase
velocity on amplitude, replacing v by v(X). There are other linear and
nonlinear wave equations for very specific applications, see for example the
Kortewegâde_Vries_equation.
**** Quantum theory[edit] ****
In quantum theory, the wave and field concepts both appear.
In quantum_mechanics, in which particles also have wave-like properties
according to waveâparticle_duality, the analogue of the classical equations
of motion (Newton's law, EulerâLagrange equation, HamiltonâJacobi equation,
etc.) is the SchrÃ¶dinger_equation in its most general form:
         i &#x210F;    &#x2202; &#x03A8;   &#x2202; t    =    H &#x005E;
      &#x03A8;  ,   {\displaystyle i\hbar {\frac {\partial \Psi }{\partial t}}=
      {\hat {H}}\Psi \,,}  [i\hbar {\frac {\partial \Psi }{\partial t}}={\hat
      {H}}\Psi \,,]
where Î¨ is the wavefunction of the system, Ä¤ is the quantum Hamiltonian
operator, rather than a function as in classical mechanics, and Ä§ is the
Planck_constant divided by 2Ï. Setting up the Hamiltonian and inserting it
into the equation results in a wave equation, the solution is the wavefunction
as a function of space and time. The SchrÃ¶dinger equation itself reduces to
the HamiltonâJacobi equation when one considers the correspondence_principle,
in the limit that Ä§ becomes zero.
Throughout all aspects of quantum theory, relativistic or non-relativistic,
there are various_formulations alternative to the SchrÃ¶dinger equation that
govern the time evolution and behavior of a quantum system, for instance:
    * the Heisenberg_equation_of_motion resembles the time evolution of
      classical observables as functions of position, momentum, and time, if
      one replaces dynamical observables by their quantum_operators and the
      classical Poisson_bracket by the commutator,
    * the phase_space_formulation closely follows classical Hamiltonian
      mechanics, placing position and momentum on equal footing,
    * the Feynman path_integral_formulation extends the principle_of_least
      action to quantum mechanics and field theory, placing emphasis on the use
      of a Lagrangians rather than Hamiltonians.
***** See also[edit] *****
    * Scalar_(physics)
    * Vector
    * Distance
    * Displacement
    * Speed
    * Velocity
    * Acceleration
    * Angular_displacement
    * Angular_speed
    * Angular_velocity
    * Angular_acceleration
    * Equations_for_a_falling_body
    * Parabolic_trajectory
    * Curvilinear_coordinates
    * Orthogonal_coordinates
    * Newton's_laws_of_motion
    * Torricelli's_equation
    * EulerâLagrange_equation
    * Generalized_forces
    * Defining_equation_(physics)
    * NewtonâEuler_laws_of_motion_for_a_rigid_body
***** References[edit] *****
   1. ^ Encyclopaedia of Physics (second Edition), R.G. Lerner, G.L. Trigg, VHC
      Publishers, 1991, ISBN (Verlagsgesellschaft) 3-527-26954-1 (VHC Inc.) 0-
      89573-752-3
   2. ^ a b c d Analytical Mechanics, L.N. Hand, J.D. Finch, Cambridge
      University Press, 2008,
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
   4. ISBN 978-0-521-57572-0
   5. ^ See History_of_Mathematics
   6. ^ The Britannica Guide to History of Mathematics, ed. Erik Gregersen
   7. ^ Discourses, Galileo
   8. ^ Dialogues Concerning Two New Sciences, by Galileo Galilei; translated
      by Henry Crew, Alfonso De Salvio
   9. ^Halliday, David; Resnick, Robert; Walker, Jearl (2004-06-16).
      Fundamentals of Physics (7 Sub ed.). Wiley. ISBN 0-471-23231-9.
  10. ^ a b Dynamics and Relativity, J.R. Forshaw, A.G. Smith, Wiley, 2009,
  11. ISBN 978-0-470-01460-8
  12. ^M.R. Spiegel; S. Lipschutz; D. Spellman (2009). Vector Analysis.
      Schaum's Outlines (2nd ed.). McGraw Hill. p. 33. ISBN 978-0-07-161545-7.
  13. ^ a b Essential Principles of Physics, P.M. Whelan, M.J. Hodgeson, second
      Edition, 1978, John Murray,
  14. ISBN 0-7195-3382-1
  15. ^Hanrahan, Val; Porkess, R (2003). Additional Mathematics for OCR.
      London: Hodder & Stoughton. p. 219. ISBN 0-340-86960-7.
  16. ^Keith Johnson (2001). Physics_for_you:_revised_national_curriculum
      edition_for_GCSE (4th ed.). Nelson Thornes. p. 135. ISBN 978-0-7487-6236-
      1. The 5 symbols are remembered by "suvat". Given any three, the other
      two can be found.
  17. ^ 3000 Solved Problems in Physics, Schaum Series, A. Halpern, Mc Graw
      Hill, 1988,
  18. ISBN 978-0-07-025734-4
  19. ^ a b An Introduction to Mechanics, D. Kleppner, R.J. Kolenkow, Cambridge
      University Press, 2010, p. 112,
  20. ISBN 978-0-521-19821-9
  21. ^ Encyclopaedia of Physics (second Edition), R.G. Lerner, G.L. Trigg, VHC
      publishers, 1991, ISBN (VHC Inc.) 0-89573-752-3
  22. ^ "Mechanics, D. Kleppner 2010"
  23. ^ "Relativity, J.R. Forshaw 2009"
  24. ^ The Physics of Vibrations and Waves (3rd edition), H.J. Pain, John
      Wiley & Sons, 1983,
  25. ISBN 0-471-90182-2
  26. ^R. Penrose (2007). The_Road_to_Reality. Vintage books. p. 474. ISBN 0-
      679-77631-1.
  27. ^ a b c Classical Mechanics (second edition), T.W.B. Kibble, European
      Physics Series, 1973,
  28. ISBN 0-07-084018-0
  29. ^ Electromagnetism (second edition), I.S. Grant, W.R. Phillips,
      Manchester Physics Series, 2008
  30. ISBN 0-471-92712-0
  31. ^ Classical Mechanics (second Edition), T.W.B. Kibble, European Physics
      Series, Mc Graw Hill (UK), 1973,
  32. ISBN 0-07-084018-0.
  33. ^ Misner, Thorne, Wheeler, Gravitation
  34. ^C.B. Parker (1994). McGraw Hill Encyclopaedia of Physics (second ed.).
      p. 1199. ISBN 0-07-051400-3.
  35. ^C.B. Parker (1994). McGraw Hill Encyclopaedia of Physics (second ed.).
      p. 1200. ISBN 0-07-051400-3.
  36. ^J.A. Wheeler; C. Misner; K.S. Thorne (1973). Gravitation. W.H. Freeman &
      Co. pp. 34â35. ISBN 0-7167-0344-0.
  37. ^H.D. Young; R.A. Freedman (2008). University Physics (12th ed.).
      Addison-Wesley (Pearson International). ISBN 0-321-50130-6.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Equations_of_motion&oldid=909346323"
Categories:
    * Classical_mechanics
    * Equations_of_physics
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
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * à¦¬à¦¾à¦à¦²à¦¾
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Latina
    * LÃ«tzebuergesch
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 4 August 2019, at 20:42 (UTC).
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
