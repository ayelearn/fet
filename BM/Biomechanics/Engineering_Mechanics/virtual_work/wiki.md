The following text has been accessed from https://en.wikipedia.org/wiki/Virtual_work at Fri Aug 9 02:48:41 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Virtual work ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
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
    * Virtual work
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
Virtual work arises in the application of the principle_of_least_action to the
study of forces and movement of a mechanical_system. The work of a force acting
on a particle as it moves along a displacement is different for different
displacements. Among all the possible displacements that a particle may follow,
called virtual_displacements, one will minimize the action. This displacement
is therefore the displacement followed by the particle according to the
principle of least action. The work of a force on a particle along a virtual
displacement is known as the virtual work.
Historically, virtual work and the associated calculus_of_variations were
formulated to analyze systems of rigid bodies,[1] but they have also been
developed for the study of the mechanics of deformable bodies.[2]
⁰
***** Contents *****
    * 1_History
    * 2_Overview
    * 3_Introduction
    * 4_Static_equilibrium
          o 4.1_Constraint_forces
    * 5_Law_of_the_lever
    * 6_Gear_train
    * 7_Dynamic_equilibrium_for_rigid_bodies
          o 7.1_Generalized_inertia_forces
          o 7.2_D'Alembert's_form_of_the_principle_of_virtual_work
    * 8_Virtual_work_principle_for_a_deformable_body
          o 8.1_Proof_of_equivalence_between_the_principle_of_virtual_work_and
            the_equilibrium_equation
          o 8.2_Principle_of_virtual_displacements
          o 8.3_Principle_of_virtual_forces
    * 9_Alternative_forms
    * 10_See_also
    * 11_External_links
    * 12_References
    * 13_Bibliography
***** History[edit] *****
The principle of virtual work had always been used in some form since antiquity
in the study of statics. It was used by the Greeks, medieval Arabs and Latins,
and Renaissance Italians as "the law of lever".[3] The idea of virtual work was
invoked by many notable physicists of the 17th century, such as Galileo,
Descartes, Torricelli, Wallis, and Huygens, in varying degrees of generality,
when solving problems in statics.[3] Working with Leibnizian concepts, Johann
Bernoulli systematized the virtual work principle and made explicit the concept
of infinitesimal displacement. He was able to solve problems for both rigid
bodies as well as fluids. Bernoulli's version of virtual work law appeared in
his letter to Pierre_Varignon in 1715, which was later published in Varignon's
second volume of Nouvelle mÃ©canique ou Statique in 1725. This formulation of
the principle is today known as the principle of virtual velocities and is
commonly considered as the prototype of the contemporary virtual work
principles.[3] In 1743 D'Alembert published his TraitÃ© de Dynamique where he
applied the principle of virtual work, based on Bernoulli's work, to solve
various problems in dynamics. His idea was to convert a dynamical problem into
static problem by introducing inertial force.[4] In 1768, Lagrange presented
the virtual work principle in a more efficient form by introducing generalized
coordinates and presented it as an alternative principle of mechanics by which
all problems of equilibrium could be solved. A systematic exposition of
Lagrange's program of applying this approach to all of mechanics, both static
and dynamic, essentially D'Alembert's_principle, was given in his MÃ©canique
Analytique of 1788.[3] Although Lagrange had presented his version of least
action_principle prior to this work, he recognized the virtual work principle
to be more fundamental mainly because it could be assumed alone as the
foundation for all mechanics, unlike the modern understanding that least action
does not account for non-conservative forces.[3]
***** Overview[edit] *****
If a force acts on a particle as it moves from point A to point B, then, for
each possible trajectory that the particle may take, it is possible to compute
the total work done by the force along the path. The principle of virtual work,
which is the form of the principle of least action applied to these systems,
states that the path actually followed by the particle is the one for which the
difference between the work along this path and other nearby paths is zero (to
first order). The formal procedure for computing the difference of functions
evaluated on nearby paths is a generalization of the derivative known from
differential calculus, and is termed the calculus of variations.
Consider a point particle that moves along a path which is described by a
function r(t) from point A, where r(t = t0), to point B, where r(t = t1). It is
possible that the particle moves from A to B along a nearby path described by r
(t) + Î´r(t), where Î´r(t) is called the variation of r(t). The variation Î´r
(t) satisfies the requirement Î´r(t0) = Î´r(t1) = 0. The components of the
variation, Î´r1(t), Î´r2(t) and Î´r3(t), are called virtual displacements. This
can be generalized to an arbitrary mechanical system defined by the generalized
coordinates qi, i = 1, ..., n. In which case, the variation of the trajectory
qi(t) is defined by the virtual displacements Î´qi, i = 1, ..., n.
Virtual work is the total work done by the applied forces and the inertial
forces of a mechanical system as it moves through a set of virtual
displacements. When considering forces applied to a body in static equilibrium,
the principle of least action requires the virtual work of these forces to be
zero.

***** Introduction[edit] *****
Consider a particle P that moves from a point A to a point B along a trajectory
r(t), while a force F(r(t)) is applied to it. The work done by the force F is
given by the integral
         W =  &#x222B;   r  (  t  0   ) = A    r  (  t  1   ) = B    F
      &#x22C5; d  r  =  &#x222B;   t  0      t  1      F  &#x22C5;    d  r    d
      t    &#xA0; d t =  &#x222B;   t  0      t  1      F  &#x22C5;  v  &#xA0;
      d t ,   {\displaystyle W=\int _{\mathbf {r} (t_{0})=A}^{\mathbf {r} (t_
      {1})=B}\mathbf {F} \cdot d\mathbf {r} =\int _{t_{0}}^{t_{1}}\mathbf {F}
      \cdot {\frac {d\mathbf {r} }{dt}}~dt=\int _{t_{0}}^{t_{1}}\mathbf {F}
      \cdot \mathbf {v} ~dt,}  [W=\int _{\mathbf {r} (t_{0})=A}^{\mathbf {r}
      (t_{1})=B}\mathbf {F} \cdot d\mathbf {r} =\int _{t_{0}}^{t_{1}}\mathbf
      {F} \cdot {\frac {d\mathbf {r} }{dt}}~dt=\int _{t_{0}}^{t_{1}}\mathbf {F}
      \cdot \mathbf {v} ~dt,]
where dr is the differential element along the curve that is the trajectory of
P, and v is its velocity. It is important to notice that the value of the work
W depends on the trajectory r(t).
Now consider particle P that moves from point A to point B again, but this time
it moves along the nearby trajectory that differs from r(t) by the variation
Î´r(t)=Îµh(t), where Îµ is a scaling constant that can be made as small as
desired and h(t) is an arbitrary function that satisfies h(t0) = h(t1) = 0.
Suppose the force F(r(t)+Îµh(t)) is the same as F(r(t)). The work done by the
force is given by the integral
            W &#x00AF;    =  &#x222B;   r  (  t  0   ) = A    r  (  t  1   ) =
      B    F  &#x22C5; d (  r  + &#x03F5;  h  ) =  &#x222B;   t  0      t  1
      F  &#x22C5;    d (  r  ( t ) + &#x03F5;  h  ( t ) )   d t    &#xA0; d t =
      &#x222B;   t  0      t  1      F  &#x22C5; (  v  + &#x03F5;     h
      &#x02D9;    ) &#xA0; d t .   {\displaystyle {\bar {W}}=\int _{\mathbf {r}
      (t_{0})=A}^{\mathbf {r} (t_{1})=B}\mathbf {F} \cdot d(\mathbf {r}
      +\epsilon \mathbf {h} )=\int _{t_{0}}^{t_{1}}\mathbf {F} \cdot {\frac {d
      (\mathbf {r} (t)+\epsilon \mathbf {h} (t))}{dt}}~dt=\int _{t_{0}}^{t_
      {1}}\mathbf {F} \cdot (\mathbf {v} +\epsilon {\dot {\mathbf {h} }})~dt.}
      [{\bar {W}}=\int _{\mathbf {r} (t_{0})=A}^{\mathbf {r} (t_{1})=B}\mathbf
      {F} \cdot d(\mathbf {r} +\epsilon \mathbf {h} )=\int _{t_{0}}^{t_
      {1}}\mathbf {F} \cdot {\frac {d(\mathbf {r} (t)+\epsilon \mathbf {h}
      (t))}{dt}}~dt=\int _{t_{0}}^{t_{1}}\mathbf {F} \cdot (\mathbf {v}
      +\epsilon {\dot {\mathbf {h} }})~dt.]
