The following text has been accessed from https://en.wikipedia.org/wiki/Simplex_algorithm at Fri Aug 9 02:38:00 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Simplex algorithm ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the linear programming algorithm. For the non-linear
optimization heuristic, see NelderâMead_method.
In mathematical_optimization, Dantzig's simplex algorithm (or simplex method)
is a popular algorithm for linear_programming.[1]
The name of the algorithm is derived from the concept of a simplex and was
suggested by T._S._Motzkin.[2] Simplices are not actually used in the method,
but one interpretation of it is that it operates on simplicial cones, and these
become proper simplices with an additional constraint.[3][4][5][6] The
simplicial cones in question are the corners (i.e., the neighborhoods of the
vertices) of a geometric object called a polytope. The shape of this polytope
is defined by the constraints applied to the objective function.
⁰
***** Contents *****
    * 1_Overview
    * 2_History
    * 3_Standard_form
    * 4_Simplex_tableau
    * 5_Pivot_operations
    * 6_Algorithm
          o 6.1_Entering_variable_selection
          o 6.2_Leaving_variable_selection
          o 6.3_Example
    * 7_Finding_an_initial_canonical_tableau
          o 7.1_Example
    * 8_Advanced_topics
          o 8.1_Implementation
          o 8.2_Degeneracy:_stalling_and_cycling
          o 8.3_Efficiency
    * 9_Other_algorithms
    * 10_Linear-fractional_programming
    * 11_See_also
    * 12_Notes
    * 13_References
    * 14_Further_reading
    * 15_External_links
***** Overview[edit] *****
Further information: Linear_programming
A system_of_linear_inequalities defines a polytope as a feasible region. The
simplex algorithm begins at a starting vertex and moves along the edges of the
polytope until it reaches the vertex of the optimal solution.
Polyhedron of simplex algorithm in 3D
The simplex algorithm operates on linear programs in the canonical_form
      maximize       c  T     x    {\textstyle \mathbf {c^{T}} \mathbf {x} }  [
      {\textstyle \mathbf {c^{T}} \mathbf {x} }]
      subject to     A  x  &#x2264;  b    {\displaystyle A\mathbf {x} \leq
      \mathbf {b} }  [{\displaystyle A\mathbf {x} \leq \mathbf {b} }] and
      x  &#x2265; 0   {\displaystyle \mathbf {x} \geq 0}  [{\displaystyle
      \mathbf {x} \geq 0}]
with      x  = (  x  1   ,  &#x2026; ,   x  n   )   {\displaystyle \mathbf {x}
=(x_{1},\,\dots ,\,x_{n})}  [{\displaystyle \mathbf {x} =(x_{1},\,\dots ,\,x_
{n})}] the variables of the problem,      c  = (  c  1   ,  &#x2026; ,   c  n
)   {\displaystyle \mathbf {c} =(c_{1},\,\dots ,\,c_{n})}  [{\displaystyle
\mathbf {c} =(c_{1},\,\dots ,\,c_{n})}] the coefficients of the objective
function,     A   {\displaystyle A}  [A] a pÃn matrix, and      b  = (  b  1
,  &#x2026; ,   b  p   )   {\displaystyle \mathbf {b} =(b_{1},\,\dots ,\,b_
{p})}  [{\displaystyle \mathbf {b} =(b_{1},\,\dots ,\,b_{p})}] nonnegative
constants (    &#x2200; j ,  b  j   &#x2265; 0 &#xA0;   {\displaystyle \forall
j,b_{j}\geq 0\ }  [{\displaystyle \forall j,b_{j}\geq 0\ }]). There is a
straightforward process to convert any linear program into one in standard
form, so using this form of linear programs results in no loss of generality.
In geometric terms, the feasible_region defined by all values of      x
{\displaystyle \mathbf {x} }  [\mathbf {x} ] such that     A  x  &#x2264;  b
{\textstyle A\mathbf {x} \leq \mathbf {b} }  [{\textstyle A\mathbf {x} \leq
\mathbf {b} }] and     &#x2200; i ,  x  i   &#x2265; 0   {\displaystyle \forall
i,x_{i}\geq 0}  [{\displaystyle \forall i,x_{i}\geq 0}] is a (possibly
unbounded) convex_polytope. An extreme point or vertex of this polytope is
known as basic_feasible_solution (BFS).
It can be shown that for a linear program in standard form, if the objective
function has a maximum value on the feasible region, then it has this value on
(at least) one of the extreme points.[7] This in itself reduces the problem to
a finite computation since there is a finite number of extreme points, but the
number of extreme points is unmanageably large for all but the smallest linear
programs.[8]
It can also be shown that, if an extreme point is not a maximum point of the
objective function, then there is an edge containing the point so that the
objective function is strictly increasing on the edge moving away from the
point.[9] If the edge is finite, then the edge connects to another extreme
point where the objective function has a greater value, otherwise the objective
function is unbounded above on the edge and the linear program has no solution.
The simplex algorithm applies this insight by walking along edges of the
polytope to extreme points with greater and greater objective values. This
continues until the maximum value is reached, or an unbounded edge is visited
(concluding that the problem has no solution). The algorithm always terminates
because the number of vertices in the polytope is finite; moreover since we
jump between vertices always in the same direction (that of the objective
function), we hope that the number of vertices visited will be small.[9]
The solution of a linear program is accomplished in two steps. In the first
step, known as Phase I, a starting extreme point is found. Depending on the
nature of the program this may be trivial, but in general it can be solved by
applying the simplex algorithm to a modified version of the original program.
The possible results of Phase I are either that a basic feasible solution is
found or that the feasible region is empty. In the latter case the linear
program is called infeasible. In the second step, Phase II, the simplex
algorithm is applied using the basic feasible solution found in Phase I as a
starting point. The possible results from Phase II are either an optimum basic
feasible solution or an infinite edge on which the objective function is
unbounded above.[10][11][12]
***** History[edit] *****
George Dantzig worked on planning methods for the US Army Air Force during
World War II using a desk calculator. During 1946 his colleague challenged him
to mechanize the planning process to distract him from taking another job.
Dantzig formulated the problem as linear inequalities inspired by the work of
Wassily_Leontief, however, at that time he didn't include an objective as part
of his formulation. Without an objective, a vast number of solutions can be
feasible, and therefore to find the "best" feasible solution, military-
specified "ground rules" must be used that describe how goals can be achieved
as opposed to specifying a goal itself. Dantzig's core insight was to realize
that most such ground rules can be translated into a linear objective function
that needs to be maximized.[13] Development of the simplex method was
evolutionary and happened over a period of about a year.[14]
After Dantzig included an objective function as part of his formulation during
mid-1947, the problem was mathematically more tractable. Dantzig realized that
one of the unsolved problems that he_had_mistaken as homework in his professor
Jerzy_Neyman's class (and actually later solved), was applicable to finding an
algorithm for linear programs. This problem involved finding the existence of
Lagrange_multipliers for general linear programs over a continuum of variables,
each bounded between zero and one, and satisfying linear constraints expressed
in the form of Lebesgue_integrals. Dantzig later published his "homework" as a
thesis to earn his doctorate. The column geometry used in this thesis gave
Dantzig insight that made him believe that the Simplex method would be very
efficient.[15]
***** Standard form[edit] *****
The transformation of a linear program to one in standard form may be
accomplished as follows.[16] First, for each variable with a lower bound other
than 0, a new variable is introduced representing the difference between the
variable and bound. The original variable can then be eliminated by
substitution. For example, given the constraint
          x  1   &#x2265; 5   {\displaystyle x_{1}\geq 5}  [x_{1}\geq 5]
