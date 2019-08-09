The following text has been accessed from https://en.wikipedia.org/wiki/Variation_of_parameters at Fri Aug 9 02:43:06 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Variation of parameters ******
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
    * Separation_of_variables
    * Undetermined_coefficients
    * Variation of parameters
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
Procedure for solving differential equations
In mathematics, variation of parameters, also known as variation of constants,
is a general method to solve inhomogeneous linear ordinary_differential
equations.
For first-order inhomogeneous linear differential equations it is usually
possible to find solutions via integrating_factors or undetermined_coefficients
with considerably less effort, although those methods leverage heuristics that
involve guessing and don't work for all inhomogeneous linear differential
equations.
Variation of parameters extends to linear partial_differential_equations as
well, specifically to inhomogeneous problems for linear evolution equations
like the heat_equation, wave_equation, and vibrating_plate equation. In this
setting, the method is more often known as Duhamel's_principle, named after
Jean-Marie_Duhamel (1797â1872) who first applied the method to solve the
inhomogeneous heat equation. Sometimes variation of parameters itself is called
Duhamel's principle and vice versa.
⁰
***** Contents *****
    * 1_Intuitive_explanation
    * 2_History
    * 3_Description_of_method
    * 4_Examples
          o 4.1_First_order_equation
          o 4.2_Specific_second_order_equation
          o 4.3_General_second-order_equation
    * 5_References
    * 6_External_links
***** Intuitive explanation[edit] *****
Consider the equation of the forced dispersionless spring, in suitable units:
          x &#x2033;  ( t ) + x ( t ) = F ( t ) .   {\displaystyle x''(t)+x
      (t)=F(t).}  [{\displaystyle x''(t)+x(t)=F(t).}]
Here x is the displacement of the spring from the equilibrium x = 0, and F(t)
is an external applied force that depends on time. When the external force is
zero, this is the homogeneous equation (whose solutions are linear combinations
of sines and cosines, corresponding to the spring oscillating with constant
total energy).
We can construct the solution physically, as follows. Between times     t = s
{\displaystyle t=s}  [{\displaystyle t=s}] and     t = s + d s   {\displaystyle
t=s+ds}  [{\displaystyle t=s+ds}], the momentum corresponding to the solution
has a net change     F ( s )  d s   {\displaystyle F(s)\,ds}  [{\displaystyle F
(s)\,ds}]. A solution to the inhomogeneous equation, at the present time t > 0,
is obtained by linearly superposing the solutions obtained in this manner, for
s going between 0 and t.
The homogeneous initial-value problem, representing a small impulse     F ( s )
d s   {\displaystyle F(s)\,ds}  [{\displaystyle F(s)\,ds}] being added to the
solution at time     t = s   {\displaystyle t=s}  [{\displaystyle t=s}], is
          x &#x2033;  ( t ) + x ( t ) = 0 ,  x ( s ) = 0 , &#xA0;  x &#x2032;
      ( s ) = F ( s )  d s .   {\displaystyle x''(t)+x(t)=0,\quad x(s)=0,\ x'
      (s)=F(s)\,ds.}  [{\displaystyle x''(t)+x(t)=0,\quad x(s)=0,\ x'(s)=F
      (s)\,ds.}]
The unique solution to this problem is easily seen to be     x ( t ) = F ( s )
sin &#x2061; ( t &#x2212; s )  d s   {\displaystyle x(t)=F(s)\sin(t-s)\,ds}  [
{\displaystyle x(t)=F(s)\sin(t-s)\,ds}]. The linear superposition of all of
these solutions is given by the integral:
         x ( t ) =  &#x222B;  0   t   F ( s ) sin &#x2061; ( t &#x2212; s )  d
      s .   {\displaystyle x(t)=\int _{0}^{t}F(s)\sin(t-s)\,ds.}  [
      {\displaystyle x(t)=\int _{0}^{t}F(s)\sin(t-s)\,ds.}]
