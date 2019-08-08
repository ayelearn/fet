The following text has been accessed from https://en.wikipedia.org/wiki/Condition_number at Thu Aug 8 23:20:55 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Condition number ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In the field of numerical_analysis, the condition number of a function measures
how much the output value of the function can change for a small change in the
input argument. This is used to measure how sensitive a function is to changes
or errors in the input, and how much error in the output results from an error
in the input. Very frequently, one is solving the inverse problem â given
f ( x ) = y ,   {\displaystyle f(x)=y,}  [f(x) = y,] one is solving for x, and
thus the condition number of the (local) inverse must be used. In linear
regression the condition number of the moment_matrix can be used as a
diagnostic for multicollinearity.[1][2]
The condition number is an application of the derivative, and is formally
defined as the value of the asymptotic worst-case relative change in output for
a relative change in input. The "function" is the solution of a problem and the
"arguments" are the data in the problem. The condition number is frequently
applied to questions in linear algebra, in which case the derivative is
straightforward but the error could be in many different directions, and is
thus computed from the geometry of the matrix. More generally, condition
numbers can be defined for non-linear functions in several variables.
A problem with a low condition number is said to be well-conditioned, while a
problem with a high condition number is said to be ill-conditioned. The
condition number is a property of the problem. Paired with the problem are any
number of algorithms that can be used to solve the problem, that is, to
calculate the solution. Some algorithms have a property called backward
stability. In general, a backward stable algorithm can be expected to
accurately solve well-conditioned problems. Numerical analysis textbooks give
formulas for the condition numbers of problems and identify known backward
stable algorithms.
As a rule of thumb, if the condition number     &#x03BA; ( A ) =  10  k
{\displaystyle \kappa (A)=10^{k}}  [\kappa(A) = 10^k], then you may lose up to
k   {\displaystyle k}  [k] digits of accuracy on top of what would be lost to
the numerical method due to loss of precision from arithmetic methods.[3]
However, the condition number does not give the exact value of the maximum
inaccuracy that may occur in the algorithm. It generally just bounds it with an
estimate (whose computed value depends on the choice of the norm to measure the
inaccuracy).
⁰
***** Contents *****
    * 1_General_definition_in_the_context_of_error_analysis
    * 2_Matrices
    * 3_Nonlinear
          o 3.1_One_variable
          o 3.2_Several_variables
    * 4_See_also
    * 5_References
    * 6_External_links
***** General definition in the context of error analysis[edit] *****
Given a problem f and an algorithm        f &#x007E;      {\displaystyle
{\tilde {f}}}  [{\tilde {f}}] with an input x, the absolute error is
&#x2016;  f ( x ) &#x2212;    f &#x007E;    ( x )  &#x2016;    {\displaystyle
\left\|f(x)-{\tilde {f}}(x)\right\|}  [{\displaystyle \left\|f(x)-{\tilde {f}}
(x)\right\|}] and the relative error is      &#x2016;  f ( x ) &#x2212;    f
&#x007E;    ( x )  &#x2016;   /   &#x2016;  f ( x )  &#x2016;    {\displaystyle
\left\|f(x)-{\tilde {f}}(x)\right\|/\left\|f(x)\right\|}  [{\displaystyle
\left\|f(x)-{\tilde {f}}(x)\right\|/\left\|f(x)\right\|}].
In this context, the absolute condition number of a problem f is
          lim  &#x03B5; &#x2192; 0    sup  &#x2016; &#x03B4; x &#x2016;
      &#x2264; &#x03B5;      &#x2016; &#x03B4; f &#x2016;   &#x2016; &#x03B4; x
      &#x2016;      {\displaystyle \lim _{\varepsilon \rightarrow 0}\sup _
      {\|\delta x\|\leq \varepsilon }{\frac {\|\delta f\|}{\|\delta x\|}}}  [
      {\displaystyle \lim _{\varepsilon \rightarrow 0}\sup _{\|\delta x\|\leq
      \varepsilon }{\frac {\|\delta f\|}{\|\delta x\|}}}]
