The following text has been accessed from https://en.wikipedia.org/wiki/Rigid_body at Fri Aug 9 03:07:04 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Rigid body ******
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
    * Harmonic_oscillator
    * Inertial / Non-inertial_reference_frame
    * Mechanics_of_planar_particle_motion
    * Motion (linear)
    * Newton's_law_of_universal_gravitation
    * Newton's_laws_of_motion
    * Relative_velocity
    * Rigid body
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
The position of a rigid body is determined by the position of its center of
mass and by its attitude (at least six parameters in total).[1]
In physics, a rigid body (also known as rigid object [2]) is a solid body in
which deformation is zero or so small it can be neglected. The distance between
any two given points on a rigid body remains constant in time regardless of
external forces exerted on it. A rigid body is usually considered as a
continuous distribution of mass.
In the study of special_relativity, a perfectly rigid body does not exist; and
objects can only be assumed to be rigid if they are not moving near the speed
of_light. In quantum_mechanics a rigid body is usually thought of as a
collection of point masses. For instance, in quantum mechanics molecules
(consisting of the point masses: electrons and nuclei) are often seen as rigid
bodies (see classification_of_molecules_as_rigid_rotors).
⁰
***** Contents *****
    * 1_Kinematics
          o 1.1_Linear_and_angular_position
          o 1.2_Linear_and_angular_velocity
    * 2_Kinematical_equations
          o 2.1_Addition_theorem_for_angular_velocity
          o 2.2_Addition_theorem_for_position
          o 2.3_Mathematical_definition_of_velocity
          o 2.4_Mathematical_definition_of_acceleration
          o 2.5_Velocity_of_two_points_fixed_on_a_rigid_body
          o 2.6_Acceleration_of_two_points_fixed_on_a_rigid_body
          o 2.7_Angular_velocity_and_acceleration_of_two_points_fixed_on_a
            rigid_body
          o 2.8_Velocity_of_one_point_moving_on_a_rigid_body
          o 2.9_Acceleration_of_one_point_moving_on_a_rigid_body
          o 2.10_Other_quantities
    * 3_Kinetics
    * 4_Geometry
    * 5_Configuration_space
    * 6_See_also
    * 7_Notes
    * 8_References
    * 9_External_links
***** Kinematics[edit] *****
**** Linear and angular position[edit] ****
The position of a rigid body is the position of all the particles of which it
is composed. To simplify the description of this position, we exploit the
property that the body is rigid, namely that all its particles maintain the
same distance relative to each other. If the body is rigid, it is sufficient to
describe the position of at least three non-collinear particles. This makes it
possible to reconstruct the position of all the other particles, provided that
their time-invariant position relative to the three selected particles is
known. However, typically a different, mathematically more convenient, but
equivalent approach is used. The position of the whole body is represented by:
   1. the linear position or position of the body, namely the position of one
      of the particles of the body, specifically chosen as a reference point
      (typically coinciding with the center_of_mass or centroid of the body),
      together with
   2. the angular_position (also known as orientation, or attitude) of the
      body.