The variation of the work Î´W associated with this nearby path, known as the
virtual work, can be computed to be
         &#x03B4; W =    W &#x00AF;    &#x2212; W =  &#x222B;   t  0      t  1
      (  F  &#x22C5; &#x03F5;     h  &#x02D9;    ) &#xA0; d t .
      {\displaystyle \delta W={\bar {W}}-W=\int _{t_{0}}^{t_{1}}(\mathbf {F}
      \cdot \epsilon {\dot {\mathbf {h} }})~dt.}  [\delta W={\bar {W}}-W=\int _
      {t_{0}}^{t_{1}}(\mathbf {F} \cdot \epsilon {\dot {\mathbf {h} }})~dt.]
If there are no constraints on the motion of P, then 6 parameters are needed to
completely describe P's position at any time t. If there are k (k â¤ 6)
constraint forces, then n = (6 - k) parameters are needed. Hence, we can define
n generalized coordinates qi (t) (i = 1, 2, ..., n), and express r(t) and
Î´r=Îµh(t) in terms of the generalized coordinates. That is,
          r  ( t ) =  r  (  q  1   ,  q  2   , . . . ,  q  n   ; t )
      {\displaystyle \mathbf {r} (t)=\mathbf {r} (q_{1},q_{2},...,q_{n};t)}
      [\mathbf {r} (t)=\mathbf {r} (q_{1},q_{2},...,q_{n};t)],
          h  ( t ) =  h  (  q  1   ,  q  2   , . . . ,  q  n   ; t )
      {\displaystyle \mathbf {h} (t)=\mathbf {h} (q_{1},q_{2},...,q_{n};t)}
      [\mathbf {h} (t)=\mathbf {h} (q_{1},q_{2},...,q_{n};t)].
Then, the derivative of the variation Î´r=Îµh(t) is given by
           d  d t    &#x03B4;  r  =   d  d t    &#x03F5;  h  =  &#x2211;  i = 1
      n      &#x2202;  h    &#x2202;  q  i      &#x03F5;     q &#x02D9;     i
      ,   {\displaystyle {\frac {d}{dt}}\delta \mathbf {r} ={\frac {d}
      {dt}}\epsilon \mathbf {h} =\sum _{i=1}^{n}{\frac {\partial \mathbf {h} }
      {\partial q_{i}}}\epsilon {\dot {q}}_{i},}  [{\frac {d}{dt}}\delta
      \mathbf {r} ={\frac {d}{dt}}\epsilon \mathbf {h} =\sum _{i=1}^{n}{\frac
      {\partial \mathbf {h} }{\partial q_{i}}}\epsilon {\dot {q}}_{i},]
then we have
         &#x03B4; W =  &#x222B;   t  0      t  1      (   &#x2211;  i = 1   n
      F  &#x22C5;    &#x2202;  h    &#x2202;  q  i      &#x03F5;     q &#x02D9;
      i    )  d t =  &#x2211;  i = 1   n    (   &#x222B;   t  0      t  1
      F  &#x22C5;    &#x2202;  h    &#x2202;  q  i      &#x03F5;     q &#x02D9;
      i   &#xA0; d t  )  .   {\displaystyle \delta W=\int _{t_{0}}^{t_{1}}\left
      (\sum _{i=1}^{n}\mathbf {F} \cdot {\frac {\partial \mathbf {h} }{\partial
      q_{i}}}\epsilon {\dot {q}}_{i}\right)dt=\sum _{i=1}^{n}\left(\int _{t_
      {0}}^{t_{1}}\mathbf {F} \cdot {\frac {\partial \mathbf {h} }{\partial q_
      {i}}}\epsilon {\dot {q}}_{i}~dt\right).}  [\delta W=\int _{t_{0}}^{t_
      {1}}\left(\sum _{i=1}^{n}\mathbf {F} \cdot {\frac {\partial \mathbf {h} }
      {\partial q_{i}}}\epsilon {\dot {q}}_{i}\right)dt=\sum _{i=1}^{n}\left
      (\int _{t_{0}}^{t_{1}}\mathbf {F} \cdot {\frac {\partial \mathbf {h} }
      {\partial q_{i}}}\epsilon {\dot {q}}_{i}~dt\right).]
The requirement that the virtual work be zero for an arbitrary variation Î´r
(t)=Îµh(t) is equivalent to the set of requirements
          Q  i   =  F  &#x22C5;    &#x2202;  h    &#x2202;  q  i      = 0 ,  i
      = 1 , &#x2026; , n .   {\displaystyle Q_{i}=\mathbf {F} \cdot {\frac
      {\partial \mathbf {h} }{\partial q_{i}}}=0,\quad i=1,\ldots ,n.}  [Q_
      {i}=\mathbf {F} \cdot {\frac {\partial \mathbf {h} }{\partial q_
      {i}}}=0,\quad i=1,\ldots ,n.]
The terms Qi are called the generalized forces associated with the virtual
displacement Î´r.
***** Static equilibrium[edit] *****
Static_equilibrium is a state in which the net force and net torque acted upon
the system is zero. In other words, both linear_momentum and angular_momentum
of the system are conserved. The principle of virtual work states that the
virtual work of the applied forces is zero for all virtual_movements of the
system from static_equilibrium. This principle can be generalized such that
three dimensional rotations are included: the virtual work of the applied
forces and applied moments is zero for all virtual_movements of the system from
static equilibrium. That is
         &#x03B4; W =  &#x2211;  i = 1   m     F   i   &#x22C5; &#x03B4;   r
      i   +  &#x2211;  j = 1   n     M   j   &#x22C5; &#x03B4;   &#x03D5;   j
      = 0 ,   {\displaystyle \delta W=\sum _{i=1}^{m}\mathbf {F} _{i}\cdot
      \delta \mathbf {r} _{i}+\sum _{j=1}^{n}\mathbf {M} _{j}\cdot \delta
      \mathbf {\phi } _{j}=0,}  [\delta W=\sum _{i=1}^{m}\mathbf {F} _{i}\cdot
      \delta \mathbf {r} _{i}+\sum _{j=1}^{n}\mathbf {M} _{j}\cdot \delta
      \mathbf {\phi } _{j}=0,]
where Fi , i = 1, 2, ..., m and Mj , j = 1, 2, ..., n are the applied forces
and applied moments, respectively, and Î´ri , i = 1, 2, ..., m and Î´Ïj , j =
1, 2, ..., n are the virtual_displacements and virtual_rotations, respectively.
Suppose the system consists of N particles, and it has f (f â¤ 6N) degrees_of
freedom. It is sufficient to use only f coordinates to give a complete
description of the motion of the system, so f generalized_coordinates qk , k =
1, 2, ..., f are defined such that the virtual_movements can be expressed in
terms of these generalized_coordinates. That is,
         &#x03B4;   r   i   (  q  1   ,  q  2   , . . . ,  q  f   ; t ) ,  i =
      1 , 2 , . . . , m ;   {\displaystyle \delta \mathbf {r} _{i}(q_{1},q_
      {2},...,q_{f};t),\quad i=1,2,...,m;}  [{\displaystyle \delta \mathbf {r}
      _{i}(q_{1},q_{2},...,q_{f};t),\quad i=1,2,...,m;}]
         &#x03B4;  &#x03D5;  j   (  q  1   ,  q  2   , . . . ,  q  f   ; t ) ,
      j = 1 , 2 , . . . , n .   {\displaystyle \delta \phi _{j}(q_{1},q_
      {2},...,q_{f};t),\quad j=1,2,...,n.}  [\delta \phi _{j}(q_{1},q_
      {2},...,q_{f};t),\quad j=1,2,...,n.]
