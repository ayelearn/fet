The following text has been accessed from https://en.wikipedia.org/wiki/Potential_flow at Thu Aug 8 23:37:05 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Potential flow ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For potential flow around a cylinder, see Potential_flow_around_a_circular
cylinder.
Potential-flow streamlines around a NACA_0012_airfoil at 11Â° angle_of_attack,
with upper and lower streamtubes identified.
In fluid_dynamics, potential flow describes the velocity_field as the gradient
of a scalar function: the velocity_potential. As a result, a potential flow is
characterized by an irrotational_velocity_field, which is a valid approximation
for several applications. The irrotationality of a potential flow is due to the
curl of the gradient of a scalar always being equal to zero.
In the case of an incompressible_flow the velocity potential satisfies
Laplace's_equation, and potential_theory is applicable. However, potential
flows also have been used to describe compressible_flows. The potential flow
approach occurs in the modeling of both stationary as well as nonstationary
flows. Applications of potential flow are for instance: the outer flow field
for aerofoils, water_waves, electroosmotic_flow, and groundwater_flow. For
flows (or parts thereof) with strong vorticity effects, the potential flow
approximation is not applicable.
⁰
***** Contents *****
    * 1_Characteristics_and_applications
          o 1.1_Description_and_characteristics
          o 1.2_Incompressible_flow
          o 1.3_Compressible_flow
                # 1.3.1_Steady_flow
                # 1.3.2_Sound_waves
          o 1.4_Applicability_and_limitations
    * 2_Analysis_for_two-dimensional_flow
    * 3_Examples_of_two-dimensional_flows
          o 3.1_Power_laws
                # 3.1.1_Power_laws_with_n_=_1:_uniform_flow
                # 3.1.2_Power_laws_with_n_=_2
                # 3.1.3_Power_laws_with_n_=_3
                # 3.1.4_Power_laws_with_n_=_â1:_doublet
                # 3.1.5_Power_laws_with_n_=_â2:_quadrupole
          o 3.2_Line_source_and_sink
          o 3.3_Line_vortex
    * 4_Analysis_for_three-dimensional_flow
          o 4.1_Point_source_and_sink
    * 5_See_also
    * 6_Notes
    * 7_References
    * 8_Further_reading
    * 9_External_links
***** Characteristics and applications[edit] *****
A potential flow is constructed by adding simple elementary flows and observing
the result.
Streamlines for the incompressible potential_flow_around_a_circular_cylinder in
a uniform onflow.
**** Description and characteristics[edit] ****
In fluid dynamics, a potential flow is described by means of a velocity
potential Ï, being a function of space and time. The flow_velocity v is a
vector_field equal to the gradient, â, of the velocity potential Ï:[1]
          v  = &#x2207; &#x03C6; .   {\displaystyle \mathbf {v} =\nabla \varphi
      .}  [{\mathbf  {v}}=\nabla \varphi .]
Sometimes, also the definition v = ââÏ, with a minus sign, is used. But
here we will use the definition above, without the minus sign. From vector
calculus it is known that the curl_of_a_gradient is equal to zero:[1]
         &#x2207; &#x00D7; &#x2207; &#x03C6; =  0   ,   {\displaystyle \nabla
      \times \nabla \varphi =\mathbf {0} \,,}  [{\displaystyle \nabla \times
      \nabla \varphi =\mathbf {0} \,,}]
and consequently the vorticity, the curl of the velocity field v, is zero:[1]
         &#x2207; &#x00D7;  v  =  0   .   {\displaystyle \nabla \times \mathbf
      {v} =\mathbf {0} \,.}  [{\displaystyle \nabla \times \mathbf {v} =\mathbf
      {0} \,.}]
This implies that a potential flow is an irrotational_flow. This has direct
consequences for the applicability of potential flow. In flow regions where
vorticity is known to be important, such as wakes and boundary_layers,
potential flow theory is not able to provide reasonable predictions of the
flow.[2] Fortunately, there are often large regions of a flow where the
assumption of irrotationality is valid which is why potential flow is used for
various applications. For instance in: flow around aircraft, groundwater_flow,
acoustics, water_waves, and electroosmotic_flow.[3]
**** Incompressible flow[edit] ****
In case of an incompressible_flow â for instance of a liquid, or a gas at low
Mach_numbers; but not for sound waves â the velocity v has zero divergence:
[1]
         &#x2207; &#x22C5;  v  = 0  ,   {\displaystyle \nabla \cdot \mathbf {v}
      =0\,,}  [{\displaystyle \nabla \cdot \mathbf {v} =0\,,}]
with the dot denoting the inner_product. As a result, the velocity potential Ï
has to satisfy Laplace's_equation[1]
          &#x2207;  2   &#x03C6; = 0  ,   {\displaystyle \nabla ^{2}\varphi
      =0\,,}  [{\displaystyle \nabla ^{2}\varphi =0\,,}]
