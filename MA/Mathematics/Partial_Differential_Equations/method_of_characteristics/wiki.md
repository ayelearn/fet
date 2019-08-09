The following text has been accessed from https://en.wikipedia.org/wiki/Method_of_characteristics at Fri Aug 9 02:36:48 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Method of characteristics ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, the method of characteristics is a technique for solving
partial_differential_equations. Typically, it applies to first-order_equations,
although more generally the method of characteristics is valid for any
hyperbolic_partial_differential_equation. The method is to reduce a partial
differential equation to a family of ordinary_differential_equations along
which the solution can be integrated from some initial data given on a suitable
hypersurface.
⁰
***** Contents *****
    * 1_Characteristics_of_first-order_partial_differential_equation
          o 1.1_Linear_and_quasilinear_cases
                # 1.1.1_Proof_for_Quasi-Linear_Case
          o 1.2_Fully_nonlinear_case
    * 2_Example
    * 3_Characteristics_of_linear_differential_operators
    * 4_Qualitative_analysis_of_characteristics
    * 5_See_also
    * 6_Notes
    * 7_References
    * 8_External_links
***** Characteristics of first-order partial differential equation[edit] *****
For a first-order PDE (partial_differential_equation), the method of
characteristics discovers curves (called characteristic curves or just
characteristics) along which the PDE becomes an ordinary_differential_equation
(ODE). Once the ODE is found, it can be solved along the characteristic curves
and transformed into a solution for the original PDE.
For the sake of simplicity, we confine our attention to the case of a function
of two independent variables x and y for the moment. Consider a quasilinear PDE
of the form
         a ( x , y , z )    &#x2202; z   &#x2202; x    + b ( x , y ,
      z )    &#x2202; z   &#x2202; y    = c ( x , y , z ) .
      {\displaystyle a(x,y,z){\frac {\partial z}{\partial x}}+b         (1)
      (x,y,z){\frac {\partial z}{\partial y}}=c(x,y,z).}  [a(x,y,z)     
      {\frac {\partial z}{\partial x}}+b(x,y,z){\frac {\partial z}
      {\partial y}}=c(x,y,z).]
Suppose that a solution z is known, and consider the surface graph z = z(x,y)
in R3. A normal_vector to this surface is given by
          (     &#x2202; z   &#x2202; x    ( x , y ) ,    &#x2202; z   &#x2202;
      y    ( x , y ) , &#x2212; 1  )  .    {\displaystyle \left({\frac
      {\partial z}{\partial x}}(x,y),{\frac {\partial z}{\partial y}}(x,y),-
      1\right).\,}  [\left({\frac {\partial z}{\partial x}}(x,y),{\frac
      {\partial z}{\partial y}}(x,y),-1\right).\,]
As a result,[1] equation (1) is equivalent to the geometrical statement that
the vector field
         ( a ( x , y , z ) , b ( x , y , z ) , c ( x , y , z ) )
      {\displaystyle (a(x,y,z),b(x,y,z),c(x,y,z))\,}  [(a(x,y,z),b(x,y,z),c
      (x,y,z))\,]
is tangent to the surface z = z(x,y) at every point, for the dot product of
this vector field with the above normal vector is zero. In other words, the
graph of the solution must be a union of integral_curves of this vector field.
These integral curves are called the characteristic curves of the original
partial differential equation and are given by the Lagrange-Charpit equations
[2]
                d x   d t      =   a ( x , y , z )        d y   d t      =   b
      ( x , y , z )        d z   d t      =   c ( x , y , z ) .
      {\displaystyle {\begin{array}{rcl}{\frac {dx}{dt}}&=&a(x,y,z)\\{\frac
      {dy}{dt}}&=&b(x,y,z)\\{\frac {dz}{dt}}&=&c(x,y,z).\end{array}}}  [{\begin
      {array}{rcl}{\frac {dx}{dt}}&=&a(x,y,z)\\{\frac {dy}{dt}}&=&b(x,y,z)\\
      {\frac {dz}{dt}}&=&c(x,y,z).\end{array}}]
A parametrization invariant form of the Lagrange-Charpit equations[2] is:
            d x   a ( x , y , z )    =    d y   b ( x , y , z )    =    d z   c
      ( x , y , z )    .   {\displaystyle {\frac {dx}{a(x,y,z)}}={\frac {dy}{b
      (x,y,z)}}={\frac {dz}{c(x,y,z)}}.}  [{\displaystyle {\frac {dx}{a
      (x,y,z)}}={\frac {dy}{b(x,y,z)}}={\frac {dz}{c(x,y,z)}}.}]
