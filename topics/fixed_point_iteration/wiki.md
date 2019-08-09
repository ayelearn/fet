The following text has been accessed from https://en.wikipedia.org/wiki/Fixed-point_iteration at Fri Aug 9 02:32:44 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Fixed-point iteration ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article needs additional citations for verification. Please help improve_this
 article by adding_citations_to_reliable_sources. Unsourced material may be challenged
 and removed.
 Find sources: "Fixed-point_iteration" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (May 2010)(Learn_how_and_when_to_remove_this_template_message)
Main article: Infinite_compositions_of_analytic_functions
In numerical_analysis, fixed-point iteration is a method of computing fixed
points of iterated_functions.
More specifically, given a function     f   {\displaystyle f}  [f] defined on
the real_numbers with real values and given a point      x  0
{\displaystyle x_{0}}  [x_{0}] in the domain of     f   {\displaystyle f}  [f],
the fixed point iteration is
          x  n + 1   = f (  x  n   ) ,  n = 0 , 1 , 2 , &#x2026;
      {\displaystyle x_{n+1}=f(x_{n}),\,n=0,1,2,\dots }  [x_{n+1}=f(x_
      {n}),\,n=0,1,2,\dots ]
which gives rise to the sequence      x  0   ,  x  1   ,  x  2   , &#x2026;
{\displaystyle x_{0},x_{1},x_{2},\dots }  [x_{0},x_{1},x_{2},\dots ] which is
hoped to converge to a point     x   {\displaystyle x}  [x]. If     f
{\displaystyle f}  [f] is continuous, then one can prove that the obtained
x   {\displaystyle x}  [x] is a fixed point of     f   {\displaystyle f}  [f],
i.e.,
         f ( x ) = x .    {\displaystyle f(x)=x.\,}  [{\displaystyle f
      (x)=x.\,}]
More generally, the function     f   {\displaystyle f}  [f] can be defined on
any metric_space with values in that same space.
⁰
***** Contents *****
    * 1_Examples
    * 2_Applications
    * 3_Contractions
    * 4_Convergence_acceleration
    * 5_See_also
    * 6_References
    * 7_Further_reading
    * 8_External_links
