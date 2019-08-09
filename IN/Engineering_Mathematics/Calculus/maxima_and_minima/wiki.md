The following text has been accessed from https://en.wikipedia.org/wiki/Maxima_and_minima at Fri Aug 9 01:25:01 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Maxima and minima ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For use in statistics, see Sample_maximum_and_minimum.
"Extreme value" redirects here. For the concept in statistics, see Extreme
value_theory. For the concept in calculus, see Extreme_value_theorem.
"Maximum" and "Minimum" redirect here. For other uses, see Maximum_
(disambiguation) and Minimum_(disambiguation).
Local and global maxima and minima for cos(3πx)/x, 0.1≤x≤1.1
In mathematical_analysis, the maxima and minima (the respective plurals of
maximum and minimum) of a function, known collectively as extrema (the plural
of extremum), are the largest and smallest value of the function, either within
a given range (the local or relative extrema) or on the entire domain_of_a
function (the global or absolute extrema).[1][2][3] Pierre_de_Fermat was one of
the first mathematicians to propose a general technique, adequality, for
finding the maxima and minima of functions.
As defined in set_theory, the maximum and minimum of a set are the greatest_and
least_elements in the set, respectively. Unbounded infinite sets, such as the
set of real_numbers, have no minimum or maximum.
⁰
***** Contents *****
    * 1_Definition
    * 2_Search
    * 3_Examples
    * 4_Functions_of_more_than_one_variable
    * 5_Maxima_or_minima_of_a_functional
    * 6_In_relation_to_sets
    * 7_See_also
    * 8_References
    * 9_External_links
