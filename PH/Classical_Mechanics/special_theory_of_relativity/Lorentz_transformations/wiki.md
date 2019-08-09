The following text has been accessed from https://en.wikipedia.org/wiki/Lorentz_transformation at Fri Aug 9 03:07:18 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Lorentz transformation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Part of a series on
Spacetime
[GPB_circling_earth.jpg]
Special_relativity
General_relativity
Spacetime concepts
Spacetime_manifold
Equivalence_principle
Lorentz transformations
Minkowski_space
General relativity
Introduction_to_general_relativity
Mathematics_of_general_relativity
Einstein_field_equations
Classical gravity
Introduction_to_gravitation
Newton's_law_of_universal_gravitation
Relevant mathematics
Four-vector
Derivations_of_relativity
Spacetime_diagrams
Differential_geometry
Curved_spacetime
Mathematics_of_general_relativity
Spacetime_topology
    * v
    * t
    * e
In physics, the Lorentz transformations are a one-parameter family of linear
transformations from a coordinate_frame in spacetime to another frame that
moves at a constant velocity (the parameter) relative to the former. The
transformations are named after the Dutch physicist Hendrik_Lorentz. The
respective inverse transformation is then parametrized by the negative of this
velocity.
The most common form of the transformation, parametrized by the real constant
v ,   {\displaystyle v,}  [v,] representing a velocity confined to the x-
direction, is expressed as[1]
              t &#x2032;     = &#x03B3;  (  t &#x2212;    v x   c  2      )
      x &#x2032;     = &#x03B3;  (  x &#x2212; v t  )       y &#x2032;     = y
      z &#x2032;     = z       {\displaystyle {\begin{aligned}t'&=\gamma \left
      (t-{\frac {vx}{c^{2}}}\right)\\x'&=\gamma \left(x-
      vt\right)\\y'&=y\\z'&=z\end{aligned}}}  [{\displaystyle {\begin
      {aligned}t'&=\gamma \left(t-{\frac {vx}{c^{2}}}\right)\\x'&=\gamma \left
      (x-vt\right)\\y'&=y\\z'&=z\end{aligned}}}]
where (t, x, y, z) and (t′, x′, y′, z′) are the coordinates of an event in two
frames, where the primed frame is seen from the unprimed frame as moving with
speed v along the x-axis, c is the speed_of_light, and     &#x03B3; =    (   1
&#x2212;    v  2    c  2       )   &#x2212; 1      {\displaystyle \gamma
=\textstyle \left({\sqrt {1-{\frac {v^{2}}{c^{2}}}}}\right)^{-1}}  [
{\displaystyle \gamma =\textstyle \left({\sqrt {1-{\frac {v^{2}}{c^
{2}}}}}\right)^{-1}}] is the Lorentz_factor. When speed v is significantly
lower than c, the factor is negligible, but as v approaches c, there is a
significant effect. The value of v cannot exceed c, in current understanding.
Expressing the speed as     &#x03B2; =   v c   ,   {\displaystyle \beta ={\frac
{v}{c}},}  [{\displaystyle \beta ={\frac {v}{c}},}] an equivalent form of the
transformation is[2]
             c  t &#x2032;     = &#x03B3;  (  c t &#x2212; &#x03B2; x  )
      x &#x2032;     = &#x03B3;  (  x &#x2212; &#x03B2; c t  )       y &#x2032;
      = y      z &#x2032;     = z .       {\displaystyle {\begin
      {aligned}ct'&=\gamma \left(ct-\beta x\right)\\x'&=\gamma \left(x-\beta
      ct\right)\\y'&=y\\z'&=z.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}ct'&=\gamma \left(ct-\beta x\right)\\x'&=\gamma \left(x-\beta
      ct\right)\\y'&=y\\z'&=z.\end{aligned}}}]
Frames of reference can be divided into two groups: inertial (relative motion
with constant velocity) and non-inertial (accelerating, moving in curved paths,
rotational motion with constant angular_velocity, etc.). The term "Lorentz
transformations" only refers to transformations between inertial frames,
usually in the context of special relativity.
In each reference_frame, an observer can use a local coordinate system (usually
Cartesian_coordinates in this context) to measure lengths, and a clock to
measure time intervals. An event is something that happens at a point in space
at an instant of time, or more formally a point in spacetime. The
transformations connect the space and time coordinates of an event as measured
by an observer in each frame.[nb_1]
They supersede the Galilean_transformation of Newtonian_physics, which assumes
an absolute space and time (see Galilean_relativity). The Galilean
transformation is a good approximation only at relative speeds well below the
speed of light. Lorentz transformations have a number of unintuitive features
that do not appear in Galilean transformations. For example, they reflect the
fact that observers moving at different velocities may measure different
distances, elapsed_times, and even different orderings_of_events, but always
such that the speed_of_light is the same in all inertial reference frames. The
invariance of light speed is one of the postulates_of_special_relativity.
Historically, the transformations were the result of attempts by Lorentz and
others to explain how the speed of light was observed to be independent of the
reference_frame, and to understand the symmetries of the laws of
electromagnetism. The Lorentz transformation is in accordance with special
relativity, but was derived before Einstein developed special relativity.
The Lorentz transformation is a linear_transformation. It may include a
rotation of space; a rotation-free Lorentz transformation is called a Lorentz
boost. In Minkowski_space, the mathematical model of spacetime in special
relativity, the Lorentz transformations preserve the spacetime_interval between
any two events. This property is the defining property of a Lorentz
transformation. They describe only the transformations in which the spacetime
event at the origin is left fixed. They can be considered as a hyperbolic
rotation of Minkowski space. The more general set of transformations that also
includes translations is known as the PoincarÃ©_group.
⁰
***** Contents *****
    * 1_History
    * 2_Derivation_of_the_group_of_Lorentz_transformations
    * 3_Generalities
    * 4_Physical_formulation_of_Lorentz_boosts
          o 4.1_Coordinate_transformation
          o 4.2_Physical_implications
          o 4.3_Vector_transformations
          o 4.4_Transformation_of_velocities
          o 4.5_Transformation_of_other_quantities
    * 5_Mathematical_formulation
          o 5.1_Homogeneous_Lorentz_group
          o 5.2_Proper_transformations
                # 5.2.1_The_Lie_group_SO+(3,1)
                # 5.2.2_The_Lie_algebra_so(3,1)
          o 5.3_Improper_transformations
          o 5.4_Inhomogeneous_Lorentz_group
    * 6_Tensor_formulation
          o 6.1_Contravariant_vectors
          o 6.2_Covariant_vectors
          o 6.3_Tensors
                # 6.3.1_Transformation_of_the_electromagnetic_field
          o 6.4_Spinors
                # 6.4.1_Transformation_of_general_fields
    * 7_See_also
    * 8_Footnotes
    * 9_Notes
    * 10_References
          o 10.1_Websites
          o 10.2_Papers
          o 10.3_Books
    * 11_Further_reading
    * 12_External_links
***** History[edit] *****
Main article: History_of_Lorentz_transformations
Many physicistsâincluding Woldemar_Voigt, George_FitzGerald, Joseph_Larmor,
and Hendrik_Lorentz[3] himselfâhad been discussing the physics implied by
these equations since 1887.[4] Early in 1889, Oliver_Heaviside had shown from
Maxwell's_equations that the electric_field surrounding a spherical
distribution of charge should cease to have spherical_symmetry once the charge
is in motion relative to the aether. FitzGerald then conjectured that
Heaviside's distortion result might be applied to a theory of intermolecular
forces. Some months later, FitzGerald published the conjecture that bodies in
motion are being contracted, in order to explain the baffling outcome of the
1887 aether-wind experiment of Michelson_and_Morley. In 1892, Lorentz
independently presented the same idea in a more detailed manner, which was
subsequently called FitzGeraldâLorentz_contraction_hypothesis.[5] Their
explanation was widely known before 1905.[6]
Lorentz (1892â1904) and Larmor (1897â1900), who believed the luminiferous
aether hypothesis, also looked for the transformation under which Maxwell's
equations are invariant when transformed from the aether to a moving frame.
They extended the FitzGeraldâLorentz_contraction hypothesis and found out
that the time coordinate has to be modified as well ("local_time"). Henri
PoincarÃ© gave a physical interpretation to local time (to first order in v/c,
the relative velocity of the two reference frames normalized to the speed of
light) as the consequence of clock synchronization, under the assumption that
the speed of light is constant in moving frames.[7] Larmor is credited to have
been the first to understand the crucial time_dilation property inherent in his
equations.[8]
In 1905, PoincarÃ© was the first to recognize that the transformation has the
properties of a mathematical_group, and named it after Lorentz.[9] Later in the
same year Albert_Einstein published what is now called special_relativity, by
deriving the Lorentz transformation under the assumptions of the principle_of
relativity and the constancy of the speed of light in any inertial_reference
frame, and by abandoning the mechanistic aether as unnecessary.[10]
***** Derivation of the group of Lorentz transformations[edit] *****
Main articles: Derivations_of_the_Lorentz_transformations and Lorentz_group
An event is something that happens at a certain point in spacetime, or more
generally, the point in spacetime itself. In any inertial frame an event is
specified by a time coordinate ct and a set of Cartesian_coordinates x, y, z to
specify position in space in that frame. Subscripts label individual events.
From Einstein's second_postulate_of_relativity follows
          c  2   (  t  2   &#x2212;  t  1    )  2   &#x2212; (  x  2
      &#x2212;  x  1    )  2   &#x2212; (  y  2   &#x2212;  y  1
      )  2   &#x2212; (  z  2   &#x2212;  z  1    )  2   = 0
      (lightlike separated events 1, 2)    {\displaystyle c^{2}(t_      
      {2}-t_{1})^{2}-(x_{2}-x_{1})^{2}-(y_{2}-y_{1})^{2}-(z_{2}-z_        (D1)
      {1})^{2}=0\quad {\text{(lightlike separated events 1, 2)}}}  [
      {\displaystyle c^{2}(t_{2}-t_{1})^{2}-(x_{2}-x_{1})^{2}-(y_
      {2}-y_{1})^{2}-(z_{2}-z_{1})^{2}=0\quad {\text{(lightlike
      separated events 1, 2)}}}]
in all inertial frames for events connected by light signals. The quantity on
the left is called the spacetime interval between events a1 = (t1, x1, y1, z1)
and a2 = (t2, x2, y2, z2). The interval between any two events, not necessarily
separated by light signals, is in fact invariant, i.e., independent of the
state of relative motion of observers in different inertial frames, as is shown
using_homogeneity_and_isotropy_of_space. The transformation sought after thus
must possess the property that
               c  2   (  t  2   &#x2212;  t  1    )  2   &#x2212;
      (  x  2   &#x2212;  x  1    )  2   &#x2212; (  y  2   &#x2212;
      y  1    )  2   &#x2212; (  z  2   &#x2212;  z  1    )  2
      =      c  2   (  t  2  &#x2032;  &#x2212;  t  1  &#x2032;   )
      2   &#x2212; (  x  2  &#x2032;  &#x2212;  x  1  &#x2032;   )
      2   &#x2212; (  y  2  &#x2032;  &#x2212;  y  1  &#x2032;   )
      2   &#x2212; (  z  2  &#x2032;  &#x2212;  z  1  &#x2032;   )
      2     (all events 1, 2)  .       {\displaystyle {\begin           
      {aligned}&c^{2}(t_{2}-t_{1})^{2}-(x_{2}-x_{1})^{2}-(y_{2}-y_        (D2)
      {1})^{2}-(z_{2}-z_{1})^{2}\\[6pt]={}&c^{2}(t_{2}'-t_{1}')^{2}-
      (x_{2}'-x_{1}')^{2}-(y_{2}'-y_{1}')^{2}-(z_{2}'-z_{1}')^
      {2}\quad {\text{(all events 1, 2)}}.\end{aligned}}}  [
      {\displaystyle {\begin{aligned}&c^{2}(t_{2}-t_{1})^{2}-(x_{2}-
      x_{1})^{2}-(y_{2}-y_{1})^{2}-(z_{2}-z_{1})^{2}\\[6pt]={}&c^{2}
      (t_{2}'-t_{1}')^{2}-(x_{2}'-x_{1}')^{2}-(y_{2}'-y_{1}')^{2}-
      (z_{2}'-z_{1}')^{2}\quad {\text{(all events 1, 2)}}.\end
      {aligned}}}]
where (ct, x, y, z) are the spacetime coordinates used to define events in one
frame, and (ct′, x′, y′, z′) are the coordinates in another frame. First one
observes that (D2) is satisfied if an arbitrary 4-tuple b of numbers are added
to events a1 and a2. Such transformations are called spacetime translations and
are not dealt with further here. Then one observes that a linear solution
preserving the origin of the simpler problem
               c  2    t  2   &#x2212;  x  2   &#x2212;  y  2
      &#x2212;  z  2   =  c  2    t  &#x2032;  2    &#x2212;  x
      &#x2032;  2    &#x2212;  y  &#x2032;  2    &#x2212;  z
      &#x2032;  2         or      c  2    t  1    t  2   &#x2212;  x
      1    x  2   &#x2212;  y  1    y  2   &#x2212;  z  1    z  2
      =  c  2    t  1  &#x2032;   t  2  &#x2032;  &#x2212;  x  1
      &#x2032;   x  2  &#x2032;  &#x2212;  y  1  &#x2032;   y  2
      &#x2032;  &#x2212;  z  1  &#x2032;   z  2  &#x2032;               
      {\displaystyle {\begin{aligned}&c^{2}t^{2}-x^{2}-y^{2}-z^           (D3)
      {2}=c^{2}t'^{2}-x'^{2}-y'^{2}-z'^{2}\\[6pt]{\text{or}}\quad
      &c^{2}t_{1}t_{2}-x_{1}x_{2}-y_{1}y_{2}-z_{1}z_{2}=c^{2}t'_
      {1}t'_{2}-x'_{1}x'_{2}-y'_{1}y'_{2}-z'_{1}z'_{2}\end
      {aligned}}}  [{\displaystyle {\begin{aligned}&c^{2}t^{2}-x^
      {2}-y^{2}-z^{2}=c^{2}t'^{2}-x'^{2}-y'^{2}-z'^{2}\\[6pt]{\text
      {or}}\quad &c^{2}t_{1}t_{2}-x_{1}x_{2}-y_{1}y_{2}-z_{1}z_
      {2}=c^{2}t'_{1}t'_{2}-x'_{1}x'_{2}-y'_{1}y'_{2}-z'_{1}z'_
      {2}\end{aligned}}}]
solves the general problem too. (A solution satisfying the left formula
automatically satisfies the right formula, see polarization_identity.) Finding
the solution to the simpler problem is just a matter of look-up in the theory
of classical_groups that preserve bilinear_forms of various signature.[nb_2]
First equation in (D3) can be written more compactly as
         ( a , a ) = (  a &#x2032;  ,  a &#x2032;  )   or   a
      &#x22C5; a =  a &#x2032;  &#x22C5;  a &#x2032;  ,            
      {\displaystyle (a,a)=(a',a')\quad {\text{or}}\quad a\cdot      (D4)
      a=a'\cdot a',}  [{\displaystyle (a,a)=(a',a')\quad {\text
      {or}}\quad a\cdot a=a'\cdot a',}]
where (Â·, Â·) refers to the bilinear form of signature (1, 3) on â4 exposed
by the right hand side formula in (D3). The alternative notation defined on the
right is referred to as the relativistic dot product. Spacetime mathematically
viewed as â4 endowed with this bilinear form is known as Minkowski_space M.
The Lorentz transformation is thus an element of the group Lorentz group O(1,
3), the Lorentz_group or, for those that prefer the other metric_signature, O
(3, 1) (also called the Lorentz group).[nb_3] One has
         ( a , a ) = ( &#x039B; a , &#x039B; a ) = (  a &#x2032;  ,
      a &#x2032;  ) ,  &#x039B; &#x2208;  O  ( 1 , 3 ) ,  a ,  a
      &#x2032;  &#x2208; M ,   {\displaystyle (a,a)=(\Lambda            (D5)
      a,\Lambda a)=(a',a'),\quad \Lambda \in \mathrm {O} (1,3),\quad    
      a,a'\in M,}  [{\displaystyle (a,a)=(\Lambda a,\Lambda a)=
      (a',a'),\quad \Lambda \in \mathrm {O} (1,3),\quad a,a'\in M,}]
which is precisely preservation of the bilinear form (D3) which implies (by
linearity of Î and bilinearity of the form) that (D2) is satisfied. The
elements of the Lorentz group are rotations and boosts and mixes thereof. If
the spacetime translations are included, then one obtains the inhomogeneous
Lorentz group or the PoincarÃ©_group.
***** Generalities[edit] *****
The relations between the primed and unprimed spacetime coordinates are the
Lorentz transformations, each coordinate in one frame is a linear_function of
all the coordinates in the other frame, and the inverse_functions are the
inverse transformation. Depending on how the frames move relative to each
other, and how they are oriented in space relative to each other, other
parameters that describe direction, speed, and orientation enter the
transformation equations.
Transformations describing relative motion with constant (uniform) velocity and
without rotation of the space coordinate axes are called boosts, and the
relative velocity between the frames is the parameter of the transformation.
The other basic type of Lorentz transformations is rotations in the spatial
coordinates only, these are also inertial frames since there is no relative
motion, the frames are simply tilted (and not continuously rotating), and in
this case quantities defining the rotation are the parameters of the
transformation (e.g., axisâangle_representation, or Euler_angles, etc.). A
combination of a rotation and boost is a homogeneous transformation, which
transforms the origin back to the origin.
The full Lorentz group O(3, 1) also contains special transformations that are
neither rotations nor boosts, but rather reflections in a plane through the
origin. Two of these can be singled out; spatial_inversion in which the spatial
coordinates of all events are reversed in sign and temporal_inversion in which
the time coordinate for each event gets its sign reversed.
Boosts should not be conflated with mere displacements in spacetime; in this
case, the coordinate systems are simply shifted and there is no relative
motion. However, these also count as symmetries forced by special relativity
since they leave the spacetime interval invariant. A combination of a rotation
with a boost, followed by a shift in spacetime, is an inhomogeneous Lorentz
transformation, an element of the PoincarÃ© group, which is also called the
inhomogeneous Lorentz group.
***** Physical formulation of Lorentz boosts[edit] *****
Further information: Derivations_of_the_Lorentz_transformations
**** Coordinate transformation[edit] ****
The spacetime coordinates of an event, as measured by each observer in their
inertial reference frame (in standard configuration) are shown in the speech
bubbles.
Top: frame F′ moves at velocity v along the x-axis of frame F.
Bottom: frame F moves at velocity âv along the xâ²-axis of frame F′.[11]
A "stationary" observer in frame F defines events with coordinates t, x, y, z.
Another frame F′ moves with velocity v relative to F, and an observer in this
"moving" frame F′ defines events using the coordinates t′, x′, y′, z′.
The coordinate axes in each frame are parallel (the x and x′ axes are parallel,
the y and y′ axes are parallel, and the z and z′ axes are parallel), remain
mutually perpendicular, and relative motion is along the coincident xx′ axes.
At t = t′ = 0, the origins of both coordinate systems are the same, (x, y, z) =
(x′, y′, z′) = (0, 0, 0). In other words, the times and positions are
coincident at this event. If all these hold, then the coordinate systems are
said to be in standard configuration, or synchronized.
If an observer in F records an event t, x, y, z, then an observer in F′ records
the same event with coordinates[12]
Lorentz boost (x direction)
              t &#x2032;     = &#x03B3;  (  t &#x2212;    v x   c  2      )
      x &#x2032;     = &#x03B3;  (  x &#x2212; v t  )       y &#x2032;     = y
      z &#x2032;     = z       {\displaystyle {\begin{aligned}t'&=\gamma \left
      (t-{\frac {vx}{c^{2}}}\right)\\x'&=\gamma \left(x-
      vt\right)\\y'&=y\\z'&=z\end{aligned}}}  [{\displaystyle {\begin
      {aligned}t'&=\gamma \left(t-{\frac {vx}{c^{2}}}\right)\\x'&=\gamma \left
      (x-vt\right)\\y'&=y\\z'&=z\end{aligned}}}]