where â2 = â â â is the Laplace_operator (sometimes also written Î).
In this case the flow can be determined completely from its kinematics: the
assumptions of irrotationality and zero divergence of flow. Dynamics only have
to be applied afterwards, if one is interested in computing pressures: for
instance for flow around airfoils through the use of Bernoulli's_principle.
In two dimensions, potential flow reduces to a very simple system that is
analyzed using complex_analysis (see below).
**** Compressible flow[edit] ****
*** Steady flow[edit] ***
Potential flow theory can also be used to model irrotational compressible flow.
The full potential equation, describing a steady_flow, is given by:[4]
          (  1 &#x2212;  M  x   2    )      &#x2202;  2   &#x03A6;   &#x2202;
      x  2      +  (  1 &#x2212;  M  y   2    )      &#x2202;  2   &#x03A6;
      &#x2202;  y  2      +  (  1 &#x2212;  M  z   2    )      &#x2202;  2
      &#x03A6;   &#x2202;  z  2      &#x2212; 2  M  x    M  y       &#x2202;  2
      &#x03A6;   &#x2202; x  &#x2202; y    &#x2212; 2  M  y    M  z
      &#x2202;  2   &#x03A6;   &#x2202; y  &#x2202; z    &#x2212; 2  M  z    M
      x       &#x2202;  2   &#x03A6;   &#x2202; z  &#x2202; x    = 0  ,
      {\displaystyle \left(1-M_{x}^{2}\right){\frac {\partial ^{2}\Phi }
      {\partial x^{2}}}+\left(1-M_{y}^{2}\right){\frac {\partial ^{2}\Phi }
      {\partial y^{2}}}+\left(1-M_{z}^{2}\right){\frac {\partial ^{2}\Phi }
      {\partial z^{2}}}-2M_{x}M_{y}{\frac {\partial ^{2}\Phi }{\partial
      x\,\partial y}}-2M_{y}M_{z}{\frac {\partial ^{2}\Phi }{\partial
      y\,\partial z}}-2M_{z}M_{x}{\frac {\partial ^{2}\Phi }{\partial
      z\,\partial x}}=0\,,}  [{\displaystyle \left(1-M_{x}^{2}\right){\frac
      {\partial ^{2}\Phi }{\partial x^{2}}}+\left(1-M_{y}^{2}\right){\frac
      {\partial ^{2}\Phi }{\partial y^{2}}}+\left(1-M_{z}^{2}\right){\frac
      {\partial ^{2}\Phi }{\partial z^{2}}}-2M_{x}M_{y}{\frac {\partial ^
      {2}\Phi }{\partial x\,\partial y}}-2M_{y}M_{z}{\frac {\partial ^{2}\Phi }
      {\partial y\,\partial z}}-2M_{z}M_{x}{\frac {\partial ^{2}\Phi }{\partial
      z\,\partial x}}=0\,,}]
with Mach_number components
          M  x   =   1 a      &#x2202; &#x03A6;   &#x2202; x     ,   M  y   =
      1 a      &#x2202; &#x03A6;   &#x2202; y     ,   and    M  z   =   1 a
      &#x2202; &#x03A6;   &#x2202; z     ,   {\displaystyle M_{x}={\frac {1}
      {a}}{\frac {\partial \Phi }{\partial x}}\,,\qquad M_{y}={\frac {1}{a}}
      {\frac {\partial \Phi }{\partial y}}\,,\qquad {\text{and}}\qquad M_{z}=
      {\frac {1}{a}}{\frac {\partial \Phi }{\partial z}}\,,}  [{\displaystyle
      M_{x}={\frac {1}{a}}{\frac {\partial \Phi }{\partial x}}\,,\qquad M_{y}=
      {\frac {1}{a}}{\frac {\partial \Phi }{\partial y}}\,,\qquad {\text
      {and}}\qquad M_{z}={\frac {1}{a}}{\frac {\partial \Phi }{\partial
      z}}\,,}]
where a is the local speed_of_sound. The flow velocity v is again equal to
âÎ¦, with Î¦ the velocity potential. The full potential equation is valid for
sub-, trans- and supersonic_flow at arbitrary angle_of_attack, as long as the
assumption of irrotationality is applicable.[4]
In case of either subsonic or supersonic (but not transonic or hypersonic)
flow, at small angles of attack and thin bodies, an additional assumption can
be made: the velocity potential is split into an undisturbed onflow velocity
Vâ in the x-direction, and a small perturbation velocity âÏ thereof. So:
[4]
         &#x2207; &#x03A6; =  V  &#x221E;   x + &#x2207; &#x03C6;  .
      {\displaystyle \nabla \Phi =V_{\infty }x+\nabla \varphi \,.}  [
      {\displaystyle \nabla \Phi =V_{\infty }x+\nabla \varphi \,.}]
In that case, the linearized small-perturbation potential equation â an
approximation to the full potential equation â can be used:[4]
          (  1 &#x2212;  M  &#x221E;   2    )      &#x2202;  2   &#x03C6;
      &#x2202;  x  2      +     &#x2202;  2   &#x03C6;   &#x2202;  y  2      +
      &#x2202;  2   &#x03C6;   &#x2202;  z  2      = 0 ,   {\displaystyle \left
      (1-M_{\infty }^{2}\right){\frac {\partial ^{2}\varphi }{\partial x^{2}}}+
      {\frac {\partial ^{2}\varphi }{\partial y^{2}}}+{\frac {\partial ^
      {2}\varphi }{\partial z^{2}}}=0,}  [\left(1-M_{\infty }^{2}\right){\frac
      {\partial ^{2}\varphi }{\partial x^{2}}}+{\frac  {\partial ^{2}\varphi }
      {\partial y^{2}}}+{\frac  {\partial ^{2}\varphi }{\partial z^{2}}}=0,]
