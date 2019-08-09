The following text has been accessed from https://en.wikipedia.org/wiki/Cayley%E2%80%93Hamilton_theorem at Thu Aug 8 23:59:46 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** CayleyâHamilton theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Arthur_Cayley, F.R.S. (1821â1895) is widely regarded as Britain's leading
pure mathematician of the 19th century. Cayley in 1848 went to Dublin to attend
lectures on quaternions by Hamilton, their discoverer. Later Cayley impressed
him by being the second to publish work on them.[1] Cayley proved the theorem
for matrices of dimension 3 and less, publishing proof for the two-dimensional
case.[2][3] As for n Ã n matrices, Cayley stated â..., I have not thought it
necessary to undertake the labor of a formal proof of the theorem in the
general case of a matrix of any degreeâ.
William_Rowan_Hamilton (1805â1865), Irish physicist, astronomer, and
mathematician, first foreign member of the American National_Academy_of
Sciences. While maintaining opposing position about how geometry should be
studied, Hamilton always remained on the best terms with Cayley.[1]

Hamilton proved that for a linear function of quaternions there exists a
certain equation, depending on the linear function, that is satisfied by the
linear function itself.[4][5][6]
In linear_algebra, the CayleyâHamilton theorem (named after the
mathematicians Arthur_Cayley and William_Rowan_Hamilton) states that every
square_matrix over a commutative_ring (such as the real or complex field)
satisfies its own characteristic_equation.
If A is a given n×n matrix and In  is the n×n identity_matrix, then the
characteristic_polynomial of A is defined as[7]
               p ( &#x03BB; ) = det ( &#x03BB;  I  n   &#x2212; A ) &#xA0; ,
            {\displaystyle p(\lambda )=\det(\lambda I_{n}-A)~,}  [p(\lambda
            )=\det(\lambda I_{n}-A)~,]
where det is the determinant operation and Î» is a scalar element of the base
ring. Since the entries of the matrix are (linear or constant) polynomials in
Î», the determinant is also an n-th order monic_polynomial in Î». The
CayleyâHamilton theorem states that if one defines an analogous matrix
equation, p(A), consisting of the replacement of the scalar eigenvalues Î» with
the matrix A, then this polynomial in the matrix A results in the zero_matrix,
               p ( A ) = 0.   {\displaystyle p(A)=0.}  [p(A)=0.]
The powers of A, obtained by substitution from powers of Î», are defined by
repeated matrix multiplication; the constant term of  p(Î») gives a multiple of
the power A0, which is defined as the identity matrix. The theorem allows An to
be expressed as a linear combination of the lower matrix powers of A. When the
ring is a field, the CayleyâHamilton theorem is equivalent to the statement
that the minimal_polynomial of a square matrix divides its characteristic
polynomial.
The theorem was first proved in 1853[8] in terms of inverses of linear
functions of quaternions, a non-commutative ring, by Hamilton.[4][5][6] This
corresponds to the special case of certain 4 Ã 4 real or 2 Ã 2 complex
matrices. The theorem holds for general quaternionic matrices.[9][nb_1] Cayley
in 1858 stated it for 3 Ã 3 and smaller matrices, but only published a proof
for the 2 Ã 2 case.[2] The general case was first proved by Frobenius in 1878.
[10]
⁰
***** Contents *****
    * 1_Examples
          o 1.1_1Ã1_matrices
          o 1.2_2Ã2_matrices
    * 2_Applications
          o 2.1_Determinant_and_inverse_matrix
          o 2.2_n-th_Power_of_matrix
          o 2.3_Matrix_functions
          o 2.4_Algebraic_number_theory
    * 3_Proving_the_theorem_in_general
          o 3.1_Preliminaries
                # 3.1.1_Adjugate_matrices
          o 3.2_A_direct_algebraic_proof
          o 3.3_A_proof_using_polynomials_with_matrix_coefficients
          o 3.4_A_synthesis_of_the_first_two_proofs
          o 3.5_A_proof_using_matrices_of_endomorphisms
          o 3.6_A_bogus_"proof":_p(A)_=_det(AIn â A)_=_det(A â A)_=_0
    * 4_Proofs_using_methods_of_abstract_algebra
    * 5_Abstraction_and_generalizations
    * 6_See_also
    * 7_Remarks
    * 8_Notes
    * 9_References
    * 10_External_links
***** Examples[edit] *****
**** 1Ã1 matrices[edit] ****
For a 1Ã1 matrix A = (a1,1), the characteristic polynomial is given by p
(Î») = Î» â a, and so p(A) = (a) â a1,1 = 0 is obvious.
**** 2Ã2 matrices[edit] ****
As a concrete example, let
         A =   (    1   2     3   4    )   .   {\displaystyle A={\begin
      {pmatrix}1&2\\3&4\end{pmatrix}}.}  [{\displaystyle A={\begin
      {pmatrix}1&2\\3&4\end{pmatrix}}.}]
Its characteristic polynomial is given by
         p ( &#x03BB; ) = det ( &#x03BB;  I  2   &#x2212; A ) = det
      (    &#x03BB; &#x2212; 1   &#x2212; 2     &#x2212; 3   &#x03BB; &#x2212;
      4    )   = ( &#x03BB; &#x2212; 1 ) ( &#x03BB; &#x2212; 4 ) &#x2212;
      ( &#x2212; 2 ) ( &#x2212; 3 ) =  &#x03BB;  2   &#x2212; 5 &#x03BB;
      &#x2212; 2.   {\displaystyle p(\lambda )=\det(\lambda I_{2}-A)=\det
      {\begin{pmatrix}\lambda -1&-2\\-3&\lambda -4\end{pmatrix}}=(\lambda -1)
      (\lambda -4)-(-2)(-3)=\lambda ^{2}-5\lambda -2.}  [p(\lambda )=\det
      (\lambda I_{2}-A)=\det {\begin{pmatrix}\lambda -1&-2\\-3&\lambda -4\end
      {pmatrix}}=(\lambda -1)(\lambda -4)-(-2)(-3)=\lambda ^{2}-5\lambda -2.]
The CayleyâHamilton theorem claims that, if we define
         p ( X ) =  X  2   &#x2212; 5 X &#x2212; 2  I  2   ,   {\displaystyle p
      (X)=X^{2}-5X-2I_{2},}  [p(X)=X^{2}-5X-2I_{2},]
then
         p ( A ) =  A  2   &#x2212; 5 A &#x2212; 2  I  2   =   (    0   0     0
      0    )   .   {\displaystyle p(A)=A^{2}-5A-2I_{2}={\begin
      {pmatrix}0&0\\0&0\\\end{pmatrix}}.}  [p(A)=A^{2}-5A-2I_{2}={\begin
      {pmatrix}0&0\\0&0\\\end{pmatrix}}.]
We can verify by computation that indeed,
          A  2   &#x2212; 5 A &#x2212; 2  I  2   =   (    7   10     15   22
      )   &#x2212;   (    5   10     15   20    )   &#x2212;   (    2   0     0
      2    )   =   (    0   0     0   0    )   .   {\displaystyle A^{2}-5A-2I_
      {2}={\begin{pmatrix}7&10\\15&22\\\end{pmatrix}}-{\begin
      {pmatrix}5&10\\15&20\\\end{pmatrix}}-{\begin{pmatrix}2&0\\0&2\\\end
      {pmatrix}}={\begin{pmatrix}0&0\\0&0\\\end{pmatrix}}.}  [A^{2}-5A-2I_{2}=
      {\begin{pmatrix}7&10\\15&22\\\end{pmatrix}}-{\begin
      {pmatrix}5&10\\15&20\\\end{pmatrix}}-{\begin{pmatrix}2&0\\0&2\\\end
      {pmatrix}}={\begin{pmatrix}0&0\\0&0\\\end{pmatrix}}.]
For a generic 2Ã2 matrix,
         A =   (    a   b     c   d    )   ,   {\displaystyle A={\begin
      {pmatrix}a&b\\c&d\\\end{pmatrix}},}  [A={\begin{pmatrix}a&b\\c&d\\\end
      {pmatrix}},]
the characteristic polynomial is given by  p(Î») = Î»2 â (a + d)Î» + 
(ad â bc), so the CayleyâHamilton theorem states that
         p ( A ) =  A  2   &#x2212; ( a + d ) A + ( a d &#x2212; b c )  I  2
      =   (    0   0     0   0    )   ;   {\displaystyle p(A)=A^{2}-(a+d)A+(ad-
      bc)I_{2}={\begin{pmatrix}0&0\\0&0\\\end{pmatrix}};}  [p(A)=A^{2}-(a+d)A+
      (ad-bc)I_{2}={\begin{pmatrix}0&0\\0&0\\\end{pmatrix}};]
which is indeed always the case, evident by working out the entries of A2.
***** Applications[edit] *****
**** Determinant and inverse matrix[edit] ****
See also: Determinant_Â§ Relation_to_eigenvalues_and_trace, and Characteristic
polynomial_Â§ Properties
For a general nÃn invertible_matrix A, i.e., one with nonzero determinant,
Aâ1 can thus be written as an (n â 1)-th order polynomial_expression in A:
As indicated, the CayleyâHamilton theorem amounts to the identity
   p ( A ) =  A  n   +  c  n &#x2212; 1    A  n &#x2212; 1   + &#x22EF; +  c  1
A + ( &#x2212; 1  )  n   det ( A )  I  n   = O .   {\displaystyle p(A)=A^{n}+c_
{n-1}A^{n-1}+\cdots +c_{1}A+(-1)^{n}\det(A)I_{n}=O.}  [{\displaystyle p(A)=A^
{n}+c_{n-1}A^{n-1}+\cdots +c_{1}A+(-1)^{n}\det(A)I_{n}=O.}]
The coefficients ci are given by the elementary_symmetric_polynomials of the
eigenvalues of A. Using Newton_identities, the elementary symmetric polynomials
can in turn be expressed in terms of power_sum_symmetric_polynomials of the
eigenvalues:
          s  k   =  &#x2211;  i = 1   n    &#x03BB;  i   k   = tr &#x2061; (  A
      k   ) ,   {\displaystyle s_{k}=\sum _{i=1}^{n}\lambda _{i}^
      {k}=\operatorname {tr} (A^{k}),}  [{\displaystyle s_{k}=\sum _{i=1}^
      {n}\lambda _{i}^{k}=\operatorname {tr} (A^{k}),}]
where tr (Ak) is the trace of the matrix Ak. Thus, we can express ci in terms
of the trace of powers of A.
In general, the formula for the coefficients ci is given in terms of complete
exponential Bell_polynomials as [nb_2]
          c  n &#x2212; k   =    ( &#x2212; 1  )  k     k !     B  k   (  s  1
      , &#x2212; 1 !  s  2   , 2 !  s  3   , &#x2026; , ( &#x2212; 1  )  k
      &#x2212; 1   ( k &#x2212; 1 ) !  s  k   ) .   {\displaystyle c_{n-k}=
      {\frac {(-1)^{k}}{k!}}B_{k}(s_{1},-1!s_{2},2!s_{3},\ldots ,(-1)^{k-1}(k-
      1)!s_{k}).}  [{\displaystyle c_{n-k}={\frac {(-1)^{k}}{k!}}B_{k}(s_{1},-
      1!s_{2},2!s_{3},\ldots ,(-1)^{k-1}(k-1)!s_{k}).}]
In particular, the determinant of A corresponds to c0. Thus, the determinant
can be written as a trace_identity
         det ( A ) =   1  n !     B  n   (  s  1   , &#x2212; 1 !  s  2   , 2 !
      s  3   , &#x2026; , ( &#x2212; 1  )  n &#x2212; 1   ( n &#x2212; 1 ) !  s
      n   ) .   {\displaystyle \det(A)={\frac {1}{n!}}B_{n}(s_{1},-1!s_{2},2!s_
      {3},\ldots ,(-1)^{n-1}(n-1)!s_{n}).}  [{\displaystyle \det(A)={\frac {1}
      {n!}}B_{n}(s_{1},-1!s_{2},2!s_{3},\ldots ,(-1)^{n-1}(n-1)!s_{n}).}]
Likewise, the characteristic polynomial can be written as
         &#x2212; ( &#x2212; 1  )  n   det ( A )  I  n   = A (  A  n &#x2212; 1
      +  c  n &#x2212; 1    A  n &#x2212; 2   + &#x22EF; +  c  1    I  n   ) ,
      {\displaystyle -(-1)^{n}\det(A)I_{n}=A(A^{n-1}+c_{n-1}A^{n-2}+\cdots +c_
      {1}I_{n}),}  [-(-1)^{n}\det(A)I_{n}=A(A^{n-1}+c_{n-1}A^{n-2}+\cdots +c_
      {1}I_{n}),]
