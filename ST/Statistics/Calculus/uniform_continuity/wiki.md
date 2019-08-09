The following text has been accessed from https://en.wikipedia.org/wiki/Uniform_continuity at Fri Aug 9 02:53:05 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Uniform continuity ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Function limiting the "growth" of distances of outputs uniformly across its
domain
The graph of     f ( x ) =    1 x      {\displaystyle f(x)={\tfrac {1}{x}}}  [
{\displaystyle f(x)={\tfrac {1}{x}}}] escapes the top and/or bottom of the
height  &#x00D7;  width  = 2 &#x03B5; &#x00D7; 2 &#x03B4;   {\displaystyle
{\text{height}}\times {\text{width}}=2\varepsilon \times 2\delta }  [
{\displaystyle {\text{height}}\times {\text{width}}=2\varepsilon \times 2\delta
}] window, however small the     &#x03B4;   {\displaystyle \delta }  [\delta ],
so     f ( x )   {\displaystyle f(x)}  [f(x)] is not uniformly continuous. The
function     g ( x ) =   x     {\displaystyle g(x)={\sqrt {x}}}  [
{\displaystyle g(x)={\sqrt {x}}}], on the other hand, is uniformly continuous.
In mathematics, a function f is uniformly continuous if, roughly speaking, it
is possible to guarantee that f(x) and f(y) be as close to each other as we
please by requiring only that x and y are sufficiently close to each other;
unlike ordinary continuity, the maximum distance between f(x) and f(y) cannot
depend on x and y themselves.
Continuous functions can fail to be uniformly continuous if they are unbounded
on a finite domain, such as     f ( x ) =    1 x      {\displaystyle f(x)=
{\tfrac {1}{x}}}  [{\displaystyle f(x)={\tfrac {1}{x}}}] on (0,1), or if their
slopes become unbounded on an infinite domain, such as     f ( x ) =  x  2
{\displaystyle f(x)=x^{2}}  [f(x)=x^{2}] on the real line. However, any
Lipschitz_map between metric_spaces is uniformly continuous, in particular any
isometry (distance-preserving map) .
Although ordinary continuity can be defined for functions between general
topological spaces, defining uniform continuity requires more structure. The
concept relies on comparing the sizes of neighbourhoods of distinct points, so
it requires a metric space, or more generally a uniform_space.
⁰
***** Contents *****
    * 1_Definition_for_functions_on_metric_spaces
    * 2_Local_continuity_versus_global_uniform_continuity
    * 3_Examples_and_counterexamples
    * 4_Properties
    * 5_Visualization
    * 6_History
    * 7_Other_characterisations
          o 7.1_Non-standard_analysis
          o 7.2_Cauchy_continuity
    * 8_Relations_with_the_extension_problem
    * 9_Generalization_to_topological_vector_spaces
    * 10_Generalization_to_uniform_spaces
    * 11_References
    * 12_Further_reading
***** Definition for functions on metric spaces[edit] *****
Given metric_spaces (X, d1) and (Y, d2), a function f : X â Y is called
uniformly continuous if for every real_number Îµ > 0 there exists real Î´ > 0
such that for every x, y â X with d1(x, y) < Î´, we have that d2(f(x), f
(y)) < Îµ.
If X and Y are subsets of the real_line, d1 and d2 can be the standard_one
dimensional_Euclidean_distance, yielding the definition: for all Îµ > 0 there
exists a Î´ > 0 such that for all x, y â X, |x â y| < Î´ implies |f
(x) â f(y)|< Îµ.
The difference between uniform continuity, versus ordinary continuity at every
point, is that in uniform continuity the value of Î´ depends only on Îµ and not
on the point in the domain.
***** Local continuity versus global uniform continuity[edit] *****
Continuity itself is a local property of a functionâthat is, a function f is
continuous, or not, at a particular point, and this can be determined by
looking only at the values of the function in an (arbitrarily small)
neighbourhood of that point. When we speak of a function being continuous on an
interval, we mean only that it is continuous at each point of the interval. In
contrast, uniform continuity is a global property of f, in the sense that the
standard definition refers to pairs of points rather than individual points. On
the other hand, it is possible to give a definition that is local in terms of
the natural extension f* (the characteristics of which at nonstandard points
are determined by the global properties of f), although it is not possible to
give a local definition of uniform continuity for an arbitrary hyperreal-valued
function, see below.
The mathematical statements that a function is continuous on an interval I and
the definition that a function is uniformly continuous on the same interval are
structurally very similar. Continuity of a function for every point x of an
interval can thus be expressed by a formula starting with the quantification
         &#x2200; x &#x2208; I  &#x2200; &#x03F5; > 0  &#x2203; &#x03B4; > 0
      &#x2200; y &#x2208; I :   |  x &#x2212; y  |  < &#x03B4;  &#x21D2;   |  f
      ( x ) &#x2212; f ( y )  |  < &#x03F5;  ,   {\displaystyle \forall x\in
      I\;\forall \epsilon >0\;\exists \delta >0\;\forall y\in I:\,|x-y|<\delta
      \,\Rightarrow \,|f(x)-f(y)|<\epsilon \,,}  [{\displaystyle \forall x\in
      I\;\forall \epsilon >0\;\exists \delta >0\;\forall y\in I:\,|x-y|<\delta
      \,\Rightarrow \,|f(x)-f(y)|<\epsilon \,,}]
