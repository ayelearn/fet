The following text has been accessed from https://en.wikipedia.org/wiki/Separation_of_variables at Fri Aug 9 00:03:13 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Separation of variables ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Differential_equations
[NavierâStokes_differential_equations_used_to_simulate_airflow_around_an
obstruction]
NavierâStokes_differential_equations used to simulate airflow around an
obstruction.
Scope
    * Natural_sciences
    * Engineering
    * Astronomy
    * Physics
    * Chemistry
    *
      Biology
    * Geology
Applied_mathematics
    * Continuum_mechanics
    * Chaos_theory
    * Dynamical_systems
Social_sciences
    * Economics
    * Population_dynamics
Classification
Types
    * Ordinary
    * Partial
    * Differential-algebraic
    * Integro-differential
    * Fractional
    * Linear
    * Non-linear
By variable type
    * Dependent_and_independent_variables
    * Autonomous
    * Complex
    * Coupled / Decoupled
    * Exact
    * Homogeneous / Nonhomogeneous
Features
    * Order
    * Operator
    * Notation
Relation to processes
    * Difference_(discrete_analogue)
    * Stochastic
    * Delay
Solution
General topics
    * PicardâLindelÃ¶f_theorem
    * Wronskian
    * Phase_portrait
    * Phase_space
    * Lyapunov / Asymptotic / Exponential_stability
    * Rate_of_convergence
    * Series / Integral solutions
    * Numerical_integration
    * Dirac_delta_function
Solution methods
    * Inspection
    * Method_of_characteristics
    *
      Euler
    * Exponential_response_formula
    * Finite_difference (CrankâNicolson)
    * Finite_element
          o Infinite_element
    * Finite_volume
    * Galerkin
          o PetrovâGalerkin
    * Integrating_factor
    * Integral_transforms
    * Perturbation_theory
    * RungeâKutta
    * Separation of variables
    * Undetermined_coefficients
    * Variation_of_parameters
People
    * Isaac_Newton
    * Gottfried_Leibniz
    * Leonhard_Euler
    * Ãmile_Picard
    * JÃ³zef_Maria_Hoene-WroÅski
    * Ernst_LindelÃ¶f
    * Rudolf_Lipschitz
    * Augustin-Louis_Cauchy
    * John_Crank
    * Phyllis_Nicolson
    * Carl_David_TolmÃ©_Runge
    * Martin_Kutta
    * v
    * t
    * e
In mathematics, separation of variables (also known as the Fourier method) is
any of several methods for solving ordinary and partial_differential_equations,
in which algebra allows one to rewrite an equation so that each of two
variables occurs on a different side of the equation.
⁰
***** Contents *****
    * 1_Ordinary_differential_equations_(ODE)
          o 1.1_Alternative_notation
          o 1.2_Example
    * 2_Partial_differential_equations
          o 2.1_Example:_homogeneous_case
          o 2.2_Example:_nonhomogeneous_case
          o 2.3_Example:_mixed_derivatives
          o 2.4_Curvilinear_coordinates
    * 3_Matrices
    * 4_See_also
    * 5_References
    * 6_External_links
***** Ordinary differential equations (ODE)[edit] *****
Suppose a differential equation can be written in the form
           d  d x    f ( x ) = g ( x ) h ( f ( x ) )   {\displaystyle {\frac
      {d}{dx}}f(x)=g(x)h(f(x))}  [{\frac  {d}{dx}}f(x)=g(x)h(f(x))]
which we can write more simply by letting     y = f ( x )   {\displaystyle y=f
(x)}  [y=f(x)]:
            d y   d x    = g ( x ) h ( y ) .   {\displaystyle {\frac {dy}
      {dx}}=g(x)h(y).}  [{\frac  {dy}{dx}}=g(x)h(y).]
As long as h(y) â  0, we can rearrange terms to obtain:
            d y   h ( y )    = g ( x )  d x ,   {\displaystyle {dy \over h
      (y)}=g(x)\,dx,}  [{\displaystyle {dy \over h(y)}=g(x)\,dx,}]
so that the two variables x and y have been separated. dx (and dy) can be
viewed, at a simple level, as just a convenient notation, which provides a
handy mnemonic aid for assisting with manipulations. A formal definition of dx
as a differential_(infinitesimal) is somewhat advanced.
**** Alternative notation[edit] ****
Those who dislike Leibniz's_notation may prefer to write this as
           1  h ( y )       d y   d x    = g ( x ) ,   {\displaystyle {\frac
      {1}{h(y)}}{\frac {dy}{dx}}=g(x),}  [{\frac  {1}{h(y)}}{\frac  {dy}{dx}}=g
      (x),]