a new variable,      y  1     {\displaystyle y_{1}}  [y_{1}], is introduced
with
              y  1   =  x  1   &#x2212; 5      x  1   =  y  1   + 5
      {\displaystyle {\begin{aligned}y_{1}=x_{1}-5\\x_{1}=y_{1}+5\end
      {aligned}}}  [{\begin{aligned}y_{1}=x_{1}-5\\x_{1}=y_{1}+5\end{aligned}}]
The second equation may be used to eliminate      x  1     {\displaystyle x_
{1}}  [x_{1}] from the linear program. In this way, all lower bound constraints
may be changed to non-negativity restrictions.
Second, for each remaining inequality constraint, a new variable, called a
slack variable, is introduced to change the constraint to an equality
constraint. This variable represents the difference between the two sides of
the inequality and is assumed to be non-negative. For example, the inequalities
              x  2   + 2  x  3      &#x2264; 3     &#x2212;  x  4   + 3  x  5
      &#x2265; 2       {\displaystyle {\begin{aligned}x_{2}+2x_{3}&\leq 3\\-x_
      {4}+3x_{5}&\geq 2\end{aligned}}}  [{\begin{aligned}x_{2}+2x_{3}&\leq 3\\-
      x_{4}+3x_{5}&\geq 2\end{aligned}}]
are replaced with
              x  2   + 2  x  3   +  s  1      = 3     &#x2212;  x  4   + 3  x
      5   &#x2212;  s  2      = 2      s  1   ,   s  2      &#x2265; 0
      {\displaystyle {\begin{aligned}x_{2}+2x_{3}+s_{1}&=3\\-x_{4}+3x_{5}-s_
      {2}&=2\\s_{1},\,s_{2}&\geq 0\end{aligned}}}  [{\begin{aligned}x_{2}+2x_
      {3}+s_{1}&=3\\-x_{4}+3x_{5}-s_{2}&=2\\s_{1},\,s_{2}&\geq 0\end{aligned}}]
It is much easier to perform algebraic manipulation on inequalities in this
form. In inequalities where â¥ appears such as the second one, some authors
refer to the variable introduced as a surplus variable.
Third, each unrestricted variable is eliminated from the linear program. This
can be done in two ways, one is by solving for the variable in one of the
equations in which it appears and then eliminating the variable by
substitution. The other is to replace the variable with the difference of two
restricted variables. For example, if      z  1     {\displaystyle z_{1}}  [z_
{1}] is unrestricted then write
               z  1   =  z  1   +   &#x2212;  z  1   &#x2212;         z  1   +
      ,   z  1   &#x2212;   &#x2265; 0       {\displaystyle {\begin{aligned}&z_
      {1}=z_{1}^{+}-z_{1}^{-}\\&z_{1}^{+},\,z_{1}^{-}\geq 0\end{aligned}}}  [
      {\begin{aligned}&z_{1}=z_{1}^{+}-z_{1}^{-}\\&z_{1}^{+},\,z_{1}^{-}\geq
      0\end{aligned}}]
The equation may be used to eliminate      z  1     {\displaystyle z_{1}}  [z_
{1}] from the linear program.
When this process is complete the feasible region will be in the form
          A   x  =  b  ,  &#x2200; i &#xA0;  x  i   &#x2265; 0   {\displaystyle
      \mathbf {A} \mathbf {x} =\mathbf {b} ,\,\forall i\ x_{i}\geq 0}  [
      {\displaystyle \mathbf {A} \mathbf {x} =\mathbf {b} ,\,\forall i\ x_
      {i}\geq 0}]
