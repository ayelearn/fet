The following text has been accessed from https://en.wikipedia.org/wiki/Linear_programming at Fri Aug 9 03:17:27 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Linear programming ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
A pictorial representation of a simple linear program with two variables and
six inequalities. The set of feasible solutions is depicted in yellow and forms
a polygon, a 2-dimensional polytope. The linear cost function is represented by
the red line and the arrow: The red line is a level_set of the cost function,
and the arrow indicates the direction in which we are optimizing.
A closed feasible region of a problem with three variables is a convex
polyhedron. The surfaces giving a fixed value of the objective function are
planes (not shown). The linear programming problem is to find a point on the
polyhedron that is on the plane with the highest possible value.
Linear programming (LP, also called linear optimization) is a method to achieve
the best outcome (such as maximum profit or lowest cost) in a mathematical
model whose requirements are represented by linear_relationships. Linear
programming is a special case of mathematical programming (also known as
mathematical_optimization).
More formally, linear programming is a technique for the optimization of a
linear objective_function, subject to linear_equality and linear_inequality
constraints. Its feasible_region is a convex_polytope, which is a set defined
as the intersection of finitely many half_spaces, each of which is defined by a
linear inequality. Its objective function is a real-valued affine_(linear)
function defined on this polyhedron. A linear programming algorithm finds a
point in the polyhedron where this function has the smallest (or largest) value
if such a point exists.
Linear programs are problems that can be expressed in canonical_form as
               Maximize       c    T     x        subject to     A  x  &#x2264;
      b        and      x  &#x2265;  0        {\displaystyle {\begin{aligned}&
      {\text{Maximize}}&&\mathbf {c} ^{\mathrm {T} }\mathbf {x} \\&{\text
      {subject to}}&&A\mathbf {x} \leq \mathbf {b} \\&{\text{and}}&&\mathbf {x}
      \geq \mathbf {0} \end{aligned}}}  [{\displaystyle {\begin{aligned}&{\text
      {Maximize}}&&\mathbf {c} ^{\mathrm {T} }\mathbf {x} \\&{\text{subject
      to}}&&A\mathbf {x} \leq \mathbf {b} \\&{\text{and}}&&\mathbf {x} \geq
      \mathbf {0} \end{aligned}}}]
where x represents the vector of variables (to be determined), c and b are
vectors of (known) coefficients, A is a (known) matrix of coefficients, and
( &#x22C5;  )   T      {\displaystyle (\cdot )^{\mathrm {T} }}  [(\cdot )^
{\mathrm {T} }] is the matrix_transpose. The expression to be maximized or
minimized is called the objective_function (cTx in this case). The inequalities
Ax â¤ b and x â¥ 0 are the constraints which specify a convex_polytope over
which the objective function is to be optimized. In this context, two vectors
are comparable when they have the same dimensions. If every entry in the first
is less-than or equal-to the corresponding entry in the second, then it can be
said that the first vector is less-than or equal-to the second vector.
Linear programming can be applied to various fields of study. It is widely used
in mathematics, and to a lesser extent in business, economics, and for some
engineering problems. Industries that use linear programming models include
transportation, energy, telecommunications, and manufacturing. It has proven
useful in modeling diverse types of problems in planning, routing, scheduling,
assignment, and design.
⁰
***** Contents *****
    * 1_History
    * 2_Uses
    * 3_Standard_form
          o 3.1_Example
    * 4_Augmented_form_(slack_form)
          o 4.1_Example
    * 5_Duality
    * 6_Variations
          o 6.1_Covering/packing_dualities
                # 6.1.1_Examples
    * 7_Complementary_slackness
    * 8_Theory
          o 8.1_Existence_of_optimal_solutions
          o 8.2_Optimal_vertices_(and_rays)_of_polyhedra
    * 9_Algorithms
          o 9.1_Basis_exchange_algorithms
                # 9.1.1_Simplex_algorithm_of_Dantzig
                # 9.1.2_Criss-cross_algorithm
          o 9.2_Interior_point
                # 9.2.1_Ellipsoid_algorithm,_following_Khachiyan
                # 9.2.2_Projective_algorithm_of_Karmarkar
                # 9.2.3_Affine_scaling
                # 9.2.4_Vaidya's_algorithm
                # 9.2.5_Path-following_algorithms
          o 9.3_Comparison_of_interior-point_methods_and_simplex_algorithms
          o 9.4_Approximate_algorithms_for_covering/packing_LPs
    * 10_Open_problems_and_recent_work
    * 11_Integer_unknowns
    * 12_Integral_linear_programs
    * 13_Solvers_and_scripting_(programming)_languages
    * 14_See_also
    * 15_Notes
    * 16_References
    * 17_Further_reading
    * 18_External_links
***** History[edit] *****
Leonid_Kantorovich
John_von_Neumann
The problem of solving a system of linear inequalities dates back at least as
far as Fourier, who in 1827 published a method for solving them,[1] and after
whom the method of FourierâMotzkin_elimination is named.
In 1939 a linear programming formulation of a problem that is equivalent to the
general linear programming problem was given by the Soviet economist Leonid
Kantorovich, who also proposed a method for solving it.[2] It is a way he
developed, during World_War_II, to plan expenditures and returns in order to
reduce costs of the army and to increase losses imposed on the enemy.[citation
needed] Kantorovich's work was initially neglected in the USSR.[3] About the
same time as Kantorovich, the Dutch-American economist T._C._Koopmans
formulated classical economic problems as linear programs. Kantorovich and
Koopmans later shared the 1975 Nobel_prize_in_economics.[1] In 1941, Frank
Lauren_Hitchcock also formulated transportation problems as linear programs and
gave a solution very similar to the later simplex_method.[2] Hitchcock had died
in 1957 and the Nobel prize is not awarded posthumously.
During 1946â1947, George_B._Dantzig independently developed general linear
programming formulation to use for planning problems in US Air Force[4]. In
1947, Dantzig also invented the simplex_method that for the first time
efficiently tackled the linear programming problem in most cases[4]. When
Dantzig arranged a meeting with John_von_Neumann to discuss his simplex method,
Neumann immediately conjectured the theory of duality by realizing that the
problem he had been working in game_theory was equivalent[4]. Dantzig provided
formal proof in an unpublished report "A Theorem on Linear Inequalities" on
January 5, 1948.[3] In the post-war years, many industries applied it in their
daily planning.
Dantzig's original example was to find the best assignment of 70 people to 70
jobs. The computing power required to test all the permutations to select the
best assignment is vast; the number of possible configurations exceeds the
number_of_particles in the observable_universe. However, it takes only a moment
to find the optimum solution by posing the problem as a linear program and
applying the simplex_algorithm. The theory behind linear programming
drastically reduces the number of possible solutions that must be checked.
The linear programming problem was first shown to be solvable in polynomial
time by Leonid_Khachiyan in 1979,[5] but a larger theoretical and practical
breakthrough in the field came in 1984 when Narendra_Karmarkar introduced a new
interior-point_method for solving linear-programming problems.[6]
***** Uses[edit] *****
Linear programming is a widely used field of optimization for several reasons.
Many practical problems in operations_research can be expressed as linear
programming problems.[3] Certain special cases of linear programming, such as
network_flow problems and multicommodity_flow_problems are considered important
enough to have generated much research on specialized algorithms for their
solution. A number of algorithms for other types of optimization problems work
by solving LP problems as sub-problems. Historically, ideas from linear
programming have inspired many of the central concepts of optimization theory,
such as duality, decomposition, and the importance of convexity and its
generalizations. Likewise, linear programming was heavily used in the early
formation of microeconomics and it is currently utilized in company management,
such as planning, production, transportation, technology and other issues.
Although the modern management issues are ever-changing, most companies would
like to maximize_profits and minimize costs with limited resources. Therefore,
many issues can be characterized as linear programming problems.
***** Standard form[edit] *****
Standard form is the usual and most intuitive form of describing a linear
programming problem. It consists of the following three parts:
    * A linear function to be maximized
      e.g.     f (  x  1   ,  x  2   ) =  c  1    x  1   +  c  2    x  2
      {\displaystyle f(x_{1},x_{2})=c_{1}x_{1}+c_{2}x_{2}}  [f(x_{1},x_{2})=c_
      {1}x_{1}+c_{2}x_{2}]
    * Problem constraints of the following form
      e.g.
                    a  11    x  1   +  a  12    x  2     &#x2264;  b  1
            a  21    x  1   +  a  22    x  2     &#x2264;  b  2        a  31
            x  1   +  a  32    x  2     &#x2264;  b  3         {\displaystyle
            {\begin{matrix}a_{11}x_{1}+a_{12}x_{2}&\leq b_{1}\\a_{21}x_{1}+a_
            {22}x_{2}&\leq b_{2}\\a_{31}x_{1}+a_{32}x_{2}&\leq b_{3}\\\end
            {matrix}}}  [{\begin{matrix}a_{11}x_{1}+a_{12}x_{2}&\leq b_{1}\\a_
            {21}x_{1}+a_{22}x_{2}&\leq b_{2}\\a_{31}x_{1}+a_{32}x_{2}&\leq b_
            {3}\\\end{matrix}}]
    * Non-negative variables
      e.g.
                    x  1   &#x2265; 0      x  2   &#x2265; 0
            {\displaystyle {\begin{matrix}x_{1}\geq 0\\x_{2}\geq 0\end
            {matrix}}}  [{\begin{matrix}x_{1}\geq 0\\x_{2}\geq 0\end{matrix}}]