To verify that this satisfies the required equation:
          x &#x2032;  ( t ) =  &#x222B;  0   t   F ( s ) cos &#x2061; ( t
      &#x2212; s )  d s   {\displaystyle x'(t)=\int _{0}^{t}F(s)\cos(t-s)\,ds}
      [{\displaystyle x'(t)=\int _{0}^{t}F(s)\cos(t-s)\,ds}]
          x &#x2033;  ( t ) = F ( t ) &#x2212;  &#x222B;  0   t   F ( s ) sin
      &#x2061; ( t &#x2212; s )  d s = F ( t ) &#x2212; x ( t ) ,
      {\displaystyle x''(t)=F(t)-\int _{0}^{t}F(s)\sin(t-s)\,ds=F(t)-x(t),}  [
      {\displaystyle x''(t)=F(t)-\int _{0}^{t}F(s)\sin(t-s)\,ds=F(t)-x(t),}]
as required.
The general method of variation of parameters allows for solution of an
inhomogeneous linear equation
         L x ( t ) = F ( t )   {\displaystyle Lx(t)=F(t)}  [{\displaystyle Lx
      (t)=F(t)}]
by interpreting the second-order linear differential operator L as the net
force, so that the total impulse imparted to a solution between time s and s+ds
is F(s)ds. Denote by      x  s     {\displaystyle x_{s}}  [{\displaystyle x_
{s}}] the solution of the homogeneous initial value problem
         L x ( t ) = 0 ,  x ( s ) = 0 ,  x &#x2032;  ( s ) = F ( s )  d s .
      {\displaystyle Lx(t)=0,\quad x(s)=0,x'(s)=F(s)\,ds.}  [{\displaystyle Lx
      (t)=0,\quad x(s)=0,x'(s)=F(s)\,ds.}]
Then a particular solution of the inhomogeneous equation is
         x ( t ) =  &#x222B;  0   t    x  s   ( t )  d s ,   {\displaystyle x
      (t)=\int _{0}^{t}x_{s}(t)\,ds,}  [{\displaystyle x(t)=\int _{0}^{t}x_{s}
      (t)\,ds,}]
the result of linearly superposing the infinitesimal homogeneous solutions.
There are generalizations to higher order linear differential operators.
In practice, variation of parameters usually involves the fundamental solution
of the homogeneous problem, the infinitesimal solutions      x  s
{\displaystyle x_{s}}  [{\displaystyle x_{s}}] then being given in terms of
explicit linear combinations of linearly independent fundamental solutions. In
the case of the forced dispersionless spring, the kernel     sin &#x2061; ( t
&#x2212; s ) = sin &#x2061; t cos &#x2061; s &#x2212; sin &#x2061; s cos
&#x2061; t   {\displaystyle \sin(t-s)=\sin t\cos s-\sin s\cos t}  [
{\displaystyle \sin(t-s)=\sin t\cos s-\sin s\cos t}] is the associated
decomposition into fundamental solutions.
***** History[edit] *****
The method of variation of parameters was introduced by the Swiss-born
mathematician Leonhard_Euler (1707â1783) and completed by the Italian-French
mathematician Joseph-Louis_Lagrange (1736â1813).[1] A forerunner of the
method of variation of a celestial body's orbital elements appeared in Euler's
work in 1748, while he was studying the mutual perturbations of Jupiter and
Saturn.[2] In his 1749 study of the motions of the earth, Euler obtained
differential equations for the orbital elements;[3] and in 1753 he applied the
method to his study of the motions of the moon.[4] Lagrange first used the
method in 1766.[5] Between 1778 and 1783, Lagrange further developed the method
both in a series of memoirs on variations in the motions of the planets[6] and
in another series of memoirs on determining the orbit of a comet from three
observations.[7] (Euler and Lagrange applied this method to nonlinear
differential equations and that, instead of varying the coefficients of linear
combinations of solutions to homogeneous equations, they varied the constants
of the unperturbed motions of the celestial bodies.[8]) During 1808â1810,
Lagrange gave the method of variation of parameters its final form in a series
of papers.[9] The central result of his study was the system of planetary
equations in the form of Lagrange, which described the evolution of the
Keplerian parameters (orbital elements) of a perturbed orbit.
In his description of evolving orbits, Lagrange set a reduced two-body problem
as an unperturbed solution, and presumed that all perturbations come from the
gravitational pull which the bodies other than the primary exert at the
secondary (orbiting) body. Accordingly, his method implied that the
perturbations depend solely on the position of the secondary, but not on its
velocity. In the 20th century, celestial mechanics began to consider
interactions which depend on both positions and velocities (relativistic
corrections, atmospheric drag, inertial forces). Therefore, the method of
variation of parameters used by Lagrange was extended to the situation with
velocity-dependent forces.[10]
***** Description of method[edit] *****
Given an ordinary non-homogeneous linear differential equation of order n
          y  ( n )   ( x ) +  &#x2211;  i = 0   n &#x2212; 1    a  i   ( x )  y
      ( i )   ( x ) = b ( x ) .     ( i )     {\displaystyle y^{(n)}(x)+\sum _
      {i=0}^{n-1}a_{i}(x)y^{(i)}(x)=b(x).\quad \quad {\rm {(i)}}}  [y^{(n)}(x)
      + \sum_{i=0}^{n-1} a_i(x) y^{(i)}(x) = b(x).\quad\quad {\rm (i)}]
Let      y  1   ( x ) , &#x2026; ,  y  n   ( x )   {\displaystyle y_{1}
(x),\ldots ,y_{n}(x)}  [y_1(x), \ldots, y_n(x)] be a fundamental_system of
solutions of the corresponding homogeneous equation
          y  ( n )   ( x ) +  &#x2211;  i = 0   n &#x2212; 1    a  i   ( x )  y
      ( i )   ( x ) = 0.     ( i i )     {\displaystyle y^{(n)}(x)+\sum _{i=0}^
      {n-1}a_{i}(x)y^{(i)}(x)=0.\quad \quad {\rm {(ii)}}}  [y^{(n)}(x) + \sum_
      {i=0}^{n-1} a_i(x) y^{(i)}(x) = 0.\quad\quad {\rm (ii)}]
Then a particular_solution to the non-homogeneous equation is given by
          y  p   ( x ) =  &#x2211;  i = 1   n    c  i   ( x )  y  i   ( x )
      ( i i i )     {\displaystyle y_{p}(x)=\sum _{i=1}^{n}c_{i}(x)y_{i}
      (x)\quad \quad {\rm {(iii)}}}  [y_p(x) = \sum_{i=1}^{n} c_i(x) y_i
      (x)\quad\quad {\rm (iii)}]
where the      c  i   ( x )   {\displaystyle c_{i}(x)}  [c_i(x)] are
differentiable functions which are assumed to satisfy the conditions
          &#x2211;  i = 1   n    c  i  &#x2032;  ( x )  y  i   ( j )   ( x ) =
      0 ,  j = 0 , &#x2026; , n &#x2212; 2.     ( i v )     {\displaystyle \sum
      _{i=1}^{n}c_{i}'(x)y_{i}^{(j)}(x)=0,\quad j=0,\ldots ,n-2.\quad \quad
      {\rm {(iv)}}}  [{\displaystyle \sum _{i=1}^{n}c_{i}'(x)y_{i}^{(j)}
      (x)=0,\quad j=0,\ldots ,n-2.\quad \quad {\rm {(iv)}}}]
Starting with (iii), repeated differentiation combined with repeated use of
(iv) gives
          y  p   ( j )   ( x ) =  &#x2211;  i = 1   n    c  i   ( x )  y  i
      ( j )   ( x ) ,  j = 0 , &#x2026; , n &#x2212; 1   .      ( v )
      {\displaystyle y_{p}^{(j)}(x)=\sum _{i=1}^{n}c_{i}(x)y_{i}^{(j)}(x),\quad
      j=0,\ldots ,n-1\,\mathrm {.} \quad \quad {\rm {(v)}}}  [{\displaystyle y_
      {p}^{(j)}(x)=\sum _{i=1}^{n}c_{i}(x)y_{i}^{(j)}(x),\quad j=0,\ldots ,n-
      1\,\mathrm {.} \quad \quad {\rm {(v)}}}]
