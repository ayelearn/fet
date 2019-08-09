The following text has been accessed from https://en.wikipedia.org/wiki/Permutation_group at Fri Aug 9 02:39:13 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Permutation group ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Algebraic_structure â Group theory
Group_theory
[Cyclic_group.svg]
Basic notions
    * Subgroup
    * Normal_subgroup
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
In mathematics, a permutation group is a group G whose elements are
permutations of a given set M and whose group_operation is the composition of
permutations in G (which are thought of as bijective_functions from the set M
to itself). The group of all permutations of a set M is the symmetric_group of
M, often written as Sym(M).[1] The term permutation group thus means a subgroup
of the symmetric group. If M = {1,2,...,n} then, Sym(M), the symmetric group on
n letters is usually denoted by Sn.
By Cayley's_theorem, every group is isomorphic to some permutation group.
The way in which the elements of a permutation group permute the elements of
the set is called its group_action. Group actions have applications in the
study of symmetries, combinatorics and many other branches of mathematics,
physics and chemistry.
The popular puzzle Rubik's_cube invented in 1974 by ErnÅ_Rubik has been used
as an illustration of permutation groups. Each rotation of a layer of the cube
results in a permutation of the surface colors and is a member of the group.
The permutation group of the cube is called the Rubik's_cube_group.
⁰
***** Contents *****
    * 1_Basic_properties_and_terminology
    * 2_Notation
    * 3_Composition_of_permutations–the_group_product
    * 4_Neutral_element_and_inverses
    * 5_Examples
    * 6_Group_actions
    * 7_Cayley's_theorem
    * 8_Permutation_isomorphic_groups
    * 9_History
    * 10_See_also
    * 11_Notes
    * 12_References
    * 13_Further_reading
    * 14_External_links
***** Basic properties and terminology[edit] *****
Being a subgroup of a symmetric group, all that is necessary for a set of
permutations to satisfy the group axioms and be a permutation group is that it
contain the identity permutation, the inverse permutation of each permutation
it contains, and be closed under composition of its permutations.[2] A general
property of finite groups implies that a finite nonempty subset of a symmetric
group is again a group if and only if it is closed under the group operation.
[3]
The degree of a group of permutations of a finite_set is the number_of_elements
in the set. The order of a group (of any type) is the number of elements
(cardinality) in the group. By Lagrange's_theorem, the order of any finite
permutation group of degree n must divide n! (n-factorial, the order of the
symmetric group Sn).
***** Notation[edit] *****
Main article: Permutation_Â§ Definition_and_usage
Since permutations are bijections of a set, they can be represented by Cauchy's
two-line notation.[4] This notation lists each of the elements of M in the
first row, and for each element, its image under the permutation below it in
the second row. If     &#x03C3;   {\displaystyle \sigma }  [\sigma ] is a
permutation of the set     M = {  x  1   ,  x  2   , &#x2026; ,  x  n   }
{\displaystyle M=\{x_{1},x_{2},\ldots ,x_{n}\}}  [M=\{x_{1},x_{2},\ldots ,x_
{n}\}] then,
         &#x03C3; =   (     x  1      x  2      x  3     &#x22EF;    x  n
      &#x03C3; (  x  1   )   &#x03C3; (  x  2   )   &#x03C3; (  x  3   )
      &#x22EF;   &#x03C3; (  x  n   )    )   .   {\displaystyle \sigma ={\begin
      {pmatrix}x_{1}&x_{2}&x_{3}&\cdots &x_{n}\\\sigma (x_{1})&\sigma (x_
      {2})&\sigma (x_{3})&\cdots &\sigma (x_{n})\end{pmatrix}}.}  [\sigma =
      {\begin{pmatrix}x_{1}&x_{2}&x_{3}&\cdots &x_{n}\\\sigma (x_{1})&\sigma
      (x_{2})&\sigma (x_{3})&\cdots &\sigma (x_{n})\end{pmatrix}}.]
