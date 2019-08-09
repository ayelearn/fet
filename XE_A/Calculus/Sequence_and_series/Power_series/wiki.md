The following text has been accessed from https://en.wikipedia.org/wiki/Power_series at Fri Aug 9 00:02:09 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Power series ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, a power series (in one variable) is an infinite_series of the
form
          &#x2211;  n = 0   &#x221E;    a  n     (  x &#x2212; c  )   n   =  a
      0   +  a  1   ( x &#x2212; c  )  1   +  a  2   ( x &#x2212; c  )  2   +
      &#x22EF;   {\displaystyle \sum _{n=0}^{\infty }a_{n}\left(x-c\right)^
      {n}=a_{0}+a_{1}(x-c)^{1}+a_{2}(x-c)^{2}+\cdots }  [{\displaystyle \sum _
      {n=0}^{\infty }a_{n}\left(x-c\right)^{n}=a_{0}+a_{1}(x-c)^{1}+a_{2}(x-c)^
      {2}+\cdots }]
where an represents the coefficient of the nth term and c is a constant. an is
independent of x and may be expressed as a function of n (e.g.,      a  n   = 1
/  n !   {\displaystyle a_{n}=1/n!}  [{\displaystyle a_{n}=1/n!}]). Power
series are useful in analysis since they arise as Taylor_series of infinitely
differentiable functions. In fact, Borel's_theorem implies that every power
series is the Taylor series of some smooth function.
In many situations c (the center of the series) is equal to zero, for instance
when considering a Maclaurin_series. In such cases, the power series takes the
simpler form
          &#x2211;  n = 0   &#x221E;    a  n    x  n   =  a  0   +  a  1   x +
      a  2    x  2   + &#x22EF;   {\displaystyle \sum _{n=0}^{\infty }a_{n}x^
      {n}=a_{0}+a_{1}x+a_{2}x^{2}+\cdots }  [{\displaystyle \sum _{n=0}^{\infty
      }a_{n}x^{n}=a_{0}+a_{1}x+a_{2}x^{2}+\cdots }]
These power series arise primarily in analysis, but also occur in combinatorics
as generating_functions (a kind of formal_power_series) and in electrical
engineering (under the name of the Z-transform). The familiar decimal_notation
for real_numbers can also be viewed as an example of a power series, with
integer coefficients, but with the argument x fixed at &#x200b;1⁄10. In number
theory, the concept of p-adic_numbers is also closely related to that of a
power series.
⁰
***** Contents *****
    * 1_Examples
          o 1.1_On_the_set_of_exponents
    * 2_Radius_of_convergence
    * 3_Operations_on_power_series
          o 3.1_Addition_and_subtraction
          o 3.2_Multiplication_and_division
          o 3.3_Differentiation_and_integration
    * 4_Analytic_functions
          o 4.1_Behavior_near_the_boundary
    * 5_Formal_power_series
    * 6_Power_series_in_several_variables
    * 7_Order_of_a_power_series
    * 8_See_also
    * 9_Notes
    * 10_References
    * 11_External_links
***** Examples[edit] *****
The exponential_function (in blue), and the sum of the first n + 1 terms of its
Maclaurin_power_series (in red).
Any polynomial can be easily expressed as a power series around any center c,
although all but finitely many the coefficients will be zero since a power
series has infinitely many terms by definition. For instance, the polynomial
f ( x ) =  x  2   + 2 x + 3   {\textstyle f(x)=x^{2}+2x+3}  [{\textstyle f
(x)=x^{2}+2x+3}] can be written as a power series around the center     c = 0
{\textstyle c=0}  [{\textstyle c=0}] as
         f ( x ) = 3 + 2 x + 1  x  2   + 0  x  3   + 0  x  4   + &#x22EF;
      {\displaystyle f(x)=3+2x+1x^{2}+0x^{3}+0x^{4}+\cdots \,}  [f(x) = 3 + 2 x
      + 1 x^2 + 0 x^3 + 0 x^4 + \cdots \,]
