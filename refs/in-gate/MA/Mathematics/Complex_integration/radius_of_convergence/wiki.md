The following text has been accessed from https://en.wikipedia.org/wiki/Radius_of_convergence at Fri Aug 9 02:37:28 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Radius of convergence ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, the radius of convergence of a power_series is the radius of
the largest disk in which the series converges. It is either a non-negative
real number or     &#x221E;   {\displaystyle \infty }  [\infty ]. When it is
positive, the power series converges_absolutely and uniformly_on_compact_sets
inside the open disk of radius equal to the radius of convergence, and it is
the Taylor_series of the analytic_function to which it converges.
⁰
***** Contents *****
    * 1_Definition
    * 2_Finding_the_radius_of_convergence
          o 2.1_Theoretical_radius
          o 2.2_Practical_estimation_of_radius_in_the_case_of_real_coefficients
    * 3_Radius_of_convergence_in_complex_analysis
          o 3.1_A_simple_example
          o 3.2_A_more_complicated_example
    * 4_Convergence_on_the_boundary
    * 5_Rate_of_convergence
    * 6_Abscissa_of_convergence_of_a_Dirichlet_series
    * 7_Notes
    * 8_References
    * 9_External_links
***** Definition[edit] *****
For a power series Æ defined as:
         f ( z ) =  &#x2211;  n = 0   &#x221E;    c  n   ( z &#x2212; a  )  n
      ,   {\displaystyle f(z)=\sum _{n=0}^{\infty }c_{n}(z-a)^{n},}  [f(z) =
      \sum_{n=0}^\infty c_n (z-a)^n, ]
where
      a is a complex constant, the center of the disk of convergence,
      cn is the nth complex coefficient, and
      z is a complex variable.
The radius of convergence r is a nonnegative real number or     &#x221E;
{\displaystyle \infty }  [\infty ] such that the series converges if
          |  z &#x2212; a  |  < r    {\displaystyle |z-a|<r\,}  [|z-a| < r\,]
and diverges if
          |  z &#x2212; a  |  > r .    {\displaystyle |z-a|>r.\,}  [|z-a| >
      r.\,]
Some may prefer an alternative definition, as existence is obvious:
         r = sup  {   |  z &#x2212; a  |  &#xA0;  |  &#xA0;  &#x2211;  n = 0
      &#x221E;    c  n   ( z &#x2212; a  )  n   &#xA0;  &#xA0;converges&#xA0;
      }    {\displaystyle r=\sup \left\{|z-a|\ \left|\ \sum _{n=0}^{\infty }c_
      {n}(z-a)^{n}\ {\text{ converges }}\right.\right\}}  [{\displaystyle
      r=\sup \left\{|z-a|\ \left|\ \sum _{n=0}^{\infty }c_{n}(z-a)^{n}\ {\text
      { converges }}\right.\right\}}]
On the boundary, that is, where |z − a| = r, the behavior of the power series
may be complicated, and the series may converge for some values of z and
diverge for others. The radius of convergence is infinite if the series
converges for all complex_numbers z.[1]
***** Finding the radius of convergence[edit] *****
Two cases arise. The first case is theoretical: when you know all the
coefficients      c  n     {\displaystyle c_{n}}  [c_{n}] then you take certain
limits and find the precise radius of convergence. The second case is
practical: when you construct a power series solution of a difficult problem
you typically will only know a finite number of terms in a power series,
anywhere from a couple of terms to a hundred terms. In this second case,
extrapolating a plot estimates the radius of convergence.
**** Theoretical radius[edit] ****
The radius of convergence can be found by applying the root_test to the terms
of the series. The root test uses the number
         C =  lim&#x2006;sup  n &#x2192; &#x221E;       |   c  n   ( z &#x2212;
      a  )  n    |    n    =  lim&#x2006;sup  n &#x2192; &#x221E;       |   c
      n    |    n     |  z &#x2212; a  |    {\displaystyle C=\limsup _
      {n\rightarrow \infty }{\sqrt[{n}]{|c_{n}(z-a)^{n}|}}=\limsup _
      {n\rightarrow \infty }{\sqrt[{n}]{|c_{n}|}}|z-a|}  [C = \limsup_
      {n\rightarrow\infty}\sqrt[n]{|c_n(z-a)^n|} = \limsup_
      {n\rightarrow\infty}\sqrt[n]{|c_n|}|z-a|]
