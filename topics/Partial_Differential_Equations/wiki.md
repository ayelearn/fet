The following text has been accessed from https://en.wikipedia.org/wiki/Partial_differential_equation at Thu Aug 8 22:50:37 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Partial differential equation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
A visualisation of a solution to the two-dimensional heat_equation with
temperature represented by the third dimension
In mathematics, a partial differential equation (PDE) is a differential
equation that contains unknown multivariable_functions and their partial
derivatives. PDEs are used to formulate problems involving functions of several
variables, and are either solved by hand, or used to create a computer_model. A
special case is ordinary_differential_equations (ODEs), which deal with
functions of a single variable and their derivatives.
PDEs can be used to describe a wide variety of phenomena such as sound, heat,
diffusion, electrostatics, electrodynamics, fluid_dynamics, elasticity, or
quantum_mechanics. These seemingly distinct physical phenomena can be
formalised similarly in terms of PDEs. Just as ordinary differential equations
often model one-dimensional dynamical_systems, partial differential equations
often model multidimensional_systems. PDEs find their generalisation in
stochastic_partial_differential_equations.
⁰
***** Contents *****
    * 1_Introduction
    * 2_Existence_and_uniqueness
    * 3_Notation
    * 4_Classification
          o 4.1_Equations_of_first_order
          o 4.2_Linear_equations_of_second_order
          o 4.3_Systems_of_first-order_equations_and_characteristic_surfaces
          o 4.4_Equations_of_mixed_type
          o 4.5_Infinite-order_PDEs_in_quantum_mechanics
    * 5_Analytical_solutions
          o 5.1_Separation_of_variables
          o 5.2_Method_of_characteristics
          o 5.3_Integral_transform
          o 5.4_Change_of_variables
          o 5.5_Fundamental_solution
          o 5.6_Superposition_principle
          o 5.7_Methods_for_non-linear_equations
          o 5.8_Lie_group_method
          o 5.9_Semianalytical_methods
    * 6_Numerical_solutions
          o 6.1_Finite_element_method
          o 6.2_Finite_difference_method
          o 6.3_Finite_volume_method
    * 7_See_also
    * 8_Notes
    * 9_References
    * 10_Further_reading
    * 11_External_links
***** Introduction[edit] *****
Partial differential equations (PDEs) are equations that involve rates of
change with respect to continuous_variables. For example, the position of a
rigid_body is specified by six parameters,[1] but the configuration of a fluid
is given by the continuous_distribution of several parameters, such as the
temperature, pressure, and so forth. The dynamics for the rigid body take place
in a finite-dimensional configuration_space; the dynamics for the fluid occur
in an infinite-dimensional configuration space. This distinction usually makes
PDEs much harder to solve than ordinary differential equations (ODEs), but here
again, there will be simple solutions for linear problems. Classic domains
where PDEs are used include acoustics, fluid_dynamics, electrodynamics, and
heat_transfer.
A partial differential equation (PDE) for the function u(x1,â¦ xn) is an
equation of the form
         f  (   x  1   , &#x2026;  x  n   ; u ,    &#x2202; u   &#x2202;  x  1
      , &#x2026;    &#x2202; u   &#x2202;  x  n      ;     &#x2202;  2   u
      &#x2202;  x  1   &#x2202;  x  1      , &#x2026;     &#x2202;  2   u
      &#x2202;  x  1   &#x2202;  x  n      ; &#x2026;  )  = 0.   {\displaystyle
      f\left(x_{1},\ldots x_{n};u,{\frac {\partial u}{\partial x_{1}}},\ldots
      {\frac {\partial u}{\partial x_{n}}};{\frac {\partial ^{2}u}{\partial x_
      {1}\partial x_{1}}},\ldots {\frac {\partial ^{2}u}{\partial x_{1}\partial
      x_{n}}};\ldots \right)=0.}  [{\displaystyle f\left(x_{1},\ldots x_{n};u,
      {\frac {\partial u}{\partial x_{1}}},\ldots {\frac {\partial u}{\partial
      x_{n}}};{\frac {\partial ^{2}u}{\partial x_{1}\partial x_{1}}},\ldots
      {\frac {\partial ^{2}u}{\partial x_{1}\partial x_{n}}};\ldots
      \right)=0.}]
If f is a linear_function of u and its derivatives, then the PDE is called
linear. Common examples of linear PDEs include the heat_equation, the wave
equation, Laplace's_equation, Helmholtz_equation, KleinâGordon_equation, and
Poisson's_equation.
A relatively simple PDE is
            &#x2202; u   &#x2202; x    ( x , y ) = 0.   {\displaystyle {\frac
      {\partial u}{\partial x}}(x,y)=0.}  [{\displaystyle {\frac {\partial u}
      {\partial x}}(x,y)=0.}]
This relation implies that the function u(x,y) is independent of x. However,
the equation gives no information on the function's dependence on the variable
y. Hence the general solution of this equation is
         u ( x , y ) = f ( y ) ,   {\displaystyle u(x,y)=f(y),}  [u(x,y)=f(y),]
