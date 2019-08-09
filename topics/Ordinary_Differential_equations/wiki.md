The following text has been accessed from https://en.wikipedia.org/wiki/Ordinary_differential_equation at Fri Aug 9 02:32:04 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Ordinary differential equation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, an ordinary differential equation (ODE) is a differential
equation containing one or more functions of one independent_variable and the
derivatives of those functions.[1] The term ordinary is used in contrast with
the term partial_differential_equation which may be with respect to more than
one independent variable.[2]
⁰
***** Contents *****
    * 1_Differential_equations
    * 2_Background
    * 3_Definitions
          o 3.1_General_definition
          o 3.2_System_of_ODEs
          o 3.3_Solutions
    * 4_Theories
          o 4.1_Singular_solutions
          o 4.2_Reduction_to_quadratures
          o 4.3_Fuchsian_theory
          o 4.4_Lie's_theory
          o 4.5_SturmâLiouville_theory
    * 5_Existence_and_uniqueness_of_solutions
          o 5.1_Local_existence_and_uniqueness_theorem_simplified
          o 5.2_Global_uniqueness_and_maximum_domain_of_solution
    * 6_Reduction_of_order
          o 6.1_Reduction_to_a_first-order_system
    * 7_Summary_of_exact_solutions
    * 8_Software_for_ODE_solving
    * 9_See_also
    * 10_Notes
    * 11_References
    * 12_Bibliography
    * 13_External_links
***** Differential equations[edit] *****
A linear_differential_equation is a differential equation that is defined by a
linear_polynomial in the unknown function and its derivatives, that is an
equation of the form
          a  0   ( x ) y +  a  1   ( x )  y &#x2032;  +  a  2   ( x )  y
      &#x2033;  + &#x22EF; +  a  n   ( x )  y  ( n )   + b ( x ) = 0 ,
      {\displaystyle a_{0}(x)y+a_{1}(x)y'+a_{2}(x)y''+\cdots +a_{n}(x)y^{(n)}+b
      (x)=0,}  [{\displaystyle a_{0}(x)y+a_{1}(x)y'+a_{2}(x)y''+\cdots +a_{n}
      (x)y^{(n)}+b(x)=0,}]
where      a  0   ( x )   {\displaystyle a_{0}(x)}  [{\displaystyle a_{0}(x)}],
...,      a  n   ( x )   {\displaystyle a_{n}(x)}  [{\displaystyle a_{n}(x)}]
and     b ( x )   {\displaystyle b(x)}  [b(x)] are arbitrary differentiable
functions that do not need to be linear, and      y &#x2032;  , &#x2026; ,  y
( n )     {\displaystyle y',\ldots ,y^{(n)}}  [{\displaystyle y',\ldots ,y^{
(n)}}] are the successive derivatives of the unknown function y of the variable
x.
Among ordinary differential equations, linear differential equations play a
prominent role for several reasons. Most elementary and special functions that
are encountered in physics and applied_mathematics are solutions of linear
differential equations (see Holonomic_function). When physical phenomena are
modeled with non-linear equations, they are generally approximated by linear
differential equations for an easier solution. The few non-linear ODEs that can
be solved explicitly are generally solved by transforming the equation into an
equivalent linear ODE (see, for example Riccati_equation).
Some ODEs can be solved explicitly in terms of known functions and integrals.
When that is not possible, the equation for computing the Taylor_series of the
solutions may be useful. For applied problems, numerical_methods_for_ordinary
differential_equations can supply an approximation of the solution.
***** Background[edit] *****
[parabolic_projectile_motion_showing_velocity_vector]
The trajectory of a projectile launched from a cannon follows a curve
determined by an ordinary differential equation that is derived from Newton's
second law.
Ordinary differential equations (ODEs) arise in many contexts of mathematics
and social and natural sciences. Mathematical descriptions of change use
differentials and derivatives. Various differentials, derivatives, and
functions become related via equations, such that a differential equation is a
result that describes dynamically changing phenomena, evolution, and variation.
Often, quantities are defined as the rate of change of other quantities (for
example, derivatives of displacement with respect to time), or gradients of
quantities, which is how they enter differential equations.
Specific mathematical fields include geometry and analytical_mechanics.
Scientific fields include much of physics and astronomy (celestial mechanics),
meteorology (weather modelling), chemistry (reaction rates),[3] biology
(infectious diseases, genetic variation), ecology and population_modelling
(population competition), economics (stock trends, interest rates and the
market equilibrium price changes).
Many mathematicians have studied differential equations and contributed to the
field, including Newton, Leibniz, the Bernoulli_family, Riccati, Clairaut,
d'Alembert, and Euler.
A simple example is Newton's_second_law of motion — the relationship between
the displacement x and the time t of an object under the force F, is given by
the differential equation
         m      d   2   x ( t )    d   t  2      = F ( x ( t ) )
      {\displaystyle m{\frac {\mathrm {d} ^{2}x(t)}{\mathrm {d} t^{2}}}=F(x
      (t))\,}  [{\displaystyle m{\frac {\mathrm {d} ^{2}x(t)}{\mathrm {d} t^
      {2}}}=F(x(t))\,}]
