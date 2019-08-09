The following text has been accessed from https://en.wikipedia.org/wiki/Dynamic_programming at Fri Aug 9 03:46:41 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Dynamic programming ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with dynamic_programming_language or dynamic_problem.
Figure 1. Finding the shortest path in a graph using optimal substructure; a
straight line indicates a single edge; a wavy line indicates a shortest path
between the two vertices it connects (among other paths, not shown, sharing the
same two vertices); the bold line is the overall shortest path from start to
goal.
Dynamic programming is both a mathematical_optimization method and a computer
programming method. The method was developed by Richard_Bellman in the 1950s
and has found applications in numerous fields, from aerospace_engineering to
economics. In both contexts it refers to simplifying a complicated problem by
breaking it down into simpler sub-problems in a recursive manner. While some
decision problems cannot be taken apart this way, decisions that span several
points in time do often break apart recursively. Likewise, in computer science,
if a problem can be solved optimally by breaking it into sub-problems and then
recursively finding the optimal solutions to the sub-problems, then it is said
to have optimal_substructure.
If sub-problems can be nested recursively inside larger problems, so that
dynamic programming methods are applicable, then there is a relation between
the value of the larger problem and the values of the sub-problems.[1] In the
optimization literature this relationship is called the Bellman_equation.
⁰
***** Contents *****
    * 1_Overview
          o 1.1_Mathematical_optimization
          o 1.2_Control_theory
                # 1.2.1_Example_from_economics:_Ramsey's_problem_of_optimal
                  saving
          o 1.3_Computer_programming
          o 1.4_Bioinformatics
    * 2_Examples:_Computer_algorithms
          o 2.1_Dijkstra's_algorithm_for_the_shortest_path_problem
          o 2.2_Fibonacci_sequence
          o 2.3_A_type_of_balanced_0â1_matrix
          o 2.4_Checkerboard
          o 2.5_Sequence_alignment
          o 2.6_Tower_of_Hanoi_puzzle
          o 2.7_Egg_dropping_puzzle
                # 2.7.1_Faster_DP_solution_using_a_different_parametrization
          o 2.8_Matrix_chain_multiplication
    * 3_History
    * 4_Algorithms_that_use_dynamic_programming
    * 5_See_also
    * 6_References
    * 7_Further_reading
    * 8_External_links
***** Overview[edit] *****
**** Mathematical optimization[edit] ****
In terms of mathematical optimization, dynamic programming usually refers to
simplifying a decision by breaking it down into a sequence of decision steps
over time. This is done by defining a sequence of value functions V1, V2, ...,
Vn taking y as an argument representing the state of the system at times i from
1 to n. The definition of Vn(y) is the value obtained in state y at the last
time n. The values Vi at earlier times i = n −1, n − 2, ..., 2, 1 can be found
by working backwards, using a recursive relationship called the Bellman
equation. For i = 2, ..., n, Vi−1 at any state y is calculated from Vi by
maximizing a simple function (usually the sum) of the gain from a decision at
time i − 1 and the function Vi at the new state of the system if this decision
is made. Since Vi has already been calculated for the needed states, the above
operation yields Vi−1 for those states. Finally, V1 at the initial state of the
system is the value of the optimal solution. The optimal values of the decision
variables can be recovered, one by one, by tracking back the calculations
already performed.
**** Control theory[edit] ****
In control_theory, a typical problem is to find an admissible control       u
&#x2217;     {\displaystyle \mathbf {u} ^{\ast }}  [{\displaystyle \mathbf {u}
^{\ast }}] which causes the system         x  &#x02D9;    ( t ) =  g   (   x
( t ) ,  u  ( t ) , t  )    {\displaystyle {\dot {\mathbf {x} }}(t)=\mathbf {g}
\left(\mathbf {x} (t),\mathbf {u} (t),t\right)}  [{\displaystyle {\dot {\mathbf
{x} }}(t)=\mathbf {g} \left(\mathbf {x} (t),\mathbf {u} (t),t\right)}] to
follow an admissible trajectory       x   &#x2217;     {\displaystyle \mathbf
{x} ^{\ast }}  [{\displaystyle \mathbf {x} ^{\ast }}] on a continuous time
interval      t  0   &#x2264; t &#x2264;  t  1     {\displaystyle t_{0}\leq
t\leq t_{1}}  [{\displaystyle t_{0}\leq t\leq t_{1}}] that minimizes a cost
function
         J = b  (   x  (  t  1   ) ,  t  1    )  +  &#x222B;   t  0      t  1
      f  (   x  ( t ) ,  u  ( t ) , t  )   d  t   {\displaystyle J=b\left
      (\mathbf {x} (t_{1}),t_{1}\right)+\int _{t_{0}}^{t_{1}}f\left(\mathbf {x}
      (t),\mathbf {u} (t),t\right)\mathrm {d} t}  [{\displaystyle J=b\left
      (\mathbf {x} (t_{1}),t_{1}\right)+\int _{t_{0}}^{t_{1}}f\left(\mathbf {x}
      (t),\mathbf {u} (t),t\right)\mathrm {d} t}]
The solution to this problem is an optimal control law or policy       u
&#x2217;   = h (  x  ( t ) , t )   {\displaystyle \mathbf {u} ^{\ast }=h
(\mathbf {x} (t),t)}  [{\displaystyle \mathbf {u} ^{\ast }=h(\mathbf {x}
(t),t)}], which produces an optimal trajectory       x   &#x2217;
{\displaystyle \mathbf {x} ^{\ast }}  [{\displaystyle \mathbf {x} ^{\ast }}]
and an optimized loss function      J  &#x2217;     {\displaystyle J^{\ast }}
[{\displaystyle J^{\ast }}]. The latter obeys the fundamental equation of
dynamic programming:
         &#x2212;  J  t   &#x2217;   =  min   u     {  f  (   x  ( t ) ,  u
      ( t ) , t  )  +  J  x   &#x2217;   T      g   (   x  ( t ) ,  u  ( t ) ,
      t  )   }    {\displaystyle -J_{t}^{\ast }=\min _{\mathbf {u} }\left\
      {f\left(\mathbf {x} (t),\mathbf {u} (t),t\right)+J_{x}^{\ast {\mathsf
      {T}}}\mathbf {g} \left(\mathbf {x} (t),\mathbf {u} (t),t\right)\right\}}
      [{\displaystyle -J_{t}^{\ast }=\min _{\mathbf {u} }\left\{f\left(\mathbf
      {x} (t),\mathbf {u} (t),t\right)+J_{x}^{\ast {\mathsf {T}}}\mathbf {g}
      \left(\mathbf {x} (t),\mathbf {u} (t),t\right)\right\}}]
a partial_differential_equation known as the HamiltonâJacobiâBellman
equation, in which      J  x   &#x2217;   =    &#x2202;  J  &#x2217;
&#x2202;  x     =   [     &#x2202;  J  &#x2217;     &#x2202;  x  1      &#xA0;
&#xA0; &#xA0; &#xA0;    &#x2202;  J  &#x2217;     &#x2202;  x  2      &#xA0;
&#xA0; &#xA0; &#xA0; &#x2026; &#xA0; &#xA0; &#xA0; &#xA0;    &#x2202;  J
&#x2217;     &#x2202;  x  n       ]    T      {\displaystyle J_{x}^{\ast }=
{\frac {\partial J^{\ast }}{\partial \mathbf {x} }}=\left[{\frac {\partial J^
{\ast }}{\partial x_{1}}}~~~~{\frac {\partial J^{\ast }}{\partial x_
{2}}}~~~~\dots ~~~~{\frac {\partial J^{\ast }}{\partial x_{n}}}\right]^{\mathsf
{T}}}  [{\displaystyle J_{x}^{\ast }={\frac {\partial J^{\ast }}{\partial
\mathbf {x} }}=\left[{\frac {\partial J^{\ast }}{\partial x_{1}}}~~~~{\frac
{\partial J^{\ast }}{\partial x_{2}}}~~~~\dots ~~~~{\frac {\partial J^{\ast }}
{\partial x_{n}}}\right]^{\mathsf {T}}}] and      J  t   &#x2217;   =
&#x2202;  J  &#x2217;     &#x2202; t      {\displaystyle J_{t}^{\ast }={\frac
{\partial J^{\ast }}{\partial t}}}  [{\displaystyle J_{t}^{\ast }={\frac
{\partial J^{\ast }}{\partial t}}}]. One finds the minimizing      u
{\displaystyle \mathbf {u} }  [\mathbf {u} ] in terms of     t   {\displaystyle
t}  [t],      x    {\displaystyle \mathbf {x} }  [\mathbf {x} ], and the
unknown function      J  x   &#x2217;     {\displaystyle J_{x}^{\ast }}  [
{\displaystyle J_{x}^{\ast }}] and then substitutes the result into the
HamiltonâJacobiâBellman equation to get the partial differential equation
to be solved with boundary condition     J  (  t  1   )  = b  (   x  (  t  1
) ,  t  1    )    {\displaystyle J\left(t_{1}\right)=b\left(\mathbf {x} (t_
{1}),t_{1}\right)}  [{\displaystyle J\left(t_{1}\right)=b\left(\mathbf {x} (t_
{1}),t_{1}\right)}].[2] In practice, this generally requires numerical
techniques for some discrete approximation to the exact optimization
relationship.
Alternatively, the continuous process can be approximated by a discrete system,
which leads to a following recurrence relation analog to the
HamiltonâJacobiâBellman equation:
          J  k   &#x2217;    (   x   n &#x2212; k   )  =  min    u   n &#x2212;
      k      {     f &#x005E;     (    x   n &#x2212; k   ,   u   n &#x2212; k
      )  +  J  k &#x2212; 1   &#x2217;    (     g &#x005E;     (    x   n
      &#x2212; k   ,   u   n &#x2212; k    )   )   }    {\displaystyle J_{k}^
      {\ast }\left(\mathbf {x} _{n-k}\right)=\min _{\mathbf {u} _{n-k}}\left\{
      {\hat {f}}\left(\mathbf {x} _{n-k},\mathbf {u} _{n-k}\right)+J_{k-1}^
      {\ast }\left({\hat {g}}\left(\mathbf {x} _{n-k},\mathbf {u} _{n-
      k}\right)\right)\right\}}  [{\displaystyle J_{k}^{\ast }\left(\mathbf {x}
      _{n-k}\right)=\min _{\mathbf {u} _{n-k}}\left\{{\hat {f}}\left(\mathbf
      {x} _{n-k},\mathbf {u} _{n-k}\right)+J_{k-1}^{\ast }\left({\hat {g}}\left
      (\mathbf {x} _{n-k},\mathbf {u} _{n-k}\right)\right)\right\}}]
