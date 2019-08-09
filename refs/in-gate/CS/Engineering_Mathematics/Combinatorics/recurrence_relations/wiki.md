The following text has been accessed from https://en.wikipedia.org/wiki/Recurrence_relation at Fri Aug 9 01:08:56 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Recurrence relation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Definition of each term of a sequence as a function of the preceding ones
"Difference equation" redirects here. It is not to be confused with
differential_equation.
In mathematics, a recurrence relation is an equation that recursively defines a
sequence or multidimensional array of values, once one or more initial terms
are given; each further term of the sequence or array is defined as a function
of the preceding terms.
The term difference_equation sometimes (and for the purposes of this article)
refers to a specific type of recurrence relation. However, "difference
equation" is frequently used to refer to any recurrence relation.
⁰
***** Contents *****
    * 1_Definition
    * 2_Examples
          o 2.1_Factorial
          o 2.2_Logistic_map
          o 2.3_Fibonacci_numbers
          o 2.4_Binomial_coefficients
    * 3_Relationship_to_difference_equations_narrowly_defined
          o 3.1_From_sequences_to_grids
    * 4_Solving
          o 4.1_Solving_homogeneous_linear_recurrence_relations_with_constant
            coefficients
                # 4.1.1_Roots_of_the_characteristic_polynomial
                # 4.1.2_Solving_via_linear_algebra
                # 4.1.3_Solving_with_z-transforms
          o 4.2_Solving_non-homogeneous_linear_recurrence_relations_with
            constant_coefficients
          o 4.3_Solving_first-order_non-homogeneous_recurrence_relations_with
            variable_coefficients
          o 4.4_Solving_general_homogeneous_linear_recurrence_relations
          o 4.5_Solving_first-order_rational_difference_equations
    * 5_Stability
          o 5.1_Stability_of_linear_higher-order_recurrences
          o 5.2_Stability_of_linear_first-order_matrix_recurrences
          o 5.3_Stability_of_nonlinear_first-order_recurrences
    * 6_Relationship_to_differential_equations
    * 7_Applications
          o 7.1_Biology
          o 7.2_Computer_science
          o 7.3_Digital_signal_processing
          o 7.4_Economics
    * 8_See_also
    * 9_Notes
    * 10_References
    * 11_External_links
***** Definition[edit] *****
A recurrence relation is an equation that expresses each element of a sequence
as a function of the preceding ones. More precisely, in the case where only the
immediately preceding element is involved, a recurrence relation has the form
          u  n   = &#x03C6; ( n ,  u  n &#x2212; 1   )   for   n > 0 ,
      {\displaystyle u_{n}=\varphi (n,u_{n-1})\quad {\text{for}}\quad n>0,}  [
      {\displaystyle u_{n}=\varphi (n,u_{n-1})\quad {\text{for}}\quad n>0,}]
where
         &#x03C6; :  N  &#x00D7; X &#x2192; X   {\displaystyle \varphi :\mathbb
      {N} \times X\to X}  [{\displaystyle \varphi :\mathbb {N} \times X\to X}]
is a function, where X is a set to which the elements of a sequence must
belong. For any      u  0   &#x2208; X   {\displaystyle u_{0}\in X}  [
{\displaystyle u_{0}\in X}], this defines a unique sequence with      u  0
{\displaystyle u_{0}}  [u_{0}] as its first element, called the initial value.
[1]
It is easy to modify the definition for getting sequences starting from the
term of index 1 or higher.
This defines recurrence relation of first order. A recurrence relation of order
k has the form
          u  n   = &#x03C6; ( n ,  u  n &#x2212; 1   ,  u  n &#x2212; 2   ,
      &#x2026; ,  u  n &#x2212; k   )   for   n &#x2265; k ,   {\displaystyle
      u_{n}=\varphi (n,u_{n-1},u_{n-2},\ldots ,u_{n-k})\quad {\text{for}}\quad
      n\geq k,}  [{\displaystyle u_{n}=\varphi (n,u_{n-1},u_{n-2},\ldots ,u_{n-
      k})\quad {\text{for}}\quad n\geq k,}]
where     &#x03C6; :  N  &#x00D7;  X  k   &#x2192; X   {\displaystyle \varphi :
\mathbb {N} \times X^{k}\to X}  [{\displaystyle \varphi :\mathbb {N} \times X^
{k}\to X}] is a function that involves k consecutive elements of the sequence.
In this case, k initial values are needed for defining a sequence.
***** Examples[edit] *****
**** Factorial[edit] ****
The factorial is defined by the recurrence relation
         n ! = n ( n &#x2212; 1 ) !   for   n > 0 ,   {\displaystyle n!=n(n-
      1)!\quad {\text{for}}\quad n>0,}  [{\displaystyle n!=n(n-1)!\quad {\text
      {for}}\quad n>0,}]
and the initial condition
         0 ! = 1.   {\displaystyle 0!=1.}  [{\displaystyle 0!=1.}]
**** Logistic map[edit] ****
An example of a recurrence relation is the logistic_map:
          x  n + 1   = r  x  n   ( 1 &#x2212;  x  n   ) ,   {\displaystyle x_
      {n+1}=rx_{n}(1-x_{n}),}  [x_{n+1}=rx_{n}(1-x_{n}),]
with a given constant r; given the initial term x0 each subsequent term is
determined by this relation.
Solving a recurrence relation means obtaining a closed-form_solution: a non-
recursive function of n.
**** Fibonacci numbers[edit] ****
The recurrence of order two satisfied by the Fibonacci_numbers is the archetype
of a homogeneous linear_recurrence relation with constant coefficients (see
below). The Fibonacci sequence is defined using the recurrence
          F  n   =  F  n &#x2212; 1   +  F  n &#x2212; 2     {\displaystyle F_
      {n}=F_{n-1}+F_{n-2}}  [F_{n}=F_{n-1}+F_{n-2}]
with initial_conditions (seed values)
          F  0   = 0   {\displaystyle F_{0}=0}  [F_{0}=0]
          F  1   = 1.   {\displaystyle F_{1}=1.}  [{\displaystyle F_{1}=1.}]
Explicitly, the recurrence yields the equations
          F  2   =  F  1   +  F  0     {\displaystyle F_{2}=F_{1}+F_{0}}  [F_
      {2}=F_{1}+F_{0}]
          F  3   =  F  2   +  F  1     {\displaystyle F_{3}=F_{2}+F_{1}}  [F_
      {3}=F_{2}+F_{1}]
          F  4   =  F  3   +  F  2     {\displaystyle F_{4}=F_{3}+F_{2}}  [F_
      {4}=F_{3}+F_{2}]
etc.
We obtain the sequence of Fibonacci numbers, which begins
      0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, ...
The recurrence can be solved by methods described below yielding Binet's
formula, which involves powers of the two roots of the characteristic
polynomial t2 = t + 1; the generating_function of the sequence is the rational
function
           t  1 &#x2212; t &#x2212;  t  2      .   {\displaystyle {\frac {t}{1-
      t-t^{2}}}.}  [{\frac {t}{1-t-t^{2}}}.]
**** Binomial coefficients[edit] ****
A simple example of a multidimensional recurrence relation is given by the
binomial_coefficients         (   n k   )       {\displaystyle {\tbinom {n}
{k}}}  [{\tbinom {n}{k}}], which count the number of ways of selecting k
elements out of a set of n elements. They can be computed by the recurrence
relation
            (   n k   )    =    (    n &#x2212; 1   k &#x2212; 1    )    +
      (    n &#x2212; 1  k   )    ,   {\displaystyle {\binom {n}{k}}={\binom
      {n-1}{k-1}}+{\binom {n-1}{k}},}  [{\binom {n}{k}}={\binom {n-1}{k-1}}+
      {\binom {n-1}{k}},]
with the base cases         (   n 0   )     =     (   n n   )     = 1
{\displaystyle {\tbinom {n}{0}}={\tbinom {n}{n}}=1}  [{\tbinom {n}{0}}={\tbinom
{n}{n}}=1]. Using this formula to compute the values of all binomial
coefficients generates an infinite array called Pascal's_triangle. The same
values can also be computed directly by a different formula that is not a
recurrence, but that requires multiplication and not just addition to compute:
(   n k   )    =    n !   k ! ( n &#x2212; k ) !    .   {\displaystyle {\binom
{n}{k}}={\frac {n!}{k!(n-k)!}}.}  [{\binom {n}{k}}={\frac {n!}{k!(n-k)!}}.]
***** Relationship to difference equations narrowly defined[edit] *****
Given an ordered sequence       {  a  n   }   n = 1   &#x221E;
{\displaystyle \left\{a_{n}\right\}_{n=1}^{\infty }}  [\left\{a_{n}\right\}_
{n=1}^{\infty }] of real_numbers: the first difference     &#x0394; (  a  n   )
{\displaystyle \Delta (a_{n})}  [\Delta (a_{n})] is defined as
         &#x0394; (  a  n   ) =  a  n + 1   &#x2212;  a  n   .   {\displaystyle
      \Delta (a_{n})=a_{n+1}-a_{n}.}  [{\displaystyle \Delta (a_{n})=a_{n+1}-a_
      {n}.}]
The second difference      &#x0394;  2   (  a  n   )   {\displaystyle \Delta ^
{2}(a_{n})}  [\Delta ^{2}(a_{n})] is defined as
          &#x0394;  2   (  a  n   ) = &#x0394; (  a  n + 1   ) &#x2212;
      &#x0394; (  a  n   ) ,   {\displaystyle \Delta ^{2}(a_{n})=\Delta (a_
      {n+1})-\Delta (a_{n}),}  [{\displaystyle \Delta ^{2}(a_{n})=\Delta (a_
      {n+1})-\Delta (a_{n}),}]
which can be simplified to
          &#x0394;  2   (  a  n   ) =  a  n + 2   &#x2212; 2  a  n + 1   +  a
      n   .   {\displaystyle \Delta ^{2}(a_{n})=a_{n+2}-2a_{n+1}+a_{n}.}  [
      {\displaystyle \Delta ^{2}(a_{n})=a_{n+2}-2a_{n+1}+a_{n}.}]
