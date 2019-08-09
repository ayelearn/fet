The following text has been accessed from https://en.wikipedia.org/wiki/Matrix_ring at Fri Aug 9 03:17:49 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Matrix ring ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Matrix algebra" redirects here. For the algebraic theory of matrices, see
Matrix_(mathematics) and Linear_algebra.
In abstract_algebra, a matrix ring is any collection of matrices over some ring
R that form a ring under matrix_addition and matrix_multiplication (Lam_1999).
The set of n Ã n matrices with entries from R is a matrix ring denoted Mn(R),
as well as some subsets of infinite matrices which form infinite matrix rings.
Any subring of a matrix ring is a matrix ring.
When R is a commutative ring, the matrix ring Mn(R) is an associative_algebra,
and may be called a matrix algebra. For this case, if M is a matrix and r is in
R, then the matrix Mr is the matrix M with each of its entries multiplied by r.
This article assumes that R is an associative_ring with a unit 1 â  0,
although matrix rings can be formed over rings without unity.
⁰
***** Contents *****
    * 1_Examples
    * 2_Structure
    * 3_Properties
    * 4_Diagonal_subring
          o 4.1_Two_dimensional_diagonal_subrings
    * 5_Matrix_semiring
    * 6_See_also
    * 7_References
***** Examples[edit] *****
    * The set of all n Ã n matrices over an arbitrary ring R, denoted Mn(R).
      This is usually referred to as the "full ring of n-by-n matrices". These
      matrices represent endomorphisms of the free module Rn.
    * The set of all upper (or set of all lower) triangular_matrices over a
      ring.
    * If R is any ring with unity, then the ring of endomorphisms of     M =
      &#x2A01;  i &#x2208; I   R   {\displaystyle M=\bigoplus _{i\in I}R}
      [M=\bigoplus _{i\in I}R] as a right R-module is isomorphic to the ring of
      column finite matrices       C F M   I   ( R )    {\displaystyle \mathbb
      {CFM} _{I}(R)\,}  [\mathbb{CFM}_I(R)\,] whose entries are indexed by I Ã
      I, and whose columns each contain only finitely many nonzero entries. The
      endomorphisms of M considered as a left R module result in an analogous
      object, the row finite matrices       R F M   I   ( R )   {\displaystyle
      \mathbb {RFM} _{I}(R)}  [\mathbb {RFM} _{I}(R)] whose rows each only have
      finitely many nonzero entries.
    * If R is a Banach_algebra, then the condition of row or column finiteness
      in the previous point can be relaxed. With the norm in place, absolutely
      convergent_series can be used instead of finite sums. For example, the
      matrices whose column sums are absolutely convergent sequences form a
      ring. Analogously of course, the matrices whose row sums are absolutely
      convergent series also form a ring. This idea can be used to represent
      operators_on_Hilbert_spaces, for example.
    * The intersection of the row and column finite matrix rings also forms a
      ring, which can be denoted by       R C F M   I   ( R )   {\displaystyle
      \mathbb {RCFM} _{I}(R)}  [{\mathbb  {RCFM}}_{I}(R)].
    * The algebra M2(R) of 2_Ã_2_real_matrices, which is isomorphic to the
      split-quaternions, is a simple example of a non-commutative associative
      algebra. Like the quaternions, it has dimension 4 over R, but unlike the
      quaternions, it has zero_divisors, as can be seen from the following
      product of the matrix_units: E11E21 = 0, hence it is not a division_ring.
      Its invertible elements are nonsingular_matrices and they form a group,
      the general_linear_group GL(2, R).
    * If R is commutative, the matrix ring has a structure of a *-algebra over
      R, where the involution * on Mn(R) is the matrix_transposition.
    * If A is a C*-algebra, then Mn(A) consists of n-by-n matrices with entries
      from the C*-algebra A, which is itself a C*-algebra. If A is non-unital,
      then Mn(A) is also non-unital. Viewing A as a norm-closed subalgebra of
      the continuous operators B(H) for some Hilbert space H (that there exists
      such a Hilbert space and isometric *-isomorphism is the content of the
      Gelfand-Naimark_theorem), we can identify Mn(A) with a subalgebra of B(H
      &#x2295; n   {\displaystyle \oplus n}  [{\displaystyle \oplus n}]). For
      simplicity, if we further suppose that H is separable and A     &#x2286;
      {\displaystyle \subseteq }  [\subseteq ] B(H) is a unital C*-algebra, we
      can break up A into a matrix ring over a smaller C*-algebra. One can do
      so by fixing a projection p and hence its orthogonal projection 1 - p;
      one can identify A with       (    p A p   p A ( 1 &#x2212; p )     ( 1
      &#x2212; p ) A p   ( 1 &#x2212; p ) A ( 1 &#x2212; p )    )
      {\displaystyle {\begin{pmatrix}pAp&pA(1-p)\\(1-p)Ap&(1-p)A(1-p)\end
      {pmatrix}}}  [{\displaystyle {\begin{pmatrix}pAp&pA(1-p)\\(1-p)Ap&(1-p)A
      (1-p)\end{pmatrix}}}], where matrix multiplication works as intended
      because of the orthogonality of the projections. In order to identify A
      with a matrix ring over a C*-algebra, we require that p and 1 â p have
      the same â³rankâ³; more precisely, we need that p and 1 â p are
      Murrayâvon Neumann equivalent, i.e. there exists a partial_isometry u
      such that p = uu* and 1 â p = u*u. One can easily generalize this to
      matrices of larger sizes.
    * Complex matrix algebras Mn(C) are, up to isomorphism, the only simple
      associative algebras over the field C of complex_numbers. For n = 2, the
      matrix algebra M2(C) plays an important role in the theory of angular
      momentum. It has an alternative basis given by the identity_matrix and
      the three Pauli_matrices. M2(C) was the scene of early abstract algebra
      in the form of biquaternions.
    * A matrix ring over a field is a Frobenius_algebra, with Frobenius form
      given by the trace of the product: Ï(A, B) = tr(AB).
***** Structure[edit] *****
    * The matrix ring Mn(R) can be identified with the ring_of_endomorphisms of
      the free_R-module of rank n, Mn(R) â EndR(Rn).[clarification_needed]
      The procedure for matrix_multiplication can be traced back to
      compositions of endomorphisms in this endomorphism ring.
    * The ring Mn(D) over a division_ring D is an Artinian simple_ring, a
      special type of semisimple_ring. The rings       C F M   I   ( D )
      {\displaystyle \mathbb {CFM} _{I}(D)}  [\mathbb{CFM}_I(D)] and       R F
      M   I   ( D )   {\displaystyle \mathbb {RFM} _{I}(D)}  [\mathbb{RFM}_I
      (D)] are not simple and not Artinian if the set I is infinite, however
      they are still full_linear_rings.
    * In general, every semisimple ring is isomorphic to a finite direct
      product of full matrix rings over division rings, which may have
      differing division rings and differing sizes. This classification is
      given by the ArtinâWedderburn_theorem.
    * There is a one-to-one correspondence between the two-sided ideals of Mn
      (R) and the two-sided ideals of R. Namely, for each ideal I of R, the set
      of all n Ã n matrices with entries in I is an ideal of Mn(R), and each
      ideal of Mn(R) arises in this way. This implies that Mn(R) is simple if
      and only if R is simple. For n â¥ 2, not every left ideal or right ideal
      of Mn(R) arises by the previous construction from a left ideal or a right
      ideal in R. For example, the set of matrices whose columns with indices 2
      through n are all zero forms a left ideal in Mn(R).
    * The previous ideal correspondence actually arises from the fact that the
      rings R and Mn(R) are Morita_equivalent. Roughly speaking, this means
      that the category of left R modules and the category of left Mn(R)
      modules are very similar. Because of this, there is a natural bijective
      correspondence between the isomorphism classes of the left R-modules and
      the left Mn(R)-modules, and between the isomorphism classes of the left
      ideals of R and Mn(R). Identical statements hold for right modules and
      right ideals. Through Morita equivalence, Mn(R) can inherit any
      properties of R which are Morita invariant, such as being simple,
      Artinian, Noetherian, prime and numerous other properties as given in the
      Morita_equivalence article.
***** Properties[edit] *****
    * The matrix ring Mn(R) is commutative if and only if R is commutative and
      n = 1. In fact, this is also true for the subring of upper triangular
      matrices. Here is an example for 2Ã2 matrices (in fact, upper triangular
      matrices) which do not commute:
                 [    1   0     0   0    ]     [    1   1     0   0    ]   =
            [    1   1     0   0    ]      {\displaystyle {\begin
            {bmatrix}1&0\\0&0\end{bmatrix}}{\begin{bmatrix}1&1\\0&0\end
            {bmatrix}}={\begin{bmatrix}1&1\\0&0\end{bmatrix}}\,}  [
              \begin{bmatrix}
                1 & 0 \\
                0 & 0
              \end{bmatrix}
              \begin{bmatrix}
                1 & 1 \\
                0 & 0
              \end{bmatrix}
            =
              \begin{bmatrix}
                1 & 1 \\
                0 & 0
              \end{bmatrix}\,
            ]
and
                 [    1   1     0   0    ]     [    1   0     0   0    ]   =
            [    1   0     0   0    ]   .    {\displaystyle {\begin
            {bmatrix}1&1\\0&0\end{bmatrix}}{\begin{bmatrix}1&0\\0&0\end
            {bmatrix}}={\begin{bmatrix}1&0\\0&0\end{bmatrix}}.\,}  [
            {\displaystyle {\begin{bmatrix}1&1\\0&0\end{bmatrix}}{\begin
            {bmatrix}1&0\\0&0\end{bmatrix}}={\begin{bmatrix}1&0\\0&0\end
            {bmatrix}}.\,}]
      This example is easily generalized to nÃn matrices.
    * For n ≥ 2, the matrix ring Mn(R) has zero_divisors and nilpotent
      elements, and again, the same thing can be said for the upper triangular
      matrices. An example in 2Ã2 matrices would be
                 [    0   1     0   0    ]     [    0   1     0   0    ]   =
            [    0   0     0   0    ]      {\displaystyle {\begin
            {bmatrix}0&1\\0&0\end{bmatrix}}{\begin{bmatrix}0&1\\0&0\end
            {bmatrix}}={\begin{bmatrix}0&0\\0&0\end{bmatrix}}\,}  [  \begin
            {bmatrix}
                0 & 1 \\
                0 & 0
              \end{bmatrix}
              \begin{bmatrix}
                0 & 1 \\
                0 & 0
              \end{bmatrix}
            =
              \begin{bmatrix}
                0 & 0 \\
                0 & 0
              \end{bmatrix}\,
            ].
    * The center of a matrix ring over a ring R consists of the matrices which
      are scalar multiples of the identity_matrix, where the scalar belongs to
      the center of R.
    * In linear algebra, it is noted that over a field F, Mn(F) has the
      property that for any two matrices A and B, AB = 1 implies BA = 1. This
      is not true for every ring R though. A ring R whose matrix rings all have
      the mentioned property is known as a stably_finite_ring (Lam_1999, p. 5).
***** Diagonal subring[edit] *****
Let D be the set of diagonal_matrices in the matrix ring Mn(R), that is the set
of the matrices such that every nonzero entry, if any, is on the main diagonal.
Then D is closed under matrix_addition and matrix_multiplication, and contains
the identity_matrix, so it is a subalgebra of Mn(R).
As an algebra_over_R, D is isomorphic to the direct_product of n copies of R.
It is a free_R-module of dimension n. The idempotent_elements of D are the
diagonal matrices such that the diagonal entries are themselves idempotent.
**** Two dimensional diagonal subrings[edit] ****
When R is the field of real_numbers, then the diagonal subring of M2(R) is
isomorphic to split-complex_numbers. When R is the field of complex_numbers,
then the diagonal subring is isomorphic to bicomplex_numbers. When R = â, the
division_ring of quaternions, then the diagonal subring is isomorphic to the
ring of split-biquaternions, presented in 1873 by William_K._Clifford.
***** Matrix semiring[edit] *****
In fact, R only needs to be a semiring for Mn(R) to be defined. In this case,
Mn(R) is a semiring, called the matrix semiring. Similarly, if R is a
commutative semiring, then Mn(R) is a matrix semialgebra.
For example, if R is the Boolean_semiring (the Two-element_Boolean_algebra R = 
{0,1} with 1 + 1 = 1), then Mn(R) is the semiring of binary_relations on an n-
element set with union as addition, composition_of_relations as multiplication,
the empty_relation (zero_matrix) as the zero, and the identity_relation
(identity_matrix) as the unit.[1]
***** See also[edit] *****
    * Central_simple_algebra
    * Clifford_algebra
    * Hurwitz's_theorem_(normed_division_algebras)
    * Generic_matrix_ring
    * Sylvester's_law_of_inertia
***** References[edit] *****
   1. ^ Droste, M., & Kuich, W. (2009). Semirings and Formal Power Series.
      Handbook of Weighted Automata, 3â28. doi:10.1007/978-3-642-01492-5_1,
      pp. 7â10
    * Lam, T. Y. (1999), Lectures_on_modules_and_rings, Graduate Texts in
      Mathematics No. 189, Berlin, New York: Springer-Verlag, ISBN 978-0-387-
      98428-5

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Matrix_ring&oldid=907843948"
Categories:
    * Algebraic_structures
    * Ring_theory
    * Matrix_theory
Hidden categories:
    * Wikipedia_articles_needing_clarification_from_June_2017
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
    * ÄeÅ¡tina
    * Deutsch
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * ä¸­æ
Edit_links
    * This page was last edited on 25 July 2019, at 17:03 (UTC).
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
