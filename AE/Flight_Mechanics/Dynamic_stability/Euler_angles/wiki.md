The following text has been accessed from https://en.wikipedia.org/wiki/Euler_angles at Thu Aug 8 23:17:32 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Euler angles ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the Euler angles used in mathematics. For the use of the
term in physics and aerospace_engineering, see rigid_body_dynamics. For chained
rotations, see chained_rotations.
The Euler angles are three angles introduced by Leonhard_Euler to describe the
orientation of a rigid_body with respect to a fixed coordinate_system.[1] They
can also represent the orientation of a mobile frame_of_reference in physics or
the orientation of a general basis in 3-dimensional linear algebra.
Any orientation can be achieved by composing three elemental_rotations, i.e.,
rotations about the axes of a coordinate_system. Euler angles can be defined by
three of these rotations. They can also be defined by elemental geometry and
the geometrical definition demonstrates that three rotations are always
sufficient to reach any frame.
The three elemental rotations may be extrinsic (rotations about the axes xyz of
the original coordinate system, which is assumed to remain motionless), or
intrinsic (rotations about the axes of the rotating coordinate system XYZ,
solidary with the moving body, which changes its orientation after each
elemental rotation).
Euler angles are typically denoted as α, β, γ, or φ, θ, ψ. Different authors
may use different sets of rotation axes to define Euler angles, or different
names for the same angles. Therefore, any discussion employing Euler angles
should always be preceded by their definition.
Without considering the possibility of using two different conventions for the
definition of the rotation axes (intrinsic or extrinsic), there exist twelve
possible sequences of rotation axes, divided in two groups:
    * Proper Euler angles (z-x-z, x-y-x, y-z-y, z-y-z, x-z-x, y-x-y)
    * TaitâBryan angles (x-y-z, y-z-x, z-x-y, x-z-y, z-y-x, y-x-z).
TaitâBryan angles are also called Cardan angles; nautical angles; heading,
elevation, and bank; or yaw, pitch, and roll. Sometimes, both kinds of
sequences are called "Euler angles". In that case, the sequences of the first
group are called proper or classic Euler angles.
⁰
***** Contents *****
    * 1_Proper_Euler_angles
          o 1.1_Geometrical_definition
          o 1.2_Definition_by_intrinsic_rotations
          o 1.3_Definition_by_extrinsic_rotations
          o 1.4_Conventions
          o 1.5_Signs_and_ranges
          o 1.6_Precession,_nutation_and_intrinsic_rotation
    * 2_TaitâBryan_angles
          o 2.1_Definitions
          o 2.2_Conventions
          o 2.3_Signs_and_ranges
          o 2.4_Alternative_names
    * 3_Angles_of_a_given_frame
          o 3.1_Proper_Euler_angles
          o 3.2_TaitâBryan_angles
          o 3.3_Last_remarks
    * 4_Conversion_to_other_orientation_representations
          o 4.1_Rotation_matrix
    * 5_Properties
          o 5.1_Geometric_algebra
          o 5.2_Higher_dimensions
    * 6_Applications
          o 6.1_Vehicles_and_moving_frames
          o 6.2_Crystallographic_texture
          o 6.3_Others
    * 7_See_also
    * 8_References
    * 9_Bibliography
    * 10_External_links
***** Proper Euler angles[edit] *****
Proper Euler angles geometrical definition. The xyz (fixed) system is shown in
blue, the XYZ (rotated) system is shown in red. The line_of_nodes (N) is shown
in green
**** Geometrical definition[edit] ****
The axes of the original frame are denoted as x, y, z and the axes of the
rotated frame as X, Y, Z. The geometrical definition (sometimes referred to as
static) begins by defining the line_of_nodes as the intersection of the planes
xy and XY (it can also be defined as the common perpendicular to the axes z and
Z and then written as the vector product N = z     &#x00D7;   {\displaystyle
\times }  [\times ] Z). Using it, the three Euler angles can be defined as
follows:
    *    &#x03B1;   {\displaystyle \alpha }  [\alpha ] (or     &#x03C6;
      {\displaystyle \varphi }  [\varphi ]) is the angle between the x axis and
      the N axis (x-convention - it could also be defined between y and N,
      called y-convention).
    *    &#x03B2;   {\displaystyle \beta }  [\beta ] (or     &#x03B8;
      {\displaystyle \theta \,}  [\theta \,]) is the angle between the z axis
      and the Z axis.
    *    &#x03B3;   {\displaystyle \gamma }  [\gamma ] (or     &#x03C8;
      {\displaystyle \psi }  [\psi ]) is the angle between the N axis and the X
      axis (x-convention).
Euler angles between two reference frames are defined only if both frames have
the same handedness.
**** Definition by intrinsic rotations[edit] ****
Intrinsic rotations are elemental rotations that occur about the axes of a
coordinate system XYZ attached to a moving body. Therefore, they change their
orientation after each elemental rotation. The XYZ system rotates, while xyz is
fixed. Starting with XYZ overlapping xyz, a composition of three intrinsic
rotations can be used to reach any target orientation for XYZ.
Euler angles can be defined by intrinsic rotations. The rotated frame XYZ may
be imagined to be initially aligned with xyz, before undergoing the three
elemental rotations represented by Euler angles. Its successive orientations
may be denoted as follows:
    * x-y-z, or x0-y0-z0 (initial)
    * xâ²-yâ²-zâ², or x1-y1-z1 (after first rotation)
    * xâ³-yâ³-zâ³, or x2-y2-z2 (after second rotation)
    * X-Y-Z, or x3-y3-z3 (final)