**** Linear and quasilinear cases[edit] ****
Consider now a PDE of the form
          &#x2211;  i = 1   n    a  i   (  x  1   , &#x2026; ,  x  n   , u )
      &#x2202; u   &#x2202;  x  i      = c (  x  1   , &#x2026; ,  x  n   , u )
      .   {\displaystyle \sum _{i=1}^{n}a_{i}(x_{1},\dots ,x_{n},u){\frac
      {\partial u}{\partial x_{i}}}=c(x_{1},\dots ,x_{n},u).}  [\sum _{i=1}^
      {n}a_{i}(x_{1},\dots ,x_{n},u){\frac {\partial u}{\partial x_{i}}}=c(x_
      {1},\dots ,x_{n},u).]
For this PDE to be linear, the coefficients ai may be functions of the spatial
variables only, and independent of u. For it to be quasilinear, ai may also
depend on the value of the function, but not on any derivatives. The
distinction between these two cases is inessential for the discussion here.
For a linear or quasilinear PDE, the characteristic curves are given
parametrically by
         (  x  1   , &#x2026; ,  x  n   , u ) = (  x  1   ( s ) , &#x2026; ,  x
      n   ( s ) , u ( s ) )   {\displaystyle (x_{1},\dots ,x_{n},u)=(x_{1}
      (s),\dots ,x_{n}(s),u(s))}  [(x_{1},\dots ,x_{n},u)=(x_{1}(s),\dots ,x_
      {n}(s),u(s))]
         u (  X  ( s ) ) = U ( s )   {\displaystyle u(\mathbf {X} (s))=U(s)}  [
      {\displaystyle u(\mathbf {X} (s))=U(s)}]
such that the following system of ODEs is satisfied
            d  x  i     d s    =  a  i   (  x  1   , &#x2026; ,  x  n    
      , u )   {\displaystyle {\frac {dx_{i}}{ds}}=a_{i}(x_{1},\dots        (2)
      ,x_{n},u)}  [{\frac {dx_{i}}{ds}}=a_{i}(x_{1},\dots ,x_{n},u)]
            d u   d s    = c (  x  1   , &#x2026; ,  x  n   , u ) .    
      {\displaystyle {\frac {du}{ds}}=c(x_{1},\dots ,x_{n},u).}  [       (3)
      {\frac {du}{ds}}=c(x_{1},\dots ,x_{n},u).]
Equations (2) and (3) give the characteristics of the PDE.
*** Proof for Quasi-Linear Case[edit] ***
In the Quasi-Linear case, the use of the method of characteristics is justified
by GrÃ¶nwall's_Inequality. The above equation may be written as
    a  (  x  , u ) &#x22C5; &#x2207; u (  x  ) = c (  x  , u )   {\displaystyle
\mathbf {a} (\mathbf {x} ,u)\cdot \nabla u(\mathbf {x} )=c(\mathbf {x} ,u)}  [
{\displaystyle \mathbf {a} (\mathbf {x} ,u)\cdot \nabla u(\mathbf {x} )=c
(\mathbf {x} ,u)}]
We must distinguish between the solutions to the ODE and the solutions to the
PDE, which we do not know are equal a priori. Letting capital letters be the
solutions to the ODE we find
     X  &#x2032;  ( s ) =  a  (  X  ( s ) , U ( s ) )   {\displaystyle \mathbf
{X} '(s)=\mathbf {a} (\mathbf {X} (s),U(s))}  [{\displaystyle \mathbf {X} '
(s)=\mathbf {a} (\mathbf {X} (s),U(s))}]
    U &#x2032;  ( s ) = c (  X  ( s ) , U ( s ) )   {\displaystyle U'(s)=c
(\mathbf {X} (s),U(s))}  [{\displaystyle U'(s)=c(\mathbf {X} (s),U(s))}]
Examining     &#x0394; ( s ) =  |  u (  X  ( s ) ) &#x2212; U ( s )   |   2
{\displaystyle \Delta (s)=|u(\mathbf {X} (s))-U(s)|^{2}}  [{\displaystyle
\Delta (s)=|u(\mathbf {X} (s))-U(s)|^{2}}], we find, upon differentiating that
    &#x0394; &#x2032;  ( s ) = 2   (   u (  X  ( s ) ) &#x2212; U ( s )   )
(     X  &#x2032;  ( s ) &#x22C5; &#x2207; u (  X  ( s ) ) &#x2212;  U &#x2032;
( s )   )     {\displaystyle \Delta '(s)=2{\big (}u(\mathbf {X} (s))-U(s){\big
)}{\Big (}\mathbf {X} '(s)\cdot \nabla u(\mathbf {X} (s))-U'(s){\Big )}}  [
{\displaystyle \Delta '(s)=2{\big (}u(\mathbf {X} (s))-U(s){\big )}{\Big
(}\mathbf {X} '(s)\cdot \nabla u(\mathbf {X} (s))-U'(s){\Big )}}]
which is the same as
    &#x0394; &#x2032;  ( s ) = 2   (   u (  X  ( s ) ) &#x2212; U ( s )   )
