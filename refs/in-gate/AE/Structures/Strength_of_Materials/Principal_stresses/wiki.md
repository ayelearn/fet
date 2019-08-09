The following text has been accessed from https://en.wikipedia.org/wiki/Cauchy_stress_tensor#Principal_stresses_and_stress_invariants at Thu Aug 8 23:11:10 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Cauchy stress tensor ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Figure 2.3 Components of stress in three dimensions
In continuum_mechanics, the Cauchy stress tensor      &#x03C3;
{\displaystyle {\boldsymbol {\sigma }}}  [{\boldsymbol  \sigma }], true stress
tensor,[1] or simply called the stress tensor is a second order tensor named
after Augustin-Louis_Cauchy. The tensor consists of nine components
&#x03C3;  i j     {\displaystyle \sigma _{ij}}  [\sigma _{ij}] that completely
define the state of stress at a point inside a material in the deformed state,
placement, or configuration. The tensor relates a unit-length direction vector
n to the stress vector T(n) across an imaginary surface perpendicular to n:
           T   (  n  )   =  n  &#x22C5;  &#x03C3;    or    T  j   ( n )   =
      &#x03C3;  i j    n  i   .   {\displaystyle \mathbf {T} ^{(\mathbf {n}
      )}=\mathbf {n} \cdot {\boldsymbol {\sigma }}\quad {\text{or}}\quad T_{j}^
      {(n)}=\sigma _{ij}n_{i}.}  [{\displaystyle \mathbf {T} ^{(\mathbf {n}
      )}=\mathbf {n} \cdot {\boldsymbol {\sigma }}\quad {\text{or}}\quad T_{j}^
      {(n)}=\sigma _{ij}n_{i}.}]
where,
          &#x03C3;  =  [      &#x03C3;  11      &#x03C3;  12      &#x03C3;  13
      &#x03C3;  21      &#x03C3;  22      &#x03C3;  23        &#x03C3;  31
      &#x03C3;  32      &#x03C3;  33       ]  &#x2261;  [      &#x03C3;  x x
      &#x03C3;  x y      &#x03C3;  x z        &#x03C3;  y x      &#x03C3;  y y
      &#x03C3;  y z        &#x03C3;  z x      &#x03C3;  z y      &#x03C3;  z z
      ]  &#x2261;  [      &#x03C3;  x      &#x03C4;  x y      &#x03C4;  x z
      &#x03C4;  y x      &#x03C3;  y      &#x03C4;  y z        &#x03C4;  z x
      &#x03C4;  z y      &#x03C3;  z       ]    {\displaystyle {\boldsymbol
      {\sigma }}=\left[{\begin{matrix}\sigma _{11}&\sigma _{12}&\sigma _
      {13}\\\sigma _{21}&\sigma _{22}&\sigma _{23}\\\sigma _{31}&\sigma _
      {32}&\sigma _{33}\\\end{matrix}}\right]\equiv \left[{\begin{matrix}\sigma
      _{xx}&\sigma _{xy}&\sigma _{xz}\\\sigma _{yx}&\sigma _{yy}&\sigma _
      {yz}\\\sigma _{zx}&\sigma _{zy}&\sigma _{zz}\\\end{matrix}}\right]\equiv
      \left[{\begin{matrix}\sigma _{x}&\tau _{xy}&\tau _{xz}\\\tau _{yx}&\sigma
      _{y}&\tau _{yz}\\\tau _{zx}&\tau _{zy}&\sigma _{z}\\\end{matrix}}\right]}
      [{\boldsymbol  {\sigma }}=\left[{{\begin{matrix}\sigma _{{11}}&\sigma _{
      {12}}&\sigma _{{13}}\\\sigma _{{21}}&\sigma _{{22}}&\sigma _{
      {23}}\\\sigma _{{31}}&\sigma _{{32}}&\sigma _{{33}}\\\end
      {matrix}}}\right]\equiv \left[{{\begin{matrix}\sigma _{{xx}}&\sigma _{
      {xy}}&\sigma _{{xz}}\\\sigma _{{yx}}&\sigma _{{yy}}&\sigma _{
      {yz}}\\\sigma _{{zx}}&\sigma _{{zy}}&\sigma _{{zz}}\\\end
      {matrix}}}\right]\equiv \left[{{\begin{matrix}\sigma _{x}&\tau _{
      {xy}}&\tau _{{xz}}\\\tau _{{yx}}&\sigma _{y}&\tau _{{yz}}\\\tau _{
      {zx}}&\tau _{{zy}}&\sigma _{z}\\\end{matrix}}}\right]]
The SI units of both stress tensor and stress vector are N/m2, corresponding to
the stress scalar. The unit vector is dimensionless.
The Cauchy stress tensor obeys the tensor transformation law under a change in
the system of coordinates. A graphical representation of this transformation
law is the Mohr's_circle for stress.
The Cauchy stress tensor is used for stress analysis of material bodies
experiencing small_deformations: It is a central concept in the linear_theory
of_elasticity. For large deformations, also called finite_deformations, other
measures of stress are required, such as the PiolaâKirchhoff_stress_tensor,
the Biot_stress_tensor, and the Kirchhoff_stress_tensor.
According to the principle of conservation_of_linear_momentum, if the continuum
body is in static equilibrium it can be demonstrated that the components of the
Cauchy stress tensor in every material point in the body satisfy the
equilibrium equations (Cauchy's_equations_of_motion for zero acceleration). At
the same time, according to the principle of conservation_of_angular_momentum,
equilibrium requires that the summation of moments with respect to an arbitrary
point is zero, which leads to the conclusion that the stress_tensor_is
symmetric, thus having only six independent stress components, instead of the
original nine.
There are certain invariants associated with the stress tensor, whose values do
not depend upon the coordinate system chosen, or the area element upon which
the stress tensor operates. These are the three eigenvalues of the stress
tensor, which are called the principal_stresses.
⁰
***** Contents *****
    * 1_EulerâCauchy_stress_principle_â_stress_vector
          o 1.1_Cauchyâs_postulate
          o 1.2_Cauchyâs_fundamental_lemma
    * 2_Cauchyâs_stress_theoremâstress_tensor
          o 2.1_Transformation_rule_of_the_stress_tensor
          o 2.2_Normal_and_shear_stresses
    * 3_Balance_laws_â_Cauchy's_equations_of_motion
          o 3.1_Cauchy's_first_law_of_motion
          o 3.2_Cauchy's_second_law_of_motion
    * 4_Principal_stresses_and_stress_invariants
    * 5_Maximum_and_minimum_shear_stresses
    * 6_Stress_deviator_tensor
          o 6.1_Invariants_of_the_stress_deviator_tensor
    * 7_Octahedral_stresses
    * 8_See_also
    * 9_References
***** EulerâCauchy stress principle â stress vector[edit] *****
Main article: Continuum_mechanics
Figure 2.1a Internal distribution of contact forces and couple stresses on a
differential     d S   {\displaystyle dS}  [dS] of the internal surface     S
{\displaystyle S}  [S] in a continuum, as a result of the interaction between
the two portions of the continuum separated by the surface
Figure 2.1b Internal distribution of contact forces and couple stresses on a
differential     d S   {\displaystyle dS}  [dS] of the internal surface     S
{\displaystyle S}  [S] in a continuum, as a result of the interaction between
the two portions of the continuum separated by the surface
Figure 2.1c Stress vector on an internal surface S with normal vector n.
Depending on the orientation of the plane under consideration, the stress
vector may not necessarily be perpendicular to that plane, i.e. parallel to
n    {\displaystyle \mathbf {n} }  [\mathbf {n} ], and can be resolved into two
components: one component normal to the plane, called normal stress
&#x03C3;   n      {\displaystyle \sigma _{\mathrm {n} }}  [\sigma _{{\mathrm
{n}}}], and another component parallel to this plane, called the shearing
stress     &#x03C4;   {\displaystyle \tau }  [\tau ].
The EulerâCauchy stress principle states that upon any surface (real or
imaginary) that divides the body, the action of one part of the body on the
other is equivalent (equipollent) to the system of distributed forces and
couples on the surface dividing the body,[2] and it is represented by a field
T   (  n  )     {\displaystyle \mathbf {T} ^{(\mathbf {n} )}}  [\mathbf{T}^{
(\mathbf{n})}], called the stress vector, defined on the surface     S
{\displaystyle S}  [S] and assumed to depend continuously on the surface's unit
vector      n    {\displaystyle \mathbf {n} }  [\mathbf {n} ].[3][4]:p.66â96
To formulate the EulerâCauchy stress principle, consider an imaginary surface
S   {\displaystyle S}  [S] passing through an internal material point     P
{\displaystyle P}  [P] dividing the continuous body into two segments, as seen
in Figure 2.1a or 2.1b (one may use either the cutting plane diagram or the
diagram with the arbitrary volume inside the continuum enclosed by the surface
S   {\displaystyle S}  [S]).
Following the classical dynamics of Newton and Euler, the motion of a material
body is produced by the action of externally applied forces which are assumed
to be of two kinds: surface_forces      F    {\displaystyle \mathbf {F} }
[\mathbf {F} ] and body_forces      b    {\displaystyle \mathbf {b} }  [\mathbf
b].[5] Thus, the total force       F     {\displaystyle {\mathcal {F}}}  [
{\mathcal {F}}] applied to a body or to a portion of the body can be expressed
as:
           F   =  b  +  F    {\displaystyle {\mathcal {F}}=\mathbf {b} +\mathbf
      {F} }  [\mathcal F = \mathbf b + \mathbf F]
Only surface forces will be discussed in this article as they are relevant to
the Cauchy stress tensor.
When the body is subjected to external surface forces or contact forces      F
{\displaystyle \mathbf {F} }  [\mathbf {F} ], following Euler's_equations_of
motion, internal contact forces and moments are transmitted from point to point
in the body, and from one segment to the other through the dividing surface
S   {\displaystyle S}  [S], due to the mechanical contact of one portion of the
continuum onto the other (Figure 2.1a and 2.1b). On an element of area
&#x0394; S   {\displaystyle \Delta S}  [\Delta S] containing     P
{\displaystyle P}  [P], with normal vector      n    {\displaystyle \mathbf {n}
}  [\mathbf {n} ], the force distribution is equipollent to a contact force
&#x0394;  F    {\displaystyle \Delta \mathbf {F} }  [{\displaystyle \Delta
\mathbf {F} }] exerted at point P and surface moment     &#x0394;  M
{\displaystyle \Delta \mathbf {M} }  [{\displaystyle \Delta \mathbf {M} }]. In
particular, the contact force is given by
         &#x0394;  F  =   T   (  n  )    &#x0394; S   {\displaystyle \Delta
      \mathbf {F} =\mathbf {T} ^{(\mathbf {n} )}\,\Delta S}  [\Delta\mathbf F=
      \mathbf T^{(\mathbf n)}\,\Delta S]
where       T   (  n  )     {\displaystyle \mathbf {T} ^{(\mathbf {n} )}}
[\mathbf {T} ^{(\mathbf {n} )}] is the mean surface traction.
Cauchy's stress principle asserts[6]:p.47â102 that as     &#x0394; S
{\displaystyle \Delta S}  [\Delta S] becomes very small and tends to zero the
ratio     &#x0394;  F   /  &#x0394; S   {\displaystyle \Delta \mathbf {F} /
\Delta S}  [{\displaystyle \Delta \mathbf {F} /\Delta S}] becomes     d  F   /
d S   {\displaystyle d\mathbf {F} /dS}  [{\displaystyle d\mathbf {F} /dS}] and
the couple stress vector     &#x0394;  M    {\displaystyle \Delta \mathbf {M} }
[{\displaystyle \Delta \mathbf {M} }] vanishes. In specific fields of continuum
mechanics the couple stress is assumed not to vanish; however, classical
branches of continuum mechanics address non-polar materials which do not
consider couple stresses and body moments.
The resultant vector     d  F   /  d S   {\displaystyle d\mathbf {F} /dS}  [
{\displaystyle d\mathbf {F} /dS}] is defined as the surface traction,[7] also
called stress vector,[8] traction,[4] or traction vector.[6] given by       T
(  n  )   =  T  i   (  n  )     e   i     {\displaystyle \mathbf {T} ^{(\mathbf
{n} )}=T_{i}^{(\mathbf {n} )}\mathbf {e} _{i}}  [{\displaystyle \mathbf {T} ^{
(\mathbf {n} )}=T_{i}^{(\mathbf {n} )}\mathbf {e} _{i}}] at the point     P
{\displaystyle P}  [P] associated with a plane with a normal vector      n
{\displaystyle \mathbf {n} }  [\mathbf {n} ]:
          T  i   (  n  )   =  lim  &#x0394; S &#x2192; 0      &#x0394;  F  i
      &#x0394; S    =    d  F  i     d S    .   {\displaystyle T_{i}^{(\mathbf
      {n} )}=\lim _{\Delta S\to 0}{\frac {\Delta F_{i}}{\Delta S}}={dF_{i}
      \over dS}.}  [T^{(\mathbf{n})}_i= \lim_{\Delta S \to 0} \frac {\Delta
      F_i}{\Delta S} = {dF_i \over dS}.]
This equation means that the stress vector depends on its location in the body
and the orientation of the plane on which it is acting.
This implies that the balancing action of internal contact forces generates a
contact force density or Cauchy traction field [5]      T  (  n  ,  x  , t )
{\displaystyle \mathbf {T} (\mathbf {n} ,\mathbf {x} ,t)}  [\mathbf {T}
(\mathbf {n} ,\mathbf {x} ,t)] that represents a distribution of internal
contact forces throughout the volume of the body in a particular configuration
of_the_body at a given time     t   {\displaystyle t}  [t]. It is not a vector
field because it depends not only on the position      x    {\displaystyle
\mathbf {x} }  [\mathbf {x} ] of a particular material point, but also on the
local orientation of the surface element as defined by its normal vector      n
{\displaystyle \mathbf {n} }  [\mathbf {n} ].[9]
Depending on the orientation of the plane under consideration, the stress
vector may not necessarily be perpendicular to that plane, i.e. parallel to
n    {\displaystyle \mathbf {n} }  [\mathbf {n} ], and can be resolved into two
components (Figure 2.1c):
    * one normal to the plane, called normal stress
           &#x03C3;   n     =  lim  &#x0394; S &#x2192; 0      &#x0394;  F   n
      &#x0394; S    =    d  F   n      d S    ,   {\displaystyle \mathbf
      {\sigma _{\mathrm {n} }} =\lim _{\Delta S\to 0}{\frac {\Delta F_{\mathrm
      {n} }}{\Delta S}}={\frac {dF_{\mathrm {n} }}{dS}},}  [\mathbf
      {\sigma_\mathrm{n}}= \lim_{\Delta S \to 0} \frac {\Delta F_\mathrm n}
      {\Delta S} = \frac{dF_\mathrm n}{dS},]
      where     d  F   n      {\displaystyle dF_{\mathrm {n} }}  [
      {\displaystyle dF_{\mathrm {n} }}] is the normal component of the force
      d  F    {\displaystyle d\mathbf {F} }  [{\displaystyle d\mathbf {F} }] to
      the differential area     d S   {\displaystyle dS}  [dS]
    * and the other parallel to this plane, called the shear stress
          &#x03C4;  =  lim  &#x0394; S &#x2192; 0      &#x0394;  F   s
      &#x0394; S    =    d  F   s      d S    ,   {\displaystyle \mathbf {\tau
      } =\lim _{\Delta S\to 0}{\frac {\Delta F_{\mathrm {s} }}{\Delta S}}=
      {\frac {dF_{\mathrm {s} }}{dS}},}  [\mathbf \tau= \lim_{\Delta S \to 0}
      \frac {\Delta F_\mathrm s}{\Delta S} = \frac{dF_\mathrm s}{dS},]
      where     d  F   s      {\displaystyle dF_{\mathrm {s} }}  [
      {\displaystyle dF_{\mathrm {s} }}] is the tangential component of the
      force     d  F    {\displaystyle d\mathbf {F} }  [{\displaystyle d\mathbf
      {F} }] to the differential surface area     d S   {\displaystyle dS}
      [dS]. The shear stress can be further decomposed into two mutually
      perpendicular vectors.
**** Cauchyâs postulate[edit] ****
According to the Cauchy Postulate, the stress vector       T   (  n  )
{\displaystyle \mathbf {T} ^{(\mathbf {n} )}}  [\mathbf{T}^{(\mathbf{n})}]
remains unchanged for all surfaces passing through the point     P
{\displaystyle P}  [P] and having the same normal vector      n
{\displaystyle \mathbf {n} }  [\mathbf {n} ] at     P   {\displaystyle P}  [P],
[7][10] i.e., having a common tangent at     P   {\displaystyle P}  [P]. This
means that the stress vector is a function of the normal vector      n
{\displaystyle \mathbf {n} }  [\mathbf {n} ] only, and is not influenced by the
curvature of the internal surfaces.
**** Cauchyâs fundamental lemma[edit] ****
A consequence of Cauchy's postulate is Cauchyâs Fundamental Lemma,[1][7][11]
also called the Cauchy reciprocal theorem,[12]:p.103â130 which states that
the stress vectors acting on opposite sides of the same surface are equal in
magnitude and opposite in direction. Cauchy's fundamental lemma is equivalent
to Newton's_third_law of motion of action and reaction, and is expressed as
         &#x2212;   T   (  n  )   =   T   ( &#x2212;  n  )   .   {\displaystyle
      -\mathbf {T} ^{(\mathbf {n} )}=\mathbf {T} ^{(-\mathbf {n} )}.}  [
      {\displaystyle -\mathbf {T} ^{(\mathbf {n} )}=\mathbf {T} ^{(-\mathbf {n}
      )}.}]
***** Cauchyâs stress theoremâstress tensor[edit] *****
The state of stress at a point in the body is then defined by all the stress
vectors T(n) associated with all planes (infinite in number) that pass through
that point.[13] However, according to Cauchyâs fundamental theorem,[11] also
called Cauchyâs stress theorem,[1] merely by knowing the stress vectors on
three mutually perpendicular planes, the stress vector on any other plane
passing through that point can be found through coordinate transformation
equations.
Cauchy's stress theorem states that there exists a second-order tensor_field Ï
(x, t), called the Cauchy stress tensor, independent of n, such that T is a
linear function of n:
           T   (  n  )   =  n  &#x22C5;  &#x03C3;    or    T  j   ( n )   =
      &#x03C3;  i j    n  i   .   {\displaystyle \mathbf {T} ^{(\mathbf {n}
      )}=\mathbf {n} \cdot {\boldsymbol {\sigma }}\quad {\text{or}}\quad T_{j}^
      {(n)}=\sigma _{ij}n_{i}.}  [{\displaystyle \mathbf {T} ^{(\mathbf {n}
      )}=\mathbf {n} \cdot {\boldsymbol {\sigma }}\quad {\text{or}}\quad T_{j}^
      {(n)}=\sigma _{ij}n_{i}.}]
