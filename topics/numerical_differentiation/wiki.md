The following text has been accessed from https://en.wikipedia.org/wiki/Numerical_differentiation at Thu Aug 8 23:41:15 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Numerical differentiation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In numerical_analysis, numerical differentiation describes algorithms for
estimating the derivative of a mathematical_function or function subroutine
using values of the function and perhaps other knowledge about the function.
[Derivative.svg]
⁰
***** Contents *****
    * 1_Finite_difference_formulas
          o 1.1_Practical_considerations_using_floating-point_arithmetic
          o 1.2_Higher-order_methods
          o 1.3_Higher_derivatives
    * 2_Practical_Implementation
    * 3_Differential_quadrature
    * 4_Complex-variable_methods
    * 5_See_also
    * 6_References
    * 7_External_links
***** Finite difference formulas[edit] *****
The simplest method is to use finite difference approximations.
A simple two-point estimation is to compute the slope of a nearby secant_line
through the points (x, f(x)) and (x + h, f(x + h)).[1] Choosing a small number
h, h represents a small change in x, and it can be either positive or negative.
The slope of this line is
            f ( x + h ) &#x2212; f ( x )  h   .   {\displaystyle {\frac {f
      (x+h)-f(x)}{h}}.}  [{\displaystyle {\frac {f(x+h)-f(x)}{h}}.}]
This expression is Newton's difference_quotient (also known as a first-order
divided_difference).
The slope of this secant line differs from the slope of the tangent line by an
amount that is approximately proportional to h. As h approaches zero, the slope
of the secant line approaches the slope of the tangent line. Therefore, the
true derivative of f at x is the limit of the value of the difference quotient
as the secant lines get closer and closer to being a tangent line:
          f &#x2032;  ( x ) =  lim  h &#x2192; 0      f ( x + h ) &#x2212; f
      ( x )  h   .   {\displaystyle f'(x)=\lim _{h\to 0}{\frac {f(x+h)-f(x)}
      {h}}.}  [{\displaystyle f'(x)=\lim _{h\to 0}{\frac {f(x+h)-f(x)}{h}}.}]
Since immediately substituting 0 for h results in division_by_zero, calculating
the derivative directly can be unintuitive.
Equivalently, the slope could be estimated by employing positions (x â h) and
x.
Another two-point formula is to compute the slope of a nearby secant line
through the points (x - h, f(x â h)) and (x + h, f(x + h)). The slope of this
line is
            f ( x + h ) &#x2212; f ( x &#x2212; h )   2 h    .   {\displaystyle
      {\frac {f(x+h)-f(x-h)}{2h}}.}  [{\displaystyle {\frac {f(x+h)-f(x-h)}
      {2h}}.}]
This formula is known as the symmetric_difference_quotient. In this case the
first-order errors cancel, so the slope of these secant lines differ from the
slope of the tangent line by an amount that is approximately proportional to
h  2     {\displaystyle h^{2}}  [h^{2}]. Hence for small values of h this is a
more accurate approximation to the tangent line than the one-sided estimation.
Note however that although the slope is being computed at x, the value of the
function at x is not involved.
The estimation error is given by
         R =    &#x2212;  f  ( 3 )   ( c )  6    h  2     {\displaystyle R=
      {\frac {-f^{(3)}(c)}{6}}h^{2}}  [{\displaystyle R={\frac {-f^{(3)}(c)}
      {6}}h^{2}}],
where     c   {\displaystyle c}  [c] is some point between     x &#x2212; h
{\displaystyle x-h}  [{\displaystyle x-h}] and     x + h   {\displaystyle x+h}
[{\displaystyle x+h}]. This error does not include the rounding_error due to
numbers being represented and calculations being performed in limited
precision.
The symmetric difference quotient is employed as the method of approximating
the derivative in a number of calculators, including TI-82, TI-83, TI-84, TI-
85, all of which use this method with h = 0.001.[2][3]
**** Practical considerations using floating-point arithmetic[edit] ****
Example showing the difficulty of choosing     h   {\displaystyle h}  [h] due
to both rounding error and formula error
An important consideration in practice when the function is calculated using
floating-point_arithmetic is how small a value of h to choose. If chosen too
small, the subtraction will yield a large rounding_error. In fact, all the
finite-difference formulae are ill-conditioned[4] and due to cancellation will
produce a value of zero if h is small enough.[5] If too large, the calculation
of the slope of the secant line will be more accurately calculated, but the
estimate of the slope of the tangent by using the secant could be worse.
For the numerical derivative formula evaluated at x and x + h, a choice for h
that is small without producing a large rounding error is       &#x03B5;   x
{\displaystyle {\sqrt {\varepsilon }}x}  [{\displaystyle {\sqrt {\varepsilon
}}x}] (though not when x = 0), where the machine_epsilon Îµ is typically of the
order of 2.2Ã10â16. [6] A formula for h that balances the rounding error
against the secant error for optimum accuracy is[7]
         h = 2   &#x03B5;  |    f ( x )    f &#x2033;  ( x )    |
      {\displaystyle h=2{\sqrt {\varepsilon \left|{\frac {f(x)}{f''
      (x)}}\right|}}}  [{\displaystyle h=2{\sqrt {\varepsilon \left|{\frac {f
      (x)}{f''(x)}}\right|}}}]