One last differentiation gives
          y  p   ( n )   ( x ) =  &#x2211;  i = 1   n    c  i  &#x2032;  ( x )
      y  i   ( n &#x2212; 1 )   ( x ) +  &#x2211;  i = 1   n    c  i   ( x )  y
      i   ( n )   ( x )   .      ( v i )     {\displaystyle y_{p}^{(n)}(x)=\sum
      _{i=1}^{n}c_{i}'(x)y_{i}^{(n-1)}(x)+\sum _{i=1}^{n}c_{i}(x)y_{i}^{(n)}
      (x)\,\mathrm {.} \quad \quad {\rm {(vi)}}}  [y_p^{(n)}(x)=\sum_{i=1}^n
      c_i'(x)y_i^{(n-1)}(x)+\sum_{i=1}^n c_i(x) y_i^{(n)}(x)\, \mathrm{.}
      \quad\quad{\rm (vi)}]
By substituting (iii) into (i) and applying (v) and (vi) it follows that
          &#x2211;  i = 1   n    c  i  &#x2032;  ( x )  y  i   ( n &#x2212; 1 )
      ( x ) = b ( x ) .     ( v i i )     {\displaystyle \sum _{i=1}^{n}c_{i}'
      (x)y_{i}^{(n-1)}(x)=b(x).\quad \quad {\rm {(vii)}}}  [\sum_{i=1}^n c_i'
      (x) y_i^{(n-1)}(x) = b(x).\quad\quad {\rm (vii)}]
The linear system (iv and vii) of n equations can then be solved using Cramer's
rule yielding
          c  i  &#x2032;  ( x ) =     W  i   ( x )   W ( x )    ,   i = 1 ,
      &#x2026; , n   {\displaystyle c_{i}'(x)={\frac {W_{i}(x)}{W(x)}},\,\quad
      i=1,\ldots ,n}  [c_i'(x) = \frac{W_i(x)}{W(x)}, \, \quad i=1,\ldots,n]
where     W ( x )   {\displaystyle W(x)}  [W(x)] is the Wronskian_determinant
of the fundamental system and      W  i   ( x )   {\displaystyle W_{i}(x)}
[W_i(x)] is the Wronskian determinant of the fundamental system with the i-th
column replaced by     ( 0 , 0 , &#x2026; , b ( x ) ) .   {\displaystyle
(0,0,\ldots ,b(x)).}  [(0, 0, \ldots, b(x)).]
The particular solution to the non-homogeneous equation can then be written as
          &#x2211;  i = 1   n    y  i   ( x )  &#x222B;     W  i   ( x )   W
      ( x )      d  x .   {\displaystyle \sum _{i=1}^{n}y_{i}(x)\,\int {\frac
      {W_{i}(x)}{W(x)}}\,\mathrm {d} x.}  [{\displaystyle \sum _{i=1}^{n}y_{i}
      (x)\,\int {\frac {W_{i}(x)}{W(x)}}\,\mathrm {d} x.}]
***** Examples[edit] *****
**** First order equation[edit] ****
          y &#x2032;  + p ( x ) y = q ( x )   {\displaystyle y'+p(x)y=q(x)}
      [y'+p(x)y=q(x)]
The general solution of the corresponding homogeneous equation (written below)
is the complementary solution to our original (inhomogeneous) equation:
          y &#x2032;  + p ( x ) y = 0   {\displaystyle y'+p(x)y=0}  [y'+p
      (x)y=0].
This homogeneous differential equation can be solved by different methods, for
example separation_of_variables:
           d  d x    y + p ( x ) y = 0   {\displaystyle {\frac {d}{dx}}y+p
      (x)y=0}  [{\frac  {d}{dx}}y+p(x)y=0]
            d y   d x    = &#x2212; p ( x ) y   {\displaystyle {\frac {dy}
      {dx}}=-p(x)y}  [{\frac  {dy}{dx}}=-p(x)y]
            d y  y   = &#x2212;  p ( x ) d x  ,   {\displaystyle {dy \over y}=-
      {p(x)dx},}  [{dy \over y}=-{p(x)dx},]
         &#x222B;   1 y    d y = &#x2212; &#x222B; p ( x )  d x
      {\displaystyle \int {\frac {1}{y}}\,dy=-\int p(x)\,dx}  [\int {\frac  {1}
      {y}}\,dy=-\int p(x)\,dx]
         ln &#x2061;  |  y  |  = &#x2212; &#x222B; p ( x )  d x +  C  0
      {\displaystyle \ln |y|=-\int p(x)\,dx+C_{0}}  [{\displaystyle \ln |y|=-
      \int p(x)\,dx+C_{0}}]
         y = &#x00B1;  e  &#x2212; &#x222B; p ( x )  d x +  C  0     =  C  0
      e  &#x2212; &#x222B; p ( x )  d x     {\displaystyle y=\pm e^{-\int p
      (x)\,dx+C_{0}}=C_{0}e^{-\int p(x)\,dx}}  [{\displaystyle y=\pm e^{-\int p
      (x)\,dx+C_{0}}=C_{0}e^{-\int p(x)\,dx}}]
The complementary solution to our original equation is therefore:
          y  c   =  C  0    e  &#x2212; &#x222B; p ( x )  d x
      {\displaystyle y_{c}=C_{0}e^{-\int p(x)\,dx}}  [{\displaystyle y_{c}=C_
      {0}e^{-\int p(x)\,dx}}]
