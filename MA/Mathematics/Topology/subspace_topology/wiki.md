The following text has been accessed from https://en.wikipedia.org/wiki/Subspace_topology at Fri Aug 9 02:34:38 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Subspace topology ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In topology and related areas of mathematics, a subspace of a topological_space
X is a subset S of X which is equipped with a topology induced from that of X
called the subspace topology (or the relative topology, or the induced
topology, or the trace topology).
⁰
***** Contents *****
    * 1_Definition
    * 2_Terminology
    * 3_Examples
    * 4_Properties
    * 5_Preservation_of_topological_properties
    * 6_See_also
    * 7_References
***** Definition[edit] *****
Given a topological space     ( X , &#x03C4; )   {\displaystyle (X,\tau )}  [
(X, \tau)] and a subset     S   {\displaystyle S}  [S] of     X
{\displaystyle X}  [X], the subspace topology on     S   {\displaystyle S}  [S]
is defined by
          &#x03C4;  S   = { S &#x2229; U &#x2223; U &#x2208; &#x03C4; } .
      {\displaystyle \tau _{S}=\lbrace S\cap U\mid U\in \tau \rbrace .}
      [\tau_S = \lbrace S \cap U \mid U \in \tau \rbrace.]
That is, a subset of     S   {\displaystyle S}  [S] is open in the subspace
topology if_and_only_if it is the intersection of     S   {\displaystyle S}
[S] with an open_set in     ( X , &#x03C4; )   {\displaystyle (X,\tau )}  [(X,
\tau)]. If     S   {\displaystyle S}  [S] is equipped with the subspace
topology then it is a topological space in its own right, and is called a
subspace of     ( X , &#x03C4; )   {\displaystyle (X,\tau )}  [(X, \tau)].
Subsets of topological spaces are usually assumed to be equipped with the
subspace topology unless otherwise stated.
Alternatively we can define the subspace topology for a subset     S
{\displaystyle S}  [S] of     X   {\displaystyle X}  [X] as the coarsest
topology for which the inclusion_map
         &#x03B9; : S &#x21AA; X   {\displaystyle \iota :S\hookrightarrow X}
      [\iota: S \hookrightarrow X]
is continuous.
More generally, suppose     &#x03B9;   {\displaystyle \iota }  [\iota ] is an
injection from a set     S   {\displaystyle S}  [S] to a topological space
X   {\displaystyle X}  [X]. Then the subspace topology on     S
{\displaystyle S}  [S] is defined as the coarsest topology for which
&#x03B9;   {\displaystyle \iota }  [\iota ] is continuous. The open sets in
this topology are precisely the ones of the form      &#x03B9;  &#x2212; 1
( U )   {\displaystyle \iota ^{-1}(U)}  [\iota^{-1}(U)] for     U
{\displaystyle U}  [U] open in     X   {\displaystyle X}  [X].     S
{\displaystyle S}  [S] is then homeomorphic to its image in     X
{\displaystyle X}  [X] (also with the subspace topology) and     &#x03B9;
{\displaystyle \iota }  [\iota ] is called a topological_embedding.
A subspace     S   {\displaystyle S}  [S] is called an open subspace if the
injection     &#x03B9;   {\displaystyle \iota }  [\iota ] is an open_map, i.e.,
if the forward image of an open set of     S   {\displaystyle S}  [S] is open
in     X   {\displaystyle X}  [X]. Likewise it is called a closed subspace if
the injection     &#x03B9;   {\displaystyle \iota }  [\iota ] is a closed_map.
***** Terminology[edit] *****
The distinction between a set and a topological space is often blurred
notationally, for convenience, which can be a source of confusion when one
first encounters these definitions. Thus, whenever     S   {\displaystyle S}
[S] is a subset of     X   {\displaystyle X}  [X], and     ( X , &#x03C4; )
{\displaystyle (X,\tau )}  [(X, \tau)] is a topological space, then the
unadorned symbols "    S   {\displaystyle S}  [S]" and "    X   {\displaystyle
X}  [X]" can often be used to refer both to     S   {\displaystyle S}  [S] and
X   {\displaystyle X}  [X] considered as two subsets of     X   {\displaystyle
X}  [X], and also to     ( S ,  &#x03C4;  S   )   {\displaystyle (S,\tau _{S})}
[(S,\tau_S)] and     ( X , &#x03C4; )   {\displaystyle (X,\tau )}  [(X,\tau )]
as the topological spaces, related as discussed above. So phrases such as "
S   {\displaystyle S}  [S] an open subspace of     X   {\displaystyle X}  [X]"
are used to mean that     ( S ,  &#x03C4;  S   )   {\displaystyle (S,\tau _
{S})}  [(S,\tau_S)] is an open subspace of     ( X , &#x03C4; )
{\displaystyle (X,\tau )}  [(X,\tau )], in the sense used below -- that is
that: (i)     S &#x2208; &#x03C4;   {\displaystyle S\in \tau }  [S\in \tau];
and (ii)     S   {\displaystyle S}  [S] is considered to be endowed with the
subspace topology.
***** Examples[edit] *****
In the following,      R    {\displaystyle \mathbb {R} }  [\mathbb {R} ]
represents the real_numbers with their usual topology.
    * The subspace topology of the natural_numbers, as a subspace of      R
      {\displaystyle \mathbb {R} }  [\mathbb {R} ], is the discrete_topology.
    * The rational_numbers      Q    {\displaystyle \mathbb {Q} }  [\mathbb {Q}
      ] considered as a subspace of      R    {\displaystyle \mathbb {R} }
      [\mathbb {R} ] do not have the discrete topology ({0} for example is not
      an open set in      Q    {\displaystyle \mathbb {Q} }  [\mathbb {Q} ]).
      If a and b are rational, then the intervals (a, b) and [a, b] are
      respectively open and closed, but if a and b are irrational, then the set
      of all rational x with a < x < b is both open and closed.
    * The set [0,1] as a subspace of      R    {\displaystyle \mathbb {R} }
      [\mathbb {R} ] is both open and closed, whereas as a subset of      R
      {\displaystyle \mathbb {R} }  [\mathbb {R} ] it is only closed.
    * As a subspace of      R    {\displaystyle \mathbb {R} }  [\mathbb {R} ],
      [0, 1] ∪ [2, 3] is composed of two disjoint open subsets (which happen
      also to be closed), and is therefore a disconnected_space.
    * Let S = [0, 1) be a subspace of the real line      R    {\displaystyle
      \mathbb {R} }  [\mathbb {R} ]. Then [0, 1/2) is open in S but not in
      R    {\displaystyle \mathbb {R} }  [\mathbb {R} ]. Likewise [½, 1) is
      closed in S but not in      R    {\displaystyle \mathbb {R} }  [\mathbb
      {R} ]. S is both open and closed as a subset of itself but not as a
      subset of      R    {\displaystyle \mathbb {R} }  [\mathbb {R} ].
***** Properties[edit] *****
The subspace topology has the following characteristic property. Let     Y
{\displaystyle Y}  [Y] be a subspace of     X   {\displaystyle X}  [X] and let
i : Y &#x2192; X   {\displaystyle i:Y\to X}  [i : Y \to X] be the inclusion
map. Then for any topological space     Z   {\displaystyle Z}  [Z] a map     f
: Z &#x2192; Y   {\displaystyle f:Z\to Y}  [f : Z\to Y] is continuous if_and
only_if the composite map     i &#x2218; f   {\displaystyle i\circ f}  [i\circ
f] is continuous.
[Characteristic_property_of_the_subspace_topology]
This property is characteristic in the sense that it can be used to define the
subspace topology on     Y   {\displaystyle Y}  [Y].
We list some further properties of the subspace topology. In the following let
S   {\displaystyle S}  [S] be a subspace of     X   {\displaystyle X}  [X].
    * If     f : X &#x2192; Y   {\displaystyle f:X\to Y}  [f:X\to Y] is
      continuous the restriction to     S   {\displaystyle S}  [S] is
      continuous.
    * If     f : X &#x2192; Y   {\displaystyle f:X\to Y}  [f:X\to Y] is
      continuous then     f : X &#x2192; f ( X )   {\displaystyle f:X\to f(X)}
      [f:X\to f(X)] is continuous.
    * The closed sets in     S   {\displaystyle S}  [S] are precisely the
      intersections of     S   {\displaystyle S}  [S] with closed sets in     X
      {\displaystyle X}  [X].
    * If     A   {\displaystyle A}  [A] is a subspace of     S   {\displaystyle
      S}  [S] then     A   {\displaystyle A}  [A] is also a subspace of     X
      {\displaystyle X}  [X] with the same topology. In other words the
      subspace topology that     A   {\displaystyle A}  [A] inherits from     S
      {\displaystyle S}  [S] is the same as the one it inherits from     X
      {\displaystyle X}  [X].
    * Suppose     S   {\displaystyle S}  [S] is an open subspace of     X
      {\displaystyle X}  [X] (so     S &#x2208; &#x03C4;   {\displaystyle S\in
      \tau }  [S\in\tau]). Then a subset of     S   {\displaystyle S}  [S] is
      open in     S   {\displaystyle S}  [S] if and only if it is open in     X
      {\displaystyle X}  [X].
    * Suppose     S   {\displaystyle S}  [S] is a closed subspace of     X
      {\displaystyle X}  [X] (so     X &#x2216; S &#x2208; &#x03C4;
      {\displaystyle X\setminus S\in \tau }  [X\setminus S\in\tau]). Then a
      subset of     S   {\displaystyle S}  [S] is closed in     S
      {\displaystyle S}  [S] if and only if it is closed in     X
      {\displaystyle X}  [X].
    * If     B   {\displaystyle B}  [B] is a basis for     X   {\displaystyle
      X}  [X] then      B  S   = { U &#x2229; S : U &#x2208; B }
      {\displaystyle B_{S}=\{U\cap S:U\in B\}}  [B_S = \{U\cap S : U \in B\}]
      is a basis for     S   {\displaystyle S}  [S].
    * The topology induced on a subset of a metric_space by restricting the
      metric to this subset coincides with subspace topology for this subset.
***** Preservation of topological properties[edit] *****
If a topological space having some topological_property implies its subspaces
have that property, then we say the property is hereditary. If only closed
subspaces must share the property we call it weakly hereditary.
    * Every open and every closed subspace of a completely_metrizable space is
      completely metrizable.
    * Every open subspace of a Baire_space is a Baire space.
    * Every closed subspace of a compact_space is compact.
    * Being a Hausdorff_space is hereditary.
    * Being a normal_space is weakly hereditary.
    * Total_boundedness is hereditary.
    * Being totally_disconnected is hereditary.
    * First_countability and second_countability are hereditary.
***** See also[edit] *****
    * the dual notion quotient_space
    * product_topology
    * direct_sum_topology
***** References[edit] *****
    * Bourbaki, Nicolas, Elements of Mathematics: General Topology, Addison-
      Wesley (1966)
    * Steen,_Lynn_Arthur; Seebach,_J._Arthur_Jr. (1995) [1978], Counterexamples
      in_Topology (Dover reprint of 1978 ed.), Berlin, New York: Springer-
      Verlag, ISBN 978-0-486-68735-3, MR 0507446
Willard, Stephen. General Topology, Dover Publications (2004)
ISBN 0-486-43479-6

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Subspace_topology&oldid=805955841"
Categories:
    * Topology
    * General_topology
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
    * Dansk
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * æè¨
    * ä¸­æ
Edit_links
    * This page was last edited on 18 October 2017, at 18:26 (UTC).
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