***** Examples[edit] *****
    * A first simple and useful example is the Babylonian_method for computing
      the square_root of a>0, which consists in taking     f ( x ) =   1 2
      (    a x   + x  )    {\displaystyle f(x)={\frac {1}{2}}\left({\frac {a}
      {x}}+x\right)}  [f(x)={\frac {1}{2}}\left({\frac {a}{x}}+x\right)], i.e.
      the mean value of x and a/x, to approach the limit     x =   a
      {\displaystyle x={\sqrt {a}}}  [x={\sqrt {a}}] (from whatever starting
      point      x  0   &#x226B; 0   {\displaystyle x_{0}\gg 0}  [x_{0}\gg 0]).
      This is a special case of Newton's_method quoted below.
The fixed-point iteration xn+1 = sin xn with initial value x0 = 2 converges to
0. This example does not satisfy the assumptions of the Banach_fixed_point
theorem and so its speed of convergence is very slow.
    * The fixed-point iteration      x  n + 1   = cos &#x2061;  x  n
      {\displaystyle x_{n+1}=\cos x_{n}\,}  [x_{n+1}=\cos x_{n}\,] converges to
      the unique fixed point of the function     f ( x ) = cos &#x2061; x
      {\displaystyle f(x)=\cos x\,}  [f(x)=\cos x\,] for any starting point
      x  0   .   {\displaystyle x_{0}.}  [x_{0}.] This example does satisfy the
      assumptions of the Banach_fixed_point_theorem. Hence, the error after n
      steps satisfies      |   x  n   &#x2212; x  |  &#x2264;    q  n    1
      &#x2212; q     |   x  1   &#x2212;  x  0    |  = C  q  n
      {\displaystyle |x_{n}-x|\leq {q^{n} \over 1-q}|x_{1}-x_{0}|=Cq^{n}}  [
      {\displaystyle |x_{n}-x|\leq {q^{n} \over 1-q}|x_{1}-x_{0}|=Cq^{n}}]
      (where we can take     q = 0.85   {\displaystyle q=0.85}  [q=0.85], if we
      start from      x  0   = 1   {\displaystyle x_{0}=1}  [x_{0}=1].) When
      the error is less than a multiple of      q  n     {\displaystyle q^{n}}
      [q^{n}] for some constant q, we say that we have linear_convergence. The
      Banach fixed-point theorem allows one to obtain fixed-point iterations
      with linear convergence.
    * The fixed-point iteration      x  n + 1   = 2  x  n      {\displaystyle
      x_{n+1}=2x_{n}\,}  [x_{n+1}=2x_{n}\,] will diverge unless      x  0   = 0
      {\displaystyle x_{0}=0}  [x_{0}=0]. We say that the fixed point of     f
      ( x ) = 2 x    {\displaystyle f(x)=2x\,}  [f(x)=2x\,] is repelling.
    * The requirement that f is continuous is important, as the following
      example shows. The iteration
          x  n + 1   =   {       x  n   2   ,    x  n   &#x2260; 0     1 ,    x
      n   = 0         {\displaystyle x_{n+1}={\begin{cases}{\frac {x_{n}}
      {2}},&x_{n}\neq 0\\1,&x_{n}=0\end{cases}}}  [x_{n+1}={\begin{cases}{\frac
      {x_{n}}{2}},&x_{n}\neq 0\\1,&x_{n}=0\end{cases}}]
converges to 0 for all values of      x  0     {\displaystyle x_{0}}  [x_{0}].
However, 0 is not a fixed point of the function
         f ( x ) =   {      x 2   ,   x &#x2260; 0     1 ,   x = 0
      {\displaystyle f(x)={\begin{cases}{\frac {x}{2}},&x\neq 0\\1,&x=0\end
      {cases}}}  [f(x)={\begin{cases}{\frac {x}{2}},&x\neq 0\\1,&x=0\end
      {cases}}]
as this function is not continuous at     x = 0   {\displaystyle x=0}  [x=0],
and in fact has no fixed points.
***** Applications[edit] *****
    * Newton's_method for finding roots of a given differentiable function
      f ( x )   {\displaystyle f(x)}  [f(x)] is
                x  n + 1   =  x  n   &#x2212;    f (  x  n   )    f &#x2032;
            (  x  n   )    .   {\displaystyle x_{n+1}=x_{n}-{\frac {f(x_{n})}
            {f'(x_{n})}}.}  [{\displaystyle x_{n+1}=x_{n}-{\frac {f(x_{n})}{f'
            (x_{n})}}.}]
      If we write     g ( x ) = x &#x2212;    f ( x )    f &#x2032;  ( x )
      {\displaystyle g(x)=x-{\frac {f(x)}{f'(x)}}}  [g(x)=x-{\frac {f(x)}{f'
      (x)}}], we may rewrite the Newton iteration as the fixed-point iteration
                x  n + 1   = g (  x  n   )   {\displaystyle x_{n+1}=g(x_{n})}
            [x_{n+1}=g(x_{n})].
      If this iteration converges to a fixed point x of g, then
               x = g ( x ) = x &#x2212;    f ( x )    f &#x2032;  ( x )
            {\displaystyle x=g(x)=x-{\frac {f(x)}{f'(x)}}}  [x=g(x)=x-{\frac {f
            (x)}{f'(x)}}], so     f ( x )  /   f &#x2032;  ( x ) = 0.
            {\displaystyle f(x)/f'(x)=0.}  [{\displaystyle f(x)/f'(x)=0.}]
      The reciprocal of anything is nonzero, therefore f(x) = 0: x is a root of
      f. Under the assumptions of the Banach_fixed_point_theorem, the Newton
      iteration, framed as the fixed point method, demonstrates linear
      convergence. However, a more detailed analysis shows quadratic
      convergence, i.e.,
                |   x  n   &#x2212; x  |  < C  q   2  n       {\displaystyle
            |x_{n}-x|<Cq^{2^{n}}}  [|x_{n}-x|<Cq^{2^{n}}], under certain
            circumstances.
    * Halley's_method is similar to Newton's_method but, when it works
      correctly, its error is      |   x  n   &#x2212; x  |  < C  q   3  n
      {\displaystyle |x_{n}-x|<Cq^{3^{n}}}  [|x_{n}-x|<Cq^{3^{n}}] (cubic
      convergence). In general, it is possible to design methods that converge
      with speed     C  q   k  n       {\displaystyle Cq^{k^{n}}}  [Cq^{k^{n}}]
      for any     k &#x2208;  N    {\displaystyle k\in \mathbb {N} }  [k\in
      {\mathbb  N}]. As a general rule, the higher the k, the less stable it
      is, and the more computationally expensive it gets. For these reasons,
      higher order methods are typically not used.
    * RungeâKutta_methods and numerical ordinary_differential_equation
      solvers in general can be viewed as fixed point iterations. Indeed, the
      core idea when analyzing the A-stability of ODE solvers is to start with
      the special case      y &#x2032;  = a y   {\displaystyle y'=ay}  [y'=ay],
      where a is a complex_number, and to check whether the ODE solver
      converges to the fixed point     y = 0   {\displaystyle y=0}  [y=0]
      whenever the real part of a is negative.[a]
    * The PicardâLindelÃ¶f_theorem, which shows that ordinary differential
      equations have solutions, is essentially an application of the Banach
      fixed_point_theorem to a special sequence of functions which forms a
      fixed point iteration, constructing the solution to the equation. Solving
      an ODE in this way is called Picard iteration, Picard's method, or the
      Picard iterative process.
    * The iteration capability in Excel can be used to find solutions to the
      Colebrook_equation to an accuracy of 15 significant figures.[1][2]
    * Some of the "successive approximation" schemes used in dynamic
      programming to solve Bellman's_functional_equation are based on fixed
      point iterations in the space of the return function.[3][4]
***** Contractions[edit] *****
If a function     f   {\displaystyle f}  [f] defined on the real line with real
values is Lipschitz_continuous with Lipschitz constant     L < 1
{\displaystyle L<1}  [L<1], then this function has precisely one fixed point,
and the fixed-point iteration converges towards that fixed point for any
initial guess      x  0   .   {\displaystyle x_{0}.}  [x_{0}.] This theorem can
be generalized to any metric space.
Proof of this theorem:
Since     f   {\displaystyle f}  [f] is Lipschitz continuous with Lipschitz
constant     L < 1   {\displaystyle L<1}  [L<1], then for the sequence     {  x
n   , n = 0 , 1 , 2 , &#x2026; }   {\displaystyle \{x_{n},n=0,1,2,\ldots \}}  [
{\displaystyle \{x_{n},n=0,1,2,\ldots \}}], we have:
              |   x  2   &#x2212;  x  1    |  =  |  f (  x  1   ) &#x2212; f
      (  x  0   )  |     &#x2264; L  |   x  1   &#x2212;  x  0    |  ,      |
      x  3   &#x2212;  x  2    |  =  |  f (  x  2   ) &#x2212; f (  x  1   )  |
      &#x2264; L  |   x  2   &#x2212;  x  1    |  ,          &#x22EE;
      {\displaystyle {\begin{aligned}|x_{2}-x_{1}|=|f(x_{1})-f(x_{0})|&\leq
      L|x_{1}-x_{0}|,\\|x_{3}-x_{2}|=|f(x_{2})-f(x_{1})|&\leq L|x_{2}-x_
      {1}|,\\&\,\,\,\vdots \end{aligned}}}  [{\displaystyle {\begin{aligned}|x_
      {2}-x_{1}|=|f(x_{1})-f(x_{0})|&\leq L|x_{1}-x_{0}|,\\|x_{3}-x_{2}|=|f(x_
      {2})-f(x_{1})|&\leq L|x_{2}-x_{1}|,\\&\,\,\,\vdots \end{aligned}}}]
and
          |   x  n   &#x2212;  x  n &#x2212; 1    |  =  |  f (  x  n &#x2212; 1
      ) &#x2212; f (  x  n &#x2212; 2   )  |  &#x2264; L  |   x  n &#x2212; 1
      &#x2212;  x  n &#x2212; 2    |  .   {\displaystyle |x_{n}-x_{n-1}|=|f(x_
      {n-1})-f(x_{n-2})|\leq L|x_{n-1}-x_{n-2}|.}  [{\displaystyle |x_{n}-x_{n-
      1}|=|f(x_{n-1})-f(x_{n-2})|\leq L|x_{n-1}-x_{n-2}|.}]
