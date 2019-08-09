The following text has been accessed from https://en.wikipedia.org/wiki/System_of_linear_equations at Fri Aug 9 01:13:09 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** System of linear equations ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (October 2015)(Learn_how_and
 when_to_remove_this_template_message)
A linear system in three variables determines a collection of planes. The
intersection point is the solution.
In mathematics, a system of linear equations (or linear system) is a collection
of two or more linear_equations involving the same set of variables. For
example,
             3 x     +     2 y     &#x2212;     z     =     1      2 x
      &#x2212;     2 y     +     4 z     =     &#x2212; 2      &#x2212; x     +
      1 2    y     &#x2212;     z     =     0        {\displaystyle {\begin
      {alignedat}{7}3x&&\;+\;&&2y&&\;-\;&&z&&\;=\;&&1&\\2x&&\;-
      \;&&2y&&\;+\;&&4z&&\;=\;&&-2&\\-x&&\;+\;&&{\tfrac {1}{2}}y&&\;-
      \;&&z&&\;=\;&&0&\end{alignedat}}}  [{\begin{alignedat}
      {7}3x&&\;+\;&&2y&&\;-\;&&z&&\;=\;&&1&\\2x&&\;-\;&&2y&&\;+\;&&4z&&\;=\;&&-
      2&\\-x&&\;+\;&&{\tfrac {1}{2}}y&&\;-\;&&z&&\;=\;&&0&\end{alignedat}}]
is a system of three equations in the three variables x, y, z. A solution to a
linear system is an assignment of values to the variables such that all the
equations are simultaneously satisfied. A solution to the system above is given
by
             x     =    1     y     =    &#x2212; 2     z     =    &#x2212; 2
      {\displaystyle {\begin{alignedat}{2}x&\,=\,&1\\y&\,=\,&-2\\z&\,=\,&-2\end
      {alignedat}}}  [{\begin{alignedat}{2}x&\,=\,&1\\y&\,=\,&-2\\z&\,=\,&-
      2\end{alignedat}}]
since it makes all three equations valid. The word "system" indicates that the
equations are to be considered collectively, rather than individually.
In mathematics, the theory of linear systems is the basis and a fundamental
part of linear_algebra, a subject which is used in most parts of modern
mathematics. Computational algorithms for finding the solutions are an
important part of numerical_linear_algebra, and play a prominent role in
engineering, physics, chemistry, computer_science, and economics. A system_of
non-linear_equations can often be approximated by a linear system (see
linearization), a helpful technique when making a mathematical_model or
computer_simulation of a relatively complex_system.
Very often, the coefficients of the equations are real or complex_numbers and
the solutions are searched in the same set of numbers, but the theory and the
algorithms apply for coefficients and solutions in any field. For solutions in
an integral_domain like the ring of the integers, or in other algebraic
structures, other theories have been developed, see Linear_equation_over_a
ring. Integer_linear_programming is a collection of methods for finding the
"best" integer solution (when there are many). GrÃ¶bner_basis theory provides
algorithms when coefficients and unknowns are polynomials. Also tropical
geometry is an example of linear algebra in a more exotic structure.
⁰
***** Contents *****
    * 1_Elementary_example
    * 2_General_form
          o 2.1_Vector_equation
          o 2.2_Matrix_equation
    * 3_Solution_set
          o 3.1_Geometric_interpretation
          o 3.2_General_behavior
    * 4_Properties
          o 4.1_Independence
          o 4.2_Consistency
          o 4.3_Equivalence
    * 5_Solving_a_linear_system
          o 5.1_Describing_the_solution
          o 5.2_Elimination_of_variables
          o 5.3_Row_reduction
          o 5.4_Cramer's_rule
          o 5.5_Matrix_solution
          o 5.6_Other_methods
    * 6_Homogeneous_systems
          o 6.1_Homogeneous_solution_set
          o 6.2_Relation_to_nonhomogeneous_systems
    * 7_See_also
    * 8_References
    * 9_Further_reading
    * 10_External_links
***** Elementary example[edit] *****
The simplest kind of linear system involves two equations and two variables:
             2 x     +     3 y     =     6      4 x     +     9 y     =     15
      .       {\displaystyle {\begin{alignedat}
      {5}2x&&\;+\;&&3y&&\;=\;&&6&\\4x&&\;+\;&&9y&&\;=\;&&15&.\end{alignedat}}}
      [{\begin{alignedat}
      {5}2x&&\;+\;&&3y&&\;=\;&&6&\\4x&&\;+\;&&9y&&\;=\;&&15&.\end{alignedat}}]
One method for solving such a system is as follows. First, solve the top
equation for     x   {\displaystyle x}  [x] in terms of     y   {\displaystyle
y}  [y]:
         x = 3 &#x2212;   3 2   y .   {\displaystyle x=3-{\frac {3}{2}}y.}
      [x=3-{\frac {3}{2}}y.]
Now substitute this expression for x into the bottom equation:
         4  (  3 &#x2212;   3 2   y  )  + 9 y = 15.   {\displaystyle 4\left(3-
      {\frac {3}{2}}y\right)+9y=15.}  [4\left(3-{\frac {3}{2}}y\right)+9y=15.]