at the     k   {\displaystyle k}  [k]-th stage of     n   {\displaystyle n}
[n] equally spaced discrete time intervals, and where        f &#x005E;
{\displaystyle {\hat {f}}}  [{\hat {f}}] and        g &#x005E;
{\displaystyle {\hat {g}}}  [{\hat {g}}] denote discrete approximations to
f   {\displaystyle f}  [f] and      g    {\displaystyle \mathbf {g} }  [\mathbf
{g} ]. This functional equation is known as the Bellman_equation, which can be
solved for an exact solution of the discrete approximation of the optimization
equation.[3]
*** Example from economics: Ramsey's problem of optimal saving[edit] ***
See also: RamseyâCassâKoopmans_model
In economics, the objective is generally to maximize (rather than minimize)
some dynamic social_welfare_function. In Ramsey's problem, this function
relates amounts of consumption to levels of utility. Loosely speaking, the
planner faces the trade-off between contemporaneous consumption and future
consumption (via investment in capital_stock that is used in production), known
as intertemporal_choice. Future consumption is discounted at a constant rate
&#x03B2; &#x2208; ( 0 , 1 )   {\displaystyle \beta \in (0,1)}  [{\displaystyle
\beta \in (0,1)}]. A discrete approximation to the transition equation of
capital is given by
          k  t + 1   =    g &#x005E;     (   k  t   ,  c  t    )  = f (  k  t
      ) &#x2212;  c  t     {\displaystyle k_{t+1}={\hat {g}}\left(k_{t},c_
      {t}\right)=f(k_{t})-c_{t}}  [{\displaystyle k_{t+1}={\hat {g}}\left(k_
      {t},c_{t}\right)=f(k_{t})-c_{t}}]
where     c   {\displaystyle c}  [c] is consumption,     k   {\displaystyle k}
[k] is capital, and     f   {\displaystyle f}  [f] is a production_function
satisfying the Inada_conditions. An initial capital stock      k  0   > 0
{\displaystyle k_{0}>0}  [{\displaystyle k_{0}>0}] is assumed.
Let      c  t     {\displaystyle c_{t}}  [c_{t}] be consumption in period t,
and assume consumption yields utility     u (  c  t   ) = ln &#x2061; (  c  t
)   {\displaystyle u(c_{t})=\ln(c_{t})}  [u(c_{t})=\ln(c_{t})] as long as the
consumer lives. Assume the consumer is impatient, so that he discounts future
utility by a factor b each period, where     0 < b < 1   {\displaystyle 0<b<1}
[0<b<1]. Let      k  t     {\displaystyle k_{t}}  [k_{t}] be capital in period
t. Assume initial capital is a given amount      k  0   > 0   {\displaystyle k_
{0}>0}  [k_{0}>0], and suppose that this period's capital and consumption
determine next period's capital as      k  t + 1   = A  k  t   a   &#x2212;  c
t     {\displaystyle k_{t+1}=Ak_{t}^{a}-c_{t}}  [k_{t+1}=Ak_{t}^{a}-c_{t}],
where A is a positive constant and     0 < a < 1   {\displaystyle 0<a<1}
[0<a<1]. Assume capital cannot be negative. Then the consumer's decision
problem can be written as follows:
         max  &#x2211;  t = 0   T    b  t   ln &#x2061; (  c  t   )
      {\displaystyle \max \sum _{t=0}^{T}b^{t}\ln(c_{t})}  [\max \sum _{t=0}^
      {T}b^{t}\ln(c_{t})] subject to      k  t + 1   = A  k  t   a   &#x2212;
      c  t   &#x2265; 0   {\displaystyle k_{t+1}=Ak_{t}^{a}-c_{t}\geq 0}  [k_
      {t+1}=Ak_{t}^{a}-c_{t}\geq 0] for all     t = 0 , 1 , 2 , &#x2026; , T
      {\displaystyle t=0,1,2,\ldots ,T}  [t=0,1,2,\ldots ,T]
Written this way, the problem looks complicated, because it involves solving
for all the choice variables      c  0   ,  c  1   ,  c  2   , &#x2026; ,  c  T
{\displaystyle c_{0},c_{1},c_{2},\ldots ,c_{T}}  [c_{0},c_{1},c_{2},\ldots ,c_
{T}]. (Note that      k  0     {\displaystyle k_{0}}  [k_{0}] is not a choice
variableâthe consumer's initial capital is taken as given.)
The dynamic programming approach to solve this problem involves breaking it
apart into a sequence of smaller decisions. To do so, we define a sequence of
value functions      V  t   ( k )   {\displaystyle V_{t}(k)}  [V_{t}(k)], for
t = 0 , 1 , 2 , &#x2026; , T , T + 1   {\displaystyle t=0,1,2,\ldots ,T,T+1}
[t=0,1,2,\ldots ,T,T+1] which represent the value of having any amount of
capital k at each time t. Note that      V  T + 1   ( k ) = 0   {\displaystyle
V_{T+1}(k)=0}  [V_{T+1}(k)=0], that is, there is (by assumption) no utility
from having capital after death.
The value of any quantity of capital at any previous time can be calculated by
backward_induction using the Bellman_equation. In this problem, for each     t
= 0 , 1 , 2 , &#x2026; , T   {\displaystyle t=0,1,2,\ldots ,T}  [t=0,1,2,\ldots
,T], the Bellman equation is
          V  t   (  k  t   )  =  max  (  ln &#x2061; (  c  t   ) + b  V  t + 1
      (  k  t + 1   )  )    {\displaystyle V_{t}(k_{t})\,=\,\max \left(\ln(c_
      {t})+bV_{t+1}(k_{t+1})\right)}  [{\displaystyle V_{t}(k_{t})\,=\,\max
      \left(\ln(c_{t})+bV_{t+1}(k_{t+1})\right)}] subject to      k  t + 1   =
      A  k  t   a   &#x2212;  c  t   &#x2265; 0   {\displaystyle k_{t+1}=Ak_
      {t}^{a}-c_{t}\geq 0}  [k_{t+1}=Ak_{t}^{a}-c_{t}\geq 0]
This problem is much simpler than the one we wrote down before, because it
involves only two decision variables,      c  t     {\displaystyle c_{t}}  [c_
{t}] and      k  t + 1     {\displaystyle k_{t+1}}  [k_{t+1}]. Intuitively,
instead of choosing his whole lifetime plan at birth, the consumer can take
things one step at a time. At time t, his current capital      k  t
{\displaystyle k_{t}}  [k_{t}] is given, and he only needs to choose current
consumption      c  t     {\displaystyle c_{t}}  [c_{t}] and saving      k  t +
1     {\displaystyle k_{t+1}}  [k_{t+1}].
To actually solve this problem, we work backwards. For simplicity, the current
level of capital is denoted as k.      V  T + 1   ( k )   {\displaystyle V_
{T+1}(k)}  [V_{T+1}(k)] is already known, so using the Bellman equation once we
can calculate      V  T   ( k )   {\displaystyle V_{T}(k)}  [V_{T}(k)], and so
on until we get to      V  0   ( k )   {\displaystyle V_{0}(k)}  [V_{0}(k)],
which is the value of the initial decision problem for the whole lifetime. In
other words, once we know      V  T &#x2212; j + 1   ( k )   {\displaystyle V_
{T-j+1}(k)}  [V_{T-j+1}(k)], we can calculate      V  T &#x2212; j   ( k )
{\displaystyle V_{T-j}(k)}  [V_{T-j}(k)], which is the maximum of     ln
&#x2061; (  c  T &#x2212; j   ) + b  V  T &#x2212; j + 1   ( A  k  a   &#x2212;
c  T &#x2212; j   )   {\displaystyle \ln(c_{T-j})+bV_{T-j+1}(Ak^{a}-c_{T-j})}
[\ln(c_{T-j})+bV_{T-j+1}(Ak^{a}-c_{T-j})], where      c  T &#x2212; j
{\displaystyle c_{T-j}}  [c_{T-j}] is the choice variable and     A  k  a
&#x2212;  c  T &#x2212; j   &#x2265; 0   {\displaystyle Ak^{a}-c_{T-j}\geq 0}
[Ak^{a}-c_{T-j}\geq 0].
Working backwards, it can be shown that the value function at time     t = T
&#x2212; j   {\displaystyle t=T-j}  [t=T-j] is
          V  T &#x2212; j   ( k )  =  a  &#x2211;  i = 0   j    a  i    b  i
      ln &#x2061; k +  v  T &#x2212; j     {\displaystyle V_{T-j}(k)\,=\,a\sum
      _{i=0}^{j}a^{i}b^{i}\ln k+v_{T-j}}  [V_{T-j}(k)\,=\,a\sum _{i=0}^{j}a^
      {i}b^{i}\ln k+v_{T-j}]