Thus, the position of a rigid body has two components: linear and angular,
respectively.[3] The same is true for other kinematic and kinetic quantities
describing the motion of a rigid body, such as linear and angular velocity,
acceleration, momentum, impulse, and kinetic_energy.[4]
The linear position can be represented by a vector with its tail at an
arbitrary reference point in space (the origin of a chosen coordinate_system)
and its tip at an arbitrary point of interest on the rigid body, typically
coinciding with its center_of_mass or centroid. This reference point may define
the origin of a coordinate_system fixed to the body.
There are several ways to numerically describe the orientation of a rigid body,
including a set of three Euler_angles, a quaternion, or a direction_cosine
matrix (also referred to as a rotation_matrix). All these methods actually
define the orientation of a basis_set (or coordinate_system) which has a fixed
orientation relative to the body (i.e. rotates together with the body),
relative to another basis set (or coordinate system), from which the motion of
the rigid body is observed. For instance, a basis set with fixed orientation
relative to an airplane can be defined as a set of three orthogonal unit
vectors b1, b2, b3, such that b1 is parallel to the chord line of the wing and
directed forward, b2 is normal to the plane of symmetry and directed rightward,
and b3 is given by the cross product      b  3   =  b  1   &#x00D7;  b  2
{\displaystyle b_{3}=b_{1}\times b_{2}}  [ b_3 = b_1 \times b_2 ].
In general, when a rigid body moves, both its position and orientation vary
with time. In the kinematic sense, these changes are referred to as translation
and rotation, respectively. Indeed, the position of a rigid body can be viewed
as a hypothetic translation and rotation (roto-translation) of the body
starting from a hypothetic reference position (not necessarily coinciding with
a position actually taken by the body during its motion).
**** Linear and angular velocity[edit] ****
Velocity (also called linear velocity) and angular_velocity are measured with
respect to a frame_of_reference.
The linear velocity of a rigid body is a vector quantity, equal to the time
rate_of_change of its linear position. Thus, it is the velocity of a reference
point fixed to the body. During purely translational motion (motion with no
rotation), all points on a rigid body move with the same velocity. However,
when motion involves rotation, the instantaneous velocity of any two points on
the body will generally not be the same. Two points of a rotating body will
have the same instantaneous velocity only if they happen to lie on an axis
parallel to the instantaneous axis_of_rotation.
Angular_velocity is a vector quantity that describes the angular_speed at which
the orientation of the rigid body is changing and the instantaneous axis about
which it is rotating (the existence of this instantaneous axis is guaranteed by
the Euler's_rotation_theorem). All points on a rigid body experience the same
angular_velocity at all times. During purely rotational motion, all points on
the body change position except for those lying on the instantaneous axis_of
rotation. The relationship between orientation and angular velocity is not
directly analogous to the relationship between position and velocity. Angular
velocity is not the time_rate_of_change of orientation, because there is no
such concept as an orientation vector that can be differentiated to obtain the
angular velocity.
***** Kinematical equations[edit] *****
**** Addition theorem for angular velocity[edit] ****
The angular velocity of a rigid body B in a reference frame N is equal to the
sum of the angular velocity of a rigid body D in N and the angular velocity of
B with respect to D:[5]
              N       &#x03C9;    B    =      N       &#x03C9;    D    +      D
      &#x03C9;    B    .   {\displaystyle {}^{\mathrm {N} }\!{\boldsymbol
      {\omega }}^{\mathrm {B} }={}^{\mathrm {N} }\!{\boldsymbol {\omega }}^
      {\mathrm {D} }+{}^{\mathrm {D} }\!{\boldsymbol {\omega }}^{\mathrm {B}
      }.}  [ {}^\mathrm{N}\!\boldsymbol{\omega}^\mathrm{B} = {}^\mathrm
      {N}\!\boldsymbol{\omega}^\mathrm{D} + {}^\mathrm{D}\!\boldsymbol
      {\omega}^\mathrm{B}.]
In this case, rigid bodies and reference frames are indistinguishable and
completely interchangeable.
**** Addition theorem for position[edit] ****
For any set of three points P, Q, and R, the position vector from P to R is the
sum of the position vector from P to Q and the position vector from Q to R:
           r    P R    =   r    P Q    +   r    Q R    .   {\displaystyle
      \mathbf {r} ^{\mathrm {PR} }=\mathbf {r} ^{\mathrm {PQ} }+\mathbf {r} ^
      {\mathrm {QR} }.}  [ \mathbf{r}^\mathrm{PR} = \mathbf{r}^\mathrm{PQ} +
      \mathbf{r}^\mathrm{QR}.]
**** Mathematical definition of velocity[edit] ****
The velocity of point P in reference frame N is defined as the time_derivative
in N of the position vector from O to P:[6]
              N      v    P    =         N     d     d  t    (   r    O P    )
      {\displaystyle {}^{\mathrm {N} }\mathbf {v} ^{\mathrm {P} }={\frac {{}^
      {\mathrm {N} }\mathrm {d} }{\mathrm {d} t}}(\mathbf {r} ^{\mathrm {OP}
      })}  [ {}^\mathrm{N}\mathbf{v}^\mathrm{P} = \frac{{}^\mathrm{N}\mathrm
      {d}}{\mathrm{d}t}(\mathbf{r}^\mathrm{OP}) ]
where O is any arbitrary point fixed in reference frame N, and the N to the
left of the d/dt operator indicates that the derivative is taken in reference
frame N. The result is independent of the selection of O so long as O is fixed
in N.
**** Mathematical definition of acceleration[edit] ****
The acceleration of point P in reference frame N is defined as the time
derivative in N of its velocity:[6]
              N      a    P    =        N     d     d  t    (      N      v
      P    ) .   {\displaystyle {}^{\mathrm {N} }\mathbf {a} ^{\mathrm {P} }=
      {\frac {^{\mathrm {N} }\mathrm {d} }{\mathrm {d} t}}({}^{\mathrm {N}
      }\mathbf {v} ^{\mathrm {P} }).}  [ {}^\mathrm{N}\mathbf{a}^\mathrm{P} =
      \frac{^\mathrm{N}\mathrm{d}}{\mathrm{d}t} ({}^\mathrm{N}\mathbf
      {v}^\mathrm{P}).]