where f is an arbitrary function of y. The analogous ordinary differential
equation is
             d  u    d  x    ( x ) = 0 ,   {\displaystyle {\frac {\mathrm {d}
      u}{\mathrm {d} x}}(x)=0,}  [{\frac {\mathrm {d} u}{\mathrm {d} x}}(x)=0,]
which has the solution
         u ( x ) = c ,   {\displaystyle u(x)=c,}  [u(x)=c,]
where c is any constant value. These two examples illustrate that general
solutions of ordinary differential equations (ODEs) involve arbitrary
constants, but solutions of PDEs involve arbitrary functions.
A solution of a PDE is generally not unique; additional conditions must
generally be specified on the boundary of the region where the solution is
defined. For instance, in the simple example above, the function f(y) can be
determined if u is specified on the line x = 0.
***** Existence and uniqueness[edit] *****
Although the issue of existence and uniqueness of solutions of ordinary
differential equations has a very satisfactory answer with the
PicardâLindelÃ¶f_theorem, that is far from the case for partial differential
equations. The CauchyâKowalevski_theorem states that the Cauchy_problem for
any partial differential equation whose coefficients are analytic in the
unknown function and its derivatives, has a locally unique analytic solution.
Although this result might appear to settle the existence and uniqueness of
solutions, there are examples of linear partial differential equations whose
coefficients have derivatives of all orders (which are nevertheless not
analytic) but which have no solutions at all: see Lewy_(1957). Even if the
solution of a partial differential equation exists and is unique, it may
nevertheless have undesirable properties. The mathematical study of these
questions is usually in the more powerful context of weak_solutions.
An example of pathological behavior is the sequence (depending upon n) of
Cauchy_problems for the Laplace_equation
             &#x2202;  2   u   &#x2202;  x  2      +     &#x2202;  2   u
      &#x2202;  y  2      = 0 ,   {\displaystyle {\frac {\partial ^{2}u}
      {\partial x^{2}}}+{\frac {\partial ^{2}u}{\partial y^{2}}}=0,}  [
      {\displaystyle {\frac {\partial ^{2}u}{\partial x^{2}}}+{\frac {\partial
      ^{2}u}{\partial y^{2}}}=0,}]
with boundary_conditions
             u ( x , 0 )    = 0 ,        &#x2202; u   &#x2202; y    ( x , 0 )
      =    sin &#x2061; n x  n   ,       {\displaystyle {\begin{aligned}u
      (x,0)&=0,\\{\frac {\partial u}{\partial y}}(x,0)&={\frac {\sin nx}
      {n}},\end{aligned}}}  [{\displaystyle {\begin{aligned}u(x,0)&=0,\\{\frac
      {\partial u}{\partial y}}(x,0)&={\frac {\sin nx}{n}},\end{aligned}}}]
where n is an integer. The derivative of u with respect to y approaches zero
uniformly in x as n increases, but the solution is
         u ( x , y ) =    sinh &#x2061; n y sin &#x2061; n x   n  2     .
      {\displaystyle u(x,y)={\frac {\sinh ny\sin nx}{n^{2}}}.}  [{\displaystyle
      u(x,y)={\frac {\sinh ny\sin nx}{n^{2}}}.}]
This solution approaches infinity if nx is not an integer multiple of Ï for
any non-zero value of y. The Cauchy problem for the Laplace equation is called
ill-posed or not well-posed, since the solution does not continuously depend on
the data of the problem. Such ill-posed problems are not usually satisfactory
for physical applications.
The existence of solutions for the NavierâStokes_equations, a partial
differential equation, is part of one of the Millennium_Prize_Problems.
***** Notation[edit] *****
In PDEs, it is common to denote partial derivatives using subscripts. That is:
          u  x   =    &#x2202; u   &#x2202; x      {\displaystyle u_{x}={\frac
      {\partial u}{\partial x}}}  [{\displaystyle u_{x}={\frac {\partial u}
      {\partial x}}}]
          u  x x   =     &#x2202;  2   u   &#x2202;  x  2        {\displaystyle
      u_{xx}={\frac {\partial ^{2}u}{\partial x^{2}}}}  [{\displaystyle u_{xx}=
      {\frac {\partial ^{2}u}{\partial x^{2}}}}]
          u  x y   =     &#x2202;  2   u   &#x2202; y  &#x2202; x    =
      &#x2202;  &#x2202; y     (    &#x2202; u   &#x2202; x    )  .
      {\displaystyle u_{xy}={\frac {\partial ^{2}u}{\partial y\,\partial x}}=
      {\frac {\partial }{\partial y}}\left({\frac {\partial u}{\partial
      x}}\right).}  [{\displaystyle u_{xy}={\frac {\partial ^{2}u}{\partial
      y\,\partial x}}={\frac {\partial }{\partial y}}\left({\frac {\partial u}
      {\partial x}}\right).}]