and, by multiplying both sides by Aâ1 (note â(â1)n = (â1)nâ1), one is
led to an expression for the inverse of A as a trace identity,
              A  &#x2212; 1      =    ( &#x2212; 1  )  n &#x2212; 1     det A
      (  A  n &#x2212; 1   +  c  n &#x2212; 1    A  n &#x2212; 2   + &#x22EF; +
      c  1    I  n   ) ,       =   1  det A     &#x2211;  k = 0   n &#x2212; 1
      ( &#x2212; 1  )  n + k &#x2212; 1      A  n &#x2212; k &#x2212; 1    k !
      B  k   (  s  1   , &#x2212; 1 !  s  2   , 2 !  s  3   , &#x2026; ,
      ( &#x2212; 1  )  k &#x2212; 1   ( k &#x2212; 1 ) !  s  k   ) .
      {\displaystyle {\begin{aligned}A^{-1}&={\frac {(-1)^{n-1}}{\det A}}(A^{n-
      1}+c_{n-1}A^{n-2}+\cdots +c_{1}I_{n}),\\[5pt]&={\frac {1}{\det A}}\sum _
      {k=0}^{n-1}(-1)^{n+k-1}{\frac {A^{n-k-1}}{k!}}B_{k}(s_{1},-1!s_{2},2!s_
      {3},\ldots ,(-1)^{k-1}(k-1)!s_{k}).\end{aligned}}}  [{\displaystyle
      {\begin{aligned}A^{-1}&={\frac {(-1)^{n-1}}{\det A}}(A^{n-1}+c_{n-1}A^{n-
      2}+\cdots +c_{1}I_{n}),\\[5pt]&={\frac {1}{\det A}}\sum _{k=0}^{n-1}(-1)^
      {n+k-1}{\frac {A^{n-k-1}}{k!}}B_{k}(s_{1},-1!s_{2},2!s_{3},\ldots ,(-1)^
      {k-1}(k-1)!s_{k}).\end{aligned}}}]
For instance, the first few Bell polynomials are B0 = 1, B1(x1) = x1, B2(x1,
x2) = x2
1 + x2, and B3(x1, x2, x3) = x3
1 + 3 x1x2 + x3.
Using these to specify the coefficients ci of the characteristic polynomial of
a 2Ã2 matrix yields
              c  2   =  B  0   = 1 ,      c  1   =    &#x2212; 1   1 !     B  1
      (  s  1   ) = &#x2212;  s  1   = &#x2212; tr &#x2061; ( A ) ,      c  0
      =   1  2 !     B  2   (  s  1   , &#x2212; 1 !  s  2   ) =   1 2   (  s
      1   2   &#x2212;  s  2   ) =   1 2   ( ( tr &#x2061; ( A )  )  2
      &#x2212; tr &#x2061; (  A  2   ) ) .       {\displaystyle {\begin
      {aligned}c_{2}=B_{0}=1,\\[4pt]c_{1}={\frac {-1}{1!}}B_{1}(s_{1})=-s_{1}=-
      \operatorname {tr} (A),\\[4pt]c_{0}={\frac {1}{2!}}B_{2}(s_{1},-1!s_{2})=
      {\frac {1}{2}}(s_{1}^{2}-s_{2})={\frac {1}{2}}((\operatorname {tr} (A))^
      {2}-\operatorname {tr} (A^{2})).\end{aligned}}}  [{\displaystyle {\begin
      {aligned}c_{2}=B_{0}=1,\\[4pt]c_{1}={\frac {-1}{1!}}B_{1}(s_{1})=-s_{1}=-
      \operatorname {tr} (A),\\[4pt]c_{0}={\frac {1}{2!}}B_{2}(s_{1},-1!s_{2})=
      {\frac {1}{2}}(s_{1}^{2}-s_{2})={\frac {1}{2}}((\operatorname {tr} (A))^
      {2}-\operatorname {tr} (A^{2})).\end{aligned}}}]
The coefficient c0 gives the determinant of the 2Ã2 matrix, c1 minus its
trace, while its inverse is given by
          A  &#x2212; 1   =    &#x2212; 1   det A    ( A +  c  1    I  2   ) =
      &#x2212; 2 ( A &#x2212; tr &#x2061; ( A )  I  2   )   ( tr &#x2061; ( A )
      )  2   &#x2212; tr &#x2061; (  A  2   )    .   {\displaystyle A^{-1}=
      {\frac {-1}{\det A}}(A+c_{1}I_{2})={\frac {-2(A-\operatorname {tr} (A)I_
      {2})}{(\operatorname {tr} (A))^{2}-\operatorname {tr} (A^{2})}}.}  [
      {\displaystyle A^{-1}={\frac {-1}{\det A}}(A+c_{1}I_{2})={\frac {-2(A-
      \operatorname {tr} (A)I_{2})}{(\operatorname {tr} (A))^{2}-\operatorname
      {tr} (A^{2})}}.}]
It is apparent from the general formula for cn-k, expressed in terms of Bell
polynomials, that the expressions
         &#x2212; tr &#x2061; ( A )   and      1 2    ( tr &#x2061; ( A  )  2
      &#x2212; tr &#x2061; (  A  2   ) )   {\displaystyle -\operatorname {tr}
      (A)\quad {\text{and}}\quad {\tfrac {1}{2}}(\operatorname {tr} (A)^{2}-
      \operatorname {tr} (A^{2}))}  [{\displaystyle -\operatorname {tr}
      (A)\quad {\text{and}}\quad {\tfrac {1}{2}}(\operatorname {tr} (A)^{2}-
      \operatorname {tr} (A^{2}))}]
always give the coefficients cnâ1 of Î»nâ1 and cnâ2 of Î»nâ2 in the
characteristic polynomial of any nÃn matrix, respectively. So, for a 3Ã3
matrix A, the statement of the CayleyâHamilton theorem can also be written as
          A  3   &#x2212; ( tr &#x2061; A )  A  2   +   1 2    (  ( tr &#x2061;
      A  )  2   &#x2212; tr &#x2061; (  A  2   )  )  A &#x2212; det ( A )  I  3
      = O ,   {\displaystyle A^{3}-(\operatorname {tr} A)A^{2}+{\frac {1}
      {2}}\left((\operatorname {tr} A)^{2}-\operatorname {tr} (A^{2})\right)A-
      \det(A)I_{3}=O,}  [{\displaystyle A^{3}-(\operatorname {tr} A)A^{2}+
      {\frac {1}{2}}\left((\operatorname {tr} A)^{2}-\operatorname {tr} (A^
      {2})\right)A-\det(A)I_{3}=O,}]