More generally: the k-th difference of the sequence an written as      &#x0394;
k   (  a  n   )   {\displaystyle \Delta ^{k}(a_{n})}  [\Delta ^{k}(a_{n})] is
defined recursively as
          &#x0394;  k   (  a  n   ) =  &#x0394;  k &#x2212; 1   (  a  n + 1   )
      &#x2212;  &#x0394;  k &#x2212; 1   (  a  n   ) =  &#x2211;  t = 0   k
      (   k t   )    ( &#x2212; 1  )  t    a  n + k &#x2212; t   .
      {\displaystyle \Delta ^{k}(a_{n})=\Delta ^{k-1}(a_{n+1})-\Delta ^{k-1}(a_
      {n})=\sum _{t=0}^{k}{\binom {k}{t}}(-1)^{t}a_{n+k-t}.}  [{\displaystyle
      \Delta ^{k}(a_{n})=\Delta ^{k-1}(a_{n+1})-\Delta ^{k-1}(a_{n})=\sum _
      {t=0}^{k}{\binom {k}{t}}(-1)^{t}a_{n+k-t}.}]
(The sequence and its differences are related by a binomial_transform.) The
more restrictive definition of difference equation is an equation composed of
an and its kth differences. (A widely used broader definition treats
"difference equation" as synonymous with "recurrence relation". See for example
rational_difference_equation and matrix_difference_equation.)
Actually, it is easily seen that,
          a  n + k   =    (   k 0   )     a  n   +    (   k 1   )    &#x0394;
      (  a  n   ) + &#x22EF; +    (   k k   )     &#x0394;  k   (  a  n   ) .
      {\displaystyle a_{n+k}={k \choose 0}a_{n}+{k \choose 1}\Delta (a_
      {n})+\cdots +{k \choose k}\Delta ^{k}(a_{n}).}  [{\displaystyle a_{n+k}=
      {k \choose 0}a_{n}+{k \choose 1}\Delta (a_{n})+\cdots +{k \choose
      k}\Delta ^{k}(a_{n}).}]
Thus, a difference equation can be defined as an equation that involves an, an-
1, an-2 etc. (or equivalently an, an+1, an+2 etc.)
Since difference equations are a very common form of recurrence, some authors
use the two terms interchangeably. For example, the difference equation
         3  &#x0394;  2   (  a  n   ) + 2 &#x0394; (  a  n   ) + 7  a  n   = 0
      {\displaystyle 3\Delta ^{2}(a_{n})+2\Delta (a_{n})+7a_{n}=0}  [3\Delta ^
      {2}(a_{n})+2\Delta (a_{n})+7a_{n}=0]
is equivalent to the recurrence relation
         3  a  n + 2   = 4  a  n + 1   &#x2212; 8  a  n   .   {\displaystyle
      3a_{n+2}=4a_{n+1}-8a_{n}.}  [{\displaystyle 3a_{n+2}=4a_{n+1}-8a_{n}.}]
Thus one can solve many recurrence relations by rephrasing them as difference
equations, and then solving the difference equation, analogously to how one
solves ordinary_differential_equations. However, the Ackermann_numbers are an
example of a recurrence relation that do not map to a difference equation, much
less points on the solution to a differential equation.
See time_scale_calculus for a unification of the theory of difference equations
with that of differential_equations.
Summation_equations relate to difference equations as integral_equations relate
to differential equations.
**** From sequences to grids[edit] ****
Single-variable or one-dimensional recurrence relations are about sequences
(i.e. functions defined on one-dimensional grids). Multi-variable or n-
dimensional recurrence relations are about n-dimensional grids. Functions
defined on n-grids can also be studied with partial difference equations.[2]
***** Solving[edit] *****
**** Solving homogeneous linear recurrence relations with constant coefficients
[edit] ****
Main articles: Constant-recursive_sequence and Linear_difference_equation
*** Roots of the characteristic polynomial[edit] ***
An order-d homogeneous linear recurrence with constant coefficients is an
equation of the form
          a  n   =  c  1    a  n &#x2212; 1   +  c  2    a  n &#x2212; 2   +
      &#x22EF; +  c  d    a  n &#x2212; d   ,   {\displaystyle a_{n}=c_{1}a_{n-
      1}+c_{2}a_{n-2}+\cdots +c_{d}a_{n-d},}  [a_{n}=c_{1}a_{n-1}+c_{2}a_{n-
      2}+\cdots +c_{d}a_{n-d},]
where the d coefficients ci (for all i) are constants, and      c  d   &#x2260;
0   {\displaystyle c_{d}\neq 0}  [{\displaystyle c_{d}\neq 0}].
A constant-recursive_sequence is a sequence satisfying a recurrence of this
form. There are d degrees_of_freedom for solutions to this recurrence, i.e.,
the initial values      a  0   , &#x2026; ,  a  d &#x2212; 1     {\displaystyle
a_{0},\dots ,a_{d-1}}  [a_{0},\dots ,a_{d-1}] can be taken to be any values but
then the recurrence determines the sequence uniquely.
The same coefficients yield the characteristic_polynomial (also "auxiliary
polynomial")
         p ( t ) =  t  d   &#x2212;  c  1    t  d &#x2212; 1   &#x2212;  c  2
      t  d &#x2212; 2   &#x2212; &#x22EF; &#x2212;  c  d     {\displaystyle p
      (t)=t^{d}-c_{1}t^{d-1}-c_{2}t^{d-2}-\cdots -c_{d}}  [p(t)=t^{d}-c_{1}t^
      {d-1}-c_{2}t^{d-2}-\cdots -c_{d}]
whose d roots play a crucial role in finding and understanding the sequences
satisfying the recurrence. If the roots r1, r2, ... are all distinct, then each
solution to the recurrence takes the form
          a  n   =  k  1    r  1   n   +  k  2    r  2   n   + &#x22EF; +  k  d
      r  d   n   ,   {\displaystyle a_{n}=k_{1}r_{1}^{n}+k_{2}r_{2}^{n}+\cdots
      +k_{d}r_{d}^{n},}  [a_{n}=k_{1}r_{1}^{n}+k_{2}r_{2}^{n}+\cdots +k_{d}r_
      {d}^{n},]
where the coefficients ki are determined in order to fit the initial conditions
of the recurrence. When the same roots occur multiple times, the terms in this
formula corresponding to the second and later occurrences of the same root are
multiplied by increasing powers of n. For instance, if the characteristic
polynomial can be factored as (xâr)3, with the same root r occurring three
times, then the solution would take the form
          a  n   =  k  1    r  n   +  k  2   n  r  n   +  k  3    n  2    r  n
      .   {\displaystyle a_{n}=k_{1}r^{n}+k_{2}nr^{n}+k_{3}n^{2}r^{n}.}  [a_
      {n}=k_{1}r^{n}+k_{2}nr^{n}+k_{3}n^{2}r^{n}.][3]
As well as the Fibonacci_numbers, other constant-recursive sequences include
the Lucas_numbers and Lucas_sequences, the Jacobsthal_numbers, the Pell_numbers
and more generally the solutions to Pell's_equation.
For order 1, the recurrence
          a  n   = r  a  n &#x2212; 1     {\displaystyle a_{n}=ra_{n-1}}  [a_
      {n}=ra_{n-1}]
has the solution an = rn with a0 = 1 and the most general solution is an = krn
with a0 = k. The characteristic polynomial equated to zero (the characteristic
equation) is simply t â r = 0.
Solutions to such recurrence relations of higher order are found by systematic
means, often using the fact that an = rn is a solution for the recurrence
exactly when t = r is a root of the characteristic polynomial. This can be
approached directly or using generating_functions (formal_power_series) or
matrices.
Consider, for example, a recurrence relation of the form
          a  n   = A  a  n &#x2212; 1   + B  a  n &#x2212; 2   .
      {\displaystyle a_{n}=Aa_{n-1}+Ba_{n-2}.}  [a_{n}=Aa_{n-1}+Ba_{n-2}.]
When does it have a solution of the same general form as an = rn? Substituting
this guess (ansatz) in the recurrence relation, we find that
          r  n   = A  r  n &#x2212; 1   + B  r  n &#x2212; 2     {\displaystyle
      r^{n}=Ar^{n-1}+Br^{n-2}}  [r^{n}=Ar^{n-1}+Br^{n-2}]
must be true for all n > 1.
Dividing through by rnâ2, we get that all these equations reduce to the same
thing:
          r  2   = A r + B ,   {\displaystyle r^{2}=Ar+B,}  [r^{2}=Ar+B,]
          r  2   &#x2212; A r &#x2212; B = 0 ,   {\displaystyle r^{2}-Ar-B=0,}
      [r^{2}-Ar-B=0,]
which is the characteristic equation of the recurrence relation. Solve for r to
obtain the two roots Î»1, Î»2: these roots are known as the characteristic
roots or eigenvalues of the characteristic equation. Different solutions are
obtained depending on the nature of the roots: If these roots are distinct, we
have the general solution
          a  n   = C  &#x03BB;  1   n   + D  &#x03BB;  2   n     {\displaystyle
      a_{n}=C\lambda _{1}^{n}+D\lambda _{2}^{n}}  [a_{n}=C\lambda _{1}^
      {n}+D\lambda _{2}^{n}]
while if they are identical (when A2 + 4B = 0), we have
          a  n   = C  &#x03BB;  n   + D n  &#x03BB;  n     {\displaystyle a_
      {n}=C\lambda ^{n}+Dn\lambda ^{n}}  [a_{n}=C\lambda ^{n}+Dn\lambda ^{n}]
This is the most general solution; the two constants C and D can be chosen
based on two given initial conditions a0 and a1 to produce a specific solution.
In the case of complex eigenvalues (which also gives rise to complex values for
the solution parameters C and D), the use of complex numbers can be eliminated
by rewriting the solution in trigonometric form. In this case we can write the
eigenvalues as      &#x03BB;  1   ,  &#x03BB;  2   = &#x03B1; &#x00B1; &#x03B2;
i .   {\displaystyle \lambda _{1},\lambda _{2}=\alpha \pm \beta i.}  [\lambda _
{1},\lambda _{2}=\alpha \pm \beta i.] Then it can be shown that
          a  n   = C  &#x03BB;  1   n   + D  &#x03BB;  2   n     {\displaystyle
      a_{n}=C\lambda _{1}^{n}+D\lambda _{2}^{n}}  [a_{n}=C\lambda _{1}^
      {n}+D\lambda _{2}^{n}]
can be rewritten as[4]:576â585
          a  n   = 2  M  n    (  E cos &#x2061; ( &#x03B8; n ) + F sin &#x2061;
      ( &#x03B8; n )  )  = 2 G  M  n   cos &#x2061; ( &#x03B8; n &#x2212;
      &#x03B4; ) ,   {\displaystyle a_{n}=2M^{n}\left(E\cos(\theta n)+F\sin
      (\theta n)\right)=2GM^{n}\cos(\theta n-\delta ),}  [a_{n}=2M^{n}\left
      (E\cos(\theta n)+F\sin(\theta n)\right)=2GM^{n}\cos(\theta n-\delta ),]
