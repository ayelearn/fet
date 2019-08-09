The following text has been accessed from https://en.wikipedia.org/wiki/Jordan_normal_form at Fri Aug 9 02:49:43 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Jordan normal form ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Form of a matrix indicating its eigenvalues and their algebraic multiplicities
An example of a matrix in Jordan normal form. The grey blocks are called Jordan
blocks. Note that the      &#x03BB;  i     {\displaystyle \lambda _{i}}
[\lambda _{i}] in different blocks can be equal.
In linear_algebra, a Jordan normal form, also known as a Jordan canonical form
[1] or JCF,[2] is an upper_triangular_matrix of a particular form called a
Jordan_matrix representing a linear_operator on a finite-dimensional vector
space with respect to some basis. Such a matrix has each non-zero off-diagonal
entry equal to 1, immediately above the main diagonal (on the superdiagonal),
and with identical diagonal entries to the left and below them.
Let V be a vector space over a field K. Then a basis with respect to which the
matrix has the required form exists if_and_only_if all eigenvalues of the
matrix lie in K, or equivalently if the characteristic_polynomial of the
operator splits into linear factors over K. This condition is always satisfied
if K is algebraically_closed (for instance, if it is the field of complex
numbers). The diagonal entries of the normal form are the eigenvalues (of the
operator), and the number of times each eigenvalue occurs is called the
algebraic_multiplicity of the eigenvalue.[3][4][5]
If the operator is originally given by a square_matrix M, then its Jordan
normal form is also called the Jordan normal form of M. Any square matrix has a
Jordan normal form if the field of coefficients is extended to one containing
all the eigenvalues of the matrix. In spite of its name, the normal form for a
given M is not entirely unique, as it is a block_diagonal_matrix formed of
Jordan_blocks, the order of which is not fixed; it is conventional to group
blocks for the same eigenvalue together, but no ordering is imposed among the
eigenvalues, nor among the blocks for a given eigenvalue, although the latter
could for instance be ordered by weakly decreasing size.[3][4][5]
The JordanâChevalley_decomposition is particularly simple with respect to a
basis for which the operator takes its Jordan normal form. The diagonal form
for diagonalizable matrices, for instance normal_matrices, is a special case of
the Jordan normal form.[6][7][8]
The Jordan normal form is named after Camille_Jordan, who first stated the
Jordan decomposition theorem in 1870.[9]
⁰
***** Contents *****
    * 1_Overview
          o 1.1_Notation
          o 1.2_Motivation
    * 2_Complex_matrices
          o 2.1_Example
          o 2.2_Example:_Obtaining_the_normal_form
    * 3_Generalized_eigenvectors
          o 3.1_A_proof
          o 3.2_Uniqueness
    * 4_Real_matrices
    * 5_Matrices_with_entries_in_a_field
    * 6_Consequences
          o 6.1_Spectral_mapping_theorem
          o 6.2_CayleyâHamilton_theorem
          o 6.3_Minimal_polynomial
          o 6.4_Invariant_subspace_decompositions
          o 6.5_Plane_(flat)_normal_form
    * 7_Matrix_functions
    * 8_Compact_operators
          o 8.1_Holomorphic_functional_calculus
          o 8.2_The_finite-dimensional_case
          o 8.3_Poles_of_an_operator
    * 9_Numerical_analysis
    * 10_See_also
    * 11_Notes
    * 12_References