and the relative condition number is
          lim  &#x03B5; &#x2192; 0    sup  &#x2016; &#x03B4; x &#x2016;
      &#x2264; &#x03B5;      &#x2016; &#x03B4; f ( x ) &#x2016;  /  &#x2016; f
      ( x ) &#x2016;   &#x2016; &#x03B4; x &#x2016;  /  &#x2016; x &#x2016;
      {\displaystyle \lim _{\varepsilon \rightarrow 0}\sup _{\|\delta x\|\leq
      \varepsilon }{\frac {\|\delta f(x)\|/\|f(x)\|}{\|\delta x\|/\|x\|}}}  [
      {\displaystyle \lim _{\varepsilon \rightarrow 0}\sup _{\|\delta x\|\leq
      \varepsilon }{\frac {\|\delta f(x)\|/\|f(x)\|}{\|\delta x\|/\|x\|}}}]
***** Matrices[edit] *****
For example, the condition number associated with the linear_equation Ax = b
gives a bound on how inaccurate the solution x will be after approximation.
Note that this is before the effects of round-off_error are taken into account;
conditioning is a property of the matrix, not the algorithm or floating_point
accuracy of the computer used to solve the corresponding system. In particular,
one should think of the condition number as being (very roughly) the rate at
which the solution, x, will change with respect to a change in b. Thus, if the
condition number is large, even a small error in b may cause a large error in
x. On the other hand, if the condition number is small then the error in x will
not be much bigger than the error in b.
The condition number is defined more precisely to be the maximum ratio of the
relative_error in x to the relative error in b.
Let e be the error in b. Assuming that A is a nonsingular matrix, the error in
the solution Aâ1b is Aâ1e. The ratio of the relative error in the solution
to the relative error in b is
             &#x2016;   A  &#x2212; 1   e  &#x2016;   &#x2016;   A  &#x2212; 1
      b  &#x2016;     &#x2016; e &#x2016;   &#x2016; b &#x2016;
      {\displaystyle {\frac {\frac {\left\|A^{-1}e\right\|}{\left\|A^{-
      1}b\right\|}}{\frac {\|e\|}{\|b\|}}}}  [{\displaystyle {\frac {\frac
      {\left\|A^{-1}e\right\|}{\left\|A^{-1}b\right\|}}{\frac {\|e\|}
      {\|b\|}}}}]
This is easily transformed to
            &#x2016;   A  &#x2212; 1   e  &#x2016;   &#x2016; e &#x2016;
      &#x2016; b &#x2016;   &#x2016;   A  &#x2212; 1   b  &#x2016;    .
      {\displaystyle {\frac {\left\|A^{-1}e\right\|}{\|e\|}}{\frac {\|b\|}
      {\left\|A^{-1}b\right\|}}.}  [{\displaystyle {\frac {\left\|A^{-
      1}e\right\|}{\|e\|}}{\frac {\|b\|}{\left\|A^{-1}b\right\|}}.}]
The maximum value (for nonzero b and e) is then seen to be the product of the
two operator_norms as follows:
              max  e , b &#x2260; 0    {     &#x2016;   A  &#x2212; 1   e
      &#x2016;   &#x2016; e &#x2016;       &#x2016; b &#x2016;   &#x2016;   A
      &#x2212; 1   b  &#x2016;     }     =  max  e &#x2260; 0    {    &#x2016;
      A  &#x2212; 1   e  &#x2016;   &#x2016; e &#x2016;    }    max  b &#x2260;
      0    {    &#x2016; b &#x2016;   &#x2016;   A  &#x2212; 1   b  &#x2016;
      }        =  max  e &#x2260; 0    {    &#x2016;   A  &#x2212; 1   e
      &#x2016;   &#x2016; e &#x2016;    }    max  x &#x2260; 0    {    &#x2016;
      A x &#x2016;   &#x2016; x &#x2016;    }        =  &#x2016;  A  &#x2212; 1
      &#x2016;   &#x2016; A &#x2016;       {\displaystyle {\begin{aligned}\max
      _{e,b\neq 0}\left\{{\frac {\left\|A^{-1}e\right\|}{\|e\|}}{\frac {\|b\|}
      {\left\|A^{-1}b\right\|}}\right\}&=\max _{e\neq 0}\left\{{\frac
      {\left\|A^{-1}e\right\|}{\|e\|}}\right\}\,\max _{b\neq 0}\left\{{\frac
      {\|b\|}{\left\|A^{-1}b\right\|}}\right\}\\&=\max _{e\neq 0}\left\{{\frac
      {\left\|A^{-1}e\right\|}{\|e\|}}\right\}\,\max _{x\neq 0}\left\{{\frac
      {\|Ax\|}{\|x\|}}\right\}\\&=\left\|A^{-1}\right\|\,\|A\|\end{aligned}}}
      [{\displaystyle {\begin{aligned}\max _{e,b\neq 0}\left\{{\frac {\left\|A^
      {-1}e\right\|}{\|e\|}}{\frac {\|b\|}{\left\|A^{-
      1}b\right\|}}\right\}&=\max _{e\neq 0}\left\{{\frac {\left\|A^{-
      1}e\right\|}{\|e\|}}\right\}\,\max _{b\neq 0}\left\{{\frac {\|b\|}
      {\left\|A^{-1}b\right\|}}\right\}\\&=\max _{e\neq 0}\left\{{\frac
      {\left\|A^{-1}e\right\|}{\|e\|}}\right\}\,\max _{x\neq 0}\left\{{\frac
      {\|Ax\|}{\|x\|}}\right\}\\&=\left\|A^{-1}\right\|\,\|A\|\end{aligned}}}]