Especially in physics, del or nabla (â) is often used to denote spatial
derivatives, and u&#x307;, Ã¼ for time derivatives. For example, the wave
equation (described below) can be written as
            u &#x00A8;    =  c  2    &#x2207;  2   u   {\displaystyle {\ddot
      {u}}=c^{2}\nabla ^{2}u}  [{\ddot {u}}=c^{2}\nabla ^{2}u]
or
            u &#x00A8;    =  c  2   &#x0394; u   {\displaystyle {\ddot {u}}=c^
      {2}\Delta u}  [{\ddot {u}}=c^{2}\Delta u]
where Î is the Laplace_operator.
***** Classification[edit] *****
Some linear, second-order partial differential equations can be classified as
parabolic, hyperbolic and elliptic. Others, such as the EulerâTricomi
equation, have different types in different regions. The classification
provides a guide to appropriate initial and boundary conditions and to the
smoothness of the solutions.
**** Equations of first order[edit] ****
Main article: First-order_partial_differential_equation
**** Linear equations of second order[edit] ****
Assuming uxy = uyx, the general linear second-order PDE in two independent
variables has the form
         A  u  x x   + 2 B  u  x y   + C  u  y y   + &#x22EF;   (lower order
      terms)   = 0 ,   {\displaystyle Au_{xx}+2Bu_{xy}+Cu_{yy}+\cdots {\mbox{
      (lower order terms)}}=0,}  [Au_{xx}+2Bu_{xy}+Cu_{yy}+\cdots {\mbox{(lower
      order terms)}}=0,]
where the coefficients A, B, C... may depend upon x and y. If A2 + B2 + C2 > 0
over a region of the xy-plane, the PDE is second-order in that region. This
form is analogous to the equation for a conic section:
         A  x  2   + 2 B x y + C  y  2   + &#x22EF; = 0.   {\displaystyle Ax^
      {2}+2Bxy+Cy^{2}+\cdots =0.}  [Ax^{2}+2Bxy+Cy^{2}+\cdots =0.]
More precisely, replacing âx by X, and likewise for other variables (formally
this is done by a Fourier_transform), converts a constant-coefficient PDE into
a polynomial of the same degree, with the top degree (a homogeneous_polynomial,
here a quadratic_form) being most significant for the classification.
Just as one classifies conic_sections and quadratic forms into parabolic,
hyperbolic, and elliptic based on the discriminant B2 â 4AC, the same can be
done for a second-order PDE at a given point. However, the discriminant in a
PDE is given by B2 â AC due to the convention of the xy term being 2B rather
than B; formally, the discriminant (of the associated quadratic form) is (2B)2
â 4AC = 4(B2 â AC), with the factor of 4 dropped for simplicity.
   1. B2 â AC < 0 (elliptic_partial_differential_equation): Solutions of
      elliptic_PDEs are as smooth as the coefficients allow, within the
      interior of the region where the equation and solutions are defined. For
      example, solutions of Laplace's equation are analytic within the domain
      where they are defined, but solutions may assume boundary values that are
      not smooth. The motion of a fluid at subsonic speeds can be approximated
      with elliptic PDEs, and the EulerâTricomi equation is elliptic where x
      < 0.
   2. B2 â AC = 0 (parabolic_partial_differential_equation): Equations that
      are parabolic at every point can be transformed into a form analogous to
      the heat_equation by a change of independent variables. Solutions smooth
      out as the transformed time variable increases. The EulerâTricomi
      equation has parabolic type on the line where x = 0.
   3. B2 â AC > 0 (hyperbolic_partial_differential_equation): hyperbolic
      equations retain any discontinuities of functions or derivatives in the
      initial data. An example is the wave equation. The motion of a fluid at
      supersonic speeds can be approximated with hyperbolic PDEs, and the
      EulerâTricomi equation is hyperbolic where x > 0.
If there are n independent variables x1, x2,â¦ xn, a general linear partial
differential equation of second order has the form
         L u =  &#x2211;  i = 1   n    &#x2211;  j = 1   n    a  i , j
      &#x2202;  2   u   &#x2202;  x  i   &#x2202;  x  j        &#xA0;plus
      lower-order terms  = 0.   {\displaystyle Lu=\sum _{i=1}^{n}\sum _{j=1}^
      {n}a_{i,j}{\frac {\partial ^{2}u}{\partial x_{i}\partial x_{j}}}\quad
      {\text{ plus lower-order terms}}=0.}  [{\displaystyle Lu=\sum _{i=1}^
      {n}\sum _{j=1}^{n}a_{i,j}{\frac {\partial ^{2}u}{\partial x_{i}\partial
      x_{j}}}\quad {\text{ plus lower-order terms}}=0.}]
The classification depends upon the signature of the eigenvalues of the
coefficient matrix ai,j.
   1. Elliptic: the eigenvalues are all positive or all negative.
   2. Parabolic: the eigenvalues are all positive or all negative, save one
      that is zero.
   3. Hyperbolic: there is only one negative eigenvalue and all the rest are
      positive, or there is only one positive eigenvalue and all the rest are
      negative.
   4. Ultrahyperbolic: there is more than one positive eigenvalue and more than
      one negative eigenvalue, and there are no zero eigenvalues. There is only
      a limited theory for ultrahyperbolic equations (Courant and Hilbert,
      1962).