Now we return to solving the non-homogeneous equation:
          y &#x2032;  + p ( x ) y = q ( x )   {\displaystyle y'+p(x)y=q(x)}
      [y'+p(x)y=q(x)]
Using the method variation of parameters, the particular solution is formed by
multiplying the complementary solution by an unknown function C(x):
          y  p   = C ( x )  e  &#x2212; &#x222B; p ( x )  d x
      {\displaystyle y_{p}=C(x)e^{-\int p(x)\,dx}}  [y_{p}=C(x)e^{{-\int p
      (x)\,dx}}]
By substituting the particular solution into the non-homogeneous equation, we
can find C(x):
          C &#x2032;  ( x )  e  &#x2212; &#x222B; p ( x )  d x   &#x2212; C ( x
      ) p ( x )  e  &#x2212; &#x222B; p ( x )  d x   + p ( x ) C ( x )  e
      &#x2212; &#x222B; p ( x )  d x   = q ( x )   {\displaystyle C'(x)e^{-\int
      p(x)\,dx}-C(x)p(x)e^{-\int p(x)\,dx}+p(x)C(x)e^{-\int p(x)\,dx}=q(x)}
      [C'(x)e^{{-\int p(x)\,dx}}-C(x)p(x)e^{{-\int p(x)\,dx}}+p(x)C(x)e^{{-\int
      p(x)\,dx}}=q(x)]
          C &#x2032;  ( x )  e  &#x2212; &#x222B; p ( x )  d x   = q ( x )
      {\displaystyle C'(x)e^{-\int p(x)\,dx}=q(x)}  [C'(x)e^{{-\int p
      (x)\,dx}}=q(x)]
          C &#x2032;  ( x ) = q ( x )  e  &#x222B; p ( x )  d x
      {\displaystyle C'(x)=q(x)e^{\int p(x)\,dx}}  [C'(x)=q(x)e^{{\int p
      (x)\,dx}}]
         C ( x ) = &#x222B; q ( x )  e  &#x222B; p ( x )  d x    d x +  C  1
      {\displaystyle C(x)=\int q(x)e^{\int p(x)\,dx}\,dx+C_{1}}  [
      {\displaystyle C(x)=\int q(x)e^{\int p(x)\,dx}\,dx+C_{1}}]
We only need a single particular solution, so we arbitrarily select      C  1
= 0   {\displaystyle C_{1}=0}  [C_1=0] for simplicity. Therefore the particular
solution is:
          y  p   =  e  &#x2212; &#x222B; p ( x )  d x   &#x222B; q ( x )  e
      &#x222B; p ( x )  d x    d x   {\displaystyle y_{p}=e^{-\int p
      (x)\,dx}\int q(x)e^{\int p(x)\,dx}\,dx}  [{\displaystyle y_{p}=e^{-\int p
      (x)\,dx}\int q(x)e^{\int p(x)\,dx}\,dx}]
The final solution of the differential equation is:
             y    =  y  c   +  y  p         =  C  0    e  &#x2212; &#x222B; p
      ( x )  d x   +  e  &#x2212; &#x222B; p ( x )  d x   &#x222B; q ( x )  e
      &#x222B; p ( x )  d x    d x       {\displaystyle {\begin{aligned}y&=y_
      {c}+y_{p}\\&=C_{0}e^{-\int p(x)\,dx}+e^{-\int p(x)\,dx}\int q(x)e^{\int p
      (x)\,dx}\,dx\end{aligned}}}  [{\displaystyle {\begin{aligned}y&=y_{c}+y_
      {p}\\&=C_{0}e^{-\int p(x)\,dx}+e^{-\int p(x)\,dx}\int q(x)e^{\int p
      (x)\,dx}\,dx\end{aligned}}}]
**** Specific second order equation[edit] ****
Let us solve
          y &#x2033;  + 4  y &#x2032;  + 4 y = cosh &#x2061; x   {\displaystyle
      y''+4y'+4y=\cosh x}  [{\displaystyle y''+4y'+4y=\cosh x}]
We want to find the general solution to the differential equation, that is, we
want to find solutions to the homogeneous differential equation
          y &#x2033;  + 4  y &#x2032;  + 4 y = 0.   {\displaystyle
      y''+4y'+4y=0.}  [{\displaystyle y''+4y'+4y=0.}]
The characteristic_equation is:
          &#x03BB;  2   + 4 &#x03BB; + 4 = ( &#x03BB; + 2  )  2   = 0
      {\displaystyle \lambda ^{2}+4\lambda +4=(\lambda +2)^{2}=0}  [
      {\displaystyle \lambda ^{2}+4\lambda +4=(\lambda +2)^{2}=0}]
Since     &#x03BB; = &#x2212; 2   {\displaystyle \lambda =-2}  [{\displaystyle
\lambda =-2}] is a repeated root, we have to introduce a factor of x for one
solution to ensure linear independence: u1 = eâ2x and u2 = xeâ2x. The
Wronskian of these two functions is
         W =   |     e  &#x2212; 2 x     x  e  &#x2212; 2 x       &#x2212; 2  e
      &#x2212; 2 x     &#x2212;  e  &#x2212; 2 x   ( 2 x &#x2212; 1 )    |   =
      &#x2212;  e  &#x2212; 2 x    e  &#x2212; 2 x   ( 2 x &#x2212; 1 ) + 2 x
      e  &#x2212; 2 x    e  &#x2212; 2 x   =  e  &#x2212; 4 x   .
      {\displaystyle W={\begin{vmatrix}e^{-2x}&xe^{-2x}\\-2e^{-2x}&-e^{-2x}(2x-
      1)\\\end{vmatrix}}=-e^{-2x}e^{-2x}(2x-1)+2xe^{-2x}e^{-2x}=e^{-4x}.}  [
      {\displaystyle W={\begin{vmatrix}e^{-2x}&xe^{-2x}\\-2e^{-2x}&-e^{-2x}(2x-
      1)\\\end{vmatrix}}=-e^{-2x}e^{-2x}(2x-1)+2xe^{-2x}e^{-2x}=e^{-4x}.}]
Because the Wronskian is non-zero, the two functions are linearly independent,
so this is in fact the general solution for the homogeneous differential
equation (and not a mere subset of it).
We seek functions A(x) and B(x) so A(x)u1 + B(x)u2 is a general solution of the
non-homogeneous equation. We need only calculate the integrals
         A ( x ) = &#x2212; &#x222B;   1 W    u  2   ( x ) b ( x )   d  x ,  B
      ( x ) = &#x222B;   1 W    u  1   ( x ) b ( x )   d  x   {\displaystyle A
      (x)=-\int {1 \over W}u_{2}(x)b(x)\,\mathrm {d} x,\;B(x)=\int {1 \over
      W}u_{1}(x)b(x)\,\mathrm {d} x}  [A(x) = - \int {1\over W} u_2(x) b
      (x)\,\mathrm dx,\; B(x) = \int {1 \over W} u_1(x)b(x)\,\mathrm dx]
Recall that for this example
         b ( x ) = cosh &#x2061; x   {\displaystyle b(x)=\cosh x}  [
      {\displaystyle b(x)=\cosh x}]
