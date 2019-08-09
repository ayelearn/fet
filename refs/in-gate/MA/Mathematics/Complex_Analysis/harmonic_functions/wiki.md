The following text has been accessed from https://en.wikipedia.org/wiki/Harmonic_function at Fri Aug 9 02:32:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Harmonic function ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about harmonic functions in mathematics. For harmonic function
in music, see diatonic_functionality.
A harmonic function defined on an annulus.
In mathematics, mathematical_physics and the theory of stochastic_processes, a
harmonic function is a twice continuously_differentiable function f : U â R
where U is an open_subset of Rn that satisfies Laplace's_equation, i.e.
             &#x2202;  2   f   &#x2202;  x  1   2      +     &#x2202;  2   f
      &#x2202;  x  2   2      + &#x22EF; +     &#x2202;  2   f   &#x2202;  x  n
      2      = 0   {\displaystyle {\frac {\partial ^{2}f}{\partial x_{1}^{2}}}+
      {\frac {\partial ^{2}f}{\partial x_{2}^{2}}}+\cdots +{\frac {\partial ^
      {2}f}{\partial x_{n}^{2}}}=0}  [ \frac{\partial^2f}{\partial x_1^2} +
      \frac{\partial^2f}{\partial x_2^2} + \cdots + \frac{\partial^2f}{\partial
      x_n^2} = 0]
everywhere on U. This is usually written as
          &#x2207;  2   f = 0   {\displaystyle \nabla ^{2}f=0}  [ \nabla^2 f =
      0 ]
or
          &#x0394; f = 0    {\displaystyle \textstyle \Delta f=0}  [\textstyle
      \Delta f = 0]
⁰
***** Contents *****
    * 1_Etymology_of_the_term_"harmonic"
    * 2_Examples
    * 3_Remarks
    * 4_Connections_with_complex_function_theory
    * 5_Properties_of_harmonic_functions
          o 5.1_Regularity_theorem_for_harmonic_functions
          o 5.2_Maximum_principle
          o 5.3_The_mean_value_property
          o 5.4_Harnack's_inequality
          o 5.5_Removal_of_singularities
          o 5.6_Liouville's_theorem
    * 6_Generalizations
          o 6.1_Weakly_harmonic_function
          o 6.2_Harmonic_functions_on_manifolds
          o 6.3_Subharmonic_functions
          o 6.4_Harmonic_forms
          o 6.5_Harmonic_maps_between_manifolds
    * 7_See_also
    * 8_Notes
    * 9_References
    * 10_External_links
***** Etymology of the term "harmonic"[edit] *****
The descriptor "harmonic" in the name harmonic function originates from a point
on a taut string which is undergoing harmonic_motion. This solution to the
differential equation for this type of motion can be written in terms of sines
and cosines, functions which are thus referred to as harmonics. Fourier
analysis involves expanding periodic functions on the unit circle in terms of a
series of these harmonics. Considering higher dimensional analogues of the
harmonics on the unit n-sphere, one arrives at the spherical_harmonics. These
functions satisfy Laplace's equation and over time "harmonic" was used_to_refer
to_all functions satisfying Laplace's equation.[1]
***** Examples[edit] *****
Examples of harmonic functions of two variables are:
    * The real or imaginary part of any holomorphic_function
    * The function       f ( x , y ) =  e  x   sin &#x2061; y   {\displaystyle
      \,\!f(x,y)=e^{x}\sin y}  [\,\! f(x,y)=e^{x} \sin y]; this is a special
      case of the example above, as     f ( x , y ) = Im &#x2061; (  e  x + i y
      )   {\displaystyle f(x,y)=\operatorname {Im} (e^{x+iy})}  [f
      (x,y)=\operatorname {Im}(e^{{x+iy}})], and      e  x + i y
      {\displaystyle e^{x+iy}}  [e^{x+iy}] is a holomorphic_function.
    * The function       f ( x , y ) = ln &#x2061; (  x  2   +  y  2   )
      {\displaystyle \,\!f(x,y)=\ln(x^{2}+y^{2})}  [{\displaystyle \,\!f
      (x,y)=\ln(x^{2}+y^{2})}] defined on       R   2   &#x2216; { 0 }
      {\displaystyle \mathbb {R} ^{2}\setminus \lbrace 0\rbrace }  [{\mathbb
      {R}}^{2}\setminus \lbrace 0\rbrace ]. This can describe the electric
      potential due to a line charge or the gravity potential due to a long
      cylindrical mass.