with Mâ = Vâ/aâ the Mach number of the incoming free stream. This linear
equation is much easier to solve than the full potential equation: it may be
recast into Laplace's equation by a simple coordinate stretching in the x-
direction.
      Derivation of the full potential equation
      For a steady inviscid flow, the Euler_equations â for the mass and
      momentum density â are, in subscript notation and in non-conservation
      form:[5]
                     &#x2202;  &#x2202;  x  i       (  &#x03C1;   v  i    )     =
            0  ,     &#x03C1;   v  j       &#x2202;  v  i     &#x2202;  x  j
            = &#x2212;    &#x2202; p   &#x2202;  x  i       ,
            {\displaystyle {\begin{aligned}{\frac {\partial }{\partial x_
            {i}}}\left(\rho \,v_{i}\right)&=0\,,\\\rho \,v_{j}\,{\frac {\partial
            v_{i}}{\partial x_{j}}}&=-{\frac {\partial p}{\partial x_{i}}}\,,\end
            {aligned}}}  [{\displaystyle {\begin{aligned}{\frac {\partial }
            {\partial x_{i}}}\left(\rho \,v_{i}\right)&=0\,,\\\rho \,v_{j}\,
            {\frac {\partial v_{i}}{\partial x_{j}}}&=-{\frac {\partial p}
            {\partial x_{i}}}\,,\end{aligned}}}]
      while using the summation_convention: since j occurs more than once in the
      term on the left hand side of the momentum equation, j is summed over all
      its components (which is from 1 to 2 in two-dimensional flow, and from 1 to
      3 in three dimensions). Further:
          * Ï is the fluid density,
          * p is the pressure,
          * (x1, x2, x3) = (x, y, z) are the coordinates and
          * (v1, v2, v3) are the corresponding components of the velocity vector
            v.
      The speed of sound squared a2 is equal to the derivative of the pressure p
      with respect to the density Ï, at constant entropy S:[6]
                a  2   =   [    &#x2202; p   &#x2202; &#x03C1;    ]   S   .
            {\displaystyle a^{2}=\left[{\frac {\partial p}{\partial \rho
            }}\right]_{S}.}  [a^{2}=\left[{\frac  {\partial p}{\partial \rho
            }}\right]_{S}.]
      As a result, the flow equations can be written as:
                v  i       &#x2202; &#x03C1;   &#x2202;  x  i      + &#x03C1;
            &#x2202;  v  i     &#x2202;  x  i      = 0   and   &#x03C1;   v  j
            &#x2202;  v  i     &#x2202;  x  j      = &#x2212;  a  2
            &#x2202; &#x03C1;   &#x2202;  x  i       .   {\displaystyle v_{i}\,
            {\frac {\partial \rho }{\partial x_{i}}}+\rho \,{\frac {\partial v_
            {i}}{\partial x_{i}}}=0\qquad {\text{and}}\qquad \rho \,v_{j}\,{\frac
            {\partial v_{i}}{\partial x_{j}}}=-a^{2}\,{\frac {\partial \rho }
            {\partial x_{i}}}\,.}  [{\displaystyle v_{i}\,{\frac {\partial \rho }
            {\partial x_{i}}}+\rho \,{\frac {\partial v_{i}}{\partial x_
            {i}}}=0\qquad {\text{and}}\qquad \rho \,v_{j}\,{\frac {\partial v_
            {i}}{\partial x_{j}}}=-a^{2}\,{\frac {\partial \rho }{\partial x_
            {i}}}\,.}]
      Multiplying (and summing) the momentum equation with vi, and using the mass
      equation to eliminate the density gradient gives:
               &#x03C1;   v  i     v  j       &#x2202;  v  i     &#x2202;  x  j
            = &#x03C1;   a  2       &#x2202;  v  i     &#x2202;  x  i       .
            {\displaystyle \rho \,v_{i}\,v_{j}\,{\frac {\partial v_{i}}{\partial
            x_{j}}}=\rho \,a^{2}\,{\frac {\partial v_{i}}{\partial x_{i}}}\,.}  [
            {\displaystyle \rho \,v_{i}\,v_{j}\,{\frac {\partial v_{i}}{\partial
            x_{j}}}=\rho \,a^{2}\,{\frac {\partial v_{i}}{\partial x_{i}}}\,.}]
      When divided by Ï, and with all terms on one side of the equation, the
      compressible flow equation is:
                  &#x2202;  v  i     &#x2202;  x  i      &#x2212;     v  i     v
            j     a  2        &#x2202;  v  i     &#x2202;  x  j      = 0  .
            {\displaystyle {\frac {\partial v_{i}}{\partial x_{i}}}-{\frac {v_
            {i}\,v_{j}}{a^{2}}}{\frac {\partial v_{i}}{\partial x_{j}}}=0\,.}  [
            {\displaystyle {\frac {\partial v_{i}}{\partial x_{i}}}-{\frac {v_
            {i}\,v_{j}}{a^{2}}}{\frac {\partial v_{i}}{\partial x_{j}}}=0\,.}]
      Note that until this stage, no assumptions have been made regarding the
      flow (besides that it is a steady_flow).
      Now, for irrotational flow the velocity v is the gradient of the velocity
      potential Î¦, and the local Mach number components Mi are defined as:
                v  i   =    &#x2202; &#x03A6;   &#x2202;  x  i        and    M  i
            =    v  i   a   =   1 a      &#x2202; &#x03A6;   &#x2202;  x  i
            .   {\displaystyle v_{i}={\frac {\partial \Phi }{\partial x_
            {i}}}\qquad {\text{and}}\qquad M_{i}={\frac {v_{i}}{a}}={\frac {1}
            {a}}{\frac {\partial \Phi }{\partial x_{i}}}\,.}  [{\displaystyle v_
            {i}={\frac {\partial \Phi }{\partial x_{i}}}\qquad {\text{and}}\qquad
            M_{i}={\frac {v_{i}}{a}}={\frac {1}{a}}{\frac {\partial \Phi }
            {\partial x_{i}}}\,.}]
      When used in the flow equation, the full potential equation results:
                   &#x2202;  2   &#x03A6;   &#x2202;  x  i    &#x2202;  x  i
            &#x2212;  M  i     M  j        &#x2202;  2   &#x03A6;   &#x2202;  x
            i    &#x2202;  x  j      = 0  .   {\displaystyle {\frac {\partial ^
            {2}\Phi }{\partial x_{i}\,\partial x_{i}}}-M_{i}\,M_{j}\,{\frac
            {\partial ^{2}\Phi }{\partial x_{i}\,\partial x_{j}}}=0\,.}  [
            {\displaystyle {\frac {\partial ^{2}\Phi }{\partial x_{i}\,\partial
            x_{i}}}-M_{i}\,M_{j}\,{\frac {\partial ^{2}\Phi }{\partial x_
            {i}\,\partial x_{j}}}=0\,.}]
      Written out in components, the form given at the beginning of this section
      is obtained. When a specific equation_of_state is provided, relating
      pressure p and density Ï, the speed of sound can be determined.
      Subsequently, together with adequate boundary conditions, the full
      potential equation can be solved (most often through the use of a
      computational_fluid_dynamics code).
