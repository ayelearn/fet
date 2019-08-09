The following text has been accessed from https://en.wikipedia.org/wiki/Linear_differential_equation at Fri Aug 9 03:11:04 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Linear differential equation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, a linear differential equation is a differential_equation that
is defined by a linear_polynomial in the unknown function and its derivatives,
that is an equation of the form
          a  0   ( x ) y +  a  1   ( x )  y &#x2032;  +  a  2   ( x )  y
      &#x2033;  + &#x22EF; +  a  n   ( x )  y  ( n )   + b ( x ) = 0 ,
      {\displaystyle a_{0}(x)y+a_{1}(x)y'+a_{2}(x)y''+\cdots +a_{n}(x)y^{(n)}+b
      (x)=0,}  [{\displaystyle a_{0}(x)y+a_{1}(x)y'+a_{2}(x)y''+\cdots +a_{n}
      (x)y^{(n)}+b(x)=0,}]
where      a  0   ( x )   {\displaystyle a_{0}(x)}  [{\displaystyle a_{0}(x)}],
...,      a  n   ( x )   {\displaystyle a_{n}(x)}  [{\displaystyle a_{n}(x)}]
and     b ( x )   {\displaystyle b(x)}  [b(x)] are arbitrary differentiable
functions that do not need to be linear, and      y &#x2032;  , &#x2026; ,  y
( n )     {\displaystyle y',\ldots ,y^{(n)}}  [{\displaystyle y',\ldots ,y^{
(n)}}] are the successive derivatives of an unknown function y of the variable
x.
This is an ordinary_differential_equation (ODE). A linear differential equation
may also be a linear_partial_differential_equation (PDE), if the unknown
function depends on several variables, and the derivatives that appear in the
equation are partial_derivatives. In this article, only ordinary differential
equations are considered.
A linear differential equation or a system of linear equations such that the
associated homogeneous equations have constant coefficients may be solved by
quadrature_(mathematics), which means that the solutions may be expressed in
terms of integrals. This is also true for a linear equation of order one, with
non-constant coefficients. An equation of order two or higher with non-constant
coefficients cannot, in general, be solved by quadrature. For order two,
Kovacic's_algorithm allows deciding whether there are solutions in terms of
integrals, and computing them if any.
The solutions of linear differential equations with polynomial coefficients are
called holonomic_functions. This class of functions is stable under sums,
products, differentiation, integration, and contains many usual functions and
special_functions such as exponential_function, logarithm, sine, cosine,
inverse_trigonometric_functions, error_function, Bessel_functions and
hypergeometric_functions. Their representation by the defining differential
equation and initial conditions allows making algorithmic (on these functions)
most operations of calculus, such as computation of antiderivatives, limits,
asymptotic_expansion, and numerical evaluation to any precision, with a
certified error bound.
⁰
***** Contents *****
    * 1_Basic_terminology
    * 2_Linear_differential_operator
    * 3_Homogeneous_equation_with_constant_coefficients
          o 3.1_Second-order_case
    * 4_Non-homogeneous_equation_with_constant_coefficients
    * 5_First-order_equation_with_variable_coefficients
    * 6_System_of_linear_differential_equations
    * 7_Higher_order_with_variable_coefficients
          o 7.1_CauchyâEuler_equation
    * 8_Holonomic_functions
    * 9_See_also
    * 10_References
    * 11_External_links
***** Basic terminology[edit] *****
The highest order_of_derivation that appears in a differentiable equation is
the order of the equation. The term b(x), which does not depend on the unknown
function and its derivatives, is sometimes called the constant term of the
equation (by analogy with algebraic_equations), even when this term is a non-
constant function. If the constant term is the zero_function, then the
differential equation is said to be homogeneous, as it is a homogeneous
polynomial in the unknown function and its derivatives. The equation obtained
by replacing, in a linear differential equation, the constant term by the zero
function is the associated homogeneous equation. A differential equation has
constant coefficients if only constant_functions appear as coefficients in the
associated homogeneous equation.
A solution of a differential equation is a function that satisfies the
equation. The solutions of a homogeneous linear differential equation form a
vector_space. In the ordinary case, this vector space has a finite dimension,
equal to the order of the equation. All solutions of a linear differential
equation are found by adding to a particular solution any solution of the
associated homogeneous equation.
***** Linear differential operator[edit] *****
Main article: Differential_operator
A basic differential operator of order i is a mapping that maps any
differentiable_function to its ith_derivative, or, in the case of several
variables, to one of its partial_derivatives of order i. It is commonly denoted
            d  i    d  x  i        {\displaystyle {\frac {d^{i}}{dx^{i}}}}  [
      {\displaystyle {\frac {d^{i}}{dx^{i}}}}]
in the case of univariate functions, and
            &#x2202;   i  1   + &#x22EF; +  i  n      &#x2202;  x  1    i  1
      &#x22EF; &#x2202;  x  n    i  n          {\displaystyle {\frac {\partial
      ^{i_{1}+\cdots +i_{n}}}{\partial x_{1}^{i_{1}}\cdots \partial x_{n}^{i_
      {n}}}}}  [{\displaystyle {\frac {\partial ^{i_{1}+\cdots +i_{n}}}
      {\partial x_{1}^{i_{1}}\cdots \partial x_{n}^{i_{n}}}}}]
in the case of functions of n variables. The basic differential operators
include the derivative of order 0, which is the identity mapping.
A linear differential operator (abbreviated, in this article, as linear
operator or, simply, operator) is a linear_combination of basic differential
operators, with differentiable functions as coefficients. In the univariate
case, a linear operator has thus the form[1]
          a  0   ( x ) +  a  1   ( x )   d  d x    + &#x22EF; +  a  n   ( x )
      d  n    d  x  n      ,   {\displaystyle a_{0}(x)+a_{1}(x){\frac {d}
      {dx}}+\cdots +a_{n}(x){\frac {d^{n}}{dx^{n}}},}  [{\displaystyle a_{0}
      (x)+a_{1}(x){\frac {d}{dx}}+\cdots +a_{n}(x){\frac {d^{n}}{dx^{n}}},}]