The problem is usually expressed in matrix form, and then becomes:
         max {   c    T     x    |   A  x  &#x2264;  b  &#x2227;  x  &#x2265; 0
      }   {\displaystyle \max\{\mathbf {c} ^{\mathrm {T} }\mathbf {x}
      \;|\;A\mathbf {x} \leq \mathbf {b} \land \mathbf {x} \geq 0\}}  [
      {\displaystyle \max\{\mathbf {c} ^{\mathrm {T} }\mathbf {x} \;|\;A\mathbf
      {x} \leq \mathbf {b} \land \mathbf {x} \geq 0\}}]
Other forms, such as minimization problems, problems with constraints on
alternative forms, as well as problems involving negative variables can always
be rewritten into an equivalent problem in standard form.
**** Example[edit] ****
Suppose that a farmer has a piece of farm land, say L km2, to be planted with
either wheat or barley or some combination of the two. The farmer has a limited
amount of fertilizer, F kilograms, and pesticide, P kilograms. Every square
kilometer of wheat requires F1 kilograms of fertilizer and P1 kilograms of
pesticide, while every square kilometer of barley requires F2 kilograms of
fertilizer and P2 kilograms of pesticide. Let S1 be the selling price of wheat
per square kilometer, and S2 be the selling price of barley. If we denote the
area of land planted with wheat and barley by x1 and x2 respectively, then
profit can be maximized by choosing optimal values for x1 and x2. This problem
can be expressed with the following linear programming problem in the standard
form:
Maximize:      S  1
&#x22C5;  x  1   +  S  2
&#x22C5;  x  2             (maximize the revenueârevenue is the "objective
{\displaystyle S_{1}\cdot  function")
x_{1}+S_{2}\cdot x_{2}}
[S_{1}\cdot x_{1}+S_
{2}\cdot x_{2}]
                x  1   +
            x  2
            &#x2264; L
Subject to: {\displaystyle (limit on total area)
            x_{1}+x_
            {2}\leq L}
            [x_{1}+x_
            {2}\leq L]
                F  1
            &#x22C5;  x  1
            +  F  2
            &#x22C5;  x  2
            &#x2264; F
            {\displaystyle (limit on fertilizer)
            F_{1}\cdot x_
            {1}+F_{2}\cdot
            x_{2}\leq F}
            [F_{1}\cdot x_
            {1}+F_{2}\cdot
            x_{2}\leq F]
                P  1
            &#x22C5;  x  1
            +  P  2
            &#x22C5;  x  2
            &#x2264; P
            {\displaystyle (limit on pesticide)
            P_{1}\cdot x_
            {1}+P_{2}\cdot
            x_{2}\leq P}
            [P_{1}\cdot x_
            {1}+P_{2}\cdot
            x_{2}\leq P]
                x  1
            &#x2265; 0 ,
            x  2
            &#x2265; 0
            {\displaystyle (cannot plant a negative area).
            x_{1}\geq 0,x_
            {2}\geq 0}
            [x_{1}\geq
            0,x_{2}\geq 0]
In matrix form this becomes:
      maximize       [     S  1      S  2      ]     [     x  1        x  2
      ]     {\displaystyle {\begin{bmatrix}S_{1}&S_{2}\end{bmatrix}}{\begin
      {bmatrix}x_{1}\\x_{2}\end{bmatrix}}}  [{\begin{bmatrix}S_{1}&S_{2}\end
      {bmatrix}}{\begin{bmatrix}x_{1}\\x_{2}\end{bmatrix}}]
      subject to       [    1   1      F  1      F  2        P  1      P  2
      ]     [     x  1        x  2      ]   &#x2264;   [    L     F     P    ]
      ,    [     x  1        x  2      ]   &#x2265;   [    0     0    ]   .
      {\displaystyle {\begin{bmatrix}1&1\\F_{1}&F_{2}\\P_{1}&P_{2}\end
      {bmatrix}}{\begin{bmatrix}x_{1}\\x_{2}\end{bmatrix}}\leq {\begin
      {bmatrix}L\\F\\P\end{bmatrix}},\,{\begin{bmatrix}x_{1}\\x_{2}\end
      {bmatrix}}\geq {\begin{bmatrix}0\\0\end{bmatrix}}.}  [{\begin
      {bmatrix}1&1\\F_{1}&F_{2}\\P_{1}&P_{2}\end{bmatrix}}{\begin{bmatrix}x_
      {1}\\x_{2}\end{bmatrix}}\leq {\begin{bmatrix}L\\F\\P\end{bmatrix}},\,
      {\begin{bmatrix}x_{1}\\x_{2}\end{bmatrix}}\geq {\begin{bmatrix}0\\0\end
      {bmatrix}}.]
