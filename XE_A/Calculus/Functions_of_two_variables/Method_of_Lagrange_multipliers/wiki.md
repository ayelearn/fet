The following text has been accessed from https://en.wikipedia.org/wiki/Lagrange_multiplier at Fri Aug 9 00:02:43 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Lagrange multiplier ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematical_optimization, the method of Lagrange multipliers is a strategy
for finding the local maxima_and_minima of a function subject to equality
constraints (i.e., subject to the condition that one or more equations have to
be satisfied exactly by the chosen values of the variables).[1] The basic idea
is to convert a constrained problem into a form such that the derivative_test
of an unconstrained problem can still be applied. Once stationary_points have
been identified from the first-order necessary conditions, the definiteness of
the bordered_Hessian_matrix determines whether those points are maxima, minima,
or saddle_points.[2]
The Lagrange multiplier theorem roughly states that at any stationary_point of
the function that also satisfies the equality constraints, the gradient of the
function at that point can be expressed as a linear_combination of the
gradients of the constraints at that point, with the Lagrange multipliers
acting as coefficients.[3] The relationship between the gradient of the
function and gradients of the constraints rather naturally leads to a
reformulation of the original problem, known as the Lagrangian function.[4]
The great advantage of this method is that it allows the optimization to be
solved without explicit parameterization in terms of the constraints. As a
result, the method of Lagrange multipliers is widely used to solve challenging
constrained optimization problems. The method can be summarized as follows: in
order to find the stationary points of a function     f ( x )   {\displaystyle
f(x)}  [f(x)] subject to the equality constraints      g  i   ( x ) = 0
{\displaystyle g_{i}(x)=0}  [{\displaystyle g_{i}(x)=0}],     i = 1 , 2 ,
&#x2026; , m   {\displaystyle i=1,2,\ldots ,m}  [{\displaystyle i=1,2,\ldots
,m}], form the Lagrangian function
           L   ( x , &#x03BB; ) = f ( x ) &#x2212;  &#x2211;  i = 1   m
      &#x03BB;  i    g  i   ( x )   {\displaystyle {\mathcal {L}}(x,\lambda )=f
      (x)-\sum _{i=1}^{m}\lambda _{i}g_{i}(x)}  [{\displaystyle {\mathcal {L}}
      (x,\lambda )=f(x)-\sum _{i=1}^{m}\lambda _{i}g_{i}(x)}]
and find the stationary points of       L     {\displaystyle {\mathcal {L}}}  [
{\mathcal {L}}] considered as a function of     x   {\displaystyle x}  [x] and
the Lagrange multiplier     &#x03BB;   {\displaystyle \lambda }  [\lambda ].[5]
⁰
***** Contents *****
    * 1_Single_constraint
    * 2_Multiple_constraints
    * 3_Modern_formulation_via_differentiable_manifolds
          o 3.1_Single_constraint
          o 3.2_Multiple_constraints
    * 4_Interpretation_of_the_Lagrange_multipliers
    * 5_Sufficient_conditions
    * 6_Examples
          o 6.1_Example_1
                # 6.1.1_Example_1a
                # 6.1.2_Example_1b
          o 6.2_Example_2
          o 6.3_Example_3:_Entropy
          o 6.4_Example_4:_Numerical_optimization
    * 7_Applications
          o 7.1_Control_theory
          o 7.2_Nonlinear_programming
    * 8_See_also
    * 9_References
    * 10_Further_reading
    * 11_External_links
***** Single constraint[edit] *****
Figure 1: The red curve shows the constraint g(x, y) = c. The blue curves are
contours of f(x, y). The point where the red constraint tangentially touches a
blue contour is the maximum of f(x, y) along the constraint, since d1 > d2.
For the case of only one constraint and only two choice variables (as
exemplified in Figure 1), consider the optimization_problem
      maximize f(x, y)
      subject to g(x, y) = 0.
(Sometimes an additive constant is shown separately rather than being included
in g, in which case the constraint is written g(x, y) = c, as in Figure 1.) We
assume that both f and g have continuous first partial_derivatives. We
introduce a new variable (Î») called a Lagrange multiplier (or Lagrange
undetermined multiplier) and study the Lagrange function (or Lagrangian or
Lagrangian expression) defined by
           L   ( x , y , &#x03BB; ) = f ( x , y ) &#x2212; &#x03BB; g ( x , y )
      ,   {\displaystyle {\mathcal {L}}(x,y,\lambda )=f(x,y)-\lambda g(x,y),}
      [{\displaystyle {\mathcal {L}}(x,y,\lambda )=f(x,y)-\lambda g(x,y),}]
where the Î» term may be either added or subtracted. If f(x0, y0) is a maximum
of f(x, y) for the original constrained problem, then there exists Î»0 such
that (x0, y0, Î»0) is a stationary_point for the Lagrange function (stationary
points are those points where the first partial derivatives of       L
{\displaystyle {\mathcal {L}}}  [{\mathcal {L}}] are zero). Also, it must be
assumed that     &#x2207; g &#x2260; 0.   {\displaystyle \nabla g\neq 0.}  [
{\displaystyle \nabla g\neq 0.}] However, not all stationary points yield a
solution of the original problem, as the method of Lagrange multipliers yields
only a necessary_condition for optimality in constrained problems.[6][7][8][9]
[10] Sufficient conditions for a minimum or maximum also_exist, but if a
particular candidate_solution satisfies the sufficient conditions, it is only
guaranteed that that solution is the best one locally â that is, it is better
than any permissible nearby points. The global optimum can be found by
comparing the values of the original objective function at the points
satisfying the necessary and locally sufficient conditions.
The method of Lagrange multipliers relies on the intuition that at a maximum, f
(x, y) cannot be increasing in the direction of any such neighboring point that
also has g = 0. If it were, we could walk along g = 0 to get higher, meaning
that the starting point wasn't actually the maximum.
We can visualize contours of f given by f(x, y) = d for various values of d,
and the contour of g given by g(x, y) = c.
Suppose we walk along the contour line with g = c. We are interested in finding
points where f does not change as we walk, since these points might be maxima.
There are two ways this could happen:
   1. We could be following a contour line of f, since by definition f does not
      change as we walk along its contour lines. This would mean that the
      contour lines of f and g are parallel here.
   2. We have reached a "level" part of f, meaning that f does not change in
      any direction.
To check the first possibility (we are following a contour line of f), notice
that since the gradient of a function is perpendicular to the contour lines,
the contour lines of f and g are parallel if and only if the gradients of f and
g are parallel. Thus we want points (x, y) where g(x, y) = 0 and
          &#x2207;  x , y   f = &#x03BB;   &#x2207;  x , y   g ,
      {\displaystyle \nabla _{x,y}f=\lambda \,\nabla _{x,y}g,}  [{\displaystyle
      \nabla _{x,y}f=\lambda \,\nabla _{x,y}g,}]
for some Î»
where
          &#x2207;  x , y   f =  (     &#x2202; f   &#x2202; x    ,    &#x2202;
      f   &#x2202; y     )  ,   &#x2207;  x , y   g =  (     &#x2202; g
      &#x2202; x    ,    &#x2202; g   &#x2202; y     )  .   {\displaystyle
      \nabla _{x,y}f=\left({\frac {\partial f}{\partial x}},{\frac {\partial f}
      {\partial y}}\right),\qquad \nabla _{x,y}g=\left({\frac {\partial g}
      {\partial x}},{\frac {\partial g}{\partial y}}\right).}  [\nabla _
      {x,y}f=\left({\frac {\partial f}{\partial x}},{\frac {\partial f}
      {\partial y}}\right),\qquad \nabla _{x,y}g=\left({\frac {\partial g}
      {\partial x}},{\frac {\partial g}{\partial y}}\right).]