where      a  0   ( x ) , &#x2026; ,  a  n   ( x )   {\displaystyle a_{0}
(x),\ldots ,a_{n}(x)}  [{\displaystyle a_{0}(x),\ldots ,a_{n}(x)}] are
differentiable functions, and the nonnegative integer n is the order of the
operator (if      a  n   ( x )   {\displaystyle a_{n}(x)}  [{\displaystyle a_
{n}(x)}] is not the zero_function).
Let L be a linear differential operator. The application of L to a function f
is usually denoted Lf or Lf(X), if one needs to specify the variable (this must
not be confused with a multiplication). A linear differential operator is a
linear_operator, since it maps sums to sums and the product by a scalar to the
product by the same scalar.
As the sum of two linear operators is a linear operator, as well as the product
(on the left) of a linear operator by a differentiable function, the linear
differential operators form a vector_space over the real_numbers or the complex
numbers (depending on the nature of the functions that are considered). They
form also a free_module over the ring of differentiable functions.
The language of operators allows a compact writing for differentiable
equations: if
         L =  a  0   ( x ) +  a  1   ( x )   d  d x    + &#x22EF; +  a  n   ( x
      )    d  n    d  x  n      ,   {\displaystyle L=a_{0}(x)+a_{1}(x){\frac
      {d}{dx}}+\cdots +a_{n}(x){\frac {d^{n}}{dx^{n}}},}  [{\displaystyle L=a_
      {0}(x)+a_{1}(x){\frac {d}{dx}}+\cdots +a_{n}(x){\frac {d^{n}}{dx^{n}}},}]
is a linear differential operator, then the equation
          a  0   ( x ) y +  a  1   ( x )  y &#x2032;  +  a  2   ( x )  y
      &#x2033;  + &#x22EF; +  a  n   ( x )  y  ( n )   = b ( x )
      {\displaystyle a_{0}(x)y+a_{1}(x)y'+a_{2}(x)y''+\cdots +a_{n}(x)y^{(n)}=b
      (x)}  [{\displaystyle a_{0}(x)y+a_{1}(x)y'+a_{2}(x)y''+\cdots +a_{n}(x)y^
      {(n)}=b(x)}]
may be rewritten
         L y = b ( x ) .   {\displaystyle Ly=b(x).}  [{\displaystyle Ly=b(x).}]
There may be several variants to this notation; in particular the variable of
differentiation may appear explicitly or not in y and the right-hand and of the
equation, such as     L y ( x ) = b ( x )   {\displaystyle Ly(x)=b(x)}  [
{\displaystyle Ly(x)=b(x)}] or     L y = b   {\displaystyle Ly=b}  [
{\displaystyle Ly=b}]
The kernel of a linear differential operator is its kernel as a linear mapping,
that is the vector_space of the solutions of the (homogeneous) differential
equation     L y = 0   {\displaystyle Ly=0}  [{\displaystyle Ly=0}].
In the case of an ordinary differential operator of order n, CarathÃ©odory's
existence_theorem implies that, under very mild conditions, the kernel of L is
a vector space of dimension n, and that the solutions of the equation     L y
( x ) = b ( x )   {\displaystyle Ly(x)=b(x)}  [{\displaystyle Ly(x)=b(x)}] have
the form
          S  0   ( x ) +  c  1    S  1   ( x ) + &#x22EF; +  c  n    S  n   ( x
      ) ,   {\displaystyle S_{0}(x)+c_{1}S_{1}(x)+\cdots +c_{n}S_{n}(x),}  [
      {\displaystyle S_{0}(x)+c_{1}S_{1}(x)+\cdots +c_{n}S_{n}(x),}]
where      c  1   , &#x2026; ,  c  n     {\displaystyle c_{1},\ldots ,c_{n}}
[c_{1},\ldots ,c_{n}] are arbitrary numbers. Typically, the hypotheses of
CarathÃ©odory's theorem are satisfied in an interval I, if the functions     b
,  a  0   , &#x2026; ,  a  n     {\displaystyle b,a_{0},\ldots ,a_{n}}  [
{\displaystyle b,a_{0},\ldots ,a_{n}}] are continuous in I, and there is a
positive real number k such that      |   a  n   ( x )  |  > k   {\displaystyle
|a_{n}(x)|>k}  [{\displaystyle |a_{n}(x)|>k}] for every x in I.
***** Homogeneous equation with constant coefficients[edit] *****
A homogeneous linear differential equation has constant coefficients if it has
the form
          a  0   y +  a  1    y &#x2032;  +  a  2    y &#x2033;  + &#x22EF; +
      a  n    y  ( n )   = 0   {\displaystyle a_{0}y+a_{1}y'+a_{2}y''+\cdots
      +a_{n}y^{(n)}=0}  [{\displaystyle a_{0}y+a_{1}y'+a_{2}y''+\cdots +a_{n}y^
      {(n)}=0}]
where      a  1   , &#x2026; ,  a  n     {\displaystyle a_{1},\ldots ,a_{n}}
[a_1, \ldots, a_n] are (real or complex) numbers. In other words, it has
constant coefficients if it is defined by a linear operator with constant
coefficients.
The study of these differential equations with constant coefficients dates back
to Leonhard_Euler, who introduced the exponential_function      e  x
{\displaystyle e^{x}}  [e^{x}], which is the unique solution of the equation
f &#x2032;  = f   {\displaystyle f'=f}  [{\displaystyle f'=f}] such that     f
( 0 ) = 1   {\displaystyle f(0)=1}  [f(0)=1]. It follows that the nth
derivative of      e  c x     {\displaystyle e^{cx}}  [{\displaystyle e^{cx}}]
is      c  n    e  c x   ,   {\displaystyle c^{n}e^{cx},}  [{\displaystyle c^
{n}e^{cx},}] and this allows solving homogeneous linear differential equations
rather easily.
Let
          a  0   y +  a  1    y &#x2032;  +  a  2    y &#x2033;  + &#x22EF; +
      a  n    y  ( n )   = 0   {\displaystyle a_{0}y+a_{1}y'+a_{2}y''+\cdots
      +a_{n}y^{(n)}=0}  [{\displaystyle a_{0}y+a_{1}y'+a_{2}y''+\cdots +a_{n}y^
      {(n)}=0}]