***** Overview[edit] *****
**** Notation[edit] ****
Some textbooks have the ones on the subdiagonal, i.e., immediately below the
main diagonal instead of on the superdiagonal. The eigenvalues are still on the
main diagonal.[10][11]
**** Motivation[edit] ****
An n × n matrix A is diagonalizable if and only if the sum of the dimensions of
the eigenspaces is n. Or, equivalently, if and only if A has n linearly
independent eigenvectors. Not all matrices are diagonalizable; matrices that
are not diagonalizable are called defective matrices. Consider the following
matrix:
   A =  [         5   4   2   1     0   1   &#x2212; 1   &#x2212; 1
&#x2212; 1   &#x2212; 1   3   0     1   1   &#x2212; 1   2        ]  .
{\displaystyle A=\left[\!\!\!{\begin{array}{*{20}{r}}5&4&2&1\\[2pt]0&1&-1&-1\\
[2pt]-1&-1&3&0\\[2pt]1&1&-1&2\end{array}}\!\!\right].}  [A=\left[\!\!\!{\begin
{array}{*{20}{r}}5&4&2&1\\[2pt]0&1&-1&-1\\[2pt]-1&-1&3&0\\[2pt]1&1&-1&2\end
{array}}\!\!\right].]
Including multiplicity, the eigenvalues of A are Î» = 1, 2, 4, 4. The dimension
of the eigenspace corresponding to the eigenvalue 4 is 1 (and not 2), so A is
not diagonalizable. However, there is an invertible matrix P such that J =
PAP−1, where
         J =   [    1   0   0   0     0   2   0   0     0   0   4   1     0   0
      0   4    ]   .   {\displaystyle J={\begin{bmatrix}1&0&0&0\\[2pt]0&2&0&0\\
      [2pt]0&0&4&1\\[2pt]0&0&0&4\end{bmatrix}}.}  [J = \begin{bmatrix}
      1 & 0 & 0 & 0 \\[2pt]
      0 & 2 & 0 & 0 \\[2pt]
      0 & 0 & 4 & 1 \\[2pt]
      0 & 0 & 0 & 4 \end{bmatrix}.]
The matrix J is almost diagonal. This is the Jordan normal form of A. The
section Example below fills in the details of the computation.
***** Complex matrices[edit] *****
In general, a square complex matrix A is similar to a block_diagonal_matrix
         J =   [     J  1                &#x22F1;               J  p      ]
      {\displaystyle J={\begin{bmatrix}J_{1}&\;&\;\\\;&\ddots &\;\\\;&\;&J_
      {p}\end{bmatrix}}}  [J = \begin{bmatrix}
      J_1 & \;     & \; \\
      \;  & \ddots & \; \\
      \;  & \;     & J_p\end{bmatrix}]
where each block Ji is a square matrix of the form
          J  i   =   [     &#x03BB;  i     1               &#x03BB;  i
      &#x22F1;              &#x22F1;   1               &#x03BB;  i      ]   .
      {\displaystyle J_{i}={\begin{bmatrix}\lambda _{i}&1&\;&\;\\\;&\lambda _
      {i}&\ddots &\;\\\;&\;&\ddots &1\\\;&\;&\;&\lambda _{i}\end{bmatrix}}.}
      [J_i =
      \begin{bmatrix}
      \lambda_i & 1            & \;     & \;  \\
      \;        & \lambda_i    & \ddots & \;  \\
      \;        & \;           & \ddots & 1   \\
      \;        & \;           & \;     & \lambda_i
      \end{bmatrix}.]
So there exists an invertible matrix P such that Pâ1AP = J is such that the
only non-zero entries of J are on the diagonal and the superdiagonal. J is
called the Jordan normal form of A. Each Ji is called a Jordan_block of A. In a
given Jordan block, every entry on the superdiagonal is 1.
Assuming this result, we can deduce the following properties:
    * Counting multiplicity, the eigenvalues of J, therefore A, are the
      diagonal entries.
    * Given an eigenvalue Î»i, its geometric_multiplicity is the dimension of
      Ker(A − Î»iI), and it is the number of Jordan blocks corresponding to
      Î»i.[12]
    * The sum of the sizes of all Jordan blocks corresponding to an eigenvalue
      Î»i is its algebraic_multiplicity.[12]
    * A is diagonalizable if and only if, for every eigenvalue Î» of A, its
      geometric and algebraic multiplicities coincide.
    * The Jordan block corresponding to Î» is of the form Î» I + N, where N is
      a nilpotent_matrix defined as Nij = Î´i,j−1 (where Î´ is the Kronecker
      delta). The nilpotency of N can be exploited when calculating f(A) where
      f is a complex analytic function. For example, in principle the Jordan
      form could give a closed-form expression for the exponential exp(A).
    * The number of Jordan blocks corresponding to Î» of size at least j is dim
      Ker(A - Î»I)j - dim Ker(A - Î»I)j-1. Thus, the number of Jordan blocks of
      size exactly j is
         2 dim &#x2061; ker &#x2061; ( A &#x2212;  &#x03BB;  i   I  )  j
      &#x2212; dim &#x2061; ker &#x2061; ( A &#x2212;  &#x03BB;  i   I  )  j +
      1   &#x2212; dim &#x2061; ker &#x2061; ( A &#x2212;  &#x03BB;  i   I  )
      j &#x2212; 1     {\displaystyle 2\dim \ker(A-\lambda _{i}I)^{j}-\dim \ker
      (A-\lambda _{i}I)^{j+1}-\dim \ker(A-\lambda _{i}I)^{j-1}}  [2 \dim \ker
      (A - \lambda_i I)^j - \dim \ker (A - \lambda_i I)^{j+1} - \dim \ker (A -
      \lambda_i I)^{j-1}]
    * Given an eigenvalue Î»i, its multiplicity in the minimal polynomial is
      the size of its largest Jordan block.
**** Example[edit] ****
Consider the matrix A from the example in the previous section. The Jordan
normal form is obtained by some similarity transformation P−1AP = J, i.e.,
          A P = P J .   {\displaystyle \;AP=PJ.}  [\; AP = PJ.]
Let P have column vectors pi, i = 1, ..., 4, then
         A   [     p  1      p  2      p  3      p  4      ]   =   [     p  1
      p  2      p  3      p  4      ]     [    1   0   0   0     0   2   0   0
      0   0   4   1     0   0   0   4    ]   =   [     p  1     2  p  2     4
      p  3      p  3   + 4  p  4      ]   .   {\displaystyle A{\begin
      {bmatrix}p_{1}&p_{2}&p_{3}&p_{4}\end{bmatrix}}={\begin{bmatrix}p_{1}&p_
      {2}&p_{3}&p_{4}\end{bmatrix}}{\begin
      {bmatrix}1&0&0&0\\0&2&0&0\\0&0&4&1\\0&0&0&4\end{bmatrix}}={\begin
      {bmatrix}p_{1}&2p_{2}&4p_{3}&p_{3}+4p_{4}\end{bmatrix}}.}  [A \begin
      {bmatrix} p_1 & p_2 & p_3 & p_4 \end{bmatrix} = \begin{bmatrix} p_1 & p_2
      & p_3 & p_4 \end{bmatrix}
      \begin{bmatrix}
      1 & 0 & 0 & 0 \\
      0 & 2 & 0 & 0 \\
      0 & 0 & 4 & 1 \\
      0 & 0 & 0 & 4 \end{bmatrix} = \begin{bmatrix} p_1 & 2p_2 & 4p_3 &
      p_3+4p_4 \end{bmatrix}.]
We see that
          ( A &#x2212; 1 I )  p  1   = 0   {\displaystyle \;(A-1I)p_{1}=0}  [\;
      (A - 1 I) p_1 = 0 ]
          ( A &#x2212; 2 I )  p  2   = 0   {\displaystyle \;(A-2I)p_{2}=0}  [\;
      (A - 2 I) p_2 = 0 ]
          ( A &#x2212; 4 I )  p  3   = 0   {\displaystyle \;(A-4I)p_{3}=0}  [\;
      (A - 4 I) p_3 = 0 ]
          ( A &#x2212; 4 I )  p  4   =  p  3   .   {\displaystyle \;(A-4I)p_
      {4}=p_{3}.}  [\; (A - 4 I) p_4 = p_3. ]
For i = 1,2,3 we have      p  i   &#x2208; Ker &#x2061; ( A &#x2212;  &#x03BB;
i   I )   {\displaystyle p_{i}\in \operatorname {Ker} (A-\lambda _{i}I)}  [p_i
\in \operatorname{Ker}(A-\lambda_{i} I)], i.e., pi is an eigenvector of A
corresponding to the eigenvalue Î»i. For i=4, multiplying both sides by     ( A
&#x2212; 4 I )   {\displaystyle (A-4I)}  [(A-4I)] gives
          ( A &#x2212; 4 I  )  2    p  4   = ( A &#x2212; 4 I )  p  3   .
      {\displaystyle \;(A-4I)^{2}p_{4}=(A-4I)p_{3}.}  [\; (A-4I)^2 p_4 = (A-4I)
      p_3. ]
But     ( A &#x2212; 4 I )  p  3   = 0   {\displaystyle (A-4I)p_{3}=0}  [(A-
4I)p_3 = 0], so
          ( A &#x2212; 4 I  )  2    p  4   = 0.   {\displaystyle \;(A-4I)^{2}p_
      {4}=0.}  [\; (A-4I)^2 p_4 = 0. ]
Thus,      p  4   &#x2208; Ker &#x2061; ( A &#x2212; 4 I  )  2   .
{\displaystyle p_{4}\in \operatorname {Ker} (A-4I)^{2}.}  [p_4 \in
\operatorname{Ker}(A-4 I)^2.]
Vectors such as      p  4     {\displaystyle p_{4}}  [p_4] are called
generalized_eigenvectors of A.
**** Example: Obtaining the normal form[edit] ****
This example shows how to calculate the Jordan normal form of a given matrix.
As the next section explains, it is important to do the computation exactly
instead of rounding the results.
Consider the matrix
         A =   [    5   4   2   1     0   1   &#x2212; 1   &#x2212; 1
      &#x2212; 1   &#x2212; 1   3   0     1   1   &#x2212; 1   2    ]
      {\displaystyle A={\begin{bmatrix}5&4&2&1\\0&1&-1&-1\\-1&-1&3&0\\1&1&-
      1&2\end{bmatrix}}}  [A =
      \begin{bmatrix}
       5 &  4 &  2 &  1 \\
       0 &  1 & -1 & -1 \\
      -1 & -1 &  3 &  0 \\
       1 &  1 & -1 &  2
      \end{bmatrix}]
which is mentioned in the beginning of the article.
The characteristic_polynomial of A is
             &#x03C7; ( &#x03BB; )    = det ( &#x03BB; I &#x2212; A )       =
      &#x03BB;  4   &#x2212; 11  &#x03BB;  3   + 42  &#x03BB;  2   &#x2212; 64
      &#x03BB; + 32       = ( &#x03BB; &#x2212; 1 ) ( &#x03BB; &#x2212; 2 )
      ( &#x03BB; &#x2212; 4  )  2   .        {\displaystyle {\begin
      {aligned}\chi (\lambda )&=\det(\lambda I-A)\\&=\lambda ^{4}-11\lambda ^
      {3}+42\lambda ^{2}-64\lambda +32\\&=(\lambda -1)(\lambda -2)(\lambda -4)^
      {2}.\,\end{aligned}}}  [{\displaystyle {\begin{aligned}\chi (\lambda
      )&=\det(\lambda I-A)\\&=\lambda ^{4}-11\lambda ^{3}+42\lambda ^{2}-
      64\lambda +32\\&=(\lambda -1)(\lambda -2)(\lambda -4)^{2}.\,\end
      {aligned}}}]
This shows that the eigenvalues are 1, 2, 4 and 4, according to algebraic
multiplicity. The eigenspace corresponding to the eigenvalue 1 can be found by
solving the equation Av = Î» v. It is spanned by the column vector v = (−1, 1,
0, 0)T. Similarly, the eigenspace corresponding to the eigenvalue 2 is spanned
by w = (1, −1, 0, 1)T. Finally, the eigenspace corresponding to the eigenvalue
4 is also one-dimensional (even though this is a double eigenvalue) and is
spanned by x = (1, 0, −1, 1)T. So, the geometric_multiplicity (i.e., the
dimension of the eigenspace of the given eigenvalue) of each of the three
eigenvalues is one. Therefore, the two eigenvalues equal to 4 correspond to a
single Jordan block, and the Jordan normal form of the matrix A is the direct
sum
         J =  J  1   ( 1 ) &#x2295;  J  1   ( 2 ) &#x2295;  J  2   ( 4 ) =
      [    1   0   0   0     0   2   0   0     0   0   4   1     0   0   0   4
      ]   .   {\displaystyle J=J_{1}(1)\oplus J_{1}(2)\oplus J_{2}(4)={\begin
      {bmatrix}1&0&0&0\\0&2&0&0\\0&0&4&1\\0&0&0&4\end{bmatrix}}.}  [ J = J_1(1)
      \oplus J_1(2) \oplus J_2(4) =
      \begin{bmatrix} 1 & 0 & 0 & 0 \\ 0 & 2 & 0 & 0 \\ 0 & 0 & 4 & 1 \\ 0 & 0
      & 0 & 4 \end{bmatrix}. ]
There are three chains. Two have length one: {v} and {w}, corresponding to the
eigenvalues 1 and 2, respectively. There is one chain of length two
corresponding to the eigenvalue 4. To find this chain, calculate
         ker &#x2061;   ( A &#x2212; 4 I )   2   = span   {    [    1     0
      0     0    ]   ,   [    1     0     &#x2212; 1     1    ]    }
      {\displaystyle \ker {(A-4I)}^{2}=\operatorname {span} \,\left\{{\begin
      {bmatrix}1\\0\\0\\0\end{bmatrix}},{\begin{bmatrix}1\\0\\-1\\1\end
      {bmatrix}}\right\}}  [{\displaystyle \ker {(A-4I)}^{2}=\operatorname
      {span} \,\left\{{\begin{bmatrix}1\\0\\0\\0\end{bmatrix}},{\begin
      {bmatrix}1\\0\\-1\\1\end{bmatrix}}\right\}}]
where I is the 4 x 4 identity matrix. Pick a vector in the above span that is
not in the kernel of A − 4I, e.g., y = (1,0,0,0)T. Now, (A − 4I)y = x and
(A − 4I)x = 0, so {y, x} is a chain of length two corresponding to the
eigenvalue 4.
The transition matrix P such that P−1AP = J is formed by putting these vectors
next to each other as follows
         P =   [    v    |    w    |    x    |    y    ]   =   [    &#x2212; 1
      1   1   1     1   &#x2212; 1   0   0     0   0   &#x2212; 1   0     0   1
      1   0    ]   .   {\displaystyle P={\Big [}\,v\,{\Big |}\,w\,{\Big |}\,x\,
      {\Big |}\,y\,{\Big ]}={\begin{bmatrix}-1&1&1&1\\1&-1&0&0\\0&0&-
      1&0\\0&1&1&0\end{bmatrix}}.}  [ P = \Big[ \,v\, \Big| \,w\, \Big| \,x\,
      \Big| \,y\, \Big] =
      \begin{bmatrix}
      -1 &  1 &  1 &  1 \\
       1 & -1 &  0 &  0 \\
       0 &  0 & -1 &  0 \\
       0 &  1 &  1 &  0
      \end{bmatrix}. ]
A computation shows that the equation P−1AP = J indeed holds.
          P  &#x2212; 1   A P = J =   [    1   0   0   0     0   2   0   0
      0   0   4   1     0   0   0   4    ]   .   {\displaystyle P^{-1}AP=J=
      {\begin{bmatrix}1&0&0&0\\0&2&0&0\\0&0&4&1\\0&0&0&4\end{bmatrix}}.}  [P^{-
      1}AP=J=\begin{bmatrix}
      1 & 0 & 0 & 0 \\
      0 & 2 & 0 & 0 \\
      0 & 0 & 4 & 1 \\
      0 & 0 & 0 & 4 \end{bmatrix}.]
If we had interchanged the order in which the chain vectors appeared, that is,
changing the order of v, w and {x, y} together, the Jordan blocks would be
interchanged. However, the Jordan forms are equivalent Jordan forms.
***** Generalized eigenvectors[edit] *****
Main article: Generalized_eigenvector
Given an eigenvalue Î», its corresponding Jordan block gives rise to a Jordan
chain. The generator, or lead vector, say pr, of the chain is a generalized
eigenvector such that (A − Î» I)rpr = 0, where r is the size of the Jordan
block. The vector p1 = (A − Î» I)r−1pr is an eigenvector corresponding to Î».
In general, pi is a preimage of pi−1 under A − Î» I. So the lead vector
generates the chain via multiplication by (A − Î» I).[13][2]
Therefore, the statement that every square matrix A can be put in Jordan normal
form is equivalent to the claim that there exists a basis consisting only of
eigenvectors and generalized eigenvectors of A.
**** A proof[edit] ****
We give a proof_by_induction that any complex-valued matrix A may be put in
Jordan normal form.[citation_needed] The 1 × 1 case is trivial. Let A be an n ×
n matrix. Take any eigenvalue Î» of A. The range of A − Î» I, denoted by Ran(A
− Î» I), is an invariant_subspace of A. Also, since Î» is an eigenvalue of A,
the dimension of Ran(A − Î» I), r, is strictly less than n. Let A' denote the
restriction of A to Ran(A − Î» I), by inductive hypothesis, there exists a
basis {p1, ..., pr} such that A', expressed with respect to this basis, is in
Jordan normal form.
Next consider the kernel, that is, the subspace Ker(A − Î» I). If
          R a n  ( A &#x2212; &#x03BB; I ) &#x2229;  K e r  ( A &#x2212;
      &#x03BB; I ) = { 0 } ,   {\displaystyle \mathrm {Ran} (A-\lambda I)\cap
      \mathrm {Ker} (A-\lambda I)=\{0\},}  [\mathrm{Ran}(A - \lambda I) \cap
      \mathrm{Ker}(A - \lambda I) = \{0\},]
the desired result follows immediately from the rankânullity_theorem. This
would be the case, for example, if A was Hermitian.
Otherwise, if
         Q =  R a n  ( A &#x2212; &#x03BB; I ) &#x2229;  K e r  ( A &#x2212;
      &#x03BB; I ) &#x2260; { 0 } ,   {\displaystyle Q=\mathrm {Ran} (A-\lambda
      I)\cap \mathrm {Ker} (A-\lambda I)\neq \{0\},}  [Q = \mathrm{Ran}(A -
      \lambda I) \cap \mathrm{Ker}(A - \lambda I) \neq \{0\},]