Combining the above inequalities yields:
          |   x  n   &#x2212;  x  n &#x2212; 1    |  &#x2264;  L  n &#x2212; 1
      |   x  1   &#x2212;  x  0    |  .   {\displaystyle |x_{n}-x_{n-1}|\leq L^
      {n-1}|x_{1}-x_{0}|.}  [{\displaystyle |x_{n}-x_{n-1}|\leq L^{n-1}|x_{1}-
      x_{0}|.}]
Since     L < 1   {\displaystyle L<1}  [L<1],      L  n &#x2212; 1   &#x2192; 0
{\displaystyle L^{n-1}\rightarrow 0}  [L^{n-1}\rightarrow 0] as     n &#x2192;
&#x221E; .   {\displaystyle n\rightarrow \infty .}  [n \rightarrow \infty.]
Therefore, we can show     {  x  n   }   {\displaystyle \{x_{n}\}}  [\{x_{n}\}]
is a Cauchy_sequence and thus it converges to a point      x  &#x2217;
{\displaystyle x^{*}}  [x^{*}].
For the iteration      x  n   = f (  x  n &#x2212; 1   )   {\displaystyle x_
{n}=f(x_{n-1})}  [x_{n}=f(x_{n-1})], let     n   {\displaystyle n}  [n] go to
infinity on both sides of the equation, we obtain      x  &#x2217;   = f (  x
&#x2217;   )   {\displaystyle x^{*}=f(x^{*})}  [x^{*}=f(x^{*})]. This shows
that      x  &#x2217;     {\displaystyle x^{*}}  [x^{*}] is the fixed point for
f   {\displaystyle f}  [f]. So we proved the iteration will eventually converge
to a fixed-point.
This property is very useful because not all iterations can arrive at a
convergent fixed-point. When constructing a fixed-point iteration, it is very
important to make sure it converges. There are several fixed-point_theorems to
guarantee the existence of the fixed point, but since the iteration function is
continuous, we can usually use the above theorem to test if an iteration
converges or not. The proof of the generalized theorem to metric space is
similar.
***** Convergence acceleration[edit] *****
The speed of convergence of the iteration sequence can be increased by using a
convergence_acceleration method such as Aitken's_delta-squared_process. The
application of Aitken's method to fixed-point iteration is known as
Steffensen's_method, and it can be shown that Steffensen's method yields a rate
of convergence that is at least quadratic.
***** See also[edit] *****
    * Contraction_mapping
    * Root-finding_algorithm
    * Fixed-point_theorem
    * Fixed-point_combinator
    * Banach_fixed-point_theorem
    * Cobweb_plot
    * Markov_chain
    * Infinite_compositions_of_analytic_functions
    * Iterated_function
    * Convergence_and_fixed_point