*** Sound waves[edit] ***
Main articles: Sound, Acoustics, and Wave_equation
Small-amplitude sound waves can be approximated with the following potential-
flow model:[7]
             &#x2202;  2   &#x03C6;   &#x2202;  t  2      =    a &#x00AF;    2
      &#x0394; &#x03C6; ,   {\displaystyle {\frac {\partial ^{2}\varphi }
      {\partial t^{2}}}={\overline {a}}^{2}\Delta \varphi ,}  [\frac{\partial^2
      \varphi}{\partial t^2} = \overline{a}^2 \Delta \varphi,]
which is a linear wave_equation for the velocity potential Ï. Again the
oscillatory part of the velocity vector v is related to the velocity potential
by v = âÏ, while as before Î is the Laplace_operator, and Ä is the average
speed of sound in the homogeneous_medium. Note that also the oscillatory parts
of the pressure p and density Ï each individually satisfy the wave equation,
in this approximation.
**** Applicability and limitations[edit] ****
Potential flow does not include all the characteristics of flows that are
encountered in the real world. Potential flow theory cannot be applied for
viscous internal_flows.[2] Richard_Feynman considered potential flow to be so
unphysical that the only fluid to obey the assumptions was "dry water" (quoting
John von Neumann).[8] Incompressible potential flow also makes a number of
invalid predictions, such as d'Alembert's_paradox, which states that the drag
on any object moving through an infinite fluid otherwise at rest is zero.[9]
More precisely, potential flow cannot account for the behaviour of flows that
include a boundary_layer.[2] Nevertheless, understanding potential flow is
important in many branches of fluid mechanics. In particular, simple potential
flows (called elementary_flows) such as the free_vortex and the point_source
possess ready analytical solutions. These solutions can be superposed to create
more complex flows satisfying a variety of boundary conditions. These flows
correspond closely to real-life flows over the whole of fluid mechanics; in
addition, many valuable insights arise when considering the deviation (often
slight) between an observed flow and the corresponding potential flow.
Potential flow finds many applications in fields such as aircraft design. For
instance, in computational_fluid_dynamics, one technique is to couple a
potential flow solution outside the boundary_layer to a solution of the
boundary_layer_equations inside the boundary layer. The absence of boundary
layer effects means that any streamline can be replaced by a solid boundary
with no change in the flow field, a technique used in many aerodynamic design
approaches. Another technique would be the use of Riabouchinsky_solids.[dubious
– discuss]
***** Analysis for two-dimensional flow[edit] *****
Main article: Conformal_map
Potential flow in two dimensions is simple to analyze using conformal_mapping,
by the use of transformations of the complex_plane. However, use of complex
numbers is not required, as for example in the classical analysis of fluid flow
past a cylinder. It is not possible to solve a potential flow using complex
numbers in three dimensions.[10]
The basic idea is to use a holomorphic (also called analytic) or meromorphic
function f, which maps the physical domain (x, y) to the transformed domain
(Ï, Ï). While x, y, Ï and Ï are all real_valued, it is convenient to define
the complex quantities
         z = x + i y   and   w = &#x03C6; + i &#x03C8;  .   {\displaystyle
      z=x+iy\qquad {\text{and}}\qquad w=\varphi +i\psi \,.}  [{\displaystyle
      z=x+iy\qquad {\text{and}}\qquad w=\varphi +i\psi \,.}]
Now, if we write the mapping f as[10]
         f ( x + i y ) = &#x03C6; + i &#x03C8;   or   f ( z ) = w  .
      {\displaystyle f(x+iy)=\varphi +i\psi \qquad {\text{or}}\qquad f(z)=w\,.}
      [{\displaystyle f(x+iy)=\varphi +i\psi \qquad {\text{or}}\qquad f
      (z)=w\,.}]
Then, because f is a holomorphic or meromorphic function, it has to satisfy the
CauchyâRiemann_equations[10]
            &#x2202; &#x03C6;   &#x2202; x    =    &#x2202; &#x03C8;   &#x2202;
      y     ,     &#x2202; &#x03C6;   &#x2202; y    = &#x2212;    &#x2202;
      &#x03C8;   &#x2202; x     .   {\displaystyle {\frac {\partial \varphi }
      {\partial x}}={\frac {\partial \psi }{\partial y}}\,,\qquad {\frac
      {\partial \varphi }{\partial y}}=-{\frac {\partial \psi }{\partial
      x}}\,.}  [{\displaystyle {\frac {\partial \varphi }{\partial x}}={\frac
      {\partial \psi }{\partial y}}\,,\qquad {\frac {\partial \varphi }
      {\partial y}}=-{\frac {\partial \psi }{\partial x}}\,.}]