let the dimension of Q be s â¤ r. Each vector in Q is an eigenvector of A'
corresponding to eigenvalue Î». So the Jordan form of A' must contain s Jordan
chains corresponding to s linearly independent eigenvectors. So the basis {p1,
..., pr} must contain s vectors, say {pr−s+1, ..., pr}, that are lead vectors
in these Jordan chains from the Jordan normal form of A'. We can "extend the
chains" by taking the preimages of these lead vectors. (This is the key step of
argument; in general, generalized eigenvectors need not lie in Ran(A − Î» I).)
Let qi be such that
          ( A &#x2212; &#x03BB; I )  q  i   =  p  i     &#xA0;for&#xA0;   i = r
      &#x2212; s + 1 , &#x2026; , r .   {\displaystyle \;(A-\lambda I)q_{i}=p_
      {i}{\mbox{ for }}i=r-s+1,\ldots ,r.}  [\; (A - \lambda I) q_i = p_i \mbox
      { for } i = r-s+1, \ldots, r.]
Clearly no non-trivial linear combination of the qi can lie in Ker(A − Î» I).
Furthermore, no non-trivial linear combination of the qi can be in Ran(A − Î»
I), for that would contradict the assumption that each pi is a lead vector in a
Jordan chain. The set {qi}, being preimages of the linearly independent set
{pi} under A − Î» I, is also linearly independent.
Finally, we can pick any linearly independent set {z1, ..., zt} that spans
           K e r  ( A &#x2212; &#x03BB; I )  /  Q .   {\displaystyle \;\mathrm
      {Ker} (A-\lambda I)/Q.}  [\; \mathrm{Ker}(A - \lambda I) / Q.]