where the right-hand side designates a 3Ã3 matrix with all entries reduced to
zero. Likewise, this determinant in the n = 3 case, is now
             det ( A )    =   1  3 !     B  3   (  s  1   , &#x2212; 1 !  s  2
      , 2 !  s  3   ) =   1 6   (  s  1   3   + 3  s  1   ( &#x2212;  s  2   )
      + 2  s  3   )       =    1 6     (  ( tr &#x2061; A  )  3   &#x2212; 3 tr
      &#x2061; (  A  2   ) ( tr &#x2061; A ) + 2 tr &#x2061; (  A  3   )  )  .
      {\displaystyle {\begin{aligned}\det(A)&={\frac {1}{3!}}B_{3}(s_{1},-1!s_
      {2},2!s_{3})={\frac {1}{6}}(s_{1}^{3}+3s_{1}(-s_{2})+2s_{3})\\[5pt]&=
      {\tfrac {1}{6}}\left((\operatorname {tr} A)^{3}-3\operatorname {tr} (A^
      {2})(\operatorname {tr} A)+2\operatorname {tr} (A^{3})\right).\end
      {aligned}}}  [{\displaystyle {\begin{aligned}\det(A)&={\frac {1}{3!}}B_
      {3}(s_{1},-1!s_{2},2!s_{3})={\frac {1}{6}}(s_{1}^{3}+3s_{1}(-s_{2})+2s_
      {3})\\[5pt]&={\tfrac {1}{6}}\left((\operatorname {tr} A)^{3}-
      3\operatorname {tr} (A^{2})(\operatorname {tr} A)+2\operatorname {tr} (A^
      {3})\right).\end{aligned}}}]
This expression gives the negative of coefficient cnâ3 of Î»nâ3 in the
general case, as seen below.
Similarly, one can write for a 4Ã4 matrix A,
          A  4   &#x2212; ( tr &#x2061; A )  A  3   +    1 2      (   ( tr
      &#x2061; A  )  2   &#x2212; tr &#x2061; (  A  2   )   )    A  2
      &#x2212;    1 6      (   ( tr &#x2061; A  )  3   &#x2212; 3 tr &#x2061;
      (  A  2   ) ( tr &#x2061; A ) + 2 tr &#x2061; (  A  3   )   )   A + det
      ( A )  I  4   = O ,   {\displaystyle A^{4}-(\operatorname {tr} A)A^{3}+
      {\tfrac {1}{2}}{\bigl (}(\operatorname {tr} A)^{2}-\operatorname {tr} (A^
      {2}){\bigr )}A^{2}-{\tfrac {1}{6}}{\bigl (}(\operatorname {tr} A)^{3}-
      3\operatorname {tr} (A^{2})(\operatorname {tr} A)+2\operatorname {tr} (A^
      {3}){\bigr )}A+\det(A)I_{4}=O,}  [{\displaystyle A^{4}-(\operatorname
      {tr} A)A^{3}+{\tfrac {1}{2}}{\bigl (}(\operatorname {tr} A)^{2}-
      \operatorname {tr} (A^{2}){\bigr )}A^{2}-{\tfrac {1}{6}}{\bigl (}
      (\operatorname {tr} A)^{3}-3\operatorname {tr} (A^{2})(\operatorname {tr}
      A)+2\operatorname {tr} (A^{3}){\bigr )}A+\det(A)I_{4}=O,}]
where, now, the determinant is cnâ4,
            1 24     (  ( tr &#x2061; A  )  4   &#x2212; 6 tr &#x2061; (  A  2
      ) ( tr &#x2061; A  )  2   + 3 ( tr &#x2061; (  A  2   )  )  2   + 8 tr
      &#x2061; (  A  3   ) tr &#x2061; ( A ) &#x2212; 6 tr &#x2061; (  A  4   )
      )  ,   {\displaystyle {\tfrac {1}{24}}\left((\operatorname {tr} A)^{4}-
      6\operatorname {tr} (A^{2})(\operatorname {tr} A)^{2}+3(\operatorname
      {tr} (A^{2}))^{2}+8\operatorname {tr} (A^{3})\operatorname {tr} (A)-
      6\operatorname {tr} (A^{4})\right),}  [{\displaystyle {\tfrac {1}
      {24}}\left((\operatorname {tr} A)^{4}-6\operatorname {tr} (A^{2})
      (\operatorname {tr} A)^{2}+3(\operatorname {tr} (A^{2}))^
      {2}+8\operatorname {tr} (A^{3})\operatorname {tr} (A)-6\operatorname {tr}
      (A^{4})\right),}]
and so on for larger matrices. The increasingly complex expressions for the
coefficients ck is deducible from Newton's_identities or the
FaddeevâLeVerrier_algorithm.
Another method for obtaining these coefficients ck for a general nÃn matrix,
provided no root be zero, relies on the following alternative expression_for
the_determinant,
         p ( &#x03BB; ) = det ( &#x03BB;  I  n   &#x2212; A ) =  &#x03BB;  n
      exp &#x2061; ( tr &#x2061; ( log &#x2061; (  I  n   &#x2212; A  /
      &#x03BB; ) ) ) .   {\displaystyle p(\lambda )=\det(\lambda I_{n}-
      A)=\lambda ^{n}\exp(\operatorname {tr} (\log(I_{n}-A/\lambda ))).}  [
      {\displaystyle p(\lambda )=\det(\lambda I_{n}-A)=\lambda ^{n}\exp
      (\operatorname {tr} (\log(I_{n}-A/\lambda ))).}]
Hence, by virtue of the Mercator_series,
         p ( &#x03BB; ) =  &#x03BB;  n   exp &#x2061;  (  &#x2212; tr &#x2061;
      &#x2211;  m = 1   &#x221E;      (   A &#x03BB;    )  m    m    )  ,
      {\displaystyle p(\lambda )=\lambda ^{n}\exp \left(-\operatorname {tr}
      \sum _{m=1}^{\infty }{({A \over \lambda })^{m} \over m}\right),}  [p
      (\lambda )=\lambda ^{n}\exp \left(-\operatorname {tr} \sum _{m=1}^{\infty
      }{({A \over \lambda })^{m} \over m}\right),]
where the exponential only needs be expanded to order Î»ân, since p(Î») is of
order n, the net negative powers of Î» automatically vanishing by the CâH
theorem. (Again, this requires a ring containing the rational numbers.) The
coefficients of Î» can be directly written in terms of complete Bell
polynomials by comparing this expression with the generating function of the
Bell polynomial.
Differentiation of this expression with respect to Î» allows determination of
the generic coefficients of the characteristic polynomial for general n, as
determinants of mÃm matrices,[nb_3]
          c  n &#x2212; m   =    ( &#x2212; 1  )  m     m !      |    tr
      &#x2061; A   m &#x2212; 1   0   &#x22EF;     tr &#x2061;  A  2     tr
      &#x2061; A   m &#x2212; 2   &#x22EF;     &#x22EE;   &#x22EE;     &#x22EE;
      tr &#x2061;  A  m &#x2212; 1     tr &#x2061;  A  m &#x2212; 2
      &#x22EF;   &#x22EF;   1     tr &#x2061;  A  m     tr &#x2061;  A  m
      &#x2212; 1     &#x22EF;   &#x22EF;   tr &#x2061; A    |   &#xA0; .
      {\displaystyle c_{n-m}={\frac {(-1)^{m}}{m!}}{\begin
      {vmatrix}\operatorname {tr} A&m-1&0&\cdots \\\operatorname {tr} A^
      {2}&\operatorname {tr} A&m-2&\cdots \\\vdots &\vdots &&&\vdots
      \\\operatorname {tr} A^{m-1}&\operatorname {tr} A^{m-2}&\cdots &\cdots
      &1\\\operatorname {tr} A^{m}&\operatorname {tr} A^{m-1}&\cdots &\cdots
      &\operatorname {tr} A\end{vmatrix}}~.}  [{\displaystyle c_{n-m}={\frac {
      (-1)^{m}}{m!}}{\begin{vmatrix}\operatorname {tr} A&m-1&0&\cdots
      \\\operatorname {tr} A^{2}&\operatorname {tr} A&m-2&\cdots \\\vdots
      &\vdots &&&\vdots \\\operatorname {tr} A^{m-1}&\operatorname {tr} A^{m-
      2}&\cdots &\cdots &1\\\operatorname {tr} A^{m}&\operatorname {tr} A^{m-
      1}&\cdots &\cdots &\operatorname {tr} A\end{vmatrix}}~.}]
**** n-th Power of matrix[edit] ****
The CayleyâHamilton theorem always provides a relationship between the powers
of A (though not always the simplest one), which allows one to simplify
expressions involving such powers, and evaluate them without having to compute
the power An or any higher powers of A.
As an example, for     A =   (    1   2     3   4    )     {\displaystyle A=
{\begin{pmatrix}1&2\\3&4\end{pmatrix}}}  [A={\begin{pmatrix}1&2\\3&4\end
{pmatrix}}] the theorem gives
          A  2   = 5 A + 2  I  2    .   {\displaystyle A^{2}=5A+2I_{2}\,.}  [A^
      {2}=5A+2I_{2}\,.]
Then, to calculate A4, observe
          A  3   = ( 5 A + 2  I  2   ) A = 5  A  2   + 2 A = 5 ( 5 A + 2  I  2
      ) + 2 A = 27 A + 10  I  2   ,   {\displaystyle A^{3}=(5A+2I_{2})A=5A^
      {2}+2A=5(5A+2I_{2})+2A=27A+10I_{2},}  [{\displaystyle A^{3}=(5A+2I_
      {2})A=5A^{2}+2A=5(5A+2I_{2})+2A=27A+10I_{2},}]
          A  4   =  A  3   A = ( 27 A + 10  I  2   ) A = 27  A  2   + 10 A = 27
      ( 5 A + 2  I  2   ) + 10 A = 145 A + 54  I  2    .   {\displaystyle A^
      {4}=A^{3}A=(27A+10I_{2})A=27A^{2}+10A=27(5A+2I_{2})+10A=145A+54I_{2}\,.}
      [A^{4}=A^{3}A=(27A+10I_{2})A=27A^{2}+10A=27(5A+2I_{2})+10A=145A+54I_
      {2}\,.]
Likewise,
          A  &#x2212; 1   =    A &#x2212; 5  I  2    2   &#xA0; .
      {\displaystyle A^{-1}={\frac {A-5I_{2}}{2}}~.}  [A^{-1}={\frac {A-5I_{2}}
      {2}}~.]
Notice that we have been able to write the matrix power as the sum of two
terms. In fact, matrix power of any order k can be written as a matrix
polynomial of degree at most n - 1, where n is the size of a square matrix.
This is an instance where CayleyâHamilton theorem can be used to express a
matrix function, which we will discuss below systematically.
**** Matrix functions[edit] ****
Given an analytic function
         f ( x ) =  &#x2211;  k = 0   &#x221E;    a  k    x  k
      {\displaystyle f(x)=\sum _{k=0}^{\infty }a_{k}x^{k}}  [{\displaystyle f
      (x)=\sum _{k=0}^{\infty }a_{k}x^{k}}]
and the characteristic polynomial p(x) of degree n of an n Ã n matrix A, the
function can be expressed using long division as
         f ( x ) = q ( x ) p ( x ) + r ( x ) ,   {\displaystyle f(x)=q(x)p(x)+r
      (x),}  [{\displaystyle f(x)=q(x)p(x)+r(x),}]
where q(x) is some quotient polynomial and r(x) is a remainder polynomial such
that 0 â¤ deg r(x) < n. By the CayleyâHamilton theorem, replacing x by the
matrix A gives p(A) = 0, so one has
         f ( A ) = r ( A ) .   {\displaystyle f(A)=r(A).}  [{\displaystyle f
      (A)=r(A).}]
Thus, the analytic function of matrix A can be expressed as a matrix polynomial
of degree less than n.
Let the remainder polynomial be
         r ( x ) =  c  0   +  c  1   x + &#x22EF; +  c  n &#x2212; 1    x  n
      &#x2212; 1   .   {\displaystyle r(x)=c_{0}+c_{1}x+\cdots +c_{n-1}x^{n-
      1}.}  [{\displaystyle r(x)=c_{0}+c_{1}x+\cdots +c_{n-1}x^{n-1}.}]
Since p(Î») = 0, evaluating the function f(x) at the n eigenvalues of A, yields
         f (  &#x03BB;  i   ) = r (  &#x03BB;  i   ) =  c  0   +  c  1
      &#x03BB;  i   + &#x22EF; +  c  n &#x2212; 1    &#x03BB;  i   n &#x2212; 1
      ,   f o r   i = 1 , 2 , . . . , n .   {\displaystyle f(\lambda _{i})=r
      (\lambda _{i})=c_{0}+c_{1}\lambda _{i}+\cdots +c_{n-1}\lambda _{i}^{n-
      1},\qquad \mathrm {for} \qquad i=1,2,...,n.}  [{\displaystyle f(\lambda _
      {i})=r(\lambda _{i})=c_{0}+c_{1}\lambda _{i}+\cdots +c_{n-1}\lambda _{i}^
      {n-1},\qquad \mathrm {for} \qquad i=1,2,...,n.}]
This amounts to a system of n linear equations, which can be solved to
determine the coefficients ci. Thus, one has
         f ( A ) =  &#x2211;  k = 0   n &#x2212; 1    c  k    A  k   .
      {\displaystyle f(A)=\sum _{k=0}^{n-1}c_{k}A^{k}.}  [{\displaystyle f
      (A)=\sum _{k=0}^{n-1}c_{k}A^{k}.}]
When the eigenvalues are repeated, that is Î»i = Î»j for some i â  j, two or
more equations are identical; and hence the linear equations cannot be solved
uniquely. For such cases, for an eigenvalue Î» with multiplicity m, the first m
â 1 derivative of p(x) vanishes at the eigenvalues. Thus, there are the extra
m â 1 linearly independent solutions
              d   k   f ( x )    d   x  k         |    x = &#x03BB;   =      d
      k   r ( x )    d   x  k         |    x = &#x03BB;     for   k = 1 , 2 ,
      &#x2026; , m &#x2212; 1 ,   {\displaystyle {\frac {\mathrm {d} ^{k}f(x)}
      {\mathrm {d} x^{k}}}{\Big |}_{x=\lambda }={\frac {\mathrm {d} ^{k}r(x)}
      {\mathrm {d} x^{k}}}{\Big |}_{x=\lambda }\qquad {\text{for}}\qquad
      k=1,2,\ldots ,m-1,}  [{\displaystyle {\frac {\mathrm {d} ^{k}f(x)}
      {\mathrm {d} x^{k}}}{\Big |}_{x=\lambda }={\frac {\mathrm {d} ^{k}r(x)}
      {\mathrm {d} x^{k}}}{\Big |}_{x=\lambda }\qquad {\text{for}}\qquad
      k=1,2,\ldots ,m-1,}]
which, when combined with others, yield the required n equations to solve for
ci.
Finding a polynomial that passes through the points (Î»i, f (Î»i)) is
essentially an interpolation_problem, and can be solved using Lagrange or
Newton_interpolation techniques, leading to Sylvester's_formula.
For example, suppose the task is to find the polynomial representation of
         f ( A ) =  e  A t     w h e r e   A =   (    1   2     0   3    )   .
      {\displaystyle f(A)=e^{At}\qquad \mathrm {where} \qquad A={\begin
      {pmatrix}1&2\\0&3\end{pmatrix}}.}  [{\displaystyle f(A)=e^{At}\qquad
      \mathrm {where} \qquad A={\begin{pmatrix}1&2\\0&3\end{pmatrix}}.}]
The characteristic polynomial is p(x) = (x â 1)(x â 3) = x2 â 4x + 3, and
the eigenvalues are Î» = 1, 3. Let r(x) = c0 + c1x. Evaluating f(Î») =r(Î») at
the eigenvalues, one obtains two linear equations et = c0 + c1 and e3t = c0 +
3c1. Solving the equations yields c0 = (3et â e3t)/2 and c1 = (e3t â et)/2.
Thus, it follows that
          e  A t   =  c  0    I  2   +  c  1   A =   (     c  0   +  c  1     2
      c  1       0    c  0   + 3  c  1      )   =   (     e  t      e  3 t
      &#x2212;  e  t       0    e  3 t      )   .   {\displaystyle e^{At}=c_
      {0}I_{2}+c_{1}A={\begin{pmatrix}c_{0}+c_{1}&2c_{1}\\0&c_{0}+3c_{1}\end
      {pmatrix}}={\begin{pmatrix}e^{t}&e^{3t}-e^{t}\\0&e^{3t}\end{pmatrix}}.}
      [{\displaystyle e^{At}=c_{0}I_{2}+c_{1}A={\begin{pmatrix}c_{0}+c_{1}&2c_
      {1}\\0&c_{0}+3c_{1}\end{pmatrix}}={\begin{pmatrix}e^{t}&e^{3t}-e^
      {t}\\0&e^{3t}\end{pmatrix}}.}]
If, instead, the function were f(A) = sin At, then the coefficients would have
been c0 = (3 sin t â sin 3t)/2 and c1 = (sin 3t - sin t)/2; hence
         sin &#x2061; ( A t ) =  c  0    I  2   +  c  1   A =   (    sin
      &#x2061; t   sin &#x2061; 3 t &#x2212; sin &#x2061; t     0   sin
      &#x2061; 3 t    )   .   {\displaystyle \sin(At)=c_{0}I_{2}+c_{1}A={\begin
      {pmatrix}\sin t&\sin 3t-\sin t\\0&\sin 3t\end{pmatrix}}.}  [
      {\displaystyle \sin(At)=c_{0}I_{2}+c_{1}A={\begin{pmatrix}\sin t&\sin 3t-
      \sin t\\0&\sin 3t\end{pmatrix}}.}]
As a further example, when considering
         f ( A ) =  e  A t     w h e r e   A =   (    0   1     &#x2212; 1   0
      )   ,   {\displaystyle f(A)=e^{At}\qquad \mathrm {where} \qquad A={\begin
      {pmatrix}0&1\\-1&0\end{pmatrix}},}  [{\displaystyle f(A)=e^{At}\qquad
      \mathrm {where} \qquad A={\begin{pmatrix}0&1\\-1&0\end{pmatrix}},}]
then the characteristic polynomial is p(x) = x2 + 1, and the eigenvalues are Î»
= Â±i. As before, evaluating the function at the eigenvalues gives us the
linear equations eit = c0 + i c1 and eâit = c0 â ic1; the solution of which
gives, c0 = (eit + eâit)/2 = cos t and c1 = (eit â eâit)/2i = sin t.
Thus, for this case,
          e  A t   = ( cos &#x2061; t )  I  2   + ( sin &#x2061; t ) A =
      (    cos &#x2061; t   sin &#x2061; t     &#x2212; sin &#x2061; t   cos
      &#x2061; t    )   ,   {\displaystyle e^{At}=(\cos t)I_{2}+(\sin t)A=
      {\begin{pmatrix}\cos t&\sin t\\-\sin t&\cos t\end{pmatrix}},}  [
      {\displaystyle e^{At}=(\cos t)I_{2}+(\sin t)A={\begin{pmatrix}\cos t&\sin
      t\\-\sin t&\cos t\end{pmatrix}},}]
which is a rotation_matrix.
Standard examples of such usage is the exponential_map from the Lie_algebra of
a matrix_Lie_group into the group. It is given by a matrix_exponential,
         exp :   g   &#x2192; G ;  t X &#x21A6;  e  t X   =  &#x2211;  n = 0
      &#x221E;       t  n    X  n     n !    = I + t X +     t  2    X  2    2
      + &#x22EF; , t &#x2208;  R  , X &#x2208;   g   .   {\displaystyle \exp :
      {\mathfrak {g}}\rightarrow G;\qquad tX\mapsto e^{tX}=\sum _{n=0}^{\infty
      }{\frac {t^{n}X^{n}}{n!}}=I+tX+{\frac {t^{2}X^{2}}{2}}+\cdots ,t\in
      \mathbb {R} ,X\in {\mathfrak {g}}.}  [{\displaystyle \exp :{\mathfrak
      {g}}\rightarrow G;\qquad tX\mapsto e^{tX}=\sum _{n=0}^{\infty }{\frac {t^
      {n}X^{n}}{n!}}=I+tX+{\frac {t^{2}X^{2}}{2}}+\cdots ,t\in \mathbb {R}
      ,X\in {\mathfrak {g}}.}]
Such expressions have long been known for SU(2),
          e  i ( &#x03B8;  /  2 ) (    n &#x005E;    &#x22C5; &#x03C3; )   =  I
      2   cos &#x2061; &#x03B8;  /  2 + i (    n &#x005E;    &#x22C5; &#x03C3;
      ) sin &#x2061; &#x03B8;  /  2 ,   {\displaystyle e^{i(\theta /2)({\hat
      {n}}\cdot \sigma )}=I_{2}\cos \theta /2+i({\hat {n}}\cdot \sigma )\sin
      \theta /2,}  [e^{i(\theta /2)({\hat {n}}\cdot \sigma )}=I_{2}\cos \theta
      /2+i({\hat {n}}\cdot \sigma )\sin \theta /2,]