The same definition is used for any consistent norm, i.e. one that satisfies
         &#x03BA; ( A ) =  &#x2016;  A  &#x2212; 1   &#x2016;    &#x2016; A
      &#x2016;  &#x2265;  &#x2016;   A  &#x2212; 1   A  &#x2016;  = 1.
      {\displaystyle \kappa (A)=\left\|A^{-1}\right\|\,\left\|A\right\|\geq
      \left\|A^{-1}A\right\|=1.}  [{\displaystyle \kappa (A)=\left\|A^{-
      1}\right\|\,\left\|A\right\|\geq \left\|A^{-1}A\right\|=1.}]
When the condition number is exactly one (which can only happen if A is a
scalar multiple of a linear_isometry), then a solution algorithm can find (in
principle, meaning if the algorithm introduces no errors of its own) an
approximation of the solution whose precision is no worse than that of the
data.
However, it does not mean that the algorithm will converge rapidly to this
solution, just that it won't diverge arbitrarily because of inaccuracy on the
source data (backward error), provided that the forward error introduced by the
algorithm does not diverge as well because of accumulating intermediate
rounding errors.[clarification_needed]
The condition number may also be infinite, but this implies that the problem is
ill-posed (does not possess a unique, well-defined solution for each choice of
data; that is, the matrix is not invertible), and no algorithm can be expected
to reliably find a solution.
The definition of the condition number depends on the choice of norm, as can be
illustrated by two examples.
If     &#x2016; &#x22C5; &#x2016;   {\displaystyle \|\cdot \|}  [{\displaystyle
\|\cdot \|}] is the norm defined in the square-summable sequence_space â2
(which matches the usual distance in a standard Euclidean space and is usually
noted as     &#x2016; &#x22C5;  &#x2016;  2     {\displaystyle \|\cdot \|_{2}}
[{\displaystyle \|\cdot \|_{2}}]), then
         &#x03BA; ( A ) =     &#x03C3;  max   ( A )    &#x03C3;  min   ( A )
      ,   {\displaystyle \kappa (A)={\frac {\sigma _{\max }(A)}{\sigma _{\min }
      (A)}},}  [{\displaystyle \kappa (A)={\frac {\sigma _{\max }(A)}{\sigma _
      {\min }(A)}},}]
where      &#x03C3;  max   ( A )   {\displaystyle \sigma _{\max }(A)}
[ \sigma_{\max}(A)] and      &#x03C3;  min   ( A )   {\displaystyle \sigma _
{\min }(A)}  [{\displaystyle \sigma _{\min }(A)}] are maximal and minimal
singular_values of     A   {\displaystyle A}  [A] respectively. Hence
    * If     A   {\displaystyle A}  [A] is normal then
               &#x03BA; ( A ) =    |   &#x03BB;  max   ( A )  |   |   &#x03BB;
            min   ( A )  |    ,   {\displaystyle \kappa (A)={\frac
            {\left|\lambda _{\max }(A)\right|}{\left|\lambda _{\min }
            (A)\right|}},}  [{\displaystyle \kappa (A)={\frac {\left|\lambda _
            {\max }(A)\right|}{\left|\lambda _{\min }(A)\right|}},}]
      where      &#x03BB;  max   ( A )   {\displaystyle \lambda _{\max }(A)}  [
      {\displaystyle \lambda _{\max }(A)}] and      &#x03BB;  min   ( A )
      {\displaystyle \lambda _{\min }(A)}  [\lambda_{\min}(A) ] are maximal and
      minimal (by moduli) eigenvalues of     A   {\displaystyle A}  [A]
      respectively.
    * If     A   {\displaystyle A}  [A] is unitary then     &#x03BA; ( A ) = 1.
      {\displaystyle \kappa (A)=1.}  [{\displaystyle \kappa (A)=1.}]