Examples of harmonic functions of three variables are given in the table below
with      r  2   =  x  2   +  y  2   +  z  2     {\displaystyle r^{2}=x^{2}+y^
{2}+z^{2}}  [r^2=x^2+y^2+z^2]:
      Function                             Singularity
           1 r     {\displaystyle {\frac   Unit point charge at origin
           {1}{r}}}  [{\frac {1}{r}}]
            x  r  3       {\displaystyle   x-directed dipole at origin
      {\frac {x}{r^{3}}}}  [\frac{x}{r^3}]
           &#x2212; ln &#x2061; (  r  2
      &#x2212;  z  2   )    {\displaystyle Line of unit charge density on
        -\ln(r^{2}-z^{2})\,}  [-\ln(r^2-   entire z-axis
                    z^2)\,]
          &#x2212; ln &#x2061; ( r + z )   Line of unit charge density on
       {\displaystyle -\ln(r+z)\,}  [-\ln  negative z-axis
                    (r+z)\,]
              x   r  2   &#x2212;  z  2    Line of x-directed dipoles on entire
       {\displaystyle {\frac {x}{r^{2}-z^  z axis
        {2}}}\,}  [\frac{x}{r^2-z^2}\,]
                 x  r ( r + z )            Line of x-directed dipoles on
           {\displaystyle {\frac {x}{r     negative z axis
         (r+z)}}\,}  [\frac{x}{r(r+z)}\,]
Harmonic functions that arise in physics are determined by their singularities
and boundary conditions (such as Dirichlet_boundary_conditions or Neumann
boundary_conditions). On regions without boundaries, adding the real or
imaginary part of any entire_function will produce a harmonic function with the
same singularity, so in this case the harmonic function is not determined by
its singularities; however, we can make the solution unique in physical
situations by requiring that the solution approaches 0 as r approaches
infinity. In this case, uniqueness follows by Liouville's_theorem.
The singular points of the harmonic functions above are expressed as "charges"
and "charge_densities" using the terminology of electrostatics, and so the
corresponding harmonic function will be proportional to the electrostatic
potential due to these charge distributions. Each function above will yield
another harmonic function when multiplied by a constant, rotated, and/or has a
constant added. The inversion of each function will yield another harmonic
function which has singularities which are the images of the original
singularities in a spherical "mirror". Also, the sum of any two harmonic
functions will yield another harmonic function.
Finally, examples of harmonic functions of n variables are:
    * The constant, linear and affine functions on all of Rn (for example, the
      electric_potential between the plates of a capacitor, and the gravity
      potential of a slab)
    * The function       f (  x  1   , &#x2026; ,  x  n   ) = (    x  1     2
      + &#x22EF; +    x  n     2    )  1 &#x2212; n  /  2     {\displaystyle
      \,\!f(x_{1},\dots ,x_{n})=({x_{1}}^{2}+\cdots +{x_{n}}^{2})^{1-n/2}}
      [\,\! f(x_1,\dots,x_n)=({x_1}^2+\cdots+{x_n}^2)^{1-n/2}] on       R   n
      &#x2216; { 0 }   {\displaystyle \mathbb {R} ^{n}\setminus \lbrace
      0\rbrace }  [{\mathbb  {R}}^{n}\setminus \lbrace 0\rbrace ] for n > 2.