It is also useful to assume that the rank of      A    {\displaystyle \mathbf
{A} }  [\mathbf {A} ] is the number of rows. This results in no loss of
generality since otherwise either the system      A   x  =  b    {\displaystyle
\mathbf {A} \mathbf {x} =\mathbf {b} }  [\mathbf {A} \mathbf {x} =\mathbf {b} ]
has redundant equations which can be dropped, or the system is inconsistent and
the linear program has no solution.[17]
***** Simplex tableau[edit] *****
A linear program in standard form can be represented as a tableau of the form
           [    1   &#x2212;   c   T     0     0    A     b     ]
      {\displaystyle {\begin{bmatrix}1&-\mathbf {c} ^{T}&0\\0&\mathbf {A}
      &\mathbf {b} \end{bmatrix}}}  [{\begin{bmatrix}1&-\mathbf {c} ^
      {T}&0\\0&\mathbf {A} &\mathbf {b} \end{bmatrix}}]
The first row defines the objective function and the remaining rows specify the
constraints. The zero in the first column represents the zero vector of the
same dimension as vector b.(Note, different authors use different conventions
as to the exact layout.) If the columns of A can be rearranged so that it
contains the identity_matrix of order p (the number of rows in A) then the
tableau is said to be in canonical form.[18] The variables corresponding to the
columns of the identity matrix are called basic variables while the remaining
variables are called nonbasic or free variables. If the values of the nonbasic
variables are set to 0, then the values of the basic variables are easily
obtained as entries in b and this solution is a basic feasible solution. The
algebraic interpretation here is that the coefficients of the linear equation
represented by each row are either     0   {\displaystyle 0}  [{\displaystyle
0}],     1   {\displaystyle 1}  [1], or some other number. Each row will have
1   {\displaystyle 1}  [1] column with value     1   {\displaystyle 1}  [1],
p &#x2212; 1   {\displaystyle p-1}  [p-1] columns with coefficients     0
{\displaystyle 0}  [{\displaystyle 0}], and the remaining columns with some
other coefficients (these other variables represent our non-basic variables).
By setting the values of the non-basic variables we ensure in each row that the
value of the variable represented by a     1   {\displaystyle 1}  [1] in its
column is equal to the     b   {\displaystyle b}  [b] value at that row.
Conversely, given a basic feasible solution, the columns corresponding to the
nonzero variables can be expanded to a nonsingular matrix. If the corresponding
tableau is multiplied by the inverse of this matrix then the result is a
tableau in canonical form.[19]
Let
           [    1   &#x2212;   c   B   T     &#x2212;   c   D   T     0     0
      I    D     b     ]     {\displaystyle {\begin{bmatrix}1&-\mathbf {c} _
      {B}^{T}&-\mathbf {c} _{D}^{T}&0\\0&I&\mathbf {D} &\mathbf {b} \end
      {bmatrix}}}  [{\begin{bmatrix}1&-\mathbf {c} _{B}^{T}&-\mathbf {c} _{D}^
      {T}&0\\0&I&\mathbf {D} &\mathbf {b} \end{bmatrix}}]
be a tableau in canonical form. Additional row-addition_transformations can be
applied to remove the coefficients cT
B  from the objective function. This process is called pricing out and results
in a canonical tableau
           [    1   0   &#x2212;      c  &#x00AF;     D   T      z  B       0
      I    D     b     ]     {\displaystyle {\begin{bmatrix}1&0&-{\bar {\mathbf
      {c} }}_{D}^{T}&z_{B}\\0&I&\mathbf {D} &\mathbf {b} \end{bmatrix}}}  [
      {\begin{bmatrix}1&0&-{\bar {\mathbf {c} }}_{D}^{T}&z_{B}\\0&I&\mathbf {D}
      &\mathbf {b} \end{bmatrix}}]
where zB is the value of the objective function at the corresponding basic
feasible solution. The updated coefficients, also known as relative cost
coefficients, are the rates of change of the objective function with respect to
the nonbasic variables.[11]
***** Pivot operations[edit] *****
The geometrical operation of moving from a basic feasible solution to an
adjacent basic feasible solution is implemented as a pivot operation. First, a
nonzero pivot element is selected in a nonbasic column. The row containing this
element is multiplied by its reciprocal to change this element to 1, and then
multiples of the row are added to the other rows to change the other entries in
the column to 0. The result is that, if the pivot element is in row r, then the
column becomes the r-th column of the identity matrix. The variable for this
column is now a basic variable, replacing the variable which corresponded to
the r-th column of the identity matrix before the operation. In effect, the
variable corresponding to the pivot column enters the set of basic variables
and is called the entering variable, and the variable being replaced leaves the
set of basic variables and is called the leaving variable. The tableau is still
in canonical form but with the set of basic variables changed by one element.
[10][11]
***** Algorithm[edit] *****
Let a linear program be given by a canonical tableau. The simplex algorithm
proceeds by performing successive pivot operations each of which give an
improved basic feasible solution; the choice of pivot element at each step is
largely determined by the requirement that this pivot improves the solution.
**** Entering variable selection[edit] ****
Since the entering variable will, in general, increase from 0 to a positive
number, the value of the objective function will decrease if the derivative of
the objective function with respect to this variable is negative. Equivalently,
the value of the objective function is decreased if the pivot column is
selected so that the corresponding entry in the objective row of the tableau is
positive.
If there is more than one column so that the entry in the objective row is
positive then the choice of which one to add to the set of basic variables is
somewhat arbitrary and several entering variable choice rules[20] such as Devex
algorithm[21] have been developed.
If all the entries in the objective row are less than or equal to 0 then no
choice of entering variable can be made and the solution is in fact optimal. It
is easily seen to be optimal since the objective row now corresponds to an
equation of the form
         z (  x  ) =  z  B   +  nonnegative terms corresponding to nonbasic
      variables    {\displaystyle z(\mathbf {x} )=z_{B}+{\text{nonnegative
      terms corresponding to nonbasic variables}}}  [z(\mathbf {x} )=z_{B}+
      {\text{nonnegative terms corresponding to nonbasic variables}}]
Note that by changing the entering variable choice rule so that it selects a
column where the entry in the objective row is negative, the algorithm is
changed so that it finds the maximum of the objective function rather than the
minimum.
**** Leaving variable selection[edit] ****
Once the pivot column has been selected, the choice of pivot row is largely
determined by the requirement that the resulting solution be feasible. First,
only positive entries in the pivot column are considered since this guarantees
that the value of the entering variable will be nonnegative. If there are no
positive entries in the pivot column then the entering variable can take any
nonnegative value with the solution remaining feasible. In this case the
objective function is unbounded below and there is no minimum.
Next, the pivot row must be selected so that all the other basic variables
remain positive. A calculation shows that this occurs when the resulting value
of the entering variable is at a minimum. In other words, if the pivot column
is c, then the pivot row r is chosen so that
          b  r    /   a  r c      {\displaystyle b_{r}/a_{rc}\,}  [b_{r}/a_
      {rc}\,]
is the minimum over all r so that arc > 0. This is called the minimum ratio
test.[20] If there is more than one row for which the minimum is achieved then
a dropping variable choice rule[22] can be used to make the determination.
**** Example[edit] ****
See also: Revised_simplex_algorithm_Â§ Numerical_example
Consider the linear program
      Minimize
               Z = &#x2212; 2 x &#x2212; 3 y &#x2212; 4 z    {\displaystyle Z=-
            2x-3y-4z\,}  [Z=-2x-3y-4z\,]
      Subject to
                   3 x + 2 y + z    &#x2264; 10     2 x + 5 y + 3 z    &#x2264;
            15     x ,  y ,  z    &#x2265; 0       {\displaystyle {\begin
            {aligned}3x+2y+z&\leq 10\\2x+5y+3z&\leq 15\\x,\,y,\,z&\geq 0\end
            {aligned}}}  [{\begin{aligned}3x+2y+z&\leq 10\\2x+5y+3z&\leq
            15\\x,\,y,\,z&\geq 0\end{aligned}}]