(though not when      f &#x2033;  ( x ) = 0   {\displaystyle f''(x)=0}  [f''
(x)=0]), and to employ it will require knowledge of the function.
This epsilon is for double-precision (64-bit) variables: such calculations in
single precision are rarely useful. The resulting value is unlikely to be a
"round" number in binary, so it is important to realise that although x is a
machine-representable number, x + h almost certainly will not be. This means
that x + h will be changed (by rounding or truncation) to a nearby machine-
representable number, with the consequence that (x + h) â x will not equal h;
the two function evaluations will not be exactly h apart. In this regard, since
most decimal fractions are recurring sequences in binary (just as 1/3 is in
decimal) a seemingly round step such as h = 0.1 will not be a round number in
binary; it is 0.000110011001100...2 A possible approach is as follows:
 h := sqrt(eps) * x;
 xph := x + h;
 dx := xph - x;
 slope := (F(xph) - F(x)) / dx;
However, with computers, compiler_optimization facilities may fail to attend to
the details of actual computer arithmetic and instead apply the axioms of
mathematics to deduce that dx and h are the same. With C and similar languages,
a directive that xph is a volatile_variable will prevent this.
**** Higher-order methods[edit] ****
Further information: Finite_difference_coefficient
Higher-order methods for approximating the derivative, as well as methods for
higher derivatives, exist.
Given below is the five-point method for the first derivative (five-point
stencil in one dimension):[8]
          f &#x2032;  ( x ) =    &#x2212; f ( x + 2 h ) + 8 f ( x + h )
      &#x2212; 8 f ( x &#x2212; h ) + f ( x &#x2212; 2 h )   12 h    +    h  4
      30    f  ( 5 )   ( c ) ,   {\displaystyle f'(x)={\frac {-f(x+2h)+8f(x+h)-
      8f(x-h)+f(x-2h)}{12h}}+{\frac {h^{4}}{30}}f^{(5)}(c),}  [{\displaystyle
      f'(x)={\frac {-f(x+2h)+8f(x+h)-8f(x-h)+f(x-2h)}{12h}}+{\frac {h^{4}}
      {30}}f^{(5)}(c),}]
