The following text has been accessed from https://en.wikipedia.org/wiki/Legendre_polynomials at Fri Aug 9 00:00:39 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Legendre polynomials ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For Legendre's Homogeneous equation, see Legendre's_equation.
      The six first Legendre polynomials.
In physical science and mathematics, Legendre polynomials (named after Adrien-
Marie_Legendre, who discovered them in 1782) are a system of complete and
orthogonal_polynomials, with a vast number of mathematically beautiful
properties, and numerous applications. They can be defined in many ways, and
the various definitions highlight different aspects as well as suggest
generalizations and connections to different mathematical structures and
physical and numerical applications.
Closely related to the Legendre polynomials are associated_Legendre
polynomials, Legendre_functions, Legendre functions of the second kind, and
associated_Legendre_functions.
⁰
***** Contents *****
    * 1_Definition_by_construction_as_an_orthogonal_system
    * 2_Definition_via_generating_function
    * 3_Definition_via_differential_equation
    * 4_Orthonormality_and_completeness
    * 5_Rodrigues'_formula_and_other_explicit_formulas
    * 6_Applications_of_Legendre_polynomials
          o 6.1_Expanding_a_1/r_potential
          o 6.2_Legendre_polynomials_in_multipole_expansions
          o 6.3_Legendre_polynomials_in_trigonometry
    * 7_Additional_properties_of_Legendre_polynomials
          o 7.1_Recursion_relations
          o 7.2_Asymptotes
          o 7.3_Zeros
          o 7.4_Pointwise_evaluations
    * 8_Legendre_polynomials_with_transformed_argument
          o 8.1_Shifted_Legendre_polynomials
          o 8.2_Legendre_rational_functions
    * 9_See_also
    * 10_Notes
    * 11_References
    * 12_External_links
***** Definition by construction as an orthogonal system[edit] *****
In this approach, the polynomials are defined as an orthogonal system with
respect to the weight function     w ( x ) = 1   {\displaystyle w(x)=1}  [w
(x)=1] over the interval     [ &#x2212; 1 , 1 ]   {\displaystyle [-1,1]}  [
{\displaystyle [-1,1]}]. That is,      P  n   ( x )   {\displaystyle P_{n}(x)}
[P_n(x)] is a polynomial of degree     n   {\displaystyle n}  [n], such that
          &#x222B;  &#x2212; 1   1    P  m   ( x )  P  n   ( x )  d x = 0
      if&#xA0;  n &#x2260; m .   {\displaystyle \int _{-1}^{1}P_{m}(x)P_{n}
      (x)\,dx=0\quad {\text{if }}n\neq m.}  [{\displaystyle \int _{-1}^{1}P_{m}
      (x)P_{n}(x)\,dx=0\quad {\text{if }}n\neq m.}]
This determines the polynomials completely up to an overall scale factor, which
is fixed by the standardization      P  n   ( 1 ) = 1   {\displaystyle P_{n}
(1)=1}  [{\displaystyle P_{n}(1)=1}]. That this is a constructive definition is
seen thus:      P  0   ( x ) = 1   {\displaystyle P_{0}(x)=1}  [{\displaystyle
P_{0}(x)=1}] is the only correctly standardized polynomial of degree 0.      P
1   ( x )   {\displaystyle P_{1}(x)}  [P_{1}(x)] must be orthogonal to      P
0     {\displaystyle P_{0}}  [P_{0}], leading to      P  1   ( x ) = x
{\displaystyle P_{1}(x)=x}  [{\displaystyle P_{1}(x)=x}], and      P  2   ( x )
{\displaystyle P_{2}(x)}  [P_{2}(x)] is determined by demanding orthogonality
to      P  0     {\displaystyle P_{0}}  [P_{0}] and      P  1
{\displaystyle P_{1}}  [P_{1}], and so on.      P  n     {\displaystyle P_{n}}
[P_{n}] is fixed by demanding orthogonality to all      P  m     {\displaystyle
P_{m}}  [P_m] with     m < n   {\displaystyle m<n}  [ m < n ]. This gives     n
{\displaystyle n}  [n] conditions, which, along with the standardization      P
n   ( 1 ) = 1   {\displaystyle P_{n}(1)=1}  [{\displaystyle P_{n}(1)=1}] fixes
all     n + 1   {\displaystyle n+1}  [{\displaystyle n+1}] coefficients in
P  n   ( x )   {\displaystyle P_{n}(x)}  [{\displaystyle P_{n}(x)}]. With work,
all the coefficients of every polynomial can be systematically determined,
leading to the explicit representation in powers of     x   {\displaystyle x}
[x] given below.
This definition of the      P  n     {\displaystyle P_{n}}  [P_{n}]'s is the
simplest one. It does not appeal to the theory of differential equations.
Second, the completeness of the polynomials follows immediately from the
completeness of the powers 1,     x ,  x  2   ,  x  3   , &#x2026;
{\displaystyle x,x^{2},x^{3},\ldots }  [{\displaystyle x,x^{2},x^{3},\ldots }].
Finally, by defining them via orthogonality with respect to the most obvious
weight function on a finite interval, it sets up the Legendre polynomials as
one of the three classical_orthogonal_polynomial_systems. The other two are the
Laguerre_polynomials, which are orthogonal over the half line     [ 0 ,
&#x221E; )   {\displaystyle [0,\infty )}  [[0,\infty )], and the Hermite
polynomials, orthogonal over the full line     ( &#x2212; &#x221E; , &#x221E; )
{\displaystyle (-\infty ,\infty )}  [(-\infty ,\infty )], with weight functions
that are the most natural analytic functions that ensure convergence of all
integrals.
***** Definition via generating function[edit] *****
The Legendre polynomials can also be defined as the coefficients in a formal
expansion in powers of     t   {\displaystyle t}  [t] of the generating
function[1]
           1  1 &#x2212; 2 x t +  t  2      =  &#x2211;  n = 0
      &#x221E;    P  n   ( x )  t  n    .   {\displaystyle {\frac {1}    
      {\sqrt {1-2xt+t^{2}}}}=\sum _{n=0}^{\infty }P_{n}(x)t^{n}\,.}        (2)
      [{\displaystyle {\frac {1}{\sqrt {1-2xt+t^{2}}}}=\sum _{n=0}^
      {\infty }P_{n}(x)t^{n}\,.}]
The coefficient of      t  n     {\displaystyle t^{n}}  [t^{n}] is a polynomial
in     x   {\displaystyle x}  [x] of degree     n   {\displaystyle n}  [n].
Expanding up to      t  1     {\displaystyle t^{1}}  [{\displaystyle t^{1}}]
gives
          P  0   ( x ) = 1  ,   P  1   ( x ) = x .   {\displaystyle P_{0}
      (x)=1\,,\quad P_{1}(x)=x.}  [{\displaystyle P_{0}(x)=1\,,\quad P_{1}
      (x)=x.}]
Expansion to higher orders gets increasingly cumbersome, but is possible to do
systematically, and again leads to one of the explicit forms given below.
It is possible to obtain the higher      P  n     {\displaystyle P_{n}}  [P_
{n}]'s without resorting to direct expansion of the Taylor series, however.
Eq. 2 is differentiated with respect to t on both sides and rearranged to
obtain
            x &#x2212; t   1 &#x2212; 2 x t +  t  2      =  (  1 &#x2212; 2 x t
      +  t  2    )   &#x2211;  n = 1   &#x221E;   n  P  n   ( x )  t  n
      &#x2212; 1    .   {\displaystyle {\frac {x-t}{\sqrt {1-2xt+t^{2}}}}=\left
      (1-2xt+t^{2}\right)\sum _{n=1}^{\infty }nP_{n}(x)t^{n-1}\,.}  [
      {\displaystyle {\frac {x-t}{\sqrt {1-2xt+t^{2}}}}=\left(1-2xt+t^
      {2}\right)\sum _{n=1}^{\infty }nP_{n}(x)t^{n-1}\,.}]
