The following text has been accessed from https://en.wikipedia.org/wiki/Invertible_matrix#Methods_of_matrix_inversion at Fri Aug 9 02:42:46 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Invertible matrix ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article includes a list_of_references, related reading or external_links,
 but its sources remain unclear because it lacks inline_citations. Please help
 to improve this article by introducing more precise citations. (June 2018)
 (Learn_how_and_when_to_remove_this_template_message)
In linear_algebra, an n-by-n square_matrix A is called invertible (also
nonsingular or nondegenerate) if there exists an n-by-n square matrix B such
that
          A B  =  B A  =   I   n   &#xA0;   {\displaystyle \mathbf {AB}
      =\mathbf {BA} =\mathbf {I} _{n}\ }  [\mathbf {AB} =\mathbf {BA} =\mathbf
      {I} _{n}\ ]
where In denotes the n-by-n identity_matrix and the multiplication used is
ordinary matrix_multiplication. If this is the case, then the matrix B is
uniquely determined by A and is called the inverse of A, denoted by Aâ1.
A square matrix that is not invertible is called singular or degenerate. A
square matrix is singular if_and_only_if its determinant is 0. Singular
matrices are rare in the sense that a square matrix randomly selected from a
continuous_uniform_distribution on its entries will almost_never be singular.
Non-square matrices (m-by-n matrices for which m â  n) do not have an inverse.
However, in some cases such a matrix may have a left_inverse or right_inverse.
If A is m-by-n and the rank of A is equal to n (n â¤ m), then A has a left
inverse: an n-by-m matrix B such that BA = In. If A has rank m (m â¤ n), then
it has a right inverse: an n-by-m matrix B such that AB = Im.
Matrix inversion is the process of finding the matrix B that satisfies the
prior equation for a given invertible matrix A.
While the most common case is that of matrices over the real or complex
numbers, all these definitions can be given for matrices over any ring.
However, in the case of the ring being commutative, the condition for a square
matrix to be invertible is that its determinant is invertible in the ring,
which in general is a stricter requirement than being nonzero. For a
noncommutative ring, the usual determinant is not defined. The conditions for
existence of left-inverse or right-inverse are more complicated since a notion
of rank does not exist over rings.
The set of n Ã n invertible matrices together with the operation of matrix
multiplication form a group, the general_linear_group of degree n.
⁰
***** Contents *****
    * 1_Properties
          o 1.1_The_invertible_matrix_theorem
          o 1.2_Other_properties
          o 1.3_In_relation_to_its_adjugate
          o 1.4_In_relation_to_the_identity_matrix
          o 1.5_Density
    * 2_Examples
    * 3_Methods_of_matrix_inversion
          o 3.1_Gaussian_elimination
          o 3.2_Newton's_method
          o 3.3_CayleyâHamilton_method
          o 3.4_Eigendecomposition
          o 3.5_Cholesky_decomposition
          o 3.6_Analytic_solution
                # 3.6.1_Inversion_of_2_Ã_2_matrices
                # 3.6.2_Inversion_of_3_Ã_3_matrices
                # 3.6.3_Inversion_of_4_Ã_4_matrices
          o 3.7_Blockwise_inversion
          o 3.8_By_Neumann_series
          o 3.9_P-adic_approximation
    * 4_Derivative_of_the_matrix_inverse
    * 5_Generalized_inverse
    * 6_Applications
          o 6.1_Regression/least_squares
          o 6.2_Matrix_inverses_in_real-time_simulations
          o 6.3_Matrix_inverses_in_MIMO_wireless_communication
    * 7_See_also
    * 8_Notes
    * 9_References
    * 10_Further_reading
    * 11_External_links
***** Properties[edit] *****
**** The invertible matrix theorem[edit] ****
Let A be a square n by n matrix over a field K (for example the field R of real
numbers). The following statements are equivalent, that is, for any given
matrix they are either all true or all false:
      A is invertible, that is, A has an inverse, is nonsingular, or is
      nondegenerate.
      A is row-equivalent to the n-by-n identity_matrix In.
      A is column-equivalent to the n-by-n identity_matrix In.
      A has n pivot_positions.
      det A â  0. In general, a square matrix over a commutative_ring is
      invertible if and only if its determinant is a unit in that ring.
      A has full rank; that is, rank A = n.
      The equation Ax = 0 has only the trivial solution x = 0.
      The kernel of A is trivial, that is, it contains only the null vector as
      an element, ker(A) = {0}.
      Null A = {0}.
      The equation Ax = b has exactly one solution for each b in Kn.
      The columns of A are linearly_independent.
      The columns of A span Kn.
      Col A = Kn.
      The columns of A form a basis of Kn.
      The linear transformation mapping x to Ax is a bijection from Kn to Kn.
      There is an n-by-n matrix B such that AB = In = BA.
      The transpose AT is an invertible matrix (hence rows of A are linearly
      independent, span Kn, and form a basis of Kn).
      The number 0 is not an eigenvalue of A.
      The matrix A can be expressed as a finite product of elementary_matrices.
      The matrix A has a left inverse (that is, there exists a B such that BA =
      I) or a right inverse (that is, there exists a C such that AC = I), in
      which case both left and right inverses exist and B = C = Aâ1.
**** Other properties[edit] ****
Furthermore, the following properties hold for an invertible matrix A:
    * (Aâ1)â1 = A;
    * (kA)â1 = kâ1Aâ1 for nonzero scalar k;
    * (Ax)+ = x+Aâ1 where + denotes the MooreâPenrose_inverse and x is a
      vector;
    * (AT)â1 = (Aâ1)T;
    * For any invertible n-by-n matrices A and B, (AB)â1 = Bâ1Aâ1. More
      generally, if A1, ..., Ak are invertible n-by-n matrices, then
      (A1A2âââAkâ1Ak)â1 = Aâ1
      kAâ1
      kâ1â¯Aâ1
      2Aâ1
      1;
    * det Aâ1 = (det A)â1.
The rows of the inverse matrix V of a matrix U are orthonormal to the columns
of U (and vice versa interchanging rows for columns). To see this, suppose that
UV = VU = I where we write the rows of V as      v  i   T     {\displaystyle v_
{i}^{T}}  [{\displaystyle v_{i}^{T}}] and the columns of U as      u  j
{\displaystyle u_{j}}  [u_{j}] for     1 &#x2264; i , j &#x2264; n
{\displaystyle 1\leq i,j\leq n}  [1\leq i,j\leq n]. Then clearly, the Euclidean
inner_product of any two      v  i   T    u  j   =  &#x03B4;  i , j
{\displaystyle v_{i}^{T}u_{j}=\delta _{i,j}}  [{\displaystyle v_{i}^{T}u_
{j}=\delta _{i,j}}]. This property can also be useful in constructing the
inverse of a square matrix in some instances where a set of orthogonal vectors
(but not necessarily orthonormal vectors) to the columns of U are known and
then applying the iterative GramâSchmidt_process to this initial set to
determine the rows of the inverse V.
A matrix that is its own inverse, that is, such that A = Aâ1 and A2 = I, is
called an involutory_matrix.
**** In relation to its adjugate[edit] ****
The adjugate of a matrix     A   {\displaystyle A}  [A] can be used to find the
inverse of     A   {\displaystyle A}  [A] as follows:
If     A   {\displaystyle A}  [A] is an     n &#x00D7; n   {\displaystyle
n\times n}  [n\times n] invertible matrix, then
          A  &#x2212; 1   =   1  det ( A )    adj &#x2061; ( A )
      {\displaystyle A^{-1}={\frac {1}{\det(A)}}\operatorname {adj} (A)}  [
      {\displaystyle A^{-1}={\frac {1}{\det(A)}}\operatorname {adj} (A)}].
**** In relation to the identity matrix[edit] ****
It follows from the associativity of matrix multiplication that if
          A B  =  I  &#xA0;   {\displaystyle \mathbf {AB} =\mathbf {I} \ }
      [\mathbf {AB} =\mathbf {I} \ ]
for finite square matrices A and B, then also
          B A  =  I  &#xA0;   {\displaystyle \mathbf {BA} =\mathbf {I} \ }
      [\mathbf {BA} =\mathbf {I} \ ][1]
