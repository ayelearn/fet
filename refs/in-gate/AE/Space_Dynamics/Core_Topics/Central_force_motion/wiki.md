The following text has been accessed from https://en.wikipedia.org/wiki/Classical_central-force_problem at Thu Aug 8 23:19:47 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Classical central-force problem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In classical_mechanics, the central-force problem is to determine the motion of
a particle under the influence of a single central_force. A central force is a
force (possibly negative) that points from the particle directly towards a
fixed point in space, the center, and whose magnitude only depends on the
distance of the object to the center. In many important cases, the problem can
be solved analytically, i.e., in terms of well-studied functions such as
trigonometric_functions.
The solution of this problem is important to classical physics, since many
naturally occurring forces are central. Examples include gravity and
electromagnetism as described by Newton's_law_of_universal_gravitation and
Coulomb's_law, respectively. The problem is also important because some more
complicated problems in classical physics (such as the two-body_problem with
forces along the line connecting the two bodies) can be reduced to a central-
force problem. Finally, the solution to the central-force problem often makes a
good initial approximation of the true motion, as in calculating the motion of
the planets in the Solar_System.
⁰
***** Contents *****
    * 1_Basics
          o 1.1_Definition_of_a_central_force
          o 1.2_Potential_energy
          o 1.3_One-dimensional_problem
          o 1.4_Uniform_circular_motion
          o 1.5_Relation_to_the_classical_two-body_problem
    * 2_Qualitative_properties
          o 2.1_Planar_motion
          o 2.2_Polar_coordinates
          o 2.3_Specific_angular_momentum
          o 2.4_Constant_areal_velocity
          o 2.5_Equivalent_parallel_force_field
    * 3_General_solution
          o 3.1_Binet_equation
          o 3.2_Orbit_of_the_particle
          o 3.3_Turning_points_and_closed_orbits
    * 4_Specific_solutions
          o 4.1_Kepler_problem
          o 4.2_Central_forces_with_exact_solutions
          o 4.3_Newton's_theorem_of_revolving_orbits
    * 5_Historical_development
          o 5.1_Newton's_derivation
    * 6_Alternative_derivations_of_the_equations_of_motion
          o 6.1_Lagrangian_mechanics
          o 6.2_Hamiltonian_mechanics
          o 6.3_Hamilton-Jacobi_equation
    * 7_See_also
    * 8_Notes
    * 9_References
    * 10_Bibliography
    * 11_External_links
***** Basics[edit] *****
The essence of the central-force problem is to solve for the position r[note_1]
of a particle moving under the influence of a central_force F, either as a
function of time t or as a function of the angle Ï relative to the center of
force and an arbitrary axis.
**** Definition of a central force[edit] ****
[A_long_arrows_runs_from_the_lower_left_to_the_upper_right._At_the_lower_left,
the_arrow_begins_with_a_black_point_labeled_"O";_at_the_upper_right,_the_arrow
ends_at_a_solid_red_circle_labeled_"P"._Above_this_arrow_is_a_shorter,_thicker
arrow_labeled_"F_sub_att"_that_points_from_the_center_of_P_towards_O.]
An attractive central force acting on a body at position P (shown in red). By
definition, a central force must point either towards a fixed point O (if
attractive) or away from it (if repulsive).
See also: Central_force and Newton's_notation
A conservative central force F has two defining properties.[1] First, it must
drive particles either directly towards or directly away from a fixed point in
space, the center of force, which is often labeled O. In other words, a central
force must act along the line joining O with the present position of the
particle. Second, a conservative central force depends only on the distance r
between O and the moving particle; it does not depend explicitly on time or
other descriptors of position.
This two-fold definition may be expressed mathematically as follows. The center
of force O can be chosen as the origin of a coordinate system. The vector r
joining O to the present position of the particle is known as the position
vector. Therefore, a central force must have the mathematical form[2]
          F  = F ( r )     r  &#x005E;      {\displaystyle \mathbf {F} =F(r)
      {\hat {\mathbf {r} }}}  [{\mathbf  {F}}=F(r){\hat  {{\mathbf  {r}}}}]
where r is the vector magnitude |r| (the distance to the center of force) and
rÌ = r/r is the corresponding unit_vector. According to Newton's_second_law_of
motion, the central force F generates a parallel acceleration a scaled by the
mass m of the particle[note_2]
          F  = F ( r )     r  &#x005E;    = m  a  = m     r  &#x00A8;
      {\displaystyle \mathbf {F} =F(r){\hat {\mathbf {r} }}=m\mathbf {a} =m
      {\ddot {\mathbf {r} }}}  [{\mathbf  {F}}=F(r){\hat  {{\mathbf  {r}}}}=m
      {\mathbf  {a}}=m{\ddot  {{\mathbf  {r}}}}]
For attractive forces, F(r) is negative, because it works to reduce the
distance r to the center. Conversely, for repulsive forces, F(r) is positive.
**** Potential energy[edit] ****
See also: Kinetic_energy and Potential_energy
A central force is always a conservative_force; the magnitude F(r) of a central
force can always be expressed as the derivative of a time-independent potential
energy function U(r)[3]
         F ( r ) = &#x2212;    d U   d r      {\displaystyle F(r)=-{\frac {dU}
      {dr}}}  [F(r)=-{\frac  {dU}{dr}}]
Thus, the total energy of the particle—the sum of its kinetic_energy and its
potential_energy U—is a constant; energy is said to be conserved. To show this,
it suffices that the work W done by the force depends only on initial and final
positions, not on the path taken between them.
         W =  &#x222B;    r   1       r   2      F  &#x22C5; d  r  =  &#x222B;
      r   1       r   2     F ( r )     r  &#x005E;    &#x22C5; d  r  =
      &#x222B;   r  1      r  2     F d r = U (  r  1   ) &#x2212; U (  r  2
      )   {\displaystyle W=\int _{\mathbf {r} _{1}}^{\mathbf {r} _{2}}\mathbf
      {F} \cdot d\mathbf {r} =\int _{\mathbf {r} _{1}}^{\mathbf {r} _{2}}F(r)
      {\hat {\mathbf {r} }}\cdot d\mathbf {r} =\int _{r_{1}}^{r_{2}}Fdr=U(r_
      {1})-U(r_{2})}  [W=\int _{{{\mathbf  {r}}_{{1}}}}^{{{\mathbf  {r}}_{
      {2}}}}{\mathbf  {F}}\cdot d{\mathbf  {r}}=\int _{{{\mathbf  {r}}_{{1}}}}^
      {{{\mathbf  {r}}_{{2}}}}F(r){\hat  {{\mathbf  {r}}}}\cdot d{\mathbf
      {r}}=\int _{{r_{{1}}}}^{{r_{{2}}}}Fdr=U(r_{{1}})-U(r_{{2}})]
Equivalently, it suffices that the curl of the force field F is zero; using the
formula_for_the_curl_in_spherical_coordinates,
         &#x2207; &#x00D7;  F  =   1  r sin &#x2061; &#x03B8;     (    &#x2202;
      F   &#x2202; &#x03C6;    )     &#x03B8; &#x005E;    &#x2212;   1 r
      (    &#x2202; F   &#x2202; &#x03B8;    )     &#x03C6; &#x005E;    = 0
      {\displaystyle \nabla \times \mathbf {F} ={\frac {1}{r\sin \theta }}\left
      ({\frac {\partial F}{\partial \varphi }}\right){\hat {\boldsymbol {\theta
      }}}-{\frac {1}{r}}\left({\frac {\partial F}{\partial \theta }}\right)
      {\hat {\boldsymbol {\varphi }}}=0}  [\nabla \times {\mathbf  {F}}={\frac
      {1}{r\sin \theta }}\left({\frac  {\partial F}{\partial \varphi }}\right)
      {\hat  {{\boldsymbol  \theta }}}-{\frac  {1}{r}}\left({\frac  {\partial
      F}{\partial \theta }}\right){\hat  {{\boldsymbol  \varphi }}}=0]
because the partial_derivatives are zero for a central force; the magnitude F
does not depend on the angular spherical_coordinates Î¸ and Ï.
Since the scalar_potential V(r) depends only on the distance r to the origin,
it has spherical_symmetry. In this respect, the central-force problem is
analogous to the Schwarzschild_geodesics in general_relativity and to the
quantum_mechanical treatments of particles_in_potentials_of_spherical_symmetry.
**** One-dimensional problem[edit] ****
If the initial velocity v of the particle is aligned with position vector r,
then the motion remains forever on the line defined by r. This follows because
the force—and by Newton's second law, also the acceleration a—is also aligned
with r. To determine this motion, it suffices to solve the equation
         m    r &#x00A8;    = F ( r )   {\displaystyle m{\ddot {r}}=F(r)}  [m
      {\ddot  {r}}=F(r)]
One solution method is to use the conservation of total energy
          |     r &#x02D9;     |  =   |      d r   d t      |   =    2 m
      E   t o t    &#x2212; U ( r )     {\displaystyle |{\dot {r}}|={\Big |}
      {\frac {dr}{dt}}{\Big |}={\sqrt {\frac {2}{m}}}{\sqrt {E_{\mathrm {tot}
      }-U(r)}}}  [|{\dot  {r}}|={\Big |}{\frac  {dr}{dt}}{\Big |}={\sqrt  {
      {\frac  {2}{m}}}}{\sqrt  {E_{{{\mathrm  {tot}}}}-U(r)}}]
Taking the reciprocal and integrating we get:
          |  t &#x2212;  t  0    |  =    m 2    &#x222B;     |  d r  |     E
      t o t    &#x2212; U ( r )      {\displaystyle |t-t_{0}|={\sqrt {\frac {m}
      {2}}}\int {\frac {|dr|}{\sqrt {E_{\mathrm {tot} }-U(r)}}}}  [|t-t_{{0}}|=
      {{\sqrt  {{\frac  {m}{2}}}}}\int {\frac  {|dr|}{{\sqrt  {E_{{{\mathrm
      {tot}}}}-U(r)}}}}]
