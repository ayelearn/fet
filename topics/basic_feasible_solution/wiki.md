The following text has been accessed from https://en.wikipedia.org/wiki/Basic_feasible_solution at Fri Aug 9 02:38:11 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Basic feasible solution ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
                        This article relies largely or entirely on a single
[Question_book-new.svg] source. Relevant discussion may be found on the talk
                        page. Please help improve_this_article by introducing
                        citations to additional sources. (December 2018)
In the theory of linear_programming, a basic feasible solution (BFS) is,
intuitively, a solution with a minimal number of non-zero variables.
Geometrically, each BFS corresponds to a corner of the polyhedron of feasible
solutions. If there exists an optimal solution, then there exists an optimal
BFS. Hence, to find an optimal solution, it is sufficient to consider the BFS-
s. This fact is used by the simplex_algorithm, which essentially travels from
some BFS to another until an optimal one is found.[1]
⁰
***** Contents *****
    * 1_Definition
    * 2_Properties
    * 3_Examples
    * 4_Geometric_interpretation
    * 5_Application_in_the_Simplex_algorithm
    * 6_References
***** Definition[edit] *****
To define a BFS, we first present the linear program in the so-called
equational form:
      maximize       c  T    &#x22C5;  x    {\textstyle \mathbf {c^{T}} \cdot
      \mathbf {x} }  [{\textstyle \mathbf {c^{T}} \cdot \mathbf {x} }]
      subject to     A  x  =  b    {\displaystyle A\mathbf {x} =\mathbf {b} }
      [A\mathbf {x} =\mathbf {b} ] and      x  &#x2265; 0   {\displaystyle
      \mathbf {x} \geq 0}  [{\displaystyle \mathbf {x} \geq 0}]
where:
    *      c  T      {\displaystyle \mathbf {c^{T}} }  [{\displaystyle \mathbf
      {c^{T}} }] and      x    {\displaystyle \mathbf {x} }  [\mathbf {x} ] are
      vectors of size n (the number of variables);
    *     b    {\displaystyle \mathbf {b} }  [\mathbf {b} ] is a vector of size
      m (the number of constraints);
    *    A   {\displaystyle A}  [A] is an m-by-n matrix;
    *     x  &#x2265; 0   {\displaystyle \mathbf {x} \geq 0}  [{\displaystyle
      \mathbf {x} \geq 0}] means that all variables are non-negative.
Any linear program can be converted into an equational form by adding slack
variables.
As a preliminary clean-up step, we verify that:
    * The system     A  x  =  b    {\displaystyle A\mathbf {x} =\mathbf {b} }
      [A\mathbf {x} =\mathbf {b} ] has at least one solution (otherwise the
      whole LP has no solution and there is nothing more to do);
    * All m rows of the matrix     A   {\displaystyle A}  [A] are linearly
      independent, i.e., its rank is m (otherwise we can just delete redundant
      rows without changing the LP).