**** Systems of first-order equations and characteristic surfaces[edit] ****
The classification of partial differential equations can be extended to systems
of first-order equations, where the unknown u is now a vector with m
components, and the coefficient matrices AÎ½ are m by m matrices for Î½ = 1,
2,â¦ n. The partial differential equation takes the form
         L u =  &#x2211;  &#x03BD; = 1   n    A  &#x03BD;      &#x2202; u
      &#x2202;  x  &#x03BD;      + B = 0 ,   {\displaystyle Lu=\sum _{\nu =1}^
      {n}A_{\nu }{\frac {\partial u}{\partial x_{\nu }}}+B=0,}  [Lu=\sum _{\nu
      =1}^{n}A_{\nu }{\frac {\partial u}{\partial x_{\nu }}}+B=0,]
where the coefficient matrices AÎ½ and the vector B may depend upon x and u. If
a hypersurface S is given in the implicit form
         &#x03C6; (  x  1   ,  x  2   , &#x2026;  x  n   ) = 0 ,
      {\displaystyle \varphi (x_{1},x_{2},\ldots x_{n})=0,}  [{\displaystyle
      \varphi (x_{1},x_{2},\ldots x_{n})=0,}]
where Ï has a non-zero gradient, then S is a characteristic surface for the
operator L at a given point if the characteristic form vanishes:
         Q  (     &#x2202; &#x03C6;   &#x2202;  x  1      , &#x2026;
      &#x2202; &#x03C6;   &#x2202;  x  n       )  = det  [   &#x2211;  &#x03BD;
      = 1   n    A  &#x03BD;      &#x2202; &#x03C6;   &#x2202;  x  &#x03BD;
      ]  = 0.    {\displaystyle Q\left({\frac {\partial \varphi }{\partial x_
      {1}}},\ldots {\frac {\partial \varphi }{\partial x_{n}}}\right)=\det
      \left[\sum _{\nu =1}^{n}A_{\nu }{\frac {\partial \varphi }{\partial x_
      {\nu }}}\right]=0.\,}  [{\displaystyle Q\left({\frac {\partial \varphi }
      {\partial x_{1}}},\ldots {\frac {\partial \varphi }{\partial x_
      {n}}}\right)=\det \left[\sum _{\nu =1}^{n}A_{\nu }{\frac {\partial
      \varphi }{\partial x_{\nu }}}\right]=0.\,}]
The geometric interpretation of this condition is as follows: if data for u are
prescribed on the surface S, then it may be possible to determine the normal
derivative of u on S from the differential equation. If the data on S and the
differential equation determine the normal derivative of u on S, then S is non-
characteristic. If the data on S and the differential equation do not determine
the normal derivative of u on S, then the surface is characteristic, and the
differential equation restricts the data on S: the differential equation is
internal to S.
   1. A first-order system Lu = 0 is elliptic if no surface is characteristic
      for L: the values of u on S and the differential equation always
      determine the normal derivative of u on S.
   2. A first-order system is hyperbolic at a point if there is a spacelike
      surface S with normal Î¾ at that point. This means that, given any non-
      trivial vector Î· orthogonal to Î¾, and a scalar multiplier Î», the
      equation Q(Î»Î¾ + Î·) = 0 has m real roots Î»1, Î»2,â¦ Î»m. The system
      is strictly hyperbolic if these roots are always distinct. The
      geometrical interpretation of this condition is as follows: the
      characteristic form Q(Î¶) = 0 defines a cone (the normal cone) with
      homogeneous coordinates Î¶. In the hyperbolic case, this cone has m
      sheets, and the axis Î¶ = Î»Î¾ runs inside these sheets: it does not
      intersect any of them. But when displaced from the origin by Î·, this
      axis intersects every sheet. In the elliptic case, the normal cone has no
      real sheets.
**** Equations of mixed type[edit] ****
If a PDE has coefficients that are not constant, it is possible that it will
not belong to any of these categories but rather be of mixed type. A simple but
important example is the EulerâTricomi_equation
          u  x x   = x  u  y y   ,   {\displaystyle u_{xx}=xu_{yy},}  [
      {\displaystyle u_{xx}=xu_{yy},}]
