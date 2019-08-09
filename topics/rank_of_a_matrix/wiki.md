The following text has been accessed from https://en.wikipedia.org/wiki/Rank_(linear_algebra) at Thu Aug 8 23:14:08 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Rank (linear algebra) ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In linear_algebra, the rank of a matrix     A   {\displaystyle A}  [A] is the
dimension of the vector space generated (or spanned) by its columns.[1] This
corresponds to the maximal number of linearly independent columns of     A
{\displaystyle A}  [A]. This, in turn, is identical to the dimension of the
space spanned by its rows.[2] Rank is thus a measure of the "nondegenerateness"
of the system_of_linear_equations and linear_transformation encoded by     A
{\displaystyle A}  [A]. There are multiple equivalent definitions of rank. A
matrix's rank is one of its most fundamental characteristics.
The rank is commonly denoted by     rank &#x2061; ( A )   {\displaystyle
\operatorname {rank} (A)}  [{\displaystyle \operatorname {rank} (A)}] or     rk
&#x2061; ( A )   {\displaystyle \operatorname {rk} (A)}  [{\displaystyle
\operatorname {rk} (A)}]; sometimes the parentheses are not written, as in
rank &#x2061; A   {\displaystyle \operatorname {rank} A}  [{\displaystyle
\operatorname {rank} A}].
⁰
***** Contents *****
    * 1_Main_definitions
    * 2_Examples
    * 3_Computing_the_rank_of_a_matrix
          o 3.1_Rank_from_row_echelon_forms
          o 3.2_Computation
    * 4_Proofs_that_column_rank_=_row_rank
          o 4.1_First_proof
          o 4.2_Second_proof
    * 5_Alternative_definitions
    * 6_Properties
    * 7_Applications
    * 8_Generalization
    * 9_Matrices_as_tensors
    * 10_See_also
    * 11_Notes
    * 12_References
    * 13_Further_reading
***** Main definitions[edit] *****
In this section, we give some definitions of the rank of a matrix. Many
definitions are possible; see Alternative_definitions for several of these.
The column rank of     A   {\displaystyle A}  [A] is the dimension of the
column_space of     A   {\displaystyle A}  [A], while the row rank of     A
{\displaystyle A}  [A] is the dimension of the row_space of     A
{\displaystyle A}  [A].
A fundamental result in linear algebra is that the column rank and the row rank
are always equal. (Two proofs of this result are given in Proofs_that_column
rank_&#x3d;_row_rank below.) This number (i.e., the number of linearly
independent rows or columns) is simply called the rank of     A
{\displaystyle A}  [A].
A matrix is said to have full rank if its rank equals the largest possible for
a matrix of the same dimensions, which is the lesser of the number of rows and
columns. A matrix is said to be rank deficient if it does not have full rank.
The rank is also the dimension of the image of the linear_transformation that
is given by multiplication by A. More generally, if a linear_operator on a
vector_space (possibly infinite-dimensional) has finite-dimensional image
(e.g., a finite-rank_operator), then the rank of the operator is defined as the
dimension of the image.
***** Examples[edit] *****
The matrix
           [    1   0   1     &#x2212; 2   &#x2212; 3   1     3   3   0    ]
      {\displaystyle {\begin{bmatrix}1&0&1\\-2&-3&1\\3&3&0\end{bmatrix}}}  [
      {\displaystyle {\begin{bmatrix}1&0&1\\-2&-3&1\\3&3&0\end{bmatrix}}}]
has rank 2: the first two columns are linearly_independent, so the rank is at
least 2, but since the third is a linear combination of the first two (the
second subtracted from the first), the three columns are linearly dependent so
the rank must be less than 3.
The matrix
         A =   [    1   1   0   2     &#x2212; 1   &#x2212; 1   0   &#x2212; 2
      ]     {\displaystyle A={\begin{bmatrix}1&1&0&2\\-1&-1&0&-2\end{bmatrix}}}
      [A=\begin{bmatrix}1&1&0&2\\-1&-1&0&-2\end{bmatrix}]
has rank 1: there are nonzero columns, so the rank is positive, but any pair of
columns is linearly dependent. Similarly, the transpose
          A   T    =   [    1   &#x2212; 1     1   &#x2212; 1     0   0     2
      &#x2212; 2    ]     {\displaystyle A^{\mathrm {T} }={\begin{bmatrix}1&-
      1\\1&-1\\0&0\\2&-2\end{bmatrix}}}  [{\displaystyle A^{\mathrm {T} }=
      {\begin{bmatrix}1&-1\\1&-1\\0&0\\2&-2\end{bmatrix}}}]