which constrains the motion of a particle of constant mass m. In general, F is
a function of the position x(t) of the particle at time t. The unknown function
x(t) appears on both sides of the differential equation, and is indicated in
the notation F(x(t)).[4][5][6][7]
***** Definitions[edit] *****
In what follows, let y be a dependent_variable and x an independent_variable,
and y = f(x) is an unknown function of x. The notation_for_differentiation
varies depending upon the author and upon which notation is most useful for the
task at hand. In this context, the Leibniz's_notation (dy/dx,d2y/dx2,...,dny/
dxn) is more useful for differentiation and integration, whereas Lagrange's
notation (y′,y′′, ..., y(n)) is more useful for representing derivatives of any
order compactly, and Newton's_notation     (    y &#x02D9;    ,    y &#x00A8;
,   y  . . .    )   {\displaystyle ({\dot {y}},{\ddot {y}},{\overset {...}
{y}})}  [{\displaystyle ({\dot {y}},{\ddot {y}},{\overset {...}{y}})}] is often
used in physics for representing derivatives of low order with respect to time.
**** General definition[edit] ****
Given F, a function of x, y, and derivatives of y. Then an equation of the form
         F  (  x , y ,  y &#x2032;  , &#x2026; ,  y  ( n &#x2212; 1 )    )  =
      y  ( n )     {\displaystyle F\left(x,y,y',\ldots ,y^{(n-1)}\right)=y^{
      (n)}}  [{\displaystyle F\left(x,y,y',\ldots ,y^{(n-1)}\right)=y^{(n)}}]
is called an explicit ordinary differential equation of order n.[8][9]
More generally, an implicit ordinary differential equation of order n takes the
form:[10]
         F  (  x , y ,  y &#x2032;  ,  y &#x2033;  , &#xA0; &#x2026; , &#xA0;
      y  ( n )    )  = 0   {\displaystyle F\left(x,y,y',y'',\ \ldots ,\ y^{
      (n)}\right)=0}  [{\displaystyle F\left(x,y,y',y'',\ \ldots ,\ y^{
      (n)}\right)=0}]
There are further classifications:
  Homogeneous
      If r(x) = 0, and consequently one "automatic" solution is the trivial
      solution, y = 0. The solution of a linear homogeneous equation is a
      complementary function, denoted here by yc.
  Nonhomogeneous (or inhomogeneous)
      If r(x) â  0. The additional solution to the complementary function is
      the particular integral, denoted here by yp.
The general solution to a linear equation can be written as y = yc + yp.
Non-linear
A differential equation that cannot be written in the form of a linear
combination.
**** System of ODEs[edit] ****
A number of coupled differential equations form a system of equations. If y is
a vector whose elements are functions; y(x) = [y1(x), y2(x),..., ym(x)], and F
is a vector-valued_function of y and its derivatives, then
           y   ( n )   =  F   (  x ,  y  ,   y  &#x2032;  ,   y  &#x2033;  ,
      &#x2026; ,   y   ( n &#x2212; 1 )    )    {\displaystyle \mathbf {y} ^{
      (n)}=\mathbf {F} \left(x,\mathbf {y} ,\mathbf {y} ',\mathbf {y} '',\ldots
      ,\mathbf {y} ^{(n-1)}\right)}  [{\displaystyle \mathbf {y} ^{(n)}=\mathbf
      {F} \left(x,\mathbf {y} ,\mathbf {y} ',\mathbf {y} '',\ldots ,\mathbf {y}
      ^{(n-1)}\right)}]
is an explicit system of ordinary differential equations of order n and
dimension m. In column_vector form:
           (     y  1   ( n )        y  2   ( n )       &#x22EE;      y  m
      ( n )      )   =   (     f  1    (  x ,  y  ,   y  &#x2032;  ,   y
      &#x2033;  , &#x2026; ,   y   ( n &#x2212; 1 )    )       f  2    (  x ,
      y  ,   y  &#x2032;  ,   y  &#x2033;  , &#x2026; ,   y   ( n &#x2212; 1 )
      )      &#x22EE;      f  m    (  x ,  y  ,   y  &#x2032;  ,   y  &#x2033;
      , &#x2026; ,   y   ( n &#x2212; 1 )    )     )     {\displaystyle {\begin
      {pmatrix}y_{1}^{(n)}\\y_{2}^{(n)}\\\vdots \\y_{m}^{(n)}\end{pmatrix}}=
      {\begin{pmatrix}f_{1}\left(x,\mathbf {y} ,\mathbf {y} ',\mathbf {y}
      '',\ldots ,\mathbf {y} ^{(n-1)}\right)\\f_{2}\left(x,\mathbf {y} ,\mathbf
      {y} ',\mathbf {y} '',\ldots ,\mathbf {y} ^{(n-1)}\right)\\\vdots \\f_
      {m}\left(x,\mathbf {y} ,\mathbf {y} ',\mathbf {y} '',\ldots ,\mathbf {y}
      ^{(n-1)}\right)\end{pmatrix}}}  [{\displaystyle {\begin{pmatrix}y_{1}^{
      (n)}\\y_{2}^{(n)}\\\vdots \\y_{m}^{(n)}\end{pmatrix}}={\begin{pmatrix}f_
      {1}\left(x,\mathbf {y} ,\mathbf {y} ',\mathbf {y} '',\ldots ,\mathbf {y}
      ^{(n-1)}\right)\\f_{2}\left(x,\mathbf {y} ,\mathbf {y} ',\mathbf {y}
      '',\ldots ,\mathbf {y} ^{(n-1)}\right)\\\vdots \\f_{m}\left(x,\mathbf {y}
      ,\mathbf {y} ',\mathbf {y} '',\ldots ,\mathbf {y} ^{(n-1)}\right)\end
      {pmatrix}}}]
These are not necessarily linear. The implicit analogue is:
          F   (  x ,  y  ,   y  &#x2032;  ,   y  &#x2033;  , &#x2026; ,   y
      ( n )    )  =  0    {\displaystyle \mathbf {F} \left(x,\mathbf {y}
      ,\mathbf {y} ',\mathbf {y} '',\ldots ,\mathbf {y} ^{(n)}\right)=
      {\boldsymbol {0}}}  [{\displaystyle \mathbf {F} \left(x,\mathbf {y}
      ,\mathbf {y} ',\mathbf {y} '',\ldots ,\mathbf {y} ^{(n)}\right)=
      {\boldsymbol {0}}}]
where 0 = (0, 0, ..., 0) is the zero_vector. In matrix form
           (     f  1   ( x ,  y  ,   y  &#x2032;  ,   y  &#x2033;  , &#x2026;
      ,   y   ( n )   )      f  2   ( x ,  y  ,   y  &#x2032;  ,   y  &#x2033;
      , &#x2026; ,   y   ( n )   )     &#x22EE;      f  m   ( x ,  y  ,   y
      &#x2032;  ,   y  &#x2033;  , &#x2026; ,   y   ( n )   )    )   =   (    0
      0     &#x22EE;     0    )     {\displaystyle {\begin{pmatrix}f_{1}
      (x,\mathbf {y} ,\mathbf {y} ',\mathbf {y} '',\ldots ,\mathbf {y} ^{
      (n)})\\f_{2}(x,\mathbf {y} ,\mathbf {y} ',\mathbf {y} '',\ldots ,\mathbf
      {y} ^{(n)})\\\vdots \\f_{m}(x,\mathbf {y} ,\mathbf {y} ',\mathbf {y}
      '',\ldots ,\mathbf {y} ^{(n)})\end{pmatrix}}={\begin{pmatrix}0\\0\\\vdots
      \\0\end{pmatrix}}}  [{\displaystyle {\begin{pmatrix}f_{1}(x,\mathbf {y}
      ,\mathbf {y} ',\mathbf {y} '',\ldots ,\mathbf {y} ^{(n)})\\f_{2}
      (x,\mathbf {y} ,\mathbf {y} ',\mathbf {y} '',\ldots ,\mathbf {y} ^{
      (n)})\\\vdots \\f_{m}(x,\mathbf {y} ,\mathbf {y} ',\mathbf {y} '',\ldots
      ,\mathbf {y} ^{(n)})\end{pmatrix}}={\begin{pmatrix}0\\0\\\vdots \\0\end
      {pmatrix}}}]
For a system of the form      F   (  x ,  y  ,   y  &#x2032;   )  =  0
{\displaystyle \mathbf {F} \left(x,\mathbf {y} ,\mathbf {y} '\right)=
{\boldsymbol {0}}}  [\mathbf {F} \left(x,\mathbf {y} ,\mathbf {y} '\right)=
{\boldsymbol {0}}], some sources also require that the Jacobian_matrix
&#x2202;  F  ( x ,  u  ,  v  )   &#x2202;  v       {\displaystyle {\frac
{\partial \mathbf {F} (x,\mathbf {u} ,\mathbf {v} )}{\partial \mathbf {v} }}}
[{\frac {\partial \mathbf {F} (x,\mathbf {u} ,\mathbf {v} )}{\partial \mathbf
{v} }}] be non-singular in order to call this an implicit ODE [system]; an
implicit ODE system satisfying this Jacobian non-singularity condition can be
transformed into an explicit ODE system. In the same sources, implicit ODE
systems with a singular Jacobian are termed differential_algebraic_equations
(DAEs). This distinction is not merely one of terminology; DAEs have
fundamentally different characteristics and are generally more involved to
solve than (nonsingular) ODE systems.[14][15] Presumably for additional
derivatives, the Hessian_matrix and so forth are also assumed non-singular
according to this scheme,[citation_needed] although note that any_ODE_of_order
greater_than_one_can_be_[and_usually_is]_rewritten_as_system_of_ODEs_of_first
order,[16] which makes the Jacobian singularity criterion sufficient for this
taxonomy to be comprehensive at all orders.
The behavior of a system of ODEs can be visualized through the use of a phase
portrait.
**** Solutions[edit] ****
Given a differential equation
         F  (  x , y ,  y &#x2032;  , &#x2026; ,  y  ( n )    )  = 0
      {\displaystyle F\left(x,y,y',\ldots ,y^{(n)}\right)=0}  [{\displaystyle
      F\left(x,y,y',\ldots ,y^{(n)}\right)=0}]
a function u: I â R â R is called a solution or integral_curve for F, if u
is n-times differentiable on I, and
         F ( x , u ,  u &#x2032;  , &#xA0; &#x2026; , &#xA0;  u  ( n )   ) = 0
      x &#x2208; I .   {\displaystyle F(x,u,u',\ \ldots ,\ u^{(n)})=0\quad x\in
      I.}  [{\displaystyle F(x,u,u',\ \ldots ,\ u^{(n)})=0\quad x\in I.}]
Given two solutions u: J â R â R and v: I â R â R, u is called an
extension of v if I â J and
         u ( x ) = v ( x )  x &#x2208; I .    {\displaystyle u(x)=v(x)\quad
      x\in I.\,}  [u(x)=v(x)\quad x\in I.\,]
A solution that has no extension is called a maximal solution. A solution
defined on all of R is called a global solution.
A general solution of an nth-order equation is a solution containing n
arbitrary independent constants_of_integration. A particular solution is
derived from the general solution by setting the constants to particular
values, often chosen to fulfill set 'initial_conditions or boundary
conditions'.[17] A singular_solution is a solution that cannot be obtained by
assigning definite values to the arbitrary constants in the general solution.
[18]
***** Theories[edit] *****
**** Singular solutions[edit] ****
The theory of singular_solutions of ordinary and partial_differential_equations
was a subject of research from the time of Leibniz, but only since the middle
of the nineteenth century has it received special attention. A valuable but
little-known work on the subject is that of Houtain (1854). Darboux (from 1873)
was a leader in the theory, and in the geometric interpretation of these
solutions he opened a field worked by various writers, notably Casorati and
Cayley. To the latter is due (1872) the theory of singular solutions of
differential equations of the first order as accepted circa 1900.
**** Reduction to quadratures[edit] ****
The primitive attempt in dealing with differential equations had in view a
reduction to quadratures. As it had been the hope of eighteenth-century
algebraists to find a method for solving the general equation of the nth
degree, so it was the hope of analysts to find a general method for integrating
any differential equation. Gauss (1799) showed, however, that complex
differential equations require complex_numbers. Hence, analysts began to
substitute the study of functions, thus opening a new and fertile field. Cauchy
was the first to appreciate the importance of this view. Thereafter, the real
question was no longer whether a solution is possible by means of known
functions or their integrals, but whether a given differential equation
suffices for the definition of a function of the independent variable or
variables, and, if so, what are the characteristic properties.
**** Fuchsian theory[edit] ****
Main article: Frobenius_method
Two memoirs by Fuchs[19] inspired a novel approach, subsequently elaborated by
ThomÃ© and Frobenius. Collet was a prominent contributor beginning in 1869. His
method for integrating a non-linear system was communicated to Bertrand in
1868. Clebsch (1873) attacked the theory along lines parallel to those in his
theory of Abelian_integrals. As the latter can be classified according to the
properties of the fundamental curve that remains unchanged under a rational
transformation, Clebsch proposed to classify the transcendent functions defined
by differential equations according to the invariant properties of the
corresponding surfaces f = 0 under rational one-to-one transformations.
**** Lie's theory[edit] ****
From 1870, Sophus_Lie's work put the theory of differential equations on a
better foundation. He showed that the integration theories of the older
mathematicians can, using Lie_groups, be referred to a common source, and that
ordinary differential equations that admit the same infinitesimal
transformations present comparable integration difficulties. He also emphasized
the subject of transformations_of_contact.
Lie's group theory of differential equations has been certified, namely: (1)
that it unifies the many ad hoc methods known for solving differential
equations, and (2) that it provides powerful new ways to find solutions. The
theory has applications to both ordinary and partial differential equations.
[20]
A general solution approach uses the symmetry property of differential
equations, the continuous infinitesimal_transformations of solutions to
solutions (Lie_theory). Continuous group_theory, Lie_algebras, and differential
geometry are used to understand the structure of linear and nonlinear (partial)
differential equations for generating integrable equations, to find its Lax
pairs, recursion operators, BÃ¤cklund_transform, and finally finding exact
analytic solutions to DE.
Symmetry methods have been applied to differential equations that arise in
mathematics, physics, engineering, and other disciplines.
**** SturmâLiouville theory[edit] ****
Main article: SturmâLiouville_theory
SturmâLiouville theory is a theory of a special type of second order linear
ordinary differential equation. Their solutions are based on eigenvalues and
corresponding eigenfunctions of linear operators defined via second-order
homogeneous_linear_equations. The problems are identified as Sturm-Liouville
Problems (SLP) and are named after J.C.F._Sturm and J._Liouville, who studied
them in the mid-1800s. SLPs have an infinite number of eigenvalues, and the
corresponding eigenfunctions form a complete, orthogonal set, which makes
orthogonal expansions possible. This is a key idea in applied mathematics,
physics, and engineering.[21] SLPs are also useful in the analysis of certain
partial differential equations.
***** Existence and uniqueness of solutions[edit] *****
There are several theorems that establish existence and uniqueness of solutions
to initial value problems involving ODEs both locally and globally. The two
main theorems are
      Theorem                    Assumption             Conclusion
      Peano_existence_theorem    F continuous           local existence only
      PicardâLindelÃ¶f_theF Lipschitz_continuous local existence and
                                                        uniqueness
In their basic form both of these theorems only guarantee local results, though
the latter can be extended to give a global result, for example, if the
conditions of GrÃ¶nwall's_inequality are met.
Also, uniqueness theorems like the Lipschitz one above do not apply to DAE
systems, which may have multiple solutions stemming from their (non-linear)
algebraic part alone.[22]
**** Local existence and uniqueness theorem simplified[edit] ****
The theorem can be stated simply as follows.[23] For the equation and initial
value problem:
          y &#x2032;  = F ( x , y )  ,   y  0   = y (  x  0   )
      {\displaystyle y'=F(x,y)\,,\quad y_{0}=y(x_{0})}  [y'=F(x,y)\,,\quad y_
      {0}=y(x_{0})]
if F and âF/ây are continuous in a closed rectangle
         R = [  x  0   &#x2212; a ,  x  0   + a ] &#x00D7; [  y  0   &#x2212; b
      ,  y  0   + b ]   {\displaystyle R=[x_{0}-a,x_{0}+a]\times [y_{0}-b,y_
      {0}+b]}  [R=[x_{0}-a,x_{0}+a]\times [y_{0}-b,y_{0}+b]]
in the x-y plane, where a and b are real (symbolically: a, b â â) and Ã
denotes the cartesian_product, square brackets denote closed_intervals, then
there is an interval
         I = [  x  0   &#x2212; h ,  x  0   + h ] &#x2282; [  x  0   &#x2212; a
      ,  x  0   + a ]   {\displaystyle I=[x_{0}-h,x_{0}+h]\subset [x_{0}-a,x_
      {0}+a]}  [I=[x_{0}-h,x_{0}+h]\subset [x_{0}-a,x_{0}+a]]
for some h â â where the solution to the above equation and initial value
problem can be found. That is, there is a solution and it is unique. Since
there is no restriction on F to be linear, this applies to non-linear equations
that take the form F(x, y), and it can also be applied to systems of equations.
**** Global uniqueness and maximum domain of solution[edit] ****
When the hypotheses of the PicardâLindelÃ¶f theorem are satisfied, then local
existence and uniqueness can be extended to a global result. More precisely:
[24]
For each initial condition (x0, y0) there exists a unique maximum (possibly
infinite) open interval
          I  max   = (  x  &#x2212;   ,  x  +   ) ,  x  &#x00B1;   &#x2208;  R
      &#x222A; { &#x00B1; &#x221E; } ,  x  0   &#x2208;  I  max
      {\displaystyle I_{\max }=(x_{-},x_{+}),x_{\pm }\in \mathbb {R} \cup \{\pm
      \infty \},x_{0}\in I_{\max }}  [{\displaystyle I_{\max }=(x_{-},x_{+}),x_
      {\pm }\in \mathbb {R} \cup \{\pm \infty \},x_{0}\in I_{\max }}]
such that any solution that satisfies this initial condition is a restriction
of the solution that satisfies this initial condition with domain      I  max
{\displaystyle I_{\max }}  [I_{\max }].
In the case that      x  &#x00B1;   &#x2260; &#x00B1; &#x221E;   {\displaystyle
x_{\pm }\neq \pm \infty }  [{\displaystyle x_{\pm }\neq \pm \infty }], there
are exactly two possibilities
    * explosion in finite time:      lim&#x2006;sup  x &#x2192;  x  &#x00B1;
      &#x2016; y ( x ) &#x2016; &#x2192; &#x221E;   {\displaystyle \limsup _
      {x\to x_{\pm }}\|y(x)\|\to \infty }  [{\displaystyle \limsup _{x\to x_
      {\pm }}\|y(x)\|\to \infty }]
    * leaves domain of definition:      lim  x &#x2192;  x  &#x00B1;     y ( x
      ) &#xA0; &#x2208; &#x2202;    &#x03A9; &#x00AF;      {\displaystyle \lim
      _{x\to x_{\pm }}y(x)\ \in \partial {\bar {\Omega }}}  [\lim _{x\to x_{\pm
      }}y(x)\ \in \partial {\bar {\Omega }}]
where Î© is the open set in which F is defined, and     &#x2202;    &#x03A9;
&#x00AF;      {\displaystyle \partial {\bar {\Omega }}}  [\partial {\bar
{\Omega }}] is its boundary.
Note that the maximum domain of the solution
    * is always an interval (to have uniqueness)
    * may be smaller than      R    {\displaystyle \mathbb {R} }  [\mathbb {R}
      ]
    * may depend on the specific choice of (x0, y0).
  Example.
          y &#x2032;  =  y  2     {\displaystyle y'=y^{2}}  [y'=y^{2}]
This means that F(x, y) = y2, which is C1 and therefore locally Lipschitz
continuous, satisfying the PicardâLindelÃ¶f theorem.
Even in such a simple setting, the maximum domain of solution cannot be all
R    {\displaystyle \mathbb {R} }  [\mathbb {R} ] since the solution is
         y ( x ) =    y  0    (  x  0   &#x2212; x )  y  0   + 1
      {\displaystyle y(x)={\frac {y_{0}}{(x_{0}-x)y_{0}+1}}}  [y(x)={\frac {y_
      {0}}{(x_{0}-x)y_{0}+1}}]
which has maximum domain:
           {     R     y  0   = 0      (  &#x2212; &#x221E; ,  x  0   +   1  y
      0      )     y  0   > 0      (   x  0   +   1  y  0     , + &#x221E;  )
      y  0   < 0         {\displaystyle {\begin{cases}\mathbb {R} &y_{0}=0\\
      [4pt]\left(-\infty ,x_{0}+{\frac {1}{y_{0}}}\right)&y_{0}>0\\[4pt]\left
      (x_{0}+{\frac {1}{y_{0}}},+\infty \right)&y_{0}<0\end{cases}}}  [
      {\displaystyle {\begin{cases}\mathbb {R} &y_{0}=0\\[4pt]\left(-\infty ,x_
      {0}+{\frac {1}{y_{0}}}\right)&y_{0}>0\\[4pt]\left(x_{0}+{\frac {1}{y_
      {0}}},+\infty \right)&y_{0}<0\end{cases}}}]
This shows clearly that the maximum interval may depend on the initial
conditions. The domain of y could be taken as being      R  &#x2216; (  x  0
+ 1  /   y  0   ) ,   {\displaystyle \mathbb {R} \setminus (x_{0}+1/y_{0}),}  [
{\displaystyle \mathbb {R} \setminus (x_{0}+1/y_{0}),}] but this would lead to
a domain that is not an interval, so that the side opposite to the initial
condition would be disconnected from the initial condition, and therefore not
uniquely determined by it.
The maximum domain is not      R    {\displaystyle \mathbb {R} }  [\mathbb {R}
] because
          lim  x &#x2192;  x  &#x00B1;     &#x2016; y ( x ) &#x2016; &#x2192;
      &#x221E; ,   {\displaystyle \lim _{x\to x_{\pm }}\|y(x)\|\to \infty ,}  [
      {\displaystyle \lim _{x\to x_{\pm }}\|y(x)\|\to \infty ,}]
which is one of the two possible cases according to the above theorem.
***** Reduction of order[edit] *****
Differential equations can usually be solved more easily if the order of the
equation can be reduced.
**** Reduction to a first-order system[edit] ****
Any explicit differential equation of order n,
         F  (  x , y ,  y &#x2032;  ,  y &#x2033;  , &#xA0; &#x2026; , &#xA0;
      y  ( n &#x2212; 1 )    )  =  y  ( n )     {\displaystyle F\left
      (x,y,y',y'',\ \ldots ,\ y^{(n-1)}\right)=y^{(n)}}  [{\displaystyle F\left
      (x,y,y',y'',\ \ldots ,\ y^{(n-1)}\right)=y^{(n)}}]
can be written as a system of n first-order differential equations by defining
a new family of unknown functions
          y  i   =  y  ( i &#x2212; 1 )   .    {\displaystyle y_{i}=y^{(i-
      1)}.\!}  [y_{i}=y^{(i-1)}.\!]
for i = 1, 2,..., n. The n-dimensional system of first-order coupled
differential equations is then
              y  1  &#x2032;    =    y  2        y  2  &#x2032;    =    y  3
      &#x22EE;       y  n &#x2212; 1  &#x2032;    =    y  n        y  n
      &#x2032;    =   F ( x ,  y  1   , &#x2026; ,  y  n   ) .
      {\displaystyle {\begin{array}{rcl}y_{1}'&=&y_{2}\\y_{2}'&=&y_{3}\\&\vdots
      &\\y_{n-1}'&=&y_{n}\\y_{n}'&=&F(x,y_{1},\ldots ,y_{n}).\end{array}}}  [
      {\displaystyle {\begin{array}{rcl}y_{1}'&=&y_{2}\\y_{2}'&=&y_{3}\\&\vdots
      &\\y_{n-1}'&=&y_{n}\\y_{n}'&=&F(x,y_{1},\ldots ,y_{n}).\end{array}}}]
more compactly in vector notation:
           y  &#x2032;  =  F  ( x ,  y  )   {\displaystyle \mathbf {y}
      '=\mathbf {F} (x,\mathbf {y} )}  [\mathbf {y} '=\mathbf {F} (x,\mathbf
      {y} )]
where
          y  = (  y  1   , &#x2026; ,  y  n   ) ,   F  ( x ,  y  1   , &#x2026;
      ,  y  n   ) = (  y  2   , &#x2026; ,  y  n   , F ( x ,  y  1   , &#x2026;
      ,  y  n   ) ) .   {\displaystyle \mathbf {y} =(y_{1},\ldots ,y_{n}),\quad
      \mathbf {F} (x,y_{1},\ldots ,y_{n})=(y_{2},\ldots ,y_{n},F(x,y_{1},\ldots
      ,y_{n})).}  [{\displaystyle \mathbf {y} =(y_{1},\ldots ,y_{n}),\quad
      \mathbf {F} (x,y_{1},\ldots ,y_{n})=(y_{2},\ldots ,y_{n},F(x,y_{1},\ldots
      ,y_{n})).}]
***** Summary of exact solutions[edit] *****
Some differential equations have solutions that can be written in an exact and
closed form. Several important classes are given here.
In the table below, P(x), Q(x), P(y), Q(y), and M(x,y), N(x,y) are any
integrable functions of x, y, and b and c are real given constants, and C1,
C2,... are arbitrary constants (complex in general). The differential equations
are in their equivalent and alternative forms that lead to the solution through
integration.
In the integral solutions, Î» and Îµ are dummy variables of integration (the
continuum analogues of indices in summation), and the notation â«xF(Î») dÎ»
just means to integrate F(Î») with respect to Î», then after the integration
substitute Î» = x, without adding constants (explicitly stated).
      Type      Differential      Solution method                                                       General solution
                equation
                First-order,
                separable in x
                and y (general
                case, see below
                for special
                cases)[25]
                        P  1
                ( x )  Q  1   ( y
                ) +  P  2   ( x )
                Q  2   ( y )
                d y   d x       =
                0      P  1   ( x
                )  Q  1   ( y )
                d x +  P  2   ( x
                )  Q  2   ( y )
                d y    = 0
                {\displaystyle                                                                              &#x222B;  x       P  1   ( &#x03BB; )    P  2   ( &#x03BB; )     d
                {\begin                                                                                 &#x03BB; +  &#x222B;  y       Q  2   ( &#x03BB; )    Q  1   ( &#x03BB; )
                {aligned}P_{1}                                                                          d &#x03BB; = C     {\displaystyle \int ^{x}{\frac {P_{1}(\lambda )}{P_{2}
                (x)Q_{1}(y)+P_{2} Separation of variables (divide by P2Q1).                             (\lambda )}}\,d\lambda +\int ^{y}{\frac {Q_{2}(\lambda )}{Q_{1}(\lambda
                (x)Q_{2}(y)\,                                                                           )}}\,d\lambda =C\,\!}  [\int ^{x}{\frac {P_{1}(\lambda )}{P_{2}(\lambda
                {\frac {dy}                                                                             )}}\,d\lambda +\int ^{y}{\frac {Q_{2}(\lambda )}{Q_{1}(\lambda )}}\,d\lambda
                {dx}}&=0\\P_{1}                                                                         =C\,\!]
                (x)Q_{1}
                (y)\,dx+P_{2}
                (x)Q_{2}
                (y)\,dy&=0\end
                {aligned}}}  [
                {\displaystyle
                {\begin
                {aligned}P_{1}
                (x)Q_{1}(y)+P_{2}
                (x)Q_{2}(y)\,
                {\frac {dy}
                {dx}}&=0\\P_{1}
                (x)Q_{1}
                (y)\,dx+P_{2}
                (x)Q_{2}
                (y)\,dy&=0\end
                {aligned}}}]
                First-order,
                separable in x
                [23]
                          d y   d
                x       = F ( x )
                d y    = F ( x )
                d x
                {\displaystyle
                {\begin{aligned}
                {\frac {dy}                                                                                y =  &#x222B;  x   F ( &#x03BB; )  d &#x03BB; + C     {\displaystyle
                {dx}}&=F          Direct integration.                                                   y=\int ^{x}F(\lambda )\,d\lambda +C\,\!}  [y=\int ^{x}F(\lambda )\,d\lambda
                (x)\\dy&=F                                                                              +C\,\!]
      Separable (x)\,dx\end
                {aligned}}}  [
                {\displaystyle
                {\begin{aligned}
                {\frac {dy}
                {dx}}&=F
                (x)\\dy&=F
                (x)\,dx\end
                {aligned}}}]
                First-order,
                autonomous,
                separable in y
                [23]
                          d y   d
                x       = F ( y )
                d y    = F ( y )
                d x
                {\displaystyle
                {\begin{aligned}                                                                           x =  &#x222B;  y      d &#x03BB;   F ( &#x03BB; )    + C
                {\frac {dy}       Separation_of_variables (divide by F).                                {\displaystyle x=\int ^{y}{\frac {d\lambda }{F(\lambda )}}+C\,\!}  [x=\int ^
                {dx}}&=F                                                                                {y}{\frac {d\lambda }{F(\lambda )}}+C\,\!]
                (y)\\dy&=F
                (y)\,dx\end
                {aligned}}}  [
                {\displaystyle
                {\begin{aligned}
                {\frac {dy}
                {dx}}&=F
                (y)\\dy&=F
                (y)\,dx\end
                {aligned}}}]
                First-order,
                separable in x
                and y[23]
                       P ( y )
                d y   d x    + Q
                ( x )    = 0
                P ( y )  d y + Q
                ( x )  d x    = 0
                {\displaystyle
                {\begin{aligned}P                                                                           &#x222B;  y   P ( &#x03BB; )  d &#x03BB; +  &#x222B;  x   Q ( &#x03BB; )
                (y){\frac {dy}    Integrate throughout.                                                 d &#x03BB; = C     {\displaystyle \int ^{y}P(\lambda )\,d\lambda +\int ^{x}Q
                {dx}}+Q(x)&=0\\P                                                                        (\lambda )\,d\lambda =C\,\!}  [{\displaystyle \int ^{y}P(\lambda )\,d\lambda
                (y)\,dy+Q                                                                               +\int ^{x}Q(\lambda )\,d\lambda =C\,\!}]
                (x)\,dx&=0\end
                {aligned}}}  [
                {\displaystyle
                {\begin{aligned}P
                (y){\frac {dy}
                {dx}}+Q(x)&=0\\P
                (y)\,dy+Q
                (x)\,dx&=0\end
                {aligned}}}]
                First-order,
                homogeneous[23]
                      d y   d x
                = F  (   y x   )
                {\displaystyle
                {\frac {dy}                                                                                ln &#x2061; ( C x ) =  &#x222B;  y  /  x      d &#x03BB;   F ( &#x03BB; )
                {dx}}=F\left(     Set y = ux, then solve by separation of variables in u and x.         &#x2212; &#x03BB;        {\displaystyle \ln(Cx)=\int ^{y/x}{\frac {d\lambda }
                {\frac {y}                                                                              {F(\lambda )-\lambda }}\,\!}  [\ln(Cx)=\int ^{y/x}{\frac {d\lambda }{F
                {x}}\right)\,\!}                                                                        (\lambda )-\lambda }}\,\!]
                [{\displaystyle
                {\frac {dy}
                {dx}}=F\left(
                {\frac {y}
                {x}}\right)\,\!}]
                First-order,
                separable[25]
                       y M ( x y
                ) + x N ( x y )
                d y   d x       =
                0     y M ( x y )
                d x + x N ( x y )
                d y    = 0
                {\displaystyle
                {\begin
                {aligned}yM                                                                                ln &#x2061; ( C x ) =  &#x222B;  x y      N ( &#x03BB; )  d &#x03BB;
                (xy)+xN(xy)\,                                                                           &#x03BB; [ N ( &#x03BB; ) &#x2212; M ( &#x03BB; ) ]        {\displaystyle \ln
                {\frac {dy}       Separation of variables (divide by xy).                               (Cx)=\int ^{xy}{\frac {N(\lambda )\,d\lambda }{\lambda [N(\lambda )-M(\lambda
                {dx}}&=0\\yM                                                                            )]}}\,\!}  [\ln(Cx)=\int ^{xy}{\frac {N(\lambda )\,d\lambda }{\lambda [N
                (xy)\,dx+xN                                                                             (\lambda )-M(\lambda )]}}\,\!]
                (xy)\,dy&=0\end                                                                         If N = M, the solution is xy = C.
                {aligned}}}  [
                {\displaystyle
                {\begin
                {aligned}yM
                (xy)+xN(xy)\,
                {\frac {dy}
                {dx}}&=0\\yM
                (xy)\,dx+xN
                (xy)\,dy&=0\end
                {aligned}}}]
                Exact
                differential,
                first-order[23]
                       M ( x , y
                )    d y   d x
                + N ( x , y )
                = 0     M ( x , y
                )  d y + N ( x ,
                y )  d x    = 0
                {\displaystyle
                {\begin{aligned}M
                (x,y){\frac {dy}
                {dx}}+N
                (x,y)&=0\\M
                (x,y)\,dy+N
                (x,y)\,dx&=0\end
                {aligned}}}  [                                                                                 F ( x , y ) =     &#x222B;  y   M ( x , &#x03BB; )  d &#x03BB; +
                {\displaystyle                                                                          &#x222B;  x   N ( &#x03BB; , y )  d &#x03BB;       + Y ( y ) + X ( x ) = C
                {\begin{aligned}M                                                                       {\displaystyle {\begin{aligned}F(x,y)=&\int ^{y}M(x,\lambda )\,d\lambda +\int
                (x,y){\frac {dy}                                                                        ^{x}N(\lambda ,y)\,d\lambda \\&+Y(y)+X(x)=C\end{aligned}}}  [{\displaystyle
      General   {dx}}+N           Integrate throughout.                                                 {\begin{aligned}F(x,y)=&\int ^{y}M(x,\lambda )\,d\lambda +\int ^{x}N(\lambda
      first-    (x,y)&=0\\M                                                                             ,y)\,d\lambda \\&+Y(y)+X(x)=C\end{aligned}}}]
      order     (x,y)\,dy+N                                                                             where Y(y) and X(x) are functions from the integrals rather than constant
                (x,y)\,dx&=0\end                                                                        values, which are set to make the final function F(x, y) satisfy the initial
                {aligned}}}]                                                                            equation.
                where
                &#x2202; M
                &#x2202; x    =
                &#x2202; N
                &#x2202; y
                {\displaystyle
                {\frac {\partial
                M}{\partial x}}=
                {\frac {\partial
                N}{\partial
                y}}\,\!}  [{\frac
                {\partial M}
                {\partial x}}=
                {\frac {\partial
                N}{\partial
                y}}\,\!]
                Inexact
                differential,
                first-order[23]
                       M ( x , y
                )    d y   d x
                + N ( x , y )
                = 0     M ( x , y
                )  d y + N ( x ,
                y )  d x    = 0
                {\displaystyle
                {\begin{aligned}M
                (x,y){\frac {dy}
                {dx}}+N
                (x,y)&=0\\M
                (x,y)\,dy+N
                (x,y)\,dx&=0\end
                {aligned}}}  [
                {\displaystyle                                                                          If Î¼(x, y) can be found:
                {\begin{aligned}M Integration_factor Î¼(x, y) satisfying                                     F ( x , y ) =     &#x222B;  y   &#x03BC; ( x , &#x03BB; ) M ( x ,
                (x,y){\frac {dy}        &#x2202; ( &#x03BC; M )   &#x2202; x    =    &#x2202;           &#x03BB; )  d &#x03BB; +  &#x222B;  x   &#x03BC; ( &#x03BB; , y ) N
                {dx}}+N           ( &#x03BC; N )   &#x2202; y        {\displaystyle {\frac {\partial    ( &#x03BB; , y )  d &#x03BB;       + Y ( y ) + X ( x ) = C
                (x,y)&=0\\M       (\mu M)}{\partial x}}={\frac {\partial (\mu N)}{\partial y}}\,\!}  [  {\displaystyle {\begin{aligned}F(x,y)=&\int ^{y}\mu (x,\lambda )M(x,\lambda
                (x,y)\,dy+N       {\frac {\partial (\mu M)}{\partial x}}={\frac {\partial (\mu N)}      )\,d\lambda +\int ^{x}\mu (\lambda ,y)N(\lambda ,y)\,d\lambda \\&+Y(y)+X
                (x,y)\,dx&=0\end  {\partial y}}\,\!]                                                    (x)=C\end{aligned}}}  [{\displaystyle {\begin{aligned}F(x,y)=&\int ^{y}\mu
                {aligned}}}]                                                                            (x,\lambda )M(x,\lambda )\,d\lambda +\int ^{x}\mu (\lambda ,y)N(\lambda
                where                                                                                   ,y)\,d\lambda \\&+Y(y)+X(x)=C\end{aligned}}}]
                &#x2202; M
                &#x2202; x
                &#x2260;
                &#x2202; N
                &#x2202; y
                {\displaystyle
                {\frac {\partial
                M}{\partial
                x}}\neq {\frac
                {\partial N}
                {\partial
                y}}\,\!}  [{\frac
                {\partial M}
                {\partial x}}\neq
                {\frac {\partial
                N}{\partial
                y}}\,\!]
                Second-order,
                autonomous[26]
                       d  2   y   Multiply both sides of equation by 2dy/dx, substitute     2    d y
                d  x  2      = F  d x        d  2   y   d  x  2      =   d  d x      (    d y   d x        x = &#x00B1;  &#x222B;  y      d &#x03BB;   2  &#x222B;  &#x03BB;   F
      General   ( y )             )   2       {\displaystyle 2{\frac {dy}{dx}}{\frac {d^{2}y}{dx^{2}}}= ( &#x03B5; )  d &#x03B5; +  C  1      +  C  2       {\displaystyle x=\pm \int
      second-   {\displaystyle    {\frac {d}{dx}}\left({\frac {dy}{dx}}\right)^{2}\,\!}  [2{\frac {dy}  ^{y}{\frac {d\lambda }{\sqrt {2\int ^{\lambda }F(\varepsilon )\,d\varepsilon
      order     {\frac {d^{2}y}   {dx}}{\frac {d^{2}y}{dx^{2}}}={\frac {d}{dx}}\left({\frac {dy}        +C_{1}}}}+C_{2}\,\!}  [{\displaystyle x=\pm \int ^{y}{\frac {d\lambda }{\sqrt
                {dx^{2}}}=F       {dx}}\right)^{2}\,\!], then integrate twice.                          {2\int ^{\lambda }F(\varepsilon )\,d\varepsilon +C_{1}}}}+C_{2}\,\!}]
                (y)\,\!}  [{\frac
                {d^{2}y}{dx^
                {2}}}=F(y)\,\!]
                First-order,
                linear,
                inhomogeneous,
                function
                coefficients[23]                                                                           y =  e  &#x2212;  &#x222B;  x   P ( &#x03BB; )  d &#x03BB;    [   &#x222B;
                      d y   d x                                                                         x    e   &#x222B;  &#x03BB;   P ( &#x03B5; )  d &#x03B5;   Q ( &#x03BB; )  d
                + P ( x ) y = Q   Integrating factor:      e   &#x222B;  x   P ( &#x03BB; )  d &#x03BB; &#x03BB; + C  ]    {\displaystyle y=e^{-\int ^{x}P(\lambda )\,d\lambda }\left
                ( x )             .   {\displaystyle e^{\int ^{x}P(\lambda )\,d\lambda }.}  [           [\int ^{x}e^{\int ^{\lambda }P(\varepsilon )\,d\varepsilon }Q(\lambda
                {\displaystyle    {\displaystyle e^{\int ^{x}P(\lambda )\,d\lambda }.}]                 )\,d\lambda +C\right]}  [{\displaystyle y=e^{-\int ^{x}P(\lambda )\,d\lambda
                {\frac {dy}                                                                             }\left[\int ^{x}e^{\int ^{\lambda }P(\varepsilon )\,d\varepsilon }Q(\lambda
                {dx}}+P(x)y=Q                                                                           )\,d\lambda +C\right]}]
                (x)\,\!}  [
                {\displaystyle
                {\frac {dy}
                {dx}}+P(x)y=Q
                (x)\,\!}]
                                                                                                           y =  y  c   +  y  p     {\displaystyle y=y_{c}+y_{p}}  [{\displaystyle
                                                                                                        y=y_{c}+y_{p}}]
                Second-order,                                                                           If b2 > 4c, then
                linear,                                                                                           y  c   =  C  1    e  &#x2212;   x 2     (  b +    b  2   &#x2212; 4
                inhomogeneous,                                                                                c    )    +  C  2    e  &#x2212;   x 2     (  b &#x2212;    b  2
                constant                                                                                      &#x2212; 4 c    )      {\displaystyle y_{c}=C_{1}e^{-{\frac {x}
                coefficients[27]                                                                              {2}}\,\left(b+{\sqrt {b^{2}-4c}}\right)}+C_{2}e^{-{\frac {x}{2}}\,\left
                       d  2   y                                                                               (b-{\sqrt {b^{2}-4c}}\right)}}  [{\displaystyle y_{c}=C_{1}e^{-{\frac
                d  x  2      + b  Complementary function yc: assume yc = eÎ±x, substitute and solve         {x}{2}}\,\left(b+{\sqrt {b^{2}-4c}}\right)}+C_{2}e^{-{\frac {x}
                d y   d x    + c  polynomial in Î±, to find the linearly_independent functions      e       {2}}\,\left(b-{\sqrt {b^{2}-4c}}\right)}}]
                y = r ( x )       &#x03B1;  j   x     {\displaystyle e^{\alpha _{j}x}}  [e^{\alpha _    If b2 = 4c, then
                {\displaystyle    {j}x}].                                                                         y  c   = (  C  1   x +  C  2   )  e  &#x2212;    b x  2
                {\frac {d^{2}y}   Particular integral yp: in general the method_of_variation_of               {\displaystyle y_{c}=(C_{1}x+C_{2})e^{-{\frac {bx}{2}}}}  [
                {dx^{2}}}+b{\frac parameters, though for very simple r(x) inspection may work.[23]            {\displaystyle y_{c}=(C_{1}x+C_{2})e^{-{\frac {bx}{2}}}}]
                {dy}{dx}}+cy=r                                                                          If b2 < 4c, then
      Linear to (x)\,\!}  [{\frac                                                                                 y  c   =  e  &#x2212;    b x  2      [   C  1   sin &#x2061;  (  x
      nth order {d^{2}y}{dx^                                                                                  4 c &#x2212;  b  2    2    )  +  C  2   cos &#x2061;  (  x     4 c
                {2}}}+b{\frac                                                                                 &#x2212;  b  2    2    )   ]    {\displaystyle y_{c}=e^{-{\frac {bx}
                {dy}{dx}}+cy=r                                                                                {2}}}\left[C_{1}\sin \left(x\,{\frac {\sqrt {4c-b^{2}}}{2}}\right)+C_
                (x)\,\!]                                                                                      {2}\cos \left(x\,{\frac {\sqrt {4c-b^{2}}}{2}}\right)\right]}  [
                                                                                                              {\displaystyle y_{c}=e^{-{\frac {bx}{2}}}\left[C_{1}\sin \left(x\,
                                                                                                              {\frac {\sqrt {4c-b^{2}}}{2}}\right)+C_{2}\cos \left(x\,{\frac {\sqrt
                                                                                                              {4c-b^{2}}}{2}}\right)\right]}]
                                                                                                           y =  y  c   +  y  p     {\displaystyle y=y_{c}+y_{p}}  [{\displaystyle
                                                                                                        y=y_{c}+y_{p}}]
                                                                                                        Since Î±j are the solutions of the polynomial of degree n:      &#x220F;  j =
                nth-order,                                                                              1   n   ( &#x03B1; &#x2212;  &#x03B1;  j   ) = 0     {\displaystyle \prod _
                linear,                                                                                 {j=1}^{n}(\alpha -\alpha _{j})=0\,\!}  [{\displaystyle \prod _{j=1}^{n}
                inhomogeneous,                                                                          (\alpha -\alpha _{j})=0\,\!}], then:
                constant                                                                                for Î±j all different,
                coefficients[27]                                                                                  y  c   =  &#x2211;  j = 1   n    C  j    e   &#x03B1;  j   x
                    &#x2211;  j =                                                                             {\displaystyle y_{c}=\sum _{j=1}^{n}C_{j}e^{\alpha _{j}x}\,\!}  [y_
                0   n    b  j     Complementary function yc: assume yc = eÎ±x, substitute and solve         {c}=\sum _{j=1}^{n}C_{j}e^{\alpha _{j}x}\,\!]
                d  j   y   d  x   polynomial in Î±, to find the linearly_independent functions      e for each root Î±j repeated kj times,
                j      = r ( x )  &#x03B1;  j   x     {\displaystyle e^{\alpha _{j}x}}  [e^{\alpha _              y  c   =  &#x2211;  j = 1   n    (   &#x2211;  &#x2113; = 1    k  j
                {\displaystyle    {j}x}].                                                                     C  j , &#x2113;    x  &#x2113; &#x2212; 1    )   e   &#x03B1;  j   x
                \sum _{j=0}^{n}b_ Particular integral yp: in general the method_of_variation_of               {\displaystyle y_{c}=\sum _{j=1}^{n}\left(\sum _{\ell =1}^{k_{j}}C_
                {j}{\frac {d^     parameters, though for very simple r(x) inspection may work.[23]            {j,\ell }x^{\ell -1}\right)e^{\alpha _{j}x}\,\!}  [{\displaystyle y_
                {j}y}{dx^{j}}}=r                                                                              {c}=\sum _{j=1}^{n}\left(\sum _{\ell =1}^{k_{j}}C_{j,\ell }x^{\ell -
                (x)\,\!}  [\sum _                                                                             1}\right)e^{\alpha _{j}x}\,\!}]
                {j=0}^{n}b_{j}                                                                          for some Î±j complex, then setting Î± = Ïj + iÎ³j, and using Euler's
                {\frac {d^{j}y}                                                                         formula, allows some terms in the previous results to be written in the form
                {dx^{j}}}=r                                                                                       C  j    e   &#x03B1;  j   x   =  C  j    e   &#x03C7;  j   x   cos
                (x)\,\!]                                                                                      &#x2061; (  &#x03B3;  j   x +  &#x03C6;  j   )     {\displaystyle C_
                                                                                                              {j}e^{\alpha _{j}x}=C_{j}e^{\chi _{j}x}\cos(\gamma _{j}x+\varphi _
                                                                                                              {j})\,\!}  [{\displaystyle C_{j}e^{\alpha _{j}x}=C_{j}e^{\chi _
                                                                                                              {j}x}\cos(\gamma _{j}x+\varphi _{j})\,\!}]
                                                                                                        where Ïj is an arbitrary constant (phase shift).
