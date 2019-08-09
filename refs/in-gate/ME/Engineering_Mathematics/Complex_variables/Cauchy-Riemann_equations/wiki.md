The following text has been accessed from https://en.wikipedia.org/wiki/Cauchy%E2%80%93Riemann_equations at Fri Aug 9 03:19:58 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** CauchyâRiemann equations ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Mathematical_analysis â Complex analysis
Complex_analysis
[Gamma_abs_3D.png]
Complex_numbers
    * Real_number
    * Imaginary_number
    * Complex_plane
    * Complex_conjugate
    * Unit_complex_number
Complex_functions
    * Complex-valued_function
    * Analytic_function
    * Holomorphic_function
    * CauchyâRiemann equations
    * Formal_power_series
Basic_Theory
    * Zeros_and_poles
    * Cauchy's_integral_theorem
    * Local_primitive
    * Cauchy's_integral_formula
    * Winding_number
    * Laurent_series
    * Isolated_singularity
    * Residue_theorem
    * Conformal_map
    * Schwarz_lemma
    * Harmonic_function
    * Laplace's_equation
Geometric_function_theory
People
    * Augustin-Louis_Cauchy
    * Leonhard_Euler
    * Carl_Friedrich_Gauss
    * Jacques_Hadamard
    * Kiyoshi_Oka
    * Bernhard_Riemann
    * Karl_Weierstrass
    * [Nuvola_apps_kmplot.svg] Analysis_portal
    * v
    * t
    * e
In the field of complex_analysis in mathematics, the CauchyâRiemann
equations, named after Augustin_Cauchy and Bernhard_Riemann, consist of a
system of two partial_differential_equations which, together with certain
continuity and differentiability criteria, form a necessary and sufficient
condition for a complex_function to be complex_differentiable, that is,
holomorphic. This system of equations first appeared in the work of Jean_le
Rond_d'Alembert (d'Alembert_1752). Later, Leonhard_Euler connected this system
to the analytic_functions (Euler_1797). Cauchy_(1814) then used these equations
to construct his theory of functions. Riemann's dissertation (Riemann_1851) on
the theory of functions appeared in 1851.
The CauchyâRiemann equations on a pair of real-valued functions of two real
variables u(x,y) and v(x,y) are the two equations:
             ( 1 a )       &#x2202; u   &#x2202; x    =    &#x2202; v
      &#x2202; y        ( 1 b )       &#x2202; u   &#x2202; y    = &#x2212;
      &#x2202; v   &#x2202; x          {\displaystyle {\begin{aligned}
      (1a)\qquad &{\frac {\partial u}{\partial x}}={\frac {\partial v}{\partial
      y}}\\[6pt](1b)\qquad &{\frac {\partial u}{\partial y}}=-{\frac {\partial
      v}{\partial x}}\end{aligned}}}  [{\displaystyle {\begin{aligned}
      (1a)\qquad &{\frac {\partial u}{\partial x}}={\frac {\partial v}{\partial
      y}}\\[6pt](1b)\qquad &{\frac {\partial u}{\partial y}}=-{\frac {\partial
      v}{\partial x}}\end{aligned}}}]
Typically u and v are taken to be the real and imaginary_parts respectively of
a complex-valued function of a single complex variable z = x + iy, f(x + iy) =
u(x,y) + iv(x,y). Suppose that u and v are real-differentiable at a point in an
open_subset of â, which can be considered as functions from â2 to â. This
implies that the partial derivatives of u and v exist (although they need not
be continuous) and we can approximate small variations of f linearly. Then f =
u + iv is complex-differentiable at that point if and only if the partial
derivatives of u and v satisfy the CauchyâRiemann equations (1a) and (1b) at
that point. The sole existence of partial derivatives satisfying the
CauchyâRiemann equations is not enough to ensure complex differentiability at
that point. It is necessary that u and v be real differentiable, which is a
stronger condition than the existence of the partial derivatives, but in
general, weaker than continuous differentiability.
Holomorphy is the property of a complex function of being differentiable at
every point of an open and connected subset of â (this is called a domain in
â). Consequently, we can assert that a complex function f, whose real and
imaginary parts u and v are real-differentiable functions, is holomorphic if
and only if, equations (1a) and (1b) are satisfied throughout the domain we are
dealing with. Holomorphic_functions_are_analytic and vice versa. This means
that, in complex analysis, a function that is complex-differentiable in a whole
domain (holomorphic) is the same as an analytic function. This is not true for
real differentiable functions.
⁰
***** Contents *****
    * 1_Simple_example
    * 2_Interpretation_and_reformulation
          o 2.1_Conformal_mappings
          o 2.2_Complex_differentiability
          o 2.3_Independence_of_the_complex_conjugate
          o 2.4_Physical_interpretation
          o 2.5_Harmonic_vector_field
          o 2.6_Preservation_of_complex_structure
          o 2.7_Other_representations
    * 3_Generalizations
          o 3.1_Goursat's_theorem_and_its_generalizations
          o 3.2_Several_variables
          o 3.3_Complex_differential_forms
          o 3.4_BÃ¤cklund_transform
          o 3.5_Definition_in_Clifford_algebra
          o 3.6_Conformal_mappings_in_higher_dimensions
    * 4_See_also
    * 5_References
    * 6_External_links
***** Simple example[edit] *****
Suppose that z = x + iy. The complex-valued function f(z) = z2 is
differentiable at any point z in the complex plane.
         f ( z ) = ( x + i y  )  2   =  x  2   &#x2212;  y  2   + 2 i x y
      {\displaystyle f(z)=(x+iy)^{2}=x^{2}-y^{2}+2ixy}  [{\displaystyle f(z)=
      (x+iy)^{2}=x^{2}-y^{2}+2ixy}]
The real part u(x, y) and the imaginary part v(x, y) of f(z) are
         u ( x , y ) =  x  2   &#x2212;  y  2     {\displaystyle u(x,y)=x^{2}-
      y^{2}}  [{\displaystyle u(x,y)=x^{2}-y^{2}}]
         v ( x , y ) = 2 x y   {\displaystyle v(x,y)=2xy}  [{\displaystyle v
      (x,y)=2xy}]