**** Velocity of two points fixed on a rigid body[edit] ****
For two points P and Q that are fixed on a rigid body B, where B has an angular
velocity           N      &#x03C9;    B        {\displaystyle \scriptstyle {^
{\mathrm {N} }{\boldsymbol {\omega }}^{\mathrm {B} }}}  [\scriptstyle{^\mathrm
{N}\boldsymbol{\omega}^\mathrm{B}}] in the reference frame N, the velocity of Q
in N can be expressed as a function of the velocity of P in N:[7]
              N      v    Q    =      N       v    P    +      N      &#x03C9;
      B    &#x00D7;   r    P Q    .   {\displaystyle {}^{\mathrm {N} }\mathbf
      {v} ^{\mathrm {Q} }={}^{\mathrm {N} }\!\mathbf {v} ^{\mathrm {P} }+{}^
      {\mathrm {N} }{\boldsymbol {\omega }}^{\mathrm {B} }\times \mathbf {r} ^
      {\mathrm {PQ} }.}  [ {}^\mathrm{N}\mathbf{v}^\mathrm{Q} = {}^\mathrm
      {N}\!\mathbf{v}^\mathrm{P} + {}^\mathrm{N}\boldsymbol{\omega}^\mathrm{B}
      \times \mathbf{r}^\mathrm{PQ}.]
**** Acceleration of two points fixed on a rigid body[edit] ****
By differentiating the equation for the Velocity of two points fixed on a rigid
body in N with respect to time, the acceleration in reference frame N of a
point Q fixed on a rigid body B can be expressed as
              N      a    Q    =      N      a    P    +      N      &#x03C9;
      B    &#x00D7;  (       N      &#x03C9;    B    &#x00D7;   r    P Q     )
      +      N      &#x03B1;    B    &#x00D7;   r    P Q      {\displaystyle
      {}^{\mathrm {N} }\mathbf {a} ^{\mathrm {Q} }={}^{\mathrm {N} }\mathbf {a}
      ^{\mathrm {P} }+{}^{\mathrm {N} }{\boldsymbol {\omega }}^{\mathrm {B}
      }\times \left({}^{\mathrm {N} }{\boldsymbol {\omega }}^{\mathrm {B}
      }\times \mathbf {r} ^{\mathrm {PQ} }\right)+{}^{\mathrm {N} }{\boldsymbol
      {\alpha }}^{\mathrm {B} }\times \mathbf {r} ^{\mathrm {PQ} }}  [
      {}^\mathrm{N}\mathbf{a}^\mathrm{Q} = {}^\mathrm{N}\mathbf{a}^\mathrm{P} +
      {}^\mathrm{N}\boldsymbol{\omega}^\mathrm{B} \times \left( {}^\mathrm
      {N}\boldsymbol{\omega}^\mathrm{B} \times \mathbf{r}^\mathrm{PQ} \right) +
      {}^\mathrm{N}\boldsymbol{\alpha}^\mathrm{B} \times \mathbf{r}^\mathrm{PQ}
      ]
where            N       &#x03B1;    B        {\displaystyle \scriptstyle {{}^
{\mathrm {N} }\!{\boldsymbol {\alpha }}^{\mathrm {B} }}}  [\scriptstyle{
{}^\mathrm{N}\!\boldsymbol{\alpha}^\mathrm{B}}] is the angular acceleration of
B in the reference frame N.[7]
**** Angular velocity and acceleration of two points fixed on a rigid body
[edit] ****
As mentioned above, all points on a rigid body B have the same angular velocity
N      &#x03C9;    B      {\displaystyle {}^{\mathrm {N} }{\boldsymbol {\omega
}}^{\mathrm {B} }}  [{}^\mathrm{N}\boldsymbol{\omega}^\mathrm{B}] in a fixed
reference frame N, and thus the same angular acceleration          N
&#x03B1;    B    .   {\displaystyle {}^{\mathrm {N} }{\boldsymbol {\alpha }}^
{\mathrm {B} }.}  [{}^\mathrm{N}\boldsymbol{\alpha}^\mathrm{B}.]
**** Velocity of one point moving on a rigid body[edit] ****
If the point R is moving in rigid body B while B moves in reference frame N,
then the velocity of R in N is
              N      v    R    =      N      v    Q    +      B      v    R
      {\displaystyle {}^{\mathrm {N} }\mathbf {v} ^{\mathrm {R} }={}^{\mathrm
      {N} }\mathbf {v} ^{\mathrm {Q} }+{}^{\mathrm {B} }\mathbf {v} ^{\mathrm
      {R} }}  [ {}^\mathrm{N}\mathbf{v}^\mathrm{R} = {}^\mathrm{N}\mathbf
      {v}^\mathrm{Q} + {}^\mathrm{B}\mathbf{v}^\mathrm{R}]