**** Density[edit] ****
Over the field of real numbers, the set of singular n-by-n matrices, considered
as a subset of Rn×n, is a null_set, that is, has Lebesgue measure_zero. This is
true because singular matrices are the roots of the determinant function. This
is a continuous function because it is a polynomial in the entries of the
matrix. Thus in the language of measure_theory, almost_all n-by-n matrices are
invertible.
Furthermore, the n-by-n invertible matrices are a dense open_set in the
topological_space of all n-by-n matrices. Equivalently, the set of singular
matrices is closed and nowhere_dense in the space of n-by-n matrices.
In practice however, one may encounter non-invertible matrices. And in
numerical_calculations, matrices which are invertible, but close to a non-
invertible matrix, can still be problematic; such matrices are said to be ill-
conditioned.
***** Examples[edit] *****
Consider the following 2-by-2 matrix:
          A  =   (    &#x2212; 1      3 2        1   &#x2212; 1    )   .
      {\displaystyle \mathbf {A} ={\begin{pmatrix}-1&{\tfrac {3}{2}}\\1&-1\end
      {pmatrix}}.}  [{\displaystyle \mathbf {A} ={\begin{pmatrix}-1&{\tfrac {3}
      {2}}\\1&-1\end{pmatrix}}.}]
The matrix      A    {\displaystyle \mathbf {A} }  [\mathbf {A} ] is
invertible. To check this, one can compute that     det  A  = &#x2212; 1  /  2
{\displaystyle \det \mathbf {A} =-1/2}  [{\displaystyle \det \mathbf {A} =-1/
2}], which is non-zero.
As an example of a non-invertible, or singular, matrix, consider the matrix
          B  =   (    &#x2212; 1      3 2           2 3      &#x2212; 1    )
      .   {\displaystyle \mathbf {B} ={\begin{pmatrix}-1&{\tfrac {3}{2}}\\
      {\tfrac {2}{3}}&-1\end{pmatrix}}.}  [{\displaystyle \mathbf {B} ={\begin
      {pmatrix}-1&{\tfrac {3}{2}}\\{\tfrac {2}{3}}&-1\end{pmatrix}}.}]
The determinant of      B    {\displaystyle \mathbf {B} }  [\mathbf {B} ] is 0,
which is a necessary and sufficient condition for a matrix to be non-
invertible.
***** Methods of matrix inversion[edit] *****
**** Gaussian elimination[edit] ****
GaussâJordan_elimination is an algorithm that can be used to determine
whether a given matrix is invertible and to find the inverse. An alternative is
the LU_decomposition, which generates upper and lower triangular matrices,
which are easier to invert.
**** Newton's method[edit] ****
A generalization of Newton's_method as used for a multiplicative_inverse
algorithm may be convenient, if it is convenient to find a suitable starting
seed:
          X  k + 1   = 2  X  k   &#x2212;  X  k   A  X  k   .   {\displaystyle
      X_{k+1}=2X_{k}-X_{k}AX_{k}.}  [X_{k+1}=2X_{k}-X_{k}AX_{k}.]
Victor_Pan and John_Reif have done work that includes ways of generating a
starting seed.[2][3] Byte_magazine summarised one of their approaches.[4]
Newton's method is particularly useful when dealing with families of related
matrices that behave enough like the sequence manufactured for the homotopy
above: sometimes a good starting point for refining an approximation for the
new inverse can be the already obtained inverse of a previous matrix that
nearly matches the current matrix, for example, the pair of sequences of
inverse matrices used in obtaining matrix_square_roots_by_DenmanâBeavers
iteration; this may need more than one pass of the iteration at each new
matrix, if they are not close enough together for just one to be enough.
Newton's method is also useful for "touch up" corrections to the GaussâJordan
algorithm which has been contaminated by small errors due to imperfect_computer
arithmetic.
**** CayleyâHamilton method[edit] ****
The CayleyâHamilton_theorem allows the inverse of     A   {\displaystyle A}
[A] to be expressed in terms of det(    A   {\displaystyle A}  [A]), traces and
powers of     A   {\displaystyle A}  [A]:[5]
           A   &#x2212; 1   =   1  det (  A  )     &#x2211;  s = 0   n &#x2212;
      1     A   s    &#x2211;   k  1   ,  k  2   , &#x2026; ,  k  n &#x2212; 1
      &#x220F;  l = 1   n &#x2212; 1      ( &#x2212; 1  )   k  l   + 1      l
      k  l      k  l   !    tr &#x2061; (   A   l    )   k  l     ,
      {\displaystyle \mathbf {A} ^{-1}={\frac {1}{\det(\mathbf {A} )}}\sum _
      {s=0}^{n-1}\mathbf {A} ^{s}\sum _{k_{1},k_{2},\ldots ,k_{n-1}}\prod _
      {l=1}^{n-1}{\frac {(-1)^{k_{l}+1}}{l^{k_{l}}k_{l}!}}\operatorname {tr}
      (\mathbf {A} ^{l})^{k_{l}},}  [{\displaystyle \mathbf {A} ^{-1}={\frac
      {1}{\det(\mathbf {A} )}}\sum _{s=0}^{n-1}\mathbf {A} ^{s}\sum _{k_{1},k_
      {2},\ldots ,k_{n-1}}\prod _{l=1}^{n-1}{\frac {(-1)^{k_{l}+1}}{l^{k_{l}}k_
      {l}!}}\operatorname {tr} (\mathbf {A} ^{l})^{k_{l}},}]
where     n   {\displaystyle n}  [n] is dimension of     A   {\displaystyle A}
[A], and     tr &#x2061; ( A )   {\displaystyle \operatorname {tr} (A)}  [
{\displaystyle \operatorname {tr} (A)}] is the trace of matrix     A
{\displaystyle A}  [A] given by the sum of the main diagonal. The sum is taken
over     s   {\displaystyle s}  [s] and the sets of all      k  l   &#x2265; 0
{\displaystyle k_{l}\geq 0}  [{\displaystyle k_{l}\geq 0}] satisfying the
linear Diophantine_equation
         s +  &#x2211;  l = 1   n &#x2212; 1   l  k  l   = n &#x2212; 1.
      {\displaystyle s+\sum _{l=1}^{n-1}lk_{l}=n-1.}  [{\displaystyle s+\sum _
      {l=1}^{n-1}lk_{l}=n-1.}]
The formula can be rewritten in terms of complete Bell_polynomials of arguments
t  l   = &#x2212; ( l &#x2212; 1 ) ! tr &#x2061; (  A  l   )   {\displaystyle
t_{l}=-(l-1)!\operatorname {tr} (A^{l})}  [{\displaystyle t_{l}=-(l-
1)!\operatorname {tr} (A^{l})}] as
           A   &#x2212; 1   =   1  det (  A  )     &#x2211;  s = 1   n     A
      s &#x2212; 1      ( &#x2212; 1  )  n &#x2212; 1     ( n &#x2212; s ) !
      B  n &#x2212; s   (  t  1   ,  t  2   , &#x2026; ,  t  n &#x2212; s   ) .
      {\displaystyle \mathbf {A} ^{-1}={\frac {1}{\det(\mathbf {A} )}}\sum _
      {s=1}^{n}\mathbf {A} ^{s-1}{\frac {(-1)^{n-1}}{(n-s)!}}B_{n-s}(t_{1},t_
      {2},\ldots ,t_{n-s}).}  [{\displaystyle \mathbf {A} ^{-1}={\frac {1}{\det
      (\mathbf {A} )}}\sum _{s=1}^{n}\mathbf {A} ^{s-1}{\frac {(-1)^{n-1}}{(n-
      s)!}}B_{n-s}(t_{1},t_{2},\ldots ,t_{n-s}).}]
**** Eigendecomposition[edit] ****
Main article: Eigendecomposition_of_a_matrix
If matrix A can be eigendecomposed, and if none of its eigenvalues are zero,
then A is invertible and its inverse is given by
           A   &#x2212; 1   =  Q    &#x039B;   &#x2212; 1     Q   &#x2212; 1
      ,   {\displaystyle \mathbf {A} ^{-1}=\mathbf {Q} \mathbf {\Lambda } ^{-
      1}\mathbf {Q} ^{-1},}  [{\displaystyle \mathbf {A} ^{-1}=\mathbf {Q}
      \mathbf {\Lambda } ^{-1}\mathbf {Q} ^{-1},}]
where Q is the square (NÃN) matrix whose i-th column is the eigenvector      q
i     {\displaystyle q_{i}}  [q_{i}] of A, and Î is the diagonal_matrix whose
diagonal elements are the corresponding eigenvalues, that is,      &#x039B;  i
i   =  &#x03BB;  i     {\displaystyle \Lambda _{ii}=\lambda _{i}}  [
{\displaystyle \Lambda _{ii}=\lambda _{i}}]. Furthermore, because Î is a
diagonal matrix, its inverse is easy to calculate:
           [  &#x039B;  &#x2212; 1   ]   i i   =   1  &#x03BB;  i     .
      {\displaystyle \left[\Lambda ^{-1}\right]_{ii}={\frac {1}{\lambda _
      {i}}}.}  [{\displaystyle \left[\Lambda ^{-1}\right]_{ii}={\frac {1}
      {\lambda _{i}}}.}]
**** Cholesky decomposition[edit] ****
Main article: Cholesky_decomposition
If matrix A is positive_definite, then its inverse can be obtained as
           A   &#x2212; 1   = (   L   &#x2217;    )  &#x2212; 1     L
      &#x2212; 1   ,   {\displaystyle \mathbf {A} ^{-1}=(\mathbf {L} ^{*})^{-
      1}\mathbf {L} ^{-1},}  [\mathbf {A} ^{-1}=(\mathbf {L} ^{*})^{-1}\mathbf
      {L} ^{-1},]