respectively. The partial derivatives of these are
             &#x2202; u   &#x2202; x     = 2 x   {\displaystyle {\dfrac
      {\partial u}{\partial x}}=2x}  [{\displaystyle {\dfrac {\partial u}
      {\partial x}}=2x}]
             &#x2202; u   &#x2202; y     = &#x2212; 2 y   {\displaystyle
      {\dfrac {\partial u}{\partial y}}=-2y}  [{\displaystyle {\dfrac {\partial
      u}{\partial y}}=-2y}]
             &#x2202; v   &#x2202; x     = 2 y   {\displaystyle {\dfrac
      {\partial v}{\partial x}}=2y}  [{\displaystyle {\dfrac {\partial v}
      {\partial x}}=2y}]
             &#x2202; v   &#x2202; y     = 2 x   {\displaystyle {\dfrac
      {\partial v}{\partial y}}=2x}  [{\displaystyle {\dfrac {\partial v}
      {\partial y}}=2x}].
These partial derivatives have the following relationships:
            &#x2202; u   &#x2202; x    =    &#x2202; v   &#x2202; y
      {\displaystyle {\frac {\partial u}{\partial x}}={\frac {\partial v}
      {\partial y}}}  [{\displaystyle {\frac {\partial u}{\partial x}}={\frac
      {\partial v}{\partial y}}}]
            &#x2202; u   &#x2202; y    = &#x2212;    &#x2202; v   &#x2202; x
      {\displaystyle {\frac {\partial u}{\partial y}}=-{\frac {\partial v}
      {\partial x}}}  [{\displaystyle {\frac {\partial u}{\partial y}}=-{\frac
      {\partial v}{\partial x}}}].
Thus this complex-valued function     f ( z )   {\displaystyle f(z)}  [f(z)]
satisfies the CauchyâRiemann equations (1a) and (1b).
***** Interpretation and reformulation[edit] *****
The equations are one way of looking at the condition on a function to be
differentiable in the sense of complex_analysis: in other words they
encapsulate the notion of function_of_a_complex_variable by means of
conventional differential_calculus. In the theory there are several other major
ways of looking at this notion, and the translation of the condition into other
language is often needed.
**** Conformal mappings[edit] ****
First, the CauchyâRiemann equations may be written in complex form
      (2)         i     &#x2202; f   &#x2202; x      =     &#x2202; f
      &#x2202; y     .   {\displaystyle {i{\dfrac {\partial f}{\partial x}}}=
      {\dfrac {\partial f}{\partial y}}.}  [{i{\dfrac {\partial f}{\partial
      x}}}={\dfrac {\partial f}{\partial y}}.]
In this form, the equations correspond structurally to the condition that the
Jacobian_matrix is of the form
           (    a   &#x2212; b     b     a    )   ,   {\displaystyle {\begin
      {pmatrix}a&-b\\b&\;\;a\end{pmatrix}},}  [{\begin{pmatrix}a&-
      b\\b&\;\;a\end{pmatrix}},]
where     a = &#x2202; u  /  &#x2202; x = &#x2202; v  /  &#x2202; y
{\displaystyle a=\partial u/\partial x=\partial v/\partial y}  [{\displaystyle
a=\partial u/\partial x=\partial v/\partial y}] and     b = &#x2202; v  /
&#x2202; x = &#x2212; &#x2202; u  /  &#x2202; y   {\displaystyle b=\partial v/
\partial x=-\partial u/\partial y}  [{\displaystyle b=\partial v/\partial x=-
\partial u/\partial y}]. A matrix of this form is the matrix_representation_of
a_complex_number. Geometrically, such a matrix is always the composition of a
rotation with a scaling, and in particular preserves angles. The Jacobian of a
function f(z) takes infinitesimal line segments at the intersection of two
curves in z and rotates them to the corresponding segments in f(z).
Consequently, a function satisfying the CauchyâRiemann equations, with a
nonzero derivative, preserves the angle between curves in the plane. That is,
the CauchyâRiemann equations are the conditions for a function to be
conformal.
Moreover, because the composition of a conformal transformation with another
conformal transformation is also conformal, the composition of a solution of
the CauchyâRiemann equations with a conformal map must itself solve the
CauchyâRiemann equations. Thus the CauchyâRiemann equations are conformally
invariant.
**** Complex differentiability[edit] ****
Suppose that
         f ( z ) = u ( z ) + i &#x22C5; v ( z )   {\displaystyle f(z)=u
      (z)+i\cdot v(z)}  [f(z)=u(z)+i\cdot v(z)]
is a function of a complex number z. Then the complex derivative of f at a
point z0 is defined by
          lim    h &#x2192; 0   h &#x2208;  C         f (  z  0   + h )
      &#x2212; f (  z  0   )  h   =  f &#x2032;  (  z  0   )   {\displaystyle
      \lim _{\underset {h\in \mathbb {C} }{h\to 0}}{\frac {f(z_{0}+h)-f(z_{0})}
      {h}}=f'(z_{0})}  [{\displaystyle \lim _{\underset {h\in \mathbb {C} }
      {h\to 0}}{\frac {f(z_{0}+h)-f(z_{0})}{h}}=f'(z_{0})}]
provided this limit exists.
If this limit exists, then it may be computed by taking the limit as h â 0
along the real axis or imaginary axis; in either case it should give the same
result. Approaching along the real axis, one finds
          lim    h &#x2192; 0   h &#x2208;  R         f (  z  0   + h )
      &#x2212; f (  z  0   )  h   =    &#x2202; f   &#x2202; x    (  z  0   ) .
      {\displaystyle \lim _{\underset {h\in \mathbb {R} }{h\to 0}}{\frac {f(z_
      {0}+h)-f(z_{0})}{h}}={\frac {\partial f}{\partial x}}(z_{0}).}  [
      {\displaystyle \lim _{\underset {h\in \mathbb {R} }{h\to 0}}{\frac {f(z_
      {0}+h)-f(z_{0})}{h}}={\frac {\partial f}{\partial x}}(z_{0}).}]