This results in a single equation involving only the variable     y
{\displaystyle y}  [y]. Solving gives     y = 1   {\displaystyle y=1}  [y=1],
and substituting this back into the equation for     x   {\displaystyle x}  [x]
yields     x = 3  /  2   {\displaystyle x=3/2}  [x=3/2]. This method
generalizes to systems with additional variables (see "elimination of
variables" below, or the article on elementary_algebra.)
***** General form[edit] *****
A general system of m linear equations with n unknowns can be written as
              a  11    x  1   +  a  12    x  2   + &#x22EF; +  a  1 n    x  n
      =  b  1        a  21    x  1   +  a  22    x  2   + &#x22EF; +  a  2 n
      x  n      =  b  2        &#xA0; &#xA0; &#x22EE;      a  m 1    x  1   +
      a  m 2    x  2   + &#x22EF; +  a  m n    x  n      =  b  m   ,
      {\displaystyle {\begin{aligned}a_{11}x_{1}+a_{12}x_{2}+\cdots +a_{1n}x_
      {n}&=b_{1}\\a_{21}x_{1}+a_{22}x_{2}+\cdots +a_{2n}x_{n}&=b_{2}\\&\ \
      \vdots \\a_{m1}x_{1}+a_{m2}x_{2}+\cdots +a_{mn}x_{n}&=b_{m},\end
      {aligned}}}  [{\displaystyle {\begin{aligned}a_{11}x_{1}+a_{12}x_
      {2}+\cdots +a_{1n}x_{n}&=b_{1}\\a_{21}x_{1}+a_{22}x_{2}+\cdots +a_{2n}x_
      {n}&=b_{2}\\&\ \ \vdots \\a_{m1}x_{1}+a_{m2}x_{2}+\cdots +a_{mn}x_{n}&=b_
      {m},\end{aligned}}}]
where      x  1   ,  x  2   , &#x2026; ,  x  n     {\displaystyle x_{1},x_
{2},\ldots ,x_{n}}  [x_{1},x_{2},\ldots ,x_{n}] are the unknowns,      a  11
,  a  12   , &#x2026; ,  a  m n     {\displaystyle a_{11},a_{12},\ldots ,a_
{mn}}  [a_{11},a_{12},\ldots ,a_{mn}] are the coefficients of the system, and
b  1   ,  b  2   , &#x2026; ,  b  m     {\displaystyle b_{1},b_{2},\ldots ,b_
{m}}  [b_{1},b_{2},\ldots ,b_{m}] are the constant terms.
Often the coefficients and unknowns are real or complex_numbers, but integers
and rational_numbers are also seen, as are polynomials and elements of an
abstract algebraic_structure.
**** Vector equation[edit] ****
One extremely helpful view is that each unknown is a weight for a column_vector
in a linear_combination.
          x  1     [     a  11        a  21       &#x22EE;      a  m 1      ]
      +  x  2     [     a  12        a  22       &#x22EE;      a  m 2      ]
      + &#x22EF; +  x  n     [     a  1 n        a  2 n       &#x22EE;      a
      m n      ]   =   [     b  1        b  2       &#x22EE;      b  m      ]
      {\displaystyle x_{1}{\begin{bmatrix}a_{11}\\a_{21}\\\vdots \\a_{m1}\end
      {bmatrix}}+x_{2}{\begin{bmatrix}a_{12}\\a_{22}\\\vdots \\a_{m2}\end
      {bmatrix}}+\cdots +x_{n}{\begin{bmatrix}a_{1n}\\a_{2n}\\\vdots \\a_
      {mn}\end{bmatrix}}={\begin{bmatrix}b_{1}\\b_{2}\\\vdots \\b_{m}\end
      {bmatrix}}}  [x_{1}{\begin{bmatrix}a_{11}\\a_{21}\\\vdots \\a_{m1}\end
      {bmatrix}}+x_{2}{\begin{bmatrix}a_{12}\\a_{22}\\\vdots \\a_{m2}\end
      {bmatrix}}+\cdots +x_{n}{\begin{bmatrix}a_{1n}\\a_{2n}\\\vdots \\a_
      {mn}\end{bmatrix}}={\begin{bmatrix}b_{1}\\b_{2}\\\vdots \\b_{m}\end
      {bmatrix}}]
This allows all the language and theory of vector_spaces (or more generally,
modules) to be brought to bear. For example, the collection of all possible
linear combinations of the vectors on the left-hand side is called their span,
and the equations have a solution just when the right-hand vector is within
that span. If every vector within that span has exactly one expression as a
linear combination of the given left-hand vectors, then any solution is unique.
In any event, the span has a basis of linearly_independent vectors that do
guarantee exactly one expression; and the number of vectors in that basis (its
dimension) cannot be larger than m or n, but it can be smaller. This is
important because if we have m independent vectors a solution is guaranteed
regardless of the right-hand side, and otherwise not guaranteed.
**** Matrix equation[edit] ****
The vector equation is equivalent to a matrix equation of the form
         A  x  =  b    {\displaystyle A\mathbf {x} =\mathbf {b} }  [A\mathbf
      {x} =\mathbf {b} ]
where A is an mÃn matrix, x is a column_vector with n entries, and b is a
column vector with m entries.
         A =   [     a  11      a  12     &#x22EF;    a  1 n        a  21
      a  22     &#x22EF;    a  2 n       &#x22EE;   &#x22EE;   &#x22F1;
      &#x22EE;      a  m 1      a  m 2     &#x22EF;    a  m n      ]   ,   x  =
      [     x  1        x  2       &#x22EE;      x  n      ]   ,   b  =
      [     b  1        b  2       &#x22EE;      b  m      ]     {\displaystyle
      A={\begin{bmatrix}a_{11}&a_{12}&\cdots &a_{1n}\\a_{21}&a_{22}&\cdots &a_
      {2n}\\\vdots &\vdots &\ddots &\vdots \\a_{m1}&a_{m2}&\cdots &a_{mn}\end
      {bmatrix}},\quad \mathbf {x} ={\begin{bmatrix}x_{1}\\x_{2}\\\vdots \\x_
      {n}\end{bmatrix}},\quad \mathbf {b} ={\begin{bmatrix}b_{1}\\b_{2}\\\vdots
      \\b_{m}\end{bmatrix}}}  [{\displaystyle A={\begin{bmatrix}a_{11}&a_
      {12}&\cdots &a_{1n}\\a_{21}&a_{22}&\cdots &a_{2n}\\\vdots &\vdots &\ddots
      &\vdots \\a_{m1}&a_{m2}&\cdots &a_{mn}\end{bmatrix}},\quad \mathbf {x} =
      {\begin{bmatrix}x_{1}\\x_{2}\\\vdots \\x_{n}\end{bmatrix}},\quad \mathbf
      {b} ={\begin{bmatrix}b_{1}\\b_{2}\\\vdots \\b_{m}\end{bmatrix}}}]
The number of vectors in a basis for the span is now expressed as the rank of
the matrix.
***** Solution set[edit] *****
The solution set for the equations x − y = −1 and 3x + y = 9 is the single
point (2, 3).
A solution of a linear system is an assignment of values to the variables x1,
x2, ..., xn such that each of the equations is satisfied. The set of all
possible solutions is called the solution_set.
A linear system may behave in any one of three possible ways:
   1. The system has infinitely many solutions.
   2. The system has a single unique solution.
   3. The system has no solution.
**** Geometric interpretation[edit] ****
For a system involving two variables (x and y), each linear equation determines
a line on the xy-plane. Because a solution to a linear system must satisfy all
of the equations, the solution set is the intersection of these lines, and is
hence either a line, a single point, or the empty_set.
For three variables, each linear equation determines a plane in three-
dimensional_space, and the solution set is the intersection of these planes.
Thus the solution set may be a plane, a line, a single point, or the empty set.
For example, as three parallel planes do not have a common point, the solution
set of their equations is empty; the solution set of the equations of three
planes intersecting at a point is single point; if three planes pass through
two points, their equations have at least two common solutions; in fact the
solution set is infinite and consists in all the line passing through these
points.[1]
For n variables, each linear equation determines a hyperplane in n-dimensional
space. The solution set is the intersection of these hyperplanes, and is a
flat, which may have any dimension lower than n.
**** General behavior[edit] ****
The solution set for two equations in three variables is, in general, a line.
In general, the behavior of a linear system is determined by the relationship
between the number of equations and the number of unknowns. Here, "in general"
means that a different behavior may occur for specific values of the
coefficients of the equations.
    * In general, a system with fewer equations than unknowns has infinitely
      many solutions, but it may have no solution. Such a system is known as an
      underdetermined_system.
    * In general, a system with the same number of equations and unknowns has a
      single unique solution.
    * In general, a system with more equations than unknowns has no solution.
      Such a system is also known as an overdetermined_system.
In the first case, the dimension of the solution set is, in general, equal to n
− m, where n is the number of variables and m is the number of equations.
The following pictures illustrate this trichotomy in the case of two variables:
      [One_Line.svg] [Two_Lines.svg] [Three_Lines.svg]
       One equation   Two equations   Three equations
The first system has infinitely many solutions, namely all of the points on the
blue line. The second system has a single unique solution, namely the
intersection of the two lines. The third system has no solutions, since the
three lines share no common point.
It must be kept in mind that the pictures above show only the most common case
(the general case). It is possible for a system of two equations and two
unknowns to have no solution (if the two lines are parallel), or for a system
of three equations and two unknowns to be solvable (if the three lines
intersect at a single point).
A system of linear equations behave differently from the general case if the
equations are linearly_dependent, or if it is inconsistent and has no more
equations than unknowns.
***** Properties[edit] *****
**** Independence[edit] ****
The equations of a linear system are independent if none of the equations can
be derived algebraically from the others. When the equations are independent,
each equation contains new information about the variables, and removing any of
the equations increases the size of the solution set. For linear equations,
logical independence is the same as linear_independence.
The equations x − 2y = −1, 3x + 5y = 8, and 4x + 3y = 7 are linearly dependent.
For example, the equations
         3 x + 2 y = 6      and      6 x + 4 y = 12   {\displaystyle
      3x+2y=6\;\;\;\;{\text{and}}\;\;\;\;6x+4y=12}  [3x+2y=6\;\;\;\;{\text
      {and}}\;\;\;\;6x+4y=12]
are not independent â they are the same equation when scaled by a factor of
two, and they would produce identical graphs. This is an example of equivalence
in a system of linear equations.
For a more complicated example, the equations
             x     &#x2212;     2 y     =     &#x2212; 1      3 x     +     5 y
      =     8      4 x     +     3 y     =     7        {\displaystyle {\begin
      {alignedat}{5}x&&\;-\;&&2y&&\;=\;&&-
      1&\\3x&&\;+\;&&5y&&\;=\;&&8&\\4x&&\;+\;&&3y&&\;=\;&&7&\end{alignedat}}}
      [{\begin{alignedat}{5}x&&\;-\;&&2y&&\;=\;&&-
      1&\\3x&&\;+\;&&5y&&\;=\;&&8&\\4x&&\;+\;&&3y&&\;=\;&&7&\end{alignedat}}]
are not independent, because the third equation is the sum of the other two.
Indeed, any one of these equations can be derived from the other two, and any
one of the equations can be removed without affecting the solution set. The
graphs of these equations are three lines that intersect at a single point.
**** Consistency[edit] ****
See also: Consistent_and_inconsistent_equations
The equations 3x + 2y = 6 and 3x + 2y = 12 are inconsistent.
A linear system is inconsistent if it has no solution, and otherwise it is said
to be consistent. When the system is inconsistent, it is possible to derive a
contradiction from the equations, that may always be rewritten as the statement
0 = 1.
For example, the equations
         3 x + 2 y = 6      and      3 x + 2 y = 12   {\displaystyle
      3x+2y=6\;\;\;\;{\text{and}}\;\;\;\;3x+2y=12}  [3x+2y=6\;\;\;\;{\text
      {and}}\;\;\;\;3x+2y=12]
are inconsistent. In fact, by subtracting the first equation from the second
one and multiplying both sides of the result by 1/6, we get 0 = 1. The graphs
of these equations on the xy-plane are a pair of parallel lines.
It is possible for three linear equations to be inconsistent, even though any
two of them are consistent together. For example, the equations
             x     +     y     =     1      2 x     +     y     =     1      3
      x     +     2 y     =     3        {\displaystyle {\begin{alignedat}
      {7}x&&\;+\;&&y&&\;=\;&&1&\\2x&&\;+\;&&y&&\;=\;&&1&\\3x&&\;+\;&&2y&&\;=\;&&3&\end
      {alignedat}}}  [{\begin{alignedat}
      {7}x&&\;+\;&&y&&\;=\;&&1&\\2x&&\;+\;&&y&&\;=\;&&1&\\3x&&\;+\;&&2y&&\;=\;&&3&\end
      {alignedat}}]
are inconsistent. Adding the first two equations together gives 3x + 2y = 2,
which can be subtracted from the third equation to yield 0 = 1. Any two of
these equations have a common solution. The same phenomenon can occur for any
number of equations.
In general, inconsistencies occur if the left-hand sides of the equations in a
system are linearly dependent, and the constant terms do not satisfy the
dependence relation. A system of equations whose left-hand sides are linearly
independent is always consistent.
Putting it another way, according to the RouchÃ©âCapelli_theorem, any system
of equations (overdetermined or otherwise) is inconsistent if the rank of the
augmented_matrix is greater than the rank of the coefficient_matrix. If, on the
other hand, the ranks of these two matrices are equal, the system must have at
least one solution. The solution is unique if and only if the rank equals the
number of variables. Otherwise the general solution has k free parameters where
k is the difference between the number of variables and the rank; hence in such
a case there are an infinitude of solutions. The rank of a system of equations
(i.e. the rank of the augmented matrix) can never be higher than [the number of
variables] + 1, which means that a system with any number of equations can
always be reduced to a system that has a number of independent_equations that
is at most equal to [the number of variables] + 1.
**** Equivalence[edit] ****
Two linear systems using the same set of variables are equivalent if each of
the equations in the second system can be derived algebraically from the
equations in the first system, and vice versa. Two systems are equivalent if
either both are inconsistent or each equation of each of them is a linear
combination of the equations of the other one. It follows that two linear
systems are equivalent if and only if they have the same solution set.
***** Solving a linear system[edit] *****
There are several algorithms for solving a system of linear equations.
**** Describing the solution[edit] ****
When the solution set is finite, it is reduced to a single element. In this
case, the unique solution is described by a sequence of equations whose left-
hand sides are the names of the unknowns and right-hand sides are the
corresponding values, for example     ( x = 3 ,  y = &#x2212; 2 ,  z = 6 )
{\displaystyle (x=3,\;y=-2,\;z=6)}  [(x=3,\;y=-2,\;z=6)]. When an order on the
unknowns has been fixed, for example the alphabetical_order the solution may be
described as a vector of values, like     ( 3 ,  &#x2212; 2 ,  6 )
{\displaystyle (3,\,-2,\,6)}  [(3,\,-2,\,6)] for the previous example.
To describe a set with an infinite number of solutions, typically some of the
variables are designated as free (or independent, or as parameters), meaning
that they are allowed to take any value, while the remaining variables are
dependent on the values of the free variables.
For example, consider the following system:
             x     +     3 y     &#x2212;     2 z     =     5      3 x     +
      5 y     +     6 z     =     7        {\displaystyle {\begin{alignedat}
      {7}x&&\;+\;&&3y&&\;-
      \;&&2z&&\;=\;&&5&\\3x&&\;+\;&&5y&&\;+\;&&6z&&\;=\;&&7&\end{alignedat}}}
      [{\begin{alignedat}{7}x&&\;+\;&&3y&&\;-
      \;&&2z&&\;=\;&&5&\\3x&&\;+\;&&5y&&\;+\;&&6z&&\;=\;&&7&\end{alignedat}}]
The solution set to this system can be described by the following equations:
         x = &#x2212; 7 z &#x2212; 1      and      y = 3 z + 2  .
      {\displaystyle x=-7z-1\;\;\;\;{\text{and}}\;\;\;\;y=3z+2{\text{.}}}  [x=-
      7z-1\;\;\;\;{\text{and}}\;\;\;\;y=3z+2{\text{.}}]
Here z is the free variable, while x and y are dependent on z. Any point in the
solution set can be obtained by first choosing a value for z, and then
computing the corresponding values for x and y.
Each free variable gives the solution space one degree_of_freedom, the number
of which is equal to the dimension of the solution set. For example, the
solution set for the above equation is a line, since a point in the solution
set can be chosen by specifying the value of the parameter z. An infinite
solution of higher order may describe a plane, or higher-dimensional set.
Different choices for the free variables may lead to different descriptions of
the same solution set. For example, the solution to the above equations can
alternatively be described as follows:
         y = &#x2212;   3 7   x +   11 7        and      z = &#x2212;   1 7   x
      &#x2212;   1 7    .    {\displaystyle y=-{\frac {3}{7}}x+{\frac {11}
      {7}}\;\;\;\;{\text{and}}\;\;\;\;z=-{\frac {1}{7}}x-{\frac {1}{7}}{\text
      {.}}}  [y=-{\frac {3}{7}}x+{\frac {11}{7}}\;\;\;\;{\text{and}}\;\;\;\;z=-
      {\frac {1}{7}}x-{\frac {1}{7}}{\text{.}}]
Here x is the free variable, and y and z are dependent.
**** Elimination of variables[edit] ****
The simplest method for solving a system of linear equations is to repeatedly
eliminate variables. This method can be described as follows:
   1. In the first equation, solve for one of the variables in terms of the
      others.
   2. Substitute this expression into the remaining equations. This yields a
      system of equations with one fewer equation and one fewer unknown.
   3. Repeat until the system is reduced to a single linear equation.
   4. Solve this equation, and then back-substitute until the entire solution
      is found.
For example, consider the following system:
             x     +     3 y     &#x2212;     2 z     =     5      3 x     +
      5 y     +     6 z     =     7      2 x     +     4 y     +     3 z     =
      8        {\displaystyle {\begin{alignedat}{7}x&&\;+\;&&3y&&\;-
      \;&&2z&&\;=\;&&5&\\3x&&\;+\;&&5y&&\;+\;&&6z&&\;=\;&&7&\\2x&&\;+\;&&4y&&\;+\;&&3z&&\;=\;&&8&\end
      {alignedat}}}  [{\begin{alignedat}{7}x&&\;+\;&&3y&&\;-
      \;&&2z&&\;=\;&&5&\\3x&&\;+\;&&5y&&\;+\;&&6z&&\;=\;&&7&\\2x&&\;+\;&&4y&&\;+\;&&3z&&\;=\;&&8&\end
      {alignedat}}]
Solving the first equation for x gives x = 5 + 2z − 3y, and plugging this into
the second and third equation yields
             &#x2212; 4 y     +     12 z     =     &#x2212; 8      &#x2212; 2 y
      +     7 z     =     &#x2212; 2        {\displaystyle {\begin{alignedat}
      {5}-4y&&\;+\;&&12z&&\;=\;&&-8&\\-2y&&\;+\;&&7z&&\;=\;&&-2&\end
      {alignedat}}}  [{\begin{alignedat}{5}-4y&&\;+\;&&12z&&\;=\;&&-8&\\-
      2y&&\;+\;&&7z&&\;=\;&&-2&\end{alignedat}}]
Solving the first of these equations for y yields y = 2 + 3z, and plugging this
into the second equation yields z = 2. We now have:
             x     =     5     +     2 z     &#x2212;     3 y      y     =
      2     +     3 z          z     =     2                {\displaystyle
      {\begin{alignedat}{7}x&&\;=\;&&5&&\;+\;&&2z&&\;-
      \;&&3y&\\y&&\;=\;&&2&&\;+\;&&3z&&&&&\\z&&\;=\;&&2&&&&&&&&&\end
      {alignedat}}}  [{\begin{alignedat}{7}x&&\;=\;&&5&&\;+\;&&2z&&\;-
      \;&&3y&\\y&&\;=\;&&2&&\;+\;&&3z&&&&&\\z&&\;=\;&&2&&&&&&&&&\end
      {alignedat}}]
Substituting z = 2 into the second equation gives y = 8, and substituting z = 2
and y = 8 into the first equation yields x = −15. Therefore, the solution set
is the single point (x, y, z) = (−15, 8, 2).
**** Row reduction[edit] ****
Main article: Gaussian_elimination
In row reduction (also known as Gaussian elimination), the linear system is
represented as an augmented_matrix:
          [     1   3   &#x2212; 2   5     3   5   6   7     2   4   3   8
      ]   .    {\displaystyle \left[{\begin{array}{rrr|r}1&3&-
      2&5\\3&5&6&7\\2&4&3&8\end{array}}\right]{\text{.}}}  [\left[{\begin
      {array}{rrr|r}1&3&-2&5\\3&5&6&7\\2&4&3&8\end{array}}\right]{\text{.}}]
This matrix is then modified using elementary_row_operations until it reaches
reduced_row_echelon_form. There are three types of elementary row operations:
      Type 1: Swap the positions of two rows.
      Type 2: Multiply a row by a nonzero scalar.
      Type 3: Add to one row a scalar multiple of another.
Because these operations are reversible, the augmented matrix produced always
represents a linear system that is equivalent to the original.
There are several specific algorithms to row-reduce an augmented matrix, the
simplest of which are Gaussian_elimination and Gauss-Jordan_elimination. The
following computation shows Gauss-Jordan elimination applied to the matrix
above:
              [     1   3   &#x2212; 2   5     3   5   6   7     2   4   3   8
      ]     &#x223C;  [     1   3   &#x2212; 2   5     0   &#x2212; 4   12
      &#x2212; 8     2   4   3   8     ]  &#x223C;  [     1   3   &#x2212; 2
      5     0   &#x2212; 4   12   &#x2212; 8     0   &#x2212; 2   7   &#x2212;
      2     ]  &#x223C;  [     1   3   &#x2212; 2   5     0   1   &#x2212; 3
      2     0   &#x2212; 2   7   &#x2212; 2     ]        &#x223C;  [     1   3
      &#x2212; 2   5     0   1   &#x2212; 3   2     0   0   1   2     ]
      &#x223C;  [     1   3   &#x2212; 2   5     0   1   0   8     0   0   1
      2     ]  &#x223C;  [     1   3   0   9     0   1   0   8     0   0   1
      2     ]  &#x223C;  [     1   0   0   &#x2212; 15     0   1   0   8     0
      0   1   2     ]  .       {\displaystyle {\begin{aligned}\left[{\begin
      {array}{rrr|r}1&3&-2&5\\3&5&6&7\\2&4&3&8\end{array}}\right]&\sim \left[
      {\begin{array}{rrr|r}1&3&-2&5\\0&-4&12&-8\\2&4&3&8\end{array}}\right]\sim
      \left[{\begin{array}{rrr|r}1&3&-2&5\\0&-4&12&-8\\0&-2&7&-2\end
      {array}}\right]\sim \left[{\begin{array}{rrr|r}1&3&-2&5\\0&1&-3&2\\0&-
      2&7&-2\end{array}}\right]\\&\sim \left[{\begin{array}{rrr|r}1&3&-
      2&5\\0&1&-3&2\\0&0&1&2\end{array}}\right]\sim \left[{\begin{array}
      {rrr|r}1&3&-2&5\\0&1&0&8\\0&0&1&2\end{array}}\right]\sim \left[{\begin
      {array}{rrr|r}1&3&0&9\\0&1&0&8\\0&0&1&2\end{array}}\right]\sim \left[
      {\begin{array}{rrr|r}1&0&0&-15\\0&1&0&8\\0&0&1&2\end{array}}\right].\end
      {aligned}}}  [{\begin{aligned}\left[{\begin{array}{rrr|r}1&3&-
      2&5\\3&5&6&7\\2&4&3&8\end{array}}\right]&\sim \left[{\begin{array}
      {rrr|r}1&3&-2&5\\0&-4&12&-8\\2&4&3&8\end{array}}\right]\sim \left[{\begin
      {array}{rrr|r}1&3&-2&5\\0&-4&12&-8\\0&-2&7&-2\end{array}}\right]\sim
      \left[{\begin{array}{rrr|r}1&3&-2&5\\0&1&-3&2\\0&-2&7&-2\end
      {array}}\right]\\&\sim \left[{\begin{array}{rrr|r}1&3&-2&5\\0&1&-
      3&2\\0&0&1&2\end{array}}\right]\sim \left[{\begin{array}{rrr|r}1&3&-
      2&5\\0&1&0&8\\0&0&1&2\end{array}}\right]\sim \left[{\begin{array}
      {rrr|r}1&3&0&9\\0&1&0&8\\0&0&1&2\end{array}}\right]\sim \left[{\begin
      {array}{rrr|r}1&0&0&-15\\0&1&0&8\\0&0&1&2\end{array}}\right].\end
      {aligned}}]