whereas for uniform continuity, the order of the first, second, and third
quantifiers are rotated:
         &#x2200; &#x03F5; > 0  &#x2203; &#x03B4; > 0  &#x2200; x , y &#x2208;
      I :   |  x &#x2212; y  |  < &#x03B4;  &#x21D2;   |  f ( x ) &#x2212; f
      ( y )  |  < &#x03F5;   {\displaystyle \forall \epsilon >0\;\exists \delta
      >0\;\forall x,y\in I:\,|x-y|<\delta \,\Rightarrow \,|f(x)-f(y)|<\epsilon
      }  [{\displaystyle \forall \epsilon >0\;\exists \delta >0\;\forall x,y\in
      I:\,|x-y|<\delta \,\Rightarrow \,|f(x)-f(y)|<\epsilon }]
Thus for continuity at each point, one takes an arbitrary point x, and then
there must exist a distance Î´,
         &#x22EF; &#x2200; x  &#x2203; &#x03B4; &#x22EF; ,   {\displaystyle
      \cdots \forall x\,\exists \delta \cdots ,}  [\cdots \forall x\,\exists
      \delta \cdots ,]
while for uniform continuity a single Î´ must work uniformly for all points x
(and y):
         &#x22EF; &#x2203; &#x03B4;  &#x2200; x  &#x2200; y &#x22EF; .
      {\displaystyle \cdots \exists \delta \,\forall x\,\forall y\cdots .}
      [\cdots \exists \delta \,\forall x\,\forall y\cdots .]
***** Examples and counterexamples[edit] *****
    * Every Lipschitz_continuous map between two metric spaces is uniformly
      continuous. In particular, every function which is differentiable and has
      bounded derivative is uniformly continuous. More generally, every HÃ¶lder
      continuous function is uniformly continuous.
    * Despite being nowhere differentiable, the Weierstrass_function is
      everywhere uniformly continuous
    * Every member of a uniformly_equicontinuous set of functions is uniformly
      continuous.
    * The tangent_function is continuous on the interval (âÏ/2, Ï/2) but is
      not uniformly continuous on that interval.
    * The exponential function x      &#x21A6;    {\displaystyle \scriptstyle
      \mapsto }  [{\displaystyle \scriptstyle \mapsto }] ex is continuous
      everywhere on the real line but is not uniformly continuous on the line.
***** Properties[edit] *****
Every uniformly continuous function is continuous, but the converse does not
hold. Consider for instance the function     f &#x003A;  R  &#x2192;  R  , x
&#x21A6;  x  2     {\displaystyle f\colon \mathbb {R} \rightarrow \mathbb {R}
,x\mapsto x^{2}}  [{\displaystyle f\colon \mathbb {R} \rightarrow \mathbb {R}
,x\mapsto x^{2}}]. Given an arbitrarily small positive real number     &#x03F5;
{\displaystyle \epsilon }  [\epsilon ], uniform continuity requires the
existence of a positive number     &#x03B4;   {\displaystyle \delta }  [\delta
] such that for all      x  1   ,  x  2     {\displaystyle x_{1},x_{2}}  [x_
{1},x_{2}] with      |   x  1   &#x2212;  x  2    |  < &#x03B4;
{\displaystyle |x_{1}-x_{2}|<\delta }  [|x_{1}-x_{2}|<\delta ], we have      |
f (  x  1   ) &#x2212; f (  x  2   )  |  < &#x03F5;   {\displaystyle |f(x_{1})-
f(x_{2})|<\epsilon }  [|f(x_{1})-f(x_{2})|<\epsilon ]. But
         f ( x + &#x03B4; ) &#x2212; f ( x ) = 2 x &#x03B4; +  &#x03B4;  2   =
      &#x03B4; ( 2 x + &#x03B4; ) &#xA0; ,   {\displaystyle f(x+\delta )-f
      (x)=2x\delta +\delta ^{2}=\delta (2x+\delta )\ ,}  [f(x+\delta )-f
      (x)=2x\delta +\delta ^{2}=\delta (2x+\delta )\ ,]