On the other hand, approaching along the imaginary axis,
          lim    h &#x2192; 0   h &#x2208;  R         f (  z  0   + i h )
      &#x2212; f (  z  0   )   i h    =   1 i      &#x2202; f   &#x2202; y
      (  z  0   ) .   {\displaystyle \lim _{\underset {h\in \mathbb {R} }{h\to
      0}}{\frac {f(z_{0}+ih)-f(z_{0})}{ih}}={\frac {1}{i}}{\frac {\partial f}
      {\partial y}}(z_{0}).}  [{\displaystyle \lim _{\underset {h\in \mathbb
      {R} }{h\to 0}}{\frac {f(z_{0}+ih)-f(z_{0})}{ih}}={\frac {1}{i}}{\frac
      {\partial f}{\partial y}}(z_{0}).}]
The equality of the derivative of f taken along the two axis is
         i    &#x2202; f   &#x2202; x    (  z  0   ) =    &#x2202; f   &#x2202;
      y    (  z  0   ) ,   {\displaystyle i{\frac {\partial f}{\partial x}}(z_
      {0})={\frac {\partial f}{\partial y}}(z_{0}),}  [i{\frac {\partial f}
      {\partial x}}(z_{0})={\frac {\partial f}{\partial y}}(z_{0}),]
which are the CauchyâRiemann equations (2) at the point z0.
Conversely, if f : â â â is a function which is differentiable when
regarded as a function on â2, then f is complex differentiable if and only if
the CauchyâRiemann equations hold. In other words, if u and v are real-
differentiable functions of two real variables, obviously u + iv is a (complex-
valued) real-differentiable function, but u + iv is complex-differentiable if
and only if the CauchyâRiemann equations hold.
Indeed, following Rudin_(1966), suppose f is a complex function defined in an
open set Î© â â. Then, writing z = x + iy for every z â Î©, one can also
regard Î© as an open subset of â2, and f as a function of two real variables
x and y, which maps Î© â â2 to â. We consider the CauchyâRiemann
equations at z = z0. So assume f is differentiable at z0, as a function of two
real variables from Î© to â. This is equivalent to the existence of the
following linear approximation
         f (  z  0   + &#x0394; z ) &#x2212; f (  z  0   ) =  f  x    &#x0394;
      x +  f  y    &#x0394; y + &#x03B7; ( &#x0394; z )  &#x0394; z
      {\displaystyle f(z_{0}+\Delta z)-f(z_{0})=f_{x}\,\Delta x+f_{y}\,\Delta
      y+\eta (\Delta z)\,\Delta z\,}  [{\displaystyle f(z_{0}+\Delta z)-f(z_
      {0})=f_{x}\,\Delta x+f_{y}\,\Delta y+\eta (\Delta z)\,\Delta z\,}]
where z = x + iy and Î·(Îz) â 0 as Îz â 0. Since     &#x0394; z +
&#x0394;    z &#x00AF;    = 2  &#x0394; x   {\displaystyle \Delta z+\Delta
{\bar {z}}=2\,\Delta x}  [{\displaystyle \Delta z+\Delta {\bar {z}}=2\,\Delta
x}] and     &#x0394; z &#x2212; &#x0394;    z &#x00AF;    = 2 i  &#x0394; y
{\displaystyle \Delta z-\Delta {\bar {z}}=2i\,\Delta y}  [{\displaystyle \Delta
z-\Delta {\bar {z}}=2i\,\Delta y}], the above can be re-written as
         &#x0394; f (  z  0   ) =     f  x   &#x2212; i  f  y    2    &#x0394;
      z +     f  x   + i  f  y    2    &#x0394;    z &#x00AF;    + &#x03B7;
      ( &#x0394; z )  &#x0394; z    {\displaystyle \Delta f(z_{0})={\frac {f_
      {x}-if_{y}}{2}}\,\Delta z+{\frac {f_{x}+if_{y}}{2}}\,\Delta {\bar
      {z}}+\eta (\Delta z)\,\Delta z\,}  [{\displaystyle \Delta f(z_{0})={\frac
      {f_{x}-if_{y}}{2}}\,\Delta z+{\frac {f_{x}+if_{y}}{2}}\,\Delta {\bar
      {z}}+\eta (\Delta z)\,\Delta z\,}]
Defining the two Wirtinger_derivatives as
           &#x2202;  &#x2202; z    =   1 2     (     &#x2202;  &#x2202; x
      &#x2212; i   &#x2202;  &#x2202; y      )   ,      &#x2202;  &#x2202;    z
      &#x00AF;       =   1 2     (     &#x2202;  &#x2202; x    + i   &#x2202;
      &#x2202; y      )   ,   {\displaystyle {\frac {\partial }{\partial z}}=
      {\frac {1}{2}}{\Bigl (}{\frac {\partial }{\partial x}}-i{\frac {\partial
      }{\partial y}}{\Bigr )},\;\;\;{\frac {\partial }{\partial {\bar {z}}}}=
      {\frac {1}{2}}{\Bigl (}{\frac {\partial }{\partial x}}+i{\frac {\partial
      }{\partial y}}{\Bigr )},}  [{\frac {\partial }{\partial z}}={\frac {1}
      {2}}{\Bigl (}{\frac {\partial }{\partial x}}-i{\frac {\partial }{\partial
      y}}{\Bigr )},\;\;\;{\frac {\partial }{\partial {\bar {z}}}}={\frac {1}
      {2}}{\Bigl (}{\frac {\partial }{\partial x}}+i{\frac {\partial }{\partial
      y}}{\Bigr )},]

