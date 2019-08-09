The following text has been accessed from https://en.wikipedia.org/wiki/Stream_function at Fri Aug 9 01:21:14 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Stream function ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For three-dimensional flows with axisymmetry, see Stokes_stream_function.
Streamlines â lines with a constant value of the stream function â for the
incompressible potential_flow_around_a_circular_cylinder in a uniform onflow.
The stream function is defined for incompressible (divergence-free) flows in
two dimensions â as well as in three dimensions with axisymmetry. The flow
velocity components can be expressed as the derivatives of the scalar stream
function. The stream function can be used to plot streamlines, which represent
the trajectories of particles in a steady flow. The two-dimensional Lagrange
stream function was introduced by Joseph_Louis_Lagrange in 1781.[1] The Stokes
stream_function is for axisymmetrical three-dimensional flow, and is named
after George_Gabriel_Stokes.[2]
Considering the particular case of fluid_dynamics, the difference between the
stream function values at any two points gives the volumetric flow rate (or
volumetric_flux) through a line connecting the two points.
Since streamlines are tangent to the flow velocity vector of the flow, the
value of the stream function must be constant along a streamline. The
usefulness of the stream function lies in the fact that the flow velocity
components in the x- and y- directions at a given point are given by the
partial_derivatives of the stream function at that point. A stream function may
be defined for any flow of dimensions greater than or equal to two, however the
two-dimensional case is generally the easiest to visualize and derive.
For two-dimensional potential_flow, streamlines are perpendicular to
equipotential lines. Taken together with the velocity_potential, the stream
function may be used to derive a complex potential. In other words, the stream
function accounts for the solenoidal part of a two-dimensional Helmholtz
decomposition, while the velocity potential accounts for the irrotational part.
⁰
***** Contents *****
    * 1_Two-dimensional_stream_function
          o 1.1_Definitions
                # 1.1.1_Definition_by_use_of_a_vector_potential
                # 1.1.2_Alternative_definition_(opposite_sign)
          o 1.2_Derivation_of_the_two-dimensional_stream_function
                # 1.2.1_Flow_in_Cartesian_coordinates
          o 1.3_Continuity:_the_derivation
          o 1.4_Vorticity
                # 1.4.1_Proof_that_a_constant_value_for_the_stream_function
                  corresponds_to_a_streamline
                # 1.4.2_Properties_of_the_stream_function
    * 2_References
          o 2.1_Citations
          o 2.2_Sources
    * 3_External_links
***** Two-dimensional stream function[edit] *****
**** Definitions[edit] ****
The volume flux through the curve between the points     A   {\displaystyle A}
[A] and     P .   {\displaystyle P.}  [P.]
Lamb and Batchelor define the stream function     &#x03C8; ( x , y , t )
{\displaystyle \psi (x,y,t)}  [\psi (x,y,t)] â in the point     P
{\displaystyle P}  [P] with two-dimensional coordinates     ( x , y )
{\displaystyle (x,y)}  [(x,y)] and as a function of time     t   {\displaystyle
t}  [t] â for an incompressible_flow by:[3]
         &#x03C8; =  &#x222B;  A   P    (  u   d  y &#x2212; v   d  x  )  .
      {\displaystyle \psi =\int _{A}^{P}\left(u\,{\text{d}}y-v\,{\text
      {d}}x\right).}  [\psi =\int _{A}^{P}\left(u\,{\text{d}}y-v\,{\text
      {d}}x\right).]