are the respective gradients. The constant Î» is required because although the
two gradient vectors are parallel, the magnitudes of the gradient vectors are
generally not equal. This constant is called the Lagrange multiplier. (In some
conventions Î» is preceded by a minus sign).
Notice that this method also solves the second possibility, that f is level: if
f is level, then its gradient is zero, and setting Î» = 0 is a solution
regardless of      &#x2207;  x , y   g   {\displaystyle \nabla _{x,y}g}  [
{\displaystyle \nabla _{x,y}g}].
To incorporate these conditions into one equation, we introduce an auxiliary
function
           L   ( x , y , &#x03BB; ) = f ( x , y ) &#x2212; &#x03BB; g ( x , y )
      ,   {\displaystyle {\mathcal {L}}(x,y,\lambda )=f(x,y)-\lambda g(x,y),}
      [{\displaystyle {\mathcal {L}}(x,y,\lambda )=f(x,y)-\lambda g(x,y),}]
and solve
          &#x2207;  x , y , &#x03BB;     L   ( x , y , &#x03BB; ) = 0.
      {\displaystyle \nabla _{x,y,\lambda }{\mathcal {L}}(x,y,\lambda )=0.}
      [\nabla _{x,y,\lambda }{\mathcal {L}}(x,y,\lambda )=0.]
Note that this amounts to solving three equations in three unknowns. This is
the method of Lagrange multipliers. Note that      &#x2207;  &#x03BB;     L
( x , y , &#x03BB; ) = 0   {\displaystyle \nabla _{\lambda }{\mathcal {L}}
(x,y,\lambda )=0}  [\nabla _{\lambda }{\mathcal {L}}(x,y,\lambda )=0] implies g
(x, y) = 0. To summarize
          &#x2207;  x , y , &#x03BB;     L   ( x , y , &#x03BB; ) = 0  &#x27FA;
      {     &#x2207;  x , y   f ( x , y ) = &#x03BB;   &#x2207;  x , y   g ( x
      , y )     g ( x , y ) = 0         {\displaystyle \nabla _{x,y,\lambda }
      {\mathcal {L}}(x,y,\lambda )=0\iff {\begin{cases}\nabla _{x,y}f
      (x,y)=\lambda \,\nabla _{x,y}g(x,y)\\g(x,y)=0\end{cases}}}  [
      {\displaystyle \nabla _{x,y,\lambda }{\mathcal {L}}(x,y,\lambda )=0\iff
      {\begin{cases}\nabla _{x,y}f(x,y)=\lambda \,\nabla _{x,y}g(x,y)\\g
      (x,y)=0\end{cases}}}]
The method generalizes readily to functions on     n   {\displaystyle n}  [n]
variables
          &#x2207;   x  1   , &#x2026; ,  x  n   , &#x03BB;     L   (  x  1   ,
      &#x2026; ,  x  n   , &#x03BB; ) = 0   {\displaystyle \nabla _{x_{1},\dots
      ,x_{n},\lambda }{\mathcal {L}}(x_{1},\dots ,x_{n},\lambda )=0}  [
      {\displaystyle \nabla _{x_{1},\dots ,x_{n},\lambda }{\mathcal {L}}(x_
      {1},\dots ,x_{n},\lambda )=0}]
which amounts to solving     n + 1   {\displaystyle n+1}  [n+1] equations in
n + 1   {\displaystyle n+1}  [n+1] unknowns.
The constrained extrema of f are critical_points of the Lagrangian       L
{\displaystyle {\mathcal {L}}}  [{\mathcal {L}}], but they are not necessarily
local extrema of       L     {\displaystyle {\mathcal {L}}}  [{\mathcal {L}}]
(see Example_2 below).
One may reformulate_the_Lagrangian as a Hamiltonian, in which case the
solutions are local minima for the Hamiltonian. This is done in optimal_control
theory, in the form of Pontryagin's_minimum_principle.
The fact that solutions of the Lagrangian are not necessarily extrema also
poses difficulties for numerical optimization. This can be addressed by
computing the magnitude of the gradient, as the zeros of the magnitude are
necessarily local minima, as illustrated in the numerical_optimization_example.
***** Multiple constraints[edit] *****
Figure 2: A paraboloid constrained along two intersecting lines.
Figure 3: Contour map of Figure 2.
The method of Lagrange multipliers can be extended to solve problems with
multiple constraints using a similar argument. Consider a paraboloid subject to
two line constraints that intersect at a single point. As the only feasible
solution, this point is obviously a constrained extremum. However, the level
set of     f   {\displaystyle f}  [f] is clearly not parallel to either
constraint at the intersection point (see Figure 3); instead, it is a linear
combination of the two constraints' gradients. In the case of multiple
constraints, that will be what we seek in general: the method of Lagrange seeks
points not at which the gradient of     f   {\displaystyle f}  [f] is multiple
of any single constraint's gradient necessarily, but in which it is a linear
combination of all the constraints' gradients.
Concretely, suppose we have     M   {\displaystyle M}  [M] constraints and are
walking along the set of points satisfying      g  i   (  x  ) = 0 , i = 1 ,
&#x2026; , M   {\displaystyle g_{i}(\mathbf {x} )=0,i=1,\dots ,M}  [
{\displaystyle g_{i}(\mathbf {x} )=0,i=1,\dots ,M}]. Every point      x
{\displaystyle \mathbf {x} }  [\mathbf {x} ] on the contour of a given
constraint function      g  i     {\displaystyle g_{i}}  [g_{i}] has a space of
allowable directions: the space of vectors perpendicular to     &#x2207;  g  i
(  x  )   {\displaystyle \nabla g_{i}(\mathbf {x} )}  [{\displaystyle \nabla g_
{i}(\mathbf {x} )}]. The set of directions that are allowed by all constraints
is thus the space of directions perpendicular to all of the constraints'
gradients. Denote this space of allowable moves by     A   {\displaystyle A}
[A] and denote the span of the constraints' gradients by     S   {\displaystyle
S}  [S]. Then     A =  S  &#x22A5;     {\displaystyle A=S^{\perp }}  [
{\displaystyle A=S^{\perp }}], the space of vectors perpendicular to every
element of     S   {\displaystyle S}  [S].
We are still interested in finding points where     f   {\displaystyle f}  [f]
does not change as we walk, since these points might be (constrained) extrema.
We therefore seek      x    {\displaystyle \mathbf {x} }  [\mathbf {x} ] such
that any allowable direction of movement away from      x    {\displaystyle
\mathbf {x} }  [\mathbf {x} ] is perpendicular to     &#x2207; f (  x  )
{\displaystyle \nabla f(\mathbf {x} )}  [\nabla f(\mathbf{x})] (otherwise we
could increase     f   {\displaystyle f}  [f] by moving along that allowable
direction). In other words,     &#x2207; f (  x  ) &#x2208;  A  &#x22A5;   = S
{\displaystyle \nabla f(\mathbf {x} )\in A^{\perp }=S}  [{\displaystyle \nabla
f(\mathbf {x} )\in A^{\perp }=S}]. Thus there are scalars Î»1, Î»2, ..., Î»M
such that
         &#x2207; f (  x  ) =  &#x2211;  k = 1   M    &#x03BB;  k    &#x2207;
      g  k   (  x  )   &#x27FA;   &#x2207; f (  x  ) &#x2212;  &#x2211;  k = 1
      M     &#x03BB;  k   &#x2207;  g  k   (  x  )  = 0.   {\displaystyle
      \nabla f(\mathbf {x} )=\sum _{k=1}^{M}\lambda _{k}\,\nabla g_{k}(\mathbf
      {x} )\quad \iff \quad \nabla f(\mathbf {x} )-\sum _{k=1}^{M}{\lambda _
      {k}\nabla g_{k}(\mathbf {x} )}=0.}  [{\displaystyle \nabla f(\mathbf {x}
      )=\sum _{k=1}^{M}\lambda _{k}\,\nabla g_{k}(\mathbf {x} )\quad \iff \quad
      \nabla f(\mathbf {x} )-\sum _{k=1}^{M}{\lambda _{k}\nabla g_{k}(\mathbf
      {x} )}=0.}]
These scalars are the Lagrange multipliers. We now have     M   {\displaystyle
M}  [M] of them, one for every constraint.
As before, we introduce an auxiliary function
           L    (   x  1   , &#x2026; ,  x  n   ,  &#x03BB;  1   , &#x2026; ,
      &#x03BB;  M    )  = f  (   x  1   , &#x2026; ,  x  n    )  &#x2212;
      &#x2211;  k = 1   M     &#x03BB;  k    g  k    (   x  1   , &#x2026; ,  x
      n    )     {\displaystyle {\mathcal {L}}\left(x_{1},\ldots ,x_{n},\lambda
      _{1},\ldots ,\lambda _{M}\right)=f\left(x_{1},\ldots ,x_{n}\right)-\sum
      \limits _{k=1}^{M}{\lambda _{k}g_{k}\left(x_{1},\ldots ,x_{n}\right)}}  [
      {\displaystyle {\mathcal {L}}\left(x_{1},\ldots ,x_{n},\lambda _
      {1},\ldots ,\lambda _{M}\right)=f\left(x_{1},\ldots ,x_{n}\right)-\sum
      \limits _{k=1}^{M}{\lambda _{k}g_{k}\left(x_{1},\ldots ,x_{n}\right)}}]
and solve
          &#x2207;   x  1   , &#x2026; ,  x  n   ,  &#x03BB;  1   , &#x2026; ,
      &#x03BB;  M       L   (  x  1   , &#x2026; ,  x  n   ,  &#x03BB;  1   ,
      &#x2026; ,  &#x03BB;  M   ) = 0  &#x27FA;    {    &#x2207; f (  x  )
      &#x2212;  &#x2211;  k = 1   M     &#x03BB;  k    &#x2207;  g  k   (  x  )
      = 0      g  1   (  x  ) = &#x22EF; =  g  M   (  x  ) = 0
      {\displaystyle \nabla _{x_{1},\ldots ,x_{n},\lambda _{1},\ldots ,\lambda
      _{M}}{\mathcal {L}}(x_{1},\ldots ,x_{n},\lambda _{1},\ldots ,\lambda _
      {M})=0\iff {\begin{cases}\nabla f(\mathbf {x} )-\sum _{k=1}^{M}{\lambda _
      {k}\,\nabla g_{k}(\mathbf {x} )}=0\\g_{1}(\mathbf {x} )=\cdots =g_{M}
      (\mathbf {x} )=0\end{cases}}}  [{\displaystyle \nabla _{x_{1},\ldots ,x_
      {n},\lambda _{1},\ldots ,\lambda _{M}}{\mathcal {L}}(x_{1},\ldots ,x_
      {n},\lambda _{1},\ldots ,\lambda _{M})=0\iff {\begin{cases}\nabla f
      (\mathbf {x} )-\sum _{k=1}^{M}{\lambda _{k}\,\nabla g_{k}(\mathbf {x}
      )}=0\\g_{1}(\mathbf {x} )=\cdots =g_{M}(\mathbf {x} )=0\end{cases}}}]