For instance, a particular permutation of the set {1,2,3,4,5} can be written
as:
         &#x03C3; =   (    1   2   3   4   5     2   5   4   3   1    )   ;
      {\displaystyle \sigma ={\begin{pmatrix}1&2&3&4&5\\2&5&4&3&1\end
      {pmatrix}};}  [\sigma ={\begin{pmatrix}1&2&3&4&5\\2&5&4&3&1\end
      {pmatrix}};]
this means that Ï satisfies Ï(1)=2, Ï(2)=5, Ï(3)=4, Ï(4)=3, and Ï(5)=1.
The elements of M need not appear in any special order in the first row. This
permutation could also be written as:
         &#x03C3; =   (    3   2   5   1   4     4   5   1   2   3    )   .
      {\displaystyle \sigma ={\begin{pmatrix}3&2&5&1&4\\4&5&1&2&3\end
      {pmatrix}}.}  [\sigma ={\begin{pmatrix}3&2&5&1&4\\4&5&1&2&3\end
      {pmatrix}}.]
Permutations are also often written in cyclic_notation (cyclic form)[5] so that
given the set M = {1,2,3,4}, a permutation g of M with g(1) = 2, g(2) = 4, g(4)
= 1 and g(3) = 3 will be written as (1,2,4)(3), or more commonly, (1,2,4) since
3 is left unchanged; if the objects are denoted by single letters or digits,
commas and spaces can also be dispensed with, and we have a notation such as
(124). The permutation written above in 2-line notation would be written in
cyclic notation as     &#x03C3; = ( 125 ) ( 34 ) .   {\displaystyle \sigma =
(125)(34).}  [\sigma =(125)(34).]
***** Composition of permutations–the group product[edit] *****
Main article: Permutation_Â§ Permutations_in_group_theory
The product of two permutations is defined as their composition as functions,
so     &#x03C3; &#x22C5; &#x03C0;   {\displaystyle \sigma \cdot \pi }  [
{\displaystyle \sigma \cdot \pi }] is the function that maps any element x of
the set to     &#x03C3; ( &#x03C0; ( x ) )   {\displaystyle \sigma (\pi (x))}
[{\displaystyle \sigma (\pi (x))}]. Note that the rightmost permutation is
applied to the argument first,[6][7] because of the way function application is
written. Some authors prefer the leftmost factor acting first, [8] [9] [10] but
to that end permutations must be written to the right of their argument, often
as a superscript, so the permutation     &#x03C3;   {\displaystyle \sigma }
[\sigma ] acting on the element     x   {\displaystyle x}  [x] results in the
image      x  &#x03C3;     {\displaystyle x^{\sigma }}  [{\displaystyle x^
{\sigma }}]. With this convention, the product is given by      x  &#x03C3;
&#x22C5; &#x03C0;   = (  x  &#x03C3;    )  &#x03C0;     {\displaystyle x^
{\sigma \cdot \pi }=(x^{\sigma })^{\pi }}  [{\displaystyle x^{\sigma \cdot \pi
}=(x^{\sigma })^{\pi }}]. However, this gives a different rule for multiplying
permutations. This convention is commonly used in the permutation group
literature, but this article uses the convention where the rightmost
permutation is applied first.
Since the composition of two bijections always gives another bijection, the
product of two permutations is again a permutation. In two-line notation, the
product of two permutations is obtained by rearranging the columns of the
second (leftmost) permutation so that its first row is identical with the
second row of the first (rightmost) permutation. The product can then be
written as the first row of the first permutation over the second row of the
modified second permutation. For example, given the permutations,
         P =   (    1   2   3   4   5     2   4   1   3   5    )
      &#xA0;and&#xA0;   Q =   (    1   2   3   4   5     5   4   3   2   1    )
      ,   {\displaystyle P={\begin{pmatrix}1&2&3&4&5\\2&4&1&3&5\end
      {pmatrix}}\quad {\text{ and }}\quad Q={\begin
      {pmatrix}1&2&3&4&5\\5&4&3&2&1\end{pmatrix}},}  [P={\begin
      {pmatrix}1&2&3&4&5\\2&4&1&3&5\end{pmatrix}}\quad {\text{  and  }}\quad Q=
      {\begin{pmatrix}1&2&3&4&5\\5&4&3&2&1\end{pmatrix}},]