So the stream function     &#x03C8;   {\displaystyle \psi }  [\psi ] is the
volume_flux through the curve     A P   {\displaystyle AP}  [AP], that is: the
integral of the dot_product of the flow_velocity vector     ( u , v )
{\displaystyle (u,v)}  [(u,v)] and the normal     ( +  d  y , &#x2212;  d  x )
{\displaystyle (+{\text{d}}y,-{\text{d}}x)}  [(+{\text{d}}y,-{\text{d}}x)] to
the curve element     (  d  x ,  d  y ) .   {\displaystyle ({\text{d}}x,{\text
{d}}y).}  [({\text{d}}x,{\text{d}}y).] The point     A   {\displaystyle A}  [A]
is a reference point defining where the stream function is zero: a shift of
A   {\displaystyle A}  [A] results in adding a constant to the stream function
&#x03C8; .   {\displaystyle \psi .}  [\psi .]
An infinitesimal shift     &#x03B4; P = ( &#x03B4; x , &#x03B4; y )
{\displaystyle \delta P=(\delta x,\delta y)}  [\delta P=(\delta x,\delta y)] of
the position     P   {\displaystyle P}  [P] results in a stream function shift:
         &#x03B4; &#x03C8; = u  &#x03B4; y &#x2212; v  &#x03B4; x ,
      {\displaystyle \delta \psi =u\,\delta y-v\,\delta x,}  [\delta \psi
      =u\,\delta y-v\,\delta x,]
which is an exact_differential provided
            &#x2202; u   &#x2202; x    +    &#x2202; v   &#x2202; y    = 0.
      {\displaystyle {\frac {\partial u}{\partial x}}+{\frac {\partial v}
      {\partial y}}=0.}  [{\frac  {\partial u}{\partial x}}+{\frac  {\partial
      v}{\partial y}}=0.]
This is the condition of zero divergence resulting from flow incompressibility.
Since
         &#x03B4; &#x03C8; =    &#x2202; &#x03C8;   &#x2202; x     &#x03B4; x +
      &#x2202; &#x03C8;   &#x2202; y     &#x03B4; y ,   {\displaystyle \delta
      \psi ={\frac {\partial \psi }{\partial x}}\,\delta x+{\frac {\partial
      \psi }{\partial y}}\,\delta y,}  [\delta \psi ={\frac  {\partial \psi }
      {\partial x}}\,\delta x+{\frac  {\partial \psi }{\partial y}}\,\delta y,]
the flow velocity components have to be
         u =    &#x2202; &#x03C8;   &#x2202; y      {\displaystyle u={\frac
      {\partial \psi }{\partial y}}}  [{\displaystyle u={\frac {\partial \psi }
      {\partial y}}}]   and       v = &#x2212;    &#x2202; &#x03C8;   &#x2202;
      x      {\displaystyle v=-{\frac {\partial \psi }{\partial x}}}  [v=-
      {\frac  {\partial \psi }{\partial x}}]
in relation to the stream function     &#x03C8; .   {\displaystyle \psi .}
[\psi .]
*** Definition by use of a vector potential[edit] ***
The sign of the stream function depends on the definition used.
One way is to define the stream function     &#x03C8;   {\displaystyle \psi }
[\psi ] for a two-dimensional flow such that the flow_velocity can be expressed
through the vector_potential      &#x03C8;  :   {\displaystyle {\boldsymbol
{\psi }}:}  [{\boldsymbol  {\psi }}:]
          u  = &#x2207; &#x00D7;  &#x03C8;    {\displaystyle \mathbf {u}
      =\nabla \times {\boldsymbol {\psi }}}  [{\mathbf  {u}}=\nabla \times
      {\boldsymbol  {\psi }}]
Where      &#x03C8;  = ( 0 , 0 , &#x03C8; )   {\displaystyle {\boldsymbol {\psi
}}=(0,0,\psi )}  [{\boldsymbol  {\psi }}=(0,0,\psi )] if the flow velocity
vector      u  = ( u , v , 0 )   {\displaystyle \mathbf {u} =(u,v,0)}  [
{\mathbf  {u}}=(u,v,0)].
In Cartesian_coordinate_system this is equivalent to
         u =    &#x2202; &#x03C8;   &#x2202; y    ,  v = &#x2212;    &#x2202;
      &#x03C8;   &#x2202; x      {\displaystyle u={\frac {\partial \psi }
      {\partial y}},\qquad v=-{\frac {\partial \psi }{\partial x}}}  [u={\frac
      {\partial \psi }{\partial y}},\qquad v=-{\frac  {\partial \psi }{\partial
      x}}]