This equation implies that the stress vector T(n) at any point P in a continuum
associated with a plane with normal unit vector n can be expressed as a
function of the stress vectors on the planes perpendicular to the coordinate
axes, i.e. in terms of the components Ïij of the stress tensor Ï.
To prove this expression, consider a tetrahedron with three faces oriented in
the coordinate planes, and with an infinitesimal area dA oriented in an
arbitrary direction specified by a normal unit vector n (Figure 2.2). The
tetrahedron is formed by slicing the infinitesimal element along an arbitrary
plane with unit normal n. The stress vector on this plane is denoted by T(n).
The stress vectors acting on the faces of the tetrahedron are denoted as T(e1),
T(e2), and T(e3), and are by definition the components Ïij of the stress
tensor Ï. This tetrahedron is sometimes called the Cauchy tetrahedron. The
equilibrium of forces, i.e. Euler's_first_law_of_motion (Newton's second law of
motion), gives:
           T   (  n  )    d A &#x2212;   T   (   e   1   )    d  A  1
      &#x2212;   T   (   e   2   )    d  A  2   &#x2212;   T   (   e   3   )
      d  A  3   = &#x03C1;  (    h 3   d A  )   a  ,   {\displaystyle \mathbf
      {T} ^{(\mathbf {n} )}\,dA-\mathbf {T} ^{(\mathbf {e} _{1})}\,dA_{1}-
      \mathbf {T} ^{(\mathbf {e} _{2})}\,dA_{2}-\mathbf {T} ^{(\mathbf {e} _
      {3})}\,dA_{3}=\rho \left({\frac {h}{3}}dA\right)\mathbf {a} ,}  [
      {\displaystyle \mathbf {T} ^{(\mathbf {n} )}\,dA-\mathbf {T} ^{(\mathbf
      {e} _{1})}\,dA_{1}-\mathbf {T} ^{(\mathbf {e} _{2})}\,dA_{2}-\mathbf {T}
      ^{(\mathbf {e} _{3})}\,dA_{3}=\rho \left({\frac {h}{3}}dA\right)\mathbf
      {a} ,}]
Figure 2.2. Stress vector acting on a plane with normal unit vector n.
A note on the sign convention: The tetrahedron is formed by slicing a
parallelepiped along an arbitrary plane n. So, the force acting on the plane n
is the reaction exerted by the other half of the parallelepiped and has an
opposite sign.
where the right-hand-side represents the product of the mass enclosed by the
tetrahedron and its acceleration: ρ is the density, a is the acceleration, and
h is the height of the tetrahedron, considering the plane n as the base. The
area of the faces of the tetrahedron perpendicular to the axes can be found by
projecting dA into each face (using the dot product):
         d  A  1   =  (   n  &#x22C5;   e   1    )  d A =  n  1    d A ,
      {\displaystyle dA_{1}=\left(\mathbf {n} \cdot \mathbf {e} _
      {1}\right)dA=n_{1}\;dA,}  [{\displaystyle dA_{1}=\left(\mathbf {n} \cdot
      \mathbf {e} _{1}\right)dA=n_{1}\;dA,}]
         d  A  2   =  (   n  &#x22C5;   e   2    )  d A =  n  2    d A ,
      {\displaystyle dA_{2}=\left(\mathbf {n} \cdot \mathbf {e} _
      {2}\right)dA=n_{2}\;dA,}  [{\displaystyle dA_{2}=\left(\mathbf {n} \cdot
      \mathbf {e} _{2}\right)dA=n_{2}\;dA,}]
         d  A  3   =  (   n  &#x22C5;   e   3    )  d A =  n  3    d A ,
      {\displaystyle dA_{3}=\left(\mathbf {n} \cdot \mathbf {e} _
      {3}\right)dA=n_{3}\;dA,}  [{\displaystyle dA_{3}=\left(\mathbf {n} \cdot
      \mathbf {e} _{3}\right)dA=n_{3}\;dA,}]
and then substituting into the equation to cancel out dA:
           T   (  n  )   &#x2212;   T   (   e   1   )    n  1   &#x2212;   T
      (   e   2   )    n  2   &#x2212;   T   (   e   3   )    n  3   = &#x03C1;
      (   h 3   )   a  .   {\displaystyle \mathbf {T} ^{(\mathbf {n} )}-\mathbf
      {T} ^{(\mathbf {e} _{1})}n_{1}-\mathbf {T} ^{(\mathbf {e} _{2})}n_{2}-
      \mathbf {T} ^{(\mathbf {e} _{3})}n_{3}=\rho \left({\frac {h}
      {3}}\right)\mathbf {a} .}  [{\displaystyle \mathbf {T} ^{(\mathbf {n} )}-
      \mathbf {T} ^{(\mathbf {e} _{1})}n_{1}-\mathbf {T} ^{(\mathbf {e} _
      {2})}n_{2}-\mathbf {T} ^{(\mathbf {e} _{3})}n_{3}=\rho \left({\frac {h}
      {3}}\right)\mathbf {a} .}]
To consider the limiting case as the tetrahedron shrinks to a point, h must go
to 0 (intuitively, the plane n is translated along n toward O). As a result,
the right-hand-side of the equation approaches 0, so
           T   (  n  )   =   T   (   e   1   )    n  1   +   T   (   e   2   )
      n  2   +   T   (   e   3   )    n  3   .   {\displaystyle \mathbf {T} ^{
      (\mathbf {n} )}=\mathbf {T} ^{(\mathbf {e} _{1})}n_{1}+\mathbf {T} ^{
      (\mathbf {e} _{2})}n_{2}+\mathbf {T} ^{(\mathbf {e} _{3})}n_{3}.}  [
      {\displaystyle \mathbf {T} ^{(\mathbf {n} )}=\mathbf {T} ^{(\mathbf {e} _
      {1})}n_{1}+\mathbf {T} ^{(\mathbf {e} _{2})}n_{2}+\mathbf {T} ^{(\mathbf
      {e} _{3})}n_{3}.}]
Assuming a material element (Figure 2.3) with planes perpendicular to the
coordinate axes of a Cartesian coordinate system, the stress vectors associated
with each of the element planes, i.e. T(e1), T(e2), and T(e3) can be decomposed
into a normal component and two shear components, i.e. components in the
direction of the three coordinate axes. For the particular case of a surface
with normal unit_vector oriented in the direction of the x1-axis, denote the
normal stress by Ï11, and the two shear stresses as Ï12 and Ï13:
           T   (   e   1   )   =  T  1   (   e   1   )     e   1   +  T  2
      (   e   1   )     e   2   +  T  3   (   e   1   )     e   3   =  &#x03C3;
      11     e   1   +  &#x03C3;  12     e   2   +  &#x03C3;  13     e   3   ,
      {\displaystyle \mathbf {T} ^{(\mathbf {e} _{1})}=T_{1}^{(\mathbf {e} _
      {1})}\mathbf {e} _{1}+T_{2}^{(\mathbf {e} _{1})}\mathbf {e} _{2}+T_{3}^{
      (\mathbf {e} _{1})}\mathbf {e} _{3}=\sigma _{11}\mathbf {e} _{1}+\sigma _
      {12}\mathbf {e} _{2}+\sigma _{13}\mathbf {e} _{3},}  [\mathbf{T}^{
      (\mathbf{e}_1)}= T_1^{(\mathbf{e}_1)}\mathbf{e}_1 + T_2^{(\mathbf{e}_1)}
      \mathbf{e}_2 + T_3^{(\mathbf{e}_1)} \mathbf{e}_3 = \sigma_{11} \mathbf
      {e}_1 + \sigma_{12} \mathbf{e}_2 + \sigma_{13} \mathbf{e}_3,]
           T   (   e   2   )   =  T  1   (   e   2   )     e   1   +  T  2
      (   e   2   )     e   2   +  T  3   (   e   2   )     e   3   =  &#x03C3;
      21     e   1   +  &#x03C3;  22     e   2   +  &#x03C3;  23     e   3   ,
      {\displaystyle \mathbf {T} ^{(\mathbf {e} _{2})}=T_{1}^{(\mathbf {e} _
      {2})}\mathbf {e} _{1}+T_{2}^{(\mathbf {e} _{2})}\mathbf {e} _{2}+T_{3}^{
      (\mathbf {e} _{2})}\mathbf {e} _{3}=\sigma _{21}\mathbf {e} _{1}+\sigma _
      {22}\mathbf {e} _{2}+\sigma _{23}\mathbf {e} _{3},}  [\mathbf{T}^{
      (\mathbf{e}_2)}= T_1^{(\mathbf{e}_2)}\mathbf{e}_1 + T_2^{(\mathbf{e}_2)}
      \mathbf{e}_2 + T_3^{(\mathbf{e}_2)} \mathbf{e}_3=\sigma_{21} \mathbf{e}_1
      + \sigma_{22} \mathbf{e}_2 + \sigma_{23} \mathbf{e}_3,]
           T   (   e   3   )   =  T  1   (   e   3   )     e   1   +  T  2
      (   e   3   )     e   2   +  T  3   (   e   3   )     e   3   =  &#x03C3;
      31     e   1   +  &#x03C3;  32     e   2   +  &#x03C3;  33     e   3   ,
      {\displaystyle \mathbf {T} ^{(\mathbf {e} _{3})}=T_{1}^{(\mathbf {e} _
      {3})}\mathbf {e} _{1}+T_{2}^{(\mathbf {e} _{3})}\mathbf {e} _{2}+T_{3}^{
      (\mathbf {e} _{3})}\mathbf {e} _{3}=\sigma _{31}\mathbf {e} _{1}+\sigma _
      {32}\mathbf {e} _{2}+\sigma _{33}\mathbf {e} _{3},}  [\mathbf{T}^{
      (\mathbf{e}_3)}= T_1^{(\mathbf{e}_3)}\mathbf{e}_1 + T_2^{(\mathbf{e}_3)}
      \mathbf{e}_2 + T_3^{(\mathbf{e}_3)} \mathbf{e}_3=\sigma_{31} \mathbf{e}_1
      + \sigma_{32} \mathbf{e}_2 + \sigma_{33} \mathbf{e}_3,]
In index notation this is
           T   (   e   i   )   =  T  j   (   e   i   )     e   j   =  &#x03C3;
      i j     e   j   .   {\displaystyle \mathbf {T} ^{(\mathbf {e} _{i})}=T_
      {j}^{(\mathbf {e} _{i})}\mathbf {e} _{j}=\sigma _{ij}\mathbf {e} _{j}.}
      [\mathbf{T}^{(\mathbf{e}_i)}= T_j^{(\mathbf{e}_i)} \mathbf{e}_j = \sigma_
      {ij} \mathbf{e}_j.]
The nine components σij of the stress vectors are the components of a second-
order Cartesian tensor called the Cauchy stress tensor, which completely
defines the state of stress at a point and is given by
          &#x03C3;  =  &#x03C3;  i j   =  [       T   (   e   1   )         T
      (   e   2   )         T   (   e   3   )       ]  =  [      &#x03C3;  11
      &#x03C3;  12      &#x03C3;  13        &#x03C3;  21      &#x03C3;  22
      &#x03C3;  23        &#x03C3;  31      &#x03C3;  32      &#x03C3;  33
      ]  &#x2261;  [      &#x03C3;  x x      &#x03C3;  x y      &#x03C3;  x z
      &#x03C3;  y x      &#x03C3;  y y      &#x03C3;  y z        &#x03C3;  z x
      &#x03C3;  z y      &#x03C3;  z z       ]  &#x2261;  [      &#x03C3;  x
      &#x03C4;  x y      &#x03C4;  x z        &#x03C4;  y x      &#x03C3;  y
      &#x03C4;  y z        &#x03C4;  z x      &#x03C4;  z y      &#x03C3;  z
      ]  ,   {\displaystyle {\boldsymbol {\sigma }}=\sigma _{ij}=\left[{\begin
      {matrix}\mathbf {T} ^{(\mathbf {e} _{1})}\\\mathbf {T} ^{(\mathbf {e} _
      {2})}\\\mathbf {T} ^{(\mathbf {e} _{3})}\\\end{matrix}}\right]=\left[
      {\begin{matrix}\sigma _{11}&\sigma _{12}&\sigma _{13}\\\sigma _
      {21}&\sigma _{22}&\sigma _{23}\\\sigma _{31}&\sigma _{32}&\sigma _
      {33}\\\end{matrix}}\right]\equiv \left[{\begin{matrix}\sigma _{xx}&\sigma
      _{xy}&\sigma _{xz}\\\sigma _{yx}&\sigma _{yy}&\sigma _{yz}\\\sigma _
      {zx}&\sigma _{zy}&\sigma _{zz}\\\end{matrix}}\right]\equiv \left[{\begin
      {matrix}\sigma _{x}&\tau _{xy}&\tau _{xz}\\\tau _{yx}&\sigma _{y}&\tau _
      {yz}\\\tau _{zx}&\tau _{zy}&\sigma _{z}\\\end{matrix}}\right],}
      [\boldsymbol{\sigma}= \sigma_{ij} = \left[{\begin{matrix} \mathbf{T}^{
      (\mathbf{e}_1)} \\
      \mathbf{T}^{(\mathbf{e}_2)} \\
      \mathbf{T}^{(\mathbf{e}_3)} \\
      \end{matrix}}\right] =
      \left[{\begin{matrix}
      \sigma _{11} & \sigma _{12} & \sigma _{13} \\
      \sigma _{21} & \sigma _{22} & \sigma _{23} \\
      \sigma _{31} & \sigma _{32} & \sigma _{33} \\
      \end{matrix}}\right] \equiv \left[{\begin{matrix}
      \sigma _{xx} & \sigma _{xy} & \sigma _{xz} \\
      \sigma _{yx} & \sigma _{yy} & \sigma _{yz} \\
      \sigma _{zx} & \sigma _{zy} & \sigma _{zz} \\
      \end{matrix}}\right] \equiv \left[{\begin{matrix}
      \sigma _x & \tau _{xy} & \tau _{xz} \\
      \tau _{yx} & \sigma _y & \tau _{yz} \\
      \tau _{zx} & \tau _{zy} & \sigma _z \\
      \end{matrix}}\right],]
where σ11, σ22, and σ33 are normal stresses, and σ12, σ13, σ21, σ23, σ31, and
σ32 are shear stresses. The first index i indicates that the stress acts on a
plane normal to the Xi -axis, and the second index j denotes the direction in
which the stress acts (For example, Ï12 implies that the stress is acting on
the plane that is normal to the 1st axis i.e.;X1 and acts along the 2nd axis
i.e.;X2). A stress component is positive if it acts in the positive direction
of the coordinate axes, and if the plane where it acts has an outward normal
vector pointing in the positive coordinate direction.
Thus, using the components of the stress tensor
               T   (  n  )      =   T   (   e   1   )    n  1   +   T   (   e
      2   )    n  2   +   T   (   e   3   )    n  3         =  &#x2211;  i = 1
      3     T   (   e   i   )    n  i         =  (   &#x03C3;  i j     e   j
      )   n  i         =  &#x03C3;  i j    n  i     e   j
      {\displaystyle {\begin{aligned}\mathbf {T} ^{(\mathbf {n} )}&=\mathbf {T}
      ^{(\mathbf {e} _{1})}n_{1}+\mathbf {T} ^{(\mathbf {e} _{2})}n_{2}+\mathbf
      {T} ^{(\mathbf {e} _{3})}n_{3}\\&=\sum _{i=1}^{3}\mathbf {T} ^{(\mathbf
      {e} _{i})}n_{i}\\&=\left(\sigma _{ij}\mathbf {e} _{j}\right)n_
      {i}\\&=\sigma _{ij}n_{i}\mathbf {e} _{j}\end{aligned}}}  [\begin{align}
      \mathbf{T}^{(\mathbf{n})} &= \mathbf{T}^{(\mathbf{e}_1)}n_1 + \mathbf{T}^
      {(\mathbf{e}_2)}n_2 + \mathbf{T}^{(\mathbf{e}_3)}n_3 \\
      & = \sum_{i=1}^3 \mathbf{T}^{(\mathbf{e}_i)}n_i \\
      &= \left( \sigma_{ij}\mathbf{e}_j \right)n_i \\
      &= \sigma_{ij}n_i\mathbf{e}_j
      \end{align}]
or, equivalently,
          T  j   (  n  )   =  &#x03C3;  i j    n  i   .   {\displaystyle T_{j}^
      {(\mathbf {n} )}=\sigma _{ij}n_{i}.}  [T_j^{(\mathbf n)}= \sigma_
      {ij}n_i.]
Alternatively, in matrix form we have
          [      T  1   (  n  )      T  2   (  n  )      T  3   (  n  )       ]
      =  [      n  1      n  2      n  3       ]  &#x22C5;  [      &#x03C3;  11
      &#x03C3;  12      &#x03C3;  13        &#x03C3;  21      &#x03C3;  22
      &#x03C3;  23        &#x03C3;  31      &#x03C3;  32      &#x03C3;  33
      ]  .   {\displaystyle \left[{\begin{matrix}T_{1}^{(\mathbf {n} )}&T_{2}^{
      (\mathbf {n} )}&T_{3}^{(\mathbf {n} )}\end{matrix}}\right]=\left[{\begin
      {matrix}n_{1}&n_{2}&n_{3}\end{matrix}}\right]\cdot \left[{\begin
      {matrix}\sigma _{11}&\sigma _{12}&\sigma _{13}\\\sigma _{21}&\sigma _
      {22}&\sigma _{23}\\\sigma _{31}&\sigma _{32}&\sigma _{33}\\\end
      {matrix}}\right].}  [\left[{\begin{matrix}
      T^{(\mathbf n)}_1 & T^{(\mathbf n)}_2 & T^{(\mathbf n)}_3\end
      {matrix}}\right]=\left[{\begin{matrix}
      n_1 & n_2 & n_3
      \end{matrix}}\right]\cdot
      \left[{\begin{matrix}
      \sigma _{11} & \sigma _{12} & \sigma _{13} \\
      \sigma _{21} & \sigma _{22} & \sigma _{23} \\
      \sigma _{31} & \sigma _{32} & \sigma _{33} \\
      \end{matrix}}\right].]
The Voigt_notation representation of the Cauchy stress tensor takes advantage
of the symmetry of the stress tensor to express the stress as a six-dimensional
vector of the form:
          &#x03C3;  =    [     &#x03C3;  1      &#x03C3;  2      &#x03C3;  3
      &#x03C3;  4      &#x03C3;  5      &#x03C3;  6      ]    T   &#x2261;
      [     &#x03C3;  11      &#x03C3;  22      &#x03C3;  33      &#x03C3;  23
      &#x03C3;  13      &#x03C3;  12      ]    T   .   {\displaystyle
      {\boldsymbol {\sigma }}={\begin{bmatrix}\sigma _{1}&\sigma _{2}&\sigma _
      {3}&\sigma _{4}&\sigma _{5}&\sigma _{6}\end{bmatrix}}^{T}\equiv {\begin
      {bmatrix}\sigma _{11}&\sigma _{22}&\sigma _{33}&\sigma _{23}&\sigma _
      {13}&\sigma _{12}\end{bmatrix}}^{T}.}  [{\displaystyle {\boldsymbol
      {\sigma }}={\begin{bmatrix}\sigma _{1}&\sigma _{2}&\sigma _{3}&\sigma _
      {4}&\sigma _{5}&\sigma _{6}\end{bmatrix}}^{T}\equiv {\begin
      {bmatrix}\sigma _{11}&\sigma _{22}&\sigma _{33}&\sigma _{23}&\sigma _
      {13}&\sigma _{12}\end{bmatrix}}^{T}.}]