The virtual work can then be reparametrized by the generalized_coordinates:
         &#x03B4; W =  &#x2211;  k = 1   f    [   (   &#x2211;  i = 1   m     F
      i   &#x22C5;    &#x2202;   r   i     &#x2202;  q  k      +  &#x2211;  j =
      1   n     M   j   &#x22C5;    &#x2202;   &#x03D5;   j     &#x2202;  q  k
      )  &#x03B4;  q  k    ]  =  &#x2211;  k = 1   f    Q  k   &#x03B4;  q  k
      ,   {\displaystyle \delta W=\sum _{k=1}^{f}\left[\left(\sum _{i=1}^
      {m}\mathbf {F} _{i}\cdot {\frac {\partial \mathbf {r} _{i}}{\partial q_
      {k}}}+\sum _{j=1}^{n}\mathbf {M} _{j}\cdot {\frac {\partial \mathbf {\phi
      } _{j}}{\partial q_{k}}}\right)\delta q_{k}\right]=\sum _{k=1}^{f}Q_
      {k}\delta q_{k},}  [\delta W=\sum _{k=1}^{f}\left[\left(\sum _{i=1}^
      {m}\mathbf {F} _{i}\cdot {\frac {\partial \mathbf {r} _{i}}{\partial q_
      {k}}}+\sum _{j=1}^{n}\mathbf {M} _{j}\cdot {\frac {\partial \mathbf {\phi
      } _{j}}{\partial q_{k}}}\right)\delta q_{k}\right]=\sum _{k=1}^{f}Q_
      {k}\delta q_{k},]
where the generalized_forces Qk are defined as
          Q  k   =  &#x2211;  i = 1   m     F   i   &#x22C5;    &#x2202;   r
      i     &#x2202;  q  k      +  &#x2211;  j = 1   n     M   j   &#x22C5;
      &#x2202;   &#x03D5;   j     &#x2202;  q  k      ,  k = 1 , 2 , . . . , f
      .   {\displaystyle Q_{k}=\sum _{i=1}^{m}\mathbf {F} _{i}\cdot {\frac
      {\partial \mathbf {r} _{i}}{\partial q_{k}}}+\sum _{j=1}^{n}\mathbf {M} _
      {j}\cdot {\frac {\partial \mathbf {\phi } _{j}}{\partial q_{k}}},\quad
      k=1,2,...,f.}  [Q_{k}=\sum _{i=1}^{m}\mathbf {F} _{i}\cdot {\frac
      {\partial \mathbf {r} _{i}}{\partial q_{k}}}+\sum _{j=1}^{n}\mathbf {M} _
      {j}\cdot {\frac {\partial \mathbf {\phi } _{j}}{\partial q_{k}}},\quad
      k=1,2,...,f.]
Kane[5] shows that these generalized_forces can also be formulated in terms of
the ratio of time derivatives. That is,
          Q  k   =  &#x2211;  i = 1   m     F   i   &#x22C5;    &#x2202;   v
      i     &#x2202;     q &#x02D9;     k      +  &#x2211;  j = 1   n     M   j
      &#x22C5;    &#x2202;   &#x03C9;   j     &#x2202;     q &#x02D9;     k
      ,  k = 1 , 2 , . . . , f .   {\displaystyle Q_{k}=\sum _{i=1}^{m}\mathbf
      {F} _{i}\cdot {\frac {\partial \mathbf {v} _{i}}{\partial {\dot {q}}_
      {k}}}+\sum _{j=1}^{n}\mathbf {M} _{j}\cdot {\frac {\partial \mathbf
      {\omega } _{j}}{\partial {\dot {q}}_{k}}},\quad k=1,2,...,f.}  [Q_
      {k}=\sum _{i=1}^{m}\mathbf {F} _{i}\cdot {\frac {\partial \mathbf {v} _
      {i}}{\partial {\dot {q}}_{k}}}+\sum _{j=1}^{n}\mathbf {M} _{j}\cdot
      {\frac {\partial \mathbf {\omega } _{j}}{\partial {\dot {q}}_{k}}},\quad
      k=1,2,...,f.]
The principle of virtual work requires that the virtual work done on a system
by the forces Fi and moments Mj vanishes if it is in equilibrium. Therefore,
the generalized forces Qk are zero, that is
         &#x03B4; W = 0  &#x21D2;   Q  k   = 0  k = 1 , 2 , . . . , f .
      {\displaystyle \delta W=0\quad \Rightarrow \quad Q_{k}=0\quad
      k=1,2,...,f.}  [\delta W=0\quad \Rightarrow \quad Q_{k}=0\quad
      k=1,2,...,f.]
**** Constraint forces[edit] ****
An important benefit of the principle of virtual work is that only forces that
do work as the system moves through a virtual_displacement are needed to
determine the mechanics of the system. There are many forces in a mechanical
system that do no work during a virtual_displacement, which means that they
need not be considered in this analysis. The two important examples are (i) the
internal forces in a rigid_body, and (ii) the constraint forces at an ideal
joint.
Lanczos[1] presents this as the postulate: "The virtual work of the forces of
reaction is always zero for any virtual_displacement which is in harmony with
the given kinematic constraints." The argument is as follows. The principle of
virtual work states that in equilibrium the virtual work of the forces applied
to a system is zero. Newton's_laws state that at equilibrium the applied forces
are equal and opposite to the reaction, or constraint forces. This means the
virtual work of the constraint forces must be zero as well.

***** Law of the lever[edit] *****
A lever is modeled as a rigid bar connected to a ground frame by a hinged joint
called a fulcrum. The lever is operated by applying an input force FA at a
point A located by the coordinate vector rA on the bar. The lever then exerts
an output force FB at the point B located by rB. The rotation of the lever
about the fulcrum P is defined by the rotation angle Î¸.
This is an engraving from Mechanics Magazine published in London in 1824.
Let the coordinate vector of the point P that defines the fulcrum be rP, and
introduce the lengths
         a =  |    r   A   &#x2212;   r   P    |  ,  b =  |    r   B   &#x2212;
      r   P    |  ,   {\displaystyle a=|\mathbf {r} _{A}-\mathbf {r} _
      {P}|,\quad b=|\mathbf {r} _{B}-\mathbf {r} _{P}|,}  [a=|\mathbf {r} _{A}-
      \mathbf {r} _{P}|,\quad b=|\mathbf {r} _{B}-\mathbf {r} _{P}|,]
which are the distances from the fulcrum to the input point A and to the output
point B, respectively.
Now introduce the unit vectors eA and eB from the fulcrum to the point A and B,
so
           r   A   &#x2212;   r   P   = a   e   A   ,    r   B   &#x2212;   r
      P   = b   e   B   .   {\displaystyle \mathbf {r} _{A}-\mathbf {r} _
      {P}=a\mathbf {e} _{A},\quad \mathbf {r} _{B}-\mathbf {r} _{P}=b\mathbf
      {e} _{B}.}  [\mathbf {r} _{A}-\mathbf {r} _{P}=a\mathbf {e} _{A},\quad
      \mathbf {r} _{B}-\mathbf {r} _{P}=b\mathbf {e} _{B}.]
This notation allows us to define the velocity of the points A and B as
           v   A   =    &#x03B8; &#x02D9;    a   e   A   &#x22A5;   ,    v   B
      =    &#x03B8; &#x02D9;    b   e   B   &#x22A5;   ,   {\displaystyle
      \mathbf {v} _{A}={\dot {\theta }}a\mathbf {e} _{A}^{\perp },\quad \mathbf
      {v} _{B}={\dot {\theta }}b\mathbf {e} _{B}^{\perp },}  [\mathbf {v} _{A}=
      {\dot {\theta }}a\mathbf {e} _{A}^{\perp },\quad \mathbf {v} _{B}={\dot
      {\theta }}b\mathbf {e} _{B}^{\perp },]