where Q is the point fixed in B that is instantaneously coincident with R at
the instant of interest.[8] This relation is often combined with the relation
for the Velocity of two points fixed on a rigid body.
**** Acceleration of one point moving on a rigid body[edit] ****
The acceleration in reference frame N of the point R moving in body B while B
is moving in frame N is given by
              N      a    R    =      N      a    Q    +      B      a    R
      + 2      N      &#x03C9;    B    &#x00D7;      B      v    R
      {\displaystyle {}^{\mathrm {N} }\mathbf {a} ^{\mathrm {R} }={}^{\mathrm
      {N} }\mathbf {a} ^{\mathrm {Q} }+{}^{\mathrm {B} }\mathbf {a} ^{\mathrm
      {R} }+2{}^{\mathrm {N} }{\boldsymbol {\omega }}^{\mathrm {B} }\times {}^
      {\mathrm {B} }\mathbf {v} ^{\mathrm {R} }}  [ {}^\mathrm{N}\mathbf
      {a}^\mathrm{R} = {}^\mathrm{N}\mathbf{a}^\mathrm{Q} + {}^\mathrm
      {B}\mathbf{a}^\mathrm{R} + 2 {}^\mathrm{N}\boldsymbol{\omega}^\mathrm{B}
      \times {}^\mathrm{B}\mathbf{v}^\mathrm{R} ]
where Q is the point fixed in B that instantaneously coincident with R at the
instant of interest.[8] This equation is often combined with Acceleration of
two points fixed on a rigid body.
**** Other quantities[edit] ****
If C is the origin of a local coordinate_system L, attached to the body,
    * the spatial or twist acceleration of a rigid body is defined as the
      spatial_acceleration of C (as opposed to material acceleration above);
          &#x03C8;  ( t ,   r   0   ) =  a  ( t ,   r   0   ) &#x2212;
      &#x03C9;  ( t ) &#x00D7;  v  ( t ,   r   0   ) =   &#x03C8;   c   ( t ) +
      &#x03B1;  ( t ) &#x00D7; A ( t )   r   0     {\displaystyle {\boldsymbol
      {\psi }}(t,\mathbf {r} _{0})=\mathbf {a} (t,\mathbf {r} _{0})-
      {\boldsymbol {\omega }}(t)\times \mathbf {v} (t,\mathbf {r} _{0})=
      {\boldsymbol {\psi }}_{c}(t)+{\boldsymbol {\alpha }}(t)\times A(t)\mathbf
      {r} _{0}}  [ \boldsymbol\psi(t,\mathbf{r}_0) = \mathbf{a}(t,\mathbf{r}_0)
      - \boldsymbol\omega(t) \times \mathbf{v}(t,\mathbf{r}_0) =
      \boldsymbol\psi_c(t) + \boldsymbol\alpha(t) \times A(t) \mathbf{r}_0]