and for all sufficiently large x this quantity is greater than     &#x03F5;
{\displaystyle \epsilon }  [\epsilon ].
Any absolutely_continuous function is uniformly continuous. On the other hand,
the Cantor_function is uniformly continuous but not absolutely continuous.
The image of a totally_bounded subset under a uniformly continuous function is
totally bounded. However, the image of a bounded subset of an arbitrary metric
space under a uniformly continuous function need not be bounded: as a
counterexample, consider the identity function from the integers endowed with
the discrete_metric to the integers endowed with the usual Euclidean_metric.
The HeineâCantor_theorem asserts that every continuous function on a compact
set is uniformly continuous. In particular, if a function is continuous on a
closed_bounded_interval of the real line, it is uniformly continuous on that
interval. The Darboux_integrability of continuous functions follows almost
immediately from this theorem.
If a real-valued function     f   {\displaystyle f}  [f] is continuous on
[ 0 , &#x221E; )   {\displaystyle [0,\infty )}  [[0,\infty )] and      lim  x
&#x2192; &#x221E;   f ( x )   {\displaystyle \lim _{x\to \infty }f(x)}  [\lim _
{x\to \infty }f(x)] exists (and is finite), then     f   {\displaystyle f}  [f]
is uniformly continuous. In particular, every element of      C  0   (  R  )
{\displaystyle C_{0}(\mathbb {R} )}  [C_{0}({\mathbb  {R}})], the space of
continuous functions on      R    {\displaystyle \mathbb {R} }  [\mathbb {R} ]
that vanish at infinity, is uniformly continuous. This is a generalization of
the Heine-Cantor theorem mentioned above, since      C  c   (  R  ) &#x2282;  C
0   (  R  )   {\displaystyle C_{c}(\mathbb {R} )\subset C_{0}(\mathbb {R} )}
[C_{c}({\mathbb  {R}})\subset C_{0}({\mathbb  {R}})].
***** Visualization[edit] *****
For a uniformly continuous function, there is for every given     &#x03F5; > 0
{\displaystyle \epsilon >0}  [\epsilon >0] a     &#x03B4; > 0   {\displaystyle
\delta >0}  [\delta >0] such that two values     f ( x )   {\displaystyle f(x)}
[f(x)] and     f ( y )   {\displaystyle f(y)}  [f(y)] have a maximal distance
&#x03F5;   {\displaystyle \epsilon }  [\epsilon ] whenever     x
{\displaystyle x}  [x] and     y   {\displaystyle y}  [y] do not differ for
more than     &#x03B4;   {\displaystyle \delta }  [\delta ]. Thus we can draw
around each point     ( x , f ( x ) )   {\displaystyle (x,f(x))}  [(x,f(x))] of
the graph a rectangle with height     2 &#x03F5;   {\displaystyle 2\epsilon }
[2\epsilon] and width     2 &#x03B4;   {\displaystyle 2\delta }  [2\delta] so
that the graph lies completely inside the rectangle and not directly above or
below. For functions that are not uniformly continuous, this isn't possible.
The graph might lie inside the rectangle for certain midpoints on the graph but
there are always midpoints of the rectangle on the graph where the function
lies above or below the rectangle.
    * For uniformly continuous functions, there is for each     &#x03F5; > 0
      {\displaystyle \epsilon >0}  [\epsilon >0] a     &#x03B4; > 0
      {\displaystyle \delta >0}  [\delta >0] such that when we draw a rectangle
      around each point of the graph with width     2 &#x03B4;   {\displaystyle
      2\delta }  [2\delta] and height     2 &#x03F5;   {\displaystyle 2\epsilon
      }  [2\epsilon], the graph lies completely inside the rectangle.
    * For functions that are not uniformly continuous, there is an     &#x03F5;
      > 0   {\displaystyle \epsilon >0}  [\epsilon >0] such that regardless of
      the     &#x03B4; > 0   {\displaystyle \delta >0}  [\delta >0] there are
      always points on the graph, when we draw a     2 &#x03F5;
      {\displaystyle 2\epsilon }  [2\epsilon]-    2 &#x03B4;   {\displaystyle
      2\delta }  [2\delta]-rectangle around it, there are values directly above
      or below the rectangle. There might be midpoints where the graph is
      completely inside the rectangle but this is not true for every midpoint.