be a homogeneous linear differential equation with constant coefficients (that
is      a  0   , &#x2026; ,  a  n     {\displaystyle a_{0},\ldots ,a_{n}}  [a_
{0},\ldots ,a_{n}] are real or complex numbers).
Searching solutions of this equation that have the form      e  &#x03B1; x
{\displaystyle e^{\alpha x}}  [{\displaystyle e^{\alpha x}}] is equivalent to
searching the constants     &#x03B1;   {\displaystyle \alpha }  [\alpha ] such
that
          a  0    e  &#x03B1; x   +  a  1   &#x03B1;  e  &#x03B1; x   +  a  2
      &#x03B1;  2    e  &#x03B1; x   + &#x22EF; +  a  n    &#x03B1;  n    e
      &#x03B1; x   = 0.   {\displaystyle a_{0}e^{\alpha x}+a_{1}\alpha e^
      {\alpha x}+a_{2}\alpha ^{2}e^{\alpha x}+\cdots +a_{n}\alpha ^{n}e^{\alpha
      x}=0.}  [{\displaystyle a_{0}e^{\alpha x}+a_{1}\alpha e^{\alpha x}+a_
      {2}\alpha ^{2}e^{\alpha x}+\cdots +a_{n}\alpha ^{n}e^{\alpha x}=0.}]
Factoring out      e  &#x03B1; x     {\displaystyle e^{\alpha x}}  [
{\displaystyle e^{\alpha x}}] (which is never zero) shows that     &#x03B1;
{\displaystyle \alpha }  [\alpha ] must be a root of the characteristic
polynomial
          a  0   +  a  1   t +  a  2    t  2   + &#x22EF; +  a  n    t  n
      {\displaystyle a_{0}+a_{1}t+a_{2}t^{2}+\cdots +a_{n}t^{n}}  [
      {\displaystyle a_{0}+a_{1}t+a_{2}t^{2}+\cdots +a_{n}t^{n}}]