where     c &#x2208; [ x &#x2212; 2 h , x + 2 h ]   {\displaystyle c\in [x-
2h,x+2h]}  [{\displaystyle c\in [x-2h,x+2h]}].
For other stencil configurations and derivative orders, the Finite_Difference
Coefficients_Calculator is a tool that can be used to generate derivative
approximation methods for any stencil with any derivative order (provided a
solution exists).
**** Higher derivatives[edit] ****
Using Newton's difference quotient,
          f &#x2032;  ( x ) =  lim  h &#x2192; 0      f ( x + h ) &#x2212; f
      ( x )  h     {\displaystyle f'(x)=\lim _{h\to 0}{\frac {f(x+h)-f(x)}{h}}}
      [{\displaystyle f'(x)=\lim _{h\to 0}{\frac {f(x+h)-f(x)}{h}}}]
the following can be shown[9] (for n>0):
          f  ( n )   ( x ) =  lim  h &#x2192; 0     1  h  n      &#x2211;  k =
      0   n   ( &#x2212; 1  )  k + n      (   n k   )    f ( x + k h ) .
      {\displaystyle f^{(n)}(x)=\lim _{h\to 0}{\frac {1}{h^{n}}}\sum _{k=0}^{n}
      (-1)^{k+n}{\binom {n}{k}}f(x+kh).}  [{\displaystyle f^{(n)}(x)=\lim _
      {h\to 0}{\frac {1}{h^{n}}}\sum _{k=0}^{n}(-1)^{k+n}{\binom {n}{k}}f
      (x+kh).}]

***** Practical Implementation[edit] *****
A fast open source Python implementation of numerical derivatives using finite
differences is the findiff project. It features calculation of any derivative
and any accuracy order in an arbitrary number of dimensions.
***** Differential quadrature[edit] *****
Differential_quadrature is the approximation of derivatives by using weighted
sums of function values.[10][11] The name is in analogy with quadrature,
meaning numerical_integration, where weighted sums are used in methods such as
Simpson's_method or the Trapezoidal_rule. There are various methods for
determining the weight coefficients. Differential quadrature is used to solve
partial_differential_equations.
***** Complex-variable methods[edit] *****
The classical finite-difference approximations for numerical differentiation
are ill-conditioned. However, if     f   {\displaystyle f}  [f] is a
holomorphic_function, real-valued on the real line, which can be evaluated at
points in the complex plane near     x   {\displaystyle x}  [x], then there are
stable methods. For example,[5] the first derivative can be calculated by the
complex-step derivative formula:[12]
          f &#x2032;  ( x ) &#x2248; &#x2111; ( f ( x + i h ) )  /  h .
      {\displaystyle f'(x)\approx \Im (f(x+ih))/h.}  [{\displaystyle f'
      (x)\approx \Im (f(x+ih))/h.}]
The above formula is only valid for calculating a first-order derivative. A
generalization of the above for calculating derivatives of any order employ
multicomplex_numbers, resulting in multicomplex derivatives.[13]
In general, derivatives of any order can be calculated using Cauchy's_integral
formula:
          f  ( n )   ( a ) =    n !   2 &#x03C0; i        &#x222E;
      &#x03B3;   &#x2061;    f ( z )   ( z &#x2212; a  )  n + 1        d  z ,
      {\displaystyle f^{(n)}(a)={\frac {n!}{2\pi i}}\oint _{\gamma }{\frac {f
      (z)}{(z-a)^{n+1}}}\,\mathrm {d} z,}  [{\displaystyle f^{(n)}(a)={\frac
      {n!}{2\pi i}}\oint _{\gamma }{\frac {f(z)}{(z-a)^{n+1}}}\,\mathrm {d}
      z,}]
where the integration is done numerically.
Using complex variables for numerical differentiation was started by Lyness and
Moler in 1967.[14] A method based on numerical inversion of a complex Laplace
transform was developed by Abate and Dubner.[15] An algorithm that can be used
without requiring knowledge about the method or the character of the function
was developed by Fornberg.[4]
***** See also[edit] *****
    * Automatic_differentiation
    * Finite_difference
    * Five-point_stencil
    * Numerical_integration
    * Numerical_ordinary_differential_equations
    * Numerical_smoothing_and_differentiation
    * List_of_numerical_analysis_software
***** References[edit] *****
   1. ^ Richard L. Burden, J. Douglas Faires (2000), Numerical Analysis, (7th
      Ed), Brooks/Cole.
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
   3. ISBN 0-534-38216-9.
   4. ^Katherine Klippert Merseth (2003). Windows on Teaching Math: Cases of
      Middle and Secondary Classrooms. Teachers College Press. p. 34. ISBN 978-
      0-8077-4279-2.
   5. ^Tamara Lefcourt Ruby; James Sellers; Lisa Korf; Jeremy Van Horn; Mike
      Munn (2014). Kaplan AP Calculus AB & BC 2015. Kaplan Publishing. p. 299.
      ISBN 978-1-61865-686-5.
   6. ^ a b Numerical Differentiation of Analytic Functions, B Fornberg â ACM
      Transactions on Mathematical Software (TOMS), 1981.
   7. ^ a b Using Complex Variables to Estimate Derivatives of Real Functions,
      W. Squire, G. Trapp â SIAM REVIEW, 1998.
   8. ^ Following Numerical_Recipes in C, Chapter_5.7.
   9. ^ p._263.
  10. ^ Abramowitz & Stegun, Table 25.2.
  11. ^Shilov, George. Elementary Real and Complex Analysis.
  12. ^ Differential Quadrature and Its Application in Engineering: Engineering
      Applications, Chang Shu, Springer, 2000,
  13. ISBN 978-1-85233-209-9.
  14. ^ Advanced Differential Quadrature Methods, Yingyan Zhang, CRC Press,
      2009,
  15. ISBN 978-1-4200-8248-7.
  16. ^Martins, J. R. R. A.; Sturdza, P.; Alonso, J. J. (2003). "The Complex-
      Step Derivative Approximation". ACM Transactions on Mathematical
      Software. 29 (3): 245â262. CiteSeerX 10.1.1.141.8002. doi:10.1145/
      838250.838251.
  17. ^ http://russell.ae.utexas.edu/FinalPublications/ConferencePapers/
      2010Feb_SanDiego_AAS-10-218_mulicomplex.pdf
  18. ^Lyness, J. N.; Moler, C. B. (1967). "Numerical differentiation of
      analytic functions". SIAM J. Numer. Anal. 4: 202â210. doi:10.1137/
      0704019.
  19. ^Abate, J; Dubner, H (March 1968). "A New Method for Generating Power
      Series Expansions of Functions". SIAM J. Numer. Anal. 5 (1): 102â112.
      doi:10.1137/0705008.
***** External links[edit] *****
 Wikibooks has a book on the topic of: Numerical_Methods
    * http://mathworld.wolfram.com/NumericalDifferentiation.html
    * Numerical_Differentiation_Resources:_Textbook_notes,_PPT,_Worksheets,
      Audiovisual_YouTube_Lectures at Numerical_Methods_for_STEM_Undergraduate
    * ftp://math.nist.gov/pub/repository/diff/src/DIFF Fortran code for the
      numerical differentiation of a function using Neville's process to
      extrapolate from a sequence of simple polynomial approximations.
    * NAG_Library_numerical_differentiation_routines
    * http://graphulator.com Online_numerical_graphing_calculator_with_calculus
      function.
    * Boost._Math_numerical_differentiation,_including_finite_differencing_and
      the_complex_step_derivative
    * Complex_Step_Differentiation
    * Differentiation_With(out)_a_Difference by Nicholas_Higham, SIAM News.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Numerical_differentiation&oldid=901876290"
Categories:
    * Numerical_analysis
    * Differential_calculus
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
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 14 June 2019, at 21:53 (UTC).
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