the product QP is:
         Q P =   (    1   2   3   4   5     5   4   3   2   1    )     (    1
      2   3   4   5     2   4   1   3   5    )   =   (    2   4   1   3   5
      4   2   5   3   1    )     (    1   2   3   4   5     2   4   1   3   5
      )   =   (    1   2   3   4   5     4   2   5   3   1    )   .
      {\displaystyle QP={\begin{pmatrix}1&2&3&4&5\\5&4&3&2&1\end{pmatrix}}
      {\begin{pmatrix}1&2&3&4&5\\2&4&1&3&5\end{pmatrix}}={\begin
      {pmatrix}2&4&1&3&5\\4&2&5&3&1\end{pmatrix}}{\begin
      {pmatrix}1&2&3&4&5\\2&4&1&3&5\end{pmatrix}}={\begin
      {pmatrix}1&2&3&4&5\\4&2&5&3&1\end{pmatrix}}.}  [QP={\begin
      {pmatrix}1&2&3&4&5\\5&4&3&2&1\end{pmatrix}}{\begin
      {pmatrix}1&2&3&4&5\\2&4&1&3&5\end{pmatrix}}={\begin
      {pmatrix}2&4&1&3&5\\4&2&5&3&1\end{pmatrix}}{\begin
      {pmatrix}1&2&3&4&5\\2&4&1&3&5\end{pmatrix}}={\begin
      {pmatrix}1&2&3&4&5\\4&2&5&3&1\end{pmatrix}}.]
The composition of permutations, when they are written in cyclic form, is
obtained by juxtaposing the two permutations (with the second one written on
the left) and then simplifying to a disjoint cycle form if desired. Thus, in
cyclic notation the above product would be given by:
         Q &#x22C5; P = ( 15 ) ( 24 ) &#x22C5; ( 1243 ) = ( 1435 ) .
      {\displaystyle Q\cdot P=(15)(24)\cdot (1243)=(1435).}  [Q\cdot P=(15)
      (24)\cdot (1243)=(1435).]
Since function_composition is associative, so is the product operation on
permutations:     ( &#x03C3; &#x22C5; &#x03C0; ) &#x22C5; &#x03C1; = &#x03C3;
&#x22C5; ( &#x03C0; &#x22C5; &#x03C1; )   {\displaystyle (\sigma \cdot \pi
)\cdot \rho =\sigma \cdot (\pi \cdot \rho )}  [{\displaystyle (\sigma \cdot \pi
)\cdot \rho =\sigma \cdot (\pi \cdot \rho )}]. Therefore, products of two or
more permutations are usually written without adding parentheses to express
grouping; they are also usually written without a dot or other sign to indicate
multiplication (the dots of the previous example were added for emphasis, so
would simply be written as     &#x03C3; &#x03C0; &#x03C1;   {\displaystyle
\sigma \pi \rho }  [{\displaystyle \sigma \pi \rho }]).
***** Neutral element and inverses[edit] *****
The identity permutation, which maps every element of the set to itself, is the
neutral element for this product. In two-line notation, the identity is
           (    1   2   3   &#x22EF;   n     1   2   3   &#x22EF;   n    )   .
      {\displaystyle {\begin{pmatrix}1&2&3&\cdots &n\\1&2&3&\cdots &n\end
      {pmatrix}}.}  [{\begin{pmatrix}1&2&3&\cdots &n\\1&2&3&\cdots &n\end
      {pmatrix}}.]
In cyclic notation, e = (1)(2)(3)...(n) which by convention is also denoted by
just (1) or even ().[11]
Since bijections have inverses, so do permutations, and the inverse Ïâ1 of
Ï is again a permutation. Explicitly, whenever Ï(x)=y one also has Ïâ1
(y)=x. In two-line notation the inverse can be obtained by interchanging the
two lines (and sorting the columns if one wishes the first line to be in a
given order). For instance
            (    1   2   3   4   5     2   5   4   3   1    )    &#x2212; 1   =
      (    2   5   4   3   1     1   2   3   4   5    )   =   (    1   2   3
      4   5     5   1   4   3   2    )   .   {\displaystyle {\begin
      {pmatrix}1&2&3&4&5\\2&5&4&3&1\end{pmatrix}}^{-1}={\begin
      {pmatrix}2&5&4&3&1\\1&2&3&4&5\end{pmatrix}}={\begin
      {pmatrix}1&2&3&4&5\\5&1&4&3&2\end{pmatrix}}.}  [{\begin
      {pmatrix}1&2&3&4&5\\2&5&4&3&1\end{pmatrix}}^{-1}={\begin
      {pmatrix}2&5&4&3&1\\1&2&3&4&5\end{pmatrix}}={\begin
      {pmatrix}1&2&3&4&5\\5&1&4&3&2\end{pmatrix}}.]
To obtain the inverse of a single cycle, we reverse the order of its elements.
Thus,
         ( 125  )  &#x2212; 1   = ( 521 ) = ( 152 ) .   {\displaystyle (125)^{-
      1}=(521)=(152).}  [(125)^{-1}=(521)=(152).]