which is called elliptic-hyperbolic because it is elliptic in the region x < 0,
hyperbolic in the region x > 0, and degenerate parabolic on the line x = 0.
**** Infinite-order PDEs in quantum mechanics[edit] ****
In the phase_space_formulation of quantum mechanics, one may consider the
quantum_Hamilton's_equations for trajectories of quantum particles. These
equations are infinite-order PDEs. However, in the semiclassical expansion, one
has a finite system of ODEs at any fixed order of Ä§. The evolution equation of
the Wigner_function is also an infinite-order PDE. The quantum trajectories are
quantum_characteristics, with the use of which one could calculate the
evolution of the Wigner function.
***** Analytical solutions[edit] *****
**** Separation of variables[edit] ****
Main article: Separable_partial_differential_equation
Linear PDEs can be reduced to systems of ordinary differential equations by the
important technique of separation of variables. This technique rests on a
characteristic of solutions to differential equations: if one can find any
solution that solves the equation and satisfies the boundary conditions, then
it is the solution (this also applies to ODEs). We assume as an ansatz that the
dependence of a solution on the parameters space and time can be written as a
product of terms that each depend on a single parameter, and then see if this
can be made to solve the problem.[2]
In the method of separation of variables, one reduces a PDE to a PDE in fewer
variables, which is an ordinary differential equation if in one variable â
these are in turn easier to solve.
This is possible for simple PDEs, which are called separable_partial
differential_equations, and the domain is generally a rectangle (a product of
intervals). Separable PDEs correspond to diagonal_matrices â thinking of "the
value for fixed x" as a coordinate, each coordinate can be understood
separately.
This generalizes to the method_of_characteristics, and is also used in integral
transforms.
**** Method of characteristics[edit] ****
Main article: Method_of_characteristics
In special cases, one can find characteristic curves on which the equation
reduces to an ODE â changing coordinates in the domain to straighten these
curves allows separation of variables, and is called the method_of
characteristics.
More generally, one may find characteristic surfaces.
**** Integral transform[edit] ****
An integral_transform may transform the PDE to a simpler one, in particular, a
separable PDE. This corresponds to diagonalizing an operator.
An important example of this is Fourier_analysis, which diagonalizes the heat
equation using the eigenbasis of sinusoidal waves.
If the domain is finite or periodic, an infinite sum of solutions such as a
Fourier_series is appropriate, but an integral of solutions such as a Fourier
integral is generally required for infinite domains. The solution for a point
source for the heat equation given above is an example of the use of a Fourier
integral.
**** Change of variables[edit] ****
Often a PDE can be reduced to a simpler form with a known solution by a
suitable change_of_variables. For example, the BlackâScholes PDE
            &#x2202; V   &#x2202; t    +    1 2     &#x03C3;  2    S  2
      &#x2202;  2   V   &#x2202;  S  2      + r S    &#x2202; V   &#x2202; S
      &#x2212; r V = 0   {\displaystyle {\frac {\partial V}{\partial t}}+
      {\tfrac {1}{2}}\sigma ^{2}S^{2}{\frac {\partial ^{2}V}{\partial S^
      {2}}}+rS{\frac {\partial V}{\partial S}}-rV=0}  [{\displaystyle {\frac
      {\partial V}{\partial t}}+{\tfrac {1}{2}}\sigma ^{2}S^{2}{\frac {\partial
      ^{2}V}{\partial S^{2}}}+rS{\frac {\partial V}{\partial S}}-rV=0}]
is reducible to the heat_equation
            &#x2202; u   &#x2202; &#x03C4;    =     &#x2202;  2   u   &#x2202;
      x  2        {\displaystyle {\frac {\partial u}{\partial \tau }}={\frac
      {\partial ^{2}u}{\partial x^{2}}}}  [{\frac {\partial u}{\partial \tau
      }}={\frac {\partial ^{2}u}{\partial x^{2}}}]
by the change of variables (for complete details see Solution_of_the_Black
Scholes_Equation at the Wayback_Machine (archived April 11, 2008))
             V ( S , t )    = K v ( x , &#x03C4; ) ,     x    = ln &#x2061;
      (    S K    )  ,     &#x03C4;    =    1 2     &#x03C3;  2   ( T &#x2212;
      t ) ,     v ( x , &#x03C4; )    =  e  &#x2212; &#x03B1; x &#x2212;
      &#x03B2; &#x03C4;   u ( x , &#x03C4; ) .       {\displaystyle {\begin
      {aligned}V(S,t)&=Kv(x,\tau ),\\[5px]x&=\ln \left({\tfrac {S}
      {K}}\right),\\[5px]\tau &={\tfrac {1}{2}}\sigma ^{2}(T-t),\\[5px]v(x,\tau
      )&=e^{-\alpha x-\beta \tau }u(x,\tau ).\end{aligned}}}  [{\displaystyle
      {\begin{aligned}V(S,t)&=Kv(x,\tau ),\\[5px]x&=\ln \left({\tfrac {S}
      {K}}\right),\\[5px]\tau &={\tfrac {1}{2}}\sigma ^{2}(T-t),\\[5px]v(x,\tau
      )&=e^{-\alpha x-\beta \tau }u(x,\tau ).\end{aligned}}}]