or around the center     c = 1   {\textstyle c=1}  [{\textstyle c=1}] as
         f ( x ) = 6 + 4 ( x &#x2212; 1 ) + 1 ( x &#x2212; 1  )  2   + 0 ( x
      &#x2212; 1  )  3   + 0 ( x &#x2212; 1  )  4   + &#x22EF;
      {\displaystyle f(x)=6+4(x-1)+1(x-1)^{2}+0(x-1)^{3}+0(x-1)^{4}+\cdots \,}
      [{\displaystyle f(x)=6+4(x-1)+1(x-1)^{2}+0(x-1)^{3}+0(x-1)^{4}+\cdots
      \,}]
or indeed around any other center c.[1] One can view power series as being like
"polynomials of infinite degree," although power series are not polynomials.
The geometric_series formula
           1  1 &#x2212; x    =  &#x2211;  n = 0   &#x221E;    x  n   = 1 + x +
      x  2   +  x  3   + &#x22EF; ,   {\displaystyle {\frac {1}{1-x}}=\sum _
      {n=0}^{\infty }x^{n}=1+x+x^{2}+x^{3}+\cdots ,}  [{\displaystyle {\frac
      {1}{1-x}}=\sum _{n=0}^{\infty }x^{n}=1+x+x^{2}+x^{3}+\cdots ,}]
which is valid for      |  x  |  < 1   {\textstyle |x|<1}  [{\textstyle
|x|<1}], is one of the most important examples of a power series, as are the
exponential function formula
          e  x   =  &#x2211;  n = 0   &#x221E;      x  n    n !    = 1 + x +
      x  2    2 !    +    x  3    3 !    + &#x22EF; ,   {\displaystyle e^
      {x}=\sum _{n=0}^{\infty }{\frac {x^{n}}{n!}}=1+x+{\frac {x^{2}}{2!}}+
      {\frac {x^{3}}{3!}}+\cdots ,}  [{\displaystyle e^{x}=\sum _{n=0}^{\infty
      }{\frac {x^{n}}{n!}}=1+x+{\frac {x^{2}}{2!}}+{\frac {x^{3}}{3!}}+\cdots
      ,}]
and the sine formula
         sin &#x2061; ( x ) =  &#x2211;  n = 0   &#x221E;      ( &#x2212; 1  )
      n    x  2 n + 1     ( 2 n + 1 ) !    = x &#x2212;    x  3    3 !    +
      x  5    5 !    &#x2212;    x  7    7 !    + &#x22EF; ,   {\displaystyle
      \sin(x)=\sum _{n=0}^{\infty }{\frac {(-1)^{n}x^{2n+1}}{(2n+1)!}}=x-{\frac
      {x^{3}}{3!}}+{\frac {x^{5}}{5!}}-{\frac {x^{7}}{7!}}+\cdots ,}  [
      {\displaystyle \sin(x)=\sum _{n=0}^{\infty }{\frac {(-1)^{n}x^{2n+1}}{
      (2n+1)!}}=x-{\frac {x^{3}}{3!}}+{\frac {x^{5}}{5!}}-{\frac {x^{7}}
      {7!}}+\cdots ,}]
valid for all real x.
These power series are also examples of Taylor_series.
**** On the set of exponents[edit] ****
Negative powers are not permitted in a power series; for instance,     1 +  x
&#x2212; 1   +  x  &#x2212; 2   + &#x22EF;   {\textstyle 1+x^{-1}+x^{-2}+\cdots
}  [{\textstyle 1+x^{-1}+x^{-2}+\cdots }] is not considered a power series
(although it is a Laurent_series). Similarly, fractional powers such as      x
1 2      {\textstyle x^{\frac {1}{2}}}  [{\textstyle x^{\frac {1}{2}}}] are not
permitted (but see Puiseux_series). The coefficients      a  n     {\textstyle
a_{n}}  [{\textstyle a_{n}}] are not allowed to depend on     x   {\textstyle
x}  [{\textstyle x}], thus for instance:
         sin &#x2061; ( x ) x + sin &#x2061; ( 2 x )  x  2   + sin &#x2061; ( 3
      x )  x  3   + &#x22EF;    {\displaystyle \sin(x)x+\sin(2x)x^{2}+\sin
      (3x)x^{3}+\cdots \,}  [\sin(x) x + \sin(2x) x^2 + \sin(3x) x^3 + \cdots
      \,]
