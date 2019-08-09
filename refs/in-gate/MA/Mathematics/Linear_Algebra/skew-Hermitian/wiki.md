The following text has been accessed from https://en.wikipedia.org/wiki/Skew-Hermitian_matrix at Fri Aug 9 02:33:33 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Skew-Hermitian matrix ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For matrices with antisymmetry over the real_number field, see Skew-symmetric
matrix.
In linear_algebra, a square_matrix with complex entries is said to be skew-
Hermitian or antihermitian if its conjugate_transpose is the negative of the
original matrix.[1] That is, the matrix     A   {\displaystyle A}  [A] is skew-
Hermitian if it satisfies the relation
   A  &#xA0;skew-Hermitian    &#x27FA;    A   H    = &#x2212; A
{\displaystyle A{\text{ skew-Hermitian}}\quad \iff \quad A^{\mathsf {H}}=-A}  [
{\displaystyle A{\text{ skew-Hermitian}}\quad \iff \quad A^{\mathsf {H}}=-A}]
where      A   H      {\displaystyle A^{\textsf {H}}}  [{\displaystyle A^
{\textsf {H}}}] denotes the conjugate transpose of the matrix     A
{\displaystyle A}  [A]. In component form, this means that
   A  &#xA0;skew-Hermitian    &#x27FA;    a  i j   = &#x2212;    a  j i
&#x00AF;     {\displaystyle A{\text{ skew-Hermitian}}\quad \iff \quad a_{ij}=-
{\overline {a_{ji}}}}  [{\displaystyle A{\text{ skew-Hermitian}}\quad \iff
\quad a_{ij}=-{\overline {a_{ji}}}}]
for all indices     i   {\displaystyle i}  [i] and     j   {\displaystyle j}
[j], where      a  i j     {\displaystyle a_{ij}}  [a_{ij}] is the element in
the     j   {\displaystyle j}  [j]-th row and     i   {\displaystyle i}  [i]-th
column of     A   {\displaystyle A}  [A], and the overline denotes complex
conjugation.
Skew-Hermitian matrices can be understood as the complex versions of real skew-
symmetric_matrices, or as the matrix analogue of the purely imaginary numbers.
[2] The set of all skew-Hermitian     n &#x00D7; n   {\displaystyle n\times n}
[n\times n] matrices forms the     u ( n )   {\displaystyle u(n)}  [u(n)] Lie
algebra, which corresponds to the Lie group U(n). The concept can be
generalized to include linear_transformations of any complex vector_space with
a sesquilinear norm.
Note that the adjoint of an operator depends on the scalar_product considered
on the     n   {\displaystyle n}  [n] dimensional complex or real space      K
n     {\displaystyle K^{n}}  [K^{n}]. If     ( &#x22C5;  |  &#x22C5; )
{\displaystyle (\cdot |\cdot )}  [{\displaystyle (\cdot |\cdot )}] denotes the
scalar product on      K  n     {\displaystyle K^{n}}  [{\displaystyle K^{n}}],
then saying     A   {\displaystyle A}  [A] is skew-adjoint means that for all
u , v &#x2208;  K  n     {\displaystyle u,v\in K^{n}}  [{\displaystyle u,v\in
K^{n}}] one has     ( A u  |  v ) = &#x2212; ( u  |  A v )    {\displaystyle
(Au|v)=-(u|Av)\,}  [{\displaystyle (Au|v)=-(u|Av)\,}].
Imaginary_numbers can be thought of as skew-adjoint (since they are like     1
&#x00D7; 1   {\displaystyle 1\times 1}  [1 \times 1] matrices), whereas real
numbers correspond to self-adjoint operators.
***** Example[edit] *****
For example, the following matrix is skew-Hermitian
         A =   [    &#x2212; i   2 + i     &#x2212; 2 + i   0    ]
      {\displaystyle A={\begin{bmatrix}-i&2+i\\-2+i&0\end{bmatrix}}}  [
      {\displaystyle A={\begin{bmatrix}-i&2+i\\-2+i&0\end{bmatrix}}}]
because
         &#x2212; A =   [    i   &#x2212; 2 &#x2212; i     2 &#x2212; i   0
      ]   =   [       &#x2212; i  &#x00AF;        &#x2212; 2 + i  &#x00AF;
      2 + i  &#x00AF;       0 &#x00AF;      ]   =    [       &#x2212; i
      &#x00AF;        2 + i  &#x00AF;          &#x2212; 2 + i  &#x00AF;       0
      &#x00AF;      ]     T    =  A   H      {\displaystyle -A={\begin
      {bmatrix}i&-2-i\\2-i&0\end{bmatrix}}={\begin{bmatrix}{\overline {-i}}&
      {\overline {-2+i}}\\{\overline {2+i}}&{\overline {0}}\end{bmatrix}}=
      {\begin{bmatrix}{\overline {-i}}&{\overline {2+i}}\\{\overline {-2+i}}&
      {\overline {0}}\end{bmatrix}}^{\mathsf {T}}=A^{\mathsf {H}}}  [
      {\displaystyle -A={\begin{bmatrix}i&-2-i\\2-i&0\end{bmatrix}}={\begin
      {bmatrix}{\overline {-i}}&{\overline {-2+i}}\\{\overline {2+i}}&
      {\overline {0}}\end{bmatrix}}={\begin{bmatrix}{\overline {-i}}&{\overline
      {2+i}}\\{\overline {-2+i}}&{\overline {0}}\end{bmatrix}}^{\mathsf {T}}=A^
      {\mathsf {H}}}]