in the limit     &#x0394; z &#x2192; 0 , &#x0394;    z &#x00AF;    &#x2192; 0
{\displaystyle \Delta z\rightarrow 0,\Delta {\bar {z}}\rightarrow 0}  [\Delta
z\rightarrow 0,\Delta {\bar {z}}\rightarrow 0] the above equality can be
written as

               d f   d z    |   z =  z  0     =       &#x2202; f   &#x2202; z
      |   z =  z  0     +       &#x2202; f   &#x2202;    z &#x00AF;       |   z
      =  z  0     &#x22C5;    d    z &#x00AF;      d z    + &#x03B7; ( &#x0394;
      z ) ,     ( &#x0394; z &#x2260; 0 ) .   {\displaystyle \left.{\frac {df}
      {dz}}\right|_{z=z_{0}}=\left.{\frac {\partial f}{\partial z}}\right|_
      {z=z_{0}}+\left.{\frac {\partial f}{\partial {\bar {z}}}}\right|_{z=z_
      {0}}\cdot {\frac {d{\bar {z}}}{dz}}+\eta (\Delta z),\;\;\;\;(\Delta z\neq
      0).}  [{\displaystyle \left.{\frac {df}{dz}}\right|_{z=z_{0}}=\left.
      {\frac {\partial f}{\partial z}}\right|_{z=z_{0}}+\left.{\frac {\partial
      f}{\partial {\bar {z}}}}\right|_{z=z_{0}}\cdot {\frac {d{\bar {z}}}
      {dz}}+\eta (\Delta z),\;\;\;\;(\Delta z\neq 0).}]
Now consider the potential values of     d    z &#x00AF;     /  d z
{\displaystyle d{\bar {z}}/dz}  [{\displaystyle d{\bar {z}}/dz}] when the limit
is taken at the origin. For z along the real line,        z &#x00AF;    = z
{\displaystyle {\bar {z}}=z}  [{\displaystyle {\bar {z}}=z}] so that     d    z
&#x00AF;     /  d z = 1   {\displaystyle d{\bar {z}}/dz=1}  [{\displaystyle d
{\bar {z}}/dz=1}]. Similarly for purely imaginary z we have     d    z &#x00AF;
/  d z = &#x2212; 1   {\displaystyle d{\bar {z}}/dz=-1}  [{\displaystyle d{\bar
{z}}/dz=-1}] so that the value of     d    z &#x00AF;     /  d z
{\displaystyle d{\bar {z}}/dz}  [{\displaystyle d{\bar {z}}/dz}] is not well
defined at the origin. It's easy to verify that     d    z &#x00AF;     /  d z
{\displaystyle d{\bar {z}}/dz}  [{\displaystyle d{\bar {z}}/dz}] is not well
defined at any complex z, hence f is complex differentiable at z0 if and only
if     ( &#x2202; f  /  &#x2202;    z &#x00AF;    ) = 0   {\displaystyle
(\partial f/\partial {\bar {z}})=0}  [(\partial f/\partial {\bar {z}})=0] at
z =  z  0     {\displaystyle z=z_{0}}  [z=z_{0}]. But this is exactly the
CauchyâRiemann equations, thus f is differentiable at z0 if and only if the
CauchyâRiemann equations hold at z0.
**** Independence of the complex conjugate[edit] ****
The above proof suggests another interpretation of the CauchyâRiemann
equations. The complex_conjugate of z, denoted        z &#x00AF;
{\displaystyle {\bar {z}}}  [{\bar {z}}], is defined by
            x + i y  &#x00AF;   := x &#x2212; i y   {\displaystyle {\overline
      {x+iy}}:=x-iy}  [{\overline {x+iy}}:=x-iy]
for real x and y. The CauchyâRiemann equations can then be written as a
single equation
      (3)            &#x2202; f   &#x2202;    z &#x00AF;        = 0
      {\displaystyle {\dfrac {\partial f}{\partial {\bar {z}}}}=0}  [{\dfrac
      {\partial f}{\partial {\bar {z}}}}=0]
by using the Wirtinger_derivative_with_respect_to_the_conjugate_variable. In
this form, the CauchyâRiemann equations can be interpreted as the statement
that f is independent of the variable        z &#x00AF;      {\displaystyle
{\bar {z}}}  [{\bar {z}}]. As such, we can view analytic functions as true
functions of one complex variable as opposed to complex functions of two real
variables.
**** Physical interpretation[edit] ****
Contour_plot of a pair u and v satisfying the CauchyâRiemann equations.
Streamlines (v = const, red) are perpendicular to equipotentials (u = const,
blue). The point (0,0) is a stationary point of the potential flow, with six
streamlines meeting, and six equipotentials also meeting and bisecting the
angles formed by the streamlines.
A standard physical interpretation of the CauchyâRiemann equations going back
to Riemann's work on function theory (see Klein_1893) is that u represents a
velocity_potential of an incompressible steady_fluid_flow in the plane, and v
is its stream_function. Suppose that the pair of (twice continuously
differentiable) functions     u , v   {\displaystyle u,v}  [u,v] satisfies the
CauchyâRiemann equations. We will take u to be a velocity potential, meaning
that we imagine a flow of fluid in the plane such that the velocity_vector of
the fluid at each point of the plane is equal to the gradient of u, defined by
         &#x2207; u =    &#x2202; u   &#x2202; x     i  +    &#x2202; u
      &#x2202; y     j    {\displaystyle \nabla u={\frac {\partial u}{\partial
      x}}\mathbf {i} +{\frac {\partial u}{\partial y}}\mathbf {j} }  [\nabla u=
      {\frac {\partial u}{\partial x}}\mathbf {i} +{\frac {\partial u}{\partial
      y}}\mathbf {j} ]
By differentiating the CauchyâRiemann equations a second time, one shows that
u solves Laplace's_equation:
             &#x2202;  2   u   &#x2202;  x  2      +     &#x2202;  2   u
      &#x2202;  y  2      = 0.   {\displaystyle {\frac {\partial ^{2}u}
      {\partial x^{2}}}+{\frac {\partial ^{2}u}{\partial y^{2}}}=0.}  [{\frac
      {\partial ^{2}u}{\partial x^{2}}}+{\frac {\partial ^{2}u}{\partial y^
      {2}}}=0.]