is not a power series.
***** Radius of convergence[edit] *****
A power series will converge for some values of the variable x and may diverge
for others. All power series f(x) in powers of (x − c) will converge at x = c.
(The correct value f(c) = a0 requires interpreting the expression 00 as equal
to 1.) If c is not the only convergent point, then there is always a number r
with 0 < r â¤ â such that the series converges whenever |x − c| < r and
diverges whenever |x − c| > r. The number r is called the radius_of_convergence
of the power series; in general it is given as
         r =  lim&#x2006;inf  n &#x2192; &#x221E;     |  a  n   |   &#x2212;
      1 n       {\displaystyle r=\liminf _{n\to \infty }\left|a_{n}\right|^{-
      {\frac {1}{n}}}}  [{\displaystyle r=\liminf _{n\to \infty }\left|a_
      {n}\right|^{-{\frac {1}{n}}}}]
or, equivalently,
          r  &#x2212; 1   =  lim&#x2006;sup  n &#x2192; &#x221E;     |  a  n
      |    1 n      {\displaystyle r^{-1}=\limsup _{n\to \infty }\left|a_
      {n}\right|^{\frac {1}{n}}}  [{\displaystyle r^{-1}=\limsup _{n\to \infty
      }\left|a_{n}\right|^{\frac {1}{n}}}]
(this is the CauchyâHadamard_theorem; see limit_superior_and_limit_inferior
for an explanation of the notation). The relation
          r  &#x2212; 1   =  lim  n &#x2192; &#x221E;    |    a  n + 1    a  n
      |    {\displaystyle r^{-1}=\lim _{n\to \infty }\left|{a_{n+1} \over a_
      {n}}\right|}  [{\displaystyle r^{-1}=\lim _{n\to \infty }\left|{a_{n+1}
      \over a_{n}}\right|}]
is also satisfied, if this limit exists.
The series converges_absolutely for |x â c| < r and converges_uniformly on
every compact subset of {x : |x â c| < r}. That is, the series is absolutely
and compactly_convergent on the interior of the disc of convergence.
For |x â c| = r, we cannot make any general statement on whether the series
converges or diverges. However, for the case of real variables, Abel's_theorem
states that the sum of the series is continuous at x if the series converges at
x. In the case of complex variables, we can only claim continuity along the
line segment starting at c and ending at x.
***** Operations on power series[edit] *****
**** Addition and subtraction[edit] ****
When two functions f and g are decomposed into power series around the same
center c, the power series of the sum or difference of the functions can be
obtained by termwise addition and subtraction. That is, if
         f ( x ) =  &#x2211;  n = 0   &#x221E;    a  n   ( x &#x2212; c  )  n
      {\displaystyle f(x)=\sum _{n=0}^{\infty }a_{n}(x-c)^{n}}  [{\displaystyle
      f(x)=\sum _{n=0}^{\infty }a_{n}(x-c)^{n}}] and     g ( x ) =  &#x2211;  n
      = 0   &#x221E;    b  n   ( x &#x2212; c  )  n     {\displaystyle g
      (x)=\sum _{n=0}^{\infty }b_{n}(x-c)^{n}}  [{\displaystyle g(x)=\sum _
      {n=0}^{\infty }b_{n}(x-c)^{n}}]
then
         f ( x ) &#x00B1; g ( x ) =  &#x2211;  n = 0   &#x221E;   (  a  n
      &#x00B1;  b  n   ) ( x &#x2212; c  )  n   .   {\displaystyle f(x)\pm g
      (x)=\sum _{n=0}^{\infty }(a_{n}\pm b_{n})(x-c)^{n}.}  [{\displaystyle f
      (x)\pm g(x)=\sum _{n=0}^{\infty }(a_{n}\pm b_{n})(x-c)^{n}.}]