***** Augmented form (slack form)[edit] *****
Linear programming problems can be converted into an augmented form in order to
apply the common form of the simplex_algorithm. This form introduces non-
negative slack_variables to replace inequalities with equalities in the
constraints. The problems can then be written in the following block_matrix
form:
      Maximize     z   {\displaystyle z}  [z]:
           [    1   &#x2212;   c   T     0     0    A     I     ]     [    z
      x       s     ]   =   [    0      b     ]     {\displaystyle {\begin
      {bmatrix}1&-\mathbf {c} ^{T}&0\\0&\mathbf {A} &\mathbf {I} \end{bmatrix}}
      {\begin{bmatrix}z\\\mathbf {x} \\\mathbf {s} \end{bmatrix}}={\begin
      {bmatrix}0\\\mathbf {b} \end{bmatrix}}}  [{\begin{bmatrix}1&-\mathbf {c}
      ^{T}&0\\0&\mathbf {A} &\mathbf {I} \end{bmatrix}}{\begin
      {bmatrix}z\\\mathbf {x} \\\mathbf {s} \end{bmatrix}}={\begin
      {bmatrix}0\\\mathbf {b} \end{bmatrix}}]
          x  &#x2265; 0 ,  s  &#x2265; 0   {\displaystyle \mathbf {x} \geq
      0,\mathbf {s} \geq 0}  [\mathbf {x} \geq 0,\mathbf {s} \geq 0]
where      s    {\displaystyle \mathbf {s} }  [\mathbf {s} ] are the newly
introduced slack variables,      x    {\displaystyle \mathbf {x} }  [\mathbf
{x} ] are the decision variables, and     z   {\displaystyle z}  [z] is the
variable to be maximized.
**** Example[edit] ****
The example above is converted into the following augmented form:
      Maximize:      S  1   &#x22C5;  x  1   +  S  2
      &#x22C5;  x  2     {\displaystyle S_{1}\cdot x_    (objective function)
      {1}+S_{2}\cdot x_{2}}  [S_{1}\cdot x_{1}+S_
      {2}\cdot x_{2}]
                      x  1   +  x  2   +  x  3   = L
      subject to: {\displaystyle x_{1}+x_{2}+x_{3}=L}    (augmented constraint)
                  [x_{1}+x_{2}+x_{3}=L]
                      F  1   &#x22C5;  x  1   +  F  2
                  &#x22C5;  x  2   +  x  4   = F
                  {\displaystyle F_{1}\cdot x_{1}+F_     (augmented constraint)
                  {2}\cdot x_{2}+x_{4}=F}  [F_{1}\cdot
                  x_{1}+F_{2}\cdot x_{2}+x_{4}=F]
                      P  1   &#x22C5;  x  1   +  P  2
                  &#x22C5;  x  2   +  x  5   = P
                  {\displaystyle P_{1}\cdot x_{1}+P_     (augmented constraint)
                  {2}\cdot x_{2}+x_{5}=P}  [P_{1}\cdot
                  x_{1}+P_{2}\cdot x_{2}+x_{5}=P]
                      x  1   ,  x  2   ,  x  3   ,  x  4
                  ,  x  5   &#x2265; 0.   {\displaystyle
                  x_{1},x_{2},x_{3},x_{4},x_{5}\geq 0.}
                  [{\displaystyle x_{1},x_{2},x_{3},x_
                  {4},x_{5}\geq 0.}]
where      x  3   ,  x  4   ,  x  5     {\displaystyle x_{3},x_{4},x_{5}}  [x_
{3},x_{4},x_{5}] are (non-negative) slack variables, representing in this
example the unused area, the amount of unused fertilizer, and the amount of
unused pesticide.
In matrix form this becomes:
      Maximize     z   {\displaystyle z}  [z]:
           [    1   &#x2212;  S  1     &#x2212;  S  2     0   0   0     0   1
      1   1   0   0     0    F  1      F  2     0   1   0     0    P  1      P
      2     0   0   1    ]     [    z      x  1        x  2        x  3
      x  4        x  5      ]   =   [    0     L     F     P    ]   ,
      [     x  1        x  2        x  3        x  4        x  5      ]
      &#x2265; 0.   {\displaystyle {\begin{bmatrix}1&-S_{1}&-S_
      {2}&0&0&0\\0&1&1&1&0&0\\0&F_{1}&F_{2}&0&1&0\\0&P_{1}&P_{2}&0&0&1\\\end
      {bmatrix}}{\begin{bmatrix}z\\x_{1}\\x_{2}\\x_{3}\\x_{4}\\x_{5}\end
      {bmatrix}}={\begin{bmatrix}0\\L\\F\\P\end{bmatrix}},\,{\begin{bmatrix}x_
      {1}\\x_{2}\\x_{3}\\x_{4}\\x_{5}\end{bmatrix}}\geq 0.}  [{\begin
      {bmatrix}1&-S_{1}&-S_{2}&0&0&0\\0&1&1&1&0&0\\0&F_{1}&F_{2}&0&1&0\\0&P_
      {1}&P_{2}&0&0&1\\\end{bmatrix}}{\begin{bmatrix}z\\x_{1}\\x_{2}\\x_{3}\\x_
      {4}\\x_{5}\end{bmatrix}}={\begin{bmatrix}0\\L\\F\\P\end{bmatrix}},\,
      {\begin{bmatrix}x_{1}\\x_{2}\\x_{3}\\x_{4}\\x_{5}\end{bmatrix}}\geq 0.]
***** Duality[edit] *****
Main article: Dual_linear_program
Every linear programming problem, referred to as a primal problem, can be
converted into a dual_problem, which provides an upper bound to the optimal
value of the primal problem. In matrix form, we can express the primal problem
as:
      Maximize cTx subject to Ax â¤ b, x â¥ 0;
            with the corresponding symmetric dual problem,
      Minimize bTy subject to ATy â¥ c, y â¥ 0.
An alternative primal formulation is:
      Maximize cTx subject to Ax â¤ b;
            with the corresponding asymmetric dual problem,
      Minimize bTy subject to ATy = c, y â¥ 0.
There are two ideas fundamental to duality theory. One is the fact that (for
the symmetric dual) the dual of a dual linear program is the original primal
linear program. Additionally, every feasible solution for a linear program
gives a bound on the optimal value of the objective function of its dual. The
weak_duality theorem states that the objective function value of the dual at
any feasible solution is always greater than or equal to the objective function
value of the primal at any feasible solution. The strong_duality theorem states
that if the primal has an optimal solution, x*, then the dual also has an
optimal solution, y*, and cTx*=bTy*.
A linear program can also be unbounded or infeasible. Duality theory tells us
that if the primal is unbounded then the dual is infeasible by the weak duality
theorem. Likewise, if the dual is unbounded, then the primal must be
infeasible. However, it is possible for both the dual and the primal to be
infeasible. See dual_linear_program for details and several more examples.
***** Variations[edit] *****
**** Covering/packing dualities[edit] ****
Covering/packing-problem_pairs
Covering_problems    Packing_problems
Minimum_set_cover    Maximum_set_packing
Minimum_vertex_cover Maximum_matching
Minimum_edge_cover   Maximum_independent_set
    * v
    * t
    * e
A covering_LP is a linear program of the form:
      Minimize: bTy,
      subject to: ATy â¥ c, y â¥ 0,
such that the matrix A and the vectors b and c are non-negative.
The dual of a covering LP is a packing_LP, a linear program of the form:
      Maximize: cTx,
      subject to: Ax â¤ b, x â¥ 0,