which amounts to solving     n + M   {\displaystyle n+M}  [{\displaystyle n+M}]
equations in     n + M   {\displaystyle n+M}  [{\displaystyle n+M}] unknowns.
The method of Lagrange multipliers is generalized by the KarushâKuhnâTucker
conditions, which can also take into account inequality constraints of the form
h(x) â¤ c.
***** Modern formulation via differentiable manifolds[edit] *****
The problem of finding the local maxima and minima subject to constraints can
be generalized to finding local maxima and minima on a differentiable_manifold
M   {\displaystyle M}  [M].[11] In what follows, it is not necessary that     M
{\displaystyle M}  [M] be a Euclidean space, or even a Riemannian manifold. All
appearances of the gradient     &#x2207;   {\displaystyle \nabla }  [\nabla ]
(which depends on a choice of Riemannian metric) can be replaced with the
exterior_derivative     d   {\displaystyle d}  [d].
**** Single constraint[edit] ****
Let     M   {\displaystyle M}  [M] be a smooth_manifold of dimension     m
{\displaystyle m}  [m]. Suppose that we wish to find the stationary points
x   {\displaystyle x}  [x] of a smooth function     f : M &#x2192;  R
{\displaystyle f:M\to \mathbb {R} }  [{\displaystyle f:M\to \mathbb {R} }] when
restricted to the submanifold     N   {\displaystyle N}  [N] defined by     g
( x ) = 0 ,   {\displaystyle g(x)=0,}  [{\displaystyle g(x)=0,}] where     g :
M &#x2192;  R    {\displaystyle g:M\to \mathbb {R} }  [{\displaystyle g:M\to
\mathbb {R} }] is a smooth function for which 0 is a regular_value of     g
{\displaystyle g}  [g].
Let     d f   {\displaystyle df}  [df] and     d g   {\displaystyle dg}  [
{\displaystyle dg}] be the exterior_derivatives. Stationarity for the
restriction     f   |   N     {\displaystyle f|_{N}}  [{\displaystyle f|_{N}}]
at     x &#x2208; N   {\displaystyle x\in N}  [{\displaystyle x\in N}] means
d ( f   |   N    )  x   = 0.   {\displaystyle d(f|_{N})_{x}=0.}  [
{\displaystyle d(f|_{N})_{x}=0.}] Equivalently, the kernel     ker &#x2061; ( d
f  x   )   {\displaystyle \ker(df_{x})}  [{\displaystyle \ker(df_{x})}]
contains      T  x   N = ker &#x2061; ( d  g  x   ) .   {\displaystyle T_
{x}N=\ker(dg_{x}).}  [{\displaystyle T_{x}N=\ker(dg_{x}).}] In other words,
d  f  x     {\displaystyle df_{x}}  [df_x] and     d  g  x     {\displaystyle
dg_{x}}  [{\displaystyle dg_{x}}] are proportional vectors. For this it is
necessary and sufficient that the following system of     m ( m &#x2212; 1 )  /
2   {\displaystyle m(m-1)/2}  [m(m-1)/2] equations holds:
         d  f  x   &#x2227; d  g  x   = 0 &#x2208;  &#x039B;  2   (  T  x
      &#x2217;   M )   {\displaystyle df_{x}\wedge dg_{x}=0\in \Lambda ^{2}(T_
      {x}^{*}M)}  [{\displaystyle df_{x}\wedge dg_{x}=0\in \Lambda ^{2}(T_{x}^
      {*}M)}]
where     &#x2227;   {\displaystyle \wedge }  [\wedge ] denotes the exterior
product. The stationary points     x   {\displaystyle x}  [x] are the solutions
of the above system of equations plus the constraint     g ( x ) = 0.
{\displaystyle g(x)=0.}  [{\displaystyle g(x)=0.}] Note that the        1 2
m ( m &#x2212; 1 )   {\displaystyle {\tfrac {1}{2}}m(m-1)}  [{\displaystyle
{\tfrac {1}{2}}m(m-1)}] equations are not independent, since the left-hand side
of the equation belongs to the subvariety of      &#x039B;  2   (  T  x
&#x2217;   M )   {\displaystyle \Lambda ^{2}(T_{x}^{*}M)}  [{\displaystyle
\Lambda ^{2}(T_{x}^{*}M)}] consisting of decomposable_elements.
In this formulation, it is not necessary to explicitly find the Lagrange
multiplier, a number     &#x03BB;   {\displaystyle \lambda }  [\lambda ] such
that     d  f  x   = &#x03BB;  d  g  x   .   {\displaystyle df_{x}=\lambda
\,dg_{x}.}  [{\displaystyle df_{x}=\lambda \,dg_{x}.}]
**** Multiple constraints[edit] ****
Let     M   {\displaystyle M}  [M] and     f   {\displaystyle f}  [f] be as in
the above section regarding the case of a single constraint. Rather than the
function     g   {\displaystyle g}  [g] described there, now consider a smooth
function     G : M &#x2192;   R   p   ( p > 1 ) ,   {\displaystyle G:M\to
\mathbb {R} ^{p}(p>1),}  [{\displaystyle G:M\to \mathbb {R} ^{p}(p>1),}] with
component functions      g  i   : M &#x2192;  R  ,   {\displaystyle g_{i}:M\to
\mathbb {R} ,}  [{\displaystyle g_{i}:M\to \mathbb {R} ,}] for which     0
&#x2208;   R   p     {\displaystyle 0\in \mathbb {R} ^{p}}  [{\displaystyle
0\in \mathbb {R} ^{p}}] is a regular_value. Let     N   {\displaystyle N}  [N]
be the submanifold of     M   {\displaystyle M}  [M] defined by     G ( x ) =
0.   {\displaystyle G(x)=0.}  [{\displaystyle G(x)=0.}]
   x   {\displaystyle x}  [x] is a stationary point of     f   |   N
{\displaystyle f|_{N}}  [{\displaystyle f|_{N}}] if and only if     ker
&#x2061; ( d  f  x   )   {\displaystyle \ker(df_{x})}  [{\displaystyle \ker(df_
{x})}] contains     ker &#x2061; ( d  G  x   )   {\displaystyle \ker(dG_{x})}
[{\displaystyle \ker(dG_{x})}]. For convenience let      L  x   = d  f  x
{\displaystyle L_{x}=df_{x}}  [{\displaystyle L_{x}=df_{x}}] and      K  x   =
d  G  x   ,   {\displaystyle K_{x}=dG_{x},}  [{\displaystyle K_{x}=dG_{x},}]
where     d G   {\displaystyle dG}  [{\displaystyle dG}] denotes the tangent
map or Jacobian     T M &#x2192; T   R   p   .   {\displaystyle TM\to T\mathbb
{R} ^{p}.}  [{\displaystyle TM\to T\mathbb {R} ^{p}.}] The subspace     ker
&#x2061; (  K  x   )   {\displaystyle \ker(K_{x})}  [{\displaystyle \ker(K_
{x})}] has dimension smaller than that of     ker &#x2061; (  L  x   )
{\displaystyle \ker(L_{x})}  [{\displaystyle \ker(L_{x})}], namely     dim
&#x2061; ( ker &#x2061; (  L  x   ) ) = n &#x2212; 1   {\displaystyle \dim(\ker
(L_{x}))=n-1}  [{\displaystyle \dim(\ker(L_{x}))=n-1}] and     dim &#x2061;
( ker &#x2061; (  K  x   ) ) = n &#x2212; p .   {\displaystyle \dim(\ker(K_
{x}))=n-p.}  [{\displaystyle \dim(\ker(K_{x}))=n-p.}]     ker &#x2061; (  K  x
)   {\displaystyle \ker(K_{x})}  [{\displaystyle \ker(K_{x})}] belongs to
ker &#x2061; (  L  x   )   {\displaystyle \ker(L_{x})}  [{\displaystyle \ker(L_
{x})}] if and only if      L  x   &#x2208;  T  x   &#x2217;   M
{\displaystyle L_{x}\in T_{x}^{*}M}  [{\displaystyle L_{x}\in T_{x}^{*}M}]
belongs to the image of      K  x   &#x2217;   :   R   p &#x2217;   &#x2192;  T
x   &#x2217;   M .   {\displaystyle K_{x}^{*}:\mathbb {R} ^{p*}\to T_{x}^{*}M.}
[{\displaystyle K_{x}^{*}:\mathbb {R} ^{p*}\to T_{x}^{*}M.}] Computationally
speaking, the condition is that      L  x     {\displaystyle L_{x}}  [L_{x}]
belongs to the row space of the matrix of      K  x   ,   {\displaystyle K_
{x},}  [{\displaystyle K_{x},}] or equivalently the column space of the matrix
of      K  x   &#x2217;     {\displaystyle K_{x}^{*}}  [{\displaystyle K_{x}^
{*}}] (the transpose). If      &#x03C9;  x   &#x2208;  &#x039B;  p   (  T  x
&#x2217;   M )   {\displaystyle \omega _{x}\in \Lambda ^{p}(T_{x}^{*}M)}  [
{\displaystyle \omega _{x}\in \Lambda ^{p}(T_{x}^{*}M)}] denotes the exterior
product of the columns of the matrix of      K  x   &#x2217;   ,
{\displaystyle K_{x}^{*},}  [{\displaystyle K_{x}^{*},}] the stationary
condition for     f   |   N     {\displaystyle f|_{N}}  [{\displaystyle f|_
{N}}] at     x   {\displaystyle x}  [x] becomes
          L  x   &#x2227;  &#x03C9;  x   = 0 &#x2208;  &#x039B;  p + 1    (   T
      x   &#x2217;   M  )    {\displaystyle L_{x}\wedge \omega _{x}=0\in
      \Lambda ^{p+1}\left(T_{x}^{*}M\right)}  [{\displaystyle L_{x}\wedge
      \omega _{x}=0\in \Lambda ^{p+1}\left(T_{x}^{*}M\right)}]