By construction, the union of the three sets {p1, ..., pr}, {qr−s +1, ..., qr},
and {z1, ..., zt} is linearly independent. Each vector in the union is either
an eigenvector or a generalized eigenvector of A. Finally, by the
rankânullity theorem, the cardinality of the union is n. In other words, we
have found a basis that consists of eigenvectors and generalized eigenvectors
of A, and this shows A can be put in Jordan normal form.
**** Uniqueness[edit] ****
It can be shown that the Jordan normal form of a given matrix A is unique up to
the order of the Jordan blocks.
Knowing the algebraic and geometric multiplicities of the eigenvalues is not
sufficient to determine the Jordan normal form of A. Assuming the algebraic
multiplicity m(Î») of an eigenvalue Î» is known, the structure of the Jordan
form can be ascertained by analyzing the ranks of the powers (A − Î» I)m(Î»).
To see this, suppose an n × n matrix A has only one eigenvalue Î». So m(Î») =
n. The smallest integer k1 such that
         ( A &#x2212; &#x03BB; I  )   k  1     = 0   {\displaystyle (A-\lambda
      I)^{k_{1}}=0}  [(A - \lambda I)^{k_1} = 0]
is the size of the largest Jordan block in the Jordan form of A. (This number
k1 is also called the index of Î». See discussion in a following section.) The
rank of
         ( A &#x2212; &#x03BB; I  )   k  1   &#x2212; 1     {\displaystyle (A-
      \lambda I)^{k_{1}-1}}  [(A - \lambda I)^{k_1 - 1}]
is the number of Jordan blocks of size k1. Similarly, the rank of
         ( A &#x2212; &#x03BB; I  )   k  1   &#x2212; 2     {\displaystyle (A-
      \lambda I)^{k_{1}-2}}  [(A - \lambda I)^{k_1 - 2}]
is twice the number of Jordan blocks of size k1 plus the number of Jordan
blocks of size k1−1. The general case is similar.
This can be used to show the uniqueness of the Jordan form. Let J1 and J2 be
two Jordan normal forms of A. Then J1 and J2 are similar and have the same
spectrum, including algebraic multiplicities of the eigenvalues. The procedure
outlined in the previous paragraph can be used to determine the structure of
these matrices. Since the rank of a matrix is preserved by similarity
transformation, there is a bijection between the Jordan blocks of J1 and J2.
This proves the uniqueness part of the statement.
***** Real matrices[edit] *****
If A is a real matrix, its Jordan form can still be non-real. Instead of
representing it with complex eigenvalues and 1's on the superdiagonal, as
discussed above, there exists a real invertible matrix P such that Pâ1AP = J
is a real block_diagonal_matrix with each block being a real Jordan block.[14]
A real Jordan block is either identical to a complex Jordan block (if the
corresponding eigenvalue      &#x03BB;  i     {\displaystyle \lambda _{i}}
[\lambda _{i}] is real), or is a block matrix itself, consisting of 2×2 blocks
(for non-real eigenvalue      &#x03BB;  i   =  a  i   + i  b  i
{\displaystyle \lambda _{i}=a_{i}+ib_{i}}  [\lambda_i = a_i+ib_i] with given
algebraic multiplicity) of the form
          C  i   =   [     a  i     &#x2212;  b  i        b  i      a  i      ]
      {\displaystyle C_{i}={\begin{bmatrix}a_{i}&-b_{i}\\b_{i}&a_{i}\\\end
      {bmatrix}}}  [{\displaystyle C_{i}={\begin{bmatrix}a_{i}&-b_{i}\\b_{i}&a_
      {i}\\\end{bmatrix}}}]
and describe multiplication by      &#x03BB;  i     {\displaystyle \lambda _
{i}}  [\lambda _{i}] in the complex plane. The superdiagonal blocks are 2×2
identity matrices and hence in this representation the matrix dimensions are
larger than the complex Jordan form. The full real Jordan block is given by
          J  i   =   [     C  i     I               C  i     &#x22F1;
      &#x22F1;   I               C  i      ]   .   {\displaystyle J_{i}={\begin
      {bmatrix}C_{i}&I&\;&\;\\\;&C_{i}&\ddots &\;\\\;&\;&\ddots &I\\\;&\;&\;&C_
      {i}\\\end{bmatrix}}.}  [J_i =
      \begin{bmatrix}
      C_i    & I       & \;     & \;    \\
      \;     & C_i     & \ddots & \;    \\
      \;     & \;      & \ddots & I     \\
      \;     & \;      & \;     & C_i   \\
      \end{bmatrix}.]