where
             M =    &#x03B1;  2   +  &#x03B2;  2       cos &#x2061; ( &#x03B8;
      ) =    &#x03B1; M      sin &#x2061; ( &#x03B8; ) =    &#x03B2; M        C
      , D = E &#x2213; F i       G =    E  2   +  F  2       cos &#x2061;
      ( &#x03B4; ) =    E G      sin &#x2061; ( &#x03B4; ) =    F G
      {\displaystyle {\begin{array}{lcl}M={\sqrt {\alpha ^{2}+\beta ^{2}}}&\cos
      (\theta )={\tfrac {\alpha }{M}}&\sin(\theta )={\tfrac {\beta }
      {M}}\\C,D=E\mp Fi&&\\G={\sqrt {E^{2}+F^{2}}}&\cos(\delta )={\tfrac {E}
      {G}}&\sin(\delta )={\tfrac {F}{G}}\end{array}}}  [{\begin{array}{lcl}M=
      {\sqrt {\alpha ^{2}+\beta ^{2}}}&\cos(\theta )={\tfrac {\alpha }{M}}&\sin
      (\theta )={\tfrac {\beta }{M}}\\C,D=E\mp Fi&&\\G={\sqrt {E^{2}+F^
      {2}}}&\cos(\delta )={\tfrac {E}{G}}&\sin(\delta )={\tfrac {F}{G}}\end
      {array}}]
Here E and F (or equivalently, G and Î´) are real constants which depend on the
initial conditions. Using
          &#x03BB;  1   +  &#x03BB;  2   = 2 &#x03B1; = A ,   {\displaystyle
      \lambda _{1}+\lambda _{2}=2\alpha =A,}  [\lambda _{1}+\lambda _
      {2}=2\alpha =A,]
          &#x03BB;  1   &#x22C5;  &#x03BB;  2   =  &#x03B1;  2   +  &#x03B2;  2
      = &#x2212; B ,   {\displaystyle \lambda _{1}\cdot \lambda _{2}=\alpha ^
      {2}+\beta ^{2}=-B,}  [\lambda _{1}\cdot \lambda _{2}=\alpha ^{2}+\beta ^
      {2}=-B,]
one may simplify the solution given above as
          a  n   = ( &#x2212; B  )   n 2     (  E cos &#x2061; ( &#x03B8; n ) +
      F sin &#x2061; ( &#x03B8; n )  )  ,   {\displaystyle a_{n}=(-B)^{\frac
      {n}{2}}\left(E\cos(\theta n)+F\sin(\theta n)\right),}  [a_{n}=(-B)^{\frac
      {n}{2}}\left(E\cos(\theta n)+F\sin(\theta n)\right),]
where a1 and a2 are the initial conditions and
             E    =    &#x2212; A  a  1   +  a  2    B       F    = &#x2212; i
      A  2    a  1   &#x2212; A  a  2   + 2  a  1   B   B    A  2   + 4 B
      &#x03B8;    = arccos &#x2061;  (   A  2   &#x2212; B      )
      {\displaystyle {\begin{aligned}E&={\frac {-Aa_{1}+a_{2}}{B}}\\F&=-i{\frac
      {A^{2}a_{1}-Aa_{2}+2a_{1}B}{B{\sqrt {A^{2}+4B}}}}\\\theta &=\arccos \left
      ({\frac {A}{2{\sqrt {-B}}}}\right)\end{aligned}}}  [{\begin{aligned}E&=
      {\frac {-Aa_{1}+a_{2}}{B}}\\F&=-i{\frac {A^{2}a_{1}-Aa_{2}+2a_{1}B}{B
      {\sqrt {A^{2}+4B}}}}\\\theta &=\arccos \left({\frac {A}{2{\sqrt {-
      B}}}}\right)\end{aligned}}]
In this way there is no need to solve for Î»1 and Î»2.
In all casesâreal distinct eigenvalues, real duplicated eigenvalues, and
complex conjugate eigenvaluesâthe equation is stable (that is, the variable a
converges to a fixed value [specifically, zero]) if and only if both
eigenvalues are smaller than one in absolute_value. In this second-order case,
this condition on the eigenvalues can be shown[5] to be equivalent to
|A| < 1 â B < 2, which is equivalent to |B| < 1 and |A| < 1 â B.
The equation in the above example was homogeneous, in that there was no
constant term. If one starts with the non-homogeneous recurrence
          b  n   = A  b  n &#x2212; 1   + B  b  n &#x2212; 2   + K
      {\displaystyle b_{n}=Ab_{n-1}+Bb_{n-2}+K}  [b_{n}=Ab_{n-1}+Bb_{n-2}+K]
with constant term K, this can be converted into homogeneous form as follows:
The steady_state is found by setting bn = bnâ1 = bnâ2 = b* to obtain
          b  &#x2217;   =   K  1 &#x2212; A &#x2212; B    .   {\displaystyle b^
      {*}={\frac {K}{1-A-B}}.}  [b^{*}={\frac {K}{1-A-B}}.]
Then the non-homogeneous recurrence can be rewritten in homogeneous form as
         [  b  n   &#x2212;  b  &#x2217;   ] = A [  b  n &#x2212; 1   &#x2212;
      b  &#x2217;   ] + B [  b  n &#x2212; 2   &#x2212;  b  &#x2217;   ] ,
      {\displaystyle [b_{n}-b^{*}]=A[b_{n-1}-b^{*}]+B[b_{n-2}-b^{*}],}  [[b_
      {n}-b^{*}]=A[b_{n-1}-b^{*}]+B[b_{n-2}-b^{*}],]
which can be solved as above.
The stability condition stated above in terms of eigenvalues for the second-
order case remains valid for the general nth-order case: the equation is stable
if and only if all eigenvalues of the characteristic equation are less than one
in absolute value.
Given a homogeneous linear recurrence relation with constant coefficients of
order d, let p(t) be the characteristic_polynomial (also "auxiliary
polynomial")
          t  d   &#x2212;  c  1    t  d &#x2212; 1   &#x2212;  c  2    t  d
      &#x2212; 2   &#x2212; &#x22EF; &#x2212;  c  d   = 0   {\displaystyle t^
      {d}-c_{1}t^{d-1}-c_{2}t^{d-2}-\cdots -c_{d}=0}  [{\displaystyle t^{d}-c_
      {1}t^{d-1}-c_{2}t^{d-2}-\cdots -c_{d}=0}]
such that each ci corresponds to each ci in the original recurrence relation
(see the general form above). Suppose λ is a root of p(t) having multiplicity
r. This is to say that (tâÎ»)r divides p(t). The following two properties
hold:
   1. Each of the r sequences      &#x03BB;  n   , n  &#x03BB;  n   ,  n  2
      &#x03BB;  n   , &#x2026; ,  n  r &#x2212; 1    &#x03BB;  n
      {\displaystyle \lambda ^{n},n\lambda ^{n},n^{2}\lambda ^{n},\dots ,n^{r-
      1}\lambda ^{n}}  [\lambda ^{n},n\lambda ^{n},n^{2}\lambda ^{n},\dots ,n^
      {r-1}\lambda ^{n}] satisfies the recurrence relation.
   2. Any sequence satisfying the recurrence relation can be written uniquely
      as a linear combination of solutions constructed in part 1 as Î» varies
      over all distinct roots of p(t).
As a result of this theorem a homogeneous linear recurrence relation with
constant coefficients can be solved in the following manner:
   1. Find the characteristic polynomial p(t).
   2. Find the roots of p(t) counting multiplicity.
   3. Write an as a linear combination of all the roots (counting multiplicity
      as shown in the theorem above) with unknown coefficients bi.
                a  n   =  (   b  1    &#x03BB;  1   n   +  b  2   n  &#x03BB;
            1   n   +  b  3    n  2    &#x03BB;  1   n   + &#x22EF; +  b  r
            n  r &#x2212; 1    &#x03BB;  1   n    )  + &#x22EF; +  (   b  d
            &#x2212; q + 1    &#x03BB;  &#x2217;   n   + &#x22EF; +  b  d    n
            q &#x2212; 1    &#x03BB;  &#x2217;   n    )    {\displaystyle a_
            {n}=\left(b_{1}\lambda _{1}^{n}+b_{2}n\lambda _{1}^{n}+b_{3}n^
            {2}\lambda _{1}^{n}+\cdots +b_{r}n^{r-1}\lambda _{1}^
            {n}\right)+\cdots +\left(b_{d-q+1}\lambda _{*}^{n}+\cdots +b_{d}n^
            {q-1}\lambda _{*}^{n}\right)}  [a_{n}=\left(b_{1}\lambda _{1}^
            {n}+b_{2}n\lambda _{1}^{n}+b_{3}n^{2}\lambda _{1}^{n}+\cdots +b_
            {r}n^{r-1}\lambda _{1}^{n}\right)+\cdots +\left(b_{d-q+1}\lambda _
            {*}^{n}+\cdots +b_{d}n^{q-1}\lambda _{*}^{n}\right)]
      This is the general solution to the original recurrence relation. (q is
      the multiplicity of Î»*)
      4. Equate each      a  0   ,  a  1   , &#x2026; ,  a  d
      {\displaystyle a_{0},a_{1},\dots ,a_{d}}  [a_{0},a_{1},\dots ,a_{d}] from
      part 3 (plugging in n = 0, ..., d into the general solution of the
      recurrence relation) with the known values      a  0   ,  a  1   ,
      &#x2026; ,  a  d     {\displaystyle a_{0},a_{1},\dots ,a_{d}}  [a_{0},a_
      {1},\dots ,a_{d}] from the original recurrence relation. However, the
      values an from the original recurrence relation used do not usually have
      to be contiguous: excluding exceptional cases, just d of them are needed
      (i.e., for an original homogeneous linear recurrence relation of order 3
      one could use the values a0, a1, a4). This process will produce a linear
      system of d equations with d unknowns. Solving these equations for the
      unknown coefficients      b  1   ,  b  2   , &#x2026; ,  b  d
      {\displaystyle b_{1},b_{2},\dots ,b_{d}}  [b_{1},b_{2},\dots ,b_{d}] of
      the general solution and plugging these values back into the general
      solution will produce the particular solution to the original recurrence
      relation that fits the original recurrence relation's initial conditions
      (as well as all subsequent values      a  0   ,  a  1   ,  a  2   ,
      &#x2026;   {\displaystyle a_{0},a_{1},a_{2},\dots }  [a_{0},a_{1},a_
      {2},\dots ] of the original recurrence relation).