"lim sup" denotes the limit_superior. The root test states that the series
converges if C < 1 and diverges if C > 1. It follows that the power series
converges if the distance from z to the center a is less than
         r =   1   lim&#x2006;sup  n &#x2192; &#x221E;       |   c  n    |    n
      {\displaystyle r={\frac {1}{\limsup _{n\rightarrow \infty }{\sqrt[{n}]
      {|c_{n}|}}}}}  [r = \frac{1}{\limsup_{n\rightarrow\infty}\sqrt[n]
      {|c_n|}}]
and diverges if the distance exceeds that number; this statement is the
CauchyâHadamard_theorem. Note that r = 1/0 is interpreted as an infinite
radius, meaning that Æ is an entire_function.
The limit involved in the ratio_test is usually easier to compute, and when
that limit exists, it shows that the radius of convergence is finite.
         r =  lim  n &#x2192; &#x221E;    |    c  n    c  n + 1     |  .
      {\displaystyle r=\lim _{n\rightarrow \infty }\left|{\frac {c_{n}}{c_
      {n+1}}}\right|.}  [{\displaystyle r=\lim _{n\rightarrow \infty }\left|
      {\frac {c_{n}}{c_{n+1}}}\right|.}]
This is shown as follows. The ratio test says the series converges if
          lim  n &#x2192; &#x221E;       |   c  n + 1   ( z &#x2212; a  )  n +
      1    |     |   c  n   ( z &#x2212; a  )  n    |     < 1.   {\displaystyle
      \lim _{n\to \infty }{\frac {|c_{n+1}(z-a)^{n+1}|}{|c_{n}(z-a)^{n}|}}<1.}
      [ \lim_{n\to\infty} \frac{|c_{n+1}(z-a)^{n+1}|}{|c_n(z-a)^n|} < 1. ]
That is equivalent to
          |  z &#x2212; a  |  <   1   lim  n &#x2192; &#x221E;       |   c  n +
      1    |     |   c  n    |        =  lim  n &#x2192; &#x221E;    |    c  n
      c  n + 1     |  .   {\displaystyle |z-a|<{\frac {1}{\lim _{n\to \infty }
      {\frac {|c_{n+1}|}{|c_{n}|}}}}=\lim _{n\to \infty }\left|{\frac {c_{n}}
      {c_{n+1}}}\right|.}  [ |z - a| < \frac{1}{\lim_{n\to\infty} \frac{|c_
      {n+1}|}{|c_n|}} = \lim_{n\to\infty} \left|\frac{c_n}{c_{n+1}}\right|. ]