where the Ï are the Pauli_matrices and for SO(3),
          e  i &#x03B8; (    n &#x005E;    &#x22C5;  J  )   =  I  3   + i
      (    n &#x005E;    &#x22C5;  J  ) sin &#x2061; &#x03B8; + (    n &#x005E;
      &#x22C5;  J   )  2   ( cos &#x2061; &#x03B8; &#x2212; 1 ) ,
      {\displaystyle e^{i\theta ({\hat {n}}\cdot \mathbf {J} )}=I_{3}+i({\hat
      {n}}\cdot \mathbf {J} )\sin \theta +({\hat {n}}\cdot \mathbf {J} )^{2}
      (\cos \theta -1),}  [e^{i\theta ({\hat {n}}\cdot \mathbf {J} )}=I_{3}+i(
      {\hat {n}}\cdot \mathbf {J} )\sin \theta +({\hat {n}}\cdot \mathbf {J} )^
      {2}(\cos \theta -1),]
which is Rodrigues'_rotation_formula. For the notation, see rotation_group_SO
(3)#A_note_on_Lie_algebra.
More recently, expressions have appeared for other groups, like the Lorentz
group SO(3, 1),[11] O(4, 2)[12] and SU(2, 2),[13] as well as GL(n, R).[14] The
group O(4, 2) is the conformal_group of spacetime, SU(2, 2) its simply
connected cover (to be precise, the simply connected cover of the connected
component SO+(4, 2) of O(4, 2)). The expressions obtained apply to the standard
representation of these groups. They require knowledge of (some of) the
eigenvalues of the matrix to exponentiate. For SU(2) (and hence for SO(3)),
closed expressions have recently been obtained for all irreducible
representations, i.e. of any spin.[15]
Ferdinand_Georg_Frobenius (1849â1917), German mathematician. His main
interests were elliptic_functions differential_equations, and later group
theory.
In 1878 he gave the first full proof of the Cayley–Hamilton theorem.[10]
**** Algebraic number theory[edit] ****
The CayleyâHamilton theorem is an effective tool for computing the minimal
polynomial of algebraic integers. For example, given a finite extension      Q
[  &#x03B1;  1   , &#x2026; ,  &#x03B1;  k   ]   {\displaystyle \mathbb {Q}
[\alpha _{1},\ldots ,\alpha _{k}]}  [{\displaystyle \mathbb {Q} [\alpha _
{1},\ldots ,\alpha _{k}]}] of      Q    {\displaystyle \mathbb {Q} }  [\mathbb
{Q} ] and an algebraic integer     &#x03B1; &#x2208;  Q  [  &#x03B1;  1   ,
&#x2026; ,  &#x03B1;  k   ]   {\displaystyle \alpha \in \mathbb {Q} [\alpha _
{1},\ldots ,\alpha _{k}]}  [{\displaystyle \alpha \in \mathbb {Q} [\alpha _
{1},\ldots ,\alpha _{k}]}] which is a non-zero linear combination of the
&#x03B1;  1    n  1     &#x22EF;  &#x03B1;  k    n  k       {\displaystyle
\alpha _{1}^{n_{1}}\cdots \alpha _{k}^{n_{k}}}  [{\displaystyle \alpha _{1}^{n_
{1}}\cdots \alpha _{k}^{n_{k}}}] we can compute the minimal polynomial of
&#x03B1;   {\displaystyle \alpha }  [\alpha ] by finding a matrix representing
the      Q    {\displaystyle \mathbb {Q} }  [\mathbb {Q} ]-linear
transformation
         &#x22C5; &#x03B1; :  Q  [  &#x03B1;  1   , &#x2026; ,  &#x03B1;  k   ]
      &#x2192;  Q  [  &#x03B1;  1   , &#x2026; ,  &#x03B1;  k   ]
      {\displaystyle \cdot \alpha :\mathbb {Q} [\alpha _{1},\ldots ,\alpha _
      {k}]\to \mathbb {Q} [\alpha _{1},\ldots ,\alpha _{k}]}  [{\displaystyle
      \cdot \alpha :\mathbb {Q} [\alpha _{1},\ldots ,\alpha _{k}]\to \mathbb
      {Q} [\alpha _{1},\ldots ,\alpha _{k}]}]
If we call this transformation matrix     A   {\displaystyle A}  [A], then we
can find the minimal polynomial by applying the CayleyâHamilton theorem to
A   {\displaystyle A}  [A].[16]
***** Proving the theorem in general[edit] *****
The CayleyâHamilton theorem is an immediate consequence of the existence of
the Jordan_normal_form for matrices over algebraically_closed_fields. In this
section direct proofs are presented.
As the examples above show, obtaining the statement of the CayleyâHamilton
theorem for an nÃn matrix
         A = (  a  i j    )  i , j = 1   n     {\displaystyle A=(a_{ij})_
      {i,j=1}^{n}}  [A=(a_{ij})_{i,j=1}^{n}]
requires two steps: first the coefficients ci of the characteristic polynomial
are determined by development as a polynomial in t of the determinant
             p ( t )    = det ( t  I  n   &#x2212; A ) =   |    t &#x2212;  a
      1 , 1     &#x2212;  a  1 , 2     &#x22EF;   &#x2212;  a  1 , n
      &#x2212;  a  2 , 1     t &#x2212;  a  2 , 2     &#x22EF;   &#x2212;  a  2
      , n       &#x22EE;   &#x22EE;   &#x22F1;   &#x22EE;     &#x2212;  a  n ,
      1     &#x2212;  a  n , 2     &#x22EF;   t &#x2212;  a  n , n      |
      =  t  n   +  c  n &#x2212; 1    t  n &#x2212; 1   + &#x22EF; +  c  1   t
      +  c  0   ,       {\displaystyle {\begin{aligned}p(t)&=\det(tI_{n}-A)=
      {\begin{vmatrix}t-a_{1,1}&-a_{1,2}&\cdots &-a_{1,n}\\-a_{2,1}&t-a_
      {2,2}&\cdots &-a_{2,n}\\\vdots &\vdots &\ddots &\vdots \\-a_{n,1}&-a_
      {n,2}&\cdots &t-a_{n,n}\end{vmatrix}}\\[5pt]&=t^{n}+c_{n-1}t^{n-1}+\cdots
      +c_{1}t+c_{0},\end{aligned}}}  [{\displaystyle {\begin{aligned}p(t)&=\det
      (tI_{n}-A)={\begin{vmatrix}t-a_{1,1}&-a_{1,2}&\cdots &-a_{1,n}\\-a_
      {2,1}&t-a_{2,2}&\cdots &-a_{2,n}\\\vdots &\vdots &\ddots &\vdots \\-a_
      {n,1}&-a_{n,2}&\cdots &t-a_{n,n}\end{vmatrix}}\\[5pt]&=t^{n}+c_{n-1}t^{n-
      1}+\cdots +c_{1}t+c_{0},\end{aligned}}}]
and then these coefficients are used in a linear combination of powers of A
that is equated to the nÃn null matrix:
          A  n   +  c  n &#x2212; 1    A  n &#x2212; 1   + &#x22EF; +  c  1   A
      +  c  0    I  n   =   (    0   &#x22EF;   0     &#x22EE;   &#x22F1;
      &#x22EE;     0   &#x22EF;   0    )   .   {\displaystyle A^{n}+c_{n-1}A^
      {n-1}+\cdots +c_{1}A+c_{0}I_{n}={\begin{pmatrix}0&\cdots &0\\\vdots
      &\ddots &\vdots \\0&\cdots &0\end{pmatrix}}.}  [{\displaystyle A^{n}+c_
      {n-1}A^{n-1}+\cdots +c_{1}A+c_{0}I_{n}={\begin{pmatrix}0&\cdots
      &0\\\vdots &\ddots &\vdots \\0&\cdots &0\end{pmatrix}}.}]
The left hand side can be worked out to an nÃn matrix whose entries are
(enormous) polynomial expressions in the set of entries ai,j of A, so the
CayleyâHamilton theorem states that each of these n2 expressions are equal to
0. For any fixed value of n these identities can be obtained by tedious but
completely straightforward algebraic manipulations. None of these computations
can show however why the CayleyâHamilton theorem should be valid for matrices
of all possible sizes n, so a uniform proof for all n is needed.
**** Preliminaries[edit] ****
If a vector v of size n happens to be an eigenvector of A with eigenvalue Î»,
in other words if Aâv = Î»v, then
             p ( A ) &#x22C5; v    =  A  n   &#x22C5; v +  c  n &#x2212; 1    A
      n &#x2212; 1   &#x22C5; v + &#x22EF; +  c  1   A &#x22C5; v +  c  0    I
      n   &#x22C5; v       =  &#x03BB;  n   v +  c  n &#x2212; 1    &#x03BB;  n
      &#x2212; 1   v + &#x22EF; +  c  1   &#x03BB; v +  c  0   v = p ( &#x03BB;
      ) v ,       {\displaystyle {\begin{aligned}p(A)\cdot v&=A^{n}\cdot v+c_
      {n-1}A^{n-1}\cdot v+\cdots +c_{1}A\cdot v+c_{0}I_{n}\cdot v\\
      [6pt]&=\lambda ^{n}v+c_{n-1}\lambda ^{n-1}v+\cdots +c_{1}\lambda v+c_
      {0}v=p(\lambda )v,\end{aligned}}}  [{\displaystyle {\begin{aligned}p
      (A)\cdot v&=A^{n}\cdot v+c_{n-1}A^{n-1}\cdot v+\cdots +c_{1}A\cdot v+c_
      {0}I_{n}\cdot v\\[6pt]&=\lambda ^{n}v+c_{n-1}\lambda ^{n-1}v+\cdots +c_
      {1}\lambda v+c_{0}v=p(\lambda )v,\end{aligned}}}]
which is the null vector since p(Î») = 0 (the eigenvalues of A are precisely
the roots of p(t)). This holds for all possible eigenvalues Î», so the two
matrices equated by the theorem certainly give the same (null) result when
applied to any eigenvector. Now if A admits a basis of eigenvectors, in other
words if A is diagonalizable, then the CayleyâHamilton theorem must hold for
A, since two matrices that give the same values when applied to each element of
a basis must be equal.
         A = X D  X  &#x2212; 1   ,  D = diag &#x2061; (  &#x03BB;  i   ) ,  i
      = 1 , 2 , . . . , n   {\displaystyle A=XDX^{-1},\quad D=\operatorname
      {diag} (\lambda _{i}),\quad i=1,2,...,n}  [{\displaystyle A=XDX^{-
      1},\quad D=\operatorname {diag} (\lambda _{i}),\quad i=1,2,...,n}]
          p  A   ( &#x03BB; ) =  |  &#x03BB; I &#x2212; A  |  =
      {\displaystyle p_{A}(\lambda )=|\lambda I-A|=}  [{\displaystyle p_{A}
      (\lambda )=|\lambda I-A|=}] product of eigenvalues of     &#x03BB; I
      &#x2212; A =  &#x220F;  i = 1   n   ( &#x03BB; &#x2212;  &#x03BB;  i   )
      &#x2261;  &#x2211;  k = 0   n    c  k    &#x03BB;  k     {\displaystyle
      \lambda I-A=\prod _{i=1}^{n}(\lambda -\lambda _{i})\equiv \sum _{k=0}^
      {n}c_{k}\lambda ^{k}}  [{\displaystyle \lambda I-A=\prod _{i=1}^{n}
      (\lambda -\lambda _{i})\equiv \sum _{k=0}^{n}c_{k}\lambda ^{k}}]
          p  A   ( A ) = &#x2211;  c  k    A  k   = X  p  A   ( D )  X
      &#x2212; 1   = X C  X  &#x2212; 1     {\displaystyle p_{A}(A)=\sum c_
      {k}A^{k}=Xp_{A}(D)X^{-1}=XCX^{-1}}  [{\displaystyle p_{A}(A)=\sum c_{k}A^
      {k}=Xp_{A}(D)X^{-1}=XCX^{-1}}]
          C  i i   =  &#x2211;  k = 0   n    c  k    &#x03BB;  i   k   =
      &#x220F;  j = 1   n   (  &#x03BB;  i   &#x2212;  &#x03BB;  j   ) = 0 ,
      C  i , j &#x2260; i   = 0   {\displaystyle C_{ii}=\sum _{k=0}^{n}c_
      {k}\lambda _{i}^{k}=\prod _{j=1}^{n}(\lambda _{i}-\lambda _{j})=0,\qquad
      C_{i,j\neq i}=0}  [{\displaystyle C_{ii}=\sum _{k=0}^{n}c_{k}\lambda _
      {i}^{k}=\prod _{j=1}^{n}(\lambda _{i}-\lambda _{j})=0,\qquad C_{i,j\neq
      i}=0}]
         &#x2234;  p  A   ( A ) = X C  X  &#x2212; 1   = O .   {\displaystyle
      \therefore p_{A}(A)=XCX^{-1}=O.}  [{\displaystyle \therefore p_{A}
      (A)=XCX^{-1}=O.}]