where
    *      r   0     {\displaystyle \mathbf {r} _{0}}  [ \mathbf{r}_0 ]
      represents the position of the point/particle with respect to the
      reference point of the body in terms of the local coordinate system L
      (the rigidity of the body means that this does not depend on time)
    *    A ( t )    {\displaystyle A(t)\,}  [A(t)\, ] is the orientation
      matrix, an orthogonal_matrix with determinant 1, representing the
      orientation (angular position) of the local coordinate system L, with
      respect to the arbitrary reference orientation of another coordinate
      system G. Think of this matrix as three orthogonal unit vectors, one in
      each column, which define the orientation of the axes of L with respect
      to G.
    *     &#x03C9;  ( t )   {\displaystyle {\boldsymbol {\omega }}(t)}
      [\boldsymbol\omega(t)] represents the angular_velocity of the rigid body
    *     v  ( t ,   r   0   )   {\displaystyle \mathbf {v} (t,\mathbf {r} _
      {0})}  [\mathbf{v}(t,\mathbf{r}_0)] represents the total velocity of the
      point/particle
    *     a  ( t ,   r   0   )   {\displaystyle \mathbf {a} (t,\mathbf {r} _
      {0})}  [\mathbf{a}(t,\mathbf{r}_0)] represents the total acceleration of
      the point/particle
    *     &#x03B1;  ( t )   {\displaystyle {\boldsymbol {\alpha }}(t)}
      [\boldsymbol\alpha(t)] represents the angular_acceleration of the rigid
      body
    *     &#x03C8;  ( t ,   r   0   )   {\displaystyle {\boldsymbol {\psi }}
      (t,\mathbf {r} _{0})}  [\boldsymbol\psi(t,\mathbf{r}_0)] represents the
      spatial_acceleration of the point/particle
    *      &#x03C8;   c   ( t )   {\displaystyle {\boldsymbol {\psi }}_{c}(t)}
      [\boldsymbol\psi_c(t)] represents the spatial_acceleration of the rigid
      body (i.e. the spatial acceleration of the origin of L).
In 2D, the angular velocity is a scalar, and matrix A(t) simply represents a
rotation in the xy-plane by an angle which is the integral of the angular
velocity over time.
Vehicles, walking people, etc., usually rotate according to changes in the
direction of the velocity: they move forward with respect to their own
orientation. Then, if the body follows a closed orbit in a plane, the angular
velocity integrated over a time interval in which the orbit is completed once,
is an integer times 360Â°. This integer is the winding_number with respect to
the origin of the velocity. Compare the amount_of_rotation_associated_with_the
vertices_of_a_polygon.
***** Kinetics[edit] *****
Main article: Rigid_body_dynamics
Any point that is rigidly connected to the body can be used as reference point
(origin of coordinate system L) to describe the linear motion of the body (the
linear position, velocity and acceleration vectors depend on the choice).
However, depending on the application, a convenient choice may be:
    * the center_of_mass of the whole system, which generally has the simplest
      motion for a body moving freely in space;
    * a point such that the translational motion is zero or simplified, e.g. on
      an axle or hinge, at the center of a ball_and_socket_joint, etc.
When the center of mass is used as reference point:
    * The (linear) momentum is independent of the rotational motion. At any
      time it is equal to the total mass of the rigid body times the
      translational velocity.
    * The angular_momentum with respect to the center of mass is the same as
      without translation: at any time it is equal to the inertia_tensor times
      the angular velocity. When the angular velocity is expressed with respect
      to a coordinate system coinciding with the principal_axes of the body,
      each component of the angular momentum is a product of a moment of
      inertia (a principal value of the inertia tensor) times the corresponding
      component of the angular velocity; the torque is the inertia tensor times
      the angular_acceleration.
    * Possible motions in the absence of external forces are translation with
      constant velocity, steady rotation about a fixed principal axis, and also
      torque-free precession.
    * The net external force on the rigid body is always equal to the total
      mass times the translational acceleration (i.e., Newton's_second_law
      holds for the translational motion, even when the net external torque is
      nonzero, and/or the body rotates).
    * The total kinetic_energy is simply the sum of translational and
      rotational_energy.
***** Geometry[edit] *****
Two rigid bodies are said to be different (not copies) if there is no proper
rotation from one to the other. A rigid body is called chiral if its mirror
image is different in that sense, i.e., if it has either no symmetry or its
symmetry_group contains only proper rotations. In the opposite case an object
is called achiral: the mirror image is a copy, not a different object. Such an
object may have a symmetry plane, but not necessarily: there may also be a
plane of reflection with respect to which the image of the object is a rotated
version. The latter applies for S2n, of which the case n = 1 is inversion
symmetry.
For a (rigid) rectangular transparent sheet, inversion symmetry corresponds to
having on one side an image without rotational symmetry and on the other side
an image such that what shines through is the image at the top side, upside
down. We can distinguish two cases:
    * the sheet surface with the image is not symmetric - in this case the two
      sides are different, but the mirror image of the object is the same,
      after a rotation by 180Â° about the axis perpendicular to the mirror
      plane.
    * the sheet surface with the image has a symmetry axis - in this case the
      two sides are the same, and the mirror image of the object is also the
      same, again after a rotation by 180Â° about the axis perpendicular to the
      mirror plane.