***** Remarks[edit] *****
The set of harmonic functions on a given open set U can be seen as the kernel
of the Laplace_operator Î and is therefore a vector_space over R: sums,
differences and scalar multiples of harmonic functions are again harmonic.
If f is a harmonic function on U, then all partial_derivatives of f are also
harmonic functions on U. The Laplace operator Î and the partial derivative
operator will commute on this class of functions.
In several ways, the harmonic functions are real analogues to holomorphic
functions. All harmonic functions are analytic, i.e. they can be locally
expressed as power_series. This is a general fact about elliptic_operators, of
which the Laplacian is a major example.
The uniform limit of a convergent sequence of harmonic functions is still
harmonic. This is true because every continuous function satisfying the mean
value property is harmonic. Consider the sequence on (ââ, 0) Ã R defined
by       f  n   ( x , y ) =   1 n   exp &#x2061; ( n x ) cos &#x2061; ( n y )
{\displaystyle \scriptstyle f_{n}(x,y)={\frac {1}{n}}\exp(nx)\cos(ny)}
[\scriptstyle f_n(x,y) = \frac1n \exp(nx)\cos(ny)]. This sequence is harmonic
and converges uniformly to the zero function; however note that the partial
derivatives are not uniformly convergent to the zero function (the derivative
of the zero function). This example shows the importance of relying on the mean
value property and continuity to argue that the limit is harmonic.
***** Connections with complex function theory[edit] *****
The real and imaginary part of any holomorphic function yield harmonic
functions on R2 (these are said to be a pair of harmonic_conjugate functions).
Conversely, any harmonic function u on an open subset Î© of R2 is locally the
real part of a holomorphic function. This is immediately seen observing that,
writing z = x + iy, the complex function g(z) := ux â i uy is holomorphic in
Î© because it satisfies the CauchyâRiemann_equations. Therefore, g has
locally a primitive f, and u is the real part of f up to a constant, as ux is
the real part of      f    &#x2032;   = g    {\displaystyle \scriptstyle f\,^
{\prime }=g}  [\scriptstyle f\,^\prime=g] .
Although the above correspondence with holomorphic functions only holds for
functions of two real variables, harmonic functions in n variables still enjoy
a number of properties typical of holomorphic functions. They are (real)
analytic; they have a maximum principle and a mean-value principle; a theorem
of removal of singularities as well as a Liouville theorem holds for them in
analogy to the corresponding theorems in complex functions theory.
***** Properties of harmonic functions[edit] *****
Some important properties of harmonic functions can be deduced from Laplace's
equation.
**** Regularity theorem for harmonic functions[edit] ****
Harmonic functions are infinitely differentiable in open sets. In fact,
harmonic functions are real_analytic.
**** Maximum principle[edit] ****
Harmonic functions satisfy the following maximum_principle: if K is a nonempty
compact_subset of U, then f restricted to K attains its maximum_and_minimum on
the boundary of K. If U is connected, this means that f cannot have local
maxima or minima, other than the exceptional case where f is constant. Similar
properties can be shown for subharmonic functions.
**** The mean value property[edit] ****
If B(x, r) is a ball with center x and radius r which is completely contained
in the open set Î© â Rn, then the value u(x) of a harmonic function u: Î© â
R at the center of the ball is given by the average value of u on the surface
of the ball; this average value is also equal to the average value of u in the
interior of the ball. In other words,
         u ( x ) =   1  n  &#x03C9;  n    r  n &#x2212; 1       &#x222B;
      &#x2202; B ( x , r )   u  d &#x03C3; =   1   &#x03C9;  n    r  n
      &#x222B;  B ( x , r )   u  d V   {\displaystyle u(x)={\frac {1}{n\omega _
      {n}r^{n-1}}}\int _{\partial B(x,r)}u\,d\sigma ={\frac {1}{\omega _{n}r^
      {n}}}\int _{B(x,r)}u\,dV}  [{\displaystyle u(x)={\frac {1}{n\omega _{n}r^
      {n-1}}}\int _{\partial B(x,r)}u\,d\sigma ={\frac {1}{\omega _{n}r^
      {n}}}\int _{B(x,r)}u\,dV}]
where Ïn is the area of the unit_sphere in n dimensions and Ï is the
(n â 1)-dimensional surface measure.
Conversely, all locally integrable functions satisfying the (volume) mean-value
property are both infinitely differentiable and harmonic.
In terms of convolutions, if
          &#x03C7;  r   :=   1   |  B ( 0 , r )  |      &#x03C7;  B ( 0 , r )
      =   n   &#x03C9;  n    r  n       &#x03C7;  B ( 0 , r )
      {\displaystyle \chi _{r}:={\frac {1}{|B(0,r)|}}\chi _{B(0,r)}={\frac {n}
      {\omega _{n}r^{n}}}\chi _{B(0,r)}}  [{\displaystyle \chi _{r}:={\frac {1}
      {|B(0,r)|}}\chi _{B(0,r)}={\frac {n}{\omega _{n}r^{n}}}\chi _{B(0,r)}}]