Typically m < n, so the system     A  x  =  b    {\displaystyle A\mathbf {x}
=\mathbf {b} }  [A\mathbf {x} =\mathbf {b} ] has many solutions; each such
solution is called a feasible solution of the LP.
Let B be a subset of m indices from {1,...,n}. Denote by      A  B
{\displaystyle A_{B}}  [A_B] the square m-by-m matrix made of the m columns of
A   {\displaystyle A}  [A] indexed by B. If      A  B     {\displaystyle A_{B}}
[A_B] is nonsingular, the columns indexed by B are a basis of the column_space
of     A   {\displaystyle A}  [A]. In this case, we call B a basis of the LP.
Since the rank of     A   {\displaystyle A}  [A] is m, it has at least one
basis; since     A   {\displaystyle A}  [A] has n columns, it has at most
(   n m   )      {\displaystyle {\binom {n}{m}}}  [{\displaystyle {\binom {n}
{m}}}] bases.
Given a basis B, we say that a feasible solution      x    {\displaystyle
\mathbf {x} }  [\mathbf {x} ] is a basic feasible solution with basis B if all
its non-zero variables are indexed by B, i.e., for all     j &#x2209; B :
&#xA0; &#xA0;  x  j   = 0   {\displaystyle j\not \in B:~~x_{j}=0}  [
{\displaystyle j\not \in B:~~x_{j}=0}].
***** Properties[edit] *****
1. A BFS is determined only by the constraints of the LP (the matrix     A
{\displaystyle A}  [A] and the vector      b    {\displaystyle \mathbf {b} }
[\mathbf {b} ]); it does not depend on the optimization objective.
2. By definition, a BFS has at most m non-zero variables and at least n-m zero
variables. A BFS can have less than m non-zero variables; in that case, it can
have many different bases, all of which contain the indices of its non-zero
variables.
3. A feasible solution      x    {\displaystyle \mathbf {x} }  [\mathbf {x} ]
is basic if-and-only-if the columns of the matrix      A  K     {\displaystyle
A_{K}}  [{\displaystyle A_{K}}] are linearly independent, where K is the set of
indices of the non-zero elements of      x    {\displaystyle \mathbf {x} }
[\mathbf {x} ]. [1]:45
4. A BFS is uniquely determined by the basis B: for each basis B of m indices,
there is at most one BFS       x  B      {\displaystyle \mathbf {x_{B}} }  [
{\displaystyle \mathbf {x_{B}} }] with basis B. This is because       x  B
{\displaystyle \mathbf {x_{B}} }  [{\displaystyle \mathbf {x_{B}} }] must
satisfy the constraint      A  B     x  B    = b   {\displaystyle A_{B}\mathbf
{x_{B}} =b}  [{\displaystyle A_{B}\mathbf {x_{B}} =b}], and by definition of
basis the matrix      A  B     {\displaystyle A_{B}}  [A_B] is non-singular, so
the constraint has a unique solution. The opposite is not true: each BFS can
come from many different bases.
If the unique solution of      A  B     x  B    = b   {\displaystyle A_
{B}\mathbf {x_{B}} =b}  [{\displaystyle A_{B}\mathbf {x_{B}} =b}] satisfies the
non-negativity constraints, then the basis is called a feasible basis.
5. If a linear program has an optimal solution (i.e., it has a feasible
solution, and the set of feasible solutions is bounded), then it has an optimal
BFS. This is a consequence of the Bauer_maximum_principle: the objective of a
linear program is convex; the set of feasible solutions is convex (it is an
intersection of hyperspaces); therefore the objective attains its maximum in an
extreme point of the set of feasible solutions.
Since the number of BFS-s is finite and bounded by        (   n m   )
{\displaystyle {\binom {n}{m}}}  [{\displaystyle {\binom {n}{m}}}], an optimal
solution to any LP can be found in finite time by just evaluating the objective
function in all        (   n m   )      {\displaystyle {\binom {n}{m}}}  [
{\displaystyle {\binom {n}{m}}}]BFS-s. This is not the most efficient way to
solve an LP; the simplex_algorithm examines the BFS-s in a much more efficient
way.
***** Examples[edit] *****
Consider a linear program with the following constraints:
        x  1   + 5  x  2   + 3  x  3   + 4  x  4   + 6  x  5      = 14      x
2   + 3  x  3   + 5  x  4   + 6  x  5      = 7     &#x2200; i &#x2208; { 1 ,
&#x2026; , 5 } :  x  i      &#x2265; 0       {\displaystyle {\begin{aligned}x_
{1}+5x_{2}+3x_{3}+4x_{4}+6x_{5}&=14\\x_{2}+3x_{3}+5x_{4}+6x_{5}&=7\\\forall
i\in \{1,\ldots ,5\}:x_{i}&\geq 0\end{aligned}}}  [{\displaystyle {\begin
{aligned}x_{1}+5x_{2}+3x_{3}+4x_{4}+6x_{5}&=14\\x_{2}+3x_{3}+5x_{4}+6x_
{5}&=7\\\forall i\in \{1,\ldots ,5\}:x_{i}&\geq 0\end{aligned}}}]
The matrix A is:
   A =   (    1   5   3   4   6     0   1   3   5   6    )   &#xA0; &#xA0;