***** Software for ODE solving[edit] *****
    * Maxima, an open-source computer_algebra_system.
    * COPASI, a free (Artistic_License_2.0) software package for the
      integration and analysis of ODEs.
    * MATLAB, a technical computing application (MATrix LABoratory)
    * GNU_Octave, a high-level language, primarily intended for numerical
      computations.
    * Scilab, an open source application for numerical computation.
    * Maple, a proprietary application for symbolic calculations.
    * Mathematica, a proprietary application primarily intended for symbolic
      calculations.
    * Julia_(programming_language), a high-level, multi-paradigm, open-source,
      dynamic programming language primarily intended for numerical
      computations, although it is flexible enough for general-purpose
      programming.
    * SageMath, an open-source application that uses a Python-like syntax with
      a wide range of capabilities spanning several branches of mathematics.
    * SciPy, a Python package that includes an ODE integration module.
    * Chebfun, an open-source package, written in MATLAB, for computing with
      functions to 15-digit accuracy.
    * GNU_R, an open source computational environment primarily intended for
      statistics, which includes package for ODE solving.
    * EROS.NET a free ODE solver for .NET.
***** See also[edit] *****
    * Examples_of_differential_equations
    * Boundary_value_problem
    * Laplace_transform_applied_to_differential_equations
    * List_of_dynamical_systems_and_differential_equations_topics
    * Matrix_differential_equation
    * Method_of_undetermined_coefficients
    * Numerical_methods_for_ordinary_differential_equations
    * Recurrence_relation
    * Separation_of_variables