Where     u   {\displaystyle u}  [u] and     v   {\displaystyle v}  [v] are the
flow velocity components in the cartesian     x   {\displaystyle x}  [x] and
y   {\displaystyle y}  [y] coordinate directions, respectively.
*** Alternative definition (opposite sign)[edit] ***
Another definition (used more widely in meteorology and oceanography than the
above) is
          u  =  z  &#x00D7; &#x2207;  &#x03C8; &#x2032;  &#x2261; ( &#x2212;
      &#x03C8;  y  &#x2032;  ,  &#x03C8;  x  &#x2032;  , 0 )   {\displaystyle
      \mathbf {u} =\mathbf {z} \times \nabla \psi '\equiv (-\psi '_{y},\psi '_
      {x},0)}  [{\mathbf  {u}}={\mathbf  {z}}\times \nabla \psi '\equiv (-\psi
      '_{y},\psi '_{x},0)],
where      z  = ( 0 , 0 , 1 )   {\displaystyle \mathbf {z} =(0,0,1)}  [{\mathbf
{z}}=(0,0,1)] is a unit vector in the     + z   {\displaystyle +z}  [+z]
direction and the subscripts indicate partial derivatives.
Note that this definition has the opposite sign to that given above
(     &#x03C8; &#x2032;  = &#x2212; &#x03C8;   {\displaystyle \psi '=-\psi }
[\psi '=-\psi ]), so we have
         u = &#x2212;    &#x2202;  &#x03C8; &#x2032;    &#x2202; y    ,  v =
      &#x2202;  &#x03C8; &#x2032;    &#x2202; x      {\displaystyle u=-{\frac
      {\partial \psi '}{\partial y}},\qquad v={\frac {\partial \psi '}{\partial
      x}}}  [{\displaystyle u=-{\frac {\partial \psi '}{\partial y}},\qquad v=
      {\frac {\partial \psi '}{\partial x}}}]
in Cartesian coordinates.
All formulations of the stream function constrain the velocity to satisfy the
two-dimensional continuity_equation exactly:
            &#x2202; u   &#x2202; x    +    &#x2202; v   &#x2202; y    = 0
      {\displaystyle {\frac {\partial u}{\partial x}}+{\frac {\partial v}
      {\partial y}}=0}  [{\frac  {\partial u}{\partial x}}+{\frac  {\partial v}
      {\partial y}}=0]
The last two definitions of stream function are related through the vector
calculus_identity
         &#x2207; &#x00D7;  (  &#x03C8;  z   )  = &#x03C8; &#x2207; &#x00D7;  z
      + &#x2207; &#x03C8; &#x00D7;  z  = &#x2207; &#x03C8; &#x00D7;  z  =  z
      &#x00D7; &#x2207;  &#x03C8; &#x2032;  .   {\displaystyle \nabla \times
      \left(\psi \mathbf {z} \right)=\psi \nabla \times \mathbf {z} +\nabla
      \psi \times \mathbf {z} =\nabla \psi \times \mathbf {z} =\mathbf {z}
      \times \nabla \psi '.}  [\nabla \times \left(\psi {\mathbf
      {z}}\right)=\psi \nabla \times {\mathbf  {z}}+\nabla \psi \times {\mathbf
      {z}}=\nabla \psi \times {\mathbf  {z}}={\mathbf  {z}}\times \nabla \psi
      '.]
Note that      &#x03C8;  = &#x03C8;  z    {\displaystyle {\boldsymbol {\psi
}}=\psi \mathbf {z} }  [{\boldsymbol  {\psi }}=\psi {\mathbf  {z}}] in this
two-dimensional flow.
**** Derivation of the two-dimensional stream function[edit] ****
Consider two points A and B in two-dimensional plane flow. If the distance
between these two points is very small: Î´n, and a stream of flow passes
between these points with an average velocity, q perpendicular to the line AB,
the volume flow rate per unit thickness, Î´Î¨ is given by:
         &#x03B4; &#x03C8; = q &#x03B4; n    {\displaystyle \delta \psi
      =q\delta n\,}  [\delta \psi =q\delta n\,]
As Î´n â 0, rearranging this expression, we get:
         q =    &#x2202; &#x03C8;   &#x2202; n       {\displaystyle q={\frac
      {\partial \psi }{\partial n}}\,}  [q={\frac  {\partial \psi }{\partial
      n}}\,]