of the differential equation.
When these roots are all distinct, one has n distinct solutions that are not
necessarily real, even if the coefficients of the equation are real. These
solutions can be shown to be linearly_independent, by considering the
Vandermonde_determinant of the values of these solutions at x = 0, ..., n â
1. Together they form a basis of the vector_space of solutions of the
differential equation (that is, the kernel of the differential operator).
Example
          y &#x2057;  &#x2212; 2  y &#x2034;  + 2  y &#x2033;  &#x2212; 2  y
      &#x2032;  + y = 0   {\displaystyle y''''-2y'''+2y''-2y'+y=0}  [y''''-
      2y'''+2y''-2y'+y=0]
has the characteristic equation
          z  4   &#x2212; 2  z  3   + 2  z  2   &#x2212; 2 z + 1 = 0.
      {\displaystyle z^{4}-2z^{3}+2z^{2}-2z+1=0.}  [z^{4}-2z^{3}+2z^{2}-
      2z+1=0.]
This has zeros, i, âi, and 1 (multiplicity 2). The solution basis is thus
          e  i x   ,   e  &#x2212; i x   ,   e  x   ,  x  e  x   .
      {\displaystyle e^{ix},\;e^{-ix},\;e^{x},\;xe^{x}.}  [{\displaystyle e^
      {ix},\;e^{-ix},\;e^{x},\;xe^{x}.}]
A real basis of solution is thus
         cos &#x2061; x ,  sin &#x2061; x ,   e  x   ,  x  e  x   .
      {\displaystyle \cos x,\;\sin x,\;e^{x},\;xe^{x}.}  [{\displaystyle \cos
      x,\;\sin x,\;e^{x},\;xe^{x}.}]
In the case where the characteristic polynomial has only simple_roots, the
preceding provides a complete basis of the solutions vector space. In the case
of multiple_roots, more linearly independent solutions are needed for having a
basis. These have the form
          x  k    e  &#x03B1; x   ,   {\displaystyle x^{k}e^{\alpha x},}  [
      {\displaystyle x^{k}e^{\alpha x},}]
where k is a nonnegative integer,     &#x03B1;   {\displaystyle \alpha }
[\alpha ] is a root of the characteristic polynomial of multiplicity m, and k <
m. For proving that these functions are solutions, one may remark that if
&#x03B1;   {\displaystyle \alpha }  [\alpha ] is a root of the characteristic
polynomial of multiplicity m, the characteristic polynomial may be factored as
P ( t ) ( t &#x2212; &#x03B1;  )  m   .   {\displaystyle P(t)(t-\alpha )^{m}.}
[{\displaystyle P(t)(t-\alpha )^{m}.}] Thus, applying the differential operator
of the equation is equivalent with applying first m times the operator       d
d x    &#x2212; &#x03B1; ,   {\displaystyle {\frac {d}{dx}}-\alpha ,}  [
{\displaystyle {\frac {d}{dx}}-\alpha ,}] and then the operator that has P as
characteristic polynomial. By the exponential_shift_theorem,
          (    d  d x    &#x2212; &#x03B1;  )   (   x  k    e  &#x03B1; x    )
      = k  x  k &#x2212; 1    e  &#x03B1; x   ,   {\displaystyle \left({\frac
      {d}{dx}}-\alpha \right)\left(x^{k}e^{\alpha x}\right)=kx^{k-1}e^{\alpha
      x},}  [{\displaystyle \left({\frac {d}{dx}}-\alpha \right)\left(x^{k}e^
      {\alpha x}\right)=kx^{k-1}e^{\alpha x},}]
and thus one gets zero after k + 1 application of       d  d x    &#x2212;
&#x03B1; .   {\displaystyle {\frac {d}{dx}}-\alpha .}  [{\displaystyle {\frac
{d}{dx}}-\alpha .}]
As, by the fundamental_theorem_of_algebra, the sum of the multiplicities of the
roots of a polynomial equals the degree of the polynomial, the number of above
solutions equals the order of the differential equation, and these solutions
form a base of the vector space of the solutions.
In the common case where the coefficients of the equation are real, it is
generally more convenient to have a basis of the solutions consisting of real-
valued_functions. Such a basis may be obtained from the preceding basis by
remarking that, if a + ib is a root of the characteristic polynomial, then a
â ib is also a root, of the same multiplicity. Thus a real basis is obtained
by using Euler's_formula, and replacing      x  k    e  ( a + i b ) x
{\displaystyle x^{k}e^{(a+ib)x}}  [{\displaystyle x^{k}e^{(a+ib)x}}] and      x
k    e  ( a &#x2212; i b ) x     {\displaystyle x^{k}e^{(a-ib)x}}  [
{\displaystyle x^{k}e^{(a-ib)x}}] by      x  k    e  a x   cos &#x2061; ( b x )
{\displaystyle x^{k}e^{ax}\cos(bx)}  [{\displaystyle x^{k}e^{ax}\cos(bx)}] and
x  k    e  a x   sin &#x2061; ( b x ) .   {\displaystyle x^{k}e^{ax}\sin(bx).}
[{\displaystyle x^{k}e^{ax}\sin(bx).}]
**** Second-order case[edit] ****
A homogeneous linear differential equation of the second order may be written
          y &#x2033;  + a  y &#x2032;  + b y = 0 ,   {\displaystyle
      y''+ay'+by=0,}  [{\displaystyle y''+ay'+by=0,}]
and its characteristic polynomial is
          r  2   + a r + b .   {\displaystyle r^{2}+ar+b.}  [{\displaystyle r^
      {2}+ar+b.}]
If a and b are real, there are three cases for the solutions, depending on the
discriminant     D =  a  2   &#x2212; 4 b .   {\displaystyle D=a^{2}-4b.}  [
{\displaystyle D=a^{2}-4b.}] In all three cases, the general solution depends
on two arbitrary constants      c  1     {\displaystyle c_{1}}  [c_{1}] and
c  2     {\displaystyle c_{2}}  [c_{2}].
    * If D > 0, the characteristic polynomial has two distinct real roots
      &#x03B1;   {\displaystyle \alpha }  [\alpha ], and     &#x03B2;
      {\displaystyle \beta }  [\beta ]. In this case, the general solution is
                c  1    e  &#x03B1; x   +  c  2    e  &#x03B2; x   .
            {\displaystyle c_{1}e^{\alpha x}+c_{2}e^{\beta x}.}  [
            {\displaystyle c_{1}e^{\alpha x}+c_{2}e^{\beta x}.}]
    * If D = 0, the characteristic polynomial has a double root     &#x2212; a
      /  2   {\displaystyle -a/2}  [{\displaystyle -a/2}], and the general
      solution is
               (  c  1   +  c  2   x )  e  &#x2212; a x  /  2   .
            {\displaystyle (c_{1}+c_{2}x)e^{-ax/2}.}  [{\displaystyle (c_{1}+c_
            {2}x)e^{-ax/2}.}]
    * If D < 0, the characteristic polynomial has two complex_conjugate roots
      &#x03B1; &#x00B1; &#x03B2; i   {\displaystyle \alpha \pm \beta i}  [
      {\displaystyle \alpha \pm \beta i}], and the general solution is
                c  1    e  ( &#x03B1; + &#x03B2; i ) x   +  c  2    e
            ( &#x03B1; &#x2212; &#x03B2; i ) x   ,   {\displaystyle c_{1}e^{
            (\alpha +\beta i)x}+c_{2}e^{(\alpha -\beta i)x},}  [{\displaystyle
            c_{1}e^{(\alpha +\beta i)x}+c_{2}e^{(\alpha -\beta i)x},}]
      which may be rewritten in real terms, using Euler's_formula as
                e  &#x03B1; x   (  c  1   cos &#x2061; ( &#x03B2; x ) +  c  2
            sin &#x2061; ( &#x03B2; x ) ) .   {\displaystyle e^{\alpha x}(c_
            {1}\cos(\beta x)+c_{2}\sin(\beta x)).}  [{\displaystyle e^{\alpha
            x}(c_{1}\cos(\beta x)+c_{2}\sin(\beta x)).}]
Finding the solution     y ( x )   {\displaystyle y(x)}  [y(x)] satisfying
y ( 0 ) =  d  1     {\displaystyle y(0)=d_{1}}  [{\displaystyle y(0)=d_{1}}]
and      y &#x2032;  ( 0 ) =  d  2   ,   {\displaystyle y'(0)=d_{2},}  [
{\displaystyle y'(0)=d_{2},}] one equates the values of the above general
solution at 0 and its derivative there to      d  1     {\displaystyle d_{1}}
[{\displaystyle d_{1}}] and      d  2   ,   {\displaystyle d_{2},}  [
{\displaystyle d_{2},}] respectively. This results in a linear system of two
linear equations in the two unknowns      c  1     {\displaystyle c_{1}}  [c_
{1}] and      c  2   .   {\displaystyle c_{2}.}  [{\displaystyle c_{2}.}]
Solving this system gives the solution for a so called Cauchy_problem, in which
the values at 0 for the solution of the DEQ and its derivative are specified.
***** Non-homogeneous equation with constant coefficients[edit] *****
A non-homogeneous equation of order n with constant coefficients may be written
          y  ( n )   ( x ) +  a  1    y  ( n &#x2212; 1 )   ( x ) + &#x22EF; +
      a  n &#x2212; 1    y &#x2032;  ( x ) +  a  n   y ( x ) = f ( x ) ,
      {\displaystyle y^{(n)}(x)+a_{1}y^{(n-1)}(x)+\cdots +a_{n-1}y'(x)+a_{n}y
      (x)=f(x),}  [{\displaystyle y^{(n)}(x)+a_{1}y^{(n-1)}(x)+\cdots +a_{n-
      1}y'(x)+a_{n}y(x)=f(x),}]
where      a  1   , &#x2026; ,  a  n     {\displaystyle a_{1},\ldots ,a_{n}}
[a_1, \ldots, a_n] are real or complex numbers, f is a given function of x, and
y is the unknown function (for sake of simplicity, "(x)" will be omitted in the
following).
There are several methods for solving such an equation. The best method depends
of the nature of the function f that makes the equation non-homogeneous. If f
is a linear combination of exponential and sinusoidal functions, then
exponential_response_formula may be used. If, more generally, f is linear
combination of functions of the form      x  n    e  a x     {\displaystyle x^
{n}e^{ax}}  [{\displaystyle x^{n}e^{ax}}],      x  n   cos &#x2061;  a x
{\displaystyle x^{n}\cos {ax}}  [{\displaystyle x^{n}\cos {ax}}] and      x  n
sin &#x2061;  a x    {\displaystyle x^{n}\sin {ax}}  [{\displaystyle x^{n}\sin
{ax}}], where n is a nonnegative integer and a a constant (which need not to be
the same in each term), then the method_of_undetermined_coefficients may be
used. Still more general, the annihilator_method applies when f satisfies a
homogeneous linear differential equation, typically, a holonomic_function.
The most general method is the variation_of_constants, which is presented here.
The general solution of the associated homogeneous equation
          y  ( n )   +  a  1    y  ( n &#x2212; 1 )   + &#x22EF; +  a  n
      &#x2212; 1    y &#x2032;  +  a  n   y = 0   {\displaystyle y^{(n)}+a_
      {1}y^{(n-1)}+\cdots +a_{n-1}y'+a_{n}y=0}  [{\displaystyle y^{(n)}+a_{1}y^
      {(n-1)}+\cdots +a_{n-1}y'+a_{n}y=0}]
is
         y =  u  1    y  1   + &#x22EF; +  u  n    y  n   ,   {\displaystyle
      y=u_{1}y_{1}+\cdots +u_{n}y_{n},}  [{\displaystyle y=u_{1}y_{1}+\cdots
      +u_{n}y_{n},}]
where     (  y  1   , &#x2026; ,  y  n   )   {\displaystyle (y_{1},\ldots ,y_
{n})}  [{\displaystyle (y_{1},\ldots ,y_{n})}] is a basis of the vector space
of the solutions and      u  1   , &#x2026; ,  u  n     {\displaystyle u_
{1},\ldots ,u_{n}}  [u_{1},\ldots ,u_{n}] are arbitrary constants. The method
of variation of constants takes its name that, instead of considering      u  1
, &#x2026; ,  u  n     {\displaystyle u_{1},\ldots ,u_{n}}  [u_{1},\ldots ,u_
{n}] as constants, they are considered as functions that have to be determined
for making y a solution of the non-homogeneous equation. For this purpose, one
adds the constraints
         0 =  u  1  &#x2032;   y  1   +  u  2  &#x2032;   y  2   + &#x22EF; +
      u  n  &#x2032;   y  n     {\displaystyle 0=u'_{1}y_{1}+u'_{2}y_{2}+\cdots
      +u'_{n}y_{n}}  [0=u'_{1}y_{1}+u'_{2}y_{2}+\cdots +u'_{n}y_{n}]
         0 =  u  1  &#x2032;   y  1  &#x2032;  +  u  2  &#x2032;   y  2
      &#x2032;  + &#x22EF; +  u  n  &#x2032;   y  n  &#x2032;    {\displaystyle
      0=u'_{1}y'_{1}+u'_{2}y'_{2}+\cdots +u'_{n}y'_{n}}  [0=u'_{1}y'_{1}+u'_
      {2}y'_{2}+\cdots +u'_{n}y'_{n}]
         &#x22EF;   {\displaystyle \cdots }  [\cdots ]
         0 =  u  1  &#x2032;   y  1   ( n &#x2212; 2 )   +  u  2  &#x2032;   y
      2   ( n &#x2212; 2 )   + &#x22EF; +  u  n  &#x2032;   y  n   ( n &#x2212;
      2 )   ,   {\displaystyle 0=u'_{1}y_{1}^{(n-2)}+u'_{2}y_{2}^{(n-2)}+\cdots
      +u'_{n}y_{n}^{(n-2)},}  [{\displaystyle 0=u'_{1}y_{1}^{(n-2)}+u'_{2}y_
      {2}^{(n-2)}+\cdots +u'_{n}y_{n}^{(n-2)},}]
which imply (by product_rule and induction)
          y  ( i )   =  u  1    y  1   ( i )   + &#x22EF; +  u  n    y  n   ( i
      )     {\displaystyle y^{(i)}=u_{1}y_{1}^{(i)}+\cdots +u_{n}y_{n}^{(i)}}
      [{\displaystyle y^{(i)}=u_{1}y_{1}^{(i)}+\cdots +u_{n}y_{n}^{(i)}}]
for i = 1, ..., n â 1, and
          y  ( n )   =  u  1    y  1   ( n )   + &#x22EF; +  u  n    y  n   ( n
      )   +  u  1  &#x2032;   y  1   ( n &#x2212; 1 )   +  u  2  &#x2032;   y
      2   ( n &#x2212; 1 )   + &#x22EF; +  u  n  &#x2032;   y  n   ( n &#x2212;
      1 )   .   {\displaystyle y^{(n)}=u_{1}y_{1}^{(n)}+\cdots +u_{n}y_{n}^{
      (n)}+u'_{1}y_{1}^{(n-1)}+u'_{2}y_{2}^{(n-1)}+\cdots +u'_{n}y_{n}^{(n-
      1)}.}  [{\displaystyle y^{(n)}=u_{1}y_{1}^{(n)}+\cdots +u_{n}y_{n}^{
      (n)}+u'_{1}y_{1}^{(n-1)}+u'_{2}y_{2}^{(n-1)}+\cdots +u'_{n}y_{n}^{(n-
      1)}.}]
Replacing in the original equation y and its derivative by these expression,
and using the fact that      y  1   , &#x2026; ,  y  n     {\displaystyle y_
{1},\ldots ,y_{n}}  [y_{1},\ldots ,y_{n}] are solutions of the original
homogeneous equation, one gets
         f =  u  1  &#x2032;   y  1   ( n &#x2212; 1 )   + &#x22EF; +  u  n
      &#x2032;   y  n   ( n &#x2212; 1 )   .   {\displaystyle f=u'_{1}y_{1}^{
      (n-1)}+\cdots +u'_{n}y_{n}^{(n-1)}.}  [{\displaystyle f=u'_{1}y_{1}^{(n-
      1)}+\cdots +u'_{n}y_{n}^{(n-1)}.}]
One has thus a system of n linear equations in      u  1  &#x2032;  , &#x2026;
,  u  n  &#x2032;    {\displaystyle u'_{1},\ldots ,u'_{n}}  [u'_{1},\ldots ,u'_
{n}], which can be solved by any method of linear_algebra. Then the computation
of antiderivatives gives      u  1   , &#x2026; ,  u  n     {\displaystyle u_
{1},\ldots ,u_{n}}  [u_{1},\ldots ,u_{n}] and then     y =  u  1    y  1   +
&#x22EF; +  u  n    y  n   .   {\displaystyle y=u_{1}y_{1}+\cdots +u_{n}y_{n}.}
[{\displaystyle y=u_{1}y_{1}+\cdots +u_{n}y_{n}.}]
As antiderivatives are defined up to the addition of a constant, one finds
again that the general solution of the non-homogeneous equation is the sum of
an arbitrary solution and the general solution of the associated homogeneous
equation.
***** First-order equation with variable coefficients[edit] *****
Example
Solving the equation
          y &#x2032;  ( x ) + y ( x )  /  x = 3 x .   {\displaystyle y'(x)+y
      (x)/x=3x.}  [{\displaystyle y'(x)+y(x)/x=3x.}]
The associated homogeneous equation gives
          y &#x2032;   /  y = &#x2212; 1  /  x ,   {\displaystyle y'/y=-1/x,}
      [{\displaystyle y'/y=-1/x,}]
that is
         y = c  /  x .   {\displaystyle y=c/x.}  [{\displaystyle y=c/x.}]
Dividing the original equation by one of these solutions gives
         x  y &#x2032;  + y = 3  x  2   .   {\displaystyle xy'+y=3x^{2}.}  [
      {\displaystyle xy'+y=3x^{2}.}]
That is
         ( x y  ) &#x2032;  = 3  x  2   ,   {\displaystyle (xy)'=3x^{2},}  [
      {\displaystyle (xy)'=3x^{2},}]
         x y =  x  3   + c ,   {\displaystyle xy=x^{3}+c,}  [{\displaystyle
      xy=x^{3}+c,}]
and
         y ( x ) =  x  2   + c  /  x .   {\displaystyle y(x)=x^{2}+c/x.}  [
      {\displaystyle y(x)=x^{2}+c/x.}]
For the initial condition
         y ( 1 ) = &#x03B1; ,   {\displaystyle y(1)=\alpha ,}  [{\displaystyle
      y(1)=\alpha ,}]
one gets the particular solution
         y ( x ) =  x  2   +    &#x03B1; &#x2212; 1  x   .   {\displaystyle y
      (x)=x^{2}+{\frac {\alpha -1}{x}}.}  [{\displaystyle y(x)=x^{2}+{\frac
      {\alpha -1}{x}}.}]
The general form of a linear ordinary differential linear equation of order 1
is, after having divided by the coefficient of      y &#x2032;  ( x )
{\displaystyle y'(x)}  [{\displaystyle y'(x)}],
          y &#x2032;  ( x ) = f ( x ) y ( x ) + g ( x ) .   {\displaystyle y'
      (x)=f(x)y(x)+g(x).}  [{\displaystyle y'(x)=f(x)y(x)+g(x).}]
In the case of a homogeneous equation (that is g(x) is the zero function), the
equation may be rewritten as (omitting "(x)" for sake of simplification)
            y &#x2032;  y   = f ,   {\displaystyle {\frac {y'}{y}}=f,}  [
      {\displaystyle {\frac {y'}{y}}=f,}]
that may easily be integrated as
         log &#x2061; y = k + F ,   {\displaystyle \log y=k+F,}  [
      {\displaystyle \log y=k+F,}]
where k is an arbitrary constant_of_integration and
         F = &#x222B; f d x   {\displaystyle F=\int fdx}  [{\displaystyle
      F=\int fdx}]
is an antiderivative of f. Thus, the general solution of the homogeneous
equation is
         y = c  e  F   ,   {\displaystyle y=ce^{F},}  [{\displaystyle y=ce^
      {F},}]
where     c =  e  k     {\displaystyle c=e^{k}}  [{\displaystyle c=e^{k}}] is
an arbitrary constant.
For solving the non homogeneous equation, one may multiply it by the
multiplicative_inverse      e  &#x2212; F     {\displaystyle e^{-F}}  [
{\displaystyle e^{-F}}] of a solution the homogeneous equation. This gives
          y &#x2032;   e  &#x2212; F   &#x2212; y f  e  &#x2212; F   = g  e
      &#x2212; F   .   {\displaystyle y'e^{-F}-yfe^{-F}=ge^{-F}.}  [
      {\displaystyle y'e^{-F}-yfe^{-F}=ge^{-F}.}]
As     &#x2212; f  e  &#x2212; F   =   d  d x     (  e  &#x2212; F   )  ,
{\displaystyle -fe^{-F}={\frac {d}{dx}}\left(e^{-F}\right),}  [{\displaystyle -
fe^{-F}={\frac {d}{dx}}\left(e^{-F}\right),}] the product_rule allows rewriting
the equation as
           d  d x     (  y  e  &#x2212; F    )  = g  e  &#x2212; F   .
      {\displaystyle {\frac {d}{dx}}\left(ye^{-F}\right)=ge^{-F}.}  [
      {\displaystyle {\frac {d}{dx}}\left(ye^{-F}\right)=ge^{-F}.}]
Thus, the general solution is
         y = c  e  F   +  e  F   &#x222B; g  e  &#x2212; F   d x ,
      {\displaystyle y=ce^{F}+e^{F}\int ge^{-F}dx,}  [{\displaystyle y=ce^
      {F}+e^{F}\int ge^{-F}dx,}]
where c is a constant of integration, and     F = &#x222B; f d x
{\displaystyle F=\int fdx}  [{\displaystyle F=\int fdx}].
***** System of linear differential equations[edit] *****
Main article: Matrix_differential_equation
A system of linear differential equations consists of several linear
differential equations that involve several unknown functions. In general one
restricts the study to systems such that the number of unknown functions equals
the number of equations.
An arbitrary linear ordinary differential equation and a system of such
equations can be converted into a first order system of linear differential
equations by adding variables for all but the highest order derivatives. That
is, if      y &#x2032;  ,  y &#x2033;  , &#x2026; ,  y  ( k )
{\displaystyle y',y'',\ldots ,y^{(k)}}  [{\displaystyle y',y'',\ldots ,y^{
(k)}}] appear in an equation, one may replace them by new unknown functions
y  1   , &#x2026; ,  y  k     {\displaystyle y_{1},\ldots ,y_{k}}  [
{\displaystyle y_{1},\ldots ,y_{k}}] that must satisfy the equations      y
&#x2032;  =  y  1     {\displaystyle y'=y_{1}}  [{\displaystyle y'=y_{1}}] and
y  i  &#x2032;  =  y  i + 1   ,   {\displaystyle y_{i}'=y_{i+1},}  [
{\displaystyle y_{i}'=y_{i+1},}] for i = 1, ..., k â 1.
A linear system of the first order, which has n unknown functions and n
differential equations may normally be solved for the derivatives of the
unknown functions. If it is not the case this is a differential-algebraic
system, and this is a different theory. Therefore, the systems that are
considered here have the form
              y  1  &#x2032;  ( x )    =  b  1   ( x ) +  a  1 , 1   ( x )  y
      1   + &#x22EF; +  a  1 , n   ( x )  y  n       &#x22EE;       y  n
      &#x2032;  ( x )    =  b  n   ( x ) +  a  n , 1   ( x )  y  1   + &#x22EF;
      +  a  n , n   ( x )  y  n   ,       {\displaystyle {\begin{aligned}y_{1}'
      (x)&=b_{1}(x)+a_{1,1}(x)y_{1}+\cdots +a_{1,n}(x)y_{n}\\\vdots &\\y_{n}'
      (x)&=b_{n}(x)+a_{n,1}(x)y_{1}+\cdots +a_{n,n}(x)y_{n},\end{aligned}}}  [
      {\displaystyle {\begin{aligned}y_{1}'(x)&=b_{1}(x)+a_{1,1}(x)y_{1}+\cdots
      +a_{1,n}(x)y_{n}\\\vdots &\\y_{n}'(x)&=b_{n}(x)+a_{n,1}(x)y_{1}+\cdots
      +a_{n,n}(x)y_{n},\end{aligned}}}]
where      b  n     {\displaystyle b_{n}}  [b_{n}] and the      a  i , j
{\displaystyle a_{i,j}}  [a_{i,j}] are functions of x. In matrix notation, this
system may be written (omitting "(x)")
           y  &#x2032;  = A  y  +  b  .   {\displaystyle \mathbf {y} '=A\mathbf
      {y} +\mathbf {b} .}  [{\displaystyle \mathbf {y} '=A\mathbf {y} +\mathbf
      {b} .}]
The solving method is similar to that of a single first order linear
differential equations, but with complications stemming from noncommutativity
of matrix multiplication.
Let
           u  &#x2032;  = A  u  .   {\displaystyle \mathbf {u} '=A\mathbf {u}
      .}  [{\displaystyle \mathbf {u} '=A\mathbf {u} .}]
be the homogeneous equation associated to the above matrix equation. Its
solutions form a vector_space of dimension n, and are therefore the columns of
a square_matrix of functions     U ( x )   {\displaystyle U(x)}  [U(x)], whose
determinant is not the zero function. If n = 1, or A is a matrix of constants,
or, more generally, if A is differentiable and commutes with its derivative,
then one may choose for U the exponential of an antiderivative      B =
&#x222B; A d x    {\displaystyle \textstyle B=\int Adx}  [{\displaystyle
\textstyle B=\int Adx}] of A. In fact, in these cases, one has
           d  d x    exp &#x2061; ( B ) = A exp &#x2061; ( B ) .
      {\displaystyle {\frac {d}{dx}}\exp(B)=A\exp(B).}  [{\displaystyle {\frac
      {d}{dx}}\exp(B)=A\exp(B).}]
In the general case there is no closed-form solution for the homogeneous
equation, and one has to use either a numerical_method, or an approximation
method such as Magnus_expansion.
Knowing the matrix U, the general solution of the non-homogeneous equation is
          y  ( x ) = U ( x )   y  0    + U ( x ) &#x222B;  U  &#x2212; 1   ( x
      )  b  ( x )  d x ,   {\displaystyle \mathbf {y} (x)=U(x)\mathbf {y_{0}}
      +U(x)\int U^{-1}(x)\mathbf {b} (x)\,dx,}  [{\displaystyle \mathbf {y}
      (x)=U(x)\mathbf {y_{0}} +U(x)\int U^{-1}(x)\mathbf {b} (x)\,dx,}]
where the column matrix       y  0      {\displaystyle \mathbf {y_{0}} }  [
{\displaystyle \mathbf {y_{0}} }] is an arbitrary constant_of_integration.
If initial conditions are given as
          y  (  x  0   ) =   y   0   ,   {\displaystyle \mathbf {y} (x_
      {0})=\mathbf {y} _{0},}  [{\displaystyle \mathbf {y} (x_{0})=\mathbf {y}
      _{0},}]
the solution that satisfies these initial conditions is
          y  ( x ) = U ( x )  U  &#x2212; 1   (  x  0   )   y  0    + U ( x )
      &#x222B;   x  0     x    U  &#x2212; 1   ( t )  b  ( t )  d t .
      {\displaystyle \mathbf {y} (x)=U(x)U^{-1}(x_{0})\mathbf {y_{0}} +U(x)\int
      _{x_{0}}^{x}U^{-1}(t)\mathbf {b} (t)\,dt.}  [{\displaystyle \mathbf {y}
      (x)=U(x)U^{-1}(x_{0})\mathbf {y_{0}} +U(x)\int _{x_{0}}^{x}U^{-1}
      (t)\mathbf {b} (t)\,dt.}]
***** Higher order with variable coefficients[edit] *****
A linear ordinary equation of order one with variable coefficients may be
solved by quadrature, which means that the solutions may be expressed in terms
of integrals. This is not the case for order at least two. This is the main
result of PicardâVessiot_theory, a theory that was initiated by Ãmile_Picard
and Ernest_Vessiot, and whose recent developments are called differential
Galois_theory.
The impossibility of solving by quadrature can be compared with the
AbelâRuffini_theorem, which states that an algebraic_equation of degree at
least five cannot, in general, be solved by radicals. This analogy extends to
the proof methods and motivates the denomination of differential_Galois_theory
Similarly to the algebraic case, the theory allows deciding which equations may
be solved by quadrature, and if possible solving them. However, for both
theories, the necessary computations are extremely difficult, even with the
most powerful computers.
Nevertheless, the case of order two with rational coefficients has been
completely solved by Kovacic's_algorithm.
**** CauchyâEuler equation[edit] ****
CauchyâEuler_equations are examples of equations of any order, with variable
coefficients, that can be solved explicitly. These are the equations of the
form
          x  n    y  ( n )   ( x ) +  a  n &#x2212; 1    x  n &#x2212; 1    y
      ( n &#x2212; 1 )   ( x ) + &#x22EF; +  a  0   y ( x ) = 0 ,
      {\displaystyle x^{n}y^{(n)}(x)+a_{n-1}x^{n-1}y^{(n-1)}(x)+\cdots +a_{0}y
      (x)=0,}  [{\displaystyle x^{n}y^{(n)}(x)+a_{n-1}x^{n-1}y^{(n-1)}
      (x)+\cdots +a_{0}y(x)=0,}]
where      a  0   , &#x2026; ,  a  n &#x2212; 1     {\displaystyle a_{0},\ldots
,a_{n-1}}  [{\displaystyle a_{0},\ldots ,a_{n-1}}] are constant coefficients.
***** Holonomic functions[edit] *****
Main article: holonomic_function
A holonomic_function, also called a D-finite function is a function that is a
solution of a homogeneous linear differential equation with polynomial
coefficients.
Most functions that are commonly considered in mathematics are holonomic or
quotients of holonomic functions. In fact, holonomic functions include
polynomials, algebraic_functions, logarithm, exponential_function, sine,
cosine, hyperbolic_sine, hyperbolic_cosine, inverse_trigonometric and inverse
hyperbolic_functions, and many special_functions such as Bessel_functions and
hypergeometric_functions.
Holonomic functions have several closure_properties; in particular, sums,
products, derivative and integrals of holonomic functions are holonomic.
Moreover, these closure properties are effective, in the sense that there are
algorithms for computing the differential equation of the result of any of
these operations, knowing the differential equations of the input.[2]
Usefulness of the concept of holonomic functions results of Zeilberger's
theorem, which follows.[2]
A holonomic sequence is a sequence of numbers that may be generated by a
recurrence_relation with polynomial coefficients. The coefficients of the
Taylor_series at a point of a holonomic function form a holonomic sequence.
Conversely, if the sequence of the coefficients of a power_series is holonomic,
then the series defines a holonomic function (even if the radius_of_convergence
is zero). There are efficient algorithms for both conversions, that is for
computing the recurrence relation from the differential equation, and vice
versa. [2]
It follows that, if one represents (in a computer) holonomic functions by their
defining differential equations and initial conditions, most calculus
operations can be done automatically on these functions, such as derivative,
indefinite and definite_integral, fast computation of Taylor series (thanks of
the recurrence relation on its coefficients), evaluation to a high precision
with certified bound of the approximation error, limits, localization of
singularities, asymptotic_behavior at infinity and near singularities, proof of
identities, etc.[3]
***** See also[edit] *****
    * Continuous-repayment_mortgage
    * Fourier_transform
    * Laplace_transform
    * Linear_difference_equation
***** References[edit] *****
   1. ^ Gershenfeld 1999, p.9
   2. ^ a b c Zeilberger, Doron. A_holonomic_systems_approach_to_special
      functions_identities. Journal of computational and applied mathematics.
      32.3 (1990): 321-368
   3. ^ Benoit, A., Chyzak, F., Darrasse, A., Gerhold, S., Mezzarobba, M., &
      Salvy, B. (2010, September). The_dynamic_dictionary_of_mathematical
      functions_(DDMF). In International Congress on Mathematical Software (pp.
      35-41). Springer, Berlin, Heidelberg.
    * Birkhoff, Garrett & Rota, Gian-Carlo (1978), Ordinary Differential
      Equations, New York: John Wiley and Sons, Inc., ISBN 0-471-07411-X
Gershenfeld, Neil (1999), The Nature of Mathematical Modeling, Cambridge, UK.:
Cambridge University Press, ISBN 978-0-521-57095-4
Robinson, James C. (2004), An Introduction to Ordinary Differential Equations,
Cambridge, UK.: Cambridge University Press, ISBN 0-521-82650-0
***** External links[edit] *****
    * http://eqworld.ipmnet.ru/en/solutions/ode.htm
    * Dynamic_Dictionary_of_Mathematical_Function. Automatic and interactive
      study of many holonomic functions.
    * v
    * t
    * e
Differential_equations
                                           * Differential_operator
                                           * Notation_for_differentiation
                                           * Ordinary
                                           * Partial
               Operations                  * Differential-algebraic
                                           * Integro-differential
                                           * Fractional
                                           * Linear
                                           * Non-linear
                                           * Dependent_and_independent_variables
Classification                             * Homogeneous
                                           * Nonhomogeneous
                                           * Coupled
               Attributes of variables     * Decoupled
                                           * Order
                                           * Degree
                                           * Autonomous
                                           * Exact_differential_equation
                                           * Complex_differential_equation
                                           * Difference (discrete analogue)
               Relation to processes       * stochastic
                                           * Delay
                            * PicardâLindelÃ¶f_theorem (existence and uniqueness)
                            * Wronskian
                            * Phase_portrait
                            * Phase_space
                            * Lyapunov_stability
               Solution     * Asymptotic_stability
               topics       * Exponential_stability
                            * Rate_of_convergence
                            * Series_solutions
                            * Integral solutions
                            * Numerical_integration
                            * Dirac_delta_function
Solutions                   * Inspection
                            * Separation_of_variables                                    [Elmer-pump-
                            * Method_of_undetermined_coefficients                        heatequation.png]
                            * Variation_of_parameters
                            * Integrating_factor
                            * Integral_transforms
               Solution     * Euler_method
               methods      * Finite_difference_method
                            * CrankâNicolson_method
                            * RungeâKutta_methods
                            * Finite_element_method
                            * Finite_volume_method
                            * Galerkin_method
                            * Perturbation_theory
                   * Astronomy
                   * Physics
                   * Continuum_mechanics
                   * Chaos_theory
Applications       * Chemistry
                   * Dynamical_system
                   * Economics
                   * Biology
                   * Geology
                   * Population_dynamics
                   * Isaac_Newton
                   * Gottfried_Wilhelm_Leibniz
                   * Leonhard_Euler
                   * Jacob_Bernoulli
                   * Ãmile_Picard
                   * JÃ³zef_Maria_Hoene-WroÅski
Mathematicians     * Ernst_LindelÃ¶f
                   * Rudolf_Lipschitz
                   * Joseph-Louis_Lagrange
                   * Augustin-Louis_Cauchy
                   * John_Crank
                   * Phyllis_Nicolson
                   * Carl_David_TolmÃ©_Runge
                   * Martin_Kutta

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Linear_differential_equation&oldid=906970688"
Categories:
    * Differential_equations
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * LietuviÅ³
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 19 July 2019, at 15:15 (UTC).
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