The method for solving linear differential_equations is similar to the method
aboveâthe "intelligent guess" (ansatz) for linear differential equations with
constant coefficients is eÎ»x where Î» is a complex number that is determined
by substituting the guess into the differential equation.
This is not a coincidence. Considering the Taylor_series of the solution to a
linear differential equation:
          &#x2211;  n = 0   &#x221E;       f  ( n )   ( a )   n !    ( x
      &#x2212; a  )  n     {\displaystyle \sum _{n=0}^{\infty }{\frac {f^{(n)}
      (a)}{n!}}(x-a)^{n}}  [\sum _{n=0}^{\infty }{\frac {f^{(n)}(a)}{n!}}(x-a)^
      {n}]
it can be seen that the coefficients of the series are given by the nth
derivative of f(x) evaluated at the point a. The differential equation provides
a linear difference equation relating these coefficients.
This equivalence can be used to quickly solve for the recurrence relationship
for the coefficients in the power series solution of a linear differential
equation.
The rule of thumb (for equations in which the polynomial multiplying the first
term is non-zero at zero) is that:
          y  [ k ]   &#x2192; f [ n + k ]   {\displaystyle y^{[k]}\to f[n+k]}
      [y^{[k]}\to f[n+k]]
and more generally
          x  m   &#x2217;  y  [ k ]   &#x2192; n ( n &#x2212; 1 ) . . . ( n
      &#x2212; m + 1 ) f [ n + k &#x2212; m ]   {\displaystyle x^{m}*y^{[k]}\to
      n(n-1)...(n-m+1)f[n+k-m]}  [{\displaystyle x^{m}*y^{[k]}\to n(n-1)...(n-
      m+1)f[n+k-m]}]
Example: The recurrence relationship for the Taylor series coefficients of the
equation:
         (  x  2   + 3 x &#x2212; 4 )  y  [ 3 ]   &#x2212; ( 3 x + 1 )  y  [ 2
      ]   + 2 y = 0   {\displaystyle (x^{2}+3x-4)y^{[3]}-(3x+1)y^{[2]}+2y=0}  [
      (x^{2}+3x-4)y^{[3]}-(3x+1)y^{[2]}+2y=0]
is given by
         n ( n &#x2212; 1 ) f [ n + 1 ] + 3 n f [ n + 2 ] &#x2212; 4 f [ n + 3
      ] &#x2212; 3 n f [ n + 1 ] &#x2212; f [ n + 2 ] + 2 f [ n ] = 0
      {\displaystyle n(n-1)f[n+1]+3nf[n+2]-4f[n+3]-3nf[n+1]-f[n+2]+2f[n]=0}  [n
      (n-1)f[n+1]+3nf[n+2]-4f[n+3]-3nf[n+1]-f[n+2]+2f[n]=0]
or
         &#x2212; 4 f [ n + 3 ] + 2 n f [ n + 2 ] + n ( n &#x2212; 4 ) f [ n +
      1 ] + 2 f [ n ] = 0.   {\displaystyle -4f[n+3]+2nf[n+2]+n(n-4)f[n+1]+2f
      [n]=0.}  [-4f[n+3]+2nf[n+2]+n(n-4)f[n+1]+2f[n]=0.]
This example shows how problems generally solved using the power series
solution method taught in normal differential equation classes can be solved in
a much easier way.
Example: The differential equation
         a  y &#x2033;  + b  y &#x2032;  + c y = 0   {\displaystyle
      ay''+by'+cy=0}  [ay''+by'+cy=0]
has solution
         y =  e  a x   .   {\displaystyle y=e^{ax}.}  [y=e^{ax}.]
The conversion of the differential equation to a difference equation of the
Taylor coefficients is
         a f [ n + 2 ] + b f [ n + 1 ] + c f [ n ] = 0.   {\displaystyle af
      [n+2]+bf[n+1]+cf[n]=0.}  [af[n+2]+bf[n+1]+cf[n]=0.]
It is easy to see that the nth derivative of eax evaluated at 0 is an
*** Solving via linear algebra[edit] ***
A linearly recursive sequence y of order n
          y  n + k   &#x2212;  c  n &#x2212; 1    y  n &#x2212; 1 + k
      &#x2212;  c  n &#x2212; 2    y  n &#x2212; 2 + k   + &#x22EF; &#x2212;  c
      0    y  k   = 0   {\displaystyle y_{n+k}-c_{n-1}y_{n-1+k}-c_{n-2}y_{n-
      2+k}+\cdots -c_{0}y_{k}=0}  [y_{n+k}-c_{n-1}y_{n-1+k}-c_{n-2}y_{n-
      2+k}+\cdots -c_{0}y_{k}=0]
is identical to
          y  n   =  c  n &#x2212; 1    y  n &#x2212; 1   +  c  n &#x2212; 2
      y  n &#x2212; 2   + &#x22EF; +  c  0    y  0   .   {\displaystyle y_
      {n}=c_{n-1}y_{n-1}+c_{n-2}y_{n-2}+\cdots +c_{0}y_{0}.}  [y_{n}=c_{n-1}y_
      {n-1}+c_{n-2}y_{n-2}+\cdots +c_{0}y_{0}.]
Expanded with n-1 identities of kind      y  n &#x2212; k   =  y  n &#x2212; k
,   {\displaystyle y_{n-k}=y_{n-k},}  [y_{n-k}=y_{n-k},] this n-th order
equation is translated into a matrix_difference_equation system of n first-
order linear equations,
             y &#x2192;     n   =   [     y  n        y  n &#x2212; 1
      &#x22EE;     &#x22EE;      y  1      ]   =   [     c  n &#x2212; 1      c
      n &#x2212; 2     &#x22EF;   &#x22EF;    c  0       1   0   &#x22EF;
      &#x22EF;   0     0   &#x22F1;   &#x22F1;    &#x22EE;     &#x22EE;
      &#x22F1;   &#x22F1;   &#x22F1;   &#x22EE;     0   &#x22EF;   0   1   0
      ]     [     y  n &#x2212; 1        y  n &#x2212; 2       &#x22EE;
      &#x22EE;      y  0      ]   = C &#xA0;     y &#x2192;     n &#x2212; 1
      =  C  n       y &#x2192;     0   .   {\displaystyle {\vec {y}}_{n}=
      {\begin{bmatrix}y_{n}\\y_{n-1}\\\vdots \\\vdots \\y_{1}\end{bmatrix}}=
      {\begin{bmatrix}c_{n-1}&c_{n-2}&\cdots &\cdots &c_{0}\\1&0&\cdots &\cdots
      &0\\0&\ddots &\ddots &&\vdots \\\vdots &\ddots &\ddots &\ddots &\vdots
      \\0&\cdots &0&1&0\end{bmatrix}}{\begin{bmatrix}y_{n-1}\\y_{n-2}\\\vdots
      \\\vdots \\y_{0}\end{bmatrix}}=C\ {\vec {y}}_{n-1}=C^{n}{\vec {y}}_{0}.}
      [{\displaystyle {\vec {y}}_{n}={\begin{bmatrix}y_{n}\\y_{n-1}\\\vdots
      \\\vdots \\y_{1}\end{bmatrix}}={\begin{bmatrix}c_{n-1}&c_{n-2}&\cdots
      &\cdots &c_{0}\\1&0&\cdots &\cdots &0\\0&\ddots &\ddots &&\vdots \\\vdots
      &\ddots &\ddots &\ddots &\vdots \\0&\cdots &0&1&0\end{bmatrix}}{\begin
      {bmatrix}y_{n-1}\\y_{n-2}\\\vdots \\\vdots \\y_{0}\end{bmatrix}}=C\ {\vec
      {y}}_{n-1}=C^{n}{\vec {y}}_{0}.}]