where v is the relative velocity between frames in the x-direction, c is the
speed_of_light, and
         &#x03B3; =   1  1 &#x2212;    v  2    c  2          {\displaystyle
      \gamma ={\frac {1}{\sqrt {1-{\frac {v^{2}}{c^{2}}}}}}}  [\gamma ={\frac
      {1}{\sqrt {1-{\frac {v^{2}}{c^{2}}}}}}]
(lowercase gamma) is the Lorentz_factor.
Here, v is the parameter of the transformation, for a given boost it is a
constant number, but can take a continuous range of values. In the setup used
here, positive relative velocity v > 0 is motion along the positive directions
of the xx′ axes, zero relative velocity v = 0 is no relative motion, while
negative relative velocity v < 0 is relative motion along the negative
directions of the xx′ axes. The magnitude of relative velocity v cannot equal
or exceed c, so only subluminal speeds âc < v < c are allowed. The
corresponding range of Î³ is 1 â¤ Î³ < â.
The transformations are not defined if v is outside these limits. At the speed
of light (v = c) Î³ is infinite, and faster_than_light (v > c) Î³ is a complex
number, each of which make the transformations unphysical. The space and time
coordinates are measurable quantities and numerically must be real numbers.
As an active_transformation, an observer in F′ notices the coordinates of the
event to be "boosted" in the negative directions of the xx′ axes, because of
the âv in the transformations. This has the equivalent effect of the
coordinate system F′ boosted in the positive directions of the xx′ axes, while
the event does not change and is simply represented in another coordinate
system, a passive_transformation.
The inverse relations (t, x, y, z in terms of t′, x′, y′, z′) can be found by
algebraically solving the original set of equations. A more efficient way is to
use physical principles. Here F′ is the "stationary" frame while F is the
"moving" frame. According to the principle of relativity, there is no
privileged frame of reference, so the transformations from F′ to F must take
exactly the same form as the transformations from F to F′. The only difference
is F moves with velocity âv relative to F′ (i.e., the relative velocity has
the same magnitude but is oppositely directed). Thus if an observer in F′ notes
an event t′, x′, y′, z′, then an observer in F notes the same event with
coordinates
Inverse Lorentz boost (x direction)
             t    = &#x03B3;  (   t &#x2032;  +    v  x &#x2032;    c  2      )
      x    = &#x03B3;  (   x &#x2032;  + v  t &#x2032;   )      y    =  y
      &#x2032;      z    =  z &#x2032;  ,       {\displaystyle {\begin
      {aligned}t&=\gamma \left(t'+{\frac {vx'}{c^{2}}}\right)\\x&=\gamma \left
      (x'+vt'\right)\\y&=y'\\z&=z',\end{aligned}}}  [{\displaystyle {\begin
      {aligned}t&=\gamma \left(t'+{\frac {vx'}{c^{2}}}\right)\\x&=\gamma \left
      (x'+vt'\right)\\y&=y'\\z&=z',\end{aligned}}}]
and the value of Î³ remains unchanged. This "trick" of simply reversing the
direction of relative velocity while preserving its magnitude, and exchanging
primed and unprimed variables, always applies to finding the inverse
transformation of every boost in any direction.
Sometimes it is more convenient to use Î² = v/c (lowercase beta) instead of v,
so that
             c  t &#x2032;     = &#x03B3;  (  c t &#x2212; &#x03B2; x  )   ,
      x &#x2032;     = &#x03B3;  (  x &#x2212; &#x03B2; c t  )   ,
      {\displaystyle {\begin{aligned}ct'&=\gamma \left(ct-\beta
      x\right)\,,\\x'&=\gamma \left(x-\beta ct\right)\,,\\\end{aligned}}}  [
      {\displaystyle {\begin{aligned}ct'&=\gamma \left(ct-\beta
      x\right)\,,\\x'&=\gamma \left(x-\beta ct\right)\,,\\\end{aligned}}}]
which shows much more clearly the symmetry in the transformation. From the
allowed ranges of v and the definition of Î², it follows â1 < Î² < 1. The use
of Î² and Î³ is standard throughout the literature.
The Lorentz transformations can also be derived in a way that resembles
circular rotations in 3d space using the hyperbolic_functions. For the boost in
the x direction, the results are
Lorentz boost (x direction with rapidity Î¶)
             c  t &#x2032;     = c t cosh &#x2061; &#x03B6; &#x2212; x sinh
      &#x2061; &#x03B6;      x &#x2032;     = x cosh &#x2061; &#x03B6; &#x2212;
      c t sinh &#x2061; &#x03B6;      y &#x2032;     = y      z &#x2032;     =
      z       {\displaystyle {\begin{aligned}ct'&=ct\cosh \zeta -x\sinh \zeta
      \\x'&=x\cosh \zeta -ct\sinh \zeta \\y'&=y\\z'&=z\end{aligned}}}  [
      {\displaystyle {\begin{aligned}ct'&=ct\cosh \zeta -x\sinh \zeta
      \\x'&=x\cosh \zeta -ct\sinh \zeta \\y'&=y\\z'&=z\end{aligned}}}]
where Î¶ (lowercase zeta) is a parameter called rapidity (many other symbols
are used, including Î¸, Ï, Ï, Î·, Ï, Î¾). Given the strong resemblance to
rotations of spatial coordinates in 3d space in the Cartesian xy, yz, and zx
planes, a Lorentz boost can be thought of as a hyperbolic_rotation of spacetime
coordinates in the xt, yt, and zt Cartesian-time planes of 4d Minkowski_space.
The parameter Î¶ is the hyperbolic_angle of rotation, analogous to the ordinary
angle for circular rotations. This transformation can be illustrated with a
Minkowski_diagram.
The hyperbolic functions arise from the difference between the squares of the
time and spatial coordinates in the spacetime interval, rather than a sum. The
geometric significance of the hyperbolic functions can be visualized by taking
x = 0 or ct = 0 in the transformations. Squaring and subtracting the results,
one can derive hyperbolic curves of constant coordinate values but varying Î¶,
which parametrizes the curves according to the identity
          cosh  2   &#x2061; &#x03B6; &#x2212;  sinh  2   &#x2061; &#x03B6; = 1
      .   {\displaystyle \cosh ^{2}\zeta -\sinh ^{2}\zeta =1\,.}  [\cosh ^
      {2}\zeta -\sinh ^{2}\zeta =1\,.]
Conversely the ct and x axes can be constructed for varying coordinates but
constant Î¶. The definition
         tanh &#x2061; &#x03B6; =    sinh &#x2061; &#x03B6;   cosh &#x2061;
      &#x03B6;     ,   {\displaystyle \tanh \zeta ={\frac {\sinh \zeta }{\cosh
      \zeta }}\,,}  [\tanh \zeta ={\frac {\sinh \zeta }{\cosh \zeta }}\,,]
provides the link between a constant value of rapidity, and the slope of the ct
axis in spacetime. A consequence these two hyperbolic formulae is an identity
that matches the Lorentz factor
         cosh &#x2061; &#x03B6; =   1  1 &#x2212;  tanh  2   &#x2061; &#x03B6;
      .   {\displaystyle \cosh \zeta ={\frac {1}{\sqrt {1-\tanh ^{2}\zeta
      }}}\,.}  [\cosh \zeta ={\frac {1}{\sqrt {1-\tanh ^{2}\zeta }}}\,.]
Comparing the Lorentz transformations in terms of the relative velocity and
rapidity, or using the above formulae, the connections between Î², Î³, and Î¶
are
             &#x03B2;    = tanh &#x2061; &#x03B6;  ,     &#x03B3;    = cosh
      &#x2061; &#x03B6;  ,     &#x03B2; &#x03B3;    = sinh &#x2061; &#x03B6;  .
      {\displaystyle {\begin{aligned}\beta &=\tanh \zeta \,,\\\gamma &=\cosh
      \zeta \,,\\\beta \gamma &=\sinh \zeta \,.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}\beta &=\tanh \zeta \,,\\\gamma &=\cosh \zeta \,,\\\beta
      \gamma &=\sinh \zeta \,.\end{aligned}}}]
Taking the inverse hyperbolic tangent gives the rapidity
         &#x03B6; =  tanh  &#x2212; 1   &#x2061; &#x03B2;  .   {\displaystyle
      \zeta =\tanh ^{-1}\beta \,.}  [\zeta =\tanh ^{-1}\beta \,.]
Since â1 < Î² < 1, it follows ââ < Î¶ < â. From the relation between Î¶
and Î², positive rapidity Î¶ > 0 is motion along the positive directions of the
xx′ axes, zero rapidity Î¶ = 0 is no relative motion, while negative rapidity
Î¶ < 0 is relative motion along the negative directions of the xx′ axes.
The inverse transformations are obtained by exchanging primed and unprimed
quantities to switch the coordinate frames, and negating rapidity Î¶ â âÎ¶
since this is equivalent to negating the relative velocity. Therefore,
Inverse Lorentz boost (x direction with rapidity Î¶)
             c t    = c  t &#x2032;  cosh &#x2061; &#x03B6; +  x &#x2032;  sinh
      &#x2061; &#x03B6;     x    =  x &#x2032;  cosh &#x2061; &#x03B6; + c  t
      &#x2032;  sinh &#x2061; &#x03B6;     y    =  y &#x2032;      z    =  z
      &#x2032;        {\displaystyle {\begin{aligned}ct&=ct'\cosh \zeta
      +x'\sinh \zeta \\x&=x'\cosh \zeta +ct'\sinh \zeta \\y&=y'\\z&=z'\end
      {aligned}}}  [{\displaystyle {\begin{aligned}ct&=ct'\cosh \zeta +x'\sinh
      \zeta \\x&=x'\cosh \zeta +ct'\sinh \zeta \\y&=y'\\z&=z'\end{aligned}}}]
The inverse transformations can be similarly visualized by considering the
cases when x′ = 0 and ct′ = 0.
So far the Lorentz transformations have been applied to one event. If there are
two events, there is a spatial separation and time interval between them. It
follows from the linearity of the Lorentz transformations that two values of
space and time coordinates can be chosen, the Lorentz transformations can be
applied to each, then subtracted to get the Lorentz transformations of the
differences;
             &#x0394;  t &#x2032;     = &#x03B3;  (  &#x0394; t &#x2212;    v
      &#x0394; x   c  2      )   ,     &#x0394;  x &#x2032;     = &#x03B3;
      (  &#x0394; x &#x2212; v  &#x0394; t  )   ,       {\displaystyle {\begin
      {aligned}\Delta t'&=\gamma \left(\Delta t-{\frac {v\,\Delta x}{c^
      {2}}}\right)\,,\\\Delta x'&=\gamma \left(\Delta x-v\,\Delta
      t\right)\,,\end{aligned}}}  [{\displaystyle {\begin{aligned}\Delta
      t'&=\gamma \left(\Delta t-{\frac {v\,\Delta x}{c^{2}}}\right)\,,\\\Delta
      x'&=\gamma \left(\Delta x-v\,\Delta t\right)\,,\end{aligned}}}]
with inverse relations
             &#x0394; t    = &#x03B3;  (  &#x0394;  t &#x2032;  +    v
      &#x0394;  x &#x2032;    c  2      )   ,     &#x0394; x    = &#x03B3;
      (  &#x0394;  x &#x2032;  + v  &#x0394;  t &#x2032;   )   .
      {\displaystyle {\begin{aligned}\Delta t&=\gamma \left(\Delta t'+{\frac
      {v\,\Delta x'}{c^{2}}}\right)\,,\\\Delta x&=\gamma \left(\Delta
      x'+v\,\Delta t'\right)\,.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}\Delta t&=\gamma \left(\Delta t'+{\frac {v\,\Delta x'}{c^
      {2}}}\right)\,,\\\Delta x&=\gamma \left(\Delta x'+v\,\Delta
      t'\right)\,.\end{aligned}}}]
where Î (uppercase delta) indicates a difference of quantities; e.g., Îx = x2
â x1 for two values of x coordinates, and so on.
These transformations on differences rather than spatial points or instants of
time are useful for a number of reasons:
    * in calculations and experiments, it is lengths between two points or time
      intervals that are measured or of interest (e.g., the length of a moving
      vehicle, or time duration it takes to travel from one place to another),
    * the transformations of velocity can be readily derived by making the
      difference infinitesimally small and dividing the equations, and the
      process repeated for the transformation of acceleration,
    * if the coordinate systems are never coincident (i.e., not in standard
      configuration), and if both observers can agree on an event t0, x0, y0,
      z0 in F and t0′, x0′, y0′, z0′ in F′, then they can use that event as the
      origin, and the spacetime coordinate differences are the differences
      between their coordinates and this origin, e.g., Îx = x â x0, Îx′ =
      x′ â x0′, etc.
**** Physical implications[edit] ****
A critical requirement of the Lorentz transformations is the invariance of the
speed of light, a fact used in their derivation, and contained in the
transformations themselves. If in F the equation for a pulse of light along the
x direction is x = ct, then in F′ the Lorentz transformations give x′ = ct′,
and vice versa, for any âc < v < c.
For relative speeds much less than the speed of light, the Lorentz
transformations reduce to the Galilean_transformation
              t &#x2032;     &#x2248; t      x &#x2032;     &#x2248; x &#x2212;
      v t       {\displaystyle {\begin{aligned}t'&\approx t\\x'&\approx x-
      vt\end{aligned}}}  [{\displaystyle {\begin{aligned}t'&\approx
      t\\x'&\approx x-vt\end{aligned}}}]
in accordance with the correspondence_principle. It is sometimes said that
nonrelativistic physics is a physics of "instantaneous action at a distance".
[13]
Three counterintuitive, but correct, predictions of the transformations are:
  Relativity_of_simultaneity
      Suppose two events occur simultaneously (Ît = 0) along the x axis, but
      separated by a nonzero displacement Îx. Then in F′, we find that
      &#x0394;  t &#x2032;  = &#x03B3;    &#x2212; v  &#x0394; x   c  2
      {\displaystyle \Delta t'=\gamma {\frac {-v\,\Delta x}{c^{2}}}}  [
      {\displaystyle \Delta t'=\gamma {\frac {-v\,\Delta x}{c^{2}}}}], so the
      events are no longer simultaneous according to a moving observer.
  Time_dilation
      Suppose there is a clock at rest in F. If a time interval is measured at
      the same point in that frame, so that Îx = 0, then the transformations
      give this interval in F′ by Ît′ = Î³Ît. Conversely, suppose there is a
      clock at rest in F′. If an interval is measured at the same point in that
      frame, so that Îx′ = 0, then the transformations give this interval in F
      by Ît = Î³Ît′. Either way, each observer measures the time interval
      between ticks of a moving clock to be longer by a factor Î³ than the time
      interval between ticks of his own clock.
  Length_contraction
      Suppose there is a rod at rest in F aligned along the x axis, with length
      Îx. In F′, the rod moves with velocity -v, so its length must be
      measured by taking two simultaneous (Ît′ = 0) measurements at opposite
      ends. Under these conditions, the inverse Lorentz transform shows that
      Îx = Î³Îx′. In F the two measurements are no longer simultaneous, but
      this does not matter because the rod is at rest in F. So each observer
      measures the distance between the end points of a moving rod to be
      shorter by a factor 1/Î³ than the end points of an identical rod at rest
      in his own frame. Length contraction affects any geometric quantity
      related to lengths, so from the perspective of a moving observer, areas
      and volumes will also appear to shrink along the direction of motion.
**** Vector transformations[edit] ****
Further information: Euclidean_vector and vector_projection
An observer in frame F observes F′ to move with velocity v, while F′ observes F
to move with velocity âv. The coordinate axes of each frame are still
parallel and orthogonal. The position vector as measured in each frame is split
into components parallel and perpendicular to the relative velocity vector v.
Left: Standard configuration. Right: Inverse configuration.
The use of vectors allows positions and velocities to be expressed in arbitrary
directions compactly. A single boost in any direction depends on the full
relative velocity_vector v with a magnitude |v| = v that cannot equal or exceed
c, so that 0 â¤ v < c.
Only time and the coordinates parallel to the direction of relative motion
change, while those coordinates perpendicular do not. With this in mind, split
the spatial position_vector r as measured in F, and r′ as measured in F′, each
into components perpendicular (â¥) and parallel ( â ) to v,
          r  =   r   &#x22A5;   +   r   &#x2016;    ,    r  &#x2032;  =   r
      &#x22A5;  &#x2032;  +   r   &#x2016;  &#x2032;   ,   {\displaystyle
      \mathbf {r} =\mathbf {r} _{\perp }+\mathbf {r} _{\|}\,,\quad \mathbf {r}
      '=\mathbf {r} _{\perp }'+\mathbf {r} _{\|}'\,,}  [\mathbf {r} =\mathbf
      {r} _{\perp }+\mathbf {r} _{\|}\,,\quad \mathbf {r} '=\mathbf {r} _{\perp
      }'+\mathbf {r} _{\|}'\,,]
then the transformations are
              t &#x2032;     = &#x03B3;  (  t &#x2212;      r   &#x2225;
      &#x22C5;  v    c  2      )        r   &#x2016;  &#x2032;     = &#x03B3;
      (   r   &#x2016;   &#x2212;  v  t )       r   &#x22A5;  &#x2032;     =
      r   &#x22A5;         {\displaystyle {\begin{aligned}t'&=\gamma \left(t-
      {\frac {\mathbf {r} _{\parallel }\cdot \mathbf {v} }{c^
      {2}}}\right)\\\mathbf {r} _{\|}'&=\gamma (\mathbf {r} _{\|}-\mathbf {v}
      t)\\\mathbf {r} _{\perp }'&=\mathbf {r} _{\perp }\end{aligned}}}  [
      {\displaystyle {\begin{aligned}t'&=\gamma \left(t-{\frac {\mathbf {r} _
      {\parallel }\cdot \mathbf {v} }{c^{2}}}\right)\\\mathbf {r} _
      {\|}'&=\gamma (\mathbf {r} _{\|}-\mathbf {v} t)\\\mathbf {r} _{\perp
      }'&=\mathbf {r} _{\perp }\end{aligned}}}]
where Â· is the dot_product. The Lorentz factor Î³ retains its definition for a
boost in any direction, since it depends only on the magnitude of the relative
velocity. The definition Î² = v/c with magnitude 0 â¤ Î² < 1 is also used by
some authors.
Introducing a unit_vector n = v/v = Î²/Î² in the direction of relative motion,
the relative velocity is v = vn with magnitude v and direction n, and vector
projection and rejection give respectively
           r   &#x2225;   = (  r  &#x22C5;  n  )  n   ,    r   &#x22A5;   =  r
      &#x2212; (  r  &#x22C5;  n  )  n    {\displaystyle \mathbf {r} _
      {\parallel }=(\mathbf {r} \cdot \mathbf {n} )\mathbf {n} \,,\quad \mathbf
      {r} _{\perp }=\mathbf {r} -(\mathbf {r} \cdot \mathbf {n} )\mathbf {n} }
      [{\displaystyle \mathbf {r} _{\parallel }=(\mathbf {r} \cdot \mathbf {n}
      )\mathbf {n} \,,\quad \mathbf {r} _{\perp }=\mathbf {r} -(\mathbf {r}
      \cdot \mathbf {n} )\mathbf {n} }]
Accumulating the results gives the full transformations,
Lorentz boost (in direction n with magnitude v)
        t &#x2032;     = &#x03B3;  (  t &#x2212;    v  n  &#x22C5;  r    c  2
)   ,       r  &#x2032;     =  r  + ( &#x03B3; &#x2212; 1 ) (  r  &#x22C5;  n
)  n  &#x2212; &#x03B3; t v  n   .       {\displaystyle {\begin
{aligned}t'&=\gamma \left(t-{\frac {v\mathbf {n} \cdot \mathbf {r} }{c^
{2}}}\right)\,,\\\mathbf {r} '&=\mathbf {r} +(\gamma -1)(\mathbf {r} \cdot
\mathbf {n} )\mathbf {n} -\gamma tv\mathbf {n} \,.\end{aligned}}}  [
{\displaystyle {\begin{aligned}t'&=\gamma \left(t-{\frac {v\mathbf {n} \cdot
\mathbf {r} }{c^{2}}}\right)\,,\\\mathbf {r} '&=\mathbf {r} +(\gamma -1)
(\mathbf {r} \cdot \mathbf {n} )\mathbf {n} -\gamma tv\mathbf {n} \,.\end
{aligned}}}]
The projection and rejection also applies to r′. For the inverse
transformations, exchange r and r′ to switch observed coordinates, and negate
the relative velocity v â âv (or simply the unit vector n â ân since
the magnitude v is always positive) to obtain
Inverse Lorentz boost (in direction n with magnitude v)
       t    = &#x03B3;  (   t &#x2032;  +      r  &#x2032;  &#x22C5; v  n    c