**** Practical estimation of radius in the case of real coefficients[edit] ****
DombâSykes plot of the function     f ( &#x03B5; ) =    &#x03B5; ( 1 +
&#x03B5;  3   )   1 + 2 &#x03B5;    .   {\displaystyle f(\varepsilon )={\frac
{\varepsilon (1+\varepsilon ^{3})}{\sqrt {1+2\varepsilon }}}.}  [f
(\varepsilon)=\frac{\varepsilon(1+\varepsilon^3)}{\sqrt{1+2\varepsilon}}.][2]
On the left (a) is a straightforward plot of the ratio of the power-series
coefficients      c  n &#x2212; 1    /   c  n     {\displaystyle c_{n-1}/c_{n}}
[{\displaystyle c_{n-1}/c_{n}}] as a function of index     n   {\displaystyle
n}  [n]; on the right, (b) is the DombâSykes plot of      c  n    /   c  n
&#x2212; 1     {\displaystyle c_{n}/c_{n-1}}  [c_{n}/c_{{n-1}}] as a function
of     1  /  n   {\displaystyle 1/n}  [1/n]. The solid green line is the
straight-line asymptote in the DombâSykes plot, which intercepts the vertical
axis at â2 and has a slope +1. Thus there is a singularity at     &#x03B5; =
&#x2212; 1  /  2   {\displaystyle \varepsilon =-1/2}  [{\displaystyle
\varepsilon =-1/2}] and so the radius of convergence is     r = 1  /  2.
{\displaystyle r=1/2.}  [{\displaystyle r=1/2.}]
Usually, in scientific applications, only a finite number of coefficients
c  n     {\displaystyle c_{n}}  [c_{n}] are known. Typically,[vague] as     n
{\displaystyle n}  [n] increases, these coefficients settle into a regular
behavior determined by the nearest radius-limiting singularity. In this case,
two main techniques have been developed, based on the fact that the
coefficients of a Taylor series are roughly exponential with ratio     1  /  r
{\displaystyle 1/r}  [1/r] where r is the radius of convergence.
    * The basic case is when the coefficients ultimately share a common sign or
      alternate in sign. As pointed out earlier in the article, in many cases
      the limit      lim  n &#x2192; &#x221E;      c  n     /    c  n &#x2212;
      1       {\displaystyle \lim _{n\to \infty }{{c_{n}}/{c_{n-1}}}}  [
      {\displaystyle \lim _{n\to \infty }{{c_{n}}/{c_{n-1}}}}] exists, and in
      this case      1   /   r  =  lim  n &#x2192; &#x221E;      c  n     /
      c  n &#x2212; 1     .   {\displaystyle {1}/{r}=\lim _{n\to \infty }{{c_
      {n}}/{c_{n-1}}}.}  [{\displaystyle {1}/{r}=\lim _{n\to \infty }{{c_{n}}/
      {c_{n-1}}}.}] Negative     r   {\displaystyle r}  [r] means the
      convergence-limiting singularity is on the negative axis. Estimate this
      limit, by plotting the      c  n    /   c  n &#x2212; 1
      {\displaystyle c_{n}/c_{n-1}}  [c_{n}/c_{{n-1}}] versus     1  /  n
      {\displaystyle 1/n}  [1/n], and graphically extrapolate to     1  /  n =
      0   {\displaystyle 1/n=0}  [1/n=0] (effectively     n = &#x221E;
      {\displaystyle n=\infty }  [n=\infty ]) via a linear fit. The intercept
      with     1  /  n = 0   {\displaystyle 1/n=0}  [1/n=0] estimates the
      reciprocal of the radius of convergence,     1  /  r   {\displaystyle 1/
      r}  [1/r]. This plot is called a DombâSykes plot.
    * The more complicated case is when the signs of the coefficients have a
      more complex pattern. Mercer and Roberts proposed the following
      procedure.[3] Define the associated sequence
                b  n   2   =     c  n + 1    c  n &#x2212; 1   &#x2212;  c  n
            2      c  n    c  n &#x2212; 2   &#x2212;  c  n &#x2212; 1   2
            n = 3 , 4 , 5 , &#x2026; .   {\displaystyle b_{n}^{2}={\frac {c_
            {n+1}c_{n-1}-c_{n}^{2}}{c_{n}c_{n-2}-c_{n-1}^{2}}}\quad
            n=3,4,5,\ldots .}  [{\displaystyle b_{n}^{2}={\frac {c_{n+1}c_{n-
            1}-c_{n}^{2}}{c_{n}c_{n-2}-c_{n-1}^{2}}}\quad n=3,4,5,\ldots .}]
      Plot the finitely many known      b  n     {\displaystyle b_{n}}  [b_{n}]
      versus     1  /  n   {\displaystyle 1/n}  [1/n], and graphically
      extrapolate to     1  /  n = 0   {\displaystyle 1/n=0}  [1/n=0] via a
      linear fit.