where each      v  T &#x2212; j     {\displaystyle v_{T-j}}  [v_{T-j}] is a
constant, and the optimal amount to consume at time     t = T &#x2212; j
{\displaystyle t=T-j}  [t=T-j] is
          c  T &#x2212; j   ( k )  =    1   &#x2211;  i = 0   j    a  i    b  i
      A  k  a     {\displaystyle c_{T-j}(k)\,=\,{\frac {1}{\sum _{i=0}^{j}a^
      {i}b^{i}}}Ak^{a}}  [c_{T-j}(k)\,=\,{\frac {1}{\sum _{i=0}^{j}a^{i}b^
      {i}}}Ak^{a}]
which can be simplified to
              c  T   ( k )    = A  k  a        c  T &#x2212; 1   ( k )    =
      A  k  a     1 + a b         c  T &#x2212; 2   ( k )    =    A  k  a     1
      + a b +  a  2    b  2            &#x2026;      c  2   ( k )    =    A  k
      a     1 + a b +  a  2    b  2   + &#x2026; +  a  T &#x2212; 2    b  T
      &#x2212; 2           c  1   ( k )    =    A  k  a     1 + a b +  a  2
      b  2   + &#x2026; +  a  T &#x2212; 2    b  T &#x2212; 2   +  a  T
      &#x2212; 1    b  T &#x2212; 1           c  0   ( k )    =    A  k  a
      1 + a b +  a  2    b  2   + &#x2026; +  a  T &#x2212; 2    b  T &#x2212;
      2   +  a  T &#x2212; 1    b  T &#x2212; 1   +  a  T    b  T
      {\displaystyle {\begin{aligned}c_{T}(k)&=Ak^{a}\\c_{T-1}(k)&={\frac {Ak^
      {a}}{1+ab}}\\c_{T-2}(k)&={\frac {Ak^{a}}{1+ab+a^{2}b^{2}}}\\&\dots \\c_
      {2}(k)&={\frac {Ak^{a}}{1+ab+a^{2}b^{2}+\ldots +a^{T-2}b^{T-2}}}\\c_{1}
      (k)&={\frac {Ak^{a}}{1+ab+a^{2}b^{2}+\ldots +a^{T-2}b^{T-2}+a^{T-1}b^{T-
      1}}}\\c_{0}(k)&={\frac {Ak^{a}}{1+ab+a^{2}b^{2}+\ldots +a^{T-2}b^{T-2}+a^
      {T-1}b^{T-1}+a^{T}b^{T}}}\end{aligned}}}  [{\displaystyle {\begin
      {aligned}c_{T}(k)&=Ak^{a}\\c_{T-1}(k)&={\frac {Ak^{a}}{1+ab}}\\c_{T-2}
      (k)&={\frac {Ak^{a}}{1+ab+a^{2}b^{2}}}\\&\dots \\c_{2}(k)&={\frac {Ak^
      {a}}{1+ab+a^{2}b^{2}+\ldots +a^{T-2}b^{T-2}}}\\c_{1}(k)&={\frac {Ak^{a}}
      {1+ab+a^{2}b^{2}+\ldots +a^{T-2}b^{T-2}+a^{T-1}b^{T-1}}}\\c_{0}(k)&=
      {\frac {Ak^{a}}{1+ab+a^{2}b^{2}+\ldots +a^{T-2}b^{T-2}+a^{T-1}b^{T-1}+a^
      {T}b^{T}}}\end{aligned}}}]
We see that it is optimal to consume a larger fraction of current wealth as one
gets older, finally consuming all remaining wealth in period T, the last period
of life.
**** Computer programming[edit] ****
 This section needs additional citations for verification. Please help improve_this
 article by adding_citations_to_reliable_sources. Unsourced material may be challenged
 and removed.
 Find sources: "Dynamic_programming" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (April 2014)(Learn_how_and_when_to_remove_this_template_message)
There are two key attributes that a problem must have in order for dynamic
programming to be applicable: optimal_substructure and overlapping_sub-
problems. If a problem can be solved by combining optimal solutions to non-
overlapping sub-problems, the strategy is called "divide_and_conquer" instead.
[1] This is why merge_sort and quick_sort are not classified as dynamic
programming problems.
Optimal substructure means that the solution to a given optimization problem
can be obtained by the combination of optimal solutions to its sub-problems.
Such optimal substructures are usually described by means of recursion. For
example, given a graph G=(V,E), the shortest path p from a vertex u to a vertex
v exhibits optimal substructure: take any intermediate vertex w on this
shortest path p. If p is truly the shortest path, then it can be split into
sub-paths p1 from u to w and p2 from w to v such that these, in turn, are
indeed the shortest paths between the corresponding vertices (by the simple
cut-and-paste argument described in Introduction_to_Algorithms). Hence, one can
easily formulate the solution for finding shortest paths in a recursive manner,
which is what the BellmanâFord_algorithm or the FloydâWarshall_algorithm
does.
Overlapping sub-problems means that the space of sub-problems must be small,
that is, any recursive algorithm solving the problem should solve the same sub-
problems over and over, rather than generating new sub-problems. For example,
consider the recursive formulation for generating the Fibonacci series: Fi =
Fi−1 + Fi−2, with base case F1 = F2 = 1. Then F43 = F42 + F41, and F42
= F41 + F40. Now F41 is being solved in the recursive sub-trees of both F43 as
well as F42. Even though the total number of sub-problems is actually small
(only 43 of them), we end up solving the same problems over and over if we
adopt a naive recursive solution such as this. Dynamic programming takes
account of this fact and solves each sub-problem only once.
Figure 2. The subproblem graph for the Fibonacci sequence. The fact that it is
not a tree indicates overlapping subproblems.
This can be achieved in either of two ways:[citation_needed]
    * Top-down_approach: This is the direct fall-out of the recursive
      formulation of any problem. If the solution to any problem can be
      formulated recursively using the solution to its sub-problems, and if its
      sub-problems are overlapping, then one can easily memoize or store the
      solutions to the sub-problems in a table. Whenever we attempt to solve a
      new sub-problem, we first check the table to see if it is already solved.
      If a solution has been recorded, we can use it directly, otherwise we
      solve the sub-problem and add its solution to the table.
    * Bottom-up_approach: Once we formulate the solution to a problem
      recursively as in terms of its sub-problems, we can try reformulating the
      problem in a bottom-up fashion: try solving the sub-problems first and
      use their solutions to build-on and arrive at solutions to bigger sub-
      problems. This is also usually done in a tabular form by iteratively
      generating solutions to bigger and bigger sub-problems by using the
      solutions to small sub-problems. For example, if we already know the
      values of F41 and F40, we can directly calculate the value of F42.
Some programming_languages can automatically memoize the result of a function
call with a particular set of arguments, in order to speed up call-by-name
evaluation (this mechanism is referred to as call-by-need). Some languages make
it possible portably (e.g. Scheme, Common_Lisp, Perl or D). Some languages have
automatic memoization built in, such as tabled Prolog and J, which supports
memoization with the M. adverb.[4] In any case, this is only possible for a
referentially_transparent function. Memoization is also encountered as an
easily accessible design pattern within term-rewrite based languages such as
Wolfram_Language.
**** Bioinformatics[edit] ****
Dynamic programming is widely used in bioinformatics for the tasks such as
sequence_alignment, protein_folding, RNA structure prediction and protein-DNA
binding. The first dynamic programming algorithms for protein-DNA binding were
developed in the 1970s independently by Charles_DeLisi in USA[5] and Georgii
Gurskii and Alexander Zasedatelev in USSR.[6] Recently these algorithms have
become very popular in bioinformatics and computational biology, particularly
in the studies of nucleosome positioning and transcription_factor binding.
***** Examples: Computer algorithms[edit] *****
**** Dijkstra's algorithm for the shortest path problem[edit] ****
From a dynamic programming point of view, Dijkstra's_algorithm for the shortest
path_problem is a successive approximation scheme that solves the dynamic
programming functional equation for the shortest path problem by the Reaching
method.[7][8][9]
In fact, Dijkstra's explanation of the logic behind the algorithm,[10] namely
     Problem 2. Find the path of minimum total length between two given
     nodes     P   {\displaystyle P}  [P] and     Q   {\displaystyle Q}
     [Q].
     We use the fact that, if     R   {\displaystyle R}  [R] is a node on
     the minimal path from     P   {\displaystyle P}  [P] to     Q
     {\displaystyle Q}  [Q], knowledge of the latter implies the knowledge
     of the minimal path from     P   {\displaystyle P}  [P] to     R
     {\displaystyle R}  [R].
is a paraphrasing of Bellman's famous Principle_of_Optimality in the context of
the shortest_path_problem.
**** Fibonacci sequence[edit] ****
Here is a naÃ¯ve implementation of a function finding the nth member of the
Fibonacci_sequence, based directly on the mathematical definition:
   function fib(n)
       if n <= 1 return n
       return fib(n â 1) + fib(n â 2)
Notice that if we call, say, fib(5), we produce a call tree that calls the
function on the same value many different times:
   1. fib(5)
   2. fib(4) + fib(3)
   3. (fib(3) + fib(2)) + (fib(2) + fib(1))
   4. ((fib(2) + fib(1)) + (fib(1) + fib(0))) + ((fib(1) + fib(0)) + fib(1))
   5. (((fib(1) + fib(0)) + fib(1)) + (fib(1) + fib(0))) + ((fib(1) + fib(0)) +
      fib(1))
In particular, fib(2) was calculated three times from scratch. In larger
examples, many more values of fib, or subproblems, are recalculated, leading to
an exponential time algorithm.
Now, suppose we have a simple map object, m, which maps each value of fib that
has already been calculated to its result, and we modify our function to use it
and update it. The resulting function requires only O(n) time instead of
exponential time (but requires O(n) space):
   var m := map(0 â 0, 1 â 1)
   function fib(n)
       if key n is not in map m
           m[n] := fib(n â 1) + fib(n â 2)
       return m[n]