That is, u is a harmonic_function. This means that the divergence of the
gradient is zero, and so the fluid is incompressible.
The function v also satisfies the Laplace equation, by a similar analysis.
Also, the CauchyâRiemann equations imply that the dot_product     &#x2207; u
&#x22C5; &#x2207; v = 0   {\displaystyle \nabla u\cdot \nabla v=0}  [\nabla
u\cdot \nabla v=0]. This implies that the gradient of u must point along the
v =  const    {\displaystyle v={\text{const}}}  [{\displaystyle v={\text
{const}}}] curves; so these are the streamlines of the flow. The     u =  const
{\displaystyle u={\text{const}}}  [{\displaystyle u={\text{const}}}] curves are
the equipotential_curves of the flow.
A holomorphic function can therefore be visualized by plotting the two families
of level_curves     u =  const    {\displaystyle u={\text{const}}}  [
{\displaystyle u={\text{const}}}] and     v =  const    {\displaystyle v={\text
{const}}}  [{\displaystyle v={\text{const}}}]. Near points where the gradient
of u (or, equivalently, v) is not zero, these families form an orthogonal
family of curves. At the points where     &#x2207; u = 0   {\displaystyle
\nabla u=0}  [\nabla u=0], the stationary points of the flow, the equipotential
curves of     u =  const    {\displaystyle u={\text{const}}}  [{\displaystyle
u={\text{const}}}] intersect. The streamlines also intersect at the same point,
bisecting the angles formed by the equipotential curves.
**** Harmonic vector field[edit] ****
Another interpretation of the CauchyâRiemann equations can be found in PÃ³lya
&_SzegÅ_(1978). Suppose that u and v satisfy the CauchyâRiemann equations in
an open subset of â2, and consider the vector_field
            f &#x00AF;    =   [    u     &#x2212; v    ]     {\displaystyle
      {\bar {f}}={\begin{bmatrix}u\\-v\end{bmatrix}}}  [{\bar {f}}={\begin
      {bmatrix}u\\-v\end{bmatrix}}]
regarded as a (real) two-component vector. Then the second CauchyâRiemann
equation (1b) asserts that        f &#x00AF;      {\displaystyle {\bar {f}}}  [
{\bar {f}}] is irrotational (its curl is 0):
            &#x2202; ( &#x2212; v )   &#x2202; x    &#x2212;    &#x2202; u
      &#x2202; y    = 0.   {\displaystyle {\frac {\partial (-v)}{\partial x}}-
      {\frac {\partial u}{\partial y}}=0.}  [{\frac {\partial (-v)}{\partial
      x}}-{\frac {\partial u}{\partial y}}=0.]
The first CauchyâRiemann equation (1a) asserts that the vector field is
solenoidal (or divergence-free):
            &#x2202; u   &#x2202; x    +    &#x2202; ( &#x2212; v )   &#x2202;
      y    = 0.   {\displaystyle {\frac {\partial u}{\partial x}}+{\frac
      {\partial (-v)}{\partial y}}=0.}  [{\frac {\partial u}{\partial x}}+
      {\frac {\partial (-v)}{\partial y}}=0.]
Owing respectively to Green's_theorem and the divergence_theorem, such a field
is necessarily a conservative one, and it is free from sources or sinks, having
net flux equal to zero through any open domain without holes. (These two
observations combine as real and imaginary parts in Cauchy's_integral_theorem.)
In fluid_dynamics, such a vector field is a potential_flow (Chanson_2007). In
magnetostatics, such vector fields model static magnetic_fields on a region of
the plane containing no current. In electrostatics, they model static electric
fields in a region of the plane containing no electric charge.
This interpretation can equivalently be restated in the language of
differential_forms. The pair u,v satisfy the CauchyâRiemann equations if and
only if the one-form     v  d x + u  d y   {\displaystyle v\,dx+u\,dy}
[v\,dx+u\,dy] is both closed and coclosed (a harmonic_differential_form).
**** Preservation of complex structure[edit] ****
Another formulation of the CauchyâRiemann equations involves the complex
structure in the plane, given by
         J =   [    0   &#x2212; 1     1   0    ]   .   {\displaystyle J=
      {\begin{bmatrix}0&-1\\1&0\end{bmatrix}}.}  [{\displaystyle J={\begin
      {bmatrix}0&-1\\1&0\end{bmatrix}}.}]
This is a complex structure in the sense that the square of J is the negative
of the 2×2 identity matrix:      J  2   = &#x2212; I   {\displaystyle J^{2}=-I}
[J^{2}=-I]. As above, if u(x,y),v(x,y) are two functions in the plane, put
         f ( x , y ) =   [    u ( x , y )     v ( x , y )    ]   .
      {\displaystyle f(x,y)={\begin{bmatrix}u(x,y)\\v(x,y)\end{bmatrix}}.}  [f
      (x,y)={\begin{bmatrix}u(x,y)\\v(x,y)\end{bmatrix}}.]
The Jacobian_matrix of f is the matrix of partial derivatives
         D f ( x , y ) =   [        &#x2202; u   &#x2202; x           &#x2202;
      u   &#x2202; y             &#x2202; v   &#x2202; x           &#x2202; v
      &#x2202; y        ]     {\displaystyle Df(x,y)={\begin{bmatrix}{\dfrac
      {\partial u}{\partial x}}&{\dfrac {\partial u}{\partial y}}\\[12pt]
      {\dfrac {\partial v}{\partial x}}&{\dfrac {\partial v}{\partial y}}\end
      {bmatrix}}}  [{\displaystyle Df(x,y)={\begin{bmatrix}{\dfrac {\partial u}
      {\partial x}}&{\dfrac {\partial u}{\partial y}}\\[12pt]{\dfrac {\partial
      v}{\partial x}}&{\dfrac {\partial v}{\partial y}}\end{bmatrix}}}]
Then the pair of functions u, v satisfies the CauchyâRiemann equations if and
only if the 2×2 matrix Df commutes with J (Kobayashi_&_Nomizu_1969, Proposition
IX.2.2)
This interpretation is useful in symplectic_geometry, where it is the starting
point for the study of pseudoholomorphic_curves.
**** Other representations[edit] ****
Other representations of the CauchyâRiemann equations occasionally arise in
other coordinate_systems. If (1a) and (1b) hold for a differentiable pair of
functions u and v, then so do
            &#x2202; u   &#x2202; n    =    &#x2202; v   &#x2202; s    ,
      &#x2202; v   &#x2202; n    = &#x2212;    &#x2202; u   &#x2202; s
      {\displaystyle {\frac {\partial u}{\partial n}}={\frac {\partial v}
      {\partial s}},\quad {\frac {\partial v}{\partial n}}=-{\frac {\partial u}
      {\partial s}}}  [{\frac {\partial u}{\partial n}}={\frac {\partial v}
      {\partial s}},\quad {\frac {\partial v}{\partial n}}=-{\frac {\partial u}
      {\partial s}}]
