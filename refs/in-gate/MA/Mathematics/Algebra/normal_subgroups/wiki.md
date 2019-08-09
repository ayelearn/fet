The following text has been accessed from https://en.wikipedia.org/wiki/Normal_subgroup at Fri Aug 9 02:39:21 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Normal subgroup ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Invariant subgroup" redirects here. It is not to be confused with Fully
invariant_subgroup.
Algebraic_structure â Group theory
Group_theory
[Cyclic_group.svg]
Basic notions
    * Subgroup
    * Normal subgroup
    * Quotient_group
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
In abstract_algebra, a normal subgroup is a subgroup that is invariant under
conjugation by members of the group of which it is a part. In other words, a
subgroup N of the group G is normal in G if and only if gngâ1 â N for all g
â G and n â N. The usual notation for this relation is     N &#x25C3; G
{\displaystyle N\triangleleft G}  [{\displaystyle N\triangleleft G}].
Normal subgroups are important because they (and only they) can be used to
construct quotient_groups of the given group. Furthermore, the normal subgroups
of G are precisely the kernels of group_homomorphisms with domain G, which
means that they can be used to internally classify those homomorphisms.
Ãvariste_Galois was the first to realize the importance of the existence of
normal subgroups.[1]
⁰
***** Contents *****
    * 1_Definitions
          o 1.1_Equivalent_conditions
    * 2_Examples
    * 3_Properties
          o 3.1_Lattice_of_normal_subgroups
    * 4_Normal_subgroups,_quotient_groups_and_homomorphisms
    * 5_See_also
          o 5.1_Operations_taking_subgroups_to_subgroups
          o 5.2_Subgroup_properties_complementary_(or_opposite)_to_normality
          o 5.3_Subgroup_properties_stronger_than_normality
          o 5.4_Subgroup_properties_weaker_than_normality
          o 5.5_Related_notions_in_algebra
    * 6_Notes
    * 7_References
    * 8_Further_reading
    * 9_External_links
***** Definitions[edit] *****
A subgroup N of a group G is called a normal subgroup of G if it is invariant
under conjugation; that is, the conjugation of an element of N by an element of
G is always in N.[2] The usual notation for this relation is     N &#x25C3; G
{\displaystyle N\triangleleft G}  [{\displaystyle N\triangleleft G}], and the
definition may be written in symbols as
   N &#x25C3; G &#x21D4; &#x2200; n &#x2208; N , &#x2200; g &#x2208; G &#x003A;
g n  g  &#x2212; 1   &#x2208; N .   {\displaystyle N\triangleleft
G\Leftrightarrow \forall n\in N,\forall g\in G\colon gng^{-1}\in N.}
[{\displaystyle N\triangleleft G\Leftrightarrow \forall n\in N,\forall g\in
G\colon gng^{-1}\in N.}]
**** Equivalent conditions[edit] ****
For any subgroup N of G, the following conditions are equivalent to N being a
normal subgroup of G. Therefore, any one of them may be taken as the
definition:
    * Any two elements commute regarding the normal subgroup membership
      relation: âg, h â G, gh â N â hg â N.
    * The image of conjugation of N by any element of G is a subset of N: âg
      â G, gNgâ1 â N.[3] In other words, N is preserved by inner
      automorphisms.[4]
    * The image of conjugation of N by any element of G is N: âg â G,
      gNgâ1 = N.[3]
    * âg â G, gN = Ng.[3]
    * The sets of left and right cosets of N in G coincide.[3]
    * The product of an element of the left coset of N with respect to g and an
      element of the left coset of N with respect to h is an element of the
      left coset of N with respect to gh: âx, y, g, h â G, if x â gN and
      y â hN then xy â (gh)N.
    * N is a union of conjugacy_classes of G: N = âgâN Cl(g).[1]
    * For all     n &#x2208; N   {\displaystyle n\in N}  [n\in N] and     g
      &#x2208; G   {\displaystyle g\in G}  [g\in G], the commutator     [ n , g
      ] =  n  &#x2212; 1    g  &#x2212; 1   n g   {\displaystyle [n,g]=n^{-1}g^
      {-1}ng}  [{\displaystyle [n,g]=n^{-1}g^{-1}ng}] is in N.[citation_needed]
    * There is some group_homomorphism G → H whose kernel is N.[1]
***** Examples[edit] *****
    * The trivial subgroup {e} consisting of just the identity element of G and
      G itself are always normal subgroups of G. If these are the only normal
      subgroups, then G is said to be simple.[5]
    * The translation_group is a normal subgroup of the Euclidean_group in any
      dimension.[6] This means: applying a rigid transformation, followed by a
      translation and then the inverse rigid transformation, has the same
      effect as a single translation (though typically a different one than the
      one we used earlier). By contrast, the subgroup of all rotations about
      the origin is not a normal subgroup of the Euclidean group, as long as
      the dimension is at least 2: first translating, then rotating about the
      origin, and then translating back will typically not fix the origin and
      will therefore not have the same effect as a single rotation about the
      origin.
    * Every subgroup N of an abelian_group G is normal, because gN = Ng. A
      group that is not abelian but for which every subgroup is normal is
      called a Hamiltonian_group.[7]
    * The center_of_a_group is a normal subgroup.[8]
    * The commutator_subgroup is a normal subgroup.[9]
    * More generally, any characteristic_subgroup is normal, since conjugation
      is always an automorphism.[10]
    * In the Rubik's_Cube_group, the subgroups consisting of operations which
      only affect the orientations of either the corner pieces or the edge
      pieces are normal.[11]
