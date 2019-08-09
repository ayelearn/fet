The following text has been accessed from https://en.wikipedia.org/wiki/LU_decomposition at Fri Aug 9 01:08:12 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** LU decomposition ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In numerical_analysis and linear_algebra, lowerâupper (LU) decomposition or
factorization factors a matrix as the product of a lower triangular_matrix and
an upper triangular matrix. The product sometimes includes a permutation_matrix
as well. LU decomposition can be viewed as the matrix form of Gaussian
elimination. Computers usually solve square systems_of_linear_equations using
LU decomposition, and it is also a key step when inverting a matrix or
computing the determinant of a matrix. LU decomposition was introduced by
mathematician Tadeusz_Banachiewicz in 1938.[1]
⁰
***** Contents *****
    * 1_Definitions
          o 1.1_LU_factorization_with_partial_pivoting
          o 1.2_LU_factorization_with_full_pivoting
          o 1.3_LDU_decomposition
    * 2_Example
    * 3_Existence_and_uniqueness
          o 3.1_Square_matrices
          o 3.2_Symmetric_positive_definite_matrices
          o 3.3_General_matrices
    * 4_Algorithms
          o 4.1_Closed_formula
          o 4.2_Doolittle_algorithm
          o 4.3_Crout_and_LUP_algorithms
          o 4.4_Randomized_algorithm
          o 4.5_Theoretical_complexity
          o 4.6_Sparse-matrix_decomposition
    * 5_Applications
          o 5.1_Solving_linear_equations
          o 5.2_Inverting_a_matrix
          o 5.3_Computing_the_determinant
          o 5.4_C_code_examples
          o 5.5_C#_code_examples
          o 5.6_MATLAB_code_examples
    * 6_See_also
    * 7_Notes
    * 8_References
    * 9_External_links
***** Definitions[edit] *****
LDU decomposition of a Walsh_matrix
Let A be a square matrix. An LU factorization refers to the factorization of A,
with proper row and/or column orderings or permutations, into two factors â a
lower triangular matrix L and an upper triangular matrix U:
         A = L U .   {\displaystyle A=LU.}  [{\displaystyle A=LU.}]
In the lower triangular matrix all elements above the diagonal are zero, in the
upper triangular matrix, all the elements below the diagonal are zero. For
example, for a 3 Ã 3 matrix A, its LU decomposition looks like this:
           [     a  11      a  12      a  13        a  21      a  22      a  23
      a  31      a  32      a  33      ]   =   [     l  11     0   0      l  21
      l  22     0      l  31      l  32      l  33      ]     [     u  11
      u  12      u  13       0    u  22      u  23       0   0    u  33      ]
      .   {\displaystyle {\begin{bmatrix}a_{11}&a_{12}&a_{13}\\a_{21}&a_{22}&a_
      {23}\\a_{31}&a_{32}&a_{33}\end{bmatrix}}={\begin{bmatrix}l_{11}&0&0\\l_
      {21}&l_{22}&0\\l_{31}&l_{32}&l_{33}\end{bmatrix}}{\begin{bmatrix}u_
      {11}&u_{12}&u_{13}\\0&u_{22}&u_{23}\\0&0&u_{33}\end{bmatrix}}.}  [
      {\displaystyle {\begin{bmatrix}a_{11}&a_{12}&a_{13}\\a_{21}&a_{22}&a_
      {23}\\a_{31}&a_{32}&a_{33}\end{bmatrix}}={\begin{bmatrix}l_{11}&0&0\\l_
      {21}&l_{22}&0\\l_{31}&l_{32}&l_{33}\end{bmatrix}}{\begin{bmatrix}u_
      {11}&u_{12}&u_{13}\\0&u_{22}&u_{23}\\0&0&u_{33}\end{bmatrix}}.}]
Without a proper ordering or permutations in the matrix, the factorization may
fail to materialize. For example, it is easy to verify (by expanding the matrix
multiplication) that      a  11   =  l  11    u  11     {\textstyle a_{11}=l_
{11}u_{11}}  [{\textstyle a_{11}=l_{11}u_{11}}]. If      a  11   = 0
{\textstyle a_{11}=0}  [{\textstyle a_{11}=0}], then at least one of      l  11
{\textstyle l_{11}}  [{\textstyle l_{11}}] and      u  11     {\textstyle u_
{11}}  [{\textstyle u_{11}}] has to be zero, which implies that either L or U
is singular. This is impossible if A is nonsingular (invertible). This is a
procedural problem. It can be removed by simply reordering the rows of A so
that the first element of the permuted matrix is nonzero. The same problem in
subsequent factorization steps can be removed the same way; see the basic
procedure below.
**** LU factorization with partial pivoting[edit] ****
It turns out that a proper permutation in rows (or columns) is sufficient for
LU factorization. LU factorization with partial pivoting (LUP) refers often to
LU factorization with row permutations only:
         P A = L U ,   {\displaystyle PA=LU,}  [{\displaystyle PA=LU,}]
where L and U are again lower and upper triangular matrices, and P is a
permutation_matrix, which, when left-multiplied to A, reorders the rows of A.
It turns out that all square matrices can be factorized in this form,[2] and
the factorization is numerically stable in practice.[3] This makes LUP
decomposition a useful technique in practice.
**** LU factorization with full pivoting[edit] ****
An LU factorization with full pivoting involves both row and column
permutations:
         P A Q = L U ,   {\displaystyle PAQ=LU,}  [{\displaystyle PAQ=LU,}]
