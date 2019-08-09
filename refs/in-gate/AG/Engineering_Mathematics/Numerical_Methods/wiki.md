The following text has been accessed from https://en.wikipedia.org/wiki/Numerical_analysis at Fri Aug 9 00:09:33 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Numerical analysis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 It has been suggested that Numerical_method be merged into this article.
 (Discuss)Proposed since January 2019.
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (November 2013)(Learn_how_and
 when_to_remove_this_template_message)
Babylonian clay tablet YBC_7289 (c. 1800â1600 BC) with annotations. The
approximation of the square_root_of_2 is four sexagesimal figures, which is
about six decimal figures. 1 + 24/60 + 51/602 + 10/603 = 1.41421296...[1]
Numerical analysis is the study of algorithms that use numerical approximation
(as opposed to symbolic_manipulations) for the problems of mathematical
analysis (as distinguished from discrete_mathematics). Numerical analysis
naturally finds application in all fields of engineering and the physical
sciences, but in the 21st century also the life sciences, social sciences,
medicine, business and even the arts have adopted elements of scientific
computations. The growth in computing power has revolutionized the use of
realistic mathematical models in science and engineering, and subtle numerical
analysis is required to implement these detailed models of the world. For
example, ordinary_differential_equations appear in celestial_mechanics
(predicting the motions of planets, stars and galaxies); numerical_linear
algebra is important for data analysis; stochastic_differential_equations and
Markov_chains are essential in simulating living cells for medicine and
biology.
Before the advent of modern computers, numerical_methods often depended on hand
interpolation formulas applied to data from large printed tables. Since the mid
20th century, computers calculate the required functions instead, but many of
the same formulas nevertheless continue to be used as part of the software
algorithms.
The numerical point of view goes back to the earliest mathematical writings. A
tablet from the Yale_Babylonian_Collection (YBC_7289), gives a sexagesimal
numerical approximation of the square_root_of_2, the length of the diagonal in
a unit_square. Computing the sides of a triangle in terms of square_roots is a
basic practical problem, for example in astronomy, carpentry, and construction.
[2]
Numerical analysis continues this long tradition: rather than exact symbolic
answers, which can only be applied to real-world measurements by translation
into digits, it gives approximate solutions within specified error bounds.
⁰
***** Contents *****
    * 1_General_introduction
          o 1.1_History
          o 1.2_Direct_and_iterative_methods
                # 1.2.1_Discretization_and_numerical_integration
          o 1.3_Discretization
    * 2_Generation_and_propagation_of_errors
          o 2.1_Round-off
          o 2.2_Truncation_and_discretization_error
          o 2.3_Numerical_stability_and_well-posed_problems
    * 3_Areas_of_study
          o 3.1_Computing_values_of_functions
          o 3.2_Interpolation,_extrapolation,_and_regression
          o 3.3_Solving_equations_and_systems_of_equations
          o 3.4_Solving_eigenvalue_or_singular_value_problems
          o 3.5_Optimization
          o 3.6_Evaluating_integrals
          o 3.7_Differential_equations
    * 4_Software
    * 5_See_also
    * 6_Notes
    * 7_References
          o 7.1_Citations
          o 7.2_Sources
    * 8_External_links
          o 8.1_Journals
          o 8.2_Online_texts
          o 8.3_Online_course_material
***** General introduction[edit] *****
The overall goal of the field of numerical analysis is the design and analysis
of techniques to give approximate but accurate solutions to hard problems, the
variety of which is suggested by the following:
    * Advanced numerical methods are essential in making numerical_weather
      prediction feasible.
    * Computing the trajectory of a spacecraft requires the accurate numerical
      solution of a system of ordinary differential equations.
    * Car companies can improve the crash safety of their vehicles by using
      computer simulations of car crashes. Such simulations essentially consist
      of solving partial_differential_equations numerically.
    * Hedge_funds (private investment funds) use tools from all fields of
      numerical analysis to attempt to calculate the value of stocks and
      derivatives more precisely than other market participants.
    * Airlines use sophisticated optimization algorithms to decide ticket
      prices, airplane and crew assignments and fuel needs. Historically, such
      algorithms were developed within the overlapping field of operations
      research.
    * Insurance companies use numerical programs for actuarial analysis.