Now consider two-dimensional plane flow with reference to a coordinate system.
Suppose an observer looks along an arbitrary axis in the direction of increase
and sees flow crossing the axis from left to right. A sign convention is
adopted such that the flow velocity is positive.
*** Flow in Cartesian coordinates[edit] ***
By observing the flow into an elemental square in an x-y Cartesian_coordinate
system, we have:
         &#x03B4; &#x03C8; = u &#x03B4; y    {\displaystyle \delta \psi
      =u\delta y\,}  [\delta \psi =u\delta y\,]
         &#x03B4; &#x03C8; = &#x2212; v &#x03B4; x    {\displaystyle \delta
      \psi =-v\delta x\,}  [\delta \psi =-v\delta x\,]
where u is the flow velocity parallel to and in the direction of the x-axis,
and v is the flow velocity parallel to and in the direction of the y-axis.
Thus, as Î´n â 0 and by rearranging, we have:
         u =    &#x2202; &#x03C8;   &#x2202; y       {\displaystyle u={\frac
      {\partial \psi }{\partial y}}\,}  [u={\frac  {\partial \psi }{\partial
      y}}\,]
         v = &#x2212;    &#x2202; &#x03C8;   &#x2202; x       {\displaystyle
      v=-{\frac {\partial \psi }{\partial x}}\,}  [v=-{\frac  {\partial \psi }
      {\partial x}}\,]
**** Continuity: the derivation[edit] ****
Consider two-dimensional plane flow within a Cartesian coordinate system.
Continuity states that if we consider incompressible flow into an elemental
square, the flow into that small element must equal the flow out of that
element.
The total flow into the element is given by:
         &#x03B4;  &#x03C8;  i n   = u &#x03B4; y + v &#x03B4; x .
      {\displaystyle \delta \psi _{in}=u\delta y+v\delta x.\,}  [\delta \psi _{
      {in}}=u\delta y+v\delta x.\,]
The total flow out of the element is given by:
         &#x03B4;  &#x03C8;  o u t   =  (  u +    &#x2202; u   &#x2202; x
      &#x03B4; x  )  &#x03B4; y +  (  v +    &#x2202; v   &#x2202; y
      &#x03B4; y  )  &#x03B4; x .    {\displaystyle \delta \psi _{out}=\left(u+
      {\frac {\partial u}{\partial x}}\delta x\right)\delta y+\left(v+{\frac
      {\partial v}{\partial y}}\delta y\right)\delta x.\,}  [\delta \psi _{
      {out}}=\left(u+{\frac  {\partial u}{\partial x}}\delta x\right)\delta
      y+\left(v+{\frac  {\partial v}{\partial y}}\delta y\right)\delta x.\,]
Thus we have:
         &#x03B4;  &#x03C8;  i n   = &#x03B4;  &#x03C8;  o u t
      {\displaystyle \delta \psi _{in}=\delta \psi _{out}\,}  [\delta \psi _{
      {in}}=\delta \psi _{{out}}\,]
         u &#x03B4; y + v &#x03B4; x &#xA0; =  (  u +    &#x2202; u   &#x2202;
      x    &#x03B4; x  )  &#x03B4; y +  (  v +    &#x2202; v   &#x2202; y
      &#x03B4; y  )  &#x03B4; x    {\displaystyle u\delta y+v\delta x\ =\left
      (u+{\frac {\partial u}{\partial x}}\delta x\right)\delta y+\left(v+{\frac
      {\partial v}{\partial y}}\delta y\right)\delta x\,}  [u\delta y+v\delta
      x\ =\left(u+{\frac  {\partial u}{\partial x}}\delta x\right)\delta
      y+\left(v+{\frac  {\partial v}{\partial y}}\delta y\right)\delta x\,]
and simplifying to:
            &#x2202; u   &#x2202; x    +    &#x2202; v   &#x2202; y    = 0.
      {\displaystyle {\frac {\partial u}{\partial x}}+{\frac {\partial v}
      {\partial y}}=0.}  [{\frac  {\partial u}{\partial x}}+{\frac  {\partial
      v}{\partial y}}=0.]