where L, U and P are defined as before, and Q is a permutation matrix that
reorders the columns of A.[4]
**** LDU decomposition[edit] ****
An LDU decomposition is a decomposition of the form
         A = L D U ,   {\displaystyle A=LDU,}  [{\displaystyle A=LDU,}]
where D is a diagonal_matrix, and L and U are unit triangular matrices, meaning
that all the entries on the diagonals of L and U are one.
Above we required that A be a square matrix, but these decompositions can all
be generalized to rectangular matrices as well. In that case, L and D are
square matrices both of which have the same number of rows as A, and U has
exactly the same dimensions as A. Upper triangular should be interpreted as
having only zero entries below the main diagonal, which starts at the upper
left corner.
***** Example[edit] *****
We factorize the following 2-by-2 matrix:
           [    4   3     6   3    ]   =   [     l  11     0      l  21      l
      22      ]     [     u  11      u  12       0    u  22      ]   .
      {\displaystyle {\begin{bmatrix}4&3\\6&3\end{bmatrix}}={\begin{bmatrix}l_
      {11}&0\\l_{21}&l_{22}\end{bmatrix}}{\begin{bmatrix}u_{11}&u_{12}\\0&u_
      {22}\end{bmatrix}}.}  [{\displaystyle {\begin{bmatrix}4&3\\6&3\end
      {bmatrix}}={\begin{bmatrix}l_{11}&0\\l_{21}&l_{22}\end{bmatrix}}{\begin
      {bmatrix}u_{11}&u_{12}\\0&u_{22}\end{bmatrix}}.}]
One way to find the LU decomposition of this simple matrix would be to simply
solve the linear equations by inspection. Expanding the matrix multiplication
gives
              l  11   &#x22C5;  u  11   + 0 &#x22C5; 0    = 4      l  11
      &#x22C5;  u  12   + 0 &#x22C5;  u  22      = 3      l  21   &#x22C5;  u
      11   +  l  22   &#x22C5; 0    = 6      l  21   &#x22C5;  u  12   +  l  22
      &#x22C5;  u  22      = 3.       {\displaystyle {\begin{aligned}l_
      {11}\cdot u_{11}+0\cdot 0&=4\\l_{11}\cdot u_{12}+0\cdot u_{22}&=3\\l_
      {21}\cdot u_{11}+l_{22}\cdot 0&=6\\l_{21}\cdot u_{12}+l_{22}\cdot u_
      {22}&=3.\end{aligned}}}  [{\displaystyle {\begin{aligned}l_{11}\cdot u_
      {11}+0\cdot 0&=4\\l_{11}\cdot u_{12}+0\cdot u_{22}&=3\\l_{21}\cdot u_
      {11}+l_{22}\cdot 0&=6\\l_{21}\cdot u_{12}+l_{22}\cdot u_{22}&=3.\end
      {aligned}}}]
This system of equations is underdetermined. In this case any two non-zero
elements of L and U matrices are parameters of the solution and can be set
arbitrarily to any non-zero value. Therefore, to find the unique LU
decomposition, it is necessary to put some restriction on L and U matrices. For
example, we can conveniently require the lower triangular matrix L to be a unit
triangular matrix (i.e. set all the entries of its main diagonal to ones). Then
the system of equations has the following solution:
              l  21      = 1.5      u  11      = 4      u  12      = 3      u
      22      = &#x2212; 1.5       {\displaystyle {\begin{aligned}l_
      {21}&=1.5\\u_{11}&=4\\u_{12}&=3\\u_{22}&=-1.5\end{aligned}}}  [
      {\displaystyle {\begin{aligned}l_{21}&=1.5\\u_{11}&=4\\u_{12}&=3\\u_
      {22}&=-1.5\end{aligned}}}]
Substituting these values into the LU decomposition above yields
           [    4   3     6   3    ]   =   [    1   0     1.5   1    ]
      [    4   3     0   &#x2212; 1.5    ]   .   {\displaystyle {\begin
      {bmatrix}4&3\\6&3\end{bmatrix}}={\begin{bmatrix}1&0\\1.5&1\end{bmatrix}}
      {\begin{bmatrix}4&3\\0&-1.5\end{bmatrix}}.}  [{\displaystyle {\begin
      {bmatrix}4&3\\6&3\end{bmatrix}}={\begin{bmatrix}1&0\\1.5&1\end{bmatrix}}
      {\begin{bmatrix}4&3\\0&-1.5\end{bmatrix}}.}]