The last matrix is in reduced row echelon form, and represents the system x =
−15, y = 8, z = 2. A comparison with the example in the previous section on the
algebraic elimination of variables shows that these two methods are in fact the
same; the difference lies in how the computations are written down.
**** Cramer's rule[edit] ****
Main article: Cramer's_rule
Cramer's rule is an explicit formula for the solution of a system of linear
equations, with each variable given by a quotient of two determinants. For
example, the solution to the system
             x     +    3 y     &#x2212;    2 z     =    5     3 x     +    5 y
      +    6 z     =    7     2 x     +    4 y     +    3 z     =    8
      {\displaystyle {\begin{alignedat}{7}x&\;+&\;3y&\;-
      &\;2z&\;=&\;5\\3x&\;+&\;5y&\;+&\;6z&\;=&\;7\\2x&\;+&\;4y&\;+&\;3z&\;=&\;8\end
      {alignedat}}}  [{\begin{alignedat}{7}x&\;+&\;3y&\;-
      &\;2z&\;=&\;5\\3x&\;+&\;5y&\;+&\;6z&\;=&\;7\\2x&\;+&\;4y&\;+&\;3z&\;=&\;8\end
      {alignedat}}]
is given by
         x =      |     5   3   &#x2212; 2     7   5   6     8   4   3     |
      |     1   3   &#x2212; 2     3   5   6     2   4   3     |      ,     y =
      |     1   5   &#x2212; 2     3   7   6     2   8   3     |       |     1
      3   &#x2212; 2     3   5   6     2   4   3     |      ,     z =      |
      1   3   5     3   5   7     2   4   8     |       |     1   3   &#x2212;
      2     3   5   6     2   4   3     |      .   {\displaystyle x={\frac
      {\,\left|{\begin{matrix}5&3&-2\\7&5&6\\8&4&3\end{matrix}}\right|\,}
      {\,\left|{\begin{matrix}1&3&-2\\3&5&6\\2&4&3\end
      {matrix}}\right|\,}},\;\;\;\;y={\frac {\,\left|{\begin{matrix}1&5&-
      2\\3&7&6\\2&8&3\end{matrix}}\right|\,}{\,\left|{\begin{matrix}1&3&-
      2\\3&5&6\\2&4&3\end{matrix}}\right|\,}},\;\;\;\;z={\frac {\,\left|{\begin
      {matrix}1&3&5\\3&5&7\\2&4&8\end{matrix}}\right|\,}{\,\left|{\begin
      {matrix}1&3&-2\\3&5&6\\2&4&3\end{matrix}}\right|\,}}.}  [x={\frac
      {\,\left|{\begin{matrix}5&3&-2\\7&5&6\\8&4&3\end{matrix}}\right|\,}
      {\,\left|{\begin{matrix}1&3&-2\\3&5&6\\2&4&3\end
      {matrix}}\right|\,}},\;\;\;\;y={\frac {\,\left|{\begin{matrix}1&5&-
      2\\3&7&6\\2&8&3\end{matrix}}\right|\,}{\,\left|{\begin{matrix}1&3&-
      2\\3&5&6\\2&4&3\end{matrix}}\right|\,}},\;\;\;\;z={\frac {\,\left|{\begin
      {matrix}1&3&5\\3&5&7\\2&4&8\end{matrix}}\right|\,}{\,\left|{\begin
      {matrix}1&3&-2\\3&5&6\\2&4&3\end{matrix}}\right|\,}}.]