This real Jordan form is a consequence of the complex Jordan form. For a real
matrix the nonreal eigenvectors and generalized eigenvectors can always be
chosen to form complex_conjugate pairs. Taking the real and imaginary part
(linear combination of the vector and its conjugate), the matrix has this form
with respect to the new basis.
***** Matrices with entries in a field[edit] *****
Jordan reduction can be extended to any square matrix M whose entries lie in a
field K. The result states that any M can be written as a sum D + N where D is
semisimple, N is nilpotent, and DN = ND. This is called the JordanâChevalley
decomposition. Whenever K contains the eigenvalues of M, in particular when K
is algebraically_closed, the normal form can be expressed explicitly as the
direct_sum of Jordan blocks.
Similar to the case when K is the complex numbers, knowing the dimensions of
the kernels of (M − Î»I)k for 1 â¤ k â¤ m, where m is the algebraic
multiplicity of the eigenvalue Î», allows one to determine the Jordan form of
M. We may view the underlying vector space V as a K[x]-module by regarding the
action of x on V as application of M and extending by K-linearity. Then the
polynomials (x − Î»)k are the elementary divisors of M, and the Jordan normal
form is concerned with representing M in terms of blocks associated to the
elementary divisors.
The proof of the Jordan normal form is usually carried out as an application to
the ring K[x] of the structure_theorem_for_finitely_generated_modules_over_a
principal_ideal_domain, of which it is a corollary.
***** Consequences[edit] *****
One can see that the Jordan normal form is essentially a classification result
for square matrices, and as such several important results from linear algebra
can be viewed as its consequences.
**** Spectral mapping theorem[edit] ****
Using the Jordan normal form, direct calculation gives a spectral mapping
theorem for the polynomial_functional_calculus: Let A be an n × n matrix with
eigenvalues Î»1, ..., Î»n, then for any polynomial p, p(A) has eigenvalues p
(Î»1), ..., p(Î»n).
**** CayleyâHamilton theorem[edit] ****
The CayleyâHamilton_theorem asserts that every matrix A satisfies its
characteristic equation: if p is the characteristic_polynomial of A, then p(A)
= 0. This can be shown via direct calculation in the Jordan form, since any
Jordan block for λ is annihilated by (X â λ)m where m is the multiplicity of
the root λ of p, the sum of the sizes of the Jordan blocks for λ, and therefore
no less than the size of the block in question. The Jordan form can be assumed
to exist over a field extending the base field of the matrix, for instance over
the splitting_field of p; this field extension does not change the matrix p(A)
in any way.
**** Minimal polynomial[edit] ****
The minimal_polynomial P of a square matrix A is the unique monic_polynomial of
least degree, m, such that P(A) = 0. Alternatively, the set of polynomials that
annihilate a given A form an ideal I in C[x], the principal_ideal_domain of
polynomials with complex coefficients. The monic element that generates I is
precisely P.
Let Î»1, ..., Î»q be the distinct eigenvalues of A, and si be the size of the
largest Jordan block corresponding to Î»i. It is clear from the Jordan normal
form that the minimal polynomial of A has degree Σsi.
While the Jordan normal form determines the minimal polynomial, the converse is
not true. This leads to the notion of elementary divisors. The elementary
divisors of a square matrix A are the characteristic polynomials of its Jordan
blocks. The factors of the minimal polynomial m are the elementary divisors of
the largest degree corresponding to distinct eigenvalues.
The degree of an elementary divisor is the size of the corresponding Jordan
block, therefore the dimension of the corresponding invariant subspace. If all
elementary divisors are linear, A is diagonalizable.
**** Invariant subspace decompositions[edit] ****
The Jordan form of a n × n matrix A is block diagonal, and therefore gives a
decomposition of the n dimensional Euclidean space into invariant_subspaces of
A. Every Jordan block Ji corresponds to an invariant subspace Xi. Symbolically,
we put
           C   n   =  &#x2A01;  i = 1   k    X  i     {\displaystyle \mathbb
      {C} ^{n}=\bigoplus _{i=1}^{k}X_{i}}  [\mathbb{C}^n = \bigoplus_{i = 1}^k
      X_i]
where each Xi is the span of the corresponding Jordan chain, and k is the
number of Jordan chains.
One can also obtain a slightly different decomposition via the Jordan form.
Given an eigenvalue Î»i, the size of its largest corresponding Jordan block si
is called the index of Î»i and denoted by Î½(Î»i). (Therefore, the degree of
the minimal polynomial is the sum of all indices.) Define a subspace Yi by
           Y  i   = Ker &#x2061; (  &#x03BB;  i   I &#x2212; A  )  &#x03BD;
      (  &#x03BB;  i   )   .   {\displaystyle \;Y_{i}=\operatorname {Ker}
      (\lambda _{i}I-A)^{\nu (\lambda _{i})}.}  [\; Y_i = \operatorname{Ker}
      (\lambda_i I - A)^{\nu(\lambda_i)}.]
This gives the decomposition
           C   n   =  &#x2A01;  i = 1   l    Y  i     {\displaystyle \mathbb
      {C} ^{n}=\bigoplus _{i=1}^{l}Y_{i}}  [\mathbb{C}^n = \bigoplus_{i = 1}^l
      Y_i]
where l is the number of distinct eigenvalues of A. Intuitively, we glob
together the Jordan block invariant subspaces corresponding to the same
eigenvalue. In the extreme case where A is a multiple of the identity matrix we
have k = n and l = 1.
The projection onto Yi and along all the other Yj ( j â  i ) is called the
spectral projection of A at Î»i and is usually denoted by P(Î»i ; A). Spectral
projections are mutually orthogonal in the sense that P(Î»i ; A) P(Î»j ; A) = 0
if i â  j. Also they commute with A and their sum is the identity matrix.
Replacing every Î»i in the Jordan matrix J by one and zeroising all other
entries gives P(Î»i ; J), moreover if U J Uâ1 is the similarity
transformation such that A = U J Uâ1 then P(Î»i ; A) = U P(Î»i ; J) Uâ1.
They are not confined to finite dimensions. See below for their application to
compact operators, and in holomorphic_functional_calculus for a more general
discussion.
Comparing the two decompositions, notice that, in general, l â¤ k. When A is
normal, the subspaces Xi's in the first decomposition are one-dimensional and
mutually orthogonal. This is the spectral_theorem for normal operators. The
second decomposition generalizes more easily for general compact operators on
Banach spaces.
It might be of interest here to note some properties of the index, Î½(Î»). More
generally, for a complex number Î», its index can be defined as the least non-
negative integer Î½(Î») such that
          K e r  ( &#x03BB; &#x2212; A  )  &#x03BD; ( &#x03BB; )   = Ker
      &#x2061; ( &#x03BB; &#x2212; A  )  m   ,  &#x2200; m &#x2265; &#x03BD;
      ( &#x03BB; ) .   {\displaystyle \mathrm {Ker} (\lambda -A)^{\nu (\lambda
      )}=\operatorname {Ker} (\lambda -A)^{m},\;\forall m\geq \nu (\lambda ).}
      [\mathrm{Ker}(\lambda - A)^{\nu(\lambda)} = \operatorname{Ker} (\lambda -
      A)^m, \; \forall m \geq \nu(\lambda) .]