That is,
         A ( x ) = &#x2212; &#x222B;   1  e  &#x2212; 4 x     x  e  &#x2212; 2
      x   cosh &#x2061; x   d  x = &#x2212; &#x222B; x  e  2 x   cosh &#x2061;
      x   d  x = &#x2212;   1 18    e  x   ( 9 ( x &#x2212; 1 ) +  e  2 x   ( 3
      x &#x2212; 1 ) ) +  C  1     {\displaystyle A(x)=-\int {1 \over e^{-
      4x}}xe^{-2x}\cosh x\,\mathrm {d} x=-\int xe^{2x}\cosh x\,\mathrm {d} x=-
      {1 \over 18}e^{x}(9(x-1)+e^{2x}(3x-1))+C_{1}}  [{\displaystyle A(x)=-\int
      {1 \over e^{-4x}}xe^{-2x}\cosh x\,\mathrm {d} x=-\int xe^{2x}\cosh
      x\,\mathrm {d} x=-{1 \over 18}e^{x}(9(x-1)+e^{2x}(3x-1))+C_{1}}]
         B ( x ) = &#x222B;   1  e  &#x2212; 4 x      e  &#x2212; 2 x   cosh
      &#x2061; x   d  x = &#x222B;  e  2 x   cosh &#x2061; x   d  x =   1 6
      e  x   ( 3 +  e  2 x   ) +  C  2     {\displaystyle B(x)=\int {1 \over e^
      {-4x}}e^{-2x}\cosh x\,\mathrm {d} x=\int e^{2x}\cosh x\,\mathrm {d} x={1
      \over 6}e^{x}(3+e^{2x})+C_{2}}  [{\displaystyle B(x)=\int {1 \over e^{-
      4x}}e^{-2x}\cosh x\,\mathrm {d} x=\int e^{2x}\cosh x\,\mathrm {d} x={1
      \over 6}e^{x}(3+e^{2x})+C_{2}}]
where      C  1     {\displaystyle C_{1}}  [C_{1}] and      C  2
{\displaystyle C_{2}}  [C_{2}] are constants of integration.
**** General second-order equation[edit] ****
We have a differential equation of the form
          u &#x2033;  + p ( x )  u &#x2032;  + q ( x ) u = f ( x )
      {\displaystyle u''+p(x)u'+q(x)u=f(x)}  [{\displaystyle u''+p(x)u'+q(x)u=f
      (x)}]
and we define the linear operator
         L =  D  2   + p ( x ) D + q ( x )   {\displaystyle L=D^{2}+p(x)D+q(x)}
      [{\displaystyle L=D^{2}+p(x)D+q(x)}]
where D represents the differential_operator. We therefore have to solve the
equation     L u ( x ) = f ( x )   {\displaystyle Lu(x)=f(x)}  [L u(x)=f(x)]
for     u ( x )   {\displaystyle u(x)}  [u(x)], where     L   {\displaystyle L}
[L] and     f ( x )   {\displaystyle f(x)}  [f(x)] are known.
We must solve first the corresponding homogeneous equation:
          u &#x2033;  + p ( x )  u &#x2032;  + q ( x ) u = 0   {\displaystyle
      u''+p(x)u'+q(x)u=0}  [{\displaystyle u''+p(x)u'+q(x)u=0}]
by the technique of our choice. Once we've obtained two linearly independent
solutions to this homogeneous differential equation (because this ODE is
second-order) â call them u1 and u2 â we can proceed with variation of
parameters.
Now, we seek the general solution to the differential equation      u  G   ( x
)   {\displaystyle u_{G}(x)}  [ u_G(x)] which we assume to be of the form
          u  G   ( x ) = A ( x )  u  1   ( x ) + B ( x )  u  2   ( x ) .
      {\displaystyle u_{G}(x)=A(x)u_{1}(x)+B(x)u_{2}(x).}  [{\displaystyle u_
      {G}(x)=A(x)u_{1}(x)+B(x)u_{2}(x).}]
Here,     A ( x )   {\displaystyle A(x)}  [A(x)] and     B ( x )
{\displaystyle B(x)}  [B(x)] are unknown and      u  1   ( x )   {\displaystyle
u_{1}(x)}  [u_{1}(x)] and      u  2   ( x )   {\displaystyle u_{2}(x)}  [u_2
(x)] are the solutions to the homogeneous equation. (Observe that if     A ( x
)   {\displaystyle A(x)}  [A(x)] and     B ( x )   {\displaystyle B(x)}  [B(x)]
are constants, then     L  u  G   ( x ) = 0   {\displaystyle Lu_{G}(x)=0}
[Lu_G(x)=0].) Since the above is only one equation and we have two unknown
functions, it is reasonable to impose a second condition. We choose the
following:
          A &#x2032;  ( x )  u  1   ( x ) +  B &#x2032;  ( x )  u  2   ( x ) =
      0.   {\displaystyle A'(x)u_{1}(x)+B'(x)u_{2}(x)=0.}  [{\displaystyle A'
      (x)u_{1}(x)+B'(x)u_{2}(x)=0.}]
Now,
              u  G  &#x2032;  ( x )    =   (  A ( x )  u  1   ( x ) + B ( x )
      u  2   ( x )  )  &#x2032;        =   (  A ( x )  u  1   ( x )  )
      &#x2032;  +   (  B ( x )  u  2   ( x )  )  &#x2032;        =  A &#x2032;
      ( x )  u  1   ( x ) + A ( x )  u  1  &#x2032;  ( x ) +  B &#x2032;  ( x )
      u  2   ( x ) + B ( x )  u  2  &#x2032;  ( x )       =  A &#x2032;  ( x )
      u  1   ( x ) +  B &#x2032;  ( x )  u  2   ( x ) + A ( x )  u  1  &#x2032;
      ( x ) + B ( x )  u  2  &#x2032;  ( x )       = A ( x )  u  1  &#x2032;
      ( x ) + B ( x )  u  2  &#x2032;  ( x )       {\displaystyle {\begin
      {aligned}u_{G}'(x)&=\left(A(x)u_{1}(x)+B(x)u_{2}(x)\right)'\\&=\left(A
      (x)u_{1}(x)\right)'+\left(B(x)u_{2}(x)\right)'\\&=A'(x)u_{1}(x)+A(x)u_
      {1}'(x)+B'(x)u_{2}(x)+B(x)u_{2}'(x)\\&=A'(x)u_{1}(x)+B'(x)u_{2}(x)+A(x)u_
      {1}'(x)+B(x)u_{2}'(x)\\&=A(x)u_{1}'(x)+B(x)u_{2}'(x)\end{aligned}}}  [
      {\displaystyle {\begin{aligned}u_{G}'(x)&=\left(A(x)u_{1}(x)+B(x)u_{2}
      (x)\right)'\\&=\left(A(x)u_{1}(x)\right)'+\left(B(x)u_{2}
      (x)\right)'\\&=A'(x)u_{1}(x)+A(x)u_{1}'(x)+B'(x)u_{2}(x)+B(x)u_{2}'
      (x)\\&=A'(x)u_{1}(x)+B'(x)u_{2}(x)+A(x)u_{1}'(x)+B(x)u_{2}'(x)\\&=A(x)u_
      {1}'(x)+B(x)u_{2}'(x)\end{aligned}}}]