where eAâ¥ and eBâ¥ are unit vectors perpendicular to eA and eB,
respectively.
The angle Î¸ is the generalized coordinate that defines the configuration of
the lever, therefore using the formula above for forces applied to a one
degree-of-freedom mechanism, the generalized force is given by
         Q =   F   A   &#x22C5;    &#x2202;   v   A     &#x2202;    &#x03B8;
      &#x02D9;       &#x2212;   F   B   &#x22C5;    &#x2202;   v   B
      &#x2202;    &#x03B8; &#x02D9;       = a (   F   A   &#x22C5;   e   A
      &#x22A5;   ) &#x2212; b (   F   B   &#x22C5;   e   B   &#x22A5;   ) .
      {\displaystyle Q=\mathbf {F} _{A}\cdot {\frac {\partial \mathbf {v} _{A}}
      {\partial {\dot {\theta }}}}-\mathbf {F} _{B}\cdot {\frac {\partial
      \mathbf {v} _{B}}{\partial {\dot {\theta }}}}=a(\mathbf {F} _{A}\cdot
      \mathbf {e} _{A}^{\perp })-b(\mathbf {F} _{B}\cdot \mathbf {e} _{B}^
      {\perp }).}  [Q=\mathbf {F} _{A}\cdot {\frac {\partial \mathbf {v} _{A}}
      {\partial {\dot {\theta }}}}-\mathbf {F} _{B}\cdot {\frac {\partial
      \mathbf {v} _{B}}{\partial {\dot {\theta }}}}=a(\mathbf {F} _{A}\cdot
      \mathbf {e} _{A}^{\perp })-b(\mathbf {F} _{B}\cdot \mathbf {e} _{B}^
      {\perp }).]
Now, denote as FA and FB the components of the forces that are perpendicular to
the radial segments PA and PB. These forces are given by
          F  A   =   F   A   &#x22C5;   e   A   &#x22A5;   ,   F  B   =   F   B
      &#x22C5;   e   B   &#x22A5;   .   {\displaystyle F_{A}=\mathbf {F} _
      {A}\cdot \mathbf {e} _{A}^{\perp },\quad F_{B}=\mathbf {F} _{B}\cdot
      \mathbf {e} _{B}^{\perp }.}  [F_{A}=\mathbf {F} _{A}\cdot \mathbf {e} _
      {A}^{\perp },\quad F_{B}=\mathbf {F} _{B}\cdot \mathbf {e} _{B}^{\perp
      }.]
This notation and the principle of virtual work yield the formula for the
generalized force as
         Q = a  F  A   &#x2212; b  F  B   = 0.   {\displaystyle Q=aF_{A}-bF_
      {B}=0.}  [{\displaystyle Q=aF_{A}-bF_{B}=0.}]
The ratio of the output force FB to the input force FA is the mechanical
advantage of the lever, and is obtained from the principle of virtual work as
         M A =    F  B    F  A     =   a b   .   {\displaystyle MA={\frac {F_
      {B}}{F_{A}}}={\frac {a}{b}}.}  [MA={\frac {F_{B}}{F_{A}}}={\frac {a}
      {b}}.]
This equation shows that if the distance a from the fulcrum to the point A
where the input force is applied is greater than the distance b from fulcrum to
the point B where the output force is applied, then the lever amplifies the
input force. If the opposite is true that the distance from the fulcrum to the
input point A is less than from the fulcrum to the output point B, then the
lever reduces the magnitude of the input force.
This is the law of the lever, which was proven by Archimedes using geometric
reasoning.[6]
***** Gear train[edit] *****
A gear train is formed by mounting gears on a frame so that the teeth of the
gears engage. Gear teeth are designed to ensure the pitch circles of engaging
gears roll on each other without slipping, this provides a smooth transmission
of rotation from one gear to the next. For this analysis, we consider a gear
train that has one degree-of-freedom, which means the angular rotation of all
the gears in the gear train are defined by the angle of the input gear.
Illustration from Army Service Corps Training on Mechanical Transport, (1911),
Fig. 112 Transmission of motion and force by gear wheels, compound train
The size of the gears and the sequence in which they engage define the ratio of
the angular velocity ÏA of the input gear to the angular velocity ÏB of the
output gear, known as the speed ratio, or gear_ratio, of the gear train. Let R
be the speed ratio, then
            &#x03C9;  A    &#x03C9;  B     = R .   {\displaystyle {\frac
      {\omega _{A}}{\omega _{B}}}=R.}  [{\frac {\omega _{A}}{\omega _{B}}}=R.]
The input torque TA acting on the input gear GA is transformed by the gear
train into the output torque TB exerted by the output gear GB. If we assume,
that the gears are rigid and that there are no losses in the engagement of the
gear teeth, then the principle of virtual work can be used to analyze the
static equilibrium of the gear train.
Let the angle Î¸ of the input gear be the generalized coordinate of the gear
train, then the speed ratio R of the gear train defines the angular velocity of
the output gear in terms of the input gear, that is
          &#x03C9;  A   = &#x03C9; ,   &#x03C9;  B   = &#x03C9;  /  R .
      {\displaystyle \omega _{A}=\omega ,\quad \omega _{B}=\omega /R.}  [
      {\displaystyle \omega _{A}=\omega ,\quad \omega _{B}=\omega /R.}]
The formula above for the principle of virtual work with applied torques yields
the generalized force
         Q =  T  A      &#x2202;  &#x03C9;  A     &#x2202; &#x03C9;    &#x2212;
      T  B      &#x2202;  &#x03C9;  B     &#x2202; &#x03C9;    =  T  A
      &#x2212;  T  B    /  R = 0.   {\displaystyle Q=T_{A}{\frac {\partial
      \omega _{A}}{\partial \omega }}-T_{B}{\frac {\partial \omega _{B}}
      {\partial \omega }}=T_{A}-T_{B}/R=0.}  [Q=T_{A}{\frac {\partial \omega _
      {A}}{\partial \omega }}-T_{B}{\frac {\partial \omega _{B}}{\partial
      \omega }}=T_{A}-T_{B}/R=0.]
The mechanical_advantage of the gear train is the ratio of the output torque TB
to the input torque TA, and the above equation yields
         M A =    T  B    T  A     = R .   {\displaystyle MA={\frac {T_{B}}{T_
      {A}}}=R.}  [MA={\frac {T_{B}}{T_{A}}}=R.]
Thus, the speed ratio of a gear train also defines its mechanical advantage.
This shows that if the input gear rotates faster than the output gear, then the
gear train amplifies the input torque. And, if the input gear rotates slower
than the output gear, then the gear train reduces the input torque.
***** Dynamic equilibrium for rigid bodies[edit] *****
If the principle of virtual work for applied forces is used on individual
particles of a rigid_body, the principle can be generalized for a rigid body:
When a rigid body that is in equilibrium is subject to virtual compatible
displacements, the total virtual work of all external forces is zero; and
conversely, if the total virtual work of all external forces acting on a rigid
body is zero then the body is in equilibrium.
If a system is not in static equilibrium, D'Alembert showed that by introducing
the acceleration terms of Newton's laws as inertia forces, this approach is
generalized to define dynamic equilibrium. The result is D'Alembert's form of
the principle of virtual work, which is used to derive the equations of motion
for a mechanical system of rigid bodies.
The expression compatible displacements means that the particles remain in
contact and displace together so that the work done by pairs of action/reaction
inter-particle forces cancel out. Various forms of this principle have been
credited to Johann_(Jean)_Bernoulli (1667â1748) and Daniel_Bernoulli
(1700â1782).

**** Generalized inertia forces[edit] ****
Let a mechanical system be constructed from n rigid bodies, Bi, i=1,...,n, and
let the resultant of the applied forces on each body be the force-torque pairs,
Fi and Ti, i=1,...,n. Notice that these applied forces do not include the
reaction forces where the bodies are connected. Finally, assume that the
velocity Vi and angular velocities Ïi, i=,1...,n, for each rigid body, are
defined by a single generalized coordinate q. Such a system of rigid bodies is
said to have one degree_of_freedom.
Consider a single rigid body which moves under the action of a resultant force
F and torque T, with one degree of freedom defined by the generalized
coordinate q. Assume the reference point for the resultant force and torque is
the center of mass of the body, then the generalized inertia force Q*
associated with the generalized coordinate q is given by
          Q  &#x2217;   = &#x2212; ( M  A  ) &#x22C5;    &#x2202;  V
      &#x2202;    q &#x02D9;       &#x2212; ( [  I  R   ] &#x03B1; + &#x03C9;
      &#x00D7; [  I  R   ] &#x03C9; ) &#x22C5;    &#x2202;    &#x03C9; &#x2192;
      &#x2202;    q &#x02D9;       .   {\displaystyle Q^{*}=-(M\mathbf {A}
      )\cdot {\frac {\partial \mathbf {V} }{\partial {\dot {q}}}}-([I_
      {R}]\alpha +\omega \times [I_{R}]\omega )\cdot {\frac {\partial {\vec
      {\omega }}}{\partial {\dot {q}}}}.}  [Q^{*}=-(M\mathbf {A} )\cdot {\frac
      {\partial \mathbf {V} }{\partial {\dot {q}}}}-([I_{R}]\alpha +\omega
      \times [I_{R}]\omega )\cdot {\frac {\partial {\vec {\omega }}}{\partial
      {\dot {q}}}}.]