Once again, in this formulation it is not necessary to explicitly find the
Lagrange multipliers, the numbers      &#x03BB;  1   , &#x2026; ,  &#x03BB;  p
{\displaystyle \lambda _{1},\ldots ,\lambda _{p}}  [{\displaystyle \lambda _
{1},\ldots ,\lambda _{p}}] such that
         d  f  x   =  &#x2211;  i = 1   p    &#x03BB;  i   d (  g  i    )  x
      .   {\displaystyle df_{x}=\sum _{i=1}^{p}\lambda _{i}d(g_{i})_{x}.}  [
      {\displaystyle df_{x}=\sum _{i=1}^{p}\lambda _{i}d(g_{i})_{x}.}]
***** Interpretation of the Lagrange multipliers[edit] *****
Often the Lagrange multipliers have an interpretation as some quantity of
interest. For example, if the Lagrangian expression is
                L   (  x  1   ,  x  2   , &#x2026; ;  &#x03BB;  1   ,  &#x03BB;
      2   , &#x2026; )     =     f (  x  1   ,  x  2   , &#x2026; ) +  &#x03BB;
      1   (  c  1   &#x2212;  g  1   (  x  1   ,  x  2   , &#x2026; ) ) +
      &#x03BB;  2   (  c  2   &#x2212;  g  2   (  x  1   ,  x  2   , &#x2026; )
      ) + &#x22EF;       {\displaystyle {\begin{aligned}&{\mathcal {L}}(x_
      {1},x_{2},\ldots ;\lambda _{1},\lambda _{2},\ldots )\\[4pt]={}&f(x_{1},x_
      {2},\ldots )+\lambda _{1}(c_{1}-g_{1}(x_{1},x_{2},\ldots ))+\lambda _{2}
      (c_{2}-g_{2}(x_{1},x_{2},\dots ))+\cdots \end{aligned}}}  [{\displaystyle
      {\begin{aligned}&{\mathcal {L}}(x_{1},x_{2},\ldots ;\lambda _{1},\lambda
      _{2},\ldots )\\[4pt]={}&f(x_{1},x_{2},\ldots )+\lambda _{1}(c_{1}-g_{1}
      (x_{1},x_{2},\ldots ))+\lambda _{2}(c_{2}-g_{2}(x_{1},x_{2},\dots
      ))+\cdots \end{aligned}}}]
then
            &#x2202;   L     &#x2202;  c  k      =  &#x03BB;  k   .
      {\displaystyle {\frac {\partial {\mathcal {L}}}{\partial c_{k}}}=\lambda
      _{k}.}  [{\displaystyle {\frac {\partial {\mathcal {L}}}{\partial c_
      {k}}}=\lambda _{k}.}]
So, Î»k is the rate of change of the quantity being optimized as a function of
the constraint parameter. As examples, in Lagrangian_mechanics the equations of
motion are derived by finding stationary points of the action, the time
integral of the difference between kinetic and potential energy. Thus, the
force on a particle due to a scalar potential, F = ââV, can be interpreted
as a Lagrange multiplier determining the change in action (transfer of
potential to kinetic energy) following a variation in the particle's
constrained trajectory. In control theory this is formulated instead as costate
equations.
Moreover, by the envelope_theorem the optimal value of a Lagrange multiplier
has an interpretation as the marginal effect of the corresponding constraint
constant upon the optimal attainable value of the original objective function:
if we denote values at the optimum with an asterisk, then it can be shown that
             d  f (  x  1   &#x2217;   (  c  1   ,  c  2   , &#x2026; ) ,  x  2
      &#x2217;   (  c  1   ,  c  2   , &#x2026; ) , &#x2026; )    d   c  k
      =  &#x03BB;  k   &#x2217;   .   {\displaystyle {\frac {{\text{d}}f(x_{1}^
      {*}(c_{1},c_{2},\dots ),x_{2}^{*}(c_{1},c_{2},\dots ),\dots )}{{\text
      {d}}c_{k}}}=\lambda _{k}^{*}.}  [{\frac {{\text{d}}f(x_{1}^{*}(c_{1},c_
      {2},\dots ),x_{2}^{*}(c_{1},c_{2},\dots ),\dots )}{{\text{d}}c_
      {k}}}=\lambda _{k}^{*}.]
For example, in economics the optimal profit to a player is calculated subject
to a constrained space of actions, where a Lagrange multiplier is the change in
the optimal value of the objective function (profit) due to the relaxation of a
given constraint (e.g. through a change in income); in such a context Î»* is
the marginal_cost of the constraint, and is referred to as the shadow_price.
***** Sufficient conditions[edit] *****
Main article: Bordered_Hessian
Sufficient conditions for a constrained local maximum or minimum can be stated
in terms of a sequence of principal minors (determinants of upper-left-
justified sub-matrices) of the bordered Hessian_matrix of second derivatives of
the Lagrangian expression.[2][12]
***** Examples[edit] *****
**** Example 1[edit] ****
Illustration of the constrained optimization problem
*** Example 1a[edit] ***
Suppose we wish to maximize     f ( x , y ) = x + y   {\displaystyle f
(x,y)=x+y}  [f(x,y)=x+y] subject to the constraint      x  2   +  y  2   = 1
{\displaystyle x^{2}+y^{2}=1}  [x^{2}+y^{2}=1]. The feasible_set is the unit
circle, and the level_sets of f are diagonal lines (with slope â1), so we can
see graphically that the maximum occurs at      (      2  2    ,     2  2     )
{\displaystyle \left({\tfrac {\sqrt {2}}{2}},{\tfrac {\sqrt {2}}{2}}\right)}
[\left({\tfrac {\sqrt {2}}{2}},{\tfrac {\sqrt {2}}{2}}\right)], and that the
minimum occurs at      (  &#x2212;     2  2    , &#x2212;     2  2     )
{\displaystyle \left(-{\tfrac {\sqrt {2}}{2}},-{\tfrac {\sqrt {2}}{2}}\right)}
[\left(-{\tfrac {\sqrt {2}}{2}},-{\tfrac {\sqrt {2}}{2}}\right)].
For the method of Lagrange multipliers, the constraint is
         g ( x , y ) =  x  2   +  y  2   &#x2212; 1 ,   {\displaystyle g
      (x,y)=x^{2}+y^{2}-1,}  [{\displaystyle g(x,y)=x^{2}+y^{2}-1,}]