***** References[edit] *****
   1. ^ One may also consider certain iterations A-stable if the iterates stay
      bounded for a long time, which is beyond the scope of this article.
   1. ^ M A Kumar (2010), Solve Implicit Equations (Colebrook) Within
      Worksheet, Createspace,
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
   3. ISBN 1-4528-1619-0
   4. ^ Brkic, Dejan (2017) Solution of the Implicit Colebrook Equation for
      Flow Friction Using Excel, Spreadsheets in Education (eJSiE): Vol. 10:
      Iss. 2, Article 2. Available at: https://sie.scholasticahq.com/article/
      4663-solution-of-the-implicit-colebrook-equation-for-flow-friction-using-
      excel
   5. ^ Bellman, R. (1957). Dynamic programming, Princeton University Press.
   6. ^ Sniedovich, M. (2010). Dynamic Programming: Foundations and Principles,
      Taylor_&_Francis.
***** Further reading[edit] *****
    * Burden, Richard L.; Faires, J. Douglas (1985). "Fixed-Point Iteration".
      Numerical Analysis (Third ed.). PWS Publishers. ISBN 0-87150-857-5.
Hoffman, Joe D.; Frankel, Steven (2001). "Fixed-Point_Iteration". Numerical
Methods for Engineers and Scientists (Second ed.). New York: CRC Press.
pp. 141â145. ISBN 0-8247-0443-6.
Judd,_Kenneth_L. (1998). "Fixed-Point_Iteration". Numerical Methods in
Economics. Cambridge: MIT Press. pp. 165â167. ISBN 0-262-10071-1.
***** External links[edit] *****
    * Fixed-point_algorithms_online
    * Fixed-point_iteration_online_calculator_(Mathematical_Assistant_on_Web)

Retrieved from "https://en.wikipedia.org/w/index.php?title=Fixed-
point_iteration&oldid=900087222"
Categories:
    * Root-finding_algorithms
    * Iterative_methods
    * Fixed-point_theorems
Hidden categories:
    * Articles_needing_additional_references_from_May_2010
    * All_articles_needing_additional_references
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
    * Deutsch
    * EspaÃ±ol
    * Italiano
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 3 June 2019, at 10:20 (UTC).
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