such that the matrix A and the vectors b and c are non-negative.
*** Examples[edit] ***
Covering and packing LPs commonly arise as a linear_programming_relaxation of a
combinatorial problem and are important in the study of approximation
algorithms.[7] For example, the LP relaxations of the set_packing_problem, the
independent_set_problem, and the matching_problem are packing LPs. The LP
relaxations of the set_cover_problem, the vertex_cover_problem, and the
dominating_set_problem are also covering LPs.
Finding a fractional_coloring of a graph is another example of a covering LP.
In this case, there is one constraint for each vertex of the graph and one
variable for each independent_set of the graph.
***** Complementary slackness[edit] *****
It is possible to obtain an optimal solution to the dual when only an optimal
solution to the primal is known using the complementary slackness theorem. The
theorem states:
Suppose that x = (x1, x2, ... , xn) is primal feasible and that y = 
(y1, y2, ... , ym) is dual feasible. Let (w1, w2, ..., wm) denote the
corresponding primal slack variables, and let (z1, z2, ... , zn) denote the
corresponding dual slack variables. Then x and y are optimal for their
respective problems if and only if
    * xj zj = 0, for j = 1, 2, ... , n, and
    * wi yi = 0, for i = 1, 2, ... , m.
So if the i-th slack variable of the primal is not zero, then the i-th variable
of the dual is equal to zero. Likewise, if the j-th slack variable of the dual
is not zero, then the j-th variable of the primal is equal to zero.
This necessary condition for optimality conveys a fairly simple economic
principle. In standard form (when maximizing), if there is slack in a
constrained primal resource (i.e., there are "leftovers"), then additional
quantities of that resource must have no value. Likewise, if there is slack in
the dual (shadow) price non-negativity constraint requirement, i.e., the price
is not zero, then there must be scarce supplies (no "leftovers").
***** Theory[edit] *****
**** Existence of optimal solutions[edit] ****
Geometrically, the linear constraints define the feasible_region, which is a
convex polyhedron. A linear_function is a convex_function, which implies that
every local_minimum is a global_minimum; similarly, a linear function is a
concave_function, which implies that every local_maximum is a global_maximum.
An optimal solution need not exist, for two reasons. First, if two constraints
are inconsistent, then no feasible solution exists: For instance, the
constraints x â¥ 2 and x â¤ 1 cannot be satisfied jointly; in this case, we
say that the LP is infeasible. Second, when the polytope is unbounded in the
direction of the gradient of the objective function (where the gradient of the
objective function is the vector of the coefficients of the objective
function), then no optimal value is attained because it is always possible to
do better than any finite value of the objective function.
**** Optimal vertices (and rays) of polyhedra[edit] ****
Otherwise, if a feasible solution exists and if the constraint set is bounded,
then the optimum value is always attained on the boundary of the constraint
set, by the maximum_principle for convex_functions (alternatively, by the
minimum principle for concave_functions) since linear functions are both convex
and concave. However, some problems have distinct optimal solutions; for
example, the problem of finding a feasible solution to a system of linear
inequalities is a linear programming problem in which the objective function is
the zero function (that is, the constant function taking the value zero
everywhere). For this feasibility problem with the zero-function for its
objective-function, if there are two distinct solutions, then every convex
combination of the solutions is a solution.
The vertices of the polytope are also called basic feasible solutions. The
reason for this choice of name is as follows. Let d denote the number of
variables. Then the fundamental theorem of linear inequalities implies (for
feasible problems) that for every vertex x* of the LP feasible region, there
exists a set of d (or fewer) inequality constraints from the LP such that, when
we treat those d constraints as equalities, the unique solution is x*. Thereby
we can study these vertices by means of looking at certain subsets of the set
of all constraints (a discrete set), rather than the continuum of LP solutions.
This principle underlies the simplex_algorithm for solving linear programs.
***** Algorithms[edit] *****
See also: List_of_numerical_analysis_topics_Â§ Linear_programming
In a linear programming problem, a series of linear constraints produces a
convex feasible_region of possible values for those variables. In the two-
variable case this region is in the shape of a convex simple_polygon.
**** Basis exchange algorithms[edit] ****
*** Simplex algorithm of Dantzig[edit] ***
The simplex_algorithm, developed by George_Dantzig in 1947, solves LP problems
by constructing a feasible solution at a vertex of the polytope and then
walking along a path on the edges of the polytope to vertices with non-
decreasing values of the objective function until an optimum is reached for
sure. In many practical problems, "stalling" occurs: many pivots are made with
no increase in the objective function.[8][9] In rare practical problems, the
usual versions of the simplex algorithm may actually "cycle".[9] To avoid
cycles, researchers developed new pivoting rules.[10][11][8][9][12][13]
In practice, the simplex algorithm is quite efficient and can be guaranteed to
find the global optimum if certain precautions against cycling are taken. The
simplex algorithm has been proved to solve "random" problems efficiently, i.e.
in a cubic number of steps,[14] which is similar to its behavior on practical
problems.[8][15]
However, the simplex algorithm has poor worst-case behavior: Klee and Minty
constructed a family of linear programming problems for which the simplex
method takes a number of steps exponential in the problem size.[8][11][12] In
fact, for some time it was not known whether the linear programming problem was
solvable in polynomial_time, i.e. of complexity_class_P.
*** Criss-cross algorithm[edit] ***
Like the simplex algorithm of Dantzig, the criss-cross_algorithm is a basis-
exchange algorithm that pivots between bases. However, the criss-cross
algorithm need not maintain feasibility, but can pivot rather from a feasible
basis to an infeasible basis. The criss-cross algorithm does not have
polynomial_time-complexity for linear programming. Both algorithms visit
all 2D corners of a (perturbed) cube in dimension D, the KleeâMinty_cube, in
the worst_case.[13][16]
**** Interior point[edit] ****
In contrast to the simplex algorithm, which finds an optimal solution by
traversing the edges between vertices on a polyhedral set, interior-point
methods move through the interior of the feasible region.
*** Ellipsoid algorithm, following Khachiyan[edit] ***
This is the first worst-case polynomial-time algorithm ever found for linear
programming. To solve a problem which has n variables and can be encoded in L
input bits, this algorithm uses O(n4L) pseudo-arithmetic operations on numbers
with O(L) digits. Leonid_Khachiyan solved this long-standing complexity issue
in 1979 with the introduction of the ellipsoid_method. The convergence analysis
has (real-number) predecessors, notably the iterative_methods developed by Naum
Z._Shor and the approximation_algorithms by Arkadi Nemirovski and D. Yudin.
*** Projective algorithm of Karmarkar[edit] ***
Main article: Karmarkar's_algorithm
Khachiyan's algorithm was of landmark importance for establishing the
polynomial-time solvability of linear programs. The algorithm was not a
computational break-through, as the simplex method is more efficient for all
but specially constructed families of linear programs.
However, Khachiyan's algorithm inspired new lines of research in linear
programming. In 1984, N._Karmarkar proposed a projective_method for linear
programming. Karmarkar's algorithm improved on Khachiyan's worst-case
polynomial bound (giving     O (  n  3.5   L )   {\displaystyle O(n^{3.5}L)}
[O(n^{3.5}L)]). Karmarkar claimed that his algorithm was much faster in
practical LP than the simplex method, a claim that created great interest in
interior-point methods.[17] Since Karmarkar's discovery, many interior-point
methods have been proposed and analyzed.
*** Affine scaling[edit] ***
Main article: Affine_scaling
Affine scaling is one of the oldest interior point methods to be developed. It
was developed in the Soviet Union in the mid-1960s, but didn't receive much
attention until the discovery of Karmarkar's algorithm, after which affine
scaling was reinvented_multiple_times and presented as a simplified version of
Karmarkar's. Affine scaling amounts to doing gradient_descent steps within the
feasible region, while rescaling the problem to make sure the steps move toward
the optimum faster.[18]
*** Vaidya's algorithm[edit] ***
In 1989, Vaidya developed an algorithm that runs in     O (  n  2.5   )
{\displaystyle O(n^{2.5})}  [O(n^{2.5})] time.[19] Formally speaking, the
algorithm takes     O ( ( n + d  )  1.5   n L )   {\displaystyle O((n+d)^
{1.5}nL)}  [{\displaystyle O((n+d)^{1.5}nL)}] arithmetic operations in the
worst case, where     d   {\displaystyle d}  [d] is the number of constraints,
n   {\displaystyle n}  [n] is the number of variables, and     L
{\displaystyle L}  [L] is the number of bits.
*** Path-following algorithms[edit] ***
For both theoretical and practical purposes, barrier_function or path-following
methods have been the most popular interior point methods since the 1990s.[20]
In 2015, Lee and Sidford showed that, it can be solved in     O ( ( n n z ( A )
+  n  2   )   n   )   {\displaystyle O((nnz(A)+n^{2}){\sqrt {n}})}  [
{\displaystyle O((nnz(A)+n^{2}){\sqrt {n}})}] time,[21] and it remains taking
O (  n  2.5   )   {\displaystyle O(n^{2.5})}  [O(n^{2.5})] in the worst case.
In 2018, Cohen, Lee and Song improved the running time to     O (  n  &#x03C9;
)   {\displaystyle O(n^{\omega })}  [{\displaystyle O(n^{\omega })}] time,
&#x03C9;   {\displaystyle \omega }  [\omega ] is the exponent of matrix
multiplication.[22]
**** Comparison of interior-point methods and simplex algorithms[edit] ****
The current opinion is that the efficiencies of good implementations of
simplex-based methods and interior point methods are similar for routine
applications of linear programming.[20] However, for specific types of LP
problems, it may be that one type of solver is better than another (sometimes
much better), and that the structure of the solutions generated by interior
point methods versus simplex-based methods are significantly different with the
support set of active variables being typically smaller for the later one.[23]
**** Approximate algorithms for covering/packing LPs[edit] ****
Covering and packing LPs can be solved approximately in nearly-linear time.
That is, if matrix A is of dimension nÃm and has N non-zero entries, then
there exist algorithms that run in time O(NÂ·(log N)O(1)/ÎµO(1)) and produce O
(1Â±Îµ) approximate solutions to given covering and packing LPs. The best known
sequential algorithm of this kind runs in time O(N + (log N)Â·(n+m)/Îµ2),[24]
and the best known parallel algorithm of this kind runs in O((log N)2/Îµ3)
iterations, each requiring only a matrix-vector multiplication which is highly
parallelizable.[25]
***** Open problems and recent work[edit] *****
                                 Unsolved problem in computer science:
[Question, Web Fundamentals.svg] Does linear programming admit a strongly
                                 polynomial-time algorithm?
                                 (more_unsolved_problems_in_computer_science)
There are several open problems in the theory of linear programming, the
solution of which would represent fundamental breakthroughs in mathematics and
potentially major advances in our ability to solve large-scale linear programs.
    * Does LP admit a strongly_polynomial-time algorithm?
    * Does LP admit a strongly polynomial-time algorithm to find a strictly
      complementary solution?
    * Does LP admit a polynomial-time algorithm in the real number (unit cost)
      model of computation?
This closely related set of problems has been cited by Stephen_Smale as among
the 18_greatest_unsolved_problems of the 21st century. In Smale's words, the
third version of the problem "is the main unsolved problem of linear
programming theory." While algorithms exist to solve linear programming in
weakly polynomial time, such as the ellipsoid_methods and interior-point
techniques, no algorithms have yet been found that allow strongly polynomial-
time performance in the number of constraints and the number of variables. The
development of such algorithms would be of great theoretical interest, and
perhaps allow practical gains in solving large LPs as well.
Although the Hirsch_conjecture was recently disproved for higher dimensions, it
still leaves the following questions open.
    * Are there pivot rules which lead to polynomial-time simplex variants?
    * Do all polytopal graphs have polynomially bounded diameter?
These questions relate to the performance analysis and development of simplex-
like methods. The immense efficiency of the simplex algorithm in practice
despite its exponential-time theoretical performance hints that there may be
variations of simplex that run in polynomial or even strongly polynomial time.
It would be of great practical and theoretical significance to know whether any
such variants exist, particularly as an approach to deciding if LP can be
solved in strongly polynomial time.
The simplex algorithm and its variants fall in the family of edge-following
algorithms, so named because they solve linear programming problems by moving
from vertex to vertex along edges of a polytope. This means that their
theoretical performance is limited by the maximum number of edges between any
two vertices on the LP polytope. As a result, we are interested in knowing the
maximum graph-theoretical_diameter of polytopal graphs. It has been proved that
all polytopes have subexponential diameter. The recent disproof of the Hirsch
conjecture is the first step to prove whether any polytope has superpolynomial
diameter. If any such polytopes exist, then no edge-following variant can run
in polynomial time. Questions about polytope diameter are of independent
mathematical interest.
Simplex pivot methods preserve primal (or dual) feasibility. On the other hand,
criss-cross pivot methods do not preserve (primal or dual) feasibilityâthey
may visit primal feasible, dual feasible or primal-and-dual infeasible bases in
any order. Pivot methods of this type have been studied since the 1970s.
[citation_needed] Essentially, these methods attempt to find the shortest pivot
path on the arrangement_polytope under the linear programming problem. In
contrast to polytopal graphs, graphs of arrangement polytopes are known to have
small diameter, allowing the possibility of strongly polynomial-time criss-
cross pivot algorithm without resolving questions about the diameter of general
polytopes.[13]
***** Integer unknowns[edit] *****
If all of the unknown variables are required to be integers, then the problem
is called an integer_programming (IP) or integer linear programming (ILP)
problem. In contrast to linear programming, which can be solved efficiently in
the worst case, integer programming problems are in many practical situations
(those with bounded variables) NP-hard. 0â1 integer programming or binary
integer programming (BIP) is the special case of integer programming where
variables are required to be 0 or 1 (rather than arbitrary integers). This
problem is also classified as NP-hard, and in fact the decision version was one
of Karp's_21_NP-complete_problems.
If only some of the unknown variables are required to be integers, then the
problem is called a mixed integer programming (MIP) problem. These are
generally also NP-hard because they are even more general than ILP programs.
There are however some important subclasses of IP and MIP problems that are
efficiently solvable, most notably problems where the constraint matrix is
totally_unimodular and the right-hand sides of the constraints are integers or
â more general â where the system has the total_dual_integrality (TDI)
property.
Advanced algorithms for solving integer linear programs include:
    * cutting-plane_method
    * Branch_and_bound
    * Branch_and_cut
    * Branch_and_price
    * if the problem has some extra structure, it may be possible to apply
      delayed_column_generation.