This technique of saving values that have already been calculated is called
memoization; this is the top-down approach, since we first break the problem
into subproblems and then calculate and store values.
In the bottom-up approach, we calculate the smaller values of fib first, then
build larger values from them. This method also uses O(n) time since it
contains a loop that repeats n â 1 times, but it only takes constant (O(1))
space, in contrast to the top-down approach which requires O(n) space to store
the map.
   function fib(n)
       if n = 0
           return 0
       else
           var previousFib := 0, currentFib := 1
           repeat n â 1 times // loop is skipped if n = 1
               var newFib := previousFib + currentFib
               previousFib := currentFib
               currentFib  := newFib
       return currentFib
In both examples, we only calculate fib(2) one time, and then use it to
calculate both fib(4) and fib(3), instead of computing it every time either of
them is evaluated.
Note that the above method actually takes     &#x03A9; (  n  2   )
{\displaystyle \Omega (n^{2})}  [\Omega (n^{2})] time for large n because
addition of two integers with     &#x03A9; ( n )   {\displaystyle \Omega (n)}
[\Omega (n)] bits each takes     &#x03A9; ( n )   {\displaystyle \Omega (n)}
[\Omega (n)] time. (The nth fibonacci number has     &#x03A9; ( n )
{\displaystyle \Omega (n)}  [\Omega (n)] bits.) Also, there is a closed form
for the Fibonacci sequence, known_as_Binet's_formula, from which the     n
{\displaystyle n}  [n]-th term can be computed in approximately     O ( n ( log
&#x2061; n  )  2   )   {\displaystyle O(n(\log n)^{2})}  [O(n(\log n)^{2})]
time, which is more efficient than the above dynamic programming technique.
However, the simple recurrence directly gives the_matrix_form that leads to an
approximately     O ( n log &#x2061; n )   {\displaystyle O(n\log n)}  [O(n\log
n)] algorithm by fast matrix_exponentiation.
**** A type of balanced 0â1 matrix[edit] ****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (May 2013)(Learn_how_and_when_to_remove_this_template_message)
Consider the problem of assigning values, either zero or one, to the positions
of an n × n matrix, with n even, so that each row and each column contains
exactly n / 2 zeros and n / 2 ones. We ask how many different assignments there
are for a given     n   {\displaystyle n}  [n]. For example, when n = 4, four
possible solutions are
           [    0   1   0   1     1   0   1   0     0   1   0   1     1   0   1
      0    ]    &#xA0;and&#xA0;    [    0   0   1   1     0   0   1   1     1
      1   0   0     1   1   0   0    ]    &#xA0;and&#xA0;    [    1   1   0   0
      0   0   1   1     1   1   0   0     0   0   1   1    ]    &#xA0;and&#xA0;
      [    1   0   0   1     0   1   1   0     0   1   1   0     1   0   0   1
      ]   .   {\displaystyle {\begin
      {bmatrix}0&1&0&1\\1&0&1&0\\0&1&0&1\\1&0&1&0\end{bmatrix}}{\text{ and }}
      {\begin{bmatrix}0&0&1&1\\0&0&1&1\\1&1&0&0\\1&1&0&0\end{bmatrix}}{\text
      { and }}{\begin{bmatrix}1&1&0&0\\0&0&1&1\\1&1&0&0\\0&0&1&1\end{bmatrix}}
      {\text{ and }}{\begin{bmatrix}1&0&0&1\\0&1&1&0\\0&1&1&0\\1&0&0&1\end
      {bmatrix}}.}  [{\begin{bmatrix}0&1&0&1\\1&0&1&0\\0&1&0&1\\1&0&1&0\end
      {bmatrix}}{\text{ and }}{\begin
      {bmatrix}0&0&1&1\\0&0&1&1\\1&1&0&0\\1&1&0&0\end{bmatrix}}{\text{ and }}
      {\begin{bmatrix}1&1&0&0\\0&0&1&1\\1&1&0&0\\0&0&1&1\end{bmatrix}}{\text
      { and }}{\begin{bmatrix}1&0&0&1\\0&1&1&0\\0&1&1&0\\1&0&0&1\end
      {bmatrix}}.]
There are at least three possible approaches: brute_force, backtracking, and
dynamic programming.
Brute force consists of checking all assignments of zeros and ones and counting
those that have balanced rows and columns (n / 2 zeros and n / 2 ones). As
there are          (   n  n  /  2    )      n     {\displaystyle {\tbinom {n}
{n/2}}^{n}}  [{\tbinom {n}{n/2}}^{n}] possible assignments, this strategy is
not practical except maybe up to     n = 6   {\displaystyle n=6}  [n=6].
Backtracking for this problem consists of choosing some order of the matrix
elements and recursively placing ones or zeros, while checking that in every
row and column the number of elements that have not been assigned plus the
number of ones or zeros are both at least n / 2. While more sophisticated than
brute force, this approach will visit every solution once, making it
impractical for n larger than six, since the number of solutions is already
116,963,796,250 for n = 8, as we shall see.
Dynamic programming makes it possible to count the number of solutions without
visiting them all. Imagine backtracking values for the first row â what
information would we require about the remaining rows, in order to be able to
accurately count the solutions obtained for each first row value? We consider k
× n boards, where 1 ≤ k ≤ n, whose     k   {\displaystyle k}  [k] rows contain
n  /  2   {\displaystyle n/2}  [n/2] zeros and     n  /  2   {\displaystyle n/
2}  [n/2] ones. The function f to which memoization is applied maps vectors of
n pairs of integers to the number of admissible boards (solutions). There is
one pair for each column, and its two components indicate respectively the
number of zeros and ones that have yet to be placed in that column. We seek the
value of     f ( ( n  /  2 , n  /  2 ) , ( n  /  2 , n  /  2 ) , &#x2026; ( n
/  2 , n  /  2 ) )   {\displaystyle f((n/2,n/2),(n/2,n/2),\ldots (n/2,n/2))}
[f((n/2,n/2),(n/2,n/2),\ldots (n/2,n/2))] (    n   {\displaystyle n}  [n]
arguments or one vector of     n   {\displaystyle n}  [n] elements). The
process of subproblem creation involves iterating over every one of
(   n  n  /  2    )       {\displaystyle {\tbinom {n}{n/2}}}  [{\tbinom {n}{n/
2}}] possible assignments for the top row of the board, and going through every
column, subtracting one from the appropriate element of the pair for that
column, depending on whether the assignment for the top row contained a zero or
a one at that position. If any one of the results is negative, then the
assignment is invalid and does not contribute to the set of solutions
(recursion stops). Otherwise, we have an assignment for the top row of the k ×
n board and recursively compute the number of solutions to the remaining (k −
1) × n board, adding the numbers of solutions for every admissible assignment
of the top row and returning the sum, which is being memoized. The base case is
the trivial subproblem, which occurs for a 1 × n board. The number of solutions
for this board is either zero or one, depending on whether the vector is a
permutation of n / 2     ( 0 , 1 )   {\displaystyle (0,1)}  [(0,1)] and n / 2
( 1 , 0 )   {\displaystyle (1,0)}  [(1,0)] pairs or not.
For example, in the first two boards shown above the sequences of vectors would
be
((2, 2) (2, 2) (2, 2) (2, 2))       ((2, 2) (2, 2) (2, 2) (2, 2))     k = 4
  0      1      0      1              0      0      1      1

((1, 2) (2, 1) (1, 2) (2, 1))       ((1, 2) (1, 2) (2, 1) (2, 1))     k = 3
  1      0      1      0              0      0      1      1

((1, 1) (1, 1) (1, 1) (1, 1))       ((0, 2) (0, 2) (2, 0) (2, 0))     k = 2
  0      1      0      1              1      1      0      0

((0, 1) (1, 0) (0, 1) (1, 0))       ((0, 1) (0, 1) (1, 0) (1, 0))     k = 1
  1      0      1      0              1      1      0      0

((0, 0) (0, 0) (0, 0) (0, 0))       ((0, 0) (0, 0), (0, 0) (0, 0))
The number of solutions (sequence A058527 in the OEIS) is
         1 ,  2 ,  90 ,  297200 ,  116963796250 ,  6736218287430460752 ,
      &#x2026;   {\displaystyle
      1,\,2,\,90,\,297200,\,116963796250,\,6736218287430460752,\ldots }
      [1,\,2,\,90,\,297200,\,116963796250,\,6736218287430460752,\ldots ]
Links to the MAPLE implementation of the dynamic programming approach may be
found among the external_links.
**** Checkerboard[edit] ****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (May 2013)(Learn_how_and_when_to_remove_this_template_message)
Consider a checkerboard with n Ã n squares and a cost function c(i, j) which
returns a cost associated with square (i,j) (i being the row, j being the
column). For instance (on a 5 Ã 5 checkerboard),
5 6   7   4   7   8
4 7   6   1   1   4
3 3   5   7   8   2
2 â6�  7   0   â
1 ââ*5* ââ
  1   2   3   4   5
Thus c(1, 3) = 5
Let us say there was a checker that could start at any square on the first rank
(i.e., row) and you wanted to know the shortest path (the sum of the minimum
costs at each visited rank) to get to the last rank; assuming the checker could
move only diagonally left forward, diagonally right forward, or straight
forward. That is, a checker on (1,3) can move to (2,2), (2,3) or (2,4).
5
4
3
2   x x x
1     o
  1 2 3 4 5
This problem exhibits optimal substructure. That is, the solution to the entire
problem relies on solutions to subproblems. Let us define a function q(i, j) as
      q(i, j) = the minimum cost to reach square (i, j).