To obtain the inverse of a product of cycles, we first reverse the order of the
cycles, and then we take the inverse of each as above. Thus,
         [ ( 125 ) ( 34 )  ]  &#x2212; 1   = ( 34  )  &#x2212; 1   ( 125  )
      &#x2212; 1   = ( 43 ) ( 521 ) = ( 34 ) ( 152 ) .   {\displaystyle [(125)
      (34)]^{-1}=(34)^{-1}(125)^{-1}=(43)(521)=(34)(152).}  [[(125)(34)]^{-1}=
      (34)^{-1}(125)^{-1}=(43)(521)=(34)(152).]
Having an associative product, an identity element, and inverses for all its
elements, makes the set of all permutations of M into a group, Sym(M); a
permutation group.
***** Examples[edit] *****
Consider the following set G1 of permutations of the set M = {1,2,3,4}:
    * e = (1)(2)(3)(4)= (1)
          o This is the identity, the trivial permutation which fixes each
            element.
    * a = (1 2)(3)(4) = (1 2)
          o This permutation interchanges 1 and 2, and fixes 3 and 4.
    * b = (1)(2)(3 4) = (3 4)
          o Like the previous one, but exchanging 3 and 4, and fixing the
            others.
    * ab = (1 2)(3 4)
          o This permutation, which is the composition of the previous two,
            exchanges simultaneously 1 with 2, and 3 with 4.
G1 forms a group, since aa = bb = e, ba = ab, and abab = e. This permutation
group is isomorphic, as an abstract group, to the Klein_group V4.
As another example consider the group_of_symmetries_of_a_square. Let the
vertices of a square be labeled 1, 2, 3 and 4 (counterclockwise around the
square starting with 1 in the top left corner). The symmetries are determined
by the images of the vertices, that can, in turn, be described by permutations.
The rotation by 90Â° (counterclockwise) about the center of the square is
described by the permutation (1234). The 180Â° and 270Â° rotations are given by
(13)(24) and (1432), respectively. The reflection about the horizontal line
through the center is given by (12)(34) and the corresponding vertical line
reflection is (14)(23). The reflection about the 1,3âdiagonal line is (24)
and reflection about the 2,4âdiagonal is (13). The only remaining symmetry is
the identity (1)(2)(3)(4). This permutation group is abstractly known as the
dihedral_group of order 8.
***** Group actions[edit] *****
Main article: Group_action_(mathematics)
In the above example of the symmetry group of a square, the permutations
"describe" the movement of the vertices of the square induced by the group of
symmetries. It is common to say that these group elements are "acting" on the
set of vertices of the square. This idea can be made precise by formally
defining a group action.[12]
Let G be a group and M a nonempty set. An action of G on M is a function f: G
Ã M â M such that
    * f(1, x) = x, for all x in M (1 is the identity (neutral) element of the
      group G), and
    * f(g, f(h, x)) = f(gh, x), for all g,h in G and all x in M.