Observe that the vector         y &#x2192;     n     {\displaystyle {\vec {y}}_
{n}}  [{\vec {y}}_{n}] can be computed by n applications of the companion
matrix, C, to the initial state vector,      y  0     {\displaystyle y_{0}}
[y_{0}]. Thereby, n-th entry of the sought sequence y, is the top component of
y &#x2192;     n   ,  y  n   =     y &#x2192;     n   [ n ]   {\displaystyle
{\vec {y}}_{n},y_{n}={\vec {y}}_{n}[n]}  [{\vec {y}}_{n},y_{n}={\vec {y}}_{n}
[n]].
Eigendecomposition,         y &#x2192;     n   =  C  n        y &#x2192;     0
=  c  1     &#x03BB;  1   n        e &#x2192;     1   +  c  2     &#x03BB;  2
n        e &#x2192;     2   + &#x22EF; +  c  n     &#x03BB;  n   n        e
&#x2192;     n     {\displaystyle {\vec {y}}_{n}=C^{n}\,{\vec {y}}_{0}=c_
{1}\,\lambda _{1}^{n}\,{\vec {e}}_{1}+c_{2}\,\lambda _{2}^{n}\,{\vec {e}}_
{2}+\cdots +c_{n}\,\lambda _{n}^{n}\,{\vec {e}}_{n}}  [{\displaystyle {\vec
{y}}_{n}=C^{n}\,{\vec {y}}_{0}=c_{1}\,\lambda _{1}^{n}\,{\vec {e}}_{1}+c_
{2}\,\lambda _{2}^{n}\,{\vec {e}}_{2}+\cdots +c_{n}\,\lambda _{n}^{n}\,{\vec
{e}}_{n}}] into eigenvalues,      &#x03BB;  1   ,  &#x03BB;  2   , &#x2026; ,
&#x03BB;  n     {\displaystyle \lambda _{1},\lambda _{2},\ldots ,\lambda _{n}}
[\lambda _{1},\lambda _{2},\ldots ,\lambda _{n}], and eigenvectors,         e
&#x2192;     1   ,     e &#x2192;     2   , &#x2026; ,     e &#x2192;     n
{\displaystyle {\vec {e}}_{1},{\vec {e}}_{2},\ldots ,{\vec {e}}_{n}}  [{\vec
{e}}_{1},{\vec {e}}_{2},\ldots ,{\vec {e}}_{n}], is used to compute         y
&#x2192;     n   .   {\displaystyle {\vec {y}}_{n}.}  [{\vec {y}}_{n}.] Thanks
to the crucial fact that system C time-shifts every eigenvector, e, by simply
scaling its components Î» times,
         C      e &#x2192;     i   =  &#x03BB;  i       e &#x2192;     i   = C
      [     e  i , n        e  i , n &#x2212; 1       &#x22EE;      e  i , 1
      ]   =   [     &#x03BB;  i     e  i , n        &#x03BB;  i     e  i , n
      &#x2212; 1       &#x22EE;      &#x03BB;  i     e  i , 1      ]
      {\displaystyle C\,{\vec {e}}_{i}=\lambda _{i}{\vec {e}}_{i}=C{\begin
      {bmatrix}e_{i,n}\\e_{i,n-1}\\\vdots \\e_{i,1}\end{bmatrix}}={\begin
      {bmatrix}\lambda _{i}\,e_{i,n}\\\lambda _{i}\,e_{i,n-1}\\\vdots \\\lambda
      _{i}\,e_{i,1}\end{bmatrix}}}  [C\,{\vec {e}}_{i}=\lambda _{i}{\vec {e}}_
      {i}=C{\begin{bmatrix}e_{i,n}\\e_{i,n-1}\\\vdots \\e_{i,1}\end{bmatrix}}=
      {\begin{bmatrix}\lambda _{i}\,e_{i,n}\\\lambda _{i}\,e_{i,n-1}\\\vdots
      \\\lambda _{i}\,e_{i,1}\end{bmatrix}}]
that is, time-shifted version of eigenvector,e, has components Î» times larger,
the eigenvector components are powers of Î»,         e &#x2192;     i   =
[     &#x03BB;  i   n &#x2212; 1     &#x22EF;    &#x03BB;  i   2      &#x03BB;
i     1    ]    T   ,   {\displaystyle {\vec {e}}_{i}={\begin{bmatrix}\lambda _
{i}^{n-1}&\cdots &\lambda _{i}^{2}&\lambda _{i}&1\end{bmatrix}}^{T},}  [{\vec
{e}}_{i}={\begin{bmatrix}\lambda _{i}^{n-1}&\cdots &\lambda _{i}^{2}&\lambda _
{i}&1\end{bmatrix}}^{T},] and, thus, recurrent homogeneous linear equation
solution is a combination of exponential functions,         y &#x2192;     n
=  &#x2211;  1   n     c  i     &#x03BB;  i   n        e &#x2192;     i
{\displaystyle {\vec {y}}_{n}=\sum _{1}^{n}{c_{i}\,\lambda _{i}^{n}\,{\vec
{e}}_{i}}}  [{\vec {y}}_{n}=\sum _{1}^{n}{c_{i}\,\lambda _{i}^{n}\,{\vec {e}}_
{i}}]. The components      c  i     {\displaystyle c_{i}}  [c_{i}] can be
determined out of initial conditions:
             y &#x2192;     0   =   [     y  0        y  &#x2212; 1
      &#x22EE;      y  &#x2212; n + 1      ]   =  &#x2211;  i = 1   n     c  i
      &#x03BB;  i   0        e &#x2192;     i    =   [        e &#x2192;     1
      e &#x2192;     2     &#x22EF;       e &#x2192;     n      ]      [     c
      1        c  2       &#x22EF;      c  n      ]   = E    [     c  1
      c  2       &#x22EF;      c  n      ]     {\displaystyle {\vec {y}}_{0}=
      {\begin{bmatrix}y_{0}\\y_{-1}\\\vdots \\y_{-n+1}\end{bmatrix}}=\sum _
      {i=1}^{n}{c_{i}\,\lambda _{i}^{0}\,{\vec {e}}_{i}}={\begin{bmatrix}{\vec
      {e}}_{1}&{\vec {e}}_{2}&\cdots &{\vec {e}}_{n}\end{bmatrix}}\,{\begin
      {bmatrix}c_{1}\\c_{2}\\\cdots \\c_{n}\end{bmatrix}}=E\,{\begin{bmatrix}c_
      {1}\\c_{2}\\\cdots \\c_{n}\end{bmatrix}}}  [{\vec {y}}_{0}={\begin
      {bmatrix}y_{0}\\y_{-1}\\\vdots \\y_{-n+1}\end{bmatrix}}=\sum _{i=1}^{n}
      {c_{i}\,\lambda _{i}^{0}\,{\vec {e}}_{i}}={\begin{bmatrix}{\vec {e}}_{1}&
      {\vec {e}}_{2}&\cdots &{\vec {e}}_{n}\end{bmatrix}}\,{\begin{bmatrix}c_
      {1}\\c_{2}\\\cdots \\c_{n}\end{bmatrix}}=E\,{\begin{bmatrix}c_{1}\\c_
      {2}\\\cdots \\c_{n}\end{bmatrix}}]
Solving for coefficients,
           [     c  1        c  2       &#x22EF;      c  n      ]   =  E
      &#x2212; 1       y &#x2192;     0   =    [     &#x03BB;  1   n &#x2212; 1
      &#x03BB;  2   n &#x2212; 1     &#x22EF;    &#x03BB;  n   n &#x2212; 1
      &#x22EE;   &#x22EE;   &#x22F1;   &#x22EE;      &#x03BB;  1      &#x03BB;
      2     &#x22EF;    &#x03BB;  n       1   1   &#x22EF;   1    ]    &#x2212;
      1      [     y  0        y  &#x2212; 1       &#x22EE;      y  &#x2212; n
      + 1      ]   .   {\displaystyle {\begin{bmatrix}c_{1}\\c_{2}\\\cdots \\c_
      {n}\end{bmatrix}}=E^{-1}{\vec {y}}_{0}={\begin{bmatrix}\lambda _{1}^{n-
      1}&\lambda _{2}^{n-1}&\cdots &\lambda _{n}^{n-1}\\\vdots &\vdots &\ddots
      &\vdots \\\lambda _{1}&\lambda _{2}&\cdots &\lambda _{n}\\1&1&\cdots
      &1\end{bmatrix}}^{-1}\,{\begin{bmatrix}y_{0}\\y_{-1}\\\vdots \\y_{-
      n+1}\end{bmatrix}}.}  [{\begin{bmatrix}c_{1}\\c_{2}\\\cdots \\c_{n}\end
      {bmatrix}}=E^{-1}{\vec {y}}_{0}={\begin{bmatrix}\lambda _{1}^{n-
      1}&\lambda _{2}^{n-1}&\cdots &\lambda _{n}^{n-1}\\\vdots &\vdots &\ddots
      &\vdots \\\lambda _{1}&\lambda _{2}&\cdots &\lambda _{n}\\1&1&\cdots
      &1\end{bmatrix}}^{-1}\,{\begin{bmatrix}y_{0}\\y_{-1}\\\vdots \\y_{-
      n+1}\end{bmatrix}}.]
This also works with arbitrary boundary conditions          y  a   ,  y  b   ,
&#x2026;  &#x23DF;    n     {\displaystyle \underbrace {y_{a},y_{b},\ldots } _
{\text{n}}}  [\underbrace {y_{a},y_{b},\ldots } _{\text{n}}], not necessary the
initial ones,
           [     y  a        y  b       &#x22EE;    ]   =   [        y &#x2192;
      a   [ n ]         y &#x2192;     b   [ n ]     &#x22EE;    ]   =
      [     &#x2211;  i = 1   n     c  i     &#x03BB;  i   a        e &#x2192;
      i   [ n ]       &#x2211;  i = 1   n     c  i     &#x03BB;  i   b        e
      &#x2192;     i   [ n ]      &#x22EE;    ]   =   [     &#x2211;  i = 1   n
      c  i     &#x03BB;  i   a     &#x03BB;  i   n &#x2212; 1         &#x2211;
      i = 1   n     c  i     &#x03BB;  i   b     &#x03BB;  i   n &#x2212; 1
      &#x22EE;    ]   =   {\displaystyle {\begin{bmatrix}y_{a}\\y_{b}\\\vdots
      \end{bmatrix}}={\begin{bmatrix}{\vec {y}}_{a}[n]\\{\vec {y}}_{b}
      [n]\\\vdots \end{bmatrix}}={\begin{bmatrix}\sum _{i=1}^{n}{c_{i}\,\lambda
      _{i}^{a}\,{\vec {e}}_{i}[n]}\\\sum _{i=1}^{n}{c_{i}\,\lambda _{i}^{b}\,
      {\vec {e}}_{i}[n]}\\\vdots \end{bmatrix}}={\begin{bmatrix}\sum _{i=1}^{n}
      {c_{i}\,\lambda _{i}^{a}\,\lambda _{i}^{n-1}}\\\sum _{i=1}^{n}{c_
      {i}\,\lambda _{i}^{b}\,\lambda _{i}^{n-1}}\\\vdots \end{bmatrix}}=}  [
      {\begin{bmatrix}y_{a}\\y_{b}\\\vdots \end{bmatrix}}={\begin{bmatrix}{\vec
      {y}}_{a}[n]\\{\vec {y}}_{b}[n]\\\vdots \end{bmatrix}}={\begin
      {bmatrix}\sum _{i=1}^{n}{c_{i}\,\lambda _{i}^{a}\,{\vec {e}}_{i}
      [n]}\\\sum _{i=1}^{n}{c_{i}\,\lambda _{i}^{b}\,{\vec {e}}_{i}[n]}\\\vdots
      \end{bmatrix}}={\begin{bmatrix}\sum _{i=1}^{n}{c_{i}\,\lambda _{i}^
      {a}\,\lambda _{i}^{n-1}}\\\sum _{i=1}^{n}{c_{i}\,\lambda _{i}^
      {b}\,\lambda _{i}^{n-1}}\\\vdots \end{bmatrix}}=]
         =   [    &#x2211;   c  i     &#x03BB;  i   a + n &#x2212; 1
      &#x2211;   c  i     &#x03BB;  i   b + n &#x2212; 1        &#x22EE;    ]
      =   [     &#x03BB;  1   a + n &#x2212; 1      &#x03BB;  2   a + n
      &#x2212; 1     &#x22EF;    &#x03BB;  n   a + n &#x2212; 1        &#x03BB;
      1   b + n &#x2212; 1      &#x03BB;  2   b + n &#x2212; 1     &#x22EF;
      &#x03BB;  n   b + n &#x2212; 1       &#x22EE;   &#x22EE;   &#x22F1;
      &#x22EE;    ]      [     c  1        c  2       &#x22EE;      c  n      ]
      .   {\displaystyle ={\begin{bmatrix}\sum {c_{i}\,\lambda _{i}^{a+n-
      1}}\\\sum {c_{i}\,\lambda _{i}^{b+n-1}}\\\vdots \end{bmatrix}}={\begin
      {bmatrix}\lambda _{1}^{a+n-1}&\lambda _{2}^{a+n-1}&\cdots &\lambda _{n}^
      {a+n-1}\\\lambda _{1}^{b+n-1}&\lambda _{2}^{b+n-1}&\cdots &\lambda _{n}^
      {b+n-1}\\\vdots &\vdots &\ddots &\vdots \end{bmatrix}}\,{\begin
      {bmatrix}c_{1}\\c_{2}\\\vdots \\c_{n}\end{bmatrix}}.}  [={\begin
      {bmatrix}\sum {c_{i}\,\lambda _{i}^{a+n-1}}\\\sum {c_{i}\,\lambda _{i}^
      {b+n-1}}\\\vdots \end{bmatrix}}={\begin{bmatrix}\lambda _{1}^{a+n-
      1}&\lambda _{2}^{a+n-1}&\cdots &\lambda _{n}^{a+n-1}\\\lambda _{1}^{b+n-
      1}&\lambda _{2}^{b+n-1}&\cdots &\lambda _{n}^{b+n-1}\\\vdots &\vdots
      &\ddots &\vdots \end{bmatrix}}\,{\begin{bmatrix}c_{1}\\c_{2}\\\vdots \\c_
      {n}\end{bmatrix}}.]
This description is really no different from general method above, however it
is more succinct. It also works nicely for situations like
           {     a  n   =  a  n &#x2212; 1   &#x2212;  b  n &#x2212; 1        b
      n   = 2  a  n &#x2212; 1   +  b  n &#x2212; 1   .         {\displaystyle
      {\begin{cases}a_{n}=a_{n-1}-b_{n-1}\\b_{n}=2a_{n-1}+b_{n-1}.\end{cases}}}
      [{\begin{cases}a_{n}=a_{n-1}-b_{n-1}\\b_{n}=2a_{n-1}+b_{n-1}.\end
      {cases}}]
where there are several linked recurrences.[6]
*** Solving with z-transforms[edit] ***
Certain difference equations - in particular, linear_constant_coefficient
difference equations - can be solved using z-transforms. The z-transforms are a
class of integral_transforms that lead to more convenient algebraic
manipulations and more straightforward solutions. There are cases in which
obtaining a direct solution would be all but impossible, yet solving the
problem via a thoughtfully chosen integral transform is straightforward.
**** Solving non-homogeneous linear recurrence relations with constant
coefficients[edit] ****
If the recurrence is non-homogeneous, a particular solution can be found by the
method_of_undetermined_coefficients and the solution is the sum of the solution
of the homogeneous and the particular solutions. Another method to solve a non-
homogeneous recurrence is the method of symbolic differentiation. For example,
consider the following recurrence:
          a  n + 1   =  a  n   + 1   {\displaystyle a_{n+1}=a_{n}+1}  [a_
      {n+1}=a_{n}+1]
This is a non-homogeneous recurrence. If we substitute n â¦ n+1, we obtain the
recurrence
          a  n + 2   =  a  n + 1   + 1   {\displaystyle a_{n+2}=a_{n+1}+1}  [a_
      {n+2}=a_{n+1}+1]
Subtracting the original recurrence from this equation yields
          a  n + 2   &#x2212;  a  n + 1   =  a  n + 1   &#x2212;  a  n
      {\displaystyle a_{n+2}-a_{n+1}=a_{n+1}-a_{n}}  [{\displaystyle a_{n+2}-a_
      {n+1}=a_{n+1}-a_{n}}]
or equivalently
          a  n + 2   = 2  a  n + 1   &#x2212;  a  n     {\displaystyle a_
      {n+2}=2a_{n+1}-a_{n}}  [a_{n+2}=2a_{n+1}-a_{n}]
This is a homogeneous recurrence, which can be solved by the methods explained
above. In general, if a linear recurrence has the form
          a  n + k   =  &#x03BB;  k &#x2212; 1    a  n + k &#x2212; 1   +
      &#x03BB;  k &#x2212; 2    a  n + k &#x2212; 2   + &#x22EF; +  &#x03BB;  1
      a  n + 1   +  &#x03BB;  0    a  n   + p ( n )   {\displaystyle a_
      {n+k}=\lambda _{k-1}a_{n+k-1}+\lambda _{k-2}a_{n+k-2}+\cdots +\lambda _
      {1}a_{n+1}+\lambda _{0}a_{n}+p(n)}  [a_{n+k}=\lambda _{k-1}a_{n+k-
      1}+\lambda _{k-2}a_{n+k-2}+\cdots +\lambda _{1}a_{n+1}+\lambda _{0}a_
      {n}+p(n)]