***** Existence and uniqueness[edit] *****
**** Square matrices[edit] ****
Any square matrix     A   {\textstyle A}  [{\textstyle A}] admits an LUP
factorization.[2] If     A   {\textstyle A}  [{\textstyle A}] is invertible,
then it admits an LU (or LDU) factorization if_and_only_if all its leading
principal minors are nonzero.[5] If     A   {\textstyle A}  [{\textstyle A}] is
a singular matrix of rank     k   {\textstyle k}  [{\textstyle k}], then it
admits an LU factorization if the first     k   {\textstyle k}  [{\textstyle
k}] leading principal minors are nonzero, although the converse is not true.[6]
If a square, invertible matrix has an LDU factorization with all diagonal
entries of L and U equal to 1, then the factorization is unique.[5] In that
case, the LU factorization is also unique if we require that the diagonal of
L   {\textstyle L}  [{\textstyle L}] (or     U   {\textstyle U}  [{\textstyle
U}]) consists of ones.
**** Symmetric positive definite matrices[edit] ****
If A is a symmetric (or Hermitian, if A is complex) positive_definite matrix,
we can arrange matters so that U is the conjugate_transpose of L. That is, we
can write A as
         A = L  L  &#x2217;   .    {\displaystyle A=LL^{*}.\,}  [{\displaystyle
      A=LL^{*}.\,}]
This decomposition is called the Cholesky_decomposition. The Cholesky
decomposition always exists and is unique â provided the matrix is positive
definite. Furthermore, computing the Cholesky decomposition is more efficient
and numerically_more_stable than computing some other LU decompositions.
**** General matrices[edit] ****
For a (not necessarily invertible) matrix over any field, the exact necessary
and sufficient conditions under which it has an LU factorization are known. The
conditions are expressed in terms of the ranks of certain submatrices. The
Gaussian elimination algorithm for obtaining LU decomposition has also been
extended to this most general case.[7]#
***** Algorithms[edit] *****
LU decomposition is basically a modified form of Gaussian_elimination. We
transform the matrix A into an upper triangular matrix U by eliminating the
entries below the main diagonal. The Doolittle algorithm does the elimination
column-by-column, starting from the left, by multiplying A to the left with
atomic lower triangular matrices. It results in a unit lower triangular matrix
and an upper triangular matrix. The Crout algorithm is slightly different and
constructs a lower triangular matrix and a unit upper triangular matrix.
Computing an LU decomposition using either of these algorithms requires 2n3/
3 floating-point operations, ignoring lower-order terms. Partial pivoting adds
only a quadratic term; this is not the case for full pivoting.[8]
**** Closed formula[edit] ****
When an LDU factorization exists and is unique, there is a closed (explicit)
formula for the elements of L, D, and U in terms of ratios of determinants of
certain submatrices of the original matrix A.[9] In particular,      D  1   =
A  1 , 1     {\textstyle D_{1}=A_{1,1}}  [{\textstyle D_{1}=A_{1,1}}], and for
i = 2 , &#x2026; , n   {\textstyle i=2,\ldots ,n}  [{\textstyle i=2,\ldots
,n}],      D  i     {\textstyle D_{i}}  [{\textstyle D_{i}}] is the ratio of
the     i   {\textstyle i}  [{\textstyle i}]-th principal submatrix to the
( i &#x2212; 1 )   {\textstyle (i-1)}  [{\textstyle (i-1)}]-th principal
submatrix. Computation of the determinants is computationally_expensive, so
this explicit formula is not used in practice.
**** Doolittle algorithm[edit] ****
Given an N Ã N matrix
         A = (  a  i , j    )  1 &#x2264; i , j &#x2264; N   ,   {\displaystyle
      A=(a_{i,j})_{1\leq i,j\leq N},}  [{\displaystyle A=(a_{i,j})_{1\leq
      i,j\leq N},}]
we define
          A  ( 0 )   := A .   {\displaystyle A^{(0)}:=A.}  [{\displaystyle A^{
      (0)}:=A.}]
We eliminate the matrix elements below the main diagonal in the n-th column of
A(n â 1) by adding to the i-th row of this matrix the n-th row multiplied by
         &#x2212;  l  i , n   := &#x2212;    a  i , n   ( n &#x2212; 1 )    a
      n , n   ( n &#x2212; 1 )       {\displaystyle -l_{i,n}:=-{\frac {a_{i,n}^
      {(n-1)}}{a_{n,n}^{(n-1)}}}}  [{\displaystyle -l_{i,n}:=-{\frac {a_{i,n}^{
      (n-1)}}{a_{n,n}^{(n-1)}}}}]
for     i = n + 1 , &#x2026; , N   {\textstyle i=n+1,\ldots ,N}  [{\textstyle
i=n+1,\ldots ,N}]. This can be done by multiplying A(n â 1) to the left with
the lower triangular matrix
          L  n   =   (    1   0    &#x2026;    0     0   &#x22F1;   &#x22F1;
      1        &#x22EE;    &#x2212;  l  n + 1 , n       &#x22EE;       &#x22EE;
      &#x22F1;   0     0    &#x2212;  l  N , n       1    )   .
      {\displaystyle L_{n}={\begin{pmatrix}1&0&&\dots &&0\\0&\ddots &\ddots
      &&&\\&&1&&&\\\vdots &&-l_{n+1,n}&&&\vdots \\&&\vdots &&\ddots &0\\0&&-l_
      {N,n}&&&1\end{pmatrix}}.}  [{\displaystyle L_{n}={\begin
      {pmatrix}1&0&&\dots &&0\\0&\ddots &\ddots &&&\\&&1&&&\\\vdots &&-l_
      {n+1,n}&&&\vdots \\&&\vdots &&\ddots &0\\0&&-l_{N,n}&&&1\end{pmatrix}}.}]
We set
          A  ( n )   :=  L  n    A  ( n &#x2212; 1 )   .   {\displaystyle A^{
      (n)}:=L_{n}A^{(n-1)}.}  [ A^{(n)} := L_n A^{(n-1)}.]