It is not true that if two power series      &#x2211;  n = 0   &#x221E;    a  n
x  n     {\textstyle \sum _{n=0}^{\infty }a_{n}x^{n}}  [{\textstyle \sum _
{n=0}^{\infty }a_{n}x^{n}}] and      &#x2211;  n = 0   &#x221E;    b  n    x  n
{\textstyle \sum _{n=0}^{\infty }b_{n}x^{n}}  [{\textstyle \sum _{n=0}^{\infty
}b_{n}x^{n}}] have the same radius of convergence, then      &#x2211;  n = 0
&#x221E;    (   a  n   +  b  n    )   x  n     {\textstyle \sum _{n=0}^{\infty
}\left(a_{n}+b_{n}\right)x^{n}}  [{\textstyle \sum _{n=0}^{\infty }\left(a_
{n}+b_{n}\right)x^{n}}] also has this radius of convergence. If      a  n   =
( &#x2212; 1  )  n     {\textstyle a_{n}=(-1)^{n}}  [{\textstyle a_{n}=(-1)^
{n}}] and      b  n   = ( &#x2212; 1  )  n + 1    (  1 &#x2212;   1  3  n
)    {\textstyle b_{n}=(-1)^{n+1}\left(1-{\frac {1}{3^{n}}}\right)}  [
{\textstyle b_{n}=(-1)^{n+1}\left(1-{\frac {1}{3^{n}}}\right)}], then both
series have the same radius of convergence of 1, but the series      &#x2211;
n = 0   &#x221E;    (   a  n   +  b  n    )   x  n   =  &#x2211;  n = 0
&#x221E;      ( &#x2212; 1  )  n     3  n      x  n     {\textstyle \sum _
{n=0}^{\infty }\left(a_{n}+b_{n}\right)x^{n}=\sum _{n=0}^{\infty }{\frac {(-1)^
{n}}{3^{n}}}x^{n}}  [{\textstyle \sum _{n=0}^{\infty }\left(a_{n}+b_
{n}\right)x^{n}=\sum _{n=0}^{\infty }{\frac {(-1)^{n}}{3^{n}}}x^{n}}] has a
radius of convergence of 3.
**** Multiplication and division[edit] ****
With the same definitions for     f ( x )   {\displaystyle f(x)}  [f(x)] and
g ( x )   {\displaystyle g(x)}  [g(x)], the power series of the product and
quotient of the functions can be obtained as follows:
             f ( x ) g ( x )    =  (   &#x2211;  n = 0   &#x221E;    a  n   ( x
      &#x2212; c  )  n    )   (   &#x2211;  n = 0   &#x221E;    b  n   ( x
      &#x2212; c  )  n    )        =  &#x2211;  i = 0   &#x221E;    &#x2211;  j
      = 0   &#x221E;    a  i    b  j   ( x &#x2212; c  )  i + j         =
      &#x2211;  n = 0   &#x221E;    (   &#x2211;  i = 0   n    a  i    b  n
      &#x2212; i    )  ( x &#x2212; c  )  n   .       {\displaystyle {\begin
      {aligned}f(x)g(x)&=\left(\sum _{n=0}^{\infty }a_{n}(x-c)^{n}\right)\left
      (\sum _{n=0}^{\infty }b_{n}(x-c)^{n}\right)\\&=\sum _{i=0}^{\infty }\sum
      _{j=0}^{\infty }a_{i}b_{j}(x-c)^{i+j}\\&=\sum _{n=0}^{\infty }\left(\sum
      _{i=0}^{n}a_{i}b_{n-i}\right)(x-c)^{n}.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}f(x)g(x)&=\left(\sum _{n=0}^{\infty }a_{n}(x-c)^
      {n}\right)\left(\sum _{n=0}^{\infty }b_{n}(x-c)^{n}\right)\\&=\sum _
      {i=0}^{\infty }\sum _{j=0}^{\infty }a_{i}b_{j}(x-c)^{i+j}\\&=\sum _{n=0}^
      {\infty }\left(\sum _{i=0}^{n}a_{i}b_{n-i}\right)(x-c)^{n}.\end
      {aligned}}}]