for any coordinate system (n(x, y), s(x, y)) such that the pair (ân, âs) is
orthonormal and positively_oriented. As a consequence, in particular, in the
system of coordinates given by the polar representation z = r eiÎ¸, the
equations then take the form
            &#x2202; u   &#x2202; r    =   1 r      &#x2202; v   &#x2202;
      &#x03B8;    ,     &#x2202; v   &#x2202; r    = &#x2212;   1 r
      &#x2202; u   &#x2202; &#x03B8;    .   {\displaystyle {\partial u \over
      \partial r}={1 \over r}{\partial v \over \partial \theta },\quad
      {\partial v \over \partial r}=-{1 \over r}{\partial u \over \partial
      \theta }.}  [{\partial u \over \partial r}={1 \over r}{\partial v \over
      \partial \theta },\quad {\partial v \over \partial r}=-{1 \over r}
      {\partial u \over \partial \theta }.]
Combining these into one equation for f gives
            &#x2202; f   &#x2202; r    =   1  i r       &#x2202; f   &#x2202;
      &#x03B8;    .   {\displaystyle {\partial f \over \partial r}={1 \over ir}
      {\partial f \over \partial \theta }.}  [{\partial f \over \partial r}={1
      \over ir}{\partial f \over \partial \theta }.]

The inhomogeneous CauchyâRiemann equations consist of the two equations for a
pair of unknown functions u(x,y) and v(x,y) of two real variables
                 &#x2202; u   &#x2202; x    &#x2212;    &#x2202; v   &#x2202; y
      = &#x03B1; ( x , y )         &#x2202; u   &#x2202; y    +    &#x2202; v
      &#x2202; x    = &#x03B2; ( x , y )       {\displaystyle {\begin{aligned}&
      {\frac {\partial u}{\partial x}}-{\frac {\partial v}{\partial y}}=\alpha
      (x,y)\\[4pt]&{\frac {\partial u}{\partial y}}+{\frac {\partial v}
      {\partial x}}=\beta (x,y)\end{aligned}}}  [{\displaystyle {\begin
      {aligned}&{\frac {\partial u}{\partial x}}-{\frac {\partial v}{\partial
      y}}=\alpha (x,y)\\[4pt]&{\frac {\partial u}{\partial y}}+{\frac {\partial
      v}{\partial x}}=\beta (x,y)\end{aligned}}}]
for some given functions Î±(x,y) and Î²(x,y) defined in an open subset of â2.
These equations are usually combined into a single equation
            &#x2202; f   &#x2202;    z &#x00AF;       = &#x03C6; ( z ,    z
      &#x00AF;    )   {\displaystyle {\frac {\partial f}{\partial {\bar
      {z}}}}=\varphi (z,{\bar {z}})}  [{\frac {\partial f}{\partial {\bar
      {z}}}}=\varphi (z,{\bar {z}})]
where f = u + iv and Ï = (Î± + iÎ²)/2.
If Ï is Ck, then the inhomogeneous equation is explicitly solvable in any
bounded domain D, provided Ï is continuous on the closure of D. Indeed, by the
Cauchy_integral_formula,
         f ( &#x03B6; ,    &#x03B6; &#x00AF;    ) =   1  2 &#x03C0; i
      &#x222C;  D   &#x03C6; ( z ,    z &#x00AF;    )     d z &#x2227; d    z
      &#x00AF;      z &#x2212; &#x03B6;      {\displaystyle f(\zeta ,{\bar
      {\zeta }})={\frac {1}{2\pi i}}\iint _{D}\varphi (z,{\bar {z}})\,{\frac
      {dz\wedge d{\bar {z}}}{z-\zeta }}}  [{\displaystyle f(\zeta ,{\bar {\zeta
      }})={\frac {1}{2\pi i}}\iint _{D}\varphi (z,{\bar {z}})\,{\frac {dz\wedge
      d{\bar {z}}}{z-\zeta }}}]
for all Î¶ â D.
***** Generalizations[edit] *****
**** Goursat's theorem and its generalizations[edit] ****
See also: CauchyâGoursat_theorem
Suppose that f = u + iv is a complex-valued function which is differentiable as
a function f : â2 â â2. Then Goursat's theorem asserts that f is analytic
in an open complex domain Î© if and only if it satisfies the CauchyâRiemann
equation in the domain (Rudin_1966, Theorem 11.2). In particular, continuous
differentiability of f need not be assumed (DieudonnÃ©_1969, Â§9.10, Ex. 1).
The hypotheses of Goursat's theorem can be weakened significantly. If f =
u + iv is continuous in an open set Î© and the partial_derivatives of f with
respect to x and y exist in Î©, and satisfy the CauchyâRiemann equations
throughout Î©, then f is holomorphic (and thus analytic). This result is the
LoomanâMenchoff_theorem.
The hypothesis that f obey the CauchyâRiemann equations throughout the domain
Î© is essential. It is possible to construct a continuous function satisfying
the CauchyâRiemann equations at a point, but which is not analytic at the
point (e.g., f(z) = z5 / |z|4). Similarly, some additional assumption is needed
besides the CauchyâRiemann equations (such as continuity), as the following
example illustrates (Looman_1923, p. 107)
         f ( z ) =   {    exp &#x2061; ( &#x2212;  z  &#x2212; 4   )
      if&#xA0;  z &#x2260; 0     0    if&#xA0;  z = 0         {\displaystyle f
      (z)={\begin{cases}\exp(-z^{-4})&{\text{if }}z\not =0\\0&{\text{if
      }}z=0\end{cases}}}  [{\displaystyle f(z)={\begin{cases}\exp(-z^{-4})&
      {\text{if }}z\not =0\\0&{\text{if }}z=0\end{cases}}}]