denotes the characteristic_function of the ball with radius r about the origin,
normalized so that       &#x222B;    R   n      &#x03C7;  r    d x = 1
{\displaystyle \scriptstyle \int _{\mathbf {R} ^{n}}\chi _{r}\,dx=1}
[\scriptstyle \int_{\mathbf{R}^n}\chi_r\, dx=1], the function u is harmonic on
Î© if and only if
         u ( x ) = u &#x2217;  &#x03C7;  r   ( x )    {\displaystyle u
      (x)=u*\chi _{r}(x)\;}  [u(x) = u*\chi_r(x)\;]
as soon as B(x, r) â Î©.
Sketch of the proof. The proof of the mean-value property of the harmonic
functions and its converse follows immediately observing that the non-
homogeneous equation, for any 0 < s < r
         &#x0394; w =  &#x03C7;  r   &#x2212;  &#x03C7;  s      {\displaystyle
      \Delta w=\chi _{r}-\chi _{s}\;}  [\Delta w = \chi_r  - \chi_s\;]
admits an easy explicit solution wr,s of class C1,1 with compact support in B
(0, r). Thus, if u is harmonic in Î©
         0 = &#x0394; u &#x2217;  w  r , s   = u &#x2217; &#x0394;  w  r , s
      = u &#x2217;  &#x03C7;  r   &#x2212; u &#x2217;  &#x03C7;  s
      {\displaystyle 0=\Delta u*w_{r,s}=u*\Delta w_{r,s}=u*\chi _{r}-u*\chi _
      {s}\;}  [0=\Delta u * w_{r,s} = u*\Delta w_{r,s}= u*\chi_r  - u*\chi_s\;]
holds in the set Î©r of all points x in     &#x03A9;   {\displaystyle \Omega }
[\Omega ] with     dist &#x2061; ( x , &#x2202; &#x03A9; ) > r   {\displaystyle
\operatorname {dist} (x,\partial \Omega )>r}  [{\displaystyle \operatorname
{dist} (x,\partial \Omega )>r}] .
Since u is continuous in Î©, u*Ïr converges to u as s â 0 showing the mean
value property for u in Î©. Conversely, if u is any      L   l o c    1
{\displaystyle L_{\mathrm {loc} }^{1}\;}  [L^1_{\mathrm{loc}}\;] function
satisfying the mean-value property in Î©, that is,
         u &#x2217;  &#x03C7;  r   = u &#x2217;  &#x03C7;  s
      {\displaystyle u*\chi _{r}=u*\chi _{s}\;}  [u*\chi_r = u*\chi_s\;]
holds in Î©r for all 0 < s < r then, iterating m times the convolution with Ïr
one has:
         u = u &#x2217;  &#x03C7;  r   = u &#x2217;  &#x03C7;  r   &#x2217;
      &#x22EF; &#x2217;  &#x03C7;  r    ,  x &#x2208;  &#x03A9;  m r   ,
      {\displaystyle u=u*\chi _{r}=u*\chi _{r}*\cdots *\chi _{r}\,,\qquad x\in
      \Omega _{mr},}  [u = u*\chi_r = u*\chi_r*\cdots*\chi_r\,,\qquad
      x\in\Omega_{mr},]
so that u is      C  m &#x2212; 1   (  &#x03A9;  m r   )    {\displaystyle C^
{m-1}(\Omega _{mr})\;}  [C^{m-1}(\Omega_{mr})\;] because the m-fold iterated
convolution of Ïr is of class      C  m &#x2212; 1      {\displaystyle C^{m-
1}\;}  [C^{m-1}\;] with support B(0, mr). Since r and m are arbitrary, u is
C  &#x221E;   ( &#x03A9; )    {\displaystyle C^{\infty }(\Omega )\;}  [C^
{\infty}(\Omega)\;] too. Moreover,
         &#x0394; u &#x2217;  w  r , s   = u &#x2217; &#x0394;  w  r , s   = u
      &#x2217;  &#x03C7;  r   &#x2212; u &#x2217;  &#x03C7;  s   = 0
      {\displaystyle \Delta u*w_{r,s}=u*\Delta w_{r,s}=u*\chi _{r}-u*\chi _
      {s}=0\;}  [\Delta u * w_{r,s} = u*\Delta w_{r,s} = u*\chi_r  -
      u*\chi_s=0\;]
