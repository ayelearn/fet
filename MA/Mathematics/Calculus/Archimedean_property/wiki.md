The following text has been accessed from https://en.wikipedia.org/wiki/Archimedean_property at Fri Aug 9 02:36:07 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Archimedean property ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about abstract algebra. For the physical law, see Archimedes'
principle.
Illustration of the Archimedean property.
In abstract_algebra and analysis, the Archimedean property, named after the
ancient Greek mathematician Archimedes of Syracuse, is a property held by some
algebraic_structures, such as ordered or normed groups, and fields. Roughly
speaking, it is the property of having no infinitely large or infinitely small
elements. It was Otto_Stolz who gave the axiom of Archimedes its name because
it appears as Axiom V of Archimedesâ On_the_Sphere_and_Cylinder.[1]
The notion arose from the theory of magnitudes of Ancient Greece; it still
plays an important role in modern mathematics such as David_Hilbert's axioms
for_geometry, and the theories of ordered_groups, ordered_fields, and local
fields.
An algebraic structure in which any two non-zero elements are comparable, in
the sense that neither of them is infinitesimal with respect to the other, is
said to be Archimedean. A structure which has a pair of non-zero elements, one
of which is infinitesimal with respect to the other, is said to be non-
Archimedean. For example, a linearly_ordered_group that is Archimedean is an
Archimedean_group.
This can be made precise in various contexts with slightly different
formulations. For example, in the context of ordered_fields, one has the axiom
of Archimedes which formulates this property, where the field of real_numbers
is Archimedean, but that of rational_functions in real coefficients is not.
⁰
***** Contents *****
    * 1_History_and_origin_of_the_name_of_the_Archimedean_property
    * 2_Definition_for_linearly_ordered_groups
          o 2.1_Ordered_fields
    * 3_Definition_for_normed_fields
    * 4_Examples_and_non-examples
          o 4.1_Archimedean_property_of_the_real_numbers
          o 4.2_Non-Archimedean_ordered_field
          o 4.3_Non-Archimedean_valued_fields
          o 4.4_Equivalent_definitions_of_Archimedean_ordered_field
    * 5_Notes
    * 6_References
    * 7_See_also
***** History and origin of the name of the Archimedean property[edit] *****
The concept was named by Otto_Stolz (in the 1880s) after the ancient_Greek
geometer and physicist Archimedes of Syracuse.
The Archimedean property appears in Book V of Euclid's_Elements as Definition
4:
     Magnitudes are said to have a ratio to one another which can, when
     multiplied, exceed one another.
Because Archimedes credited it to Eudoxus_of_Cnidus it is also known as the
"Theorem of Eudoxus" or the Eudoxus axiom.[2]
Archimedes_used_infinitesimals in heuristic arguments, although he denied that
those were finished mathematical_proofs.
***** Definition for linearly ordered groups[edit] *****
Let x and y be positive elements of a linearly_ordered_group G. Then x is
infinitesimal with respect to y (or equivalently, y is infinite with respect to
x) if, for every natural_number n, the multiple nx is less than y, that is, the
following inequality holds:
                         x + &#x22EF; + x  &#x23DF;    n  &#xA0;terms    < y .
                  {\displaystyle \underbrace {x+\cdots +x} _{n{\text
                  { terms}}}<y.\,}  [ \underbrace{x+\cdots+x}_{n\text{ terms}}
                  < y. \, ]
The group G is Archimedean if there is no pair x,y such that x is infinitesimal
with respect to y.
Additionally, if K is an algebraic_structure with a unit (1) â for example, a
ring â a similar definition applies to K. If x is infinitesimal with respect
to 1, then x is an infinitesimal element. Likewise, if y is infinite with
respect to 1, then y is an infinite element. The algebraic structure K is
Archimedean if it has no infinite elements and no infinitesimal elements.
**** Ordered fields[edit] ****
An ordered_field has some additional properties.
    * One may assume that the rational numbers are contained in the field.
    * If x is infinitesimal, then 1/x is infinite, and vice versa. Therefore,
      to verify that a field is Archimedean it is enough to check only that
      there are no infinitesimal elements, or to check that there are no
      infinite elements.
    * If x is infinitesimal and r is a rational number, then râx is also
      infinitesimal. As a result, given a general element c, the three numbers
      c/2, c, and 2c are either all infinitesimal or all non-infinitesimal.
In this setting, an ordered field K is Archimedean precisely when the following
statement, called the axiom of Archimedes, holds:
      Let x be any element of K. Then there exists a natural number n such that
      n > x.
Alternatively one can use the following characterization:
      âÎµ > 0 â K: ân â N:1/n < Îµ.