but that fails to make it quite as obvious why this is called "separation of
variables". Integrating both sides of the equation with respect to     x
{\displaystyle x}  [x], we have
         &#x222B;   1  h ( y )       d y   d x     d x = &#x222B; g ( x )  d x
      ,   ( 1 )   {\displaystyle \int {\frac {1}{h(y)}}{\frac {dy}
      {dx}}\,dx=\int g(x)\,dx,\qquad \qquad (1)}  [\int {\frac  {1}{h(y)}}
      {\frac  {dy}{dx}}\,dx=\int g(x)\,dx,\qquad \qquad (1)]
or equivalently,
         &#x222B;   1  h ( y )     d y = &#x222B; g ( x )  d x   {\displaystyle
      \int {\frac {1}{h(y)}}\,dy=\int g(x)\,dx}  [\int {\frac  {1}{h
      (y)}}\,dy=\int g(x)\,dx]
because of the substitution_rule_for_integrals.
If one can evaluate the two integrals, one can find a solution to the
differential equation. Observe that this process effectively allows us to treat
the derivative        d y   d x      {\displaystyle {\frac {dy}{dx}}}  [{\frac
{dy}{dx}}] as a fraction which can be separated. This allows us to solve
separable differential equations more conveniently, as demonstrated in the
example below.
(Note that we do not need to use two constants_of_integration, in equation (1)
as in
         &#x222B;   1  h ( y )     d y +  C  1   = &#x222B; g ( x )  d x +  C
      2   ,   {\displaystyle \int {\frac {1}{h(y)}}\,dy+C_{1}=\int g(x)\,dx+C_
      {2},}  [\int {\frac  {1}{h(y)}}\,dy+C_{1}=\int g(x)\,dx+C_{2},]
because a single constant     C =  C  2   &#x2212;  C  1     {\displaystyle
C=C_{2}-C_{1}}  [C=C_{2}-C_{1}] is equivalent.)
**** Example[edit] ****
Population growth is often modeled by the differential equation
            d P   d t    = k P  (  1 &#x2212;   P K    )    {\displaystyle
      {\frac {dP}{dt}}=kP\left(1-{\frac {P}{K}}\right)}  [{\frac  {dP}
      {dt}}=kP\left(1-{\frac  {P}{K}}\right)]