hence
               L   ( x , y , &#x03BB; )    = f ( x , y ) + &#x03BB; &#x22C5; g
      ( x , y )       = x + y + &#x03BB; (  x  2   +  y  2   &#x2212; 1 ) .
      {\displaystyle {\begin{aligned}{\mathcal {L}}(x,y,\lambda )&=f
      (x,y)+\lambda \cdot g(x,y)\\[4pt]&=x+y+\lambda (x^{2}+y^{2}-1).\end
      {aligned}}}  [{\displaystyle {\begin{aligned}{\mathcal {L}}(x,y,\lambda
      )&=f(x,y)+\lambda \cdot g(x,y)\\[4pt]&=x+y+\lambda (x^{2}+y^{2}-1).\end
      {aligned}}}]
Now we can calculate the gradient:
              &#x2207;  x , y , &#x03BB;     L   ( x , y , &#x03BB; )    =
      (     &#x2202;   L     &#x2202; x    ,    &#x2202;   L     &#x2202; y
      ,    &#x2202;   L     &#x2202; &#x03BB;     )        =  (  1 + 2 &#x03BB;
      x , 1 + 2 &#x03BB; y ,  x  2   +  y  2   &#x2212; 1  )
      {\displaystyle {\begin{aligned}\nabla _{x,y,\lambda }{\mathcal {L}}
      (x,y,\lambda )&=\left({\frac {\partial {\mathcal {L}}}{\partial x}},
      {\frac {\partial {\mathcal {L}}}{\partial y}},{\frac {\partial {\mathcal
      {L}}}{\partial \lambda }}\right)\\[4pt]&=\left(1+2\lambda x,1+2\lambda
      y,x^{2}+y^{2}-1\right)\end{aligned}}}  [{\displaystyle {\begin
      {aligned}\nabla _{x,y,\lambda }{\mathcal {L}}(x,y,\lambda )&=\left({\frac
      {\partial {\mathcal {L}}}{\partial x}},{\frac {\partial {\mathcal {L}}}
      {\partial y}},{\frac {\partial {\mathcal {L}}}{\partial \lambda
      }}\right)\\[4pt]&=\left(1+2\lambda x,1+2\lambda y,x^{2}+y^{2}-
      1\right)\end{aligned}}}]
and therefore:
          &#x2207;  x , y , &#x03BB;     L   ( x , y , &#x03BB; ) = 0  &#x21D4;
      {    1 + 2 &#x03BB; x = 0     1 + 2 &#x03BB; y = 0      x  2   +  y  2
      &#x2212; 1 = 0         {\displaystyle \nabla _{x,y,\lambda }{\mathcal
      {L}}(x,y,\lambda )=0\quad \Leftrightarrow \quad {\begin{cases}1+2\lambda
      x=0\\1+2\lambda y=0\\x^{2}+y^{2}-1=0\end{cases}}}  [{\displaystyle \nabla
      _{x,y,\lambda }{\mathcal {L}}(x,y,\lambda )=0\quad \Leftrightarrow \quad
      {\begin{cases}1+2\lambda x=0\\1+2\lambda y=0\\x^{2}+y^{2}-1=0\end
      {cases}}}]
Notice that the last equation is the original constraint.
The first two equations yield
         x = y = &#x2212;   1  2 &#x03BB;    ,  &#x03BB; &#x2260; 0.
      {\displaystyle x=y=-{\frac {1}{2\lambda }},\qquad \lambda \neq 0.}  [
      {\displaystyle x=y=-{\frac {1}{2\lambda }},\qquad \lambda \neq 0.}]
By substituting into the last equation we have:
           1  4  &#x03BB;  2      +   1  4  &#x03BB;  2      &#x2212; 1 = 0 ,
      {\displaystyle {\frac {1}{4\lambda ^{2}}}+{\frac {1}{4\lambda ^{2}}}-
      1=0,}  [{\displaystyle {\frac {1}{4\lambda ^{2}}}+{\frac {1}{4\lambda ^
      {2}}}-1=0,}]
so
         &#x03BB; = &#x00B1;   1  2    ,   {\displaystyle \lambda =\pm {\frac
      {1}{\sqrt {2}}},}  [{\displaystyle \lambda =\pm {\frac {1}{\sqrt {2}}},}]
which implies that the stationary points of       L     {\displaystyle
{\mathcal {L}}}  [{\mathcal {L}}] are
          (      2  2    ,     2  2    , &#x2212;    1  2      )  ,
      (  &#x2212;     2  2    , &#x2212;     2  2    ,    1  2      )  .
      {\displaystyle \left({\tfrac {\sqrt {2}}{2}},{\tfrac {\sqrt {2}}{2}},-
      {\tfrac {1}{\sqrt {2}}}\right),\qquad \left(-{\tfrac {\sqrt {2}}{2}},-
      {\tfrac {\sqrt {2}}{2}},{\tfrac {1}{\sqrt {2}}}\right).}  [{\displaystyle
      \left({\tfrac {\sqrt {2}}{2}},{\tfrac {\sqrt {2}}{2}},-{\tfrac {1}{\sqrt
      {2}}}\right),\qquad \left(-{\tfrac {\sqrt {2}}{2}},-{\tfrac {\sqrt {2}}
      {2}},{\tfrac {1}{\sqrt {2}}}\right).}]
Evaluating the objective function f at these points yields
         f  (      2  2    ,     2  2     )  =   2   ,  f  (  &#x2212;     2  2
      , &#x2212;     2  2     )  = &#x2212;   2   .   {\displaystyle f\left(
      {\tfrac {\sqrt {2}}{2}},{\tfrac {\sqrt {2}}{2}}\right)={\sqrt {2}},\qquad
      f\left(-{\tfrac {\sqrt {2}}{2}},-{\tfrac {\sqrt {2}}{2}}\right)=-{\sqrt
      {2}}.}  [{\displaystyle f\left({\tfrac {\sqrt {2}}{2}},{\tfrac {\sqrt
      {2}}{2}}\right)={\sqrt {2}},\qquad f\left(-{\tfrac {\sqrt {2}}{2}},-
      {\tfrac {\sqrt {2}}{2}}\right)=-{\sqrt {2}}.}]
Thus the constrained maximum is       2     {\displaystyle {\sqrt {2}}}  [
{\sqrt {2}}] and the constrained minimum is     &#x2212;   2     {\displaystyle
-{\sqrt {2}}}  [-{\sqrt {2}}].
*** Example 1b[edit] ***
Now we modify the objective function of Example 1a so that we minimize     f
( x , y ) = ( x + y  )  2     {\displaystyle f(x,y)=(x+y)^{2}}  [f(x,y)=
(x+y)^2] instead of     f ( x , y ) = x + y ,   {\displaystyle f(x,y)=x+y,}  [
{\displaystyle f(x,y)=x+y,}] again along the circle     g ( x , y ) =  x  2   +
y  2   &#x2212; 1 = 0   {\displaystyle g(x,y)=x^{2}+y^{2}-1=0}  [{\displaystyle
g(x,y)=x^{2}+y^{2}-1=0}]. Now the level sets of f are still lines of slope
â1, and the points on the circle tangent to these level sets are again
(   2    /  2 ,   2    /  2 )   {\displaystyle ({\sqrt {2}}/2,{\sqrt {2}}/2)}
[({\sqrt {2}}/2,{\sqrt {2}}/2)] and     ( &#x2212;   2    /  2 , &#x2212;   2
/  2 )   {\displaystyle (-{\sqrt {2}}/2,-{\sqrt {2}}/2)}  [(-{\sqrt {2}}/2,-
{\sqrt {2}}/2)]. These tangency points are maxima of f.
On the other hand, the minima occur on the level set for f = 0 (since by its
construction f cannot take negative values), at     (   2    /  2 , &#x2212;
2    /  2 )   {\displaystyle ({\sqrt {2}}/2,-{\sqrt {2}}/2)}  [(\sqrt{2}/2,-
\sqrt{2}/2)] and     ( &#x2212;   2    /  2 ,   2    /  2 )   {\displaystyle (-
{\sqrt {2}}/2,{\sqrt {2}}/2)}  [{\displaystyle (-{\sqrt {2}}/2,{\sqrt {2}}/
2)}], where the level curves of f are not tangent to the constraint. The
condition that     &#x2207; f = &#x03BB;  &#x2207; g   {\displaystyle \nabla
f=\lambda \,\nabla g}  [\nabla f=\lambda \, \nabla g] correctly identifies all
four points as extrema; the minima are characterized in particular by
&#x03BB; = 0.   {\displaystyle \lambda =0.}  [{\displaystyle \lambda =0.}]
**** Example 2[edit] ****
Illustration of the constrained optimization problem
In this example we will deal with some more strenuous calculations, but it is
still a single constraint problem.
Suppose we want to find the maximum values of
         f ( x , y ) =  x  2   y   {\displaystyle f(x,y)=x^{2}y}  [f(x,y)=x^
      {2}y]
with the condition that the x and y coordinates lie on the circle around the
origin with radius √3, that is, subject to the constraint
         g ( x , y ) =  x  2   +  y  2   &#x2212; 3 = 0.   {\displaystyle g
      (x,y)=x^{2}+y^{2}-3=0.}  [{\displaystyle g(x,y)=x^{2}+y^{2}-3=0.}]