of     A   {\displaystyle A}  [A] has rank 1. Indeed, since the column vectors
of     A   {\displaystyle A}  [A] are the row vectors of the transpose of     A
{\displaystyle A}  [A], the statement that the column rank of a matrix equals
its row rank is equivalent to the statement that the rank of a matrix is equal
to the rank of its transpose, i.e.,    rank &#x2061; ( A ) = rank &#x2061; (  A
T    )   {\displaystyle \operatorname {rank} (A)=\operatorname {rank} (A^
{\mathrm {T} })}  [{\displaystyle \operatorname {rank} (A)=\operatorname {rank}
(A^{\mathrm {T} })}].
***** Computing the rank of a matrix[edit] *****
**** Rank from row echelon forms[edit] ****
Main article: Gaussian_elimination
A common approach to finding the rank of a matrix is to reduce it to a simpler
form, generally row_echelon_form, by elementary_row_operations. Row operations
do not change the row space (hence do not change the row rank), and, being
invertible, map the column space to an isomorphic space (hence do not change
the column rank). Once in row echelon form, the rank is clearly the same for
both row rank and column rank, and equals the number of pivots (or basic
columns) and also the number of non-zero rows.
For example, the matrix     A   {\displaystyle A}  [A] given by
         A =   [    1   2   1     &#x2212; 2   &#x2212; 3   1     3   5   0
      ]     {\displaystyle A={\begin{bmatrix}1&2&1\\-2&-3&1\\3&5&0\end
      {bmatrix}}}  [A=\begin{bmatrix}1&2&1\\-2&-3&1\\3&5&0\end{bmatrix}]
can be put in reduced row-echelon form by using the following elementary row
operations:
           [    1   2   1     &#x2212; 2   &#x2212; 3   1     3   5   0    ]
      R  2   &#x2192; 2  r  1   +  r  2     [    1   2   1     0   1   3     3
      5   0    ]    R  3   &#x2192; &#x2212; 3  r  1   +  r  3     [    1   2
      1     0   1   3     0   &#x2212; 1   &#x2212; 3    ]    R  3   &#x2192;
      r  2   +  r  3     [    1   2   1     0   1   3     0   0   0    ]    R
      1   &#x2192; &#x2212; 2  r  2   +  r  1     [    1   0   &#x2212; 5     0
      1   3     0   0   0    ]     {\displaystyle {\begin{bmatrix}1&2&1\\-2&-
      3&1\\3&5&0\end{bmatrix}}R_{2}\rightarrow 2r_{1}+r_{2}{\begin
      {bmatrix}1&2&1\\0&1&3\\3&5&0\end{bmatrix}}R_{3}\rightarrow -3r_{1}+r_{3}
      {\begin{bmatrix}1&2&1\\0&1&3\\0&-1&-3\end{bmatrix}}R_{3}\rightarrow r_
      {2}+r_{3}{\begin{bmatrix}1&2&1\\0&1&3\\0&0&0\end{bmatrix}}R_
      {1}\rightarrow -2r_{2}+r_{1}{\begin{bmatrix}1&0&-5\\0&1&3\\0&0&0\end
      {bmatrix}}}  [\begin{bmatrix}1&2&1\\-2&-3&1\\3&5&0\end
      {bmatrix}R_2\rightarrow 2r_1 + r_2 \begin{bmatrix}1&2&1\\0&1&3\\3&5&0\end
      {bmatrix} R_3 \rightarrow -3r_1 + r_3 \begin{bmatrix}1&2&1\\0&1&3\\0&-1&-
      3\end{bmatrix} R_3 \rightarrow r_2 + r_3 \begin
      {bmatrix}1&2&1\\0&1&3\\0&0&0\end{bmatrix} R_1 \rightarrow -2r_2 + r_1
      \begin{bmatrix}1&0&-5\\0&1&3\\0&0&0\end{bmatrix}].