2      )   ,      r     =   r  &#x2032;  + ( &#x03B3; &#x2212; 1 ) (   r
&#x2032;  &#x22C5;  n  )  n  + &#x03B3;  t &#x2032;  v  n   ,
{\displaystyle {\begin{aligned}t&=\gamma \left(t'+{\frac {\mathbf {r} '\cdot
v\mathbf {n} }{c^{2}}}\right)\,,\\\mathbf {r} &=\mathbf {r} '+(\gamma -1)
(\mathbf {r} '\cdot \mathbf {n} )\mathbf {n} +\gamma t'v\mathbf {n} \,,\end
{aligned}}}  [{\displaystyle {\begin{aligned}t&=\gamma \left(t'+{\frac {\mathbf
{r} '\cdot v\mathbf {n} }{c^{2}}}\right)\,,\\\mathbf {r} &=\mathbf {r} '+
(\gamma -1)(\mathbf {r} '\cdot \mathbf {n} )\mathbf {n} +\gamma t'v\mathbf {n}
\,,\end{aligned}}}]
The unit vector has the advantage of simplifying equations for a single boost,
allows either v or Î² to be reinstated when convenient, and the rapidity
parametrization is immediately obtained by replacing Î² and Î²Î³. It is not
convenient for multiple boosts.
The vectorial relation between relative velocity and rapidity is[14]
          &#x03B2;  = &#x03B2;  n  =  n  tanh &#x2061; &#x03B6;  ,
      {\displaystyle {\boldsymbol {\beta }}=\beta \mathbf {n} =\mathbf {n}
      \tanh \zeta \,,}  [{\boldsymbol {\beta }}=\beta \mathbf {n} =\mathbf {n}
      \tanh \zeta \,,]
and the "rapidity vector" can be defined as
          &#x03B6;  = &#x03B6;  n  =  n   tanh  &#x2212; 1   &#x2061; &#x03B2;
      ,   {\displaystyle {\boldsymbol {\zeta }}=\zeta \mathbf {n} =\mathbf {n}
      \tanh ^{-1}\beta \,,}  [{\boldsymbol {\zeta }}=\zeta \mathbf {n} =\mathbf
      {n} \tanh ^{-1}\beta \,,]
each of which serves as a useful abbreviation in some contexts. The magnitude
of Î¶ is the absolute value of the rapidity scalar confined to 0 â¤ Î¶ < â,
which agrees with the range 0 â¤ Î² < 1.
**** Transformation of velocities[edit] ****
Further information: differential_of_a_function and velocity_addition_formula
The transformation of velocities provides the definition relativistic_velocity
addition ⊕, the ordering of vectors is chosen to reflect the ordering of the
addition of velocities; first v (the velocity of F′ relative to F) then u′ (the
velocity of X relative to F′) to obtain u = v ⊕ u′ (the velocity of X relative
to F).
Defining the coordinate velocities and Lorentz factor by
          u  =    d  r    d t     ,    u  &#x2032;  =    d   r  &#x2032;    d
      t &#x2032;      ,   &#x03B3;   v    =   1  1 &#x2212;      v  &#x22C5;  v
      c  2           {\displaystyle \mathbf {u} ={\frac {d\mathbf {r} }
      {dt}}\,,\quad \mathbf {u} '={\frac {d\mathbf {r} '}{dt'}}\,,\quad \gamma
      _{\mathbf {v} }={\frac {1}{\sqrt {1-{\dfrac {\mathbf {v} \cdot \mathbf
      {v} }{c^{2}}}}}}}  [\mathbf {u} ={\frac {d\mathbf {r} }{dt}}\,,\quad
      \mathbf {u} '={\frac {d\mathbf {r} '}{dt'}}\,,\quad \gamma _{\mathbf {v}
      }={\frac {1}{\sqrt {1-{\dfrac {\mathbf {v} \cdot \mathbf {v} }{c^
      {2}}}}}}]
taking the differentials in the coordinates and time of the vector
transformations, then dividing equations, leads to
           u  &#x2032;  =   1  1 &#x2212;     v  &#x22C5;  u    c  2
      [     u   &#x03B3;   v      &#x2212;  v  +   1  c  2        &#x03B3;   v
      &#x03B3;   v    + 1     (   u  &#x22C5;  v   )   v   ]    {\displaystyle
      \mathbf {u} '={\frac {1}{1-{\frac {\mathbf {v} \cdot \mathbf {u} }{c^
      {2}}}}}\left[{\frac {\mathbf {u} }{\gamma _{\mathbf {v} }}}-\mathbf {v} +
      {\frac {1}{c^{2}}}{\frac {\gamma _{\mathbf {v} }}{\gamma _{\mathbf {v}
      }+1}}\left(\mathbf {u} \cdot \mathbf {v} \right)\mathbf {v} \right]}  [
      {\displaystyle \mathbf {u} '={\frac {1}{1-{\frac {\mathbf {v} \cdot
      \mathbf {u} }{c^{2}}}}}\left[{\frac {\mathbf {u} }{\gamma _{\mathbf {v}
      }}}-\mathbf {v} +{\frac {1}{c^{2}}}{\frac {\gamma _{\mathbf {v} }}{\gamma
      _{\mathbf {v} }+1}}\left(\mathbf {u} \cdot \mathbf {v} \right)\mathbf {v}
      \right]}]
The velocities u and u′ are the velocity of some massive object. They can also
be for a third inertial frame (say F′′), in which case they must be constant.
Denote either entity by X. Then X moves with velocity u relative to F, or
equivalently with velocity u′ relative to F′, in turn F′ moves with velocity v
relative to F. The inverse transformations can be obtained in a similar way, or
as with position coordinates exchange u and u′, and change v to âv.
The transformation of velocity is useful in stellar_aberration, the Fizeau
experiment, and the relativistic_Doppler_effect.
The Lorentz_transformations_of_acceleration can be similarly obtained by taking
differentials in the velocity vectors, and dividing these by the time
differential.
**** Transformation of other quantities[edit] ****
In general, given four quantities A and Z = (Zx, Zy, Zz) and their Lorentz-
boosted counterparts A′ and Z′ = (Z′x, Z′y, Z′z), a relation of the form
          A  2   &#x2212;  Z  &#x22C5;  Z  =    A &#x2032;    2   &#x2212;   Z
      &#x2032;  &#x22C5;   Z  &#x2032;    {\displaystyle A^{2}-\mathbf {Z}
      \cdot \mathbf {Z} ={A'}^{2}-\mathbf {Z} '\cdot \mathbf {Z} '}  [
      {\displaystyle A^{2}-\mathbf {Z} \cdot \mathbf {Z} ={A'}^{2}-\mathbf {Z}
      '\cdot \mathbf {Z} '}]
implies the quantities transform under Lorentz transformations similar to the
transformation of spacetime coordinates;
              A &#x2032;     = &#x03B3;  (  A &#x2212;    v  n  &#x22C5;  Z   c
      )   ,       Z  &#x2032;     =  Z  + ( &#x03B3; &#x2212; 1 ) (  Z
      &#x22C5;  n  )  n  &#x2212;    &#x03B3; A v  n   c    .
      {\displaystyle {\begin{aligned}A'&=\gamma \left(A-{\frac {v\mathbf {n}
      \cdot \mathbf {Z} }{c}}\right)\,,\\\mathbf {Z} '&=\mathbf {Z} +(\gamma -
      1)(\mathbf {Z} \cdot \mathbf {n} )\mathbf {n} -{\frac {\gamma Av\mathbf
      {n} }{c}}\,.\end{aligned}}}  [{\displaystyle {\begin{aligned}A'&=\gamma
      \left(A-{\frac {v\mathbf {n} \cdot \mathbf {Z} }{c}}\right)\,,\\\mathbf
      {Z} '&=\mathbf {Z} +(\gamma -1)(\mathbf {Z} \cdot \mathbf {n} )\mathbf
      {n} -{\frac {\gamma Av\mathbf {n} }{c}}\,.\end{aligned}}}]
The decomposition of Z (and Zâ²) into components perpendicular and parallel to
v is exactly the same as for the position vector, as is the process of
obtaining the inverse transformations (exchange (A, Z) and (A′, Z′) to switch
observed quantities, and reverse the direction of relative motion by the
substitution n â¦ ân).
The quantities (A, Z) collectively make up a four-vector, where A is the
"timelike component", and Z the "spacelike component". Examples of A and Z are
the following:
      Four vector      A                                       Z
      Position four-   Time (multiplied by c), ct              Position_vector,
      vector                                                   r
      Four_momentum    Energy (divided by c), E/c              Momentum, p
      Four-wave_vector angular_frequency (divided by c), Ï/cwave_vector, k
      Four_spin        (No name), st                           Spin, s
      Four_current     Charge_density (multiplied by c), Ïc Current_density,
                                                               j
      Electromagnetic  Electric_potential (divided by c), Ï/Magnetic
      four_potential                                           potential, A
For a given object (e.g., particle, fluid, field, material), if A or Z
correspond to properties specific to the object like its charge_density, mass
density, spin, etc., its properties can be fixed in the rest frame of that
object. Then the Lorentz transformations give the corresponding properties in a
frame moving relative to the object with constant velocity. This breaks some
notions taken for granted in non-relativistic physics. For example, the energy
E of an object is a scalar in non-relativistic mechanics, but not in
relativistic mechanics because energy changes under Lorentz transformations;
its value is different for various inertial frames. In the rest frame of an
object, it has a rest_energy and zero momentum. In a boosted frame its energy
is different and it appears to have a momentum. Similarly, in non-relativistic
quantum mechanics the spin of a particle is a constant vector, but in
relativistic_quantum_mechanics spin s depends on relative motion. In the rest
frame of the particle, the spin pseudovector can be fixed to be its ordinary
non-relativistic spin with a zero timelike quantity st, however a boosted
observer will perceive a nonzero timelike component and an altered spin.[15]
Not all quantities are invariant in the form as shown above, for example
orbital angular_momentum L does not have a timelike quantity, and neither does
the electric_field E nor the magnetic_field B. The definition of angular
momentum is L = r Ã p, and in a boosted frame the altered angular momentum is
L′ = r′ Ã p′. Applying this definition using the transformations of
coordinates and momentum leads to the transformation of angular momentum. It
turns out L transforms with another vector quantity N = (E/c2)r â tp related
to boosts, see relativistic_angular_momentum for details. For the case of the E
and B fields, the transformations cannot be obtained as directly using vector
algebra. The Lorentz_force is the definition of these fields, and in F it is F
= q(E + v Ã B) while in F′ it is F′ = q(E′ + v′ Ã B′). A method of deriving
the EM field transformations in an efficient way which also illustrates the
unit of the electromagnetic field uses tensor algebra, given_below.
***** Mathematical formulation[edit] *****
Main article: Lorentz_group
Further information: Matrix_(mathematics), matrix_product, linear_algebra, and
rotation_formalisms_in_three_dimensions
Throughout, italic non-bold capital letters are 4Ã4 matrices, while non-italic
bold letters are 3Ã3 matrices.
**** Homogeneous Lorentz group[edit] ****
Writing the coordinates in column vectors and the Minkowski_metric Î· as a
square matrix
          X &#x2032;  =   [    c   t &#x2032;       x &#x2032;       y &#x2032;
      z &#x2032;     ]    ,  &#x03B7; =   [    &#x2212; 1   0   0   0     0   1
      0   0     0   0   1   0     0   0   0   1    ]    ,  X =   [    c  t
      x     y     z    ]     {\displaystyle X'={\begin
      {bmatrix}c\,t'\\x'\\y'\\z'\end{bmatrix}}\,,\quad \eta ={\begin{bmatrix}-
      1&0&0&0\\0&1&0&0\\0&0&1&0\\0&0&0&1\end{bmatrix}}\,,\quad X={\begin
      {bmatrix}c\,t\\x\\y\\z\end{bmatrix}}}  [{\displaystyle X'={\begin
      {bmatrix}c\,t'\\x'\\y'\\z'\end{bmatrix}}\,,\quad \eta ={\begin{bmatrix}-
      1&0&0&0\\0&1&0&0\\0&0&1&0\\0&0&0&1\end{bmatrix}}\,,\quad X={\begin
      {bmatrix}c\,t\\x\\y\\z\end{bmatrix}}}]