The condition number with respect to L2 arises so often in numerical linear
algebra that it is given a name, the condition number of a matrix.
If     &#x2016; &#x22C5; &#x2016;   {\displaystyle \|\cdot \|}  [\|\cdot \|] is
the norm defined in the sequence_space ââ of all bounded sequences (which
matches the maximum of distances measured on projections into the base
subspaces and is usually denoted by     &#x2016; &#x22C5;  &#x2016;  &#x221E;
{\displaystyle \|\cdot \|_{\infty }}  [{\displaystyle \|\cdot \|_{\infty }}]),
and     A   {\displaystyle A}  [A] is lower_triangular non-singular (i.e.,
&#x2200; i ,  a  i i   &#x2260; 0   {\displaystyle \forall i,a_{ii}\neq 0}  [
{\displaystyle \forall i,a_{ii}\neq 0}]) then
         &#x03BA; ( A ) &#x2265;     max  i   (  |   a  i i    |  )    min  i
      (  |   a  i i    |  )    .   {\displaystyle \kappa (A)\geq {\frac {\max _
      {i}(|a_{ii}|)}{\min _{i}(|a_{ii}|)}}.}  [ \kappa(A) \geq \frac{\max_i(|a_
      {ii}|)}{\min_i(|a_{ii}|)} .]
The condition number computed with this norm is generally larger than the
condition number computed with square-summable sequences, but it can be
evaluated more easily (and this is often the only practicably computable
condition number, when the problem to solve involves a non-linear algebra
[clarification_needed], for example when approximating irrational and
transcendental functions or numbers with numerical methods).
If the condition number is not too much larger than one, the matrix is well
conditioned which means its inverse can be computed with good accuracy. If the
condition number is very large, then the matrix is said to be ill-conditioned.
Practically, such a matrix is almost singular, and the computation of its
inverse, or solution of a linear system of equations is prone to large
numerical errors. A matrix that is not invertible has condition number equal to
infinity.
***** Nonlinear[edit] *****
Condition numbers can also be defined for nonlinear functions, and can be
computed using calculus. The condition number varies with the point; in some
cases one can use the maximum (or supremum) condition number over the domain of
the function or domain of the question as an overall condition number, while in
other cases the condition number at a particular point is of more interest.
**** One variable[edit] ****
See also: Significance_arithmetic_Â§ Transcendental_functions
The condition number of a differentiable function f in one variable as a
function is      |  x  f &#x2032;   /  f  |  .   {\displaystyle \left|xf'/
f\right|.}  [{\displaystyle \left|xf'/f\right|.}] Evaluated at a point x this
is:
          |    x  f &#x2032;  ( x )   f ( x )    |    {\displaystyle \left|
      {\frac {xf'(x)}{f(x)}}\right|}  [{\displaystyle \left|{\frac {xf'(x)}{f
      (x)}}\right|}]