***** Notes[edit] *****
   1. ^Dennis G. Zill (15 March 2012). A_First_Course_in_Differential_Equations
      with_Modeling_Applications. Cengage Learning. ISBN 1-285-40110-7.
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
   3. ^"What_is_the_origin_of_the_term_"ordinary_differential_equations"?".
      hsm.stackexchange.com. Stack_Exchange. Retrieved 2016-07-28.
   4. ^ Mathematics for Chemists, D.M. Hirst, Macmillan_Press, 1976, (No ISBN)
      SBN: 333-18172-7
   5. ^ Kreyszig_(1972, p. 64)
   6. ^ Simmons_(1972, pp. 1,2)
   7. ^ Halliday_&_Resnick_(1977, p. 78)
   8. ^ Tipler_(1991, pp. 78â83)
   9. ^ a b Harper_(1976, p. 127)
  10. ^ Kreyszig_(1972, p. 2)
  11. ^ Simmons_(1972, p. 3)
  12. ^ a b Kreyszig_(1972, p. 24)
  13. ^ Simmons_(1972, p. 47)
  14. ^ Harper_(1976, p. 128)
  15. ^Uri M. Ascher; Linda R. Petzold (1998). Computer Methods for Ordinary
      Differential Equations and Differential-Algebraic Equations. SIAM. p. 12.
      ISBN 978-1-61197-139-2.
  16. ^Achim Ilchmann; Timo Reis (2014). Surveys in Differential-Algebraic
      Equations II. Springer. pp. 104â105. ISBN 978-3-319-11050-9.
  17. ^Uri M. Ascher; Linda R. Petzold (1998). Computer Methods for Ordinary
      Differential Equations and Differential-Algebraic Equations. SIAM. p. 5.
      ISBN 978-1-61197-139-2.
  18. ^ Kreyszig_(1972, p. 78)
  19. ^ Kreyszig_(1972, p. 4)
  20. ^ Crelle, 1866, 1868
  21. ^ Lawrence_(1999, p. 9)
  22. ^ Logan, J. (2013). Applied mathematics (Fourth ed.).
  23. ^Uri M. Ascher; Linda R. Petzold (1998). Computer Methods for Ordinary
      Differential Equations and Differential-Algebraic Equations. SIAM. p. 13.
      ISBN 978-1-61197-139-2.
  24. ^ a b c d e f g h i j Elementary Differential Equations and Boundary
      Value Problems (4th Edition), W.E. Boyce, R.C. Diprima, Wiley
      International, John Wiley & Sons, 1986,
  25. ISBN 0-471-83824-1
  26. ^ Boscain; Chitour 2011, p. 21
  27. ^ a b Mathematical Handbook of Formulas and Tables (3rd edition), S.
      Lipschutz, M. R. Spiegel, J. Liu, Schuam's Outline Series, 2009, ISC_2N
      978-0-07-154855-7
  28. ^ Further Elementary Analysis, R. Porter, G.Bell & Sons (London), 1978,
  29. ISBN 0-7135-1594-5
  30. ^ a b Mathematical methods for physics and engineering, K.F. Riley, M.P.
      Hobson, S.J. Bence, Cambridge University Press, 2010, ISC_2N 978-0-521-
      86153-3