(    a  (  X  ( s ) , U ( s ) ) &#x22C5; &#x2207; u (  X  ( s ) ) &#x2212; c
(  X  ( s ) , U ( s ) )   )     {\displaystyle \Delta '(s)=2{\big (}u(\mathbf
{X} (s))-U(s){\big )}{\Big (}\mathbf {a} (\mathbf {X} (s),U(s))\cdot \nabla u
(\mathbf {X} (s))-c(\mathbf {X} (s),U(s)){\Big )}}  [{\displaystyle \Delta '
(s)=2{\big (}u(\mathbf {X} (s))-U(s){\big )}{\Big (}\mathbf {a} (\mathbf {X}
(s),U(s))\cdot \nabla u(\mathbf {X} (s))-c(\mathbf {X} (s),U(s)){\Big )}}]
We cannot conclude the above is 0 as we would like, since the PDE only
guarantees us that this relationship is satisfied for     u (  x  )
{\displaystyle u(\mathbf {x} )}  [u(\mathbf {x} )],      a  (  x  , u )
&#x22C5; &#x2207; u (  x  ) = c (  x  , u )   {\displaystyle \mathbf {a}
(\mathbf {x} ,u)\cdot \nabla u(\mathbf {x} )=c(\mathbf {x} ,u)}  [
{\displaystyle \mathbf {a} (\mathbf {x} ,u)\cdot \nabla u(\mathbf {x} )=c
(\mathbf {x} ,u)}], and we do not yet know that     U ( s ) = u (  X  ( s ) )
{\displaystyle U(s)=u(\mathbf {X} (s))}  [{\displaystyle U(s)=u(\mathbf {X}
(s))}].
However, we can see that
    &#x0394; &#x2032;  ( s ) = 2   (   u (  X  ( s ) ) &#x2212; U ( s )   )
(    a  (  X  ( s ) , U ( s ) ) &#x22C5; &#x2207; u (  X  ( s ) ) &#x2212; c
(  X  ( s ) , U ( s ) ) &#x2212;   (    a  (  X  ( s ) , u (  X  ( s ) ) )
&#x22C5; &#x2207; u (  X  ( s ) ) &#x2212; c (  X  ( s ) , u (  X  ( s ) ) )
)     )     {\displaystyle \Delta '(s)=2{\big (}u(\mathbf {X} (s))-U(s){\big )}
{\Big (}\mathbf {a} (\mathbf {X} (s),U(s))\cdot \nabla u(\mathbf {X} (s))-c
(\mathbf {X} (s),U(s))-{\big (}\mathbf {a} (\mathbf {X} (s),u(\mathbf {X}
(s)))\cdot \nabla u(\mathbf {X} (s))-c(\mathbf {X} (s),u(\mathbf {X} (s))){\big
)}{\Big )}}  [{\displaystyle \Delta '(s)=2{\big (}u(\mathbf {X} (s))-U(s){\big
)}{\Big (}\mathbf {a} (\mathbf {X} (s),U(s))\cdot \nabla u(\mathbf {X} (s))-c
(\mathbf {X} (s),U(s))-{\big (}\mathbf {a} (\mathbf {X} (s),u(\mathbf {X}
(s)))\cdot \nabla u(\mathbf {X} (s))-c(\mathbf {X} (s),u(\mathbf {X} (s))){\big
)}{\Big )}}]
since by the PDE, the last term is 0. This equals
    &#x0394; &#x2032;  ( s ) = 2   (   u (  X  ( s ) ) &#x2212; U ( s )   )
(     (    a  (  X  ( s ) , U ( s ) ) &#x2212;  a  (  X  ( s ) , u (  X  ( s )
) )   )   &#x22C5; &#x2207; u (  X  ( s ) ) &#x2212;   (   c (  X  ( s ) , U
( s ) ) &#x2212; c (  X  ( s ) , u (  X  ( s ) ) )   )     )     {\displaystyle
\Delta '(s)=2{\big (}u(\mathbf {X} (s))-U(s){\big )}{\Big (}{\big (}\mathbf {a}
(\mathbf {X} (s),U(s))-\mathbf {a} (\mathbf {X} (s),u(\mathbf {X} (s))){\big
)}\cdot \nabla u(\mathbf {X} (s))-{\big (}c(\mathbf {X} (s),U(s))-c(\mathbf {X}
(s),u(\mathbf {X} (s))){\big )}{\Big )}}  [{\displaystyle \Delta '(s)=2{\big
(}u(\mathbf {X} (s))-U(s){\big )}{\Big (}{\big (}\mathbf {a} (\mathbf {X} (s),U
(s))-\mathbf {a} (\mathbf {X} (s),u(\mathbf {X} (s))){\big )}\cdot \nabla u
(\mathbf {X} (s))-{\big (}c(\mathbf {X} (s),U(s))-c(\mathbf {X} (s),u(\mathbf
{X} (s))){\big )}{\Big )}}]
By the triangle inequality, we have
    |   &#x0394; &#x2032;  ( s )  |  = 2   |   u (  X  ( s ) ) &#x2212; U ( s )