for all 0 < s < r so that Îu = 0 in Î© by the fundamental theorem of the
calculus of variations, proving the equivalence between harmonicity and mean-
value property.
This statement of the mean value property can be generalized as follows: If h
is any spherically symmetric function supported in B(x,r) such that â«h = 1,
then u(x) = h * u(x). In other words, we can take the weighted average of u
about a point and recover u(x). In particular, by taking h to be a Câ
function, we can recover the value of u at any point even if we only know how u
acts as a distribution. See Weyl's_lemma.
**** Harnack's inequality[edit] ****
Let u be a non-negative harmonic function in a bounded domain Î©. Then for
every connected set
         V &#x2282;   V &#x00AF;   &#x2282; &#x03A9; ,   {\displaystyle
      V\subset {\overline {V}}\subset \Omega ,}  [V \subset \overline{V}
      \subset \Omega,]
Harnack's_inequality
          sup  V   u &#x2264; C  inf  V   u   {\displaystyle \sup _{V}u\leq
      C\inf _{V}u}  [\sup_V u \le C \inf_V u]
holds for some constant C that depends only on V and Î©.
**** Removal of singularities[edit] ****
The following principle of removal of singularities holds for harmonic
functions. If f is a harmonic function defined on a dotted open subset
&#x03A9;  &#x2216;  {  x  0   }    {\displaystyle \scriptstyle \Omega
\,\setminus \,\{x_{0}\}}  [\scriptstyle \Omega \,\setminus \,\{x_{0}\}] of Rn,
which is less singular at x0 than the fundamental solution, that is
         f ( x ) = o  (  | x &#x2212;  x  0    |  2 &#x2212; n    )  ,
      as&#xA0;  x &#x2192;  x  0   ,   {\displaystyle f(x)=o\left(\vert x-x_
      {0}\vert ^{2-n}\right),\qquad {\text{as }}x\to x_{0},}  [f(x)=o\left
      (\vert x-x_{0}\vert ^{{2-n}}\right),\qquad {\text{as }}x\to x_{0},]
then f extends to a harmonic function on Î© (compare Riemann's_theorem for
functions of a complex variable).
**** Liouville's theorem[edit] ****
Theorem: If f is a harmonic function defined on all of Rn which is bounded
above or bounded below, then f is constant.
(Compare Liouville's_theorem_for_functions_of_a_complex_variable).
Edward_Nelson gave a particularly short proof [2] of this theorem for the case
of bounded functions, using the mean value property mentioned above:
     Given two points, choose two balls with the given points as centers
     and of equal radius. If the radius is large enough, the two balls
     will coincide except for an arbitrarily small proportion of their
     volume. Since f is bounded, the averages of it over the two balls are
     arbitrarily close, and so f assumes the same value at any two points.
The proof can be adapted to the case where the harmonic function f is merely
bounded above or below. By adding a constant and possibly multiplying by
&#x2212; 1   {\displaystyle -1}  [-1], we may assume that f is non-negative.
Then for any two points     x   {\displaystyle x}  [x] and     y
{\displaystyle y}  [y], and any positive number     R   {\displaystyle R}  [R],
we let     r = R + d ( x , y )   {\displaystyle r=R+d(x,y)}  [{\displaystyle
r=R+d(x,y)}]. We then consider the balls      B  R   ( x )   {\displaystyle B_
{R}(x)}  [{\displaystyle B_{R}(x)}] and      B  r   ( y )   {\displaystyle B_
{r}(y)}  [{\displaystyle B_{r}(y)}], where by the triangle inequality, the
first ball is contained in the second.
By the averaging property and the monotonicity of the integral, we have
         f ( x ) =   1  vol &#x2061; (  B  R   )     &#x222B;   B  R   ( x )
      f ( z )  d z &#x2264;   1  vol &#x2061; (  B  R   )     &#x222B;   B  r
      ( y )   f ( z )  d z .   {\displaystyle f(x)={\frac {1}{\operatorname
      {vol} (B_{R})}}\int _{B_{R}(x)}f(z)\,dz\leq {\frac {1}{\operatorname
      {vol} (B_{R})}}\int _{B_{r}(y)}f(z)\,dz.}  [{\displaystyle f(x)={\frac
      {1}{\operatorname {vol} (B_{R})}}\int _{B_{R}(x)}f(z)\,dz\leq {\frac {1}
      {\operatorname {vol} (B_{R})}}\int _{B_{r}(y)}f(z)\,dz.}]
(Note that since     vol &#x2061; (  B  R   ( x ) )   {\displaystyle
\operatorname {vol} (B_{R}(x))}  [{\displaystyle \operatorname {vol} (B_{R}
(x))}] is independent of     x   {\displaystyle x}  [x], we denote it merely as
vol &#x2061; (  B  R   )   {\displaystyle \operatorname {vol} (B_{R})}  [
{\displaystyle \operatorname {vol} (B_{R})}].) In the last expression, we may
multiply and divide by     vol &#x2061; (  B  r   )   {\displaystyle
\operatorname {vol} (B_{r})}  [{\displaystyle \operatorname {vol} (B_{r})}] and
use the averaging property again, to obtain
         f ( x ) &#x2264;    vol &#x2061; (  B  r   )   vol &#x2061; (  B  R
      )    f ( y ) .   {\displaystyle f(x)\leq {\frac {\operatorname {vol} (B_
      {r})}{\operatorname {vol} (B_{R})}}f(y).}  [{\displaystyle f(x)\leq
      {\frac {\operatorname {vol} (B_{r})}{\operatorname {vol} (B_{R})}}f(y).}]