The final matrix (in row echelon form) has two non-zero rows and thus the rank
of matrix     A   {\displaystyle A}  [A] is 2.
**** Computation[edit] ****
When applied to floating_point computations on computers, basic Gaussian
elimination (LU_decomposition) can be unreliable, and a rank-revealing
decomposition should be used instead. An effective alternative is the singular
value_decomposition (SVD), but there are other less expensive choices, such as
QR_decomposition with pivoting (so-called rank-revealing_QR_factorization),
which are still more numerically robust than Gaussian elimination. Numerical
determination of rank requires a criterion for deciding when a value, such as a
singular value from the SVD, should be treated as zero, a practical choice
which depends on both the matrix and the application.
***** Proofs that column rank = row rank[edit] *****
The fact that the column and row ranks of any matrix are equal forms an
important part of the fundamental_theorem_of_linear_algebra. We present two
proofs of this result. The first is short, uses only basic properties of linear
combinations of vectors, and is valid over any field. The proof is based upon
Wardlaw (2005).[3] The second is an elegant argument using orthogonality and is
valid for matrices over the real_numbers; it is based upon Mackiw (1995).[2]
Both proofs can be found in the book by Banerjee and Roy (2014).[4]
**** First proof[edit] ****
Let A be a matrix of size m Ã n (with m rows and n columns). Let the column
rank of A be r and let c1,...,cr be any basis for the column space of A. Place
these as the columns of an m Ã r matrix C. Every column of A can be expressed
as a linear combination of the r columns in C. This means that there is an r Ã
n matrix R such that A = CR. R is the matrix whose i-th column is formed from
the coefficients giving the i-th column of A as a linear combination of the r
columns of C. Now, each row of A is given by a linear combination of the r rows
of R. Therefore, the rows of R form a spanning set of the row space of A and,
by the Steinitz_exchange_lemma, the row rank of A cannot exceed r. This proves
that the row rank of A is less than or equal to the column rank of A. This
result can be applied to any matrix, so apply the result to the transpose of A.
Since the row rank of the transpose of A is the column rank of A and the column
rank of the transpose of A is the row rank of A, this establishes the reverse
inequality and we obtain the equality of the row rank and the column rank of A.
(Also see rank_factorization.)
**** Second proof[edit] ****
Let A be an m Ã n matrix with entries in the real_numbers whose row rank is r.
Therefore, the dimension of the row space of A is r. Let      x  1   ,  x  2
, &#x2026; ,  x  r     {\displaystyle x_{1},x_{2},\ldots ,x_{r}}  [x_1,
x_2,\ldots, x_r] be a basis of the row space of A. We claim that the vectors
A  x  1   , A  x  2   , &#x2026; , A  x  r     {\displaystyle Ax_{1},Ax_
{2},\ldots ,Ax_{r}}  [Ax_1, Ax_2,\ldots, Ax_r] are linearly_independent. To see
why, consider a linear homogeneous relation involving these vectors with scalar
coefficients      c  1   ,  c  2   , &#x2026; ,  c  r     {\displaystyle c_
{1},c_{2},\ldots ,c_{r}}  [c_1,c_2,\ldots,c_r]:
         0 =  c  1   A  x  1   +  c  2   A  x  2   + &#x22EF; +  c  r   A  x  r
      = A (  c  1    x  1   +  c  2    x  2   + &#x22EF; +  c  r    x  r   ) =
      A v ,   {\displaystyle 0=c_{1}Ax_{1}+c_{2}Ax_{2}+\cdots +c_{r}Ax_{r}=A(c_
      {1}x_{1}+c_{2}x_{2}+\cdots +c_{r}x_{r})=Av,}  [0 = c_1 Ax_1 + c_2 Ax_2 +
      \cdots + c_r Ax_r = A(c_1x_1 + c_2x_2 + \cdots + c_rx_r) = Av, ]
where     v =  c  1    x  1   +  c  2    x  2   + &#x22EF; +  c  r    x  r
{\displaystyle v=c_{1}x_{1}+c_{2}x_{2}+\cdots +c_{r}x_{r}}  [v = c_1x_1 +
c_2x_2 + \cdots + c_r x_r]. We make two observations: (a) v is a linear
combination of vectors in the row space of A, which implies that v belongs to
the row space of A, and (b) since A v = 0, the vector v is orthogonal to every
row vector of A and, hence, is orthogonal to every vector in the row space of
A. The facts (a) and (b) together imply that v is orthogonal to itself, which
proves that v = 0 or, by the definition of v,
          c  1    x  1   +  c  2    x  2   + &#x22EF; +  c  r    x  r   = 0.
      {\displaystyle c_{1}x_{1}+c_{2}x_{2}+\cdots +c_{r}x_{r}=0.}  [c_1x_1 +
      c_2x_2 + \cdots + c_r x_r = 0.]
But recall that the      x  i     {\displaystyle x_{i}}  [x_{i}] were chosen as
a basis of the row space of A and so are linearly independent. This implies
that      c  1   =  c  2   = &#x22EF; =  c  r   = 0   {\displaystyle c_{1}=c_
{2}=\cdots =c_{r}=0}  [c_1 = c_2 = \cdots = c_r = 0]. It follows that     A  x
1   , A  x  2   , &#x2026; , A  x  r     {\displaystyle Ax_{1},Ax_{2},\ldots
,Ax_{r}}  [Ax_1, Ax_2,\ldots, Ax_r] are linearly independent.
Now, each     A  x  i     {\displaystyle Ax_{i}}  [Ax_{i}] is obviously a
vector in the column space of A. So,     A  x  1   , A  x  2   , &#x2026; , A
x  r     {\displaystyle Ax_{1},Ax_{2},\ldots ,Ax_{r}}  [Ax_1, Ax_2,\ldots,
Ax_r] is a set of r linearly independent vectors in the column space of A and,
hence, the dimension of the column space of A (i.e., the column rank of A) must
be at least as big as r. This proves that row rank of A is no larger than the
column rank of A. Now apply this result to the transpose of A to get the
reverse inequality and conclude as in the previous proof.
***** Alternative definitions[edit] *****
In all the definitions in this section, the matrix A is taken to be an m Ã n
matrix over an arbitrary field F.
  Dimension of image