For the above-listed sequence of rotations, the line_of_nodes N can be simply
defined as the orientation of X after the first elemental rotation. Hence, N
can be simply denoted xâ². Moreover, since the third elemental rotation occurs
about Z, it does not change the orientation of Z. Hence Z coincides with zâ³.
This allows us to simplify the definition of the Euler angles as follows:
    * Î± (or     &#x03C6;   {\displaystyle \varphi }  [\varphi ]) represents a
      rotation around the z axis,
    * Î² (or     &#x03B8;   {\displaystyle \theta }  [\theta ]) represents a
      rotation around the xâ² axis,
    * Î³ (or     &#x03C8;   {\displaystyle \psi }  [\psi ]) represents a
      rotation around the zâ³ axis.
**** Definition by extrinsic rotations[edit] ****
Extrinsic rotations are elemental rotations that occur about the axes of the
fixed coordinate system xyz. The XYZ system rotates, while xyz is fixed.
Starting with XYZ overlapping xyz, a composition of three extrinsic rotations
can be used to reach any target orientation for XYZ. The Euler or TaitâBryan
angles (Î±, Î², Î³) are the amplitudes of these elemental rotations. For
instance, the target orientation can be reached as follows:
    * The XYZ system rotates about the z axis by Î³. The X axis is now at angle
      Î³ with respect to the x axis.
    * The XYZ system rotates again about the x axis by Î². The Z axis is now at
      angle Î² with respect to the z axis.
    * The XYZ system rotates a third time about the z axis by Î±.
In sum, the three elemental rotations occur about z, x and z. Indeed, this
sequence is often denoted z-x-z (or 3-1-3). Sets of rotation axes associated
with both proper Euler angles and TaitâBryan angles are commonly named using
this notation (see above for details).
**** Conventions[edit] ****
There are six possibilities of choosing the rotation axes for proper Euler
angles. In all of them, the first and third rotation axes are the same. The six
possible sequences are:
   1. z1-xâ²-z2â³ (intrinsic rotations) or z2-x-z1 (extrinsic rotations)
   2. x1-yâ²-x2â³ (intrinsic rotations) or x2-y-x1 (extrinsic rotations)
   3. y1-zâ²-y2â³ (intrinsic rotations) or y2-z-y1 (extrinsic rotations)
   4. z1-yâ²-z2â³ (intrinsic rotations) or z2-y-z1 (extrinsic rotations)
   5. x1-zâ²-x2â³ (intrinsic rotations) or x2-z-x1 (extrinsic rotations)
   6. y1-xâ²-y2â³ (intrinsic rotations) or y2-x-y1 (extrinsic rotations)
**** Signs and ranges[edit] ****
Angles are commonly defined according to the right-hand_rule. Namely, they have
positive values when they represent a rotation that appears clockwise when
looking in the positive direction of the axis, and negative values when the
rotation appears counter-clockwise. The opposite convention (left hand rule) is
less frequently adopted.
About the ranges (using interval_notation):
    * for Î± and Î³, the range is defined modulo 2Ï radians. For instance, a
      valid range could be [−Ï,âÏ].
    * for Î², the range covers Ï radians (but can't be said to be modulo Ï).
      For example, it could be [0,âÏ] or [−Ï/2,âÏ/2].
The angles Î±, Î² and Î³ are uniquely determined except for the singular case
that the xy and the XY planes are identical, i.e. when the z axis and the Z
axis have the same or opposite directions. Indeed, if the z axis and the Z axis
are the same, Î² = 0 and only (Î± + Î³) is uniquely defined (not the individual
values), and, similarly, if the z axis and the Z axis are opposite, Î² = Ï and
only (Î± − Î³) is uniquely defined (not the individual values). These
ambiguities are known as gimbal_lock in applications.
**** Precession, nutation and intrinsic rotation[edit] ****
Euler basic motions of the Earth. Intrinsic (green), Precession (blue) and
Nutation (red)
Precession, nutation, and intrinsic_rotation (spin) are defined as the
movements obtained by changing one of the Euler angles while leaving the other
two constant. These motions are not expressed in terms of the external frame,
or in terms of the co-moving rotated body frame, but in a mixture. They
constitute a mixed axes of rotation system, where the first angle moves the
line of nodes around the external axis z, the second rotates around the line of
nodes N and the third one is an intrinsic rotation around Z, an axis fixed in
the body that moves.
Left: A gimbal set, showing a z-x-z rotation sequence. External frame shown in
the base. Internal axes in red color. Right: A simple diagram showing similar
Euler angles in a diagram.
The static definition implies that:
    * Î± (precession) represents a rotation around the z axis,
    * Î² (nutation) represents a rotation around the N or xâ² axis,
    * Î³ (intrinsic rotation) represents a rotation around the Z or zâ³ axis.
If Î² is zero, there is no rotation about N. As a consequence, Z coincides with
z, Î± and Î³ represent rotations about the same axis (z), and the final
orientation can be obtained with a single rotation about z, by an angle equal
to Î± + Î³.
As an example, consider a top. The top spins around its own axis of symmetry;
this corresponds to its intrinsic rotation. It also rotates around its pivotal
axis, with its center of mass orbiting the pivotal axis; this rotation is a
precession. Finally, the top can wobble up and down; the inclination angle is
the nutation angle. The same example can be seen with the movements of the
earth.
Though all three movements can be represented by a rotation operator with
constant coefficients in some frame, they cannot be represented by these
operators all at the same time. Given a reference frame, at most one of them
will be coefficient-free. Only precession can be expressed in general as a
matrix in the basis of the space without dependencies of the other angles.
These movements also behave as a gimbal set. If we suppose a set of frames,
able to move each with respect to the former according to just one angle, like
a gimbal, there will exist an external fixed frame, one final frame and two
frames in the middle, which are called "intermediate frames". The two in the
middle work as two gimbal rings that allow the last frame to reach any
orientation in space.
***** TaitâBryan angles[edit] *****
See also: Aircraft_principal_axes
TaitâBryan angles. z-yâ²-xâ³ sequence (intrinsic rotations; N coincides
with yâ). The angle rotation sequence is Ï, Î¸, Ð¤. Note that in this case
Ï > 90Â° and Î¸ is a negative angle.
The second type of formalism is called TaitâBryan angles, after Peter_Guthrie
Tait and George_H._Bryan. It is the convention normally used for aerospace
applications, so that zero degrees elevation represents the horizontal
attitude. TaitâBryan angles represent the orientation of the aircraft with
respect to the world frame. When dealing with other vehicles, different axes
conventions are possible.
**** Definitions[edit] ****
TaitâBryan angles. z-xâ²-yâ³ sequence (intrinsic rotations; N coincides
with xâ²)
The definitions and notations used for TaitâBryan angles are similar to those
described above for proper Euler angles (geometrical_definition, intrinsic
rotation_definition, extrinsic_rotation_definition). The only difference is
that TaitâBryan angles represent rotations about three distinct axes (e.g. x-
y-z, or x-yâ²-zâ³), while proper Euler angles use the same axis for both the
first and third elemental rotations (e.g., z-x-z, or z-xâ²-zâ³).
This implies a different definition for the line_of_nodes in the geometrical
construction. In the proper Euler angles case it was defined as the
intersection between two homologous Cartesian planes (parallel when Euler
angles are zero; e.g. xy and XY). In the second one, it is defined as the
intersection of two non-homologous planes (perpendicular when Euler angles are
zero; e.g. xy and YZ).
**** Conventions[edit] ****
Heading, elevation and bank angles (Z-Yâ²-Xâ³) for an aircraft using onboard
ENU axes both onboard and for the ground tracking station. The fixed reference
frame x-y-z represents such a tracking station. Onboard axes Y and Z are not
shown. X shown in green color. This figure doesn't respect the RHS rules: the
Z-axis must be turned upside down
The three elemental rotations may occur either about the axes of the original
coordinate system, which remains motionless (extrinsic_rotations), or about the
axes of the rotating coordinate system, which changes its orientation after
each elemental rotation (intrinsic_rotations).
There are six possibilities of choosing the rotation axes for TaitâBryan
angles. The six possible sequences are:
    * x-yâ²-zâ³ (intrinsic rotations) or z-y-x (extrinsic rotations)
    * y-zâ²-xâ³ (intrinsic rotations) or x-z-y (extrinsic rotations)
    * z-x'-yâ³ (intrinsic rotations) or y-x-z (extrinsic rotations)
    * x-zâ²-yâ³ (intrinsic rotations) or y-z-x (extrinsic rotations)
    * z-yâ²-xâ³ (intrinsic rotations) or x-y-z (extrinsic rotations): the
      intrinsic rotations are known as: yaw, pitch and roll
    * y-xâ²-zâ³ (intrinsic rotations) or z-x-y (extrinsic rotations)
**** Signs and ranges[edit] ****
The principal_axes of an aircraft according to the air norm DIN 9300. Notice
that fixed and mobile frames must be coincident with angles zero. Therefore,
this norm would force also a compatible axes_convention in the reference system
TaitâBryan convention is widely used in engineering with different purposes.
There are several axes_conventions in practice for choosing the mobile and
fixed axes, and these conventions determine the signs of the angles. Therefore,
signs must be studied in each case carefully.
The range for the angles ψ and φ covers 2π radians. For θ the range covers π
radians.
**** Alternative names[edit] ****
These angles are normally taken as one in the external reference frame
(heading, bearing), one in the intrinsic moving frame (bank) and one in a
middle frame, representing an elevation or inclination respect the horizontal
plane, which is equivalent to the line of nodes for this purpose.
For an aircraft, they can be obtained with three rotations around its principal
axes if done in the proper order. A yaw will obtain the bearing, a pitch will
yield the elevation and a roll gives the bank angle. Therefore, in aerospace
they are sometimes called yaw, pitch and roll. Notice that this will not work
if the rotations are applied in any other order or if the airplane axes start
in any position non-equivalent to the reference frame.
TaitâBryan angles, following z-yâ²-xâ³ (intrinsic rotations) convention,
are also known as nautical angles, because they can be used to describe the
orientation of a ship or aircraft, or Cardan angles, after the Italian
mathematician and physicist Gerolamo_Cardano, who first described in detail the
Cardan_suspension and the Cardan_joint.
***** Angles of a given frame[edit] *****
Projections of Z vector
Projections of Y vector
A common problem is to find the Euler angles of a given frame. The fastest way
to get them is to write the three given vectors as columns of a matrix and
compare it with the expression of the theoretical matrix (see later table of
matrices). Hence the three Euler Angles can be calculated. Nevertheless, the
same result can be reached avoiding matrix algebra and using only elemental
geometry. Here we present the results for the two most commonly used
conventions: ZXZ for proper Euler angles and ZYX for TaitâBryan. Notice that
any other convention can be obtained just changing the name of the axes.
**** Proper Euler angles[edit] ****
Assuming a frame with unit_vectors (X, Y, Z) given by their coordinates as in
the main diagram, it can be seen that:
         cos &#x2061; ( &#x03B2; ) =  Z  3   .   {\displaystyle \cos(\beta )=Z_
      {3}.}  [\cos(\beta )=Z_{3}.]
And, since
          sin  2   &#x2061; x = 1 &#x2212;  cos  2   &#x2061; x ,
      {\displaystyle \sin ^{2}x=1-\cos ^{2}x,}  [\sin ^{2}x=1-\cos ^{2}x,]
we have
         sin &#x2061; ( &#x03B2; ) =   1 &#x2212;  Z  3   2     .
      {\displaystyle \sin(\beta )={\sqrt {1-Z_{3}^{2}}}.}  [\sin(\beta )={\sqrt
      {1-Z_{3}^{2}}}.]
As      Z  2     {\displaystyle Z_{2}}  [Z_{2}] is the double projection of a
unitary vector,
         cos &#x2061; ( &#x03B1; ) &#x22C5; sin &#x2061; ( &#x03B2; ) =
      &#x2212;  Z  2   ,   {\displaystyle \cos(\alpha )\cdot \sin(\beta )=-Z_
      {2},}  [\cos(\alpha) \cdot \sin(\beta) = -Z_2,]
         cos &#x2061; ( &#x03B1; ) = &#x2212;  Z  2    /    1 &#x2212;  Z  3
      2     .   {\displaystyle \cos(\alpha )=-Z_{2}/{\sqrt {1-Z_{3}^{2}}}.}
      [\cos(\alpha) = -Z_2 / \sqrt{1 - Z_3^2}.]
There is a similar construction for      Y  3     {\displaystyle Y_{3}}  [Y_
{3}], projecting it first over the plane defined by the axis z and the line of
nodes. As the angle between the planes is     &#x03C0;  /  2 &#x2212; &#x03B2;
{\displaystyle \pi /2-\beta }  [\pi /2-\beta ] and     cos &#x2061; ( &#x03C0;
/  2 &#x2212; &#x03B2; ) = sin &#x2061; ( &#x03B2; )   {\displaystyle \cos(\pi
/2-\beta )=\sin(\beta )}  [\cos(\pi /2-\beta )=\sin(\beta )], this leads to:
         sin &#x2061; ( &#x03B2; ) &#x22C5; cos &#x2061; ( &#x03B3; ) =  Y  3
      ,   {\displaystyle \sin(\beta )\cdot \cos(\gamma )=Y_{3},}  [\sin(\beta
      )\cdot \cos(\gamma )=Y_{3},]
         cos &#x2061; ( &#x03B3; ) =  Y  3    /    1 &#x2212;  Z  3   2     ,
      {\displaystyle \cos(\gamma )=Y_{3}/{\sqrt {1-Z_{3}^{2}}},}  [\cos(\gamma
      )=Y_{3}/{\sqrt {1-Z_{3}^{2}}},]