where      &#x03BB;  0   ,  &#x03BB;  1   , &#x2026; ,  &#x03BB;  k &#x2212; 1
{\displaystyle \lambda _{0},\lambda _{1},\dots ,\lambda _{k-1}}  [\lambda _
{0},\lambda _{1},\dots ,\lambda _{k-1}] are constant coefficients and p(n) is
the inhomogeneity, then if p(n) is a polynomial with degree r, then this non-
homogeneous recurrence can be reduced to a homogeneous recurrence by applying
the method of symbolic differencing r times.
If
         P ( x ) =  &#x2211;  n = 0   &#x221E;    p  n    x  n
      {\displaystyle P(x)=\sum _{n=0}^{\infty }p_{n}x^{n}}  [P(x)=\sum _{n=0}^
      {\infty }p_{n}x^{n}]
is the generating function of the inhomogeneity, the generating function
         A ( x ) =  &#x2211;  n = 0   &#x221E;   a ( n )  x  n
      {\displaystyle A(x)=\sum _{n=0}^{\infty }a(n)x^{n}}  [A(x)=\sum _{n=0}^
      {\infty }a(n)x^{n}]
of the non-homogeneous recurrence
          a  n   =  &#x2211;  i = 1   s    c  i    a  n &#x2212; i   +  p  n
      ,  n &#x2265;  n  r   ,   {\displaystyle a_{n}=\sum _{i=1}^{s}c_{i}a_{n-
      i}+p_{n},\quad n\geq n_{r},}  [a_{n}=\sum _{i=1}^{s}c_{i}a_{n-i}+p_
      {n},\quad n\geq n_{r},]
with constant coefficients ci is derived from
          (  1 &#x2212;  &#x2211;  i = 1   s    c  i    x  i    )  A ( x ) = P
      ( x ) +  &#x2211;  n = 0    n  r   &#x2212; 1   [  a  n   &#x2212;  p  n
      ]  x  n   &#x2212;  &#x2211;  i = 1   s    c  i    x  i    &#x2211;  n =
      0    n  r   &#x2212; i &#x2212; 1    a  n    x  n   .   {\displaystyle
      \left(1-\sum _{i=1}^{s}c_{i}x^{i}\right)A(x)=P(x)+\sum _{n=0}^{n_{r}-1}
      [a_{n}-p_{n}]x^{n}-\sum _{i=1}^{s}c_{i}x^{i}\sum _{n=0}^{n_{r}-i-1}a_
      {n}x^{n}.}  [\left(1-\sum _{i=1}^{s}c_{i}x^{i}\right)A(x)=P(x)+\sum _
      {n=0}^{n_{r}-1}[a_{n}-p_{n}]x^{n}-\sum _{i=1}^{s}c_{i}x^{i}\sum _{n=0}^
      {n_{r}-i-1}a_{n}x^{n}.]
If P(x) is a rational generating function, A(x) is also one. The case discussed
above, where pn = K is a constant, emerges as one example of this formula, with
P(x) = K/(1âx). Another example, the recurrence      a  n   = 10  a  n
&#x2212; 1   + n   {\displaystyle a_{n}=10a_{n-1}+n}  [a_{n}=10a_{n-1}+n] with
linear inhomogeneity, arises in the definition of the schizophrenic_numbers.
The solution of homogeneous recurrences is incorporated as p = P = 0.
**** Solving first-order non-homogeneous recurrence relations with variable
coefficients[edit] ****
Moreover, for the general first-order non-homogeneous linear recurrence
relation with variable coefficients:
          a  n + 1   =  f  n    a  n   +  g  n   ,   f  n   &#x2260; 0 ,
      {\displaystyle a_{n+1}=f_{n}a_{n}+g_{n},\qquad f_{n}\neq 0,}  [a_{n+1}=f_
      {n}a_{n}+g_{n},\qquad f_{n}\neq 0,]
there is also a nice method to solve it:[7]
          a  n + 1   &#x2212;  f  n    a  n   =  g  n     {\displaystyle a_
      {n+1}-f_{n}a_{n}=g_{n}}  [a_{n+1}-f_{n}a_{n}=g_{n}]
            a  n + 1     &#x220F;  k = 0   n    f  k      &#x2212;     f  n
      a  n      &#x220F;  k = 0   n    f  k      =    g  n     &#x220F;  k = 0
      n    f  k        {\displaystyle {\frac {a_{n+1}}{\prod _{k=0}^{n}f_{k}}}-
      {\frac {f_{n}a_{n}}{\prod _{k=0}^{n}f_{k}}}={\frac {g_{n}}{\prod _{k=0}^
      {n}f_{k}}}}  [{\frac {a_{n+1}}{\prod _{k=0}^{n}f_{k}}}-{\frac {f_{n}a_
      {n}}{\prod _{k=0}^{n}f_{k}}}={\frac {g_{n}}{\prod _{k=0}^{n}f_{k}}}]
            a  n + 1     &#x220F;  k = 0   n    f  k      &#x2212;    a  n
      &#x220F;  k = 0   n &#x2212; 1    f  k      =    g  n     &#x220F;  k = 0
      n    f  k        {\displaystyle {\frac {a_{n+1}}{\prod _{k=0}^{n}f_{k}}}-
      {\frac {a_{n}}{\prod _{k=0}^{n-1}f_{k}}}={\frac {g_{n}}{\prod _{k=0}^
      {n}f_{k}}}}  [{\frac {a_{n+1}}{\prod _{k=0}^{n}f_{k}}}-{\frac {a_{n}}
      {\prod _{k=0}^{n-1}f_{k}}}={\frac {g_{n}}{\prod _{k=0}^{n}f_{k}}}]
Let
          A  n   =    a  n     &#x220F;  k = 0   n &#x2212; 1    f  k      ,
      {\displaystyle A_{n}={\frac {a_{n}}{\prod _{k=0}^{n-1}f_{k}}},}  [A_{n}=
      {\frac {a_{n}}{\prod _{k=0}^{n-1}f_{k}}},]
