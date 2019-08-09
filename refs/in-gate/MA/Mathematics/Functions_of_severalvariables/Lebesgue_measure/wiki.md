The following text has been accessed from https://en.wikipedia.org/wiki/Lebesgue_measure at Fri Aug 9 02:34:05 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Lebesgue measure ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In measure_theory, the Lebesgue measure, named after French mathematician Henri
Lebesgue, is the standard way of assigning a measure to subsets of n-
dimensional Euclidean_space. For n = 1, 2, or 3, it coincides with the standard
measure of length, area, or volume. In general, it is also called n-dimensional
volume, n-volume, or simply volume.[1] It is used throughout real_analysis, in
particular to define Lebesgue_integration. Sets that can be assigned a Lebesgue
measure are called Lebesgue-measurable; the measure of the Lebesgue-measurable
set A is here denoted by Î»(A).
Henri Lebesgue described this measure in the year 1901, followed the next year
by his description of the Lebesgue_integral. Both were published as part of his
dissertation in 1902.[2]
The Lebesgue measure is often denoted by dx, but this should not be confused
with the distinct notion of a volume_form.
⁰
***** Contents *****
    * 1_Definition
          o 1.1_Intuition
    * 2_Examples
    * 3_Properties
    * 4_Null_sets
    * 5_Construction_of_the_Lebesgue_measure
    * 6_Relation_to_other_measures
    * 7_See_also
    * 8_References
***** Definition[edit] *****
Given a subset     E &#x2286;  R    {\displaystyle E\subseteq \mathbb {R} }
[E\subseteq {\mathbb  {R}}], with the length of interval     I = [ a , b ]
&#xA0;(or&#xA0;  I = ( a , b ) )   {\displaystyle I=[a,b]{\text{ (or }}I=
(a,b))}  [{\displaystyle I=[a,b]{\text{ (or }}I=(a,b))}] given by     &#x2113;
( I ) = b &#x2212; a   {\displaystyle \ell (I)=b-a}  [{\displaystyle \ell
(I)=b-a}], the Lebesgue outer_measure [3]      &#x03BB;  &#x2217;   ( E )
{\displaystyle \lambda ^{*}(E)}  [\lambda^*(E)] is defined as
          &#x03BB;  &#x2217;   ( E ) = inf &#x2061;  {   &#x2211;  k = 1
      &#x221E;   &#x2113; (  I  k   ) :  (  I  k    )  k &#x2208;  N
      &#xA0;is a sequence of intervals with open boundaries with&#xA0;  E
      &#x2286;  &#x22C3;  k = 1   &#x221E;    I  k    }    {\displaystyle
      \lambda ^{*}(E)=\operatorname {inf} \left\{\sum _{k=1}^{\infty }\ell (I_
      {k}):{(I_{k})_{k\in \mathbb {N} }}{\text{ is a sequence of intervals with
      open boundaries with }}E\subseteq \bigcup _{k=1}^{\infty }I_{k}\right\}}
      [{\displaystyle \lambda ^{*}(E)=\operatorname {inf} \left\{\sum _{k=1}^
      {\infty }\ell (I_{k}):{(I_{k})_{k\in \mathbb {N} }}{\text{ is a sequence
      of intervals with open boundaries with }}E\subseteq \bigcup _{k=1}^
      {\infty }I_{k}\right\}}].
The Lebesgue measure is defined on the Lebesgue Ï-algebra, which is the
collection of all sets     E   {\displaystyle E}  [E] which satisfy the
"CarathÃ©odory criterion" which requires that for every     A &#x2286;  R
{\displaystyle A\subseteq \mathbb {R} }  [{\displaystyle A\subseteq \mathbb {R}
}],
          &#x03BB;  &#x2217;   ( A ) =  &#x03BB;  &#x2217;   ( A &#x2229; E ) +
      &#x03BB;  &#x2217;   ( A &#x2229;  E  c   )   {\displaystyle \lambda ^{*}
      (A)=\lambda ^{*}(A\cap E)+\lambda ^{*}(A\cap E^{c})}  [\lambda^*(A) =
      \lambda^*(A \cap E) + \lambda^*(A \cap E^c) ]