Most elegantly, this can be understood as (the absolute value of) the ratio of
the logarithmic_derivative of f, which is     ( log &#x2061; f  ) &#x2032;  =
f &#x2032;   /  f   {\displaystyle (\log f)'=f'/f}  [(\log f)' = f'/f] and the
logarithmic derivative of x, which is     ( log &#x2061; x  ) &#x2032;  =  x
&#x2032;   /  x = 1  /  x ,   {\displaystyle (\log x)'=x'/x=1/x,}  [(\log x)' =
x'/x = 1/x,] yielding a ratio of     x  f &#x2032;   /  f .   {\displaystyle
xf'/f.}  [xf'/f.] This is because the logarithmic derivative is the
infinitesimal rate of relative change in a function: it is the derivative
f &#x2032;    {\displaystyle f'}  [f'] scaled by the value of f. Note that if a
function has a zero at a point, its condition number at the point is infinite,
as infinitesimal changes in the input can change the output from zero to
positive or negative, yielding a ratio with zero in the denominator, hence
infinite relative change.
More directly, given a small change     &#x0394; x   {\displaystyle \Delta x}
[\Delta x] in x, the relative change in x is     [ ( x + &#x0394; x ) &#x2212;
x ]  /  x = ( &#x0394; x )  /  x ,   {\displaystyle [(x+\Delta x)-x]/x=(\Delta
x)/x,}  [[(x + \Delta x) - x]/x = (\Delta x)/x,] while the relative change in
f ( x )   {\displaystyle f(x)}  [f(x)] is     [ f ( x + &#x0394; x ) &#x2212; f
( x ) ]  /  f ( x ) .   {\displaystyle [f(x+\Delta x)-f(x)]/f(x).}  [[f(x +
\Delta x) - f(x)]/f(x).] Taking the ratio yields:
            [ f ( x + &#x0394; x ) &#x2212; f ( x ) ]  /  f ( x )   ( &#x0394;
      x )  /  x    =   x  f ( x )       f ( x + &#x0394; x ) &#x2212; f ( x )
      ( x + &#x0394; x ) &#x2212; x    .   {\displaystyle {\frac {[f(x+\Delta
      x)-f(x)]/f(x)}{(\Delta x)/x}}={\frac {x}{f(x)}}{\frac {f(x+\Delta x)-f
      (x)}{(x+\Delta x)-x}}.}  [{\displaystyle {\frac {[f(x+\Delta x)-f(x)]/f
      (x)}{(\Delta x)/x}}={\frac {x}{f(x)}}{\frac {f(x+\Delta x)-f(x)}{
      (x+\Delta x)-x}}.}]
The last term is the difference_quotient (the slope of the secant line), and
taking the limit yields the derivative.
Condition numbers of common elementary_functions are particularly important in
computing significant_figures, and can be computed immediately from the
derivative; see significance_arithmetic_of_transcendental_functions. A few
important ones are given below:
Name                     Symbol                     Condition number
                              e  x                      x   {\displaystyle x}
Exponential function     {\displaystyle e^{x}}  [e^ [x]
                         {x}]
                             ln &#x2061; ( x )            1  ln &#x2061; ( x )
Natural logarithm        {\displaystyle \ln(x)}     {\displaystyle {\frac {1}
function                 [\ln(x)]                   {\ln(x)}}}  [\frac{1}{\ln
                                                    (x)}]
                             sin &#x2061; ( x )         x cot &#x2061; ( x )
Sine function            {\displaystyle \sin(x)}    {\displaystyle x\cot(x)}
                         [\sin(x)]                  [x\cot(x)]
                             cos &#x2061; ( x )         x tan &#x2061; ( x )
Cosine function          {\displaystyle \cos(x)}    {\displaystyle x\tan(x)}
                         [\cos(x)]                  [x\tan(x)]
                                                        x ( tan &#x2061; ( x )
                             tan &#x2061; ( x )     + cot &#x2061; ( x ) )
Tangent function         {\displaystyle \tan(x)}    {\displaystyle x(\tan
                         [\tan(x)]                  (x)+\cot(x))}  [x(\tan
                                                    (x)+\cot(x))]
                                                          x    1 &#x2212;  x
                                                    2     arcsin &#x2061; ( x
                             arcsin &#x2061; ( x )  )      {\displaystyle
Inverse sine function    {\displaystyle \arcsin(x)} {\frac {x}{{\sqrt {1-x^
                         [\arcsin(x)]               {2}}}\arcsin(x)}}}  [\frac
                                                    {x}{\sqrt{1-x^2}\arcsin
                                                    (x)}]
                                                          x    1 &#x2212;  x
                                                    2     arccos &#x2061; ( x
                             arccos &#x2061; ( x )  )      {\displaystyle
Inverse cosine function  {\displaystyle \arccos(x)} {\frac {x}{{\sqrt {1-x^
                         [\arccos(x)]               {2}}}\arccos(x)}}}  [\frac
                                                    {x}{\sqrt{1-x^2}\arccos
                                                    (x)}]
                                                          x  ( 1 +  x  2   )
                             arctan &#x2061; ( x )  arctan &#x2061; ( x )
Inverse tangent function {\displaystyle \arctan(x)} {\displaystyle {\frac {x}{
                         [\arctan(x)]               (1+x^{2})\arctan(x)}}}
                                                    [\frac{x}{(1+x^2)\arctan
                                                    (x)}]