Then
          A  n + 1   &#x2212;  A  n   =    g  n     &#x220F;  k = 0   n    f  k
      {\displaystyle A_{n+1}-A_{n}={\frac {g_{n}}{\prod _{k=0}^{n}f_{k}}}}  [A_
      {n+1}-A_{n}={\frac {g_{n}}{\prod _{k=0}^{n}f_{k}}}]
          &#x2211;  m = 0   n &#x2212; 1   (  A  m + 1   &#x2212;  A  m   ) =
      A  n   &#x2212;  A  0   =  &#x2211;  m = 0   n &#x2212; 1      g  m
      &#x220F;  k = 0   m    f  k        {\displaystyle \sum _{m=0}^{n-1}(A_
      {m+1}-A_{m})=A_{n}-A_{0}=\sum _{m=0}^{n-1}{\frac {g_{m}}{\prod _{k=0}^
      {m}f_{k}}}}  [\sum _{m=0}^{n-1}(A_{m+1}-A_{m})=A_{n}-A_{0}=\sum _{m=0}^
      {n-1}{\frac {g_{m}}{\prod _{k=0}^{m}f_{k}}}]
            a  n     &#x220F;  k = 0   n &#x2212; 1    f  k      =  A  0   +
      &#x2211;  m = 0   n &#x2212; 1      g  m     &#x220F;  k = 0   m    f  k
      {\displaystyle {\frac {a_{n}}{\prod _{k=0}^{n-1}f_{k}}}=A_{0}+\sum _
      {m=0}^{n-1}{\frac {g_{m}}{\prod _{k=0}^{m}f_{k}}}}  [{\frac {a_{n}}{\prod
      _{k=0}^{n-1}f_{k}}}=A_{0}+\sum _{m=0}^{n-1}{\frac {g_{m}}{\prod _{k=0}^
      {m}f_{k}}}]
          a  n   =  (   &#x220F;  k = 0   n &#x2212; 1    f  k    )   (   A  0
      +  &#x2211;  m = 0   n &#x2212; 1      g  m     &#x220F;  k = 0   m    f
      k       )    {\displaystyle a_{n}=\left(\prod _{k=0}^{n-1}f_
      {k}\right)\left(A_{0}+\sum _{m=0}^{n-1}{\frac {g_{m}}{\prod _{k=0}^{m}f_
      {k}}}\right)}  [a_{n}=\left(\prod _{k=0}^{n-1}f_{k}\right)\left(A_
      {0}+\sum _{m=0}^{n-1}{\frac {g_{m}}{\prod _{k=0}^{m}f_{k}}}\right)]
If we apply the formula to      a  n + 1   = ( 1 + h  f  n h   )  a  n   + h  g
n h     {\displaystyle a_{n+1}=(1+hf_{nh})a_{n}+hg_{nh}}  [{\displaystyle a_
{n+1}=(1+hf_{nh})a_{n}+hg_{nh}}] and take the limit hâ0, we get the formula
for first order linear_differential_equations with variable coefficients; the
sum becomes an integral, and the product becomes the exponential function of an
integral.
**** Solving general homogeneous linear recurrence relations[edit] ****
Many homogeneous linear recurrence relations may be solved by means of the
generalized_hypergeometric_series. Special cases of these lead to recurrence
relations for the orthogonal_polynomials, and many special_functions. For
example, the solution to
          J  n + 1   =    2 n  z    J  n   &#x2212;  J  n &#x2212; 1
      {\displaystyle J_{n+1}={\frac {2n}{z}}J_{n}-J_{n-1}}  [J_{n+1}={\frac
      {2n}{z}}J_{n}-J_{n-1}]
is given by
          J  n   =  J  n   ( z ) ,   {\displaystyle J_{n}=J_{n}(z),}  [
      {\displaystyle J_{n}=J_{n}(z),}]
the Bessel_function, while
         ( b &#x2212; n )  M  n &#x2212; 1   + ( 2 n &#x2212; b &#x2212; z )  M
      n   &#x2212; n  M  n + 1   = 0   {\displaystyle (b-n)M_{n-1}+(2n-b-z)M_
      {n}-nM_{n+1}=0}  [{\displaystyle (b-n)M_{n-1}+(2n-b-z)M_{n}-nM_{n+1}=0}]
is solved by
          M  n   = M ( n , b ; z )   {\displaystyle M_{n}=M(n,b;z)}  [
      {\displaystyle M_{n}=M(n,b;z)}]
the confluent_hypergeometric_series. Sequences which are the solutions of
linear_difference_equations_with_polynomial_coefficients are called P-
recursive. For these specific recurrence equations algorithms are known which
find polynomial, rational or hypergeometric solutions.
**** Solving first-order rational difference equations[edit] ****
Main article: Rational_difference_equation
A first order rational difference equation has the form      w  t + 1   =     a
w  t   + b   c  w  t   + d       {\displaystyle w_{t+1}={\tfrac {aw_{t}+b}{cw_
{t}+d}}}  [w_{t+1}={\tfrac {aw_{t}+b}{cw_{t}+d}}]. Such an equation can be
solved by writing      w  t     {\displaystyle w_{t}}  [w_{t}] as a nonlinear
transformation of another variable      x  t     {\displaystyle x_{t}}  [x_{t}]
which itself evolves linearly. Then standard methods can be used to solve the
linear difference equation in      x  t     {\displaystyle x_{t}}  [x_{t}].
***** Stability[edit] *****
**** Stability of linear higher-order recurrences[edit] ****
The linear recurrence of order d,
          a  n   =  c  1    a  n &#x2212; 1   +  c  2    a  n &#x2212; 2   +
      &#x22EF; +  c  d    a  n &#x2212; d   ,   {\displaystyle a_{n}=c_{1}a_{n-
      1}+c_{2}a_{n-2}+\cdots +c_{d}a_{n-d},}  [{\displaystyle a_{n}=c_{1}a_{n-
      1}+c_{2}a_{n-2}+\cdots +c_{d}a_{n-d},}]
has the characteristic_equation
          &#x03BB;  d   &#x2212;  c  1    &#x03BB;  d &#x2212; 1   &#x2212;  c
      2    &#x03BB;  d &#x2212; 2   &#x2212; &#x22EF; &#x2212;  c  d
      &#x03BB;  0   = 0.   {\displaystyle \lambda ^{d}-c_{1}\lambda ^{d-1}-c_
      {2}\lambda ^{d-2}-\cdots -c_{d}\lambda ^{0}=0.}  [{\displaystyle \lambda
      ^{d}-c_{1}\lambda ^{d-1}-c_{2}\lambda ^{d-2}-\cdots -c_{d}\lambda ^
      {0}=0.}]
The recurrence is stable, meaning that the iterates converge asymptotically to
a fixed value, if and only if the eigenvalues (i.e., the roots of the
characteristic equation), whether real or complex, are all less than unity in
absolute value.
**** Stability of linear first-order matrix recurrences[edit] ****
Main article: Matrix_difference_equation
In the first-order matrix difference equation
         [  x  t   &#x2212;  x  &#x2217;   ] = A [  x  t &#x2212; 1   &#x2212;
      x  &#x2217;   ]   {\displaystyle [x_{t}-x^{*}]=A[x_{t-1}-x^{*}]}  [
      {\displaystyle [x_{t}-x^{*}]=A[x_{t-1}-x^{*}]}]
with state vector x and transition matrix A, x converges asymptotically to the
steady state vector x* if and only if all eigenvalues of the transition matrix
A (whether real or complex) have an absolute_value which is less than 1.
**** Stability of nonlinear first-order recurrences[edit] ****
Consider the nonlinear first-order recurrence
          x  n   = f (  x  n &#x2212; 1   ) .   {\displaystyle x_{n}=f(x_{n-
      1}).}  [x_{n}=f(x_{n-1}).]