For the remainder of the article, it is assumed that the initial velocity v of
the particle is not aligned with position vector r, i.e., that the angular
momentum vector L = r × m v is not zero.
**** Uniform circular motion[edit] ****
Every central force can produce uniform circular motion, provided that the
initial radius r and speed v satisfy the equation for the centripetal_force
            m  v  2    r   = F ( r )   {\displaystyle {\frac {mv^{2}}{r}}=F(r)}
      [{\frac  {mv^{{2}}}{r}}=F(r)]
If this equation is satisfied at the initial moments, it will be satisfied at
all later times; the particle will continue to move in a circle of radius r at
speed v forever.
**** Relation to the classical two-body problem[edit] ****
The positions x1 and x2 of two bodies can be expressed in terms of their
relative separation r and the position of their center of mass Rcm.
See also: Two-body_problem
The central-force problem concerns an ideal situation (a "one-body problem") in
which a single particle is attracted or repelled from an immovable point O, the
center of force.[4] However, physical forces are generally between two bodies;
and by Newton's third law, if the first body applies a force on the second, the
second body applies an equal and opposite force on the first. Therefore, both
bodies are accelerated if a force is present between them; there is no
perfectly immovable center of force. However, if one body is overwhelmingly
more massive than the other, its acceleration relative to the other may be
neglected; the center of the more massive body may be treated as approximately
fixed.[5] For example, the Sun is overwhelmingly more massive than the planet
Mercury; hence, the Sun may be approximated as an immovable center of force,
reducing the problem to the motion of Mercury in response to the force applied
by the Sun. In reality, however, the Sun also moves (albeit only slightly) in
response to the force applied by the planet Mercury.
Any classical two-body problem to be converted into an equivalent one-body
problem. The mass μ of the one equivalent body equals the reduced mass of the
two original bodies, and its position r equals the difference of their
positions.
Such approximations are unnecessary, however. Newton's laws of motion allow any
classical two-body problem to be converted into a corresponding exact one-body
problem.[6] To demonstrate this, let x1 and x2 be the positions of the two
particles, and let r = x1 − x2 be their relative position. Then, by Newton's
second law,
             r  &#x00A8;    =      x  &#x00A8;     1   &#x2212;      x
      &#x00A8;     2   =  (      F   21    m  1     &#x2212;     F   12    m  2
      )  =  (    1  m  1     +   1  m  2      )    F   21     {\displaystyle
      {\ddot {\mathbf {r} }}={\ddot {\mathbf {x} }}_{1}-{\ddot {\mathbf {x} }}_
      {2}=\left({\frac {\mathbf {F} _{21}}{m_{1}}}-{\frac {\mathbf {F} _{12}}
      {m_{2}}}\right)=\left({\frac {1}{m_{1}}}+{\frac {1}{m_{2}}}\right)\mathbf
      {F} _{21}}  [{\ddot  {{\mathbf  {r}}}}={\ddot  {{\mathbf  {x}}}}_{{1}}-
      {\ddot  {{\mathbf  {x}}}}_{{2}}=\left({\frac  {{\mathbf  {F}}_{{21}}}{m_{
      {1}}}}-{\frac  {{\mathbf  {F}}_{{12}}}{m_{{2}}}}\right)=\left({\frac  {1}
      {m_{{1}}}}+{\frac  {1}{m_{{2}}}}\right){\mathbf  {F}}_{{21}}]
The final equation derives from Newton's_third_law; the force of the second
body on the first body (F21) is equal and opposite to the force of the first
body on the second (F12). Thus, the equation of motion for r can be written in
the form
         &#x03BC;     r  &#x00A8;    =  F    {\displaystyle \mu {\ddot {\mathbf
      {r} }}=\mathbf {F} }  [\mu {\ddot  {{\mathbf  {r}}}}={\mathbf  {F}}]
where     &#x03BC;   {\displaystyle \mu }  [\mu ] is the reduced_mass
         &#x03BC; =   1    1  m  1     +   1  m  2        =     m  1    m  2
      m  1   +  m  2        {\displaystyle \mu ={\frac {1}{{\frac {1}{m_{1}}}+
      {\frac {1}{m_{2}}}}}={\frac {m_{1}m_{2}}{m_{1}+m_{2}}}}  [\mu ={\frac
      {1}{{\frac  {1}{m_{{1}}}}+{\frac  {1}{m_{{2}}}}}}={\frac  {m_{{1}}m_{
      {2}}}{m_{{1}}+m_{{2}}}}]
As a special case, the problem of two bodies interacting by a central_force can
be reduced to a central-force problem of one body.
***** Qualitative properties[edit] *****
**** Planar motion[edit] ****
[The_image_shows_a_yellow_disc_with_three_vectors._The_vector_L_is
perpendicular_to_the_disk,_the_vector_r_goes_from_the_center_of_the_disk_to_a
point_on_its_periphery,_and_the_vector_v_is_tangential_to_the_disk,_starting
from_the_point_where_r_meets_the_periphery.]
Illustration of planar motion. The angular momentum vector L is constant;
therefore, the position vector r and velocity vector v must lie in the yellow
plane perpendicular to L.
See also: Angular_momentum
The motion of a particle under a central force F always remains in the plane
defined by its initial position and velocity.[7] This may be seen by symmetry.
Since the position r, velocity v and force F all lie in the same plane, there
is never an acceleration perpendicular to that plane, because that would break
the symmetry between "above" the plane and "below" the plane.
To demonstrate this mathematically, it suffices to show that the angular
momentum of the particle is constant. This angular_momentum L is defined by the
equation
          L  =  r  &#x00D7;  p  =  r  &#x00D7; m  v    {\displaystyle \mathbf
      {L} =\mathbf {r} \times \mathbf {p} =\mathbf {r} \times m\mathbf {v} }  [
      {\mathbf  {L}}={\mathbf  {r}}\times {\mathbf  {p}}={\mathbf  {r}}\times m
      {\mathbf  {v}}]
where m is the mass of the particle and p is its linear_momentum.[note_3]
Therefore, the angular momentum vector L is always perpendicular to the plane
defined by the particle's position vector r and velocity vector v.[note_4]
In general, the rate of change of the angular momentum L equals the net torque
r × F[8]
            d  L    d t    =     r  &#x02D9;    &#x00D7; m  v  +  r  &#x00D7; m
      v  &#x02D9;    =  v  &#x00D7; m  v  +  r  &#x00D7;  F  =  r  &#x00D7;  F
      &#xA0; ,   {\displaystyle {\frac {d\mathbf {L} }{dt}}={\dot {\mathbf {r}
      }}\times m\mathbf {v} +\mathbf {r} \times m{\dot {\mathbf {v} }}=\mathbf
      {v} \times m\mathbf {v} +\mathbf {r} \times \mathbf {F} =\mathbf {r}
      \times \mathbf {F} \ ,}  [{\frac  {d{\mathbf  {L}}}{dt}}={\dot  {{\mathbf
      {r}}}}\times m{\mathbf  {v}}+{\mathbf  {r}}\times m{\dot  {{\mathbf
      {v}}}}={\mathbf  {v}}\times m{\mathbf  {v}}+{\mathbf  {r}}\times {\mathbf
      {F}}={\mathbf  {r}}\times {\mathbf  {F}}\ ,]
The first term m v × v is always zero, because the vector cross_product is
always zero for any two vectors pointing in the same or opposite directions.
However, when F is a central force, the remaining term r × F is also zero
because the vectors r and F point in the same or opposite directions.
Therefore, the angular momentum vector L is constant. Then
          r  &#x22C5;  L  =  r  &#x22C5; (  r  &#x00D7;  p  ) =  p  &#x22C5;
      (  r  &#x00D7;  r  ) = 0   {\displaystyle \mathbf {r} \cdot \mathbf {L}
      =\mathbf {r} \cdot (\mathbf {r} \times \mathbf {p} )=\mathbf {p} \cdot
      (\mathbf {r} \times \mathbf {r} )=0}  [{\displaystyle \mathbf {r} \cdot
      \mathbf {L} =\mathbf {r} \cdot (\mathbf {r} \times \mathbf {p} )=\mathbf
      {p} \cdot (\mathbf {r} \times \mathbf {r} )=0}]
Consequently, the particle's position r (and hence velocity v) always lies in a
plane perpendicular to L.[9]
**** Polar coordinates[edit] ****
[Two_perpendicular_lines_(Cartesian_coordinate_axes)_are_labeled_x_(horizontal)
and_y_(vertical)._They_intersect_at_the_lower_left_in_a_point_labeled_O_(the
origin)._An_arrow_labeled_r_runs_form_the_origin_to_the_upper_right,_ending_in
a_point P._The_angle_between_the_x-axis_and_the_vector_r_is_labeled_with_the
Greek_letter Ï._A_vertical_line_is_dropped_from_P_to_the_x-axis,_and_the
horizontal_and_vertical_segments_are_labeled_"r_cosine_phi"_and_"r_sine_phi",
respectively.]
The position vector r of a point P in the plane can be specified by its
distance r from the center (the origin O) and its azimuthal angle φ. The x and
y Cartesian components of the vector are r cos φ and r sin φ, respectively.
See also: Polar_coordinate_system
Since the motion is planar and the force radial, it is customary to switch to
polar_coordinates.[9] In these coordinates, the position vector r is
represented in terms of the radial distance r and the azimuthal angle Ï.
          r  = ( x , &#xA0; y ) = r ( cos &#x2061; &#x03C6; , &#xA0; sin
      &#x2061; &#x03C6; )   {\displaystyle \mathbf {r} =(x,\ y)=r(\cos \varphi
      ,\ \sin \varphi )}  [{\mathbf  {r}}=(x,\ y)=r(\cos \varphi ,\ \sin
      \varphi )]
Taking the first derivative with respect to time yields the particle's velocity
vector v
          v  =    d  r    d t    =    r &#x02D9;    ( cos &#x2061; &#x03C6; ,
      &#xA0; sin &#x2061; &#x03C6; ) + r    &#x03C6; &#x02D9;    ( &#x2212; sin
      &#x2061; &#x03C6; , cos &#x2061; &#x03C6; )   {\displaystyle \mathbf {v}
      ={\frac {d\mathbf {r} }{dt}}={\dot {r}}(\cos \varphi ,\ \sin \varphi )+r
      {\dot {\varphi }}(-\sin \varphi ,\cos \varphi )}  [{\mathbf  {v}}={\frac
      {d{\mathbf  {r}}}{dt}}={\dot  {r}}(\cos \varphi ,\ \sin \varphi )+r{\dot
      {\varphi }}(-\sin \varphi ,\cos \varphi )]