where L is the lower triangular Cholesky_decomposition of A, and L* denotes the
conjugate transpose of L.
**** Analytic solution[edit] ****
Main article: Cramer's_rule
Writing the transpose of the matrix_of_cofactors, known as an adjugate_matrix,
can also be an efficient way to calculate the inverse of small matrices, but
this recursive method is inefficient for large matrices. To determine the
inverse, we calculate a matrix of cofactors:
           A   &#x2212; 1   =   1   |     A     |       C    T    =   1   |
      A     |       (      C   11       C   21     &#x22EF;     C   n 1
      C   12       C   22     &#x22EF;     C   n 2       &#x22EE;   &#x22EE;
      &#x22F1;   &#x22EE;       C   1 n       C   2 n     &#x22EF;     C   n n
      )     {\displaystyle \mathbf {A} ^{-1}={1 \over {\begin{vmatrix}\mathbf
      {A} \end{vmatrix}}}\mathbf {C} ^{\mathrm {T} }={1 \over {\begin
      {vmatrix}\mathbf {A} \end{vmatrix}}}{\begin{pmatrix}\mathbf {C} _
      {11}&\mathbf {C} _{21}&\cdots &\mathbf {C} _{n1}\\\mathbf {C} _
      {12}&\mathbf {C} _{22}&\cdots &\mathbf {C} _{n2}\\\vdots &\vdots &\ddots
      &\vdots \\\mathbf {C} _{1n}&\mathbf {C} _{2n}&\cdots &\mathbf {C} _
      {nn}\\\end{pmatrix}}}  [\mathbf {A} ^{-1}={1 \over {\begin
      {vmatrix}\mathbf {A} \end{vmatrix}}}\mathbf {C} ^{\mathrm {T} }={1 \over
      {\begin{vmatrix}\mathbf {A} \end{vmatrix}}}{\begin{pmatrix}\mathbf {C} _
      {11}&\mathbf {C} _{21}&\cdots &\mathbf {C} _{n1}\\\mathbf {C} _
      {12}&\mathbf {C} _{22}&\cdots &\mathbf {C} _{n2}\\\vdots &\vdots &\ddots
      &\vdots \\\mathbf {C} _{1n}&\mathbf {C} _{2n}&\cdots &\mathbf {C} _
      {nn}\\\end{pmatrix}}]
so that
           (   A   &#x2212; 1   )   i j   =   1   |     A     |       (   C
      T    )   i j   =   1   |     A     |      (   C   j i   )
      {\displaystyle \left(\mathbf {A} ^{-1}\right)_{ij}={1 \over {\begin
      {vmatrix}\mathbf {A} \end{vmatrix}}}\left(\mathbf {C} ^{\mathrm {T}
      }\right)_{ij}={1 \over {\begin{vmatrix}\mathbf {A} \end{vmatrix}}}\left
      (\mathbf {C} _{ji}\right)}  [\left(\mathbf {A} ^{-1}\right)_{ij}={1 \over
      {\begin{vmatrix}\mathbf {A} \end{vmatrix}}}\left(\mathbf {C} ^{\mathrm
      {T} }\right)_{ij}={1 \over {\begin{vmatrix}\mathbf {A} \end
      {vmatrix}}}\left(\mathbf {C} _{ji}\right)]
where |A| is the determinant of A, C is the matrix_of_cofactors, and CT
represents the matrix transpose.
*** Inversion of 2 Ã 2 matrices[edit] ***
The cofactor equation listed above yields the following result for 2 Ã 2
matrices. Inversion of these matrices can be done as follows:[6]
           A   &#x2212; 1   =    [    a   b     c   d    ]    &#x2212; 1   =
      1  det  A       [       d     &#x2212; b     &#x2212; c    a    ]   =   1
      a d &#x2212; b c      [       d     &#x2212; b     &#x2212; c    a    ]
      .   {\displaystyle \mathbf {A} ^{-1}={\begin{bmatrix}a&b\\c&d\\\end
      {bmatrix}}^{-1}={\frac {1}{\det \mathbf {A} }}{\begin
      {bmatrix}\,\,\,d&\!\!-b\\-c&\,a\\\end{bmatrix}}={\frac {1}{ad-bc}}{\begin
      {bmatrix}\,\,\,d&\!\!-b\\-c&\,a\\\end{bmatrix}}.}  [{\displaystyle
      \mathbf {A} ^{-1}={\begin{bmatrix}a&b\\c&d\\\end{bmatrix}}^{-1}={\frac
      {1}{\det \mathbf {A} }}{\begin{bmatrix}\,\,\,d&\!\!-b\\-c&\,a\\\end
      {bmatrix}}={\frac {1}{ad-bc}}{\begin{bmatrix}\,\,\,d&\!\!-b\\-c&\,a\\\end
      {bmatrix}}.}]
This is possible because 1/(ad â bc) is the reciprocal of the determinant of
the matrix in question, and the same strategy could be used for other matrix
sizes.
The CayleyâHamilton method gives
           A   &#x2212; 1   =   1  det  A      [   (  tr &#x2061;  A   )   I
      &#x2212;  A   ]  .   {\displaystyle \mathbf {A} ^{-1}={\frac {1}{\det
      \mathbf {A} }}\left[\left(\operatorname {tr} \mathbf {A} \right)\mathbf
      {I} -\mathbf {A} \right].}  [{\displaystyle \mathbf {A} ^{-1}={\frac {1}
      {\det \mathbf {A} }}\left[\left(\operatorname {tr} \mathbf {A}
      \right)\mathbf {I} -\mathbf {A} \right].}]
*** Inversion of 3 Ã 3 matrices[edit] ***
A computationally efficient 3 Ã 3 matrix inversion is given by
           A   &#x2212; 1   =    [    a   b   c     d   e   f     g   h   i
      ]    &#x2212; 1   =   1  det (  A  )       [     A    B    C      D    E
      F      G    H    I    ]     T    =   1  det (  A  )      [     A    D
      G      B    E    H      C    F    I    ]     {\displaystyle \mathbf {A} ^
      {-1}={\begin{bmatrix}a&b&c\\d&e&f\\g&h&i\\\end{bmatrix}}^{-1}={\frac {1}
      {\det(\mathbf {A} )}}{\begin
      {bmatrix}\,A&\,B&\,C\\\,D&\,E&\,F\\\,G&\,H&\,I\\\end{bmatrix}}^{\mathrm
      {T} }={\frac {1}{\det(\mathbf {A} )}}{\begin
      {bmatrix}\,A&\,D&\,G\\\,B&\,E&\,H\\\,C&\,F&\,I\\\end{bmatrix}}}  [
      {\displaystyle \mathbf {A} ^{-1}={\begin
      {bmatrix}a&b&c\\d&e&f\\g&h&i\\\end{bmatrix}}^{-1}={\frac {1}{\det(\mathbf
      {A} )}}{\begin{bmatrix}\,A&\,B&\,C\\\,D&\,E&\,F\\\,G&\,H&\,I\\\end
      {bmatrix}}^{\mathrm {T} }={\frac {1}{\det(\mathbf {A} )}}{\begin
      {bmatrix}\,A&\,D&\,G\\\,B&\,E&\,H\\\,C&\,F&\,I\\\end{bmatrix}}}]
(where the scalar A is not to be confused with the matrix A). If the
determinant is non-zero, the matrix is invertible, with the elements of the
intermediary matrix on the right side above given by
             A    =     ( e i &#x2212; f h ) ,      D    =     &#x2212; ( b i
      &#x2212; c h ) ,      G    =     ( b f &#x2212; c e ) ,     B    =
      &#x2212; ( d i &#x2212; f g ) ,      E    =     ( a i &#x2212; c g ) ,
      H    =     &#x2212; ( a f &#x2212; c d ) ,     C    =     ( d h &#x2212;
      e g ) ,      F    =     &#x2212; ( a h &#x2212; b g ) ,      I    =
      ( a e &#x2212; b d ) .       {\displaystyle {\begin{alignedat}{6}A&={}&
      (ei-fh),&\quad &D&={}&-(bi-ch),&\quad &G&={}&(bf-ce),\\B&={}&-(di-
      fg),&\quad &E&={}&(ai-cg),&\quad &H&={}&-(af-cd),\\C&={}&(dh-eg),&\quad
      &F&={}&-(ah-bg),&\quad &I&={}&(ae-bd).\\\end{alignedat}}}  [
      {\displaystyle {\begin{alignedat}{6}A&={}&(ei-fh),&\quad &D&={}&-(bi-
      ch),&\quad &G&={}&(bf-ce),\\B&={}&-(di-fg),&\quad &E&={}&(ai-cg),&\quad
      &H&={}&-(af-cd),\\C&={}&(dh-eg),&\quad &F&={}&-(ah-bg),&\quad &I&={}&(ae-
      bd).\\\end{alignedat}}}]