Given the matrix     A   {\displaystyle A}  [A], there is an associated linear
mapping
         f :  F  n   &#x21A6;  F  m     {\displaystyle f:F^{n}\mapsto F^{m}}  [
      {\displaystyle f:F^{n}\mapsto F^{m}}]
defined by
         f ( x ) = A x   {\displaystyle f(x)=Ax}  [{\displaystyle f(x)=Ax}].
The rank of     A   {\displaystyle A}  [A] is the dimension of the image of
f   {\displaystyle f}  [f]. This definition has the advantage that it can be
applied to any linear map without need for a specific matrix.
  Rank in terms of nullity
Given the same linear mapping f as above, the rank is n minus the dimension of
the kernel of f. The rankânullity_theorem states that this definition is
equivalent to the preceding one.
  Column rank â dimension of column space
The rank of A is the maximal number of linearly independent columns      c  1
,  c  2   , &#x2026; ,  c  k     {\displaystyle c_{1},c_{2},\dots ,c_{k}}
[c_1,c_2,\dots,c_k] of A; this is the dimension of the column_space of A (the
column space being the subspace of Fm generated by the columns of A, which is
in fact just the image of the linear map f associated to A).
  Row rank â dimension of row space
The rank of A is the maximal number of linearly independent rows of A; this is
the dimension of the row_space of A.
  Decomposition rank
The rank of A is the smallest integer k such that A can be factored as     A =
C R   {\displaystyle A=CR}  [A=CR], where C is an m Ã k matrix and R is a k Ã
n matrix. In fact, for all integers k, the following are equivalent:
   1. the column rank of A is less than or equal to k,
   2. there exist k columns      c  1   , &#x2026; ,  c  k     {\displaystyle
      c_{1},\ldots ,c_{k}}  [c_1,\ldots,c_k] of size m such that every column
      of A is a linear combination of      c  1   , &#x2026; ,  c  k
      {\displaystyle c_{1},\ldots ,c_{k}}  [c_1,\ldots,c_k],
   3. there exist an     m &#x00D7; k   {\displaystyle m\times k}  [m \times k]
      matrix C and a     k &#x00D7; n   {\displaystyle k\times n}  [k\times n]
      matrix R such that     A = C R   {\displaystyle A=CR}  [A = CR] (when k
      is the rank, this is a rank_factorization of A),
   4. there exist k rows      r  1   , &#x2026; ,  r  k     {\displaystyle r_
      {1},\ldots ,r_{k}}  [r_1,\ldots,r_k] of size n such that every row of A
      is a linear combination of      r  1   , &#x2026; ,  r  k
      {\displaystyle r_{1},\ldots ,r_{k}}  [r_1,\ldots,r_k],
   5. the row rank of A is less than or equal to k.