Similarly, the second derivative of the particle's position r equals its
acceleration a
          a  =    r &#x00A8;    ( cos &#x2061; &#x03C6; , &#xA0; sin &#x2061;
      &#x03C6; ) + 2    r &#x02D9;       &#x03C6; &#x02D9;    ( &#x2212; sin
      &#x2061; &#x03C6; , &#xA0; cos &#x2061; &#x03C6; ) + r    &#x03C6;
      &#x00A8;    ( &#x2212; sin &#x2061; &#x03C6; , cos &#x2061; &#x03C6; )
      &#x2212; r     &#x03C6; &#x02D9;     2   ( cos &#x2061; &#x03C6; , sin
      &#x2061; &#x03C6; )   {\displaystyle \mathbf {a} ={\ddot {r}}(\cos
      \varphi ,\ \sin \varphi )+2{\dot {r}}{\dot {\varphi }}(-\sin \varphi ,\
      \cos \varphi )+r{\ddot {\varphi }}(-\sin \varphi ,\cos \varphi )-r{\dot
      {\varphi }}^{2}(\cos \varphi ,\sin \varphi )}  [{\mathbf  {a}}={\ddot
      {r}}(\cos \varphi ,\ \sin \varphi )+2{\dot  {r}}{\dot  {\varphi }}(-\sin
      \varphi ,\ \cos \varphi )+r{\ddot  {\varphi }}(-\sin \varphi ,\cos
      \varphi )-r{\dot  {\varphi }}^{{2}}(\cos \varphi ,\sin \varphi )]
The velocity v and acceleration a can be expressed in terms of the radial and
azimuthal unit vectors. The radial unit vector is obtained by dividing the
position vector r by its magnitude r, as described above
            r &#x005E;    = ( cos &#x2061; &#x03C6; , &#xA0; sin &#x2061;
      &#x03C6; )   {\displaystyle \mathbf {\hat {r}} =(\cos \varphi ,\ \sin
      \varphi )}  [{\mathbf  {{\hat  {r}}}}=(\cos \varphi ,\ \sin \varphi )]
The azimuthal unit vector is given by[note_5]
            &#x03C6; &#x005E;    = ( &#x2212; sin &#x2061; &#x03C6; , &#xA0;
      cos &#x2061; &#x03C6; )   {\displaystyle {\hat {\boldsymbol {\varphi }}}=
      (-\sin \varphi ,\ \cos \varphi )}  [{\hat  {{\boldsymbol  \varphi }}}=(-
      \sin \varphi ,\ \cos \varphi )]
Thus, the velocity can be written as
          v  =  v  r      r &#x005E;    +  v  &#x03C6;      &#x03C6; &#x005E;
      =    r &#x02D9;       r &#x005E;    + r    &#x03C6; &#x02D9;
      &#x03C6; &#x005E;      {\displaystyle \mathbf {v} =v_{r}\mathbf {\hat
      {r}} +v_{\varphi }{\hat {\boldsymbol {\varphi }}}={\dot {r}}\mathbf {\hat
      {r}} +r{\dot {\varphi }}{\hat {\boldsymbol {\varphi }}}}  [{\mathbf
      {v}}=v_{{r}}{\mathbf  {{\hat  {r}}}}+v_{{\varphi }}{\hat  {{\boldsymbol
      \varphi }}}={\dot  {r}}{\mathbf  {{\hat  {r}}}}+r{\dot  {\varphi }}{\hat
      {{\boldsymbol  \varphi }}}]
whereas the acceleration equals
          a  =  a  r      r &#x005E;    +  a  &#x03C6;      &#x03C6; &#x005E;
      = (    r &#x00A8;    &#x2212; r     &#x03C6; &#x02D9;     2   )    r
      &#x005E;    + ( 2    r &#x02D9;       &#x03C6; &#x02D9;    + r
      &#x03C6; &#x00A8;    )    &#x03C6; &#x005E;      {\displaystyle \mathbf
      {a} =a_{r}\mathbf {\hat {r}} +a_{\varphi }{\hat {\boldsymbol {\varphi
      }}}=({\ddot {r}}-r{\dot {\varphi }}^{2})\mathbf {\hat {r}} +(2{\dot {r}}
      {\dot {\varphi }}+r{\ddot {\varphi }}){\hat {\boldsymbol {\varphi }}}}  [
      {\mathbf  {a}}=a_{{r}}{\mathbf  {{\hat  {r}}}}+a_{{\varphi }}{\hat  {
      {\boldsymbol  \varphi }}}=({\ddot  {r}}-r{\dot  {\varphi }}^{{2}})
      {\mathbf  {{\hat  {r}}}}+(2{\dot  {r}}{\dot  {\varphi }}+r{\ddot
      {\varphi }}){\hat  {{\boldsymbol  \varphi }}}]
**** Specific angular momentum[edit] ****
The specific angular momentum h equals the speed v times r⊥, the component of
the position vector r perpendicular to the velocity vector v. h also equals the
radial distance r times the azimuthal component vφ of the velocity. Both of
these formulae are equal to rv cos β.
See also: Specific_relative_angular_momentum
Since F = ma by Newton's second law of motion and since F is a central force,
then only the radial component of the acceleration a can be non-zero; the
angular component aÏ must be zero
          a  &#x03C6;   = 2    r &#x02D9;       &#x03C6; &#x02D9;    + r
      &#x03C6; &#x00A8;    = 0   {\displaystyle a_{\varphi }=2{\dot {r}}{\dot
      {\varphi }}+r{\ddot {\varphi }}=0}  [a_{{\varphi }}=2{\dot  {r}}{\dot
      {\varphi }}+r{\ddot  {\varphi }}=0]
Therefore,
           d  d t     (   r  2      &#x03C6; &#x02D9;     )  = r ( 2    r
      &#x02D9;       &#x03C6; &#x02D9;    + r    &#x03C6; &#x00A8;    ) = r  a
      &#x03C6;   = 0   {\displaystyle {\frac {d}{dt}}\left(r^{2}{\dot {\varphi
      }}\right)=r(2{\dot {r}}{\dot {\varphi }}+r{\ddot {\varphi }})=ra_{\varphi
      }=0}  [{\frac  {d}{dt}}\left(r^{{2}}{\dot  {\varphi }}\right)=r(2{\dot
      {r}}{\dot  {\varphi }}+r{\ddot  {\varphi }})=ra_{{\varphi }}=0]
This expression in parentheses is usually denoted h
         h =  r  2      &#x03C6; &#x02D9;    = r  v  &#x03C6;   =  |   r
      &#x00D7;  v   |  = v  r  &#x22A5;   =   L m     {\displaystyle h=r^{2}
      {\dot {\varphi }}=rv_{\varphi }=\left|\mathbf {r} \times \mathbf {v}
      \right|=vr_{\perp }={\frac {L}{m}}}  [h=r^{{2}}{\dot  {\varphi }}=rv_{
      {\varphi }}=\left|{\mathbf  {r}}\times {\mathbf  {v}}\right|=vr_{{\perp
      }}={\frac  {L}{m}}]
which equals the speed v times râ¥, the component of the radius vector
perpendicular to the velocity. h is the magnitude of the specific_angular
momentum because it equals the magnitude L of the angular momentum divided by
the mass m of the particle.
For brevity, the angular speed is sometimes written Ï
         &#x03C9; =    &#x03C6; &#x02D9;    =    d &#x03C6;   d t
      {\displaystyle \omega ={\dot {\varphi }}={\frac {d\varphi }{dt}}}
      [\omega ={\dot  {\varphi }}={\frac  {d\varphi }{dt}}]
However, it should not be assumed that Ï is constant. Since h is constant, Ï
varies with the radius r according to the formula[10]
         &#x03C9; =   h  r  2       {\displaystyle \omega ={\frac {h}{r^{2}}}}
      [\omega ={\frac  {h}{r^{{2}}}}]
Since h is constant and r2 is positive, the angle Ï changes monotonically in
any central-force problem, either continuously increasing (h positive) or
continuously decreasing (h negative).[11]
**** Constant areal velocity[edit] ****
Since the area A equals Â½ r⊥vt, the areal velocity dA/dt (the rate at which A
is swept out by the particle) equals Â½ r⊥v = Â½h.
See also: Areal_velocity
The magnitude of h also equals twice the areal_velocity, which is the rate at
which area is being swept out by the particle relative to the center.[12] Thus,
the areal velocity is constant for a particle acted upon by any type of central
force; this is Kepler's_second_law.[13] Conversely, if the motion under a
conservative force F is planar and has constant areal velocity for all initial
conditions of the radius r and velocity v, then the azimuthal acceleration aÏ
is always zero. Hence, by Newton's second law, F = ma, the force is a central
force.
The constancy of areal velocity may be illustrated by uniform circular and
linear motion. In uniform circular motion, the particle moves with constant
speed v around the circumference of a circle of radius r. Since the angular
velocity Ï = v/r is constant, the area swept out in a time Ît equals Ï
r2Ît; hence, equal areas are swept out in equal times Ît. In uniform linear
motion (i.e., motion in the absence of a force, by Newton's first law of
motion), the particle moves with constant velocity, that is, with constant
speed v along a line. In a time Ît, the particle sweeps out an area Â½vÎtrâ¥
(the impact_parameter).[note_6] The distance râ¥ does not change as the
particle moves along the line; it represents the distance of closest approach
of the line to the center O (the impact_parameter). Since the speed v is
likewise unchanging, the areal velocity Â½vrâ¥ is a constant of motion; the
particle sweeps out equal areas in equal times.
The area A of a circular sector equals ½ r2φ = ½ r2ωt = ½ r vφt. Hence, the
areal velocity dA/dt equals ½ r vφ = ½ h. For uniform circular motion, r and vφ
are constant; thus, dA/dt is also constant.
**** Equivalent parallel force field[edit] ****
By a transformation of variables,[14] any central-force problem can be
converted into an equivalent parallel-force problem.[note_7] In place of the
ordinary x and y Cartesian coordinates, two new position variables Î¾ = x/y and
Î· = 1/y are defined, as is a new time coordinate Ï
         &#x03C4; = &#x222B;    d t   y  2       {\displaystyle \tau =\int
      {\frac {dt}{y^{2}}}}  [\tau =\int {\frac  {dt}{y^{{2}}}}]