After N â 1 steps, we eliminated all the matrix elements below the main
diagonal, so we obtain an upper triangular matrix A(N â 1). We find the
decomposition
         A =  L  1   &#x2212; 1    L  1    A  ( 0 )   =  L  1   &#x2212; 1    A
      ( 1 )   =  L  1   &#x2212; 1    L  2   &#x2212; 1    L  2    A  ( 1 )   =
      L  1   &#x2212; 1    L  2   &#x2212; 1    A  ( 2 )   = &#x22EF; =  L  1
      &#x2212; 1   &#x2026;  L  N &#x2212; 1   &#x2212; 1    A  ( N &#x2212; 1
      )   .   {\displaystyle A=L_{1}^{-1}L_{1}A^{(0)}=L_{1}^{-1}A^{(1)}=L_{1}^
      {-1}L_{2}^{-1}L_{2}A^{(1)}=L_{1}^{-1}L_{2}^{-1}A^{(2)}=\dotsb =L_{1}^{-
      1}\ldots L_{N-1}^{-1}A^{(N-1)}.}  [{\displaystyle A=L_{1}^{-1}L_{1}A^{
      (0)}=L_{1}^{-1}A^{(1)}=L_{1}^{-1}L_{2}^{-1}L_{2}A^{(1)}=L_{1}^{-1}L_{2}^
      {-1}A^{(2)}=\dotsb =L_{1}^{-1}\ldots L_{N-1}^{-1}A^{(N-1)}.}]
Denote the upper triangular matrix A(N â 1) by U, and     L =  L  1
&#x2212; 1   &#x2026;  L  N &#x2212; 1   &#x2212; 1     {\textstyle L=L_{1}^{-
1}\ldots L_{N-1}^{-1}}  [{\textstyle L=L_{1}^{-1}\ldots L_{N-1}^{-1}}]. Because
the inverse of a lower triangular matrix Ln is again a lower triangular matrix,
and the multiplication of two lower triangular matrices is again a lower
triangular matrix, it follows that L is a lower triangular matrix. Moreover, it
can be seen that
         L =   (    1   0   &#x2026;     0      l  2 , 1     &#x22F1;
      &#x22F1;          1        &#x22EE;     l  n + 1 , n     &#x22F1;
      &#x22EE;       &#x22EE;    1   0      l  N , 1       l  N , n       l  N
      , N &#x2212; 1     1    )   .   {\displaystyle L={\begin
      {pmatrix}1&0&\dots &&&0\\l_{2,1}&\ddots &\ddots &&&\\&&1&&&\\\vdots &&l_
      {n+1,n}&\ddots &&\vdots \\&&\vdots &&1&0\\l_{N,1}&&l_{N,n}&&l_{N,N-
      1}&1\end{pmatrix}}.}  [{\displaystyle L={\begin{pmatrix}1&0&\dots
      &&&0\\l_{2,1}&\ddots &\ddots &&&\\&&1&&&\\\vdots &&l_{n+1,n}&\ddots
      &&\vdots \\&&\vdots &&1&0\\l_{N,1}&&l_{N,n}&&l_{N,N-1}&1\end{pmatrix}}.}]