|     (     &#x2016;    a  (  X  ( s ) , U ( s ) ) &#x2212;  a  (  X  ( s ) , u
(  X  ( s ) ) )   &#x2016;   &#xA0; &#x2016; &#x2207; u (  X  ( s ) ) &#x2016;
+   |   c (  X  ( s ) , U ( s ) ) &#x2212; c (  X  ( s ) , u (  X  ( s ) ) )
|     )     {\displaystyle |\Delta '(s)|=2{\big |}u(\mathbf {X} (s))-U(s){\big
|}{\Big (}{\big \|}\mathbf {a} (\mathbf {X} (s),U(s))-\mathbf {a} (\mathbf {X}
(s),u(\mathbf {X} (s))){\big \|}\ \|\nabla u(\mathbf {X} (s))\|+{\big |}c
(\mathbf {X} (s),U(s))-c(\mathbf {X} (s),u(\mathbf {X} (s))){\big |}{\Big )}}
[{\displaystyle |\Delta '(s)|=2{\big |}u(\mathbf {X} (s))-U(s){\big |}{\Big (}
{\big \|}\mathbf {a} (\mathbf {X} (s),U(s))-\mathbf {a} (\mathbf {X} (s),u
(\mathbf {X} (s))){\big \|}\ \|\nabla u(\mathbf {X} (s))\|+{\big |}c(\mathbf
{X} (s),U(s))-c(\mathbf {X} (s),u(\mathbf {X} (s))){\big |}{\Big )}}]
Assuming      a  , c   {\displaystyle \mathbf {a} ,c}  [{\displaystyle \mathbf
{a} ,c}] are at least      C  1     {\displaystyle C^{1}}  [{\displaystyle C^
{1}}], we can bound this for small times. Choose a neighborhood     &#x03A9;
{\displaystyle \Omega }  [{\displaystyle \Omega }] around      X  ( 0 ) , U ( 0
)   {\displaystyle \mathbf {X} (0),U(0)}  [{\displaystyle \mathbf {X} (0),U
(0)}] small enough such that      a  , c   {\displaystyle \mathbf {a} ,c}  [
{\displaystyle \mathbf {a} ,c}] are Locally_Lipschitz. By continuity,     (  X
( s ) , U ( s ) )   {\displaystyle (\mathbf {X} (s),U(s))}  [{\displaystyle
(\mathbf {X} (s),U(s))}] will remain in     &#x03A9;   {\displaystyle \Omega }
[{\displaystyle \Omega }] for small enough     s   {\displaystyle s}  [
{\displaystyle s}]. Since     U ( 0 ) = u (  X  ( 0 ) )   {\displaystyle U(0)=u
(\mathbf {X} (0))}  [{\displaystyle U(0)=u(\mathbf {X} (0))}], we also have
that     (  X  ( s ) , u (  X  ( s ) ) )   {\displaystyle (\mathbf {X} (s),u
(\mathbf {X} (s)))}  [{\displaystyle (\mathbf {X} (s),u(\mathbf {X} (s)))}]
will be in     &#x03A9;   {\displaystyle \Omega }  [{\displaystyle \Omega }]
for small enough     s   {\displaystyle s}  [{\displaystyle s}] by continuity.
So,     (  X  ( s ) , U ( s ) ) &#x2208; &#x03A9;   {\displaystyle (\mathbf {X}
(s),U(s))\in \Omega }  [{\displaystyle (\mathbf {X} (s),U(s))\in \Omega }] and
(  X  ( s ) , u (  X  ( s ) ) ) &#x2208; &#x03A9;   {\displaystyle (\mathbf {X}
(s),u(\mathbf {X} (s)))\in \Omega }  [{\displaystyle (\mathbf {X} (s),u(\mathbf
{X} (s)))\in \Omega }] for     s &#x2208; [ 0 ,  s  0   ]   {\displaystyle s\in
[0,s_{0}]}  [{\displaystyle s\in [0,s_{0}]}]. Additionally,     &#x2016;
&#x2207; u (  X  ( s ) ) &#x2016; &#x2264; M   {\displaystyle \|\nabla u
(\mathbf {X} (s))\|\leq M}  [{\displaystyle \|\nabla u(\mathbf {X} (s))\|\leq
M}] for some     M &#x2208;  R    {\displaystyle M\in \mathbb {R} }  [
{\displaystyle M\in \mathbb {R} }] for     s &#x2208; [ 0 ,  s  0   ]
{\displaystyle s\in [0,s_{0}]}  [{\displaystyle s\in [0,s_{0}]}] by
compactness. From this, we find the above is bounded as
    |   &#x0394; &#x2032;  ( s )  |  &#x2264; C  |  u (  X  ( s ) ) &#x2212; U