The corresponding equations of motion for Î¾ and Î· are given by
            d &#x03BE;   d &#x03C4;    =   d  d t     (   x y   )     d t   d
      &#x03C4;    =  (       x &#x02D9;    y &#x2212;    y &#x02D9;    x   y  2
      )   y  2   = &#x2212; h   {\displaystyle {\frac {d\xi }{d\tau }}={\frac
      {d}{dt}}\left({\frac {x}{y}}\right){\frac {dt}{d\tau }}=\left({\frac {
      {\dot {x}}y-{\dot {y}}x}{y^{2}}}\right)y^{2}=-h}  [{\frac  {d\xi }{d\tau
      }}={\frac  {d}{dt}}\left({\frac  {x}{y}}\right){\frac  {dt}{d\tau
      }}=\left({\frac  {{\dot  {x}}y-{\dot  {y}}x}{y^{{2}}}}\right)y^{{2}}=-h]
            d &#x03B7;   d &#x03C4;    =   d  d t     (   1 y   )     d t   d
      &#x03C4;    = &#x2212;     y &#x02D9;    y  2      y  2   = &#x2212;    y
      &#x02D9;      {\displaystyle {\frac {d\eta }{d\tau }}={\frac {d}
      {dt}}\left({\frac {1}{y}}\right){\frac {dt}{d\tau }}=-{\frac {\dot {y}}
      {y^{2}}}y^{2}=-{\dot {y}}}  [{\frac  {d\eta }{d\tau }}={\frac  {d}
      {dt}}\left({\frac  {1}{y}}\right){\frac  {dt}{d\tau }}=-{\frac  {{\dot
      {y}}}{y^{{2}}}}y^{{2}}=-{\dot  {y}}]
Since the rate of change of Î¾ is constant, its second derivative is zero
             d  2   &#x03BE;   d  &#x03C4;  2      = 0   {\displaystyle {\frac
      {d^{2}\xi }{d\tau ^{2}}}=0}  [{\frac  {d^{{2}}\xi }{d\tau ^{{2}}}}=0]
Since this is the acceleration in the Î¾ direction and since F=ma by Newton's
second law, it follows that the force in the Î¾ direction is zero. Hence the
force is only along the Î· direction, which is the criterion for a parallel-
force problem. Explicitly, the acceleration in the Î· direction equals
             d  2   &#x03B7;   d  &#x03C4;  2      =    d t   d &#x03C4;      d
      d t     (    d &#x03B7;   d &#x03C4;    )  = &#x2212;  y  2      y
      &#x00A8;    = &#x2212;    y  3    m r    F ( r )   {\displaystyle {\frac
      {d^{2}\eta }{d\tau ^{2}}}={\frac {dt}{d\tau }}{\frac {d}{dt}}\left({\frac
      {d\eta }{d\tau }}\right)=-y^{2}{\ddot {y}}=-{\frac {y^{3}}{mr}}F(r)}  [
      {\frac  {d^{{2}}\eta }{d\tau ^{{2}}}}={\frac  {dt}{d\tau }}{\frac  {d}
      {dt}}\left({\frac  {d\eta }{d\tau }}\right)=-y^{{2}}{\ddot  {y}}=-{\frac
      {y^{{3}}}{mr}}F(r)]
because the acceleration in the y-direction equals
            y &#x00A8;    =   1 m    F  y   =   1 m   F ( r )    y r
      {\displaystyle {\ddot {y}}={\frac {1}{m}}F_{y}={\frac {1}{m}}F(r)\,{\frac
      {y}{r}}}  [{\ddot  {y}}={\frac  {1}{m}}F_{{y}}={\frac  {1}{m}}F(r)\,
      {\frac  {y}{r}}]
Here, Fy denotes the y-component of the central force, and y/r equals the
cosine of the angle between the y-axis and the radial vector r.
***** General solution[edit] *****
**** Binet equation[edit] ****
See also: Binet_equation
Since a central force F acts only along the radius, only the radial component
of the acceleration is nonzero. By Newton's second law of motion, the magnitude
of F equals the mass m of the particle times the magnitude of its radial
acceleration[15]
         F ( r ) = m    r &#x00A8;    &#x2212; m r  &#x03C9;  2   = m     d  2
      r   d  t  2      &#x2212;    m  h  2     r  3       {\displaystyle F(r)=m
      {\ddot {r}}-mr\omega ^{2}=m{\frac {d^{2}r}{dt^{2}}}-{\frac {mh^{2}}{r^
      {3}}}}  [F(r)=m{\ddot  {r}}-mr\omega ^{{2}}=m{\frac  {d^{{2}}r}{dt^{
      {2}}}}-{\frac  {mh^{{2}}}{r^{{3}}}}]
This equation has integration factor        d r   d t      {\displaystyle
{\frac {dr}{dt}}}  [{\frac  {dr}{dt}}]
             F ( r )  d r    = F ( r )    d r   d t     d t       = m  (     d
      r   d t        d  2   r   d  t  2      &#x2212;    h  2    r  3        d
      r   d t     )   d t       =   m 2    d  [    (    d r   d t    )   2   +
      (   h r   )   2    ]        {\displaystyle {\begin{aligned}F(r)\,dr&=F(r)
      {\frac {dr}{dt}}\,dt\\&=m\left({\frac {dr}{dt}}{\frac {d^{2}r}{dt^{2}}}-
      {\frac {h^{2}}{r^{3}}}{\frac {dr}{dt}}\right)\,dt\\&={\frac {m}
      {2}}\,d\left[\left({\frac {dr}{dt}}\right)^{2}+\left({\frac {h}
      {r}}\right)^{2}\right]\end{aligned}}}  [{\begin{aligned}F(r)\,dr&=F(r)
      {\frac  {dr}{dt}}\,dt\\&=m\left({\frac  {dr}{dt}}{\frac  {d^{{2}}r}{dt^{
      {2}}}}-{\frac  {h^{{2}}}{r^{{3}}}}{\frac  {dr}{dt}}\right)\,dt\\&={\frac
      m2}\,d\left[\left({\frac  {dr}{dt}}\right)^{2}+\left({\frac  hr}\right)^
      {2}\right]\end{aligned}}]
Integrating yields
          &#x222B;  r   F ( r )  d r =   m 2    [    (    d r   d t    )   2
      +   (   h r   )   2    ]    {\displaystyle \int ^{r}F(r)\,dr={\frac {m}
      {2}}\left[\left({\frac {dr}{dt}}\right)^{2}+\left({\frac {h}{r}}\right)^
      {2}\right]}  [\int ^{{r}}F(r)\,dr={\frac  m2}\left[\left({\frac  {dr}
      {dt}}\right)^{2}+\left({\frac  hr}\right)^{2}\right]]
If h is not zero, the independent variable can be changed from t to Ï[16]
           d  d t    = &#x03C9;   d  d &#x03C6;    =   h  r  2       d  d
      &#x03C6;      {\displaystyle {\frac {d}{dt}}=\omega {\frac {d}{d\varphi
      }}={\frac {h}{r^{2}}}{\frac {d}{d\varphi }}}  [{\frac  {d}{dt}}=\omega
      {\frac  {d}{d\varphi }}={\frac  {h}{r^{{2}}}}{\frac  {d}{d\varphi }}]
giving the new equation of motion[17]
          &#x222B;  r   F ( r )  d r =    m  h  2    2    [    (  &#x2212;   1
      r  2        d r   d &#x03C6;     )   2   +   (   1 r   )   2    ]
      {\displaystyle \int ^{r}F(r)\,dr={\frac {mh^{2}}{2}}\left[\left(-{\frac
      {1}{r^{2}}}{\frac {dr}{d\varphi }}\right)^{2}+\left({\frac {1}
      {r}}\right)^{2}\right]}  [\int ^{{r}}F(r)\,dr={\frac  {mh^{2}}2}\left
      [\left(-{\frac  1{r^{2}}}{\frac  {dr}{d\varphi }}\right)^{2}+\left({\frac
      1r}\right)^{2}\right]]
Making the change of variables to the inverse radius u = 1/r[17] yields
           (    d u   d &#x03C6;    )   2   = C &#x2212;  u  2
      &#x2212; G  ( u )    {\displaystyle \left({\frac {du}{d\varphi    (1)
      }}\right)^{2}=C-u^{2}-G\left(u\right)}  [\left({\frac  {du}       
      {d\varphi }}\right)^{{2}}=C-u^{2}-G\left(u\right)]
where C is a constant of integration and the function G(u) is defined by
         G ( u ) = &#x2212;   2  m  h  2       &#x222B;   1 u    F ( r )  d r
      {\displaystyle G(u)=-{\frac {2}{mh^{2}}}\int ^{\frac {1}{u}}F(r)\,dr}  [G
      (u)=-{\frac  2{mh^{{2}}}}\int ^{{{\frac  1u}}}F(r)\,dr]
This equation becomes quasilinear on differentiating by Ï
             d  2   u   d  &#x03C6;  2      + u = &#x2212;   1  m  h  2    u  2
      F ( 1  /  u )   {\displaystyle {\frac {d^{2}u}{d\varphi ^{2}}}+u=-{\frac
      {1}{mh^{2}u^{2}}}F(1/u)}  [{\frac  {d^{{2}}u}{d\varphi ^{{2}}}}+u=-{\frac
      {1}{mh^{{2}}u^{{2}}}}F(1/u)]
This is known as the Binet_equation. Integrating (1) yields the solution for Ï
[18]
         &#x03C6; =  &#x03C6;  0   +  &#x222B;   1 r       d u   C &#x2212;  u
      2   &#x2212; G ( u )      {\displaystyle \varphi =\varphi _{0}+\int ^
      {\frac {1}{r}}{\frac {du}{\sqrt {C-u^{2}-G(u)}}}}  [\varphi =\varphi _{
      {0}}+\int ^{{{\frac  1r}}}{\frac  {du}{{\sqrt  {C-u^{{2}}-G(u)}}}}]