The sequence      m  n   =  &#x2211;  i = 0   n    a  i    b  n &#x2212; i
{\displaystyle m_{n}=\sum _{i=0}^{n}a_{i}b_{n-i}}  [m_n = \sum_{i=0}^n a_i b_
{n-i}] is known as the convolution of the sequences      a  n
{\displaystyle a_{n}}  [a_{n}] and      b  n     {\displaystyle b_{n}}  [b_
{n}].
For division, if one defines the sequence      d  n     {\displaystyle d_{n}}
[d_{n}] by
            f ( x )   g ( x )    =     &#x2211;  n = 0   &#x221E;    a  n   ( x
      &#x2212; c  )  n      &#x2211;  n = 0   &#x221E;    b  n   ( x &#x2212; c
      )  n      =  &#x2211;  n = 0   &#x221E;    d  n   ( x &#x2212; c  )  n
      {\displaystyle {\frac {f(x)}{g(x)}}={\frac {\sum _{n=0}^{\infty }a_{n}(x-
      c)^{n}}{\sum _{n=0}^{\infty }b_{n}(x-c)^{n}}}=\sum _{n=0}^{\infty }d_{n}
      (x-c)^{n}}  [{\displaystyle {\frac {f(x)}{g(x)}}={\frac {\sum _{n=0}^
      {\infty }a_{n}(x-c)^{n}}{\sum _{n=0}^{\infty }b_{n}(x-c)^{n}}}=\sum _
      {n=0}^{\infty }d_{n}(x-c)^{n}}]
then
         f ( x ) =  (   &#x2211;  n = 0   &#x221E;    b  n   ( x &#x2212; c  )
      n    )   (   &#x2211;  n = 0   &#x221E;    d  n   ( x &#x2212; c  )  n
      )    {\displaystyle f(x)=\left(\sum _{n=0}^{\infty }b_{n}(x-c)^
      {n}\right)\left(\sum _{n=0}^{\infty }d_{n}(x-c)^{n}\right)}  [
      {\displaystyle f(x)=\left(\sum _{n=0}^{\infty }b_{n}(x-c)^{n}\right)\left
      (\sum _{n=0}^{\infty }d_{n}(x-c)^{n}\right)}]
and one can solve recursively for the terms      d  n     {\displaystyle d_{n}}
[d_{n}] by comparing coefficients.
Solving the corresponding equations yields the formulae based on determinants
of certain matrices of the coefficients of     f ( x )   {\displaystyle f(x)}
[f(x)] and     g ( x )   {\displaystyle g(x)}  [g(x)]
          d  0   =    a  0    b  0       {\displaystyle d_{0}={\frac {a_{0}}{b_
      {0}}}}  [{\displaystyle d_{0}={\frac {a_{0}}{b_{0}}}}]
          d  n   =   1  b  0   n + 1     &#x22C5; det   |     a  n      b  1
      b  2     &#x2026;    b  n        a  n &#x2212; 1      b  0      b  1
      &#x2026;    b  n &#x2212; 1        a  n &#x2212; 2     0    b  0
      &#x2026;    b  n &#x2212; 2       &#x22EE;   &#x22EE;   &#x22EE;
      &#x22F1;   &#x22EE;      a  0     0   0   &#x2026;    b  0      |
      {\displaystyle d_{n}={\frac {1}{b_{0}^{n+1}}}\cdot \det {\begin
      {vmatrix}a_{n}&b_{1}&b_{2}&\ldots &b_{n}\\a_{n-1}&b_{0}&b_{1}&\ldots &b_
      {n-1}\\a_{n-2}&0&b_{0}&\ldots &b_{n-2}\\\vdots &\vdots &\vdots &\ddots
      &\vdots \\a_{0}&0&0&\ldots &b_{0}\end{vmatrix}}}  [{\displaystyle d_{n}=
      {\frac {1}{b_{0}^{n+1}}}\cdot \det {\begin{vmatrix}a_{n}&b_{1}&b_
      {2}&\ldots &b_{n}\\a_{n-1}&b_{0}&b_{1}&\ldots &b_{n-1}\\a_{n-2}&0&b_
      {0}&\ldots &b_{n-2}\\\vdots &\vdots &\vdots &\ddots &\vdots \\a_
      {0}&0&0&\ldots &b_{0}\end{vmatrix}}}]