The intercept with     1  /  n = 0   {\displaystyle 1/n=0}  [1/n=0] estimates
the reciprocal of the radius of convergence,     1  /  r   {\displaystyle 1/r}
[1/r].
      This procedure also estimates two other characteristics of the
      convergence limiting singularity. Suppose the nearest singularity is of
      degree     p   {\displaystyle p}  [p] and has angle     &#x00B1; &#x03B8;
      {\displaystyle \pm \theta }  [{\displaystyle \pm \theta }] to the real
      axis. Then the slope of the linear fit given above is     &#x2212; ( p +
      1 )  /  r   {\displaystyle -(p+1)/r}  [{\displaystyle -(p+1)/r}].
      Further, plot       1 2    (      c  n &#x2212; 1    b  n     c  n     +
      c  n + 1     c  n    b  n       )    {\displaystyle {\frac {1}{2}}\left(
      {\frac {c_{n-1}b_{n}}{c_{n}}}+{\frac {c_{n+1}}{c_{n}b_{n}}}\right)}  [
      {\displaystyle {\frac {1}{2}}\left({\frac {c_{n-1}b_{n}}{c_{n}}}+{\frac
      {c_{n+1}}{c_{n}b_{n}}}\right)}] versus     1  /   n  2     {\displaystyle
      1/n^{2}}  [1/n^{2}], then a linear fit extrapolated to     1  /   n  2
      = 0   {\displaystyle 1/n^{2}=0}  [{\displaystyle 1/n^{2}=0}] has
      intercept at     cos &#x2061; &#x03B8;   {\displaystyle \cos \theta }
      [\cos \theta ].
***** Radius of convergence in complex analysis[edit] *****
A power series with a positive radius of convergence can be made into a
holomorphic_function by taking its argument to be a complex variable. The
radius of convergence can be characterized by the following theorem:
      The radius of convergence of a power series Æ centered on a point a is
      equal to the distance from a to the nearest point where Æ cannot be
      defined in a way that makes it holomorphic.
The set of all points whose distance to a is strictly less than the radius of
convergence is called the disk of convergence.
A graph of the functions explained in the text: Approximations in blue, circle
of convergence in white
The nearest point means the nearest point in the complex_plane, not necessarily
on the real line, even if the center and all coefficients are real. For
example, the function
         f ( z ) =   1  1 +  z  2        {\displaystyle f(z)={\frac {1}{1+z^
      {2}}}}  [{\displaystyle f(z)={\frac {1}{1+z^{2}}}}]
has no singularities on the real line, since     1 +  z  2     {\displaystyle
1+z^{2}}  [1+z^2] has no real roots. Its Taylor series about 0 is given by
          &#x2211;  n = 0   &#x221E;   ( &#x2212; 1  )  n    z  2 n   .
      {\displaystyle \sum _{n=0}^{\infty }(-1)^{n}z^{2n}.}  [\sum_{n=0}^\infty
      (-1)^n z^{2n}.]
The root test shows that its radius of convergence is 1. In accordance with
this, the function ƒ(z) has singularities at Â±i, which are at a distance 1
from 0.
For a proof of this theorem, see analyticity_of_holomorphic_functions.
**** A simple example[edit] ****
The arctangent function of trigonometry can be expanded in a power series:
         arctan &#x2061; ( z ) = z &#x2212;    z  3   3   +    z  5   5
      &#x2212;    z  7   7   + &#x22EF; .   {\displaystyle \arctan(z)=z-{\frac
      {z^{3}}{3}}+{\frac {z^{5}}{5}}-{\frac {z^{7}}{7}}+\cdots .}  [
      {\displaystyle \arctan(z)=z-{\frac {z^{3}}{3}}+{\frac {z^{5}}{5}}-{\frac
      {z^{7}}{7}}+\cdots .}]
It is easy to apply the root test in this case to find that the radius of
convergence is 1.
**** A more complicated example[edit] ****
Consider this power series:
           z   e  z   &#x2212; 1    =  &#x2211;  n = 0   &#x221E;      B  n
      n !     z  n     {\displaystyle {\frac {z}{e^{z}-1}}=\sum _{n=0}^{\infty
      }{\frac {B_{n}}{n!}}z^{n}}  [{\displaystyle {\frac {z}{e^{z}-1}}=\sum _
      {n=0}^{\infty }{\frac {B_{n}}{n!}}z^{n}}]
where the rational numbers Bn are the Bernoulli_numbers. It may be cumbersome
to try to apply the ratio test to find the radius of convergence of this
series. But the theorem of complex analysis stated above quickly solves the
problem. At z = 0, there is in effect no singularity since the_singularity_is
removable. The only non-removable singularities are therefore located at the
other points where the denominator is zero. We solve
          e  z   &#x2212; 1 = 0    {\displaystyle e^{z}-1=0\,}  [e^z-1=0\,]
