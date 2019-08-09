The following text has been accessed from https://en.wikipedia.org/wiki/Laurent_series at Thu Aug 8 22:52:26 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Laurent series ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Power series generalized to allow negative powers
This article is about doubly infinite power series. For power series with
finitely many negative exponents, see Formal_Laurent_series.
A Laurent series is defined with respect to a particular point c and a path of
integration Î³. The path of integration must lie in an annulus, indicated here
by the red color, inside which f(z) is holomorphic (analytic).
In mathematics, the Laurent series of a complex function f(z) is a
representation of that function as a power_series which includes terms of
negative degree. It may be used to express complex functions in cases where a
Taylor_series expansion cannot be applied. The Laurent series was named after
and first published by Pierre_Alphonse_Laurent in 1843. Karl_Weierstrass may
have discovered it first in a paper written in 1841, but it was not published
until after his death.[1]
The Laurent series for a complex function f(z) about a point c is given by:
         f ( z ) =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;    a  n   ( z
      &#x2212; c  )  n     {\displaystyle f(z)=\sum _{n=-\infty }^{\infty }a_
      {n}(z-c)^{n}}  [f(z)=\sum _{n=-\infty }^{\infty }a_{n}(z-c)^{n}]
where an and c are constants, with an defined by a line_integral that
generalizes Cauchy's_integral_formula:
          a  n   =   1  2 &#x03C0; i        &#x222E;       &#x03B3;   &#x2061;
      f ( z )   ( z &#x2212; c  )  n + 1       d z .   {\displaystyle a_{n}=
      {\frac {1}{2\pi i}}\oint _{\gamma }{\frac {f(z)}{(z-c)^{n+1}}}\,dz.}  [
      {\displaystyle a_{n}={\frac {1}{2\pi i}}\oint _{\gamma }{\frac {f(z)}{(z-
      c)^{n+1}}}\,dz.}]
The path of integration     &#x03B3;   {\displaystyle \gamma }  [\gamma ] is
counterclockwise around a Jordan_curve enclosing c and lying in an annulus A in
which     f ( z )   {\displaystyle f(z)}  [f(z)] is holomorphic (analytic). The
expansion for     f ( z )   {\displaystyle f(z)}  [f(z)] will then be valid
anywhere inside the annulus. The annulus is shown in red in the figure on the
right, along with an example of a suitable path of integration labeled
&#x03B3;   {\displaystyle \gamma }  [\gamma ]. If we take     &#x03B3;
{\displaystyle \gamma }  [\gamma ] to be a circle      |  z &#x2212; c  |  =
&#x03F1;   {\displaystyle |z-c|=\varrho }  [|z-c|=\varrho ], where     r <
&#x03F1; < R   {\displaystyle r<\varrho <R}  [r<\varrho <R], this just amounts
to computing the complex Fourier_coefficients of the restriction of     f
{\displaystyle f}  [f] to     &#x03B3;   {\displaystyle \gamma }  [\gamma ].
The fact that these integrals are unchanged by a deformation of the contour
&#x03B3;   {\displaystyle \gamma }  [\gamma ] is an immediate consequence of
Green's_theorem.
In practice, the above integral formula may not offer the most practical method
for computing the coefficients      a  n     {\displaystyle a_{n}}  [a_{n}] for
a given function     f ( z )   {\displaystyle f(z)}  [f(z)]; instead, one often
pieces together the Laurent series by combining known Taylor expansions.
Because the Laurent expansion of a function is unique whenever it exists, any
expression of this form that actually equals the given function     f ( z )
{\displaystyle f(z)}  [f(z)] in some annulus must actually be the Laurent
expansion of     f ( z )   {\displaystyle f(z)}  [f(z)].
⁰
***** Contents *****
    * 1_Convergent_Laurent_series
    * 2_Uniqueness
    * 3_Laurent_polynomials
    * 4_Principal_part
          o 4.1_Multiplication
    * 5_See_also
    * 6_References
    * 7_External_links