Replacing the quotient of the square root with its definition in Eq. 2, and
equating_the_coefficients of powers of t in the resulting expansion gives
Bonnetâs recursion formula
         ( n + 1 )  P  n + 1   ( x ) = ( 2 n + 1 ) x  P  n   ( x ) &#x2212; n
      P  n &#x2212; 1   ( x )  .   {\displaystyle (n+1)P_{n+1}(x)=(2n+1)xP_{n}
      (x)-nP_{n-1}(x)\,.}  [{\displaystyle (n+1)P_{n+1}(x)=(2n+1)xP_{n}(x)-nP_
      {n-1}(x)\,.}]
This relation, along with the first two polynomials P0 and P1, allows all the
rest to be generated recursively.
The generating function approach is directly connected to the multipole
expansion in electrostatics, as explained below, and is how the polynomials
were first defined by Legendre in 1782.
***** Definition via differential equation[edit] *****
A third definition is in terms of solutions to Legendre's differential_equation
           d  d x     [   (  1 &#x2212;  x  2    )     d  P  n   ( x
      )   d x     ]  + n ( n + 1 )  P  n   ( x ) = 0  .
      {\displaystyle {\frac {d}{dx}}\left[\left(1-x^{2}\right){\frac     (1)
      {dP_{n}(x)}{dx}}\right]+n(n+1)P_{n}(x)=0\,.}  [{\displaystyle      
      {\frac {d}{dx}}\left[\left(1-x^{2}\right){\frac {dP_{n}(x)}
      {dx}}\right]+n(n+1)P_{n}(x)=0\,.}]
This differential equation has regular_singular_points at x = Â±1 so if a
solution is sought using the standard Frobenius or power_series method, a
series about the origin will only converge for |x| < 1 in general. When n is an
integer, the solution Pn(x) that is regular at x = 1 is also regular at x =
â1, and the series for this solution terminates (i.e. it is a polynomial).
The orthogonality and completeness of these solutions is best seen from the
viewpoint of SturmâLiouville_theory. We rewrite the differential equation as
an eigenvalue problem,
           d  d x     (   (  1 &#x2212;  x  2    )    d  d x     )  P ( x ) =
      &#x2212; &#x03BB; P ( x )  ,   {\displaystyle {\frac {d}{dx}}\left(\left
      (1-x^{2}\right){\frac {d}{dx}}\right)P(x)=-\lambda P(x)\,,}  [
      {\displaystyle {\frac {d}{dx}}\left(\left(1-x^{2}\right){\frac {d}
      {dx}}\right)P(x)=-\lambda P(x)\,,}]
with the eigenvalue     &#x03BB;   {\displaystyle \lambda }  [\lambda ] in lieu
of     n ( n + 1 )   {\displaystyle n(n+1)}  [{\displaystyle n(n+1)}]. If we
demand that the solution be regular at     x = &#x00B1; 1   {\displaystyle
x=\pm 1}  [x=\pm 1], the differential_operator on the left is Hermitean. The
eigenvalues are found to be of the form n(n + 1), with     n = 0 , 1 , 2 ,
&#x2026;   {\displaystyle n=0,1,2,\ldots }  [{\displaystyle n=0,1,2,\ldots }],
and the eigenfunctions are the      P  n   ( x )   {\displaystyle P_{n}(x)}
[P_n(x)]. The orthogonality and completeness of this set of solutions follows
at once from the larger framework of SturmâLiouville theory.
The differential equation admits another, non-polynomial solution, the Legendre
functions of the second kind      Q  n     {\displaystyle Q_{n}}  [Q_{n}]. A
two-parameter generalization of (Eq. 1) is called Legendre's general
differential equation, solved by the Associated_Legendre_polynomials. Legendre
functions are solutions of Legendre's differential equation (generalized or
not) with non-integer parameters.
In physical settings, Legendre's differential equation arises naturally
whenever one solves Laplace's_equation (and related partial_differential
equations) by separation of variables in spherical_coordinates. From this
standpoint, the eigenfunctions of the angular part of the Laplacian operator
are the spherical_harmonics, of which the Legendre polynomials are (up to a
multiplicative constant) the subset that is left invariant by rotations about
the polar axis. The polynomials appear as      P  n   ( cos &#x2061; &#x03B8; )
{\displaystyle P_{n}(\cos \theta )}  [P_{n}(\cos \theta )] where     &#x03B8;
{\displaystyle \theta }  [\theta ] is the polar angle. This approach to the
Legendre polynomials provides a deep connection to rotational symmetry. Many of
their properties which are found laboriously through the methods of analysis
â for example the addition theorem â are more easily found using the
methods of symmetry and group theory, and acquire profound physical and
geometrical meaning.
***** Orthonormality and completeness[edit] *****
The standardization      P  n   ( 1 ) = 1   {\displaystyle P_{n}(1)=1}  [
{\displaystyle P_{n}(1)=1}] fixes the normalization of the Legendre polynomials
(with respect to the L2_norm on the interval â1 â¤ x â¤ 1). Since they are
also orthogonal with respect to the same norm, the two statements can be
combined into the single equation,
          &#x222B;  &#x2212; 1   1    P  m   ( x )  P  n   ( x )  d x =   2  2
      n + 1     &#x03B4;  m n   ,   {\displaystyle \int _{-1}^{1}P_{m}(x)P_{n}
      (x)\,dx={\frac {2}{2n+1}}\delta _{mn},}  [{\displaystyle \int _{-1}^{1}P_
      {m}(x)P_{n}(x)\,dx={\frac {2}{2n+1}}\delta _{mn},}]
(where Î´mn denotes the Kronecker_delta, equal to 1 if m = n and to 0
otherwise). This normalization is most readily found by employing Rodrigues'
formula, given below.
That the polynomials are complete means the following. Given any piecewise
continuous function     f ( x )   {\displaystyle f(x)}  [f(x)] with finitely
many discontinuities in the interval [â1,1], the sequence of sums
          f  n   ( x ) =  &#x2211;  &#x2113; = 0   n    a  &#x2113;    P
      &#x2113;   ( x )   {\displaystyle f_{n}(x)=\sum _{\ell =0}^{n}a_{\ell }P_
      {\ell }(x)}  [{\displaystyle f_{n}(x)=\sum _{\ell =0}^{n}a_{\ell }P_{\ell
      }(x)}]
converges in the mean to     f ( x )   {\displaystyle f(x)}  [f(x)] as     n
&#x2192; &#x221E;   {\displaystyle n\to \infty }  [n\to \infty ], provided we
take
          a  &#x2113;   =    2 &#x2113; + 1  2    &#x222B;  &#x2212; 1   1   f
      ( x )  P  &#x2113;   ( x )  d x .   {\displaystyle a_{\ell }={\frac
      {2\ell +1}{2}}\int _{-1}^{1}f(x)P_{\ell }(x)\,dx.}  [{\displaystyle a_
      {\ell }={\frac {2\ell +1}{2}}\int _{-1}^{1}f(x)P_{\ell }(x)\,dx.}]