Substituting the expressions of the stream function into this equation, we
have:
             &#x2202;  2   &#x03C8;   &#x2202; x &#x2202; y    &#x2212;
      &#x2202;  2   &#x03C8;   &#x2202; y &#x2202; x    = 0.   {\displaystyle
      {\frac {\partial ^{2}\psi }{\partial x\partial y}}-{\frac {\partial ^
      {2}\psi }{\partial y\partial x}}=0.}  [{\frac  {\partial ^{2}\psi }
      {\partial x\partial y}}-{\frac  {\partial ^{2}\psi }{\partial y\partial
      x}}=0.]
**** Vorticity[edit] ****
See also: Vorticity
The stream function can be found from vorticity using the following Poisson's
equation:
          &#x2207;  2   &#x03C8; = &#x2212; &#x03C9;   {\displaystyle \nabla ^
      {2}\psi =-\omega }  [\nabla ^{2}\psi =-\omega ]
or
          &#x2207;  2    &#x03C8; &#x2032;  = + &#x03C9;   {\displaystyle
      \nabla ^{2}\psi '=+\omega }  [\nabla ^{2}\psi '=+\omega ]
where the vorticity vector      &#x03C9;  = &#x2207; &#x00D7;  u
{\displaystyle {\boldsymbol {\omega }}=\nabla \times \mathbf {u} }  [
{\boldsymbol  {\omega }}=\nabla \times {\mathbf  {u}}] â defined as the curl
of the flow velocity vector      u    {\displaystyle \mathbf {u} }  [\mathbf
{u} ] â for this two-dimensional flow has      &#x03C9;  = ( 0 , 0 , &#x03C9;
) ,   {\displaystyle {\boldsymbol {\omega }}=(0,0,\omega ),}  [{\boldsymbol
{\omega }}=(0,0,\omega ),] i.e. only the     z   {\displaystyle z}  [z]-
component     &#x03C9;   {\displaystyle \omega }  [\omega ] can be non-zero.
*** Proof that a constant value for the stream function corresponds to a
streamline[edit] ***
Consider two-dimensional plane flow within a Cartesian coordinate system.
Consider two infinitesimally close points     P = ( x , y )   {\displaystyle P=
(x,y)}  [P=(x,y)] and     Q = ( x + d x , y + d y )   {\displaystyle Q=
(x+dx,y+dy)}  [Q=(x+dx,y+dy)]. From calculus we have that
         &#x03C8; ( x + d x , y + d y ) &#x2212; &#x03C8; ( x , y ) =
      &#x2202; &#x03C8;   &#x2202; x    d x +    &#x2202; &#x03C8;   &#x2202; y
      d y   {\displaystyle \psi (x+dx,y+dy)-\psi (x,y)={\partial \psi \over
      \partial x}dx+{\partial \psi \over \partial y}dy}  [\psi (x+dx,y+dy)-\psi
      (x,y)={\partial \psi  \over \partial x}dx+{\partial \psi  \over \partial
      y}dy]
           = &#x2207; &#x03C8; &#x22C5; d  r    {\displaystyle \qquad \qquad
      =\nabla \psi \cdot d{\boldsymbol {r}}}  [\qquad \qquad =\nabla \psi \cdot
      d{\boldsymbol  {r}}]
Say     &#x03C8;   {\displaystyle \psi }  [\psi ] takes the same value, say
C   {\displaystyle C}  [C], at the two points     P   {\displaystyle P}  [P]
and     Q   {\displaystyle Q}  [Q], then     d  r    {\displaystyle d
{\boldsymbol {r}}}  [d{\boldsymbol  {r}}] is tangent to the curve     &#x03C8;
= C   {\displaystyle \psi =C}  [\psi =C] at     P   {\displaystyle P}  [P] and
         0 = &#x03C8; ( x + d x , y + d y ) &#x2212; &#x03C8; ( x , y ) =
      &#x2207; &#x03C8; &#x22C5; d  r    {\displaystyle 0=\psi (x+dx,y+dy)-\psi
      (x,y)=\nabla \psi \cdot d{\boldsymbol {r}}}  [0=\psi (x+dx,y+dy)-\psi
      (x,y)=\nabla \psi \cdot d{\boldsymbol  {r}}]
