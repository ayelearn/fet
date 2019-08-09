The following text has been accessed from https://en.wikipedia.org/wiki/Residue_theorem at Thu Aug 8 22:52:29 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Residue theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Mathematical_analysis â Complex analysis
Complex_analysis
[Gamma_abs_3D.png]
Complex_numbers
    * Real_number
    * Imaginary_number
    * Complex_plane
    * Complex_conjugate
    * Unit_complex_number
Complex_functions
    * Complex-valued_function
    * Analytic_function
    * Holomorphic_function
    * CauchyâRiemann_equations
    * Formal_power_series
Basic_Theory
    * Zeros_and_poles
    * Cauchy's_integral_theorem
    * Local_primitive
    * Cauchy's_integral_formula
    * Winding_number
    * Laurent_series
    * Isolated_singularity
    * Residue theorem
    * Conformal_map
    * Schwarz_lemma
    * Harmonic_function
    * Laplace's_equation
Geometric_function_theory
People
    * Augustin-Louis_Cauchy
    * Leonhard_Euler
    * Carl_Friedrich_Gauss
    * Jacques_Hadamard
    * Kiyoshi_Oka
    * Bernhard_Riemann
    * Karl_Weierstrass
    * [Nuvola_apps_kmplot.svg] Analysis_portal
    * v
    * t
    * e
In complex_analysis, a discipline within mathematics, the residue theorem,
sometimes called Cauchy's residue theorem, is a powerful tool to evaluate line
integrals of analytic_functions over closed curves; it can often be used to
compute real integrals and infinite_series as well. It generalizes the Cauchy
integral_theorem and Cauchy's_integral_formula. From a geometrical perspective,
it is a special case of the generalized_Stokes'_theorem.
⁰
***** Contents *****
    * 1_Statement
    * 2_Examples
          o 2.1_An_integral_along_the_real_axis
          o 2.2_An_infinite_sum
    * 3_See_also
    * 4_References
    * 5_External_links
***** Statement[edit] *****
The statement is as follows:
Illustration of the setting.
Let U be a simply_connected open_subset of the complex_plane containing a
finite list of points a1, ..., an, and f a function defined and holomorphic on
U \{a1, ..., an}. Let Î³ be a closed rectifiable_curve in U which does not meet
any of the ak, and denote the winding_number of Î³ around ak by I(Î³, ak). The
line integral of f around Î³ is equal to 2Ïi times the sum of residues of f at
the points, each counted as many times as Î³ winds around the point:
             &#x222E;       &#x03B3;   &#x2061; f ( z )  d z = 2 &#x03C0; i
      &#x2211;  k = 1   n   I &#x2061; ( &#x03B3; ,  a  k   ) Res &#x2061; ( f
      ,  a  k   ) .   {\displaystyle \oint _{\gamma }f(z)\,dz=2\pi i\sum _
      {k=1}^{n}\operatorname {I} (\gamma ,a_{k})\operatorname {Res} (f,a_{k}).}
      [{\displaystyle \oint _{\gamma }f(z)\,dz=2\pi i\sum _{k=1}^
      {n}\operatorname {I} (\gamma ,a_{k})\operatorname {Res} (f,a_{k}).}]
If Î³ is a positively_oriented simple_closed_curve, I(Î³, ak) = 1 if ak is in
the interior of Î³, and 0 if not, so
             &#x222E;       &#x03B3;   &#x2061; f ( z )  d z = 2 &#x03C0; i
      &#x2211; Res &#x2061; ( f ,  a  k   )   {\displaystyle \oint _{\gamma }f
      (z)\,dz=2\pi i\sum \operatorname {Res} (f,a_{k})}  [{\displaystyle \oint
      _{\gamma }f(z)\,dz=2\pi i\sum \operatorname {Res} (f,a_{k})}]