Starting at rank n and descending to rank 1, we compute the value of this
function for all the squares at each successive rank. Picking the square that
holds the minimum value at each rank gives us the shortest path between rank n
and rank 1.
Note that q(i, j) is equal to the minimum cost to get to any of the three
squares below it (since those are the only squares that can reach it) plus c(i,
j). For instance:
5
4     A
3   B C D
2
1
  1 2 3 4 5
         q ( A ) = min ( q ( B ) , q ( C ) , q ( D ) ) + c ( A )
      {\displaystyle q(A)=\min(q(B),q(C),q(D))+c(A)\,}  [q(A)=\min(q(B),q(C),q
      (D))+c(A)\,]
Now, let us define q(i, j) in somewhat more general terms:
         q ( i , j ) =   {    &#x221E;   j < 1  &#xA0;or&#xA0;  j > n     c ( i
      , j )   i = 1     min ( q ( i &#x2212; 1 , j &#x2212; 1 ) , q ( i
      &#x2212; 1 , j ) , q ( i &#x2212; 1 , j + 1 ) ) + c ( i , j )
      otherwise.          {\displaystyle q(i,j)={\begin{cases}\infty &j<1{\text
      { or }}j>n\\c(i,j)&i=1\\\min(q(i-1,j-1),q(i-1,j),q(i-1,j+1))+c(i,j)&
      {\text{otherwise.}}\end{cases}}}  [q(i,j)={\begin{cases}\infty &j<1{\text
      { or }}j>n\\c(i,j)&i=1\\\min(q(i-1,j-1),q(i-1,j),q(i-1,j+1))+c(i,j)&
      {\text{otherwise.}}\end{cases}}]
The first line of this equation deals with a board modeled as squares indexed
on 1 at the lowest bound and n at the highest bound. The second line specifies
what happens at the last rank; providing a base case. The third line, the
recursion, is the important part. It represents the A,B,C,D terms in the
example. From this definition we can derive straightforward recursive code for
q(i, j). In the following pseudocode, n is the size of the board, c(i, j) is
the cost function, and min() returns the minimum of a number of values:
function minCost(i, j)
    if j < 1 or j > n
        return infinity
    else if i = 1
        return c(i, j)
    else
        return min( minCost(i-1, j-1), minCost(i-1, j), minCost(i-1, j+1) ) + c
(i, j)
This function only computes the path cost, not the actual path. We discuss the
actual path below. This, like the Fibonacci-numbers example, is horribly slow
because it too exhibits the overlapping sub-problems attribute. That is, it
recomputes the same path costs over and over. However, we can compute it much
faster in a bottom-up fashion if we store path costs in a two-dimensional array
q[i, j] rather than using a function. This avoids recomputation; all the values
needed for array q[i, j] are computed ahead of time only once. Precomputed
values for (i,j) are simply looked-up whenever needed.
We also need to know what the actual shortest path is. To do this, we use
another array p[i, j]; a predecessor array. This array records the path to any
square s. The predecessor of s is modeled as an offset relative to the index
(in q[i, j]) of the precomputed path cost of s. To reconstruct the complete
path, we lookup the predecessor of s, then the predecessor of that square, then
the predecessor of that square, and so on recursively, until we reach the
starting square. Consider the following code:
 function computeShortestPathArrays()
     for x from 1 to n
         q[1, x] := c(1, x)
     for y from 1 to n
         q[y, 0]     := infinity
         q[y, n + 1] := infinity
     for y from 2 to n
         for x from 1 to n
             m := min(q[y-1, x-1], q[y-1, x], q[y-1, x+1])
             q[y, x] := m + c(y, x)
             if m = q[y-1, x-1]
                 p[y, x] := -1
             else if m = q[y-1, x]
                 p[y, x] :=  0
             else
                 p[y, x] :=  1
Now the rest is a simple matter of finding the minimum and printing it.
 function computeShortestPath()
     computeShortestPathArrays()
     minIndex := 1
     min := q[n, 1]
     for i from 2 to n
         if q[n, i] < min
             minIndex := i
             min := q[n, i]
     printPath(n, minIndex)
 function printPath(y, x)
     print(x)
     print("<-")
     if y = 2
         print(x + p[y, x])
     else
         printPath(y-1, x + p[y, x])
**** Sequence alignment[edit] ****
In genetics, sequence_alignment is an important application where dynamic
programming is essential.[11] Typically, the problem consists of transforming
one sequence into another using edit operations that replace, insert, or remove
an element. Each operation has an associated cost, and the goal is to find the
sequence_of_edits_with_the_lowest_total_cost.
The problem can be stated naturally as a recursion, a sequence A is optimally
edited into a sequence B by either:
   1. inserting the first character of B, and performing an optimal alignment
      of A and the tail of B
   2. deleting the first character of A, and performing the optimal alignment
      of the tail of A and B
   3. replacing the first character of A with the first character of B, and
      performing optimal alignments of the tails of A and B.
The partial alignments can be tabulated in a matrix, where cell (i,j) contains
the cost of the optimal alignment of A[1..i] to B[1..j]. The cost in cell (i,j)
can be calculated by adding the cost of the relevant operations to the cost of
its neighboring cells, and selecting the optimum.
Different variants exist, see SmithâWaterman_algorithm and NeedlemanâWunsch
algorithm.
**** Tower of Hanoi puzzle[edit] ****
A model set of the Towers of Hanoi (with 8 disks)
An animated solution of the Tower of Hanoi puzzle for T(4,3).
The Tower_of_Hanoi or Towers of Hanoi is a mathematical_game or puzzle. It
consists of three rods, and a number of disks of different sizes which can
slide onto any rod. The puzzle starts with the disks in a neat stack in
ascending order of size on one rod, the smallest at the top, thus making a
conical shape.
The objective of the puzzle is to move the entire stack to another rod, obeying
the following rules:
    * Only one disk may be moved at a time.
    * Each move consists of taking the upper disk from one of the rods and
      sliding it onto another rod, on top of the other disks that may already
      be present on that rod.
    * No disk may be placed on top of a smaller disk.
The dynamic programming solution consists of solving the functional_equation
      S(n,h,t) = S(n-1,h, not(h,t)) ; S(1,h,t) ; S(n-1,not(h,t),t)
where n denotes the number of disks to be moved, h denotes the home rod, t
denotes the target rod, not(h,t) denotes the third rod (neither h nor t), ";"
denotes concatenation, and
      S(n, h, t) := solution to a problem consisting of n disks that are to be
      moved from rod h to rod t.
Note that for n=1 the problem is trivial, namely S(1,h,t) = "move a disk from
rod h to rod t" (there is only one disk left).
The number of moves required by this solution is 2n − 1. If the objective is to
maximize the number of moves (without cycling) then the dynamic programming
functional_equation is slightly more complicated and 3n − 1 moves are required.
[12]
**** Egg dropping puzzle[edit] ****
The following is a description of the instance of this famous puzzle involving
N=2 eggs and a building with H=36 floors:[13]
      Suppose that we wish to know which stories in a 36-story building are
      safe to drop eggs from, and which will cause the eggs to break on landing
      (using U.S._English terminology, in which the first floor is at ground
      level). We make a few assumptions:
          * An egg that survives a fall can be used again.
          * A broken egg must be discarded.
          * The effect of a fall is the same for all eggs.
          * If an egg breaks when dropped, then it would break if dropped from
            a higher window.
          * If an egg survives a fall, then it would survive a shorter fall.
          * It is not ruled out that the first-floor windows break eggs, nor is
            it ruled out that eggs can survive the 36th-floor windows.
      If only one egg is available and we wish to be sure of obtaining the
      right result, the experiment can be carried out in only one way. Drop the
      egg from the first-floor window; if it survives, drop it from the second-
      floor window. Continue upward until it breaks. In the worst case, this
      method may require 36 droppings. Suppose 2 eggs are available. What is
      the lowest number of egg-droppings that is guaranteed to work in all
      cases?
To derive a dynamic programming functional_equation for this puzzle, let the
state of the dynamic programming model be a pair s = (n,k), where
      n = number of test eggs available, n = 0, 1, 2, 3, ..., N − 1.
      k = number of (consecutive) floors yet to be tested, k = 0, 1, 2, ...,
      H − 1.
For instance, s = (2,6) indicates that two test eggs are available and 6
(consecutive) floors are yet to be tested. The initial state of the process is
s = (N,H) where N denotes the number of test eggs available at the commencement
of the experiment. The process terminates either when there are no more test
eggs (n = 0) or when k = 0, whichever occurs first. If termination occurs at
state s = (0,k) and k > 0, then the test failed.
Now, let
      W(n,k) = minimum number of trials required to identify the value of the
      critical floor under the worst-case scenario given that the process is in
      state s = (n,k).
Then it can be shown that[14]
      W(n,k) = 1 + min{max(W(n − 1, x − 1), W(n,k − x)): x = 1, 2, ..., k }
with W(n,0) = 0 for all n > 0 and W(1,k) = k for all k. It is easy to solve
this equation iteratively by systematically increasing the values of n and k.
An interactive online facility is available for experimentation with this model
as well as with other versions of this puzzle (e.g. when the objective is to
minimize the expected value of the number of trials.)[14]
*** Faster DP solution using a different parametrization[edit] ***
Notice that the above solution takes     O ( n  k  2   )   {\displaystyle O(nk^
{2})}  [O(nk^{2})] time with a DP solution. This can be improved to     O ( n k
log &#x2061; k )   {\displaystyle O(nk\log k)}  [O(nk\log k)] time by binary
searching on the optimal     x   {\displaystyle x}  [x] in the above
recurrence, since     W ( n &#x2212; 1 , x &#x2212; 1 )   {\displaystyle W(n-
1,x-1)}  [W(n-1,x-1)] is increasing in     x   {\displaystyle x}  [x] while
W ( n , k &#x2212; x )   {\displaystyle W(n,k-x)}  [W(n,k-x)] is decreasing in
x   {\displaystyle x}  [x], thus a local minimum of     max ( W ( n &#x2212; 1
, x &#x2212; 1 ) , W ( n , k &#x2212; x ) )   {\displaystyle \max(W(n-1,x-1),W
(n,k-x))}  [\max(W(n-1,x-1),W(n,k-x))] is a global minimum. Also, by storing
the optimal     x   {\displaystyle x}  [x] for each cell in the DP table and
referring to its value for the previous cell, the optimal     x
{\displaystyle x}  [x] for each cell can be found in constant time, improving
it to     O ( n k )   {\displaystyle O(nk)}  [O(nk)] time. However, there is an
even faster solution that involves a different parametrization of the problem:
Let     k   {\displaystyle k}  [k] be the total number of floors such that the
eggs break when dropped from the     k   {\displaystyle k}  [k]th floor (The
example above is equivalent to taking     k = 37   {\displaystyle k=37}
[k=37]).
Let     m   {\displaystyle m}  [m] be the minimum floor from which the egg must
be dropped to be broken.
Let     f ( t , n )   {\displaystyle f(t,n)}  [f(t,n)] be the maximum number of
values of     m   {\displaystyle m}  [m] that are distinguishable using     t
{\displaystyle t}  [t] tries and     n   {\displaystyle n}  [n] eggs.
Then     f ( t , 0 ) = f ( 0 , n ) = 1   {\displaystyle f(t,0)=f(0,n)=1}  [f
(t,0)=f(0,n)=1] for all     t , n &#x2265; 0   {\displaystyle t,n\geq 0}
[t,n\geq 0].
Let     a   {\displaystyle a}  [a] be the floor from which the first egg is
dropped in the optimal strategy.
If the first egg broke,     m   {\displaystyle m}  [m] is from     1
{\displaystyle 1}  [1] to     a   {\displaystyle a}  [a] and distinguishable
using at most     t &#x2212; 1   {\displaystyle t-1}  [t-1] tries and     n
&#x2212; 1   {\displaystyle n-1}  [n-1] eggs.
If the first egg did not break,     m   {\displaystyle m}  [m] is from     a +
1   {\displaystyle a+1}  [a+1] to     k   {\displaystyle k}  [k] and
distinguishable using     t &#x2212; 1   {\displaystyle t-1}  [t-1] tries and
n   {\displaystyle n}  [n] eggs.
Therefore,     f ( t , n ) = f ( t &#x2212; 1 , n &#x2212; 1 ) + f ( t &#x2212;
1 , n )   {\displaystyle f(t,n)=f(t-1,n-1)+f(t-1,n)}  [f(t,n)=f(t-1,n-1)+f(t-
1,n)].
Then the problem is equivalent to finding the minimum     x   {\displaystyle x}
[x] such that     f ( x , n ) &#x2265; k   {\displaystyle f(x,n)\geq k}  [f
(x,n)\geq k].
To do so, we could compute     { f ( t , i ) : 0 &#x2264; i &#x2264; n }
{\displaystyle \{f(t,i):0\leq i\leq n\}}  [\{f(t,i):0\leq i\leq n\}] in order
of increasing     t   {\displaystyle t}  [t], which would take     O ( n x )
{\displaystyle O(nx)}  [O(nx)] time.
Thus, if we separately handle the case of     n = 1   {\displaystyle n=1}
[n=1], the algorithm would take     O ( n   k   )   {\displaystyle O(n{\sqrt
{k}})}  [O(n{\sqrt {k}})] time.
But the recurrence relation can in fact be solved, giving     f ( t , n ) =
&#x2211;  i = 0   n      (   t i   )      {\displaystyle f(t,n)=\sum _{i=0}^{n}
{\binom {t}{i}}}  [f(t,n)=\sum _{i=0}^{n}{\binom {t}{i}}], which can be
computed in     O ( n )   {\displaystyle O(n)}  [O(n)] time using the identity
(   t  i + 1    )    =    (   t i   )       t &#x2212; i   i + 1
{\displaystyle {\binom {t}{i+1}}={\binom {t}{i}}{\frac {t-i}{i+1}}}  [{\binom
{t}{i+1}}={\binom {t}{i}}{\frac {t-i}{i+1}}] for all     i &#x2265; 0
{\displaystyle i\geq 0}  [i\geq 0].
Since     f ( t , n ) &#x2264; f ( t + 1 , n )   {\displaystyle f(t,n)\leq f
(t+1,n)}  [f(t,n)\leq f(t+1,n)] for all     t &#x2265; 0   {\displaystyle t\geq
0}  [t\geq 0], we can binary search on     t   {\displaystyle t}  [t] to find
x   {\displaystyle x}  [x], giving an     O ( n log &#x2061; k )
{\displaystyle O(n\log k)}  [O(n\log k)] algorithm. [15]
**** Matrix chain multiplication[edit] ****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (May 2013)(Learn_how_and_when_to_remove_this_template_message)
Main article: Matrix_chain_multiplication
Matrix chain multiplication is a well-known example that demonstrates utility
of dynamic programming. For example, engineering applications often have to
multiply a chain of matrices. It is not surprising to find matrices of large
dimensions, for example 100Ã100. Therefore, our task is to multiply matrices
A  1   ,  A  2   , . . . .  A  n     {\displaystyle A_{1},A_{2},....A_{n}}  [
{\displaystyle A_{1},A_{2},....A_{n}}]. As we know from basic linear algebra,
matrix multiplication is not commutative, but is associative; and we can
multiply only two matrices at a time. So, we can multiply this chain of
matrices in many different ways, for example:
      ((A1 Ã A2) Ã A3) Ã ... An
      A1Ã(((A2ÃA3)Ã ... ) Ã An)
      (A1 Ã A2) Ã (A3 Ã ... An)
and so on. There are numerous ways to multiply this chain of matrices. They
will all produce the same final result, however they will take more or less
time to compute, based on which particular matrices are multiplied. If matrix A
has dimensions mÃn and matrix B has dimensions nÃq, then matrix C=AÃB will
have dimensions mÃq, and will require m*n*q scalar multiplications (using a
simplistic matrix multiplication algorithm for purposes of illustration).
For example, let us multiply matrices A, B and C. Let us assume that their
dimensions are mÃn, nÃp, and pÃs, respectively. Matrix AÃBÃC will be of
size mÃs and can be calculated in two ways shown below:
   1. Ax(BÃC) This order of matrix multiplication will require nps + mns
      scalar multiplications.
   2. (AÃB)ÃC This order of matrix multiplication will require mnp + mps
      scalar calculations.
Let us assume that m = 10, n = 100, p = 10 and s = 1000. So, the first way to
multiply the chain will require 1,000,000 + 1,000,000 calculations. The second
way will require only 10,000+100,000 calculations. Obviously, the second way is
faster, and we should multiply the matrices using that arrangement of
parenthesis.
Therefore, our conclusion is that the order of parenthesis matters, and that
our task is to find the optimal order of parenthesis.
At this point, we have several choices, one of which is to design a dynamic
programming algorithm that will split the problem into overlapping problems and
calculate the optimal arrangement of parenthesis. The dynamic programming
solution is presented below.
Let's call m[i,j] the minimum number of scalar multiplications needed to
multiply a chain of matrices from matrix i to matrix j (i.e. Ai Ã .... Ã Aj,
i.e. i<=j). We split the chain at some matrix k, such that i <= k < j, and try
to find out which combination produces minimum m[i,j].
The formula is:
       if i = j, m[i,j]= 0
       if i < j, m[i,j]= min over all possible values of k (m[i,k]+m[k+1,j] +




          p

            i
            &#x2212;
            1


        &#x2217;

          p

            k


        &#x2217;

          p

            j




    {\displaystyle p_{i-1}*p_{k}*p_{j}}

[p_{i-1}*p_{k}*p_{j}])
where k ranges from i to j − 1.
    *     p  i &#x2212; 1     {\displaystyle p_{i-1}}  [p_{i-1}] is the row
      dimension of matrix i,
    *     p  k     {\displaystyle p_{k}}  [p_{k}] is the column dimension of
      matrix k,
    *     p  j     {\displaystyle p_{j}}  [p_{j}] is the column dimension of
      matrix j.
This formula can be coded as shown below, where input parameter "chain" is the
chain of matrices, i.e.      A  1   ,  A  2   , . . .  A  n     {\displaystyle
A_{1},A_{2},...A_{n}}  [A_{1},A_{2},...A_{n}]:
 function OptimalMatrixChainParenthesis(chain)
     n = length(chain)
     for i = 1, n
         m[i,i] = 0    // Since it takes no calculations to multiply one matrix
     for len = 2, n
         for i = 1, n - len + 1
             j = i + len -1
             m[i,j] = infinity      // So that the first calculation updates
             for k = i, j-1
                 q = m[i, k] + m[k+1, j] +




          p

            i
            &#x2212;
            1


        &#x2217;

          p

            k


        &#x2217;

          p

            j




    {\displaystyle p_{i-1}*p_{k}*p_{j}}

[p_{i-1}*p_{k}*p_{j}]
                 if q < m[i, j]     // The new order of parentheses is better
than what we had
                     m[i, j] = q    // Update
                     s[i, j] = k    // Record which k to split on, i.e. where
to place the parenthesis
So far, we have calculated values for all possible m[i, j], the minimum number
of calculations to multiply a chain from matrix i to matrix j, and we have
recorded the corresponding "split point"s[i, j]. For example, if we are
multiplying chain A1ÃA2ÃA3ÃA4, and it turns out that m[1, 3] = 100 and s[1,
3] = 2, that means that the optimal placement of parenthesis for matrices 1 to
3 is     (  A  1   &#x00D7;  A  2   ) &#x00D7;  A  3     {\displaystyle (A_
{1}\times A_{2})\times A_{3}}  [{\displaystyle (A_{1}\times A_{2})\times A_
{3}}] and to multiply those matrices will require 100 scalar calculation.
This algorithm will produce "tables" m[, ] and s[, ] that will have entries for
all possible values of i and j. The final solution for the entire chain is m[1,
n], with corresponding split at s[1, n]. Unraveling the solution will be
recursive, starting from the top and continuing until we reach the base case,
i.e. multiplication of single matrices.
Therefore, the next step is to actually split the chain, i.e. to place the
parenthesis where they (optimally) belong. For this purpose we could use the
following algorithm:
 function PrintOptimalParenthesis(s, i, j)
     if i = j
        print "A"i
     else
        print "(" PrintOptimalParenthesis(s, i, s[i, j])