where Ï0 is another constant of integration. A central-force problem is said
to be "integrable" if this final integration can be solved in terms of known
functions.
**** Orbit of the particle[edit] ****
The total energy of the system Etot equals the sum of the potential energy and
the kinetic energy[19]
          E   t o t    =   1 2   m     r &#x02D9;     2   +   1 2   m  r  2
      &#x03C6; &#x02D9;     2   + U ( r ) =   1 2   m     r &#x02D9;     2   +
      m  h  2     2  r  2      + U ( r )   {\displaystyle E_{\mathrm {tot} }=
      {\frac {1}{2}}m{\dot {r}}^{2}+{\frac {1}{2}}mr^{2}{\dot {\varphi }}^{2}+U
      (r)={\frac {1}{2}}m{\dot {r}}^{2}+{\frac {mh^{2}}{2r^{2}}}+U(r)}  [E_{{
      {\mathrm  {tot}}}}={\frac  {1}{2}}m{\dot  {r}}^{{2}}+{\frac  {1}{2}}mr^{
      {2}}{\dot  {\varphi }}^{{2}}+U(r)={\frac  {1}{2}}m{\dot  {r}}^{{2}}+
      {\frac  {mh^{{2}}}{2r^{{2}}}}+U(r)]
Since the total energy is constant, the rate of change of r can be calculated
[20]
            r &#x02D9;    =    d r   d t    =    2 m       E   t o t
      &#x2212; U ( r ) &#x2212;    m  h  2     2  r  2          {\displaystyle
      {\dot {r}}={\frac {dr}{dt}}={\sqrt {\frac {2}{m}}}{\sqrt {E_{\mathrm
      {tot} }-U(r)-{\frac {mh^{2}}{2r^{2}}}}}}  [{\dot  {r}}={\frac  {dr}{dt}}=
      {\sqrt  {{\frac  {2}{m}}}}{\sqrt  {E_{{{\mathrm  {tot}}}}-U(r)-{\frac
      {mh^{{2}}}{2r^{{2}}}}}}]
which may be converted (as before) to the derivative of r with respect to the
azimuthal angle Ï[17]
            d r   d &#x03C6;    =    r  2   h      d r   d t
      {\displaystyle {\frac {dr}{d\varphi }}={\frac {r^{2}}{h}}{\frac {dr}
      {dt}}}  [{\frac  {dr}{d\varphi }}={\frac  {r^{{2}}}{h}}{\frac  {dr}{dt}}]
Integrating and using the angular-momentum formula L=mh yields the formula[21]
         &#x03C6; =  &#x03C6;  0   +   L  2 m     &#x222B;  r      d r    r  2
      E   t o t    &#x2212; U ( r ) &#x2212;    L  2    2 m  r  2
      {\displaystyle \varphi =\varphi _{0}+{\frac {L}{\sqrt {2m}}}\int ^{r}
      {\frac {dr}{r^{2}{\sqrt {E_{\mathrm {tot} }-U(r)-{\frac {L^{2}}{2mr^
      {2}}}}}}}}  [\varphi =\varphi _{{0}}+{\frac  {L}{{\sqrt  {2m}}}}\int ^{
      {r}}{\frac  {dr}{r^{{2}}{\sqrt  {E_{{{\mathrm  {tot}}}}-U(r)-{\frac  {L^{
      {2}}}{2mr^{{2}}}}}}}}]
which indicates that the angular momentum contributes an effective potential
energy[22]
          U   e f f    = U ( r ) +    L  2    2 m  r  2        {\displaystyle
      U_{\mathrm {eff} }=U(r)+{\frac {L^{2}}{2mr^{2}}}}  [U_{{{\mathrm
      {eff}}}}=U(r)+{\frac  {L^{{2}}}{2mr^{{2}}}}]
Changing the variable of integration to the inverse radius yields the integral
[23]
         &#x03C6; =  &#x03C6;  0   +  &#x222B;  u      d u      2 m   L  2
      E   t o t    &#x2212;    2 m   L  2     U ( 1  /  u ) &#x2212;  u  2
      {\displaystyle \varphi =\varphi _{0}+\int ^{u}{\frac {du}{\sqrt {{\frac
      {2m}{L^{2}}}E_{\mathrm {tot} }-{\frac {2m}{L^{2}}}U(1/u)-u^{2}}}}}
      [\varphi =\varphi _{{0}}+\int ^{{u}}{\frac  {du}{{\sqrt  {{\frac  {2m}{L^
      {{2}}}}E_{{{\mathrm  {tot}}}}-{\frac  {2m}{L^{{2}}}}U(1/u)-u^{{2}}}}}}]
which expresses the above constants C = 2mEtot/L2 and G(u) = 2mU(1/u)/L2 above
in terms of the total energy Etot and the potential energy U(r).
**** Turning points and closed orbits[edit] ****
Main article: Bertrand's_theorem
The rate of change of r is zero whenever the effective potential energy equals
the total energy[24]
          E   t o t    = U ( r ) +    L  2    2 m  r  2        {\displaystyle
      E_{\mathrm {tot} }=U(r)+{\frac {L^{2}}{2mr^{2}}}}  [E_{{{\mathrm
      {tot}}}}=U(r)+{\frac  {L^{{2}}}{2mr^{{2}}}}]
The points where this equation is satisfied are known as turning points.[24]
The orbit on either side of a turning point is symmetrical; in other words, if
the azimuthal angle is defined such that Ï = 0 at the turning point, then the
orbit is the same in opposite directions, r(Ï) = r(−Ï).[25]
If there are two turning points such that the radius r is bounded between rmin
and rmax, then the motion is contained within an annulus of those radii.[24] As
the radius varies from the one turning point to the other, the change in
azimuthal angle Ï equals[24]
         &#x0394; &#x03C6; =   L  2 m     &#x222B;   r   m i n       r   m a x
      d r    r  2     E &#x2212; U ( r ) &#x2212;    L  2    2 m  r  2
      {\displaystyle \Delta \varphi ={\frac {L}{\sqrt {2m}}}\int _{r_{\mathrm
      {min} }}^{r_{\mathrm {max} }}{\frac {dr}{r^{2}{\sqrt {E-U(r)-{\frac {L^
      {2}}{2mr^{2}}}}}}}}  [\Delta \varphi ={\frac  {L}{{\sqrt  {2m}}}}\int _{
      {r_{{{\mathrm  {min}}}}}}^{{r_{{{\mathrm  {max}}}}}}{\frac  {dr}{r^{{2}}
      {\sqrt  {E-U(r)-{\frac  {L^{{2}}}{2mr^{{2}}}}}}}}]
The orbit will close upon itself[note_8] provided that ÎÏ equals a rational
fraction of 2Ï, i.e.,[24]
         &#x0394; &#x03C6; = 2 &#x03C0;   m n     {\displaystyle \Delta \varphi
      =2\pi {\frac {m}{n}}}  [\Delta \varphi =2\pi {\frac  {m}{n}}]
where m and n are integers. In that case, the radius oscillates exactly m times
while the azimuthal angle Ï makes exactly n revolutions. In general, however,
ÎÏ/2Ï will not be such a rational_number, and thus the orbit will not be
closed. In that case, the particle will eventually pass arbitrarily close to
every point within the annulus. Two types of central force always produce
closed orbits: F(r) = Î±r (a linear force) and F(r) = Î±/r2 (an inverse-square
law). As shown by Bertrand, these two central forces are the only ones that
guarantee closed orbits.[26]
In general, if the angular momentum L is nonzero, the L2/2mr2 term prevents the
particle from falling into the origin, unless the effective potential energy
goes to negative infinity in the limit of r going to zero.[27] Therefore, if
there is a single turning point, the orbit generally goes to infinity; the
turning point corresponds to a point of minimum radius.
***** Specific solutions[edit] *****
**** Kepler problem[edit] ****
[An_animation_showing_a_small_particle_moving_on_a_red_ellipse;_a_large_blue
mass_is_located_at_one_focus_of_the_ellipse.]
Classical gravity is a central force. Solving that central-force problem shows
that a bound particle follows an elliptical orbit in which equal areas are
swept out in equal times, as described by Kepler's_second_law.
See also: Kepler_problem and LaplaceâRungeâLenz_vector
In classical_physics, many important forces follow an inverse-square law, such
as gravity or electrostatics. The general mathematical form of such inverse-
square central forces is
         F =   &#x03B1;  r  2     = &#x03B1;  u  2     {\displaystyle F={\frac
      {\alpha }{r^{2}}}=\alpha u^{2}}  [F={\frac  {\alpha }{r^{{2}}}}=\alpha u^
      {{2}}]
for a constant     &#x03B1;   {\displaystyle \alpha }  [\alpha ], which is
negative for an attractive force and positive for a repulsive one.
This special case of the classical central-force problem is called the Kepler
problem. For an inverse-square force, the Binet equation derived above is
linear
             d  2   u   d  &#x03C6;  2      + u = &#x2212;   &#x03B1;  m  h  2
      .   {\displaystyle {\frac {d^{2}u}{d\varphi ^{2}}}+u=-{\frac {\alpha }
      {mh^{2}}}.}  [{\frac  {d^{{2}}u}{d\varphi ^{{2}}}}+u=-{\frac  {\alpha }
      {mh^{{2}}}}.]
The solution of this equation is
         u ( &#x03C6; ) = &#x2212;   &#x03B1;  m  h  2       [  1 + e cos
      &#x2061;  (  &#x03C6; &#x2212;  &#x03C6;  0    )   ]    {\displaystyle u
      (\varphi )=-{\frac {\alpha }{mh^{2}}}\left[1+e\cos \left(\varphi -\varphi
      _{0}\right)\right]}  [{\displaystyle u(\varphi )=-{\frac {\alpha }{mh^
      {2}}}\left[1+e\cos \left(\varphi -\varphi _{0}\right)\right]}]