***** Convergent Laurent series[edit] *****
Laurent series with complex coefficients are an important tool in complex
analysis, especially to investigate the behavior of functions near
singularities.
e−(1/x2) and Laurent approximations: see text for key. As the negative degree
of the Laurent series rises, it approaches the correct function.
e−(1/x2) and its Laurent approximations with the negative degree rising. The
neighborhood around the zero singularity can never be approximated.
Consider for instance the function     f ( x ) =  e  &#x2212; 1  /   x  2
{\displaystyle f(x)=e^{-1/x^{2}}}  [f(x)=e^{-1/x^{2}}] with     f ( 0 ) = 0
{\displaystyle f(0)=0}  [f(0)=0]. As a real function, it is infinitely
differentiable everywhere; as a complex function however it is not
differentiable at x = 0. By replacing x with −1/x2 in the power_series for the
exponential_function, we obtain its Laurent series which converges and is equal
to f(x) for all complex numbers x except at the singularity x = 0. The graph
opposite shows e−1/x2 in black and its Laurent approximations
          &#x2211;  n = 0   N   ( &#x2212; 1  )  n       x  &#x2212; 2 n    n !
      {\displaystyle \sum _{n=0}^{N}(-1)^{n}\,{x^{-2n} \over n!}}  [\sum _
      {n=0}^{N}(-1)^{n}\,{x^{-2n} \over n!}]
for N = 1, 2, 3, 4, 5, 6, 7 and 50. As N â â, the approximation becomes
exact for all (complex) numbers x except at the singularity x = 0.
More generally, Laurent series can be used to express holomorphic_functions
defined on an annulus, much as power_series are used to express holomorphic
functions defined on a disc.
Suppose
          &#x2211;  n = &#x2212; &#x221E;   &#x221E;    a  n   ( z &#x2212; c
      )  n     {\displaystyle \sum _{n=-\infty }^{\infty }a_{n}(z-c)^{n}}
      [\sum _{n=-\infty }^{\infty }a_{n}(z-c)^{n}]
is a given Laurent series with complex coefficients an and a complex center c.
Then there exists a unique inner radius r and outer radius R such that:
    * The Laurent series converges on the open annulus A â¡ {z :
      r < |z − c| < R}. To say that the Laurent series converges, we mean that
      both the positive degree power series and the negative degree power
      series converge. Furthermore, this convergence will be uniform on compact
      sets. Finally, the convergent series defines a holomorphic_function f(z)
      on the open annulus.
    * Outside the annulus, the Laurent series diverges. That is, at each point
      of the exterior of A, the positive degree power series or the negative
      degree power series diverges.
    * On the boundary of the annulus, one cannot make a general statement,
      except to say that there is at least one point on the inner boundary and
      one point on the outer boundary such that f(z) cannot be holomorphically
      continued to those points.
It is possible that r may be zero or R may be infinite; at the other extreme,
it's not necessarily true that r is less than R. These radii can be computed as
follows:
             r    =  lim&#x2006;sup  n &#x2192; &#x221E;    |   a  &#x2212; n
      |    1 n          1 R      =  lim&#x2006;sup  n &#x2192; &#x221E;    |
      a  n     |    1 n    .       {\displaystyle {\begin{aligned}r&=\limsup _
      {n\rightarrow \infty }|a_{-n}|^{\frac {1}{n}}\\{1 \over R}&=\limsup _
      {n\rightarrow \infty }|a_{n}|^{\frac {1}{n}}.\end{aligned}}}  [{\begin
      {aligned}r&=\limsup _{n\rightarrow \infty }|a_{-n}|^{\frac {1}{n}}\\{1
      \over R}&=\limsup _{n\rightarrow \infty }|a_{n}|^{\frac {1}{n}}.\end
      {aligned}}]
We take R to be infinite when this latter lim_sup is zero.
Conversely, if we start with an annulus of the form A â¡ {z : r < |z − c| < R}
and a holomorphic function f(z) defined on A, then there always exists a unique
Laurent series with center c which converges (at least) on A and represents the
function f(z).
As an example, consider the following rational function, along with its partial
fraction expansion:
         f ( z ) &#xA0; = &#xA0;   1  ( z  &#x2212;  1 ) ( z  &#x2212;  2 i )
      &#xA0; = &#xA0;    1 + 2 i  5    (    1  z  &#x2212;  1    &#x2212;   1
      z  &#x2212;  2 i     )  .   {\displaystyle f(z)\ =\ {\frac {1}{(z{-}1)(z
      {-}2i)}}\ =\ {\frac {1+2i}{5}}\left({\frac {1}{z{-}1}}-{\frac {1}{z{-
      }2i}}\right).}  [{\displaystyle f(z)\ =\ {\frac {1}{(z{-}1)(z{-}2i)}}\ =\
      {\frac {1+2i}{5}}\left({\frac {1}{z{-}1}}-{\frac {1}{z{-}2i}}\right).}]