We obtain     A = L U   {\textstyle A=LU}  [{\textstyle A=LU}].
It is clear that in order for this algorithm to work, one needs to have      a
n , n   ( n &#x2212; 1 )   &#x2260; 0   {\textstyle a_{n,n}^{(n-1)}\neq 0}  [
{\textstyle a_{n,n}^{(n-1)}\neq 0}] at each step (see the definition of      l
i , n     {\textstyle l_{i,n}}  [{\textstyle l_{i,n}}]). If this assumption
fails at some point, one needs to interchange n-th row with another row below
it before continuing. This is why an LU decomposition in general looks like
P  &#x2212; 1   A = L U   {\textstyle P^{-1}A=LU}  [{\textstyle P^{-1}A=LU}].
**** Crout and LUP algorithms[edit] ****
The LUP decomposition algorithm by Cormen et al. generalizes Crout_matrix
decomposition. It can be described as follows.
   1. If     A   {\textstyle A}  [{\textstyle A}] has a nonzero entry in its
      first row, then take a permutation matrix      P  1     {\textstyle P_
      {1}}  [{\textstyle P_{1}}] such that     A  P  1     {\textstyle AP_{1}}
      [{\textstyle AP_{1}}] has a nonzero entry in its upper left corner.
      Otherwise, take for      P  1     {\textstyle P_{1}}  [{\textstyle P_
      {1}}] the identity matrix. Let      A  1   = A  P  1     {\textstyle A_
      {1}=AP_{1}}  [{\textstyle A_{1}=AP_{1}}].
   2. Let      A  2     {\textstyle A_{2}}  [{\textstyle A_{2}}] be the matrix
      that one gets from      A  1     {\textstyle A_{1}}  [{\textstyle A_{1}}]
      by deleting both the first row and the first column. Decompose      A  2
      =  L  2    U  2    P  2     {\textstyle A_{2}=L_{2}U_{2}P_{2}}  [
      {\textstyle A_{2}=L_{2}U_{2}P_{2}}] recursively. Make     L   {\textstyle
      L}  [{\textstyle L}] from      L  2     {\textstyle L_{2}}  [{\textstyle
      L_{2}}] by first adding a zero row above and then adding the first column
      of      A  1     {\textstyle A_{1}}  [{\textstyle A_{1}}] at the left.
   3. Make      U  3     {\textstyle U_{3}}  [{\textstyle U_{3}}] from      U
      2     {\textstyle U_{2}}  [{\textstyle U_{2}}] by first adding a zero row
      above and a zero column at the left and then replacing the upper left
      entry (which is 0 at this point) by 1. Make      P  3     {\textstyle P_
      {3}}  [{\textstyle P_{3}}] from      P  2     {\textstyle P_{2}}  [
      {\textstyle P_{2}}] in a similar manner and define      A  3   =  A  1
      /   P  3   = A  P  1    /   P  3     {\textstyle A_{3}=A_{1}/P_{3}=AP_
      {1}/P_{3}}  [{\textstyle A_{3}=A_{1}/P_{3}=AP_{1}/P_{3}}]. Let     P
      {\textstyle P}  [{\textstyle P}] be the inverse of      P  1    /   P  3
      {\textstyle P_{1}/P_{3}}  [{\textstyle P_{1}/P_{3}}].
   4. At this point,      A  3     {\textstyle A_{3}}  [{\textstyle A_{3}}] is
      the same as     L  U  3     {\textstyle LU_{3}}  [{\textstyle LU_{3}}],
      except (possibly) at the first row. If the first row of     A
      {\textstyle A}  [{\textstyle A}] is zero, then      A  3   = L  U  3
      {\textstyle A_{3}=LU_{3}}  [{\textstyle A_{3}=LU_{3}}], since both have
      first row zero, and     A = L  U  3   P   {\textstyle A=LU_{3}P}  [
      {\textstyle A=LU_{3}P}] follows, as desired. Otherwise,      A  3
      {\textstyle A_{3}}  [{\textstyle A_{3}}] and     L  U  3     {\textstyle
      LU_{3}}  [{\textstyle LU_{3}}] have the same nonzero entry in the upper
      left corner, and      A  3   = L  U  3    U  1     {\textstyle A_{3}=LU_
      {3}U_{1}}  [{\textstyle A_{3}=LU_{3}U_{1}}] for some upper triangular
      square matrix      U  1     {\textstyle U_{1}}  [{\textstyle U_{1}}] with
      ones on the diagonal (     U  1     {\textstyle U_{1}}  [{\textstyle U_
      {1}}] clears entries of     L  U  3     {\textstyle LU_{3}}  [{\textstyle
      LU_{3}}] and adds entries of      A  3     {\textstyle A_{3}}  [
      {\textstyle A_{3}}] by way of the upper left corner). Now     A = L  U  3
      U  1   P   {\textstyle A=LU_{3}U_{1}P}  [{\textstyle A=LU_{3}U_{1}P}] is
      a decomposition of the desired form.
**** Randomized algorithm[edit] ****
It is possible to find a low rank approximation to an LU decomposition using a
randomized algorithm. Given an input matrix     A   {\textstyle A}  [
{\textstyle A}] and a desired low rank     k   {\textstyle k}  [{\textstyle
k}], the randomized LU returns permutation matrices     P , Q   {\textstyle
P,Q}  [{\textstyle P,Q}] and lower/upper trapezoidal matrices     L , U
{\textstyle L,U}  [{\textstyle L,U}] of size     m &#x00D7; k   {\textstyle
m\times k}  [{\textstyle m\times k}] and     k &#x00D7; n   {\textstyle k\times
n}  [{\textstyle k\times n}] respectively, such that with high probability
&#x2016; P A Q &#x2212; L U  &#x2016;  2   &#x2264; C  &#x03C3;  k + 1
{\textstyle \Vert PAQ-LU\Vert _{2}\leq C\sigma _{k+1}}  [{\textstyle \Vert PAQ-
LU\Vert _{2}\leq C\sigma _{k+1}}], where     C   {\textstyle C}  [{\textstyle
C}] is a constant that depends on the parameters of the algorithm and
&#x03C3;  k + 1     {\textstyle \sigma _{k+1}}  [{\textstyle \sigma _{k+1}}] is
the     ( k + 1 )   {\textstyle (k+1)}  [{\textstyle (k+1)}]th singular value
of the input matrix     A   {\textstyle A}  [{\textstyle A}].[10]
**** Theoretical complexity[edit] ****
If two matrices of order n can be multiplied in time M(n), where M(n) â¥ na
for some a > 2, then an LU decomposition can be computed in time O(M(n)).[11]
This means, for example, that an O(n2.376) algorithm exists based on the
CoppersmithâWinograd_algorithm.
**** Sparse-matrix decomposition[edit] ****
Special algorithms have been developed for factorizing large sparse_matrices.
These algorithms attempt to find sparse factors L and U. Ideally, the cost of
computation is determined by the number of nonzero entries, rather than by the
size of the matrix.
These algorithms use the freedom to exchange rows and columns to minimize fill-
in (entries that change from an initial zero to a non-zero value during the
execution of an algorithm).
General treatment of orderings that minimize fill-in can be addressed using
graph_theory.
***** Applications[edit] *****
**** Solving linear equations[edit] ****
Given a system of linear equations in matrix form
         A x = b ,   {\displaystyle Ax=b,}  [Ax=b,]