which satisfies the CauchyâRiemann equations everywhere, but fails to be
continuous at z = 0.
Nevertheless, if a function satisfies the CauchyâRiemann equations in an open
set in a weak_sense, then the function is analytic. More precisely (Gray_&
Morris_1978, Theorem 9):
    * If f(z) is locally integrable in an open domain Î© â â, and satisfies
      the CauchyâRiemann equations weakly, then f agrees almost_everywhere
      with an analytic function in Î©.
This is in fact a special case of a more general result on the regularity of
solutions of hypoelliptic partial differential equations.
**** Several variables[edit] ****
There are CauchyâRiemann equations, appropriately generalized, in the theory
of several_complex_variables. They form a significant overdetermined_system of
PDEs. This is done using a straightforward generalization of the Wirtinger
derivative, where the function in question is required to have the (partial)
Wirtinger derivative with respect to each complex variable vanish.
**** Complex differential forms[edit] ****
As often formulated, the d-bar_operator
            &#x2202; &#x00AF;      {\displaystyle {\bar {\partial }}}  [{\bar
      {\partial }}]
annihilates holomorphic functions. This generalizes most directly the
formulation
            &#x2202; f   &#x2202;    z &#x00AF;       = 0 ,   {\displaystyle
      {\partial f \over \partial {\bar {z}}}=0,}  [{\partial f \over \partial
      {\bar {z}}}=0,]
where
            &#x2202; f   &#x2202;    z &#x00AF;       =   1 2    (     &#x2202;
      f   &#x2202; x    + i    &#x2202; f   &#x2202; y     )  .
      {\displaystyle {\partial f \over \partial {\bar {z}}}={1 \over 2}\left(
      {\partial f \over \partial x}+i{\partial f \over \partial y}\right).}  [
      {\partial f \over \partial {\bar {z}}}={1 \over 2}\left({\partial f \over
      \partial x}+i{\partial f \over \partial y}\right).]
**** BÃ¤cklund transform[edit] ****
Viewed as conjugate_harmonic_functions, the CauchyâRiemann equations are a
simple example of a BÃ¤cklund_transform. More complicated, generally non-linear
BÃ¤cklund transforms, such as in the sine-Gordon_equation, are of great
interest in the theory of solitons and integrable_systems.
**** Definition in Clifford algebra[edit] ****
In Clifford_algebra the complex number     z = x + i y   {\displaystyle z=x+iy}
[z=x+iy] is represented as     z &#x2261; x + I y   {\displaystyle z\equiv
x+Iy}  [z\equiv x+Iy] where     I &#x2261;  &#x03C3;  1    &#x03C3;  2
{\displaystyle I\equiv \sigma _{1}\sigma _{2}}  [I\equiv \sigma _{1}\sigma _
{2}]. The fundamental derivative operator in Clifford algebra of Complex
numbers is defined as     &#x2207; &#x2261;  &#x03C3;  1    &#x2202;  x   +
&#x03C3;  2    &#x2202;  y     {\displaystyle \nabla \equiv \sigma _{1}\partial
_{x}+\sigma _{2}\partial _{y}}  [\nabla \equiv \sigma _{1}\partial _{x}+\sigma
_{2}\partial _{y}]. The function     f = u + I v   {\displaystyle f=u+Iv}
[f=u+Iv] is considered analytic if and only if     &#x2207; f = 0
{\displaystyle \nabla f=0}  [\nabla f=0], which can be calculated in following
way:
             0    = &#x2207; f = (  &#x03C3;  1    &#x2202;  x   +  &#x03C3;  2
      &#x2202;  y   ) ( u +  &#x03C3;  1    &#x03C3;  2   v )       =  &#x03C3;
      1    &#x2202;  x   u +      &#x03C3;  1    &#x03C3;  1    &#x03C3;  2
      &#x23DF;    =  &#x03C3;  2      &#x2202;  x   v +  &#x03C3;  2
      &#x2202;  y   u +      &#x03C3;  2    &#x03C3;  1    &#x03C3;  2
      &#x23DF;    = &#x2212;  &#x03C3;  1      &#x2202;  y   v = 0
      {\displaystyle {\begin{aligned}0&=\nabla f=(\sigma _{1}\partial _
      {x}+\sigma _{2}\partial _{y})(u+\sigma _{1}\sigma _{2}v)\\[4pt]&=\sigma _
      {1}\partial _{x}u+\underbrace {\sigma _{1}\sigma _{1}\sigma _{2}} _
      {=\sigma _{2}}\partial _{x}v+\sigma _{2}\partial _{y}u+\underbrace
      {\sigma _{2}\sigma _{1}\sigma _{2}} _{=-\sigma _{1}}\partial _{y}v=0\end
      {aligned}}}  [{\displaystyle {\begin{aligned}0&=\nabla f=(\sigma _
      {1}\partial _{x}+\sigma _{2}\partial _{y})(u+\sigma _{1}\sigma _{2}v)\\
      [4pt]&=\sigma _{1}\partial _{x}u+\underbrace {\sigma _{1}\sigma _
      {1}\sigma _{2}} _{=\sigma _{2}}\partial _{x}v+\sigma _{2}\partial _
      {y}u+\underbrace {\sigma _{2}\sigma _{1}\sigma _{2}} _{=-\sigma _
      {1}}\partial _{y}v=0\end{aligned}}}]
Grouping by      &#x03C3;  1     {\displaystyle \sigma _{1}}  [\sigma _{1}] and
&#x03C3;  2     {\displaystyle \sigma _{2}}  [\sigma _{2}]:
         &#x2207; f =  &#x03C3;  1   (  &#x2202;  x   u &#x2212;  &#x2202;  y
      v ) +  &#x03C3;  2   (  &#x2202;  x   v +  &#x2202;  y   u ) = 0 &#x21D4;
      {     &#x2202;  x   u &#x2212;  &#x2202;  y   v = 0      &#x2202;  x   v
      +  &#x2202;  y   u = 0         {\displaystyle \nabla f=\sigma _{1}
      (\partial _{x}u-\partial _{y}v)+\sigma _{2}(\partial _{x}v+\partial _
      {y}u)=0\Leftrightarrow {\begin{cases}\partial _{x}u-\partial _{y}v=0\\
      [4pt]\partial _{x}v+\partial _{y}u=0\end{cases}}}  [{\displaystyle \nabla
      f=\sigma _{1}(\partial _{x}u-\partial _{y}v)+\sigma _{2}(\partial _
      {x}v+\partial _{y}u)=0\Leftrightarrow {\begin{cases}\partial _{x}u-
      \partial _{y}v=0\\[4pt]\partial _{x}v+\partial _{y}u=0\end{cases}}}]
