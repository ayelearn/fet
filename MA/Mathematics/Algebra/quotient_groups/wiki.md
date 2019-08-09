The following text has been accessed from https://en.wikipedia.org/wiki/Quotient_group at Fri Aug 9 02:39:18 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Quotient group ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Algebraic_structure â Group theory
Group_theory
[Cyclic_group.svg]
Basic notions
    * Subgroup
    * Normal_subgroup
    * Quotient group
    * (Semi-)direct_product
Group_homomorphisms
    * kernel
    * image
    * direct_sum
    * wreath_product
    * simple
    * finite
    * infinite
    * continuous
    * multiplicative
    * additive
    * cyclic
    * abelian
    * dihedral
    * nilpotent
    * solvable
    * List_of_group_theory_topics
Finite_groups
Classification_of_finite_simple_groups
    * cyclic
    * alternating
    * Lie_type
    * sporadic
    * Lagrange's_theorem
    * Sylow_theorems
    * Hall's_theorem
    * p-group
    * Elementary_abelian_group
    * Frobenius_group
    * Schur_multiplier
    * Symmetric_group Sn
    * Klein_four-group V
    * Dihedral_group Dn
    * Quaternion_group Q
    * Dicyclic_group Dicn
    * Discrete_groups
    * Lattices
    * Integers (Z)
    * Free_group
Modular_groups
    * PSL(2,Z)
    * SL(2,Z)
    * Arithmetic_group
    * Lattice
    * Hyperbolic_group
Topological and Lie_groups
    * Solenoid
    * Circle
    * General_linear GL(n)
    * Special_linear SL(n)
    * Orthogonal O(n)
    * Euclidean E(n)
    * Special_orthogonal SO(n)
    * Unitary U(n)
    * Special_unitary SU(n)
    * Symplectic Sp(n)
    * G2
    * F4
    * E6
    * E7
    * E8
    * Lorentz
    * PoincarÃ©
    * Conformal
    * Diffeomorphism
    * Loop
Infinite_dimensional_Lie_group
    * O(â)
    * SU(â)
    * Sp(â)
Algebraic_groups
    * Linear_algebraic_group
    * Reductive_group
    * Abelian_variety
    * Elliptic_curve
    * v
    * t
    * e
A quotient group or factor group is a mathematical group obtained by
aggregating similar elements of a larger group using an equivalence_relation
that preserves some of the group structure (the rest of the structure is
"factored" out). For example, the cyclic_group of addition_modulo_n can be
obtained from the group of integers under addition by identifying elements that
differ by a multiple of n and defining a group structure that operates on each
such class (known as a congruence_class) as a single entity. It is part of the
mathematical field known as group_theory.
In a quotient of a group, the equivalence_class of the identity_element is
always a normal_subgroup of the original group, and the other equivalence
classes are precisely the cosets of that normal subgroup. The resulting
quotient is written G / N, where G is the original group and N is the normal
subgroup. (This is pronounced "G mod N", where "mod" is short for modulo.)
Much of the importance of quotient groups is derived from their relation to
homomorphisms. The first_isomorphism_theorem states that the image of any group
G under a homomorphism is always isomorphic to a quotient of G. Specifically,
the image of G under a homomorphism Ï: G â H is isomorphic to G / ker(Ï)
where ker(Ï) denotes the kernel of Ï.
The dual notion of a quotient group is a subgroup, these being the two primary
ways of forming a smaller group from a larger one. Any normal subgroup has a
corresponding quotient group, formed from the larger group by eliminating the
distinction between elements of the subgroup. In category_theory, quotient
groups are examples of quotient_objects, which are dual to subobjects. For
other examples of quotient objects, see quotient_ring, quotient_space_(linear
algebra), quotient_space_(topology), and quotient_set.
⁰
***** Contents *****
    * 1_Definition_and_illustration
          o 1.1_Definition
          o 1.2_Example:_Addition_modulo_6
    * 2_Motivation_for_the_name_"quotient"
    * 3_Examples
          o 3.1_Even_and_odd_integers
          o 3.2_Remainders_of_integer_division
          o 3.3_Complex_integer_roots_of_1
          o 3.4_Sums_of_integers_and_real_numbers
          o 3.5_Matrices_of_real_numbers
          o 3.6_Integer_modular_arithmetic
          o 3.7_Integer_multiplication
    * 4_Properties
    * 5_Quotients_of_Lie_groups
    * 6_See_also
    * 7_Notes
    * 8_References