the spacetime interval takes the form (T denotes transpose)
         X &#x22C5; X =  X   T    &#x03B7; X =    X &#x2032;     T    &#x03B7;
      X &#x2032;     {\displaystyle X\cdot X=X^{\mathrm {T} }\eta X={X'}^
      {\mathrm {T} }\eta {X'}}  [X\cdot X=X^{\mathrm {T} }\eta X={X'}^{\mathrm
      {T} }\eta {X'}]
and is invariant under a Lorentz transformation
          X &#x2032;  = &#x039B; X   {\displaystyle X'=\Lambda X}  [
      {\displaystyle X'=\Lambda X}]
where Î is a square matrix which can depend on parameters.
The set of all Lorentz transformations Î in this article is denoted       L
{\displaystyle {\mathcal {L}}}  [{\mathcal {L}}]. This set together with matrix
multiplication forms a group, in this context known as the Lorentz_group. Also,
the above expression XÂ·X is a quadratic_form of signature (3,1) on spacetime,
and the group of transformations which leaves this quadratic form invariant is
the indefinite_orthogonal_group O(3,1), a Lie_group. In other words, the
Lorentz group is O(3,1). As presented in this article, any Lie groups mentioned
are matrix_Lie_groups. In this context the operation of composition amounts to
matrix_multiplication.
From the invariance of the spacetime interval it follows
         &#x03B7; =  &#x039B;   T    &#x03B7; &#x039B;   {\displaystyle \eta
      =\Lambda ^{\mathrm {T} }\eta \Lambda }  [\eta =\Lambda ^{\mathrm {T}
      }\eta \Lambda ]
and this matrix equation contains the general conditions on the Lorentz
transformation to ensure invariance of the spacetime interval. Taking the
determinant of the equation using the product rule[nb_4] gives immediately
         [ det ( &#x039B; )  ]  2   = 1  &#x21D2;  det ( &#x039B; ) = &#x00B1;
      1   {\displaystyle [\det(\Lambda )]^{2}=1\quad \Rightarrow \quad \det
      (\Lambda )=\pm 1}  [[\det(\Lambda )]^{2}=1\quad \Rightarrow \quad \det
      (\Lambda )=\pm 1]
Writing the Minkowski metric as a block matrix, and the Lorentz transformation
in the most general form,
         &#x03B7; =   [    &#x2212; 1   0     0    I     ]    ,  &#x039B; =
      [    &#x0393;   &#x2212;   a    T        &#x2212;  b     M     ]    ,
      {\displaystyle \eta ={\begin{bmatrix}-1&0\\0&\mathbf {I} \end
      {bmatrix}}\,,\quad \Lambda ={\begin{bmatrix}\Gamma &-\mathbf {a} ^
      {\mathrm {T} }\\-\mathbf {b} &\mathbf {M} \end{bmatrix}}\,,}  [
      {\displaystyle \eta ={\begin{bmatrix}-1&0\\0&\mathbf {I} \end
      {bmatrix}}\,,\quad \Lambda ={\begin{bmatrix}\Gamma &-\mathbf {a} ^
      {\mathrm {T} }\\-\mathbf {b} &\mathbf {M} \end{bmatrix}}\,,}]
carrying out the block matrix multiplications obtains general conditions on Î,
a, b, M to ensure relativistic invariance. Not much information can be directly
extracted from all the conditions, however one of the results
          &#x0393;  2   = 1 +   b    T     b    {\displaystyle \Gamma ^
      {2}=1+\mathbf {b} ^{\mathrm {T} }\mathbf {b} }  [{\displaystyle \Gamma ^
      {2}=1+\mathbf {b} ^{\mathrm {T} }\mathbf {b} }]
is useful; bTb â¥ 0 always so it follows that
          &#x0393;  2   &#x2265; 1  &#x21D2;  &#x0393; &#x2264; &#x2212; 1  ,
      &#x0393; &#x2265; 1   {\displaystyle \Gamma ^{2}\geq 1\quad \Rightarrow
      \quad \Gamma \leq -1\,,\quad \Gamma \geq 1}  [\Gamma ^{2}\geq 1\quad
      \Rightarrow \quad \Gamma \leq -1\,,\quad \Gamma \geq 1]
The negative inequality may be unexpected, because Î multiplies the time
coordinate and this has an effect on time_symmetry. If the positive equality
holds, then Î is the Lorentz factor.
The determinant and inequality provide four ways to classify Lorentz
Transformations (herein LTs for brevity). Any particular LT has only one
determinant sign and only one inequality. There are four sets which include
every possible pair given by the intersections ("n"-shaped symbol meaning
"and") of these classifying sets.
                          Antichronous (or non-
                          orthochronous) LTs         Orthochronous LTs
                                      L    &#x2193;              L    &#x2191;
                                = { &#x039B;  :            = { &#x039B;  :
                                &#x0393; &#x2264;          &#x0393; &#x2265; 1
                                &#x2212; 1 }               }   {\displaystyle
                                {\displaystyle             {\mathcal {L}}^
Intersection, â©            {\mathcal {L}}^            {\uparrow }=\
                                {\downarrow }=\            {\Lambda \,:\,\Gamma
                                {\Lambda \,:\,\Gamma       \geq 1\}}  [
                                \leq -1\}}  [              {\displaystyle
                                {\displaystyle             {\mathcal {L}}^
                                {\mathcal {L}}^            {\uparrow }=\
                                {\downarrow }=\            {\Lambda \,:\,\Gamma
                                {\Lambda \,:\,\Gamma       \geq 1\}}]
                                \leq -1\}}]
                          Proper antichronous LTs    Proper orthochronous LTs
Proper LTs                            L    +                     L    +
            L    +   =          &#x2193;   =    L          &#x2191;   =    L
      { &#x039B;  :  det        +   &#x2229;    L          +   &#x2229;    L
      ( &#x039B; ) = + 1        &#x2193;                   &#x2191;
      }   {\displaystyle        {\displaystyle             {\displaystyle
      {\mathcal {L}}_           {\mathcal {L}}_{+}^        {\mathcal {L}}_{+}^
      {+}=\{\Lambda \,:         {\downarrow }=             {\uparrow }=
      \,\det(\Lambda            {\mathcal {L}}_            {\mathcal {L}}_
      )=+1\}}  [                {+}\cap {\mathcal          {+}\cap {\mathcal
      {\displaystyle            {L}}^{\downarrow }}        {L}}^{\uparrow }}  [
      {\mathcal {L}}_           [{\mathcal {L}}_{+}^       {\mathcal {L}}_{+}^
      {+}=\{\Lambda \,:         {\downarrow }=             {\uparrow }=
      \,\det(\Lambda            {\mathcal {L}}_            {\mathcal {L}}_
      )=+1\}}]                  {+}\cap {\mathcal          {+}\cap {\mathcal
                                {L}}^{\downarrow }]        {L}}^{\uparrow }]
Improper LTs              Improper antichronous LTs  Improper orthochronous LTs
            L    &#x2212;             L    &#x2212;              L    &#x2212;
      = { &#x039B;  :           &#x2193;   =    L          &#x2191;   =    L
      det ( &#x039B; ) =        &#x2212;   &#x2229;        &#x2212;   &#x2229;
      &#x2212; 1 }              L    &#x2193;              L    &#x2191;
      {\displaystyle            {\displaystyle             {\displaystyle
      {\mathcal {L}}_{-         {\mathcal {L}}_{-}^        {\mathcal {L}}_{-}^
      }=\{\Lambda \,:           {\downarrow }=             {\uparrow }=
      \,\det(\Lambda )=-        {\mathcal {L}}_{-          {\mathcal {L}}_{-
      1\}}  [                   }\cap {\mathcal            }\cap {\mathcal
      {\displaystyle            {L}}^{\downarrow }}        {L}}^{\uparrow }}  [
      {\mathcal {L}}_{-         [{\mathcal {L}}_{-}^       {\mathcal {L}}_{-}^
      }=\{\Lambda \,:           {\downarrow }=             {\uparrow }=
      \,\det(\Lambda )=-        {\mathcal {L}}_{-          {\mathcal {L}}_{-
      1\}}]                     }\cap {\mathcal            }\cap {\mathcal
                                {L}}^{\downarrow }]        {L}}^{\uparrow }]
where "+" and "â" indicate the determinant sign, while "â" for â¥ and
"â" for â¤ denote the inequalities.
The full Lorentz group splits into the union ("u"-shaped symbol meaning "or")
of four disjoint_sets
           L   =    L    +   &#x2191;   &#x222A;    L    &#x2212;   &#x2191;
      &#x222A;    L    +   &#x2193;   &#x222A;    L    &#x2212;   &#x2193;
      {\displaystyle {\mathcal {L}}={\mathcal {L}}_{+}^{\uparrow }\cup
      {\mathcal {L}}_{-}^{\uparrow }\cup {\mathcal {L}}_{+}^{\downarrow }\cup
      {\mathcal {L}}_{-}^{\downarrow }}  [{\displaystyle {\mathcal {L}}=
      {\mathcal {L}}_{+}^{\uparrow }\cup {\mathcal {L}}_{-}^{\uparrow }\cup
      {\mathcal {L}}_{+}^{\downarrow }\cup {\mathcal {L}}_{-}^{\downarrow }}]
A subgroup of a group must be closed under the same operation of the group
(here matrix multiplication). In other words, for two Lorentz transformations
Î and L from a particular set, the composite Lorentz transformations ÎL and
LÎ must be in the same set as Î and L. This will not always be the case; it
can be shown that the composition of any two Lorentz transformations always has
the positive determinant and positive inequality, a proper orthochronous
transformation. The sets        L    +   &#x2191;     {\displaystyle {\mathcal
{L}}_{+}^{\uparrow }}  [{\displaystyle {\mathcal {L}}_{+}^{\uparrow }}],
L    +     {\displaystyle {\mathcal {L}}_{+}}  [{\mathcal {L}}_{+}],        L
&#x2191;     {\displaystyle {\mathcal {L}}^{\uparrow }}  [{\displaystyle
{\mathcal {L}}^{\uparrow }}], and        L    0   =    L    +   &#x2191;
&#x222A;    L    &#x2212;   &#x2193;     {\displaystyle {\mathcal {L}}_{0}=
{\mathcal {L}}_{+}^{\uparrow }\cup {\mathcal {L}}_{-}^{\downarrow }}  [
{\mathcal {L}}_{0}={\mathcal {L}}_{+}^{\uparrow }\cup {\mathcal {L}}_{-}^
{\downarrow }] all form subgroups. The other sets involving the improper and/or
antichronous properties (i.e.        L    +   &#x2193;     {\displaystyle
{\mathcal {L}}_{+}^{\downarrow }}  [{\displaystyle {\mathcal {L}}_{+}^
{\downarrow }}],        L    &#x2212;   &#x2193;     {\displaystyle {\mathcal
{L}}_{-}^{\downarrow }}  [{\displaystyle {\mathcal {L}}_{-}^{\downarrow }}],
L    &#x2212;   &#x2191;     {\displaystyle {\mathcal {L}}_{-}^{\uparrow }}  [
{\displaystyle {\mathcal {L}}_{-}^{\uparrow }}]) do not form subgroups, because
the composite transformation always has a positive determinant or inequality,
whereas the original separate transformations will have negative determinants
and/or inequalities.
**** Proper transformations[edit] ****
The Lorentz boost is
          X &#x2032;  = B (  v  ) X   {\displaystyle X'=B(\mathbf {v} )X}
      [X'=B(\mathbf {v} )X]
where the boost matrix is
         B (  v  ) =   [    &#x03B3;   &#x2212; &#x03B3; &#x03B2;  n  x
      &#x2212; &#x03B3; &#x03B2;  n  y     &#x2212; &#x03B3; &#x03B2;  n  z
      &#x2212; &#x03B3; &#x03B2;  n  x     1 + ( &#x03B3; &#x2212; 1 )  n  x
      2     ( &#x03B3; &#x2212; 1 )  n  x    n  y     ( &#x03B3; &#x2212; 1 )
      n  x    n  z       &#x2212; &#x03B3; &#x03B2;  n  y     ( &#x03B3;
      &#x2212; 1 )  n  y    n  x     1 + ( &#x03B3; &#x2212; 1 )  n  y   2
      ( &#x03B3; &#x2212; 1 )  n  y    n  z       &#x2212; &#x03B3; &#x03B2;  n
      z     ( &#x03B3; &#x2212; 1 )  n  z    n  x     ( &#x03B3; &#x2212; 1 )
      n  z    n  y     1 + ( &#x03B3; &#x2212; 1 )  n  z   2      ]    .
      {\displaystyle B(\mathbf {v} )={\begin{bmatrix}\gamma &-\gamma \beta n_
      {x}&-\gamma \beta n_{y}&-\gamma \beta n_{z}\\-\gamma \beta n_{x}&1+
      (\gamma -1)n_{x}^{2}&(\gamma -1)n_{x}n_{y}&(\gamma -1)n_{x}n_{z}\\-\gamma
      \beta n_{y}&(\gamma -1)n_{y}n_{x}&1+(\gamma -1)n_{y}^{2}&(\gamma -1)n_
      {y}n_{z}\\-\gamma \beta n_{z}&(\gamma -1)n_{z}n_{x}&(\gamma -1)n_{z}n_
      {y}&1+(\gamma -1)n_{z}^{2}\\\end{bmatrix}}\,.}  [{\displaystyle B(\mathbf
      {v} )={\begin{bmatrix}\gamma &-\gamma \beta n_{x}&-\gamma \beta n_{y}&-
      \gamma \beta n_{z}\\-\gamma \beta n_{x}&1+(\gamma -1)n_{x}^{2}&(\gamma -
      1)n_{x}n_{y}&(\gamma -1)n_{x}n_{z}\\-\gamma \beta n_{y}&(\gamma -1)n_
      {y}n_{x}&1+(\gamma -1)n_{y}^{2}&(\gamma -1)n_{y}n_{z}\\-\gamma \beta n_
      {z}&(\gamma -1)n_{z}n_{x}&(\gamma -1)n_{z}n_{y}&1+(\gamma -1)n_{z}^
      {2}\\\end{bmatrix}}\,.}]
The boosts along the Cartesian directions can be readily obtained, for example
the unit vector in the x direction has components nx = 1 and ny = nz = 0.
The matrices make one or more successive transformations easier to handle,
rather than rotely iterating the transformations to obtain the result of more
than one transformation. If a frame F′ is boosted with velocity u relative to
frame F, and another frame F′′ is boosted with velocity v relative to F′, the
separate boosts are
          X &#x2033;  = B (  v  )  X &#x2032;   ,   X &#x2032;  = B (  u  ) X
      {\displaystyle X''=B(\mathbf {v} )X'\,,\quad X'=B(\mathbf {u} )X}  [
      {\displaystyle X''=B(\mathbf {v} )X'\,,\quad X'=B(\mathbf {u} )X}]
and the composition of the two boosts connects the coordinates in F′′ and F,
          X &#x2033;  = B (  v  ) B (  u  ) X  .   {\displaystyle X''=B(\mathbf
      {v} )B(\mathbf {u} )X\,.}  [{\displaystyle X''=B(\mathbf {v} )B(\mathbf
      {u} )X\,.}]
Successive transformations act on the left. If u and v are collinear (parallel
or antiparallel along the same line of relative motion), the boost matrices
commute: B(v)B(u) = B(u)B(v) and this composite transformation happens to be
another boost.
If u and v are not collinear but in different directions, the situation is
considerably more complicated. Lorentz boosts along different directions do not
commute: B(v)B(u) and B(u)B(v) are not equal. Also, each of these compositions
is not a single boost, but still a Lorentz transformation as each boost still
preserves invariance of the spacetime interval. It turns out the composition of
any two Lorentz boosts is equivalent to a boost followed or preceded by a
rotation on the spatial coordinates, in the form of R(Ï)B(w) or B(w)R(Ï). The
w and w are composite_velocities, while Ï and Ï are rotation parameters (e.g.
axis-angle variables, Euler_angles, etc.). The rotation in block_matrix form is
simply
          R (  &#x03C1;  ) =   [    1   0     0    R  (  &#x03C1;  )    ]    ,
      {\displaystyle \quad R({\boldsymbol {\rho }})={\begin
      {bmatrix}1&0\\0&\mathbf {R} ({\boldsymbol {\rho }})\end{bmatrix}}\,,}  [
      {\displaystyle \quad R({\boldsymbol {\rho }})={\begin
      {bmatrix}1&0\\0&\mathbf {R} ({\boldsymbol {\rho }})\end{bmatrix}}\,,}]
where R(Ï) is a 3d rotation_matrix, which rotates any 3d vector in one sense
(active transformation), or equivalently the coordinate frame in the opposite
sense (passive transformation). It is not simple to connect w and Ï (or w and
Ï) to the original boost parameters u and v. In a composition of boosts, the R
matrix is named the Wigner_rotation, and gives rise to the Thomas_precession.
These articles give the explicit formulae for the composite transformation
matrices, including expressions for w, Ï, w, Ï.
In this article the axis-angle_representation is used for Ï. The rotation is
about an axis in the direction of a unit_vector e, through angle Î¸ (positive
anticlockwise, negative clockwise, according to the right-hand_rule). The
"axis-angle vector"
          &#x03B8;  = &#x03B8;  e    {\displaystyle {\boldsymbol {\theta
      }}=\theta \mathbf {e} }  [{\displaystyle {\boldsymbol {\theta }}=\theta
      \mathbf {e} }]
will serve as a useful abbreviation.
Spatial rotations alone are also Lorentz transformations they leave the
spacetime interval invariant. Like boosts, successive rotations about different
axes do not commute. Unlike boosts, the composition of any two rotations is
equivalent to a single rotation. Some other similarities and differences
between the boost and rotation matrices include:
    * inverses: B(v)â1 = B(âv) (relative motion in the opposite direction),
      and R(Î¸)â1 = R(âÎ¸) (rotation in the opposite sense about the same
      axis)
    * identity_transformation for no relative motion/rotation: B(0) = R(0) = I
    * unit determinant: det(B) = det(R) = +1. This property makes them proper
      transformations.
    * matrix_symmetry: B is symmetric (equals transpose), while R is
      nonsymmetric but orthogonal (transpose equals inverse, RT = Râ1).
The most general proper Lorentz transformation Î(v, Î¸) includes a boost and
rotation together, and is a nonsymmetric matrix. As special cases, Î(0, Î¸) =
R(Î¸) and Î(v, 0) = B(v). An explicit form of the general Lorentz
transformation is cumbersome to write down and will not be given here.
Nevertheless, closed form expressions for the transformation matrices will be
given below using group theoretical arguments. It will be easier to use the
rapidity parametrization for boosts, in which case one writes Î(Î¶, Î¸) and B
(Î¶).
*** The Lie group SO+(3,1)[edit] ***
The set of transformations
         { B (  &#x03B6;  ) , R (  &#x03B8;  ) , &#x039B; (  &#x03B6;  ,
      &#x03B8;  ) }   {\displaystyle \{B({\boldsymbol {\zeta }}),R({\boldsymbol
      {\theta }}),\Lambda ({\boldsymbol {\zeta }},{\boldsymbol {\theta }})\}}
      [{\displaystyle \{B({\boldsymbol {\zeta }}),R({\boldsymbol {\theta
      }}),\Lambda ({\boldsymbol {\zeta }},{\boldsymbol {\theta }})\}}]
with matrix multiplication as the operation of composition forms a group,
called the "restricted Lorentz group", and is the special_indefinite_orthogonal
group SO+(3,1). (The plus sign indicates that it preserves the orientation of
the temporal dimension).
For simplicity, look at the infinitesimal Lorentz boost in the x direction
(examining a boost in any other direction, or rotation about any axis, follows
an identical procedure). The infinitesimal boost is a small boost away from the
identity, obtained by the Taylor_expansion of the boost matrix to first order
about Î¶ = 0,
          B  x   = I + &#x03B6;       &#x2202;  B  x     &#x2202; &#x03B6;    |
      &#x03B6; = 0   + &#x22EF;   {\displaystyle B_{x}=I+\zeta \left.{\frac
      {\partial B_{x}}{\partial \zeta }}\right|_{\zeta =0}+\cdots }  [
      {\displaystyle B_{x}=I+\zeta \left.{\frac {\partial B_{x}}{\partial \zeta
      }}\right|_{\zeta =0}+\cdots }]
where the higher order terms not shown are negligible because Î¶ is small, and
Bx is simply the boost matrix in the x direction. The derivative_of_the_matrix
is the matrix of derivatives (of the entries, with respect to the same
variable), and it is understood the derivatives are found first then evaluated
at Î¶ = 0,
               &#x2202;  B  x     &#x2202; &#x03B6;    |   &#x03B6; = 0   =
      &#x2212;  K  x    .   {\displaystyle \left.{\frac {\partial B_{x}}
      {\partial \zeta }}\right|_{\zeta =0}=-K_{x}\,.}  [{\displaystyle \left.
      {\frac {\partial B_{x}}{\partial \zeta }}\right|_{\zeta =0}=-K_{x}\,.}]
For now, Kx is defined by this result (its significance will be explained
shortly). In the limit of an infinite number of infinitely small steps, the
finite boost transformation in the form of a matrix_exponential is obtained
          B  x   =  lim  N &#x2192; &#x221E;     (  I &#x2212;   &#x03B6; N
      K  x    )   N   =  e  &#x2212; &#x03B6;  K  x       {\displaystyle B_
      {x}=\lim _{N\rightarrow \infty }\left(I-{\frac {\zeta }{N}}K_{x}\right)^
      {N}=e^{-\zeta K_{x}}}  [{\displaystyle B_{x}=\lim _{N\rightarrow \infty
      }\left(I-{\frac {\zeta }{N}}K_{x}\right)^{N}=e^{-\zeta K_{x}}}]
where the limit_definition_of_the_exponential has been used (see also
characterizations_of_the_exponential_function). More generally[nb_5]
         B (  &#x03B6;  ) =  e  &#x2212;  &#x03B6;  &#x22C5;  K     ,  R
      (  &#x03B8;  ) =  e   &#x03B8;  &#x22C5;  J     .   {\displaystyle B(
      {\boldsymbol {\zeta }})=e^{-{\boldsymbol {\zeta }}\cdot \mathbf {K}
      }\,,\quad R({\boldsymbol {\theta }})=e^{{\boldsymbol {\theta }}\cdot
      \mathbf {J} }\,.}  [{\displaystyle B({\boldsymbol {\zeta }})=e^{-
      {\boldsymbol {\zeta }}\cdot \mathbf {K} }\,,\quad R({\boldsymbol {\theta
      }})=e^{{\boldsymbol {\theta }}\cdot \mathbf {J} }\,.}]
