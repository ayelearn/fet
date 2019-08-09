The following text has been accessed from https://en.wikipedia.org/wiki/Probability_axioms at Fri Aug 9 00:02:50 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Probability axioms ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Part of a series on statistics
Probability_theory
[Nuvola_apps_atlantik.png]
    * Probability axioms
    * Probability_space
    * Sample_space
    * Elementary_event
    * Event
    * Random_variable
    * Probability_measure
    * Complementary_event
    * Joint_probability
    * Marginal_probability
    * Conditional_probability
    * Independence
    * Conditional_independence
    * Law_of_total_probability
    * Law_of_large_numbers
    * Bayes'_theorem
    * Boole's_inequality
    * Venn_diagram
    * Tree_diagram
    * v
    * t
    * e
The Kolmogorov axioms are a fundamental part of Andrey_Kolmogorov's probability
theory. In it, the probability P of some event E, denoted     P ( E )
{\displaystyle P(E)}  [P(E)], is usually defined as to satisfy these axioms.
The axioms are described below.
These assumptions can be summarised as follows: Let (Î©, F, P) be a measure
space with P(Î©) = 1. Then (Î©, F, P) is a probability_space, with sample space
Î©, event space F and probability measure P.
An alternative approach to formalising probability, favoured by some Bayesians,
is given by Cox's_theorem.
⁰
***** Contents *****
    * 1_Axioms
          o 1.1_First_axiom
          o 1.2_Second_axiom
          o 1.3_Third_axiom
    * 2_Consequences
          o 2.1_The_probability_of_the_empty_set
          o 2.2_Monotonicity
          o 2.3_The_numeric_bound
    * 3_Proofs
    * 4_Further_consequences
    * 5_Simple_example:_coin_toss
    * 6_See_also
    * 7_Further_reading
    * 8_External_links
***** Axioms[edit] *****
**** First axiom[edit] ****
The probability of an event is a non-negative real number:
         P ( E ) &#x2208;  R  , P ( E ) &#x2265; 0  &#x2200; E &#x2208; F
      {\displaystyle P(E)\in \mathbb {R} ,P(E)\geq 0\qquad \forall E\in F}  [
      {\displaystyle P(E)\in \mathbb {R} ,P(E)\geq 0\qquad \forall E\in F}]
where     F   {\displaystyle F}  [F] is the event space. It follows that     P
( E )   {\displaystyle P(E)}  [P(E)] is always finite, in contrast with more
general measure_theory. Theories which assign negative_probability relax the
first axiom.
**** Second axiom[edit] ****
See also: Unitarity_(physics)
This is the assumption of unit_measure: that the probability that at least one
of the elementary_events in the entire sample space will occur is 1.
         P ( &#x03A9; ) = 1.   {\displaystyle P(\Omega )=1.}  [P(\Omega )=1.]
**** Third axiom[edit] ****
This is the assumption of σ-additivity:
      Any countable sequence of disjoint sets (synonymous with mutually
      exclusive events)      E  1   ,  E  2   , &#x2026;   {\displaystyle E_
      {1},E_{2},\ldots }  [{\displaystyle E_{1},E_{2},\ldots }] satisfies
               P  (   &#x22C3;  i = 1   &#x221E;    E  i    )  =  &#x2211;  i =
            1   &#x221E;   P (  E  i   ) .   {\displaystyle P\left(\bigcup _
            {i=1}^{\infty }E_{i}\right)=\sum _{i=1}^{\infty }P(E_{i}).}
            [P\left(\bigcup _{i=1}^{\infty }E_{i}\right)=\sum _{i=1}^{\infty }P
            (E_{i}).]
Some authors consider merely finitely_additive probability spaces, in which
case one just needs an algebra_of_sets, rather than a σ-algebra.
Quasiprobability_distributions in general relax the third axiom.
***** Consequences[edit] *****
From the Kolmogorov axioms, one can deduce other useful rules for calculating
probabilities.
**** The probability of the empty set[edit] ****
         P ( &#x2205; ) = 0.   {\displaystyle P(\varnothing )=0.}  [P
      (\varnothing )=0.]
In some cases,     &#x2205;   {\displaystyle \varnothing }  [\varnothing ] is
not the only event with probability 0.
**** Monotonicity[edit] ****
           if   A &#x2286; B   then   P ( A ) &#x2264; P ( B ) .
      {\displaystyle \quad {\text{if}}\quad A\subseteq B\quad {\text
      {then}}\quad P(A)\leq P(B).}  [\quad {\text{if}}\quad A\subseteq B\quad
      {\text{then}}\quad P(A)\leq P(B).]