Differentiating again (omitting intermediary steps)
          u  G  &#x2033;  ( x ) = A ( x )  u  1  &#x2033;  ( x ) + B ( x )  u
      2  &#x2033;  ( x ) +  A &#x2032;  ( x )  u  1  &#x2032;  ( x ) +  B
      &#x2032;  ( x )  u  2  &#x2032;  ( x ) .   {\displaystyle u_{G}''(x)=A
      (x)u_{1}''(x)+B(x)u_{2}''(x)+A'(x)u_{1}'(x)+B'(x)u_{2}'(x).}  [
      {\displaystyle u_{G}''(x)=A(x)u_{1}''(x)+B(x)u_{2}''(x)+A'(x)u_{1}'(x)+B'
      (x)u_{2}'(x).}]
Now we can write the action of L upon uG as
         L  u  G   = A ( x ) L  u  1   ( x ) + B ( x ) L  u  2   ( x ) +  A
      &#x2032;  ( x )  u  1  &#x2032;  ( x ) +  B &#x2032;  ( x )  u  2
      &#x2032;  ( x ) .   {\displaystyle Lu_{G}=A(x)Lu_{1}(x)+B(x)Lu_{2}(x)+A'
      (x)u_{1}'(x)+B'(x)u_{2}'(x).}  [{\displaystyle Lu_{G}=A(x)Lu_{1}(x)+B
      (x)Lu_{2}(x)+A'(x)u_{1}'(x)+B'(x)u_{2}'(x).}]
Since u1 and u2 are solutions, then
         L  u  G   =  A &#x2032;  ( x )  u  1  &#x2032;  ( x ) +  B &#x2032;
      ( x )  u  2  &#x2032;  ( x ) .   {\displaystyle Lu_{G}=A'(x)u_{1}'(x)+B'
      (x)u_{2}'(x).}  [{\displaystyle Lu_{G}=A'(x)u_{1}'(x)+B'(x)u_{2}'(x).}]
We have the system of equations
           (     u  1   ( x )    u  2   ( x )      u  1  &#x2032;  ( x )    u
      2  &#x2032;  ( x )    )     (     A &#x2032;  ( x )      B &#x2032;  ( x
      )    )   =   (    0     f    )   .   {\displaystyle {\begin{pmatrix}u_{1}
      (x)&u_{2}(x)\\u_{1}'(x)&u_{2}'(x)\end{pmatrix}}{\begin{pmatrix}A'(x)\\B'
      (x)\end{pmatrix}}={\begin{pmatrix}0\\f\end{pmatrix}}.}  [\begin{pmatrix}
      u_1(x)  & u_2(x) \\
      u_1'(x) & u_2'(x) \end{pmatrix}
      \begin{pmatrix}
      A'(x) \\
      B'(x)\end{pmatrix} =
      \begin{pmatrix}
      0\\
      f\end{pmatrix}.]
Expanding,
           (     A &#x2032;  ( x )  u  1   ( x ) +  B &#x2032;  ( x )  u  2
      ( x )      A &#x2032;  ( x )  u  1  &#x2032;  ( x ) +  B &#x2032;  ( x )
      u  2  &#x2032;  ( x )    )   =   (    0     f    )   .   {\displaystyle
      {\begin{pmatrix}A'(x)u_{1}(x)+B'(x)u_{2}(x)\\A'(x)u_{1}'(x)+B'(x)u_{2}'
      (x)\end{pmatrix}}={\begin{pmatrix}0\\f\end{pmatrix}}.}  [{\displaystyle
      {\begin{pmatrix}A'(x)u_{1}(x)+B'(x)u_{2}(x)\\A'(x)u_{1}'(x)+B'(x)u_{2}'
      (x)\end{pmatrix}}={\begin{pmatrix}0\\f\end{pmatrix}}.}]
So the above system determines precisely the conditions
          A &#x2032;  ( x )  u  1   ( x ) +  B &#x2032;  ( x )  u  2   ( x ) =
      0.   {\displaystyle A'(x)u_{1}(x)+B'(x)u_{2}(x)=0.}  [{\displaystyle A'
      (x)u_{1}(x)+B'(x)u_{2}(x)=0.}]
          A &#x2032;  ( x )  u  1  &#x2032;  ( x ) +  B &#x2032;  ( x )  u  2
      &#x2032;  ( x ) = L  u  G   = f .   {\displaystyle A'(x)u_{1}'(x)+B'(x)u_
      {2}'(x)=Lu_{G}=f.}  [{\displaystyle A'(x)u_{1}'(x)+B'(x)u_{2}'(x)=Lu_
      {G}=f.}]