The rest of this section outlines several important themes of numerical
analysis.
**** History[edit] ****
The field of numerical analysis predates the invention of modern computers by
many centuries. Linear_interpolation was already in use more than 2000 years
ago. Many great mathematicians of the past were preoccupied by numerical
analysis, as is obvious from the names of important algorithms like Newton's
method, Lagrange_interpolation_polynomial, Gaussian_elimination, or Euler's
method.
To facilitate computations by hand, large books were produced with formulas and
tables of data such as interpolation points and function coefficients. Using
these tables, often calculated out to 16 decimal places or more for some
functions, one could look up values to plug into the formulas given and achieve
very good numerical estimates of some functions. The canonical work in the
field is the NIST publication edited by Abramowitz_and_Stegun, a 1000-plus page
book of a very large number of commonly used formulas and functions and their
values at many points. The function values are no longer very useful when a
computer is available, but the large listing of formulas can still be very
handy.
The mechanical_calculator was also developed as a tool for hand computation.
These calculators evolved into electronic computers in the 1940s, and it was
then found that these computers were also useful for administrative purposes.
But the invention of the computer also influenced the field of numerical
analysis, since now longer and more complicated calculations could be done.
**** Direct and iterative methods[edit] ****
Direct vs iterative methods
Consider the problem of solving
      3x3 + 4 = 28
for the unknown quantity x.
        Direct method
                3x3 + 4 = 28.
Subtract 4      3x3 = 24.
Divide by 3     x3 =  8.
Take cube roots x =  2.
For the iterative method, apply the bisection_method to f(x) = 3x3 − 24. The initial
values are a = 0, b = 3, f(a) = −24, f(b) = 57.
     Iterative method
a     b    mid    f(mid)
0     3    1.5    −13.875
1.5   3    2.25   10.17...
1.5   2.25 1.875  −4.22...
1.875 2.25 2.0625 2.32...
From this table it can be concluded that the solution is between 1.875 and 2.0625.
The algorithm might return any number in that range with an error less than 0.2.
*** Discretization and numerical integration[edit] ***
[Schumacher_(Ferrari)_in_practice_at_USGP_2005.jpg]
In a two-hour race, the speed of the car is measured at three instants and recorded
in the following table.
Time 0:20 1:00 1:40
km/h 140  150  180
A discretization would be to say that the speed of the car was constant from 0:00 to
0:40, then from 0:40 to 1:20 and finally from 1:20 to 2:00. For instance, the total
distance traveled in the first 40 minutes is approximately (2/3 h × 140 km/
h) = 93.3 km. This would allow us to estimate the total distance traveled as 93.3 km
+ 100 km + 120 km = 313.3 km, which is an example of numerical integration (see
below) using a Riemann_sum, because displacement is the integral of velocity.
Ill-conditioned problem: Take the function f(x) = 1/(x − 1). Note that f(1.1) = 10
and f(1.001) = 1000: a change in x of less than 0.1 turns into a change in f(x) of
nearly 1000. Evaluating f(x) near x = 1 is an ill-conditioned problem.
Well-conditioned problem: By contrast, evaluating the same function f(x) = 1/(x − 1)
near x = 10 is a well-conditioned problem. For instance, f(10) = 1/9 â 0.111 and f
(11) = 0.1: a modest change in x leads to a modest change in f(x).
Direct methods compute the solution to a problem in a finite number of steps.
These methods would give the precise answer if they were performed in infinite
precision_arithmetic. Examples include Gaussian_elimination, the QR
factorization method for solving systems_of_linear_equations, and the simplex
method of linear_programming. In practice, finite_precision is used and the
result is an approximation of the true solution (assuming stability).
In contrast to direct methods, iterative_methods are not expected to terminate
in a finite number of steps. Starting from an initial guess, iterative methods
form successive approximations that converge to the exact solution only in the
limit. A convergence test, often involving the_residual, is specified in order
to decide when a sufficiently accurate solution has (hopefully) been found.
Even using infinite precision arithmetic these methods would not reach the
solution within a finite number of steps (in general). Examples include
Newton's method, the bisection_method, and Jacobi_iteration. In computational
matrix algebra, iterative methods are generally needed for large problems.
Iterative methods are more common than direct methods in numerical analysis.
Some methods are direct in principle but are usually used as though they were
not, e.g. GMRES and the conjugate_gradient_method. For these methods the number
of steps needed to obtain the exact solution is so large that an approximation
is accepted in the same manner as for an iterative method.
**** Discretization[edit] ****
Furthermore, continuous problems must sometimes be replaced by a discrete
problem whose solution is known to approximate that of the continuous problem;
this process is called 'discretization'. For example, the solution of a
differential_equation is a function. This function must be represented by a
finite amount of data, for instance by its value at a finite number of points
at its domain, even though this domain is a continuum.
***** Generation and propagation of errors[edit] *****
The study of errors forms an important part of numerical analysis. There are
several ways in which error can be introduced in the solution of the problem.
**** Round-off[edit] ****
Round-off_errors arise because it is impossible to represent all real_numbers
exactly on a machine with finite memory (which is what all practical digital
computers are).
**** Truncation and discretization error[edit] ****
Truncation_errors are committed when an iterative method is terminated or a
mathematical procedure is approximated, and the approximate solution differs
from the exact solution. Similarly, discretization induces a discretization
error because the solution of the discrete problem does not coincide with the
solution of the continuous problem. For instance, in the iteration in the
sidebar to compute the solution of     3  x  3   + 4 = 28   {\displaystyle 3x^
{3}+4=28}  [3x^{3}+4=28], after 10 or so iterations, it can be concluded that
the root is roughly 1.99 (for example). Therefore there is a truncation error
of 0.01.
Once an error is generated, it will generally propagate through the
calculation. For instance, already noted is that the operation + on a
calculator (or a computer) is inexact. It follows that a calculation of the
type     a + b + c + d + e   {\displaystyle a+b+c+d+e}  [{\displaystyle
a+b+c+d+e}] is even more inexact.
The truncation error is created when a mathematical procedure is approximated.
To integrate a function exactly it is required to find the sum of infinite
trapezoids, but numerically only the sum of only finite trapezoids can be
found, and hence the approximation of the mathematical procedure. Similarly, to
differentiate a function, the differential element approaches zero but
numerically only a finite value of the differential element can be chosen.
**** Numerical stability and well-posed problems[edit] ****
Numerical_stability is a notion in numerical analysis. An algorithm is called
'numerically stable' if an error, whatever its cause, does not grow to be much
larger during the calculation. This happens if the problem is 'well-
conditioned', meaning that the solution changes by only a small amount if the
problem data are changed by a small amount. To the contrary, if a problem is
'ill-conditioned', then any small error in the data will grow to be a large
error.
Both the original problem and the algorithm used to solve that problem can be
'well-conditioned' or 'ill-conditioned', and any combination is possible.
So an algorithm that solves a well-conditioned problem may be either
numerically stable or numerically unstable. An art of numerical analysis is to
find a stable algorithm for solving a well-posed mathematical problem. For
instance, computing the square root of 2 (which is roughly 1.41421) is a well-
posed problem. Many algorithms solve this problem by starting with an initial
approximation x0 to       2     {\displaystyle {\sqrt {2}}}  [{\sqrt {2}}], for
instance x0 = 1.4, and then computing improved guesses x1, x2, etc. One such
method is the famous Babylonian_method, which is given by xk+1 = xk/2 + 1/xk.
Another method, called 'method X', is given by xk+1 = (xk2 â 2)2 + xk.[note
1] A few iterations of each scheme are calculated in table form below, with
initial guesses x0 = 1.4 and x0 = 1.42.
Babylonian          Babylonian         Method X              Method X
x0 = 1.4            x0 = 1.42          x0 = 1.4              x0 = 1.42
x1 = 1.4142857...   x1 = 1.41422535... x1 = 1.4016           x1 = 1.42026896
x2 = 1.414213564... x2 =               x2 = 1.4028614...     x2 = 1.42056...
                    1.41421356242...
                                       ...                   ...
                                       x1000000 = 1.41421... x27 = 7280.2284...