For each variable, the denominator is the determinant of the matrix of
coefficients, while the numerator is the determinant of a matrix in which one
column has been replaced by the vector of constant terms.
Though Cramer's rule is important theoretically, it has little practical value
for large matrices, since the computation of large determinants is somewhat
cumbersome. (Indeed, large determinants are most easily computed using row
reduction.) Further, Cramer's rule has very poor numerical properties, making
it unsuitable for solving even small systems reliably, unless the operations
are performed in rational arithmetic with unbounded precision.[citation_needed]
**** Matrix solution[edit] ****
If the equation system is expressed in the matrix form     A  x  =  b
{\displaystyle A\mathbf {x} =\mathbf {b} }  [A\mathbf {x} =\mathbf {b} ], the
entire solution set can also be expressed in matrix form. If the matrix A is
square (has m rows and n=m columns) and has full rank (all m rows are
independent), then the system has a unique solution given by
          x  =  A  &#x2212; 1    b    {\displaystyle \mathbf {x} =A^{-1}\mathbf
      {b} }  [{\displaystyle \mathbf {x} =A^{-1}\mathbf {b} }]
where      A  &#x2212; 1     {\displaystyle A^{-1}}  [A^{-1}] is the inverse of
A. More generally, regardless of whether m=n or not and regardless of the rank
of A, all solutions (if any exist) are given using the Moore-Penrose
pseudoinverse of A, denoted      A  +     {\displaystyle A^{+}}  [A^{+}], as
follows:
          x  =  A  +    b  + ( I &#x2212;  A  +   A )  w    {\displaystyle
      \mathbf {x} =A^{+}\mathbf {b} +(I-A^{+}A)\mathbf {w} }  [{\displaystyle
      \mathbf {x} =A^{+}\mathbf {b} +(I-A^{+}A)\mathbf {w} }]