This recurrence is locally_stable, meaning that it converges to a fixed point
x* from points sufficiently close to x*, if the slope of f in the neighborhood
of x* is smaller than unity in absolute value: that is,
          |   f &#x2032;  (  x  &#x2217;   )  |  < 1.   {\displaystyle |f'(x^
      {*})|<1.}  [{\displaystyle |f'(x^{*})|<1.}]
A nonlinear recurrence could have multiple fixed points, in which case some
fixed points may be locally stable and others locally unstable; for continuous
f two adjacent fixed points cannot both be locally stable.
A nonlinear recurrence relation could also have a cycle of period k for k > 1.
Such a cycle is stable, meaning that it attracts a set of initial conditions of
positive measure, if the composite function
         g ( x ) := f &#x2218; f &#x2218; &#x22EF; &#x2218; f ( x )
      {\displaystyle g(x):=f\circ f\circ \cdots \circ f(x)}  [{\displaystyle g
      (x):=f\circ f\circ \cdots \circ f(x)}]
with f appearing k times is locally stable according to the same criterion:
          |   g &#x2032;  (  x  &#x2217;   )  |  < 1 ,   {\displaystyle |g'(x^
      {*})|<1,}  [|g'(x^{*})|<1,]
where x* is any point on the cycle.
In a chaotic recurrence relation, the variable x stays in a bounded region but
never converges to a fixed point or an attracting cycle; any fixed points or
cycles of the equation are unstable. See also logistic_map, dyadic
transformation, and tent_map.
***** Relationship to differential equations[edit] *****
When solving an ordinary_differential_equation numerically, one typically
encounters a recurrence relation. For example, when solving the initial_value
problem
          y &#x2032;  ( t ) = f ( t , y ( t ) ) , &#xA0; &#xA0; y (  t  0   ) =
      y  0   ,   {\displaystyle y'(t)=f(t,y(t)),\ \ y(t_{0})=y_{0},}  [y'(t)=f
      (t,y(t)),\ \ y(t_{0})=y_{0},]
with Euler's_method and a step size h, one calculates the values
          y  0   = y (  t  0   ) , &#xA0; &#xA0;  y  1   = y (  t  0   + h ) ,
      &#xA0; &#xA0;  y  2   = y (  t  0   + 2 h ) , &#xA0; &#x2026;
      {\displaystyle y_{0}=y(t_{0}),\ \ y_{1}=y(t_{0}+h),\ \ y_{2}=y(t_
      {0}+2h),\ \dots }  [y_{0}=y(t_{0}),\ \ y_{1}=y(t_{0}+h),\ \ y_{2}=y(t_
      {0}+2h),\ \dots ]
by the recurrence
           y  n + 1   =  y  n   + h f (  t  n   ,  y  n   ) ,  t  n   =  t  0
      + n h   {\displaystyle \,y_{n+1}=y_{n}+hf(t_{n},y_{n}),t_{n}=t_{0}+nh}  [
      {\displaystyle \,y_{n+1}=y_{n}+hf(t_{n},y_{n}),t_{n}=t_{0}+nh}]
Systems of linear first order differential equations can be discretized exactly
analytically using the methods shown in the discretization article.
***** Applications[edit] *****
**** Biology[edit] ****
Some of the best-known difference equations have their origins in the attempt
to model population dynamics. For example, the Fibonacci_numbers were once used
as a model for the growth of a rabbit population.
The logistic_map is used either directly to model population growth, or as a
starting point for more detailed models of population_dynamics. In this
context, coupled difference equations are often used to model the interaction
of two or more populations. For example, the Nicholson-Bailey model for a host-
parasite interaction is given by
          N  t + 1   = &#x03BB;  N  t    e  &#x2212; a  P  t
      {\displaystyle N_{t+1}=\lambda N_{t}e^{-aP_{t}}}  [{\displaystyle N_
      {t+1}=\lambda N_{t}e^{-aP_{t}}}]
          P  t + 1   =  N  t   ( 1 &#x2212;  e  &#x2212; a  P  t     ) ,
      {\displaystyle P_{t+1}=N_{t}(1-e^{-aP_{t}}),}  [{\displaystyle P_{t+1}=N_
      {t}(1-e^{-aP_{t}}),}]
with Nt representing the hosts, and Pt the parasites, at time t.
Integrodifference_equations are a form of recurrence relation important to
spatial ecology. These and other difference equations are particularly suited
to modeling univoltine populations.
**** Computer science[edit] ****
Recurrence relations are also of fundamental importance in analysis_of
algorithms.[8][9] If an algorithm is designed so that it will break a problem
into smaller subproblems (divide_and_conquer), its running time is described by
a recurrence relation.
A simple example is the time an algorithm takes to find an element in an
ordered vector with     n   {\displaystyle n}  [n] elements, in the worst case.
A naive algorithm will search from left to right, one element at a time. The
worst possible scenario is when the required element is the last, so the number
of comparisons is     n   {\displaystyle n}  [n].
A better algorithm is called binary_search. However, it requires a sorted
vector. It will first check if the element is at the middle of the vector. If
not, then it will check if the middle element is greater or lesser than the
sought element. At this point, half of the vector can be discarded, and the
algorithm can be run again on the other half. The number of comparisons will be
given by
          c  1   = 1   {\displaystyle c_{1}=1}  [c_{1}=1]
          c  n   = 1 +  c  n  /  2     {\displaystyle c_{n}=1+c_{n/2}}  [c_
      {n}=1+c_{n/2}]
the time_complexity of which will be     O (  log  2   &#x2061; ( n ) )
{\displaystyle O(\log _{2}(n))}  [{\displaystyle O(\log _{2}(n))}].
**** Digital signal processing[edit] ****
In digital_signal_processing, recurrence relations can model feedback in a
system, where outputs at one time become inputs for future time. They thus
arise in infinite_impulse_response (IIR) digital_filters.
For example, the equation for a "feedforward" IIR comb_filter of delay T is:
          y  t   = ( 1 &#x2212; &#x03B1; )  x  t   + &#x03B1;  y  t &#x2212; T
      {\displaystyle y_{t}=(1-\alpha )x_{t}+\alpha y_{t-T}}  [y_{t}=(1-\alpha
      )x_{t}+\alpha y_{t-T}]
Where      x  t     {\displaystyle x_{t}}  [x_{t}] is the input at time t,
y  t     {\displaystyle y_{t}}  [y_{t}] is the output at time t, and Î±
controls how much of the delayed signal is fed back into the output. From this
we can see that
          y  t   = ( 1 &#x2212; &#x03B1; )  x  t   + &#x03B1; ( ( 1 &#x2212;
      &#x03B1; )  x  t &#x2212; T   + &#x03B1;  y  t &#x2212; 2 T   )
      {\displaystyle y_{t}=(1-\alpha )x_{t}+\alpha ((1-\alpha )x_{t-T}+\alpha
      y_{t-2T})}  [y_{t}=(1-\alpha )x_{t}+\alpha ((1-\alpha )x_{t-T}+\alpha y_
      {t-2T})]
          y  t   = ( 1 &#x2212; &#x03B1; )  x  t   + ( &#x03B1; &#x2212;
      &#x03B1;  2   )  x  t &#x2212; T   +  &#x03B1;  2    y  t &#x2212; 2 T
      )   {\displaystyle y_{t}=(1-\alpha )x_{t}+(\alpha -\alpha ^{2})x_{t-
      T}+\alpha ^{2}y_{t-2T})}  [y_{t}=(1-\alpha )x_{t}+(\alpha -\alpha ^{2})x_
      {t-T}+\alpha ^{2}y_{t-2T})]
etc.
**** Economics[edit] ****
Recurrence relations, especially linear recurrence relations, are used
extensively in both theoretical and empirical economics.[10][11] In particular,
in macroeconomics one might develop a model of various broad sectors of the
economy (the financial sector, the goods sector, the labor market, etc.) in
which some agents' actions depend on lagged variables. The model would then be
solved for current values of key variables (interest rate, real GDP, etc.) in
terms of exogenous_variables and lagged endogenous variables. See also time
series_analysis.
***** See also[edit] *****
    * Holonomic_sequences
    * Iterated_function
    * Orthogonal_polynomials
    * Recursion
    * Recursion_(computer_science)
    * Lagged_Fibonacci_generator
    * Master_theorem_(analysis_of_algorithms)
    * Circle_points_segments_proof
    * Continued_fraction
    * Time_scale_calculus
    * Integrodifference_equation
    * Combinatorial_principles
    * Infinite_impulse_response
    * Multiplicative_calculus
    * Integration_by_reduction_formulae
    * Mathematical_induction
***** Notes[edit] *****
   1. ^ Jacobson, Nathan , Basic Algebra 2 (2nd ed.), Â§ 0.4. pg 16.
   2. ^ Partial_difference_equations, Sui Sun Cheng, CRC Press, 2003,
   3. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   4. ISBN 978-0-415-29884-1
   5. ^Greene, Daniel H.; Knuth,_Donald_E. (1982), "2.1.1 Constant coefficients
      â A) Homogeneous equations", Mathematics for the Analysis of Algorithms
      (2nd ed.), BirkhÃ¤user, p. 17
   6. .
   7. ^ Chiang, Alpha C., Fundamental Methods of Mathematical Economics, third
      edition, McGraw-Hill, 1984.
   8. ^ Papanicolaou, Vassilis, "On the asymptotic stability of a class of
      linear difference equations," Mathematics Magazine 69(1), February 1996,
      34–43.
   9. ^Maurer, Stephen B.; Ralston, Anthony (1998), Discrete Algorithmic
      Mathematics (2nd ed.), A K Peters, p. 609, ISBN 9781568810911
  10. .
  11. ^"Archived_copy" (PDF). Archived (PDF) from the original on 2010-07-05.
      Retrieved 2010-10-19.CS1 maint: Archived copy as title (link)
  12. ^ Cormen, T. et al, Introduction to Algorithms, MIT Press, 2009
  13. ^ R. Sedgewick, F. Flajolet, An Introduction to the Analysis of
      Algorithms, Addison-Wesley, 2013
  14. ^Stokey,_Nancy_L.; Lucas,_Robert_E.,_Jr.; Prescott,_Edward_C. (1989).
      Recursive_Methods_in_Economic_Dynamics. Cambridge: Harvard University
      Press. ISBN 0-674-75096-9.
  15. ^Ljungqvist,_Lars; Sargent,_Thomas_J. (2004). Recursive_Macroeconomic
      Theory (Second ed.). Cambridge: MIT Press. ISBN 0-262-12274-X.
***** References[edit] *****
    * Batchelder, Paul M. (1967). An introduction to linear difference
      equations. Dover Publications.
Miller, Kenneth S. (1968). Linear difference equations. W. A. Benjamin.
Fillmore, Jay P.; Marx, Morris L. (1968). "Linear recursive sequences". SIAM
Rev. 10 (3). pp. 324â353. JSTOR 2027658.
Brousseau, Alfred (1971). Linear_Recursion_and_Fibonacci_Sequences. Fibonacci
Association.
Thomas_H._Cormen, Charles_E._Leiserson, Ronald_L._Rivest, and Clifford_Stein.
Introduction_to_Algorithms, Second Edition. MIT Press and McGraw-Hill, 1990.
ISBN 0-262-03293-7. Chapter 4: Recurrences, pp. 62â90.
Graham, Ronald L.; Knuth, Donald E.; Patashnik, Oren (1994). Concrete
Mathematics: A Foundation for Computer Science (2 ed.). Addison-Welsey. ISBN 0-
201-55802-5.
Enders, Walter (2010). Applied_Econometric_Times_Series (3 ed.). Archived from
the_original on 2014-11-10.
Cull, Paul; Flahive,_Mary; Robson, Robbie (2005). Difference Equations: From
Rabbits to Chaos. Springer. ISBN 0-387-23234-6.
 chapter 7.
Jacques, Ian (2006). Mathematics for Economics and Business (Fifth ed.).
Prentice Hall. pp. 551â568. ISBN 0-273-70195-9.
 Chapter 9.1: Difference Equations.
Minh, Tang; Van To, Tan (2006). "Using_generating_functions_to_solve_linear
inhomogeneous_recurrence_equations" (PDF). Proc. Int. Conf. Simulation,
Modelling and Optimization, SMO'06. pp. 399â404.
Polyanin, Andrei D. "Difference_and_Functional_Equations:_Exact_Solutions".
 at EqWorld - The World of Mathematical Equations.
Polyanin, Andrei D. "Difference_and_Functional_Equations:_Methods".
 at EqWorld - The World of Mathematical Equations.
Wang, Xiang-Sheng; Wong, Roderick (2012). "Asymptotics of orthogonal
polynomials via recurrence relations". Anal. Appl. 10 (2): 215â235. arXiv:
1101.4371. doi:10.1142/S0219530512500108.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Recurrence_relation",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Weisstein,_Eric_W. "Recurrence_Equation". MathWorld.
"OEIS_Index_Rec".
 OEIS index to a few thousand examples of linear recurrences, sorted by order
(number of terms) and signature (vector of values of the constant coefficients)
Authority_control [Edit_this_at_Wikidata]     * GND: 4012264-5

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Recurrence_relation&oldid=909503613"
Categories:
    * Algebra
    * Recurrence_relations
    * Combinatorics
Hidden categories:
    * CS1_maint:_Archived_copy_as_title
    * Articles_with_short_description
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * á áá­á
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 5 August 2019, at 21:02 (UTC).
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