This inertia force can be computed from the kinetic energy of the rigid body,
         T =   1 2   M  V  &#x22C5;  V  +   1 2      &#x03C9; &#x2192;
      &#x22C5; [  I  R   ]    &#x03C9; &#x2192;    ,   {\displaystyle T={\frac
      {1}{2}}M\mathbf {V} \cdot \mathbf {V} +{\frac {1}{2}}{\vec {\omega
      }}\cdot [I_{R}]{\vec {\omega }},}  [T={\frac {1}{2}}M\mathbf {V} \cdot
      \mathbf {V} +{\frac {1}{2}}{\vec {\omega }}\cdot [I_{R}]{\vec {\omega
      }},]
by using the formula
          Q  &#x2217;   = &#x2212;  (    d  d t       &#x2202; T   &#x2202;
      q &#x02D9;       &#x2212;    &#x2202; T   &#x2202; q     )  .
      {\displaystyle Q^{*}=-\left({\frac {d}{dt}}{\frac {\partial T}{\partial
      {\dot {q}}}}-{\frac {\partial T}{\partial q}}\right).}  [Q^{*}=-\left(
      {\frac {d}{dt}}{\frac {\partial T}{\partial {\dot {q}}}}-{\frac {\partial
      T}{\partial q}}\right).]
A system of n rigid bodies with m generalized coordinates has the kinetic
energy
         T =  &#x2211;  i = 1   n   (   1 2   M   V   i   &#x22C5;   V   i   +
      1 2       &#x03C9; &#x2192;     i   &#x22C5; [  I  R   ]     &#x03C9;
      &#x2192;     i   ) ,   {\displaystyle T=\sum _{i=1}^{n}({\frac {1}
      {2}}M\mathbf {V} _{i}\cdot \mathbf {V} _{i}+{\frac {1}{2}}{\vec {\omega
      }}_{i}\cdot [I_{R}]{\vec {\omega }}_{i}),}  [T=\sum _{i=1}^{n}({\frac {1}
      {2}}M\mathbf {V} _{i}\cdot \mathbf {V} _{i}+{\frac {1}{2}}{\vec {\omega
      }}_{i}\cdot [I_{R}]{\vec {\omega }}_{i}),]
which can be used to calculate the m generalized inertia forces[7]
          Q  j   &#x2217;   = &#x2212;  (    d  d t       &#x2202; T   &#x2202;
      q &#x02D9;     j      &#x2212;    &#x2202; T   &#x2202;  q  j       )  ,
      j = 1 , &#x2026; , m .   {\displaystyle Q_{j}^{*}=-\left({\frac {d}{dt}}
      {\frac {\partial T}{\partial {\dot {q}}_{j}}}-{\frac {\partial T}
      {\partial q_{j}}}\right),\quad j=1,\ldots ,m.}  [Q_{j}^{*}=-\left({\frac
      {d}{dt}}{\frac {\partial T}{\partial {\dot {q}}_{j}}}-{\frac {\partial T}
      {\partial q_{j}}}\right),\quad j=1,\ldots ,m.]
**** D'Alembert's form of the principle of virtual work[edit] ****
D'Alembert's form of the principle of virtual work states that a system of
rigid bodies is in dynamic equilibrium when the virtual work of the sum of the
applied forces and the inertial forces is zero for any virtual displacement of
the system. Thus, dynamic equilibrium of a system of n rigid bodies with m
generalized coordinates requires that
         &#x03B4; W = (  Q  1   +  Q  1   &#x2217;   ) &#x03B4;  q  1   +
      &#x2026; + (  Q  m   +  Q  m   &#x2217;   ) &#x03B4;  q  m   = 0 ,
      {\displaystyle \delta W=(Q_{1}+Q_{1}^{*})\delta q_{1}+\ldots +(Q_{m}+Q_
      {m}^{*})\delta q_{m}=0,}  [\delta W=(Q_{1}+Q_{1}^{*})\delta q_{1}+\ldots
      +(Q_{m}+Q_{m}^{*})\delta q_{m}=0,]
for any set of virtual displacements Î´qj. This condition yields m equations,
          Q  j   +  Q  j   &#x2217;   = 0 ,  j = 1 , &#x2026; , m ,
      {\displaystyle Q_{j}+Q_{j}^{*}=0,\quad j=1,\ldots ,m,}  [Q_{j}+Q_{j}^
      {*}=0,\quad j=1,\ldots ,m,]
which can also be written as
           d  d t       &#x2202; T   &#x2202;     q &#x02D9;     j
      &#x2212;    &#x2202; T   &#x2202;  q  j      =  Q  j   ,  j = 1 ,
      &#x2026; , m .   {\displaystyle {\frac {d}{dt}}{\frac {\partial T}
      {\partial {\dot {q}}_{j}}}-{\frac {\partial T}{\partial q_{j}}}=Q_
      {j},\quad j=1,\ldots ,m.}  [{\frac {d}{dt}}{\frac {\partial T}{\partial
      {\dot {q}}_{j}}}-{\frac {\partial T}{\partial q_{j}}}=Q_{j},\quad
      j=1,\ldots ,m.]
The result is a set of m equations of motion that define the dynamics of the
rigid body system.
If the generalized forces Qj are derivable from a potential energy V
(q1,...,qm), then these equations of motion take the form
           d  d t       &#x2202; T   &#x2202;     q &#x02D9;     j
      &#x2212;    &#x2202; T   &#x2202;  q  j      = &#x2212;    &#x2202; V
      &#x2202;  q  j      ,  j = 1 , &#x2026; , m .   {\displaystyle {\frac {d}
      {dt}}{\frac {\partial T}{\partial {\dot {q}}_{j}}}-{\frac {\partial T}
      {\partial q_{j}}}=-{\frac {\partial V}{\partial q_{j}}},\quad j=1,\ldots
      ,m.}  [{\frac {d}{dt}}{\frac {\partial T}{\partial {\dot {q}}_{j}}}-
      {\frac {\partial T}{\partial q_{j}}}=-{\frac {\partial V}{\partial q_
      {j}}},\quad j=1,\ldots ,m.]
In this case, introduce the Lagrangian, L=T-V, so these equations of motion
become
           d  d t       &#x2202; L   &#x2202;     q &#x02D9;     j
      &#x2212;    &#x2202; L   &#x2202;  q  j      = 0  j = 1 , &#x2026; , m .
      {\displaystyle {\frac {d}{dt}}{\frac {\partial L}{\partial {\dot {q}}_
      {j}}}-{\frac {\partial L}{\partial q_{j}}}=0\quad j=1,\ldots ,m.}  [
      {\frac {d}{dt}}{\frac {\partial L}{\partial {\dot {q}}_{j}}}-{\frac
      {\partial L}{\partial q_{j}}}=0\quad j=1,\ldots ,m.]
These are known as Lagrange's_equations_of_motion.
***** Virtual work principle for a deformable body[edit] *****
Consider now the free_body_diagram of a deformable_body, which is composed of
an infinite number of differential cubes. Let's define two unrelated states for
the body:
    * The      &#x03C3;    {\displaystyle {\boldsymbol {\sigma }}}  [
      {\boldsymbol {\sigma }}]-State : This shows external surface forces T,
      body forces f, and internal stresses      &#x03C3;    {\displaystyle
      {\boldsymbol {\sigma }}}  [{\boldsymbol {\sigma }}] in equilibrium.
    * The      &#x03F5;    {\displaystyle {\boldsymbol {\epsilon }}}  [
      {\boldsymbol {\epsilon }}]-State : This shows continuous displacements
      u   &#x2217;     {\displaystyle \mathbf {u} ^{*}}  [\mathbf {u} ^{*}] and
      consistent strains       &#x03F5;   &#x2217;     {\displaystyle
      {\boldsymbol {\epsilon }}^{*}}  [{\boldsymbol {\epsilon }}^{*}].