But as     R &#x2192; &#x221E;   {\displaystyle R\rightarrow \infty }
[R\rightarrow\infty], the quantity
            vol &#x2061; (  B  r   )   vol &#x2061; (  B  R   )    =    ( R + d
      ( x , y )  )  n     R  n       {\displaystyle {\frac {\operatorname {vol}
      (B_{r})}{\operatorname {vol} (B_{R})}}={\frac {(R+d(x,y))^{n}}{R^{n}}}}
      [{\displaystyle {\frac {\operatorname {vol} (B_{r})}{\operatorname {vol}
      (B_{R})}}={\frac {(R+d(x,y))^{n}}{R^{n}}}}]
tends to 1. Thus,     f ( x ) &#x2264; f ( y )   {\displaystyle f(x)\leq f(y)}
[{\displaystyle f(x)\leq f(y)}]. The same argument with the roles of     x
{\displaystyle x}  [x] and     y   {\displaystyle y}  [y] reversed shows that
f ( y ) &#x2264; f ( x )   {\displaystyle f(y)\leq f(x)}  [{\displaystyle f
(y)\leq f(x)}], so that     f ( x ) = f ( y )   {\displaystyle f(x)=f(y)}  [f
(x)=f(y)].
***** Generalizations[edit] *****
**** Weakly harmonic function[edit] ****
A function (or, more generally, a distribution) is weakly_harmonic if it
satisfies Laplace's equation
         &#x0394; f = 0    {\displaystyle \Delta f=0\,}  [\Delta f = 0\,]
in a weak sense (or, equivalently, in the sense of distributions). A weakly
harmonic function coincides almost everywhere with a strongly harmonic
function, and is in particular smooth. A weakly harmonic distribution is
precisely the distribution associated to a strongly harmonic function, and so
also is smooth. This is Weyl's_lemma.
There are other weak_formulations of Laplace's equation that are often useful.
One of which is Dirichlet's_principle, representing harmonic functions in the
Sobolev_space H1(Î©) as the minimizers of the Dirichlet_energy integral
         J ( u ) :=  &#x222B;  &#x03A9;    |  &#x2207; u   |   2    d x
      {\displaystyle J(u):=\int _{\Omega }|\nabla u|^{2}\,dx}  [J(u):
      =\int_\Omega |\nabla u|^2\, dx]
with respect to local variations, that is, all functions     u &#x2208;  H  1
( &#x03A9; )   {\displaystyle u\in H^{1}(\Omega )}  [u\in H^1(\Omega)] such
that J(u) â¤ J(u + v) holds for all     v &#x2208;  C  c   &#x221E;
( &#x03A9; ) ,   {\displaystyle v\in C_{c}^{\infty }(\Omega ),}  [v\in
C^\infty_c(\Omega),] or equivalently, for all     v &#x2208;  H  0   1
( &#x03A9; ) .   {\displaystyle v\in H_{0}^{1}(\Omega ).}  [v\in H^1_0
(\Omega).]
**** Harmonic functions on manifolds[edit] ****
Harmonic functions can be defined on an arbitrary Riemannian_manifold, using
the LaplaceâBeltrami_operator Î. In this context, a function is called
harmonic if
         &#xA0; &#x0394; f = 0.   {\displaystyle \ \Delta f=0.}  [\ \Delta f =
      0.]