which shows that the orbit is a conic_section of eccentricity e; here, Ï0 is
the initial angle, and the center of force is at the focus of the conic
section. Using the half-angle_formula_for_sine, this solution can also be
written as
         u ( &#x03C6; ) =  u  1   + (  u  2   &#x2212;  u  1   )  sin  2
      &#x2061;  (    &#x03C6; &#x2212;  &#x03C6;  0    2   )    {\displaystyle
      u(\varphi )=u_{1}+(u_{2}-u_{1})\sin ^{2}\left({\frac {\varphi -\varphi _
      {0}}{2}}\right)}  [u(\varphi )=u_{{1}}+(u_{{2}}-u_{{1}})\sin ^{{2}}\left(
      {\frac  {\varphi -\varphi _{{0}}}{2}}\right)]
[Blue_ellipse_with_the_two_foci_indicated_as_black_points._Four_line_segments
go_out_from_the_left_focus_to_the_ellipse,_forming_two_shaded_pseudo-triangles
with_two_straight_sides_and_the_third_side_made_from_the_curved_segment_of_the
intervening_ellipse.]
As for all central forces, the particle in the Kepler problem sweeps out equal
areas in equal times, as illustrated by the two blue elliptical sectors. The
center of force is located at one of the foci of the elliptical orbit.
where u1 and u2 are constants, with u2 larger than u1. The two versions of the
solution are related by the equations
          u  1   +  u  2   =    &#x2212; 2 &#x03B1;   m  h  2
      {\displaystyle u_{1}+u_{2}={\frac {-2\alpha }{mh^{2}}}}  [u_{{1}}+u_{
      {2}}={\frac  {-2\alpha }{mh^{{2}}}}]
and
         e =     u  2   &#x2212;  u  1      u  2   +  u  1
      {\displaystyle e={\frac {u_{2}-u_{1}}{u_{2}+u_{1}}}}  [e={\frac  {u_{
      {2}}-u_{{1}}}{u_{{2}}+u_{{1}}}}]
Since the sin2 function is always greater than zero, u2 is the largest possible
value of u and the inverse of the smallest possible value of r, i.e., the
distance of closest approach (periapsis). Since the radial distance r cannot be
a negative number, neither can its inverse u; therefore, u2 must be a positive
number. If u1 is also positive, it is the smallest possible value of u, which
corresponds to the largest possible value of r, the distance of furthest
approach (apoapsis). If u1 is zero or negative, then the smallest possible
value of u is zero (the orbit goes to infinity); in this case, the only
relevant values of Ï are those that make u positive.
For an attractive force (Î± < 0), the orbit is an ellipse, a hyperbola or
parabola, depending on whether u1 is positive, negative, or zero, respectively;
this corresponds to an eccentricity e less than one, greater than one, or equal
to one. For a repulsive force (Î± > 0), u1 must be negative, since u2 is
positive by definition and their sum is negative; hence, the orbit is a
hyperbola. Naturally, if no force is present (Î±=0), the orbit is a straight
line.
**** Central forces with exact solutions[edit] ****
See also: Exact_solutions_of_classical_central-force_problems
The Binet equation for u(Ï) can be solved numerically for nearly any central
force F(1/u). However, only a handful of forces result in formulae for u in
terms of known functions. As derived above, the solution for Ï can be
expressed as an integral over u
         &#x03C6; =  &#x03C6;  0   +   L  2 m     &#x222B;  u      d u    E   t
      o t    &#x2212; U ( 1  /  u ) &#x2212;     L  2    u  2     2 m
      {\displaystyle \varphi =\varphi _{0}+{\frac {L}{\sqrt {2m}}}\int ^{u}
      {\frac {du}{\sqrt {E_{\mathrm {tot} }-U(1/u)-{\frac {L^{2}u^{2}}{2m}}}}}}
      [\varphi =\varphi _{{0}}+{\frac  {L}{{\sqrt  {2m}}}}\int ^{{u}}{\frac
      {du}{{\sqrt  {E_{{{\mathrm  {tot}}}}-U(1/u)-{\frac  {L^{{2}}u^{{2}}}
      {2m}}}}}}]
A central-force problem is said to be "integrable" if this integration can be
solved in terms of known functions.
If the force is a power law, i.e., if F(r) = Î± rn, then u can be expressed in
terms of circular_functions and/or elliptic_functions if n equals 1, -2, -3
(circular functions) and -7, -5, -4, 0, 3, 5, -3/2, -5/2, -1/3, -5/3 and -7/3
(elliptic functions).[28] Similarly, only six possible linear combinations of
power laws give solutions in terms of circular and elliptic functions[29][30]
         F ( r ) = A  r  &#x2212; 3   + B r + C  r  3   + D  r  5
      {\displaystyle F(r)=Ar^{-3}+Br+Cr^{3}+Dr^{5}}  [F(r)=Ar^{{-3}}+Br+Cr^{
      {3}}+Dr^{{5}}]
         F ( r ) = A  r  &#x2212; 3   + B r + C  r  &#x2212; 5   + D  r
      &#x2212; 7     {\displaystyle F(r)=Ar^{-3}+Br+Cr^{-5}+Dr^{-7}}  [F(r)=Ar^
      {{-3}}+Br+Cr^{{-5}}+Dr^{{-7}}]
         F ( r ) = A  r  &#x2212; 3   + B  r  &#x2212; 2   + C r + D
      {\displaystyle F(r)=Ar^{-3}+Br^{-2}+Cr+D}  [F(r)=Ar^{{-3}}+Br^{{-
      2}}+Cr+D]
         F ( r ) = A  r  &#x2212; 3   + B  r  &#x2212; 2   + C  r  &#x2212; 4
      + D  r  &#x2212; 5     {\displaystyle F(r)=Ar^{-3}+Br^{-2}+Cr^{-4}+Dr^{-
      5}}  [F(r)=Ar^{{-3}}+Br^{{-2}}+Cr^{{-4}}+Dr^{{-5}}]
         F ( r ) = A  r  &#x2212; 3   + B  r  &#x2212; 2   + C  r  &#x2212; 3
      /  2   + D  r  &#x2212; 5  /  2     {\displaystyle F(r)=Ar^{-3}+Br^{-
      2}+Cr^{-3/2}+Dr^{-5/2}}  [F(r)=Ar^{{-3}}+Br^{{-2}}+Cr^{{-3/2}}+Dr^{{-5/
      2}}]
         F ( r ) = A  r  &#x2212; 3   + B  r  &#x2212; 1  /  3   + C  r
      &#x2212; 5  /  3   + D  r  &#x2212; 7  /  3     {\displaystyle F(r)=Ar^{-
      3}+Br^{-1/3}+Cr^{-5/3}+Dr^{-7/3}}  [F(r)=Ar^{{-3}}+Br^{{-1/3}}+Cr^{{-5/
      3}}+Dr^{{-7/3}}]
The following special cases of the first two force types always result in
circular functions.
         F ( r ) = A  r  &#x2212; 3   + B r   {\displaystyle F(r)=Ar^{-3}+Br}
      [F(r)=Ar^{{-3}}+Br]
         F ( r ) = A  r  &#x2212; 3   + B  r  &#x2212; 2     {\displaystyle F
      (r)=Ar^{-3}+Br^{-2}}  [F(r)=Ar^{{-3}}+Br^{{-2}}]
The special case
         F ( r ) = A  r  &#x2212; 5     {\displaystyle F(r)=Ar^{-5}}  [F(r)=Ar^
      {{-5}}]
was mentioned by Newton, in corollary 1 to proposition VII of the principia, as
the force implied by circular orbits passing through the point of attraction.
**** Newton's theorem of revolving orbits[edit] ****
[File:Newton revolving orbit e0.6 3rd subharmonic.ogv]Play_media
Illustration of Newton's theorem of revolving orbits. The green planet
completes one (subharmonic) orbit for every three orbits of the blue planet
(k=1/3). A GIF version of this animation is found here.
Main article: Newton's_theorem_of_revolving_orbits
The term r−3 occurs in all the force laws above, indicating that the addition
of the inverse-cube force does not influence the solubility of the problem in
terms of known functions. Newton showed that, with adjustments in the initial
conditions, the addition of such a force does not affect the radial motion of
the particle, but multiplies its angular motion by a constant factor k. An
extension of Newton's theorem was discovered in 2000 by Mahomed and Vawda.[30]
Assume that a particle is moving under an arbitrary central force F1(r), and
let its radius r and azimuthal angle Ï be denoted as r(t) and Ï1(t) as a
function of time t. Now consider a second particle with the same mass m that
shares the same radial motion r(t), but one whose angular speed is k times
faster than that of the first particle. In other words, the azimuthal_angles of
the two particles are related by the equation Ï2(t) = k Ï1(t). Newton showed
that the force acting on the second particle equals the force F1(r) acting on
the first particle, plus an inverse-cube central force[31]
          F  2   ( r ) =  F  1   ( r ) +    L  1   2    m  r  3       (  1
      &#x2212;  k  2    )    {\displaystyle F_{2}(r)=F_{1}(r)+{\frac {L_{1}^
      {2}}{mr^{3}}}\left(1-k^{2}\right)}  [F_{{2}}(r)=F_{{1}}(r)+{\frac  {L_{
      {1}}^{{2}}}{mr^{{3}}}}\left(1-k^{{2}}\right)]
