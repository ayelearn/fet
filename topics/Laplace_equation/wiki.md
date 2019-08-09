The following text has been accessed from https://en.wikipedia.org/wiki/Laplace%27s_equation at Fri Aug 9 00:03:11 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Laplace's equation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Second order partial differential equation
For Laplace's tidal equations, see Theory_of_tides_Â§ Laplace's_tidal
equations.
In mathematics, Laplace's equation is a second-order partial_differential
equation named after Pierre-Simon_Laplace who first studied its properties.
This is often written as
          &#x2207;  2   f = 0    or    &#x0394; f = 0 ,   {\displaystyle \nabla
      ^{2}f=0\qquad {\mbox{or}}\qquad \Delta f=0,}  [{\displaystyle \nabla ^
      {2}f=0\qquad {\mbox{or}}\qquad \Delta f=0,}]
where     &#x0394; = &#x2207; &#x22C5; &#x2207; =  &#x2207;  2
{\displaystyle \Delta =\nabla \cdot \nabla =\nabla ^{2}}  [{\displaystyle
\Delta =\nabla \cdot \nabla =\nabla ^{2}}]is the Laplace_operator,[note_1]
&#x2207; &#x22C5;   {\displaystyle \nabla \cdot }  [\nabla \cdot] is divergence
operator (also symbolized "div"),     &#x2207;   {\displaystyle \nabla }
[\nabla ] is the gradient operator (also symbolized "grad"), and     f ( x , y
, z )   {\displaystyle f(x,y,z)}  [{\displaystyle f(x,y,z)}] is a twice-
differentiable real-valued function. The Laplace operator therefore maps a
scalar function to another scalar function.
If the right-hand side is specified as a given function,     h ( x , y , z )
{\displaystyle h(x,y,z)}  [{\displaystyle h(x,y,z)}], we have
         &#x0394; f = h .   {\displaystyle \Delta f=h.}  [{\displaystyle \Delta
      f=h.}]
This is called Poisson's_equation, a generalization of Laplace's equation,
Laplace's and Poisson's equation are the simplest examples of elliptic_partial
differential_equations.
The Laplace equation is also a special case of the Helmholtz_equation.
The general theory of solutions to Laplace's equation is known as potential
theory. The solutions of Laplace's equation are the harmonic_functions,[1]
which are important in branches of physics, notably electrostatics,
gravitation, and fluid_dynamics. In the study of heat_conduction, the Laplace
equation is the steady-state heat_equation.[2]
⁰
***** Contents *****
    * 1_Forms_in_different_coordinate_systems
    * 2_Boundary_conditions
    * 3_In_two_dimensions
          o 3.1_Analytic_functions
          o 3.2_Fluid_flow
          o 3.3_Electrostatics
    * 4_In_three_dimensions
          o 4.1_Fundamental_solution
          o 4.2_Green's_function
          o 4.3_Electrostatics
    * 5_In_the_Schwarzschild_metric
    * 6_See_also
    * 7_Notes
    * 8_References
    * 9_Further_reading
    * 10_External_links
***** Forms in different coordinate systems[edit] *****
In Cartesian_coordinates,[3]
         &#x0394; f =     &#x2202;  2   f   &#x2202;  x  2      +     &#x2202;
      2   f   &#x2202;  y  2      +     &#x2202;  2   f   &#x2202;  z  2      =
      0.   {\displaystyle \Delta f={\frac {\partial ^{2}f}{\partial x^{2}}}+
      {\frac {\partial ^{2}f}{\partial y^{2}}}+{\frac {\partial ^{2}f}{\partial
      z^{2}}}=0.}  [{\displaystyle \Delta f={\frac {\partial ^{2}f}{\partial x^
      {2}}}+{\frac {\partial ^{2}f}{\partial y^{2}}}+{\frac {\partial ^{2}f}
      {\partial z^{2}}}=0.}]
In cylindrical_coordinates,[3]
         &#x0394; f =   1 r     &#x2202;  &#x2202; r     (  r    &#x2202; f
      &#x2202; r     )  +   1  r  2         &#x2202;  2   f   &#x2202;
      &#x03D5;  2      +     &#x2202;  2   f   &#x2202;  z  2      = 0.
      {\displaystyle \Delta f={\frac {1}{r}}{\frac {\partial }{\partial
      r}}\left(r{\frac {\partial f}{\partial r}}\right)+{\frac {1}{r^{2}}}
      {\frac {\partial ^{2}f}{\partial \phi ^{2}}}+{\frac {\partial ^{2}f}
      {\partial z^{2}}}=0.}  [{\displaystyle \Delta f={\frac {1}{r}}{\frac
      {\partial }{\partial r}}\left(r{\frac {\partial f}{\partial r}}\right)+
      {\frac {1}{r^{2}}}{\frac {\partial ^{2}f}{\partial \phi ^{2}}}+{\frac
      {\partial ^{2}f}{\partial z^{2}}}=0.}]