The superscript * emphasizes that the two states are unrelated. Other than the
above stated conditions, there is no need to specify if any of the states are
real or virtual.
Imagine now that the forces and stresses in the      &#x03C3;    {\displaystyle
{\boldsymbol {\sigma }}}  [{\boldsymbol {\sigma }}]-State undergo the
displacements and deformations in the      &#x03F5;    {\displaystyle
{\boldsymbol {\epsilon }}}  [{\boldsymbol {\epsilon }}]-State: We can compute
the total virtual (imaginary) work done by all forces acting on the faces of
all cubes in two different ways:
    * First, by summing the work done by forces such as      F  A
      {\displaystyle F_{A}}  [F_{A}] which act on individual common faces
      (Fig.c): Since the material experiences compatible displacements, such
      work cancels out, leaving only the virtual work done by the surface
      forces T (which are equal to stresses on the cubes' faces, by
      equilibrium).
    * Second, by computing the net work done by stresses or forces such as
      F  A     {\displaystyle F_{A}}  [F_{A}],      F  B     {\displaystyle F_
      {B}}  [F_{B}] which act on an individual cube, e.g. for the one-
      dimensional case in Fig.(c):
          F  B    (   u  &#x2217;   +    &#x2202;  u  &#x2217;     &#x2202; x
      d x  )  &#x2212;  F  A    u  &#x2217;   &#x2248;    &#x2202;  u  &#x2217;
      &#x2202; x    &#x03C3; d V +  u  &#x2217;      &#x2202; &#x03C3;
      &#x2202; x    d V =  &#x03F5;  &#x2217;   &#x03C3; d V &#x2212;  u
      &#x2217;   f d V   {\displaystyle F_{B}\left(u^{*}+{\frac {\partial u^
      {*}}{\partial x}}dx\right)-F_{A}u^{*}\approx {\frac {\partial u^{*}}
      {\partial x}}\sigma dV+u^{*}{\frac {\partial \sigma }{\partial
      x}}dV=\epsilon ^{*}\sigma dV-u^{*}fdV}  [{\displaystyle F_{B}\left(u^{*}+
      {\frac {\partial u^{*}}{\partial x}}dx\right)-F_{A}u^{*}\approx {\frac
      {\partial u^{*}}{\partial x}}\sigma dV+u^{*}{\frac {\partial \sigma }
      {\partial x}}dV=\epsilon ^{*}\sigma dV-u^{*}fdV}]
      where the equilibrium relation        &#x2202; &#x03C3;   &#x2202; x    +
      f = 0   {\displaystyle {\frac {\partial \sigma }{\partial x}}+f=0}  [
      {\frac {\partial \sigma }{\partial x}}+f=0] has been used and the second
      order term has been neglected.
      Integrating over the whole body gives:
          &#x222B;  V     &#x03F5;   &#x2217; T    &#x03C3;   d V
      {\displaystyle \int _{V}{\boldsymbol {\epsilon }}^{*T}{\boldsymbol
      {\sigma }}\,dV}  [\int _{V}{\boldsymbol {\epsilon }}^{*T}{\boldsymbol
      {\sigma }}\,dV] â Work done by the body forces f.
Equating the two results leads to the principle of virtual work for a
deformable body:
           Total external virtual work   =  &#x222B;  V     &#x03F5;   &#x2217;
      T    &#x03C3;  d V   ( d )    {\displaystyle {\mbox{Total external
      virtual work}}=\int _{V}{\boldsymbol {\epsilon }}^{*T}{\boldsymbol
      {\sigma }}dV\qquad \mathrm {(d)} }  [{\mbox{Total external virtual
      work}}=\int _{V}{\boldsymbol {\epsilon }}^{*T}{\boldsymbol {\sigma
      }}dV\qquad \mathrm {(d)} ]
where the total external virtual work is done by T and f. Thus,
          &#x222B;  S     u   &#x2217; T    T  d S +  &#x222B;  V     u
      &#x2217; T    f  d V =  &#x222B;  V     &#x03F5;   &#x2217; T    &#x03C3;
      d V   ( e )    {\displaystyle \int _{S}\mathbf {u} ^{*T}\mathbf {T}
      dS+\int _{V}\mathbf {u} ^{*T}\mathbf {f} dV=\int _{V}{\boldsymbol
      {\epsilon }}^{*T}{\boldsymbol {\sigma }}dV\qquad \mathrm {(e)} }  [\int _
      {S}\mathbf {u} ^{*T}\mathbf {T} dS+\int _{V}\mathbf {u} ^{*T}\mathbf {f}
      dV=\int _{V}{\boldsymbol {\epsilon }}^{*T}{\boldsymbol {\sigma }}dV\qquad
      \mathrm {(e)} ]
The right-hand-side of (d,e) is often called the internal virtual work. The
principle of virtual work then states: External virtual work is equal to
internal virtual work when equilibrated forces and stresses undergo unrelated
but consistent displacements and strains. It includes the principle of virtual
work for rigid bodies as a special case where the internal virtual work is
zero.
**** Proof of equivalence between the principle of virtual work and the
equilibrium equation[edit] ****
We start by looking at the total work done by surface traction on the body
going through the specified deformation:
          &#x222B;  S    u &#x22C5; T  d S =  &#x222B;  S    u &#x22C5;
      &#x03C3;  &#x22C5; n  d S   {\displaystyle \int _{S}\mathbf {u\cdot T}
      dS=\int _{S}\mathbf {u\cdot {\boldsymbol {\sigma }}\cdot n} dS}  [\int _
      {S}\mathbf {u\cdot T} dS=\int _{S}\mathbf {u\cdot {\boldsymbol {\sigma
      }}\cdot n} dS]
Applying divergence theorem to the right hand side yields:
          &#x222B;  S    u &#x22C5;  &#x03C3;  &#x22C5; n  d S =  &#x222B;  V
      &#x2207; &#x22C5;  (   u  &#x22C5;  &#x03C3;   )  d V   {\displaystyle
      \int _{S}\mathbf {u\cdot {\boldsymbol {\sigma }}\cdot n} dS=\int _
      {V}\nabla \cdot \left(\mathbf {u} \cdot {\boldsymbol {\sigma }}\right)dV}
      [\int _{S}\mathbf {u\cdot {\boldsymbol {\sigma }}\cdot n} dS=\int _
      {V}\nabla \cdot \left(\mathbf {u} \cdot {\boldsymbol {\sigma }}\right)dV]
Now switch to indicial notation for the ease of derivation.
              &#x222B;  V   &#x2207; &#x22C5;  (   u  &#x22C5;  &#x03C3;   )  d
      V    =  &#x222B;  V     &#x2202;  &#x2202;  x  j       (   u  i
      &#x03C3;  i j    )  d V       =  &#x222B;  V      &#x2202;  u  i
      &#x2202;  x  j       &#x03C3;  i j   +  u  i      &#x2202;  &#x03C3;  i j
      &#x2202;  x  j      d V       {\displaystyle {\begin{aligned}\int _
      {V}\nabla \cdot \left(\mathbf {u} \cdot {\boldsymbol {\sigma
      }}\right)dV&=\int _{V}{\frac {\partial }{\partial x_{j}}}\left(u_
      {i}\sigma _{ij}\right)dV\\&=\int _{V}{\frac {\partial u_{i}}{\partial x_
      {j}}}\sigma _{ij}+u_{i}{\frac {\partial \sigma _{ij}}{\partial x_
      {j}}}dV\end{aligned}}}  [{\begin{aligned}\int _{V}\nabla \cdot \left
      (\mathbf {u} \cdot {\boldsymbol {\sigma }}\right)dV&=\int _{V}{\frac
      {\partial }{\partial x_{j}}}\left(u_{i}\sigma _{ij}\right)dV\\&=\int _{V}
      {\frac {\partial u_{i}}{\partial x_{j}}}\sigma _{ij}+u_{i}{\frac
      {\partial \sigma _{ij}}{\partial x_{j}}}dV\end{aligned}}]