where     P   {\displaystyle P}  [P] is the population with respect to time
t   {\displaystyle t}  [t],     k   {\displaystyle k}  [k] is the rate of
growth, and     K   {\displaystyle K}  [K] is the carrying_capacity of the
environment.
Separation of variables may be used to solve this differential equation.
                 d P   d t    = k P  (  1 &#x2212;   P K    )        &#x222B;
      d P   P  (  1 &#x2212;   P K    )     = &#x222B; k  d t
      {\displaystyle {\begin{aligned}&{\frac {dP}{dt}}=kP\left(1-{\frac {P}
      {K}}\right)\\[5pt]&\int {\frac {dP}{P\left(1-{\frac {P}{K}}\right)}}=\int
      k\,dt\end{aligned}}}  [{\displaystyle {\begin{aligned}&{\frac {dP}
      {dt}}=kP\left(1-{\frac {P}{K}}\right)\\[5pt]&\int {\frac {dP}{P\left(1-
      {\frac {P}{K}}\right)}}=\int k\,dt\end{aligned}}}]
To evaluate the integral on the left side, we simplify the fraction
           1  P  (  1 &#x2212;   P K    )     =   K  P  (  K &#x2212; P  )
      {\displaystyle {\frac {1}{P\left(1-{\frac {P}{K}}\right)}}={\frac {K}
      {P\left(K-P\right)}}}  [{\frac  {1}{P\left(1-{\frac  {P}{K}}\right)}}=
      {\frac  {K}{P\left(K-P\right)}}]
and then, we decompose the fraction into partial fractions
           K  P ( K &#x2212; P )    =   1 P   +   1  K &#x2212; P
      {\displaystyle {\frac {K}{P(K-P)}}={\frac {1}{P}}+{\frac {1}{K-P}}}  [
      {\displaystyle {\frac {K}{P(K-P)}}={\frac {1}{P}}+{\frac {1}{K-P}}}]
Thus we have
               &#x222B;  (    1 P   +   1  K &#x2212; P     )   d P = &#x222B;
      k  d t      ln &#x2061;   |    P    |   &#x2212; ln &#x2061;   |    K
      &#x2212; P    |   = k t + C      ln &#x2061;   |    K &#x2212; P    |
      &#x2212; ln &#x2061;   |    P    |   = &#x2212; k t &#x2212; C      ln
      &#x2061;   |            K &#x2212; P          P         |   = &#x2212; k
      t &#x2212; C        |        K &#x2212; P  P       |   =  e  &#x2212; k t
      &#x2212; C          |        K &#x2212; P  P       |   =  e  &#x2212; C
      e  &#x2212; k t           K &#x2212; P  P   = &#x00B1;  e  &#x2212; C
      e  &#x2212; k t        Let&#xA0;    A = &#x00B1;  e  &#x2212; C   .
      K &#x2212; P  P   = A  e  &#x2212; k t          K P   &#x2212; 1 = A  e
      &#x2212; k t          K P   = 1 + A  e  &#x2212; k t          P K   =   1
      1 + A  e  &#x2212; k t           P =   K  1 + A  e  &#x2212; k t
      {\displaystyle {\begin{aligned}&\int \left({\frac {1}{P}}+{\frac {1}{K-
      P}}\right)\,dP=\int k\,dt\\[6pt]&\ln {\begin{vmatrix}P\end{vmatrix}}-\ln
      {\begin{vmatrix}K-P\end{vmatrix}}=kt+C\\[6pt]&\ln {\begin{vmatrix}K-P\end
      {vmatrix}}-\ln {\begin{vmatrix}P\end{vmatrix}}=-kt-C\\[6pt]&\ln {\begin
      {vmatrix}{\cfrac {K-P}{P}}\end{vmatrix}}=-kt-C\\[6pt]&{\begin{vmatrix}
      {\dfrac {K-P}{P}}\end{vmatrix}}=e^{-kt-C}\\[6pt]&{\begin{vmatrix}{\dfrac
      {K-P}{P}}\end{vmatrix}}=e^{-C}e^{-kt}\\[6pt]&{\frac {K-P}{P}}=\pm e^{-
      C}e^{-kt}\\[6pt]{\text{Let }}&A=\pm e^{-C}.\\[6pt]&{\frac {K-P}{P}}=Ae^{-
      kt}\\[6pt]&{\frac {K}{P}}-1=Ae^{-kt}\\[6pt]&{\frac {K}{P}}=1+Ae^{-kt}\\
      [6pt]&{\frac {P}{K}}={\frac {1}{1+Ae^{-kt}}}\\[6pt]&P={\frac {K}{1+Ae^{-
      kt}}}\end{aligned}}}  [{\displaystyle {\begin{aligned}&\int \left({\frac
      {1}{P}}+{\frac {1}{K-P}}\right)\,dP=\int k\,dt\\[6pt]&\ln {\begin
      {vmatrix}P\end{vmatrix}}-\ln {\begin{vmatrix}K-P\end{vmatrix}}=kt+C\\
      [6pt]&\ln {\begin{vmatrix}K-P\end{vmatrix}}-\ln {\begin{vmatrix}P\end
      {vmatrix}}=-kt-C\\[6pt]&\ln {\begin{vmatrix}{\cfrac {K-P}{P}}\end
      {vmatrix}}=-kt-C\\[6pt]&{\begin{vmatrix}{\dfrac {K-P}{P}}\end
      {vmatrix}}=e^{-kt-C}\\[6pt]&{\begin{vmatrix}{\dfrac {K-P}{P}}\end
      {vmatrix}}=e^{-C}e^{-kt}\\[6pt]&{\frac {K-P}{P}}=\pm e^{-C}e^{-kt}\\[6pt]
      {\text{Let }}&A=\pm e^{-C}.\\[6pt]&{\frac {K-P}{P}}=Ae^{-kt}\\[6pt]&
      {\frac {K}{P}}-1=Ae^{-kt}\\[6pt]&{\frac {K}{P}}=1+Ae^{-kt}\\[6pt]&{\frac
      {P}{K}}={\frac {1}{1+Ae^{-kt}}}\\[6pt]&P={\frac {K}{1+Ae^{-kt}}}\end
      {aligned}}}]
Therefore, the solution to the logistic equation is
         P ( t ) =   K  1 + A  e  &#x2212; k t        {\displaystyle P(t)=
      {\frac {K}{1+Ae^{-kt}}}}  [{\displaystyle P(t)={\frac {K}{1+Ae^{-kt}}}}]
To find     A   {\displaystyle A}  [A], let     t = 0   {\displaystyle t=0}
[t=0] and     P  ( 0 )  =  P  0     {\displaystyle P\left(0\right)=P_{0}}
[P\left(0\right)=P_{0}]. Then we have
          P  0   =   K  1 + A  e  0        {\displaystyle P_{0}={\frac {K}
      {1+Ae^{0}}}}  [P_{0}={\frac  {K}{1+Ae^{0}}}]
Noting that      e  0   = 1   {\displaystyle e^{0}=1}  [e^{0}=1], and solving
for A we get
         A =    K &#x2212;  P  0     P  0     .   {\displaystyle A={\frac {K-P_
      {0}}{P_{0}}}.}  [{\displaystyle A={\frac {K-P_{0}}{P_{0}}}.}]