In spherical_coordinates, using the     ( r , &#x03B8; , &#x03C6; )
{\displaystyle (r,\theta ,\varphi )}  [{\displaystyle (r,\theta ,\varphi
)}]convention,[3]
         &#x0394; f =   1  r  2       &#x2202;  &#x2202; r     (   r  2
      &#x2202; f   &#x2202; r     )  +   1   r  2   sin &#x2061; &#x03B8;
      &#x2202;  &#x2202; &#x03B8;     (  sin &#x2061; &#x03B8;    &#x2202; f
      &#x2202; &#x03B8;     )  +   1   r  2    sin  2   &#x2061; &#x03B8;
      &#x2202;  2   f   &#x2202;  &#x03C6;  2      = 0.   {\displaystyle \Delta
      f={\frac {1}{r^{2}}}{\frac {\partial }{\partial r}}\left(r^{2}{\frac
      {\partial f}{\partial r}}\right)+{\frac {1}{r^{2}\sin \theta }}{\frac
      {\partial }{\partial \theta }}\left(\sin \theta {\frac {\partial f}
      {\partial \theta }}\right)+{\frac {1}{r^{2}\sin ^{2}\theta }}{\frac
      {\partial ^{2}f}{\partial \varphi ^{2}}}=0.}  [{\displaystyle \Delta f=
      {\frac {1}{r^{2}}}{\frac {\partial }{\partial r}}\left(r^{2}{\frac
      {\partial f}{\partial r}}\right)+{\frac {1}{r^{2}\sin \theta }}{\frac
      {\partial }{\partial \theta }}\left(\sin \theta {\frac {\partial f}
      {\partial \theta }}\right)+{\frac {1}{r^{2}\sin ^{2}\theta }}{\frac
      {\partial ^{2}f}{\partial \varphi ^{2}}}=0.}]
More generally, in curvilinear_coordinates,
         &#x0394; f =   &#x2202;  &#x2202;  &#x03BE;  j       (     &#x2202; f
      &#x2202;  &#x03BE;  k       g  k j    )  +    &#x2202; f   &#x2202;
      &#x03BE;  j       g  j m    &#x0393;  m n   n   = 0 ,   {\displaystyle
      \Delta f={\frac {\partial }{\partial \xi ^{j}}}\left({\frac {\partial f}
      {\partial \xi ^{k}}}g^{kj}\right)+{\frac {\partial f}{\partial \xi ^
      {j}}}g^{jm}\Gamma _{mn}^{n}=0,}  [\Delta f={\frac {\partial }{\partial
      \xi ^{j}}}\left({\frac {\partial f}{\partial \xi ^{k}}}g^{kj}\right)+
      {\frac {\partial f}{\partial \xi ^{j}}}g^{jm}\Gamma _{mn}^{n}=0,]
or
         &#x0394; f =   1   |  g  |       &#x2202;  &#x2202;  &#x03BE;  i
      (     |  g  |     g  i j      &#x2202; f   &#x2202;  &#x03BE;  j       )
      = 0 ,  ( g =  d e t  {  g  i j   } ) .   {\displaystyle \Delta f={\frac
      {1}{\sqrt {|g|}}}{\frac {\partial }{\partial \xi ^{i}}}\!\left({\sqrt
      {|g|}}g^{ij}{\frac {\partial f}{\partial \xi ^{j}}}\right)=0,\qquad
      (g=\mathrm {det} \{g_{ij}\}).}  [\Delta f={\frac {1}{\sqrt {|g|}}}{\frac
      {\partial }{\partial \xi ^{i}}}\!\left({\sqrt {|g|}}g^{ij}{\frac
      {\partial f}{\partial \xi ^{j}}}\right)=0,\qquad (g=\mathrm {det} \{g_
      {ij}\}).]
***** Boundary conditions[edit] *****
Laplace's equation on an annulus (inner radius r = 2 and outer radius R = 4)
with Dirichlet boundary conditions u(r=2) = 0 and u(R=4) = 4 sin(5 Î¸)
See also: Boundary_value_problem
The Dirichlet_problem for Laplace's equation consists of finding a solution Ï
on some domain D such that Ï on the boundary of D is equal to some given
function. Since the Laplace operator appears in the heat_equation, one physical
interpretation of this problem is as follows: fix the temperature on the
boundary of the domain according to the given specification of the boundary
condition. Allow heat to flow until a stationary state is reached in which the
temperature at each point on the domain doesn't change anymore. The temperature
distribution in the interior will then be given by the solution to the
corresponding Dirichlet problem.
The Neumann_boundary_conditions for Laplace's equation specify not the function
Ï itself on the boundary of D, but its normal_derivative. Physically, this
corresponds to the construction of a potential for a vector field whose effect
is known at the boundary of D alone.
Solutions of Laplace's equation are called harmonic_functions; they are all
analytic within the domain where the equation is satisfied. If any two
functions are solutions to Laplace's equation (or any linear homogeneous
differential equation), their sum (or any linear combination) is also a
solution. This property, called the principle_of_superposition, is very useful,
e.g., solutions to complex problems can be constructed by summing simple
solutions.
***** In two dimensions[edit] *****
Laplace's equation in two independent variables in rectangular coordinates has
the form
             &#x2202;  2   &#x03C8;   &#x2202;  x  2      +     &#x2202;  2
      &#x03C8;   &#x2202;  y  2      &#x2261;  &#x03C8;  x x   +  &#x03C8;  y y
      = 0.   {\displaystyle {\frac {\partial ^{2}\psi }{\partial x^{2}}}+{\frac
      {\partial ^{2}\psi }{\partial y^{2}}}\equiv \psi _{xx}+\psi _{yy}=0.}  [
      {\frac {\partial ^{2}\psi }{\partial x^{2}}}+{\frac {\partial ^{2}\psi }
      {\partial y^{2}}}\equiv \psi _{xx}+\psi _{yy}=0.]