With the addition of slack variables s and t, this is represented by the
canonical tableau
           [    1   2   3   4   0   0   0     0   3   2   1   1   0   10     0
      2   5   3   0   1   15    ]     {\displaystyle {\begin
      {bmatrix}1&2&3&4&0&0&0\\0&3&2&1&1&0&10\\0&2&5&3&0&1&15\end{bmatrix}}}  [
      {\begin{bmatrix}1&2&3&4&0&0&0\\0&3&2&1&1&0&10\\0&2&5&3&0&1&15\end
      {bmatrix}}]
where columns 5 and 6 represent the basic variables s and t and the
corresponding basic feasible solution is
         x = y = z = 0 ,  s = 10 ,  t = 15.   {\displaystyle
      x=y=z=0,\,s=10,\,t=15.}  [x=y=z=0,\,s=10,\,t=15.]
Columns 2, 3, and 4 can be selected as pivot columns, for this example column 4
is selected. The values of z resulting from the choice of rows 2 and 3 as pivot
rows are 10/1 = 10 and 15/3 = 5 respectively. Of these the minimum is 5, so row
3 must be the pivot row. Performing the pivot produces
           [    3   &#x2212; 2   &#x2212; 11   0   0   &#x2212; 4   &#x2212; 60
      0   7   1   0   3   &#x2212; 1   15     0   2   5   3   0   1   15    ]
      {\displaystyle {\begin{bmatrix}3&-2&-11&0&0&-4&-60\\0&7&1&0&3&-
      1&15\\0&2&5&3&0&1&15\end{bmatrix}}}  [{\displaystyle {\begin{bmatrix}3&-
      2&-11&0&0&-4&-60\\0&7&1&0&3&-1&15\\0&2&5&3&0&1&15\end{bmatrix}}}]
Now columns 4 and 5 represent the basic variables z and s and the corresponding
basic feasible solution is
         x = y = t = 0 ,  z = 5 ,  s = 5.   {\displaystyle
      x=y=t=0,\,z=5,\,s=5.}  [x=y=t=0,\,z=5,\,s=5.]
For the next step, there are no positive entries in the objective row and in
fact
         Z =     &#x2212; 60 + 2 x + 11 y + 4 t  3    = &#x2212; 20 +     2 x +
      11 y + 4 t  3      {\displaystyle Z={\tfrac {-60+2x+11y+4t}{3}}=-20+
      {\tfrac {2x+11y+4t}{3}}}  [{\displaystyle Z={\tfrac {-60+2x+11y+4t}{3}}=-
      20+{\tfrac {2x+11y+4t}{3}}}]
so the minimum value of Z is −20.
***** Finding an initial canonical tableau[edit] *****
In general, a linear program will not be given in canonical form and an
equivalent canonical tableau must be found before the simplex algorithm can
start. This can be accomplished by the introduction of artificial variables.
Columns of the identity matrix are added as column vectors for these variables.
If the b value for a constraint equation is negative, the equation is negated
before adding the identity matrix columns. This does not change the set of
feasible solutions or the optimal solution, and it ensures that the slack
variables will constitute an initial feasible solution. The new tableau is in
canonical form but it is not equivalent to the original problem. So a new
objective function, equal to the sum of the artificial variables, is introduced
and the simplex algorithm is applied to find the minimum; the modified linear
program is called the Phase I problem.[23]
The simplex algorithm applied to the Phase I problem must terminate with a
minimum value for the new objective function since, being the sum of
nonnegative variables, its value is bounded below by 0. If the minimum is 0
then the artificial variables can be eliminated from the resulting canonical
tableau producing a canonical tableau equivalent to the original problem. The
simplex algorithm can then be applied to find the solution; this step is called
Phase II. If the minimum is positive then there is no feasible solution for the
Phase I problem where the artificial variables are all zero. This implies that
the feasible region for the original problem is empty, and so the original
problem has no solution.[10][11][24]
**** Example[edit] ****
Consider the linear program
      Minimize
               Z = &#x2212; 2 x &#x2212; 3 y &#x2212; 4 z    {\displaystyle Z=-
            2x-3y-4z\,}  [Z=-2x-3y-4z\,]
      Subject to
                   3 x + 2 y + z    = 10     2 x + 5 y + 3 z    = 15     x ,  y
            ,  z    &#x2265; 0       {\displaystyle {\begin
            {aligned}3x+2y+z&=10\\2x+5y+3z&=15\\x,\,y,\,z&\geq 0\end{aligned}}}
            [{\begin{aligned}3x+2y+z&=10\\2x+5y+3z&=15\\x,\,y,\,z&\geq 0\end
            {aligned}}]