If A is a subset of, or equal to B, then the probability of A is less than, or
equal to the probability of B.
**** The numeric bound[edit] ****
It immediately follows from the monotonicity property that
         0 &#x2264; P ( E ) &#x2264; 1  &#x2200; E &#x2208; F .
      {\displaystyle 0\leq P(E)\leq 1\qquad \forall E\in F.}  [0\leq P(E)\leq
      1\qquad \forall E\in F.]
***** Proofs[edit] *****
The proofs of these properties are both interesting and insightful. They
illustrate the power of the third axiom, and its interaction with the remaining
two axioms. When studying axiomatic probability_theory, many deep consequences
follow from merely these three axioms. In order to verify the monotonicity
property, we set      E  1   = A   {\displaystyle E_{1}=A}  [E_{1}=A] and
E  2   = B &#x2216; A   {\displaystyle E_{2}=B\setminus A}  [{\displaystyle E_
{2}=B\setminus A}], where      A &#x2286; B   {\displaystyle \quad A\subseteq
B}  [{\displaystyle \quad A\subseteq B}] and      E  i   = &#x2205;
{\displaystyle E_{i}=\varnothing }  [{\displaystyle E_{i}=\varnothing }] for
i &#x2265; 3   {\displaystyle i\geq 3}  [i\geq 3]. It is easy to see that the
sets      E  i     {\displaystyle E_{i}}  [E_{i}] are pairwise disjoint and
E  1   &#x222A;  E  2   &#x222A; &#x22EF; = B   {\displaystyle E_{1}\cup E_
{2}\cup \cdots =B}  [{\displaystyle E_{1}\cup E_{2}\cup \cdots =B}]. Hence, we
obtain from the third axiom that
         P ( A ) + P ( B &#x2216; A ) +  &#x2211;  i = 3   &#x221E;   P (  E  i
      ) = P ( B ) .   {\displaystyle P(A)+P(B\setminus A)+\sum _{i=3}^{\infty
      }P(E_{i})=P(B).}  [{\displaystyle P(A)+P(B\setminus A)+\sum _{i=3}^
      {\infty }P(E_{i})=P(B).}]
Since the left-hand side of this equation is a series of non-negative numbers,
and since it converges to     P ( B )   {\displaystyle P(B)}  [P(B)] which is
finite, we obtain both     P ( A ) &#x2264; P ( B )   {\displaystyle P(A)\leq P
(B)}  [P(A)\leq P(B)] and     P ( &#x2205; ) = 0   {\displaystyle P(\varnothing
)=0}  [P(\varnothing )=0]. The second part of the statement is seen by
contradiction: if     P ( &#x2205; ) = a   {\displaystyle P(\varnothing )=a}
[P(\varnothing )=a] then the left hand side is not less than infinity
          &#x2211;  i = 3   &#x221E;   P (  E  i   ) =  &#x2211;  i = 3
      &#x221E;   P ( &#x2205; ) =  &#x2211;  i = 3   &#x221E;   a =   {    0
      if&#xA0;  a = 0 ,     &#x221E;    if&#xA0;  a > 0.         {\displaystyle
      \sum _{i=3}^{\infty }P(E_{i})=\sum _{i=3}^{\infty }P(\varnothing )=\sum _
      {i=3}^{\infty }a={\begin{cases}0&{\text{if }}a=0,\\\infty &{\text{if
      }}a>0.\end{cases}}}  [\sum _{i=3}^{\infty }P(E_{i})=\sum _{i=3}^{\infty
      }P(\varnothing )=\sum _{i=3}^{\infty }a={\begin{cases}0&{\text{if
      }}a=0,\\\infty &{\text{if }}a>0.\end{cases}}]