***** Definition and illustration[edit] *****
Given a group G and a subgroup H, and an element a in G, one can consider the
corresponding left coset: aH := { ah : h in H }. Cosets are a natural class of
subsets of a group; for example consider the abelian group G of integers, with
operation defined by the usual addition, and the subgroup H of even integers.
Then there are exactly two cosets: 0 + H, which are the even integers, and 1 +
H, which are the odd integers (here we are using additive notation for the
binary operation instead of multiplicative notation).
For a general subgroup H, it is desirable to define a compatible group
operation on the set of all possible cosets, { aH : a in G }. This is possible
exactly when H is a normal_subgroup, see below. A subgroup N of a group G is
normal if_and_only_if the coset equality aN = Na holds for all a in G. A normal
subgroup of G is denoted N â G.
**** Definition[edit] ****
Let N be a normal subgroup of a group G. Define the set G/N to be the set of
all left cosets of N in G. That is, G/N = { aN : a ∈ G }. Since the identity
element e ∈ N, a ∈ aN. Define an operation on the set of cosets, G/N, as
follows. For each aN and bN in G/N, the product of aN and bN, (aN)(bN), is
(ab)N. This works only because (ab)N does not depend on the choice of the
representatives, a and b, of each left coset, aN and bN. To prove this suppose
xN = aN and yN = bN for some x, y in G. Then
      (ab)N = a(bN) = a(yN) = a(Ny) = (aN)y = (xN)y = x(Ny) = x(yN) = (xy)N.
This depends on the fact that N is a normal subgroup. It still remains to be
shown that this condition is not only sufficient but necessary to define the
operation on G/N, which will not be done here. Nonetheless, it can be checked
that this operation on G/N is always associative. G/N has identity element N
and the inverse of element aN can always be represented by aâ1N. Therefore,
the set G/N together with the operation defined by (aN)(bN) = (ab)N forms a
group; this is known as the quotient group of G by N.
Due to the normality of N, the left cosets and right cosets of N in G are the
same, and so, G/N could have been defined to be the set of right cosets of N in
G.
**** Example: Addition modulo 6[edit] ****
For example, consider the group with addition modulo 6: G = {0, 1, 2, 3, 4, 5}.
Consider the subgroup N = {0, 3}, which is normal because G is abelian. Then
the set of (left) cosets is of size three:
      G/N = { a+N : a ∈ G } = { {0, 3}, {1, 4}, {2, 5} } = { 0+N, 1+N, 2+N }.