This function has singularities at z = 1 and z = 2i, where the denominator of
the expression is zero and the expression is therefore undefined. A Taylor
series about z = 0 (which yields a power series) will only converge in a disc
of radius 1, since it "hits" the singularity at 1.
However, there are three possible Laurent expansions about 0, depending on the
radius of z:
    * One series is defined on the inner disc where |z| < 1; it is the same as
      the Taylor series,
         f ( z ) =    1 + 2 i  5    &#x2211;  n = 0   &#x221E;    (    1  ( 2 i
      )  n + 1      &#x2212; 1  )   z  n   .   {\displaystyle f(z)={\frac
      {1+2i}{5}}\sum _{n=0}^{\infty }\left({\frac {1}{(2i)^{n+1}}}-1\right)z^
      {n}.}  [{\displaystyle f(z)={\frac {1+2i}{5}}\sum _{n=0}^{\infty }\left(
      {\frac {1}{(2i)^{n+1}}}-1\right)z^{n}.}]
This follows from the partial fraction form of the function, along with the
formula for the sum of a geometric_series,        1  z &#x2212; a    = &#x2212;
1 a    &#x2211;  n = 0   &#x221E;     (    z a    )   n      {\displaystyle
\textstyle {\frac {1}{z-a}}=-{\frac {1}{a}}\sum _{n=0}^{\infty }\left({\tfrac
{z}{a}}\right)^{n}}  [{\displaystyle \textstyle {\frac {1}{z-a}}=-{\frac {1}
{a}}\sum _{n=0}^{\infty }\left({\tfrac {z}{a}}\right)^{n}}] for      |  z  |  <
|  a  |    {\displaystyle |z|<|a|}  [{\displaystyle |z|<|a|}].
    * The second series is defined on the middle annulus where 1 < |z| < 2,
      caught between the two singularities,
         f ( z ) =    1 + 2 i  5    (   &#x2211;  n = 1   &#x221E;    z
      &#x2212; n   +  &#x2211;  n = 0   &#x221E;     1  ( 2 i  )  n + 1       z
      n    )  .   {\displaystyle f(z)={\frac {1+2i}{5}}\left(\sum _{n=1}^
      {\infty }z^{-n}+\sum _{n=0}^{\infty }{\frac {1}{(2i)^{n+1}}}z^
      {n}\right).}  [{\displaystyle f(z)={\frac {1+2i}{5}}\left(\sum _{n=1}^
      {\infty }z^{-n}+\sum _{n=0}^{\infty }{\frac {1}{(2i)^{n+1}}}z^
      {n}\right).}]
Here, we use the alternative form of the geometric series summation,        1
z &#x2212; a    =   1 z    &#x2211;  n = 0   &#x221E;     (    a z    )   n
{\displaystyle \textstyle {\frac {1}{z-a}}={\frac {1}{z}}\sum _{n=0}^{\infty
}\left({\tfrac {a}{z}}\right)^{n}}  [{\displaystyle \textstyle {\frac {1}{z-
a}}={\frac {1}{z}}\sum _{n=0}^{\infty }\left({\tfrac {a}{z}}\right)^{n}}] for
|  a  |  <  |  z  |    {\displaystyle |a|<|z|}  [{\displaystyle |a|<|z|}].
    * The third series is defined on the infinite outer annulus where 2 <
      |z| < â,
         f ( z ) =    1 + 2 i  5    &#x2211;  n = 1   &#x221E;   ( 1 &#x2212;
      ( 2 i  )  n &#x2212; 1   )  z  &#x2212; n   .   {\displaystyle f(z)=
      {\frac {1+2i}{5}}\sum _{n=1}^{\infty }(1-(2i)^{n-1})z^{-n}.}  [
      {\displaystyle f(z)={\frac {1+2i}{5}}\sum _{n=1}^{\infty }(1-(2i)^{n-
      1})z^{-n}.}]