***** Properties[edit] *****
    * If H is a normal subgroup of G, and K is a subgroup of G containing H,
      then H is a normal subgroup of K.[12]
    * A normal subgroup of a normal subgroup of a group need not be normal in
      the group. That is, normality is not a transitive_relation. The smallest
      group exhibiting this phenomenon is the dihedral_group of order 8.[13]
      However, a characteristic_subgroup of a normal subgroup is normal.[14] A
      group in which normality is transitive is called a T-group.[15]
    * The two groups G and H are normal subgroups of their direct product
      direct_product G × H.
    * If the group G is a semidirect_product     G = N &#x22CA; H ,
      {\displaystyle G=N\rtimes H,}  [G=N\rtimes H,], then N is normal in G,
      though H need not be normal in G.
    * Normality is preserved under surjective homomorphisms,[16] i.e. if G → H
      is a surjective group homomorphism and N is normal in G, then the image f
      (N) is normal in H.
    * Normality is preserved by taking inverse_images,[16] i.e. if G → H is a
      group homomorphism and N is normal in H, then the inverse image f -1(N)
      is normal in G.
    * Normality is preserved on taking direct_products,[17] i.e. if      N  1
      &#x25C3;  G  1     {\displaystyle N_{1}\triangleleft G_{1}}  [
      {\displaystyle N_{1}\triangleleft G_{1}}] and      N  2   &#x25C3;  G  2
      {\displaystyle N_{2}\triangleleft G_{2}}  [{\displaystyle N_
      {2}\triangleleft G_{2}}], then      N  1   &#x00D7;  N  2    &#x25C3;   G
      1   &#x00D7;  G  2     {\displaystyle N_{1}\times N_{2}\;\triangleleft
      \;G_{1}\times G_{2}}  [{\displaystyle N_{1}\times N_{2}\;\triangleleft
      \;G_{1}\times G_{2}}].
    * Every subgroup of index 2 is normal. More generally, a subgroup, H, of
      finite index, n, in G contains a subgroup, K, normal in G and of index
      dividing n! called the normal_core. In particular, if p is the smallest
      prime dividing the order of G, then every subgroup of index p is normal.
      [18]
    * The fact that normal subgroups of G are precisely the kernels of group
      homomorphisms defined on G accounts for some of the importance of normal
      subgroups; they are a way to internally classify all homomorphisms
      defined on a group. For example, a non-identity finite group is simple if
      and only if it is isomorphic to all of its non-identity homomorphic
      images,[19] a finite group is perfect if and only if it has no normal
      subgroups of prime index, and a group is imperfect if and only if the
      derived_subgroup is not supplemented by any proper normal subgroup.
**** Lattice of normal subgroups[edit] ****
Given two normal subgroups, N and M, of G, their intersection     N &#x2229; M
{\displaystyle N\cap M}  [{\displaystyle N\cap M}]and their product     N M =
{ n m &#x2223; n &#x2208; N   &#xA0;and&#xA0;   m &#x2208; M }   {\displaystyle
NM=\{nm\mid n\in N\;{\text{ and }}\;m\in M\}}  [{\displaystyle NM=\{nm\mid n\in
N\;{\text{ and }}\;m\in M\}}] are also normal subgroups of G.
The normal subgroups of G form a lattice under subset_inclusion with least
element, {e} , and greatest_element, G. The meet of two normal subgroups, N and
M, in this lattice is their intersection and the join is their product.
The lattice is complete and modular.[17]
***** Normal subgroups, quotient groups and homomorphisms[edit] *****
If N is a normal subgroup, we can define a multiplication on cosets as follows:
         (  a  1   N ) (  a  2   N ) := (  a  1    a  2   ) N .
      {\displaystyle (a_{1}N)(a_{2}N):=(a_{1}a_{2})N.}  [{\displaystyle (a_
      {1}N)(a_{2}N):=(a_{1}a_{2})N.}]
With this operation, the set of cosets is itself a group, called the quotient
group and denoted G/N. There is a natural homomorphism, f: G â G/N given by f
(a) = aN. The image f(N) consists only of the identity element of G/N, the
coset eN = N.[20]
In general, a group homomorphism, f: G â H sends subgroups of G to subgroups
of H. Also, the preimage of any subgroup of H is a subgroup of G. We call the
preimage of the trivial group {e}  in H the kernel of the homomorphism and
denote it by ker(f). As it turns out, the kernel is always normal and the image
of G, f(G), is always isomorphic to G/ker(f) (the first_isomorphism_theorem).
[21] In fact, this correspondence is a bijection between the set of all
quotient groups of G, G/N, and the set of all homomorphic images of G (up_to
isomorphism).[22] It is also easy to see that the kernel of the quotient map,
f: G â G/N, is N itself, so the normal subgroups are precisely the kernels of
homomorphisms with domain G.[23]
***** See also[edit] *****
**** Operations taking subgroups to subgroups[edit] ****
    * Normalizer
    * Conjugate_closure
    * Normal_core