where L1 is the magnitude of the first particle's angular_momentum.
If k2 is greater than one, F2âF1 is a negative number; thus, the added
inverse-cube force is attractive. Conversely, if k2 is less than one, F2âF1
is a positive number; the added inverse-cube force is repulsive. If k is an
integer such as 3, the orbit of the second particle is said to be a harmonic of
the first particle's orbit; by contrast, if k is the inverse of an integer,
such as â, the second orbit is said to be a subharmonic of the first orbit.
***** Historical development[edit] *****
Figure 10: Newton's geometrical proof that a moving particle sweeps out equal
areas in equal times if and only if the force acting on it at the point B is a
central force. Here, the triangle OAB has the same area as the triangles OBC
and OBK.
**** Newton's derivation[edit] ****
The classical central-force problem was solved geometrically by Isaac_Newton in
his PhilosophiÃ¦_Naturalis_Principia_Mathematica, in which Newton introduced
his laws_of_motion. Newton used an equivalent of leapfrog_integration to
convert the continuous motion to a discrete one, so that geometrical methods
may be applied. In this approach, the position of the particle is considered
only at evenly spaced time points. For illustration, the particle in Figure 10
is located at point A at time t = 0, at point B at time t = Ît, at point C at
time t = 2Ît, and so on for all times t = nÎt, where n is an integer. The
velocity is assumed to be constant between these time points. Thus, the vector
rAB = rB − rA equals Ît times the velocity vector vAB (red line), whereas
rBC = rC − rB equals vBCÎt (blue line). Since the velocity is constant between
points, the force is assumed to act instantaneously at each new position; for
example, the force acting on the particle at point B instantly changes the
velocity from vAB to vBC. The difference vector Îr = rBC − rAB equals ÎvÎt
(green line), where Îv = vBC − vAB is the change in velocity resulting from
the force at point B. Since the acceleration a is parallel to Îv and since
F = ma, the force F must be parallel to Îv and Îr. If F is a central force,
it must be parallel to the vector rB from the center O to the point B (dashed
green line); in that case, Îr is also parallel to rB.
If no force acts at point B, the velocity is unchanged, and the particle
arrives at point K at time t = 2Ît. The areas of the triangles OAB and OBK are
equal, because they share the same base (rAB) and height (râ¥). If Îr is
parallel to rB, the triangles OBK and OBC are likewise equal, because they
share the same base (rB) and the height is unchanged. In that case, the areas
of the triangles OAB and OBC are the same, and the particle sweeps out equal
areas in equal time. Conversely, if the areas of all such triangles are equal,
then Îr must be parallel to rB, from which it follows that F is a central
force. Thus, a particle sweeps out equal areas in equal times if and only if F
is a central force.
***** Alternative derivations of the equations of motion[edit] *****
**** Lagrangian mechanics[edit] ****
The formula for the radial force may also be obtained using Lagrangian
mechanics. In polar coordinates, the Lagrangian L of a single particle in a
potential energy field U(r) is given by
         L =   1 2   m     r &#x02D9;     2   +   1 2   m  r  2       &#x03C6;
      &#x02D9;     2   &#x2212; U ( r )   {\displaystyle L={\frac {1}{2}}m{\dot
      {r}}^{2}+{\frac {1}{2}}mr^{2}{\dot {\varphi }}^{2}-U(r)}  [L={\frac  {1}
      {2}}m{\dot  {r}}^{{2}}+{\frac  {1}{2}}mr^{{2}}{\dot  {\varphi }}^{{2}}-U
      (r)]
Then Lagrange's equations of motion
           d  d t     (    &#x2202; L   &#x2202;    r &#x02D9;       )  =
      &#x2202; L   &#x2202; r      {\displaystyle {\frac {d}{dt}}\left({\frac
      {\partial L}{\partial {\dot {r}}}}\right)={\frac {\partial L}{\partial
      r}}}  [{\frac  {d}{dt}}\left({\frac  {\partial L}{\partial {\dot
      {r}}}}\right)={\frac  {\partial L}{\partial r}}]
take the form
         m    r &#x00A8;    = m r     &#x03C6; &#x02D9;     2   &#x2212;    d U
      d r    =    m  h  2     r  3     + F ( r )   {\displaystyle m{\ddot
      {r}}=mr{\dot {\varphi }}^{2}-{\frac {dU}{dr}}={\frac {mh^{2}}{r^{3}}}+F
      (r)}  [m{\ddot  {r}}=mr{\dot  {\varphi }}^{{2}}-{\frac  {dU}{dr}}={\frac
      {mh^{{2}}}{r^{{3}}}}+F(r)]
since the magnitude F(r) of the radial force equals the negative derivative of
the potential energy U(r) in the radial direction.
**** Hamiltonian mechanics[edit] ****
The radial force formula may also be derived using Hamiltonian_mechanics. In
polar coordinates, the Hamiltonian can be written as
         H =   1  2 m     (   p  r   2   +    p  &#x03C6;   2    r  2      )  +
      U ( r )   {\displaystyle H={\frac {1}{2m}}\left(p_{r}^{2}+{\frac {p_
      {\varphi }^{2}}{r^{2}}}\right)+U(r)}  [{\displaystyle H={\frac {1}
      {2m}}\left(p_{r}^{2}+{\frac {p_{\varphi }^{2}}{r^{2}}}\right)+U(r)}]
Since the azimuthal angle Ï does not appear in the Hamiltonian, its conjugate
momentum pÏ is a constant of the motion. This conjugate momentum is the
magnitude L of the angular momentum, as shown by the Hamiltonian equation of
motion for Ï
            d &#x03C6;   d t    =    &#x2202; H   &#x2202;  p  &#x03C6;      =
      p  &#x03C6;    m  r  2      =   L  m  r  2        {\displaystyle {\frac
      {d\varphi }{dt}}={\frac {\partial H}{\partial p_{\varphi }}}={\frac {p_
      {\varphi }}{mr^{2}}}={\frac {L}{mr^{2}}}}  [{\frac  {d\varphi }{dt}}=
      {\frac  {\partial H}{\partial p_{{\varphi }}}}={\frac  {p_{{\varphi }}}
      {mr^{{2}}}}={\frac  {L}{mr^{{2}}}}]
The corresponding equation of motion for r is
            d r   d t    =    &#x2202; H   &#x2202;  p  r      =    p  r   m
      {\displaystyle {\frac {dr}{dt}}={\frac {\partial H}{\partial p_{r}}}=
      {\frac {p_{r}}{m}}}  [{\frac  {dr}{dt}}={\frac  {\partial H}{\partial p_{
      {r}}}}={\frac  {p_{{r}}}{m}}]
Taking the second derivative of r with respect to time and using Hamilton's
equation of motion for pr yields the radial-force equation
             d  2   r   d  t  2      =   1 m      d  p  r     d t    = &#x2212;
      1 m    (    &#x2202; H   &#x2202; r    )  =    p  &#x03C6;   2     m  2
      r  3      &#x2212;   1 m      d U   d r    =    L  2     m  2    r  3
      +   1 m   F ( r )   {\displaystyle {\frac {d^{2}r}{dt^{2}}}={\frac {1}
      {m}}{\frac {dp_{r}}{dt}}=-{\frac {1}{m}}\left({\frac {\partial H}
      {\partial r}}\right)={\frac {p_{\varphi }^{2}}{m^{2}r^{3}}}-{\frac {1}
      {m}}{\frac {dU}{dr}}={\frac {L^{2}}{m^{2}r^{3}}}+{\frac {1}{m}}F(r)}  [
      {\frac  {d^{{2}}r}{dt^{{2}}}}={\frac  {1}{m}}{\frac  {dp_{{r}}}{dt}}=-
      {\frac  {1}{m}}\left({\frac  {\partial H}{\partial r}}\right)={\frac  {p_
      {{\varphi }}^{{2}}}{m^{{2}}r^{{3}}}}-{\frac  {1}{m}}{\frac  {dU}{dr}}=
      {\frac  {L^{{2}}}{m^{{2}}r^{{3}}}}+{\frac  {1}{m}}F(r)]
**** Hamilton-Jacobi equation[edit] ****
The orbital equation can be derived directly from the HamiltonâJacobi
equation.[32] Adopting the radial distance r and the azimuthal angle Ï as the
coordinates, the Hamilton-Jacobi equation for a central-force problem can be
written
           1  2 m      (    d  S  r     d r    )   2   +   1  2 m  r  2
      (    d  S  &#x03C6;     d &#x03C6;    )   2   + U ( r ) =  E   t o t
      {\displaystyle {\frac {1}{2m}}\left({\frac {dS_{r}}{dr}}\right)^{2}+
      {\frac {1}{2mr^{2}}}\left({\frac {dS_{\varphi }}{d\varphi }}\right)^{2}+U
      (r)=E_{\mathrm {tot} }}  [{\frac  {1}{2m}}\left({\frac  {dS_{{r}}}
      {dr}}\right)^{{2}}+{\frac  {1}{2mr^{{2}}}}\left({\frac  {dS_{{\varphi }}}
      {d\varphi }}\right)^{{2}}+U(r)=E_{{{\mathrm  {tot}}}}]
where S = SÏ(Ï) + Sr(r) - Etott is Hamilton's_principal_function, and Etot
and t represent the total energy and time, respectively. This equation may be
solved by successive integrations of ordinary_differential_equations, beginning
with the Ï equation
            d  S  &#x03C6;     d &#x03C6;    =  p  &#x03C6;   = L
      {\displaystyle {\frac {dS_{\varphi }}{d\varphi }}=p_{\varphi }=L}  [
      {\frac  {dS_{{\varphi }}}{d\varphi }}=p_{{\varphi }}=L]
where pÏ is a constant_of_the_motion equal to the magnitude of the angular
momentum L. Thus, SÏ(Ï) = LÏ and the HamiltonâJacobi equation becomes
           1  2 m      (    d  S  r     d r    )   2   +    L  2    2 m  r  2
      + U ( r ) =  E   t o t      {\displaystyle {\frac {1}{2m}}\left({\frac
      {dS_{r}}{dr}}\right)^{2}+{\frac {L^{2}}{2mr^{2}}}+U(r)=E_{\mathrm {tot}
      }}  [{\frac  {1}{2m}}\left({\frac  {dS_{{r}}}{dr}}\right)^{{2}}+{\frac
      {L^{{2}}}{2mr^{{2}}}}+U(r)=E_{{{\mathrm  {tot}}}}]
Integrating this equation for Sr yields
          S  r   ( r ) =   2 m   &#x222B; d r    E   t o t    &#x2212; U ( r )
      &#x2212;    L  2    2 m  r  2          {\displaystyle S_{r}(r)={\sqrt
      {2m}}\int dr{\sqrt {E_{\mathrm {tot} }-U(r)-{\frac {L^{2}}{2mr^{2}}}}}}
      [S_{{r}}(r)={\sqrt  {2m}}\int dr{\sqrt  {E_{{{\mathrm  {tot}}}}-U(r)-
      {\frac  {L^{{2}}}{2mr^{{2}}}}}}]