where      w    {\displaystyle \mathbf {w} }  [\mathbf {w} ] is a vector of
free parameters that ranges over all possible nÃ1 vectors. A necessary and
sufficient condition for any solution(s) to exist is that the potential
solution obtained using      w  =  0    {\displaystyle \mathbf {w} =\mathbf {0}
}  [{\displaystyle \mathbf {w} =\mathbf {0} }] satisfy     A  x  =  b
{\displaystyle A\mathbf {x} =\mathbf {b} }  [A\mathbf {x} =\mathbf {b} ] — that
is, that     A  A  +    b  =  b  .   {\displaystyle AA^{+}\mathbf {b} =\mathbf
{b} .}  [{\displaystyle AA^{+}\mathbf {b} =\mathbf {b} .}] If this condition
does not hold, the equation system is inconsistent and has no solution. If the
condition holds, the system is consistent and at least one solution exists. For
example, in the above-mentioned case in which A is square and of full rank,
A  +     {\displaystyle A^{+}}  [A^{+}] simply equals      A  &#x2212; 1
{\displaystyle A^{-1}}  [A^{-1}] and the general solution equation simplifies
to      x  =  A  &#x2212; 1    b  + ( I &#x2212;  A  &#x2212; 1   A )  w  =  A
&#x2212; 1    b  + ( I &#x2212; I )  w  =  A  &#x2212; 1    b    {\displaystyle
\mathbf {x} =A^{-1}\mathbf {b} +(I-A^{-1}A)\mathbf {w} =A^{-1}\mathbf {b} +(I-
I)\mathbf {w} =A^{-1}\mathbf {b} }  [{\displaystyle \mathbf {x} =A^{-1}\mathbf
{b} +(I-A^{-1}A)\mathbf {w} =A^{-1}\mathbf {b} +(I-I)\mathbf {w} =A^{-1}\mathbf
{b} }] as previously stated, where      w    {\displaystyle \mathbf {w} }
[\mathbf {w} ] has completely dropped out of the solution, leaving only a
single solution. In other cases, though,      w    {\displaystyle \mathbf {w} }
[\mathbf {w} ] remains and hence an infinitude of potential values of the free
parameter vector      w    {\displaystyle \mathbf {w} }  [\mathbf {w} ] give an
infinitude of solutions of the equation.
**** Other methods[edit] ****
While systems of three or four equations can be readily solved by hand (see
Cracovian), computers are often used for larger systems. The standard algorithm
for solving a system of linear equations is based on Gaussian elimination with
some modifications. Firstly, it is essential to avoid division by small
numbers, which may lead to inaccurate results. This can be done by reordering
the equations if necessary, a process known as pivoting. Secondly, the
algorithm does not exactly do Gaussian elimination, but it computes the LU
decomposition of the matrix A. This is mostly an organizational tool, but it is
much quicker if one has to solve several systems with the same matrix A but
different vectors b.
If the matrix A has some special structure, this can be exploited to obtain
faster or more accurate algorithms. For instance, systems with a symmetric
positive_definite matrix can be solved twice as fast with the Cholesky
decomposition. Levinson_recursion is a fast method for Toeplitz_matrices.
Special methods exist also for matrices with many zero elements (so-called
sparse_matrices), which appear often in applications.
A completely different approach is often taken for very large systems, which
would otherwise take too much time or memory. The idea is to start with an
initial approximation to the solution (which does not have to be accurate at
all), and to change this approximation in several steps to bring it closer to
the true solution. Once the approximation is sufficiently accurate, this is
taken to be the solution to the system. This leads to the class of iterative
methods.
There is also a quantum_algorithm_for_linear_systems_of_equations.[2]
***** Homogeneous systems[edit] *****
See also: Homogeneous_differential_equation
A system of linear equations is homogeneous if all of the constant terms are
zero:
              a  11    x  1       +      a  12    x  2       + &#x22EF; +
      a  1 n    x  n       =      0      a  21    x  1       +      a  22    x
      2       + &#x22EF; +      a  2 n    x  n       =      0     &#x22EE;
      &#x22EE;         &#x22EE;            &#x22EE;      a  m 1    x  1       +
      a  m 2    x  2       + &#x22EF; +      a  m n    x  n       =      0.
      {\displaystyle {\begin{alignedat}{7}a_{11}x_{1}&&\;+\;&&a_{12}x_
      {2}&&\;+\cdots +\;&&a_{1n}x_{n}&&\;=\;&&&0\\a_{21}x_{1}&&\;+\;&&a_{22}x_
      {2}&&\;+\cdots +\;&&a_{2n}x_{n}&&\;=\;&&&0\\\vdots \;\;\;&&&&\vdots
      \;\;\;&&&&\vdots \;\;\;&&&&&\,\vdots \\a_{m1}x_{1}&&\;+\;&&a_{m2}x_
      {2}&&\;+\cdots +\;&&a_{mn}x_{n}&&\;=\;&&&0.\\\end{alignedat}}}  [{\begin
      {alignedat}{7}a_{11}x_{1}&&\;+\;&&a_{12}x_{2}&&\;+\cdots +\;&&a_{1n}x_
      {n}&&\;=\;&&&0\\a_{21}x_{1}&&\;+\;&&a_{22}x_{2}&&\;+\cdots +\;&&a_{2n}x_
      {n}&&\;=\;&&&0\\\vdots \;\;\;&&&&\vdots \;\;\;&&&&\vdots
      \;\;\;&&&&&\,\vdots \\a_{m1}x_{1}&&\;+\;&&a_{m2}x_{2}&&\;+\cdots +\;&&a_
      {mn}x_{n}&&\;=\;&&&0.\\\end{alignedat}}]