For any set in the Lebesgue Ï-algebra, its Lebesgue measure is given by its
Lebesgue outer measure     &#x03BB; ( E ) =  &#x03BB;  &#x2217;   ( E )
{\displaystyle \lambda (E)=\lambda ^{*}(E)}  [\lambda(E)=\lambda^*(E)].
Sets that are not included in the Lebesgue Ï-algebra are not Lebesgue-
measurable. Such sets do exist, i.e., the Lebesgue Ï-algebra is strictly
contained in the power_set of      R    {\displaystyle \mathbb {R} }  [
{\displaystyle \mathbb {R} }].
**** Intuition[edit] ****
The first part of the definition states that the subset     E   {\displaystyle
E}  [E] of the real numbers is reduced to its outer measure by coverage by sets
of open intervals. Each of these sets of intervals     I   {\displaystyle I}
[I] covers     E   {\displaystyle E}  [E] in the sense that when the intervals
are combined together by union, they contain     E   {\displaystyle E}  [E].
The total length of any covering interval set can easily overestimate the
measure of     E   {\displaystyle E}  [E], because     E   {\displaystyle E}
[E] is a subset of the union of the intervals, and so the intervals may include
points which are not in     E   {\displaystyle E}  [E]. The Lebesgue outer
measure emerges as the greatest_lower_bound_(infimum) of the lengths from among
all possible such sets. Intuitively, it is the total length of those interval
sets which fit     E   {\displaystyle E}  [E] most tightly and do not overlap.
That characterizes the Lebesgue outer measure. Whether this outer measure
translates to the Lebesgue measure proper depends on an additional condition.
This condition is tested by taking subsets     A   {\displaystyle A}  [A] of
the real numbers using     E   {\displaystyle E}  [E] as an instrument to split
A   {\displaystyle A}  [A] into two partitions: the part of     A
{\displaystyle A}  [A] which intersects with     E   {\displaystyle E}  [E] and
the remaining part of     A   {\displaystyle A}  [A] which is not in     E
{\displaystyle E}  [E]: the set difference of     A   {\displaystyle A}  [A]
and     E   {\displaystyle E}  [E]. These partitions of     A   {\displaystyle
A}  [A] are subject to the outer measure. If for all possible such subsets
A   {\displaystyle A}  [A] of the real numbers, the partitions of     A
{\displaystyle A}  [A] cut apart by     E   {\displaystyle E}  [E] have outer
measures whose sum is the outer measure of     A   {\displaystyle A}  [A], then
the outer Lebesgue measure of     E   {\displaystyle E}  [E] gives its Lebesgue
measure. Intuitively, this condition means that the set     E   {\displaystyle
E}  [E] must not have some curious properties which causes a discrepancy in the
measure of another set when     E   {\displaystyle E}  [E] is used as a "mask"
to "clip" that set, hinting at the existence of sets for which the Lebesgue
outer measure does not give the Lebesgue measure. (Such sets are, in fact, not
Lebesgue-measurable.)
***** Examples[edit] *****
    * Any open or closed interval [a, b] of real_numbers is Lebesgue-
      measurable, and its Lebesgue measure is the length b − a. The open
      interval (a, b) has the same measure, since the difference between the
      two sets consists only of the end points a and b and has measure_zero.
    * Any Cartesian_product of intervals [a, b] and [c, d] is Lebesgue-
      measurable, and its Lebesgue measure is (b − a)(d − c), the area of the
      corresponding rectangle.
    * Moreover, every Borel_set is Lebesgue-measurable. However, there are
      Lebesgue-measurable sets which are not Borel sets.[4][5]
    * Any countable set of real numbers has Lebesgue measure 0.
    * In particular, the Lebesgue measure of the set of rational_numbers is 0,
      although the set is dense in R.
    * The Cantor_set is an example of an uncountable_set that has Lebesgue
      measure zero.
    * If the axiom_of_determinacy holds then all sets of reals are Lebesgue-
      measurable. Determinacy is however not compatible with the axiom_of
      choice.
    * Vitali_sets are examples of sets that are not_measurable with respect to
      the Lebesgue measure. Their existence relies on the axiom_of_choice.
    * Osgood_curves are simple plane curves with positive Lebesgue measure[6]
      (it can be obtained by small variation of the Peano_curve construction).
      The dragon_curve is another unusual example.
    * Any line in       R   n     {\displaystyle \mathbb {R} ^{n}}  [\mathbb
      {R} ^{n}], for     n &#x2265; 2   {\displaystyle n\geq 2}  [n\geq 2], has
      a zero Lebesgue measure. In general, every proper hyperplane has a zero
      Lebesgue measure in its ambient_space.
