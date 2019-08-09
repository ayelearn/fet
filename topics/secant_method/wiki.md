The following text has been accessed from https://en.wikipedia.org/wiki/Secant_method at Fri Aug 9 02:32:48 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Secant method ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Root-finding method
The first two iterations of the secant method. The red curve shows the function
f, and the blue lines are the secants. For this particular case, the secant
method will not converge to the visible root.
In numerical_analysis, the secant method is a root-finding_algorithm that uses
a succession of roots of secant_lines to better approximate a root of a
function f. The secant method can be thought of as a finite-difference
approximation of Newton's_method. However, the method was developed
independently of Newton's method and predates it by over 3000 years.[1]
⁰
***** Contents *****
    * 1_The_method
    * 2_Derivation_of_the_method
    * 3_Convergence
    * 4_Comparison_with_other_root-finding_methods
    * 5_Generalizations
    * 6_A_computational_example
    * 7_Notes
    * 8_See_also
    * 9_References
    * 10_External_links
***** The method[edit] *****
The secant method is defined by the recurrence_relation
          x  n   =  x  n &#x2212; 1   &#x2212; f (  x  n &#x2212; 1   )     x
      n &#x2212; 1   &#x2212;  x  n &#x2212; 2     f (  x  n &#x2212; 1   )
      &#x2212; f (  x  n &#x2212; 2   )    =     x  n &#x2212; 2   f (  x  n
      &#x2212; 1   ) &#x2212;  x  n &#x2212; 1   f (  x  n &#x2212; 2   )   f
      (  x  n &#x2212; 1   ) &#x2212; f (  x  n &#x2212; 2   )    .
      {\displaystyle x_{n}=x_{n-1}-f(x_{n-1}){\frac {x_{n-1}-x_{n-2}}{f(x_{n-
      1})-f(x_{n-2})}}={\frac {x_{n-2}f(x_{n-1})-x_{n-1}f(x_{n-2})}{f(x_{n-1})-
      f(x_{n-2})}}.}  [{\displaystyle x_{n}=x_{n-1}-f(x_{n-1}){\frac {x_{n-1}-
      x_{n-2}}{f(x_{n-1})-f(x_{n-2})}}={\frac {x_{n-2}f(x_{n-1})-x_{n-1}f(x_{n-
      2})}{f(x_{n-1})-f(x_{n-2})}}.}]
As can be seen from the recurrence relation, the secant method requires two
initial values, x0 and x1, which should ideally be chosen to lie close to the
root.
***** Derivation of the method[edit] *****
Starting with initial values x0 and x1, we construct a line through the points
(x0, f(x0)) and (x1, f(x1)), as shown in the picture above. In
slopeâintercept form, the equation of this line is
         y =    f (  x  1   ) &#x2212; f (  x  0   )    x  1   &#x2212;  x  0
      ( x &#x2212;  x  1   ) + f (  x  1   ) .   {\displaystyle y={\frac {f(x_
      {1})-f(x_{0})}{x_{1}-x_{0}}}(x-x_{1})+f(x_{1}).}  [{\displaystyle y=
      {\frac {f(x_{1})-f(x_{0})}{x_{1}-x_{0}}}(x-x_{1})+f(x_{1}).}]
The root of this linear function, that is the value of x such that y = 0 is
         x =  x  1   &#x2212; f (  x  1   )     x  1   &#x2212;  x  0     f
      (  x  1   ) &#x2212; f (  x  0   )    .   {\displaystyle x=x_{1}-f(x_{1})
      {\frac {x_{1}-x_{0}}{f(x_{1})-f(x_{0})}}.}  [{\displaystyle x=x_{1}-f(x_
      {1}){\frac {x_{1}-x_{0}}{f(x_{1})-f(x_{0})}}.}]