**** Analytic functions[edit] ****
The real and imaginary parts of a complex analytic_function both satisfy the
Laplace equation. That is, if z = x + iy, and if
         f ( z ) = u ( x , y ) + i v ( x , y ) ,   {\displaystyle f(z)=u
      (x,y)+iv(x,y),}  [f(z)=u(x,y)+iv(x,y),]
then the necessary condition that f(z) be analytic is that the CauchyâRiemann
equations be satisfied:
          u  x   =  v  y   ,   v  x   = &#x2212;  u  y   .   {\displaystyle u_
      {x}=v_{y},\quad v_{x}=-u_{y}.}  [u_{x}=v_{y},\quad v_{x}=-u_{y}.]
where ux is the first partial derivative of u with respect to x. It follows
that
          u  y y   = ( &#x2212;  v  x    )  y   = &#x2212; (  v  y    )  x   =
      &#x2212; (  u  x    )  x   .   {\displaystyle u_{yy}=(-v_{x})_{y}=-(v_
      {y})_{x}=-(u_{x})_{x}.}  [u_{yy}=(-v_{x})_{y}=-(v_{y})_{x}=-(u_{x})_{x}.]
Therefore u satisfies the Laplace equation. A similar calculation shows that v
also satisfies the Laplace equation. Conversely, given a harmonic function, it
is the real part of an analytic function, f(z) (at least locally). If a trial
form is
         f ( z ) = &#x03C6; ( x , y ) + i &#x03C8; ( x , y ) ,   {\displaystyle
      f(z)=\varphi (x,y)+i\psi (x,y),}  [f(z)=\varphi (x,y)+i\psi (x,y),]
then the CauchyâRiemann equations will be satisfied if we set
          &#x03C8;  x   = &#x2212;  &#x03C6;  y   ,   &#x03C8;  y   =  &#x03C6;
      x   .   {\displaystyle \psi _{x}=-\varphi _{y},\quad \psi _{y}=\varphi _
      {x}.}  [\psi _{x}=-\varphi _{y},\quad \psi _{y}=\varphi _{x}.]
This relation does not determine Ï, but only its increments:
         d &#x03C8; = &#x2212;  &#x03C6;  y    d x +  &#x03C6;  x    d y .
      {\displaystyle d\psi =-\varphi _{y}\,dx+\varphi _{x}\,dy.}  [d\psi =-
      \varphi _{y}\,dx+\varphi _{x}\,dy.]
The Laplace equation for Ï implies that the integrability condition for Ï is
satisfied:
          &#x03C8;  x y   =  &#x03C8;  y x   ,   {\displaystyle \psi _{xy}=\psi
      _{yx},}  [\psi _{xy}=\psi _{yx},]
and thus Ï may be defined by a line integral. The integrability condition and
Stokes'_theorem implies that the value of the line integral connecting two
points is independent of the path. The resulting pair of solutions of the
Laplace equation are called conjugate harmonic functions. This construction is
only valid locally, or provided that the path does not loop around a
singularity. For example, if r and Î¸ are polar coordinates and
         &#x03C6; = log &#x2061; r ,   {\displaystyle \varphi =\log r,}
      [\varphi =\log r,]
then a corresponding analytic function is
         f ( z ) = log &#x2061; z = log &#x2061; r + i &#x03B8; .
      {\displaystyle f(z)=\log z=\log r+i\theta .}  [f(z)=\log z=\log r+i\theta
      .]
However, the angle Î¸ is single-valued only in a region that does not enclose
the origin.
The close connection between the Laplace equation and analytic functions
implies that any solution of the Laplace equation has derivatives of all
orders, and can be expanded in a power series, at least inside a circle that
does not enclose a singularity. This is in sharp contrast to solutions of the
wave_equation, which generally have less regularity.
There is an intimate connection between power series and Fourier_series. If we
expand a function f in a power series inside a circle of radius R, this means
that
         f ( z ) =  &#x2211;  n = 0   &#x221E;    c  n    z  n   ,
      {\displaystyle f(z)=\sum _{n=0}^{\infty }c_{n}z^{n},}  [f(z)=\sum _{n=0}^
      {\infty }c_{n}z^{n},]