To continue our derivation, we substitute in the equilibrium equation
&#x2202;  &#x03C3;  i j     &#x2202;  x  j      +  f  i   = 0   {\displaystyle
{\frac {\partial \sigma _{ij}}{\partial x_{j}}}+f_{i}=0}  [{\frac {\partial
\sigma _{ij}}{\partial x_{j}}}+f_{i}=0]. Then
          &#x222B;  V      &#x2202;  u  i     &#x2202;  x  j       &#x03C3;  i
      j   +  u  i      &#x2202;  &#x03C3;  i j     &#x2202;  x  j      d V =
      &#x222B;  V      &#x2202;  u  i     &#x2202;  x  j       &#x03C3;  i j
      &#x2212;  u  i    f  i   d V   {\displaystyle \int _{V}{\frac {\partial
      u_{i}}{\partial x_{j}}}\sigma _{ij}+u_{i}{\frac {\partial \sigma _{ij}}
      {\partial x_{j}}}dV=\int _{V}{\frac {\partial u_{i}}{\partial x_
      {j}}}\sigma _{ij}-u_{i}f_{i}dV}  [\int _{V}{\frac {\partial u_{i}}
      {\partial x_{j}}}\sigma _{ij}+u_{i}{\frac {\partial \sigma _{ij}}
      {\partial x_{j}}}dV=\int _{V}{\frac {\partial u_{i}}{\partial x_
      {j}}}\sigma _{ij}-u_{i}f_{i}dV]
The first term on the right hand side needs to be broken into a symmetric part
and a skew part as follows:
              &#x222B;  V      &#x2202;  u  i     &#x2202;  x  j       &#x03C3;
      i j   &#x2212;  u  i    f  i   d V    =  &#x222B;  V     1 2    [
      (     &#x2202;  u  i     &#x2202;  x  j      +    &#x2202;  u  j
      &#x2202;  x  i       )  +  (     &#x2202;  u  i     &#x2202;  x  j
      &#x2212;    &#x2202;  u  j     &#x2202;  x  i       )   ]   &#x03C3;  i j
      &#x2212;  u  i    f  i   d V       =  &#x222B;  V    [   &#x03F5;  i j
      +   1 2    (     &#x2202;  u  i     &#x2202;  x  j      &#x2212;
      &#x2202;  u  j     &#x2202;  x  i       )   ]   &#x03C3;  i j   &#x2212;
      u  i    f  i   d V       =  &#x222B;  V    &#x03F5;  i j    &#x03C3;  i j
      &#x2212;  u  i    f  i   d V       =  &#x222B;  V    &#x03F5;  :
      &#x03C3;  &#x2212;  u  &#x22C5;  f  d V       {\displaystyle {\begin
      {aligned}\int _{V}{\frac {\partial u_{i}}{\partial x_{j}}}\sigma _{ij}-u_
      {i}f_{i}dV&=\int _{V}{\frac {1}{2}}\left[\left({\frac {\partial u_{i}}
      {\partial x_{j}}}+{\frac {\partial u_{j}}{\partial x_{i}}}\right)+\left(
      {\frac {\partial u_{i}}{\partial x_{j}}}-{\frac {\partial u_{j}}{\partial
      x_{i}}}\right)\right]\sigma _{ij}-u_{i}f_{i}dV\\&=\int _{V}\left[\epsilon
      _{ij}+{\frac {1}{2}}\left({\frac {\partial u_{i}}{\partial x_{j}}}-{\frac
      {\partial u_{j}}{\partial x_{i}}}\right)\right]\sigma _{ij}-u_{i}f_
      {i}dV\\&=\int _{V}\epsilon _{ij}\sigma _{ij}-u_{i}f_{i}dV\\&=\int _{V}
      {\boldsymbol {\epsilon }}:{\boldsymbol {\sigma }}-\mathbf {u} \cdot
      \mathbf {f} dV\end{aligned}}}  [{\begin{aligned}\int _{V}{\frac {\partial
      u_{i}}{\partial x_{j}}}\sigma _{ij}-u_{i}f_{i}dV&=\int _{V}{\frac {1}
      {2}}\left[\left({\frac {\partial u_{i}}{\partial x_{j}}}+{\frac {\partial
      u_{j}}{\partial x_{i}}}\right)+\left({\frac {\partial u_{i}}{\partial x_
      {j}}}-{\frac {\partial u_{j}}{\partial x_{i}}}\right)\right]\sigma _{ij}-
      u_{i}f_{i}dV\\&=\int _{V}\left[\epsilon _{ij}+{\frac {1}{2}}\left({\frac
      {\partial u_{i}}{\partial x_{j}}}-{\frac {\partial u_{j}}{\partial x_
      {i}}}\right)\right]\sigma _{ij}-u_{i}f_{i}dV\\&=\int _{V}\epsilon _
      {ij}\sigma _{ij}-u_{i}f_{i}dV\\&=\int _{V}{\boldsymbol {\epsilon }}:
      {\boldsymbol {\sigma }}-\mathbf {u} \cdot \mathbf {f} dV\end{aligned}}]
where      &#x03F5;    {\displaystyle {\boldsymbol {\epsilon }}}  [{\boldsymbol
{\epsilon }}] is the strain that is consistent with the specified displacement
field. The 2nd to last equality comes from the fact that the stress matrix is
symmetric and that the product of a skew matrix and a symmetric matrix is zero.
Now recap. We have shown through the above derivation that
          &#x222B;  S    u &#x22C5; T  d S =  &#x222B;  V    &#x03F5;  :
      &#x03C3;  d V &#x2212;  &#x222B;  V    u  &#x22C5;  f  d V
      {\displaystyle \int _{S}\mathbf {u\cdot T} dS=\int _{V}{\boldsymbol
      {\epsilon }}:{\boldsymbol {\sigma }}dV-\int _{V}\mathbf {u} \cdot \mathbf
      {f} dV}  [\int _{S}\mathbf {u\cdot T} dS=\int _{V}{\boldsymbol {\epsilon
      }}:{\boldsymbol {\sigma }}dV-\int _{V}\mathbf {u} \cdot \mathbf {f} dV]
Move the 2nd term on the right hand side of the equation to the left:
          &#x222B;  S    u &#x22C5; T  d S +  &#x222B;  V    u  &#x22C5;  f  d
      V =  &#x222B;  V    &#x03F5;  :  &#x03C3;  d V   {\displaystyle \int _
      {S}\mathbf {u\cdot T} dS+\int _{V}\mathbf {u} \cdot \mathbf {f} dV=\int _
      {V}{\boldsymbol {\epsilon }}:{\boldsymbol {\sigma }}dV}  [\int _
      {S}\mathbf {u\cdot T} dS+\int _{V}\mathbf {u} \cdot \mathbf {f} dV=\int _
      {V}{\boldsymbol {\epsilon }}:{\boldsymbol {\sigma }}dV]
The physical interpretation of the above equation is, the External virtual work
is equal to internal virtual work when equilibrated forces and stresses undergo
unrelated but consistent displacements and strains.
For practical applications:
    * In order to impose equilibrium on real stresses and forces, we use
      consistent virtual displacements and strains in the virtual work
      equation.
    * In order to impose consistent displacements and strains, we use
      equilibriated virtual stresses and forces in the virtual work equation.