and finally, using the inverse_cosine function,
         &#x03B1; = arccos &#x2061; ( &#x2212;  Z  2    /    1 &#x2212;  Z  3
      2     ) ,   {\displaystyle \alpha =\arccos(-Z_{2}/{\sqrt {1-Z_{3}^
      {2}}}),}  [\alpha = \arccos(-Z_2 / \sqrt{1 - Z_3^2}),]
         &#x03B2; = arccos &#x2061; (  Z  3   ) ,   {\displaystyle \beta
      =\arccos(Z_{3}),}  [\beta =\arccos(Z_{3}),]
         &#x03B3; = arccos &#x2061; (  Y  3    /    1 &#x2212;  Z  3   2     )
      .   {\displaystyle \gamma =\arccos(Y_{3}/{\sqrt {1-Z_{3}^{2}}}).}
      [\gamma =\arccos(Y_{3}/{\sqrt {1-Z_{3}^{2}}}).]
**** TaitâBryan angles[edit] ****
projections of X axis after three TaitâBryan rotations. Notice that theta is
a negative rotation around the axis yâ².
Assuming a frame with unit_vectors (X, Y, Z) given by their coordinates as in
this new diagram (notice that the angle theta is negative), it can be seen
that:
         sin &#x2061; ( &#x03B8; ) = &#x2212;  X  3     {\displaystyle \sin
      (\theta )=-X_{3}}  [{\displaystyle \sin(\theta )=-X_{3}}]
As before,
          cos  2   &#x2061; x = 1 &#x2212;  sin  2   &#x2061; x ,
      {\displaystyle \cos ^{2}x=1-\sin ^{2}x,}  [{\displaystyle \cos ^{2}x=1-
      \sin ^{2}x,}]
we have
         cos &#x2061; ( &#x03B8; ) =   1 &#x2212;  X  3   2     .
      {\displaystyle \cos(\theta )={\sqrt {1-X_{3}^{2}}}.}  [{\displaystyle
      \cos(\theta )={\sqrt {1-X_{3}^{2}}}.}]
in a way analogous to the former one:
         sin &#x2061; ( &#x03C8; ) =  X  2    /    1 &#x2212;  X  3   2     .
      {\displaystyle \sin(\psi )=X_{2}/{\sqrt {1-X_{3}^{2}}}.}  [{\displaystyle
      \sin(\psi )=X_{2}/{\sqrt {1-X_{3}^{2}}}.}]
         sin &#x2061; ( &#x03D5; ) =  Y  3    /    1 &#x2212;  X  3   2     .
      {\displaystyle \sin(\phi )=Y_{3}/{\sqrt {1-X_{3}^{2}}}.}  [{\displaystyle
      \sin(\phi )=Y_{3}/{\sqrt {1-X_{3}^{2}}}.}]