with suitably defined coefficients whose real and imaginary parts are given by
          c  n   =  a  n   + i  b  n   .   {\displaystyle c_{n}=a_{n}+ib_{n}.}
      [c_{n}=a_{n}+ib_{n}.]
Therefore
         f ( z ) =  &#x2211;  n = 0   &#x221E;    [   a  n    r  n   cos
      &#x2061; n &#x03B8; &#x2212;  b  n    r  n   sin &#x2061; n &#x03B8;  ]
      + i  &#x2211;  n = 1   &#x221E;    [   a  n    r  n   sin &#x2061; n
      &#x03B8; +  b  n    r  n   cos &#x2061; n &#x03B8;  ]  ,   {\displaystyle
      f(z)=\sum _{n=0}^{\infty }\left[a_{n}r^{n}\cos n\theta -b_{n}r^{n}\sin
      n\theta \right]+i\sum _{n=1}^{\infty }\left[a_{n}r^{n}\sin n\theta +b_
      {n}r^{n}\cos n\theta \right],}  [f(z)=\sum _{n=0}^{\infty }\left[a_{n}r^
      {n}\cos n\theta -b_{n}r^{n}\sin n\theta \right]+i\sum _{n=1}^{\infty
      }\left[a_{n}r^{n}\sin n\theta +b_{n}r^{n}\cos n\theta \right],]
which is a Fourier series for f. These trigonometric functions can themselves
be expanded, using multiple_angle_formulae.
**** Fluid flow[edit] ****
Let the quantities u and v be the horizontal and vertical components of the
velocity field of a steady incompressible, irrotational flow in two dimensions.
The continuity condition for an incompressible flow is that
          u  x   +  v  y   = 0 ,   {\displaystyle u_{x}+v_{y}=0,}  [u_{x}+v_
      {y}=0,]
and the condition that the flow be irrotational is that
         &#x2207; &#x00D7;  V  =  v  x   &#x2212;  u  y   = 0.   {\displaystyle
      \nabla \times \mathbf {V} =v_{x}-u_{y}=0.}  [\nabla \times \mathbf {V}
      =v_{x}-u_{y}=0.]
If we define the differential of a function Ï by
         d &#x03C8; = v d x &#x2212; u d y ,   {\displaystyle d\psi =vdx-udy,}
      [d\psi =vdx-udy,]
then the continuity condition is the integrability condition for this
differential: the resulting function is called the stream_function because it
is constant along flow_lines. The first derivatives of Ï are given by
          &#x03C8;  x   = v ,   &#x03C8;  y   = &#x2212; u ,   {\displaystyle
      \psi _{x}=v,\quad \psi _{y}=-u,}  [\psi _{x}=v,\quad \psi _{y}=-u,]
and the irrotationality condition implies that Ï satisfies the Laplace
equation. The harmonic function Ï that is conjugate to Ï is called the
velocity_potential. The CauchyâRiemann equations imply that
          &#x03C6;  x   = &#x2212; u ,   &#x03C6;  y   = &#x2212; v .
      {\displaystyle \varphi _{x}=-u,\quad \varphi _{y}=-v.}  [\varphi _{x}=-
      u,\quad \varphi _{y}=-v.]
Thus every analytic function corresponds to a steady incompressible,
irrotational fluid flow in the plane. The real part is the velocity potential,
and the imaginary part is the stream function.
**** Electrostatics[edit] ****
According to Maxwell's_equations, an electric field (u, v) in two space
dimensions that is independent of time satisfies
         &#x2207; &#x00D7; ( u , v , 0 ) = (  v  x   &#x2212;  u  y   )     k
      &#x005E;    =  0  ,   {\displaystyle \nabla \times (u,v,0)=(v_{x}-u_{y})
      {\hat {\mathbf {k} }}=\mathbf {0} ,}  [\nabla \times (u,v,0)=(v_{x}-u_
      {y}){\hat {\mathbf {k} }}=\mathbf {0} ,]
and
         &#x2207; &#x22C5; ( u , v ) = &#x03C1; ,   {\displaystyle \nabla \cdot
      (u,v)=\rho ,}  [\nabla \cdot (u,v)=\rho ,]
where Ï is the charge density. The first Maxwell equation is the integrability
condition for the differential
         d &#x03C6; = &#x2212; u  d x &#x2212; v  d y ,   {\displaystyle
      d\varphi =-u\,dx-v\,dy,}  [d\varphi =-u\,dx-v\,dy,]
so the electric potential Ï may be constructed to satisfy
          &#x03C6;  x   = &#x2212; u ,   &#x03C6;  y   = &#x2212; v .
      {\displaystyle \varphi _{x}=-u,\quad \varphi _{y}=-v.}  [\varphi _{x}=-
      u,\quad \varphi _{y}=-v.]
The second of Maxwell's equations then implies that
          &#x03C6;  x x   +  &#x03C6;  y y   = &#x2212; &#x03C1; ,
      {\displaystyle \varphi _{xx}+\varphi _{yy}=-\rho ,}  [\varphi _
      {xx}+\varphi _{yy}=-\rho ,]