we want to solve the equation for x, given A and b. Suppose we have already
obtained the LUP decomposition of A such that     P A = L U   {\textstyle
PA=LU}  [{\textstyle PA=LU}], so     L U x = P b   {\textstyle LUx=Pb}  [
{\textstyle LUx=Pb}].
In this case the solution is done in two logical steps:
   1. First, we solve the equation     L y = P b   {\textstyle Ly=Pb}  [
      {\textstyle Ly=Pb}] for y.
   2. Second, we solve the equation     U x = y   {\textstyle Ux=y}  [
      {\textstyle Ux=y}] for x.
In both cases we are dealing with triangular matrices (L and U), which can be
solved directly by forward_and_backward_substitution without using the Gaussian
elimination process (however we do need this process or equivalent to compute
the LU decomposition itself).
The above procedure can be repeatedly applied to solve the equation multiple
times for different b. In this case it is faster (and more convenient) to do an
LU decomposition of the matrix A once and then solve the triangular matrices
for the different b, rather than using Gaussian elimination each time. The
matrices L and U could be thought to have "encoded" the Gaussian elimination
process.
The cost of solving a system of linear equations is approximately       2 3
n  3     {\textstyle {\frac {2}{3}}n^{3}}  [{\textstyle {\frac {2}{3}}n^{3}}]
floating-point operations if the matrix     A   {\textstyle A}  [{\textstyle
A}] has size     n   {\textstyle n}  [{\textstyle n}]. This makes it twice as
fast as algorithms based on QR_decomposition, which costs about       4 3    n
3     {\textstyle {\frac {4}{3}}n^{3}}  [{\textstyle {\frac {4}{3}}n^{3}}]
floating-point operations when Householder_reflections are used. For this
reason, LU decomposition is usually preferred.[12]
**** Inverting a matrix[edit] ****
When solving systems of equations, b is usually treated as a vector with a
length equal to the height of matrix A. In matrix inversion however, instead of
vector b, we have matrix B, where B is an n-by-p matrix, so that we are trying
to find a matrix X (also a n-by-p matrix):
         A X = L U X = B .   {\displaystyle AX=LUX=B.}  [{\displaystyle
      AX=LUX=B.}]
We can use the same algorithm presented earlier to solve for each column of
matrix X. Now suppose that B is the identity matrix of size n. It would follow
that the result X must be the inverse of A.[13] An implementation of this
methodology in the_C_programming_language can be found here.
**** Computing the determinant[edit] ****
Given the LUP decomposition     A =  P  &#x2212; 1   L U   {\textstyle A=P^{-
1}LU}  [{\textstyle A=P^{-1}LU}] of a square matrix A, the determinant of A can
be computed straightforwardly as
         det ( A ) = det (  P  &#x2212; 1   ) det ( L ) det ( U ) = ( &#x2212;
      1  )  S    (   &#x220F;  i = 1   n    l  i i    )   (   &#x220F;  i = 1
      n    u  i i    )  .   {\displaystyle \det(A)=\det(P^{-1})\det(L)\det(U)=
      (-1)^{S}\left(\prod _{i=1}^{n}l_{ii}\right)\left(\prod _{i=1}^{n}u_
      {ii}\right).}  [{\displaystyle \det(A)=\det(P^{-1})\det(L)\det(U)=(-1)^
      {S}\left(\prod _{i=1}^{n}l_{ii}\right)\left(\prod _{i=1}^{n}u_
      {ii}\right).}]
The second equation follows from the fact that the determinant of a triangular
matrix is simply the product of its diagonal entries, and that the determinant
of a permutation matrix is equal to (â1)S where S is the number of row
exchanges in the decomposition.
In the case of LU decomposition with full pivoting,     det ( A )   {\textstyle
\det(A)}  [{\textstyle \det(A)}] also equals the right-hand side of the above
equation, if we let S be the total number of row and column exchanges.
The same method readily applies to LU decomposition by setting P equal to the
identity matrix.
**** C code examples[edit] ****
/* INPUT: A - array of pointers to rows of a square matrix having dimension N
 *        Tol - small tolerance number to detect failure when the matrix is
near degenerate
 * OUTPUT: Matrix A is changed, it contains both matrices L-E and U as A=(L-
E)+U such that P*A=L*U.
 *        The permutation matrix is not stored as a matrix, but in an integer
vector P of size N+1
 *        containing column indexes where the permutation matrix has "1". The
last element P[N]=S+N,
 *        where S is the number of row exchanges needed for determinant
computation, det(P)=(-1)^S
 */