We seek A(x) and B(x) from these conditions, so, given
           (     u  1   ( x )    u  2   ( x )      u  1  &#x2032;  ( x )    u
      2  &#x2032;  ( x )    )     (     A &#x2032;  ( x )      B &#x2032;  ( x
      )    )   =   (    0     f    )     {\displaystyle {\begin{pmatrix}u_{1}
      (x)&u_{2}(x)\\u_{1}'(x)&u_{2}'(x)\end{pmatrix}}{\begin{pmatrix}A'(x)\\B'
      (x)\end{pmatrix}}={\begin{pmatrix}0\\f\end{pmatrix}}}  [\begin{pmatrix}
      u_1(x)  & u_2(x) \\
      u_1'(x) & u_2'(x) \end{pmatrix}
      \begin{pmatrix}
      A'(x) \\
      B'(x)\end{pmatrix} =
      \begin{pmatrix}
      0\\
      f\end{pmatrix}]
we can solve for (Aâ²(x), Bâ²(x))T, so
           (     A &#x2032;  ( x )      B &#x2032;  ( x )    )   =    (     u
      1   ( x )    u  2   ( x )      u  1  &#x2032;  ( x )    u  2  &#x2032;
      ( x )    )    &#x2212; 1     (    0     f    )   =   1 W     (     u  2
      &#x2032;  ( x )   &#x2212;  u  2   ( x )     &#x2212;  u  1  &#x2032;
      ( x )    u  1   ( x )    )     (    0     f    )   ,   {\displaystyle
      {\begin{pmatrix}A'(x)\\B'(x)\end{pmatrix}}={\begin{pmatrix}u_{1}(x)&u_{2}
      (x)\\u_{1}'(x)&u_{2}'(x)\end{pmatrix}}^{-1}{\begin{pmatrix}0\\f\end
      {pmatrix}}={\frac {1}{W}}{\begin{pmatrix}u_{2}'(x)&-u_{2}(x)\\-u_{1}'
      (x)&u_{1}(x)\end{pmatrix}}{\begin{pmatrix}0\\f\end{pmatrix}},}  [
      {\displaystyle {\begin{pmatrix}A'(x)\\B'(x)\end{pmatrix}}={\begin
      {pmatrix}u_{1}(x)&u_{2}(x)\\u_{1}'(x)&u_{2}'(x)\end{pmatrix}}^{-1}{\begin
      {pmatrix}0\\f\end{pmatrix}}={\frac {1}{W}}{\begin{pmatrix}u_{2}'(x)&-u_
      {2}(x)\\-u_{1}'(x)&u_{1}(x)\end{pmatrix}}{\begin{pmatrix}0\\f\end
      {pmatrix}},}]
where W denotes the Wronskian of u1 and u2. (We know that W is nonzero, from
the assumption that u1 and u2 are linearly independent.) So,
              A &#x2032;  ( x )    = &#x2212;   1 W    u  2   ( x ) f ( x ) ,
      B &#x2032;  ( x ) =   1 W    u  1   ( x ) f ( x )     A ( x )    =
      &#x2212; &#x222B;   1 W    u  2   ( x ) f ( x )   d  x ,  B ( x ) =
      &#x222B;   1 W    u  1   ( x ) f ( x )   d  x       {\displaystyle
      {\begin{aligned}A'(x)&=-{1 \over W}u_{2}(x)f(x),\;B'(x)={1 \over W}u_{1}
      (x)f(x)\\A(x)&=-\int {1 \over W}u_{2}(x)f(x)\,\mathrm {d} x,\;B(x)=\int
      {1 \over W}u_{1}(x)f(x)\,\mathrm {d} x\end{aligned}}}  [{\displaystyle
      {\begin{aligned}A'(x)&=-{1 \over W}u_{2}(x)f(x),\;B'(x)={1 \over W}u_{1}
      (x)f(x)\\A(x)&=-\int {1 \over W}u_{2}(x)f(x)\,\mathrm {d} x,\;B(x)=\int
      {1 \over W}u_{1}(x)f(x)\,\mathrm {d} x\end{aligned}}}]