with the sum over those ak inside Î³.
The relationship of the residue theorem to Stokes' theorem is given by the
Jordan_curve_theorem. The general plane_curve Î³ must first be reduced to a set
of simple closed curves {Î³i} whose total is equivalent to Î³ for integration
purposes; this reduces the problem to finding the integral of f dz along a
Jordan curve Î³i with interior V. The requirement that f be holomorphic on U0 =
U \ {ak} is equivalent to the statement that the exterior_derivative d(f dz) =
0 on U0. Thus if two planar regions V and W of U enclose the same subset {aj}
of {ak}, the regions V \ W and W \ V lie entirely in U0, and hence
          &#x222B;  V &#x2216; W   d ( f  d z ) &#x2212;  &#x222B;  W &#x2216;
      V   d ( f  d z )   {\displaystyle \int _{V\smallsetminus W}d(f\,dz)-\int
      _{W\smallsetminus V}d(f\,dz)}  [{\displaystyle \int _{V\smallsetminus W}d
      (f\,dz)-\int _{W\smallsetminus V}d(f\,dz)}]
is well-defined and equal to zero. Consequently, the contour integral of f dz
along Î³j = âV is equal to the sum of a set of integrals along paths Î»j,
each enclosing an arbitrarily small region around a single aj â the residues
of f (up to the conventional factor 2Ïi) at {aj}. Summing over {Î³j}, we
recover the final expression of the contour integral in terms of the winding
numbers {I(Î³, ak)}.
In order to evaluate real integrals, the residue theorem is used in the
following manner: the integrand is extended to the complex plane and its
residues are computed (which is usually easy), and a part of the real axis is
extended to a closed curve by attaching a half-circle in the upper or lower
half-plane, forming a semicircle. The integral over this curve can then be
computed using the residue theorem. Often, the half-circle part of the integral
will tend towards zero as the radius of the half-circle grows, leaving only the
real-axis part of the integral, the one we were originally interested in.
***** Examples[edit] *****
**** An integral along the real axis[edit] ****
The integral
          &#x222B;  &#x2212; &#x221E;   &#x221E;      e  i t x     x  2   + 1
      d x   {\displaystyle \int _{-\infty }^{\infty }{\frac {e^{itx}}{x^
      {2}+1}}\,dx}  [{\displaystyle \int _{-\infty }^{\infty }{\frac {e^{itx}}
      {x^{2}+1}}\,dx}]
The contour C.
arises in probability_theory when calculating the characteristic_function of
the Cauchy_distribution. It resists the techniques of elementary calculus but
can be evaluated by expressing it as a limit of contour_integrals.
Suppose t > 0 and define the contour C that goes along the real line from âa
to a and then counterclockwise along a semicircle centered at 0 from a to âa.
Take a to be greater than 1, so that the imaginary unit i is enclosed within
the curve. Now consider the contour integral
          &#x222B;  C    f ( z )   d z =  &#x222B;  C      e  i t z     z  2
      + 1     d z .   {\displaystyle \int _{C}{f(z)}\,dz=\int _{C}{\frac {e^
      {itz}}{z^{2}+1}}\,dz.}  [{\displaystyle \int _{C}{f(z)}\,dz=\int _{C}
      {\frac {e^{itz}}{z^{2}+1}}\,dz.}]
Since eitz is an entire_function (having no singularities at any point in the
complex plane), this function has singularities only where the denominator z2 +
1 is zero. Since z2 + 1 = (z + i)(z â i), that happens only where z = i or z
= âi. Only one of those points is in the region bounded by this contour.
Because f(z) is
                e  i t z     z  2   + 1       =    e  i t z    2 i     (    1
      z &#x2212; i    &#x2212;   1  z + i     )        =    e  i t z    2 i ( z
      &#x2212; i )    &#x2212;    e  i t z    2 i ( z + i )    ,
      {\displaystyle {\begin{aligned}{\frac {e^{itz}}{z^{2}+1}}&={\frac {e^
      {itz}}{2i}}\left({\frac {1}{z-i}}-{\frac {1}{z+i}}\right)\\&={\frac {e^
      {itz}}{2i(z-i)}}-{\frac {e^{itz}}{2i(z+i)}},\end{aligned}}}  [{\begin
      {aligned}{\frac {e^{itz}}{z^{2}+1}}&={\frac {e^{itz}}{2i}}\left({\frac
      {1}{z-i}}-{\frac {1}{z+i}}\right)\\&={\frac {e^{itz}}{2i(z-i)}}-{\frac
      {e^{itz}}{2i(z+i)}},\end{aligned}}]
the residue of f(z) at z = i is
          Res  z = i   &#x2061; f ( z ) =    e  &#x2212; t    2 i    .
      {\displaystyle \operatorname {Res} \limits _{z=i}f(z)={\frac {e^{-t}}
      {2i}}.}  [{\displaystyle \operatorname {Res} \limits _{z=i}f(z)={\frac
      {e^{-t}}{2i}}.}]
According to the residue theorem, then, we have
          &#x222B;  C   f ( z )  d z = 2 &#x03C0; i &#x22C5;  Res  z = i
      &#x2061; f ( z ) = 2 &#x03C0; i    e  &#x2212; t    2 i    = &#x03C0;  e
      &#x2212; t   .   {\displaystyle \int _{C}f(z)\,dz=2\pi i\cdot
      \operatorname {Res} \limits _{z=i}f(z)=2\pi i{\frac {e^{-t}}{2i}}=\pi e^
      {-t}.}  [{\displaystyle \int _{C}f(z)\,dz=2\pi i\cdot \operatorname {Res}
      \limits _{z=i}f(z)=2\pi i{\frac {e^{-t}}{2i}}=\pi e^{-t}.}]