Looking for similar expressions to the former ones:
         &#x03C8; = arcsin &#x2061; (  X  2    /    1 &#x2212;  X  3   2     )
      ,   {\displaystyle \psi =\arcsin(X_{2}/{\sqrt {1-X_{3}^{2}}}),}  [
      {\displaystyle \psi =\arcsin(X_{2}/{\sqrt {1-X_{3}^{2}}}),}]
         &#x03B8; = arcsin &#x2061; ( &#x2212;  X  3   ) ,   {\displaystyle
      \theta =\arcsin(-X_{3}),}  [{\displaystyle \theta =\arcsin(-X_{3}),}]
         &#x03D5; = arcsin &#x2061; (  Y  3    /    1 &#x2212;  X  3   2     )
      .   {\displaystyle \phi =\arcsin(Y_{3}/{\sqrt {1-X_{3}^{2}}}).}  [
      {\displaystyle \phi =\arcsin(Y_{3}/{\sqrt {1-X_{3}^{2}}}).}]
**** Last remarks[edit] ****
Note that the inverse sine and cosine functions yield two possible values for
the argument. In this geometrical description only one of the solutions is
valid. When Euler Angles are defined as a sequence of rotations, all the
solutions can be valid, but there will be only one inside the angle ranges.
This is because the sequence of rotations to reach the target frame is not
unique if the ranges are not previously defined.[2]
For computational purposes, it may be useful to represent the angles using
atan2(y, x). For example, in the case of proper Euler angles:
         &#x03B1; = atan2 &#x2061; (  Z  1   , &#x2212;  Z  2   ) ,
      {\displaystyle \alpha =\operatorname {atan2} (Z_{1},-Z_{2}),}  [\alpha =
      \operatorname{atan2}(Z_1 , -Z_2),]
         &#x03B3; = atan2 &#x2061; (  X  3   ,  Y  3   ) .   {\displaystyle
      \gamma =\operatorname {atan2} (X_{3},Y_{3}).}  [\gamma =\operatorname
      {atan2} (X_{3},Y_{3}).]
***** Conversion to other orientation representations[edit] *****
Main article: Rotation_formalisms_in_three_dimensions_Â§ Conversion_formulae
between_formalisms
Euler angles are one way to represent orientations. There are others, and it is
possible to change to and from other conventions. Three parameters are always
required to describe orientations in a 3-dimensional Euclidean_space. They can
be given in several ways, Euler angles being one of them; see charts_on_SO(3)
for others.
The most used orientation representation are the rotation_matrices, the axis-
angle and the quaternions, also known as EulerâRodrigues_parameters, which
provide another_mechanism for representing 3D rotations. This is equivalent to
the special unitary group description.
Expressing rotations in 3D as unit quaternions instead of matrices has some
advantages:
    * Concatenating rotations is computationally faster and numerically more
      stable.
    * Extracting the angle and axis of rotation is simpler.
    * Interpolation is more straightforward. See for example slerp.
    * Quaternions do not suffer from gimbal_lock as Euler angles do.
Regardless, the rotation matrix calculation is the first step for obtaining the
other two representations.
**** Rotation matrix[edit] ****
Any orientation can be achieved by composing three elemental rotations,
starting from a known standard orientation. Equivalently, any rotation_matrix R
can be decomposed as a product of three elemental rotation matrices. For
instance:
         R = X ( &#x03B1; ) Y ( &#x03B2; ) Z ( &#x03B3; )   {\displaystyle R=X
      (\alpha )Y(\beta )Z(\gamma )}  [R=X(\alpha )Y(\beta )Z(\gamma )]
is a rotation matrix that may be used to represent a composition of extrinsic
rotations about axes z, y, x, (in that order), or a composition of intrinsic
rotations about axes x-yâ²-zâ³ (in that order). However, both the definition
of the elemental rotation matrices X, Y, Z, and their multiplication order
depend on the choices taken by the user about the definition of both rotation
matrices and Euler angles (see, for instance, Ambiguities_in_the_definition_of
rotation_matrices). Unfortunately, different sets of conventions are adopted by
users in different contexts. The following table was built according to this
set of conventions:
   1. Each matrix is meant to operate by pre-multiplying column_vectors
      [    x     y     z    ]     {\textstyle {\begin{bmatrix}x\\y\\z\end
      {bmatrix}}}  [{\textstyle {\begin{bmatrix}x\\y\\z\end{bmatrix}}}] (see
      Ambiguities_in_the_definition_of_rotation_matrices)
   2. Each matrix is meant to represent an active_rotation (the composing and
      composed matrices are supposed to act on the coordinates of vectors
      defined in the initial fixed reference frame and give as a result the
      coordinates of a rotated vector defined in the same reference frame).
   3. Each matrix is meant to represent, primarily, the composition of
      extrinsic_rotations (which corresponds to the constructive evaluation of
      the R matrix by the multiplication of three truly elemental matrices)
      and, secondarily, the composition of three non elemental matrices
      representing globally an intrinsic_rotations (around the axes of the
      rotating reference frame, in inverse order).
   4. Right_handed reference frames are adopted, and the right_hand_rule is
      used to determine the sign of the angles Î±, Î², Î³.