PrintOptimalParenthesis(s, s[i, j] + 1, j) ")"
Of course, this algorithm is not useful for actual multiplication. This
algorithm is just a user-friendly way to see what the result looks like.
To actually multiply the matrices using the proper splits, we need the
following algorithm:
   function MatrixChainMultiply(chain from 1 to n)       // returns the final
matrix, i.e. A1ÃA2Ã... ÃAn
      OptimalMatrixChainParenthesis(chain from 1 to n)   // this will produce s
[ . ] and m[ . ] "tables"
      OptimalMatrixMultiplication(s, chain from 1 to n)  // actually multiply

   function OptimalMatrixMultiplication(s, i, j)   // returns the result of
multiplying a chain of matrices from Ai to Aj in optimal way
      if i < j
         // keep on splitting the chain and multiplying the matrices in left
and right sides
         LeftSide = OptimalMatrixMultiplication(s, i, s[i, j])
         RightSide = OptimalMatrixMultiplication(s, s[i, j] + 1, j)
         return MatrixMultiply(LeftSide, RightSide)
      else if i = j
         return Ai   // matrix at position i
      else
         print "error, i <= j must hold"

    function MatrixMultiply(A, B)    // function that multiplies two matrices
      if columns(A) = rows(B)
         for i = 1, rows(A)
            for j = 1, columns(B)
               C[i, j] = 0
               for k = 1, columns(A)
                   C[i, j] = C[i, j] + A[i, k]*B[k, j]
               return C
      else
          print "error, incompatible dimensions."