***** References[edit] *****
    * Halliday, David; Resnick, Robert (1977), Physics (3rd ed.), New York:
      Wiley, ISBN 0-471-71716-9
Harper, Charlie (1976), Introduction to Mathematical Physics, New Jersey:
Prentice-Hall, ISBN 0-13-487538-9
Kreyszig,_Erwin (1972), Advanced Engineering Mathematics (3rd ed.), New York:
Wiley, ISBN 0-471-50728-8
.
Polyanin, A. D. and V. F. Zaitsev, Handbook of Exact Solutions for Ordinary
Differential Equations (2nd edition)", Chapman & Hall/CRC Press, Boca Raton,
2003.
ISBN 1-58488-297-2
Simmons,_George_F. (1972), Differential Equations with Applications and
Historical Notes, New York: McGraw-Hill, LCCN 75173716
Tipler, Paul A. (1991), Physics for Scientists and Engineers: Extended version
(3rd ed.), New York: Worth_Publishers, ISBN 0-87901-432-6
Boscain, Ugo; Chitour, Yacine (2011), Introduction_Ã _l'automatique (PDF) (in
French)
Dresner, Lawrence (1999), Applications of Lie's Theory of Ordinary and Partial
Differential Equations, Bristol and Philadelphia: Institute_of_Physics
Publishing, ISBN 978-0750305303
***** Bibliography[edit] *****
    * Coddington, Earl A.; Levinson, Norman (1955). Theory of Ordinary
      Differential Equations. New York: McGraw-Hill.