The Voigt notation is used extensively in representing stressâstrain
relations in solid mechanics and for computational efficiency in numerical
structural mechanics software.
**** Transformation rule of the stress tensor[edit] ****
It can be shown that the stress tensor is a contravariant second order tensor,
which is a statement of how it transforms under a change of the coordinate
system. From an xi-system to an xi'-system, the components Ïij in the initial
system are transformed into the components Ïij' in the new system according to
the tensor transformation rule (Figure 2.4):
          &#x03C3;  i j  &#x2032;  =  a  i m    a  j n    &#x03C3;  m n     or
      &#x03C3;  &#x2032;  =  A   &#x03C3;    A   T   ,   {\displaystyle \sigma
      '_{ij}=a_{im}a_{jn}\sigma _{mn}\quad {\text{or}}\quad {\boldsymbol
      {\sigma }}'=\mathbf {A} {\boldsymbol {\sigma }}\mathbf {A} ^{T},}
      [\sigma'_{ij}=a_{im}a_{jn}\sigma_{mn} \quad \text{or} \quad \boldsymbol
      {\sigma}' = \mathbf A \boldsymbol{\sigma} \mathbf A^{T},]
where A is a rotation_matrix with components aij. In matrix form this is
          [      &#x03C3;  11  &#x2032;     &#x03C3;  12  &#x2032;     &#x03C3;
      13  &#x2032;       &#x03C3;  21  &#x2032;     &#x03C3;  22  &#x2032;
      &#x03C3;  23  &#x2032;       &#x03C3;  31  &#x2032;     &#x03C3;  32
      &#x2032;     &#x03C3;  33  &#x2032;      ]  =  [      a  11      a  12
      a  13        a  21      a  22      a  23        a  31      a  32      a
      33       ]   [      &#x03C3;  11      &#x03C3;  12      &#x03C3;  13
      &#x03C3;  21      &#x03C3;  22      &#x03C3;  23        &#x03C3;  31
      &#x03C3;  32      &#x03C3;  33       ]   [      a  11      a  21      a
      31        a  12      a  22      a  32        a  13      a  23      a  33
      ]  .   {\displaystyle \left[{\begin{matrix}\sigma '_{11}&\sigma '_
      {12}&\sigma '_{13}\\\sigma '_{21}&\sigma '_{22}&\sigma '_{23}\\\sigma '_
      {31}&\sigma '_{32}&\sigma '_{33}\\\end{matrix}}\right]=\left[{\begin
      {matrix}a_{11}&a_{12}&a_{13}\\a_{21}&a_{22}&a_{23}\\a_{31}&a_{32}&a_
      {33}\\\end{matrix}}\right]\left[{\begin{matrix}\sigma _{11}&\sigma _
      {12}&\sigma _{13}\\\sigma _{21}&\sigma _{22}&\sigma _{23}\\\sigma _
      {31}&\sigma _{32}&\sigma _{33}\\\end{matrix}}\right]\left[{\begin
      {matrix}a_{11}&a_{21}&a_{31}\\a_{12}&a_{22}&a_{32}\\a_{13}&a_{23}&a_
      {33}\\\end{matrix}}\right].}  [\left[{{\begin{matrix}\sigma '_{
      {11}}&\sigma '_{{12}}&\sigma '_{{13}}\\\sigma '_{{21}}&\sigma '_{
      {22}}&\sigma '_{{23}}\\\sigma '_{{31}}&\sigma '_{{32}}&\sigma '_{
      {33}}\\\end{matrix}}}\right]=\left[{{\begin{matrix}a_{{11}}&a_{{12}}&a_{
      {13}}\\a_{{21}}&a_{{22}}&a_{{23}}\\a_{{31}}&a_{{32}}&a_{{33}}\\\end
      {matrix}}}\right]\left[{{\begin{matrix}\sigma _{{11}}&\sigma _{
      {12}}&\sigma _{{13}}\\\sigma _{{21}}&\sigma _{{22}}&\sigma _{
      {23}}\\\sigma _{{31}}&\sigma _{{32}}&\sigma _{{33}}\\\end
      {matrix}}}\right]\left[{{\begin{matrix}a_{{11}}&a_{{21}}&a_{{31}}\\a_{
      {12}}&a_{{22}}&a_{{32}}\\a_{{13}}&a_{{23}}&a_{{33}}\\\end
      {matrix}}}\right].]
Figure 2.4 Transformation of the stress tensor
Expanding the matrix_operation, and simplifying terms using the symmetry_of_the
stress_tensor, gives
          &#x03C3;  11  &#x2032;  =  a  11   2    &#x03C3;  11   +  a  12   2
      &#x03C3;  22   +  a  13   2    &#x03C3;  33   + 2  a  11    a  12
      &#x03C3;  12   + 2  a  11    a  13    &#x03C3;  13   + 2  a  12    a  13
      &#x03C3;  23   ,   {\displaystyle \sigma _{11}'=a_{11}^{2}\sigma _{11}+a_
      {12}^{2}\sigma _{22}+a_{13}^{2}\sigma _{33}+2a_{11}a_{12}\sigma _{12}+2a_
      {11}a_{13}\sigma _{13}+2a_{12}a_{13}\sigma _{23},}  [\sigma_{11}' = a_
      {11}^2\sigma_{11}+a_{12}^2\sigma_{22}+a_{13}^2\sigma_{33}+2a_{11}a_
      {12}\sigma_{12}+2a_{11}a_{13}\sigma_{13}+2a_{12}a_{13}\sigma_{23},]
          &#x03C3;  22  &#x2032;  =  a  21   2    &#x03C3;  11   +  a  22   2
      &#x03C3;  22   +  a  23   2    &#x03C3;  33   + 2  a  21    a  22
      &#x03C3;  12   + 2  a  21    a  23    &#x03C3;  13   + 2  a  22    a  23
      &#x03C3;  23   ,   {\displaystyle \sigma _{22}'=a_{21}^{2}\sigma _{11}+a_
      {22}^{2}\sigma _{22}+a_{23}^{2}\sigma _{33}+2a_{21}a_{22}\sigma _{12}+2a_
      {21}a_{23}\sigma _{13}+2a_{22}a_{23}\sigma _{23},}  [\sigma_{22}' = a_
      {21}^2\sigma_{11}+a_{22}^2\sigma_{22}+a_{23}^2\sigma_{33}+2a_{21}a_
      {22}\sigma_{12}+2a_{21}a_{23}\sigma_{13}+2a_{22}a_{23}\sigma_{23},]
          &#x03C3;  33  &#x2032;  =  a  31   2    &#x03C3;  11   +  a  32   2
      &#x03C3;  22   +  a  33   2    &#x03C3;  33   + 2  a  31    a  32
      &#x03C3;  12   + 2  a  31    a  33    &#x03C3;  13   + 2  a  32    a  33
      &#x03C3;  23   ,   {\displaystyle \sigma _{33}'=a_{31}^{2}\sigma _{11}+a_
      {32}^{2}\sigma _{22}+a_{33}^{2}\sigma _{33}+2a_{31}a_{32}\sigma _{12}+2a_
      {31}a_{33}\sigma _{13}+2a_{32}a_{33}\sigma _{23},}  [\sigma_{33}' = a_
      {31}^2\sigma_{11}+a_{32}^2\sigma_{22}+a_{33}^2\sigma_{33}+2a_{31}a_
      {32}\sigma_{12}+2a_{31}a_{33}\sigma_{13}+2a_{32}a_{33}\sigma_{23},]
              &#x03C3;  12  &#x2032;  =    a  11    a  21    &#x03C3;  11   +
      a  12    a  22    &#x03C3;  22   +  a  13    a  23    &#x03C3;  33
      + (  a  11    a  22   +  a  12    a  21   )  &#x03C3;  12   + (  a  12
      a  23   +  a  13    a  22   )  &#x03C3;  23   + (  a  11    a  23   +  a
      13    a  21   )  &#x03C3;  13   ,       {\displaystyle {\begin
      {aligned}\sigma _{12}'=&a_{11}a_{21}\sigma _{11}+a_{12}a_{22}\sigma _
      {22}+a_{13}a_{23}\sigma _{33}\\&+(a_{11}a_{22}+a_{12}a_{21})\sigma _{12}+
      (a_{12}a_{23}+a_{13}a_{22})\sigma _{23}+(a_{11}a_{23}+a_{13}a_{21})\sigma
      _{13},\end{aligned}}}  [\begin{align}
      \sigma_{12}' = &a_{11}a_{21}\sigma_{11}+a_{12}a_{22}\sigma_{22}+a_{13}a_
      {23}\sigma_{33}\\
      &+(a_{11}a_{22}+a_{12}a_{21})\sigma_{12}+(a_{12}a_{23}+a_{13}a_
      {22})\sigma_{23}+(a_{11}a_{23}+a_{13}a_{21})\sigma_{13},
      \end{align}]
              &#x03C3;  23  &#x2032;  =    a  21    a  31    &#x03C3;  11   +
      a  22    a  32    &#x03C3;  22   +  a  23    a  33    &#x03C3;  33
      + (  a  21    a  32   +  a  22    a  31   )  &#x03C3;  12   + (  a  22
      a  33   +  a  23    a  32   )  &#x03C3;  23   + (  a  21    a  33   +  a
      23    a  31   )  &#x03C3;  13   ,       {\displaystyle {\begin
      {aligned}\sigma _{23}'=&a_{21}a_{31}\sigma _{11}+a_{22}a_{32}\sigma _
      {22}+a_{23}a_{33}\sigma _{33}\\&+(a_{21}a_{32}+a_{22}a_{31})\sigma _{12}+
      (a_{22}a_{33}+a_{23}a_{32})\sigma _{23}+(a_{21}a_{33}+a_{23}a_{31})\sigma
      _{13},\end{aligned}}}  [\begin{align}
      \sigma_{23}' = &a_{21}a_{31}\sigma_{11}+a_{22}a_{32}\sigma_{22}+a_{23}a_
      {33}\sigma_{33}\\
      &+(a_{21}a_{32}+a_{22}a_{31})\sigma_{12}+(a_{22}a_{33}+a_{23}a_
      {32})\sigma_{23}+(a_{21}a_{33}+a_{23}a_{31})\sigma_{13},\end{align}]
              &#x03C3;  13  &#x2032;  =    a  11    a  31    &#x03C3;  11   +
      a  12    a  32    &#x03C3;  22   +  a  13    a  33    &#x03C3;  33
      + (  a  11    a  32   +  a  12    a  31   )  &#x03C3;  12   + (  a  12
      a  33   +  a  13    a  32   )  &#x03C3;  23   + (  a  11    a  33   +  a
      13    a  31   )  &#x03C3;  13   .       {\displaystyle {\begin
      {aligned}\sigma _{13}'=&a_{11}a_{31}\sigma _{11}+a_{12}a_{32}\sigma _
      {22}+a_{13}a_{33}\sigma _{33}\\&+(a_{11}a_{32}+a_{12}a_{31})\sigma _{12}+
      (a_{12}a_{33}+a_{13}a_{32})\sigma _{23}+(a_{11}a_{33}+a_{13}a_{31})\sigma
      _{13}.\end{aligned}}}  [\begin{align}
      \sigma_{13}' = &a_{11}a_{31}\sigma_{11}+a_{12}a_{32}\sigma_{22}+a_{13}a_
      {33}\sigma_{33}\\
      &+(a_{11}a_{32}+a_{12}a_{31})\sigma_{12}+(a_{12}a_{33}+a_{13}a_
      {32})\sigma_{23}+(a_{11}a_{33}+a_{13}a_{31})\sigma_{13}.\end{align}]
The Mohr_circle for stress is a graphical representation of this transformation
of stresses.
**** Normal and shear stresses[edit] ****
The magnitude of the normal stress component σn of any stress vector T(n)
acting on an arbitrary plane with normal unit vector n at a given point, in
terms of the components σij of the stress tensor Ï, is the dot_product of the
stress vector and the normal unit vector:
              &#x03C3;   n       =   T   (  n  )   &#x22C5;  n        =  T  i
      (  n  )    n  i         =  &#x03C3;  i j    n  i    n  j   .
      {\displaystyle {\begin{aligned}\sigma _{\mathrm {n} }&=\mathbf {T} ^{
      (\mathbf {n} )}\cdot \mathbf {n} \\&=T_{i}^{(\mathbf {n} )}n_
      {i}\\&=\sigma _{ij}n_{i}n_{j}.\end{aligned}}}  [\begin{align}
      \sigma_\mathrm{n} &= \mathbf{T}^{(\mathbf{n})}\cdot \mathbf{n} \\
      &=T^{(\mathbf n)}_i n_i \\
      &=\sigma_{ij}n_i n_j.
      \end{align}]
The magnitude of the shear stress component τn, acting orthogonal to the vector
n, can then be found using the Pythagorean_theorem:
              &#x03C4;   n       =     (  T  (  n  )   )   2   &#x2212;
      &#x03C3;   n    2           =    T  i   (  n  )    T  i   (  n  )
      &#x2212;  &#x03C3;   n    2     ,       {\displaystyle {\begin
      {aligned}\tau _{\mathrm {n} }&={\sqrt {\left(T^{(\mathbf {n} )}\right)^
      {2}-\sigma _{\mathrm {n} }^{2}}}\\&={\sqrt {T_{i}^{(\mathbf {n} )}T_{i}^{
      (\mathbf {n} )}-\sigma _{\mathrm {n} }^{2}}},\end{aligned}}}  [\begin
      {align}
      \tau_\mathrm{n} &=\sqrt{ \left( T^{(\mathbf n)} \right)^2-\sigma_\mathrm
      {n}^2} \\
      &= \sqrt{T_i^{(\mathbf n)}T_i^{(\mathbf n)}-\sigma_\mathrm{n}^2},
      \end{align}]
where
           (  T  (  n  )   )   2   =  T  i   (  n  )    T  i   (  n  )   =
      (   &#x03C3;  i j    n  j    )   (   &#x03C3;  i k    n  k    )  =
      &#x03C3;  i j    &#x03C3;  i k    n  j    n  k   .   {\displaystyle \left
      (T^{(\mathbf {n} )}\right)^{2}=T_{i}^{(\mathbf {n} )}T_{i}^{(\mathbf {n}
      )}=\left(\sigma _{ij}n_{j}\right)\left(\sigma _{ik}n_{k}\right)=\sigma _
      {ij}\sigma _{ik}n_{j}n_{k}.}  [\left( T^{(\mathbf n)} \right)^2 = T_i^{
      (\mathbf n)} T_i^{(\mathbf n)} = \left( \sigma_{ij} n_j \right) \left
      (\sigma_{ik} n_k \right) = \sigma_{ij} \sigma_{ik} n_j n_k.]
***** Balance laws â Cauchy's equations of motion[edit] *****
Figure 4. Continuum body in equilibrium
**** Cauchy's first law of motion[edit] ****
According to the principle of conservation_of_linear_momentum, if the continuum
body is in static equilibrium it can be demonstrated that the components of the
Cauchy stress tensor in every material point in the body satisfy the
equilibrium equations.
          &#x03C3;  j i , j   +  F  i   = 0   {\displaystyle \sigma _{ji,j}+F_
      {i}=0}  [{\displaystyle \sigma _{ji,j}+F_{i}=0}]
For example, for a hydrostatic_fluid in equilibrium conditions, the stress
tensor takes on the form:
           &#x03C3;  i j    = &#x2212; p   &#x03B4;  i j    ,   {\displaystyle
      {\sigma _{ij}}=-p{\delta _{ij}},}  [{\displaystyle {\sigma _{ij}}=-p
      {\delta _{ij}},}]
where     p   {\displaystyle p}  [p] is the hydrostatic pressure, and
&#x03B4;  i j    &#xA0;   {\displaystyle {\delta _{ij}}\ }  [{\delta_{ij}}\ ]
is the kronecker_delta.
      Derivation of equilibrium equations
      Consider a continuum body (see Figure 4) occupying a volume     V
      {\displaystyle V}  [V], having a surface area     S   {\displaystyle S}
      [S], with defined traction or surface forces      T  i   ( n )
      {\displaystyle T_{i}^{(n)}}  [{\displaystyle T_{i}^{(n)}}] per unit area
      acting on every point of the body surface, and body forces      F  i
      {\displaystyle F_{i}}  [F_{i}] per unit of volume on every point within
      the volume     V   {\displaystyle V}  [V]. Thus, if the body is in
      equilibrium the resultant force acting on the volume is zero, thus:
                &#x222B;  S    T  i   ( n )   d S +  &#x222B;  V    F  i   d V
            = 0   {\displaystyle \int _{S}T_{i}^{(n)}dS+\int _{V}F_{i}dV=0}  [
            {\displaystyle \int _{S}T_{i}^{(n)}dS+\int _{V}F_{i}dV=0}]
      By definition the stress vector is      T  i   ( n )   =  &#x03C3;  j i
      n  j     {\displaystyle T_{i}^{(n)}=\sigma _{ji}n_{j}}  [{\displaystyle
      T_{i}^{(n)}=\sigma _{ji}n_{j}}], then
                &#x222B;  S    &#x03C3;  j i    n  j    d S +  &#x222B;  V    F
            i    d V = 0   {\displaystyle \int _{S}\sigma _{ji}n_{j}\,dS+\int _
            {V}F_{i}\,dV=0}  [{\displaystyle \int _{S}\sigma _{ji}n_
            {j}\,dS+\int _{V}F_{i}\,dV=0}]
      Using the Gauss's_divergence_theorem to convert a surface integral to a
      volume integral gives
                &#x222B;  V    &#x03C3;  j i , j    d V +  &#x222B;  V    F  i
            d V = 0   {\displaystyle \int _{V}\sigma _{ji,j}\,dV+\int _{V}F_
            {i}\,dV=0}  [{\displaystyle \int _{V}\sigma _{ji,j}\,dV+\int _{V}F_
            {i}\,dV=0}]
                &#x222B;  V   (  &#x03C3;  j i , j   +  F  i    ) d V = 0
            {\displaystyle \int _{V}(\sigma _{ji,j}+F_{i}\,)dV=0}  [
            {\displaystyle \int _{V}(\sigma _{ji,j}+F_{i}\,)dV=0}]
      For an arbitrary volume the integral vanishes, and we have the
      equilibrium equations
                &#x03C3;  j i , j   +  F  i   = 0   {\displaystyle \sigma _
            {ji,j}+F_{i}=0}  [{\displaystyle \sigma _{ji,j}+F_{i}=0}]