Indeed, the following equivalences are obvious:     ( 1 ) &#x21D4; ( 2 )
&#x21D4; ( 3 ) &#x21D4; ( 4 ) &#x21D4; ( 5 )   {\displaystyle
(1)\Leftrightarrow (2)\Leftrightarrow (3)\Leftrightarrow (4)\Leftrightarrow
(5)}  [(1)\Leftrightarrow(2)\Leftrightarrow(3)\Leftrightarrow(4)\Leftrightarrow
(5)]. For example, to prove (3) from (2), take C to be the matrix whose columns
are      c  1   , &#x2026; ,  c  k     {\displaystyle c_{1},\ldots ,c_{k}}
[c_1,\ldots,c_k] from (2). To prove (2) from (3), take      c  1   , &#x2026; ,
c  k     {\displaystyle c_{1},\ldots ,c_{k}}  [c_1,\ldots,c_k] to be the
columns of C.
It follows from the equivalence     ( 1 ) &#x21D4; ( 5 )   {\displaystyle
(1)\Leftrightarrow (5)}  [(1)\Leftrightarrow(5)] that the row rank is equal to
the column rank.
As in the case of the "dimension of image" characterization, this can be
generalized to a definition of the rank of any linear map: the rank of a linear
map f : V â W is the minimal dimension k of an intermediate space X such that
f can be written as the composition of a map V â X and a map X â W.
Unfortunately, this definition does not suggest an efficient manner to compute
the rank (for which it is better to use one of the alternative definitions).
See rank_factorization for details.
  Rank in terms of singular values
The rank of A equals the number of non-zero singular_values, which is the same
as the number of non-zero diagonal elements in Î£ in the singular_value
decomposition     A = U &#x03A3;  V  &#x2217;     {\displaystyle A=U\Sigma V^
{*}}  [{\displaystyle A=U\Sigma V^{*}}].
  Determinantal rank â size of largest non-vanishing minor
The rank of A is the largest order of any non-zero minor in A. (The order of a
minor is the side-length of the square sub-matrix of which it is the
determinant.) Like the decomposition rank characterization, this does not give
an efficient way of computing the rank, but it is useful theoretically: a
single non-zero minor witnesses a lower bound (namely its order) for the rank
of the matrix, which can be useful (for example) to prove that certain
operations do not lower the rank of a matrix.
A non-vanishing p-minor (p Ã p submatrix with non-zero determinant) shows that
the rows and columns of that submatrix are linearly independent, and thus those
rows and columns of the full matrix are linearly independent (in the full
matrix), so the row and column rank are at least as large as the determinantal
rank; however, the converse is less straightforward. The equivalence of
determinantal rank and column rank is a strengthening of the statement that if
the span of n vectors has dimension p, then p of those vectors span the space
(equivalently, that one can choose a spanning set that is a subset of the
vectors): the equivalence implies that a subset of the rows and a subset of the
columns simultaneously define an invertible submatrix (equivalently, if the
span of n vectors has dimension p, then p of these vectors span the space and
there is a set of p coordinates on which they are linearly independent).
  Tensor rank â minimum number of simple tensors