**** Fundamental solution[edit] ****
Main article: Fundamental_solution
Inhomogeneous equations can often be solved (for constant coefficient PDEs,
always be solved) by finding the fundamental_solution (the solution for a point
source), then taking the convolution with the boundary conditions to get the
solution.
This is analogous in signal_processing to understanding a filter by its impulse
response.
**** Superposition principle[edit] ****
Further information: Superposition_principle
The superposition principle applies to any linear system, including linear
systems of PDEs. A common visualization of this concept is the interaction of
two waves in phase being combined to result in a greater amplitude, for example
sin x + sin x = 2 sin x. The same principle can be observed in PDEs where the
solutions may be real or complex and additive. superposition If u1 and u2 are
solutions of linear PDE in some function space R, then u = c1u1 + c2u2 with any
constants c1 and c2 are also a solution of that PDE in the same function space.
**** Methods for non-linear equations[edit] ****
See also: nonlinear_partial_differential_equation
There are no generally applicable methods to solve nonlinear PDEs. Still,
existence and uniqueness results (such as the CauchyâKowalevski_theorem) are
often possible, as are proofs of important qualitative and quantitative
properties of solutions (getting these results is a major part of analysis).
Computational solution to the nonlinear PDEs, the split-step_method, exist for
specific equations like nonlinear_SchrÃ¶dinger_equation.
Nevertheless, some techniques can be used for several types of equations. The
h-principle is the most powerful method to solve underdetermined equations. The
RiquierâJanet_theory is an effective method for obtaining information about
many analytic overdetermined systems.
The method_of_characteristics can be used in some very special cases to solve
partial differential equations.
In some cases, a PDE can be solved via perturbation_analysis in which the
solution is considered to be a correction to an equation with a known solution.
Alternatives are numerical_analysis techniques from simple finite_difference
schemes to the more mature multigrid and finite_element_methods. Many
interesting problems in science and engineering are solved in this way using
computers, sometimes high performance supercomputers.
**** Lie group method[edit] ****
From 1870 Sophus_Lie's work put the theory of differential equations on a more
satisfactory foundation. He showed that the integration theories of the older
mathematicians can, by the introduction of what are now called Lie_groups, be
referred, to a common source; and that ordinary differential equations which
admit the same infinitesimal_transformations present comparable difficulties of
integration. He also emphasized the subject of transformations_of_contact.
A general approach to solving PDEs uses the symmetry property of differential
equations, the continuous infinitesimal_transformations of solutions to
solutions (Lie_theory). Continuous group_theory, Lie_algebras and differential
geometry are used to understand the structure of linear and nonlinear partial
differential equations for generating integrable equations, to find its Lax
pairs, recursion operators, BÃ¤cklund_transform and finally finding exact
analytic solutions to the PDE.
Symmetry methods have been recognized to study differential equations arising
in mathematics, physics, engineering, and many other disciplines.
**** Semianalytical methods[edit] ****
The Adomian_decomposition_method, the Lyapunov artificial small parameter
method, and He's homotopy_perturbation_method are all special cases of the more
general homotopy_analysis_method. These are series expansion methods, and
except for the Lyapunov method, are independent of small physical parameters as
compared to the well known perturbation_theory, thus giving these methods
greater flexibility and solution generality.
***** Numerical solutions[edit] *****
The three most widely used numerical methods to solve PDEs are the finite
element_method (FEM), finite_volume_methods (FVM) and finite_difference_methods
(FDM), as well other kind of methods called Meshfree_methods, which were made
to solve problems where the before mentioned methods are limited. The FEM has a
prominent position among these methods and especially its exceptionally
efficient higher-order version hp-FEM. Other hybrid versions of FEM and
Meshfree methods include the generalized finite element method (GFEM), extended
finite_element_method (XFEM), spectral_finite_element_method (SFEM), meshfree
finite_element_method, discontinuous_Galerkin_finite_element_method (DGFEM),
Element-Free_Galerkin_Method (EFGM), Interpolating_Element-Free_Galerkin_Method
(IEFGM), etc.
**** Finite element method[edit] ****
Main article: Finite_element_method
The finite element method (FEM) (its practical application often known as
finite element analysis (FEA)) is a numerical technique for finding approximate
solutions of partial differential equations (PDE) as well as of integral
equations. The solution approach is based either on eliminating the
differential equation completely (steady state problems), or rendering the PDE
into an approximating system of ordinary differential equations, which are then
numerically integrated using standard techniques such as Euler's method,
RungeâKutta, etc.
**** Finite difference method[edit] ****
Main article: Finite_difference_method
Finite-difference methods are numerical methods for approximating the solutions
to differential equations using finite_difference equations to approximate
derivatives.
**** Finite volume method[edit] ****
Main article: Finite_volume_method
Similar to the finite difference method or finite element method, values are
calculated at discrete places on a meshed geometry. "Finite volume" refers to
the small volume surrounding each node point on a mesh. In the finite volume
method, surface integrals in a partial differential equation that contain a
divergence term are converted to volume integrals, using the divergence
theorem. These terms are then evaluated as fluxes at the surfaces of each
finite volume. Because the flux entering a given volume is identical to that
leaving the adjacent volume, these methods conserve mass by design.
***** See also[edit] *****
    * Dirichlet_boundary_condition
    * Jet_bundle
    * Laplace_transform_applied_to_differential_equations
    * List_of_dynamical_systems_and_differential_equations_topics
    * Matrix_differential_equation
    * Neumann_boundary_condition
    * Numerical_partial_differential_equations
    * Partial_differential_algebraic_equation
    * Recurrence_relation
    * Robin_boundary_condition
    * Stochastic_processes_and_boundary_value_problems