As there is just a single constraint, we will use only one multiplier, say Î».
The constraint g(x, y) is identically zero on the circle of radius √3. See that
any multiple of g(x, y) may be added to f(x, y) leaving f(x, y) unchanged in
the region of interest (on the circle where our original constraint is
satisfied).
Apply the ordinary Langrange multiplier method. Let:
               L   ( x , y , &#x03BB; )    = f ( x , y ) + &#x03BB; &#x22C5; g
      ( x , y )       =  x  2   y + &#x03BB; (  x  2   +  y  2   &#x2212; 3 )
      {\displaystyle {\begin{aligned}{\mathcal {L}}(x,y,\lambda )&=f
      (x,y)+\lambda \cdot g(x,y)\\&=x^{2}y+\lambda (x^{2}+y^{2}-3)\end
      {aligned}}}  [{\displaystyle {\begin{aligned}{\mathcal {L}}(x,y,\lambda
      )&=f(x,y)+\lambda \cdot g(x,y)\\&=x^{2}y+\lambda (x^{2}+y^{2}-3)\end
      {aligned}}}]
Now we can calculate the gradient:
              &#x2207;  x , y , &#x03BB;     L   ( x , y , &#x03BB; )    =
      (     &#x2202;   L     &#x2202; x    ,    &#x2202;   L     &#x2202; y
      ,    &#x2202;   L     &#x2202; &#x03BB;     )        =  (  2 x y + 2
      &#x03BB; x ,  x  2   + 2 &#x03BB; y ,  x  2   +  y  2   &#x2212; 3  )
      {\displaystyle {\begin{aligned}\nabla _{x,y,\lambda }{\mathcal {L}}
      (x,y,\lambda )&=\left({\frac {\partial {\mathcal {L}}}{\partial x}},
      {\frac {\partial {\mathcal {L}}}{\partial y}},{\frac {\partial {\mathcal
      {L}}}{\partial \lambda }}\right)\\&=\left(2xy+2\lambda x,x^{2}+2\lambda
      y,x^{2}+y^{2}-3\right)\end{aligned}}}  [{\displaystyle {\begin
      {aligned}\nabla _{x,y,\lambda }{\mathcal {L}}(x,y,\lambda )&=\left({\frac
      {\partial {\mathcal {L}}}{\partial x}},{\frac {\partial {\mathcal {L}}}
      {\partial y}},{\frac {\partial {\mathcal {L}}}{\partial \lambda
      }}\right)\\&=\left(2xy+2\lambda x,x^{2}+2\lambda y,x^{2}+y^{2}-
      3\right)\end{aligned}}}]
And therefore:
          &#x2207;  x , y , &#x03BB;     L   ( x , y , &#x03BB; ) = 0  &#x21D4;
      {    2 x y + 2 &#x03BB; x = 0      x  2   + 2 &#x03BB; y = 0      x  2
      +  y  2   &#x2212; 3 = 0        &#x21D4;    {    x ( y + &#x03BB; ) = 0
      (i)       x  2   = &#x2212; 2 &#x03BB; y    (ii)       x  2   +  y  2   =
      3    (iii)          {\displaystyle \nabla _{x,y,\lambda }{\mathcal {L}}
      (x,y,\lambda )=0\quad \Leftrightarrow \quad {\begin{cases}2xy+2\lambda
      x=0\\x^{2}+2\lambda y=0\\x^{2}+y^{2}-3=0\end{cases}}\quad \Leftrightarrow
      \quad {\begin{cases}x(y+\lambda )=0&{\text{(i)}}\\x^{2}=-2\lambda y&
      {\text{(ii)}}\\x^{2}+y^{2}=3&{\text{(iii)}}\end{cases}}}  [{\displaystyle
      \nabla _{x,y,\lambda }{\mathcal {L}}(x,y,\lambda )=0\quad \Leftrightarrow
      \quad {\begin{cases}2xy+2\lambda x=0\\x^{2}+2\lambda y=0\\x^{2}+y^{2}-
      3=0\end{cases}}\quad \Leftrightarrow \quad {\begin{cases}x(y+\lambda )=0&
      {\text{(i)}}\\x^{2}=-2\lambda y&{\text{(ii)}}\\x^{2}+y^{2}=3&{\text{
      (iii)}}\end{cases}}}]
Notice that (iii) is just the original constraint. (i) implies x = 0 or Î» =
ây. If x = 0 then     y = &#x00B1;   3     {\displaystyle y=\pm {\sqrt {3}}}
[y=\pm {\sqrt {3}}] by (iii) and consequently Î» = 0 from (ii). If Î» = ây,
substituting in (ii) we get x2 = 2y2. Substituting this in (iii) and solving
for y gives y = Â±1. Thus there are six critical points of       L
{\displaystyle {\mathcal {L}}}  [{\mathcal {L}}]:
         (   2   , 1 , &#x2212; 1 ) ;  ( &#x2212;   2   , 1 , &#x2212; 1 ) ;
      (   2   , &#x2212; 1 , 1 ) ;  ( &#x2212;   2   , &#x2212; 1 , 1 ) ;  ( 0
      ,   3   , 0 ) ;  ( 0 , &#x2212;   3   , 0 ) .   {\displaystyle ({\sqrt
      {2}},1,-1);\quad (-{\sqrt {2}},1,-1);\quad ({\sqrt {2}},-1,1);\quad (-
      {\sqrt {2}},-1,1);\quad (0,{\sqrt {3}},0);\quad (0,-{\sqrt {3}},0).}  [
      {\displaystyle ({\sqrt {2}},1,-1);\quad (-{\sqrt {2}},1,-1);\quad ({\sqrt
      {2}},-1,1);\quad (-{\sqrt {2}},-1,1);\quad (0,{\sqrt {3}},0);\quad (0,-
      {\sqrt {3}},0).}]
Evaluating the objective at these points, we find that
         f ( &#x00B1;   2   , 1 ) = 2 ;  f ( &#x00B1;   2   , &#x2212; 1 ) =
      &#x2212; 2 ;  f ( 0 , &#x00B1;   3   ) = 0.   {\displaystyle f(\pm {\sqrt
      {2}},1)=2;\quad f(\pm {\sqrt {2}},-1)=-2;\quad f(0,\pm {\sqrt {3}})=0.}
      [f(\pm {\sqrt {2}},1)=2;\quad f(\pm {\sqrt {2}},-1)=-2;\quad f(0,\pm
      {\sqrt {3}})=0.]
Therefore, the objective function attains the global_maximum (subject to the
constraints) at     ( &#x00B1;   2   , 1 )   {\displaystyle (\pm {\sqrt
{2}},1)}  [(\pm {\sqrt {2}},1)] and the global_minimum at     ( &#x00B1;   2
, &#x2212; 1 ) .   {\displaystyle (\pm {\sqrt {2}},-1).}  [(\pm {\sqrt {2}},-
1).] The point     ( 0 ,   3   )   {\displaystyle (0,{\sqrt {3}})}  [(0,{\sqrt
{3}})] is a local_minimum of f and     ( 0 , &#x2212;   3   )   {\displaystyle
(0,-{\sqrt {3}})}  [(0,-{\sqrt {3}})] is a local_maximum of f, as may be
determined by consideration of the Hessian_matrix of       L   ( x , y , 0 )
{\displaystyle {\mathcal {L}}(x,y,0)}  [{\mathcal {L}}(x,y,0)].
Note that while     (   2   , 1 , &#x2212; 1 )   {\displaystyle ({\sqrt
{2}},1,-1)}  [({\sqrt {2}},1,-1)] is a critical point of       L
{\displaystyle {\mathcal {L}}}  [{\mathcal {L}}], it is not a local extremum of
L   .   {\displaystyle {\mathcal {L}}.}  [{\mathcal {L}}.] We have
           L    (    2   + &#x03B5; , 1 , &#x2212; 1 + &#x03B4;  )  = 2 +
      &#x03B4;  (   &#x03B5;  2   +  (  2   2    )  &#x03B5;  )  .
      {\displaystyle {\mathcal {L}}\left({\sqrt {2}}+\varepsilon ,1,-1+\delta
      \right)=2+\delta \left(\varepsilon ^{2}+\left(2{\sqrt
      {2}}\right)\varepsilon \right).}  [{\displaystyle {\mathcal {L}}\left(
      {\sqrt {2}}+\varepsilon ,1,-1+\delta \right)=2+\delta \left(\varepsilon ^
      {2}+\left(2{\sqrt {2}}\right)\varepsilon \right).}]
Given any neighbourhood of     (   2   , 1 , &#x2212; 1 )   {\displaystyle (
{\sqrt {2}},1,-1)}  [({\sqrt {2}},1,-1)], we can choose a small positive
&#x03B5;   {\displaystyle \varepsilon }  [\varepsilon ] and a small
&#x03B4;   {\displaystyle \delta }  [\delta ] of either sign to get       L
{\displaystyle {\mathcal {L}}}  [{\mathcal {L}}] values both greater and less
than     2   {\displaystyle 2}  [2]. This can also be seen from the fact that
the Hessian matrix of       L     {\displaystyle {\mathcal {L}}}  [{\mathcal
{L}}] evaluated at this point (or indeed at any of the critical points) is an
indefinite_matrix. Each of the critical points of       L     {\displaystyle
{\mathcal {L}}}  [{\mathcal {L}}] is a saddle_point of       L   .
{\displaystyle {\mathcal {L}}.}  [{\mathcal {L}}.]
**** Example 3: Entropy[edit] ****
Suppose we wish to find the discrete_probability_distribution on the points
{  p  1   ,  p  2   , &#x2026; ,  p  n   }   {\displaystyle \{p_{1},p_
{2},\ldots ,p_{n}\}}  [\{p_{1},p_{2},\ldots ,p_{n}\}] with maximal information
entropy. This is the same as saying that we wish to find the least_structured
probability distribution on the points     {  p  1   ,  p  2   , &#x22EF; ,  p
n   }   {\displaystyle \{p_{1},p_{2},\cdots ,p_{n}\}}  [{\displaystyle \{p_
{1},p_{2},\cdots ,p_{n}\}}]. In other words, we wish to maximize the Shannon
entropy equation:
         f (  p  1   ,  p  2   , &#x2026; ,  p  n   ) = &#x2212;  &#x2211;  j =
      1   n    p  j    log  2   &#x2061;  p  j   .   {\displaystyle f(p_{1},p_
      {2},\ldots ,p_{n})=-\sum _{j=1}^{n}p_{j}\log _{2}p_{j}.}  [f(p_{1},p_
      {2},\ldots ,p_{n})=-\sum _{j=1}^{n}p_{j}\log _{2}p_{j}.]