A homogeneous system is equivalent to a matrix equation of the form
         A   x   =   0     {\displaystyle A{\textbf {x}}={\textbf {0}}}  [A
      {\textbf {x}}={\textbf {0}}]
where A is an m × n matrix, x is a column vector with n entries, and 0 is the
zero_vector with m entries.
**** Homogeneous solution set[edit] ****
Every homogeneous system has at least one solution, known as the zero solution
(or trivial solution), which is obtained by assigning the value of zero to each
of the variables. If the system has a non-singular_matrix (det(A) â  0) then
it is also the only solution. If the system has a singular matrix then there is
a solution set with an infinite number of solutions. This solution set has the
following additional properties:
   1. If u and v are two vectors representing solutions to a homogeneous
      system, then the vector sum u + v is also a solution to the system.
   2. If u is a vector representing a solution to a homogeneous system, and r
      is any scalar, then ru is also a solution to the system.
These are exactly the properties required for the solution set to be a linear
subspace of Rn. In particular, the solution set to a homogeneous system is the
same as the null_space of the corresponding matrix A. Numerical solutions to a
homogeneous system can be found with a singular_value_decomposition.
**** Relation to nonhomogeneous systems[edit] ****
There is a close relationship between the solutions to a linear system and the
solutions to the corresponding homogeneous system:
         A   x   =   b     and   A   x   =   0    .    {\displaystyle A{\textbf
      {x}}={\textbf {b}}\qquad {\text{and}}\qquad A{\textbf {x}}={\textbf {0}}
      {\text{.}}}  [A{\textbf {x}}={\textbf {b}}\qquad {\text{and}}\qquad A
      {\textbf {x}}={\textbf {0}}{\text{.}}]