&#xA0; &#xA0; &#xA0;  b  = ( 14 &#xA0; &#xA0; 7 )   {\displaystyle A={\begin
{pmatrix}1&5&3&4&6\\0&1&3&5&6\end{pmatrix}}~~~~~\mathbf {b} =(14~~7)}  [
{\displaystyle A={\begin{pmatrix}1&5&3&4&6\\0&1&3&5&6\end{pmatrix}}~~~~~\mathbf
{b} =(14~~7)}]
Here, m=2 and there are 10 subsets of 2 indices, however, not all of them are
bases: the set {3,5} is not a basis since columns 3 and 5 are linearly
dependent.
The set B={2,4} is a basis, since the matrix      A  B   =   (    5   4     1
5    )     {\displaystyle A_{B}={\begin{pmatrix}5&4\\1&5\end{pmatrix}}}  [
{\displaystyle A_{B}={\begin{pmatrix}5&4\\1&5\end{pmatrix}}}] is non-singular.
The unique BFS corresponding to this basis is      x  B   = ( 0 &#xA0; &#xA0; 2
&#xA0; &#xA0; 0 &#xA0; &#xA0; 1 &#xA0; &#xA0; 0 )   {\displaystyle x_{B}=
(0~~2~~0~~1~~0)}  [{\displaystyle x_{B}=(0~~2~~0~~1~~0)}].
***** Geometric interpretation[edit] *****
[Elongated_pentagonal_orthocupolarotunda.png]
The set of all feasible solutions is an intersection of hyperspaces. Therefore,
it is a convex_polyhedron. If it is bounded, then it is a convex_polytope.
Each BFS corresponds to a vertex of this polytope. [1]:53-56
***** Application in the Simplex algorithm[edit] *****
Main article: simplex_algorithm
The simplex_algorithm keeps, at each point of its execution, a "current basis"
B (a subset of m out of n variables), a "current BFS", and a "current tableau".
The tableau is a representation of the linear program where the basic variables
are expressed in terms of the non-basic ones: [1]:65
        x  B      = p + Q  x  N       z    =  z  0   +  r  T    x  N
{\displaystyle {\begin{aligned}x_{B}&=p+Qx_{N}\\z&=z_{0}+r^{T}x_{N}\end
{aligned}}}
[{\displaystyle {\begin{aligned}x_{B}&=p+Qx_{N}\\z&=z_{0}+r^{T}x_{N}\end
{aligned}}}]
where      x  B     {\displaystyle x_{B}}  [x_{B}]is the vector of m basic
variables,      x  N     {\displaystyle x_{N}}  [x_N]is the vector of n non-
basic variables, and     z   {\displaystyle z}  [z]is the maximization
objective. Since non-basic variables equal 0, the current BFS is     p
{\displaystyle p}  [p], and the current maximization objective is      z  0
{\displaystyle z_{0}}  [z_{0}].
If all coefficients in     r   {\displaystyle r}  [r]are negative, then      z
0     {\displaystyle z_{0}}  [z_{0}]is an optimal solution, since all variables
(including all non-basic variables) must be at least 0, so the second line
implies     z &#x2264;  z  0     {\displaystyle z\leq z_{0}}  [{\displaystyle
z\leq z_{0}}].
If some coefficients in     r   {\displaystyle r}  [r]are positive, then it may
be possible to increase the maximization target. For example, if      x  5
{\displaystyle x_{5}}  [x_5]is non-basic and its coefficient in     r
{\displaystyle r}  [r]is positive, then increasing it above 0 may make     z
{\displaystyle z}  [z]larger. If it is possible to do so without violating
other constraints, then the increased variable becomes basic (it "enters the
base"), while another non-basic variable is decreased to 0 to keep the equality
constraints and thus becomes non-basic (it "exits the base").
If this process is done carefully, then it is possible to guarantee that     z
{\displaystyle z}  [z]increases until it reachces the optimal BFS.
***** References[edit] *****
   1. ^ a b c dBernd GÃ¤rtner and JiÅÃ­_MatouÅ¡ek (2006). Understanding and
      Using Linear Programming. Berlin: Springer. ISBN 3-540-30697-8.
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
   3. :44-48

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Basic_feasible_solution&oldid=899197737"
Categories:
    * Linear_programming
Hidden categories:
    * Articles_needing_additional_references_from_December_2018
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
Add_links
    * This page was last edited on 28 May 2019, at 14:03 (UTC).
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