which is the Poisson_equation. The Laplace equation can be used in three-
dimensional problems in electrostatics and fluid flow just as in two
dimensions.
***** In three dimensions[edit] *****
**** Fundamental solution[edit] ****
A fundamental_solution of Laplace's equation satisfies
         &#x0394; u =  u  x x   +  u  y y   +  u  z z   = &#x2212; &#x03B4; ( x
      &#x2212;  x &#x2032;  , y &#x2212;  y &#x2032;  , z &#x2212;  z &#x2032;
      ) ,   {\displaystyle \Delta u=u_{xx}+u_{yy}+u_{zz}=-\delta (x-x',y-y',z-
      z'),}  [\Delta u=u_{xx}+u_{yy}+u_{zz}=-\delta (x-x',y-y',z-z'),]
where the Dirac_delta_function Î´ denotes a unit source concentrated at the
point (xâ², yâ², zâ²). No function has this property: in fact it is a
distribution rather than a function; but it can be thought of as a limit of
functions whose integrals over space are unity, and whose support (the region
where the function is non-zero) shrinks to a point (see weak_solution). It is
common to take a different sign convention for this equation than one typically
does when defining fundamental solutions. This choice of sign is often
convenient to work with because âÎ is a positive_operator. The definition of
the fundamental solution thus implies that, if the Laplacian of u is integrated
over any volume that encloses the source point, then
          &#x222D;  V   &#x2207; &#x22C5; &#x2207; u  d V = &#x2212; 1.
      {\displaystyle \iiint _{V}\nabla \cdot \nabla u\,dV=-1.}  [\iiint _
      {V}\nabla \cdot \nabla u\,dV=-1.]
The Laplace equation is unchanged under a rotation of coordinates, and hence we
can expect that a fundamental solution may be obtained among solutions that
only depend upon the distance r from the source point. If we choose the volume
to be a ball of radius a around the source point, then Gauss'_divergence
theorem implies that
         &#x2212; 1 =  &#x222D;  V   &#x2207; &#x22C5; &#x2207; u  d V =
      &#x222C;  S      d u   d r     d S =     4 &#x03C0;  a  2      d u   d r
      |   r = a   .   {\displaystyle -1=\iiint _{V}\nabla \cdot \nabla
      u\,dV=\iint _{S}{\frac {du}{dr}}\,dS=\left.4\pi a^{2}{\frac {du}
      {dr}}\right|_{r=a}.}  [-1=\iiint _{V}\nabla \cdot \nabla u\,dV=\iint _{S}
      {\frac {du}{dr}}\,dS=\left.4\pi a^{2}{\frac {du}{dr}}\right|_{r=a}.]
It follows that
            d u   d r    = &#x2212;   1  4 &#x03C0;  r  2      ,
      {\displaystyle {\frac {du}{dr}}=-{\frac {1}{4\pi r^{2}}},}  [{\frac {du}
      {dr}}=-{\frac {1}{4\pi r^{2}}},]
on a sphere of radius r that is centered on the source point, and hence
         u =   1  4 &#x03C0; r    .   {\displaystyle u={\frac {1}{4\pi r}}.}
      [u={\frac {1}{4\pi r}}.]
Note that, with the opposite sign convention (used in physics), this is the
potential generated by a point_particle, for an inverse-square_law force,
arising in the solution of Poisson_equation. A similar argument shows that in
two dimensions
         u = &#x2212;    log &#x2061; ( r )   2 &#x03C0;    .   {\displaystyle
      u=-{\frac {\log(r)}{2\pi }}.}  [u=-{\frac {\log(r)}{2\pi }}.]
where log(r) denotes the natural_logarithm. Note that, with the opposite sign
convention, this is the potential generated by a pointlike sink (see point
particle), which is the solution of the Euler_equations in two-dimensional
incompressible_flow.
**** Green's function[edit] ****
A Green's_function is a fundamental solution that also satisfies a suitable
condition on the boundary S of a volume V. For instance,
         G ( x , y , z ;  x &#x2032;  ,  y &#x2032;  ,  z &#x2032;  )
      {\displaystyle G(x,y,z;x',y',z')}  [G(x,y,z;x',y',z')]
may satisfy
         &#x2207; &#x22C5; &#x2207; G = &#x2212; &#x03B4; ( x &#x2212;  x
      &#x2032;  , y &#x2212;  y &#x2032;  , z &#x2212;  z &#x2032;  )
      in&#xA0;   V ,   {\displaystyle \nabla \cdot \nabla G=-\delta (x-x',y-
      y',z-z')\qquad {\hbox{in }}V,}  [\nabla \cdot \nabla G=-\delta (x-x',y-
      y',z-z')\qquad {\hbox{in }}V,]
         G = 0    if    ( x , y , z )    on&#xA0;   S .   {\displaystyle
      G=0\quad {\hbox{if}}\quad (x,y,z)\qquad {\hbox{on }}S.}  [G=0\quad {\hbox
      {if}}\quad (x,y,z)\qquad {\hbox{on }}S.]