**** Differentiation and integration[edit] ****
Once a function     f ( x )   {\displaystyle f(x)}  [f(x)] is given as a power
series as above, it is differentiable on the interior of the domain of
convergence. It can be differentiated and integrated quite easily, by treating
every term separately:
              f  &#x2032;   ( x )    =  &#x2211;  n = 1   &#x221E;    a  n   n
      (  x &#x2212; c  )   n &#x2212; 1   =  &#x2211;  n = 0   &#x221E;    a  n
      + 1    (  n + 1  )    (  x &#x2212; c  )   n   ,     &#x222B; f ( x )  d
      x    =  &#x2211;  n = 0   &#x221E;       a  n     (  x &#x2212; c  )   n
      + 1     n + 1    + k =  &#x2211;  n = 1   &#x221E;       a  n &#x2212; 1
      (  x &#x2212; c  )   n    n   + k .       {\displaystyle {\begin
      {aligned}f^{\prime }(x)&=\sum _{n=1}^{\infty }a_{n}n\left(x-c\right)^{n-
      1}=\sum _{n=0}^{\infty }a_{n+1}\left(n+1\right)\left(x-c\right)^
      {n},\\\int f(x)\,dx&=\sum _{n=0}^{\infty }{\frac {a_{n}\left(x-c\right)^
      {n+1}}{n+1}}+k=\sum _{n=1}^{\infty }{\frac {a_{n-1}\left(x-c\right)^{n}}
      {n}}+k.\end{aligned}}}  [{\displaystyle {\begin{aligned}f^{\prime }
      (x)&=\sum _{n=1}^{\infty }a_{n}n\left(x-c\right)^{n-1}=\sum _{n=0}^
      {\infty }a_{n+1}\left(n+1\right)\left(x-c\right)^{n},\\\int f
      (x)\,dx&=\sum _{n=0}^{\infty }{\frac {a_{n}\left(x-c\right)^{n+1}}
      {n+1}}+k=\sum _{n=1}^{\infty }{\frac {a_{n-1}\left(x-c\right)^{n}}
      {n}}+k.\end{aligned}}}]
Both of these series have the same radius of convergence as the original one.
***** Analytic functions[edit] *****
Main article: Analytic_function
A function f defined on some open_subset U of R or C is called analytic if it
is locally given by a convergent power series. This means that every a â U
has an open neighborhood V â U, such that there exists a power series with
center a which converges to f(x) for every x â V.
Every power series with a positive radius of convergence is analytic on the
interior of its region of convergence. All holomorphic_functions are complex-
analytic. Sums and products of analytic functions are analytic, as are
quotients as long as the denominator is non-zero.
If a function is analytic, then it is infinitely differentiable, but in the
real case the converse is not generally true. For an analytic function, the
coefficients an can be computed as
          a  n   =     f   ( n )     ( c )    n !      {\displaystyle a_{n}=
      {\frac {f^{\left(n\right)}\left(c\right)}{n!}}}  [{\displaystyle a_{n}=
      {\frac {f^{\left(n\right)}\left(c\right)}{n!}}}]
where      f  ( n )   ( c )   {\displaystyle f^{(n)}(c)}  [f^{(n)}(c)] denotes
the nth derivative of f at c, and      f  ( 0 )   ( c ) = f ( c )
{\displaystyle f^{(0)}(c)=f(c)}  [f^{(0)}(c) = f(c)]. This means that every
analytic function is locally represented by its Taylor_series.
The global form of an analytic function is completely determined by its local
behavior in the following sense: if f and g are two analytic functions defined
on the same connected open set U, and if there exists an element câU such
that f (n)(c) = g (n)(c) for all n â¥ 0, then f(x) = g(x) for all x â U.
If a power series with radius of convergence r is given, one can consider
analytic_continuations of the series, i.e. analytic functions f which are
defined on larger sets than { x : |x â c| < r } and agree with the given
power series on this set. The number r is maximal in the following sense: there
always exists a complex_number x with |x â c| = r such that no analytic
continuation of the series can be defined at x.
The power series expansion of the inverse_function of an analytic function can
be determined using the Lagrange_inversion_theorem.
**** Behavior near the boundary[edit] ****
The sum of a power series with a positive radius of convergence is an analytic
function at every point in the interior of the disc of convergence. However,
different behavior can occur at points on the boundary of that disc. For
example:
   1. Divergence while the sum extends to an analytic function:      &#x2211;
      n = 0   &#x221E;    z  n     {\displaystyle \sum _{n=0}^{\infty }z^{n}}
      [{\displaystyle \sum _{n=0}^{\infty }z^{n}}] has radius of convergence
      equal to     1   {\displaystyle 1}  [1] and diverges at every point of
      |  z  |  = 1   {\displaystyle |z|=1}  [|z|=1]. Nevertheless, the sum in
      |  z  |  < 1   {\displaystyle |z|<1}  [|z|<1] is       1  1 &#x2212; z
      {\displaystyle {\frac {1}{1-z}}}  [{\frac  {1}{1-z}}], which is analytic
      at every point of the plane except for     z = 1   {\displaystyle z=1}
      [z=1].
   2. Convergent at some points divergent at others.:      &#x2211;  n = 1
      &#x221E;   ( &#x2212; 1  )  n + 1      z  n   n     {\displaystyle \sum _
      {n=1}^{\infty }(-1)^{n+1}{\frac {z^{n}}{n}}}  [{\displaystyle \sum _
      {n=1}^{\infty }(-1)^{n+1}{\frac {z^{n}}{n}}}] has radius of convergence
      1   {\displaystyle 1}  [1]. It converges for     z = 1   {\displaystyle
      z=1}  [z=1], while it diverges for     z = &#x2212; 1   {\displaystyle
      z=-1}  [z=-1]
   3. Absolute convergence at every point of the boundary:      &#x2211;  n = 1
      &#x221E;      z  n    n  2       {\displaystyle \sum _{n=1}^{\infty }
      {\frac {z^{n}}{n^{2}}}}  [{\displaystyle \sum _{n=1}^{\infty }{\frac {z^
      {n}}{n^{2}}}}] has radius of convergence     1   {\displaystyle 1}  [1],
      while it converges absolutely, and uniformly, at every point of      |  z
      |  = 1   {\displaystyle |z|=1}  [|z|=1] due to Weierstrass_M-test applied
      with the hyper-harmonic_convergent_series      &#x2211;  n = 1   &#x221E;
      1  n  2       {\displaystyle \sum _{n=1}^{\infty }{\frac {1}{n^{2}}}}
      [\sum _{{n=1}}^{{\infty }}{\frac  {1}{n^{2}}}].
   4. Convergent on the closure of the disc of convergence but not continuous
      sum: SierpiÅski gave an example[2] of a power series with radius of
      convergence     1   {\displaystyle 1}  [1], convergent at all points with
      |  z  |  = 1   {\displaystyle |z|=1}  [|z|=1], but the sum is an
      unbounded function and, in particular, discontinuous. A sufficient
      condition for one-sided continuity at a boundary point is given by Abel's
      theorem.