The axis-angle vector Î¸ and rapidity vector Î¶ are altogether six continuous
variables which make up the group parameters (in this particular
representation), and the generators of the group are K = (Kx, Ky, Kz) and J =
(Jx, Jy, Jz), each vectors of matrices with the explicit forms[nb_6]
          K  x   =   [    0   1   0   0     1   0   0   0     0   0   0   0
      0   0   0   0    ]    ,   K  y   =   [    0   0   1   0     0   0   0   0
      1   0   0   0     0   0   0   0    ]    ,   K  z   =   [    0   0   0   1
      0   0   0   0     0   0   0   0     1   0   0   0    ]     {\displaystyle
      K_{x}={\begin{bmatrix}0&1&0&0\\1&0&0&0\\0&0&0&0\\0&0&0&0\\\end
      {bmatrix}}\,,\quad K_{y}={\begin
      {bmatrix}0&0&1&0\\0&0&0&0\\1&0&0&0\\0&0&0&0\end{bmatrix}}\,,\quad K_{z}=
      {\begin{bmatrix}0&0&0&1\\0&0&0&0\\0&0&0&0\\1&0&0&0\end{bmatrix}}}  [
      {\displaystyle K_{x}={\begin
      {bmatrix}0&1&0&0\\1&0&0&0\\0&0&0&0\\0&0&0&0\\\end{bmatrix}}\,,\quad K_
      {y}={\begin{bmatrix}0&0&1&0\\0&0&0&0\\1&0&0&0\\0&0&0&0\end
      {bmatrix}}\,,\quad K_{z}={\begin
      {bmatrix}0&0&0&1\\0&0&0&0\\0&0&0&0\\1&0&0&0\end{bmatrix}}}]
          J  x   =   [    0   0   0   0     0   0   0   0     0   0   0
      &#x2212; 1     0   0   1   0    ]    ,   J  y   =   [    0   0   0   0
      0   0   0   1     0   0   0   0     0   &#x2212; 1   0   0    ]    ,   J
      z   =   [    0   0   0   0     0   0   &#x2212; 1   0     0   1   0   0
      0   0   0   0    ]     {\displaystyle J_{x}={\begin
      {bmatrix}0&0&0&0\\0&0&0&0\\0&0&0&-1\\0&0&1&0\\\end{bmatrix}}\,,\quad J_
      {y}={\begin{bmatrix}0&0&0&0\\0&0&0&1\\0&0&0&0\\0&-1&0&0\end
      {bmatrix}}\,,\quad J_{z}={\begin{bmatrix}0&0&0&0\\0&0&-
      1&0\\0&1&0&0\\0&0&0&0\end{bmatrix}}}  [{\displaystyle J_{x}={\begin
      {bmatrix}0&0&0&0\\0&0&0&0\\0&0&0&-1\\0&0&1&0\\\end{bmatrix}}\,,\quad J_
      {y}={\begin{bmatrix}0&0&0&0\\0&0&0&1\\0&0&0&0\\0&-1&0&0\end
      {bmatrix}}\,,\quad J_{z}={\begin{bmatrix}0&0&0&0\\0&0&-
      1&0\\0&1&0&0\\0&0&0&0\end{bmatrix}}}]
These are all defined in an analogous way to Kx above, although the minus signs
in the boost generators are conventional. Physically, the generators of the
Lorentz group correspond to important symmetries in spacetime: J are the
rotation generators which correspond to angular_momentum, and K are the boost
generators which correspond to the motion of the system in spacetime. The
derivative of any smooth curve C(t) with C(0) = I in the group depending on
some group parameter t with respect to that group parameter, evaluated at t =
0, serves as a definition of a corresponding group generator G, and this
reflects an infinitesimal transformation away from the identity. The smooth
curve can always be taken as an exponential as the exponential will always map
G smoothly back into the group via t â exp(tG) for all t; this curve will
yield G again when differentiated at t = 0.
Expanding the exponentials in their Taylor series obtains
         B (  &#x03B6;  ) = I &#x2212; sinh &#x2061; &#x03B6; (  n  &#x22C5;  K
      ) + ( cosh &#x2061; &#x03B6; &#x2212; 1 ) (  n  &#x22C5;  K   )  2
      {\displaystyle B({\boldsymbol {\zeta }})=I-\sinh \zeta (\mathbf {n} \cdot
      \mathbf {K} )+(\cosh \zeta -1)(\mathbf {n} \cdot \mathbf {K} )^{2}}  [
      {\displaystyle B({\boldsymbol {\zeta }})=I-\sinh \zeta (\mathbf {n} \cdot
      \mathbf {K} )+(\cosh \zeta -1)(\mathbf {n} \cdot \mathbf {K} )^{2}}]
         R (  &#x03B8;  ) = I + sin &#x2061; &#x03B8; (  e  &#x22C5;  J  ) +
      ( 1 &#x2212; cos &#x2061; &#x03B8; ) (  e  &#x22C5;  J   )  2    .
      {\displaystyle R({\boldsymbol {\theta }})=I+\sin \theta (\mathbf {e}
      \cdot \mathbf {J} )+(1-\cos \theta )(\mathbf {e} \cdot \mathbf {J} )^
      {2}\,.}  [{\displaystyle R({\boldsymbol {\theta }})=I+\sin \theta
      (\mathbf {e} \cdot \mathbf {J} )+(1-\cos \theta )(\mathbf {e} \cdot
      \mathbf {J} )^{2}\,.}]
which compactly reproduce the boost and rotation matrices as given in the
previous section.
It has been stated that the general proper Lorentz transformation is a product
of a boost and rotation. At the infinitesimal level the product
             &#x039B;    = ( I &#x2212;  &#x03B6;  &#x22C5;  K  + &#x22EF; )
      ( I +  &#x03B8;  &#x22C5;  J  + &#x22EF; )       = ( I +  &#x03B8;
      &#x22C5;  J  + &#x22EF; ) ( I &#x2212;  &#x03B6;  &#x22C5;  K  + &#x22EF;
      )       = I &#x2212;  &#x03B6;  &#x22C5;  K  +  &#x03B8;  &#x22C5;  J  +
      &#x22EF;       {\displaystyle {\begin{aligned}\Lambda &=(I-{\boldsymbol
      {\zeta }}\cdot \mathbf {K} +\cdots )(I+{\boldsymbol {\theta }}\cdot
      \mathbf {J} +\cdots )\\&=(I+{\boldsymbol {\theta }}\cdot \mathbf {J}
      +\cdots )(I-{\boldsymbol {\zeta }}\cdot \mathbf {K} +\cdots )\\&=I-
      {\boldsymbol {\zeta }}\cdot \mathbf {K} +{\boldsymbol {\theta }}\cdot
      \mathbf {J} +\cdots \end{aligned}}}  [{\displaystyle {\begin
      {aligned}\Lambda &=(I-{\boldsymbol {\zeta }}\cdot \mathbf {K} +\cdots )
      (I+{\boldsymbol {\theta }}\cdot \mathbf {J} +\cdots )\\&=(I+{\boldsymbol
      {\theta }}\cdot \mathbf {J} +\cdots )(I-{\boldsymbol {\zeta }}\cdot
      \mathbf {K} +\cdots )\\&=I-{\boldsymbol {\zeta }}\cdot \mathbf {K} +
      {\boldsymbol {\theta }}\cdot \mathbf {J} +\cdots \end{aligned}}}]
is commutative because only linear terms are required (products like (Î¸Â·J)
(Î¶Â·K) and (Î¶Â·K)(Î¸Â·J) count as higher order terms and are negligible).
Taking the limit as before leads to the finite transformation in the form of an
exponential
         &#x039B; (  &#x03B6;  ,  &#x03B8;  ) =  e  &#x2212;  &#x03B6;
      &#x22C5;  K  +  &#x03B8;  &#x22C5;  J    .   {\displaystyle \Lambda (
      {\boldsymbol {\zeta }},{\boldsymbol {\theta }})=e^{-{\boldsymbol {\zeta
      }}\cdot \mathbf {K} +{\boldsymbol {\theta }}\cdot \mathbf {J} }.}  [
      {\displaystyle \Lambda ({\boldsymbol {\zeta }},{\boldsymbol {\theta
      }})=e^{-{\boldsymbol {\zeta }}\cdot \mathbf {K} +{\boldsymbol {\theta
      }}\cdot \mathbf {J} }.}]
The converse is also true, but the decomposition of a finite general Lorentz
transformation into such factors is nontrivial. In particular,
          e  &#x2212;  &#x03B6;  &#x22C5;  K  +  &#x03B8;  &#x22C5;  J
      &#x2260;  e  &#x2212;  &#x03B6;  &#x22C5;  K     e   &#x03B8;  &#x22C5;
      J    ,   {\displaystyle e^{-{\boldsymbol {\zeta }}\cdot \mathbf {K} +
      {\boldsymbol {\theta }}\cdot \mathbf {J} }\neq e^{-{\boldsymbol {\zeta
      }}\cdot \mathbf {K} }e^{{\boldsymbol {\theta }}\cdot \mathbf {J} },}  [
      {\displaystyle e^{-{\boldsymbol {\zeta }}\cdot \mathbf {K} +{\boldsymbol
      {\theta }}\cdot \mathbf {J} }\neq e^{-{\boldsymbol {\zeta }}\cdot \mathbf
      {K} }e^{{\boldsymbol {\theta }}\cdot \mathbf {J} },}]
because the generators do not commute. For a description of how to find the
factors of a general Lorentz transformation in terms of a boost and a rotation
in principle (this usually does not yield an intelligible expression in terms
of generators J and K), see Wigner_rotation. If, on the other hand, the
decomposition is given in terms of the generators, and one wants to find the
product in terms of the generators, then the Baker–Campbell–Hausdorff_formula
applies.
*** The Lie algebra so(3,1)[edit] ***
Lorentz generators can be added together, or multiplied by real numbers, to
obtain more Lorentz generators. In other words, the set of all Lorentz
generators
         V = {  &#x03B6;  &#x22C5;  K  +  &#x03B8;  &#x22C5;  J  }
      {\displaystyle V=\{{\boldsymbol {\zeta }}\cdot \mathbf {K} +{\boldsymbol
      {\theta }}\cdot \mathbf {J} \}}  [V=\{{\boldsymbol {\zeta }}\cdot \mathbf
      {K} +{\boldsymbol {\theta }}\cdot \mathbf {J} \}]
together with the operations of ordinary matrix_addition and multiplication_of
a_matrix_by_a_number, forms a vector_space over the real numbers.[nb_7] The
generators Jx, Jy, Jz, Kx, Ky, Kz form a basis set of V, and the components of
the axis-angle and rapidity vectors, Î¸x, Î¸y, Î¸z, Î¶x, Î¶y, Î¶z, are the
coordinates of a Lorentz generator with respect to this basis.[nb_8]
Three of the commutation_relations of the Lorentz generators are
         [  J  x   ,  J  y   ] =  J  z    ,  [  K  x   ,  K  y   ] = &#x2212;
      J  z    ,  [  J  x   ,  K  y   ] =  K  z    ,   {\displaystyle [J_{x},J_
      {y}]=J_{z}\,,\quad [K_{x},K_{y}]=-J_{z}\,,\quad [J_{x},K_{y}]=K_{z}\,,}
      [{\displaystyle [J_{x},J_{y}]=J_{z}\,,\quad [K_{x},K_{y}]=-J_{z}\,,\quad
      [J_{x},K_{y}]=K_{z}\,,}]
where the bracket [A, B] = AB â BA is known as the commutator, and the other
relations can be found by taking cyclic_permutations of x, y, z components
(i.e. change x to y, y to z, and z to x, repeat).
These commutation relations, and the vector space of generators, fulfill the
definition of the Lie_algebra       s o   ( 3 , 1 )   {\displaystyle {\mathfrak
{so}}(3,1)}  [{\displaystyle {\mathfrak {so}}(3,1)}]. In summary, a Lie algebra
is defined as a vector_space V over a field of numbers, and with a binary
operation [ , ] (called a Lie_bracket in this context) on the elements of the
vector space, satisfying the axioms of bilinearity, alternatization, and the
Jacobi_identity. Here the operation [ , ] is the commutator which satisfies all
of these axioms, the vector space is the set of Lorentz generators V as given
previously, and the field is the set of real numbers.
Linking terminology used in mathematics and physics: A group generator is any
element of the Lie algebra. A group parameter is a component of a coordinate
vector representing an arbitrary element of the Lie algebra with respect to
some basis. A basis, then, is a set of generators being a basis of the Lie
algebra in the usual vector space sense.
The exponential_map from the Lie algebra to the Lie group,
          e x p   :    s o   ( 3 , 1 ) &#x2192;  S O  ( 3 , 1 ) ,
      {\displaystyle \mathrm {exp} \,:\,{\mathfrak {so}}(3,1)\rightarrow
      \mathrm {SO} (3,1),}  [\mathrm {exp} \,:\,{\mathfrak {so}}
      (3,1)\rightarrow \mathrm {SO} (3,1),]
provides a one-to-one correspondence between small enough neighborhoods of the
origin of the Lie algebra and neighborhoods of the identity element of the Lie
group. It the case of the Lorentz group, the exponential map is just the matrix
exponential. Globally, the exponential map is not one-to-one, but in the case
of the Lorentz group, it is surjective (onto). Hence any group element in the
connected component of the identity can be expressed as an exponential of an
element of the Lie algebra.
**** Improper transformations[edit] ****
Lorentz transformations also include parity_inversion
         P =   [    1   0     0   &#x2212;  I     ]     {\displaystyle P=
      {\begin{bmatrix}1&0\\0&-\mathbf {I} \end{bmatrix}}}  [{\displaystyle P=
      {\begin{bmatrix}1&0\\0&-\mathbf {I} \end{bmatrix}}}]
which negates all the spatial coordinates only, and time_reversal
         T =   [    &#x2212; 1   0     0    I     ]     {\displaystyle T=
      {\begin{bmatrix}-1&0\\0&\mathbf {I} \end{bmatrix}}}  [{\displaystyle T=
      {\begin{bmatrix}-1&0\\0&\mathbf {I} \end{bmatrix}}}]
which negates the time coordinate only, because these transformations leave the
spacetime interval invariant. Here I is the 3d identity_matrix. These are both
symmetric, they are their own inverses (see involution_(mathematics)), and each
have determinant â1. This latter property makes them improper
transformations.
If Î is a proper orthochronous Lorentz transformation, then TÎ is improper
antichronous, PÎ is improper orthochronous, and TPÎ = PTÎ is proper
antichronous.
**** Inhomogeneous Lorentz group[edit] ****
Two other spacetime symmetries have not been accounted for. For the spacetime
interval to be invariant, it can be shown[16] that it is necessary and
sufficient for the coordinate transformation to be of the form
          X &#x2032;  = &#x039B; X + C   {\displaystyle X'=\Lambda X+C}
      [X'=\Lambda X+C]
where C is a constant column containing translations in time and space. If C
â  0, this is an inhomogeneous Lorentz transformation or PoincarÃ©
transformation.[17][18] If C = 0, this is a homogeneous Lorentz transformation.
PoincarÃ© transformations are not dealt further in this article.
***** Tensor formulation[edit] *****
Main article: Representation_theory_of_the_Lorentz_group
For the notation used, see Ricci_calculus.
**** Contravariant vectors[edit] ****
Writing the general matrix transformation of coordinates as the matrix equation
           [       x &#x2032;    0          x &#x2032;    1          x &#x2032;
      2          x &#x2032;    3      ]   =   [       &#x039B;  0     0
      &#x039B;  0     1        &#x039B;  0     2        &#x039B;  0     3
      &#x039B;  1     0        &#x039B;  1     1        &#x039B;  1     2
      &#x039B;  1     3          &#x039B;  2     0        &#x039B;  2     1
      &#x039B;  2     2        &#x039B;  2     3          &#x039B;  3     0
      &#x039B;  3     1        &#x039B;  3     2        &#x039B;  3     3
      ]     [     x  0        x  1        x  2        x  3      ]
      {\displaystyle {\begin{bmatrix}{x'}^{0}\\{x'}^{1}\\{x'}^{2}\\{x'}^{3}\end
      {bmatrix}}={\begin{bmatrix}{\Lambda ^{0}}_{0}&{\Lambda ^{0}}_{1}&{\Lambda
      ^{0}}_{2}&{\Lambda ^{0}}_{3}\\{\Lambda ^{1}}_{0}&{\Lambda ^{1}}_{1}&
      {\Lambda ^{1}}_{2}&{\Lambda ^{1}}_{3}\\{\Lambda ^{2}}_{0}&{\Lambda ^{2}}_
      {1}&{\Lambda ^{2}}_{2}&{\Lambda ^{2}}_{3}\\{\Lambda ^{3}}_{0}&{\Lambda ^
      {3}}_{1}&{\Lambda ^{3}}_{2}&{\Lambda ^{3}}_{3}\\\end{bmatrix}}{\begin
      {bmatrix}x^{0}\\x^{1}\\x^{2}\\x^{3}\end{bmatrix}}}  [{\displaystyle
      {\begin{bmatrix}{x'}^{0}\\{x'}^{1}\\{x'}^{2}\\{x'}^{3}\end{bmatrix}}=
      {\begin{bmatrix}{\Lambda ^{0}}_{0}&{\Lambda ^{0}}_{1}&{\Lambda ^{0}}_{2}&
      {\Lambda ^{0}}_{3}\\{\Lambda ^{1}}_{0}&{\Lambda ^{1}}_{1}&{\Lambda ^{1}}_
      {2}&{\Lambda ^{1}}_{3}\\{\Lambda ^{2}}_{0}&{\Lambda ^{2}}_{1}&{\Lambda ^
      {2}}_{2}&{\Lambda ^{2}}_{3}\\{\Lambda ^{3}}_{0}&{\Lambda ^{3}}_{1}&
      {\Lambda ^{3}}_{2}&{\Lambda ^{3}}_{3}\\\end{bmatrix}}{\begin{bmatrix}x^
      {0}\\x^{1}\\x^{2}\\x^{3}\end{bmatrix}}}]
allows the transformation of other physical quantities that cannot be expressed
as four-vectors; e.g., tensors or spinors of any order in 4d spacetime, to be
defined. In the corresponding tensor_index_notation, the above matrix
expression is
            x  &#x2032;     &#x03BD;   =    &#x039B;  &#x03BD;     &#x03BC;
      x  &#x03BC;   ,   {\displaystyle {x^{\prime }}^{\nu }={\Lambda ^{\nu }}_
      {\mu }x^{\mu },}  [{\displaystyle {x^{\prime }}^{\nu }={\Lambda ^{\nu }}_
      {\mu }x^{\mu },}]
where lower and upper indices label covariant_and_contravariant_components
respectively,[19] and the summation_convention is applied. It is a standard
convention to use Greek indices that take the value 0 for time components, and
1, 2, 3 for space components, while Latin indices simply take the values 1, 2,
3, for spatial components. Note that the first index (reading left to right)
corresponds in the matrix notation to a row index. The second index corresponds
to the column index.
The transformation matrix is universal for all four-vectors, not just 4-
dimensional spacetime coordinates. If A is any four-vector, then in tensor
index_notation
            A  &#x2032;     &#x03BD;   =    &#x039B;  &#x03BD;     &#x03BC;
      A  &#x03BC;    .   {\displaystyle {A^{\prime }}^{\nu }={\Lambda ^{\nu }}_
      {\mu }A^{\mu }\,.}  [{\displaystyle {A^{\prime }}^{\nu }={\Lambda ^{\nu
      }}_{\mu }A^{\mu }\,.}]
Alternatively, one writes
          A   &#x03BD; &#x2032;    =    &#x039B;   &#x03BD; &#x2032;
      &#x03BC;    A  &#x03BC;    .   {\displaystyle A^{\nu '}={\Lambda ^{\nu
      '}}_{\mu }A^{\mu }\,.}  [{\displaystyle A^{\nu '}={\Lambda ^{\nu '}}_{\mu
      }A^{\mu }\,.}]
in which the primed indices denote the indices of A in the primed frame. This
notation cuts risk of exhausting the Greek alphabet roughly in half.
For a general n-component object one may write
            X &#x2032;    &#x03B1;   =   &#x03A0; ( &#x039B;  )  &#x03B1;
      &#x03B2;    X  &#x03B2;    ,   {\displaystyle {X'}^{\alpha }={\Pi
      (\Lambda )^{\alpha }}_{\beta }X^{\beta }\,,}  [{\displaystyle {X'}^
      {\alpha }={\Pi (\Lambda )^{\alpha }}_{\beta }X^{\beta }\,,}]
where Î  is the appropriate representation_of_the_Lorentz_group, an nÃn matrix
for every Î. In this case, the indices should not be thought of as spacetime
indices (sometimes called Lorentz indices), and they run from 1 to n. E.g., if
X is a bispinor, then the indices are called Dirac indices.
**** Covariant vectors[edit] ****
There are also vector quantities with covariant indices. They are generally
obtained from their corresponding objects with contravariant indices by the
operation of lowering an index; e.g.,
          x  &#x03BD;   =  &#x03B7;  &#x03BC; &#x03BD;    x  &#x03BC;   ,
      {\displaystyle x_{\nu }=\eta _{\mu \nu }x^{\mu },}  [x_{\nu }=\eta _{\mu
      \nu }x^{\mu },]
where Î· is the metric_tensor. (The linked article also provides more
information about what the operation of raising and lowering indices really is
mathematically.) The inverse of this transformation is given by
          x  &#x03BC;   =  &#x03B7;  &#x03BC; &#x03BD;    x  &#x03BD;   ,
      {\displaystyle x^{\mu }=\eta ^{\mu \nu }x_{\nu },}  [{\displaystyle x^
      {\mu }=\eta ^{\mu \nu }x_{\nu },}]
where, when viewed as matrices, Î·Î¼Î½ is the inverse of Î·Î¼Î½. As it happens,
Î·Î¼Î½ = Î·Î¼Î½. This is referred to as raising an index. To transform a
covariant vector AÎ¼, first raise its index, then transform it according to the
same rule as for contravariant 4-vectors, then finally lower the index;
            A &#x2032;    &#x03BD;   =  &#x03B7;  &#x03C1; &#x03BD;
      &#x039B;  &#x03C1;     &#x03C3;    &#x03B7;  &#x03BC; &#x03C3;    A
      &#x03BC;   .   {\displaystyle {A'}_{\nu }=\eta _{\rho \nu }{\Lambda ^
      {\rho }}_{\sigma }\eta ^{\mu \sigma }A_{\mu }.}  [{\displaystyle {A'}_
      {\nu }=\eta _{\rho \nu }{\Lambda ^{\rho }}_{\sigma }\eta ^{\mu \sigma }A_
      {\mu }.}]
But
          &#x03B7;  &#x03C1; &#x03BD;      &#x039B;  &#x03C1;     &#x03C3;
      &#x03B7;  &#x03BC; &#x03C3;   =     (  &#x039B;  &#x2212; 1   )
      &#x03BC;     &#x03BD;   ,   {\displaystyle \eta _{\rho \nu }{\Lambda ^
      {\rho }}_{\sigma }\eta ^{\mu \sigma }={\left(\Lambda ^{-1}\right)^{\mu
      }}_{\nu },}  [{\displaystyle \eta _{\rho \nu }{\Lambda ^{\rho }}_{\sigma
      }\eta ^{\mu \sigma }={\left(\Lambda ^{-1}\right)^{\mu }}_{\nu },}]