Taking the derivative of S with respect to L yields the orbital equation
derived above
          &#x03C6;  0   =    &#x2202; S   &#x2202; L    =    &#x2202;  S
      &#x03C6;     &#x2202; L    +    &#x2202;  S  r     &#x2202; L    =
      &#x03C6; &#x2212;   L  2 m     &#x222B;  r      d r    r  2      E   t o
      t    &#x2212; U ( r ) &#x2212;    L  2    2 m  r  2
      {\displaystyle \varphi _{0}={\frac {\partial S}{\partial L}}={\frac
      {\partial S_{\varphi }}{\partial L}}+{\frac {\partial S_{r}}{\partial
      L}}=\varphi -{\frac {L}{\sqrt {2m}}}\int ^{r}{\frac {dr}{r^{2}{\sqrt {E_
      {\mathrm {tot} }-U(r)-{\frac {L^{2}}{2mr^{2}}}}}}}}  [\varphi _{{0}}=
      {\frac  {\partial S}{\partial L}}={\frac  {\partial S_{{\varphi }}}
      {\partial L}}+{\frac  {\partial S_{{r}}}{\partial L}}=\varphi -{\frac
      {L}{{\sqrt  {2m}}}}\int ^{{r}}{\frac  {dr}{r^{{2}}{\sqrt  {E_{{{\mathrm
      {tot}}}}-U(r)-{\frac  {L^{{2}}}{2mr^{{2}}}}}}}}]
***** See also[edit] *****
    * Schwarzschild_geodesics, for a central-force problem in general
      relativity
    * Particle_in_a_spherically_symmetric_potential, the quantum-mechanical
      analog of the central-force problem
    * Hydrogen-like_atom, the Kepler problem in quantum_mechanics
    * Inverse_square_potential
***** Notes[edit] *****
   1. ^ Throughout this article, boldface type is used to indicate that
      quantities such as r and F are vectors, whereas ordinary numbers are
      written in italics. Briefly, a vector v is a quantity that has a
      magnitude v (also written |v|) and a direction. Vectors are often
      specified by their components. For example, the position_vector r = (x,
      y) in Cartesian_coordinates is described as an ordered pair of its x and
      y coordinates.
   2. ^ In this article, Newton's_notation for derivatives ("dot notation") is
      used sometimes to make the formulae easier to read; it has no other
      significance. In this notation, a single dot over a variable signifies
      its first derivative with respect to time, e.g.,
                  r &#x02D9;    =    d r   d t      {\displaystyle {\dot {r}}=
            {\frac {dr}{dt}}}  [{\dot  {r}}={\frac  {dr}{dt}}]
      Similarly, a double dot over a variable signifies its second derivative
      with respect for time, e.g.,
                  r &#x00A8;    =     d  2   r   d  t  2        {\displaystyle
            {\ddot {r}}={\frac {d^{2}r}{dt^{2}}}}  [{\ddot  {r}}={\frac  {d^{
            {2}}r}{dt^{{2}}}}]
   3. ^ Here, the times symbol × indicates the vector_cross_product, not simple
      multiplication.
   4. ^ If a and b are three-dimensional vectors, their vector cross product c
      = a × b is always perpendicular to the plane defined by a and b.
   5. ^ This formula for the azimuthal unit vector may be verified by
      calculation; its magnitude equals one
                  &#x03C6; &#x005E;    &#x22C5;    &#x03C6; &#x005E;    =
            ( &#x2212; sin &#x2061; &#x03C6;  )  2   + ( cos &#x2061; &#x03C6;
            )  2   = 1   {\displaystyle {\hat {\boldsymbol {\varphi }}}\cdot
            {\hat {\boldsymbol {\varphi }}}=(-\sin \varphi )^{2}+(\cos \varphi
            )^{2}=1}  [{\hat  {{\boldsymbol  \varphi }}}\cdot {\hat  {
            {\boldsymbol  \varphi }}}=(-\sin \varphi )^{{2}}+(\cos \varphi )^{
            {2}}=1]
      and its dot-product with r equals zero
                  &#x03C6; &#x005E;    &#x22C5;    r &#x005E;    = &#x2212; sin
            &#x2061; &#x03C6; cos &#x2061; &#x03C6; + cos &#x2061; &#x03C6; sin
            &#x2061; &#x03C6; = 0   {\displaystyle {\hat {\boldsymbol {\varphi
            }}}\cdot \mathbf {\hat {r}} =-\sin \varphi \cos \varphi +\cos
            \varphi \sin \varphi =0}  [{\hat  {{\boldsymbol  \varphi }}}\cdot
            {\mathbf  {{\hat  {r}}}}=-\sin \varphi \cos \varphi +\cos \varphi
            \sin \varphi =0]
      Therefore, it is a unit vector perpendicular to the radial vector r.
   6. ^ The area of a triangle equals one half the base times its height. In
      this case, the base is given by vΔt and the height equals the impact
      parameter r⊥.
   7. ^ A parallel-force problem is one in which the force is exactly zero
      along one direction.
   8. ^ A closed orbit is one that returns to its starting position after a
      finite time with exactly the same velocity. Hence, it executes exactly
      the same motion over and over again.
***** References[edit] *****
   1. ^ Goldstein, p. 71; Landau and Lifshitz, p. 30; Sommerfeld, p. 39; Symon,
      p. 121.
   2. ^ Landau and Lifshitz, p. 30; Symon, p. 121.
   3. ^ Goldstein, p. 4; Landau and Lifshitz, p. 30; Symon, p. 122.
   4. ^ Goldstein, p. 71; Landau and Lifshitz, p. 30; Whittaker, p. 77.
   5. ^ Sommerfeld, p. 39; Symon, p. 123.
   6. ^ Goldstein, pp. 70–71; Landau and Lifshitz, p. 29; Symon, pp. 182–185;
      Whittaker, pp. 76–77.
   7. ^ Goldstein, p. 72; Landau and Lifshitz, p. 30; Whittaker, p. 77.
   8. ^ Goldstein, pp. 2–3, 6–7.
   9. ^ a b Goldstein, p. 72.
  10. ^ Goldstein, p. 73; Landau and Lifshitz, pp. 30–31; Sommerfeld, pp.
      39–40; Symon, pp. 124, 127.
  11. ^ Landau and Lifshitz, p. 31.
  12. ^ Goldstein, p. 73; Landau and Lifshitz, pp. 30–31; Sommerfeld, pp. 36,
      39; Symon, pp. 127–128.
  13. ^ Goldstein, p. 73; Landau and Lifshitz, p. 31; Sommerfeld, p. 39; Symon,
      p. 135.
  14. ^ Whittaker, pp. 93–94.
  15. ^ Goldstein, p. 73.
  16. ^ Goldstein, p. 75, 86.
  17. ^ a b c Goldstein, p. 86.
  18. ^ Whittaker, pp. 80â81.
  19. ^ Goldstein, p. 4.
  20. ^ Goldstein, p. 75.
  21. ^ Goldstein, p. 87.
  22. ^ Goldstein, pp. 76–82.
  23. ^ Goldstein, p. 88.
  24. ^ a b c d e Landau and Lifshitz, p. 32.
  25. ^ Landau and Lifshitz, pp. 32–33.
  26. ^ Goldstein, pp. 601–605.
  27. ^ Landau and Lifshitz, p. 33.
  28. ^ Whittaker, pp. 80–95.
  29. ^Broucke R (1980). "Notes on the central force rn". Astrophysics and
      Space Science. 72: 33â53. Bibcode:1980Ap&SS..72...33B. doi:10.1007/
      BF00642162.
  30. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
  31. ^ a bMahomed FM, Vawda F (2000). "Application of Symmetries to Central
      Force Problems". Nonlinear_Dynamics. 21: 307â315. doi:10.1023/A:
      1008317327402.
  32. ^ Newton, Principia, section IX of Book I, Propositions 43â45, pp.
      135â147.
  33. ^ Goldstein, pp. 454–457; Landau and Lifshitz, pp. 149–151; Misner,
      Thorne, and Wheeler, pp. 644–649; Sommerfeld, pp. 235–238.
***** Bibliography[edit] *****
    * Goldstein,_H. (1980). Classical_Mechanics (2nd ed.). Reading, MA:
      Addison-Wesley. ISBN 0-201-02918-9.
Landau,_L._D. and Lifshitz,_E._M. (1976). Mechanics. Course_of_Theoretical
Physics (3rd ed.). New York: Pergamon Press. ISBN 0-08-029141-4.CS1 maint:
Multiple names: authors list (link)
Misner,_C._W., Thorne,_K., and Wheeler,_J._A. (1973). Gravitation. San
Francisco: W. H. Freeman. ISBN 978-0-7167-0344-0.CS1 maint: Multiple names:
authors list (link)
Sommerfeld,_A. (1970). Mechanics. Lectures on Theoretical Physics, Volume I
(4th ed.). New York: Academic Press. ISBN 978-0-12-654670-5.
Symon KR (1971). Mechanics (3rd ed.). Reading, Massachusetts: Addison-Wesley.
ISBN 0-201-07392-7.
Whittaker,_E._T. (1937). A Treatise on the Analytical Dynamics of Particles and
Rigid Bodies, with an Introduction to the Problem of Three Bodies (4th ed.).
New York: Dover Publications. ISBN 978-0-521-35883-5.
***** External links[edit] *****
    * Two-body_Central_Force_Problems by D. E. Gary of the New_Jersey_Institute
      of_Technology
    * Motion_in_a_Central-Force_Field by A. Brizard of Saint_Michael's_College
    * Motion_under_the_Influence_of_a_Central_Force by G. W. Collins, II of
      Case_Western_Reserve_University
    * Video_lecture by W. H. G. Lewin of the Massachusetts_Institute_of
      Technology

Retrieved from "https://en.wikipedia.org/w/index.php?title=Classical_central-
force_problem&oldid=883144244"
Categories:
    * Classical_mechanics
Hidden categories:
    * CS1_maint:_Multiple_names:_authors_list
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * FranÃ§ais
Edit_links
    * This page was last edited on 13 February 2019, at 15:24 (UTC).
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