The determinant of A can be computed by applying the rule_of_Sarrus as follows:
         det (  A  ) = a A + b B + c C .   {\displaystyle \det(\mathbf {A}
      )=aA+bB+cC.}  [\det(\mathbf {A} )=aA+bB+cC.]
The CayleyâHamilton decomposition gives
           A   &#x2212; 1   =   1  det (  A  )     [    1 2    (  ( tr &#x2061;
      A   )  2   &#x2212; tr &#x2061;   A   2    )   I  &#x2212;  A  tr
      &#x2061;  A  +   A   2    ]  .   {\displaystyle \mathbf {A} ^{-1}={\frac
      {1}{\det(\mathbf {A} )}}\left[{\frac {1}{2}}\left((\operatorname {tr}
      \mathbf {A} )^{2}-\operatorname {tr} \mathbf {A} ^{2}\right)\mathbf {I} -
      \mathbf {A} \operatorname {tr} \mathbf {A} +\mathbf {A} ^{2}\right].}  [
      {\displaystyle \mathbf {A} ^{-1}={\frac {1}{\det(\mathbf {A} )}}\left[
      {\frac {1}{2}}\left((\operatorname {tr} \mathbf {A} )^{2}-\operatorname
      {tr} \mathbf {A} ^{2}\right)\mathbf {I} -\mathbf {A} \operatorname {tr}
      \mathbf {A} +\mathbf {A} ^{2}\right].}]
The general 3 Ã 3 inverse can be expressed concisely in terms of the cross
product and triple_product. If a matrix      A  =  [    x   0   ,    x   1   ,
x   2    ]    {\displaystyle \mathbf {A} =\left[\mathbf {x} _{0},\;\mathbf {x}
_{1},\;\mathbf {x} _{2}\right]}  [{\displaystyle \mathbf {A} =\left[\mathbf {x}
_{0},\;\mathbf {x} _{1},\;\mathbf {x} _{2}\right]}] (consisting of three column
vectors,       x   0     {\displaystyle \mathbf {x} _{0}}  [\mathbf {x} _{0}],
x   1     {\displaystyle \mathbf {x} _{1}}  [\mathbf {x} _{1}], and       x   2
{\displaystyle \mathbf {x} _{2}}  [\mathbf {x} _{2}]) is invertible, its
inverse is given by
           A   &#x2212; 1   =   1  det (  A  )      [      (   x  1    &#x00D7;
      x  2    )    T          (   x  2    &#x00D7;   x  0    )    T
      (   x  0    &#x00D7;   x  1    )    T       ]   .   {\displaystyle
      \mathbf {A} ^{-1}={\frac {1}{\det(\mathbf {A} )}}{\begin{bmatrix}{
      (\mathbf {x_{1}} \times \mathbf {x_{2}} )}^{\mathrm {T} }\\{(\mathbf {x_
      {2}} \times \mathbf {x_{0}} )}^{\mathrm {T} }\\{(\mathbf {x_{0}} \times
      \mathbf {x_{1}} )}^{\mathrm {T} }\\\end{bmatrix}}.}  [{\displaystyle
      \mathbf {A} ^{-1}={\frac {1}{\det(\mathbf {A} )}}{\begin{bmatrix}{
      (\mathbf {x_{1}} \times \mathbf {x_{2}} )}^{\mathrm {T} }\\{(\mathbf {x_
      {2}} \times \mathbf {x_{0}} )}^{\mathrm {T} }\\{(\mathbf {x_{0}} \times
      \mathbf {x_{1}} )}^{\mathrm {T} }\\\end{bmatrix}}.}]
Note that     det (  A  )   {\displaystyle \det(\mathbf {A} )}  [{\displaystyle
\det(\mathbf {A} )}] is equal to the triple product of       x  0
{\displaystyle \mathbf {x_{0}} }  [\mathbf {x_{0}} ],       x  1
{\displaystyle \mathbf {x_{1}} }  [\mathbf {x_{1}} ], and       x  2
{\displaystyle \mathbf {x_{2}} }  [\mathbf {x_{2}} ]âthe volume of the
parallelepiped formed by the rows or columns:
         det (  A  ) =   x   0   &#x22C5; (   x   1   &#x00D7;   x   2   ) .
      {\displaystyle \det(\mathbf {A} )=\mathbf {x} _{0}\cdot (\mathbf {x} _
      {1}\times \mathbf {x} _{2}).}  [{\displaystyle \det(\mathbf {A} )=\mathbf
      {x} _{0}\cdot (\mathbf {x} _{1}\times \mathbf {x} _{2}).}]
The correctness of the formula can be checked by using cross- and triple-
product properties and by noting that for groups, left and right inverses
always coincide. Intuitively, because of the cross products, each row of
A   &#x2212; 1     {\displaystyle \mathbf {A} ^{-1}}  [\mathbf {A} ^{-1}] is
orthogonal to the non-corresponding two columns of      A    {\displaystyle
\mathbf {A} }  [\mathbf {A} ] (causing the off-diagonal terms of      I  =   A
&#x2212; 1    A    {\displaystyle \mathbf {I} =\mathbf {A} ^{-1}\mathbf {A} }
[\mathbf {I} =\mathbf {A} ^{-1}\mathbf {A} ] be zero). Dividing by
         det (  A  ) =   x   0   &#x22C5; (   x   1   &#x00D7;   x   2   )
      {\displaystyle \det(\mathbf {A} )=\mathbf {x} _{0}\cdot (\mathbf {x} _
      {1}\times \mathbf {x} _{2})}  [{\displaystyle \det(\mathbf {A} )=\mathbf
      {x} _{0}\cdot (\mathbf {x} _{1}\times \mathbf {x} _{2})}]
causes the diagonal elements of      I  =   A   &#x2212; 1    A
{\displaystyle \mathbf {I} =\mathbf {A} ^{-1}\mathbf {A} }  [\mathbf {I}
=\mathbf {A} ^{-1}\mathbf {A} ] to be unity. For example, the first diagonal
is:
         1 =   1    x  0    &#x22C5; (   x   1   &#x00D7;   x   2   )      x  0
      &#x22C5; (   x   1   &#x00D7;   x   2   ) .   {\displaystyle 1={\frac {1}
      {\mathbf {x_{0}} \cdot (\mathbf {x} _{1}\times \mathbf {x} _{2})}}\mathbf
      {x_{0}} \cdot (\mathbf {x} _{1}\times \mathbf {x} _{2}).}  [
      {\displaystyle 1={\frac {1}{\mathbf {x_{0}} \cdot (\mathbf {x} _{1}\times
      \mathbf {x} _{2})}}\mathbf {x_{0}} \cdot (\mathbf {x} _{1}\times \mathbf
      {x} _{2}).}]
*** Inversion of 4 Ã 4 matrices[edit] ***
With increasing dimension, expressions for the inverse of A get complicated.
For n = 4, the CayleyâHamilton method leads to an expression that is still
tractable:
           A   &#x2212; 1   =   1  det (  A  )     [    1 6    (  ( tr &#x2061;
      A   )  3   &#x2212; 3 tr &#x2061;  A  tr &#x2061;   A   2   + 2 tr
      &#x2061;   A   3    )   I  &#x2212;   1 2    A   (  ( tr &#x2061;  A   )
      2   &#x2212; tr &#x2061;   A   2    )  +   A   2   tr &#x2061;  A
      &#x2212;   A   3    ]  .   {\displaystyle \mathbf {A} ^{-1}={\frac {1}
      {\det(\mathbf {A} )}}\left[{\frac {1}{6}}\left((\operatorname {tr}
      \mathbf {A} )^{3}-3\operatorname {tr} \mathbf {A} \operatorname {tr}
      \mathbf {A} ^{2}+2\operatorname {tr} \mathbf {A} ^{3}\right)\mathbf {I} -
      {\frac {1}{2}}\mathbf {A} \left((\operatorname {tr} \mathbf {A} )^{2}-
      \operatorname {tr} \mathbf {A} ^{2}\right)+\mathbf {A} ^{2}\operatorname
      {tr} \mathbf {A} -\mathbf {A} ^{3}\right].}  [{\displaystyle \mathbf {A}
      ^{-1}={\frac {1}{\det(\mathbf {A} )}}\left[{\frac {1}{6}}\left(
      (\operatorname {tr} \mathbf {A} )^{3}-3\operatorname {tr} \mathbf {A}
      \operatorname {tr} \mathbf {A} ^{2}+2\operatorname {tr} \mathbf {A} ^
      {3}\right)\mathbf {I} -{\frac {1}{2}}\mathbf {A} \left((\operatorname
      {tr} \mathbf {A} )^{2}-\operatorname {tr} \mathbf {A} ^{2}\right)+\mathbf
      {A} ^{2}\operatorname {tr} \mathbf {A} -\mathbf {A} ^{3}\right].}]