Consider now the function     e :  M  n   &#x2192;  M  n     {\displaystyle e:
M_{n}\to M_{n}}  [{\displaystyle e:M_{n}\to M_{n}}]which maps     n &#x00D7; n
{\displaystyle n\times n}  [n\times n]matrices to     n &#x00D7; n
{\displaystyle n\times n}  [n\times n]matrices given by the formula     e ( A )
=  p  A   ( A )   {\displaystyle e(A)=p_{A}(A)}  [{\displaystyle e(A)=p_{A}
(A)}], i.e. which takes a matrix     A   {\displaystyle A}  [A]and plugs it
into its own characteristic polynomial. Not all matrices are diagonalizable,
but for matrices with complex coefficients many of them are: the set of     D
{\displaystyle D}  [D] diagonalizable complex square matrices of a given size
is dense in the set of all such square matrices[17] (for a matrix to be
diagonalizable it suffices for instance that its characteristic polynomial not
have any multiple roots). Now viewed as a function     e :   C    n  2
&#x2192;   C    n  2       {\displaystyle e:\mathbb {C} ^{n^{2}}\to \mathbb {C}
^{n^{2}}}  [{\displaystyle e:\mathbb {C} ^{n^{2}}\to \mathbb {C} ^{n^{2}}}]
(since matrices have      n  2     {\displaystyle n^{2}}  [n^{2}]entries) we
see that this function is continuous. This is true because the entries of the
image of a matrix are given by polynomials in the entries of the matrix. Since
   e ( D ) =  {   (    0   &#x22EF;   0     &#x22EE;   &#x22F1;   &#x22EE;
0   &#x22EF;   0    )   }    {\displaystyle e(D)=\left\{{\begin
{pmatrix}0&\cdots &0\\\vdots &\ddots &\vdots \\0&\cdots &0\end
{pmatrix}}\right\}}  [{\displaystyle e(D)=\left\{{\begin{pmatrix}0&\cdots
&0\\\vdots &\ddots &\vdots \\0&\cdots &0\end{pmatrix}}\right\}}]
and since     D   {\displaystyle D}  [D]is dense, by continuity this function
must map the entire set of     n &#x00D7; n   {\displaystyle n\times n}
[n\times n]matrices to the zero matrix. Therefore the CayleyâHamilton theorem
is true for complex numbers, and must therefore also hold for      Q
{\displaystyle \mathbb {Q} }  [\mathbb {Q} ]or      R    {\displaystyle \mathbb
{R} }  [\mathbb {R} ]valued matrices..
While this provides a valid proof, the argument is not very satisfactory, since
the identities represented by the theorem do not in any way depend on the
nature of the matrix (diagonalizable or not), nor on the kind of entries
allowed (for matrices with real entries the diagonalizable ones do not form a
dense set, and it seems strange one would have to consider complex matrices to
see that the CayleyâHamilton theorem holds for them). We shall therefore now
consider only arguments that prove the theorem directly for any matrix using
algebraic manipulations only; these also have the benefit of working for
matrices with entries in any commutative_ring.
There is a great variety of such proofs of the CayleyâHamilton theorem, of
which several will be given here. They vary in the amount of abstract algebraic
notions required to understand the proof. The simplest proofs use just those
notions needed to formulate the theorem (matrices, polynomials with numeric
entries, determinants), but involve technical computations that render somewhat
mysterious the fact that they lead precisely to the correct conclusion. It is
possible to avoid such details, but at the price of involving more subtle
algebraic notions: polynomials with coefficients in a non-commutative ring, or
matrices with unusual kinds of entries.
*** Adjugate matrices[edit] ***
All proofs below use the notion of the adjugate_matrix adj(M) of an nÃn matrix
M, the transpose of its cofactor_matrix.
This is a matrix whose coefficients are given by polynomial expressions in the
coefficients of M (in fact, by certain (n â 1)Ã(n â 1) determinants), in
such a way that the following fundamental relations hold,
         adj &#x2061; ( M ) &#x22C5; M = det ( M )  I  n   = M &#x22C5; adj
      &#x2061; ( M ) &#xA0; .   {\displaystyle \operatorname {adj} (M)\cdot
      M=\det(M)I_{n}=M\cdot \operatorname {adj} (M)~.}  [\operatorname {adj}
      (M)\cdot M=\det(M)I_{n}=M\cdot \operatorname {adj} (M)~.]
These relations are a direct consequence of the basic properties of
determinants: evaluation of the (i,j) entry of the matrix product on the left
gives the expansion by column j of the determinant of the matrix obtained from
M by replacing column i by a copy of column j, which is det(M) if i = j and
zero otherwise; the matrix product on the right is similar, but for expansions
by rows.
Being a consequence of just algebraic expression manipulation, these relations
are valid for matrices with entries in any commutative ring (commutativity must
be assumed for determinants to be defined in the first place). This is
important to note here, because these relations will be applied below for
matrices with non-numeric entries such as polynomials.
**** A direct algebraic proof[edit] ****
This proof uses just the kind of objects needed to formulate the
CayleyâHamilton theorem: matrices with polynomials as entries. The matrix t
In âA whose determinant is the characteristic polynomial of A is such a
matrix, and since polynomials form a commutative ring, it has an adjugate
         B = adj &#x2061; ( t  I  n   &#x2212; A ) .   {\displaystyle
      B=\operatorname {adj} (tI_{n}-A).}  [B=\operatorname {adj} (tI_{n}-A).]
Then, according to the right-hand fundamental relation of the adjugate, one has
         ( t  I  n   &#x2212; A ) B = det ( t  I  n   &#x2212; A )  I  n   = p
      ( t )  I  n   &#xA0; .   {\displaystyle (tI_{n}-A)B=\det(tI_{n}-A)I_{n}=p
      (t)I_{n}~.}  [{\displaystyle (tI_{n}-A)B=\det(tI_{n}-A)I_{n}=p(t)I_
      {n}~.}]
Since B is also a matrix with polynomials in t as entries, one can, for each i
, collect the coefficients of ti in each entry to form a matrix B i of numbers,
such that one has
         B =  &#x2211;  i = 0   n &#x2212; 1    t  i    B  i   &#xA0; .
      {\displaystyle B=\sum _{i=0}^{n-1}t^{i}B_{i}~.}  [{\displaystyle B=\sum _
      {i=0}^{n-1}t^{i}B_{i}~.}]
(The way the entries of B are defined makes clear that no powers higher than
tnâ1 occur). While this looks like a polynomial with matrices as
coefficients, we shall not consider such a notion; it is just a way to write a
matrix with polynomial entries as a linear combination of n constant matrices,
and the coefficient t i has been written to the left of the matrix to stress
this point of view.
Now, one can expand the matrix product in our equation by bilinearity
             p ( t )  I  n      = ( t  I  n   &#x2212; A ) B       = ( t  I  n
      &#x2212; A )  &#x2211;  i = 0   n &#x2212; 1    t  i    B  i         =
      &#x2211;  i = 0   n &#x2212; 1   t  I  n   &#x22C5;  t  i    B  i
      &#x2212;  &#x2211;  i = 0   n &#x2212; 1   A &#x22C5;  t  i    B  i
      =  &#x2211;  i = 0   n &#x2212; 1    t  i + 1    B  i   &#x2212;
      &#x2211;  i = 0   n &#x2212; 1    t  i   A  B  i         =  t  n    B  n
      &#x2212; 1   +  &#x2211;  i = 1   n &#x2212; 1    t  i   (  B  i &#x2212;
      1   &#x2212; A  B  i   ) &#x2212; A  B  0   &#xA0; .       {\displaystyle
      {\begin{aligned}p(t)I_{n}&=(tI_{n}-A)B\\&=(tI_{n}-A)\sum _{i=0}^{n-1}t^
      {i}B_{i}\\&=\sum _{i=0}^{n-1}tI_{n}\cdot t^{i}B_{i}-\sum _{i=0}^{n-
      1}A\cdot t^{i}B_{i}\\&=\sum _{i=0}^{n-1}t^{i+1}B_{i}-\sum _{i=0}^{n-1}t^
      {i}AB_{i}\\&=t^{n}B_{n-1}+\sum _{i=1}^{n-1}t^{i}(B_{i-1}-AB_{i})-AB_
      {0}~.\end{aligned}}}  [{\displaystyle {\begin{aligned}p(t)I_{n}&=(tI_{n}-
      A)B\\&=(tI_{n}-A)\sum _{i=0}^{n-1}t^{i}B_{i}\\&=\sum _{i=0}^{n-1}tI_
      {n}\cdot t^{i}B_{i}-\sum _{i=0}^{n-1}A\cdot t^{i}B_{i}\\&=\sum _{i=0}^{n-
      1}t^{i+1}B_{i}-\sum _{i=0}^{n-1}t^{i}AB_{i}\\&=t^{n}B_{n-1}+\sum _{i=1}^
      {n-1}t^{i}(B_{i-1}-AB_{i})-AB_{0}~.\end{aligned}}}]
Writing
         p ( t )  I  n   =  t  n    I  n   +  t  n &#x2212; 1    c  n &#x2212;
      1    I  n   + &#x22EF; + t  c  1    I  n   +  c  0    I  n   &#xA0; ,
      {\displaystyle p(t)I_{n}=t^{n}I_{n}+t^{n-1}c_{n-1}I_{n}+\cdots +tc_{1}I_
      {n}+c_{0}I_{n}~,}  [p(t)I_{n}=t^{n}I_{n}+t^{n-1}c_{n-1}I_{n}+\cdots +tc_
      {1}I_{n}+c_{0}I_{n}~,]
one obtains an equality of two matrices with polynomial entries, written as
linear combinations of constant matrices with powers of t as coefficients.
Such an equality can hold only if in any matrix position the entry that is
multiplied by a given power  ti is the same on both sides; it follows that the
constant matrices with coefficient ti in both expressions must be equal.
Writing these equations then for i from n down to 0, one finds
          B  n &#x2212; 1   =  I  n   ,   B  i &#x2212; 1   &#x2212; A  B  i
      =  c  i    I  n     for&#xA0;  1 &#x2264; i &#x2264; n &#x2212; 1 ,
      &#x2212; A  B  0   =  c  0    I  n   &#xA0; .   {\displaystyle B_{n-1}=I_
      {n},\qquad B_{i-1}-AB_{i}=c_{i}I_{n}\quad {\text{for }}1\leq i\leq n-
      1,\qquad -AB_{0}=c_{0}I_{n}~.}  [{\displaystyle B_{n-1}=I_{n},\qquad B_
      {i-1}-AB_{i}=c_{i}I_{n}\quad {\text{for }}1\leq i\leq n-1,\qquad -AB_
      {0}=c_{0}I_{n}~.}]
Finally, multiply the equation of the coefficients of ti from the left by Ai,
and sum up:
    A  n    B  n &#x2212; 1   +  &#x2211;  i = 1   n &#x2212; 1    (   A  i
B  i &#x2212; 1   &#x2212;  A  i + 1    B  i    )  &#x2212; A  B  0   =  A  n
+  c  n &#x2212; 1    A  n &#x2212; 1   + &#x22EF; +  c  1   A +  c  0    I  n
&#xA0; .   {\textstyle A^{n}B_{n-1}+\sum \limits _{i=1}^{n-1}\left(A^{i}B_{i-
1}-A^{i+1}B_{i}\right)-AB_{0}=A^{n}+c_{n-1}A^{n-1}+\cdots +c_{1}A+c_{0}I_{n}~.}
[{\textstyle A^{n}B_{n-1}+\sum \limits _{i=1}^{n-1}\left(A^{i}B_{i-1}-A^{i+1}B_
{i}\right)-AB_{0}=A^{n}+c_{n-1}A^{n-1}+\cdots +c_{1}A+c_{0}I_{n}~.}]
The left-hand sides form a telescoping_sum and cancel completely; the right-
hand sides add up to     p ( A )   {\displaystyle p(A)}  [{\displaystyle p
(A)}]:
         0 = p ( A ) &#xA0; .   {\displaystyle 0=p(A)~.}  [{\displaystyle 0=p
      (A)~.}]
This completes the proof.
**** A proof using polynomials with matrix coefficients[edit] ****
This proof is similar to the first one, but tries to give meaning to the notion
of polynomial with matrix coefficients that was suggested by the expressions
occurring in that proof. This requires considerable care, since it is somewhat
unusual to consider polynomials with coefficients in a non-commutative ring,
and not all reasoning that is valid for commutative polynomials can be applied
in this setting.
Notably, while arithmetic of polynomials over a commutative ring models the
arithmetic of polynomial_functions, this is not the case over a non-commutative
ring (in fact there is no obvious notion of polynomial function in this case
that is closed under multiplication). So when considering polynomials in t with
matrix coefficients, the variable t must not be thought of as an "unknown", but
as a formal symbol that is to be manipulated according to given rules; in
particular one cannot just set t to a specific value.
         ( f + g ) ( x ) =  &#x2211;  i    (   f  i   +  g  i    )   x  i   =
      &#x2211;  i     f  i    x  i    +  &#x2211;  i     g  i    x  i    = f
      ( x ) + g ( x ) .   {\displaystyle (f+g)(x)=\sum _{i}\left(f_{i}+g_
      {i}\right)x^{i}=\sum _{i}{f_{i}x^{i}}+\sum _{i}{g_{i}x^{i}}=f(x)+g(x).}
      [{\displaystyle (f+g)(x)=\sum _{i}\left(f_{i}+g_{i}\right)x^{i}=\sum _{i}
      {f_{i}x^{i}}+\sum _{i}{g_{i}x^{i}}=f(x)+g(x).}]
Let M(n, R) be the ring of nÃn matrices with entries in some ring R (such as
the real or complex numbers) that has A as an element. Matrices with as
coefficients polynomials in t, such as     t  I  n   &#x2212; A
{\displaystyle tI_{n}-A}  [tI_{n}-A] or its adjugate B in the first proof, are
elements of M(n, R[t]).
By collecting like powers of t, such matrices can be written as "polynomials"
in t with constant matrices as coefficients; write M(n, R)[t] for the set of
such polynomials. Since this set is in bijection with M(n, R[t]), one defines
arithmetic operations on it correspondingly, in particular multiplication is
given by
          (   &#x2211;  i    M  i    t  i    )   (   &#x2211;  j    N  j    t
      j    )  =  &#x2211;  i , j   (  M  i    N  j   )  t  i + j   ,
      {\displaystyle \left(\sum _{i}M_{i}t^{i}\right)\left(\sum _{j}N_{j}t^
      {j}\right)=\sum _{i,j}(M_{i}N_{j})t^{i+j},}  [{\displaystyle \left(\sum _
      {i}M_{i}t^{i}\right)\left(\sum _{j}N_{j}t^{j}\right)=\sum _{i,j}(M_{i}N_
      {j})t^{i+j},}]