So Î½(Î») > 0 if and only if Î» is an eigenvalue of A. In the finite-
dimensional case, Î½(Î») â¤ the algebraic multiplicity of Î».
**** Plane (flat) normal form[edit] ****
The Jordan form is used to find a normal form of matrices up to conjugacy such
that normal matrices make up an algebraic variety of a low fixed degree in the
ambient matrix space.
Sets of representatives of matrix conjugacy classes for Jordan normal form or
rational canonical forms in general do not constitute linear or affine
subspaces in the ambient matrix spaces.
Vladimir_Arnold posed a problem in [15] - find a canonical form of matrices
over a field for which the set of representatives of matrix conjugacy classes
is a union of affine linear subspaces (flats). In other words, map the set of
matrix conjugacy classes injectively back into the intitial set of matrices so
that the image of this embedding - the set of all normal matrices, has the
lowest possible degree â it is a union of shifted linear subspaces.
It was solved for algebraically closed fields by Peteris Daugulis [16]. The
construction of a uniquely defined plane normal form of a matrix starts by
considering its Jordan normal form.
***** Matrix functions[edit] *****
Main article: Matrix_function
Iteration of the Jordan chain motivates various extensions to more abstract
settings. For finite matrices, once gets matrix functions; this can be extended
to compact operators and the holomorphic functional calculus, as described
further below.
The Jordan normal form is the most convenient for computation of the matrix
functions (though it may be not the best choice for computer computations). Let
f(z) be an analytical function of a complex argument. Applying the function on
a nÃn Jordan block J with eigenvalue Î» results in an upper triangular matrix:
         f ( J ) =   [    f ( &#x03BB; )    f &#x2032;  ( &#x03BB; )        f
      &#x2033;  ( &#x03BB; )  2      . . .        f  ( n &#x2212; 1 )
      ( &#x03BB; )   ( n &#x2212; 1 ) !         0   f ( &#x03BB; )    f
      &#x2032;  ( &#x03BB; )   . . .        f  ( n &#x2212; 2 )   ( &#x03BB; )
      ( n &#x2212; 2 ) !         &#x22EE;   &#x22EE;   &#x22F1;   &#x22F1;
      &#x22EE;     0   0   0   f ( &#x03BB; )    f &#x2032;  ( &#x03BB; )     0
      0   0   0   f ( &#x03BB; )    ]   ,   {\displaystyle f(J)={\begin
      {bmatrix}f(\lambda )&f'(\lambda )&{\tfrac {f''(\lambda )}{2}}&...&{\tfrac
      {f^{(n-1)}(\lambda )}{(n-1)!}}\\0&f(\lambda )&f'(\lambda )&...&{\tfrac
      {f^{(n-2)}(\lambda )}{(n-2)!}}\\\vdots &\vdots &\ddots &\ddots &\vdots
      \\0&0&0&f(\lambda )&f'(\lambda )\\0&0&0&0&f(\lambda )\end{bmatrix}},}  [
      {\displaystyle f(J)={\begin{bmatrix}f(\lambda )&f'(\lambda )&{\tfrac {f''
      (\lambda )}{2}}&...&{\tfrac {f^{(n-1)}(\lambda )}{(n-1)!}}\\0&f(\lambda
      )&f'(\lambda )&...&{\tfrac {f^{(n-2)}(\lambda )}{(n-2)!}}\\\vdots &\vdots
      &\ddots &\ddots &\vdots \\0&0&0&f(\lambda )&f'(\lambda )\\0&0&0&0&f
      (\lambda )\end{bmatrix}},}]
so that the elements of the k-th superdiagonal of the resulting matrix are
f  ( k )   ( &#x03BB; )   k !       {\displaystyle {\tfrac {f^{(k)}(\lambda )}
{k!}}}  [{\displaystyle {\tfrac {f^{(k)}(\lambda )}{k!}}}]. For a matrix of
general Jordan normal form the above expression shall be applied to each Jordan
block.
The following example shows the application to the power function f(z)=zn:
            [     &#x03BB;  1     1   0   0   0     0    &#x03BB;  1     1   0
      0     0   0    &#x03BB;  1     0   0     0   0   0    &#x03BB;  2     1
      0   0   0   0    &#x03BB;  2      ]    n   =   [     &#x03BB;  1   n
      (   n 1   )      &#x03BB;  1   n &#x2212; 1         (   n 2   )
      &#x03BB;  1   n &#x2212; 2     0   0     0    &#x03BB;  1   n
      (   n 1   )      &#x03BB;  1   n &#x2212; 1     0   0     0   0
      &#x03BB;  1   n     0   0     0   0   0    &#x03BB;  2   n         (   n
      1   )      &#x03BB;  2   n &#x2212; 1       0   0   0   0    &#x03BB;  2
      n      ]   ,   {\displaystyle {\begin{bmatrix}\lambda _
      {1}&1&0&0&0\\0&\lambda _{1}&1&0&0\\0&0&\lambda _{1}&0&0\\0&0&0&\lambda _
      {2}&1\\0&0&0&0&\lambda _{2}\end{bmatrix}}^{n}={\begin{bmatrix}\lambda _
      {1}^{n}&{\tbinom {n}{1}}\lambda _{1}^{n-1}&{\tbinom {n}{2}}\lambda _{1}^
      {n-2}&0&0\\0&\lambda _{1}^{n}&{\tbinom {n}{1}}\lambda _{1}^{n-
      1}&0&0\\0&0&\lambda _{1}^{n}&0&0\\0&0&0&\lambda _{2}^{n}&{\tbinom {n}
      {1}}\lambda _{2}^{n-1}\\0&0&0&0&\lambda _{2}^{n}\end{bmatrix}},}  [
      {\displaystyle {\begin{bmatrix}\lambda _{1}&1&0&0&0\\0&\lambda _
      {1}&1&0&0\\0&0&\lambda _{1}&0&0\\0&0&0&\lambda _{2}&1\\0&0&0&0&\lambda _
      {2}\end{bmatrix}}^{n}={\begin{bmatrix}\lambda _{1}^{n}&{\tbinom {n}
      {1}}\lambda _{1}^{n-1}&{\tbinom {n}{2}}\lambda _{1}^{n-2}&0&0\\0&\lambda
      _{1}^{n}&{\tbinom {n}{1}}\lambda _{1}^{n-1}&0&0\\0&0&\lambda _{1}^
      {n}&0&0\\0&0&0&\lambda _{2}^{n}&{\tbinom {n}{1}}\lambda _{2}^{n-
      1}\\0&0&0&0&\lambda _{2}^{n}\end{bmatrix}},}]
where the binomial coefficients are defined as         (   n k   )     =
&#x220F;  i = 1   k       n + 1 &#x2212; i  i      {\displaystyle {\tbinom {n}
{k}}=\prod _{i=1}^{k}{\tfrac {n+1-i}{i}}}  [{\displaystyle {\tbinom {n}
{k}}=\prod _{i=1}^{k}{\tfrac {n+1-i}{i}}}]. For integer positive n it reduces
to standard definition of the coefficients. For negative n the identity
(    &#x2212; n  k   )     =   (  &#x2212; 1  )   k       (    n + k &#x2212; 1
k   )       {\displaystyle {\tbinom {-n}{k}}=\left(-1\right)^{k}{\tbinom {n+k-
1}{k}}}  [{\displaystyle {\tbinom {-n}{k}}=\left(-1\right)^{k}{\tbinom {n+k-1}
{k}}}] may be of use.
***** Compact operators[edit] *****
A result analogous to the Jordan normal form holds for compact_operators on a
Banach_space. One restricts to compact operators because every point x in the
spectrum of a compact operator T, the only exception being when x is the limit
point of the spectrum, is an eigenvalue. This is not true for bounded operators
in general. To give some idea of this generalization, we first reformulate the
Jordan decomposition in the language of functional analysis.
**** Holomorphic functional calculus[edit] ****
Further information: holomorphic_functional_calculus
Let X be a Banach space, L(X) be the bounded operators on X, and Ï(T) denote
the spectrum of T â L(X). The holomorphic_functional_calculus is defined as
follows:
Fix a bounded operator T. Consider the family Hol(T) of complex functions that
is holomorphic on some open set G containing Ï(T). Let Î = {Î³i} be a finite
collection of Jordan_curves such that Ï(T) lies in the inside of Î, we define
f(T) by
         f ( T ) =   1  2 &#x03C0; i     &#x222B;  &#x0393;   f ( z ) ( z
      &#x2212; T  )  &#x2212; 1   d z .   {\displaystyle f(T)={\frac {1}{2\pi
      i}}\int _{\Gamma }f(z)(z-T)^{-1}dz.}  [f(T) = \frac{1}{2 \pi i} \int_
      {\Gamma} f(z)(z - T)^{-1} dz.]