I. e., it is the (Î¼, Î½)-component of the inverse Lorentz transformation. One
defines (as a matter of notation),
            &#x039B;  &#x03BD;     &#x03BC;   &#x2261;     (  &#x039B;
      &#x2212; 1   )   &#x03BC;     &#x03BD;   ,   {\displaystyle {\Lambda _
      {\nu }}^{\mu }\equiv {\left(\Lambda ^{-1}\right)^{\mu }}_{\nu },}  [
      {\displaystyle {\Lambda _{\nu }}^{\mu }\equiv {\left(\Lambda ^{-
      1}\right)^{\mu }}_{\nu },}]
and may in this notation write
            A &#x2032;    &#x03BD;   =    &#x039B;  &#x03BD;     &#x03BC;    A
      &#x03BC;   .   {\displaystyle {A'}_{\nu }={\Lambda _{\nu }}^{\mu }A_{\mu
      }.}  [{\displaystyle {A'}_{\nu }={\Lambda _{\nu }}^{\mu }A_{\mu }.}]
Now for a subtlety. The implied summation on the right hand side of
            A &#x2032;    &#x03BD;   =    &#x039B;  &#x03BD;     &#x03BC;    A
      &#x03BC;   =     (  &#x039B;  &#x2212; 1   )   &#x03BC;     &#x03BD;    A
      &#x03BC;     {\displaystyle {A'}_{\nu }={\Lambda _{\nu }}^{\mu }A_{\mu }=
      {\left(\Lambda ^{-1}\right)^{\mu }}_{\nu }A_{\mu }}  [{\displaystyle
      {A'}_{\nu }={\Lambda _{\nu }}^{\mu }A_{\mu }={\left(\Lambda ^{-1}\right)^
      {\mu }}_{\nu }A_{\mu }}]
is running over a row index of the matrix representing Îâ1. Thus, in terms
of matrices, this transformation should be thought of as the inverse transpose
of Î acting on the column vector AÎ¼. That is, in pure matrix notation,
          A &#x2032;  =   (  &#x039B;  &#x2212; 1   )    T    A .
      {\displaystyle A'=\left(\Lambda ^{-1}\right)^{\mathrm {T} }A.}  [
      {\displaystyle A'=\left(\Lambda ^{-1}\right)^{\mathrm {T} }A.}]
This means exactly that covariant vectors (thought of as column matrices)
transform according to the dual_representation of the standard representation
of the Lorentz group. This notion generalizes to general representations,
simply replace Î with Î (Î).
**** Tensors[edit] ****
If A and B are linear operators on vector spaces U and V, then a linear
operator A â B may be defined on the tensor_product of U and V, denoted U â
V according to[20]
         ( A &#x2297; B ) ( u &#x2297; v ) = A u &#x2297; B v ,  u &#x2208; U ,
      v &#x2208; V , u &#x2297; v &#x2208; U &#x2297; V .   {\displaystyle
      (A\otimes B)(u\otimes v)=Au\otimes Bv,\qquad u\in U,v\in V,u\otimes v\in
      U\otimes V.}  [(A\otimes B)(u\otimes v)=Au\otimes Bv,\qquad u\in U,v\in
      V,u\otimes v\in U\otimes V.]               (T1)
From this it is immediately clear that if u and v are a four-vectors in V, then
u â v â T2V â¡ V â V transforms as
         u &#x2297; v &#x2192; &#x039B; u &#x2297; &#x039B; v =    &#x039B;
      &#x03BC;     &#x03BD;    u  &#x03BD;   &#x2297;    &#x039B;  &#x03C1;
      &#x03C3;    v  &#x03C3;   =    &#x039B;  &#x03BC;     &#x03BD;
      &#x039B;  &#x03C1;     &#x03C3;    u  &#x03BD;   &#x2297;  v  &#x03C3;
      &#x2261;    &#x039B;  &#x03BC;     &#x03BD;      &#x039B;  &#x03C1;
      &#x03C3;    w  &#x03BD; &#x03C3;   .   {\displaystyle u\otimes
      v\rightarrow \Lambda u\otimes \Lambda v={\Lambda ^{\mu }}_{\nu }u^{\nu
      }\otimes {\Lambda ^{\rho }}_{\sigma }v^{\sigma }={\Lambda ^{\mu }}_{\nu }
      {\Lambda ^{\rho }}_{\sigma }u^{\nu }\otimes v^{\sigma }\equiv {\Lambda ^
      {\mu }}_{\nu }{\Lambda ^{\rho }}_{\sigma }w^{\nu \sigma }.}  [
      {\displaystyle u\otimes v\rightarrow \Lambda u\otimes \Lambda v={\Lambda
      ^{\mu }}_{\nu }u^{\nu }\otimes {\Lambda ^{\rho }}_{\sigma }v^{\sigma }=
      {\Lambda ^{\mu }}_{\nu }{\Lambda ^{\rho }}_{\sigma }u^{\nu }\otimes v^
      {\sigma }\equiv {\Lambda ^{\mu }}_{\nu }{\Lambda ^{\rho }}_{\sigma }w^
      {\nu \sigma }.}]               (T2)
The second step uses the bilinearity of the tensor product and the last step
defines a 2-tensor on component form, or rather, it just renames the tensor u
â v.
These observations generalize in an obvious way to more factors, and using the
fact that a general tensor on a vector space V can be written as a sum of a
coefficient (component!) times tensor products of basis vectors and basis
covectors, one arrives at the transformation law for any tensor quantity T. It
is given by[21]
          T   &#x03B8; &#x2032;   &#x03B9; &#x2032;  &#x22EF;  &#x03BA;
      &#x2032;     &#x03B1; &#x2032;   &#x03B2; &#x2032;  &#x22EF;  &#x03B6;
      &#x2032;    =    &#x039B;   &#x03B1; &#x2032;      &#x03BC;      &#x039B;
      &#x03B2; &#x2032;      &#x03BD;   &#x22EF;    &#x039B;   &#x03B6;
      &#x2032;      &#x03C1;      &#x039B;   &#x03B8; &#x2032;      &#x03C3;
      &#x039B;   &#x03B9; &#x2032;      &#x03C5;   &#x22EF;    &#x039B;
      &#x03BA; &#x2032;      &#x03B6;    T  &#x03C3; &#x03C5; &#x22EF; &#x03B6;
      &#x03BC; &#x03BD; &#x22EF; &#x03C1;   ,   {\displaystyle T_{\theta '\iota
      '\cdots \kappa '}^{\alpha '\beta '\cdots \zeta '}={\Lambda ^{\alpha '}}_
      {\mu }{\Lambda ^{\beta '}}_{\nu }\cdots {\Lambda ^{\zeta '}}_{\rho }
      {\Lambda _{\theta '}}^{\sigma }{\Lambda _{\iota '}}^{\upsilon }\cdots
      {\Lambda _{\kappa '}}^{\zeta }T_{\sigma \upsilon \cdots \zeta }^{\mu \nu
      \cdots \rho },}  [{\displaystyle T_{\theta '\iota '\cdots \kappa '}^
      {\alpha '\beta '\cdots \zeta '}={\Lambda ^{\alpha '}}_{\mu }{\Lambda ^
      {\beta '}}_{\nu }\cdots {\Lambda ^{\zeta '}}_{\rho }{\Lambda _{\theta
      '}}^{\sigma }{\Lambda _{\iota '}}^{\upsilon }\cdots {\Lambda _{\kappa
      '}}^{\zeta }T_{\sigma \upsilon \cdots \zeta }^{\mu \nu \cdots \rho },}]  
                  (T3)
where ÎÏ′Ï is defined above. This form can generally be reduced to the form
for general n-component objects given above with a single matrix (Î (Î))
operating on column vectors. This latter form is sometimes preferred; e.g., for
the electromagnetic field tensor.
*** Transformation of the electromagnetic field[edit] ***
Lorentz boost of an electric charge, the charge is at rest in one frame or the
other.
Main article: Electromagnetic_tensor
Further information: classical_electromagnetism_and_special_relativity
Lorentz transformations can also be used to illustrate that the magnetic_field
B and electric_field E are simply different aspects of the same force â the
electromagnetic_force, as a consequence of relative motion between electric
charges and observers.[22] The fact that the electromagnetic field shows
relativistic effects becomes clear by carrying out a simple thought experiment.
[23]
    * An observer measures a charge at rest in frame F. The observer will
      detect a static electric field. As the charge is stationary in this
      frame, there is no electric current, so the observer does not observe any
      magnetic field.
    * The other observer in frame Fâ² moves at velocity v relative to F and
      the charge. This observer sees a different electric field because the
      charge moves at velocity âv in their rest frame. The motion of the
      charge corresponds to an electric_current, and thus the observer in frame
      Fâ² also sees a magnetic field.
The electric and magnetic fields transform differently from space and time, but
exactly the same way as relativistic angular momentum and the boost vector.
The electromagnetic field strength tensor is given by
          F  &#x03BC; &#x03BD;   =   [    0   &#x2212;   1 c    E  x
      &#x2212;   1 c    E  y     &#x2212;   1 c    E  z         1 c    E  x
      0   &#x2212;  B  z      B  y         1 c    E  y      B  z     0
      &#x2212;  B  x         1 c    E  z     &#x2212;  B  y      B  x     0
      ]    (SI units, signature&#xA0;  ( + , &#x2212; , &#x2212; , &#x2212; )
      )  .   {\displaystyle F^{\mu \nu }={\begin{bmatrix}0&-{\frac {1}{c}}E_
      {x}&-{\frac {1}{c}}E_{y}&-{\frac {1}{c}}E_{z}\\{\frac {1}{c}}E_{x}&0&-B_
      {z}&B_{y}\\{\frac {1}{c}}E_{y}&B_{z}&0&-B_{x}\\{\frac {1}{c}}E_{z}&-B_
      {y}&B_{x}&0\end{bmatrix}}{\text{(SI units, signature }}(+,-,-,-){\text
      {)}}.}  [{\displaystyle F^{\mu \nu }={\begin{bmatrix}0&-{\frac {1}{c}}E_
      {x}&-{\frac {1}{c}}E_{y}&-{\frac {1}{c}}E_{z}\\{\frac {1}{c}}E_{x}&0&-B_
      {z}&B_{y}\\{\frac {1}{c}}E_{y}&B_{z}&0&-B_{x}\\{\frac {1}{c}}E_{z}&-B_
      {y}&B_{x}&0\end{bmatrix}}{\text{(SI units, signature }}(+,-,-,-){\text
      {)}}.}]
in SI_units. In relativity, the Gaussian_system_of_units is often preferred
over SI units, even in texts whose main choice of units is SI units, because in
it the electric field E and the magnetic induction B have the same units making
the appearance of the electromagnetic_field_tensor more natural.[24] Consider a
Lorentz boost in the x-direction. It is given by[25]
            &#x039B;  &#x03BC;     &#x03BD;   =   [    &#x03B3;   &#x2212;
      &#x03B3; &#x03B2;   0   0     &#x2212; &#x03B3; &#x03B2;   &#x03B3;   0
      0     0   0   1   0     0   0   0   1    ]   ,   F  &#x03BC; &#x03BD;   =
      [    0    E  x      E  y      E  z       &#x2212;  E  x     0    B  z
      &#x2212;  B  y       &#x2212;  E  y     &#x2212;  B  z     0    B  x
      &#x2212;  E  z      B  y     &#x2212;  B  x     0    ]    (Gaussian
      units, signature&#xA0;  ( &#x2212; , + , + , + )  )  ,   {\displaystyle
      {\Lambda ^{\mu }}_{\nu }={\begin{bmatrix}\gamma &-\gamma \beta &0&0\\-
      \gamma \beta &\gamma &0&0\\0&0&1&0\\0&0&0&1\\\end{bmatrix}},\qquad F^{\mu
      \nu }={\begin{bmatrix}0&E_{x}&E_{y}&E_{z}\\-E_{x}&0&B_{z}&-B_{y}\\-E_
      {y}&-B_{z}&0&B_{x}\\-E_{z}&B_{y}&-B_{x}&0\end{bmatrix}}{\text{(Gaussian
      units, signature }}(-,+,+,+){\text{)}},}  [{\displaystyle {\Lambda ^{\mu
      }}_{\nu }={\begin{bmatrix}\gamma &-\gamma \beta &0&0\\-\gamma \beta
      &\gamma &0&0\\0&0&1&0\\0&0&0&1\\\end{bmatrix}},\qquad F^{\mu \nu }=
      {\begin{bmatrix}0&E_{x}&E_{y}&E_{z}\\-E_{x}&0&B_{z}&-B_{y}\\-E_{y}&-B_
      {z}&0&B_{x}\\-E_{z}&B_{y}&-B_{x}&0\end{bmatrix}}{\text{(Gaussian units,
      signature }}(-,+,+,+){\text{)}},}]
where the field tensor is displayed side by side for easiest possible reference
in the manipulations below.
The general transformation law (T3) becomes
          F   &#x03BC; &#x2032;   &#x03BD; &#x2032;    =    &#x039B;   &#x03BC;
      &#x2032;      &#x03BC;      &#x039B;   &#x03BD; &#x2032;      &#x03BD;
      F  &#x03BC; &#x03BD;   .   {\displaystyle F^{\mu '\nu '}={\Lambda ^{\mu
      '}}_{\mu }{\Lambda ^{\nu '}}_{\nu }F^{\mu \nu }.}  [{\displaystyle F^{\mu
      '\nu '}={\Lambda ^{\mu '}}_{\mu }{\Lambda ^{\nu '}}_{\nu }F^{\mu \nu }.}]