The velocity components (u, v), in the (x, y) directions respectively, can be
obtained directly from f by differentiating with respect to z. That is[10]
            d f   d z    = u &#x2212; i v   {\displaystyle {\frac {df}{dz}}=u-
      iv}  [{\frac  {df}{dz}}=u-iv]
So the velocity field v = (u, v) is specified by[10]
         u =    &#x2202; &#x03C6;   &#x2202; x    =    &#x2202; &#x03C8;
      &#x2202; y    ,  v =    &#x2202; &#x03C6;   &#x2202; y    = &#x2212;
      &#x2202; &#x03C8;   &#x2202; x     .   {\displaystyle u={\frac {\partial
      \varphi }{\partial x}}={\frac {\partial \psi }{\partial y}},\qquad v=
      {\frac {\partial \varphi }{\partial y}}=-{\frac {\partial \psi }{\partial
      x}}\,.}  [{\displaystyle u={\frac {\partial \varphi }{\partial x}}={\frac
      {\partial \psi }{\partial y}},\qquad v={\frac {\partial \varphi }
      {\partial y}}=-{\frac {\partial \psi }{\partial x}}\,.}]
Both Ï and Ï then satisfy Laplace's_equation:[10]
         &#x0394; &#x03C6; =     &#x2202;  2   &#x03C6;   &#x2202;  x  2      +
      &#x2202;  2   &#x03C6;   &#x2202;  y  2      = 0   and   &#x0394;
      &#x03C8; =     &#x2202;  2   &#x03C8;   &#x2202;  x  2      +
      &#x2202;  2   &#x03C8;   &#x2202;  y  2      = 0  .   {\displaystyle
      \Delta \varphi ={\frac {\partial ^{2}\varphi }{\partial x^{2}}}+{\frac
      {\partial ^{2}\varphi }{\partial y^{2}}}=0\qquad {\text{and}}\qquad
      \Delta \psi ={\frac {\partial ^{2}\psi }{\partial x^{2}}}+{\frac
      {\partial ^{2}\psi }{\partial y^{2}}}=0\,.}  [{\displaystyle \Delta
      \varphi ={\frac {\partial ^{2}\varphi }{\partial x^{2}}}+{\frac {\partial
      ^{2}\varphi }{\partial y^{2}}}=0\qquad {\text{and}}\qquad \Delta \psi =
      {\frac {\partial ^{2}\psi }{\partial x^{2}}}+{\frac {\partial ^{2}\psi }
      {\partial y^{2}}}=0\,.}]
So Ï can be identified as the velocity potential and Ï is called the stream
function.[10] Lines of constant Ï are known as streamlines and lines of
constant Ï are known as equipotential lines (see equipotential_surface).
Streamlines and equipotential lines are orthogonal to each other, since[10]
         &#x2207; &#x03C6; &#x22C5; &#x2207; &#x03C8; =    &#x2202; &#x03C6;
      &#x2202; x       &#x2202; &#x03C8;   &#x2202; x    +    &#x2202; &#x03C6;
      &#x2202; y       &#x2202; &#x03C8;   &#x2202; y    =    &#x2202; &#x03C8;
      &#x2202; y       &#x2202; &#x03C8;   &#x2202; x    &#x2212;    &#x2202;
      &#x03C8;   &#x2202; x       &#x2202; &#x03C8;   &#x2202; y    = 0  .
      {\displaystyle \nabla \varphi \cdot \nabla \psi ={\frac {\partial \varphi
      }{\partial x}}{\frac {\partial \psi }{\partial x}}+{\frac {\partial
      \varphi }{\partial y}}{\frac {\partial \psi }{\partial y}}={\frac
      {\partial \psi }{\partial y}}{\frac {\partial \psi }{\partial x}}-{\frac
      {\partial \psi }{\partial x}}{\frac {\partial \psi }{\partial y}}=0\,.}
      [{\displaystyle \nabla \varphi \cdot \nabla \psi ={\frac {\partial
      \varphi }{\partial x}}{\frac {\partial \psi }{\partial x}}+{\frac
      {\partial \varphi }{\partial y}}{\frac {\partial \psi }{\partial y}}=
      {\frac {\partial \psi }{\partial y}}{\frac {\partial \psi }{\partial x}}-
      {\frac {\partial \psi }{\partial x}}{\frac {\partial \psi }{\partial
      y}}=0\,.}]
Thus the flow occurs along the lines of constant Ï and at right angles to the
lines of constant Ï.[10]
ÎÏ = 0 is also satisfied, this relation being equivalent to â Ã v = 0. So
the flow is irrotational. The automatic condition â2Î¨/âx ây = â2Î¨/
ây âx then gives the incompressibility constraint â Â· v = 0.
***** Examples of two-dimensional flows[edit] *****
Main articles: Potential_flow_around_a_circular_cylinder and Rankine_half_body
Any differentiable function may be used for f. The examples that follow use a
variety of elementary_functions; special_functions may also be used. Note that
multi-valued_functions such as the natural_logarithm may be used, but attention
must be confined to a single Riemann_surface.
**** Power laws[edit] ****
[Conformal_power_half.svg]
[Conformal_power_two_third.svg]
[Conformal_power_one.svg]
[Conformal_power_one_and_a_half.svg]
[Conformal_power_two.svg]
[Conformal_power_three.svg]
[Conformal_power_minus_one.svg]
Examples of conformal maps for the power law w = Azn, for different values of
the power n. Shown is the z-plane, showing lines of constant potential Ï and
streamfunction Ï, while w = Ï + iÏ.
In case the following power-law conformal map is applied, from z = x + iy to w
= Ï + iÏ:[11]
         w = A  z  n    ,   {\displaystyle w=Az^{n}\,,}  [{\displaystyle w=Az^
      {n}\,,}]