**** Cauchy's second law of motion[edit] ****
According to the principle of conservation_of_angular_momentum, equilibrium
requires that the summation of moments with respect to an arbitrary point is
zero, which leads to the conclusion that the stress tensor is symmetric, thus
having only six independent stress components, instead of the original nine:
          &#x03C3;  i j   =  &#x03C3;  j i     {\displaystyle \sigma _
      {ij}=\sigma _{ji}}  [{\displaystyle \sigma _{ij}=\sigma _{ji}}]
      Derivation of symmetry of the stress tensor
      Summing moments about point O (Figure 4) the resultant moment is zero as
      the body is in equilibrium. Thus,
                    M  O      =  &#x222B;  S   (  r  &#x00D7;  T  ) d S +
            &#x222B;  V   (  r  &#x00D7;  F  ) d V = 0     0    =  &#x222B;  S
            &#x03B5;  i j k    x  j    T  k   ( n )   d S +  &#x222B;  V
            &#x03B5;  i j k    x  j    F  k   d V       {\displaystyle {\begin
            {aligned}M_{O}&=\int _{S}(\mathbf {r} \times \mathbf {T} )dS+\int _
            {V}(\mathbf {r} \times \mathbf {F} )dV=0\\0&=\int _{S}\varepsilon _
            {ijk}x_{j}T_{k}^{(n)}dS+\int _{V}\varepsilon _{ijk}x_{j}F_
            {k}dV\\\end{aligned}}}  [{\displaystyle {\begin{aligned}M_{O}&=\int
            _{S}(\mathbf {r} \times \mathbf {T} )dS+\int _{V}(\mathbf {r}
            \times \mathbf {F} )dV=0\\0&=\int _{S}\varepsilon _{ijk}x_{j}T_{k}^
            {(n)}dS+\int _{V}\varepsilon _{ijk}x_{j}F_{k}dV\\\end{aligned}}}]
      where      r    {\displaystyle \mathbf {r} }  [\mathbf {r} ] is the
      position vector and is expressed as
                r  =  x  j     e   j     {\displaystyle \mathbf {r} =x_
            {j}\mathbf {e} _{j}}  [{\displaystyle \mathbf {r} =x_{j}\mathbf {e}
            _{j}}]
      Knowing that      T  k   ( n )   =  &#x03C3;  m k    n  m
      {\displaystyle T_{k}^{(n)}=\sigma _{mk}n_{m}}  [{\displaystyle T_{k}^{
      (n)}=\sigma _{mk}n_{m}}] and using Gauss's divergence theorem to change
      from a surface integral to a volume integral, we have
                   0    =  &#x222B;  S    &#x03B5;  i j k    x  j    &#x03C3;
            m k    n  m    d S +  &#x222B;  V    &#x03B5;  i j k    x  j    F
            k    d V       =  &#x222B;  V   (  &#x03B5;  i j k    x  j
            &#x03C3;  m k    )  , m   d V +  &#x222B;  V    &#x03B5;  i j k
            x  j    F  k    d V       =  &#x222B;  V   (  &#x03B5;  i j k    x
            j , m    &#x03C3;  m k   +  &#x03B5;  i j k    x  j    &#x03C3;  m
            k , m   ) d V +  &#x222B;  V    &#x03B5;  i j k    x  j    F  k
            d V       =  &#x222B;  V   (  &#x03B5;  i j k    x  j , m
            &#x03C3;  m k   ) d V +  &#x222B;  V    &#x03B5;  i j k    x  j
            (  &#x03C3;  m k , m   +  F  k   ) d V       {\displaystyle {\begin
            {aligned}0&=\int _{S}\varepsilon _{ijk}x_{j}\sigma _{mk}n_
            {m}\,dS+\int _{V}\varepsilon _{ijk}x_{j}F_{k}\,dV\\&=\int _{V}
            (\varepsilon _{ijk}x_{j}\sigma _{mk})_{,m}dV+\int _{V}\varepsilon _
            {ijk}x_{j}F_{k}\,dV\\&=\int _{V}(\varepsilon _{ijk}x_{j,m}\sigma _
            {mk}+\varepsilon _{ijk}x_{j}\sigma _{mk,m})dV+\int _{V}\varepsilon
            _{ijk}x_{j}F_{k}\,dV\\&=\int _{V}(\varepsilon _{ijk}x_{j,m}\sigma _
            {mk})dV+\int _{V}\varepsilon _{ijk}x_{j}(\sigma _{mk,m}+F_
            {k})dV\\\end{aligned}}}  [{\displaystyle {\begin{aligned}0&=\int _
            {S}\varepsilon _{ijk}x_{j}\sigma _{mk}n_{m}\,dS+\int _
            {V}\varepsilon _{ijk}x_{j}F_{k}\,dV\\&=\int _{V}(\varepsilon _
            {ijk}x_{j}\sigma _{mk})_{,m}dV+\int _{V}\varepsilon _{ijk}x_{j}F_
            {k}\,dV\\&=\int _{V}(\varepsilon _{ijk}x_{j,m}\sigma _
            {mk}+\varepsilon _{ijk}x_{j}\sigma _{mk,m})dV+\int _{V}\varepsilon
            _{ijk}x_{j}F_{k}\,dV\\&=\int _{V}(\varepsilon _{ijk}x_{j,m}\sigma _
            {mk})dV+\int _{V}\varepsilon _{ijk}x_{j}(\sigma _{mk,m}+F_
            {k})dV\\\end{aligned}}}]
      The second integral is zero as it contains the equilibrium equations.
      This leaves the first integral, where      x  j , m   =  &#x03B4;  j m
      {\displaystyle x_{j,m}=\delta _{jm}}  [{\displaystyle x_{j,m}=\delta _
      {jm}}], therefore
                &#x222B;  V   (  &#x03B5;  i j k    &#x03C3;  j k   ) d V = 0
            {\displaystyle \int _{V}(\varepsilon _{ijk}\sigma _{jk})dV=0}  [
            {\displaystyle \int _{V}(\varepsilon _{ijk}\sigma _{jk})dV=0}]
      For an arbitrary volume V, we then have
                &#x03B5;  i j k    &#x03C3;  j k   = 0   {\displaystyle
            \varepsilon _{ijk}\sigma _{jk}=0}  [{\displaystyle \varepsilon _
            {ijk}\sigma _{jk}=0}]
      which is satisfied at every point within the body. Expanding this
      equation we have
                &#x03C3;  12   =  &#x03C3;  21     {\displaystyle \sigma _
            {12}=\sigma _{21}}  [{\displaystyle \sigma _{12}=\sigma _{21}}],
            &#x03C3;  23   =  &#x03C3;  32     {\displaystyle \sigma _
            {23}=\sigma _{32}}  [{\displaystyle \sigma _{23}=\sigma _{32}}],
            and      &#x03C3;  13   =  &#x03C3;  31     {\displaystyle \sigma _
            {13}=\sigma _{31}}  [{\displaystyle \sigma _{13}=\sigma _{31}}]
      or in general
                &#x03C3;  i j   =  &#x03C3;  j i     {\displaystyle \sigma _
            {ij}=\sigma _{ji}}  [{\displaystyle \sigma _{ij}=\sigma _{ji}}]
      This proves that the stress tensor is symmetric
However, in the presence of couple-stresses, i.e. moments per unit volume, the
stress tensor is non-symmetric. This also is the case when the Knudsen_number
is close to one,      K  n   &#x2192; 1   {\displaystyle K_{n}\rightarrow 1}  [
{\displaystyle K_{n}\rightarrow 1}], or the continuum is a non-Newtonian fluid,
which can lead to rotationally non-invariant fluids, such as polymers.
***** Principal stresses and stress invariants[edit] *****
At every point in a stressed body there are at least three planes, called
principal planes, with normal vectors      n    {\displaystyle \mathbf {n} }
[\mathbf {n} ], called principal directions, where the corresponding stress
vector is perpendicular to the plane, i.e., parallel or in the same direction
as the normal vector      n    {\displaystyle \mathbf {n} }  [\mathbf {n} ],
and where there are no normal shear stresses      &#x03C4;   n
{\displaystyle \tau _{\mathrm {n} }}  [\tau _{{\mathrm  {n}}}]. The three
stresses normal to these principal planes are called principal stresses.
The components      &#x03C3;  i j     {\displaystyle \sigma _{ij}}  [\sigma _
{ij}] of the stress tensor depend on the orientation of the coordinate system
at the point under consideration. However, the stress tensor itself is a
physical quantity and as such, it is independent of the coordinate system
chosen to represent it. There are certain invariants associated with every
tensor which are also independent of the coordinate system. For example, a
vector is a simple tensor of rank one. In three dimensions, it has three
components. The value of these components will depend on the coordinate system
chosen to represent the vector, but the magnitude of the vector is a physical
quantity (a scalar) and is independent of the Cartesian_coordinate_system
chosen to represent the vector (so long as it is normal). Similarly, every
second rank tensor (such as the stress and the strain tensors) has three
independent invariant quantities associated with it. One set of such invariants
are the principal stresses of the stress tensor, which are just the eigenvalues
of the stress tensor. Their direction vectors are the principal directions or
eigenvectors.
A stress vector parallel to the normal unit vector      n    {\displaystyle
\mathbf {n} }  [\mathbf {n} ] is given by:
           T   (  n  )   = &#x03BB;  n  =   &#x03C3;    n     n
      {\displaystyle \mathbf {T} ^{(\mathbf {n} )}=\lambda \mathbf {n} =\mathbf
      {\sigma } _{\mathrm {n} }\mathbf {n} }  [{\displaystyle \mathbf {T} ^{
      (\mathbf {n} )}=\lambda \mathbf {n} =\mathbf {\sigma } _{\mathrm {n}
      }\mathbf {n} }]
where     &#x03BB;   {\displaystyle \lambda }  [\lambda ] is a constant of
proportionality, and in this particular case corresponds to the magnitudes
&#x03C3;   n      {\displaystyle \sigma _{\mathrm {n} }}  [\sigma _{{\mathrm
{n}}}] of the normal stress vectors or principal stresses.
Knowing that      T  i   ( n )   =  &#x03C3;  i j    n  j     {\displaystyle T_
{i}^{(n)}=\sigma _{ij}n_{j}}  [{\displaystyle T_{i}^{(n)}=\sigma _{ij}n_{j}}]
and      n  i   =  &#x03B4;  i j    n  j     {\displaystyle n_{i}=\delta _
{ij}n_{j}}  [{\displaystyle n_{i}=\delta _{ij}n_{j}}], we have
              T  i   ( n )      = &#x03BB;  n  i        &#x03C3;  i j    n  j
      = &#x03BB;  n  i        &#x03C3;  i j    n  j   &#x2212; &#x03BB;  n  i
      = 0      (   &#x03C3;  i j   &#x2212; &#x03BB;  &#x03B4;  i j    )   n  j
      = 0       {\displaystyle {\begin{aligned}T_{i}^{(n)}&=\lambda n_
      {i}\\\sigma _{ij}n_{j}&=\lambda n_{i}\\\sigma _{ij}n_{j}-\lambda n_
      {i}&=0\\\left(\sigma _{ij}-\lambda \delta _{ij}\right)n_{j}&=0\\\end
      {aligned}}}  [{\displaystyle {\begin{aligned}T_{i}^{(n)}&=\lambda n_
      {i}\\\sigma _{ij}n_{j}&=\lambda n_{i}\\\sigma _{ij}n_{j}-\lambda n_
      {i}&=0\\\left(\sigma _{ij}-\lambda \delta _{ij}\right)n_{j}&=0\\\end
      {aligned}}}]
This is a homogeneous_system, i.e. equal to zero, of three linear equations
where      n  j     {\displaystyle n_{j}}  [n_{j}] are the unknowns. To obtain
a nontrivial (non-zero) solution for      n  j     {\displaystyle n_{j}}  [n_
{j}], the determinant matrix of the coefficients must be equal to zero, i.e.
the system is singular. Thus,
          |   &#x03C3;  i j   &#x2212; &#x03BB;  &#x03B4;  i j    |  =   |
      &#x03C3;  11   &#x2212; &#x03BB;    &#x03C3;  12      &#x03C3;  13
      &#x03C3;  21      &#x03C3;  22   &#x2212; &#x03BB;    &#x03C3;  23
      &#x03C3;  31      &#x03C3;  32      &#x03C3;  33   &#x2212; &#x03BB;    |
      = 0   {\displaystyle \left|\sigma _{ij}-\lambda \delta _{ij}\right|=
      {\begin{vmatrix}\sigma _{11}-\lambda &\sigma _{12}&\sigma _{13}\\\sigma _
      {21}&\sigma _{22}-\lambda &\sigma _{23}\\\sigma _{31}&\sigma _{32}&\sigma
      _{33}-\lambda \\\end{vmatrix}}=0}  [{\displaystyle \left|\sigma _{ij}-
      \lambda \delta _{ij}\right|={\begin{vmatrix}\sigma _{11}-\lambda &\sigma
      _{12}&\sigma _{13}\\\sigma _{21}&\sigma _{22}-\lambda &\sigma _
      {23}\\\sigma _{31}&\sigma _{32}&\sigma _{33}-\lambda \\\end{vmatrix}}=0}]
Expanding the determinant leads to the characteristic equation
          |   &#x03C3;  i j   &#x2212; &#x03BB;  &#x03B4;  i j    |  = &#x2212;
      &#x03BB;  3   +  I  1    &#x03BB;  2   &#x2212;  I  2   &#x03BB; +  I  3
      = 0   {\displaystyle \left|\sigma _{ij}-\lambda \delta _{ij}\right|=-
      \lambda ^{3}+I_{1}\lambda ^{2}-I_{2}\lambda +I_{3}=0}  [{\displaystyle
      \left|\sigma _{ij}-\lambda \delta _{ij}\right|=-\lambda ^{3}+I_{1}\lambda
      ^{2}-I_{2}\lambda +I_{3}=0}]
where
              I  1      =  &#x03C3;  11   +  &#x03C3;  22   +  &#x03C3;  33
      =  &#x03C3;  k k   =  tr  (  &#x03C3;  )      I  2      =   |
      &#x03C3;  22      &#x03C3;  23        &#x03C3;  32      &#x03C3;  33
      |   +   |     &#x03C3;  11      &#x03C3;  13        &#x03C3;  31
      &#x03C3;  33      |   +   |     &#x03C3;  11      &#x03C3;  12
      &#x03C3;  21      &#x03C3;  22      |         =  &#x03C3;  11    &#x03C3;
      22   +  &#x03C3;  22    &#x03C3;  33   +  &#x03C3;  11    &#x03C3;  33
      &#x2212;  &#x03C3;  12   2   &#x2212;  &#x03C3;  23   2   &#x2212;
      &#x03C3;  31   2         =   1 2    (   &#x03C3;  i i    &#x03C3;  j j
      &#x2212;  &#x03C3;  i j    &#x03C3;  j i    )  =   1 2    [    (   tr
      (  &#x03C3;  )  )   2   &#x2212;  tr  (   &#x03C3;   2   )  ]       I  3
      = det (  &#x03C3;  i j   ) = det (  &#x03C3;  )       =  &#x03C3;  11
      &#x03C3;  22    &#x03C3;  33   + 2  &#x03C3;  12    &#x03C3;  23
      &#x03C3;  31   &#x2212;  &#x03C3;  12   2    &#x03C3;  33   &#x2212;
      &#x03C3;  23   2    &#x03C3;  11   &#x2212;  &#x03C3;  31   2    &#x03C3;
      22         {\displaystyle {\begin{aligned}I_{1}&=\sigma _{11}+\sigma _
      {22}+\sigma _{33}\\&=\sigma _{kk}={\text{tr}}({\boldsymbol {\sigma
      }})\\I_{2}&={\begin{vmatrix}\sigma _{22}&\sigma _{23}\\\sigma _
      {32}&\sigma _{33}\\\end{vmatrix}}+{\begin{vmatrix}\sigma _{11}&\sigma _
      {13}\\\sigma _{31}&\sigma _{33}\\\end{vmatrix}}+{\begin{vmatrix}\sigma _
      {11}&\sigma _{12}\\\sigma _{21}&\sigma _{22}\\\end{vmatrix}}\\&=\sigma _
      {11}\sigma _{22}+\sigma _{22}\sigma _{33}+\sigma _{11}\sigma _{33}-\sigma
      _{12}^{2}-\sigma _{23}^{2}-\sigma _{31}^{2}\\&={\frac {1}{2}}\left(\sigma
      _{ii}\sigma _{jj}-\sigma _{ij}\sigma _{ji}\right)={\frac {1}{2}}\left
      [\left({\text{tr}}({\boldsymbol {\sigma }})\right)^{2}-{\text{tr}}(
      {\boldsymbol {\sigma }}^{2})\right]\\I_{3}&=\det(\sigma _{ij})=\det(
      {\boldsymbol {\sigma }})\\&=\sigma _{11}\sigma _{22}\sigma _{33}+2\sigma
      _{12}\sigma _{23}\sigma _{31}-\sigma _{12}^{2}\sigma _{33}-\sigma _{23}^
      {2}\sigma _{11}-\sigma _{31}^{2}\sigma _{22}\\\end{aligned}}}  [
      {\displaystyle {\begin{aligned}I_{1}&=\sigma _{11}+\sigma _{22}+\sigma _
      {33}\\&=\sigma _{kk}={\text{tr}}({\boldsymbol {\sigma }})\\I_{2}&={\begin
      {vmatrix}\sigma _{22}&\sigma _{23}\\\sigma _{32}&\sigma _{33}\\\end
      {vmatrix}}+{\begin{vmatrix}\sigma _{11}&\sigma _{13}\\\sigma _{31}&\sigma
      _{33}\\\end{vmatrix}}+{\begin{vmatrix}\sigma _{11}&\sigma _{12}\\\sigma _
      {21}&\sigma _{22}\\\end{vmatrix}}\\&=\sigma _{11}\sigma _{22}+\sigma _
      {22}\sigma _{33}+\sigma _{11}\sigma _{33}-\sigma _{12}^{2}-\sigma _{23}^
      {2}-\sigma _{31}^{2}\\&={\frac {1}{2}}\left(\sigma _{ii}\sigma _{jj}-
      \sigma _{ij}\sigma _{ji}\right)={\frac {1}{2}}\left[\left({\text{tr}}(
      {\boldsymbol {\sigma }})\right)^{2}-{\text{tr}}({\boldsymbol {\sigma }}^
      {2})\right]\\I_{3}&=\det(\sigma _{ij})=\det({\boldsymbol {\sigma
      }})\\&=\sigma _{11}\sigma _{22}\sigma _{33}+2\sigma _{12}\sigma _
      {23}\sigma _{31}-\sigma _{12}^{2}\sigma _{33}-\sigma _{23}^{2}\sigma _
      {11}-\sigma _{31}^{2}\sigma _{22}\\\end{aligned}}}]
The characteristic equation has three real roots      &#x03BB;  i
{\displaystyle \lambda _{i}}  [\lambda _{i}], i.e. not imaginary due to the
symmetry of the stress tensor. The      &#x03C3;  1   = max  (   &#x03BB;  1
,  &#x03BB;  2   ,  &#x03BB;  3    )    {\displaystyle \sigma _{1}=\max \left
(\lambda _{1},\lambda _{2},\lambda _{3}\right)}  [{\displaystyle \sigma _
{1}=\max \left(\lambda _{1},\lambda _{2},\lambda _{3}\right)}],      &#x03C3;
3   = min  (   &#x03BB;  1   ,  &#x03BB;  2   ,  &#x03BB;  3    )
{\displaystyle \sigma _{3}=\min \left(\lambda _{1},\lambda _{2},\lambda _
{3}\right)}  [{\displaystyle \sigma _{3}=\min \left(\lambda _{1},\lambda _
{2},\lambda _{3}\right)}] and      &#x03C3;  2   =  I  1   &#x2212;  &#x03C3;
1   &#x2212;  &#x03C3;  3     {\displaystyle \sigma _{2}=I_{1}-\sigma _{1}-
\sigma _{3}}  [{\displaystyle \sigma _{2}=I_{1}-\sigma _{1}-\sigma _{3}}], are
the principal stresses, functions of the eigenvalues      &#x03BB;  i
{\displaystyle \lambda _{i}}  [\lambda _{i}]. The eigenvalues are the roots of
the characteristic_polynomial. The principal stresses are unique for a given
stress tensor. Therefore, from the characteristic equation, the coefficients
I  1     {\displaystyle I_{1}}  [I_{1}],      I  2     {\displaystyle I_{2}}
[I_{2}] and      I  3     {\displaystyle I_{3}}  [I_{3}], called the first,
second, and third stress invariants, respectively, always have the same value
regardless of the coordinate system's orientation.
For each eigenvalue, there is a non-trivial solution for      n  j
{\displaystyle n_{j}}  [n_{j}] in the equation      (   &#x03C3;  i j
&#x2212; &#x03BB;  &#x03B4;  i j    )   n  j   = 0   {\displaystyle \left
(\sigma _{ij}-\lambda \delta _{ij}\right)n_{j}=0}  [{\displaystyle \left(\sigma
_{ij}-\lambda \delta _{ij}\right)n_{j}=0}]. These solutions are the principal
directions or eigenvectors defining the plane where the principal stresses act.
The principal stresses and principal directions characterize the stress at a
point and are independent of the orientation.
A coordinate system with axes oriented to the principal directions implies that
the normal stresses are the principal stresses and the stress tensor is
represented by a diagonal matrix:
          &#x03C3;  i j   =   [     &#x03C3;  1     0   0     0    &#x03C3;  2
      0     0   0    &#x03C3;  3      ]     {\displaystyle \sigma _{ij}={\begin
      {bmatrix}\sigma _{1}&0&0\\0&\sigma _{2}&0\\0&0&\sigma _{3}\end{bmatrix}}}
      [{\displaystyle \sigma _{ij}={\begin{bmatrix}\sigma _{1}&0&0\\0&\sigma _
      {2}&0\\0&0&\sigma _{3}\end{bmatrix}}}]