Now if u is any solution of the Poisson equation in V:
         &#x2207; &#x22C5; &#x2207; u = &#x2212; f ,   {\displaystyle \nabla
      \cdot \nabla u=-f,}  [\nabla \cdot \nabla u=-f,]
and u assumes the boundary values g on S, then we may apply Green's_identity,
(a consequence of the divergence theorem) which states that
          &#x222D;  V    [  G  &#x2207; &#x22C5; &#x2207; u &#x2212; u
      &#x2207; &#x22C5; &#x2207; G  ]   d V =  &#x222D;  V   &#x2207; &#x22C5;
      [  G &#x2207; u &#x2212; u &#x2207; G  ]   d V =  &#x222C;  S    [  G  u
      n   &#x2212; u  G  n    ]   d S .    {\displaystyle \iiint _{V}\left
      [G\,\nabla \cdot \nabla u-u\,\nabla \cdot \nabla G\right]\,dV=\iiint _
      {V}\nabla \cdot \left[G\nabla u-u\nabla G\right]\,dV=\iint _{S}\left[Gu_
      {n}-uG_{n}\right]\,dS.\,}  [\iiint _{V}\left[G\,\nabla \cdot \nabla u-
      u\,\nabla \cdot \nabla G\right]\,dV=\iiint _{V}\nabla \cdot \left[G\nabla
      u-u\nabla G\right]\,dV=\iint _{S}\left[Gu_{n}-uG_{n}\right]\,dS.\,]
