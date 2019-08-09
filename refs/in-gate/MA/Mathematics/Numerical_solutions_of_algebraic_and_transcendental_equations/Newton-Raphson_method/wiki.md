The following text has been accessed from https://en.wikipedia.org/wiki/Newton%27s_method at Fri Aug 9 02:32:41 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Newton's method ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about Newton's method for finding roots. For Newton's method
for finding minima, see Newton's_method_in_optimization.
In numerical_analysis, Newton's method, also known as the NewtonâRaphson
method, named after Isaac_Newton and Joseph_Raphson, is a root-finding
algorithm which produces successively better approximations to the roots (or
zeroes) of a real-valued function. The most basic version starts with a single-
variable function f defined for a real_variable x, the function's derivative
f â², and an initial guess x0 for a root of f. If the function satisfies
sufficient assumptions and the initial guess is close, then
          x  1   =  x  0   &#x2212;    f (  x  0   )    f &#x2032;  (  x  0   )
      .   {\displaystyle x_{1}=x_{0}-{\frac {f(x_{0})}{f'(x_{0})}}\,.}  [x_
      {1}=x_{0}-{\frac {f(x_{0})}{f'(x_{0})}}\,.]
is a better approximation of the root than x0. Geometrically, (x1, 0) is the
intersection of the x-axis and the tangent of the graph of f at (x0, f (x0)):
that is, the improved guess is the unique root of the linear_approximation at
the initial point. The process is repeated as
          x  n + 1   =  x  n   &#x2212;    f (  x  n   )    f &#x2032;  (  x  n
      )       {\displaystyle x_{n+1}=x_{n}-{\frac {f(x_{n})}{f'(x_{n})}}\,}
      [x_{n+1}=x_{n}-{\frac {f(x_{n})}{f'(x_{n})}}\,]
until a sufficiently precise value is reached. This algorithm is first in the
class of Householder's_methods, succeeded by Halley's_method. The method can
also be extended to complex_functions and to systems_of_equations.
⁰
***** Contents *****
    * 1_Description
    * 2_History
    * 3_Practical_considerations
          o 3.1_Difficulty_in_calculating_derivative_of_a_function
          o 3.2_Failure_of_the_method_to_converge_to_the_root
                # 3.2.1_Overshoot
                # 3.2.2_Stationary_point
                # 3.2.3_Poor_initial_estimate
                # 3.2.4_Mitigation_of_non-convergence
          o 3.3_Slow_convergence_for_roots_of_multiplicity_greater_than_1
    * 4_Analysis
          o 4.1_Proof_of_quadratic_convergence_for_Newton's_iterative_method
          o 4.2_Basins_of_attraction
    * 5_Failure_analysis
          o 5.1_Bad_starting_points
                # 5.1.1_Iteration_point_is_stationary
                # 5.1.2_Starting_point_enters_a_cycle
          o 5.2_Derivative_issues
                # 5.2.1_Derivative_does_not_exist_at_root
                # 5.2.2_Discontinuous_derivative
          o 5.3_Non-quadratic_convergence
                # 5.3.1_Zero_derivative
                # 5.3.2_No_second_derivative
    * 6_Generalizations
          o 6.1_Complex_functions
                # 6.1.1_Chebyshev's_third_-order_method
                # 6.1.2_NashâMoser_iteration
          o 6.2_Nonlinear_systems_of_equations
                # 6.2.1_k_variables,_k_functions
                # 6.2.2_k_variables,_m_equations,_with_m_>_k
          o 6.3_Nonlinear_equations_in_a_Banach_space
          o 6.4_Nonlinear_equations_over_p-adic_numbers
          o 6.5_NewtonâFourier_method
          o 6.6_Quasi-Newton_methods
          o 6.7_q-analog
          o 6.8_Modified_Newton_methods
                # 6.8.1_Maehly's_procedure
                # 6.8.2_Hirano's_modified_Newton_method
                # 6.8.3_Interval_Newton's_method
    * 7_Applications
          o 7.1_Minimization_and_maximization_problems
          o 7.2_Multiplicative_inverses_of_numbers_and_power_series
          o 7.3_Solving_transcendental_equations
          o 7.4_Obtaining_zeros_of_special_functions
          o 7.5_Numerical_verification_for_solutions_of_nonlinear_equations
    * 8_Examples
          o 8.1_Square_root_of_a_number
          o 8.2_Solution_of_cos_x_=_x3
    * 9_Pseudocode
    * 10_See_also
    * 11_Notes
    * 12_References
    * 13_Further_reading
    * 14_External_links
***** Description[edit] *****
The function f is shown in blue and the tangent line is in red. We see that xn
+ 1 is a better approximation than xn for the root x of the function f.
The idea is to start with an initial guess which is reasonably close to the
true root, then to approximate the function by its tangent_line using calculus,
and finally to compute the x-intercept of this tangent line by elementary
algebra. This x-intercept will typically be a better approximation to the
original function's root than the first guess, and the method can be iterated.
More formally, suppose f : (a, b) â â is a differentiable function defined
on the interval (a, b) with values in the real_numbers â, and we have some
current approximation xn. Then we can derive the formula for a better
approximation, xn + 1 by referring to the diagram on the right. The equation of
the tangent_line to the curve y = f (x) at x = xn is
         y =  f &#x2032;  (  x  n   )  ( x &#x2212;  x  n   ) + f (  x  n   ) ,
      {\displaystyle y=f'(x_{n})\,(x-x_{n})+f(x_{n}),}  [y=f'(x_{n})\,(x-x_
      {n})+f(x_{n}),]
where fâ² denotes the derivative. The x-intercept of this line (the value of x
which makes y = 0) is taken as the next approximation,xn + 1, to the root, so
that the equation of the tangent line is satisfied when     ( x , y ) = (  x  n
+ 1   , 0 )   {\displaystyle (x,y)=(x_{n+1},0)}  [{\displaystyle (x,y)=(x_
{n+1},0)}]:
         0 =  f &#x2032;  (  x  n   )  (  x  n + 1   &#x2212;  x  n   ) + f
      (  x  n   ) .   {\displaystyle 0=f'(x_{n})\,(x_{n+1}-x_{n})+f(x_{n}).}
      [0=f'(x_{n})\,(x_{n+1}-x_{n})+f(x_{n}).]
Solving for xn + 1 gives
          x  n + 1   =  x  n   &#x2212;    f (  x  n   )    f &#x2032;  (  x  n
      )    .   {\displaystyle x_{n+1}=x_{n}-{\frac {f(x_{n})}{f'(x_{n})}}.}  [
      {\displaystyle x_{n+1}=x_{n}-{\frac {f(x_{n})}{f'(x_{n})}}.}]
We start the process with some arbitrary initial value x0. (The closer to the
zero, the better. But, in the absence of any intuition about where the zero
might lie, a "guess and check" method might narrow the possibilities to a
reasonably small interval by appealing to the intermediate_value_theorem.) The
method will usually converge, provided this initial guess is close enough to
the unknown zero, and that f â²(x0) â  0. Furthermore, for a zero of
multiplicity 1, the convergence is at least quadratic (see rate_of_convergence)
in a neighbourhood of the zero, which intuitively means that the number of
correct digits roughly doubles in every step. More details can be found in the
analysis_section below.
Householder's_methods are similar but have higher order for even faster
convergence. However, the extra computations required for each step can slow
down the overall performance relative to Newton's method, particularly if f or
its derivatives are computationally expensive to evaluate.
***** History[edit] *****
The name "Newton's method" is derived from Isaac_Newton's description of a
special case of the method in De_analysi_per_aequationes_numero_terminorum
infinitas (written in 1669, published in 1711 by William_Jones) and in De
metodis fluxionum et serierum infinitarum (written in 1671, translated and
published as Method_of_Fluxions in 1736 by John_Colson). However, his method
differs substantially from the modern method given above: Newton applies the
method only to polynomials. He does not compute the successive approximations
xn, but computes a sequence of polynomials, and only at the end arrives at an
approximation for the root x. Finally, Newton views the method as purely
algebraic and makes no mention of the connection with calculus. Newton may have
derived his method from a similar but less precise method by Vieta. The essence
of Vieta's method can be found in the work of the Persian_mathematician Sharaf
al-Din_al-Tusi, while his successor JamshÄ«d_al-KÄshÄ« used a form of Newton's
method to solve xP â N = 0 to find roots of N (Ypma 1995). A special case of
Newton's method for calculating square roots was known since ancient times and
is often called the Babylonian_method.
Newton's method was used by 17th-century Japanese mathematician Seki_KÅwa to
solve single-variable equations, though the connection with calculus was
missing.[1][citation_needed]
Newton's method was first published in 1685 in A Treatise of Algebra both
Historical and Practical by John_Wallis.[2] In 1690, Joseph_Raphson published a
simplified description in Analysis aequationum universalis.[3] Raphson again
viewed Newton's method purely as an algebraic method and restricted its use to
polynomials, but he describes the method in terms of the successive
approximations xn instead of the more complicated sequence of polynomials used
by Newton. Finally, in 1740, Thomas_Simpson described Newton's method as an
iterative method for solving general nonlinear equations using calculus,
essentially giving the description above. In the same publication, Simpson also
gives the generalization to systems of two equations and notes that Newton's
method can be used for solving optimization problems by setting the gradient to
zero.
Arthur_Cayley in 1879 in The NewtonâFourier imaginary problem was the first
to notice the difficulties in generalizing Newton's method to complex roots of
polynomials with degree greater than 2 and complex initial values. This opened
the way to the study of the theory_of_iterations of rational functions.
***** Practical considerations[edit] *****
Newton's method is an extremely powerful techniqueâin general the convergence
is quadratic: as the method converges on the root, the difference between the
root and the approximation is squared (the number of accurate digits roughly
doubles) at each step. However, there are some difficulties with the method.
**** Difficulty in calculating derivative of a function[edit] ****
Newton's method requires that the derivative can be calculated directly. An
analytical expression for the derivative may not be easily obtainable or could
be expensive to evaluate. In these situations, it may be appropriate to
approximate the derivative by using the slope of a line through two nearby
points on the function. Using this approximation would result in something like
the secant_method whose convergence is slower than that of Newton's method.
**** Failure of the method to converge to the root[edit] ****
It is important to review the proof_of_quadratic_convergence of Newton's Method
before implementing it. Specifically, one should review the assumptions made in
the proof. For situations_where_the_method_fails_to_converge, it is because the
assumptions made in this proof are not met.
*** Overshoot[edit] ***
If the first derivative is not well behaved in the neighborhood of a particular
root, the method may overshoot, and diverge from that root. An example of a
function with one root, for which the derivative is not well behaved in the
neighborhood of the root, is
         f ( x ) =  |  x   |   a   ,  0 < a <    1 2      {\displaystyle f
      (x)=|x|^{a},\quad 0<a<{\tfrac {1}{2}}}  [f(x)=|x|^{a},\quad 0<a<{\tfrac
      {1}{2}}]
for which the root will be overshot and the sequence of x will diverge. For a =
1/2, the root will still be overshot, but the sequence will oscillate between
two values. For 1/2 < a < 1, the root will still be overshot but the sequence
will converge, and for a â¥ 1 the root will not be overshot at all.
In some cases, Newton's method can be stabilized by using successive_over-
relaxation, or the speed of convergence can be increased by using the same
method.
*** Stationary point[edit] ***
If a stationary_point of the function is encountered, the derivative is zero
and the method will terminate due to division_by_zero.
*** Poor initial estimate[edit] ***
A large error in the initial estimate can contribute to non-convergence of the
algorithm. To overcome this problem one can often linearise the function that
is being optimized using calculus, logs, differentials, or even using
evolutionary algorithms, such as the stochastic_funnel_algorithm. Good initial
estimates lie close to the final globally optimal parameter estimate. In
nonlinear regression, the sum of squared errors (SSE) is only "close to"
parabolic in the region of the final parameter estimates. Initial estimates
found here will allow the NewtonâRaphson method to quickly converge. It is
only here that the Hessian_matrix of the SSE is positive and the first
derivative of the SSE is close to zero.
*** Mitigation of non-convergence[edit] ***
In a robust implementation of Newton's method, it is common to place limits on
the number of iterations, bound the solution to an interval known to contain
the root, and combine the method with a more robust root finding method.
**** Slow convergence for roots of multiplicity greater than 1[edit] ****
If the root being sought has multiplicity greater than one, the convergence
rate is merely linear (errors reduced by a constant factor at each step) unless
special steps are taken. When there are two or more roots that are close
together then it may take many iterations before the iterates get close enough
to one of them for the quadratic convergence to be apparent. However, if the
multiplicity     m   {\displaystyle m}  [m] of the root is known, the following
modified algorithm preserves the quadratic convergence rate:[4]
          x  n + 1   =  x  n   &#x2212; m    f (  x  n   )    f &#x2032;  (  x
      n   )    .   {\displaystyle x_{n+1}=x_{n}-m{\frac {f(x_{n})}{f'(x_
      {n})}}.}  [{\displaystyle x_{n+1}=x_{n}-m{\frac {f(x_{n})}{f'(x_{n})}}.}]
This is equivalent to using successive_over-relaxation. On the other hand, if
the multiplicity m of the root is not known, it is possible to estimate     m
{\displaystyle m}  [m] after carrying out one or two iterations, and then use
that value to increase the rate of convergence.
***** Analysis[edit] *****
Suppose that the function f has a zero at Î±, i.e., f (Î±) = 0, and f is
differentiable in a neighborhood of Î±.
If f is continuously differentiable and its derivative is nonzero at Î±, then
there exists a neighborhood of Î± such that for all starting values x0 in that
neighborhood, the sequence {xn} will converge to Î±.[5]
If the function is continuously differentiable and its derivative is not 0 at
Î± and it has a second_derivative at Î± then the convergence is quadratic or
faster. If the second derivative is not 0 at Î± then the convergence is merely
quadratic. If the third derivative exists and is bounded in a neighborhood of
Î±, then:
         &#x0394;  x  i + 1   =     f &#x2033;  ( &#x03B1; )   2  f &#x2032;
      ( &#x03B1; )    ( &#x0394;  x  i    )  2   + O ( &#x0394;  x  i    )  3
      ,   {\displaystyle \Delta x_{i+1}={\frac {f''(\alpha )}{2f'(\alpha )}}
      (\Delta x_{i})^{2}+O(\Delta x_{i})^{3}\,,}  [{\displaystyle \Delta x_
      {i+1}={\frac {f''(\alpha )}{2f'(\alpha )}}(\Delta x_{i})^{2}+O(\Delta x_
      {i})^{3}\,,}]
where
         &#x0394;  x  i   &#x225C;  x  i   &#x2212; &#x03B1;  .
      {\displaystyle \Delta x_{i}\triangleq x_{i}-\alpha \,.}  [\Delta x_
      {i}\triangleq x_{i}-\alpha \,.]
If the derivative is 0 at Î±, then the convergence is usually only linear.
Specifically, if f is twice continuously differentiable, f â²(Î±) = 0 and
f â³(Î±) â  0, then there exists a neighborhood of Î± such that for all
starting values x0 in that neighborhood, the sequence of iterates converges
linearly, with rate 1/2[6] Alternatively if f â²(Î±) = 0 and f â²(x) â  0
for x â  Î±, x in a neighborhood U of Î±, Î± being a zero of multiplicity r,
and if f â Cr(U) then there exists a neighborhood of Î± such that for all
starting values x0 in that neighborhood, the sequence of iterates converges
linearly.
However, even linear convergence is not guaranteed in pathological situations.
In practice these results are local, and the neighborhood of convergence is not
known in advance. But there are also some results on global convergence: for
instance, given a right neighborhood U+ of Î±, if f is twice differentiable in
U+ and if f â² â  0, f Â· f â³ > 0 in U+, then, for each x0 in U+ the
sequence xk is monotonically decreasing to Î±.
**** Proof of quadratic convergence for Newton's iterative method[edit] ****
According to Taylor's_theorem, any function f (x) which has a continuous second
derivative can be represented by an expansion about a point that is close to a
root of f (x). Suppose this root is Î±. Then the expansion of f (Î±) about xn
is:
         f ( &#x03B1; ) = f (  x  n   ) +  f &#x2032;  (  x  n   )
      ( &#x03B1; &#x2212;  x  n   ) +  R  1      {\displaystyle f       
      (\alpha )=f(x_{n})+f'(x_{n})(\alpha -x_{n})+R_{1}\,}  [             (1)
      {\displaystyle f(\alpha )=f(x_{n})+f'(x_{n})(\alpha -x_{n})+R_
      {1}\,}]
where the Lagrange_form_of_the_Taylor_series_expansion_remainder is
          R  1   =   1  2 !     f &#x2033;  (  &#x03BE;  n   ) ( &#x03B1;
      &#x2212;  x  n    )  2    ,   {\displaystyle R_{1}={\frac {1}{2!}}f''(\xi
      _{n})(\alpha -x_{n})^{2}\,,}  [{\displaystyle R_{1}={\frac {1}{2!}}f''
      (\xi _{n})(\alpha -x_{n})^{2}\,,}]
where Î¾n is in between xn and Î±.
Since Î± is the root, (1) becomes:
         0 = f ( &#x03B1; ) = f (  x  n   ) +  f &#x2032;  (  x  n
      ) ( &#x03B1; &#x2212;  x  n   ) +    1 2     f &#x2033;
      (  &#x03BE;  n   ) ( &#x03B1; &#x2212;  x  n    )  2              
      {\displaystyle 0=f(\alpha )=f(x_{n})+f'(x_{n})(\alpha -x_{n})+      (2)
      {\tfrac {1}{2}}f''(\xi _{n})(\alpha -x_{n})^{2}\,}  [
      {\displaystyle 0=f(\alpha )=f(x_{n})+f'(x_{n})(\alpha -x_{n})+
      {\tfrac {1}{2}}f''(\xi _{n})(\alpha -x_{n})^{2}\,}]
Dividing equation (2) by f â²(xn) and rearranging gives
            f (  x  n   )    f &#x2032;  (  x  n   )    +
      (  &#x03B1; &#x2212;  x  n    )  =    &#x2212;  f &#x2033;
      (  &#x03BE;  n   )   2  f &#x2032;  (  x  n   )
      (  &#x03B1; &#x2212;  x  n    )   2     {\displaystyle {\frac      
      {f(x_{n})}{f'(x_{n})}}+\left(\alpha -x_{n}\right)={\frac {-f''       (3)
      (\xi _{n})}{2f'(x_{n})}}\left(\alpha -x_{n}\right)^{2}}  [
      {\displaystyle {\frac {f(x_{n})}{f'(x_{n})}}+\left(\alpha -x_
      {n}\right)={\frac {-f''(\xi _{n})}{2f'(x_{n})}}\left(\alpha -x_
      {n}\right)^{2}}]
Remembering that xn + 1 is defined by
          x  n + 1   =  x  n   &#x2212;    f (  x  n   )    f
      &#x2032;  (  x  n   )     ,   {\displaystyle x_{n+1}=x_{n}-      (4)
      {\frac {f(x_{n})}{f'(x_{n})}}\,,}  [{\displaystyle x_{n+1}=x_    
      {n}-{\frac {f(x_{n})}{f'(x_{n})}}\,,}]
one finds that
             &#x03B1; &#x2212;  x  n + 1    &#x23DF;     &#x03B5;  n + 1     =
      &#x2212;  f &#x2033;  (  &#x03BE;  n   )   2  f &#x2032;  (  x  n   )
      (      &#x03B1; &#x2212;  x  n    &#x23DF;     &#x03B5;  n       )  2
      .   {\displaystyle \underbrace {\alpha -x_{n+1}} _{\varepsilon _{n+1}}=
      {\frac {-f''(\xi _{n})}{2f'(x_{n})}}(\,\underbrace {\alpha -x_{n}} _
      {\varepsilon _{n}}\,)^{2}\,.}  [{\displaystyle \underbrace {\alpha -x_
      {n+1}} _{\varepsilon _{n+1}}={\frac {-f''(\xi _{n})}{2f'(x_{n})}}
      (\,\underbrace {\alpha -x_{n}} _{\varepsilon _{n}}\,)^{2}\,.}]
That is,
          &#x03B5;  n + 1   =    &#x2212;  f &#x2033;  (  &#x03BE;  n
      )   2  f &#x2032;  (  x  n   )    &#x22C5;    &#x03B5;  n     2
      .   {\displaystyle \varepsilon _{n+1}={\frac {-f''(\xi _{n})}      (5)
      {2f'(x_{n})}}\cdot {\varepsilon _{n}}^{2}\,.}  [{\displaystyle     
      \varepsilon _{n+1}={\frac {-f''(\xi _{n})}{2f'(x_{n})}}\cdot
      {\varepsilon _{n}}^{2}\,.}]
Taking absolute value of both sides gives
          |   &#x03B5;  n + 1    |  =    |   f &#x2033;  (  &#x03BE;
      n   )  |   2  |   f &#x2032;  (  x  n   )  |     &#x22C5;
      &#x03B5;  n     2    .   {\displaystyle \left|{\varepsilon _
      {n+1}}\right|={\frac {\left|f''(\xi _{n})\right|}{2\left|f'(x_     (6)
      {n})\right|}}\cdot {\varepsilon _{n}}^{2}\,.}  [{\displaystyle     
      \left|{\varepsilon _{n+1}}\right|={\frac {\left|f''(\xi _
      {n})\right|}{2\left|f'(x_{n})\right|}}\cdot {\varepsilon _{n}}^
      {2}\,.}]
Equation (6) shows that the rate_of_convergence is quadratic if the following
conditions are satisfied:
   1. f â²(x) â  0; for all x â I, where I is the interval [Î± â r, Î± +
      r] for some r â¥ |Î± â x0|;
   2. f â³(x) is continuous, for all x â I;
   3. x0 sufficiently close to the root Î±.
The term sufficiently close in this context means the following:
   1. Taylor approximation is accurate enough such that we can ignore higher
      order terms;
   2.      1 2    |     f &#x2033;  (  x  n   )    f &#x2032;  (  x  n   )    |
      < C  |     f &#x2033;  ( &#x03B1; )    f &#x2032;  ( &#x03B1; )    |  ,
      {\displaystyle {\frac {1}{2}}\left|{\frac {f''(x_{n})}{f'(x_
      {n})}}\right|<C\left|{\frac {f''(\alpha )}{f'(\alpha )}}\right|,}  [
      {\displaystyle {\frac {1}{2}}\left|{\frac {f''(x_{n})}{f'(x_
      {n})}}\right|<C\left|{\frac {f''(\alpha )}{f'(\alpha )}}\right|,}] for
      some C < â;
   3.    C  |     f &#x2033;  ( &#x03B1; )    f &#x2032;  ( &#x03B1; )    |
      &#x03B5;  n   < 1 ,   {\displaystyle C\left|{\frac {f''(\alpha )}{f'
      (\alpha )}}\right|\varepsilon _{n}<1,}  [{\displaystyle C\left|{\frac
      {f''(\alpha )}{f'(\alpha )}}\right|\varepsilon _{n}<1,}] for n â â¤, n
      â¥ 0 and C satisfying condition b.
Finally, (6) can be expressed in the following way:
          |   &#x03B5;  n + 1    |  &#x2264; M    &#x03B5;  n     2
      {\displaystyle \left|{\varepsilon _{n+1}}\right|\leq M{\varepsilon _{n}}^
      {2}\,}  [{\displaystyle \left|{\varepsilon _{n+1}}\right|\leq M
      {\varepsilon _{n}}^{2}\,}]
where M is the supremum of the variable coefficient of Îµn2 on the interval I
defined in condition 1, that is:
         M =  sup  x &#x2208; I     1 2    |     f &#x2033;  ( x )    f
      &#x2032;  ( x )    |  .    {\displaystyle M=\sup _{x\in I}{\frac {1}
      {2}}\left|{\frac {f''(x)}{f'(x)}}\right|.\,}  [{\displaystyle M=\sup _
      {x\in I}{\frac {1}{2}}\left|{\frac {f''(x)}{f'(x)}}\right|.\,}]
The initial point x0 has to be chosen such that conditions 1 to 3 are
satisfied, where the third condition requires that M |Îµ0| < 1.
**** Basins of attraction[edit] ****
The disjoint subsets of the basins_of_attractionâthe regions of the real
number line such that within each region iteration from any point leads to one
particular rootâcan be infinite in number and arbitrarily small. For example,
[7] for the function f (x) = x3 â 2x2 â 11x + 12 = (x â 4)(x â 1)(x +
3), the following initial conditions are in successive basins of attraction:
      2.35287527  converges to    4;
      2.35284172  converges to â3;
      2.35283735  converges to    4;
      2.352836327 converges to â3;
      2.352836323 converges to    1.
***** Failure analysis[edit] *****
Newton's method is only guaranteed to converge if certain conditions are
satisfied. If the assumptions made in the proof of quadratic convergence are
met, the method will converge. For the following subsections, failure of the
method to converge indicates that the assumptions made in the proof were not
met.
**** Bad starting points[edit] ****
In some cases the conditions on the function that are necessary for convergence
are satisfied, but the point chosen as the initial point is not in the interval
where the method converges. This can happen, for example, if the function whose
root is sought approaches zero asymptotically as x goes to â or ââ. In
such cases a different method, such as bisection, should be used to obtain a
better estimate for the zero to use as an initial point.
*** Iteration point is stationary[edit] ***
Consider the function:
         f ( x ) = 1 &#x2212;  x  2   .   {\displaystyle f(x)=1-x^{2}.}  [
      {\displaystyle f(x)=1-x^{2}.}]
It has a maximum at x = 0 and solutions of f (x) = 0 at x = Â±1. If we start
iterating from the stationary_point x0 = 0 (where the derivative is zero), x1
will be undefined, since the tangent at (0,1) is parallel to the x-axis:
          x  1   =  x  0   &#x2212;    f (  x  0   )    f &#x2032;  (  x  0   )
      = 0 &#x2212;   1 0   .   {\displaystyle x_{1}=x_{0}-{\frac {f(x_{0})}{f'
      (x_{0})}}=0-{\frac {1}{0}}.}  [x_{1}=x_{0}-{\frac {f(x_{0})}{f'(x_
      {0})}}=0-{\frac {1}{0}}.]
The same issue occurs if, instead of the starting point, any iteration point is
stationary. Even if the derivative is small but not zero, the next iteration
will be a far worse approximation.
*** Starting point enters a cycle[edit] ***
The tangent lines of x3 â 2x + 2 at 0 and 1 intersect the x-axis at 1 and 0
respectively, illustrating why Newton's method oscillates between these values
for some starting points.
For some functions, some starting points may enter an infinite cycle,
preventing convergence. Let
         f ( x ) =  x  3   &#x2212; 2 x + 2    {\displaystyle f(x)=x^{3}-
      2x+2\!}  [f(x)=x^{3}-2x+2\!]
and take 0 as the starting point. The first iteration produces 1 and the second
iteration returns to 0 so the sequence will alternate between the two without
converging to a root. In fact, this 2-cycle is stable: there are neighborhoods
around 0 and around 1 from which all points iterate asymptotically to the 2-
cycle (and hence not to the root of the function). In general, the behavior of
the sequence can be very complex (see Newton_fractal). The real solution of
this equation is â1.76929235â¦.
**** Derivative issues[edit] ****
If the function is not continuously differentiable in a neighborhood of the
root then it is possible that Newton's method will always diverge and fail,
unless the solution is guessed on the first try.
*** Derivative does not exist at root[edit] ***
A simple example of a function where Newton's method diverges is trying to find
the cube root of zero. The cube root is continuous and infinitely
differentiable, except for x = 0, where its derivative is undefined:
         f ( x ) =   x  3    .   {\displaystyle f(x)={\sqrt[{3}]{x}}.}  [f(x)=
      {\sqrt[{3}]{x}}.]
For any iteration point xn, the next iteration point will be:
          x  n + 1   =  x  n   &#x2212;    f (  x  n   )    f &#x2032;  (  x  n
      )    =  x  n   &#x2212;      x  n      1 3       1 3      x  n       1 3
      &#x2212; 1      =  x  n   &#x2212; 3  x  n   = &#x2212; 2  x  n   .
      {\displaystyle x_{n+1}=x_{n}-{\frac {f(x_{n})}{f'(x_{n})}}=x_{n}-{\frac {
      {x_{n}}^{\frac {1}{3}}}{{\frac {1}{3}}{x_{n}}^{{\frac {1}{3}}-1}}}=x_{n}-
      3x_{n}=-2x_{n}.}  [{\displaystyle x_{n+1}=x_{n}-{\frac {f(x_{n})}{f'(x_
      {n})}}=x_{n}-{\frac {{x_{n}}^{\frac {1}{3}}}{{\frac {1}{3}}{x_{n}}^{
      {\frac {1}{3}}-1}}}=x_{n}-3x_{n}=-2x_{n}.}]
The algorithm overshoots the solution and lands on the other side of the y-
axis, farther away than it initially was; applying Newton's method actually
doubles the distances from the solution at each iteration.
In fact, the iterations diverge to infinity for every f (x) = |x|Î±, where 0 <
Î± < 1/2. In the limiting case of Î± = 1/2 (square root), the iterations will
alternate indefinitely between points x0 and âx0, so they do not converge in
this case either.
*** Discontinuous derivative[edit] ***
If the derivative is not continuous at the root, then convergence may fail to
occur in any neighborhood of the root. Consider the function
         f ( x ) =   {    0    if&#xA0;  x = 0 ,     x +  x  2   sin &#x2061;
      2 x      if&#xA0;  x &#x2260; 0.         {\displaystyle f(x)={\begin
      {cases}0&{\text{if }}x=0,\\x+x^{2}\sin {\frac {2}{x}}&{\text{if }}x\neq
      0.\end{cases}}}  [{\displaystyle f(x)={\begin{cases}0&{\text{if
      }}x=0,\\x+x^{2}\sin {\frac {2}{x}}&{\text{if }}x\neq 0.\end{cases}}}]
Its derivative is:
          f &#x2032;  ( x ) =   {    1    if&#xA0;  x = 0 ,     1 + 2 x sin
      &#x2061;   2 x   &#x2212; 2 cos &#x2061;   2 x      if&#xA0;  x &#x2260;
      0.         {\displaystyle f'(x)={\begin{cases}1&{\text{if
      }}x=0,\\1+2x\sin {\frac {2}{x}}-2\cos {\frac {2}{x}}&{\text{if }}x\neq
      0.\end{cases}}}  [{\displaystyle f'(x)={\begin{cases}1&{\text{if
      }}x=0,\\1+2x\sin {\frac {2}{x}}-2\cos {\frac {2}{x}}&{\text{if }}x\neq
      0.\end{cases}}}]
Within any neighborhood of the root, this derivative keeps changing sign as x
approaches 0 from the right (or from the left) while f (x) â¥ x â x2 > 0 for
0 < x < 1.
So f (x)/f â²(x) is unbounded near the root, and Newton's method will diverge
almost everywhere in any neighborhood of it, even though:
    * the function is differentiable (and thus continuous) everywhere;
    * the derivative at the root is nonzero;
    * f is infinitely differentiable except at the root; and
    * the derivative is bounded in a neighborhood of the root (unlike f (x)/
      f â²(x)).
**** Non-quadratic convergence[edit] ****
In some cases the iterates converge but do not converge as quickly as promised.
In these cases simpler methods converge just as quickly as Newton's method.
*** Zero derivative[edit] ***
If the first derivative is zero at the root, then convergence will not be
quadratic. Let
         f ( x ) =  x  2      {\displaystyle f(x)=x^{2}\!}  [f(x)=x^{2}\!]
then f â²(x) = 2x and consequently
         x &#x2212;    f ( x )    f &#x2032;  ( x )    =   x 2   .
      {\displaystyle x-{\frac {f(x)}{f'(x)}}={\frac {x}{2}}.}  [{\displaystyle
      x-{\frac {f(x)}{f'(x)}}={\frac {x}{2}}.}]
So convergence is not quadratic, even though the function is infinitely
differentiable everywhere.
Similar problems occur even when the root is only "nearly" double. For example,
let
         f ( x ) =  x  2   ( x &#x2212; 1000 ) + 1.   {\displaystyle f(x)=x^{2}
      (x-1000)+1.}  [{\displaystyle f(x)=x^{2}(x-1000)+1.}]
Then the first few iterations starting at x0 = 1 are
      x0 = 1
      x1 = 0.500250376â¦
      x2 = 0.251062828â¦
      x3 = 0.127507934â¦
      x4 = 0.067671976â¦
      x5 = 0.041224176â¦
      x6 = 0.032741218â¦
      x7 = 0.031642362â¦
it takes six iterations to reach a point where the convergence appears to be
quadratic.
*** No second derivative[edit] ***
If there is no second derivative at the root, then convergence may fail to be
quadratic. Let
         f ( x ) = x +  x   4 3    .   {\displaystyle f(x)=x+x^{\frac {4}{3}}.}
      [{\displaystyle f(x)=x+x^{\frac {4}{3}}.}]
Then
          f &#x2032;  ( x ) = 1 +    4 3     x   1 3    .   {\displaystyle f'
      (x)=1+{\tfrac {4}{3}}x^{\frac {1}{3}}.}  [{\displaystyle f'(x)=1+{\tfrac
      {4}{3}}x^{\frac {1}{3}}.}]
And
          f &#x2033;  ( x ) =    4 9     x  &#x2212;   2 3       {\displaystyle
      f''(x)={\tfrac {4}{9}}x^{-{\frac {2}{3}}}}  [{\displaystyle f''(x)=
      {\tfrac {4}{9}}x^{-{\frac {2}{3}}}}]
except when x = 0 where it is undefined. Given xn,
          x  n + 1   =  x  n   &#x2212;    f (  x  n   )    f &#x2032;  (  x  n
      )    =      1 3      x  n      4 3      1 +    4 3       x  n      1 3
      {\displaystyle x_{n+1}=x_{n}-{\frac {f(x_{n})}{f'(x_{n})}}={\frac {{\frac
      {1}{3}}{x_{n}}^{\frac {4}{3}}}{1+{\tfrac {4}{3}}{x_{n}}^{\frac {1}{3}}}}}
      [{\displaystyle x_{n+1}=x_{n}-{\frac {f(x_{n})}{f'(x_{n})}}={\frac {
      {\frac {1}{3}}{x_{n}}^{\frac {4}{3}}}{1+{\tfrac {4}{3}}{x_{n}}^{\frac {1}
      {3}}}}}]
which has approximately 4/3 times as many bits of precision as xn has. This is
less than the 2 times as many which would be required for quadratic
convergence. So the convergence of Newton's method (in this case) is not
quadratic, even though: the function is continuously differentiable everywhere;
the derivative is not zero at the root; and f is infinitely differentiable
except at the desired root.
***** Generalizations[edit] *****
**** Complex functions[edit] ****
Basins of attraction for x5 â 1 = 0; darker means more iterations to
converge.
Main article: Newton_fractal
When dealing with complex_functions, Newton's method can be directly applied to
find their zeroes.[8] Each zero has a basin_of_attraction in the complex plane,
the set of all starting values that cause the method to converge to that
particular zero. These sets can be mapped as in the image shown. For many
complex functions, the boundaries of the basins of attraction are fractals.
In some cases there are regions in the complex plane which are not in any of
these basins of attraction, meaning the iterates do not converge. For example,
[9] if one uses a real initial condition to seek a root of x2 + 1, all
subsequent iterates will be real numbers and so the iterations cannot converge
to either root, since both roots are non-real. In this case almost_all real
initial conditions lead to chaotic_behavior, while some initial conditions
iterate either to infinity or to repeating cycles of any finite length.
Curt McMullen has shown that for any possible purely iterative algorithm
similar to Newton's Method, the algorithm will diverge on some open regions of
the complex plane when applied to some polynomial of degree 4 or higher.
However, McMullen gave a generally convergent algorithm for polynomials of
degree 3.[10]
*** Chebyshev's third -order method[edit] ***
[[icon]] This section is empty. You can help by adding_to_it. (February 2019)
*** NashâMoser iteration[edit] ***
[[icon]] This section is empty. You can help by adding_to_it. (February 2019)
**** Nonlinear systems of equations[edit] ****
*** k variables, k functions[edit] ***
One may also use Newton's method to solve systems of k (nonlinear) equations,
which amounts to finding the zeroes of continuously differentiable functions
F : âk â âk. In the formulation given above, one then has to left
multiply with the inverse of the k Ã k Jacobian_matrix JF(xn) instead of
dividing by f â²(xn):
          x  n + 1   =  x  n   &#x2212;  J  F   (  x  n    )  &#x2212; 1   F
      (  x  n   )   {\displaystyle x_{n+1}=x_{n}-J_{F}(x_{n})^{-1}F(x_{n})}  [
      {\displaystyle x_{n+1}=x_{n}-J_{F}(x_{n})^{-1}F(x_{n})}]
Rather than actually computing the inverse of the Jacobian matrix, one can save
time by solving the system_of_linear_equations
          J  F   (  x  n   ) (  x  n + 1   &#x2212;  x  n   ) = &#x2212; F (  x
      n   )   {\displaystyle J_{F}(x_{n})(x_{n+1}-x_{n})=-F(x_{n})}  [
      {\displaystyle J_{F}(x_{n})(x_{n+1}-x_{n})=-F(x_{n})}]
for the unknown xn + 1 â xn.
*** k variables, m equations, with m > k[edit] ***
The k-dimensional variant of Newton's method can be used to solve systems of
greater than k (nonlinear) equations as well if the algorithm uses the
generalized_inverse of the non-square Jacobian matrix J+ = (JTJ)â1JT instead
of the inverse of J. If the nonlinear_system has no solution, the method
attempts to find a solution in the non-linear_least_squares sense. See
GaussâNewton_algorithm for more information.
**** Nonlinear equations in a Banach space[edit] ****
Another generalization is Newton's method to find a root of a functional F
defined in a Banach_space. In this case the formulation is
          X  n + 1   =  X  n   &#x2212;   (    F &#x2032;  (  X  n   )    )
      &#x2212; 1   F (  X  n   ) ,    {\displaystyle X_{n+1}=X_{n}-{\bigl (}F'
      (X_{n}){\bigr )}^{-1}F(X_{n}),\,}  [{\displaystyle X_{n+1}=X_{n}-{\bigl
      (}F'(X_{n}){\bigr )}^{-1}F(X_{n}),\,}]
where Fâ²(Xn) is the FrÃ©chet_derivative computed at Xn. One needs the
FrÃ©chet derivative to be boundedly invertible at each Xn in order for the
method to be applicable. A condition for existence of and convergence to a root
is given by the NewtonâKantorovich_theorem.
**** Nonlinear equations over p-adic numbers[edit] ****
In p-adic analysis, the standard method to show a polynomial equation in one
variable has a p-adic root is Hensel's_lemma, which uses the recursion from
Newton's method on the p-adic numbers. Because of the more stable behavior of
addition and multiplication in the p-adic numbers compared to the real numbers
(specifically, the unit ball in the p-adics is a ring), convergence in Hensel's
lemma can be guaranteed under much simpler hypotheses than in the classical
Newton's method on the real line.
**** NewtonâFourier method[edit] ****
The NewtonâFourier method is Joseph_Fourier's extension of Newton's method to
provide bounds on the absolute error of the root approximation, while still
providing quadratic convergence.
Assume that f (x) is twice continuously differentiable on [a, b] and that f
contains a root in this interval. Assume that f â²(x), f â³(x) â  0 on this
interval (this is the case for instance if f (a) < 0, f (b) > 0, and f â²(x) >
0, and f â³(x) > 0 on this interval). This guarantees that there is a unique
root on this interval, call it Î±. If it is concave down instead of concave up
then replace f (x) by âf (x) since they have the same roots.
Let x0 = b be the right endpoint of the interval and let z0 = a be the left
endpoint of the interval. Given xn, define
          x  n + 1   =  x  n   &#x2212;    f (  x  n   )    f &#x2032;  (  x  n
      )    ,   {\displaystyle x_{n+1}=x_{n}-{\frac {f(x_{n})}{f'(x_{n})}},}  [
      {\displaystyle x_{n+1}=x_{n}-{\frac {f(x_{n})}{f'(x_{n})}},}]
which is just Newton's method as before. Then define
          z  n + 1   =  z  n   &#x2212;    f (  z  n   )    f &#x2032;  (  x  n
      )    ,   {\displaystyle z_{n+1}=z_{n}-{\frac {f(z_{n})}{f'(x_{n})}},}  [
      {\displaystyle z_{n+1}=z_{n}-{\frac {f(z_{n})}{f'(x_{n})}},}]
where the denominator is f â²(xn) and not f â²(zn). The iterations xn will be
strictly decreasing to the root while the iterations zn will be strictly
increasing to the root. Also,
          lim  n &#x2192; &#x221E;       x  n + 1   &#x2212;  z  n + 1     (  x
      n   &#x2212;  z  n    )  2      =     f &#x2033;  ( &#x03B1; )   2  f
      &#x2032;  ( &#x03B1; )      {\displaystyle \lim _{n\to \infty }{\frac {x_
      {n+1}-z_{n+1}}{(x_{n}-z_{n})^{2}}}={\frac {f''(\alpha )}{2f'(\alpha )}}}
      [\lim _{n\to \infty }{\frac {x_{n+1}-z_{n+1}}{(x_{n}-z_{n})^{2}}}={\frac
      {f''(\alpha )}{2f'(\alpha )}}]
so that distance between xn and zn decreases quadratically.
**** Quasi-Newton methods[edit] ****
When the Jacobian is unavailable or too expensive to compute at every
iteration, a quasi-Newton_method can be used.
**** q-analog[edit] ****
Newton's method can be generalized with the q-analog of the usual derivative.
[11]
**** Modified Newton methods[edit] ****
*** Maehly's procedure[edit] ***
A nonlinear equation has multiple solutions in general. But if the initial
value is not appropriate, Newton's method may not converge to the desired
solution or may converge to the same solution found earlier. When we have
already found N solutions of     f ( x ) = 0   {\displaystyle f(x)=0}  [f
(x)=0], then the next root can be found by applying Newton's method to the next
equation:[12][13]
         F ( x ) =    f ( x )    &#x220F;  i = 1   N   ( x &#x2212;  x  i   )
      = 0.   {\displaystyle F(x)={\frac {f(x)}{\prod _{i=1}^{N}(x-x_{i})}}=0.}
      [{\displaystyle F(x)={\frac {f(x)}{\prod _{i=1}^{N}(x-x_{i})}}=0.}]
This method is applied to obtain zeros of the Bessel_function of the second
kind.[14]
*** Hirano's modified Newton method[edit] ***
Hirano's modified Newton method is a modification conserving the convergence of
Newton method and avoiding unstableness.[15] It is developed to solve complex
polynomials.
*** Interval Newton's method[edit] ***
                                 This section possibly contains
                                 inappropriate or misinterpreted citations
[Text_document_with_red_question that do not verify the text. Please help
mark.svg]                        improve_this_article by checking for
                                 citation inaccuracies. (February 2019)
                                 (Learn_how_and_when_to_remove_this
                                 template_message)
Combining Newton's method with interval_arithmetic is very useful in some
contexts. This provides a stopping criterion that is more reliable than the
usual ones (which are a small value of the function or a small variation of the
variable between consecutive iterations). Also, this may detect cases where
Newton's method converges theoretically but diverges numerically because of an
insufficient floating-point_precision (this is typically the case for
polynomials of large degree, where a very small change of the variable may
change dramatically the value of the function; see Wilkinson's_polynomial).[16]
[17]
Consider     f &#x2208;    C    1   ( X )   {\displaystyle f\in {\mathcal {C}}^
{1}(X)}  [{\displaystyle f\in {\mathcal {C}}^{1}(X)}], where     X
{\displaystyle X}  [X] is a real interval, and suppose that we have an interval
extension      F &#x2032;    {\displaystyle F'}  [F'] of      f &#x2032;
{\displaystyle f'}  [f'], meaning that      F &#x2032;    {\displaystyle F'}
[F'] takes as input an interval     Y &#x2286; X   {\displaystyle Y\subseteq X}
[Y \subseteq X] and outputs an interval      F &#x2032;  ( Y )   {\displaystyle
F'(Y)}  [{\displaystyle F'(Y)}] such that:
              F &#x2032;  ( [ y , y ] )    = {  f &#x2032;  ( y ) }      F
      &#x2032;  ( Y )    &#x2287; {  f &#x2032;  ( y ) &#x2223; y &#x2208; Y }
      .       {\displaystyle {\begin{aligned}F'([y,y])&=\{f'(y)\}\\[5pt]F'
      (Y)&\supseteq \{f'(y)\mid y\in Y\}.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}F'([y,y])&=\{f'(y)\}\\[5pt]F'(Y)&\supseteq \{f'(y)\mid
      y\in Y\}.\end{aligned}}}]
We also assume that     0 &#x2209;  F &#x2032;  ( X )   {\displaystyle 0\notin
F'(X)}  [{\displaystyle 0\notin F'(X)}], so in particular     f
{\displaystyle f}  [f] has at most one root in     X   {\displaystyle X}  [X].
We then define the interval Newton operator by:
         N ( Y ) = m &#x2212;    f ( m )    F &#x2032;  ( Y )    =  {     m
      &#x2212;    f ( m )  z   &#xA0;  |  &#xA0; z &#x2208;  F &#x2032;  ( Y )
      }    {\displaystyle N(Y)=m-{\frac {f(m)}{F'(Y)}}=\left\{\left.m-{\frac {f
      (m)}{z}}~\right|~z\in F'(Y)\right\}}  [{\displaystyle N(Y)=m-{\frac {f
      (m)}{F'(Y)}}=\left\{\left.m-{\frac {f(m)}{z}}~\right|~z\in F'
      (Y)\right\}}]
where     m &#x2208; Y   {\displaystyle m\in Y}  [{\displaystyle m\in Y}]. Note
that the hypothesis on      F &#x2032;    {\displaystyle F'}  [F'] implies that
N ( Y )   {\displaystyle N(Y)}  [{\displaystyle N(Y)}] is well defined and is
an interval (see interval_arithmetic for further details on interval
operations). This naturally leads to the following sequence:
              X  0      = X      X  k + 1      = N (  X  k   ) &#x2229;  X  k
      .       {\displaystyle {\begin{aligned}X_{0}&=X\\X_{k+1}&=N(X_{k})\cap X_
      {k}.\end{aligned}}}  [{\displaystyle {\begin{aligned}X_{0}&=X\\X_{k+1}&=N
      (X_{k})\cap X_{k}.\end{aligned}}}]
The mean_value_theorem ensures that if there is a root of     f
{\displaystyle f}  [f] in      X  k     {\displaystyle X_{k}}  [X_{k}], then it
is also in      X  k + 1     {\displaystyle X_{k+1}}  [{\displaystyle X_
{k+1}}]. Moreover, the hypothesis on      F &#x2032;    {\displaystyle F'}
[F'] ensures that      X  k + 1     {\displaystyle X_{k+1}}  [{\displaystyle X_
{k+1}}] is at most half the size of      X  k     {\displaystyle X_{k}}  [X_
{k}] when     m   {\displaystyle m}  [m] is the midpoint of     Y
{\displaystyle Y}  [Y], so this sequence converges towards     [  x  &#x2217;
,  x  &#x2217;   ]   {\displaystyle [x^{*},x^{*}]}  [{\displaystyle [x^{*},x^
{*}]}], where      x  &#x2217;     {\displaystyle x^{*}}  [x^{*}] is the root
of     f   {\displaystyle f}  [f] in     X   {\displaystyle X}  [X].
If      F &#x2032;  ( X )   {\displaystyle F'(X)}  [{\displaystyle F'(X)}]
strictly contains     0   {\displaystyle 0}  [{\displaystyle 0}], the use of
extended interval division produces a union of two intervals for     N ( X )
{\displaystyle N(X)}  [N(X)] ; multiple roots are therefore automatically
separated and bounded.
***** Applications[edit] *****
**** Minimization and maximization problems[edit] ****
Main article: Newton's_method_in_optimization
Newton's method can be used to find a minimum or maximum of a function     f
( x )   {\displaystyle f(x)}  [f(x)]. The derivative is zero at a minimum or
maximum, so local minima and maxima can be found by applying Newton's method to
the derivative. The iteration becomes:
          x  n + 1   =  x  n   &#x2212;     f &#x2032;  (  x  n   )    f
      &#x2033;  (  x  n   )    .   {\displaystyle x_{n+1}=x_{n}-{\frac {f'(x_
      {n})}{f''(x_{n})}}.}  [{\displaystyle x_{n+1}=x_{n}-{\frac {f'(x_{n})}
      {f''(x_{n})}}.}]
**** Multiplicative inverses of numbers and power series[edit] ****
An important application is NewtonâRaphson_division, which can be used to
quickly find the reciprocal of a number, using only multiplication and
subtraction.
Finding the reciprocal of a amounts to finding the root of the function
         f ( x ) = a &#x2212;   1 x     {\displaystyle f(x)=a-{\frac {1}{x}}}
      [f(x)=a-{\frac {1}{x}}]
Newton's iteration is
              x  n + 1      =  x  n   &#x2212;    f (  x  n   )    f &#x2032;
      (  x  n   )          =  x  n   &#x2212;    a &#x2212;   1  x  n       1
      x  n   2            =  x  n   ( 2 &#x2212; a  x  n   )
      {\displaystyle {\begin{aligned}x_{n+1}&=x_{n}-{\frac {f(x_{n})}{f'(x_
      {n})}}\\[5pt]&=x_{n}-{\frac {a-{\frac {1}{x_{n}}}}{\frac {1}{x_{n}^
      {2}}}}\\[5pt]&=x_{n}(2-ax_{n})\end{aligned}}}  [{\displaystyle {\begin
      {aligned}x_{n+1}&=x_{n}-{\frac {f(x_{n})}{f'(x_{n})}}\\[5pt]&=x_{n}-
      {\frac {a-{\frac {1}{x_{n}}}}{\frac {1}{x_{n}^{2}}}}\\[5pt]&=x_{n}(2-ax_
      {n})\end{aligned}}}]
Therefore, Newton's iteration needs only two multiplications and one
subtraction.
This method is also very efficient to compute the multiplicative inverse of a
power_series.
**** Solving transcendental equations[edit] ****
Many transcendental_equations can be solved using Newton's method. Given the
equation
         g ( x ) = h ( x ) ,   {\displaystyle g(x)=h(x),}  [{\displaystyle g
      (x)=h(x),}]
with g(x) and/or h(x) a transcendental_function, one writes
         f ( x ) = g ( x ) &#x2212; h ( x ) .   {\displaystyle f(x)=g(x)-h(x).}
      [{\displaystyle f(x)=g(x)-h(x).}]
The values of x that solve the original equation are then the roots of f (x),
which may be found via Newton's method.
**** Obtaining zeros of special functions[edit] ****
Newton's method is applied to the ratio of Bessel functions in order to obtain
its root.[18]
**** Numerical verification for solutions of nonlinear equations[edit] ****
A numerical verification for solutions of nonlinear equations has been
established by using Newton's method multiple times and forming a set of
solution candidates.[19][20]
***** Examples[edit] *****
**** Square root of a number[edit] ****
Consider the problem of finding the square root of a number S. Newton's method
is one of many methods_of_computing_square_roots.
For example, if one wishes to find the square root of 612, this is equivalent
to finding the solution to
          x  2   = 612   {\displaystyle x^{2}=612}  [{\displaystyle x^{2}=612}]
The function to use in Newton's method is then
         f ( x ) =  x  2   &#x2212; 612   {\displaystyle f(x)=x^{2}-612}  [
      {\displaystyle f(x)=x^{2}-612}]
with derivative
          f &#x2032;  ( x ) = 2 x .    {\displaystyle f'(x)=2x.\,}  [f'
      (x)=2x.\,]
With an initial guess of 10, the sequence given by Newton's method is
              x  1     =    x  0   &#x2212;     f (  x  0   )    f &#x2032;
      (  x  0   )       =   10 &#x2212;      10  2   &#x2212; 612   2 &#x00D7;
      10       =   35.6              x  2     =    x  1   &#x2212;     f (  x
      1   )    f &#x2032;  (  x  1   )       =   35.6 &#x2212;      35.6  2
      &#x2212; 612   2 &#x00D7; 35.6       =     2 &#x005F;   6.395  505  617
      978 &#x2026;      x  3     =   &#x22EE;   =   &#x22EE;   =     24.7
      &#x005F;   90  635  492  455 &#x2026;      x  4     =   &#x22EE;   =
      &#x22EE;   =      24.738  6  &#x005F;   88  294  075 &#x2026;      x  5
      =   &#x22EE;   =   &#x22EE;   =      24.738  633  753  7  &#x005F;   67
      &#x2026;       {\displaystyle {\begin{matrix}x_{1}&=&x_{0}-{\dfrac {f(x_
      {0})}{f'(x_{0})}}&=&10-{\dfrac {10^{2}-612}{2\times 10}}&=&35.6\qquad
      \qquad \qquad \quad \;\,{}\\x_{2}&=&x_{1}-{\dfrac {f(x_{1})}{f'(x_
      {1})}}&=&35.6-{\dfrac {35.6^{2}-612}{2\times 35.6}}&=&{\underline
      {2}}6.395\,505\,617\,978\dots \\x_{3}&=&\vdots &=&\vdots &=&{\underline
      {24.7}}90\,635\,492\,455\dots \\x_{4}&=&\vdots &=&\vdots &=&{\underline
      {24.738\,6}}88\,294\,075\dots \\x_{5}&=&\vdots &=&\vdots &=&{\underline
      {24.738\,633\,753\,7}}67\dots \end{matrix}}}  [{\displaystyle {\begin
      {matrix}x_{1}&=&x_{0}-{\dfrac {f(x_{0})}{f'(x_{0})}}&=&10-{\dfrac {10^
      {2}-612}{2\times 10}}&=&35.6\qquad \qquad \qquad \quad \;\,{}\\x_{2}&=&x_
      {1}-{\dfrac {f(x_{1})}{f'(x_{1})}}&=&35.6-{\dfrac {35.6^{2}-612}{2\times
      35.6}}&=&{\underline {2}}6.395\,505\,617\,978\dots \\x_{3}&=&\vdots
      &=&\vdots &=&{\underline {24.7}}90\,635\,492\,455\dots \\x_{4}&=&\vdots
      &=&\vdots &=&{\underline {24.738\,6}}88\,294\,075\dots \\x_{5}&=&\vdots
      &=&\vdots &=&{\underline {24.738\,633\,753\,7}}67\dots \end{matrix}}}]
where the correct digits are underlined. With only a few iterations one can
obtain a solution accurate to many decimal places.
Rearranging the formula as follows yields the Babylonian_method_of_finding
square_roots:
          x  n + 1   =  x  n   &#x2212;     f (  x  n   )    f &#x2032;  (  x
      n   )     =  x  n   &#x2212;      x  n   2   &#x2212; S   2  x  n       =
      1 2      (   2  x  n   &#x2212;   (    x  n   &#x2212;    S  x  n
      )     )   =    1 2      (    x  n   +    S  x  n        )
      {\displaystyle x_{n+1}=x_{n}-{\dfrac {f(x_{n})}{f'(x_{n})}}=x_{n}-{\dfrac
      {x_{n}^{2}-S}{2x_{n}}}={\dfrac {1}{2}}{\Bigl (}2x_{n}-{\bigl (}x_{n}-
      {\dfrac {S}{x_{n}}}{\bigr )}{\Bigr )}={\dfrac {1}{2}}{\Bigl (}x_{n}+
      {\dfrac {S}{x_{n}}}{\Bigr )}}  [{\displaystyle x_{n+1}=x_{n}-{\dfrac {f
      (x_{n})}{f'(x_{n})}}=x_{n}-{\dfrac {x_{n}^{2}-S}{2x_{n}}}={\dfrac {1}{2}}
      {\Bigl (}2x_{n}-{\bigl (}x_{n}-{\dfrac {S}{x_{n}}}{\bigr )}{\Bigr )}=
      {\dfrac {1}{2}}{\Bigl (}x_{n}+{\dfrac {S}{x_{n}}}{\Bigr )}}]
i.e. the arithmetic_mean of the guess, xn and S/xn .
**** Solution of cos x = x3[edit] ****
Consider the problem of finding the positive number x with cos x = x3. We can
rephrase that as finding the zero of f (x) = cos(x) â x3. We have f â²(x) =
âsin(x) â 3x2. Since cos(x) â¤ 1 for all x and x3 > 1 for x > 1, we know
that our solution lies between 0 and 1. We try a starting value of x0 = 0.5.
(Note that a starting value of 0 will lead to an undefined result, showing the
importance of using a starting point that is close to the solution.)
              x  1     =    x  0   &#x2212;     f (  x  0   )    f &#x2032;
      (  x  0   )       =   0.5 &#x2212;     cos &#x2061; 0.5 &#x2212;  0.5  3
      &#x2212; sin &#x2061; 0.5 &#x2212; 3 &#x00D7;  0.5  2         =   1.112
      141  637  097 &#x2026;      x  2     =    x  1   &#x2212;     f (  x  1
      )    f &#x2032;  (  x  1   )       =   &#x22EE;   =     0. &#x005F;   909
      672  693  736 &#x2026;      x  3     =   &#x22EE;   =   &#x22EE;   =
      0.86 &#x005F;   7  263  818  209 &#x2026;      x  4     =   &#x22EE;   =
      &#x22EE;   =      0.865  47  &#x005F;   7  135  298 &#x2026;      x  5
      =   &#x22EE;   =   &#x22EE;   =      0.865  474  033  1  &#x005F;   11
      &#x2026;      x  6     =   &#x22EE;   =   &#x22EE;   =      0.865  474
      033  102  &#x005F;   &#x2026;       {\displaystyle {\begin{matrix}x_
      {1}&=&x_{0}-{\dfrac {f(x_{0})}{f'(x_{0})}}&=&0.5-{\dfrac {\cos 0.5-0.5^
      {3}}{-\sin 0.5-3\times 0.5^{2}}}&=&1.112\,141\,637\,097\dots \\x_{2}&=&x_
      {1}-{\dfrac {f(x_{1})}{f'(x_{1})}}&=&\vdots &=&{\underline
      {0.}}909\,672\,693\,736\dots \\x_{3}&=&\vdots &=&\vdots &=&{\underline
      {0.86}}7\,263\,818\,209\dots \\x_{4}&=&\vdots &=&\vdots &=&{\underline
      {0.865\,47}}7\,135\,298\dots \\x_{5}&=&\vdots &=&\vdots &=&{\underline
      {0.865\,474\,033\,1}}11\dots \\x_{6}&=&\vdots &=&\vdots &=&{\underline
      {0.865\,474\,033\,102}}\dots \end{matrix}}}  [{\displaystyle {\begin
      {matrix}x_{1}&=&x_{0}-{\dfrac {f(x_{0})}{f'(x_{0})}}&=&0.5-{\dfrac {\cos
      0.5-0.5^{3}}{-\sin 0.5-3\times 0.5^{2}}}&=&1.112\,141\,637\,097\dots \\x_
      {2}&=&x_{1}-{\dfrac {f(x_{1})}{f'(x_{1})}}&=&\vdots &=&{\underline
      {0.}}909\,672\,693\,736\dots \\x_{3}&=&\vdots &=&\vdots &=&{\underline
      {0.86}}7\,263\,818\,209\dots \\x_{4}&=&\vdots &=&\vdots &=&{\underline
      {0.865\,47}}7\,135\,298\dots \\x_{5}&=&\vdots &=&\vdots &=&{\underline
      {0.865\,474\,033\,1}}11\dots \\x_{6}&=&\vdots &=&\vdots &=&{\underline
      {0.865\,474\,033\,102}}\dots \end{matrix}}}]
The correct digits are underlined in the above example. In particular, x6 is
correct to 12 decimal places. We see that the number of correct digits after
the decimal point increases from 2 (for x3) to 5 and 10, illustrating the
quadratic convergence.
***** Pseudocode[edit] *****
The following is an example of an implementation of the Newton's Method for
finding a root of a function f which has derivative fprime.
The initial guess will be x0 = 1 and the function will be f (x) = x2 â 2 so
that f â²(x) = 2x.
Each new iteration of Newton's method will be denoted by x1. We will check
during the computation whether the denominator (yprime) becomes too small
(smaller than epsilon), which would be the case if f â²(xn) â 0, since
otherwise a large amount of error could be introduced.
%These choices depend on the problem being solved
x0 = 1 %The initial value
f = @(x) x^2 - 2 %The function whose root we are trying to find
fprime = @(x) 2*x %The derivative of f(x)
tolerance = 10^(-7) %7 digit accuracy is desired
epsilon = 10^(-14) %Don't want to divide by a number smaller than this

maxIterations = 20 %Don't allow the iterations to continue indefinitely
haveWeFoundSolution = false %Have not converged to a solution yet

for i = 1 : maxIterations

 y = f(x0)
 yprime = fprime(x0)

 if(abs(yprime) < epsilon) %Don't want to divide by too small of a number
 % denominator is too small
 break; %Leave the loop
 end

 x1 = x0 - y/yprime %Do Newton's computation

 if(abs(x1 - x0) <= tolerance * abs(x1)) %If the result is within the desired
tolerance
 haveWeFoundSolution = true
 break; %Done, so leave the loop
 end

 x0 = x1 %Update x0 to start the process again

end

if (haveWeFoundSolution)
 ... % x1 is a solution within tolerance and maximum number of iterations
else
 ... % did not converge
end
***** See also[edit] *****
    * Aitken's_delta-squared_process
    * Bisection_method
    * Euler_method
    * Fast_inverse_square_root
    * Fisher_scoring
    * Gradient_descent
    * Integer_square_root
    * Kantorovich_theorem
    * Laguerre's_method
    * Methods_of_computing_square_roots
    * Newton's_method_in_optimization
    * Richardson_extrapolation
    * Root-finding_algorithm
    * Secant_method
    * Steffensen's_method
    * Subgradient_method
***** Notes[edit] *****
   1. ^"Chapter_2._Seki_Takakazu". Japanese Mathematics in the Edo Period.
      National Diet Library. Retrieved 24 February 2019.
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
   3. ^Wallis,_John (1685). A_Treatise_of_Algebra,_both_Historical_and
      Practical._Shewing_the_Original,_Progress,_and_Advancement_thereof,_from
      time_to_time,_and_by_what_Steps_it_hath_attained_to_the_Heighth_at_which
      it_now_is. Oxford: Richard Davis. doi:10.3931/e-rara-8842.
   4. ^Raphson,_Joseph (1697). Analysis_Ãequationum_Universalis_seu_ad
      Ãequationes_Algebraicas_Resolvendas_Methodus_Generalis,_&_Expedita,_Ex
      nova_Infinitarum_Serierum_Methodo,_Deducta_ac_Demonstrata (in Latin)
      (secunda ed.). London. doi:10.3931/e-rara-13516.
   5. ^"Accelerated_and_Modified_Newton_Methods".
   6. ^Ryaben'kii, Victor S.; Tsynkov, Semyon V. (2006), A_Theoretical
      Introduction_to_Numerical_Analysis, CRC Press, p. 243, ISBN 9781584886075
   7. .
   8. ^ SÃ¼li_&_Mayers_2003, Exercise 1.6
   9. ^Dence, Thomas (November 1997). "Cubics, chaos and Newton's method".
      Mathematical_Gazette. 81: 403â408. doi:10.2307/3619617.
  10. ^Henrici, Peter (1974). "Applied and Computational Complex Analysis". 1.
  11. ^Strang, Gilbert (January 1991). "A chaotic search for i". The_College
      Mathematics_Journal. 22: 3â12. doi:10.2307/2686733.
  12. ^McMullen, Curt (1987). "Families_of_rational_maps_and_iterative_root-
      finding_algorithms" (PDF). Annals of Mathematics. Second Series. 125 (3):
      467â493. doi:10.2307/1971408.
  13. ^ Rajkovic,_Stankovic_&_Marinkovic_2002[incomplete_short_citation]
  14. ^ Press_et_al._1992[incomplete_short_citation]
  15. ^ Stoer_&_Bulirsch_1980[incomplete_short_citation]
  16. ^ Zhang_&_Jin_1996[incomplete_short_citation]
  17. ^Murota, Kazuo (1982). "Global Convergence of a Modified Newton Iteration
      for Algebraic Equations". SIAM J. Numer. Anal. 19 (4): 793â799. doi:
      10.1137/0719055.
  18. ^ Moore, R. E. (1979). Methods and applications of interval analysis
      (Vol. 2). Siam.
  19. ^ Hansen, E. (1978). Interval forms of Newtons method. Computing, 20(2),
      153-163.
  20. ^ Gil,_Segura_&_Temme_(2007)[incomplete_short_citation]
  21. ^ Kahan (1968)[incomplete_short_citation]
  22. ^ Krawczyk_(1969)[incomplete_short_citation][incomplete_short_citation]
***** References[edit] *****
    * Gil, A.; Segura, J.; Temme, N. M. (2007). Numerical_methods_for_special
      functions (PDF). Society for Industrial and Applied Mathematics.
      ISBN 978-0-89871-634-4.
SÃ¼li,_Endre; Mayers, David (2003). An Introduction to Numerical Analysis.
Cambridge University Press. ISBN 0-521-00794-1.
***** Further reading[edit] *****
    * Kendall E. Atkinson, An Introduction to Numerical Analysis, (1989) John
      Wiley & Sons, Inc,
ISBN 0-471-62489-6
Tjalling J. Ypma, Historical development of the NewtonâRaphson method, SIAM
Review 37 (4), 531â551, 1995. doi:10.1137/1037125.
Bonnans, J. FrÃ©dÃ©ric; Gilbert, J. Charles; LemarÃ©chal,_Claude;
SagastizÃ¡bal,_Claudia A. (2006). Numerical_optimization:_Theoretical_and
practical_aspects. Universitext (Second revised ed. of translation of 1997
French ed.). Berlin: Springer-Verlag. pp. xiv+490. doi:10.1007/978-3-540-35447-
5. ISBN 3-540-35445-X. MR 2265882.
P. Deuflhard, Newton Methods for Nonlinear Problems. Affine Invariance and
Adaptive Algorithms. Springer Series in Computational Mathematics, Vol. 35.
Springer, Berlin, 2004.
ISBN 3-540-21099-7.
C. T. Kelley, Solving Nonlinear Equations with Newton's Method, no 1 in
Fundamentals of Algorithms, SIAM, 2003.
ISBN 0-89871-546-6.
J. M. Ortega, W. C. Rheinboldt, Iterative Solution of Nonlinear Equations in
Several Variables. Classics in Applied Mathematics, SIAM, 2000.
ISBN 0-89871-461-3.
Press, W. H.; Teukolsky, S. A.; Vetterling, W. T.; Flannery, B. P. (2007).
"Chapter_9._Root_Finding_and_Nonlinear_Sets_of_Equations_Importance_Sampling".
Numerical Recipes: The Art of Scientific Computing (3rd ed.). New York:
Cambridge University Press. ISBN 978-0-521-88068-8.
. See especially Sections 9.4, 9.6, and 9.7.
Kaw, Autar; Kalu, Egwu (2008). "Numerical Methods with Applications" (1st ed.)
.
***** External links[edit] *****
 Wikimedia Commons has media related to Newton_Method.
 For a list of words relating to Newton's method, see the Newton's_method
 category_of_article in Wikibooks.
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Newton_method", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Weisstein,_Eric_W. "Newton's_Method". MathWorld.
Newton's_method,_Citizendium.
Mathews,_J.,_The_Accelerated_and_Modified_Newton_Methods,_Course_notes.
Wu,_X.,_Roots_of_Equations,_Course_notes.
    * v
    * t
    * e
Sir_Isaac_Newton
                   * Fluxions (1671)
                   * De_Motu (1684)
                   * Principia (1687; writing)
Publications       * Opticks (1704)
                   * Queries (1704)
                   * Arithmetica (1707)
                   * De_Analysi (1711)
                   * Quaestiones (1661â65)
                   * "standing_on_the_shoulders_of_giants" (1675)
Other writings     * Notes_on_the_Jewish_Temple (c. 1680)
                   * "General_Scholium" (1713; "hypotheses_non_fingo" )
                   * Ancient_Kingdoms_Amended (1728)
                   * Corruptions_of_Scripture (1754)
                   * Calculus
                         o fluxion
                   * Impact_depth
                   * Inertia
                   * Newton_disc
                   * Newton_polygon
Contributions            o NewtonâOkounkov_body
                   * Newton's_reflector
                   * Newtonian_telescope
                   * Newton_scale
                   * Newton's_metal
                   * Newton's_cradle
                   * Spectrum
                   * Structural_coloration
                   * Bucket_argument
                   * Newton's_inequalities
                   * Newton's_law_of_cooling
                   * Newton's_law_of_universal_gravitation
                         o post-Newtonian_expansion
                         o parameterized
                         o gravitational_constant
                   * NewtonâCartan_theory
                   * SchrÃ¶dingerâNewton_equation
                   * Newton's_laws_of_motion
                         o Kepler's_laws
                   * Newtonian_dynamics
                   * Newton's_method_in_optimization
                         o Apollonius's_problem
                         o truncated_Newton_method
                   * GaussâNewton_algorithm
                   * Newton's_rings
                   * Newton's_theorem_about_ovals
                   * NewtonâPepys_problem
                   * Newtonian_potential
                   * Newtonian_fluid
Newtonianism       * Classical_mechanics
                   * Newtonian_fluid
                   * Corpuscular_theory_of_light
                   * LeibnizâNewton_calculus_controversy
                   * Newton's_notation
                   * Rotating_spheres
                   * Newton's_cannonball
                   * NewtonâCotes_formulas
                   * Newton's method
                         o generalized_GaussâNewton_method
                   * Newton_fractal
                   * Newton's_identities
                   * Newton_polynomial
                   * Newton's_theorem_of_revolving_orbits
                   * NewtonâEuler_equations
                   * Newton_number
                         o kissing_number_problem
                   * Newton's_quotient
                   * Parallelogram_of_force
                   * NewtonâPuiseux_theorem
                   * Absolute_space_and_time
                   * Newtonian_series
                         o table
                   * Woolsthorpe_Manor (birthplace)
                   * Cranbury_Park (home)
                   * Early_life
Personal life      * Later_life
                   * Religious_views
                   * Occult_studies
                   * Scientific_revolution
                   * Copernican_revolution
                   * Catherine_Barton (niece)
                   * John_Conduitt (nephew-in-law)
                   * Isaac_Barrow (professor)
                   * William_Clarke (mentor)
Relations          * Benjamin_Pulleyn (tutor)
                   * John_Keill (disciple)
                   * William_Stukeley (friend)
                   * William_Jones (friend)
                   * Abraham_de_Moivre (friend)
Depictions         * Newton_by_Blake (monotype)
                   * Newton_by_Paolozzi (sculpture)
                   * Isaac_Newton_Institute
                   * Isaac_Newton_Medal
Namesake           * Isaac_Newton_Telescope
                   * Isaac_Newton_Group_of_Telescopes
                   * Newton_(unit)
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
Root-finding_algorithms
Bracketing_(no_derivative)     * Bisection_method
Quasi-Newton                   * Regula_falsi
                               * Secant_method
Newton                         * Newton's method
Hybrid_methods                 * Brent's_method
                               * Bairstow's_method
Polynomial methods             * JenkinsâTraub_method
                               * Laguerre's_method

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Newton%27s_method&oldid=903360911"
Categories:
    * Optimization_algorithms_and_methods
    * Root-finding_algorithms
Hidden categories:
    * CS1_Latin-language_sources_(la)
    * Articles_needing_more_detailed_references
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_October_2018
    * Articles_to_be_expanded_from_February_2019
    * All_articles_to_be_expanded
    * Articles_with_empty_sections_from_February_2019
    * All_articles_with_empty_sections
    * Articles_using_small_message_boxes
    * Articles_lacking_reliable_references_from_February_2019
    * All_articles_lacking_reliable_references
    * Articles_with_inconsistent_citation_formats
    * Commons_category_link_is_on_Wikidata
    * Use_dmy_dates_from_January_2012
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
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AzÉrbaycanca
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * æè¨
    * ä¸­æ
Edit_links
    * This page was last edited on 25 June 2019, at 07:44 (UTC).
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