This completeness property underlies all the expansions discussed in this
article, and is often stated in the form
          &#x2211;  &#x2113; = 0   &#x221E;      2 &#x2113; + 1  2    P
      &#x2113;   ( x )  P  &#x2113;   ( y ) = &#x03B4; ( x &#x2212; y ) ,
      {\displaystyle \sum _{\ell =0}^{\infty }{\frac {2\ell +1}{2}}P_{\ell }
      (x)P_{\ell }(y)=\delta (x-y),}  [{\displaystyle \sum _{\ell =0}^{\infty }
      {\frac {2\ell +1}{2}}P_{\ell }(x)P_{\ell }(y)=\delta (x-y),}]
with â1 â¤ x â¤ 1 and â1 â¤ y â¤ 1.
***** Rodrigues' formula and other explicit formulas[edit] *****
An especially compact expression for the Legendre polynomials is given by
Rodrigues'_formula:
          P  n   ( x ) =   1   2  n   n !       d  n    d  x  n      (  x  2
      &#x2212; 1  )  n    .   {\displaystyle P_{n}(x)={\frac {1}{2^{n}n!}}
      {\frac {d^{n}}{dx^{n}}}(x^{2}-1)^{n}\,.}  [{\displaystyle P_{n}(x)={\frac
      {1}{2^{n}n!}}{\frac {d^{n}}{dx^{n}}}(x^{2}-1)^{n}\,.}]
This formula enables derivation of a large number of properties of the      P
n     {\displaystyle P_{n}}  [P_{n}]'s. Among these are explicit
representations such as
              P  n   ( x )    =   1  2  n      &#x2211;  k = 0   n       (   n
      k   )     2   ( x &#x2212; 1  )  n &#x2212; k   ( x + 1  )  k   ,      P
      n   ( x )    =  &#x2211;  k = 0   n      (   n k   )       (    n + k  k
      )      (    x &#x2212; 1  2   )   k   ,      P  n   ( x )    =   1  2  n
      &#x2211;  k = 0   [   n 2   ]   ( &#x2212; 1  )  k      (   n k   )
      (    2 n &#x2212; 2 k  n   )     x  n &#x2212; 2 k   ,      P  n   ( x )
      =  2  n    &#x2211;  k = 0   n    x  k      (   n k   )       (     n + k
      &#x2212; 1  2  n   )    ,       {\displaystyle {\begin{aligned}P_{n}(x)&=
      {\frac {1}{2^{n}}}\sum _{k=0}^{n}{\binom {n}{k}}^{2}(x-1)^{n-k}(x+1)^
      {k},\\P_{n}(x)&=\sum _{k=0}^{n}{\binom {n}{k}}{\binom {n+k}{k}}\left(
      {\frac {x-1}{2}}\right)^{k},\\P_{n}(x)&={\frac {1}{2^{n}}}\sum _{k=0}^{[
      {\frac {n}{2}}]}(-1)^{k}{\binom {n}{k}}{\binom {2n-2k}{n}}x^{n-2k},\\P_
      {n}(x)&=2^{n}\sum _{k=0}^{n}x^{k}{\binom {n}{k}}{\binom {\frac {n+k-1}
      {2}}{n}},\end{aligned}}}  [{\displaystyle {\begin{aligned}P_{n}(x)&=
      {\frac {1}{2^{n}}}\sum _{k=0}^{n}{\binom {n}{k}}^{2}(x-1)^{n-k}(x+1)^
      {k},\\P_{n}(x)&=\sum _{k=0}^{n}{\binom {n}{k}}{\binom {n+k}{k}}\left(
      {\frac {x-1}{2}}\right)^{k},\\P_{n}(x)&={\frac {1}{2^{n}}}\sum _{k=0}^{[
      {\frac {n}{2}}]}(-1)^{k}{\binom {n}{k}}{\binom {2n-2k}{n}}x^{n-2k},\\P_
      {n}(x)&=2^{n}\sum _{k=0}^{n}x^{k}{\binom {n}{k}}{\binom {\frac {n+k-1}
      {2}}{n}},\end{aligned}}}]