The open set G could vary with f and need not be connected. The integral is
defined as the limit of the Riemann sums, as in the scalar case. Although the
integral makes sense for continuous f, we restrict to holomorphic functions to
apply the machinery from classical function theory (e.g., the Cauchy integral
formula). The assumption that Ï(T) lie in the inside of Î ensures f(T) is
well defined; it does not depend on the choice of Î. The functional calculus
is the mapping Î¦ from Hol(T) to L(X) given by
          &#x03A6; ( f ) = f ( T ) .   {\displaystyle \;\Phi (f)=f(T).}  [\;
      \Phi(f) = f(T).]
We will require the following properties of this functional calculus:
   1. Î¦ extends the polynomial functional calculus.
   2. The spectral mapping theorem holds: Ï(f(T)) = f(Ï(T)).
   3. Î¦ is an algebra homomorphism.
**** The finite-dimensional case[edit] ****
In the finite-dimensional case, Ï(T) = {Î»i} is a finite discrete set in the
complex plane. Let ei be the function that is 1 in some open neighborhood of
Î»i and 0 elsewhere. By property 3 of the functional calculus, the operator
           e  i   ( T )   {\displaystyle \;e_{i}(T)}  [\; e_i(T)]
is a projection. Moreoever, let Î½i be the index of Î»i and
         f ( z ) = ( z &#x2212;  &#x03BB;  i    )   &#x03BD;  i     .
      {\displaystyle f(z)=(z-\lambda _{i})^{\nu _{i}}.}  [f(z)= (z -
      \lambda_i)^{\nu_i}.]
The spectral mapping theorem tells us
         f ( T )  e  i   ( T ) = ( T &#x2212;  &#x03BB;  i    )   &#x03BD;  i
      e  i   ( T )   {\displaystyle f(T)e_{i}(T)=(T-\lambda _{i})^{\nu _{i}}e_
      {i}(T)}  [ f(T) e_i (T) = (T - \lambda_i)^{\nu_i} e_i (T)]
has spectrum {0}. By property 1, f(T) can be directly computed in the Jordan
form, and by inspection, we see that the operator f(T)ei(T) is the zero matrix.
By property 3, f(T) ei(T) = ei(T) f(T). So ei(T) is precisely the projection
onto the subspace
          R a n    e  i   ( T ) =  K e r  ( T &#x2212;  &#x03BB;  i    )
      &#x03BD;  i     .   {\displaystyle \mathrm {Ran} \;e_{i}(T)=\mathrm {Ker}
      (T-\lambda _{i})^{\nu _{i}}.}  [\mathrm{Ran} \; e_i (T) = \mathrm{Ker}(T
      - \lambda_i)^{\nu_i}.]
The relation
           &#x2211;  i    e  i   = 1   {\displaystyle \;\sum _{i}e_{i}=1}  [\;
      \sum_i e_i = 1]
implies
           C   n   =  &#x2A01;  i     R a n    e  i   ( T ) =  &#x2A01;  i
      K e r  ( T &#x2212;  &#x03BB;  i    )   &#x03BD;  i       {\displaystyle
      \mathbb {C} ^{n}=\bigoplus _{i}\;\mathrm {Ran} \;e_{i}(T)=\bigoplus _
      {i}\;\mathrm {Ker} (T-\lambda _{i})^{\nu _{i}}}  [\mathbb{C}^n =
      \bigoplus_i \; \mathrm{Ran}\; e_i (T) = \bigoplus_i \; \mathrm{Ker}(T -
      \lambda_i)^{\nu_i}]
where the index i runs through the distinct eigenvalues of T. This is exactly
the invariant subspace decomposition
           C   n   =  &#x2A01;  i    Y  i     {\displaystyle \mathbb {C} ^
      {n}=\bigoplus _{i}Y_{i}}  [\mathbb{C}^n = \bigoplus_i Y_i]
given in a previous section. Each ei(T) is the projection onto the subspace
spanned by the Jordan chains corresponding to Î»i and along the subspaces
spanned by the Jordan chains corresponding to Î»j for j â  i. In other words,
ei(T) = P(Î»i;T). This explicit identification of the operators ei(T) in turn
gives an explicit form of holomorphic functional calculus for matrices:
      For all f â Hol(T),
         f ( T ) =  &#x2211;   &#x03BB;  i   &#x2208; &#x03C3; ( T )
      &#x2211;  k = 0    &#x03BD;  i   &#x2212; 1      f  ( k )    k !    ( T
      &#x2212;  &#x03BB;  i    )  k    e  i   ( T ) .   {\displaystyle f
      (T)=\sum _{\lambda _{i}\in \sigma (T)}\sum _{k=0}^{\nu _{i}-1}{\frac {f^{
      (k)}}{k!}}(T-\lambda _{i})^{k}e_{i}(T).}  [f(T) = \sum_{\lambda_i \in
      \sigma(T)} \sum_{k = 0}^{\nu_i -1} \frac{f^{(k)}}{k!} (T - \lambda_i)^k
      e_i (T).]
Notice that the expression of f(T) is a finite sum because, on each
neighborhood of Î»i, we have chosen the Taylor series expansion of f centered
at Î»i.
**** Poles of an operator[edit] ****
Let T be a bounded operator Î» be an isolated point of Ï(T). (As stated above,
when T is compact, every point in its spectrum is an isolated point, except
possibly the limit point 0.)
The point Î» is called a pole of operator T with order Î½ if the resolvent
function RT defined by
           R  T   ( &#x03BB; ) = ( &#x03BB; &#x2212; T  )  &#x2212; 1
      {\displaystyle \;R_{T}(\lambda )=(\lambda -T)^{-1}}  [\; R_T(\lambda) =
      (\lambda - T)^{-1}]
has a pole of order Î½ at Î».
We will show that, in the finite-dimensional case, the order of an eigenvalue
coincides with its index. The result also holds for compact operators.
Consider the annular region A centered at the eigenvalue Î» with sufficiently
small radius Îµ such that the intersection of the open disc BÎµ(Î») and Ï(T)
is {Î»}. The resolvent function RT is holomorphic on A. Extending a result from
classical function theory, RT has a Laurent_series representation on A:
          R  T   ( z ) =  &#x2211;  &#x2212; &#x221E;   &#x221E;    a  m
      ( &#x03BB; &#x2212; z  )  m     {\displaystyle R_{T}(z)=\sum _{-\infty }^
      {\infty }a_{m}(\lambda -z)^{m}}  [R_T(z) = \sum _{- \infty} ^{\infty} a_m
      (\lambda - z)^m]
where
          a  &#x2212; m   = &#x2212;   1  2 &#x03C0; i     &#x222B;  C
      ( &#x03BB; &#x2212; z  )  m &#x2212; 1   ( z &#x2212; T  )  &#x2212; 1
      d z   {\displaystyle a_{-m}=-{\frac {1}{2\pi i}}\int _{C}(\lambda -z)^{m-
      1}(z-T)^{-1}dz}  [a_{-m} = - \frac{1}{2 \pi i} \int_C (\lambda - z) ^{m-
      1} (z - T)^{-1} d z] and C is a small circle centered at Î».
By the previous discussion on the functional calculus,
           a  &#x2212; m   = &#x2212; ( &#x03BB; &#x2212; T  )  m &#x2212; 1
      e  &#x03BB;   ( T )   {\displaystyle \;a_{-m}=-(\lambda -T)^{m-1}e_
      {\lambda }(T)}  [\; a_{-m} = -(\lambda - T)^{m-1} e_{\lambda} (T)] where
      e  &#x03BB;     {\displaystyle \;e_{\lambda }}  [\; e_{\lambda}] is 1 on
      B  &#x03F5;   ( &#x03BB; )   {\displaystyle \;B_{\epsilon }(\lambda )}
      [\; B_{\epsilon}(\lambda)] and 0 elsewhere.
But we have shown that the smallest positive integer m such that
          a  &#x2212; m   &#x2260; 0   {\displaystyle a_{-m}\neq 0}  [a_{-m}
      \neq 0] and      a  &#x2212; l   = 0   &#x2200;  l &#x2265; m
      {\displaystyle a_{-l}=0\;\;\forall \;l\geq m}  [a_{-l} = 0 \; \; \forall
      \; l \geq m]