For this to be a probability distribution the sum of the probabilities      p
i     {\displaystyle p_{i}}  [p_{i}] at each point      x  i     {\displaystyle
x_{i}}  [x_{i}] must equal 1, so our constraint is:
         g (  p  1   ,  p  2   , &#x2026; ,  p  n   ) =  &#x2211;  j = 1   n
      p  j   = 1.   {\displaystyle g(p_{1},p_{2},\ldots ,p_{n})=\sum _{j=1}^
      {n}p_{j}=1.}  [g(p_{1},p_{2},\ldots ,p_{n})=\sum _{j=1}^{n}p_{j}=1.]
We use Lagrange multipliers to find the point of maximum entropy,         p
&#x2192;      &#x2217;     {\displaystyle {\vec {p}}^{\,*}}  [{\vec {p}}^
{\,*}], across all discrete probability distributions        p &#x2192;
{\displaystyle {\vec {p}}}  [{\vec {p}}] on     {  x  1   ,  x  2   , &#x2026;
,  x  n   }   {\displaystyle \{x_{1},x_{2},\ldots ,x_{n}\}}  [\{x_{1},x_
{2},\ldots ,x_{n}\}]. We require that:
               &#x2202;  &#x2202;    p &#x2192;       ( f + &#x03BB; ( g
      &#x2212; 1 ) )  |      p &#x2192;    =     p &#x2192;      &#x2217;     =
      0 ,   {\displaystyle \left.{\frac {\partial }{\partial {\vec {p}}}}
      (f+\lambda (g-1))\right|_{{\vec {p}}={\vec {p}}^{\,*}}=0,}  [\left.{\frac
      {\partial }{\partial {\vec {p}}}}(f+\lambda (g-1))\right|_{{\vec {p}}=
      {\vec {p}}^{\,*}}=0,]
which gives a system of n equations,     k = 1 , &#x2026; , n   {\displaystyle
k=1,\ldots ,n}  [{\displaystyle k=1,\ldots ,n}], such that:
               &#x2202;  &#x2202;  p  k       {  &#x2212;  (   &#x2211;  j = 1
      n    p  j    log  2   &#x2061;  p  j    )  + &#x03BB;  (   &#x2211;  j =
      1   n    p  j   &#x2212; 1  )   }   |    p  k   =  p  k   &#x2217;     =
      0.   {\displaystyle \left.{\frac {\partial }{\partial p_{k}}}\left\{-
      \left(\sum _{j=1}^{n}p_{j}\log _{2}p_{j}\right)+\lambda \left(\sum _
      {j=1}^{n}p_{j}-1\right)\right\}\right|_{p_{k}=p_{k}^{*}}=0.}  [\left.
      {\frac {\partial }{\partial p_{k}}}\left\{-\left(\sum _{j=1}^{n}p_{j}\log
      _{2}p_{j}\right)+\lambda \left(\sum _{j=1}^{n}p_{j}-
      1\right)\right\}\right|_{p_{k}=p_{k}^{*}}=0.]
Carrying out the differentiation of these n equations, we get
         &#x2212;  (    1  ln &#x2061; 2    +  log  2   &#x2061;  p  k
      &#x2217;    )  + &#x03BB; = 0.   {\displaystyle -\left({\frac {1}{\ln
      2}}+\log _{2}p_{k}^{*}\right)+\lambda =0.}  [-\left({\frac {1}{\ln
      2}}+\log _{2}p_{k}^{*}\right)+\lambda =0.]
This shows that all      p  k   &#x2217;     {\displaystyle p_{k}^{*}}  [p_{k}^
{*}] are equal (because they depend on Î» only). By using the constraint
          &#x2211;  j    p  j   = 1 ,   {\displaystyle \sum _{j}p_{j}=1,}
      [\sum _{j}p_{j}=1,]
we find
          p  k   &#x2217;   =   1 n   .   {\displaystyle p_{k}^{*}={\frac {1}
      {n}}.}  [p_{k}^{*}={\frac {1}{n}}.]