respecting the order of the coefficient matrices from the two operands;
obviously this gives a non-commutative multiplication.
Thus, the identity
         ( t  I  n   &#x2212; A ) B = p ( t )  I  n   .   {\displaystyle (tI_
      {n}-A)B=p(t)I_{n}.}  [{\displaystyle (tI_{n}-A)B=p(t)I_{n}.}]
from the first proof can be viewed as one involving a multiplication of
elements in M(n, R)[t].
At this point, it is tempting to simply set t equal to the matrix A , which
makes the first factor on the left equal to the null matrix, and the right hand
side equal to p(A); however, this is not an allowed operation when coefficients
do not commute. It is possible to define a "right-evaluation map" evA : M[t]
â M, which replaces each ti by the matrix power Ai of A , where one
stipulates that the power is always to be multiplied on the right to the
corresponding coefficient.
But this map is not a ring homomorphism: the right-evaluation of a product
differs in general from the product of the right-evaluations. This is so
because multiplication of polynomials with matrix coefficients does not model
multiplication of expressions containing unknowns: a product     M  t  i   N  t
j   = ( M &#x22C5; N )  t  i + j     {\displaystyle Mt^{i}Nt^{j}=(M\cdot N)t^
{i+j}}  [Mt^{i}Nt^{j}=(M\cdot N)t^{i+j}] is defined assuming that t commutes
with N, but this may fail if t is replaced by the matrix A.
One can work around this difficulty in the particular situation at hand, since
the above right-evaluation map does become a ring homomorphism if the matrix A
is in the center of the ring of coefficients, so that it commutes with all the
coefficients of the polynomials (the argument proving this is straightforward,
exactly because commuting t with coefficients is now justified after
evaluation).
Now, A is not always in the center of M, but we may replace M with a smaller
ring provided it contains all the coefficients of the polynomials in question:
I  n     {\displaystyle I_{n}}  [I_{n}], A, and the coefficients      B  i
{\displaystyle B_{i}}  [B_{i}] of the polynomial B. The obvious choice for such
a subring is the centralizer Z of A, the subring of all matrices that commute
with A; by definition A is in the center of Z.
This centralizer obviously contains      I  n     {\displaystyle I_{n}}  [I_
{n}], and A, but one has to show that it contains the matrices      B  i
{\displaystyle B_{i}}  [B_{i}]. To do this, one combines the two fundamental
relations for adjugates, writing out the adjugate B as a polynomial:
              (   &#x2211;  i = 0   m    B  i    t  i    )  ( t  I  n
      &#x2212; A )    = ( t  I  n   &#x2212; A )  &#x2211;  i = 0   m    B  i
      t  i        &#x2211;  i = 0   m    B  i    t  i + 1   &#x2212;  &#x2211;
      i = 0   m    B  i   A  t  i      =  &#x2211;  i = 0   m    B  i    t  i +
      1   &#x2212;  &#x2211;  i = 0   m   A  B  i    t  i        &#x2211;  i =
      0   m    B  i   A  t  i      =  &#x2211;  i = 0   m   A  B  i    t  i   .
      {\displaystyle {\begin{aligned}\left(\sum _{i=0}^{m}B_{i}t^{i}\right)(tI_
      {n}-A)&=(tI_{n}-A)\sum _{i=0}^{m}B_{i}t^{i}\\\sum _{i=0}^{m}B_{i}t^{i+1}-
      \sum _{i=0}^{m}B_{i}At^{i}&=\sum _{i=0}^{m}B_{i}t^{i+1}-\sum _{i=0}^
      {m}AB_{i}t^{i}\\\sum _{i=0}^{m}B_{i}At^{i}&=\sum _{i=0}^{m}AB_{i}t^
      {i}.\end{aligned}}}  [{\begin{aligned}\left(\sum _{i=0}^{m}B_{i}t^
      {i}\right)(tI_{n}-A)&=(tI_{n}-A)\sum _{i=0}^{m}B_{i}t^{i}\\\sum _{i=0}^
      {m}B_{i}t^{i+1}-\sum _{i=0}^{m}B_{i}At^{i}&=\sum _{i=0}^{m}B_{i}t^{i+1}-
      \sum _{i=0}^{m}AB_{i}t^{i}\\\sum _{i=0}^{m}B_{i}At^{i}&=\sum _{i=0}^
      {m}AB_{i}t^{i}.\end{aligned}}]
Equating_the_coefficients shows that for each i, we have A Bi = Bi A as
desired. Having found the proper setting in which evA is indeed a homomorphism
of rings, one can complete the proof as suggested above:
              ev  A   &#x2061;   (   p ( t )  I  n     )      =  ev  A
      &#x2061; ( ( t  I  n   &#x2212; A ) B )     p ( A )    =  ev  A
      &#x2061; ( t  I  n   &#x2212; A ) &#x22C5;  ev  A   &#x2061; ( B )     p
      ( A )    = ( A  I  n   &#x2212; A ) &#x22C5;  ev  A   &#x2061; ( B ) = O
      &#x22C5;  ev  A   &#x2061; ( B ) = O .       {\displaystyle {\begin
      {aligned}\operatorname {ev} _{A}{\bigl (}p(t)I_{n}{\bigr
      )}&=\operatorname {ev} _{A}((tI_{n}-A)B)\\[5pt]p(A)&=\operatorname {ev} _
      {A}(tI_{n}-A)\cdot \operatorname {ev} _{A}(B)\\[5pt]p(A)&=(AI_{n}-A)\cdot
      \operatorname {ev} _{A}(B)=O\cdot \operatorname {ev} _{A}(B)=O.\end
      {aligned}}}  [{\displaystyle {\begin{aligned}\operatorname {ev} _{A}
      {\bigl (}p(t)I_{n}{\bigr )}&=\operatorname {ev} _{A}((tI_{n}-A)B)\\[5pt]p
      (A)&=\operatorname {ev} _{A}(tI_{n}-A)\cdot \operatorname {ev} _{A}(B)\\
      [5pt]p(A)&=(AI_{n}-A)\cdot \operatorname {ev} _{A}(B)=O\cdot
      \operatorname {ev} _{A}(B)=O.\end{aligned}}}]
This completes the proof.
**** A synthesis of the first two proofs[edit] ****
In the first proof, one was able to determine the coefficients Bi of B based on
the right-hand fundamental relation for the adjugate only. In fact the first n
equations derived can be interpreted as determining the quotient B of the
Euclidean_division of the polynomial p(t)In on the left by the monic_polynomial
Int â A, while the final equation expresses the fact that the remainder is
zero. This division is performed in the ring of polynomials with matrix
coefficients. Indeed, even over a non-commutative ring, Euclidean division by a
monic polynomial P is defined, and always produces a unique quotient and
remainder with the same degree condition as in the commutative case, provided
it is specified at which side one wishes P to be a factor (here that is to the
left).
To see that quotient and remainder are unique (which is the important part of
the statement here), it suffices to write     P Q + r = P  Q &#x2032;  +  r
&#x2032;    {\displaystyle PQ+r=PQ'+r'}  [PQ+r=PQ'+r'] as     P ( Q &#x2212;  Q
&#x2032;  ) =  r &#x2032;  &#x2212; r   {\displaystyle P(Q-Q')=r'-r}  [P(Q-
Q')=r'-r] and observe that since P is monic, P(QâQ') cannot have a degree
less than that of P, unless Q=Q'.
But the dividend p(t)In and divisor IntâA used here both lie in the subring
(R[A])[t], where R[A] is the subring of the matrix ring M(n, R) generated by A:
the R-linear span of all powers of A. Therefore, the Euclidean division can in
fact be performed within that commutative polynomial ring, and of course it
then gives the same quotient B and remainder 0 as in the larger ring; in
particular this shows that B in fact lies in (R[A])[t].
But, in this commutative setting, it is valid to set t to A in the equation
         p ( t )  I  n   = ( t  I  n   &#x2212; A ) B ;   {\displaystyle p(t)I_
      {n}=(tI_{n}-A)B;}  [{\displaystyle p(t)I_{n}=(tI_{n}-A)B;}]
in other words, to apply the evaluation map
          ev  A   : ( R [ A ] ) [ t ] &#x2192; R [ A ]   {\displaystyle
      \operatorname {ev} _{A}:(R[A])[t]\to R[A]}  [\operatorname {ev} _{A}:(R
      [A])[t]\to R[A]]
which is a ring homomorphism, giving
         p ( A ) = 0 &#x22C5;  ev  A   &#x2061; ( B ) = 0   {\displaystyle p
      (A)=0\cdot \operatorname {ev} _{A}(B)=0}  [p(A)=0\cdot \operatorname {ev}
      _{A}(B)=0]
just like in the second proof, as desired.
In addition to proving the theorem, the above argument tells us that the
coefficients  Bi of B are polynomials in A, while from the second proof we only
knew that they lie in the centralizer Z of A; in general Z is a larger subring
than R[A], and not necessarily commutative. In particular the constant term B0=
adj(âA) lies in R[A]. Since A is an arbitrary square matrix, this proves that
adj(A) can always be expressed as a polynomial in A (with coefficients that
depend on A).
In fact, the equations found in the first proof allow successively expressing
B  n &#x2212; 1   , &#x2026; ,  B  1   ,  B  0     {\displaystyle B_{n-
1},\ldots ,B_{1},B_{0}}  [B_{n-1},\ldots ,B_{1},B_{0}] as polynomials in A,
which leads to the identity
   adj &#x2061; ( &#x2212; A ) =  &#x2211;  i = 1   n    c  i    A  i &#x2212;
1   ,   {\displaystyle \operatorname {adj} (-A)=\sum _{i=1}^{n}c_{i}A^{i-1},}
[\operatorname {adj} (-A)=\sum _{i=1}^{n}c_{i}A^{i-1},]
valid for all nÃn matrices, where
         p ( t ) =  t  n   +  c  n &#x2212; 1    t  n &#x2212; 1   + &#x22EF; +
      c  1   t +  c  0     {\displaystyle p(t)=t^{n}+c_{n-1}t^{n-1}+\cdots +c_
      {1}t+c_{0}}  [{\displaystyle p(t)=t^{n}+c_{n-1}t^{n-1}+\cdots +c_{1}t+c_
      {0}}]
is the characteristic polynomial of A.
Note that this identity also implies the statement of the CayleyâHamilton
theorem: one may move adj(âA) to the right hand side, multiply the resulting
equation (on the left or on the right) by A, and use the fact that
         &#x2212; A &#x22C5; adj &#x2061; ( &#x2212; A ) = adj &#x2061;
      ( &#x2212; A ) &#x22C5; ( &#x2212; A ) = det ( &#x2212; A )  I  n   =  c
      0    I  n   .   {\displaystyle -A\cdot \operatorname {adj} (-
      A)=\operatorname {adj} (-A)\cdot (-A)=\det(-A)I_{n}=c_{0}I_{n}.}  [
      {\displaystyle -A\cdot \operatorname {adj} (-A)=\operatorname {adj} (-
      A)\cdot (-A)=\det(-A)I_{n}=c_{0}I_{n}.}]
See also: FaddeevâLeVerrier_algorithm
**** A proof using matrices of endomorphisms[edit] ****
As was mentioned above, the matrix p(A) in statement of the theorem is obtained
by first evaluating the determinant and then substituting the matrix A for t;
doing that substitution into the matrix     t  I  n   &#x2212; A
{\displaystyle tI_{n}-A}  [tI_{n}-A] before evaluating the determinant is not
meaningful. Nevertheless, it is possible to give an interpretation where p(A)
is obtained directly as the value of a certain determinant, but this requires a
more complicated setting, one of matrices over a ring in which one can
interpret both the entries      A  i , j     {\displaystyle A_{i,j}}  [A_{i,j}]
of A, and all of A itself. One could take for this the ring M(n, R) of nÃn
matrices over R, where the entry      A  i , j     {\displaystyle A_{i,j}}  [A_
{i,j}] is realised as      A  i , j    I  n     {\displaystyle A_{i,j}I_{n}}
[A_{i,j}I_{n}], and A as itself. But considering matrices with matrices as
entries might cause confusion with block_matrices, which is not intended, as
that gives the wrong notion of determinant (recall that the determinant of a
matrix is defined as a sum of products of its entries, and in the case of a
block matrix this is generally not the same as the corresponding sum of
products of its blocks!). It is clearer to distinguish A from the endomorphism
Ï of an n-dimensional vector space V (or free R-module if R is not a field)
defined by it in a basis e1, ..., en, and to take matrices over the ring End(V)
of all such endomorphisms. Then Ï â End(V) is a possible matrix entry, while
A designates the element of M(n, End(V)) whose i,j entry is endomorphism of
scalar multiplication by      A  i , j     {\displaystyle A_{i,j}}  [A_{i,j}];
similarly In will be interpreted as element of M(n, End(V)). However, since End
(V) is not a commutative ring, no determinant is defined on M(n, End(V)); this
can only be done for matrices over a commutative subring of End(V). Now the
entries of the matrix     &#x03C6;  I  n   &#x2212; A   {\displaystyle \varphi
I_{n}-A}  [\varphi I_{n}-A] all lie in the subring R[Ï] generated by the
identity and Ï, which is commutative. Then a determinant map M(n, R[Ï]) â R
[Ï] is defined, and     det ( &#x03C6;  I  n   &#x2212; A )   {\displaystyle
\det(\varphi I_{n}-A)}  [\det(\varphi I_{n}-A)] evaluates to the value p(Ï) of
the characteristic polynomial of A at Ï (this holds independently of the
relation between A and Ï); the CayleyâHamilton theorem states that p(Ï) is
the null endomorphism.
In this form, the following proof can be obtained from that of (Atiyah &
MacDonald 1969, Prop. 2.4) (which in fact is the more general statement related
to the Nakayama_lemma; one takes for the ideal in that proposition the whole
ring R). The fact that A is the matrix of Ï in the basis e1, ..., en means
that
         &#x03C6; (  e  i   ) =  &#x2211;  j = 1   n    A  j , i    e  j
      for&#xA0;  i = 1 , &#x2026; , n .   {\displaystyle \varphi (e_{i})=\sum _
      {j=1}^{n}A_{j,i}e_{j}\quad {\text{for }}i=1,\ldots ,n.}  [\varphi (e_
      {i})=\sum _{j=1}^{n}A_{j,i}e_{j}\quad {\text{for }}i=1,\ldots ,n.]