The principal stresses can be combined to form the stress invariants,      I  1
{\displaystyle I_{1}}  [I_{1}],      I  2     {\displaystyle I_{2}}  [I_{2}],
and      I  3     {\displaystyle I_{3}}  [I_{3}]. The first and third invariant
are the trace and determinant respectively, of the stress tensor. Thus,
              I  1      =  &#x03C3;  1   +  &#x03C3;  2   +  &#x03C3;  3
      I  2      =  &#x03C3;  1    &#x03C3;  2   +  &#x03C3;  2    &#x03C3;  3
      +  &#x03C3;  3    &#x03C3;  1        I  3      =  &#x03C3;  1    &#x03C3;
      2    &#x03C3;  3         {\displaystyle {\begin{aligned}I_{1}&=\sigma _
      {1}+\sigma _{2}+\sigma _{3}\\I_{2}&=\sigma _{1}\sigma _{2}+\sigma _
      {2}\sigma _{3}+\sigma _{3}\sigma _{1}\\I_{3}&=\sigma _{1}\sigma _
      {2}\sigma _{3}\\\end{aligned}}}  [{\displaystyle {\begin{aligned}I_
      {1}&=\sigma _{1}+\sigma _{2}+\sigma _{3}\\I_{2}&=\sigma _{1}\sigma _
      {2}+\sigma _{2}\sigma _{3}+\sigma _{3}\sigma _{1}\\I_{3}&=\sigma _
      {1}\sigma _{2}\sigma _{3}\\\end{aligned}}}]
Because of its simplicity, the principal coordinate system is often useful when
considering the state of the elastic medium at a particular point. Principal
stresses are often expressed in the following equation for evaluating stresses
in the x and y directions or axial and bending stresses on a part.[14]:
p.58â59 The principal normal stresses can then be used to calculate the von
Mises_stress and ultimately the safety factor and margin of safety.
          &#x03C3;  1   ,  &#x03C3;  2   =     &#x03C3;  x   +  &#x03C3;  y
      2   &#x00B1;     (     &#x03C3;  x   &#x2212;  &#x03C3;  y    2   )   2
      +  &#x03C4;  x y   2       {\displaystyle \sigma _{1},\sigma _{2}={\frac
      {\sigma _{x}+\sigma _{y}}{2}}\pm {\sqrt {\left({\frac {\sigma _{x}-\sigma
      _{y}}{2}}\right)^{2}+\tau _{xy}^{2}}}}  [{\displaystyle \sigma _
      {1},\sigma _{2}={\frac {\sigma _{x}+\sigma _{y}}{2}}\pm {\sqrt {\left(
      {\frac {\sigma _{x}-\sigma _{y}}{2}}\right)^{2}+\tau _{xy}^{2}}}}]
Using just the part of the equation under the square_root is equal to the
maximum and minimum shear stress for plus and minus. This is shown as:
          &#x03C4;  m a x   ,  &#x03C4;  m i n   = &#x00B1;     (     &#x03C3;
      x   &#x2212;  &#x03C3;  y    2   )   2   +  &#x03C4;  x y   2
      {\displaystyle \tau _{max},\tau _{min}=\pm {\sqrt {\left({\frac {\sigma _
      {x}-\sigma _{y}}{2}}\right)^{2}+\tau _{xy}^{2}}}}  [{\displaystyle \tau _
      {max},\tau _{min}=\pm {\sqrt {\left({\frac {\sigma _{x}-\sigma _{y}}
      {2}}\right)^{2}+\tau _{xy}^{2}}}}]
***** Maximum and minimum shear stresses[edit] *****
The maximum shear stress or maximum principal shear stress is equal to one-half
the difference between the largest and smallest principal stresses, and acts on
the plane that bisects the angle between the directions of the largest and
smallest principal stresses, i.e. the plane of the maximum shear stress is
oriented      45  &#x2218;     {\displaystyle 45^{\circ }}  [45^\circ] from the
principal stress planes. The maximum shear stress is expressed as
          &#x03C4;  max   =   1 2    |   &#x03C3;  max   &#x2212;  &#x03C3;
      min    |    {\displaystyle \tau _{\max }={\frac {1}{2}}\left|\sigma _
      {\max }-\sigma _{\min }\right|}  [{\displaystyle \tau _{\max }={\frac {1}
      {2}}\left|\sigma _{\max }-\sigma _{\min }\right|}]
Assuming      &#x03C3;  1   &#x2265;  &#x03C3;  2   &#x2265;  &#x03C3;  3
{\displaystyle \sigma _{1}\geq \sigma _{2}\geq \sigma _{3}}  [{\displaystyle
\sigma _{1}\geq \sigma _{2}\geq \sigma _{3}}] then
          &#x03C4;  max   =   1 2    |   &#x03C3;  1   &#x2212;  &#x03C3;  3
      |    {\displaystyle \tau _{\max }={\frac {1}{2}}\left|\sigma _{1}-\sigma
      _{3}\right|}  [{\displaystyle \tau _{\max }={\frac {1}{2}}\left|\sigma _
      {1}-\sigma _{3}\right|}]