**** Subgroup properties complementary (or opposite) to normality[edit] ****
    * Malnormal_subgroup
    * Contranormal_subgroup
    * Abnormal_subgroup
    * Self-normalizing_subgroup
**** Subgroup properties stronger than normality[edit] ****
    * Characteristic_subgroup
    * Fully_characteristic_subgroup
**** Subgroup properties weaker than normality[edit] ****
    * Subnormal_subgroup
    * Ascendant_subgroup
    * Descendant_subgroup
    * Quasinormal_subgroup
    * Seminormal_subgroup
    * Conjugate_permutable_subgroup
    * Modular_subgroup
    * Pronormal_subgroup
    * Paranormal_subgroup
    * Polynormal_subgroup
    * C-normal_subgroup
**** Related notions in algebra[edit] ****
    * Ideal_(ring_theory)
***** Notes[edit] *****
   1. ^ a b c Cantrell_2000, p. 160.
   2. ^ Dummit_&_Foote_2004.
   3. ^ a b c d Hungerford_2003, p. 41.
   4. ^ Fraleigh_2003, p. 141.
   5. ^ Robinson_1996, p. 16.
   6. ^ Thurston_1997, p. 218.
   7. ^ Hall_1999, p. 190.
   8. ^ Hungerford_2003, p. 45.
   9. ^ Hall_1999, p. 138.
  10. ^ Hall_1999, p. 32.
  11. ^ Bergvall_et_al._2010, p. 96.
  12. ^ Hungerford_2003, p. 42.
  13. ^ Robinson_1996, p. 17.
  14. ^ Robinson_1996, p. 28.
  15. ^ Robinson_1996, p. 402.
  16. ^ a b Hall_1999, p. 29.
  17. ^ a b Hungerford_2003, p. 46.
  18. ^ Robinson_1996, p. 36.
  19. ^ DÃµmÃµsi_&_Nehaniv_2004, p. 7.
  20. ^ Hungerford_2003, pp. 42â43.
  21. ^ Hungerford_2003, p. 44.
  22. ^ Robinson_1996, p. 20.
  23. ^ Hall_1999, p. 27.
***** References[edit] *****
    * Bergvall, Olof; Hynning, Elin; Hedberg, Mikael; Mickelin, Joel; Masawe,
      Patrick (16 May 2010). "On_Rubik's_Cube" (PDF). KTH.
Cantrell, C.D. (2000). Modern Mathematical Methods for Physicists and
Engineers. Cambridge University Press. ISBN 978-0-521-59180-5.
DÃµmÃµsi, PÃ¡l; Nehaniv, Chrystopher L. (2004). Algebraic Theory of Automata
Networks. SIAM Monographs on Discrete Mathematics and Applications. SIAM.
Dummit, David S.; Foote, Richard M. (2004). Abstract Algebra (3rd ed.). John
Wiley & Sons. ISBN 0-471-43334-9.
Fraleigh, John B. (2003). A First Course in Abstract Algebra (7th ed.).
Addison-Wesley. ISBN 978-0-321-15608-2.
Hall, Marshall (1999). The Theory of Groups. Providence: Chelsea Publishing.
ISBN 978-0-8218-1967-8.
Hungerford, Thomas (2003). Algebra. Graduate Texts in Mathematics. Springer.
Robinson, Derek J. S. (1996). A Course in the Theory of Groups. Graduate Texts
in Mathematics. 80 (2nd ed.). Springer-Verlag. ISBN 978-1-4612-6443-9.
Zbl 0836.20001.
Thurston,_William (1997). Levy, Silvio (ed.). Three-dimensional geometry and
topology, Vol. 1. Princeton Mathematical Series. Princeton University Press.
ISBN 978-0-691-08304-9.
***** Further reading[edit] *****
    * I._N._Herstein, Topics in algebra. Second edition. Xerox College
      Publishing, Lexington, Mass.-Toronto, Ont., 1975. xi+388 pp.
***** External links[edit] *****
    * Weisstein,_Eric_W. "normal_subgroup". MathWorld.
Normal_subgroup_in_Springer's_Encyclopedia_of_Mathematics
Robert_Ash:_Group_Fundamentals_in_Abstract_Algebra._The_Basic_Graduate_Year
Timothy_Gowers,_Normal_subgroups_and_quotient_groups
John_Baez,_What's_a_Normal_Subgroup?

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Normal_subgroup&oldid=900129185"
Categories:
    * Subgroup_properties
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_March_2019
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * à´®à´²à´¯à´¾à´³à´
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 3 June 2019, at 16:39 (UTC).
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