This series can be derived using geometric series as before, or by performing
polynomial long division of 1 by (x−1)(x−2i), not stopping with a remainder but
continuing into x−n terms; indeed, the "outer" Laurent series of a rational
function is analogous to the decimal form of a fraction. (The "inner" Taylor
series expansion can be obtained similarly, just reversing the term_order in
the division algorithm.)
The case r = 0; i.e., a holomorphic function f(z) which may be undefined at a
single point c, is especially important.
The coefficient aâ1 of the Laurent expansion of such a function is called the
residue of f(z) at the singularity c; it plays a prominent role in the residue
theorem.
For an example of this, consider
         f ( z ) =    e  z   z   +  e   1 z    .   {\displaystyle f(z)={e^{z}
      \over z}+e^{\frac {1}{z}}.}  [f(z)={e^{z} \over z}+e^{\frac {1}{z}}.]
This function is holomorphic everywhere except at z = 0. To determine the
Laurent expansion about c = 0, we use our knowledge of the Taylor series of the
exponential_function:
         f ( z ) = &#x22EF; +  (   1  3 !    )   z  &#x2212; 3   +  (   1  2 !
      )   z  &#x2212; 2   + 2  z  &#x2212; 1   + 2 +  (   1  2 !    )  z +
      (   1  3 !    )   z  2   +  (   1  4 !    )   z  3   + &#x22EF;
      {\displaystyle f(z)=\cdots +\left({1 \over 3!}\right)z^{-3}+\left({1
      \over 2!}\right)z^{-2}+2z^{-1}+2+\left({1 \over 2!}\right)z+\left({1
      \over 3!}\right)z^{2}+\left({1 \over 4!}\right)z^{3}+\cdots }  [f
      (z)=\cdots +\left({1 \over 3!}\right)z^{-3}+\left({1 \over 2!}\right)z^{-
      2}+2z^{-1}+2+\left({1 \over 2!}\right)z+\left({1 \over 3!}\right)z^
      {2}+\left({1 \over 4!}\right)z^{3}+\cdots ]
and we find that the residue is 2.
***** Uniqueness[edit] *****
Suppose a function f(z) holomorphic on the annulus r < |z â c| < R has two
Laurent series:
         f ( z ) =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;    a  n     (  z
      &#x2212; c  )   n   =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;    b  n
      (  z &#x2212; c  )   n   .   {\displaystyle f(z)=\sum _{n=-\infty }^
      {\infty }a_{n}\left(z-c\right)^{n}=\sum _{n=-\infty }^{\infty }b_{n}\left
      (z-c\right)^{n}.}  [f(z)=\sum _{n=-\infty }^{\infty }a_{n}\left(z-
      c\right)^{n}=\sum _{n=-\infty }^{\infty }b_{n}\left(z-c\right)^{n}.]
Multiply both sides with       (  z &#x2212; c  )   &#x2212; k &#x2212; 1
{\displaystyle \left(z-c\right)^{-k-1}}  [\left(z-c\right)^{-k-1}], where k is
an arbitrary integer, and integrate on a path Î³ inside the annulus,
             &#x222E;       &#x03B3;   &#x2061;  &#x2211;  n = &#x2212;
      &#x221E;   &#x221E;    a  n     (  z &#x2212; c  )   n &#x2212; k
      &#x2212; 1    d  z =     &#x222E;       &#x03B3;   &#x2061;  &#x2211;  n
      = &#x2212; &#x221E;   &#x221E;    b  n     (  z &#x2212; c  )   n
      &#x2212; k &#x2212; 1    d  z .   {\displaystyle \oint _{\gamma }\sum _
      {n=-\infty }^{\infty }a_{n}\left(z-c\right)^{n-k-1}\mathrm {d} z=\oint _
      {\gamma }\sum _{n=-\infty }^{\infty }b_{n}\left(z-c\right)^{n-k-1}\mathrm
      {d} z.}  [\oint _{\gamma }\sum _{n=-\infty }^{\infty }a_{n}\left(z-
      c\right)^{n-k-1}\mathrm {d} z=\oint _{\gamma }\sum _{n=-\infty }^{\infty
      }b_{n}\left(z-c\right)^{n-k-1}\mathrm {d} z.]
The series converges uniformly on     r + &#x03F5; &#x2264;  |  z &#x2212; c  |
&#x2264; R &#x2212; &#x03F5;   {\displaystyle r+\epsilon \leq |z-c|\leq R-
\epsilon }  [r+\epsilon \leq |z-c|\leq R-\epsilon ], where Îµ is a positive
number small enough for Î³ to be contained in the constricted closed annulus,
so the integration and summation can be interchanged. Substituting the identity
             &#x222E;       &#x03B3;   &#x2061; ( z &#x2212; c  )  n &#x2212; k
      &#x2212; 1   d z = 2 &#x03C0; i  &#x03B4;  n k     {\displaystyle \oint _
      {\gamma }(z-c)^{n-k-1}dz=2\pi i\delta _{nk}}  [\oint _{\gamma }(z-c)^{n-
      k-1}dz=2\pi i\delta _{nk}]