***** Properties[edit] *****
Translation invariance: The Lebesgue measure of     A   {\displaystyle A}  [A]
and     A + t   {\displaystyle A+t}  [A+t] are the same.
The Lebesgue measure on Rn has the following properties:
   1. If A is a cartesian_product of intervals I1 × I2 × ... × In, then A is
      Lebesgue-measurable and     &#x03BB; ( A ) =  |   I  1    |  &#x22C5;  |
      I  2    |  &#x22EF;  |   I  n    |  .   {\displaystyle \lambda (A)=|I_
      {1}|\cdot |I_{2}|\cdots |I_{n}|.}  [\lambda (A)=|I_1|\cdot |I_2|\cdots
      |I_n|.] Here, |I| denotes the length of the interval I.
   2. If A is a disjoint_union of countably_many disjoint Lebesgue-measurable
      sets, then A is itself Lebesgue-measurable and Î»(A) is equal to the sum
      (or infinite_series) of the measures of the involved measurable sets.
   3. If A is Lebesgue-measurable, then so is its complement.
   4. Î»(A) â¥ 0 for every Lebesgue-measurable set A.
   5. If A and B are Lebesgue-measurable and A is a subset of B, then Î»(A) â¤
      Î»(B). (A consequence of 2, 3 and 4.)
   6. Countable unions and intersections of Lebesgue-measurable sets are
      Lebesgue-measurable. (Not a consequence of 2 and 3, because a family of
      sets that is closed under complements and disjoint countable unions need
      not be closed under countable unions:     { &#x2205; , { 1 , 2 , 3 , 4 }
      , { 1 , 2 } , { 3 , 4 } , { 1 , 3 } , { 2 , 4 } }   {\displaystyle \
      {\emptyset ,\{1,2,3,4\},\{1,2\},\{3,4\},\{1,3\},\{2,4\}\}}  [\{\emptyset,
      \{1,2,3,4\}, \{1,2\}, \{3,4\}, \{1,3\}, \{2,4\}\}].)
   7. If A is an open or closed subset of Rn (or even Borel_set, see metric
      space), then A is Lebesgue-measurable.
   8. If A is a Lebesgue-measurable set, then it is "approximately open" and
      "approximately closed" in the sense of Lebesgue measure (see the
      regularity_theorem_for_Lebesgue_measure).
   9. A Lebesgue-measurable set can be "squeezed" between a containing open set
      and a contained closed set. This property has been used as an alternative
      definition of Lebesgue measurability. More precisely,     E &#x2282;  R
      {\displaystyle E\subset \mathbb {R} }  [{\displaystyle E\subset \mathbb
      {R} }] is Lebesgue-measurable if and only if for every     &#x03B5; > 0
      {\displaystyle \varepsilon >0}  [\varepsilon >0] there exist an open set
      G   {\displaystyle G}  [G] and a closed set     F   {\displaystyle F}
      [F] such that     F &#x2282; E &#x2282; G   {\displaystyle F\subset
      E\subset G}  [{\displaystyle F\subset E\subset G}] and     &#x03BB; ( G
      &#x2216; F ) < &#x03B5;   {\displaystyle \lambda (G\setminus
      F)<\varepsilon }  [{\displaystyle \lambda (G\setminus F)<\varepsilon }].
      [7]
  10. A Lebesgue-measurable set can be "squeezed" between a containing GÎ´set
      and a contained FÏ. I.e, if A is Lebesgue-measurable then there exist a
      GÎ´set G and an FÏ F such that G â A â F and Î»(G \ A) = Î»
      (A \ F) = 0.
  11. Lebesgue measure is both locally_finite and inner_regular, and so it is a
      Radon_measure.
  12. Lebesgue measure is strictly_positive on non-empty open sets, and so its
      support is the whole of Rn.
  13. If A is a Lebesgue-measurable set with Î»(A) = 0 (a null_set), then every
      subset ofAis also a null set. A_fortiori, every subset ofAis measurable.
  14. If A is Lebesgue-measurable and x is an element of Rn, then the
      translation ofAby x, defined by A + x = {a + x : a â A}, is also
      Lebesgue-measurable and has the same measure as A.
  15. If A is Lebesgue-measurable and     &#x03B4; > 0   {\displaystyle \delta
      >0}  [\delta >0], then the dilation of     A   {\displaystyle A}  [A] by
      &#x03B4;   {\displaystyle \delta }  [\delta ] defined by     &#x03B4; A =
      { &#x03B4; x : x &#x2208; A }   {\displaystyle \delta A=\{\delta x:x\in
      A\}}  [\delta A=\{\delta x:x\in A\}] is also Lebesgue-measurable and has
      measure      &#x03B4;  n   &#x03BB;  ( A ) .   {\displaystyle \delta ^
      {n}\lambda \,(A).}  [\delta^{n}\lambda\,(A).]
  16. More generally, if T is a linear_transformation and A is a measurable
      subset of Rn, then T(A) is also Lebesgue-measurable and has the measure
      |  det ( T )  |  &#x03BB; ( A )   {\displaystyle \left|\det
      (T)\right|\lambda (A)}  [{\displaystyle \left|\det(T)\right|\lambda
      (A)}].