The contour C may be split into a straight part and a curved arc, so that
          &#x222B;   s t r a i g h t    f ( z )  d z +  &#x222B;   a r c    f
      ( z )  d z = &#x03C0;  e  &#x2212; t      {\displaystyle \int _{\mathrm
      {straight} }f(z)\,dz+\int _{\mathrm {arc} }f(z)\,dz=\pi e^{-t}\,}  [\int
      _{\mathrm {straight} }f(z)\,dz+\int _{\mathrm {arc} }f(z)\,dz=\pi e^{-
      t}\,]
and thus
          &#x222B;  &#x2212; a   a   f ( z )  d z = &#x03C0;  e  &#x2212; t
      &#x2212;  &#x222B;   a r c    f ( z )  d z .   {\displaystyle \int _{-a}^
      {a}f(z)\,dz=\pi e^{-t}-\int _{\mathrm {arc} }f(z)\,dz.}  [\int _{-a}^{a}f
      (z)\,dz=\pi e^{-t}-\int _{\mathrm {arc} }f(z)\,dz.]
Using some estimations, we have
          |   &#x222B;   a r c       e  i t z     z  2   + 1     d z  |
      &#x2264; &#x03C0; a &#x22C5;  sup  arc    |    e  i t z     z  2   + 1
      |  &#x2264; &#x03C0; a &#x22C5;  sup  arc     1   |   z  2   + 1  |
      &#x2264;    &#x03C0; a    a  2   &#x2212; 1    ,   {\displaystyle
      \left|\int _{\mathrm {arc} }{\frac {e^{itz}}{z^{2}+1}}\,dz\right|\leq \pi
      a\cdot \sup _{\text{arc}}\left|{\frac {e^{itz}}{z^{2}+1}}\right|\leq \pi
      a\cdot \sup _{\text{arc}}{\frac {1}{|z^{2}+1|}}\leq {\frac {\pi a}{a^{2}-
      1}},}  [{\displaystyle \left|\int _{\mathrm {arc} }{\frac {e^{itz}}{z^
      {2}+1}}\,dz\right|\leq \pi a\cdot \sup _{\text{arc}}\left|{\frac {e^
      {itz}}{z^{2}+1}}\right|\leq \pi a\cdot \sup _{\text{arc}}{\frac {1}{|z^
      {2}+1|}}\leq {\frac {\pi a}{a^{2}-1}},}]
and
          lim  a &#x2192; &#x221E;      &#x03C0; a    a  2   &#x2212; 1    = 0.
      {\displaystyle \lim _{a\to \infty }{\frac {\pi a}{a^{2}-1}}=0.}  [
      {\displaystyle \lim _{a\to \infty }{\frac {\pi a}{a^{2}-1}}=0.}]
The estimate on the numerator follows since t > 0, and for complex numbers z
along the arc (which lies in the upper halfplane), the argument Ï of z lies
between 0 and Ï. So,
          |  e  i t z   |  =  |  e  i t  |  z  |  ( cos &#x2061; &#x03D5; + i
      sin &#x2061; &#x03D5; )   |  =  |  e  &#x2212; t  |  z  |  sin &#x2061;
      &#x03D5; + i t  |  z  |  cos &#x2061; &#x03D5;   |  =  e  &#x2212; t  |
      z  |  sin &#x2061; &#x03D5;   &#x2264; 1.   {\displaystyle \left|e^
      {itz}\right|=\left|e^{it|z|(\cos \phi +i\sin \phi )}\right|=\left|e^{-
      t|z|\sin \phi +it|z|\cos \phi }\right|=e^{-t|z|\sin \phi }\leq 1.}
      [\left|e^{itz}\right|=\left|e^{it|z|(\cos \phi +i\sin \phi
      )}\right|=\left|e^{-t|z|\sin \phi +it|z|\cos \phi }\right|=e^{-t|z|\sin
      \phi }\leq 1.]