where the last, which is also immediate from the recursion formula, expresses
the Legendre polynomials by simple monomials and involves the multiplicative
formula of the binomial_coefficient.[clarification_needed]
The first few Legendre polynomials are:
              n    P  n   ( x )     0   1     1   x     2      1 2     (  3  x
      2   &#x2212; 1  )      3      1 2     (  5  x  3   &#x2212; 3 x  )      4
      1 8     (  35  x  4   &#x2212; 30  x  2   + 3  )      5      1 8
      (  63  x  5   &#x2212; 70  x  3   + 15 x  )      6      1 16     (  231
      x  6   &#x2212; 315  x  4   + 105  x  2   &#x2212; 5  )      7      1 16
      (  429  x  7   &#x2212; 693  x  5   + 315  x  3   &#x2212; 35 x  )      8
      1 128     (  6435  x  8   &#x2212; 12012  x  6   + 6930  x  4   &#x2212;
      1260  x  2   + 35  )      9      1 128     (  12155  x  9   &#x2212;
      25740  x  7   + 18018  x  5   &#x2212; 4620  x  3   + 315 x  )      10
      1 256     (  46189  x  10   &#x2212; 109395  x  8   + 90090  x  6
      &#x2212; 30030  x  4   + 3465  x  2   &#x2212; 63  )
      {\displaystyle {\begin{array}{r|r}n&P_{n}(x)\\\hline 0&1\\1&x\\2&{\tfrac
      {1}{2}}\left(3x^{2}-1\right)\\3&{\tfrac {1}{2}}\left(5x^{3}-3x\right)\\4&
      {\tfrac {1}{8}}\left(35x^{4}-30x^{2}+3\right)\\5&{\tfrac {1}{8}}\left
      (63x^{5}-70x^{3}+15x\right)\\6&{\tfrac {1}{16}}\left(231x^{6}-315x^
      {4}+105x^{2}-5\right)\\7&{\tfrac {1}{16}}\left(429x^{7}-693x^{5}+315x^
      {3}-35x\right)\\8&{\tfrac {1}{128}}\left(6435x^{8}-12012x^{6}+6930x^{4}-
      1260x^{2}+35\right)\\9&{\tfrac {1}{128}}\left(12155x^{9}-25740x^
      {7}+18018x^{5}-4620x^{3}+315x\right)\\10&{\tfrac {1}{256}}\left(46189x^
      {10}-109395x^{8}+90090x^{6}-30030x^{4}+3465x^{2}-63\right)\\\hline \end
      {array}}}  [{\displaystyle {\begin{array}{r|r}n&P_{n}(x)\\\hline
      0&1\\1&x\\2&{\tfrac {1}{2}}\left(3x^{2}-1\right)\\3&{\tfrac {1}{2}}\left
      (5x^{3}-3x\right)\\4&{\tfrac {1}{8}}\left(35x^{4}-30x^{2}+3\right)\\5&
      {\tfrac {1}{8}}\left(63x^{5}-70x^{3}+15x\right)\\6&{\tfrac {1}{16}}\left
      (231x^{6}-315x^{4}+105x^{2}-5\right)\\7&{\tfrac {1}{16}}\left(429x^{7}-
      693x^{5}+315x^{3}-35x\right)\\8&{\tfrac {1}{128}}\left(6435x^{8}-12012x^
      {6}+6930x^{4}-1260x^{2}+35\right)\\9&{\tfrac {1}{128}}\left(12155x^{9}-
      25740x^{7}+18018x^{5}-4620x^{3}+315x\right)\\10&{\tfrac {1}{256}}\left
      (46189x^{10}-109395x^{8}+90090x^{6}-30030x^{4}+3465x^{2}-
      63\right)\\\hline \end{array}}}]
The graphs of these polynomials (up to n = 5) are shown below:
      [Plot_of_the_six_first_Legendre_polynomials.]
***** Applications of Legendre polynomials[edit] *****
**** Expanding a 1/r potential[edit] ****
The Legendre polynomials were first introduced in 1782 by Adrien-Marie_Legendre
[2] as the coefficients in the expansion of the Newtonian_potential
           1  |   x  &#x2212;   x  &#x2032;   |    =   1   r  2   +    r
      &#x2032;    2   &#x2212; 2 r   r &#x2032;   cos &#x2061; &#x03B3;    =
      &#x2211;  &#x2113; = 0   &#x221E;        r &#x2032;    &#x2113;    r
      &#x2113; + 1      P  &#x2113;   ( cos &#x2061; &#x03B3; ) ,
      {\displaystyle {\frac {1}{\left|\mathbf {x} -\mathbf {x} '\right|}}=
      {\frac {1}{\sqrt {r^{2}+{r'}^{2}-2r{r'}\cos \gamma }}}=\sum _{\ell =0}^
      {\infty }{\frac {{r'}^{\ell }}{r^{\ell +1}}}P_{\ell }(\cos \gamma ),}  [
      {\displaystyle {\frac {1}{\left|\mathbf {x} -\mathbf {x} '\right|}}=
      {\frac {1}{\sqrt {r^{2}+{r'}^{2}-2r{r'}\cos \gamma }}}=\sum _{\ell =0}^
      {\infty }{\frac {{r'}^{\ell }}{r^{\ell +1}}}P_{\ell }(\cos \gamma ),}]
where r and râ² are the lengths of the vectors x and xâ² respectively and Î³
is the angle between those two vectors. The series converges when r > râ². The
expression gives the gravitational_potential associated to a point_mass or the
Coulomb_potential associated to a point_charge. The expansion using Legendre
polynomials might be useful, for instance, when integrating this expression
over a continuous mass or charge distribution.
Legendre polynomials occur in the solution of Laplace's_equation of the static
potential, â2 Î¦(x) = 0, in a charge-free region of space, using the method
of separation_of_variables, where the boundary_conditions have axial symmetry
(no dependence on an azimuthal_angle). Where áº is the axis of symmetry and Î¸
is the angle between the position of the observer and the áº axis (the zenith
angle), the solution for the potential will be
         &#x03A6; ( r , &#x03B8; ) =  &#x2211;  &#x2113; = 0   &#x221E;
      (   A  &#x2113;    r  &#x2113;   +  B  &#x2113;    r  &#x2212; ( &#x2113;
      + 1 )    )   P  &#x2113;   ( cos &#x2061; &#x03B8; )  .   {\displaystyle
      \Phi (r,\theta )=\sum _{\ell =0}^{\infty }\left(A_{\ell }r^{\ell }+B_
      {\ell }r^{-(\ell +1)}\right)P_{\ell }(\cos \theta )\,.}  [{\displaystyle
      \Phi (r,\theta )=\sum _{\ell =0}^{\infty }\left(A_{\ell }r^{\ell }+B_
      {\ell }r^{-(\ell +1)}\right)P_{\ell }(\cos \theta )\,.}]
Al and Bl are to be determined according to the boundary condition of each
problem.[3]
They also appear when solving the SchrÃ¶dinger_equation in three dimensions for
a central force.
**** Legendre polynomials in multipole expansions[edit] ****
[Diagram_for_the_multipole_expansion_of_electric_potential.]
Legendre polynomials are also useful in expanding functions of the form (this
is the same as before, written a little differently):
           1  1 +  &#x03B7;  2   &#x2212; 2 &#x03B7; x    =  &#x2211;  k = 0
      &#x221E;    &#x03B7;  k    P  k   ( x ) ,   {\displaystyle {\frac {1}
      {\sqrt {1+\eta ^{2}-2\eta x}}}=\sum _{k=0}^{\infty }\eta ^{k}P_{k}(x),}
      [{\displaystyle {\frac {1}{\sqrt {1+\eta ^{2}-2\eta x}}}=\sum _{k=0}^
      {\infty }\eta ^{k}P_{k}(x),}]
which arise naturally in multipole_expansions. The left-hand side of the
equation is the generating_function for the Legendre polynomials.
As an example, the electric_potential Î¦(r,Î¸) (in spherical_coordinates) due
to a point_charge located on the z-axis at z = a (see diagram right) varies as
         &#x03A6; ( r , &#x03B8; ) &#x221D;   1 R   =   1   r  2   +  a  2
      &#x2212; 2 a r cos &#x2061; &#x03B8;    .   {\displaystyle \Phi (r,\theta
      )\propto {\frac {1}{R}}={\frac {1}{\sqrt {r^{2}+a^{2}-2ar\cos \theta
      }}}.}  [{\displaystyle \Phi (r,\theta )\propto {\frac {1}{R}}={\frac {1}
      {\sqrt {r^{2}+a^{2}-2ar\cos \theta }}}.}]
If the radius r of the observation point P is greater than a, the potential may
be expanded in the Legendre polynomials
         &#x03A6; ( r , &#x03B8; ) &#x221D;   1 r    &#x2211;  k = 0   &#x221E;
      (   a r   )   k    P  k   ( cos &#x2061; &#x03B8; ) ,   {\displaystyle
      \Phi (r,\theta )\propto {\frac {1}{r}}\sum _{k=0}^{\infty }\left({\frac
      {a}{r}}\right)^{k}P_{k}(\cos \theta ),}  [{\displaystyle \Phi (r,\theta
      )\propto {\frac {1}{r}}\sum _{k=0}^{\infty }\left({\frac {a}{r}}\right)^
      {k}P_{k}(\cos \theta ),}]
where we have defined Î· = a/r < 1 and x = cos Î¸. This expansion is used to
develop the normal multipole_expansion.
Conversely, if the radius r of the observation point P is smaller than a, the
potential may still be expanded in the Legendre polynomials as above, but with
a and r exchanged. This expansion is the basis of interior_multipole_expansion.
**** Legendre polynomials in trigonometry[edit] ****
The trigonometric functions cos nÎ¸, also denoted as the Chebyshev_polynomials
Tn(cos Î¸) â¡ cos nÎ¸, can also be multipole expanded by the Legendre
polynomials Pn(cos Î¸). The first several orders are as follows:
              T  0   ( cos &#x2061; &#x03B8; )    = 1     =  P  0   ( cos
      &#x2061; &#x03B8; ) ,      T  1   ( cos &#x2061; &#x03B8; )    = cos
      &#x2061; &#x03B8;     =  P  1   ( cos &#x2061; &#x03B8; ) ,      T  2
      ( cos &#x2061; &#x03B8; )    = cos &#x2061; 2 &#x03B8;     =    1 3
      (   4  P  2   ( cos &#x2061; &#x03B8; ) &#x2212;  P  0   ( cos &#x2061;
      &#x03B8; )   )   ,      T  3   ( cos &#x2061; &#x03B8; )    = cos
      &#x2061; 3 &#x03B8;     =    1 5      (   8  P  3   ( cos &#x2061;
      &#x03B8; ) &#x2212; 3  P  1   ( cos &#x2061; &#x03B8; )   )   ,      T  4
      ( cos &#x2061; &#x03B8; )    = cos &#x2061; 4 &#x03B8;     =    1 105
      (   192  P  4   ( cos &#x2061; &#x03B8; ) &#x2212; 80  P  2   ( cos
      &#x2061; &#x03B8; ) &#x2212; 7  P  0   ( cos &#x2061; &#x03B8; )   )   ,
      T  5   ( cos &#x2061; &#x03B8; )    = cos &#x2061; 5 &#x03B8;     =    1
      63      (   128  P  5   ( cos &#x2061; &#x03B8; ) &#x2212; 56  P  3
      ( cos &#x2061; &#x03B8; ) &#x2212; 9  P  1   ( cos &#x2061; &#x03B8; )
      )   ,      T  6   ( cos &#x2061; &#x03B8; )    = cos &#x2061; 6 &#x03B8;
      =    1 1155      (   2560  P  6   ( cos &#x2061; &#x03B8; ) &#x2212; 1152
      P  4   ( cos &#x2061; &#x03B8; ) &#x2212; 220  P  2   ( cos &#x2061;
      &#x03B8; ) &#x2212; 33  P  0   ( cos &#x2061; &#x03B8; )   )   .
      {\displaystyle {\begin{aligned}T_{0}(\cos \theta )&=1&&=P_{0}(\cos \theta
      ),\\[4pt]T_{1}(\cos \theta )&=\cos \theta &&=P_{1}(\cos \theta ),\\
      [4pt]T_{2}(\cos \theta )&=\cos 2\theta &&={\tfrac {1}{3}}{\bigl (}4P_{2}
      (\cos \theta )-P_{0}(\cos \theta ){\bigr )},\\[4pt]T_{3}(\cos \theta
      )&=\cos 3\theta &&={\tfrac {1}{5}}{\bigl (}8P_{3}(\cos \theta )-3P_{1}
      (\cos \theta ){\bigr )},\\[4pt]T_{4}(\cos \theta )&=\cos 4\theta &&=
      {\tfrac {1}{105}}{\bigl (}192P_{4}(\cos \theta )-80P_{2}(\cos \theta )-
      7P_{0}(\cos \theta ){\bigr )},\\[4pt]T_{5}(\cos \theta )&=\cos 5\theta
      &&={\tfrac {1}{63}}{\bigl (}128P_{5}(\cos \theta )-56P_{3}(\cos \theta )-
      9P_{1}(\cos \theta ){\bigr )},\\[4pt]T_{6}(\cos \theta )&=\cos 6\theta
      &&={\tfrac {1}{1155}}{\bigl (}2560P_{6}(\cos \theta )-1152P_{4}(\cos
      \theta )-220P_{2}(\cos \theta )-33P_{0}(\cos \theta ){\bigr )}.\end
      {aligned}}}  [{\displaystyle {\begin{aligned}T_{0}(\cos \theta )&=1&&=P_
      {0}(\cos \theta ),\\[4pt]T_{1}(\cos \theta )&=\cos \theta &&=P_{1}(\cos
      \theta ),\\[4pt]T_{2}(\cos \theta )&=\cos 2\theta &&={\tfrac {1}{3}}
      {\bigl (}4P_{2}(\cos \theta )-P_{0}(\cos \theta ){\bigr )},\\[4pt]T_{3}
      (\cos \theta )&=\cos 3\theta &&={\tfrac {1}{5}}{\bigl (}8P_{3}(\cos
      \theta )-3P_{1}(\cos \theta ){\bigr )},\\[4pt]T_{4}(\cos \theta )&=\cos
      4\theta &&={\tfrac {1}{105}}{\bigl (}192P_{4}(\cos \theta )-80P_{2}(\cos
      \theta )-7P_{0}(\cos \theta ){\bigr )},\\[4pt]T_{5}(\cos \theta )&=\cos
      5\theta &&={\tfrac {1}{63}}{\bigl (}128P_{5}(\cos \theta )-56P_{3}(\cos
      \theta )-9P_{1}(\cos \theta ){\bigr )},\\[4pt]T_{6}(\cos \theta )&=\cos
      6\theta &&={\tfrac {1}{1155}}{\bigl (}2560P_{6}(\cos \theta )-1152P_{4}
      (\cos \theta )-220P_{2}(\cos \theta )-33P_{0}(\cos \theta ){\bigr )}.\end
      {aligned}}}]
Another property is the expression for sin (n + 1)Î¸, which is
            sin &#x2061; ( n + 1 ) &#x03B8;   sin &#x2061; &#x03B8;    =
      &#x2211;  &#x2113; = 0   n    P  &#x2113;   ( cos &#x2061; &#x03B8; )  P
      n &#x2212; &#x2113;   ( cos &#x2061; &#x03B8; ) .   {\displaystyle {\frac
      {\sin(n+1)\theta }{\sin \theta }}=\sum _{\ell =0}^{n}P_{\ell }(\cos
      \theta )P_{n-\ell }(\cos \theta ).}  [{\displaystyle {\frac {\sin
      (n+1)\theta }{\sin \theta }}=\sum _{\ell =0}^{n}P_{\ell }(\cos \theta )P_
      {n-\ell }(\cos \theta ).}]
***** Additional properties of Legendre polynomials[edit] *****
Legendre polynomials have definite parity. That is, they are symmetric_or
antisymmetric,[4] according to
          P  n   ( &#x2212; x ) = ( &#x2212; 1  )  n    P  n   ( x )  .
      {\displaystyle P_{n}(-x)=(-1)^{n}P_{n}(x)\,.}  [{\displaystyle P_{n}(-x)=
      (-1)^{n}P_{n}(x)\,.}]
Another useful property is
          &#x222B;  &#x2212; 1   1    P  n   ( x )  d x = 0  &#xA0;for&#xA0;  n
      &#x2265; 1 ,   {\displaystyle \int _{-1}^{1}P_{n}(x)\,dx=0{\text{ for
      }}n\geq 1,}  [{\displaystyle \int _{-1}^{1}P_{n}(x)\,dx=0{\text{ for
      }}n\geq 1,}]
which follows from considering the orthogonality relation with      P  0   ( x
) = 1   {\displaystyle P_{0}(x)=1}  [{\displaystyle P_{0}(x)=1}]. It is
convenient when a Legendre series      &#x2211;  i    a  i    P  i
{\displaystyle \sum _{i}a_{i}P_{i}}  [{\displaystyle \sum _{i}a_{i}P_{i}}] is
used to approximate a function or experimental data: the average of the series
over the interval [â1, 1] is simply given by the leading expansion
coefficient      a  0     {\displaystyle a_{0}}  [a_{0}].
Since the differential equation and the orthogonality property are independent
of scaling, the Legendre polynomials' definitions are "standardized" (sometimes
called "normalization", but note that the actual norm is not 1) by being scaled
so that
          P  n   ( 1 ) = 1  .   {\displaystyle P_{n}(1)=1\,.}  [{\displaystyle
      P_{n}(1)=1\,.}]
The derivative at the end point is given by
          P  n  &#x2032;  ( 1 ) =    n ( n + 1 )  2    .   {\displaystyle P_
      {n}'(1)={\frac {n(n+1)}{2}}\,.}  [{\displaystyle P_{n}'(1)={\frac {n
      (n+1)}{2}}\,.}]
The AskeyâGasper_inequality for Legendre polynomials reads
          &#x2211;  j = 0   n    P  j   ( x ) &#x2265; 0    for&#xA0;  x
      &#x2265; &#x2212; 1  .   {\displaystyle \sum _{j=0}^{n}P_{j}(x)\geq
      0\,\quad {\text{for }}x\geq -1\,.}  [{\displaystyle \sum _{j=0}^{n}P_{j}
      (x)\geq 0\,\quad {\text{for }}x\geq -1\,.}]
The Legendre polynomials of a scalar_product of unit_vectors can be expanded
with spherical_harmonics using
          P  &#x2113;    (  r &#x22C5;  r &#x2032;   )  =    4 &#x03C0;   2
      &#x2113; + 1     &#x2211;  m = &#x2212; &#x2113;   &#x2113;    Y
      &#x2113; m   ( &#x03B8; , &#x03C6; )  Y  &#x2113; m   &#x2217;
      (  &#x03B8; &#x2032;  ,  &#x03C6; &#x2032;  )  ,   {\displaystyle P_{\ell
      }\left(r\cdot r'\right)={\frac {4\pi }{2\ell +1}}\sum _{m=-\ell }^{\ell
      }Y_{\ell m}(\theta ,\varphi )Y_{\ell m}^{*}(\theta ',\varphi ')\,,}  [
      {\displaystyle P_{\ell }\left(r\cdot r'\right)={\frac {4\pi }{2\ell
      +1}}\sum _{m=-\ell }^{\ell }Y_{\ell m}(\theta ,\varphi )Y_{\ell m}^{*}
      (\theta ',\varphi ')\,,}]
where the unit vectors r and râ² have spherical_coordinates (Î¸,Ï) and
(Î¸â²,Ïâ²), respectively.
**** Recursion relations[edit] ****
As discussed above, the Legendre polynomials obey the three-term recurrence
relation known as Bonnetâs recursion formula
         ( n + 1 )  P  n + 1   ( x ) = ( 2 n + 1 ) x  P  n   ( x ) &#x2212; n
      P  n &#x2212; 1   ( x )   {\displaystyle (n+1)P_{n+1}(x)=(2n+1)xP_{n}(x)-
      nP_{n-1}(x)}  [{\displaystyle (n+1)P_{n+1}(x)=(2n+1)xP_{n}(x)-nP_{n-1}
      (x)}]
and
             x  2   &#x2212; 1  n     d  d x     P  n   ( x ) = x  P  n   ( x )
      &#x2212;  P  n &#x2212; 1   ( x )    {\displaystyle {\frac {x^{2}-1}{n}}
      {\frac {d}{dx}}P_{n}(x)=xP_{n}(x)-P_{n-1}(x)\,}  [{\displaystyle {\frac
      {x^{2}-1}{n}}{\frac {d}{dx}}P_{n}(x)=xP_{n}(x)-P_{n-1}(x)\,}]
or, with the alternative expression, which also holds at the endpoints
           d  d x     P  n + 1   ( x ) = ( n + 1 )  P  n   ( x ) + x   d  d x
      P  n   ( x )  .   {\displaystyle {\frac {d}{dx}}P_{n+1}(x)=(n+1)P_{n}
      (x)+x{\frac {d}{dx}}P_{n}(x)\,.}  [{\displaystyle {\frac {d}{dx}}P_{n+1}
      (x)=(n+1)P_{n}(x)+x{\frac {d}{dx}}P_{n}(x)\,.}]
Useful for the integration of Legendre polynomials is
         ( 2 n + 1 )  P  n   ( x ) =   d  d x      (    P  n + 1   ( x )
      &#x2212;  P  n &#x2212; 1   ( x )   )    .   {\displaystyle (2n+1)P_{n}
      (x)={\frac {d}{dx}}{\bigl (}P_{n+1}(x)-P_{n-1}(x){\bigr )}\,.}  [
      {\displaystyle (2n+1)P_{n}(x)={\frac {d}{dx}}{\bigl (}P_{n+1}(x)-P_{n-1}
      (x){\bigr )}\,.}]
From the above one can see also that
           d  d x     P  n + 1   ( x ) = ( 2 n + 1 )  P  n   ( x ) +   (   2
      ( n &#x2212; 2 ) + 1   )    P  n &#x2212; 2   ( x ) +   (   2 ( n
      &#x2212; 4 ) + 1   )    P  n &#x2212; 4   ( x ) + &#x22EF;
      {\displaystyle {\frac {d}{dx}}P_{n+1}(x)=(2n+1)P_{n}(x)+{\bigl (}2(n-2)+1
      {\bigr )}P_{n-2}(x)+{\bigl (}2(n-4)+1{\bigr )}P_{n-4}(x)+\cdots }  [
      {\displaystyle {\frac {d}{dx}}P_{n+1}(x)=(2n+1)P_{n}(x)+{\bigl (}2(n-2)+1
      {\bigr )}P_{n-2}(x)+{\bigl (}2(n-4)+1{\bigr )}P_{n-4}(x)+\cdots }]
or equivalently
           d  d x     P  n + 1   ( x ) =    2  P  n   ( x )    &#x2016;  P  n
      &#x2016;   2     +    2  P  n &#x2212; 2   ( x )    &#x2016;  P  n
      &#x2212; 2   &#x2016;   2     + &#x22EF;   {\displaystyle {\frac {d}
      {dx}}P_{n+1}(x)={\frac {2P_{n}(x)}{\left\|P_{n}\right\|^{2}}}+{\frac {2P_
      {n-2}(x)}{\left\|P_{n-2}\right\|^{2}}}+\cdots }  [{\displaystyle {\frac
      {d}{dx}}P_{n+1}(x)={\frac {2P_{n}(x)}{\left\|P_{n}\right\|^{2}}}+{\frac
      {2P_{n-2}(x)}{\left\|P_{n-2}\right\|^{2}}}+\cdots }]
where ||Pn|| is the norm over the interval â1 â¤ x â¤ 1
         &#x2016;  P  n   &#x2016; =    &#x222B;  &#x2212; 1   1     (    P  n
      ( x )    )    2    d x   =    2  2 n + 1      .   {\displaystyle \|P_
      {n}\|={\sqrt {\int _{-1}^{1}{\bigl (}P_{n}(x){\bigr )}^{2}\,dx}}={\sqrt
      {\frac {2}{2n+1}}}\,.}  [{\displaystyle \|P_{n}\|={\sqrt {\int _{-1}^{1}
      {\bigl (}P_{n}(x){\bigr )}^{2}\,dx}}={\sqrt {\frac {2}{2n+1}}}\,.}]
**** Asymptotes[edit] ****
Asymptotically for l â â[5]
              P  &#x2113;   ( cos &#x2061; &#x03B8; )    =    &#x03B8;  sin
      &#x2061; &#x03B8;       J  0   ( ( &#x2113; + 1  /  2 ) &#x03B8; ) +   O
      (  &#x2113;  &#x2212; 1   )        =   2  2 &#x03C0; &#x2113; sin
      &#x2061; &#x03B8;    cos &#x2061;  (   (  &#x2113; +    1 2     )
      &#x03B8; &#x2212;   &#x03C0; 4    )  +   O    (  &#x2113;  &#x2212; 1   )
      ,  &#x03B8; &#x2208; ( 0 , &#x03C0; ) ,       {\displaystyle {\begin
      {aligned}P_{\ell }(\cos \theta )&={\sqrt {\frac {\theta }{\sin \theta
      }}}\,J_{0}((\ell +1/2)\theta )+{\mathcal {O}}\left(\ell ^{-1}\right)\\&=
      {\frac {2}{\sqrt {2\pi \ell \sin \theta }}}\cos \left(\left(\ell +{\tfrac
      {1}{2}}\right)\theta -{\frac {\pi }{4}}\right)+{\mathcal {O}}\left(\ell ^
      {-1}\right),\quad \theta \in (0,\pi ),\end{aligned}}}  [{\displaystyle
      {\begin{aligned}P_{\ell }(\cos \theta )&={\sqrt {\frac {\theta }{\sin
      \theta }}}\,J_{0}((\ell +1/2)\theta )+{\mathcal {O}}\left(\ell ^{-
      1}\right)\\&={\frac {2}{\sqrt {2\pi \ell \sin \theta }}}\cos \left(\left
      (\ell +{\tfrac {1}{2}}\right)\theta -{\frac {\pi }{4}}\right)+{\mathcal
      {O}}\left(\ell ^{-1}\right),\quad \theta \in (0,\pi ),\end{aligned}}}]
and for arguments of magnitude greater than 1
              P  &#x2113;    (   1  1 &#x2212;  e  2      )     =  I  0
      ( &#x2113; e ) +   O    (  &#x2113;  &#x2212; 1   )        =   1  2
      &#x03C0; &#x2113; e       ( 1 + e  )    &#x2113; + 1  2      ( 1 &#x2212;
      e  )   &#x2113; 2       +   O    (  &#x2113;  &#x2212; 1   )   ,
      {\displaystyle {\begin{aligned}P_{\ell }\left({\frac {1}{\sqrt {1-e^
      {2}}}}\right)&=I_{0}(\ell e)+{\mathcal {O}}\left(\ell ^{-1}\right)\\&=
      {\frac {1}{\sqrt {2\pi \ell e}}}{\frac {(1+e)^{\frac {\ell +1}{2}}}{(1-
      e)^{\frac {\ell }{2}}}}+{\mathcal {O}}\left(\ell ^{-1}\right)\,,\end
      {aligned}}}  [{\displaystyle {\begin{aligned}P_{\ell }\left({\frac {1}
      {\sqrt {1-e^{2}}}}\right)&=I_{0}(\ell e)+{\mathcal {O}}\left(\ell ^{-
      1}\right)\\&={\frac {1}{\sqrt {2\pi \ell e}}}{\frac {(1+e)^{\frac {\ell
      +1}{2}}}{(1-e)^{\frac {\ell }{2}}}}+{\mathcal {O}}\left(\ell ^{-
      1}\right)\,,\end{aligned}}}]
where J0 and I0 are Bessel_functions.
**** Zeros[edit] ****
All     n   {\displaystyle n}  [n] zeros of      P  n   ( x )   {\displaystyle
P_{n}(x)}  [P_n(x)] are real, distinct from each other, and lie in the interval
( &#x2212; 1 , 1 )   {\displaystyle (-1,1)}  [(-1,1)]. Further, if we regard
them as dividing the interval     [ &#x2212; 1 , 1 ]   {\displaystyle [-1,1]}
[[-1,1]] into     n + 1   {\displaystyle n+1}  [ n+1 ] subintervals, each
subinterval will contain exactly one zero of      P  n + 1     {\displaystyle
P_{n+1}}  [P_{n+1}]. This is known as the interlacing property. Because of the
parity property it is evident that if      x  k     {\displaystyle x_{k}}  [x_
{k}] is a zero of      P  n   ( x )   {\displaystyle P_{n}(x)}  [P_n(x)], so is
&#x2212;  x  k     {\displaystyle -x_{k}}  [{\displaystyle -x_{k}}]. These
zeros play an important role in numerical integration based on Gaussian
quadrature. The specific quadrature based on the      P  n     {\displaystyle
P_{n}}  [P_{n}]'s is known as Gauss-Legendre quadrature.
**** Pointwise evaluations[edit] ****
The parity and normalization implicate the values at the boundaries     x =
&#x00B1; 1   {\displaystyle x=\pm 1}  [{\displaystyle x=\pm 1}] to be
          P  n   ( 1 ) = 1  ,   P  n   ( &#x2212; 1 ) =   {    1    for   n = 2
      m     &#x2212; 1    for   n = 2 m + 1  .         {\displaystyle P_{n}
      (1)=1\,,\quad P_{n}(-1)={\begin{cases}1&{\text{for}}\quad n=2m\\-1&{\text
      {for}}\quad n=2m+1\,.\end{cases}}}  [{\displaystyle P_{n}(1)=1\,,\quad P_
      {n}(-1)={\begin{cases}1&{\text{for}}\quad n=2m\\-1&{\text{for}}\quad
      n=2m+1\,.\end{cases}}}]
At the origin     x = 0   {\displaystyle x=0}  [x=0] one can show that the
values are given by
          P  n   ( 0 ) =   {       ( &#x2212; 1  )  m     4  m         (    2 m
      m   )     =    ( &#x2212; 1  )  m     2  2 m + 1        ( 2 m ) !   m !
      for   n = 2 m     0    for   n = 2 m + 1  .         {\displaystyle P_{n}
      (0)={\begin{cases}{\frac {(-1)^{m}}{4^{m}}}{\tbinom {2m}{m}}={\frac {(-
      1)^{m}}{2^{2m+1}}}{\frac {(2m)!}{m!}}&{\text{for}}\quad n=2m\\0&{\text
      {for}}\quad n=2m+1\,.\end{cases}}}  [{\displaystyle P_{n}(0)={\begin
      {cases}{\frac {(-1)^{m}}{4^{m}}}{\tbinom {2m}{m}}={\frac {(-1)^{m}}{2^
      {2m+1}}}{\frac {(2m)!}{m!}}&{\text{for}}\quad n=2m\\0&{\text{for}}\quad
      n=2m+1\,.\end{cases}}}]
***** Legendre polynomials with transformed argument[edit] *****
**** Shifted Legendre polynomials[edit] ****
The shifted Legendre polynomials are defined as
             P &#x007E;     n   ( x ) =  P  n   ( 2 x &#x2212; 1 )
      {\displaystyle {\widetilde {P}}_{n}(x)=P_{n}(2x-1)\,}  [{\displaystyle
      {\widetilde {P}}_{n}(x)=P_{n}(2x-1)\,}].
Here the "shifting" function x â¦ 2x â 1 is an affine_transformation that
bijectively_maps the interval [0,1] to the interval [â1,1], implying that the
polynomials PÌn(x) are orthogonal on [0,1]:
          &#x222B;  0   1       P &#x007E;     m   ( x )     P &#x007E;     n
      ( x )  d x =   1  2 n + 1     &#x03B4;  m n    .   {\displaystyle \int _
      {0}^{1}{\widetilde {P}}_{m}(x){\widetilde {P}}_{n}(x)\,dx={\frac {1}
      {2n+1}}\delta _{mn}\,.}  [{\displaystyle \int _{0}^{1}{\widetilde {P}}_
      {m}(x){\widetilde {P}}_{n}(x)\,dx={\frac {1}{2n+1}}\delta _{mn}\,.}]
An explicit expression for the shifted Legendre polynomials is given by
             P &#x007E;     n   ( x ) = ( &#x2212; 1  )  n    &#x2211;  k = 0
      n      (   n k   )       (    n + k  k   )    ( &#x2212; x  )  k    .
      {\displaystyle {\widetilde {P}}_{n}(x)=(-1)^{n}\sum _{k=0}^{n}{\binom {n}
      {k}}{\binom {n+k}{k}}(-x)^{k}\,.}  [{\displaystyle {\widetilde {P}}_{n}
      (x)=(-1)^{n}\sum _{k=0}^{n}{\binom {n}{k}}{\binom {n+k}{k}}(-x)^{k}\,.}]
The analogue of Rodrigues'_formula for the shifted Legendre polynomials is
             P &#x007E;     n   ( x ) =   1  n !       d  n    d  x  n
      (   x  2   &#x2212; x  )   n    .   {\displaystyle {\widetilde {P}}_{n}
      (x)={\frac {1}{n!}}{\frac {d^{n}}{dx^{n}}}\left(x^{2}-x\right)^{n}\,.}  [
      {\displaystyle {\widetilde {P}}_{n}(x)={\frac {1}{n!}}{\frac {d^{n}}{dx^
      {n}}}\left(x^{2}-x\right)^{n}\,.}]
The first few shifted Legendre polynomials are:
             n       P &#x007E;     n   ( x )     0   1     1   2 x &#x2212; 1
      2   6  x  2   &#x2212; 6 x + 1     3   20  x  3   &#x2212; 30  x  2   +
      12 x &#x2212; 1     4   70  x  4   &#x2212; 140  x  3   + 90  x  2
      &#x2212; 20 x + 1     5   252  x  5   &#x2212; 630  x  4   + 560  x  3
      &#x2212; 210  x  2   + 30 x &#x2212; 1       {\displaystyle {\begin
      {array}{r|r}n&{\widetilde {P}}_{n}(x)\\\hline 0&1\\1&2x-1\\2&6x^{2}-
      6x+1\\3&20x^{3}-30x^{2}+12x-1\\4&70x^{4}-140x^{3}+90x^{2}-20x+1\\5&252x^
      {5}-630x^{4}+560x^{3}-210x^{2}+30x-1\end{array}}}  [{\displaystyle
      {\begin{array}{r|r}n&{\widetilde {P}}_{n}(x)\\\hline 0&1\\1&2x-1\\2&6x^
      {2}-6x+1\\3&20x^{3}-30x^{2}+12x-1\\4&70x^{4}-140x^{3}+90x^{2}-
      20x+1\\5&252x^{5}-630x^{4}+560x^{3}-210x^{2}+30x-1\end{array}}}]
**** Legendre rational functions[edit] ****
Main article: Legendre_rational_functions
The Legendre_rational_functions are a sequence of orthogonal_functions on [0,
â). They are obtained by composing the Cayley_transform with Legendre
polynomials.
A rational Legendre function of degree n is defined as:
          R  n   ( x ) =    2   x + 1      P  n    (    x &#x2212; 1   x + 1
      )   .   {\displaystyle R_{n}(x)={\frac {\sqrt {2}}{x+1}}\,P_{n}\left(
      {\frac {x-1}{x+1}}\right)\,.}  [{\displaystyle R_{n}(x)={\frac {\sqrt
      {2}}{x+1}}\,P_{n}\left({\frac {x-1}{x+1}}\right)\,.}]
They are eigenfunctions of the singular SturmâLiouville_problem:
         ( x + 1 )  &#x2202;  x   ( x  &#x2202;  x   ( ( x + 1 ) v ( x ) ) ) +
      &#x03BB; v ( x ) = 0   {\displaystyle (x+1)\partial _{x}(x\partial _{x}(
      (x+1)v(x)))+\lambda v(x)=0}  [(x+1)\partial_x(x\partial_x((x+1)v
      (x)))+\lambda v(x)=0]
with eigenvalues
          &#x03BB;  n   = n ( n + 1 )  .   {\displaystyle \lambda _{n}=n
      (n+1)\,.}  [{\displaystyle \lambda _{n}=n(n+1)\,.}]
***** See also[edit] *****
    * Gaussian_quadrature
    * Gegenbauer_polynomials
    * TurÃ¡n's_inequalities
    * Legendre_wavelet
    * Jacobi_polynomials
    * Romanovski_polynomials
***** Notes[edit] *****
   1. ^ Arfken_&_Weber_2005, p.743
   2. ^Legendre, A.-M. (1785) [1782]. "Recherches sur l'attraction des
      sphÃ©roÃ¯des homogÃ¨nes". MÃ©moires_de_MathÃ©matiques_et_de_Physique,
      prÃ©sentÃ©s_Ã _l'AcadÃ©mie_Royale_des_Sciences,_par_divers_savans,_et_lus
      dans_ses_AssemblÃ©es (PDF) (in French). X. Paris. pp. 411â435. Archived
      from the_original (PDF) on 2009-09-20.
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
   4. ^Jackson, J. D. (1999). Classical Electrodynamics (3rd ed.). Wiley &
      Sons. p. 103. ISBN 978-0-471-30932-1.
   5. ^ Arfken_&_Weber_2005, p.753
   6. ^1895â1985., SzegÅ, GÃ¡bor, (1975). Orthogonal_polynomials (4th ed.).
      Providence: American Mathematical Society. pp. 194 (Theorem 8.21.2).
      ISBN 0821810235. OCLC 1683237.
***** References[edit] *****
    * Abramowitz,_Milton; Stegun,_Irene_Ann, eds. (1983) [June 1964]. "Chapter
      8". Handbook_of_Mathematical_Functions_with_Formulas,_Graphs,_and
      Mathematical_Tables. Applied Mathematics Series. 55 (Ninth reprint with
      additional corrections of tenth original printing with corrections
      (December 1972); first ed.). Washington D.C.; New York: United States
      Department of Commerce, National Bureau of Standards; Dover Publications.
      pp. 332, 773. ISBN 978-0-486-61272-0. LCCN 64-60036. MR 0167642. LCCN 65-
      12253.
 See also chapter_22.
Arfken,_George_B.; Weber, Hans J. (2005). Mathematical Methods for Physicists.
Elsevier Academic Press. ISBN 0-12-059876-0.
Bayin, S. S. (2006). Mathematical Methods in Science and Engineering. Wiley.
ch. 2. ISBN 978-0-470-04142-0.
Belousov, S. L. (1962). Tables of Normalized Associated Legendre Polynomials.
Mathematical Tables. 18. Pergamon Press. ISBN 978-0-08-009723-7.
Courant,_Richard; Hilbert,_David (1953). Methods of Mathematical Physics. 1.
New York, NY: Interscience. ISBN 978-0-471-50447-4.
Dunster, T. M. (2010), "Legendre_and_Related_Functions", in Olver,_Frank_W._J.;
Lozier, Daniel M.; Boisvert, Ronald F.; Clark, Charles W. (eds.), NIST_Handbook
of_Mathematical_Functions, Cambridge University Press, ISBN 978-0521192255,
MR 2723248
El Attar, Refaat (2009). Legendre Polynomials and Functions. CreateSpace.
ISBN 978-1-4414-9012-4.
Koornwinder,_Tom_H.; Wong, Roderick S. C.; Koekoek, Roelof; Swarttouw, RenÃ© F.
(2010), "Orthogonal_Polynomials", in Olver,_Frank_W._J.; Lozier, Daniel M.;
Boisvert, Ronald F.; Clark, Charles W. (eds.), NIST_Handbook_of_Mathematical
Functions, Cambridge University Press, ISBN 978-0521192255, MR 2723248
***** External links[edit] *****
 Wikimedia Commons has media related to Legendre_polynomials.
    * A_quick_informal_derivation_of_the_Legendre_polynomial_in_the_context_of
      the_quantum_mechanics_of_hydrogen
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Legendre_polynomials",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Wolfram_MathWorld_entry_on_Legendre_polynomials
Dr_James_B._Calvert's_article_on_Legendre_polynomials_from_his_personal
collection_of_mathematics
The_Legendre_Polynomials_by_Carlyle_E._Moore
Legendre_Polynomials_from_Hyperphysics
                                              * BNF: cb12122983h (data)
                                              * GND: 4333222-5
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85075779
                                              * NDL: 00567364
                                              * SUDOC: 029649501

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Legendre_polynomials&oldid=908811031"
Categories:
    * Special_hypergeometric_functions
    * Orthogonal_polynomials
    * Polynomials
Hidden categories:
    * CS1_French-language_sources_(fr)
    * Wikipedia_articles_needing_clarification_from_June_2019
    * Commons_category_link_is_on_Wikidata
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
    * Wikipedia_articles_with_SUDOC_identifiers
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
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
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
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 1 August 2019, at 04:10 (UTC).
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