by recalling that if z = x + iy and e iy = cos(y) + i sin(y) then
          e  z   =  e  x    e  i y   =  e  x   ( cos &#x2061; ( y ) + i sin
      &#x2061; ( y ) ) ,    {\displaystyle e^{z}=e^{x}e^{iy}=e^{x}(\cos
      (y)+i\sin(y)),\,}  [e^z = e^x e^{iy} = e^x(\cos(y)+i\sin(y)),\,]
and then take x and y to be real. Since y is real, the absolute value of cos
(y) + i sin(y) is necessarily 1. Therefore, the absolute value of e z can be 1
only if e x is 1; since x is real, that happens only if x = 0. Therefore z is
pure imaginary and cos(y) + i sin(y) = 1. Since y is real, that happens only if
cos(y) = 1 and sin(y) = 0, so that y is an integer multiple of 2Ï.
Consequently the singular points of this function occur at
      z = a nonzero integer multiple of 2Ïi.
The singularities nearest 0, which is the center of the power series expansion,
are at Â±2Ïi. The distance from the center to either of those points is 2Ï,
so the radius of convergence is 2Ï.
***** Convergence on the boundary[edit] *****
If the power series is expanded around the point a and the radius of
convergence is r, then the set of all points z such that |z â a| = r is a
circle called the boundary of the disk of convergence. A power series may
diverge at every point on the boundary, or diverge on some points and converge
at other points, or converge at all the points on the boundary. Furthermore,
even if the series converges everywhere on the boundary (even uniformly), it
does not necessarily converge absolutely.
Example 1: The power series for the function Æ(z) = 1/(1 â z), expanded
around z = 0, which is simply
          &#x2211;  n = 0   &#x221E;    z  n   ,   {\displaystyle \sum _{n=0}^
      {\infty }z^{n},}  [ \sum_{n=0}^\infty z^n,]
has radius of convergence 1 and diverges at every point on the boundary.
Example 2: The power series for g(z) = âln(1 â z), expanded around z = 0,
which is
          &#x2211;  n = 1   &#x221E;     1 n    z  n   ,   {\displaystyle \sum
      _{n=1}^{\infty }{\frac {1}{n}}z^{n},}  [ \sum_{n=1}^\infty \frac{1}{n}
      z^n,]
has radius of convergence 1, and diverges for z = 1 but converges for all other
points on the boundary. The function Æ(z) of Example 1 is the derivative of g
(z).
Example 3: The power series
          &#x2211;  n = 1   &#x221E;     1  n  2      z  n     {\displaystyle
      \sum _{n=1}^{\infty }{\frac {1}{n^{2}}}z^{n}}  [{\displaystyle \sum _
      {n=1}^{\infty }{\frac {1}{n^{2}}}z^{n}}]
has radius of convergence 1 and converges everywhere on the boundary
absolutely. If h is the function represented by this series on the unit disk,
then the derivative of h(z) is equal to g(z)/z with g of Example 2. It turns
out that h(z) is the dilogarithm function.
Example 4: The power series
          &#x2211;  i = 1   &#x221E;    a  i    z  i    &#xA0;where&#xA0;   a
      i   =    ( &#x2212; 1  )  n &#x2212; 1      2  n   n     &#xA0;for&#xA0;
      n = &#x230A;  log  2   &#x2061; ( i ) &#x230B; + 1  , the unique integer
      with&#xA0;   2  n &#x2212; 1   &#x2264; i <  2  n   ,   {\displaystyle
      \sum _{i=1}^{\infty }a_{i}z^{i}{\text{ where }}a_{i}={\frac {(-1)^{n-1}}
      {2^{n}n}}{\text{ for }}n=\lfloor \log _{2}(i)\rfloor +1{\text{, the
      unique integer with }}2^{n-1}\leq i<2^{n},}  [{\displaystyle \sum _{i=1}^
      {\infty }a_{i}z^{i}{\text{ where }}a_{i}={\frac {(-1)^{n-1}}{2^{n}n}}
      {\text{ for }}n=\lfloor \log _{2}(i)\rfloor +1{\text{, the unique integer
      with }}2^{n-1}\leq i<2^{n},}]