***** Definition[edit] *****
A real-valued function f defined on a domain X has a global (or absolute)
maximum point at x∗ if f(x∗) ≥ f(x) for all x in X. Similarly, the function has
a global (or absolute) minimum point at x∗ if f(x∗) ≤ f(x) for all x in X. The
value of the function at a maximum point is called the maximum value of the
function and the value of the function at a minimum point is called the minimum
value of the function. Symbolically, this can be written as follows:
          x  0   &#x2208;  X    {\displaystyle x_{0}\in \mathrm {X} }  [
      {\displaystyle x_{0}\in \mathrm {X} }] is a global maximum point of
      function     f :  X  &#x2192;  R    {\displaystyle f:\mathrm {X} \to
      \mathbb {R} }  [{\displaystyle f:\mathrm {X} \to \mathbb {R} }] if
      ( &#x2200; x &#x2208;  X  )  f (  x  0   ) &#x2265; f ( x ) .
      {\displaystyle (\forall x\in \mathrm {X} )\,f(x_{0})\geq f(x).}  [
      {\displaystyle (\forall x\in \mathrm {X} )\,f(x_{0})\geq f(x).}]
Similarly for global minimum point.
If the domain X is a metric_space then f is said to have a local (or relative)
maximum point at the point x∗ if there exists some ε > 0 such that f(x∗) ≥ f(x)
for all x in X within distance ε of x∗. Similarly, the function has a local
minimum point at x∗ if f(x∗) ≤ f(x) for all x in X within distance ε of x∗. A
similar definition can be used when X is a topological_space, since the
definition just given can be rephrased in terms of neighbourhoods.
Mathematically, the given definition is written as follows:
      Let     (  X  ,  d   X    )   {\displaystyle (\mathrm {X} ,d_{\mathrm {X}
      })}  [{\displaystyle (\mathrm {X} ,d_{\mathrm {X} })}] be a metric space
      and function     f :  X  &#x2192;  R    {\displaystyle f:\mathrm {X} \to
      \mathbb {R} }  [{\displaystyle f:\mathrm {X} \to \mathbb {R} }]. Then
      x  0   &#x2208;  X    {\displaystyle x_{0}\in \mathrm {X} }  [
      {\displaystyle x_{0}\in \mathrm {X} }] is a local maximum point of
      function     f   {\displaystyle f}  [f] if     ( &#x2203; &#x03B5; > 0 )
      {\displaystyle (\exists \varepsilon >0)}  [{\displaystyle (\exists
      \varepsilon >0)}] such that     ( &#x2200; x &#x2208;  X  )   d   X
      ( x ,  x  0   ) < &#x03B5;  &#x27F9;  f (  x  0   ) &#x2265; f ( x ) .
      {\displaystyle (\forall x\in \mathrm {X} )\,d_{\mathrm {X} }(x,x_
      {0})<\varepsilon \implies f(x_{0})\geq f(x).}  [{\displaystyle (\forall
      x\in \mathrm {X} )\,d_{\mathrm {X} }(x,x_{0})<\varepsilon \implies f(x_
      {0})\geq f(x).}]
Similarly for a local minimum point.
In both the global and local cases, the concept of a strict extremum can be
defined. For example, x∗ is a strict global maximum point if, for all x in X
with x â  x∗, we have f(x∗) > f(x), and x∗ is a strict local maximum point if
there exists some ε > 0 such that, for all x in X within distance ε of x∗ with
x â  x∗, we have f(x∗) > f(x). Note that a point is a strict global maximum
point if and only if it is the unique global maximum point, and similarly for
minimum points.
A continuous real-valued function with a compact domain always has a maximum
point and a minimum point. An important example is a function whose domain is a
closed (and bounded) interval of real_numbers (see the graph above).
***** Search[edit] *****
Finding global maxima and minima is the goal of mathematical_optimization. If a
function is continuous on a closed interval, then by the extreme_value_theorem
global maxima and minima exist. Furthermore, a global maximum (or minimum)
either must be a local maximum (or minimum) in the interior of the domain, or
must lie on the boundary of the domain. So a method of finding a global maximum
(or minimum) is to look at all the local maxima (or minima) in the interior,
and also look at the maxima (or minima) of the points on the boundary, and take
the largest (or smallest) one.
Likely the most important, yet quite obvious, feature of continuous real-valued
functions of a_real_variable is that they decrease before local minima and
increase afterwards, likewise for maxima. (Formally, if f is continuous real-
valued function of a real variable x then x0 is a local minimum iff there exist
a<x0<b such that f decreases on (a,x0) and increases on (x0,b))[4] A direct
consequence of this is the Fermat's_theorem, which states that local extrema
must occur at critical_points. One can distinguish whether a critical point is
a local maximum or local minimum by using the first_derivative_test, second
derivative_test, or higher-order_derivative_test, given sufficient
differentiability.
For any function that is defined piecewise, one finds a maximum (or minimum) by
finding the maximum (or minimum) of each piece separately, and then seeing
which one is largest (or smallest).
***** Examples[edit] *****
The global maximum of       x  x      {\displaystyle {\sqrt[{x}]{x}}}  [{\sqrt[
{x}]{x}}] occurs at x = e.
    * The function x2 has a unique global minimum at x = 0.
    * The function x3 has no global minima or maxima. Although the first
      derivative (3x2) is 0 at x = 0, this is an inflection_point.
    * The function       x  x      {\displaystyle {\sqrt[{x}]{x}}}  [{\sqrt[
      {x}]{x}}] has a unique global maximum at x = e. (See figure at right)
    * The function xâx has a unique global maximum over the positive real
      numbers at x = 1/e.
    * The function x3/3 â x has first derivative x2 â 1 and second
      derivative 2x. Setting the first derivative to 0 and solving for x gives
      stationary points at â1 and +1. From the sign of the second derivative
      we can see that â1 is a local maximum and +1 is a local minimum. Note
      that this function has no global maximum or minimum.
    * The function |x| has a global minimum at x = 0 that cannot be found by
      taking derivatives, because the derivative does not exist at x = 0.
    * The function cos(x) has infinitely many global maxima at 0, Â±2Ï, Â±4Ï,
      ..., and infinitely many global minima at Â±π, Â±3π, ....
    * The function 2 cos(x) â x has infinitely many local maxima and minima,
      but no global maximum or minimum.
    * The function cos(3Ïx)/x with 0.1 ≤ x ≤ 1.1 has a global maximum at x =
      0.1 (a boundary), a global minimum near x = 0.3, a local maximum near x =
      0.6, and a local minimum near x = 1.0. (See figure at top of page.)
    * The function x3 + 3x2 â 2x + 1 defined over the closed interval
      (segment) [â4,2] has a local maximum at x = â1â√15/3, a local
      minimum at x = â1+√15/3, a global maximum at x = 2 and a global minimum
      at x = â4.
***** Functions of more than one variable[edit] *****
Main article: Second_partial_derivative_test
Peano_surface, a counterexample to some criteria of local maxima of the 19th
century
For functions of more than one variable, similar conditions apply. For example,
in the (enlargeable) figure at the right, the necessary conditions for a local
maximum are similar to those of a function with only one variable. The first
partial_derivatives as to z (the variable to be maximized) are zero at the
maximum (the glowing dot on top in the figure). The second partial derivatives
are negative. These are only necessary, not sufficient, conditions for a local
maximum because of the possibility of a saddle_point. For use of these
conditions to solve for a maximum, the function z must also be differentiable
throughout. The second_partial_derivative_test can help classify the point as a
relative maximum or relative minimum. In contrast, there are substantial
differences between functions of one variable and functions of more than one
variable in the identification of global extrema. For example, if a bounded
differentiable function f defined on a closed interval in the real line has a
single critical point, which is a local minimum, then it is also a global
minimum (use the intermediate_value_theorem and Rolle's_theorem to prove this
by reductio_ad_absurdum). In two and more dimensions, this argument fails, as
the function
         f ( x , y ) =  x  2   +  y  2   ( 1 &#x2212; x  )  3   ,  x , y
      &#x2208;  R  ,   {\displaystyle f(x,y)=x^{2}+y^{2}(1-x)^{3},\qquad x,y\in
      \mathbb {R} ,}  [f(x,y)=x^{2}+y^{2}(1-x)^{3},\qquad x,y\in {\mathbb
      {R}},]
shows. Its only critical point is at (0,0), which is a local minimum with Æ
(0,0) = 0. However, it cannot be a global one, because Æ(2,3) = â5.
Multivariate functions
    * The global maximum is the point at the top
    * Counterexample: The red dot shows a local minimum that is not a global
      minimum
***** Maxima or minima of a functional[edit] *****
If the domain of a function for which an extremum is to be found consists
itself of functions, i.e. if an extremum is to be found of a functional, the
extremum is found using the calculus_of_variations.
***** In relation to sets[edit] *****
Maxima and minima can also be defined for sets. In general, if an ordered_set S
has a greatest_element m, m is a maximal_element. Furthermore, if S is a subset
of an ordered set T and m is the greatest element of S with respect to order
induced by T, m is a least_upper_bound of S in T. The similar result holds for
least_element, minimal_element and greatest_lower_bound. The maximum and
minimum function for sets are used in databases, and can be computed rapidly,
since the maximum (or minimum) of a set can be computed from the maxima of a
partition; formally, they are self-decomposable_aggregation_functions.
In the case of a general partial_order, the least element (smaller than all
other) should not be confused with a minimal element (nothing is smaller).
Likewise, a greatest_element of a partially_ordered_set (poset) is an upper
bound of the set which is contained within the set, whereas a maximal element m
of a poset A is an element of A such that if m â¤ b (for any b in A) then m =
b. Any least element or greatest element of a poset is unique, but a poset can
have several minimal or maximal elements. If a poset has more than one maximal
element, then these elements will not be mutually comparable.
In a totally_ordered set, or chain, all elements are mutually comparable, so
such a set can have at most one minimal element and at most one maximal
element. Then, due to mutual comparability, the minimal element will also be
the least element and the maximal element will also be the greatest element.
Thus in a totally ordered set we can simply use the terms minimum and maximum.
If a chain is finite then it will always have a maximum and a minimum. If a
chain is infinite then it need not have a maximum or a minimum. For example,
the set of natural_numbers has no maximum, though it has a minimum. If an
infinite chain S is bounded, then the closure Cl(S) of the set occasionally has
a minimum and a maximum, in such case they are called the greatest lower bound
and the least upper bound of the set S, respectively.
***** See also[edit] *****
    * Derivative_test
    * Infimum_and_supremum
    * Limit_superior_and_limit_inferior
    * Mechanical_equilibrium
    * Sample_maximum_and_minimum
    * Saddle_point
***** References[edit] *****
   1. ^Stewart,_James (2008). Calculus: Early Transcendentals (6th ed.).
      Brooks/Cole. ISBN 0-495-01166-5.
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
   3. ^Larson,_Ron; Edwards, Bruce H. (2009). Calculus (9th ed.). Brooks/Cole.
      ISBN 0-547-16702-4.
   4. ^Thomas,_George_B.; Weir, Maurice D.; Hass,_Joel (2010). Thomas'
      Calculus: Early Transcendentals (12th ed.). Addison-Wesley. ISBN 0-321-
      58876-2.
   5. ^Problems_in_mathematical_analysis. DemidovÇc, Boris P., Baranenkov, G.
      Moscow(IS): Moskva. 1964. ISBN 0846407612. OCLC 799468131.CS1 maint:
      others (link)
***** External links[edit] *****
 Wikimedia Commons has media related to Extrema_(calculus).
 Look up maxima, minima, or extremum in Wiktionary, the free dictionary.
    * Maxima_and_Minima From MathWorldâA Wolfram Web Resource.
    * Thomas_Simpson's_work_on_Maxima_and_Minima at Convergence
    * Application_of_Maxima_and_Minima_with_sub_pages_of_solved_problems

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Maxima_and_minima&oldid=907656336"
Categories:
    * Calculus
    * Mathematical_analysis
    * Mathematical_optimization
    * Superlatives
Hidden categories:
    * CS1_maint:_others
    * Commons_category_link_is_on_Wikidata
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * ChiShona
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Lumbaart
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 24 July 2019, at 11:17 (UTC).
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