Hartman,_Philip (2002) [1964], Ordinary_differential_equations, Classics in
Applied Mathematics, 38, Philadelphia: Society_for_Industrial_and_Applied
Mathematics, doi:10.1137/1.9780898719222, ISBN 978-0-89871-510-1, MR 1929104
W. Johnson, A_Treatise_on_Ordinary_and_Partial_Differential_Equations, John
Wiley and Sons, 1913, in University_of_Michigan_Historical_Math_Collection
Ince,_Edward_L. (1944) [1926], Ordinary_Differential_Equations, Dover
Publications, New York, ISBN 978-0-486-60349-0, MR 0010757
Witold_Hurewicz, Lectures on Ordinary Differential Equations, Dover
Publications,
ISBN 0-486-49510-8
Ibragimov, Nail H (1993). CRC Handbook of Lie Group Analysis of Differential
Equations Vol. 1-3. Providence: CRC-Press. ISBN 0-8493-4488-3
.
Teschl,_Gerald (2012). Ordinary_Differential_Equations_and_Dynamical_Systems.
Providence: American_Mathematical_Society. ISBN 978-0-8218-8328-0.
A._D._Polyanin, V. F. Zaitsev, and A. Moussiaux, Handbook of First Order
Partial Differential Equations, Taylor & Francis, London, 2002.
ISBN 0-415-27267-X
D. Zwillinger, Handbook of Differential Equations (3rd edition), Academic
Press, Boston, 1997.
***** External links[edit] *****
 Wikibooks has a book on the topic of: Calculus/Ordinary_differential_equations
 Wikimedia Commons has media related to Ordinary_differential_equations.
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Differential_equation,
      ordinary", Encyclopedia_of_Mathematics, Springer Science+Business Media
      B.V. / Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Differential_Equations at Curlie (includes a list of software for solving
differential equations).
EqWorld:_The_World_of_Mathematical_Equations, containing a list of ordinary
differential equations with their solutions.
Online_Notes_/_Differential_Equations by Paul Dawkins, Lamar_University.
Differential_Equations, S.O.S. Mathematics.
A_primer_on_analytical_solution_of_differential_equations from the Holistic
Numerical Methods Institute, University of South Florida.
Ordinary_Differential_Equations_and_Dynamical_Systems lecture notes by Gerald
Teschl.
Notes_on_Diffy_Qs:_Differential_Equations_for_Engineers An introductory
textbook on differential equations by Jiri Lebl of UIUC.
Modeling_with_ODEs_using_Scilab A tutorial on how to model a physical system
described by ODE using Scilab standard programming language by Openeering team.
Solving_an_ordinary_differential_equation_in_Wolfram|Alpha
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
Authority_control [Edit_this_at_Wikidata]     * NDL: 00574993

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Ordinary_differential_equation&oldid=906735137"
Categories:
    * Differential_calculus
    * Ordinary_differential_equations
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_December_2014
    * CS1_French-language_sources_(fr)
    * Articles_with_inconsistent_citation_formats
    * Commons_category_link_is_on_Wikidata
    * Articles_with_Curlie_links
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
    * Wikiversity
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * ÐÐ°ÑÒ¡Ð¾ÑÑÑÐ°
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
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
    * Bahasa_Melayu
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * à·à·à¶à·à¶½
    * Simple_English
    * SlovenÄina
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 17 July 2019, at 21:28 (UTC).
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