int LUPDecompose(double **A, int N, double Tol, int *P) {

    int i, j, k, imax;
    double maxA, *ptr, absA;

    for (i = 0; i <= N; i++)
        P[i] = i; //Unit permutation matrix, P[N] initialized with N

    for (i = 0; i < N; i++) {
        maxA = 0.0;
        imax = i;

        for (k = i; k < N; k++)
            if ((absA = fabs(A[k][i])) > maxA) {
                maxA = absA;
                imax = k;
            }

        if (maxA < Tol) return 0; //failure, matrix is degenerate

        if (imax != i) {
            //pivoting P
            j = P[i];
            P[i] = P[imax];
            P[imax] = j;

            //pivoting rows of A
            ptr = A[i];
            A[i] = A[imax];
            A[imax] = ptr;

            //counting pivots starting from N (for determinant)
            P[N]++;
        }

        for (j = i + 1; j < N; j++) {
            A[j][i] /= A[i][i];

            for (k = i + 1; k < N; k++)
                A[j][k] -= A[j][i] * A[i][k];
        }
    }

    return 1;  //decomposition done
}

/* INPUT: A,P filled in LUPDecompose; b - rhs vector; N - dimension
 * OUTPUT: x - solution vector of A*x=b
 */
void LUPSolve(double **A, int *P, double *b, int N, double *x) {

    for (int i = 0; i < N; i++) {
        x[i] = b[P[i]];

        for (int k = 0; k < i; k++)
            x[i] -= A[i][k] * x[k];
    }

    for (int i = N - 1; i >= 0; i--) {
        for (int k = i + 1; k < N; k++)
            x[i] -= A[i][k] * x[k];

        x[i] = x[i] / A[i][i];
    }
}

/* INPUT: A,P filled in LUPDecompose; N - dimension
 * OUTPUT: IA is the inverse of the initial matrix
 */
void LUPInvert(double **A, int *P, int N, double **IA) {

    for (int j = 0; j < N; j++) {
        for (int i = 0; i < N; i++) {
            if (P[i] == j)
                IA[i][j] = 1.0;
            else
                IA[i][j] = 0.0;

            for (int k = 0; k < i; k++)
                IA[i][j] -= A[i][k] * IA[k][j];
        }

        for (int i = N - 1; i >= 0; i--) {
            for (int k = i + 1; k < N; k++)
                IA[i][j] -= A[i][k] * IA[k][j];

            IA[i][j] = IA[i][j] / A[i][i];
        }
    }
}

/* INPUT: A,P filled in LUPDecompose; N - dimension.
 * OUTPUT: Function returns the determinant of the initial matrix
 */
double LUPDeterminant(double **A, int *P, int N) {

    double det = A[0][0];

    for (int i = 1; i < N; i++)
        det *= A[i][i];

    if ((P[N] - N) % 2 == 0)
        return det;
    else
        return -det;
}
**** C# code examples[edit] ****
public class SystemOfLinearEquations
    {
        public double[] SolveUsingLU(double[,] matrix, double[] rightPart, int
n)
        {
            // decomposition of matrix
            double[,] lu = new double[n, n];
            double sum = 0;
            for (int i = 0; i < n; i++)
            {
                for (int j = i; j < n; j++)
                {
                    sum = 0;
                    for (int k = 0; k < i; k++)
                        sum += lu[i, k] * lu[k, j];
                    lu[i, j] = matrix[i, j] - sum;
                }
                for (int j = i + 1; j < n; j++)
                {
                    sum = 0;
                    for (int k = 0; k < i; k++)
                        sum += lu[j, k] * lu[k, i];
                    lu[j, i] = (1 / lu[i, i]) * (matrix[j, i] - sum);
                }
            }

            // lu = L+U-I
            // find solution of Ly = b
            double[] y = new double[n];
            for (int i = 0; i < n; i++)
            {
                sum = 0;
                for (int k = 0; k < i; k++)
                    sum += lu[i, k] * y[k];
                y[i] = rightPart[i] - sum;
            }
            // find solution of Ux = y
            double[] x = new double[n];
            for (int i = n - 1; i >= 0; i--)
            {
                sum = 0;
                for (int k = i + 1; k < n; k++)
                    sum += lu[i, k] * x[k];
                x[i] = (1 / lu[i, i]) * (y[i] - sum);
            }
            return x;
        }
}
**** MATLAB code examples[edit] ****
function x = SolveLinearSystem(A, b)
    n = length(b);
    x = zeros(n, 1);
    y = zeros(n, 1);
    % decomposition of matrix, Doolittleâs Method
    for i = 1:1:n
        for j = 1:1:(i - 1)
            alpha = A(i,j);
            for k = 1:1:(j - 1)
                alpha = alpha - A(i,k)*A(k,j);
            end
            A(i,j) = alpha/A(j,j);
        end
        for j = i:1:n
            alpha = A(i,j);
            for k = 1:1:(i - 1)
                alpha = alpha - A(i,k)*A(k,j);
            end
            A(i,j) = alpha;
        end
    end
    %A = L+U-I
    % find solution of Ly = b
    for i = 1:1:n
        alpha = 0;
        for k = 1:1:i
            alpha = alpha + A(i,k)*y(k);
        end
        y(i) = b(i) - alpha;
    end
    % find solution of Ux = y
    for i = n:(-1):1
        alpha = 0;
        for k = (i + 1):1:n
            alpha = alpha + A(i,k)*x(k);
        end
        x(i) = (y(i) - alpha)/A(i, i);
    end
end
***** See also[edit] *****
    * Block_LU_decomposition
    * Bruhat_decomposition
    * Cholesky_decomposition
    * Incomplete_LU_factorization
    * LU_Reduction
    * Matrix_decomposition
    * QR_decomposition