***** Formal power series[edit] *****
Main article: Formal_power_series
In abstract_algebra, one attempts to capture the essence of power series
without being restricted to the fields of real and complex numbers, and without
the need to talk about convergence. This leads to the concept of formal_power
series, a concept of great utility in algebraic_combinatorics.
***** Power series in several variables[edit] *****
An extension of the theory is necessary for the purposes of multivariable
calculus. A power series is here defined to be an infinite series of the form
         f (  x  1   , &#x2026; ,  x  n   ) =  &#x2211;   j  1   , &#x2026; ,
      j  n   = 0   &#x221E;    a   j  1   , &#x2026; ,  j  n      &#x220F;  k =
      1   n     (   x  k   &#x2212;  c  k    )    j  k     ,   {\displaystyle f
      (x_{1},\dots ,x_{n})=\sum _{j_{1},\dots ,j_{n}=0}^{\infty }a_{j_{1},\dots
      ,j_{n}}\prod _{k=1}^{n}\left(x_{k}-c_{k}\right)^{j_{k}},}  [
      {\displaystyle f(x_{1},\dots ,x_{n})=\sum _{j_{1},\dots ,j_{n}=0}^{\infty
      }a_{j_{1},\dots ,j_{n}}\prod _{k=1}^{n}\left(x_{k}-c_{k}\right)^{j_
      {k}},}]
where j = (j1, ..., jn) is a vector of natural numbers, the coefficients a(j1,
â¦, jn) are usually real or complex numbers, and the center c = (c1, ..., cn)
and argument x = (x1, ..., xn) are usually real or complex vectors. The symbol
&#x03A0;   {\displaystyle \Pi }  [\Pi ] is the product_symbol, denoting
multiplication. In the more convenient multi-index notation this can be written
         f ( x ) =  &#x2211;  &#x03B1; &#x2208;   N   n      a  &#x03B1;
      (  x &#x2212; c  )   &#x03B1;   .   {\displaystyle f(x)=\sum _{\alpha \in
      \mathbb {N} ^{n}}a_{\alpha }\left(x-c\right)^{\alpha }.}  [{\displaystyle
      f(x)=\sum _{\alpha \in \mathbb {N} ^{n}}a_{\alpha }\left(x-c\right)^
      {\alpha }.}]