For the magnetic field one obtains
              B   x &#x2032;       =  F   2 &#x2032;   3 &#x2032;    =
      &#x039B;  2     &#x03BC;      &#x039B;  3     &#x03BD;    F  &#x03BC;
      &#x03BD;   =    &#x039B;  2     2      &#x039B;  3     3    F  23   = 1
      &#x00D7; 1 &#x00D7;  B  x         =  B  x   ,      B   y &#x2032;       =
      F   3 &#x2032;   1 &#x2032;    =    &#x039B;  3     &#x03BC;
      &#x039B;  1     &#x03BD;    F  &#x03BC; &#x03BD;   =    &#x039B;  3     3
      &#x039B;  1     &#x03BD;    F  3 &#x03BD;   =    &#x039B;  3     3
      &#x039B;  1     0    F  30   +    &#x039B;  3     3      &#x039B;  1
      1    F  31         = 1 &#x00D7; ( &#x2212; &#x03B2; &#x03B3; ) ( &#x2212;
      E  z   ) + 1 &#x00D7; &#x03B3;  B  y   = &#x03B3;  B  y   + &#x03B2;
      &#x03B3;  E  z         = &#x03B3;   (   B  &#x2212;  &#x03B2;  &#x00D7;
      E   )   y        B   z &#x2032;       =  F   1 &#x2032;   2 &#x2032;    =
      &#x039B;  1     &#x03BC;      &#x039B;  2     &#x03BD;    F  &#x03BC;
      &#x03BD;   =    &#x039B;  1     &#x03BC;      &#x039B;  2     2    F
      &#x03BC; 2   =    &#x039B;  1     0      &#x039B;  2     2    F  02   +
      &#x039B;  1     1      &#x039B;  2     2    F  12         = ( &#x2212;
      &#x03B3; &#x03B2; ) &#x00D7; 1 &#x00D7;  E  y   + &#x03B3; &#x00D7; 1
      &#x00D7;  B  z   = &#x03B3;  B  z   &#x2212; &#x03B2; &#x03B3;  E  y
      = &#x03B3;   (   B  &#x2212;  &#x03B2;  &#x00D7;  E   )   z
      {\displaystyle {\begin{aligned}B_{x'}&=F^{2'3'}={\Lambda ^{2}}_{\mu }
      {\Lambda ^{3}}_{\nu }F^{\mu \nu }={\Lambda ^{2}}_{2}{\Lambda ^{3}}_{3}F^
      {23}=1\times 1\times B_{x}\\&=B_{x},\\B_{y'}&=F^{3'1'}={\Lambda ^{3}}_
      {\mu }{\Lambda ^{1}}_{\nu }F^{\mu \nu }={\Lambda ^{3}}_{3}{\Lambda ^{1}}_
      {\nu }F^{3\nu }={\Lambda ^{3}}_{3}{\Lambda ^{1}}_{0}F^{30}+{\Lambda ^
      {3}}_{3}{\Lambda ^{1}}_{1}F^{31}\\&=1\times (-\beta \gamma )(-E_
      {z})+1\times \gamma B_{y}=\gamma B_{y}+\beta \gamma E_{z}\\&=\gamma \left
      (\mathbf {B} -{\boldsymbol {\beta }}\times \mathbf {E} \right)_{y}\\B_
      {z'}&=F^{1'2'}={\Lambda ^{1}}_{\mu }{\Lambda ^{2}}_{\nu }F^{\mu \nu }=
      {\Lambda ^{1}}_{\mu }{\Lambda ^{2}}_{2}F^{\mu 2}={\Lambda ^{1}}_{0}
      {\Lambda ^{2}}_{2}F^{02}+{\Lambda ^{1}}_{1}{\Lambda ^{2}}_{2}F^{12}\\&=(-
      \gamma \beta )\times 1\times E_{y}+\gamma \times 1\times B_{z}=\gamma B_
      {z}-\beta \gamma E_{y}\\&=\gamma \left(\mathbf {B} -{\boldsymbol {\beta
      }}\times \mathbf {E} \right)_{z}\end{aligned}}}  [{\displaystyle {\begin
      {aligned}B_{x'}&=F^{2'3'}={\Lambda ^{2}}_{\mu }{\Lambda ^{3}}_{\nu }F^
      {\mu \nu }={\Lambda ^{2}}_{2}{\Lambda ^{3}}_{3}F^{23}=1\times 1\times B_
      {x}\\&=B_{x},\\B_{y'}&=F^{3'1'}={\Lambda ^{3}}_{\mu }{\Lambda ^{1}}_{\nu
      }F^{\mu \nu }={\Lambda ^{3}}_{3}{\Lambda ^{1}}_{\nu }F^{3\nu }={\Lambda ^
      {3}}_{3}{\Lambda ^{1}}_{0}F^{30}+{\Lambda ^{3}}_{3}{\Lambda ^{1}}_{1}F^
      {31}\\&=1\times (-\beta \gamma )(-E_{z})+1\times \gamma B_{y}=\gamma B_
      {y}+\beta \gamma E_{z}\\&=\gamma \left(\mathbf {B} -{\boldsymbol {\beta
      }}\times \mathbf {E} \right)_{y}\\B_{z'}&=F^{1'2'}={\Lambda ^{1}}_{\mu }
      {\Lambda ^{2}}_{\nu }F^{\mu \nu }={\Lambda ^{1}}_{\mu }{\Lambda ^{2}}_
      {2}F^{\mu 2}={\Lambda ^{1}}_{0}{\Lambda ^{2}}_{2}F^{02}+{\Lambda ^{1}}_
      {1}{\Lambda ^{2}}_{2}F^{12}\\&=(-\gamma \beta )\times 1\times E_
      {y}+\gamma \times 1\times B_{z}=\gamma B_{z}-\beta \gamma E_{y}\\&=\gamma
      \left(\mathbf {B} -{\boldsymbol {\beta }}\times \mathbf {E} \right)_
      {z}\end{aligned}}}]
For the electric field results
              E   x &#x2032;       =  F   0 &#x2032;   1 &#x2032;    =
      &#x039B;  0     &#x03BC;      &#x039B;  1     &#x03BD;    F  &#x03BC;
      &#x03BD;   =    &#x039B;  0     1      &#x039B;  1     0    F  10   +
      &#x039B;  0     0      &#x039B;  1     1    F  01         = ( &#x2212;
      &#x03B3; &#x03B2; ) ( &#x2212; &#x03B3; &#x03B2; ) ( &#x2212;  E  x   ) +
      &#x03B3; &#x03B3;  E  x   = &#x2212;  &#x03B3;  2    &#x03B2;  2   (  E
      x   ) +  &#x03B3;  2    E  x   =  E  x   ( 1 &#x2212;  &#x03B2;  2   )
      &#x03B3;  2         =  E  x   ,      E   y &#x2032;       =  F   0
      &#x2032;   2 &#x2032;    =    &#x039B;  0     &#x03BC;      &#x039B;  2
      &#x03BD;    F  &#x03BC; &#x03BD;   =    &#x039B;  0     &#x03BC;
      &#x039B;  2     2    F  &#x03BC; 2   =    &#x039B;  0     0      &#x039B;
      2     2    F  02   +    &#x039B;  0     1      &#x039B;  2     2    F  12
      = &#x03B3; &#x00D7; 1 &#x00D7;  E  y   + ( &#x2212; &#x03B2; &#x03B3; )
      &#x00D7; 1 &#x00D7;  B  z   = &#x03B3;  E  y   &#x2212; &#x03B2; &#x03B3;
      B  z         = &#x03B3;   (   E  +  &#x03B2;  &#x00D7;  B   )   y
      E   z &#x2032;       =  F   0 &#x2032;   3 &#x2032;    =    &#x039B;  0
      &#x03BC;      &#x039B;  3     &#x03BD;    F  &#x03BC; &#x03BD;   =
      &#x039B;  0     &#x03BC;      &#x039B;  3     3    F  &#x03BC; 3   =
      &#x039B;  0     0      &#x039B;  3     3    F  03   +    &#x039B;  0
      1      &#x039B;  3     3    F  13         = &#x03B3; &#x00D7; 1 &#x00D7;
      E  z   &#x2212; &#x03B2; &#x03B3; &#x00D7; 1 &#x00D7; ( &#x2212;  B  y
      ) = &#x03B3;  E  z   + &#x03B2; &#x03B3;  B  y         = &#x03B3;   (   E
      +  &#x03B2;  &#x00D7;  B   )   z   .       {\displaystyle {\begin
      {aligned}E_{x'}&=F^{0'1'}={\Lambda ^{0}}_{\mu }{\Lambda ^{1}}_{\nu }F^
      {\mu \nu }={\Lambda ^{0}}_{1}{\Lambda ^{1}}_{0}F^{10}+{\Lambda ^{0}}_{0}
      {\Lambda ^{1}}_{1}F^{01}\\&=(-\gamma \beta )(-\gamma \beta )(-E_
      {x})+\gamma \gamma E_{x}=-\gamma ^{2}\beta ^{2}(E_{x})+\gamma ^{2}E_
      {x}=E_{x}(1-\beta ^{2})\gamma ^{2}\\&=E_{x},\\E_{y'}&=F^{0'2'}={\Lambda ^
      {0}}_{\mu }{\Lambda ^{2}}_{\nu }F^{\mu \nu }={\Lambda ^{0}}_{\mu }
      {\Lambda ^{2}}_{2}F^{\mu 2}={\Lambda ^{0}}_{0}{\Lambda ^{2}}_{2}F^{02}+
      {\Lambda ^{0}}_{1}{\Lambda ^{2}}_{2}F^{12}\\&=\gamma \times 1\times E_
      {y}+(-\beta \gamma )\times 1\times B_{z}=\gamma E_{y}-\beta \gamma B_
      {z}\\&=\gamma \left(\mathbf {E} +{\boldsymbol {\beta }}\times \mathbf {B}
      \right)_{y}\\E_{z'}&=F^{0'3'}={\Lambda ^{0}}_{\mu }{\Lambda ^{3}}_{\nu
      }F^{\mu \nu }={\Lambda ^{0}}_{\mu }{\Lambda ^{3}}_{3}F^{\mu 3}={\Lambda ^
      {0}}_{0}{\Lambda ^{3}}_{3}F^{03}+{\Lambda ^{0}}_{1}{\Lambda ^{3}}_{3}F^
      {13}\\&=\gamma \times 1\times E_{z}-\beta \gamma \times 1\times (-B_
      {y})=\gamma E_{z}+\beta \gamma B_{y}\\&=\gamma \left(\mathbf {E} +
      {\boldsymbol {\beta }}\times \mathbf {B} \right)_{z}.\end{aligned}}}  [
      {\displaystyle {\begin{aligned}E_{x'}&=F^{0'1'}={\Lambda ^{0}}_{\mu }
      {\Lambda ^{1}}_{\nu }F^{\mu \nu }={\Lambda ^{0}}_{1}{\Lambda ^{1}}_{0}F^
      {10}+{\Lambda ^{0}}_{0}{\Lambda ^{1}}_{1}F^{01}\\&=(-\gamma \beta )(-
      \gamma \beta )(-E_{x})+\gamma \gamma E_{x}=-\gamma ^{2}\beta ^{2}(E_
      {x})+\gamma ^{2}E_{x}=E_{x}(1-\beta ^{2})\gamma ^{2}\\&=E_{x},\\E_
      {y'}&=F^{0'2'}={\Lambda ^{0}}_{\mu }{\Lambda ^{2}}_{\nu }F^{\mu \nu }=
      {\Lambda ^{0}}_{\mu }{\Lambda ^{2}}_{2}F^{\mu 2}={\Lambda ^{0}}_{0}
      {\Lambda ^{2}}_{2}F^{02}+{\Lambda ^{0}}_{1}{\Lambda ^{2}}_{2}F^
      {12}\\&=\gamma \times 1\times E_{y}+(-\beta \gamma )\times 1\times B_
      {z}=\gamma E_{y}-\beta \gamma B_{z}\\&=\gamma \left(\mathbf {E} +
      {\boldsymbol {\beta }}\times \mathbf {B} \right)_{y}\\E_{z'}&=F^{0'3'}=
      {\Lambda ^{0}}_{\mu }{\Lambda ^{3}}_{\nu }F^{\mu \nu }={\Lambda ^{0}}_
      {\mu }{\Lambda ^{3}}_{3}F^{\mu 3}={\Lambda ^{0}}_{0}{\Lambda ^{3}}_{3}F^
      {03}+{\Lambda ^{0}}_{1}{\Lambda ^{3}}_{3}F^{13}\\&=\gamma \times 1\times
      E_{z}-\beta \gamma \times 1\times (-B_{y})=\gamma E_{z}+\beta \gamma B_
      {y}\\&=\gamma \left(\mathbf {E} +{\boldsymbol {\beta }}\times \mathbf {B}
      \right)_{z}.\end{aligned}}}]
Here, Î² = (Î², 0, 0) is used. These results can be summarized by
               E    &#x2225; &#x2032;       =   E   &#x2225;         B
      &#x2225; &#x2032;       =   B   &#x2225;         E    &#x22A5; &#x2032;
      = &#x03B3;  (    E   &#x22A5;   +  &#x03B2;  &#x00D7;   B   &#x22A5;    )
      = &#x03B3;   (   E  +  &#x03B2;  &#x00D7;  B   )   &#x22A5;   ,       B
      &#x22A5; &#x2032;       = &#x03B3;  (    B   &#x22A5;   &#x2212;
      &#x03B2;  &#x00D7;   E   &#x22A5;    )  = &#x03B3;   (   B  &#x2212;
      &#x03B2;  &#x00D7;  E   )   &#x22A5;   ,       {\displaystyle {\begin
      {aligned}\mathbf {E} _{\parallel '}&=\mathbf {E} _{\parallel }\\\mathbf
      {B} _{\parallel '}&=\mathbf {B} _{\parallel }\\\mathbf {E} _{\bot
      '}&=\gamma \left(\mathbf {E} _{\bot }+{\boldsymbol {\beta }}\times
      \mathbf {B} _{\bot }\right)=\gamma \left(\mathbf {E} +{\boldsymbol {\beta
      }}\times \mathbf {B} \right)_{\bot },\\\mathbf {B} _{\bot '}&=\gamma
      \left(\mathbf {B} _{\bot }-{\boldsymbol {\beta }}\times \mathbf {E} _
      {\bot }\right)=\gamma \left(\mathbf {B} -{\boldsymbol {\beta }}\times
      \mathbf {E} \right)_{\bot },\end{aligned}}}  [{\displaystyle {\begin
      {aligned}\mathbf {E} _{\parallel '}&=\mathbf {E} _{\parallel }\\\mathbf
      {B} _{\parallel '}&=\mathbf {B} _{\parallel }\\\mathbf {E} _{\bot
      '}&=\gamma \left(\mathbf {E} _{\bot }+{\boldsymbol {\beta }}\times
      \mathbf {B} _{\bot }\right)=\gamma \left(\mathbf {E} +{\boldsymbol {\beta
      }}\times \mathbf {B} \right)_{\bot },\\\mathbf {B} _{\bot '}&=\gamma
      \left(\mathbf {B} _{\bot }-{\boldsymbol {\beta }}\times \mathbf {E} _
      {\bot }\right)=\gamma \left(\mathbf {B} -{\boldsymbol {\beta }}\times
      \mathbf {E} \right)_{\bot },\end{aligned}}}]
and are independent of the metric signature. For SI units, substitute E â
&#x200b;E⁄c. Misner,_Thorne_&_Wheeler_(1973) refer to this last form as the 3 +
1 view as opposed to the geometric view represented by the tensor expression
          F   &#x03BC; &#x2032;   &#x03BD; &#x2032;    =    &#x039B;   &#x03BC;
      &#x2032;      &#x03BC;      &#x039B;   &#x03BD; &#x2032;      &#x03BD;
      F  &#x03BC; &#x03BD;   ,   {\displaystyle F^{\mu '\nu '}={\Lambda ^{\mu
      '}}_{\mu }{\Lambda ^{\nu '}}_{\nu }F^{\mu \nu },}  [{\displaystyle F^{\mu
      '\nu '}={\Lambda ^{\mu '}}_{\mu }{\Lambda ^{\nu '}}_{\nu }F^{\mu \nu },}]
and make a strong point of the ease with which results that are difficult to
achieve using the 3 + 1 view can be obtained and understood. Only objects that
have well defined Lorentz transformation properties (in fact under any smooth
coordinate transformation) are geometric objects. In the geometric view, the
electromagnetic field is a six-dimensional geometric object in spacetime as
opposed to two interdependent, but separate, 3-vector fields in space and time.
The fields E (alone) and B (alone) do not have well defined Lorentz
transformation properties. The mathematical underpinnings are equations (T1)
and (T2) that immediately yield (T3). One should note that the primed and
unprimed tensors refer to the same event in spacetime. Thus the complete
equation with spacetime dependence is
          F   &#x03BC; &#x2032;   &#x03BD; &#x2032;     (  x &#x2032;  )  =
      &#x039B;   &#x03BC; &#x2032;      &#x03BC;      &#x039B;   &#x03BD;
      &#x2032;      &#x03BD;    F  &#x03BC; &#x03BD;    (   &#x039B;  &#x2212;
      1    x &#x2032;   )  =    &#x039B;   &#x03BC; &#x2032;      &#x03BC;
      &#x039B;   &#x03BD; &#x2032;      &#x03BD;    F  &#x03BC; &#x03BD;   ( x
      ) .   {\displaystyle F^{\mu '\nu '}\left(x'\right)={\Lambda ^{\mu '}}_
      {\mu }{\Lambda ^{\nu '}}_{\nu }F^{\mu \nu }\left(\Lambda ^{-1}x'\right)=
      {\Lambda ^{\mu '}}_{\mu }{\Lambda ^{\nu '}}_{\nu }F^{\mu \nu }(x).}  [
      {\displaystyle F^{\mu '\nu '}\left(x'\right)={\Lambda ^{\mu '}}_{\mu }
      {\Lambda ^{\nu '}}_{\nu }F^{\mu \nu }\left(\Lambda ^{-1}x'\right)=
      {\Lambda ^{\mu '}}_{\mu }{\Lambda ^{\nu '}}_{\nu }F^{\mu \nu }(x).}]
Length contraction has an effect on charge_density Ï and current_density J,
and time dilation has an effect on the rate of flow of charge (current), so
charge and current distributions must transform in a related way under a boost.
It turns out they transform exactly like the space-time and energy-momentum
four-vectors,
               j  &#x2032;     =  j  &#x2212; &#x03B3; &#x03C1; v  n  +
      (  &#x03B3; &#x2212; 1  )  (  j  &#x22C5;  n  )  n       &#x03C1;
      &#x2032;     = &#x03B3;  (  &#x03C1; &#x2212;  j  &#x22C5;    v  n    c
      2      )  ,       {\displaystyle {\begin{aligned}\mathbf {j} '&=\mathbf
      {j} -\gamma \rho v\mathbf {n} +\left(\gamma -1\right)(\mathbf {j} \cdot
      \mathbf {n} )\mathbf {n} \\\rho '&=\gamma \left(\rho -\mathbf {j} \cdot
      {\frac {v\mathbf {n} }{c^{2}}}\right),\end{aligned}}}  [{\displaystyle
      {\begin{aligned}\mathbf {j} '&=\mathbf {j} -\gamma \rho v\mathbf {n}
      +\left(\gamma -1\right)(\mathbf {j} \cdot \mathbf {n} )\mathbf {n} \\\rho
      '&=\gamma \left(\rho -\mathbf {j} \cdot {\frac {v\mathbf {n} }{c^
      {2}}}\right),\end{aligned}}}]
or, in the simpler geometric view,
          j   &#x03BC;  &#x2032;     =    &#x039B;   &#x03BC; &#x2032;
      &#x03BC;    j  &#x03BC;   .   {\displaystyle j^{\mu ^{\prime }}={\Lambda
      ^{\mu '}}_{\mu }j^{\mu }.}  [{\displaystyle j^{\mu ^{\prime }}={\Lambda ^
      {\mu '}}_{\mu }j^{\mu }.}]
One says that charge density transforms as the time component of a four-vector.
It is a rotational scalar. The current density is a 3-vector.
The Maxwell_equations are invariant under Lorentz transformations.
**** Spinors[edit] ****
Equation (T1) hold unmodified for any representation of the Lorentz group,
including the bispinor representation. In (T2) one simply replaces all
occurrences of Î by the bispinor representation Î (Î),
             u &#x2297; v &#x2192; &#x03A0; ( &#x039B; ) u &#x2297; &#x03A0;
      ( &#x039B; ) v    =   &#x03A0; ( &#x039B;  )  &#x03B1;     &#x03B2;    u
      &#x03B2;   &#x2297;   &#x03A0; ( &#x039B;  )  &#x03C1;     &#x03C3;    v
      &#x03C3;         =   &#x03A0; ( &#x039B;  )  &#x03B1;     &#x03B2;
      &#x03A0; ( &#x039B;  )  &#x03C1;     &#x03C3;    u  &#x03B2;   &#x2297;
      v  &#x03C3;         &#x2261;   &#x03A0; ( &#x039B;  )  &#x03B1;
      &#x03B2;     &#x03A0; ( &#x039B;  )  &#x03C1;     &#x03C3;    w  &#x03B1;
      &#x03B2;         {\displaystyle {\begin{aligned}u\otimes v\rightarrow \Pi
      (\Lambda )u\otimes \Pi (\Lambda )v&={\Pi (\Lambda )^{\alpha }}_{\beta }u^
      {\beta }\otimes {\Pi (\Lambda )^{\rho }}_{\sigma }v^{\sigma }\\&={\Pi
      (\Lambda )^{\alpha }}_{\beta }{\Pi (\Lambda )^{\rho }}_{\sigma }u^{\beta
      }\otimes v^{\sigma }\\&\equiv {\Pi (\Lambda )^{\alpha }}_{\beta }{\Pi
      (\Lambda )^{\rho }}_{\sigma }w^{\alpha \beta }\end{aligned}}}  [
      {\displaystyle {\begin{aligned}u\otimes v\rightarrow \Pi (\Lambda
      )u\otimes \Pi (\Lambda )v&={\Pi (\Lambda )^{\alpha }}_{\beta }u^{\beta
      }\otimes {\Pi (\Lambda )^{\rho }}_{\sigma }v^{\sigma }\\&={\Pi (\Lambda
      )^{\alpha }}_{\beta }{\Pi (\Lambda )^{\rho }}_{\sigma }u^{\beta }\otimes
      v^{\sigma }\\&\equiv {\Pi (\Lambda )^{\alpha }}_{\beta }{\Pi (\Lambda )^
      {\rho }}_{\sigma }w^{\alpha \beta }\end{aligned}}}]               (T4)
The above equation could, for instance, be the transformation of a state in
Fock_space describing two free electrons.
*** Transformation of general fields[edit] ***
A general noninteracting multi-particle state (Fock space state) in quantum
field_theory transforms according to the rule[26]
              U ( &#x039B; , a )  &#x03A8;   p  1    &#x03C3;  1
      n  1   ;  p  2    &#x03C3;  2    n  2   ; &#x22EF;       =
      e  &#x2212; i  a  &#x03BC;    [  ( &#x039B;  p  1    )
      &#x03BC;   + ( &#x039B;  p  2    )  &#x03BC;   + &#x22EF;  ]
      ( &#x039B;  p  1    )  0   ( &#x039B;  p  2    )  0
      &#x22EF;    p  1   0    p  2   0   &#x22EF;      (   &#x2211;
      &#x03C3;  1  &#x2032;   &#x03C3;  2  &#x2032;  &#x22EF;    D
      &#x03C3;  1  &#x2032;   &#x03C3;  1     (  j  1   )    [  W
      ( &#x039B; ,  p  1   )  ]   D   &#x03C3;  2  &#x2032;
      &#x03C3;  2     (  j  2   )    [  W ( &#x039B; ,  p  2   )  ]
      &#x22EF;  )   &#x03A8;  &#x039B;  p  1    &#x03C3;  1
      &#x2032;   n  1   ; &#x039B;  p  2    &#x03C3;  2  &#x2032;
      n  2   ; &#x22EF;   ,       {\displaystyle {\begin{aligned}&U
      (\Lambda ,a)\Psi _{p_{1}\sigma _{1}n_{1};p_{2}\sigma _{2}n_
      {2};\cdots }\\={}&e^{-ia_{\mu }\left[(\Lambda p_{1})^{\mu }+
      (\Lambda p_{2})^{\mu }+\cdots \right]}{\sqrt {\frac {(\Lambda    ( 1 )
      p_{1})^{0}(\Lambda p_{2})^{0}\cdots }{p_{1}^{0}p_{2}^            
      {0}\cdots }}}\left(\sum _{\sigma _{1}'\sigma _{2}'\cdots }D_
      {\sigma _{1}'\sigma _{1}}^{(j_{1})}\left[W(\Lambda ,p_
      {1})\right]D_{\sigma _{2}'\sigma _{2}}^{(j_{2})}\left[W
      (\Lambda ,p_{2})\right]\cdots \right)\Psi _{\Lambda p_
      {1}\sigma _{1}'n_{1};\Lambda p_{2}\sigma _{2}'n_{2};\cdots
      },\end{aligned}}}  [{\displaystyle {\begin{aligned}&U(\Lambda
      ,a)\Psi _{p_{1}\sigma _{1}n_{1};p_{2}\sigma _{2}n_{2};\cdots
      }\\={}&e^{-ia_{\mu }\left[(\Lambda p_{1})^{\mu }+(\Lambda p_
      {2})^{\mu }+\cdots \right]}{\sqrt {\frac {(\Lambda p_{1})^{0}
      (\Lambda p_{2})^{0}\cdots }{p_{1}^{0}p_{2}^{0}\cdots }}}\left
      (\sum _{\sigma _{1}'\sigma _{2}'\cdots }D_{\sigma _{1}'\sigma
      _{1}}^{(j_{1})}\left[W(\Lambda ,p_{1})\right]D_{\sigma _
      {2}'\sigma _{2}}^{(j_{2})}\left[W(\Lambda ,p_
      {2})\right]\cdots \right)\Psi _{\Lambda p_{1}\sigma _{1}'n_
      {1};\Lambda p_{2}\sigma _{2}'n_{2};\cdots },\end{aligned}}}]
where W(Î, p) is the Wigner_rotation and D(j) is the (2j + 1)-dimensional
representation of SO(3).
***** See also[edit] *****
    * Ricci_calculus
    * Electromagnetic_field
    * Galilean_transformation
    * Hyperbolic_rotation
    * Lorentz_group
    * Representation_theory_of_the_Lorentz_group
    * Principle_of_relativity
    * Velocity-addition_formula
    * Algebra_of_physical_space
    * Relativistic_aberration
    * PrandtlâGlauert_transformation
    * Split-complex_number
    * Gyrovector_space
***** Footnotes[edit] *****
   1. ^  One can imagine that in each inertial frame there are observers
      positioned throughout space, each with a synchronized clock and at rest
      in the particular inertial frame. These observers then report to a
      central office, where a report is collected. When one speaks of a
      particular observer, one refers to someone having, at least in principle,
      a copy of this report. See, e.g., Sard_(1970).
   2. ^ The separate requirements of the three equations lead to three
      different groups. The second equation is satisfied for spacetime
      translations in addition to Lorentz transformations leading to the
      PoincarÃ©_group or the inhomogeneous Lorentz group. The first equation
      (or the second restricted to lightlike separation) leads to a yet larger
      group, the conformal_group of spacetime.
   3. ^ The groups O(3, 1) and O(1, 3) are isomorphic. It is widely believed
      that the choice between the two metric signatures has no physical
      relevance, even though some objects related to O(3, 1) and O(1, 3)
      respectively, e.g., the Clifford_algebras corresponding to the different
      signatures of the bilinear form associated to the two groups, are non-
      isomorphic.
   4. ^ For two square matrices A and B, det(AB) = det(A)det(B)
   5. ^ Explicitly,
                &#x03B6;  &#x22C5;  K  =  &#x03B6;  x    K  x   +  &#x03B6;  y
            K  y   +  &#x03B6;  z    K  z     {\displaystyle {\boldsymbol
            {\zeta }}\cdot \mathbf {K} =\zeta _{x}K_{x}+\zeta _{y}K_{y}+\zeta _
            {z}K_{z}}  [{\displaystyle {\boldsymbol {\zeta }}\cdot \mathbf {K}
            =\zeta _{x}K_{x}+\zeta _{y}K_{y}+\zeta _{z}K_{z}}]
                &#x03B8;  &#x22C5;  J  =  &#x03B8;  x    J  x   +  &#x03B8;  y
            J  y   +  &#x03B8;  z    J  z     {\displaystyle {\boldsymbol
            {\theta }}\cdot \mathbf {J} =\theta _{x}J_{x}+\theta _{y}J_
            {y}+\theta _{z}J_{z}}  [{\displaystyle {\boldsymbol {\theta }}\cdot
            \mathbf {J} =\theta _{x}J_{x}+\theta _{y}J_{y}+\theta _{z}J_{z}}]
   6. ^ In quantum_mechanics, relativistic_quantum_mechanics, and quantum_field
      theory, a different convention is used for these matrices; the right hand
      sides are all multiplied by a factor of the imaginary unit i = √â1.
   7. ^ Until now the term "vector" has exclusively referred to "Euclidean
      vector", examples are position r, velocity v, etc. The term "vector"
      applies much more broadly than Euclidean vectors, row or column vectors,
      etc., see linear_algebra and vector_space for details. The generators of
      a Lie group also form a vector space over a field of numbers (e.g. real
      numbers, complex_numbers), since a linear_combination of the generators
      is also a generator. They just live in a different space to the position
      vectors in ordinary 3d space.
   8. ^ In ordinary 3d position_space, the position vector r = xex + yey + zez
      is expressed as a linear combination of the Cartesian unit vectors ex,
      ey, ez which form a basis, and the Cartesian coordinates x, y, z are
      coordinates with respect to this basis.