Therefore,
          &#x222B;  &#x2212; &#x221E;   &#x221E;      e  i t z     z  2   + 1
      d z = &#x03C0;  e  &#x2212; t   .   {\displaystyle \int _{-\infty }^
      {\infty }{\frac {e^{itz}}{z^{2}+1}}\,dz=\pi e^{-t}.}  [{\displaystyle
      \int _{-\infty }^{\infty }{\frac {e^{itz}}{z^{2}+1}}\,dz=\pi e^{-t}.}]
If t < 0 then a similar argument with an arc Câ² that winds around âi rather
than i shows that
The contour Câ².
          &#x222B;  &#x2212; &#x221E;   &#x221E;      e  i t z     z  2   + 1
      d z = &#x03C0;  e  t   ,   {\displaystyle \int _{-\infty }^{\infty }
      {\frac {e^{itz}}{z^{2}+1}}\,dz=\pi e^{t},}  [{\displaystyle \int _{-
      \infty }^{\infty }{\frac {e^{itz}}{z^{2}+1}}\,dz=\pi e^{t},}]
and finally we have
          &#x222B;  &#x2212; &#x221E;   &#x221E;      e  i t z     z  2   + 1
      d z = &#x03C0;  e  &#x2212;  | t |    .   {\displaystyle \int _{-\infty
      }^{\infty }{\frac {e^{itz}}{z^{2}+1}}\,dz=\pi e^{-\left|t\right|}.}  [
      {\displaystyle \int _{-\infty }^{\infty }{\frac {e^{itz}}{z^
      {2}+1}}\,dz=\pi e^{-\left|t\right|}.}]
(If t = 0 then the integral yields immediately to elementary calculus methods
and its value is Ï.)
**** An infinite sum[edit] ****
The fact that Ï cot(Ïz) has simple poles with residue 1 at each integer can
be used to compute the sum
           &#x2211;  n = &#x2212; &#x221E;   &#x221E;   f ( n ) .
      {\displaystyle \displaystyle \sum _{n=-\infty }^{\infty }f(n).}  [
      {\displaystyle \displaystyle \sum _{n=-\infty }^{\infty }f(n).}]
Consider, for example, f(z) = zâ2. Let ÎN be the rectangle that is the
boundary of [âN â 1/2, N + 1/2]2 with positive orientation, with an integer
N. By the residue formula,
           1  2 &#x03C0; i     &#x222B;   &#x0393;  N     f ( z ) &#x03C0; cot
      &#x2061; ( &#x03C0; z )  d z =  Res  z = 0   +  &#x2211;    n = &#x2212;
      N   n &#x2260; 0     N    n  &#x2212; 2   .   {\displaystyle {\frac {1}
      {2\pi i}}\int _{\Gamma _{N}}f(z)\pi \cot(\pi z)\,dz=\operatorname {Res}
      \limits _{z=0}+\sum _{n=-N \atop n\neq 0}^{N}n^{-2}.}  [{\displaystyle
      {\frac {1}{2\pi i}}\int _{\Gamma _{N}}f(z)\pi \cot(\pi
      z)\,dz=\operatorname {Res} \limits _{z=0}+\sum _{n=-N \atop n\neq 0}^
      {N}n^{-2}.}]
The left-hand side goes to zero as N â â since the integrand has order O
(Nâ2). On the other hand,[1]
           z 2   cot &#x2061;  (   z 2   )  = 1 &#x2212;  B  2      z  2    2 !
      + &#x22EF; ;   B  2   =   1 6   .   {\displaystyle {\frac {z}{2}}\cot
      \left({\frac {z}{2}}\right)=1-B_{2}{\frac {z^{2}}{2!}}+\cdots ;\qquad B_
      {2}={\frac {1}{6}}.}  [{\displaystyle {\frac {z}{2}}\cot \left({\frac {z}
      {2}}\right)=1-B_{2}{\frac {z^{2}}{2!}}+\cdots ;\qquad B_{2}={\frac {1}
      {6}}.}]