***** Definition for normed fields[edit] *****
The qualifier "Archimedean" is also formulated in the theory of rank_one_valued
fields and normed spaces over rank one valued fields as follows. Let F be a
field endowed with an absolute value function, i.e., a function which
associates the real number 0 with the field element 0 and associates a positive
real number      |  x  |    {\displaystyle |x|}  [|x|] with each non-zero     x
&#x2208; F   {\displaystyle x\in F}  [ x\in F] and satisfies      |  x y  |  =
|  x  |   |  y  |    {\displaystyle |xy|=|x||y|}  [|xy|=|x| |y|] and      |  x
+ y  |  &#x2264;  |  x  |  +  |  y  |    {\displaystyle |x+y|\leq |x|+|y|}
[|x+y| \le |x|+|y|]. Then, F is said to be Archimedean if for any non-zero
x &#x2208; F   {\displaystyle x\in F}  [ x\in F] there exists a natural_number
n such that
                      |      x + &#x22EF; + x  &#x23DF;    n  &#xA0;terms     |
                  > 1.    {\displaystyle |\underbrace {x+\cdots +x} _{n{\text
                  { terms}}}|>1.\,}  [|\underbrace{x+\cdots+x}_{n\text
                  { terms}}| > 1. \, ]
Similarly, a normed space is Archimedean if a sum of     n   {\displaystyle n}
[n] terms, each equal to a non-zero vector     x   {\displaystyle x}  [x], has
norm greater than one for sufficiently large     n   {\displaystyle n}  [n]. A
field with an absolute value or a normed space is either Archimedean or
satisfies the stronger condition, referred to as the ultrametric triangle
inequality,
                      |  x + y  |  &#x2264; max (  |  x  |  ,  |  y  |  )
                  {\displaystyle |x+y|\leq \max(|x|,|y|)}  [|x+y| \le \max
                  (|x|,|y|)],