Specifically, if p is any specific solution to the linear system Ax = b, then
the entire solution set can be described as
          {    p   +   v   :   v    &#xA0;is any solution to&#xA0;  A   x   =
      0    }  .   {\displaystyle \left\{{\textbf {p}}+{\textbf {v}}:{\textbf
      {v}}{\text{ is any solution to }}A{\textbf {x}}={\textbf {0}}\right\}.}
      [\left\{{\textbf {p}}+{\textbf {v}}:{\textbf {v}}{\text{ is any solution
      to }}A{\textbf {x}}={\textbf {0}}\right\}.]
Geometrically, this says that the solution set for Ax = b is a translation of
the solution set for Ax = 0. Specifically, the flat for the first system can be
obtained by translating the linear_subspace for the homogeneous system by the
vector p.
This reasoning only applies if the system Ax = b has at least one solution.
This occurs if and only if the vector b lies in the image of the linear
transformation A.
***** See also[edit] *****
    * Arrangement_of_hyperplanes
    * Iterative_refinement
    * Coates_graph
    * LAPACK (the free standard package to solve linear equations numerically;
      available in Fortran, C, C++)
    * Linear_equation_over_a_ring
    * Linear_least_squares
    * Matrix_decomposition
    * Matrix_splitting
    * NAG_Numerical_Library (NAG Library versions of LAPACK solvers)
    * Simultaneous_equations
    * MooreâPenrose_pseudoinverse