When the stress tensor is non zero the normal stress component acting on the
plane for the maximum shear stress is non-zero and it is equal to
    &#x03C3;   n    =   1 2    (   &#x03C3;  1   +  &#x03C3;  3    )
{\displaystyle \sigma _{\mathrm {n} }={\frac {1}{2}}\left(\sigma _{1}+\sigma _
{3}\right)}  [{\displaystyle \sigma _{\mathrm {n} }={\frac {1}{2}}\left(\sigma
_{1}+\sigma _{3}\right)}]
      Derivation of the maximum and minimum shear stresses[8]:p.45â78[11]:p.1â46
      [13][15]:p.111â157[16]:p.9â41[17]:p.33â66[18]:p.43â61
      The normal stress can be written in terms of principal stresses     (  &#x03C3;
      1   &#x2265;  &#x03C3;  2   &#x2265;  &#x03C3;  3   )   {\displaystyle (\sigma _
      {1}\geq \sigma _{2}\geq \sigma _{3})}  [{\displaystyle (\sigma _{1}\geq \sigma _
      {2}\geq \sigma _{3})}] as
                    &#x03C3;   n       =  &#x03C3;  i j    n  i    n  j         =
            &#x03C3;  1    n  1   2   +  &#x03C3;  2    n  2   2   +  &#x03C3;  3    n
            3   2         {\displaystyle {\begin{aligned}\sigma _{\mathrm {n} }&=\sigma
            _{ij}n_{i}n_{j}\\&=\sigma _{1}n_{1}^{2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_
            {3}^{2}\\\end{aligned}}}  [{\displaystyle {\begin{aligned}\sigma _{\mathrm
            {n} }&=\sigma _{ij}n_{i}n_{j}\\&=\sigma _{1}n_{1}^{2}+\sigma _{2}n_{2}^
            {2}+\sigma _{3}n_{3}^{2}\\\end{aligned}}}]
      Knowing that       (  T  ( n )   )   2   =  &#x03C3;  i j    &#x03C3;  i k    n
      j    n  k     {\displaystyle \left(T^{(n)}\right)^{2}=\sigma _{ij}\sigma _{ik}n_
      {j}n_{k}}  [\left( T^{(n)} \right)^2=\sigma_{ij}\sigma_{ik}n_jn_k], the shear
      stress in terms of principal stresses components is expressed as
                    &#x03C4;   n    2      =   (  T  ( n )   )   2   &#x2212;  &#x03C3;
            n    2         =  &#x03C3;  1   2    n  1   2   +  &#x03C3;  2   2    n  2
            2   +  &#x03C3;  3   2    n  3   2   &#x2212;   (   &#x03C3;  1    n  1   2
            +  &#x03C3;  2    n  2   2   +  &#x03C3;  3    n  3   2    )   2         =
            (  &#x03C3;  1   2   &#x2212;  &#x03C3;  2   2   )  n  1   2   +
            (  &#x03C3;  2   2   &#x2212;  &#x03C3;  3   2   )  n  2   2   +  &#x03C3;
            3   2   &#x2212;   [   (   &#x03C3;  1   &#x2212;  &#x03C3;  3    )   n  1
            2   +  (   &#x03C3;  2   &#x2212;  &#x03C3;  2    )   n  2   2   +
            &#x03C3;  3    ]   2         = (  &#x03C3;  1   &#x2212;  &#x03C3;  2    )
            2    n  1   2    n  2   2   + (  &#x03C3;  2   &#x2212;  &#x03C3;  3    )
            2    n  2   2    n  3   2   + (  &#x03C3;  1   &#x2212;  &#x03C3;  3    )
            2    n  1   2    n  3   2         {\displaystyle {\begin{aligned}\tau _
            {\mathrm {n} }^{2}&=\left(T^{(n)}\right)^{2}-\sigma _{\mathrm {n} }^
            {2}\\&=\sigma _{1}^{2}n_{1}^{2}+\sigma _{2}^{2}n_{2}^{2}+\sigma _{3}^{2}n_
            {3}^{2}-\left(\sigma _{1}n_{1}^{2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^
            {2}\right)^{2}\\&=(\sigma _{1}^{2}-\sigma _{2}^{2})n_{1}^{2}+(\sigma _{2}^
            {2}-\sigma _{3}^{2})n_{2}^{2}+\sigma _{3}^{2}-\left[\left(\sigma _{1}-
            \sigma _{3}\right)n_{1}^{2}+\left(\sigma _{2}-\sigma _{2}\right)n_{2}^
            {2}+\sigma _{3}\right]^{2}\\&=(\sigma _{1}-\sigma _{2})^{2}n_{1}^{2}n_{2}^
            {2}+(\sigma _{2}-\sigma _{3})^{2}n_{2}^{2}n_{3}^{2}+(\sigma _{1}-\sigma _
            {3})^{2}n_{1}^{2}n_{3}^{2}\\\end{aligned}}}  [{\displaystyle {\begin
            {aligned}\tau _{\mathrm {n} }^{2}&=\left(T^{(n)}\right)^{2}-\sigma _
            {\mathrm {n} }^{2}\\&=\sigma _{1}^{2}n_{1}^{2}+\sigma _{2}^{2}n_{2}^
            {2}+\sigma _{3}^{2}n_{3}^{2}-\left(\sigma _{1}n_{1}^{2}+\sigma _{2}n_{2}^
            {2}+\sigma _{3}n_{3}^{2}\right)^{2}\\&=(\sigma _{1}^{2}-\sigma _{2}^{2})n_
            {1}^{2}+(\sigma _{2}^{2}-\sigma _{3}^{2})n_{2}^{2}+\sigma _{3}^{2}-\left
            [\left(\sigma _{1}-\sigma _{3}\right)n_{1}^{2}+\left(\sigma _{2}-\sigma _
            {2}\right)n_{2}^{2}+\sigma _{3}\right]^{2}\\&=(\sigma _{1}-\sigma _{2})^
            {2}n_{1}^{2}n_{2}^{2}+(\sigma _{2}-\sigma _{3})^{2}n_{2}^{2}n_{3}^{2}+
            (\sigma _{1}-\sigma _{3})^{2}n_{1}^{2}n_{3}^{2}\\\end{aligned}}}]
      The maximum shear stress at a point in a continuum body is determined by
      maximizing      &#x03C4;   n    2     {\displaystyle \tau _{\mathrm {n} }^{2}}  [
      {\displaystyle \tau _{\mathrm {n} }^{2}}] subject to the condition that
                n  i    n  i   =  n  1   2   +  n  2   2   +  n  3   2   = 1
            {\displaystyle n_{i}n_{i}=n_{1}^{2}+n_{2}^{2}+n_{3}^{2}=1}  [{\displaystyle
            n_{i}n_{i}=n_{1}^{2}+n_{2}^{2}+n_{3}^{2}=1}]
      This is a constrained maximization problem, which can be solved using the
      Lagrangian_multiplier technique to convert the problem into an unconstrained
      optimization problem. Thus, the stationary values (maximum and minimum values)of
      &#x03C4;   n    2     {\displaystyle \tau _{\mathrm {n} }^{2}}  [{\displaystyle
      \tau _{\mathrm {n} }^{2}}] occur where the gradient of      &#x03C4;   n    2
      {\displaystyle \tau _{\mathrm {n} }^{2}}  [{\displaystyle \tau _{\mathrm {n} }^
      {2}}] is parallel to the gradient of     F   {\displaystyle F}  [F].
      The Lagrangian function for this problem can be written as
                   F  (   n  1   ,  n  2   ,  n  3   , &#x03BB;  )     =  &#x03C4;  2
            + &#x03BB;  (  g  (   n  1   ,  n  2   ,  n  3    )  &#x2212; 1  )        =
            &#x03C3;  1   2    n  1   2   +  &#x03C3;  2   2    n  2   2   +  &#x03C3;
            3   2    n  3   2   &#x2212;   (   &#x03C3;  1    n  1   2   +  &#x03C3;  2
            n  2   2   +  &#x03C3;  3    n  3   2    )   2   + &#x03BB;  (   n  1   2
            +  n  2   2   +  n  3   2   &#x2212; 1  )        {\displaystyle {\begin
            {aligned}F\left(n_{1},n_{2},n_{3},\lambda \right)&=\tau ^{2}+\lambda \left
            (g\left(n_{1},n_{2},n_{3}\right)-1\right)\\&=\sigma _{1}^{2}n_{1}^
            {2}+\sigma _{2}^{2}n_{2}^{2}+\sigma _{3}^{2}n_{3}^{2}-\left(\sigma _{1}n_
            {1}^{2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^{2}\right)^{2}+\lambda \left
            (n_{1}^{2}+n_{2}^{2}+n_{3}^{2}-1\right)\\\end{aligned}}}  [{\displaystyle
            {\begin{aligned}F\left(n_{1},n_{2},n_{3},\lambda \right)&=\tau ^{2}+\lambda
            \left(g\left(n_{1},n_{2},n_{3}\right)-1\right)\\&=\sigma _{1}^{2}n_{1}^
            {2}+\sigma _{2}^{2}n_{2}^{2}+\sigma _{3}^{2}n_{3}^{2}-\left(\sigma _{1}n_
            {1}^{2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^{2}\right)^{2}+\lambda \left
            (n_{1}^{2}+n_{2}^{2}+n_{3}^{2}-1\right)\\\end{aligned}}}]
      where     &#x03BB;   {\displaystyle \lambda }  [\lambda ] is the Lagrangian
      multiplier (which is different from the     &#x03BB;   {\displaystyle \lambda }
      [\lambda ] use to denote eigenvalues).
      The extreme values of these functions are
                  &#x2202; F   &#x2202;  n  1      = 0     &#x2202; F   &#x2202;  n  2
            = 0     &#x2202; F   &#x2202;  n  3      = 0   {\displaystyle {\frac
            {\partial F}{\partial n_{1}}}=0\qquad {\frac {\partial F}{\partial n_
            {2}}}=0\qquad {\frac {\partial F}{\partial n_{3}}}=0}  [{\displaystyle
            {\frac {\partial F}{\partial n_{1}}}=0\qquad {\frac {\partial F}{\partial
            n_{2}}}=0\qquad {\frac {\partial F}{\partial n_{3}}}=0}]
      thence
                  &#x2202; F   &#x2202;  n  1      =  n  1    &#x03C3;  1   2
            &#x2212; 2  n  1    &#x03C3;  1    (   &#x03C3;  1    n  1   2   +
            &#x03C3;  2    n  2   2   +  &#x03C3;  3    n  3   2    )  + &#x03BB;  n  1
            = 0   {\displaystyle {\frac {\partial F}{\partial n_{1}}}=n_{1}\sigma _{1}^
            {2}-2n_{1}\sigma _{1}\left(\sigma _{1}n_{1}^{2}+\sigma _{2}n_{2}^{2}+\sigma
            _{3}n_{3}^{2}\right)+\lambda n_{1}=0}  [{\displaystyle {\frac {\partial F}
            {\partial n_{1}}}=n_{1}\sigma _{1}^{2}-2n_{1}\sigma _{1}\left(\sigma _{1}n_
            {1}^{2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^{2}\right)+\lambda n_{1}=0}]
                  &#x2202; F   &#x2202;  n  2      =  n  2    &#x03C3;  2   2
            &#x2212; 2  n  2    &#x03C3;  2    (   &#x03C3;  1    n  1   2   +
            &#x03C3;  2    n  2   2   +  &#x03C3;  3    n  3   2    )  + &#x03BB;  n  2
            = 0   {\displaystyle {\frac {\partial F}{\partial n_{2}}}=n_{2}\sigma _{2}^
            {2}-2n_{2}\sigma _{2}\left(\sigma _{1}n_{1}^{2}+\sigma _{2}n_{2}^{2}+\sigma
            _{3}n_{3}^{2}\right)+\lambda n_{2}=0}  [{\displaystyle {\frac {\partial F}
            {\partial n_{2}}}=n_{2}\sigma _{2}^{2}-2n_{2}\sigma _{2}\left(\sigma _{1}n_
            {1}^{2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^{2}\right)+\lambda n_{2}=0}]
                  &#x2202; F   &#x2202;  n  3      =  n  3    &#x03C3;  3   2
            &#x2212; 2  n  3    &#x03C3;  3    (   &#x03C3;  1    n  1   2   +
            &#x03C3;  2    n  2   2   +  &#x03C3;  3    n  3   2    )  + &#x03BB;  n  3
            = 0   {\displaystyle {\frac {\partial F}{\partial n_{3}}}=n_{3}\sigma _{3}^
            {2}-2n_{3}\sigma _{3}\left(\sigma _{1}n_{1}^{2}+\sigma _{2}n_{2}^{2}+\sigma
            _{3}n_{3}^{2}\right)+\lambda n_{3}=0}  [{\displaystyle {\frac {\partial F}
            {\partial n_{3}}}=n_{3}\sigma _{3}^{2}-2n_{3}\sigma _{3}\left(\sigma _{1}n_
            {1}^{2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^{2}\right)+\lambda n_{3}=0}]
      These three equations together with the condition      n  i    n  i   = 1
      {\displaystyle n_{i}n_{i}=1}  [{\displaystyle n_{i}n_{i}=1}] may be solved for
      &#x03BB; ,  n  1   ,  n  2   ,   {\displaystyle \lambda ,n_{1},n_{2},}  [
      {\displaystyle \lambda ,n_{1},n_{2},}] and      n  3     {\displaystyle n_{3}}
      [n_{3}]
      By multiplying the first three equations by      n  1   ,   n  2   ,
      {\displaystyle n_{1},\,n_{2},}  [{\displaystyle n_{1},\,n_{2},}] and      n  3
      {\displaystyle n_{3}}  [n_{3}], respectively, and knowing that      &#x03C3;   n
      =  &#x03C3;  i j    n  i    n  j   =  &#x03C3;  1    n  1   2   +  &#x03C3;  2
      n  2   2   +  &#x03C3;  3    n  3   2     {\displaystyle \sigma _{\mathrm {n}
      }=\sigma _{ij}n_{i}n_{j}=\sigma _{1}n_{1}^{2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_
      {3}^{2}}  [{\displaystyle \sigma _{\mathrm {n} }=\sigma _{ij}n_{i}n_{j}=\sigma _
      {1}n_{1}^{2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^{2}}] we obtain
                n  1   2    &#x03C3;  1   2   &#x2212; 2  &#x03C3;  1    n  1   2
            &#x03C3;   n    +  n  1   2   &#x03BB; = 0   {\displaystyle n_{1}^{2}\sigma
            _{1}^{2}-2\sigma _{1}n_{1}^{2}\sigma _{\mathrm {n} }+n_{1}^{2}\lambda =0}
            [{\displaystyle n_{1}^{2}\sigma _{1}^{2}-2\sigma _{1}n_{1}^{2}\sigma _
            {\mathrm {n} }+n_{1}^{2}\lambda =0}]
                n  2   2    &#x03C3;  2   2   &#x2212; 2  &#x03C3;  2    n  2   2
            &#x03C3;   n    +  n  2   2   &#x03BB; = 0   {\displaystyle n_{2}^{2}\sigma
            _{2}^{2}-2\sigma _{2}n_{2}^{2}\sigma _{\mathrm {n} }+n_{2}^{2}\lambda =0}
            [{\displaystyle n_{2}^{2}\sigma _{2}^{2}-2\sigma _{2}n_{2}^{2}\sigma _
            {\mathrm {n} }+n_{2}^{2}\lambda =0}]
                n  3   2    &#x03C3;  3   2   &#x2212; 2  &#x03C3;  1    n  3   2
            &#x03C3;   n    +  n  3   2   &#x03BB; = 0   {\displaystyle n_{3}^{2}\sigma
            _{3}^{2}-2\sigma _{1}n_{3}^{2}\sigma _{\mathrm {n} }+n_{3}^{2}\lambda =0}
            [{\displaystyle n_{3}^{2}\sigma _{3}^{2}-2\sigma _{1}n_{3}^{2}\sigma _
            {\mathrm {n} }+n_{3}^{2}\lambda =0}]
      Adding these three equations we get
                    [   n  1   2    &#x03C3;  1   2   +  n  2   2    &#x03C3;  2   2
            +  n  3   2    &#x03C3;  3   2    ]  &#x2212; 2  (   &#x03C3;  1    n  1
            2   +  &#x03C3;  2    n  2   2   +  &#x03C3;  3    n  3   2    )   &#x03C3;
            n    + &#x03BB;  (   n  1   2   +  n  2   2   +  n  3   2    )     = 0
            [   &#x03C4;   n    2   +   (   &#x03C3;  1    n  1   2   +  &#x03C3;  2
            n  2   2   +  &#x03C3;  3    n  3   2    )   2    ]  &#x2212; 2  &#x03C3;
            n    2   + &#x03BB;    = 0      [   &#x03C4;   n    2   +  &#x03C3;   n
            2    ]  &#x2212; 2  &#x03C3;   n    2   + &#x03BB;    = 0     &#x03BB;    =
            &#x03C3;   n    2   &#x2212;  &#x03C4;   n    2         {\displaystyle
            {\begin{aligned}\left[n_{1}^{2}\sigma _{1}^{2}+n_{2}^{2}\sigma _{2}^{2}+n_
            {3}^{2}\sigma _{3}^{2}\right]-2\left(\sigma _{1}n_{1}^{2}+\sigma _{2}n_{2}^
            {2}+\sigma _{3}n_{3}^{2}\right)\sigma _{\mathrm {n} }+\lambda \left(n_{1}^
            {2}+n_{2}^{2}+n_{3}^{2}\right)&=0\\\left[\tau _{\mathrm {n} }^{2}+\left
            (\sigma _{1}n_{1}^{2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^{2}\right)^
            {2}\right]-2\sigma _{\mathrm {n} }^{2}+\lambda &=0\\\left[\tau _{\mathrm
            {n} }^{2}+\sigma _{\mathrm {n} }^{2}\right]-2\sigma _{\mathrm {n} }^
            {2}+\lambda &=0\\\lambda &=\sigma _{\mathrm {n} }^{2}-\tau _{\mathrm {n} }^
            {2}\end{aligned}}}  [{\displaystyle {\begin{aligned}\left[n_{1}^{2}\sigma _
            {1}^{2}+n_{2}^{2}\sigma _{2}^{2}+n_{3}^{2}\sigma _{3}^{2}\right]-2\left
            (\sigma _{1}n_{1}^{2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^
            {2}\right)\sigma _{\mathrm {n} }+\lambda \left(n_{1}^{2}+n_{2}^{2}+n_{3}^
            {2}\right)&=0\\\left[\tau _{\mathrm {n} }^{2}+\left(\sigma _{1}n_{1}^
            {2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^{2}\right)^{2}\right]-2\sigma _
            {\mathrm {n} }^{2}+\lambda &=0\\\left[\tau _{\mathrm {n} }^{2}+\sigma _
            {\mathrm {n} }^{2}\right]-2\sigma _{\mathrm {n} }^{2}+\lambda &=0\\\lambda
            &=\sigma _{\mathrm {n} }^{2}-\tau _{\mathrm {n} }^{2}\end{aligned}}}]
      this result can be substituted into each of the first three equations to obtain
                      &#x2202; F   &#x2202;  n  1      =  n  1    &#x03C3;  1   2
            &#x2212; 2  n  1    &#x03C3;  1    (   &#x03C3;  1    n  1   2   +
            &#x03C3;  2    n  2   2   +  &#x03C3;  3    n  3   2    )  +  (   &#x03C3;
            n    2   &#x2212;  &#x03C4;   n    2    )   n  1      = 0      n  1
            &#x03C3;  1   2   &#x2212; 2  n  1    &#x03C3;  1    &#x03C3;   n    +
            (   &#x03C3;   n    2   &#x2212;  &#x03C4;   n    2    )   n  1      = 0
            (   &#x03C3;  1   2   &#x2212; 2  &#x03C3;  1    &#x03C3;   n    +
            &#x03C3;   n    2   &#x2212;  &#x03C4;   n    2    )   n  1      = 0
            {\displaystyle {\begin{aligned}{\frac {\partial F}{\partial n_{1}}}=n_
            {1}\sigma _{1}^{2}-2n_{1}\sigma _{1}\left(\sigma _{1}n_{1}^{2}+\sigma _
            {2}n_{2}^{2}+\sigma _{3}n_{3}^{2}\right)+\left(\sigma _{\mathrm {n} }^{2}-
            \tau _{\mathrm {n} }^{2}\right)n_{1}&=0\\n_{1}\sigma _{1}^{2}-2n_{1}\sigma
            _{1}\sigma _{\mathrm {n} }+\left(\sigma _{\mathrm {n} }^{2}-\tau _{\mathrm
            {n} }^{2}\right)n_{1}&=0\\\left(\sigma _{1}^{2}-2\sigma _{1}\sigma _
            {\mathrm {n} }+\sigma _{\mathrm {n} }^{2}-\tau _{\mathrm {n} }^{2}\right)n_
            {1}&=0\\\end{aligned}}}  [{\displaystyle {\begin{aligned}{\frac {\partial
            F}{\partial n_{1}}}=n_{1}\sigma _{1}^{2}-2n_{1}\sigma _{1}\left(\sigma _
            {1}n_{1}^{2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^{2}\right)+\left(\sigma
            _{\mathrm {n} }^{2}-\tau _{\mathrm {n} }^{2}\right)n_{1}&=0\\n_{1}\sigma _
            {1}^{2}-2n_{1}\sigma _{1}\sigma _{\mathrm {n} }+\left(\sigma _{\mathrm {n}
            }^{2}-\tau _{\mathrm {n} }^{2}\right)n_{1}&=0\\\left(\sigma _{1}^{2}-
            2\sigma _{1}\sigma _{\mathrm {n} }+\sigma _{\mathrm {n} }^{2}-\tau _
            {\mathrm {n} }^{2}\right)n_{1}&=0\\\end{aligned}}}]
      Doing the same for the other two equations we have
                  &#x2202; F   &#x2202;  n  2      =  (   &#x03C3;  2   2   &#x2212; 2
            &#x03C3;  2    &#x03C3;   n    +  &#x03C3;   n    2   &#x2212;  &#x03C4;
            n    2    )   n  2   = 0   {\displaystyle {\frac {\partial F}{\partial n_
            {2}}}=\left(\sigma _{2}^{2}-2\sigma _{2}\sigma _{\mathrm {n} }+\sigma _
            {\mathrm {n} }^{2}-\tau _{\mathrm {n} }^{2}\right)n_{2}=0}  [{\displaystyle
            {\frac {\partial F}{\partial n_{2}}}=\left(\sigma _{2}^{2}-2\sigma _
            {2}\sigma _{\mathrm {n} }+\sigma _{\mathrm {n} }^{2}-\tau _{\mathrm {n} }^
            {2}\right)n_{2}=0}]
                  &#x2202; F   &#x2202;  n  3      =  (   &#x03C3;  3   2   &#x2212; 2
            &#x03C3;  3    &#x03C3;   n    +  &#x03C3;   n    2   &#x2212;  &#x03C4;
            n    2    )   n  3   = 0   {\displaystyle {\frac {\partial F}{\partial n_
            {3}}}=\left(\sigma _{3}^{2}-2\sigma _{3}\sigma _{\mathrm {n} }+\sigma _
            {\mathrm {n} }^{2}-\tau _{\mathrm {n} }^{2}\right)n_{3}=0}  [{\displaystyle
            {\frac {\partial F}{\partial n_{3}}}=\left(\sigma _{3}^{2}-2\sigma _
            {3}\sigma _{\mathrm {n} }+\sigma _{\mathrm {n} }^{2}-\tau _{\mathrm {n} }^
            {2}\right)n_{3}=0}]
      A first approach to solve these last three equations is to consider the trivial
      solution      n  i   = 0   {\displaystyle n_{i}=0}  [{\displaystyle n_{i}=0}].
      However, this option does not fulfill the constraint      n  i    n  i   = 1
      {\displaystyle n_{i}n_{i}=1}  [{\displaystyle n_{i}n_{i}=1}].
      Considering the solution where      n  1   =  n  2   = 0   {\displaystyle n_
      {1}=n_{2}=0}  [{\displaystyle n_{1}=n_{2}=0}] and      n  3   &#x2260; 0
      {\displaystyle n_{3}\neq 0}  [{\displaystyle n_{3}\neq 0}], it is determine from
      the condition      n  i    n  i   = 1   {\displaystyle n_{i}n_{i}=1}  [
      {\displaystyle n_{i}n_{i}=1}] that      n  3   = &#x00B1; 1   {\displaystyle n_
      {3}=\pm 1}  [{\displaystyle n_{3}=\pm 1}], then from the original equation for
      &#x03C4;   n    2     {\displaystyle \tau _{\mathrm {n} }^{2}}  [{\displaystyle
      \tau _{\mathrm {n} }^{2}}] it is seen that      &#x03C4;   n    = 0
      {\displaystyle \tau _{\mathrm {n} }=0}  [{\displaystyle \tau _{\mathrm {n} }=0}].
      The other two possible values for      &#x03C4;   n      {\displaystyle \tau _
      {\mathrm {n} }}  [\tau _{{\mathrm  {n}}}] can be obtained similarly by assuming
                n  1   =  n  3   = 0   {\displaystyle n_{1}=n_{3}=0}  [{\displaystyle
            n_{1}=n_{3}=0}] and      n  2   &#x2260; 0   {\displaystyle n_{2}\neq 0}  [
            {\displaystyle n_{2}\neq 0}]
                n  2   =  n  3   = 0   {\displaystyle n_{2}=n_{3}=0}  [{\displaystyle
            n_{2}=n_{3}=0}] and      n  1   &#x2260; 0   {\displaystyle n_{1}\neq 0}  [
            {\displaystyle n_{1}\neq 0}]
      Thus, one set of solutions for these four equations is:
                    n  1      = 0 ,    n  2     = 0 ,    n  3      = &#x00B1; 1 ,
            &#x03C4;   n      = 0      n  1      = 0 ,    n  2     = &#x00B1; 1 ,    n
            3      = 0 ,    &#x03C4;   n      = 0      n  1      = &#x00B1; 1 ,    n  2
            = 0 ,    n  3      = 0 ,    &#x03C4;   n      = 0       {\displaystyle
            {\begin{aligned}n_{1}&=0,\,\,n_{2}&=0,\,\,n_{3}&=\pm 1,\,\,\tau _{\mathrm
            {n} }&=0\\n_{1}&=0,\,\,n_{2}&=\pm 1,\,\,n_{3}&=0,\,\,\tau _{\mathrm {n}
            }&=0\\n_{1}&=\pm 1,\,\,n_{2}&=0,\,\,n_{3}&=0,\,\,\tau _{\mathrm {n}
            }&=0\end{aligned}}}  [{\displaystyle {\begin{aligned}n_{1}&=0,\,\,n_
            {2}&=0,\,\,n_{3}&=\pm 1,\,\,\tau _{\mathrm {n} }&=0\\n_{1}&=0,\,\,n_
            {2}&=\pm 1,\,\,n_{3}&=0,\,\,\tau _{\mathrm {n} }&=0\\n_{1}&=\pm 1,\,\,n_
            {2}&=0,\,\,n_{3}&=0,\,\,\tau _{\mathrm {n} }&=0\end{aligned}}}]
      These correspond to minimum values for      &#x03C4;   n      {\displaystyle \tau
      _{\mathrm {n} }}  [\tau _{{\mathrm  {n}}}] and verifies that there are no shear
      stresses on planes normal to the principal directions of stress, as shown
      previously.
      A second set of solutions is obtained by assuming      n  1   = 0 ,   n  2
      &#x2260; 0   {\displaystyle n_{1}=0,\,n_{2}\neq 0}  [{\displaystyle n_{1}=0,\,n_
      {2}\neq 0}] and      n  3   &#x2260; 0   {\displaystyle n_{3}\neq 0}  [
      {\displaystyle n_{3}\neq 0}]. Thus we have
                  &#x2202; F   &#x2202;  n  2      =  &#x03C3;  2   2   &#x2212; 2
            &#x03C3;  2    &#x03C3;   n    +  &#x03C3;   n    2   &#x2212;  &#x03C4;
            n    2   = 0   {\displaystyle {\frac {\partial F}{\partial n_{2}}}=\sigma _
            {2}^{2}-2\sigma _{2}\sigma _{\mathrm {n} }+\sigma _{\mathrm {n} }^{2}-\tau
            _{\mathrm {n} }^{2}=0}  [{\displaystyle {\frac {\partial F}{\partial n_
            {2}}}=\sigma _{2}^{2}-2\sigma _{2}\sigma _{\mathrm {n} }+\sigma _{\mathrm
            {n} }^{2}-\tau _{\mathrm {n} }^{2}=0}]
                  &#x2202; F   &#x2202;  n  3      =  &#x03C3;  3   2   &#x2212; 2
            &#x03C3;  3    &#x03C3;   n    +  &#x03C3;   n    2   &#x2212;  &#x03C4;
            n    2   = 0   {\displaystyle {\frac {\partial F}{\partial n_{3}}}=\sigma _
            {3}^{2}-2\sigma _{3}\sigma _{\mathrm {n} }+\sigma _{\mathrm {n} }^{2}-\tau
            _{\mathrm {n} }^{2}=0}  [{\displaystyle {\frac {\partial F}{\partial n_
            {3}}}=\sigma _{3}^{2}-2\sigma _{3}\sigma _{\mathrm {n} }+\sigma _{\mathrm
            {n} }^{2}-\tau _{\mathrm {n} }^{2}=0}]
      To find the values for      n  2     {\displaystyle n_{2}}  [n_{2}] and      n  3
      {\displaystyle n_{3}}  [n_{3}] we first add these two equations
                    &#x03C3;  2   2   &#x2212;  &#x03C3;  3   2   &#x2212; 2  &#x03C3;
            2    &#x03C3;  n   + 2  &#x03C3;  3    &#x03C3;  n      = 0      &#x03C3;
            2   2   &#x2212;  &#x03C3;  3   2   &#x2212; 2  &#x03C3;  n    (   &#x03C3;
            2   &#x2212;  &#x03C3;  3    )     = 0      &#x03C3;  2   +  &#x03C3;  3
            = 2  &#x03C3;  n         {\displaystyle {\begin{aligned}\sigma _{2}^{2}-
            \sigma _{3}^{2}-2\sigma _{2}\sigma _{n}+2\sigma _{3}\sigma _{n}&=0\\\sigma
            _{2}^{2}-\sigma _{3}^{2}-2\sigma _{n}\left(\sigma _{2}-\sigma _
            {3}\right)&=0\\\sigma _{2}+\sigma _{3}&=2\sigma _{n}\end{aligned}}}  [
            {\displaystyle {\begin{aligned}\sigma _{2}^{2}-\sigma _{3}^{2}-2\sigma _
            {2}\sigma _{n}+2\sigma _{3}\sigma _{n}&=0\\\sigma _{2}^{2}-\sigma _{3}^{2}-
            2\sigma _{n}\left(\sigma _{2}-\sigma _{3}\right)&=0\\\sigma _{2}+\sigma _
            {3}&=2\sigma _{n}\end{aligned}}}]
      Knowing that for      n  1   = 0   {\displaystyle n_{1}=0}  [{\displaystyle n_
      {1}=0}]
                &#x03C3;   n    =  &#x03C3;  1    n  1   2   +  &#x03C3;  2    n  2   2
            +  &#x03C3;  3    n  3   2   =  &#x03C3;  2    n  2   2   +  &#x03C3;  3
            n  3   2     {\displaystyle \sigma _{\mathrm {n} }=\sigma _{1}n_{1}^
            {2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^{2}=\sigma _{2}n_{2}^{2}+\sigma _
            {3}n_{3}^{2}}  [{\displaystyle \sigma _{\mathrm {n} }=\sigma _{1}n_{1}^
            {2}+\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^{2}=\sigma _{2}n_{2}^{2}+\sigma _
            {3}n_{3}^{2}}]
      and
                n  1   2   +  n  2   2   +  n  3   2   =  n  2   2   +  n  3   2   = 1
            {\displaystyle n_{1}^{2}+n_{2}^{2}+n_{3}^{2}=n_{2}^{2}+n_{3}^{2}=1}  [
            {\displaystyle n_{1}^{2}+n_{2}^{2}+n_{3}^{2}=n_{2}^{2}+n_{3}^{2}=1}]
      we have
                    &#x03C3;  2   +  &#x03C3;  3      = 2  &#x03C3;  n        &#x03C3;
            2   +  &#x03C3;  3      = 2  (   &#x03C3;  2    n  2   2   +  &#x03C3;  3
            n  3   2    )       &#x03C3;  2   +  &#x03C3;  3      = 2  (   &#x03C3;  2
            n  2   2   +  &#x03C3;  3    (  1 &#x2212;  n  2   2    )   )    = 0
            {\displaystyle {\begin{aligned}\sigma _{2}+\sigma _{3}&=2\sigma _
            {n}\\\sigma _{2}+\sigma _{3}&=2\left(\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^
            {2}\right)\\\sigma _{2}+\sigma _{3}&=2\left(\sigma _{2}n_{2}^{2}+\sigma _
            {3}\left(1-n_{2}^{2}\right)\right)&=0\end{aligned}}}  [{\displaystyle
            {\begin{aligned}\sigma _{2}+\sigma _{3}&=2\sigma _{n}\\\sigma _{2}+\sigma _
            {3}&=2\left(\sigma _{2}n_{2}^{2}+\sigma _{3}n_{3}^{2}\right)\\\sigma _
            {2}+\sigma _{3}&=2\left(\sigma _{2}n_{2}^{2}+\sigma _{3}\left(1-n_{2}^
            {2}\right)\right)&=0\end{aligned}}}]
      and solving for      n  2     {\displaystyle n_{2}}  [n_{2}] we have
                n  2   = &#x00B1;   1  2      {\displaystyle n_{2}=\pm {\frac {1}{\sqrt
            {2}}}}  [{\displaystyle n_{2}=\pm {\frac {1}{\sqrt {2}}}}]
      Then solving for      n  3     {\displaystyle n_{3}}  [n_{3}] we have
                n  3   =   1 &#x2212;  n  2   2     = &#x00B1;   1  2
            {\displaystyle n_{3}={\sqrt {1-n_{2}^{2}}}=\pm {\frac {1}{\sqrt {2}}}}  [
            {\displaystyle n_{3}={\sqrt {1-n_{2}^{2}}}=\pm {\frac {1}{\sqrt {2}}}}]
      and
                    &#x03C4;   n    2      = (  &#x03C3;  2   &#x2212;  &#x03C3;  3
            )  2    n  2   2    n  3   2        &#x03C4;   n       =     &#x03C3;  2
            &#x2212;  &#x03C3;  3    2         {\displaystyle {\begin{aligned}\tau _
            {\mathrm {n} }^{2}&=(\sigma _{2}-\sigma _{3})^{2}n_{2}^{2}n_{3}^{2}\\\tau _
            {\mathrm {n} }&={\frac {\sigma _{2}-\sigma _{3}}{2}}\end{aligned}}}  [
            {\displaystyle {\begin{aligned}\tau _{\mathrm {n} }^{2}&=(\sigma _{2}-
            \sigma _{3})^{2}n_{2}^{2}n_{3}^{2}\\\tau _{\mathrm {n} }&={\frac {\sigma _
            {2}-\sigma _{3}}{2}}\end{aligned}}}]
      The other two possible values for      &#x03C4;   n      {\displaystyle \tau _
      {\mathrm {n} }}  [\tau _{{\mathrm  {n}}}] can be obtained similarly by assuming
                n  2   = 0 ,   n  1   &#x2260; 0   {\displaystyle n_{2}=0,\,n_{1}\neq
            0}  [{\displaystyle n_{2}=0,\,n_{1}\neq 0}] and      n  3   &#x2260; 0
            {\displaystyle n_{3}\neq 0}  [{\displaystyle n_{3}\neq 0}]
                n  3   = 0 ,   n  1   &#x2260; 0   {\displaystyle n_{3}=0,\,n_{1}\neq
            0}  [{\displaystyle n_{3}=0,\,n_{1}\neq 0}] and      n  2   &#x2260; 0
            {\displaystyle n_{2}\neq 0}  [{\displaystyle n_{2}\neq 0}]
      Therefore, the second set of solutions for        &#x2202; F   &#x2202;  n  1
      = 0   {\displaystyle {\frac {\partial F}{\partial n_{1}}}=0}  [{\displaystyle
      {\frac {\partial F}{\partial n_{1}}}=0}], representing a maximum for
      &#x03C4;   n      {\displaystyle \tau _{\mathrm {n} }}  [\tau _{{\mathrm  {n}}}]
      is
                n  1   = 0 ,    n  2   = &#x00B1;   1  2    ,    n  3   = &#x00B1;   1
            2    ,    &#x03C4;   n    = &#x00B1;     &#x03C3;  2   &#x2212;  &#x03C3;
            3    2     {\displaystyle n_{1}=0,\,\,n_{2}=\pm {\frac {1}{\sqrt
            {2}}},\,\,n_{3}=\pm {\frac {1}{\sqrt {2}}},\,\,\tau _{\mathrm {n} }=\pm
            {\frac {\sigma _{2}-\sigma _{3}}{2}}}  [{\displaystyle n_{1}=0,\,\,n_
            {2}=\pm {\frac {1}{\sqrt {2}}},\,\,n_{3}=\pm {\frac {1}{\sqrt
            {2}}},\,\,\tau _{\mathrm {n} }=\pm {\frac {\sigma _{2}-\sigma _{3}}{2}}}]
                n  1   = &#x00B1;   1  2    ,    n  2   = 0 ,    n  3   = &#x00B1;   1
            2    ,    &#x03C4;   n    = &#x00B1;     &#x03C3;  1   &#x2212;  &#x03C3;
            3    2     {\displaystyle n_{1}=\pm {\frac {1}{\sqrt {2}}},\,\,n_
            {2}=0,\,\,n_{3}=\pm {\frac {1}{\sqrt {2}}},\,\,\tau _{\mathrm {n} }=\pm
            {\frac {\sigma _{1}-\sigma _{3}}{2}}}  [{\displaystyle n_{1}=\pm {\frac {1}
            {\sqrt {2}}},\,\,n_{2}=0,\,\,n_{3}=\pm {\frac {1}{\sqrt {2}}},\,\,\tau _
            {\mathrm {n} }=\pm {\frac {\sigma _{1}-\sigma _{3}}{2}}}]
                n  1   = &#x00B1;   1  2    ,    n  2   = &#x00B1;   1  2    ,    n  3
            = 0 ,    &#x03C4;   n    = &#x00B1;     &#x03C3;  1   &#x2212;  &#x03C3;  2
            2     {\displaystyle n_{1}=\pm {\frac {1}{\sqrt {2}}},\,\,n_{2}=\pm {\frac
            {1}{\sqrt {2}}},\,\,n_{3}=0,\,\,\tau _{\mathrm {n} }=\pm {\frac {\sigma _
            {1}-\sigma _{2}}{2}}}  [{\displaystyle n_{1}=\pm {\frac {1}{\sqrt
            {2}}},\,\,n_{2}=\pm {\frac {1}{\sqrt {2}}},\,\,n_{3}=0,\,\,\tau _{\mathrm
            {n} }=\pm {\frac {\sigma _{1}-\sigma _{2}}{2}}}]
      Therefore, assuming      &#x03C3;  1   &#x2265;  &#x03C3;  2   &#x2265;  &#x03C3;
      3     {\displaystyle \sigma _{1}\geq \sigma _{2}\geq \sigma _{3}}  [
      {\displaystyle \sigma _{1}\geq \sigma _{2}\geq \sigma _{3}}], the maximum shear
      stress is expressed by
                &#x03C4;   m a x    =   1 2    |   &#x03C3;  1   &#x2212;  &#x03C3;  3
            |  =   1 2    |   &#x03C3;   m a x    &#x2212;  &#x03C3;   m i n     |
            {\displaystyle \tau _{\mathrm {max} }={\frac {1}{2}}\left|\sigma _{1}-
            \sigma _{3}\right|={\frac {1}{2}}\left|\sigma _{\mathrm {max} }-\sigma _
            {\mathrm {min} }\right|}  [{\displaystyle \tau _{\mathrm {max} }={\frac {1}
            {2}}\left|\sigma _{1}-\sigma _{3}\right|={\frac {1}{2}}\left|\sigma _
            {\mathrm {max} }-\sigma _{\mathrm {min} }\right|}]
      and it can be stated as being equal to one-half the difference between the
      largest and smallest principal stresses, acting on the plane that bisects the
      angle between the directions of the largest and smallest principal stresses.