Many of the properties of harmonic functions on domains in Euclidean space
carry over to this more general setting, including the mean value theorem (over
geodesic balls), the maximum principle, and the Harnack inequality. With the
exception of the mean value theorem, these are easy consequences of the
corresponding results for general linear elliptic_partial_differential
equations of the second order.
**** Subharmonic functions[edit] ****
A C2 function that satisfies Îf â¥ 0 is called subharmonic. This condition
guarantees that the maximum principle will hold, although other properties of
harmonic functions may fail. More generally, a function is subharmonic if and
only if, in the interior of any ball in its domain, its graph lies below that
of the harmonic function interpolating its boundary values on the ball.
**** Harmonic forms[edit] ****
One generalization of the study of harmonic functions is the study of harmonic
forms on Riemannian_manifolds, and it is related to the study of cohomology.
Also, it is possible to define harmonic vector-valued functions, or harmonic
maps of two Riemannian manifolds, which are critical points of a generalized
Dirichlet energy functional (this includes harmonic functions as a special
case, a result known as Dirichlet_principle). This kind of harmonic map appears
in the theory of minimal surfaces. For example, a curve, that is, a map from an
interval in R to a Riemannian manifold, is a harmonic map if and only if it is
a geodesic.
**** Harmonic maps between manifolds[edit] ****
Main article: Harmonic_map
If M and N are two Riemannian manifolds, then a harmonic_map u : M → N is
defined to be a critical point of the Dirichlet energy
         D [ u ] =   1 2    &#x222B;  M   &#x2016; d u  &#x2016;  2    d Vol
      {\displaystyle D[u]={\frac {1}{2}}\int _{M}\|du\|^{2}\,d\operatorname
      {Vol} }  [D[u] = \frac{1}{2}\int_M \|du\|^2\,d\operatorname{Vol}]
in which du : TM → TN is the differential of u, and the norm is that induced by
the metric on M and that on N on the tensor product bundle T*M â u−1 TN.
Important special cases of harmonic maps between manifolds include minimal
surfaces, which are precisely the harmonic immersions of a surface into three-
dimensional Euclidean space. More generally, minimal submanifolds are harmonic
immersions of one manifold in another. Harmonic_coordinates are a harmonic
diffeomorphism from a manifold to an open subset of a Euclidean space of the
same dimension.
***** See also[edit] *****
    * Balayage
    * Biharmonic_map
    * Dirichlet_energy
    * Dirichlet_principle
    * Dirichlet_problem
    * Harmonic_map
    * Harmonic_morphism
    * Harmonic_polynomial
    * Heat_equation
    * Laplace's_equation
    * Poisson's_equation
    * Quadrature_domains
    * Subharmonic_function
***** Notes[edit] *****
   1. ^Axler, Sheldon; Bourdon, Paul; Ramey, Wade (2001). Harmonic Function
      Theory. New York: Springer. p. 25. ISBN 0-387-95218-7.
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
   3. ^ Edward Nelson, A_proof_of_Liouville's_theorem. Proceedings of the AMS,
      1961.
***** References[edit] *****
    * Evans,_Lawrence_C. (1998), Partial Differential Equations, American
      Mathematical Society
.
Gilbarg,_David; Trudinger,_Neil, Elliptic Partial Differential Equations of
Second Order, ISBN 3-540-41160-7
.
Han, Q.; Lin, F. (2000), Elliptic Partial Differential Equations, American
Mathematical Society
.
Jost, JÃ¼rgen (2005), Riemannian Geometry and Geometric Analysis (4th ed.),
Berlin, New York: Springer-Verlag, ISBN 978-3-540-25907-7
.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Harmonic_function", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Weisstein,_Eric_W. "Harmonic_Function". MathWorld.
Harmonic_Function_Theory_by_S.Axler,_Paul_Bourdon,_and_Wade_Ramey
                                              * BNE: XX532255
                                              * BNF: cb11977733w (data)
Authority_control [Edit_this_at_Wikidata]     * GND: 4159122-7
                                              * LCCN: sh85058943
                                              * NDL: 00573755
                                              * SUDOC: 027816702

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Harmonic_function&oldid=900206845"
Categories:
    * Harmonic_functions
Hidden categories:
    * Wikipedia_articles_with_BNE_identifiers
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
    * Wikipedia_articles_with_SUDOC_identifiers
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
    * CatalÃ 
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 4 June 2019, at 03:46 (UTC).
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