If     a > 0   {\displaystyle a>0}  [a>0] then we obtain a contradiction,
because the sum does not exceed     P ( B )   {\displaystyle P(B)}  [P(B)]
which is finite. Thus,     a = 0   {\displaystyle a=0}  [a=0]. We have shown as
a byproduct of the proof of monotonicity that     P ( &#x2205; ) = 0
{\displaystyle P(\varnothing )=0}  [P(\varnothing )=0].
***** Further consequences[edit] *****
Another important property is:
         P ( A &#x222A; B ) = P ( A ) + P ( B ) &#x2212; P ( A &#x2229; B ) .
      {\displaystyle P(A\cup B)=P(A)+P(B)-P(A\cap B).}  [P(A\cup B)=P(A)+P(B)-P
      (A\cap B).]
This is called the addition law of probability, or the sum rule. That is, the
probability that A or B will happen is the sum of the probabilities that A will
happen and that B will happen, minus the probability that both A and B will
happen. The proof of this is as follows:
Firstly,
         P ( A &#x222A; B ) = P ( A ) + P ( B &#x2216; A )   {\displaystyle P
      (A\cup B)=P(A)+P(B\setminus A)}  [{\displaystyle P(A\cup B)=P(A)+P
      (B\setminus A)}] (by Axiom 3)
So,
         P ( A &#x222A; B ) = P ( A ) + P ( B &#x2216; ( A &#x2229; B ) )
      {\displaystyle P(A\cup B)=P(A)+P(B\setminus (A\cap B))}  [{\displaystyle
      P(A\cup B)=P(A)+P(B\setminus (A\cap B))}] (by     B &#x2216; A = B
      &#x2216; ( A &#x2229; B )   {\displaystyle B\setminus A=B\setminus (A\cap
      B)}  [{\displaystyle B\setminus A=B\setminus (A\cap B)}]).
Also,
         P ( B ) = P ( B &#x2216; ( A &#x2229; B ) ) + P ( A &#x2229; B )
      {\displaystyle P(B)=P(B\setminus (A\cap B))+P(A\cap B)}  [P(B)=P
      (B\setminus (A\cap B))+P(A\cap B)]
and eliminating     P ( B &#x2216; ( A &#x2229; B ) )   {\displaystyle P
(B\setminus (A\cap B))}  [P(B\setminus (A\cap B))] from both equations gives us
the desired result.
An extension of the addition law to any number of sets is the
inclusionâexclusion_principle.
Setting B to the complement Ac of A in the addition law gives
         P  (  A  c   )  = P ( &#x03A9; &#x2216; A ) = 1 &#x2212; P ( A )
      {\displaystyle P\left(A^{c}\right)=P(\Omega \setminus A)=1-P(A)}  [
      {\displaystyle P\left(A^{c}\right)=P(\Omega \setminus A)=1-P(A)}]
That is, the probability that any event will not happen (or the event's
complement) is 1 minus the probability that it will.
***** Simple example: coin toss[edit] *****
Consider a single coin-toss, and assume that the coin will either land heads
(H) or tails (T) (but not both). No assumption is made as to whether the coin
is fair.
We may define:
         &#x03A9; = { H , T }   {\displaystyle \Omega =\{H,T\}}  [\Omega =\
      {H,T\}]
         F = { &#x2205; , { H } , { T } , { H , T } }   {\displaystyle F=\
      {\varnothing ,\{H\},\{T\},\{H,T\}\}}  [F=\{\varnothing ,\{H\},\{T\},\
      {H,T\}\}]
Kolmogorov's axioms imply that:
         P ( &#x2205; ) = 0   {\displaystyle P(\varnothing )=0}  [P(\varnothing
      )=0]
The probability of neither heads nor tails, is 0.
         P ( { H , T  }  c   ) = 0   {\displaystyle P(\{H,T\}^{c})=0}  [
      {\displaystyle P(\{H,T\}^{c})=0}]
The probability of either heads or tails, is 1.
         P ( { H } ) + P ( { T } ) = 1   {\displaystyle P(\{H\})+P(\{T\})=1}
      [P(\{H\})+P(\{T\})=1]
The sum of the probability of heads and the probability of tails, is 1.
***** See also[edit] *****
    * Borel_algebra
    * Ï-algebra
    * Set_theory
    * Conditional_probability
    * Quasiprobability
    * Fully_probabilistic_design
 This article includes a list_of_references, related reading or external_links,
 but its sources remain unclear because it lacks inline_citations. Please help
 to improve this article by introducing more precise citations. (November 2010)
 (Learn_how_and_when_to_remove_this_template_message)
***** Further reading[edit] *****
    * DeGroot,_Morris_H. (1975). Probability and Statistics. Reading: Addison-
      Wesley. pp. 12â16. ISBN 0-201-01503-X.
McCord, James R.; Moroney, Richard M. (1964). "Axiomatic Probability".
Introduction to Probability Theory. New York: Macmillan. pp. 13â28.
***** External links[edit] *****
    * Kolmogorov`s_probability_calculus, Stanford Encyclopedia of Philosophy.
    * Formal_definition of probability in the Mizar_system, and the list_of
      theorems formally proved about it.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Probability_axioms&oldid=896762513"
Categories:
    * Probability_theory
    * Mathematical_axioms
Hidden categories:
    * Articles_lacking_in-text_citations_from_November_2010
    * All_articles_lacking_in-text_citations
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
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * Ãslenska
    * ×¢××¨××ª
    * á¥áá áá£áá
    * Nederlands
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * Suomi
    * Svenska
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 12 May 2019, at 18:38 (UTC).
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