For the sake of simplicity, the following table uses the following
nomenclature:
   1. 1, 2, 3 represent the angles Î±, Î² and Î³, i.e. the angles corresponding
      to the first, second and third elemental rotations respectively.
   2. X, Y, Z are the matrices representing the elemental rotations about the
      axes x, y, z of the fixed frame (e.g., X1 represents a rotation about x
      by an angle Î±).
   3. s and c represent sine and cosine (e.g., s1 represents the sine of Î±).
   4. Each matrix is denoted by the formula used to calculate it. If     R =  Z
      1    X  2    Z  3     {\displaystyle R=Z_{1}X_{2}Z_{3}}  [R=Z_{1}X_{2}Z_
      {3}], we name it      Z  1    X  2    Z  3     {\displaystyle Z_{1}X_
      {2}Z_{3}}  [Z_{1}X_{2}Z_{3}].
      Proper Euler angles                  TaitâBryan angles
          X  1    Z  2    X  3   =             X  1    Z  2    Y  3   =
      [     c  2     &#x2212;  c  3    s   [     c  2    c  3     &#x2212;  s
      2      s  2    s  3        c  1    s 2      c  2    s  3        s  1    s
      2      c  1    c  2    c  3          3   +  c  1    c  3    s  2      c
      &#x2212;  s  1    s  3     &#x2212;  1    c  2      c  1    s  2    s  3
      c  3    s  1   &#x2212;  c  1    c   &#x2212;  c  3    s  1        c  3
      2    s  3        s  1    s  2      c s  1    s  2   &#x2212;  c  1    s
      1    s  3   +  c  2    c  3    s  1  3      c  2    s  1      c  1    c
      c  1    c  3   &#x2212;  c  2    s   3   +  s  1    s  2    s  3      ]
      1    s  3      ]     {\displaystyle  {\displaystyle X_{1}Z_{2}Y_{3}=
      X_{1}Z_{2}X_{3}={\begin{bmatrix}c_   {\begin{bmatrix}c_{2}c_{3}&-s_{2}&c_
      {2}&-c_{3}s_{2}&s_{2}s_{3}\\c_{1}s_  {2}s_{3}\\s_{1}s_{3}+c_{1}c_{3}s_
      {2}&c_{1}c_{2}c_{3}-s_{1}s_{3}&-c_   {2}&c_{1}c_{2}&c_{1}s_{2}s_{3}-c_
      {3}s_{1}-c_{1}c_{2}s_{3}\\s_{1}s_    {3}s_{1}\\c_{3}s_{1}s_{2}-c_{1}s_
      {2}&c_{1}s_{3}+c_{2}c_{3}s_{1}&c_    {3}&c_{2}s_{1}&c_{1}c_{3}+s_{1}s_
      {1}c_{3}-c_{2}s_{1}s_{3}\end         {2}s_{3}\end{bmatrix}}}  [X_{1}Z_
      {bmatrix}}}  [{\displaystyle X_{1}Z_ {2}Y_{3}={\begin{bmatrix}c_{2}c_
      {2}X_{3}={\begin{bmatrix}c_{2}&-c_   {3}&-s_{2}&c_{2}s_{3}\\s_{1}s_{3}+c_
      {3}s_{2}&s_{2}s_{3}\\c_{1}s_{2}&c_   {1}c_{3}s_{2}&c_{1}c_{2}&c_{1}s_
      {1}c_{2}c_{3}-s_{1}s_{3}&-c_{3}s_    {2}s_{3}-c_{3}s_{1}\\c_{3}s_{1}s_
      {1}-c_{1}c_{2}s_{3}\\s_{1}s_{2}&c_   {2}-c_{1}s_{3}&c_{2}s_{1}&c_{1}c_
      {1}s_{3}+c_{2}c_{3}s_{1}&c_{1}c_{3}- {3}+s_{1}s_{2}s_{3}\end{bmatrix}}]
      c_{2}s_{1}s_{3}\end{bmatrix}}}]
          X  1    Y  2    X  3   =             X  1    Y  2    Z  3   =
      [     c  2      s  2    s  3      c  [     c  2    c  3     &#x2212;  c
      3    s  2        s  1    s  2      c 2    s  3      s  2        c  1    s
      1    c  3   &#x2212;  c  2    s  1   3   +  c  3    s  1    s  2      c
      s  3     &#x2212;  c  1    s  3      1    c  3   &#x2212;  s  1    s  2
      &#x2212;  c  2    c  3    s  1       s  3     &#x2212;  c  2    s  1
      &#x2212;  c  1    s  2      c  3     s  1    s  3   &#x2212;  c  1    c
      s  1   +  c  1    c  2    s  3       3    s  2      c  3    s  1   +  c
      c  1    c  2    c  3   &#x2212;  s   1    s  2    s  3      c  1    c  2
      1    s  3      ]     {\displaystyle  ]     {\displaystyle X_{1}Y_{2}Z_
      X_{1}Y_{2}X_{3}={\begin{bmatrix}c_   {3}={\begin{bmatrix}c_{2}c_{3}&-c_
      {2}&s_{2}s_{3}&c_{3}s_{2}\\s_{1}s_   {2}s_{3}&s_{2}\\c_{1}s_{3}+c_{3}s_
      {2}&c_{1}c_{3}-c_{2}s_{1}s_{3}&-c_   {1}s_{2}&c_{1}c_{3}-s_{1}s_{2}s_
      {1}s_{3}-c_{2}c_{3}s_{1}\\-c_{1}s_   {3}&-c_{2}s_{1}\\s_{1}s_{3}-c_{1}c_
      {2}&c_{3}s_{1}+c_{1}c_{2}s_{3}&c_    {3}s_{2}&c_{3}s_{1}+c_{1}s_{2}s_
      {1}c_{2}c_{3}-s_{1}s_{3}\end         {3}&c_{1}c_{2}\end{bmatrix}}}  [X_
      {bmatrix}}}  [X_{1}Y_{2}X_{3}=       {1}Y_{2}Z_{3}={\begin{bmatrix}c_
      {\begin{bmatrix}c_{2}&s_{2}s_{3}&c_  {2}c_{3}&-c_{2}s_{3}&s_{2}\\c_{1}s_
      {3}s_{2}\\s_{1}s_{2}&c_{1}c_{3}-c_   {3}+c_{3}s_{1}s_{2}&c_{1}c_{3}-s_
      {2}s_{1}s_{3}&-c_{1}s_{3}-c_{2}c_    {1}s_{2}s_{3}&-c_{2}s_{1}\\s_{1}s_
      {3}s_{1}\\-c_{1}s_{2}&c_{3}s_{1}+c_  {3}-c_{1}c_{3}s_{2}&c_{3}s_{1}+c_
      {1}c_{2}s_{3}&c_{1}c_{2}c_{3}-s_     {1}s_{2}s_{3}&c_{1}c_{2}\end
      {1}s_{3}\end{bmatrix}}]              {bmatrix}}]
          Y  1    X  2    Y  3   =             Y  1    X  2    Z  3   =
      [     c  1    c  3   &#x2212;  c  2  [     c  1    c  3   +  s  1    s  2
      s  1    s  3      s  1    s  2       s  3      c  3    s  1    s  2
      c  1    s  3   +  c  2    c  3    s  &#x2212;  c  1    s  3      c  2
      1        s  2    s  3      c  2      s  1        c  2    s  3      c  2
      &#x2212;  c  3    s  2               c  3     &#x2212;  s  2        c  1
      &#x2212;  c  3    s  1   &#x2212;  c s  2    s  3   &#x2212;  c  3    s
      1    c  2    s  3      c  1    s  2  1      c  1    c  3    s  2   +  s
      c  1    c  2    c  3   &#x2212;  s   1    s  3      c  1    c  2      ]
      1    s  3      ]     {\displaystyle  {\displaystyle Y_{1}X_{2}Z_{3}=
      Y_{1}X_{2}Y_{3}={\begin{bmatrix}c_   {\begin{bmatrix}c_{1}c_{3}+s_{1}s_
      {1}c_{3}-c_{2}s_{1}s_{3}&s_{1}s_     {2}s_{3}&c_{3}s_{1}s_{2}-c_{1}s_
      {2}&c_{1}s_{3}+c_{2}c_{3}s_{1}\\s_   {3}&c_{2}s_{1}\\c_{2}s_{3}&c_{2}c_
      {2}s_{3}&c_{2}&-c_{3}s_{2}\\-c_{3}s_ {3}&-s_{2}\\c_{1}s_{2}s_{3}-c_{3}s_
      {1}-c_{1}c_{2}s_{3}&c_{1}s_{2}&c_    {1}&c_{1}c_{3}s_{2}+s_{1}s_{3}&c_
      {1}c_{2}c_{3}-s_{1}s_{3}\end         {1}c_{2}\end{bmatrix}}}  [Y_{1}X_
      {bmatrix}}}  [Y_{1}X_{2}Y_{3}=       {2}Z_{3}={\begin{bmatrix}c_{1}c_
      {\begin{bmatrix}c_{1}c_{3}-c_{2}s_   {3}+s_{1}s_{2}s_{3}&c_{3}s_{1}s_{2}-
      {1}s_{3}&s_{1}s_{2}&c_{1}s_{3}+c_    c_{1}s_{3}&c_{2}s_{1}\\c_{2}s_{3}&c_
      {2}c_{3}s_{1}\\s_{2}s_{3}&c_{2}&-c_  {2}c_{3}&-s_{2}\\c_{1}s_{2}s_{3}-c_
      {3}s_{2}\\-c_{3}s_{1}-c_{1}c_{2}s_   {3}s_{1}&c_{1}c_{3}s_{2}+s_{1}s_
      {3}&c_{1}s_{2}&c_{1}c_{2}c_{3}-s_    {3}&c_{1}c_{2}\end{bmatrix}}]
      {1}s_{3}\end{bmatrix}}]
          Y  1    Z  2    Y  3   =             Y  1    Z  2    X  3   =
      [     c  1    c  2    c  3           [     c  1    c  2      s  1    s  3
      &#x2212;  s  1    s  3     &#x2212;  &#x2212;  c  1    c  3    s  2
      c  1    s  2      c  3    s  1   +   c  3    s  1   +  c  1    s  2    s
      c  1    c  2    s  3        c  3     3        s  2      c  2    c  3
      s  2      c  2      s  2    s  3     &#x2212;  c  2    s  3
      &#x2212;  c  1    s  3   &#x2212;  c &#x2212;  c  2    s  1      c  1
      2    c  3    s  1      s  1    s  2  s  3   +  c  3    s  1    s  2
      c  1    c  3   &#x2212;  c  2    s   c  1    c  3   &#x2212;  s  1    s
      1    s  3      ]     {\displaystyle  2    s  3      ]     {\displaystyle
      Y_{1}Z_{2}Y_{3}={\begin{bmatrix}c_   Y_{1}Z_{2}X_{3}={\begin{bmatrix}c_
      {1}c_{2}c_{3}-s_{1}s_{3}&-c_{1}s_    {1}c_{2}&s_{1}s_{3}-c_{1}c_{3}s_
      {2}&c_{3}s_{1}+c_{1}c_{2}s_{3}\\c_   {2}&c_{3}s_{1}+c_{1}s_{2}s_{3}\\s_
      {3}s_{2}&c_{2}&s_{2}s_{3}\\-c_{1}s_  {2}&c_{2}c_{3}&-c_{2}s_{3}\\-c_{2}s_
      {3}-c_{2}c_{3}s_{1}&s_{1}s_{2}&c_    {1}&c_{1}s_{3}+c_{3}s_{1}s_{2}&c_
      {1}c_{3}-c_{2}s_{1}s_{3}\end         {1}c_{3}-s_{1}s_{2}s_{3}\end
      {bmatrix}}}  [Y_{1}Z_{2}Y_{3}=       {bmatrix}}}  [Y_{1}Z_{2}X_{3}=
      {\begin{bmatrix}c_{1}c_{2}c_{3}-s_   {\begin{bmatrix}c_{1}c_{2}&s_{1}s_
      {1}s_{3}&-c_{1}s_{2}&c_{3}s_{1}+c_   {3}-c_{1}c_{3}s_{2}&c_{3}s_{1}+c_
      {1}c_{2}s_{3}\\c_{3}s_{2}&c_{2}&s_   {1}s_{2}s_{3}\\s_{2}&c_{2}c_{3}&-c_
      {2}s_{3}\\-c_{1}s_{3}-c_{2}c_{3}s_   {2}s_{3}\\-c_{2}s_{1}&c_{1}s_{3}+c_
      {1}&s_{1}s_{2}&c_{1}c_{3}-c_{2}s_    {3}s_{1}s_{2}&c_{1}c_{3}-s_{1}s_
      {1}s_{3}\end{bmatrix}}]              {2}s_{3}\end{bmatrix}}]
          Z  1    Y  2    Z  3   =             Z  1    Y  2    X  3   =
      [     c  1    c  2    c  3           [     c  1    c  2      c  1    s  2
      &#x2212;  s  1    s  3     &#x2212;  s  3   &#x2212;  c  3    s  1      s
      c  3    s  1   &#x2212;  c  1    c   1    s  3   +  c  1    c  3    s  2
      2    s  3      c  1    s  2        c c  2    s  1      c  1    c  3   +
      1    s  3   +  c  2    c  3    s  1  s  1    s  2    s  3      c  3    s
      c  1    c  3   &#x2212;  c  2    s   1    s  2   &#x2212;  c  1    s  3
      1    s  3      s  1    s  2          &#x2212;  s  2      c  2    s  3
      &#x2212;  c  3    s  2      s  2     c  2    c  3      ]
      s  3      c  2      ]                {\displaystyle Z_{1}Y_{2}X_{3}=
      {\displaystyle Z_{1}Y_{2}Z_{3}=      {\begin{bmatrix}c_{1}c_{2}&c_{1}s_
      {\begin{bmatrix}c_{1}c_{2}c_{3}-s_   {2}s_{3}-c_{3}s_{1}&s_{1}s_{3}+c_
      {1}s_{3}&-c_{3}s_{1}-c_{1}c_{2}s_    {1}c_{3}s_{2}\\c_{2}s_{1}&c_{1}c_
      {3}&c_{1}s_{2}\\c_{1}s_{3}+c_{2}c_   {3}+s_{1}s_{2}s_{3}&c_{3}s_{1}s_{2}-
      {3}s_{1}&c_{1}c_{3}-c_{2}s_{1}s_     c_{1}s_{3}\\-s_{2}&c_{2}s_{3}&c_
      {3}&s_{1}s_{2}\\-c_{3}s_{2}&s_{2}s_  {2}c_{3}\end{bmatrix}}}  [Z_{1}Y_
      {3}&c_{2}\end{bmatrix}}}  [Z_{1}Y_   {2}X_{3}={\begin{bmatrix}c_{1}c_
      {2}Z_{3}={\begin{bmatrix}c_{1}c_     {2}&c_{1}s_{2}s_{3}-c_{3}s_{1}&s_
      {2}c_{3}-s_{1}s_{3}&-c_{3}s_{1}-c_   {1}s_{3}+c_{1}c_{3}s_{2}\\c_{2}s_
      {1}c_{2}s_{3}&c_{1}s_{2}\\c_{1}s_    {1}&c_{1}c_{3}+s_{1}s_{2}s_{3}&c_
      {3}+c_{2}c_{3}s_{1}&c_{1}c_{3}-c_    {3}s_{1}s_{2}-c_{1}s_{3}\\-s_{2}&c_
      {2}s_{1}s_{3}&s_{1}s_{2}\\-c_{3}s_   {2}s_{3}&c_{2}c_{3}\end{bmatrix}}]
      {2}&s_{2}s_{3}&c_{2}\end{bmatrix}}]
          Z  1    X  2    Z  3   =             Z  1    X  2    Y  3   =
      [     c  1    c  3   &#x2212;  c  2  [     c  1    c  3   &#x2212;  s  1
      s  1    s  3     &#x2212;  c  1    s s  2    s  3     &#x2212;  c  2    s
      3   &#x2212;  c  2    c  3    s  1   1      c  1    s  3   +  c  3    s
      s  1    s  2        c  3    s  1   + 1    s  2        c  3    s  1   +  c
      c  1    c  2    s  3      c  1    c  1    s  2    s  3      c  1    c  2
      2    c  3   &#x2212;  s  1    s  3   s  1    s  3   &#x2212;  c  1    c
      &#x2212;  c  1    s  2        s  2   3    s  2       &#x2212;  c  2    s
      s  3      c  3    s  2      c  2     3      s  2      c  2    c  3      ]
      ]     {\displaystyle Z_{1}X_{2}Z_    {\displaystyle Z_{1}X_{2}Y_{3}=
      {3}={\begin{bmatrix}c_{1}c_{3}-c_    {\begin{bmatrix}c_{1}c_{3}-s_{1}s_
      {2}s_{1}s_{3}&-c_{1}s_{3}-c_{2}c_    {2}s_{3}&-c_{2}s_{1}&c_{1}s_{3}+c_
      {3}s_{1}&s_{1}s_{2}\\c_{3}s_{1}+c_   {3}s_{1}s_{2}\\c_{3}s_{1}+c_{1}s_
      {1}c_{2}s_{3}&c_{1}c_{2}c_{3}-s_     {2}s_{3}&c_{1}c_{2}&s_{1}s_{3}-c_
      {1}s_{3}&-c_{1}s_{2}\\s_{2}s_{3}&c_  {1}c_{3}s_{2}\\-c_{2}s_{3}&s_{2}&c_
      {3}s_{2}&c_{2}\end{bmatrix}}}  [Z_   {2}c_{3}\end{bmatrix}}}  [Z_{1}X_
      {1}X_{2}Z_{3}={\begin{bmatrix}c_     {2}Y_{3}={\begin{bmatrix}c_{1}c_{3}-
      {1}c_{3}-c_{2}s_{1}s_{3}&-c_{1}s_    s_{1}s_{2}s_{3}&-c_{2}s_{1}&c_{1}s_
      {3}-c_{2}c_{3}s_{1}&s_{1}s_{2}\\c_   {3}+c_{3}s_{1}s_{2}\\c_{3}s_{1}+c_
      {3}s_{1}+c_{1}c_{2}s_{3}&c_{1}c_     {1}s_{2}s_{3}&c_{1}c_{2}&s_{1}s_{3}-
      {2}c_{3}-s_{1}s_{3}&-c_{1}s_{2}\\s_  c_{1}c_{3}s_{2}\\-c_{2}s_{3}&s_
      {2}s_{3}&c_{3}s_{2}&c_{2}\end        {2}&c_{2}c_{3}\end{bmatrix}}]
      {bmatrix}}]