***** Partial differential equations[edit] *****
The method of separation of variables is also used to solve a wide range of
linear partial differential equations with boundary and initial conditions,
such as the heat_equation, wave_equation, Laplace_equation, Helmholtz_equation
and biharmonic_equation.
The analytical method of separation of variables for solving partial
differential equations has also been generalized into a computational method of
decomposition in invariant structures that can be used to solve systems of
partial differential equations[1].
**** Example: homogeneous case[edit] ****
Consider the one-dimensional heat_equation. The equation is
            &#x2202; u   &#x2202; t    &#x2212; &#x03B1;     &#x2202;
      2   u   &#x2202;  x  2      = 0   {\displaystyle {\frac            
      {\partial u}{\partial t}}-\alpha {\frac {\partial ^{2}u}             (1)
      {\partial x^{2}}}=0}  [{\frac  {\partial u}{\partial t}}-\alpha
      {\frac  {\partial ^{{2}}u}{\partial x^{{2}}}}=0]
The variable u denotes temperature. The boundary condition is homogeneous, that
is
         u    |    x = 0   = u    |    x = L   = 0   {\displaystyle u    
      {\big |}_{x=0}=u{\big |}_{x=L}=0}  [u{\big |}_{{x=0}}=u{\big         (2)
      |}_{{x=L}}=0]
Let us attempt to find a solution which is not identically zero satisfying the
boundary conditions but with the following property: u is a product in which
the dependence of u on x, t is separated, that is:
         u ( x , t ) = X ( x ) T ( t ) .   {\displaystyle u(x,t)=X    (3)
      (x)T(t).}  [u(x,t)=X(x)T(t).]                                   
Substituting u back into equation (1) and using the product_rule,
             T &#x2032;  ( t )   &#x03B1; T ( t )    =     X &#x2033;
      ( x )   X ( x )    .   {\displaystyle {\frac {T'(t)}{\alpha T      (4)
      (t)}}={\frac {X''(x)}{X(x)}}.}  [{\frac {T'(t)}{\alpha T(t)}}=     
      {\frac {X''(x)}{X(x)}}.]
Since the right hand side depends only on x and the left hand side only on t,
both sides are equal to some constant value â Î». Thus:
          T &#x2032;  ( t ) = &#x2212; &#x03BB; &#x03B1; T ( t ) ,       
      {\displaystyle T'(t)=-\lambda \alpha T(t),}  [T'(t)=-\lambda         (5)
      \alpha T(t),]
and
          X &#x2033;  ( x ) = &#x2212; &#x03BB; X ( x ) .               (6)
      {\displaystyle X''(x)=-\lambda X(x).}  [X''(x)=-\lambda X(x).]    
â Î» here is the eigenvalue for both differential operators, and T(t) and X
(x) are corresponding eigenfunctions.
We will now show that solutions for X(x) for values of Î» â¤ 0 cannot occur:
Suppose that Î» < 0. Then there exist real numbers B, C such that
         X ( x ) = B  e    &#x2212; &#x03BB;    x   + C  e  &#x2212;   &#x2212;
      &#x03BB;    x   .   {\displaystyle X(x)=Be^{{\sqrt {-\lambda }}\,x}+Ce^{-
      {\sqrt {-\lambda }}\,x}.}  [X(x)=Be^{{\sqrt {-\lambda }}\,x}+Ce^{-{\sqrt
      {-\lambda }}\,x}.]