This last condition can also be expressed as saying that the action induces a
group homomorphism from G into Sym(M).[12] Any such homomorphism is called a
(permutation) representation of G on M.
For any permutation group, the action that sends (g, x) â g(x) is called the
natural action of G on M. This is the action that is assumed unless otherwise
indicated.[12] In the example of the symmetry group of the square, the group's
action on the set of vertices is the natural action. However, this group also
induces an action on the set of four triangles in the square, which are: t1 =
234, t2 = 134, t3 = 124 and t4 = 123. It also acts on the two diagonals: d1 =
13 and d2 = 24.
Group element Action on triangles Action on diagonals
(1)           (1)                 (1)
(1234)        (t1 t2 t3 t4)       (d1 d2)
(13)(24)      (t1 t3)(t2 t4)      (1)
(1432)        (t1 t4 t3 t2)       (d1 d2)
(12)(34)      (t1 t2)(t3 t4)      (d1 d2)
(14)(23)      (t1 t4)(t2 t3)      (d1 d2)
(13)          (t1 t3)             (1)
(24)          (t2 t4)             (1)
***** Cayley's theorem[edit] *****
Main article: Cayley's_theorem
Any group G can act on itself (the elements of the group being thought of as
the set M) in many ways. In particular, there is a regular_action given by
(left) multiplication in the group. That is, f(g, x) = gx for all g and x in G.
For each fixed g, the function fg(x) = gx is a bijection on G and therefore a
permutation of the "set" G. Each element of G can be thought of as a
permutation in this way and so, G is isomorphic to a permutation group; this is
the content of Cayley's_theorem.
Consider the group G1 acting on the set {1,2,3,4} given above. Let the elements
of this group be denoted by e, a, b and c = ab = ba. The action of G1 on itself
described in Cayley's theorem gives the following permutation representation:
      fe â¦ (e)(a)(b)(c)
      fa â¦ (ea)(bc)
      fb â¦ (eb)(ac)
      fc â¦ (ec)(ab).
***** Permutation isomorphic groups[edit] *****
If G and H are two permutation groups on sets X and Y with actions f1 and f2
respectively, then we say that G and H are permutation isomorphic (isomorphic
as permutation groups) if there exists a bijective_map Î» : X â Y and a group
isomorphism Ï : G â H such that:[13]
      Î»(f1(g, x)) = f2(Ï(g), Î»(x)) for all g in G and x in X.
If X = Y this is equivalent to G and H being conjugate as subgroups of Sym(X).
[14] The special case where G = H and Ï is the identity_map gives rise to the
concept of equivalent actions of a group.[15]
In the example of the symmetries of a square given above, the natural action on
the set {1,2,3,4} is equivalent to the action on the triangles. The bijection
Î» between the sets is given by i â¦ ti. The natural action of group G1 above
and its action on itself (via left multiplication) are not equivalent as the
natural action has fixed points and the second action does not.
***** History[edit] *****
Main article: History_of_group_theory
The study of groups originally grew out of an understanding of permutation
groups.[16] Permutations had themselves been intensively studied by Lagrange in
1770 in his work on the algebraic solutions of polynomial equations. This
subject flourished and by the mid 19th century a well-developed theory of
permutation groups existed, codified by Camille_Jordan in his book TraitÃ© des
Substitutions et des Ãquations AlgÃ©briques of 1870. Jordan's book was, in
turn, based on the papers that were left by Ãvariste_Galois in 1832.
When Cayley introduced the concept of an abstract group, it was not immediately
clear whether or not this was a larger collection of objects than the known
permutation groups (which had a definition different from the modern one).
Cayley went on to prove that the two concepts were equivalent in Cayley's
theorem.[17]
Another classical text containing several chapters on permutation groups is
Burnside's Theory of Groups of Finite Order of 1911.[18] The first half of the
twentieth century was a fallow period in the study of group theory in general,
but interest in permutation groups was revived in the 1950s by H._Wielandt
whose German lecture notes were reprinted as Finite Permutation Groups in 1964.
[19]
***** See also[edit] *****
    * Rank_3_permutation_group
    * Primitive_group
    * Oligomorphic_group