respectively. A field or normed space satisfying the ultrametric triangle
inequality is called non-Archimedean.
The concept of a non-Archimedean normed linear space was introduced by A. F.
Monna.[3]
***** Examples and non-examples[edit] *****
**** Archimedean property of the real numbers[edit] ****
The field of the rational numbers can be assigned one of a number of absolute
value functions, including the trivial function      |  x  |  = 1 ,
{\displaystyle |x|=1,}  [|x|=1,] when     x &#x2260; 0   {\displaystyle x\neq
0}  [ x \neq 0], the more usual      |  x  |  =    x  2       {\displaystyle
|x|={\sqrt {x^{2}}}}  [|x| = \sqrt{x^2}], and the p-adic absolute value
functions. By Ostrowski's_theorem, every non-trivial absolute value on the
rational numbers is equivalent to either the usual absolute value or some p-
adic absolute value. The rational field is not complete with respect to non-
trivial absolute values; with respect to the trivial absolute value, the
rational field is a discrete topological space, so complete. The completion
with respect to the usual absolute value (from the order) is the field of real
numbers. By this construction the field of real numbers is Archimedean both as
an ordered field and as a normed field.[4] On the other hand, the completions
with respect to the other non-trivial absolute values give the fields of p-adic
numbers, where p is a prime integer number (see below); since the p-adic
absolute values satisfy the ultrametric property, then the p-adic number fields
are non-Archimedean as normed fields (they cannot be made into ordered fields).
In the axiomatic_theory_of_real_numbers, the non-existence of nonzero
infinitesimal real numbers is implied by the least_upper_bound_property as
follows. Denote by Z the set consisting of all positive infinitesimals. This
set is bounded above by 1. Now assume_for_a_contradiction that Z is nonempty.
Then it has a least_upper_bound c, which is also positive, so c/2 < c < 2c.
Since c is an upper_bound of Z and 2c is strictly larger than c, 2c is not a
positive infinitesimal. That is, there is some natural number n for which 1/n <
2c. On the other hand, c/2 is a positive infinitesimal, since by the definition
of least upper bound there must be an infinitesimal x between c/2 and c, and if
1/k < c/2 <= x then x is not infinitesimal. But 1/(4n) < c/2, so c/2 is not
infinitesimal, and this is a contradiction. This means that Z is empty after
all: there are no positive, infinitesimal real numbers.
The Archimedean property of real numbers holds also in constructive_analysis,
even though the least upper bound property may fail in that context.
**** Non-Archimedean ordered field[edit] ****
Main article: Non-Archimedean_ordered_field
For an example of an ordered_field that is not Archimedean, take the field of
rational_functions with real coefficients. (A rational function is any function
that can be expressed as one polynomial divided by another polynomial; we will
assume in what follows that this has been done in such a way that the leading
coefficient of the denominator is positive.) To make this an ordered field, one
must assign an ordering compatible with the addition and multiplication
operations. Now f > g if and only if f â g > 0, so we only have to say which
rational functions are considered positive. Call the function positive if the
leading coefficient of the numerator is positive. (One must check that this
ordering is well defined and compatible with addition and multiplication.) By
this definition, the rational function 1/x is positive but less than the
rational function 1. In fact, if n is any natural number, then n(1/x) = n/x is
positive but still less than 1, no matter how big n is. Therefore, 1/x is an
infinitesimal in this field.
This example generalizes to other coefficients. Taking rational functions with
rational instead of real coefficients produces a countable non-Archimedean
ordered field. Taking the coefficients to be the rational functions in a
different variable, say y, produces an example with a different order_type.
**** Non-Archimedean valued fields[edit] ****
The field of the rational numbers endowed with the p-adic metric and the p-adic
number fields which are the completions, do not have the Archimedean property
as fields with absolute values. All Archimedean valued fields are isometrically
isomorphic to a subfield of the complex numbers with a power of the usual
absolute value.[5]
**** Equivalent definitions of Archimedean ordered field[edit] ****
Every linearly ordered field K contains (an isomorphic copy of) the rationals
as an ordered subfield, namely the subfield generated by the multiplicative
unit 1 of K, which in turn contains the integers as an ordered subgroup, which
contains the natural numbers as an ordered monoid. The embedding of the
rationals then gives a way of speaking about the rationals, integers, and
natural numbers in K. The following are equivalent characterizations of
Archimedean fields in terms of these substructures.[6]
1. The natural numbers are cofinal in K. That is, every element of K is less
than some natural number. (This is not the case when there exist infinite
elements.) Thus an Archimedean field is one whose natural numbers grow without
bound.
2. Zero is the infimum in K of the set {1/2,â1/3,â1/4,â...â}. (If K
contained a positive infinitesimal it would be a lower bound for the set whence
zero would not be the greatest lower bound.)
3. The set of elements of K between the positive and negative rationals is non-
open. This is because the set consists of all the infinitesimals, which is just
the set {0} when there are no nonzero infinitesimals, and otherwise is open,
there being neither a least nor greatest nonzero infinitesimal. Observe that in
both cases, the set of infinitesimals is closed. In the latter case, (i) every
infinitesimal is less than every positive rational, (ii) there is neither a
greatest infinitesimal nor a least positive rational, and (iii) there is
nothing else in between. Consequently, any non-Archimedean ordered field is
both incomplete and disconnected.
4. For any x in K the set of integers greater than x has a least element. (If x
were a negative infinite quantity every integer would be greater than it.)
5. Every nonempty open interval of K contains a rational. (If x is a positive
infinitesimal, the open interval (x,â2x) contains infinitely many
infinitesimals but not a single rational.)
6. The rationals are dense in K with respect to both sup and inf. (That is,
every element of K is the sup of some set of rationals, and the inf of some
other set of rationals.) Thus an Archimedean field is any dense ordered
extension of the rationals, in the sense of any ordered field that densely
embeds its rational elements.
***** Notes[edit] *****
   1. ^ G. Fisher (1994) in P. Ehrlich(ed.), Real Numbers, Generalizations of
      the Reals, and Theories of continua, 107-145, Kluwer Academic
   2. ^Knopp,_Konrad (1951). Theory and Application of Infinite Series (English
      2nd ed.). London and Glasgow: Blackie & Son, Ltd. p. 7. ISBN 0-486-66165-
      2.
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
   4. ^ Monna, A. F., Over een lineare P-adisches ruimte, Indag. Math., 46
      (1943), 74â84.
   5. ^ Neal_Koblitz, "p-adic Numbers, p-adic Analysis, and Zeta-Functions",
      Springer-Verlag,1977.
   6. ^ Shell, Niel, Topological Fields and Near Valuations, Dekker, New York,
      1990.
   7. ISBN 0-8247-8412-X
   8. ^ Schechter_1997, Â§10.3
***** References[edit] *****
    * Schechter,_Eric (1997). Handbook_of_Analysis_and_its_Foundations.
      Academic Press. ISBN 0-12-622760-8.
***** See also[edit] *****
    * 0.999...#Infinitesimals

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Archimedean_property&oldid=904183754"
Categories:
    * Field_theory
    * Ordered_groups
    * Real_algebraic_geometry
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
    * Alemannisch
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * Nederlands
    * æ¥æ¬èª
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * SlovenÅ¡Äina
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 30 June 2019, at 14:35 (UTC).
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