From (2) we get
         X ( 0 ) = 0 = X ( L ) ,   {\displaystyle X(0)=0=X(L),}  [X    (7)
      (0)=0=X(L),]                                                     
and therefore B = 0 = C which implies u is identically 0.
Suppose that Î» = 0. Then there exist real numbers B, C such that
         X ( x ) = B x + C .   {\displaystyle X(x)=Bx+C.}  [X(x)=Bx+C.]
From (7) we conclude in the same manner as in 1 that u is identically 0.
Therefore, it must be the case that Î» > 0. Then there exist real numbers A, B,
C such that
         T ( t ) = A  e  &#x2212; &#x03BB; &#x03B1; t   ,   {\displaystyle T
      (t)=Ae^{-\lambda \alpha t},}  [T(t)=Ae^{{-\lambda \alpha t}},]
and
         X ( x ) = B sin &#x2061; (   &#x03BB;    x ) + C cos &#x2061;
      (   &#x03BB;    x ) .   {\displaystyle X(x)=B\sin({\sqrt {\lambda
      }}\,x)+C\cos({\sqrt {\lambda }}\,x).}  [X(x)=B\sin({\sqrt {\lambda
      }}\,x)+C\cos({\sqrt {\lambda }}\,x).]
From (7) we get C = 0 and that for some positive integer n,
           &#x03BB;   = n   &#x03C0; L   .   {\displaystyle {\sqrt {\lambda
      }}=n{\frac {\pi }{L}}.}  [{\sqrt {\lambda }}=n{\frac {\pi }{L}}.]
This solves the heat equation in the special case that the dependence of u has
the special form of (3).
In general, the sum of solutions to (1) which satisfy the boundary conditions
(2) also satisfies (1) and (3). Hence a complete solution can be given as
         u ( x , t ) =  &#x2211;  n = 1   &#x221E;    D  n   sin &#x2061;    n
      &#x03C0; x  L   exp &#x2061;  (  &#x2212;     n  2    &#x03C0;  2
      &#x03B1; t   L  2      )  ,   {\displaystyle u(x,t)=\sum _{n=1}^{\infty
      }D_{n}\sin {\frac {n\pi x}{L}}\exp \left(-{\frac {n^{2}\pi ^{2}\alpha t}
      {L^{2}}}\right),}  [u(x,t)=\sum _{{n=1}}^{{\infty }}D_{n}\sin {\frac
      {n\pi x}{L}}\exp \left(-{\frac  {n^{2}\pi ^{2}\alpha t}{L^{2}}}\right),]
where Dn are coefficients determined by initial condition.
Given the initial condition
         u    |    t = 0   = f ( x ) ,   {\displaystyle u{\big |}_{t=0}=f(x),}
      [u{\big |}_{{t=0}}=f(x),]
we can get
         f ( x ) =  &#x2211;  n = 1   &#x221E;    D  n   sin &#x2061;    n
      &#x03C0; x  L   .   {\displaystyle f(x)=\sum _{n=1}^{\infty }D_{n}\sin
      {\frac {n\pi x}{L}}.}  [f(x)=\sum _{{n=1}}^{{\infty }}D_{n}\sin {\frac
      {n\pi x}{L}}.]
This is the sine_series expansion of f(x). Multiplying both sides with     sin
&#x2061;    n &#x03C0; x  L     {\displaystyle \sin {\frac {n\pi x}{L}}}  [\sin
{\frac  {n\pi x}{L}}] and integrating over [0,L] result in
          D  n   =   2 L    &#x222B;  0   L   f ( x ) sin &#x2061;    n
      &#x03C0; x  L    d x .   {\displaystyle D_{n}={\frac {2}{L}}\int _{0}^
      {L}f(x)\sin {\frac {n\pi x}{L}}\,dx.}  [D_{n}={\frac  {2}{L}}\int _{0}^
      {L}f(x)\sin {\frac  {n\pi x}{L}}\,dx.]