***** Properties[edit] *****
    * The eigenvalues of a skew-Hermitian matrix are all purely imaginary (and
      possibly zero). Furthermore, skew-Hermitian matrices are normal. Hence
      they are diagonalizable and their eigenvectors for distinct eigenvalues
      must be orthogonal.[3]
    * All entries on the main_diagonal of a skew-Hermitian matrix have to be
      pure imaginary; i.e., on the imaginary axis (the number zero is also
      considered purely imaginary).[4]
    * If     A   {\displaystyle A}  [A] and     B   {\displaystyle B}  [B] are
      skew-Hermitian, then     a A + b B   {\displaystyle aA+bB}  [
      {\displaystyle aA+bB}] is skew-Hermitian for all real scalars     a
      {\displaystyle a}  [a] and     b   {\displaystyle b}  [b].[5]
    *    A   {\displaystyle A}  [A] is skew-Hermitian if and only if     i A
      {\displaystyle iA}  [{\displaystyle iA}] (or equivalently,     &#x2212; i
      A   {\displaystyle -iA}  [{\displaystyle -iA}]) is Hermitian.[5]
    *    A   {\displaystyle A}  [A] is skew-Hermitian if and only if the real
      part     &#x211C;  ( A )    {\displaystyle \Re {(A)}}  [{\displaystyle
      \Re {(A)}}] is skew-symmetric and the imaginary part     &#x2111;  ( A )
      {\displaystyle \Im {(A)}}  [{\displaystyle \Im {(A)}}] is symmetric.
    * If     A   {\displaystyle A}  [A] is skew-Hermitian, then      A  k
      {\displaystyle A^{k}}  [A^{k}] is Hermitian if     k   {\displaystyle k}
      [k] is an even integer and skew-Hermitian if     k   {\displaystyle k}
      [k] is an odd integer.
    *    A   {\displaystyle A}  [A] is skew-Hermitian if and only if      x   H
      A y = &#x2212;  y   H    A x   {\displaystyle x^{\mathsf {H}}Ay=-y^
      {\mathsf {H}}Ax}  [{\displaystyle x^{\mathsf {H}}Ay=-y^{\mathsf {H}}Ax}]
      for all vectors     x , y   {\displaystyle x,y}  [x,y].
    * If     A   {\displaystyle A}  [A] is skew-Hermitian, then the matrix
      exponential      e  A     {\displaystyle e^{A}}  [e^{A}] is unitary.
    * The space of skew-Hermitian matrices forms the Lie_algebra     u ( n )
      {\displaystyle u(n)}  [u(n)] of the Lie_group     U ( n )
      {\displaystyle U(n)}  [{\displaystyle U(n)}].
***** Decomposition into Hermitian and skew-Hermitian[edit] *****
    * The sum of a square matrix and its conjugate transpose      (  A +  A   H
      )    {\displaystyle \left(A+A^{\mathsf {H}}\right)}  [{\displaystyle
      \left(A+A^{\mathsf {H}}\right)}] is Hermitian.
    * The difference of a square matrix and its conjugate transpose      (  A
      &#x2212;  A   H     )    {\displaystyle \left(A-A^{\mathsf {H}}\right)}
      [{\displaystyle \left(A-A^{\mathsf {H}}\right)}] is skew-Hermitian. This
      implies that commutator of two Hermitian matrices is skew-Hermitian.
    * An arbitrary square matrix     C   {\displaystyle C}  [C] can be written
      as the sum of a Hermitian matrix     A   {\displaystyle A}  [A] and a
      skew-Hermitian matrix     B   {\displaystyle B}  [B]:
               C = A + B    with    A =   1 2    (  C +  C   H     )     and
            B =   1 2    (  C &#x2212;  C   H     )    {\displaystyle
            C=A+B\quad {\mbox{with}}\quad A={\frac {1}{2}}\left(C+C^{\mathsf
            {H}}\right)\quad {\mbox{and}}\quad B={\frac {1}{2}}\left(C-C^
            {\mathsf {H}}\right)}  [{\displaystyle C=A+B\quad {\mbox
            {with}}\quad A={\frac {1}{2}}\left(C+C^{\mathsf {H}}\right)\quad
            {\mbox{and}}\quad B={\frac {1}{2}}\left(C-C^{\mathsf {H}}\right)}]
***** See also[edit] *****
    * Bivector_(complex)
    * Hermitian_matrix
    * Normal_matrix
    * Skew-symmetric_matrix
    * Unitary_matrix
***** Notes[edit] *****
   1. ^ Horn_&_Johnson_(1985), Â§4.1.1; Meyer_(2000), Â§3.2
   2. ^ Horn_&_Johnson_(1985), Â§4.1.2
   3. ^ Horn_&_Johnson_(1985), Â§2.5.2, Â§2.5.4
   4. ^ Meyer_(2000), Exercise 3.2.5
   5. ^ a b Horn_&_Johnson_(1985), Â§4.1.1
***** References[edit] *****
    * Horn, Roger A.; Johnson, Charles R. (1985), Matrix Analysis, Cambridge
      University_Press, ISBN 978-0-521-38632-6
.
Meyer, Carl D. (2000), Matrix_Analysis_and_Applied_Linear_Algebra, SIAM,
ISBN 978-0-89871-454-8
.

Retrieved from "https://en.wikipedia.org/w/index.php?title=Skew-
Hermitian_matrix&oldid=887511816"
Categories:
    * Matrices
    * Abstract_algebra
    * Linear_algebra
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
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * Italiano
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Suomi
    * à¹à¸à¸¢
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 13 March 2019, at 03:10 (UTC).
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