Such integer-programming algorithms are discussed by Padberg and in Beasley.
***** Integral linear programs[edit] *****
A linear program in real variables is said to be integral if it has at least
one optimal solution which is integral. Likewise, a polyhedron     P = { x
&#x2223; A x &#x2265; 0 }   {\displaystyle P=\{x\mid Ax\geq 0\}}  [P=\{x\mid
Ax\geq 0\}] is said to be integral if for all bounded feasible objective
functions c, the linear program     { max c x &#x2223; x &#x2208; P }
{\displaystyle \{\max cx\mid x\in P\}}  [\{\max cx\mid x\in P\}] has an optimum
x  &#x2217;     {\displaystyle x^{*}}  [x^{*}] with integer coordinates. As
observed by Edmonds and Giles in 1977, one can equivalently say that the
polyhedron     P   {\displaystyle P}  [P] is integral if for every bounded
feasible integral objective function c, the optimal value of the linear program
{ max c x &#x2223; x &#x2208; P }   {\displaystyle \{\max cx\mid x\in P\}}  [\
{\max cx\mid x\in P\}] is an integer.
Integral linear programs are of central importance in the polyhedral aspect of
combinatorial_optimization since they provide an alternate characterization of
a problem. Specifically, for any problem, the convex hull of the solutions is
an integral polyhedron; if this polyhedron has a nice/compact description, then
we can efficiently find the optimal feasible solution under any linear
objective. Conversely, if we can prove that a linear_programming_relaxation is
integral, then it is the desired description of the convex hull of feasible
(integral) solutions.
Note that terminology is not consistent throughout the literature, so one
should be careful to distinguish the following two concepts,
    * in an integer linear program, described in the previous section,
      variables are forcibly constrained to be integers, and this problem is
      NP-hard in general,
    * in an integral linear program, described in this section, variables are
      not constrained to be integers but rather one has proven somehow that the
      continuous problem always has an integral optimal value (assuming c is
      integral), and this optimal value may be found efficiently since all
      polynomial-size linear programs can be solved in polynomial time.
One common way of proving that a polyhedron is integral is to show that it is
totally_unimodular. There are other general methods including the integer
decomposition_property and total_dual_integrality. Other specific well-known
integral LPs include the matching polytope, lattice polyhedra, submodular flow
polyhedra, and the intersection of 2 generalized polymatroids/g-polymatroids
â e.g. see Schrijver 2003.
A bounded integral polyhedron is sometimes called a convex_lattice_polytope,
particularly in two dimensions.
***** Solvers and scripting (programming) languages[edit] *****
Permissive licenses:
Name  License Brief info
Pyomo BSD     An open-source modeling language for large-scale linear, mixed
              integer and nonlinear optimization
Copyleft_(reciprocal) licenses:
Name                        License Brief info
                                    an incremental constraint solving toolkit
Cassowary_constraint_solver LGPL    that efficiently solves systems of linear
                                    equalities and inequalities
CLP                         CPL     an LP solver from COIN-OR
                                    GNU Linear Programming Kit, an LP/MILP
                                    solver with a native C API and numerous
glpk                        GPL     (15) third-party wrappers for other
                                    languages. Specialist support for flow
                                    networks. Bundles the AMPL-like GNU
                                    MathProg modelling language and translator.
                                    a library for incrementally solving systems
Qoca                        GPL     of linear equations with various goal
                                    functions
                                    a programming language and software
R-Project                   GPL     environment for statistical computing and
                                    graphics
MINTO (Mixed Integer Optimizer, an integer_programming solver which uses branch
and bound algorithm) has publicly available source code[26] but is not open
source.
Proprietary licenses:
Name                     Brief info
                         A modeling language that allows to model linear, mixed
                         integer, and nonlinear optimization models. It also
                         offers a tool for constraint programming. Algorithm,
AIMMS                    in the forms of heuristics or exact methods, such as
                         Branch-and-Cut or Column Generation, can also be
                         implemented. The tool calls an appropriate solver such
                         as CPLEX, Gurobi or similar, to solve the optimization
                         problem at hand. Academic licenses are free of charge.
                         A popular modeling language for large-scale linear,
AMPL                     mixed integer and nonlinear optimisation with a free
                         student limited version available (500 variables and
                         500 constraints).
                         API to MATLAB and Python. Solve example Linear
APMonitor                Programming_(LP)_problems through MATLAB, Python, or a
                         web-interface.
                         Popular solver with an API for several programming
CPLEX                    languages, and also has a modelling language and works
                         with AIMMS, AMPL, GAMS, MPL, OpenOpt, OPL Development
                         Studio, and TOMLAB. Free for academic use.
                         A nonlinear solver adjusted to spreadsheets in which
Excel Solver Function    function evaluations are based on the recalculating
                         cells. Basic version available as a standard add-on
                         for Excel.
FortMP
GAMS
                         Solver with parallel algorithms for large-scale linear
Gurobi                   programs, quadratic programs and mixed-integer
                         programs. Free for academic use.
                         Collections of math and statistical algorithms
                         available in C/C++, Fortran, Java and C#/.NET.
IMSL_Numerical_Libraries Optimization routines in the IMSL Libraries include
                         unconstrained, linearly and nonlinearly constrained
                         minimizations, and linear programming algorithms.
                         Solver with an API for large scale optimization of
                         linear, integer, quadratic, conic and general
                         nonlinear programs with stochastic programming
                         extensions. It offers a global optimization procedure
                         for finding guaranteed globally optimal solution to
LINDO                    general nonlinear programs with continuous and
                         discrete variables. It also has a statistical sampling
                         API to integrate Monte-Carlo simulations into an
                         optimization framework. It has an algebraic modeling
                         language (LINGO) and allows modeling within a
                         spreadsheet (What'sBest).
Maple                    A general-purpose programming-language for symbolic
                         and numerical computing.
                         A general-purpose and matrix-oriented programming-
                         language for numerical computing. Linear programming
MATLAB                   in MATLAB requires the Optimization_Toolbox in
                         addition to the base MATLAB product; available
                         routines include INTLINPROG and LINPROG
Mathcad                  A WYSIWYG math editor. It has functions for solving
                         both linear and nonlinear optimization problems.
                         A general-purpose programming-language for
Mathematica              mathematics, including symbolic and numerical
                         capabilities.
MOSEK                    A solver for large scale optimization with API for
                         several languages (C++,java,.net, Matlab and python).
                         A collection of mathematical and statistical routines
                         developed by the Numerical_Algorithms_Group for
                         multiple programming languages (C, C++, Fortran,
                         Visual Basic, Java and C#) and packages (MATLAB,
                         Excel, R, LabVIEW). The Optimization chapter of the
                         NAG Library includes routines for linear programming
NAG_Numerical_Library    problems with both sparse and non-sparse linear
                         constraint matrices, together with routines for the
                         optimization of quadratic, nonlinear, sums of squares
                         of linear or nonlinear functions with nonlinear,
                         bounded or no constraints. The NAG Library has
                         routines for both local and global optimization, and
                         for continuous or integer problems.
NMath_Stats              A general-purpose .NET statistical library containing
                         a simplex solver.[27]
OptimJ                   A Java-based modeling language for optimization with a
                         free version available.[28][29]
                         A suite of solvers for Linear, Integer, Nonlinear,
                         Derivative-Free, Network, Combinatorial and Constraint
SAS/OR                   Optimization; the Algebraic_modeling_language
                         OPTMODEL; and a variety of vertical solutions aimed at
                         specific problems/markets, all of which are fully
                         integrated with the SAS_System.
                         A general-purpose constraint integer programming
SCIP                     solver with an emphasis on MIP. Compatible with Zimpl
                         modelling language. Free for academic use and
                         available in source code.
                         Solver for large-scale linear programs, quadratic
                         programs, general nonlinear and mixed-integer
XPRESS                   programs. Has API for several programming languages,
                         also has a modelling language Mosel and works with
                         AMPL, GAMS. Free for academic use.
VisSim                   A visual block_diagram language for simulation of
                         dynamical_systems.
***** See also[edit] *****
    * Convex_programming
    * Dynamic_programming
    * Expected_shortfall#Optimization_of_expected_shortfall
    * Inputâoutput_model
    * Job_shop_scheduling
    * Linear-fractional_programming_(LFP)
    * LP-type_problem
    * Mathematical_programming
    * Nonlinear_programming
    * Oriented_matroid
    * Quadratic_programming, a superset of linear programming
    * Semidefinite_programming
    * Shadow_price
    * Simplex_algorithm, used to solve LP problems
***** Notes[edit] *****
   1. ^ a bGerard Sierksma; Yori Zwols (2015). Linear and Integer Optimization:
      Theory and Practice, Third Edition. CRC Press. p. 1. ISBN 9781498710169.
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
   3. ^ a bAlexander Schrijver (1998). Theory of Linear and Integer
      Programming. John Wiley & Sons. pp. 221â222. ISBN 978-0-471-98232-6.
   4. ^ a b cGeorge B. Dantzig (April 1982). "Reminiscences_about_the_origins
      of_linear_programming". Operations Research Letters. 1 (2): 43â48. doi:
      10.1016/0167-6377(82)90043-8.
   5. ^ a b cDantzig, George B. (George Bernard), 1914-2005. (Â©1997-2003).
      Linear programming. Thapa, Mukund Narain. New York: Springer. pp. xxvii.
      ISBN 0387948333. OCLC 35318475.Check date values in: |date= (help)CS1
      maint: Multiple names: authors list (link)
   6. ^Leonid Khachiyan (1979). "A Polynomial Algorithm for Linear
      Programming". Doklady Akademii Nauk SSSR. 224 (5): 1093â1096.
   7. ^Narendra Karmarkar (1984). "A New Polynomial-Time Algorithm for Linear
      Programming". Combinatorica. 4 (4): 373â395. doi:10.1007/BF02579150.
   8. ^ Vazirani_(2001, p. 112)
   9. ^ a b c d Dantzig_&_Thapa_(2003)
  10. ^ a b c Padberg_(1999)
  11. ^ Bland_(1977)
  12. ^ a b Murty_(1983)
  13. ^ a b Papadimitriou_&_Steiglitz
  14. ^ a b c Fukuda_&_Terlaky_(1997):Fukuda, Komei; Terlaky, TamÃ¡s (1997).
      Thomas M. Liebling and Dominique de Werra (eds.). "Criss-cross methods: A
      fresh view on pivot algorithms". Mathematical Programming, Series B. 79
      (1â3): 369â395. CiteSeerX 10.1.1.36.9373. doi:10.1007/BF02614325.
      MR 1464775.CS1 maint: Uses editors parameter (link)
  15. ^ Borgwardt_(1987)
  16. ^ Todd_(2002)
  17. ^ Roos_(1990):Roos, C. (1990). "An exponential example for Terlaky's
      pivoting rule for the criss-cross simplex method". Mathematical
      Programming. Series A. 46 (1): 79â84. doi:10.1007/BF01585729.
      MR 1045573.
  18. ^Strang,_Gilbert (1 June 1987). "Karmarkar's algorithm and its place in
      applied mathematics". The_Mathematical_Intelligencer. 9 (2): 4â10. doi:
      10.1007/BF03025891. ISSN 0343-6993. MR 0883185.
  19. ^ Vanderbei_(2001, pp. 333â347)
  20. ^Vaidya, Pravin M. (1989). Speeding-up_linear_programming_using_fast
      matrix_multiplication. 30th Annual Symposium on Foun- dations of Computer
      Science (FOCS'89).
  21. ^ a b Gondzio_&_Terlaky_(1996)
  22. ^Lee, Yin-Tat; Sidford, Aaron (2015). Efficient inverse maintenance and
      faster algorithms for linear programming. FOCS '15 Foundations of
      Computer Science. arXiv:1503.01752.
  23. ^Cohen, Michael B.; Lee, Yin-Tat; Song, Zhao (2018). Solving Linear
      Programs in the Current Matrix Multiplication Time. arXiv:1810.07896.
  24. ^IllÃ©s, Tibor; Terlaky, TamÃ¡s (2002). "Pivot_versus_interior_point
      methods:_Pros_and_cons". European Journal of Operational Research. 140
      (2): 170. CiteSeerX 10.1.1.646.3539. doi:10.1016/S0377-2217(02)00061-9.
  25. ^Christos Koufogiannakis; Neal E. Young (2013). "A Nearly Linear-Time
      PTAS for Explicit Fractional Packing and Covering Linear Programs".
      Algorithmica. 70 (4): 648â674. arXiv:0801.1987. doi:10.1007/s00453-013-
      9771-6.
  26. ^Zeyuan Allen-Zhu; Lorenzo Orecchia (2015). Using Optimization to Break
      the Epsilon Barrier: A Faster and Simpler Width-Independent Algorithm for
      Solving Positive Linear Programs in Parallel. ACM-SIAM Symposium on
      Discrete Algorithms. arXiv:1407.1925. Bibcode:2014arXiv1407.1925A.
  27. ^"COR@L_â_Computational_Optimization_Research_At_Lehigh". lehigh.edu.
  28. ^"C#_Linear_Programming". centerspace.net.
  29. [permanent_dead_link]
  30. ^ http://www.in-ter-trans.eu/resources/
      Zesch_Hellingrath_2010_Integrated+Production-Distribution+Planning.pdf
      OptimJ used in an optimization model for mixed-model assembly lines,
      University of MÃ¼nster
  31. ^ http://www.aaai.org/ocs/index.php/AAAI/AAAI10/paper/viewFile/1769/2076
      OptimJ used in an Approximate Subgame-Perfect Equilibrium Computation
      Technique for Repeated Games
***** References[edit] *****
    * Kantorovich, L. V. (1940). "ÐÐ± Ð¾Ð´Ð½Ð¾Ð¼ ÑÑÑÐµÐºÑÐ¸Ð²Ð½Ð¾Ð¼
      Ð¼ÐµÑÐ¾Ð´Ðµ ÑÐµÑÐµÐ½Ð¸Ñ Ð½ÐµÐºÐ¾ÑÐ¾ÑÑÑ ÐºÐ»Ð°ÑÑÐ¾Ð²
      ÑÐºÑÑÑÐµÐ¼Ð°Ð»ÑÐ½ÑÑ Ð¿ÑÐ¾Ð±Ð»ÐµÐ¼" [A new method of solving some
      classes of extremal problems]. Doklady_Akad_Sci_SSSR. 28: 211â214.
F. L. Hitchcock: The_distribution_of_a_product_from_several_sources_to_numerous
localities, Journal of Mathematics and Physics, 20, 1941, 224â230.
G.B Dantzig: Maximization_of_a_linear_function_of_variables_subject_to_linear
inequalities, 1947. Published pp. 339â347 in T.C. Koopmans (ed.):Activity
Analysis of Production and Allocation, New York-London 1951 (Wiley & Chapman-
Hall)
J. E. Beasley, editor. Advances in Linear and Integer Programming. Oxford
Science, 1996. (Collection of surveys)
Bland, Robert G. (1977). "New Finite Pivoting Rules for the Simplex Method".
Mathematics of Operations Research. 2 (2): 103â107. doi:10.1287/moor.2.2.103.
JSTOR 3689647.
Karl-Heinz Borgwardt, The Simplex Algorithm: A Probabilistic Analysis,
Algorithms and Combinatorics, Volume 1, Springer-Verlag, 1987. (Average
behavior on random problems)
Richard W. Cottle, ed. The Basic George B. Dantzig. Stanford Business Books,
Stanford University Press, Stanford, California, 2003. (Selected papers by
George_B._Dantzig)
George B. Dantzig and Mukund N. Thapa. 1997. Linear programming 1:
Introduction. Springer-Verlag.
George B. Dantzig and Mukund N. Thapa. 2003. Linear Programming 2: Theory and
Extensions. Springer-Verlag. (Comprehensive, covering e.g. pivoting and
interior-point algorithms, large-scale problems, decomposition_following
DantzigâWolfe and Benders, and introducing stochastic_programming.)
Edmonds, Jack; Giles, Rick (1977). "A Min-Max Relation for Submodular Functions
on Graphs". Studies in Integer Programming. Annals of Discrete Mathematics. 1.
pp. 185â204. doi:10.1016/S0167-5060(08)70734-9. ISBN 978-0-7204-0765-5.
Fukuda, Komei; Terlaky, TamÃ¡s (1997). Thomas M. Liebling and Dominique
de Werra (eds.). "Criss-cross methods: A fresh view on pivot algorithms".
Mathematical Programming, Series B. 79 (1â3): 369â395.
CiteSeerX 10.1.1.36.9373. doi:10.1007/BF02614325. MR 1464775.CS1 maint: Uses
editors parameter (link)
Gondzio, Jacek; Terlaky, TamÃ¡s (1996). "3_A_computational_view_of_interior
point_methods". In J. E. Beasley (ed.). Advances in linear and integer
programming. Oxford Lecture Series in Mathematics and its Applications. 4. New
York: Oxford University Press. pp. 103â144. MR 1438311. Postscript_file_at
website_of_Gondzio and at_McMaster_University_website_of_Terlaky.
Murty,_Katta G. (1983). Linear programming. New York: John Wiley & Sons, Inc.
pp. xix+482. ISBN 978-0-471-09725-9. MR 0720547. (comprehensive reference to
classical approaches).
Evar D. Nering and Albert_W._Tucker, 1993, Linear Programs and Related
Problems, Academic Press. (elementary)
M. Padberg, Linear Optimization and Extensions, Second Edition, Springer-
Verlag, 1999. (carefully written account of primal and dual simplex algorithms
and projective algorithms, with an introduction to integer linear programming
â featuring the traveling_salesman_problem for Odysseus.)
Christos_H._Papadimitriou and Kenneth Steiglitz, Combinatorial Optimization:
Algorithms and Complexity, Corrected republication with a new preface, Dover.
(computer science)
Michael J. Todd (February 2002). "The many facets of linear programming".
Mathematical Programming. 91 (3): 417â436. doi:10.1007/s101070100261.
 (Invited survey, from the International Symposium on Mathematical
Programming.)
Vanderbei, Robert J. (2001). Linear Programming: Foundations and Extensions.
Springer Verlag.
Vazirani,_Vijay_V. (2001). Approximation Algorithms. Springer-Verlag. ISBN 978-
3-540-65367-7.
 (Computer science)
***** Further reading[edit] *****
Library_resources about
Linear programming
===============================================================================
    * Resources_in_your_library
A reader may consider beginning with Nering and Tucker, with the first volume
of Dantzig and Thapa, or with Williams.
    * Dmitris Alevras and Manfred W. Padberg, Linear_Optimization_and
      Extensions:_Problems_and_Solutions, Universitext, Springer-Verlag, 2001.
      (Problems from Padberg with solutions.)
    * Mark de Berg, Marc van Kreveld, Mark_Overmars, and Otfried Schwarzkopf
      (2000). Computational Geometry (2nd revised ed.). Springer-Verlag.
      ISBN 978-3-540-65620-3.CS1 maint: Multiple names: authors list (link)
 Chapter 4: Linear Programming: pp. 63â94. Describes a randomized half-plane
intersection algorithm for linear programming.
Michael_R._Garey and David_S._Johnson (1979). Computers_and_Intractability:_A
Guide_to_the_Theory_of_NP-Completeness. W.H. Freeman. ISBN 978-0-7167-1045-5.
 A6: MP1: INTEGER PROGRAMMING, pg.245. (computer science, complexity theory)
Bernd GÃ¤rtner and JiÅÃ­_MatouÅ¡ek (2006). Understanding and Using Linear
Programming. Berlin: Springer. ISBN 3-540-30697-8.
 (elementary introduction for mathematicians and computer scientists)
Cornelis Roos, TamÃ¡s Terlaky, Jean-Philippe Vial, Interior Point Methods for
Linear Optimization, Second Edition, Springer-Verlag, 2006. (Graduate level)
Alexander Schrijver (2003). Combinatorial optimization: polyhedra and
efficiency. Springer.
Alexander Schrijver, Theory of Linear and Integer Programming. John Wiley &
sons, 1998,
ISBN 0-471-98232-6 (mathematical)
Gerard Sierksma; Yori Zwols (2015). Linear and Integer Optimization: Theory and
Practice. CRC Press. ISBN 978-1-498-71016-9.
Gerard Sierksma; Diptesh Ghosh (2010). Networks in Action; Text and Computer
Exercises in Network Optimization. Springer. ISBN 978-1-4419-5512-8.
 (linear optimization modeling)
H. P. Williams, Model_Building_in_Mathematical_Programming, Fifth Edition,
2013. (Modeling)
Stephen J. Wright, 1997, Primal-Dual_Interior-Point_Methods, SIAM. (Graduate
level)
Yinyu_Ye, 1997, Interior Point Algorithms: Theory and Analysis, Wiley.
(Advanced graduate-level)
Ziegler,_GÃ¼nter_M., Chapters 1â3 and 6â7 in Lectures on Polytopes,
Springer-Verlag, New York, 1994. (Geometry)
***** External links[edit] *****
 Wikimedia Commons has media related to Linear_programming.
    * Guidance_On_Formulating_LP_Problems
    * Mathematical_Programming_Glossary
    * The_Linear_Programming_FAQ
    * Benchmarks_For_Optimisation_Software
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
                  * Dynamic_programming
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
Complementarity_problems_and_algorithms
                              * Linear programming (LP)
                              * Quadratic_programming_(QP)
Complementarity Problems      * Linear_complementarity_problem_(LCP)
                              * Mixed_linear_(MLCP)
                              * Mixed_(MCP)
                              * Nonlinear(NCP)
                              * Simplex (Dantzig)
Basis-exchange_algorithms     * Revised_simplex
                              * Criss-cross
                              * Lemke
Authority_control [Edit_this_at_Wikidata]     * GND: 4035816-1
                                              * NDL: 00570683

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Linear_programming&oldid=909323112"
Categories:
    * Linear_programming
    * Convex_optimization
    * Geometric_algorithms
    * P-complete_problems
Hidden categories:
    * CS1_errors:_dates
    * CS1_maint:_Multiple_names:_authors_list
    * CS1_maint:_Uses_editors_parameter
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_December_2017
    * Articles_with_permanently_dead_external_links
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_August_2017
    * Articles_with_unsourced_statements_from_February_2019
    * Commons_category_link_from_Wikidata
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
    * Wikiquote
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * à´®à´²à´¯à´¾à´³à´
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Sicilianu
    * Simple_English
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
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
    * This page was last edited on 4 August 2019, at 17:37 (UTC).
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