Hence, the uniform distribution is the distribution with the greatest entropy,
among distributions on n points.
**** Example 4: Numerical optimization[edit] ****
Lagrange multipliers cause the critical points to occur at saddle points.
The magnitude of the gradient can be used to force the critical points to occur
at local minima.
The critical points of Lagrangians occur at saddle_points, rather than at local
maxima (or minima).[13] Unfortunately, many numerical optimization techniques,
such as hill_climbing, gradient_descent, some of the quasi-Newton_methods,
among others, are designed to find local maxima (or minima) and not saddle
points. For this reason, one must either modify the formulation to ensure that
it's a minimization problem (for example, by extremizing the square of the
gradient of the Lagrangian as below), or else use an optimization technique
that finds stationary_points (such as Newton's_method without an extremum
seeking line_search) and not necessarily extrema.
As a simple example, consider the problem of finding the value of x that
minimizes     f ( x ) =  x  2     {\displaystyle f(x)=x^{2}}  [f(x)=x^{2}],
constrained such that      x  2   = 1   {\displaystyle x^{2}=1}  [x^{2}=1].
(This problem is somewhat pathological because there are only two values that
satisfy this constraint, but it is useful for illustration purposes because the
corresponding unconstrained function can be visualized in three dimensions.)
Using Lagrange multipliers, this problem can be converted into an unconstrained
optimization problem:
           L   ( x , &#x03BB; ) =  x  2   + &#x03BB; (  x  2   &#x2212; 1 ) .
      {\displaystyle {\mathcal {L}}(x,\lambda )=x^{2}+\lambda (x^{2}-1).}  [
      {\mathcal {L}}(x,\lambda )=x^{2}+\lambda (x^{2}-1).]
The two critical points occur at saddle points where x = 1 and x = â1.
In order to solve this problem with a numerical optimization technique, we must
first transform this problem such that the critical points occur at local
minima. This is done by computing the magnitude of the gradient of the
unconstrained optimization problem.
First, we compute the partial derivative of the unconstrained problem with
respect to each variable:
                 &#x2202;   L     &#x2202; x    = 2 x + 2 x &#x03BB;
      &#x2202;   L     &#x2202; &#x03BB;    =  x  2   &#x2212; 1.
      {\displaystyle {\begin{aligned}&{\frac {\partial {\mathcal {L}}}{\partial
      x}}=2x+2x\lambda \\[5pt]&{\frac {\partial {\mathcal {L}}}{\partial
      \lambda }}=x^{2}-1.\end{aligned}}}  [{\displaystyle {\begin{aligned}&
      {\frac {\partial {\mathcal {L}}}{\partial x}}=2x+2x\lambda \\[5pt]&{\frac
      {\partial {\mathcal {L}}}{\partial \lambda }}=x^{2}-1.\end{aligned}}}]
If the target function is not easily differentiable, the differential with
respect to each variable can be approximated as
                &#x2202;   L     &#x2202; x    &#x2248;      L   ( x + &#x03B5;
      , &#x03BB; ) &#x2212;   L   ( x , &#x03BB; )  &#x03B5;   ,
      &#x2202;   L     &#x2202; &#x03BB;    &#x2248;      L   ( x , &#x03BB; +
      &#x03B5; ) &#x2212;   L   ( x , &#x03BB; )  &#x03B5;   ,
      {\displaystyle {\begin{aligned}{\frac {\partial {\mathcal {L}}}{\partial
      x}}\approx {\frac {{\mathcal {L}}(x+\varepsilon ,\lambda )-{\mathcal {L}}
      (x,\lambda )}{\varepsilon }},\\[5pt]{\frac {\partial {\mathcal {L}}}
      {\partial \lambda }}\approx {\frac {{\mathcal {L}}(x,\lambda +\varepsilon
      )-{\mathcal {L}}(x,\lambda )}{\varepsilon }},\end{aligned}}}  [
      {\displaystyle {\begin{aligned}{\frac {\partial {\mathcal {L}}}{\partial
      x}}\approx {\frac {{\mathcal {L}}(x+\varepsilon ,\lambda )-{\mathcal {L}}
      (x,\lambda )}{\varepsilon }},\\[5pt]{\frac {\partial {\mathcal {L}}}
      {\partial \lambda }}\approx {\frac {{\mathcal {L}}(x,\lambda +\varepsilon
      )-{\mathcal {L}}(x,\lambda )}{\varepsilon }},\end{aligned}}}]
where     &#x03B5;   {\displaystyle \varepsilon }  [\varepsilon ] is a small
value.
Next, we compute the magnitude of the gradient, which is the square root of the
sum of the squares of the partial derivatives:
             h ( x , &#x03BB; )    =   ( 2 x + 2 x &#x03BB;  )  2   + (  x  2
      &#x2212; 1  )  2           &#x2248;     (      L   ( x + &#x03B5; ,
      &#x03BB; ) &#x2212;   L   ( x , &#x03BB; )  &#x03B5;   )   2   +
      (      L   ( x , &#x03BB; + &#x03B5; ) &#x2212;   L   ( x , &#x03BB; )
      &#x03B5;   )   2     .       {\displaystyle {\begin{aligned}h(x,\lambda
      )&={\sqrt {(2x+2x\lambda )^{2}+(x^{2}-1)^{2}}}\\[4pt]&\approx {\sqrt
      {\left({\frac {{\mathcal {L}}(x+\varepsilon ,\lambda )-{\mathcal {L}}
      (x,\lambda )}{\varepsilon }}\right)^{2}+\left({\frac {{\mathcal {L}}
      (x,\lambda +\varepsilon )-{\mathcal {L}}(x,\lambda )}{\varepsilon
      }}\right)^{2}}}.\end{aligned}}}  [{\displaystyle {\begin{aligned}h
      (x,\lambda )&={\sqrt {(2x+2x\lambda )^{2}+(x^{2}-1)^{2}}}\\[4pt]&\approx
      {\sqrt {\left({\frac {{\mathcal {L}}(x+\varepsilon ,\lambda )-{\mathcal
      {L}}(x,\lambda )}{\varepsilon }}\right)^{2}+\left({\frac {{\mathcal {L}}
      (x,\lambda +\varepsilon )-{\mathcal {L}}(x,\lambda )}{\varepsilon
      }}\right)^{2}}}.\end{aligned}}}]
(Since magnitude is always non-negative, optimizing over the squared-magnitude
is equivalent to optimizing over the magnitude. Thus, the ''square root" may be
omitted from these equations with no expected difference in the results of
optimization.)
The critical points of h occur at x = 1 and x = â1, just as in       L
{\displaystyle {\mathcal {L}}}  [{\mathcal {L}}]. Unlike the critical points in
L     {\displaystyle {\mathcal {L}}}  [{\mathcal {L}}], however, the critical
points in h occur at local minima, so numerical optimization techniques can be
used to find them.
***** Applications[edit] *****
**** Control theory[edit] ****
In optimal_control theory, the Lagrange multipliers are interpreted as costate
variables, and Lagrange multipliers are reformulated as the minimization of the
Hamiltonian, in Pontryagin's_minimum_principle.
**** Nonlinear programming[edit] ****
The Lagrange multiplier method has several generalizations. In nonlinear
programming there are several multiplier rules, e.g. the CarathÃ©odoryâJohn
Multiplier Rule and the Convex Multiplier Rule, for inequality constraints.[14]
***** See also[edit] *****
    * Adjustment_of_observations
    * Duality
    * Gittins_index
    * KarushâKuhnâTucker_conditions: generalization of the method of
      Lagrange multipliers
    * Lagrange_multipliers_on_Banach_spaces: another generalization of the
      method of Lagrange multipliers
    * Lagrange_multiplier_test in maximum likelihood estimation
    * Lagrangian_relaxation
***** References[edit] *****
   1. ^Hoffmann, Laurence D.; Bradley, Gerald L. (2004). Calculus for Business,
      Economics, and the Social and Life Sciences (8th ed.). pp. 575â588.
      ISBN 0-07-242432-X.
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
   3. ^ a bSilberberg, Eugene; Suen, Wing (2001). The Structure of Economics :
      A Mathematical Analysis (Third ed.). Boston: Irwin McGraw-Hill.
      pp. 134â141. ISBN 0-07-234352-4.
   4. ^Luenberger,_David_G. (1969). Optimization by Vector Space Methods. New
      York: John Wiley & Sons. pp. 188â189.
   5. ^Beavis, Brian; Dobbs, Ian M. (1990). "Static_Optimization". Optimization
      and Stability Theory for Economic Analysis. New York: Cambridge
      University Press. p. 40. ISBN 0-521-33605-8.
   6. ^Protter,_Murray_H.; Morrey,_Charles_B.,_Jr. (1985). Intermediate
      Calculus (2nd ed.). New York: Springer. p. 267. ISBN 0-387-96058-9.
   7. ^Bertsekas,_Dimitri_P. (1999). Nonlinear Programming (Second ed.).
      Cambridge, MA.: Athena Scientific. ISBN 1-886529-00-0.
   8. ^Vapnyarskii, I.B. (2001) [1994], "Lagrange_multipliers", in Hazewinkel,
      Michiel (ed.), Encyclopedia_of_Mathematics, Springer Science+Business
      Media B.V. / Kluwer Academic Publishers, ISBN 978-1-55608-010-4
   9. .
  10. ^Lasdon, Leon S. (2002). Optimization Theory for Large Systems (Reprint
      of the 1970 Macmillan ed.). Mineola, New York: Dover. ISBN 0-486-41999-1.
      MR 1888251.
  11. ^Hiriart-Urruty, Jean-Baptiste; LemarÃ©chal,_Claude (1993). "XII Abstract
      duality for practitioners". Convex analysis and minimization algorithms,
      Volume II: Advanced theory and bundle methods. Grundlehren der
      Mathematischen Wissenschaften [Fundamental Principles of Mathematical
      Sciences]. 306. Berlin: Springer-Verlag. pp. 136â193 (and
      Bibliographical comments on pp.&nbsp, 334â335). ISBN 3-540-56852-2.
      MR 1295240.
  12. ^LemarÃ©chal,_Claude (2001). "Lagrangian relaxation". In JÃ¼nger,
      Michael; Naddef, Denis (eds.). Computational combinatorial optimization:
      Papers from the Spring School held in SchloÃ Dagstuhl,
      May 15â19, 2000. Lecture Notes in Computer Science. 2241. Berlin:
      Springer-Verlag. pp. 112â156. doi:10.1007/3-540-45586-8_4. ISBN 3-540-
      42877-1. MR 1900016.
  13. ^Lafontaine, Jacques (2015). An_Introduction_to_Differential_Manifolds.
      Springer. p. 70. ISBN 9783319207353.
  14. ^Chiang,_Alpha_C. (1984). Fundamental Methods of Mathematical Economics
      (Third ed.). McGraw-Hill. p. 386. ISBN 0-07-010813-7.
  15. ^Heath,_Michael_T. (2005). Scientific_Computing:_An_Introductory_Survey.
      McGraw-Hill. p. 203. ISBN 978-0-07-124489-3.
  16. ^Pourciau, Bruce H. (1980). "Modern_multiplier_rules". American
      Mathematical_Monthly. 87 (6): 433â452. doi:10.2307/2320250.
      JSTOR 2320250.
***** Further reading[edit] *****
    * Beavis, Brian; Dobbs, Ian M. (1990). "Static_Optimization". Optimization
      and Stability Theory for Economic Analysis. New York: Cambridge
      University Press. pp. 32â72. ISBN 0-521-33605-8.
Bertsekas,_Dimitri_P. (1982). Constrained Optimization and Lagrange Multiplier
Methods. New York: Academic Press. ISBN 0-12-093480-9.
Beveridge, Gordon S. G.; Schechter, Robert S. (1970). "Lagrangian_Multipliers".
Optimization: Theory and Practice. New York: McGraw-Hill. pp. 244â259.
ISBN 0-07-005128-3.
Binger, Brian R.; Hoffman, Elizabeth (1998). "Constrained Optimization".
Microeconomics with Calculus (2nd ed.). Reading: Addison-Wesley. pp. 56â91.
ISBN 0-321-01225-9.
Carter, Michael (2001). "Equality_Constraints". Foundations of Mathematical
Economics. Cambridge: MIT Press. pp. 516â549. ISBN 0-262-53192-5.
Hestenes,_Magnus_R. (1966). "Minima of functions subject to equality
constraints". Calculus of Variations and Optimal Control Theory. New York:
Wiley. pp. 29â34.
Wylie, C. Ray; Barrett, Louis C. (1995). "The Extrema of Integrals under
Constraint". Advanced Engineering Mathematics (Sixth ed.). New York: McGraw-
Hill. pp. 1096â1103. ISBN 0-07-072206-4.
***** External links[edit] *****
 The Wikibook Calculus_optimization_methods has a page on the topic of:
 Lagrange_multipliers
Exposition
    * Conceptual_introduction (plus a brief discussion of Lagrange multipliers
      in the calculus_of_variations as used in physics)
    * Lagrange_Multipliers_for_Quadratic_Forms_With_Linear_Constraints by
      Kenneth H. Carpenter
For additional text and interactive applets
    * Simple_explanation_with_an_example_of_governments_using_taxes_as_Lagrange
      multipliers
    * Lagrange_Multipliers_without_Permanent_Scarring Explanation with focus on
      the intuition by Dan Klein
    * Geometric_Representation_of_Method_of_Lagrange_Multipliers Provides
      compelling insight in 2 dimensions that at a minimizing point, the
      direction of steepest descent must be perpendicular to the tangent of the
      constraint curve at that point. [Needs InternetExplorer/Firefox/Safari]
      Mathematica demonstration by Shashi Sathyanarayana
    * Applet
    * MIT_OpenCourseware_Video_Lecture_on_Lagrange_Multipliers_from
      Multivariable_Calculus_course
    * Slides_accompanying_Bertsekas's_nonlinear_optimization_text, with details
      on Lagrange multipliers (lectures 11 and 12)
    * Geometric_idea_behind_Lagrange_multipliers
    * MATLAB_example_of_using_Lagrange_Multipliers_in_Optimization

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Lagrange_multiplier&oldid=907840371"
Categories:
    * Multivariable_calculus
    * Mathematical_optimization
    * Mathematical_and_quantitative_methods_(economics)
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * Tagalog
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 25 July 2019, at 16:33 (UTC).
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