To change the formulas for passive_rotations (or find reverse active rotation),
transpose the matrices (then each matrix transforms the initial coordinates of
a vector remaining fixed to the coordinates of the same vector measured in the
rotated reference system; same rotation axis, same angles, but now the
coordinate system rotates, rather than the vector).
***** Properties[edit] *****
See also: Charts_on_SO(3) and Quaternions_and_spatial_rotation
The Euler angles form a chart on all of SO(3), the special_orthogonal_group of
rotations in 3D space. The chart is smooth except for a polar coordinate style
singularity along Î² = 0. See charts_on_SO(3) for a more complete treatment.
The space of rotations is called in general "The Hypersphere_of_rotations",
though this is a misnomer: the group Spin(3) is isometric to the hypersphere
S3, but the rotation space SO(3) is instead isometric to the real_projective
space RP3 which is a 2-fold quotient_space of the hypersphere. This 2-to-
1 ambiguity is the mathematical origin of spin_in_physics.
A similar three angle decomposition applies to SU(2), the special_unitary_group
of rotations in complex 2D space, with the difference that Î² ranges from 0 to
2Ï. These are also called Euler angles.
The Haar_measure for SO(3) in Euler angles is given by the Hopf angle
parametrisation of SO(3),       d   V &#x221D; sin &#x2061; &#x03B1; .   d
&#x03B1; .   d   &#x03B2; .   d   &#x03B3;   {\displaystyle {\textrm
{d}}V\propto \sin \alpha .{\textrm {d}}\alpha .{\textrm {d}}\beta .{\textrm
{d}}\gamma }  [{\displaystyle {\textrm {d}}V\propto \sin \alpha .{\textrm
{d}}\alpha .{\textrm {d}}\beta .{\textrm {d}}\gamma }],[3] where     ( &#x03B1;
, &#x03B2; )   {\displaystyle (\alpha ,\beta )}  [(\alpha ,\beta )] parametrise
S  2     {\displaystyle S^{2}}  [S^{{2}}], the space of rotation axes.
For example, to generate uniformly randomized orientations, let Î± and Î³ be
uniform from 0 to 2Ï, let z be uniform from −1 to 1, and let Î² = arccos(z).
**** Geometric algebra[edit] ****
Other properties of Euler angles and rotations in general can be found from the
Geometric_algebra(GA). GA is a higher level abstraction, in which the
quaternions are an even subalgebra. The principal tool in GA is the rotor
R   = [ cos &#x2061; ( &#x03B8;  /  2 ) &#x2212; I u sin &#x2061; ( &#x03B8;  /
2 ) ]   {\displaystyle \mathbf {\mathbb {R} } =[\cos(\theta /2)-Iu\sin(\theta /
2)]}  [{\displaystyle \mathbf {\mathbb {R} } =[\cos(\theta /2)-Iu\sin(\theta /
2)]}] where      &#x03B8;  =   {\displaystyle \mathbf {\theta } =}  [
{\displaystyle \mathbf {\theta } =}]angle_of_rotation,      (  u ) =
{\displaystyle \mathbf {(} u)=}  [{\displaystyle \mathbf {(} u)=}]rotation axis
(unitary vector) and      (  I ) =   {\displaystyle \mathbf {(} I)=}  [
{\displaystyle \mathbf {(} I)=}]pseudoscalar (trivector in       R   3
{\displaystyle \mathbb {R} ^{3}}  [\mathbb {R} ^{3}])
**** Higher dimensions[edit] ****
It is possible to define parameters analogous to the Euler angles in dimensions
higher than three.[4]
The number of degrees of freedom of a rotation matrix is always less than the
dimension of the matrix squared. That is, the elements of a rotation matrix are
not all completely independent. For example, the rotation matrix in dimension 2
has only one degree of freedom, since all four of its elements depend on a
single angle of rotation. A rotation matrix in dimension 3 (which has nine
elements) has three degrees of freedom, corresponding to each independent
rotation, for example by its three Euler angles or a magnitude one (unit)
quaternion.
In SO(4) the rotation matrix is_defined_by_two_quaternions, and is therefore 6-
parametric (three degrees of freedom for every quaternion). The 4Ã4 rotation
matrices have therefore 6 out of 16 independent components.
Any set of 6 parameters that define the rotation matrix could be considered an
extension of Euler angles to dimension 4.
In general, the number of euler angles in dimension D is quadratic in D; since
any one rotation consists of choosing two dimensions to rotate between, the
total number of rotations available in dimension     D   {\displaystyle D}  [D]
is      N  r o t   =    (   D 2   )    = D ( D &#x2212; 1 )  /  2
{\displaystyle N_{rot}={\binom {D}{2}}=D(D-1)/2}  [N_{rot}={\binom {D}{2}}=D(D-
1)/2], which for     D = 2 , 3 , 4   {\displaystyle D=2,3,4}  [D=2,3,4] yields
N  r o t   = 1 , 3 , 6   {\displaystyle N_{rot}=1,3,6}  [N_{rot}=1,3,6].
***** Applications[edit] *****
A gyroscope keeps its rotation axis constant. Therefore, angles measured in
this frame are equivalent to angles measured in the lab frame.
**** Vehicles and moving frames[edit] ****
Main article: rigid_body
See also: axes_conventions
Their main advantage over other orientation descriptions is that they are
directly measurable from a gimbal mounted in a vehicle. As gyroscopes keep
their rotation axis constant, angles measured in a gyro frame are equivalent to
angles measured in the lab frame. Therefore, gyros are used to know the actual
orientation of moving spacecraft, and Euler angles are directly measurable.
Intrinsic rotation angle cannot be read from a single gimbal, so there has to
be more than one gimbal in a spacecraft. Normally there are at least three for
redundancy. There is also a relation to the well-known gimbal_lock problem of
mechanical_engineering [5] .
When studying rigid bodies in general, one calls the xyz system space
coordinates, and the XYZ system body coordinates. The space coordinates are
treated as unmoving, while the body coordinates are considered embedded in the
moving body. Calculations involving acceleration, angular_acceleration, angular
velocity, angular_momentum, and kinetic_energy are often easiest in body
coordinates, because then the moment of inertia tensor does not change in time.
If one also diagonalizes the rigid body's moment of inertia tensor (with nine
components, six of which are independent), then one has a set of coordinates
(called the principal axes) in which the moment of inertia tensor has only
three components.
The angular velocity of a rigid body takes a simple_form using Euler angles in
the moving frame. Also the Euler's_rigid_body_equations are simpler because the
inertia tensor is constant in that frame.
**** Crystallographic texture[edit] ****
Pole figures displaying crystallographic texture of gamma-TiAl in an alpha2-
gamma alloy, as measured by high energy X-rays.[6]
In materials science, crystallographic texture (or preferred orientation) can
be described using Euler angles. In texture analysis, the Euler angles provide
a mathematical depiction of the orientation of individual crystallites within a
polycrystalline material, allowing for the quantitative description of the
macroscopic material.[7] The most common definition of the angles is due to
Bunge and corresponds to the ZXZ convention. It is important to note, however,
that the application generally involves axis transformations of tensor
quantities, i.e. passive rotations. Thus the matrix that corresponds to the
Bunge Euler angles is the transpose of that shown in the table above.[8]
**** Others[edit] ****
Industrial robot operating in a foundry
Euler angles, normally in the TaitâBryan convention, are also used in
robotics for speaking about the degrees of freedom of a wrist. They are also
used in Electronic_stability_control in a similar way.
Gun fire control systems require corrections to gun-order angles (bearing and
elevation) to compensate for deck tilt (pitch and roll). In traditional
systems, a stabilizing gyroscope with a vertical spin axis corrects for deck
tilt, and stabilizes the optical sights and radar antenna. However, gun barrels
point in a direction different from the line of sight to the target, to
anticipate target movement and fall of the projectile due to gravity, among
other factors. Gun mounts roll and pitch with the deck plane, but also require
stabilization. Gun orders include angles computed from the vertical gyro data,
and those computations involve Euler angles.
Euler angles are also used extensively in the quantum mechanics of angular
momentum. In quantum mechanics, explicit descriptions of the representations of
SO(3) are very important for calculations, and almost all the work has been
done using Euler angles. In the early history of quantum mechanics, when
physicists and chemists had a sharply negative reaction towards abstract group
theoretic methods (called the Gruppenpest), reliance on Euler angles was also
essential for basic theoretical work.
Many mobile computing devices contain accelerometers which can determine these
devices' Euler angles with respect to the earth's gravitational attraction.
These are used in applications such as games, bubble_level simulations, and
kaleidoscopes.[citation_needed]
***** See also[edit] *****
    * 3D_projection
    * Axis-angle_representation
    * Conversion_between_quaternions_and_Euler_angles
    * Euler's_rotation_theorem
    * Quaternion
    * Quaternions_and_spatial_rotation
    * Rotation_formalisms_in_three_dimensions
    * Spherical_coordinate_system