**** Several variables[edit] ****
Condition numbers can be defined for any function f mapping its data from some
domain (e.g. an m-tuple of real numbers x) into some codomain [e.g. an n-tuple
of real numbers f(x)], where both the domain and codomain are Banach_spaces.
They express how sensitive that function is to small changes (or small errors)
in its arguments. This is crucial in assessing the sensitivity and potential
accuracy difficulties of numerous computational problems, for example
polynomial root_finding or computing eigenvalues.
The condition number of f at a point x (specifically, its relative condition
number[4]) is then defined to be the maximum ratio of the fractional change in
f(x) to any fractional change in x, in the limit where the change Î´x in x
becomes infinitesimally small:[4]
          lim  &#x03B5; &#x2192;  0  +      sup  &#x2016; &#x03B4; x &#x2016;
      &#x2264; &#x03B5;    [       &#x2016;  f ( x + &#x03B4; x ) &#x2212; f
      ( x )  &#x2016;   &#x2016; f ( x ) &#x2016;    /     &#x2016; &#x03B4; x
      &#x2016;   &#x2016; x &#x2016;     ]  ,   {\displaystyle \lim _
      {\varepsilon \to 0^{+}}\sup _{\|\delta x\|\leq \varepsilon }\left[\left.
      {\frac {\left\|f(x+\delta x)-f(x)\right\|}{\|f(x)\|}}\right/{\frac
      {\|\delta x\|}{\|x\|}}\right],}  [{\displaystyle \lim _{\varepsilon \to
      0^{+}}\sup _{\|\delta x\|\leq \varepsilon }\left[\left.{\frac {\left\|f
      (x+\delta x)-f(x)\right\|}{\|f(x)\|}}\right/{\frac {\|\delta x\|}
      {\|x\|}}\right],}]
where     &#x2016; &#x22C5; &#x2016;   {\displaystyle \|\cdot \|}  [\|\cdot \|]
is a norm on the domain/codomain of f(x).
If f is differentiable, this is equivalent to:[4]
            &#x2016; J ( x ) &#x2016;   &#x2016; f ( x ) &#x2016;  /  &#x2016;
      x &#x2016;    ,   {\displaystyle {\frac {\|J(x)\|}{\|f(x)\|/\|x\|}},}  [
      {\displaystyle {\frac {\|J(x)\|}{\|f(x)\|/\|x\|}},}]
where     J ( x )   {\displaystyle J(x)}  [J(x)] denotes the Jacobian_matrix of
partial_derivatives of f at x and     &#x2016; J ( x ) &#x2016;
{\displaystyle \|J(x)\|}  [{\displaystyle \|J(x)\|}] is the induced_norm on the
matrix.
***** See also[edit] *****
    * Numerical_methods_for_linear_least_squares
    * Ill-posed_problem
    * Singular_value
***** References[edit] *****
   1. ^Belsley, David A.; Kuh,_Edwin; Welsch, Roy E. (1980). "The_Condition
      Number". Regression Diagnostics: Identifying Influential Data and Sources
      of Collinearity. New York: John Wiley & Sons. pp. 100â104. ISBN 0-471-
      05856-4.
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
   3. ^Pesaran,_M._Hashem (2015). "The_Multicollinearity_Problem". Time Series
      and Panel Data Econometrics. New York: Oxford University Press.
      pp. 67â72 [p. 70]. ISBN 978-0-19-875998-0.
   4. ^Cheney; Kincaid (2007-08-03). Numerical_Mathematics_and_Computing.
      ISBN 978-0-495-11475-8.
   5. ^ a b cTrefethen, L. N.; Bau, D. (1997). Numerical_Linear_Algebra. SIAM.
      ISBN 978-0-89871-361-9.
***** External links[edit] *****
    * Condition_Number_of_a_Matrix at Holistic Numerical Methods Institute
    * "Matrix_condition_number". PlanetMath.
MATLAB_library_function_to_determine_condition_number
Condition_number_â_Encyclopedia_of_Mathematics

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Condition_number&oldid=904598566"
Categories:
    * Numerical_analysis
    * Matrices
Hidden categories:
    * Wikipedia_articles_needing_clarification_from_October_2014
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
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 3 July 2019, at 06:21 (UTC).
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