**** Blockwise inversion[edit] ****
Matrices can also be inverted blockwise by using the following analytic
inversion formula:
             [     A     B       C     D     ]    &#x2212; 1   =
      [      A   &#x2212; 1   +   A   &#x2212; 1    B  (  D
      &#x2212;   C A   &#x2212; 1    B   )  &#x2212; 1     C A
      &#x2212; 1     &#x2212;   A   &#x2212; 1    B  (  D  &#x2212;
      C A   &#x2212; 1    B   )  &#x2212; 1       &#x2212; (  D
      &#x2212;   C A   &#x2212; 1    B   )  &#x2212; 1     C A
      &#x2212; 1     (  D  &#x2212;   C A   &#x2212; 1    B   )
      &#x2212; 1      ]   ,   {\displaystyle {\begin
      {bmatrix}\mathbf {A} &\mathbf {B} \\\mathbf {C} &\mathbf {D}
      \end{bmatrix}}^{-1}={\begin{bmatrix}\mathbf {A} ^{-1}+\mathbf
      {A} ^{-1}\mathbf {B} (\mathbf {D} -\mathbf {CA} ^{-1}\mathbf     
      {B} )^{-1}\mathbf {CA} ^{-1}&-\mathbf {A} ^{-1}\mathbf {B}         ( 1 )
      (\mathbf {D} -\mathbf {CA} ^{-1}\mathbf {B} )^{-1}\\-(\mathbf
      {D} -\mathbf {CA} ^{-1}\mathbf {B} )^{-1}\mathbf {CA} ^{-1}&
      (\mathbf {D} -\mathbf {CA} ^{-1}\mathbf {B} )^{-1}\end
      {bmatrix}},}  [{\begin{bmatrix}\mathbf {A} &\mathbf {B}
      \\\mathbf {C} &\mathbf {D} \end{bmatrix}}^{-1}={\begin
      {bmatrix}\mathbf {A} ^{-1}+\mathbf {A} ^{-1}\mathbf {B}
      (\mathbf {D} -\mathbf {CA} ^{-1}\mathbf {B} )^{-1}\mathbf
      {CA} ^{-1}&-\mathbf {A} ^{-1}\mathbf {B} (\mathbf {D} -
      \mathbf {CA} ^{-1}\mathbf {B} )^{-1}\\-(\mathbf {D} -\mathbf
      {CA} ^{-1}\mathbf {B} )^{-1}\mathbf {CA} ^{-1}&(\mathbf {D} -
      \mathbf {CA} ^{-1}\mathbf {B} )^{-1}\end{bmatrix}},]
where A, B, C and D are matrix_sub-blocks of arbitrary size. (A must be square,
so that it can be inverted. Furthermore, A and D − CA−1B must be nonsingular.
[7]) This strategy is particularly advantageous if A is diagonal and D − CA−1B
(the Schur_complement of A) is a small matrix, since they are the only matrices
requiring inversion.
This technique was reinvented several times and is due to Hans_Boltz (1923),
[citation_needed] who used it for the inversion of geodetic matrices, and
Tadeusz_Banachiewicz (1937), who generalized it and proved its correctness.
The nullity_theorem says that the nullity of A equals the nullity of the sub-
block in the lower right of the inverse matrix, and that the nullity of B
equals the nullity of the sub-block in the upper right of the inverse matrix.
The inversion procedure that led to Equation (1) performed matrix block
operations that operated on C and D first. Instead, if A and B are operated on
first, and provided D and A − BD−1C are nonsingular,[8] the result is
             [     A     B       C     D     ]    &#x2212; 1   =
      [    (  A  &#x2212;   B D   &#x2212; 1    C   )  &#x2212; 1
      &#x2212; (  A  &#x2212;   B D   &#x2212; 1    C   )  &#x2212;
      1     B D   &#x2212; 1       &#x2212;   D   &#x2212; 1    C
      (  A  &#x2212;   B D   &#x2212; 1    C   )  &#x2212; 1
      D   &#x2212; 1   +   D   &#x2212; 1    C  (  A  &#x2212;   B
      D   &#x2212; 1    C   )  &#x2212; 1     B D   &#x2212; 1
      ]   .   {\displaystyle {\begin{bmatrix}\mathbf {A} &\mathbf
      {B} \\\mathbf {C} &\mathbf {D} \end{bmatrix}}^{-1}={\begin
      {bmatrix}(\mathbf {A} -\mathbf {BD} ^{-1}\mathbf {C} )^{-1}&-
      (\mathbf {A} -\mathbf {BD} ^{-1}\mathbf {C} )^{-1}\mathbf        
      {BD} ^{-1}\\-\mathbf {D} ^{-1}\mathbf {C} (\mathbf {A} -           ( 2 )
      \mathbf {BD} ^{-1}\mathbf {C} )^{-1}&\quad \mathbf {D} ^{-
      1}+\mathbf {D} ^{-1}\mathbf {C} (\mathbf {A} -\mathbf {BD} ^
      {-1}\mathbf {C} )^{-1}\mathbf {BD} ^{-1}\end{bmatrix}}.}  [
      {\begin{bmatrix}\mathbf {A} &\mathbf {B} \\\mathbf {C}
      &\mathbf {D} \end{bmatrix}}^{-1}={\begin{bmatrix}(\mathbf {A}
      -\mathbf {BD} ^{-1}\mathbf {C} )^{-1}&-(\mathbf {A} -\mathbf
      {BD} ^{-1}\mathbf {C} )^{-1}\mathbf {BD} ^{-1}\\-\mathbf {D}
      ^{-1}\mathbf {C} (\mathbf {A} -\mathbf {BD} ^{-1}\mathbf {C}
      )^{-1}&\quad \mathbf {D} ^{-1}+\mathbf {D} ^{-1}\mathbf {C}
      (\mathbf {A} -\mathbf {BD} ^{-1}\mathbf {C} )^{-1}\mathbf
      {BD} ^{-1}\end{bmatrix}}.]
Equating Equations (1) and (2) leads to
          (  A  &#x2212;   B D   &#x2212; 1    C   )  &#x2212; 1
      =   A   &#x2212; 1   +   A   &#x2212; 1    B  (  D  &#x2212;
      C A   &#x2212; 1    B   )  &#x2212; 1     C A   &#x2212; 1
      {\displaystyle (\mathbf {A} -\mathbf {BD} ^{-1}\mathbf {C} )^
      {-1}=\mathbf {A} ^{-1}+\mathbf {A} ^{-1}\mathbf {B} (\mathbf     ( 3 )
      {D} -\mathbf {CA} ^{-1}\mathbf {B} )^{-1}\mathbf {CA} ^{-        
      1}\,}  [(\mathbf {A} -\mathbf {BD} ^{-1}\mathbf {C} )^{-
      1}=\mathbf {A} ^{-1}+\mathbf {A} ^{-1}\mathbf {B} (\mathbf
      {D} -\mathbf {CA} ^{-1}\mathbf {B} )^{-1}\mathbf {CA} ^{-
      1}\,]
         (  A  &#x2212;   B D   &#x2212; 1    C   )  &#x2212; 1     B D
      &#x2212; 1   =   A   &#x2212; 1    B  (  D  &#x2212;   C A   &#x2212; 1
      B   )  &#x2212; 1      {\displaystyle (\mathbf {A} -\mathbf {BD} ^{-
      1}\mathbf {C} )^{-1}\mathbf {BD} ^{-1}=\mathbf {A} ^{-1}\mathbf {B}
      (\mathbf {D} -\mathbf {CA} ^{-1}\mathbf {B} )^{-1}\,}  [(\mathbf {A} -
      \mathbf {BD} ^{-1}\mathbf {C} )^{-1}\mathbf {BD} ^{-1}=\mathbf {A} ^{-
      1}\mathbf {B} (\mathbf {D} -\mathbf {CA} ^{-1}\mathbf {B} )^{-1}\,]
           D   &#x2212; 1    C  (  A  &#x2212;   B D   &#x2212; 1    C   )
      &#x2212; 1   = (  D  &#x2212;   C A   &#x2212; 1    B   )  &#x2212; 1
      C A   &#x2212; 1      {\displaystyle \mathbf {D} ^{-1}\mathbf {C}
      (\mathbf {A} -\mathbf {BD} ^{-1}\mathbf {C} )^{-1}=(\mathbf {D} -\mathbf
      {CA} ^{-1}\mathbf {B} )^{-1}\mathbf {CA} ^{-1}\,}  [\mathbf {D} ^{-
      1}\mathbf {C} (\mathbf {A} -\mathbf {BD} ^{-1}\mathbf {C} )^{-1}=(\mathbf
      {D} -\mathbf {CA} ^{-1}\mathbf {B} )^{-1}\mathbf {CA} ^{-1}\,]
           D   &#x2212; 1   +   D   &#x2212; 1    C  (  A  &#x2212;   B D
      &#x2212; 1    C   )  &#x2212; 1     B D   &#x2212; 1   = (  D  &#x2212;
      C A   &#x2212; 1    B   )  &#x2212; 1      {\displaystyle \mathbf {D} ^{-
      1}+\mathbf {D} ^{-1}\mathbf {C} (\mathbf {A} -\mathbf {BD} ^{-1}\mathbf
      {C} )^{-1}\mathbf {BD} ^{-1}=(\mathbf {D} -\mathbf {CA} ^{-1}\mathbf {B}
      )^{-1}\,}  [\mathbf {D} ^{-1}+\mathbf {D} ^{-1}\mathbf {C} (\mathbf {A} -
      \mathbf {BD} ^{-1}\mathbf {C} )^{-1}\mathbf {BD} ^{-1}=(\mathbf {D} -
      \mathbf {CA} ^{-1}\mathbf {B} )^{-1}\,]