***** Notes[edit] *****
   1. ^ Forshaw_&_Smith_2009
   2. ^Cottingham, W. N.; Greenwood, D. A. (2007). An_Introduction_to_the
      Standard_Model_of_Particle_Physics (2nd ed.). Cambridge University Press.
      p. 21. ISBN 978-1-139-46221-1.
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
   4. Extract_of_page_21
   5. ^Lorentz, Hendrik Antoon (1904), "Electromagnetic_phenomena_in_a_system
      moving_with_any_velocity_smaller_than_that_of_light" , Proceedings of the
      Royal Netherlands Academy of Arts and Sciences, 6: 809â831
   6. ^ John_&_O'Connor_1996
   7. ^ Brown_2003
   8. ^ Rothman_2006, pp. 112f.
   9. ^ Darrigol_2005, pp. 1â22
  10. ^  Macrossan_1986, pp. 232â34
  11. ^ The reference is within the following paper:PoincarÃ©_1905,
      pp. 1504â1508
  12. ^ Einstein_1905, pp. 891â921
  13. ^ Young_&_Freedman_2008
  14. ^ Forshaw_&_Smith_2009
  15. ^ Einstein_1916
  16. ^ Barut_1964, p. 18â19
  17. ^ Chaichian_&_Hagedorn_1997, p. 239
  18. ^ Weinberg_1972
  19. ^ Weinberg_2005, pp. 55â58
  20. ^ Ohlsson_2011, p. 3â9
  21. ^Dennery, Philippe; Krzywicki, AndrÃ© (2012). Mathematics_for_Physicists.
      Courier Corporation. p. 138. ISBN 978-0-486-15712-2.
  22.  Extract_of_page_138
  23. ^ Hall_2003, Chapter 4
  24. ^ Carroll_2004, p. 22
  25. ^ Grant_&_Phillips_2008
  26. ^ Griffiths_2007
  27. ^ Jackson_1999
  28. ^ Misner,_Thorne_&_Wheeler_1973
  29. ^ Weinberg_2002, Chapter 3
***** References[edit] *****
**** Websites[edit] ****
    * O'Connor, John J.; Robertson, Edmund F. (1996), A_History_of_Special
      Relativity
Brown, Harvey R. (2003), Michelson,_FitzGerald_and_Lorentz:_the_Origins_of
Relativity_Revisited
**** Papers[edit] ****
    * Cushing, J. T. (1967). "Vector_Lorentz_transformations". American_Journal
      of_Physics. 35 (9): 858â862. Bibcode:1967AmJPh..35..858C. doi:10.1119/
      1.1974267.
Macfarlane, A. J. (1962). "On the Restricted Lorentz Group and Groups
Homomorphically Related to It". Journal_of_Mathematical_Physics. 3 (6):
1116â1129. Bibcode:1962JMP.....3.1116M. doi:10.1063/1.1703854.
Rothman, Tony (2006), "Lost_in_Einstein's_Shadow" (PDF), American Scientist, 94
(2): 112f
    * Darrigol, Olivier (2005), "The_Genesis_of_the_theory_of_relativity"
      (PDF), SÃ©minaire PoincarÃ©, 1: 1â22, doi:10.1007/3-7643-7436-5_1,
      ISBN 978-3-7643-7435-8
    * Macrossan, Michael N. (1986), "A_Note_on_Relativity_Before_Einstein",
      Brit. Journal Philos. Science, 37 (2): 232â34,
      CiteSeerX 10.1.1.679.5898, doi:10.1093/bjps/37.2.232
    * PoincarÃ©,_Henri (1905), "On_the_Dynamics_of_the_Electron" , Comptes
      Rendus Hebdomadaires des SÃ©ances de l'AcadÃ©mie des Sciences, 140:
      1504â1508
    * Einstein, Albert (1905), "Zur_Elektrodynamik_bewegter_KÃ¶rper" (PDF),
      Annalen der Physik, 322 (10): 891â921, Bibcode:1905AnP...322..891E,
      doi:10.1002/andp.19053221004
. See also: English_translation.
    * Einstein,_A. (1916). "Relativity:_The_Special_and_General_Theory" (PDF).
      Retrieved 2012-01-23.
Ungar, A. A. (1988). "Thomas rotation and the parameterization of the Lorentz
transformation group". Foundations of Physics Letters. 1 (1): 55â89. Bibcode:
1988FoPhL...1...57U. doi:10.1007/BF00661317. ISSN 0894-9875.
 eqn (55).
Ungar, A. A. (1989). "The_relativistic_velocity_composition_paradox_and_the
Thomas_rotation". Foundations_of_Physics. 19 (11): 1385â1396. Bibcode:
1989FoPh...19.1385U. doi:10.1007/BF00732759.
Ungar, A. A. (2000). "The relativistic composite-velocity reciprocity
principle". Foundations_of_Physics. 30 (2): 331â342.
CiteSeerX 10.1.1.35.1131.
Mocanu, C. I. (1986). "Some difficulties within the framework of relativistic
electrodynamics". Archiv fÃ¼r Elektrotechnik. 69 (2): 97â110. doi:10.1007/
bf01574845.
Mocanu, C. I. (1992). "On the relativistic velocity composition paradox and the
Thomas rotation". Foundations_of_Physics. 5 (5): 443â456. Bibcode:
1992FoPhL...5..443M. doi:10.1007/bf00690425.
Weinberg,_S. (2002). The Quantum Theory of Fields, vol I. Cambridge_University
Press. ISBN 978-0-521-55001-7.
**** Books[edit] ****
    * Young, H. D.; Freedman, R. A. (2008). University Physics â With Modern
      Physics (12th ed.). ISBN 978-0-321-50130-1.
Halpern, A. (1988). 3000 Solved Problems in Physics. Schaum Series. Mc Graw
Hill. p. 688. ISBN 978-0-07-025734-4.
Forshaw, J. R.; Smith, A. G. (2009). Dynamics and Relativity. Manchester
Physics Series. John Wiley & Sons Ltd. pp. 124â126. ISBN 978-0-470-01460-8.
Wheeler,_J._A.; Taylor,_E._F (1971). Spacetime Physics. Freeman. ISBN 978-0-
7167-0336-5.
Wheeler,_J._A.; Thorne,_K._S.; Misner,_C._W. (1973). Gravitation. Freeman.
ISBN 978-0-7167-0344-0.
Carroll,_S._M. (2004). Spacetime_and_Geometry:_An_Introduction_to_General
Relativity (illustrated ed.). Addison Wesley. p. 22. ISBN 978-0-8053-8732-2.
Grant, I. S.; Phillips, W. R. (2008). "14". Electromagnetism. Manchester
Physics (2nd ed.). John Wiley & Sons. ISBN 978-0-471-92712-9.
Griffiths,_D._J. (2007). Introduction to Electrodynamics (3rd ed.). Pearson
Education, Dorling Kindersley. ISBN 978-81-7758-293-2.
Hall, Brian C. (2003). Lie Groups, Lie Algebras, and Representations An
Elementary Introduction. Springer. ISBN 978-0-387-40122-5.
Weinberg,_S. (2008), Cosmology, Wiley, ISBN 978-0-19-852682-7
Weinberg,_S. (2005), The quantum theory of fields (3 vol.), 1, Cambridge
University Press, ISBN 978-0-521-67053-1
Ohlsson,_T. (2011), Relativistic Quantum Physics, Cambridge University Press,
ISBN 978-0-521-76726-2
Goldstein,_H. (1980) [1950]. Classical Mechanics (2nd ed.). Reading MA:
Addison-Wesley. ISBN 978-0-201-02918-5.
Jackson,_J._D. (1975) [1962]. "Chapter 11". Classical Electrodynamics (2nd
ed.). John_Wiley_&_Sons. pp. 542â545. ISBN 978-0-471-43132-9.
Landau,_L._D.; Lifshitz,_E._M. (2002) [1939]. The Classical Theory of Fields.
Course_of_Theoretical_Physics. 2 (4th ed.). Butterworth–Heinemann. pp. 9â12.
ISBN 0_7506_2768_9.
Feynman,_R._P.; Leighton,_R._B.; Sands,_M. (1977) [1963]. "15". The Feynman
Lectures on Physics. 1. Addison Wesley. ISBN 978-0-201-02117-2.
Feynman,_R._P.; Leighton,_R._B.; Sands,_M. (1977) [1964]. "13". The Feynman
Lectures on Physics. 2. Addison Wesley. ISBN 978-0-201-02117-2.
Misner,_Charles_W.; Thorne,_Kip_S.; Wheeler,_John_Archibald (1973).
Gravitation. San Francisco: W._H._Freeman. ISBN 978-0-7167-0344-0.
Rindler,_W. (2006) [2001]. "Chapter 9". Relativity Special, General and
Cosmological (2nd ed.). Dallas: Oxford_University_Press. ISBN 978-0-19-856732-
5.
Ryder,_L._H. (1996) [1985]. Quantum Field Theory (2nd ed.). Cambridge:
Cambridge_University_Press. ISBN 978-0521478144.
Sard, R. D. (1970). Relativistic Mechanics - Special Relativity and Classical
Particle Dynamics. New York: W. A. Benjamin. ISBN 978-0805384918.
R. U. Sexl, H. K. Urbantke (2001) [1992]. Relativity,_Groups_Particles._Special
Relativity_and_Relativistic_Symmetry_in_Field_and_Particle_Physics. Springer.
ISBN 978-3211834435.
Gourgoulhon, Eric (2013). Special_Relativity_in_General_Frames:_From_Particles
to_Astrophysics. Springer. p. 213. ISBN 978-3-642-37276-6.
Chaichian, Masud; Hagedorn, Rolf (1997). Symmetry_in_quantum_mechanics:From
angular_momentum_to_supersymmetry. IoP. p. 239. ISBN 978-0-7503-0408-5.
Landau,_L.D.; Lifshitz,_E.M. (2002) [1939]. The Classical Theory of Fields.
Course of Theoretical Physics. 2 (4th ed.). Butterworth–Heinemann. ISBN 0_7506
2768_9.
***** Further reading[edit] *****
    * Einstein,_Albert (1961), Relativity:_The_Special_and_the_General_Theory,
      New York: Three Rivers Press (published 1995), ISBN 978-0-517-88441-6
Ernst, A.; Hsu, J.-P. (2001), "First_proposal_of_the_universal_speed_of_light
by_Voigt_1887" (PDF), Chinese Journal of Physics, 39 (3): 211â230, Bibcode:
2001ChJPh..39..211E, archived from the_original (PDF) on 2011-07-16
Thornton, Stephen T.; Marion, Jerry B. (2004), Classical dynamics of particles
and systems (5th ed.), Belmont, [CA.]: Brooks/Cole, pp. 546â579, ISBN 978-0-
534-40896-1
Voigt,_Woldemar (1887), "Ãber das Doppler'sche princip", Nachrichten von der
KÃ¶niglicher Gesellschaft den Wissenschaft zu GÃ¶ttingen, 2: 41â51
***** External links[edit] *****
 Wikisource has original works on the topic: Relativity
 Wikibooks has a book on the topic of: special_relativity
    * Derivation_of_the_Lorentz_transformations. This web page contains a more
      detailed derivation of the Lorentz transformation with special emphasis
      on group properties.
    * The_Paradox_of_Special_Relativity. This webpage poses a problem, the
      solution of which is the Lorentz transformation, which is presented
      graphically in its next page.
    * Relativity â a chapter from an online textbook
    * Warp_Special_Relativity_Simulator. A computer program demonstrating the
      Lorentz transformations on everyday objects.
    * Animation_clip on YouTube visualizing the Lorentz transformation.
    * Lorentz_Frames_Animated from John de Pillis. Online Flash animations of
      Galilean and Lorentz frames, various paradoxes, EM wave phenomena, etc.
    * v
    * t
    * e
Relativity
                           * Principle_of_relativity (Galilean_relativity
           Background      * Galilean_transformation)
                           * Special_relativity
                           * Doubly_special_relativity
                           * Frame_of_reference
                           * Speed_of_light
                           * Hyperbolic_orthogonality
           Fundamental     * Rapidity
           concepts        * Maxwell's_equations
                           * Proper_length
                           * Proper_time
                           * Relativistic_mass
Special    Formulation     * Lorentz transformation
relativity                 * Time_dilation
                           * Massâenergy_equivalence
                           * Length_contraction
           Phenomena       * Relativity_of_simultaneity
                           * Relativistic_Doppler_effect
                           * Thomas_precession
                           * Ladder_paradox
                           * Twin_paradox
                           * Light_cone
                           * World_line
           Spacetime       * Minkowski_diagram
                           * Biquaternions
                           * Minkowski_space
           Background      * Introduction
                           * Mathematical_formulation
                           * Equivalence_principle
           Fundamental     * Riemannian_geometry
           concepts        * Penrose_diagram
                           * Geodesics
                           * Mach's_principle
                           * ADM_formalism
                           * BSSN_formalism
                           * Einstein_field_equations
           Formulation     * Linearized_gravity
                           * Post-Newtonian_formalism
                           * Raychaudhuri_equation
                           * HamiltonâJacobiâEinstein_equation
                           * Ernst_equation
                           * Black_hole
                           * Event_horizon
                           * Singularity
                           * Two-body_problem
                           * Gravitational_waves: astronomy
                           * detectors (LIGO and collaboration
                           * Virgo
           Phenomena       * LISA_Pathfinder
                           * GEO)
General                    * Hulse-Taylor_binary
relativity                 * Other_tests: precession of Mercury
                           * lensing                                                                                   [Spacetime
                           * redshift                                                                                  curvature.png]
                           * Shapiro_delay
                           * frame-dragging / geodetic_effect (Lense-Thirring_precession)
                           * pulsar_timing_arrays
           Advanced        * BransâDicke_theory
           theories        * KaluzaâKlein
                           * Quantum_gravity
                           * Cosmological: FriedmannâLemaÃ®treâRobertsonâWalker (Friedmann_equations)
                           * Kasner
                           * BKL_singularity
                           * GÃ¶del
                           * Milne
                           * Spherical: Schwarzschild (interior
                           * TolmanâOppenheimerâVolkoff_equation)
           Solutions       * ReissnerâNordstrÃ¶m
                           * LemaÃ®treâTolman
                           * Axisymmetric: Kerr (KerrâNewman)
                           * WeylâLewisâPapapetrou
                           * TaubâNUT
                           * van_Stockum_dust
                           * discs
                           * Others: pp-wave
                           * OzsvÃ¡thâSchÃ¼cking_metric
               * PoincarÃ©
               * Lorentz
               * Einstein
               * Hilbert
               * Schwarzschild
               * de_Sitter
               * Weyl
               * Eddington
               * Friedmann
               * LemaÃ®tre
               * Milne
               * Robertson
               * Chandrasekhar
               * Zwicky
               * Wheeler
Scientists     * Choquet-Bruhat
               * Kerr
               * Zel'dovich
               * Novikov
               * Ehlers
               * Geroch
               * Penrose
               * Hawking
               * Taylor
               * Hulse
               * Bondi
               * Misner
               * Yau
               * Thorne
               * Weiss
               * others

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Lorentz_transformation&oldid=909314312"
Categories:
    * Special_relativity
    * Theoretical_physics
    * Mathematical_physics
    * Spacetime
    * Coordinate_systems
    * Hendrik_Lorentz
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
    * Alemannisch
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * à¨ªà©°à¨à¨¾à¨¬à©
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Tagalog
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 4 August 2019, at 16:30 (UTC).
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