All the above may be succinctly summarized as follows:
      The Lebesgue-measurable sets form a Ï-algebra containing all products of
      intervals, and λ is the unique complete translation-invariant measure on
      that σ-algebra with     &#x03BB; ( [ 0 , 1 ] &#x00D7; [ 0 , 1 ] &#x00D7;
      &#x22EF; &#x00D7; [ 0 , 1 ] ) = 1.   {\displaystyle \lambda ([0,1]\times
      [0,1]\times \cdots \times [0,1])=1.}  [\lambda([0,1]\times [0, 1]\times
      \cdots \times [0, 1])=1.]
The Lebesgue measure also has the property of being Ï-finite.
***** Null sets[edit] *****
Main article: Null_set
A subset of Rn is a null set if, for every Îµ > 0, it can be covered with
countably many products of n intervals whose total volume is at most Îµ. All
countable sets are null sets.
If a subset of Rn has Hausdorff_dimension less than n then it is a null set
with respect to n-dimensional Lebesgue measure. Here Hausdorff dimension is
relative to the Euclidean_metric on Rn (or any metric Lipschitz equivalent to
it). On the other hand, a set may have topological_dimension less than n and
have positive n-dimensional Lebesgue measure. An example of this is the
SmithâVolterraâCantor_set which has topological dimension 0 yet has
positive 1-dimensional Lebesgue measure.
In order to show that a given set A is Lebesgue-measurable, one usually tries
to find a "nicer" set B which differs from A only by a null set (in the sense
that the symmetric_difference (A − B)     &#x222A;   {\displaystyle \cup }
[\cup ](B − A) is a null set) and then show that B can be generated using
countable unions and intersections from open or closed sets.
***** Construction of the Lebesgue measure[edit] *****
The modern construction of the Lebesgue measure is an application of
CarathÃ©odory's_extension_theorem. It proceeds as follows.
Fix n ∈ N. A box in Rn is a set of the form
         B =  &#x220F;  i = 1   n   [  a  i   ,  b  i   ]  ,   {\displaystyle
      B=\prod _{i=1}^{n}[a_{i},b_{i}]\,,}  [B=\prod_{i=1}^n [a_i,b_i] \, ,]
where bi ≥ ai, and the product symbol here represents a Cartesian product. The
volume of this box is defined to be
         vol &#x2061; ( B ) =  &#x220F;  i = 1   n   (  b  i   &#x2212;  a  i
      )  .   {\displaystyle \operatorname {vol} (B)=\prod _{i=1}^{n}(b_{i}-a_
      {i})\,.}  [\operatorname{vol}(B)=\prod_{i=1}^n (b_i-a_i) \, .]
For any subset A of Rn, we can define its outer_measure Î»*(A) by:
          &#x03BB;  &#x2217;   ( A ) = inf  {   &#x2211;  B &#x2208;   C
      vol &#x2061; ( B ) :   C    &#xA0;is a countable collection of boxes
      whose union covers&#xA0;  A  }  .   {\displaystyle \lambda ^{*}(A)=\inf
      \left\{\sum _{B\in {\mathcal {C}}}\operatorname {vol} (B):{\mathcal {C}}
      {\text{ is a countable collection of boxes whose union covers
      }}A\right\}.}  [{\displaystyle \lambda ^{*}(A)=\inf \left\{\sum _{B\in
      {\mathcal {C}}}\operatorname {vol} (B):{\mathcal {C}}{\text{ is a
      countable collection of boxes whose union covers }}A\right\}.}]