This is represented by the (non-canonical) tableau
           [    1   2   3   4   0     0   3   2   1   10     0   2   5   3   15
      ]     {\displaystyle {\begin
      {bmatrix}1&2&3&4&0\\0&3&2&1&10\\0&2&5&3&15\end{bmatrix}}}  [{\begin
      {bmatrix}1&2&3&4&0\\0&3&2&1&10\\0&2&5&3&15\end{bmatrix}}]
Introduce artificial variables u and v and objective function W = u + v, giving
a new tableau
           [    1   0   0   0   0   &#x2212; 1   &#x2212; 1   0     0   1   2
      3   4   0   0   0     0   0   3   2   1   1   0   10     0   0   2   5
      3   0   1   15    ]     {\displaystyle {\begin{bmatrix}1&0&0&0&0&-1&-
      1&0\\0&1&2&3&4&0&0&0\\0&0&3&2&1&1&0&10\\0&0&2&5&3&0&1&15\end{bmatrix}}}
      [{\begin{bmatrix}1&0&0&0&0&-1&-
      1&0\\0&1&2&3&4&0&0&0\\0&0&3&2&1&1&0&10\\0&0&2&5&3&0&1&15\end{bmatrix}}]
Note that the equation defining the original objective function is retained in
anticipation of Phase II.
By construction, u and v are both non-basic variables since they are part of
the initial identity matrix. However, the objective function W currently
assumes that u and v are both 0. In order to adjust the objective function to
be the correct value where u = 10 and v = 15, add the third and fourth rows to
the first row giving
           [    1   0   5   7   4   0   0   25     0   1   2   3   4   0   0
      0     0   0   3   2   1   1   0   10     0   0   2   5   3   0   1   15
      ]     {\displaystyle {\begin
      {bmatrix}1&0&5&7&4&0&0&25\\0&1&2&3&4&0&0&0\\0&0&3&2&1&1&0&10\\0&0&2&5&3&0&1&15\end
      {bmatrix}}}  [{\begin
      {bmatrix}1&0&5&7&4&0&0&25\\0&1&2&3&4&0&0&0\\0&0&3&2&1&1&0&10\\0&0&2&5&3&0&1&15\end
      {bmatrix}}]