These two general scenarios give rise to two often stated variational
principles. They are valid irrespective of material behaviour.
**** Principle of virtual displacements[edit] ****
Depending on the purpose, we may specialize the virtual work equation. For
example, to derive the principle of virtual displacements in variational
notations for supported bodies, we specify:
    * Virtual displacements and strains as variations of the real displacements
      and strains using variational notation such as     &#x03B4; &#xA0;  u
      &#x2261;   u   &#x2217;     {\displaystyle \delta \ \mathbf {u} \equiv
      \mathbf {u} ^{*}}  [\delta \ \mathbf {u} \equiv \mathbf {u} ^{*}] and
      &#x03B4; &#xA0;  &#x03F5;  &#x2261;   &#x03F5;   &#x2217;
      {\displaystyle \delta \ {\boldsymbol {\epsilon }}\equiv {\boldsymbol
      {\epsilon }}^{*}}  [\delta \ {\boldsymbol {\epsilon }}\equiv {\boldsymbol
      {\epsilon }}^{*}]
    * Virtual displacements be zero on the part of the surface that has
      prescribed displacements, and thus the work done by the reactions is
      zero. There remains only external surface forces on the part      S  t
      {\displaystyle S_{t}}  [S_{t}] that do work.
The virtual work equation then becomes the principle of virtual displacements:
          &#x222B;   S  t     &#x03B4; &#xA0;   u   T    T  d S +  &#x222B;  V
      &#x03B4; &#xA0;   u   T    f  d V =  &#x222B;  V   &#x03B4;   &#x03F5;
      T    &#x03C3;  d V   ( f )    {\displaystyle \int _{S_{t}}\delta \
      \mathbf {u} ^{T}\mathbf {T} dS+\int _{V}\delta \ \mathbf {u} ^{T}\mathbf
      {f} dV=\int _{V}\delta {\boldsymbol {\epsilon }}^{T}{\boldsymbol {\sigma
      }}dV\qquad \mathrm {(f)} }  [\int _{S_{t}}\delta \ \mathbf {u} ^
      {T}\mathbf {T} dS+\int _{V}\delta \ \mathbf {u} ^{T}\mathbf {f} dV=\int _
      {V}\delta {\boldsymbol {\epsilon }}^{T}{\boldsymbol {\sigma }}dV\qquad
      \mathrm {(f)} ]
This relation is equivalent to the set of equilibrium equations written for a
differential element in the deformable body as well as of the stress boundary
conditions on the part      S  t     {\displaystyle S_{t}}  [S_{t}] of the
surface. Conversely, (f) can be reached, albeit in a non-trivial manner, by
starting with the differential equilibrium equations and the stress boundary
conditions on      S  t     {\displaystyle S_{t}}  [S_{t}], and proceeding in
the manner similar to (a) and (b).
Since virtual displacements are automatically compatible when they are
expressed in terms of continuous, single-valued_functions, we often mention
only the need for consistency between strains and displacements. The virtual
work principle is also valid for large real displacements; however, Eq.(f)
would then be written using more complex measures of stresses and strains.
**** Principle of virtual forces[edit] ****
Here, we specify:
    * Virtual forces and stresses as variations of the real forces and
      stresses.
    * Virtual forces be zero on the part      S  t     {\displaystyle S_{t}}
      [S_{t}] of the surface that has prescribed forces, and thus only surface
      (reaction) forces on      S  u     {\displaystyle S_{u}}  [S_{u}] (where
      displacements are prescribed) would do work.
The virtual work equation becomes the principle of virtual forces:
          &#x222B;   S  u       u   T   &#x03B4; &#xA0;  T  d S +  &#x222B;  V
      u   T   &#x03B4; &#xA0;  f  d V =  &#x222B;  V     &#x03F5;   T
      &#x03B4;  &#x03C3;  d V   ( g )    {\displaystyle \int _{S_{u}}\mathbf
      {u} ^{T}\delta \ \mathbf {T} dS+\int _{V}\mathbf {u} ^{T}\delta \ \mathbf
      {f} dV=\int _{V}{\boldsymbol {\epsilon }}^{T}\delta {\boldsymbol {\sigma
      }}dV\qquad \mathrm {(g)} }  [\int _{S_{u}}\mathbf {u} ^{T}\delta \
      \mathbf {T} dS+\int _{V}\mathbf {u} ^{T}\delta \ \mathbf {f} dV=\int _{V}
      {\boldsymbol {\epsilon }}^{T}\delta {\boldsymbol {\sigma }}dV\qquad
      \mathrm {(g)} ]
This relation is equivalent to the set of strain-compatibility equations as
well as of the displacement boundary conditions on the part      S  u
{\displaystyle S_{u}}  [S_{u}]. It has another name: the principle of
complementary virtual work.
***** Alternative forms[edit] *****
A specialization of the principle of virtual forces is the unit_dummy_force
method, which is very useful for computing displacements in structural systems.
According to D'Alembert's_principle, inclusion of inertial forces as additional
body forces will give the virtual work equation applicable to dynamical
systems. More generalized principles can be derived by:
    * allowing variations of all quantities.
    * using Lagrange_multipliers to impose boundary conditions and/or to relax
      the conditions specified in the two states.
These are described in some of the references.
Among the many energy_principles_in_structural_mechanics, the virtual work
principle deserves a special place due to its generality that leads to powerful
applications in structural_analysis, solid_mechanics, and finite_element_method
in_structural_mechanics.
***** See also[edit] *****
    * Flexibility_method
    * Unit_dummy_force_method
    * Finite_element_method_in_structural_mechanics
    * Calculus_of_variations
    * Lagrangian_mechanics
    * MÃ¼ller-Breslau's_principle
***** External links[edit] *****
    * Examples_applications_of_the_virtual_work_principle
***** References[edit] *****
   1. ^ a b C._LÃ¡nczos,_The_Variational_Principles_of_Mechanics,_4th_Ed.,
      General_Publishing_Co.,_Canada,_1970
   2. ^ Dym, C. L. and I. H. Shames, Solid Mechanics: A Variational Approach,
      McGraw-Hill, 1973.
   3. ^ a b c d eCapecchi, Danilo (2012). History of Virtual Work Laws. Milano:
      Springer Milan. doi:10.1007/978-88-470-2056-6. ISBN 978-88-470-2055-9.
   4. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   5. ^ RenÃ© Dugas, A History of Mechanics, Courier Corporation, 2012
   6. ^ T. R. Kane and D. A. Levinson, Dynamics: theory and applications,
      McGraw-Hill, New York, 1985
   7. ^Usher,_A._P. (1929). A_History_of_Mechanical_Inventions. Harvard
      University Press (reprinted by Dover Publications 1988). p. 94. ISBN 978-
      0-486-14359-0. OCLC 514178. Retrieved 7 April 2013.
   8. ^ T. R. Kane and D. A. Levinson, Dynamics,_Theory_and_Applications,
      McGraw-Hill, NY, 2005.
***** Bibliography[edit] *****
    * Bathe,_K.J. "Finite Element Procedures", Prentice Hall, 1996.
ISBN 0-13-301458-4
Charlton, T.M. Energy Principles in Theory of Structures, Oxford University
Press, 1973.
ISBN 0-19-714102-1
Dym, C. L. and I. H. Shames, Solid Mechanics: A Variational Approach, McGraw-
Hill, 1973.
Greenwood, Donald T. Classical Dynamics, Dover Publications Inc., 1977,
ISBN 0-486-69690-1
Hu, H. Variational Principles of Theory of Elasticity With Applications, Taylor
& Francis, 1984.
ISBN 0-677-31330-6
Langhaar, H. L. Energy Methods in Applied Mechanics, Krieger, 1989.
Reddy,_J.N. Energy Principles and Variational Methods in Applied Mechanics,
John Wiley, 2002.
ISBN 0-471-17985-X
Shames, I. H. and Dym, C. L. Energy and Finite Element Methods in Structural
Mechanics, Taylor & Francis, 1995,
ISBN 0-89116-942-3
Tauchert, T.R. Energy Principles in Structural Mechanics, McGraw-Hill, 1974.
ISBN 0-07-062925-0
Washizu, K. Variational Methods in Elasticity and Plasticity, Pergamon Pr,
1982.
ISBN 0-08-026723-8
Wunderlich, W. Mechanics of Structures: Variational and Computational Methods,
CRC, 2002.
ISBN 0-8493-0700-7

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Virtual_work&oldid=903570336"
Categories:
    * Mechanics
    * Dynamical_systems
    * Structural_analysis
    * Linkages_(mechanical)
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
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * ä¸­æ
Edit_links
    * This page was last edited on 26 June 2019, at 13:18 (UTC).
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