where Equation (3) is the Woodbury_matrix_identity, which is equivalent to the
binomial_inverse_theorem.
Since a blockwise inversion of an n Ã n matrix requires inversion of two half-
sized matrices and 6 multiplications between two half-sized matrices, it can be
shown that a divide_and_conquer_algorithm that uses blockwise inversion to
invert a matrix runs with the same time complexity as the matrix multiplication
algorithm that is used internally.[9] There exist matrix_multiplication
algorithms with a complexity of O(n2.3727) operations, while the best proven
lower bound is Î©(n2 log n).[10]
This formula simplifies significantly when the upper right block matrix     B
{\displaystyle B}  [B] is the zero matrix. This formulation is useful when the
matrices     A   {\displaystyle A}  [A] and     D   {\displaystyle D}  [D] have
relatively simple inverse formulas (or pseudo_inverses in the case where the
blocks are not all square. In this special case, the block matrix inversion
formula stated in full generality above becomes
            [     A     0       C     D     ]    &#x2212; 1   =   [      A
      &#x2212; 1      0      &#x2212;   D   &#x2212; 1     C A   &#x2212; 1
      D   &#x2212; 1      ]   .   {\displaystyle {\begin{bmatrix}\mathbf {A}
      &\mathbf {0} \\\mathbf {C} &\mathbf {D} \end{bmatrix}}^{-1}={\begin
      {bmatrix}\mathbf {A} ^{-1}&\mathbf {0} \\-\mathbf {D} ^{-1}\mathbf {CA} ^
      {-1}&\mathbf {D} ^{-1}\end{bmatrix}}.}  [{\displaystyle {\begin
      {bmatrix}\mathbf {A} &\mathbf {0} \\\mathbf {C} &\mathbf {D} \end
      {bmatrix}}^{-1}={\begin{bmatrix}\mathbf {A} ^{-1}&\mathbf {0} \\-\mathbf
      {D} ^{-1}\mathbf {CA} ^{-1}&\mathbf {D} ^{-1}\end{bmatrix}}.}]
**** By Neumann series[edit] ****
If a matrix A has the property that
          lim  n &#x2192; &#x221E;   (  I  &#x2212;  A   )  n   = 0
      {\displaystyle \lim _{n\to \infty }(\mathbf {I} -\mathbf {A} )^{n}=0}
      [\lim _{n\to \infty }(\mathbf {I} -\mathbf {A} )^{n}=0]
then A is nonsingular and its inverse may be expressed by a Neumann_series:[11]
           A   &#x2212; 1   =  &#x2211;  n = 0   &#x221E;   (  I  &#x2212;  A
      )  n   .   {\displaystyle \mathbf {A} ^{-1}=\sum _{n=0}^{\infty }(\mathbf
      {I} -\mathbf {A} )^{n}.}  [\mathbf {A} ^{-1}=\sum _{n=0}^{\infty }
      (\mathbf {I} -\mathbf {A} )^{n}.]
Truncating the sum results in an "approximate" inverse which may be useful as a
preconditioner. Note that a truncated series can be accelerated exponentially
by noting that the Neumann series is a geometric_sum. As such, it satisfies
          &#x2211;  n = 0    2  L   &#x2212; 1   (  I  &#x2212;  A   )  n   =
      &#x220F;  l = 0   L &#x2212; 1   (  I  + (  I  &#x2212;  A   )   2  l
      )   {\displaystyle \sum _{n=0}^{2^{L}-1}(\mathbf {I} -\mathbf {A} )^
      {n}=\prod _{l=0}^{L-1}(\mathbf {I} +(\mathbf {I} -\mathbf {A} )^{2^{l}})}
      [\sum _{n=0}^{2^{L}-1}(\mathbf {I} -\mathbf {A} )^{n}=\prod _{l=0}^{L-1}
      (\mathbf {I} +(\mathbf {I} -\mathbf {A} )^{2^{l}})].
Therefore, only     2 L &#x2212; 2   {\displaystyle 2L-2}  [2L-2] matrix
multiplications are needed to compute      2  L     {\displaystyle 2^{L}}  [2^
{L}] terms of the sum.
More generally, if A is "near" the invertible matrix X in the sense that
          lim  n &#x2192; &#x221E;   (  I  &#x2212;   X   &#x2212; 1    A   )
      n   = 0  &#xA0; &#xA0; o r &#xA0; &#xA0;   lim  n &#x2192; &#x221E;
      (  I  &#x2212;  A    X   &#x2212; 1    )  n   = 0   {\displaystyle \lim _
      {n\to \infty }(\mathbf {I} -\mathbf {X} ^{-1}\mathbf {A} )^{n}=0\mathrm
      {~~or~~} \lim _{n\to \infty }(\mathbf {I} -\mathbf {A} \mathbf {X} ^{-
      1})^{n}=0}  [\lim _{n\to \infty }(\mathbf {I} -\mathbf {X} ^{-1}\mathbf
      {A} )^{n}=0\mathrm {~~or~~} \lim _{n\to \infty }(\mathbf {I} -\mathbf {A}
      \mathbf {X} ^{-1})^{n}=0]
then A is nonsingular and its inverse is
           A   &#x2212; 1   =  &#x2211;  n = 0   &#x221E;     (    X   &#x2212;
      1   (  X  &#x2212;  A  )  )   n     X   &#x2212; 1   &#xA0; .
      {\displaystyle \mathbf {A} ^{-1}=\sum _{n=0}^{\infty }\left(\mathbf {X} ^
      {-1}(\mathbf {X} -\mathbf {A} )\right)^{n}\mathbf {X} ^{-1}~.}  [\mathbf
      {A} ^{-1}=\sum _{n=0}^{\infty }\left(\mathbf {X} ^{-1}(\mathbf {X} -
      \mathbf {A} )\right)^{n}\mathbf {X} ^{-1}~.]
If it is also the case that A â X has rank 1 then this simplifies to
           A   &#x2212; 1   =   X   &#x2212; 1   &#x2212;      X   &#x2212; 1
      (  A  &#x2212;  X  )   X   &#x2212; 1     1 + tr &#x2061; (   X
      &#x2212; 1   (  A  &#x2212;  X  ) )    &#xA0; .   {\displaystyle \mathbf
      {A} ^{-1}=\mathbf {X} ^{-1}-{\frac {\mathbf {X} ^{-1}(\mathbf {A} -
      \mathbf {X} )\mathbf {X} ^{-1}}{1+\operatorname {tr} (\mathbf {X} ^{-1}
      (\mathbf {A} -\mathbf {X} ))}}~.}  [\mathbf {A} ^{-1}=\mathbf {X} ^{-1}-
      {\frac {\mathbf {X} ^{-1}(\mathbf {A} -\mathbf {X} )\mathbf {X} ^{-1}}
      {1+\operatorname {tr} (\mathbf {X} ^{-1}(\mathbf {A} -\mathbf {X} ))}}~.]
**** P-adic approximation[edit] ****
[[icon]] This section needs expansion. You can help by adding_to_it. (February
         2015)
If A is a matrix with integer or rational coefficients and we seek a solution
in arbitrary-precision rationals, then a p-adic approximation method converges
to an exact solution in     O (  n  4    log  2   &#x2061; n )   {\displaystyle
O(n^{4}\log ^{2}n)}  [O(n^{4}\log ^{2}n)], assuming standard     O (  n  3   )
{\displaystyle O(n^{3})}  [O(n^{3})] matrix multiplication is used.[12] The
method relies on solving n linear systems via Dixon's method of p-adic
approximation (each in     O (  n  3    log  2   &#x2061; n )   {\displaystyle
O(n^{3}\log ^{2}n)}  [O(n^{3}\log ^{2}n)]) and is available as such in software
specialized in arbitrary-precision matrix operations, for example, in IML.[13]
***** Derivative of the matrix inverse[edit] *****
Suppose that the invertible matrix A depends on a parameter t. Then the
derivative of the inverse of A with respect to t is given by
             d    A   &#x2212; 1      d  t    = &#x2212;   A   &#x2212; 1
      d   A     d  t      A   &#x2212; 1   .   {\displaystyle {\frac {\mathrm
      {d} \mathbf {A} ^{-1}}{\mathrm {d} t}}=-\mathbf {A} ^{-1}{\frac {\mathrm
      {d} \mathbf {A} }{\mathrm {d} t}}\mathbf {A} ^{-1}.}  [{\frac {\mathrm
      {d} \mathbf {A} ^{-1}}{\mathrm {d} t}}=-\mathbf {A} ^{-1}{\frac {\mathrm
      {d} \mathbf {A} }{\mathrm {d} t}}\mathbf {A} ^{-1}.]