Main articles: Tensor_rank_decomposition and Tensor_rank
The rank of A is the smallest number k such that A can be written as a sum of k
rank 1 matrices, where a matrix is defined to have rank 1 if and only if it can
be written as a nonzero product     c &#x22C5; r   {\displaystyle c\cdot r}  [c
\cdot r] of a column vector c and a row vector r. This notion of rank is called
tensor_rank; it can be generalized in the separable_models interpretation of
the singular_value_decomposition.
***** Properties[edit] *****
We assume that A is an m Ã n matrix, and we define the linear map f by f(x) =
Ax as above.
    * The rank of an m Ã n matrix is a nonnegative integer and cannot be
      greater than either m or n. That is,
               rank &#x2061; ( A ) &#x2264; min ( m , n ) .   {\displaystyle
            \operatorname {rank} (A)\leq \min(m,n).}  [\operatorname{rank}(A)
            \le \min(m, n).]
      A matrix that has rank min(m, n) is said to have full rank; otherwise,
      the matrix is rank deficient.
    * Only a zero_matrix has rank zero.
    * f is injective (or "one-to-one") if and only if A has rank n (in this
      case, we say that A has full column rank).
    * f is surjective (or "onto") if and only if A has rank m (in this case, we
      say that A has full row rank).
    * If A is a square matrix (i.e., m = n), then A is invertible if and only
      if A has rank n (that is, A has full rank).
    * If A is a square matrix, then A is invertible if and only if its
      determinant is non-zero.
    * If B is any n Ã k matrix, then
               rank &#x2061; ( A B ) &#x2264; min ( rank &#x2061; ( A ) , rank
            &#x2061; ( B ) ) .   {\displaystyle \operatorname {rank} (AB)\leq
            \min(\operatorname {rank} (A),\operatorname {rank} (B)).}  [
            {\displaystyle \operatorname {rank} (AB)\leq \min(\operatorname
            {rank} (A),\operatorname {rank} (B)).}]
    * If B is an n Ã k matrix of rank n, then
               rank &#x2061; ( A B ) = rank &#x2061; ( A ) .   {\displaystyle
            \operatorname {rank} (AB)=\operatorname {rank} (A).}
            [\operatorname{rank}(AB) = \operatorname{rank}(A).]
    * If C is an l Ã m matrix of rank m, then
               rank &#x2061; ( C A ) = rank &#x2061; ( A ) .   {\displaystyle
            \operatorname {rank} (CA)=\operatorname {rank} (A).}
            [\operatorname{rank}(CA) = \operatorname{rank}(A).]
    * The rank of A is equal to r if and only if there exists an invertible m
      Ã m matrix X and an invertible n Ã n matrix Y such that
               X A Y =   [     I  r     0     0   0    ]   ,   {\displaystyle
            XAY={\begin{bmatrix}I_{r}&0\\0&0\\\end{bmatrix}},}  [
              XAY =
              \begin{bmatrix}
                I_r & 0 \\
                0 & 0 \\
              \end{bmatrix},
            ]
      where Ir denotes the r Ã r identity_matrix.
    * Sylvesterâs rank inequality: if A is an m Ã n matrix and B is n Ã k,
      then
               rank &#x2061; ( A ) + rank &#x2061; ( B ) &#x2212; n &#x2264;
            rank &#x2061; ( A B ) .   {\displaystyle \operatorname {rank}
            (A)+\operatorname {rank} (B)-n\leq \operatorname {rank} (AB).}
            [\operatorname{rank}(A) + \operatorname{rank}(B) - n \leq
            \operatorname{rank}(A B).][i]
      This is a special case of the next inequality.
    * The inequality due to Frobenius: if AB, ABC and BC are defined, then
               rank &#x2061; ( A B ) + rank &#x2061; ( B C ) &#x2264; rank
            &#x2061; ( B ) + rank &#x2061; ( A B C ) .   {\displaystyle
            \operatorname {rank} (AB)+\operatorname {rank} (BC)\leq
            \operatorname {rank} (B)+\operatorname {rank} (ABC).}
            [\operatorname{rank}(AB) + \operatorname{rank}(BC) \le
            \operatorname{rank}(B) + \operatorname{rank}(ABC).][ii]
    * Subadditivity:
               rank &#x2061; ( A + B ) &#x2264; rank &#x2061; ( A ) + rank
            &#x2061; ( B )   {\displaystyle \operatorname {rank} (A+B)\leq
            \operatorname {rank} (A)+\operatorname {rank} (B)}  [\operatorname
            {rank}(A+ B) \le \operatorname{rank}(A) + \operatorname{rank}(B) ]
      when A and B are of the same dimension. As a consequence, a rank-k matrix
      can be written as the sum of k rank-1 matrices, but not fewer.
    * The rank of a matrix plus the nullity of the matrix equals the number of
      columns of the matrix. (This is the rankânullity_theorem.)
    * If A is a matrix over the real_numbers then the rank of A and the rank of
      its corresponding Gram_matrix are equal. Thus, for real matrices
               rank &#x2061; (  A   T    A ) = rank &#x2061; ( A  A   T    ) =
            rank &#x2061; ( A ) = rank &#x2061; (  A   T    ) .
            {\displaystyle \operatorname {rank} (A^{\mathrm {T}
            }A)=\operatorname {rank} (AA^{\mathrm {T} })=\operatorname {rank}
            (A)=\operatorname {rank} (A^{\mathrm {T} }).}  [\operatorname{rank}
            (A^\mathrm{T} A) = \operatorname{rank}(A A^\mathrm{T}) =
            \operatorname{rank}(A) = \operatorname{rank}(A^\mathrm{T}).]
      This can be shown by proving equality of their null_spaces. The null
      space of the Gram matrix is given by vectors x for which      A   T    A
      x = 0.   {\displaystyle A^{\mathrm {T} }Ax=0.}  [A^\mathrm{T} A x = 0.]
      If this condition is fulfilled, we also have     0 =  x   T     A   T
      A x =   |  A x  |   2   .   {\displaystyle 0=x^{\mathrm {T} }A^{\mathrm
      {T} }Ax=\left|Ax\right|^{2}.}  [0 = x^\mathrm{T} A^\mathrm{T} A x =
      \left| A x \right| ^2.][5]
    * If A is a matrix over the complex_numbers and       A &#x00AF;
      {\displaystyle {\overline {A}}}  [{\overline {A}}] denotes the complex
      conjugate of A and Aâ the conjugate transpose of A (i.e., the adjoint
      of A), then
               rank &#x2061; ( A ) = rank &#x2061; (   A &#x00AF;   ) = rank
            &#x2061; (  A   T    ) = rank &#x2061; (  A  &#x2217;   ) = rank
            &#x2061; (  A  &#x2217;   A ) = rank &#x2061; ( A  A  &#x2217;   )
            .   {\displaystyle \operatorname {rank} (A)=\operatorname {rank} (
            {\overline {A}})=\operatorname {rank} (A^{\mathrm {T}
            })=\operatorname {rank} (A^{*})=\operatorname {rank} (A^
            {*}A)=\operatorname {rank} (AA^{*}).}  [{\displaystyle
            \operatorname {rank} (A)=\operatorname {rank} ({\overline
            {A}})=\operatorname {rank} (A^{\mathrm {T} })=\operatorname {rank}
            (A^{*})=\operatorname {rank} (A^{*}A)=\operatorname {rank} (AA^
            {*}).}]