We then define the set A to be Lebesgue-measurable if for every subset S of Rn,
          &#x03BB;  &#x2217;   ( S ) =  &#x03BB;  &#x2217;   ( S &#x2229; A ) +
      &#x03BB;  &#x2217;   ( S &#x2216; A )  .   {\displaystyle \lambda ^{*}
      (S)=\lambda ^{*}(S\cap A)+\lambda ^{*}(S\setminus A)\,.}  [\lambda^*(S) =
      \lambda^*(S \cap A) + \lambda^*(S \setminus A) \, .]
These Lebesgue-measurable sets form a Ï-algebra, and the Lebesgue measure is
defined by Î»(A) = Î»*(A) for any Lebesgue-measurable set A.
The existence of sets that are not Lebesgue-measurable is a consequence of a
certain set-theoretical axiom, the axiom_of_choice, which is independent from
many of the conventional systems of axioms for set_theory. The Vitali_theorem,
which follows from the axiom, states that there exist subsets of R that are not
Lebesgue-measurable. Assuming the axiom of choice, non-measurable_sets with
many surprising properties have been demonstrated, such as those of the
BanachâTarski_paradox.
In 1970, Robert_M._Solovay showed that the existence of sets that are not
Lebesgue-measurable is not provable within the framework of ZermeloâFraenkel
set_theory in the absence of the axiom of choice (see Solovay's_model).[8]
***** Relation to other measures[edit] *****
The Borel_measure agrees with the Lebesgue measure on those sets for which it
is defined; however, there are many more Lebesgue-measurable sets than there
are Borel measurable sets. The Borel measure is translation-invariant, but not
complete.
The Haar_measure can be defined on any locally_compact group and is a
generalization of the Lebesgue measure (Rn with addition is a locally compact
group).
The Hausdorff_measure is a generalization of the Lebesgue measure that is
useful for measuring the subsets of Rn of lower dimensions than n, like
submanifolds, for example, surfaces or curves in R3 and fractal sets. The
Hausdorff measure is not to be confused with the notion of Hausdorff_dimension.
It can be shown that there_is_no_infinite-dimensional_analogue_of_Lebesgue
measure.
***** See also[edit] *****
    * Lebesgue's_density_theorem
    * Lebesgue_measure_of_the_set_of_Liouville_numbers
***** References[edit] *****
   1. ^ The term volume is also used, more strictly, as a synonym of 3-
      dimensional volume
   2. ^Henri Lebesgue (1902). "IntÃ©grale, longueur, aire". UniversitÃ© de
      Paris.
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
   4. ^Royden,_H._L. (1988). Real Analysis (3rd ed.). New York: Macmillan.
      p. 56. ISBN 0-02-404151-3.
   5. ^Asaf Karagila. "What_sets_are_Lebesgue-measurable?". math stack
      exchange. Retrieved 26 September 2015.
   6. ^Asaf Karagila. "Is_there_a_sigma-algebra_on_R_strictly_between_the_Borel
      and_Lebesgue_algebras?". math stack exchange. Retrieved 26 September
      2015.
   7. ^Osgood,_William_F. (January 1903). "A Jordan Curve of Positive Area".
      Transactions of the American Mathematical Society. American Mathematical
      Society. 4 (1): 107â112. doi:10.2307/1986455. ISSN 0002-9947.
      JSTOR 1986455.
   8. ^Carothers, N. L. (2000). Real Analysis. Cambridge: Cambridge University
      Press. p. 293. ISBN 9780521497565.
   9. ^Solovay, Robert M. (1970). "A model of set-theory in which every set of
      reals is Lebesgue-measurable". Annals_of_Mathematics. Second Series. 92
      (1): 1â56. doi:10.2307/1970696. JSTOR 1970696.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Lebesgue_measure&oldid=909968863"
Categories:
    * Measures_(measure_theory)
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
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 8 August 2019, at 20:17 (UTC).
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