***** Notes[edit] *****
   1. ^Sciavicco, Lorenzo; Siciliano, Bruno (2001-02-19). Modelling_and_Control
      of_Robot_Manipulators. Springer Science & Business Media.
      ISBN 9781852332211.
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
   3. ^Gershenfeld, Neil (2000). The nature of mathematical modeling (Reprinted
      (with corr.) ed.). Cambridge: Cambridge Univ. Press. p. 27.
      ISBN 0521570956.
***** References[edit] *****
    * Adomian, G. (1994). Solving_Frontier_problems_of_Physics:_The
      decomposition_method. Kluwer Academic Publishers.
Courant, R. & Hilbert, D. (1962), Methods_of_Mathematical_Physics, II, New
York: Wiley-Interscience
.
Evans,_L._C. (1998), Partial Differential Equations, Providence: American
Mathematical Society, ISBN 0-8218-0772-2
.
HolubovÃ¡, Pavel DrÃ¡bek ; Gabriela (2007). Elements of partial differential
equations ([Online-Ausg.]. ed.). Berlin: de Gruyter. ISBN 9783110191240.
Ibragimov, Nail H (1993), CRC Handbook of Lie Group Analysis of Differential
Equations Vol. 1-3, Providence: CRC-Press, ISBN 0-8493-4488-3
.
John,_F. (1982), Partial Differential Equations (4th ed.), New York: Springer-
Verlag, ISBN 0-387-90609-6
.
Jost, J. (2002), Partial Differential Equations, New York: Springer-Verlag,
ISBN 0-387-95428-7
.
Lewy, Hans (1957), "An example of a smooth linear partial differential equation
without solution", Annals of Mathematics, Second Series, 66 (1): 155â158,
doi:10.2307/1970121
.
Liao,_S.J. (2003), Beyond Perturbation: Introduction to the Homotopy Analysis
Method, Boca Raton: Chapman & Hall/ CRC Press, ISBN 1-58488-407-X
Olver,_P.J. (1995), Equivalence, Invariants and Symmetry, Cambridge Press
.
Petrovskii,_I._G. (1967), Partial Differential Equations, Philadelphia: W. B.
Saunders Co.
.
Pinchover, Y. & Rubinstein, J. (2005), An Introduction to Partial Differential
Equations, New York: Cambridge University Press, ISBN 0-521-84886-5
.
Polyanin, A. D. (2002), Handbook of Linear Partial Differential Equations for
Engineers and Scientists, Boca Raton: Chapman & Hall/CRC Press, ISBN 1-58488-
299-9
.
Polyanin, A. D. & Zaitsev, V. F. (2004), Handbook of Nonlinear Partial
Differential Equations, Boca Raton: Chapman & Hall/CRC Press, ISBN 1-58488-355-
3
.
Polyanin, A. D.; Zaitsev, V. F. & Moussiaux, A. (2002), Handbook of First Order
Partial Differential Equations, London: Taylor & Francis, ISBN 0-415-27267-X
.
RoubÃ­Äek, T. (2013), Nonlinear Partial Differential Equations with
Applications (2nd ed.), Basel, Boston, Berlin: BirkhÃ¤user, doi:10.1007/978-3-
0348-0513-1, ISBN 978-3-0348-0512-4, MR 3014456
Solin, P. (2005), Partial Differential Equations and the Finite Element Method,
Hoboken, NJ: J. Wiley & Sons, ISBN 0-471-72070-4
.
Solin, P.; Segeth, K. & Dolezel, I. (2003), Higher-Order Finite Element
Methods, Boca Raton: Chapman & Hall/CRC Press, ISBN 1-58488-438-X
.
Stephani, H. (1989), Differential Equations: Their Solution Using Symmetries.
Edited by M. MacCallum, Cambridge University Press
.
Wazwaz, Abdul-Majid (2009). Partial Differential Equations and Solitary Waves
Theory. Higher Education Press. ISBN 978-3-642-00251-9.
Wazwaz, Abdul-Majid (2002). Partial Differential Equations Methods and
Applications. A.A. Balkema. ISBN 90-5809-369-7.
Zwillinger, D. (1997), Handbook of Differential Equations (3rd ed.), Boston:
Academic Press, ISBN 0-12-784395-7
.
Fakher Iqbal, Partial Differential Equations (Radial Basis function) - Thermal
Colony Muzaffargarh (2019)
Gershenfeld,_N. (1999), The Nature of Mathematical Modeling (1st ed.), New
York: Cambridge University Press, New York, NY, USA, ISBN 0-521-57095-6
.
Krasil'shchik, I.S. & Vinogradov, A.M., Eds. (1999), Symmetries and
Conserwation Laws for Differential Equations of Mathematical Physics, American
Mathematical Society, Providence, Rhode Island, USA, ISBN 0-8218-0958-X
.
Krasil'shchik, I.S.; Lychagin, V.V. & Vinogradov, A.M. (1986), Geometry of Jet
Spaces and Nonlinear Partial Differential Equations, Gordon and Breach Science
Publishers, New York, London, Paris, Montreux, Tokyo, ISBN 2-88124-051-8
.
Vinogradov, A.M. (2001), Cohomological Analysis of Partial Differential
Equations and Secondary Calculus, American Mathematical Society, Providence,
Rhode Island, USA, ISBN 0-8218-2922-X
.
***** Further reading[edit] *****
    * Cajori,_Florian (1928). "The_Early_History_of_Partial_Differential
      Equations_and_of_Partial_Differentiation_and_Integration" (PDF). The
      American Mathematical Monthly. 35 (9): 459â467. doi:10.2307/2298771.