***** History[edit] *****
The term dynamic programming was originally used in the 1940s by Richard
Bellman to describe the process of solving problems where one needs to find the
best decisions one after another. By 1953, he refined this to the modern
meaning, referring specifically to nesting smaller decision problems inside
larger decisions,[16] and the field was thereafter recognized by the IEEE as a
systems_analysis and engineering topic. Bellman's contribution is remembered in
the name of the Bellman_equation, a central result of dynamic programming which
restates an optimization problem in recursive form.
Bellman explains the reasoning behind the term dynamic programming in his
autobiography, Eye of the Hurricane: An Autobiography (1984, page 159). He
explains:
      "I spent the Fall quarter (of 1950) at RAND. My first task was to find a
      name for multistage decision processes. An interesting question is, Where
      did the name, dynamic programming, come from? The 1950s were not good
      years for mathematical research. We had a very interesting gentleman in
      Washington named Wilson. He was Secretary of Defense, and he actually had
      a pathological fear and hatred of the word research. Iâm not using the
      term lightly; Iâm using it precisely. His face would suffuse, he would
      turn red, and he would get violent if people used the term research in
      his presence. You can imagine how he felt, then, about the term
      mathematical. The RAND Corporation was employed by the Air Force, and the
      Air Force had Wilson as its boss, essentially. Hence, I felt I had to do
      something to shield Wilson and the Air Force from the fact that I was
      really doing mathematics inside the RAND Corporation. What title, what
      name, could I choose? In the first place I was interested in planning, in
      decision making, in thinking. But planning, is not a good word for
      various reasons. I decided therefore to use the word âprogrammingâ. I
      wanted to get across the idea that this was dynamic, this was multistage,
      this was time-varying. I thought, let's kill two birds with one stone.
      Let's take a word that has an absolutely precise meaning, namely dynamic,
      in the classical physical sense. It also has a very interesting property
      as an adjective, and that is it's impossible to use the word dynamic in a
      pejorative sense. Try thinking of some combination that will possibly
      give it a pejorative meaning. It's impossible. Thus, I thought dynamic
      programming was a good name. It was something not even a Congressman
      could object to. So I used it as an umbrella for my activities."
The word dynamic was chosen by Bellman to capture the time-varying aspect of
the problems, and because it sounded impressive.[11] The word programming
referred to the use of the method to find an optimal program, in the sense of a
military schedule for training or logistics. This usage is the same as that in
the phrases linear_programming and mathematical programming, a synonym for
mathematical_optimization.[17]
The above explanation of the origin of the term is lacking. As Russell and
Norvig in their book have written, referring to the above story: "This cannot
be strictly true, because his first paper using the term (Bellman, 1952)
appeared before Wilson became Secretary of Defense in 1953.â[18] Also, there
is a comment in a speech by Harold_J._Kushner, where he remembers Bellman.
Quoting Kushner as he speaks of Bellman: "On the other hand, when I asked him
the same question, he replied that he was trying to upstage Dantzig's linear
programming by adding dynamic. Perhaps both motivations were true."
***** Algorithms that use dynamic programming[edit] *****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (May 2013)(Learn_how_and_when_to_remove_this_template_message)
    * Recurrent solutions to lattice_models for protein-DNA binding
    * Backward_induction as a solution method for finite-horizon discrete-time
      dynamic optimization problems
    * Method_of_undetermined_coefficients can be used to solve the Bellman
      equation in infinite-horizon, discrete-time, discounted, time-invariant
      dynamic optimization problems
    * Many string algorithms including longest_common_subsequence, longest
      increasing_subsequence, longest_common_substring, Levenshtein_distance
      (edit distance)
    * Many algorithmic problems on graphs can be solved efficiently for graphs
      of bounded treewidth or bounded clique-width by using dynamic programming
      on a tree_decomposition of the graph.
    * The CockeâYoungerâKasami_(CYK)_algorithm which determines whether and
      how a given string can be generated by a given context-free_grammar
    * Knuth's_word_wrapping_algorithm that minimizes raggedness when word
      wrapping text
    * The use of transposition_tables and refutation_tables in computer_chess
    * The Viterbi_algorithm (used for hidden_Markov_models, and particularly in
      part_of_speech_tagging)
    * The Earley_algorithm (a type of chart_parser)
    * The NeedlemanâWunsch_algorithm and other algorithms used in
      bioinformatics, including sequence_alignment, structural_alignment, RNA
      structure_prediction
    * Floyd's_all-pairs_shortest_path_algorithm
    * Optimizing the order for chain_matrix_multiplication
    * Pseudo-polynomial_time algorithms for the subset_sum, knapsack and
      partition problems
    * The dynamic_time_warping algorithm for computing the global distance
      between two time series
    * The Selinger (a.k.a. System_R) algorithm for relational database query
      optimization
    * De_Boor_algorithm for evaluating B-spline curves
    * DuckworthâLewis_method for resolving the problem when games of cricket
      are interrupted
    * The value iteration method for solving Markov_decision_processes
    * Some graphic image edge following selection methods such as the "magnet"
      selection tool in Photoshop
    * Some methods for solving interval_scheduling problems
    * Some methods for solving the travelling_salesman_problem, either exactly
      (in exponential_time) or approximately (e.g. via the bitonic_tour)
    * Recursive_least_squares method
    * Beat tracking in music_information_retrieval
    * Adaptive-critic training strategy for artificial_neural_networks
    * Stereo algorithms for solving the correspondence_problem used in stereo
      vision
    * Seam_carving (content-aware image resizing)
    * The BellmanâFord_algorithm for finding the shortest distance in a graph
    * Some approximate solution methods for the linear_search_problem
    * Kadane's algorithm for the maximum_subarray_problem
    * Optimization of electric generation expansion plans in the Wein_Automatic
      System_Planning_(WASP) package
***** See also[edit] *****
    * [icon]Computer_science_portal
    * Convexity_in_economics
    * Greedy_algorithm
    * Non-convexity_(economics)
    * Stochastic_programming
    * Stochastic_dynamic_programming