where      N    {\displaystyle \mathbb {N} }  [\mathbb {N} ] is the set of
natural_numbers, and so       N   n     {\displaystyle \mathbb {N} ^{n}}
[\mathbb {N} ^{n}] is the set of ordered n-tuples of natural numbers.
The theory of such series is trickier than for single-variable series, with
more complicated regions of convergence. For instance, the power series
&#x2211;  n = 0   &#x221E;    x  1   n    x  2   n     {\displaystyle \sum _
{n=0}^{\infty }x_{1}^{n}x_{2}^{n}}  [{\displaystyle \sum _{n=0}^{\infty }x_{1}^
{n}x_{2}^{n}}] is absolutely convergent in the set     { (  x  1   ,  x  2   )
:  |   x  1    x  2    |  < 1 }   {\displaystyle \{(x_{1},x_{2}):|x_{1}x_
{2}|<1\}}  [{\displaystyle \{(x_{1},x_{2}):|x_{1}x_{2}|<1\}}] between two
hyperbolas. (This is an example of a log-convex set, in the sense that the set
of points     ( log &#x2061;  |   x  1    |  , log &#x2061;  |   x  2    |  )
{\displaystyle (\log |x_{1}|,\log |x_{2}|)}  [(\log |x_1|, \log |x_2|)], where
(  x  1   ,  x  2   )   {\displaystyle (x_{1},x_{2})}  [(x_{1},x_{2})] lies in
the above region, is a convex set. More generally, one can show that when c=0,
the interior of the region of absolute convergence is always a log-convex set
in this sense.) On the other hand, in the interior of this region of
convergence one may differentiate and integrate under the series sign, just as
one may with ordinary power series.
***** Order of a power series[edit] *****
Let Î± be a multi-index for a power series f(x1, x2, ..., xn). The order of the
power series f is defined to be the least value     r   {\displaystyle r}  [r]
such that there is aÎ± â  0 with     r =  |  &#x03B1;  |  =  &#x03B1;  1   +
&#x03B1;  2   + &#x2026; +  &#x03B1;  n     {\displaystyle r=|\alpha |=\alpha _
{1}+\alpha _{2}+\ldots +\alpha _{n}}  [{\displaystyle r=|\alpha |=\alpha _
{1}+\alpha _{2}+\ldots +\alpha _{n}}], or     &#x221E;   {\displaystyle \infty
}  [\infty ] if f â¡ 0. In particular, for a power series f(x) in a single
variable x, the order of f is the smallest power of x with a nonzero
coefficient. This definition readily extends to Laurent_series.
***** See also[edit] *****
    * Flat_function
    * Linear_approximation
    * Random_variable
    * Series_multisection
***** Notes[edit] *****
   1. ^Howard_Levi (1967). Polynomials,_Power_Series,_and_Calculus. Van
      Nostrand. p. 24.
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
   3. ^WacÅaw_SierpiÅski (1916). Sur_une_sÃ©rie_potentielle_qui,_Ã©tant
      convergente_en_tout_point_de_son_cercle_de_convergence,_reprÃ©sente_sur
      ce_cercle_une_fonction_discontinue._(French). Palermo Rend.
      pp. 187â190.
***** References[edit] *****
    * Solomentsev, E.D. (2001) [1994], "Power_series", in Hazewinkel,_Michiel
      (ed.), Encyclopedia_of_Mathematics, Springer Science+Business Media B.V.
      / Kluwer Academic Publishers, ISBN 978-1-55608-010-4
***** External links[edit] *****
    * Weisstein,_Eric_W. "Formal_Power_Series". MathWorld.
Weisstein,_Eric_W. "Power_Series". MathWorld.
Powers_of_Complex_Numbers by Michael Schreiber, Wolfram_Demonstrations_Project.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Power_series&oldid=906973309"
Categories:
    * Real_analysis
    * Complex_analysis
    * Multivariable_calculus
    * Mathematical_series
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AzÉrbaycanca
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * ä¸­æ
Edit_links
    * This page was last edited on 19 July 2019, at 15:37 (UTC).
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