is precisely the index of Î», Î½(Î»). In other words, the function RT has a
pole of order Î½(Î») at Î».
***** Numerical analysis[edit] *****
If the matrix A has multiple eigenvalues, or is close to a matrix with multiple
eigenvalues, then its Jordan normal form is very sensitive to perturbations.
Consider for instance the matrix
         A =   [    1   1     &#x03B5;   1    ]   .   {\displaystyle A={\begin
      {bmatrix}1&1\\\varepsilon &1\end{bmatrix}}.}  [ A = \begin{bmatrix} 1 & 1
      \\ \varepsilon & 1 \end{bmatrix}. ]
If Îµ = 0, then the Jordan normal form is simply
           [    1   1     0   1    ]   .   {\displaystyle {\begin
      {bmatrix}1&1\\0&1\end{bmatrix}}.}  [ \begin{bmatrix} 1 & 1 \\ 0 & 1 \end
      {bmatrix}. ]
However, for Îµ â  0, the Jordan normal form is
           [    1 +   &#x03B5;     0     0   1 &#x2212;   &#x03B5;      ]   .
      {\displaystyle {\begin{bmatrix}1+{\sqrt {\varepsilon }}&0\\0&1-{\sqrt
      {\varepsilon }}\end{bmatrix}}.}  [ \begin{bmatrix} 1+\sqrt\varepsilon & 0
      \\ 0 & 1-\sqrt\varepsilon \end{bmatrix}. ]
This ill_conditioning makes it very hard to develop a robust numerical
algorithm for the Jordan normal form, as the result depends critically on
whether two eigenvalues are deemed to be equal. For this reason, the Jordan
normal form is usually avoided in numerical_analysis; the stable Schur
decomposition[17] or pseudospectra[18] are better alternatives.
***** See also[edit] *****
    * Canonical_basis
    * Canonical_form
    * Frobenius_normal_form
    * Jordan_matrix
    * JordanâChevalley_decomposition
    * Matrix_decomposition
    * Modal_matrix
    * Weyr_canonical_form
***** Notes[edit] *****
   1. ^  Shilov defines the term Jordan canonical form and in a footnote says
      that Jordan normal form is synonymous. These terms are sometimes
      shortened to Jordan form. (Shilov) The term Classical canonical form is
      also sometimes used in the sense of this article. (James & James, 1976)
   2. ^ a b Holt_&_Rumynin_(2009, p. 9)
   3. ^ a b Beauregard_&_Fraleigh_(1973, pp. 310â316)
   4. ^ a b Golub_&_Van_Loan_(1996, p. 355)
   5. ^ a b Nering_(1970, pp. 118â127)
   6. ^ Beauregard_&_Fraleigh_(1973, pp. 270â274)
   7. ^ Golub_&_Van_Loan_(1996, p. 353)
   8. ^ Nering_(1970, pp. 113â118)
   9. ^ Brechenmacher, "Histoire_du_thÃ©orÃ¨me_de_Jordan_de_la_dÃ©composition
      matricielle_(1870-1930)._Formes_de_reprÃ©sentation_et_mÃ©thodes_de
      dÃ©composition", Thesis, 2007
  10. ^ Cullen_(1966, p. 114)
  11. ^ Franklin_(1968, p. 122)
  12. ^ a b Horn_&_Johnson_(1985, Â§3.2.1)
  13. ^ Bronson_(1970, pp. 189,194)
  14. ^ Horn_&_Johnson_(1985, Theorem 3.4.5)
  15. ^Vladimir I. Arnold (Ed.) (2004). Arnold's problems. Springer-Verlag
      Berlin Heidelberg. p. 127. doi:10.1007/b138219. ISBN 978-3-540-20748-
      1.CS1 maint: Extra text: authors list (link)
  16. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
  17. ^Peteris Daugulis. (2012). "A parametrization of matrix conjugacy orbit
      sets as unions of affine planes". Linear Algebra and its Applications.
      436 (3): 709â721. arXiv:1110.0907. doi:10.1016/j.laa.2011.07.032.
  18. ^ See Golub & Van Loan (2014), Â§7.6.5; or Golub & Wilkinson (1976) for
      details.
  19. ^ See Golub & Van Loan (2014), Â§7.9
***** References[edit] *****
    * Beauregard, Raymond A.; Fraleigh, John B. (1973), A First Course In
      Linear Algebra: with Optional Introduction to Groups, Rings, and Fields,
      Boston: Houghton_Mifflin_Co., ISBN 0-395-14017-X
Bronson, Richard (1970), Matrix Methods: An Introduction, New York: Academic
Press, LCCN 70097490
Cullen, Charles G. (1966), Matrices and Linear Transformations, Reading:
Addison-Wesley, LCCN 66021267
Dunford, N.; Schwartz, J. T. (1958), Linear Operators, Part I: General Theory,
Interscience
Finkbeiner II, Daniel T. (1978), Introduction to Matrices and Linear
Transformations (3rd ed.), W._H._Freeman_and_Company
Franklin, Joel N. (1968), Matrix Theory, Englewood Cliffs: Prentice-Hall,
LCCN 68016345
Golub, Gene H.; Van Loan, Charles F. (1996), Matrix Computations (3rd ed.),
Baltimore: Johns_Hopkins_University_Press, ISBN 0-8018-5414-8
Golub, Gene H.; Wilkinson, J. H. (1976). "Ill-conditioned eigensystems and the
computation of the Jordan normal form". SIAM_Review. 18 (4): 578â619.
Holt, Derek; Rumynin, Dmitriy (2009), Algebra_I_â_Advanced_Linear_Algebra_
(MA251)_Lecture_Notes (PDF)
Horn, Roger A.; Johnson, Charles R. (1985), Matrix Analysis, Cambridge
University_Press, ISBN 978-0-521-38632-6
James, Glenn; James, Robert C. (1976), Mathematics Dictionary (2nd ed.), Van
Nostrand_Reinhold
MacLane, Saunders; Birkhoff, Garrett (1967), Algebra, Macmillan_Publishers
Michel, Anthony N.; Herget, Charles J. (1993), Applied Algebra and Functional
Analysis, Dover_Publications
Nering, Evar D. (1970), Linear Algebra and Matrix Theory (2nd ed.), New York:
Wiley, LCCN 76091646
Shafarevich, I. R.; Remizov, A. O. (2012), Linear Algebra and Geometry,
Springer, ISBN 978-3-642-30993-9
Shilov, Georgi E. (1977), Linear Algebra, Dover_Publications
Jordan_Canonical_Form_article_at_mathworld.wolfram.com

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Jordan_normal_form&oldid=902039155"
Categories:
    * Linear_algebra
    * Matrix_theory
    * Matrix_normal_forms
    * Matrix_decompositions
Hidden categories:
    * CS1_maint:_Extra_text:_authors_list
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_October_2017
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
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 16 June 2019, at 03:09 (UTC).
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