The notations un and Gn denote normal derivatives on S. In view of the
conditions satisfied by u and G, this result simplifies to
         u (  x &#x2032;  ,  y &#x2032;  ,  z &#x2032;  ) =  &#x222D;  V   G f
      d V +  &#x222C;  S    G  n   g  d S .    {\displaystyle u
      (x',y',z')=\iiint _{V}Gf\,dV+\iint _{S}G_{n}g\,dS.\,}  [u
      (x',y',z')=\iiint _{V}Gf\,dV+\iint _{S}G_{n}g\,dS.\,]
Thus the Green's function describes the influence at (xâ², yâ², zâ²) of the
data f and g. For the case of the interior of a sphere of radius a, the Green's
function may be obtained by means of a reflection (Sommerfeld_1949): the source
point P at distance Ï from the center of the sphere is reflected along its
radial line to a point P' that is at a distance
          &#x03C1; &#x2032;  =    a  2   &#x03C1;   .    {\displaystyle \rho '=
      {\frac {a^{2}}{\rho }}.\,}  [\rho '={\frac {a^{2}}{\rho }}.\,]
Note that if P is inside the sphere, then P' will be outside the sphere. The
Green's function is then given by
           1  4 &#x03C0; R    &#x2212;   a  4 &#x03C0; &#x03C1;  R &#x2032;
      ,    {\displaystyle {\frac {1}{4\pi R}}-{\frac {a}{4\pi \rho R'}},\,}  [
      {\frac {1}{4\pi R}}-{\frac {a}{4\pi \rho R'}},\,]
where R denotes the distance to the source point P and Râ² denotes the
distance to the reflected point Pâ². A consequence of this expression for the
Green's function is the Poisson_integral_formula. Let Ï, Î¸, and Ï be
spherical_coordinates for the source point P. Here Î¸ denotes the angle with
the vertical axis, which is contrary to the usual American mathematical
notation, but agrees with standard European and physical practice. Then the
solution of the Laplace equation with Dirichlet boundary values g inside the
sphere is given by
         u ( P ) =   1  4 &#x03C0;     a  3    (  1 &#x2212;    &#x03C1;  2
      a  2      )   &#x222B;  0   2 &#x03C0;    &#x222B;  0   &#x03C0;      g
      (  &#x03B8; &#x2032;  ,  &#x03C6; &#x2032;  ) sin &#x2061;  &#x03B8;
      &#x2032;    (  a  2   +  &#x03C1;  2   &#x2212; 2 a &#x03C1; cos &#x2061;
      &#x0398;  )   3 2       d  &#x03B8; &#x2032;   d  &#x03C6; &#x2032;
      {\displaystyle u(P)={\frac {1}{4\pi }}a^{3}\left(1-{\frac {\rho ^{2}}{a^
      {2}}}\right)\int _{0}^{2\pi }\int _{0}^{\pi }{\frac {g(\theta ',\varphi
      ')\sin \theta '}{(a^{2}+\rho ^{2}-2a\rho \cos \Theta )^{\frac {3}
      {2}}}}d\theta '\,d\varphi '}  [{\displaystyle u(P)={\frac {1}{4\pi }}a^
      {3}\left(1-{\frac {\rho ^{2}}{a^{2}}}\right)\int _{0}^{2\pi }\int _{0}^
      {\pi }{\frac {g(\theta ',\varphi ')\sin \theta '}{(a^{2}+\rho ^{2}-2a\rho
      \cos \Theta )^{\frac {3}{2}}}}d\theta '\,d\varphi '}] (Zachmanoglou_1986,
      p. 228)
where
         cos &#x2061; &#x0398; = cos &#x2061; &#x03B8; cos &#x2061;  &#x03B8;
      &#x2032;  + sin &#x2061; &#x03B8; sin &#x2061;  &#x03B8; &#x2032;  cos
      &#x2061; ( &#x03C6; &#x2212;  &#x03C6; &#x2032;  )   {\displaystyle \cos
      \Theta =\cos \theta \cos \theta '+\sin \theta \sin \theta '\cos(\varphi -
      \varphi ')}  [{\displaystyle \cos \Theta =\cos \theta \cos \theta '+\sin
      \theta \sin \theta '\cos(\varphi -\varphi ')}]
is the cosine of the angle between (Î¸, Ï) and (Î¸â², Ïâ²). A simple
consequence of this formula is that if u is a harmonic function, then the value
of u at the center of the sphere is the mean value of its values on the sphere.
This mean value property immediately implies that a non-constant harmonic
function cannot assume its maximum value at an interior point.
**** Electrostatics[edit] ****
Let      E    {\displaystyle \mathbf {E} }  [\mathbf {E} ] be the electric
field,     &#x03C1;   {\displaystyle \rho }  [\rho ] be the electric charge
density, and      &#x03B5;  0     {\displaystyle \varepsilon _{0}}
[\varepsilon _{0}] be the permittivity of free space. Then Gauss's law for
electricity (Maxwell's first equation) in differential form states[4]
   &#x2207; &#x22C5;  E  =   &#x03C1;  &#x03F5;  0     .   {\displaystyle
\nabla \cdot \mathbf {E} ={\frac {\rho }{\epsilon _{0}}}.}  [{\displaystyle
\nabla \cdot \mathbf {E} ={\frac {\rho }{\epsilon _{0}}}.}]
Now, the electric field can be expressed as the negative gradient of the
electric potential     V   {\displaystyle V}  [V],
   E = &#x2212; &#x2207; V ,   {\displaystyle E=-\nabla V,}  [{\displaystyle
E=-\nabla V,}]
if the field is irrotational,     &#x2207; &#x00D7;  E  =  0    {\displaystyle
\nabla \times \mathbf {E} =\mathbf {0} }  [{\displaystyle \nabla \times \mathbf
{E} =\mathbf {0} }]. The irrotationality of      E    {\displaystyle \mathbf
{E} }  [\mathbf {E} ] is also known as the electrostatic condition.[4]
Plugging this relation into Gauss's law, we obtain Poisson's equation for
electricity,[4]
    &#x2207;  2   V = &#x2212;   &#x03C1;  &#x03B5;  0     .   {\displaystyle
\nabla ^{2}V=-{\frac {\rho }{\varepsilon _{0}}}.}  [{\displaystyle \nabla ^
{2}V=-{\frac {\rho }{\varepsilon _{0}}}.}]
In the particular case of a source-free region,     &#x03C1; = 0
{\displaystyle \rho =0}  [\rho =0] and Poisson's equation reduces to Laplace's
equation for the electric potential.[4]
If the electrostatic potential     V   {\displaystyle V}  [V] is specified on
the boundary of a region       R     {\displaystyle {\mathcal {R}}}  [{\mathcal
{R}}], then it is uniquely determined. If       R     {\displaystyle {\mathcal
{R}}}  [{\mathcal {R}}] is surrounded by a conducting material with a specified
charge density     &#x03C1;   {\displaystyle \rho }  [\rho ], and if the total
charge     Q   {\displaystyle Q}  [Q] is known, then     V   {\displaystyle V}
[V] is also unique.[5]
A potential that doesn't satisfy Laplace's equation together with the boundary
condition is an invalid electrostatic potential.
***** In the Schwarzschild metric[edit] *****
S. Persides[6] solved the Laplace equation in Schwarzschild_spacetime on
hypersurfaces of constant t. Using the canonical variables r, Î¸, Ï the
solution is
         &#x03A8; ( r , &#x03B8; , &#x03C6; ) = R ( r )  Y  l   ( &#x03B8; ,
      &#x03C6; ) ,   {\displaystyle \Psi (r,\theta ,\varphi )=R(r)Y_{l}(\theta
      ,\varphi ),}  [{\displaystyle \Psi (r,\theta ,\varphi )=R(r)Y_{l}(\theta
      ,\varphi ),}]