has radius of convergence 1 and converges uniformly on the entire boundary z,
but does not converge_absolutely on the boundary.[4]
***** Rate of convergence[edit] *****
If we expand the function
         f ( x ) = sin &#x2061; x =  &#x2211;  n = 0   &#x221E;      ( &#x2212;
      1  )  n     ( 2 n + 1 ) !     x  2 n + 1   = x &#x2212;    x  3    3 !
      +    x  5    5 !    &#x2212; &#x22EF;  &#xA0;for all&#xA0;  x
      {\displaystyle f(x)=\sin x=\sum _{n=0}^{\infty }{\frac {(-1)^{n}}{
      (2n+1)!}}x^{2n+1}=x-{\frac {x^{3}}{3!}}+{\frac {x^{5}}{5!}}-\cdots {\text
      { for all }}x}  [f(x)=\sin x = \sum^{\infin}_{n=0} \frac{(-1)^n}{(2n+1)!}
      x^{2n+1} =  x - \frac{x^3}{3!} + \frac{x^5}{5!} - \cdots\text{ for all }
      x]
around the point x = 0, we find out that the radius of convergence of this
series is      &#x221E;    {\displaystyle \scriptstyle \infty }
[\scriptstyle\infty] meaning that this series converges for all complex
numbers. However, in applications, one is often interested in the precision of
a numerical_answer. Both the number of terms and the value at which the series
is to be evaluated affect the accuracy of the answer. For example, if we want
to calculate f(0.1) = sin(0.1) accurate up to five decimal places, we only need
the first two terms of the series. However, if we want the same precision for x
= 1 we must evaluate and sum the first five terms of the series. For f(10), one
requires the first 18 terms of the series, and for f(100) we need to evaluate
the first 141 terms.
So the fastest convergence of a power series expansion is at the center, and as
one moves away from the center of convergence, the rate_of_convergence slows
down until you reach the boundary (if it exists) and cross over, in which case
the series will diverge.
***** Abscissa of convergence of a Dirichlet series[edit] *****
An analogous concept is the abscissa of convergence of a Dirichlet_series
          &#x2211;  n = 1   &#x221E;      a  n    n  s     .   {\displaystyle
      \sum _{n=1}^{\infty }{a_{n} \over n^{s}}.}  [\sum_{n=1}^\infty {a_n \over
      n^s}.]
Such a series converges if the real part of s is greater than a particular
number depending on the coefficients an: the abscissa of convergence.
***** Notes[edit] *****
   1. ^Mathematical_Analysis-II. Krishna Prakashan Media.
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
   3. ^ See Figure 8.1 in:Hinch, E.J. (1991), Perturbation Methods, Cambridge
      Texts in Applied Mathematics, 6, Cambridge University Press, p. 146,
      ISBN 0-521-37897-4
   4. ^Mercer, G.N.; Roberts, A.J. (1990), "A centre manifold description of
      contaminant dispersion in channels with varying flow properties", SIAM J.
      Appl. Math., 50 (6): 1547â1565, doi:10.1137/0150091
   5. ^SierpiÅski,_WacÅaw (1918), "O szeregu potÄgowym ktÃ³ry jest zbieÅ¼ny
      na caÅem swem kole zbieÅ¼noÅci jednostajnie ale nie bezwzglÄdnie",
      Prace matematyka-fizyka, 29, pp. 263â266
***** References[edit] *****
    * Brown, James; Churchill, Ruel (1989), Complex variables and applications,
      New York: McGraw-Hill, ISBN 978-0-07-010905-6
Stein,_Elias; Shakarchi, Rami (2003), Complex Analysis, Princeton, New Jersey:
Princeton_University_Press, ISBN 0-691-11385-8
***** External links[edit] *****
    * What_is_radius_of_convergence?

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Radius_of_convergence&oldid=909470868"
Categories:
    * Analytic_functions
    * Convergence_(mathematics)
    * Mathematical_physics
    * Theoretical_physics
Hidden categories:
    * All_Wikipedia_articles_needing_clarification
    * Wikipedia_articles_needing_clarification_from_April_2014
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
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * Italiano
    * æ¥æ¬èª
    * Norsk_nynorsk
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 5 August 2019, at 17:10 (UTC).
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