(In fact, z/2 cot(z/2) = iz/1 â eâiz â iz/2.) Thus, the residue Resz = 0
is âÏ2/3. We conclude:
          &#x2211;  n = 1   &#x221E;     1  n  2     =    &#x03C0;  2   6
      {\displaystyle \sum _{n=1}^{\infty }{\frac {1}{n^{2}}}={\frac {\pi ^{2}}
      {6}}}  [{\displaystyle \sum _{n=1}^{\infty }{\frac {1}{n^{2}}}={\frac
      {\pi ^{2}}{6}}}]
which is a proof of the Basel_problem.
The same trick can be used to establish
         &#x03C0; cot &#x2061; ( &#x03C0; z ) =  lim  N &#x2192; &#x221E;
      &#x2211;  n = &#x2212; N   N   ( z &#x2212; n  )  &#x2212; 1   ,
      {\displaystyle \pi \cot(\pi z)=\lim _{N\to \infty }\sum _{n=-N}^{N}(z-n)^
      {-1},}  [{\displaystyle \pi \cot(\pi z)=\lim _{N\to \infty }\sum _{n=-N}^
      {N}(z-n)^{-1},}]
that is, the Eisenstein_series.
We take f(z) = (w â z)â1 with w a non-integer and we shall show the above
for w. The difficulty in this case is to show the vanishing of the contour
integral at infinity. We have:
          &#x222B;   &#x0393;  N        &#x03C0; cot &#x2061; ( &#x03C0; z )  z
      d z = 0   {\displaystyle \int _{\Gamma _{N}}{\frac {\pi \cot(\pi z)}
      {z}}\,dz=0}  [{\displaystyle \int _{\Gamma _{N}}{\frac {\pi \cot(\pi z)}
      {z}}\,dz=0}]
since the integrand is an even function and so the contributions from the
contour in the left-half plane and the contour in the right cancel each other
out. Thus,
          &#x222B;   &#x0393;  N     f ( z ) &#x03C0; cot &#x2061; ( &#x03C0; z
      )  d z =  &#x222B;   &#x0393;  N      (    1  w &#x2212; z    +   1 z
      )  &#x03C0; cot &#x2061; ( &#x03C0; z )  d z   {\displaystyle \int _
      {\Gamma _{N}}f(z)\pi \cot(\pi z)\,dz=\int _{\Gamma _{N}}\left({\frac {1}
      {w-z}}+{\frac {1}{z}}\right)\pi \cot(\pi z)\,dz}  [{\displaystyle \int _
      {\Gamma _{N}}f(z)\pi \cot(\pi z)\,dz=\int _{\Gamma _{N}}\left({\frac {1}
      {w-z}}+{\frac {1}{z}}\right)\pi \cot(\pi z)\,dz}]
goes to zero as N â â.
***** See also[edit] *****
    * Cauchy's_integral_formula
    * Glasser's_master_theorem
    * Jordan's_lemma
    * Methods_of_contour_integration
    * Morera's_theorem
    * Nachbin's_theorem
    * Residue_at_infinity
    * Logarithmic_form
***** References[edit] *****
   1. ^Whittaker,_E._T.; Watson,_G._N. (1902). A_Course_of_Modern_Analysis.
      Cambridge University Press. Â§ 7.2.
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
    * Ahlfors,_Lars (1979), Complex Analysis, McGraw Hill, ISBN 0-07-085008-9
MitroniviÄ, Dragoslav; KeÄkiÄ, Jovan (1984), The Cauchy method of residues:
Theory and applications, D. Reidel Publishing Company, ISBN 90-277-1623-4
LindelÃ¶f,_Ernst (1905), Le calcul des rÃ©sidus et ses applications Ã  la
thÃ©orie des fonctions, Editions Jacques Gabay (published 1989), ISBN 2-87647-
060-8
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Cauchy_integral_theorem",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Residue_theorem in MathWorld

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Residue_theorem&oldid=895353981"
Categories:
    * Theorems_in_complex_analysis
    * Analytic_functions
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
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * Nederlands
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 3 May 2019, at 17:35 (UTC).
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