***** References[edit] *****
   1. ^ a b Cormen, T. H.; Leiserson, C. E.; Rivest, R. L.; Stein, C. (2001),
      Introduction to Algorithms (2nd ed.), MIT Press & McGrawâHill,
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
   3. ISBN 0-262-03293-7 . pp. 344.
   4. ^Kamien,_M._I.; Schwartz,_N._L. (1991). Dynamic_Optimization:_The
      Calculus_of_Variations_and_Optimal_Control_in_Economics_and_Management
      (Second ed.). New York: Elsevier. p. 261. ISBN 978-0-444-01609-6.
   5. ^Kirk, Donald E. (1970). Optimal_Control_Theory:_An_Introduction.
      Englewood Cliffs, NJ: Prentice-Hall. pp. 94â95. ISBN 978-0-13-638098-6.
   6. ^"M._Memo". J Vocabulary. J Software. Retrieved 28 October 2011.
   7. ^ DeLisi, Biopolymers, 1974, Volume 13, Issue 7, pages 1511â1512, July
      1974
   8. ^ GurskiÄ­ GV, Zasedatelev AS, Biofizika, 1978 Sep-Oct;23(5):932-46
   9. ^Sniedovich, M. (2006), "Dijkstra's_algorithm_revisited:_the_dynamic
      programming_connexion" (PDF), Journal of Control and Cybernetics, 35 (3):
      599â620.
  10.  Online_version_of_the_paper_with_interactive_computational_modules.
  11. ^Denardo, E.V. (2003), Dynamic Programming: Models and Applications,
      Mineola, NY: Dover_Publications, ISBN 978-0-486-42810-9
  12. ^Sniedovich, M. (2010), Dynamic Programming: Foundations and Principles,
      Taylor_&_Francis, ISBN 978-0-8247-4099-3
  13. ^ Dijkstra_1959, p. 270
  14. ^ a bEddy,_S._R. (2004). "What is Dynamic Programming?". Nature
      Biotechnology. 22 (7): 909â910. doi:10.1038/nbt0704-909. PMID 15229554.
  15. ^Moshe Sniedovich (2002), "OR/MS_Games:_2._The_Towers_of_Hanoi_Problem",
      INFORMS Transactions on Education, 3 (1): 34â51.
  16. ^ Konhauser J.D.E., Velleman, D., and Wagon, S. (1996). Which_way_did_the
      Bicycle_Go?[permanent_dead_link] Dolciani Mathematical Expositions â No
      18. The_Mathematical_Association_of_America.
  17. ^ a b Sniedovich, M. (2003). The_joy_of_egg-dropping_in_Braunschweig_and
      Hong_Kong. INFORMS Transactions on Education, 4(1) 48â64.
  18. ^Dean Connable Wills, Connections_between_combinatorics_of_permutations
      and_algorithms_and_geometry
  19. ^ Stuart Dreyfus. "Richard_Bellman_on_the_birth_of_Dynamical
      Programming".
  20. ^Nocedal, J.; Wright, S. J. (2006). Numerical Optimization. Springer.
      p. 9.
  21. ^Russell, S.; Norvig, P. (2009). Artificial Intelligence: A Modern
      Approach (3rd ed.). Prentice Hall. ISBN 978-0-13-207148-2.
***** Further reading[edit] *****
    * Adda, Jerome; Cooper, Russell (2003), Dynamic_Economics, MIT Press
. An accessible introduction to dynamic programming in economics. The link
contains sample programs.
Bellman,_Richard (1954), "The theory of dynamic programming", Bulletin_of_the
American_Mathematical_Society, 60 (6): 503â516, doi:10.1090/S0002-9904-1954-
09848-8, MR 0067459, PMC 1063639, PMID 16589166
. Includes an extensive bibliography of the literature in the area, up to the
year 1954.
Bellman,_Richard (1957), Dynamic Programming, Princeton University Press
. Dover paperback edition (2003),
ISBN 0-486-42809-5.
Bertsekas, D. P. (2017), Dynamic Programming and Optimal Control (4th ed.),
Athena Scientific, ISBN 978-1-886529-08-3
. In two volumes.
Cormen,_Thomas_H.; Leiserson,_Charles_E.; Rivest,_Ronald_L.; Stein,_Clifford
(2001), Introduction_to_Algorithms (2nd ed.), MIT Press & McGrawâHill,
ISBN 978-0-262-03293-3
. Especially pp. 323â69.
Dreyfus, Stuart E.; Law, Averill M. (1977), The Art and Theory of Dynamic
Programming, Academic Press, ISBN 978-0-12-221860-6
.
Giegerich, R.; Meyer, C.; Steffen, P. (2004), "A_Discipline_of_Dynamic
Programming_over_Sequence_Data" (PDF), Science of Computer Programming, 51 (3):
215â263, doi:10.1016/j.scico.2003.12.005
.
Meyn, Sean (2007), Control_Techniques_for_Complex_Networks, Cambridge
University Press, ISBN 978-0-521-88441-9, archived from the_original on 2010-
06-19
.
Sritharan, S. S. (1991). "Dynamic Programming of the Navier-Stokes Equations".
Systems and Control Letters. 16 (4): 299â307. doi:10.1016/0167-6911(91)90020-
f.
Stokey,_Nancy; Lucas,_Robert_E.; Prescott,_Edward (1989), Recursive Methods in
Economic Dynamics, Harvard Univ. Press, ISBN 978-0-674-75096-8
.
***** External links[edit] *****
 This article's use of external_links may not follow Wikipedia's policies or
 guidelines. Please improve_this_article by removing excessive or inappropriate
 external links, and converting useful links where appropriate into footnote
 references. (March 2016)(Learn_how_and_when_to_remove_this_template_message)
    * 7_Step_Framework_to_Solve_Dynamic_Programming_Interview_Problems
    * An_Introduction_to_Dynamic_Programming
    * Dynamic_Optimization_Online_Course
    * A_Tutorial_on_Dynamic_programming
    * MIT_course_on_algorithms â Includes a video lecture on DP along with
      lecture notes
    * More_DP_Notes
    * King, Ian, 2002 (1987), "A_Simple_Introduction_to_Dynamic_Programming_in
      Macroeconomic_Models." An introduction to dynamic programming as an
      important tool in economic theory.
    * Dynamic_Programming:_from_novice_to_advanced A TopCoder.com article by
      Dumitru on Dynamic Programming
    * Algebraic_Dynamic_Programming â a formalized framework for dynamic
      programming, including an entry-level_course to DP, University of
      Bielefeld
    * Dreyfus, Stuart, "Richard_Bellman_on_the_birth_of_Dynamic_Programming."
    * Dynamic_programming_tutorial
    * A_Gentle_Introduction_to_Dynamic_Programming_and_the_Viterbi_Algorithm
    * Tabled Prolog BProlog and XSB
    * Online_interactive_dynamic_programming_modules including, shortest path,
      traveling salesman, knapsack, false coin, egg dropping, bridge and torch,
      replacement, chained matrix products, and critical path problem.
    * v
    * t
    * e
Optimization: Algorithms, methods, and heuristics
Unconstrained_nonlinear
               * Golden-section_search
â¦         * Interpolation_methods
functions      * Line_search
               * NelderâMead_method
               * Successive_parabolic_interpolation
           Convergence        * Trust_region
                              * Wolfe_conditions
                              * BerndtâHallâHallâHausman
           QuasiâNewt    * BroydenâFletcherâGoldfarbâShanno and L-BFGS
â¦ and                    * DavidonâFletcherâPowell
gradients                     * Symmetric_rank-one_(SR1)
                              * GaussâNewton
                              * Gradient
           Other_methods      * LevenbergâMarquardt
                              * Conjugate_gradient
                              * Truncated_Newton
â¦ and     * Newton's_method
Hessians
Constrained_nonlinear
General            * Barrier_methods
                   * Penalty_methods
                   * Augmented_Lagrangian_methods
Differentiable     * Sequential_quadratic_programming
                   * Successive_linear_programming                                         [Graph_of
Convex_optimization                                                                        a
Convex           * Cutting-plane_method                                                    strictly
minimization     * Reduced_gradient_(FrankâWolfe)                                     concave
                 * Subgradient_method                                                      quadratic
                                * Affine_scaling                                           function
             Interior_point     * Ellipsoid_algorithm_of_Khachiyan                         with
Linear and                      * Projective_algorithm_of_Karmarkar                        unique
quadratic                       * Simplex_algorithm_of_Dantzig                             maximum.]
             Basis-exchange     * Revised_simplex_algorithm
                                * Criss-cross_algorithm
                                * Principal_pivoting_algorithm_of_Lemke
Combinatorial
                  * Approximation_algorithm
                  * Dynamic programming
Paradigms         * Greedy_algorithm
                  * Integer_programming
                        o Branch_and_bound/cut
                                * BellmanâFord
                                * BorÅ¯vka
Graph         Minimum           * Dijkstra
algorithms    spanning_tree     * FloydâWarshall
                                * Johnson
                                * Kruskal
                  * Dinic
Network_flows     * EdmondsâKarp
                  * FordâFulkerson
                  * Pushârelabel_maximum_flow
Metaheuristics
    * Evolutionary_algorithm
    * Hill_climbing
    * Local_search
    * Simulated_annealing
    * Tabu_search
    * Software
    * v
    * t
    * e
Parsing_algorithms
                   * LL
Top-down           * Recursive_descent
                         o Tail_recursive
                         o Pratt_parser
                   * Precedence
                         o Simple
                         o Operator
                               # Shunting-yard
                   * Bounded-context
                   * LR
Bottom-up                o Simple
                         o Look-ahead
                         o Canonical
                         o Generalized
                   * CYK
                   * Recursive_ascent
                   * Shift-reduce
                   * Combinator
Mixed/Other        * Chart
                   * Earley
                   * PEG
                   * Definite_clause_grammar
                   * Dynamic programming
                   * Memoization
                   * Parser_generator
Related topics           o LALR
                   * Metacompiler
                   * Parse_tree
                   * AST
                   * Scannerless_parsing
                   * History_of_compiler_construction
                   * Comparison_of_parser_generators
Authority_control [Edit_this_at_Wikidata]     * GND: 4125677-3
                                              * NDL: 00571739

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Dynamic_programming&oldid=908656970"
Categories:
    * Dynamic_programming
    * Optimization_algorithms_and_methods
    * Equations
    * Systems_engineering
    * Optimal_control
Hidden categories:
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_July_2019
    * Articles_with_permanently_dead_external_links
    * Articles_needing_additional_references_from_April_2014
    * All_articles_needing_additional_references
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_June_2009
    * Articles_needing_additional_references_from_May_2013
    * Wikipedia_external_links_cleanup_from_March_2016
    * Wikipedia_spam_cleanup_from_March_2016
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LietuviÅ³
    * à´®à´²à´¯à´¾à´³à´
    * æ¥æ¬èª
    * Norsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Svenska
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 31 July 2019, at 03:54 (UTC).
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