To derive the above expression for the derivative of the inverse of A, one can
differentiate the definition of the matrix inverse       A   &#x2212; 1    A  =
I    {\displaystyle \mathbf {A} ^{-1}\mathbf {A} =\mathbf {I} }  [\mathbf {A} ^
{-1}\mathbf {A} =\mathbf {I} ] and then solve for the inverse of A:
             d    A   &#x2212; 1    A     d  t    =     d    A   &#x2212; 1
      d  t     A  +   A   &#x2212; 1       d   A     d  t    =     d   I     d
      t    =  0  .   {\displaystyle {\frac {\mathrm {d} \mathbf {A} ^{-
      1}\mathbf {A} }{\mathrm {d} t}}={\frac {\mathrm {d} \mathbf {A} ^{-1}}
      {\mathrm {d} t}}\mathbf {A} +\mathbf {A} ^{-1}{\frac {\mathrm {d} \mathbf
      {A} }{\mathrm {d} t}}={\frac {\mathrm {d} \mathbf {I} }{\mathrm {d}
      t}}=\mathbf {0} .}  [{\frac {\mathrm {d} \mathbf {A} ^{-1}\mathbf {A} }
      {\mathrm {d} t}}={\frac {\mathrm {d} \mathbf {A} ^{-1}}{\mathrm {d}
      t}}\mathbf {A} +\mathbf {A} ^{-1}{\frac {\mathrm {d} \mathbf {A} }
      {\mathrm {d} t}}={\frac {\mathrm {d} \mathbf {I} }{\mathrm {d}
      t}}=\mathbf {0} .]
Subtracting       A   &#x2212; 1       d   A     d  t      {\displaystyle
\mathbf {A} ^{-1}{\frac {\mathrm {d} \mathbf {A} }{\mathrm {d} t}}}  [\mathbf
{A} ^{-1}{\frac {\mathrm {d} \mathbf {A} }{\mathrm {d} t}}] from both sides of
the above and multiplying on the right by       A   &#x2212; 1
{\displaystyle \mathbf {A} ^{-1}}  [\mathbf {A} ^{-1}] gives the correct
expression for the derivative of the inverse:
             d    A   &#x2212; 1      d  t    = &#x2212;   A   &#x2212; 1
      d   A     d  t      A   &#x2212; 1   .   {\displaystyle {\frac {\mathrm
      {d} \mathbf {A} ^{-1}}{\mathrm {d} t}}=-\mathbf {A} ^{-1}{\frac {\mathrm
      {d} \mathbf {A} }{\mathrm {d} t}}\mathbf {A} ^{-1}.}  [{\frac {\mathrm
      {d} \mathbf {A} ^{-1}}{\mathrm {d} t}}=-\mathbf {A} ^{-1}{\frac {\mathrm
      {d} \mathbf {A} }{\mathrm {d} t}}\mathbf {A} ^{-1}.]
Similarly, if     &#x03F5;   {\displaystyle \epsilon }  [\epsilon ] is a small
number then
           (   A  + &#x03F5;  X   )   &#x2212; 1   =   A   &#x2212; 1
      &#x2212; &#x03F5;   A   &#x2212; 1    X    A   &#x2212; 1   +   O
      (  &#x03F5;  2   )  .   {\displaystyle \left(\mathbf {A} +\epsilon
      \mathbf {X} \right)^{-1}=\mathbf {A} ^{-1}-\epsilon \mathbf {A} ^{-
      1}\mathbf {X} \mathbf {A} ^{-1}+{\mathcal {O}}(\epsilon ^{2})\,.}  [\left
      (\mathbf {A} +\epsilon \mathbf {X} \right)^{-1}=\mathbf {A} ^{-1}-
      \epsilon \mathbf {A} ^{-1}\mathbf {X} \mathbf {A} ^{-1}+{\mathcal {O}}
      (\epsilon ^{2})\,.]
More generally, if
             d  f (  A  )    d  t    =  &#x2211;  i    g  i   (  A  )     d   A
      d  t     h  i   (  A  ) ,   {\displaystyle {\frac {\mathrm {d} f(\mathbf
      {A} )}{\mathrm {d} t}}=\sum _{i}g_{i}(\mathbf {A} ){\frac {\mathrm {d}
      \mathbf {A} }{\mathrm {d} t}}h_{i}(\mathbf {A} ),}  [{\displaystyle
      {\frac {\mathrm {d} f(\mathbf {A} )}{\mathrm {d} t}}=\sum _{i}g_{i}
      (\mathbf {A} ){\frac {\mathrm {d} \mathbf {A} }{\mathrm {d} t}}h_{i}
      (\mathbf {A} ),}]