( s )   |   2   = C  |  &#x0394; ( s )  |    {\displaystyle |\Delta '(s)|\leq
C|u(\mathbf {X} (s))-U(s)|^{2}=C|\Delta (s)|}  [{\displaystyle |\Delta '
(s)|\leq C|u(\mathbf {X} (s))-U(s)|^{2}=C|\Delta (s)|}]
for some     C &#x2208;  R    {\displaystyle C\in \mathbb {R} }  [
{\displaystyle C\in \mathbb {R} }]. It is a straightforward application of
GrÃ¶nwall's Inequality to show that since     &#x0394; ( 0 ) = 0
{\displaystyle \Delta (0)=0}  [{\displaystyle \Delta (0)=0}] we have
&#x0394; ( s ) = 0   {\displaystyle \Delta (s)=0}  [{\displaystyle \Delta
(s)=0}] for as long as this inequality holds. We have some interval     [ 0 ,
&#x03F5; )   {\displaystyle [0,\epsilon )}  [{\displaystyle [0,\epsilon )}]
such that     u ( X ( s ) ) = U ( s )   {\displaystyle u(X(s))=U(s)}  [
{\displaystyle u(X(s))=U(s)}] in this interval. Choose the largest     &#x03F5;
{\displaystyle \epsilon }  [\epsilon ] such that this is true. Then, by
continuity,     U ( &#x03F5; ) = u (  X  ( &#x03F5; ) )   {\displaystyle U
(\epsilon )=u(\mathbf {X} (\epsilon ))}  [{\displaystyle U(\epsilon )=u(\mathbf
{X} (\epsilon ))}]. Provided the ODE still has a solution in some interval
after     &#x03F5;   {\displaystyle \epsilon }  [\epsilon ], we can repeat the
argument above to find that     u ( X ( s ) ) = U ( s )   {\displaystyle u(X
(s))=U(s)}  [{\displaystyle u(X(s))=U(s)}] in a larger interval. Thus, so long
as the ODE has a solution, we have     u ( X ( s ) ) = U ( s )   {\displaystyle
u(X(s))=U(s)}  [{\displaystyle u(X(s))=U(s)}].
**** Fully nonlinear case[edit] ****
Consider the partial differential equation
         F (  x  1   , &#x2026; ,  x  n   , u ,  p  1   , &#x2026; ,
      p  n   ) = 0   {\displaystyle F(x_{1},\dots ,x_{n},u,p_           (4)
      {1},\dots ,p_{n})=0}  [F(x_{1},\dots ,x_{n},u,p_{1},\dots ,p_     
      {n})=0]
where the variables pi are shorthand for the partial derivatives
          p  i   =    &#x2202; u   &#x2202;  x  i      .   {\displaystyle p_
      {i}={\frac {\partial u}{\partial x_{i}}}.}  [p_{i}={\frac {\partial u}
      {\partial x_{i}}}.]
Let (xi(s),u(s),pi(s)) be a curve in R2n+1. Suppose that u is any solution, and
that
         u ( s ) = u (  x  1   ( s ) , &#x2026; ,  x  n   ( s ) ) .
      {\displaystyle u(s)=u(x_{1}(s),\dots ,x_{n}(s)).}  [u(s)=u(x_{1}(s),\dots
      ,x_{n}(s)).]
Along a solution, differentiating (4) with respect to s gives
          &#x2211;  i   (  F   x  i     +  F  u    p  i   )     x &#x02D9;
      i   +  &#x2211;  i    F   p  i         p &#x02D9;     i   = 0
      {\displaystyle \sum _{i}(F_{x_{i}}+F_{u}p_{i}){\dot {x}}_{i}+\sum _{i}F_
      {p_{i}}{\dot {p}}_{i}=0}  [\sum _{i}(F_{x_{i}}+F_{u}p_{i}){\dot {x}}_
      {i}+\sum _{i}F_{p_{i}}{\dot {p}}_{i}=0]
            u &#x02D9;    &#x2212;  &#x2211;  i    p  i       x &#x02D9;     i
      = 0   {\displaystyle {\dot {u}}-\sum _{i}p_{i}{\dot {x}}_{i}=0}  [{\dot
      {u}}-\sum _{i}p_{i}{\dot {x}}_{i}=0]
          &#x2211;  i   (     x &#x02D9;     i   d  p  i   &#x2212;     p
      &#x02D9;     i   d  x  i   ) = 0.   {\displaystyle \sum _{i}({\dot {x}}_
      {i}dp_{i}-{\dot {p}}_{i}dx_{i})=0.}  [\sum _{i}({\dot {x}}_{i}dp_{i}-
      {\dot {p}}_{i}dx_{i})=0.]