then, writing z in polar coordinates as z = x + iy = reiÎ¸, we have[11]
         &#x03C6; = A  r  n   cos &#x2061; n &#x03B8;   and   &#x03C8; = A  r
      n   sin &#x2061; n &#x03B8;  .   {\displaystyle \varphi =Ar^{n}\cos
      n\theta \qquad {\text{and}}\qquad \psi =Ar^{n}\sin n\theta \,.}  [
      {\displaystyle \varphi =Ar^{n}\cos n\theta \qquad {\text{and}}\qquad \psi
      =Ar^{n}\sin n\theta \,.}]
In the figures to the right examples are given for several values of n. The
black line is the boundary of the flow, while the darker blue lines are
streamlines, and the lighter blue lines are equi-potential lines. Some
interesting powers n are:[11]
    * n = 1/2: this corresponds with flow around a semi-infinite plate,
    * n = 2/3: flow around a right corner,
    * n = 1: a trivial case of uniform flow,
    * n = 2: flow through a corner, or near a stagnation point, and
    * n = â1: flow due to a source doublet
The constant A is a scaling parameter: its absolute_value |A| determines the
scale, while its argument arg(A) introduces a rotation (if non-zero).
*** Power laws with n = 1: uniform flow[edit] ***
If w = Az1, that is, a power law with n = 1, the streamlines (i.e. lines of
constant Ï) are a system of straight lines parallel to the x-axis. This is
easiest to see by writing in terms of real and imaginary components:
         f ( x + i y ) = A  ( x + i y ) = A x + i A y   {\displaystyle f
      (x+iy)=A\,(x+iy)=Ax+iAy}  [{\displaystyle f(x+iy)=A\,(x+iy)=Ax+iAy}]
thus giving Ï = Ax and Ï = Ay. This flow may be interpreted as uniform flow
parallel to the x-axis.
*** Power laws with n = 2[edit] ***
If n = 2, then w = Az2 and the streamline corresponding to a particular value
of Ï are those points satisfying
         &#x03C8; = A  r  2   sin &#x2061; 2 &#x03B8;  ,   {\displaystyle \psi
      =Ar^{2}\sin 2\theta \,,}  [{\displaystyle \psi =Ar^{2}\sin 2\theta \,,}]
which is a system of rectangular_hyperbolae. This may be seen by again
rewriting in terms of real and imaginary components. Noting that sin_2Î¸_=_2
sin_Î¸_cos_Î¸ and rewriting sin Î¸ = y/r and cos Î¸ = x/r it is seen (on
simplifying) that the streamlines are given by
         &#x03C8; = 2 A x y  .   {\displaystyle \psi =2Axy\,.}  [{\displaystyle
      \psi =2Axy\,.}]
The velocity field is given by âÏ, or
           (    u     v    )   =   (       &#x2202; &#x03C6;   &#x2202; x
      &#x2202; &#x03C6;   &#x2202; y       )   =   (    +    &#x2202; &#x03C8;
      &#x2202; y        &#x2212;    &#x2202; &#x03C8;   &#x2202; x       )   =
      (    + 2 A x     &#x2212; 2 A y    )    .   {\displaystyle {\begin
      {pmatrix}u\\v\end{pmatrix}}={\begin{pmatrix}{\frac {\partial \varphi }
      {\partial x}}\\[2px]{\frac {\partial \varphi }{\partial y}}\end
      {pmatrix}}={\begin{pmatrix}+{\partial \psi \over \partial y}\\[2px]-
      {\partial \psi \over \partial x}\end{pmatrix}}={\begin{pmatrix}+2Ax\\
      [2px]-2Ay\end{pmatrix}}\,.}  [{\displaystyle {\begin{pmatrix}u\\v\end
      {pmatrix}}={\begin{pmatrix}{\frac {\partial \varphi }{\partial x}}\\[2px]
      {\frac {\partial \varphi }{\partial y}}\end{pmatrix}}={\begin{pmatrix}+
      {\partial \psi  \over \partial y}\\[2px]-{\partial \psi  \over \partial
      x}\end{pmatrix}}={\begin{pmatrix}+2Ax\\[2px]-2Ay\end{pmatrix}}\,.}]
In fluid dynamics, the flowfield near the origin corresponds to a stagnation
point. Note that the fluid at the origin is at rest (this follows on
differentiation of f(z) = z2 at z = 0). The Ï = 0 streamline is particularly
interesting: it has two (or four) branches, following the coordinate axes, i.e.
x = 0 and y = 0. As no fluid flows across the x-axis, it (the x-axis) may be
treated as a solid boundary. It is thus possible to ignore the flow in the
lower half-plane where y < 0 and to focus on the flow in the upper halfplane.
With this interpretation, the flow is that of a vertically directed jet
impinging on a horizontal flat plate. The flow may also be interpreted as flow
into a 90 degree corner if the regions specified by (say) x, y < 0 are ignored.
*** Power laws with n = 3[edit] ***
If n = 3, the resulting flow is a sort of hexagonal version of the n = 2 case
considered above. Streamlines are given by, Ï = 3x2y â y3 and the flow in
this case may be interpreted as flow into a 60Â° corner.
*** Power laws with n = â1: doublet[edit] ***
If n = â1, the streamlines are given by
         &#x03C8; = &#x2212;   A r   sin &#x2061; &#x03B8; .   {\displaystyle
      \psi =-{\frac {A}{r}}\sin \theta .}  [\psi =-{\frac  {A}{r}}\sin \theta
      .]