Select column 5 as a pivot column, so the pivot row must be row 4, and the
updated tableau is
           [    3   0   7   1   0   0   &#x2212; 4   15     0   3   &#x2212; 2
      &#x2212; 11   0   0   &#x2212; 4   &#x2212; 60     0   0   7   1   0   3
      &#x2212; 1   15     0   0   2   5   3   0   1   15    ]
      {\displaystyle {\begin{bmatrix}3&0&7&1&0&0&-4&15\\0&3&-2&-11&0&0&-4&-
      60\\0&0&7&1&0&3&-1&15\\0&0&2&5&3&0&1&15\end{bmatrix}}}  [{\displaystyle
      {\begin{bmatrix}3&0&7&1&0&0&-4&15\\0&3&-2&-11&0&0&-4&-60\\0&0&7&1&0&3&-
      1&15\\0&0&2&5&3&0&1&15\end{bmatrix}}}]
Now select column 3 as a pivot column, for which row 3 must be the pivot row,
to get
           [    1   0   0   0   0   &#x2212; 1   &#x2212; 1   0     0   7   0
      &#x2212; 25   0   2   &#x2212; 10   &#x2212; 130     0   0   7   1   0
      3   &#x2212; 1   15     0   0   0   11   7   &#x2212; 2   3   25    ]
      {\displaystyle {\begin{bmatrix}1&0&0&0&0&-1&-1&0\\0&7&0&-25&0&2&-10&-
      130\\0&0&7&1&0&3&-1&15\\0&0&0&11&7&-2&3&25\end{bmatrix}}}  [
      {\displaystyle {\begin{bmatrix}1&0&0&0&0&-1&-1&0\\0&7&0&-25&0&2&-10&-
      130\\0&0&7&1&0&3&-1&15\\0&0&0&11&7&-2&3&25\end{bmatrix}}}]
The artificial variables are now 0 and they may be dropped giving a canonical
tableau equivalent to the original problem:
           [    7   0   &#x2212; 25   0   &#x2212; 130     0   7   1   0   15
      0   0   11   7   25    ]     {\displaystyle {\begin{bmatrix}7&0&-25&0&-
      130\\0&7&1&0&15\\0&0&11&7&25\end{bmatrix}}}  [{\displaystyle {\begin
      {bmatrix}7&0&-25&0&-130\\0&7&1&0&15\\0&0&11&7&25\end{bmatrix}}}]
This is, fortuitously, already optimal and the optimum value for the original
linear program is â130/7.
***** Advanced topics[edit] *****
**** Implementation[edit] ****
Main article: Revised_simplex_algorithm
The tableau form used above to describe the algorithm lends itself to an
immediate implementation in which the tableau is maintained as a rectangular
(m + 1)-by-(m + n + 1) array. It is straightforward to avoid storing the m
explicit columns of the identity matrix that will occur within the tableau by
virtue of B being a subset of the columns of [A, I]. This implementation is
referred to as the "standard simplex algorithm". The storage and computation
overhead are such that the standard simplex method is a prohibitively expensive
approach to solving large linear programming problems.
In each simplex iteration, the only data required are the first row of the
tableau, the (pivotal) column of the tableau corresponding to the entering
variable and the right-hand-side. The latter can be updated using the pivotal
column and the first row of the tableau can be updated using the (pivotal) row
corresponding to the leaving variable. Both the pivotal column and pivotal row
may be computed directly using the solutions of linear systems of equations
involving the matrix B and a matrix-vector product using A. These observations
motivate the "revised_simplex_algorithm", for which implementations are
distinguished by their invertible representation of B.[25]
In large linear-programming problems A is typically a sparse_matrix and, when
the resulting sparsity of B is exploited when maintaining its invertible
representation, the revised simplex algorithm is much more efficient than the
standard simplex method. Commercial simplex solvers are based on the revised
simplex algorithm.[24][25][26][27][28]
**** Degeneracy: stalling and cycling[edit] ****
If the values of all basic variables are strictly positive, then a pivot must
result in an improvement in the objective value. When this is always the case
no set of basic variables occurs twice and the simplex algorithm must terminate
after a finite number of steps. Basic feasible solutions where at least one of
the basicvariables is zero are called degenerate and may result in pivots for
which there is no improvement in the objective value. In this case there is no
actual change in the solution but only a change in the set of basic variables.
When several such pivots occur in succession, there is no improvement; in large
industrial applications, degeneracy is common and such "stalling" is notable.
Worse than stalling is the possibility the same set of basic variables occurs
twice, in which case, the deterministic pivoting rules of the simplex algorithm
will produce an infinite loop, or "cycle". While degeneracy is the rule in
practice and stalling is common, cycling is rare in practice. A discussion of
an example of practical cycling occurs in Padberg.[24] Bland's_rule prevents
cycling and thus guarantees that the simplex algorithm always terminates.[24]
[29][30] Another pivoting algorithm, the criss-cross_algorithm never cycles on
linear programs.[31]
History-based pivot rules such as Zadeh's_rule and Cunningham's_rule also try
to circumvent the issue of stalling and cycling by keeping track how often
particular variables are being used, and then favor such variables that have
been used least often.
**** Efficiency[edit] ****
The simplex method is remarkably efficient in practice and was a great
improvement over earlier methods such as FourierâMotzkin_elimination.
However, in 1972, Klee and Minty[32] gave an example, the KleeâMinty_cube,
showing that the worst-case complexity of simplex method as formulated by
Dantzig is exponential_time. Since then, for almost every variation on the
method, it has been shown that there is a family of linear programs for which
it performs badly. It is an open question if there is a variation with
polynomial_time, although sub-exponential pivot rules are known.[33]
In 2018, it was proved that a particular variant of the simplex method is NP-
mighty, i.e., it can be used to solve, with polynomial overhead, any problem in
NP implicitly during the algorithm's execution. Moreover, deciding whether a
given variable ever enters the basis during the algorithm's execution on a
given input, and determining the number of iterations needed for solving a
given problem, are both NP-hard problems.[34] Computing the output of some
other pivot rules was already known to be PSPACE-complete[35][36].
Analyzing and quantifying the observation that the simplex algorithm is
efficient in practice despite its exponential worst-case complexity has led to
the development of other measures of complexity. The simplex algorithm has
polynomial-time average-case_complexity under various probability
distributions, with the precise average-case performance of the simplex
algorithm depending on the choice of a probability distribution for the random
matrices.[37][38] Another approach to studying "typical_phenomena" uses Baire
category_theory from general_topology, and to show that (topologically) "most"
matrices can be solved by the simplex algorithm in a polynomial number of
steps.[citation_needed] Another method to analyze the performance of the
simplex algorithm studies the behavior of worst-case scenarios under small
perturbation â are worst-case scenarios stable under a small change (in the
sense of structural_stability), or do they become tractable? This area of
research, called smoothed_analysis, was introduced specifically to study the
simplex method. Indeed, the running time of the simplex method on input with
noise is polynomial in the number of variables and the magnitude of the
perturbations.[39]
***** Other algorithms[edit] *****
Other algorithms for solving linear-programming problems are described in the
linear-programming article. Another basis-exchange pivoting algorithm is the
criss-cross_algorithm.[40][41] There are polynomial-time algorithms for linear
programming that use interior point methods: these include Khachiyan's
ellipsoidal_algorithm, Karmarkar's projective_algorithm, and path-following
algorithms.[12]
***** Linear-fractional programming[edit] *****
Main article: Linear-fractional_programming
Linearâfractional_programming (LFP) is a generalization of linear_programming
(LP). In LP the objective function is a linear_function, while the objective
function of a linearâfractional program is a ratio of two linear functions.
In other words, a linear program is a fractionalâlinear program in which the
denominator is the constant function having the value one everywhere. A
linearâfractional program can be solved by a variant of the simplex algorithm
[42][43][44][45] or by the criss-cross_algorithm.[46]
***** See also[edit] *****
    * Criss-cross_algorithm
    * Cutting-plane_method
    * Devex_algorithm
    * FourierâMotzkin_elimination
    * Karmarkar's_algorithm
    * NelderâMead_simplicial_heuristic
    * Pivoting_rule_of_Bland, which avoids cycling
***** Notes[edit] *****
   1. ^Murty,_Katta_G. Linear_programming. John Wiley & Sons Inc.1, 2000.
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
   3. ^ Murty_(1983, Comment 2.2)
   4. ^ Murty_(1983, Note 3.9)
   5. ^Stone, Richard E.; Tovey, Craig A. (1991). "The simplex and projective
      scaling algorithms as iteratively reweighted least squares methods". SIAM
      Review. 33 (2): 220â237. doi:10.1137/1033049. JSTOR 2031142.
      MR 1124362.
   6. ^Stone, Richard E.; Tovey, Craig A. (1991). "Erratum: The simplex and
      projective scaling algorithms as iteratively reweighted least squares
      methods". SIAM Review. 33 (3): 461. doi:10.1137/1033100. JSTOR 2031443.
      MR 1124362.
   7. ^Strang,_Gilbert (1 June 1987). "Karmarkar's algorithm and its place in
      applied mathematics". The_Mathematical_Intelligencer. 9 (2): 4â10. doi:
      10.1007/BF03025891. ISSN 0343-6993. MR 0883185.
   8. ^ Murty_(1983, Theorem 3.3)
   9. ^ Murty_(1983, p. 143, Section 3.13)
  10. ^ a b Murty_(1983, p. 137, Section 3.8)
  11. ^ a b c George_B._Dantzig and Mukund N. Thapa. 1997. Linear programming
      1: Introduction. Springer-Verlag.
  12. ^ a b c d  Evar D. Nering and Albert_W._Tucker, 1993, Linear Programs and
      Related Problems, Academic Press. (elementary)
  13. ^ a b Robert J. Vanderbei, Linear_Programming:_Foundations_and
      Extensions, 3rd ed., International Series in Operations Research &
      Management Science, Vol. 114, Springer Verlag, 2008.
  14. ISBN 978-0-387-74387-5.
  15. ^Dantzig, George B. (April 1982). "Reminiscences_about_the_origins_of
      linear_programming". Operations Research Letters. 1 (2): 43â48. doi:
      10.1016/0167-6377(82)90043-8.
  16. ^Albers and Reid (1986). "An_Interview_with_George_B._Dantzig:_The_Father
      of_Linear_Programming". College Mathematics Journal: 292â314.
  17. ^Dantzig, George (May 1987). Origins_of_the_simplex_method (PDF). A
      History of Scientific Computing. doi:10.1145/87252.88081 (inactive 2019-
      07-04). ISBN 978-0-201-50814-7.
  18. ^ Murty_(1983, Section 2.2)
  19. ^ Murty_(1983, p. 173)
  20. ^ Murty_(1983, section 2.3.2)
  21. ^ Murty_(1983, section 3.12)
  22. ^ a b Murty_(1983, p. 66)
  23. ^ Harris, Paula MJ. "Pivot selection methods of the Devex LP code."
      Mathematical programming 5.1 (1973): 1â28
  24. ^ Murty_(1983, p. 67)
  25. ^ Murty_(1983, p. 60)
  26. ^ a b c d M. Padberg, Linear Optimization and Extensions, Second Edition,
      Springer-Verlag, 1999.
  27. ^ a b  George_B._Dantzig and Mukund N. Thapa. 2003. Linear Programming 2:
      Theory and Extensions. Springer-Verlag.
  28. ^ Dmitris Alevras and Manfred W. Padberg, Linear Optimization and
      Extensions: Problems and Extensions, Universitext, Springer-Verlag, 2001.
      (Problems from Padberg with solutions.)
  29. ^Maros, IstvÃ¡n; Mitra, Gautam (1996). "Simplex algorithms". In J. E.
      Beasley (ed.). Advances in linear and integer programming. Oxford
      Science. pp. 1â46. MR 1438309.
  30. ^Maros, IstvÃ¡n (2003). Computational techniques of the simplex method.
      International Series in Operations Research & Management Science. 61.
      Boston, MA: Kluwer Academic Publishers. pp. xx+325. ISBN 978-1-4020-7332-
      8. MR 1960274.
  31. ^ Bland, Robert G. (May 1977). "New finite pivoting rules for the simplex
      method". Mathematics of Operations Research. 2 (2): 103â107. doi:
      10.1287/moor.2.2.103. JSTOR 3689647. MR 0459599.
  32. ^ Murty_(1983, p. 79)
  33. ^ There are abstract optimization problems, called oriented_matroid
      programs, on which Bland's rule cycles (incorrectly) while the criss-
      cross_algorithm terminates correctly.
  34. ^Klee,_Victor; Minty,_George_J. (1972). "How good is the simplex
      algorithm?". In Shisha, Oved (ed.). Inequalities III (Proceedings of the
      Third Symposium on Inequalities held at the University of California, Los
      Angeles, Calif., September 1â9, 1969, dedicated to the memory of
      Theodore S. Motzkin). New York-London: Academic Press. pp. 159â175.
      MR 0332165.
  35. ^Hansen, Thomas; Zwick,_Uri (2015), "An Improved Version of the Random-
      Facet Pivoting Rule for the Simplex Algorithm", Proceedings of the Forty-
      seventh Annual ACM Symposium on Theory of Computing: 209â218,
      CiteSeerX 10.1.1.697.2526, doi:10.1145/2746539.2746557,
      ISBN 9781450335362
  36. ^Disser, Yann; Skutella, Martin (2018-11-01). "The Simplex Algorithm Is
      NP-Mighty". ACM Trans. Algorithms. 15 (1): 5:1â5:19. arXiv:1311.5935.
      doi:10.1145/3280847. ISSN 1549-6325.
  37. ^Adler, Ilan; Christos,_Papadimitriou; Rubinstein, Aviad (2014), "On
      Simplex Pivoting Rules and Complexity Theory", International Conference
      on Integer Programming and Combinatorial Optimization, Lecture Notes in
      Computer Science, 17: 13â24, arXiv:1404.3320, doi:10.1007/978-3-319-
      07557-0_2, ISBN 978-3-319-07556-3
  38. ^Fearnly, John; Savani, Rahul (2015), "The Complexity of the Simplex
      Method", Proceedings of the Forty-seventh Annual ACM Symposium on Theory
      of Computing: 201â208, arXiv:1404.0605, doi:10.1145/2746539.2746558,
      ISBN 9781450335362
  39. ^ Alexander_Schrijver, Theory of Linear and Integer Programming. John
      Wiley & sons, 1998,
  40. ISBN 0-471-98232-6 (mathematical)
  41. ^ The simplex algorithm takes on average D steps for a cube. Borgwardt_
      (1987):Borgwardt, Karl-Heinz (1987). The simplex method: A probabilistic
      analysis. Algorithms and Combinatorics (Study and Research Texts). 1.
      Berlin: Springer-Verlag. pp. xii+268. ISBN 978-3-540-17096-9. MR 0868467.
  42. ^Spielman, Daniel; Teng,_Shang-Hua (2001). "Smoothed analysis of
      algorithms: why the simplex algorithm usually takes polynomial time".
      Proceedings of the Thirty-Third Annual ACM Symposium on Theory of
      Computing. ACM. pp. 296â305. arXiv:cs/0111050. doi:10.1145/
      380752.380813. ISBN 978-1-58113-349-3.
  43. ^Terlaky, TamÃ¡s; Zhang, Shu Zhong (1993). "Pivot rules for linear
      programming: A Survey on recent theoretical developments". Annals of
      Operations Research. 46â47 (1): 203â233. CiteSeerX 10.1.1.36.7658.
      doi:10.1007/BF02096264. ISSN 0254-5330. MR 1260019.
  44. ^Fukuda, Komei; Terlaky, TamÃ¡s (1997). Thomas M. Liebling and Dominique
      de Werra (eds.). "Criss-cross methods: A fresh view on pivot algorithms".
      Mathematical Programming, Series B. 79 (1â3). Amsterdam: North-Holland
      Publishing Co. pp. 369â395. doi:10.1007/BF02614325. MR 1464775.CS1
      maint: Uses editors parameter (link)
  45. ^ Murty_(1983, Chapter 3.20 (pp. 160â164) and pp. 168 and 179)
  46. ^ Chapter five:Craven, B. D. (1988). Fractional programming. Sigma Series
      in Applied Mathematics. 4. Berlin: Heldermann Verlag. p. 145. ISBN 978-3-
      88538-404-5. MR 0949209.
  47. ^Kruk, Serge; Wolkowicz, Henry (1999). "Pseudolinear programming". SIAM
      Review. 41 (4): 795â805. Bibcode:1999SIAMR..41..795K.
      CiteSeerX 10.1.1.53.7355. doi:10.1137/S0036144598335259. JSTOR 2653207.
      MR 1723002.
  48. ^Mathis, Frank H.; Mathis, Lenora Jane (1995). "A nonlinear programming
      algorithm for hospital management". SIAM_Review. 37 (2): 230â234. doi:
      10.1137/1037046. JSTOR 2132826. MR 1343214.
  49. ^IllÃ©s, Tibor; Szirmai, Ãkos; Terlaky, TamÃ¡s (1999). "The_finite
      criss-cross_method_for_hyperbolic_programming". European Journal of
      Operational Research. 114 (1): 198â214. CiteSeerX 10.1.1.36.7090. doi:
      10.1016/S0377-2217(98)00049-6. ISSN 0377-2217. PDF_preprint.
***** References[edit] *****
    * Murty,_Katta_G. (1983). Linear programming. New York: John Wiley & Sons,
      Inc. pp. xix+482. ISBN 978-0-471-09725-9. MR 0720547.
***** Further reading[edit] *****
These introductions are written for students of computer_science and operations
research:
    * Thomas_H._Cormen, Charles_E._Leiserson, Ronald_L._Rivest, and Clifford
      Stein. Introduction to Algorithms, Second Edition. MIT Press and McGraw-
      Hill, 2001.
ISBN 0-262-03293-7. Section 29.3: The simplex algorithm, pp. 790–804.
Frederick S. Hillier and Gerald J. Lieberman: Introduction to Operations
Research, 8th edition. McGraw-Hill.
ISBN 0-07-123828-X
Rardin, Ronald L. (1997). Optimization in operations research. Prentice Hall.
p. 919. ISBN 978-0-02-398415-0.
***** External links[edit] *****
 The Wikibook Operations_Research has a page on the topic of: The_Simplex
 Method
    * An_Introduction_to_Linear_Programming_and_the_Simplex_Algorithm by Spyros
      Reveliotis of the Georgia Institute of Technology.
    * Greenberg, Harvey J., KleeâMinty Polytope Shows Exponential Time
      Complexity of Simplex Method University of Colorado at Denver (1997) PDF
      download
    * Simplex_Method A tutorial for Simplex Method with examples (also two-
      phase and M-method).
    * Mathstools Simplex Calculator from www.mathstools.com
    * Example_of_Simplex_Procedure_for_a_Standard_Linear_Programming_Problem by
      Thomas McFarland of the University of Wisconsin-Whitewater.
    * PHPSimplex:_online_tool_to_solve_Linear_Programming_Problems by Daniel
      Izquierdo and Juan JosÃ© Ruiz of the University of MÃ¡laga (UMA, Spain)
    * simplex-m Online Simplex Solver
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
quadratic                       * Simplex algorithm of Dantzig                             maximum.]
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
                              * Linear_programming_(LP)
                              * Quadratic_programming_(QP)
Complementarity Problems      * Linear_complementarity_problem_(LCP)
                              * Mixed_linear_(MLCP)
                              * Mixed_(MCP)
                              * Nonlinear(NCP)
                              * Simplex (Dantzig)
Basis-exchange_algorithms     * Revised_simplex
                              * Criss-cross
                              * Lemke

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Simplex_algorithm&oldid=907993170"
Categories:
    * Optimization_algorithms_and_methods
    * 1947_in_computer_science
    * Exchange_algorithms
    * Linear_programming
    * Computer-related_introductions_in_1947
Hidden categories:
    * Pages_with_DOIs_inactive_as_of_2019
    * CS1:_long_volume_value
    * CS1_maint:_Uses_editors_parameter
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_June_2019
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
    * à¦¬à¦¾à¦à¦²à¦¾
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Svenska
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 26 July 2019, at 17:24 (UTC).
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