then,
         f (  A  + &#x03F5;  X  ) = f (  A  ) + &#x03F5;  &#x2211;  i    g  i
      (  A  )  X   h  i   (  A  ) +   O   (  &#x03F5;  2   ) .   {\displaystyle
      f(\mathbf {A} +\epsilon \mathbf {X} )=f(\mathbf {A} )+\epsilon \sum _
      {i}g_{i}(\mathbf {A} )\mathbf {X} h_{i}(\mathbf {A} )+{\mathcal {O}}
      (\epsilon ^{2}).}  [{\displaystyle f(\mathbf {A} +\epsilon \mathbf {X}
      )=f(\mathbf {A} )+\epsilon \sum _{i}g_{i}(\mathbf {A} )\mathbf {X} h_{i}
      (\mathbf {A} )+{\mathcal {O}}(\epsilon ^{2}).}]
Given a positive integer     n   {\displaystyle n}  [n],
                 d    A   n      d  t       =  &#x2211;  i = 1   n     A   i
      &#x2212; 1       d   A     d  t      A   n &#x2212; i   ,         d    A
      &#x2212; n      d  t       = &#x2212;  &#x2211;  i = 1   n     A
      &#x2212; i       d   A     d  t      A   &#x2212; ( n + 1 &#x2212; i )
      .       {\displaystyle {\begin{aligned}{\frac {\mathrm {d} \mathbf {A} ^
      {n}}{\mathrm {d} t}}&=\sum _{i=1}^{n}\mathbf {A} ^{i-1}{\frac {\mathrm
      {d} \mathbf {A} }{\mathrm {d} t}}\mathbf {A} ^{n-i},\\{\frac {\mathrm {d}
      \mathbf {A} ^{-n}}{\mathrm {d} t}}&=-\sum _{i=1}^{n}\mathbf {A} ^{-i}
      {\frac {\mathrm {d} \mathbf {A} }{\mathrm {d} t}}\mathbf {A} ^{-(n+1-
      i)}.\end{aligned}}}  [{\displaystyle {\begin{aligned}{\frac {\mathrm {d}
      \mathbf {A} ^{n}}{\mathrm {d} t}}&=\sum _{i=1}^{n}\mathbf {A} ^{i-1}
      {\frac {\mathrm {d} \mathbf {A} }{\mathrm {d} t}}\mathbf {A} ^{n-i},\\
      {\frac {\mathrm {d} \mathbf {A} ^{-n}}{\mathrm {d} t}}&=-\sum _{i=1}^
      {n}\mathbf {A} ^{-i}{\frac {\mathrm {d} \mathbf {A} }{\mathrm {d}
      t}}\mathbf {A} ^{-(n+1-i)}.\end{aligned}}}]
Therefore,
             (  A  + &#x03F5;  X   )  n      =   A   n   + &#x03F5;  &#x2211;
      i = 1   n     A   i &#x2212; 1    X    A   n &#x2212; i   +   O
      (  &#x03F5;  2   ) ,     (  A  + &#x03F5;  X   )  &#x2212; n      =   A
      &#x2212; n   &#x2212; &#x03F5;  &#x2211;  i = 1   n     A   &#x2212; i
      X    A   &#x2212; ( n + 1 &#x2212; i )   +   O   (  &#x03F5;  2   ) .
      {\displaystyle {\begin{aligned}(\mathbf {A} +\epsilon \mathbf {X} )^
      {n}&=\mathbf {A} ^{n}+\epsilon \sum _{i=1}^{n}\mathbf {A} ^{i-1}\mathbf
      {X} \mathbf {A} ^{n-i}+{\mathcal {O}}(\epsilon ^{2}),\\(\mathbf {A}
      +\epsilon \mathbf {X} )^{-n}&=\mathbf {A} ^{-n}-\epsilon \sum _{i=1}^
      {n}\mathbf {A} ^{-i}\mathbf {X} \mathbf {A} ^{-(n+1-i)}+{\mathcal {O}}
      (\epsilon ^{2}).\end{aligned}}}  [{\displaystyle {\begin{aligned}(\mathbf
      {A} +\epsilon \mathbf {X} )^{n}&=\mathbf {A} ^{n}+\epsilon \sum _{i=1}^
      {n}\mathbf {A} ^{i-1}\mathbf {X} \mathbf {A} ^{n-i}+{\mathcal {O}}
      (\epsilon ^{2}),\\(\mathbf {A} +\epsilon \mathbf {X} )^{-n}&=\mathbf {A}
      ^{-n}-\epsilon \sum _{i=1}^{n}\mathbf {A} ^{-i}\mathbf {X} \mathbf {A} ^
      {-(n+1-i)}+{\mathcal {O}}(\epsilon ^{2}).\end{aligned}}}]
***** Generalized inverse[edit] *****
Some of the properties of inverse matrices are shared by generalized_inverses
(for example, the MooreâPenrose_inverse), which can be defined for any m-by-
n matrix.
***** Applications[edit] *****
For most practical applications, it is not necessary to invert a matrix to
solve a system_of_linear_equations; however, for a unique solution, it is
necessary that the matrix involved be invertible.
Decomposition techniques like LU_decomposition are much faster than inversion,
and various fast algorithms for special classes of linear systems have also
been developed.
**** Regression/least_squares[edit] ****
Although an explicit inverse is not necessary to estimate the vector of
unknowns, it is the easiest way to estimate their accuracy, found in the
diagonal of a matrix inverse (the posterior covariance matrix of the vector of
unknowns). However, faster algorithms to compute only the diagonal entries of a
matrix inverse are known in many cases.[14]
**** Matrix inverses in real-time simulations[edit] ****
Matrix inversion plays a significant role in computer_graphics, particularly in
3D_graphics rendering and 3D simulations. Examples include screen-to-world ray
casting, world-to-subspace-to-world object transformations, and physical
simulations.
**** Matrix inverses in MIMO wireless communication[edit] ****
Matrix inversion also plays a significant role in the MIMO (Multiple-Input,
Multiple-Output) technology in wireless communications. The MIMO system
consists of N transmit and M receive antennas. Unique signals, occupying the
same frequency band, are sent via N transmit antennas and are received via M
receive antennas. The signal arriving at each receive antenna will be a linear
combination of the N transmitted signals forming a NxM transmission matrix H.
It is crucial for the matrix H to be invertible for the receiver to be able to
figure out the transmitted information.
***** See also[edit] *****
    * Binomial_inverse_theorem
    * LU_decomposition
    * Matrix_decomposition
    * Matrix_square_root
    * Pseudoinverse
    * Singular_value_decomposition
    * Woodbury_matrix_identity
***** Notes[edit] *****
   1. ^Horn, Roger A.; Johnson, Charles R. (1985). Matrix Analysis. Cambridge
      University_Press. p. 14. ISBN 978-0-521-38632-6.
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
   3. .
   4. ^Pan, Victor; Reif, John (1985), Efficient Parallel Solution of Linear
      Systems, Proceedings of the 17th Annual ACM Symposium on Theory of
      Computing, Providence: ACM
   5. ^ Pan, Victor; Reif, John (1985), Harvard University Center for Research
      in Computing Technology Report TR-02-85, Cambridge, MA: Aiken_Computation
      Laboratory
   6. ^"The Inversion of Large Matrices". Byte_Magazine. 11 (4): 181â190.
      April 1986.
   7. ^ A proof can be found in the Appendix B ofKondratyuk, L. A.;
      Krivoruchenko, M. I. (1992). "Superconducting_quark_matter_in_SU(2)_color
      group". Zeitschrift fÃ¼r Physik A. 344: 99â115. doi:10.1007/BF01291027.
   8. ^Strang, Gilbert (2003). Introduction_to_linear_algebra (3rd ed.). SIAM.
      p. 71. ISBN 978-0-9614088-9-3.
   9. , Chapter_2,_page_71
  10. ^ Bernstein, Dennis (2005). Matrix Mathematics. Princeton University
      Press. p. 44. ISBN 978-0-691-11802-4.
  11. ^ Bernstein, Dennis (2005). Matrix Mathematics. Princeton University
      Press. p. 45. ISBN 978-0-691-11802-4.
  12. ^ T. H. Cormen, C. E. Leiserson, R. L. Rivest, C. Stein, Introduction to
      Algorithms, 3rd ed., MIT Press, Cambridge, MA, 2009, Â§28.2.
  13. ^ Ran_Raz. On the complexity of matrix product. In Proceedings of the
      thirty-fourth annual ACM symposium on Theory of computing. ACM Press,
      2002. doi:10.1145/509907.509932.
  14. ^ Stewart, Gilbert (1998). Matrix Algorithms: Basic decompositions. SIAM.
      p. 55. ISBN 978-0-89871-414-2.
  15. ^Haramoto, H.; Matsumoto, M. (2009). "A p-adic algorithm for computing
      the inverse of integer matrices". Journal of Computational and Applied
      Mathematics. 225: 320â322. doi:10.1016/j.cam.2008.07.044.
  16. ^"IML_-_Integer_Matrix_Library". cs.uwaterloo.ca. Retrieved 14 April
      2018.
  17. ^ Lin Lin, Jianfeng Lu, Lexing Ying, Roberto Car, and Weinan E, "Fast
      algorithm_for_extracting_the_diagonal_of_the_inverse_matrix_with
      application_to_the_electronic_structure_analysis_of_metallic_systems,"
      *Communications in Mathematical Sciences* vol. 7, pp. 755â777 (doi:
      10.4310/CMS.2009.v7.n3.a12).
***** References[edit] *****
    * Cormen,_Thomas_H.; Leiserson,_Charles_E.; Rivest,_Ronald_L.; Stein,
      Clifford (2001) [1990]. "28.4: Inverting matrices". Introduction_to
      Algorithms (2nd ed.). MIT Press and McGraw-Hill. pp. 755â760. ISBN 0-
      262-03293-7.
***** Further reading[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Inversion_of_a_matrix",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Matrix_Mathematics:_Theory,_Facts,_and_Formulas at Google_books
The_Matrix_Cookbook
***** External links[edit] *****
 This article's use of external_links may not follow Wikipedia's policies or
 guidelines. Please improve_this_article by removing excessive or inappropriate
 external links, and converting useful links where appropriate into footnote
 references. (June 2015)(Learn_how_and_when_to_remove_this_template_message)
    * Lecture_on_Inverse_Matrices_by_Khan_Academy
    * Linear_Algebra_Lecture_on_Inverse_Matrices_by_MIT
    * LAPACK – a collection of FORTRAN subroutines for solving dense linear
      algebra problems
    * ALGLIB – includes a partial port of the LAPACK to C++, C#, Delphi, etc.
    * Online_Inverse_Matrix_Calculator_using_AJAX
    * Symbolic_Inverse_of_Matrix_Calculator_with_steps_shown
    * Moore-Penrose_Pseudo-Inverse_Matrix
    * Inverse_of_a_Matrix_Notes
    * Calculator_for_Singular_or_Non-Square_Matrix_Inverse
    * Inverse_calculator_online
    * "Derivative_of_inverse_matrix". PlanetMath.
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

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Invertible_matrix&oldid=908401118"
Categories:
    * Linear_algebra
    * Matrices
    * Determinants
    * Matrix_theory
Hidden categories:
    * Articles_lacking_in-text_citations_from_June_2018
    * All_articles_lacking_in-text_citations
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_December_2009
    * Articles_to_be_expanded_from_February_2015
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
    * Wikipedia_external_links_cleanup_from_June_2015
    * Wikipedia_spam_cleanup_from_June_2015
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Lumbaart
    * Magyar
    * æ¥æ¬èª
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 29 July 2019, at 13:50 (UTC).
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