This is more easily interpreted in terms of real and imaginary components:
         &#x03C8; =    &#x2212; A y   r  2     =    &#x2212; A y    x  2   +  y
      2       ,   {\displaystyle \psi ={\frac {-Ay}{r^{2}}}={\frac {-Ay}{x^
      {2}+y^{2}}}\,,}  [{\displaystyle \psi ={\frac {-Ay}{r^{2}}}={\frac {-Ay}
      {x^{2}+y^{2}}}\,,}]
          x  2   +  y  2   +    A y  &#x03C8;   = 0  ,   {\displaystyle x^
      {2}+y^{2}+{\frac {Ay}{\psi }}=0\,,}  [{\displaystyle x^{2}+y^{2}+{\frac
      {Ay}{\psi }}=0\,,}]
          x  2   +   (  y +   A  2 &#x03C8;     )   2   =   (   A  2 &#x03C8;
      )   2    .   {\displaystyle x^{2}+\left(y+{\frac {A}{2\psi }}\right)^
      {2}=\left({\frac {A}{2\psi }}\right)^{2}\,.}  [{\displaystyle x^{2}+\left
      (y+{\frac {A}{2\psi }}\right)^{2}=\left({\frac {A}{2\psi }}\right)^
      {2}\,.}]
Thus the streamlines are circles that are tangent to the x-axis at the origin.
The circles in the upper half-plane thus flow clockwise, those in the lower
half-plane flow anticlockwise. Note that the velocity components are
proportional to râ2; and their values at the origin is infinite. This flow
pattern is usually referred to as a doublet, or dipole, and can be interpreted
as the combination of a source-sink pair of infinite strength kept an
infinitesimally small distance apart. The velocity field is given by
         ( u , v ) =  (     &#x2202; &#x03C8;   &#x2202; y    , &#x2212;
      &#x2202; &#x03C8;   &#x2202; x     )  =  (  A     y  2   &#x2212;  x  2
      (   x  2   +  y  2    )   2     , &#x2212; A    2 x y    (   x  2   +  y
      2    )   2      )   .   {\displaystyle (u,v)=\left({\frac {\partial \psi
      }{\partial y}},-{\frac {\partial \psi }{\partial x}}\right)=\left(A{\frac
      {y^{2}-x^{2}}{\left(x^{2}+y^{2}\right)^{2}}},-A{\frac {2xy}{\left(x^
      {2}+y^{2}\right)^{2}}}\right)\,.}  [{\displaystyle (u,v)=\left({\frac
      {\partial \psi }{\partial y}},-{\frac {\partial \psi }{\partial
      x}}\right)=\left(A{\frac {y^{2}-x^{2}}{\left(x^{2}+y^{2}\right)^{2}}},-A
      {\frac {2xy}{\left(x^{2}+y^{2}\right)^{2}}}\right)\,.}]
or in polar coordinates:
         (  u  r   ,  u  &#x03B8;   ) =  (    1 r      &#x2202; &#x03C8;
      &#x2202; &#x03B8;    , &#x2212;    &#x2202; &#x03C8;   &#x2202; r     )
      =  (  &#x2212;   A  r  2     cos &#x2061; &#x03B8; , &#x2212;   A  r  2
      sin &#x2061; &#x03B8;  )   .   {\displaystyle (u_{r},u_{\theta })=\left(
      {\frac {1}{r}}{\frac {\partial \psi }{\partial \theta }},-{\frac
      {\partial \psi }{\partial r}}\right)=\left(-{\frac {A}{r^{2}}}\cos \theta
      ,-{\frac {A}{r^{2}}}\sin \theta \right)\,.}  [{\displaystyle (u_{r},u_
      {\theta })=\left({\frac {1}{r}}{\frac {\partial \psi }{\partial \theta
      }},-{\frac {\partial \psi }{\partial r}}\right)=\left(-{\frac {A}{r^
      {2}}}\cos \theta ,-{\frac {A}{r^{2}}}\sin \theta \right)\,.}]
*** Power laws with n = â2: quadrupole[edit] ***
If n = â2, the streamlines are given by
         &#x03C8; = &#x2212;   A  r  2     sin &#x2061; 2 &#x03B8;  .
      {\displaystyle \psi =-{\frac {A}{r^{2}}}\sin 2\theta \,.}  [
      {\displaystyle \psi =-{\frac {A}{r^{2}}}\sin 2\theta \,.}]
This is the flow field associated with a quadrupole.[12]
**** Line source and sink[edit] ****
A line source or sink of strength     Q   {\displaystyle Q}  [Q] (    Q > 0
{\displaystyle Q>0}  [Q>0] for source and     Q < 0   {\displaystyle Q<0}  [
{\displaystyle Q<0}] for sink) is given by the potential
         w =   Q  2 &#x03C0;    ln &#x2061; z   {\displaystyle w={\frac {Q}
      {2\pi }}\ln z}  [{\displaystyle w={\frac {Q}{2\pi }}\ln z}]
where     Q   {\displaystyle Q}  [Q] in fact is the volume flux per unit length
across an surface enclosing the source or sink. The velocity field in polar
coordinates are
          u  r   =   Q  2 &#x03C0; r    ,   u  &#x03B8;   = 0   {\displaystyle
      u_{r}={\frac {Q}{2\pi r}},\quad u_{\theta }=0}  [{\displaystyle u_{r}=
      {\frac {Q}{2\pi r}},\quad u_{\theta }=0}]