The second equation follows from applying the chain_rule to a solution u, and
the third follows by taking an exterior_derivative of the relation     d u
&#x2212;  &#x2211;  i    p  i    d  x  i   = 0   {\displaystyle du-\sum _{i}p_
{i}\,dx_{i}=0}  [du-\sum _{i}p_{i}\,dx_{i}=0]. Manipulating these equations
gives
             x &#x02D9;     i   = &#x03BB;  F   p  i     ,      p &#x02D9;
      i   = &#x2212; &#x03BB; (  F   x  i     +  F  u    p  i   ) ,     u
      &#x02D9;    = &#x03BB;  &#x2211;  i    p  i    F   p  i
      {\displaystyle {\dot {x}}_{i}=\lambda F_{p_{i}},\quad {\dot {p}}_{i}=-
      \lambda (F_{x_{i}}+F_{u}p_{i}),\quad {\dot {u}}=\lambda \sum _{i}p_{i}F_
      {p_{i}}}  [{\dot {x}}_{i}=\lambda F_{p_{i}},\quad {\dot {p}}_{i}=-\lambda
      (F_{x_{i}}+F_{u}p_{i}),\quad {\dot {u}}=\lambda \sum _{i}p_{i}F_{p_{i}}]
where Î» is a constant. Writing these equations more symmetrically, one obtains
the Lagrange-Charpit equations for the characteristic
               x &#x02D9;     i    F   p  i       = &#x2212;       p &#x02D9;
      i     F   x  i     +  F  u    p  i      =     u &#x02D9;    &#x2211;  p
      i    F   p  i        .   {\displaystyle {\frac {{\dot {x}}_{i}}{F_{p_
      {i}}}}=-{\frac {{\dot {p}}_{i}}{F_{x_{i}}+F_{u}p_{i}}}={\frac {\dot {u}}
      {\sum p_{i}F_{p_{i}}}}.}  [{\frac {{\dot {x}}_{i}}{F_{p_{i}}}}=-{\frac {
      {\dot {p}}_{i}}{F_{x_{i}}+F_{u}p_{i}}}={\frac {\dot {u}}{\sum p_{i}F_{p_
      {i}}}}.]
Geometrically, the method of characteristics in the fully nonlinear case can be
interpreted as requiring that the Monge_cone of the differential equation
should everywhere be tangent to the graph of the solution.
For a pedagogical way of deriving the Lagrange-Charpit equations see the
chapter 4 at [1].
***** Example[edit] *****
As an example, consider the advection_equation (this example assumes
familiarity with PDE notation, and solutions to basic ODEs).
         a    &#x2202; u   &#x2202; x    +    &#x2202; u   &#x2202; t    = 0
      {\displaystyle a{\frac {\partial u}{\partial x}}+{\frac {\partial u}
      {\partial t}}=0\,}  [a{\frac {\partial u}{\partial x}}+{\frac {\partial
      u}{\partial t}}=0\,]
where     a    {\displaystyle a\,}  [a\,] is constant and     u
{\displaystyle u\,}  [u\,] is a function of     x    {\displaystyle x\,}  [x\,]
and     t    {\displaystyle t\,}  [t\,]. We want to transform this linear
first-order PDE into an ODE along the appropriate curve; i.e. something of the
form
           d  d s    u ( x ( s ) , t ( s ) ) = F ( u , x ( s ) , t ( s ) )
      {\displaystyle {\frac {d}{ds}}u(x(s),t(s))=F(u,x(s),t(s))}  [{\frac {d}
      {ds}}u(x(s),t(s))=F(u,x(s),t(s))],
where     ( x ( s ) , t ( s ) )    {\displaystyle (x(s),t(s))\,}  [(x(s),t
(s))\,] is a characteristic line. First, we find
           d  d s    u ( x ( s ) , t ( s ) ) =    &#x2202; u   &#x2202; x
      d x   d s    +    &#x2202; u   &#x2202; t       d t   d s
      {\displaystyle {\frac {d}{ds}}u(x(s),t(s))={\frac {\partial u}{\partial
      x}}{\frac {dx}{ds}}+{\frac {\partial u}{\partial t}}{\frac {dt}{ds}}}  [
      {\frac {d}{ds}}u(x(s),t(s))={\frac {\partial u}{\partial x}}{\frac {dx}
      {ds}}+{\frac {\partial u}{\partial t}}{\frac {dt}{ds}}]
by the chain rule. Now, if we set        d x   d s    = a   {\displaystyle
{\frac {dx}{ds}}=a}  [{\frac {dx}{ds}}=a] and        d t   d s    = 1
{\displaystyle {\frac {dt}{ds}}=1}  [{\frac {dt}{ds}}=1] we get
         a    &#x2202; u   &#x2202; x    +    &#x2202; u   &#x2202; t
      {\displaystyle a{\frac {\partial u}{\partial x}}+{\frac {\partial u}
      {\partial t}}\,}  [a{\frac {\partial u}{\partial x}}+{\frac {\partial u}
      {\partial t}}\,]
which is the left hand side of the PDE we started with. Thus
           d  d s    u = a    &#x2202; u   &#x2202; x    +    &#x2202; u
      &#x2202; t    = 0.   {\displaystyle {\frac {d}{ds}}u=a{\frac {\partial u}
      {\partial x}}+{\frac {\partial u}{\partial t}}=0.}  [{\frac {d}{ds}}u=a
      {\frac {\partial u}{\partial x}}+{\frac {\partial u}{\partial t}}=0.]