***** Notes[edit] *****
   1. ^Schwarzenberg-Czerny, A. (1995). "On matrix factorization and efficient
      least squares solution". Astronomy and Astrophysics Supplement Series.
      110: 405. Bibcode:1995A&AS..110..405S.
   2. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   3. ^ a b Okunev_&_Johnson_(1997), Corollary 3.
   4. ^ Trefethen_&_Bau_(1997), p. 166.
   5. ^ Trefethen_&_Bau_(1997), p. 161.
   6. ^ a b Horn_&_Johnson_(1985), Corollary 3.5.5
   7. ^ Horn_&_Johnson_(1985), Theorem 3.5.2
   8. ^ Okunev_&_Johnson_(1997)
   9. ^ Golub_&_Van_Loan_(1996), p. 112, 119.
  10. ^ Householder_(1975)
  11. ^Shabat, Gil; Shmueli, Yaniv; Aizenbud, Yariv; Averbuch, Amir (2016).
      "Randomized LU Decomposition". Applied and Computational Harmonic
      Analysis. 44 (2): 246â272. arXiv:1310.7202. doi:10.1016/
      j.acha.2016.04.006.
  12. ^ Bunch_&_Hopcroft_(1974)
  13. ^ Trefethen_&_Bau_(1997), p. 152.
  14. ^ Golub_&_Van_Loan_(1996), p. 121
***** References[edit] *****
    * Bunch, James R.; Hopcroft,_John (1974), "Triangular factorization and
      inversion by fast matrix multiplication", Mathematics_of_Computation, 28
      (125): 231â236, doi:10.2307/2005828, ISSN 0025-5718, JSTOR 2005828
.
Cormen,_Thomas_H.; Leiserson,_Charles_E.; Rivest,_Ronald_L.; Stein,_Clifford
(2001), Introduction_to_Algorithms, MIT Press and McGraw-Hill, ISBN 978-0-262-
03293-3
.
Golub,_Gene_H.; Van_Loan,_Charles_F. (1996), Matrix Computations (3rd ed.),
Baltimore: Johns Hopkins, ISBN 978-0-8018-5414-9
.
Horn, Roger A.; Johnson, Charles R. (1985), Matrix Analysis, Cambridge
University Press, ISBN 978-0-521-38632-6
. See Section 3.5. N â 1
Householder, Alston S. (1975), The Theory of Matrices in Numerical Analysis,
New York: Dover_Publications, MR 0378371
.
Okunev, Pavel; Johnson, Charles R. (1997), Necessary And Sufficient Conditions
For Existence of the LU Factorization of an Arbitrary Matrix, arXiv:math.NA/
0506382
.
Poole, David (2006), Linear Algebra: A Modern Introduction (2nd ed.), Canada:
Thomson Brooks/Cole, ISBN 978-0-534-99845-5
.
Press, WH; Teukolsky, SA; Vetterling, WT; Flannery, BP (2007), "Section_2.3",
Numerical Recipes: The Art of Scientific Computing (3rd ed.), New York:
Cambridge University Press, ISBN 978-0-521-88068-8
.
Trefethen,_Lloyd_N.; Bau, David (1997), Numerical linear algebra, Philadelphia:
Society for Industrial and Applied Mathematics, ISBN 978-0-89871-361-9
.
***** External links[edit] *****
References
    * LU_decomposition on MathWorld.
    * LU_decomposition on Math-Linux.
    * LU_decomposition at Holistic Numerical Methods Institute
    * LU_matrix_factorization. MATLAB reference.
Computer code
    * LAPACK is a collection of FORTRAN subroutines for solving dense linear
      algebra problems
    * ALGLIB includes a partial port of the LAPACK to C++, C#, Delphi, etc.
    * C++_code, Prof. J. Loomis, University_of_Dayton
    * C_code, Mathematics Source Library
    * LU_in_X10
    * [1] Lu in C++ Anil Pedgaonkar
    * Randomized_LU_MATLAB_Code
Online resources
    * WebApp_descriptively_solving_systems_of_linear_equations_with_LU
      Decomposition
    * Matrix_Calculator, bluebit.gr
    * LU_Decomposition_Tool, uni-bonn.de
    * LU_Decomposition by Ed_Pegg,_Jr., The_Wolfram_Demonstrations_Project,
      2007.
    * v
    * t
    * e
Numerical_linear_algebra
Key concepts     * Floating_point
                 * Numerical_stability
                 * System_of_linear_equations
                 * Matrix_decompositions
Problems         * Matrix_multiplication (algorithms)
                 * Matrix_splitting
                 * Sparse_problems
                 * CPU_cache
                 * TLB
Hardware         * Cache-oblivious_algorithm
                 * SIMD
                 * Multiprocessing
                 * MATLAB
                 * Basic_Linear_Algebra_Subprograms_(BLAS)
Software         * LAPACK
                 * Specialized_libraries
                 * General_purpose_software

Retrieved from "https://en.wikipedia.org/w/
index.php?title=LU_decomposition&oldid=909780587"
Categories:
    * Matrix_decompositions
    * Numerical_linear_algebra
Hidden categories:
    * Articles_with_example_C_code
    * Articles_with_example_C_Sharp_code
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
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 15:29 (UTC).
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