***** Stress deviator tensor[edit] *****
The stress tensor      &#x03C3;  i j     {\displaystyle \sigma _{ij}}  [\sigma
_{ij}] can be expressed as the sum of two other stress tensors:
   1. a mean hydrostatic_stress tensor or volumetric stress tensor or mean
      normal stress tensor,     &#x03C0;  &#x03B4;  i j     {\displaystyle \pi
      \delta _{ij}}  [{\displaystyle \pi \delta _{ij}}], which tends to change
      the volume of the stressed body; and
   2. a deviatoric component called the stress deviator tensor,      s  i j
      {\displaystyle s_{ij}}  [s_{ij}], which tends to distort it.
So:
          &#x03C3;  i j   =  s  i j   + &#x03C0;  &#x03B4;  i j   ,
      {\displaystyle \sigma _{ij}=s_{ij}+\pi \delta _{ij},\,}  [\sigma_{ij}= s_
      {ij} + \pi\delta_{ij},\,]
where     &#x03C0;   {\displaystyle \pi }  [\pi ] is the mean stress given by
         &#x03C0; =    &#x03C3;  k k   3   =     &#x03C3;  11   +  &#x03C3;  22
      +  &#x03C3;  33    3   =    1 3     I  1   .    {\displaystyle \pi =
      {\frac {\sigma _{kk}}{3}}={\frac {\sigma _{11}+\sigma _{22}+\sigma _{33}}
      {3}}={\tfrac {1}{3}}I_{1}.\,}  [\pi=\frac{\sigma_{kk}}{3}=\frac{\sigma_
      {11}+\sigma_{22}+\sigma_{33}}{3}=\tfrac{1}{3}I_1.\,]
Pressure (    p   {\displaystyle p}  [p]) is generally defined as negative one-
third the trace of the stress tensor minus any stress the divergence of the
velocity contributes with, i.e.
         p = &#x03BB;  &#x2207; &#x22C5;    u &#x2192;    &#x2212; &#x03C0; =
      &#x03BB;     &#x2202;  u  k     &#x2202;  x  k      &#x2212; &#x03C0; =
      &#x2211;  k   &#x03BB;     &#x2202;  u  k     &#x2202;  x  k
      &#x2212; &#x03C0; ,   {\displaystyle p=\lambda \,\nabla \cdot {\vec {u}}-
      \pi =\lambda \,{\frac {\partial u_{k}}{\partial x_{k}}}-\pi =\sum _
      {k}\lambda \,{\frac {\partial u_{k}}{\partial x_{k}}}-\pi ,}  [p =
      \lambda\, \nabla\cdot\vec{u} -\pi = \lambda\,\frac{\partial u_k}{\partial
      x_k} -\pi = \sum_k\lambda\,\frac{\partial u_k}{\partial x_k} -\pi,]
