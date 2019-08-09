The following text has been accessed from https://en.wikipedia.org/wiki/Urysohn%27s_lemma at Fri Aug 9 02:34:27 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Urysohn's lemma ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In topology, Urysohn's lemma is a lemma that states that a topological_space is
normal if and only if any two disjoint closed_subsets can be separated by a
continuous_function.[1]
Urysohn's lemma is commonly used to construct continuous functions with various
properties on normal spaces. It is widely applicable since all metric_spaces
and all compact Hausdorff_spaces are normal. The lemma is generalized by (and
usually used in the proof of) the Tietze_extension_theorem.
The lemma is named after the mathematician Pavel_Samuilovich_Urysohn.
⁰
***** Contents *****
    * 1_Formal_statement
    * 2_Sketch_of_proof
    * 3_See_also
    * 4_Notes
    * 5_References
    * 6_External_links
***** Formal statement[edit] *****
Two subsets A and B of a topological_space X are said to be separated_by
neighbourhoods if there are neighbourhoods U of A and V of B that are disjoint.
In particular A and B are necessarily disjoint.
Two plain subsets A and B are said to be separated_by_a_function if there
exists a continuous_function f from X into the unit_interval [0,1] such that f
(a) = 0 for all a in A and f(b) = 1 for all b in B. Any such function is called
a Urysohn function for A and B. In particular A and B are necessarily disjoint.
It follows that if two subsets A and B are separated_by_a_function then so are
their closures.
Also it follows that if two subsets A and B are separated_by_a_function then A
and B are separated_by_neighbourhoods.
A normal_space is a topological space in which any two disjoint closed sets can
be separated by neighbourhoods. Urysohn's lemma states that a topological space
is normal if and only if any two disjoint closed sets can be separated by a
continuous function.
The sets A and B need not be precisely_separated_by_f, i.e., we do not, and in
general cannot, require that f(x) â  0 and â  1 for x outside of A and B. The
spaces in which this property holds are the perfectly_normal_spaces.
Urysohn's lemma has led to the formulation of other topological properties such
as the 'Tychonoff property' and 'completely Hausdorff spaces'. For example, a
corollary of the lemma is that normal T1_spaces are Tychonoff.
***** Sketch of proof[edit] *****
Illustration of Urysohn's "onion" function.
The procedure is an entirely straightforward application of the definition of
normality (once one draws some figures representing the first few steps in the
induction described below to see what is going on), beginning with two disjoint
closed sets. The clever part of the proof is the indexing the open sets thus
constructed by dyadic fractions.
For every dyadic_fraction r â (0,1), we are going to construct an open_subset
U(r) of X such that:
   1. U(r) contains A and is disjoint from B for all r
   2. for r < s, the closure of U(r) is contained in U(s).
Once we have these sets, we define f(x) = 1 if x â U(r) for any r; otherwise
f(x) = inf { r : x â U(r) } for every x â X. Using the fact that the dyadic
rationals are dense, it is then not too hard to show that f is continuous and
has the property f(A) â {0} and f(B) â {1}.
In order to construct the sets U(r), we actually do a little bit more: we
construct sets U(r) and V(r) such that
    * A â U(r) and B â V(r) for all r
    * U(r) and V(r) are open and disjoint for all r
    * for r < s, V(s) is contained in the complement of U(r) and the complement
      of V(r) is contained in U(s).
Since the complement of V(r) is closed and contains U(r), the latter condition
then implies condition (2) from above.
This construction proceeds by mathematical_induction. First define U(1) = X \ B
and V(0) = X \ A. Since X is normal, we can find two disjoint open sets U(1/2)
and V(1/2) which contain A and B, respectively. Now assume that nâ¥1 and the
sets U(k/2n) and V(k/2n) have already been constructed for k = 1,...,2n-1.
Since X is normal, for any a â { 0,1,...,2n-1 }, we can find two disjoint
open sets which contain X \ V(a/2n) and X \ U((a+1)/2n), respectively. Call
these two open sets U((2a+1)/2n+1) and V((2a+1)/2n+1), and verify the above
three conditions.
The Mizar_project has completely formalized and automatically checked a proof
of Urysohn's lemma in the URYSOHN3_file.
***** See also[edit] *****
    * Cutoff_function
***** Notes[edit] *****
   1. ^ Willard_1970 Section 15.
***** References[edit] *****
    * Willard, Stephen (1970). General Topology. Dover Publications. ISBN 0-
      486-43479-6.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Urysohn_lemma", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
"proof_of_Urysohn's_lemma". PlanetMath.
Mizar_system proof: http://mizar.org/version/current/html/urysohn3.html#T20

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Urysohn%27s_lemma&oldid=870217267"
Categories:
    * Lemmas
    * Theorems_in_topology
    * Separation_axioms
Hidden categories:
    * Articles_containing_proofs
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
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 23 November 2018, at 07:33 (UTC).
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