***** References[edit] *****
   1. ^Charles G. Cullen (1990). Matrices_and_Linear_Transformations. MA:
      Dover. p. 3. ISBN 978-0-486-66328-9.
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
   3. ^ Quantum_algorithm_for_solving_linear_systems_of_equations,_by_Harrow_et
      al..
***** Further reading[edit] *****
    * Axler, Sheldon Jay (1997), Linear Algebra Done Right (2nd ed.), Springer-
      Verlag, ISBN 0-387-98259-0
Lay, David C. (August 22, 2005), Linear Algebra and Its Applications (3rd ed.),
Addison Wesley, ISBN 978-0-321-28713-7
Meyer, Carl D. (February 15, 2001), Matrix_Analysis_and_Applied_Linear_Algebra,
Society for Industrial and Applied Mathematics (SIAM), ISBN 978-0-89871-454-8,
archived from the_original on March 1, 2001
Poole, David (2006), Linear Algebra: A Modern Introduction (2nd ed.), Brooks/
Cole, ISBN 0-534-99845-3
Anton, Howard (2005), Elementary Linear Algebra (Applications Version) (9th
ed.), Wiley International
Leon, Steven J. (2006), Linear Algebra With Applications (7th ed.), Pearson
Prentice Hall
Strang,_Gilbert (2005), Linear Algebra and Its Applications
***** External links[edit] *****
    *  Media related to System_of_linear_equations at Wikimedia Commons
    * v
    * t
    * e
Linear_algebra
                            * Scalar
                            * Vector
                            * Vector_space
                            * Scalar_multiplication
                            * Vector_projection
                            * Linear_span
                            * Linear_map
                            * Linear_projection
                            * Linear_independence
                            * Linear_combination
                            * Basis
Basic concepts              * Change_of_basis
                            * Row_and_column_spaces
                            * Orthogonality
                            * Kernel
                            * Eigenvalues_and
                              eigenvectors
                            * Outer_product
                            * Inner_product_space
                            * Dot_product
                            * Transpose
                            * GramâSchmidt_process
                            * Linear equations
                            * Fundamental_theorem
                            * Cross_product
Vector algebra              * Triple_product
                            * Seven-dimensional_cross
                              product
                            * Geometric_algebra
                            * Exterior_algebra          [Three_dimensional
Multilinear_algebra         * Bivector                  Euclidean_space]
                            * Multivector
                            * Tensor
                            * Outermorphism
                            * Block
                            * Decomposition
                            * Invertible
                            * Minor
Matrices                    * Multiplication
                            * Rank
                            * Transformation
                            * Cramer's_rule
                            * Gaussian_elimination
                            * Determinant
                            * Dual
                            * Direct_sum
Algebraic constructions     * Function_space
                            * Quotient
                            * Subspace
                            * Tensor_product
                            * Floating-point
                            * MATLAB
                            * Numerical_stability
                            * Basic_Linear_Algebra
Numerical                     Subprograms_(BLAS)
                            * Sparse_matrix
                            * Comparison_of_linear
                              algebra_libraries
                            * Comparison_of_numerical
                              analysis_software
    * [Category] Category
    * [List-Class article] Outline
    * [Portal] Portal
    * [Wikibooks page] Wikibook
    * [Wikiversity page] Wikiversity

Retrieved from "https://en.wikipedia.org/w/
index.php?title=System_of_linear_equations&oldid=909835014"
Categories:
    * Equations
    * Linear_algebra
    * Numerical_linear_algebra
Hidden categories:
    * Articles_lacking_in-text_citations_from_October_2015
    * All_articles_lacking_in-text_citations
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_March_2017
    * Commons_category_link_from_Wikidata
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
    * Alemannisch
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AragonÃ©s
    * Asturianu
    * AzÉrbaycanca
    * ÐÐ°ÑÒ¡Ð¾ÑÑÑÐ°
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * Fiji_Hindi
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Interlingua
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Latina
    * LatvieÅ¡u
    * Lumbaart
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Occitan
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Ù¾ÙØ¬Ø§Ø¨Û
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * à·à·à¶à·à¶½
    * Simple_English
    * Ø³ÙÚÙ
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * Winaray
    * å´è¯­
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 22:12 (UTC).
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