While homogeneous equations are relatively easy to solve, this method allows
the calculation of the coefficients of the general solution of the
inhomogeneous equation, and thus the complete general solution of the
inhomogeneous equation can be determined.
Note that     A ( x )   {\displaystyle A(x)}  [A(x)] and     B ( x )
{\displaystyle B(x)}  [ B(x)] are each determined only up to an arbitrary
additive constant (the constant_of_integration). Adding a constant to     A ( x
)   {\displaystyle A(x)}  [A(x)] or     B ( x )   {\displaystyle B(x)}  [B(x)]
does not change the value of     L  u  G   ( x )   {\displaystyle Lu_{G}(x)}
[Lu_G(x)] because the extra term is just a linear combination of u1 and u2,
which is a solution of     L   {\displaystyle L}  [L] by definition.
***** References[edit] *****
   1. ^ See:
          o Forest_Ray_Moulton, An Introduction to Celestial Mechanics, 2nd ed.
            (first published by the Macmillan Company in 1914; reprinted in
            1970 by Dover Publications, Inc., Mineola, New York), page_431.
          o Edgar Odell Lovett (1899) "The_theory_of_perturbations_and_Lie's
            theory_of_contact_transformations," The Quarterly Journal of Pure
            and Applied Mathematics, vol. 30, pages 47â149; see especially
            pages 48â61.
   2. ^ Euler, L. (1748) "Recherches_sur_la_question_des_inÃ©galitÃ©s_du
      mouvement_de_Saturne_et_de_Jupiter,_sujet_proposÃ©_pour_le_prix_de
      l'annÃ©e_1748,_par_lâAcadÃ©mie_Royale_des_Sciences_de_Paris"
      [Investigations on the question of the differences in the movement of
      Saturn and Jupiter; this subject proposed for the prize of 1748 by the
      Royal Academy of Sciences (Paris)] (Paris, France: G. Martin, J.B.
      Coignard, & H.L. Guerin, 1749).
   3. ^ Euler, L. (1749) "Recherches_sur_la_prÃ©cession_des_Ã©quinoxes,_et_sur
      la_nutation_de_lâaxe_de_la_terre," Histoire [or MÃ©moires ] de
      l'AcadÃ©mie Royale des Sciences et Belles-lettres (Berlin), pages
      289â325 [published in 1751].
   4. ^ Euler, L. (1753) Theoria_motus_lunae:_exhibens_omnes_ejus
      inaequalitates_... [The theory of the motion of the moon: demonstrating
      all of its inequalities ... ] (Saint Petersburg, Russia: Academia
      Imperialis Scientiarum Petropolitanae [Imperial Academy of Science (St.
      Petersburg)], 1753).
   5. ^ Lagrange, J.-L. (1766) âSolution_de_diffÃ©rens_problÃ¨mes_du_calcul
      integral,â MÃ©langes de philosophie et de mathÃ©matique de la SociÃ©tÃ©
      royale de Turin, vol. 3, pages 179â380.
   6. ^ See:
          o Lagrange, J.-L. (1781) "ThÃ©orie_des_variations_sÃ©culaires_des
            Ã©lÃ©mens_des_Planetes._Premiere_partie,_..._," Nouveaux MÃ©moires
            de l'AcadÃ©mie Royale des Sciences et Belles-lettres (Berlin),
            pages 199â276.
          o Lagrange, J.-L. (1782) "ThÃ©orie_des_variations_sÃ©culaires_des
            Ã©lÃ©mens_des_Planetes._Seconde_partie,_..._," Nouveaux MÃ©moires
            de l'AcadÃ©mie Royale des Sciences et Belles-lettres (Berlin),
            pages 169â292.
          o Lagrange, J.-L. (1783) "ThÃ©orie_des_variations_pÃ©riodiques_des
            mouvemens_des_Planetes._Premiere_partie,_..._," Nouveaux MÃ©moires
            de l'AcadÃ©mie Royale des Sciences et Belles-lettres (Berlin),
            pages 161â190.
   7. ^ See:
          o Lagrange, J.-L. (1778) "Sur_le_probleme_de_la_dÃ©termination_des
            orbites_des_cometes_d'aprÃ¨s_trois_observations,_premier_mÃ©moire"
            (On the problem of determining the orbits of comets from three
            observations, first memoir), Nouveaux MÃ©moires de l'AcadÃ©mie
            Royale des Sciences et Belles-lettres (Berlin), pages 111â123
            [published in 1780].
          o Lagrange, J.-L. (1778) "Sur_le_probleme_de_la_dÃ©termination_des
            orbites_des_cometes_d'aprÃ¨s_trois_observations,_second_mÃ©moire",
            Nouveaux MÃ©moires de l'AcadÃ©mie Royale des Sciences et Belles-
            lettres (Berlin), pages 124â161 [published in 1780].
          o Lagrange, J.-L. (1783) "Sur_le_probleme_de_la_dÃ©termination_des
            orbites_des_cometes_d'aprÃ¨s_trois_observations._TroisiÃ¨me
            mÃ©moire,_dans_lequel_on_donne_une_solution_directe_et_gÃ©nÃ©rale
            du_problÃ¨me.", Nouveaux MÃ©moires de l'AcadÃ©mie Royale des
            Sciences et Belles-lettres (Berlin), pages 296â332 [published in
            1785].
   8. ^ Michael Efroimsky (2002) "Implicit_gauge_symmetry_emerging_in_the_N-
      body_problem_of_celestial_mechanics," page 3.
   9. ^ See:
          o Lagrange, J.-L. (1808) âSur la thÃ©orie des variations des
            Ã©lÃ©ments des planÃ¨tes et en particulier des variations des
            grands axes de leurs orbites,â MÃ©moires de la premiÃ¨re Classe
            de lâInstitut de France. Reprinted in: Joseph-Louis Lagrange with
            Joseph-Alfred Serret, ed., Oeuvres de Lagrange (Paris, France:
            Gauthier-Villars, 1873), vol. 6, pages_713â768.
          o Lagrange, J.-L. (1809) âSur la thÃ©orie gÃ©nÃ©rale de la
            variation des constantes arbitraires dans tous les problÃ¨mes de la
            mÃ©chanique,â MÃ©moires de la premiÃ¨re Classe de lâInstitut de
            France. Reprinted in: Joseph-Louis Lagrange with Joseph-Alfred
            Serret, ed., Oeuvres de Lagrange (Paris, France: Gauthier-Villars,
            1873), vol. 6, pages_771â805.
          o Lagrange, J.-L. (1810) âSecond mÃ©moire sur la thÃ©orie
            gÃ©nÃ©rale de la variation des constantes arbitraires dans tous les
            problÃ¨mes de la mÃ©chanique, ... ,â MÃ©moires de la premiÃ¨re
            Classe de lâInstitut de France. Reprinted in: Joseph-Louis
            Lagrange with Joseph-Alfred Serret, ed., Oeuvres de Lagrange
            (Paris, France: Gauthier-Villars, 1873), vol. 6, pages_809â816.
  10. ^ See:
          o Michael Efroimsky (2005) "Gauge_Freedom_in_Orbital_Mechanics."
            ANYAS,_Vol._1065,_pp._346â374_(2005)
          o Michael Efroimsky and Peter Goldreich (2004) "Gauge_symmetry_of_the
            N-body_problem_of_Celestial_Mechanics."_Astronomy_and_Astrophysics,
            Vol._415,_pp._1187â1199._(2004)
          o Michael Efroimsky and Peter Goldreich (2003) "Gauge_symmetry_of_the
            N-body_problem_in_the_HamiltonâJacobi_approach."_Journal_of
            Mathematical_Physics,_Vol._44,_pp._5958â5977._(2003)
    * Coddington, Earl A.; Levinson, Norman (1955). Theory of Ordinary
      Differential Equations. New York: McGraw-Hill.
Boyce, W. E.; DiPrima, R. C. (1965). Elementary Differential Equations and
Boundary Value Problems 8th Edition. Wiley Interscience.
, pages 186â192, 237â241
Teschl,_Gerald. Ordinary_Differential_Equations_and_Dynamical_Systems.
Providence: American_Mathematical_Society.
***** External links[edit] *****
    * Online_Notes_/_Proof by Paul Dawkins, Lamar_University.
    * PlanetMath_page.
    * A_NOTE_ON_LAGRANGEâS_METHOD_OF_VARIATION_OF_PARAMETERS

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Variation_of_parameters&oldid=908485160"
Categories:
    * Ordinary_differential_equations
Hidden categories:
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 30 July 2019, at 01:08 (UTC).
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