One can interpret these as n components of one equation in Vn, whose members
can be written using the matrix-vector product M(n, End(V)) Ã Vn â Vn that
is defined as usual, but with individual entries Ï â End(V) and v in V being
"multiplied" by forming     &#x03C8; ( v )   {\displaystyle \psi (v)}  [\psi
(v)]; this gives:
         &#x03C6;  I  n   &#x22C5; E =  A  tr   &#x22C5; E ,   {\displaystyle
      \varphi I_{n}\cdot E=A^{\operatorname {tr} }\cdot E,}  [{\displaystyle
      \varphi I_{n}\cdot E=A^{\operatorname {tr} }\cdot E,}]
where     E &#x2208;  V  n     {\displaystyle E\in V^{n}}  [E\in V^{n}] is the
element whose component i is ei (in other words it is the basis e1, ..., en of
V written as a column of vectors). Writing this equation as
         ( &#x03C6;  I  n   &#x2212;  A  tr   ) &#x22C5; E = 0 &#x2208;  V  n
      {\displaystyle (\varphi I_{n}-A^{\operatorname {tr} })\cdot E=0\in V^{n}}
      [{\displaystyle (\varphi I_{n}-A^{\operatorname {tr} })\cdot E=0\in V^
      {n}}]
one recognizes the transpose of the matrix     &#x03C6;  I  n   &#x2212; A
{\displaystyle \varphi I_{n}-A}  [\varphi I_{n}-A] considered above, and its
determinant (as element of M(n, R[Ï])) is also p(Ï). To derive from this
equation that p(Ï) = 0 â End(V), one left-multiplies by the adjugate_matrix
of     &#x03C6;  I  n   &#x2212;  A  tr     {\displaystyle \varphi I_{n}-A^
{\operatorname {tr} }}  [{\displaystyle \varphi I_{n}-A^{\operatorname {tr}
}}], which is defined in the matrix ring M(n, R[Ï]), giving
             0    = adj &#x2061; ( &#x03C6;  I  n   &#x2212;  A  tr   )
      &#x22C5; ( ( &#x03C6;  I  n   &#x2212;  A  tr   ) &#x22C5; E )       =
      ( adj &#x2061; ( &#x03C6;  I  n   &#x2212;  A  tr   ) &#x22C5; ( &#x03C6;
      I  n   &#x2212;  A  tr   ) ) &#x22C5; E       = ( det ( &#x03C6;  I  n
      &#x2212;  A  tr   )  I  n   ) &#x22C5; E       = ( p ( &#x03C6; )  I  n
      ) &#x22C5; E ;       {\displaystyle {\begin{aligned}0&=\operatorname
      {adj} (\varphi I_{n}-A^{\operatorname {tr} })\cdot ((\varphi I_{n}-A^
      {\operatorname {tr} })\cdot E)\\&=(\operatorname {adj} (\varphi I_{n}-A^
      {\operatorname {tr} })\cdot (\varphi I_{n}-A^{\operatorname {tr} }))\cdot
      E\\&=(\det(\varphi I_{n}-A^{\operatorname {tr} })I_{n})\cdot E\\&=(p
      (\varphi )I_{n})\cdot E;\end{aligned}}}  [{\displaystyle {\begin
      {aligned}0&=\operatorname {adj} (\varphi I_{n}-A^{\operatorname {tr}
      })\cdot ((\varphi I_{n}-A^{\operatorname {tr} })\cdot E)\\&=
      (\operatorname {adj} (\varphi I_{n}-A^{\operatorname {tr} })\cdot
      (\varphi I_{n}-A^{\operatorname {tr} }))\cdot E\\&=(\det(\varphi I_{n}-A^
      {\operatorname {tr} })I_{n})\cdot E\\&=(p(\varphi )I_{n})\cdot E;\end
      {aligned}}}]
the associativity of matrix-matrix and matrix-vector multiplication used in the
first step is a purely formal property of those operations, independent of the
nature of the entries. Now component i of this equation says that p(Ï)(ei) = 0
â V; thus p(Ï) vanishes on all ei, and since these elements generate V it
follows that p(Ï) = 0 â End(V), completing the proof.
One additional fact that follows from this proof is that the matrix A whose
characteristic polynomial is taken need not be identical to the value Ï
substituted into that polynomial; it suffices that Ï be an endomorphism of V
satisfying the initial equations
         &#x03C6; (  e  i   ) =  &#x2211;  j    A  j , i    e  j
      {\displaystyle \varphi (e_{i})=\sum _{j}A_{j,i}e_{j}}  [\varphi (e_
      {i})=\sum _{j}A_{j,i}e_{j}]
for some sequence of elements e1,...,en that generate V (which space might have
smaller dimension than n, or in case the ring R is not a field it might not be
a free_module at all).
**** A bogus "proof": p(A) = det(AIn â A) = det(A â A) = 0[edit] ****
One persistent elementary but incorrect argument[18] for the theorem is to
"simply" take the definition
         p ( &#x03BB; ) = det ( &#x03BB;  I  n   &#x2212; A )   {\displaystyle
      p(\lambda )=\det(\lambda I_{n}-A)}  [p(\lambda )=\det(\lambda I_{n}-A)]
and substitute A for Î», obtaining
         p ( A ) = det ( A  I  n   &#x2212; A ) = det ( A &#x2212; A ) = 0
      &#xA0; .   {\displaystyle p(A)=\det(AI_{n}-A)=\det(A-A)=0~.}  [
      {\displaystyle p(A)=\det(AI_{n}-A)=\det(A-A)=0~.}]
There are many ways to see why this argument is wrong. First, in
CayleyâHamilton theorem, p(A) is an nÃn matrix. However, the right hand side
of the above equation is the value of a determinant, which is a scalar. So they
cannot be equated unless n = 1 (i.e. A is just a scalar). Second, in the
expression     det ( &#x03BB;  I  n   &#x2212; A )   {\displaystyle \det
(\lambda I_{n}-A)}  [\det(\lambda I_{n}-A)], the variable Î» actually occurs at
the diagonal entries of the matrix     &#x03BB;  I  n   &#x2212; A
{\displaystyle \lambda I_{n}-A}  [\lambda I_{n}-A]. To illustrate, consider the
characteristic polynomial in the previous example again:
         det   (    &#x03BB; &#x2212; 1   &#x2212; 2     &#x2212; 3   &#x03BB;
      &#x2212; 4    )   .   {\displaystyle \det {\begin{pmatrix}\lambda -1&-
      2\\-3&\lambda -4\end{pmatrix}}.}  [\det {\begin{pmatrix}\lambda -1&-2\\-
      3&\lambda -4\end{pmatrix}}.]
If one substitutes the entire matrix A for Î» in those positions, one obtains
         det   (      (    1   2     3   4    )   &#x2212; 1   &#x2212; 2
      &#x2212; 3     (    1   2     3   4    )   &#x2212; 4    )   ,
      {\displaystyle \det {\begin{pmatrix}{\begin{pmatrix}1&2\\3&4\end
      {pmatrix}}-1&-2\\-3&{\begin{pmatrix}1&2\\3&4\end{pmatrix}}-4\end
      {pmatrix}},}  [\det {\begin{pmatrix}{\begin{pmatrix}1&2\\3&4\end
      {pmatrix}}-1&-2\\-3&{\begin{pmatrix}1&2\\3&4\end{pmatrix}}-4\end
      {pmatrix}},]
in which the "matrix" expression is simply not a valid one. Note, however, that
if scalar multiples of identity matrices instead of scalars are subtracted in
the above, i.e. if the substitution is performed as
         det   (      (    1   2     3   4    )   &#x2212;  I  2     &#x2212; 2
      I  2       &#x2212; 3  I  2       (    1   2     3   4    )   &#x2212; 4
      I  2      )   ,   {\displaystyle \det {\begin{pmatrix}{\begin
      {pmatrix}1&2\\3&4\end{pmatrix}}-I_{2}&-2I_{2}\\-3I_{2}&{\begin
      {pmatrix}1&2\\3&4\end{pmatrix}}-4I_{2}\end{pmatrix}},}  [\det {\begin
      {pmatrix}{\begin{pmatrix}1&2\\3&4\end{pmatrix}}-I_{2}&-2I_{2}\\-3I_{2}&
      {\begin{pmatrix}1&2\\3&4\end{pmatrix}}-4I_{2}\end{pmatrix}},]
then the determinant is indeed zero, but the expanded matrix in question does
not evaluate to     A  I  n   &#x2212; A   {\displaystyle AI_{n}-A}  [AI_{n}-
A]; nor can its determinant (a scalar) be compared to p(A) (a matrix). So the
argument that     p ( A ) = det ( A  I  n   &#x2212; A ) = 0   {\displaystyle p
(A)=\det(AI_{n}-A)=0}  [p(A)=\det(AI_{n}-A)=0] still does not apply.
Actually, if such an argument holds, it should also hold when other multilinear
forms instead of determinant is used. For instance, if we consider the
permanent function and define     q ( &#x03BB; ) = perm &#x2061; ( &#x03BB;  I
n   &#x2212; A )   {\displaystyle q(\lambda )=\operatorname {perm} (\lambda I_
{n}-A)}  [q(\lambda )=\operatorname {perm} (\lambda I_{n}-A)], then by the same
argument, we should be able to "prove" that q(A) = 0. But this statement is
demonstrably wrong. In the 2-dimensional case, for instance, the permanent of a
matrix is given by
         perm &#x2061;   (    a   b     c   d    )   = a d + b c .
      {\displaystyle \operatorname {perm} {\begin{pmatrix}a&b\\c&d\end
      {pmatrix}}=ad+bc.}  [\operatorname {perm} {\begin{pmatrix}a&b\\c&d\end
      {pmatrix}}=ad+bc.]
So, for the matrix A in the previous example,
             q ( &#x03BB; )    = perm &#x2061; ( &#x03BB;  I  2   &#x2212; A )
      = perm &#x2061;   (    &#x03BB; &#x2212; 1   &#x2212; 2     &#x2212; 3
      &#x03BB; &#x2212; 4    )         = ( &#x03BB; &#x2212; 1 ) ( &#x03BB;
      &#x2212; 4 ) + ( &#x2212; 2 ) ( &#x2212; 3 ) =  &#x03BB;  2   &#x2212; 5
      &#x03BB; + 10.       {\displaystyle {\begin{aligned}q(\lambda
      )&=\operatorname {perm} (\lambda I_{2}-A)=\operatorname {perm} {\begin
      {pmatrix}\lambda -1&-2\\-3&\lambda -4\end{pmatrix}}\\[6pt]&=(\lambda -1)
      (\lambda -4)+(-2)(-3)=\lambda ^{2}-5\lambda +10.\end{aligned}}}  [
      {\displaystyle {\begin{aligned}q(\lambda )&=\operatorname {perm} (\lambda
      I_{2}-A)=\operatorname {perm} {\begin{pmatrix}\lambda -1&-2\\-3&\lambda -
      4\end{pmatrix}}\\[6pt]&=(\lambda -1)(\lambda -4)+(-2)(-3)=\lambda ^{2}-
      5\lambda +10.\end{aligned}}}]
Yet one can verify that
         q ( A ) =  A  2   &#x2212; 5 A + 10  I  2   = 12  I  2   &#x2260; 0.
      {\displaystyle q(A)=A^{2}-5A+10I_{2}=12I_{2}\not =0.}  [q(A)=A^{2}-
      5A+10I_{2}=12I_{2}\not =0.]