***** External links[edit] *****
Partial differential equationat Wikipedia's sister_projects
    * Media from Wikimedia Commons
    * Quotations from Wikiquote
    * Textbooks from Wikibooks
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Differential_equation,_partial",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Partial_Differential_Equations:_Exact_Solutions at EqWorld: The World of
Mathematical Equations.
Partial_Differential_Equations:_Index at EqWorld: The World of Mathematical
Equations.
Partial_Differential_Equations:_Methods at EqWorld: The World of Mathematical
Equations.
Example_problems_with_solutions at exampleproblems.com
Partial_Differential_Equations at mathworld.wolfram.com
Partial_Differential_Equations with Mathematica
Partial_Differential_Equations in Cleve Moler: Numerical Computing with MATLAB
Partial_Differential_Equations at nag.com
Sanderson, Grant (April 21, 2019). "But_what_is_a_partial_differential
equation?". 3Blue1Brown – via YouTube.
    * v
    * t
    * e
Differential_equations
                                           * Differential_operator
                                           * Notation_for_differentiation
                                           * Ordinary
                                           * Partial
               Operations                  * Differential-algebraic
                                           * Integro-differential
                                           * Fractional
                                           * Linear
                                           * Non-linear
                                           * Dependent_and_independent_variables
Classification                             * Homogeneous
                                           * Nonhomogeneous
                                           * Coupled
               Attributes of variables     * Decoupled
                                           * Order
                                           * Degree
                                           * Autonomous
                                           * Exact_differential_equation
                                           * Complex_differential_equation
                                           * Difference (discrete analogue)
               Relation to processes       * stochastic
                                           * Delay
                            * PicardâLindelÃ¶f_theorem (existence and uniqueness)
                            * Wronskian
                            * Phase_portrait
                            * Phase_space
                            * Lyapunov_stability
               Solution     * Asymptotic_stability
               topics       * Exponential_stability
                            * Rate_of_convergence
                            * Series_solutions
                            * Integral solutions
                            * Numerical_integration
                            * Dirac_delta_function
Solutions                   * Inspection
                            * Separation_of_variables                                    [Elmer-pump-
                            * Method_of_undetermined_coefficients                        heatequation.png]
                            * Variation_of_parameters
                            * Integrating_factor
                            * Integral_transforms
               Solution     * Euler_method
               methods      * Finite_difference_method
                            * CrankâNicolson_method
                            * RungeâKutta_methods
                            * Finite_element_method
                            * Finite_volume_method
                            * Galerkin_method
                            * Perturbation_theory
                   * Astronomy
                   * Physics
                   * Continuum_mechanics
                   * Chaos_theory
Applications       * Chemistry
                   * Dynamical_system
                   * Economics
                   * Biology
                   * Geology
                   * Population_dynamics
                   * Isaac_Newton
                   * Gottfried_Wilhelm_Leibniz
                   * Leonhard_Euler
                   * Jacob_Bernoulli
                   * Ãmile_Picard
                   * JÃ³zef_Maria_Hoene-WroÅski
Mathematicians     * Ernst_LindelÃ¶f
                   * Rudolf_Lipschitz
                   * Joseph-Louis_Lagrange
                   * Augustin-Louis_Cauchy
                   * John_Crank
                   * Phyllis_Nicolson
                   * Carl_David_TolmÃ©_Runge
                   * Martin_Kutta
Authority_control [Edit_this_at_Wikidata]     * GND: 4044779-0
                                              * NDL: 00563088

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Partial_differential_equation&oldid=906967870"
Categories:
    * Multivariable_calculus
    * Differential_equations
    * Partial_differential_equations
    * Concepts_in_physics
Hidden categories:
    * Webarchive_template_wayback_links
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_NDL_identifiers
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
    * Wikibooks
    * Wikiquote
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
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
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Simple_English
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 19 July 2019, at 14:51 (UTC).
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