***** Applications[edit] *****
One useful application of calculating the rank of a matrix is the computation
of the number of solutions of a system_of_linear_equations. According to the
RouchÃ©âCapelli_theorem, the system is inconsistent if the rank of the
augmented_matrix is greater than the rank of the coefficient_matrix. If, on the
other hand, the ranks of these two matrices are equal, then the system must
have at least one solution. The solution is unique if and only if the rank
equals the number of variables. Otherwise the general solution has k free
parameters where k is the difference between the number of variables and the
rank. In this case (and assuming the system of equations is in the real or
complex numbers) the system of equations has infinitely many solutions.
In control_theory, the rank of a matrix can be used to determine whether a
linear_system is controllable, or observable.
In the field of communication_complexity, the rank of the communication_matrix
of a function gives bounds on the amount of communication needed for two
parties to compute the function.
***** Generalization[edit] *****
There are different generalizations of the concept of rank to matrices over
arbitrary rings, where column rank, row rank, dimension of column space, and
dimension of row space of a matrix may be different from the others or may not
exist.
Thinking of matrices as tensors, the tensor_rank generalizes to arbitrary
tensors; note that for tensors of order greater than 2 (matrices are order 2
tensors), rank is very hard to compute, unlike for matrices.
There is a notion of rank for smooth_maps between smooth_manifolds. It is equal
to the linear rank of the derivative.
***** Matrices as tensors[edit] *****
Matrix rank should not be confused with tensor_order, which is called tensor
rank. Tensor order is the number of indices required to write a tensor, and
thus matrices all have tensor order 2. More precisely, matrices are tensors of
type (1,1), having one row index and one column index, also called covariant
order 1 and contravariant order 1; see Tensor_(intrinsic_definition) for
details.
Note that the tensor rank of a matrix can also mean the minimum number of
simple_tensors necessary to express the matrix as a linear combination, and
that this definition does agree with matrix rank as here discussed.
***** See also[edit] *****
    * Matroid_rank
    * Nonnegative_rank_(linear_algebra)
    * Rank_(differential_topology)
    * Multicollinearity
    * Linear_dependence