Henceforth in traditional notation:
           {        &#x2202; u   &#x2202; x     =     &#x2202; v   &#x2202; y
      &#x2202; u   &#x2202; y     = &#x2212;     &#x2202; v   &#x2202; x
      {\displaystyle {\begin{cases}{\dfrac {\partial u}{\partial x}}={\dfrac
      {\partial v}{\partial y}}\\[12pt]{\dfrac {\partial u}{\partial y}}=-
      {\dfrac {\partial v}{\partial x}}\end{cases}}}  [{\displaystyle {\begin
      {cases}{\dfrac {\partial u}{\partial x}}={\dfrac {\partial v}{\partial
      y}}\\[12pt]{\dfrac {\partial u}{\partial y}}=-{\dfrac {\partial v}
      {\partial x}}\end{cases}}}]
**** Conformal mappings in higher dimensions[edit] ****
Let Ω be an open set in the Euclidean space ân. The equation for an
orientation-preserving mapping     f : &#x03A9; &#x2192;   R   n
{\displaystyle f:\Omega \to \mathbb {R} ^{n}}  [{\displaystyle f:\Omega \to
\mathbb {R} ^{n}}] to be a conformal_mapping (that is, angle-preserving) is
that
         D  f  T   D f = ( det ( D f )  )  2  /  n   I   {\displaystyle Df^
      {T}Df=(\det(Df))^{2/n}I}  [Df^{T}Df=(\det(Df))^{2/n}I]
where Df is the Jacobian matrix, with transpose     D  f  T     {\displaystyle
Df^{T}}  [Df^{T}], and I denotes the identity matrix (Iwaniec_&_Martin_2001,
p. 32). For n = 2, this system is equivalent to the standard CauchyâRiemann
equations of complex variables, and the solutions are holomorphic functions. In
dimension n > 2, this is still sometimes called the CauchyâRiemann system,
and Liouville's_theorem implies, under suitable smoothness assumptions, that
any such mapping is a MÃ¶bius_transformation.
***** See also[edit] *****
    * List_of_complex_analysis_topics
    * Morera's_theorem
    * Wirtinger_derivatives
***** References[edit] *****
    * Ahlfors,_Lars (1953), Complex analysis (3rd ed.), McGraw Hill (published
      1979), ISBN 0-07-000657-1
.
d'Alembert,_Jean (1752), Essai_d'une_nouvelle_thÃ©orie_de_la_rÃ©sistance_des
fluides, Paris
.
Cauchy,_Augustin_L. (1814), MÃ©moire sur les intÃ©grales dÃ©finies, Oeuvres
complÃ¨tes Ser. 1, 1, Paris (published 1882), pp. 319â506
Chanson, H. (2007), "Le_Potentiel_de_Vitesse_pour_les_Ecoulements_de_Fluides
RÃ©els:_la_Contribution_de_Joseph-Louis_Lagrange."_('Velocity_Potential_in_Real
Fluid_Flows:_Joseph-Louis_Lagrange's_Contribution.')", Journal La Houille
Blanche, 5: 127â131, doi:10.1051/lhb:2007072, ISSN 0018-6368
.
DieudonnÃ©,_Jean_Alexandre (1969), Foundations of modern analysis, Academic
Press
.
Euler,_Leonhard (1797), "Ulterior_disquisitio_de_formulis_integralibus
imaginariis", Nova Acta Academiae Scientiarum Imperialis Petropolitanae, 10:
3â19
Gray, J. D.; Morris, S. A. (1978), "When is a Function that Satisfies the
Cauchy–Riemann Equations Analytic?", The American Mathematical Monthly
(published April 1978), 85 (4): 246â256, doi:10.2307/2321164, JSTOR 2321164
.
Klein,_Felix (1893), On Riemann's theory of algebraic functions and their
integrals, Cambridge: MacMillan and Bowes
; translated by Frances Hardcastle.
Iwaniec, T; Martin, G (2001), Geometric function theory and non-linear
analysis, Oxford
.
Looman, H. (1923), "Ãber die Cauchy–Riemannschen Differentialgleichungen",
GÃ¶ttinger Nachrichten: 97â108
.
Kobayashi,_Shoshichi; Nomizu,_Katsumi (1969), Foundations of differential
geometry, volume 2, Wiley
.
PÃ³lya,_George; SzegÅ, GÃ¡bor (1978), Problems and theorems in analysis I,
Springer, ISBN 3-540-63640-4
Riemann,_Bernhard (1851), "Grundlagen fÃ¼r eine allgemeine Theorie der
Funktionen einer verÃ¤nderlichen komplexen GrÃ¶sse", in H. Weber (ed.),
Riemann's gesammelte math. Werke, Dover (published 1953), pp. 3â48
Rudin,_Walter (1966), Real and complex analysis (3rd ed.), McGraw Hill
(published 1987), ISBN 0-07-054234-1
.
Solomentsev, E.D. (2001) [1994], "CauchyâRiemann_conditions", in Hazewinkel,
Michiel (ed.), Encyclopedia_of_Mathematics, Springer Science+Business Media
B.V. / Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Stewart,_Ian; Tall, David (1983), Complex Analysis (1st ed.), CUP (published
1984), ISBN 0-521-28763-4
.
***** External links[edit] *****
    * Weisstein,_Eric_W. "CauchyâRiemann_Equations". MathWorld.
CauchyâRiemann_Equations_Module_by_John_H._Mathews

Retrieved from "https://en.wikipedia.org/w/
index.php?title=CauchyâRiemann_equations&oldid=906964318"
Categories:
    * Partial_differential_equations
    * Complex_analysis
    * Harmonic_functions
    * Bernhard_Riemann
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * LietuviÅ³
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * PiemontÃ¨is
    * Polski
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 19 July 2019, at 14:23 (UTC).
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