where     &#x03BB;   {\displaystyle \lambda }  [\lambda ] is a proportionality
constant,     &#x2207;   {\displaystyle \nabla }  [\nabla ] is the divergence
operator,      x  k     {\displaystyle x_{k}}  [x_{k}] is the k:th Cartesian
coordinate,        u &#x2192;      {\displaystyle {\vec {u}}}  [{\vec {u}}] is
the velocity and      u  k     {\displaystyle u_{k}}  [u_{k}] is the k:th
Cartesian component of        u &#x2192;      {\displaystyle {\vec {u}}}  [
{\vec {u}}].
The deviatoric stress tensor can be obtained by subtracting the hydrostatic
stress tensor from the Cauchy stress tensor:
             &#xA0;  s  i j      =  &#x03C3;  i j   &#x2212;    &#x03C3;  k k
      3    &#x03B4;  i j   ,       [      s  11      s  12      s  13        s
      21      s  22      s  23        s  31      s  32      s  33       ]     =
      [      &#x03C3;  11      &#x03C3;  12      &#x03C3;  13        &#x03C3;
      21      &#x03C3;  22      &#x03C3;  23        &#x03C3;  31      &#x03C3;
      32      &#x03C3;  33       ]  &#x2212;  [     &#x03C0;   0   0     0
      &#x03C0;   0     0   0   &#x03C0;     ]        =  [      &#x03C3;  11
      &#x2212; &#x03C0;    &#x03C3;  12      &#x03C3;  13        &#x03C3;  21
      &#x03C3;  22   &#x2212; &#x03C0;    &#x03C3;  23        &#x03C3;  31
      &#x03C3;  32      &#x03C3;  33   &#x2212; &#x03C0;     ]  .
      {\displaystyle {\begin{aligned}\ s_{ij}&=\sigma _{ij}-{\frac {\sigma _
      {kk}}{3}}\delta _{ij},\,\\\left[{\begin{matrix}s_{11}&s_{12}&s_{13}\\s_
      {21}&s_{22}&s_{23}\\s_{31}&s_{32}&s_{33}\end{matrix}}\right]&=\left[
      {\begin{matrix}\sigma _{11}&\sigma _{12}&\sigma _{13}\\\sigma _
      {21}&\sigma _{22}&\sigma _{23}\\\sigma _{31}&\sigma _{32}&\sigma _
      {33}\end{matrix}}\right]-\left[{\begin{matrix}\pi &0&0\\0&\pi &0\\0&0&\pi
      \end{matrix}}\right]\\&=\left[{\begin{matrix}\sigma _{11}-\pi &\sigma _
      {12}&\sigma _{13}\\\sigma _{21}&\sigma _{22}-\pi &\sigma _{23}\\\sigma _
      {31}&\sigma _{32}&\sigma _{33}-\pi \end{matrix}}\right].\end{aligned}}}
      [\begin{align}
      \ s_{ij} &= \sigma_{ij} - \frac{\sigma_{kk}}{3}\delta_{ij},\,\\
      \left[{\begin{matrix}
      s_{11} & s_{12} & s_{13} \\
      s_{21} & s_{22} & s_{23} \\
      s_{31} & s_{32} & s_{33}
      \end{matrix}}\right]
      &=\left[{\begin{matrix}
      \sigma_{11} & \sigma_{12} & \sigma_{13} \\
      \sigma_{21} & \sigma_{22} & \sigma_{23} \\
      \sigma_{31} & \sigma_{32} & \sigma_{33}
      \end{matrix}}\right]-\left[{\begin{matrix}
      \pi & 0   & 0   \\
      0   & \pi & 0   \\
      0   & 0   & \pi
      \end{matrix}}\right] \\
      &=\left[{\begin{matrix}
      \sigma_{11}-\pi & \sigma_{12}     & \sigma_{13} \\
      \sigma_{21}     & \sigma_{22}-\pi & \sigma_{23} \\
      \sigma_{31}     & \sigma_{32}     & \sigma_{33}-\pi
      \end{matrix}}\right].
      \end{align}]
**** Invariants of the stress deviator tensor[edit] ****
As it is a second order tensor, the stress deviator tensor also has a set of
invariants, which can be obtained using the same procedure used to calculate
the invariants of the stress tensor. It can be shown that the principal
directions of the stress deviator tensor      s  i j     {\displaystyle s_{ij}}
[s_{ij}] are the same as the principal directions of the stress tensor
&#x03C3;  i j     {\displaystyle \sigma _{ij}}  [\sigma _{ij}]. Thus, the
characteristic equation is
          |   s  i j   &#x2212; &#x03BB;  &#x03B4;  i j    |  = &#x2212;
      &#x03BB;  3   +  J  1    &#x03BB;  2   &#x2212;  J  2   &#x03BB; +  J  3
      = 0 ,   {\displaystyle \left|s_{ij}-\lambda \delta _{ij}\right|=-\lambda
      ^{3}+J_{1}\lambda ^{2}-J_{2}\lambda +J_{3}=0,}  [{\displaystyle \left|s_
      {ij}-\lambda \delta _{ij}\right|=-\lambda ^{3}+J_{1}\lambda ^{2}-J_
      {2}\lambda +J_{3}=0,}]
where      J  1     {\displaystyle J_{1}}  [J_{1}],      J  2
{\displaystyle J_{2}}  [J_{2}] and      J  3     {\displaystyle J_{3}}  [J_3]
are the first, second, and third deviatoric stress invariants, respectively.
Their values are the same (invariant) regardless of the orientation of the
coordinate system chosen. These deviatoric stress invariants can be expressed
as a function of the components of      s  i j     {\displaystyle s_{ij}}  [s_
{ij}] or its principal values      s  1     {\displaystyle s_{1}}  [s_{1}],
s  2     {\displaystyle s_{2}}  [s_{2}], and      s  3     {\displaystyle s_
{3}}  [s_{3}], or alternatively, as a function of      &#x03C3;  i j
{\displaystyle \sigma _{ij}}  [\sigma _{ij}] or its principal values
&#x03C3;  1     {\displaystyle \sigma _{1}}  [\sigma _{1}],      &#x03C3;  2
{\displaystyle \sigma _{2}}  [\sigma _{2}], and      &#x03C3;  3
{\displaystyle \sigma _{3}}  [\sigma_3]. Thus,
              J  1      =  s  k k   = 0 ,       J  2      =    1 2    s  i j
      s  j i   =    1 2     tr  (   s   2   )        =    1 2    (  s  1   2
      +  s  2   2   +  s  3   2   )       =    1 6     [  (  &#x03C3;  11
      &#x2212;  &#x03C3;  22    )  2   + (  &#x03C3;  22   &#x2212;  &#x03C3;
      33    )  2   + (  &#x03C3;  33   &#x2212;  &#x03C3;  11    )  2    ]  +
      &#x03C3;  12   2   +  &#x03C3;  23   2   +  &#x03C3;  31   2         =
      1 6     [  (  &#x03C3;  1   &#x2212;  &#x03C3;  2    )  2   + (  &#x03C3;
      2   &#x2212;  &#x03C3;  3    )  2   + (  &#x03C3;  3   &#x2212;  &#x03C3;
      1    )  2    ]        =    1 3     I  1   2   &#x2212;  I  2   =   1 2
      [   tr  (   &#x03C3;   2   ) &#x2212;   1 3    tr  (  &#x03C3;   )  2
      ]  ,       J  3      = det (  s  i j   )       =    1 3     s  i j    s
      j k    s  k i   =    1 3     tr  (   s   3   )       =    1 3    (  s  1
      3   +  s  2   3   +  s  3   3   )       =  s  1    s  2    s  3         =
      2 27     I  1   3   &#x2212;    1 3     I  1    I  2   +  I  3   =    1 3
      [   tr  (   &#x03C3;   3   ) &#x2212;  tr  (   &#x03C3;   2   )  tr
      (  &#x03C3;  ) +    2 9     tr  (  &#x03C3;   )  3    ]  .
      {\displaystyle {\begin{aligned}J_{1}&=s_{kk}=0,\,\\J_{2}&=\textstyle
      {\frac {1}{2}}s_{ij}s_{ji}={\tfrac {1}{2}}{\text{tr}}({\boldsymbol {s}}^
      {2})\\&={\tfrac {1}{2}}(s_{1}^{2}+s_{2}^{2}+s_{3}^{2})\\&={\tfrac {1}
      {6}}\left[(\sigma _{11}-\sigma _{22})^{2}+(\sigma _{22}-\sigma _{33})^
      {2}+(\sigma _{33}-\sigma _{11})^{2}\right]+\sigma _{12}^{2}+\sigma _{23}^
      {2}+\sigma _{31}^{2}\\&={\tfrac {1}{6}}\left[(\sigma _{1}-\sigma _{2})^
      {2}+(\sigma _{2}-\sigma _{3})^{2}+(\sigma _{3}-\sigma _{1})^
      {2}\right]\\&={\tfrac {1}{3}}I_{1}^{2}-I_{2}={\frac {1}{2}}\left[{\text
      {tr}}({\boldsymbol {\sigma }}^{2})-{\frac {1}{3}}{\text{tr}}({\boldsymbol
      {\sigma }})^{2}\right],\,\\J_{3}&=\det(s_{ij})\\&={\tfrac {1}{3}}s_{ij}s_
      {jk}s_{ki}={\tfrac {1}{3}}{\text{tr}}({\boldsymbol {s}}^{3})\\&={\tfrac
      {1}{3}}(s_{1}^{3}+s_{2}^{3}+s_{3}^{3})\\&=s_{1}s_{2}s_{3}\\&={\tfrac {2}
      {27}}I_{1}^{3}-{\tfrac {1}{3}}I_{1}I_{2}+I_{3}={\tfrac {1}{3}}\left[
      {\text{tr}}({\boldsymbol {\sigma }}^{3})-{\text{tr}}({\boldsymbol {\sigma
      }}^{2}){\text{tr}}({\boldsymbol {\sigma }})+{\tfrac {2}{9}}{\text{tr}}(
      {\boldsymbol {\sigma }})^{3}\right].\,\end{aligned}}}  [{\displaystyle
      {\begin{aligned}J_{1}&=s_{kk}=0,\,\\J_{2}&=\textstyle {\frac {1}{2}}s_
      {ij}s_{ji}={\tfrac {1}{2}}{\text{tr}}({\boldsymbol {s}}^{2})\\&={\tfrac
      {1}{2}}(s_{1}^{2}+s_{2}^{2}+s_{3}^{2})\\&={\tfrac {1}{6}}\left[(\sigma _
      {11}-\sigma _{22})^{2}+(\sigma _{22}-\sigma _{33})^{2}+(\sigma _{33}-
      \sigma _{11})^{2}\right]+\sigma _{12}^{2}+\sigma _{23}^{2}+\sigma _{31}^
      {2}\\&={\tfrac {1}{6}}\left[(\sigma _{1}-\sigma _{2})^{2}+(\sigma _{2}-
      \sigma _{3})^{2}+(\sigma _{3}-\sigma _{1})^{2}\right]\\&={\tfrac {1}
      {3}}I_{1}^{2}-I_{2}={\frac {1}{2}}\left[{\text{tr}}({\boldsymbol {\sigma
      }}^{2})-{\frac {1}{3}}{\text{tr}}({\boldsymbol {\sigma }})^
      {2}\right],\,\\J_{3}&=\det(s_{ij})\\&={\tfrac {1}{3}}s_{ij}s_{jk}s_{ki}=
      {\tfrac {1}{3}}{\text{tr}}({\boldsymbol {s}}^{3})\\&={\tfrac {1}{3}}(s_
      {1}^{3}+s_{2}^{3}+s_{3}^{3})\\&=s_{1}s_{2}s_{3}\\&={\tfrac {2}{27}}I_{1}^
      {3}-{\tfrac {1}{3}}I_{1}I_{2}+I_{3}={\tfrac {1}{3}}\left[{\text{tr}}(
      {\boldsymbol {\sigma }}^{3})-{\text{tr}}({\boldsymbol {\sigma }}^{2})
      {\text{tr}}({\boldsymbol {\sigma }})+{\tfrac {2}{9}}{\text{tr}}(
      {\boldsymbol {\sigma }})^{3}\right].\,\end{aligned}}}]
Because      s  k k   = 0   {\displaystyle s_{kk}=0}  [{\displaystyle s_
{kk}=0}], the stress deviator tensor is in a state of pure shear.
A quantity called the equivalent stress or von_Mises_stress is commonly used in
solid mechanics. The equivalent stress is defined as
          &#x03C3;   v m    =   3 &#xA0;  J  2     =      1 2    &#xA0;  [
      (  &#x03C3;  1   &#x2212;  &#x03C3;  2    )  2   + (  &#x03C3;  2
      &#x2212;  &#x03C3;  3    )  2   + (  &#x03C3;  3   &#x2212;  &#x03C3;  1
      )  2    ]     .   {\displaystyle \sigma _{\mathrm {vm} }={\sqrt {3~J_
      {2}}}={\sqrt {{\tfrac {1}{2}}~\left[(\sigma _{1}-\sigma _{2})^{2}+(\sigma
      _{2}-\sigma _{3})^{2}+(\sigma _{3}-\sigma _{1})^{2}\right]}}\,.}  [
      {\displaystyle \sigma _{\mathrm {vm} }={\sqrt {3~J_{2}}}={\sqrt {{\tfrac
      {1}{2}}~\left[(\sigma _{1}-\sigma _{2})^{2}+(\sigma _{2}-\sigma _{3})^
      {2}+(\sigma _{3}-\sigma _{1})^{2}\right]}}\,.}]
***** Octahedral stresses[edit] *****
Figure 6. Octahedral stress planes
Considering the principal directions as the coordinate axes, a plane whose
normal vector makes equal angles with each of the principal axes (i.e. having
direction cosines equal to      |  1  /    3    |    {\displaystyle |1/{\sqrt
{3}}|}  [{\displaystyle |1/{\sqrt {3}}|}]) is called an octahedral plane. There
are a total of eight octahedral planes (Figure 6). The normal and shear
components of the stress tensor on these planes are called octahedral normal
stress      &#x03C3;   o c t      {\displaystyle \sigma _{\mathrm {oct} }}  [
{\displaystyle \sigma _{\mathrm {oct} }}] and octahedral shear stress
&#x03C4;   o c t      {\displaystyle \tau _{\mathrm {oct} }}  [{\displaystyle
\tau _{\mathrm {oct} }}], respectively. Octahedral plane passing through the
origin is known as the Ï-plane (Ï not to be confused with mean stress denoted
by Ï in above section) . On the Ï-plane,      s  i j   = I  /  3
{\displaystyle s_{ij}=I/3}  [{\displaystyle s_{ij}=I/3}].
Knowing that the stress tensor of point O (Figure 6) in the principal axes is
          &#x03C3;  i j   =   [     &#x03C3;  1     0   0     0    &#x03C3;  2
      0     0   0    &#x03C3;  3      ]     {\displaystyle \sigma _{ij}={\begin
      {bmatrix}\sigma _{1}&0&0\\0&\sigma _{2}&0\\0&0&\sigma _{3}\end{bmatrix}}}
      [{\displaystyle \sigma _{ij}={\begin{bmatrix}\sigma _{1}&0&0\\0&\sigma _
      {2}&0\\0&0&\sigma _{3}\end{bmatrix}}}]
the stress vector on an octahedral plane is then given by:
               T    o c t    (  n  )      =  &#x03C3;  i j    n  i     e   j
      =  &#x03C3;  1    n  1     e   1   +  &#x03C3;  2    n  2     e   2   +
      &#x03C3;  3    n  3     e   3         =    1  3     (  &#x03C3;  1     e
      1   +  &#x03C3;  2     e   2   +  &#x03C3;  3     e   3   )
      {\displaystyle {\begin{aligned}\mathbf {T} _{\mathrm {oct} }^{(\mathbf
      {n} )}&=\sigma _{ij}n_{i}\mathbf {e} _{j}\\&=\sigma _{1}n_{1}\mathbf {e}
      _{1}+\sigma _{2}n_{2}\mathbf {e} _{2}+\sigma _{3}n_{3}\mathbf {e} _
      {3}\\&={\tfrac {1}{\sqrt {3}}}(\sigma _{1}\mathbf {e} _{1}+\sigma _
      {2}\mathbf {e} _{2}+\sigma _{3}\mathbf {e} _{3})\end{aligned}}}  [
      {\displaystyle {\begin{aligned}\mathbf {T} _{\mathrm {oct} }^{(\mathbf
      {n} )}&=\sigma _{ij}n_{i}\mathbf {e} _{j}\\&=\sigma _{1}n_{1}\mathbf {e}
      _{1}+\sigma _{2}n_{2}\mathbf {e} _{2}+\sigma _{3}n_{3}\mathbf {e} _
      {3}\\&={\tfrac {1}{\sqrt {3}}}(\sigma _{1}\mathbf {e} _{1}+\sigma _
      {2}\mathbf {e} _{2}+\sigma _{3}\mathbf {e} _{3})\end{aligned}}}]
The normal component of the stress vector at point O associated with the
octahedral plane is
              &#x03C3;   o c t       =  T  i   ( n )    n  i         =
      &#x03C3;  i j    n  i    n  j         =  &#x03C3;  1    n  1    n  1   +
      &#x03C3;  2    n  2    n  2   +  &#x03C3;  3    n  3    n  3         =
      1 3    (  &#x03C3;  1   +  &#x03C3;  2   +  &#x03C3;  3   ) =    1 3
      I  1         {\displaystyle {\begin{aligned}\sigma _{\mathrm {oct} }&=T_
      {i}^{(n)}n_{i}\\&=\sigma _{ij}n_{i}n_{j}\\&=\sigma _{1}n_{1}n_{1}+\sigma
      _{2}n_{2}n_{2}+\sigma _{3}n_{3}n_{3}\\&={\tfrac {1}{3}}(\sigma _
      {1}+\sigma _{2}+\sigma _{3})={\tfrac {1}{3}}I_{1}\end{aligned}}}  [
      {\displaystyle {\begin{aligned}\sigma _{\mathrm {oct} }&=T_{i}^{(n)}n_
      {i}\\&=\sigma _{ij}n_{i}n_{j}\\&=\sigma _{1}n_{1}n_{1}+\sigma _{2}n_{2}n_
      {2}+\sigma _{3}n_{3}n_{3}\\&={\tfrac {1}{3}}(\sigma _{1}+\sigma _
      {2}+\sigma _{3})={\tfrac {1}{3}}I_{1}\end{aligned}}}]
which is the mean normal stress or hydrostatic stress. This value is the same
in all eight octahedral planes. The shear stress on the octahedral plane is
then
              &#x03C4;   o c t       =    T  i   ( n )    T  i   ( n )
      &#x2212;  &#x03C3;   n    2           =   [     1 3    (  &#x03C3;  1   2
      +  &#x03C3;  2   2   +  &#x03C3;  3   2   ) &#x2212;    1 9
      (  &#x03C3;  1   +  &#x03C3;  2   +  &#x03C3;  3    )  2    ]   1  /  2
      =    1 3      [  (  &#x03C3;  1   &#x2212;  &#x03C3;  2    )  2   +
      (  &#x03C3;  2   &#x2212;  &#x03C3;  3    )  2   + (  &#x03C3;  3
      &#x2212;  &#x03C3;  1    )  2    ]   1  /  2   =    1 3      2  I  1   2
      &#x2212; 6  I  2     =      2 3     J  2           {\displaystyle {\begin
      {aligned}\tau _{\mathrm {oct} }&={\sqrt {T_{i}^{(n)}T_{i}^{(n)}-\sigma _
      {\mathrm {n} }^{2}}}\\&=\left[{\tfrac {1}{3}}(\sigma _{1}^{2}+\sigma _
      {2}^{2}+\sigma _{3}^{2})-{\tfrac {1}{9}}(\sigma _{1}+\sigma _{2}+\sigma _
      {3})^{2}\right]^{1/2}\\&={\tfrac {1}{3}}\left[(\sigma _{1}-\sigma _{2})^
      {2}+(\sigma _{2}-\sigma _{3})^{2}+(\sigma _{3}-\sigma _{1})^{2}\right]^
      {1/2}={\tfrac {1}{3}}{\sqrt {2I_{1}^{2}-6I_{2}}}={\sqrt {{\tfrac {2}
      {3}}J_{2}}}\end{aligned}}}  [{\displaystyle {\begin{aligned}\tau _
      {\mathrm {oct} }&={\sqrt {T_{i}^{(n)}T_{i}^{(n)}-\sigma _{\mathrm {n} }^
      {2}}}\\&=\left[{\tfrac {1}{3}}(\sigma _{1}^{2}+\sigma _{2}^{2}+\sigma _
      {3}^{2})-{\tfrac {1}{9}}(\sigma _{1}+\sigma _{2}+\sigma _{3})^{2}\right]^
      {1/2}\\&={\tfrac {1}{3}}\left[(\sigma _{1}-\sigma _{2})^{2}+(\sigma _{2}-
      \sigma _{3})^{2}+(\sigma _{3}-\sigma _{1})^{2}\right]^{1/2}={\tfrac {1}
      {3}}{\sqrt {2I_{1}^{2}-6I_{2}}}={\sqrt {{\tfrac {2}{3}}J_{2}}}\end
      {aligned}}}]
***** See also[edit] *****
    * Critical_plane_analysis
***** References[edit] *****
   1. ^ a b c  Fridtjov Irgens (2008), "Continuum_Mechanics". Springer.
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
   3. ISBN 3-540-74297-2
   4. ^ Truesdell_&_Toupin_1960
   5. ^  Peter Chadwick (1999), "Continuum_Mechanics:_Concise_Theory_and
      Problems". Dover Publications, series "Books on Physics".
   6. ISBN 0-486-40180-4. pages
   7. ^ a b  Yuan-cheng Fung and Pin Tong (2001) "Classical_and_Computational
      Solid_Mechanics". World Scientific.
   8. ISBN 981-02-4124-0
   9. ^ a b Smith & Truesdell p.97
  10. ^ a b  G. Thomas Mase and George E. Mase (1999), "Continuum_Mechanics_for
      Engineers" (2nd edition). CRC Press.
  11. ISBN 0-8493-1855-6
  12. ^ a b c  I-Shih Liu (2002), "Continuum_Mechanics". Springer
  13. ISBN 3-540-43019-9
  14. ^ a b  Han-Chin Wu (2005), "Continuum_Mechanics_and_Plasticity". CRC
      Press.
  15. ISBN 1-58488-363-4
  16. ^ Lubliner
  17. ^ Basar
  18. ^ a b c  Teodor M. Atanackovic and ArdÃ©shir Guran (2000), "Theory_of
      Elasticity_for_Scientists_and_Engineers". Springer.
  19. ISBN 0-8176-4072-X
  20. ^  Keith D. Hjelmstad (2005), "Fundamentals_of_Structural_Mechanics" (2nd
      edition). Prentice-Hall.
  21. ISBN 0-387-23330-X
  22. ^ a b  Wai-Fah Chen and Da-Jian Han (2007), "Plasticity_for_Structural
      Engineers". J. Ross Publishing
  23. ISBN 1-932159-75-4
  24. ^  Bernard Hamrock (2005), "Fundamentals_of_Machine_Elements".
      McGrawâHill.
  25. ISBN 0-07-297682-9
  26. ^  Rabindranath Chatterjee (1999), "Mathematical_Theory_of_Continuum
      Mechanics". Alpha Science.
  27. ISBN 81-7319-244-8
  28. ^  John Conrad Jaeger, N. G. W. Cook, and R. W. Zimmerman (2007),
      "Fundamentals_of_Rock_Mechanics" (4th edition). Wiley-Blackwell.
  29. ISBN 0-632-05759-9
  30. ^  Mohammed Ameen (2005), "Computational_Elasticity:_Theory_of_Elasticity
      and_Finite_and_Boundary_Element_Methods" (book). Alpha Science,
  31. ISBN 1-84265-201-X
  32. ^  William Prager (2004), "Introduction_to_Mechanics_of_Continua". Dover
      Publications.
  33. ISBN 0-486-43809-0
    * v
    * t
    * e
Tensors
Glossary_of_tensor_theory
                                      * coordinate_system
                                      * multilinear_algebra
                                      * Euclidean_geometry
                Mathematics           * tensor_algebra
                                      * dyadic_algebra
                                      * differential_geometry
Scope                                 * exterior_calculus
                                      * tensor_calculus
                                      * continuum_mechanics
                    * Physics         * electromagnetism
                    * Engineering     * transport_phenomena
                                      * general_relativity
                                      * computer_vision
                    * index_notation
                    * multi-index_notation
                    * Einstein_notation
                    * Ricci_calculus
Notation            * Penrose_graphical_notation
                    * Voigt_notation
                    * abstract_index_notation
                    * tetrad_(index_notation)
                    * Van_der_Waerden_notation
                    * tensor_(intrinsic_definition)
                    * tensor_field
                    * tensor_density
                    * tensors_in_curvilinear_coordinates
Tensor              * mixed_tensor
definitions         * antisymmetric_tensor
                    * symmetric_tensor
                    * tensor_operator
                    * tensor_bundle
                    * two-point_tensor
                    * tensor_product
                    * exterior_product
                    * tensor_contraction
                    * transpose_(2nd-order_tensors)
Operations          * raising_and_lowering_indices
                    * Hodge_star_operator
                    * covariant_derivative
                    * exterior_derivative
                    * exterior_covariant_derivative
                    * Lie_derivative
                    * dimension
                    * basis
                    * vector, vector_space
                    * multivector
                    * covariance_and_contravariance_of_vectors
                    * linear_transformation
                    * matrix
Related             * spinor
abstractions        * Cartan_formalism_(physics)
                    * differential_form
                    * exterior_form
                    * connection_form
                    * geodesic
                    * manifold
                    * fiber_bundle
                    * Levi-Civita_connection
                    * affine_connection
                                * Kronecker_delta
                                * Levi-Civita_symbol
                                * metric_tensor
                                * nonmetricity_tensor
                Mathematics     * Christoffel_symbols
                                * Ricci_curvature
                                * Riemann_curvature_tensor
                                * Weyl_tensor
Notable tensors                 * torsion_tensor
                                * moment_of_inertia
                                * angular_momentum_tensor
                                * spin_tensor
                                * Cauchy stress tensor
                Physics         * stressâenergy_tensor
                                * EM_tensor
                                * gluon_field_strength_tensor
                                * Einstein_tensor
                                * metric_tensor_(GR)
                    * Leonhard_Euler
                    * Carl_Friedrich_Gauss
                    * Augustin-Louis_Cauchy
                    * Hermann_Grassmann
                    * Gregorio_Ricci-Curbastro
                    * Tullio_Levi-Civita
Mathematicians      * Jan_Arnoldus_Schouten
                    * Bernhard_Riemann
                    * Elwin_Bruno_Christoffel
                    * Woldemar_Voigt
                    * Ãlie_Cartan
                    * Hermann_Weyl
                    * Albert_Einstein

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Cauchy_stress_tensor&oldid=908506214"
Categories:
    * Tensors
    * Solid_mechanics
    * Continuum_mechanics
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
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * ×¢××¨××ª
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 30 July 2019, at 04:45 (UTC).
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