Observe that the Babylonian method converges quickly regardless of the initial
guess, whereas Method X converges extremely slowly with initial guess x0 = 1.4
and diverges for initial guess x0 = 1.42. Hence, the Babylonian method is
numerically stable, while Method X is numerically unstable.
      Numerical stability is affected by the number of the significant digits
      the machine keeps on, if a machine is used that keeps only the four most
      significant decimal digits, a good example on loss of significance can be
      given by these two equivalent functions
         f ( x ) = x  (    x + 1   &#x2212;   x    )   &#xA0;and&#xA0;  g ( x )
      =   x    x + 1   +   x      .   {\displaystyle f(x)=x\left({\sqrt {x+1}}-
      {\sqrt {x}}\right){\text{ and }}g(x)={\frac {x}{{\sqrt {x+1}}+{\sqrt
      {x}}}}.}  [
      f(x)=x\left(\sqrt{x+1}-\sqrt{x}\right)
      \text{ and } g(x)=\frac{x}{\sqrt{x+1}+\sqrt{x}}.
      ]
      Comparing the results of
               f ( 500 ) = 500  (    501   &#x2212;   500    )  = 500  (  22.38
            &#x2212; 22.36  )  = 500 ( 0.02 ) = 10   {\displaystyle f
            (500)=500\left({\sqrt {501}}-{\sqrt {500}}\right)=500\left(22.38-
            22.36\right)=500(0.02)=10}  [ f(500)=500 \left(\sqrt{501}-\sqrt
            {500} \right)=500 \left(22.38-22.36 \right)=500(0.02)=10]
      and
             g ( 500 )    =   500    501   +   500            =   500  22.38 +
      22.36          =   500 44.74   = 11.17       {\displaystyle {\begin
      {alignedat}{3}g(500)&={\frac {500}{{\sqrt {501}}+{\sqrt {500}}}}\\&=
      {\frac {500}{22.38+22.36}}\\&={\frac {500}{44.74}}=11.17\end{alignedat}}}
      [
      \begin{alignat}{3}g(500)&=\frac{500}{\sqrt{501}+\sqrt{500}}\\
            &=\frac{500}{22.38+22.36}\\
            &=\frac{500}{44.74}=11.17
      \end{alignat}
      ]
      by comparing the two results above, it is clear that loss_of_significance
      (caused here by 'catastrophic cancelation') has a huge effect on the
      results, even though both functions are equivalent, as shown below
                   f ( x )    = x  (    x + 1   &#x2212;   x    )        = x
            (    x + 1   &#x2212;   x    )       x + 1   +   x       x + 1   +
            x            = x    (   x + 1    )  2   &#x2212; (   x    )  2
            x + 1   +   x            = x    x + 1 &#x2212; x     x + 1   +   x
            = x   1    x + 1   +   x            =   x    x + 1   +   x
            = g ( x )       {\displaystyle {\begin{alignedat}{4}f(x)&=x\left(
            {\sqrt {x+1}}-{\sqrt {x}}\right)\\&=x\left({\sqrt {x+1}}-{\sqrt
            {x}}\right){\frac {{\sqrt {x+1}}+{\sqrt {x}}}{{\sqrt {x+1}}+{\sqrt
            {x}}}}\\&=x{\frac {({\sqrt {x+1}})^{2}-({\sqrt {x}})^{2}}{{\sqrt
            {x+1}}+{\sqrt {x}}}}\\&=x{\frac {x+1-x}{{\sqrt {x+1}}+{\sqrt
            {x}}}}\\&=x{\frac {1}{{\sqrt {x+1}}+{\sqrt {x}}}}\\&={\frac {x}{
            {\sqrt {x+1}}+{\sqrt {x}}}}\\&=g(x)\end{alignedat}}}  [
            {\displaystyle {\begin{alignedat}{4}f(x)&=x\left({\sqrt {x+1}}-
            {\sqrt {x}}\right)\\&=x\left({\sqrt {x+1}}-{\sqrt {x}}\right){\frac
            {{\sqrt {x+1}}+{\sqrt {x}}}{{\sqrt {x+1}}+{\sqrt {x}}}}\\&=x{\frac
            {({\sqrt {x+1}})^{2}-({\sqrt {x}})^{2}}{{\sqrt {x+1}}+{\sqrt
            {x}}}}\\&=x{\frac {x+1-x}{{\sqrt {x+1}}+{\sqrt {x}}}}\\&=x{\frac
            {1}{{\sqrt {x+1}}+{\sqrt {x}}}}\\&={\frac {x}{{\sqrt {x+1}}+{\sqrt
            {x}}}}\\&=g(x)\end{alignedat}}}]
      The desired value, computed using infinite precision, is 11.174755...
    * The example is a modification of one taken from Mathew; Numerical methods
      using Matlab, 3rd ed.
***** Areas of study[edit] *****
The field of numerical analysis includes many sub-disciplines. Some of the
major ones are:
**** Computing values of functions[edit] ****
Interpolation: Observing that the temperature varies from 20 degrees Celsius at
1:00 to 14 degrees at 3:00, a linear interpolation of this data would conclude
that it was 17 degrees at 2:00 and 18.5 degrees at 1:30pm.
Extrapolation: If the gross_domestic_product of a country has been growing an
average of 5% per year and was 100 billion last year, it might extrapolated
that it will be 105 billion this year.
[A_line_through_20_points]
Regression: In linear regression, given n points, a line is computed that
passes as close as possible to those n points.
[How_much_for_a_glass_of_lemonade?]
Optimization: Say lemonade is sold at a lemonade_stand, at $1 197 glasses of
lemonade can be sold per day, and that for each increase of $0.01, one glass of
lemonade less will be sold per day. If $1.485 could be charged, profit would be
maximized but due to the constraint of having to charge a whole cent amount,
charging $1.48 or $1.49 per glass will both yield the maximum income of $220.52
per day.
[Wind_direction_in_blue,_true_trajectory_in_black,_Euler_method_in_red.]
Differential equation: If 100 fans are set up to blow air from one end of the
room to the other and then a feather isdropped into the wind, what happens? The
feather will follow the air currents, which may be very complex. One
approximation is to measure the speed at which the air is blowing near the
feather every second, and advance the simulated feather as if it were moving in
a straight line at that same speed for one second, before measuring the wind
speed again. This is called the Euler_method for solving an ordinary
differential equation.
One of the simplest problems is the evaluation of a function at a given point.
The most straightforward approach, of just plugging in the number in the
formula is sometimes not very efficient. For polynomials, a better approach is
using the Horner_scheme, since it reduces the necessary number of
multiplications and additions. Generally, it is important to estimate and
control round-off_errors arising from the use of floating_point arithmetic.
**** Interpolation, extrapolation, and regression[edit] ****
Interpolation solves the following problem: given the value of some unknown
function at a number of points, what value does that function have at some
other point between the given points?
Extrapolation is very similar to interpolation, except that now the value of
the unknown function at a point which is outside the given points must be
found.
Regression is also similar, but it takes into account that the data is
imprecise. Given some points, and a measurement of the value of some function
at these points (with an error), the unknown function can be found. The least
squares-method is one way to achieve this.
**** Solving equations and systems of equations[edit] ****
Another fundamental problem is computing the solution of some given equation.
Two cases are commonly distinguished, depending on whether the equation is
linear or not. For instance, the equation     2 x + 5 = 3   {\displaystyle
2x+5=3}  [2x+5=3] is linear while     2  x  2   + 5 = 3   {\displaystyle 2x^
{2}+5=3}  [2x^2+5=3] is not.
Much effort has been put in the development of methods for solving systems_of
linear_equations. Standard direct methods, i.e., methods that use some matrix
decomposition are Gaussian_elimination, LU_decomposition, Cholesky
decomposition for symmetric (or hermitian) and positive-definite_matrix, and QR
decomposition for non-square matrices. Iterative methods such as the Jacobi
method, GaussâSeidel_method, successive_over-relaxation and conjugate
gradient_method are usually preferred for large systems. General iterative
methods can be developed using a matrix_splitting.
Root-finding_algorithms are used to solve nonlinear equations (they are so
named since a root of a function is an argument for which the function yields
zero). If the function is differentiable and the derivative is known, then
Newton's method is a popular choice. Linearization is another technique for
solving nonlinear equations.
**** Solving eigenvalue or singular value problems[edit] ****
Several important problems can be phrased in terms of eigenvalue_decompositions
or singular_value_decompositions. For instance, the spectral_image_compression
algorithm[3] is based on the singular value decomposition. The corresponding
tool in statistics is called principal_component_analysis.
**** Optimization[edit] ****
Main article: Mathematical_optimization
Optimization problems ask for the point at which a given function is maximized
(or minimized). Often, the point also has to satisfy some constraints.
The field of optimization is further split in several subfields, depending on
the form of the objective function and the constraint. For instance, linear
programming deals with the case that both the objective function and the
constraints are linear. A famous method in linear programming is the simplex
method.
The method of Lagrange_multipliers can be used to reduce optimization problems
with constraints to unconstrained optimization problems.
**** Evaluating integrals[edit] ****
Main article: Numerical_integration
Numerical integration, in some instances also known as numerical quadrature,
asks for the value of a definite integral. Popular methods use one of the
NewtonâCotes_formulas (like the midpoint rule or Simpson's_rule) or Gaussian
quadrature. These methods rely on a "divide and conquer" strategy, whereby an
integral on a relatively large set is broken down into integrals on smaller
sets. In higher dimensions, where these methods become prohibitively expensive
in terms of computational effort, one may use Monte_Carlo or quasi-Monte_Carlo
methods (see Monte_Carlo_integration), or, in modestly large dimensions, the
method of sparse_grids.
**** Differential equations[edit] ****
Main articles: Numerical_ordinary_differential_equations and Numerical_partial
differential_equations
Numerical analysis is also concerned with computing (in an approximate way) the
solution of differential equations, both ordinary differential equations and
partial differential equations.
Partial differential equations are solved by first discretizing the equation,
bringing it into a finite-dimensional subspace. This can be done by a finite
element_method, a finite_difference method, or (particularly in engineering) a
finite_volume_method. The theoretical justification of these methods often
involves theorems from functional_analysis. This reduces the problem to the
solution of an algebraic equation.
***** Software[edit] *****
Main articles: List_of_numerical_analysis_software and Comparison_of_numerical
analysis_software
Since the late twentieth century, most algorithms are implemented in a variety
of programming languages. The Netlib repository contains various collections of
software routines for numerical problems, mostly in Fortran and C. Commercial
products implementing many different numerical algorithms include the IMSL and
NAG libraries; a free-software alternative is the GNU_Scientific_Library.
There are several popular numerical computing applications such as MATLAB, TK
Solver, S-PLUS, and IDL as well as free and open source alternatives such as
FreeMat, Scilab, GNU_Octave (similar to Matlab), and IT++ (a C++ library).
There are also programming languages such as R (similar to S-PLUS) and Python
with libraries such as NumPy, SciPy and SymPy. Performance varies widely: while
vector and matrix operations are usually fast, scalar loops may vary in speed
by more than an order of magnitude.[4][5]
Many computer_algebra_systems such as Mathematica also benefit from the
availability of arbitrary-precision_arithmetic which can provide more accurate
results.
Also, any spreadsheet software can be used to solve simple problems relating to
numerical analysis.
***** See also[edit] *****
    * Analysis_of_algorithms
    * Computational_science
    * Interval_arithmetic
    * List_of_numerical_analysis_topics
    * Numerical_differentiation
    * Numerical_Recipes
    * Symbolic-numeric_computation
***** Notes[edit] *****
   1. ^ This is a fixed_point_iteration for the equation     x = (  x  2
      &#x2212; 2  )  2   + x = f ( x )   {\displaystyle x=(x^{2}-2)^{2}+x=f(x)}
      [x=(x^2-2)^2+x=f(x)], whose solutions include       2     {\displaystyle
      {\sqrt {2}}}  [{\sqrt {2}}]. The iterates always move to the right since
      f ( x ) &#x2265; x   {\displaystyle f(x)\geq x}  [f(x)\geq x]. Hence
      x  1   = 1.4 <   2     {\displaystyle x_{1}=1.4<{\sqrt {2}}}
      [x_1=1.4<\sqrt{2}] converges and      x  1   = 1.42 >   2
      {\displaystyle x_{1}=1.42>{\sqrt {2}}}  [x_1=1.42>\sqrt{2}] diverges.
***** References[edit] *****
**** Citations[edit] ****
   1. ^ Photograph,_illustration,_and_description_of_the_root(2)_tablet_from
      the_Yale_Babylonian_Collection
   2. ^ The New Zealand Qualification authority specifically mentions this
      skill in document 13004 version 2, dated 17 October 2003 titled CARPENTRY
      THEORY:_Demonstrate_knowledge_of_setting_out_a_building
   3. ^ The_Singular_Value_Decomposition_and_Its_Applications_in_Image
      Compression Archived 4 October 2006 at the Wayback_Machine
   4. ^ Speed_comparison_of_various_number_crunching_packages Archived 5
      October 2006 at the Wayback_Machine
   5. ^ Comparison_of_mathematical_programs_for_data_analysis Stefan Steinhaus,
      ScientificWeb.com
**** Sources[edit] ****
    * Golub,_Gene_H.; Charles_F._Van_Loan (1986). Matrix Computations (3rd
      ed.). Johns Hopkins University Press. ISBN 0-8018-5413-X.
Higham,_Nicholas_J. (1996). Accuracy and Stability of Numerical Algorithms.
Society for Industrial and Applied Mathematics. ISBN 0-89871-355-2.
Hildebrand,_F._B. (1974). Introduction to Numerical Analysis (2nd ed.). McGraw-
Hill. ISBN 0-07-028761-9.
Leader,_Jeffery_J. (2004). Numerical Analysis and Scientific Computation.
Addison Wesley. ISBN 0-201-73499-0.
Wilkinson,_J.H. (1965). The Algebraic Eigenvalue Problem. Clarendon Press.
Kahan,_W. (1972). A survey of error-analysis. Proc. IFIP Congress 71 in
Ljubljana. Info. Processing 71. vol. 2. Amsterdam: North-Holland Publishing.
pp. 1214â39.
 (examples of the importance of accurate arithmetic).
Trefethen,_Lloyd_N. (2006). "Numerical_analysis", 20 pages. In: Timothy Gowers
and June Barrow-Green (editors), Princeton Companion of Mathematics, Princeton
University Press.
***** External links[edit] *****
Numerical analysisat Wikipedia's sister_projects
    * Media from Wikimedia Commons
    * Quotations from Wikiquote
    * Textbooks from Wikibooks
**** Journals[edit] ****
    * gdz.sub.uni-goettingen, Numerische Mathematik, volumes 1-66, Springer,
      1959-1994 (searchable; pages are images). (in English) (in German)
    * springerlink.com, Numerische Mathematik, volumes 1-112, Springer,
      1959â2009
    * SIAM_Journal_on_Numerical_Analysis, volumes 1-47, SIAM, 1964â2009
**** Online texts[edit] ****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Numerical_analysis",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Numerical_Recipes, William H. Press (free, downloadable previous editions)
First_Steps_in_Numerical_Analysis (archived), R.J.Hosking, S.Joe, D.C.Joyce,
and J.C.Turner
CSEP_(Computational_Science_Education_Project), U.S._Department_of_Energy
**** Online course material[edit] ****
    * Numerical_Methods, Stuart Dalziel University_of_Cambridge
    * Lectures_on_Numerical_Analysis, Dennis Deturck and Herbert S. Wilf
      University_of_Pennsylvania
    * Numerical_methods, John D. Fenton University_of_Karlsruhe
    * Numerical_Methods_for_Physicists, Anthony OâHare Oxford_University
    * Lectures_in_Numerical_Analysis (archived), R. Radok Mahidol_University
    * Introduction_to_Numerical_Analysis_for_Engineering, Henrik Schmidt
      Massachusetts_Institute_of_Technology
    * Numerical_Analysis_for_Engineering, D. W. Harder University_of_Waterloo
    * v
    * t
    * e
Areas_of_mathematics
                  * Category_theory
                  * Information_theory
Foundations       * Mathematical_logic
                  * Philosophy_of_mathematics
                  * Set_theory
                  * Abstract
Algebra           * Elementary
                  * Linear
                  * Multilinear
                  * Calculus
                  * Real_analysis
Analysis          * Complex_analysis
                  * Differential_equations
                  * Functional_analysis
                  * Combinatorics
Discrete          * Graph_theory
                  * Order_theory
                  * Game_theory
                  * Algebraic
                  * Analytic
Geometry          * Differential
                  * Discrete
                  * Euclidean
                  * Finite
                  * Arithmetic
Number_theory     * Algebraic_number_theory
                  * Analytic_number_theory
                  * Diophantine_geometry
                  * Algebraic
Topology          * Differential
                  * Geometric
                  * Control_theory
                  * Mathematical_economics
                  * Mathematical_finance
Applied           * Mathematical_physics
                  * Mathematical_statistics
                  * Probability
                  * Statistics
                  * Computer_science
                  * Theory_of_computation
Computational     * Numerical analysis
                  * Optimization
                  * Computer_algebra
                  * History_of_mathematics
Others            * Recreational_mathematics
                  * Mathematics_and_art
                  * Mathematics_education
    * [Category] Category
    * [Portal] Portal
    * [Commons page]Commons
    * [WikiProject]WikiProject
    * v
    * t
    * e
Branches_of_physics
                      * Theoretical
                            o Phenomenology
Divisions             * Computational
                      * Experimental
                      * Applied
                                            * Continuum
                  Classical_mechanics             o Solid
                                                  o Fluid
                                            * Acoustics
                                            * Electrostatics
                  Electrodynamics           * Magnetostatics
                                            * Plasma_physics
Classical                                   * Accelerator_physics
                                            * Thermodynamics
                                            * Condensed_matter
                                                  o Materials
                  Statistical_mechanics           o Mesoscopic
                                                  o Polymers
                                                  o Soft
                                                  o Solid-state
                                          * Quantum_electrodynamics
                  Quantum_mechanics       * Quantum_field_theory
                                          * Quantum_gravity
                                          * Quantum_information
                  Relativity              * General
                                          * Special
                                          * Astroparticle
                  Particle_physics        * Nuclear
                                          * Quantum_chromodynamics
Modern                                    * Atomic_physics
                  Atomic,_molecular       * Molecular_physics
                  and_optical_physics     * Optics
                                          * Photonics
                                          * Quantum_optics
                                          * Astrophysics
                                                o Nuclear
                  Cosmology               * Celestial_mechanics
                                          * Solar
                                                o Heliophysics
                                          * Space_physics
                      * Agrophysics
                      * Biophysics
                            o Medical
                            o Neurophysics
                      * Engineering
                      * Geophysics
Interdisciplinary           o Atmospheric
                            o Cloud
                      * Mathematical
                      * Physical_chemistry
                            o Chemical_physics
                      * Quantum_computing
                      * Social_physics
                            o Econophysics
                      * History_of_physics
See also              * Nobel_Prize_in_Physics
                      * Timeline_of_physics_discoveries
                      * Theory_of_everything
    * v
    * t
    * e
Computer_science
Note: This template roughly follows the 2012 ACM_Computing_Classification
System.
                          * Printed_circuit_board
                          * Peripheral
                          * Integrated_circuit
Hardware                  * Very_Large_Scale_Integration
                          * Systems_on_Chip_(SoCs)
                          * Energy_consumption_(Green_computing)
                          * Electronic_design_automation
                          * Hardware_acceleration
                          * Computer_architecture
Computer systems          * Embedded_system
organization              * Real-time_computing
                          * Dependability
                          * Network_architecture
                          * Network_protocol
Networks                  * Network_components
                          * Network_scheduler
                          * Network_performance_evaluation
                          * Network_service
                          * Interpreter
                          * Middleware
Software organization     * Virtual_machine
                          * Operating_system
                          * Software_quality
                          * Programming_paradigm
                          * Programming_language
                          * Compiler
                          * Domain-specific_language
Software_notations        * Modeling_language
and tools                 * Software_framework
                          * Integrated_development_environment
                          * Software_configuration_management
                          * Software_library
                          * Software_repository
                          * Software_development_process
                          * Requirements_analysis
                          * Software_design
Software_development      * Software_construction
                          * Software_deployment
                          * Software_maintenance
                          * Programming_team
                          * Open-source_model
                          * Model_of_computation
                          * Formal_language
Theory_of_computation     * Automata_theory
                          * Computational_complexity_theory
                          * Logic
                          * Semantics
                          * Algorithm_design
                          * Analysis_of_algorithms
Algorithms                * Algorithmic_efficiency
                          * Randomized_algorithm
                          * Computational_geometry
                          * Discrete_mathematics
                          * Probability
Mathematics               * Statistics
of computing              * Mathematical_software
                          * Information_theory
                          * Mathematical_analysis
                          * Numerical analysis
                          * Database_management_system
                          * Information_storage_systems
                          * Enterprise_information_system
                          * Social_information_systems
                          * Geographic_information_system
                          * Decision_support_system
Information               * Process_control_system
systems                   * Multimedia_information_system
                          * Data_mining
                          * Digital_library
                          * Computing_platform
                          * Digital_marketing
                          * World_Wide_Web
                          * Information_retrieval
                          * Cryptography
                          * Formal_methods
                          * Security_services
Security                  * Intrusion_detection_system
                          * Hardware_security
                          * Network_security
                          * Information_security
                          * Application_security
                          * Interaction_design
Humanâcomputer       * Social_computing
interaction               * Ubiquitous_computing
                          * Visualization
                          * Accessibility
                          * Concurrent_computing
                          * Parallel_computing
Concurrency               * Distributed_computing
                          * Multithreading
                          * Multiprocessing
                          * Natural_language_processing
                          * Knowledge_representation_and_reasoning
                          * Computer_vision
Artificial                * Automated_planning_and_scheduling
intelligence              * Search_methodology
                          * Control_method
                          * Philosophy_of_artificial_intelligence
                          * Distributed_artificial_intelligence
                          * Supervised_learning
                          * Unsupervised_learning
Machine_learning          * Reinforcement_learning
                          * Multi-task_learning
                          * Cross-validation
                          * Animation
                          * Rendering
                          * Image_manipulation
Graphics                  * Graphics_processing_unit
                          * Mixed_reality
                          * Virtual_reality
                          * Image_compression
                          * Solid_modeling
                          * E-commerce
                          * Enterprise_software
                          * Computational_mathematics
                          * Computational_physics
                          * Computational_chemistry
                          * Computational_biology
                          * Computational_social_science
                          * Computational_engineering
Applied                   * Computational_healthcare
computing                 * Digital_art
                          * Electronic_publishing
                          * Cyberwarfare
                          * Electronic_voting
                          * Video_games
                          * Word_processing
                          * Operations_research
                          * Educational_technology
                          * Document_management
    * [Wikipedia book] Book
    * [Category] Category
    * [Portal] Portal
    * [Outline] Outline
    * [WikiProject]WikiProject
    * [Commons page] Commons
Authority_control [Edit_this_at_Wikidata]     * GND: 4042805-9

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Numerical_analysis&oldid=909166460"
Categories:
    * Numerical_analysis
    * Mathematical_physics
    * Computational_science
Hidden categories:
    * Webarchive_template_wayback_links
    * Articles_to_be_merged_from_January_2019
    * All_articles_to_be_merged
    * Articles_lacking_in-text_citations_from_November_2013
    * All_articles_lacking_in-text_citations
    * Use_dmy_dates_from_July_2012
    * CS1:_long_volume_value
    * Articles_with_German-language_external_links
    * Wikipedia_articles_with_GND_identifiers
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
    * Wikiversity
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Afrikaans
    * Alemannisch
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AragonÃ©s
    * Asturianu
    * à¦¬à¦¾à¦à¦²à¦¾
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÐ°ÑÒ¡Ð¾ÑÑÑÐ°
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * Fiji_Hindi
    * FranÃ§ais
    * Gaeilge
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Latina
    * LatvieÅ¡u
    * LÃ«tzebuergesch
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Bahasa_Melayu
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * æ¥æ¬èª
    * Nordfriisk
    * Norsk
    * Norsk_nynorsk
    * Occitan
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Ù¾ÙØ¬Ø§Ø¨Û
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Sardu
    * à·à·à¶à·à¶½
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Basa_Sunda
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * Winaray
    * å´è¯­
    * ××Ö´×××©
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 3 August 2019, at 15:44 (UTC).
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