This method requires that the eigenfunctions of x, here       {  sin &#x2061;
n &#x03C0; x  L    }   n = 1   &#x221E;     {\displaystyle \left\{\sin {\frac
{n\pi x}{L}}\right\}_{n=1}^{\infty }}  [\left\{\sin {\frac  {n\pi x}
{L}}\right\}_{{n=1}}^{{\infty }}], are orthogonal and complete. In general this
is guaranteed by Sturm-Liouville_theory.
**** Example: nonhomogeneous case[edit] ****
Suppose the equation is nonhomogeneous,
            &#x2202; u   &#x2202; t    &#x2212; &#x03B1;     &#x2202;
      2   u   &#x2202;  x  2      = h ( x , t )   {\displaystyle         
      {\frac {\partial u}{\partial t}}-\alpha {\frac {\partial ^{2}u}      (8)
      {\partial x^{2}}}=h(x,t)}  [{\frac  {\partial u}{\partial t}}-
      \alpha {\frac  {\partial ^{{2}}u}{\partial x^{{2}}}}=h(x,t)]
with the boundary condition the same as (2).
Expand h(x,t), u(x,t) and f(x) into
         h ( x , t ) =  &#x2211;  n = 1   &#x221E;    h  n   ( t )
      sin &#x2061;    n &#x03C0; x  L   ,   {\displaystyle h             
      (x,t)=\sum _{n=1}^{\infty }h_{n}(t)\sin {\frac {n\pi x}{L}},}        (9)
      [h(x,t)=\sum _{{n=1}}^{{\infty }}h_{{n}}(t)\sin {\frac  {n\pi
      x}{L}},]
         u ( x , t ) =  &#x2211;  n = 1   &#x221E;    u  n   ( t )
      sin &#x2061;    n &#x03C0; x  L   ,   {\displaystyle u           
      (x,t)=\sum _{n=1}^{\infty }u_{n}(t)\sin {\frac {n\pi x}{L}},}      (10)
      [u(x,t)=\sum _{{n=1}}^{{\infty }}u_{{n}}(t)\sin {\frac  {n\pi
      x}{L}},]
         f ( x ) =  &#x2211;  n = 1   &#x221E;    b  n   sin
      &#x2061;    n &#x03C0; x  L   ,   {\displaystyle f(x)=\sum _     (11)
      {n=1}^{\infty }b_{n}\sin {\frac {n\pi x}{L}},}  [f(x)=\sum _{    
      {n=1}}^{{\infty }}b_{{n}}\sin {\frac  {n\pi x}{L}},]
where hn(t) and bn can be calculated by integration, while un(t) is to be
determined.
Substitute (9) and (10) back to (8) and considering the orthogonality of sine
functions we get
          u  n  &#x2032;  ( t ) + &#x03B1;     n  2    &#x03C0;  2     L  2
      u  n   ( t ) =  h  n   ( t ) ,   {\displaystyle u'_{n}(t)+\alpha {\frac
      {n^{2}\pi ^{2}}{L^{2}}}u_{n}(t)=h_{n}(t),}  [u'_{{n}}(t)+\alpha {\frac
      {n^{{2}}\pi ^{{2}}}{L^{{2}}}}u_{{n}}(t)=h_{{n}}(t),]
which are a sequence of linear_differential_equations that can be readily
solved with, for instance, Laplace_transform, or Integrating_factor. Finally,
we can get
          u  n   ( t ) =  e  &#x2212; &#x03B1;     n  2    &#x03C0;  2     L  2
      t    (   b  n   +  &#x222B;  0   t    h  n   ( s )  e  &#x03B1;     n  2
      &#x03C0;  2     L  2     s    d s  )  .   {\displaystyle u_{n}(t)=e^{-
      \alpha {\frac {n^{2}\pi ^{2}}{L^{2}}}t}\left(b_{n}+\int _{0}^{t}h_{n}
      (s)e^{\alpha {\frac {n^{2}\pi ^{2}}{L^{2}}}s}\,ds\right).}  [u_{{n}}
      (t)=e^{{-\alpha {\frac  {n^{{2}}\pi ^{{2}}}{L^{{2}}}}t}}\left(b_{
      {n}}+\int _{{0}}^{{t}}h_{{n}}(s)e^{{\alpha {\frac  {n^{{2}}\pi ^{{2}}}{L^
      {{2}}}}s}}\,ds\right).]