***** References[edit] *****
   1. ^ Novi Commentarii academiae scientiarum Petropolitanae 20, 1776, pp.
      189â207 (E478) PDF
   2. ^ Gregory_G._Slabaugh,_Computing_Euler_angles_from_a_rotation_matrix
   3. ^ Section 8 - Derivation of Hopf parametrisation : Generating_Uniform
      Incremental_Grids_on_SO(3)_Using_the_Hopf_Fibration  .
   4. ^ (in Italian) A_generalization_of_Euler_Angles_to_n-dimensional_real
      spaces
   5. ^ The relation between the Euler angles and the Cardan suspension is
      explained in chap. 11.7 of the following textbook: U. Krey, A. Owen,
      Basic Theoretical Physics â A Concise Overview, New York, London,
      Berlin, Heidelberg, Springer (2007) .
   6. ^Liss KD, Bartels A, Schreyer A, Clemens H (2003). "High energy X-rays: A
      tool for advanced bulk investigations in materials science and physics".
      Textures Microstruct. 35 (3/4): 219â52. doi:10.1080/
      07303300310001634952.
   7. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   8. ^Kocks, U.F.; TomÃ©, C.N.; Wenk, H.-R. (2000), Texture and Anisotropy:
      Preferred Orientations in Polycrystals and their effect on Materials
      Properties, Cambridge, ISBN 978-0-521-79420-6
   9. ^Bunge, H. (1993), Texture Analysis in Materials Science: Mathematical
      Methods, Cuvillier_Verlag, ASIN B0014XV9HU