***** History[edit] *****
The first published definition of uniform continuity was by Heine in 1870, and
in 1872 he published a proof that a continuous function on an open interval
need not be uniformly continuous. The proofs are almost verbatim given by
Dirichlet in his lectures on definite integrals in 1854. The definition of
uniform continuity appears earlier in the work of Bolzano where he also proved
that continuous functions on an open interval do not need to be uniformly
continuous. In addition he also states that a continuous function on a closed
interval is uniformly continuous, but he does not give a complete proof.[1]
***** Other characterisations[edit] *****
**** Non-standard analysis[edit] ****
In non-standard_analysis, a real-valued function f of a real variable is
microcontinuous at a point a precisely if the difference f*(a + Î´) â f*(a)
is infinitesimal whenever Î´ is infinitesimal. Thus f is continuous on a set A
in R precisely if f* is microcontinuous at every real point a â A. Uniform
continuity can be expressed as the condition that (the natural extension of) f
is microcontinuous not only at real points in A, but at all points in its non-
standard counterpart (natural extension) *A in *R. Note that there exist
hyperreal-valued functions which meet this criterion but are not uniformly
continuous, as well as uniformly continuous hyperreal-valued functions which do
not meet this criterion, however, such functions cannot be expressed in the
form f* for any real-valued function f. (see non-standard_calculus for more
details and examples).
**** Cauchy continuity[edit] ****
For a function between metric spaces, uniform continuity implies Cauchy
continuity (Fitzpatrick_2006). More specifically, let A be a subset of Rn. If a
function f : A â Rm is uniformly continuous then for every pair of sequences
xn and yn such that
          lim  n &#x2192; &#x221E;    |   x  n   &#x2212;  y  n    |  = 0
      {\displaystyle \lim _{n\to \infty }|x_{n}-y_{n}|=0}  [{\displaystyle \lim
      _{n\to \infty }|x_{n}-y_{n}|=0}]
we have
          lim  n &#x2192; &#x221E;    |  f (  x  n   ) &#x2212; f (  y  n   )
      |  = 0.   {\displaystyle \lim _{n\to \infty }|f(x_{n})-f(y_{n})|=0.}  [
      {\displaystyle \lim _{n\to \infty }|f(x_{n})-f(y_{n})|=0.}]
***** Relations with the extension problem[edit] *****
Let X be a metric space, S a subset of X, R a complete metric space, and     f
: S &#x2192; R   {\displaystyle f:S\rightarrow R}  [f:S\rightarrow R] a
continuous function. When can f be extended to a continuous function on all of
X?
If S is closed in X, the answer is given by the Tietze_extension_theorem:
always. So it is necessary and sufficient to extend f to the closure of S in X:
that is, we may assume without loss of generality that S is dense in X, and
this has the further pleasant consequence that if the extension exists, it is
unique.
Let us suppose moreover that X is complete, so that X is the completion of S.
Then a continuous function     f : S &#x2192; R   {\displaystyle f:S\rightarrow
R}  [f:S\rightarrow R] extends to all of X if and only if f is Cauchy-
continuous, i. e., the image under f of a Cauchy sequence remains Cauchy. (In
general, Cauchy continuity is necessary and sufficient for extension of f to
the completion of X, so is a priori stronger than extendability to X.)
It is easy to see that every uniformly continuous function is Cauchy-continuous
and thus extends to X. The converse does not hold, since the function     f : R
&#x2192; R , x &#x21A6;  x  2     {\displaystyle f:R\rightarrow R,x\mapsto x^
{2}}  [{\displaystyle f:R\rightarrow R,x\mapsto x^{2}}] is, as seen above, not
uniformly continuous, but it is continuous and thus -- since R is complete -
- Cauchy continuous. In general, for functions defined on unbounded spaces like
R, uniform continuity is a rather strong condition. It is desirable to have a
weaker condition from which to deduce extendability.
For example, suppose a > 1 is a real number. At the precalculus level, the
function     f : x &#x21A6;  a  x     {\displaystyle f:x\mapsto a^{x}}  [f:
x\mapsto a^{x}] can be given a precise definition only for rational values of x
(assuming the existence of qth roots of positive real numbers, an application
of the Intermediate Value Theorem). One would like to extend f to a function
defined on all of R. The identity
         f ( x + &#x03B4; ) &#x2212; f ( x ) =  a  x   (  a  &#x03B4;
      &#x2212; 1 )   {\displaystyle f(x+\delta )-f(x)=a^{x}(a^{\delta }-1)}  [
      {\displaystyle f(x+\delta )-f(x)=a^{x}(a^{\delta }-1)}]