A sheet with a through_and_through image is achiral. We can distinguish again
two cases:
    * the sheet surface with the image has no symmetry axis - the two sides are
      different
    * the sheet surface with the image has a symmetry axis - the two sides are
      the same
***** Configuration space[edit] *****
The configuration_space of a rigid body with one point fixed (i.e., a body with
zero translational motion) is given by the underlying manifold of the rotation
group_SO(3). The configuration space of a nonfixed (with non-zero translational
motion) rigid body is E+(3), the subgroup of direct_isometries of the Euclidean
group in three dimensions (combinations of translations and rotations).
***** See also[edit] *****
    * Angular_velocity
    * Axes_conventions
    * Rigid_body_dynamics
    * Infinitesimal_rotations
    * Euler's_equations_(rigid_body_dynamics)
    * Euler's_laws
    * Born_rigidity
    * Rigid_rotor
    * Geometric_Mechanics
    * Classical_Mechanics_(Goldstein)
***** Notes[edit] *****
   1. ^ Lorenzo Sciavicco, Bruno Siciliano (2000). "Â§2.4.2 Roll-pitch-yaw
      angles". Modelling_and_control_of_robot_manipulators (2nd ed.). Springer.
      p. 32. ISBN 1-85233-221-2.
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
   3. ^Andy Ruina and Rudra Pratap (2015). Introduction to Statics and
      Dynamics. Oxford University Press.
   4.  (link: [1])
   5. ^ In general, the position of a point or particle is also known, in
      physics, as linear position, as opposed to the angular position of a
      line, or line segment (e.g., in circular_motion, the "radius" joining the
      rotating point with the center of rotation), or basis_set, or coordinate
      system.
   6. ^ In kinematics, linear means "along a straight or curved line" (the path
      of the particle in space). In mathematics, however, linear has a
      different meaning. In both contexts, the word "linear" is related to the
      word "line". In mathematics, a line is often defined as a straight curve.
      For those who adopt this definition, a curve can be straight, and curved
      lines are not supposed to exist. In kinematics, the term line is used as
      a synonym of the term trajectory, or path (namely, it has the same non-
      restricted meaning as that given, in mathematics, to the word curve). In
      short, both straight and curved lines are supposed to exist. In
      kinematics and dynamics, the following words refer to the same non-
      restricted meaning of the term "line":
          o "linear" (= along a straight or curved line),
          o "rectilinear" (= along a straight line, from Latin rectus =
            straight, and linere = spread),
          o "curvilinear" (=along a curved line, from Latin curvus = curved,
            and linere = spread).
      In topology and meteorology, the term "line" has the same meaning;
      namely, a contour_line is a curve.
   7. ^Kane, Thomas; Levinson, David (1996). "2-4 Auxiliary Reference Frames".
      Dynamics Online. Sunnyvale, California: OnLine Dynamics, Inc.
   8. ^ a bKane, Thomas; Levinson, David (1996). "2-6 Velocity and
      Acceleration". Dynamics Online. Sunnyvale, California: OnLine Dynamics,
      Inc.
   9. ^ a bKane, Thomas; Levinson, David (1996). "2-7 Two Points Fixed on a
      Rigid Body". Dynamics Online. Sunnyvale, California: OnLine Dynamics,
      Inc.
  10. ^ a bKane, Thomas; Levinson, David (1996). "2-8 One Point Moving on a
      Rigid Body". Dynamics Online. Sunnyvale, California: OnLine Dynamics,
      Inc.
***** References[edit] *****
    * Roy Featherstone (1987). Robot Dynamics Algorithms. Springer. ISBN 0-
      89838-230-0.
 This reference effectively combines screw_theory with rigid body dynamics for
robotic applications. The author also chooses to use spatial_accelerations
extensively in place of material accelerations as they simplify the equations
and allow for compact notation.
JPL DARTS page has a section on spatial operator algebra (link: [2]) as well as
an extensive list of references (link: [3]).
Andy Ruina and Rudra Pratap (2015). Introduction to Statics and Dynamics.
Oxford University Press.
 (link: [4]).
***** External links[edit] *****
Rigid bodyat Wikipedia's sister_projects
    * Quotations from Wikiquote

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Rigid_body&oldid=886757655"
Categories:
    * Rigid_bodies
    * Rigid_bodies_mechanics
    * Rotational_symmetry
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
    * Wikiquote
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * KurdÃ®
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * SlovenÅ¡Äina
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 8 March 2019, at 09:42 (UTC).
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