One of the proofs for CayleyâHamilton theorem above bears some similarity to
the argument that     p ( A ) = det ( A  I  n   &#x2212; A ) = 0
{\displaystyle p(A)=\det(AI_{n}-A)=0}  [p(A)=\det(AI_{n}-A)=0]. By introducing
a matrix with non-numeric coefficients, one can actually let A live inside a
matrix entry, but then     A  I  n     {\displaystyle AI_{n}}  [AI_{n}] is not
equal to A, and the conclusion is reached differently.
***** Proofs using methods of abstract algebra[edit] *****
Basic properties of HasseâSchmidt_derivations on the exterior_algebra     A =
&#x22C0; M   {\displaystyle A=\bigwedge M}  [{\displaystyle A=\bigwedge M}] of
some B-module M (supposed to be free and of finite rank) have been used by
Gatto_&_Salehyan_(2016, Â§4) to prove the CayleyâHamilton theorem.
***** Abstraction and generalizations[edit] *****
The above proofs show that the CayleyâHamilton theorem holds for matrices
with entries in any commutative ring R, and that p(Ï) = 0 will hold whenever
Ï is an endomorphism of an R module generated by elements e1,...,en that
satisfies
         &#x03C6; (  e  j   ) = &#x2211;  a  i j    e  i   ,  j = 1 , &#x2026;
      , n .   {\displaystyle \varphi (e_{j})=\sum a_{ij}e_{i},\qquad j=1,\ldots
      ,n.}  [{\displaystyle \varphi (e_{j})=\sum a_{ij}e_{i},\qquad j=1,\ldots
      ,n.}]
This more general version of the theorem is the source of the celebrated
Nakayama_lemma in commutative algebra and algebraic geometry.
***** See also[edit] *****
    * Companion_matrix
***** Remarks[edit] *****
   1. ^ Due to the non-commutative nature of the multiplication operation for
      quaternions and related constructions, care needs to be taken with
      definitions, most notably in this context, for the determinant. The
      theorem holds as well for the slightly less well-behaved split-
      quaternions, see AlagÃ¶s,_Oral_&_YÃ¼ce_(2012). The rings of quaternions
      and split-quaternions can both be represented by certain 2 Ã 2 complex
      matrices. (When restricted to unit norm, these are the groups SU(2) and
      SU(1, 1) respectively.) Therefore it is not surprising that the theorem
      holds.


      There is no such matrix representation for the octonions, since the
      multiplication operation is not associative in this case. However, a
      modified CayleyâHamilton theorem still holds for the octonions, see
      Tian_(2000).
   2. ^ An explicit expression for these coefficients is
                c  i   =  &#x2211;   k  1   ,  k  2   , &#x2026; ,  k  n
            &#x220F;  l = 1   n      ( &#x2212; 1  )   k  l   + 1      l   k  l
            k  l   !    tr &#x2061; (  A  l    )   k  l     ,   {\displaystyle
            c_{i}=\sum _{k_{1},k_{2},\ldots ,k_{n}}\prod _{l=1}^{n}{\frac {(-
            1)^{k_{l}+1}}{l^{k_{l}}k_{l}!}}\operatorname {tr} (A^{l})^{k_{l}},}
            [{\displaystyle c_{i}=\sum _{k_{1},k_{2},\ldots ,k_{n}}\prod _
            {l=1}^{n}{\frac {(-1)^{k_{l}+1}}{l^{k_{l}}k_{l}!}}\operatorname
            {tr} (A^{l})^{k_{l}},}]
      where the sum is taken over the sets of all integer partitions kl â¥ 0
      satisfying the equation
                &#x2211;  l = 1   n   l  k  l   = n &#x2212; i .
            {\displaystyle \sum _{l=1}^{n}lk_{l}=n-i.}  [{\displaystyle \sum _
            {l=1}^{n}lk_{l}=n-i.}]
   3. ^ See, e.g., p. 54 of Brown_1994, which solves Jacobi's_formula,
               &#x2202; p ( &#x03BB; )  /  &#x2202; &#x03BB; = p ( &#x03BB; )
            &#x2211;  m = 0   &#x221E;    &#x03BB;  &#x2212; ( m + 1 )   tr
            &#x2061;  A  m   = p ( &#x03BB; ) &#xA0; tr &#x2061;   I  &#x03BB;
            I &#x2212; A    &#x2261; tr &#x2061; B &#xA0; ,   {\displaystyle
            \partial p(\lambda )/\partial \lambda =p(\lambda )\sum _{m=0}^
            {\infty }\lambda ^{-(m+1)}\operatorname {tr} A^{m}=p(\lambda
            )~\operatorname {tr} {\frac {I}{\lambda I-A}}\equiv \operatorname
            {tr} B~,}  [\partial p(\lambda )/\partial \lambda =p(\lambda )\sum
            _{m=0}^{\infty }\lambda ^{-(m+1)}\operatorname {tr} A^{m}=p(\lambda
            )~\operatorname {tr} {\frac {I}{\lambda I-A}}\equiv \operatorname
            {tr} B~,]
      where B is the adjugate matrix of the next section. There also exists an
      equivalent, related recursive algorithm introduced by Urbain_Le_Verrier
      and Dmitry_Konstantinovich_Faddeevâthe FaddeevâLeVerrier_algorithm,
      which reads
                    M  0      &#x2261; O    c  n      = 1    ( k = 0 )      M
            k      &#x2261; A  M  k &#x2212; 1   &#x2212;   1  k &#x2212; 1
            ( tr &#x2061; ( A  M  k &#x2212; 1   ) ) I      c  n &#x2212; k
            = &#x2212;   1 k   tr &#x2061; ( A  M  k   )    k = 1 , &#x2026; ,
            n &#xA0; .       {\displaystyle {\begin{aligned}M_{0}&\equiv O&c_
            {n}&=1\qquad &(k=0)\\[5pt]M_{k}&\equiv AM_{k-1}-{\frac {1}{k-1}}
            (\operatorname {tr} (AM_{k-1}))I\qquad \qquad &c_{n-k}&=-{\frac {1}
            {k}}\operatorname {tr} (AM_{k})\qquad &k=1,\ldots ,n~.\end
            {aligned}}}  [{\displaystyle {\begin{aligned}M_{0}&\equiv O&c_
            {n}&=1\qquad &(k=0)\\[5pt]M_{k}&\equiv AM_{k-1}-{\frac {1}{k-1}}
            (\operatorname {tr} (AM_{k-1}))I\qquad \qquad &c_{n-k}&=-{\frac {1}
            {k}}\operatorname {tr} (AM_{k})\qquad &k=1,\ldots ,n~.\end
            {aligned}}}]
      (see, e.g., p 88 of Gantmacher_1960.) Observe Aâ1 = âMn /c0 as the
      recursion terminates. See the algebraic proof in the following section,
      which relies on the modes of the adjugate, Bk â¡ Mnâk .  
      Specifically,     ( &#x03BB; I &#x2212; A ) B = I p ( &#x03BB; )
      {\displaystyle (\lambda I-A)B=Ip(\lambda )}  [(\lambda I-A)B=Ip(\lambda
      )] and the above derivative of p when one traces it yields
               &#x03BB;  p &#x2032;  &#x2212; n p = tr &#x2061; ( A B ) &#xA0;
            ,   {\displaystyle \lambda p'-np=\operatorname {tr} (AB)~,}  [
            {\displaystyle \lambda p'-np=\operatorname {tr} (AB)~,}] (Hou
            1998), and the above recursions, in turn.
***** Notes[edit] *****
   1. ^ a b Crilly_1998
   2. ^ a b Cayley_1858, pp. 17â37
   3. ^ Cayley_1889, pp. 475â496
   4. ^ a b Hamilton_1864a
   5. ^ a b Hamilton_1864b
   6. ^ a b Hamilton_1862
   7. ^ Atiyah_&_MacDonald_1969
   8. ^ Hamilton_1853, p. 562
   9. ^ Zhang_1997
  10. ^ a b Frobenius_1878
  11. ^ Zeni_&_Rodrigues_1992
  12. ^ Barut,_Zeni_&_Laufer_1994a
  13. ^ Barut,_Zeni_&_Laufer_1994b
  14. ^ Laufer_1997
  15. ^ Curtright,_Fairlie_&_Zachos_2014
  16. ^Stein, William. Algebraic_Number_Theory,_a_Computational_Approach (PDF).
      p. 29.
  17. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
  18. ^ Bhatia_1997, p. 7
  19. ^ Garrett,_2007_&_p._381
***** References[edit] *****
    * AlagÃ¶s, Y.; Oral, K.; YÃ¼ce, S. (2012). "Split Quaternion Matrices".
      Miskolc Mathematical Notes. 13 (2): 223â232. doi:10.18514/MMN.2012.364.
      ISSN 1787-2405
 (open access)
Atiyah,_M._F.; MacDonald,_I._G. (1969), Introduction to Commutative Algebra,
Westview Press, ISBN 978-0-201-40751-8
Barut,_A._O.; Zeni, J. R.; Laufer, A. (1994a). "The_exponential_map_for_the
conformal_group_O(2,4)". J. Phys. A: Math. Gen. 27 (15): 5239â5250. arXiv:
hep-th/9408105. Bibcode:1994JPhA...27.5239B. doi:10.1088/0305-4470/27/15/022.
Barut,_A._O.; Zeni, J. R.; Laufer, A. (1994b). "The_exponential_map_for_the
unitary_group_SU(2,2)". J. Phys. A: Math. Gen. 27 (20): 6799â6806. arXiv:hep-
th/9408145. Bibcode:1994JPhA...27.6799B. doi:10.1088/0305-4470/27/20/017.
Bhatia, R. (1997). Matrix Analysis. Graduate texts in mathematics. 169.
Springer. ISBN 978-0387948461.
Brown, Lowell S. (1994). Quantum Field Theory. Cambridge_University_Press.
ISBN 978-0-521-46946-3.
Cayley,_A. (1858). "A Memoir on the Theory of Matrices". Philos. Trans. 148.
Cayley, A. (1889). The Collected Mathematical Papers of Arthur Cayley. (Classic
Reprint). 2. Forgotten books. ASIN B008HUED9O.
Crilly, T. (1998). "The young Arthur Cayley". Notes Rec. R. Soc. Lond. 52 (2):
267â282. doi:10.1098/rsnr.1998.0050.
Curtright,_T_L; Fairlie,_D_B; Zachos,_C_K (2014). "A compact formula for
rotations as spin matrix polynomials". SIGMA. 10 (2014): 084. arXiv:1402.3541.
Bibcode:2014SIGMA..10..084C. doi:10.3842/SIGMA.2014.084.
Frobenius,_G. (1878). "Ueber lineare Substutionen und bilineare Formen". J.
Reine Angew. Math. 1878 (84): 1â63. doi:10.1515/crll.1878.84.1.
Gantmacher, F.R. (1960). The Theory of Matrices. NY: Chelsea Publishing.
ISBN 978-0-8218-1376-8.
    * Gatto, Letterio; Salehyan, Parham (2016), HasseâSchmidt derivations on
      Grassmann algebras, Springer, doi:10.1007/978-3-319-31842-4, ISBN 978-3-
      319-31842-4, MR 3524604
    * Garrett, Paul B. (2007). Abstract Algebra. NY: Chapman and Hall/CRC.
      ISBN 978-1584886891.
Hamilton,_W._R. (1853). Lectures on Quaternions. Dublin.
Hamilton, W. R. (1864a). "On a New and General Method of Inverting a Linear and
Quaternion Function of a Quaternion". Proceedings_of_the_Royal_Irish_Academy.
viii: 182â183.
 (communicated on June 9, 1862)
Hamilton, W. R. (1864b). "On the Existence of a Symbolic and Biquadratic
Equation, which is satisfied by the Symbol of Linear Operation in Quaternions".
Proceedings_of_the_Royal_Irish_Academy. viii: 190â101.
 (communicated on June 23, 1862)
Hou, S. H. (1998). "Classroom Note: A Simple Proof of the Leverrier--Faddeev
Characteristic Polynomial Algorithm". SIAM Review. 40 (3): 706â709. Bibcode:
1998SIAMR..40..706H. doi:10.1137/S003614459732076X.
 "Classroom_Note:_A_Simple_Proof_of_the_Leverrier--Faddeev_Characteristic
Polynomial_Algorithm"
Hamilton, W. R. (1862). "On_the_Existence_of_a_Symbolic_and_Biquadratic
Equation_which_is_satisfied_by_the_Symbol_of_Linear_or_Distributive_Operation
on_a_Quaternion". The_London,_Edinburgh,_and_Dublin_Philosophical_Magazine_and
Journal_of_Science. series iv. 24: 127â128. ISSN 1478-6435. Retrieved 2015-
02-14.
Householder,_Alston_S. (2006). The Theory of Matrices in Numerical Analysis.
Dover Books on Mathematics. ISBN 978-0486449722.
Laufer, A. (1997). "The_exponential_map_of_GL(N)". J. Phys. A: Math. Gen. 30
(15): 5455â5470. arXiv:hep-th/9604049. Bibcode:1997JPhA...30.5455L. doi:
10.1088/0305-4470/30/15/029.
Tian, Y. (2000). "Matrix representations of octonions and their application".
Advances_in_Applied_Clifford_Algebras. 10 (1): 61â90. arXiv:math/0003166.
CiteSeerX 10.1.1.237.2217. doi:10.1007/BF03042010. ISSN 0188-7009.
Zeni, J. R.; Rodrigues, W.A. (1992). "A thoughful study of Lorentz
transformations by Clifford algebras". Int. J. Mod. Phys. A. 7 (8): 1793 pp.
Bibcode:1992IJMPA...7.1793Z. doi:10.1142/S0217751X92000776.
Zhang, F. (1997). "Quaternions and matrices of quaternions". Linear Algebra and
Its Applications. 251: 21â57. doi:10.1016/0024-3795(95)00543-9. ISSN 0024-
3795
 (open archive).
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "CayleyâHamilton_theorem",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
A_proof_from_PlanetMath.
The_CayleyâHamilton_theorem_at_MathPages

Retrieved from "https://en.wikipedia.org/w/
index.php?title=CayleyâHamilton_theorem&oldid=909225419"
Categories:
    * Theorems_in_linear_algebra
    * Matrix_theory
    * William_Rowan_Hamilton
Hidden categories:
    * Articles_containing_proofs
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
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Hrvatski
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * ä¸­æ
Edit_links
    * This page was last edited on 4 August 2019, at 00:30 (UTC).
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