So, along the characteristic line     ( x ( s ) , t ( s ) )    {\displaystyle
(x(s),t(s))\,}  [(x(s),t(s))\,], the original PDE becomes the ODE      u  s   =
F ( u , x ( s ) , t ( s ) ) = 0    {\displaystyle u_{s}=F(u,x(s),t(s))=0\,}
[u_{s}=F(u,x(s),t(s))=0\,]. That is to say that along the characteristics, the
solution is constant. Thus,     u (  x  s   ,  t  s   ) = u (  x  0   , 0 )
{\displaystyle u(x_{s},t_{s})=u(x_{0},0)\,}  [u(x_{s},t_{s})=u(x_{0},0)\,]
where     (  x  s   ,  t  s   )    {\displaystyle (x_{s},t_{s})\,}  [(x_{s},t_
{s})\,] and     (  x  0   , 0 )    {\displaystyle (x_{0},0)\,}  [(x_{0},0)\,]
lie on the same characteristic. Therefore, to determine the general solution,
it is enough to find the characteristics by solving the characteristic system
of ODEs:
    *       d t   d s    = 1   {\displaystyle {\frac {dt}{ds}}=1}  [{\frac {dt}
      {ds}}=1], letting     t ( 0 ) = 0    {\displaystyle t(0)=0\,}  [t(0)=0\,]
      we know     t = s    {\displaystyle t=s\,}  [t=s\,],
    *       d x   d s    = a   {\displaystyle {\frac {dx}{ds}}=a}  [{\frac {dx}
      {ds}}=a], letting     x ( 0 ) =  x  0      {\displaystyle x(0)=x_{0}\,}
      [x(0)=x_{0}\,] we know     x = a s +  x  0   = a t +  x  0
      {\displaystyle x=as+x_{0}=at+x_{0}\,}  [x=as+x_{0}=at+x_{0}\,],
    *       d u   d s    = 0   {\displaystyle {\frac {du}{ds}}=0}  [{\frac {du}
      {ds}}=0], letting     u ( 0 ) = f (  x  0   )    {\displaystyle u(0)=f(x_
      {0})\,}  [u(0)=f(x_{0})\,] we know     u ( x ( t ) , t ) = f (  x  0   )
      = f ( x &#x2212; a t )    {\displaystyle u(x(t),t)=f(x_{0})=f(x-at)\,}
      [u(x(t),t)=f(x_{0})=f(x-at)\,].
In this case, the characteristic lines are straight lines with slope     a
{\displaystyle a\,}  [a\,], and the value of     u    {\displaystyle u\,}
[u\,] remains constant along any characteristic line.
***** Characteristics of linear differential operators[edit] *****
Let X be a differentiable_manifold and P a linear differential_operator
         P :  C  &#x221E;   ( X ) &#x2192;  C  &#x221E;   ( X )
      {\displaystyle P:C^{\infty }(X)\to C^{\infty }(X)}  [P:C^{\infty }(X)\to
      C^{\infty }(X)]
of order k. In a local coordinate system xi,
         P =  &#x2211;   |  &#x03B1;  |  &#x2264; k    P  &#x03B1;   ( x )
      &#x2202;  &#x2202;  x  &#x03B1;        {\displaystyle P=\sum _{|\alpha
      |\leq k}P^{\alpha }(x){\frac {\partial }{\partial x^{\alpha }}}}  [P=\sum
      _{|\alpha |\leq k}P^{\alpha }(x){\frac {\partial }{\partial x^{\alpha
      }}}]
in which Î± denotes a multi-index. The principal symbol of P, denoted ÏP, is
the function on the cotangent_bundle TâX defined in these local coordinates
by
          &#x03C3;  P   ( x , &#x03BE; ) =  &#x2211;   |  &#x03B1;  |  = k    P
      &#x03B1;   ( x )  &#x03BE;  &#x03B1;     {\displaystyle \sigma _{P}(x,\xi
      )=\sum _{|\alpha |=k}P^{\alpha }(x)\xi _{\alpha }}  [\sigma _{P}(x,\xi
      )=\sum _{|\alpha |=k}P^{\alpha }(x)\xi _{\alpha }]
where the Î¾i are the fiber coordinates on the cotangent bundle induced by the
coordinate differentials dxi. Although this is defined using a particular
coordinate system, the transformation law relating the Î¾i and the xi ensures
that ÏP is a well-defined function on the cotangent bundle.
The function ÏP is homogeneous of degree k in the Î¾ variable. The zeros of
ÏP, away from the zero section of TâX, are the characteristics of P. A
hypersurface of X defined by the equation F(x) = c is called a characteristic
hypersurface at x if
          &#x03C3;  P   ( x , d F ( x ) ) = 0.   {\displaystyle \sigma _{P}
      (x,dF(x))=0.}  [\sigma _{P}(x,dF(x))=0.]