i.e., a purely radial flow.
**** Line vortex[edit] ****
A line vortex of strength     &#x0393;   {\displaystyle \Gamma }  [\Gamma ] is
given by
         w =   &#x0393;  2 &#x03C0; i    ln &#x2061; z   {\displaystyle w=
      {\frac {\Gamma }{2\pi i}}\ln z}  [{\displaystyle w={\frac {\Gamma }{2\pi
      i}}\ln z}]
where     &#x0393;   {\displaystyle \Gamma }  [\Gamma ] is the circulation
around any simple closed contour enclosing the vortex. The velocity field in
polar coordinates are
          u  r   = 0 ,   u  &#x03B8;   =   &#x0393;  2 &#x03C0; r
      {\displaystyle u_{r}=0,\quad u_{\theta }={\frac {\Gamma }{2\pi r}}}  [
      {\displaystyle u_{r}=0,\quad u_{\theta }={\frac {\Gamma }{2\pi r}}}]
i.e., a purely azimuthal flow.
***** Analysis for three-dimensional flow[edit] *****
For three-dimensional flows, complex potential cannot be obtained.
**** Point source and sink[edit] ****
The velocity potential of a point source or sink of strength     Q
{\displaystyle Q}  [Q] (    Q > 0   {\displaystyle Q>0}  [Q>0] for source and
Q < 0   {\displaystyle Q<0}  [{\displaystyle Q<0}] for sink) in spherical polar
coordinates is given by
         &#x03D5; = &#x2212;   Q  4 &#x03C0; r      {\displaystyle \phi =-
      {\frac {Q}{4\pi r}}}  [{\displaystyle \phi =-{\frac {Q}{4\pi r}}}]
where     Q   {\displaystyle Q}  [Q] in fact is the volume flux across a closed
surface enclosing the source or sink.

***** See also[edit] *****
    * Potential_flow_around_a_circular_cylinder
    * Aerodynamic_potential-flow_code
    * Conformal_mapping
    * Darwin_drift
    * Flownet
    * Laplacian_field
    * Potential_theory
    * Stream_function
    * Velocity_potential
***** Notes[edit] *****
   1. ^ a b c d e Batchelor (1973) pp. 99â101.
   2. ^ a b c Batchelor (1973) pp. 378â380.
   3. ^Kirby, B.J. (2010), Micro-_and_Nanoscale_Fluid_Mechanics:_Transport_in
      Microfluidic_Devices., Cambridge University Press, ISBN 978-0-521-11903-0
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
   5. ^ a b c dAnderson,_J._D. (2002). Modern compressible flow. McGraw-Hill.
      p. 358â359. ISBN 0-07-242443-5.
   6. ^ Lamb (1994) Â§6âÂ§7, pp. 3â6.
   7. ^ Batchelor (1973) p. 161.
   8. ^ Lamb (1994) Â§287, pp. 492â495.
   9. ^Feynman,_R._P.; Leighton,_R._B.; Sands,_M. (1964), The_Feynman_Lectures
      on_Physics, 2, Addison-Wesley
  10. , p. 40-3. Chapter 40 has the title: The flow of dry water.
  11. ^ Batchelor (1973) pp. 404â405.
  12. ^ a b c d e f g h i Batchelor (1973) pp. 106â108.
  13. ^ a b c Batchelor (1973) pp. 409â413.
  14. ^Kyrala, A. (1972). Applied Functions of a Complex Variable. Wiley-
      Interscience. pp. 116â117. ISBN 9780471511298.
***** References[edit] *****
    * Batchelor,_G.K. (1973), An introduction to fluid dynamics, Cambridge
      University Press, ISBN 0-521-09817-3
Chanson,_H. (2009), Applied_Hydrodynamics:_An_Introduction_to_Ideal_and_Real
Fluid_Flows, CRC Press, Taylor & Francis Group, Leiden, The Netherlands, 478
pages, ISBN 978-0-415-49271-3
Lamb,_H. (1994) [1932], Hydrodynamics (6th ed.), Cambridge University Press,
ISBN 978-0-521-45868-9
Milne-Thomson,_L.M. (1996) [1968], Theoretical hydrodynamics (5th ed.), Dover,
ISBN 0-486-68970-0
***** Further reading[edit] *****
    * Chanson,_H. (2007), "Le_potentiel_de_vitesse_pour_les_Ã©coulements_de
      fluides_rÃ©els:_la_contribution_de_Joseph-Louis_Lagrange_[Velocity
      potential_in_real_fluid_flows:_Joseph-Louis_Lagrange's_contribution]", La
      Houille Blanche (in French) (5): 127â131, doi:10.1051/lhb:2007072
Wehausen,_J.V.; Laitone, E.V. (1960), "Surface waves", in FlÃ¼gge,_S.;
Truesdell,_C. (eds.), Encyclopedia_of_Physics, IX, Springer Verlag,
pp. 446â778
***** External links[edit] *****
 Wikimedia Commons has media related to Potential_flow.
    * "Irrotational_flow_of_an_inviscid_fluid". University_of_Genoa, Faculty of
      Engineering. Retrieved 2009-03-29.
"Conformal_Maps_Gallery". 3D-XplorMath. Retrieved 2009-03-29.
 â Java applets for exploring conformal maps
Joukowsky_Transform_Interactive_WebApp

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Potential_flow&oldid=907446551"
Categories:
    * Fluid_dynamics
Hidden categories:
    * All_accuracy_disputes
    * Articles_with_disputed_statements_from_March_2009
    * CS1_French-language_sources_(fr)
    * Commons_category_link_from_Wikidata
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * FranÃ§ais
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * ä¸­æ
Edit_links
    * This page was last edited on 22 July 2019, at 23:35 (UTC).
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