where Yl(Î¸, Ï) is a spherical_harmonic_function, and
         R ( r ) = ( &#x2212; 1  )  l      ( l !  )  2    r  s   l     ( 2 l )
      !     P  l    (  1 &#x2212;    2 r   r  s      )  + ( &#x2212; 1  )  l +
      1      2 ( 2 l + 1 ) !   ( l )  !  2    r  s   l + 1       Q  l    (  1
      &#x2212;    2 r   r  s      )  .   {\displaystyle R(r)=(-1)^{l}{\frac {
      (l!)^{2}r_{s}^{l}}{(2l)!}}P_{l}\left(1-{\frac {2r}{r_{s}}}\right)+(-1)^
      {l+1}{\frac {2(2l+1)!}{(l)!^{2}r_{s}^{l+1}}}Q_{l}\left(1-{\frac {2r}{r_
      {s}}}\right).}  [{\displaystyle R(r)=(-1)^{l}{\frac {(l!)^{2}r_{s}^{l}}{
      (2l)!}}P_{l}\left(1-{\frac {2r}{r_{s}}}\right)+(-1)^{l+1}{\frac {2
      (2l+1)!}{(l)!^{2}r_{s}^{l+1}}}Q_{l}\left(1-{\frac {2r}{r_{s}}}\right).}]
Here Pl and Ql are Legendre_functions of the first and second kind,
respectively, while rs is the Schwarzschild_radius. The parameter l is an
arbitrary non-negative integer.
***** See also[edit] *****
    * 6-sphere_coordinates, a coordinate system under which Laplace's equation
      becomes R-separable
    * Helmholtz_equation, a general case of Laplace's equation.
    * Spherical_harmonic
    * Quadrature_domains
    * Potential_theory
    * Potential_flow
    * Bateman_transform
    * Earnshaw's_theorem uses the Laplace equation to show that stable static
      ferromagnetic suspension is impossible
    * Vector_Laplacian
    * Fundamental_solution
***** Notes[edit] *****
   1. ^ The delta symbol, Î, is also commonly used to represent a finite
      change in some quantity, e.g.     &#x0394; x =  x  1   &#x2212;  x  2
      {\displaystyle \Delta x=x_{1}-x_{2}}  [{\displaystyle \Delta x=x_{1}-x_
      {2}}]. Its use to represent the Laplacian should not be confused with
      this use.
***** References[edit] *****
   1. ^ Stewart, James. Calculus :_Early_Transcendentals. 7th ed., Brooks/Cole,
      Cengage Learning, 2012. Chapter 14: Partial Derivatives. p. 908.
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
   3. ISBN 978-0-538-49790-9.
   4. ^ Zill, Dennis G, and Michael R Cullen. Differential Equations with
      Boundary-Value Problems. 8th edition / ed., Brooks/Cole, Cengage
      Learning, 2013. Chapter 12: Boundary-value Problems in Rectangular
      Coordinates. p. 462.
   5. ISBN 978-1-111-82706-9.
   6. ^ a b c Griffiths, David J. Introduction_to_Electrodynamics. 4th ed.,
      Pearson, 2013. Inner front cover.
   7. ISBN 978-1-108-42041-9.
   8. ^ a b c d Griffiths, David J. Introduction to Electrodynamics. Fourth
      ed., Pearson, 2013. Chapter 2: Electrostatics. p. 83-4.
   9. ISBN 978-1-108-42041-9.
  10. ^ Griffiths, David J. Introduction to Electrodynamics. Fourth ed.,
      Pearson, 2013. Chapter 3: Potentials. p. 119-121.
  11. ISBN 978-1-108-42041-9.
  12. ^Persides, S. (1973). "The Laplace and poisson equations in
      Schwarzschild's space-time". Journal of Mathematical Analysis and
      Applications. 43 (3): 571â578. doi:10.1016/0022-247X(73)90277-1.
***** Further reading[edit] *****
    * Evans, L. C. (1998). Partial Differential Equations. Providence: American
      Mathematical Society. ISBN 978-0-8218-0772-9.
Petrovsky, I. G. (1967). Partial Differential Equations. Philadelphia: W. B.
Saunders.
Polyanin, A. D. (2002). Handbook of Linear Partial Differential Equations for
Engineers and Scientists. Boca Raton: Chapman & Hall/CRC Press. ISBN 978-1-
58488-299-2.
Sommerfeld, A. (1949). Partial Differential Equations in Physics. New York:
Academic Press.
Zachmanoglou, E. C. (1986). Introduction to Partial Differential Equations with
Applications. New York: Dover.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Laplace_equation", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Laplace_Equation_(particular_solutions_and_boundary_value_problems) at EqWorld:
The World of Mathematical Equations.
Example_initial-boundary_value_problems using Laplace's equation from
exampleproblems.com.
Weisstein,_Eric_W. "Laplace's_Equation". MathWorld.
Find_out_how_boundary_value_problems_governed_by_Laplace's_equation_may_be
solved_numerically_by_boundary_element_method

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Laplace%27s_equation&oldid=906969840"
Categories:
    * Elliptic_partial_differential_equations
    * Harmonic_functions
    * Equations
    * Fourier_analysis
    * Pierre-Simon_Laplace
Hidden categories:
    * Use_American_English_from_March_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * CatalÃ 
    * Cymraeg
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
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à°¤à±à°²à±à°à±
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * VÃ¨neto
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 19 July 2019, at 15:07 (UTC).
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