shows that f is not uniformly continuous on the set Q of all rational numbers;
however for any bounded interval I the restriction of f to     Q &#x2229; I
{\displaystyle Q\cap I}  [Q\cap I] is uniformly continuous, hence Cauchy-
continuous, hence f extends to a continuous function on I. But since this holds
for every I, there is then a unique extension of f to a continuous function on
all of R.
More generally, a continuous function     f : S &#x2192; R   {\displaystyle f:
S\rightarrow R}  [f:S\rightarrow R] whose restriction to every bounded subset
of S is uniformly continuous is extendable to X, and the converse holds if X is
locally_compact.
A typical application of the extendability of a uniformly continuous function
is the proof of the inverse Fourier_transformation formula. We first prove that
the formula is true for test functions, there are densely many of them. We then
extend the inverse map to the whole space using the fact that linear map is
continuous; thus, uniformly continuous.
***** Generalization to topological vector spaces[edit] *****
In the special case of two topological_vector_spaces     V   {\displaystyle V}
[V] and     W   {\displaystyle W}  [W], the notion of uniform continuity of a
map     f : V &#x2192; W   {\displaystyle f:V\to W}  [f:V\to W] becomes: for
any neighborhood     B   {\displaystyle B}  [B] of zero in     W
{\displaystyle W}  [W], there exists a neighborhood     A   {\displaystyle A}
[A] of zero in     V   {\displaystyle V}  [V] such that      v  1   &#x2212;  v
2   &#x2208; A   {\displaystyle v_{1}-v_{2}\in A}  [v_{1}-v_{2}\in A] implies
f (  v  1   ) &#x2212; f (  v  2   ) &#x2208; B .   {\displaystyle f(v_{1})-f
(v_{2})\in B.}  [f(v_{1})-f(v_{2})\in B.]
For linear_transformations     f : V &#x2192; W   {\displaystyle f:V\to W}  [f:
V\to W], uniform continuity is equivalent to continuity. This fact is
frequently used implicitly in functional_analysis to extend a linear map off a
dense subspace of a Banach_space.
***** Generalization to uniform spaces[edit] *****
Just as the most natural and general setting for continuity is topological
spaces, the most natural and general setting for the study of uniform
continuity are the uniform_spaces. A function f : X â Y between uniform
spaces is called uniformly continuous if for every entourage V in Y there
exists an entourage U in X such that for every (x1, x2) in U we have (f(x1), f
(x2)) in V.
In this setting, it is also true that uniformly continuous maps transform
Cauchy sequences into Cauchy sequences.
Each compact Hausdorff space possesses exactly one uniform structure compatible
with the topology. A consequence is a generalisation of the Heine-Cantor
theorem: each continuous function from a compact Hausdorff space to a uniform
space is uniformly continuous.
***** References[edit] *****
   1. ^ Rusnock_&_Kerr-Lawson_2005.
***** Further reading[edit] *****
    * Bourbaki,_Nicolas. General Topology: Chapters 1â4 [Topologie
      GÃ©nÃ©rale]. ISBN 0-387-19374-X.
 Chapter II is a comprehensive reference of uniform spaces.
DieudonnÃ©,_Jean (1960). Foundations of Modern Analysis. Academic Press.
Fitzpatrick, Patrick (2006). Advanced Calculus. Brooks/Cole. ISBN 0-534-92612-
6.
Kelley, John L. (1955). General topology. Graduate Texts in Mathematics.
Springer-Verlag. ISBN 0-387-90125-6.
Kudryavtsev, L.D. (2001) [1994], "Uniform_continuity", in Hazewinkel,_Michiel
(ed.), Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Rudin,_Walter (1976). Principles of Mathematical Analysis. New York: McGraw-
Hill. ISBN 978-0-07-054235-8.
Rusnock, P.; Kerr-Lawson, A. (2005), "Bolzano and uniform continuity", Historia
Mathematica, 32 (3): 303â311, doi:10.1016/j.hm.2004.11.003

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Uniform_continuity&oldid=907054527"
Categories:
    * Continuous_mappings
    * Calculus
    * Mathematical_analysis
    * General_topology
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Hrvatski
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 20 July 2019, at 04:41 (UTC).
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