If the boundary condition is nonhomogeneous, then the expansion of (9) and (10)
is no longer valid. One has to find a function v that satisfies the boundary
condition only, and subtract it from u. The function u-v then satisfies
homogeneous boundary condition, and can be solved with the above method.
**** Example: mixed derivatives[edit] ****
For some equations involving mixed derivatives, the equation does not separate
as easily as the heat equation did in the first example above, but nonetheless
separation of variables may still be applied. Consider the two-dimensional
biharmonic_equation
             &#x2202;  4   u   &#x2202;  x  4      + 2     &#x2202;  4   u
      &#x2202;  x  2   &#x2202;  y  2      +     &#x2202;  4   u   &#x2202;  y
      4      = 0.   {\displaystyle {\frac {\partial ^{4}u}{\partial x^{4}}}+2
      {\frac {\partial ^{4}u}{\partial x^{2}\partial y^{2}}}+{\frac {\partial ^
      {4}u}{\partial y^{4}}}=0.}  [{\displaystyle {\frac {\partial ^{4}u}
      {\partial x^{4}}}+2{\frac {\partial ^{4}u}{\partial x^{2}\partial y^
      {2}}}+{\frac {\partial ^{4}u}{\partial y^{4}}}=0.}]
Proceeding in the usual manner, we look for solutions of the form
         u ( x , y ) = X ( x ) Y ( y )   {\displaystyle u(x,y)=X(x)Y(y)}  [
      {\displaystyle u(x,y)=X(x)Y(y)}]
and we obtain the equation
             X  ( 4 )   ( x )   X ( x )    + 2     X &#x2033;  ( x )   X ( x )
      Y &#x2033;  ( y )   Y ( y )    +     Y  ( 4 )   ( y )   Y ( y )    = 0.
      {\displaystyle {\frac {X^{(4)}(x)}{X(x)}}+2{\frac {X''(x)}{X(x)}}{\frac
      {Y''(y)}{Y(y)}}+{\frac {Y^{(4)}(y)}{Y(y)}}=0.}  [{\displaystyle {\frac
      {X^{(4)}(x)}{X(x)}}+2{\frac {X''(x)}{X(x)}}{\frac {Y''(y)}{Y(y)}}+{\frac
      {Y^{(4)}(y)}{Y(y)}}=0.}]
Writing this equation in the form
         E ( x ) + F ( x ) G ( y ) + H ( y ) = 0 ,   {\displaystyle E(x)+F(x)G
      (y)+H(y)=0,}  [{\displaystyle E(x)+F(x)G(y)+H(y)=0,}]
we see that the derivative with respect to x and y eliminates the first and
last terms, so that
          F &#x2032;  ( x )  G &#x2032;  ( y ) = 0 ,   {\displaystyle F'(x)G'
      (y)=0,}  [{\displaystyle F'(x)G'(y)=0,}]
i.e. either F(x) or G(y) must be a constant, say -Î». This further implies that
either     &#x2212; E ( x ) = F ( x ) G ( y ) + H ( y )   {\displaystyle -E
(x)=F(x)G(y)+H(y)}  [{\displaystyle -E(x)=F(x)G(y)+H(y)}] or     &#x2212; H ( y
) = E ( x ) + F ( x ) G ( y )   {\displaystyle -H(y)=E(x)+F(x)G(y)}  [
{\displaystyle -H(y)=E(x)+F(x)G(y)}] are constant. Returning to the equation
for X and Y, we have two cases
              X &#x2033;  ( x )    = &#x2212;  &#x03BB;  1   X ( x )      X
      ( 4 )   ( x )    =  &#x03BC;  1   X ( x )      Y  ( 4 )   ( y ) &#x2212;
      2  &#x03BB;  1    Y &#x2033;  ( y )    = &#x2212;  &#x03BC;  1   Y ( y )
      {\displaystyle {\begin{aligned}X''(x)&=-\lambda _{1}X(x)\\X^{(4)}(x)&=\mu
      _{1}X(x)\\Y^{(4)}(y)-2\lambda _{1}Y''(y)&=-\mu _{1}Y(y)\end{aligned}}}  [
      {\displaystyle {\begin{aligned}X''(x)&=-\lambda _{1}X(x)\\X^{(4)}(x)&=\mu
      _{1}X(x)\\Y^{(4)}(y)-2\lambda _{1}Y''(y)&=-\mu _{1}Y(y)\end{aligned}}}]
and
              Y &#x2033;  ( y )    = &#x2212;  &#x03BB;  2   Y ( y )      Y
      ( 4 )   ( y )    =  &#x03BC;  2   Y ( y )      X  ( 4 )   ( x ) &#x2212;
      2  &#x03BB;  2    X &#x2033;  ( x )    = &#x2212;  &#x03BC;  2   X ( x )
      {\displaystyle {\begin{aligned}Y''(y)&=-\lambda _{2}Y(y)\\Y^{(4)}(y)&=\mu
      _{2}Y(y)\\X^{(4)}(x)-2\lambda _{2}X''(x)&=-\mu _{2}X(x)\end{aligned}}}  [
      {\displaystyle {\begin{aligned}Y''(y)&=-\lambda _{2}Y(y)\\Y^{(4)}(y)&=\mu
      _{2}Y(y)\\X^{(4)}(x)-2\lambda _{2}X''(x)&=-\mu _{2}X(x)\end{aligned}}}]