***** Bibliography[edit] *****
    * Biedenharn, L. C.; Louck, J. D. (1981), Angular Momentum in Quantum
      Physics, Reading, MA: AddisonâWesley, ISBN 978-0-201-13507-7
Goldstein,_Herbert (1980), Classical Mechanics (2nd ed.), Reading, MA:
AddisonâWesley, ISBN 978-0-201-02918-5
Gray, Andrew (1918), A Treatise on Gyrostatics and Rotational Motion, London:
Macmillan (published 2007), ISBN 978-1-4212-5592-7
Rose, M. E. (1957), Elementary Theory of Angular Momentum, New York, NY: John
Wiley_&_Sons (published 1995), ISBN 978-0-486-68480-2
Symon, Keith (1971), Mechanics, Reading, MA: Addison-Wesley, ISBN 978-0-201-
07392-8
Landau,_L.D.; Lifshitz,_E._M. (1996), Mechanics (3rd ed.), Oxford: Butterworth-
Heinemann, ISBN 978-0-7506-2896-9
***** External links[edit] *****
 Wikimedia Commons has media related to Euler_angles.
    * Weisstein,_Eric_W. "Euler_Angles". MathWorld.
An interactive tutorial on Euler angles available at https://www.mecademic.com/
resources/Euler-angles/Euler-angles
EulerAngles – an iOS app for visualizing in 3D the three rotations associated
with Euler angles
Orientation_Library – "orilib", a collection of routines for rotation /
orientation manipulation, including special tools for crystal orientations
Online tool to convert rotation matrices available at rotation_converter
(numerical conversion)
Online tool to convert symbolic rotation matrices (dead, but still available
from the Wayback_Machine) symbolic_rotation_converter
Rotation,_Reflection,_and_Frame_Change:_Orthogonal_tensors_in_computational
engineering_mechanics, IOP Publishing

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Euler_angles&oldid=904762215"
Categories:
    * Rotation_in_three_dimensions
    * Euclidean_symmetries
    * Angle
    * Analytic_geometry
Hidden categories:
    * Articles_with_Italian-language_external_links
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_May_2011
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
    * CatalÃ 
    * Deutsch
    * EspaÃ±ol
    * Euskara
    * FranÃ§ais
    * Gaeilge
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 4 July 2019, at 10:49 (UTC).
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