We then use this new value of x as x2 and repeat the process, using x1 and x2
instead of x0 and x1. We continue this process, solving for x3, x4, etc., until
we reach a sufficiently high level of precision (a sufficiently small
difference between xn and xnâ1):
              x  2      =  x  1   &#x2212; f (  x  1   )     x  1   &#x2212;  x
      0     f (  x  1   ) &#x2212; f (  x  0   )    ,      x  3      =  x  2
      &#x2212; f (  x  2   )     x  2   &#x2212;  x  1     f (  x  2   )
      &#x2212; f (  x  1   )    ,          &#x22EE;      x  n      =  x  n
      &#x2212; 1   &#x2212; f (  x  n &#x2212; 1   )     x  n &#x2212; 1
      &#x2212;  x  n &#x2212; 2     f (  x  n &#x2212; 1   ) &#x2212; f (  x  n
      &#x2212; 2   )    .       {\displaystyle {\begin{aligned}x_{2}&=x_{1}-f
      (x_{1}){\frac {x_{1}-x_{0}}{f(x_{1})-f(x_{0})}},\\[6pt]x_{3}&=x_{2}-f(x_
      {2}){\frac {x_{2}-x_{1}}{f(x_{2})-f(x_{1})}},\\[6pt]&\,\,\,\vdots \\
      [6pt]x_{n}&=x_{n-1}-f(x_{n-1}){\frac {x_{n-1}-x_{n-2}}{f(x_{n-1})-f(x_{n-
      2})}}.\end{aligned}}}  [{\displaystyle {\begin{aligned}x_{2}&=x_{1}-f(x_
      {1}){\frac {x_{1}-x_{0}}{f(x_{1})-f(x_{0})}},\\[6pt]x_{3}&=x_{2}-f(x_{2})
      {\frac {x_{2}-x_{1}}{f(x_{2})-f(x_{1})}},\\[6pt]&\,\,\,\vdots \\[6pt]x_
      {n}&=x_{n-1}-f(x_{n-1}){\frac {x_{n-1}-x_{n-2}}{f(x_{n-1})-f(x_{n-
      2})}}.\end{aligned}}}]
***** Convergence[edit] *****
The iterates      x  n     {\displaystyle x_{n}}  [x_{n}] of the secant method
converge to a root of     f   {\displaystyle f}  [f], if the initial values
x  0     {\displaystyle x_{0}}  [x_{0}] and      x  1     {\displaystyle x_{1}}
[x_{1}] are sufficiently close to the root. The order_of_convergence is Ï,
where
         &#x03C6; =    1 +   5    2   &#x2248; 1.618   {\displaystyle \varphi =
      {\frac {1+{\sqrt {5}}}{2}}\approx 1.618}  [{\displaystyle \varphi ={\frac
      {1+{\sqrt {5}}}{2}}\approx 1.618}]
is the golden_ratio. In particular, the convergence is superlinear, but not
quite quadratic.
This result only holds under some technical conditions, namely that     f
{\displaystyle f}  [f] be twice continuously differentiable and the root in
question be simple (i.e., with multiplicity 1).
If the initial values are not close enough to the root, then there is no
guarantee that the secant method converges. There is no general definition of
"close enough", but the criterion has to do with how "wiggly" the function is
on the interval     [  x  0   ,  x  1   ]   {\displaystyle [x_{0},x_{1}]}  [[x_
{0},x_{1}]]. For example, if     f   {\displaystyle f}  [f] is differentiable
on that interval and there is a point where      f &#x2032;  = 0
{\displaystyle f'=0}  [{\displaystyle f'=0}] on the interval, then the
algorithm may not converge.
***** Comparison with other root-finding methods[edit] *****
The secant method does not require that the root remain bracketed, like the
bisection_method does, and hence it does not always converge. The false
position_method (or regula falsi) uses the same formula as the secant method.
However, it does not apply the formula on      x  n &#x2212; 1
{\displaystyle x_{n-1}}  [x_{n-1}] and      x  n &#x2212; 2     {\displaystyle
x_{n-2}}  [x_{n-2}], like the secant method, but on      x  n &#x2212; 1
{\displaystyle x_{n-1}}  [x_{n-1}] and on the last iterate      x  k
{\displaystyle x_{k}}  [x_{k}] such that     f (  x  k   )   {\displaystyle f
(x_{k})}  [f(x_{k})] and     f (  x  n &#x2212; 1   )   {\displaystyle f(x_{n-
1})}  [f(x_{n-1})] have a different sign. This means that the false_position
method always converges.
The recurrence formula of the secant method can be derived from the formula for
Newton's_method
          x  n   =  x  n &#x2212; 1   &#x2212;    f (  x  n &#x2212; 1   )    f
      &#x2032;  (  x  n &#x2212; 1   )      {\displaystyle x_{n}=x_{n-1}-{\frac
      {f(x_{n-1})}{f'(x_{n-1})}}}  [{\displaystyle x_{n}=x_{n-1}-{\frac {f(x_
      {n-1})}{f'(x_{n-1})}}}]
by using the finite-difference approximation
          f &#x2032;  (  x  n &#x2212; 1   ) &#x2248;    f (  x  n &#x2212; 1
      ) &#x2212; f (  x  n &#x2212; 2   )    x  n &#x2212; 1   &#x2212;  x  n
      &#x2212; 2      .   {\displaystyle f'(x_{n-1})\approx {\frac {f(x_{n-1})-
      f(x_{n-2})}{x_{n-1}-x_{n-2}}}.}  [{\displaystyle f'(x_{n-1})\approx
      {\frac {f(x_{n-1})-f(x_{n-2})}{x_{n-1}-x_{n-2}}}.}]