which can each be solved by considering the separate cases for      &#x03BB;  i
< 0 ,  &#x03BB;  i   = 0 ,  &#x03BB;  i   > 0   {\displaystyle \lambda _
{i}<0,\lambda _{i}=0,\lambda _{i}>0}  [{\displaystyle \lambda _{i}<0,\lambda _
{i}=0,\lambda _{i}>0}] and noting that      &#x03BC;  i   =  &#x03BB;  i   2
{\displaystyle \mu _{i}=\lambda _{i}^{2}}  [{\displaystyle \mu _{i}=\lambda _
{i}^{2}}].
**** Curvilinear coordinates[edit] ****
In orthogonal_curvilinear_coordinates, separation of variables can still be
used, but in some details different from that in Cartesian coordinates. For
instance, regularity or periodic condition may determine the eigenvalues in
place of boundary conditions. See spherical_harmonics for example.
***** Matrices[edit] *****
The matrix form of the separation of variables is the Kronecker_sum.
As an example we consider the 2D discrete_Laplacian on a regular_grid:
         L =   D  x x    &#x2295;   D  y y    =   D  x x    &#x2297;  I  +  I
      &#x2297;   D  y y    ,    {\displaystyle L=\mathbf {D_{xx}} \oplus
      \mathbf {D_{yy}} =\mathbf {D_{xx}} \otimes \mathbf {I} +\mathbf {I}
      \otimes \mathbf {D_{yy}} ,\,}  [L={\mathbf  {D_{{xx}}}}\oplus {\mathbf
      {D_{{yy}}}}={\mathbf  {D_{{xx}}}}\otimes {\mathbf  {I}}+{\mathbf
      {I}}\otimes {\mathbf  {D_{{yy}}}},\,]
where       D  x x      {\displaystyle \mathbf {D_{xx}} }  [{\mathbf  {D_{
{xx}}}}] and       D  y y      {\displaystyle \mathbf {D_{yy}} }  [{\mathbf
{D_{{yy}}}}] are 1D discrete Laplacians in the x- and y-directions,
correspondingly, and      I    {\displaystyle \mathbf {I} }  [{\mathbf  {I}}]
are the identities of appropriate sizes. See the main article Kronecker_sum_of
discrete_Laplacians for details.
***** See also[edit] *****
    * Inseparable_differential_equation
***** References[edit] *****
   1. ^Miroshnikov, Victor A. (2017). Harmonic_Wave_Systems:_Partial
      Differential_Equations_of_the_Helmholtz_Decomposition. Scientific
      Research Publishing.
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
    * Polyanin, Andrei D. (2001-11-28). Handbook of Linear Partial Differential
      Equations for Engineers and Scientists. Boca Raton, FL: Chapman_&_Hall/
      CRC. ISBN 1-58488-299-9.
Myint-U, Tyn; Debnath,_Lokenath (2007). Linear_Partial_Differential_Equations
for_Scientists_and_Engineers. Boston, MA: BirkhÃ¤user_Boston. doi:10.1007/978-
0-8176-4560-1. ISBN 978-0-8176-4393-5. Retrieved 2011-03-29.
Teschl,_Gerald (2012). Ordinary_Differential_Equations_and_Dynamical_Systems.
Graduate_Studies_in_Mathematics. 140. Providence, RI: American_Mathematical
Society. ISBN 978-0-8218-8328-0.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Fourier_method", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
John Renze, Eric_W._Weisstein, Separation_of_variables (Differential_Equation)
at MathWorld.
Methods_of_Generalized_and_Functional_Separation_of_Variables at EqWorld: The
World of Mathematical Equations
Examples of separating variables to solve PDEs
"A_Short_Justification_of_Separation_of_Variables"

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Separation_of_variables&oldid=902077203"
Categories:
    * Ordinary_differential_equations
    * Partial_differential_equations
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
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * FranÃ§ais
    * íêµ­ì´
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 16 June 2019, at 11:29 (UTC).
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