into the summation yields
          a  k   =  b  k     {\displaystyle a_{k}=b_{k}}  [a_{k}=b_{k}]
Hence the Laurent series is unique.
***** Laurent polynomials[edit] *****
Main article: Laurent_polynomial
A Laurent polynomial is a Laurent series in which only finitely many
coefficients are non-zero. Laurent polynomials differ from ordinary polynomials
in that they may have terms of negative degree.
***** Principal part[edit] *****
The principal part of a Laurent series is the series of terms with negative
degree, that is
          &#x2211;  k = &#x2212; &#x221E;   &#x2212; 1    a  k   ( z &#x2212; c
      )  k   .   {\displaystyle \sum _{k=-\infty }^{-1}a_{k}(z-c)^{k}.}  [\sum
      _{k=-\infty }^{-1}a_{k}(z-c)^{k}.]
If the principal part of f is a finite sum, then f has a pole at c of order
equal to (negative) the degree of the highest term; on the other hand, if f has
an essential_singularity at c, the principal part is an infinite sum (meaning
it has infinitely many non-zero terms).
If the inner radius of convergence of the Laurent series for f is 0, then f has
an essential singularity at c if and only if the principal part is an infinite
sum, and has a pole otherwise.
If the inner radius of convergence is positive, f may have infinitely many
negative terms but still be regular at c, as in the example above, in which
case it is represented by a different Laurent series in a disk about c.
Laurent series with only finitely many negative terms are well-behavedâthey
are a power series divided by      z  k     {\displaystyle z^{k}}  [z^{k}], and
can be analyzed similarlyâwhile Laurent series with infinitely many negative
terms have complicated behavior on the inner circle of convergence.
**** Multiplication[edit] ****
Laurent series cannot in general be multiplied. Algebraically, the expression
for the terms of the product may involve infinite sums which need not converge
(one cannot take the convolution of integer sequences). Geometrically, the two
Laurent series may have non-overlapping annuli of convergence.
Two Laurent series with only finitely many negative terms can be multiplied:
algebraically, the sums are all finite; geometrically, these have poles at c,
and inner radius of convergence 0, so they both converge on an overlapping
annulus.
Thus when defining formal_Laurent_series, one requires Laurent series with only
finitely many negative terms.
Similarly, the sum of two convergent Laurent series need not converge, though
it is always defined formally, but the sum of two bounded below Laurent series
(or any Laurent series on a punctured disk) has a non-empty annulus of
convergence.
***** See also[edit] *****
    * Puiseux_series
    * Mittag-Leffler's_theorem
    * Formal_Laurent_series — Laurent series considered formally, with
      coefficients from an arbitrary commutative_ring, without regard for
      convergence, and with only finitely many negative terms, so that
      multiplication is always defined.
    * Z-transform — the special case where the Laurent series is taken about
      zero has much use in time series analysis.
    * Fourier_series — the substitution     z =  e  &#x03C0; i w
      {\displaystyle z=e^{\pi iw}}  [z=e^{\pi iw}] transforms a Laurent series
      into a Fourier series, or conversely. This is used in the q-series
      expansion of the j-invariant.
    * PadÃ©_approximant — Another technique used when a Taylor_series is not
      viable
***** References[edit] *****
   1. ^Rodriguez, Rubi; Kra, Irwin; Gilman,_Jane_P. (2012), Complex_Analysis:
      In_the_Spirit_of_Lipman_Bers, Graduate Texts in Mathematics, 245,
      Springer, p. 12, ISBN 9781441973238
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
   3. .
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Laurent_series", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
O'Connor,_John_J.; Robertson,_Edmund_F., "Laurent_series", MacTutor_History_of
Mathematics_archive, University_of_St_Andrews
.
Weisstein,_Eric_W. "Laurent_Series". MathWorld.
Laurent_Series_and_Mandelbrot_set_by_Robert_Munafo

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Laurent_series&oldid=890438602"
Categories:
    * Complex_analysis
    * Series_expansions
Hidden categories:
    * Articles_with_short_description
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * LietuviÅ³
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 1 April 2019, at 10:46 (UTC).
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