The binary operation defined above makes this set into a group, known as the
quotient group, which in this case is isomorphic to the cyclic_group of order
3.
***** Motivation for the name "quotient"[edit] *****
The reason G/N is called a quotient group comes from division of integers. When
dividing 12 by 3 one obtains the answer 4 because one can regroup 12 objects
into 4 subcollections of 3 objects. The quotient group is the same idea,
although we end up with a group for a final answer instead of a number because
groups have more structure than an arbitrary collection of objects.
To elaborate, when looking at G/N with N a normal subgroup of G, the group
structure is used to form a natural "regrouping". These are the cosets of N in
G. Because we started with a group and normal subgroup, the final quotient
contains more information than just the number of cosets (which is what regular
division yields), but instead has a group structure itself.
***** Examples[edit] *****
**** Even and odd integers[edit] ****
Consider the group of integers Z (under addition) and the subgroup 2Z
consisting of all even integers. This is a normal subgroup, because Z is
abelian. There are only two cosets: the set of even integers and the set of odd
integers, and therefore the quotient group Z/2Z is the cyclic group with two
elements. This quotient group is isomorphic with the set {0,1} with addition
modulo 2; informally, it is sometimes said that Z/2Z equals the set {0,1} with
addition modulo 2.
Example further explained...
Let     &#x03B3; ( m ) =   {\displaystyle \gamma (m)=}  [{\displaystyle \gamma
(m)=}] remainders of     m &#x2208;  Z    {\displaystyle m\in \mathbb {Z} }  [
{\displaystyle m\in \mathbb {Z} }] when dividing by     2   {\displaystyle 2}
[2].
Then     &#x03B3; ( m ) = 0   {\displaystyle \gamma (m)=0}  [{\displaystyle
\gamma (m)=0}] when     m   {\displaystyle m}  [m] is even and     &#x03B3; ( m
) = 1   {\displaystyle \gamma (m)=1}  [{\displaystyle \gamma (m)=1}] when     m
{\displaystyle m}  [m] is odd.
By definition of     &#x03B3;   {\displaystyle \gamma }  [\gamma ], the kernel
of     &#x03B3;   {\displaystyle \gamma }  [\gamma ],
ker(    &#x03B3;   {\displaystyle \gamma }  [\gamma ])     = { m &#x2208;  Z  :
&#x03B3; ( m ) = 0 }   {\displaystyle =\{m\in \mathbb {Z} :\gamma (m)=0\}}  [
{\displaystyle =\{m\in \mathbb {Z} :\gamma (m)=0\}}], is the set of all even
integers.
Let     H =   {\displaystyle H=}  [{\displaystyle H=}] ker(    &#x03B3;
{\displaystyle \gamma }  [\gamma ]).
Then     H   {\displaystyle H}  [H] is a subgroup, because the identity in
Z    {\displaystyle \mathbb {Z} }  [ \Z ], which is     0   {\displaystyle 0}
[{\displaystyle  0 }], is in     H   {\displaystyle H}  [H],
the sum of two even integers is even and hence if     m   {\displaystyle m}
[m] and     n   {\displaystyle n}  [n] are in     H   {\displaystyle H}  [H],
m + n   {\displaystyle m+n}  [{\displaystyle m+n}] is in     H   {\displaystyle
H}  [H] (closure)
and if     m   {\displaystyle m}  [m] is even,     &#x2212; m   {\displaystyle
-m}  [{\displaystyle -m}] is also even and so     H   {\displaystyle H}  [H]
contains its inverses.
Define     &#x03BC; :   {\displaystyle \mu :}  [{\displaystyle \mu :}]      Z
{\displaystyle \mathbb {Z} }  [\mathbb {Z} ] / H    &#x2192;   Z   2
{\displaystyle \to \mathbb {Z} _{2}}  [{\displaystyle \to \mathbb {Z} _{2}}] as
&#x03BC; ( a H ) = &#x03B3; ( a )   {\displaystyle \mu (aH)=\gamma (a)}  [
{\displaystyle \mu (aH)=\gamma (a)}] for     a &#x2208;  Z    {\displaystyle
a\in \mathbb {Z} }  [{\displaystyle a\in \mathbb {Z} }]
and       Z    {\displaystyle \mathbb {Z} }  [\mathbb {Z} ] / H is the quotient
group of left cosets;       Z    {\displaystyle \mathbb {Z} }  [\mathbb {Z} ] /
H    = { H , 1 + H }   {\displaystyle =\{H,1+H\}}  [{\displaystyle =\
{H,1+H\}}].
By the way we have defined     &#x03BC;   {\displaystyle \mu }  [\mu ],
&#x03BC; ( a H )   {\displaystyle \mu (aH)}  [{\displaystyle \mu (aH)}] is
1   {\displaystyle 1}  [1] if     a   {\displaystyle a}  [a] is odd and     0
{\displaystyle 0}  [{\displaystyle  0 }] if     a   {\displaystyle a}  [a] is
even.
Thus,     &#x03BC;   {\displaystyle \mu }  [\mu ] is an isomorphism from
Z    {\displaystyle \mathbb {Z} }  [\mathbb {Z} ] / H to       Z   2
{\displaystyle \mathbb {Z} _{2}}  [{\displaystyle \mathbb {Z} _{2}}].
**** Remainders of integer division[edit] ****
A slight generalization of the last example. Once again consider the group of
integers Z under addition. Let n be any positive integer. We will consider the
subgroup nZ of Z consisting of all multiples of n. Once again nZ is normal in Z
because Z is abelian. The cosets are the collection {nZ, 1+nZ, ..., (n−2)+nZ,
(n−1)+nZ}. An integer k belongs to the coset r+nZ, where r is the remainder
when dividing k by n. The quotient Z/nZ can be thought of as the group of
"remainders" modulo n. This is a cyclic_group of order n.
**** Complex integer roots of 1[edit] ****
The cosets of the fourth roots_of_unity N in the twelfth roots of unity G.
The twelfth roots_of_unity, which are points on the complex unit_circle, form a
multiplicative abelian group G, shown on the picture on the right as colored
balls with the number at each point giving its complex argument. Consider its
subgroup N made of the fourth roots of unity, shown as red balls. This normal
subgroup splits the group into three cosets, shown in red, green and blue. One
can check that the cosets form a group of three elements (the product of a red
element with a blue element is blue, the inverse of a blue element is green,
etc.). Thus, the quotient group G/N is the group of three colors, which turns
out to be the cyclic group with three elements.
**** Sums of integers and real numbers[edit] ****
Consider the group of real_numbers R under addition, and the subgroup Z of
integers. The cosets of Z in R are all sets of the form a+Z, with 0 â¤ a < 1 a
real number. Adding such cosets is done by adding the corresponding real
numbers, and subtracting 1 if the result is greater than or equal to 1. The
quotient group R/Z is isomorphic to the circle_group S1, the group of complex
numbers of absolute_value 1 under multiplication, or correspondingly, the group
of rotations in 2D about the origin, that is, the special orthogonal_group SO
(2). An isomorphism is given by f(a+Z) = exp(2Ïia) (see Euler's_identity).
**** Matrices of real numbers[edit] ****
If G is the group of invertible 3 Ã 3 real matrices, and N is the subgroup of
3 Ã 3 real matrices with determinant 1, then N is normal in G (since it is the
kernel of the determinant homomorphism). The cosets of N are the sets of
matrices with a given determinant, and hence G/N is isomorphic to the
multiplicative group of non-zero real numbers. The group N is known as the
special_linear_group SL(3).
**** Integer modular arithmetic[edit] ****
Consider the abelian group Z4 = Z/4Z (that is, the set { 0, 1, 2, 3 } with
addition modulo 4), and its subgroup { 0, 2 }. The quotient group Z4/{ 0, 2 }
is { { 0, 2 }, { 1, 3 } }. This is a group with identity element { 0, 2 }, and
group operations such as { 0, 2 } + { 1, 3 } = { 1, 3 }. Both the subgroup { 0,
2 } and the quotient group { { 0, 2 }, { 1, 3 } } are isomorphic with Z2.
**** Integer multiplication[edit] ****
Consider the multiplicative group     G =   Z    n  2     &#x2217;
{\displaystyle G=\mathbf {Z} _{n^{2}}^{*}}  [G=\mathbf{Z}^*_{n^2}]. The set N
of nth residues is a multiplicative subgroup isomorphic to       Z   n
&#x2217;     {\displaystyle \mathbf {Z} _{n}^{*}}  [\mathbf{Z}^*_{n}]. Then N
is normal in G and the factor group G/N has the cosets N, (1+n)N, (1+n)2N, ...,
(1+n)n−1N. The Paillier_cryptosystem is based on the conjecture that it is
difficult to determine the coset of a random element of G without knowing the
factorization of n.
***** Properties[edit] *****
The quotient group G/G is isomorphic to the trivial_group (the group with one
element), and G/{e} is isomorphic to G.
The order of G/N, by definition the number of elements, is equal to |G : N|,
the index of N in G. If G is finite, the index is also equal to the order of G
divided by the order of N. Note that G/N may be finite, although both G and N
are infinite (for example, Z/2Z).
There is a "natural" surjective group_homomorphism Ï : G â G/N, sending each
element g of G to the coset of N to which g belongs, that is: Ï(g) = gN. The
mapping Ï is sometimes called the canonical projection of G onto G/N. Its
kernel is N.
There is a bijective correspondence between the subgroups of G that contain N
and the subgroups of G/N; if H is a subgroup of G containing N, then the
corresponding subgroup of G/N is Ï(H). This correspondence holds for normal
subgroups of G and G/N as well, and is formalized in the lattice_theorem.
Several important properties of quotient groups are recorded in the fundamental
theorem_on_homomorphisms and the isomorphism_theorems.
If G is abelian, nilpotent, solvable, cyclic or finitely_generated, then so is
G/N.
If H is a subgroup in a finite group G, and the order of H is one half of the
order of G, then H is guaranteed to be a normal subgroup, so G/H exists and is
isomorphic to C2. This result can also be stated as "any subgroup of index 2 is
normal", and in this form it applies also to infinite groups. Furthermore, if p
is the smallest prime number dividing the order of a finite group, G, then if
G/H has order p, H must be a normal subgroup of G.[1]
Given G and a normal subgroup N, then G is a group_extension of G/N by N. One
could ask whether this extension is trivial or split; in other words, one could
ask whether G is a direct_product or semidirect_product of N and G/N. This is a
special case of the extension_problem. An example where the extension is not
split is as follows: Let G = Z4 = {0, 1, 2, 3}, and N = {0, 2}, which is
isomorphic to Z2. Then G/N is also isomorphic to Z2. But Z2 has only the
trivial automorphism, so the only semi-direct product of N and G/N is the
direct product. Since Z4 is different from Z2 Ã Z2, we conclude that G is not
a semi-direct product of N and G/N.
***** Quotients of Lie groups[edit] *****
If G is a Lie_group and N is a normal Lie_subgroup of G, the quotient G / N is
also a Lie group. In this case, the original group G has the structure of a
fiber_bundle (specifically, a principal_N-bundle), with base space G / N and
fiber N.
For a non-normal Lie subgroup N, the space G / N of left cosets is not a group,
but simply a differentiable_manifold on which G acts. The result is known as a
homogeneous_space.
***** See also[edit] *****
    * Group_extension
    * Lattice_theorem
    * Quotient_category
    * Short_exact_sequence
***** Notes[edit] *****
   1. ^ Dummit_&_Foote_(2003, p. 120)
***** References[edit] *****
    * Dummit, David S.; Foote, Richard M. (2003), Abstract Algebra (3rd ed.),
      New York: Wiley, ISBN 978-0-471-43334-7
Herstein, I. N. (1975), Topics in Algebra (2nd ed.), New York: Wiley, ISBN 0-
471-02371-X

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Quotient_group&oldid=904064742"
Categories:
    * Group_theory
    * Quotient_objects
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * à´®à´²à´¯à´¾à´³à´
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 29 June 2019, at 19:06 (UTC).
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