***** Notes[edit] *****
   1. ^ Proof: Apply the rankânullity theorem to the inequality
                     dim &#x2061; ker &#x2061; ( A B ) &#x2264; dim &#x2061;
                  ker &#x2061; ( A ) + dim &#x2061; ker &#x2061; ( B )
                  {\displaystyle \dim \operatorname {ker} (AB)\leq \dim
                  \operatorname {ker} (A)+\dim \operatorname {ker} (B)}  [\dim
                  \operatorname{ker}(AB) \le \dim \operatorname{ker}(A) + \dim
                  \operatorname{ker}(B)].
   2. ^ Proof: The map
               C : ker &#x2061; ( A B C )  /  ker &#x2061; ( B C ) &#x2192; ker
            &#x2061; ( A B )  /  ker &#x2061; ( B )   {\displaystyle C:
            \operatorname {ker} (ABC)/\operatorname {ker} (BC)\to \operatorname
            {ker} (AB)/\operatorname {ker} (B)}  [C: \operatorname{ker}(ABC) /
            \operatorname{ker}(BC) \to \operatorname{ker}(AB) / \operatorname
            {ker}(B)]
      is well-defined and injective. We thus obtain the inequality in terms of
      dimensions of kernel, which can then be converted to the inequality in
      terms of ranks by the rankânullity theorem. Alternatively, if M is a
      linear subspace then dim(AM) â¤ dim(M); apply this inequality to the
      subspace defined by the (orthogonal) complement of the image of BC in the
      image of B, whose dimension is rk(B) â rk(BC); its image under A has
      dimension rk(AB) â rk(ABC).
***** References[edit] *****
   1. ^ Bourbaki, Algebra, ch. II, Â§10.12, p. 359
   2. ^ a bMackiw, G. (1995), "A Note on the Equality of the Column and Row
      Rank of a Matrix", Mathematics_Magazine, 68 (4)
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
   4. ^ Wardlaw, William P. (2005), "Row Rank Equals Column Rank", Mathematics
      Magazine, 78 (4)
   5. ^Banerjee, Sudipto; Roy, Anindya (2014), Linear Algebra and Matrix
      Analysis for Statistics, Texts in Statistical Science (1st ed.), Chapman
      and Hall/CRC, ISBN 978-1420095388
   6. ^Mirsky, Leonid (1955). An introduction to linear algebra. Dover
      Publications. ISBN 978-0-486-66434-7.
***** Further reading[edit] *****
    * Roger A. Horn and Charles R. Johnson (1985). Matrix Analysis. ISBN 978-0-
      521-38632-6.
Kaw, Autar K. Two Chapters from the book Introduction to Matrix Algebra: 1.
Vectors [1] and System of Equations [2]
Mike Brookes: Matrix Reference Manual. [3]
    * v
    * t
    * e
Linear_algebra
                            * Scalar
                            * Vector
                            * Vector_space
                            * Scalar_multiplication
                            * Vector_projection
                            * Linear_span
                            * Linear_map
                            * Linear_projection
                            * Linear_independence
                            * Linear_combination
                            * Basis
Basic concepts              * Change_of_basis
                            * Row_and_column_spaces
                            * Orthogonality
                            * Kernel
                            * Eigenvalues_and
                              eigenvectors
                            * Outer_product
                            * Inner_product_space
                            * Dot_product
                            * Transpose
                            * GramâSchmidt_process
                            * Linear_equations
                            * Fundamental_theorem
                            * Cross_product
Vector algebra              * Triple_product
                            * Seven-dimensional_cross
                              product
                            * Geometric_algebra
                            * Exterior_algebra          [Three_dimensional
Multilinear_algebra         * Bivector                  Euclidean_space]
                            * Multivector
                            * Tensor
                            * Outermorphism
                            * Block
                            * Decomposition
                            * Invertible
                            * Minor
Matrices                    * Multiplication
                            * Rank
                            * Transformation
                            * Cramer's_rule
                            * Gaussian_elimination
                            * Determinant
                            * Dual
                            * Direct_sum
Algebraic constructions     * Function_space
                            * Quotient
                            * Subspace
                            * Tensor_product
                            * Floating-point
                            * MATLAB
                            * Numerical_stability
                            * Basic_Linear_Algebra
Numerical                     Subprograms_(BLAS)
                            * Sparse_matrix
                            * Comparison_of_linear
                              algebra_libraries
                            * Comparison_of_numerical
                              analysis_software
    * [Category] Category
    * [List-Class article] Outline
    * [Portal] Portal
    * [Wikibooks page] Wikibook
    * [Wikiversity page] Wikiversity

Retrieved from "https://en.wikipedia.org/w/index.php?title=Rank_
(linear_algebra)&oldid=904923438"
Categories:
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AzÉrbaycanca
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Hrvatski
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Lumbaart
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * ä¸­æ
Edit_links
    * This page was last edited on 5 July 2019, at 15:06 (UTC).
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