Invariantly, a characteristic hypersurface is a hypersurface whose conormal
bundle is in the characteristic set of P.
***** Qualitative analysis of characteristics[edit] *****
Characteristics are also a powerful tool for gaining qualitative insight into a
PDE.
One can use the crossings of the characteristics to find shock_waves for
potential flow in a compressible fluid. Intuitively, we can think of each
characteristic line implying a solution to     u    {\displaystyle u\,}  [u\,]
along itself. Thus, when two characteristics cross, the function becomes multi-
valued resulting in a non-physical solution. Physically, this contradiction is
removed by the formation of a shock wave, a tangential discontinuity or a weak
discontinuity and can result in non-potential flow, violating the initial
assumptions.
Characteristics may fail to cover part of the domain of the PDE. This is called
a rarefaction, and indicates the solution typically exists only in a weak, i.e.
integral_equation, sense.
The direction of the characteristic lines indicate the flow of values through
the solution, as the example above demonstrates. This kind of knowledge is
useful when solving PDEs numerically as it can indicate which finite_difference
scheme is best for the problem.
***** See also[edit] *****
    * Method_of_quantum_characteristics
***** Notes[edit] *****
   1. ^ John_1991
   2. ^ a b Delgado_1997
***** References[edit] *****
    * Courant,_Richard; Hilbert,_David (1962), Methods of Mathematical Physics,
      Volume II, Wiley-Interscience
Delgado, Manuel (1997), "The Lagrange-Charpit Method", SIAM Review, 39 (2):
298â304, Bibcode:1997SIAMR..39..298D, doi:10.1137/S0036144595293534,
JSTOR 2133111
Evans,_Lawrence_C. (1998), Partial Differential Equations, Providence: American
Mathematical Society, ISBN 0-8218-0772-2
John,_Fritz (1991), Partial differential equations (4th ed.), Springer,
ISBN 978-0-387-90609-6
Polyanin, A. D.; Zaitsev, V. F.; Moussiaux, A. (2002), Handbook of First Order
Partial Differential Equations, London: Taylor & Francis, ISBN 0-415-27267-X
Polyanin, A. D. (2002), Handbook of Linear Partial Differential Equations for
Engineers and Scientists, Boca Raton: Chapman & Hall/CRC Press, ISBN 1-58488-
299-9
Sarra, Scott (2003), "The_Method_of_Characteristics_with_applications_to
Conservation_Laws", Journal of Online Mathematics and its Applications
.
Streeter, VL; Wylie, EB (1998), Fluid mechanics (International 9th Revised
ed.), McGraw-Hill Higher Education
***** External links[edit] *****
    * Prof._Scott_Sarra_tutorial_on_Method_of_Characteristics
    * Prof._Alan_Hood_tutorial_on_Method_of_Characteristics
    * v
    * t
    * e
Numerical_partial_differential_equations by method
                     Parabolic      * Forward-time_central-space (FTCS)
                                    * CrankâNicolson
                                    * LaxâFriedrichs
                                    * LaxâWendroff
Finite_difference    Hyperbolic     * MacCormack
                                    * Upwind
                                    * Method of characteristics
                     Others         * Alternating_direction-implicit (ADI)
                                    * Finite-difference_time-domain (FDTD)
                         * Godunov
                         * High-resolution
                         * Monotonic_upstream-centered (MUSCL)
Finite_volume            * Advection_upstream-splitting (AUSM)
                         * Riemann_solver
                         * essentially_non-oscillatory (ENO)
                         * weighted_essentially_non-oscillatory (WENO)
                         * hp-FEM
                         * Extended (XFEM)
                         * Discontinuous_Galerkin (DG)
Finite_element           * Spectral_element (SEM)
                         * Mortar
                         * Gradient_discretisation (GDM)
                         * Loubignac_iteration
                         * Smoothed (S-FEM)
                         * Smoothed-particle_hydrodynamics (SPH)
Meshless/Meshfree        * Moving_particle_semi-implicit_method (MPS)
                         * Material_point_method (MPM)
                         * Particle-in-cell (PIC)
                         * Schur_complement
                         * Fictitious_domain
                         * Schwarz_alternating
                               o additive
                               o abstract_additive
Domain_decomposition     * NeumannâDirichlet
                         * NeumannâNeumann
                         * PoincarÃ©âSteklov_operator
                         * Balancing (BDD)
                         * Balancing_by_constraints (BDDC)
                         * Tearing_and_interconnect (FETI)
                         * FETI-DP
                         * Spectral
                         * Pseudospectral (DVR)
                         * Method_of_lines
                         * Multigrid
                         * Collocation
                         * Level-set
                         * Boundary_element
Others                   * Immersed_boundary
                         * Analytic_element
                         * Particle-in-cell
                         * Isogeometric_analysis
                         * Infinite_difference_method
                         * Infinite_element_method
                         * Galerkin_method
                               o PetrovâGalerkin_method

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Method_of_characteristics&oldid=871498227"
Categories:
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
    * Deutsch
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * Nederlands
    * æ¥æ¬èª
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 1 December 2018, at 13:53 (UTC).
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