The secant method can be interpreted as a method in which the derivative is
replaced by an approximation and is thus a quasi-Newton_method.
If we compare Newton's method with the secant method, we see that Newton's
method converges faster (order 2 against Ï â 1.6). However, Newton's method
requires the evaluation of both     f   {\displaystyle f}  [f] and its
derivative      f &#x2032;    {\displaystyle f'}  [f'] at every step, while the
secant method only requires the evaluation of     f   {\displaystyle f}  [f].
Therefore, the secant method may occasionally be faster in practice. For
instance, if we assume that evaluating     f   {\displaystyle f}  [f] takes as
much time as evaluating its derivative and we neglect all other costs, we can
do two steps of the secant method (decreasing the logarithm of the error by a
factor Ï2 â 2.6) for the same cost as one step of Newton's method
(decreasing the logarithm of the error by a factor 2), so the secant method is
faster. If, however, we consider parallel processing for the evaluation of the
derivative, Newton's method proves its worth, being faster in time, though
still spending more steps.
***** Generalizations[edit] *****
Broyden's_method is a generalization of the secant method to more than one
dimension.
The following graph shows the function f in red and the last secant line in
bold blue. In the graph, the x intercept of the secant line seems to be a good
approximation of the root of f.
[Secant_method_example_code_result.svg]
***** A computational example[edit] *****
The secant method is applied to find a root of the function f(x) = x2 â 612.
Here is an implementation in the Python language (from calculation, we expect
that the iteration converges at x = 24.7386):
def f(x):
    return x**2. - 612.

N = 7
x = [0]*N
x[0] = 10.
x[1] = 30.

for i in range(2,N)
    f_xi1 = f(x[i-1])
    f_xi2 = f(x[i-2])
    x[i] = x[i-1] - f_xi1 * (x[i-1] - x[i-2]) / (f_xi1 - f_xi2)
end

root=x[-1]
***** Notes[edit] *****
   1. ^Papakonstantinou, J., The_Historical_Development_of_the_Secant_Method_in
      1-D, retrieved 2011-06-29
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
***** See also[edit] *****
    * False_position_method
***** References[edit] *****
    * Kaw, Autar; Kalu, Egwu (2008), Numerical_Methods_with_Applications (1st
      ed.)
.
Allen, Myron B.; Isaacson, Eli L. (1998). Numerical_analysis_for_applied
science. John_Wiley_&_Sons. pp. 188â195. ISBN 978-0-471-55266-6.
***** External links[edit] *****
    * Secant_Method Notes, PPT, Mathcad, Maple, Mathematica, Matlab at Holistic
      Numerical_Methods_Institute
    * Weisstein,_Eric_W. "Secant_Method". MathWorld.
    * v
    * t
    * e
Root-finding_algorithms
Bracketing_(no_derivative)     * Bisection_method
Quasi-Newton                   * Regula_falsi
                               * Secant method
Newton                         * Newton's_method
Hybrid_methods                 * Brent's_method
                               * Bairstow's_method
Polynomial methods             * JenkinsâTraub_method
                               * Laguerre's_method

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Secant_method&oldid=909919509"
Categories:
    * Root-finding_algorithms
Hidden categories:
    * Use_American_English_from_March_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * Articles_containing_Latin-language_text
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
    * Dansk
    * Deutsch
    * EspaÃ±ol
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
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 8 August 2019, at 13:45 (UTC).
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