***** Notes[edit] *****
   1. ^ The notations SM and SM are also used.
   2. ^ Rotman_2006, p. 148, Definition of subgroup
   3. ^ Rotman_2006, p. 149, Proposition 2.69
   4. ^Wussing, Hans (2007), The_Genesis_of_the_Abstract_Group_Concept:_A
      Contribution_to_the_History_of_the_Origin_of_Abstract_Group_Theory,
      Courier Dover Publications, p. 94, ISBN 9780486458687, Cauchy used his
      permutation notationâin which the arrangements are written one below
      the other and both are enclosed in parenthesesâfor the first time in
      1815.
   5. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   6. ^ especially when the algebraic properties of the permutation are of
      interest.
   7. ^ Biggs, Norman L.; White, A. T. (1979). Permutation groups and
      combinatorial structures. Cambridge University Press. ISBN 0-521-22287-7.
   8. ^ Rotman_2006, p. 107 – note especially the footnote on this page.
   9. ^  Dixon_&_Mortimer_1996, p. 3 – see the comment following Example 1.2.2
  10. ^ Cameron, Peter J. (1999). Permutation groups. Cambridge University
      Press. ISBN 0-521-65302-9.
  11. ^ Jerrum, M. (1986). "A compact representation of permutation groups". J.
      Algorithms. 7 (1): 60â78. doi:10.1016/0196-6774(86)90038-6.
  12. ^ Rotman_2006, p. 108
  13. ^ a b c Dixon_&_Mortimer_1996, p. 5
  14. ^ Dixon_&_Mortimer_1996, p. 17
  15. ^ Dixon_&_Mortimer_1996, p. 18
  16. ^ Cameron_1994, p. 228
  17. ^ Dixon_&_Mortimer_1996, p. 28
  18. ^ Cameron_1994, p. 226
  19. ^Burnside, William (1955) [1911], Theory of Groups of Finite Order (2nd
      ed.), Dover
  20. ^Wielandt, H. (1964), Finite Permutation Groups, Academic Press
***** References[edit] *****
    * Cameron, Peter J. (1994), Combinatorics: Topics, Techniques, Algorithms,
      Cambridge University Press, ISBN 0-521-45761-0
Dixon, John D.; Mortimer, Brian (1996), Permutation Groups, Graduate Texts in
Mathematics 163), Springer-Verlag, ISBN 0-387-94599-7
Rotman, Joseph J. (2006), A First Course in Abstract Algebra with Applications
(3rd ed.), Pearson Prentice-Hall, ISBN 0-13-186267-7
***** Further reading[edit] *****
    * Akos Seress. Permutation group algorithms. Cambridge Tracts in
      Mathematics, 152. Cambridge University Press, Cambridge, 2003.
    * Meenaxi Bhattacharjee, Dugald Macpherson, RÃ¶gnvaldur G. MÃ¶ller and
      Peter M. Neumann. Notes on Infinite Permutation Groups. Number 1698 in
      Lecture Notes in Mathematics. Springer-Verlag, 1998.
    * Peter_J._Cameron. Permutation Groups. LMS Student Text 45. Cambridge
      University Press, Cambridge, 1999.
    * Peter J. Cameron. Oligomorphic Permutation Groups. Cambridge University
      Press, Cambridge, 1990.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Permutation_group", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Alexander Hulpke. GAP Data Library "Transitive_Permutation_Groups".

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Permutation_group&oldid=909023014"
Categories:
    * Permutation_groups
    * Finite_groups
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
    * Wikibooks
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * CatalÃ 
    * Dansk
    * Deutsch
    * FranÃ§ais
    * Bahasa_Indonesia
    * Nederlands
    * Polski
    * PortuguÃªs
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 2 August 2019, at 14:57 (UTC).
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