implying that the vector     &#x2207; &#x03C8;   {\displaystyle \nabla \psi }
[\nabla \psi] is normal to the curve     &#x03C8; = C   {\displaystyle \psi =C}
[\psi =C]. If we can show that everywhere      u  &#x22C5; &#x2207; &#x03C8; =
0   {\displaystyle {\boldsymbol {u}}\cdot \nabla \psi =0}  [{\boldsymbol
{u}}\cdot \nabla \psi =0], using the formula for      u    {\displaystyle
{\boldsymbol {u}}}  [\boldsymbol{u}] in terms of     &#x03C8;   {\displaystyle
\psi }  [\psi ], then we will have proved the result. This easily follows,
          u  &#x22C5; &#x2207; &#x03C8; =    &#x2202; &#x03C8;   &#x2202; y
      &#x2202; &#x03C8;   &#x2202; x    +   (   &#x2212;    &#x2202; &#x03C8;
      &#x2202; x      )      &#x2202; &#x03C8;   &#x2202; y    = 0.
      {\displaystyle {\boldsymbol {u}}\cdot \nabla \psi ={\partial \psi \over
      \partial y}{\partial \psi \over \partial x}+{\Big (}-{\partial \psi \over
      \partial x}{\Big )}{\partial \psi \over \partial y}=0.}  [{\boldsymbol
      {u}}\cdot \nabla \psi ={\partial \psi  \over \partial y}{\partial \psi
      \over \partial x}+{\Big (}-{\partial \psi  \over \partial x}{\Big )}
      {\partial \psi  \over \partial y}=0.]
*** Properties of the stream function[edit] ***
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (August 2017)(Learn_how_and_when_to_remove_this_template_message)
   1. The stream function     &#x03C8;   {\displaystyle \psi }  [\psi ] is
      constant along any streamline.
   2. For a continuous flow (no sources or sinks), the volume flow rate across
      any closed path is equal to zero.
   3. For two incompressible flow patterns, the algebraic sum of the stream
      functions is equal to another stream function obtained if the two flow
      patterns are super-imposed.
   4. The rate of change of stream function with distance is directly
      proportional to the velocity component perpendicular to the direction of
      change.
***** References[edit] *****
**** Citations[edit] ****
   1. ^Lagrange,_J.-L. (1868), "MÃ©moire sur la thÃ©orie du mouvement des
      fluides (in: Nouveaux MÃ©moires de l'AcadÃ©mie Royale des Sciences et
      Belles-Lettres de Berlin, annÃ©e 1781)", Oevres_de_Lagrange, Tome IV,
      pp. 695â748
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
   3. ^Stokes,_G.G. (1842), "On the steady motion of incompressible fluids",
      Transactions of the Cambridge Philosophical Society, 7: 439â453,
      Bibcode:1848TCaPS...7..439S
   4.
      Reprinted in:Stokes, G.G. (1880), Mathematical_and_Physical_Papers,
      Volume_I, Cambridge University Press, pp. 1â16
   5. ^ Lamb_(1932, pp. 62â63) and Batchelor_(1967, pp. 75â79)
**** Sources[edit] ****
    * Batchelor,_G._K. (1967), An Introduction to Fluid Dynamics, Cambridge
      University Press, ISBN 0-521-09817-3
Lamb,_H. (1932), Hydrodynamics (6th ed.), Cambridge University Press,
republished by Dover Publications, ISBN 0-486-60256-7
Massey, B. S.; Ward-Smith, J. (1998), Mechanics of Fluids (7th ed.), UK: Nelson
Thornes
White, F. M. (2003), Fluid Mechanics (5th ed.), New York: McGraw-Hill
Gamelin, T. W. (2001), Complex Analysis, New York: Springer, ISBN 0-387-95093-1
"Streamfunction", AMS Glossary of Meteorology, American_Meteorological_Society,
retrieved 2014-01-30
***** External links[edit] *****
    * Joukowsky_Transform_Interactive_WebApp

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Stream_function&oldid=881779967"
Categories:
    * Continuum_mechanics
    * Fluid_dynamics
Hidden categories:
    * CS1:_long_volume_value
    * Articles_needing_additional_references_from_August_2017
    * All_articles_needing_additional_references
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
    * Deutsch
    * FranÃ§ais
    * æ¥æ¬èª
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 4 February 2019, at 19:37 (UTC).
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
